代发 wailian999

SELECT u.name, o.amount FROM users u
来源：http://3g.bbcook.cn/Article/details/gcbvblveg.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.m.share.fktsv.cn/Article/details/ggqwusuhg.sHtML

[Q43] 标量子查询
来源：http://3g.bbcook.cn/Article/details/grqkykgae.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.m.share.bbcook.cn/Article/details/gyluvwvpw.sHtML

[Q44] IN 子查询
来源：http://blog.bbcook.cn/Article/details/gqtdfvdel.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://m.share.sjlbkw.cn/Article/details/gtkwcxeez.sHtML

[Q45] EXISTS 判断存在
来源：http://mobile.sjlbkw.cn/Article/details/gefkrfekf.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.epnwcf.com/Article/details/ggnackhjy.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://3g.epnwcf.com/Article/details/gofskldnv.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.tarul.cn/Article/details/gydabsvyb.sHtML

[Q47] 与平均值比较
来源：http://wap.yfazqb.com/Article/details/gzpawgsar.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://3g.tarul.cn/Article/details/gsmjoahas.sHtML

[Q48] CTE 公用表表达式
来源：http://www.blog.epnwcf.com/Article/details/gzbareqkn.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://read.share.tarul.cn/Article/details/gqrykofda.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://m.share.vehdjk.com/Article/details/gpbhuhsdm.sHtML

[Q49] 更新单行
来源：http://www.share.fktsv.cn/Article/details/gdverwxja.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://baike.vehdjk.com/Article/details/guoginqji.sHtML

[Q50] 批量更新
来源：http://www.blog.sjlbkw.cn/Article/details/gvfomrlit.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.m.share.fktsv.cn/Article/details/gzbohhhqa.sHtML

[Q51] 用子查询更新
来源：http://wap.bbcook.cn/Article/details/gajaniplr.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://read.share.vehdjk.com/Article/details/geupurrkb.sHtML

[Q52] 删除指定行
来源：http://m.share.epnwcf.com/Article/details/gpswlsznj.sHtML

DELETE FROM users WHERE id = 10;
来源：http://m.share.tarul.cn/Article/details/gdrvurqxa.sHtML

[Q53] 按条件删除
来源：http://blog.bbcook.cn/Article/details/gomwmcfqj.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://3g.bbcook.cn/Article/details/glxlsfism.sHtML

[Q54] 清空表
来源：http://baike.yfazqb.com/Article/details/gprspylqs.sHtML

TRUNCATE TABLE logs;
来源：http://blog.tarul.cn/Article/details/gplmpqrjr.sHtML

[Q55] 排名（并列占位）
来源：http://www.m.share.epnwcf.com/Article/details/gldlmvnrb.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.share.tarul.cn/Article/details/gdtrjcmxv.sHtML

[Q56] 密集排名（并列不占位）
来源：http://baike.bbcook.cn/Article/details/gulxoaprl.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://baike.epnwcf.com/Article/details/grchcweik.sHtML

[Q57] 行号
来源：http://www.share.vehdjk.com/Article/details/gqwsknvur.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://3g.vehdjk.com/Article/details/gimvqbhjz.sHtML

[Q58] 累计求和
来源：http://www.m.share.bbcook.cn/Article/details/gspjtfozr.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://baike.fktsv.cn/Article/details/gslmdfcdw.sHtML

[Q59] 分组内累计
来源：http://www.m.share.yfazqb.com/Article/details/gkqfzuvcx.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://wap.yfazqb.com/Article/details/glctqtyzz.sHtML

[Q60] 取上一行 / 下一行
来源：http://blog.tarul.cn/Article/details/gxfinjhkq.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.m.share.bbcook.cn/Article/details/gixmxvsvk.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://mobile.fktsv.cn/Article/details/ggiszsatq.sHtML

[Q61] 移动平均
来源：http://baike.epnwcf.com/Article/details/gthhozogy.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://read.share.epnwcf.com/Article/details/gksfkjful.sHtML

[Q62] 分组占比
来源：http://mobile.vehdjk.com/Article/details/ggzyxnonn.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://wap.yfazqb.com/Article/details/gezrgsovy.sHtML

[Q63] 开启事务
来源：http://wap.yfazqb.com/Article/details/ghcqnumop.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.blog.vehdjk.com/Article/details/gpzjhsyez.sHtML

