def encrypt(text):
    encrypted_text = ""
    for char in text:
        # يقوم بتحويل كل حرف إلى الحرف التالي في الترتيب الأبجدي
        if char.isalpha():  # يتأكد مما إذا كان الحرف حرفًا
            if char == 'z':
                encrypted_text += 'a'  # يعيد الحرف 'z' إلى 'a'
            elif char == 'Z':
                encrypted_text += 'A'  # يعيد الحرف 'Z' إلى 'A'
            else:
                # يضيف الحرف التالي في الترتيب الأبجدي
                encrypted_text += chr(ord(char) + 1)
        else:
            # إذا لم يكن الحرف حرفًا، يتركه كما هو
            encrypted_text += char
    return encrypted_text

def decrypt(text):
    decrypted_text = ""
    for char in text:
        # يقوم بتحويل كل حرف إلى الحرف السابق في الترتيب الأبجدي
        if char.isalpha():  # يتأكد مما إذا كان الحرف حرفًا
            if char == 'a':
                decrypted_text += 'z'  # يعيد الحرف 'a' إلى 'z'
            elif char == 'A':
                decrypted_text += 'Z'  # يعيد الحرف 'A' إلى 'Z'
            else:
                # يضيف الحرف السابق في الترتيب الأبجدي
                decrypted_text += chr(ord(char) - 1)
        else:
            # إذا لم يكن الحرف حرفًا، يتركه كما هو
            decrypted_text += char
    return decrypted_text

# يسأل المستخدم ما إذا كان يرغب في تشفير أو فك تشفير الكلمة
choice = input("Would you like to encrypt or decrypt a word? Enter 'encrypt' or 'decrypt': ")

if choice.lower() == 'encrypt':
    word = input("Enter the word to encrypt: ")
    encrypted_word = encrypt(word)
    print("Encrypted word:", encrypted_word)
elif choice.lower() == 'decrypt':
    word = input("Enter the word to decrypt: ")
    decrypted_word = decrypt(word)
    print("Decrypted word:", decrypted_word)
else:
    print("Invalid choice! Please enter 'encrypt' or 'decrypt'.")
