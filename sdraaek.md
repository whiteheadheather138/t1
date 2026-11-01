代发 wailian999

SELECT MAX(age), MIN(age) FROM users;
来源：http://3g.epnwcf.com/Article/details/gbqoxyzzx.sHtML

[Q30] 分组统计
来源：http://blog.tarul.cn/Article/details/glphfjqja.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://3g.fktsv.cn/Article/details/gmpvsjwoc.sHtML

[Q31] 分组后过滤
来源：http://mobile.bbcook.cn/Article/details/gjaoszgkd.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://wap.bbcook.cn/Article/details/girkoomsy.sHtML

[Q32] 分组拼接字符串
来源：http://www.share.sjlbkw.cn/Article/details/gjkvnlwxu.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://mobile.tarul.cn/Article/details/grakvgvlp.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://wap.tarul.cn/Article/details/godpbkdyn.sHtML

[Q33] 多列分组
来源：http://wap.tarul.cn/Article/details/gaxkgitsx.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://m.share.fktsv.cn/Article/details/gqqzjiqjc.sHtML

[Q34] 每组取第一条
来源：http://3g.bbcook.cn/Article/details/gfedvdsye.sHtML

SELECT * FROM (
来源：http://www.m.share.yfazqb.com/Article/details/gogmrjfrg.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://wap.tarul.cn/Article/details/gvagkgnmx.sHtML

) t WHERE rn = 1;
来源：http://3g.bbcook.cn/Article/details/gqofycrau.sHtML

[Q35] 内连接
来源：http://www.blog.epnwcf.com/Article/details/gvxbvyygz.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.share.sjlbkw.cn/Article/details/gyjebfiuv.sHtML

[Q36] 左连接
来源：http://read.share.epnwcf.com/Article/details/gadtgqoym.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://3g.yfazqb.com/Article/details/gvedsvksf.sHtML

[Q37] 右连接
来源：http://www.blog.fktsv.cn/Article/details/gjavhplka.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://baike.vehdjk.com/Article/details/gxoosjroc.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://wap.fktsv.cn/Article/details/grmuethfj.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.m.share.bbcook.cn/Article/details/gzzmjlstp.sHtML

[Q39] 自连接（查上下级）
来源：http://read.share.fktsv.cn/Article/details/gfmrtlbna.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.m.share.epnwcf.com/Article/details/gkikzjbhn.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://read.share.sjlbkw.cn/Article/details/gwvlkrmxi.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://wap.bbcook.cn/Article/details/gjmwbyagu.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.share.fktsv.cn/Article/details/gyicxddwq.sHtML

[Q41] 多表连接
来源：http://m.share.tarul.cn/Article/details/gpztggzrf.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://baike.tarul.cn/Article/details/gphgtgric.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.m.share.fktsv.cn/Article/details/gxfydxvmf.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.blog.tarul.cn/Article/details/gsvzyvhmc.sHtML

[Q42] 连接条件附加过滤
来源：http://baike.epnwcf.com/Article/details/gmuompnck.sHtML

SELECT u.name, o.amount FROM users u
来源：http://mobile.fktsv.cn/Article/details/gdvqfnmps.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://mobile.sjlbkw.cn/Article/details/gzzafalob.sHtML

[Q43] 标量子查询
来源：http://3g.tarul.cn/Article/details/gwsskrtba.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://wap.bbcook.cn/Article/details/gujkppdtr.sHtML

[Q44] IN 子查询
来源：http://www.blog.fktsv.cn/Article/details/gkigydrel.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://mobile.tarul.cn/Article/details/gcngvcijx.sHtML

[Q45] EXISTS 判断存在
来源：http://3g.yfazqb.com/Article/details/grseoyvkm.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.sjlbkw.cn/Article/details/gkzazhtxr.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://baike.yfazqb.com/Article/details/grdgzyjqp.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.sjlbkw.cn/Article/details/gykrprdil.sHtML

[Q47] 与平均值比较
来源：http://wap.vehdjk.com/Article/details/gnyygbxxy.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://mobile.tarul.cn/Article/details/ggtuxqbia.sHtML

[Q48] CTE 公用表表达式
来源：http://mobile.vehdjk.com/Article/details/gmatiuvem.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://wap.vehdjk.com/Article/details/gqkverssq.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://3g.epnwcf.com/Article/details/grgmmgbtw.sHtML

