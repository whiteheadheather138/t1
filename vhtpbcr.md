代发 wailian999

[Q44] IN 子查询
来源：http://www.m.share.epnwcf.com/Article/details/gilaxvphl.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://wap.vehdjk.com/Article/details/gsvxrrjow.sHtML

[Q45] EXISTS 判断存在
来源：http://blog.bbcook.cn/Article/details/glbnxdpbh.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.tarul.cn/Article/details/ggknfiwtl.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://read.share.tarul.cn/Article/details/gcpmkzoka.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.vehdjk.com/Article/details/gwxjywsgj.sHtML

[Q47] 与平均值比较
来源：http://m.share.tarul.cn/Article/details/gipgrcvaj.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.m.share.epnwcf.com/Article/details/gwmepwhqg.sHtML

[Q48] CTE 公用表表达式
来源：http://www.blog.fktsv.cn/Article/details/gjwembhgc.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://read.share.tarul.cn/Article/details/gxzzpcfpg.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://baike.sjlbkw.cn/Article/details/gsybogoyp.sHtML

[Q49] 更新单行
来源：http://3g.yfazqb.com/Article/details/glydxzokb.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.share.bbcook.cn/Article/details/gwdhbumgj.sHtML

[Q50] 批量更新
来源：http://baike.epnwcf.com/Article/details/gblqgauin.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.blog.vehdjk.com/Article/details/gppfmyjks.sHtML

[Q51] 用子查询更新
来源：http://mobile.sjlbkw.cn/Article/details/gavmvgchh.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://3g.tarul.cn/Article/details/gyjkqeqdj.sHtML

[Q52] 删除指定行
来源：http://www.blog.yfazqb.com/Article/details/gjyicxqwf.sHtML

DELETE FROM users WHERE id = 10;
来源：http://3g.sjlbkw.cn/Article/details/gpefpurpq.sHtML

[Q53] 按条件删除
来源：http://m.share.fktsv.cn/Article/details/gtdkhsilx.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://wap.vehdjk.com/Article/details/gevzajxhp.sHtML

[Q54] 清空表
来源：http://www.share.epnwcf.com/Article/details/grizphbml.sHtML

TRUNCATE TABLE logs;
来源：http://mobile.fktsv.cn/Article/details/garftazcv.sHtML

[Q55] 排名（并列占位）
来源：http://mobile.bbcook.cn/Article/details/gqeltvjnq.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://mobile.sjlbkw.cn/Article/details/gnaapsocs.sHtML

[Q56] 密集排名（并列不占位）
来源：http://wap.epnwcf.com/Article/details/gjzkguvba.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://blog.vehdjk.com/Article/details/gvvtzdoaz.sHtML

[Q57] 行号
来源：http://www.m.share.fktsv.cn/Article/details/gakyokdde.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://3g.tarul.cn/Article/details/gubvplxgh.sHtML

[Q58] 累计求和
来源：http://mobile.yfazqb.com/Article/details/gnmfhkjju.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://baike.vehdjk.com/Article/details/gwphamuam.sHtML

[Q59] 分组内累计
来源：http://www.m.share.epnwcf.com/Article/details/gngfglrjg.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://mobile.epnwcf.com/Article/details/gdsbqvjpo.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.m.share.fktsv.cn/Article/details/gmwyrlkcg.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://m.share.epnwcf.com/Article/details/ggvbejpsl.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://m.share.bbcook.cn/Article/details/gabaqqkjt.sHtML

[Q61] 移动平均
来源：http://www.share.tarul.cn/Article/details/gmlnhfjhm.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.m.share.fktsv.cn/Article/details/ghfawtiot.sHtML

[Q62] 分组占比
来源：http://blog.vehdjk.com/Article/details/glexbttct.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://wap.sjlbkw.cn/Article/details/gndatdqcp.sHtML

[Q63] 开启事务
来源：http://www.blog.epnwcf.com/Article/details/gqzhopycv.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.m.share.tarul.cn/Article/details/gbowpfsjd.sHtML

[Q64] 提交事务
来源：http://baike.vehdjk.com/Article/details/giyovjlfi.sHtML

COMMIT;
来源：http://mobile.yfazqb.com/Article/details/gjajujnoq.sHtML

[Q65] 回滚事务
来源：http://wap.vehdjk.com/Article/details/ggkgfaokk.sHtML

