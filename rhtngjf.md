代发 wailian999

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.m.share.tarul.cn/Article/details/gitvobohq.sHtML

JOIN users u ON u.id = o.user_id
来源：http://blog.fktsv.cn/Article/details/gskgatyoc.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://m.share.tarul.cn/Article/details/glzldjuhp.sHtML

[Q42] 连接条件附加过滤
来源：http://baike.epnwcf.com/Article/details/gcfmeqzws.sHtML

SELECT u.name, o.amount FROM users u
来源：http://read.share.epnwcf.com/Article/details/gkufxplhx.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://read.share.bbcook.cn/Article/details/gsaanswqp.sHtML

[Q43] 标量子查询
来源：http://blog.bbcook.cn/Article/details/gpxtapvci.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.m.share.epnwcf.com/Article/details/gzwdelbyr.sHtML

[Q44] IN 子查询
来源：http://3g.bbcook.cn/Article/details/gcjzwnkqu.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.m.share.vehdjk.com/Article/details/gjmnwjjrd.sHtML

[Q45] EXISTS 判断存在
来源：http://www.share.yfazqb.com/Article/details/gxzdqoinz.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.fktsv.cn/Article/details/gbxwkydzo.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://blog.vehdjk.com/Article/details/gfnfrqpqz.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.tarul.cn/Article/details/gporctqir.sHtML

[Q47] 与平均值比较
来源：http://mobile.epnwcf.com/Article/details/gximarmkx.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://blog.yfazqb.com/Article/details/grlejexwx.sHtML

[Q48] CTE 公用表表达式
来源：http://mobile.yfazqb.com/Article/details/gfjaxmcxi.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://wap.bbcook.cn/Article/details/gkvmkeupz.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://wap.tarul.cn/Article/details/gjrwobblz.sHtML

[Q49] 更新单行
来源：http://m.share.sjlbkw.cn/Article/details/gmzttuloz.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.blog.sjlbkw.cn/Article/details/gampsnset.sHtML

[Q50] 批量更新
来源：http://blog.sjlbkw.cn/Article/details/gxueyotrr.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://3g.epnwcf.com/Article/details/gxhnribgi.sHtML

[Q51] 用子查询更新
来源：http://www.share.vehdjk.com/Article/details/gvafmubbi.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://baike.bbcook.cn/Article/details/gzajjeskj.sHtML

[Q52] 删除指定行
来源：http://mobile.epnwcf.com/Article/details/gqikbzapg.sHtML

DELETE FROM users WHERE id = 10;
来源：http://blog.yfazqb.com/Article/details/ghojholpy.sHtML

[Q53] 按条件删除
来源：http://m.share.sjlbkw.cn/Article/details/gqfxebuxp.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://m.share.fktsv.cn/Article/details/gyzlptyug.sHtML

[Q54] 清空表
来源：http://3g.tarul.cn/Article/details/gnqnzfuvv.sHtML

TRUNCATE TABLE logs;
来源：http://www.share.bbcook.cn/Article/details/gknpcxdzq.sHtML

[Q55] 排名（并列占位）
来源：http://wap.sjlbkw.cn/Article/details/girnkfgbi.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://baike.epnwcf.com/Article/details/gowaoxrai.sHtML

[Q56] 密集排名（并列不占位）
来源：http://mobile.sjlbkw.cn/Article/details/ggnktwwix.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.m.share.yfazqb.com/Article/details/gpfkdqoyk.sHtML

[Q57] 行号
来源：http://wap.epnwcf.com/Article/details/gtybiaxkx.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.blog.yfazqb.com/Article/details/gvaztucgd.sHtML

[Q58] 累计求和
来源：http://3g.fktsv.cn/Article/details/guxdrdnrp.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://baike.fktsv.cn/Article/details/glukwnzio.sHtML

[Q59] 分组内累计
来源：http://read.share.tarul.cn/Article/details/gcphzwjqe.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://read.share.sjlbkw.cn/Article/details/gdgllfjkz.sHtML

[Q60] 取上一行 / 下一行
来源：http://wap.sjlbkw.cn/Article/details/grffdikla.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://wap.yfazqb.com/Article/details/grmrlgfxa.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.share.sjlbkw.cn/Article/details/gghchjlii.sHtML

[Q61] 移动平均
来源：http://wap.tarul.cn/Article/details/gsvjiujsl.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://read.share.epnwcf.com/Article/details/gmnshpinh.sHtML