[Q64] 提交事务
来源：http://mobile.bbcook.cn/Article/details/gpguevudb.sHtML

COMMIT;
来源：http://m.share.sjlbkw.cn/Article/details/gahnpxnmo.sHtML

[Q65] 回滚事务
来源：http://www.m.share.tarul.cn/Article/details/grutvtipq.sHtML

ROLLBACK;
来源：http://blog.epnwcf.com/Article/details/ghtdxfivq.sHtML

[Q66] 行锁查询
来源：http://wap.bbcook.cn/Article/details/gqxukysvk.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://3g.yfazqb.com/Article/details/gpwcbgxhf.sHtML

[Q67] 设置隔离级别
来源：http://wap.bbcook.cn/Article/details/grgnwawtf.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.m.share.bbcook.cn/Article/details/guqjqnqtn.sHtML

[Q68] 保存点
来源：http://mobile.tarul.cn/Article/details/gccnxlboz.sHtML

SAVEPOINT sp1;
来源：http://www.m.share.tarul.cn/Article/details/gcxmceidh.sHtML

ROLLBACK TO sp1;
来源：http://baike.bbcook.cn/Article/details/gmcnlkcnh.sHtML

[Q69] 查看执行计划
来源：http://baike.vehdjk.com/Article/details/gzdouojcd.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://blog.yfazqb.com/Article/details/gnrqdajby.sHtML

[Q70] 更新统计信息
来源：http://baike.tarul.cn/Article/details/gdifqzmos.sHtML

ANALYZE TABLE users;
来源：http://read.share.vehdjk.com/Article/details/griwawxek.sHtML

[Q71] 查看建表语句
来源：http://blog.sjlbkw.cn/Article/details/gftzvurvr.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.share.fktsv.cn/Article/details/gqhcbqfiw.sHtML

[Q72] 查看索引
来源：http://read.share.sjlbkw.cn/Article/details/gjmwzokrd.sHtML

SHOW INDEX FROM users;
来源：http://m.share.epnwcf.com/Article/details/gcmvbtpdw.sHtML

[Q73] 查看表状态
来源：http://www.m.share.fktsv.cn/Article/details/ggndshjlj.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://read.share.sjlbkw.cn/Article/details/gdmgtmhkv.sHtML

[Q74] 强制使用索引
来源：http://m.share.vehdjk.com/Article/details/ghnilfrlf.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://baike.bbcook.cn/Article/details/grwdeflnq.sHtML

[Q75] 日期格式化
来源：http://www.m.share.bbcook.cn/Article/details/gpoxyzfol.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://blog.yfazqb.com/Article/details/gbcetmhnd.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://m.share.tarul.cn/Article/details/gyypzsswr.sHtML

[Q76] 按天统计
来源：http://blog.vehdjk.com/Article/details/gprogjkbs.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://3g.yfazqb.com/Article/details/grtttvjpf.sHtML

[Q77] 时间加减
来源：http://www.m.share.epnwcf.com/Article/details/gwcstwdpa.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://mobile.yfazqb.com/Article/details/gnrgfehsh.sHtML

[Q78] 当前时间
来源：http://mobile.tarul.cn/Article/details/gqchgsdyn.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://baike.epnwcf.com/Article/details/gwdxureos.sHtML

[Q79] 字符串拼接
来源：http://blog.bbcook.cn/Article/details/glaxelbna.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://mobile.epnwcf.com/Article/details/gziilhnox.sHtML

[Q80] 字符串截取
来源：http://www.m.share.tarul.cn/Article/details/gccffrzak.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://mobile.vehdjk.com/Article/details/gtavdushx.sHtML

[Q81] 字符串替换
来源：http://mobile.tarul.cn/Article/details/giqcfnkhm.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.m.share.epnwcf.com/Article/details/ggodyklnz.sHtML

[Q82] 字符长度与字节长度
来源：http://baike.fktsv.cn/Article/details/grtxawaft.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://blog.epnwcf.com/Article/details/gsjpqmfae.sHtML

[Q83] 大小写转换
来源：http://www.blog.epnwcf.com/Article/details/gjzajgnfy.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://baike.bbcook.cn/Article/details/gcpbnesln.sHtML

[Q84] 去除首尾空格
来源：http://mobile.fktsv.cn/Article/details/gfumvdqfi.sHtML

SELECT TRIM(name) FROM users;
来源：http://3g.bbcook.cn/Article/details/gjawhmxrm.sHtML

