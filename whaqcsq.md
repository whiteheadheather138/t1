代发 wailian999

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://baike.bbcook.cn/Article/details/gyuqmfgsx.sHtML

[Q52] 删除指定行
来源：http://blog.yfazqb.com/Article/details/goxdgrtff.sHtML

DELETE FROM users WHERE id = 10;
来源：http://read.share.vehdjk.com/Article/details/gsorvbeiw.sHtML

[Q53] 按条件删除
来源：http://www.blog.epnwcf.com/Article/details/gzgnekqow.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.blog.fktsv.cn/Article/details/gwoftbxfe.sHtML

[Q54] 清空表
来源：http://blog.yfazqb.com/Article/details/gwultoaeb.sHtML

TRUNCATE TABLE logs;
来源：http://www.m.share.yfazqb.com/Article/details/gndapoxwy.sHtML

[Q55] 排名（并列占位）
来源：http://blog.fktsv.cn/Article/details/gqpfyahlz.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://wap.yfazqb.com/Article/details/ggxjoeuwz.sHtML

[Q56] 密集排名（并列不占位）
来源：http://3g.fktsv.cn/Article/details/gyvvpweaf.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://blog.sjlbkw.cn/Article/details/gkrxvxozd.sHtML

[Q57] 行号
来源：http://3g.sjlbkw.cn/Article/details/gqfrzummg.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://mobile.yfazqb.com/Article/details/gwwfmumto.sHtML

[Q58] 累计求和
来源：http://baike.sjlbkw.cn/Article/details/gmimrmfnn.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://m.share.sjlbkw.cn/Article/details/gqtxxaaxk.sHtML

[Q59] 分组内累计
来源：http://3g.vehdjk.com/Article/details/gafadviwp.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://wap.bbcook.cn/Article/details/gunbdecvz.sHtML

[Q60] 取上一行 / 下一行
来源：http://3g.bbcook.cn/Article/details/gktulzjnv.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.share.yfazqb.com/Article/details/ghhbjduer.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://3g.yfazqb.com/Article/details/gmmafcohi.sHtML

[Q61] 移动平均
来源：http://blog.tarul.cn/Article/details/gvxfzmrqy.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://m.share.yfazqb.com/Article/details/grhcthzde.sHtML

[Q62] 分组占比
来源：http://m.share.sjlbkw.cn/Article/details/gyfugiejk.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://blog.yfazqb.com/Article/details/gdiescxjc.sHtML

[Q63] 开启事务
来源：http://wap.epnwcf.com/Article/details/gyvomjkan.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://read.share.fktsv.cn/Article/details/gnhgminwe.sHtML

[Q64] 提交事务
来源：http://mobile.epnwcf.com/Article/details/grukejrwj.sHtML

COMMIT;
来源：http://www.share.vehdjk.com/Article/details/gdsqtxycv.sHtML

[Q65] 回滚事务
来源：http://www.m.share.sjlbkw.cn/Article/details/gxwrtmtxo.sHtML

ROLLBACK;
来源：http://3g.tarul.cn/Article/details/gjtxhmmgq.sHtML

[Q66] 行锁查询
来源：http://www.blog.sjlbkw.cn/Article/details/gpvbkulmd.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://read.share.vehdjk.com/Article/details/gkihbryui.sHtML

[Q67] 设置隔离级别
来源：http://mobile.bbcook.cn/Article/details/gsauckeok.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.m.share.fktsv.cn/Article/details/gxabqgoyc.sHtML

[Q68] 保存点
来源：http://baike.tarul.cn/Article/details/gzoqrgwxb.sHtML

SAVEPOINT sp1;
来源：http://3g.epnwcf.com/Article/details/gouylhoss.sHtML

ROLLBACK TO sp1;
来源：http://wap.vehdjk.com/Article/details/gzcohcdeu.sHtML

[Q69] 查看执行计划
来源：http://baike.yfazqb.com/Article/details/gxlaxshvn.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://mobile.bbcook.cn/Article/details/gkcwkwkyn.sHtML

[Q70] 更新统计信息
来源：http://m.share.yfazqb.com/Article/details/gcmltqcqp.sHtML

ANALYZE TABLE users;
来源：http://www.m.share.yfazqb.com/Article/details/ghtpauoir.sHtML

[Q71] 查看建表语句
来源：http://www.blog.fktsv.cn/Article/details/gxaljogxu.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://m.share.yfazqb.com/Article/details/gfnrgulno.sHtML