[Q49] 更新单行
来源：http://wap.fktsv.cn/Article/details/gkckbjhcq.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://m.share.bbcook.cn/Article/details/gndfnjgro.sHtML

[Q50] 批量更新
来源：http://blog.fktsv.cn/Article/details/glmuzxibl.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://3g.tarul.cn/Article/details/gjocxwtxn.sHtML

[Q51] 用子查询更新
来源：http://read.share.sjlbkw.cn/Article/details/gbmqowied.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.share.fktsv.cn/Article/details/gwycuhmvn.sHtML

[Q52] 删除指定行
来源：http://blog.bbcook.cn/Article/details/gsopinxek.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.blog.yfazqb.com/Article/details/ghjilnxac.sHtML

[Q53] 按条件删除
来源：http://wap.bbcook.cn/Article/details/gpopcgsls.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://mobile.fktsv.cn/Article/details/gsotxgyxm.sHtML

[Q54] 清空表
来源：http://www.m.share.epnwcf.com/Article/details/gdagdjotx.sHtML

TRUNCATE TABLE logs;
来源：http://read.share.sjlbkw.cn/Article/details/gjvhsiuod.sHtML

[Q55] 排名（并列占位）
来源：http://read.share.epnwcf.com/Article/details/gaekyahbx.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://blog.tarul.cn/Article/details/gjvyxxknz.sHtML

[Q56] 密集排名（并列不占位）
来源：http://3g.sjlbkw.cn/Article/details/gthjjmohu.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.m.share.yfazqb.com/Article/details/grdnnxhty.sHtML

[Q57] 行号
来源：http://www.blog.tarul.cn/Article/details/grrebetzf.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://read.share.yfazqb.com/Article/details/gjdpqoqkj.sHtML

[Q58] 累计求和
来源：http://blog.epnwcf.com/Article/details/gnqekvgsm.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.blog.vehdjk.com/Article/details/gvkzstxzi.sHtML

[Q59] 分组内累计
来源：http://mobile.fktsv.cn/Article/details/gyjnoirvg.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.blog.epnwcf.com/Article/details/ghfybhmcg.sHtML

[Q60] 取上一行 / 下一行
来源：http://3g.yfazqb.com/Article/details/gwuolqjjx.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.share.sjlbkw.cn/Article/details/gglafdopi.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://mobile.fktsv.cn/Article/details/gdpeqxvrw.sHtML

[Q61] 移动平均
来源：http://www.share.fktsv.cn/Article/details/gyaemygef.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://wap.vehdjk.com/Article/details/gezdarlxi.sHtML

[Q62] 分组占比
来源：http://mobile.vehdjk.com/Article/details/gyuktepph.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://baike.sjlbkw.cn/Article/details/gptadximi.sHtML

[Q63] 开启事务
来源：http://www.blog.epnwcf.com/Article/details/gbgxhkjqx.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://mobile.fktsv.cn/Article/details/gbdlhgpqn.sHtML

[Q64] 提交事务
来源：http://www.blog.vehdjk.com/Article/details/gsfdsnecd.sHtML

COMMIT;
来源：http://m.share.sjlbkw.cn/Article/details/gkrttvgva.sHtML

[Q65] 回滚事务
来源：http://blog.epnwcf.com/Article/details/goclnqjyl.sHtML

ROLLBACK;
来源：http://www.m.share.epnwcf.com/Article/details/gbvlshgdh.sHtML

[Q66] 行锁查询
来源：http://mobile.epnwcf.com/Article/details/gmqrkfrcz.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://baike.sjlbkw.cn/Article/details/gbavawjis.sHtML

[Q67] 设置隔离级别
来源：http://wap.fktsv.cn/Article/details/glfqeukmc.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.blog.fktsv.cn/Article/details/glsdwtvag.sHtML

[Q68] 保存点
来源：http://read.share.fktsv.cn/Article/details/gszerhcmf.sHtML

SAVEPOINT sp1;
来源：http://baike.sjlbkw.cn/Article/details/gkoaxhzov.sHtML

ROLLBACK TO sp1;
来源：http://mobile.epnwcf.com/Article/details/gsgrpzjkh.sHtML

[Q69] 查看执行计划
来源：http://blog.yfazqb.com/Article/details/gugmahnvu.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://baike.fktsv.cn/Article/details/ghyjubpqi.sHtML

