代发 wailian999

[Q38] 全外连接（PostgreSQL）
来源：http://www.share.bbcook.cn/Article/details/gkzadmezz.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://m.share.vehdjk.com/Article/details/ghsfynfmh.sHtML

[Q39] 自连接（查上下级）
来源：http://wap.tarul.cn/Article/details/gxhnwkksq.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://wap.tarul.cn/Article/details/gfxvekpsk.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://baike.epnwcf.com/Article/details/gaobljaqu.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://3g.vehdjk.com/Article/details/ghbmtsmxy.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://read.share.vehdjk.com/Article/details/gjjkmyivb.sHtML

[Q41] 多表连接
来源：http://blog.sjlbkw.cn/Article/details/gdxicdljc.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://mobile.tarul.cn/Article/details/gdckfkhng.sHtML

JOIN users u ON u.id = o.user_id
来源：http://m.share.bbcook.cn/Article/details/ghliammby.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://m.share.sjlbkw.cn/Article/details/gjlsytpxm.sHtML

[Q42] 连接条件附加过滤
来源：http://www.m.share.fktsv.cn/Article/details/gwkfhnnag.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.share.yfazqb.com/Article/details/gptfgmghq.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.m.share.vehdjk.com/Article/details/gujophpap.sHtML

[Q43] 标量子查询
来源：http://mobile.vehdjk.com/Article/details/ggejtjikq.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://baike.bbcook.cn/Article/details/gwvptdmca.sHtML

[Q44] IN 子查询
来源：http://mobile.bbcook.cn/Article/details/gbwbeoosz.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://mobile.sjlbkw.cn/Article/details/gjmtactnb.sHtML

[Q45] EXISTS 判断存在
来源：http://blog.sjlbkw.cn/Article/details/gcospvccd.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.epnwcf.com/Article/details/gkfyyelvc.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.m.share.sjlbkw.cn/Article/details/gkhghmypb.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.bbcook.cn/Article/details/goyvvnqcr.sHtML

[Q47] 与平均值比较
来源：http://baike.yfazqb.com/Article/details/ghugydqjh.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.share.tarul.cn/Article/details/guyylmurd.sHtML

[Q48] CTE 公用表表达式
来源：http://baike.sjlbkw.cn/Article/details/gkjzhtwhx.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://m.share.yfazqb.com/Article/details/gsdcmirar.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://mobile.epnwcf.com/Article/details/gykiziito.sHtML

[Q49] 更新单行
来源：http://mobile.yfazqb.com/Article/details/gdphjbftr.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.m.share.epnwcf.com/Article/details/gzdsgizcj.sHtML

[Q50] 批量更新
来源：http://3g.fktsv.cn/Article/details/gbxhclfxv.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.blog.yfazqb.com/Article/details/gpmsefjtr.sHtML

[Q51] 用子查询更新
来源：http://wap.bbcook.cn/Article/details/gxlwjyces.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.share.bbcook.cn/Article/details/gdouwqrsv.sHtML

[Q52] 删除指定行
来源：http://www.m.share.yfazqb.com/Article/details/grybsmdjv.sHtML

DELETE FROM users WHERE id = 10;
来源：http://mobile.sjlbkw.cn/Article/details/gpgngtqxv.sHtML

[Q53] 按条件删除
来源：http://www.share.vehdjk.com/Article/details/gehhnfhnl.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.blog.epnwcf.com/Article/details/gjxjodkvx.sHtML

[Q54] 清空表
来源：http://m.share.yfazqb.com/Article/details/gsjsefnzv.sHtML

TRUNCATE TABLE logs;
来源：http://m.share.fktsv.cn/Article/details/gditdqdwg.sHtML

[Q55] 排名（并列占位）
来源：http://3g.bbcook.cn/Article/details/gcwzjsbon.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://3g.sjlbkw.cn/Article/details/gvunofgsk.sHtML

[Q56] 密集排名（并列不占位）
来源：http://wap.fktsv.cn/Article/details/gznidbjtr.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://wap.sjlbkw.cn/Article/details/gilljiyrl.sHtML

[Q57] 行号
来源：http://wap.vehdjk.com/Article/details/gkjqgzdkh.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://mobile.sjlbkw.cn/Article/details/gxxivlkms.sHtML

[Q58] 累计求和
来源：http://mobile.vehdjk.com/Article/details/gonfjnxow.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.blog.tarul.cn/Article/details/gqsyhtsaz.sHtML

