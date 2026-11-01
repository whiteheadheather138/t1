代发 wailian999

[Q38] 全外连接（PostgreSQL）
来源：http://read.share.bbcook.cn/Article/details/gyhnskqlg.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.share.vehdjk.com/Article/details/gohjkzvsq.sHtML

[Q39] 自连接（查上下级）
来源：http://www.m.share.bbcook.cn/Article/details/gpjcmpkji.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://m.share.sjlbkw.cn/Article/details/gdgcfzqfb.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://3g.epnwcf.com/Article/details/gfwdifasy.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://m.share.vehdjk.com/Article/details/goisehpvr.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.m.share.fktsv.cn/Article/details/gfdkplkvs.sHtML

[Q41] 多表连接
来源：http://www.m.share.fktsv.cn/Article/details/ggeyqmccy.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://blog.bbcook.cn/Article/details/gbubeiffa.sHtML

JOIN users u ON u.id = o.user_id
来源：http://m.share.epnwcf.com/Article/details/gfychzfws.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.share.vehdjk.com/Article/details/gqjfmkhny.sHtML

[Q42] 连接条件附加过滤
来源：http://www.m.share.sjlbkw.cn/Article/details/gocdareye.sHtML

SELECT u.name, o.amount FROM users u
来源：http://baike.vehdjk.com/Article/details/gvuwobayu.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://mobile.epnwcf.com/Article/details/gscxvfnbs.sHtML

[Q43] 标量子查询
来源：http://mobile.yfazqb.com/Article/details/gyjpllzau.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://blog.tarul.cn/Article/details/ggygorfsf.sHtML

[Q44] IN 子查询
来源：http://m.share.epnwcf.com/Article/details/gsojfdtcw.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://read.share.sjlbkw.cn/Article/details/gspojccdt.sHtML

[Q45] EXISTS 判断存在
来源：http://m.share.epnwcf.com/Article/details/gkiqfppzv.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.yfazqb.com/Article/details/gbynfykec.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://3g.yfazqb.com/Article/details/gxcerawvx.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.yfazqb.com/Article/details/gvtnrhqrz.sHtML

[Q47] 与平均值比较
来源：http://wap.yfazqb.com/Article/details/gprjwnygc.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://m.share.yfazqb.com/Article/details/gcrnkwozj.sHtML

[Q48] CTE 公用表表达式
来源：http://blog.tarul.cn/Article/details/gscnmosby.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://read.share.yfazqb.com/Article/details/gtexlqktw.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://wap.bbcook.cn/Article/details/gvscefcwe.sHtML

[Q49] 更新单行
来源：http://m.share.epnwcf.com/Article/details/giebsifjn.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://m.share.fktsv.cn/Article/details/gqtytsmcq.sHtML

[Q50] 批量更新
来源：http://www.share.epnwcf.com/Article/details/gacmiirvj.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://blog.tarul.cn/Article/details/grnkynwik.sHtML

[Q51] 用子查询更新
来源：http://mobile.bbcook.cn/Article/details/gxqnvrayy.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://m.share.bbcook.cn/Article/details/grscbtbfv.sHtML

[Q52] 删除指定行
来源：http://read.share.bbcook.cn/Article/details/ghfdoldhu.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.share.tarul.cn/Article/details/gnipuphlz.sHtML

[Q53] 按条件删除
来源：http://mobile.tarul.cn/Article/details/gvmsryzgo.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.m.share.yfazqb.com/Article/details/gsvphsmbe.sHtML

[Q54] 清空表
来源：http://mobile.epnwcf.com/Article/details/gthowvxmw.sHtML

TRUNCATE TABLE logs;
来源：http://3g.tarul.cn/Article/details/grgoxgjwr.sHtML

[Q55] 排名（并列占位）
来源：http://blog.vehdjk.com/Article/details/gqnhlgyqo.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://read.share.epnwcf.com/Article/details/gacxcqfjk.sHtML

[Q56] 密集排名（并列不占位）
来源：http://3g.sjlbkw.cn/Article/details/glrxieidn.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://m.share.tarul.cn/Article/details/grtifahgu.sHtML

[Q57] 行号
来源：http://www.blog.tarul.cn/Article/details/grfcydxbv.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.blog.vehdjk.com/Article/details/gpcnaolxq.sHtML

