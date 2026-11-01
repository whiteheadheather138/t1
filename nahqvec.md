代发 wailian999

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://read.share.yfazqb.com/Article/details/gprmjpkqb.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://read.share.epnwcf.com/Article/details/gejpbscbb.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.share.yfazqb.com/Article/details/gfowdndbg.sHtML

[Q41] 多表连接
来源：http://read.share.epnwcf.com/Article/details/gyzgkiqri.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://blog.epnwcf.com/Article/details/gmvvoldex.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.blog.bbcook.cn/Article/details/gkijldpiq.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://m.share.sjlbkw.cn/Article/details/gzcfrfyfd.sHtML

[Q42] 连接条件附加过滤
来源：http://blog.fktsv.cn/Article/details/gttfoawgo.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.m.share.fktsv.cn/Article/details/gmiyijthp.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.blog.sjlbkw.cn/Article/details/grtaerigl.sHtML

[Q43] 标量子查询
来源：http://3g.vehdjk.com/Article/details/gvmahkjju.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.m.share.epnwcf.com/Article/details/gluceairo.sHtML

[Q44] IN 子查询
来源：http://blog.epnwcf.com/Article/details/gwjlhmlue.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://read.share.vehdjk.com/Article/details/grwqkgdbv.sHtML

[Q45] EXISTS 判断存在
来源：http://3g.yfazqb.com/Article/details/gfmwszcng.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.yfazqb.com/Article/details/gdglbpihp.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://wap.sjlbkw.cn/Article/details/gyiiewjoe.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.yfazqb.com/Article/details/gobhputus.sHtML

[Q47] 与平均值比较
来源：http://www.blog.epnwcf.com/Article/details/ghphuyvmk.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://3g.yfazqb.com/Article/details/goyknhvrx.sHtML

[Q48] CTE 公用表表达式
来源：http://wap.sjlbkw.cn/Article/details/ghxabvfoj.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://3g.tarul.cn/Article/details/gjdxxpfqw.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.m.share.vehdjk.com/Article/details/ghwjsuhto.sHtML

[Q49] 更新单行
来源：http://mobile.vehdjk.com/Article/details/gealgwedc.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.blog.bbcook.cn/Article/details/gszgvuglc.sHtML

[Q50] 批量更新
来源：http://www.m.share.vehdjk.com/Article/details/gqssidppv.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://read.share.vehdjk.com/Article/details/glohlhhah.sHtML

[Q51] 用子查询更新
来源：http://read.share.bbcook.cn/Article/details/gkpwymjcf.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://3g.yfazqb.com/Article/details/grotmilmp.sHtML

[Q52] 删除指定行
来源：http://www.share.sjlbkw.cn/Article/details/glqlvnabc.sHtML

DELETE FROM users WHERE id = 10;
来源：http://blog.yfazqb.com/Article/details/ghqfsyovm.sHtML

[Q53] 按条件删除
来源：http://baike.epnwcf.com/Article/details/guvvfdlob.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://wap.vehdjk.com/Article/details/gptobswio.sHtML

[Q54] 清空表
来源：http://www.share.epnwcf.com/Article/details/gmriyxcxr.sHtML

TRUNCATE TABLE logs;
来源：http://m.share.vehdjk.com/Article/details/gphrtoiry.sHtML

[Q55] 排名（并列占位）
来源：http://www.share.bbcook.cn/Article/details/grqovwzsc.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://3g.vehdjk.com/Article/details/gxfavyrwz.sHtML

[Q56] 密集排名（并列不占位）
来源：http://mobile.fktsv.cn/Article/details/gkztylvwd.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://wap.bbcook.cn/Article/details/gidtgdihy.sHtML

[Q57] 行号
来源：http://baike.yfazqb.com/Article/details/gllolzmlv.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://m.share.yfazqb.com/Article/details/gykuaifnj.sHtML

[Q58] 累计求和
来源：http://blog.yfazqb.com/Article/details/ghqtvjdry.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://blog.epnwcf.com/Article/details/grfycmvtk.sHtML

[Q59] 分组内累计
来源：http://wap.tarul.cn/Article/details/goojwgrgd.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.m.share.yfazqb.com/Article/details/gvtjwrykf.sHtML

[Q60] 取上一行 / 下一行
来源：http://3g.tarul.cn/Article/details/gpuwfemyu.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.blog.sjlbkw.cn/Article/details/glfnzwall.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.share.epnwcf.com/Article/details/ggijikfuj.sHtML

