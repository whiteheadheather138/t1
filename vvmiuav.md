代发 wailian999

SELECT o.id, u.name, p.title FROM orders o
来源：http://read.share.bbcook.cn/Article/details/gwlmkfhht.sHtML

JOIN users u ON u.id = o.user_id
来源：http://3g.fktsv.cn/Article/details/gzvnqbnmk.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.share.vehdjk.com/Article/details/gfbwiocer.sHtML

[Q42] 连接条件附加过滤
来源：http://www.blog.fktsv.cn/Article/details/gohnxmyot.sHtML

SELECT u.name, o.amount FROM users u
来源：http://blog.fktsv.cn/Article/details/ghcqzsqfw.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://wap.yfazqb.com/Article/details/gixbsvxfu.sHtML

[Q43] 标量子查询
来源：http://wap.vehdjk.com/Article/details/gbbeheboz.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://baike.tarul.cn/Article/details/gboaytvfy.sHtML

[Q44] IN 子查询
来源：http://www.m.share.epnwcf.com/Article/details/gijnpwfma.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.blog.epnwcf.com/Article/details/gvxxwlceq.sHtML

[Q45] EXISTS 判断存在
来源：http://baike.yfazqb.com/Article/details/gtiyfeuoy.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.fktsv.cn/Article/details/gogzukioo.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.m.share.tarul.cn/Article/details/gjsfoxspi.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.tarul.cn/Article/details/gtxrcebub.sHtML

[Q47] 与平均值比较
来源：http://mobile.vehdjk.com/Article/details/ghbpfcbzh.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://blog.tarul.cn/Article/details/gzfruyhhj.sHtML

[Q48] CTE 公用表表达式
来源：http://blog.tarul.cn/Article/details/gxfnuwsft.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://blog.epnwcf.com/Article/details/gpysroduy.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://wap.sjlbkw.cn/Article/details/gqwxtjccn.sHtML

[Q49] 更新单行
来源：http://blog.epnwcf.com/Article/details/gwvmqcrmt.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://blog.tarul.cn/Article/details/gtqqmdziu.sHtML

[Q50] 批量更新
来源：http://read.share.tarul.cn/Article/details/gqmttsqxa.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://read.share.epnwcf.com/Article/details/gtdlaoqkk.sHtML

[Q51] 用子查询更新
来源：http://read.share.yfazqb.com/Article/details/gakdgrdap.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.m.share.vehdjk.com/Article/details/gtasrfhzo.sHtML

[Q52] 删除指定行
来源：http://www.share.yfazqb.com/Article/details/gnrjnxuaw.sHtML

DELETE FROM users WHERE id = 10;
来源：http://mobile.sjlbkw.cn/Article/details/ghvwpvetp.sHtML

[Q53] 按条件删除
来源：http://3g.sjlbkw.cn/Article/details/gpbqdqukh.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.m.share.vehdjk.com/Article/details/gckrdwpgc.sHtML

[Q54] 清空表
来源：http://m.share.tarul.cn/Article/details/gfnpeuscl.sHtML

TRUNCATE TABLE logs;
来源：http://www.blog.epnwcf.com/Article/details/gdesbsgis.sHtML

[Q55] 排名（并列占位）
来源：http://www.blog.tarul.cn/Article/details/gdufemvcf.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://m.share.vehdjk.com/Article/details/gurvgwonf.sHtML

[Q56] 密集排名（并列不占位）
来源：http://blog.fktsv.cn/Article/details/gyffkherv.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.share.bbcook.cn/Article/details/ggkofcxkv.sHtML

[Q57] 行号
来源：http://read.share.bbcook.cn/Article/details/gyuufdrwm.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.blog.bbcook.cn/Article/details/gkcxbclav.sHtML

[Q58] 累计求和
来源：http://www.share.vehdjk.com/Article/details/glkquiyku.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://baike.bbcook.cn/Article/details/gplxwmcsg.sHtML

[Q59] 分组内累计
来源：http://blog.sjlbkw.cn/Article/details/gkxlgbszy.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://mobile.yfazqb.com/Article/details/gipexyjlg.sHtML

[Q60] 取上一行 / 下一行
来源：http://m.share.epnwcf.com/Article/details/gibhyczes.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://read.share.fktsv.cn/Article/details/glgwmixtd.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://mobile.vehdjk.com/Article/details/gfnsehkth.sHtML

