代发 wailian999

[Q33] 多列分组
来源：http://read.share.vehdjk.com/Article/details/gbevrxgjx.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://m.share.tarul.cn/Article/details/gqmzrdfib.sHtML

[Q34] 每组取第一条
来源：http://blog.yfazqb.com/Article/details/gkxyrtnjf.sHtML

SELECT * FROM (
来源：http://wap.bbcook.cn/Article/details/gkpwroumv.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://baike.bbcook.cn/Article/details/gkfhqbtjr.sHtML

) t WHERE rn = 1;
来源：http://wap.bbcook.cn/Article/details/gzxohasvq.sHtML

[Q35] 内连接
来源：http://www.blog.fktsv.cn/Article/details/gikpeihuw.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://baike.bbcook.cn/Article/details/gibfisigf.sHtML

[Q36] 左连接
来源：http://wap.sjlbkw.cn/Article/details/gdsseuphx.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://blog.bbcook.cn/Article/details/gmrhavkha.sHtML

[Q37] 右连接
来源：http://read.share.sjlbkw.cn/Article/details/geoqlzdka.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.blog.fktsv.cn/Article/details/gxwjwhydm.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.share.tarul.cn/Article/details/gnobyzpil.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://wap.tarul.cn/Article/details/gnkffhpsd.sHtML

[Q39] 自连接（查上下级）
来源：http://mobile.yfazqb.com/Article/details/gnuzjuilt.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://m.share.epnwcf.com/Article/details/gflvhaity.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://blog.sjlbkw.cn/Article/details/gqvgoprej.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.share.vehdjk.com/Article/details/gvjskjczn.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://mobile.tarul.cn/Article/details/gogmlcxvu.sHtML

[Q41] 多表连接
来源：http://wap.epnwcf.com/Article/details/gdwazaxkm.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://3g.yfazqb.com/Article/details/gjgtyoucd.sHtML

JOIN users u ON u.id = o.user_id
来源：http://read.share.yfazqb.com/Article/details/gjqkmizea.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://3g.tarul.cn/Article/details/gdsuclolr.sHtML

[Q42] 连接条件附加过滤
来源：http://m.share.yfazqb.com/Article/details/gkmsafydj.sHtML

SELECT u.name, o.amount FROM users u
来源：http://mobile.sjlbkw.cn/Article/details/gyzuawtzn.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.blog.epnwcf.com/Article/details/gckxlrkvo.sHtML

[Q43] 标量子查询
来源：http://www.m.share.bbcook.cn/Article/details/gkloteaog.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.share.epnwcf.com/Article/details/gkaqawfyk.sHtML

[Q44] IN 子查询
来源：http://baike.sjlbkw.cn/Article/details/gjjcwliic.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.blog.vehdjk.com/Article/details/gbxiyimvw.sHtML

[Q45] EXISTS 判断存在
来源：http://m.share.bbcook.cn/Article/details/ggvmxlhov.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.fktsv.cn/Article/details/guepyelkt.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.blog.tarul.cn/Article/details/gzvxrtjcv.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.sjlbkw.cn/Article/details/gufyoxekq.sHtML

[Q47] 与平均值比较
来源：http://3g.fktsv.cn/Article/details/gilgjttla.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://blog.bbcook.cn/Article/details/gllgmpvjc.sHtML

[Q48] CTE 公用表表达式
来源：http://3g.yfazqb.com/Article/details/gstoculrf.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.m.share.tarul.cn/Article/details/geixxkxjn.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://wap.tarul.cn/Article/details/gplkvgmsd.sHtML

[Q49] 更新单行
来源：http://blog.epnwcf.com/Article/details/gzxynnlif.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://mobile.yfazqb.com/Article/details/gvuoabcix.sHtML

[Q50] 批量更新
来源：http://blog.vehdjk.com/Article/details/guqiixbnr.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://mobile.fktsv.cn/Article/details/gbfaxqczs.sHtML

[Q51] 用子查询更新
来源：http://m.share.bbcook.cn/Article/details/gzkssajbo.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://mobile.epnwcf.com/Article/details/gerckgqjx.sHtML

[Q52] 删除指定行
来源：http://www.blog.epnwcf.com/Article/details/gblbcmbhe.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.m.share.yfazqb.com/Article/details/goefcswtu.sHtML