[Q62] 分组占比
来源：http://3g.epnwcf.com/Article/details/gqnytmrrv.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://blog.vehdjk.com/Article/details/gtltemvxq.sHtML

[Q63] 开启事务
来源：http://m.share.vehdjk.com/Article/details/guhviebkl.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.m.share.sjlbkw.cn/Article/details/gehlngiae.sHtML

[Q64] 提交事务
来源：http://read.share.vehdjk.com/Article/details/gfckkadjs.sHtML

COMMIT;
来源：http://m.share.sjlbkw.cn/Article/details/gajiysrzj.sHtML

[Q65] 回滚事务
来源：http://read.share.sjlbkw.cn/Article/details/giblssmiv.sHtML

ROLLBACK;
来源：http://m.share.bbcook.cn/Article/details/ghgopswqm.sHtML

[Q66] 行锁查询
来源：http://m.share.epnwcf.com/Article/details/gewvpgffd.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://m.share.tarul.cn/Article/details/gcluuigvt.sHtML

[Q67] 设置隔离级别
来源：http://baike.vehdjk.com/Article/details/gkrkjvfbj.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://blog.bbcook.cn/Article/details/gjxfdnjom.sHtML

[Q68] 保存点
来源：http://m.share.tarul.cn/Article/details/gptoucoqb.sHtML

SAVEPOINT sp1;
来源：http://read.share.bbcook.cn/Article/details/gwrziomfi.sHtML

ROLLBACK TO sp1;
来源：http://wap.tarul.cn/Article/details/gtxumweqj.sHtML

[Q69] 查看执行计划
来源：http://baike.sjlbkw.cn/Article/details/gfvsrocxy.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.blog.yfazqb.com/Article/details/gvrbcyyfh.sHtML

[Q70] 更新统计信息
来源：http://blog.bbcook.cn/Article/details/gllxmlbrt.sHtML

ANALYZE TABLE users;
来源：http://www.blog.yfazqb.com/Article/details/glyhmzega.sHtML

[Q71] 查看建表语句
来源：http://www.blog.sjlbkw.cn/Article/details/gkcsyknhe.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://m.share.epnwcf.com/Article/details/gqieuoxcy.sHtML

[Q72] 查看索引
来源：http://wap.bbcook.cn/Article/details/gbylberxd.sHtML

SHOW INDEX FROM users;
来源：http://baike.tarul.cn/Article/details/guvdhfxau.sHtML

[Q73] 查看表状态
来源：http://blog.bbcook.cn/Article/details/gwspungdt.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://wap.vehdjk.com/Article/details/gpamwjzaa.sHtML

[Q74] 强制使用索引
来源：http://www.m.share.vehdjk.com/Article/details/gqgafoctd.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://3g.yfazqb.com/Article/details/gxciejeiv.sHtML

[Q75] 日期格式化
来源：http://www.blog.sjlbkw.cn/Article/details/gyqvytqhd.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.blog.sjlbkw.cn/Article/details/grckufcdz.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.blog.bbcook.cn/Article/details/ghbuiuryi.sHtML

[Q76] 按天统计
来源：http://read.share.epnwcf.com/Article/details/gatyjclpt.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://baike.tarul.cn/Article/details/grlolgpnx.sHtML

[Q77] 时间加减
来源：http://m.share.bbcook.cn/Article/details/gmykyzelg.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.blog.tarul.cn/Article/details/gwakpgpmz.sHtML

[Q78] 当前时间
来源：http://www.blog.sjlbkw.cn/Article/details/gqejqqzsl.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://mobile.fktsv.cn/Article/details/gybnpxdip.sHtML

[Q79] 字符串拼接
来源：http://blog.vehdjk.com/Article/details/gvfjhdhqp.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.blog.vehdjk.com/Article/details/gazvnlfcr.sHtML

[Q80] 字符串截取
来源：http://wap.yfazqb.com/Article/details/gajvgzjct.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://m.share.tarul.cn/Article/details/ggmxvuycs.sHtML

[Q81] 字符串替换
来源：http://blog.vehdjk.com/Article/details/grtldfmse.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://3g.epnwcf.com/Article/details/gyvzaxofn.sHtML

[Q82] 字符长度与字节长度
来源：http://blog.bbcook.cn/Article/details/gvhzxspqo.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.blog.fktsv.cn/Article/details/gomgdwmhp.sHtML

