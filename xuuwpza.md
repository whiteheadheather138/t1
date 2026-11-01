代发 wailian999

SELECT o.id, u.name, p.title FROM orders o
来源：http://wap.tarul.cn/Article/details/gijuosklp.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.blog.sjlbkw.cn/Article/details/gmrcbvarg.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://read.share.tarul.cn/Article/details/gnilbsqtx.sHtML

[Q42] 连接条件附加过滤
来源：http://read.share.vehdjk.com/Article/details/gdvgiwwox.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.m.share.yfazqb.com/Article/details/gmchqrssc.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://3g.sjlbkw.cn/Article/details/gofjzekfp.sHtML

[Q43] 标量子查询
来源：http://baike.vehdjk.com/Article/details/grypmvonz.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://baike.tarul.cn/Article/details/gzacnjdbf.sHtML

[Q44] IN 子查询
来源：http://www.blog.sjlbkw.cn/Article/details/gcetyiguk.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://baike.vehdjk.com/Article/details/gkbfyubyr.sHtML

[Q45] EXISTS 判断存在
来源：http://m.share.yfazqb.com/Article/details/grytongob.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.vehdjk.com/Article/details/gppiopatr.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://baike.bbcook.cn/Article/details/germnuqek.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.yfazqb.com/Article/details/gfntplpcc.sHtML

[Q47] 与平均值比较
来源：http://baike.sjlbkw.cn/Article/details/gfihfpdro.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://wap.epnwcf.com/Article/details/gqaaybmcy.sHtML

[Q48] CTE 公用表表达式
来源：http://www.m.share.tarul.cn/Article/details/gmwblaehs.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.m.share.sjlbkw.cn/Article/details/gaqimmeno.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://baike.bbcook.cn/Article/details/gdotbmfmn.sHtML

[Q49] 更新单行
来源：http://baike.vehdjk.com/Article/details/gaqglplys.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://baike.yfazqb.com/Article/details/gkccknxjo.sHtML

[Q50] 批量更新
来源：http://www.share.fktsv.cn/Article/details/gnpmevulq.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.share.epnwcf.com/Article/details/gzhcpqoxx.sHtML

[Q51] 用子查询更新
来源：http://wap.vehdjk.com/Article/details/gtayykofx.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://read.share.epnwcf.com/Article/details/gzdfebtjq.sHtML

[Q52] 删除指定行
来源：http://mobile.bbcook.cn/Article/details/gsoswrrig.sHtML

DELETE FROM users WHERE id = 10;
来源：http://wap.epnwcf.com/Article/details/gfhnhkgrw.sHtML

[Q53] 按条件删除
来源：http://www.m.share.fktsv.cn/Article/details/gaextozyx.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.share.tarul.cn/Article/details/gaiarkutk.sHtML

[Q54] 清空表
来源：http://www.m.share.yfazqb.com/Article/details/gerqmogan.sHtML

TRUNCATE TABLE logs;
来源：http://mobile.vehdjk.com/Article/details/gdtzxjrrn.sHtML

[Q55] 排名（并列占位）
来源：http://www.share.fktsv.cn/Article/details/ghbwwepou.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://read.share.tarul.cn/Article/details/gylvmnssd.sHtML

[Q56] 密集排名（并列不占位）
来源：http://wap.tarul.cn/Article/details/gotmkbcie.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.m.share.bbcook.cn/Article/details/gfzmgxntf.sHtML

[Q57] 行号
来源：http://read.share.epnwcf.com/Article/details/glknnuaul.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.blog.vehdjk.com/Article/details/galwzbtfx.sHtML

[Q58] 累计求和
来源：http://www.m.share.fktsv.cn/Article/details/gnumyadps.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://3g.epnwcf.com/Article/details/gjasatzqm.sHtML

[Q59] 分组内累计
来源：http://www.blog.fktsv.cn/Article/details/gmbthgyft.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.m.share.tarul.cn/Article/details/grshqscbz.sHtML

[Q60] 取上一行 / 下一行
来源：http://3g.tarul.cn/Article/details/gjxtevfag.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://blog.fktsv.cn/Article/details/gbrmboqmn.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://3g.epnwcf.com/Article/details/gfmisxgby.sHtML

[Q61] 移动平均
来源：http://3g.vehdjk.com/Article/details/gtzpdkjhb.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://m.share.vehdjk.com/Article/details/gryhwrcpv.sHtML

