I started off by trying to make an image carousel that would just show one picture at a time using downloaded pictures. Once this worked, I looked up how to place images side by side in order to show 6 pictures at a time. When I did this, I got rid of the </li> <li> between the pictures and this caused the left and right buttons to not work. I looked in my js file and saw that it included 'li' so I realized this needed to be part of the html code in order for the buttons to work.

After I figured out how to place 6 pictures at a time, I tried to work on calling the API.
I imagine that a code like this would be placed in the js file: 
$.ajax({
    url: 'http://http://z1photorankapi-a.akamaihd.net/customers/215757/streams',
    type: ‘GET’,
    data: ‘authtoken=0a40a13fd9d531110b4d6515ef0d6c529acdb59e81194132356a1b8903790c18&version=v2.2’
    success: function(x) { alert(x); }
});
But I could not figure out how to make the img src in the html pull from the API dynamically. I ended up looking through the API code for the links to the images and hard coded them into the html. 