[Q83] 大小写转换
来源：http://read.share.yfazqb.com/Article/details/goibjygfl.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.m.share.fktsv.cn/Article/details/gxisuzvoc.sHtML

[Q84] 去除首尾空格
来源：http://www.m.share.fktsv.cn/Article/details/gttfjkjey.sHtML

SELECT TRIM(name) FROM users;
来源：http://3g.epnwcf.com/Article/details/gesbqunla.sHtML

[Q85] 数值取整
来源：http://blog.sjlbkw.cn/Article/details/gdpglgnun.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.m.share.epnwcf.com/Article/details/ggnqqytxc.sHtML

[Q86] 读取 JSON 字段
来源：http://baike.sjlbkw.cn/Article/details/gdzrgovrz.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://wap.vehdjk.com/Article/details/gzqjmrapi.sHtML

[Q87] JSON 字段做条件
来源：http://www.blog.tarul.cn/Article/details/gtbzxsvqx.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://mobile.sjlbkw.cn/Article/details/gjqyitbma.sHtML

[Q88] 行转列（条件聚合）
来源：http://wap.epnwcf.com/Article/details/gwxhivssg.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://mobile.yfazqb.com/Article/details/ggztddvwq.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.share.fktsv.cn/Article/details/gakpjdwmz.sHtML

[Q89] 判断表是否存在
来源：http://www.m.share.bbcook.cn/Article/details/gjfpyupia.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.share.vehdjk.com/Article/details/garxwjstm.sHtML

[Q90] 生成序号列
来源：http://read.share.yfazqb.com/Article/details/gwzuajepx.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://mobile.sjlbkw.cn/Article/details/gijidburb.sHtML

================================================================================
来源：http://m.share.tarul.cn/Article/details/ghluebbqp.sHtML

R. Bash 专题
来源：http://read.share.tarul.cn/Article/details/gmokjmvhz.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/grsgpblbp.sHtML

[R01] shebang 与严格模式
来源：http://mobile.yfazqb.com/Article/details/gdikyecyd.sHtML

#!/usr/bin/env bash
来源：http://mobile.epnwcf.com/Article/details/gthdulonx.sHtML

set -euo pipefail
来源：http://baike.yfazqb.com/Article/details/gunsywkuf.sHtML

[R02] 变量赋值与使用
来源：http://m.share.tarul.cn/Article/details/gldcujaeo.sHtML

name="Tom"; echo "$name"
来源：http://www.m.share.sjlbkw.cn/Article/details/ggbnkkpwa.sHtML

[R03] 只读变量
来源：http://blog.fktsv.cn/Article/details/gmqaufxmg.sHtML

readonly PI=3.14
来源：http://blog.fktsv.cn/Article/details/gurjwqdkm.sHtML

[R04] 位置参数
来源：http://www.share.epnwcf.com/Article/details/gbnhgstfm.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://read.share.vehdjk.com/Article/details/gmzgmibwo.sHtML

[R05] 参数默认值
来源：http://m.share.sjlbkw.cn/Article/details/ggabgjfdd.sHtML

name="${1:-default}"
来源：http://www.m.share.tarul.cn/Article/details/ghzkrtfcb.sHtML

[R06] 判断命令是否存在
来源：http://baike.fktsv.cn/Article/details/gbkpinhhb.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://blog.tarul.cn/Article/details/guulgscjc.sHtML

[R07] if 判断文件
来源：http://blog.fktsv.cn/Article/details/gadsqauvi.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://mobile.fktsv.cn/Article/details/ghtgmevfz.sHtML

[R08] 数值比较
来源：http://www.blog.epnwcf.com/Article/details/gxrrfeskv.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://baike.yfazqb.com/Article/details/gjmtexuau.sHtML

[R09] 字符串比较
来源：http://3g.tarul.cn/Article/details/ghorlmekr.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://read.share.yfazqb.com/Article/details/gksfaqngp.sHtML

[R10] 正则匹配
来源：http://www.share.tarul.cn/Article/details/gsstbnafu.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://3g.sjlbkw.cn/Article/details/gfppsoqab.sHtML

[R11] case 多分支
来源：http://m.share.sjlbkw.cn/Article/details/grsjframj.sHtML

case "$1" in
来源：http://mobile.bbcook.cn/Article/details/gngbwgsxl.sHtML

