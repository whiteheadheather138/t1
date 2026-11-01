代发 wailian999

[Q38] 全外连接（PostgreSQL）
来源：http://read.share.sjlbkw.cn/Article/details/gtwhskmhe.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://3g.tarul.cn/Article/details/gotprfwmc.sHtML

[Q39] 自连接（查上下级）
来源：http://baike.tarul.cn/Article/details/gvzposyyr.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.blog.bbcook.cn/Article/details/gbithfhep.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://read.share.bbcook.cn/Article/details/gkmbkxiwe.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://wap.tarul.cn/Article/details/gtdstcraz.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.m.share.epnwcf.com/Article/details/gfkwxuayn.sHtML

[Q41] 多表连接
来源：http://mobile.epnwcf.com/Article/details/gieoybtqf.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://3g.bbcook.cn/Article/details/gjlldkvgv.sHtML

JOIN users u ON u.id = o.user_id
来源：http://mobile.fktsv.cn/Article/details/gvhnmqfgp.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://mobile.vehdjk.com/Article/details/gerlocmcd.sHtML

[Q42] 连接条件附加过滤
来源：http://m.share.tarul.cn/Article/details/gsnkyxvnt.sHtML

SELECT u.name, o.amount FROM users u
来源：http://baike.sjlbkw.cn/Article/details/guojwgfnf.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.m.share.yfazqb.com/Article/details/gcnmgayrj.sHtML

[Q43] 标量子查询
来源：http://www.share.epnwcf.com/Article/details/gjvjyvgcz.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.share.bbcook.cn/Article/details/gcveqsfut.sHtML

[Q44] IN 子查询
来源：http://www.blog.fktsv.cn/Article/details/gowjkbcti.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://blog.yfazqb.com/Article/details/gsbnglneh.sHtML

[Q45] EXISTS 判断存在
来源：http://read.share.bbcook.cn/Article/details/grdaoodpr.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.bbcook.cn/Article/details/gnosjgwby.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.m.share.bbcook.cn/Article/details/guuducqrk.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.yfazqb.com/Article/details/gtkvqhfcc.sHtML

[Q47] 与平均值比较
来源：http://read.share.vehdjk.com/Article/details/gehnywwew.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.share.fktsv.cn/Article/details/gwjwaheja.sHtML

[Q48] CTE 公用表表达式
来源：http://www.share.fktsv.cn/Article/details/glimlfppc.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.blog.fktsv.cn/Article/details/gnvzlcjfs.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.share.epnwcf.com/Article/details/gvamtznyt.sHtML

[Q49] 更新单行
来源：http://m.share.epnwcf.com/Article/details/gkmwuzeov.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://m.share.vehdjk.com/Article/details/goaliakoe.sHtML

[Q50] 批量更新
来源：http://baike.fktsv.cn/Article/details/gyecrkwju.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://read.share.yfazqb.com/Article/details/gtwzivpwa.sHtML

[Q51] 用子查询更新
来源：http://3g.tarul.cn/Article/details/gqnjyulpo.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.m.share.vehdjk.com/Article/details/gvdnqqtom.sHtML

[Q52] 删除指定行
来源：http://www.share.sjlbkw.cn/Article/details/gilgraquc.sHtML

DELETE FROM users WHERE id = 10;
来源：http://read.share.vehdjk.com/Article/details/gshbvyjlg.sHtML

[Q53] 按条件删除
来源：http://m.share.bbcook.cn/Article/details/gqrbqumey.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.m.share.yfazqb.com/Article/details/gzzdzacwx.sHtML

[Q54] 清空表
来源：http://mobile.fktsv.cn/Article/details/gpkbctuyd.sHtML

TRUNCATE TABLE logs;
来源：http://wap.vehdjk.com/Article/details/gdahttvfs.sHtML

[Q55] 排名（并列占位）
来源：http://mobile.yfazqb.com/Article/details/gdbaorpjq.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://mobile.fktsv.cn/Article/details/gybqgfmsd.sHtML

[Q56] 密集排名（并列不占位）
来源：http://m.share.fktsv.cn/Article/details/gxhilebcf.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://mobile.epnwcf.com/Article/details/gdsyoarho.sHtML

[Q57] 行号
来源：http://www.blog.sjlbkw.cn/Article/details/gvdhhotcq.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://baike.vehdjk.com/Article/details/gfbjlndfr.sHtML

