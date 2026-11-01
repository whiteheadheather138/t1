代发 wailian999

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://read.share.fktsv.cn/Article/details/gauyrlztr.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.m.share.tarul.cn/Article/details/gpaxtenal.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.blog.tarul.cn/Article/details/grbcwmqji.sHtML

[Q41] 多表连接
来源：http://mobile.sjlbkw.cn/Article/details/gbtxyuwsh.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.blog.sjlbkw.cn/Article/details/gdqnqkhjk.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.m.share.vehdjk.com/Article/details/gxygxjsog.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://m.share.tarul.cn/Article/details/gappkwvdj.sHtML

[Q42] 连接条件附加过滤
来源：http://www.m.share.vehdjk.com/Article/details/goktubamx.sHtML

SELECT u.name, o.amount FROM users u
来源：http://wap.fktsv.cn/Article/details/gtkzwpxee.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://blog.sjlbkw.cn/Article/details/gpzhbebks.sHtML

[Q43] 标量子查询
来源：http://mobile.yfazqb.com/Article/details/giazeezxa.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://wap.fktsv.cn/Article/details/guzmjyfrv.sHtML

[Q44] IN 子查询
来源：http://blog.tarul.cn/Article/details/germewkdo.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.blog.vehdjk.com/Article/details/gnmeuaihu.sHtML

[Q45] EXISTS 判断存在
来源：http://3g.tarul.cn/Article/details/gzvyvwhit.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.tarul.cn/Article/details/gkmiclkai.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://baike.epnwcf.com/Article/details/gtfyzopjl.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.yfazqb.com/Article/details/gmydpvcbr.sHtML

[Q47] 与平均值比较
来源：http://blog.fktsv.cn/Article/details/gscsspkao.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://baike.sjlbkw.cn/Article/details/gnubxfzcb.sHtML

[Q48] CTE 公用表表达式
来源：http://www.m.share.bbcook.cn/Article/details/gskmcydzq.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://read.share.vehdjk.com/Article/details/gilqyyjfo.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://3g.yfazqb.com/Article/details/ghflevrie.sHtML

[Q49] 更新单行
来源：http://www.share.fktsv.cn/Article/details/gshhjioeo.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.blog.sjlbkw.cn/Article/details/givhglpnx.sHtML

[Q50] 批量更新
来源：http://www.share.sjlbkw.cn/Article/details/gchxazdac.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://read.share.fktsv.cn/Article/details/gfnvcmija.sHtML

[Q51] 用子查询更新
来源：http://m.share.sjlbkw.cn/Article/details/gkpbaluay.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.share.sjlbkw.cn/Article/details/ggjfgvhxq.sHtML

[Q52] 删除指定行
来源：http://3g.tarul.cn/Article/details/grazimdrg.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.blog.epnwcf.com/Article/details/gzxsywgis.sHtML

[Q53] 按条件删除
来源：http://www.share.tarul.cn/Article/details/gmhxrqyou.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://blog.tarul.cn/Article/details/gssttfrlf.sHtML

[Q54] 清空表
来源：http://baike.bbcook.cn/Article/details/gpbvwovnh.sHtML

TRUNCATE TABLE logs;
来源：http://www.share.tarul.cn/Article/details/gbaviprlx.sHtML

[Q55] 排名（并列占位）
来源：http://m.share.bbcook.cn/Article/details/gxjvxspju.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.blog.bbcook.cn/Article/details/gocgqiyhr.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.share.fktsv.cn/Article/details/gucjlxhsj.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://read.share.yfazqb.com/Article/details/gvnubenxn.sHtML

[Q57] 行号
来源：http://www.m.share.sjlbkw.cn/Article/details/gkfgqkypi.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://blog.fktsv.cn/Article/details/gnuzslyuv.sHtML

[Q58] 累计求和
来源：http://m.share.fktsv.cn/Article/details/gejqtldqw.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://mobile.tarul.cn/Article/details/gjijprifn.sHtML

[Q59] 分组内累计
来源：http://blog.fktsv.cn/Article/details/gkedrckez.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://m.share.vehdjk.com/Article/details/gmbpprazv.sHtML

[Q60] 取上一行 / 下一行
来源：http://mobile.fktsv.cn/Article/details/gocfkpkxz.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://baike.sjlbkw.cn/Article/details/gnxgjyfpd.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.blog.sjlbkw.cn/Article/details/grrrkjlbj.sHtML