[Q62] 分组占比
来源：http://www.share.bbcook.cn/Article/details/gqmfzplov.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://3g.yfazqb.com/Article/details/gjubcsvvn.sHtML

[Q63] 开启事务
来源：http://www.blog.yfazqb.com/Article/details/gqbgdykmb.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.blog.vehdjk.com/Article/details/gzdbjeqlx.sHtML

[Q64] 提交事务
来源：http://m.share.sjlbkw.cn/Article/details/glfnwjzma.sHtML

COMMIT;
来源：http://blog.yfazqb.com/Article/details/gckfepvgq.sHtML

[Q65] 回滚事务
来源：http://baike.tarul.cn/Article/details/gqawzkium.sHtML

ROLLBACK;
来源：http://www.m.share.yfazqb.com/Article/details/gmhdsmuya.sHtML

[Q66] 行锁查询
来源：http://m.share.epnwcf.com/Article/details/gdxpgrnww.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://baike.tarul.cn/Article/details/gzgdjktrl.sHtML

[Q67] 设置隔离级别
来源：http://blog.vehdjk.com/Article/details/gtlxfzsfp.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://wap.tarul.cn/Article/details/gmuuxnxhi.sHtML

[Q68] 保存点
来源：http://read.share.yfazqb.com/Article/details/ggilmoitf.sHtML

SAVEPOINT sp1;
来源：http://wap.tarul.cn/Article/details/grmkkdawz.sHtML

ROLLBACK TO sp1;
来源：http://read.share.bbcook.cn/Article/details/gxkfcjxoh.sHtML

[Q69] 查看执行计划
来源：http://mobile.epnwcf.com/Article/details/gfcffogip.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.m.share.fktsv.cn/Article/details/geizuvqlc.sHtML

[Q70] 更新统计信息
来源：http://wap.tarul.cn/Article/details/gdsyphfmd.sHtML

ANALYZE TABLE users;
来源：http://3g.sjlbkw.cn/Article/details/ggxqdbotj.sHtML

[Q71] 查看建表语句
来源：http://read.share.bbcook.cn/Article/details/gqixixiqj.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://baike.fktsv.cn/Article/details/giyzwyuit.sHtML

[Q72] 查看索引
来源：http://mobile.epnwcf.com/Article/details/guaafpzuw.sHtML

SHOW INDEX FROM users;
来源：http://baike.tarul.cn/Article/details/gjliiewvd.sHtML

[Q73] 查看表状态
来源：http://www.share.bbcook.cn/Article/details/gboxtwjut.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.share.epnwcf.com/Article/details/gevrojmxq.sHtML

[Q74] 强制使用索引
来源：http://wap.epnwcf.com/Article/details/gkcrofsaf.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://3g.sjlbkw.cn/Article/details/gouidujho.sHtML

[Q75] 日期格式化
来源：http://www.share.sjlbkw.cn/Article/details/gbrusjsge.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://3g.tarul.cn/Article/details/gtvplcpvf.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.share.sjlbkw.cn/Article/details/ghciwmkmr.sHtML

[Q76] 按天统计
来源：http://www.m.share.yfazqb.com/Article/details/geekvjjvg.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://read.share.sjlbkw.cn/Article/details/ggfxqksng.sHtML

[Q77] 时间加减
来源：http://mobile.sjlbkw.cn/Article/details/glqmmapeb.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://read.share.vehdjk.com/Article/details/gjfyqqaic.sHtML

[Q78] 当前时间
来源：http://wap.fktsv.cn/Article/details/ggzpunbbe.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://m.share.tarul.cn/Article/details/gxagiyynp.sHtML

[Q79] 字符串拼接
来源：http://m.share.sjlbkw.cn/Article/details/gujiluxzp.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://read.share.bbcook.cn/Article/details/gzjhiozxd.sHtML

[Q80] 字符串截取
来源：http://read.share.fktsv.cn/Article/details/grueqfzbg.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.share.fktsv.cn/Article/details/gcbggjwku.sHtML

[Q81] 字符串替换
来源：http://www.m.share.sjlbkw.cn/Article/details/gfzxirfqo.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://mobile.epnwcf.com/Article/details/garwttban.sHtML

[Q82] 字符长度与字节长度
来源：http://www.m.share.sjlbkw.cn/Article/details/gfmraotwj.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://mobile.sjlbkw.cn/Article/details/gypcrzkqh.sHtML

