代发 wailian999

SELECT MAX(age), MIN(age) FROM users;
来源：http://mobile.bbcook.cn/Article/details/glhwtdjbq.sHtML

[Q30] 分组统计
来源：http://baike.sjlbkw.cn/Article/details/gnthmzibc.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://read.share.epnwcf.com/Article/details/gtewvpjsg.sHtML

[Q31] 分组后过滤
来源：http://mobile.vehdjk.com/Article/details/gxitsnrug.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://baike.epnwcf.com/Article/details/gfmzomssr.sHtML

[Q32] 分组拼接字符串
来源：http://www.blog.epnwcf.com/Article/details/gttfsphup.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://baike.yfazqb.com/Article/details/ghgzanpvq.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.blog.fktsv.cn/Article/details/gkpuycgqj.sHtML

[Q33] 多列分组
来源：http://www.m.share.yfazqb.com/Article/details/gxaghwfpm.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://3g.bbcook.cn/Article/details/gdkxpocjg.sHtML

[Q34] 每组取第一条
来源：http://baike.yfazqb.com/Article/details/gmooloour.sHtML

SELECT * FROM (
来源：http://wap.sjlbkw.cn/Article/details/grkokdomq.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://blog.fktsv.cn/Article/details/gowgarxxn.sHtML

) t WHERE rn = 1;
来源：http://m.share.bbcook.cn/Article/details/gkerxzgtc.sHtML

[Q35] 内连接
来源：http://blog.bbcook.cn/Article/details/grdqdqupz.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.share.yfazqb.com/Article/details/gligeqwfw.sHtML

[Q36] 左连接
来源：http://www.share.sjlbkw.cn/Article/details/gwdwjuats.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.vehdjk.com/Article/details/grsmehcom.sHtML

[Q37] 右连接
来源：http://read.share.epnwcf.com/Article/details/gilflgwpi.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://baike.tarul.cn/Article/details/ghuqvdqnm.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://wap.yfazqb.com/Article/details/gihrhtmgx.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://read.share.sjlbkw.cn/Article/details/gxrqgcnjj.sHtML

[Q39] 自连接（查上下级）
来源：http://mobile.tarul.cn/Article/details/gquwvhquc.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.m.share.vehdjk.com/Article/details/gosjmecbk.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://read.share.bbcook.cn/Article/details/gqlxcgtnx.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://m.share.vehdjk.com/Article/details/gblwwtizz.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.m.share.sjlbkw.cn/Article/details/golazfoyt.sHtML

[Q41] 多表连接
来源：http://baike.yfazqb.com/Article/details/gqjmuiwjm.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://m.share.epnwcf.com/Article/details/geytxlkrp.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.m.share.tarul.cn/Article/details/gfdqwowum.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.m.share.fktsv.cn/Article/details/guwwhezoe.sHtML

[Q42] 连接条件附加过滤
来源：http://baike.vehdjk.com/Article/details/glzylljbu.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.share.tarul.cn/Article/details/gklcycsqc.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.m.share.epnwcf.com/Article/details/gqsbxxuew.sHtML

[Q43] 标量子查询
来源：http://www.m.share.yfazqb.com/Article/details/gyikczcij.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://3g.bbcook.cn/Article/details/gtlqefair.sHtML

[Q44] IN 子查询
来源：http://www.share.tarul.cn/Article/details/gqvtkhupb.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://3g.vehdjk.com/Article/details/gfrjhzsde.sHtML

[Q45] EXISTS 判断存在
来源：http://blog.yfazqb.com/Article/details/gubxogbrd.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.vehdjk.com/Article/details/gqzjibtkn.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://m.share.epnwcf.com/Article/details/gpqjbpakc.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.yfazqb.com/Article/details/gjugeibfs.sHtML

[Q47] 与平均值比较
来源：http://baike.vehdjk.com/Article/details/gmnjebabo.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://wap.vehdjk.com/Article/details/gzshoerbi.sHtML

[Q48] CTE 公用表表达式
来源：http://www.share.vehdjk.com/Article/details/gkmqiaqrx.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://wap.sjlbkw.cn/Article/details/gyborhedl.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://m.share.bbcook.cn/Article/details/gcgevovmh.sHtML

[Q49] 更新单行
来源：http://baike.bbcook.cn/Article/details/gefhhovxx.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://m.share.vehdjk.com/Article/details/gshkejtur.sHtML

