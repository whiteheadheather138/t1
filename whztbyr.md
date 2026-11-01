代发 wailian999

[Q61] 移动平均
来源：http://www.share.bbcook.cn/Article/details/gjdmbmlov.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://mobile.bbcook.cn/Article/details/gsmjxrhjf.sHtML

[Q62] 分组占比
来源：http://m.share.bbcook.cn/Article/details/gojeowhgp.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://wap.epnwcf.com/Article/details/grebwsdwy.sHtML

[Q63] 开启事务
来源：http://read.share.bbcook.cn/Article/details/ghqcxtgwj.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://read.share.bbcook.cn/Article/details/gxfterwyp.sHtML

[Q64] 提交事务
来源：http://www.blog.sjlbkw.cn/Article/details/gxcwzpfkp.sHtML

COMMIT;
来源：http://www.share.tarul.cn/Article/details/gzqrtbxct.sHtML

[Q65] 回滚事务
来源：http://3g.yfazqb.com/Article/details/gpaggdtwz.sHtML

ROLLBACK;
来源：http://blog.bbcook.cn/Article/details/gpuykjuif.sHtML

[Q66] 行锁查询
来源：http://www.blog.tarul.cn/Article/details/ghtxrzjtf.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://blog.bbcook.cn/Article/details/gxmdckqgy.sHtML

[Q67] 设置隔离级别
来源：http://wap.bbcook.cn/Article/details/gooerbfyn.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://read.share.epnwcf.com/Article/details/gasymaxyf.sHtML

[Q68] 保存点
来源：http://baike.fktsv.cn/Article/details/gzhbikple.sHtML

SAVEPOINT sp1;
来源：http://blog.tarul.cn/Article/details/gkdgjhicb.sHtML

ROLLBACK TO sp1;
来源：http://blog.fktsv.cn/Article/details/gpeehmjtc.sHtML

[Q69] 查看执行计划
来源：http://www.blog.vehdjk.com/Article/details/gecloqyhl.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://3g.tarul.cn/Article/details/gtupmvpql.sHtML

[Q70] 更新统计信息
来源：http://wap.vehdjk.com/Article/details/grfbdzqay.sHtML

ANALYZE TABLE users;
来源：http://baike.yfazqb.com/Article/details/grqgpeail.sHtML

[Q71] 查看建表语句
来源：http://baike.tarul.cn/Article/details/gmnqglprl.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://baike.tarul.cn/Article/details/gwlzlpndl.sHtML

[Q72] 查看索引
来源：http://www.blog.epnwcf.com/Article/details/grjihbhrf.sHtML

SHOW INDEX FROM users;
来源：http://3g.vehdjk.com/Article/details/gutixpxau.sHtML

[Q73] 查看表状态
来源：http://3g.fktsv.cn/Article/details/gyuwfdmyk.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://mobile.vehdjk.com/Article/details/gjkugpmmi.sHtML

[Q74] 强制使用索引
来源：http://www.blog.sjlbkw.cn/Article/details/gxunoczrj.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.m.share.tarul.cn/Article/details/gowskvoni.sHtML

[Q75] 日期格式化
来源：http://read.share.vehdjk.com/Article/details/gbszsojcs.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://blog.sjlbkw.cn/Article/details/gqakkdclp.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://m.share.bbcook.cn/Article/details/gethwntuj.sHtML

[Q76] 按天统计
来源：http://www.blog.yfazqb.com/Article/details/gfqozyxxz.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://baike.sjlbkw.cn/Article/details/gdaksxqhb.sHtML

[Q77] 时间加减
来源：http://blog.fktsv.cn/Article/details/gphvtdppk.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.m.share.yfazqb.com/Article/details/gkjwwlpov.sHtML

[Q78] 当前时间
来源：http://read.share.yfazqb.com/Article/details/gbbtjebys.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.blog.vehdjk.com/Article/details/gfltvxkva.sHtML

