# ThreeFold Circles

![](img/circles.jpeg)

## Circles Demystified

Circles are teams of people working on shared tasks, products, services. They are organized around stories, that have the agreement of shareholders. Circles have owners that are not in charge, but support everybody in the circle to reach their goals. The circle owner is also responsible for the set targets, goal or objective. Circles become obsolete when the goals have been reached. Objective is to create small circles with clear stories, responsible capable owners and motivated circle members.

Below picture visualizes the [ThreeFold Foundation Circle](/circles/foundation/foundation.md) and its subcircles, with in each circle the name of the owner:

```mermaid

graph TB; 
    Foundation((Foundation<BR>Kristof)) --- TFLove((TFLove<br>Olivia))
    Foundation --- TFGRID((TFGRID<br>Andreas))
    Foundation --- TFTOKENS((TFTOKENS<br>Adnan))
    Foundation --- Community{Community}
    Foundation --- Org{Org<br>See Below}
    Community --- Europe{Europe}
    Community --- Global{Global}
    Foundation --- TFInnovate((TFInnovate<br>Kristof<br>Incubation))
    Foundation --- TFImpact((TFImpact<br>Chris<br>Africa Fund))

    Community --- TFAmbassadors((Ambassadors<br>Owen))
    Europe --- CommunityIbiza((Community<br>Ibiza<br>???<br>???))
    Europe --- CommunityGreen((Community<br>???<br>???))
    Global --- CommunityVeda((Community<br>Students<br>Celebrities<br>Isabelle<br>Adnan))
    Global --- Veda((Awareness<br>Veda<br>Isabelle))
 

    classDef circle text-align:center,stroke:#33,stroke-width:3px;  

    class Foundation,TFLove,TFGRID,TFTOKENS,TFAmbassadors,TFInnovate,TFImpact,CommunityIbiza,CommunityVeda,CommunityGreen,Veda,Crypto,Org circle;

    click TFGRID "https://threefoldfoundation.github.io/info_foundation/#/circles/foundation/grid/grid"

```

And this picture visualizes the [ThreeFold Organization Circle](/circles/tf_organization/tf_organization.md) and its subcircles, again with in each circle the name of the owner:

```mermaid

graph TB; 
    Foundation{Foundation<br>Organization}
    Foundation --- Web((Web<br>Wiki<br>Roel))
    Foundation --- Support((Support<br>Sabrina))
    Foundation --- IT((Tools/IT<br>Ramez))
    Foundation --- Tech((Technology<br>Kristof))
    Tech  --- TFPlatform((TF-Platform<br>Reem/Christophe))
    Tech  --- TFCHain((TF-Chain<br>Rob))

    classDef circle text-align:center,stroke:#33,stroke-width:3px;  

    class Web,Support,IT,Tech,Evangelization circle;


```

## [**ThreeFold Foundation Circle**](/circles/foundation/foundation.md)  

  
### ThreeFold Cooperative Circles
  
  - [**BetterToken Circle**](/circles/bettertoken/bettertoken.md)
  - [**Mazraa Circle**](/circles/mazraa/mazraa.md)

### How to work together

- [Collaboration at ThreeFold](/collaboration/README.md)
