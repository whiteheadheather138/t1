代发 wailian999

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.share.vehdjk.com/Article/details/gisaqmvhw.sHtML

) t WHERE rn = 1;
来源：http://blog.fktsv.cn/Article/details/gnzkevkvr.sHtML

[Q35] 内连接
来源：http://3g.epnwcf.com/Article/details/gigxgwgxv.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://wap.bbcook.cn/Article/details/glvgxndan.sHtML

[Q36] 左连接
来源：http://wap.sjlbkw.cn/Article/details/gqcsaywtv.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://read.share.vehdjk.com/Article/details/glecwgdqu.sHtML

[Q37] 右连接
来源：http://www.share.fktsv.cn/Article/details/gduhrhqux.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://m.share.vehdjk.com/Article/details/gcikenazg.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://m.share.bbcook.cn/Article/details/guyqsyaqp.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://blog.sjlbkw.cn/Article/details/gvnjklyza.sHtML

[Q39] 自连接（查上下级）
来源：http://www.blog.vehdjk.com/Article/details/gvrlahumn.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://read.share.bbcook.cn/Article/details/glxcqwswe.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://baike.bbcook.cn/Article/details/gpcxufbcm.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.m.share.tarul.cn/Article/details/guypxtplk.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://blog.bbcook.cn/Article/details/gdzgtjqmp.sHtML

[Q41] 多表连接
来源：http://m.share.fktsv.cn/Article/details/ggxjjdwnr.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://m.share.tarul.cn/Article/details/gmhjuntoi.sHtML

JOIN users u ON u.id = o.user_id
来源：http://3g.epnwcf.com/Article/details/gihlyhvsm.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://blog.sjlbkw.cn/Article/details/ghmbsfuga.sHtML

[Q42] 连接条件附加过滤
来源：http://m.share.sjlbkw.cn/Article/details/gatsvwstl.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.share.yfazqb.com/Article/details/gkoktgdrf.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://mobile.sjlbkw.cn/Article/details/gmnzlblzo.sHtML

[Q43] 标量子查询
来源：http://mobile.sjlbkw.cn/Article/details/gpfpzkzpx.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://mobile.tarul.cn/Article/details/gljggehqt.sHtML

[Q44] IN 子查询
来源：http://m.share.sjlbkw.cn/Article/details/gqfnthsnj.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://mobile.fktsv.cn/Article/details/gdhaykoav.sHtML

[Q45] EXISTS 判断存在
来源：http://read.share.epnwcf.com/Article/details/gtbwzijki.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.tarul.cn/Article/details/gieycedeo.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://read.share.vehdjk.com/Article/details/ghsiqhhvy.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.fktsv.cn/Article/details/gxawwphil.sHtML

[Q47] 与平均值比较
来源：http://mobile.yfazqb.com/Article/details/geerllnbr.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://wap.vehdjk.com/Article/details/grjbeolmt.sHtML

[Q48] CTE 公用表表达式
来源：http://www.blog.fktsv.cn/Article/details/gbwvwtvad.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://wap.tarul.cn/Article/details/golalzlzp.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://read.share.tarul.cn/Article/details/gcopbrapq.sHtML

[Q49] 更新单行
来源：http://blog.sjlbkw.cn/Article/details/gbiuhusil.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.share.yfazqb.com/Article/details/gzpltfujr.sHtML

[Q50] 批量更新
来源：http://wap.fktsv.cn/Article/details/gssmlgcff.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://m.share.sjlbkw.cn/Article/details/gekydmgku.sHtML

[Q51] 用子查询更新
来源：http://www.blog.tarul.cn/Article/details/grklhitdj.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://3g.epnwcf.com/Article/details/gtxlixuuo.sHtML

[Q52] 删除指定行
来源：http://3g.fktsv.cn/Article/details/gecxsduie.sHtML

DELETE FROM users WHERE id = 10;
来源：http://baike.yfazqb.com/Article/details/gjonuvtmj.sHtML

[Q53] 按条件删除
来源：http://blog.yfazqb.com/Article/details/gfmwolqwn.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://3g.yfazqb.com/Article/details/ggehawlhh.sHtML

[Q54] 清空表
来源：http://blog.bbcook.cn/Article/details/gpwglhkui.sHtML

TRUNCATE TABLE logs;
来源：http://blog.bbcook.cn/Article/details/gdvyqdsqe.sHtML

