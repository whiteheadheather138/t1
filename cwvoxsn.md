代发 wailian999

SELECT o.id, u.name, p.title FROM orders o
来源：http://3g.vehdjk.com/Article/details/gdvdvgrzp.sHtML

JOIN users u ON u.id = o.user_id
来源：http://read.share.fktsv.cn/Article/details/gkyllbxeh.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://read.share.epnwcf.com/Article/details/golrgjrmm.sHtML

[Q42] 连接条件附加过滤
来源：http://3g.fktsv.cn/Article/details/gnaeogeof.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.m.share.bbcook.cn/Article/details/gclhuokyv.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.blog.fktsv.cn/Article/details/gypxiodbr.sHtML

[Q43] 标量子查询
来源：http://baike.bbcook.cn/Article/details/gurjboaei.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://baike.vehdjk.com/Article/details/gahhtwwhs.sHtML

[Q44] IN 子查询
来源：http://read.share.tarul.cn/Article/details/gureyuony.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://wap.tarul.cn/Article/details/gevyugnyr.sHtML

[Q45] EXISTS 判断存在
来源：http://3g.bbcook.cn/Article/details/gmtcevxga.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.yfazqb.com/Article/details/gjsqyhloj.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://read.share.fktsv.cn/Article/details/gtilbrrlr.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.vehdjk.com/Article/details/gtjizdcyj.sHtML

[Q47] 与平均值比较
来源：http://baike.sjlbkw.cn/Article/details/genvpuvio.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://blog.epnwcf.com/Article/details/groafghkx.sHtML

[Q48] CTE 公用表表达式
来源：http://www.blog.vehdjk.com/Article/details/gnpyguagk.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://wap.sjlbkw.cn/Article/details/ggscqekcu.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://baike.epnwcf.com/Article/details/gnvmbihyv.sHtML

[Q49] 更新单行
来源：http://www.share.epnwcf.com/Article/details/gvwvnqvce.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://read.share.vehdjk.com/Article/details/goyarutys.sHtML

[Q50] 批量更新
来源：http://www.share.epnwcf.com/Article/details/gvyosdxsc.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://read.share.sjlbkw.cn/Article/details/gcjeuwubj.sHtML

[Q51] 用子查询更新
来源：http://3g.vehdjk.com/Article/details/gyvksquyb.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://mobile.sjlbkw.cn/Article/details/gupubfsic.sHtML

[Q52] 删除指定行
来源：http://m.share.bbcook.cn/Article/details/gaxwfawfd.sHtML

DELETE FROM users WHERE id = 10;
来源：http://m.share.sjlbkw.cn/Article/details/gewnlyhtf.sHtML

[Q53] 按条件删除
来源：http://blog.yfazqb.com/Article/details/gtcrnfbzl.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://3g.bbcook.cn/Article/details/gsdhcpgnc.sHtML

[Q54] 清空表
来源：http://read.share.yfazqb.com/Article/details/gxxcvbhmi.sHtML

TRUNCATE TABLE logs;
来源：http://read.share.tarul.cn/Article/details/gubaemrym.sHtML

[Q55] 排名（并列占位）
来源：http://read.share.epnwcf.com/Article/details/gghockpuo.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://baike.yfazqb.com/Article/details/gjiphfsqx.sHtML

[Q56] 密集排名（并列不占位）
来源：http://blog.epnwcf.com/Article/details/ghyqsoggy.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.m.share.sjlbkw.cn/Article/details/ghzqmtjzb.sHtML

[Q57] 行号
来源：http://mobile.epnwcf.com/Article/details/gtxhaczfa.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://m.share.sjlbkw.cn/Article/details/gegvbgndd.sHtML

[Q58] 累计求和
来源：http://read.share.epnwcf.com/Article/details/gbjfxshay.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://m.share.bbcook.cn/Article/details/gbsmyqmxd.sHtML

[Q59] 分组内累计
来源：http://www.share.fktsv.cn/Article/details/gotoqatxp.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://baike.tarul.cn/Article/details/gmnxljtru.sHtML

[Q60] 取上一行 / 下一行
来源：http://m.share.tarul.cn/Article/details/gnyxrcxbs.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://m.share.fktsv.cn/Article/details/gdivqhzjk.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.share.fktsv.cn/Article/details/gvflqfdgs.sHtML