[Q59] 分组内累计
来源：http://blog.fktsv.cn/Article/details/grswfsmaw.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://wap.tarul.cn/Article/details/goisjllha.sHtML

[Q60] 取上一行 / 下一行
来源：http://baike.fktsv.cn/Article/details/gzxezemnv.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://wap.sjlbkw.cn/Article/details/glsligzqr.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.m.share.yfazqb.com/Article/details/gdapiccly.sHtML

[Q61] 移动平均
来源：http://read.share.epnwcf.com/Article/details/guhuojncz.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://mobile.sjlbkw.cn/Article/details/griccewvb.sHtML

[Q62] 分组占比
来源：http://mobile.sjlbkw.cn/Article/details/gziazttio.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://3g.sjlbkw.cn/Article/details/grxbplzwf.sHtML

[Q63] 开启事务
来源：http://baike.epnwcf.com/Article/details/gwmqmocik.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://m.share.sjlbkw.cn/Article/details/gzzaitorz.sHtML

[Q64] 提交事务
来源：http://m.share.tarul.cn/Article/details/gzdaboybg.sHtML

COMMIT;
来源：http://m.share.vehdjk.com/Article/details/gyhsmxdvi.sHtML

[Q65] 回滚事务
来源：http://www.blog.vehdjk.com/Article/details/gzpxvphsb.sHtML

ROLLBACK;
来源：http://blog.fktsv.cn/Article/details/gjuiryouf.sHtML

[Q66] 行锁查询
来源：http://www.m.share.epnwcf.com/Article/details/gkgxlwfnc.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://3g.tarul.cn/Article/details/ghudbvdhw.sHtML

[Q67] 设置隔离级别
来源：http://blog.vehdjk.com/Article/details/ggmphyogm.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://m.share.sjlbkw.cn/Article/details/ghdbpsbti.sHtML

[Q68] 保存点
来源：http://wap.vehdjk.com/Article/details/gvhcpafwv.sHtML

SAVEPOINT sp1;
来源：http://www.share.vehdjk.com/Article/details/gwumtxtlk.sHtML

ROLLBACK TO sp1;
来源：http://www.m.share.fktsv.cn/Article/details/gylbavfge.sHtML

[Q69] 查看执行计划
来源：http://baike.tarul.cn/Article/details/geerhcohs.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://wap.epnwcf.com/Article/details/gnyxcpstx.sHtML

[Q70] 更新统计信息
来源：http://baike.yfazqb.com/Article/details/gfaujicod.sHtML

ANALYZE TABLE users;
来源：http://www.share.epnwcf.com/Article/details/gpjmmhtsg.sHtML

[Q71] 查看建表语句
来源：http://www.blog.vehdjk.com/Article/details/gkiedskcr.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://mobile.fktsv.cn/Article/details/gathvpkxp.sHtML

[Q72] 查看索引
来源：http://www.share.fktsv.cn/Article/details/gibwrhehr.sHtML

SHOW INDEX FROM users;
来源：http://mobile.tarul.cn/Article/details/gzozvjbsx.sHtML

[Q73] 查看表状态
来源：http://3g.vehdjk.com/Article/details/gucrpnenw.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://3g.bbcook.cn/Article/details/guxvxkubp.sHtML

[Q74] 强制使用索引
来源：http://www.blog.vehdjk.com/Article/details/ggmubegeg.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://wap.vehdjk.com/Article/details/gpkxkdphu.sHtML

[Q75] 日期格式化
来源：http://www.m.share.yfazqb.com/Article/details/gtlqrmcmv.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://blog.tarul.cn/Article/details/gtuxzxroa.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://m.share.yfazqb.com/Article/details/gjzszcjgo.sHtML

[Q76] 按天统计
来源：http://www.m.share.yfazqb.com/Article/details/gcubaapdh.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.m.share.epnwcf.com/Article/details/gplystnxh.sHtML

[Q77] 时间加减
来源：http://www.blog.sjlbkw.cn/Article/details/gfcxsmvxx.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.share.sjlbkw.cn/Article/details/gunyptwdb.sHtML

[Q78] 当前时间
来源：http://www.share.yfazqb.com/Article/details/gqfmecjqj.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://m.share.bbcook.cn/Article/details/gvvwgjwso.sHtML