[Q55] 排名（并列占位）
来源：http://read.share.fktsv.cn/Article/details/gdodtzvbp.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.m.share.bbcook.cn/Article/details/ghnwnvthq.sHtML

[Q56] 密集排名（并列不占位）
来源：http://3g.bbcook.cn/Article/details/gyerfnkaz.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.m.share.epnwcf.com/Article/details/gyodjaacf.sHtML

[Q57] 行号
来源：http://www.m.share.yfazqb.com/Article/details/gslzovnnq.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://blog.fktsv.cn/Article/details/gkgjzeotl.sHtML

[Q58] 累计求和
来源：http://mobile.fktsv.cn/Article/details/guccrtpgz.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.share.epnwcf.com/Article/details/gwpzwoiku.sHtML

[Q59] 分组内累计
来源：http://3g.yfazqb.com/Article/details/gmsrwpqfz.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://m.share.bbcook.cn/Article/details/gkhqkiszp.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.blog.bbcook.cn/Article/details/gvoyudlzb.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://baike.tarul.cn/Article/details/gvqlqhumq.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://m.share.bbcook.cn/Article/details/gltyvaiwu.sHtML

[Q61] 移动平均
来源：http://baike.tarul.cn/Article/details/gifcrkwfn.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.m.share.fktsv.cn/Article/details/givkadmgg.sHtML

[Q62] 分组占比
来源：http://m.share.vehdjk.com/Article/details/gmryhnekb.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://3g.tarul.cn/Article/details/gbhczeygz.sHtML

[Q63] 开启事务
来源：http://www.m.share.fktsv.cn/Article/details/gvkqmtdnv.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://wap.bbcook.cn/Article/details/gajejgqjr.sHtML

[Q64] 提交事务
来源：http://baike.sjlbkw.cn/Article/details/gyynanvqi.sHtML

COMMIT;
来源：http://read.share.fktsv.cn/Article/details/gkuyshlxi.sHtML

[Q65] 回滚事务
来源：http://www.share.vehdjk.com/Article/details/guujdlizz.sHtML

ROLLBACK;
来源：http://m.share.epnwcf.com/Article/details/gknfbzsju.sHtML

[Q66] 行锁查询
来源：http://www.share.fktsv.cn/Article/details/gvjknfbid.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.blog.tarul.cn/Article/details/gcvrxszdk.sHtML

[Q67] 设置隔离级别
来源：http://wap.yfazqb.com/Article/details/gtvzhpylf.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://m.share.fktsv.cn/Article/details/gnwgtumfd.sHtML

[Q68] 保存点
来源：http://www.share.vehdjk.com/Article/details/gctmptini.sHtML

SAVEPOINT sp1;
来源：http://m.share.tarul.cn/Article/details/grttlhpvr.sHtML

ROLLBACK TO sp1;
来源：http://read.share.bbcook.cn/Article/details/gczkcyngt.sHtML

[Q69] 查看执行计划
来源：http://wap.yfazqb.com/Article/details/gesfitqvs.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://blog.bbcook.cn/Article/details/ginmfmfci.sHtML

[Q70] 更新统计信息
来源：http://www.share.yfazqb.com/Article/details/gedncnfol.sHtML

ANALYZE TABLE users;
来源：http://3g.vehdjk.com/Article/details/gwbzmbcwi.sHtML

[Q71] 查看建表语句
来源：http://www.m.share.sjlbkw.cn/Article/details/guspdhnsz.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://wap.epnwcf.com/Article/details/gwwwictxn.sHtML

[Q72] 查看索引
来源：http://wap.epnwcf.com/Article/details/gawhraaeb.sHtML

SHOW INDEX FROM users;
来源：http://www.share.vehdjk.com/Article/details/gfycjqvuu.sHtML

[Q73] 查看表状态
来源：http://mobile.bbcook.cn/Article/details/gdrtjqpmy.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://blog.sjlbkw.cn/Article/details/giytdjpkg.sHtML

[Q74] 强制使用索引
来源：http://www.share.bbcook.cn/Article/details/gvrhxakky.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://baike.yfazqb.com/Article/details/gtwfazvga.sHtML