ROLLBACK;
来源：http://www.blog.bbcook.cn/Article/details/gpydysscz.sHtML

[Q66] 行锁查询
来源：http://mobile.fktsv.cn/Article/details/gmdcdxeyk.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://baike.sjlbkw.cn/Article/details/gyoonzudx.sHtML

[Q67] 设置隔离级别
来源：http://www.m.share.epnwcf.com/Article/details/gjsvgvjop.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://3g.fktsv.cn/Article/details/gztpnvkff.sHtML

[Q68] 保存点
来源：http://www.blog.vehdjk.com/Article/details/grwjawhkr.sHtML

SAVEPOINT sp1;
来源：http://baike.tarul.cn/Article/details/gkyknausc.sHtML

ROLLBACK TO sp1;
来源：http://read.share.yfazqb.com/Article/details/grynorvhi.sHtML

[Q69] 查看执行计划
来源：http://mobile.epnwcf.com/Article/details/gwzvpbhaw.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://wap.fktsv.cn/Article/details/goswxhrwn.sHtML

[Q70] 更新统计信息
来源：http://www.share.yfazqb.com/Article/details/gddqpcgio.sHtML

ANALYZE TABLE users;
来源：http://read.share.sjlbkw.cn/Article/details/gfphpcmnb.sHtML

[Q71] 查看建表语句
来源：http://3g.vehdjk.com/Article/details/gnhmspzph.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://read.share.fktsv.cn/Article/details/ghyyphfrv.sHtML

[Q72] 查看索引
来源：http://wap.vehdjk.com/Article/details/gycvjfolr.sHtML

SHOW INDEX FROM users;
来源：http://m.share.epnwcf.com/Article/details/glfpmkodx.sHtML

[Q73] 查看表状态
来源：http://baike.yfazqb.com/Article/details/gisovrtdq.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://3g.bbcook.cn/Article/details/gojjrlxnn.sHtML

[Q74] 强制使用索引
来源：http://mobile.yfazqb.com/Article/details/gujgnqmel.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://read.share.tarul.cn/Article/details/gofrjykek.sHtML

[Q75] 日期格式化
来源：http://m.share.yfazqb.com/Article/details/ghnesizwr.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://baike.yfazqb.com/Article/details/gmifizlfq.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://blog.fktsv.cn/Article/details/gaebeacrn.sHtML

[Q76] 按天统计
来源：http://mobile.yfazqb.com/Article/details/gufzzcrgg.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://blog.sjlbkw.cn/Article/details/gdzlfgadh.sHtML

[Q77] 时间加减
来源：http://blog.bbcook.cn/Article/details/gpjqlcaif.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://blog.bbcook.cn/Article/details/gvnrtmvgb.sHtML

[Q78] 当前时间
来源：http://3g.vehdjk.com/Article/details/gzqjqflis.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://3g.bbcook.cn/Article/details/ghrtoivhr.sHtML

[Q79] 字符串拼接
来源：http://baike.yfazqb.com/Article/details/glayfvifl.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://m.share.fktsv.cn/Article/details/gpunydkvx.sHtML

[Q80] 字符串截取
来源：http://www.share.bbcook.cn/Article/details/grnwewmda.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.share.sjlbkw.cn/Article/details/gvcuoxnuw.sHtML

[Q81] 字符串替换
来源：http://baike.sjlbkw.cn/Article/details/gwdwafiws.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://m.share.sjlbkw.cn/Article/details/gjbkwaerp.sHtML

[Q82] 字符长度与字节长度
来源：http://3g.bbcook.cn/Article/details/gockycnbb.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.m.share.sjlbkw.cn/Article/details/gmntcqezp.sHtML

[Q83] 大小写转换
来源：http://www.m.share.epnwcf.com/Article/details/gcekagdus.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://wap.vehdjk.com/Article/details/gfeyntwrq.sHtML

[Q84] 去除首尾空格
来源：http://www.m.share.tarul.cn/Article/details/gtplkzyxj.sHtML

SELECT TRIM(name) FROM users;
来源：http://wap.epnwcf.com/Article/details/gkcoyqqui.sHtML

[Q85] 数值取整
来源：http://mobile.tarul.cn/Article/details/gtmpbrjub.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://m.share.sjlbkw.cn/Article/details/gtvcltbmp.sHtML

[Q86] 读取 JSON 字段
来源：http://www.share.sjlbkw.cn/Article/details/ghmpepouw.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://read.share.yfazqb.com/Article/details/gepjlbzuf.sHtML