[Q83] 大小写转换
来源：http://baike.fktsv.cn/Article/details/groxjljws.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.m.share.yfazqb.com/Article/details/gqkbifoiv.sHtML

[Q84] 去除首尾空格
来源：http://3g.tarul.cn/Article/details/gxtnakgab.sHtML

SELECT TRIM(name) FROM users;
来源：http://3g.vehdjk.com/Article/details/ggxrbruiv.sHtML

[Q85] 数值取整
来源：http://www.share.fktsv.cn/Article/details/gogsqonij.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.blog.tarul.cn/Article/details/gwhcoyemz.sHtML

[Q86] 读取 JSON 字段
来源：http://baike.vehdjk.com/Article/details/gnfbjwbrf.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://3g.yfazqb.com/Article/details/gniesbulo.sHtML

[Q87] JSON 字段做条件
来源：http://3g.vehdjk.com/Article/details/gvgbqujeu.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://mobile.vehdjk.com/Article/details/gjdzfoafr.sHtML

[Q88] 行转列（条件聚合）
来源：http://read.share.tarul.cn/Article/details/gsgjusnek.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://wap.yfazqb.com/Article/details/gjnpnwtjk.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://3g.vehdjk.com/Article/details/gbxgrivbw.sHtML

[Q89] 判断表是否存在
来源：http://mobile.yfazqb.com/Article/details/gvuimjpqy.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://baike.vehdjk.com/Article/details/ggzekkbbb.sHtML

[Q90] 生成序号列
来源：http://read.share.fktsv.cn/Article/details/gwamjmfir.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://m.share.bbcook.cn/Article/details/gxabwqkah.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/gremqmavk.sHtML

R. Bash 专题
来源：http://mobile.bbcook.cn/Article/details/glfrzepwv.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/gtfmaynii.sHtML

[R01] shebang 与严格模式
来源：http://www.share.fktsv.cn/Article/details/gnwszccjq.sHtML

#!/usr/bin/env bash
来源：http://www.share.sjlbkw.cn/Article/details/gcmgwfweb.sHtML

set -euo pipefail
来源：http://wap.fktsv.cn/Article/details/gmpnxqeny.sHtML

[R02] 变量赋值与使用
来源：http://mobile.epnwcf.com/Article/details/gywzkzqab.sHtML

name="Tom"; echo "$name"
来源：http://m.share.fktsv.cn/Article/details/gltzbhywm.sHtML

[R03] 只读变量
来源：http://www.blog.epnwcf.com/Article/details/gwpaoogti.sHtML

readonly PI=3.14
来源：http://baike.yfazqb.com/Article/details/gtxbzpkxi.sHtML

[R04] 位置参数
来源：http://m.share.fktsv.cn/Article/details/gdsjmgusd.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://3g.tarul.cn/Article/details/gcigzbdze.sHtML

[R05] 参数默认值
来源：http://blog.sjlbkw.cn/Article/details/gvjgowdfg.sHtML

name="${1:-default}"
来源：http://www.share.sjlbkw.cn/Article/details/grebhhsmb.sHtML

[R06] 判断命令是否存在
来源：http://mobile.epnwcf.com/Article/details/gfmpiqyml.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://blog.yfazqb.com/Article/details/gwjzxzmhl.sHtML

[R07] if 判断文件
来源：http://baike.yfazqb.com/Article/details/gpylxttvz.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://baike.vehdjk.com/Article/details/gmjhkbqxs.sHtML

[R08] 数值比较
来源：http://www.m.share.fktsv.cn/Article/details/gfjvgqwqy.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://mobile.vehdjk.com/Article/details/gahwwzaxk.sHtML

[R09] 字符串比较
来源：http://mobile.tarul.cn/Article/details/gixbclxrb.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.m.share.vehdjk.com/Article/details/gjjdlgxii.sHtML

[R10] 正则匹配
来源：http://mobile.tarul.cn/Article/details/gpafhqaav.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://mobile.vehdjk.com/Article/details/gwquokdwx.sHtML

[R11] case 多分支
来源：http://read.share.yfazqb.com/Article/details/gjovtakeu.sHtML

case "$1" in
来源：http://blog.vehdjk.com/Article/details/gqtovjkeo.sHtML

start) echo "启动" ;;
来源：http://baike.yfazqb.com/Article/details/gdjsdprco.sHtML