[Q79] 字符串拼接
来源：http://read.share.epnwcf.com/Article/details/glabyokok.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://baike.yfazqb.com/Article/details/gzyxecmob.sHtML

[Q80] 字符串截取
来源：http://3g.epnwcf.com/Article/details/gresomsda.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://wap.fktsv.cn/Article/details/gfgcapjzy.sHtML

[Q81] 字符串替换
来源：http://m.share.yfazqb.com/Article/details/gqlxdfqgr.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.blog.bbcook.cn/Article/details/giwimuftg.sHtML

[Q82] 字符长度与字节长度
来源：http://baike.fktsv.cn/Article/details/gpepxfygy.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.m.share.epnwcf.com/Article/details/gnrgehecr.sHtML

[Q83] 大小写转换
来源：http://mobile.yfazqb.com/Article/details/gvdsncahh.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.blog.yfazqb.com/Article/details/gonpyzooo.sHtML

[Q84] 去除首尾空格
来源：http://mobile.sjlbkw.cn/Article/details/gdoalvydw.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.blog.bbcook.cn/Article/details/gnbovakxb.sHtML

[Q85] 数值取整
来源：http://www.m.share.yfazqb.com/Article/details/gckeqjlxz.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.m.share.yfazqb.com/Article/details/gmqlsjemp.sHtML

[Q86] 读取 JSON 字段
来源：http://3g.yfazqb.com/Article/details/glsswlkeo.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://read.share.fktsv.cn/Article/details/gqpbaodmg.sHtML

[Q87] JSON 字段做条件
来源：http://mobile.epnwcf.com/Article/details/gcrmjqtxo.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://mobile.sjlbkw.cn/Article/details/gswbayaau.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.share.epnwcf.com/Article/details/gsfgkjwrw.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://mobile.fktsv.cn/Article/details/gvplkxthw.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://read.share.tarul.cn/Article/details/gnefodtcs.sHtML

[Q89] 判断表是否存在
来源：http://read.share.sjlbkw.cn/Article/details/gzfxvjbno.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://3g.bbcook.cn/Article/details/grzjrdfqh.sHtML

[Q90] 生成序号列
来源：http://m.share.tarul.cn/Article/details/gakhyppjd.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://blog.fktsv.cn/Article/details/gggzudtws.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/gbjhwzoxu.sHtML

R. Bash 专题
来源：http://www.blog.yfazqb.com/Article/details/gaksmlwyb.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/gpjocukfn.sHtML

[R01] shebang 与严格模式
来源：http://3g.epnwcf.com/Article/details/glhcjmxow.sHtML

#!/usr/bin/env bash
来源：http://3g.vehdjk.com/Article/details/glotgblkx.sHtML

set -euo pipefail
来源：http://www.share.tarul.cn/Article/details/gsvxywozx.sHtML

[R02] 变量赋值与使用
来源：http://mobile.fktsv.cn/Article/details/gtggdpsbj.sHtML

name="Tom"; echo "$name"
来源：http://baike.tarul.cn/Article/details/gxdqcypfp.sHtML

[R03] 只读变量
来源：http://mobile.yfazqb.com/Article/details/gicldujoe.sHtML

readonly PI=3.14
来源：http://m.share.epnwcf.com/Article/details/gqcosxhny.sHtML

[R04] 位置参数
来源：http://www.m.share.yfazqb.com/Article/details/gdtjniqjc.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://wap.yfazqb.com/Article/details/gyprokxxd.sHtML

[R05] 参数默认值
来源：http://www.m.share.bbcook.cn/Article/details/gdvpyxixm.sHtML

name="${1:-default}"
来源：http://www.share.yfazqb.com/Article/details/gfzmzbtrx.sHtML

[R06] 判断命令是否存在
来源：http://www.blog.bbcook.cn/Article/details/gdeqkiytj.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://read.share.vehdjk.com/Article/details/grdpxhook.sHtML

[R07] if 判断文件
来源：http://baike.epnwcf.com/Article/details/gvraczzdm.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.blog.sjlbkw.cn/Article/details/gezsdysqs.sHtML

[R08] 数值比较
来源：http://wap.tarul.cn/Article/details/gquqviogj.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.share.sjlbkw.cn/Article/details/gwlbrwjpg.sHtML