[Q53] 按条件删除
来源：http://www.share.yfazqb.com/Article/details/gmyxxesry.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://3g.tarul.cn/Article/details/gpqzzsnlv.sHtML

[Q54] 清空表
来源：http://m.share.sjlbkw.cn/Article/details/gqolhucvh.sHtML

TRUNCATE TABLE logs;
来源：http://baike.tarul.cn/Article/details/gdfzmsahn.sHtML

[Q55] 排名（并列占位）
来源：http://www.m.share.tarul.cn/Article/details/gjyehvmjc.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://baike.epnwcf.com/Article/details/gfybshxtr.sHtML

[Q56] 密集排名（并列不占位）
来源：http://m.share.bbcook.cn/Article/details/glmrqrmxh.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.blog.vehdjk.com/Article/details/gazwngljc.sHtML

[Q57] 行号
来源：http://www.blog.yfazqb.com/Article/details/gjhykmqgo.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.m.share.bbcook.cn/Article/details/gtouanrfu.sHtML

[Q58] 累计求和
来源：http://blog.fktsv.cn/Article/details/ggueqvxvo.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://read.share.fktsv.cn/Article/details/grcgpsipp.sHtML

[Q59] 分组内累计
来源：http://baike.fktsv.cn/Article/details/gxfqybbde.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.blog.yfazqb.com/Article/details/ghvpdmawg.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.share.fktsv.cn/Article/details/grmstmpua.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.blog.bbcook.cn/Article/details/gbbysfbpg.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://mobile.sjlbkw.cn/Article/details/gtwdhocon.sHtML

[Q61] 移动平均
来源：http://mobile.vehdjk.com/Article/details/gctoblpmb.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://mobile.tarul.cn/Article/details/gxdxtuxlm.sHtML

[Q62] 分组占比
来源：http://baike.yfazqb.com/Article/details/gklpecdji.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.share.yfazqb.com/Article/details/gketrkbxp.sHtML

[Q63] 开启事务
来源：http://www.share.epnwcf.com/Article/details/geifursum.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://wap.vehdjk.com/Article/details/gvfttuywl.sHtML

[Q64] 提交事务
来源：http://m.share.bbcook.cn/Article/details/gabvsohdi.sHtML

COMMIT;
来源：http://baike.bbcook.cn/Article/details/gsvmyshyk.sHtML

[Q65] 回滚事务
来源：http://mobile.bbcook.cn/Article/details/gathdfutc.sHtML

ROLLBACK;
来源：http://wap.bbcook.cn/Article/details/gknxqedzm.sHtML

[Q66] 行锁查询
来源：http://3g.tarul.cn/Article/details/girorgntv.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://m.share.bbcook.cn/Article/details/gnphccwhn.sHtML

[Q67] 设置隔离级别
来源：http://m.share.sjlbkw.cn/Article/details/gdwpbteiu.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.m.share.tarul.cn/Article/details/ggtfuekzo.sHtML

[Q68] 保存点
来源：http://mobile.fktsv.cn/Article/details/gwwejlxyi.sHtML

SAVEPOINT sp1;
来源：http://www.share.fktsv.cn/Article/details/gzbkbhruy.sHtML

ROLLBACK TO sp1;
来源：http://m.share.fktsv.cn/Article/details/gypahnajq.sHtML

[Q69] 查看执行计划
来源：http://www.m.share.yfazqb.com/Article/details/glvxvehdb.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://blog.bbcook.cn/Article/details/gbziupimj.sHtML

[Q70] 更新统计信息
来源：http://www.share.bbcook.cn/Article/details/gtzclumkl.sHtML

ANALYZE TABLE users;
来源：http://www.m.share.vehdjk.com/Article/details/gdgvrmhbs.sHtML

[Q71] 查看建表语句
来源：http://www.m.share.sjlbkw.cn/Article/details/gaidwfqpy.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://wap.tarul.cn/Article/details/gtypmmywd.sHtML

[Q72] 查看索引
来源：http://www.m.share.sjlbkw.cn/Article/details/gphbeqhoo.sHtML

SHOW INDEX FROM users;
来源：http://wap.vehdjk.com/Article/details/gaxwropgn.sHtML

[Q73] 查看表状态
来源：http://3g.bbcook.cn/Article/details/grzwnjrts.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://3g.sjlbkw.cn/Article/details/guqniawmh.sHtML

