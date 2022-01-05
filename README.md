# modul-4

**kelompok 10**

**rachmad saflyi & alifia**

------

## Step by Step

------

Make 2 copies of each containers

![Screenshot (546)](https://user-images.githubusercontent.com/93419670/148258029-750783d0-df53-4e9f-b4e1-bbf7840548e2.png)

Then start each containers

![Screenshot (547)](https://user-images.githubusercontent.com/93419670/148258139-c7ef30b9-7795-462e-9d8d-3900430559df.png)

Go to 'ubuntu_php7.4_2', then change the IP address to '10.0.3.111' so that differ from 'ubuntu_php7.4'. Same as 'ubuntu_php7.4_3' change the IP address to '10.0.3.123'

![Screenshot (548)](https://user-images.githubusercontent.com/93419670/148258214-2a9dc5a3-42b6-4d93-b076-cd9d2e362539.png)

Go to etc/hosts to register 'lxc_php7_2.dev'

![Screenshot (550)](https://user-images.githubusercontent.com/93419670/148258321-b4c025f3-8fe1-4db1-948d-365876d5d0ac.png)

Then change the server name

![Screenshot (552)](https://user-images.githubusercontent.com/93419670/148258425-90c5bca4-6cfb-4f61-adfd-b4a56925f0a2.png)

Restart nginx then curl it. Repeat the same steps for 'ubuntu_php7.4_3'

![Screenshot (553)](https://user-images.githubusercontent.com/93419670/148258543-00dcccbe-0ceb-4804-a63e-faab30449f11.png)
![Screenshot (554)](https://user-images.githubusercontent.com/93419670/148258720-8d07f576-5988-4bd4-a863-3c115d79643b.png)

Same as ubuntu_php7.4 we need to start all container

![Screenshot (556)](https://user-images.githubusercontent.com/93419670/148258854-2de8a672-4848-46bd-8709-767cbc88624a.png)

Go to 'debian_php5.6_2' and change the IP address to '10.0.3.112'. The same for 'debian_php5.6_3' and change the IP address to '10.0.3.122'

![Screenshot (557)](https://user-images.githubusercontent.com/93419670/148259167-43460480-791c-4686-856e-5b114425fe35.png)

Register 'lxc_php5_2.dev' at /etc/hosts

![Screenshot (558)](https://user-images.githubusercontent.com/93419670/148259204-184e8e55-ff8a-4712-b8e7-6a3857cce11c.png)

change the server name, then repeat the same steps for 'debian_php5.6_3'. don't forget to restart the container

![Screenshot (559)](https://user-images.githubusercontent.com/93419670/148259277-e7321944-5857-41be-9ab6-8595e03743b4.png)

Register all the contaiers in /etc/hosts (on vm)

![Screenshot (566)](https://user-images.githubusercontent.com/93419670/148259389-9efad118-0359-483f-b33d-bffd1188db08.png)

Run the jmeter. Change the number of threads from user access from 50, 100, 150

![Screenshot (571)](https://user-images.githubusercontent.com/93419670/148259538-934e139b-a11c-408b-80fc-272d971ed349.png)

![Screenshot (572)](https://user-images.githubusercontent.com/93419670/148259577-4508e592-f833-4952-8dce-1056af46f16b.png)

![Screenshot (573)](https://user-images.githubusercontent.com/93419670/148259593-6300500e-95c2-432f-b187-f9b64925a5be.png)

![Screenshot (574)](https://user-images.githubusercontent.com/93419670/148259606-62022a6d-5b2d-4e84-9244-05d2aafca664.png)

![Screenshot (575)](https://user-images.githubusercontent.com/93419670/148259766-914b9c2a-04e7-4679-abe9-e71dc6f64ee6.png)

![Screenshot (576)](https://user-images.githubusercontent.com/93419670/148259778-faf7f464-d0b5-41a3-8678-8835c505b705.png)

![Screenshot (577)](https://user-images.githubusercontent.com/93419670/148259788-eb804333-cd91-4ebd-8bd0-bc44e7f5bedc.png)

![Screenshot (578)](https://user-images.githubusercontent.com/93419670/148259859-59d05bee-1c37-40f6-92ff-e80ae41a7c8d.png)

![Screenshot (579)](https://user-images.githubusercontent.com/93419670/148259882-2c462546-cd4e-4d0f-b66c-790f0dddb1d6.png)

![Screenshot (580)](https://user-images.githubusercontent.com/93419670/148259902-dbd6042d-8e04-44c4-b412-ab28288421b2.png)

Then we went back to VM than go to

```
nano /etc/nginx/sites-available/vm.local
```

to add upstream landing, php5, and php7

![Screenshot (581)](https://user-images.githubusercontent.com/93419670/148260039-32272238-4246-40de-8cb3-d1e88b56a2a6.png)

change the proxy_pass

![Screenshot (582)](https://user-images.githubusercontent.com/93419670/148260108-f0a3faee-2bd0-4a99-af15-524932f0eea2.png)

Then we go back to the jmeter and redo it

![Screenshot (583)](https://user-images.githubusercontent.com/93419670/148260316-14959aa4-c4bd-45e8-a090-90a3ce1a1b67.png)

![Screenshot (584)](https://user-images.githubusercontent.com/93419670/148260336-5d966922-5f49-4373-8640-5725f589b390.png)

![Screenshot (585)](https://user-images.githubusercontent.com/93419670/148260353-73b2c14d-d8c6-43e6-9d9c-df644829d611.png)

![Screenshot (586)](https://user-images.githubusercontent.com/93419670/148260379-281c4c1f-e1ac-481e-aa75-2891e5b68666.png)

![Screenshot (587)](https://user-images.githubusercontent.com/93419670/148260394-eda6f246-1b19-4bfb-976a-d82dbe096dcd.png)

![Screenshot (588)](https://user-images.githubusercontent.com/93419670/148260431-182fc3fb-67dc-4d93-b289-6bcd913f68e7.png)

![Screenshot (589)](https://user-images.githubusercontent.com/93419670/148260451-fbb1a86b-ff6d-4cad-8b24-468a150f28ef.png)

![Screenshot (590)](https://user-images.githubusercontent.com/93419670/148260473-701d0c9c-f688-416f-ad25-c110d9f6b4bc.png)

![Screenshot (591)](https://user-images.githubusercontent.com/93419670/148260506-af32d720-ed56-4e31-9682-36bff82d61fb.png)

![Screenshot (592)](https://user-images.githubusercontent.com/93419670/148260532-6447c6c3-dc32-4fd9-bd72-059f984686f8.png)

Analysis

Below is the results from when we use load balancer and not using the load balancer

 - When there is 50 users that access our web, if we don't use load balancer the average time of user accessing our web is
   - landing : 785 ms = 0.79 s
   - blog : 360 ms = 0.36 s
   - app : 438 ms = 0.44 s
- When we use load balancer, then
   - landing : 686 ms = 0.69 s
   - blog : 229 ms = 0.23 s
   - app : 225 ms = 0.23 s

Here we can know that the average time of user accessing our web is faster then if we use load balancer. For the throughput or the amount of user accessing our web is

- When there is 50 users that access our web, if we don't use load balancer the amount of user accessing our web is

  - landing : 42 user / second
  - blog :  43 user / second
  - app : 47 user / second

- When we use load balancer, then

  - landing : 54 user / second
  - blog :  84 user / second
  - app : 77 user / second

  Here we can know that the average time of amount of user accessing our web in 1 second is faster then if we don't use load balancer.


  The conclusion is, if we use load balancer, then the time is faster and the amount of users that accessing our web is much more then when we don't use load balancer.

  
