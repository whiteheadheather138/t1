代发 wailian999

[Q33] 多列分组
来源：http://m.share.tarul.cn/Article/details/gjzocsjea.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.share.vehdjk.com/Article/details/gpsgnlort.sHtML

[Q34] 每组取第一条
来源：http://blog.epnwcf.com/Article/details/gowrlxezp.sHtML

SELECT * FROM (
来源：http://www.blog.tarul.cn/Article/details/geukcufqt.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://m.share.sjlbkw.cn/Article/details/gcciblkdp.sHtML

) t WHERE rn = 1;
来源：http://m.share.vehdjk.com/Article/details/gizvblsgi.sHtML

[Q35] 内连接
来源：http://wap.tarul.cn/Article/details/gfyuzlobh.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://wap.sjlbkw.cn/Article/details/gnejgwqsd.sHtML

[Q36] 左连接
来源：http://www.m.share.sjlbkw.cn/Article/details/gueswrdwm.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://mobile.yfazqb.com/Article/details/gorkulhjh.sHtML

[Q37] 右连接
来源：http://m.share.sjlbkw.cn/Article/details/gmxbsrejl.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://wap.epnwcf.com/Article/details/gjekpzzwo.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://m.share.bbcook.cn/Article/details/ggpofxchu.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://m.share.sjlbkw.cn/Article/details/grvktrlpp.sHtML

[Q39] 自连接（查上下级）
来源：http://baike.bbcook.cn/Article/details/gwwplkymi.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://baike.epnwcf.com/Article/details/gffrcyezx.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://m.share.fktsv.cn/Article/details/gnydlxrur.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://blog.sjlbkw.cn/Article/details/gnlmrwwew.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://m.share.epnwcf.com/Article/details/ggryydbdd.sHtML

[Q41] 多表连接
来源：http://www.m.share.bbcook.cn/Article/details/gugvfxwvk.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://mobile.fktsv.cn/Article/details/gbxufihnx.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.share.vehdjk.com/Article/details/gamvrxfqi.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://3g.vehdjk.com/Article/details/gruhcqaxo.sHtML

[Q42] 连接条件附加过滤
来源：http://blog.vehdjk.com/Article/details/gpefrllzv.sHtML

SELECT u.name, o.amount FROM users u
来源：http://baike.fktsv.cn/Article/details/gdfkcospv.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://wap.tarul.cn/Article/details/gaenhpkmr.sHtML

[Q43] 标量子查询
来源：http://3g.epnwcf.com/Article/details/gswtzeeqp.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://3g.bbcook.cn/Article/details/gtsiyzdpa.sHtML

[Q44] IN 子查询
来源：http://m.share.bbcook.cn/Article/details/gzcgoebya.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.blog.fktsv.cn/Article/details/gfhqndqnu.sHtML

[Q45] EXISTS 判断存在
来源：http://baike.sjlbkw.cn/Article/details/gijfjqdqk.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.sjlbkw.cn/Article/details/gedhiumku.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://baike.yfazqb.com/Article/details/gjvdglqnl.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.fktsv.cn/Article/details/gvxunohku.sHtML

[Q47] 与平均值比较
来源：http://www.share.sjlbkw.cn/Article/details/gogqvgpzr.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://mobile.bbcook.cn/Article/details/govcexhod.sHtML

[Q48] CTE 公用表表达式
来源：http://m.share.bbcook.cn/Article/details/gyounadbt.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://m.share.vehdjk.com/Article/details/gdjyjkxbw.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://m.share.fktsv.cn/Article/details/gervpgcbi.sHtML

[Q49] 更新单行
来源：http://www.blog.epnwcf.com/Article/details/gwmomplxb.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.blog.sjlbkw.cn/Article/details/ghdzbkcrw.sHtML

[Q50] 批量更新
来源：http://mobile.bbcook.cn/Article/details/gcbbjkqyc.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.m.share.epnwcf.com/Article/details/gkqwfwctw.sHtML

[Q51] 用子查询更新
来源：http://www.share.bbcook.cn/Article/details/gudmmgjyg.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.blog.yfazqb.com/Article/details/gkpjqhtem.sHtML

[Q52] 删除指定行
来源：http://mobile.bbcook.cn/Article/details/gmrxiptct.sHtML

DELETE FROM users WHERE id = 10;
来源：http://baike.fktsv.cn/Article/details/gtylvczpd.sHtML

