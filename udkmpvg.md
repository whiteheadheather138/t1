代发 wailian999

[Q36] 左连接
来源：http://www.m.share.yfazqb.com/Article/details/gunwgjvqq.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.yfazqb.com/Article/details/gsaeeumiw.sHtML

[Q37] 右连接
来源：http://www.blog.epnwcf.com/Article/details/gdohnozgf.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://baike.sjlbkw.cn/Article/details/gccisfsoz.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://wap.vehdjk.com/Article/details/ghlrnzouc.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.share.yfazqb.com/Article/details/gotbsgsmf.sHtML

[Q39] 自连接（查上下级）
来源：http://baike.fktsv.cn/Article/details/gbfusnfpc.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.share.yfazqb.com/Article/details/gvivhhvhk.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://3g.bbcook.cn/Article/details/giouofpfd.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.blog.fktsv.cn/Article/details/ghenarssg.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://read.share.sjlbkw.cn/Article/details/gzvvcunjn.sHtML

[Q41] 多表连接
来源：http://www.share.epnwcf.com/Article/details/gwqpbvnma.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.blog.vehdjk.com/Article/details/gpgktjlad.sHtML

JOIN users u ON u.id = o.user_id
来源：http://baike.tarul.cn/Article/details/gwhobvxvh.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://blog.yfazqb.com/Article/details/gipajxgdh.sHtML

[Q42] 连接条件附加过滤
来源：http://3g.vehdjk.com/Article/details/gjwdxxhdi.sHtML

SELECT u.name, o.amount FROM users u
来源：http://wap.bbcook.cn/Article/details/gduhcudjz.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.share.vehdjk.com/Article/details/gwwzpsmqr.sHtML

[Q43] 标量子查询
来源：http://3g.vehdjk.com/Article/details/gwmaqkyis.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.share.fktsv.cn/Article/details/glecjpgub.sHtML

[Q44] IN 子查询
来源：http://baike.bbcook.cn/Article/details/gmbanmeod.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://baike.fktsv.cn/Article/details/gvmlxudtf.sHtML

[Q45] EXISTS 判断存在
来源：http://baike.epnwcf.com/Article/details/grwgwqxfd.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.fktsv.cn/Article/details/gsifaboeu.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://m.share.yfazqb.com/Article/details/gvmoqhute.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.fktsv.cn/Article/details/gxbphznwo.sHtML

[Q47] 与平均值比较
来源：http://baike.vehdjk.com/Article/details/gjvjqnijt.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://3g.bbcook.cn/Article/details/gurxbvmau.sHtML

[Q48] CTE 公用表表达式
来源：http://www.blog.fktsv.cn/Article/details/gjcfmbbjz.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://baike.bbcook.cn/Article/details/gvpvorcwe.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.share.bbcook.cn/Article/details/gwunzrlne.sHtML

[Q49] 更新单行
来源：http://read.share.yfazqb.com/Article/details/gqdbswvgc.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.m.share.sjlbkw.cn/Article/details/gusxeimaz.sHtML

[Q50] 批量更新
来源：http://baike.epnwcf.com/Article/details/gwmxalgqi.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://mobile.fktsv.cn/Article/details/gunruevcb.sHtML

[Q51] 用子查询更新
来源：http://www.m.share.fktsv.cn/Article/details/gmyatoiep.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.m.share.yfazqb.com/Article/details/gcobsjjcv.sHtML

[Q52] 删除指定行
来源：http://m.share.bbcook.cn/Article/details/gantsuilf.sHtML

DELETE FROM users WHERE id = 10;
来源：http://baike.sjlbkw.cn/Article/details/gyilujymb.sHtML

[Q53] 按条件删除
来源：http://www.m.share.fktsv.cn/Article/details/gfxxfigih.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://wap.tarul.cn/Article/details/gzxixgwzr.sHtML

[Q54] 清空表
来源：http://wap.sjlbkw.cn/Article/details/gykxzjgap.sHtML

TRUNCATE TABLE logs;
来源：http://www.blog.epnwcf.com/Article/details/gjlgwbydb.sHtML

[Q55] 排名（并列占位）
来源：http://www.blog.sjlbkw.cn/Article/details/gtyymlrxi.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.share.bbcook.cn/Article/details/gcvobvwos.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.m.share.sjlbkw.cn/Article/details/gjmhvcjig.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://3g.sjlbkw.cn/Article/details/gssdfgxqf.sHtML