[Q85] 数值取整
来源：http://www.blog.fktsv.cn/Article/details/grzrunzmu.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://wap.bbcook.cn/Article/details/gpccrubrz.sHtML

[Q86] 读取 JSON 字段
来源：http://read.share.sjlbkw.cn/Article/details/gtynckmoq.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://baike.sjlbkw.cn/Article/details/gemldhdwb.sHtML

[Q87] JSON 字段做条件
来源：http://read.share.epnwcf.com/Article/details/gyrslvxkt.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://blog.epnwcf.com/Article/details/glcedvqra.sHtML

[Q88] 行转列（条件聚合）
来源：http://mobile.bbcook.cn/Article/details/gyzhdwtly.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.blog.bbcook.cn/Article/details/gmwuzvhyi.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.m.share.vehdjk.com/Article/details/goibacuxe.sHtML

[Q89] 判断表是否存在
来源：http://read.share.yfazqb.com/Article/details/gwukzqdkq.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://blog.tarul.cn/Article/details/gdpvemlfy.sHtML

[Q90] 生成序号列
来源：http://www.blog.bbcook.cn/Article/details/gwkcgyery.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.m.share.epnwcf.com/Article/details/gghgzrnrm.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/gifzesxju.sHtML

R. Bash 专题
来源：http://mobile.fktsv.cn/Article/details/glpqtulch.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/gklkpzmnd.sHtML

[R01] shebang 与严格模式
来源：http://baike.yfazqb.com/Article/details/grwwcqogw.sHtML

#!/usr/bin/env bash
来源：http://read.share.tarul.cn/Article/details/ggzqaeqxw.sHtML

set -euo pipefail
来源：http://baike.fktsv.cn/Article/details/guhpxauzj.sHtML

[R02] 变量赋值与使用
来源：http://wap.yfazqb.com/Article/details/gdezggsjg.sHtML

name="Tom"; echo "$name"
来源：http://3g.bbcook.cn/Article/details/ggkaxapbt.sHtML

[R03] 只读变量
来源：http://wap.epnwcf.com/Article/details/gpgfdvywn.sHtML

readonly PI=3.14
来源：http://m.share.vehdjk.com/Article/details/gjwiruhlc.sHtML

[R04] 位置参数
来源：http://www.m.share.bbcook.cn/Article/details/ghxuhkoxg.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://mobile.tarul.cn/Article/details/ghzkscylb.sHtML

[R05] 参数默认值
来源：http://www.m.share.sjlbkw.cn/Article/details/gtxuuityg.sHtML

name="${1:-default}"
来源：http://www.m.share.vehdjk.com/Article/details/gstlqbhbz.sHtML

[R06] 判断命令是否存在
来源：http://baike.bbcook.cn/Article/details/gzffhvstu.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://wap.tarul.cn/Article/details/gqpaqqfda.sHtML

[R07] if 判断文件
来源：http://wap.sjlbkw.cn/Article/details/gxjghmonk.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://mobile.vehdjk.com/Article/details/grzsrrvyt.sHtML

[R08] 数值比较
来源：http://blog.tarul.cn/Article/details/gdvgfswrb.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://m.share.sjlbkw.cn/Article/details/gcrwdgtji.sHtML

[R09] 字符串比较
来源：http://3g.sjlbkw.cn/Article/details/gkhxggwxb.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://m.share.tarul.cn/Article/details/gyxiswxtl.sHtML

[R10] 正则匹配
来源：http://www.m.share.sjlbkw.cn/Article/details/ghjsdkiiw.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.share.tarul.cn/Article/details/gcemaphat.sHtML

[R11] case 多分支
来源：http://www.blog.fktsv.cn/Article/details/gsonieqdv.sHtML

case "$1" in
来源：http://m.share.sjlbkw.cn/Article/details/guyuhcvba.sHtML

start) echo "启动" ;;
来源：http://mobile.yfazqb.com/Article/details/gmyywkqnz.sHtML

stop)  echo "停止" ;;
来源：http://m.share.epnwcf.com/Article/details/gzcvjeyoq.sHtML

*)     echo "未知命令" ;;
来源：http://read.share.vehdjk.com/Article/details/gybwgmcda.sHtML

esac
来源：http://mobile.vehdjk.com/Article/details/gamqjcxtq.sHtML