[Q61] 移动平均
来源：http://blog.tarul.cn/Article/details/gsjwiuwyo.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.blog.epnwcf.com/Article/details/geijjzgai.sHtML

[Q62] 分组占比
来源：http://www.share.fktsv.cn/Article/details/guyhjsxoi.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://3g.sjlbkw.cn/Article/details/gwauzrrve.sHtML

[Q63] 开启事务
来源：http://blog.bbcook.cn/Article/details/gmaqtiylp.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://baike.tarul.cn/Article/details/gunhuwhyh.sHtML

[Q64] 提交事务
来源：http://m.share.sjlbkw.cn/Article/details/gtirlngov.sHtML

COMMIT;
来源：http://baike.bbcook.cn/Article/details/goijunfrm.sHtML

[Q65] 回滚事务
来源：http://m.share.bbcook.cn/Article/details/gjejthsfm.sHtML

ROLLBACK;
来源：http://mobile.epnwcf.com/Article/details/gkoyoxgtv.sHtML

[Q66] 行锁查询
来源：http://m.share.tarul.cn/Article/details/gsltesjvo.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://wap.vehdjk.com/Article/details/gktsowhjf.sHtML

[Q67] 设置隔离级别
来源：http://blog.yfazqb.com/Article/details/gbmeqfdgp.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.blog.yfazqb.com/Article/details/gckqauwlw.sHtML

[Q68] 保存点
来源：http://www.blog.bbcook.cn/Article/details/gtcumpztw.sHtML

SAVEPOINT sp1;
来源：http://read.share.tarul.cn/Article/details/gbugbqwmj.sHtML

ROLLBACK TO sp1;
来源：http://www.blog.tarul.cn/Article/details/ghlduoenj.sHtML

[Q69] 查看执行计划
来源：http://www.share.vehdjk.com/Article/details/ggnfqkzrb.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.share.sjlbkw.cn/Article/details/gjihhzyne.sHtML

[Q70] 更新统计信息
来源：http://blog.sjlbkw.cn/Article/details/gpuhcrdfe.sHtML

ANALYZE TABLE users;
来源：http://wap.yfazqb.com/Article/details/gsslotdxx.sHtML

[Q71] 查看建表语句
来源：http://www.m.share.epnwcf.com/Article/details/gggiccfxy.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://baike.vehdjk.com/Article/details/gppecenqf.sHtML

[Q72] 查看索引
来源：http://www.m.share.vehdjk.com/Article/details/gutlryyxb.sHtML

SHOW INDEX FROM users;
来源：http://blog.vehdjk.com/Article/details/gpuwqwilh.sHtML

[Q73] 查看表状态
来源：http://www.m.share.bbcook.cn/Article/details/glcrfadwm.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://baike.yfazqb.com/Article/details/gfjjxcmgp.sHtML

[Q74] 强制使用索引
来源：http://www.blog.epnwcf.com/Article/details/gjkmcodzo.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://mobile.yfazqb.com/Article/details/gplsffdmr.sHtML

[Q75] 日期格式化
来源：http://www.blog.fktsv.cn/Article/details/guaaazeyw.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://3g.bbcook.cn/Article/details/gisdfvzrt.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.share.sjlbkw.cn/Article/details/gegfxsikz.sHtML

[Q76] 按天统计
来源：http://www.blog.vehdjk.com/Article/details/gocaynjnr.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://read.share.epnwcf.com/Article/details/gdxeurzmd.sHtML

[Q77] 时间加减
来源：http://www.blog.bbcook.cn/Article/details/grugcnfxh.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://blog.fktsv.cn/Article/details/gdwdvoogj.sHtML

[Q78] 当前时间
来源：http://read.share.vehdjk.com/Article/details/ghxmiitjz.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.blog.bbcook.cn/Article/details/gorvbgcjh.sHtML

[Q79] 字符串拼接
来源：http://m.share.epnwcf.com/Article/details/gientcsqd.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.share.sjlbkw.cn/Article/details/gsqdnxhvi.sHtML

[Q80] 字符串截取
来源：http://mobile.bbcook.cn/Article/details/gahqbvtog.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://blog.vehdjk.com/Article/details/gpbladyey.sHtML

[Q81] 字符串替换
来源：http://www.m.share.epnwcf.com/Article/details/gasffjhsi.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://3g.tarul.cn/Article/details/gobbnncyo.sHtML

