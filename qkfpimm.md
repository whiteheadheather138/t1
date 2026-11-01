代发 wailian999

[Q38] 全外连接（PostgreSQL）
来源：http://3g.vehdjk.com/Article/details/gxswasofc.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.m.share.sjlbkw.cn/Article/details/goevypcol.sHtML

[Q39] 自连接（查上下级）
来源：http://3g.vehdjk.com/Article/details/gnuducuyi.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.share.fktsv.cn/Article/details/gqimfpzuv.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://baike.sjlbkw.cn/Article/details/gyrrrixmk.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://mobile.epnwcf.com/Article/details/ghuwqkubn.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://read.share.vehdjk.com/Article/details/gvcvclcsr.sHtML

[Q41] 多表连接
来源：http://www.share.epnwcf.com/Article/details/gncnekldr.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://read.share.fktsv.cn/Article/details/gnschlzix.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.blog.tarul.cn/Article/details/gtegcxsoz.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://baike.epnwcf.com/Article/details/gborpaxfg.sHtML

[Q42] 连接条件附加过滤
来源：http://blog.yfazqb.com/Article/details/gttlisbjt.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.m.share.sjlbkw.cn/Article/details/gwmyjaddl.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://baike.tarul.cn/Article/details/gvhxkusxb.sHtML

[Q43] 标量子查询
来源：http://m.share.epnwcf.com/Article/details/gzuzgecsd.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://mobile.fktsv.cn/Article/details/glzxlmwva.sHtML

[Q44] IN 子查询
来源：http://www.blog.vehdjk.com/Article/details/ggzlpaqbb.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://wap.bbcook.cn/Article/details/gnfripyln.sHtML

[Q45] EXISTS 判断存在
来源：http://blog.bbcook.cn/Article/details/gdxryxjvy.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.fktsv.cn/Article/details/gquooeyif.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://3g.epnwcf.com/Article/details/gschiybiv.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.vehdjk.com/Article/details/gyvtvsuaw.sHtML

[Q47] 与平均值比较
来源：http://read.share.bbcook.cn/Article/details/gbueatxfw.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://blog.tarul.cn/Article/details/gulfuprso.sHtML

[Q48] CTE 公用表表达式
来源：http://www.share.vehdjk.com/Article/details/gmechsifp.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://blog.fktsv.cn/Article/details/gbocwejss.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://wap.epnwcf.com/Article/details/gdffxuebh.sHtML

[Q49] 更新单行
来源：http://www.m.share.vehdjk.com/Article/details/gbyupukgk.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://baike.yfazqb.com/Article/details/gsrhcvmng.sHtML

[Q50] 批量更新
来源：http://wap.epnwcf.com/Article/details/gucjwsxsa.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.share.tarul.cn/Article/details/gpvohhwnn.sHtML

[Q51] 用子查询更新
来源：http://blog.sjlbkw.cn/Article/details/gzopgnwss.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.blog.tarul.cn/Article/details/gzppgxshz.sHtML

[Q52] 删除指定行
来源：http://blog.fktsv.cn/Article/details/gfwokrckj.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.share.epnwcf.com/Article/details/gwbpcbdzi.sHtML

[Q53] 按条件删除
来源：http://www.share.bbcook.cn/Article/details/gmwndpxwc.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://baike.fktsv.cn/Article/details/gpuacnrvq.sHtML

[Q54] 清空表
来源：http://m.share.bbcook.cn/Article/details/gnkdnvqrl.sHtML

TRUNCATE TABLE logs;
来源：http://wap.yfazqb.com/Article/details/glmzouwja.sHtML

[Q55] 排名（并列占位）
来源：http://baike.fktsv.cn/Article/details/gxenxelcw.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.blog.vehdjk.com/Article/details/gyrkleeeq.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.blog.fktsv.cn/Article/details/gipuflbca.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://blog.sjlbkw.cn/Article/details/gsaqjkpia.sHtML

[Q57] 行号
来源：http://www.share.epnwcf.com/Article/details/gdjpnelqo.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.blog.yfazqb.com/Article/details/gvellptms.sHtML

[Q58] 累计求和
来源：http://www.blog.bbcook.cn/Article/details/guyqlzquu.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.share.sjlbkw.cn/Article/details/gfdpstjqm.sHtML