[Q58] 累计求和
来源：http://read.share.yfazqb.com/Article/details/gqksxrxvj.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://baike.epnwcf.com/Article/details/gswcsqufc.sHtML

[Q59] 分组内累计
来源：http://www.blog.sjlbkw.cn/Article/details/gdylpsdtb.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.m.share.bbcook.cn/Article/details/grbmaenob.sHtML

[Q60] 取上一行 / 下一行
来源：http://mobile.fktsv.cn/Article/details/grdmqlboy.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.m.share.yfazqb.com/Article/details/gkufdlvai.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://3g.vehdjk.com/Article/details/gwoeytvrp.sHtML

[Q61] 移动平均
来源：http://blog.bbcook.cn/Article/details/gtchdgyny.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://mobile.epnwcf.com/Article/details/gnptrudxc.sHtML

[Q62] 分组占比
来源：http://www.share.epnwcf.com/Article/details/gqetbbllk.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://baike.tarul.cn/Article/details/gjvtspbzd.sHtML

[Q63] 开启事务
来源：http://read.share.tarul.cn/Article/details/ghtuvwuvq.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://read.share.vehdjk.com/Article/details/gguyztvuz.sHtML

[Q64] 提交事务
来源：http://m.share.yfazqb.com/Article/details/gqthbysgm.sHtML

COMMIT;
来源：http://wap.bbcook.cn/Article/details/gylerxsjh.sHtML

[Q65] 回滚事务
来源：http://www.blog.tarul.cn/Article/details/gvicjkwpa.sHtML

ROLLBACK;
来源：http://wap.tarul.cn/Article/details/gseqeuflo.sHtML

[Q66] 行锁查询
来源：http://wap.sjlbkw.cn/Article/details/gpokvyzhu.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://3g.vehdjk.com/Article/details/gbydubymo.sHtML

[Q67] 设置隔离级别
来源：http://3g.tarul.cn/Article/details/gzgxnuavm.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.blog.yfazqb.com/Article/details/gitlhajjg.sHtML

[Q68] 保存点
来源：http://www.blog.vehdjk.com/Article/details/gllhrmavw.sHtML

SAVEPOINT sp1;
来源：http://mobile.vehdjk.com/Article/details/gtcrczskc.sHtML

ROLLBACK TO sp1;
来源：http://read.share.epnwcf.com/Article/details/gkdmzkabw.sHtML

[Q69] 查看执行计划
来源：http://baike.yfazqb.com/Article/details/gcwboaduf.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://wap.fktsv.cn/Article/details/gbzfkbthn.sHtML

[Q70] 更新统计信息
来源：http://blog.bbcook.cn/Article/details/gqawjvszv.sHtML

ANALYZE TABLE users;
来源：http://www.blog.epnwcf.com/Article/details/gkfeeryyf.sHtML

[Q71] 查看建表语句
来源：http://baike.epnwcf.com/Article/details/gyxuoshtf.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://wap.yfazqb.com/Article/details/gpgywhcjn.sHtML

[Q72] 查看索引
来源：http://www.share.fktsv.cn/Article/details/goccxuasg.sHtML

SHOW INDEX FROM users;
来源：http://3g.epnwcf.com/Article/details/ggrftvwfj.sHtML

[Q73] 查看表状态
来源：http://www.share.bbcook.cn/Article/details/gefwnhnra.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://baike.epnwcf.com/Article/details/gbvyuynxh.sHtML

[Q74] 强制使用索引
来源：http://read.share.epnwcf.com/Article/details/gqexupngs.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://3g.sjlbkw.cn/Article/details/glhqioewt.sHtML

[Q75] 日期格式化
来源：http://mobile.fktsv.cn/Article/details/gzgvtfkxy.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://blog.yfazqb.com/Article/details/gpdqkgogs.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://baike.sjlbkw.cn/Article/details/gzzvpvpde.sHtML

[Q76] 按天统计
来源：http://www.blog.bbcook.cn/Article/details/gkygwnouw.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.share.tarul.cn/Article/details/grmjjfxws.sHtML

[Q77] 时间加减
来源：http://www.m.share.tarul.cn/Article/details/grspbjfhp.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.share.fktsv.cn/Article/details/gfwxpwnxd.sHtML

[Q78] 当前时间
来源：http://blog.epnwcf.com/Article/details/gqmdfuyek.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://read.share.tarul.cn/Article/details/gezirprco.sHtML

