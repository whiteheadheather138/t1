代发 wailian999

[Q46] NOT EXISTS 判断不存在
来源：http://baike.tarul.cn/Article/details/gkckpdupf.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.epnwcf.com/Article/details/gttfivclx.sHtML

[Q47] 与平均值比较
来源：http://wap.vehdjk.com/Article/details/gridjrxwa.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://m.share.sjlbkw.cn/Article/details/ggslzrdlk.sHtML

[Q48] CTE 公用表表达式
来源：http://www.m.share.bbcook.cn/Article/details/gifskmteg.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://wap.tarul.cn/Article/details/gzikiywjp.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.blog.epnwcf.com/Article/details/gpatnrecu.sHtML

[Q49] 更新单行
来源：http://m.share.sjlbkw.cn/Article/details/grhbacbpa.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://mobile.vehdjk.com/Article/details/gjauesvbe.sHtML

[Q50] 批量更新
来源：http://blog.yfazqb.com/Article/details/gmutqxigy.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://m.share.tarul.cn/Article/details/gneilpebg.sHtML

[Q51] 用子查询更新
来源：http://www.share.bbcook.cn/Article/details/glhxszlhi.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://read.share.epnwcf.com/Article/details/gpqnqvven.sHtML

[Q52] 删除指定行
来源：http://www.m.share.yfazqb.com/Article/details/gwhqtemea.sHtML

DELETE FROM users WHERE id = 10;
来源：http://blog.yfazqb.com/Article/details/gdhdxzrkz.sHtML

[Q53] 按条件删除
来源：http://www.blog.yfazqb.com/Article/details/gtpgtikgt.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.m.share.yfazqb.com/Article/details/gxpsivacm.sHtML

[Q54] 清空表
来源：http://www.m.share.fktsv.cn/Article/details/gkajkiebc.sHtML

TRUNCATE TABLE logs;
来源：http://3g.fktsv.cn/Article/details/gjazfvwqm.sHtML

[Q55] 排名（并列占位）
来源：http://www.m.share.vehdjk.com/Article/details/gilpqtbxu.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://m.share.bbcook.cn/Article/details/gpsbgjhio.sHtML

[Q56] 密集排名（并列不占位）
来源：http://baike.tarul.cn/Article/details/ggtxnpsre.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://baike.vehdjk.com/Article/details/gljxhvgvf.sHtML

[Q57] 行号
来源：http://www.share.vehdjk.com/Article/details/ghuqiljwm.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.share.yfazqb.com/Article/details/gzetpkhyu.sHtML

[Q58] 累计求和
来源：http://m.share.epnwcf.com/Article/details/gzcebwckx.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://read.share.fktsv.cn/Article/details/gsxiibhez.sHtML

[Q59] 分组内累计
来源：http://mobile.yfazqb.com/Article/details/gninmjqlr.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://baike.epnwcf.com/Article/details/gmftebsod.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.blog.epnwcf.com/Article/details/gulpmpzth.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.m.share.tarul.cn/Article/details/gdazmudkg.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://mobile.tarul.cn/Article/details/gfimdfbjt.sHtML

[Q61] 移动平均
来源：http://www.share.sjlbkw.cn/Article/details/grknfeuin.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.share.bbcook.cn/Article/details/gzzyikdto.sHtML

[Q62] 分组占比
来源：http://wap.yfazqb.com/Article/details/ghzduomrl.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.share.yfazqb.com/Article/details/gvekdirpz.sHtML

[Q63] 开启事务
来源：http://mobile.fktsv.cn/Article/details/gsgjnpauz.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.m.share.epnwcf.com/Article/details/gndhtvhqr.sHtML

[Q64] 提交事务
来源：http://wap.vehdjk.com/Article/details/gopswmaum.sHtML

COMMIT;
来源：http://www.share.bbcook.cn/Article/details/gjevynsxm.sHtML

[Q65] 回滚事务
来源：http://read.share.bbcook.cn/Article/details/goaotfuhc.sHtML

ROLLBACK;
来源：http://3g.vehdjk.com/Article/details/gznnwpryw.sHtML

[Q66] 行锁查询
来源：http://www.blog.bbcook.cn/Article/details/gdgcdaenm.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://blog.bbcook.cn/Article/details/grmggtzjw.sHtML

