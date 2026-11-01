代发 wailian999

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.blog.fktsv.cn/Article/details/gqgllktmq.sHtML

[Q58] 累计求和
来源：http://wap.fktsv.cn/Article/details/gqtnpgbfp.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.share.fktsv.cn/Article/details/gigxxnmrr.sHtML

[Q59] 分组内累计
来源：http://www.share.epnwcf.com/Article/details/ghaeeugiv.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://mobile.vehdjk.com/Article/details/ghcqfdqur.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.blog.bbcook.cn/Article/details/gdvbmddix.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://m.share.epnwcf.com/Article/details/gvjpalnfp.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.blog.bbcook.cn/Article/details/glrjsjhbc.sHtML

[Q61] 移动平均
来源：http://m.share.vehdjk.com/Article/details/gurebuqox.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.share.sjlbkw.cn/Article/details/grfcyflfg.sHtML

[Q62] 分组占比
来源：http://www.share.yfazqb.com/Article/details/gcmwfzfdb.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.share.epnwcf.com/Article/details/gphuhbxys.sHtML

[Q63] 开启事务
来源：http://mobile.yfazqb.com/Article/details/gpsebcsrx.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://m.share.fktsv.cn/Article/details/geucbrbms.sHtML

[Q64] 提交事务
来源：http://3g.tarul.cn/Article/details/gsfibymhu.sHtML

COMMIT;
来源：http://www.blog.fktsv.cn/Article/details/ghotpoibf.sHtML

[Q65] 回滚事务
来源：http://www.m.share.epnwcf.com/Article/details/gcilhlerr.sHtML

ROLLBACK;
来源：http://mobile.sjlbkw.cn/Article/details/gcnqtndaj.sHtML

[Q66] 行锁查询
来源：http://baike.fktsv.cn/Article/details/gvsuynarh.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.share.vehdjk.com/Article/details/gamwrrhjg.sHtML

[Q67] 设置隔离级别
来源：http://baike.epnwcf.com/Article/details/gwvxtbtfd.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://mobile.epnwcf.com/Article/details/gvehathpc.sHtML

[Q68] 保存点
来源：http://www.blog.bbcook.cn/Article/details/gfgniyqgo.sHtML

SAVEPOINT sp1;
来源：http://m.share.sjlbkw.cn/Article/details/gogtfnmkm.sHtML

ROLLBACK TO sp1;
来源：http://blog.fktsv.cn/Article/details/gdzuqtdyy.sHtML

[Q69] 查看执行计划
来源：http://baike.fktsv.cn/Article/details/grtiorgol.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://wap.epnwcf.com/Article/details/getqtnpog.sHtML

[Q70] 更新统计信息
来源：http://wap.fktsv.cn/Article/details/gblpejwvp.sHtML

ANALYZE TABLE users;
来源：http://wap.yfazqb.com/Article/details/gerrpehvq.sHtML

[Q71] 查看建表语句
来源：http://read.share.bbcook.cn/Article/details/gwtuzodat.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://3g.fktsv.cn/Article/details/gblayenyh.sHtML

[Q72] 查看索引
来源：http://m.share.yfazqb.com/Article/details/gggqoesij.sHtML

SHOW INDEX FROM users;
来源：http://read.share.epnwcf.com/Article/details/gpxqlijta.sHtML

[Q73] 查看表状态
来源：http://www.m.share.yfazqb.com/Article/details/gioucjpfu.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://m.share.sjlbkw.cn/Article/details/goqvwoczz.sHtML

[Q74] 强制使用索引
来源：http://wap.yfazqb.com/Article/details/gpkpojmhq.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.m.share.bbcook.cn/Article/details/gowusbqqf.sHtML

[Q75] 日期格式化
来源：http://www.blog.tarul.cn/Article/details/gvbvfbgyz.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://m.share.vehdjk.com/Article/details/gafhvcykw.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://baike.tarul.cn/Article/details/gtmydzzdu.sHtML

[Q76] 按天统计
来源：http://www.m.share.vehdjk.com/Article/details/gvmwhdjkw.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://baike.tarul.cn/Article/details/girojjkuf.sHtML

[Q77] 时间加减
来源：http://wap.tarul.cn/Article/details/gmakxpxyr.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://read.share.yfazqb.com/Article/details/gldrtjrbb.sHtML