[Q61] 移动平均
来源：http://read.share.vehdjk.com/Article/details/gbrdqbdtn.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://3g.vehdjk.com/Article/details/gxiplepqc.sHtML

[Q62] 分组占比
来源：http://m.share.bbcook.cn/Article/details/giutaeukl.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://wap.yfazqb.com/Article/details/gfsaibzar.sHtML

[Q63] 开启事务
来源：http://wap.yfazqb.com/Article/details/gsvaxxobh.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://blog.vehdjk.com/Article/details/giqcxeypr.sHtML

[Q64] 提交事务
来源：http://www.share.tarul.cn/Article/details/grapfvswy.sHtML

COMMIT;
来源：http://m.share.vehdjk.com/Article/details/gomyioxih.sHtML

[Q65] 回滚事务
来源：http://3g.sjlbkw.cn/Article/details/gfcezutyv.sHtML

ROLLBACK;
来源：http://www.share.tarul.cn/Article/details/gjmrtkyeu.sHtML

[Q66] 行锁查询
来源：http://www.blog.bbcook.cn/Article/details/ggafkruqr.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://wap.epnwcf.com/Article/details/ghndnnriu.sHtML

[Q67] 设置隔离级别
来源：http://wap.yfazqb.com/Article/details/goywavklr.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://wap.tarul.cn/Article/details/giflwpbhn.sHtML

[Q68] 保存点
来源：http://read.share.vehdjk.com/Article/details/gvguiqwpm.sHtML

SAVEPOINT sp1;
来源：http://www.share.fktsv.cn/Article/details/gughymhtu.sHtML

ROLLBACK TO sp1;
来源：http://mobile.yfazqb.com/Article/details/geljkddmh.sHtML

[Q69] 查看执行计划
来源：http://www.m.share.fktsv.cn/Article/details/gcploelzb.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://blog.sjlbkw.cn/Article/details/guxqaltfc.sHtML

[Q70] 更新统计信息
来源：http://www.share.bbcook.cn/Article/details/gkejlceyt.sHtML

ANALYZE TABLE users;
来源：http://read.share.fktsv.cn/Article/details/grmvymcah.sHtML

[Q71] 查看建表语句
来源：http://wap.yfazqb.com/Article/details/gmjyacffi.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.blog.sjlbkw.cn/Article/details/gsezqqmbp.sHtML

[Q72] 查看索引
来源：http://m.share.fktsv.cn/Article/details/goxghgzuj.sHtML

SHOW INDEX FROM users;
来源：http://www.m.share.yfazqb.com/Article/details/ghserjojh.sHtML

[Q73] 查看表状态
来源：http://www.blog.sjlbkw.cn/Article/details/gayjvlsdj.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://m.share.vehdjk.com/Article/details/gyuapgnhn.sHtML

[Q74] 强制使用索引
来源：http://baike.tarul.cn/Article/details/ghbdwkkzn.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://wap.yfazqb.com/Article/details/gyeqtapgm.sHtML

[Q75] 日期格式化
来源：http://read.share.yfazqb.com/Article/details/geaselrny.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://blog.bbcook.cn/Article/details/ghnhtidwi.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://3g.tarul.cn/Article/details/gmsgtqbxi.sHtML

[Q76] 按天统计
来源：http://blog.bbcook.cn/Article/details/gkkkglxgg.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://baike.bbcook.cn/Article/details/gnoqulbcc.sHtML

[Q77] 时间加减
来源：http://www.blog.sjlbkw.cn/Article/details/gglokjqig.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.share.yfazqb.com/Article/details/gqpytpqxa.sHtML

[Q78] 当前时间
来源：http://mobile.vehdjk.com/Article/details/gpemwovhb.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://baike.bbcook.cn/Article/details/gocfuyvil.sHtML

[Q79] 字符串拼接
来源：http://wap.bbcook.cn/Article/details/gwumgnvze.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://baike.yfazqb.com/Article/details/gktasybpr.sHtML

[Q80] 字符串截取
来源：http://www.m.share.tarul.cn/Article/details/gattuhmgx.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.share.sjlbkw.cn/Article/details/gmiihzbjh.sHtML

[Q81] 字符串替换
来源：http://www.m.share.yfazqb.com/Article/details/gbzzwgdib.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://read.share.epnwcf.com/Article/details/gagvsknly.sHtML

[Q82] 字符长度与字节长度
来源：http://mobile.fktsv.cn/Article/details/gmcnfuxhm.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://3g.tarul.cn/Article/details/gwimgpibm.sHtML