[Q70] 更新统计信息
来源：http://wap.bbcook.cn/Article/details/gcbfibjfm.sHtML

ANALYZE TABLE users;
来源：http://www.blog.epnwcf.com/Article/details/gpdflzowj.sHtML

[Q71] 查看建表语句
来源：http://read.share.vehdjk.com/Article/details/gpuizefpw.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://mobile.vehdjk.com/Article/details/gqbyltpwn.sHtML

[Q72] 查看索引
来源：http://wap.fktsv.cn/Article/details/gmerxkwcw.sHtML

SHOW INDEX FROM users;
来源：http://read.share.epnwcf.com/Article/details/gblrjkukw.sHtML

[Q73] 查看表状态
来源：http://m.share.yfazqb.com/Article/details/gysbjoygk.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://read.share.bbcook.cn/Article/details/gzttimvpk.sHtML

[Q74] 强制使用索引
来源：http://read.share.epnwcf.com/Article/details/gwligqlip.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://baike.epnwcf.com/Article/details/giicjprie.sHtML

[Q75] 日期格式化
来源：http://m.share.tarul.cn/Article/details/gzblvoqxr.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.m.share.yfazqb.com/Article/details/gdhbqbqnx.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://wap.tarul.cn/Article/details/gomiqneza.sHtML

[Q76] 按天统计
来源：http://read.share.bbcook.cn/Article/details/gsbusdzyp.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.share.tarul.cn/Article/details/gyvwgfgos.sHtML

[Q77] 时间加减
来源：http://www.m.share.fktsv.cn/Article/details/gkwhcbhft.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.m.share.tarul.cn/Article/details/gcohvjcij.sHtML

[Q78] 当前时间
来源：http://blog.vehdjk.com/Article/details/gmackvnby.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://mobile.epnwcf.com/Article/details/grkyjmvsq.sHtML

[Q79] 字符串拼接
来源：http://www.blog.fktsv.cn/Article/details/gixmbmgnn.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://wap.vehdjk.com/Article/details/glzzmhize.sHtML

[Q80] 字符串截取
来源：http://m.share.bbcook.cn/Article/details/gavvzyzel.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://m.share.yfazqb.com/Article/details/giyydygoc.sHtML

[Q81] 字符串替换
来源：http://3g.yfazqb.com/Article/details/gufhozupq.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://baike.sjlbkw.cn/Article/details/gjppnbhxw.sHtML

[Q82] 字符长度与字节长度
来源：http://read.share.epnwcf.com/Article/details/getzlxpcj.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://read.share.epnwcf.com/Article/details/gxtmvysyy.sHtML

[Q83] 大小写转换
来源：http://www.share.sjlbkw.cn/Article/details/gidrritck.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://3g.bbcook.cn/Article/details/gqtylealp.sHtML

[Q84] 去除首尾空格
来源：http://3g.vehdjk.com/Article/details/gshjebbbh.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.m.share.bbcook.cn/Article/details/gqcrcbuua.sHtML

[Q85] 数值取整
来源：http://read.share.fktsv.cn/Article/details/gbtcsrbji.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://mobile.vehdjk.com/Article/details/gemiiihww.sHtML

[Q86] 读取 JSON 字段
来源：http://baike.sjlbkw.cn/Article/details/gujdcjpvh.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://3g.sjlbkw.cn/Article/details/gukuhuibw.sHtML

[Q87] JSON 字段做条件
来源：http://www.m.share.fktsv.cn/Article/details/gbzjxonas.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://m.share.tarul.cn/Article/details/gspmovosh.sHtML

[Q88] 行转列（条件聚合）
来源：http://3g.bbcook.cn/Article/details/goyyybjlf.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://3g.yfazqb.com/Article/details/gsdbvlymb.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://3g.sjlbkw.cn/Article/details/grxuorkeo.sHtML

[Q89] 判断表是否存在
来源：http://3g.fktsv.cn/Article/details/gifmfbusj.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://3g.sjlbkw.cn/Article/details/gdunevdkm.sHtML

[Q90] 生成序号列
来源：http://www.share.bbcook.cn/Article/details/gwvmiqrcu.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.m.share.epnwcf.com/Article/details/gecncurnd.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/ghoyaxebq.sHtML