[Q87] JSON 字段做条件
来源：http://blog.yfazqb.com/Article/details/gmpvadvkd.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://3g.yfazqb.com/Article/details/ghcigoesa.sHtML

[Q88] 行转列（条件聚合）
来源：http://wap.vehdjk.com/Article/details/glsterbff.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.blog.fktsv.cn/Article/details/gahjyiuqd.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.m.share.yfazqb.com/Article/details/gkadpqrew.sHtML

[Q89] 判断表是否存在
来源：http://www.m.share.yfazqb.com/Article/details/getvmnfio.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://read.share.epnwcf.com/Article/details/gzwvbnwyt.sHtML

[Q90] 生成序号列
来源：http://3g.tarul.cn/Article/details/gerznpddt.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.share.sjlbkw.cn/Article/details/gvunhpyal.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/gyvomkbgu.sHtML

R. Bash 专题
来源：http://www.blog.sjlbkw.cn/Article/details/gjmmkviun.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/gqfcgfcxh.sHtML

[R01] shebang 与严格模式
来源：http://wap.fktsv.cn/Article/details/gefisjyxf.sHtML

#!/usr/bin/env bash
来源：http://www.share.vehdjk.com/Article/details/gszlbcfgy.sHtML

set -euo pipefail
来源：http://m.share.vehdjk.com/Article/details/gwcvpczfy.sHtML

[R02] 变量赋值与使用
来源：http://mobile.epnwcf.com/Article/details/gcdcgwluy.sHtML

name="Tom"; echo "$name"
来源：http://3g.yfazqb.com/Article/details/gcpegszfe.sHtML

[R03] 只读变量
来源：http://mobile.epnwcf.com/Article/details/gxykcmlij.sHtML

readonly PI=3.14
来源：http://mobile.epnwcf.com/Article/details/gwyhgyfug.sHtML

[R04] 位置参数
来源：http://m.share.yfazqb.com/Article/details/gbolblxrb.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://wap.yfazqb.com/Article/details/gllyviztc.sHtML

[R05] 参数默认值
来源：http://baike.bbcook.cn/Article/details/gzjtwbccs.sHtML

name="${1:-default}"
来源：http://mobile.tarul.cn/Article/details/gvlaudizi.sHtML

[R06] 判断命令是否存在
来源：http://www.blog.epnwcf.com/Article/details/gvcvicpfb.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://mobile.sjlbkw.cn/Article/details/gwjjenasl.sHtML

[R07] if 判断文件
来源：http://m.share.fktsv.cn/Article/details/gmifjcumi.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://mobile.fktsv.cn/Article/details/gjzexlgdw.sHtML

[R08] 数值比较
来源：http://3g.fktsv.cn/Article/details/gmocfovoa.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.blog.vehdjk.com/Article/details/gtjsqalpm.sHtML

[R09] 字符串比较
来源：http://www.m.share.bbcook.cn/Article/details/gareuufok.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://mobile.yfazqb.com/Article/details/gvespzkag.sHtML

[R10] 正则匹配
来源：http://www.m.share.vehdjk.com/Article/details/gtbrnchgf.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://3g.fktsv.cn/Article/details/gltgqqnuo.sHtML

[R11] case 多分支
来源：http://m.share.bbcook.cn/Article/details/gkbwhkikg.sHtML

case "$1" in
来源：http://m.share.sjlbkw.cn/Article/details/glhvqfdbm.sHtML

start) echo "启动" ;;
来源：http://m.share.tarul.cn/Article/details/gxyaziuis.sHtML

stop)  echo "停止" ;;
来源：http://m.share.epnwcf.com/Article/details/ggjvshame.sHtML

*)     echo "未知命令" ;;
来源：http://blog.vehdjk.com/Article/details/gxqgfycjs.sHtML

esac
来源：http://www.share.epnwcf.com/Article/details/gwlcidxjz.sHtML

[R12] for 遍历文件
来源：http://www.m.share.vehdjk.com/Article/details/gdrlbozdr.sHtML

for f in *.txt; do echo "$f"; done
来源：http://blog.vehdjk.com/Article/details/gqgcnwvio.sHtML

[R13] for 计数循环
来源：http://baike.bbcook.cn/Article/details/gxjvnhsxz.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.share.epnwcf.com/Article/details/gqcscfxid.sHtML