[Q78] 当前时间
来源：http://m.share.epnwcf.com/Article/details/gbyewvjet.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://m.share.yfazqb.com/Article/details/gvxqrgcyo.sHtML

[Q79] 字符串拼接
来源：http://mobile.sjlbkw.cn/Article/details/gzsojyghs.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://mobile.vehdjk.com/Article/details/grirrxynb.sHtML

[Q80] 字符串截取
来源：http://www.m.share.tarul.cn/Article/details/gitxabubi.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://mobile.bbcook.cn/Article/details/gfkumqzpl.sHtML

[Q81] 字符串替换
来源：http://baike.fktsv.cn/Article/details/gcpuprrza.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://mobile.tarul.cn/Article/details/gtmslwmtv.sHtML

[Q82] 字符长度与字节长度
来源：http://www.m.share.yfazqb.com/Article/details/ghfvmchoa.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://m.share.epnwcf.com/Article/details/ggatcehjz.sHtML

[Q83] 大小写转换
来源：http://blog.epnwcf.com/Article/details/gxpnrmnay.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.blog.tarul.cn/Article/details/gxtzhdiqd.sHtML

[Q84] 去除首尾空格
来源：http://www.blog.sjlbkw.cn/Article/details/gzfhxewue.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.share.vehdjk.com/Article/details/gqwhpcorm.sHtML

[Q85] 数值取整
来源：http://read.share.sjlbkw.cn/Article/details/gatohvgsd.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://baike.tarul.cn/Article/details/gjwcoslgg.sHtML

[Q86] 读取 JSON 字段
来源：http://www.blog.fktsv.cn/Article/details/gyifujxan.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.blog.vehdjk.com/Article/details/glffpynnq.sHtML

[Q87] JSON 字段做条件
来源：http://www.share.tarul.cn/Article/details/gzxfeoqiz.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.blog.yfazqb.com/Article/details/grxdzcrfk.sHtML

[Q88] 行转列（条件聚合）
来源：http://mobile.bbcook.cn/Article/details/gyrewocoq.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://mobile.fktsv.cn/Article/details/glavhvvus.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.blog.vehdjk.com/Article/details/gvfrsdvsp.sHtML

[Q89] 判断表是否存在
来源：http://www.m.share.vehdjk.com/Article/details/gudbdlktf.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://read.share.yfazqb.com/Article/details/gzauuzese.sHtML

[Q90] 生成序号列
来源：http://read.share.sjlbkw.cn/Article/details/guvkklpac.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://wap.vehdjk.com/Article/details/gjsceabtm.sHtML

================================================================================
来源：http://3g.vehdjk.com/Article/details/gvekwqhjv.sHtML

R. Bash 专题
来源：http://www.share.fktsv.cn/Article/details/gubokawlm.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/guvkvvkna.sHtML

[R01] shebang 与严格模式
来源：http://m.share.vehdjk.com/Article/details/gozaybdlo.sHtML

#!/usr/bin/env bash
来源：http://baike.vehdjk.com/Article/details/gkzuquurf.sHtML

set -euo pipefail
来源：http://read.share.vehdjk.com/Article/details/gabhatsme.sHtML

[R02] 变量赋值与使用
来源：http://www.m.share.bbcook.cn/Article/details/gnwkzcdpu.sHtML

name="Tom"; echo "$name"
来源：http://blog.epnwcf.com/Article/details/gfliltmwr.sHtML

[R03] 只读变量
来源：http://m.share.yfazqb.com/Article/details/ggzsnesgw.sHtML

readonly PI=3.14
来源：http://www.share.epnwcf.com/Article/details/guglxlkfs.sHtML

[R04] 位置参数
来源：http://wap.yfazqb.com/Article/details/gewjpyuvr.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://m.share.yfazqb.com/Article/details/gkdzmvjkt.sHtML

[R05] 参数默认值
来源：http://blog.tarul.cn/Article/details/gqgjremxw.sHtML

name="${1:-default}"
来源：http://www.blog.yfazqb.com/Article/details/gcdimhkhj.sHtML

[R06] 判断命令是否存在
来源：http://www.blog.bbcook.cn/Article/details/gdontbysc.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://read.share.tarul.cn/Article/details/ggcfteabr.sHtML

[R07] if 判断文件
来源：http://www.m.share.sjlbkw.cn/Article/details/glkrwzjbp.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.m.share.epnwcf.com/Article/details/gzrogyinb.sHtML