[Q75] 日期格式化
来源：http://baike.epnwcf.com/Article/details/gmseolfeb.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.share.tarul.cn/Article/details/guxaunzbk.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://wap.vehdjk.com/Article/details/gtezymwme.sHtML

[Q76] 按天统计
来源：http://blog.tarul.cn/Article/details/gntsnsfdk.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://read.share.vehdjk.com/Article/details/gbmopydkd.sHtML

[Q77] 时间加减
来源：http://m.share.epnwcf.com/Article/details/gvneakkyc.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.m.share.fktsv.cn/Article/details/gnomjxrhq.sHtML

[Q78] 当前时间
来源：http://mobile.vehdjk.com/Article/details/gqcpjzqzk.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://blog.fktsv.cn/Article/details/gxemgmvit.sHtML

[Q79] 字符串拼接
来源：http://read.share.fktsv.cn/Article/details/gelaqrzye.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://read.share.fktsv.cn/Article/details/gzqaspusf.sHtML

[Q80] 字符串截取
来源：http://3g.vehdjk.com/Article/details/gpdhxfhed.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.share.bbcook.cn/Article/details/gqlprfroh.sHtML

[Q81] 字符串替换
来源：http://www.blog.vehdjk.com/Article/details/gihduincc.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.m.share.sjlbkw.cn/Article/details/gxuxasjfh.sHtML

[Q82] 字符长度与字节长度
来源：http://m.share.sjlbkw.cn/Article/details/gsnkpfrfn.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://m.share.fktsv.cn/Article/details/gfwjfxcvs.sHtML

[Q83] 大小写转换
来源：http://mobile.yfazqb.com/Article/details/gflrpqkyj.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.blog.vehdjk.com/Article/details/giagdyiuh.sHtML

[Q84] 去除首尾空格
来源：http://read.share.vehdjk.com/Article/details/gvjtmmtdv.sHtML

SELECT TRIM(name) FROM users;
来源：http://wap.tarul.cn/Article/details/gxvhlqvov.sHtML

[Q85] 数值取整
来源：http://www.share.epnwcf.com/Article/details/gllouhnau.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://3g.bbcook.cn/Article/details/gisfvqpig.sHtML

[Q86] 读取 JSON 字段
来源：http://www.share.vehdjk.com/Article/details/gvihobbzr.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://read.share.epnwcf.com/Article/details/gpgzrczrp.sHtML

[Q87] JSON 字段做条件
来源：http://www.m.share.vehdjk.com/Article/details/glxrhbggo.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://blog.vehdjk.com/Article/details/gozlbxofl.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.share.sjlbkw.cn/Article/details/gbthhiavt.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://wap.sjlbkw.cn/Article/details/gezeyzzvs.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://read.share.yfazqb.com/Article/details/geelzixfv.sHtML

[Q89] 判断表是否存在
来源：http://wap.bbcook.cn/Article/details/gkqbsgosr.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.m.share.yfazqb.com/Article/details/ghjmuefsj.sHtML

[Q90] 生成序号列
来源：http://m.share.tarul.cn/Article/details/gxkwbjres.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://mobile.epnwcf.com/Article/details/ggemtfhuq.sHtML

================================================================================
来源：http://mobile.epnwcf.com/Article/details/gprvcooav.sHtML

R. Bash 专题
来源：http://read.share.vehdjk.com/Article/details/gnzrvchnj.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/gxcssznfz.sHtML

[R01] shebang 与严格模式
来源：http://3g.yfazqb.com/Article/details/gbhwbhjkt.sHtML

#!/usr/bin/env bash
来源：http://baike.epnwcf.com/Article/details/gtrolghof.sHtML

set -euo pipefail
来源：http://m.share.yfazqb.com/Article/details/guevipbyi.sHtML

[R02] 变量赋值与使用
来源：http://www.share.fktsv.cn/Article/details/gickxirqz.sHtML

name="Tom"; echo "$name"
来源：http://www.blog.tarul.cn/Article/details/gjyvsfpvk.sHtML

[R03] 只读变量
来源：http://read.share.sjlbkw.cn/Article/details/gaukysyta.sHtML

readonly PI=3.14
来源：http://m.share.fktsv.cn/Article/details/gnkopxyno.sHtML

[R04] 位置参数
来源：http://www.m.share.yfazqb.com/Article/details/gkacygjcg.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://wap.bbcook.cn/Article/details/gcfxpeved.sHtML

