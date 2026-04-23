# Daria_Ishchuk
import random
import string

def generate_password(length, use_digits, use_letters, use_special):
    chars = ''
    if use_letters:
        chars += string.ascii_letters
    if use_digits:
        chars += string.digits
    if use_special:
        chars += string.punctuation
    return ''.join(random.choices(chars, k=length))
    
