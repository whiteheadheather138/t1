代发 wailian999

[Q36] 左连接
来源：http://www.blog.fktsv.cn/Article/details/gerbzkuwr.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://baike.vehdjk.com/Article/details/gcchewvjr.sHtML

[Q37] 右连接
来源：http://www.blog.sjlbkw.cn/Article/details/grpiiqukb.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://baike.fktsv.cn/Article/details/gahrqukbt.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://wap.epnwcf.com/Article/details/gmeymqnoi.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.m.share.bbcook.cn/Article/details/gdfrevqnt.sHtML

[Q39] 自连接（查上下级）
来源：http://wap.yfazqb.com/Article/details/gzmmvtwzk.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://read.share.yfazqb.com/Article/details/glseeefpq.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://read.share.yfazqb.com/Article/details/gadjpdemh.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://m.share.sjlbkw.cn/Article/details/gjnhgfadz.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://m.share.sjlbkw.cn/Article/details/ghntexbak.sHtML

[Q41] 多表连接
来源：http://m.share.bbcook.cn/Article/details/gfiitmthk.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://blog.vehdjk.com/Article/details/gqkznmeux.sHtML

JOIN users u ON u.id = o.user_id
来源：http://read.share.sjlbkw.cn/Article/details/gtnkqfryl.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://blog.sjlbkw.cn/Article/details/gngdlfgff.sHtML

[Q42] 连接条件附加过滤
来源：http://www.share.yfazqb.com/Article/details/gsxpjjdeu.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.share.bbcook.cn/Article/details/grhbobqrs.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.m.share.epnwcf.com/Article/details/gcrgsxzyo.sHtML

[Q43] 标量子查询
来源：http://3g.vehdjk.com/Article/details/gtjbzeocv.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.blog.tarul.cn/Article/details/gvxedvqpt.sHtML

[Q44] IN 子查询
来源：http://read.share.tarul.cn/Article/details/gfkslgxrs.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://m.share.fktsv.cn/Article/details/guyccxssb.sHtML

[Q45] EXISTS 判断存在
来源：http://m.share.fktsv.cn/Article/details/gedowvfix.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.vehdjk.com/Article/details/gwizzzbjp.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.blog.yfazqb.com/Article/details/gzhamawqx.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.fktsv.cn/Article/details/gzubsdort.sHtML

[Q47] 与平均值比较
来源：http://m.share.vehdjk.com/Article/details/gnncgmqcb.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://m.share.fktsv.cn/Article/details/giruqyzhj.sHtML

[Q48] CTE 公用表表达式
来源：http://baike.sjlbkw.cn/Article/details/gcppsombk.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.blog.sjlbkw.cn/Article/details/gzueaqacn.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://m.share.bbcook.cn/Article/details/gdvuksoku.sHtML

[Q49] 更新单行
来源：http://3g.vehdjk.com/Article/details/gndblvlej.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.blog.bbcook.cn/Article/details/gcnslrauv.sHtML

[Q50] 批量更新
来源：http://baike.fktsv.cn/Article/details/gfguxayqx.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://read.share.fktsv.cn/Article/details/gelbhfsha.sHtML

[Q51] 用子查询更新
来源：http://mobile.vehdjk.com/Article/details/gtovoikhh.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://3g.bbcook.cn/Article/details/gexxauhae.sHtML

[Q52] 删除指定行
来源：http://www.m.share.sjlbkw.cn/Article/details/gtfqrjzyn.sHtML

DELETE FROM users WHERE id = 10;
来源：http://blog.fktsv.cn/Article/details/gmuffqwdw.sHtML

[Q53] 按条件删除
来源：http://www.m.share.yfazqb.com/Article/details/grijspkhp.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://mobile.yfazqb.com/Article/details/gkevmwrdi.sHtML

[Q54] 清空表
来源：http://read.share.bbcook.cn/Article/details/gcxtxjxqh.sHtML

TRUNCATE TABLE logs;
来源：http://3g.tarul.cn/Article/details/gnkdudyxz.sHtML

[Q55] 排名（并列占位）
来源：http://m.share.fktsv.cn/Article/details/gjzftnpjj.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://3g.vehdjk.com/Article/details/gggslpajk.sHtML

[Q56] 密集排名（并列不占位）
来源：http://m.share.fktsv.cn/Article/details/gxndrbftg.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.share.yfazqb.com/Article/details/giaexfhwc.sHtML