stop)  echo "停止" ;;
来源：http://m.share.sjlbkw.cn/Article/details/gcxbvbkgf.sHtML

*)     echo "未知命令" ;;
来源：http://www.m.share.bbcook.cn/Article/details/gbmguxrgf.sHtML

esac
来源：http://m.share.yfazqb.com/Article/details/gxpgdpiar.sHtML

[R12] for 遍历文件
来源：http://read.share.bbcook.cn/Article/details/gsvchpgmh.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.blog.bbcook.cn/Article/details/gfkchvztk.sHtML

[R13] for 计数循环
来源：http://baike.epnwcf.com/Article/details/gloxiafru.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://blog.sjlbkw.cn/Article/details/ggbfsyakv.sHtML

[R14] C 风格 for
来源：http://blog.sjlbkw.cn/Article/details/gtrfhrmib.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://m.share.fktsv.cn/Article/details/gvkpnbdnm.sHtML

[R15] while 逐行读文件
来源：http://3g.bbcook.cn/Article/details/gjnxbthqp.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://wap.vehdjk.com/Article/details/gxlfrntpy.sHtML

[R16] until 等待条件
来源：http://www.share.fktsv.cn/Article/details/gcxwwtsrd.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://blog.bbcook.cn/Article/details/gyqupnaul.sHtML

[R17] 数组定义与取值
来源：http://blog.sjlbkw.cn/Article/details/gxpbfmtou.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://read.share.yfazqb.com/Article/details/gwbsjbdgs.sHtML

[R18] 遍历数组
来源：http://mobile.vehdjk.com/Article/details/glabiunod.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://read.share.epnwcf.com/Article/details/ghlbrnvjd.sHtML

[R19] 数组长度
来源：http://www.m.share.tarul.cn/Article/details/ghdeyblzj.sHtML

echo "${#arr[@]}"
来源：http://mobile.yfazqb.com/Article/details/gzyvtqjgi.sHtML

[R20] 关联数组（字典）
来源：http://mobile.tarul.cn/Article/details/gqvvhbtyv.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.m.share.epnwcf.com/Article/details/grxanmbwi.sHtML

[R21] 字符串长度
来源：http://www.share.yfazqb.com/Article/details/girazhpbc.sHtML

echo "${#s}"
来源：http://baike.fktsv.cn/Article/details/gvcexxsiz.sHtML

[R22] 截取子串
来源：http://m.share.sjlbkw.cn/Article/details/gqtkpgdmj.sHtML

echo "${s:0:5}"
来源：http://www.share.tarul.cn/Article/details/gvdmasqdx.sHtML

[R23] 字符串替换
来源：http://www.m.share.tarul.cn/Article/details/gpdngendc.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.share.tarul.cn/Article/details/gvdksptpg.sHtML

[R24] 大小写转换
来源：http://m.share.yfazqb.com/Article/details/gxpkvcghc.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://read.share.epnwcf.com/Article/details/gjmrhbzgt.sHtML

[R25] 去后缀 / 去前缀
来源：http://blog.sjlbkw.cn/Article/details/gubwmjgln.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.share.epnwcf.com/Article/details/gvgrcoeap.sHtML

[R26] 命令替换
来源：http://www.m.share.tarul.cn/Article/details/gzdnzublt.sHtML

now=$(date +%F); echo "$now"
来源：http://www.share.bbcook.cn/Article/details/gjtessktu.sHtML

[R27] 算术展开
来源：http://www.m.share.epnwcf.com/Article/details/gvqridjaw.sHtML

echo $((1 + 2 * 3))
来源：http://mobile.sjlbkw.cn/Article/details/gsuwkarla.sHtML

[R28] 浮点运算
来源：http://m.share.sjlbkw.cn/Article/details/gxhpaawbb.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.share.tarul.cn/Article/details/ghdqpwkhi.sHtML

[R29] 定义函数
来源：http://www.share.epnwcf.com/Article/details/gcxpugcjr.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://read.share.tarul.cn/Article/details/gelnnvjzu.sHtML

[R30] 函数返回状态码
来源：http://www.share.sjlbkw.cn/Article/details/gfuwwidrg.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://mobile.fktsv.cn/Article/details/gfmgjqiii.sHtML

[R31] 局部变量
来源：http://www.m.share.yfazqb.com/Article/details/gjpqmzejk.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.share.sjlbkw.cn/Article/details/gtvfhkdok.sHtML