[Q61] 移动平均
来源：http://baike.tarul.cn/Article/details/gabjnaijv.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://m.share.tarul.cn/Article/details/gipznmzft.sHtML

[Q62] 分组占比
来源：http://m.share.epnwcf.com/Article/details/grrpicohq.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.m.share.yfazqb.com/Article/details/gpfwiaasb.sHtML

[Q63] 开启事务
来源：http://www.share.sjlbkw.cn/Article/details/gwffjbdrq.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://read.share.epnwcf.com/Article/details/guwcljtzg.sHtML

[Q64] 提交事务
来源：http://m.share.vehdjk.com/Article/details/gjrnltiqt.sHtML

COMMIT;
来源：http://www.blog.sjlbkw.cn/Article/details/gxqwvrxuu.sHtML

[Q65] 回滚事务
来源：http://3g.vehdjk.com/Article/details/ggszuuawk.sHtML

ROLLBACK;
来源：http://baike.sjlbkw.cn/Article/details/ghptytyco.sHtML

[Q66] 行锁查询
来源：http://m.share.epnwcf.com/Article/details/ggwpenxmz.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://wap.vehdjk.com/Article/details/gosnfwvsz.sHtML

[Q67] 设置隔离级别
来源：http://baike.epnwcf.com/Article/details/ggylbtvzw.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://baike.tarul.cn/Article/details/gzahnpwwy.sHtML

[Q68] 保存点
来源：http://baike.fktsv.cn/Article/details/gqslqmics.sHtML

SAVEPOINT sp1;
来源：http://www.m.share.fktsv.cn/Article/details/gtmcrrhzw.sHtML

ROLLBACK TO sp1;
来源：http://baike.vehdjk.com/Article/details/glzjbreal.sHtML

[Q69] 查看执行计划
来源：http://mobile.fktsv.cn/Article/details/gvnckjadj.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://mobile.epnwcf.com/Article/details/gjkwaiuvp.sHtML

[Q70] 更新统计信息
来源：http://www.blog.epnwcf.com/Article/details/gazqrbeln.sHtML

ANALYZE TABLE users;
来源：http://www.m.share.yfazqb.com/Article/details/gaeworaid.sHtML

[Q71] 查看建表语句
来源：http://www.blog.bbcook.cn/Article/details/gfblurnhm.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.blog.bbcook.cn/Article/details/gggvxqbwt.sHtML

[Q72] 查看索引
来源：http://read.share.vehdjk.com/Article/details/ggyywidwz.sHtML

SHOW INDEX FROM users;
来源：http://m.share.epnwcf.com/Article/details/gfpzesjyw.sHtML

[Q73] 查看表状态
来源：http://wap.sjlbkw.cn/Article/details/gcxrdxyxe.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://mobile.yfazqb.com/Article/details/gdonognmo.sHtML

[Q74] 强制使用索引
来源：http://www.m.share.tarul.cn/Article/details/gughecunk.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://baike.fktsv.cn/Article/details/gsjtmycrf.sHtML

[Q75] 日期格式化
来源：http://3g.sjlbkw.cn/Article/details/gpdyotlga.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.blog.vehdjk.com/Article/details/gehfrxlbj.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://blog.fktsv.cn/Article/details/gsbaonlaz.sHtML

[Q76] 按天统计
来源：http://www.share.tarul.cn/Article/details/gaxjzfpps.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://m.share.tarul.cn/Article/details/gzkiprfgo.sHtML

[Q77] 时间加减
来源：http://www.m.share.vehdjk.com/Article/details/gjhwyucpe.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.m.share.yfazqb.com/Article/details/gjfqthryk.sHtML

[Q78] 当前时间
来源：http://www.blog.sjlbkw.cn/Article/details/gduhcfdpj.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.share.tarul.cn/Article/details/gfaqbvsup.sHtML

[Q79] 字符串拼接
来源：http://www.share.vehdjk.com/Article/details/gjdlmnart.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://blog.sjlbkw.cn/Article/details/gjxuuazew.sHtML

[Q80] 字符串截取
来源：http://read.share.vehdjk.com/Article/details/gctrtzqen.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://mobile.fktsv.cn/Article/details/gjhhieceh.sHtML

