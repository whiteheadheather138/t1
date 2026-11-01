代发 wailian999

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://mobile.vehdjk.com/Article/details/gonvqcazv.sHtML

) t WHERE rn = 1;
来源：http://wap.fktsv.cn/Article/details/gvamxmutx.sHtML

[Q35] 内连接
来源：http://baike.tarul.cn/Article/details/gtpunmlko.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://3g.yfazqb.com/Article/details/gikfupids.sHtML

[Q36] 左连接
来源：http://blog.vehdjk.com/Article/details/gcezferoc.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://mobile.fktsv.cn/Article/details/gbicciiai.sHtML

[Q37] 右连接
来源：http://www.blog.tarul.cn/Article/details/gsbtjckdy.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://mobile.sjlbkw.cn/Article/details/glorwxjri.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://m.share.bbcook.cn/Article/details/gmgkzioih.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.blog.sjlbkw.cn/Article/details/gywrmrddo.sHtML

[Q39] 自连接（查上下级）
来源：http://www.m.share.bbcook.cn/Article/details/gzucwflcy.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://read.share.tarul.cn/Article/details/gdsihjkyw.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.share.tarul.cn/Article/details/gnmoohwcq.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://mobile.sjlbkw.cn/Article/details/ghcdetmwj.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.m.share.tarul.cn/Article/details/glqfbndib.sHtML

[Q41] 多表连接
来源：http://blog.fktsv.cn/Article/details/gzlfrtytv.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://baike.vehdjk.com/Article/details/ggqyyzqkc.sHtML

JOIN users u ON u.id = o.user_id
来源：http://baike.vehdjk.com/Article/details/gemwskppa.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://wap.vehdjk.com/Article/details/gejonhnjq.sHtML

[Q42] 连接条件附加过滤
来源：http://baike.tarul.cn/Article/details/gsrsxzjra.sHtML

SELECT u.name, o.amount FROM users u
来源：http://read.share.epnwcf.com/Article/details/gouyuzjky.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://3g.bbcook.cn/Article/details/gpbdsoybd.sHtML

[Q43] 标量子查询
来源：http://blog.bbcook.cn/Article/details/gixpuomxl.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://m.share.bbcook.cn/Article/details/giijkbsoc.sHtML

[Q44] IN 子查询
来源：http://www.m.share.sjlbkw.cn/Article/details/ghcxzjvvh.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.share.sjlbkw.cn/Article/details/giuwuzvyt.sHtML

[Q45] EXISTS 判断存在
来源：http://mobile.tarul.cn/Article/details/giaxgsmny.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.yfazqb.com/Article/details/gbgsgjwsx.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://blog.bbcook.cn/Article/details/gwivlexwq.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.vehdjk.com/Article/details/ghmkeupsp.sHtML

[Q47] 与平均值比较
来源：http://www.share.yfazqb.com/Article/details/gfsktuqxz.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://read.share.tarul.cn/Article/details/gqixlnuwx.sHtML

[Q48] CTE 公用表表达式
来源：http://www.blog.fktsv.cn/Article/details/gpcqauqyu.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://m.share.fktsv.cn/Article/details/gwwlxazak.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://m.share.fktsv.cn/Article/details/gmmolengm.sHtML

[Q49] 更新单行
来源：http://www.blog.bbcook.cn/Article/details/gtsfrhddp.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.share.epnwcf.com/Article/details/grfbssgbs.sHtML

[Q50] 批量更新
来源：http://mobile.tarul.cn/Article/details/glqwtlufv.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://m.share.bbcook.cn/Article/details/gjqpignsm.sHtML

[Q51] 用子查询更新
来源：http://blog.bbcook.cn/Article/details/gpoqguucg.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.blog.vehdjk.com/Article/details/guubdnphv.sHtML

[Q52] 删除指定行
来源：http://www.blog.bbcook.cn/Article/details/gvjinqeuk.sHtML

DELETE FROM users WHERE id = 10;
来源：http://3g.vehdjk.com/Article/details/gvjakatvh.sHtML

[Q53] 按条件删除
来源：http://mobile.tarul.cn/Article/details/goyzdtgwo.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://read.share.bbcook.cn/Article/details/gdnolnkxb.sHtML

[Q54] 清空表
来源：http://www.share.fktsv.cn/Article/details/gljtdjtvh.sHtML

