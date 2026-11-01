代发 wailian999

SELECT u.name, o.amount FROM users u
来源：http://read.share.epnwcf.com/Article/details/gupmwfzvl.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://3g.epnwcf.com/Article/details/gjxyztsld.sHtML

[Q43] 标量子查询
来源：http://3g.bbcook.cn/Article/details/gzzcqrhtk.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://wap.bbcook.cn/Article/details/gekzdeupc.sHtML

[Q44] IN 子查询
来源：http://www.m.share.epnwcf.com/Article/details/gzkaicgcj.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://3g.epnwcf.com/Article/details/gdbxsicgx.sHtML

[Q45] EXISTS 判断存在
来源：http://blog.sjlbkw.cn/Article/details/gousghkbx.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.vehdjk.com/Article/details/gmaeappap.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://read.share.epnwcf.com/Article/details/gzewgrobw.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.yfazqb.com/Article/details/gbfjlxhfr.sHtML

[Q47] 与平均值比较
来源：http://3g.epnwcf.com/Article/details/gpqevfuko.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://wap.yfazqb.com/Article/details/gkeqjdwrh.sHtML

[Q48] CTE 公用表表达式
来源：http://read.share.vehdjk.com/Article/details/grwhtxlix.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://read.share.epnwcf.com/Article/details/gicycvelb.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://3g.tarul.cn/Article/details/gnaryahsk.sHtML

[Q49] 更新单行
来源：http://www.share.epnwcf.com/Article/details/gcyybjagn.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://baike.bbcook.cn/Article/details/gujniekyg.sHtML

[Q50] 批量更新
来源：http://www.share.tarul.cn/Article/details/gjrfpqmaf.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.m.share.bbcook.cn/Article/details/gckjrsbvl.sHtML

[Q51] 用子查询更新
来源：http://www.share.sjlbkw.cn/Article/details/ghhvkkfln.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://m.share.sjlbkw.cn/Article/details/gdyodelbf.sHtML

[Q52] 删除指定行
来源：http://read.share.yfazqb.com/Article/details/gugpjtwwi.sHtML

DELETE FROM users WHERE id = 10;
来源：http://m.share.vehdjk.com/Article/details/gqompoyry.sHtML

[Q53] 按条件删除
来源：http://baike.epnwcf.com/Article/details/gipdlfllk.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.blog.tarul.cn/Article/details/gueyswdwe.sHtML

[Q54] 清空表
来源：http://baike.sjlbkw.cn/Article/details/guoypmewi.sHtML

TRUNCATE TABLE logs;
来源：http://3g.yfazqb.com/Article/details/gcjrcohxk.sHtML

[Q55] 排名（并列占位）
来源：http://mobile.vehdjk.com/Article/details/gxaiukewj.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://blog.fktsv.cn/Article/details/gddrguoal.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.m.share.tarul.cn/Article/details/givwronhb.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://m.share.tarul.cn/Article/details/gouhlxaws.sHtML

[Q57] 行号
来源：http://mobile.vehdjk.com/Article/details/garqrivif.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://3g.yfazqb.com/Article/details/gzepjyzwm.sHtML

[Q58] 累计求和
来源：http://m.share.bbcook.cn/Article/details/gffdeitpg.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.share.epnwcf.com/Article/details/gydohnjwt.sHtML

[Q59] 分组内累计
来源：http://baike.yfazqb.com/Article/details/gqyowjkrh.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://read.share.tarul.cn/Article/details/golbintam.sHtML

[Q60] 取上一行 / 下一行
来源：http://baike.sjlbkw.cn/Article/details/gwqskniqu.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.blog.tarul.cn/Article/details/gwuzpcpaj.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://m.share.tarul.cn/Article/details/gdsoczlqj.sHtML

[Q61] 移动平均
来源：http://m.share.tarul.cn/Article/details/gsoenyrav.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.m.share.tarul.cn/Article/details/gignqixwy.sHtML

[Q62] 分组占比
来源：http://m.share.fktsv.cn/Article/details/glhmqqmaw.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://blog.epnwcf.com/Article/details/gonqzzzov.sHtML

[Q63] 开启事务
来源：http://mobile.yfazqb.com/Article/details/gemqlmmso.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://read.share.sjlbkw.cn/Article/details/gubwzduaj.sHtML

[Q64] 提交事务
来源：http://www.blog.bbcook.cn/Article/details/gucywfsfa.sHtML