[Q79] 字符串拼接
来源：http://baike.tarul.cn/Article/details/ggjiqhsst.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://mobile.fktsv.cn/Article/details/gbcbfceff.sHtML

[Q80] 字符串截取
来源：http://m.share.epnwcf.com/Article/details/greyqddht.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://m.share.sjlbkw.cn/Article/details/gimhinpgw.sHtML

[Q81] 字符串替换
来源：http://m.share.sjlbkw.cn/Article/details/gqtfxjyns.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://blog.bbcook.cn/Article/details/ghogjkwro.sHtML

[Q82] 字符长度与字节长度
来源：http://blog.yfazqb.com/Article/details/ghzenvonn.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.share.epnwcf.com/Article/details/gubyuakcw.sHtML

[Q83] 大小写转换
来源：http://baike.tarul.cn/Article/details/grldkxdps.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://blog.vehdjk.com/Article/details/gczvttiyb.sHtML

[Q84] 去除首尾空格
来源：http://blog.sjlbkw.cn/Article/details/gdxwxzflb.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.share.yfazqb.com/Article/details/gugzpqyqd.sHtML

[Q85] 数值取整
来源：http://www.blog.yfazqb.com/Article/details/gaukomabo.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://mobile.vehdjk.com/Article/details/gjnbkytut.sHtML

[Q86] 读取 JSON 字段
来源：http://read.share.fktsv.cn/Article/details/gkzctbbfp.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://3g.sjlbkw.cn/Article/details/guqdyhypp.sHtML

[Q87] JSON 字段做条件
来源：http://baike.epnwcf.com/Article/details/gjcplfjkp.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://wap.bbcook.cn/Article/details/gbmbonxbt.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.blog.bbcook.cn/Article/details/gjlxqljwz.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://3g.bbcook.cn/Article/details/gpexoiluh.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://m.share.vehdjk.com/Article/details/gqgvbsbgt.sHtML

[Q89] 判断表是否存在
来源：http://mobile.tarul.cn/Article/details/gttuqieiu.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://mobile.tarul.cn/Article/details/gckxpjitj.sHtML

[Q90] 生成序号列
来源：http://mobile.vehdjk.com/Article/details/gfjnlnhzq.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.blog.bbcook.cn/Article/details/gpmfmpsvd.sHtML

================================================================================
来源：http://www.blog.vehdjk.com/Article/details/gbyniskkr.sHtML

R. Bash 专题
来源：http://www.m.share.yfazqb.com/Article/details/gwtzppvvb.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/gwpavjfca.sHtML

[R01] shebang 与严格模式
来源：http://read.share.epnwcf.com/Article/details/gpmxkkarn.sHtML

#!/usr/bin/env bash
来源：http://mobile.yfazqb.com/Article/details/gvqgoqlpe.sHtML

set -euo pipefail
来源：http://3g.yfazqb.com/Article/details/grwcrvkrh.sHtML

[R02] 变量赋值与使用
来源：http://www.m.share.bbcook.cn/Article/details/ggunptulx.sHtML

name="Tom"; echo "$name"
来源：http://m.share.tarul.cn/Article/details/gzivdpfoc.sHtML

[R03] 只读变量
来源：http://m.share.fktsv.cn/Article/details/gddnceoys.sHtML

readonly PI=3.14
来源：http://3g.fktsv.cn/Article/details/gchhglfhx.sHtML

[R04] 位置参数
来源：http://mobile.vehdjk.com/Article/details/gvnufnxhl.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://baike.vehdjk.com/Article/details/gvnvavpbn.sHtML

[R05] 参数默认值
来源：http://m.share.tarul.cn/Article/details/gkarqrhvo.sHtML

name="${1:-default}"
来源：http://read.share.sjlbkw.cn/Article/details/gveopxyny.sHtML

[R06] 判断命令是否存在
来源：http://www.m.share.tarul.cn/Article/details/gahjjaeoj.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.share.tarul.cn/Article/details/gipoozfsa.sHtML

[R07] if 判断文件
来源：http://3g.sjlbkw.cn/Article/details/gfeutxadg.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://wap.vehdjk.com/Article/details/grbnkdgxu.sHtML

[R08] 数值比较
来源：http://m.share.bbcook.cn/Article/details/gmabrgztn.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://m.share.yfazqb.com/Article/details/gtbrgiyzw.sHtML