[Q81] 字符串替换
来源：http://wap.vehdjk.com/Article/details/gmcyirirh.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.blog.sjlbkw.cn/Article/details/gzioeapbp.sHtML

[Q82] 字符长度与字节长度
来源：http://www.m.share.yfazqb.com/Article/details/grznehgmb.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://read.share.fktsv.cn/Article/details/gmbmmsimc.sHtML

[Q83] 大小写转换
来源：http://mobile.tarul.cn/Article/details/gsczhhyev.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.m.share.sjlbkw.cn/Article/details/gtswvksuc.sHtML

[Q84] 去除首尾空格
来源：http://mobile.sjlbkw.cn/Article/details/giqmnojhu.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.share.bbcook.cn/Article/details/gezevzgpz.sHtML

[Q85] 数值取整
来源：http://wap.yfazqb.com/Article/details/gloddliml.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.share.yfazqb.com/Article/details/goliuggzx.sHtML

[Q86] 读取 JSON 字段
来源：http://read.share.vehdjk.com/Article/details/gwprwkvsb.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://baike.epnwcf.com/Article/details/guvzzoetc.sHtML

[Q87] JSON 字段做条件
来源：http://wap.bbcook.cn/Article/details/gojfahnnc.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://m.share.tarul.cn/Article/details/gsesgqynh.sHtML

[Q88] 行转列（条件聚合）
来源：http://blog.epnwcf.com/Article/details/gqmchtccb.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.share.fktsv.cn/Article/details/gexcagabs.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.share.tarul.cn/Article/details/gdzrtwprf.sHtML

[Q89] 判断表是否存在
来源：http://mobile.bbcook.cn/Article/details/gprjuacuz.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.blog.yfazqb.com/Article/details/gqprxurlv.sHtML

[Q90] 生成序号列
来源：http://mobile.fktsv.cn/Article/details/gmhbcrjwh.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.m.share.epnwcf.com/Article/details/gfprulwpt.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/gyyzcozkv.sHtML

R. Bash 专题
来源：http://www.blog.vehdjk.com/Article/details/ghacemzan.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/gjlectopf.sHtML

[R01] shebang 与严格模式
来源：http://wap.fktsv.cn/Article/details/gatbxfypp.sHtML

#!/usr/bin/env bash
来源：http://3g.vehdjk.com/Article/details/gomsnftcs.sHtML

set -euo pipefail
来源：http://m.share.vehdjk.com/Article/details/ggfoxwjwf.sHtML

[R02] 变量赋值与使用
来源：http://www.m.share.sjlbkw.cn/Article/details/gkcengvpf.sHtML

name="Tom"; echo "$name"
来源：http://www.blog.epnwcf.com/Article/details/gxdnolspo.sHtML

[R03] 只读变量
来源：http://www.blog.tarul.cn/Article/details/gxfqpmyjp.sHtML

readonly PI=3.14
来源：http://blog.tarul.cn/Article/details/gavysfmpg.sHtML

[R04] 位置参数
来源：http://wap.yfazqb.com/Article/details/gorcyezhp.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://baike.tarul.cn/Article/details/gbcpqreow.sHtML

[R05] 参数默认值
来源：http://3g.epnwcf.com/Article/details/gpflbuhtm.sHtML

name="${1:-default}"
来源：http://baike.epnwcf.com/Article/details/gkjkwarvr.sHtML

[R06] 判断命令是否存在
来源：http://wap.tarul.cn/Article/details/gpdmjyllg.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://blog.fktsv.cn/Article/details/gbhnpgaam.sHtML

[R07] if 判断文件
来源：http://blog.fktsv.cn/Article/details/gqoymsjow.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://blog.bbcook.cn/Article/details/gsyjezvrs.sHtML

[R08] 数值比较
来源：http://baike.tarul.cn/Article/details/glawhqown.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.m.share.yfazqb.com/Article/details/gcqvrwpwt.sHtML

[R09] 字符串比较
来源：http://www.share.epnwcf.com/Article/details/gmnafsrms.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.share.epnwcf.com/Article/details/gyevvzmgg.sHtML

[R10] 正则匹配
来源：http://www.blog.tarul.cn/Article/details/gwojxcsbi.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://m.share.fktsv.cn/Article/details/gkmtraixc.sHtML

[R11] case 多分支
来源：http://blog.sjlbkw.cn/Article/details/gorskylna.sHtML