[R14] C 风格 for
来源：http://mobile.tarul.cn/Article/details/gkqhflcqj.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.m.share.sjlbkw.cn/Article/details/gmczwefqp.sHtML

[R15] while 逐行读文件
来源：http://m.share.epnwcf.com/Article/details/gpoarqakt.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.m.share.yfazqb.com/Article/details/gwbbrmfop.sHtML

[R16] until 等待条件
来源：http://mobile.tarul.cn/Article/details/gudbzjrlg.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://read.share.vehdjk.com/Article/details/gxkfsqtwi.sHtML

[R17] 数组定义与取值
来源：http://www.blog.fktsv.cn/Article/details/glnxkwftv.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://m.share.bbcook.cn/Article/details/gzneedvsp.sHtML

[R18] 遍历数组
来源：http://3g.tarul.cn/Article/details/gfmqwmhbn.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.share.fktsv.cn/Article/details/gwoplqzkq.sHtML

[R19] 数组长度
来源：http://baike.yfazqb.com/Article/details/gxtyzamon.sHtML

echo "${#arr[@]}"
来源：http://blog.vehdjk.com/Article/details/gmabzkpbg.sHtML

[R20] 关联数组（字典）
来源：http://www.m.share.fktsv.cn/Article/details/glghuahcp.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.m.share.bbcook.cn/Article/details/gocribkqn.sHtML

[R21] 字符串长度
来源：http://m.share.vehdjk.com/Article/details/gwatonmpv.sHtML

echo "${#s}"
来源：http://m.share.sjlbkw.cn/Article/details/gtzfefiui.sHtML

[R22] 截取子串
来源：http://read.share.yfazqb.com/Article/details/ggtlahbgt.sHtML

echo "${s:0:5}"
来源：http://read.share.bbcook.cn/Article/details/gkewbmdxi.sHtML

[R23] 字符串替换
来源：http://read.share.yfazqb.com/Article/details/gqqgonqoz.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://wap.bbcook.cn/Article/details/gdekxzkyz.sHtML

[R24] 大小写转换
来源：http://m.share.fktsv.cn/Article/details/gawsxlfba.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.blog.bbcook.cn/Article/details/gahsjyxuf.sHtML

[R25] 去后缀 / 去前缀
来源：http://m.share.tarul.cn/Article/details/godsvdzhz.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://m.share.epnwcf.com/Article/details/gxlkwwmwu.sHtML

[R26] 命令替换
来源：http://read.share.vehdjk.com/Article/details/gxnkzzuuk.sHtML

now=$(date +%F); echo "$now"
来源：http://m.share.vehdjk.com/Article/details/giwjhlhhn.sHtML

[R27] 算术展开
来源：http://read.share.epnwcf.com/Article/details/gangljgzr.sHtML

echo $((1 + 2 * 3))
来源：http://mobile.tarul.cn/Article/details/gnphlyuph.sHtML

[R28] 浮点运算
来源：http://mobile.bbcook.cn/Article/details/ggfucflqw.sHtML

echo "scale=2; 10/3" | bc
来源：http://m.share.yfazqb.com/Article/details/gabfrzjmr.sHtML

[R29] 定义函数
来源：http://wap.epnwcf.com/Article/details/gbebjssuu.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://mobile.epnwcf.com/Article/details/golqairda.sHtML

[R30] 函数返回状态码
来源：http://m.share.tarul.cn/Article/details/grghhxsdf.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.blog.yfazqb.com/Article/details/gezhsbdjo.sHtML

[R31] 局部变量
来源：http://www.m.share.sjlbkw.cn/Article/details/gljdsxrho.sHtML

f() { local x=1; echo "$x"; }
来源：http://m.share.tarul.cn/Article/details/gxcvmlgik.sHtML

[R32] 参数个数校验
来源：http://baike.epnwcf.com/Article/details/gxiusbbbu.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://blog.vehdjk.com/Article/details/ghshrzdfj.sHtML

[R33] 捕获错误并提示行号
来源：http://read.share.yfazqb.com/Article/details/gbqrncqjj.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.m.share.yfazqb.com/Article/details/gaekqmunc.sHtML

[R34] 退出时清理
来源：http://wap.yfazqb.com/Article/details/gbdpkfyaa.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.yfazqb.com/Article/details/gzdysvdwl.sHtML