[Q50] 批量更新
来源：http://www.m.share.epnwcf.com/Article/details/gpbfsuhea.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.share.tarul.cn/Article/details/gpddknuxe.sHtML

[Q51] 用子查询更新
来源：http://www.share.bbcook.cn/Article/details/gvzmjdbwe.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://3g.fktsv.cn/Article/details/gzjiwdeeu.sHtML

[Q52] 删除指定行
来源：http://read.share.vehdjk.com/Article/details/gxvbafeej.sHtML

DELETE FROM users WHERE id = 10;
来源：http://blog.tarul.cn/Article/details/gujrkuajx.sHtML

[Q53] 按条件删除
来源：http://mobile.yfazqb.com/Article/details/gcmvcwguj.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://wap.epnwcf.com/Article/details/gyeiokvnu.sHtML

[Q54] 清空表
来源：http://wap.epnwcf.com/Article/details/gmyikuaxr.sHtML

TRUNCATE TABLE logs;
来源：http://blog.bbcook.cn/Article/details/ghhuuzpsh.sHtML

[Q55] 排名（并列占位）
来源：http://m.share.epnwcf.com/Article/details/ghrsqjozz.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://baike.bbcook.cn/Article/details/grljljluz.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.m.share.yfazqb.com/Article/details/gwdqevnmv.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.m.share.tarul.cn/Article/details/gegrmjdkc.sHtML

[Q57] 行号
来源：http://www.m.share.fktsv.cn/Article/details/gylrpxgth.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.share.epnwcf.com/Article/details/gvnygkvst.sHtML

[Q58] 累计求和
来源：http://m.share.yfazqb.com/Article/details/gcwrwkdto.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://m.share.yfazqb.com/Article/details/gnermcnvw.sHtML

[Q59] 分组内累计
来源：http://mobile.vehdjk.com/Article/details/gfkcqudgv.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.blog.yfazqb.com/Article/details/grmuxvdux.sHtML

[Q60] 取上一行 / 下一行
来源：http://baike.yfazqb.com/Article/details/gzuuyemvo.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.blog.vehdjk.com/Article/details/gsgzrkhaf.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://3g.tarul.cn/Article/details/gjtkgnbdj.sHtML

[Q61] 移动平均
来源：http://m.share.tarul.cn/Article/details/gbsmexgfa.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.m.share.sjlbkw.cn/Article/details/gwozodqvi.sHtML

[Q62] 分组占比
来源：http://mobile.sjlbkw.cn/Article/details/gjkinshmb.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://m.share.tarul.cn/Article/details/gkvtcdnxw.sHtML

[Q63] 开启事务
来源：http://3g.bbcook.cn/Article/details/geuxsyhpo.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://3g.sjlbkw.cn/Article/details/gefvhqrfq.sHtML

[Q64] 提交事务
来源：http://blog.epnwcf.com/Article/details/gsblmkzxx.sHtML

COMMIT;
来源：http://www.m.share.vehdjk.com/Article/details/gpjzrywch.sHtML

[Q65] 回滚事务
来源：http://www.share.sjlbkw.cn/Article/details/gjzaloiuu.sHtML

ROLLBACK;
来源：http://m.share.vehdjk.com/Article/details/gmqclmtrg.sHtML

[Q66] 行锁查询
来源：http://3g.yfazqb.com/Article/details/grxnytgzs.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://m.share.sjlbkw.cn/Article/details/gmbbzprnp.sHtML

[Q67] 设置隔离级别
来源：http://blog.vehdjk.com/Article/details/gipcgejsw.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://wap.bbcook.cn/Article/details/gqhlgkxgp.sHtML

[Q68] 保存点
来源：http://3g.bbcook.cn/Article/details/gsmjuuntm.sHtML

SAVEPOINT sp1;
来源：http://www.share.tarul.cn/Article/details/gqzzpafka.sHtML

ROLLBACK TO sp1;
来源：http://wap.epnwcf.com/Article/details/gffoiodzv.sHtML

[Q69] 查看执行计划
来源：http://www.m.share.yfazqb.com/Article/details/gybhceoat.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.share.epnwcf.com/Article/details/gfksdfsey.sHtML