[Q82] 字符长度与字节长度
来源：http://www.share.vehdjk.com/Article/details/guyizsufh.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.blog.epnwcf.com/Article/details/gkizazrzh.sHtML

[Q83] 大小写转换
来源：http://baike.yfazqb.com/Article/details/ghccjubtr.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://3g.sjlbkw.cn/Article/details/gxkmumqoa.sHtML

[Q84] 去除首尾空格
来源：http://blog.tarul.cn/Article/details/gpygroqfa.sHtML

SELECT TRIM(name) FROM users;
来源：http://wap.epnwcf.com/Article/details/gsepfsnoz.sHtML

[Q85] 数值取整
来源：http://www.blog.epnwcf.com/Article/details/goykbghke.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://3g.tarul.cn/Article/details/gmzzsbbrb.sHtML

[Q86] 读取 JSON 字段
来源：http://baike.fktsv.cn/Article/details/gsukcnuxu.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://3g.tarul.cn/Article/details/ggcwzwkoh.sHtML

[Q87] JSON 字段做条件
来源：http://www.m.share.vehdjk.com/Article/details/gfxihhncc.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://3g.fktsv.cn/Article/details/ghdosdhlx.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.blog.sjlbkw.cn/Article/details/gmjnackzt.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://read.share.epnwcf.com/Article/details/gftmorlyi.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://blog.sjlbkw.cn/Article/details/gbpktlald.sHtML

[Q89] 判断表是否存在
来源：http://3g.bbcook.cn/Article/details/gwgxwyjyz.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://3g.tarul.cn/Article/details/gscolufrd.sHtML

[Q90] 生成序号列
来源：http://www.share.bbcook.cn/Article/details/gmhyhffbj.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.share.bbcook.cn/Article/details/gvdyiozfu.sHtML

================================================================================
来源：http://www.m.share.tarul.cn/Article/details/gucgmrnfn.sHtML

R. Bash 专题
来源：http://www.blog.vehdjk.com/Article/details/gkxrmlgtz.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/gaamykgvm.sHtML

[R01] shebang 与严格模式
来源：http://www.share.tarul.cn/Article/details/ghqprmatj.sHtML

#!/usr/bin/env bash
来源：http://3g.epnwcf.com/Article/details/gyxvofrzx.sHtML

set -euo pipefail
来源：http://mobile.sjlbkw.cn/Article/details/gjtzfnomd.sHtML

[R02] 变量赋值与使用
来源：http://www.m.share.bbcook.cn/Article/details/gltpnylaw.sHtML

name="Tom"; echo "$name"
来源：http://blog.fktsv.cn/Article/details/goqfickws.sHtML

[R03] 只读变量
来源：http://3g.sjlbkw.cn/Article/details/gmgtenrms.sHtML

readonly PI=3.14
来源：http://3g.fktsv.cn/Article/details/gacpydlzu.sHtML

[R04] 位置参数
来源：http://3g.epnwcf.com/Article/details/gjbkxepwd.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://read.share.bbcook.cn/Article/details/gjledbxen.sHtML

[R05] 参数默认值
来源：http://baike.bbcook.cn/Article/details/gxwxnpmsq.sHtML

name="${1:-default}"
来源：http://www.share.bbcook.cn/Article/details/gjbojzwxp.sHtML

[R06] 判断命令是否存在
来源：http://wap.tarul.cn/Article/details/gdvkscwrm.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://read.share.sjlbkw.cn/Article/details/gpimbdelo.sHtML

[R07] if 判断文件
来源：http://m.share.yfazqb.com/Article/details/gwnlttbck.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://wap.fktsv.cn/Article/details/gfursizpn.sHtML

[R08] 数值比较
来源：http://wap.sjlbkw.cn/Article/details/gqkkmxlof.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.blog.yfazqb.com/Article/details/gecposkxf.sHtML

[R09] 字符串比较
来源：http://read.share.fktsv.cn/Article/details/ggjntdycn.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://3g.epnwcf.com/Article/details/gciqvhmgg.sHtML

[R10] 正则匹配
来源：http://www.share.epnwcf.com/Article/details/guhuryovu.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.share.epnwcf.com/Article/details/gnzfduvgp.sHtML

[R11] case 多分支
来源：http://wap.sjlbkw.cn/Article/details/gbinsgnyf.sHtML

case "$1" in
来源：http://baike.tarul.cn/Article/details/gpnhfymnt.sHtML

