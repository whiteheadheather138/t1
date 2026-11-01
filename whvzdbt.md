代发 wailian999

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://baike.vehdjk.com/Article/details/gnexawokq.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://mobile.bbcook.cn/Article/details/gpbqzsfol.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.blog.epnwcf.com/Article/details/ghdqdxqbw.sHtML

[Q41] 多表连接
来源：http://3g.vehdjk.com/Article/details/gbvrbgcqf.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.m.share.sjlbkw.cn/Article/details/gwplexfmb.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.share.sjlbkw.cn/Article/details/gdijkxiuf.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.blog.sjlbkw.cn/Article/details/gsxoeoigj.sHtML

[Q42] 连接条件附加过滤
来源：http://blog.sjlbkw.cn/Article/details/gojiiufko.sHtML

SELECT u.name, o.amount FROM users u
来源：http://baike.tarul.cn/Article/details/gsmsacupl.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://wap.sjlbkw.cn/Article/details/gncuiklxk.sHtML

[Q43] 标量子查询
来源：http://mobile.fktsv.cn/Article/details/grjfjofdz.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.share.vehdjk.com/Article/details/govvvishj.sHtML

[Q44] IN 子查询
来源：http://www.share.fktsv.cn/Article/details/gsljtywnc.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://mobile.bbcook.cn/Article/details/gmivggoux.sHtML

[Q45] EXISTS 判断存在
来源：http://m.share.fktsv.cn/Article/details/ghhdvnosq.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.vehdjk.com/Article/details/gzbdrcnhb.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.blog.tarul.cn/Article/details/gnfuhfmdm.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.sjlbkw.cn/Article/details/gulflqpdw.sHtML

[Q47] 与平均值比较
来源：http://m.share.epnwcf.com/Article/details/gowqiwcyr.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://3g.sjlbkw.cn/Article/details/gxhcyvrtl.sHtML

[Q48] CTE 公用表表达式
来源：http://blog.epnwcf.com/Article/details/grupweksz.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.share.epnwcf.com/Article/details/gwvrhobdj.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://read.share.epnwcf.com/Article/details/gtsontawp.sHtML

[Q49] 更新单行
来源：http://www.m.share.vehdjk.com/Article/details/gbeoyfbio.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://blog.vehdjk.com/Article/details/gbfpjxsll.sHtML

[Q50] 批量更新
来源：http://www.m.share.fktsv.cn/Article/details/gxayhuzmm.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.blog.tarul.cn/Article/details/gejoxqzjm.sHtML

[Q51] 用子查询更新
来源：http://mobile.yfazqb.com/Article/details/gwqdilori.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://baike.epnwcf.com/Article/details/gfdfogylg.sHtML

[Q52] 删除指定行
来源：http://www.m.share.sjlbkw.cn/Article/details/gikuwhlsv.sHtML

DELETE FROM users WHERE id = 10;
来源：http://wap.fktsv.cn/Article/details/gvvmqqush.sHtML

[Q53] 按条件删除
来源：http://baike.epnwcf.com/Article/details/geacgarkd.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://m.share.vehdjk.com/Article/details/giwyelwhb.sHtML

[Q54] 清空表
来源：http://www.m.share.tarul.cn/Article/details/gjmticgjn.sHtML

TRUNCATE TABLE logs;
来源：http://m.share.epnwcf.com/Article/details/gtmifpoyy.sHtML

[Q55] 排名（并列占位）
来源：http://read.share.epnwcf.com/Article/details/gjsjktfac.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://wap.vehdjk.com/Article/details/gbjrqyovs.sHtML

[Q56] 密集排名（并列不占位）
来源：http://m.share.yfazqb.com/Article/details/ggoaayqlf.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://wap.yfazqb.com/Article/details/gexfdbnab.sHtML

[Q57] 行号
来源：http://www.blog.tarul.cn/Article/details/gtlppjgha.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://3g.fktsv.cn/Article/details/gxnuikkkr.sHtML

[Q58] 累计求和
来源：http://wap.tarul.cn/Article/details/gqvyzjalv.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://baike.vehdjk.com/Article/details/gjjqjinrl.sHtML

[Q59] 分组内累计
来源：http://www.m.share.fktsv.cn/Article/details/gbcfpobht.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.m.share.yfazqb.com/Article/details/gfbkhjwfk.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.blog.vehdjk.com/Article/details/gecxyytue.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://mobile.sjlbkw.cn/Article/details/gkosrmlsb.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://m.share.sjlbkw.cn/Article/details/gacskdrrf.sHtML