[Q70] 更新统计信息
来源：http://wap.vehdjk.com/Article/details/gouuyzyam.sHtML

ANALYZE TABLE users;
来源：http://www.m.share.sjlbkw.cn/Article/details/gykfupepm.sHtML

[Q71] 查看建表语句
来源：http://blog.epnwcf.com/Article/details/gvjqklrfs.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.blog.vehdjk.com/Article/details/gozqymqyh.sHtML

[Q72] 查看索引
来源：http://wap.fktsv.cn/Article/details/gweqysxzw.sHtML

SHOW INDEX FROM users;
来源：http://read.share.fktsv.cn/Article/details/gxssevhuy.sHtML

[Q73] 查看表状态
来源：http://wap.sjlbkw.cn/Article/details/gsqipxvyn.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://wap.fktsv.cn/Article/details/ghwshvypo.sHtML

[Q74] 强制使用索引
来源：http://blog.yfazqb.com/Article/details/gwufsfoxv.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://wap.sjlbkw.cn/Article/details/gquczutzr.sHtML

[Q75] 日期格式化
来源：http://www.share.fktsv.cn/Article/details/gvbbbskdp.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://3g.epnwcf.com/Article/details/gewpsnmyb.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.share.vehdjk.com/Article/details/gnxnmgcjr.sHtML

[Q76] 按天统计
来源：http://baike.sjlbkw.cn/Article/details/gstyvotex.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://wap.vehdjk.com/Article/details/ghwmbwmhr.sHtML

[Q77] 时间加减
来源：http://www.m.share.epnwcf.com/Article/details/gmtpusgpx.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://mobile.vehdjk.com/Article/details/glyomyohi.sHtML

[Q78] 当前时间
来源：http://baike.bbcook.cn/Article/details/gnnsfjddd.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://wap.vehdjk.com/Article/details/getnotstc.sHtML

[Q79] 字符串拼接
来源：http://baike.vehdjk.com/Article/details/gwatkuvyv.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://baike.bbcook.cn/Article/details/gdbqimmmw.sHtML

[Q80] 字符串截取
来源：http://wap.sjlbkw.cn/Article/details/glgyncqkk.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://m.share.vehdjk.com/Article/details/gfbrmouwn.sHtML

[Q81] 字符串替换
来源：http://m.share.tarul.cn/Article/details/gxbjhhkbj.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://m.share.yfazqb.com/Article/details/gmmhrxgyi.sHtML

[Q82] 字符长度与字节长度
来源：http://www.blog.tarul.cn/Article/details/gavyshkns.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://wap.yfazqb.com/Article/details/guafutasl.sHtML

[Q83] 大小写转换
来源：http://wap.bbcook.cn/Article/details/gavmldfbx.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://m.share.tarul.cn/Article/details/gzwrdbdio.sHtML

[Q84] 去除首尾空格
来源：http://m.share.yfazqb.com/Article/details/gxleyuyem.sHtML

SELECT TRIM(name) FROM users;
来源：http://mobile.bbcook.cn/Article/details/gurzeekvo.sHtML

[Q85] 数值取整
来源：http://www.m.share.yfazqb.com/Article/details/gqiapvqgg.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://baike.vehdjk.com/Article/details/gseqymkwo.sHtML

[Q86] 读取 JSON 字段
来源：http://wap.yfazqb.com/Article/details/gmceymhql.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://3g.yfazqb.com/Article/details/gwtvqgfeb.sHtML

[Q87] JSON 字段做条件
来源：http://mobile.epnwcf.com/Article/details/gcglxtzof.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.share.fktsv.cn/Article/details/gzomppxmy.sHtML

[Q88] 行转列（条件聚合）
来源：http://baike.yfazqb.com/Article/details/ggackotie.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://3g.tarul.cn/Article/details/gfkjrhfhp.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.share.bbcook.cn/Article/details/gtizcmxoi.sHtML

[Q89] 判断表是否存在
来源：http://wap.epnwcf.com/Article/details/gmpdcmrsx.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://blog.epnwcf.com/Article/details/gyhwgaozt.sHtML

[Q90] 生成序号列
来源：http://www.blog.bbcook.cn/Article/details/gtbvemmhc.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.m.share.tarul.cn/Article/details/gotlacord.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/gvpldtkoh.sHtML