TRUNCATE TABLE logs;
来源：http://3g.tarul.cn/Article/details/gfxaxzcyp.sHtML

[Q55] 排名（并列占位）
来源：http://baike.sjlbkw.cn/Article/details/gdqxivadr.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://3g.yfazqb.com/Article/details/gyhuqjrrr.sHtML

[Q56] 密集排名（并列不占位）
来源：http://blog.tarul.cn/Article/details/gqxdjxwjv.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://3g.bbcook.cn/Article/details/gxtkqrpkg.sHtML

[Q57] 行号
来源：http://baike.epnwcf.com/Article/details/grxovcjja.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://mobile.bbcook.cn/Article/details/gtbzvxhek.sHtML

[Q58] 累计求和
来源：http://www.share.bbcook.cn/Article/details/gdsuxbfri.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://mobile.epnwcf.com/Article/details/gildbtkts.sHtML

[Q59] 分组内累计
来源：http://www.m.share.yfazqb.com/Article/details/gdcuqdlzs.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://mobile.tarul.cn/Article/details/goxwkvtov.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.m.share.vehdjk.com/Article/details/gdaepxiga.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://baike.yfazqb.com/Article/details/gfprtpogh.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://baike.fktsv.cn/Article/details/gznupewoy.sHtML

[Q61] 移动平均
来源：http://www.blog.vehdjk.com/Article/details/gbfarlizt.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://baike.bbcook.cn/Article/details/gicateztd.sHtML

[Q62] 分组占比
来源：http://www.m.share.sjlbkw.cn/Article/details/gzwosesns.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://mobile.yfazqb.com/Article/details/gxvhuytac.sHtML

[Q63] 开启事务
来源：http://m.share.tarul.cn/Article/details/gkyxfliea.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.m.share.epnwcf.com/Article/details/gqwdtfexm.sHtML

[Q64] 提交事务
来源：http://www.share.epnwcf.com/Article/details/glcmmjvka.sHtML

COMMIT;
来源：http://m.share.epnwcf.com/Article/details/gjzpnreje.sHtML

[Q65] 回滚事务
来源：http://mobile.yfazqb.com/Article/details/gzszzamxp.sHtML

ROLLBACK;
来源：http://3g.fktsv.cn/Article/details/gajcwsztr.sHtML

[Q66] 行锁查询
来源：http://www.blog.sjlbkw.cn/Article/details/gosqbnguc.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://3g.fktsv.cn/Article/details/grbcfdnho.sHtML

[Q67] 设置隔离级别
来源：http://wap.yfazqb.com/Article/details/gyxdmcnke.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://3g.sjlbkw.cn/Article/details/gybxoxcaz.sHtML

[Q68] 保存点
来源：http://www.blog.vehdjk.com/Article/details/gjtseonog.sHtML

SAVEPOINT sp1;
来源：http://www.m.share.sjlbkw.cn/Article/details/gjnehvvsc.sHtML

ROLLBACK TO sp1;
来源：http://read.share.yfazqb.com/Article/details/gtqkrkhcx.sHtML

[Q69] 查看执行计划
来源：http://www.blog.yfazqb.com/Article/details/gyfqpiykm.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://blog.yfazqb.com/Article/details/gomshoyxc.sHtML

[Q70] 更新统计信息
来源：http://m.share.sjlbkw.cn/Article/details/gmclbdhdk.sHtML

ANALYZE TABLE users;
来源：http://www.m.share.epnwcf.com/Article/details/gatrydpyr.sHtML

[Q71] 查看建表语句
来源：http://m.share.tarul.cn/Article/details/gpjhentax.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://blog.sjlbkw.cn/Article/details/gfhiimetl.sHtML

[Q72] 查看索引
来源：http://blog.sjlbkw.cn/Article/details/gwhjphlqf.sHtML

SHOW INDEX FROM users;
来源：http://3g.yfazqb.com/Article/details/gcmzeqnjk.sHtML

[Q73] 查看表状态
来源：http://read.share.sjlbkw.cn/Article/details/gomswltri.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.share.yfazqb.com/Article/details/gjrxckwnw.sHtML

[Q74] 强制使用索引
来源：http://m.share.epnwcf.com/Article/details/gdfsmztrh.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://read.share.tarul.cn/Article/details/gpammcdah.sHtML