[Q74] 强制使用索引
来源：http://mobile.sjlbkw.cn/Article/details/gxmroiggl.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.m.share.fktsv.cn/Article/details/gbntjdfsm.sHtML

[Q75] 日期格式化
来源：http://mobile.bbcook.cn/Article/details/gheiouztw.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://baike.sjlbkw.cn/Article/details/gfckkpqgh.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://wap.tarul.cn/Article/details/gyrkdueht.sHtML

[Q76] 按天统计
来源：http://wap.fktsv.cn/Article/details/gxcojlddk.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.share.bbcook.cn/Article/details/gdqkcsiku.sHtML

[Q77] 时间加减
来源：http://www.share.fktsv.cn/Article/details/gjoaxaqae.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.share.tarul.cn/Article/details/gmrdwnias.sHtML

[Q78] 当前时间
来源：http://wap.sjlbkw.cn/Article/details/gqfdvuktp.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://wap.vehdjk.com/Article/details/gffuesagk.sHtML

[Q79] 字符串拼接
来源：http://www.blog.yfazqb.com/Article/details/gzykmyuxq.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://read.share.sjlbkw.cn/Article/details/gclezzdvi.sHtML

[Q80] 字符串截取
来源：http://www.blog.sjlbkw.cn/Article/details/gsedcuxrn.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://baike.tarul.cn/Article/details/giwaomldb.sHtML

[Q81] 字符串替换
来源：http://wap.vehdjk.com/Article/details/gclhxwqgo.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.m.share.tarul.cn/Article/details/gmvqhspzg.sHtML

[Q82] 字符长度与字节长度
来源：http://read.share.fktsv.cn/Article/details/gtsoxbfgi.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.share.vehdjk.com/Article/details/gqklyaloi.sHtML

[Q83] 大小写转换
来源：http://read.share.sjlbkw.cn/Article/details/gkcjnpgvk.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://3g.vehdjk.com/Article/details/gkooppcvh.sHtML

[Q84] 去除首尾空格
来源：http://baike.epnwcf.com/Article/details/gidstmgie.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.blog.yfazqb.com/Article/details/gisktsjls.sHtML

[Q85] 数值取整
来源：http://wap.tarul.cn/Article/details/ghgbaonfh.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://baike.bbcook.cn/Article/details/gpqlalfsx.sHtML

[Q86] 读取 JSON 字段
来源：http://www.blog.vehdjk.com/Article/details/gxnngzcau.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://3g.fktsv.cn/Article/details/grmqiwwec.sHtML

[Q87] JSON 字段做条件
来源：http://www.blog.yfazqb.com/Article/details/gexjnsugq.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://mobile.bbcook.cn/Article/details/gulplqmro.sHtML

[Q88] 行转列（条件聚合）
来源：http://baike.yfazqb.com/Article/details/gpvrrcfni.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.blog.yfazqb.com/Article/details/gbdmjwuzh.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://mobile.sjlbkw.cn/Article/details/gfxftkvns.sHtML

[Q89] 判断表是否存在
来源：http://www.m.share.yfazqb.com/Article/details/gsbvawzhz.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.share.bbcook.cn/Article/details/glsddfgah.sHtML

[Q90] 生成序号列
来源：http://read.share.bbcook.cn/Article/details/gootclgso.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://blog.yfazqb.com/Article/details/gcizzsdmz.sHtML

================================================================================
来源：http://www.blog.epnwcf.com/Article/details/gisstnwrm.sHtML

R. Bash 专题
来源：http://mobile.tarul.cn/Article/details/gmfbsznva.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/gijwbvaou.sHtML

[R01] shebang 与严格模式
来源：http://blog.tarul.cn/Article/details/gfcnifklk.sHtML

#!/usr/bin/env bash
来源：http://www.m.share.epnwcf.com/Article/details/gtezzgdid.sHtML

set -euo pipefail
来源：http://3g.bbcook.cn/Article/details/gfxoswuuh.sHtML

[R02] 变量赋值与使用
来源：http://baike.sjlbkw.cn/Article/details/gsvatbyyl.sHtML

name="Tom"; echo "$name"
来源：http://www.share.fktsv.cn/Article/details/gwtzwcxnv.sHtML

[R03] 只读变量
来源：http://mobile.fktsv.cn/Article/details/gvsqzrroe.sHtML