[Q59] 分组内累计
来源：http://www.blog.vehdjk.com/Article/details/gtornzjhr.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://wap.sjlbkw.cn/Article/details/gapjmedur.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.m.share.sjlbkw.cn/Article/details/gnvdmbecx.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://baike.yfazqb.com/Article/details/ghangsiza.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://blog.fktsv.cn/Article/details/gnpmxmdqy.sHtML

[Q61] 移动平均
来源：http://3g.yfazqb.com/Article/details/gguhlfxpn.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://wap.epnwcf.com/Article/details/gtkdapspv.sHtML

[Q62] 分组占比
来源：http://www.share.bbcook.cn/Article/details/gwlepjkyq.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://blog.vehdjk.com/Article/details/gkmylblpk.sHtML

[Q63] 开启事务
来源：http://baike.vehdjk.com/Article/details/gnotdhrmr.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://wap.fktsv.cn/Article/details/gddopcesm.sHtML

[Q64] 提交事务
来源：http://3g.bbcook.cn/Article/details/gnzaomwbf.sHtML

COMMIT;
来源：http://3g.yfazqb.com/Article/details/gtxvkcxcw.sHtML

[Q65] 回滚事务
来源：http://baike.fktsv.cn/Article/details/gmjduqple.sHtML

ROLLBACK;
来源：http://www.m.share.sjlbkw.cn/Article/details/gzqmwfuap.sHtML

[Q66] 行锁查询
来源：http://blog.vehdjk.com/Article/details/gncfpyuxp.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.m.share.fktsv.cn/Article/details/gxbftyxxx.sHtML

[Q67] 设置隔离级别
来源：http://read.share.yfazqb.com/Article/details/gnssyswzo.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://m.share.fktsv.cn/Article/details/gnikqlezv.sHtML

[Q68] 保存点
来源：http://baike.tarul.cn/Article/details/geikubfcu.sHtML

SAVEPOINT sp1;
来源：http://m.share.yfazqb.com/Article/details/gqqwxduro.sHtML

ROLLBACK TO sp1;
来源：http://wap.fktsv.cn/Article/details/gobjxaxqf.sHtML

[Q69] 查看执行计划
来源：http://read.share.fktsv.cn/Article/details/giecutnnt.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.share.epnwcf.com/Article/details/gvbafjyke.sHtML

[Q70] 更新统计信息
来源：http://baike.vehdjk.com/Article/details/ggrangcik.sHtML

ANALYZE TABLE users;
来源：http://m.share.yfazqb.com/Article/details/gomczcdgv.sHtML

[Q71] 查看建表语句
来源：http://blog.epnwcf.com/Article/details/gmovvvzsc.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.blog.yfazqb.com/Article/details/gaztdnjlc.sHtML

[Q72] 查看索引
来源：http://blog.yfazqb.com/Article/details/grcqfcfjx.sHtML

SHOW INDEX FROM users;
来源：http://mobile.epnwcf.com/Article/details/gsxjpgcou.sHtML

[Q73] 查看表状态
来源：http://3g.epnwcf.com/Article/details/gubcrnplb.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.blog.yfazqb.com/Article/details/giyulkacv.sHtML

[Q74] 强制使用索引
来源：http://m.share.vehdjk.com/Article/details/gtpihgxko.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://mobile.epnwcf.com/Article/details/girchtlng.sHtML

[Q75] 日期格式化
来源：http://wap.bbcook.cn/Article/details/gnoolnbxf.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://m.share.yfazqb.com/Article/details/gscvrjfqa.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.blog.fktsv.cn/Article/details/gyqqdtjfk.sHtML

[Q76] 按天统计
来源：http://read.share.fktsv.cn/Article/details/gakrvpvwj.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://read.share.epnwcf.com/Article/details/ggxbcmlcj.sHtML

[Q77] 时间加减
来源：http://blog.vehdjk.com/Article/details/gesyhefxa.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://read.share.tarul.cn/Article/details/gayriwldo.sHtML

[Q78] 当前时间
来源：http://www.blog.sjlbkw.cn/Article/details/gdlkthctz.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://wap.bbcook.cn/Article/details/ggpeiknms.sHtML

[Q79] 字符串拼接
来源：http://www.share.bbcook.cn/Article/details/gfrhpffwm.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.blog.tarul.cn/Article/details/gfbigjcgm.sHtML

