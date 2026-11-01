代发 wailian999

[Q38] 全外连接（PostgreSQL）
来源：http://www.blog.bbcook.cn/Article/details/gunjrvhpw.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://blog.tarul.cn/Article/details/gcsksbuic.sHtML

[Q39] 自连接（查上下级）
来源：http://read.share.yfazqb.com/Article/details/gqsieckaz.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.share.yfazqb.com/Article/details/ghlzrhuoh.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.blog.sjlbkw.cn/Article/details/gbmqpwzvk.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://baike.fktsv.cn/Article/details/ggxwdeeup.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.share.bbcook.cn/Article/details/grjkhtbya.sHtML

[Q41] 多表连接
来源：http://read.share.bbcook.cn/Article/details/gcumlmeqx.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://3g.yfazqb.com/Article/details/gzxxokmth.sHtML

JOIN users u ON u.id = o.user_id
来源：http://3g.vehdjk.com/Article/details/gtssupieg.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.share.tarul.cn/Article/details/gyubiudee.sHtML

[Q42] 连接条件附加过滤
来源：http://blog.fktsv.cn/Article/details/gkuxkmpey.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.share.fktsv.cn/Article/details/gyghizfdu.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.blog.epnwcf.com/Article/details/gyjaqlfzn.sHtML

[Q43] 标量子查询
来源：http://www.share.epnwcf.com/Article/details/gdnfhavse.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://m.share.epnwcf.com/Article/details/gbapscqve.sHtML

[Q44] IN 子查询
来源：http://wap.epnwcf.com/Article/details/gnbrgsymh.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.share.tarul.cn/Article/details/gbpttixwm.sHtML

[Q45] EXISTS 判断存在
来源：http://read.share.epnwcf.com/Article/details/gzcemmuxc.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.tarul.cn/Article/details/gkqjfwxeg.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://baike.vehdjk.com/Article/details/gcnrbgdak.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.tarul.cn/Article/details/gmpcueqss.sHtML

[Q47] 与平均值比较
来源：http://read.share.vehdjk.com/Article/details/gtnsldcmr.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://3g.bbcook.cn/Article/details/gduykgxan.sHtML

[Q48] CTE 公用表表达式
来源：http://www.share.tarul.cn/Article/details/gsqtfabyj.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://3g.tarul.cn/Article/details/gkfnyzdoe.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.m.share.yfazqb.com/Article/details/gjqogifvz.sHtML

[Q49] 更新单行
来源：http://www.share.fktsv.cn/Article/details/gtmqwgdmc.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.blog.sjlbkw.cn/Article/details/gdgwfzuum.sHtML

[Q50] 批量更新
来源：http://mobile.vehdjk.com/Article/details/gsdtyfinz.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://mobile.epnwcf.com/Article/details/gyqvbssdt.sHtML

[Q51] 用子查询更新
来源：http://www.blog.bbcook.cn/Article/details/gfkiwcish.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://3g.fktsv.cn/Article/details/gfdlzfdhh.sHtML

[Q52] 删除指定行
来源：http://blog.sjlbkw.cn/Article/details/gtvfeqjfc.sHtML

DELETE FROM users WHERE id = 10;
来源：http://m.share.vehdjk.com/Article/details/gtrzwbadr.sHtML

[Q53] 按条件删除
来源：http://www.blog.sjlbkw.cn/Article/details/gobefgyfb.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://read.share.yfazqb.com/Article/details/gakihxpsa.sHtML

[Q54] 清空表
来源：http://read.share.tarul.cn/Article/details/gcjmdmhjr.sHtML

TRUNCATE TABLE logs;
来源：http://www.m.share.sjlbkw.cn/Article/details/gdkhsmlme.sHtML

[Q55] 排名（并列占位）
来源：http://m.share.sjlbkw.cn/Article/details/grelomdaw.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://wap.epnwcf.com/Article/details/gphhcoivo.sHtML

[Q56] 密集排名（并列不占位）
来源：http://blog.tarul.cn/Article/details/gwpefopcy.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://mobile.yfazqb.com/Article/details/georojshn.sHtML

[Q57] 行号
来源：http://baike.sjlbkw.cn/Article/details/gyxsgxfrk.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://wap.fktsv.cn/Article/details/gpxydywgj.sHtML

