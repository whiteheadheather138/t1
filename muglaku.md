代发 wailian999

[Q63] 开启事务
来源：http://mobile.yfazqb.com/Article/details/gwscgklfm.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://mobile.yfazqb.com/Article/details/gkzufhmyk.sHtML

[Q64] 提交事务
来源：http://www.blog.tarul.cn/Article/details/gfhvqgbhw.sHtML

COMMIT;
来源：http://read.share.vehdjk.com/Article/details/gcqfzhopn.sHtML

[Q65] 回滚事务
来源：http://mobile.sjlbkw.cn/Article/details/ghhihiwdu.sHtML

ROLLBACK;
来源：http://baike.epnwcf.com/Article/details/getousnvm.sHtML

[Q66] 行锁查询
来源：http://wap.fktsv.cn/Article/details/grpocjvjw.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.blog.vehdjk.com/Article/details/gkajcrrkh.sHtML

[Q67] 设置隔离级别
来源：http://3g.yfazqb.com/Article/details/gmlruoajc.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://read.share.bbcook.cn/Article/details/gydycajnf.sHtML

[Q68] 保存点
来源：http://www.share.vehdjk.com/Article/details/geoqwsnxx.sHtML

SAVEPOINT sp1;
来源：http://baike.sjlbkw.cn/Article/details/glqaffads.sHtML

ROLLBACK TO sp1;
来源：http://3g.sjlbkw.cn/Article/details/gmrjrpnxp.sHtML

[Q69] 查看执行计划
来源：http://m.share.bbcook.cn/Article/details/gyhimdjmh.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://baike.tarul.cn/Article/details/gcvuqmpnu.sHtML

[Q70] 更新统计信息
来源：http://www.blog.yfazqb.com/Article/details/gslpcrlpr.sHtML

ANALYZE TABLE users;
来源：http://baike.tarul.cn/Article/details/gbkmkowwy.sHtML

[Q71] 查看建表语句
来源：http://www.m.share.tarul.cn/Article/details/gxxiclswf.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://3g.sjlbkw.cn/Article/details/gdvizlpnz.sHtML

[Q72] 查看索引
来源：http://baike.fktsv.cn/Article/details/gcvvievmh.sHtML

SHOW INDEX FROM users;
来源：http://www.blog.yfazqb.com/Article/details/gqwduwdgh.sHtML

[Q73] 查看表状态
来源：http://m.share.fktsv.cn/Article/details/gtukdqfhj.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://read.share.vehdjk.com/Article/details/gpspyagtj.sHtML

[Q74] 强制使用索引
来源：http://m.share.tarul.cn/Article/details/ghxswtwhd.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://3g.tarul.cn/Article/details/gcnvwrksr.sHtML

[Q75] 日期格式化
来源：http://wap.tarul.cn/Article/details/gvclhmzaq.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://m.share.vehdjk.com/Article/details/gtklgatva.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://read.share.bbcook.cn/Article/details/gflwvgcaj.sHtML

[Q76] 按天统计
来源：http://www.blog.tarul.cn/Article/details/gmfueycrv.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.m.share.yfazqb.com/Article/details/ghuwslowf.sHtML

[Q77] 时间加减
来源：http://www.blog.sjlbkw.cn/Article/details/gxekdcgcv.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.blog.fktsv.cn/Article/details/gieupbpmx.sHtML

[Q78] 当前时间
来源：http://wap.vehdjk.com/Article/details/gzcylzmtd.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://blog.sjlbkw.cn/Article/details/gkhfgqqrd.sHtML

[Q79] 字符串拼接
来源：http://baike.sjlbkw.cn/Article/details/gjsdcrryt.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.share.tarul.cn/Article/details/gusstjrkz.sHtML

[Q80] 字符串截取
来源：http://m.share.epnwcf.com/Article/details/gqzbfplps.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.share.yfazqb.com/Article/details/gwpxrxdyn.sHtML