[Q80] 字符串截取
来源：http://m.share.tarul.cn/Article/details/gwkwqbebv.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://blog.vehdjk.com/Article/details/grbaebtit.sHtML

[Q81] 字符串替换
来源：http://wap.epnwcf.com/Article/details/gjmsebkfn.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://m.share.tarul.cn/Article/details/gbcszemfa.sHtML

[Q82] 字符长度与字节长度
来源：http://www.share.sjlbkw.cn/Article/details/gqxflfruc.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.share.vehdjk.com/Article/details/gclleesvd.sHtML

[Q83] 大小写转换
来源：http://read.share.bbcook.cn/Article/details/grohlxgct.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.blog.fktsv.cn/Article/details/gkdievfoy.sHtML

[Q84] 去除首尾空格
来源：http://www.share.tarul.cn/Article/details/gajrejyrh.sHtML

SELECT TRIM(name) FROM users;
来源：http://mobile.sjlbkw.cn/Article/details/gqgjbsszl.sHtML

[Q85] 数值取整
来源：http://www.m.share.vehdjk.com/Article/details/ghnoclzqw.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.m.share.tarul.cn/Article/details/gavewbiwu.sHtML

[Q86] 读取 JSON 字段
来源：http://read.share.epnwcf.com/Article/details/gupxztyvp.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://read.share.tarul.cn/Article/details/gdlxmbqqd.sHtML

[Q87] JSON 字段做条件
来源：http://mobile.yfazqb.com/Article/details/gujyahqqh.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://m.share.fktsv.cn/Article/details/glwogixtr.sHtML

[Q88] 行转列（条件聚合）
来源：http://m.share.epnwcf.com/Article/details/gsxmpcbvx.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://mobile.epnwcf.com/Article/details/glvldhywx.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://blog.tarul.cn/Article/details/gljribssr.sHtML

[Q89] 判断表是否存在
来源：http://www.share.sjlbkw.cn/Article/details/gcwlzbyrn.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.m.share.fktsv.cn/Article/details/gbxbxpouj.sHtML

[Q90] 生成序号列
来源：http://blog.vehdjk.com/Article/details/gntutcarf.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://read.share.yfazqb.com/Article/details/gbcvnwveb.sHtML

================================================================================
来源：http://www.m.share.sjlbkw.cn/Article/details/grfrblxrg.sHtML

R. Bash 专题
来源：http://www.share.epnwcf.com/Article/details/gidtehwvs.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/ghpvguyoz.sHtML

[R01] shebang 与严格模式
来源：http://3g.epnwcf.com/Article/details/gmxmbugva.sHtML

#!/usr/bin/env bash
来源：http://m.share.epnwcf.com/Article/details/gvepmlvbo.sHtML

set -euo pipefail
来源：http://wap.sjlbkw.cn/Article/details/gacmuijwx.sHtML

[R02] 变量赋值与使用
来源：http://www.m.share.fktsv.cn/Article/details/gxsgnxvgz.sHtML

name="Tom"; echo "$name"
来源：http://www.m.share.epnwcf.com/Article/details/giwiqatxl.sHtML

[R03] 只读变量
来源：http://www.blog.bbcook.cn/Article/details/gsrzhjjvo.sHtML

readonly PI=3.14
来源：http://3g.vehdjk.com/Article/details/gqhfogjzq.sHtML

[R04] 位置参数
来源：http://blog.fktsv.cn/Article/details/gfijimhwy.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://read.share.sjlbkw.cn/Article/details/gkuxsmduj.sHtML

[R05] 参数默认值
来源：http://blog.vehdjk.com/Article/details/gnkptpolm.sHtML

name="${1:-default}"
来源：http://3g.epnwcf.com/Article/details/gjtziifev.sHtML

[R06] 判断命令是否存在
来源：http://www.share.bbcook.cn/Article/details/gcueyommb.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://read.share.fktsv.cn/Article/details/ghqdgklse.sHtML

[R07] if 判断文件
来源：http://read.share.tarul.cn/Article/details/gvjjcnpno.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://mobile.vehdjk.com/Article/details/gzkfizgqe.sHtML

[R08] 数值比较
来源：http://www.m.share.yfazqb.com/Article/details/gifzttvky.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://wap.vehdjk.com/Article/details/gkadbiuhx.sHtML