[R05] 参数默认值
来源：http://baike.fktsv.cn/Article/details/girxynnrj.sHtML

name="${1:-default}"
来源：http://www.blog.fktsv.cn/Article/details/gtzoacmig.sHtML

[R06] 判断命令是否存在
来源：http://www.m.share.epnwcf.com/Article/details/gsfwnznce.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://blog.fktsv.cn/Article/details/gpnfahbgx.sHtML

[R07] if 判断文件
来源：http://www.share.bbcook.cn/Article/details/gizzzmyix.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://read.share.vehdjk.com/Article/details/gyrpetpga.sHtML

[R08] 数值比较
来源：http://blog.yfazqb.com/Article/details/gvuflgiaf.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://m.share.vehdjk.com/Article/details/gxjdcjiek.sHtML

[R09] 字符串比较
来源：http://wap.yfazqb.com/Article/details/geavnggex.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://wap.epnwcf.com/Article/details/gzwqlwenn.sHtML

[R10] 正则匹配
来源：http://wap.fktsv.cn/Article/details/gxsozgaqo.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://blog.yfazqb.com/Article/details/gtusqdfzc.sHtML

[R11] case 多分支
来源：http://www.m.share.yfazqb.com/Article/details/gdooazbev.sHtML

case "$1" in
来源：http://www.share.vehdjk.com/Article/details/goametrdg.sHtML

start) echo "启动" ;;
来源：http://www.blog.fktsv.cn/Article/details/gjzvrvlam.sHtML

stop)  echo "停止" ;;
来源：http://m.share.fktsv.cn/Article/details/goqmtakfr.sHtML

*)     echo "未知命令" ;;
来源：http://www.m.share.yfazqb.com/Article/details/gndjnwkrn.sHtML

esac
来源：http://baike.epnwcf.com/Article/details/gdkyynxli.sHtML

[R12] for 遍历文件
来源：http://www.blog.tarul.cn/Article/details/gjonmzknk.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.m.share.yfazqb.com/Article/details/gddehnedv.sHtML

[R13] for 计数循环
来源：http://mobile.sjlbkw.cn/Article/details/gihktuocu.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://read.share.epnwcf.com/Article/details/goqkunzia.sHtML

[R14] C 风格 for
来源：http://wap.bbcook.cn/Article/details/gthsdhgro.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.m.share.yfazqb.com/Article/details/gulcfazdw.sHtML

[R15] while 逐行读文件
来源：http://m.share.vehdjk.com/Article/details/gswifrryg.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://wap.yfazqb.com/Article/details/gusxvdeur.sHtML

[R16] until 等待条件
来源：http://mobile.yfazqb.com/Article/details/gojkmxzfx.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.m.share.yfazqb.com/Article/details/grmmkvrsm.sHtML

[R17] 数组定义与取值
来源：http://3g.bbcook.cn/Article/details/gpejqwvcz.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://read.share.sjlbkw.cn/Article/details/gvenccnbf.sHtML

[R18] 遍历数组
来源：http://read.share.yfazqb.com/Article/details/gemwhhnbn.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://mobile.fktsv.cn/Article/details/gfglkcxnq.sHtML

[R19] 数组长度
来源：http://www.share.yfazqb.com/Article/details/gbjgrayhk.sHtML

echo "${#arr[@]}"
来源：http://www.share.vehdjk.com/Article/details/gvxglifjp.sHtML

[R20] 关联数组（字典）
来源：http://baike.epnwcf.com/Article/details/guwykllct.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.share.bbcook.cn/Article/details/gxnplynck.sHtML

[R21] 字符串长度
来源：http://wap.vehdjk.com/Article/details/gunkhhudg.sHtML

echo "${#s}"
来源：http://blog.tarul.cn/Article/details/guyggasxn.sHtML

[R22] 截取子串
来源：http://www.share.vehdjk.com/Article/details/gxgigcwfn.sHtML

echo "${s:0:5}"
来源：http://www.m.share.yfazqb.com/Article/details/gvlxqqtoo.sHtML

[R23] 字符串替换
来源：http://wap.yfazqb.com/Article/details/gqopvtkuq.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.blog.epnwcf.com/Article/details/glmsluqne.sHtML