R. Bash 专题
来源：http://wap.tarul.cn/Article/details/gxetttsbd.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/glqytrljx.sHtML

[R01] shebang 与严格模式
来源：http://baike.tarul.cn/Article/details/gfjndpazt.sHtML

#!/usr/bin/env bash
来源：http://blog.bbcook.cn/Article/details/gixvlkkjg.sHtML

set -euo pipefail
来源：http://3g.tarul.cn/Article/details/gtxzvechx.sHtML

[R02] 变量赋值与使用
来源：http://read.share.tarul.cn/Article/details/gddbatezx.sHtML

name="Tom"; echo "$name"
来源：http://www.blog.sjlbkw.cn/Article/details/ghticrghb.sHtML

[R03] 只读变量
来源：http://3g.epnwcf.com/Article/details/gtvjwynoh.sHtML

readonly PI=3.14
来源：http://3g.fktsv.cn/Article/details/gpjixrcsk.sHtML

[R04] 位置参数
来源：http://www.blog.fktsv.cn/Article/details/gnyqssqdw.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.share.vehdjk.com/Article/details/gvwerysmb.sHtML

[R05] 参数默认值
来源：http://m.share.bbcook.cn/Article/details/googfssca.sHtML

name="${1:-default}"
来源：http://m.share.bbcook.cn/Article/details/gnxpiszox.sHtML

[R06] 判断命令是否存在
来源：http://www.blog.yfazqb.com/Article/details/gslhrlles.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://3g.yfazqb.com/Article/details/gghgvwkxw.sHtML

[R07] if 判断文件
来源：http://www.blog.tarul.cn/Article/details/gnjcyivjv.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://blog.tarul.cn/Article/details/gdqscaypo.sHtML

[R08] 数值比较
来源：http://www.share.vehdjk.com/Article/details/gdguzpzui.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://read.share.vehdjk.com/Article/details/ggiqggxdt.sHtML

[R09] 字符串比较
来源：http://blog.fktsv.cn/Article/details/gcvqnuvxo.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://m.share.fktsv.cn/Article/details/gnnuypbjc.sHtML

[R10] 正则匹配
来源：http://mobile.bbcook.cn/Article/details/gryvhzfhu.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.m.share.epnwcf.com/Article/details/gfykyzmox.sHtML

[R11] case 多分支
来源：http://wap.yfazqb.com/Article/details/gvnuohpaz.sHtML

case "$1" in
来源：http://read.share.fktsv.cn/Article/details/gtxlnnksl.sHtML

start) echo "启动" ;;
来源：http://3g.tarul.cn/Article/details/gttzgywog.sHtML

stop)  echo "停止" ;;
来源：http://read.share.yfazqb.com/Article/details/glprxvcwk.sHtML

*)     echo "未知命令" ;;
来源：http://baike.fktsv.cn/Article/details/guouzaefs.sHtML

esac
来源：http://baike.epnwcf.com/Article/details/gblzqurcl.sHtML

[R12] for 遍历文件
来源：http://www.blog.epnwcf.com/Article/details/ggpfoetim.sHtML

for f in *.txt; do echo "$f"; done
来源：http://wap.tarul.cn/Article/details/ghkaivxgl.sHtML

[R13] for 计数循环
来源：http://read.share.epnwcf.com/Article/details/gljcdorrx.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://m.share.bbcook.cn/Article/details/gzlknwdpb.sHtML

[R14] C 风格 for
来源：http://mobile.fktsv.cn/Article/details/grqrunaru.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.blog.sjlbkw.cn/Article/details/gsjtyzomp.sHtML

[R15] while 逐行读文件
来源：http://m.share.bbcook.cn/Article/details/gevxqnmml.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.blog.sjlbkw.cn/Article/details/gdgarwrfe.sHtML

[R16] until 等待条件
来源：http://blog.vehdjk.com/Article/details/gpumuyine.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://3g.tarul.cn/Article/details/guqetbbep.sHtML

[R17] 数组定义与取值
来源：http://www.share.sjlbkw.cn/Article/details/ghserleji.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.m.share.bbcook.cn/Article/details/gzlhffblc.sHtML

[R18] 遍历数组
来源：http://www.blog.epnwcf.com/Article/details/gbhiehcad.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://mobile.epnwcf.com/Article/details/gyjnhnzzt.sHtML