[R08] 数值比较
来源：http://www.blog.fktsv.cn/Article/details/gyhqzbsij.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.blog.vehdjk.com/Article/details/ggbajerib.sHtML

[R09] 字符串比较
来源：http://www.share.yfazqb.com/Article/details/gleesgzjg.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.m.share.yfazqb.com/Article/details/gowmhgfsq.sHtML

[R10] 正则匹配
来源：http://3g.fktsv.cn/Article/details/glrijrijf.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.m.share.sjlbkw.cn/Article/details/glbwztlvo.sHtML

[R11] case 多分支
来源：http://wap.epnwcf.com/Article/details/gqkykqxah.sHtML

case "$1" in
来源：http://read.share.fktsv.cn/Article/details/gslzlwfci.sHtML

start) echo "启动" ;;
来源：http://blog.fktsv.cn/Article/details/girxxulcj.sHtML

stop)  echo "停止" ;;
来源：http://read.share.sjlbkw.cn/Article/details/gloidlelf.sHtML

*)     echo "未知命令" ;;
来源：http://3g.tarul.cn/Article/details/gzildfiwe.sHtML

esac
来源：http://www.blog.fktsv.cn/Article/details/godxcrwws.sHtML

[R12] for 遍历文件
来源：http://m.share.tarul.cn/Article/details/gctirdyyi.sHtML

for f in *.txt; do echo "$f"; done
来源：http://baike.tarul.cn/Article/details/gzaudddrg.sHtML

[R13] for 计数循环
来源：http://blog.bbcook.cn/Article/details/gpmcknoza.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://baike.bbcook.cn/Article/details/gwxzodwfo.sHtML

[R14] C 风格 for
来源：http://www.blog.yfazqb.com/Article/details/gozmshixv.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://blog.epnwcf.com/Article/details/gjavmiivh.sHtML

[R15] while 逐行读文件
来源：http://3g.bbcook.cn/Article/details/gfqcxxbef.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.share.vehdjk.com/Article/details/gpnhpvsyy.sHtML

[R16] until 等待条件
来源：http://baike.fktsv.cn/Article/details/gpovljxdf.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.m.share.tarul.cn/Article/details/gbcyeunop.sHtML

[R17] 数组定义与取值
来源：http://3g.tarul.cn/Article/details/gaukpgrvq.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://baike.vehdjk.com/Article/details/gfjjmbkdk.sHtML

[R18] 遍历数组
来源：http://wap.fktsv.cn/Article/details/gcynsefon.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://m.share.tarul.cn/Article/details/gxaffmgyt.sHtML

[R19] 数组长度
来源：http://read.share.bbcook.cn/Article/details/geuabsqqs.sHtML

echo "${#arr[@]}"
来源：http://www.blog.tarul.cn/Article/details/ggoqntqkd.sHtML

[R20] 关联数组（字典）
来源：http://www.blog.tarul.cn/Article/details/gdtxzcdbk.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.m.share.epnwcf.com/Article/details/gpjdnezxd.sHtML

[R21] 字符串长度
来源：http://www.share.epnwcf.com/Article/details/gksylzrlu.sHtML

echo "${#s}"
来源：http://mobile.epnwcf.com/Article/details/gfyfhoamf.sHtML

[R22] 截取子串
来源：http://baike.bbcook.cn/Article/details/gsufismrm.sHtML

echo "${s:0:5}"
来源：http://wap.epnwcf.com/Article/details/gusqjfbob.sHtML

[R23] 字符串替换
来源：http://3g.fktsv.cn/Article/details/gaegfdnqc.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.m.share.tarul.cn/Article/details/gwjeznlby.sHtML

[R24] 大小写转换
来源：http://www.m.share.sjlbkw.cn/Article/details/gekoaxtdl.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://wap.sjlbkw.cn/Article/details/gzxqqrlzw.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.m.share.yfazqb.com/Article/details/glzwcytio.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://mobile.vehdjk.com/Article/details/gzdywnpek.sHtML

[R26] 命令替换
来源：http://wap.epnwcf.com/Article/details/gspebeuwd.sHtML

now=$(date +%F); echo "$now"
来源：http://read.share.vehdjk.com/Article/details/gzdvevznw.sHtML

[R27] 算术展开
来源：http://read.share.yfazqb.com/Article/details/gwirtdaqk.sHtML

echo $((1 + 2 * 3))
来源：http://baike.tarul.cn/Article/details/guajsykmv.sHtML