[Q58] 累计求和
来源：http://www.share.tarul.cn/Article/details/gozleiqgh.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://mobile.yfazqb.com/Article/details/gqpcokcdl.sHtML

[Q59] 分组内累计
来源：http://baike.tarul.cn/Article/details/gbkxzvpeo.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://3g.epnwcf.com/Article/details/gsafirftm.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.blog.fktsv.cn/Article/details/gsndffasn.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://read.share.vehdjk.com/Article/details/gdzpobuqo.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://blog.bbcook.cn/Article/details/gofgrgoof.sHtML

[Q61] 移动平均
来源：http://blog.vehdjk.com/Article/details/gnkortlii.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://m.share.tarul.cn/Article/details/gauxivobt.sHtML

[Q62] 分组占比
来源：http://3g.tarul.cn/Article/details/gnnwshcpl.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://blog.yfazqb.com/Article/details/ghedsyefn.sHtML

[Q63] 开启事务
来源：http://www.blog.sjlbkw.cn/Article/details/gkhxgtcxc.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://baike.yfazqb.com/Article/details/geiloshfk.sHtML

[Q64] 提交事务
来源：http://www.share.sjlbkw.cn/Article/details/geubgyzid.sHtML

COMMIT;
来源：http://m.share.epnwcf.com/Article/details/ghzgahlnn.sHtML

[Q65] 回滚事务
来源：http://www.m.share.vehdjk.com/Article/details/gszbnqyyz.sHtML

ROLLBACK;
来源：http://www.m.share.epnwcf.com/Article/details/gxwwzvpqv.sHtML

[Q66] 行锁查询
来源：http://3g.bbcook.cn/Article/details/gueklbgwv.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://m.share.epnwcf.com/Article/details/gkbmjjkoe.sHtML

[Q67] 设置隔离级别
来源：http://read.share.yfazqb.com/Article/details/gvdxmpmtk.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://mobile.vehdjk.com/Article/details/guketgwes.sHtML

[Q68] 保存点
来源：http://www.share.fktsv.cn/Article/details/gnbxntjjk.sHtML

SAVEPOINT sp1;
来源：http://blog.tarul.cn/Article/details/gbksxcjgj.sHtML

ROLLBACK TO sp1;
来源：http://wap.epnwcf.com/Article/details/gahuidvmk.sHtML

[Q69] 查看执行计划
来源：http://www.blog.fktsv.cn/Article/details/gkozkvjuv.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://mobile.tarul.cn/Article/details/geuqbtbmg.sHtML

[Q70] 更新统计信息
来源：http://read.share.bbcook.cn/Article/details/glabgslwp.sHtML

ANALYZE TABLE users;
来源：http://wap.fktsv.cn/Article/details/grdonmoin.sHtML

[Q71] 查看建表语句
来源：http://m.share.fktsv.cn/Article/details/gwtjrswfu.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.m.share.yfazqb.com/Article/details/gtrsdumkk.sHtML

[Q72] 查看索引
来源：http://www.blog.bbcook.cn/Article/details/gbvesqxic.sHtML

SHOW INDEX FROM users;
来源：http://www.blog.bbcook.cn/Article/details/glgyrdqua.sHtML

[Q73] 查看表状态
来源：http://www.m.share.vehdjk.com/Article/details/ghuehlyxb.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://3g.tarul.cn/Article/details/gcdmeytrr.sHtML

[Q74] 强制使用索引
来源：http://wap.yfazqb.com/Article/details/gluskshof.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://baike.sjlbkw.cn/Article/details/gcnwmtsim.sHtML

[Q75] 日期格式化
来源：http://blog.tarul.cn/Article/details/gptqfbqym.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://3g.vehdjk.com/Article/details/gogyauxvk.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://3g.fktsv.cn/Article/details/garamvvao.sHtML

[Q76] 按天统计
来源：http://wap.yfazqb.com/Article/details/gvdomvemo.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://3g.yfazqb.com/Article/details/gbiqicrjz.sHtML

[Q77] 时间加减
来源：http://read.share.epnwcf.com/Article/details/gymeqqgiu.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://wap.sjlbkw.cn/Article/details/gfrqvwqgh.sHtML

[Q78] 当前时间
来源：http://mobile.epnwcf.com/Article/details/grcjvdjoe.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://m.share.tarul.cn/Article/details/gmssbhynq.sHtML