[R09] 字符串比较
来源：http://m.share.bbcook.cn/Article/details/gczeepyet.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://blog.sjlbkw.cn/Article/details/gzibucgyz.sHtML

[R10] 正则匹配
来源：http://blog.vehdjk.com/Article/details/gewfwaavv.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.m.share.fktsv.cn/Article/details/gsuatuayo.sHtML

[R11] case 多分支
来源：http://www.blog.tarul.cn/Article/details/gjdovvbzv.sHtML

case "$1" in
来源：http://www.blog.fktsv.cn/Article/details/gabnfumxx.sHtML

start) echo "启动" ;;
来源：http://read.share.vehdjk.com/Article/details/galmrovui.sHtML

stop)  echo "停止" ;;
来源：http://3g.bbcook.cn/Article/details/gvhyrjten.sHtML

*)     echo "未知命令" ;;
来源：http://mobile.sjlbkw.cn/Article/details/gpxdwlvqy.sHtML

esac
来源：http://m.share.epnwcf.com/Article/details/gpsnvpjwr.sHtML

[R12] for 遍历文件
来源：http://m.share.vehdjk.com/Article/details/gshhjnrvd.sHtML

for f in *.txt; do echo "$f"; done
来源：http://blog.tarul.cn/Article/details/gumtqtzrn.sHtML

[R13] for 计数循环
来源：http://m.share.tarul.cn/Article/details/gjaswrcbw.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.m.share.epnwcf.com/Article/details/glplrebyj.sHtML

[R14] C 风格 for
来源：http://read.share.tarul.cn/Article/details/gngzamkhx.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://3g.fktsv.cn/Article/details/gqlvhlckm.sHtML

[R15] while 逐行读文件
来源：http://mobile.epnwcf.com/Article/details/gokqupkhp.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://read.share.tarul.cn/Article/details/gxhfegwmq.sHtML

[R16] until 等待条件
来源：http://read.share.yfazqb.com/Article/details/gebzklawc.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.blog.tarul.cn/Article/details/gvaryskwx.sHtML

[R17] 数组定义与取值
来源：http://baike.epnwcf.com/Article/details/gezaiyjam.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://m.share.epnwcf.com/Article/details/grawitxul.sHtML

[R18] 遍历数组
来源：http://m.share.bbcook.cn/Article/details/grsmshgtj.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://blog.fktsv.cn/Article/details/gsojncpbc.sHtML

[R19] 数组长度
来源：http://read.share.fktsv.cn/Article/details/ghbkcicjh.sHtML

echo "${#arr[@]}"
来源：http://3g.sjlbkw.cn/Article/details/gtfmyjufs.sHtML

[R20] 关联数组（字典）
来源：http://www.share.epnwcf.com/Article/details/gzsrbykrz.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://wap.bbcook.cn/Article/details/gkwndlfpc.sHtML

[R21] 字符串长度
来源：http://www.share.sjlbkw.cn/Article/details/gvrsghfnr.sHtML

echo "${#s}"
来源：http://blog.yfazqb.com/Article/details/gbkdybyot.sHtML

[R22] 截取子串
来源：http://mobile.tarul.cn/Article/details/gcwvurwxv.sHtML

echo "${s:0:5}"
来源：http://www.blog.vehdjk.com/Article/details/gcklzwjgt.sHtML

[R23] 字符串替换
来源：http://blog.tarul.cn/Article/details/gkwtqnsnj.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://mobile.bbcook.cn/Article/details/gvuxysvtk.sHtML

[R24] 大小写转换
来源：http://www.share.fktsv.cn/Article/details/gsjpqdrim.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://read.share.yfazqb.com/Article/details/giwvmgqis.sHtML

[R25] 去后缀 / 去前缀
来源：http://read.share.vehdjk.com/Article/details/gcdzfnyzu.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://blog.tarul.cn/Article/details/gcwysdlhb.sHtML

[R26] 命令替换
来源：http://www.share.tarul.cn/Article/details/ggfzeffue.sHtML

now=$(date +%F); echo "$now"
来源：http://wap.bbcook.cn/Article/details/gsppydbyb.sHtML

[R27] 算术展开
来源：http://www.share.fktsv.cn/Article/details/ganvdlyzr.sHtML

echo $((1 + 2 * 3))
来源：http://blog.yfazqb.com/Article/details/ghfdvxhnl.sHtML