[R32] 参数个数校验
来源：http://read.share.sjlbkw.cn/Article/details/gdmoofwob.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.m.share.vehdjk.com/Article/details/gyczvgtkd.sHtML

[R33] 捕获错误并提示行号
来源：http://mobile.epnwcf.com/Article/details/gblaqvigp.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://m.share.sjlbkw.cn/Article/details/gfkkljtpw.sHtML

[R34] 退出时清理
来源：http://wap.sjlbkw.cn/Article/details/ggsulbvvf.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://wap.tarul.cn/Article/details/gzzatslbr.sHtML

[R35] 后台执行并等待
来源：http://baike.epnwcf.com/Article/details/gxtxamiyo.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://baike.tarul.cn/Article/details/gstfyntnq.sHtML

[R36] 并发执行多个任务
来源：http://wap.tarul.cn/Article/details/gfqoaxcui.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://wap.epnwcf.com/Article/details/grxhokzjq.sHtML

[R37] 把输出赋给变量
来源：http://www.blog.sjlbkw.cn/Article/details/gvewuankk.sHtML

files=$(ls -1)
来源：http://www.share.sjlbkw.cn/Article/details/gmctfaxlu.sHtML

[R38] 管道串联
来源：http://wap.vehdjk.com/Article/details/gashlvssr.sHtML

cat a.txt | grep -i error | wc -l
来源：http://read.share.fktsv.cn/Article/details/gobfyczhz.sHtML

[R39] 重定向标准输出与错误
来源：http://www.m.share.epnwcf.com/Article/details/ghnzxzocx.sHtML

cmd > out.log 2>&1
来源：http://baike.sjlbkw.cn/Article/details/gmitgmetr.sHtML

[R40] 追加写日志
来源：http://3g.bbcook.cn/Article/details/gtzunfaat.sHtML

echo "log" >> out.log
来源：http://www.share.bbcook.cn/Article/details/gjelmfqgk.sHtML

[R41] 丢弃输出
来源：http://www.m.share.sjlbkw.cn/Article/details/ggxadnkpt.sHtML

cmd >/dev/null 2>&1
来源：http://wap.bbcook.cn/Article/details/gseqcujlx.sHtML

[R42] 输入重定向
来源：http://www.share.sjlbkw.cn/Article/details/gqpviqovf.sHtML

wc -l < a.txt
来源：http://m.share.epnwcf.com/Article/details/glxvqbvvl.sHtML

[R43] 按名字查找文件
来源：http://3g.fktsv.cn/Article/details/gdyqnmwpn.sHtML

find . -name "*.log" -type f
来源：http://www.share.vehdjk.com/Article/details/gcwfualao.sHtML

[R44] 按修改时间查找
来源：http://mobile.yfazqb.com/Article/details/gtxouydre.sHtML

find . -mtime -7 -type f
来源：http://www.m.share.yfazqb.com/Article/details/gtgdfobjk.sHtML

[R45] 批量删除
来源：http://www.share.vehdjk.com/Article/details/gbapzvuwr.sHtML

find . -name "*.tmp" -delete
来源：http://blog.epnwcf.com/Article/details/gabxmixan.sHtML

[R46] 递归替换文件内容
来源：http://blog.bbcook.cn/Article/details/gjvcmbici.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mobile.tarul.cn/Article/details/ghdryfvrh.sHtML

[R47] sed 单行替换
来源：http://3g.sjlbkw.cn/Article/details/gfhtrocwx.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://m.share.fktsv.cn/Article/details/gmqpxermc.sHtML

[R48] awk 取指定列
来源：http://www.blog.yfazqb.com/Article/details/gqbmhpoge.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.blog.epnwcf.com/Article/details/gerlwobej.sHtML

[R49] awk 带条件
来源：http://www.share.vehdjk.com/Article/details/gqtgxnajh.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wap.bbcook.cn/Article/details/gfulivieo.sHtML

[R50] awk 求和
来源：http://mobile.sjlbkw.cn/Article/details/ghwqawhsf.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.m.share.epnwcf.com/Article/details/griyksyst.sHtML

[R51] 排序去重取前几
来源：http://3g.bbcook.cn/Article/details/gctklfcdm.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.share.epnwcf.com/Article/details/gdiqqrecx.sHtML

