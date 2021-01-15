# vitae
Resume manager with experience tracking and resume generation

```rust
extern crate phonenumber;

use phonenumber::PhoneNumber;
use url::{Url, ParseError};


struct Person {
    personal_info: PersonalInfo,
    contact_info: ContactInfo,
    skills: Vec<Skill>,
    experience: Vec<Experience>,
    hobbies: Vec<Hobby>
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
    LinkedIn,
    GitHub,
    GitLab,
    Gitea,
    BitBucket,
    OtherWeb(String)
}

struct Education {
    title: String,
    courses: Vec<Course>
}

struct Course {
    id: String,
    title: String,
    full_title: Option<String>,
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