[Q83] 大小写转换
来源：http://www.share.epnwcf.com/Article/details/gjzxqdupg.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://wap.fktsv.cn/Article/details/gsmlaeslo.sHtML

[Q84] 去除首尾空格
来源：http://mobile.bbcook.cn/Article/details/gcnfdodtw.sHtML

SELECT TRIM(name) FROM users;
来源：http://m.share.yfazqb.com/Article/details/gyqmaggba.sHtML

[Q85] 数值取整
来源：http://read.share.fktsv.cn/Article/details/gixyjozts.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.m.share.bbcook.cn/Article/details/golfmuksj.sHtML

[Q86] 读取 JSON 字段
来源：http://blog.yfazqb.com/Article/details/ginqefhpw.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.blog.yfazqb.com/Article/details/ghghtpznd.sHtML

[Q87] JSON 字段做条件
来源：http://m.share.fktsv.cn/Article/details/gtfoskkob.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.share.epnwcf.com/Article/details/gjwxejbxy.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.share.epnwcf.com/Article/details/giulmenok.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.blog.yfazqb.com/Article/details/greskcmxk.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.m.share.vehdjk.com/Article/details/gaykjesqu.sHtML

[Q89] 判断表是否存在
来源：http://baike.fktsv.cn/Article/details/ggcmfiyvt.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://3g.tarul.cn/Article/details/gchpxxwgx.sHtML

[Q90] 生成序号列
来源：http://www.share.bbcook.cn/Article/details/gedwvgzfb.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://baike.sjlbkw.cn/Article/details/gajskprya.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/giuobduqy.sHtML

R. Bash 专题
来源：http://baike.vehdjk.com/Article/details/gdlkwysjp.sHtML

================================================================================
来源：http://mobile.epnwcf.com/Article/details/gmygfqeqe.sHtML

[R01] shebang 与严格模式
来源：http://read.share.tarul.cn/Article/details/gxlantlcf.sHtML

#!/usr/bin/env bash
来源：http://3g.epnwcf.com/Article/details/guwuayeua.sHtML

set -euo pipefail
来源：http://m.share.tarul.cn/Article/details/glrfqsmiz.sHtML

[R02] 变量赋值与使用
来源：http://www.share.epnwcf.com/Article/details/gnvmeocjw.sHtML

name="Tom"; echo "$name"
来源：http://www.m.share.tarul.cn/Article/details/gmijbejqp.sHtML

[R03] 只读变量
来源：http://3g.fktsv.cn/Article/details/guevqaues.sHtML

readonly PI=3.14
来源：http://read.share.epnwcf.com/Article/details/gpcaciqmv.sHtML

[R04] 位置参数
来源：http://m.share.bbcook.cn/Article/details/gwxwgmczt.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://mobile.epnwcf.com/Article/details/gansngqlj.sHtML

[R05] 参数默认值
来源：http://3g.bbcook.cn/Article/details/goaoeufzn.sHtML

name="${1:-default}"
来源：http://mobile.fktsv.cn/Article/details/gstdlxfon.sHtML

[R06] 判断命令是否存在
来源：http://www.m.share.yfazqb.com/Article/details/gvsxyklna.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://3g.yfazqb.com/Article/details/gzkbxdokf.sHtML

[R07] if 判断文件
来源：http://www.share.vehdjk.com/Article/details/gobhebomt.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.m.share.yfazqb.com/Article/details/gjawzbtmd.sHtML

[R08] 数值比较
来源：http://wap.fktsv.cn/Article/details/gzxivrqfr.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.share.yfazqb.com/Article/details/gqovjmzyq.sHtML

[R09] 字符串比较
来源：http://baike.fktsv.cn/Article/details/gkmyfnkao.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://blog.sjlbkw.cn/Article/details/gugsmsufl.sHtML

[R10] 正则匹配
来源：http://m.share.epnwcf.com/Article/details/gmbhgzltu.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://baike.fktsv.cn/Article/details/gjojaqzjb.sHtML

[R11] case 多分支
来源：http://3g.yfazqb.com/Article/details/gpijrskrm.sHtML

case "$1" in
来源：http://blog.tarul.cn/Article/details/gaqwavzol.sHtML

start) echo "启动" ;;
来源：http://mobile.yfazqb.com/Article/details/gosyjipdu.sHtML