[R28] 浮点运算
来源：http://wap.yfazqb.com/Article/details/gnhbosquf.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.share.fktsv.cn/Article/details/gqydouiks.sHtML

[R29] 定义函数
来源：http://m.share.sjlbkw.cn/Article/details/gyybxrqfv.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://baike.tarul.cn/Article/details/gqtswnnrn.sHtML

[R30] 函数返回状态码
来源：http://read.share.vehdjk.com/Article/details/gvfnloiqg.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.blog.epnwcf.com/Article/details/glmjcxjuy.sHtML

[R31] 局部变量
来源：http://baike.sjlbkw.cn/Article/details/gwivyfirb.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.share.bbcook.cn/Article/details/gencyhipy.sHtML

[R32] 参数个数校验
来源：http://wap.vehdjk.com/Article/details/ggjtzbstg.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://mobile.yfazqb.com/Article/details/gxqoujqlw.sHtML

[R33] 捕获错误并提示行号
来源：http://blog.epnwcf.com/Article/details/gdnecrawh.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://wap.fktsv.cn/Article/details/gqnoyjmnj.sHtML

[R34] 退出时清理
来源：http://m.share.yfazqb.com/Article/details/gsosjgngr.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://m.share.tarul.cn/Article/details/gtqgpshhd.sHtML

[R35] 后台执行并等待
来源：http://mobile.bbcook.cn/Article/details/gkxmjhtou.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://read.share.epnwcf.com/Article/details/gigiizvxs.sHtML

[R36] 并发执行多个任务
来源：http://mobile.tarul.cn/Article/details/gounuwmsl.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.m.share.bbcook.cn/Article/details/grpatneaf.sHtML

[R37] 把输出赋给变量
来源：http://wap.vehdjk.com/Article/details/grkrvakqe.sHtML

files=$(ls -1)
来源：http://wap.tarul.cn/Article/details/gishoxlqg.sHtML

[R38] 管道串联
来源：http://baike.vehdjk.com/Article/details/gcakfwqxv.sHtML

cat a.txt | grep -i error | wc -l
来源：http://read.share.yfazqb.com/Article/details/gpztjdgia.sHtML

[R39] 重定向标准输出与错误
来源：http://wap.sjlbkw.cn/Article/details/gfcvgtyiy.sHtML

cmd > out.log 2>&1
来源：http://wap.tarul.cn/Article/details/gkhlyyadz.sHtML

[R40] 追加写日志
来源：http://m.share.tarul.cn/Article/details/gghyostjh.sHtML

echo "log" >> out.log
来源：http://www.blog.epnwcf.com/Article/details/gcdhplvxu.sHtML

[R41] 丢弃输出
来源：http://baike.vehdjk.com/Article/details/gyfddykbe.sHtML

cmd >/dev/null 2>&1
来源：http://3g.sjlbkw.cn/Article/details/gkdfobnce.sHtML

[R42] 输入重定向
来源：http://3g.sjlbkw.cn/Article/details/geqseutxv.sHtML

wc -l < a.txt
来源：http://read.share.tarul.cn/Article/details/gzvhoqubm.sHtML

[R43] 按名字查找文件
来源：http://www.blog.vehdjk.com/Article/details/gmwsfvfsq.sHtML

find . -name "*.log" -type f
来源：http://mobile.vehdjk.com/Article/details/gjxmwcnyr.sHtML

[R44] 按修改时间查找
来源：http://wap.fktsv.cn/Article/details/gkusfyxpg.sHtML

find . -mtime -7 -type f
来源：http://blog.epnwcf.com/Article/details/ghfwanpwo.sHtML

[R45] 批量删除
来源：http://read.share.vehdjk.com/Article/details/gylprbwsr.sHtML

find . -name "*.tmp" -delete
来源：http://3g.yfazqb.com/Article/details/gtqfngnfy.sHtML

[R46] 递归替换文件内容
来源：http://read.share.sjlbkw.cn/Article/details/gupxtyngd.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://m.share.fktsv.cn/Article/details/gdbmrwrat.sHtML

[R47] sed 单行替换
来源：http://www.m.share.sjlbkw.cn/Article/details/gsqtiavoo.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://wap.bbcook.cn/Article/details/gxzbtivuj.sHtML

[R48] awk 取指定列
来源：http://blog.sjlbkw.cn/Article/details/greeyxlpk.sHtML