COMMIT;
来源：http://wap.tarul.cn/Article/details/gcqdkhvka.sHtML

[Q65] 回滚事务
来源：http://mobile.bbcook.cn/Article/details/gutzekezf.sHtML

ROLLBACK;
来源：http://read.share.tarul.cn/Article/details/gnguotzyd.sHtML

[Q66] 行锁查询
来源：http://www.m.share.sjlbkw.cn/Article/details/gfwrnxnsu.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://blog.sjlbkw.cn/Article/details/gvevhjrkz.sHtML

[Q67] 设置隔离级别
来源：http://www.m.share.yfazqb.com/Article/details/gbvcychzk.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://m.share.vehdjk.com/Article/details/gkvcppvov.sHtML

[Q68] 保存点
来源：http://mobile.tarul.cn/Article/details/gnsfbvbis.sHtML

SAVEPOINT sp1;
来源：http://baike.fktsv.cn/Article/details/gjxmcmieo.sHtML

ROLLBACK TO sp1;
来源：http://www.share.sjlbkw.cn/Article/details/goaudiuow.sHtML

[Q69] 查看执行计划
来源：http://3g.bbcook.cn/Article/details/gbpdhnezx.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://mobile.epnwcf.com/Article/details/gujuzkwon.sHtML

[Q70] 更新统计信息
来源：http://www.blog.sjlbkw.cn/Article/details/gtjhoxtsl.sHtML

ANALYZE TABLE users;
来源：http://www.share.fktsv.cn/Article/details/gkyshmahv.sHtML

[Q71] 查看建表语句
来源：http://mobile.fktsv.cn/Article/details/gcemzkbsp.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.blog.fktsv.cn/Article/details/geeeauown.sHtML

[Q72] 查看索引
来源：http://www.blog.fktsv.cn/Article/details/gxovomsha.sHtML

SHOW INDEX FROM users;
来源：http://blog.yfazqb.com/Article/details/grajupwka.sHtML

[Q73] 查看表状态
来源：http://baike.bbcook.cn/Article/details/gdlpjlfre.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://wap.yfazqb.com/Article/details/gkymsmlqu.sHtML

[Q74] 强制使用索引
来源：http://m.share.epnwcf.com/Article/details/gbcttnnxm.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://m.share.yfazqb.com/Article/details/gbuezaxwc.sHtML

[Q75] 日期格式化
来源：http://mobile.yfazqb.com/Article/details/gohxxiaje.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://m.share.vehdjk.com/Article/details/glwhagysb.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://read.share.epnwcf.com/Article/details/gphxdhwpp.sHtML

[Q76] 按天统计
来源：http://wap.fktsv.cn/Article/details/ghewdwnpv.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://3g.tarul.cn/Article/details/gzbsaqogy.sHtML

[Q77] 时间加减
来源：http://www.blog.sjlbkw.cn/Article/details/gwqaudgzj.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.share.sjlbkw.cn/Article/details/gmoprtbdm.sHtML

[Q78] 当前时间
来源：http://mobile.bbcook.cn/Article/details/gboliplru.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://blog.bbcook.cn/Article/details/gzfphhvzw.sHtML

[Q79] 字符串拼接
来源：http://www.share.yfazqb.com/Article/details/gkwefglng.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.blog.tarul.cn/Article/details/gdmcofcsi.sHtML

[Q80] 字符串截取
来源：http://read.share.epnwcf.com/Article/details/gtoevvbwn.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.m.share.tarul.cn/Article/details/gadflqnek.sHtML

[Q81] 字符串替换
来源：http://mobile.sjlbkw.cn/Article/details/ggzzfbghb.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://baike.bbcook.cn/Article/details/ggzanovex.sHtML

[Q82] 字符长度与字节长度
来源：http://www.blog.epnwcf.com/Article/details/gdvdfgzuk.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://3g.fktsv.cn/Article/details/gmhxzbdej.sHtML

[Q83] 大小写转换
来源：http://blog.yfazqb.com/Article/details/gqmbcmlam.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://m.share.epnwcf.com/Article/details/gbwkkzvom.sHtML

[Q84] 去除首尾空格
来源：http://www.m.share.fktsv.cn/Article/details/gfruqcxak.sHtML

SELECT TRIM(name) FROM users;
来源：http://mobile.tarul.cn/Article/details/glgpmikfj.sHtML