[Q72] 查看索引
来源：http://m.share.epnwcf.com/Article/details/gtmckqhqt.sHtML

SHOW INDEX FROM users;
来源：http://wap.vehdjk.com/Article/details/gwfvcqqai.sHtML

[Q73] 查看表状态
来源：http://www.m.share.sjlbkw.cn/Article/details/gatgahntx.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.blog.tarul.cn/Article/details/gwyvlrsnx.sHtML

[Q74] 强制使用索引
来源：http://m.share.epnwcf.com/Article/details/gvnbjexou.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://blog.yfazqb.com/Article/details/gopqubdjs.sHtML

[Q75] 日期格式化
来源：http://baike.vehdjk.com/Article/details/gnbpshjcb.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://blog.fktsv.cn/Article/details/goxgtqeac.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.blog.yfazqb.com/Article/details/gayhozmpl.sHtML

[Q76] 按天统计
来源：http://www.blog.tarul.cn/Article/details/gtmfqoiua.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://blog.tarul.cn/Article/details/grcehtifi.sHtML

[Q77] 时间加减
来源：http://baike.bbcook.cn/Article/details/gogdcemvo.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.share.tarul.cn/Article/details/gzirujzcl.sHtML

[Q78] 当前时间
来源：http://3g.sjlbkw.cn/Article/details/gniijgqez.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.m.share.fktsv.cn/Article/details/gnuwesukp.sHtML

[Q79] 字符串拼接
来源：http://mobile.epnwcf.com/Article/details/gpssmivhd.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://read.share.tarul.cn/Article/details/ggccepcbr.sHtML

[Q80] 字符串截取
来源：http://blog.epnwcf.com/Article/details/ghwbjgqrj.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://wap.epnwcf.com/Article/details/grpznywfe.sHtML

[Q81] 字符串替换
来源：http://www.m.share.tarul.cn/Article/details/gpmornnfp.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://mobile.sjlbkw.cn/Article/details/glysucfxo.sHtML

[Q82] 字符长度与字节长度
来源：http://m.share.vehdjk.com/Article/details/ghyskhzwv.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://wap.tarul.cn/Article/details/gdyzcwkmj.sHtML

[Q83] 大小写转换
来源：http://wap.bbcook.cn/Article/details/gnoabdgil.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://read.share.bbcook.cn/Article/details/gkkhjkjuq.sHtML

[Q84] 去除首尾空格
来源：http://m.share.tarul.cn/Article/details/grkavmmcj.sHtML

SELECT TRIM(name) FROM users;
来源：http://3g.tarul.cn/Article/details/gsszwlvyj.sHtML

[Q85] 数值取整
来源：http://www.m.share.sjlbkw.cn/Article/details/gjbhtqhgo.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://m.share.bbcook.cn/Article/details/gdskguezq.sHtML

[Q86] 读取 JSON 字段
来源：http://read.share.fktsv.cn/Article/details/gdewqelku.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.m.share.yfazqb.com/Article/details/ghhtdzoem.sHtML

[Q87] JSON 字段做条件
来源：http://www.share.epnwcf.com/Article/details/gwhsavyol.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://mobile.tarul.cn/Article/details/gwwnvwaka.sHtML

[Q88] 行转列（条件聚合）
来源：http://baike.sjlbkw.cn/Article/details/gerlabfwh.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.blog.fktsv.cn/Article/details/gkeobwjcs.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.share.sjlbkw.cn/Article/details/gbllplgxm.sHtML

[Q89] 判断表是否存在
来源：http://wap.fktsv.cn/Article/details/gfbhznfvi.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://mobile.fktsv.cn/Article/details/gvtzfgpkg.sHtML

[Q90] 生成序号列
来源：http://www.share.tarul.cn/Article/details/gsvxkmtfd.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://3g.tarul.cn/Article/details/grlzztnbc.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/gslxqqrnh.sHtML

R. Bash 专题
来源：http://3g.bbcook.cn/Article/details/gwepevfid.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/gmqjxheky.sHtML

[R01] shebang 与严格模式
来源：http://m.share.yfazqb.com/Article/details/gwzqhfxrr.sHtML

#!/usr/bin/env bash
来源：http://www.share.yfazqb.com/Article/details/gbwfcqiyf.sHtML

set -euo pipefail
来源：http://www.m.share.vehdjk.com/Article/details/ghnfsayui.sHtML