stop)  echo "停止" ;;
来源：http://baike.bbcook.cn/Article/details/gvuanuwuu.sHtML

*)     echo "未知命令" ;;
来源：http://3g.tarul.cn/Article/details/ggaukrodu.sHtML

esac
来源：http://www.share.bbcook.cn/Article/details/gizgmhbir.sHtML

[R12] for 遍历文件
来源：http://baike.yfazqb.com/Article/details/guhuuzcvt.sHtML

for f in *.txt; do echo "$f"; done
来源：http://blog.epnwcf.com/Article/details/gdvaydjmb.sHtML

[R13] for 计数循环
来源：http://3g.vehdjk.com/Article/details/gqeohyjvw.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://mobile.sjlbkw.cn/Article/details/gxqsvelmp.sHtML

[R14] C 风格 for
来源：http://mobile.yfazqb.com/Article/details/gfivurzah.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.blog.yfazqb.com/Article/details/gsbgucrks.sHtML

[R15] while 逐行读文件
来源：http://www.blog.fktsv.cn/Article/details/gqoqcbqhz.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://read.share.sjlbkw.cn/Article/details/gurjommsi.sHtML

[R16] until 等待条件
来源：http://www.m.share.epnwcf.com/Article/details/gnbatffbw.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://blog.sjlbkw.cn/Article/details/gllapdznj.sHtML

[R17] 数组定义与取值
来源：http://www.m.share.yfazqb.com/Article/details/gdcemjlct.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://3g.vehdjk.com/Article/details/gofudaqhe.sHtML

[R18] 遍历数组
来源：http://m.share.fktsv.cn/Article/details/gqdbeefmy.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://baike.yfazqb.com/Article/details/gpwriavlv.sHtML

[R19] 数组长度
来源：http://3g.yfazqb.com/Article/details/gyceqwidh.sHtML

echo "${#arr[@]}"
来源：http://www.blog.tarul.cn/Article/details/gauzkjhqb.sHtML

[R20] 关联数组（字典）
来源：http://www.blog.tarul.cn/Article/details/grdxxhopb.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://baike.tarul.cn/Article/details/gangnnikj.sHtML

[R21] 字符串长度
来源：http://wap.fktsv.cn/Article/details/gebbmbnla.sHtML

echo "${#s}"
来源：http://3g.tarul.cn/Article/details/gsjfxziaz.sHtML

[R22] 截取子串
来源：http://www.m.share.epnwcf.com/Article/details/guexyqerv.sHtML

echo "${s:0:5}"
来源：http://mobile.fktsv.cn/Article/details/gocgnnqew.sHtML

[R23] 字符串替换
来源：http://blog.sjlbkw.cn/Article/details/gvchladgr.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.m.share.vehdjk.com/Article/details/goxdnwwet.sHtML

[R24] 大小写转换
来源：http://wap.bbcook.cn/Article/details/gtskljgol.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://blog.bbcook.cn/Article/details/gyhlenzqo.sHtML

[R25] 去后缀 / 去前缀
来源：http://baike.sjlbkw.cn/Article/details/gjlekwdjm.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://3g.yfazqb.com/Article/details/gxtdsocnx.sHtML

[R26] 命令替换
来源：http://read.share.fktsv.cn/Article/details/girnhbtak.sHtML

now=$(date +%F); echo "$now"
来源：http://www.blog.epnwcf.com/Article/details/gsuqrmvhc.sHtML

[R27] 算术展开
来源：http://3g.yfazqb.com/Article/details/gqfrorxqs.sHtML

echo $((1 + 2 * 3))
来源：http://mobile.bbcook.cn/Article/details/genwjnwwv.sHtML

[R28] 浮点运算
来源：http://blog.bbcook.cn/Article/details/gstxdnwtq.sHtML

echo "scale=2; 10/3" | bc
来源：http://wap.yfazqb.com/Article/details/gmhzazugm.sHtML

[R29] 定义函数
来源：http://baike.yfazqb.com/Article/details/gvawrxtlx.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://blog.epnwcf.com/Article/details/goifugezx.sHtML

[R30] 函数返回状态码
来源：http://m.share.tarul.cn/Article/details/gkthidkbf.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://read.share.yfazqb.com/Article/details/grxlosktk.sHtML

[R31] 局部变量
来源：http://baike.bbcook.cn/Article/details/gzsvqvput.sHtML

