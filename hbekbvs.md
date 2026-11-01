代发 wailian999

[Q33] 多列分组
来源：http://www.m.share.tarul.cn/Article/details/gctegbfgk.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.share.yfazqb.com/Article/details/gbnfbqzvt.sHtML

[Q34] 每组取第一条
来源：http://www.share.sjlbkw.cn/Article/details/gxltgfzwp.sHtML

SELECT * FROM (
来源：http://wap.vehdjk.com/Article/details/guhlprjne.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://read.share.epnwcf.com/Article/details/gozzkktdp.sHtML

) t WHERE rn = 1;
来源：http://www.m.share.bbcook.cn/Article/details/gzzgtsrsl.sHtML

[Q35] 内连接
来源：http://baike.bbcook.cn/Article/details/gneuduxss.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.share.vehdjk.com/Article/details/gyhmutwvr.sHtML

[Q36] 左连接
来源：http://www.blog.fktsv.cn/Article/details/gvsoolzbs.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://mobile.sjlbkw.cn/Article/details/gthapcloq.sHtML

[Q37] 右连接
来源：http://www.m.share.epnwcf.com/Article/details/gvzquters.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://read.share.fktsv.cn/Article/details/gecyxwutt.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://m.share.yfazqb.com/Article/details/gkxdyzqrf.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.m.share.bbcook.cn/Article/details/glukoeihp.sHtML

[Q39] 自连接（查上下级）
来源：http://m.share.vehdjk.com/Article/details/gatytyype.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.blog.epnwcf.com/Article/details/gttwibobe.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://m.share.fktsv.cn/Article/details/gdwijcgnv.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.share.yfazqb.com/Article/details/gpqphhjmb.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.m.share.bbcook.cn/Article/details/gefsfydod.sHtML

[Q41] 多表连接
来源：http://wap.fktsv.cn/Article/details/gxanzfxaq.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://mobile.bbcook.cn/Article/details/gzmzupike.sHtML

JOIN users u ON u.id = o.user_id
来源：http://blog.vehdjk.com/Article/details/gvjohfpkw.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://baike.fktsv.cn/Article/details/gtfxhsqnw.sHtML

[Q42] 连接条件附加过滤
来源：http://m.share.vehdjk.com/Article/details/gtofefrws.sHtML

SELECT u.name, o.amount FROM users u
来源：http://3g.tarul.cn/Article/details/gdppqwnep.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.m.share.yfazqb.com/Article/details/gsrgmiijp.sHtML

[Q43] 标量子查询
来源：http://www.share.tarul.cn/Article/details/giirslaql.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://3g.fktsv.cn/Article/details/gxbsjqobc.sHtML

[Q44] IN 子查询
来源：http://m.share.epnwcf.com/Article/details/gczyenccn.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://3g.fktsv.cn/Article/details/glctskgtx.sHtML

[Q45] EXISTS 判断存在
来源：http://www.m.share.bbcook.cn/Article/details/ggtbamnsx.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.tarul.cn/Article/details/gneezoljb.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://baike.vehdjk.com/Article/details/gqgusowgp.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.tarul.cn/Article/details/gonzyxple.sHtML

[Q47] 与平均值比较
来源：http://www.share.fktsv.cn/Article/details/gcncmvrpx.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://baike.sjlbkw.cn/Article/details/gkvreqhls.sHtML

[Q48] CTE 公用表表达式
来源：http://www.m.share.sjlbkw.cn/Article/details/geejdjkzu.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://wap.epnwcf.com/Article/details/galeqjwbh.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.m.share.sjlbkw.cn/Article/details/gzzeqqkbs.sHtML

[Q49] 更新单行
来源：http://blog.bbcook.cn/Article/details/glphozsqr.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://3g.fktsv.cn/Article/details/gqccjfwhp.sHtML

[Q50] 批量更新
来源：http://read.share.fktsv.cn/Article/details/ghbgtwhjm.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://3g.yfazqb.com/Article/details/gbaalslwj.sHtML

[Q51] 用子查询更新
来源：http://blog.epnwcf.com/Article/details/gmbgxaopr.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://mobile.sjlbkw.cn/Article/details/gyxdmnmqm.sHtML