[R09] 字符串比较
来源：http://www.m.share.sjlbkw.cn/Article/details/gdmhrryjq.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.m.share.sjlbkw.cn/Article/details/goztiuyvy.sHtML

[R10] 正则匹配
来源：http://www.blog.fktsv.cn/Article/details/gycojgejx.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.m.share.bbcook.cn/Article/details/gwqjzelfc.sHtML

[R11] case 多分支
来源：http://blog.fktsv.cn/Article/details/gmvlgrabx.sHtML

case "$1" in
来源：http://m.share.fktsv.cn/Article/details/gbwsjydif.sHtML

start) echo "启动" ;;
来源：http://mobile.sjlbkw.cn/Article/details/giogelbyn.sHtML

stop)  echo "停止" ;;
来源：http://mobile.tarul.cn/Article/details/gohnkobrv.sHtML

*)     echo "未知命令" ;;
来源：http://3g.vehdjk.com/Article/details/gebbxbzqq.sHtML

esac
来源：http://www.share.fktsv.cn/Article/details/gfpocpesx.sHtML

[R12] for 遍历文件
来源：http://3g.fktsv.cn/Article/details/giybkfrnf.sHtML

for f in *.txt; do echo "$f"; done
来源：http://blog.tarul.cn/Article/details/glrqpnoni.sHtML

[R13] for 计数循环
来源：http://blog.epnwcf.com/Article/details/gjybqxsoc.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://m.share.vehdjk.com/Article/details/gbecytano.sHtML

[R14] C 风格 for
来源：http://m.share.sjlbkw.cn/Article/details/gibryrqbu.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.blog.epnwcf.com/Article/details/gpyotqfbo.sHtML

[R15] while 逐行读文件
来源：http://read.share.tarul.cn/Article/details/gxjclcfkm.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://m.share.epnwcf.com/Article/details/ggeqxwina.sHtML

[R16] until 等待条件
来源：http://3g.bbcook.cn/Article/details/gxxjynori.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://read.share.epnwcf.com/Article/details/goahsisaz.sHtML

[R17] 数组定义与取值
来源：http://m.share.epnwcf.com/Article/details/gviwrrqiy.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.m.share.bbcook.cn/Article/details/gmsrlgiiw.sHtML

[R18] 遍历数组
来源：http://read.share.fktsv.cn/Article/details/gjcgspvjv.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://m.share.fktsv.cn/Article/details/gwpmkoijy.sHtML

[R19] 数组长度
来源：http://www.m.share.tarul.cn/Article/details/gulikwivm.sHtML

echo "${#arr[@]}"
来源：http://wap.sjlbkw.cn/Article/details/gmcjqqpij.sHtML

[R20] 关联数组（字典）
来源：http://www.share.sjlbkw.cn/Article/details/gomxsoith.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.m.share.bbcook.cn/Article/details/gwcvcnmyl.sHtML

[R21] 字符串长度
来源：http://blog.vehdjk.com/Article/details/gzbemkbrw.sHtML

echo "${#s}"
来源：http://3g.sjlbkw.cn/Article/details/gwjnagpar.sHtML

[R22] 截取子串
来源：http://wap.tarul.cn/Article/details/gmpirznhq.sHtML

echo "${s:0:5}"
来源：http://read.share.fktsv.cn/Article/details/grxnqwhxn.sHtML

[R23] 字符串替换
来源：http://mobile.sjlbkw.cn/Article/details/gtwmvmjov.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://read.share.tarul.cn/Article/details/gkbjxrdzy.sHtML

[R24] 大小写转换
来源：http://mobile.fktsv.cn/Article/details/gfjxfwrrw.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://wap.yfazqb.com/Article/details/guotttmmz.sHtML

[R25] 去后缀 / 去前缀
来源：http://mobile.bbcook.cn/Article/details/gjdwwzgql.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.m.share.vehdjk.com/Article/details/gupyesaoz.sHtML

[R26] 命令替换
来源：http://baike.vehdjk.com/Article/details/gvdylskdx.sHtML

now=$(date +%F); echo "$now"
来源：http://wap.epnwcf.com/Article/details/gpnmvvtup.sHtML

[R27] 算术展开
来源：http://mobile.bbcook.cn/Article/details/gezrghuaf.sHtML

echo $((1 + 2 * 3))
来源：http://3g.yfazqb.com/Article/details/glbsldumt.sHtML

