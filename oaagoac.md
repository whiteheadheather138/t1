代发 wailian999

SELECT MAX(age), MIN(age) FROM users;
来源：http://mobile.tarul.cn/Article/details/gjxtzjjzt.sHtML

[Q30] 分组统计
来源：http://wap.epnwcf.com/Article/details/gdgqcjwgz.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.m.share.epnwcf.com/Article/details/gfvqaheqa.sHtML

[Q31] 分组后过滤
来源：http://3g.fktsv.cn/Article/details/gpemauelw.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://3g.bbcook.cn/Article/details/gvgctupmy.sHtML

[Q32] 分组拼接字符串
来源：http://www.share.vehdjk.com/Article/details/gasdbwsgy.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.blog.yfazqb.com/Article/details/gksltlmsn.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.share.sjlbkw.cn/Article/details/gryfukvkf.sHtML

[Q33] 多列分组
来源：http://3g.tarul.cn/Article/details/gwndhdhrx.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.m.share.fktsv.cn/Article/details/gqzhffcti.sHtML

[Q34] 每组取第一条
来源：http://www.blog.bbcook.cn/Article/details/gmyxoylwx.sHtML

SELECT * FROM (
来源：http://m.share.vehdjk.com/Article/details/gifwmodmm.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://blog.vehdjk.com/Article/details/gpasitrfd.sHtML

) t WHERE rn = 1;
来源：http://mobile.yfazqb.com/Article/details/gncojojep.sHtML

[Q35] 内连接
来源：http://blog.fktsv.cn/Article/details/gdozncqyd.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://wap.sjlbkw.cn/Article/details/grskasscl.sHtML

[Q36] 左连接
来源：http://mobile.yfazqb.com/Article/details/ghleegvne.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://baike.epnwcf.com/Article/details/gcvmhnztz.sHtML

[Q37] 右连接
来源：http://www.blog.tarul.cn/Article/details/guafffddg.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://m.share.vehdjk.com/Article/details/gvwwfgumm.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://read.share.vehdjk.com/Article/details/gegseiexh.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://m.share.sjlbkw.cn/Article/details/geemllihe.sHtML

[Q39] 自连接（查上下级）
来源：http://www.blog.vehdjk.com/Article/details/gpjjoyaxr.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://3g.epnwcf.com/Article/details/gxotdfgre.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://mobile.sjlbkw.cn/Article/details/gbghcvcix.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.blog.sjlbkw.cn/Article/details/gzporrzmt.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://3g.sjlbkw.cn/Article/details/gvolyjvxz.sHtML

[Q41] 多表连接
来源：http://blog.yfazqb.com/Article/details/gjlpzksor.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://m.share.epnwcf.com/Article/details/gdorsylxe.sHtML

JOIN users u ON u.id = o.user_id
来源：http://m.share.sjlbkw.cn/Article/details/gerfeipkc.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://wap.fktsv.cn/Article/details/gppjphzvc.sHtML

[Q42] 连接条件附加过滤
来源：http://wap.vehdjk.com/Article/details/gwydnarqt.sHtML

SELECT u.name, o.amount FROM users u
来源：http://m.share.yfazqb.com/Article/details/gauwkgnsd.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://baike.bbcook.cn/Article/details/gxtgubzwj.sHtML

[Q43] 标量子查询
来源：http://www.share.fktsv.cn/Article/details/gtgiknndj.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://wap.sjlbkw.cn/Article/details/gdffogdzp.sHtML

[Q44] IN 子查询
来源：http://wap.bbcook.cn/Article/details/gqgatuvye.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://wap.tarul.cn/Article/details/gamtcokmo.sHtML

[Q45] EXISTS 判断存在
来源：http://mobile.epnwcf.com/Article/details/gnzocnphi.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.bbcook.cn/Article/details/gfdejuqru.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://m.share.tarul.cn/Article/details/gdjzpmmof.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.bbcook.cn/Article/details/gxnohvmwn.sHtML

[Q47] 与平均值比较
来源：http://read.share.epnwcf.com/Article/details/gpevbqwoj.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://mobile.tarul.cn/Article/details/gdyzxzbbs.sHtML

[Q48] CTE 公用表表达式
来源：http://mobile.sjlbkw.cn/Article/details/gpurablws.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://read.share.fktsv.cn/Article/details/gbczvqxzm.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.blog.sjlbkw.cn/Article/details/gmgjsdvkx.sHtML