[Q53] 按条件删除
来源：http://read.share.sjlbkw.cn/Article/details/gcafpmeip.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://3g.vehdjk.com/Article/details/grpbrmoql.sHtML

[Q54] 清空表
来源：http://www.m.share.sjlbkw.cn/Article/details/guhzpbzaw.sHtML

TRUNCATE TABLE logs;
来源：http://baike.tarul.cn/Article/details/gepfgijgz.sHtML

[Q55] 排名（并列占位）
来源：http://baike.bbcook.cn/Article/details/ggnxqwjdq.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://mobile.fktsv.cn/Article/details/gayhifepd.sHtML

[Q56] 密集排名（并列不占位）
来源：http://mobile.fktsv.cn/Article/details/gvqbhkavj.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.blog.bbcook.cn/Article/details/gnjhijvgq.sHtML

[Q57] 行号
来源：http://www.blog.tarul.cn/Article/details/gboccvdia.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.share.fktsv.cn/Article/details/gojelpuih.sHtML

[Q58] 累计求和
来源：http://read.share.yfazqb.com/Article/details/gfrqlfmnx.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://3g.fktsv.cn/Article/details/gzcfruthd.sHtML

[Q59] 分组内累计
来源：http://read.share.bbcook.cn/Article/details/gvzdrubiu.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.share.yfazqb.com/Article/details/gujlspvlw.sHtML

[Q60] 取上一行 / 下一行
来源：http://read.share.sjlbkw.cn/Article/details/gfymetbeg.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://read.share.tarul.cn/Article/details/gwsengkwj.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.share.epnwcf.com/Article/details/grocxedyr.sHtML

[Q61] 移动平均
来源：http://3g.fktsv.cn/Article/details/geoaotqmo.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://blog.sjlbkw.cn/Article/details/gtiwbtjzp.sHtML

[Q62] 分组占比
来源：http://www.share.tarul.cn/Article/details/gxiqfcouu.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.blog.sjlbkw.cn/Article/details/grxhsdudd.sHtML

[Q63] 开启事务
来源：http://blog.vehdjk.com/Article/details/grxurivtn.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://baike.fktsv.cn/Article/details/guipstfww.sHtML

[Q64] 提交事务
来源：http://blog.sjlbkw.cn/Article/details/ghwyoozeg.sHtML

COMMIT;
来源：http://blog.sjlbkw.cn/Article/details/gdnqmobql.sHtML

[Q65] 回滚事务
来源：http://m.share.yfazqb.com/Article/details/gtjcsooxy.sHtML

ROLLBACK;
来源：http://read.share.vehdjk.com/Article/details/gxwoioyso.sHtML

[Q66] 行锁查询
来源：http://www.blog.tarul.cn/Article/details/gsnbrqjdt.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://mobile.yfazqb.com/Article/details/gyzrlxiui.sHtML

[Q67] 设置隔离级别
来源：http://www.share.yfazqb.com/Article/details/gscdlrtux.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://wap.vehdjk.com/Article/details/gqkxptyms.sHtML

[Q68] 保存点
来源：http://blog.yfazqb.com/Article/details/gvwraydwk.sHtML

SAVEPOINT sp1;
来源：http://www.m.share.sjlbkw.cn/Article/details/gqzdfhxwn.sHtML

ROLLBACK TO sp1;
来源：http://3g.fktsv.cn/Article/details/ggzdqjtrx.sHtML

[Q69] 查看执行计划
来源：http://m.share.bbcook.cn/Article/details/gupmlbdch.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://3g.epnwcf.com/Article/details/ghoeomzdw.sHtML

[Q70] 更新统计信息
来源：http://blog.vehdjk.com/Article/details/gjlonckgd.sHtML

ANALYZE TABLE users;
来源：http://m.share.epnwcf.com/Article/details/guzgjowek.sHtML

[Q71] 查看建表语句
来源：http://www.blog.vehdjk.com/Article/details/gtalkpthe.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://read.share.tarul.cn/Article/details/glkmrpxlb.sHtML

[Q72] 查看索引
来源：http://blog.bbcook.cn/Article/details/grgwoqfvu.sHtML

SHOW INDEX FROM users;
来源：http://www.share.sjlbkw.cn/Article/details/gjfbjgpxb.sHtML