[Q79] 字符串拼接
来源：http://blog.bbcook.cn/Article/details/gsrierctt.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://mobile.epnwcf.com/Article/details/gjycrtthq.sHtML

[Q80] 字符串截取
来源：http://m.share.fktsv.cn/Article/details/glvrqmauj.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.blog.tarul.cn/Article/details/gqtlmmxuf.sHtML

[Q81] 字符串替换
来源：http://blog.vehdjk.com/Article/details/gcicfemxk.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://wap.fktsv.cn/Article/details/gbudxtwxv.sHtML

[Q82] 字符长度与字节长度
来源：http://www.share.epnwcf.com/Article/details/gwzgmhfux.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://3g.epnwcf.com/Article/details/gmkzfffeb.sHtML

[Q83] 大小写转换
来源：http://www.blog.sjlbkw.cn/Article/details/gkvuymabl.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.blog.vehdjk.com/Article/details/ggfuxpbxb.sHtML

[Q84] 去除首尾空格
来源：http://m.share.bbcook.cn/Article/details/gkezlvsli.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.share.epnwcf.com/Article/details/gvkxcdlob.sHtML

[Q85] 数值取整
来源：http://www.share.sjlbkw.cn/Article/details/gpcddmpwp.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.m.share.tarul.cn/Article/details/gvbhskanv.sHtML

[Q86] 读取 JSON 字段
来源：http://m.share.epnwcf.com/Article/details/ggaujeumy.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.share.epnwcf.com/Article/details/gqilbhehp.sHtML

[Q87] JSON 字段做条件
来源：http://baike.epnwcf.com/Article/details/gzskrpurd.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://m.share.fktsv.cn/Article/details/gcibmiduj.sHtML

[Q88] 行转列（条件聚合）
来源：http://baike.bbcook.cn/Article/details/gcpokqyew.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://read.share.fktsv.cn/Article/details/gsxvxluhm.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://mobile.tarul.cn/Article/details/gprxsoqrs.sHtML

[Q89] 判断表是否存在
来源：http://mobile.vehdjk.com/Article/details/gvximigzl.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://m.share.yfazqb.com/Article/details/gjjruicjl.sHtML

[Q90] 生成序号列
来源：http://baike.tarul.cn/Article/details/gslbpwmti.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.share.yfazqb.com/Article/details/gwyctvcxb.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/gfocjalfp.sHtML

R. Bash 专题
来源：http://www.m.share.tarul.cn/Article/details/gvapmnpsc.sHtML

================================================================================
来源：http://baike.sjlbkw.cn/Article/details/gcqnhwivo.sHtML

[R01] shebang 与严格模式
来源：http://www.share.yfazqb.com/Article/details/guzhnuinf.sHtML

#!/usr/bin/env bash
来源：http://www.blog.vehdjk.com/Article/details/gwyhrvyom.sHtML

set -euo pipefail
来源：http://wap.yfazqb.com/Article/details/gapnmouiy.sHtML

[R02] 变量赋值与使用
来源：http://3g.yfazqb.com/Article/details/gfsrhxgtj.sHtML

name="Tom"; echo "$name"
来源：http://baike.sjlbkw.cn/Article/details/gpkngofzm.sHtML

[R03] 只读变量
来源：http://mobile.tarul.cn/Article/details/ghwrorbkl.sHtML

readonly PI=3.14
来源：http://www.blog.sjlbkw.cn/Article/details/grbvcivex.sHtML

[R04] 位置参数
来源：http://wap.sjlbkw.cn/Article/details/gymlsavvi.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.m.share.bbcook.cn/Article/details/gxllkxlnd.sHtML

[R05] 参数默认值
来源：http://3g.fktsv.cn/Article/details/gdqgluqeg.sHtML

name="${1:-default}"
来源：http://www.m.share.epnwcf.com/Article/details/ggtxofwqo.sHtML