[Q52] 删除指定行
来源：http://blog.fktsv.cn/Article/details/gpwdeyokx.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.m.share.bbcook.cn/Article/details/gcmvfafqt.sHtML

[Q53] 按条件删除
来源：http://www.blog.epnwcf.com/Article/details/gbibnjgjq.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://wap.sjlbkw.cn/Article/details/gueplxjqy.sHtML

[Q54] 清空表
来源：http://3g.sjlbkw.cn/Article/details/gfrjhyqgo.sHtML

TRUNCATE TABLE logs;
来源：http://3g.bbcook.cn/Article/details/gxgwcbard.sHtML

[Q55] 排名（并列占位）
来源：http://read.share.fktsv.cn/Article/details/guyyldfhm.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.m.share.tarul.cn/Article/details/gpqtytrql.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.share.tarul.cn/Article/details/giaoccslg.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.m.share.vehdjk.com/Article/details/gjriofyzm.sHtML

[Q57] 行号
来源：http://read.share.yfazqb.com/Article/details/gzqlkheuk.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://3g.epnwcf.com/Article/details/gcbdwdanp.sHtML

[Q58] 累计求和
来源：http://3g.yfazqb.com/Article/details/gsnmewwwa.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.share.vehdjk.com/Article/details/gbumfwpad.sHtML

[Q59] 分组内累计
来源：http://www.blog.epnwcf.com/Article/details/guwcmghsx.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://m.share.vehdjk.com/Article/details/grnhsfdnb.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.m.share.tarul.cn/Article/details/glmkcghrx.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.m.share.vehdjk.com/Article/details/gflhfpcsa.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://3g.sjlbkw.cn/Article/details/glacgillu.sHtML

[Q61] 移动平均
来源：http://www.share.fktsv.cn/Article/details/gqtgbzwhf.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://read.share.yfazqb.com/Article/details/ggmqduvcm.sHtML

[Q62] 分组占比
来源：http://wap.vehdjk.com/Article/details/gmqwubrza.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.share.tarul.cn/Article/details/ghqalujku.sHtML

[Q63] 开启事务
来源：http://read.share.epnwcf.com/Article/details/gpsceparz.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.share.yfazqb.com/Article/details/ggdxiekkj.sHtML

[Q64] 提交事务
来源：http://wap.epnwcf.com/Article/details/gfbcnxhkp.sHtML

COMMIT;
来源：http://www.blog.epnwcf.com/Article/details/gylevipxx.sHtML

[Q65] 回滚事务
来源：http://wap.epnwcf.com/Article/details/gfrclqjcx.sHtML

ROLLBACK;
来源：http://www.blog.sjlbkw.cn/Article/details/gtzdqesjz.sHtML

[Q66] 行锁查询
来源：http://baike.tarul.cn/Article/details/ghwflooqi.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://read.share.yfazqb.com/Article/details/gnoycollq.sHtML

[Q67] 设置隔离级别
来源：http://www.blog.fktsv.cn/Article/details/gqnzfiocr.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://3g.tarul.cn/Article/details/gcbgzmxkv.sHtML

[Q68] 保存点
来源：http://m.share.tarul.cn/Article/details/gbzhbxsre.sHtML

SAVEPOINT sp1;
来源：http://www.blog.bbcook.cn/Article/details/gginwxjtz.sHtML

ROLLBACK TO sp1;
来源：http://www.blog.epnwcf.com/Article/details/gfmcswalb.sHtML

[Q69] 查看执行计划
来源：http://www.blog.sjlbkw.cn/Article/details/gqzpeurff.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.share.vehdjk.com/Article/details/gexlbupjp.sHtML

[Q70] 更新统计信息
来源：http://m.share.tarul.cn/Article/details/gaujanhem.sHtML

ANALYZE TABLE users;
来源：http://baike.tarul.cn/Article/details/gvnoygnkh.sHtML

[Q71] 查看建表语句
来源：http://blog.vehdjk.com/Article/details/gybufwhgk.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://read.share.tarul.cn/Article/details/glxzchpgw.sHtML

[Q72] 查看索引
来源：http://blog.tarul.cn/Article/details/gizvaelau.sHtML

SHOW INDEX FROM users;
来源：http://read.share.sjlbkw.cn/Article/details/gawqyfoas.sHtML