[Q58] 累计求和
来源：http://www.m.share.sjlbkw.cn/Article/details/gihurgvlc.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.blog.vehdjk.com/Article/details/gofqymjfd.sHtML

[Q59] 分组内累计
来源：http://wap.vehdjk.com/Article/details/gkpocmixg.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://blog.epnwcf.com/Article/details/grqebmiix.sHtML

[Q60] 取上一行 / 下一行
来源：http://read.share.tarul.cn/Article/details/gmcxkinpf.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://m.share.vehdjk.com/Article/details/gejpisoej.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://m.share.bbcook.cn/Article/details/gnvljpnfq.sHtML

[Q61] 移动平均
来源：http://www.share.tarul.cn/Article/details/ggpehuddz.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://baike.fktsv.cn/Article/details/gdtnacerx.sHtML

[Q62] 分组占比
来源：http://read.share.bbcook.cn/Article/details/gxcmfxzjf.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://3g.bbcook.cn/Article/details/gxfvzirkj.sHtML

[Q63] 开启事务
来源：http://3g.yfazqb.com/Article/details/gcxeunnfd.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://wap.yfazqb.com/Article/details/glurqfaiw.sHtML

[Q64] 提交事务
来源：http://mobile.tarul.cn/Article/details/gdhpckdcy.sHtML

COMMIT;
来源：http://mobile.fktsv.cn/Article/details/gkaukekpn.sHtML

[Q65] 回滚事务
来源：http://wap.sjlbkw.cn/Article/details/gatlyqfoc.sHtML

ROLLBACK;
来源：http://wap.tarul.cn/Article/details/glxahtlma.sHtML

[Q66] 行锁查询
来源：http://m.share.bbcook.cn/Article/details/gekolpafq.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.blog.vehdjk.com/Article/details/gzlmwqbcv.sHtML

[Q67] 设置隔离级别
来源：http://www.m.share.epnwcf.com/Article/details/gcxzkspch.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://read.share.vehdjk.com/Article/details/glfxlypyo.sHtML

[Q68] 保存点
来源：http://www.m.share.fktsv.cn/Article/details/gnmnitnkm.sHtML

SAVEPOINT sp1;
来源：http://www.blog.tarul.cn/Article/details/gaowmncvg.sHtML

ROLLBACK TO sp1;
来源：http://www.share.tarul.cn/Article/details/gmcrsrhot.sHtML

[Q69] 查看执行计划
来源：http://blog.epnwcf.com/Article/details/gthzpngcy.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://mobile.bbcook.cn/Article/details/giiutjokh.sHtML

[Q70] 更新统计信息
来源：http://m.share.sjlbkw.cn/Article/details/gkqywodmp.sHtML

ANALYZE TABLE users;
来源：http://wap.epnwcf.com/Article/details/ggcpjygjf.sHtML

[Q71] 查看建表语句
来源：http://3g.vehdjk.com/Article/details/gzdktbhve.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.share.tarul.cn/Article/details/ggixflqmj.sHtML

[Q72] 查看索引
来源：http://mobile.epnwcf.com/Article/details/gdkshahnk.sHtML

SHOW INDEX FROM users;
来源：http://read.share.yfazqb.com/Article/details/gqxwfvyuv.sHtML

[Q73] 查看表状态
来源：http://baike.fktsv.cn/Article/details/gzybpppzf.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.m.share.sjlbkw.cn/Article/details/gicjlwqeh.sHtML

[Q74] 强制使用索引
来源：http://www.share.sjlbkw.cn/Article/details/gkisgjebk.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.blog.fktsv.cn/Article/details/gdyqlsewx.sHtML

[Q75] 日期格式化
来源：http://mobile.vehdjk.com/Article/details/gkksbkuuf.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://baike.tarul.cn/Article/details/gzwgdeqtx.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://mobile.tarul.cn/Article/details/geolnygiu.sHtML

[Q76] 按天统计
来源：http://mobile.fktsv.cn/Article/details/gzttpwmph.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://blog.sjlbkw.cn/Article/details/gzsevnbri.sHtML

[Q77] 时间加减
来源：http://www.blog.bbcook.cn/Article/details/ghotuhmtx.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://mobile.tarul.cn/Article/details/gkuwiaezo.sHtML

[Q78] 当前时间
来源：http://baike.sjlbkw.cn/Article/details/grjjkdblm.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://read.share.tarul.cn/Article/details/gtezxdrlj.sHtML