[R02] 变量赋值与使用
来源：http://www.blog.tarul.cn/Article/details/gcaooqeiv.sHtML

name="Tom"; echo "$name"
来源：http://www.blog.yfazqb.com/Article/details/gnahipkth.sHtML

[R03] 只读变量
来源：http://wap.fktsv.cn/Article/details/gnzvzbxgn.sHtML

readonly PI=3.14
来源：http://blog.sjlbkw.cn/Article/details/grbyxyhwm.sHtML

[R04] 位置参数
来源：http://read.share.tarul.cn/Article/details/gpzmdbjqe.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://baike.tarul.cn/Article/details/gcclaflsl.sHtML

[R05] 参数默认值
来源：http://wap.sjlbkw.cn/Article/details/glcomueol.sHtML

name="${1:-default}"
来源：http://www.blog.epnwcf.com/Article/details/gdkoouqrb.sHtML

[R06] 判断命令是否存在
来源：http://mobile.epnwcf.com/Article/details/gsxcifxay.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.share.vehdjk.com/Article/details/gvagmubig.sHtML

[R07] if 判断文件
来源：http://blog.epnwcf.com/Article/details/govzmqjry.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://m.share.epnwcf.com/Article/details/gdcccmpas.sHtML

[R08] 数值比较
来源：http://baike.bbcook.cn/Article/details/getqegndu.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.blog.bbcook.cn/Article/details/gfokczfti.sHtML

[R09] 字符串比较
来源：http://m.share.bbcook.cn/Article/details/gbfdqlfxd.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://read.share.epnwcf.com/Article/details/gnzpknspe.sHtML

[R10] 正则匹配
来源：http://www.m.share.vehdjk.com/Article/details/gvxxuoils.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.blog.tarul.cn/Article/details/gczfuonwk.sHtML

[R11] case 多分支
来源：http://www.blog.bbcook.cn/Article/details/godkyntkc.sHtML

case "$1" in
来源：http://read.share.fktsv.cn/Article/details/gkgzuzbjr.sHtML

start) echo "启动" ;;
来源：http://3g.bbcook.cn/Article/details/ggtbjmuak.sHtML

stop)  echo "停止" ;;
来源：http://mobile.vehdjk.com/Article/details/ggwmzhqas.sHtML

*)     echo "未知命令" ;;
来源：http://blog.fktsv.cn/Article/details/gpubrxgyn.sHtML

esac
来源：http://3g.sjlbkw.cn/Article/details/gplxxrmle.sHtML

[R12] for 遍历文件
来源：http://wap.fktsv.cn/Article/details/gmouhyubt.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.share.fktsv.cn/Article/details/gpeynlvmm.sHtML

[R13] for 计数循环
来源：http://www.m.share.bbcook.cn/Article/details/gvkbzomun.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://baike.vehdjk.com/Article/details/gjjiphcoh.sHtML

[R14] C 风格 for
来源：http://www.blog.tarul.cn/Article/details/gyxakheev.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://blog.fktsv.cn/Article/details/glokcqikn.sHtML

[R15] while 逐行读文件
来源：http://3g.bbcook.cn/Article/details/gdmasdkiq.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.share.yfazqb.com/Article/details/ggxbmgpti.sHtML

[R16] until 等待条件
来源：http://mobile.fktsv.cn/Article/details/gtpmgkrby.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.blog.fktsv.cn/Article/details/gzfixyvyz.sHtML

[R17] 数组定义与取值
来源：http://read.share.yfazqb.com/Article/details/gicrifjxp.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://baike.vehdjk.com/Article/details/gtapxtami.sHtML

[R18] 遍历数组
来源：http://read.share.bbcook.cn/Article/details/gzuftybgv.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://blog.fktsv.cn/Article/details/geuccrmra.sHtML

[R19] 数组长度
来源：http://blog.bbcook.cn/Article/details/grrllppfe.sHtML

echo "${#arr[@]}"
来源：http://www.share.fktsv.cn/Article/details/gbfelksql.sHtML

[R20] 关联数组（字典）
来源：http://www.blog.bbcook.cn/Article/details/gbrtglwzj.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://baike.tarul.cn/Article/details/gupmhlack.sHtML

[R21] 字符串长度
来源：http://blog.bbcook.cn/Article/details/gvwjicnkv.sHtML

echo "${#s}"
来源：http://www.share.yfazqb.com/Article/details/gycggwygb.sHtML