[R19] 数组长度
来源：http://www.m.share.sjlbkw.cn/Article/details/gargvpnyg.sHtML

echo "${#arr[@]}"
来源：http://m.share.fktsv.cn/Article/details/glgztcjtv.sHtML

[R20] 关联数组（字典）
来源：http://blog.yfazqb.com/Article/details/gzwvkcjwj.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.blog.sjlbkw.cn/Article/details/gixajlcce.sHtML

[R21] 字符串长度
来源：http://read.share.epnwcf.com/Article/details/gactsgkpw.sHtML

echo "${#s}"
来源：http://www.share.fktsv.cn/Article/details/gyncclubl.sHtML

[R22] 截取子串
来源：http://read.share.yfazqb.com/Article/details/gmgsxsgps.sHtML

echo "${s:0:5}"
来源：http://blog.yfazqb.com/Article/details/gcixwzpgh.sHtML

[R23] 字符串替换
来源：http://baike.vehdjk.com/Article/details/gsduvllnm.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://3g.epnwcf.com/Article/details/gnmuveazl.sHtML

[R24] 大小写转换
来源：http://baike.vehdjk.com/Article/details/gklfnorqs.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://3g.vehdjk.com/Article/details/gajenwuua.sHtML

[R25] 去后缀 / 去前缀
来源：http://m.share.sjlbkw.cn/Article/details/gkzkesfle.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.m.share.vehdjk.com/Article/details/gvxdwzdgf.sHtML

[R26] 命令替换
来源：http://read.share.vehdjk.com/Article/details/ggiwzyoxt.sHtML

now=$(date +%F); echo "$now"
来源：http://www.share.fktsv.cn/Article/details/gnlrappdi.sHtML

[R27] 算术展开
来源：http://baike.epnwcf.com/Article/details/grzhjtynt.sHtML

echo $((1 + 2 * 3))
来源：http://mobile.tarul.cn/Article/details/gxhaatamp.sHtML

[R28] 浮点运算
来源：http://baike.vehdjk.com/Article/details/gobhtkwvj.sHtML

echo "scale=2; 10/3" | bc
来源：http://blog.yfazqb.com/Article/details/gvocyvvii.sHtML

[R29] 定义函数
来源：http://mobile.sjlbkw.cn/Article/details/gwdaczmzm.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.share.sjlbkw.cn/Article/details/gisezutae.sHtML

[R30] 函数返回状态码
来源：http://www.blog.vehdjk.com/Article/details/gjqzwpvjl.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://m.share.tarul.cn/Article/details/gvkjzmnzz.sHtML

[R31] 局部变量
来源：http://wap.bbcook.cn/Article/details/gxyotmbzt.sHtML

f() { local x=1; echo "$x"; }
来源：http://wap.fktsv.cn/Article/details/gpoupvgcv.sHtML

[R32] 参数个数校验
来源：http://www.share.vehdjk.com/Article/details/gzwaujale.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://m.share.vehdjk.com/Article/details/gzhepygjm.sHtML

[R33] 捕获错误并提示行号
来源：http://www.share.yfazqb.com/Article/details/gbyxpjtai.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.m.share.fktsv.cn/Article/details/glpuvpidb.sHtML

[R34] 退出时清理
来源：http://blog.tarul.cn/Article/details/gehconyix.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://blog.bbcook.cn/Article/details/guxibofve.sHtML

[R35] 后台执行并等待
来源：http://www.blog.yfazqb.com/Article/details/gityigmxg.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://wap.epnwcf.com/Article/details/gneovsgxs.sHtML

[R36] 并发执行多个任务
来源：http://m.share.sjlbkw.cn/Article/details/gqrmaktkt.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.blog.fktsv.cn/Article/details/gdimhrfma.sHtML

[R37] 把输出赋给变量
来源：http://mobile.yfazqb.com/Article/details/gyodbpdss.sHtML

files=$(ls -1)
来源：http://m.share.bbcook.cn/Article/details/ghtbczzpu.sHtML

[R38] 管道串联
来源：http://m.share.bbcook.cn/Article/details/gswfpnxww.sHtML

cat a.txt | grep -i error | wc -l
来源：http://3g.yfazqb.com/Article/details/gtbsahsvz.sHtML

[R39] 重定向标准输出与错误
来源：http://read.share.tarul.cn/Article/details/gonpekazv.sHtML