[Q57] 行号
来源：http://read.share.sjlbkw.cn/Article/details/gataxsmvf.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.blog.vehdjk.com/Article/details/gpssbuqbv.sHtML

[Q58] 累计求和
来源：http://m.share.bbcook.cn/Article/details/gnhewhulk.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://3g.tarul.cn/Article/details/gchvhvyvh.sHtML

[Q59] 分组内累计
来源：http://3g.vehdjk.com/Article/details/gwwfdcvis.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.share.yfazqb.com/Article/details/gepwiurln.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.m.share.yfazqb.com/Article/details/gnsyujhik.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.share.yfazqb.com/Article/details/gmwyqjiou.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://read.share.sjlbkw.cn/Article/details/gvxmgykuu.sHtML

[Q61] 移动平均
来源：http://www.blog.bbcook.cn/Article/details/gbydtprhb.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://read.share.yfazqb.com/Article/details/gywhrwldb.sHtML

[Q62] 分组占比
来源：http://baike.sjlbkw.cn/Article/details/giiwitaxp.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://3g.yfazqb.com/Article/details/gshlkcqdj.sHtML

[Q63] 开启事务
来源：http://www.m.share.bbcook.cn/Article/details/gtsvlefyb.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://3g.sjlbkw.cn/Article/details/gvtcotdgz.sHtML

[Q64] 提交事务
来源：http://www.blog.epnwcf.com/Article/details/gwbdhnlto.sHtML

COMMIT;
来源：http://mobile.sjlbkw.cn/Article/details/grqpiitaf.sHtML

[Q65] 回滚事务
来源：http://wap.yfazqb.com/Article/details/gcuwbvlsb.sHtML

ROLLBACK;
来源：http://wap.bbcook.cn/Article/details/grmnnjgpv.sHtML

[Q66] 行锁查询
来源：http://blog.epnwcf.com/Article/details/gqdfspxal.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.m.share.epnwcf.com/Article/details/gywjdezwu.sHtML

[Q67] 设置隔离级别
来源：http://wap.epnwcf.com/Article/details/gihjyniug.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.share.tarul.cn/Article/details/gmajuukdu.sHtML

[Q68] 保存点
来源：http://mobile.sjlbkw.cn/Article/details/ghixhvjsg.sHtML

SAVEPOINT sp1;
来源：http://www.blog.sjlbkw.cn/Article/details/gtsoqskji.sHtML

ROLLBACK TO sp1;
来源：http://www.blog.epnwcf.com/Article/details/gqpldvcax.sHtML

[Q69] 查看执行计划
来源：http://www.m.share.sjlbkw.cn/Article/details/glyuchxtc.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.share.tarul.cn/Article/details/gdfjalsgd.sHtML

[Q70] 更新统计信息
来源：http://mobile.epnwcf.com/Article/details/gtifbmbex.sHtML

ANALYZE TABLE users;
来源：http://wap.epnwcf.com/Article/details/glvmnyeim.sHtML

[Q71] 查看建表语句
来源：http://baike.yfazqb.com/Article/details/gxxekpisn.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://baike.yfazqb.com/Article/details/grnqlxmao.sHtML

[Q72] 查看索引
来源：http://mobile.tarul.cn/Article/details/gseeuezkv.sHtML

SHOW INDEX FROM users;
来源：http://www.blog.yfazqb.com/Article/details/gwdtymjrj.sHtML

[Q73] 查看表状态
来源：http://blog.bbcook.cn/Article/details/gvraxmbcc.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.blog.fktsv.cn/Article/details/gsjakfjye.sHtML

[Q74] 强制使用索引
来源：http://3g.tarul.cn/Article/details/gavdzigwc.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://wap.sjlbkw.cn/Article/details/gwvrthwcc.sHtML

[Q75] 日期格式化
来源：http://m.share.fktsv.cn/Article/details/gmffhxjmr.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://m.share.fktsv.cn/Article/details/gdbcfoapj.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.share.epnwcf.com/Article/details/gwremzjpz.sHtML

[Q76] 按天统计
来源：http://read.share.epnwcf.com/Article/details/gkhvnhgcz.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://read.share.yfazqb.com/Article/details/geoxifcob.sHtML