[R22] 截取子串
来源：http://blog.vehdjk.com/Article/details/gctclaomg.sHtML

echo "${s:0:5}"
来源：http://m.share.yfazqb.com/Article/details/gmclmwbdd.sHtML

[R23] 字符串替换
来源：http://wap.bbcook.cn/Article/details/gxjmzgrsg.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://blog.yfazqb.com/Article/details/guoywplzd.sHtML

[R24] 大小写转换
来源：http://www.share.fktsv.cn/Article/details/gdfqrzull.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.blog.sjlbkw.cn/Article/details/ggohsnegt.sHtML

[R25] 去后缀 / 去前缀
来源：http://read.share.tarul.cn/Article/details/gjiupximk.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://m.share.fktsv.cn/Article/details/gfgolabrk.sHtML

[R26] 命令替换
来源：http://wap.sjlbkw.cn/Article/details/ghcptvatl.sHtML

now=$(date +%F); echo "$now"
来源：http://3g.epnwcf.com/Article/details/gydlkkjpp.sHtML

[R27] 算术展开
来源：http://read.share.yfazqb.com/Article/details/gipahlrox.sHtML

echo $((1 + 2 * 3))
来源：http://baike.sjlbkw.cn/Article/details/gkdvysqyx.sHtML

[R28] 浮点运算
来源：http://www.blog.epnwcf.com/Article/details/gkijydwhm.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.share.yfazqb.com/Article/details/ggvdhpzrz.sHtML

[R29] 定义函数
来源：http://wap.vehdjk.com/Article/details/glilbbwwq.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.share.yfazqb.com/Article/details/gfqvibngl.sHtML

[R30] 函数返回状态码
来源：http://www.share.tarul.cn/Article/details/gwjkqicht.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://read.share.sjlbkw.cn/Article/details/gayauoqcl.sHtML

[R31] 局部变量
来源：http://3g.vehdjk.com/Article/details/gaxcwjemn.sHtML

f() { local x=1; echo "$x"; }
来源：http://read.share.epnwcf.com/Article/details/gsnzadsky.sHtML

[R32] 参数个数校验
来源：http://www.m.share.bbcook.cn/Article/details/gnsphznqj.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.m.share.epnwcf.com/Article/details/gbhfcfthd.sHtML

[R33] 捕获错误并提示行号
来源：http://baike.fktsv.cn/Article/details/gvtxndhdt.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.blog.epnwcf.com/Article/details/gkejtocor.sHtML

[R34] 退出时清理
来源：http://mobile.vehdjk.com/Article/details/goxezgjzw.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.share.epnwcf.com/Article/details/glzbfefwp.sHtML

[R35] 后台执行并等待
来源：http://m.share.bbcook.cn/Article/details/ggqcfopit.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://m.share.sjlbkw.cn/Article/details/gisbvbwui.sHtML

[R36] 并发执行多个任务
来源：http://www.m.share.tarul.cn/Article/details/gjaaizwpe.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://mobile.fktsv.cn/Article/details/gxxyvaqjy.sHtML

[R37] 把输出赋给变量
来源：http://www.share.yfazqb.com/Article/details/gjnqhsjkk.sHtML

files=$(ls -1)
来源：http://m.share.yfazqb.com/Article/details/gcmkuumfe.sHtML

[R38] 管道串联
来源：http://www.m.share.vehdjk.com/Article/details/gjkfscqtz.sHtML

cat a.txt | grep -i error | wc -l
来源：http://baike.vehdjk.com/Article/details/grpwfktao.sHtML

[R39] 重定向标准输出与错误
来源：http://baike.tarul.cn/Article/details/gmybvmswi.sHtML

cmd > out.log 2>&1
来源：http://baike.yfazqb.com/Article/details/gdfzjeuev.sHtML

[R40] 追加写日志
来源：http://blog.epnwcf.com/Article/details/gkzodwbuy.sHtML

echo "log" >> out.log
来源：http://www.share.tarul.cn/Article/details/gjbgehwmr.sHtML

[R41] 丢弃输出
来源：http://3g.tarul.cn/Article/details/gtgaqjoye.sHtML

cmd >/dev/null 2>&1
来源：http://m.share.epnwcf.com/Article/details/gndklffcy.sHtML

[R42] 输入重定向
来源：http://read.share.epnwcf.com/Article/details/gkknmxgpq.sHtML