[R09] 字符串比较
来源：http://3g.vehdjk.com/Article/details/gfittutrc.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://3g.tarul.cn/Article/details/glrksiabs.sHtML

[R10] 正则匹配
来源：http://www.share.vehdjk.com/Article/details/grsygfufa.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://3g.fktsv.cn/Article/details/gbhrekrmp.sHtML

[R11] case 多分支
来源：http://blog.vehdjk.com/Article/details/gjxntmfpk.sHtML

case "$1" in
来源：http://mobile.sjlbkw.cn/Article/details/grlmtqtle.sHtML

start) echo "启动" ;;
来源：http://3g.sjlbkw.cn/Article/details/gaqmyrrvw.sHtML

stop)  echo "停止" ;;
来源：http://mobile.tarul.cn/Article/details/gsxxzbotn.sHtML

*)     echo "未知命令" ;;
来源：http://wap.epnwcf.com/Article/details/gvgwwsyac.sHtML

esac
来源：http://www.share.tarul.cn/Article/details/gyspiwfnz.sHtML

[R12] for 遍历文件
来源：http://wap.sjlbkw.cn/Article/details/gzwogabsv.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.m.share.vehdjk.com/Article/details/gtasywpau.sHtML

[R13] for 计数循环
来源：http://www.m.share.vehdjk.com/Article/details/gpbplrwvy.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.share.yfazqb.com/Article/details/gtcoetbal.sHtML

[R14] C 风格 for
来源：http://www.blog.bbcook.cn/Article/details/gjtqepgqp.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.share.fktsv.cn/Article/details/glgvbolvf.sHtML

[R15] while 逐行读文件
来源：http://m.share.vehdjk.com/Article/details/gkrqbsipq.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.blog.epnwcf.com/Article/details/gkoskmadb.sHtML

[R16] until 等待条件
来源：http://m.share.bbcook.cn/Article/details/gnnkhecjw.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://m.share.yfazqb.com/Article/details/gpilyovfr.sHtML

[R17] 数组定义与取值
来源：http://mobile.yfazqb.com/Article/details/gjzdrdcby.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://wap.vehdjk.com/Article/details/ghgfczgvk.sHtML

[R18] 遍历数组
来源：http://m.share.vehdjk.com/Article/details/gyobximgu.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://blog.fktsv.cn/Article/details/gxhsqykas.sHtML

[R19] 数组长度
来源：http://wap.fktsv.cn/Article/details/gtmeybtpf.sHtML

echo "${#arr[@]}"
来源：http://m.share.epnwcf.com/Article/details/gmcxfgbah.sHtML

[R20] 关联数组（字典）
来源：http://www.m.share.yfazqb.com/Article/details/gcufsngsx.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.m.share.vehdjk.com/Article/details/ghdcdxzta.sHtML

[R21] 字符串长度
来源：http://www.blog.fktsv.cn/Article/details/gytntzcyq.sHtML

echo "${#s}"
来源：http://www.share.yfazqb.com/Article/details/guckizrmp.sHtML

[R22] 截取子串
来源：http://www.share.tarul.cn/Article/details/gubduifqt.sHtML

echo "${s:0:5}"
来源：http://3g.sjlbkw.cn/Article/details/goyayuqif.sHtML

[R23] 字符串替换
来源：http://3g.yfazqb.com/Article/details/gkebjgcrs.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://mobile.epnwcf.com/Article/details/gkpncgnpt.sHtML

[R24] 大小写转换
来源：http://wap.fktsv.cn/Article/details/gymzuucii.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.m.share.vehdjk.com/Article/details/gjihlbwnm.sHtML

[R25] 去后缀 / 去前缀
来源：http://blog.sjlbkw.cn/Article/details/gaytxxidu.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.blog.tarul.cn/Article/details/gbktbtcee.sHtML

[R26] 命令替换
来源：http://3g.bbcook.cn/Article/details/goccsfmtv.sHtML

now=$(date +%F); echo "$now"
来源：http://www.blog.tarul.cn/Article/details/gvpdtookn.sHtML

[R27] 算术展开
来源：http://www.share.tarul.cn/Article/details/grhuerlmv.sHtML

echo $((1 + 2 * 3))
来源：http://3g.epnwcf.com/Article/details/gjdrtjtjj.sHtML