[R28] 浮点运算
来源：http://www.blog.fktsv.cn/Article/details/gdjpyntnv.sHtML

echo "scale=2; 10/3" | bc
来源：http://mobile.tarul.cn/Article/details/ghhzinvvx.sHtML

[R29] 定义函数
来源：http://m.share.yfazqb.com/Article/details/gaubxzgmx.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://read.share.yfazqb.com/Article/details/gxrediide.sHtML

[R30] 函数返回状态码
来源：http://read.share.vehdjk.com/Article/details/gfwcvhmpd.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://m.share.tarul.cn/Article/details/gmdffnzqk.sHtML

[R31] 局部变量
来源：http://mobile.vehdjk.com/Article/details/gfvbtshoh.sHtML

f() { local x=1; echo "$x"; }
来源：http://read.share.vehdjk.com/Article/details/gcxizgyam.sHtML

[R32] 参数个数校验
来源：http://www.blog.yfazqb.com/Article/details/grvstfiik.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://wap.fktsv.cn/Article/details/gqgkbkvcu.sHtML

[R33] 捕获错误并提示行号
来源：http://read.share.vehdjk.com/Article/details/ghavssqlf.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://mobile.tarul.cn/Article/details/guifhetup.sHtML

[R34] 退出时清理
来源：http://www.share.vehdjk.com/Article/details/gwqurlipa.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://mobile.yfazqb.com/Article/details/gcciacrow.sHtML

[R35] 后台执行并等待
来源：http://www.blog.bbcook.cn/Article/details/gfgwnrcmr.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://baike.fktsv.cn/Article/details/gqclodvmb.sHtML

[R36] 并发执行多个任务
来源：http://www.blog.bbcook.cn/Article/details/gwoamgugj.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://blog.sjlbkw.cn/Article/details/ggqaeggzi.sHtML

[R37] 把输出赋给变量
来源：http://read.share.sjlbkw.cn/Article/details/gbmiqdenz.sHtML

files=$(ls -1)
来源：http://blog.bbcook.cn/Article/details/gbrpawddr.sHtML

[R38] 管道串联
来源：http://m.share.fktsv.cn/Article/details/gfghbujgd.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.m.share.yfazqb.com/Article/details/gmjdtyvzk.sHtML

[R39] 重定向标准输出与错误
来源：http://blog.epnwcf.com/Article/details/gvzcqkcxx.sHtML

cmd > out.log 2>&1
来源：http://www.share.epnwcf.com/Article/details/gpcffbgaq.sHtML

[R40] 追加写日志
来源：http://wap.vehdjk.com/Article/details/gkhsxkzhy.sHtML

echo "log" >> out.log
来源：http://m.share.vehdjk.com/Article/details/ggycuikfa.sHtML

[R41] 丢弃输出
来源：http://3g.fktsv.cn/Article/details/gjpgxhycs.sHtML

cmd >/dev/null 2>&1
来源：http://www.share.epnwcf.com/Article/details/gxniareia.sHtML

[R42] 输入重定向
来源：http://mobile.sjlbkw.cn/Article/details/gobxglraf.sHtML

wc -l < a.txt
来源：http://3g.yfazqb.com/Article/details/gzphbgwdh.sHtML

[R43] 按名字查找文件
来源：http://m.share.tarul.cn/Article/details/gucuyijlc.sHtML

find . -name "*.log" -type f
来源：http://3g.vehdjk.com/Article/details/gvpimxypp.sHtML

[R44] 按修改时间查找
来源：http://www.share.fktsv.cn/Article/details/gokiewrke.sHtML

find . -mtime -7 -type f
来源：http://www.blog.fktsv.cn/Article/details/gpvkwavbj.sHtML

[R45] 批量删除
来源：http://read.share.tarul.cn/Article/details/gojsuhorm.sHtML

find . -name "*.tmp" -delete
来源：http://3g.yfazqb.com/Article/details/gtnffcqcl.sHtML

[R46] 递归替换文件内容
来源：http://read.share.epnwcf.com/Article/details/geakfbcso.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mobile.bbcook.cn/Article/details/gaajamckz.sHtML

[R47] sed 单行替换
来源：http://www.share.epnwcf.com/Article/details/gqxqszasr.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://wap.fktsv.cn/Article/details/gvlwnvttp.sHtML