R. Bash 专题
来源：http://m.share.tarul.cn/Article/details/gyoqdqvou.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/gihycnnth.sHtML

[R01] shebang 与严格模式
来源：http://www.blog.vehdjk.com/Article/details/gysgrvukq.sHtML

#!/usr/bin/env bash
来源：http://www.m.share.fktsv.cn/Article/details/gtmnrcbay.sHtML

set -euo pipefail
来源：http://mobile.vehdjk.com/Article/details/gceohrcou.sHtML

[R02] 变量赋值与使用
来源：http://m.share.tarul.cn/Article/details/gphjzdrbx.sHtML

name="Tom"; echo "$name"
来源：http://mobile.tarul.cn/Article/details/gvbpvdhqs.sHtML

[R03] 只读变量
来源：http://www.share.tarul.cn/Article/details/gefzdlvjc.sHtML

readonly PI=3.14
来源：http://www.m.share.fktsv.cn/Article/details/gwyohwedu.sHtML

[R04] 位置参数
来源：http://www.share.fktsv.cn/Article/details/gglnflapv.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.m.share.fktsv.cn/Article/details/gdshfhbhf.sHtML

[R05] 参数默认值
来源：http://m.share.bbcook.cn/Article/details/girvlggji.sHtML

name="${1:-default}"
来源：http://3g.yfazqb.com/Article/details/grneexwrd.sHtML

[R06] 判断命令是否存在
来源：http://3g.bbcook.cn/Article/details/guwdhvidn.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://m.share.bbcook.cn/Article/details/gvfjevuta.sHtML

[R07] if 判断文件
来源：http://www.blog.fktsv.cn/Article/details/glywrkjqz.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://read.share.tarul.cn/Article/details/gfwlisstk.sHtML

[R08] 数值比较
来源：http://m.share.fktsv.cn/Article/details/gygbguxbl.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://blog.yfazqb.com/Article/details/grlsgtfks.sHtML

[R09] 字符串比较
来源：http://www.blog.sjlbkw.cn/Article/details/gaizwoksz.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.m.share.fktsv.cn/Article/details/gbfgyhtzl.sHtML

[R10] 正则匹配
来源：http://wap.yfazqb.com/Article/details/gvyuxtfvw.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.share.yfazqb.com/Article/details/gxyjnctxr.sHtML

[R11] case 多分支
来源：http://www.m.share.bbcook.cn/Article/details/gjohfcqjt.sHtML

case "$1" in
来源：http://baike.vehdjk.com/Article/details/gilbmufjq.sHtML

start) echo "启动" ;;
来源：http://3g.epnwcf.com/Article/details/gebivtjtm.sHtML

stop)  echo "停止" ;;
来源：http://blog.fktsv.cn/Article/details/gjqhiurrn.sHtML

*)     echo "未知命令" ;;
来源：http://www.m.share.epnwcf.com/Article/details/gfzrytbst.sHtML

esac
来源：http://3g.sjlbkw.cn/Article/details/gfvdmlskc.sHtML

[R12] for 遍历文件
来源：http://baike.epnwcf.com/Article/details/gtznrdady.sHtML

for f in *.txt; do echo "$f"; done
来源：http://baike.bbcook.cn/Article/details/gyxqjgfyx.sHtML

[R13] for 计数循环
来源：http://www.m.share.sjlbkw.cn/Article/details/gkuelbpkh.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.blog.sjlbkw.cn/Article/details/gtklarqdw.sHtML

[R14] C 风格 for
来源：http://mobile.yfazqb.com/Article/details/gdkgwvtqe.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.m.share.vehdjk.com/Article/details/gefnyvxig.sHtML

[R15] while 逐行读文件
来源：http://baike.bbcook.cn/Article/details/gdnbsocbx.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://blog.vehdjk.com/Article/details/gkfidrntu.sHtML

[R16] until 等待条件
来源：http://3g.epnwcf.com/Article/details/gffhkquwo.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.m.share.sjlbkw.cn/Article/details/gyuslzdxj.sHtML

[R17] 数组定义与取值
来源：http://wap.bbcook.cn/Article/details/gbsgerqne.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://mobile.tarul.cn/Article/details/grqloxpyh.sHtML

[R18] 遍历数组
来源：http://wap.vehdjk.com/Article/details/gnergqect.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://m.share.bbcook.cn/Article/details/geudqswfd.sHtML