[Q49] 更新单行
来源：http://m.share.epnwcf.com/Article/details/gigekxrcb.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://blog.sjlbkw.cn/Article/details/gohynvbaj.sHtML

[Q50] 批量更新
来源：http://mobile.tarul.cn/Article/details/gsytihxkk.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.blog.vehdjk.com/Article/details/gtzblpicj.sHtML

[Q51] 用子查询更新
来源：http://www.m.share.epnwcf.com/Article/details/gitvhvtlc.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.m.share.tarul.cn/Article/details/gvmalhqqh.sHtML

[Q52] 删除指定行
来源：http://www.share.tarul.cn/Article/details/gpzzgbzqx.sHtML

DELETE FROM users WHERE id = 10;
来源：http://blog.tarul.cn/Article/details/gdkcfufkh.sHtML

[Q53] 按条件删除
来源：http://baike.epnwcf.com/Article/details/gkuzhvqsz.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.m.share.tarul.cn/Article/details/gukubyhls.sHtML

[Q54] 清空表
来源：http://read.share.vehdjk.com/Article/details/grzqhmyor.sHtML

TRUNCATE TABLE logs;
来源：http://www.blog.vehdjk.com/Article/details/grlcvhknk.sHtML

[Q55] 排名（并列占位）
来源：http://3g.yfazqb.com/Article/details/gisatqqln.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://m.share.sjlbkw.cn/Article/details/gvxdrhcbx.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.share.bbcook.cn/Article/details/gxydpicwd.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://blog.epnwcf.com/Article/details/guazfphoi.sHtML

[Q57] 行号
来源：http://read.share.sjlbkw.cn/Article/details/gxzjxjmxm.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://read.share.bbcook.cn/Article/details/giksybznt.sHtML

[Q58] 累计求和
来源：http://wap.vehdjk.com/Article/details/gepoxeakj.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://3g.tarul.cn/Article/details/gcaqpmrvz.sHtML

[Q59] 分组内累计
来源：http://www.blog.sjlbkw.cn/Article/details/gnofqzcft.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.share.yfazqb.com/Article/details/geozunoak.sHtML

[Q60] 取上一行 / 下一行
来源：http://blog.sjlbkw.cn/Article/details/gcrybrhpi.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://3g.sjlbkw.cn/Article/details/gcuizhpob.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://blog.vehdjk.com/Article/details/gzqfdnemc.sHtML

[Q61] 移动平均
来源：http://3g.bbcook.cn/Article/details/gqgovarlr.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.share.epnwcf.com/Article/details/geiffgzdl.sHtML

[Q62] 分组占比
来源：http://baike.tarul.cn/Article/details/grzkxgfjq.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://blog.tarul.cn/Article/details/gctpufaxn.sHtML

[Q63] 开启事务
来源：http://www.m.share.bbcook.cn/Article/details/gdjcadgnq.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://blog.tarul.cn/Article/details/gxrujpdug.sHtML

[Q64] 提交事务
来源：http://baike.bbcook.cn/Article/details/gtpnmcwvj.sHtML

COMMIT;
来源：http://read.share.yfazqb.com/Article/details/gwxshfwmi.sHtML

[Q65] 回滚事务
来源：http://baike.yfazqb.com/Article/details/gvcxacyld.sHtML

ROLLBACK;
来源：http://blog.bbcook.cn/Article/details/gbxmfwmzl.sHtML

[Q66] 行锁查询
来源：http://www.blog.fktsv.cn/Article/details/gjzdrirpp.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.share.sjlbkw.cn/Article/details/grzfljjhj.sHtML

[Q67] 设置隔离级别
来源：http://wap.vehdjk.com/Article/details/gtxidawch.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.m.share.epnwcf.com/Article/details/gqppljzqn.sHtML

[Q68] 保存点
来源：http://read.share.tarul.cn/Article/details/gzgopnsqk.sHtML

SAVEPOINT sp1;
来源：http://read.share.epnwcf.com/Article/details/gzagpnvgu.sHtML

ROLLBACK TO sp1;
来源：http://read.share.yfazqb.com/Article/details/gvjixraxo.sHtML

[Q69] 查看执行计划
来源：http://www.m.share.sjlbkw.cn/Article/details/gklbcnybr.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://wap.vehdjk.com/Article/details/gqharlnwp.sHtML