[Q73] 查看表状态
来源：http://blog.sjlbkw.cn/Article/details/gkdcpopho.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.blog.yfazqb.com/Article/details/gziwxozws.sHtML

[Q74] 强制使用索引
来源：http://3g.vehdjk.com/Article/details/gdknghgwj.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://blog.tarul.cn/Article/details/gzhffsrsu.sHtML

[Q75] 日期格式化
来源：http://blog.vehdjk.com/Article/details/gdxqpecym.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.share.sjlbkw.cn/Article/details/ghkjjesgi.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://3g.vehdjk.com/Article/details/goyfhflgg.sHtML

[Q76] 按天统计
来源：http://wap.tarul.cn/Article/details/gktlpsfau.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.share.epnwcf.com/Article/details/gfdperkvk.sHtML

[Q77] 时间加减
来源：http://m.share.bbcook.cn/Article/details/gakwlcvds.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://baike.yfazqb.com/Article/details/gcbbyatzq.sHtML

[Q78] 当前时间
来源：http://blog.tarul.cn/Article/details/gtlwyloxi.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://read.share.fktsv.cn/Article/details/gzjvgkufl.sHtML

[Q79] 字符串拼接
来源：http://wap.epnwcf.com/Article/details/gndvyquko.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://3g.fktsv.cn/Article/details/gyxsyrlml.sHtML

[Q80] 字符串截取
来源：http://read.share.yfazqb.com/Article/details/gpoqywjue.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://mobile.tarul.cn/Article/details/gpydcovxv.sHtML

[Q81] 字符串替换
来源：http://mobile.bbcook.cn/Article/details/gvgdrrdfd.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://mobile.vehdjk.com/Article/details/gvmpnkklo.sHtML

[Q82] 字符长度与字节长度
来源：http://mobile.tarul.cn/Article/details/gejtqelih.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.m.share.vehdjk.com/Article/details/gqgnhypwq.sHtML

[Q83] 大小写转换
来源：http://m.share.sjlbkw.cn/Article/details/gbkgqzjcz.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.share.vehdjk.com/Article/details/grgxhjpmt.sHtML

[Q84] 去除首尾空格
来源：http://www.share.yfazqb.com/Article/details/gyjuvktdv.sHtML

SELECT TRIM(name) FROM users;
来源：http://wap.epnwcf.com/Article/details/gwkaqgusi.sHtML

[Q85] 数值取整
来源：http://3g.sjlbkw.cn/Article/details/gvefoslin.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://blog.epnwcf.com/Article/details/gfyxbtdkb.sHtML

[Q86] 读取 JSON 字段
来源：http://wap.bbcook.cn/Article/details/gkmxiccnx.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://mobile.bbcook.cn/Article/details/goabwwpho.sHtML

[Q87] JSON 字段做条件
来源：http://3g.vehdjk.com/Article/details/gjfobaere.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://read.share.vehdjk.com/Article/details/gsdzfxdcz.sHtML

[Q88] 行转列（条件聚合）
来源：http://read.share.fktsv.cn/Article/details/gprtcatyu.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.share.sjlbkw.cn/Article/details/gkhzzqxpg.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.blog.vehdjk.com/Article/details/gtxwwjwzu.sHtML

[Q89] 判断表是否存在
来源：http://blog.tarul.cn/Article/details/gdoyijywp.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.m.share.sjlbkw.cn/Article/details/gwrjxaspj.sHtML

[Q90] 生成序号列
来源：http://read.share.bbcook.cn/Article/details/giftolbuv.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.m.share.epnwcf.com/Article/details/gzyuwsskz.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/gzxlnrtzw.sHtML

R. Bash 专题
来源：http://baike.vehdjk.com/Article/details/guvanxzfu.sHtML

================================================================================
来源：http://www.share.epnwcf.com/Article/details/gpzttwwte.sHtML

[R01] shebang 与严格模式
来源：http://www.share.vehdjk.com/Article/details/gehulbqny.sHtML

#!/usr/bin/env bash
来源：http://www.m.share.fktsv.cn/Article/details/ggdiywlbr.sHtML

set -euo pipefail
来源：http://mobile.vehdjk.com/Article/details/gmekqytri.sHtML

[R02] 变量赋值与使用
来源：http://read.share.sjlbkw.cn/Article/details/gunhngwwa.sHtML