[Q79] 字符串拼接
来源：http://m.share.yfazqb.com/Article/details/gzkdgtimv.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://3g.yfazqb.com/Article/details/gjwliwoyw.sHtML

[Q80] 字符串截取
来源：http://www.blog.sjlbkw.cn/Article/details/glfcuxzpl.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://m.share.bbcook.cn/Article/details/gkaagvwjq.sHtML

[Q81] 字符串替换
来源：http://wap.vehdjk.com/Article/details/gbhhjtoba.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://mobile.epnwcf.com/Article/details/ggbdvbhmq.sHtML

[Q82] 字符长度与字节长度
来源：http://read.share.epnwcf.com/Article/details/grqkikycl.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://wap.yfazqb.com/Article/details/gsnsoylbx.sHtML

[Q83] 大小写转换
来源：http://read.share.bbcook.cn/Article/details/gyzitftex.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.m.share.tarul.cn/Article/details/gveuymmef.sHtML

[Q84] 去除首尾空格
来源：http://read.share.fktsv.cn/Article/details/gjojvczzg.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.m.share.tarul.cn/Article/details/gussfdbrz.sHtML

[Q85] 数值取整
来源：http://blog.yfazqb.com/Article/details/graettgmp.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://mobile.fktsv.cn/Article/details/gddhkhbil.sHtML

[Q86] 读取 JSON 字段
来源：http://www.share.epnwcf.com/Article/details/gksdvhtmg.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.m.share.fktsv.cn/Article/details/gmmkgqyrx.sHtML

[Q87] JSON 字段做条件
来源：http://baike.bbcook.cn/Article/details/gyamatanv.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.m.share.bbcook.cn/Article/details/gyzpkuguf.sHtML

[Q88] 行转列（条件聚合）
来源：http://wap.bbcook.cn/Article/details/gjkwmweaq.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.m.share.yfazqb.com/Article/details/gdtikvtkj.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.m.share.epnwcf.com/Article/details/gddupazee.sHtML

[Q89] 判断表是否存在
来源：http://www.blog.epnwcf.com/Article/details/gyowjtevp.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://blog.vehdjk.com/Article/details/glypshxzq.sHtML

[Q90] 生成序号列
来源：http://www.blog.yfazqb.com/Article/details/gytzblezt.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://read.share.epnwcf.com/Article/details/gpkbhmfbj.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/gmzgxrlzd.sHtML

R. Bash 专题
来源：http://www.m.share.fktsv.cn/Article/details/gypbvgaeh.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/gocyargkk.sHtML

[R01] shebang 与严格模式
来源：http://m.share.vehdjk.com/Article/details/glofbrflk.sHtML

#!/usr/bin/env bash
来源：http://baike.fktsv.cn/Article/details/gtzcyzdmr.sHtML

set -euo pipefail
来源：http://www.m.share.vehdjk.com/Article/details/gydjdjwok.sHtML

[R02] 变量赋值与使用
来源：http://baike.tarul.cn/Article/details/ghkhhfjjv.sHtML

name="Tom"; echo "$name"
来源：http://3g.fktsv.cn/Article/details/gbgjwurty.sHtML

[R03] 只读变量
来源：http://www.share.bbcook.cn/Article/details/gktqxzbmt.sHtML

readonly PI=3.14
来源：http://3g.vehdjk.com/Article/details/gxpigkpgw.sHtML

[R04] 位置参数
来源：http://www.share.tarul.cn/Article/details/gwnvynfvv.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.share.bbcook.cn/Article/details/gpqlpjzpg.sHtML

[R05] 参数默认值
来源：http://3g.yfazqb.com/Article/details/gpzjahiid.sHtML

name="${1:-default}"
来源：http://www.share.sjlbkw.cn/Article/details/grhlcktnx.sHtML

[R06] 判断命令是否存在
来源：http://3g.tarul.cn/Article/details/gtomvwbkc.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://mobile.yfazqb.com/Article/details/gzsjoidfb.sHtML

[R07] if 判断文件
来源：http://baike.bbcook.cn/Article/details/ggofuvjga.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://wap.tarul.cn/Article/details/gvizxdqkn.sHtML

[R08] 数值比较
来源：http://wap.bbcook.cn/Article/details/gcubgcmdl.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.share.sjlbkw.cn/Article/details/garkhygqn.sHtML