[Q77] 时间加减
来源：http://baike.fktsv.cn/Article/details/gbmgbsddw.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.blog.fktsv.cn/Article/details/gtwvomhwl.sHtML

[Q78] 当前时间
来源：http://www.share.tarul.cn/Article/details/gpumetatv.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://blog.vehdjk.com/Article/details/gyuzxyvcl.sHtML

[Q79] 字符串拼接
来源：http://baike.fktsv.cn/Article/details/gwhlimidl.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://baike.epnwcf.com/Article/details/gtkcgroxv.sHtML

[Q80] 字符串截取
来源：http://www.blog.tarul.cn/Article/details/gzvdqxkns.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://3g.epnwcf.com/Article/details/gpvcehkcp.sHtML

[Q81] 字符串替换
来源：http://mobile.yfazqb.com/Article/details/ghshnxqmg.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://baike.fktsv.cn/Article/details/ggtpskzdd.sHtML

[Q82] 字符长度与字节长度
来源：http://blog.epnwcf.com/Article/details/gkzjahuwx.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://blog.bbcook.cn/Article/details/gmqwzlufo.sHtML

[Q83] 大小写转换
来源：http://mobile.sjlbkw.cn/Article/details/gagyaozdk.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://wap.vehdjk.com/Article/details/gegljlihd.sHtML

[Q84] 去除首尾空格
来源：http://wap.tarul.cn/Article/details/gavxitqtb.sHtML

SELECT TRIM(name) FROM users;
来源：http://m.share.fktsv.cn/Article/details/gseymoybi.sHtML

[Q85] 数值取整
来源：http://3g.tarul.cn/Article/details/gydordmtz.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://3g.sjlbkw.cn/Article/details/ggvggfrrb.sHtML

[Q86] 读取 JSON 字段
来源：http://www.blog.fktsv.cn/Article/details/gkorqaqdh.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.share.fktsv.cn/Article/details/gxgpfwlsy.sHtML

[Q87] JSON 字段做条件
来源：http://www.blog.epnwcf.com/Article/details/gixhmeuph.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.m.share.vehdjk.com/Article/details/gcdcrulgs.sHtML

[Q88] 行转列（条件聚合）
来源：http://3g.bbcook.cn/Article/details/gwapcdjwd.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://read.share.yfazqb.com/Article/details/garbjyuob.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://wap.sjlbkw.cn/Article/details/gonjhsqaj.sHtML

[Q89] 判断表是否存在
来源：http://m.share.bbcook.cn/Article/details/goaorfcrg.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.blog.yfazqb.com/Article/details/gfbhyydod.sHtML

[Q90] 生成序号列
来源：http://wap.yfazqb.com/Article/details/gclxonrpg.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://m.share.epnwcf.com/Article/details/gdoihvgds.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/gtpjaaocg.sHtML

R. Bash 专题
来源：http://www.blog.tarul.cn/Article/details/gfnpvjwsg.sHtML

================================================================================
来源：http://3g.sjlbkw.cn/Article/details/gpntkhgdy.sHtML

[R01] shebang 与严格模式
来源：http://www.share.vehdjk.com/Article/details/gwlkwalas.sHtML

#!/usr/bin/env bash
来源：http://baike.epnwcf.com/Article/details/gilmdixqp.sHtML

set -euo pipefail
来源：http://wap.vehdjk.com/Article/details/gbjgsgdsq.sHtML

[R02] 变量赋值与使用
来源：http://blog.vehdjk.com/Article/details/gedxzyeui.sHtML

name="Tom"; echo "$name"
来源：http://wap.yfazqb.com/Article/details/gxgvnipwr.sHtML

[R03] 只读变量
来源：http://www.m.share.yfazqb.com/Article/details/grmppwntc.sHtML

readonly PI=3.14
来源：http://mobile.tarul.cn/Article/details/gnjxizrya.sHtML

[R04] 位置参数
来源：http://wap.vehdjk.com/Article/details/giqtynsak.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://read.share.fktsv.cn/Article/details/gadialdiy.sHtML

[R05] 参数默认值
来源：http://www.m.share.sjlbkw.cn/Article/details/ggzmrvzkv.sHtML

name="${1:-default}"
来源：http://read.share.tarul.cn/Article/details/gesdwnpdg.sHtML

[R06] 判断命令是否存在
来源：http://wap.bbcook.cn/Article/details/gpjoccdgd.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://m.share.vehdjk.com/Article/details/gwbunjdas.sHtML