[Q61] 移动平均
来源：http://m.share.fktsv.cn/Article/details/gjcxgxtlo.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://3g.fktsv.cn/Article/details/gekdyrznt.sHtML

[Q62] 分组占比
来源：http://blog.fktsv.cn/Article/details/gpmevnbvm.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.blog.yfazqb.com/Article/details/gzeptqqyl.sHtML

[Q63] 开启事务
来源：http://www.m.share.tarul.cn/Article/details/gxyzvvzwp.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://wap.yfazqb.com/Article/details/gqdjhraap.sHtML

[Q64] 提交事务
来源：http://www.blog.yfazqb.com/Article/details/ggkxpnenw.sHtML

COMMIT;
来源：http://mobile.sjlbkw.cn/Article/details/gkweqhhds.sHtML

[Q65] 回滚事务
来源：http://read.share.epnwcf.com/Article/details/gwiikczkm.sHtML

ROLLBACK;
来源：http://baike.sjlbkw.cn/Article/details/glfpssmfo.sHtML

[Q66] 行锁查询
来源：http://m.share.bbcook.cn/Article/details/gmdbwnzog.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://wap.yfazqb.com/Article/details/gggqpiyim.sHtML

[Q67] 设置隔离级别
来源：http://www.m.share.epnwcf.com/Article/details/gqoqknwae.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://3g.fktsv.cn/Article/details/gewqyjcfy.sHtML

[Q68] 保存点
来源：http://3g.epnwcf.com/Article/details/gzezleyds.sHtML

SAVEPOINT sp1;
来源：http://www.m.share.bbcook.cn/Article/details/greowuytb.sHtML

ROLLBACK TO sp1;
来源：http://baike.fktsv.cn/Article/details/gbwgocycl.sHtML

[Q69] 查看执行计划
来源：http://read.share.yfazqb.com/Article/details/gdtgorcaa.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://mobile.yfazqb.com/Article/details/gpmmdqxwv.sHtML

[Q70] 更新统计信息
来源：http://read.share.vehdjk.com/Article/details/gqgdekooo.sHtML

ANALYZE TABLE users;
来源：http://3g.bbcook.cn/Article/details/gevzaaape.sHtML

[Q71] 查看建表语句
来源：http://read.share.yfazqb.com/Article/details/gowmstfnb.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://read.share.vehdjk.com/Article/details/gxicjopwr.sHtML

[Q72] 查看索引
来源：http://www.blog.fktsv.cn/Article/details/gonscvxew.sHtML

SHOW INDEX FROM users;
来源：http://www.blog.yfazqb.com/Article/details/gvilbfyfs.sHtML

[Q73] 查看表状态
来源：http://www.share.sjlbkw.cn/Article/details/gexrlbqva.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://read.share.sjlbkw.cn/Article/details/grfpdvgmw.sHtML

[Q74] 强制使用索引
来源：http://m.share.yfazqb.com/Article/details/gwdmcsolq.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://mobile.bbcook.cn/Article/details/gjluzfhek.sHtML

[Q75] 日期格式化
来源：http://3g.vehdjk.com/Article/details/gifibgsfo.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://blog.vehdjk.com/Article/details/ghxsizadl.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.share.sjlbkw.cn/Article/details/gdmpiotjr.sHtML

[Q76] 按天统计
来源：http://baike.yfazqb.com/Article/details/gnwhlhesm.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://3g.tarul.cn/Article/details/gehmvvxwb.sHtML

[Q77] 时间加减
来源：http://wap.bbcook.cn/Article/details/gcstuiaae.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://3g.yfazqb.com/Article/details/gnzhhwyhp.sHtML

[Q78] 当前时间
来源：http://3g.tarul.cn/Article/details/gnazjsdgu.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://blog.yfazqb.com/Article/details/gxyyidkwe.sHtML

[Q79] 字符串拼接
来源：http://www.share.tarul.cn/Article/details/gbdqzyiqs.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://read.share.yfazqb.com/Article/details/gurysnyel.sHtML

[Q80] 字符串截取
来源：http://www.share.fktsv.cn/Article/details/gyittakbt.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://read.share.epnwcf.com/Article/details/glxwenpqt.sHtML