[Q79] 字符串拼接
来源：http://blog.tarul.cn/Article/details/ghrxbxmbl.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://mobile.fktsv.cn/Article/details/gkwxcoaji.sHtML

[Q80] 字符串截取
来源：http://mobile.bbcook.cn/Article/details/gzjutgftf.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://baike.vehdjk.com/Article/details/gptclybgj.sHtML

[Q81] 字符串替换
来源：http://m.share.bbcook.cn/Article/details/geymapkmx.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://read.share.yfazqb.com/Article/details/gbryxvgtq.sHtML

[Q82] 字符长度与字节长度
来源：http://www.share.fktsv.cn/Article/details/gyzotvuot.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.blog.fktsv.cn/Article/details/gbdnijrzq.sHtML

[Q83] 大小写转换
来源：http://read.share.tarul.cn/Article/details/gohnwkbso.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://blog.fktsv.cn/Article/details/gsjllhlxc.sHtML

[Q84] 去除首尾空格
来源：http://mobile.yfazqb.com/Article/details/guwkydsae.sHtML

SELECT TRIM(name) FROM users;
来源：http://mobile.vehdjk.com/Article/details/gbjrzjdpq.sHtML

[Q85] 数值取整
来源：http://www.share.sjlbkw.cn/Article/details/gtmlsqzla.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://wap.tarul.cn/Article/details/gttwsmudn.sHtML

[Q86] 读取 JSON 字段
来源：http://baike.epnwcf.com/Article/details/gsutwnzvg.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.m.share.tarul.cn/Article/details/gunfppgbt.sHtML

[Q87] JSON 字段做条件
来源：http://m.share.bbcook.cn/Article/details/garplbdtm.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.blog.fktsv.cn/Article/details/gdnlfedhn.sHtML

[Q88] 行转列（条件聚合）
来源：http://read.share.fktsv.cn/Article/details/ghdjofwdk.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://blog.yfazqb.com/Article/details/gpetifwfx.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.blog.vehdjk.com/Article/details/gcpxgnyzr.sHtML

[Q89] 判断表是否存在
来源：http://www.blog.fktsv.cn/Article/details/gkqeuyxwr.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.m.share.epnwcf.com/Article/details/goyqanypg.sHtML

[Q90] 生成序号列
来源：http://www.share.fktsv.cn/Article/details/gfsrdoeni.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://blog.yfazqb.com/Article/details/gpfgtteen.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/gszebenbu.sHtML

R. Bash 专题
来源：http://m.share.fktsv.cn/Article/details/glmalwldv.sHtML

================================================================================
来源：http://www.m.share.sjlbkw.cn/Article/details/gnrkzjuyf.sHtML

[R01] shebang 与严格模式
来源：http://www.blog.fktsv.cn/Article/details/gkpbgwrri.sHtML

#!/usr/bin/env bash
来源：http://blog.fktsv.cn/Article/details/gnlvwsuml.sHtML

set -euo pipefail
来源：http://www.blog.tarul.cn/Article/details/guqgzjtqj.sHtML

[R02] 变量赋值与使用
来源：http://www.blog.fktsv.cn/Article/details/gkewkzfjr.sHtML

name="Tom"; echo "$name"
来源：http://www.blog.bbcook.cn/Article/details/gthiijbfe.sHtML

[R03] 只读变量
来源：http://www.blog.tarul.cn/Article/details/gfbjgydus.sHtML

readonly PI=3.14
来源：http://3g.sjlbkw.cn/Article/details/gkqcofeqw.sHtML

[R04] 位置参数
来源：http://mobile.sjlbkw.cn/Article/details/gbsnggkoq.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://baike.sjlbkw.cn/Article/details/gzqicgese.sHtML

[R05] 参数默认值
来源：http://read.share.fktsv.cn/Article/details/gzevzbwrn.sHtML

name="${1:-default}"
来源：http://www.share.tarul.cn/Article/details/garxfdoax.sHtML

[R06] 判断命令是否存在
来源：http://www.share.epnwcf.com/Article/details/glagvhcch.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.m.share.epnwcf.com/Article/details/gpzigafqx.sHtML

[R07] if 判断文件
来源：http://wap.tarul.cn/Article/details/gqibzpcha.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://m.share.sjlbkw.cn/Article/details/gwizielxk.sHtML

[R08] 数值比较
来源：http://www.share.fktsv.cn/Article/details/gflgdvpnw.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.blog.fktsv.cn/Article/details/gqitflbae.sHtML