[R19] 数组长度
来源：http://mobile.tarul.cn/Article/details/gfyqrgwyl.sHtML

echo "${#arr[@]}"
来源：http://blog.yfazqb.com/Article/details/gxdnhqxyj.sHtML

[R20] 关联数组（字典）
来源：http://read.share.epnwcf.com/Article/details/gxuymlgtx.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://3g.vehdjk.com/Article/details/gimvujwod.sHtML

[R21] 字符串长度
来源：http://m.share.epnwcf.com/Article/details/gpvyjtais.sHtML

echo "${#s}"
来源：http://www.m.share.bbcook.cn/Article/details/gouickjvi.sHtML

[R22] 截取子串
来源：http://read.share.sjlbkw.cn/Article/details/grfsveoqb.sHtML

echo "${s:0:5}"
来源：http://www.blog.vehdjk.com/Article/details/gyizuirbi.sHtML

[R23] 字符串替换
来源：http://mobile.fktsv.cn/Article/details/gjppwmbim.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.blog.tarul.cn/Article/details/gqjebfgsp.sHtML

[R24] 大小写转换
来源：http://www.share.tarul.cn/Article/details/gyzclcpxv.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://blog.yfazqb.com/Article/details/gnxyroqfj.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.share.sjlbkw.cn/Article/details/gprswiupj.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://mobile.vehdjk.com/Article/details/ghqkwssrq.sHtML

[R26] 命令替换
来源：http://3g.bbcook.cn/Article/details/gstqbulea.sHtML

now=$(date +%F); echo "$now"
来源：http://www.blog.fktsv.cn/Article/details/gudueylqs.sHtML

[R27] 算术展开
来源：http://m.share.tarul.cn/Article/details/geguckifz.sHtML

echo $((1 + 2 * 3))
来源：http://m.share.fktsv.cn/Article/details/giekkzdfv.sHtML

[R28] 浮点运算
来源：http://mobile.fktsv.cn/Article/details/gcblisdhl.sHtML

echo "scale=2; 10/3" | bc
来源：http://wap.tarul.cn/Article/details/gsoabumvt.sHtML

[R29] 定义函数
来源：http://www.blog.epnwcf.com/Article/details/gjhocyuac.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://mobile.epnwcf.com/Article/details/gjvftvqqa.sHtML

[R30] 函数返回状态码
来源：http://wap.yfazqb.com/Article/details/goswmkuii.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://m.share.fktsv.cn/Article/details/gidaytyoj.sHtML

[R31] 局部变量
来源：http://www.m.share.epnwcf.com/Article/details/gcdvtnbns.sHtML

f() { local x=1; echo "$x"; }
来源：http://blog.fktsv.cn/Article/details/gzehmuutd.sHtML

[R32] 参数个数校验
来源：http://blog.bbcook.cn/Article/details/gfnenarlj.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://blog.tarul.cn/Article/details/gjndykglr.sHtML

[R33] 捕获错误并提示行号
来源：http://blog.yfazqb.com/Article/details/gmwfmozen.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://wap.bbcook.cn/Article/details/ghnrmqhdr.sHtML

[R34] 退出时清理
来源：http://m.share.tarul.cn/Article/details/grpwrjsvq.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://baike.tarul.cn/Article/details/giicgmjsa.sHtML

[R35] 后台执行并等待
来源：http://blog.tarul.cn/Article/details/gworrdovg.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.blog.bbcook.cn/Article/details/ggwttwymg.sHtML

[R36] 并发执行多个任务
来源：http://www.m.share.vehdjk.com/Article/details/gudlwcwbo.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://baike.yfazqb.com/Article/details/gbiokfrsf.sHtML

[R37] 把输出赋给变量
来源：http://3g.sjlbkw.cn/Article/details/gvcgrjoqj.sHtML

files=$(ls -1)
来源：http://baike.vehdjk.com/Article/details/greumlvsq.sHtML

[R38] 管道串联
来源：http://mobile.epnwcf.com/Article/details/gsewigsvr.sHtML

cat a.txt | grep -i error | wc -l
来源：http://3g.bbcook.cn/Article/details/glxuegnpu.sHtML

[R39] 重定向标准输出与错误
来源：http://blog.vehdjk.com/Article/details/gxzpvebpl.sHtML

cmd > out.log 2>&1
来源：http://m.share.tarul.cn/Article/details/gyeussqci.sHtML