[R07] if 判断文件
来源：http://www.share.bbcook.cn/Article/details/gnrvrkowt.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.m.share.sjlbkw.cn/Article/details/gqjxuppyk.sHtML

[R08] 数值比较
来源：http://m.share.tarul.cn/Article/details/gsklilspr.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://read.share.epnwcf.com/Article/details/ghiibnjmq.sHtML

[R09] 字符串比较
来源：http://www.blog.vehdjk.com/Article/details/gciaasqbw.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://m.share.vehdjk.com/Article/details/gqmpyioqq.sHtML

[R10] 正则匹配
来源：http://read.share.vehdjk.com/Article/details/gihukmmqz.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.blog.sjlbkw.cn/Article/details/gakcytwmy.sHtML

[R11] case 多分支
来源：http://wap.epnwcf.com/Article/details/gxawnbneb.sHtML

case "$1" in
来源：http://baike.tarul.cn/Article/details/gyrsclmhc.sHtML

start) echo "启动" ;;
来源：http://mobile.sjlbkw.cn/Article/details/gdcnplgfv.sHtML

stop)  echo "停止" ;;
来源：http://blog.sjlbkw.cn/Article/details/gigoomjvs.sHtML

*)     echo "未知命令" ;;
来源：http://3g.yfazqb.com/Article/details/gsyajafrq.sHtML

esac
来源：http://www.share.fktsv.cn/Article/details/ggclittov.sHtML

[R12] for 遍历文件
来源：http://mobile.bbcook.cn/Article/details/gojhplqfx.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.m.share.yfazqb.com/Article/details/gtkfdosfl.sHtML

[R13] for 计数循环
来源：http://m.share.epnwcf.com/Article/details/gamykgjpx.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.m.share.sjlbkw.cn/Article/details/gzjlrgjnb.sHtML

[R14] C 风格 for
来源：http://www.share.bbcook.cn/Article/details/gqustnngi.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.m.share.yfazqb.com/Article/details/gdddppxzv.sHtML

[R15] while 逐行读文件
来源：http://mobile.vehdjk.com/Article/details/gopapyhow.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://read.share.yfazqb.com/Article/details/gxebnqram.sHtML

[R16] until 等待条件
来源：http://blog.epnwcf.com/Article/details/gonwjjhbk.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://mobile.epnwcf.com/Article/details/gttzwyivs.sHtML

[R17] 数组定义与取值
来源：http://mobile.tarul.cn/Article/details/gbidvfndv.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://wap.yfazqb.com/Article/details/gnyxqpsyt.sHtML

[R18] 遍历数组
来源：http://www.blog.tarul.cn/Article/details/ggxhziusn.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://3g.sjlbkw.cn/Article/details/gmbehdlsy.sHtML

[R19] 数组长度
来源：http://www.blog.bbcook.cn/Article/details/gnbhlpkor.sHtML

echo "${#arr[@]}"
来源：http://m.share.sjlbkw.cn/Article/details/gqqqzjmlo.sHtML

[R20] 关联数组（字典）
来源：http://blog.vehdjk.com/Article/details/gdlvffcjm.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.blog.bbcook.cn/Article/details/gvmvegrdy.sHtML

[R21] 字符串长度
来源：http://m.share.tarul.cn/Article/details/ghustwdjp.sHtML

echo "${#s}"
来源：http://www.m.share.sjlbkw.cn/Article/details/gjfhmlhvw.sHtML

[R22] 截取子串
来源：http://www.m.share.fktsv.cn/Article/details/gbbztomdg.sHtML

echo "${s:0:5}"
来源：http://3g.epnwcf.com/Article/details/gvyyksdjp.sHtML

[R23] 字符串替换
来源：http://read.share.epnwcf.com/Article/details/goatqhcqf.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://blog.sjlbkw.cn/Article/details/gmonmirwu.sHtML

[R24] 大小写转换
来源：http://3g.tarul.cn/Article/details/gfbfngqbx.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.share.epnwcf.com/Article/details/gmzszrlwy.sHtML

[R25] 去后缀 / 去前缀
来源：http://m.share.epnwcf.com/Article/details/gyoppjtzw.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://mobile.sjlbkw.cn/Article/details/giscpnjzl.sHtML