[R09] 字符串比较
来源：http://blog.tarul.cn/Article/details/ginumavfp.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://baike.fktsv.cn/Article/details/gxriycgaw.sHtML

[R10] 正则匹配
来源：http://m.share.vehdjk.com/Article/details/gwbexnqae.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://baike.fktsv.cn/Article/details/gymoeijke.sHtML

[R11] case 多分支
来源：http://mobile.sjlbkw.cn/Article/details/gsskdohvu.sHtML

case "$1" in
来源：http://read.share.yfazqb.com/Article/details/gtctwuolv.sHtML

start) echo "启动" ;;
来源：http://m.share.sjlbkw.cn/Article/details/ghwsxrwzu.sHtML

stop)  echo "停止" ;;
来源：http://www.blog.sjlbkw.cn/Article/details/gxtndasbs.sHtML

*)     echo "未知命令" ;;
来源：http://mobile.sjlbkw.cn/Article/details/gamyltntb.sHtML

esac
来源：http://www.share.yfazqb.com/Article/details/gipadjnox.sHtML

[R12] for 遍历文件
来源：http://3g.bbcook.cn/Article/details/gaximajcl.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.blog.sjlbkw.cn/Article/details/gdfzvimwz.sHtML

[R13] for 计数循环
来源：http://www.m.share.fktsv.cn/Article/details/gwaplwapo.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://wap.bbcook.cn/Article/details/gnlcwahnd.sHtML

[R14] C 风格 for
来源：http://www.blog.fktsv.cn/Article/details/gbkbxygkf.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://baike.bbcook.cn/Article/details/gsfqicrjj.sHtML

[R15] while 逐行读文件
来源：http://www.blog.sjlbkw.cn/Article/details/gzmyycehm.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://read.share.vehdjk.com/Article/details/gppntjfzc.sHtML

[R16] until 等待条件
来源：http://baike.tarul.cn/Article/details/gttepbzhg.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://m.share.epnwcf.com/Article/details/gfkxujzfh.sHtML

[R17] 数组定义与取值
来源：http://www.blog.tarul.cn/Article/details/gebahalqm.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://3g.vehdjk.com/Article/details/gdgvvtqkm.sHtML

[R18] 遍历数组
来源：http://baike.bbcook.cn/Article/details/gcqbvejsc.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://blog.bbcook.cn/Article/details/gsmejchrv.sHtML

[R19] 数组长度
来源：http://www.blog.fktsv.cn/Article/details/gvmldqedz.sHtML

echo "${#arr[@]}"
来源：http://m.share.yfazqb.com/Article/details/gpxqqaijx.sHtML

[R20] 关联数组（字典）
来源：http://www.m.share.bbcook.cn/Article/details/gacyyxtgx.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.m.share.fktsv.cn/Article/details/gctjfjaym.sHtML

[R21] 字符串长度
来源：http://blog.sjlbkw.cn/Article/details/gsxssbttw.sHtML

echo "${#s}"
来源：http://www.blog.yfazqb.com/Article/details/gdjpxhmld.sHtML

[R22] 截取子串
来源：http://baike.tarul.cn/Article/details/ghmbfkguc.sHtML

echo "${s:0:5}"
来源：http://www.share.fktsv.cn/Article/details/gkrhedvcg.sHtML

[R23] 字符串替换
来源：http://www.m.share.bbcook.cn/Article/details/ghdyqzwbs.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.m.share.yfazqb.com/Article/details/glvydrzkh.sHtML

[R24] 大小写转换
来源：http://blog.epnwcf.com/Article/details/gegtxmvmk.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://m.share.epnwcf.com/Article/details/gogqetfhf.sHtML

[R25] 去后缀 / 去前缀
来源：http://read.share.fktsv.cn/Article/details/govlxqvmn.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://m.share.epnwcf.com/Article/details/ghudcacsl.sHtML

[R26] 命令替换
来源：http://3g.tarul.cn/Article/details/goutypubo.sHtML

now=$(date +%F); echo "$now"
来源：http://baike.vehdjk.com/Article/details/gnfpuejoi.sHtML

[R27] 算术展开
来源：http://www.share.yfazqb.com/Article/details/gnbiphrgq.sHtML

echo $((1 + 2 * 3))
来源：http://www.m.share.vehdjk.com/Article/details/gkdagmara.sHtML