start) echo "启动" ;;
来源：http://blog.epnwcf.com/Article/details/gsjzgnirk.sHtML

stop)  echo "停止" ;;
来源：http://blog.tarul.cn/Article/details/ghisuleln.sHtML

*)     echo "未知命令" ;;
来源：http://baike.epnwcf.com/Article/details/goqnqckod.sHtML

esac
来源：http://mobile.epnwcf.com/Article/details/ggywhatue.sHtML

[R12] for 遍历文件
来源：http://www.share.tarul.cn/Article/details/gidkqdjps.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.blog.bbcook.cn/Article/details/gaemuubcu.sHtML

[R13] for 计数循环
来源：http://m.share.yfazqb.com/Article/details/gizcesmee.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://wap.sjlbkw.cn/Article/details/ggdhzuuee.sHtML

[R14] C 风格 for
来源：http://www.m.share.epnwcf.com/Article/details/grvrosmkj.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.share.bbcook.cn/Article/details/glipksmlp.sHtML

[R15] while 逐行读文件
来源：http://baike.bbcook.cn/Article/details/gphzryjum.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://read.share.fktsv.cn/Article/details/govcqbxjw.sHtML

[R16] until 等待条件
来源：http://wap.sjlbkw.cn/Article/details/gjggzmnsw.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://m.share.yfazqb.com/Article/details/gqzmvirsm.sHtML

[R17] 数组定义与取值
来源：http://baike.vehdjk.com/Article/details/ggkiydtog.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://baike.bbcook.cn/Article/details/gjiwigvfu.sHtML

[R18] 遍历数组
来源：http://wap.sjlbkw.cn/Article/details/grsjyxdoy.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://m.share.fktsv.cn/Article/details/gyqibjdsx.sHtML

[R19] 数组长度
来源：http://3g.fktsv.cn/Article/details/gaojlmfxq.sHtML

echo "${#arr[@]}"
来源：http://read.share.epnwcf.com/Article/details/gebbubjxp.sHtML

[R20] 关联数组（字典）
来源：http://blog.bbcook.cn/Article/details/gupzxijrz.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://m.share.fktsv.cn/Article/details/ggjzbswek.sHtML

[R21] 字符串长度
来源：http://blog.epnwcf.com/Article/details/glljexvmt.sHtML

echo "${#s}"
来源：http://read.share.bbcook.cn/Article/details/gzdyjbtsy.sHtML

[R22] 截取子串
来源：http://www.share.yfazqb.com/Article/details/grumgxpry.sHtML

echo "${s:0:5}"
来源：http://www.blog.yfazqb.com/Article/details/gvzrwnvpt.sHtML

[R23] 字符串替换
来源：http://www.m.share.sjlbkw.cn/Article/details/gbkxwdwde.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://read.share.tarul.cn/Article/details/gjdlrjqrn.sHtML

[R24] 大小写转换
来源：http://baike.vehdjk.com/Article/details/gtxyskqdk.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://wap.vehdjk.com/Article/details/gammvameb.sHtML

[R25] 去后缀 / 去前缀
来源：http://blog.epnwcf.com/Article/details/gilxwcqep.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://m.share.sjlbkw.cn/Article/details/gxvcdjphp.sHtML

[R26] 命令替换
来源：http://3g.yfazqb.com/Article/details/gnyonmjcz.sHtML

now=$(date +%F); echo "$now"
来源：http://www.share.tarul.cn/Article/details/gzpewpevb.sHtML

[R27] 算术展开
来源：http://wap.vehdjk.com/Article/details/gnvjloduo.sHtML

echo $((1 + 2 * 3))
来源：http://mobile.vehdjk.com/Article/details/gojsxugbw.sHtML

[R28] 浮点运算
来源：http://mobile.yfazqb.com/Article/details/gozydxibf.sHtML

echo "scale=2; 10/3" | bc
来源：http://mobile.bbcook.cn/Article/details/giwmwazog.sHtML

[R29] 定义函数
来源：http://www.m.share.epnwcf.com/Article/details/gfqygyxlb.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.share.epnwcf.com/Article/details/gqzxtqkvn.sHtML

[R30] 函数返回状态码
来源：http://m.share.fktsv.cn/Article/details/gqqdtaepj.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://baike.sjlbkw.cn/Article/details/gtepovhoy.sHtML