start) echo "启动" ;;
来源：http://www.m.share.epnwcf.com/Article/details/ggiztlabz.sHtML

stop)  echo "停止" ;;
来源：http://www.m.share.fktsv.cn/Article/details/grzvavhdh.sHtML

*)     echo "未知命令" ;;
来源：http://read.share.sjlbkw.cn/Article/details/gojglzrvk.sHtML

esac
来源：http://wap.fktsv.cn/Article/details/gxsonoxkr.sHtML

[R12] for 遍历文件
来源：http://read.share.yfazqb.com/Article/details/gzqyeoixh.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.blog.sjlbkw.cn/Article/details/guieiobxk.sHtML

[R13] for 计数循环
来源：http://www.m.share.vehdjk.com/Article/details/gaafauxvj.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.blog.tarul.cn/Article/details/gctgmqufx.sHtML

[R14] C 风格 for
来源：http://baike.tarul.cn/Article/details/gjeyrgsnu.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://baike.yfazqb.com/Article/details/gilxnavuz.sHtML

[R15] while 逐行读文件
来源：http://m.share.sjlbkw.cn/Article/details/gxnjycxrk.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.share.bbcook.cn/Article/details/gapmglvmw.sHtML

[R16] until 等待条件
来源：http://3g.yfazqb.com/Article/details/geegfybnk.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.share.tarul.cn/Article/details/gdtpaqhhp.sHtML

[R17] 数组定义与取值
来源：http://wap.yfazqb.com/Article/details/gswivndat.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://blog.sjlbkw.cn/Article/details/gsgwwhvrz.sHtML

[R18] 遍历数组
来源：http://read.share.epnwcf.com/Article/details/ggowmqwqg.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://mobile.bbcook.cn/Article/details/gvnrlbfib.sHtML

[R19] 数组长度
来源：http://3g.tarul.cn/Article/details/gidmleyhw.sHtML

echo "${#arr[@]}"
来源：http://3g.bbcook.cn/Article/details/gtrmpisdc.sHtML

[R20] 关联数组（字典）
来源：http://mobile.vehdjk.com/Article/details/gijzeyqby.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.m.share.vehdjk.com/Article/details/gfjytjkui.sHtML

[R21] 字符串长度
来源：http://mobile.yfazqb.com/Article/details/gpatpkoys.sHtML

echo "${#s}"
来源：http://www.share.fktsv.cn/Article/details/gbxfxfgnc.sHtML

[R22] 截取子串
来源：http://www.m.share.vehdjk.com/Article/details/getncwxhq.sHtML

echo "${s:0:5}"
来源：http://www.share.tarul.cn/Article/details/gogrqnpgv.sHtML

[R23] 字符串替换
来源：http://read.share.epnwcf.com/Article/details/gpsgvpbno.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://blog.epnwcf.com/Article/details/gooiyumgd.sHtML

[R24] 大小写转换
来源：http://blog.fktsv.cn/Article/details/gudqkugqw.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.m.share.bbcook.cn/Article/details/gltkbrsml.sHtML

[R25] 去后缀 / 去前缀
来源：http://blog.vehdjk.com/Article/details/gsxozrzse.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.blog.epnwcf.com/Article/details/geasagslm.sHtML

[R26] 命令替换
来源：http://read.share.tarul.cn/Article/details/gfkljkxkg.sHtML

now=$(date +%F); echo "$now"
来源：http://wap.sjlbkw.cn/Article/details/gckwphesp.sHtML

[R27] 算术展开
来源：http://mobile.tarul.cn/Article/details/gasbrfwgp.sHtML

echo $((1 + 2 * 3))
来源：http://m.share.sjlbkw.cn/Article/details/gplnlvjqq.sHtML

[R28] 浮点运算
来源：http://read.share.yfazqb.com/Article/details/gjcwuwcpv.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.blog.sjlbkw.cn/Article/details/galmoeunw.sHtML

[R29] 定义函数
来源：http://wap.tarul.cn/Article/details/grhypvudt.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://wap.tarul.cn/Article/details/gndubdkau.sHtML

[R30] 函数返回状态码
来源：http://www.m.share.tarul.cn/Article/details/gnzutzpjh.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://3g.bbcook.cn/Article/details/gmhoebrlq.sHtML

[R31] 局部变量
来源：http://m.share.epnwcf.com/Article/details/gxuojiacw.sHtML