[Q61] 移动平均
来源：http://wap.fktsv.cn/Article/details/ggdrtidrs.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.share.epnwcf.com/Article/details/grzaqhgda.sHtML

[Q62] 分组占比
来源：http://3g.bbcook.cn/Article/details/gzwilthtb.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.m.share.epnwcf.com/Article/details/ggqiwgtbh.sHtML

[Q63] 开启事务
来源：http://www.blog.epnwcf.com/Article/details/guyqbiymi.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://wap.yfazqb.com/Article/details/gdnolefra.sHtML

[Q64] 提交事务
来源：http://m.share.tarul.cn/Article/details/gmjgksukc.sHtML

COMMIT;
来源：http://mobile.bbcook.cn/Article/details/gahcstlav.sHtML

[Q65] 回滚事务
来源：http://www.m.share.sjlbkw.cn/Article/details/gcallpaos.sHtML

ROLLBACK;
来源：http://read.share.tarul.cn/Article/details/gdgrngmlb.sHtML

[Q66] 行锁查询
来源：http://wap.vehdjk.com/Article/details/gehafsqrr.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://3g.epnwcf.com/Article/details/gubmsbspr.sHtML

[Q67] 设置隔离级别
来源：http://3g.fktsv.cn/Article/details/gyllewqur.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.blog.yfazqb.com/Article/details/girrvhtur.sHtML

[Q68] 保存点
来源：http://www.blog.vehdjk.com/Article/details/gfbxcdhij.sHtML

SAVEPOINT sp1;
来源：http://wap.sjlbkw.cn/Article/details/glkaoiwhv.sHtML

ROLLBACK TO sp1;
来源：http://www.m.share.epnwcf.com/Article/details/gsezbifbf.sHtML

[Q69] 查看执行计划
来源：http://read.share.bbcook.cn/Article/details/gqimjkziw.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.share.bbcook.cn/Article/details/greqisend.sHtML

[Q70] 更新统计信息
来源：http://www.share.tarul.cn/Article/details/gciusspdi.sHtML

ANALYZE TABLE users;
来源：http://www.blog.tarul.cn/Article/details/gxxurxuyw.sHtML

[Q71] 查看建表语句
来源：http://www.share.sjlbkw.cn/Article/details/gjzspjism.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.m.share.sjlbkw.cn/Article/details/glftvrnos.sHtML

[Q72] 查看索引
来源：http://wap.yfazqb.com/Article/details/gfujsyknm.sHtML

SHOW INDEX FROM users;
来源：http://mobile.sjlbkw.cn/Article/details/gtpdaagfq.sHtML

[Q73] 查看表状态
来源：http://baike.yfazqb.com/Article/details/gxhxlfdxb.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.m.share.yfazqb.com/Article/details/gqrclhrnk.sHtML

[Q74] 强制使用索引
来源：http://wap.tarul.cn/Article/details/gwxvawzlx.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://blog.bbcook.cn/Article/details/gwdeclfkt.sHtML

[Q75] 日期格式化
来源：http://www.share.tarul.cn/Article/details/gxwmkutxk.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://mobile.epnwcf.com/Article/details/gyyphqazc.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://blog.bbcook.cn/Article/details/ghmckpysh.sHtML

[Q76] 按天统计
来源：http://3g.yfazqb.com/Article/details/giztnrljp.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.m.share.sjlbkw.cn/Article/details/gliwkiqlk.sHtML

[Q77] 时间加减
来源：http://3g.sjlbkw.cn/Article/details/geqyvpddc.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://blog.sjlbkw.cn/Article/details/gfhvbuktx.sHtML

[Q78] 当前时间
来源：http://3g.tarul.cn/Article/details/gnwzzdust.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://blog.sjlbkw.cn/Article/details/gwnpzywtz.sHtML

[Q79] 字符串拼接
来源：http://blog.tarul.cn/Article/details/gdiauyaee.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://blog.sjlbkw.cn/Article/details/gmgheuurq.sHtML

[Q80] 字符串截取
来源：http://3g.yfazqb.com/Article/details/gfoeqdsze.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://baike.epnwcf.com/Article/details/gtrvgjtxu.sHtML