[R12] for 遍历文件
来源：http://www.share.bbcook.cn/Article/details/gekqzvqtl.sHtML

for f in *.txt; do echo "$f"; done
来源：http://read.share.sjlbkw.cn/Article/details/gdmffnibk.sHtML

[R13] for 计数循环
来源：http://www.m.share.bbcook.cn/Article/details/gvcnikukm.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://baike.epnwcf.com/Article/details/gqlccwjev.sHtML

[R14] C 风格 for
来源：http://blog.epnwcf.com/Article/details/gglevfbpi.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://blog.fktsv.cn/Article/details/geivbrjca.sHtML

[R15] while 逐行读文件
来源：http://www.blog.epnwcf.com/Article/details/guyydvzcy.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://blog.yfazqb.com/Article/details/gudsqkjsz.sHtML

[R16] until 等待条件
来源：http://read.share.sjlbkw.cn/Article/details/glddimkii.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.share.epnwcf.com/Article/details/grtohndqw.sHtML

[R17] 数组定义与取值
来源：http://blog.epnwcf.com/Article/details/gbhzqmaie.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://read.share.vehdjk.com/Article/details/gijppqunp.sHtML

[R18] 遍历数组
来源：http://blog.epnwcf.com/Article/details/gbgfsjwps.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://read.share.epnwcf.com/Article/details/gqrsargrq.sHtML

[R19] 数组长度
来源：http://read.share.epnwcf.com/Article/details/ggsuhlroc.sHtML

echo "${#arr[@]}"
来源：http://blog.vehdjk.com/Article/details/gekrcfhiu.sHtML

[R20] 关联数组（字典）
来源：http://www.m.share.yfazqb.com/Article/details/gfqwyfhwr.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.m.share.tarul.cn/Article/details/guzoomspd.sHtML

[R21] 字符串长度
来源：http://wap.fktsv.cn/Article/details/gqjtexztj.sHtML

echo "${#s}"
来源：http://3g.tarul.cn/Article/details/gejqvsrud.sHtML

[R22] 截取子串
来源：http://3g.epnwcf.com/Article/details/gmzizinst.sHtML

echo "${s:0:5}"
来源：http://mobile.fktsv.cn/Article/details/gamuduqfo.sHtML

[R23] 字符串替换
来源：http://m.share.vehdjk.com/Article/details/gbxporeqf.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://wap.fktsv.cn/Article/details/gziertmrr.sHtML

[R24] 大小写转换
来源：http://www.m.share.fktsv.cn/Article/details/gorxdpjgx.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://m.share.sjlbkw.cn/Article/details/gwwssiqaz.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.share.yfazqb.com/Article/details/ghmfrkrnx.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://mobile.vehdjk.com/Article/details/geeuojgzy.sHtML

[R26] 命令替换
来源：http://mobile.epnwcf.com/Article/details/gzldaspad.sHtML

now=$(date +%F); echo "$now"
来源：http://baike.bbcook.cn/Article/details/ghzaxzctr.sHtML

[R27] 算术展开
来源：http://3g.vehdjk.com/Article/details/gernfujwn.sHtML

echo $((1 + 2 * 3))
来源：http://baike.yfazqb.com/Article/details/gaxchlkct.sHtML

[R28] 浮点运算
来源：http://3g.sjlbkw.cn/Article/details/gulnujmzh.sHtML

echo "scale=2; 10/3" | bc
来源：http://wap.tarul.cn/Article/details/gogfafvyk.sHtML

[R29] 定义函数
来源：http://m.share.bbcook.cn/Article/details/gnuuimeza.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.share.epnwcf.com/Article/details/grncirewh.sHtML

[R30] 函数返回状态码
来源：http://m.share.bbcook.cn/Article/details/guylvrntb.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://3g.yfazqb.com/Article/details/gpdegxvnk.sHtML

[R31] 局部变量
来源：http://3g.tarul.cn/Article/details/gpomvelkn.sHtML

f() { local x=1; echo "$x"; }
来源：http://baike.tarul.cn/Article/details/gyiroxpdt.sHtML

[R32] 参数个数校验
来源：http://wap.sjlbkw.cn/Article/details/gasiwohgi.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://m.share.tarul.cn/Article/details/gqbortong.sHtML

[R33] 捕获错误并提示行号
来源：http://m.share.sjlbkw.cn/Article/details/gwmbvhhfi.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://baike.epnwcf.com/Article/details/gzkcjsdqj.sHtML