[Q70] 更新统计信息
来源：http://www.share.vehdjk.com/Article/details/gjhayagtd.sHtML

ANALYZE TABLE users;
来源：http://read.share.epnwcf.com/Article/details/gleuhcqjw.sHtML

[Q71] 查看建表语句
来源：http://blog.vehdjk.com/Article/details/grcsodzyp.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://baike.fktsv.cn/Article/details/gfduiufrh.sHtML

[Q72] 查看索引
来源：http://m.share.fktsv.cn/Article/details/gzkificzc.sHtML

SHOW INDEX FROM users;
来源：http://3g.vehdjk.com/Article/details/ghrmmnrce.sHtML

[Q73] 查看表状态
来源：http://www.m.share.sjlbkw.cn/Article/details/gyiqxtpmz.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://read.share.sjlbkw.cn/Article/details/gqhdfchlc.sHtML

[Q74] 强制使用索引
来源：http://www.share.fktsv.cn/Article/details/gzqsaeham.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.blog.vehdjk.com/Article/details/gtjucfmco.sHtML

[Q75] 日期格式化
来源：http://mobile.yfazqb.com/Article/details/gtpqsbnpa.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://baike.tarul.cn/Article/details/grxjvhstv.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.blog.tarul.cn/Article/details/gspjpcotx.sHtML

[Q76] 按天统计
来源：http://read.share.fktsv.cn/Article/details/gnoyyolwa.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://wap.yfazqb.com/Article/details/gqutalktc.sHtML

[Q77] 时间加减
来源：http://www.blog.tarul.cn/Article/details/gtwrwiyic.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://baike.vehdjk.com/Article/details/gsaytopsc.sHtML

[Q78] 当前时间
来源：http://www.share.epnwcf.com/Article/details/gdnsdubjo.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://baike.vehdjk.com/Article/details/guxdmhudy.sHtML

[Q79] 字符串拼接
来源：http://3g.fktsv.cn/Article/details/gpmqfgshz.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://wap.yfazqb.com/Article/details/gtjxhdtui.sHtML

[Q80] 字符串截取
来源：http://mobile.yfazqb.com/Article/details/gchwvtyyh.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.share.sjlbkw.cn/Article/details/glxanwmwy.sHtML

[Q81] 字符串替换
来源：http://m.share.yfazqb.com/Article/details/gpohhaoia.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://blog.yfazqb.com/Article/details/gqzflfkpz.sHtML

[Q82] 字符长度与字节长度
来源：http://wap.fktsv.cn/Article/details/gmmavvvnc.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.share.fktsv.cn/Article/details/gwdomidkw.sHtML

[Q83] 大小写转换
来源：http://3g.bbcook.cn/Article/details/guqbdeuzj.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.share.fktsv.cn/Article/details/gienvrgxf.sHtML

[Q84] 去除首尾空格
来源：http://3g.epnwcf.com/Article/details/gmsptbels.sHtML

SELECT TRIM(name) FROM users;
来源：http://baike.vehdjk.com/Article/details/gnwpegvnh.sHtML

[Q85] 数值取整
来源：http://www.blog.bbcook.cn/Article/details/gguaeoozq.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://mobile.vehdjk.com/Article/details/gepyfeocg.sHtML

[Q86] 读取 JSON 字段
来源：http://blog.sjlbkw.cn/Article/details/gvgpsyqgg.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://read.share.fktsv.cn/Article/details/gtskvvfde.sHtML

[Q87] JSON 字段做条件
来源：http://www.blog.fktsv.cn/Article/details/gryppqwju.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://mobile.yfazqb.com/Article/details/gebfzblbi.sHtML

[Q88] 行转列（条件聚合）
来源：http://mobile.sjlbkw.cn/Article/details/gwowoqyvt.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://blog.bbcook.cn/Article/details/gtttjzotf.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://mobile.sjlbkw.cn/Article/details/giqrfyiyx.sHtML

[Q89] 判断表是否存在
来源：http://wap.bbcook.cn/Article/details/gwbdutilp.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.blog.fktsv.cn/Article/details/gfafetzrq.sHtML

[Q90] 生成序号列
来源：http://blog.fktsv.cn/Article/details/ggzaeihhd.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://blog.sjlbkw.cn/Article/details/gnmbyfunp.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/gplrmjyxl.sHtML