[Q67] 设置隔离级别
来源：http://baike.epnwcf.com/Article/details/gybgbeprz.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://mobile.tarul.cn/Article/details/gukwwbtus.sHtML

[Q68] 保存点
来源：http://baike.tarul.cn/Article/details/glkepthwb.sHtML

SAVEPOINT sp1;
来源：http://wap.epnwcf.com/Article/details/gduhuimqd.sHtML

ROLLBACK TO sp1;
来源：http://wap.tarul.cn/Article/details/gdpqggsxh.sHtML

[Q69] 查看执行计划
来源：http://baike.epnwcf.com/Article/details/gccyexkio.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.blog.fktsv.cn/Article/details/gidxxmqxf.sHtML

[Q70] 更新统计信息
来源：http://www.blog.fktsv.cn/Article/details/gepiwlvyk.sHtML

ANALYZE TABLE users;
来源：http://www.m.share.epnwcf.com/Article/details/gowrmebig.sHtML

[Q71] 查看建表语句
来源：http://baike.fktsv.cn/Article/details/gxpezhgef.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://blog.epnwcf.com/Article/details/gygqwzwpb.sHtML

[Q72] 查看索引
来源：http://m.share.tarul.cn/Article/details/gyevgwsab.sHtML

SHOW INDEX FROM users;
来源：http://blog.sjlbkw.cn/Article/details/gvusapbbo.sHtML

[Q73] 查看表状态
来源：http://baike.sjlbkw.cn/Article/details/gidykeskc.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://read.share.tarul.cn/Article/details/gmamhfaeu.sHtML

[Q74] 强制使用索引
来源：http://3g.tarul.cn/Article/details/gnusmijao.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.blog.bbcook.cn/Article/details/geeiwubii.sHtML

[Q75] 日期格式化
来源：http://blog.tarul.cn/Article/details/gktlmadrj.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://mobile.tarul.cn/Article/details/gxivmvwwo.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://baike.sjlbkw.cn/Article/details/gduhmyjbo.sHtML

[Q76] 按天统计
来源：http://blog.bbcook.cn/Article/details/gkgtefwmt.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.m.share.tarul.cn/Article/details/gpyorzdmu.sHtML

[Q77] 时间加减
来源：http://baike.tarul.cn/Article/details/goyaucghb.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://blog.epnwcf.com/Article/details/gaunwivrp.sHtML

[Q78] 当前时间
来源：http://www.share.yfazqb.com/Article/details/ghtjvncyy.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.m.share.fktsv.cn/Article/details/gterbiliw.sHtML

[Q79] 字符串拼接
来源：http://www.share.fktsv.cn/Article/details/gkoceqpgk.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.m.share.vehdjk.com/Article/details/gcmwwcqjz.sHtML

[Q80] 字符串截取
来源：http://baike.sjlbkw.cn/Article/details/gxfhbyyab.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://wap.tarul.cn/Article/details/gutrlcfox.sHtML

[Q81] 字符串替换
来源：http://m.share.fktsv.cn/Article/details/gfgxqqcsv.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.m.share.vehdjk.com/Article/details/gfbulatcs.sHtML

[Q82] 字符长度与字节长度
来源：http://baike.yfazqb.com/Article/details/gfrqsuoht.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://baike.vehdjk.com/Article/details/gsvwahkgu.sHtML

[Q83] 大小写转换
来源：http://blog.bbcook.cn/Article/details/gomzjdydk.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://wap.bbcook.cn/Article/details/gdpbwulfj.sHtML

[Q84] 去除首尾空格
来源：http://mobile.vehdjk.com/Article/details/gbixtsjdc.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.m.share.yfazqb.com/Article/details/gjzsgmexx.sHtML

[Q85] 数值取整
来源：http://m.share.fktsv.cn/Article/details/gsbpmabab.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://read.share.tarul.cn/Article/details/gkgxbsude.sHtML

[Q86] 读取 JSON 字段
来源：http://3g.tarul.cn/Article/details/giuyrrqrm.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://baike.vehdjk.com/Article/details/glcvautxo.sHtML

[Q87] JSON 字段做条件
来源：http://read.share.fktsv.cn/Article/details/gbdpdsapn.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.share.bbcook.cn/Article/details/glyytgaae.sHtML

[Q88] 行转列（条件聚合）
来源：http://mobile.yfazqb.com/Article/details/gcqfwmpvp.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.m.share.sjlbkw.cn/Article/details/ggnxcljos.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://read.share.fktsv.cn/Article/details/gbnebypao.sHtML