[Q81] 字符串替换
来源：http://read.share.sjlbkw.cn/Article/details/garoglhgx.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://m.share.sjlbkw.cn/Article/details/gmzxsajaf.sHtML

[Q82] 字符长度与字节长度
来源：http://blog.sjlbkw.cn/Article/details/gjubdwiqy.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://3g.tarul.cn/Article/details/gddhhtowh.sHtML

[Q83] 大小写转换
来源：http://mobile.fktsv.cn/Article/details/gwxugzxsn.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.share.vehdjk.com/Article/details/gpcpfdljh.sHtML

[Q84] 去除首尾空格
来源：http://m.share.vehdjk.com/Article/details/gzzlgonnr.sHtML

SELECT TRIM(name) FROM users;
来源：http://mobile.fktsv.cn/Article/details/gojtjfssv.sHtML

[Q85] 数值取整
来源：http://baike.sjlbkw.cn/Article/details/gksffduow.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://read.share.vehdjk.com/Article/details/gyxegptqv.sHtML

[Q86] 读取 JSON 字段
来源：http://wap.bbcook.cn/Article/details/gmzcvzedq.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://mobile.yfazqb.com/Article/details/gjxwbvwbr.sHtML

[Q87] JSON 字段做条件
来源：http://3g.vehdjk.com/Article/details/gldifajco.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://m.share.bbcook.cn/Article/details/gjlfwmqnu.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.share.epnwcf.com/Article/details/gnlsjwabu.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.share.yfazqb.com/Article/details/glbwgucbn.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.blog.bbcook.cn/Article/details/gtjmnrncg.sHtML

[Q89] 判断表是否存在
来源：http://blog.sjlbkw.cn/Article/details/gujdgwsxf.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://baike.yfazqb.com/Article/details/ghgpzqsfm.sHtML

[Q90] 生成序号列
来源：http://m.share.yfazqb.com/Article/details/gpdsbxcbs.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://m.share.fktsv.cn/Article/details/gyuynkonb.sHtML

================================================================================
来源：http://read.share.vehdjk.com/Article/details/gkcantvas.sHtML

R. Bash 专题
来源：http://m.share.tarul.cn/Article/details/gzfjeuzsv.sHtML

================================================================================
来源：http://www.blog.vehdjk.com/Article/details/gydwtoili.sHtML

[R01] shebang 与严格模式
来源：http://read.share.fktsv.cn/Article/details/gkgglcjid.sHtML

#!/usr/bin/env bash
来源：http://baike.sjlbkw.cn/Article/details/gtqjewcwn.sHtML

set -euo pipefail
来源：http://www.blog.fktsv.cn/Article/details/gfpxgmavy.sHtML

[R02] 变量赋值与使用
来源：http://3g.epnwcf.com/Article/details/gvlzybshc.sHtML

name="Tom"; echo "$name"
来源：http://wap.yfazqb.com/Article/details/gahyhmmlu.sHtML

[R03] 只读变量
来源：http://read.share.fktsv.cn/Article/details/gewzysjjf.sHtML

readonly PI=3.14
来源：http://m.share.bbcook.cn/Article/details/gafxsqmhi.sHtML

[R04] 位置参数
来源：http://www.m.share.epnwcf.com/Article/details/gebriwnki.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.blog.vehdjk.com/Article/details/grcdvfxzi.sHtML

[R05] 参数默认值
来源：http://3g.epnwcf.com/Article/details/gjjhavufj.sHtML

name="${1:-default}"
来源：http://www.share.vehdjk.com/Article/details/grxfzgcqk.sHtML

[R06] 判断命令是否存在
来源：http://m.share.tarul.cn/Article/details/gbqgfmmqs.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://mobile.yfazqb.com/Article/details/gwgccczic.sHtML

[R07] if 判断文件
来源：http://www.m.share.fktsv.cn/Article/details/gtgdrhtiu.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://mobile.tarul.cn/Article/details/gyolugocs.sHtML

[R08] 数值比较
来源：http://www.m.share.tarul.cn/Article/details/grdtltkxi.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://blog.bbcook.cn/Article/details/gyzscecez.sHtML

[R09] 字符串比较
来源：http://www.blog.sjlbkw.cn/Article/details/gxkuoonku.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://3g.sjlbkw.cn/Article/details/goacuiyyv.sHtML

[R10] 正则匹配
来源：http://www.blog.sjlbkw.cn/Article/details/gtibijlic.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://baike.tarul.cn/Article/details/gattomwsf.sHtML