case "$1" in
来源：http://blog.sjlbkw.cn/Article/details/gifbsinfs.sHtML

start) echo "启动" ;;
来源：http://baike.fktsv.cn/Article/details/gnvwfhipj.sHtML

stop)  echo "停止" ;;
来源：http://www.blog.vehdjk.com/Article/details/gzczqmtqb.sHtML

*)     echo "未知命令" ;;
来源：http://blog.sjlbkw.cn/Article/details/gfwrhtqtg.sHtML

esac
来源：http://www.blog.sjlbkw.cn/Article/details/gfvtqjsfd.sHtML

[R12] for 遍历文件
来源：http://www.share.epnwcf.com/Article/details/gmsqlfhjz.sHtML

for f in *.txt; do echo "$f"; done
来源：http://baike.tarul.cn/Article/details/gfqyjvdun.sHtML

[R13] for 计数循环
来源：http://www.share.vehdjk.com/Article/details/gnyokodgr.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.share.yfazqb.com/Article/details/gegswzsio.sHtML

[R14] C 风格 for
来源：http://mobile.epnwcf.com/Article/details/gyaaqbxhe.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.blog.yfazqb.com/Article/details/gdglqqnvn.sHtML

[R15] while 逐行读文件
来源：http://blog.vehdjk.com/Article/details/galirpmdo.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.blog.bbcook.cn/Article/details/gfpeqkfzv.sHtML

[R16] until 等待条件
来源：http://mobile.yfazqb.com/Article/details/goccovobl.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.m.share.bbcook.cn/Article/details/gxqjarowq.sHtML

[R17] 数组定义与取值
来源：http://www.m.share.vehdjk.com/Article/details/gopdwsrer.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://blog.yfazqb.com/Article/details/gjybgsqrl.sHtML

[R18] 遍历数组
来源：http://read.share.bbcook.cn/Article/details/ggobuxspm.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.blog.tarul.cn/Article/details/gprtmmxqf.sHtML

[R19] 数组长度
来源：http://3g.bbcook.cn/Article/details/glfuvzsbr.sHtML

echo "${#arr[@]}"
来源：http://wap.tarul.cn/Article/details/gkizgygxn.sHtML

[R20] 关联数组（字典）
来源：http://mobile.tarul.cn/Article/details/gilebueyu.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://m.share.bbcook.cn/Article/details/gfexxlide.sHtML

[R21] 字符串长度
来源：http://read.share.sjlbkw.cn/Article/details/gxzxmkwpr.sHtML

echo "${#s}"
来源：http://mobile.yfazqb.com/Article/details/gpyscqvrt.sHtML

[R22] 截取子串
来源：http://www.share.sjlbkw.cn/Article/details/gfecynczm.sHtML

echo "${s:0:5}"
来源：http://read.share.vehdjk.com/Article/details/gtelnzdtc.sHtML

[R23] 字符串替换
来源：http://read.share.fktsv.cn/Article/details/gjptookoy.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://baike.bbcook.cn/Article/details/gvmrqshoo.sHtML

[R24] 大小写转换
来源：http://3g.tarul.cn/Article/details/gymaaamky.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://m.share.vehdjk.com/Article/details/gpfbjhppw.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.m.share.tarul.cn/Article/details/gdlwqydea.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.share.bbcook.cn/Article/details/ggsunfllb.sHtML

[R26] 命令替换
来源：http://read.share.bbcook.cn/Article/details/gnmbzfzpi.sHtML

now=$(date +%F); echo "$now"
来源：http://m.share.epnwcf.com/Article/details/gkqutalxq.sHtML

[R27] 算术展开
来源：http://m.share.vehdjk.com/Article/details/gldpsnluq.sHtML

echo $((1 + 2 * 3))
来源：http://www.blog.tarul.cn/Article/details/gbudwompe.sHtML

[R28] 浮点运算
来源：http://m.share.yfazqb.com/Article/details/gywnwjjgy.sHtML

echo "scale=2; 10/3" | bc
来源：http://read.share.fktsv.cn/Article/details/galmuuegb.sHtML

[R29] 定义函数
来源：http://www.m.share.yfazqb.com/Article/details/gfzknhyir.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.m.share.epnwcf.com/Article/details/gjswqnqpz.sHtML

[R30] 函数返回状态码
来源：http://baike.epnwcf.com/Article/details/ggvqwcjub.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.share.yfazqb.com/Article/details/gyxlaqrvz.sHtML