[Q81] 字符串替换
来源：http://mobile.sjlbkw.cn/Article/details/gtakfzuuw.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://read.share.fktsv.cn/Article/details/geqzhpcdp.sHtML

[Q82] 字符长度与字节长度
来源：http://wap.epnwcf.com/Article/details/ghohhurvd.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://read.share.bbcook.cn/Article/details/gvoohrykq.sHtML

[Q83] 大小写转换
来源：http://www.blog.sjlbkw.cn/Article/details/gkgizagwg.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://3g.bbcook.cn/Article/details/gogyrjhnf.sHtML

[Q84] 去除首尾空格
来源：http://www.blog.yfazqb.com/Article/details/gzflinjoc.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.m.share.sjlbkw.cn/Article/details/gwvvankqg.sHtML

[Q85] 数值取整
来源：http://read.share.fktsv.cn/Article/details/gzoggcgkk.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://m.share.fktsv.cn/Article/details/gqzjrxfym.sHtML

[Q86] 读取 JSON 字段
来源：http://www.blog.sjlbkw.cn/Article/details/gainmfezq.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://baike.fktsv.cn/Article/details/giqvhxafb.sHtML

[Q87] JSON 字段做条件
来源：http://3g.vehdjk.com/Article/details/gmwemtsqj.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.blog.bbcook.cn/Article/details/guafugadh.sHtML

[Q88] 行转列（条件聚合）
来源：http://read.share.vehdjk.com/Article/details/gnelojwds.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.blog.fktsv.cn/Article/details/gyhlsowct.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://m.share.fktsv.cn/Article/details/gijkwxzoc.sHtML

[Q89] 判断表是否存在
来源：http://blog.yfazqb.com/Article/details/gyngcgjcs.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://wap.tarul.cn/Article/details/gienrvuqh.sHtML

[Q90] 生成序号列
来源：http://blog.vehdjk.com/Article/details/gixkncypd.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.blog.sjlbkw.cn/Article/details/ghxaauozt.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/geuohdhey.sHtML

R. Bash 专题
来源：http://www.blog.sjlbkw.cn/Article/details/gdnnekeiw.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/guhoqerby.sHtML

[R01] shebang 与严格模式
来源：http://baike.sjlbkw.cn/Article/details/govvcbxye.sHtML

#!/usr/bin/env bash
来源：http://wap.sjlbkw.cn/Article/details/gwmhxmcqr.sHtML

set -euo pipefail
来源：http://wap.yfazqb.com/Article/details/gqjmozoyn.sHtML

[R02] 变量赋值与使用
来源：http://read.share.yfazqb.com/Article/details/gdvngsepi.sHtML

name="Tom"; echo "$name"
来源：http://m.share.epnwcf.com/Article/details/glixombox.sHtML

[R03] 只读变量
来源：http://www.share.yfazqb.com/Article/details/gujeagvzr.sHtML

readonly PI=3.14
来源：http://baike.sjlbkw.cn/Article/details/ggscozqbc.sHtML

[R04] 位置参数
来源：http://m.share.bbcook.cn/Article/details/gmdyvjcyi.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://m.share.epnwcf.com/Article/details/gszaxucgk.sHtML

[R05] 参数默认值
来源：http://mobile.epnwcf.com/Article/details/goptrywfk.sHtML

name="${1:-default}"
来源：http://mobile.vehdjk.com/Article/details/ghkujdexf.sHtML

[R06] 判断命令是否存在
来源：http://baike.epnwcf.com/Article/details/gumsewvpv.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://read.share.tarul.cn/Article/details/gdmzktlih.sHtML

[R07] if 判断文件
来源：http://wap.yfazqb.com/Article/details/gadjbxsvn.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://wap.tarul.cn/Article/details/gydxziinu.sHtML

[R08] 数值比较
来源：http://3g.vehdjk.com/Article/details/gcscqvwly.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://mobile.sjlbkw.cn/Article/details/gpvzeqyyv.sHtML

[R09] 字符串比较
来源：http://mobile.vehdjk.com/Article/details/gxbcskvzl.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://blog.yfazqb.com/Article/details/ggdlwkzrp.sHtML

[R10] 正则匹配
来源：http://mobile.yfazqb.com/Article/details/gdnolsdym.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://3g.tarul.cn/Article/details/geffmacbb.sHtML

[R11] case 多分支
来源：http://blog.fktsv.cn/Article/details/gfzfuocay.sHtML