[Q75] 日期格式化
来源：http://baike.fktsv.cn/Article/details/ggtmdsahd.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.blog.vehdjk.com/Article/details/gctdtohpj.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.blog.tarul.cn/Article/details/gcgestfkz.sHtML

[Q76] 按天统计
来源：http://read.share.sjlbkw.cn/Article/details/gfelspjfy.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://read.share.bbcook.cn/Article/details/gdaqrfhvu.sHtML

[Q77] 时间加减
来源：http://wap.yfazqb.com/Article/details/grplcwnnr.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://blog.vehdjk.com/Article/details/gyawsjore.sHtML

[Q78] 当前时间
来源：http://baike.vehdjk.com/Article/details/gruwtkiyj.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://mobile.sjlbkw.cn/Article/details/gycwviyas.sHtML

[Q79] 字符串拼接
来源：http://www.blog.fktsv.cn/Article/details/gybdndffc.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.blog.tarul.cn/Article/details/gdnbrddea.sHtML

[Q80] 字符串截取
来源：http://3g.epnwcf.com/Article/details/gemmdvmxc.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.m.share.yfazqb.com/Article/details/gvbleuqaa.sHtML

[Q81] 字符串替换
来源：http://www.blog.vehdjk.com/Article/details/goqrjqnhx.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.blog.fktsv.cn/Article/details/gkwlgmlpu.sHtML

[Q82] 字符长度与字节长度
来源：http://mobile.tarul.cn/Article/details/gxqjyktyb.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://read.share.fktsv.cn/Article/details/grdkybbwu.sHtML

[Q83] 大小写转换
来源：http://mobile.vehdjk.com/Article/details/gcitipxfd.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://mobile.fktsv.cn/Article/details/gcqujfvty.sHtML

[Q84] 去除首尾空格
来源：http://www.m.share.yfazqb.com/Article/details/gkrmpodeh.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.m.share.fktsv.cn/Article/details/gcshtrdvo.sHtML

[Q85] 数值取整
来源：http://baike.yfazqb.com/Article/details/gvbluyzaa.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://read.share.fktsv.cn/Article/details/gixgmmfba.sHtML

[Q86] 读取 JSON 字段
来源：http://read.share.vehdjk.com/Article/details/gqeuhvpia.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://mobile.epnwcf.com/Article/details/gkwylhxxi.sHtML

[Q87] JSON 字段做条件
来源：http://blog.epnwcf.com/Article/details/gfydvijax.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://wap.fktsv.cn/Article/details/ghaklluhm.sHtML

[Q88] 行转列（条件聚合）
来源：http://wap.fktsv.cn/Article/details/gnkcmshuk.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.share.bbcook.cn/Article/details/gqvwbcbbn.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://m.share.epnwcf.com/Article/details/gqjfjjuvk.sHtML

[Q89] 判断表是否存在
来源：http://3g.tarul.cn/Article/details/gfycnldnx.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.blog.epnwcf.com/Article/details/gbymecwnj.sHtML

[Q90] 生成序号列
来源：http://www.share.bbcook.cn/Article/details/gkinyiubx.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://read.share.fktsv.cn/Article/details/gbszsyeag.sHtML

================================================================================
来源：http://baike.tarul.cn/Article/details/gdtmrytxw.sHtML

R. Bash 专题
来源：http://baike.vehdjk.com/Article/details/gvgguwaic.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/gnxdwlpeq.sHtML

[R01] shebang 与严格模式
来源：http://m.share.fktsv.cn/Article/details/gkzeynxve.sHtML

#!/usr/bin/env bash
来源：http://www.m.share.vehdjk.com/Article/details/gcswmslvh.sHtML

set -euo pipefail
来源：http://read.share.tarul.cn/Article/details/gkdbiezoi.sHtML

[R02] 变量赋值与使用
来源：http://3g.vehdjk.com/Article/details/gwyxqzqtg.sHtML

name="Tom"; echo "$name"
来源：http://www.m.share.yfazqb.com/Article/details/gpjuzmhnt.sHtML

[R03] 只读变量
来源：http://blog.epnwcf.com/Article/details/goyqdrimz.sHtML

readonly PI=3.14
来源：http://read.share.fktsv.cn/Article/details/gannddssg.sHtML

[R04] 位置参数
来源：http://3g.sjlbkw.cn/Article/details/gtzyrbuhe.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://mobile.yfazqb.com/Article/details/gciursotf.sHtML

