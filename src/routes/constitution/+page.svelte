<script>
    import { dues } from '$lib/utils/helper';
    let one, oneOne, oneOneOne, oneTwo, oneTwoOne, oneTwoTwo, oneTwoThree, oneTwoFour, oneTwoFive, oneThree;
    let two, twoOne, twoTwo, twoThree;
    let three, threeOne;
    let four, fourOne, fourTwo;
    let five, fiveOne;
    let six, sixOne, sixTwo, sixThree;
    let seven, sevenOne, sevenTwo, sevenThree;

    const goToSection = (section) => {
        const top = section.getBoundingClientRect().top + window.pageYOffset;
        window.scrollTo({left: 0, top, behavior: 'smooth'});
    }
</script>

<style>
    .constitution {
        position: relative;
        z-index: 1;
        width: 92%;
        max-width: 800px;
        margin: 8em auto 10em;
    }

    h1 {
        font-size: 2em;
        line-height: 1.2em;
        text-align: center;
        margin: 2em 0 1.5em;
    }

    h2 {
        font-size: 1.5em;
        line-height: 1.2em;
    }

    h3 {
        text-decoration: underline;
        font-size: 1.3em;
        line-height: 1.2em;
    }

    h4 {
        text-decoration: underline;
        margin-left: 2em;
        font-size: 1.2em;
        line-height: 1.2em;
    }

    h5 {
        margin-left: 6em;
        font-size: 0.8em;
        line-height: 1.1em;
    }

    .subBlock {
        margin-left: 2.4em;
    }

    .sectionHeading {
        margin: 4em 0 1.5em;
    }

    .subSectionHeading {
        margin: 1.5em 0 1.5em;
    }

    .underscore {
        text-decoration: underline;
    }

    .right {
        text-align: right;
    }

    .positionMaximums td {
        min-width: 3em;
    }

    .noUnderscore {
        text-decoration: none;
    }

    .clickable {
        cursor: pointer;
    }

    .clickable:hover {
        color: #00316b;
    }

    p {
        color: #777;
    }
</style>