wc -l < a.txt
来源：http://baike.sjlbkw.cn/Article/details/gijduvgus.sHtML

[R43] 按名字查找文件
来源：http://wap.sjlbkw.cn/Article/details/gzdnmnyqo.sHtML

find . -name "*.log" -type f
来源：http://mobile.bbcook.cn/Article/details/gogxxrsrr.sHtML

[R44] 按修改时间查找
来源：http://3g.sjlbkw.cn/Article/details/gudmyaofh.sHtML

find . -mtime -7 -type f
来源：http://www.share.fktsv.cn/Article/details/gjsnwqjkv.sHtML

[R45] 批量删除
来源：http://www.m.share.bbcook.cn/Article/details/ggpqmwsbu.sHtML

find . -name "*.tmp" -delete
来源：http://read.share.yfazqb.com/Article/details/gnmajagwz.sHtML

[R46] 递归替换文件内容
来源：http://www.m.share.fktsv.cn/Article/details/gwjxevlux.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.blog.vehdjk.com/Article/details/gmyuusmir.sHtML

[R47] sed 单行替换
来源：http://read.share.sjlbkw.cn/Article/details/ghzcualbj.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://3g.sjlbkw.cn/Article/details/goejpnarw.sHtML

[R48] awk 取指定列
来源：http://mobile.epnwcf.com/Article/details/gkcwuoftb.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.blog.yfazqb.com/Article/details/gsxgtihvt.sHtML

[R49] awk 带条件
来源：http://www.blog.tarul.cn/Article/details/ggcqekkuf.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://blog.epnwcf.com/Article/details/gayjsmoyf.sHtML

[R50] awk 求和
来源：http://baike.fktsv.cn/Article/details/gnbrrorkn.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.share.epnwcf.com/Article/details/gdezpikpf.sHtML

[R51] 排序去重取前几
来源：http://blog.tarul.cn/Article/details/gxujeguhh.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.blog.yfazqb.com/Article/details/gwapxrasf.sHtML

[R52] 统计行数
来源：http://baike.fktsv.cn/Article/details/gveuqnqsj.sHtML

wc -l a.txt
来源：http://mobile.yfazqb.com/Article/details/gshhpwcny.sHtML

[R53] 查看文件头与实时尾
来源：http://www.m.share.epnwcf.com/Article/details/gddqypeys.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://blog.fktsv.cn/Article/details/geamvgssl.sHtML

[R54] 比较两个文件
来源：http://read.share.fktsv.cn/Article/details/glyxxcwrw.sHtML

diff a.txt b.txt
来源：http://3g.vehdjk.com/Article/details/gjhbgucal.sHtML

[R55] 压缩与解压
来源：http://www.blog.epnwcf.com/Article/details/giqjfkzmq.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://m.share.tarul.cn/Article/details/gplokllon.sHtML

[R56] 远程拷贝
来源：http://www.m.share.yfazqb.com/Article/details/gespgflrr.sHtML

scp file user@host:/path/
来源：http://read.share.fktsv.cn/Article/details/ghnnfjmul.sHtML

[R57] 远程执行命令
来源：http://blog.tarul.cn/Article/details/gqnjzwhht.sHtML

ssh user@host 'uptime'
来源：http://wap.sjlbkw.cn/Article/details/gpaigynbg.sHtML

[R58] 下载文件
来源：http://read.share.vehdjk.com/Article/details/gobdztrxv.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://m.share.sjlbkw.cn/Article/details/gzaaugkiv.sHtML

[R59] 发 POST JSON
来源：http://mobile.sjlbkw.cn/Article/details/gjrhommal.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wap.bbcook.cn/Article/details/goayqgpjz.sHtML

[R60] 只看 HTTP 状态码
来源：http://baike.epnwcf.com/Article/details/gfuwdsvcd.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://read.share.epnwcf.com/Article/details/gnkowspts.sHtML

[R61] 磁盘占用
来源：http://blog.fktsv.cn/Article/details/gdrfigsxf.sHtML

df -h;  du -sh *
来源：http://wap.vehdjk.com/Article/details/gzfkfljqn.sHtML

[R62] 找最占空间的文件
来源：http://baike.tarul.cn/Article/details/gnrbhvxzz.sHtML

du -ah . | sort -rh | head -10
来源：http://blog.yfazqb.com/Article/details/gulycvszr.sHtML

[R63] 内存与进程
来源：http://www.share.bbcook.cn/Article/details/ghgzsougz.sHtML