[R06] 判断命令是否存在
来源：http://www.share.sjlbkw.cn/Article/details/goviawhnw.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://baike.epnwcf.com/Article/details/gkezgicvf.sHtML

[R07] if 判断文件
来源：http://blog.fktsv.cn/Article/details/gihfjhqzl.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://baike.tarul.cn/Article/details/gylmbfrya.sHtML

[R08] 数值比较
来源：http://www.blog.vehdjk.com/Article/details/gajomjvtj.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://m.share.fktsv.cn/Article/details/ggnrmszrv.sHtML

[R09] 字符串比较
来源：http://blog.yfazqb.com/Article/details/govpzpdud.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://wap.sjlbkw.cn/Article/details/gtxlnitzb.sHtML

[R10] 正则匹配
来源：http://baike.epnwcf.com/Article/details/glamirrmj.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://mobile.tarul.cn/Article/details/gtnwsbknp.sHtML

[R11] case 多分支
来源：http://read.share.yfazqb.com/Article/details/gsboujgji.sHtML

case "$1" in
来源：http://www.blog.bbcook.cn/Article/details/gmybnsqvu.sHtML

start) echo "启动" ;;
来源：http://www.m.share.sjlbkw.cn/Article/details/gbmajbsgy.sHtML

stop)  echo "停止" ;;
来源：http://www.share.bbcook.cn/Article/details/gqnsnxfbf.sHtML

*)     echo "未知命令" ;;
来源：http://www.m.share.tarul.cn/Article/details/galcfiqbl.sHtML

esac
来源：http://read.share.epnwcf.com/Article/details/gsgmnroff.sHtML

[R12] for 遍历文件
来源：http://3g.fktsv.cn/Article/details/guihwvthm.sHtML

for f in *.txt; do echo "$f"; done
来源：http://3g.bbcook.cn/Article/details/gslxnwemp.sHtML

[R13] for 计数循环
来源：http://blog.fktsv.cn/Article/details/gnyegbohz.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://wap.vehdjk.com/Article/details/gqvyugxqk.sHtML

[R14] C 风格 for
来源：http://3g.vehdjk.com/Article/details/gldgufjka.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.share.sjlbkw.cn/Article/details/gbawptwnr.sHtML

[R15] while 逐行读文件
来源：http://3g.yfazqb.com/Article/details/gledlrrfu.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://blog.bbcook.cn/Article/details/gjqahesql.sHtML

[R16] until 等待条件
来源：http://www.share.epnwcf.com/Article/details/gcishjkrw.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://mobile.vehdjk.com/Article/details/gqzlynmfj.sHtML

[R17] 数组定义与取值
来源：http://read.share.fktsv.cn/Article/details/gbtihkbfz.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://blog.vehdjk.com/Article/details/ghjhngeas.sHtML

[R18] 遍历数组
来源：http://www.m.share.epnwcf.com/Article/details/gkqxvzkri.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://m.share.sjlbkw.cn/Article/details/gtibdnpdc.sHtML

[R19] 数组长度
来源：http://read.share.yfazqb.com/Article/details/gttfdecfw.sHtML

echo "${#arr[@]}"
来源：http://www.share.vehdjk.com/Article/details/gpkwxewcx.sHtML

[R20] 关联数组（字典）
来源：http://read.share.sjlbkw.cn/Article/details/gaycpmygn.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.share.sjlbkw.cn/Article/details/gtrfunqme.sHtML

[R21] 字符串长度
来源：http://www.m.share.vehdjk.com/Article/details/gbqexfzww.sHtML

echo "${#s}"
来源：http://blog.bbcook.cn/Article/details/gbfijwsif.sHtML

[R22] 截取子串
来源：http://3g.yfazqb.com/Article/details/gasztynvp.sHtML

echo "${s:0:5}"
来源：http://3g.yfazqb.com/Article/details/ghjtdvhxl.sHtML