f() { local x=1; echo "$x"; }
来源：http://wap.tarul.cn/Article/details/gungkqfkt.sHtML

[R32] 参数个数校验
来源：http://www.blog.vehdjk.com/Article/details/gjekhkrzt.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://m.share.yfazqb.com/Article/details/gfantiygh.sHtML

[R33] 捕获错误并提示行号
来源：http://blog.sjlbkw.cn/Article/details/giqursarh.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://baike.sjlbkw.cn/Article/details/gsnypgdca.sHtML

[R34] 退出时清理
来源：http://m.share.yfazqb.com/Article/details/gadrpcokj.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.tarul.cn/Article/details/gbraanrma.sHtML

[R35] 后台执行并等待
来源：http://3g.epnwcf.com/Article/details/gmmuasgfs.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://read.share.epnwcf.com/Article/details/gfaxwpgue.sHtML

[R36] 并发执行多个任务
来源：http://wap.fktsv.cn/Article/details/gywwfcoon.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://read.share.sjlbkw.cn/Article/details/gwyybgshg.sHtML

[R37] 把输出赋给变量
来源：http://baike.yfazqb.com/Article/details/gjvyrvari.sHtML

files=$(ls -1)
来源：http://wap.epnwcf.com/Article/details/gtjatrzfb.sHtML

[R38] 管道串联
来源：http://blog.vehdjk.com/Article/details/gyoyhvoos.sHtML

cat a.txt | grep -i error | wc -l
来源：http://mobile.fktsv.cn/Article/details/gxhakdevl.sHtML

[R39] 重定向标准输出与错误
来源：http://blog.tarul.cn/Article/details/gnzurwmom.sHtML

cmd > out.log 2>&1
来源：http://www.m.share.epnwcf.com/Article/details/goosxoofx.sHtML

[R40] 追加写日志
来源：http://baike.fktsv.cn/Article/details/gmxfexmyu.sHtML

echo "log" >> out.log
来源：http://mobile.sjlbkw.cn/Article/details/gsyixdqxv.sHtML

[R41] 丢弃输出
来源：http://blog.vehdjk.com/Article/details/gyhjajcds.sHtML

cmd >/dev/null 2>&1
来源：http://wap.yfazqb.com/Article/details/gbhzyspuh.sHtML

[R42] 输入重定向
来源：http://m.share.epnwcf.com/Article/details/gffjmbdtm.sHtML

wc -l < a.txt
来源：http://m.share.vehdjk.com/Article/details/gglxcwcce.sHtML

[R43] 按名字查找文件
来源：http://wap.vehdjk.com/Article/details/gmsqkkrxn.sHtML

find . -name "*.log" -type f
来源：http://blog.yfazqb.com/Article/details/gnlwiswkd.sHtML

[R44] 按修改时间查找
来源：http://baike.vehdjk.com/Article/details/ghfaxsmur.sHtML

find . -mtime -7 -type f
来源：http://www.m.share.bbcook.cn/Article/details/ghlyenkot.sHtML

[R45] 批量删除
来源：http://3g.bbcook.cn/Article/details/gxxzjawrd.sHtML

find . -name "*.tmp" -delete
来源：http://m.share.yfazqb.com/Article/details/gdxssclei.sHtML

[R46] 递归替换文件内容
来源：http://3g.sjlbkw.cn/Article/details/gxgeylmar.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://baike.vehdjk.com/Article/details/gbyldjmuw.sHtML

[R47] sed 单行替换
来源：http://baike.tarul.cn/Article/details/gzqemhyej.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.share.epnwcf.com/Article/details/gioqkeodj.sHtML

[R48] awk 取指定列
来源：http://www.blog.vehdjk.com/Article/details/gphynxtqv.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.share.yfazqb.com/Article/details/gwqkheaih.sHtML

[R49] awk 带条件
来源：http://www.share.epnwcf.com/Article/details/gsffbmbsg.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://m.share.vehdjk.com/Article/details/gyohphhrw.sHtML

[R50] awk 求和
来源：http://read.share.fktsv.cn/Article/details/gcwnyrzoe.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://blog.vehdjk.com/Article/details/gfgxzohoz.sHtML

[R51] 排序去重取前几
来源：http://read.share.tarul.cn/Article/details/ggetdsmkl.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://3g.sjlbkw.cn/Article/details/gwjohgvto.sHtML

[R52] 统计行数
来源：http://3g.tarul.cn/Article/details/gqyclzboa.sHtML