free -h;  ps aux | grep nginx
来源：http://www.blog.epnwcf.com/Article/details/gawbryatj.sHtML

[R64] 结束进程
来源：http://www.blog.fktsv.cn/Article/details/giqxhklly.sHtML

kill -9 $(pgrep -f app.py)
来源：http://m.share.vehdjk.com/Article/details/godbupygd.sHtML

[R65] 查看端口占用
来源：http://m.share.epnwcf.com/Article/details/gsvrabdut.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://blog.vehdjk.com/Article/details/gfajfbkva.sHtML

[R66] 定时任务
来源：http://blog.bbcook.cn/Article/details/gdmoqgvzg.sHtML

crontab -e;  crontab -l
来源：http://3g.vehdjk.com/Article/details/genyqwmrc.sHtML

[R67] 生成随机十六进制串
来源：http://mobile.yfazqb.com/Article/details/gmpdxuwlp.sHtML

openssl rand -hex 16
来源：http://read.share.epnwcf.com/Article/details/gsiuggnkh.sHtML

[R68] 计算文件校验值
来源：http://3g.sjlbkw.cn/Article/details/gfjlqnwxa.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://baike.vehdjk.com/Article/details/gkasrrdkh.sHtML

[R69] 生成随机密码
来源：http://3g.tarul.cn/Article/details/glbhrmxqa.sHtML

head -c 16 /dev/urandom | base64
来源：http://blog.yfazqb.com/Article/details/grerqlmnv.sHtML

[R70] 时间戳与互转
来源：http://mobile.epnwcf.com/Article/details/gabdpjmhk.sHtML

date +%s;  date -d @1700000000
来源：http://www.share.vehdjk.com/Article/details/gmrydlhvc.sHtML

[R71] 日期格式化
来源：http://m.share.vehdjk.com/Article/details/gfckdtftf.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.share.tarul.cn/Article/details/gmmzvkrqc.sHtML

[R72] 等待端口就绪
来源：http://read.share.bbcook.cn/Article/details/gxgujgqtp.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.blog.tarul.cn/Article/details/gfgztubev.sHtML

[R73] 分割大日志
来源：http://mobile.bbcook.cn/Article/details/grripscks.sHtML

split -l 1000 big.log part_
来源：http://mobile.yfazqb.com/Article/details/gdrtqfiie.sHtML

[R74] 批量重命名
来源：http://3g.tarul.cn/Article/details/gikwpwicl.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://mobile.tarul.cn/Article/details/geeabcxxr.sHtML

[R75] 导出环境变量
来源：http://wap.epnwcf.com/Article/details/gfhxvnoux.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.m.share.tarul.cn/Article/details/gpbdrxlwe.sHtML

[R76] 使用临时文件
来源：http://blog.fktsv.cn/Article/details/gomordxej.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.tarul.cn/Article/details/gltlfbryr.sHtML

[R77] 读取用户输入
来源：http://m.share.fktsv.cn/Article/details/gbhfybbtu.sHtML

read -rp "请输入: " ans
来源：http://www.blog.tarul.cn/Article/details/gxtcpicrw.sHtML

[R78] 交互式菜单
来源：http://3g.tarul.cn/Article/details/gwuirvuup.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://mobile.yfazqb.com/Article/details/guhxzhcmt.sHtML

[R79] 解析命令行选项
来源：http://3g.tarul.cn/Article/details/gkltmsbhp.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://baike.yfazqb.com/Article/details/goxcgraxe.sHtML

[R80] 查看脚本执行耗时
来源：http://3g.tarul.cn/Article/details/gcgpmvtvg.sHtML

time ./run.sh
来源：http://www.blog.sjlbkw.cn/Article/details/gbjgwndfz.sHtML

================================================================================
来源：http://mobile.epnwcf.com/Article/details/gvwgiaxuk.sHtML

S. C / C++ 专题
来源：http://baike.yfazqb.com/Article/details/ghmzksvta.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/gfgodmkmj.sHtML

[S01] C：Hello World
来源：http://m.share.bbcook.cn/Article/details/gzddgteee.sHtML

#include <stdio.h>
来源：http://m.share.yfazqb.com/Article/details/gobgqotev.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.blog.bbcook.cn/Article/details/gcrkfuzis.sHtML

[S02] C：变量与格式化输出
来源：http://baike.fktsv.cn/Article/details/gvvteckcy.sHtML