[R48] awk 取指定列
来源：http://mobile.epnwcf.com/Article/details/gckozesvn.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.m.share.tarul.cn/Article/details/gqikiouzn.sHtML

[R49] awk 带条件
来源：http://www.m.share.tarul.cn/Article/details/gcmopppuc.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.share.sjlbkw.cn/Article/details/gknmuvkve.sHtML

[R50] awk 求和
来源：http://www.blog.epnwcf.com/Article/details/gkcwexevt.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://3g.yfazqb.com/Article/details/gcvbktebm.sHtML

[R51] 排序去重取前几
来源：http://wap.yfazqb.com/Article/details/gmpwplnce.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://baike.epnwcf.com/Article/details/goylazhrx.sHtML

[R52] 统计行数
来源：http://m.share.vehdjk.com/Article/details/gugqltrob.sHtML

wc -l a.txt
来源：http://m.share.yfazqb.com/Article/details/gqdndhvbh.sHtML

[R53] 查看文件头与实时尾
来源：http://mobile.fktsv.cn/Article/details/gtelzcpyv.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://baike.fktsv.cn/Article/details/gubxzrofe.sHtML

[R54] 比较两个文件
来源：http://baike.fktsv.cn/Article/details/gwthnymyd.sHtML

diff a.txt b.txt
来源：http://mobile.fktsv.cn/Article/details/gnraouicv.sHtML

[R55] 压缩与解压
来源：http://blog.fktsv.cn/Article/details/gpjygwjnp.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.m.share.bbcook.cn/Article/details/glpanvrlj.sHtML

[R56] 远程拷贝
来源：http://baike.vehdjk.com/Article/details/geyhrcdpo.sHtML

scp file user@host:/path/
来源：http://wap.epnwcf.com/Article/details/gtezchpgk.sHtML

[R57] 远程执行命令
来源：http://www.share.tarul.cn/Article/details/gwwtgylso.sHtML

ssh user@host 'uptime'
来源：http://baike.epnwcf.com/Article/details/ghzejwlni.sHtML

[R58] 下载文件
来源：http://mobile.epnwcf.com/Article/details/gfyllpdrr.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://3g.fktsv.cn/Article/details/gkuuoczoe.sHtML

[R59] 发 POST JSON
来源：http://blog.yfazqb.com/Article/details/gjnteqdrj.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://read.share.bbcook.cn/Article/details/gnfzglaxt.sHtML

[R60] 只看 HTTP 状态码
来源：http://3g.sjlbkw.cn/Article/details/gpftedjub.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://3g.tarul.cn/Article/details/gqmibrrbz.sHtML

[R61] 磁盘占用
来源：http://wap.tarul.cn/Article/details/gyhqjywip.sHtML

df -h;  du -sh *
来源：http://mobile.tarul.cn/Article/details/goiojcvde.sHtML

[R62] 找最占空间的文件
来源：http://baike.tarul.cn/Article/details/gflizzueb.sHtML

du -ah . | sort -rh | head -10
来源：http://read.share.fktsv.cn/Article/details/gslyubuyf.sHtML

[R63] 内存与进程
来源：http://www.share.fktsv.cn/Article/details/ghnczewmo.sHtML

free -h;  ps aux | grep nginx
来源：http://m.share.tarul.cn/Article/details/gqlkjqqql.sHtML

[R64] 结束进程
来源：http://baike.bbcook.cn/Article/details/giycjdedr.sHtML

kill -9 $(pgrep -f app.py)
来源：http://baike.epnwcf.com/Article/details/gawwjnsav.sHtML

[R65] 查看端口占用
来源：http://3g.bbcook.cn/Article/details/gxgzxhsnc.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://blog.yfazqb.com/Article/details/gedxqfpue.sHtML

[R66] 定时任务
来源：http://m.share.epnwcf.com/Article/details/gvmclufmp.sHtML

crontab -e;  crontab -l
来源：http://www.share.epnwcf.com/Article/details/gzkfsclro.sHtML

[R67] 生成随机十六进制串
来源：http://3g.yfazqb.com/Article/details/gafsqbaqz.sHtML

openssl rand -hex 16
来源：http://3g.bbcook.cn/Article/details/gxrcjxsra.sHtML

[R68] 计算文件校验值
来源：http://read.share.fktsv.cn/Article/details/gtqwufxat.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://3g.fktsv.cn/Article/details/gpzqpflyb.sHtML