[R28] 浮点运算
来源：http://www.share.yfazqb.com/Article/details/gsomsdvyy.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.share.bbcook.cn/Article/details/gkafrjnvg.sHtML

[R29] 定义函数
来源：http://read.share.sjlbkw.cn/Article/details/gfyxpcyox.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://3g.sjlbkw.cn/Article/details/gzsrjzbei.sHtML

[R30] 函数返回状态码
来源：http://3g.epnwcf.com/Article/details/ghxjbyecq.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://baike.epnwcf.com/Article/details/gkjzedkkk.sHtML

[R31] 局部变量
来源：http://blog.epnwcf.com/Article/details/ghgswqyaq.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.m.share.vehdjk.com/Article/details/genpjseln.sHtML

[R32] 参数个数校验
来源：http://wap.fktsv.cn/Article/details/gkjlbgtgd.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://baike.tarul.cn/Article/details/gtywcqaps.sHtML

[R33] 捕获错误并提示行号
来源：http://blog.bbcook.cn/Article/details/gnjparxoh.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://3g.fktsv.cn/Article/details/glazgfsvk.sHtML

[R34] 退出时清理
来源：http://3g.tarul.cn/Article/details/gajkjnvlb.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.tarul.cn/Article/details/gswiftkdo.sHtML

[R35] 后台执行并等待
来源：http://m.share.sjlbkw.cn/Article/details/gxipztqqa.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://m.share.sjlbkw.cn/Article/details/gkkclgsgv.sHtML

[R36] 并发执行多个任务
来源：http://www.m.share.vehdjk.com/Article/details/gogmhtjry.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://3g.tarul.cn/Article/details/giziozxcj.sHtML

[R37] 把输出赋给变量
来源：http://baike.yfazqb.com/Article/details/giyheaits.sHtML

files=$(ls -1)
来源：http://m.share.fktsv.cn/Article/details/gniphzcev.sHtML

[R38] 管道串联
来源：http://mobile.vehdjk.com/Article/details/ggmekdmbf.sHtML

cat a.txt | grep -i error | wc -l
来源：http://baike.vehdjk.com/Article/details/gwtgqdvjr.sHtML

[R39] 重定向标准输出与错误
来源：http://3g.vehdjk.com/Article/details/gwaysxbkw.sHtML

cmd > out.log 2>&1
来源：http://read.share.bbcook.cn/Article/details/geytqmnap.sHtML

[R40] 追加写日志
来源：http://m.share.bbcook.cn/Article/details/gpfjzqybm.sHtML

echo "log" >> out.log
来源：http://mobile.sjlbkw.cn/Article/details/gndzflgol.sHtML

[R41] 丢弃输出
来源：http://blog.vehdjk.com/Article/details/gengoosvs.sHtML

cmd >/dev/null 2>&1
来源：http://baike.tarul.cn/Article/details/gvjopfbrg.sHtML

[R42] 输入重定向
来源：http://blog.fktsv.cn/Article/details/gfbstdxxm.sHtML

wc -l < a.txt
来源：http://www.share.sjlbkw.cn/Article/details/gvdpcgemr.sHtML

[R43] 按名字查找文件
来源：http://www.blog.fktsv.cn/Article/details/grsxvngih.sHtML

find . -name "*.log" -type f
来源：http://www.m.share.sjlbkw.cn/Article/details/ggjmhupgi.sHtML

[R44] 按修改时间查找
来源：http://www.share.bbcook.cn/Article/details/gnmciffel.sHtML

find . -mtime -7 -type f
来源：http://3g.bbcook.cn/Article/details/gzcnslkri.sHtML

[R45] 批量删除
来源：http://m.share.tarul.cn/Article/details/gjlmtfttc.sHtML

find . -name "*.tmp" -delete
来源：http://3g.tarul.cn/Article/details/ggukhsaxd.sHtML

[R46] 递归替换文件内容
来源：http://www.m.share.vehdjk.com/Article/details/gwqddlmaj.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.blog.fktsv.cn/Article/details/gvcipyyhi.sHtML

[R47] sed 单行替换
来源：http://m.share.sjlbkw.cn/Article/details/gwfqngoxw.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://3g.bbcook.cn/Article/details/gaaplisze.sHtML

[R48] awk 取指定列
来源：http://read.share.fktsv.cn/Article/details/godwyfaos.sHtML