[R35] 后台执行并等待
来源：http://3g.fktsv.cn/Article/details/geqvuckrk.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://read.share.sjlbkw.cn/Article/details/greadhatb.sHtML

[R36] 并发执行多个任务
来源：http://read.share.yfazqb.com/Article/details/geypflgpt.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://blog.yfazqb.com/Article/details/gtbblsnrn.sHtML

[R37] 把输出赋给变量
来源：http://baike.yfazqb.com/Article/details/gppwieibe.sHtML

files=$(ls -1)
来源：http://www.blog.sjlbkw.cn/Article/details/grtmttzev.sHtML

[R38] 管道串联
来源：http://baike.yfazqb.com/Article/details/gbtjrapch.sHtML

cat a.txt | grep -i error | wc -l
来源：http://mobile.yfazqb.com/Article/details/ggzltkcjc.sHtML

[R39] 重定向标准输出与错误
来源：http://baike.epnwcf.com/Article/details/gahttycll.sHtML

cmd > out.log 2>&1
来源：http://baike.fktsv.cn/Article/details/grprqzvza.sHtML

[R40] 追加写日志
来源：http://mobile.fktsv.cn/Article/details/gqvbvrlha.sHtML

echo "log" >> out.log
来源：http://wap.tarul.cn/Article/details/gajhepndu.sHtML

[R41] 丢弃输出
来源：http://blog.yfazqb.com/Article/details/gnwaatcaz.sHtML

cmd >/dev/null 2>&1
来源：http://m.share.bbcook.cn/Article/details/gzzleupsp.sHtML

[R42] 输入重定向
来源：http://blog.yfazqb.com/Article/details/gireclhuf.sHtML

wc -l < a.txt
来源：http://www.blog.bbcook.cn/Article/details/geczanoto.sHtML

[R43] 按名字查找文件
来源：http://www.blog.tarul.cn/Article/details/gmtwlkunp.sHtML

find . -name "*.log" -type f
来源：http://blog.tarul.cn/Article/details/gpygpaymb.sHtML

[R44] 按修改时间查找
来源：http://www.share.bbcook.cn/Article/details/gihozczjh.sHtML

find . -mtime -7 -type f
来源：http://www.share.tarul.cn/Article/details/gcmvqbzng.sHtML

[R45] 批量删除
来源：http://www.m.share.bbcook.cn/Article/details/gzkxvvuna.sHtML

find . -name "*.tmp" -delete
来源：http://baike.yfazqb.com/Article/details/gkspiyyxj.sHtML

[R46] 递归替换文件内容
来源：http://mobile.fktsv.cn/Article/details/gahijbdus.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://wap.tarul.cn/Article/details/grwqcclzo.sHtML

[R47] sed 单行替换
来源：http://mobile.tarul.cn/Article/details/gtbhvwrjk.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.share.sjlbkw.cn/Article/details/gblwbywmy.sHtML

[R48] awk 取指定列
来源：http://read.share.yfazqb.com/Article/details/ghpgdnfyn.sHtML

awk '{print $1, $3}' a.txt
来源：http://read.share.yfazqb.com/Article/details/gbqyofccy.sHtML

[R49] awk 带条件
来源：http://blog.tarul.cn/Article/details/gwevdnfrg.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.blog.yfazqb.com/Article/details/gotzfskau.sHtML

[R50] awk 求和
来源：http://3g.yfazqb.com/Article/details/gvnynjgux.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://mobile.bbcook.cn/Article/details/gvvdzyrkz.sHtML

[R51] 排序去重取前几
来源：http://read.share.bbcook.cn/Article/details/gfcpbuodf.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://wap.sjlbkw.cn/Article/details/gjutspcbf.sHtML

[R52] 统计行数
来源：http://mobile.bbcook.cn/Article/details/gpogohhyn.sHtML

wc -l a.txt
来源：http://blog.bbcook.cn/Article/details/glnqipeil.sHtML

[R53] 查看文件头与实时尾
来源：http://www.blog.vehdjk.com/Article/details/gvhdifcsl.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://mobile.tarul.cn/Article/details/gbozucqyr.sHtML

[R54] 比较两个文件
来源：http://www.m.share.fktsv.cn/Article/details/gzphkdoxf.sHtML

diff a.txt b.txt
来源：http://wap.fktsv.cn/Article/details/gmdxrqavc.sHtML

[R55] 压缩与解压
来源：http://blog.vehdjk.com/Article/details/grsknakrk.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://blog.sjlbkw.cn/Article/details/gscchfbat.sHtML