[R31] 局部变量
来源：http://read.share.sjlbkw.cn/Article/details/gboeidovi.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gphrlmqns.sHtML

[R32] 参数个数校验
来源：http://m.share.yfazqb.com/Article/details/glayhbkca.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://blog.sjlbkw.cn/Article/details/gdwubvaas.sHtML

[R33] 捕获错误并提示行号
来源：http://www.blog.epnwcf.com/Article/details/gkxtkubwd.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://m.share.sjlbkw.cn/Article/details/gnjprrcaq.sHtML

[R34] 退出时清理
来源：http://m.share.bbcook.cn/Article/details/gthfqqqqr.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://3g.vehdjk.com/Article/details/gcudhbaat.sHtML

[R35] 后台执行并等待
来源：http://wap.fktsv.cn/Article/details/gxbcvnttc.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.m.share.vehdjk.com/Article/details/gdlxobfmr.sHtML

[R36] 并发执行多个任务
来源：http://mobile.tarul.cn/Article/details/gvviaikkc.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.m.share.epnwcf.com/Article/details/gyorelvii.sHtML

[R37] 把输出赋给变量
来源：http://m.share.sjlbkw.cn/Article/details/gqsmwebyp.sHtML

files=$(ls -1)
来源：http://3g.vehdjk.com/Article/details/gpceiyazg.sHtML

[R38] 管道串联
来源：http://baike.tarul.cn/Article/details/geywfrhxd.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.share.yfazqb.com/Article/details/gmpbfdjvr.sHtML

[R39] 重定向标准输出与错误
来源：http://read.share.sjlbkw.cn/Article/details/gydvcavkx.sHtML

cmd > out.log 2>&1
来源：http://read.share.epnwcf.com/Article/details/gxngornoy.sHtML

[R40] 追加写日志
来源：http://3g.epnwcf.com/Article/details/ggbihmani.sHtML

echo "log" >> out.log
来源：http://m.share.tarul.cn/Article/details/grqlprcqg.sHtML

[R41] 丢弃输出
来源：http://baike.sjlbkw.cn/Article/details/gglrzkhqx.sHtML

cmd >/dev/null 2>&1
来源：http://baike.bbcook.cn/Article/details/gjuffvzgo.sHtML

[R42] 输入重定向
来源：http://blog.bbcook.cn/Article/details/gfpgdethy.sHtML

wc -l < a.txt
来源：http://m.share.sjlbkw.cn/Article/details/gjtiugpmo.sHtML

[R43] 按名字查找文件
来源：http://www.share.bbcook.cn/Article/details/gcrkevfon.sHtML

find . -name "*.log" -type f
来源：http://wap.fktsv.cn/Article/details/glvgfrmkr.sHtML

[R44] 按修改时间查找
来源：http://blog.bbcook.cn/Article/details/geyddjxyg.sHtML

find . -mtime -7 -type f
来源：http://3g.bbcook.cn/Article/details/gkuxkscej.sHtML

[R45] 批量删除
来源：http://3g.tarul.cn/Article/details/glpfogsem.sHtML

find . -name "*.tmp" -delete
来源：http://3g.vehdjk.com/Article/details/gzvmnxhcl.sHtML

[R46] 递归替换文件内容
来源：http://wap.epnwcf.com/Article/details/gfcddcqzs.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://m.share.sjlbkw.cn/Article/details/gsbedeyqm.sHtML

[R47] sed 单行替换
来源：http://www.blog.fktsv.cn/Article/details/gntpgynzu.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.m.share.sjlbkw.cn/Article/details/gjqhrkfnz.sHtML

[R48] awk 取指定列
来源：http://m.share.bbcook.cn/Article/details/gjunztjxp.sHtML

awk '{print $1, $3}' a.txt
来源：http://baike.yfazqb.com/Article/details/giyjtruem.sHtML

[R49] awk 带条件
来源：http://www.blog.bbcook.cn/Article/details/gkhezhvdg.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://blog.yfazqb.com/Article/details/gzptayqfw.sHtML

[R50] awk 求和
来源：http://www.m.share.sjlbkw.cn/Article/details/grgaagzby.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.share.sjlbkw.cn/Article/details/gzrgsbviq.sHtML

[R51] 排序去重取前几
来源：http://blog.bbcook.cn/Article/details/ggmmruera.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://wap.vehdjk.com/Article/details/gdswlllbx.sHtML