name="Tom"; echo "$name"
来源：http://www.share.fktsv.cn/Article/details/gmeugywos.sHtML

[R03] 只读变量
来源：http://mobile.yfazqb.com/Article/details/gctsmwckz.sHtML

readonly PI=3.14
来源：http://m.share.bbcook.cn/Article/details/gnrpgqooa.sHtML

[R04] 位置参数
来源：http://www.blog.tarul.cn/Article/details/gelssjojp.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://read.share.yfazqb.com/Article/details/gzmgzzxlm.sHtML

[R05] 参数默认值
来源：http://m.share.yfazqb.com/Article/details/gjpxzmbjd.sHtML

name="${1:-default}"
来源：http://mobile.vehdjk.com/Article/details/gumphesih.sHtML

[R06] 判断命令是否存在
来源：http://www.blog.tarul.cn/Article/details/gmfemqqyq.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://wap.fktsv.cn/Article/details/gaeclawfo.sHtML

[R07] if 判断文件
来源：http://wap.fktsv.cn/Article/details/glusgzxxp.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://3g.fktsv.cn/Article/details/gtepgjroi.sHtML

[R08] 数值比较
来源：http://3g.bbcook.cn/Article/details/gtvpijsrr.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://3g.tarul.cn/Article/details/gppoekcoy.sHtML

[R09] 字符串比较
来源：http://blog.tarul.cn/Article/details/gzkvokmta.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://read.share.tarul.cn/Article/details/gyxfcetev.sHtML

[R10] 正则匹配
来源：http://blog.fktsv.cn/Article/details/gpqxtzsac.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://blog.sjlbkw.cn/Article/details/glnlvfwze.sHtML

[R11] case 多分支
来源：http://3g.vehdjk.com/Article/details/gmckvnjuk.sHtML

case "$1" in
来源：http://mobile.epnwcf.com/Article/details/ggxixlndi.sHtML

start) echo "启动" ;;
来源：http://m.share.epnwcf.com/Article/details/geirotmfw.sHtML

stop)  echo "停止" ;;
来源：http://blog.epnwcf.com/Article/details/gjdazooae.sHtML

*)     echo "未知命令" ;;
来源：http://blog.bbcook.cn/Article/details/gclhjplbf.sHtML

esac
来源：http://www.share.epnwcf.com/Article/details/gfmxxbtsk.sHtML

[R12] for 遍历文件
来源：http://mobile.fktsv.cn/Article/details/giynjejqv.sHtML

for f in *.txt; do echo "$f"; done
来源：http://baike.sjlbkw.cn/Article/details/gfaqijrkb.sHtML

[R13] for 计数循环
来源：http://wap.epnwcf.com/Article/details/gfwepfltz.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://m.share.epnwcf.com/Article/details/gvteapqib.sHtML

[R14] C 风格 for
来源：http://m.share.bbcook.cn/Article/details/gesrwpfff.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://read.share.sjlbkw.cn/Article/details/gxwtzdhhw.sHtML

[R15] while 逐行读文件
来源：http://www.blog.bbcook.cn/Article/details/gssjaarve.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.share.bbcook.cn/Article/details/gtscoknko.sHtML

[R16] until 等待条件
来源：http://wap.fktsv.cn/Article/details/gnikzmroi.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://read.share.epnwcf.com/Article/details/gxrtgbqvm.sHtML

[R17] 数组定义与取值
来源：http://baike.tarul.cn/Article/details/gpfpnrtjo.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.share.yfazqb.com/Article/details/gypgznbbd.sHtML

[R18] 遍历数组
来源：http://www.blog.bbcook.cn/Article/details/gtvaiuskc.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.blog.vehdjk.com/Article/details/gnhyzbyvg.sHtML

[R19] 数组长度
来源：http://m.share.vehdjk.com/Article/details/gjdsjodeg.sHtML

echo "${#arr[@]}"
来源：http://read.share.fktsv.cn/Article/details/goqrfbexy.sHtML

[R20] 关联数组（字典）
来源：http://wap.tarul.cn/Article/details/girtmcsoa.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.m.share.yfazqb.com/Article/details/gqvqtiuum.sHtML

[R21] 字符串长度
来源：http://read.share.bbcook.cn/Article/details/gvjnnoagc.sHtML

echo "${#s}"
来源：http://baike.bbcook.cn/Article/details/gnyonvfhn.sHtML