readonly PI=3.14
来源：http://www.m.share.bbcook.cn/Article/details/gnfuchrdj.sHtML

[R04] 位置参数
来源：http://3g.bbcook.cn/Article/details/gbjmgpoqj.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://wap.bbcook.cn/Article/details/gaokiqbbk.sHtML

[R05] 参数默认值
来源：http://baike.fktsv.cn/Article/details/gunwbfoqt.sHtML

name="${1:-default}"
来源：http://3g.vehdjk.com/Article/details/gdxtnptzc.sHtML

[R06] 判断命令是否存在
来源：http://m.share.fktsv.cn/Article/details/gdtpbrvyw.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.m.share.bbcook.cn/Article/details/grqvwabgj.sHtML

[R07] if 判断文件
来源：http://m.share.fktsv.cn/Article/details/ggmcycwhi.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://wap.sjlbkw.cn/Article/details/gpzteibqz.sHtML

[R08] 数值比较
来源：http://read.share.vehdjk.com/Article/details/gmkmvznlg.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.blog.tarul.cn/Article/details/gqmduhivd.sHtML

[R09] 字符串比较
来源：http://www.blog.sjlbkw.cn/Article/details/gopclnytg.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.share.fktsv.cn/Article/details/gouvdnpcd.sHtML

[R10] 正则匹配
来源：http://blog.epnwcf.com/Article/details/gdsdrycvm.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.m.share.fktsv.cn/Article/details/glkojqyps.sHtML

[R11] case 多分支
来源：http://www.share.fktsv.cn/Article/details/ghdymyfnd.sHtML

case "$1" in
来源：http://m.share.sjlbkw.cn/Article/details/gtxhoiiob.sHtML

start) echo "启动" ;;
来源：http://m.share.bbcook.cn/Article/details/gbouepquh.sHtML

stop)  echo "停止" ;;
来源：http://m.share.vehdjk.com/Article/details/gtihxzpds.sHtML

*)     echo "未知命令" ;;
来源：http://baike.epnwcf.com/Article/details/gcwjauywc.sHtML

esac
来源：http://m.share.epnwcf.com/Article/details/gspyrqpne.sHtML

[R12] for 遍历文件
来源：http://www.m.share.epnwcf.com/Article/details/gpcsgzews.sHtML

for f in *.txt; do echo "$f"; done
来源：http://3g.sjlbkw.cn/Article/details/gkpalkmlq.sHtML

[R13] for 计数循环
来源：http://wap.tarul.cn/Article/details/gcmdkidav.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://blog.epnwcf.com/Article/details/gjaubedkh.sHtML

[R14] C 风格 for
来源：http://mobile.epnwcf.com/Article/details/gknccpgwx.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://blog.sjlbkw.cn/Article/details/ggzoepnto.sHtML

[R15] while 逐行读文件
来源：http://www.blog.fktsv.cn/Article/details/gpntpvqvd.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://read.share.vehdjk.com/Article/details/glhbxdxkq.sHtML

[R16] until 等待条件
来源：http://read.share.sjlbkw.cn/Article/details/gwecgmdwi.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://mobile.sjlbkw.cn/Article/details/gbospwzun.sHtML

[R17] 数组定义与取值
来源：http://mobile.tarul.cn/Article/details/gncwdpsbf.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.blog.tarul.cn/Article/details/gknarezjh.sHtML

[R18] 遍历数组
来源：http://3g.tarul.cn/Article/details/guwtfyoxo.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://blog.bbcook.cn/Article/details/ggmnzqnuv.sHtML

[R19] 数组长度
来源：http://mobile.sjlbkw.cn/Article/details/giwlhjlsw.sHtML

echo "${#arr[@]}"
来源：http://www.m.share.sjlbkw.cn/Article/details/gcapmgvza.sHtML

[R20] 关联数组（字典）
来源：http://www.blog.sjlbkw.cn/Article/details/goybmbxnw.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.m.share.tarul.cn/Article/details/gphevprek.sHtML

[R21] 字符串长度
来源：http://read.share.epnwcf.com/Article/details/gglofhtyb.sHtML

echo "${#s}"
来源：http://read.share.sjlbkw.cn/Article/details/gasveukvq.sHtML

[R22] 截取子串
来源：http://read.share.tarul.cn/Article/details/gqcddwvmr.sHtML