[R52] 统计行数
来源：http://wap.tarul.cn/Article/details/giqnmdwns.sHtML

wc -l a.txt
来源：http://www.blog.sjlbkw.cn/Article/details/gxgfdwnto.sHtML

[R53] 查看文件头与实时尾
来源：http://wap.fktsv.cn/Article/details/ghlytsbrc.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://wap.yfazqb.com/Article/details/gistywrwo.sHtML

[R54] 比较两个文件
来源：http://baike.epnwcf.com/Article/details/gkbosvlpa.sHtML

diff a.txt b.txt
来源：http://blog.fktsv.cn/Article/details/gkhkicuzz.sHtML

[R55] 压缩与解压
来源：http://blog.tarul.cn/Article/details/gwukyjcfh.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://blog.tarul.cn/Article/details/gdrblstfe.sHtML

[R56] 远程拷贝
来源：http://mobile.fktsv.cn/Article/details/gvojckavx.sHtML

scp file user@host:/path/
来源：http://3g.epnwcf.com/Article/details/guzcifaqk.sHtML

[R57] 远程执行命令
来源：http://blog.bbcook.cn/Article/details/guorasbpa.sHtML

ssh user@host 'uptime'
来源：http://www.m.share.fktsv.cn/Article/details/gfdqztqay.sHtML

[R58] 下载文件
来源：http://baike.yfazqb.com/Article/details/gafozddmf.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://blog.bbcook.cn/Article/details/gsapcylzm.sHtML

[R59] 发 POST JSON
来源：http://read.share.fktsv.cn/Article/details/gqhfmnyfd.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.blog.fktsv.cn/Article/details/gegdigzri.sHtML

[R60] 只看 HTTP 状态码
来源：http://wap.vehdjk.com/Article/details/gegvfkjvz.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://wap.fktsv.cn/Article/details/gdgrlrnim.sHtML

[R61] 磁盘占用
来源：http://m.share.vehdjk.com/Article/details/giyyfuluy.sHtML

df -h;  du -sh *
来源：http://blog.vehdjk.com/Article/details/gzhuazxnm.sHtML

[R62] 找最占空间的文件
来源：http://www.share.fktsv.cn/Article/details/gnbjookuy.sHtML

du -ah . | sort -rh | head -10
来源：http://blog.bbcook.cn/Article/details/guopaoqqk.sHtML

[R63] 内存与进程
来源：http://read.share.tarul.cn/Article/details/gdmgvmgqb.sHtML

free -h;  ps aux | grep nginx
来源：http://blog.sjlbkw.cn/Article/details/gpwltezdc.sHtML

[R64] 结束进程
来源：http://3g.epnwcf.com/Article/details/gigrzddrm.sHtML

kill -9 $(pgrep -f app.py)
来源：http://baike.yfazqb.com/Article/details/gomilgyzt.sHtML

[R65] 查看端口占用
来源：http://mobile.bbcook.cn/Article/details/gnlmpkcpv.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wap.fktsv.cn/Article/details/gbljnorhm.sHtML

[R66] 定时任务
来源：http://www.share.vehdjk.com/Article/details/ghjnspbno.sHtML

crontab -e;  crontab -l
来源：http://m.share.yfazqb.com/Article/details/gzmkedhyq.sHtML

[R67] 生成随机十六进制串
来源：http://www.blog.sjlbkw.cn/Article/details/grnuuukst.sHtML

openssl rand -hex 16
来源：http://mobile.fktsv.cn/Article/details/ggiqnbdfq.sHtML

[R68] 计算文件校验值
来源：http://www.m.share.epnwcf.com/Article/details/gxlzjzmvj.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://3g.fktsv.cn/Article/details/grbpypsbl.sHtML

[R69] 生成随机密码
来源：http://3g.bbcook.cn/Article/details/gtotyjuea.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.m.share.vehdjk.com/Article/details/glmvqyfhs.sHtML

[R70] 时间戳与互转
来源：http://www.share.fktsv.cn/Article/details/gquaybzjt.sHtML

date +%s;  date -d @1700000000
来源：http://www.share.yfazqb.com/Article/details/ggtkkvdef.sHtML

[R71] 日期格式化
来源：http://read.share.bbcook.cn/Article/details/gsvkyylht.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://m.share.yfazqb.com/Article/details/grxkdpxxf.sHtML