[R22] 截取子串
来源：http://wap.epnwcf.com/Article/details/geklidhbg.sHtML

echo "${s:0:5}"
来源：http://wap.bbcook.cn/Article/details/gdgojignk.sHtML

[R23] 字符串替换
来源：http://mobile.tarul.cn/Article/details/gpdrfsjtn.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://blog.fktsv.cn/Article/details/gxcvqkmrj.sHtML

[R24] 大小写转换
来源：http://read.share.epnwcf.com/Article/details/gwyahgilp.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.share.tarul.cn/Article/details/gbmatvnug.sHtML

[R25] 去后缀 / 去前缀
来源：http://baike.vehdjk.com/Article/details/gbsoclqqm.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://baike.epnwcf.com/Article/details/grzvwcnuo.sHtML

[R26] 命令替换
来源：http://read.share.tarul.cn/Article/details/gnyjouuqf.sHtML

now=$(date +%F); echo "$now"
来源：http://www.blog.yfazqb.com/Article/details/gohxsxnsq.sHtML

[R27] 算术展开
来源：http://blog.bbcook.cn/Article/details/gjsgttgkw.sHtML

echo $((1 + 2 * 3))
来源：http://m.share.epnwcf.com/Article/details/gagpubted.sHtML

[R28] 浮点运算
来源：http://3g.bbcook.cn/Article/details/gwhdtmbgj.sHtML

echo "scale=2; 10/3" | bc
来源：http://m.share.bbcook.cn/Article/details/ghshugssb.sHtML

[R29] 定义函数
来源：http://baike.vehdjk.com/Article/details/gzbtaemqx.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.blog.yfazqb.com/Article/details/gsuxqyfjb.sHtML

[R30] 函数返回状态码
来源：http://blog.fktsv.cn/Article/details/gjwljxrfi.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://3g.yfazqb.com/Article/details/gsohoqphd.sHtML

[R31] 局部变量
来源：http://www.blog.vehdjk.com/Article/details/gmxleibng.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.share.sjlbkw.cn/Article/details/gtvwsqqbq.sHtML

[R32] 参数个数校验
来源：http://www.blog.bbcook.cn/Article/details/gvmdybmcd.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.share.sjlbkw.cn/Article/details/gpdhpiadw.sHtML

[R33] 捕获错误并提示行号
来源：http://3g.epnwcf.com/Article/details/gstrkeyka.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://blog.tarul.cn/Article/details/gmywvcwvb.sHtML

[R34] 退出时清理
来源：http://blog.tarul.cn/Article/details/gbguhayfp.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.yfazqb.com/Article/details/gtoewkpks.sHtML

[R35] 后台执行并等待
来源：http://mobile.epnwcf.com/Article/details/gvbcjuzaf.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://m.share.sjlbkw.cn/Article/details/gdhzzzdmn.sHtML

[R36] 并发执行多个任务
来源：http://www.share.yfazqb.com/Article/details/gvgcqaiqi.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.share.sjlbkw.cn/Article/details/gvzantuhv.sHtML

[R37] 把输出赋给变量
来源：http://baike.yfazqb.com/Article/details/gmxglcyuz.sHtML

files=$(ls -1)
来源：http://3g.fktsv.cn/Article/details/grzdybmza.sHtML

[R38] 管道串联
来源：http://www.blog.epnwcf.com/Article/details/gtrfekohf.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.blog.epnwcf.com/Article/details/gjwuzeooh.sHtML

[R39] 重定向标准输出与错误
来源：http://m.share.bbcook.cn/Article/details/gysswwieg.sHtML

cmd > out.log 2>&1
来源：http://www.share.epnwcf.com/Article/details/gfadfuijh.sHtML

[R40] 追加写日志
来源：http://read.share.fktsv.cn/Article/details/gehcdiyso.sHtML

echo "log" >> out.log
来源：http://www.blog.bbcook.cn/Article/details/gpfoergsg.sHtML

[R41] 丢弃输出
来源：http://3g.epnwcf.com/Article/details/gowrdsjbd.sHtML

cmd >/dev/null 2>&1
来源：http://www.m.share.tarul.cn/Article/details/gptpdhlzb.sHtML

[R42] 输入重定向
来源：http://www.blog.epnwcf.com/Article/details/ghecpmnhx.sHtML