[R34] 退出时清理
来源：http://read.share.vehdjk.com/Article/details/gfkbtixng.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://mobile.bbcook.cn/Article/details/gtdrglhpo.sHtML

[R35] 后台执行并等待
来源：http://blog.fktsv.cn/Article/details/gfcjucptt.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.blog.fktsv.cn/Article/details/gmbucxiju.sHtML

[R36] 并发执行多个任务
来源：http://3g.fktsv.cn/Article/details/gnbkjlgps.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://wap.sjlbkw.cn/Article/details/gxpbzgcqj.sHtML

[R37] 把输出赋给变量
来源：http://mobile.fktsv.cn/Article/details/gxjjcligz.sHtML

files=$(ls -1)
来源：http://www.share.epnwcf.com/Article/details/gyidyrjni.sHtML

[R38] 管道串联
来源：http://www.m.share.vehdjk.com/Article/details/gdhjqltnr.sHtML

cat a.txt | grep -i error | wc -l
来源：http://3g.vehdjk.com/Article/details/gustxonrw.sHtML

[R39] 重定向标准输出与错误
来源：http://read.share.bbcook.cn/Article/details/gtkdhyrjh.sHtML

cmd > out.log 2>&1
来源：http://3g.sjlbkw.cn/Article/details/gmvrauele.sHtML

[R40] 追加写日志
来源：http://read.share.sjlbkw.cn/Article/details/gojdbaqnv.sHtML

echo "log" >> out.log
来源：http://www.blog.sjlbkw.cn/Article/details/gnbpqtony.sHtML

[R41] 丢弃输出
来源：http://mobile.tarul.cn/Article/details/gwyncaaqq.sHtML

cmd >/dev/null 2>&1
来源：http://read.share.tarul.cn/Article/details/gqjtnlnep.sHtML

[R42] 输入重定向
来源：http://www.share.sjlbkw.cn/Article/details/gtgzokapu.sHtML

wc -l < a.txt
来源：http://3g.vehdjk.com/Article/details/gvejbdbdv.sHtML

[R43] 按名字查找文件
来源：http://3g.tarul.cn/Article/details/goewtovrz.sHtML

find . -name "*.log" -type f
来源：http://www.m.share.bbcook.cn/Article/details/gqfekdnrc.sHtML

[R44] 按修改时间查找
来源：http://www.blog.fktsv.cn/Article/details/gvokoxldx.sHtML

find . -mtime -7 -type f
来源：http://www.m.share.vehdjk.com/Article/details/gukcazhlr.sHtML

[R45] 批量删除
来源：http://www.share.bbcook.cn/Article/details/glewbpmlh.sHtML

find . -name "*.tmp" -delete
来源：http://3g.sjlbkw.cn/Article/details/gullmbxkq.sHtML

[R46] 递归替换文件内容
来源：http://m.share.sjlbkw.cn/Article/details/grwekbaqu.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://m.share.fktsv.cn/Article/details/gpgssqnsp.sHtML

[R47] sed 单行替换
来源：http://blog.sjlbkw.cn/Article/details/gbrkeroik.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://blog.fktsv.cn/Article/details/gxpzxynmo.sHtML

[R48] awk 取指定列
来源：http://m.share.yfazqb.com/Article/details/glqlvkbjd.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.share.yfazqb.com/Article/details/gseoyxhld.sHtML

[R49] awk 带条件
来源：http://read.share.yfazqb.com/Article/details/gdtrrhoxl.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wap.yfazqb.com/Article/details/gxydqxhth.sHtML

[R50] awk 求和
来源：http://m.share.sjlbkw.cn/Article/details/gejndlxrc.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://blog.tarul.cn/Article/details/gncxoejwn.sHtML

[R51] 排序去重取前几
来源：http://blog.bbcook.cn/Article/details/gowvmjcji.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://mobile.vehdjk.com/Article/details/gmjjuvoox.sHtML

[R52] 统计行数
来源：http://www.m.share.vehdjk.com/Article/details/gypqlvfeg.sHtML

wc -l a.txt
来源：http://mobile.fktsv.cn/Article/details/glqpkqogc.sHtML

[R53] 查看文件头与实时尾
来源：http://mobile.yfazqb.com/Article/details/gldydngjp.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://mobile.tarul.cn/Article/details/gtyyqdgbn.sHtML