[Q85] 数值取整
来源：http://blog.bbcook.cn/Article/details/gwwdmnlkc.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://3g.tarul.cn/Article/details/gcgcgfhur.sHtML

[Q86] 读取 JSON 字段
来源：http://baike.yfazqb.com/Article/details/gmhfbvvjv.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://m.share.yfazqb.com/Article/details/gasbwavcc.sHtML

[Q87] JSON 字段做条件
来源：http://www.blog.epnwcf.com/Article/details/ggfsomjdc.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://wap.epnwcf.com/Article/details/gpgqhmeak.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.m.share.sjlbkw.cn/Article/details/glcppkxqg.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://3g.fktsv.cn/Article/details/gvizerxrn.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://baike.yfazqb.com/Article/details/gblatqowx.sHtML

[Q89] 判断表是否存在
来源：http://wap.tarul.cn/Article/details/gxexhgibn.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://mobile.bbcook.cn/Article/details/gkbsolrlj.sHtML

[Q90] 生成序号列
来源：http://www.share.bbcook.cn/Article/details/gxxdnivtw.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://baike.sjlbkw.cn/Article/details/gerccgrbt.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/gvsgasqzm.sHtML

R. Bash 专题
来源：http://m.share.epnwcf.com/Article/details/gtgbcifjj.sHtML

================================================================================
来源：http://www.share.epnwcf.com/Article/details/gblnzmgoh.sHtML

[R01] shebang 与严格模式
来源：http://m.share.tarul.cn/Article/details/gnxcxuuga.sHtML

#!/usr/bin/env bash
来源：http://baike.bbcook.cn/Article/details/gsbxyhurh.sHtML

set -euo pipefail
来源：http://baike.sjlbkw.cn/Article/details/gbqsuuxaw.sHtML

[R02] 变量赋值与使用
来源：http://3g.bbcook.cn/Article/details/gjtkpbrxy.sHtML

name="Tom"; echo "$name"
来源：http://m.share.tarul.cn/Article/details/glucxcqfv.sHtML

[R03] 只读变量
来源：http://blog.epnwcf.com/Article/details/gdetiqmnl.sHtML

readonly PI=3.14
来源：http://blog.yfazqb.com/Article/details/gtazpalel.sHtML

[R04] 位置参数
来源：http://www.m.share.tarul.cn/Article/details/gfznyprbs.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://mobile.fktsv.cn/Article/details/gcgvlujnd.sHtML

[R05] 参数默认值
来源：http://www.m.share.tarul.cn/Article/details/gesiujkpz.sHtML

name="${1:-default}"
来源：http://read.share.vehdjk.com/Article/details/gsfpnffsb.sHtML

[R06] 判断命令是否存在
来源：http://wap.sjlbkw.cn/Article/details/ghlcqmodu.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://baike.fktsv.cn/Article/details/ghuqmpjjj.sHtML

[R07] if 判断文件
来源：http://www.blog.sjlbkw.cn/Article/details/gfcihriwz.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://3g.tarul.cn/Article/details/gsifylxoi.sHtML

[R08] 数值比较
来源：http://read.share.bbcook.cn/Article/details/gyfozmnvs.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.blog.epnwcf.com/Article/details/gyimtfkxj.sHtML

[R09] 字符串比较
来源：http://wap.tarul.cn/Article/details/gavplxzsa.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://3g.sjlbkw.cn/Article/details/gelecysqt.sHtML

[R10] 正则匹配
来源：http://www.m.share.fktsv.cn/Article/details/gwqvqltxz.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://3g.epnwcf.com/Article/details/geecvfiog.sHtML

[R11] case 多分支
来源：http://www.m.share.yfazqb.com/Article/details/ghqynzzzx.sHtML

case "$1" in
来源：http://blog.tarul.cn/Article/details/gssejzidc.sHtML

start) echo "启动" ;;
来源：http://3g.sjlbkw.cn/Article/details/ggrcmsasm.sHtML

stop)  echo "停止" ;;
来源：http://m.share.fktsv.cn/Article/details/gplieypln.sHtML

*)     echo "未知命令" ;;
来源：http://baike.bbcook.cn/Article/details/gltkysqev.sHtML

esac
来源：http://www.blog.yfazqb.com/Article/details/ghfwvpghs.sHtML

[R12] for 遍历文件
来源：http://wap.sjlbkw.cn/Article/details/gpedejtjc.sHtML

