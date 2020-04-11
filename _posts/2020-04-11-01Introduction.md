---
title: 01Introduction
tags: 
  - Stanford
  - Swift
---

# iOS

-   ## Four layers

    -   Core OS (Unix is mostly written in C, so most of that stuff is in C)

        ![image-20191220193633376](https://tva1.sinaimg.cn/large/006tNbRwly1ga3f552ojrj309d06s77y.jpg)

    -   Core Services (Finding out where the phone is on the planet or its orientation or access some files in the file system, we're gonna be using this layer right here and I'll be teaching you all about this layer. Core Services layer)

        ![image-20191220193645312](https://tva1.sinaimg.cn/large/006tNbRwly1ga3f5cgthnj307w06swhu.jpg)

    -   Media (This is kind of not a strict layering, but is the Media layer. It's got all kinds of media, video, audio, many different kinds, images, all this stuff.)

        ![image-20191220193659537](https://tva1.sinaimg.cn/large/006tNbRwly1ga3f5lc97wj309406wgpb.jpg)

    -   Cocoa Touch (Cocoa Touch is the UI layer of iOS. This is where the buttons and sliders, all those things are in.And there's also, really powerful objects here, like the Map Kit has a single object that you can just drop in your app that gives you pretty much the entire functionality of the map's app inside a rectangle, inside you window.)

        ![image-20191220193608598](https://tva1.sinaimg.cn/large/006tNbRwly1ga3f4r547hj309307gwip.jpg)

-   ## Platform Components

    -   Tools -> Xcode 
    -   Language -> Swift
    -   Frameworks -> Frameworks are just collections of objects
    -   Design Strategy -> MVC

-   ### Instance variable 

    -   Two way to initialization
        1.  Write a init (short for initializer) for a class & struct (short for structure)
        2.  Give a value for this property (instance variable)

-   ### Extremely strict for typing

    -   Although swift is extremely strict for typing, swift is also a language that has strong type inference, which means it will, if it can, guess the type for you.

-   ### didSet

    -   Any property, if you want, you can put code after it that says, didSet. And it will execute this code every time that thing gets set.
    -   Obviously we use property observers a lot to keep the UI in sync with the instance variables of our class.

-   ### Outlet Collection

    -   Outlet Collection means an array of the things in UI.

-   ## Optional

    -   `Int?` is an Optional that is a different type entirely from `Int` .
    -   Optional is a type that has two and only two states, set and not set. It's an enumeration (The cool things about enumerations in Swift, not a lot of other languages have this. For each case of an enumeration you can have associated data, just data that goes along with that thing) .
    -   An optional when it's in the set state, has associated data, which in this case is an int.
    -   `nil` always means an optional that's not set.

-   ## Today

    -   Creating a Project in Xcode 9, including building a UI and running in the iOS Simulator 
    -   Subclassing in Swift, including how to specify instance variables and methods 
    -   Connecting UI elements to invoke methods in our Swift code (actions) 
    -   print (outputting to the console using \() notation) 
    -   Connecting properties (instance variables) from our Swift code to the UI (outlets) 
    -   Accessing iOS documentation from our code 
    -   Automatically doing something every time a property ’ s value changes (didSet) 
    -   Array 
    -   Optionals

---

![image-20191122171731384](https://tva1.sinaimg.cn/large/006y8mN6ly1g96xrw6r0lj30hb08vqbl.jpg)
![image-20191122171953492](https://tva1.sinaimg.cn/large/006y8mN6ly1g96xue2ak2j30np0bh18d.jpg)
![image-20191122172008302](https://tva1.sinaimg.cn/large/006y8mN6ly1g96xul704pj30l205nq9n.jpg)![image-20191122172038775](https://tva1.sinaimg.cn/large/006y8mN6ly1g96xv57ewmj30k80dkam2.jpg)![image-20191122172101996](https://tva1.sinaimg.cn/large/006y8mN6ly1g96xwxwduxj30j70dfabf.jpg)![image-20191122172114441](https://tva1.sinaimg.cn/large/006y8mN6ly1g96xyq6wf9j30ie0dtwfu.jpg)![image-20191122172127700](https://tva1.sinaimg.cn/large/006y8mN6ly1g96xvzw43hj30is0dp7fb.jpg)![image-20191122172139910](https://tva1.sinaimg.cn/large/006y8mN6ly1g96xw8wgptj30ms0cm4ep.jpg)![image-20191122172428563](https://tva1.sinaimg.cn/large/006y8mN6ly1g96xz5t4zdj30m50c34e6.jpg)

### struct

> - 每一个在struct中的property must be initialized
>   1. Get an initializer. This means you have to give a init method(initializer)
>   2. Give the var value

### Outlet 

> - Outlet creates an instance variable (property) 
> - **action create a method**

### Rename 

> - when you want to rename ,the best way is to cmd+click and choose rename

### Optional 

> - this is an enumeration ([美: ɪˌnuːməˈreɪʃn] [英: ɪˌnjuːməˈreɪʃn]n. 列举；[数] 计算；细目)
> - 

| splash         | [美: splæʃ] [英: splæʃ]                                      | v. 泼洒；把（水、泥等）泼在……上；（在水中）溅着水花行走；（在显著位置）刊登 |
| -------------- | ------------------------------------------------------------ | ------------------------------------------------------------ |
| Splash  screen | 启动页                                                       | n. 落水声；拍水；溅上的液体；色块；（非正式）掺饮料的少量液体；（非正式）要闻；（非正式）引人注目的效果 |
| Pop up         | 显示在这里                                                   | pop v. 突然出现；突然地行动；爆开；射击；瞪大眼；（使）发出爆裂声；迅速放置；速去；耳压发生变化；（过度）服药； |
| Navigator      | [美: ˈnævɪɡeɪtər] [英: ˈnævɪɡeɪtə(r)]                        | 导航器                                                       |
| Instructor     | [美: ɪnˈstrʌktər] [英: ɪnˈstrʌktə(r)]                        | n. 指导书；教员；指导者                                      |
| Dude           | [美: duːd] [英: duːd; djuːd]                                 | 伙计                                                         |
| Burden         | [美: ˈbɜːrdn] [英: ˈbɜːdn]                                   | n. 负担；责任；船的载货量                                    |
| infer          | [美: ɪnˈfɜːr] [英: ɪnˈfɜː(r)]                                | vi. 推断；作出推论                                           |
| Grip           | [美: ɡrɪp] [英: ɡrɪp]                                        | n. 紧握；柄；支配；握拍方式；拍柄绷带                        |
| directive      | [美: dɪrekˈtiv; dəˈrɛktɪv; daɪˈrɛktɪv] [英: daɪ'rektɪv; dɪ'rektɪv] | n. 指示；指令                                                |
| Exclamation    | [美: ˌɛkskləˈmeʃən] [英: ˌekskləˈmeɪʃn]                      | n. 感叹；惊叫；惊叹词                                        |
| Side effect    | 副作用                                                       | Side  n. 方面；侧面；旁边                                    |
| Freak out      | 吓一跳                                                       | Freak [美: friːk] [英: friːk] n. 怪人，怪事；畸形人；反复无常 |
| Increment      | [美: ˈɪŋkrəmənt] [英: ˈɪŋkrəmənt]                            | n. [数] 增量；增加；增额；盈余                               |
| Fantastic      | [美: fænˈtæstɪk] [英: fænˈtæstɪk]                            | adj. 奇异的；空想的；异想天开的；古怪的；极好的，极出色的；不可思议的；不切实际的 |
| Nasty          | [美: ˈnæsti] [英: ˈnɑːsti]                                   | adj. 极差的；恶心的；恶意的；有害的；严重的（伤、疾病）；粗鲁的，下流的；可恶的；难对付的 |
| horrendous     | [美: həˈrendəs] [英: həˈrendəs]                              | adj. 可怕的；惊人的                                          |
| Observer       | [美: əbˈzɜːrvər] [英: əbˈzɜːvə(r)]                           | n. 观察者；[天] 观测者；遵守者                               |
| Simultaneously | [美: ˌsaɪmlˈteɪniəsli] [英: ˌsɪmlˈteɪniəsli]                 | adv. 同时地                                                  |
| Architecture   | [美: ˈɑːrkɪtektʃər] [英: ˈɑːkɪtektʃə(r)]                     | n. 建筑学；建筑风格；建筑式样；架构                          |
| Attack         | [美: əˈtæk] [英: əˈtæk]                                      | n. 攻击；抨击；疾病发作                                      |
| Specify        | [美: ˈspesɪfaɪ] [英: ˈspesɪfaɪ]                              | vt. 指定；详细说明；列举；把…列入说明书                      |
| Entirely       | [美: ɪnˈtaɪərli] [英: ɪnˈtaɪəli]                             | adv. 完全地，彻底地                                          |
| Discreet       | [美: dɪˈskriːt] [英: dɪˈskriːt]                              | adj. 谨慎的；小心的                                          |
| Associate      | [美: əˈsoʊsieɪt,əˈsoʊʃieɪt] [英: əˈsəʊsieɪt; əˈsəʊʃieɪt]     | v. 联想，联系；（使）关联；与（不被认同的人）交往；将……和……联系起来；表示同意 |
| Fatal          | [美: ˈfeɪtl] [英: ˈfeɪtl]                                    | adj. 致命的；重大的；毁灭性的；命中注定的                    |
| nil            | [美: nɪl] [英: nɪl]                                          | n. 无，零                                                    |
| Wrap           | [美: ræp] [英: ræp]                                          | n. 外套；围巾      vt. 包；缠绕；隐藏；掩护                  |
| Unwrap         | [美: ʌnˈræp] [英: ʌnˈræp]                                    | vt. 打开                                                     |
| Conditionally  | [美: kənˈdɪʃənəli] [英: kənˈdɪʃənəli]                        | adv. 附有条件地                                              |
| Fragile        | [美: ˈfrædʒl] [英: ˈfrædʒaɪl]                                | adj. 脆的；易碎的                                            |
| Paragpraph     | [美: ˈpærəɡræf] [英: ˈpærəɡrɑːf]                             | n. 段落；短评；段落符号                                      |
| Dime           | [美: daɪm] [英: daɪm]                                        | n. （美国、加拿大的）十分硬币；少量的钱；小东西              |