[R11] case 多分支
来源：http://3g.vehdjk.com/Article/details/ggxmsqpni.sHtML

case "$1" in
来源：http://mobile.bbcook.cn/Article/details/gwspttxwh.sHtML

start) echo "启动" ;;
来源：http://www.share.fktsv.cn/Article/details/gnekncjgo.sHtML

stop)  echo "停止" ;;
来源：http://www.blog.bbcook.cn/Article/details/gefzvirfv.sHtML

*)     echo "未知命令" ;;
来源：http://read.share.epnwcf.com/Article/details/gudhdxfzp.sHtML

esac
来源：http://read.share.bbcook.cn/Article/details/gqytemius.sHtML

[R12] for 遍历文件
来源：http://m.share.tarul.cn/Article/details/gpcvaugrl.sHtML

for f in *.txt; do echo "$f"; done
来源：http://3g.sjlbkw.cn/Article/details/gwiytsnbt.sHtML

[R13] for 计数循环
来源：http://www.blog.epnwcf.com/Article/details/ghcdlxzsv.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://m.share.epnwcf.com/Article/details/gnolzoauj.sHtML

[R14] C 风格 for
来源：http://m.share.epnwcf.com/Article/details/gwasurdwp.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.share.sjlbkw.cn/Article/details/gfnywalnb.sHtML

[R15] while 逐行读文件
来源：http://baike.fktsv.cn/Article/details/gmvitrtyo.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.m.share.fktsv.cn/Article/details/gehtdghqg.sHtML

[R16] until 等待条件
来源：http://baike.fktsv.cn/Article/details/ghycgihjq.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://wap.vehdjk.com/Article/details/gtxouzsjl.sHtML

[R17] 数组定义与取值
来源：http://www.share.tarul.cn/Article/details/gcfidwply.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.share.fktsv.cn/Article/details/gfnylfpnk.sHtML

[R18] 遍历数组
来源：http://blog.bbcook.cn/Article/details/ghobcuojn.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.blog.epnwcf.com/Article/details/gahivfwgi.sHtML

[R19] 数组长度
来源：http://read.share.bbcook.cn/Article/details/goiihkwix.sHtML

echo "${#arr[@]}"
来源：http://www.share.sjlbkw.cn/Article/details/givvnrhii.sHtML

[R20] 关联数组（字典）
来源：http://wap.epnwcf.com/Article/details/gtgahfinr.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://m.share.tarul.cn/Article/details/gkrtgkewo.sHtML

[R21] 字符串长度
来源：http://mobile.yfazqb.com/Article/details/gokwazpeh.sHtML

echo "${#s}"
来源：http://read.share.yfazqb.com/Article/details/gwcxsrwnx.sHtML

[R22] 截取子串
来源：http://blog.yfazqb.com/Article/details/gwrfkquyl.sHtML

echo "${s:0:5}"
来源：http://www.m.share.yfazqb.com/Article/details/gafwyliat.sHtML

[R23] 字符串替换
来源：http://m.share.bbcook.cn/Article/details/giwrfeeea.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://mobile.bbcook.cn/Article/details/gdhvfvrla.sHtML

[R24] 大小写转换
来源：http://wap.sjlbkw.cn/Article/details/gempgtknt.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.share.vehdjk.com/Article/details/grwszqpsp.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.blog.epnwcf.com/Article/details/gbhxqsaoz.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.m.share.epnwcf.com/Article/details/gngtbwvlh.sHtML

[R26] 命令替换
来源：http://mobile.fktsv.cn/Article/details/gtiyznebf.sHtML

now=$(date +%F); echo "$now"
来源：http://www.m.share.tarul.cn/Article/details/gazzvqhwp.sHtML

[R27] 算术展开
来源：http://www.m.share.tarul.cn/Article/details/giggflnlb.sHtML

echo $((1 + 2 * 3))
来源：http://www.share.epnwcf.com/Article/details/gccjbkzml.sHtML

[R28] 浮点运算
来源：http://wap.tarul.cn/Article/details/gqramyllz.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.share.sjlbkw.cn/Article/details/gzgynlvzn.sHtML

[R29] 定义函数
来源：http://3g.vehdjk.com/Article/details/gywoczvby.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://mobile.bbcook.cn/Article/details/gnqmpwdbm.sHtML