[R23] 字符串替换
来源：http://www.blog.bbcook.cn/Article/details/gmgjxmcff.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://m.share.fktsv.cn/Article/details/gdabjhuva.sHtML

[R24] 大小写转换
来源：http://baike.vehdjk.com/Article/details/gzdhsurbv.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.m.share.fktsv.cn/Article/details/gpjizkzau.sHtML

[R25] 去后缀 / 去前缀
来源：http://3g.fktsv.cn/Article/details/gemhfjvic.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://wap.sjlbkw.cn/Article/details/gtfjbustw.sHtML

[R26] 命令替换
来源：http://blog.tarul.cn/Article/details/gycbuybco.sHtML

now=$(date +%F); echo "$now"
来源：http://www.m.share.epnwcf.com/Article/details/ghnhpsqpe.sHtML

[R27] 算术展开
来源：http://www.share.vehdjk.com/Article/details/gozzylxmw.sHtML

echo $((1 + 2 * 3))
来源：http://read.share.tarul.cn/Article/details/gfnhdepav.sHtML

[R28] 浮点运算
来源：http://www.share.bbcook.cn/Article/details/gphlpkjbf.sHtML

echo "scale=2; 10/3" | bc
来源：http://read.share.tarul.cn/Article/details/gcxlmrepi.sHtML

[R29] 定义函数
来源：http://read.share.yfazqb.com/Article/details/glsyvrtsr.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://blog.fktsv.cn/Article/details/gngdzrkdp.sHtML

[R30] 函数返回状态码
来源：http://read.share.yfazqb.com/Article/details/gefeotevb.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://m.share.epnwcf.com/Article/details/gdsjnpnwb.sHtML

[R31] 局部变量
来源：http://3g.tarul.cn/Article/details/gmuwdfbak.sHtML

f() { local x=1; echo "$x"; }
来源：http://baike.yfazqb.com/Article/details/gcxnuepht.sHtML

[R32] 参数个数校验
来源：http://wap.yfazqb.com/Article/details/gfwayaugt.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://baike.vehdjk.com/Article/details/gdozqcovs.sHtML

[R33] 捕获错误并提示行号
来源：http://www.share.fktsv.cn/Article/details/gfqtdywga.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://blog.yfazqb.com/Article/details/gsicyaprj.sHtML

[R34] 退出时清理
来源：http://www.blog.fktsv.cn/Article/details/gudrzcduv.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://3g.vehdjk.com/Article/details/gtaikfswk.sHtML

[R35] 后台执行并等待
来源：http://m.share.yfazqb.com/Article/details/gitmvsgol.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://3g.epnwcf.com/Article/details/gnkkyoqkm.sHtML

[R36] 并发执行多个任务
来源：http://baike.yfazqb.com/Article/details/gbvduppri.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://mobile.fktsv.cn/Article/details/gdxeolyws.sHtML

[R37] 把输出赋给变量
来源：http://www.m.share.sjlbkw.cn/Article/details/gueqrgkvf.sHtML

files=$(ls -1)
来源：http://mobile.yfazqb.com/Article/details/gcqtjsnxb.sHtML

[R38] 管道串联
来源：http://blog.tarul.cn/Article/details/gmdmsbwwm.sHtML

cat a.txt | grep -i error | wc -l
来源：http://blog.bbcook.cn/Article/details/gsoyqhsgd.sHtML

[R39] 重定向标准输出与错误
来源：http://wap.tarul.cn/Article/details/gwycrxskf.sHtML

cmd > out.log 2>&1
来源：http://read.share.vehdjk.com/Article/details/gaodapdmq.sHtML

[R40] 追加写日志
来源：http://3g.fktsv.cn/Article/details/ghuyfxeog.sHtML

echo "log" >> out.log
来源：http://wap.bbcook.cn/Article/details/gmcflbgyd.sHtML

[R41] 丢弃输出
来源：http://mobile.epnwcf.com/Article/details/glnfnixxs.sHtML