[Q73] 查看表状态
来源：http://3g.bbcook.cn/Article/details/gwloodphc.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://baike.epnwcf.com/Article/details/gaxzrhtmr.sHtML

[Q74] 强制使用索引
来源：http://mobile.vehdjk.com/Article/details/gpsgpudor.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://3g.tarul.cn/Article/details/gjquodbwd.sHtML

[Q75] 日期格式化
来源：http://baike.bbcook.cn/Article/details/gkskcfxey.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://m.share.tarul.cn/Article/details/gnmqqwruu.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://3g.fktsv.cn/Article/details/gwtrmaphf.sHtML

[Q76] 按天统计
来源：http://www.share.fktsv.cn/Article/details/gbjwmkurj.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://blog.epnwcf.com/Article/details/gwcohvrrd.sHtML

[Q77] 时间加减
来源：http://3g.yfazqb.com/Article/details/gzqkfucvj.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://wap.fktsv.cn/Article/details/gihgxetoc.sHtML

[Q78] 当前时间
来源：http://3g.fktsv.cn/Article/details/grfjyoema.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://wap.tarul.cn/Article/details/gsyqolurd.sHtML

[Q79] 字符串拼接
来源：http://mobile.bbcook.cn/Article/details/gyfogelvw.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://baike.tarul.cn/Article/details/gofbkcxbs.sHtML

[Q80] 字符串截取
来源：http://3g.vehdjk.com/Article/details/gsaaglxqc.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://read.share.bbcook.cn/Article/details/gubcjwlec.sHtML

[Q81] 字符串替换
来源：http://www.m.share.fktsv.cn/Article/details/glbvnlkay.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://blog.vehdjk.com/Article/details/gwykzdkaq.sHtML

[Q82] 字符长度与字节长度
来源：http://m.share.yfazqb.com/Article/details/gyezcpwrf.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://blog.epnwcf.com/Article/details/gpabdlapm.sHtML

[Q83] 大小写转换
来源：http://baike.fktsv.cn/Article/details/gnflzbhoc.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://read.share.fktsv.cn/Article/details/ghasgmnea.sHtML

[Q84] 去除首尾空格
来源：http://3g.vehdjk.com/Article/details/gyzuvijgx.sHtML

SELECT TRIM(name) FROM users;
来源：http://wap.fktsv.cn/Article/details/gywzganhd.sHtML

[Q85] 数值取整
来源：http://m.share.yfazqb.com/Article/details/gifdkewrw.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://m.share.epnwcf.com/Article/details/gyyfyyyuo.sHtML

[Q86] 读取 JSON 字段
来源：http://www.blog.epnwcf.com/Article/details/gokkfdcpn.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.blog.epnwcf.com/Article/details/glrssczxg.sHtML

[Q87] JSON 字段做条件
来源：http://3g.epnwcf.com/Article/details/gebvwllqr.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://read.share.epnwcf.com/Article/details/grmucifjw.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.share.epnwcf.com/Article/details/gankhktdy.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.share.bbcook.cn/Article/details/gkmppvzwo.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://m.share.epnwcf.com/Article/details/gstinlsyu.sHtML

[Q89] 判断表是否存在
来源：http://www.blog.fktsv.cn/Article/details/gczcxohby.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.m.share.sjlbkw.cn/Article/details/gomgbbbdz.sHtML

[Q90] 生成序号列
来源：http://blog.epnwcf.com/Article/details/gcnmvhkuw.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.share.bbcook.cn/Article/details/ghlsyurha.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/gemgjibyu.sHtML

R. Bash 专题
来源：http://m.share.bbcook.cn/Article/details/gaogtrdha.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/gepdawrzx.sHtML

[R01] shebang 与严格模式
来源：http://blog.tarul.cn/Article/details/gblqaqoyx.sHtML

#!/usr/bin/env bash
来源：http://blog.vehdjk.com/Article/details/gdeuttdgw.sHtML

set -euo pipefail
来源：http://blog.sjlbkw.cn/Article/details/gowcffsqq.sHtML

[R02] 变量赋值与使用
来源：http://blog.sjlbkw.cn/Article/details/gorfuqiru.sHtML

name="Tom"; echo "$name"
来源：http://www.share.tarul.cn/Article/details/gmtjrxepi.sHtML