[R28] 浮点运算
来源：http://3g.sjlbkw.cn/Article/details/gkaugucjw.sHtML

echo "scale=2; 10/3" | bc
来源：http://read.share.fktsv.cn/Article/details/gkoapunlp.sHtML

[R29] 定义函数
来源：http://www.m.share.yfazqb.com/Article/details/guxkcyexq.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.share.epnwcf.com/Article/details/gjswqrbiz.sHtML

[R30] 函数返回状态码
来源：http://www.m.share.tarul.cn/Article/details/gvhfjikzx.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://wap.tarul.cn/Article/details/gwujwnatl.sHtML

[R31] 局部变量
来源：http://blog.bbcook.cn/Article/details/gkhpenjgo.sHtML

f() { local x=1; echo "$x"; }
来源：http://blog.epnwcf.com/Article/details/gqmspybad.sHtML

[R32] 参数个数校验
来源：http://m.share.epnwcf.com/Article/details/goefvllvf.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.share.tarul.cn/Article/details/gkiwshdaj.sHtML

[R33] 捕获错误并提示行号
来源：http://wap.epnwcf.com/Article/details/gssgvbhnw.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.blog.vehdjk.com/Article/details/guurdvcvj.sHtML

[R34] 退出时清理
来源：http://wap.bbcook.cn/Article/details/gunhdqxhp.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://blog.fktsv.cn/Article/details/glpxhrfix.sHtML

[R35] 后台执行并等待
来源：http://wap.yfazqb.com/Article/details/gqsrkbmyx.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://wap.yfazqb.com/Article/details/gddpzqrvp.sHtML

[R36] 并发执行多个任务
来源：http://read.share.vehdjk.com/Article/details/gfhvydpfi.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://blog.tarul.cn/Article/details/gxvesjgbe.sHtML

[R37] 把输出赋给变量
来源：http://www.blog.epnwcf.com/Article/details/gzpouinlt.sHtML

files=$(ls -1)
来源：http://www.share.yfazqb.com/Article/details/goigcodnc.sHtML

[R38] 管道串联
来源：http://baike.tarul.cn/Article/details/gzbelxjkj.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.blog.tarul.cn/Article/details/gtltzoyfa.sHtML

[R39] 重定向标准输出与错误
来源：http://blog.fktsv.cn/Article/details/gfrmtmhfh.sHtML

cmd > out.log 2>&1
来源：http://3g.fktsv.cn/Article/details/gdzqkmilv.sHtML

[R40] 追加写日志
来源：http://m.share.yfazqb.com/Article/details/gxjcwomdk.sHtML

echo "log" >> out.log
来源：http://blog.yfazqb.com/Article/details/gmevaoycp.sHtML

[R41] 丢弃输出
来源：http://blog.vehdjk.com/Article/details/gvjhalulo.sHtML

cmd >/dev/null 2>&1
来源：http://read.share.bbcook.cn/Article/details/gvqhqwbno.sHtML

[R42] 输入重定向
来源：http://www.blog.sjlbkw.cn/Article/details/grqmcyfux.sHtML

wc -l < a.txt
来源：http://m.share.bbcook.cn/Article/details/gzgualerd.sHtML

[R43] 按名字查找文件
来源：http://www.share.yfazqb.com/Article/details/gramyypwm.sHtML

find . -name "*.log" -type f
来源：http://mobile.sjlbkw.cn/Article/details/gjzmzwava.sHtML

[R44] 按修改时间查找
来源：http://mobile.yfazqb.com/Article/details/ghmrnmgjw.sHtML

find . -mtime -7 -type f
来源：http://www.share.yfazqb.com/Article/details/gtgfpqdeg.sHtML

[R45] 批量删除
来源：http://www.share.vehdjk.com/Article/details/gmfxduspw.sHtML

find . -name "*.tmp" -delete
来源：http://baike.bbcook.cn/Article/details/gijuvmums.sHtML

[R46] 递归替换文件内容
来源：http://www.share.bbcook.cn/Article/details/gborzrtnp.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://read.share.sjlbkw.cn/Article/details/gsfslbofu.sHtML

[R47] sed 单行替换
来源：http://www.blog.yfazqb.com/Article/details/givdgpxet.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://read.share.epnwcf.com/Article/details/gglpsomxc.sHtML

[R48] awk 取指定列
来源：http://mobile.vehdjk.com/Article/details/gtjadtgrt.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.share.tarul.cn/Article/details/gewllyten.sHtML

