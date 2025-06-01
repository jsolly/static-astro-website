# Unity Raft-Based Creature Collector: Game Design Plan

## 1. Game Concept

*   **Core Idea:** A fishing game where the player is on a raft. Different types of fish, when caught, pull the raft to different pre-determined spots or types of locations.
*   **Starting Creature:**
    *   Initially water-based.
    *   Design: Fish-like.
*   **Initial Setting:**
    *   Player starts on a basic raft (e.g., wood spars tied together with rope).
    *   Environment primarily water-based.

## 2. Core Mechanics

*   **Creature Catching:**
    *   **Primary Mechanism:** Claw shot (inspired by Legend of Zelda).
        *   Animation: Extends from the raft, snaps shut on the creature, reels it in.
        *   Rationale: Considered potentially easier to animate than a traditional bending fishing rod.
    *   *Initial Idea (alternative):* Traditional fishing rod with bending animation.
*   **Raft Movement:**
    *   Caught creatures are attached to the front of the raft.
    *   The creatures pull the raft through the water to a new spot determined by the type of fish caught.
*   **Creature Behavior (Initial):**
    *   Each fish species, when caught, is associated with a specific destination or type of destination it will pull the raft towards.
    *   Potential for a speed boost if more creatures (or specific combinations) are attached to the raft.
*   **Gold Fish (Exciting & Valuable Catches):**
    *   Gold fish are rare, shimmering, and highly valuable catches that stand out visually and aurally.
    *   Visuals: Gold fish shimmer, glow, or sparkle—immediately recognizable with bright, saturated golds, cel-shaded highlights, and sparkles (Wind Waker style).
    *   Audio: Catching a gold fish triggers a special celebratory sound (e.g., magical chime or coin jingle).
    *   Feedback: Catching a gold fish creates a burst of golden particles or a "shower of coins" effect.
    *   Gameplay: Gold fish can be used as currency for upgrades, unlocking new areas, or cosmetic items. They may also grant temporary bonuses (e.g., speed boost, unique destinations).
    *   Rarity: Gold fish are rare, making their appearance a special event and encouraging collection.
    *   Lore: Gold fish could be legendary or magical creatures, with stories or myths attached.
    *   Collection: Add a "Gold Fish Collection" or trophy system to encourage players to seek them out.

## 3. Progression & World

*   **Creature Collection:** The primary progression involves discovering and catching different types of fish to unlock new areas.
*   **Environment:** Starts on a floating pontoon/raft in a water-based world. New water environments are unlocked by catching specific fish.

## 4. Game Feel & "Juiciness" (Sensory Feedback)