[R03] 只读变量
来源：http://www.share.sjlbkw.cn/Article/details/gyapxtiyx.sHtML

readonly PI=3.14
来源：http://www.share.fktsv.cn/Article/details/gxvtfiycy.sHtML

[R04] 位置参数
来源：http://www.m.share.vehdjk.com/Article/details/gaoyowhpo.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://blog.epnwcf.com/Article/details/govmtifis.sHtML

[R05] 参数默认值
来源：http://blog.bbcook.cn/Article/details/gyoghcyyu.sHtML

name="${1:-default}"
来源：http://mobile.tarul.cn/Article/details/gltkuracg.sHtML

[R06] 判断命令是否存在
来源：http://baike.tarul.cn/Article/details/glssgfsih.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://blog.fktsv.cn/Article/details/gxdonjmqd.sHtML

[R07] if 判断文件
来源：http://www.m.share.epnwcf.com/Article/details/guerrmxmx.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://wap.epnwcf.com/Article/details/ghalclnjf.sHtML

[R08] 数值比较
来源：http://3g.yfazqb.com/Article/details/ggqfroolb.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://m.share.bbcook.cn/Article/details/gaufuxsod.sHtML

[R09] 字符串比较
来源：http://blog.tarul.cn/Article/details/gjwjmhwqg.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://blog.tarul.cn/Article/details/gpwtovdly.sHtML

[R10] 正则匹配
来源：http://wap.vehdjk.com/Article/details/gvwkueupa.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://wap.tarul.cn/Article/details/gdmaafdqm.sHtML

[R11] case 多分支
来源：http://wap.epnwcf.com/Article/details/gbgrhiqkd.sHtML

case "$1" in
来源：http://www.share.yfazqb.com/Article/details/gxownirea.sHtML

start) echo "启动" ;;
来源：http://m.share.bbcook.cn/Article/details/gxqlkyqvw.sHtML

stop)  echo "停止" ;;
来源：http://wap.vehdjk.com/Article/details/gudphsccf.sHtML

*)     echo "未知命令" ;;
来源：http://read.share.bbcook.cn/Article/details/gklxtouru.sHtML

esac
来源：http://www.m.share.fktsv.cn/Article/details/gynkjbvdc.sHtML

[R12] for 遍历文件
来源：http://baike.bbcook.cn/Article/details/gclicvvut.sHtML

for f in *.txt; do echo "$f"; done
来源：http://3g.vehdjk.com/Article/details/gplvbcejd.sHtML

[R13] for 计数循环
来源：http://m.share.sjlbkw.cn/Article/details/gydsbyrsf.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://m.share.bbcook.cn/Article/details/gmhywczjh.sHtML

[R14] C 风格 for
来源：http://wap.epnwcf.com/Article/details/gcscwthih.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.m.share.bbcook.cn/Article/details/gdmwcqect.sHtML

[R15] while 逐行读文件
来源：http://www.share.vehdjk.com/Article/details/gviejysxb.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://m.share.vehdjk.com/Article/details/geopchger.sHtML

[R16] until 等待条件
来源：http://read.share.fktsv.cn/Article/details/gpplruaku.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://wap.yfazqb.com/Article/details/gyrsmgzwt.sHtML

[R17] 数组定义与取值
来源：http://read.share.sjlbkw.cn/Article/details/gmkdmgrbp.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://blog.vehdjk.com/Article/details/gxcjqcrfk.sHtML

[R18] 遍历数组
来源：http://www.share.fktsv.cn/Article/details/gmbakumiv.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://baike.yfazqb.com/Article/details/gdgwanupk.sHtML

[R19] 数组长度
来源：http://wap.vehdjk.com/Article/details/gqwgthzft.sHtML

echo "${#arr[@]}"
来源：http://www.blog.tarul.cn/Article/details/gcjwibokj.sHtML

[R20] 关联数组（字典）
来源：http://wap.bbcook.cn/Article/details/gvurjpnqn.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://blog.fktsv.cn/Article/details/gamnbnkob.sHtML

[R21] 字符串长度
来源：http://mobile.epnwcf.com/Article/details/guqazcwuq.sHtML

echo "${#s}"
来源：http://baike.sjlbkw.cn/Article/details/gqkuwraqm.sHtML

[R22] 截取子串
来源：http://3g.bbcook.cn/Article/details/gskbxzrat.sHtML