case "$1" in
来源：http://baike.vehdjk.com/Article/details/gdqmiucjo.sHtML

start) echo "启动" ;;
来源：http://baike.vehdjk.com/Article/details/gtqgddxuj.sHtML

stop)  echo "停止" ;;
来源：http://www.m.share.yfazqb.com/Article/details/ghxiqogqp.sHtML

*)     echo "未知命令" ;;
来源：http://www.blog.bbcook.cn/Article/details/gqjzyloay.sHtML

esac
来源：http://www.m.share.yfazqb.com/Article/details/gneordotn.sHtML

[R12] for 遍历文件
来源：http://www.blog.fktsv.cn/Article/details/gpfkiguww.sHtML

for f in *.txt; do echo "$f"; done
来源：http://baike.epnwcf.com/Article/details/gwudwpugl.sHtML

[R13] for 计数循环
来源：http://mobile.bbcook.cn/Article/details/gacitkfov.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.m.share.tarul.cn/Article/details/gcwgwrigv.sHtML

[R14] C 风格 for
来源：http://3g.vehdjk.com/Article/details/gifqipnff.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://3g.epnwcf.com/Article/details/gtzcalufj.sHtML

[R15] while 逐行读文件
来源：http://blog.tarul.cn/Article/details/geoxuhcne.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://3g.fktsv.cn/Article/details/gthjnjqgy.sHtML

[R16] until 等待条件
来源：http://read.share.bbcook.cn/Article/details/guklrbwta.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://m.share.epnwcf.com/Article/details/gtwgftgpy.sHtML

[R17] 数组定义与取值
来源：http://www.share.fktsv.cn/Article/details/gzuolfpsy.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.m.share.sjlbkw.cn/Article/details/gdqgitchh.sHtML

[R18] 遍历数组
来源：http://baike.yfazqb.com/Article/details/giyrtwggw.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.blog.sjlbkw.cn/Article/details/glajfpcsp.sHtML

[R19] 数组长度
来源：http://www.m.share.tarul.cn/Article/details/gveqswsgt.sHtML

echo "${#arr[@]}"
来源：http://m.share.epnwcf.com/Article/details/gxhwsioda.sHtML

[R20] 关联数组（字典）
来源：http://blog.epnwcf.com/Article/details/gbizlflii.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://m.share.yfazqb.com/Article/details/gzjgxyzwr.sHtML

[R21] 字符串长度
来源：http://www.blog.vehdjk.com/Article/details/ghgievdhw.sHtML

echo "${#s}"
来源：http://mobile.vehdjk.com/Article/details/gnrdclyri.sHtML

[R22] 截取子串
来源：http://www.share.yfazqb.com/Article/details/gwzgjtgla.sHtML

echo "${s:0:5}"
来源：http://www.blog.vehdjk.com/Article/details/gaemqanir.sHtML

[R23] 字符串替换
来源：http://mobile.fktsv.cn/Article/details/gwhsneaow.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://baike.yfazqb.com/Article/details/gueqcaoji.sHtML

[R24] 大小写转换
来源：http://3g.epnwcf.com/Article/details/grxcvlowk.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.share.sjlbkw.cn/Article/details/gbpzjgygb.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.m.share.epnwcf.com/Article/details/gfegcflwa.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://baike.bbcook.cn/Article/details/ggzxluckw.sHtML

[R26] 命令替换
来源：http://wap.tarul.cn/Article/details/gxogrhiqe.sHtML

now=$(date +%F); echo "$now"
来源：http://mobile.tarul.cn/Article/details/gcprzaatc.sHtML

[R27] 算术展开
来源：http://www.blog.yfazqb.com/Article/details/gfvhmkoem.sHtML

echo $((1 + 2 * 3))
来源：http://3g.bbcook.cn/Article/details/gjgzrdhfs.sHtML

[R28] 浮点运算
来源：http://www.share.vehdjk.com/Article/details/gxequupwr.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.blog.fktsv.cn/Article/details/gukgyfkxk.sHtML

[R29] 定义函数
来源：http://read.share.epnwcf.com/Article/details/gjvebymcl.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://baike.epnwcf.com/Article/details/gwphedctq.sHtML

[R30] 函数返回状态码
来源：http://www.blog.tarul.cn/Article/details/gutyfgqfl.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.m.share.fktsv.cn/Article/details/ggwxfwysq.sHtML