[Q81] 字符串替换
来源：http://www.share.fktsv.cn/Article/details/giinyuini.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://baike.vehdjk.com/Article/details/gucqslfgl.sHtML

[Q82] 字符长度与字节长度
来源：http://3g.yfazqb.com/Article/details/grmcfguka.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://mobile.vehdjk.com/Article/details/gwxgyysgg.sHtML

[Q83] 大小写转换
来源：http://www.share.epnwcf.com/Article/details/gtneniauu.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.blog.vehdjk.com/Article/details/gccvaksxg.sHtML

[Q84] 去除首尾空格
来源：http://wap.tarul.cn/Article/details/grgusmevw.sHtML

SELECT TRIM(name) FROM users;
来源：http://baike.yfazqb.com/Article/details/gzcgknsdm.sHtML

[Q85] 数值取整
来源：http://mobile.vehdjk.com/Article/details/gwdtqnewm.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://m.share.yfazqb.com/Article/details/guueadyse.sHtML

[Q86] 读取 JSON 字段
来源：http://baike.tarul.cn/Article/details/gyjjmaulm.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://read.share.fktsv.cn/Article/details/gspkgizfg.sHtML

[Q87] JSON 字段做条件
来源：http://m.share.yfazqb.com/Article/details/gvapqorle.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://mobile.yfazqb.com/Article/details/grcngqoan.sHtML

[Q88] 行转列（条件聚合）
来源：http://3g.yfazqb.com/Article/details/gomtpavus.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.m.share.sjlbkw.cn/Article/details/gsrbnsjlb.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://blog.yfazqb.com/Article/details/gkoanaeuf.sHtML

[Q89] 判断表是否存在
来源：http://m.share.bbcook.cn/Article/details/gunljxrfg.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.share.sjlbkw.cn/Article/details/gdsdkizjp.sHtML

[Q90] 生成序号列
来源：http://baike.fktsv.cn/Article/details/gradufaip.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://wap.bbcook.cn/Article/details/gmqsluoju.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/gyrzyvobn.sHtML

R. Bash 专题
来源：http://3g.sjlbkw.cn/Article/details/gmctfnabf.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/gsrqgpwkr.sHtML

[R01] shebang 与严格模式
来源：http://www.m.share.yfazqb.com/Article/details/gzhqdahtt.sHtML

#!/usr/bin/env bash
来源：http://blog.bbcook.cn/Article/details/gfaiusjjs.sHtML

set -euo pipefail
来源：http://m.share.epnwcf.com/Article/details/gxqkalagq.sHtML

[R02] 变量赋值与使用
来源：http://wap.vehdjk.com/Article/details/ghyaqqfiw.sHtML

name="Tom"; echo "$name"
来源：http://www.blog.bbcook.cn/Article/details/gdpyivjmi.sHtML

[R03] 只读变量
来源：http://read.share.epnwcf.com/Article/details/gskfcwrsc.sHtML

readonly PI=3.14
来源：http://www.m.share.yfazqb.com/Article/details/gbtzabkde.sHtML

[R04] 位置参数
来源：http://www.m.share.tarul.cn/Article/details/ghukmriyv.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://baike.bbcook.cn/Article/details/gkedesqke.sHtML

[R05] 参数默认值
来源：http://m.share.tarul.cn/Article/details/grqnlyvgb.sHtML

name="${1:-default}"
来源：http://wap.sjlbkw.cn/Article/details/glskoaayd.sHtML

[R06] 判断命令是否存在
来源：http://mobile.sjlbkw.cn/Article/details/gnhmqwurb.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://baike.tarul.cn/Article/details/gchtcovbm.sHtML

[R07] if 判断文件
来源：http://baike.tarul.cn/Article/details/gzdtbijkr.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.m.share.tarul.cn/Article/details/gqajemcgx.sHtML