*   **Essential Feedback Elements:**
    *   **Catching a Creature:**
        *   Visuals: Splash, line/claw animation.
        *   Audio: Triumphant sound effect, "snap" or "clamp" of the claw.
    *   **Raft Movement (Pulled by Creature):**
        *   Movement Feel (Inspired by The Legend of Zelda: Wind Waker):
            *   The raft glides smoothly, with gentle bobbing and tilting as it moves, evoking the feel of Wind Waker's boat.
            *   Acceleration is gradual, with a sense of weight and momentum—movement is never instant or jerky.
            *   The raft responds to water physics: small waves, splashes, and a visible wake behind it.
            *   Subtle camera sway or follow effects enhance immersion.
        *   Visuals, Textures, and Colors (Wind Waker Inspiration):
            *   Art Style: Bright, saturated colors; simple, bold shapes; soft, painterly textures; and possible outlines or subtle shading for a cartoon-like effect.
            *   Water: Stylized water shader with visible wave lines, animated foam, and sparkles/reflections on the surface.
            *   Lighting: Bright, dynamic lighting with soft shadows; consider a day/night cycle for added atmosphere.
        *   Game Feel Enhancements:
            *   When the raft is pulled, add a slight shake and bounce, water spray and foam at the front and sides, and whooshing/splashing sound effects.
            *   When catching a creature, use bright, celebratory effects (sparkles, colorful bursts) and joyful sounds.
        *   Open Questions:
            *   Should the cel-shaded look apply to all assets or just water/raft?
            *   Should the raft always move in a straight line to the destination, or allow some player steering (like Wind Waker's sailboat)?
            *   Are there specific color palettes or references to use for the world/creatures?
*   **Creature Sounds:**
    *   **Rewarding Catch Sound (A Celebration!):**
        *   Inspiration: Bright and celebratory sounds like a dolphin's chirp (playful, joyful, magical) or a clear trilling songbird (e.g., thrush, nightingale - signifying triumph and upliftment).
        *   Characteristics: Short, crisp, memorable, possibly with a slight echo for immersion, creating a moment of celebration for the player.
    *   **Gameplay Cue Sounds:**
        *   Line/Chain Tension:
            *   Elastic line: Tight, creaky twang (signals biting or struggling).
            *   Metal chain: Sharp, clanking rattle (signals sudden movement or high tension).

## 5. Climax / End Game / Lose State Concept
*   **Win State (Fish Celebration):**
    *   The final area is teeming with fish, jumping out of the water in celebration.
    *   Fish might even jump into the player's boat, creating a joyous and chaotic scene.
    *   This creates a visually exciting and rewarding conclusion for the player.
*   **Lose State (Giant Fish Eats You):**
    *   A giant fish appears and eats the player's raft.
    *   The player ends up inside the fish (like Jonah).
    *   Inside the fish, the player might find evidence of previous losses (e.g., other rafts that were eaten).
    *   This could be a humorous and memorable way to handle the lose state, and potentially a unique environment to explore or escape from.

## 7. Initial Player Experience - Immediate Gratification

*   **Option 1: "Freebie" First Catch:**
    *   A fish jumps onto the deck of the raft.
    *   Player uses the harpoon gun/claw shot to "shoot" it for an instant first catch.
    *   Sounds: Loud splash (fish jumping), quick harpoon whoosh, triumphant thud (fish secured). (This is the one I'm leaning towards)

## 8. Key Assets Required (Beyond Initial Character/Raft)

*   **Models:**
    *   Various fish/creature models (for collection).
*   **Effects:**
    *   Water interaction effects (splashes, sprays, wakes).
*   **Sound Effects (General):**
    *   Ambient water sounds.
    *   Interactions (claw deploying, retracting, impacts).
    *   Celebration sounds (e.g., dolphin chirp, songbird trill).
    *   Water sounds (e.g., whooshing, splashing).
    *   Fishing rod bending sound (e.g., creaky twang).
    *   Metal chain clanking sound (e.g., sharp rattle).
    *   Fish biting sound (e.g., crunching).
    *   Fish thrashing sound (e.g., splashing).
    *   Fish jumping sound (e.g., splash).
    *   Fish swimming sound (e.g., whooshing).


## 9. Prototyping Considerations

*   **Raft Physics (Unity Engine):**
    *   Considered feasible for a prototype.
    *   Utilize Unity's built-in physics engine.
    *   Focus on tweaking buoyancy and drag settings for a satisfying feel.
    *   Initial goal: Smooth, steady movement pulled by the fish to a new location.
*   **Sound in Initial Rough Prototype:**
    *   Not strictly *necessary* but highly *recommended* for game feel.
    *   Even basic placeholder sounds (e.g., a simple click for catch, a whoosh for movement) can significantly improve testing feedback and engagement.

## 10. Inspirational Games (Mechanics, Feel, Mini-games)

*   **Raft-like / Survival:**
    *   `Raft` (resource gathering, survival on a drifting platform)
*   **Underwater Exploration / Creature Interaction:**
    *   `Subnautica` (underwater exploration, taming aquatic creatures, base-building) - *Focus on exploration aspect*.
*   **Satisfying Fishing Mechanics:**
    *   `Stardew Valley` (tricky but rewarding fishing mini-game)
    *   `Dredge` (fishing adventure with dark, gripping narrative and tense mechanics)