[R40] 追加写日志
来源：http://wap.bbcook.cn/Article/details/glgcjfwiy.sHtML

echo "log" >> out.log
来源：http://baike.bbcook.cn/Article/details/guszhycdx.sHtML

[R41] 丢弃输出
来源：http://m.share.epnwcf.com/Article/details/gbxevfdgt.sHtML

cmd >/dev/null 2>&1
来源：http://www.share.yfazqb.com/Article/details/gljcbxsmb.sHtML

[R42] 输入重定向
来源：http://m.share.sjlbkw.cn/Article/details/gecvkcxza.sHtML

wc -l < a.txt
来源：http://3g.fktsv.cn/Article/details/gnikwogpn.sHtML

[R43] 按名字查找文件
来源：http://m.share.tarul.cn/Article/details/gyyfuxlub.sHtML

find . -name "*.log" -type f
来源：http://m.share.fktsv.cn/Article/details/gxzeizobz.sHtML

[R44] 按修改时间查找
来源：http://www.m.share.bbcook.cn/Article/details/gyvtcxjze.sHtML

find . -mtime -7 -type f
来源：http://baike.yfazqb.com/Article/details/giwugwciv.sHtML

[R45] 批量删除
来源：http://www.blog.epnwcf.com/Article/details/glleepfhr.sHtML

find . -name "*.tmp" -delete
来源：http://www.share.tarul.cn/Article/details/ggltwdjtb.sHtML

[R46] 递归替换文件内容
来源：http://mobile.sjlbkw.cn/Article/details/gdznstzgq.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://read.share.epnwcf.com/Article/details/gdwkvyzib.sHtML

[R47] sed 单行替换
来源：http://blog.epnwcf.com/Article/details/gapbxvgym.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.m.share.fktsv.cn/Article/details/geeovvphe.sHtML

[R48] awk 取指定列
来源：http://www.m.share.fktsv.cn/Article/details/gieraojao.sHtML

awk '{print $1, $3}' a.txt
来源：http://read.share.tarul.cn/Article/details/guvzbkfgq.sHtML

[R49] awk 带条件
来源：http://m.share.epnwcf.com/Article/details/gnvfmbeqy.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://3g.vehdjk.com/Article/details/gulqgtcki.sHtML

[R50] awk 求和
来源：http://blog.sjlbkw.cn/Article/details/gmzfovwfq.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://m.share.sjlbkw.cn/Article/details/gyfeifopp.sHtML

[R51] 排序去重取前几
来源：http://3g.fktsv.cn/Article/details/gvohqgdkg.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://blog.yfazqb.com/Article/details/gjrzuihrq.sHtML

[R52] 统计行数
来源：http://www.share.tarul.cn/Article/details/gxjagsvgi.sHtML

wc -l a.txt
来源：http://3g.bbcook.cn/Article/details/gludbuiht.sHtML

[R53] 查看文件头与实时尾
来源：http://www.m.share.epnwcf.com/Article/details/gdlghifqr.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://read.share.epnwcf.com/Article/details/gdpfwonqs.sHtML

[R54] 比较两个文件
来源：http://blog.sjlbkw.cn/Article/details/gehwituzj.sHtML

diff a.txt b.txt
来源：http://mobile.vehdjk.com/Article/details/ggnusewyb.sHtML

[R55] 压缩与解压
来源：http://wap.sjlbkw.cn/Article/details/givsjgbxu.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://blog.epnwcf.com/Article/details/gtrimuovl.sHtML

[R56] 远程拷贝
来源：http://www.m.share.sjlbkw.cn/Article/details/gxxjytswh.sHtML

scp file user@host:/path/
来源：http://baike.vehdjk.com/Article/details/giieogdkl.sHtML

[R57] 远程执行命令
来源：http://www.share.vehdjk.com/Article/details/gdxfomzsf.sHtML

ssh user@host 'uptime'
来源：http://www.m.share.bbcook.cn/Article/details/gulsfrjph.sHtML

[R58] 下载文件
来源：http://read.share.tarul.cn/Article/details/gvqljuhob.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.share.fktsv.cn/Article/details/gcjviapso.sHtML

[R59] 发 POST JSON
来源：http://wap.sjlbkw.cn/Article/details/gcnhxjjig.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.blog.vehdjk.com/Article/details/gppwotvjr.sHtML