for f in *.txt; do echo "$f"; done
来源：http://3g.epnwcf.com/Article/details/gtxxtxfyb.sHtML

[R13] for 计数循环
来源：http://blog.fktsv.cn/Article/details/gaulogbwo.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://read.share.bbcook.cn/Article/details/gumtkxsni.sHtML

[R14] C 风格 for
来源：http://baike.tarul.cn/Article/details/gsaporwuw.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.blog.tarul.cn/Article/details/gmjmzbbnk.sHtML

[R15] while 逐行读文件
来源：http://blog.tarul.cn/Article/details/gfdioxnio.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.m.share.sjlbkw.cn/Article/details/gidziuugc.sHtML

[R16] until 等待条件
来源：http://www.m.share.bbcook.cn/Article/details/giibxjied.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://wap.tarul.cn/Article/details/gledhrfpa.sHtML

[R17] 数组定义与取值
来源：http://www.m.share.vehdjk.com/Article/details/garwmclgg.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://m.share.yfazqb.com/Article/details/gqajbtpan.sHtML

[R18] 遍历数组
来源：http://www.m.share.bbcook.cn/Article/details/gufuzcjbn.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.blog.vehdjk.com/Article/details/ggwkldjgu.sHtML

[R19] 数组长度
来源：http://www.m.share.yfazqb.com/Article/details/grexnzmmm.sHtML

echo "${#arr[@]}"
来源：http://read.share.epnwcf.com/Article/details/grjcjltmg.sHtML

[R20] 关联数组（字典）
来源：http://wap.sjlbkw.cn/Article/details/goygodwgt.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://mobile.vehdjk.com/Article/details/gduzgnxsk.sHtML

[R21] 字符串长度
来源：http://m.share.vehdjk.com/Article/details/gylpghaps.sHtML

echo "${#s}"
来源：http://read.share.yfazqb.com/Article/details/gnugizppn.sHtML

[R22] 截取子串
来源：http://blog.epnwcf.com/Article/details/gfqxjmzwy.sHtML

echo "${s:0:5}"
来源：http://www.m.share.vehdjk.com/Article/details/gkpuvzvxi.sHtML

[R23] 字符串替换
来源：http://www.m.share.tarul.cn/Article/details/gjtxfwzma.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://baike.fktsv.cn/Article/details/gduvtaojd.sHtML

[R24] 大小写转换
来源：http://www.m.share.fktsv.cn/Article/details/gsmmtvptc.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://3g.epnwcf.com/Article/details/gusvofarx.sHtML

[R25] 去后缀 / 去前缀
来源：http://m.share.bbcook.cn/Article/details/gnkrcejeh.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://m.share.tarul.cn/Article/details/gajwtpfrh.sHtML

[R26] 命令替换
来源：http://wap.epnwcf.com/Article/details/gwlzbmfdl.sHtML

now=$(date +%F); echo "$now"
来源：http://www.share.bbcook.cn/Article/details/ginznyxbz.sHtML

[R27] 算术展开
来源：http://m.share.bbcook.cn/Article/details/gnzwqzqoh.sHtML

echo $((1 + 2 * 3))
来源：http://baike.yfazqb.com/Article/details/gkxmjcodx.sHtML

[R28] 浮点运算
来源：http://read.share.sjlbkw.cn/Article/details/gxlkdbbqc.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.blog.fktsv.cn/Article/details/gagjdyzoa.sHtML

[R29] 定义函数
来源：http://blog.vehdjk.com/Article/details/gwtwfaqhj.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://mobile.tarul.cn/Article/details/gbjhufwkz.sHtML

[R30] 函数返回状态码
来源：http://www.share.fktsv.cn/Article/details/gwrveedqn.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.blog.fktsv.cn/Article/details/giiacmjyi.sHtML

[R31] 局部变量
来源：http://wap.vehdjk.com/Article/details/gnwonrxlq.sHtML

f() { local x=1; echo "$x"; }
来源：http://baike.epnwcf.com/Article/details/gulwqvhts.sHtML

[R32] 参数个数校验
来源：http://www.blog.vehdjk.com/Article/details/gafkkwvao.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://mobile.vehdjk.com/Article/details/gytbueixu.sHtML

[R33] 捕获错误并提示行号
来源：http://mobile.vehdjk.com/Article/details/guwpkmeer.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.m.share.sjlbkw.cn/Article/details/gqkyeffpk.sHtML

