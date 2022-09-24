from extras import alphabet, logo

print(logo)
run = True
while run:
        direction = input("Type 'encode' to encrypt, type 'decode' to decrypt:\n")
        text = input("Type your message:\n").lower()
        shift = int(input("Type the shift number:\n"))
        shift = shift%26
        def ceaser(text, shift_number, direction):
                    if direction == 'encode':
                        encode = ''
                        for letter in text:
                            if letter in alphabet:
                                index = alphabet.index(letter)
                                encode += alphabet[index+shift_number]
                            else:
                                encode += letter
                        print(f'Your encoded text is {encode}')
                    elif direction == 'decode':
                        decode = ''
                        for letter in text:
                            if letter in alphabet:
                                index = alphabet.index(letter)
                                decode += alphabet[index-shift_number]
                            else:
                                decode += letter
                        print(f'Your decoded text is {decode}')
        ceaser(text=text, shift_number=shift, direction=direction)
        restart = input('If the user want to restart the cipher program? ').lower()
        if restart == 'yes':
            run = True
        elif restart == 'no':
            run = False