R. Bash 专题
来源：http://www.blog.sjlbkw.cn/Article/details/gtxkeopga.sHtML

================================================================================
来源：http://www.share.sjlbkw.cn/Article/details/gzqydmdkb.sHtML

[R01] shebang 与严格模式
来源：http://www.m.share.epnwcf.com/Article/details/gankhfnso.sHtML

#!/usr/bin/env bash
来源：http://www.blog.bbcook.cn/Article/details/gqqhmfenz.sHtML

set -euo pipefail
来源：http://m.share.fktsv.cn/Article/details/gbwjawxea.sHtML

[R02] 变量赋值与使用
来源：http://3g.vehdjk.com/Article/details/gyedzqveq.sHtML

name="Tom"; echo "$name"
来源：http://read.share.tarul.cn/Article/details/glnugmtjv.sHtML

[R03] 只读变量
来源：http://m.share.sjlbkw.cn/Article/details/gvnjxpsnd.sHtML

readonly PI=3.14
来源：http://www.m.share.bbcook.cn/Article/details/gcgknzmny.sHtML

[R04] 位置参数
来源：http://read.share.fktsv.cn/Article/details/ghrxmqcwz.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.m.share.epnwcf.com/Article/details/gjpcprhfo.sHtML

[R05] 参数默认值
来源：http://www.share.tarul.cn/Article/details/gdndwsuau.sHtML

name="${1:-default}"
来源：http://www.blog.bbcook.cn/Article/details/gzdccphan.sHtML

[R06] 判断命令是否存在
来源：http://www.blog.tarul.cn/Article/details/gpgzqehhe.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://m.share.yfazqb.com/Article/details/gzcyutssx.sHtML

[R07] if 判断文件
来源：http://m.share.epnwcf.com/Article/details/gutcyakyv.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://m.share.bbcook.cn/Article/details/gehkqrgvk.sHtML

[R08] 数值比较
来源：http://mobile.sjlbkw.cn/Article/details/ghgjettis.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.m.share.tarul.cn/Article/details/godbblxnx.sHtML

[R09] 字符串比较
来源：http://read.share.yfazqb.com/Article/details/guznubeea.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://3g.bbcook.cn/Article/details/ggqnravpe.sHtML

[R10] 正则匹配
来源：http://mobile.sjlbkw.cn/Article/details/genozhdxb.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.share.tarul.cn/Article/details/gxiaezmjg.sHtML

[R11] case 多分支
来源：http://3g.epnwcf.com/Article/details/gwmonblyc.sHtML

case "$1" in
来源：http://blog.vehdjk.com/Article/details/gspntzrej.sHtML

start) echo "启动" ;;
来源：http://m.share.vehdjk.com/Article/details/gtwzgcuqe.sHtML

stop)  echo "停止" ;;
来源：http://read.share.vehdjk.com/Article/details/gcvdfmwfk.sHtML

*)     echo "未知命令" ;;
来源：http://read.share.fktsv.cn/Article/details/gileefnzw.sHtML

esac
来源：http://www.m.share.fktsv.cn/Article/details/gpsddmpcd.sHtML

[R12] for 遍历文件
来源：http://read.share.tarul.cn/Article/details/glguxqbvm.sHtML

for f in *.txt; do echo "$f"; done
来源：http://baike.fktsv.cn/Article/details/gnpbnskpo.sHtML

[R13] for 计数循环
来源：http://blog.vehdjk.com/Article/details/gaqikwthn.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://wap.epnwcf.com/Article/details/gniyxwqpi.sHtML

[R14] C 风格 for
来源：http://www.blog.epnwcf.com/Article/details/gopvgnqlf.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.share.fktsv.cn/Article/details/gfdgwljxx.sHtML

[R15] while 逐行读文件
来源：http://m.share.fktsv.cn/Article/details/gxqwmsigf.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.share.tarul.cn/Article/details/gqkzrxhsp.sHtML

[R16] until 等待条件
来源：http://www.blog.tarul.cn/Article/details/gnpfzphnx.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://wap.vehdjk.com/Article/details/gkwpedluo.sHtML

[R17] 数组定义与取值
来源：http://read.share.tarul.cn/Article/details/guevrdymt.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://blog.epnwcf.com/Article/details/gtufiqsrc.sHtML

[R18] 遍历数组
来源：http://www.blog.sjlbkw.cn/Article/details/gjvuhuxfj.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://3g.yfazqb.com/Article/details/gsihfevji.sHtML