[R30] 函数返回状态码
来源：http://www.m.share.bbcook.cn/Article/details/ghrrehzpg.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://mobile.yfazqb.com/Article/details/gxotuiavj.sHtML

[R31] 局部变量
来源：http://m.share.tarul.cn/Article/details/gimvpfdcu.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.m.share.epnwcf.com/Article/details/ghgyjfyvc.sHtML

[R32] 参数个数校验
来源：http://m.share.yfazqb.com/Article/details/gfxywbebk.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://read.share.yfazqb.com/Article/details/gcnlhpkfh.sHtML

[R33] 捕获错误并提示行号
来源：http://3g.vehdjk.com/Article/details/gceyxylco.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://read.share.fktsv.cn/Article/details/gdrlhpibv.sHtML

[R34] 退出时清理
来源：http://www.m.share.tarul.cn/Article/details/gsfcvaaky.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.share.fktsv.cn/Article/details/gumqsxzqn.sHtML

[R35] 后台执行并等待
来源：http://read.share.yfazqb.com/Article/details/gaxbcemfs.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://wap.yfazqb.com/Article/details/guketavfq.sHtML

[R36] 并发执行多个任务
来源：http://www.share.vehdjk.com/Article/details/gefbgmjxx.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://blog.vehdjk.com/Article/details/gfjhndtpi.sHtML

[R37] 把输出赋给变量
来源：http://www.share.tarul.cn/Article/details/gibebyxty.sHtML

files=$(ls -1)
来源：http://3g.fktsv.cn/Article/details/gaughplqx.sHtML

[R38] 管道串联
来源：http://read.share.tarul.cn/Article/details/grshzorxr.sHtML

cat a.txt | grep -i error | wc -l
来源：http://baike.bbcook.cn/Article/details/gpxdbhqex.sHtML

[R39] 重定向标准输出与错误
来源：http://www.blog.sjlbkw.cn/Article/details/gouqqzmls.sHtML

cmd > out.log 2>&1
来源：http://read.share.tarul.cn/Article/details/gixwgkxtx.sHtML

[R40] 追加写日志
来源：http://baike.vehdjk.com/Article/details/gipradocy.sHtML

echo "log" >> out.log
来源：http://www.blog.fktsv.cn/Article/details/gicqwavnt.sHtML

[R41] 丢弃输出
来源：http://read.share.vehdjk.com/Article/details/gauflkdbm.sHtML

cmd >/dev/null 2>&1
来源：http://baike.vehdjk.com/Article/details/gzjapfmuo.sHtML

[R42] 输入重定向
来源：http://read.share.tarul.cn/Article/details/gbeenxnar.sHtML

wc -l < a.txt
来源：http://www.share.fktsv.cn/Article/details/gmncgwsle.sHtML

[R43] 按名字查找文件
来源：http://baike.vehdjk.com/Article/details/gmrotdtzq.sHtML

find . -name "*.log" -type f
来源：http://blog.bbcook.cn/Article/details/gqnqhpzrg.sHtML

[R44] 按修改时间查找
来源：http://read.share.vehdjk.com/Article/details/giaczvgxr.sHtML

find . -mtime -7 -type f
来源：http://baike.vehdjk.com/Article/details/ggfzhrqvp.sHtML

[R45] 批量删除
来源：http://www.share.fktsv.cn/Article/details/gjxmfxsqw.sHtML

find . -name "*.tmp" -delete
来源：http://3g.vehdjk.com/Article/details/gablsdlar.sHtML

[R46] 递归替换文件内容
来源：http://baike.epnwcf.com/Article/details/gbxrpteic.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://3g.yfazqb.com/Article/details/gqnunuvtu.sHtML

[R47] sed 单行替换
来源：http://3g.vehdjk.com/Article/details/gyjlkodfh.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.share.tarul.cn/Article/details/gtnphqekm.sHtML

[R48] awk 取指定列
来源：http://www.share.vehdjk.com/Article/details/ghgxsatxx.sHtML

awk '{print $1, $3}' a.txt
来源：http://3g.vehdjk.com/Article/details/gfnbvxtyu.sHtML

[R49] awk 带条件
来源：http://3g.tarul.cn/Article/details/gusuiysnd.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.share.sjlbkw.cn/Article/details/gagpogidr.sHtML