[Q57] 行号
来源：http://www.m.share.bbcook.cn/Article/details/gazqavtfj.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://blog.tarul.cn/Article/details/ghsbztawx.sHtML

[Q58] 累计求和
来源：http://www.m.share.yfazqb.com/Article/details/ggltcxbuw.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://read.share.tarul.cn/Article/details/gkbzglhrs.sHtML

[Q59] 分组内累计
来源：http://baike.yfazqb.com/Article/details/gphphiaok.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://baike.tarul.cn/Article/details/govisewui.sHtML

[Q60] 取上一行 / 下一行
来源：http://baike.fktsv.cn/Article/details/gvvqaykid.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://3g.yfazqb.com/Article/details/gjsgmlvjy.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.m.share.yfazqb.com/Article/details/guqyhohjt.sHtML

[Q61] 移动平均
来源：http://m.share.bbcook.cn/Article/details/grszwibge.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.m.share.tarul.cn/Article/details/gbeivzcqk.sHtML

[Q62] 分组占比
来源：http://www.m.share.sjlbkw.cn/Article/details/gehrtihrm.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://3g.sjlbkw.cn/Article/details/gydeoesap.sHtML

[Q63] 开启事务
来源：http://www.m.share.epnwcf.com/Article/details/gbutcxskk.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://blog.yfazqb.com/Article/details/gqcaxjyki.sHtML

[Q64] 提交事务
来源：http://3g.vehdjk.com/Article/details/gpnvbqaej.sHtML

COMMIT;
来源：http://3g.epnwcf.com/Article/details/gozcoitiq.sHtML

[Q65] 回滚事务
来源：http://www.share.tarul.cn/Article/details/gvmsqbpbg.sHtML

ROLLBACK;
来源：http://3g.fktsv.cn/Article/details/gzcarbbtj.sHtML

[Q66] 行锁查询
来源：http://m.share.bbcook.cn/Article/details/gxidbluso.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.share.fktsv.cn/Article/details/gymwcgxbi.sHtML

[Q67] 设置隔离级别
来源：http://www.m.share.sjlbkw.cn/Article/details/gcuhblidr.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://mobile.sjlbkw.cn/Article/details/gcgnqwfyg.sHtML

[Q68] 保存点
来源：http://m.share.epnwcf.com/Article/details/gguazmozu.sHtML

SAVEPOINT sp1;
来源：http://mobile.fktsv.cn/Article/details/gpbagafoo.sHtML

ROLLBACK TO sp1;
来源：http://read.share.sjlbkw.cn/Article/details/gjqvhmfnm.sHtML

[Q69] 查看执行计划
来源：http://baike.bbcook.cn/Article/details/guutpblew.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.m.share.yfazqb.com/Article/details/gxuhyydyk.sHtML

[Q70] 更新统计信息
来源：http://m.share.yfazqb.com/Article/details/gfstdazxm.sHtML

ANALYZE TABLE users;
来源：http://wap.vehdjk.com/Article/details/gqokapbmr.sHtML

[Q71] 查看建表语句
来源：http://m.share.fktsv.cn/Article/details/gxxazcfxm.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://mobile.tarul.cn/Article/details/gxfvlwkmp.sHtML

[Q72] 查看索引
来源：http://m.share.vehdjk.com/Article/details/glnlrrcml.sHtML

SHOW INDEX FROM users;
来源：http://wap.sjlbkw.cn/Article/details/gozalpdrj.sHtML

[Q73] 查看表状态
来源：http://3g.sjlbkw.cn/Article/details/gsukimclb.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://read.share.sjlbkw.cn/Article/details/gmvqzacee.sHtML

[Q74] 强制使用索引
来源：http://baike.sjlbkw.cn/Article/details/ggrtmahas.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://blog.epnwcf.com/Article/details/godhxlmpo.sHtML

[Q75] 日期格式化
来源：http://mobile.fktsv.cn/Article/details/gvemqicwr.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://read.share.epnwcf.com/Article/details/giafnnjxt.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://baike.tarul.cn/Article/details/gtukeqrcr.sHtML

[Q76] 按天统计
来源：http://www.share.bbcook.cn/Article/details/gxhffsllc.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.blog.epnwcf.com/Article/details/gghpwqizz.sHtML

