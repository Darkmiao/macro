## 审判宏 ##
智慧审判宏，会按照智慧+审判的顺序出招，抽筋狂按不会给自己狂刷buff。
* 英文端
    /script for i=1,16 do if(UnitBuff("player",i)) then if(string.find(UnitBuff("player",i),"RighteousnessAura")) then CastSpellByName("Judgement");break;end;else CastSpellByName("Seal of Wisdom()");break;end;end
* 中文端
    待测试

其他审判：
InnerRage--Command(命令)
HealingAura—Light(光明)
RighteousnessAura—wisdom(智慧)
HolySmite—Crusader(十字军)

## 战场旗手宏 ##
由于骑士无法通过连续点击取消无敌，固有此宏，用于战场出旗。用1级无敌省蓝。
* 英文端
    /cast Divine Shield(Rank 1)
    /script local i for i = 0,15 do if ( GetPlayerBuffTexture(i) == "Interface\\Icons\\Spell_Holy_DivineIntervention") then CancelPlayerBuff(i);end;end
* 中文端
    待测试