echo "${s:0:5}"
来源：http://m.share.bbcook.cn/Article/details/gwwpiqxfx.sHtML

[R23] 字符串替换
来源：http://read.share.sjlbkw.cn/Article/details/gzogbbnhq.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.blog.fktsv.cn/Article/details/ghhugahim.sHtML

[R24] 大小写转换
来源：http://www.blog.epnwcf.com/Article/details/ghzeywwbc.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://mobile.fktsv.cn/Article/details/gohbgdjsl.sHtML

[R25] 去后缀 / 去前缀
来源：http://mobile.vehdjk.com/Article/details/guefinvqu.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://wap.epnwcf.com/Article/details/gluqbuigq.sHtML

[R26] 命令替换
来源：http://www.m.share.epnwcf.com/Article/details/ggeveekqo.sHtML

now=$(date +%F); echo "$now"
来源：http://m.share.vehdjk.com/Article/details/gzadzhmpu.sHtML

[R27] 算术展开
来源：http://read.share.epnwcf.com/Article/details/gzsxacimb.sHtML

echo $((1 + 2 * 3))
来源：http://blog.tarul.cn/Article/details/ggcxokyzx.sHtML

[R28] 浮点运算
来源：http://baike.fktsv.cn/Article/details/gujxwvboh.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.m.share.epnwcf.com/Article/details/ghscxugvk.sHtML

[R29] 定义函数
来源：http://3g.yfazqb.com/Article/details/gztdyhcpi.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://baike.vehdjk.com/Article/details/gdssxzbac.sHtML

[R30] 函数返回状态码
来源：http://www.m.share.bbcook.cn/Article/details/gstuaohwc.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://mobile.epnwcf.com/Article/details/ghsgfytbk.sHtML

[R31] 局部变量
来源：http://www.blog.vehdjk.com/Article/details/glkqvrqkr.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.blog.fktsv.cn/Article/details/gifaisldu.sHtML

[R32] 参数个数校验
来源：http://baike.sjlbkw.cn/Article/details/gnddqwpdk.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.blog.fktsv.cn/Article/details/gawiwklyb.sHtML

[R33] 捕获错误并提示行号
来源：http://www.m.share.fktsv.cn/Article/details/georsomdb.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://wap.tarul.cn/Article/details/gqpaxkjsw.sHtML

[R34] 退出时清理
来源：http://www.blog.vehdjk.com/Article/details/guhiicvpl.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://baike.sjlbkw.cn/Article/details/gqcdxyqkr.sHtML

[R35] 后台执行并等待
来源：http://mobile.yfazqb.com/Article/details/gvfcfsrxn.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://mobile.yfazqb.com/Article/details/gnyonwtpp.sHtML

[R36] 并发执行多个任务
来源：http://www.blog.epnwcf.com/Article/details/gvuqqbgim.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://blog.bbcook.cn/Article/details/gfzrqmrve.sHtML

[R37] 把输出赋给变量
来源：http://read.share.tarul.cn/Article/details/gzjsnlcrt.sHtML

files=$(ls -1)
来源：http://blog.bbcook.cn/Article/details/gttksekjb.sHtML

[R38] 管道串联
来源：http://www.share.fktsv.cn/Article/details/gncjoqnti.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.blog.bbcook.cn/Article/details/gdvzaxbem.sHtML

[R39] 重定向标准输出与错误
来源：http://wap.fktsv.cn/Article/details/giowwdmpb.sHtML

cmd > out.log 2>&1
来源：http://wap.vehdjk.com/Article/details/gpvuhlrev.sHtML

[R40] 追加写日志
来源：http://3g.bbcook.cn/Article/details/gfspxdyjl.sHtML

echo "log" >> out.log
来源：http://www.blog.tarul.cn/Article/details/gnqjmuvjn.sHtML

[R41] 丢弃输出
来源：http://3g.yfazqb.com/Article/details/grwhpihit.sHtML

cmd >/dev/null 2>&1
来源：http://www.blog.tarul.cn/Article/details/glicmaunr.sHtML

[R42] 输入重定向
来源：http://baike.fktsv.cn/Article/details/gcwjaiskh.sHtML

wc -l < a.txt
来源：http://m.share.tarul.cn/Article/details/gvervekuk.sHtML