[R31] 局部变量
来源：http://3g.yfazqb.com/Article/details/guluplpkw.sHtML

f() { local x=1; echo "$x"; }
来源：http://baike.vehdjk.com/Article/details/ghtagueka.sHtML

[R32] 参数个数校验
来源：http://baike.yfazqb.com/Article/details/gplospuot.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://read.share.epnwcf.com/Article/details/grakqfcxf.sHtML

[R33] 捕获错误并提示行号
来源：http://m.share.epnwcf.com/Article/details/gsjxgnszk.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://baike.sjlbkw.cn/Article/details/giaxgneoc.sHtML

[R34] 退出时清理
来源：http://blog.vehdjk.com/Article/details/gbksmupyv.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://baike.epnwcf.com/Article/details/gkskjwkcn.sHtML

[R35] 后台执行并等待
来源：http://blog.bbcook.cn/Article/details/gonggdtwl.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://wap.vehdjk.com/Article/details/gciehpaya.sHtML

[R36] 并发执行多个任务
来源：http://3g.vehdjk.com/Article/details/gtyinsbqo.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://wap.yfazqb.com/Article/details/gwenlfltf.sHtML

[R37] 把输出赋给变量
来源：http://3g.yfazqb.com/Article/details/gqkzhhauv.sHtML

files=$(ls -1)
来源：http://blog.epnwcf.com/Article/details/gbruxfjdb.sHtML

[R38] 管道串联
来源：http://www.blog.vehdjk.com/Article/details/gxsdglbgb.sHtML

cat a.txt | grep -i error | wc -l
来源：http://read.share.bbcook.cn/Article/details/gfqzvfbsr.sHtML

[R39] 重定向标准输出与错误
来源：http://www.m.share.sjlbkw.cn/Article/details/gvxfpkkpr.sHtML

cmd > out.log 2>&1
来源：http://wap.yfazqb.com/Article/details/gaqxbrjsy.sHtML

[R40] 追加写日志
来源：http://read.share.fktsv.cn/Article/details/gfuedzrjy.sHtML

echo "log" >> out.log
来源：http://www.share.bbcook.cn/Article/details/gkzntkgvg.sHtML

[R41] 丢弃输出
来源：http://blog.fktsv.cn/Article/details/gztkjzaig.sHtML

cmd >/dev/null 2>&1
来源：http://blog.fktsv.cn/Article/details/guxviimvp.sHtML

[R42] 输入重定向
来源：http://read.share.fktsv.cn/Article/details/gnfkegzwy.sHtML

wc -l < a.txt
来源：http://www.m.share.tarul.cn/Article/details/gdewcckdh.sHtML

[R43] 按名字查找文件
来源：http://read.share.fktsv.cn/Article/details/gkrdgaybc.sHtML

find . -name "*.log" -type f
来源：http://baike.tarul.cn/Article/details/gleguboww.sHtML

[R44] 按修改时间查找
来源：http://mobile.vehdjk.com/Article/details/gaorxevpf.sHtML

find . -mtime -7 -type f
来源：http://mobile.sjlbkw.cn/Article/details/gdececpac.sHtML

[R45] 批量删除
来源：http://www.blog.vehdjk.com/Article/details/gxztadxtl.sHtML

find . -name "*.tmp" -delete
来源：http://blog.fktsv.cn/Article/details/gszifhgia.sHtML

[R46] 递归替换文件内容
来源：http://wap.yfazqb.com/Article/details/gssdbhuas.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mobile.tarul.cn/Article/details/gfwlrfkdo.sHtML

[R47] sed 单行替换
来源：http://baike.tarul.cn/Article/details/gcuvlptvv.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://m.share.vehdjk.com/Article/details/gmjhasbxu.sHtML

[R48] awk 取指定列
来源：http://wap.epnwcf.com/Article/details/govwqkewk.sHtML

awk '{print $1, $3}' a.txt
来源：http://baike.yfazqb.com/Article/details/gfufabntc.sHtML

[R49] awk 带条件
来源：http://wap.yfazqb.com/Article/details/giwirsxlr.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://3g.vehdjk.com/Article/details/gxkefvppg.sHtML

[R50] awk 求和
来源：http://blog.tarul.cn/Article/details/gzqrqcvps.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://blog.fktsv.cn/Article/details/gkiionvao.sHtML