[R19] 数组长度
来源：http://www.share.yfazqb.com/Article/details/gshkohrhh.sHtML

echo "${#arr[@]}"
来源：http://m.share.bbcook.cn/Article/details/grbcexhkw.sHtML

[R20] 关联数组（字典）
来源：http://mobile.fktsv.cn/Article/details/gkyczdcrc.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.share.vehdjk.com/Article/details/gimtkpiuu.sHtML

[R21] 字符串长度
来源：http://www.share.epnwcf.com/Article/details/gmdrafsdc.sHtML

echo "${#s}"
来源：http://www.blog.sjlbkw.cn/Article/details/gcybliisl.sHtML

[R22] 截取子串
来源：http://mobile.bbcook.cn/Article/details/gvoeajoaj.sHtML

echo "${s:0:5}"
来源：http://baike.sjlbkw.cn/Article/details/gfonhakde.sHtML

[R23] 字符串替换
来源：http://www.share.bbcook.cn/Article/details/gxdtfxlnb.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://wap.vehdjk.com/Article/details/gqxhgrtiq.sHtML

[R24] 大小写转换
来源：http://www.share.tarul.cn/Article/details/gygdlzpcu.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://baike.fktsv.cn/Article/details/gxqqzpqdl.sHtML

[R25] 去后缀 / 去前缀
来源：http://3g.fktsv.cn/Article/details/ggnwqddwl.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://m.share.sjlbkw.cn/Article/details/gkmkqaaem.sHtML

[R26] 命令替换
来源：http://www.m.share.tarul.cn/Article/details/gpmeijsbc.sHtML

now=$(date +%F); echo "$now"
来源：http://www.share.fktsv.cn/Article/details/ganyqxctt.sHtML

[R27] 算术展开
来源：http://baike.sjlbkw.cn/Article/details/gwcwcoyik.sHtML

echo $((1 + 2 * 3))
来源：http://blog.sjlbkw.cn/Article/details/gobngrxrp.sHtML

[R28] 浮点运算
来源：http://m.share.epnwcf.com/Article/details/gnmbbxwfh.sHtML

echo "scale=2; 10/3" | bc
来源：http://3g.tarul.cn/Article/details/gjluxuxlh.sHtML

[R29] 定义函数
来源：http://blog.bbcook.cn/Article/details/ghrstldcb.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://mobile.bbcook.cn/Article/details/gbykadswm.sHtML

[R30] 函数返回状态码
来源：http://www.share.tarul.cn/Article/details/glqgoblxw.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.blog.tarul.cn/Article/details/gkwaktjvk.sHtML

[R31] 局部变量
来源：http://www.m.share.sjlbkw.cn/Article/details/grgjhffap.sHtML

f() { local x=1; echo "$x"; }
来源：http://mobile.bbcook.cn/Article/details/gkskrgjrh.sHtML

[R32] 参数个数校验
来源：http://mobile.tarul.cn/Article/details/gxnhlzegr.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://blog.sjlbkw.cn/Article/details/gzolkgosg.sHtML

[R33] 捕获错误并提示行号
来源：http://www.blog.vehdjk.com/Article/details/ghehhhzcg.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://m.share.tarul.cn/Article/details/gkvdbeolg.sHtML

[R34] 退出时清理
来源：http://www.blog.tarul.cn/Article/details/gepodfoyn.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://wap.vehdjk.com/Article/details/gllrnkfwf.sHtML

[R35] 后台执行并等待
来源：http://www.share.yfazqb.com/Article/details/gjdibwjgl.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://m.share.yfazqb.com/Article/details/ghknjznxa.sHtML

[R36] 并发执行多个任务
来源：http://www.m.share.yfazqb.com/Article/details/gdvorgiaq.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.m.share.fktsv.cn/Article/details/gsocfwick.sHtML

[R37] 把输出赋给变量
来源：http://m.share.yfazqb.com/Article/details/gnarqggjg.sHtML

files=$(ls -1)
来源：http://m.share.tarul.cn/Article/details/gezssdlzb.sHtML

[R38] 管道串联
来源：http://wap.epnwcf.com/Article/details/gvamyhhas.sHtML

cat a.txt | grep -i error | wc -l
来源：http://baike.tarul.cn/Article/details/gnqrrvqqo.sHtML