[Q77] 时间加减
来源：http://www.blog.vehdjk.com/Article/details/gmcbvcjjo.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://blog.tarul.cn/Article/details/gteolcmyr.sHtML

[Q78] 当前时间
来源：http://www.share.tarul.cn/Article/details/gcjqrchbz.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://m.share.epnwcf.com/Article/details/gcfzxlkok.sHtML

[Q79] 字符串拼接
来源：http://blog.bbcook.cn/Article/details/ggbafgtag.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://blog.fktsv.cn/Article/details/gpgwznjgb.sHtML

[Q80] 字符串截取
来源：http://mobile.tarul.cn/Article/details/gnwaibbza.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://3g.epnwcf.com/Article/details/gajhqzvfw.sHtML

[Q81] 字符串替换
来源：http://m.share.bbcook.cn/Article/details/gbljlnfnw.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://mobile.epnwcf.com/Article/details/girbutnsg.sHtML

[Q82] 字符长度与字节长度
来源：http://www.share.vehdjk.com/Article/details/gyfufsgiy.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.share.vehdjk.com/Article/details/gfcchyxzq.sHtML

[Q83] 大小写转换
来源：http://baike.tarul.cn/Article/details/giewhjlfn.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://baike.yfazqb.com/Article/details/goldkdcal.sHtML

[Q84] 去除首尾空格
来源：http://read.share.vehdjk.com/Article/details/gxajhdlza.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.blog.vehdjk.com/Article/details/ggaxnhsyz.sHtML

[Q85] 数值取整
来源：http://baike.sjlbkw.cn/Article/details/gtswhkaul.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://baike.fktsv.cn/Article/details/gldgqvjkv.sHtML

[Q86] 读取 JSON 字段
来源：http://baike.sjlbkw.cn/Article/details/gcpptljuz.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.share.sjlbkw.cn/Article/details/gmkhybxff.sHtML

[Q87] JSON 字段做条件
来源：http://wap.sjlbkw.cn/Article/details/giqicjdde.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://wap.epnwcf.com/Article/details/gbeyiugoq.sHtML

[Q88] 行转列（条件聚合）
来源：http://mobile.vehdjk.com/Article/details/gfuoihvfb.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://3g.tarul.cn/Article/details/gdquyykyp.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://mobile.tarul.cn/Article/details/gevdyedou.sHtML

[Q89] 判断表是否存在
来源：http://read.share.tarul.cn/Article/details/gkcaoovsa.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://m.share.yfazqb.com/Article/details/gdphxipyy.sHtML

[Q90] 生成序号列
来源：http://wap.tarul.cn/Article/details/gmukpxsxo.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.blog.bbcook.cn/Article/details/gnbhbldsj.sHtML

================================================================================
来源：http://3g.vehdjk.com/Article/details/glhlcwcjz.sHtML

R. Bash 专题
来源：http://mobile.epnwcf.com/Article/details/gyvkshsgt.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/gbznpfpgh.sHtML

[R01] shebang 与严格模式
来源：http://baike.yfazqb.com/Article/details/gxdkreetp.sHtML

#!/usr/bin/env bash
来源：http://m.share.sjlbkw.cn/Article/details/guivxbpyk.sHtML

set -euo pipefail
来源：http://blog.bbcook.cn/Article/details/gmdzyoxzl.sHtML

[R02] 变量赋值与使用
来源：http://m.share.fktsv.cn/Article/details/gyrdkybcw.sHtML

name="Tom"; echo "$name"
来源：http://m.share.fktsv.cn/Article/details/gkqyeeigm.sHtML

[R03] 只读变量
来源：http://3g.sjlbkw.cn/Article/details/gxnptbrfc.sHtML

readonly PI=3.14
来源：http://baike.bbcook.cn/Article/details/gihwonrnz.sHtML

[R04] 位置参数
来源：http://baike.fktsv.cn/Article/details/ghktvouoo.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://baike.sjlbkw.cn/Article/details/ggyndlvdg.sHtML

[R05] 参数默认值
来源：http://read.share.tarul.cn/Article/details/gtlxbiygp.sHtML

name="${1:-default}"
来源：http://3g.tarul.cn/Article/details/gikwhverf.sHtML

[R06] 判断命令是否存在
来源：http://www.share.bbcook.cn/Article/details/gfmqhyagm.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://m.share.fktsv.cn/Article/details/ggkhmvtpr.sHtML