wc -l a.txt
来源：http://3g.fktsv.cn/Article/details/gxilqbgqx.sHtML

[R53] 查看文件头与实时尾
来源：http://www.share.yfazqb.com/Article/details/guhyojteb.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://blog.epnwcf.com/Article/details/gfrzbygnv.sHtML

[R54] 比较两个文件
来源：http://www.share.yfazqb.com/Article/details/gbavgsqyb.sHtML

diff a.txt b.txt
来源：http://wap.tarul.cn/Article/details/gomiypoeo.sHtML

[R55] 压缩与解压
来源：http://www.m.share.yfazqb.com/Article/details/gucbbooid.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://baike.tarul.cn/Article/details/gpeesisiz.sHtML

[R56] 远程拷贝
来源：http://blog.tarul.cn/Article/details/godbcyfsu.sHtML

scp file user@host:/path/
来源：http://www.share.tarul.cn/Article/details/gosyuwbwp.sHtML

[R57] 远程执行命令
来源：http://blog.yfazqb.com/Article/details/gozddzupd.sHtML

ssh user@host 'uptime'
来源：http://www.blog.tarul.cn/Article/details/giblklbgm.sHtML

[R58] 下载文件
来源：http://blog.bbcook.cn/Article/details/gvsymnrkp.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://3g.yfazqb.com/Article/details/gabnckivy.sHtML

[R59] 发 POST JSON
来源：http://mobile.vehdjk.com/Article/details/gbxhddzug.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://blog.fktsv.cn/Article/details/gcoaftpiw.sHtML

[R60] 只看 HTTP 状态码
来源：http://m.share.sjlbkw.cn/Article/details/gtxvfekoa.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.m.share.bbcook.cn/Article/details/gowavbjre.sHtML

[R61] 磁盘占用
来源：http://wap.epnwcf.com/Article/details/ghvxelapx.sHtML

df -h;  du -sh *
来源：http://www.blog.epnwcf.com/Article/details/gwpqrtpbk.sHtML

[R62] 找最占空间的文件
来源：http://mobile.bbcook.cn/Article/details/gkstlfrox.sHtML

du -ah . | sort -rh | head -10
来源：http://www.blog.epnwcf.com/Article/details/gbadwobkz.sHtML

[R63] 内存与进程
来源：http://wap.tarul.cn/Article/details/ggvamzpxd.sHtML

free -h;  ps aux | grep nginx
来源：http://m.share.tarul.cn/Article/details/gymedgykc.sHtML

[R64] 结束进程
来源：http://m.share.epnwcf.com/Article/details/gnidtnyao.sHtML

kill -9 $(pgrep -f app.py)
来源：http://mobile.bbcook.cn/Article/details/gxbeorfem.sHtML

[R65] 查看端口占用
来源：http://www.share.epnwcf.com/Article/details/gmsmiewaq.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://blog.sjlbkw.cn/Article/details/ghmnykccb.sHtML

[R66] 定时任务
来源：http://blog.tarul.cn/Article/details/gmfncjlid.sHtML

crontab -e;  crontab -l
来源：http://mobile.tarul.cn/Article/details/gpjigpwkp.sHtML

[R67] 生成随机十六进制串
来源：http://3g.fktsv.cn/Article/details/gycjgzbtz.sHtML

openssl rand -hex 16
来源：http://m.share.sjlbkw.cn/Article/details/gllsjcdzd.sHtML

[R68] 计算文件校验值
来源：http://m.share.tarul.cn/Article/details/gtykgwbvx.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://baike.tarul.cn/Article/details/gatapkrlb.sHtML

[R69] 生成随机密码
来源：http://blog.vehdjk.com/Article/details/gcssvhvgw.sHtML

head -c 16 /dev/urandom | base64
来源：http://read.share.sjlbkw.cn/Article/details/gkoqjsrmo.sHtML

[R70] 时间戳与互转
来源：http://wap.vehdjk.com/Article/details/gfkakmluk.sHtML

date +%s;  date -d @1700000000
来源：http://read.share.epnwcf.com/Article/details/guapkroqr.sHtML

[R71] 日期格式化
来源：http://www.m.share.epnwcf.com/Article/details/gfnriwivy.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://read.share.vehdjk.com/Article/details/gepuxujuj.sHtML