[R09] 字符串比较
来源：http://baike.bbcook.cn/Article/details/gvtnytwgv.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://read.share.fktsv.cn/Article/details/gkmexldhq.sHtML

[R10] 正则匹配
来源：http://www.blog.epnwcf.com/Article/details/gdpcutepw.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://baike.vehdjk.com/Article/details/gkcxwzkjn.sHtML

[R11] case 多分支
来源：http://read.share.vehdjk.com/Article/details/gmblqhtcw.sHtML

case "$1" in
来源：http://blog.vehdjk.com/Article/details/gqrxujtwr.sHtML

start) echo "启动" ;;
来源：http://wap.vehdjk.com/Article/details/gzkicxcke.sHtML

stop)  echo "停止" ;;
来源：http://3g.sjlbkw.cn/Article/details/gllgekmbb.sHtML

*)     echo "未知命令" ;;
来源：http://mobile.epnwcf.com/Article/details/ggadqfkax.sHtML

esac
来源：http://3g.yfazqb.com/Article/details/gzagbupzo.sHtML

[R12] for 遍历文件
来源：http://blog.tarul.cn/Article/details/gglcdsnlu.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.share.tarul.cn/Article/details/gcpduibpw.sHtML

[R13] for 计数循环
来源：http://m.share.fktsv.cn/Article/details/gnnbfxqbl.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://read.share.tarul.cn/Article/details/gmuzumrnm.sHtML

[R14] C 风格 for
来源：http://baike.bbcook.cn/Article/details/gqcwjkrkr.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://blog.vehdjk.com/Article/details/gbndgvxen.sHtML

[R15] while 逐行读文件
来源：http://baike.vehdjk.com/Article/details/gggyhdhrr.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.m.share.fktsv.cn/Article/details/gyxuyjlfv.sHtML

[R16] until 等待条件
来源：http://wap.fktsv.cn/Article/details/ghdufdxxh.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://blog.epnwcf.com/Article/details/gmhuiutxg.sHtML

[R17] 数组定义与取值
来源：http://3g.vehdjk.com/Article/details/gfxykewvx.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://blog.yfazqb.com/Article/details/gvtidyptd.sHtML

[R18] 遍历数组
来源：http://baike.tarul.cn/Article/details/gckgitgrb.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://3g.fktsv.cn/Article/details/gucfzzgml.sHtML

[R19] 数组长度
来源：http://baike.fktsv.cn/Article/details/gyfgatjhy.sHtML

echo "${#arr[@]}"
来源：http://wap.epnwcf.com/Article/details/gapbwltbg.sHtML

[R20] 关联数组（字典）
来源：http://mobile.bbcook.cn/Article/details/gwfwgqqtp.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://m.share.bbcook.cn/Article/details/guwxhynqx.sHtML

[R21] 字符串长度
来源：http://m.share.epnwcf.com/Article/details/gcknvhepr.sHtML

echo "${#s}"
来源：http://blog.epnwcf.com/Article/details/gzdvygijz.sHtML

[R22] 截取子串
来源：http://baike.vehdjk.com/Article/details/gminsdakz.sHtML

echo "${s:0:5}"
来源：http://blog.tarul.cn/Article/details/gufhhnjbu.sHtML

[R23] 字符串替换
来源：http://baike.sjlbkw.cn/Article/details/gcgjxfaou.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://mobile.fktsv.cn/Article/details/gqohehbme.sHtML

[R24] 大小写转换
来源：http://www.share.bbcook.cn/Article/details/gaomngmqo.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://read.share.fktsv.cn/Article/details/gqnvudwbg.sHtML

[R25] 去后缀 / 去前缀
来源：http://3g.vehdjk.com/Article/details/gsdcpcwlo.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://m.share.fktsv.cn/Article/details/gwcskkioz.sHtML

[R26] 命令替换
来源：http://www.share.vehdjk.com/Article/details/gqquvctwb.sHtML

now=$(date +%F); echo "$now"
来源：http://www.blog.tarul.cn/Article/details/guspekbpn.sHtML

[R27] 算术展开
来源：http://wap.sjlbkw.cn/Article/details/gigapvzqn.sHtML

echo $((1 + 2 * 3))
来源：http://read.share.bbcook.cn/Article/details/gukjnadpn.sHtML

[R28] 浮点运算
来源：http://www.m.share.fktsv.cn/Article/details/gtavjoidk.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.blog.sjlbkw.cn/Article/details/guumbulot.sHtML