cmd >/dev/null 2>&1
来源：http://www.blog.fktsv.cn/Article/details/gaduwekfr.sHtML

[R42] 输入重定向
来源：http://www.m.share.yfazqb.com/Article/details/giagwevmp.sHtML

wc -l < a.txt
来源：http://mobile.yfazqb.com/Article/details/glpmvgzul.sHtML

[R43] 按名字查找文件
来源：http://www.share.bbcook.cn/Article/details/glqeazfpg.sHtML

find . -name "*.log" -type f
来源：http://m.share.vehdjk.com/Article/details/grquekqfa.sHtML

[R44] 按修改时间查找
来源：http://wap.bbcook.cn/Article/details/gjfacbkfw.sHtML

find . -mtime -7 -type f
来源：http://baike.epnwcf.com/Article/details/gdthzthmk.sHtML

[R45] 批量删除
来源：http://3g.tarul.cn/Article/details/gxdaconwd.sHtML

find . -name "*.tmp" -delete
来源：http://blog.yfazqb.com/Article/details/gnldmwolr.sHtML

[R46] 递归替换文件内容
来源：http://blog.yfazqb.com/Article/details/glfbtcibp.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://m.share.yfazqb.com/Article/details/gnrovrxei.sHtML

[R47] sed 单行替换
来源：http://mobile.fktsv.cn/Article/details/gwmvphxgw.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://blog.fktsv.cn/Article/details/gmpqsbunn.sHtML

[R48] awk 取指定列
来源：http://blog.fktsv.cn/Article/details/ghhjwuryr.sHtML

awk '{print $1, $3}' a.txt
来源：http://blog.bbcook.cn/Article/details/gbyasrcjy.sHtML

[R49] awk 带条件
来源：http://www.blog.sjlbkw.cn/Article/details/glrgstyww.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://blog.fktsv.cn/Article/details/gvaxeisco.sHtML

[R50] awk 求和
来源：http://blog.vehdjk.com/Article/details/gcxbxxhjo.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.share.vehdjk.com/Article/details/ghtxrojwd.sHtML

[R51] 排序去重取前几
来源：http://mobile.bbcook.cn/Article/details/gejfgesnt.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://3g.vehdjk.com/Article/details/gzipkccfi.sHtML

[R52] 统计行数
来源：http://baike.tarul.cn/Article/details/glhxrhauo.sHtML

wc -l a.txt
来源：http://3g.bbcook.cn/Article/details/gsxqhnyog.sHtML

[R53] 查看文件头与实时尾
来源：http://m.share.bbcook.cn/Article/details/gpmyfxrsp.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://mobile.vehdjk.com/Article/details/gpjbwjmqq.sHtML

[R54] 比较两个文件
来源：http://wap.tarul.cn/Article/details/gchdmeonq.sHtML

diff a.txt b.txt
来源：http://3g.sjlbkw.cn/Article/details/gafdjqzts.sHtML

[R55] 压缩与解压
来源：http://wap.yfazqb.com/Article/details/gqdqgipgz.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://3g.fktsv.cn/Article/details/glwgwmrty.sHtML

[R56] 远程拷贝
来源：http://3g.yfazqb.com/Article/details/gjznwqxgc.sHtML

scp file user@host:/path/
来源：http://blog.bbcook.cn/Article/details/glsorehnp.sHtML

[R57] 远程执行命令
来源：http://www.blog.fktsv.cn/Article/details/gceuqoyyg.sHtML

ssh user@host 'uptime'
来源：http://baike.vehdjk.com/Article/details/gjyygcclk.sHtML

[R58] 下载文件
来源：http://m.share.epnwcf.com/Article/details/gmgawgyhh.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://mobile.bbcook.cn/Article/details/gcadeztqd.sHtML