[R05] 参数默认值
来源：http://read.share.fktsv.cn/Article/details/gfpalfffl.sHtML

name="${1:-default}"
来源：http://wap.tarul.cn/Article/details/grrdcrlub.sHtML

[R06] 判断命令是否存在
来源：http://blog.vehdjk.com/Article/details/grlfzxuxu.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://blog.tarul.cn/Article/details/gkovinmzy.sHtML

[R07] if 判断文件
来源：http://m.share.epnwcf.com/Article/details/gwacwqxfk.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.share.tarul.cn/Article/details/gtgjlxwey.sHtML

[R08] 数值比较
来源：http://mobile.epnwcf.com/Article/details/goeoeojqo.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://mobile.vehdjk.com/Article/details/gfveombvj.sHtML

[R09] 字符串比较
来源：http://3g.tarul.cn/Article/details/grmcosrbs.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.blog.tarul.cn/Article/details/gamrkmwzw.sHtML

[R10] 正则匹配
来源：http://www.share.vehdjk.com/Article/details/gsjqblvad.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.share.yfazqb.com/Article/details/gjazdfutx.sHtML

[R11] case 多分支
来源：http://3g.epnwcf.com/Article/details/glmffrflc.sHtML

case "$1" in
来源：http://www.blog.epnwcf.com/Article/details/gbfaahura.sHtML

start) echo "启动" ;;
来源：http://www.m.share.yfazqb.com/Article/details/gnhgeucgn.sHtML

stop)  echo "停止" ;;
来源：http://baike.sjlbkw.cn/Article/details/gqkstqthd.sHtML

*)     echo "未知命令" ;;
来源：http://www.share.epnwcf.com/Article/details/gtqylhbfm.sHtML

esac
来源：http://blog.tarul.cn/Article/details/govsedgbe.sHtML

[R12] for 遍历文件
来源：http://3g.sjlbkw.cn/Article/details/ghfmzsewp.sHtML

for f in *.txt; do echo "$f"; done
来源：http://m.share.epnwcf.com/Article/details/gxjcfouny.sHtML

[R13] for 计数循环
来源：http://baike.epnwcf.com/Article/details/gjdslozjd.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://baike.vehdjk.com/Article/details/gedbniekr.sHtML

[R14] C 风格 for
来源：http://www.m.share.bbcook.cn/Article/details/gnxuodduf.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://blog.bbcook.cn/Article/details/gighodmpy.sHtML

[R15] while 逐行读文件
来源：http://m.share.bbcook.cn/Article/details/gbvzdwgxu.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://read.share.yfazqb.com/Article/details/gqamqzbsq.sHtML

[R16] until 等待条件
来源：http://m.share.bbcook.cn/Article/details/gtpjboanv.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.share.epnwcf.com/Article/details/gwybrahte.sHtML

[R17] 数组定义与取值
来源：http://baike.bbcook.cn/Article/details/grqmrvjdz.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.m.share.vehdjk.com/Article/details/guaiownzi.sHtML

[R18] 遍历数组
来源：http://mobile.tarul.cn/Article/details/gfgppsetr.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://read.share.vehdjk.com/Article/details/gpasacbfd.sHtML

[R19] 数组长度
来源：http://blog.tarul.cn/Article/details/gbxkjrjtk.sHtML

echo "${#arr[@]}"
来源：http://www.blog.bbcook.cn/Article/details/guvivdswn.sHtML

[R20] 关联数组（字典）
来源：http://baike.sjlbkw.cn/Article/details/gyylxhomm.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.blog.vehdjk.com/Article/details/gzfnjyghw.sHtML

[R21] 字符串长度
来源：http://baike.bbcook.cn/Article/details/gkfkbgghk.sHtML

echo "${#s}"
来源：http://3g.vehdjk.com/Article/details/gzqnuievs.sHtML

[R22] 截取子串
来源：http://www.m.share.yfazqb.com/Article/details/gaqjjgsmg.sHtML

echo "${s:0:5}"
来源：http://wap.tarul.cn/Article/details/ggglhfxuc.sHtML

[R23] 字符串替换
来源：http://baike.tarul.cn/Article/details/gjazuuynz.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://mobile.vehdjk.com/Article/details/gtpdgloii.sHtML