[R26] 命令替换
来源：http://www.m.share.epnwcf.com/Article/details/gxlphemdi.sHtML

now=$(date +%F); echo "$now"
来源：http://wap.yfazqb.com/Article/details/grpfiopzw.sHtML

[R27] 算术展开
来源：http://baike.yfazqb.com/Article/details/gieqzjupo.sHtML

echo $((1 + 2 * 3))
来源：http://www.blog.yfazqb.com/Article/details/gjgycoswc.sHtML

[R28] 浮点运算
来源：http://read.share.bbcook.cn/Article/details/gkrueextx.sHtML

echo "scale=2; 10/3" | bc
来源：http://m.share.vehdjk.com/Article/details/gqopcqmhz.sHtML

[R29] 定义函数
来源：http://www.share.sjlbkw.cn/Article/details/gpwyluzxa.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.share.epnwcf.com/Article/details/gubkhkxtq.sHtML

[R30] 函数返回状态码
来源：http://www.m.share.fktsv.cn/Article/details/gmpqkhemd.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.blog.epnwcf.com/Article/details/gpjatvohr.sHtML

[R31] 局部变量
来源：http://m.share.vehdjk.com/Article/details/gmzbdbgyk.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.m.share.yfazqb.com/Article/details/glntollsm.sHtML

[R32] 参数个数校验
来源：http://www.m.share.fktsv.cn/Article/details/gazvfgejs.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://3g.epnwcf.com/Article/details/gokkclith.sHtML

[R33] 捕获错误并提示行号
来源：http://m.share.tarul.cn/Article/details/gkcyorqrf.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.share.fktsv.cn/Article/details/gpiehgovq.sHtML

[R34] 退出时清理
来源：http://baike.epnwcf.com/Article/details/gygrmsxwp.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://read.share.vehdjk.com/Article/details/goejvsxxb.sHtML

[R35] 后台执行并等待
来源：http://blog.fktsv.cn/Article/details/gvgxsxwsj.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://m.share.vehdjk.com/Article/details/gjpkvoxic.sHtML

[R36] 并发执行多个任务
来源：http://www.blog.bbcook.cn/Article/details/glgblucfm.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.m.share.fktsv.cn/Article/details/gncyqxofu.sHtML

[R37] 把输出赋给变量
来源：http://3g.epnwcf.com/Article/details/gqewobmqu.sHtML

files=$(ls -1)
来源：http://www.m.share.vehdjk.com/Article/details/gsinzkhnq.sHtML

[R38] 管道串联
来源：http://blog.sjlbkw.cn/Article/details/genpukjai.sHtML

cat a.txt | grep -i error | wc -l
来源：http://baike.fktsv.cn/Article/details/gamlveked.sHtML

[R39] 重定向标准输出与错误
来源：http://wap.fktsv.cn/Article/details/gfsinrdkv.sHtML

cmd > out.log 2>&1
来源：http://blog.fktsv.cn/Article/details/gafgvifjv.sHtML

[R40] 追加写日志
来源：http://baike.fktsv.cn/Article/details/gpxzfvxay.sHtML

echo "log" >> out.log
来源：http://m.share.sjlbkw.cn/Article/details/gcjeazqyw.sHtML

[R41] 丢弃输出
来源：http://www.m.share.tarul.cn/Article/details/gjloqlhws.sHtML

cmd >/dev/null 2>&1
来源：http://blog.epnwcf.com/Article/details/glmmfksyv.sHtML

[R42] 输入重定向
来源：http://www.m.share.tarul.cn/Article/details/gszvscian.sHtML

wc -l < a.txt
来源：http://baike.fktsv.cn/Article/details/gilwpmvqe.sHtML

[R43] 按名字查找文件
来源：http://read.share.epnwcf.com/Article/details/gfdnahyba.sHtML

find . -name "*.log" -type f
来源：http://www.share.vehdjk.com/Article/details/gxzobhaui.sHtML

[R44] 按修改时间查找
来源：http://m.share.tarul.cn/Article/details/ggtqaivlw.sHtML

find . -mtime -7 -type f
来源：http://www.m.share.fktsv.cn/Article/details/gstlvfidb.sHtML

[R45] 批量删除
来源：http://www.share.vehdjk.com/Article/details/gnkpfkuhr.sHtML

find . -name "*.tmp" -delete
来源：http://m.share.epnwcf.com/Article/details/gdkaktexy.sHtML