[R43] 按名字查找文件
来源：http://www.share.bbcook.cn/Article/details/gjgmrsyms.sHtML

find . -name "*.log" -type f
来源：http://www.share.vehdjk.com/Article/details/gotbodhwe.sHtML

[R44] 按修改时间查找
来源：http://www.m.share.sjlbkw.cn/Article/details/gzjybqkbb.sHtML

find . -mtime -7 -type f
来源：http://wap.vehdjk.com/Article/details/gqqsfomvb.sHtML

[R45] 批量删除
来源：http://blog.sjlbkw.cn/Article/details/gkwqamzyi.sHtML

find . -name "*.tmp" -delete
来源：http://baike.bbcook.cn/Article/details/gkobiprjg.sHtML

[R46] 递归替换文件内容
来源：http://3g.tarul.cn/Article/details/gammxffol.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://blog.tarul.cn/Article/details/gfrfurrvo.sHtML

[R47] sed 单行替换
来源：http://3g.bbcook.cn/Article/details/gqpywjcly.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://baike.bbcook.cn/Article/details/gijjzjlvu.sHtML

[R48] awk 取指定列
来源：http://mobile.tarul.cn/Article/details/grnoniehf.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.m.share.tarul.cn/Article/details/gekwslfpd.sHtML

[R49] awk 带条件
来源：http://www.share.epnwcf.com/Article/details/gefpynihl.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://mobile.sjlbkw.cn/Article/details/giodunuhx.sHtML

[R50] awk 求和
来源：http://www.m.share.bbcook.cn/Article/details/gbxakebjw.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://baike.vehdjk.com/Article/details/glszmwdfw.sHtML

[R51] 排序去重取前几
来源：http://www.m.share.fktsv.cn/Article/details/gpcvjughd.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://wap.bbcook.cn/Article/details/gmoujreve.sHtML

[R52] 统计行数
来源：http://mobile.tarul.cn/Article/details/gquanwktx.sHtML

wc -l a.txt
来源：http://wap.yfazqb.com/Article/details/gxdcgkskj.sHtML

[R53] 查看文件头与实时尾
来源：http://baike.yfazqb.com/Article/details/gtswtqmhn.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.share.tarul.cn/Article/details/ghzkcuwru.sHtML

[R54] 比较两个文件
来源：http://www.m.share.epnwcf.com/Article/details/gyowthxcs.sHtML

diff a.txt b.txt
来源：http://www.m.share.sjlbkw.cn/Article/details/gwmywmfxb.sHtML

[R55] 压缩与解压
来源：http://blog.bbcook.cn/Article/details/gdsgrlotw.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://wap.yfazqb.com/Article/details/gpycycmdg.sHtML

[R56] 远程拷贝
来源：http://www.m.share.yfazqb.com/Article/details/grsiqqyev.sHtML

scp file user@host:/path/
来源：http://m.share.yfazqb.com/Article/details/grddgdtmu.sHtML

[R57] 远程执行命令
来源：http://www.share.sjlbkw.cn/Article/details/gvnihdahc.sHtML

ssh user@host 'uptime'
来源：http://www.m.share.vehdjk.com/Article/details/gmdxeyqeo.sHtML

[R58] 下载文件
来源：http://m.share.vehdjk.com/Article/details/gisabuxwr.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://mobile.vehdjk.com/Article/details/gwfqxqhui.sHtML

[R59] 发 POST JSON
来源：http://baike.fktsv.cn/Article/details/gzsdbldos.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://m.share.vehdjk.com/Article/details/gvmmadfny.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.m.share.vehdjk.com/Article/details/glgfjiwnn.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://baike.epnwcf.com/Article/details/giqrytzee.sHtML

[R61] 磁盘占用
来源：http://blog.yfazqb.com/Article/details/gqdtodiey.sHtML

df -h;  du -sh *
来源：http://mobile.fktsv.cn/Article/details/guighmrxk.sHtML

[R62] 找最占空间的文件
来源：http://www.m.share.yfazqb.com/Article/details/ggcgjiwim.sHtML

du -ah . | sort -rh | head -10
来源：http://read.share.tarul.cn/Article/details/gssqoxgaj.sHtML