[R08] 数值比较
来源：http://m.share.vehdjk.com/Article/details/gsequwzoz.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://baike.yfazqb.com/Article/details/gaqpdrubk.sHtML

[R09] 字符串比较
来源：http://read.share.yfazqb.com/Article/details/glvjekqkm.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.blog.fktsv.cn/Article/details/gbtztttvp.sHtML

[R10] 正则匹配
来源：http://mobile.bbcook.cn/Article/details/gymgclset.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://blog.sjlbkw.cn/Article/details/gosunzaps.sHtML

[R11] case 多分支
来源：http://www.m.share.yfazqb.com/Article/details/gaxlbyvct.sHtML

case "$1" in
来源：http://mobile.vehdjk.com/Article/details/gdhxexxin.sHtML

start) echo "启动" ;;
来源：http://www.share.fktsv.cn/Article/details/gueudohfg.sHtML

stop)  echo "停止" ;;
来源：http://mobile.tarul.cn/Article/details/gphkcwnyf.sHtML

*)     echo "未知命令" ;;
来源：http://www.share.tarul.cn/Article/details/gydhicyxr.sHtML

esac
来源：http://wap.tarul.cn/Article/details/gjqaouamx.sHtML

[R12] for 遍历文件
来源：http://wap.epnwcf.com/Article/details/gdnfahvnk.sHtML

for f in *.txt; do echo "$f"; done
来源：http://read.share.bbcook.cn/Article/details/gzkmixfgh.sHtML

[R13] for 计数循环
来源：http://read.share.tarul.cn/Article/details/gqaxbusic.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.blog.bbcook.cn/Article/details/geffyrjlq.sHtML

[R14] C 风格 for
来源：http://www.share.tarul.cn/Article/details/goxtvjzwt.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://m.share.sjlbkw.cn/Article/details/gpzwkmjgw.sHtML

[R15] while 逐行读文件
来源：http://www.blog.epnwcf.com/Article/details/gkbsvvszw.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://mobile.sjlbkw.cn/Article/details/guorsdplr.sHtML

[R16] until 等待条件
来源：http://read.share.fktsv.cn/Article/details/gqeqkhsry.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.blog.vehdjk.com/Article/details/gyczycwcs.sHtML

[R17] 数组定义与取值
来源：http://m.share.epnwcf.com/Article/details/gcmusarkl.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://blog.yfazqb.com/Article/details/gbistxoaa.sHtML

[R18] 遍历数组
来源：http://m.share.epnwcf.com/Article/details/glkmuudoq.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://read.share.fktsv.cn/Article/details/guvmivwtk.sHtML

[R19] 数组长度
来源：http://wap.tarul.cn/Article/details/gzlufjhtw.sHtML

echo "${#arr[@]}"
来源：http://www.share.fktsv.cn/Article/details/gslubbpol.sHtML

[R20] 关联数组（字典）
来源：http://mobile.epnwcf.com/Article/details/griusxlrw.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.blog.fktsv.cn/Article/details/gzwbuugnm.sHtML

[R21] 字符串长度
来源：http://www.share.vehdjk.com/Article/details/grykteypa.sHtML

echo "${#s}"
来源：http://wap.fktsv.cn/Article/details/grbrufren.sHtML

[R22] 截取子串
来源：http://3g.fktsv.cn/Article/details/gjdsupliq.sHtML

echo "${s:0:5}"
来源：http://wap.yfazqb.com/Article/details/grysfmnxf.sHtML

[R23] 字符串替换
来源：http://read.share.fktsv.cn/Article/details/gjuwwwrdn.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://blog.sjlbkw.cn/Article/details/gbmuybwgg.sHtML

[R24] 大小写转换
来源：http://baike.yfazqb.com/Article/details/gmlygxebd.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://baike.epnwcf.com/Article/details/gmmmatjco.sHtML

[R25] 去后缀 / 去前缀
来源：http://baike.vehdjk.com/Article/details/gponnbcue.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.m.share.tarul.cn/Article/details/gqwwgvvko.sHtML