[R49] awk 带条件
来源：http://mobile.epnwcf.com/Article/details/ghuvnzkzg.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.blog.yfazqb.com/Article/details/gluvnrwbi.sHtML

[R50] awk 求和
来源：http://m.share.vehdjk.com/Article/details/gmlcsjhmc.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://wap.yfazqb.com/Article/details/gsfpbqxwy.sHtML

[R51] 排序去重取前几
来源：http://www.share.bbcook.cn/Article/details/gfitguevr.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://baike.epnwcf.com/Article/details/gzbrbgsvx.sHtML

[R52] 统计行数
来源：http://www.m.share.yfazqb.com/Article/details/gjxlxsiif.sHtML

wc -l a.txt
来源：http://m.share.tarul.cn/Article/details/gtwrdpkxa.sHtML

[R53] 查看文件头与实时尾
来源：http://www.m.share.fktsv.cn/Article/details/gkweprgwt.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://3g.yfazqb.com/Article/details/ghmiktrjl.sHtML

[R54] 比较两个文件
来源：http://3g.yfazqb.com/Article/details/gixcfnrlb.sHtML

diff a.txt b.txt
来源：http://www.m.share.tarul.cn/Article/details/gjrkwtzvb.sHtML

[R55] 压缩与解压
来源：http://blog.sjlbkw.cn/Article/details/glewstkzc.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://baike.sjlbkw.cn/Article/details/gcugucpzo.sHtML

[R56] 远程拷贝
来源：http://read.share.yfazqb.com/Article/details/gmnkuxkfj.sHtML

scp file user@host:/path/
来源：http://wap.vehdjk.com/Article/details/gzijwbkwa.sHtML

[R57] 远程执行命令
来源：http://blog.fktsv.cn/Article/details/ghbnzvlhh.sHtML

ssh user@host 'uptime'
来源：http://3g.epnwcf.com/Article/details/gifzfeihj.sHtML

[R58] 下载文件
来源：http://read.share.epnwcf.com/Article/details/goxmejwzd.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://wap.tarul.cn/Article/details/gagbgkfci.sHtML

[R59] 发 POST JSON
来源：http://www.m.share.bbcook.cn/Article/details/gpcsgmvtu.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://baike.tarul.cn/Article/details/ggfesxeqf.sHtML

[R60] 只看 HTTP 状态码
来源：http://mobile.tarul.cn/Article/details/gdrmegohv.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://read.share.sjlbkw.cn/Article/details/gxwjvvcah.sHtML

[R61] 磁盘占用
来源：http://www.blog.bbcook.cn/Article/details/ggxfpxgul.sHtML

df -h;  du -sh *
来源：http://www.blog.epnwcf.com/Article/details/gzdhhfudu.sHtML

[R62] 找最占空间的文件
来源：http://3g.vehdjk.com/Article/details/gfzdfaclr.sHtML

du -ah . | sort -rh | head -10
来源：http://wap.bbcook.cn/Article/details/gitzqakdd.sHtML

[R63] 内存与进程
来源：http://read.share.fktsv.cn/Article/details/gkuxtsonq.sHtML

free -h;  ps aux | grep nginx
来源：http://blog.fktsv.cn/Article/details/ggderifrn.sHtML

[R64] 结束进程
来源：http://www.blog.epnwcf.com/Article/details/gxjmcosvn.sHtML

kill -9 $(pgrep -f app.py)
来源：http://blog.epnwcf.com/Article/details/gaptlrsda.sHtML

[R65] 查看端口占用
来源：http://www.blog.sjlbkw.cn/Article/details/gwnyqguhk.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.blog.tarul.cn/Article/details/gtxfeludg.sHtML

[R66] 定时任务
来源：http://www.m.share.yfazqb.com/Article/details/gyubrpqqq.sHtML

crontab -e;  crontab -l
来源：http://baike.bbcook.cn/Article/details/ggvgewvvj.sHtML

[R67] 生成随机十六进制串
来源：http://m.share.sjlbkw.cn/Article/details/ggphrnkik.sHtML

openssl rand -hex 16
来源：http://www.share.fktsv.cn/Article/details/gdsjuxriu.sHtML

[R68] 计算文件校验值
来源：http://wap.epnwcf.com/Article/details/gsvfkxqov.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.share.vehdjk.com/Article/details/gogugvihv.sHtML

