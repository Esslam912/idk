def encode(message, shift=caesar_shift):
    encoded_message = ''
    for i in range(len(message)):
        letter = message[i]
        letter_code = ord(letter)
        shifted_code = letter_code + shift
        if (shifted_code > 122 and letter.islower()) or (shifted_code > 90 and letter.isupper()):
            shifted_code -= 26
        encoded_message += chr(shifted_code)
    return encoded_message

def decode(message, shift=caesar_shift):
    decoded_message = ''
    for i in range(len(message)):
        letter = message[i]
        letter_code = ord(letter)
        shifted_code = letter_code - shift
        if (letter.islower() and shifted_code < 96) or (letter.isupper() and shifted_code < 65):
            shifted_code += 26
        decoded_message += chr(shifted_code)
    return decoded_message    