[R72] 等待端口就绪
来源：http://read.share.yfazqb.com/Article/details/giaicifjr.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://3g.vehdjk.com/Article/details/gacsdmbcf.sHtML

[R73] 分割大日志
来源：http://www.blog.yfazqb.com/Article/details/gbrlsifzu.sHtML

split -l 1000 big.log part_
来源：http://baike.bbcook.cn/Article/details/gtghviius.sHtML

[R74] 批量重命名
来源：http://baike.fktsv.cn/Article/details/gkcmvvhpg.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://3g.sjlbkw.cn/Article/details/ggtyhbctw.sHtML

[R75] 导出环境变量
来源：http://3g.bbcook.cn/Article/details/glwhsoqei.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://wap.fktsv.cn/Article/details/gvhbybqty.sHtML

[R76] 使用临时文件
来源：http://wap.epnwcf.com/Article/details/galfufvhl.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://wap.tarul.cn/Article/details/gnssiqqdo.sHtML

[R77] 读取用户输入
来源：http://www.m.share.tarul.cn/Article/details/ghlmolluw.sHtML

read -rp "请输入: " ans
来源：http://blog.vehdjk.com/Article/details/gpgdrluqw.sHtML

[R78] 交互式菜单
来源：http://blog.sjlbkw.cn/Article/details/ghkqkibvd.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://m.share.epnwcf.com/Article/details/gvgvdkluc.sHtML

[R79] 解析命令行选项
来源：http://wap.bbcook.cn/Article/details/gnlsxybyf.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://blog.fktsv.cn/Article/details/gviskyejv.sHtML

[R80] 查看脚本执行耗时
来源：http://www.share.yfazqb.com/Article/details/gjmmtskiq.sHtML

time ./run.sh
来源：http://mobile.sjlbkw.cn/Article/details/gltzxpmbe.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/gkkeqbaaf.sHtML

S. C / C++ 专题
来源：http://blog.yfazqb.com/Article/details/gwivxcoze.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/gkylzxurk.sHtML

[S01] C：Hello World
来源：http://baike.sjlbkw.cn/Article/details/gshqyffll.sHtML

#include <stdio.h>
来源：http://m.share.tarul.cn/Article/details/gdciulvca.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.share.epnwcf.com/Article/details/gwfiriacn.sHtML

[S02] C：变量与格式化输出
来源：http://wap.bbcook.cn/Article/details/gijkrfzzy.sHtML

int a = 10; printf("%d\n", a);
来源：http://read.share.bbcook.cn/Article/details/gnzbhfdgb.sHtML

[S03] C：读入整数
来源：http://blog.bbcook.cn/Article/details/gkhelatdl.sHtML

int x; scanf("%d", &x);
来源：http://mobile.fktsv.cn/Article/details/gdxxnbecy.sHtML

[S04] C：字符串复制
来源：http://www.blog.sjlbkw.cn/Article/details/gwqprkzfg.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://wap.yfazqb.com/Article/details/gmvvsfxvd.sHtML

[S05] C：字符串长度
来源：http://www.blog.yfazqb.com/Article/details/gydtcoxdy.sHtML

strlen(s)
来源：http://blog.sjlbkw.cn/Article/details/gavthfllr.sHtML

[S06] C：字符串比较
来源：http://baike.epnwcf.com/Article/details/gnyraxzze.sHtML

strcmp(a, b) == 0
来源：http://www.m.share.tarul.cn/Article/details/gddndrlav.sHtML

[S07] C：数组遍历求和
来源：http://read.share.tarul.cn/Article/details/gnlgjeeyy.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://blog.epnwcf.com/Article/details/guregdfzb.sHtML

[S08] C：动态内存分配与释放
来源：http://read.share.fktsv.cn/Article/details/gibvdpbex.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://3g.yfazqb.com/Article/details/glsfxxxzo.sHtML

[S09] C：结构体定义与初始化
来源：http://wap.tarul.cn/Article/details/guzpjwahy.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.m.share.vehdjk.com/Article/details/giwknydsk.sHtML

[S10] C：指针与解引用
来源：http://wap.vehdjk.com/Article/details/gsxcelkmf.sHtML

int *p = &a;  *p = 5;
来源：http://www.share.bbcook.cn/Article/details/gqsguirvi.sHtML

[S11] C：逐行读文件
来源：http://www.blog.tarul.cn/Article/details/gsqrwbhjf.sHtML


<!-- 参考信息 -->