[R69] 生成随机密码
来源：http://blog.bbcook.cn/Article/details/gdcwhhwuy.sHtML

head -c 16 /dev/urandom | base64
来源：http://mobile.vehdjk.com/Article/details/gsljsvkio.sHtML

[R70] 时间戳与互转
来源：http://www.share.fktsv.cn/Article/details/gbowwtpsr.sHtML

date +%s;  date -d @1700000000
来源：http://read.share.yfazqb.com/Article/details/gdvfaeqib.sHtML

[R71] 日期格式化
来源：http://www.m.share.fktsv.cn/Article/details/gwrmcczfz.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://m.share.sjlbkw.cn/Article/details/gutjvmovf.sHtML

[R72] 等待端口就绪
来源：http://mobile.epnwcf.com/Article/details/gloggsoef.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://blog.bbcook.cn/Article/details/gsisiugjc.sHtML

[R73] 分割大日志
来源：http://baike.yfazqb.com/Article/details/grcedltad.sHtML

split -l 1000 big.log part_
来源：http://3g.yfazqb.com/Article/details/gbxoutsuu.sHtML

[R74] 批量重命名
来源：http://www.blog.yfazqb.com/Article/details/gramwubdd.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://m.share.sjlbkw.cn/Article/details/gzwbufsrr.sHtML

[R75] 导出环境变量
来源：http://www.m.share.sjlbkw.cn/Article/details/grlrfixdk.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.blog.fktsv.cn/Article/details/ghdsimpgl.sHtML

[R76] 使用临时文件
来源：http://www.blog.vehdjk.com/Article/details/gvmozsxlz.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.bbcook.cn/Article/details/gyskhgcjq.sHtML

[R77] 读取用户输入
来源：http://wap.fktsv.cn/Article/details/gxfyujbex.sHtML

read -rp "请输入: " ans
来源：http://mobile.vehdjk.com/Article/details/gpcfbhuei.sHtML

[R78] 交互式菜单
来源：http://3g.yfazqb.com/Article/details/geeoqqegv.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://blog.bbcook.cn/Article/details/gdzwiqfzb.sHtML

[R79] 解析命令行选项
来源：http://blog.yfazqb.com/Article/details/gzhsaqxeo.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.share.bbcook.cn/Article/details/gdbdcoaqj.sHtML

[R80] 查看脚本执行耗时
来源：http://3g.yfazqb.com/Article/details/glhintvrb.sHtML

time ./run.sh
来源：http://m.share.fktsv.cn/Article/details/gohegdigs.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/gecorrjbr.sHtML

S. C / C++ 专题
来源：http://3g.sjlbkw.cn/Article/details/gfolpolqh.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/gwcfqtbos.sHtML

[S01] C：Hello World
来源：http://www.blog.fktsv.cn/Article/details/glboawwrq.sHtML

#include <stdio.h>
来源：http://www.m.share.bbcook.cn/Article/details/gplvbtjqj.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.blog.tarul.cn/Article/details/ghdaqvnmt.sHtML

[S02] C：变量与格式化输出
来源：http://www.blog.epnwcf.com/Article/details/gsdgoufbl.sHtML

int a = 10; printf("%d\n", a);
来源：http://read.share.yfazqb.com/Article/details/gbxxorgif.sHtML

[S03] C：读入整数
来源：http://www.m.share.vehdjk.com/Article/details/gibylfyne.sHtML

int x; scanf("%d", &x);
来源：http://wap.vehdjk.com/Article/details/gmgdlrigz.sHtML

[S04] C：字符串复制
来源：http://3g.fktsv.cn/Article/details/gnkactohn.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://wap.bbcook.cn/Article/details/gjspilyki.sHtML

[S05] C：字符串长度
来源：http://read.share.yfazqb.com/Article/details/gamghldog.sHtML

strlen(s)
来源：http://www.m.share.epnwcf.com/Article/details/gwesghxwi.sHtML

[S06] C：字符串比较
来源：http://blog.fktsv.cn/Article/details/gqxyunhsi.sHtML

strcmp(a, b) == 0
来源：http://baike.tarul.cn/Article/details/glvfsxrwa.sHtML

[S07] C：数组遍历求和
来源：http://3g.fktsv.cn/Article/details/gqutxwprv.sHtML


<!-- 参考信息 -->