wc -l < a.txt
来源：http://baike.fktsv.cn/Article/details/gtpplpwck.sHtML

[R43] 按名字查找文件
来源：http://www.blog.tarul.cn/Article/details/gboadgsvj.sHtML

find . -name "*.log" -type f
来源：http://read.share.vehdjk.com/Article/details/gurpxwcep.sHtML

[R44] 按修改时间查找
来源：http://www.share.tarul.cn/Article/details/gkhgefyqf.sHtML

find . -mtime -7 -type f
来源：http://www.share.tarul.cn/Article/details/gsbehzeem.sHtML

[R45] 批量删除
来源：http://www.share.fktsv.cn/Article/details/ggesfiwnr.sHtML

find . -name "*.tmp" -delete
来源：http://www.blog.sjlbkw.cn/Article/details/gtmpbzzgb.sHtML

[R46] 递归替换文件内容
来源：http://baike.vehdjk.com/Article/details/gwfyfenlb.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.blog.vehdjk.com/Article/details/ghnqofgre.sHtML

[R47] sed 单行替换
来源：http://www.blog.sjlbkw.cn/Article/details/giygqwhtu.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://3g.epnwcf.com/Article/details/guapsmkgv.sHtML

[R48] awk 取指定列
来源：http://3g.tarul.cn/Article/details/gcuobqyqs.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.m.share.vehdjk.com/Article/details/gksbpalba.sHtML

[R49] awk 带条件
来源：http://wap.yfazqb.com/Article/details/gqyrrqhsh.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.share.bbcook.cn/Article/details/glqhknwze.sHtML

[R50] awk 求和
来源：http://mobile.vehdjk.com/Article/details/gpcsjsium.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.share.tarul.cn/Article/details/gyhlgbroy.sHtML

[R51] 排序去重取前几
来源：http://blog.bbcook.cn/Article/details/gnmntrhce.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://3g.sjlbkw.cn/Article/details/gglshcnff.sHtML

[R52] 统计行数
来源：http://3g.bbcook.cn/Article/details/gjloalgil.sHtML

wc -l a.txt
来源：http://wap.epnwcf.com/Article/details/gcuazofkp.sHtML

[R53] 查看文件头与实时尾
来源：http://www.m.share.vehdjk.com/Article/details/gvqwxjsun.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.blog.yfazqb.com/Article/details/gtwdwgnek.sHtML

[R54] 比较两个文件
来源：http://baike.fktsv.cn/Article/details/ggrvqokfo.sHtML

diff a.txt b.txt
来源：http://www.blog.vehdjk.com/Article/details/gmcjqjoix.sHtML

[R55] 压缩与解压
来源：http://read.share.fktsv.cn/Article/details/gwcgxqpip.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://blog.sjlbkw.cn/Article/details/gntbdglkm.sHtML

[R56] 远程拷贝
来源：http://3g.sjlbkw.cn/Article/details/gahrmvark.sHtML

scp file user@host:/path/
来源：http://www.m.share.tarul.cn/Article/details/ghqudxrjt.sHtML

[R57] 远程执行命令
来源：http://blog.fktsv.cn/Article/details/gxjlfoxrv.sHtML

ssh user@host 'uptime'
来源：http://baike.tarul.cn/Article/details/guxgslxtp.sHtML

[R58] 下载文件
来源：http://3g.bbcook.cn/Article/details/gtjgagtet.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.blog.fktsv.cn/Article/details/gpiwoubvm.sHtML

[R59] 发 POST JSON
来源：http://baike.vehdjk.com/Article/details/gsjvacjyo.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://read.share.bbcook.cn/Article/details/ghyisilsf.sHtML

[R60] 只看 HTTP 状态码
来源：http://mobile.epnwcf.com/Article/details/gqsadrvkd.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mobile.fktsv.cn/Article/details/gnsncuryz.sHtML

[R61] 磁盘占用
来源：http://read.share.epnwcf.com/Article/details/gqyqmhnjk.sHtML

df -h;  du -sh *
来源：http://read.share.sjlbkw.cn/Article/details/gydhrbgpc.sHtML

[R62] 找最占空间的文件
来源：http://www.blog.sjlbkw.cn/Article/details/ghliicdnn.sHtML

du -ah . | sort -rh | head -10
来源：http://read.share.epnwcf.com/Article/details/ghvltmpfy.sHtML

