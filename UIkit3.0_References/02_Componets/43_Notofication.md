Notification
Create toggleable notifications that fade out automatically.

Usage
The notification will not fade out but remain visible when you hover the message until you stop hovering. You can also close the notification by clicking it. To show notifications, the component provides a simple JavaScript API. The following code snippet gets you started.

JavaScript
UIkit.notification({
    message: 'my-message!',
    status: 'primary',
    pos: 'top-right',
    timeout: 5000
});

// Shortcuts
UIkit.notification('My message');
UIkit.notification('My message', status);
UIkit.notification('My message', { /* options */ });
PREVIEW
MARKUP
CLICK ME
HTML message
You can use HTML inside your notification message, like an icon from the Icon component.

UIkit.notification("<span uk-icon='icon: check'></span> Message");
PREVIEW
MARKUP
WITH ICON
Position
Add one of the following parameters to adjust the notification's position to different corners.

UIkit.notification("...", {pos: 'top-right'})
POSITION	CODE
top-left	UIkit.notification("...", {pos: 'top-left'})
top-center	UIkit.notification("...", {pos: 'top-center'})
top-right	UIkit.notification("...", {pos: 'top-right'})
bottom-left	UIkit.notification("...", {pos: 'bottom-left'})
bottom-center	UIkit.notification("...", {pos: 'bottom-center'})
bottom-right	UIkit.notification("...", {pos: 'bottom-right'})
PREVIEW
MARKUP
TOP LEFT  TOP CENTER  TOP RIGHT  BOTTOM LEFT BOTTOM CENTER  BOTTOM RIGHT

Style
A notification can be styled by adding a status to the message to indicate a primary, success, warning or a danger status.

UIkit.notification("...", {status: 'primary'})
STYLE	CODE
primary	UIkit.notification("...", {status:'primary'})
success	UIkit.notification("...", {status:'success'})
warning	UIkit.notification("...", {status:'warning'})
danger	UIkit.notification("...", {status:'danger'})
PREVIEW
MARKUP
PRIMARY  SUCCESS  WARNING  DANGER

Close all
You can close all open notifications by calling UIkit.notification.closeAll().

PREVIEW
MARKUP
CLOSE ALL
Component options
Any of these options can be applied to the component attribute. Separate multiple options with a semicolon. Learn more

OPTION	VALUE	DEFAULT	DESCRIPTION
message	String	false	Notification message to show.
status	String	null	Notification status color.
timeout	Integer	5000	Visibility duration until a notification disappears.
group	String	null	Useful, if you want to close all notifications in a specific group.
pos	String	top-center	Display corner.
JavaScript
Learn more about JavaScript components.

Initialization
This is a Functional Component and may omit the element argument.

UIkit.notification(options);
UIkit.notification(message, status);
Events
The following events will be triggered on elements with this component attached:

NAME	DESCRIPTION
close	Fires after the notification has been closed.
Methods
The following methods are available for the component:

Close
UIkit.notification(element).close(immediate);
Closes the notification.

NAME	TYPE	DEFAULT	DESCRIPTION
immediate	Boolean	true	Transition the notification out.