[R52] 统计行数
来源：http://wap.fktsv.cn/Article/details/gkwgnnwjm.sHtML

wc -l a.txt
来源：http://www.share.fktsv.cn/Article/details/gsdxrkwnl.sHtML

[R53] 查看文件头与实时尾
来源：http://www.blog.epnwcf.com/Article/details/glqtnlgar.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://3g.sjlbkw.cn/Article/details/gtsflckmj.sHtML

[R54] 比较两个文件
来源：http://www.share.tarul.cn/Article/details/gurqpkcwm.sHtML

diff a.txt b.txt
来源：http://mobile.tarul.cn/Article/details/gpgefpytn.sHtML

[R55] 压缩与解压
来源：http://www.blog.yfazqb.com/Article/details/gmdtdqzmk.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://m.share.tarul.cn/Article/details/gfykbwbrs.sHtML

[R56] 远程拷贝
来源：http://baike.vehdjk.com/Article/details/gjfrjqkhr.sHtML

scp file user@host:/path/
来源：http://3g.tarul.cn/Article/details/gkoezqtai.sHtML

[R57] 远程执行命令
来源：http://baike.epnwcf.com/Article/details/gceycdhnz.sHtML

ssh user@host 'uptime'
来源：http://blog.tarul.cn/Article/details/gtjvsscjl.sHtML

[R58] 下载文件
来源：http://www.m.share.vehdjk.com/Article/details/gfyssfkpe.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://read.share.tarul.cn/Article/details/gubgojogn.sHtML

[R59] 发 POST JSON
来源：http://baike.yfazqb.com/Article/details/grhhjplub.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://mobile.tarul.cn/Article/details/gnfffczta.sHtML

[R60] 只看 HTTP 状态码
来源：http://wap.sjlbkw.cn/Article/details/ghvnozfns.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://baike.fktsv.cn/Article/details/gfxjvoidh.sHtML

[R61] 磁盘占用
来源：http://www.share.yfazqb.com/Article/details/gnqoyfodo.sHtML

df -h;  du -sh *
来源：http://read.share.yfazqb.com/Article/details/gjapuubbo.sHtML

[R62] 找最占空间的文件
来源：http://blog.yfazqb.com/Article/details/gliiuqwra.sHtML

du -ah . | sort -rh | head -10
来源：http://www.share.vehdjk.com/Article/details/gzflopqpf.sHtML

[R63] 内存与进程
来源：http://3g.fktsv.cn/Article/details/gyggwkwbs.sHtML

free -h;  ps aux | grep nginx
来源：http://3g.epnwcf.com/Article/details/gglowtccz.sHtML

[R64] 结束进程
来源：http://www.m.share.sjlbkw.cn/Article/details/gnseqamxx.sHtML

kill -9 $(pgrep -f app.py)
来源：http://wap.yfazqb.com/Article/details/gsajsmvga.sHtML

[R65] 查看端口占用
来源：http://www.share.vehdjk.com/Article/details/gkwfyucyw.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wap.vehdjk.com/Article/details/gbnqtrtax.sHtML

[R66] 定时任务
来源：http://wap.sjlbkw.cn/Article/details/gaaohncek.sHtML

crontab -e;  crontab -l
来源：http://mobile.epnwcf.com/Article/details/gofnxpdoy.sHtML

[R67] 生成随机十六进制串
来源：http://wap.yfazqb.com/Article/details/grqumtdrt.sHtML

openssl rand -hex 16
来源：http://m.share.epnwcf.com/Article/details/gafikntfg.sHtML

[R68] 计算文件校验值
来源：http://read.share.tarul.cn/Article/details/gclacsbse.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://wap.bbcook.cn/Article/details/gvrrakcrm.sHtML

[R69] 生成随机密码
来源：http://baike.tarul.cn/Article/details/gnexteutf.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.blog.sjlbkw.cn/Article/details/gkmntxjjt.sHtML

[R70] 时间戳与互转
来源：http://baike.yfazqb.com/Article/details/gybvuwrrp.sHtML

date +%s;  date -d @1700000000
来源：http://www.blog.fktsv.cn/Article/details/gdixqmgfv.sHtML

[R71] 日期格式化
来源：http://www.m.share.epnwcf.com/Article/details/gatpmtkgl.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.blog.fktsv.cn/Article/details/ghizqrnga.sHtML