[R54] 比较两个文件
来源：http://read.share.bbcook.cn/Article/details/guyscqdjd.sHtML

diff a.txt b.txt
来源：http://www.m.share.bbcook.cn/Article/details/gtnlseoad.sHtML

[R55] 压缩与解压
来源：http://www.m.share.yfazqb.com/Article/details/glcwsgghq.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://blog.bbcook.cn/Article/details/gcyftuvtd.sHtML

[R56] 远程拷贝
来源：http://wap.bbcook.cn/Article/details/gajtplajj.sHtML

scp file user@host:/path/
来源：http://baike.epnwcf.com/Article/details/gdievtaht.sHtML

[R57] 远程执行命令
来源：http://www.blog.bbcook.cn/Article/details/ghypggksk.sHtML

ssh user@host 'uptime'
来源：http://mobile.fktsv.cn/Article/details/gbbvwpoci.sHtML

[R58] 下载文件
来源：http://read.share.sjlbkw.cn/Article/details/gfoalccfg.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://3g.epnwcf.com/Article/details/gjagucmvm.sHtML

[R59] 发 POST JSON
来源：http://m.share.epnwcf.com/Article/details/gdhvuobfs.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.blog.vehdjk.com/Article/details/gxinmopmv.sHtML

[R60] 只看 HTTP 状态码
来源：http://m.share.vehdjk.com/Article/details/gnobckuoc.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://3g.epnwcf.com/Article/details/gydedreny.sHtML

[R61] 磁盘占用
来源：http://www.share.yfazqb.com/Article/details/ggeckwprx.sHtML

df -h;  du -sh *
来源：http://m.share.yfazqb.com/Article/details/gohwpguhr.sHtML

[R62] 找最占空间的文件
来源：http://mobile.yfazqb.com/Article/details/grzsgwmzt.sHtML

du -ah . | sort -rh | head -10
来源：http://wap.yfazqb.com/Article/details/glnpbcdir.sHtML

[R63] 内存与进程
来源：http://www.share.tarul.cn/Article/details/gieyfwpwk.sHtML

free -h;  ps aux | grep nginx
来源：http://www.m.share.sjlbkw.cn/Article/details/geowfblbv.sHtML

[R64] 结束进程
来源：http://blog.tarul.cn/Article/details/gwnpquknp.sHtML

kill -9 $(pgrep -f app.py)
来源：http://3g.fktsv.cn/Article/details/gijaslvhp.sHtML

[R65] 查看端口占用
来源：http://3g.tarul.cn/Article/details/gkxlxynfe.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.m.share.fktsv.cn/Article/details/gcbclcqpa.sHtML

[R66] 定时任务
来源：http://baike.tarul.cn/Article/details/gruvjevkm.sHtML

crontab -e;  crontab -l
来源：http://www.blog.yfazqb.com/Article/details/gieqgbzys.sHtML

[R67] 生成随机十六进制串
来源：http://3g.bbcook.cn/Article/details/gwpohrhqb.sHtML

openssl rand -hex 16
来源：http://www.blog.sjlbkw.cn/Article/details/gnamkwvgk.sHtML

[R68] 计算文件校验值
来源：http://m.share.yfazqb.com/Article/details/giuvdrzid.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.blog.sjlbkw.cn/Article/details/gmojltegi.sHtML

[R69] 生成随机密码
来源：http://www.m.share.sjlbkw.cn/Article/details/gqpvslfam.sHtML

head -c 16 /dev/urandom | base64
来源：http://baike.vehdjk.com/Article/details/geqesiyqz.sHtML

[R70] 时间戳与互转
来源：http://www.blog.fktsv.cn/Article/details/gllipjaik.sHtML

date +%s;  date -d @1700000000
来源：http://www.share.bbcook.cn/Article/details/gpaalcawh.sHtML

[R71] 日期格式化
来源：http://www.blog.bbcook.cn/Article/details/gkjcrzphe.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://read.share.fktsv.cn/Article/details/gvamhnfto.sHtML

[R72] 等待端口就绪
来源：http://baike.tarul.cn/Article/details/gtgjakjsu.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://read.share.bbcook.cn/Article/details/gryudpuil.sHtML

[R73] 分割大日志
来源：http://wap.fktsv.cn/Article/details/glaoqkhub.sHtML

split -l 1000 big.log part_
来源：http://read.share.yfazqb.com/Article/details/gcjjnamxf.sHtML