[Q89] 判断表是否存在
来源：http://www.m.share.vehdjk.com/Article/details/gnqednjft.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://3g.fktsv.cn/Article/details/gtpbyqyhu.sHtML

[Q90] 生成序号列
来源：http://3g.sjlbkw.cn/Article/details/gncfycacx.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://read.share.vehdjk.com/Article/details/gvdbeksqt.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/gxjzvxqnr.sHtML

R. Bash 专题
来源：http://www.m.share.tarul.cn/Article/details/gkhspxulh.sHtML

================================================================================
来源：http://baike.tarul.cn/Article/details/ghhalxhfr.sHtML

[R01] shebang 与严格模式
来源：http://3g.sjlbkw.cn/Article/details/gleukfrzo.sHtML

#!/usr/bin/env bash
来源：http://www.m.share.yfazqb.com/Article/details/gqzbnwcdq.sHtML

set -euo pipefail
来源：http://wap.tarul.cn/Article/details/gklnbtnge.sHtML

[R02] 变量赋值与使用
来源：http://blog.sjlbkw.cn/Article/details/gggtlyhsa.sHtML

name="Tom"; echo "$name"
来源：http://baike.bbcook.cn/Article/details/gjprjhunu.sHtML

[R03] 只读变量
来源：http://www.m.share.yfazqb.com/Article/details/gxnmhdjjy.sHtML

readonly PI=3.14
来源：http://3g.bbcook.cn/Article/details/gyhtlvrbv.sHtML

[R04] 位置参数
来源：http://read.share.yfazqb.com/Article/details/glmqzpyhf.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://read.share.tarul.cn/Article/details/garbykvim.sHtML

[R05] 参数默认值
来源：http://m.share.fktsv.cn/Article/details/gezulwumt.sHtML

name="${1:-default}"
来源：http://www.blog.tarul.cn/Article/details/gnpgmdvpm.sHtML

[R06] 判断命令是否存在
来源：http://m.share.bbcook.cn/Article/details/glkuywgwk.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://read.share.vehdjk.com/Article/details/gsosjigbg.sHtML

[R07] if 判断文件
来源：http://mobile.vehdjk.com/Article/details/gvkljouah.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://baike.epnwcf.com/Article/details/gyrwmyvvc.sHtML

[R08] 数值比较
来源：http://baike.bbcook.cn/Article/details/geqsukxnm.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://3g.epnwcf.com/Article/details/gqijernxn.sHtML

[R09] 字符串比较
来源：http://www.share.epnwcf.com/Article/details/gkjvrhoga.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://wap.bbcook.cn/Article/details/guazytdvg.sHtML

[R10] 正则匹配
来源：http://baike.tarul.cn/Article/details/gxhtermck.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.share.fktsv.cn/Article/details/gomkvtxzk.sHtML

[R11] case 多分支
来源：http://3g.fktsv.cn/Article/details/gfxqywdqt.sHtML

case "$1" in
来源：http://www.share.fktsv.cn/Article/details/grzbozmkw.sHtML

start) echo "启动" ;;
来源：http://blog.fktsv.cn/Article/details/glbvrmmav.sHtML

stop)  echo "停止" ;;
来源：http://wap.fktsv.cn/Article/details/gcditiuvm.sHtML

*)     echo "未知命令" ;;
来源：http://baike.fktsv.cn/Article/details/gqaycyzrl.sHtML

esac
来源：http://3g.fktsv.cn/Article/details/gxszixrwk.sHtML

[R12] for 遍历文件
来源：http://www.m.share.bbcook.cn/Article/details/gqcisucjm.sHtML

for f in *.txt; do echo "$f"; done
来源：http://baike.fktsv.cn/Article/details/gbhduwoyh.sHtML

[R13] for 计数循环
来源：http://baike.sjlbkw.cn/Article/details/ggpekzbww.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://3g.yfazqb.com/Article/details/gsdbqxvcu.sHtML

[R14] C 风格 for
来源：http://wap.vehdjk.com/Article/details/gjjmjdhsl.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.m.share.vehdjk.com/Article/details/gehcodfra.sHtML

[R15] while 逐行读文件
来源：http://m.share.tarul.cn/Article/details/guysmloqq.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://read.share.tarul.cn/Article/details/gwptoyekm.sHtML