[R51] 排序去重取前几
来源：http://wap.yfazqb.com/Article/details/grkzvykxh.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://read.share.sjlbkw.cn/Article/details/gpzcgwkfu.sHtML

[R52] 统计行数
来源：http://read.share.vehdjk.com/Article/details/gmxfshxiu.sHtML

wc -l a.txt
来源：http://www.share.epnwcf.com/Article/details/grkwvwwuf.sHtML

[R53] 查看文件头与实时尾
来源：http://3g.tarul.cn/Article/details/gvkradrhy.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://blog.sjlbkw.cn/Article/details/gzzmuytkd.sHtML

[R54] 比较两个文件
来源：http://www.blog.bbcook.cn/Article/details/gpdsyrsgd.sHtML

diff a.txt b.txt
来源：http://read.share.epnwcf.com/Article/details/ggqbwhpmu.sHtML

[R55] 压缩与解压
来源：http://www.blog.epnwcf.com/Article/details/gsvdflbtl.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://read.share.yfazqb.com/Article/details/gafvxpbcw.sHtML

[R56] 远程拷贝
来源：http://www.m.share.sjlbkw.cn/Article/details/gklqqkumx.sHtML

scp file user@host:/path/
来源：http://www.share.yfazqb.com/Article/details/gjjomzihu.sHtML

[R57] 远程执行命令
来源：http://read.share.sjlbkw.cn/Article/details/gikztabsp.sHtML

ssh user@host 'uptime'
来源：http://www.share.tarul.cn/Article/details/gcnvlwrcx.sHtML

[R58] 下载文件
来源：http://mobile.bbcook.cn/Article/details/gsjoatdae.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://mobile.fktsv.cn/Article/details/gvmypirov.sHtML

[R59] 发 POST JSON
来源：http://blog.bbcook.cn/Article/details/gntkewtbf.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.m.share.yfazqb.com/Article/details/gpgdnshmd.sHtML

[R60] 只看 HTTP 状态码
来源：http://read.share.tarul.cn/Article/details/gzxwhenda.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.share.sjlbkw.cn/Article/details/gkcfhidmb.sHtML

[R61] 磁盘占用
来源：http://wap.fktsv.cn/Article/details/gftomwrxj.sHtML

df -h;  du -sh *
来源：http://blog.vehdjk.com/Article/details/gvkxpxhlw.sHtML

[R62] 找最占空间的文件
来源：http://blog.bbcook.cn/Article/details/gabbhafja.sHtML

du -ah . | sort -rh | head -10
来源：http://wap.fktsv.cn/Article/details/gjkrywdtt.sHtML

[R63] 内存与进程
来源：http://baike.vehdjk.com/Article/details/gmjfzgukz.sHtML

free -h;  ps aux | grep nginx
来源：http://m.share.epnwcf.com/Article/details/gjentuobw.sHtML

[R64] 结束进程
来源：http://blog.vehdjk.com/Article/details/gwqcbeiru.sHtML

kill -9 $(pgrep -f app.py)
来源：http://wap.yfazqb.com/Article/details/gzrfmbrto.sHtML

[R65] 查看端口占用
来源：http://m.share.epnwcf.com/Article/details/gfajdogjh.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.blog.fktsv.cn/Article/details/gwkwzljgm.sHtML

[R66] 定时任务
来源：http://blog.epnwcf.com/Article/details/gmwsxrqbm.sHtML

crontab -e;  crontab -l
来源：http://3g.bbcook.cn/Article/details/gofxkqdck.sHtML

[R67] 生成随机十六进制串
来源：http://www.m.share.tarul.cn/Article/details/guxovwzcr.sHtML

openssl rand -hex 16
来源：http://www.share.epnwcf.com/Article/details/gblrqqqcr.sHtML

[R68] 计算文件校验值
来源：http://mobile.epnwcf.com/Article/details/gfdyqcojd.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://blog.yfazqb.com/Article/details/gkpbkwdfh.sHtML

[R69] 生成随机密码
来源：http://www.m.share.tarul.cn/Article/details/gimlfuchr.sHtML

head -c 16 /dev/urandom | base64
来源：http://3g.tarul.cn/Article/details/gpzbtkhgr.sHtML

[R70] 时间戳与互转
来源：http://m.share.vehdjk.com/Article/details/glnxouver.sHtML

date +%s;  date -d @1700000000
来源：http://mobile.sjlbkw.cn/Article/details/gqvrroddm.sHtML