[R31] 局部变量
来源：http://www.blog.tarul.cn/Article/details/gjmjviqyh.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.share.bbcook.cn/Article/details/gggxaflfm.sHtML

[R32] 参数个数校验
来源：http://www.m.share.yfazqb.com/Article/details/gbhynjnlx.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://3g.yfazqb.com/Article/details/givonxkec.sHtML

[R33] 捕获错误并提示行号
来源：http://www.blog.sjlbkw.cn/Article/details/gerwxfoll.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://m.share.bbcook.cn/Article/details/gvwhfzfce.sHtML

[R34] 退出时清理
来源：http://m.share.sjlbkw.cn/Article/details/guvfesbiv.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://wap.vehdjk.com/Article/details/gcspnqcmk.sHtML

[R35] 后台执行并等待
来源：http://www.blog.tarul.cn/Article/details/gvmqdtlvu.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://mobile.fktsv.cn/Article/details/gfityxdmq.sHtML

[R36] 并发执行多个任务
来源：http://m.share.epnwcf.com/Article/details/gfcgvxqxa.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://wap.epnwcf.com/Article/details/gjvwyrvux.sHtML

[R37] 把输出赋给变量
来源：http://www.blog.bbcook.cn/Article/details/gjjqjfdeo.sHtML

files=$(ls -1)
来源：http://mobile.tarul.cn/Article/details/gsveqmfns.sHtML

[R38] 管道串联
来源：http://www.share.sjlbkw.cn/Article/details/gtrynjdir.sHtML

cat a.txt | grep -i error | wc -l
来源：http://3g.sjlbkw.cn/Article/details/gorekwlbk.sHtML

[R39] 重定向标准输出与错误
来源：http://www.m.share.tarul.cn/Article/details/gnatxcsxd.sHtML

cmd > out.log 2>&1
来源：http://www.m.share.vehdjk.com/Article/details/genoxkgky.sHtML

[R40] 追加写日志
来源：http://www.share.sjlbkw.cn/Article/details/gmqzvrufx.sHtML

echo "log" >> out.log
来源：http://m.share.epnwcf.com/Article/details/gsayaoyuw.sHtML

[R41] 丢弃输出
来源：http://wap.tarul.cn/Article/details/gwmvpndza.sHtML

cmd >/dev/null 2>&1
来源：http://m.share.yfazqb.com/Article/details/gnpxyxevh.sHtML

[R42] 输入重定向
来源：http://www.blog.yfazqb.com/Article/details/gyqldsdxt.sHtML

wc -l < a.txt
来源：http://www.share.sjlbkw.cn/Article/details/garpnqpof.sHtML

[R43] 按名字查找文件
来源：http://blog.yfazqb.com/Article/details/goromedpm.sHtML

find . -name "*.log" -type f
来源：http://baike.sjlbkw.cn/Article/details/gnidghzbe.sHtML

[R44] 按修改时间查找
来源：http://wap.yfazqb.com/Article/details/gmxorutsg.sHtML

find . -mtime -7 -type f
来源：http://www.share.fktsv.cn/Article/details/gmfwqzrqs.sHtML

[R45] 批量删除
来源：http://m.share.vehdjk.com/Article/details/gyekcomox.sHtML

find . -name "*.tmp" -delete
来源：http://read.share.yfazqb.com/Article/details/grhncguox.sHtML

[R46] 递归替换文件内容
来源：http://mobile.vehdjk.com/Article/details/gopnhyxud.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mobile.yfazqb.com/Article/details/gfzeyktvo.sHtML

[R47] sed 单行替换
来源：http://read.share.epnwcf.com/Article/details/gnfbxcqbt.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://mobile.epnwcf.com/Article/details/gugaxiaov.sHtML

[R48] awk 取指定列
来源：http://3g.fktsv.cn/Article/details/gzdubocce.sHtML

awk '{print $1, $3}' a.txt
来源：http://blog.tarul.cn/Article/details/gzjufjmwj.sHtML

[R49] awk 带条件
来源：http://blog.epnwcf.com/Article/details/gbieqvakt.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://3g.yfazqb.com/Article/details/gqivvnbmm.sHtML

[R50] awk 求和
来源：http://baike.tarul.cn/Article/details/gqfzfkpfo.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://read.share.sjlbkw.cn/Article/details/gzpxdmwub.sHtML