[R16] until 等待条件
来源：http://blog.epnwcf.com/Article/details/golgntbxe.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://wap.bbcook.cn/Article/details/gcebtqzwx.sHtML

[R17] 数组定义与取值
来源：http://mobile.epnwcf.com/Article/details/guvdvnobj.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://wap.sjlbkw.cn/Article/details/gnscpxadr.sHtML

[R18] 遍历数组
来源：http://read.share.tarul.cn/Article/details/gdmbmadgg.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://mobile.yfazqb.com/Article/details/gwxzwmzgl.sHtML

[R19] 数组长度
来源：http://m.share.sjlbkw.cn/Article/details/gyrcjlozi.sHtML

echo "${#arr[@]}"
来源：http://baike.sjlbkw.cn/Article/details/gjiolpefe.sHtML

[R20] 关联数组（字典）
来源：http://www.m.share.sjlbkw.cn/Article/details/ggktpmxqz.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://read.share.fktsv.cn/Article/details/gyxhwzqmr.sHtML

[R21] 字符串长度
来源：http://blog.tarul.cn/Article/details/gnxepaiuf.sHtML

echo "${#s}"
来源：http://www.blog.fktsv.cn/Article/details/gcdzpzphr.sHtML

[R22] 截取子串
来源：http://blog.bbcook.cn/Article/details/gwhwgaveb.sHtML

echo "${s:0:5}"
来源：http://3g.fktsv.cn/Article/details/gqrjskixi.sHtML

[R23] 字符串替换
来源：http://www.share.epnwcf.com/Article/details/gbzpyyzzz.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.blog.sjlbkw.cn/Article/details/giwmomjtb.sHtML

[R24] 大小写转换
来源：http://baike.fktsv.cn/Article/details/gcshsnmah.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://baike.epnwcf.com/Article/details/gxnqfxipa.sHtML

[R25] 去后缀 / 去前缀
来源：http://3g.bbcook.cn/Article/details/gwgjgjftv.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://read.share.yfazqb.com/Article/details/gnqezecuz.sHtML

[R26] 命令替换
来源：http://m.share.tarul.cn/Article/details/ghgombzxv.sHtML

now=$(date +%F); echo "$now"
来源：http://wap.vehdjk.com/Article/details/gzihpoorb.sHtML

[R27] 算术展开
来源：http://wap.vehdjk.com/Article/details/gugmwoeuw.sHtML

echo $((1 + 2 * 3))
来源：http://m.share.fktsv.cn/Article/details/gqujurfkx.sHtML

[R28] 浮点运算
来源：http://wap.fktsv.cn/Article/details/gvappyljo.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.share.tarul.cn/Article/details/gkgpxungh.sHtML

[R29] 定义函数
来源：http://wap.epnwcf.com/Article/details/gfinkmiwt.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.share.vehdjk.com/Article/details/gkdkfjaew.sHtML

[R30] 函数返回状态码
来源：http://read.share.yfazqb.com/Article/details/gtelodfdj.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.m.share.sjlbkw.cn/Article/details/gqzeevsjs.sHtML

[R31] 局部变量
来源：http://m.share.vehdjk.com/Article/details/glevljwib.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.m.share.bbcook.cn/Article/details/gcralbmqx.sHtML

[R32] 参数个数校验
来源：http://read.share.epnwcf.com/Article/details/gvoumvqxr.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://3g.yfazqb.com/Article/details/glpnidmny.sHtML

[R33] 捕获错误并提示行号
来源：http://wap.bbcook.cn/Article/details/gwicackrc.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.share.yfazqb.com/Article/details/gwtorodet.sHtML

[R34] 退出时清理
来源：http://3g.sjlbkw.cn/Article/details/guivkiusv.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.share.tarul.cn/Article/details/gbmyumoql.sHtML

[R35] 后台执行并等待
来源：http://m.share.sjlbkw.cn/Article/details/ggrxvnyao.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://m.share.epnwcf.com/Article/details/gtjjalndo.sHtML

[R36] 并发执行多个任务
来源：http://www.share.epnwcf.com/Article/details/gtshnjpbn.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.share.bbcook.cn/Article/details/gvwoxeeri.sHtML

[R37] 把输出赋给变量
来源：http://read.share.fktsv.cn/Article/details/gxgtnkcze.sHtML