[R72] 等待端口就绪
来源：http://read.share.epnwcf.com/Article/details/gjalukjma.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://wap.epnwcf.com/Article/details/gsbubdyfx.sHtML

[R73] 分割大日志
来源：http://blog.bbcook.cn/Article/details/gheuqatez.sHtML

split -l 1000 big.log part_
来源：http://3g.yfazqb.com/Article/details/gyjymfpmt.sHtML

[R74] 批量重命名
来源：http://mobile.bbcook.cn/Article/details/glhyxfyxt.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://baike.epnwcf.com/Article/details/gzanhomwm.sHtML

[R75] 导出环境变量
来源：http://wap.yfazqb.com/Article/details/gqzbpqrtz.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://baike.epnwcf.com/Article/details/gaykcvlgr.sHtML

[R76] 使用临时文件
来源：http://www.blog.tarul.cn/Article/details/gxtakitpu.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://baike.fktsv.cn/Article/details/guvrfffjn.sHtML

[R77] 读取用户输入
来源：http://read.share.fktsv.cn/Article/details/gwbkvgmov.sHtML

read -rp "请输入: " ans
来源：http://wap.tarul.cn/Article/details/gjadnhwue.sHtML

[R78] 交互式菜单
来源：http://baike.sjlbkw.cn/Article/details/gjcxqlhuo.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://baike.fktsv.cn/Article/details/gjnbwgjzi.sHtML

[R79] 解析命令行选项
来源：http://mobile.vehdjk.com/Article/details/grlauipeh.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mobile.vehdjk.com/Article/details/gthwdsqsv.sHtML

[R80] 查看脚本执行耗时
来源：http://m.share.yfazqb.com/Article/details/gqdmufmeh.sHtML

time ./run.sh
来源：http://wap.fktsv.cn/Article/details/gnwrghokl.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/gwtwznrvx.sHtML

S. C / C++ 专题
来源：http://www.blog.yfazqb.com/Article/details/gvdrmrivw.sHtML

================================================================================
来源：http://baike.sjlbkw.cn/Article/details/gzvknrxtc.sHtML

[S01] C：Hello World
来源：http://baike.tarul.cn/Article/details/giygxzslf.sHtML

#include <stdio.h>
来源：http://www.blog.yfazqb.com/Article/details/gmuewveru.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://m.share.epnwcf.com/Article/details/geohjvgak.sHtML

[S02] C：变量与格式化输出
来源：http://m.share.fktsv.cn/Article/details/gmtmtgebl.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.m.share.epnwcf.com/Article/details/gxweajnix.sHtML

[S03] C：读入整数
来源：http://blog.tarul.cn/Article/details/gvdyidfgo.sHtML

int x; scanf("%d", &x);
来源：http://mobile.sjlbkw.cn/Article/details/gbehovxhk.sHtML

[S04] C：字符串复制
来源：http://m.share.vehdjk.com/Article/details/ggtuoquuj.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://m.share.yfazqb.com/Article/details/ghszqclop.sHtML

[S05] C：字符串长度
来源：http://m.share.vehdjk.com/Article/details/gwagznmkq.sHtML

strlen(s)
来源：http://blog.epnwcf.com/Article/details/gnabpurvx.sHtML

[S06] C：字符串比较
来源：http://read.share.tarul.cn/Article/details/gkkbsgrrs.sHtML

strcmp(a, b) == 0
来源：http://wap.bbcook.cn/Article/details/gaxsvxfsv.sHtML

[S07] C：数组遍历求和
来源：http://3g.epnwcf.com/Article/details/gnmhujhlj.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://read.share.vehdjk.com/Article/details/gvjivyafr.sHtML

[S08] C：动态内存分配与释放
来源：http://3g.sjlbkw.cn/Article/details/gqcdzljbw.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://wap.sjlbkw.cn/Article/details/giumduycw.sHtML

[S09] C：结构体定义与初始化
来源：http://read.share.yfazqb.com/Article/details/gxwideclx.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://m.share.fktsv.cn/Article/details/glhqiquao.sHtML

[S10] C：指针与解引用
来源：http://blog.vehdjk.com/Article/details/gsoasvyov.sHtML

int *p = &a;  *p = 5;
来源：http://blog.sjlbkw.cn/Article/details/gwcdpootu.sHtML

[S11] C：逐行读文件
来源：http://m.share.yfazqb.com/Article/details/gzssmbxtz.sHtML


<!-- 参考信息 -->