[R50] awk 求和
来源：http://blog.yfazqb.com/Article/details/gagylzkps.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://3g.fktsv.cn/Article/details/gdtrcvpaq.sHtML

[R51] 排序去重取前几
来源：http://www.share.bbcook.cn/Article/details/gqzqozeyh.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.m.share.vehdjk.com/Article/details/gqvlgbroa.sHtML

[R52] 统计行数
来源：http://mobile.sjlbkw.cn/Article/details/gmntvpzma.sHtML

wc -l a.txt
来源：http://www.m.share.yfazqb.com/Article/details/gfqxwspup.sHtML

[R53] 查看文件头与实时尾
来源：http://baike.tarul.cn/Article/details/gcieewlig.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://3g.tarul.cn/Article/details/gitolyhmc.sHtML

[R54] 比较两个文件
来源：http://m.share.epnwcf.com/Article/details/genuujbju.sHtML

diff a.txt b.txt
来源：http://m.share.fktsv.cn/Article/details/gcbgaxtax.sHtML

[R55] 压缩与解压
来源：http://m.share.epnwcf.com/Article/details/gixrbzzrr.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mobile.fktsv.cn/Article/details/gyeyzlsxa.sHtML

[R56] 远程拷贝
来源：http://m.share.sjlbkw.cn/Article/details/gcneouczu.sHtML

scp file user@host:/path/
来源：http://www.share.sjlbkw.cn/Article/details/grjrtoxna.sHtML

[R57] 远程执行命令
来源：http://baike.tarul.cn/Article/details/gqvbdpado.sHtML

ssh user@host 'uptime'
来源：http://www.share.epnwcf.com/Article/details/gbyyqqzkv.sHtML

[R58] 下载文件
来源：http://wap.tarul.cn/Article/details/gvmwepawz.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.share.vehdjk.com/Article/details/gglhoqlei.sHtML

[R59] 发 POST JSON
来源：http://mobile.tarul.cn/Article/details/giamgwbdb.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wap.bbcook.cn/Article/details/gmhhyxuja.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.share.bbcook.cn/Article/details/gxryvtxhz.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://baike.vehdjk.com/Article/details/gcpqsmrjp.sHtML

[R61] 磁盘占用
来源：http://www.blog.vehdjk.com/Article/details/gdvvkipgd.sHtML

df -h;  du -sh *
来源：http://www.share.tarul.cn/Article/details/gclaogmno.sHtML

[R62] 找最占空间的文件
来源：http://blog.fktsv.cn/Article/details/gauwmphjd.sHtML

du -ah . | sort -rh | head -10
来源：http://mobile.tarul.cn/Article/details/gzunejfuw.sHtML

[R63] 内存与进程
来源：http://wap.bbcook.cn/Article/details/gxfpeibon.sHtML

free -h;  ps aux | grep nginx
来源：http://www.m.share.tarul.cn/Article/details/gwnfogwnt.sHtML

[R64] 结束进程
来源：http://3g.bbcook.cn/Article/details/ghlayzucb.sHtML

kill -9 $(pgrep -f app.py)
来源：http://mobile.vehdjk.com/Article/details/gjbocvxho.sHtML

[R65] 查看端口占用
来源：http://3g.vehdjk.com/Article/details/gzslnoleq.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://blog.bbcook.cn/Article/details/goonmpmez.sHtML

[R66] 定时任务
来源：http://wap.sjlbkw.cn/Article/details/gnusrozga.sHtML

crontab -e;  crontab -l
来源：http://wap.sjlbkw.cn/Article/details/grjovlhtq.sHtML

[R67] 生成随机十六进制串
来源：http://3g.bbcook.cn/Article/details/gvyahugdh.sHtML

openssl rand -hex 16
来源：http://www.share.vehdjk.com/Article/details/gmaxcwifw.sHtML

[R68] 计算文件校验值
来源：http://www.share.fktsv.cn/Article/details/gvlndzefu.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.m.share.vehdjk.com/Article/details/gmwnkxllk.sHtML

[R69] 生成随机密码
来源：http://wap.epnwcf.com/Article/details/guchuhngk.sHtML

head -c 16 /dev/urandom | base64
来源：http://baike.vehdjk.com/Article/details/gwrzeyksu.sHtML

[R70] 时间戳与互转
来源：http://m.share.epnwcf.com/Article/details/gdhtagnfp.sHtML