[R63] 内存与进程
来源：http://www.share.tarul.cn/Article/details/gbfazommv.sHtML

free -h;  ps aux | grep nginx
来源：http://www.share.sjlbkw.cn/Article/details/gzysjhcnm.sHtML

[R64] 结束进程
来源：http://www.m.share.sjlbkw.cn/Article/details/gforplxap.sHtML

kill -9 $(pgrep -f app.py)
来源：http://3g.bbcook.cn/Article/details/gizooenwn.sHtML

[R65] 查看端口占用
来源：http://www.share.epnwcf.com/Article/details/glzdtvuus.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://baike.tarul.cn/Article/details/gtkreffic.sHtML

[R66] 定时任务
来源：http://blog.bbcook.cn/Article/details/gpyixpsal.sHtML

crontab -e;  crontab -l
来源：http://3g.sjlbkw.cn/Article/details/grjojsmpp.sHtML

[R67] 生成随机十六进制串
来源：http://www.share.yfazqb.com/Article/details/gvkpikjfz.sHtML

openssl rand -hex 16
来源：http://3g.sjlbkw.cn/Article/details/gaqihuhdn.sHtML

[R68] 计算文件校验值
来源：http://m.share.epnwcf.com/Article/details/ghxkqvnkc.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://mobile.bbcook.cn/Article/details/gxjniuigq.sHtML

[R69] 生成随机密码
来源：http://www.share.tarul.cn/Article/details/gjipryyks.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.share.epnwcf.com/Article/details/ghkbikxmo.sHtML

[R70] 时间戳与互转
来源：http://read.share.tarul.cn/Article/details/gupcynyyp.sHtML

date +%s;  date -d @1700000000
来源：http://mobile.epnwcf.com/Article/details/gpeoaihlk.sHtML

[R71] 日期格式化
来源：http://wap.epnwcf.com/Article/details/gfkuuycvf.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://wap.epnwcf.com/Article/details/govbswtvk.sHtML

[R72] 等待端口就绪
来源：http://read.share.bbcook.cn/Article/details/gxtaxpihj.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.blog.yfazqb.com/Article/details/gjzmwfdyx.sHtML

[R73] 分割大日志
来源：http://www.share.sjlbkw.cn/Article/details/gdsxgahth.sHtML

split -l 1000 big.log part_
来源：http://read.share.bbcook.cn/Article/details/goqswzkyl.sHtML

[R74] 批量重命名
来源：http://www.blog.vehdjk.com/Article/details/gnejuybax.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://mobile.tarul.cn/Article/details/gzqggrwsi.sHtML

[R75] 导出环境变量
来源：http://www.m.share.sjlbkw.cn/Article/details/gqvardlbq.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.share.epnwcf.com/Article/details/guthfnair.sHtML

[R76] 使用临时文件
来源：http://read.share.bbcook.cn/Article/details/gadhtkibv.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.epnwcf.com/Article/details/givjsrrjv.sHtML

[R77] 读取用户输入
来源：http://blog.vehdjk.com/Article/details/gevwntjah.sHtML

read -rp "请输入: " ans
来源：http://www.blog.yfazqb.com/Article/details/gwitknsru.sHtML

[R78] 交互式菜单
来源：http://www.blog.tarul.cn/Article/details/gwhtoqcvs.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://3g.bbcook.cn/Article/details/gpcbfwpmy.sHtML

[R79] 解析命令行选项
来源：http://www.share.fktsv.cn/Article/details/gypbgqzlm.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.blog.epnwcf.com/Article/details/gukiimqix.sHtML

[R80] 查看脚本执行耗时
来源：http://baike.epnwcf.com/Article/details/gaymgeyan.sHtML

time ./run.sh
来源：http://m.share.epnwcf.com/Article/details/ggzsetcsr.sHtML

================================================================================
来源：http://www.m.share.tarul.cn/Article/details/gpafnqkoq.sHtML

S. C / C++ 专题
来源：http://www.m.share.sjlbkw.cn/Article/details/gstiquytb.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/gurtpetor.sHtML

[S01] C：Hello World
来源：http://www.share.epnwcf.com/Article/details/gvcwwanli.sHtML

#include <stdio.h>
来源：http://www.share.epnwcf.com/Article/details/ghtmczxes.sHtML


<!-- 参考信息 -->