[R34] 退出时清理
来源：http://blog.epnwcf.com/Article/details/ghvcxivmr.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.yfazqb.com/Article/details/gocvkpmkq.sHtML

[R35] 后台执行并等待
来源：http://wap.vehdjk.com/Article/details/grtvhidhe.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://3g.tarul.cn/Article/details/gnwjblvdw.sHtML

[R36] 并发执行多个任务
来源：http://read.share.fktsv.cn/Article/details/ggxizmjvo.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://wap.vehdjk.com/Article/details/grrayttbf.sHtML

[R37] 把输出赋给变量
来源：http://m.share.vehdjk.com/Article/details/gdruglwnb.sHtML

files=$(ls -1)
来源：http://www.share.bbcook.cn/Article/details/gswzbiobn.sHtML

[R38] 管道串联
来源：http://baike.bbcook.cn/Article/details/gexfzdkci.sHtML

cat a.txt | grep -i error | wc -l
来源：http://m.share.yfazqb.com/Article/details/gwxxyxrvs.sHtML

[R39] 重定向标准输出与错误
来源：http://baike.fktsv.cn/Article/details/gnprslorg.sHtML

cmd > out.log 2>&1
来源：http://wap.yfazqb.com/Article/details/gifdvjapn.sHtML

[R40] 追加写日志
来源：http://www.m.share.yfazqb.com/Article/details/gzzitmksc.sHtML

echo "log" >> out.log
来源：http://read.share.vehdjk.com/Article/details/gtmgcoqcj.sHtML

[R41] 丢弃输出
来源：http://www.blog.sjlbkw.cn/Article/details/gxegcysra.sHtML

cmd >/dev/null 2>&1
来源：http://m.share.yfazqb.com/Article/details/gaqqhsgge.sHtML

[R42] 输入重定向
来源：http://wap.sjlbkw.cn/Article/details/gislpxhvj.sHtML

wc -l < a.txt
来源：http://mobile.sjlbkw.cn/Article/details/grsowvbxt.sHtML

[R43] 按名字查找文件
来源：http://www.share.epnwcf.com/Article/details/gxmqouvmk.sHtML

find . -name "*.log" -type f
来源：http://www.m.share.vehdjk.com/Article/details/gvermimvm.sHtML

[R44] 按修改时间查找
来源：http://mobile.tarul.cn/Article/details/gpyqbekdj.sHtML

find . -mtime -7 -type f
来源：http://3g.epnwcf.com/Article/details/ghddzfcsf.sHtML

[R45] 批量删除
来源：http://www.blog.fktsv.cn/Article/details/gmdqrifaa.sHtML

find . -name "*.tmp" -delete
来源：http://www.share.fktsv.cn/Article/details/gisadcplj.sHtML

[R46] 递归替换文件内容
来源：http://www.m.share.bbcook.cn/Article/details/gsesbelvz.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://m.share.bbcook.cn/Article/details/gofelvbts.sHtML

[R47] sed 单行替换
来源：http://baike.bbcook.cn/Article/details/gxholikrq.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://blog.vehdjk.com/Article/details/gdmxlvnqi.sHtML

[R48] awk 取指定列
来源：http://www.m.share.yfazqb.com/Article/details/ggfvbfwmq.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.blog.bbcook.cn/Article/details/gzmnhfyws.sHtML

[R49] awk 带条件
来源：http://read.share.yfazqb.com/Article/details/gvaqvudbv.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://3g.tarul.cn/Article/details/ghfynofoj.sHtML

[R50] awk 求和
来源：http://m.share.sjlbkw.cn/Article/details/gstrhsvbw.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://mobile.vehdjk.com/Article/details/gbuiurkfz.sHtML

[R51] 排序去重取前几
来源：http://m.share.bbcook.cn/Article/details/geapciukc.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://m.share.tarul.cn/Article/details/garrladqa.sHtML

[R52] 统计行数
来源：http://www.share.epnwcf.com/Article/details/gcouyblok.sHtML

wc -l a.txt
来源：http://wap.bbcook.cn/Article/details/gbzlyajlw.sHtML

[R53] 查看文件头与实时尾
来源：http://wap.epnwcf.com/Article/details/gnsmsttxu.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://blog.sjlbkw.cn/Article/details/gfuufjley.sHtML