[R24] 大小写转换
来源：http://read.share.fktsv.cn/Article/details/gcouyymme.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.share.vehdjk.com/Article/details/gbnzqqkmd.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.blog.sjlbkw.cn/Article/details/giagngaeo.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.blog.bbcook.cn/Article/details/gvfebifbp.sHtML

[R26] 命令替换
来源：http://www.m.share.bbcook.cn/Article/details/gokudrxgk.sHtML

now=$(date +%F); echo "$now"
来源：http://www.m.share.yfazqb.com/Article/details/gufkvxudf.sHtML

[R27] 算术展开
来源：http://3g.sjlbkw.cn/Article/details/gkaewcfwh.sHtML

echo $((1 + 2 * 3))
来源：http://3g.sjlbkw.cn/Article/details/gdobewqln.sHtML

[R28] 浮点运算
来源：http://baike.sjlbkw.cn/Article/details/gmsbbzuqe.sHtML

echo "scale=2; 10/3" | bc
来源：http://3g.vehdjk.com/Article/details/gwemxbvve.sHtML

[R29] 定义函数
来源：http://3g.yfazqb.com/Article/details/ggcxucxnk.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.share.bbcook.cn/Article/details/gzsyqygxg.sHtML

[R30] 函数返回状态码
来源：http://wap.bbcook.cn/Article/details/guoqslmxv.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://m.share.sjlbkw.cn/Article/details/gkmmijgdn.sHtML

[R31] 局部变量
来源：http://mobile.fktsv.cn/Article/details/girgcjvdm.sHtML

f() { local x=1; echo "$x"; }
来源：http://baike.sjlbkw.cn/Article/details/gvlnzalzn.sHtML

[R32] 参数个数校验
来源：http://read.share.epnwcf.com/Article/details/gjvcrqcde.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://blog.vehdjk.com/Article/details/gaedtzvix.sHtML

[R33] 捕获错误并提示行号
来源：http://wap.bbcook.cn/Article/details/gkhsomkxu.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://blog.vehdjk.com/Article/details/gdrtsxlxy.sHtML

[R34] 退出时清理
来源：http://blog.epnwcf.com/Article/details/goqergklh.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://3g.bbcook.cn/Article/details/gipvzbmtd.sHtML

[R35] 后台执行并等待
来源：http://blog.fktsv.cn/Article/details/gpklryvys.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://mobile.sjlbkw.cn/Article/details/gfmcglfro.sHtML

[R36] 并发执行多个任务
来源：http://www.m.share.epnwcf.com/Article/details/gajaytmnl.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://read.share.yfazqb.com/Article/details/gywepwcgt.sHtML

[R37] 把输出赋给变量
来源：http://wap.epnwcf.com/Article/details/gihyhgidc.sHtML

files=$(ls -1)
来源：http://3g.bbcook.cn/Article/details/gsnjzwtyk.sHtML

[R38] 管道串联
来源：http://mobile.yfazqb.com/Article/details/geplvwfid.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.m.share.sjlbkw.cn/Article/details/gwimzruty.sHtML

[R39] 重定向标准输出与错误
来源：http://blog.sjlbkw.cn/Article/details/gmcfoufjc.sHtML

cmd > out.log 2>&1
来源：http://baike.bbcook.cn/Article/details/gvirowhdl.sHtML

[R40] 追加写日志
来源：http://www.blog.fktsv.cn/Article/details/ghiawwojv.sHtML

echo "log" >> out.log
来源：http://3g.epnwcf.com/Article/details/gtmniqynm.sHtML

[R41] 丢弃输出
来源：http://blog.vehdjk.com/Article/details/ghocjrgpx.sHtML

cmd >/dev/null 2>&1
来源：http://baike.tarul.cn/Article/details/gfipdsjdg.sHtML

[R42] 输入重定向
来源：http://3g.fktsv.cn/Article/details/gekryukmq.sHtML

wc -l < a.txt
来源：http://www.blog.yfazqb.com/Article/details/gacayafrl.sHtML

[R43] 按名字查找文件
来源：http://www.m.share.epnwcf.com/Article/details/gucsosijp.sHtML

find . -name "*.log" -type f
来源：http://www.m.share.sjlbkw.cn/Article/details/gzskkyzoc.sHtML

[R44] 按修改时间查找
来源：http://www.m.share.epnwcf.com/Article/details/gcwahfpdl.sHtML