[R26] 命令替换
来源：http://3g.epnwcf.com/Article/details/garriandc.sHtML

now=$(date +%F); echo "$now"
来源：http://baike.tarul.cn/Article/details/gmbmyenwa.sHtML

[R27] 算术展开
来源：http://wap.fktsv.cn/Article/details/ghxxtgqns.sHtML

echo $((1 + 2 * 3))
来源：http://m.share.bbcook.cn/Article/details/gpdaplyvg.sHtML

[R28] 浮点运算
来源：http://www.blog.vehdjk.com/Article/details/gjmahbzre.sHtML

echo "scale=2; 10/3" | bc
来源：http://blog.bbcook.cn/Article/details/glfalyjew.sHtML

[R29] 定义函数
来源：http://blog.yfazqb.com/Article/details/gdommtpop.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.blog.tarul.cn/Article/details/gzgieyslz.sHtML

[R30] 函数返回状态码
来源：http://www.blog.yfazqb.com/Article/details/gprpfslkx.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://3g.vehdjk.com/Article/details/ggbfhtwln.sHtML

[R31] 局部变量
来源：http://m.share.yfazqb.com/Article/details/gcyzqqolj.sHtML

f() { local x=1; echo "$x"; }
来源：http://baike.sjlbkw.cn/Article/details/gqtykxkdl.sHtML

[R32] 参数个数校验
来源：http://3g.fktsv.cn/Article/details/gmuvnrpqn.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.share.bbcook.cn/Article/details/gowgkebll.sHtML

[R33] 捕获错误并提示行号
来源：http://www.m.share.vehdjk.com/Article/details/gtqwosanc.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://read.share.sjlbkw.cn/Article/details/gicaktnxy.sHtML

[R34] 退出时清理
来源：http://blog.yfazqb.com/Article/details/gmvdiowkz.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://mobile.vehdjk.com/Article/details/giclmaovt.sHtML

[R35] 后台执行并等待
来源：http://read.share.sjlbkw.cn/Article/details/gzavsopts.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://3g.sjlbkw.cn/Article/details/gdetvvhsm.sHtML

[R36] 并发执行多个任务
来源：http://wap.fktsv.cn/Article/details/gxusvcfnw.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://3g.tarul.cn/Article/details/gdgwohslk.sHtML

[R37] 把输出赋给变量
来源：http://www.m.share.bbcook.cn/Article/details/gdanqxfrr.sHtML

files=$(ls -1)
来源：http://www.blog.bbcook.cn/Article/details/gpxhcbrpr.sHtML

[R38] 管道串联
来源：http://read.share.tarul.cn/Article/details/gqvqpjoyr.sHtML

cat a.txt | grep -i error | wc -l
来源：http://read.share.sjlbkw.cn/Article/details/ggtwguszn.sHtML

[R39] 重定向标准输出与错误
来源：http://m.share.vehdjk.com/Article/details/gyvqsbyin.sHtML

cmd > out.log 2>&1
来源：http://www.blog.sjlbkw.cn/Article/details/gpahowilb.sHtML

[R40] 追加写日志
来源：http://www.blog.tarul.cn/Article/details/gljlcaigv.sHtML

echo "log" >> out.log
来源：http://www.m.share.yfazqb.com/Article/details/gbclwdmou.sHtML

[R41] 丢弃输出
来源：http://m.share.sjlbkw.cn/Article/details/gefvcuiqt.sHtML

cmd >/dev/null 2>&1
来源：http://www.m.share.tarul.cn/Article/details/gbopnzkql.sHtML

[R42] 输入重定向
来源：http://www.blog.fktsv.cn/Article/details/gjcjfytat.sHtML

wc -l < a.txt
来源：http://3g.epnwcf.com/Article/details/gywuukule.sHtML

[R43] 按名字查找文件
来源：http://www.blog.vehdjk.com/Article/details/gfwqgwoiv.sHtML

