
Select the element that contains the profile image (hint: look for the class). Change the src attribute so it points to a picture of your choosing instead (hint: use attr()).
PROTIP: use the inspector to learn the dimensions of the current profile image and use a placeholder image service such as Place Bear to get an image of the same size.
    $('img.profile-image').attr('src', 'https://placebear.com/400/400')


Use the same approach to select the element that contains the photo of the sky and change the src attribute to another picture URL of your choosing.
    $('img.photography').attr('src', 'https://placebear.com/325/225')


Select the heading that says "Panda the Bear" and change it to your own name. (hint: use text())
    $('h1.highlight').text('Lauren Rosentzveig')


Select the heading that says "Employment" and change it to something else. (hint: use a descendant selector)
    $('div#employment > h3').html('<i class="icon-suitcase"></i> &nbsp; Experience')

Panda the Bear is lying about their skills! Take the "time travel" skill off the page to satisfy your personal sense of justice. Use your googling and docs-skimming skillz to find a jQuery function that will allow you to remove elements from the DOM. (hint: there are multiple ways of doing this, but the parent() function might be useful when it comes to selecting the right element)
    $('div#time-travel.bar-filled.highlight').parent().remove();

Change the colour of the body. (hint: use css())
    $('body').css('background-color', 'darkgoldenrod')

Change the colour used by the highlight class.
    $('.highlight').css('background-color', 'indigo')

Change the font family of the h1 to 'monospace'.
    $('h1').css('font-family', 'monospace')

Find a way to select the round icons in the sidebar and then change their colour.
    $('a.action-icon-bg').css('background-color', 'darkblue')

Scroll down to the contact form. Change the placeholder attribute of the name field to "identify yourself".
    $('input#name').attr('placeholder', "Identify Yourself")

Change the placeholder attribute of the message field to "state your business".
    $('textarea#message').attr('placeholder', 'State Your Business')

Give the name field a "value" attribute of "your nemesis".
    $('input#name').attr('value', "Your Nemesis")

Change the value attribute of the email field to "koalathebear@gmail.com".
    $('input#email').attr('value', "koalathebear@gmail.com")

Change the value of the submit button on the contact form to "En garde!".
    $('input#submit').attr('value', "En garde!")

Bonus points: try experimenting with both the attr() function and the val() function to find different ways of doing this.

We should stop Koala from sending an email to Panda that they might regret! Find a way to disable the submit button (hint: familiarize yourself with the disabled attribute).
    $('input#submit').prop('disabled', true)

We should help Panda protect their privacy by clearing their personal details from the sidebar. You can use empty() to do this.
    $('ul.bio-info').empty()