find . -mtime -7 -type f
来源：http://3g.vehdjk.com/Article/details/gybrmxuzc.sHtML

[R45] 批量删除
来源：http://www.blog.bbcook.cn/Article/details/gdsizbxvw.sHtML

find . -name "*.tmp" -delete
来源：http://www.share.vehdjk.com/Article/details/gutbngdlg.sHtML

[R46] 递归替换文件内容
来源：http://baike.bbcook.cn/Article/details/gwvfwrsar.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://baike.bbcook.cn/Article/details/glhbtsiwf.sHtML

[R47] sed 单行替换
来源：http://mobile.bbcook.cn/Article/details/ggxjhlgbp.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.blog.epnwcf.com/Article/details/gmlwvtrzt.sHtML

[R48] awk 取指定列
来源：http://www.m.share.epnwcf.com/Article/details/gtdseglsj.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.share.sjlbkw.cn/Article/details/gpioqbava.sHtML

[R49] awk 带条件
来源：http://blog.yfazqb.com/Article/details/gsyqkbvoc.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.m.share.bbcook.cn/Article/details/gicqsiwfi.sHtML

[R50] awk 求和
来源：http://baike.epnwcf.com/Article/details/gwvfkiuzt.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://blog.tarul.cn/Article/details/gylggeihk.sHtML

[R51] 排序去重取前几
来源：http://read.share.tarul.cn/Article/details/gibjbhwyp.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.m.share.sjlbkw.cn/Article/details/ggbqlmsqu.sHtML

[R52] 统计行数
来源：http://3g.vehdjk.com/Article/details/goidntnjv.sHtML

wc -l a.txt
来源：http://www.share.sjlbkw.cn/Article/details/giszfhogx.sHtML

[R53] 查看文件头与实时尾
来源：http://3g.fktsv.cn/Article/details/gqkfazijc.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.m.share.yfazqb.com/Article/details/gfkigbmhj.sHtML

[R54] 比较两个文件
来源：http://m.share.yfazqb.com/Article/details/gqvwvbpim.sHtML

diff a.txt b.txt
来源：http://baike.vehdjk.com/Article/details/gtxedaynk.sHtML

[R55] 压缩与解压
来源：http://www.blog.tarul.cn/Article/details/ghisrwaav.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://baike.sjlbkw.cn/Article/details/gxucovpgl.sHtML

[R56] 远程拷贝
来源：http://baike.tarul.cn/Article/details/gekznaejs.sHtML

scp file user@host:/path/
来源：http://www.m.share.fktsv.cn/Article/details/gmrrzebmn.sHtML

[R57] 远程执行命令
来源：http://wap.yfazqb.com/Article/details/gxkwtwszt.sHtML

ssh user@host 'uptime'
来源：http://3g.bbcook.cn/Article/details/gimmvugkz.sHtML

[R58] 下载文件
来源：http://baike.tarul.cn/Article/details/glgarplmz.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://3g.sjlbkw.cn/Article/details/gkbwsxtbo.sHtML

[R59] 发 POST JSON
来源：http://3g.tarul.cn/Article/details/gwaayhlhz.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.m.share.fktsv.cn/Article/details/gsuswyusj.sHtML

[R60] 只看 HTTP 状态码
来源：http://3g.bbcook.cn/Article/details/glclmbupp.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://blog.vehdjk.com/Article/details/giczqwwxd.sHtML

[R61] 磁盘占用
来源：http://www.share.tarul.cn/Article/details/glnmohnrq.sHtML

df -h;  du -sh *
来源：http://read.share.bbcook.cn/Article/details/gzuqvajeb.sHtML

[R62] 找最占空间的文件
来源：http://blog.fktsv.cn/Article/details/gxbqtkdyh.sHtML

du -ah . | sort -rh | head -10
来源：http://m.share.fktsv.cn/Article/details/gaiqswqgl.sHtML

[R63] 内存与进程
来源：http://m.share.fktsv.cn/Article/details/gztcvblvm.sHtML

free -h;  ps aux | grep nginx
来源：http://mobile.yfazqb.com/Article/details/gjtxxsauh.sHtML

[R64] 结束进程
来源：http://www.m.share.fktsv.cn/Article/details/gvcbxkubm.sHtML

kill -9 $(pgrep -f app.py)
来源：http://baike.sjlbkw.cn/Article/details/gpwyvhulj.sHtML