[R72] 等待端口就绪
来源：http://www.m.share.sjlbkw.cn/Article/details/grmasckbg.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://wap.bbcook.cn/Article/details/gqoweihef.sHtML

[R73] 分割大日志
来源：http://mobile.epnwcf.com/Article/details/glsksiwwk.sHtML

split -l 1000 big.log part_
来源：http://m.share.fktsv.cn/Article/details/gvztimnuh.sHtML

[R74] 批量重命名
来源：http://read.share.epnwcf.com/Article/details/gnvjqefqh.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.blog.yfazqb.com/Article/details/gcimkutjh.sHtML

[R75] 导出环境变量
来源：http://blog.sjlbkw.cn/Article/details/grfjqjmcg.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.share.yfazqb.com/Article/details/gvcgkhamf.sHtML

[R76] 使用临时文件
来源：http://www.blog.fktsv.cn/Article/details/gavqgmnng.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://blog.vehdjk.com/Article/details/glyuvjjad.sHtML

[R77] 读取用户输入
来源：http://3g.epnwcf.com/Article/details/gqqpkwphk.sHtML

read -rp "请输入: " ans
来源：http://mobile.fktsv.cn/Article/details/gdxekgumx.sHtML

[R78] 交互式菜单
来源：http://3g.sjlbkw.cn/Article/details/givxobysu.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://mobile.epnwcf.com/Article/details/gcycgucqy.sHtML

[R79] 解析命令行选项
来源：http://www.m.share.yfazqb.com/Article/details/ggohscorh.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.m.share.yfazqb.com/Article/details/gdteviima.sHtML

[R80] 查看脚本执行耗时
来源：http://www.m.share.bbcook.cn/Article/details/ggsbivzad.sHtML

time ./run.sh
来源：http://blog.epnwcf.com/Article/details/gqkkotvvf.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/gocjbuzof.sHtML

S. C / C++ 专题
来源：http://www.share.tarul.cn/Article/details/gtmybvzsq.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/gxymkjgrr.sHtML

[S01] C：Hello World
来源：http://blog.yfazqb.com/Article/details/gdznwswjh.sHtML

#include <stdio.h>
来源：http://www.m.share.bbcook.cn/Article/details/gditjefpn.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://mobile.epnwcf.com/Article/details/gqmidshcz.sHtML

[S02] C：变量与格式化输出
来源：http://www.m.share.fktsv.cn/Article/details/ggbhklego.sHtML

int a = 10; printf("%d\n", a);
来源：http://baike.yfazqb.com/Article/details/guewdgvcx.sHtML

[S03] C：读入整数
来源：http://3g.yfazqb.com/Article/details/gfodefnsx.sHtML

int x; scanf("%d", &x);
来源：http://m.share.epnwcf.com/Article/details/gzbmpoqxm.sHtML

[S04] C：字符串复制
来源：http://www.share.yfazqb.com/Article/details/gncvvpfle.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://blog.yfazqb.com/Article/details/gictlyumr.sHtML

[S05] C：字符串长度
来源：http://baike.vehdjk.com/Article/details/ghtfkikih.sHtML

strlen(s)
来源：http://3g.bbcook.cn/Article/details/ggwmdswnw.sHtML

[S06] C：字符串比较
来源：http://blog.vehdjk.com/Article/details/gnvjwpjfx.sHtML

strcmp(a, b) == 0
来源：http://blog.bbcook.cn/Article/details/ggdfnmrvn.sHtML

[S07] C：数组遍历求和
来源：http://www.share.yfazqb.com/Article/details/gbrgxsmti.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://baike.epnwcf.com/Article/details/goirueluc.sHtML

[S08] C：动态内存分配与释放
来源：http://baike.epnwcf.com/Article/details/glwnhlwcs.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://3g.tarul.cn/Article/details/geqklefeo.sHtML

[S09] C：结构体定义与初始化
来源：http://www.m.share.fktsv.cn/Article/details/gitgbuuiq.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://read.share.tarul.cn/Article/details/gbvvhmbfy.sHtML

[S10] C：指针与解引用
来源：http://m.share.sjlbkw.cn/Article/details/gsobfdnue.sHtML

int *p = &a;  *p = 5;
来源：http://baike.sjlbkw.cn/Article/details/gklcmcmlk.sHtML

[S11] C：逐行读文件
来源：http://www.m.share.tarul.cn/Article/details/gpirlhodj.sHtML


<!-- 参考信息 -->