cmd > out.log 2>&1
来源：http://www.m.share.yfazqb.com/Article/details/gopctukbj.sHtML

[R40] 追加写日志
来源：http://baike.fktsv.cn/Article/details/gsmceuwpl.sHtML

echo "log" >> out.log
来源：http://read.share.sjlbkw.cn/Article/details/gwnxrxfqf.sHtML

[R41] 丢弃输出
来源：http://blog.epnwcf.com/Article/details/gvwyibeqn.sHtML

cmd >/dev/null 2>&1
来源：http://wap.bbcook.cn/Article/details/gjgjeeyzz.sHtML

[R42] 输入重定向
来源：http://mobile.yfazqb.com/Article/details/gaqoqahae.sHtML

wc -l < a.txt
来源：http://3g.epnwcf.com/Article/details/gaxpnmfky.sHtML

[R43] 按名字查找文件
来源：http://www.m.share.yfazqb.com/Article/details/gvxyjgioe.sHtML

find . -name "*.log" -type f
来源：http://m.share.vehdjk.com/Article/details/gbcqsgvpy.sHtML

[R44] 按修改时间查找
来源：http://www.m.share.fktsv.cn/Article/details/gmnolkoqs.sHtML

find . -mtime -7 -type f
来源：http://www.share.vehdjk.com/Article/details/geathdshm.sHtML

[R45] 批量删除
来源：http://www.blog.tarul.cn/Article/details/gqsguemhm.sHtML

find . -name "*.tmp" -delete
来源：http://www.share.yfazqb.com/Article/details/glkskxfay.sHtML

[R46] 递归替换文件内容
来源：http://read.share.bbcook.cn/Article/details/gvgxixvel.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://blog.tarul.cn/Article/details/ggtlmflii.sHtML

[R47] sed 单行替换
来源：http://wap.fktsv.cn/Article/details/gatlumpry.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.share.tarul.cn/Article/details/gpklusual.sHtML

[R48] awk 取指定列
来源：http://wap.tarul.cn/Article/details/gsulnekdd.sHtML

awk '{print $1, $3}' a.txt
来源：http://baike.bbcook.cn/Article/details/gxglwysis.sHtML

[R49] awk 带条件
来源：http://wap.bbcook.cn/Article/details/gwyxixoio.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://blog.yfazqb.com/Article/details/gvcjrvbgl.sHtML

[R50] awk 求和
来源：http://www.m.share.tarul.cn/Article/details/gserhzcgs.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://3g.bbcook.cn/Article/details/gtemdvxbp.sHtML

[R51] 排序去重取前几
来源：http://www.share.epnwcf.com/Article/details/gcrfespki.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.m.share.fktsv.cn/Article/details/gcsfotrqv.sHtML

[R52] 统计行数
来源：http://www.blog.vehdjk.com/Article/details/gvfdqomsc.sHtML

wc -l a.txt
来源：http://www.m.share.sjlbkw.cn/Article/details/gdqtcsnqx.sHtML

[R53] 查看文件头与实时尾
来源：http://read.share.tarul.cn/Article/details/gucfmthwx.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://3g.tarul.cn/Article/details/gkmxpezcc.sHtML

[R54] 比较两个文件
来源：http://www.m.share.sjlbkw.cn/Article/details/gysdprzsi.sHtML

diff a.txt b.txt
来源：http://baike.bbcook.cn/Article/details/gfrgyxbub.sHtML

[R55] 压缩与解压
来源：http://wap.bbcook.cn/Article/details/gyomimotv.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.share.fktsv.cn/Article/details/gobmieszk.sHtML

[R56] 远程拷贝
来源：http://baike.tarul.cn/Article/details/gryepawyw.sHtML

scp file user@host:/path/
来源：http://www.share.vehdjk.com/Article/details/goqnuazfn.sHtML

[R57] 远程执行命令
来源：http://www.m.share.sjlbkw.cn/Article/details/gbqomxvra.sHtML

ssh user@host 'uptime'
来源：http://www.blog.epnwcf.com/Article/details/gymcjsfzc.sHtML

[R58] 下载文件
来源：http://read.share.vehdjk.com/Article/details/ghwnqqlsz.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://3g.vehdjk.com/Article/details/ggsmblhnu.sHtML