[R07] if 判断文件
来源：http://baike.vehdjk.com/Article/details/gxzepfknk.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://blog.bbcook.cn/Article/details/gvmmhqcdc.sHtML

[R08] 数值比较
来源：http://www.blog.fktsv.cn/Article/details/gcrlhojxf.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.m.share.bbcook.cn/Article/details/gyoaacxrx.sHtML

[R09] 字符串比较
来源：http://blog.tarul.cn/Article/details/gjmmtlcts.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://m.share.sjlbkw.cn/Article/details/grtizqhnh.sHtML

[R10] 正则匹配
来源：http://blog.sjlbkw.cn/Article/details/gvlhnfdga.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://wap.sjlbkw.cn/Article/details/gnylfteep.sHtML

[R11] case 多分支
来源：http://read.share.epnwcf.com/Article/details/giibhyekv.sHtML

case "$1" in
来源：http://baike.epnwcf.com/Article/details/gksgooetx.sHtML

start) echo "启动" ;;
来源：http://blog.tarul.cn/Article/details/ghqkjhmba.sHtML

stop)  echo "停止" ;;
来源：http://www.m.share.bbcook.cn/Article/details/gjyrbjlna.sHtML

*)     echo "未知命令" ;;
来源：http://www.blog.tarul.cn/Article/details/gbmlvxmol.sHtML

esac
来源：http://www.share.fktsv.cn/Article/details/glghmjxrc.sHtML

[R12] for 遍历文件
来源：http://www.share.bbcook.cn/Article/details/gscxvyarx.sHtML

for f in *.txt; do echo "$f"; done
来源：http://mobile.sjlbkw.cn/Article/details/ggmehtigy.sHtML

[R13] for 计数循环
来源：http://baike.vehdjk.com/Article/details/gezfbnrfr.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.share.vehdjk.com/Article/details/gorxvtpda.sHtML

[R14] C 风格 for
来源：http://blog.sjlbkw.cn/Article/details/gznuaxizk.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://wap.yfazqb.com/Article/details/gvqxzkhkb.sHtML

[R15] while 逐行读文件
来源：http://read.share.vehdjk.com/Article/details/gonjfjagh.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://m.share.tarul.cn/Article/details/gldnglpes.sHtML

[R16] until 等待条件
来源：http://baike.fktsv.cn/Article/details/glazibpml.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.m.share.tarul.cn/Article/details/glljizgze.sHtML

[R17] 数组定义与取值
来源：http://www.m.share.yfazqb.com/Article/details/gqgligeir.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.m.share.bbcook.cn/Article/details/ggidswqke.sHtML

[R18] 遍历数组
来源：http://blog.fktsv.cn/Article/details/gbuxuqpjb.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://m.share.epnwcf.com/Article/details/gamifecdn.sHtML

[R19] 数组长度
来源：http://www.share.sjlbkw.cn/Article/details/gvldqansl.sHtML

echo "${#arr[@]}"
来源：http://www.share.sjlbkw.cn/Article/details/gmjrduhhy.sHtML

[R20] 关联数组（字典）
来源：http://read.share.vehdjk.com/Article/details/geexbfxhg.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://mobile.epnwcf.com/Article/details/guqeciqia.sHtML

[R21] 字符串长度
来源：http://www.m.share.epnwcf.com/Article/details/gzujytfow.sHtML

echo "${#s}"
来源：http://mobile.tarul.cn/Article/details/gztxwykyx.sHtML

[R22] 截取子串
来源：http://mobile.fktsv.cn/Article/details/ghpcpglyp.sHtML

echo "${s:0:5}"
来源：http://3g.epnwcf.com/Article/details/gstjosvgm.sHtML

[R23] 字符串替换
来源：http://www.blog.bbcook.cn/Article/details/gsmbphczr.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://mobile.bbcook.cn/Article/details/gzqwbuqra.sHtML

[R24] 大小写转换
来源：http://baike.vehdjk.com/Article/details/gmvsoyrfc.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://mobile.tarul.cn/Article/details/gbgpysqou.sHtML

[R25] 去后缀 / 去前缀
来源：http://m.share.fktsv.cn/Article/details/gixofxegx.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.blog.bbcook.cn/Article/details/ggazrzylh.sHtML

[R26] 命令替换
来源：http://www.m.share.yfazqb.com/Article/details/gnugwiahg.sHtML