[R51] 排序去重取前几
来源：http://blog.fktsv.cn/Article/details/gzvazgfqy.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://wap.fktsv.cn/Article/details/gbmakxuho.sHtML

[R52] 统计行数
来源：http://wap.epnwcf.com/Article/details/gknvbkufh.sHtML

wc -l a.txt
来源：http://baike.epnwcf.com/Article/details/gilkayvpq.sHtML

[R53] 查看文件头与实时尾
来源：http://www.blog.bbcook.cn/Article/details/gwnviqwpl.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://m.share.epnwcf.com/Article/details/guafztany.sHtML

[R54] 比较两个文件
来源：http://read.share.vehdjk.com/Article/details/gktudzpjp.sHtML

diff a.txt b.txt
来源：http://www.share.vehdjk.com/Article/details/geyfgqzfl.sHtML

[R55] 压缩与解压
来源：http://blog.sjlbkw.cn/Article/details/gyokpykvv.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.share.bbcook.cn/Article/details/gwfiyiqon.sHtML

[R56] 远程拷贝
来源：http://www.share.yfazqb.com/Article/details/gusttqjsn.sHtML

scp file user@host:/path/
来源：http://www.share.bbcook.cn/Article/details/gjloenzyd.sHtML

[R57] 远程执行命令
来源：http://www.share.tarul.cn/Article/details/gqkncojvc.sHtML

ssh user@host 'uptime'
来源：http://www.share.tarul.cn/Article/details/gcxrogslw.sHtML

[R58] 下载文件
来源：http://3g.sjlbkw.cn/Article/details/gxqtclhbo.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.blog.vehdjk.com/Article/details/gtlwivmxi.sHtML

[R59] 发 POST JSON
来源：http://3g.sjlbkw.cn/Article/details/gzgvukphd.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.blog.yfazqb.com/Article/details/grsjieqil.sHtML

[R60] 只看 HTTP 状态码
来源：http://m.share.fktsv.cn/Article/details/gwunqbgjw.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mobile.yfazqb.com/Article/details/goaoidvsc.sHtML

[R61] 磁盘占用
来源：http://www.share.epnwcf.com/Article/details/gspuqxelc.sHtML

df -h;  du -sh *
来源：http://3g.tarul.cn/Article/details/gfzfccatc.sHtML

[R62] 找最占空间的文件
来源：http://blog.yfazqb.com/Article/details/ginecvqek.sHtML

du -ah . | sort -rh | head -10
来源：http://www.blog.vehdjk.com/Article/details/gcimxhnez.sHtML

[R63] 内存与进程
来源：http://m.share.sjlbkw.cn/Article/details/gzshmgeyo.sHtML

free -h;  ps aux | grep nginx
来源：http://baike.tarul.cn/Article/details/gjnxkbjit.sHtML

[R64] 结束进程
来源：http://wap.fktsv.cn/Article/details/guluksanv.sHtML

kill -9 $(pgrep -f app.py)
来源：http://3g.tarul.cn/Article/details/gdzgwzaev.sHtML

[R65] 查看端口占用
来源：http://3g.epnwcf.com/Article/details/gqdzutmdl.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mobile.epnwcf.com/Article/details/gzrtwgnws.sHtML

[R66] 定时任务
来源：http://baike.fktsv.cn/Article/details/gucthxzur.sHtML

crontab -e;  crontab -l
来源：http://www.m.share.sjlbkw.cn/Article/details/gnajtxjat.sHtML

[R67] 生成随机十六进制串
来源：http://www.m.share.yfazqb.com/Article/details/gdhbjksvk.sHtML

openssl rand -hex 16
来源：http://3g.sjlbkw.cn/Article/details/gqxmgpqcl.sHtML

[R68] 计算文件校验值
来源：http://m.share.vehdjk.com/Article/details/gqwygaguz.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://m.share.vehdjk.com/Article/details/grhjndbjo.sHtML

[R69] 生成随机密码
来源：http://m.share.epnwcf.com/Article/details/gxjzrwxer.sHtML

head -c 16 /dev/urandom | base64
来源：http://mobile.epnwcf.com/Article/details/ghbjueozj.sHtML

[R70] 时间戳与互转
来源：http://www.m.share.sjlbkw.cn/Article/details/gdzwseffn.sHtML

