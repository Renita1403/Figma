# Ex09 Event Registration Web Application
## Date:8/10/2025

## AIM:
To design, develop and deploy a web application for event registration.

## DESIGN STEPS:

### Step 1:
Create a new frame.

### Step 2:
Select any one preset size of your choice.

### Step 3:
Select the shapes you need.

### Step 4:
Import images as needed.

### Step 5:
Create pages based on your need and link them.

### Step 6:

Validate the HTML and CSS code.

### Step 6:

Publish the website in the given URL.

## DESIGN TOOL:
Figma

## CODE:
```
import React from "react";
import download1 from "./download-1.png";
import image from "./image.svg";
import images2 from "./images-2.png";
import textOnAPath2 from "./text-on-a-path-2.svg";
import textOnAPath from "./text-on-a-path.svg";

export const IphoneProMax = (): JSX.Element => {
  const handleLogin = () => {
    console.log("Login clicked");
  };

  const handleRegister = () => {
    console.log("Register clicked");
  };

  return (
    <div className="bg-[#62a1a0] overflow-hidden w-full min-w-[1222px] min-h-[2133px] relative">
      <img
        className="absolute top-[242px] left-[360px] w-[529px] h-[509px] aspect-[1.04] object-cover"
        alt="Download"
        src={download1}
      />

      <img
        className="absolute top-[2325px] left-[2020px] w-[416px] h-[196px]"
        alt="Text on a path"
        src={image}
      />

      <img
        className="absolute top-[2721px] left-[2020px] w-[416px] h-[187px]"
        alt="Text on a path"
        src={textOnAPath2}
      />

      <img
        className="absolute top-[15px] left-[282px] w-[758px] h-[157px] aspect-[4.83] object-cover"
        alt="Images"
        src={images2}
      />

      <h1 className="absolute top-[860px] left-[294px] [font-family:'Inter-SemiBold',Helvetica] font-semibold text-[#181616] text-[64px] tracking-[0] leading-[normal]">
        SPORTS DAY EVENT
      </h1>

      <img
        className="absolute top-[2423px] left-[2014px] w-[422px] h-[173px]"
        alt="Text on a path"
        src={textOnAPath}
      />

      <button
        className="top-[1135px] absolute left-[254px] w-[635px] h-[190px] bg-[#151a3a] cursor-pointer transition-opacity hover:opacity-90 active:opacity-80"
        onClick={handleLogin}
        aria-label="Login to Sports Day Event"
      >
        <span className="absolute top-[59px] left-[209px] [font-family:'Inter-SemiBold',Helvetica] font-semibold text-white text-[64px] tracking-[0] leading-[normal]">
          LOGIN
        </span>
      </button>

      <button
        className="top-[1528px] absolute left-[254px] w-[635px] h-[190px] bg-[#151a3a] cursor-pointer transition-opacity hover:opacity-90 active:opacity-80"
        onClick={handleRegister}
        aria-label="Register for Sports Day Event"
      >
        <span className="absolute top-[56px] left-[156px] [font-family:'Inter-SemiBold',Helvetica] font-semibold text-white text-[64px] tracking-[0] leading-[normal]">
          REGISTER
        </span>
      </button>
    </div>
  );
};

import React from "react";
import download11 from "./download-1-1.png";

export const Image = (): JSX.Element => {
  return (
    <div className="w-[3375px] h-[2198px]">
      <img
        className="fixed top-7 left-[1186px] w-[1147px] h-[2170px] aspect-[1.54] object-cover"
        alt="Download"
        src={download11}
      />
    </div>
  );
};
import React, { useState } from "react";
import cricketStadiumUnderDramaticSunsetSkyIlluminatedFieldEmptyStandsWideViewConceptSportChampionshipCalm3855808671 from "./cricket-stadium-under-dramatic-sunset-sky-illuminated-field-empty-stands-wide-view-concept-sport-championship-calm-385580867-1.png";
import rectangle11 from "./rectangle-11.svg";

export const IphoneProMax = (): JSX.Element => {
  const [formData, setFormData] = useState({
    fullName: "",
    gender: "",
    age: "",
    registerNumber: "",
    department: "",
    mobileNumber: "",
    emailId: "",
    eventsToRegister: "",
  });

  const handleInputChange = (
    e: React.ChangeEvent<
      HTMLInputElement | HTMLSelectElement | HTMLTextAreaElement
    >,
  ) => {
    const { name, value } = e.target;
    setFormData((prev) => ({
      ...prev,
      [name]: value,
    }));
  };

  const handleSubmit = (e: React.FormEvent) => {
    e.preventDefault();
    console.log("Form submitted:", formData);
  };

  const formFields = [
    {
      name: "fullName",
      label: "FULL NAME",
      type: "text",
      top: "182px",
      labelTop: "218px",
      labelLeft: "308px",
      height: "130px",
    },
    {
      name: "gender",
      label: "GENDER",
      type: "select",
      top: "364px",
      labelTop: "406px",
      labelLeft: "346px",
      height: "142px",
    },
    {
      name: "age",
      label: "AGE",
      type: "number",
      top: "558px",
      labelTop: "580px",
      labelLeft: "404px",
      height: "136px",
    },
    {
      name: "registerNumber",
      label: "REGISTER NUMBER",
      type: "text",
      top: "754px",
      labelTop: "798px",
      labelLeft: "228px",
      height: "147px",
    },
    {
      name: "department",
      label: "DEPARTMENT",
      type: "text",
      top: "961px",
      labelTop: "997px",
      labelLeft: "322px",
      height: "143px",
    },
    {
      name: "mobileNumber",
      label: "MOBILE NUMBER",
      type: "tel",
      top: "1195px",
      labelTop: "1234px",
      labelLeft: "302px",
      height: "139px",
    },
    {
      name: "emailId",
      label: "EMAIL ID",
      type: "email",
      top: "1408px",
      labelTop: "1458px",
      labelLeft: "391px",
      height: "157px",
    },
    {
      name: "eventsToRegister",
      label: "EVENTS TO REGISTER",
      type: "text",
      top: "1615px",
      labelTop: "1669px",
      labelLeft: "285px",
      height: "137px",
    },
  ];

  return (
    <div className="bg-white w-full min-w-[1106px] min-h-[2174px] relative">
      <img
        className="absolute top-0 left-0 w-[1106px] h-[2174px] aspect-[0.56] object-cover"
        alt="Cricket stadium"
        src={
          cricketStadiumUnderDramaticSunsetSkyIlluminatedFieldEmptyStandsWideViewConceptSportChampionshipCalm3855808671
        }
      />

      <h1 className="absolute top-[7px] left-[63px] [font-family:'Inter-ExtraBold_Italic',Helvetica] font-extrabold italic text-[#e45449] text-[64px] tracking-[0] leading-[normal]">
        EVENT&nbsp;&nbsp;REGISTRATION FORM
      </h1>

      <form onSubmit={handleSubmit}>
        <div className="absolute top-[182px] left-[130px] w-[777px] h-[130px] bg-[#d9d9d9]">
          <input
            type="text"
            name="fullName"
            value={formData.fullName}
            onChange={handleInputChange}
            className="w-full h-full px-4 bg-transparent text-black text-3xl [font-family:'Inter-SemiBold_Italic',Helvetica] font-semibold italic"
            aria-label="Full Name"
            required
          />
        </div>

        <div className="absolute top-[364px] left-[133px] w-[777px] h-[142px] bg-[#d9d9d9]">
          <select
            name="gender"
            value={formData.gender}
            onChange={handleInputChange}
            className="w-full h-full px-4 bg-transparent text-black text-3xl [font-family:'Inter-SemiBold_Italic',Helvetica] font-semibold italic"
            aria-label="Gender"
            required
          >
            <option value="">Select Gender</option>
            <option value="male">Male</option>
            <option value="female">Female</option>
            <option value="other">Other</option>
          </select>
        </div>

        <div className="absolute top-[558px] left-[130px] w-[777px] h-[136px] bg-[#d9d9d9]">
          <input
            type="number"
            name="age"
            value={formData.age}
            onChange={handleInputChange}
            className="w-full h-full px-4 bg-transparent text-black text-3xl [font-family:'Inter-SemiBold_Italic',Helvetica] font-semibold italic"
            aria-label="Age"
            required
          />
        </div>

        <div className="absolute top-[754px] left-[140px] w-[777px] h-[147px] bg-[#d9d9d9]">
          <input
            type="text"
            name="registerNumber"
            value={formData.registerNumber}
            onChange={handleInputChange}
            className="w-full h-full px-4 bg-transparent text-black text-3xl [font-family:'Inter-SemiBold_Italic',Helvetica] font-semibold italic"
            aria-label="Register Number"
            required
          />
        </div>

        <div className="absolute top-[961px] left-[130px] w-[777px] h-[143px] bg-[#d9d9d9]">
          <input
            type="text"
            name="department"
            value={formData.department}
            onChange={handleInputChange}
            className="w-full h-full px-4 bg-transparent text-black text-3xl [font-family:'Inter-SemiBold_Italic',Helvetica] font-semibold italic"
            aria-label="Department"
            required
          />
        </div>

        <div className="absolute top-[1195px] left-[130px] w-[777px] h-[139px] bg-[#d9d9d9]">
          <input
            type="tel"
            name="mobileNumber"
            value={formData.mobileNumber}
            onChange={handleInputChange}
            className="w-full h-full px-4 bg-transparent text-black text-3xl [font-family:'Inter-SemiBold_Italic',Helvetica] font-semibold italic"
            aria-label="Mobile Number"
            required
          />
        </div>

        <div className="absolute top-[1408px] left-[138px] w-[777px] h-[157px]">
          <img
            className="absolute top-0 left-0 w-full h-full"
            alt="Rectangle"
            src={rectangle11}
          />
          <input
            type="email"
            name="emailId"
            value={formData.emailId}
            onChange={handleInputChange}
            className="absolute top-0 left-0 w-full h-full px-4 bg-transparent text-black text-3xl [font-family:'Inter-SemiBold_Italic',Helvetica] font-semibold italic"
            aria-label="Email ID"
            required
          />
        </div>

        <div className="absolute top-[1615px] left-[140px] w-[777px] h-[137px] bg-[#d9d9d9]">
          <input
            type="text"
            name="eventsToRegister"
            value={formData.eventsToRegister}
            onChange={handleInputChange}
            className="w-full h-full px-4 bg-transparent text-black text-3xl [font-family:'Inter-SemiBold_Italic',Helvetica] font-semibold italic"
            aria-label="Events to Register"
            required
          />
        </div>

        <div className="absolute top-[109px] left-[314px] [font-family:'Inter-SemiBold_Italic',Helvetica] font-semibold italic text-white text-[40px] tracking-[0] leading-[normal] whitespace-nowrap">
          FILL&nbsp;&nbsp;THE DETAILS
        </div>

        <label
          htmlFor="fullName"
          className="absolute top-[218px] left-[308px] [font-family:'Inter-SemiBold_Italic',Helvetica] font-semibold italic text-black text-5xl tracking-[0] leading-[normal]"
        >
          FULL NAME
        </label>

        <label
          htmlFor="gender"
          className="absolute top-[406px] left-[346px] [font-family:'Inter-SemiBold_Italic',Helvetica] font-semibold italic text-black text-5xl tracking-[0] leading-[normal]"
        >
          GENDER
        </label>

        <label
          htmlFor="age"
          className="absolute top-[580px] left-[404px] [font-family:'Inter-SemiBold_Italic',Helvetica] font-semibold italic text-black text-5xl tracking-[0] leading-[normal]"
        >
          AGE
        </label>

        <label
          htmlFor="registerNumber"
          className="absolute top-[798px] left-[228px] [font-family:'Inter-SemiBold_Italic',Helvetica] font-semibold italic text-black text-5xl tracking-[0] leading-[normal]"
        >
          REGISTER NUMBER
        </label>

        <label
          htmlFor="department"
          className="absolute top-[997px] left-[322px] w-[339px] [font-family:'Inter-SemiBold_Italic',Helvetica] font-semibold italic text-black text-5xl tracking-[0] leading-[normal]"
        >
          DEPARTMENT
        </label>

        <label
          htmlFor="mobileNumber"
          className="absolute top-[1234px] left-[302px] [font-family:'Inter-SemiBold_Italic',Helvetica] font-semibold italic text-black text-5xl tracking-[0] leading-[normal]"
        >
          MOBILE NUMBER
        </label>

        <label
          htmlFor="emailId"
          className="absolute top-[1458px] left-[391px] [font-family:'Inter-SemiBold_Italic',Helvetica] font-semibold italic text-black text-5xl tracking-[0] leading-[normal]"
        >
          EMAIL ID
        </label>

        <label
          htmlFor="eventsToRegister"
          className="absolute top-[1669px] left-[285px] [font-family:'Inter-SemiBold_Italic',Helvetica] font-semibold italic text-black text-5xl tracking-[0] leading-[normal]"
        >
          EVENTS TO REGISTER
        </label>

        <button
          type="submit"
          className="absolute top-[1918px] left-[458px] w-[596px] h-[157px] bg-[#b51717] cursor-pointer hover:bg-[#9a1414] transition-colors"
          aria-label="Register"
        >
          <span className="absolute top-[50px] left-[181px] [font-family:'Inter-SemiBold_Italic',Helvetica] font-semibold italic text-white text-5xl tracking-[0] leading-[normal]">
            REGISTER
          </span>
        </button>
      </form>
    </div>
  );
};
import React from "react";
import download31 from "./download-3-1.png";
import images2 from "./images-2.png";

export const IphoneProMax = (): JSX.Element => {
  const contactInfo = {
    email: "SAVEETHA ENGINEERING COLLEGE@GMAIL.COM.",
    phoneNumbers: ["8807869640", "98765432101"],
  };

  return (
    <div className="bg-white overflow-hidden w-full min-w-[1176px] min-h-[2174px] relative">
      <img
        className="absolute top-0 left-0 w-[1176px] h-[2174px] aspect-[0.67] object-cover"
        alt="Download"
        src={download31}
      />

      <img
        className="absolute top-[120px] left-[79px] w-[956px] h-[198px] aspect-[4.83] object-cover"
        alt="Images"
        src={images2}
      />

      <h1 className="absolute top-[428px] left-[228px] [font-family:'Inter-SemiBold',Helvetica] font-semibold text-[#131212] text-8xl tracking-[0] leading-[normal]">
        THANK YOU
      </h1>

      <p className="absolute top-[654px] left-[115px] w-[1131px] [font-family:'Inter-SemiBold',Helvetica] font-semibold text-black text-[64px] tracking-[0] leading-[normal]">
        WE ARE EAGERLY WAITING FOR <br />
        YOUR PARTICIPATION IN THE <br />
        SPORTS EVENTS
      </p>

      <h2 className="absolute top-[1345px] left-[228px] [font-family:'Inter-SemiBold',Helvetica] font-semibold text-white text-8xl tracking-[0] leading-[normal]">
        CONTACT US:
      </h2>

      <address className="absolute top-[1473px] left-[291px] [font-family:'Inter-SemiBold',Helvetica] font-semibold text-white text-5xl tracking-[0] leading-[normal] not-italic">
        EMAIL ID:
        <br />
        {contactInfo.email}
        <br />
        <br />
        PNONE NUMBER:
        <br />
        &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
        {contactInfo.phoneNumbers[0]}
        <br />
        &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
        {contactInfo.phoneNumbers[1]}
      </address>
    </div>
  );
};
```


## OUTPUT:

![alt text](<Screenshot 2025-10-08 150848.png>)

![alt text](<Screenshot 2025-10-08 150901.png>)

![alt text](<Screenshot 2025-10-08 150913.png>)

![alt text](<Screenshot 2025-10-08 150921.png>)

## RESULT:
The program to design, develop and deploy a web application for event registration is completed successfully.