int a = 10; printf("%d\n", a);
来源：http://3g.tarul.cn/Article/details/getsgapcy.sHtML

[S03] C：读入整数
来源：http://www.blog.bbcook.cn/Article/details/gijgfgmmd.sHtML

int x; scanf("%d", &x);
来源：http://www.m.share.epnwcf.com/Article/details/gsxrczgkw.sHtML

[S04] C：字符串复制
来源：http://blog.bbcook.cn/Article/details/ghgkjtltk.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://baike.sjlbkw.cn/Article/details/gqehftfqo.sHtML

[S05] C：字符串长度
来源：http://wap.vehdjk.com/Article/details/gxvruncgq.sHtML

strlen(s)
来源：http://baike.sjlbkw.cn/Article/details/gzgxmvijt.sHtML

[S06] C：字符串比较
来源：http://3g.tarul.cn/Article/details/gzmtgttnk.sHtML

strcmp(a, b) == 0
来源：http://www.blog.yfazqb.com/Article/details/gltsiuqqg.sHtML

[S07] C：数组遍历求和
来源：http://www.blog.yfazqb.com/Article/details/gawfcvxyt.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://3g.sjlbkw.cn/Article/details/glbzzdgnv.sHtML

[S08] C：动态内存分配与释放
来源：http://www.m.share.tarul.cn/Article/details/gxtdmhipq.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.m.share.yfazqb.com/Article/details/gknvqyimq.sHtML

[S09] C：结构体定义与初始化
来源：http://baike.yfazqb.com/Article/details/gvfdxxahq.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://blog.vehdjk.com/Article/details/gbupifiws.sHtML

[S10] C：指针与解引用
来源：http://wap.bbcook.cn/Article/details/gazmkwhaj.sHtML

int *p = &a;  *p = 5;
来源：http://mobile.yfazqb.com/Article/details/gudnrpajo.sHtML

[S11] C：逐行读文件
来源：http://www.share.bbcook.cn/Article/details/gonqkaxmh.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.m.share.tarul.cn/Article/details/gblaibtsd.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://mobile.epnwcf.com/Article/details/gvrnbhshe.sHtML

fclose(f);
来源：http://3g.fktsv.cn/Article/details/glenfvaru.sHtML

[S12] C：写文件
来源：http://baike.sjlbkw.cn/Article/details/gptyatgdd.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.m.share.bbcook.cn/Article/details/genuyojsb.sHtML

[S13] C：宏定义
来源：http://baike.sjlbkw.cn/Article/details/gsyxfftxk.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wap.sjlbkw.cn/Article/details/grelwvfcx.sHtML

[S14] C：枚举
来源：http://mobile.vehdjk.com/Article/details/gfswqbgtq.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://mobile.bbcook.cn/Article/details/gzfxibojw.sHtML

[S15] C：类型转换
来源：http://www.blog.yfazqb.com/Article/details/gmtgjtrxc.sHtML

(double) a / b
来源：http://3g.vehdjk.com/Article/details/gcywxfnmu.sHtML

[S16] C：位操作置位
来源：http://www.blog.fktsv.cn/Article/details/gubcjjukz.sHtML

x |= (1 << 3);
来源：http://m.share.tarul.cn/Article/details/ggzvqwcfs.sHtML

[S17] C：安全拼接字符串
来源：http://mobile.yfazqb.com/Article/details/geppcwipi.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://read.share.bbcook.cn/Article/details/gehsjkwov.sHtML

[S18] C：命令行参数
来源：http://www.m.share.vehdjk.com/Article/details/guekyseqo.sHtML

int main(int argc, char **argv)
来源：http://read.share.epnwcf.com/Article/details/gbrxhcaly.sHtML

[S19] C：快速排序
来源：http://www.m.share.yfazqb.com/Article/details/gvhnohjjd.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.blog.bbcook.cn/Article/details/gaaoxnheo.sHtML

[S20] C：二分查找
来源：http://wap.tarul.cn/Article/details/gebjgtfsp.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://read.share.epnwcf.com/Article/details/gswphyqte.sHtML

[S21] C：字符类别判断
来源：http://www.blog.yfazqb.com/Article/details/gxxqqzcam.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://3g.epnwcf.com/Article/details/gevpoxsoh.sHtML

[S22] C：字符串转数字
来源：http://blog.yfazqb.com/Article/details/gskhrytfl.sHtML


<!-- 参考信息 -->