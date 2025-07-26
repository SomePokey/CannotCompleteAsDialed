# CannotCompleteAsDialed
Custom FreePBX dialplan that allows for your voice to say "your call cannot be completed as dialed"

This works by the system setting the language for that specific call to a custom language folder (in this case /var/lib/asterisk/sounds/en-custom) and playing a file from that folder. It then hangs up with the cause code of 1, which is Asterisk's way of telling you the number you just dialed is unallocated.