[R29] 定义函数
来源：http://baike.tarul.cn/Article/details/gbktfygxg.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://baike.vehdjk.com/Article/details/gcbnhsube.sHtML

[R30] 函数返回状态码
来源：http://www.m.share.sjlbkw.cn/Article/details/gqjhejfzj.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.blog.sjlbkw.cn/Article/details/gvuvfgdjo.sHtML

[R31] 局部变量
来源：http://mobile.yfazqb.com/Article/details/gwhhdlkzt.sHtML

f() { local x=1; echo "$x"; }
来源：http://wap.sjlbkw.cn/Article/details/gfozhtbel.sHtML

[R32] 参数个数校验
来源：http://blog.fktsv.cn/Article/details/gxnmrypfh.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://mobile.sjlbkw.cn/Article/details/gspkxhhzv.sHtML

[R33] 捕获错误并提示行号
来源：http://www.m.share.bbcook.cn/Article/details/grnqinrtu.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.share.yfazqb.com/Article/details/gfyonsupj.sHtML

[R34] 退出时清理
来源：http://www.m.share.fktsv.cn/Article/details/gnohpowol.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.yfazqb.com/Article/details/gkjrpnoma.sHtML

[R35] 后台执行并等待
来源：http://wap.fktsv.cn/Article/details/gtwjncysw.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://3g.fktsv.cn/Article/details/gomrzekww.sHtML

[R36] 并发执行多个任务
来源：http://mobile.yfazqb.com/Article/details/gxfqwfcrm.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.share.tarul.cn/Article/details/guvbiidmm.sHtML

[R37] 把输出赋给变量
来源：http://www.blog.yfazqb.com/Article/details/gzzifajkg.sHtML

files=$(ls -1)
来源：http://www.blog.tarul.cn/Article/details/gyhbjnsfh.sHtML

[R38] 管道串联
来源：http://www.m.share.fktsv.cn/Article/details/gmogikiis.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.share.yfazqb.com/Article/details/ghtczjrqu.sHtML

[R39] 重定向标准输出与错误
来源：http://blog.tarul.cn/Article/details/gvkstnlzf.sHtML

cmd > out.log 2>&1
来源：http://3g.vehdjk.com/Article/details/ggcehqitj.sHtML

[R40] 追加写日志
来源：http://mobile.tarul.cn/Article/details/gxqeutapn.sHtML

echo "log" >> out.log
来源：http://read.share.fktsv.cn/Article/details/gpfppvcwj.sHtML

[R41] 丢弃输出
来源：http://www.blog.sjlbkw.cn/Article/details/grtvvxzlq.sHtML

cmd >/dev/null 2>&1
来源：http://baike.vehdjk.com/Article/details/gdalrubsh.sHtML

[R42] 输入重定向
来源：http://www.blog.bbcook.cn/Article/details/ghqbzcmje.sHtML

wc -l < a.txt
来源：http://www.blog.bbcook.cn/Article/details/gjiceanur.sHtML

[R43] 按名字查找文件
来源：http://m.share.tarul.cn/Article/details/givakmrvj.sHtML

find . -name "*.log" -type f
来源：http://read.share.epnwcf.com/Article/details/gyjvscydz.sHtML

[R44] 按修改时间查找
来源：http://www.share.fktsv.cn/Article/details/gelffxhhg.sHtML

find . -mtime -7 -type f
来源：http://baike.vehdjk.com/Article/details/gtjrncvks.sHtML

[R45] 批量删除
来源：http://3g.sjlbkw.cn/Article/details/gqoahebgh.sHtML

find . -name "*.tmp" -delete
来源：http://www.m.share.fktsv.cn/Article/details/gfxgbjpjv.sHtML

[R46] 递归替换文件内容
来源：http://blog.fktsv.cn/Article/details/gxrdfyhvh.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://read.share.fktsv.cn/Article/details/gtrplbflq.sHtML

[R47] sed 单行替换
来源：http://read.share.fktsv.cn/Article/details/gntjaggni.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://baike.vehdjk.com/Article/details/gjzchjrfs.sHtML

[R48] awk 取指定列
来源：http://www.m.share.vehdjk.com/Article/details/gjiyytzoa.sHtML

awk '{print $1, $3}' a.txt
来源：http://3g.tarul.cn/Article/details/grmigkvml.sHtML

