# my2-PremRakesh
# Alasakani Prem Rakesh
###### Hawaii
Hawaii is famous for its **Beaches**</br>
The Resorts provide a lot of options for **Relax and chill**
The Hawaian **climate** and **locations** makes it a tourist attraction
___
### Activities(ordered list)
1. Swim
2. Relax
3. Beach volley
4. Scuba dive
### Food(Unordered list)
* Hawaian delicacies
    * poke
    * laula
* seafood

[link to MyStats.md](MyStats.md)
___
### Tables
The below table has to be followed by the students inorder to maintain proper fitness and overcome fatigue.
| Name of the sport | Reason | Hours in a week |
| --- | --- | ---: |
| Run | Helps Build Stamina | 4 |
| Pushups | Builds upper body and arms | 3 |
| Tennis | Arms, Stamina and concentration | 7 |
| Cycling | Builds lower body | 7 |
___
### Quotes
>"Two things are infinite: the universe and human stupidity; and I'm not sure about the universe. "- *Albert Einstein*
>"There is no law except the law that there is no law." - *John Archibald Wheeler*
___
### Code Fencing
>I am struggling to get the right formula for placing n items onto a circles edge. I have seen many examples but can't get the formulas to work in my code. I have also watched a couple vids on cos, sin, tan but it's not helping me get the right formula for what I want. I suck at math and am also new to js so this is twice as painful.
[link](https://stackoverflow.com/questions/64392955/placing-items-on-a-circles-edge-javascript)
```
/// Mixin to place items on a circle
/// @author Kitty Giraudel
/// @author Ana Tudor
/// @param {Integer} $item-count - Number of items on the circle
/// @param {Length} $circle-size - Large circle size
/// @param {Length} $item-size - Single item size
@mixin on-circle($item-count, $circle-size, $item-size) {
  position: relative;
  width:  $circle-size;
  height: $circle-size;
  padding: 0;
  border-radius: 50%; 
  list-style: none;       
  
  > * {
    display: block;
    position: absolute;
    top:  50%; 
    left: 50%;
    width:  $item-size;
    height: $item-size;
    margin: -($item-size / 2);
  
    $angle: (360 / $item-count);
    $rot: 0;

    @for $i from 1 through $item-count {
      &:nth-of-type(#{$i}) {
        transform: 
          rotate($rot * 1deg) 
          translate($circle-size / 2) 
          rotate($rot * -1deg);
      }

      $rot: $rot + $angle;
    }
  }
}
```
[link](https://css-tricks.com/snippets/sass/placing-items-circle/)