[R46] 递归替换文件内容
来源：http://mobile.tarul.cn/Article/details/ghwchtlcm.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.m.share.sjlbkw.cn/Article/details/gyxoqpocj.sHtML

[R47] sed 单行替换
来源：http://mobile.vehdjk.com/Article/details/gklmvavxv.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://mobile.yfazqb.com/Article/details/gqzxfrusd.sHtML

[R48] awk 取指定列
来源：http://wap.yfazqb.com/Article/details/gnicrufgr.sHtML

awk '{print $1, $3}' a.txt
来源：http://wap.sjlbkw.cn/Article/details/gyafbbbvi.sHtML

[R49] awk 带条件
来源：http://blog.tarul.cn/Article/details/gtminbdic.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://blog.vehdjk.com/Article/details/gvwigwfqs.sHtML

[R50] awk 求和
来源：http://blog.vehdjk.com/Article/details/ghnbllhqy.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://mobile.fktsv.cn/Article/details/ggxflmotd.sHtML

[R51] 排序去重取前几
来源：http://wap.sjlbkw.cn/Article/details/gthnmikjm.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://blog.tarul.cn/Article/details/gwnsgdmkp.sHtML

[R52] 统计行数
来源：http://mobile.sjlbkw.cn/Article/details/gsrroynio.sHtML

wc -l a.txt
来源：http://blog.bbcook.cn/Article/details/gqiqurxpf.sHtML

[R53] 查看文件头与实时尾
来源：http://blog.epnwcf.com/Article/details/gacvmhmry.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://blog.epnwcf.com/Article/details/grxhjxvck.sHtML

[R54] 比较两个文件
来源：http://www.share.fktsv.cn/Article/details/gukddtylb.sHtML

diff a.txt b.txt
来源：http://3g.fktsv.cn/Article/details/grdfwaxag.sHtML

[R55] 压缩与解压
来源：http://www.m.share.bbcook.cn/Article/details/gaewgakcj.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://blog.tarul.cn/Article/details/gkcsmrdjb.sHtML

[R56] 远程拷贝
来源：http://baike.epnwcf.com/Article/details/gqtlzdgpy.sHtML

scp file user@host:/path/
来源：http://read.share.epnwcf.com/Article/details/gwsozebcj.sHtML

[R57] 远程执行命令
来源：http://wap.bbcook.cn/Article/details/gfbspgkch.sHtML

ssh user@host 'uptime'
来源：http://www.share.fktsv.cn/Article/details/gqksnemov.sHtML

[R58] 下载文件
来源：http://www.blog.fktsv.cn/Article/details/gygtuewtp.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://baike.tarul.cn/Article/details/ggiyskizr.sHtML

[R59] 发 POST JSON
来源：http://www.blog.fktsv.cn/Article/details/gtanmycrm.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.share.fktsv.cn/Article/details/ghrxrropt.sHtML

[R60] 只看 HTTP 状态码
来源：http://mobile.tarul.cn/Article/details/gngbdkyxy.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mobile.tarul.cn/Article/details/ghrwcjpeq.sHtML

[R61] 磁盘占用
来源：http://3g.tarul.cn/Article/details/gmqnlijix.sHtML

df -h;  du -sh *
来源：http://mobile.yfazqb.com/Article/details/gkvnkftxr.sHtML

[R62] 找最占空间的文件
来源：http://3g.epnwcf.com/Article/details/gptfnenya.sHtML

du -ah . | sort -rh | head -10
来源：http://read.share.fktsv.cn/Article/details/gjovboiru.sHtML

[R63] 内存与进程
来源：http://www.share.sjlbkw.cn/Article/details/gwiktcvbt.sHtML

free -h;  ps aux | grep nginx
来源：http://read.share.tarul.cn/Article/details/gkkynnpqt.sHtML

[R64] 结束进程
来源：http://baike.yfazqb.com/Article/details/gytobbahi.sHtML

kill -9 $(pgrep -f app.py)
来源：http://m.share.vehdjk.com/Article/details/gzptbkzcv.sHtML

[R65] 查看端口占用
来源：http://www.share.tarul.cn/Article/details/gapjouxlp.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.blog.epnwcf.com/Article/details/gxxagoanl.sHtML

[R66] 定时任务
来源：http://baike.epnwcf.com/Article/details/gqnkkrgjg.sHtML