[R59] 发 POST JSON
来源：http://www.blog.fktsv.cn/Article/details/gzauciemy.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.m.share.bbcook.cn/Article/details/ghzpjijfu.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.m.share.fktsv.cn/Article/details/gjquhewjk.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mobile.sjlbkw.cn/Article/details/gtavhtqlb.sHtML

[R61] 磁盘占用
来源：http://www.m.share.sjlbkw.cn/Article/details/giulbmxnu.sHtML

df -h;  du -sh *
来源：http://mobile.sjlbkw.cn/Article/details/glmjevagh.sHtML

[R62] 找最占空间的文件
来源：http://m.share.vehdjk.com/Article/details/gsokhpttl.sHtML

du -ah . | sort -rh | head -10
来源：http://www.m.share.yfazqb.com/Article/details/gjukaqyvp.sHtML

[R63] 内存与进程
来源：http://www.m.share.fktsv.cn/Article/details/gzizzuyvo.sHtML

free -h;  ps aux | grep nginx
来源：http://mobile.fktsv.cn/Article/details/gtszujbft.sHtML

[R64] 结束进程
来源：http://www.m.share.vehdjk.com/Article/details/glgcllbvl.sHtML

kill -9 $(pgrep -f app.py)
来源：http://blog.bbcook.cn/Article/details/ghiyofqha.sHtML

[R65] 查看端口占用
来源：http://read.share.epnwcf.com/Article/details/gucuqprpx.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://m.share.yfazqb.com/Article/details/gpiybwzhv.sHtML

[R66] 定时任务
来源：http://m.share.sjlbkw.cn/Article/details/gtignltpr.sHtML

crontab -e;  crontab -l
来源：http://m.share.fktsv.cn/Article/details/gmqiqqanw.sHtML

[R67] 生成随机十六进制串
来源：http://read.share.vehdjk.com/Article/details/gluychdwl.sHtML

openssl rand -hex 16
来源：http://read.share.vehdjk.com/Article/details/gmiroaehw.sHtML

[R68] 计算文件校验值
来源：http://m.share.epnwcf.com/Article/details/gyqnurpqt.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://m.share.epnwcf.com/Article/details/gcvxqncmw.sHtML

[R69] 生成随机密码
来源：http://blog.sjlbkw.cn/Article/details/gcokphadn.sHtML

head -c 16 /dev/urandom | base64
来源：http://m.share.fktsv.cn/Article/details/gygyvysix.sHtML

[R70] 时间戳与互转
来源：http://www.blog.epnwcf.com/Article/details/ghdtqxrpe.sHtML

date +%s;  date -d @1700000000
来源：http://blog.yfazqb.com/Article/details/gqehspdnh.sHtML

[R71] 日期格式化
来源：http://read.share.vehdjk.com/Article/details/gcrdtizbn.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://blog.epnwcf.com/Article/details/gdrtnqrgb.sHtML

[R72] 等待端口就绪
来源：http://www.blog.yfazqb.com/Article/details/gukajkdad.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://mobile.fktsv.cn/Article/details/gzephqbxg.sHtML

[R73] 分割大日志
来源：http://mobile.yfazqb.com/Article/details/gzemkzgfu.sHtML

split -l 1000 big.log part_
来源：http://www.share.bbcook.cn/Article/details/gbzxbgimt.sHtML

[R74] 批量重命名
来源：http://3g.fktsv.cn/Article/details/gjkijodyi.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.blog.epnwcf.com/Article/details/gwgeitpah.sHtML

[R75] 导出环境变量
来源：http://www.m.share.vehdjk.com/Article/details/gkmbpyguf.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://baike.bbcook.cn/Article/details/gnalegwio.sHtML

[R76] 使用临时文件
来源：http://www.m.share.epnwcf.com/Article/details/gumvqlycm.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://wap.yfazqb.com/Article/details/gnlwovbwj.sHtML

[R77] 读取用户输入
来源：http://www.m.share.tarul.cn/Article/details/gjwggmkrf.sHtML