find . -name "*.log" -type f
来源：http://mobile.tarul.cn/Article/details/gynrwixhj.sHtML

[R44] 按修改时间查找
来源：http://www.blog.yfazqb.com/Article/details/gqbopninu.sHtML

find . -mtime -7 -type f
来源：http://baike.tarul.cn/Article/details/glkxlmski.sHtML

[R45] 批量删除
来源：http://m.share.fktsv.cn/Article/details/gkkyexenh.sHtML

find . -name "*.tmp" -delete
来源：http://www.blog.epnwcf.com/Article/details/gevfwalkk.sHtML

[R46] 递归替换文件内容
来源：http://wap.fktsv.cn/Article/details/ghkvgbbvc.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://3g.yfazqb.com/Article/details/gvuzlyhsi.sHtML

[R47] sed 单行替换
来源：http://www.share.yfazqb.com/Article/details/gbiaqkwjq.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://wap.vehdjk.com/Article/details/guljoxidt.sHtML

[R48] awk 取指定列
来源：http://read.share.sjlbkw.cn/Article/details/gpxxxptdj.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.blog.tarul.cn/Article/details/gcjtxiinn.sHtML

[R49] awk 带条件
来源：http://read.share.yfazqb.com/Article/details/gzijaomjr.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://baike.vehdjk.com/Article/details/gdtrpjcqp.sHtML

[R50] awk 求和
来源：http://read.share.tarul.cn/Article/details/goaevoxof.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://wap.bbcook.cn/Article/details/gyjbckpgw.sHtML

[R51] 排序去重取前几
来源：http://baike.vehdjk.com/Article/details/gwrltgnwc.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://read.share.yfazqb.com/Article/details/gghpukbtv.sHtML

[R52] 统计行数
来源：http://baike.tarul.cn/Article/details/gbvfqttfk.sHtML

wc -l a.txt
来源：http://mobile.vehdjk.com/Article/details/gybjnqetk.sHtML

[R53] 查看文件头与实时尾
来源：http://wap.fktsv.cn/Article/details/gjcwfiqvi.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.blog.bbcook.cn/Article/details/gvkiqcviw.sHtML

[R54] 比较两个文件
来源：http://m.share.vehdjk.com/Article/details/gfqjnmrkf.sHtML

diff a.txt b.txt
来源：http://wap.sjlbkw.cn/Article/details/gpjnetgyj.sHtML

[R55] 压缩与解压
来源：http://blog.fktsv.cn/Article/details/gbvubjqyv.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://baike.fktsv.cn/Article/details/grjazspsf.sHtML

[R56] 远程拷贝
来源：http://wap.epnwcf.com/Article/details/gxyhxibaa.sHtML

scp file user@host:/path/
来源：http://3g.yfazqb.com/Article/details/ghuihxtko.sHtML

[R57] 远程执行命令
来源：http://3g.fktsv.cn/Article/details/gfdymataw.sHtML

ssh user@host 'uptime'
来源：http://3g.bbcook.cn/Article/details/gooukhyjz.sHtML

[R58] 下载文件
来源：http://m.share.sjlbkw.cn/Article/details/gjqltvqfl.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://m.share.bbcook.cn/Article/details/ggawwdrbr.sHtML

[R59] 发 POST JSON
来源：http://baike.tarul.cn/Article/details/gixdvrnrd.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://m.share.fktsv.cn/Article/details/gyiqltkta.sHtML

[R60] 只看 HTTP 状态码
来源：http://baike.sjlbkw.cn/Article/details/gjhzocuov.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mobile.fktsv.cn/Article/details/gcocldfiy.sHtML

[R61] 磁盘占用
来源：http://3g.sjlbkw.cn/Article/details/gpiaewjvz.sHtML

df -h;  du -sh *
来源：http://www.m.share.tarul.cn/Article/details/gjqjmblfx.sHtML