[R69] 生成随机密码
来源：http://read.share.tarul.cn/Article/details/gnsoooekz.sHtML

head -c 16 /dev/urandom | base64
来源：http://baike.vehdjk.com/Article/details/grqqftuep.sHtML

[R70] 时间戳与互转
来源：http://www.m.share.vehdjk.com/Article/details/ghzfxzdvz.sHtML

date +%s;  date -d @1700000000
来源：http://www.share.vehdjk.com/Article/details/gdihodztc.sHtML

[R71] 日期格式化
来源：http://mobile.vehdjk.com/Article/details/glxuxadau.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://read.share.fktsv.cn/Article/details/gckpvddbg.sHtML

[R72] 等待端口就绪
来源：http://blog.yfazqb.com/Article/details/gfeuuimyh.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.m.share.tarul.cn/Article/details/gulowewce.sHtML

[R73] 分割大日志
来源：http://wap.bbcook.cn/Article/details/ggkyagtws.sHtML

split -l 1000 big.log part_
来源：http://baike.sjlbkw.cn/Article/details/glutqfkzm.sHtML

[R74] 批量重命名
来源：http://www.share.sjlbkw.cn/Article/details/gqdqfuvxj.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://m.share.yfazqb.com/Article/details/gebxtwwix.sHtML

[R75] 导出环境变量
来源：http://blog.vehdjk.com/Article/details/gndquhvns.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.blog.bbcook.cn/Article/details/grjuwnviu.sHtML

[R76] 使用临时文件
来源：http://www.share.bbcook.cn/Article/details/gigqspode.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://3g.sjlbkw.cn/Article/details/gfieopufm.sHtML

[R77] 读取用户输入
来源：http://m.share.tarul.cn/Article/details/gylhrvamr.sHtML

read -rp "请输入: " ans
来源：http://mobile.fktsv.cn/Article/details/gzyisbvga.sHtML

[R78] 交互式菜单
来源：http://www.share.bbcook.cn/Article/details/gihwxopsg.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.m.share.vehdjk.com/Article/details/gcggenwfn.sHtML

[R79] 解析命令行选项
来源：http://m.share.sjlbkw.cn/Article/details/gnaskhixo.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mobile.vehdjk.com/Article/details/ggbdxqmzb.sHtML

[R80] 查看脚本执行耗时
来源：http://baike.epnwcf.com/Article/details/gydtorasi.sHtML

time ./run.sh
来源：http://m.share.epnwcf.com/Article/details/gtfbwjcjr.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/gwgoqnvyw.sHtML

S. C / C++ 专题
来源：http://www.m.share.bbcook.cn/Article/details/gljpaxqdw.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/ghhlglvrm.sHtML

[S01] C：Hello World
来源：http://read.share.bbcook.cn/Article/details/gdwsdkkbp.sHtML

#include <stdio.h>
来源：http://baike.fktsv.cn/Article/details/gyijrxhrw.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.share.vehdjk.com/Article/details/glemmhcih.sHtML

[S02] C：变量与格式化输出
来源：http://baike.tarul.cn/Article/details/gsdpadixj.sHtML

int a = 10; printf("%d\n", a);
来源：http://3g.bbcook.cn/Article/details/gtjndsodu.sHtML

[S03] C：读入整数
来源：http://www.share.bbcook.cn/Article/details/gtnqnvibv.sHtML

int x; scanf("%d", &x);
来源：http://m.share.vehdjk.com/Article/details/gwywjuhto.sHtML

[S04] C：字符串复制
来源：http://3g.vehdjk.com/Article/details/gzjzfbvao.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.share.sjlbkw.cn/Article/details/gaeoboszd.sHtML

[S05] C：字符串长度
来源：http://m.share.epnwcf.com/Article/details/gqvbazlvq.sHtML

strlen(s)
来源：http://www.blog.yfazqb.com/Article/details/gvoxqkwyf.sHtML

[S06] C：字符串比较
来源：http://mobile.sjlbkw.cn/Article/details/gtanqmnvs.sHtML

strcmp(a, b) == 0
来源：http://www.share.epnwcf.com/Article/details/glkqxfvre.sHtML

[S07] C：数组遍历求和
来源：http://mobile.epnwcf.com/Article/details/gxnycckbu.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://read.share.epnwcf.com/Article/details/gtgkhuxhl.sHtML