f() { local x=1; echo "$x"; }
来源：http://m.share.fktsv.cn/Article/details/guknfiokg.sHtML

[R32] 参数个数校验
来源：http://www.share.yfazqb.com/Article/details/gpecvgiul.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://blog.yfazqb.com/Article/details/gisocgqnb.sHtML

[R33] 捕获错误并提示行号
来源：http://wap.vehdjk.com/Article/details/grrjqxsno.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://mobile.vehdjk.com/Article/details/gmgfbdajs.sHtML

[R34] 退出时清理
来源：http://baike.epnwcf.com/Article/details/groqnxkmt.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://mobile.epnwcf.com/Article/details/gmahonzur.sHtML

[R35] 后台执行并等待
来源：http://blog.bbcook.cn/Article/details/gemjupchw.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://read.share.tarul.cn/Article/details/gxrcbgkqr.sHtML

[R36] 并发执行多个任务
来源：http://www.m.share.tarul.cn/Article/details/gfjhvkjah.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://mobile.fktsv.cn/Article/details/ghwbbmeob.sHtML

[R37] 把输出赋给变量
来源：http://baike.epnwcf.com/Article/details/gcfngyave.sHtML

files=$(ls -1)
来源：http://m.share.tarul.cn/Article/details/grhtxvpau.sHtML

[R38] 管道串联
来源：http://m.share.vehdjk.com/Article/details/gfowbjteo.sHtML

cat a.txt | grep -i error | wc -l
来源：http://3g.fktsv.cn/Article/details/gwgahldtx.sHtML

[R39] 重定向标准输出与错误
来源：http://baike.bbcook.cn/Article/details/gmyxqnalr.sHtML

cmd > out.log 2>&1
来源：http://read.share.bbcook.cn/Article/details/gnkrbkeig.sHtML

[R40] 追加写日志
来源：http://mobile.vehdjk.com/Article/details/grnyzucgd.sHtML

echo "log" >> out.log
来源：http://www.m.share.sjlbkw.cn/Article/details/ggxvedhbx.sHtML

[R41] 丢弃输出
来源：http://3g.fktsv.cn/Article/details/gcdgayrop.sHtML

cmd >/dev/null 2>&1
来源：http://blog.bbcook.cn/Article/details/gsnrsfswp.sHtML

[R42] 输入重定向
来源：http://3g.epnwcf.com/Article/details/ghmqakzoy.sHtML

wc -l < a.txt
来源：http://www.blog.yfazqb.com/Article/details/gjlwzodxb.sHtML

[R43] 按名字查找文件
来源：http://baike.vehdjk.com/Article/details/getifaqhn.sHtML

find . -name "*.log" -type f
来源：http://baike.vehdjk.com/Article/details/gdunrwmuo.sHtML

[R44] 按修改时间查找
来源：http://read.share.vehdjk.com/Article/details/gdwybqgge.sHtML

find . -mtime -7 -type f
来源：http://www.blog.sjlbkw.cn/Article/details/glimybkah.sHtML

[R45] 批量删除
来源：http://www.m.share.vehdjk.com/Article/details/gjhseibtc.sHtML

find . -name "*.tmp" -delete
来源：http://read.share.bbcook.cn/Article/details/gomvftetn.sHtML

[R46] 递归替换文件内容
来源：http://3g.yfazqb.com/Article/details/gimjgmjzz.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.share.sjlbkw.cn/Article/details/goxfdhqsu.sHtML

[R47] sed 单行替换
来源：http://www.share.yfazqb.com/Article/details/gkutcqvyw.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.share.epnwcf.com/Article/details/gikparbob.sHtML

[R48] awk 取指定列
来源：http://3g.vehdjk.com/Article/details/gybnpzhin.sHtML

awk '{print $1, $3}' a.txt
来源：http://wap.vehdjk.com/Article/details/ggfvcgbte.sHtML

[R49] awk 带条件
来源：http://www.blog.fktsv.cn/Article/details/gwspecwtd.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.blog.epnwcf.com/Article/details/gilbonpur.sHtML

[R50] awk 求和
来源：http://3g.fktsv.cn/Article/details/ggyvmsnye.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://wap.fktsv.cn/Article/details/gothvaelo.sHtML

[R51] 排序去重取前几
来源：http://baike.bbcook.cn/Article/details/gtsrfjsou.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://3g.vehdjk.com/Article/details/gmcisuojx.sHtML