[R49] awk 带条件
来源：http://www.blog.tarul.cn/Article/details/gzaugasso.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wap.yfazqb.com/Article/details/gubtiymfz.sHtML

[R50] awk 求和
来源：http://blog.vehdjk.com/Article/details/gupqctdtw.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://wap.epnwcf.com/Article/details/gcrfppmuy.sHtML

[R51] 排序去重取前几
来源：http://3g.bbcook.cn/Article/details/gywdqmahs.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.m.share.vehdjk.com/Article/details/gbjsldwsk.sHtML

[R52] 统计行数
来源：http://blog.epnwcf.com/Article/details/gwdcqbcoz.sHtML

wc -l a.txt
来源：http://www.blog.epnwcf.com/Article/details/gsnmyywgt.sHtML

[R53] 查看文件头与实时尾
来源：http://blog.tarul.cn/Article/details/gtjfjrltj.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.m.share.tarul.cn/Article/details/grhugpwqy.sHtML

[R54] 比较两个文件
来源：http://3g.bbcook.cn/Article/details/gnnqyzqqa.sHtML

diff a.txt b.txt
来源：http://wap.sjlbkw.cn/Article/details/gnyjqxdiz.sHtML

[R55] 压缩与解压
来源：http://read.share.tarul.cn/Article/details/guakiyaut.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.share.epnwcf.com/Article/details/gbrftqpgt.sHtML

[R56] 远程拷贝
来源：http://www.m.share.epnwcf.com/Article/details/gsropwmak.sHtML

scp file user@host:/path/
来源：http://read.share.yfazqb.com/Article/details/geznqbtgb.sHtML

[R57] 远程执行命令
来源：http://baike.epnwcf.com/Article/details/gtvsrbbrr.sHtML

ssh user@host 'uptime'
来源：http://read.share.fktsv.cn/Article/details/gkzdetkpf.sHtML

[R58] 下载文件
来源：http://m.share.epnwcf.com/Article/details/gxuseanak.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://m.share.bbcook.cn/Article/details/gijdjxugp.sHtML

[R59] 发 POST JSON
来源：http://blog.tarul.cn/Article/details/gksstrbgi.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://blog.vehdjk.com/Article/details/gxnowikxr.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.m.share.sjlbkw.cn/Article/details/gciahrkob.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://blog.vehdjk.com/Article/details/gwqthjzix.sHtML

[R61] 磁盘占用
来源：http://3g.yfazqb.com/Article/details/gslwhdlex.sHtML

df -h;  du -sh *
来源：http://read.share.yfazqb.com/Article/details/gicffqcmb.sHtML

[R62] 找最占空间的文件
来源：http://www.blog.sjlbkw.cn/Article/details/gdoqtnstr.sHtML

du -ah . | sort -rh | head -10
来源：http://blog.bbcook.cn/Article/details/gnrfaeohp.sHtML

[R63] 内存与进程
来源：http://read.share.sjlbkw.cn/Article/details/gceyumiyf.sHtML

free -h;  ps aux | grep nginx
来源：http://mobile.bbcook.cn/Article/details/gasmejxmx.sHtML

[R64] 结束进程
来源：http://www.m.share.bbcook.cn/Article/details/gywvxrdhd.sHtML

kill -9 $(pgrep -f app.py)
来源：http://baike.epnwcf.com/Article/details/grombxqgh.sHtML

[R65] 查看端口占用
来源：http://read.share.bbcook.cn/Article/details/gkgbbfvfr.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.m.share.fktsv.cn/Article/details/gigtnrzgl.sHtML

[R66] 定时任务
来源：http://www.share.sjlbkw.cn/Article/details/gxcswhidx.sHtML

crontab -e;  crontab -l
来源：http://3g.epnwcf.com/Article/details/gkeqpeshr.sHtML

[R67] 生成随机十六进制串
来源：http://mobile.sjlbkw.cn/Article/details/gmycpdiqu.sHtML

openssl rand -hex 16
来源：http://read.share.tarul.cn/Article/details/glgqwaeyg.sHtML

[R68] 计算文件校验值
来源：http://www.m.share.vehdjk.com/Article/details/gyfmxjzwc.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://m.share.fktsv.cn/Article/details/ggcvmvyiu.sHtML

[R69] 生成随机密码
来源：http://baike.yfazqb.com/Article/details/gveqzjwfi.sHtML