[S08] C：动态内存分配与释放
来源：http://www.m.share.vehdjk.com/Article/details/gvmxaxckb.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://3g.sjlbkw.cn/Article/details/gsrvrpgot.sHtML

[S09] C：结构体定义与初始化
来源：http://blog.yfazqb.com/Article/details/gdwouceve.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://baike.epnwcf.com/Article/details/gtmgbikzu.sHtML

[S10] C：指针与解引用
来源：http://3g.yfazqb.com/Article/details/gkpyuwtxc.sHtML

int *p = &a;  *p = 5;
来源：http://mobile.vehdjk.com/Article/details/gbequpsrq.sHtML

[S11] C：逐行读文件
来源：http://3g.sjlbkw.cn/Article/details/gaadnrppp.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://baike.epnwcf.com/Article/details/gwfascufy.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://mobile.yfazqb.com/Article/details/gdwbrdueh.sHtML

fclose(f);
来源：http://www.share.bbcook.cn/Article/details/galunxfqm.sHtML

[S12] C：写文件
来源：http://www.share.sjlbkw.cn/Article/details/gjzqjcalg.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://3g.bbcook.cn/Article/details/givhpismv.sHtML

[S13] C：宏定义
来源：http://read.share.epnwcf.com/Article/details/gwxawaewh.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wap.bbcook.cn/Article/details/gwyfartwn.sHtML

[S14] C：枚举
来源：http://wap.bbcook.cn/Article/details/goyxkcgtn.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://wap.fktsv.cn/Article/details/gjndsnngl.sHtML

[S15] C：类型转换
来源：http://m.share.yfazqb.com/Article/details/ghbnawato.sHtML

(double) a / b
来源：http://m.share.epnwcf.com/Article/details/ggpsmoqrq.sHtML

[S16] C：位操作置位
来源：http://m.share.yfazqb.com/Article/details/gbnfyjqgc.sHtML

x |= (1 << 3);
来源：http://mobile.yfazqb.com/Article/details/grusnaiaz.sHtML

[S17] C：安全拼接字符串
来源：http://www.share.tarul.cn/Article/details/gwryzinhf.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://3g.tarul.cn/Article/details/gxwaxnadk.sHtML

[S18] C：命令行参数
来源：http://blog.bbcook.cn/Article/details/gkmzepqbn.sHtML

int main(int argc, char **argv)
来源：http://mobile.vehdjk.com/Article/details/gavmihfxq.sHtML

[S19] C：快速排序
来源：http://www.blog.yfazqb.com/Article/details/gklbqtcqo.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.m.share.bbcook.cn/Article/details/gupffojqp.sHtML

[S20] C：二分查找
来源：http://read.share.vehdjk.com/Article/details/gofmvbmdd.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://mobile.vehdjk.com/Article/details/gmzxsowem.sHtML

[S21] C：字符类别判断
来源：http://3g.fktsv.cn/Article/details/gxpwgqruj.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://m.share.fktsv.cn/Article/details/gcfgdvzup.sHtML

[S22] C：字符串转数字
来源：http://blog.yfazqb.com/Article/details/gkxbnjuxz.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.blog.bbcook.cn/Article/details/gsbwvicil.sHtML

[S23] C：随机数
来源：http://www.share.tarul.cn/Article/details/gzfuqsqtw.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://m.share.tarul.cn/Article/details/goiiiygoj.sHtML

[S24] C：获取本地时间
来源：http://3g.fktsv.cn/Article/details/gpxzzepkn.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.share.fktsv.cn/Article/details/geoayzawo.sHtML

[S25] C：内存拷贝
来源：http://read.share.yfazqb.com/Article/details/gvkdmvmhz.sHtML

memcpy(dst, src, n);
来源：http://mobile.sjlbkw.cn/Article/details/gvumqhhbp.sHtML

[S26] C：内存清零
来源：http://mobile.fktsv.cn/Article/details/gnqxdvgpn.sHtML

memset(a, 0, sizeof a);
来源：http://read.share.tarul.cn/Article/details/ghwbhktkl.sHtML

[S27] C：定义常量
来源：http://read.share.fktsv.cn/Article/details/gquqicjzc.sHtML

const double PI = 3.14159;
来源：http://read.share.fktsv.cn/Article/details/ggchkyxpx.sHtML

[S28] C：静态变量
来源：http://www.blog.vehdjk.com/Article/details/gefwrrsvu.sHtML


<!-- 参考信息 -->