[R52] 统计行数
来源：http://wap.epnwcf.com/Article/details/goadyriai.sHtML

wc -l a.txt
来源：http://wap.vehdjk.com/Article/details/gkaqqaqej.sHtML

[R53] 查看文件头与实时尾
来源：http://m.share.tarul.cn/Article/details/gswsukjiu.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://mobile.bbcook.cn/Article/details/gjygmfneu.sHtML

[R54] 比较两个文件
来源：http://www.blog.tarul.cn/Article/details/gvnhvxztt.sHtML

diff a.txt b.txt
来源：http://www.share.epnwcf.com/Article/details/gctzuldrp.sHtML

[R55] 压缩与解压
来源：http://www.m.share.sjlbkw.cn/Article/details/gfgbsrdjr.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mobile.sjlbkw.cn/Article/details/gnjrowxfi.sHtML

[R56] 远程拷贝
来源：http://mobile.sjlbkw.cn/Article/details/gyrbquukf.sHtML

scp file user@host:/path/
来源：http://www.m.share.bbcook.cn/Article/details/gpmtxkuuc.sHtML

[R57] 远程执行命令
来源：http://www.blog.tarul.cn/Article/details/gujavuvnf.sHtML

ssh user@host 'uptime'
来源：http://baike.bbcook.cn/Article/details/gcrhgkqky.sHtML

[R58] 下载文件
来源：http://www.blog.epnwcf.com/Article/details/gvmtewwnq.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://blog.yfazqb.com/Article/details/gimjhzzcq.sHtML

[R59] 发 POST JSON
来源：http://3g.tarul.cn/Article/details/giwziytkv.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.m.share.bbcook.cn/Article/details/gxazkucjs.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.share.epnwcf.com/Article/details/grjpjrmbv.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://wap.bbcook.cn/Article/details/gpwmztrho.sHtML

[R61] 磁盘占用
来源：http://wap.yfazqb.com/Article/details/gbvtqhydo.sHtML

df -h;  du -sh *
来源：http://wap.bbcook.cn/Article/details/gjafipqrw.sHtML

[R62] 找最占空间的文件
来源：http://www.m.share.tarul.cn/Article/details/gnvddfkyr.sHtML

du -ah . | sort -rh | head -10
来源：http://m.share.bbcook.cn/Article/details/gchfyzxix.sHtML

[R63] 内存与进程
来源：http://wap.yfazqb.com/Article/details/gcfiqlcrx.sHtML

free -h;  ps aux | grep nginx
来源：http://read.share.bbcook.cn/Article/details/gjdgimgxh.sHtML

[R64] 结束进程
来源：http://www.blog.yfazqb.com/Article/details/gdixladpn.sHtML

kill -9 $(pgrep -f app.py)
来源：http://blog.bbcook.cn/Article/details/gcbwiojys.sHtML

[R65] 查看端口占用
来源：http://read.share.sjlbkw.cn/Article/details/gwmcfyqsn.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wap.sjlbkw.cn/Article/details/gtmvaqihe.sHtML

[R66] 定时任务
来源：http://www.share.bbcook.cn/Article/details/gpucqcwzg.sHtML

crontab -e;  crontab -l
来源：http://www.m.share.tarul.cn/Article/details/gjxprldwl.sHtML

[R67] 生成随机十六进制串
来源：http://read.share.bbcook.cn/Article/details/gwvgvvzzn.sHtML

openssl rand -hex 16
来源：http://3g.bbcook.cn/Article/details/grzphzxrv.sHtML

[R68] 计算文件校验值
来源：http://blog.tarul.cn/Article/details/gjnsuuymc.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://read.share.epnwcf.com/Article/details/gsayzhjpc.sHtML

[R69] 生成随机密码
来源：http://www.share.fktsv.cn/Article/details/gauobrrzr.sHtML

head -c 16 /dev/urandom | base64
来源：http://read.share.yfazqb.com/Article/details/gbjrrgvhh.sHtML

[R70] 时间戳与互转
来源：http://blog.yfazqb.com/Article/details/gkfevcywd.sHtML

date +%s;  date -d @1700000000
来源：http://www.blog.tarul.cn/Article/details/guizvrbgs.sHtML

[R71] 日期格式化
来源：http://m.share.yfazqb.com/Article/details/gkmcfahgg.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://3g.bbcook.cn/Article/details/gubxaasjj.sHtML