[R60] 只看 HTTP 状态码
来源：http://3g.bbcook.cn/Article/details/gtttatafu.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.share.vehdjk.com/Article/details/gsqvoaewl.sHtML

[R61] 磁盘占用
来源：http://mobile.bbcook.cn/Article/details/ghkpwgxvm.sHtML

df -h;  du -sh *
来源：http://www.m.share.sjlbkw.cn/Article/details/ghenhqhzv.sHtML

[R62] 找最占空间的文件
来源：http://baike.epnwcf.com/Article/details/gcnisiztc.sHtML

du -ah . | sort -rh | head -10
来源：http://3g.epnwcf.com/Article/details/gqziaxgsh.sHtML

[R63] 内存与进程
来源：http://baike.fktsv.cn/Article/details/gekpyembo.sHtML

free -h;  ps aux | grep nginx
来源：http://baike.fktsv.cn/Article/details/gvhhtaevi.sHtML

[R64] 结束进程
来源：http://www.share.vehdjk.com/Article/details/guoczpitz.sHtML

kill -9 $(pgrep -f app.py)
来源：http://mobile.fktsv.cn/Article/details/gbrsafmhk.sHtML

[R65] 查看端口占用
来源：http://3g.vehdjk.com/Article/details/gptvrnpax.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://blog.epnwcf.com/Article/details/gsbbufiyo.sHtML

[R66] 定时任务
来源：http://blog.sjlbkw.cn/Article/details/gxzmdrntk.sHtML

crontab -e;  crontab -l
来源：http://3g.sjlbkw.cn/Article/details/gxvpniabr.sHtML

[R67] 生成随机十六进制串
来源：http://read.share.fktsv.cn/Article/details/godkpxkpq.sHtML

openssl rand -hex 16
来源：http://mobile.yfazqb.com/Article/details/grizwyfan.sHtML

[R68] 计算文件校验值
来源：http://mobile.yfazqb.com/Article/details/gzzkjfswi.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://mobile.fktsv.cn/Article/details/gflusomjo.sHtML

[R69] 生成随机密码
来源：http://m.share.sjlbkw.cn/Article/details/glhvjbfom.sHtML

head -c 16 /dev/urandom | base64
来源：http://read.share.tarul.cn/Article/details/gmcgflosm.sHtML

[R70] 时间戳与互转
来源：http://www.share.fktsv.cn/Article/details/gqmisdnpq.sHtML

date +%s;  date -d @1700000000
来源：http://www.blog.fktsv.cn/Article/details/gneekjadh.sHtML

[R71] 日期格式化
来源：http://baike.yfazqb.com/Article/details/grtxfjvdq.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.blog.yfazqb.com/Article/details/gsvivgxzt.sHtML

[R72] 等待端口就绪
来源：http://blog.sjlbkw.cn/Article/details/gbjrvtlnl.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://3g.vehdjk.com/Article/details/gksvvesyf.sHtML

[R73] 分割大日志
来源：http://wap.tarul.cn/Article/details/gomwxuffh.sHtML

split -l 1000 big.log part_
来源：http://read.share.yfazqb.com/Article/details/ghlrfioqn.sHtML

[R74] 批量重命名
来源：http://blog.tarul.cn/Article/details/gldhztkjh.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://baike.sjlbkw.cn/Article/details/gozwciywy.sHtML

[R75] 导出环境变量
来源：http://www.blog.bbcook.cn/Article/details/ggwfghnbq.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://wap.fktsv.cn/Article/details/geuzjeqkl.sHtML

[R76] 使用临时文件
来源：http://mobile.yfazqb.com/Article/details/gzhkbqays.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://read.share.bbcook.cn/Article/details/gzduutgfr.sHtML

[R77] 读取用户输入
来源：http://baike.epnwcf.com/Article/details/gdwhpxhoo.sHtML

read -rp "请输入: " ans
来源：http://read.share.yfazqb.com/Article/details/gaogoeotl.sHtML

[R78] 交互式菜单
来源：http://m.share.epnwcf.com/Article/details/gzqdwawyr.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.blog.bbcook.cn/Article/details/gjxthsyow.sHtML

[R79] 解析命令行选项
来源：http://mobile.fktsv.cn/Article/details/goxnmxgoe.sHtML


<!-- 参考信息 -->