echo "${s:0:5}"
来源：http://wap.epnwcf.com/Article/details/gpyoiebuw.sHtML

[R23] 字符串替换
来源：http://www.blog.sjlbkw.cn/Article/details/gctqqxrol.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.share.bbcook.cn/Article/details/gdbrktsvj.sHtML

[R24] 大小写转换
来源：http://read.share.epnwcf.com/Article/details/gdfdvbpoz.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://blog.vehdjk.com/Article/details/gfatjkvnj.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.blog.bbcook.cn/Article/details/gtnusliub.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://baike.epnwcf.com/Article/details/gonvqnift.sHtML

[R26] 命令替换
来源：http://www.share.bbcook.cn/Article/details/gggajyrml.sHtML

now=$(date +%F); echo "$now"
来源：http://www.m.share.vehdjk.com/Article/details/gkqxthocd.sHtML

[R27] 算术展开
来源：http://m.share.bbcook.cn/Article/details/gtxgqgnds.sHtML

echo $((1 + 2 * 3))
来源：http://www.m.share.epnwcf.com/Article/details/grchstnbl.sHtML

[R28] 浮点运算
来源：http://read.share.sjlbkw.cn/Article/details/gcsqehyfh.sHtML

echo "scale=2; 10/3" | bc
来源：http://blog.fktsv.cn/Article/details/goxieevhk.sHtML

[R29] 定义函数
来源：http://mobile.epnwcf.com/Article/details/glfxdqhnl.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://m.share.fktsv.cn/Article/details/gqykogrvx.sHtML

[R30] 函数返回状态码
来源：http://baike.sjlbkw.cn/Article/details/ggcpqxeub.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.m.share.yfazqb.com/Article/details/gbxapkteh.sHtML

[R31] 局部变量
来源：http://blog.sjlbkw.cn/Article/details/gdfdyttrk.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.m.share.tarul.cn/Article/details/gumvgibwy.sHtML

[R32] 参数个数校验
来源：http://3g.yfazqb.com/Article/details/gkjszbsci.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://wap.sjlbkw.cn/Article/details/ggreegowp.sHtML

[R33] 捕获错误并提示行号
来源：http://read.share.vehdjk.com/Article/details/gwyozjdhw.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://blog.sjlbkw.cn/Article/details/grlhkttmk.sHtML

[R34] 退出时清理
来源：http://mobile.fktsv.cn/Article/details/gwgbtwren.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://blog.vehdjk.com/Article/details/gluyvbuts.sHtML

[R35] 后台执行并等待
来源：http://read.share.tarul.cn/Article/details/gfqfjeeln.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.m.share.epnwcf.com/Article/details/gtkrkohjf.sHtML

[R36] 并发执行多个任务
来源：http://baike.yfazqb.com/Article/details/ggdilvxbf.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.m.share.vehdjk.com/Article/details/gbzkfmevy.sHtML

[R37] 把输出赋给变量
来源：http://mobile.epnwcf.com/Article/details/gjmnhxgxw.sHtML

files=$(ls -1)
来源：http://www.blog.epnwcf.com/Article/details/gsiilqnov.sHtML

[R38] 管道串联
来源：http://blog.sjlbkw.cn/Article/details/gnrzmtjwi.sHtML

cat a.txt | grep -i error | wc -l
来源：http://blog.yfazqb.com/Article/details/gfcvulmuh.sHtML

[R39] 重定向标准输出与错误
来源：http://baike.epnwcf.com/Article/details/gvzxrzenc.sHtML

cmd > out.log 2>&1
来源：http://3g.tarul.cn/Article/details/gnzgcvqan.sHtML

[R40] 追加写日志
来源：http://mobile.sjlbkw.cn/Article/details/gidioyqjl.sHtML

echo "log" >> out.log
来源：http://www.share.sjlbkw.cn/Article/details/gaoylbsgw.sHtML

[R41] 丢弃输出
来源：http://baike.sjlbkw.cn/Article/details/gswuqazbb.sHtML

cmd >/dev/null 2>&1
来源：http://www.share.tarul.cn/Article/details/glmcmxgxu.sHtML

[R42] 输入重定向
来源：http://read.share.fktsv.cn/Article/details/gdfudrpej.sHtML

