1.  Select the element that contains the profile image.
Change the src attribute so it points to a picture of
your choosing instead.

  => profile = document.querySelector('.profile-image')
  => profile.src = "images/clouds-man.jpg"

2.  Use the same approach to select the element that
contains the photo of the sky and change the src
attribute to another picture URL of your choosing.

  => leftImage = document.querySelector('#left-image.portfolio-image img')
  => leftImage.src = "images/pikachu-drawing.jpg"

3.  Select the heading that says "Panda the Bear" and
change it to your own name.

  => heading = document.querySelector('h1.highlight')
  => heading.innerText = 'Don Cooper'

4.  Select the heading that says "Employment" and change
it to something else.

  => employment = document.querySelector('#employment h3.info-title')
  => employment.innerText = 'Napping'

5.  Change the colour of the body.

  => mainSection = document.querySelector('body')
  => mainSection.style.backgroundColor = 'white'

6.  Change the colour used by the highlight class.

  => featured = document.querySelectorAll('.highlight')
  => featured.forEach(function(item) { item.style.color = 'purple'})

7.  Change the font family of the h1 to 'monospace'.

  => heading = document.querySelectorAll('h1')
  => heading.forEach(function(item) { item.style.fontFamily = 'monospace' })

8.  Find a way to select the round icons in the sidebar
and then change their colour.

  => icon = document.querySelectorAll('a.action-icon-bg')
  => icon.forEach(function(item) { item.style.backgroundColor = 'blue' })

9.  Scroll down to the contact form. Change the placeholder
attribute of the name field to "identify yourself".

  => nameField = document.querySelector('input#name.contact-info')
  => nameField.placeholder = 'identify yourself'

10.  Change the placeholder attribute of the message field
to "state your business".

  => messageField = document.querySelector('textarea#message')
  => messageField.placeholder = 'state your business'

11.  Give the name field a "value" attribute of "your nemesis".

  => nameField = document.querySelector('input#name.contact-info')
  => nameField.value = 'your nemesis'

12.  Change the value attribute of the email field to
"koalathebear@gmail.com"

  => emailField = document.querySelector('input#email.contact-info')
  => emailField.value = 'koalathebear@gmail.com'

13.  Change the value of the submit button on the contact form
to "En garde!".

  => submitButton = document.querySelector('input#submit')
  => submitButton.value = 'En garde!'

14.  Find a way to disable the submit button

  => submitButton = document.querySelector('input#submit')
  => submitButton.disabled = 'disabled'

15.  We should help Panda protect their privacy by clearing
their personal details from the sidebar.

  => form = document.querySelector('form')
  => reset = form.reset()


/////  PART 2  /////

1.  Panda the Bear is lying about their skills! Take the "time
travel" skill off the page

  => skills = document.querySelectorAll('.bar-default')[2]
  => timeTravel = document.querySelector('#time-travel')
  => skills.removeChild(timeTravel)

2.  That drawing of Pikachu is really cute. Let’s duplicate it using cloneNode() and insert it at the bottom of the .portfolio-container

  => portfolio = document.querySelector('.portfolio-container')
  => image = document.querySelector('.profile-image').cloneNode()
  => portfolio.appendChild(image)

3.  Wow, that was so satisfying I think we should do it 10 more
times. Use a for loop to help you do this.

  => 