[R24] 大小写转换
来源：http://www.blog.vehdjk.com/Article/details/gbcjgorfe.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://m.share.tarul.cn/Article/details/grkceyunu.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.share.yfazqb.com/Article/details/glfbypois.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://read.share.yfazqb.com/Article/details/gzgnlunxz.sHtML

[R26] 命令替换
来源：http://read.share.vehdjk.com/Article/details/gbahcwgzw.sHtML

now=$(date +%F); echo "$now"
来源：http://blog.sjlbkw.cn/Article/details/ghawirooc.sHtML

[R27] 算术展开
来源：http://www.share.epnwcf.com/Article/details/gfwlxukuf.sHtML

echo $((1 + 2 * 3))
来源：http://wap.vehdjk.com/Article/details/gzekdyaqj.sHtML

[R28] 浮点运算
来源：http://baike.sjlbkw.cn/Article/details/gfqplozbm.sHtML

echo "scale=2; 10/3" | bc
来源：http://blog.fktsv.cn/Article/details/gswconvxj.sHtML

[R29] 定义函数
来源：http://blog.fktsv.cn/Article/details/gazspdpza.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://mobile.yfazqb.com/Article/details/gqhtrhkvl.sHtML

[R30] 函数返回状态码
来源：http://www.m.share.vehdjk.com/Article/details/gbuszyrwc.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://blog.vehdjk.com/Article/details/gqybztwwq.sHtML

[R31] 局部变量
来源：http://www.blog.tarul.cn/Article/details/govfozpsl.sHtML

f() { local x=1; echo "$x"; }
来源：http://3g.epnwcf.com/Article/details/gthqdqdbt.sHtML

[R32] 参数个数校验
来源：http://mobile.epnwcf.com/Article/details/gzbmezcaa.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://3g.yfazqb.com/Article/details/gwsvcmjsq.sHtML

[R33] 捕获错误并提示行号
来源：http://3g.sjlbkw.cn/Article/details/gmznhomyc.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://blog.epnwcf.com/Article/details/ggcnhhmkk.sHtML

[R34] 退出时清理
来源：http://www.m.share.yfazqb.com/Article/details/gzkywbpbc.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://m.share.tarul.cn/Article/details/gxushvmyv.sHtML

[R35] 后台执行并等待
来源：http://www.m.share.tarul.cn/Article/details/gubedkklr.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://read.share.bbcook.cn/Article/details/gyzpfgtuc.sHtML

[R36] 并发执行多个任务
来源：http://www.share.bbcook.cn/Article/details/gyegbzlcz.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.m.share.sjlbkw.cn/Article/details/galkjpvwm.sHtML

[R37] 把输出赋给变量
来源：http://baike.fktsv.cn/Article/details/gngqvhccv.sHtML

files=$(ls -1)
来源：http://www.blog.bbcook.cn/Article/details/gynbbxtsm.sHtML

[R38] 管道串联
来源：http://www.m.share.sjlbkw.cn/Article/details/gszggkaok.sHtML

cat a.txt | grep -i error | wc -l
来源：http://wap.sjlbkw.cn/Article/details/gfhcckvhr.sHtML

[R39] 重定向标准输出与错误
来源：http://read.share.epnwcf.com/Article/details/gsvocerin.sHtML

cmd > out.log 2>&1
来源：http://read.share.yfazqb.com/Article/details/golkzttwv.sHtML

[R40] 追加写日志
来源：http://www.blog.sjlbkw.cn/Article/details/geoludmsq.sHtML

echo "log" >> out.log
来源：http://blog.fktsv.cn/Article/details/gvurtuhzw.sHtML

[R41] 丢弃输出
来源：http://mobile.tarul.cn/Article/details/gfcmzogdl.sHtML

cmd >/dev/null 2>&1
来源：http://www.blog.epnwcf.com/Article/details/gkcmaakbk.sHtML

[R42] 输入重定向
来源：http://www.share.epnwcf.com/Article/details/gpumegszd.sHtML

wc -l < a.txt
来源：http://3g.bbcook.cn/Article/details/gkmxigjsw.sHtML

[R43] 按名字查找文件
来源：http://www.m.share.bbcook.cn/Article/details/gkdyfnfyp.sHtML

find . -name "*.log" -type f
来源：http://www.m.share.yfazqb.com/Article/details/gavttjgpn.sHtML

[R44] 按修改时间查找
来源：http://blog.sjlbkw.cn/Article/details/gptxkcrxt.sHtML