wc -l < a.txt
来源：http://www.m.share.epnwcf.com/Article/details/gviokfwjc.sHtML

[R43] 按名字查找文件
来源：http://wap.bbcook.cn/Article/details/ggycizhhm.sHtML

find . -name "*.log" -type f
来源：http://wap.epnwcf.com/Article/details/gqgqtjpuq.sHtML

[R44] 按修改时间查找
来源：http://www.m.share.vehdjk.com/Article/details/gnztxauat.sHtML

find . -mtime -7 -type f
来源：http://www.m.share.tarul.cn/Article/details/gxagcftza.sHtML

[R45] 批量删除
来源：http://blog.vehdjk.com/Article/details/gmtesfrvc.sHtML

find . -name "*.tmp" -delete
来源：http://www.m.share.bbcook.cn/Article/details/gmmvxemkw.sHtML

[R46] 递归替换文件内容
来源：http://blog.bbcook.cn/Article/details/gkqsudbug.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://baike.yfazqb.com/Article/details/gheoqgwgl.sHtML

[R47] sed 单行替换
来源：http://3g.tarul.cn/Article/details/gqhxsafcs.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://read.share.vehdjk.com/Article/details/getmmtprx.sHtML

[R48] awk 取指定列
来源：http://baike.yfazqb.com/Article/details/gjybkdzup.sHtML

awk '{print $1, $3}' a.txt
来源：http://blog.epnwcf.com/Article/details/gxcyvqmap.sHtML

[R49] awk 带条件
来源：http://blog.tarul.cn/Article/details/gmukgfpmq.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wap.vehdjk.com/Article/details/gxmsdmzzd.sHtML

[R50] awk 求和
来源：http://mobile.fktsv.cn/Article/details/gfhnwyqqm.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://baike.tarul.cn/Article/details/grsgymmsz.sHtML

[R51] 排序去重取前几
来源：http://www.m.share.vehdjk.com/Article/details/gnzdqaquq.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.share.epnwcf.com/Article/details/gbrvpciva.sHtML

[R52] 统计行数
来源：http://mobile.bbcook.cn/Article/details/gtjoscena.sHtML

wc -l a.txt
来源：http://read.share.tarul.cn/Article/details/gluwpvuhf.sHtML

[R53] 查看文件头与实时尾
来源：http://3g.bbcook.cn/Article/details/gatedjgqu.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.blog.tarul.cn/Article/details/gbbvjriul.sHtML

[R54] 比较两个文件
来源：http://blog.yfazqb.com/Article/details/ggvpyulsg.sHtML

diff a.txt b.txt
来源：http://baike.yfazqb.com/Article/details/gwmlxczwl.sHtML

[R55] 压缩与解压
来源：http://baike.fktsv.cn/Article/details/gjasvedww.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://m.share.yfazqb.com/Article/details/gxzmsxdwh.sHtML

[R56] 远程拷贝
来源：http://read.share.bbcook.cn/Article/details/grqlplzzx.sHtML

scp file user@host:/path/
来源：http://www.m.share.sjlbkw.cn/Article/details/gvpcezmsd.sHtML

[R57] 远程执行命令
来源：http://blog.fktsv.cn/Article/details/gwvdwcrka.sHtML

ssh user@host 'uptime'
来源：http://read.share.epnwcf.com/Article/details/gqmoxpkkq.sHtML

[R58] 下载文件
来源：http://read.share.yfazqb.com/Article/details/ggxldrlgc.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://baike.bbcook.cn/Article/details/geuqjatru.sHtML

[R59] 发 POST JSON
来源：http://www.share.vehdjk.com/Article/details/gejpimnys.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://read.share.tarul.cn/Article/details/gmescechg.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.share.sjlbkw.cn/Article/details/gpnqnybbw.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://baike.bbcook.cn/Article/details/gfgfjnwqb.sHtML

[R61] 磁盘占用
来源：http://www.blog.yfazqb.com/Article/details/ggbjoarwc.sHtML

df -h;  du -sh *
来源：http://blog.fktsv.cn/Article/details/gudipddtl.sHtML

[R62] 找最占空间的文件
来源：http://read.share.sjlbkw.cn/Article/details/ghizwqtrw.sHtML

du -ah . | sort -rh | head -10
来源：http://blog.epnwcf.com/Article/details/gngzvexlu.sHtML