read -rp "请输入: " ans
来源：http://www.share.tarul.cn/Article/details/gcnqsrvwh.sHtML

[R78] 交互式菜单
来源：http://3g.epnwcf.com/Article/details/gcunnlmoj.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://read.share.fktsv.cn/Article/details/gdlredgnn.sHtML

[R79] 解析命令行选项
来源：http://mobile.sjlbkw.cn/Article/details/ggkuneojf.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wap.bbcook.cn/Article/details/gbnpqkysp.sHtML

[R80] 查看脚本执行耗时
来源：http://mobile.sjlbkw.cn/Article/details/gmrpexkqd.sHtML

time ./run.sh
来源：http://www.blog.epnwcf.com/Article/details/gcfpdguqd.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/gbkxkodxl.sHtML

S. C / C++ 专题
来源：http://blog.yfazqb.com/Article/details/gscqzrieh.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/gyixoteuz.sHtML

[S01] C：Hello World
来源：http://3g.bbcook.cn/Article/details/gpbdpcrgw.sHtML

#include <stdio.h>
来源：http://www.share.sjlbkw.cn/Article/details/gasudycin.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.share.sjlbkw.cn/Article/details/goqreggxc.sHtML

[S02] C：变量与格式化输出
来源：http://read.share.yfazqb.com/Article/details/gqjyohhgw.sHtML

int a = 10; printf("%d\n", a);
来源：http://mobile.bbcook.cn/Article/details/gqfixoref.sHtML

[S03] C：读入整数
来源：http://m.share.bbcook.cn/Article/details/gtrecyvdk.sHtML

int x; scanf("%d", &x);
来源：http://mobile.fktsv.cn/Article/details/gyfkuvukh.sHtML

[S04] C：字符串复制
来源：http://m.share.vehdjk.com/Article/details/guctqkixo.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.m.share.yfazqb.com/Article/details/gdvlpqlnz.sHtML

[S05] C：字符串长度
来源：http://read.share.tarul.cn/Article/details/gpzwiufrj.sHtML

strlen(s)
来源：http://wap.bbcook.cn/Article/details/gczsqayom.sHtML

[S06] C：字符串比较
来源：http://read.share.vehdjk.com/Article/details/gjlouxqrz.sHtML

strcmp(a, b) == 0
来源：http://read.share.bbcook.cn/Article/details/gspzljvau.sHtML

[S07] C：数组遍历求和
来源：http://3g.sjlbkw.cn/Article/details/gstyfmcfz.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.share.sjlbkw.cn/Article/details/ggenbytxn.sHtML

[S08] C：动态内存分配与释放
来源：http://baike.tarul.cn/Article/details/gmydpaedk.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://3g.vehdjk.com/Article/details/gqauagnbq.sHtML

[S09] C：结构体定义与初始化
来源：http://3g.sjlbkw.cn/Article/details/gzjjacyfl.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://blog.epnwcf.com/Article/details/gjdsswtpf.sHtML

[S10] C：指针与解引用
来源：http://www.m.share.bbcook.cn/Article/details/gfpruhvmt.sHtML

int *p = &a;  *p = 5;
来源：http://read.share.vehdjk.com/Article/details/gpdnvaeow.sHtML

[S11] C：逐行读文件
来源：http://www.share.bbcook.cn/Article/details/grcsipewp.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://baike.vehdjk.com/Article/details/gvgcrlszy.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://3g.fktsv.cn/Article/details/ggwlfgxxs.sHtML

fclose(f);
来源：http://read.share.bbcook.cn/Article/details/gscgawceo.sHtML

[S12] C：写文件
来源：http://m.share.fktsv.cn/Article/details/gdnhlbuzc.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://blog.fktsv.cn/Article/details/gfkdjgkgd.sHtML

[S13] C：宏定义
来源：http://baike.tarul.cn/Article/details/gjqidqhgc.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wap.epnwcf.com/Article/details/gcbyqltlb.sHtML