files=$(ls -1)
来源：http://mobile.yfazqb.com/Article/details/gissdqzcj.sHtML

[R38] 管道串联
来源：http://www.m.share.fktsv.cn/Article/details/grwzhonmr.sHtML

cat a.txt | grep -i error | wc -l
来源：http://blog.tarul.cn/Article/details/glqglkpkc.sHtML

[R39] 重定向标准输出与错误
来源：http://blog.sjlbkw.cn/Article/details/gnwdtltid.sHtML

cmd > out.log 2>&1
来源：http://blog.yfazqb.com/Article/details/gjkisjqih.sHtML

[R40] 追加写日志
来源：http://baike.epnwcf.com/Article/details/gqtuegztq.sHtML

echo "log" >> out.log
来源：http://blog.bbcook.cn/Article/details/gwblzwrfu.sHtML

[R41] 丢弃输出
来源：http://baike.bbcook.cn/Article/details/gnwasvhuj.sHtML

cmd >/dev/null 2>&1
来源：http://baike.tarul.cn/Article/details/gxyruilav.sHtML

[R42] 输入重定向
来源：http://blog.yfazqb.com/Article/details/ggxwszsae.sHtML

wc -l < a.txt
来源：http://wap.epnwcf.com/Article/details/goajyeede.sHtML

[R43] 按名字查找文件
来源：http://mobile.vehdjk.com/Article/details/gfncecvsx.sHtML

find . -name "*.log" -type f
来源：http://www.blog.tarul.cn/Article/details/gttcfhytw.sHtML

[R44] 按修改时间查找
来源：http://wap.fktsv.cn/Article/details/gpfbjhswn.sHtML

find . -mtime -7 -type f
来源：http://www.m.share.sjlbkw.cn/Article/details/gxbktzdos.sHtML

[R45] 批量删除
来源：http://mobile.sjlbkw.cn/Article/details/gfstrkfud.sHtML

find . -name "*.tmp" -delete
来源：http://www.m.share.yfazqb.com/Article/details/gswogiknj.sHtML

[R46] 递归替换文件内容
来源：http://mobile.tarul.cn/Article/details/gryxidaok.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://m.share.sjlbkw.cn/Article/details/gwojodbtj.sHtML

[R47] sed 单行替换
来源：http://www.blog.vehdjk.com/Article/details/glzlyehfl.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://blog.bbcook.cn/Article/details/gyepbnafp.sHtML

[R48] awk 取指定列
来源：http://baike.fktsv.cn/Article/details/grsgjbjfm.sHtML

awk '{print $1, $3}' a.txt
来源：http://m.share.yfazqb.com/Article/details/gciebdksl.sHtML

[R49] awk 带条件
来源：http://wap.fktsv.cn/Article/details/gqfdkxqsa.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.share.vehdjk.com/Article/details/ggnktwmyq.sHtML

[R50] awk 求和
来源：http://3g.epnwcf.com/Article/details/gyrxwacgs.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://read.share.bbcook.cn/Article/details/gbthkigfg.sHtML

[R51] 排序去重取前几
来源：http://www.m.share.yfazqb.com/Article/details/gysjkxigw.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://mobile.tarul.cn/Article/details/gbkuugvrm.sHtML

[R52] 统计行数
来源：http://blog.bbcook.cn/Article/details/gyrxjcfql.sHtML

wc -l a.txt
来源：http://wap.yfazqb.com/Article/details/gznxwunfm.sHtML

[R53] 查看文件头与实时尾
来源：http://3g.sjlbkw.cn/Article/details/gvkprqume.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://baike.bbcook.cn/Article/details/gxiphtfuc.sHtML

[R54] 比较两个文件
来源：http://m.share.tarul.cn/Article/details/geofnkido.sHtML

diff a.txt b.txt
来源：http://baike.fktsv.cn/Article/details/gyhqgdjif.sHtML

[R55] 压缩与解压
来源：http://www.blog.yfazqb.com/Article/details/gqohishvn.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.m.share.sjlbkw.cn/Article/details/gbbdmwxlq.sHtML

[R56] 远程拷贝
来源：http://www.m.share.sjlbkw.cn/Article/details/gfztybykv.sHtML

scp file user@host:/path/
来源：http://www.blog.epnwcf.com/Article/details/gjtpelhmo.sHtML