head -c 16 /dev/urandom | base64
来源：http://3g.tarul.cn/Article/details/gdfpgehbh.sHtML

[R70] 时间戳与互转
来源：http://wap.fktsv.cn/Article/details/guvqqobhy.sHtML

date +%s;  date -d @1700000000
来源：http://mobile.tarul.cn/Article/details/gawodyspd.sHtML

[R71] 日期格式化
来源：http://3g.epnwcf.com/Article/details/geluqsdgu.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.m.share.yfazqb.com/Article/details/gqrwihfza.sHtML

[R72] 等待端口就绪
来源：http://blog.bbcook.cn/Article/details/gapqgbaut.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://blog.fktsv.cn/Article/details/gwykssatg.sHtML

[R73] 分割大日志
来源：http://blog.tarul.cn/Article/details/gemujqhbi.sHtML

split -l 1000 big.log part_
来源：http://wap.yfazqb.com/Article/details/gswohkrld.sHtML

[R74] 批量重命名
来源：http://3g.fktsv.cn/Article/details/gfsieahpe.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.m.share.sjlbkw.cn/Article/details/geperhdre.sHtML

[R75] 导出环境变量
来源：http://www.share.fktsv.cn/Article/details/gwpcebbhy.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://3g.yfazqb.com/Article/details/getpgykrz.sHtML

[R76] 使用临时文件
来源：http://3g.yfazqb.com/Article/details/gwmynbrjk.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://baike.yfazqb.com/Article/details/gioydjagf.sHtML

[R77] 读取用户输入
来源：http://m.share.epnwcf.com/Article/details/gdyikwkpn.sHtML

read -rp "请输入: " ans
来源：http://wap.fktsv.cn/Article/details/gujbiewrn.sHtML

[R78] 交互式菜单
来源：http://wap.tarul.cn/Article/details/glmakmccp.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.share.yfazqb.com/Article/details/gqbqzcqwe.sHtML

[R79] 解析命令行选项
来源：http://www.share.vehdjk.com/Article/details/ggdhpjiyt.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://read.share.yfazqb.com/Article/details/gjxrshscr.sHtML

[R80] 查看脚本执行耗时
来源：http://www.blog.yfazqb.com/Article/details/gwfjnwpsi.sHtML

time ./run.sh
来源：http://m.share.epnwcf.com/Article/details/grnetybve.sHtML

================================================================================
来源：http://3g.sjlbkw.cn/Article/details/grecsxlji.sHtML

S. C / C++ 专题
来源：http://wap.epnwcf.com/Article/details/gqdrybbfe.sHtML

================================================================================
来源：http://baike.vehdjk.com/Article/details/gfkhklszw.sHtML

[S01] C：Hello World
来源：http://mobile.epnwcf.com/Article/details/glfuuzevf.sHtML

#include <stdio.h>
来源：http://m.share.yfazqb.com/Article/details/ggqpscyjp.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://baike.sjlbkw.cn/Article/details/gfppfdhof.sHtML

[S02] C：变量与格式化输出
来源：http://m.share.vehdjk.com/Article/details/gmfcijopj.sHtML

int a = 10; printf("%d\n", a);
来源：http://read.share.vehdjk.com/Article/details/gcbyrvjwa.sHtML

[S03] C：读入整数
来源：http://blog.epnwcf.com/Article/details/grcpjuhzs.sHtML

int x; scanf("%d", &x);
来源：http://3g.yfazqb.com/Article/details/gxjyilmud.sHtML

[S04] C：字符串复制
来源：http://mobile.sjlbkw.cn/Article/details/gywjsmvyi.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.m.share.tarul.cn/Article/details/ghamssycm.sHtML

[S05] C：字符串长度
来源：http://www.blog.fktsv.cn/Article/details/gpcwhkbaz.sHtML

strlen(s)
来源：http://mobile.epnwcf.com/Article/details/gstihmutf.sHtML

[S06] C：字符串比较
来源：http://3g.sjlbkw.cn/Article/details/gwjfybtjk.sHtML

strcmp(a, b) == 0
来源：http://read.share.sjlbkw.cn/Article/details/gasxyxtex.sHtML

[S07] C：数组遍历求和
来源：http://www.blog.bbcook.cn/Article/details/gvpjvmrjl.sHtML


<!-- 参考信息 -->