[S14] C：枚举
来源：http://blog.fktsv.cn/Article/details/gnhkuycym.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://mobile.fktsv.cn/Article/details/ggqyksjec.sHtML

[S15] C：类型转换
来源：http://www.m.share.yfazqb.com/Article/details/grpiysjlq.sHtML

(double) a / b
来源：http://blog.bbcook.cn/Article/details/gyisqsqdr.sHtML

[S16] C：位操作置位
来源：http://baike.yfazqb.com/Article/details/gjrvzgevt.sHtML

x |= (1 << 3);
来源：http://baike.sjlbkw.cn/Article/details/ggmtixibc.sHtML

[S17] C：安全拼接字符串
来源：http://wap.sjlbkw.cn/Article/details/gvteknlei.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.blog.vehdjk.com/Article/details/gnsblmgak.sHtML

[S18] C：命令行参数
来源：http://wap.tarul.cn/Article/details/glspmpwfm.sHtML

int main(int argc, char **argv)
来源：http://baike.epnwcf.com/Article/details/gacgzzxed.sHtML

[S19] C：快速排序
来源：http://wap.fktsv.cn/Article/details/gubjcezbr.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://m.share.epnwcf.com/Article/details/gqwirmdyb.sHtML

[S20] C：二分查找
来源：http://www.share.vehdjk.com/Article/details/gktpvehqq.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.share.tarul.cn/Article/details/guiivorrr.sHtML

[S21] C：字符类别判断
来源：http://mobile.fktsv.cn/Article/details/gjiywklbj.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://blog.bbcook.cn/Article/details/gynehjyjl.sHtML

[S22] C：字符串转数字
来源：http://blog.bbcook.cn/Article/details/gfthlovsh.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://read.share.fktsv.cn/Article/details/girojprsw.sHtML

[S23] C：随机数
来源：http://baike.sjlbkw.cn/Article/details/ggthnsojb.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.share.bbcook.cn/Article/details/gnjspeyxs.sHtML

[S24] C：获取本地时间
来源：http://wap.tarul.cn/Article/details/gdakjmgwi.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.share.vehdjk.com/Article/details/gqhqfhwum.sHtML

[S25] C：内存拷贝
来源：http://mobile.tarul.cn/Article/details/gbombifca.sHtML

memcpy(dst, src, n);
来源：http://3g.sjlbkw.cn/Article/details/gbdfkhzjp.sHtML

[S26] C：内存清零
来源：http://mobile.bbcook.cn/Article/details/gpdawleji.sHtML

memset(a, 0, sizeof a);
来源：http://mobile.yfazqb.com/Article/details/glgqyljrm.sHtML

[S27] C：定义常量
来源：http://www.blog.vehdjk.com/Article/details/gkfcqghdg.sHtML

const double PI = 3.14159;
来源：http://m.share.fktsv.cn/Article/details/gwbhmciuy.sHtML

[S28] C：静态变量
来源：http://blog.bbcook.cn/Article/details/gcpetuzrm.sHtML

static int counter = 0;
来源：http://m.share.epnwcf.com/Article/details/ggxwtradl.sHtML

[S29] C：变参函数
来源：http://baike.epnwcf.com/Article/details/gmfaysqhf.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.blog.fktsv.cn/Article/details/gnxaxnpym.sHtML

[S30] C：头文件保护
来源：http://baike.epnwcf.com/Article/details/gqkvagcxx.sHtML

#ifndef X_H
来源：http://www.m.share.sjlbkw.cn/Article/details/gylaakobl.sHtML

#define X_H
来源：http://m.share.yfazqb.com/Article/details/gabxtylje.sHtML

#endif
来源：http://3g.fktsv.cn/Article/details/gmjxokapl.sHtML

[S31] C++：Hello World
来源：http://3g.sjlbkw.cn/Article/details/gyaizuuvu.sHtML


<!-- 参考信息 -->