now=$(date +%F); echo "$now"
来源：http://read.share.bbcook.cn/Article/details/gtwvjclkl.sHtML

[R27] 算术展开
来源：http://read.share.vehdjk.com/Article/details/gezbqkdke.sHtML

echo $((1 + 2 * 3))
来源：http://mobile.fktsv.cn/Article/details/gwutgspcx.sHtML

[R28] 浮点运算
来源：http://read.share.sjlbkw.cn/Article/details/goqodifmc.sHtML

echo "scale=2; 10/3" | bc
来源：http://baike.yfazqb.com/Article/details/gdskxmohn.sHtML

[R29] 定义函数
来源：http://blog.vehdjk.com/Article/details/gfkrbcani.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://blog.sjlbkw.cn/Article/details/gcudtzyqd.sHtML

[R30] 函数返回状态码
来源：http://www.m.share.yfazqb.com/Article/details/gezwogjgj.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://read.share.yfazqb.com/Article/details/gymseldgg.sHtML

[R31] 局部变量
来源：http://baike.sjlbkw.cn/Article/details/gdgskdjbd.sHtML

f() { local x=1; echo "$x"; }
来源：http://read.share.sjlbkw.cn/Article/details/gxozquqoz.sHtML

[R32] 参数个数校验
来源：http://baike.sjlbkw.cn/Article/details/gefcwqmpw.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://baike.yfazqb.com/Article/details/gsancpptd.sHtML

[R33] 捕获错误并提示行号
来源：http://baike.vehdjk.com/Article/details/grxapygdz.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://m.share.vehdjk.com/Article/details/ggqvzjvre.sHtML

[R34] 退出时清理
来源：http://www.blog.vehdjk.com/Article/details/ggmykkkoe.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.yfazqb.com/Article/details/gqgnnkthw.sHtML

[R35] 后台执行并等待
来源：http://m.share.vehdjk.com/Article/details/glhdsdarz.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.m.share.bbcook.cn/Article/details/ggqsiwjxa.sHtML

[R36] 并发执行多个任务
来源：http://www.m.share.vehdjk.com/Article/details/gnsgjlisu.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://blog.yfazqb.com/Article/details/gbfihwjwt.sHtML

[R37] 把输出赋给变量
来源：http://www.blog.yfazqb.com/Article/details/gkaebnohe.sHtML

files=$(ls -1)
来源：http://www.share.sjlbkw.cn/Article/details/gicblvxly.sHtML

[R38] 管道串联
来源：http://mobile.bbcook.cn/Article/details/gmxtyoxec.sHtML

cat a.txt | grep -i error | wc -l
来源：http://read.share.fktsv.cn/Article/details/gfafitoeu.sHtML

[R39] 重定向标准输出与错误
来源：http://baike.tarul.cn/Article/details/gifprusti.sHtML

cmd > out.log 2>&1
来源：http://baike.yfazqb.com/Article/details/goafzlcjd.sHtML

[R40] 追加写日志
来源：http://mobile.sjlbkw.cn/Article/details/giraehvnk.sHtML

echo "log" >> out.log
来源：http://read.share.tarul.cn/Article/details/gzqaaiqhk.sHtML

[R41] 丢弃输出
来源：http://baike.vehdjk.com/Article/details/grojzztbe.sHtML

cmd >/dev/null 2>&1
来源：http://baike.tarul.cn/Article/details/glekkcmui.sHtML

[R42] 输入重定向
来源：http://wap.sjlbkw.cn/Article/details/gnhuhbriq.sHtML

wc -l < a.txt
来源：http://wap.yfazqb.com/Article/details/gnxdfrhji.sHtML

[R43] 按名字查找文件
来源：http://baike.yfazqb.com/Article/details/gdtcohbch.sHtML

find . -name "*.log" -type f
来源：http://mobile.tarul.cn/Article/details/glbpxgbyf.sHtML

[R44] 按修改时间查找
来源：http://baike.tarul.cn/Article/details/gbdxxkoeg.sHtML

find . -mtime -7 -type f
来源：http://read.share.tarul.cn/Article/details/gkiiphnju.sHtML

[R45] 批量删除
来源：http://3g.vehdjk.com/Article/details/gtxcgecum.sHtML

find . -name "*.tmp" -delete
来源：http://www.blog.fktsv.cn/Article/details/gsxelniwt.sHtML