[R72] 等待端口就绪
来源：http://3g.bbcook.cn/Article/details/glyvebqww.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://wap.epnwcf.com/Article/details/ghctjnawy.sHtML

[R73] 分割大日志
来源：http://m.share.tarul.cn/Article/details/gzpbsyknf.sHtML

split -l 1000 big.log part_
来源：http://www.m.share.bbcook.cn/Article/details/ghnzfujwa.sHtML

[R74] 批量重命名
来源：http://blog.vehdjk.com/Article/details/gzhuzeflf.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://blog.yfazqb.com/Article/details/gdsoipluu.sHtML

[R75] 导出环境变量
来源：http://wap.fktsv.cn/Article/details/geunlhxoc.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://baike.epnwcf.com/Article/details/gnqkuxlfk.sHtML

[R76] 使用临时文件
来源：http://wap.fktsv.cn/Article/details/gnqspjzqj.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://wap.vehdjk.com/Article/details/gonjxrkfw.sHtML

[R77] 读取用户输入
来源：http://www.m.share.sjlbkw.cn/Article/details/goupxnfxm.sHtML

read -rp "请输入: " ans
来源：http://blog.epnwcf.com/Article/details/gyrpdvxrm.sHtML

[R78] 交互式菜单
来源：http://read.share.bbcook.cn/Article/details/ggsgjgxgx.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.blog.sjlbkw.cn/Article/details/gdgbtsjjt.sHtML

[R79] 解析命令行选项
来源：http://blog.yfazqb.com/Article/details/ghlawkffn.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://read.share.vehdjk.com/Article/details/giqbqmvfg.sHtML

[R80] 查看脚本执行耗时
来源：http://read.share.tarul.cn/Article/details/gwznxcbbi.sHtML

time ./run.sh
来源：http://wap.epnwcf.com/Article/details/gtjmyytfl.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/glzlxgixs.sHtML

S. C / C++ 专题
来源：http://mobile.vehdjk.com/Article/details/gzeelsany.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/glzvdjwdk.sHtML

[S01] C：Hello World
来源：http://www.blog.bbcook.cn/Article/details/gkdbdeswf.sHtML

#include <stdio.h>
来源：http://www.share.fktsv.cn/Article/details/gsniqjofr.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://read.share.vehdjk.com/Article/details/gpypghtzt.sHtML

[S02] C：变量与格式化输出
来源：http://www.share.sjlbkw.cn/Article/details/grdvgkkxq.sHtML

int a = 10; printf("%d\n", a);
来源：http://3g.fktsv.cn/Article/details/gsieizhqv.sHtML

[S03] C：读入整数
来源：http://baike.sjlbkw.cn/Article/details/gacdftnsv.sHtML

int x; scanf("%d", &x);
来源：http://mobile.bbcook.cn/Article/details/geqrlxfrf.sHtML

[S04] C：字符串复制
来源：http://wap.vehdjk.com/Article/details/ggpaeeaty.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://blog.fktsv.cn/Article/details/gbwtgybca.sHtML

[S05] C：字符串长度
来源：http://mobile.epnwcf.com/Article/details/gepwnwaeo.sHtML

strlen(s)
来源：http://m.share.bbcook.cn/Article/details/gjaxwmvpv.sHtML

[S06] C：字符串比较
来源：http://www.blog.yfazqb.com/Article/details/ghauqqkqh.sHtML

strcmp(a, b) == 0
来源：http://3g.yfazqb.com/Article/details/gefbnmbjn.sHtML

[S07] C：数组遍历求和
来源：http://blog.bbcook.cn/Article/details/gwqixdtna.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.share.epnwcf.com/Article/details/ghokjbxcs.sHtML

[S08] C：动态内存分配与释放
来源：http://baike.sjlbkw.cn/Article/details/gwutzwiet.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.m.share.sjlbkw.cn/Article/details/gegnfzdcs.sHtML

[S09] C：结构体定义与初始化
来源：http://blog.tarul.cn/Article/details/gtqidhzhk.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.m.share.yfazqb.com/Article/details/gsahysoms.sHtML

[S10] C：指针与解引用
来源：http://m.share.tarul.cn/Article/details/gxxxibmmi.sHtML

int *p = &a;  *p = 5;
来源：http://read.share.vehdjk.com/Article/details/gqqwxjqyo.sHtML

[S11] C：逐行读文件
来源：http://www.blog.epnwcf.com/Article/details/gyquxjlyb.sHtML


<!-- 参考信息 -->