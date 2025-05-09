<script lang="ts">
  type OpenSpaceData = {
    days: {
      [key: string]: DayData,
    }
  }

  type DayData = {
    times: {
      [key: string]: TimeData,
    }
  }

  type TimeData = {
    rooms: {
      [key: string]: ActivityData,
    }
  }

  type ActivityData = {
    name: string,
    mastodon?: string,
  }

  let openSpaceData: OpenSpaceData = {
    days: {
      "2024-05-17": {
        times: {
          "08:00": {
            rooms: {
              "308": {
                name: "",
              },
              "309": {
                name: "",
              },
              "315": {
                name: "",
              },
              "316": {
                name: "",
              },
              "318": {
                name: "",
              },
              "320": {
                name: "",
              },
              "321": {
                name: "",
              },
            }
          },
          "09:00": {
            rooms: {
            }
          },
          "10:00": {
            rooms: {
            }
          },
          "11:00": {
            rooms: {
              "309": {
                name: "Python Professional Educators from Australia/NZ",
              },
              "315": {
                name: "Open Source AI Workshop",
              },
              "316": {
                name: "Software Testing",
              },
              "318": {
                name: "FastAPI (Backend dev in Python)",
              },
              "320": {
                name: "Music and Audio",
              },
              "321": {
                name: "",
              },
            }
          },
          "12:00": {
            rooms: {
              "315": {
                name: "Open Source AI Workshop",
              },
            }
          },
          "13:00": {
            rooms: {
              "309": {
                name: "NYC Pythonistas",
              },
              "316": {
                name: "Boston Python: en español",
              },
            }
          },
          "14:00": {
            rooms: {
              "308": {
                name: "Healthcare (IT) Industry Professionals",
              },
              "309": {
                name: "Wagtail CMS and Django",
                mastodon: "#WagtailCMS and #Django"
              },
              "315": {
                name: "Civic Tech",
              },
              "316": {
                name: "Microsoft Azure Container Apps",
                mastodon: "#Microsoft #Azure Container Apps"
              },
              "318": {
                name: "PyBay 2024",
                mastodon: "#PyBay 2024"
              },
              "320": {
                name: "Pandas / Tabular Data",
              },
              "321": {
                name: "Sad Python Girls Podcast",
              },
            }
          },
          "15:00": {
            rooms: {
              "308": {
                name: "Healthcare (IT) Industry Professionals",
              },
              "309": {
                name: "Python in Aviation",
              },
              "315": {
                name: "What improv comedy canm teach you about communication and collaboration",
              },
              "316": {
                name: "Property Based Testing",
              },
              "318": {
                name: "Queer Trans Meetup",
              },
              "320": {
                name: "Vim",
              },
              "321": {
                name: "Data Pipelines",
              },
            }
          },
          "16:00": {
            rooms: {
              "308": {
                name: "Tech Nomads",
              },
              "309": {
                name: "Female Founder Coffee",
              },
              "315": {
                name: "Python Discord Meetup",
              },
              "316": {
                name: "Trio and Structured Computing",
              },
              "318": {
                name: "Pickleball",
              },
              "320": {
                name: "JITs",
              },
              "321": {
                name: "SQL and Python (DuckDB and Ibis)",
                mastodon: "SQL and Python (@duckdb@mastodon.social and Ibis)"
              },
            }
          },
          "17:00": {
            rooms: {
              "308": {
                name: "Game Development",
              },
              "309": {
                name: "Co-op board games",
              },
              "320": {
                name: "Learn ASL with Python",
              },
            }
          },
          "18:00": {
            rooms: {
              "309": {
                name: "Mobbing / Team programming",
              },
            }
          },
          "19:00": {
            rooms: {
              "315": {
                name: "Code Reading Club",
              },
            }
          },
        }
      },
      "2024-05-18": {
        times: {
          "08:00": {
            rooms: {
              "308": {
                name: "",
              },
              "309": {
                name: "Python Professional Educators from Australia/NZ",
              },
              "315": {
                name: "",
              },
              "316": {
                name: "",
              },
              "318": {
                name: "",
              },
              "320": {
                name: "",
              },
              "321": {
                name: "",
              },
            }
          },
          "09:00": {
            rooms: {
              "308": {
                name: "Python in Excel",
              },
              "309": {
                name: "Open Source Architect Community",
              },
              "321": {
                name: "Don't talk about overemployment",
              },
            }
          },
          "10:00": {
            rooms: {
              "308": {
                name: "Conda & friends",
                mastodon: "@conda@fosstodon.org and friends",
              },
              "309": {
                name: "Performance Testing in CI",
              },
              "315": {
                name: "OWASP/Cybersecurity for devs",
                mastodon: "#OWASP and Cybersecurity"
              },
              "318": {
                name: "AI + Coding",
                mastodon: "#AI and Coding"
              },
              "320": {
                name: "Working orchestration with Prefect",
              },
              "321": {
                name: "Neurodivergent people meet+greet",
              },
            }
          },
          "11:00": {
            rooms: {
              "308": {
                name: "MicroPython",
                mastodon: "@micropython@fosstodon.org"
              },
              "309": {
                name: "Nix, NixOS, Nixpkgs",
                mastodon: "@nix@programming.dev",
              },
              "315": {
                name: "Python + CUDA",
                mastodon: "#Python + #CUDA",
              },
              "316": {
                name: "Data Engineering Patterns for Healthcare",
              },
              "318": {
                name: "High Schoolers",
              },
              "320": {
                name: "Learning Rust",
                mastodon: "@rust@social.rust-lang.org",
              },
              "321": {
                name: "Data Science Meetup",
              },
            }
          },
          "12:00": {
            rooms: {
              "308": {
                name: "Single Node Data Processing",
              },
              "309": {
                name: "Bash + other terminals + tools",
              },
              "315": {
                name: "Interview Question Practice",
              },
              "316": {
                name: "Using Python with Apache Beam and Apache Airflow",
                mastodon: "Using Python with #Apache Beam and @airflow@fosstodon.org",
              },
              "318": {
                name: "LiteStar Bug Bash",
              },
              "320": {
                name: "Geospatial",
              },
              "321": {
                name: "Python APAC",
              },
            }
          },
          "13:00": {
            rooms: {
              "308": {
                name: "Lets Talk Math",
              },
              "309": {
                name: "How do you know your app is production-ready?",
              },
              "315": {
                name: "Research Software Engineer",
              },
              "316": {
                name: "Outdoor Adventure Enthusiast",
              },
              "318": {
                name: "Functional Error Handling",
              },
              "320": {
                name: "Python Types in Practice",
              },
              "321": {
                name: "Educators meetup",
              },
            }
          },
          "14:00": {
            rooms: {
              "308": {
                name: "Research Engineering",
              },
              "309": {
                name: "Right to Repair",
              },
              "315": {
                name: "PyScript",
              },
              "316": {
                name: "Python Learning",
                mastodon: "@PythonMorsels@mastodon.social",
              },
              "318": {
                name: "PyBay 2024",
                mastodon: "@pybay@fosstodon.org #PyBay2024"
              },
              "321": {
                name: "How to wear a Kimono",
              },
            }
          },
          "15:00": {
            rooms: {
              "308": {
                name: "P.A.O. - Python Asia Organization",
              },
              "309": {
                name: "Black Python Devs & AfroPython",
                mastodon: "@blackpythondevs@mastodon.social and AfroPython",
              },
              "315": {
                name: "Getting started with Temporal",
              },
              "316": {
                name: "Profile Pic Palooza",
              },
              "318": {
                name: "Infrastructure Code BoF",
              },
              "320": {
                name: "Bug detection in projects",
              },
              "321": {
                name: "Python Help",
              },
            }
          },
          "16:00": {
            rooms: {
              "308": {
                name: "Fediverse / Mastodon",
              },
              "309": {
                name: "Automate Python Code Optimization",
              },
              "315": {
                name: "Dr Chuck",
                mastodon: "@drchuck@openedtech.social",
              },
              "316": {
                name: "RenPy and Visual Novel Meetup",
                mastodon: "#RenPy and Visual Novel Meetup",
              },
              "318": {
                name: "Azure",
                mastodon: "#Azure",
              },
              "320": {
                name: "Faster CPython",
              },
              "321": {
                name: "Space",
              },
            }
          },
          "17:00": {
            rooms: {
              "308": {
                name: "Django + OIDC",
                mastodon: "#Django + OIDC"
              },
              "309": {
                name: "Randomized Pictorial Paper Forecasting (Tarot)",
              },
              "315": {
                name: "Startups / Bootstrappers / Indie Hackers",
              },
              "316": {
                name: "Computer Vision",
              },
              "318": {
                name: "Flask, ThreeJS, WebGL",
              },
              "320": {
                name: "Python for Test + Measurement",
              },
              "321": {
                name: "STEM Scout Merit Badge Instruction",
              },
            }
          },
          "18:00": {
            rooms: {
              "308": {
                name: "Body Wake Up",
              },
            }
          },
        }
      },
      "2024-05-19": {
        times: {
          "08:00": {
            rooms: {
              "308": {
                name: "",
              },
              "309": {
                name: "",
              },
              "310/311": {
                name: "",
              },
              "315": {
                name: "",
              },
              "316": {
                name: "",
              },
              "318": {
                name: "",
              },
              "319": {
                name: "",
              },
              "320": {
                name: "",
              },
              "321": {
                name: "",
              },
            }
          },
          "09:00": {
            rooms: {
            }
          },
          "10:00": {
            rooms: {
              "308": {
                name: "Self Hosting",
              },
              "309": {
                name: "pyOpenSci",
                mastodon: "@pyOpenSci@fosstodon.org",
              },
              "310/311": {
                name: "Meetup of Meetups Organizers",
              },
              "315": {
                name: "SQL might be good?",
              },
              "316": {
                name: "Real World Python",
              },
              "318": {
                name: "Starting Your Python Community",
              },
              "319": {
                name: "Open Source Architect Community",
              },
              "320": {
                name: "AI/LLMs",
              },
            }
          },
          "11:00": {
            rooms: {
              "308": {
                name: "Spyder",
                mastodon: "@Spyder@fosstodon.org",
              },
              "309": {
                name: "Qt and PySide",
                mastodon: "@qt@floss.social and #PySide",
              },
              "310/311": {
                name: "Rock, Paper, Scissors! Competition",
              },
              "315": {
                name: "Py5: Creative Coding with Python",
                mastodon: "@py5coding@fosstodon.org"
              },
              "316": {
                name: "Solo Dev or Tiny Biz?",
              },
              "318": {
                name: "How can we improve DevX?",
              },
              "319": {
                name: "NYC People Meetup",
              },
              "320": {
                name: "My Users Use Python",
              },
            }
          },
          "12:00": {
            rooms: {
            }
          },
          "13:00": {
            rooms: {
              "308": {
                name: "Twisted BoF",
                mastodon: "#Twisted BoF"
              },
              "309": {
                name: "Python and Sports Analytics",
              },
              "310/311": {
                name: "Climate Tech",
              },
              "315": {
                name: "Protecting Python Code",
              },
              "316": {
                name: "Data Storytelling",
              },
              "318": {
                name: "Quants & Financial Analysts Meetup",
              },
              "319": {
                name: "Sushi",
              },
              "320": {
                name: "Fix your estimation",
              },
              "321": {
                name: "Web Frameworks",
              },
            }
          },
          "14:00": {
            rooms: {
              "308": {
                name: "Bayesian Statistics"
              },
              "309": {
                name: "Internal AI Tooling",
              },
              "310/311": {
                name: "Creator Economy",
              },
              "315": {
                name: "20th Anniversary of Beautiful Soup",
                mastodon: "20th Anniversary of #BeautifulSoup"
              },
              "316": {
                name: "QA Automation",
              },
              "318": {
                name: "PyScript + PySheets Spreadsheets",
                mastodon: "#PyScript + #PySheets Spreadsheets"
              },
              "319": {
                name: "Ricing",
              },
              "320": {
                name: "Advanced Knitting Theory",
              },
            }
          },
          "15:00": {
            rooms: {
              "308": {
                name: "Motorcycles are dope",
              },
              "309": {
                name: "Real Estate Data Meetup",
              },
              "310/311": {
                name: "State of AI Tools",
              },
              "315": {
                name: "Ensemble Programming",
              },
              "316": {
                name: "GDS Factory",
              },
              "318": {
                name: "Ray",
              },
              "319": {
                name: "First time? Make friends!",
              },
              "320": {
                name: "Nominating Pythonistas",
              },
              "321": {
                name: "Pydantic & LogFire",
                mastodon: "#Pydantic & #LogFire"
              },
            }
          },
          "16:00": {
            rooms: {
              "308": {
                name: "State of W...",
              },
              "309": {
                name: "Quick Rust Chat",
                mastodon: "Quick #Rust Chat",
              },
              "310/311": {
                name: "Framework Laptops",
                mastodon: "@frameworkcomputer@fosstodon.org Laptops",
              },
              "315": {
                name: "So you want to become a farmer",
              },
              "316": {
                name: "Meet the Astral team",
                mastodon: "Meet the #Astral team",
              },
              "318": {
                name: "PyFlink",
                mastodon: "#PyFlink",
              },
              "319": {
                name: "Book! ML! Okay!",
              },
            }
          },
          "17:00": {
            rooms: {
            }
          },
          "18:00": {
            rooms: {
              "308": {
                name: "Board Games"
              }
            }
          },
          "19:00": {
            rooms: {
              "309": {
                name: "Social Dancing"
              },
              "310/311": {
                name: "Python and Rust",
                mastodon: "#Python and #Rust"
              }
            }
          },
        }
      }
    }
  }
</script>

{#each Object.entries(openSpaceData.days) as [date, dayData]}
{@const roomNames = Object.keys(Object.values(dayData.times)[0].rooms).toSorted((a, b) => a.split("/")[0].localeCompare(b.split("/")[0]))}
<table class="table-auto border border-black">
  <thead>
    <tr>
      <th colspan={roomNames.length + 1}>{date}</th>
    </tr>
    <tr>
      <th></th>
      {#each roomNames as room}
      <th class="border border-black p-1">{room}</th>
      {/each}
    </tr>
  </thead>
  <tbody>
    {#each Object.entries(dayData.times) as [time, timeData]}
    <tr>
      <th class="border border-black p-1">{time}</th>
      {#each roomNames as roomName}
      {@const activity = timeData.rooms[roomName]}
      <td class="border border-black p-1">
        {activity?.name}
      </td>
      {/each}
    </tr>
    {/each}
  </tbody>
</table>
{/each}