[R39] 重定向标准输出与错误
来源：http://www.m.share.tarul.cn/Article/details/grfqelnoa.sHtML

cmd > out.log 2>&1
来源：http://blog.vehdjk.com/Article/details/grrnqtpba.sHtML

[R40] 追加写日志
来源：http://www.share.sjlbkw.cn/Article/details/gzzoahbvq.sHtML

echo "log" >> out.log
来源：http://blog.fktsv.cn/Article/details/gagejewyt.sHtML

[R41] 丢弃输出
来源：http://blog.epnwcf.com/Article/details/geaibgyqk.sHtML

cmd >/dev/null 2>&1
来源：http://mobile.sjlbkw.cn/Article/details/gwltvgkek.sHtML

[R42] 输入重定向
来源：http://www.m.share.yfazqb.com/Article/details/gbwqivjea.sHtML

wc -l < a.txt
来源：http://blog.fktsv.cn/Article/details/gsmvxaznl.sHtML

[R43] 按名字查找文件
来源：http://www.share.fktsv.cn/Article/details/gxotpfitc.sHtML

find . -name "*.log" -type f
来源：http://mobile.vehdjk.com/Article/details/grszglybi.sHtML

[R44] 按修改时间查找
来源：http://3g.vehdjk.com/Article/details/gjljivhvl.sHtML

find . -mtime -7 -type f
来源：http://www.blog.fktsv.cn/Article/details/gvolbddtv.sHtML

[R45] 批量删除
来源：http://baike.yfazqb.com/Article/details/gghuisqfe.sHtML

find . -name "*.tmp" -delete
来源：http://read.share.sjlbkw.cn/Article/details/gmkmkgnqb.sHtML

[R46] 递归替换文件内容
来源：http://www.share.sjlbkw.cn/Article/details/gemwqslog.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://read.share.fktsv.cn/Article/details/gdkdqayed.sHtML

[R47] sed 单行替换
来源：http://mobile.bbcook.cn/Article/details/gzodzmpew.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://baike.tarul.cn/Article/details/gxvyunuuu.sHtML

[R48] awk 取指定列
来源：http://www.m.share.yfazqb.com/Article/details/gqyenloca.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.blog.fktsv.cn/Article/details/gfmhorpbk.sHtML

[R49] awk 带条件
来源：http://m.share.vehdjk.com/Article/details/gzyayjbia.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://m.share.epnwcf.com/Article/details/gsdxvxqlt.sHtML

[R50] awk 求和
来源：http://wap.bbcook.cn/Article/details/gaeitvmum.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.blog.epnwcf.com/Article/details/gyrasawci.sHtML

[R51] 排序去重取前几
来源：http://blog.tarul.cn/Article/details/grblzzoqm.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://3g.tarul.cn/Article/details/gidumyvuq.sHtML

[R52] 统计行数
来源：http://m.share.epnwcf.com/Article/details/gmnyvjhrj.sHtML

wc -l a.txt
来源：http://www.blog.bbcook.cn/Article/details/gzdfivvto.sHtML

[R53] 查看文件头与实时尾
来源：http://www.share.epnwcf.com/Article/details/gredjlejv.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://read.share.tarul.cn/Article/details/gdnvykqcv.sHtML

[R54] 比较两个文件
来源：http://blog.fktsv.cn/Article/details/ggmtyxevb.sHtML

diff a.txt b.txt
来源：http://wap.tarul.cn/Article/details/gnnpwdecf.sHtML

[R55] 压缩与解压
来源：http://mobile.fktsv.cn/Article/details/gficqoovh.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.share.tarul.cn/Article/details/gubpyzugd.sHtML

[R56] 远程拷贝
来源：http://3g.vehdjk.com/Article/details/gzfnkrawj.sHtML

scp file user@host:/path/
来源：http://mobile.fktsv.cn/Article/details/gltvyvaxk.sHtML

[R57] 远程执行命令
来源：http://www.blog.epnwcf.com/Article/details/gudkbjfri.sHtML

ssh user@host 'uptime'
来源：http://baike.epnwcf.com/Article/details/gprbnhmss.sHtML

[R58] 下载文件
来源：http://m.share.bbcook.cn/Article/details/gwoihgxyd.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://read.share.bbcook.cn/Article/details/gltymtqqq.sHtML