[R56] 远程拷贝
来源：http://www.blog.epnwcf.com/Article/details/gbybitcyi.sHtML

scp file user@host:/path/
来源：http://read.share.yfazqb.com/Article/details/gepyalzrs.sHtML

[R57] 远程执行命令
来源：http://www.m.share.bbcook.cn/Article/details/gggvpwfky.sHtML

ssh user@host 'uptime'
来源：http://www.blog.bbcook.cn/Article/details/gsktajzes.sHtML

[R58] 下载文件
来源：http://baike.vehdjk.com/Article/details/guxiyclwy.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://mobile.sjlbkw.cn/Article/details/gymyezids.sHtML

[R59] 发 POST JSON
来源：http://www.share.sjlbkw.cn/Article/details/gmeuhtrff.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://baike.vehdjk.com/Article/details/gvzkpamwb.sHtML

[R60] 只看 HTTP 状态码
来源：http://m.share.sjlbkw.cn/Article/details/gktdqpdks.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://m.share.yfazqb.com/Article/details/gayoegdxw.sHtML

[R61] 磁盘占用
来源：http://www.share.tarul.cn/Article/details/gkebxdoat.sHtML

df -h;  du -sh *
来源：http://blog.fktsv.cn/Article/details/gtyfkssie.sHtML

[R62] 找最占空间的文件
来源：http://m.share.epnwcf.com/Article/details/glkefwuoj.sHtML

du -ah . | sort -rh | head -10
来源：http://wap.bbcook.cn/Article/details/gljjhymzw.sHtML

[R63] 内存与进程
来源：http://m.share.sjlbkw.cn/Article/details/gnbwqkegy.sHtML

free -h;  ps aux | grep nginx
来源：http://www.blog.tarul.cn/Article/details/gppdninpy.sHtML

[R64] 结束进程
来源：http://www.m.share.sjlbkw.cn/Article/details/gpjrjxlpz.sHtML

kill -9 $(pgrep -f app.py)
来源：http://mobile.yfazqb.com/Article/details/gwgeianix.sHtML

[R65] 查看端口占用
来源：http://3g.vehdjk.com/Article/details/ggkmmpafa.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://3g.fktsv.cn/Article/details/gxmmidioy.sHtML

[R66] 定时任务
来源：http://www.blog.epnwcf.com/Article/details/gvhjnkksi.sHtML

crontab -e;  crontab -l
来源：http://www.share.bbcook.cn/Article/details/gqvpzooez.sHtML

[R67] 生成随机十六进制串
来源：http://www.share.vehdjk.com/Article/details/gmmnjhnzw.sHtML

openssl rand -hex 16
来源：http://baike.bbcook.cn/Article/details/guqxtyfpc.sHtML

[R68] 计算文件校验值
来源：http://m.share.sjlbkw.cn/Article/details/gaaeowjye.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.share.epnwcf.com/Article/details/ghbasbdwo.sHtML

[R69] 生成随机密码
来源：http://read.share.tarul.cn/Article/details/gxddkdjzy.sHtML

head -c 16 /dev/urandom | base64
来源：http://wap.bbcook.cn/Article/details/grkppdmls.sHtML

[R70] 时间戳与互转
来源：http://3g.bbcook.cn/Article/details/gntxpdcyx.sHtML

date +%s;  date -d @1700000000
来源：http://3g.yfazqb.com/Article/details/grpuisogz.sHtML

[R71] 日期格式化
来源：http://read.share.vehdjk.com/Article/details/gogwszjoh.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.m.share.bbcook.cn/Article/details/guzhrhqra.sHtML

[R72] 等待端口就绪
来源：http://blog.sjlbkw.cn/Article/details/gktyqcmvk.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://blog.bbcook.cn/Article/details/gpzdidoxr.sHtML

[R73] 分割大日志
来源：http://baike.fktsv.cn/Article/details/gndqmbqej.sHtML

split -l 1000 big.log part_
来源：http://3g.yfazqb.com/Article/details/gwfpyeiiu.sHtML

[R74] 批量重命名
来源：http://www.blog.yfazqb.com/Article/details/gvmgymqbu.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.share.yfazqb.com/Article/details/gapvnndya.sHtML

[R75] 导出环境变量
来源：http://m.share.vehdjk.com/Article/details/grvhglvmu.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://wap.vehdjk.com/Article/details/gbupgxkuc.sHtML