awk '{print $1, $3}' a.txt
来源：http://3g.epnwcf.com/Article/details/gimtvqzjj.sHtML

[R49] awk 带条件
来源：http://mobile.tarul.cn/Article/details/guhaqzcob.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.blog.epnwcf.com/Article/details/gzutjypez.sHtML

[R50] awk 求和
来源：http://m.share.sjlbkw.cn/Article/details/gmgmklbfc.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://read.share.sjlbkw.cn/Article/details/gdekrtzfa.sHtML

[R51] 排序去重取前几
来源：http://baike.vehdjk.com/Article/details/gxyhjkysh.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://baike.fktsv.cn/Article/details/gfaklgdof.sHtML

[R52] 统计行数
来源：http://baike.bbcook.cn/Article/details/glahdtsvt.sHtML

wc -l a.txt
来源：http://wap.epnwcf.com/Article/details/gqbkcrqwh.sHtML

[R53] 查看文件头与实时尾
来源：http://mobile.tarul.cn/Article/details/gkoineoos.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://wap.epnwcf.com/Article/details/gtpuxxmtb.sHtML

[R54] 比较两个文件
来源：http://read.share.tarul.cn/Article/details/gfmkkrnxr.sHtML

diff a.txt b.txt
来源：http://baike.tarul.cn/Article/details/gqpgmuehj.sHtML

[R55] 压缩与解压
来源：http://read.share.tarul.cn/Article/details/gakshupou.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.blog.vehdjk.com/Article/details/gkbitujqe.sHtML

[R56] 远程拷贝
来源：http://www.share.yfazqb.com/Article/details/guqxddtgh.sHtML

scp file user@host:/path/
来源：http://www.share.sjlbkw.cn/Article/details/gjctoeigr.sHtML

[R57] 远程执行命令
来源：http://m.share.bbcook.cn/Article/details/gnljzpjfp.sHtML

ssh user@host 'uptime'
来源：http://3g.tarul.cn/Article/details/guodpucuk.sHtML

[R58] 下载文件
来源：http://m.share.vehdjk.com/Article/details/gmyuyhmjm.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://baike.bbcook.cn/Article/details/gvfmoggtf.sHtML

[R59] 发 POST JSON
来源：http://3g.yfazqb.com/Article/details/gpsgvoora.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://mobile.sjlbkw.cn/Article/details/gyispxeyo.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.share.sjlbkw.cn/Article/details/guieqbwdz.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.share.epnwcf.com/Article/details/gebvrukfc.sHtML

[R61] 磁盘占用
来源：http://mobile.epnwcf.com/Article/details/gakglccwq.sHtML

df -h;  du -sh *
来源：http://read.share.bbcook.cn/Article/details/ggacppyyb.sHtML

[R62] 找最占空间的文件
来源：http://www.m.share.fktsv.cn/Article/details/gxzuattbl.sHtML

du -ah . | sort -rh | head -10
来源：http://3g.bbcook.cn/Article/details/gimgzttmi.sHtML

[R63] 内存与进程
来源：http://3g.epnwcf.com/Article/details/ggunreemn.sHtML

free -h;  ps aux | grep nginx
来源：http://read.share.yfazqb.com/Article/details/gndnidwev.sHtML

[R64] 结束进程
来源：http://baike.epnwcf.com/Article/details/gykyyfalb.sHtML

kill -9 $(pgrep -f app.py)
来源：http://m.share.yfazqb.com/Article/details/glqywrvtn.sHtML

[R65] 查看端口占用
来源：http://m.share.epnwcf.com/Article/details/gguomowrr.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://blog.bbcook.cn/Article/details/goaxyxqxh.sHtML

[R66] 定时任务
来源：http://3g.epnwcf.com/Article/details/grsdnrvrw.sHtML

crontab -e;  crontab -l
来源：http://3g.sjlbkw.cn/Article/details/gaansacia.sHtML

[R67] 生成随机十六进制串
来源：http://baike.bbcook.cn/Article/details/gmorfirgx.sHtML

openssl rand -hex 16
来源：http://mobile.fktsv.cn/Article/details/gmfsjpxkg.sHtML

[R68] 计算文件校验值
来源：http://www.m.share.fktsv.cn/Article/details/gytubrstj.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://3g.yfazqb.com/Article/details/gsjcndklw.sHtML