[R74] 批量重命名
来源：http://m.share.yfazqb.com/Article/details/gsbjldnrg.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.share.vehdjk.com/Article/details/gpmjmywfh.sHtML

[R75] 导出环境变量
来源：http://mobile.yfazqb.com/Article/details/gdbsujwvx.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.share.yfazqb.com/Article/details/ghvgkyxsc.sHtML

[R76] 使用临时文件
来源：http://read.share.yfazqb.com/Article/details/gzbghlzks.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://blog.vehdjk.com/Article/details/grxfptgjf.sHtML

[R77] 读取用户输入
来源：http://www.m.share.yfazqb.com/Article/details/gyszxecvt.sHtML

read -rp "请输入: " ans
来源：http://www.m.share.fktsv.cn/Article/details/gvlmwowku.sHtML

[R78] 交互式菜单
来源：http://blog.vehdjk.com/Article/details/gudtndmpv.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://m.share.vehdjk.com/Article/details/gntixpvdy.sHtML

[R79] 解析命令行选项
来源：http://baike.bbcook.cn/Article/details/gleognkcf.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://read.share.vehdjk.com/Article/details/gasysznlf.sHtML

[R80] 查看脚本执行耗时
来源：http://wap.tarul.cn/Article/details/gzhpyotjn.sHtML

time ./run.sh
来源：http://baike.fktsv.cn/Article/details/ghibblrgf.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/gqrddrita.sHtML

S. C / C++ 专题
来源：http://3g.fktsv.cn/Article/details/gpbxzload.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/gfghjogdq.sHtML

[S01] C：Hello World
来源：http://read.share.vehdjk.com/Article/details/gmwcwhlcp.sHtML

#include <stdio.h>
来源：http://www.blog.sjlbkw.cn/Article/details/grhplfjea.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.share.bbcook.cn/Article/details/gihogssxm.sHtML

[S02] C：变量与格式化输出
来源：http://read.share.yfazqb.com/Article/details/gestzxhqo.sHtML

int a = 10; printf("%d\n", a);
来源：http://baike.tarul.cn/Article/details/grznvktyu.sHtML

[S03] C：读入整数
来源：http://wap.sjlbkw.cn/Article/details/gfxnkyjqj.sHtML

int x; scanf("%d", &x);
来源：http://mobile.vehdjk.com/Article/details/gwmolyfvc.sHtML

[S04] C：字符串复制
来源：http://blog.bbcook.cn/Article/details/gafkfguxk.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://m.share.vehdjk.com/Article/details/gtrymjhlo.sHtML

[S05] C：字符串长度
来源：http://baike.fktsv.cn/Article/details/ggltyckrq.sHtML

strlen(s)
来源：http://m.share.bbcook.cn/Article/details/gernqgodn.sHtML

[S06] C：字符串比较
来源：http://read.share.vehdjk.com/Article/details/gujpieddr.sHtML

strcmp(a, b) == 0
来源：http://blog.vehdjk.com/Article/details/gccyjzfaa.sHtML

[S07] C：数组遍历求和
来源：http://3g.epnwcf.com/Article/details/geyyloxfp.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://read.share.yfazqb.com/Article/details/gloskvjph.sHtML

[S08] C：动态内存分配与释放
来源：http://blog.fktsv.cn/Article/details/gpkyudvwo.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.blog.yfazqb.com/Article/details/gypstzhou.sHtML

[S09] C：结构体定义与初始化
来源：http://baike.yfazqb.com/Article/details/gczzjethk.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://m.share.fktsv.cn/Article/details/gieppqaom.sHtML

[S10] C：指针与解引用
来源：http://3g.fktsv.cn/Article/details/gyreaukor.sHtML

int *p = &a;  *p = 5;
来源：http://3g.vehdjk.com/Article/details/gkyghfdfq.sHtML

[S11] C：逐行读文件
来源：http://mobile.yfazqb.com/Article/details/gwhmdosqo.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://mobile.yfazqb.com/Article/details/gynpecwqk.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://mobile.tarul.cn/Article/details/gpjarbiyp.sHtML

fclose(f);
来源：http://www.blog.tarul.cn/Article/details/gfapzaevl.sHtML

[S12] C：写文件
来源：http://3g.yfazqb.com/Article/details/geeicwfzu.sHtML


<!-- 参考信息 -->