import os
from os import path
try:
    import string
    import requests
    import numpy
    from colorama import Fore, init
    import threading
    import random
except:
    os.system('pip install string')
    os.system('pip install requests')
    os.system('pip install numpy')
    os.system('pip install colorama')
    os.system('pip install threading')
    os.system('pip install random')
init(autoreset=True)
m = Fore.MAGENTA
b = Fore.BLUE
print(f'''
         @7lm.py
{m}███████{b}╗    {m}██{b}╗         {m}███{b}╗   {m}███{b}╗
╚════{m}██{b}║    {m}██{b}║         {m}████{b}╗ {m}████{b}║
    {m}██{b}╔╝    {m}██{b}║         {m}██{b}╔{m}████{b}╔{m}██{b}║
   {m}██{b}╔╝     {m}██{b}║         {m}██{b}║╚{m}██{b}╔╝{m}██{b}║
   {m}██{b}║      {m}███████{b}╗    {m}██{b}║ ╚═╝ {m}██{b}║
   ╚═╝      ╚══════╝    ╚═╝     ╚═╝
         {Fore.LIGHTMAGENTA_EX}NITRO{Fore.RESET} CHECKER
         
    [{Fore.BLUE}1{Fore.RESET}] Create CODE {Fore.LIGHTMAGENTA_EX}NITRO{Fore.RESET}
    [{Fore.BLUE}2{Fore.RESET}] AUTO CHECKER {Fore.LIGHTMAGENTA_EX}NITRO{Fore.RESET}
    [{Fore.BLUE}3{Fore.RESET}] CHECK [ {Fore.RED}nitro-CHECK.txt{Fore.RESET} ]
    [{Fore.CYAN}*{Fore.RESET}] You should have {Fore.GREEN}proxy.txt{Fore.RESET}
    ''')
number = input('''              NUMBER : ''')

print(' ')
if number == '1':
    num = input('How many codes do you want : ')
    print(' ')
    chars = []
    chars[:0] = string.ascii_letters + string.digits
    for code in range(int(num)):
        s = numpy.random.choice(chars, size=19)[0]
        s1 = numpy.random.choice(chars, size=19)[0]
        s2 = numpy.random.choice(chars, size=19)[0]
        s3 = numpy.random.choice(chars, size=19)[0]
        s4 = numpy.random.choice(chars, size=19)[0]
        s5 = numpy.random.choice(chars, size=19)[0]
        s6 = numpy.random.choice(chars, size=19)[0]
        s7 = numpy.random.choice(chars, size=19)[0]
        s8 = numpy.random.choice(chars, size=19)[0]
        s9 = numpy.random.choice(chars, size=19)[0]
        s10 = numpy.random.choice(chars, size=19)[0]
        s11 = numpy.random.choice(chars, size=19)[0]
        s12 = numpy.random.choice(chars, size=19)[0]
        s13 = numpy.random.choice(chars, size=19)[0]
        s14 = numpy.random.choice(chars, size=19)[0]
        s15 = numpy.random.choice(chars, size=19)[0]
        s16 = numpy.random.choice(chars, size=19)[0]
        s17 = numpy.random.choice(chars, size=19)[0]
        s18 = numpy.random.choice(chars, size=19)[0]
        c = str(s+s1+s2+s3+s4+s5+s6+s7+s8+s9+s10+s11+s12+s13+s14+s15+s16+s17+s18)
        with open('nitro-code.txt', 'a') as cod:
            cod.write(c + '\n')
        print(c)