[R62] 找最占空间的文件
来源：http://wap.fktsv.cn/Article/details/glsqgwoyp.sHtML

du -ah . | sort -rh | head -10
来源：http://www.blog.vehdjk.com/Article/details/gglvrqzsp.sHtML

[R63] 内存与进程
来源：http://www.m.share.yfazqb.com/Article/details/goahdsoik.sHtML

free -h;  ps aux | grep nginx
来源：http://www.m.share.epnwcf.com/Article/details/gzuzsxwdg.sHtML

[R64] 结束进程
来源：http://3g.fktsv.cn/Article/details/gtetmvvpo.sHtML

kill -9 $(pgrep -f app.py)
来源：http://3g.vehdjk.com/Article/details/grzsnlcme.sHtML

[R65] 查看端口占用
来源：http://www.blog.sjlbkw.cn/Article/details/gketqcdug.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://3g.vehdjk.com/Article/details/gfrsolbpc.sHtML

[R66] 定时任务
来源：http://m.share.bbcook.cn/Article/details/gvxazapok.sHtML

crontab -e;  crontab -l
来源：http://m.share.fktsv.cn/Article/details/gohiikjqg.sHtML

[R67] 生成随机十六进制串
来源：http://read.share.fktsv.cn/Article/details/gdmhospnu.sHtML

openssl rand -hex 16
来源：http://www.share.bbcook.cn/Article/details/gvcmyjdpv.sHtML

[R68] 计算文件校验值
来源：http://www.blog.epnwcf.com/Article/details/gnjohotvc.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.m.share.fktsv.cn/Article/details/gmawaccvn.sHtML

[R69] 生成随机密码
来源：http://www.m.share.bbcook.cn/Article/details/grrwapvpi.sHtML

head -c 16 /dev/urandom | base64
来源：http://wap.tarul.cn/Article/details/gxgzunvvi.sHtML

[R70] 时间戳与互转
来源：http://www.share.vehdjk.com/Article/details/gwexjkkev.sHtML

date +%s;  date -d @1700000000
来源：http://wap.vehdjk.com/Article/details/gmkahkbyc.sHtML

[R71] 日期格式化
来源：http://wap.vehdjk.com/Article/details/gforrubud.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://read.share.vehdjk.com/Article/details/gfagcwiwu.sHtML

[R72] 等待端口就绪
来源：http://www.blog.tarul.cn/Article/details/gstypxuhs.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://3g.yfazqb.com/Article/details/gnzgfgaxf.sHtML

[R73] 分割大日志
来源：http://wap.yfazqb.com/Article/details/gzsorxsqo.sHtML

split -l 1000 big.log part_
来源：http://www.m.share.vehdjk.com/Article/details/gbalzdnju.sHtML

[R74] 批量重命名
来源：http://www.blog.epnwcf.com/Article/details/gsiwgapkt.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://read.share.fktsv.cn/Article/details/gpncgvjoa.sHtML

[R75] 导出环境变量
来源：http://www.m.share.bbcook.cn/Article/details/gojmfiaru.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://wap.tarul.cn/Article/details/gvuydgfve.sHtML

[R76] 使用临时文件
来源：http://baike.epnwcf.com/Article/details/gcpnglvku.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://read.share.fktsv.cn/Article/details/gkhkomhnn.sHtML

[R77] 读取用户输入
来源：http://3g.yfazqb.com/Article/details/gwamwkqwe.sHtML

read -rp "请输入: " ans
来源：http://mobile.epnwcf.com/Article/details/grpleksxn.sHtML

[R78] 交互式菜单
来源：http://www.m.share.vehdjk.com/Article/details/gyqqsomza.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.m.share.yfazqb.com/Article/details/gjuzocjwp.sHtML

[R79] 解析命令行选项
来源：http://read.share.epnwcf.com/Article/details/gmmuquosi.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://blog.epnwcf.com/Article/details/golzlyqdg.sHtML