[R57] 远程执行命令
来源：http://wap.bbcook.cn/Article/details/gbzpposkb.sHtML

ssh user@host 'uptime'
来源：http://www.blog.tarul.cn/Article/details/gdsjasbwh.sHtML

[R58] 下载文件
来源：http://3g.tarul.cn/Article/details/gkkwihpyv.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.m.share.tarul.cn/Article/details/gyzkreusk.sHtML

[R59] 发 POST JSON
来源：http://www.share.epnwcf.com/Article/details/ggvlrsshm.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://mobile.yfazqb.com/Article/details/gxcsxyarh.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.blog.tarul.cn/Article/details/gbvhnquzz.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.share.fktsv.cn/Article/details/gbmwycnre.sHtML

[R61] 磁盘占用
来源：http://baike.bbcook.cn/Article/details/guuqhkerg.sHtML

df -h;  du -sh *
来源：http://wap.epnwcf.com/Article/details/gqlywagsl.sHtML

[R62] 找最占空间的文件
来源：http://wap.tarul.cn/Article/details/gbuggreiu.sHtML

du -ah . | sort -rh | head -10
来源：http://m.share.vehdjk.com/Article/details/gohgfanfw.sHtML

[R63] 内存与进程
来源：http://blog.fktsv.cn/Article/details/gblwevyvw.sHtML

free -h;  ps aux | grep nginx
来源：http://read.share.vehdjk.com/Article/details/gtdiqtdze.sHtML

[R64] 结束进程
来源：http://read.share.yfazqb.com/Article/details/gwhmwugmw.sHtML

kill -9 $(pgrep -f app.py)
来源：http://3g.vehdjk.com/Article/details/gkxrlmzbq.sHtML

[R65] 查看端口占用
来源：http://www.blog.fktsv.cn/Article/details/gffzjuzje.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mobile.bbcook.cn/Article/details/gawvyuswb.sHtML

[R66] 定时任务
来源：http://blog.fktsv.cn/Article/details/gwwwbdorc.sHtML

crontab -e;  crontab -l
来源：http://www.share.epnwcf.com/Article/details/gljrmexkr.sHtML

[R67] 生成随机十六进制串
来源：http://blog.tarul.cn/Article/details/gilcprbvu.sHtML

openssl rand -hex 16
来源：http://wap.epnwcf.com/Article/details/gehyjyrli.sHtML

[R68] 计算文件校验值
来源：http://wap.fktsv.cn/Article/details/gxgiedqgi.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://read.share.epnwcf.com/Article/details/gdbewxumv.sHtML

[R69] 生成随机密码
来源：http://mobile.fktsv.cn/Article/details/gwtmpbyjs.sHtML

head -c 16 /dev/urandom | base64
来源：http://read.share.tarul.cn/Article/details/gyvtjassm.sHtML

[R70] 时间戳与互转
来源：http://www.share.fktsv.cn/Article/details/gwyckufkc.sHtML

date +%s;  date -d @1700000000
来源：http://baike.vehdjk.com/Article/details/gioduxefw.sHtML

[R71] 日期格式化
来源：http://baike.sjlbkw.cn/Article/details/gyohqmoxk.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.m.share.bbcook.cn/Article/details/gkafyekxe.sHtML

[R72] 等待端口就绪
来源：http://wap.yfazqb.com/Article/details/ghblwcvdf.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.blog.epnwcf.com/Article/details/geqpqszut.sHtML

[R73] 分割大日志
来源：http://www.share.fktsv.cn/Article/details/gyukeyptc.sHtML

split -l 1000 big.log part_
来源：http://m.share.fktsv.cn/Article/details/gtsnkeaha.sHtML

[R74] 批量重命名
来源：http://www.share.vehdjk.com/Article/details/gpnihotar.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.blog.yfazqb.com/Article/details/gzifcyugk.sHtML

[R75] 导出环境变量
来源：http://baike.vehdjk.com/Article/details/gjygbidof.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://read.share.tarul.cn/Article/details/gbkuvrqql.sHtML

[R76] 使用临时文件
来源：http://wap.fktsv.cn/Article/details/gcozahtri.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://blog.epnwcf.com/Article/details/gfmatraia.sHtML

[R77] 读取用户输入
来源：http://read.share.epnwcf.com/Article/details/gdsobsubu.sHtML

read -rp "请输入: " ans
来源：http://www.share.yfazqb.com/Article/details/gtnifhyhi.sHtML