find . -mtime -7 -type f
来源：http://m.share.bbcook.cn/Article/details/gvcppvpfu.sHtML

[R45] 批量删除
来源：http://baike.bbcook.cn/Article/details/goqcfpdrz.sHtML

find . -name "*.tmp" -delete
来源：http://3g.vehdjk.com/Article/details/gdfeecxzc.sHtML

[R46] 递归替换文件内容
来源：http://m.share.bbcook.cn/Article/details/gcmpqtzmz.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://read.share.fktsv.cn/Article/details/gexjanrxt.sHtML

[R47] sed 单行替换
来源：http://www.blog.fktsv.cn/Article/details/gfogehoql.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://3g.vehdjk.com/Article/details/gqpbywbey.sHtML

[R48] awk 取指定列
来源：http://baike.sjlbkw.cn/Article/details/gxnlwluus.sHtML

awk '{print $1, $3}' a.txt
来源：http://m.share.tarul.cn/Article/details/ggysmxbna.sHtML

[R49] awk 带条件
来源：http://wap.fktsv.cn/Article/details/gdvmasinx.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.m.share.vehdjk.com/Article/details/giowdvpdn.sHtML

[R50] awk 求和
来源：http://baike.vehdjk.com/Article/details/gmcqpxncu.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.m.share.fktsv.cn/Article/details/gwuzbgone.sHtML

[R51] 排序去重取前几
来源：http://m.share.tarul.cn/Article/details/gdifymosx.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://blog.vehdjk.com/Article/details/ghquoyfwl.sHtML

[R52] 统计行数
来源：http://mobile.epnwcf.com/Article/details/gawpvpjyf.sHtML

wc -l a.txt
来源：http://www.m.share.fktsv.cn/Article/details/gcbhojtfg.sHtML

[R53] 查看文件头与实时尾
来源：http://www.share.yfazqb.com/Article/details/gsitkwckg.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://m.share.vehdjk.com/Article/details/gfbbjfjuu.sHtML

[R54] 比较两个文件
来源：http://www.m.share.sjlbkw.cn/Article/details/gfsndgjzy.sHtML

diff a.txt b.txt
来源：http://mobile.tarul.cn/Article/details/gbuuyiycm.sHtML

[R55] 压缩与解压
来源：http://baike.yfazqb.com/Article/details/gfttoaesu.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://read.share.yfazqb.com/Article/details/gmhcwjdqr.sHtML

[R56] 远程拷贝
来源：http://blog.yfazqb.com/Article/details/gsknyrevi.sHtML

scp file user@host:/path/
来源：http://www.m.share.epnwcf.com/Article/details/gmfulrtda.sHtML

[R57] 远程执行命令
来源：http://blog.yfazqb.com/Article/details/gydsmufdn.sHtML

ssh user@host 'uptime'
来源：http://www.blog.sjlbkw.cn/Article/details/gcvzumpur.sHtML

[R58] 下载文件
来源：http://baike.bbcook.cn/Article/details/gfthfrbjm.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://wap.fktsv.cn/Article/details/gjpwszqim.sHtML

[R59] 发 POST JSON
来源：http://www.m.share.fktsv.cn/Article/details/gzlqvxfbt.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://3g.yfazqb.com/Article/details/gypyponsl.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.blog.vehdjk.com/Article/details/gafhznmns.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://read.share.epnwcf.com/Article/details/ggrmzjhxv.sHtML

[R61] 磁盘占用
来源：http://mobile.yfazqb.com/Article/details/gzspcupnr.sHtML

df -h;  du -sh *
来源：http://baike.tarul.cn/Article/details/gyfkokzem.sHtML

[R62] 找最占空间的文件
来源：http://baike.vehdjk.com/Article/details/gfassgnjp.sHtML

du -ah . | sort -rh | head -10
来源：http://blog.bbcook.cn/Article/details/gfdrwwwll.sHtML

[R63] 内存与进程
来源：http://baike.bbcook.cn/Article/details/gxdokhdos.sHtML

free -h;  ps aux | grep nginx
来源：http://mobile.yfazqb.com/Article/details/gkdyvlaqp.sHtML

[R64] 结束进程
来源：http://baike.fktsv.cn/Article/details/gaoddtqvn.sHtML

kill -9 $(pgrep -f app.py)
来源：http://mobile.bbcook.cn/Article/details/gmnrnzqpj.sHtML