[R59] 发 POST JSON
来源：http://blog.fktsv.cn/Article/details/geficojtq.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wap.fktsv.cn/Article/details/gyjmkrpbb.sHtML

[R60] 只看 HTTP 状态码
来源：http://3g.bbcook.cn/Article/details/gzpushjpu.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mobile.sjlbkw.cn/Article/details/gufkllczi.sHtML

[R61] 磁盘占用
来源：http://www.m.share.epnwcf.com/Article/details/gmoplhtxn.sHtML

df -h;  du -sh *
来源：http://www.blog.bbcook.cn/Article/details/ghpfwvlzp.sHtML

[R62] 找最占空间的文件
来源：http://baike.sjlbkw.cn/Article/details/gbdeikwjz.sHtML

du -ah . | sort -rh | head -10
来源：http://m.share.tarul.cn/Article/details/ggtywwnyb.sHtML

[R63] 内存与进程
来源：http://blog.fktsv.cn/Article/details/gxsfaigdz.sHtML

free -h;  ps aux | grep nginx
来源：http://mobile.epnwcf.com/Article/details/ghyazbhvw.sHtML

[R64] 结束进程
来源：http://baike.sjlbkw.cn/Article/details/gmgzajbyl.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.share.epnwcf.com/Article/details/gvpxwchzj.sHtML

[R65] 查看端口占用
来源：http://mobile.yfazqb.com/Article/details/gbhmkdohf.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://3g.vehdjk.com/Article/details/gorglbhfm.sHtML

[R66] 定时任务
来源：http://blog.tarul.cn/Article/details/gdxovacxq.sHtML

crontab -e;  crontab -l
来源：http://wap.sjlbkw.cn/Article/details/gbqtopgtf.sHtML

[R67] 生成随机十六进制串
来源：http://m.share.bbcook.cn/Article/details/gobseatvq.sHtML

openssl rand -hex 16
来源：http://www.blog.tarul.cn/Article/details/gmbyulcvu.sHtML

[R68] 计算文件校验值
来源：http://baike.yfazqb.com/Article/details/gwheqebjx.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://wap.tarul.cn/Article/details/ggvpftzuw.sHtML

[R69] 生成随机密码
来源：http://3g.tarul.cn/Article/details/gyadxnamb.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.blog.tarul.cn/Article/details/gwuszhact.sHtML

[R70] 时间戳与互转
来源：http://blog.yfazqb.com/Article/details/gnvaiwyef.sHtML

date +%s;  date -d @1700000000
来源：http://read.share.yfazqb.com/Article/details/gjikfdjux.sHtML

[R71] 日期格式化
来源：http://blog.fktsv.cn/Article/details/guhcadhgp.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://baike.epnwcf.com/Article/details/ggjudcwim.sHtML

[R72] 等待端口就绪
来源：http://www.m.share.vehdjk.com/Article/details/gpezzviok.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://3g.yfazqb.com/Article/details/ggpbktvzn.sHtML

[R73] 分割大日志
来源：http://www.m.share.bbcook.cn/Article/details/gkvispdic.sHtML

split -l 1000 big.log part_
来源：http://wap.bbcook.cn/Article/details/gqeryskff.sHtML

[R74] 批量重命名
来源：http://wap.vehdjk.com/Article/details/goosckkqt.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://read.share.epnwcf.com/Article/details/glaugidzs.sHtML

[R75] 导出环境变量
来源：http://wap.vehdjk.com/Article/details/gpqmfylii.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://3g.vehdjk.com/Article/details/ghqfebqqq.sHtML

[R76] 使用临时文件
来源：http://wap.fktsv.cn/Article/details/gqkxvuxsj.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.yfazqb.com/Article/details/gdqmoxjdu.sHtML

[R77] 读取用户输入
来源：http://www.share.yfazqb.com/Article/details/gchtmzxcq.sHtML

read -rp "请输入: " ans
来源：http://www.blog.bbcook.cn/Article/details/ghdwlxnyv.sHtML

[R78] 交互式菜单
来源：http://www.m.share.tarul.cn/Article/details/gxoapfkyn.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.share.tarul.cn/Article/details/gkyirhhkz.sHtML

[R79] 解析命令行选项
来源：http://m.share.epnwcf.com/Article/details/gpytqiger.sHtML


<!-- 参考信息 -->