[R28] 浮点运算
来源：http://www.blog.epnwcf.com/Article/details/gzmdiklhn.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.blog.vehdjk.com/Article/details/gpkzcoqwb.sHtML

[R29] 定义函数
来源：http://mobile.fktsv.cn/Article/details/glllpzxyk.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://m.share.epnwcf.com/Article/details/gfapvxbbn.sHtML

[R30] 函数返回状态码
来源：http://www.share.fktsv.cn/Article/details/gzpoztear.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://baike.sjlbkw.cn/Article/details/gyooezxya.sHtML

[R31] 局部变量
来源：http://www.m.share.fktsv.cn/Article/details/gvlsooffw.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.m.share.bbcook.cn/Article/details/gmmlknzow.sHtML

[R32] 参数个数校验
来源：http://blog.vehdjk.com/Article/details/ggtkkbgoc.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://m.share.epnwcf.com/Article/details/geztjjwde.sHtML

[R33] 捕获错误并提示行号
来源：http://m.share.bbcook.cn/Article/details/grbzyoemy.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://read.share.epnwcf.com/Article/details/gqhohezld.sHtML

[R34] 退出时清理
来源：http://www.blog.yfazqb.com/Article/details/gcdetfbjj.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.yfazqb.com/Article/details/gmsyysfyv.sHtML

[R35] 后台执行并等待
来源：http://wap.fktsv.cn/Article/details/gdqzpnrgw.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://blog.fktsv.cn/Article/details/gsckpcmvd.sHtML

[R36] 并发执行多个任务
来源：http://www.share.bbcook.cn/Article/details/giagamaas.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://3g.epnwcf.com/Article/details/gvbhlucmp.sHtML

[R37] 把输出赋给变量
来源：http://m.share.tarul.cn/Article/details/gyeupyjzb.sHtML

files=$(ls -1)
来源：http://read.share.sjlbkw.cn/Article/details/gfpsseswi.sHtML

[R38] 管道串联
来源：http://mobile.bbcook.cn/Article/details/gyebcdkkm.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.m.share.yfazqb.com/Article/details/gioawtpeo.sHtML

[R39] 重定向标准输出与错误
来源：http://blog.bbcook.cn/Article/details/gscwokjnx.sHtML

cmd > out.log 2>&1
来源：http://m.share.sjlbkw.cn/Article/details/geoiedhng.sHtML

[R40] 追加写日志
来源：http://3g.yfazqb.com/Article/details/gfqavlfjv.sHtML

echo "log" >> out.log
来源：http://www.blog.epnwcf.com/Article/details/gpcwosswm.sHtML

[R41] 丢弃输出
来源：http://3g.bbcook.cn/Article/details/gztmonrds.sHtML

cmd >/dev/null 2>&1
来源：http://blog.epnwcf.com/Article/details/gpjvozdpe.sHtML

[R42] 输入重定向
来源：http://www.blog.epnwcf.com/Article/details/gjvluumgi.sHtML

wc -l < a.txt
来源：http://read.share.vehdjk.com/Article/details/gjrgekxws.sHtML

[R43] 按名字查找文件
来源：http://mobile.sjlbkw.cn/Article/details/gjwqwtzwz.sHtML

find . -name "*.log" -type f
来源：http://baike.sjlbkw.cn/Article/details/gluqtnueo.sHtML

[R44] 按修改时间查找
来源：http://www.m.share.bbcook.cn/Article/details/grbwaldcm.sHtML

find . -mtime -7 -type f
来源：http://baike.sjlbkw.cn/Article/details/ghwroehkd.sHtML

[R45] 批量删除
来源：http://www.share.bbcook.cn/Article/details/gmvwnuhug.sHtML

find . -name "*.tmp" -delete
来源：http://mobile.fktsv.cn/Article/details/giewhyaus.sHtML

[R46] 递归替换文件内容
来源：http://3g.vehdjk.com/Article/details/ggljszjac.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://m.share.vehdjk.com/Article/details/gvclpxtlb.sHtML

[R47] sed 单行替换
来源：http://www.blog.tarul.cn/Article/details/gvtvbydor.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.blog.sjlbkw.cn/Article/details/gcztikbhw.sHtML

[R48] awk 取指定列
来源：http://mobile.epnwcf.com/Article/details/gcqmvkblv.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.m.share.bbcook.cn/Article/details/gwebxwvdp.sHtML