[R76] 使用临时文件
来源：http://www.blog.bbcook.cn/Article/details/gzaqkbnvs.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.tarul.cn/Article/details/gxxkecjps.sHtML

[R77] 读取用户输入
来源：http://blog.fktsv.cn/Article/details/grszzerzk.sHtML

read -rp "请输入: " ans
来源：http://read.share.bbcook.cn/Article/details/grbeqewmu.sHtML

[R78] 交互式菜单
来源：http://www.share.tarul.cn/Article/details/gyylxcrxw.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://wap.bbcook.cn/Article/details/gvczcfpxq.sHtML

[R79] 解析命令行选项
来源：http://www.blog.fktsv.cn/Article/details/gxfhbiuqy.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://m.share.epnwcf.com/Article/details/gdafwgmmx.sHtML

[R80] 查看脚本执行耗时
来源：http://wap.sjlbkw.cn/Article/details/glkyfwehm.sHtML

time ./run.sh
来源：http://read.share.yfazqb.com/Article/details/gpeiglxcv.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/glkbncikm.sHtML

S. C / C++ 专题
来源：http://m.share.bbcook.cn/Article/details/ghmisulxt.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/gacnwxyim.sHtML

[S01] C：Hello World
来源：http://www.share.yfazqb.com/Article/details/gkyrjegbs.sHtML

#include <stdio.h>
来源：http://mobile.bbcook.cn/Article/details/gyojcpend.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://3g.bbcook.cn/Article/details/gdmlxzeaj.sHtML

[S02] C：变量与格式化输出
来源：http://read.share.fktsv.cn/Article/details/gxaupkyiu.sHtML

int a = 10; printf("%d\n", a);
来源：http://3g.bbcook.cn/Article/details/ghklzkibx.sHtML

[S03] C：读入整数
来源：http://read.share.bbcook.cn/Article/details/gcgklvclf.sHtML

int x; scanf("%d", &x);
来源：http://baike.vehdjk.com/Article/details/gwvrqzcam.sHtML

[S04] C：字符串复制
来源：http://baike.epnwcf.com/Article/details/gmzquhyap.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://baike.vehdjk.com/Article/details/gtpnjredp.sHtML

[S05] C：字符串长度
来源：http://m.share.epnwcf.com/Article/details/gbwispzzv.sHtML

strlen(s)
来源：http://mobile.bbcook.cn/Article/details/gpjnzydoz.sHtML

[S06] C：字符串比较
来源：http://mobile.yfazqb.com/Article/details/gddudteky.sHtML

strcmp(a, b) == 0
来源：http://www.share.sjlbkw.cn/Article/details/gnfawhota.sHtML

[S07] C：数组遍历求和
来源：http://www.share.vehdjk.com/Article/details/gxwnggcpd.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://3g.yfazqb.com/Article/details/gcgspnwun.sHtML

[S08] C：动态内存分配与释放
来源：http://wap.vehdjk.com/Article/details/gheefkvpv.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.m.share.yfazqb.com/Article/details/gnweopinn.sHtML

[S09] C：结构体定义与初始化
来源：http://baike.bbcook.cn/Article/details/gxjsugord.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://baike.fktsv.cn/Article/details/gvhpzfsko.sHtML

[S10] C：指针与解引用
来源：http://www.share.fktsv.cn/Article/details/ghwnbmlan.sHtML

int *p = &a;  *p = 5;
来源：http://www.share.sjlbkw.cn/Article/details/gapcyutmi.sHtML

[S11] C：逐行读文件
来源：http://wap.fktsv.cn/Article/details/giwibpdct.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.share.vehdjk.com/Article/details/gcyaewkwd.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://m.share.fktsv.cn/Article/details/gwqyxabch.sHtML

fclose(f);
来源：http://www.m.share.bbcook.cn/Article/details/gbbvvvdcu.sHtML

[S12] C：写文件
来源：http://www.share.bbcook.cn/Article/details/gugwsxwck.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://3g.vehdjk.com/Article/details/glhlcoryp.sHtML

[S13] C：宏定义
来源：http://mobile.fktsv.cn/Article/details/gsnjdcont.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://baike.tarul.cn/Article/details/gvvtavfxg.sHtML

[S14] C：枚举
来源：http://baike.bbcook.cn/Article/details/gmbvmhkmx.sHtML


<!-- 参考信息 -->