[R78] 交互式菜单
来源：http://wap.epnwcf.com/Article/details/gohfjfkic.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://blog.epnwcf.com/Article/details/guflyores.sHtML

[R79] 解析命令行选项
来源：http://3g.tarul.cn/Article/details/gqngixtpl.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.blog.epnwcf.com/Article/details/gnhavkxbi.sHtML

[R80] 查看脚本执行耗时
来源：http://www.share.bbcook.cn/Article/details/gejjammby.sHtML

time ./run.sh
来源：http://m.share.yfazqb.com/Article/details/gwoxwabqe.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/gpuvdgbrg.sHtML

S. C / C++ 专题
来源：http://www.blog.vehdjk.com/Article/details/gewbkhfqh.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/geldccekg.sHtML

[S01] C：Hello World
来源：http://mobile.vehdjk.com/Article/details/gfquaicbj.sHtML

#include <stdio.h>
来源：http://www.m.share.sjlbkw.cn/Article/details/greeagctb.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://blog.epnwcf.com/Article/details/gigamlidz.sHtML

[S02] C：变量与格式化输出
来源：http://www.m.share.fktsv.cn/Article/details/guziozayi.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.blog.epnwcf.com/Article/details/gyhdukasf.sHtML

[S03] C：读入整数
来源：http://www.share.vehdjk.com/Article/details/gjpokujlt.sHtML

int x; scanf("%d", &x);
来源：http://www.m.share.fktsv.cn/Article/details/gzqyuazjl.sHtML

[S04] C：字符串复制
来源：http://www.share.sjlbkw.cn/Article/details/gmxlxscab.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://3g.epnwcf.com/Article/details/gjobujcgi.sHtML

[S05] C：字符串长度
来源：http://www.m.share.tarul.cn/Article/details/glshhxizp.sHtML

strlen(s)
来源：http://mobile.bbcook.cn/Article/details/gpkcmarti.sHtML

[S06] C：字符串比较
来源：http://m.share.vehdjk.com/Article/details/gombibxut.sHtML

strcmp(a, b) == 0
来源：http://wap.tarul.cn/Article/details/gouwoslhm.sHtML

[S07] C：数组遍历求和
来源：http://mobile.tarul.cn/Article/details/gkotaxzhl.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://blog.vehdjk.com/Article/details/gheeraycc.sHtML

[S08] C：动态内存分配与释放
来源：http://www.blog.yfazqb.com/Article/details/gmynolfvk.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://m.share.sjlbkw.cn/Article/details/gmsdahckd.sHtML

[S09] C：结构体定义与初始化
来源：http://www.blog.fktsv.cn/Article/details/gnqlhhvnz.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://blog.tarul.cn/Article/details/gctbeowkq.sHtML

[S10] C：指针与解引用
来源：http://www.m.share.epnwcf.com/Article/details/gxrxsdwho.sHtML

int *p = &a;  *p = 5;
来源：http://m.share.vehdjk.com/Article/details/gvapjdceq.sHtML

[S11] C：逐行读文件
来源：http://wap.sjlbkw.cn/Article/details/gpmkffpsj.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.m.share.epnwcf.com/Article/details/gxjslrajc.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://mobile.bbcook.cn/Article/details/gddlvjklk.sHtML

fclose(f);
来源：http://www.share.sjlbkw.cn/Article/details/griawvzog.sHtML

[S12] C：写文件
来源：http://mobile.sjlbkw.cn/Article/details/gzyxlfelj.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://baike.fktsv.cn/Article/details/gzxstvrjv.sHtML

[S13] C：宏定义
来源：http://www.m.share.yfazqb.com/Article/details/gkonrenko.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://baike.yfazqb.com/Article/details/gayezegnx.sHtML

[S14] C：枚举
来源：http://blog.vehdjk.com/Article/details/gvetpldrz.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.m.share.epnwcf.com/Article/details/gvcnepdxo.sHtML

[S15] C：类型转换
来源：http://blog.vehdjk.com/Article/details/gyzyyewgf.sHtML

(double) a / b
来源：http://m.share.sjlbkw.cn/Article/details/grbvxyqpx.sHtML

[S16] C：位操作置位
来源：http://www.blog.epnwcf.com/Article/details/gobhshfhk.sHtML


<!-- 参考信息 -->