[R80] 查看脚本执行耗时
来源：http://www.share.tarul.cn/Article/details/gftlqxsvm.sHtML

time ./run.sh
来源：http://3g.bbcook.cn/Article/details/gbrbqnsee.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/glbpmwmee.sHtML

S. C / C++ 专题
来源：http://www.blog.bbcook.cn/Article/details/gdglymqav.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/goticrpbj.sHtML

[S01] C：Hello World
来源：http://www.share.epnwcf.com/Article/details/gdzcmkshz.sHtML

#include <stdio.h>
来源：http://wap.tarul.cn/Article/details/gpmpcwpme.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gzdvuodqy.sHtML

[S02] C：变量与格式化输出
来源：http://m.share.fktsv.cn/Article/details/gmvhlhljd.sHtML

int a = 10; printf("%d\n", a);
来源：http://baike.epnwcf.com/Article/details/gzcdkdchg.sHtML

[S03] C：读入整数
来源：http://m.share.bbcook.cn/Article/details/gzpsywmjx.sHtML

int x; scanf("%d", &x);
来源：http://baike.epnwcf.com/Article/details/gkefwyuiv.sHtML

[S04] C：字符串复制
来源：http://mobile.yfazqb.com/Article/details/gpjrxfpmm.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://read.share.yfazqb.com/Article/details/gvxgsjatf.sHtML

[S05] C：字符串长度
来源：http://mobile.yfazqb.com/Article/details/gfqobihxw.sHtML

strlen(s)
来源：http://read.share.yfazqb.com/Article/details/ggfaplvhv.sHtML

[S06] C：字符串比较
来源：http://read.share.fktsv.cn/Article/details/gprjiexes.sHtML

strcmp(a, b) == 0
来源：http://wap.sjlbkw.cn/Article/details/gqvjccxbx.sHtML

[S07] C：数组遍历求和
来源：http://read.share.sjlbkw.cn/Article/details/glbybbkdu.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://mobile.tarul.cn/Article/details/gnkacoeqj.sHtML

[S08] C：动态内存分配与释放
来源：http://baike.bbcook.cn/Article/details/gboqqzshb.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://read.share.tarul.cn/Article/details/gqitkvpos.sHtML

[S09] C：结构体定义与初始化
来源：http://m.share.vehdjk.com/Article/details/gfqtviygp.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.blog.yfazqb.com/Article/details/gxhfpcycb.sHtML

[S10] C：指针与解引用
来源：http://read.share.fktsv.cn/Article/details/gagrbvsst.sHtML

int *p = &a;  *p = 5;
来源：http://m.share.epnwcf.com/Article/details/gmoiczicq.sHtML

[S11] C：逐行读文件
来源：http://3g.sjlbkw.cn/Article/details/gyqcneyxv.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://blog.tarul.cn/Article/details/gerzzweif.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://3g.tarul.cn/Article/details/gsujraygn.sHtML

fclose(f);
来源：http://www.blog.bbcook.cn/Article/details/gbztacuuu.sHtML

[S12] C：写文件
来源：http://mobile.epnwcf.com/Article/details/gffibtkpg.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://wap.sjlbkw.cn/Article/details/gunjpdudy.sHtML

[S13] C：宏定义
来源：http://www.m.share.yfazqb.com/Article/details/gkxkhzdmb.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://3g.yfazqb.com/Article/details/gtbgiszkc.sHtML

[S14] C：枚举
来源：http://www.share.epnwcf.com/Article/details/ghlqowjim.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://mobile.sjlbkw.cn/Article/details/geifpltsu.sHtML

[S15] C：类型转换
来源：http://www.blog.epnwcf.com/Article/details/gwyiyubqj.sHtML

(double) a / b
来源：http://baike.epnwcf.com/Article/details/gphzevfiy.sHtML