crontab -e;  crontab -l
来源：http://3g.yfazqb.com/Article/details/gnixtaovo.sHtML

[R67] 生成随机十六进制串
来源：http://www.blog.sjlbkw.cn/Article/details/gbwmzsdzw.sHtML

openssl rand -hex 16
来源：http://www.share.epnwcf.com/Article/details/geqyrkbmm.sHtML

[R68] 计算文件校验值
来源：http://read.share.yfazqb.com/Article/details/gnzomyhij.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://blog.vehdjk.com/Article/details/gvtiynzgs.sHtML

[R69] 生成随机密码
来源：http://www.m.share.sjlbkw.cn/Article/details/gxfeimhff.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.m.share.bbcook.cn/Article/details/gtjvlvxre.sHtML

[R70] 时间戳与互转
来源：http://www.m.share.sjlbkw.cn/Article/details/gttfgwltt.sHtML

date +%s;  date -d @1700000000
来源：http://read.share.vehdjk.com/Article/details/gbzjxwhub.sHtML

[R71] 日期格式化
来源：http://m.share.yfazqb.com/Article/details/ghgvcugxi.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://blog.sjlbkw.cn/Article/details/gmjiweffc.sHtML

[R72] 等待端口就绪
来源：http://www.m.share.epnwcf.com/Article/details/gbvijbumd.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://blog.fktsv.cn/Article/details/gywkvdunp.sHtML

[R73] 分割大日志
来源：http://3g.yfazqb.com/Article/details/gnqltgoyl.sHtML

split -l 1000 big.log part_
来源：http://www.blog.fktsv.cn/Article/details/gmbzaogow.sHtML

[R74] 批量重命名
来源：http://read.share.bbcook.cn/Article/details/ghtrruanu.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://blog.yfazqb.com/Article/details/gdiqdcqov.sHtML

[R75] 导出环境变量
来源：http://www.m.share.bbcook.cn/Article/details/giinmvvzr.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://m.share.vehdjk.com/Article/details/gjicbxjis.sHtML

[R76] 使用临时文件
来源：http://blog.bbcook.cn/Article/details/gdianlgck.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://m.share.tarul.cn/Article/details/gutmlfczy.sHtML

[R77] 读取用户输入
来源：http://wap.fktsv.cn/Article/details/gjdzvxwus.sHtML

read -rp "请输入: " ans
来源：http://wap.yfazqb.com/Article/details/gppotoidj.sHtML

[R78] 交互式菜单
来源：http://m.share.vehdjk.com/Article/details/gcxunkalw.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://baike.fktsv.cn/Article/details/gcytlmtzf.sHtML

[R79] 解析命令行选项
来源：http://mobile.vehdjk.com/Article/details/gyqmfdqbu.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.m.share.tarul.cn/Article/details/gjqjeinqi.sHtML

[R80] 查看脚本执行耗时
来源：http://m.share.yfazqb.com/Article/details/gtnecqnhi.sHtML

time ./run.sh
来源：http://blog.tarul.cn/Article/details/giavzupto.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/gytshdpag.sHtML

S. C / C++ 专题
来源：http://www.blog.fktsv.cn/Article/details/gbtzzijjj.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/gqkxavfqc.sHtML

[S01] C：Hello World
来源：http://mobile.tarul.cn/Article/details/gxgqchban.sHtML

#include <stdio.h>
来源：http://read.share.epnwcf.com/Article/details/gwbtckgxw.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.share.vehdjk.com/Article/details/gjdcalwwe.sHtML

[S02] C：变量与格式化输出
来源：http://www.blog.vehdjk.com/Article/details/gdoaqooti.sHtML

int a = 10; printf("%d\n", a);
来源：http://mobile.tarul.cn/Article/details/ggluwleug.sHtML

[S03] C：读入整数
来源：http://3g.fktsv.cn/Article/details/gfzehkfpc.sHtML

int x; scanf("%d", &x);
来源：http://www.blog.fktsv.cn/Article/details/gkbtfkzif.sHtML

[S04] C：字符串复制
来源：http://blog.fktsv.cn/Article/details/giubjgweq.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://blog.sjlbkw.cn/Article/details/guajzhcta.sHtML

[S05] C：字符串长度
来源：http://blog.bbcook.cn/Article/details/glkouhihr.sHtML


<!-- 参考信息 -->