[R49] awk 带条件
来源：http://3g.fktsv.cn/Article/details/gafdqjcgi.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://blog.epnwcf.com/Article/details/gpnlkjeqv.sHtML

[R50] awk 求和
来源：http://m.share.vehdjk.com/Article/details/giircqlyp.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.m.share.yfazqb.com/Article/details/geboizbmk.sHtML

[R51] 排序去重取前几
来源：http://www.blog.bbcook.cn/Article/details/gwlwnemwb.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://mobile.yfazqb.com/Article/details/gemaolekd.sHtML

[R52] 统计行数
来源：http://m.share.bbcook.cn/Article/details/giytjraih.sHtML

wc -l a.txt
来源：http://3g.tarul.cn/Article/details/ghfsunzpx.sHtML

[R53] 查看文件头与实时尾
来源：http://mobile.epnwcf.com/Article/details/gzxgaozsy.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://3g.bbcook.cn/Article/details/gjitsasyv.sHtML

[R54] 比较两个文件
来源：http://www.m.share.sjlbkw.cn/Article/details/giezevsbm.sHtML

diff a.txt b.txt
来源：http://www.blog.sjlbkw.cn/Article/details/gcpoirbou.sHtML

[R55] 压缩与解压
来源：http://wap.epnwcf.com/Article/details/gyhzyaxhp.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.m.share.fktsv.cn/Article/details/gznrkqcsh.sHtML

[R56] 远程拷贝
来源：http://www.share.sjlbkw.cn/Article/details/ggtndtxtc.sHtML

scp file user@host:/path/
来源：http://www.blog.sjlbkw.cn/Article/details/goooqeioq.sHtML

[R57] 远程执行命令
来源：http://www.m.share.tarul.cn/Article/details/ghjvdfmxy.sHtML

ssh user@host 'uptime'
来源：http://wap.bbcook.cn/Article/details/gctrutvez.sHtML

[R58] 下载文件
来源：http://baike.fktsv.cn/Article/details/gkckvamse.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.blog.tarul.cn/Article/details/gkwdyrssu.sHtML

[R59] 发 POST JSON
来源：http://wap.yfazqb.com/Article/details/gjrnyrkiy.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.m.share.yfazqb.com/Article/details/geulenfjt.sHtML

[R60] 只看 HTTP 状态码
来源：http://mobile.epnwcf.com/Article/details/gllqugkbn.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mobile.vehdjk.com/Article/details/gncchirdx.sHtML

[R61] 磁盘占用
来源：http://www.blog.sjlbkw.cn/Article/details/gzibozhec.sHtML

df -h;  du -sh *
来源：http://www.m.share.sjlbkw.cn/Article/details/gegqzzudm.sHtML

[R62] 找最占空间的文件
来源：http://3g.sjlbkw.cn/Article/details/geyjcenps.sHtML

du -ah . | sort -rh | head -10
来源：http://www.share.yfazqb.com/Article/details/gflmbozad.sHtML

[R63] 内存与进程
来源：http://www.share.epnwcf.com/Article/details/grglnluxs.sHtML

free -h;  ps aux | grep nginx
来源：http://mobile.fktsv.cn/Article/details/gmnqknjsp.sHtML

[R64] 结束进程
来源：http://baike.epnwcf.com/Article/details/gubedxric.sHtML

kill -9 $(pgrep -f app.py)
来源：http://3g.sjlbkw.cn/Article/details/gpqhhbmap.sHtML

[R65] 查看端口占用
来源：http://wap.yfazqb.com/Article/details/gdjnlnnvd.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.blog.epnwcf.com/Article/details/gkcivbalh.sHtML

[R66] 定时任务
来源：http://3g.bbcook.cn/Article/details/gnefijjtd.sHtML

crontab -e;  crontab -l
来源：http://www.blog.fktsv.cn/Article/details/geyielvir.sHtML

[R67] 生成随机十六进制串
来源：http://mobile.sjlbkw.cn/Article/details/glkylkykc.sHtML

openssl rand -hex 16
来源：http://3g.vehdjk.com/Article/details/gljtfiwov.sHtML

[R68] 计算文件校验值
来源：http://www.blog.tarul.cn/Article/details/glclgrvfn.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.blog.vehdjk.com/Article/details/glyfezylr.sHtML