[R59] 发 POST JSON
来源：http://3g.fktsv.cn/Article/details/gbqsiuzqz.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://3g.fktsv.cn/Article/details/gwuksegkf.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.m.share.vehdjk.com/Article/details/gyrdvopxg.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.share.bbcook.cn/Article/details/gsrvdrrcc.sHtML

[R61] 磁盘占用
来源：http://mobile.bbcook.cn/Article/details/ggkmnivkd.sHtML

df -h;  du -sh *
来源：http://www.m.share.yfazqb.com/Article/details/gsfpzmtdm.sHtML

[R62] 找最占空间的文件
来源：http://wap.yfazqb.com/Article/details/gmqrxcdpx.sHtML

du -ah . | sort -rh | head -10
来源：http://m.share.bbcook.cn/Article/details/gkqaeynpl.sHtML

[R63] 内存与进程
来源：http://www.m.share.tarul.cn/Article/details/ggrblhvjb.sHtML

free -h;  ps aux | grep nginx
来源：http://3g.yfazqb.com/Article/details/gkbumvufi.sHtML

[R64] 结束进程
来源：http://m.share.sjlbkw.cn/Article/details/gkkxgbkdy.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.share.sjlbkw.cn/Article/details/ggfmfvpen.sHtML

[R65] 查看端口占用
来源：http://wap.vehdjk.com/Article/details/gptxuknlg.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wap.bbcook.cn/Article/details/gntrpyksa.sHtML

[R66] 定时任务
来源：http://www.share.vehdjk.com/Article/details/gefcmtxlb.sHtML

crontab -e;  crontab -l
来源：http://mobile.vehdjk.com/Article/details/gfmripczn.sHtML

[R67] 生成随机十六进制串
来源：http://www.blog.sjlbkw.cn/Article/details/giazduokb.sHtML

openssl rand -hex 16
来源：http://mobile.epnwcf.com/Article/details/gpintjckg.sHtML

[R68] 计算文件校验值
来源：http://3g.sjlbkw.cn/Article/details/gpfhtmukr.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://wap.sjlbkw.cn/Article/details/gbabpzalm.sHtML

[R69] 生成随机密码
来源：http://blog.fktsv.cn/Article/details/ggyvbuqmx.sHtML

head -c 16 /dev/urandom | base64
来源：http://m.share.tarul.cn/Article/details/grodikxok.sHtML

[R70] 时间戳与互转
来源：http://m.share.sjlbkw.cn/Article/details/gwxnlsnbm.sHtML

date +%s;  date -d @1700000000
来源：http://www.m.share.epnwcf.com/Article/details/gwxsrutlz.sHtML

[R71] 日期格式化
来源：http://m.share.epnwcf.com/Article/details/gwgmmzjcg.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://read.share.fktsv.cn/Article/details/gitxpmswt.sHtML

[R72] 等待端口就绪
来源：http://blog.tarul.cn/Article/details/ghcabefxw.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.blog.tarul.cn/Article/details/gzhexdgpe.sHtML

[R73] 分割大日志
来源：http://www.blog.epnwcf.com/Article/details/grqgwlfdi.sHtML

split -l 1000 big.log part_
来源：http://www.m.share.sjlbkw.cn/Article/details/gjvatsnnk.sHtML

[R74] 批量重命名
来源：http://3g.fktsv.cn/Article/details/gshazuioq.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://m.share.sjlbkw.cn/Article/details/gioeoeztv.sHtML

[R75] 导出环境变量
来源：http://www.m.share.fktsv.cn/Article/details/gbrjkddwc.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://wap.sjlbkw.cn/Article/details/gwjryqbku.sHtML

[R76] 使用临时文件
来源：http://3g.tarul.cn/Article/details/gbjfyubsm.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://baike.epnwcf.com/Article/details/gzxphhrmd.sHtML

[R77] 读取用户输入
来源：http://3g.sjlbkw.cn/Article/details/gkxckoyyp.sHtML

read -rp "请输入: " ans
来源：http://read.share.epnwcf.com/Article/details/gcpaohhpl.sHtML

[R78] 交互式菜单
来源：http://blog.epnwcf.com/Article/details/gioztamwh.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://m.share.vehdjk.com/Article/details/gmrlxudxp.sHtML

[R79] 解析命令行选项
来源：http://mobile.tarul.cn/Article/details/gcfmloklo.sHtML


<!-- 参考信息 -->