<div class="constitution">
    <h1 class="noUnderscore">LEGENDS LEAGUE CONSTITUTION</h1>
    
    <h2 class="noUnderscore">TABLE OF CONTENTS</h2>
    
    <h3 class="noUnderscore clickable" onclick={() => goToSection(one)}>Section 1: Roster</h3>
        <h4 class="noUnderscore clickable" onclick={() => goToSection(oneOne)}>1.1 Positional Breakdown</h4>
        <h4 class="noUnderscore clickable" onclick={() => goToSection(oneTwo)}>1.2 Trading</h4>
            <h5 class="noUnderscore clickable" onclick={() => goToSection(oneTwoOne)}>1.2.1 Trade Collusion</h5>
            <h5 class="noUnderscore clickable" onclick={() => goToSection(oneTwoTwo)}>1.2.2 Lending Players Prohibition</h5>
            <h5 class="noUnderscore clickable" onclick={() => goToSection(oneTwoThree)}>1.2.3 Trade Deadline</h5>
            <h5 class="noUnderscore clickable" onclick={() => goToSection(oneTwoFour)}>1.2.4 Trade Restrictions</h5>
            <h5 class="noUnderscore clickable" onclick={() => goToSection(oneTwoFive)}>1.2.5 Veto/Trade Process</h5>
        <h4 class="noUnderscore clickable" onclick={() => goToSection(oneThree)}>1.3 Waiver Wire</h4>
    
    <h3 class="noUnderscore clickable" onclick={() => goToSection(two)}>Section 2: Drafting</h3>
    
        <h4 class="noUnderscore clickable" onclick={() => goToSection(twoOne)}>2.1 Draft Order</h4>
    
    <h3 class="noUnderscore clickable" onclick={() => goToSection(three)}>Section 3: Scoring System</h3>
    
        <h4 class="noUnderscore clickable" onclick={() => goToSection(threeOne)}>3.1 Scoring System</h4>
    
    <h3 class="noUnderscore clickable" onclick={() => goToSection(four)}>Section 4: Postseason</h3>
    
        <h4 class="noUnderscore clickable" onclick={() => goToSection(fourOne)}>4.1 Playoffs</h4>
        <h4 class="noUnderscore clickable" onclick={() => goToSection(fourTwo)}>4.2 Playoffs Seeding Tiebreakers</h4>

    <h3 class="noUnderscore clickable" onclick={() => goToSection(five)}>Section 5: Tanking Policy</h3>
    
        <h4 class="noUnderscore clickable" onclick={() => goToSection(fiveOne)}>5.1 League Tanking Policy</h4>

    <h3 class="noUnderscore clickable" onclick={() => goToSection(six)}>Section 6: Replacing Managers</h3>
    
        <h4 class="noUnderscore clickable" onclick={() => goToSection(sixOne)}>6.1 Removing Managers</h4>
        <h4 class="noUnderscore clickable" onclick={() => goToSection(sixTwo)}>6.2 Replacing Managers</h4>
        <h4 class="noUnderscore clickable" onclick={() => goToSection(sixThree)}>6.3 Replacement Incentive</h4>

    <h3 class="noUnderscore clickable" onclick={() => goToSection(seven)}>Section 7: League Finances</h3>
    
        <h4 class="noUnderscore clickable" onclick={() => goToSection(sevenOne)}>7.1 League Entry Fees</h4>
        <h4 class="noUnderscore clickable" onclick={() => goToSection(sevenTwo)}>7.2 Payout</h4>
        <h4 class="noUnderscore clickable" onclick={() => goToSection(sevenThree)}>7.3 Raising Fees</h4>

    <h3 class="noUnderscore clickable" onclick={() => goToSection(eight)}>Section 8: In-Season/Off-Season</h3>

        <h4 class="noUnderscore clickable" onclick={() => goToSection(eightOne)}>8.1 In-Season League Changes</h4>
        <h4 class="noUnderscore clickable" onclick={() => goToSection(eightTwo)}>8.2 Off-Season League Changes</h4>
    
    <hr />
    
    <h2 class="sectionHeading" bind:this={one}>Section 1: Team Roster </h2>
    
    <h3 class="subSectionHeading" bind:this={oneOne}>1.1 Positional Setup</h3>
    
    <p class="underscore">Starters</p>
    <ul>
        <li>1 x QB</li>
        <li>2 x RB</li>
        <li>2 x WR</li>
        <li>1 x TE</li>
        <li>2 x FLEX (RB/WR/TE)</li>
        <li>1 x D/ST</li>
        <li>1 x K</li>
    </ul>
    
    <p>6 x Bench spots</p>

    <p>2 x IR Spots (Players must be marked as IR, Suspended, or COVID in the Sleeper app to be eligible for IR spots)</p>


    <h3 class="subSectionHeading" bind:this={oneTwo}>1.2 Trading</h3>
    
    <p>Trades will be processed immediately.</p>
    <p>Trades may be reversed if flagged and found to involve collusion.</p>
    <p>Tradable assets include players and current-season FAAB dollars.</p>
    
    <h4 bind:this={oneTwoOne}>1.2.1 Trade Collusion</h4>
    <div class="subBlock">
        <p>If any manager is found to be offering or accepting bribes, trading non-fantasy assets, or otherwise colluding to unfairly enhance a team:</p>
        
        <ul>
            <li>First Offense: I80% reduction in FAAB budget</li>
            <li>Second Offense: 8-week freeze on trades and waiver access</li>
            <li>Third Offense: League meeting to determine further action</li>
        </ul>

        <p>Colluded trades will be reversed. If game outcomes were affected, match results may be retroactively adjusted.</p>

        <p>The commissioner will lean toward letting managers manage their teams—but reserves the right to review trades and assess intentions in extreme cases.</p>
    </div>

    <h4 bind:this={oneTwoTwo}>1.2.2 Lending Players (Reacquisition Rule)</h4>
    <div class="subBlock">
        <p>A manager may not re-acquire a traded player within 3 weeks of the original trade unless the deal is clearly in good faith and approved by the league. Repeat trade-backs may trigger a collusion review.</p>
    </div>
    
    <h4 bind:this={oneTwoThree}>1.2.3 Trade Deadline</h4>
    <div class="subBlock">
        <p>The trade deadline is <strong>Week 12</strong> of the NFL regular season.</p>
    </div>
    
    <h4 bind:this={oneTwoFour}>1.2.4 Trade Restrictions</h4>
    <div class="subBlock">
        <p>You may only trade FAAB $ from the current season.</p>
    </div>
    
    <h4 bind:this={oneTwoFive}>1.2.5 Veto/Trade Process</h4>
    <div class="subBlock">
        <p>A total of 7 veto votes are required to veto a trade. Vetoes are only appropriate in instances of collusion or an egregious mismatch of value (i.e. CMC for a backup kicker). Not liking a trade does not warrant a veto.</p>
    </div>
     
    
    <h3 bind:this={oneThree}>1.3 Waiver Wire</h3>
    
    <p>FAAB Waiver wire system. Each team will begin the season with $100. $0 bids are allowed. Bids will be processed on Wednesdays at 8 AM BST.</p>

    <p>If multiple Managers bid for the same player, the manager with the highest claim will win the player. In the likelihood that multiple managers bid the same amount, the tie-breaker will be the reverse order of standings.</p>

    <p>FAAB budgets will reset each season.</p>
    
    <h2 class="sectionHeading" bind:this={two}>Section 2: Drafting</h2>
    
    <h3 bind:this={twoOne}>2.1 Draft Order</h3>
    <p>The draft order each year will be randomised in the form of a Snake draft.</p>
    
    <h2 class="sectionHeading" bind:this={three}>Section 3: Scoring System</h2>

    <h3 bind:this={threeOne}>3.1 Scoring System</h3>
    <p>The league scoring system breakdown is listed on the Sleeper fantasy app (for the most part, it follows typical .5PPR Scoring).</p>
    
    <h2 class="sectionHeading" bind:this={four}>Section 4: Postseason</h2>
    
    <h3 bind:this={fourOne}>4.1 Playoffs</h3>
    <p>At the end of the season 6 teams will make the playoffs. The first round of playoffs will commence in week 15. The top 2 teams will receive a bye week in the first round of the playoffs. Each playoff matchup will only last one week and the winner will advance. Week 17 is the Dirty Soda Bowl Championship game. Week 18 will not be used.</p>
    
    <h3 bind:this={fourTwo}>4.2 Seeding Tiebreakers</h3>
    <p>If two teams finish with the same record the tiebreakers will go as follows:</p>

    <ol>
        <li>Points For</li>
        <li>Head 2 Head Record</li>
        <li>Total Points Against</li>
        <li>Coin Flip</li>
        <li>Duel to the death</li>
    </ol>

    <h2 class="sectionHeading" bind:this={five}>Section 5: Tanking Policy</h2>
    
    <h3 bind:this={fiveOne}>5.1 League Tanking Policy</h3>
    <p>No team may intentionally leave starting roster spots empty. Any evidence of intentionally leaving roster spots empty in order to improve your draft position may be subject to punishment, including a suspension from using the waiver wire the following week. Repeat offenders will face being kicked out of the league.</p>

    <h2 class="sectionHeading" bind:this={six}>Section 6: Replacing Managers</h2>
    
    <h3 bind:this={sixOne}>6.1 Removing Managers</h3>
    <p>Short of continuously failing to set a valid lineup, or confirmed collusion, no manager can be removed against their will. Participation, through the league chat, trade offers, and the waiver wire.</p>
    
    <h3 bind:this={sixTwo}>6.2 Replacing Managers</h3>
    <p>When a manager needs to be replaced, the commissioner will try to find a suitable candidate with some connection to at least a portion of the existing managers. Priority will be placed on managers who will not upset the balance but are committed to driving up competitiveness within the league.</p>
    
    <h3 bind:this={sixThree}>6.3 Replacement Incentive</h3>
    <p> If a manager chooses to quit the league or is removed by a commissioner, an incoming manager is offered a 50% reduction on their first-year buy-in.</p>

    <h2 class="sectionHeading" bind:this={seven}>Section 7: League Finances</h2>
    
    <h3 bind:this={sevenOne}>7.1 League Entry Fees</h3>
    <p>League entry fees are set at £10.00 per manager. Fees are collected by the commissioner and collection will be sent out no later than the first of August. All managers must be fully paid up before the start of the regular season. If a manager fails to pay before the deadline, a 10% penalty will be added to their payment and will go towards the payouts at the end of the year.</p>
    
    <h3 bind:this={sevenTwo}>7.2 Payout</h3>
    <p>League payout is structured as follows:</p>
    <ul>
        <li>1st place: £85.00</li>
        <li>2nd place: £10.00</li>
        <li>Highest Regular Season Point Scorer: £25.00</li>
    </ul>
    <p>In the event that a manager is fined due to late payment, their extra fee will be added to the winner's payout. Similarly, if new managers come into the league and the payout is smaller, the difference will come out of the winner's prize.</p>
    
    <h3 bind:this={sevenThree}>7.3 Raising Dues</h3>
    <p>A majority vote is required in order to raise league entry fees. In the event that a manager is no longer financially comfortable with the buy-in, finding a co-manager to split the cost is recommended.</p>

    <h2 class="sectionHeading" bind:this={eight}>Section 8: In-Season/Off-Season</h2>

    <h3 bind:this={eightOne}>8.1 In-Season League Changes</h3>
    <p>Beginning in the 2025 season, the league has approved the ability to implement rule changes during the season. This is intended to provide flexibility for addressing unforeseen issues, loopholes, format inconsistencies, or broken mechanics.</p>

    <p>The deadline for proposing in-season changes is the end of Week 6 of the regular season. Any proposals submitted after this deadline will be deferred to the off-season review period.</p>
   
    <p>All proposed in-season changes must be brought forward by a league member and require a majority vote to be enacted.</p>

    <p>Note: Proposed rule changes may not target or reverse rules that were newly implemented in the most recent offseason.</p>

    <h3 bind:this={eightTwo}>8.2 off-Season League Changes</h3>

    <p>After each season, league members will vote on a list of proposed changes gathered throughout the year—beginning after the Week 6 in-season change deadline.</p>

    <p>Any rule change that receives a majority vote during this period will be adopted and applied for the following season.</p>

</div>