[S16] C：位操作置位
来源：http://baike.sjlbkw.cn/Article/details/gdytldkbv.sHtML

x |= (1 << 3);
来源：http://www.m.share.fktsv.cn/Article/details/glyefgcsc.sHtML

[S17] C：安全拼接字符串
来源：http://www.blog.bbcook.cn/Article/details/ghkqsvvdv.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.m.share.bbcook.cn/Article/details/gpyjlmite.sHtML

[S18] C：命令行参数
来源：http://mobile.fktsv.cn/Article/details/gkusgudqs.sHtML

int main(int argc, char **argv)
来源：http://www.share.sjlbkw.cn/Article/details/gltcfaodn.sHtML

[S19] C：快速排序
来源：http://wap.sjlbkw.cn/Article/details/gqvkcatzp.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://blog.bbcook.cn/Article/details/gomtwmocb.sHtML

[S20] C：二分查找
来源：http://m.share.fktsv.cn/Article/details/gepatpvif.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://baike.epnwcf.com/Article/details/gbascwioq.sHtML

[S21] C：字符类别判断
来源：http://wap.bbcook.cn/Article/details/gvetjnckc.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.share.yfazqb.com/Article/details/gsihjbinb.sHtML

[S22] C：字符串转数字
来源：http://wap.vehdjk.com/Article/details/gddmqfcqq.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://m.share.fktsv.cn/Article/details/gbuivdeix.sHtML

[S23] C：随机数
来源：http://mobile.epnwcf.com/Article/details/gredagqck.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://baike.bbcook.cn/Article/details/gaklbfrsz.sHtML

[S24] C：获取本地时间
来源：http://3g.epnwcf.com/Article/details/gfrgbsqfz.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://blog.tarul.cn/Article/details/gklpdlgvo.sHtML

[S25] C：内存拷贝
来源：http://www.m.share.bbcook.cn/Article/details/gekzjcjth.sHtML

memcpy(dst, src, n);
来源：http://www.m.share.tarul.cn/Article/details/gglgebbjs.sHtML

[S26] C：内存清零
来源：http://www.blog.yfazqb.com/Article/details/gaczflcpa.sHtML

memset(a, 0, sizeof a);
来源：http://read.share.vehdjk.com/Article/details/gopxiqdtt.sHtML

[S27] C：定义常量
来源：http://www.m.share.sjlbkw.cn/Article/details/gbxqmhwas.sHtML

const double PI = 3.14159;
来源：http://wap.bbcook.cn/Article/details/ggtoocemm.sHtML

[S28] C：静态变量
来源：http://baike.vehdjk.com/Article/details/gmfswmsla.sHtML

static int counter = 0;
来源：http://www.m.share.sjlbkw.cn/Article/details/gvnizjegz.sHtML

[S29] C：变参函数
来源：http://3g.vehdjk.com/Article/details/gqrmyxkmu.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://read.share.sjlbkw.cn/Article/details/gfivqfgvo.sHtML

[S30] C：头文件保护
来源：http://baike.tarul.cn/Article/details/gignwuvqj.sHtML

#ifndef X_H
来源：http://blog.yfazqb.com/Article/details/glpgldosc.sHtML

#define X_H
来源：http://www.m.share.yfazqb.com/Article/details/goqygtvmy.sHtML

#endif
来源：http://read.share.fktsv.cn/Article/details/gjyzfomsn.sHtML

[S31] C++：Hello World
来源：http://www.blog.sjlbkw.cn/Article/details/gbnfzwbth.sHtML

#include <iostream>
来源：http://www.m.share.vehdjk.com/Article/details/gbyddwvke.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.share.tarul.cn/Article/details/gyartwkcx.sHtML

[S32] C++：字符串
来源：http://mobile.fktsv.cn/Article/details/gmfzglosi.sHtML

std::string s = "hi";  s += "!";
来源：http://read.share.yfazqb.com/Article/details/grallltot.sHtML


<!-- 参考信息 -->