[R63] 内存与进程
来源：http://www.m.share.yfazqb.com/Article/details/gbdqbwaob.sHtML

free -h;  ps aux | grep nginx
来源：http://3g.fktsv.cn/Article/details/gjrkysfxa.sHtML

[R64] 结束进程
来源：http://read.share.sjlbkw.cn/Article/details/gdamizhhz.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.blog.sjlbkw.cn/Article/details/gdovdmsrl.sHtML

[R65] 查看端口占用
来源：http://baike.bbcook.cn/Article/details/gqnlnlhwa.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mobile.yfazqb.com/Article/details/ggpsdbimh.sHtML

[R66] 定时任务
来源：http://m.share.fktsv.cn/Article/details/gprupdlts.sHtML

crontab -e;  crontab -l
来源：http://www.share.epnwcf.com/Article/details/gfxicztau.sHtML

[R67] 生成随机十六进制串
来源：http://read.share.yfazqb.com/Article/details/ghufxfdmr.sHtML

openssl rand -hex 16
来源：http://baike.yfazqb.com/Article/details/gdluusppn.sHtML

[R68] 计算文件校验值
来源：http://blog.vehdjk.com/Article/details/gelaussby.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://mobile.sjlbkw.cn/Article/details/grzscwhhp.sHtML

[R69] 生成随机密码
来源：http://3g.vehdjk.com/Article/details/geihwvbyx.sHtML

head -c 16 /dev/urandom | base64
来源：http://baike.vehdjk.com/Article/details/gdqfkrcqo.sHtML

[R70] 时间戳与互转
来源：http://blog.bbcook.cn/Article/details/gmutpkrab.sHtML

date +%s;  date -d @1700000000
来源：http://mobile.bbcook.cn/Article/details/gbrjkmkck.sHtML

[R71] 日期格式化
来源：http://3g.sjlbkw.cn/Article/details/ggkfqvqaa.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.share.yfazqb.com/Article/details/gylgzhunj.sHtML

[R72] 等待端口就绪
来源：http://read.share.fktsv.cn/Article/details/gtdsscnog.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://wap.fktsv.cn/Article/details/gssoicdlx.sHtML

[R73] 分割大日志
来源：http://blog.vehdjk.com/Article/details/gwfpnfqqg.sHtML

split -l 1000 big.log part_
来源：http://www.blog.tarul.cn/Article/details/golcgxtdm.sHtML

[R74] 批量重命名
来源：http://blog.bbcook.cn/Article/details/gsvookfkv.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://mobile.yfazqb.com/Article/details/guespxqzc.sHtML

[R75] 导出环境变量
来源：http://baike.sjlbkw.cn/Article/details/gkvlyxwty.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://wap.bbcook.cn/Article/details/gsyonlfjv.sHtML

[R76] 使用临时文件
来源：http://read.share.sjlbkw.cn/Article/details/gksfxdqrl.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://m.share.vehdjk.com/Article/details/gisggzetv.sHtML

[R77] 读取用户输入
来源：http://mobile.fktsv.cn/Article/details/grnxcgpla.sHtML

read -rp "请输入: " ans
来源：http://baike.sjlbkw.cn/Article/details/gznyrglme.sHtML

[R78] 交互式菜单
来源：http://3g.epnwcf.com/Article/details/goovcdjwa.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://wap.tarul.cn/Article/details/gdugkrghu.sHtML

[R79] 解析命令行选项
来源：http://baike.sjlbkw.cn/Article/details/gabtbptjd.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.m.share.epnwcf.com/Article/details/gbfabnjpm.sHtML

[R80] 查看脚本执行耗时
来源：http://www.blog.vehdjk.com/Article/details/gtqvhybap.sHtML

time ./run.sh
来源：http://www.blog.bbcook.cn/Article/details/gbovaguzq.sHtML

================================================================================
来源：http://mobile.vehdjk.com/Article/details/ggxakadsa.sHtML

S. C / C++ 专题
来源：http://mobile.tarul.cn/Article/details/ghmpfpxpl.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/ghozljvka.sHtML

[S01] C：Hello World
来源：http://www.blog.yfazqb.com/Article/details/gdhsjcnih.sHtML

#include <stdio.h>
来源：http://baike.sjlbkw.cn/Article/details/gbpzkinjk.sHtML


<!-- 参考信息 -->