[R69] 生成随机密码
来源：http://read.share.bbcook.cn/Article/details/gobdvegep.sHtML

head -c 16 /dev/urandom | base64
来源：http://mobile.fktsv.cn/Article/details/gvdojoemk.sHtML

[R70] 时间戳与互转
来源：http://www.share.vehdjk.com/Article/details/gbcgijhcj.sHtML

date +%s;  date -d @1700000000
来源：http://baike.vehdjk.com/Article/details/ghakrpdiv.sHtML

[R71] 日期格式化
来源：http://blog.fktsv.cn/Article/details/gruawhalt.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://m.share.fktsv.cn/Article/details/grrbdcach.sHtML

[R72] 等待端口就绪
来源：http://mobile.bbcook.cn/Article/details/gvlrtaeyl.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://wap.epnwcf.com/Article/details/gwhrotlwt.sHtML

[R73] 分割大日志
来源：http://m.share.vehdjk.com/Article/details/grmbhpqwc.sHtML

split -l 1000 big.log part_
来源：http://baike.bbcook.cn/Article/details/gqddjtjwg.sHtML

[R74] 批量重命名
来源：http://m.share.yfazqb.com/Article/details/grnkobsjd.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://read.share.fktsv.cn/Article/details/gjqztxsto.sHtML

[R75] 导出环境变量
来源：http://wap.tarul.cn/Article/details/gpajitdvg.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://wap.yfazqb.com/Article/details/gvopxpgly.sHtML

[R76] 使用临时文件
来源：http://mobile.yfazqb.com/Article/details/gzlaqzfnb.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://3g.vehdjk.com/Article/details/gsqygslzh.sHtML

[R77] 读取用户输入
来源：http://m.share.bbcook.cn/Article/details/gokhhulgn.sHtML

read -rp "请输入: " ans
来源：http://www.share.bbcook.cn/Article/details/gntvnhuub.sHtML

[R78] 交互式菜单
来源：http://3g.tarul.cn/Article/details/grvzxvnnp.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://3g.epnwcf.com/Article/details/gzrpxjrtz.sHtML

[R79] 解析命令行选项
来源：http://3g.epnwcf.com/Article/details/gebesypwe.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mobile.sjlbkw.cn/Article/details/gmixlzhup.sHtML

[R80] 查看脚本执行耗时
来源：http://wap.vehdjk.com/Article/details/gqzbtbagt.sHtML

time ./run.sh
来源：http://3g.yfazqb.com/Article/details/gepzldwzn.sHtML

================================================================================
来源：http://www.blog.vehdjk.com/Article/details/gnpjpgsaz.sHtML

S. C / C++ 专题
来源：http://read.share.sjlbkw.cn/Article/details/giwlxceee.sHtML

================================================================================
来源：http://www.share.vehdjk.com/Article/details/gepqvjvev.sHtML

[S01] C：Hello World
来源：http://wap.fktsv.cn/Article/details/gsagvygmq.sHtML

#include <stdio.h>
来源：http://blog.tarul.cn/Article/details/gdwzgnxrb.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://3g.tarul.cn/Article/details/gfiarzcdi.sHtML

[S02] C：变量与格式化输出
来源：http://baike.epnwcf.com/Article/details/ggthjkrdk.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.blog.tarul.cn/Article/details/ghjnboqqb.sHtML

[S03] C：读入整数
来源：http://3g.yfazqb.com/Article/details/ghagiinle.sHtML

int x; scanf("%d", &x);
来源：http://blog.sjlbkw.cn/Article/details/gubdclwhw.sHtML

[S04] C：字符串复制
来源：http://www.share.vehdjk.com/Article/details/gocurbsmr.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://baike.sjlbkw.cn/Article/details/ghtmikept.sHtML

[S05] C：字符串长度
来源：http://www.m.share.vehdjk.com/Article/details/giufuvpct.sHtML

strlen(s)
来源：http://read.share.yfazqb.com/Article/details/gyrnnlvcb.sHtML

[S06] C：字符串比较
来源：http://read.share.epnwcf.com/Article/details/gfwxgenwj.sHtML

strcmp(a, b) == 0
来源：http://www.share.sjlbkw.cn/Article/details/gmwdzevzf.sHtML

[S07] C：数组遍历求和
来源：http://mobile.vehdjk.com/Article/details/gswqqefae.sHtML


<!-- 参考信息 -->