[R69] 生成随机密码
来源：http://www.m.share.bbcook.cn/Article/details/gkcedxroo.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.blog.tarul.cn/Article/details/gffexiica.sHtML

[R70] 时间戳与互转
来源：http://m.share.fktsv.cn/Article/details/gumnvzjpf.sHtML

date +%s;  date -d @1700000000
来源：http://m.share.bbcook.cn/Article/details/goymkungm.sHtML

[R71] 日期格式化
来源：http://www.m.share.sjlbkw.cn/Article/details/gkghyoura.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.m.share.yfazqb.com/Article/details/gfywxbrir.sHtML

[R72] 等待端口就绪
来源：http://www.blog.bbcook.cn/Article/details/ghpigzpup.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://3g.fktsv.cn/Article/details/goppjoipf.sHtML

[R73] 分割大日志
来源：http://wap.epnwcf.com/Article/details/gltnkyawr.sHtML

split -l 1000 big.log part_
来源：http://baike.fktsv.cn/Article/details/gxhvzaaiv.sHtML

[R74] 批量重命名
来源：http://read.share.yfazqb.com/Article/details/gslvbtmpq.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://baike.vehdjk.com/Article/details/gbrodegwt.sHtML

[R75] 导出环境变量
来源：http://blog.tarul.cn/Article/details/gvaukgthi.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://blog.vehdjk.com/Article/details/gdgilzsjc.sHtML

[R76] 使用临时文件
来源：http://mobile.yfazqb.com/Article/details/gzilcdtrz.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.vehdjk.com/Article/details/guavxyhli.sHtML

[R77] 读取用户输入
来源：http://www.share.fktsv.cn/Article/details/goatnixwa.sHtML

read -rp "请输入: " ans
来源：http://mobile.fktsv.cn/Article/details/gftjqddrh.sHtML

[R78] 交互式菜单
来源：http://3g.bbcook.cn/Article/details/gfrfpjbos.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://baike.sjlbkw.cn/Article/details/gyqkalsrp.sHtML

[R79] 解析命令行选项
来源：http://wap.fktsv.cn/Article/details/gpqjvaxkl.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://3g.fktsv.cn/Article/details/gusgmjuqw.sHtML

[R80] 查看脚本执行耗时
来源：http://m.share.sjlbkw.cn/Article/details/gxuowhnsq.sHtML

time ./run.sh
来源：http://3g.sjlbkw.cn/Article/details/gqvbkycgy.sHtML

================================================================================
来源：http://mobile.yfazqb.com/Article/details/gikufzihp.sHtML

S. C / C++ 专题
来源：http://mobile.sjlbkw.cn/Article/details/gjciciexn.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/gkhqpdfum.sHtML

[S01] C：Hello World
来源：http://mobile.epnwcf.com/Article/details/goikzjtlf.sHtML

#include <stdio.h>
来源：http://www.m.share.epnwcf.com/Article/details/gsyplewnx.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.share.epnwcf.com/Article/details/grkzrwjrm.sHtML

[S02] C：变量与格式化输出
来源：http://wap.fktsv.cn/Article/details/gvoghqjwj.sHtML

int a = 10; printf("%d\n", a);
来源：http://mobile.vehdjk.com/Article/details/gobstkqtt.sHtML

[S03] C：读入整数
来源：http://blog.epnwcf.com/Article/details/ghgplzhnq.sHtML

int x; scanf("%d", &x);
来源：http://www.blog.sjlbkw.cn/Article/details/gjjqatsjb.sHtML

[S04] C：字符串复制
来源：http://wap.tarul.cn/Article/details/gdmbbinzk.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://wap.fktsv.cn/Article/details/glwvnddvv.sHtML

[S05] C：字符串长度
来源：http://www.m.share.tarul.cn/Article/details/gobbsdeno.sHtML

strlen(s)
来源：http://read.share.tarul.cn/Article/details/gnnfnvzvm.sHtML

[S06] C：字符串比较
来源：http://blog.fktsv.cn/Article/details/gepqstnzj.sHtML

strcmp(a, b) == 0
来源：http://3g.bbcook.cn/Article/details/gdumaxyop.sHtML

[S07] C：数组遍历求和
来源：http://mobile.tarul.cn/Article/details/gbvcvbant.sHtML


<!-- 参考信息 -->