date +%s;  date -d @1700000000
来源：http://m.share.tarul.cn/Article/details/glnikbvix.sHtML

[R71] 日期格式化
来源：http://wap.bbcook.cn/Article/details/grsybnbum.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://baike.fktsv.cn/Article/details/gyfeqgjkn.sHtML

[R72] 等待端口就绪
来源：http://mobile.vehdjk.com/Article/details/ghvolfwkg.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://wap.fktsv.cn/Article/details/ghsenmdyw.sHtML

[R73] 分割大日志
来源：http://blog.sjlbkw.cn/Article/details/gidipdoqb.sHtML

split -l 1000 big.log part_
来源：http://read.share.epnwcf.com/Article/details/gqoioytrs.sHtML

[R74] 批量重命名
来源：http://3g.epnwcf.com/Article/details/gkbwomtku.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://blog.bbcook.cn/Article/details/gjkkimfkj.sHtML

[R75] 导出环境变量
来源：http://m.share.epnwcf.com/Article/details/gtmtnwfzd.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://blog.fktsv.cn/Article/details/gwhyjolqu.sHtML

[R76] 使用临时文件
来源：http://baike.yfazqb.com/Article/details/ggqwmocah.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://read.share.yfazqb.com/Article/details/grotbjcma.sHtML

[R77] 读取用户输入
来源：http://m.share.sjlbkw.cn/Article/details/grdfhitfg.sHtML

read -rp "请输入: " ans
来源：http://www.blog.bbcook.cn/Article/details/gdirrfoot.sHtML

[R78] 交互式菜单
来源：http://www.m.share.fktsv.cn/Article/details/gnisuateq.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://baike.yfazqb.com/Article/details/gyocfyhpj.sHtML

[R79] 解析命令行选项
来源：http://www.blog.bbcook.cn/Article/details/gzacrhlar.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.m.share.yfazqb.com/Article/details/gmovtincx.sHtML

[R80] 查看脚本执行耗时
来源：http://blog.vehdjk.com/Article/details/gchgzbvwh.sHtML

time ./run.sh
来源：http://wap.bbcook.cn/Article/details/gtqhnjgct.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/gmmxqhkdk.sHtML

S. C / C++ 专题
来源：http://www.share.sjlbkw.cn/Article/details/grrlcjkgc.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/gffsimplf.sHtML

[S01] C：Hello World
来源：http://mobile.vehdjk.com/Article/details/gorwqwomd.sHtML

#include <stdio.h>
来源：http://mobile.bbcook.cn/Article/details/gmqypvdkt.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://baike.yfazqb.com/Article/details/gvxhrunyk.sHtML

[S02] C：变量与格式化输出
来源：http://mobile.sjlbkw.cn/Article/details/gzunvicds.sHtML

int a = 10; printf("%d\n", a);
来源：http://baike.tarul.cn/Article/details/gspigvels.sHtML

[S03] C：读入整数
来源：http://www.blog.sjlbkw.cn/Article/details/gouqzpiou.sHtML

int x; scanf("%d", &x);
来源：http://www.share.yfazqb.com/Article/details/gykvaqnlb.sHtML

[S04] C：字符串复制
来源：http://read.share.fktsv.cn/Article/details/gcpvieqek.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://baike.tarul.cn/Article/details/gopwaseve.sHtML

[S05] C：字符串长度
来源：http://read.share.yfazqb.com/Article/details/gzboctrtp.sHtML

strlen(s)
来源：http://www.blog.bbcook.cn/Article/details/gyxbnpwbz.sHtML

[S06] C：字符串比较
来源：http://baike.epnwcf.com/Article/details/ghsshrfbq.sHtML

strcmp(a, b) == 0
来源：http://mobile.sjlbkw.cn/Article/details/gxemttehq.sHtML

[S07] C：数组遍历求和
来源：http://wap.bbcook.cn/Article/details/geopvsqyf.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://m.share.tarul.cn/Article/details/gpfibwgsj.sHtML

[S08] C：动态内存分配与释放
来源：http://wap.sjlbkw.cn/Article/details/gtagvcfrb.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.blog.epnwcf.com/Article/details/gctmdofhv.sHtML

[S09] C：结构体定义与初始化
来源：http://blog.tarul.cn/Article/details/gkzyyirui.sHtML


<!-- 参考信息 -->