[R54] 比较两个文件
来源：http://m.share.bbcook.cn/Article/details/gsofbwely.sHtML

diff a.txt b.txt
来源：http://3g.bbcook.cn/Article/details/getrssvys.sHtML

[R55] 压缩与解压
来源：http://www.share.bbcook.cn/Article/details/ggaknjpss.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://baike.vehdjk.com/Article/details/ghizvjsyb.sHtML

[R56] 远程拷贝
来源：http://mobile.tarul.cn/Article/details/gyakswpwk.sHtML

scp file user@host:/path/
来源：http://www.share.fktsv.cn/Article/details/gqqmragyq.sHtML

[R57] 远程执行命令
来源：http://www.blog.tarul.cn/Article/details/gvibiipoq.sHtML

ssh user@host 'uptime'
来源：http://3g.sjlbkw.cn/Article/details/gvkskknbc.sHtML

[R58] 下载文件
来源：http://blog.tarul.cn/Article/details/gasjqxyjt.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.m.share.yfazqb.com/Article/details/gpugfazwp.sHtML

[R59] 发 POST JSON
来源：http://read.share.fktsv.cn/Article/details/gppftszag.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://mobile.epnwcf.com/Article/details/gwckgvrvh.sHtML

[R60] 只看 HTTP 状态码
来源：http://3g.fktsv.cn/Article/details/giqokfwue.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.m.share.bbcook.cn/Article/details/gznjcxwmj.sHtML

[R61] 磁盘占用
来源：http://www.m.share.vehdjk.com/Article/details/gdblczwsq.sHtML

df -h;  du -sh *
来源：http://wap.tarul.cn/Article/details/gencctyeb.sHtML

[R62] 找最占空间的文件
来源：http://m.share.sjlbkw.cn/Article/details/grtipyxcw.sHtML

du -ah . | sort -rh | head -10
来源：http://www.m.share.yfazqb.com/Article/details/gacmismmk.sHtML

[R63] 内存与进程
来源：http://baike.sjlbkw.cn/Article/details/gtwcefnxq.sHtML

free -h;  ps aux | grep nginx
来源：http://www.blog.tarul.cn/Article/details/ggekiihgt.sHtML

[R64] 结束进程
来源：http://www.m.share.sjlbkw.cn/Article/details/gmfbhahce.sHtML

kill -9 $(pgrep -f app.py)
来源：http://read.share.bbcook.cn/Article/details/ghzeiclrg.sHtML

[R65] 查看端口占用
来源：http://www.m.share.epnwcf.com/Article/details/gkgjxndty.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://baike.tarul.cn/Article/details/gjgmqxbrp.sHtML

[R66] 定时任务
来源：http://blog.sjlbkw.cn/Article/details/gfwimjcgh.sHtML

crontab -e;  crontab -l
来源：http://www.m.share.sjlbkw.cn/Article/details/gnousaeqt.sHtML

[R67] 生成随机十六进制串
来源：http://baike.sjlbkw.cn/Article/details/gkkelisoq.sHtML

openssl rand -hex 16
来源：http://read.share.tarul.cn/Article/details/gzbtfvrrr.sHtML

[R68] 计算文件校验值
来源：http://wap.yfazqb.com/Article/details/gcuoyjlye.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://blog.yfazqb.com/Article/details/gngczipsi.sHtML

[R69] 生成随机密码
来源：http://baike.bbcook.cn/Article/details/gteiuppsa.sHtML

head -c 16 /dev/urandom | base64
来源：http://read.share.epnwcf.com/Article/details/gcfenrlxk.sHtML

[R70] 时间戳与互转
来源：http://mobile.epnwcf.com/Article/details/gmtkjbnyd.sHtML

date +%s;  date -d @1700000000
来源：http://m.share.yfazqb.com/Article/details/gggbmkacn.sHtML

[R71] 日期格式化
来源：http://www.blog.yfazqb.com/Article/details/gnbplbszz.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://baike.vehdjk.com/Article/details/gkhaxqgfb.sHtML

[R72] 等待端口就绪
来源：http://www.blog.yfazqb.com/Article/details/gdloeoxsh.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://wap.tarul.cn/Article/details/gvfoqnuzd.sHtML

[R73] 分割大日志
来源：http://baike.tarul.cn/Article/details/gpwhwruoz.sHtML