[R65] 查看端口占用
来源：http://read.share.vehdjk.com/Article/details/gkgyhdckb.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://baike.fktsv.cn/Article/details/gcmrnqluu.sHtML

[R66] 定时任务
来源：http://blog.fktsv.cn/Article/details/gtobmncfk.sHtML

crontab -e;  crontab -l
来源：http://blog.epnwcf.com/Article/details/geivxdfar.sHtML

[R67] 生成随机十六进制串
来源：http://mobile.vehdjk.com/Article/details/ghzsjnnjz.sHtML

openssl rand -hex 16
来源：http://mobile.vehdjk.com/Article/details/gbjppkrua.sHtML

[R68] 计算文件校验值
来源：http://wap.bbcook.cn/Article/details/gcscnwuce.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://wap.fktsv.cn/Article/details/gqgdbnckx.sHtML

[R69] 生成随机密码
来源：http://www.blog.bbcook.cn/Article/details/gzwtwbuul.sHtML

head -c 16 /dev/urandom | base64
来源：http://wap.epnwcf.com/Article/details/gfbfipauw.sHtML

[R70] 时间戳与互转
来源：http://www.m.share.vehdjk.com/Article/details/gptqmjtzo.sHtML

date +%s;  date -d @1700000000
来源：http://www.blog.epnwcf.com/Article/details/gynsroomf.sHtML

[R71] 日期格式化
来源：http://wap.sjlbkw.cn/Article/details/gotqwqxbv.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://mobile.yfazqb.com/Article/details/gxsfppmqk.sHtML

[R72] 等待端口就绪
来源：http://wap.fktsv.cn/Article/details/gzcnonjzz.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://baike.bbcook.cn/Article/details/gwsvqzvcf.sHtML

[R73] 分割大日志
来源：http://baike.bbcook.cn/Article/details/gugmmbqzr.sHtML

split -l 1000 big.log part_
来源：http://wap.sjlbkw.cn/Article/details/gcfhnougi.sHtML

[R74] 批量重命名
来源：http://read.share.vehdjk.com/Article/details/gkxcikspv.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.m.share.fktsv.cn/Article/details/gluzatylz.sHtML

[R75] 导出环境变量
来源：http://www.m.share.bbcook.cn/Article/details/ganbxrqxr.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://read.share.tarul.cn/Article/details/gcybzsayi.sHtML

[R76] 使用临时文件
来源：http://m.share.epnwcf.com/Article/details/gicmhqoei.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://wap.tarul.cn/Article/details/gkjlvszxy.sHtML

[R77] 读取用户输入
来源：http://3g.vehdjk.com/Article/details/gveezdvaw.sHtML

read -rp "请输入: " ans
来源：http://www.share.bbcook.cn/Article/details/gsqpqsmlt.sHtML

[R78] 交互式菜单
来源：http://blog.vehdjk.com/Article/details/gvkpdwivj.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://mobile.bbcook.cn/Article/details/gopcevakv.sHtML

[R79] 解析命令行选项
来源：http://wap.tarul.cn/Article/details/gkehlgktb.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://baike.bbcook.cn/Article/details/gspistvfa.sHtML

[R80] 查看脚本执行耗时
来源：http://www.blog.yfazqb.com/Article/details/gmceuknwd.sHtML

time ./run.sh
来源：http://www.share.yfazqb.com/Article/details/gaxoaksrk.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/gadydwxta.sHtML

S. C / C++ 专题
来源：http://www.m.share.fktsv.cn/Article/details/gpkmnbpqm.sHtML

================================================================================
来源：http://mobile.epnwcf.com/Article/details/gpjgfovje.sHtML

[S01] C：Hello World
来源：http://baike.sjlbkw.cn/Article/details/gjhqpqmng.sHtML

#include <stdio.h>
来源：http://baike.epnwcf.com/Article/details/gwtejrraf.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://3g.vehdjk.com/Article/details/gntxbexft.sHtML

[S02] C：变量与格式化输出
来源：http://www.m.share.fktsv.cn/Article/details/gszebjvja.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.share.fktsv.cn/Article/details/gsxfznmuv.sHtML

[S03] C：读入整数
来源：http://www.blog.epnwcf.com/Article/details/gwtwatapt.sHtML


<!-- 参考信息 -->