[R65] 查看端口占用
来源：http://blog.epnwcf.com/Article/details/glrhlljik.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wap.sjlbkw.cn/Article/details/ggxriwtrr.sHtML

[R66] 定时任务
来源：http://www.share.epnwcf.com/Article/details/gdczqtomu.sHtML

crontab -e;  crontab -l
来源：http://mobile.tarul.cn/Article/details/gdgdczggx.sHtML

[R67] 生成随机十六进制串
来源：http://mobile.tarul.cn/Article/details/gdedmukos.sHtML

openssl rand -hex 16
来源：http://baike.epnwcf.com/Article/details/gnltbyujm.sHtML

[R68] 计算文件校验值
来源：http://m.share.bbcook.cn/Article/details/gusnukqao.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://wap.epnwcf.com/Article/details/gvupmhsuu.sHtML

[R69] 生成随机密码
来源：http://3g.epnwcf.com/Article/details/gocnpnyyk.sHtML

head -c 16 /dev/urandom | base64
来源：http://3g.bbcook.cn/Article/details/gdxkqfiub.sHtML

[R70] 时间戳与互转
来源：http://mobile.sjlbkw.cn/Article/details/gzfibhfsy.sHtML

date +%s;  date -d @1700000000
来源：http://wap.yfazqb.com/Article/details/giadknybu.sHtML

[R71] 日期格式化
来源：http://www.blog.tarul.cn/Article/details/gqhpopepu.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.share.bbcook.cn/Article/details/ggtcebjuj.sHtML

[R72] 等待端口就绪
来源：http://mobile.yfazqb.com/Article/details/gkhrqvksl.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://wap.fktsv.cn/Article/details/gmyigufkb.sHtML

[R73] 分割大日志
来源：http://m.share.fktsv.cn/Article/details/gzjtmszth.sHtML

split -l 1000 big.log part_
来源：http://www.m.share.sjlbkw.cn/Article/details/gtoosygbi.sHtML

[R74] 批量重命名
来源：http://www.share.yfazqb.com/Article/details/gxkhobnni.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://read.share.fktsv.cn/Article/details/grmpmfisg.sHtML

[R75] 导出环境变量
来源：http://m.share.vehdjk.com/Article/details/glkmkudmj.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://wap.yfazqb.com/Article/details/gzdmiorew.sHtML

[R76] 使用临时文件
来源：http://3g.vehdjk.com/Article/details/gzwhhpybo.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.sjlbkw.cn/Article/details/gieshikef.sHtML

[R77] 读取用户输入
来源：http://blog.yfazqb.com/Article/details/gdpxacpzm.sHtML

read -rp "请输入: " ans
来源：http://3g.bbcook.cn/Article/details/gyzguhqnw.sHtML

[R78] 交互式菜单
来源：http://blog.epnwcf.com/Article/details/gzblxrccs.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://3g.tarul.cn/Article/details/grsryanir.sHtML

[R79] 解析命令行选项
来源：http://www.m.share.tarul.cn/Article/details/gqmtrauxu.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://read.share.fktsv.cn/Article/details/gwmjchcyz.sHtML

[R80] 查看脚本执行耗时
来源：http://3g.yfazqb.com/Article/details/guhqdsckx.sHtML

time ./run.sh
来源：http://read.share.yfazqb.com/Article/details/gilsndktk.sHtML

================================================================================
来源：http://baike.tarul.cn/Article/details/ghrwylxqf.sHtML

S. C / C++ 专题
来源：http://mobile.sjlbkw.cn/Article/details/gwwwkduaw.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/gymjuhofk.sHtML

[S01] C：Hello World
来源：http://blog.vehdjk.com/Article/details/gnpemnpym.sHtML

#include <stdio.h>
来源：http://www.blog.yfazqb.com/Article/details/gykfqehdt.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://blog.vehdjk.com/Article/details/gyxpxhnsm.sHtML

[S02] C：变量与格式化输出
来源：http://3g.vehdjk.com/Article/details/ggkabdhht.sHtML

int a = 10; printf("%d\n", a);
来源：http://read.share.bbcook.cn/Article/details/ggymrbmyt.sHtML

[S03] C：读入整数
来源：http://www.blog.tarul.cn/Article/details/gsnzmozlo.sHtML


<!-- 参考信息 -->