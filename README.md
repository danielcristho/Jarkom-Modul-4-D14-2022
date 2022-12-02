
# Jarkom-Modul-4-D14-2022

Lapres Praktikum Jarkom Modul 4 Kelompok D-14

| Nama                      | NRP      |
|---------------------------|----------|
|Gloriyano C. Daniel Pepuho |5025201121|

## Cara Pengerjaan

 1. [VLSM-CPT](#vlsm---cpt)
 2. [CIDR-GNS3](#cidr---gns3)


## VLSM - CPT

<details>
  <summary>Expand</summary>
  
 1. [Alokasi VLSM](https://user-images.githubusercontent.com/69733783/203913765-884e4481-4cbd-4b65-a967-2c35ab6245fc.jpg)
 2. [Pohon IP](https://miro.com/app/board/uXjVPAiX5fE=/?share_link_id=462538221993)
 3. [Topologi](https://user-images.githubusercontent.com/69733783/203913758-07a4fdc5-98d2-4081-865a-b9756b1ab2d9.png)

</details>

### Alokasi IP

Node                        | Alokasi      |  Netmask   |
|---------------------------|--------------|------------|
|A1                         |1001          |/22         |
|A2                         |2             |/30         |
|A3                         |2             |/30         |
|A4                         |251           |/24         |
|A5                         |51            |/26         |
|A6                         |2             |/30         |
|A7                         |2             |/30         |
|A8                         |2             |/30         |
|A9                         |271           |/23         |
|A10                        |2             |/30         |
|A11                        |2             |/30         |
|A12                        |121           |/25         |
|A13                        |71            |/25         |
|A14                        |121           |/25         |
|A15                        |501           |/23         |
|A16                        |212           |/24         |
|A17                        |2             |/30         |
|A18                        |2             |/30         |
|Jumlah                     |2618          |/20         |

<!-- ### Inventory

|Router                     |  Interface   |  IP               |
|---------------------------|--------------|-------------------|
|The Minister               | Fa1/0        | 192.192.1.1/22    |
|                           | Fa0/0        | 192.192.11.193/30 |
|                           | Fa2/0        | 192.192.11.197/30 |
|The Dauntless              | Fa1/0        | 192.192.8.1/24    |
|                           | Fa2/0        | 192.192.11.198/30 |
|The Order                  | Fa0/0        | 192.192.11.194/30 |
|                           | Fa1/0        | 192.192.11.129/26 |
|                           | Fa2/0        | 192.192.11.201/30 |
|The Ressinance             | Fa0/0        | 192.192.11.213/30 |
|                           | Fa2/0        | 192.192.11.202/30 |
|                           | Fa3/0        | 192.192.11.209/30 |
|                           | Fa4/0        | 192.192.11.205/30 |
|The Magical                | Fa1/0        | 192.192.6.1/23    |
|                           | Fa3/0        | 192.192.11.210/30 |
|The Instrument             | Fa0/0        | 192.192.11.214/30 |
|                           | Fa1/0        | 192.192.11.1/25   |
|                           | Fa2/0        | 192.192.11.221/30 |
|                           | Fa3/0        | 192.192.11.218/30 |
|The Firefist               | Fa0/0        | 192.192.9.1/24    |
|                           | Fa1/0        | 192.192.4.1/23    | -->

### Routing

* The Minister

```bash
192.192.8.0/24 via 192.192.11.198
192.192.11.128/26 via 192.192.11.194
192.192.11.204/30 via 192.192.11.194
0.0.0.0/0 via 192.192.11.194
```

* The Dauntless

```bash
192.192.0.0/22 via 192.192.11.197
0.0.0.0/0 via 192.192.11.197
```

* The Order

```bash
192.192.0.0/22 via 192.192.11.193
192.192.11.204/30 via 192.192.11.202
0.0.0.0/0 via 192.192.11.193
0.0.0.0/0 via 192.192.11.202
```

* The Ressinance

```bash
192.192.11.128/26 via 192.192.11.201
192.192.0.0/22 via 192.192.11.201
0.0.0.0/0 via 192.192.11.201
192.192.6.0/23 via 192.192.11.210
0.0.0.0/0 via 192.192.11.210
0.0.0.0/0 via 192.192.11.214
```

* The Magical

```bash
192.192.11.204/30 via 192.192.11.209
0.0.0.0/0 via 192.192.11.209
```

* The Instrument

```bash
0.0.0.0/0 via 192.192.11.213
0.0.0.0/0 via 192.192.11.219
0.0.0.0/0 via 192.192.11.222
```

* The Refound

```bash
192.192.11.0/25 via 192.192.11.218
0.0.0.0/0 via 192.192.11.218
```

* The Firefist

```bash
0.0.0.0/0 via 192.192.11.221
192.192.11.224/30 via 192.192.9.2
```

* The Queen

```bash
192.192.4.0/23 via 192.192.9.1
0.0.0.0/0 via 192.192.9.1

```

## CIDR - GNS3
<details>
  <summary>Expand</summary>
  
 1. [Alokasi CIDR](https://user-images.githubusercontent.com/69733783/204085390-e9bd18a2-5d3c-4433-9d9b-e64adb26767d.png)
 2. [Pohon IP](https://miro.com/app/board/uXjVPAiX5fE=/?share_link_id=462538221993)
 3. [Topologi](https://user-images.githubusercontent.com/69733783/204131796-f4d45483-f3ef-460c-8063-c85924e4c57b.png)

</details>

### Alokasi IP

#### A

|Node                       | Alokasi      |  Netmask   |
|---------------------------|--------------|------------|
|A1                         |1001          |/22         |
|A2                         |2             |/30         |
|A3                         |2             |/30         |
|A4                         |251           |/24         |
|A5                         |51            |/26         | -
|A6                         |2             |/30         |
|A7                         |2             |/30         |
|A8                         |2             |/30         |
|A9                         |271           |/23         |
|A10                        |2             |/30         |
|A11                        |2             |/30         |
|A12                        |121           |/25         |
|A13                        |71            |/25         |
|A14                        |121           |/25         |
|A15                        |501           |/23         |
|A16                        |212           |/24         |
|A17                        |2             |/30         |
|A18                        |2             |/30         |
|Jumlah                     |2618          |/20         |

#### B

|Node                       | Alokasi      |  Netmask   |
|---------------------------|--------------|------------|
|B1 (A3,A4)                 |252           |/23         | - 
|B2 (A12,A13)               |192           |/24         |
|B3 (A16,A18)               |213           |/23         |

#### C

|Node                       | Alokasi      |  Netmask   |
|---------------------------|--------------|------------|
|C1 (B1,A1)                 |1253          |/21         |
|C2 (B2,A11)                |194           |/23         |
|C3 (B3,A15)                |714           |/22         |

#### D

|Node                       | Alokasi      |  Netmask   |
|---------------------------|--------------|------------|
|D1 (C1,A2)                 |1255          |/20         |
|D2 (C2,A14)                |315           |/22         |
|D3 (C3,A17)                |214           |/21         |

#### E

|Node                       | Alokasi      |  Netmask   |
|---------------------------|--------------|------------|
|E1 (D1,A5)                 |1306          |/19         |
|E2 (D2,D3)                 |529           |/20         |

#### F

|Node                       | Alokasi      |  Netmask   |
|---------------------------|--------------|------------|
|F1 (E1,A6)                 |1308          |/18         | - 
|F2 (E2,A10)                |531           |/19         |

#### G

|Node                       | Alokasi      |  Netmask   |
|---------------------------|--------------|------------|
|G1 (F1,A7)                 |1309          |/17         | - 
|G2 (F2,A8)                 |533           |/18         |

#### H

|Node                       | Alokasi      |  Netmask   |
|---------------------------|--------------|------------|
|H1 (G2,A9)                 |804           |/17         |

#### I

|Node                       | Alokasi      |  Netmask   |
|---------------------------|--------------|------------|
|I1 (H1,G1)                 |2113          |/16         | - 


### Routing

* The Minister

```bash
route add -net 192.192.6.0 netmask 255.255.255.0 gw 192.192.32.2
route add -net 192.192.16.0 netmask 255.255.255.192 gw 192.192.64.2
route add -net 0.0.0.0 netmask 0.0.0.0 gw 192.192.64.2

```

* The Dauntless

```bash
route add -net 192.192.0.0 netmask 255.255.252.0 gw 192.192.32.1
route add -net 0.0.0.0 netmask 0.0.0.0 gw 192.192.32.1
```

* The Order

```bash
route add -net 192.192.5.0 netmask 255.255.255.252 gw 192.192.8.2
route add -net 192.192.0.0 netmask 255.255.252.0 gw 192.192.64.1
route add -net 0.0.0.0 netmask 0.0.0.0 gw 192.192.64.1
route add -net 0.0.0.0 netmask 0.0.0.0 gw 192.192.8.2
```

* The Resinnace

```bash
route add -net 192.192.16.0 netmask 255.255.255.192 gw 192.192.8.1
route add -net 192.192.192.0 netmask 255.255.254.0 gw 192.192.160.2
route add -net 192.192.136.0 netmask 255.255.255.128 gw 192.192.144.2
route add -net 0.0.0.0 netmask 0.0.0.0 gw 192.192.144.2
route add -net 0.0.0.0 netmask 0.0.0.0 gw 192.192.8.1

route add default gw 192.168.122.1
```

* The Magical

```bash
route add -net 192.192.5.0 netmask 255.255.255.252 gw 192.192.160.1
route add -net 0.0.0.0 netmask 0.0.0.0 gw 192.192.160.1
```

* The Instrument

```bash
route add -net 192.192.5.0 netmask 255.255.255.252 gw 192.192.144.1
route add -net 192.192.138.0 netmask 255.255.255.128 gw 192.192.138.2
route add -net 192.192.136.128 netmask 255.255.255.128 gw 192.192.138.2
route add -net 192.192.128.0 netmask 255.255.254.0 gw 192.192.132.2
route add -net 192.192.130.0 netmask 255.255.255.0 gw 192.192.132.2
route add -net 0.0.0.0 netmask 0.0.0.0 gw 192.192.144.1
route add -net 0.0.0.0 netmask 0.0.0.0 gw 192.192.132.2
```

* The Refound

```bash
route add -net 0.0.0.0 netmask 0.0.0.0 gw 192.192.138.1
route add -net 192.192.136.0 netmask 255.255.255.128 gw 192.192.138.1
```

* The Firefist

```bash
route add -net 192.192.131.0 netmask 255.255.255.252 gw 192.192.130.2
route add -net 0.0.0.0 netmask 0.0.0.0 gw 192.192.132.1
```

* The Queen

```bash
route add -net 192.192.128.0 netmask 255.255.254.0 gw 192.192.130.1
route add -net 0.0.0.0 netmask 0.0.0.0 gw 192.192.130.1
```