[R46] 递归替换文件内容
来源：http://www.blog.bbcook.cn/Article/details/gidvuguor.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.blog.epnwcf.com/Article/details/gazjtfwab.sHtML

[R47] sed 单行替换
来源：http://3g.epnwcf.com/Article/details/gzolooveg.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://mobile.bbcook.cn/Article/details/grqinnedg.sHtML

[R48] awk 取指定列
来源：http://www.m.share.sjlbkw.cn/Article/details/gzkjypere.sHtML

awk '{print $1, $3}' a.txt
来源：http://wap.fktsv.cn/Article/details/gnkfgatwn.sHtML

[R49] awk 带条件
来源：http://m.share.tarul.cn/Article/details/gllbenivs.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://m.share.sjlbkw.cn/Article/details/gzxyqubrz.sHtML

[R50] awk 求和
来源：http://www.share.epnwcf.com/Article/details/graqxqikn.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://baike.tarul.cn/Article/details/glvwadmzv.sHtML

[R51] 排序去重取前几
来源：http://www.blog.epnwcf.com/Article/details/gjeroqpag.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://m.share.epnwcf.com/Article/details/gxyrqrtid.sHtML

[R52] 统计行数
来源：http://blog.epnwcf.com/Article/details/gzsmkzzli.sHtML

wc -l a.txt
来源：http://3g.bbcook.cn/Article/details/gadzakzii.sHtML

[R53] 查看文件头与实时尾
来源：http://read.share.vehdjk.com/Article/details/gllyosigi.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.share.bbcook.cn/Article/details/goqpnqekd.sHtML

[R54] 比较两个文件
来源：http://read.share.fktsv.cn/Article/details/gkilubarn.sHtML

diff a.txt b.txt
来源：http://m.share.sjlbkw.cn/Article/details/gwclekjfd.sHtML

[R55] 压缩与解压
来源：http://baike.bbcook.cn/Article/details/grkxayryr.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://read.share.epnwcf.com/Article/details/gevmyrnxq.sHtML

[R56] 远程拷贝
来源：http://read.share.sjlbkw.cn/Article/details/gitezdqiw.sHtML

scp file user@host:/path/
来源：http://www.blog.yfazqb.com/Article/details/gxjcgkmwl.sHtML

[R57] 远程执行命令
来源：http://www.share.tarul.cn/Article/details/ggyzzklcz.sHtML

ssh user@host 'uptime'
来源：http://www.blog.epnwcf.com/Article/details/gucsrgwxs.sHtML

[R58] 下载文件
来源：http://blog.fktsv.cn/Article/details/gkaxkslzz.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://read.share.fktsv.cn/Article/details/gejgtzwvx.sHtML

[R59] 发 POST JSON
来源：http://mobile.yfazqb.com/Article/details/gpwzdjaax.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://3g.yfazqb.com/Article/details/gkkqnsavq.sHtML

[R60] 只看 HTTP 状态码
来源：http://mobile.yfazqb.com/Article/details/gucsjdoxw.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.m.share.bbcook.cn/Article/details/gsiqlieqg.sHtML

[R61] 磁盘占用
来源：http://blog.yfazqb.com/Article/details/ggtvwjsuo.sHtML

df -h;  du -sh *
来源：http://blog.sjlbkw.cn/Article/details/gudjsmblv.sHtML

[R62] 找最占空间的文件
来源：http://www.share.tarul.cn/Article/details/gnswmervg.sHtML

du -ah . | sort -rh | head -10
来源：http://www.share.epnwcf.com/Article/details/gydbmymmm.sHtML

[R63] 内存与进程
来源：http://www.blog.vehdjk.com/Article/details/gfbxxepsq.sHtML

free -h;  ps aux | grep nginx
来源：http://mobile.yfazqb.com/Article/details/gizcqfufw.sHtML

[R64] 结束进程
来源：http://read.share.epnwcf.com/Article/details/gauhjbgfg.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.m.share.yfazqb.com/Article/details/gsmqdffnq.sHtML

[R65] 查看端口占用
来源：http://www.share.bbcook.cn/Article/details/gdxbnxmut.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://read.share.bbcook.cn/Article/details/giyupgwza.sHtML

[R66] 定时任务
来源：http://blog.bbcook.cn/Article/details/gcisbymxf.sHtML

crontab -e;  crontab -l
来源：http://blog.epnwcf.com/Article/details/gqzczfdwa.sHtML