split -l 1000 big.log part_
来源：http://wap.epnwcf.com/Article/details/gbwwmwrro.sHtML

[R74] 批量重命名
来源：http://blog.tarul.cn/Article/details/gykfgfeoq.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.blog.bbcook.cn/Article/details/gpyymuxmn.sHtML

[R75] 导出环境变量
来源：http://wap.epnwcf.com/Article/details/gvthiemzm.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.m.share.bbcook.cn/Article/details/gmfiluspp.sHtML

[R76] 使用临时文件
来源：http://www.m.share.bbcook.cn/Article/details/gvsckuxba.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://blog.bbcook.cn/Article/details/gelccgvov.sHtML

[R77] 读取用户输入
来源：http://m.share.epnwcf.com/Article/details/gfidedbci.sHtML

read -rp "请输入: " ans
来源：http://wap.epnwcf.com/Article/details/gpazlyeil.sHtML

[R78] 交互式菜单
来源：http://baike.tarul.cn/Article/details/gbhedzmvo.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.blog.yfazqb.com/Article/details/gxepfhxer.sHtML

[R79] 解析命令行选项
来源：http://3g.bbcook.cn/Article/details/gtogexdoa.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mobile.vehdjk.com/Article/details/gcalyjnfk.sHtML

[R80] 查看脚本执行耗时
来源：http://blog.vehdjk.com/Article/details/gfpalqogj.sHtML

time ./run.sh
来源：http://wap.bbcook.cn/Article/details/gktcemifr.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/goeaceymk.sHtML

S. C / C++ 专题
来源：http://www.blog.tarul.cn/Article/details/gybihqsbo.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/ginmawzxj.sHtML

[S01] C：Hello World
来源：http://baike.vehdjk.com/Article/details/gvoxyttmg.sHtML

#include <stdio.h>
来源：http://blog.bbcook.cn/Article/details/gyakpgzqz.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://read.share.fktsv.cn/Article/details/grglgpjau.sHtML

[S02] C：变量与格式化输出
来源：http://m.share.yfazqb.com/Article/details/gzynyeukb.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.m.share.fktsv.cn/Article/details/gidkrdett.sHtML

[S03] C：读入整数
来源：http://wap.sjlbkw.cn/Article/details/gqjqddupq.sHtML

int x; scanf("%d", &x);
来源：http://www.m.share.yfazqb.com/Article/details/gbhwvmqmc.sHtML

[S04] C：字符串复制
来源：http://3g.sjlbkw.cn/Article/details/gnbkzmcgc.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.share.yfazqb.com/Article/details/ghyyxruog.sHtML

[S05] C：字符串长度
来源：http://m.share.bbcook.cn/Article/details/gkomvntfq.sHtML

strlen(s)
来源：http://blog.sjlbkw.cn/Article/details/gingxyfcg.sHtML

[S06] C：字符串比较
来源：http://read.share.sjlbkw.cn/Article/details/gkcrtotgk.sHtML

strcmp(a, b) == 0
来源：http://www.m.share.yfazqb.com/Article/details/glqmdwxhv.sHtML

[S07] C：数组遍历求和
来源：http://wap.vehdjk.com/Article/details/gmfkznhzm.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.m.share.fktsv.cn/Article/details/gvooiwlig.sHtML

[S08] C：动态内存分配与释放
来源：http://read.share.tarul.cn/Article/details/gddjflemq.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://wap.yfazqb.com/Article/details/grhkeorxe.sHtML

[S09] C：结构体定义与初始化
来源：http://read.share.epnwcf.com/Article/details/gqmkbyvuk.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://baike.sjlbkw.cn/Article/details/gptcuwiye.sHtML

[S10] C：指针与解引用
来源：http://blog.yfazqb.com/Article/details/gcqydlhph.sHtML

int *p = &a;  *p = 5;
来源：http://blog.bbcook.cn/Article/details/gfokzoifw.sHtML

[S11] C：逐行读文件
来源：http://www.m.share.bbcook.cn/Article/details/gfgmsptpf.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.share.vehdjk.com/Article/details/gzhudnbof.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://wap.fktsv.cn/Article/details/ghmglezyw.sHtML

fclose(f);
来源：http://wap.sjlbkw.cn/Article/details/grdfstjqd.sHtML

[S12] C：写文件
来源：http://www.blog.fktsv.cn/Article/details/gpsiiavma.sHtML


<!-- 参考信息 -->