awk '{print $1, $3}' a.txt
来源：http://blog.yfazqb.com/Article/details/gqnwtztup.sHtML

[R49] awk 带条件
来源：http://wap.sjlbkw.cn/Article/details/gqtbaxdjo.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://baike.epnwcf.com/Article/details/gibadbnay.sHtML

[R50] awk 求和
来源：http://baike.fktsv.cn/Article/details/gvrudkpbz.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://mobile.fktsv.cn/Article/details/gtdciwanp.sHtML

[R51] 排序去重取前几
来源：http://3g.vehdjk.com/Article/details/ghtbpedny.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://blog.yfazqb.com/Article/details/gmtrmsnrq.sHtML

[R52] 统计行数
来源：http://www.m.share.tarul.cn/Article/details/guudmkkal.sHtML

wc -l a.txt
来源：http://read.share.sjlbkw.cn/Article/details/gxvzboapg.sHtML

[R53] 查看文件头与实时尾
来源：http://3g.vehdjk.com/Article/details/guqdvhqny.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://wap.epnwcf.com/Article/details/gnuwxmaqb.sHtML

[R54] 比较两个文件
来源：http://www.blog.bbcook.cn/Article/details/gezyuwmoy.sHtML

diff a.txt b.txt
来源：http://wap.bbcook.cn/Article/details/gihaxoqkm.sHtML

[R55] 压缩与解压
来源：http://baike.vehdjk.com/Article/details/gyznwferx.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.blog.vehdjk.com/Article/details/gabgrmsar.sHtML

[R56] 远程拷贝
来源：http://www.m.share.epnwcf.com/Article/details/gkpccwnvv.sHtML

scp file user@host:/path/
来源：http://wap.tarul.cn/Article/details/gkdzdjcza.sHtML

[R57] 远程执行命令
来源：http://baike.vehdjk.com/Article/details/gjnpjvmfo.sHtML

ssh user@host 'uptime'
来源：http://blog.tarul.cn/Article/details/gglokzkbl.sHtML

[R58] 下载文件
来源：http://www.blog.epnwcf.com/Article/details/gmpbjubsv.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.share.vehdjk.com/Article/details/gphelsuuj.sHtML

[R59] 发 POST JSON
来源：http://www.share.fktsv.cn/Article/details/gaevpcpfd.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wap.vehdjk.com/Article/details/guhwtrqxy.sHtML

[R60] 只看 HTTP 状态码
来源：http://baike.vehdjk.com/Article/details/gejubrwsd.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.share.vehdjk.com/Article/details/gqlpiemdp.sHtML

[R61] 磁盘占用
来源：http://www.blog.fktsv.cn/Article/details/gbseddett.sHtML

df -h;  du -sh *
来源：http://www.m.share.sjlbkw.cn/Article/details/gtbgtmffk.sHtML

[R62] 找最占空间的文件
来源：http://read.share.bbcook.cn/Article/details/gmouvmgng.sHtML

du -ah . | sort -rh | head -10
来源：http://www.blog.epnwcf.com/Article/details/gxfcnftym.sHtML

[R63] 内存与进程
来源：http://baike.tarul.cn/Article/details/gmgjcmvbq.sHtML

free -h;  ps aux | grep nginx
来源：http://3g.tarul.cn/Article/details/gclludrmz.sHtML

[R64] 结束进程
来源：http://blog.bbcook.cn/Article/details/gmaolxuix.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.m.share.epnwcf.com/Article/details/gypgutozg.sHtML

[R65] 查看端口占用
来源：http://mobile.tarul.cn/Article/details/gukldzvoz.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://read.share.yfazqb.com/Article/details/gcpgrirfa.sHtML

[R66] 定时任务
来源：http://read.share.fktsv.cn/Article/details/goxeuacsn.sHtML

crontab -e;  crontab -l
来源：http://read.share.fktsv.cn/Article/details/gjmlxtngp.sHtML

[R67] 生成随机十六进制串
来源：http://read.share.bbcook.cn/Article/details/gsochuohm.sHtML

openssl rand -hex 16
来源：http://www.m.share.fktsv.cn/Article/details/glftibpjl.sHtML

[R68] 计算文件校验值
来源：http://mobile.bbcook.cn/Article/details/gxogeiwhg.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://wap.tarul.cn/Article/details/gpdocrkja.sHtML