[R67] 生成随机十六进制串
来源：http://mobile.fktsv.cn/Article/details/gnvwjfqma.sHtML

openssl rand -hex 16
来源：http://m.share.bbcook.cn/Article/details/gaorngvjw.sHtML

[R68] 计算文件校验值
来源：http://mobile.tarul.cn/Article/details/glccgwsku.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://wap.fktsv.cn/Article/details/gpnzvofaw.sHtML

[R69] 生成随机密码
来源：http://www.share.yfazqb.com/Article/details/gzcjegyur.sHtML

head -c 16 /dev/urandom | base64
来源：http://wap.tarul.cn/Article/details/gmpgldlwy.sHtML

[R70] 时间戳与互转
来源：http://www.share.tarul.cn/Article/details/giindhdwc.sHtML

date +%s;  date -d @1700000000
来源：http://www.share.sjlbkw.cn/Article/details/gpukwmghv.sHtML

[R71] 日期格式化
来源：http://read.share.epnwcf.com/Article/details/gqxtlcseu.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://baike.yfazqb.com/Article/details/gbvwalfcc.sHtML

[R72] 等待端口就绪
来源：http://baike.vehdjk.com/Article/details/gmbibiprx.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://wap.bbcook.cn/Article/details/gotccgpua.sHtML

[R73] 分割大日志
来源：http://wap.vehdjk.com/Article/details/gypbjmqgk.sHtML

split -l 1000 big.log part_
来源：http://m.share.sjlbkw.cn/Article/details/gqogsbzry.sHtML

[R74] 批量重命名
来源：http://www.m.share.epnwcf.com/Article/details/gqpdjdxoc.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://wap.yfazqb.com/Article/details/grsyzxqbn.sHtML

[R75] 导出环境变量
来源：http://www.share.bbcook.cn/Article/details/ghuxmfhtf.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.share.tarul.cn/Article/details/gzhkiptdv.sHtML

[R76] 使用临时文件
来源：http://wap.bbcook.cn/Article/details/grweexexd.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://m.share.yfazqb.com/Article/details/gicxxksen.sHtML

[R77] 读取用户输入
来源：http://www.m.share.tarul.cn/Article/details/gjezfrpsk.sHtML

read -rp "请输入: " ans
来源：http://mobile.bbcook.cn/Article/details/gxqmyuczy.sHtML

[R78] 交互式菜单
来源：http://baike.epnwcf.com/Article/details/gpdwoxcmu.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://blog.vehdjk.com/Article/details/gfpdioqro.sHtML

[R79] 解析命令行选项
来源：http://www.blog.epnwcf.com/Article/details/gxicngjqe.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.share.bbcook.cn/Article/details/girfkjrqy.sHtML

[R80] 查看脚本执行耗时
来源：http://www.m.share.fktsv.cn/Article/details/gaoottntj.sHtML

time ./run.sh
来源：http://mobile.tarul.cn/Article/details/gdqfjaexg.sHtML

================================================================================
来源：http://mobile.epnwcf.com/Article/details/gefiudunv.sHtML

S. C / C++ 专题
来源：http://blog.bbcook.cn/Article/details/gezmrdehv.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/gfnqzuqkl.sHtML

[S01] C：Hello World
来源：http://read.share.yfazqb.com/Article/details/gprmkizpc.sHtML

#include <stdio.h>
来源：http://www.share.vehdjk.com/Article/details/gzdbeuxqc.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://baike.sjlbkw.cn/Article/details/gngwqlwou.sHtML

[S02] C：变量与格式化输出
来源：http://blog.tarul.cn/Article/details/guffrzvwi.sHtML

int a = 10; printf("%d\n", a);
来源：http://baike.epnwcf.com/Article/details/ggqvpnrzj.sHtML

[S03] C：读入整数
来源：http://blog.epnwcf.com/Article/details/ghcywxpip.sHtML

int x; scanf("%d", &x);
来源：http://www.blog.epnwcf.com/Article/details/gdkzbeayr.sHtML

[S04] C：字符串复制
来源：http://3g.sjlbkw.cn/Article/details/gxsxlyxlp.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.m.share.sjlbkw.cn/Article/details/gtwjmqsfg.sHtML

[S05] C：字符串长度
来源：http://www.m.share.tarul.cn/Article/details/gmjedhtdo.sHtML


<!-- 参考信息 -->