if number == '2':

    if path.exists("proxy.txt"):
        proxyfile = open("proxy.txt", 'r').read().splitlines()
    else:
        print("Make proxy.txt file\n")
        input()
        exit()
    print(' ')
    thr = input('Threads : ')
    print(f'[{Fore.CYAN}*{Fore.RESET}] You should have {Fore.GREEN}valid proxy{Fore.RESET}')
    print(f'[{Fore.CYAN}*{Fore.RESET}] I Will save any valid code in [{Fore.RED} Nitro-Codes.txt {Fore.RESET}]')

    input('Press ENTER TO START ..\>')
    print(' ')
    def check():
        url2 = 'https://discord.gift/'
        chars = []
        chars[:0] = string.ascii_letters + string.digits
        zero = 0
        zero2 = 0
        zero3 = 0
        while 1:
            proxy_dict = []
            for proxy in proxyfile:
                proxy_dict.append(proxy)
                rnd = str(random.choice(proxy_dict))
            try:
                proxyf = {
                    "http": f"http://{rnd}",
                    "https": f"http://{rnd}"
                }
                s = numpy.random.choice(chars, size=19)[0]
                s1 = numpy.random.choice(chars, size=19)[0]
                s2 = numpy.random.choice(chars, size=19)[0]
                s3 = numpy.random.choice(chars, size=19)[0]
                s4 = numpy.random.choice(chars, size=19)[0]
                s5 = numpy.random.choice(chars, size=19)[0]
                s6 = numpy.random.choice(chars, size=19)[0]
                s7 = numpy.random.choice(chars, size=19)[0]
                s8 = numpy.random.choice(chars, size=19)[0]
                s9 = numpy.random.choice(chars, size=19)[0]
                s10 = numpy.random.choice(chars, size=19)[0]
                s11 = numpy.random.choice(chars, size=19)[0]
                s12 = numpy.random.choice(chars, size=19)[0]
                s13 = numpy.random.choice(chars, size=19)[0]
                s14 = numpy.random.choice(chars, size=19)[0]
                s15 = numpy.random.choice(chars, size=19)[0]
                s16 = numpy.random.choice(chars, size=19)[0]
                s17 = numpy.random.choice(chars, size=19)[0]
                s18 = numpy.random.choice(chars, size=19)[0]
                c = str(s+s1+s2+s3+s4+s5+s6+s7+s8+s9+s10+s11+s12+s13+s14+s15+s16+s17+s18)
                url = f"https://discordapp.com/api/v9/entitlements/gift-codes/{c}?with_application=false&with_subscription_plan=true"
                response = requests.get(url)
                if response.status_code == 200:
                    zero += 1
                    print(f"""\r[{Fore.CYAN}*{Fore.RESET}] > [{Fore.GREEN}+{Fore.RESET}] {Fore.GREEN}Valid{Fore.RESET} [{zero}] | [{Fore.RED}-{Fore.RESET}] {Fore.RED}Invalid{Fore.RESET} [{zero2}] | [{Fore.LIGHTRED_EX}-{Fore.RESET}] Bad Proxy [{zero3}] | [ {url2+c} ]""", end="")
                    with open("Nitro-Codes.txt", "w") as file:
                        file.write(url)
                else:
                    zero2 += 1
                    print(f"""\r[{Fore.CYAN}*{Fore.RESET}] > [{Fore.GREEN}+{Fore.RESET}] {Fore.GREEN}Valid{Fore.RESET} [{zero}] | [{Fore.RED}-{Fore.RESET}] {Fore.RED}Invalid{Fore.RESET} [{zero2}] | [{Fore.LIGHTRED_EX}-{Fore.RESET}] Bad Proxy [{zero3}] | [ {url2+c} ]""", end="")
            except requests.exceptions.ConnectionError:
                zero3 += 1
                print(f"""\r[{Fore.CYAN}*{Fore.RESET}] > [{Fore.GREEN}+{Fore.RESET}] {Fore.GREEN}Valid{Fore.RESET} [{zero}] | [{Fore.RED}-{Fore.RESET}] {Fore.RED}Invalid{Fore.RESET} [{zero2}] | [{Fore.LIGHTRED_EX}-{Fore.RESET}] Bad Proxy [{zero3}] | [ {url2 + c} ]""",end="")
threads = []
for i in range(int(thr)):
    t = threading.Thread(target=check)
    t.start()
    threads.append(t)
for i in threads:
    i.join()

if number == '3':
    if path.exists("proxy.txt"):
        proxyfile = open("proxy.txt", 'r').read().splitlines()
    else:
        print("Make proxy.txt file\n")
        input()
        exit()
    print(' ')
    thr = input('Threads : ')
    print(f'[{Fore.CYAN}*{Fore.RESET}] You should have {Fore.GREEN}valid proxy{Fore.RESET}')
    print(f'[{Fore.CYAN}*{Fore.RESET}] I Will save any valid code in [{Fore.RED} Nitro-Codes.txt {Fore.RESET}]')

    input('Press ENTER TO START ..\>')
    print(' ')
    def check():
        url2 = 'https://discord.gift/'
        file = open('nitro-CHECK.txt', 'r')
        zero = 0
        zero2 = 0
        zero3 = 0
        while 1:
            proxy_dict = []
            for proxy in proxyfile:
                proxy_dict.append(proxy)
                rnd = str(random.choice(proxy_dict))
            try:
                proxyf = {
                    "http": f"http://{rnd}",
                    "https": f"http://{rnd}"
                }
                code = file.readline().split('\n')[0]
                url = f"https://discordapp.com/api/v9/entitlements/gift-codes/{code}?with_application=false&with_subscription_plan=true"
                response = requests.get(url, proxies=proxyf)
                if response.status_code == 200:
                    zero += 1
                    print(
                        f"""\r[{Fore.CYAN}*{Fore.RESET}] > [{Fore.GREEN}+{Fore.RESET}] {Fore.GREEN}Valid{Fore.RESET} [{zero}] | [{Fore.RED}-{Fore.RESET}] {Fore.RED}Invalid{Fore.RESET} [{zero2}] | [{Fore.LIGHTRED_EX}-{Fore.RESET}] ERROR[{zero3}] | [ {url2 + c} ]""",
                        end="")
                    with open("Nitro-Codes.txt", "w") as file:
                        file.write(url)
                else:
                    zero2 += 1
                    print(
                        f"""\r[{Fore.CYAN}*{Fore.RESET}] > [{Fore.GREEN}+{Fore.RESET}] {Fore.GREEN}Valid{Fore.RESET} [{zero}] | [{Fore.RED}-{Fore.RESET}] {Fore.RED}Invalid{Fore.RESET} [{zero2}] | [{Fore.LIGHTRED_EX}-{Fore.RESET}] ERROR [{zero3}] | [ {url2 + c} ]""",
                        end="")
            except requests.exceptions.ConnectionError:
                zero3 += 1
                print(
                    f"""\r[{Fore.CYAN}*{Fore.RESET}] > [{Fore.GREEN}+{Fore.RESET}] {Fore.GREEN}Valid{Fore.RESET} [{zero}] | [{Fore.RED}-{Fore.RESET}] {Fore.RED}Invalid{Fore.RESET} [{zero2}] | [{Fore.LIGHTRED_EX}-{Fore.RESET}] ERROR [{zero3}] | [ {url2 + c} ]""",
                    end="")
threads = []
for i in range(int(thr)):
    t = threading.Thread(target=check)
    t.start()
    threads.append(t)
for i in threads:
    i.join()