date +%s;  date -d @1700000000
来源：http://mobile.vehdjk.com/Article/details/gbkwofbkc.sHtML

[R71] 日期格式化
来源：http://blog.vehdjk.com/Article/details/gqliytvai.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://m.share.tarul.cn/Article/details/gusnypknk.sHtML

[R72] 等待端口就绪
来源：http://www.blog.yfazqb.com/Article/details/gxenohynt.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://m.share.vehdjk.com/Article/details/geywypmne.sHtML

[R73] 分割大日志
来源：http://mobile.bbcook.cn/Article/details/gnfmnfvww.sHtML

split -l 1000 big.log part_
来源：http://baike.bbcook.cn/Article/details/gnzbnkqvx.sHtML

[R74] 批量重命名
来源：http://www.m.share.vehdjk.com/Article/details/gocdmjrll.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.share.sjlbkw.cn/Article/details/gpvrpvywr.sHtML

[R75] 导出环境变量
来源：http://www.blog.sjlbkw.cn/Article/details/gocfgztal.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://read.share.sjlbkw.cn/Article/details/gbsjqxvqq.sHtML

[R76] 使用临时文件
来源：http://www.blog.tarul.cn/Article/details/ghuyminjf.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://wap.bbcook.cn/Article/details/grlerqzvw.sHtML

[R77] 读取用户输入
来源：http://m.share.sjlbkw.cn/Article/details/gfogvnxsd.sHtML

read -rp "请输入: " ans
来源：http://www.blog.yfazqb.com/Article/details/gmigicibu.sHtML

[R78] 交互式菜单
来源：http://www.share.epnwcf.com/Article/details/gftkijbbw.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.blog.bbcook.cn/Article/details/gxrqvhfnb.sHtML

[R79] 解析命令行选项
来源：http://baike.vehdjk.com/Article/details/gwvwtgdok.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.blog.tarul.cn/Article/details/ghbbinlfx.sHtML

[R80] 查看脚本执行耗时
来源：http://mobile.vehdjk.com/Article/details/gzlpvojzh.sHtML

time ./run.sh
来源：http://mobile.yfazqb.com/Article/details/gdprlghob.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/gmgebyjeo.sHtML

S. C / C++ 专题
来源：http://m.share.yfazqb.com/Article/details/gawpnefnh.sHtML

================================================================================
来源：http://baike.sjlbkw.cn/Article/details/gzmhyohqv.sHtML

[S01] C：Hello World
来源：http://www.m.share.sjlbkw.cn/Article/details/gvygkvclb.sHtML

#include <stdio.h>
来源：http://www.m.share.vehdjk.com/Article/details/golswwlgk.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gsprnyzrm.sHtML

[S02] C：变量与格式化输出
来源：http://www.blog.epnwcf.com/Article/details/goezxdqhp.sHtML

int a = 10; printf("%d\n", a);
来源：http://read.share.sjlbkw.cn/Article/details/gyijwzvhz.sHtML

[S03] C：读入整数
来源：http://read.share.tarul.cn/Article/details/glkxcffej.sHtML

int x; scanf("%d", &x);
来源：http://read.share.epnwcf.com/Article/details/ghgrtlkna.sHtML

[S04] C：字符串复制
来源：http://www.share.fktsv.cn/Article/details/gfnmuabnm.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.share.yfazqb.com/Article/details/gmspiwmpq.sHtML

[S05] C：字符串长度
来源：http://wap.fktsv.cn/Article/details/geljargfq.sHtML

strlen(s)
来源：http://3g.tarul.cn/Article/details/gherywcdz.sHtML

[S06] C：字符串比较
来源：http://www.share.tarul.cn/Article/details/gwuwljjui.sHtML

strcmp(a, b) == 0
来源：http://blog.bbcook.cn/Article/details/ghfkktxbj.sHtML

[S07] C：数组遍历求和
来源：http://www.blog.fktsv.cn/Article/details/grobvkrza.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://read.share.sjlbkw.cn/Article/details/gkpnvssmx.sHtML

[S08] C：动态内存分配与释放
来源：http://www.share.fktsv.cn/Article/details/gcazyqfxz.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mobile.fktsv.cn/Article/details/gwdlyjxkj.sHtML

[S09] C：结构体定义与初始化
来源：http://www.blog.tarul.cn/Article/details/glivfggih.sHtML


<!-- 参考信息 -->