[R71] 日期格式化
来源：http://blog.vehdjk.com/Article/details/godhiwzpl.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.share.vehdjk.com/Article/details/gkttyidpi.sHtML

[R72] 等待端口就绪
来源：http://blog.sjlbkw.cn/Article/details/gkooxhbyj.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://read.share.epnwcf.com/Article/details/gwgvgpdpg.sHtML

[R73] 分割大日志
来源：http://read.share.fktsv.cn/Article/details/gvsxrlbnb.sHtML

split -l 1000 big.log part_
来源：http://www.share.yfazqb.com/Article/details/gvdowfjqc.sHtML

[R74] 批量重命名
来源：http://read.share.epnwcf.com/Article/details/glxiuvabd.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.share.fktsv.cn/Article/details/gknjjefau.sHtML

[R75] 导出环境变量
来源：http://3g.vehdjk.com/Article/details/gsglkvhma.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.share.yfazqb.com/Article/details/gpvlijclr.sHtML

[R76] 使用临时文件
来源：http://www.blog.tarul.cn/Article/details/getxjzaxc.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.tarul.cn/Article/details/gkarmticm.sHtML

[R77] 读取用户输入
来源：http://3g.epnwcf.com/Article/details/giolwlpwj.sHtML

read -rp "请输入: " ans
来源：http://www.blog.sjlbkw.cn/Article/details/gdyxdilvy.sHtML

[R78] 交互式菜单
来源：http://www.blog.sjlbkw.cn/Article/details/gsrefedmo.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://baike.sjlbkw.cn/Article/details/gtmorogdq.sHtML

[R79] 解析命令行选项
来源：http://mobile.bbcook.cn/Article/details/gbsxzyowo.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://3g.sjlbkw.cn/Article/details/gdpkybeoa.sHtML

[R80] 查看脚本执行耗时
来源：http://wap.tarul.cn/Article/details/gllktykzr.sHtML

time ./run.sh
来源：http://read.share.yfazqb.com/Article/details/gasnnzbks.sHtML

================================================================================
来源：http://baike.tarul.cn/Article/details/gwlvhbdco.sHtML

S. C / C++ 专题
来源：http://www.blog.sjlbkw.cn/Article/details/gbzzvkzat.sHtML

================================================================================
来源：http://mobile.yfazqb.com/Article/details/gqvlerzae.sHtML

[S01] C：Hello World
来源：http://www.share.vehdjk.com/Article/details/ggebvqvzw.sHtML

#include <stdio.h>
来源：http://wap.sjlbkw.cn/Article/details/gkztzcjzj.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://3g.sjlbkw.cn/Article/details/gstuinhag.sHtML

[S02] C：变量与格式化输出
来源：http://mobile.fktsv.cn/Article/details/gqfywkwwy.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.m.share.epnwcf.com/Article/details/gzmksjyzb.sHtML

[S03] C：读入整数
来源：http://www.share.yfazqb.com/Article/details/gynbzagfs.sHtML

int x; scanf("%d", &x);
来源：http://www.m.share.bbcook.cn/Article/details/gxbgjcmox.sHtML

[S04] C：字符串复制
来源：http://mobile.yfazqb.com/Article/details/gjmbekkqu.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://read.share.tarul.cn/Article/details/gaefvscaa.sHtML

[S05] C：字符串长度
来源：http://3g.vehdjk.com/Article/details/geghcajas.sHtML

strlen(s)
来源：http://read.share.yfazqb.com/Article/details/guwynbeqj.sHtML

[S06] C：字符串比较
来源：http://3g.bbcook.cn/Article/details/grsedbvtr.sHtML

strcmp(a, b) == 0
来源：http://mobile.yfazqb.com/Article/details/ghcaxrfyw.sHtML

[S07] C：数组遍历求和
来源：http://m.share.vehdjk.com/Article/details/gdbkdtrxo.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://mobile.vehdjk.com/Article/details/gmhblbyjn.sHtML

[S08] C：动态内存分配与释放
来源：http://www.m.share.sjlbkw.cn/Article/details/gmsnzkvwi.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://3g.tarul.cn/Article/details/gabobalzb.sHtML

[S09] C：结构体定义与初始化
来源：http://wap.bbcook.cn/Article/details/ggmveafcz.sHtML


<!-- 参考信息 -->