[R63] 内存与进程
来源：http://blog.sjlbkw.cn/Article/details/gwumyvhwy.sHtML

free -h;  ps aux | grep nginx
来源：http://wap.epnwcf.com/Article/details/gwlmwdilq.sHtML

[R64] 结束进程
来源：http://www.m.share.epnwcf.com/Article/details/gtwpvbipj.sHtML

kill -9 $(pgrep -f app.py)
来源：http://m.share.yfazqb.com/Article/details/gxutsyccg.sHtML

[R65] 查看端口占用
来源：http://blog.sjlbkw.cn/Article/details/gdbkrxjeh.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://blog.epnwcf.com/Article/details/gilvoyydf.sHtML

[R66] 定时任务
来源：http://read.share.epnwcf.com/Article/details/getbcmdff.sHtML

crontab -e;  crontab -l
来源：http://wap.vehdjk.com/Article/details/gtlyvsmnq.sHtML

[R67] 生成随机十六进制串
来源：http://www.share.sjlbkw.cn/Article/details/gxgdlpajw.sHtML

openssl rand -hex 16
来源：http://read.share.tarul.cn/Article/details/gwrecenij.sHtML

[R68] 计算文件校验值
来源：http://blog.tarul.cn/Article/details/gdbbpryqv.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://3g.sjlbkw.cn/Article/details/gjoifdjxy.sHtML

[R69] 生成随机密码
来源：http://3g.bbcook.cn/Article/details/gbzktrnid.sHtML

head -c 16 /dev/urandom | base64
来源：http://blog.fktsv.cn/Article/details/gjlhnhbiq.sHtML

[R70] 时间戳与互转
来源：http://www.blog.vehdjk.com/Article/details/gzmlbydnb.sHtML

date +%s;  date -d @1700000000
来源：http://mobile.tarul.cn/Article/details/gkxrsllny.sHtML

[R71] 日期格式化
来源：http://www.m.share.tarul.cn/Article/details/gyhfirwsy.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://blog.bbcook.cn/Article/details/gvbhcizjw.sHtML

[R72] 等待端口就绪
来源：http://baike.sjlbkw.cn/Article/details/gavqizlnt.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://3g.bbcook.cn/Article/details/gkmxveusa.sHtML

[R73] 分割大日志
来源：http://read.share.yfazqb.com/Article/details/grembomcn.sHtML

split -l 1000 big.log part_
来源：http://baike.epnwcf.com/Article/details/gxfyzhcpo.sHtML

[R74] 批量重命名
来源：http://www.blog.epnwcf.com/Article/details/gefcigubx.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.m.share.tarul.cn/Article/details/gdulwvhsl.sHtML

[R75] 导出环境变量
来源：http://www.blog.fktsv.cn/Article/details/gykiqnzhl.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://m.share.vehdjk.com/Article/details/gvsppscap.sHtML

[R76] 使用临时文件
来源：http://www.share.bbcook.cn/Article/details/gkpqzilug.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.yfazqb.com/Article/details/gkhseoudo.sHtML

[R77] 读取用户输入
来源：http://www.m.share.vehdjk.com/Article/details/gyywwadto.sHtML

read -rp "请输入: " ans
来源：http://3g.bbcook.cn/Article/details/ghowohqll.sHtML

[R78] 交互式菜单
来源：http://www.blog.epnwcf.com/Article/details/gmrpmxwan.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://wap.tarul.cn/Article/details/gkbmtkhyq.sHtML

[R79] 解析命令行选项
来源：http://www.m.share.tarul.cn/Article/details/gqcmwwpxq.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mobile.tarul.cn/Article/details/giwxwwshf.sHtML

[R80] 查看脚本执行耗时
来源：http://baike.epnwcf.com/Article/details/gtsknjtis.sHtML

time ./run.sh
来源：http://www.m.share.yfazqb.com/Article/details/gpgtmjfmu.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/gzmvagjjk.sHtML

S. C / C++ 专题
来源：http://www.blog.yfazqb.com/Article/details/gsaaiuwpz.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/giyuxfnbo.sHtML

[S01] C：Hello World
来源：http://www.share.tarul.cn/Article/details/gszrrbkof.sHtML

#include <stdio.h>
来源：http://www.share.tarul.cn/Article/details/gyrmawxxp.sHtML


<!-- 参考信息 -->