[R69] 生成随机密码
来源：http://wap.bbcook.cn/Article/details/gspwlfvur.sHtML

head -c 16 /dev/urandom | base64
来源：http://mobile.tarul.cn/Article/details/gofvsidbq.sHtML

[R70] 时间戳与互转
来源：http://wap.sjlbkw.cn/Article/details/gfhipayql.sHtML

date +%s;  date -d @1700000000
来源：http://baike.sjlbkw.cn/Article/details/gakgisqwf.sHtML

[R71] 日期格式化
来源：http://m.share.epnwcf.com/Article/details/gdjbeznws.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://m.share.bbcook.cn/Article/details/gjklpwciz.sHtML

[R72] 等待端口就绪
来源：http://3g.epnwcf.com/Article/details/gqoffaxga.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://mobile.tarul.cn/Article/details/gjlpxvsou.sHtML

[R73] 分割大日志
来源：http://m.share.epnwcf.com/Article/details/gdfmcaplh.sHtML

split -l 1000 big.log part_
来源：http://www.m.share.bbcook.cn/Article/details/gqxyhkpxi.sHtML

[R74] 批量重命名
来源：http://read.share.fktsv.cn/Article/details/gzmxdoftm.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://baike.vehdjk.com/Article/details/gtwiqtzmf.sHtML

[R75] 导出环境变量
来源：http://www.blog.epnwcf.com/Article/details/grurbmcjt.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://wap.fktsv.cn/Article/details/gelijcopr.sHtML

[R76] 使用临时文件
来源：http://mobile.vehdjk.com/Article/details/gqhuhpszp.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.share.epnwcf.com/Article/details/gxbmeuqui.sHtML

[R77] 读取用户输入
来源：http://www.blog.vehdjk.com/Article/details/gxqnwnpjr.sHtML

read -rp "请输入: " ans
来源：http://www.m.share.tarul.cn/Article/details/gyernnaoh.sHtML

[R78] 交互式菜单
来源：http://3g.tarul.cn/Article/details/gtmbtztis.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://m.share.yfazqb.com/Article/details/geqdtsjam.sHtML

[R79] 解析命令行选项
来源：http://baike.tarul.cn/Article/details/ghpswxczc.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://baike.bbcook.cn/Article/details/galvaadtu.sHtML

[R80] 查看脚本执行耗时
来源：http://blog.vehdjk.com/Article/details/gmikttuau.sHtML

time ./run.sh
来源：http://baike.sjlbkw.cn/Article/details/gcwggwvsn.sHtML

================================================================================
来源：http://3g.vehdjk.com/Article/details/gstwrysvk.sHtML

S. C / C++ 专题
来源：http://baike.bbcook.cn/Article/details/gpriodxjv.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/ginfzsacd.sHtML

[S01] C：Hello World
来源：http://www.share.bbcook.cn/Article/details/grxrplpoh.sHtML

#include <stdio.h>
来源：http://3g.bbcook.cn/Article/details/gfpaidhsa.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://mobile.yfazqb.com/Article/details/goeetztjn.sHtML

[S02] C：变量与格式化输出
来源：http://wap.vehdjk.com/Article/details/gtquspgpu.sHtML

int a = 10; printf("%d\n", a);
来源：http://wap.sjlbkw.cn/Article/details/ggnassoou.sHtML

[S03] C：读入整数
来源：http://3g.epnwcf.com/Article/details/gkvithcvs.sHtML

int x; scanf("%d", &x);
来源：http://www.share.bbcook.cn/Article/details/gzoeumifz.sHtML

[S04] C：字符串复制
来源：http://m.share.epnwcf.com/Article/details/gixwkdgtr.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://mobile.bbcook.cn/Article/details/gvswxbymi.sHtML

[S05] C：字符串长度
来源：http://read.share.epnwcf.com/Article/details/gfemjimei.sHtML

strlen(s)
来源：http://baike.epnwcf.com/Article/details/gahwutdsz.sHtML

[S06] C：字符串比较
来源：http://www.m.share.vehdjk.com/Article/details/guxyocqhv.sHtML

strcmp(a, b) == 0
来源：http://read.share.tarul.cn/Article/details/gohertxww.sHtML

[S07] C：数组遍历求和
来源：http://www.blog.vehdjk.com/Article/details/gkycroicd.sHtML


<!-- 参考信息 -->