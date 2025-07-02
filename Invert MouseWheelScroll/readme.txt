Invert MouseWheelScroll;

This setting inverts the mousewheel scroll.
So, for as long as it is active, mousewheelup becomes mousewheeldown and mousewheeldown becomes mousewheelup.

It is the correct way of doing it.


Computer\HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Enum\HID\VID_???\???\Device Parameters
"FlipFlopWheel"=dword:00000001


Tested to work with Win11 24H2

What is it useful for?
It may be useful for wanting to reverse the controls of certain hardcoded mousewheel directions in certain applications or video games.

The HID\VID_ code may be different on your computer.

There is also a way to invert horizontal scrolling with:

"FlipFlopHScroll"=dword:00000001
	(Changed from the default "FlipFlopHScroll"=dword:00000000)
