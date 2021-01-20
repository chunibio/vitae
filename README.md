# vitae
Plan cources, track experience, build resume.

```shell
> vitae
Plan cources, track experience, build resume.

> vitae hobby
------------------------------------------------
Title           | Description
------------------------------------------------
Snowboarding    | ...
Knifes          | ...
Other           | ...

> vita
```


```rust
extern crate phonenumber;

use phonenumber::PhoneNumber;
use url::{Url, ParseError};


struct Person {
    personal_info: PersonalInfo,
    contact_info: ContactInfo,
    education: Vec<Education>,
    skills: Vec<Skill>,
    experience: Vec<Experience>,
    hobbies: Vec<Hobby>
}

trait Student {
    fn get_cources();
    fn get_gpa();
}

struct PersonalInfo {
    first_name: String,
    last_name: String,
    nickname: String,
    pronounce: String
}

struct ContactInfo {
    mobile_phone: Option<Phone>,
    home_phone: Option<Phone>,
    primary_email: String,
    secondary_email: Option<String>,
    primary_website: Option<Website>,
    secondary_website: Option<Website>
}

struct Phone {
    type: String,
    number: PhoneNumber
}

struct Website {
    url: Url,
    type: Option<WebsiteType>
}

enum WebsiteType {
    Personal,
    Portfolio,
    LinkedIn,
    GitHub,
    GitLab,
    Gitea,
    BitBucket,
    OtherWeb(String)
}

enum Education {
    HighSchool,
    University,
    OnlineCourse
}

struct University {
    name: String,
    gpa: Option<?>
}

struct Course {
    id: String,
    title: String,
    full_title: Option<String>,
    grade: Option <?>,
    projects: Vec<Projects>
}

struct Project {
    title: String
}

struct Skill {
    title: String,
    description: String,
    type: SkillType,
    level: SkillLevel
}

enum SkillType {
    TechnicalSkill,
    OtherSkill(String)
}

enum SkillLevel {
    TechnicalSkill,
    OtherSkill(String)
}

struct Hobby {
    title: String,  // shoul be limited to N symbols
    description: String,
    priority: HobbyPriority
}

```


### Resources
- https://crates.io/crates/qcv
- https://crates.io/crates/resufancy
- https://crates.io/search?q=Vitae
- https://app.standardresume.co/resumes/LwXFx3LjmoJckZ3td7f9i/write
