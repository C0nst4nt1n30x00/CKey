#!/usr/bin/python3

import os

print(''' 
░█████╗░██╗░░██╗███████╗██╗░░░██╗
██╔══██╗██║░██╔╝██╔════╝╚██╗░██╔╝
██║░░╚═╝█████═╝░█████╗░░░╚████╔╝░
██║░░██╗██╔═██╗░██╔══╝░░░░╚██╔╝░░
╚█████╔╝██║░╚██╗███████╗░░░██║░░░
░╚════╝░╚═╝░░╚═╝╚══════╝░░░╚═╝░░░ By Dhane Ashley Diabajo | Constantine''')


def main():
    print("Select an option:")
    print("1) Bing")
    print("2) Cloudflare")
    print("3) Datadog")
    print("4) Facebook Access Token")
    print("5) Facebook App Secret")
    print("6) GitHub Client ID and Secret")
    print("7) GitLab")
    print("8) HubSpot API Key")
    print("9) Stripe")
    print("10) Twitter API Secret")
    
    choice = input("Enter your choice (1-10): ")

    if choice == '1':
        api_key = input("Enter your Bing API key: ")
        url = f"https://dev.virtualearth.net/REST/v1/Locations?CountryRegion=US&adminDistrict=WA&locality=Somewhere&postalCode=98001&addressLine=100%20Main%20St.&key={api_key}"
        print(f"Calling: {url}")
        os.system(f"curl '{url}'")

    elif choice == '2':
        token = input("Enter your Cloudflare token: ")
        url = f"https://api.cloudflare.com/client/v4/user/tokens/verify"
        print(f"Calling: {url}")
        os.system(f"curl -X GET '{url}' -H 'Authorization: Bearer {token}'")

    elif choice == '3':
        api_key = input("Enter your Datadog API key: ")
        application_key = input("Enter your Datadog application key: ")
        url = f"https://api.datadoghq.com/api/v1/dashboard?api_key={api_key}&application_key={application_key}"
        print(f"Calling: {url}")
        os.system(f"curl '{url}'")

    elif choice == '4':
        access_token = input("Enter your Facebook access token: ")
        url = f"https://developers.facebook.com/tools/debug/accesstoken/?access_token={access_token}&version=v3.2"
        print(f"Calling: {url}")
        os.system(f"curl '{url}'")

    elif choice == '5':
        app_id = input("Enter your Facebook app ID: ")
        app_secret = input("Enter your Facebook app secret: ")
        url = f"https://graph.facebook.com/oauth/access_token?client_id={app_id}&client_secret={app_secret}&redirect_uri=&grant_type=client_credentials"
        print(f"Calling: {url}")
        os.system(f"curl '{url}'")

    elif choice == '6':
        client_id = input("Enter your GitHub client ID: ")
        client_secret = input("Enter your GitHub client secret: ")
        url = f"https://api.github.com/users/whatever?client_id={client_id}&client_secret={client_secret}"
        print(f"Calling: {url}")
        os.system(f"curl '{url}'")

    elif choice == '7':
        token = input("Enter your GitLab token: ")
        url = f"https://gitlab.example.com/api/v4/projects?private_token={token}"
        print(f"Calling: {url}")
        os.system(f"curl '{url}'")

    elif choice == '8':
        api_key = input("Enter your HubSpot API key: ")
        urls = [
            f"https://api.hubapi.com/owners/v2/owners?hapikey={api_key}",
            f"https://api.hubapi.com/contacts/v1/lists/all/contacts/all?hapikey={api_key}"
        ]
        for url in urls:
            print(f"Calling: {url}")
            os.system(f"curl '{url}'")

    elif choice == '9':
        token = input("Enter your Stripe token: ")
        
        charge_url = f"https://api.stripe.com/v1/charges"
        user_url = f"https://api.stripe.com/v1/users"

        print(f"Calling: {charge_url}")
        os.system(f"curl '{charge_url}' -u '{token}':")
        
        print(f"Calling: {user_url}")
        os.system(f"curl '{user_url}' -u '{token}':")

    elif choice == '10':
        api_key = input("Enter your Twitter API key: ")
        api_secret_key = input("Enter your Twitter API secret key: ")
        url = f"https://api.twitter.com/oauth2/token"
        print(f"Calling: {url}")
        os.system(f"curl -u '{api_key}:{api_secret_key}' --data 'grant_type=client_credentials' '{url}'")

if __name__ == "__main__":
    main()
           
