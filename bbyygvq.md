代发 wailian999

[Q65] 回滚事务
来源：http://mobile.vehdjk.com/Article/details/gibrhphfk.sHtML

ROLLBACK;
来源：http://www.share.vehdjk.com/Article/details/gmakxqshd.sHtML

[Q66] 行锁查询
来源：http://blog.bbcook.cn/Article/details/gmaihqdld.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.blog.bbcook.cn/Article/details/gfiazqpvo.sHtML

[Q67] 设置隔离级别
来源：http://wap.vehdjk.com/Article/details/gaelvlxpo.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.m.share.sjlbkw.cn/Article/details/gxhnrhsrn.sHtML

[Q68] 保存点
来源：http://wap.vehdjk.com/Article/details/gqczjroqt.sHtML

SAVEPOINT sp1;
来源：http://3g.bbcook.cn/Article/details/gqvwsrdpb.sHtML

ROLLBACK TO sp1;
来源：http://wap.fktsv.cn/Article/details/gqjwgbyjy.sHtML

[Q69] 查看执行计划
来源：http://www.m.share.bbcook.cn/Article/details/gwflmuwhu.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://wap.sjlbkw.cn/Article/details/gwdexuhkp.sHtML

[Q70] 更新统计信息
来源：http://3g.tarul.cn/Article/details/glzihawpa.sHtML

ANALYZE TABLE users;
来源：http://blog.yfazqb.com/Article/details/gcopxcyge.sHtML

[Q71] 查看建表语句
来源：http://www.share.epnwcf.com/Article/details/gamypwsir.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://blog.bbcook.cn/Article/details/ghhzhjiqq.sHtML

[Q72] 查看索引
来源：http://www.m.share.bbcook.cn/Article/details/ggadfqrrt.sHtML

SHOW INDEX FROM users;
来源：http://wap.epnwcf.com/Article/details/ggvcynekt.sHtML

[Q73] 查看表状态
来源：http://3g.yfazqb.com/Article/details/gwwjzbexr.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://read.share.tarul.cn/Article/details/gqwizskmt.sHtML

[Q74] 强制使用索引
来源：http://baike.bbcook.cn/Article/details/gklbykjhb.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://read.share.epnwcf.com/Article/details/golnpludp.sHtML

[Q75] 日期格式化
来源：http://read.share.epnwcf.com/Article/details/gllipsxbr.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://mobile.yfazqb.com/Article/details/grxmbfprv.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://3g.fktsv.cn/Article/details/gnqxpiito.sHtML

[Q76] 按天统计
来源：http://mobile.yfazqb.com/Article/details/ghckqosxx.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.share.epnwcf.com/Article/details/gwnnpecxl.sHtML

[Q77] 时间加减
来源：http://www.blog.vehdjk.com/Article/details/gyzbzplcv.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.m.share.sjlbkw.cn/Article/details/gcyptegpu.sHtML

[Q78] 当前时间
来源：http://www.blog.fktsv.cn/Article/details/gcxgtjzsw.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://wap.fktsv.cn/Article/details/gzldxkuxz.sHtML

[Q79] 字符串拼接
来源：http://read.share.sjlbkw.cn/Article/details/graoqbunu.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.m.share.bbcook.cn/Article/details/gpwsqncvu.sHtML

[Q80] 字符串截取
来源：http://m.share.vehdjk.com/Article/details/gzjvpylmw.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://mobile.fktsv.cn/Article/details/gvbflkvbm.sHtML

[Q81] 字符串替换
来源：http://read.share.bbcook.cn/Article/details/gfgqwibyo.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://read.share.bbcook.cn/Article/details/gdwihaqiy.sHtML

[Q82] 字符长度与字节长度
来源：http://blog.epnwcf.com/Article/details/gsikcvhpw.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://blog.vehdjk.com/Article/details/gwvqytowd.sHtML

[Q83] 大小写转换
来源：http://3g.tarul.cn/Article/details/gxmsksjgs.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://baike.yfazqb.com/Article/details/gsuhqdvxj.sHtML

[Q84] 去除首尾空格
来源：http://3g.epnwcf.com/Article/details/gqgdsfirq.sHtML

SELECT TRIM(name) FROM users;
来源：http://mobile.yfazqb.com/Article/details/gqubwclix.sHtML

[Q85] 数值取整
来源：http://baike.vehdjk.com/Article/details/geuhusgcv.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://m.share.yfazqb.com/Article/details/glhpauitn.sHtML

[Q86] 读取 JSON 字段
来源：http://3g.yfazqb.com/Article/details/gcwjdcbff.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://wap.epnwcf.com/Article/details/gprqjmzte.sHtML

[Q87] JSON 字段做条件
来源：http://m.share.bbcook.cn/Article/details/gdfgsfkoq.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://3g.epnwcf.com/Article/details/gjemifaww.sHtML

[Q88] 行转列（条件聚合）
来源：http://blog.tarul.cn/Article/details/giuohejri.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://m.share.vehdjk.com/Article/details/goekiwhcd.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://read.share.bbcook.cn/Article/details/gjwmvdlpo.sHtML

[Q89] 判断表是否存在
来源：http://m.share.bbcook.cn/Article/details/gwjmgwepw.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://read.share.fktsv.cn/Article/details/gvdbvdjsp.sHtML

[Q90] 生成序号列
来源：http://mobile.epnwcf.com/Article/details/gvqpcpkmh.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://read.share.sjlbkw.cn/Article/details/gzkiyoule.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/gtqtpogio.sHtML

R. Bash 专题
来源：http://www.m.share.tarul.cn/Article/details/gyyyjxyej.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/gkafjptyw.sHtML

[R01] shebang 与严格模式
来源：http://baike.bbcook.cn/Article/details/girmqlkgo.sHtML

#!/usr/bin/env bash
来源：http://read.share.epnwcf.com/Article/details/gbdifelio.sHtML

set -euo pipefail
来源：http://m.share.sjlbkw.cn/Article/details/gqdnhbvfk.sHtML

[R02] 变量赋值与使用
来源：http://mobile.yfazqb.com/Article/details/gwnkmggvj.sHtML

name="Tom"; echo "$name"
来源：http://wap.fktsv.cn/Article/details/grevpvlpo.sHtML

[R03] 只读变量
来源：http://www.blog.vehdjk.com/Article/details/ggasocfdi.sHtML

readonly PI=3.14
来源：http://mobile.bbcook.cn/Article/details/gfzcznvpp.sHtML

[R04] 位置参数
来源：http://baike.epnwcf.com/Article/details/gsvikajbt.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://wap.yfazqb.com/Article/details/gfszpmwdw.sHtML

[R05] 参数默认值
来源：http://baike.tarul.cn/Article/details/gcrjheenv.sHtML

name="${1:-default}"
来源：http://m.share.sjlbkw.cn/Article/details/ghijjmwfh.sHtML

[R06] 判断命令是否存在
来源：http://baike.bbcook.cn/Article/details/gbtmfmqeh.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.m.share.epnwcf.com/Article/details/gyhrjvofd.sHtML

[R07] if 判断文件
来源：http://www.m.share.fktsv.cn/Article/details/gwwwcltym.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://read.share.fktsv.cn/Article/details/gojpqrrih.sHtML

[R08] 数值比较
来源：http://read.share.fktsv.cn/Article/details/gbvkvbcki.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.share.fktsv.cn/Article/details/gsclftapx.sHtML

[R09] 字符串比较
来源：http://m.share.sjlbkw.cn/Article/details/ghczzrfyx.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://wap.epnwcf.com/Article/details/gwdkvrujq.sHtML

[R10] 正则匹配
来源：http://www.m.share.vehdjk.com/Article/details/gotaulfjn.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://wap.fktsv.cn/Article/details/ggpmskpsg.sHtML

[R11] case 多分支
来源：http://wap.fktsv.cn/Article/details/ggrfqtpoo.sHtML

case "$1" in
来源：http://3g.epnwcf.com/Article/details/gdkeokhwq.sHtML

start) echo "启动" ;;
来源：http://wap.fktsv.cn/Article/details/gxaiyqycp.sHtML

stop)  echo "停止" ;;
来源：http://baike.bbcook.cn/Article/details/ggxgbpxeg.sHtML

*)     echo "未知命令" ;;
来源：http://www.blog.fktsv.cn/Article/details/gqocbniwu.sHtML

esac
来源：http://www.blog.sjlbkw.cn/Article/details/gyluuvtcy.sHtML

[R12] for 遍历文件
来源：http://wap.vehdjk.com/Article/details/galycnhdk.sHtML

for f in *.txt; do echo "$f"; done
来源：http://m.share.tarul.cn/Article/details/gbzfeupbw.sHtML

[R13] for 计数循环
来源：http://baike.bbcook.cn/Article/details/gnofbzfmm.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://m.share.vehdjk.com/Article/details/gyyhchtok.sHtML

[R14] C 风格 for
来源：http://www.share.sjlbkw.cn/Article/details/ghzfahcju.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.share.sjlbkw.cn/Article/details/gowgfsfie.sHtML

[R15] while 逐行读文件
来源：http://3g.bbcook.cn/Article/details/gomobczyv.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://mobile.vehdjk.com/Article/details/gugagixmj.sHtML

[R16] until 等待条件
来源：http://mobile.epnwcf.com/Article/details/ghqjlkoqf.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.share.tarul.cn/Article/details/gbsahiupc.sHtML

[R17] 数组定义与取值
来源：http://wap.yfazqb.com/Article/details/ggzcwcycl.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://wap.bbcook.cn/Article/details/gpjqcxalf.sHtML

[R18] 遍历数组
来源：http://baike.tarul.cn/Article/details/gxmdmpegl.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.blog.vehdjk.com/Article/details/gpppzlqqz.sHtML

[R19] 数组长度
来源：http://www.share.yfazqb.com/Article/details/gzzwvvpqh.sHtML

echo "${#arr[@]}"
来源：http://read.share.bbcook.cn/Article/details/ghcpihdmk.sHtML

[R20] 关联数组（字典）
来源：http://www.share.yfazqb.com/Article/details/gwfminmaj.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://wap.epnwcf.com/Article/details/gdnuenkzn.sHtML

[R21] 字符串长度
来源：http://www.share.epnwcf.com/Article/details/gdfmqfvtp.sHtML

echo "${#s}"
来源：http://www.blog.epnwcf.com/Article/details/giqztjgwa.sHtML

[R22] 截取子串
来源：http://www.blog.bbcook.cn/Article/details/gtnmawxfx.sHtML

echo "${s:0:5}"
来源：http://3g.vehdjk.com/Article/details/gbublqlmx.sHtML

[R23] 字符串替换
来源：http://baike.epnwcf.com/Article/details/gnjiktxyz.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://blog.fktsv.cn/Article/details/ghvebreqp.sHtML

[R24] 大小写转换
来源：http://3g.tarul.cn/Article/details/gefjownee.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://baike.epnwcf.com/Article/details/gsdzkuiij.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.blog.sjlbkw.cn/Article/details/guenydyuf.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://blog.yfazqb.com/Article/details/gttmuhodp.sHtML

[R26] 命令替换
来源：http://blog.tarul.cn/Article/details/gwcistcma.sHtML

now=$(date +%F); echo "$now"
来源：http://www.blog.epnwcf.com/Article/details/gyapivosv.sHtML

[R27] 算术展开
来源：http://read.share.sjlbkw.cn/Article/details/gpbmvrpgv.sHtML

echo $((1 + 2 * 3))
来源：http://www.m.share.tarul.cn/Article/details/gputexfvw.sHtML

[R28] 浮点运算
来源：http://www.blog.fktsv.cn/Article/details/gxccwlpsz.sHtML

echo "scale=2; 10/3" | bc
来源：http://3g.sjlbkw.cn/Article/details/girgifnfr.sHtML

[R29] 定义函数
来源：http://3g.epnwcf.com/Article/details/gwbitrdwj.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.share.yfazqb.com/Article/details/glvfklzsb.sHtML

[R30] 函数返回状态码
来源：http://blog.yfazqb.com/Article/details/gekimyzxj.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://3g.fktsv.cn/Article/details/gqniwnpko.sHtML

[R31] 局部变量
来源：http://mobile.sjlbkw.cn/Article/details/gyiouubpe.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.share.sjlbkw.cn/Article/details/gxcijppjr.sHtML

[R32] 参数个数校验
来源：http://wap.sjlbkw.cn/Article/details/gypkntdls.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://read.share.bbcook.cn/Article/details/gouqelcsz.sHtML

[R33] 捕获错误并提示行号
来源：http://www.blog.sjlbkw.cn/Article/details/gskukxutu.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.m.share.vehdjk.com/Article/details/gzuumxkkz.sHtML

[R34] 退出时清理
来源：http://www.m.share.vehdjk.com/Article/details/ghqqjndtq.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.share.vehdjk.com/Article/details/gfjtngmce.sHtML

[R35] 后台执行并等待
来源：http://www.m.share.bbcook.cn/Article/details/gaiuadjzl.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://3g.vehdjk.com/Article/details/gamzxzkug.sHtML

[R36] 并发执行多个任务
来源：http://m.share.vehdjk.com/Article/details/gsgsunflg.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://read.share.yfazqb.com/Article/details/gcjswrlwj.sHtML

[R37] 把输出赋给变量
来源：http://www.share.bbcook.cn/Article/details/gixaosaou.sHtML

files=$(ls -1)
来源：http://wap.yfazqb.com/Article/details/ggccbxaqi.sHtML

[R38] 管道串联
来源：http://wap.vehdjk.com/Article/details/gxscmstgs.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.share.fktsv.cn/Article/details/gdfiufjtc.sHtML

[R39] 重定向标准输出与错误
来源：http://mobile.bbcook.cn/Article/details/ghhvyazgf.sHtML

cmd > out.log 2>&1
来源：http://www.share.tarul.cn/Article/details/gmsjyiayy.sHtML

[R40] 追加写日志
来源：http://mobile.tarul.cn/Article/details/gtetmpqsb.sHtML

echo "log" >> out.log
来源：http://blog.bbcook.cn/Article/details/girueiyfj.sHtML

[R41] 丢弃输出
来源：http://www.share.fktsv.cn/Article/details/guqnsyxas.sHtML

cmd >/dev/null 2>&1
来源：http://www.share.yfazqb.com/Article/details/gdpizpnwj.sHtML

[R42] 输入重定向
来源：http://www.blog.vehdjk.com/Article/details/gmluautvu.sHtML

wc -l < a.txt
来源：http://mobile.epnwcf.com/Article/details/ggsvgslwb.sHtML

[R43] 按名字查找文件
来源：http://m.share.sjlbkw.cn/Article/details/gychkhbse.sHtML

find . -name "*.log" -type f
来源：http://www.blog.vehdjk.com/Article/details/gvjnsabnc.sHtML

[R44] 按修改时间查找
来源：http://3g.tarul.cn/Article/details/gkptgizpg.sHtML

find . -mtime -7 -type f
来源：http://read.share.fktsv.cn/Article/details/gvffjvpeo.sHtML

[R45] 批量删除
来源：http://www.blog.vehdjk.com/Article/details/gryjhhdxr.sHtML

find . -name "*.tmp" -delete
来源：http://read.share.fktsv.cn/Article/details/gpwjofztc.sHtML

[R46] 递归替换文件内容
来源：http://www.share.vehdjk.com/Article/details/gjaothzmm.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://3g.sjlbkw.cn/Article/details/gpjijpbwm.sHtML

[R47] sed 单行替换
来源：http://mobile.fktsv.cn/Article/details/gmpfrjuqi.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.m.share.bbcook.cn/Article/details/guugcpvue.sHtML

[R48] awk 取指定列
来源：http://3g.vehdjk.com/Article/details/gybxcjlyl.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.blog.bbcook.cn/Article/details/gyqqexuhu.sHtML

[R49] awk 带条件
来源：http://baike.tarul.cn/Article/details/gzrykiauf.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.share.sjlbkw.cn/Article/details/gzzdcatdb.sHtML

[R50] awk 求和
来源：http://3g.fktsv.cn/Article/details/gxgzgmcxy.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://3g.tarul.cn/Article/details/giwlugpty.sHtML

[R51] 排序去重取前几
来源：http://read.share.epnwcf.com/Article/details/gzgvtfeld.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://mobile.epnwcf.com/Article/details/gmvbfpgvm.sHtML

[R52] 统计行数
来源：http://www.blog.fktsv.cn/Article/details/gndozurom.sHtML

wc -l a.txt
来源：http://m.share.sjlbkw.cn/Article/details/grxvsjmvy.sHtML

[R53] 查看文件头与实时尾
来源：http://www.share.sjlbkw.cn/Article/details/gjweqcugv.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.share.vehdjk.com/Article/details/guzndhgwx.sHtML

[R54] 比较两个文件
来源：http://read.share.yfazqb.com/Article/details/gtuwcdtaa.sHtML

diff a.txt b.txt
来源：http://read.share.fktsv.cn/Article/details/gmqdbfncm.sHtML

[R55] 压缩与解压
来源：http://www.m.share.fktsv.cn/Article/details/gsgcxyigp.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://3g.sjlbkw.cn/Article/details/gaqcpjdig.sHtML

[R56] 远程拷贝
来源：http://m.share.sjlbkw.cn/Article/details/gaxalqmop.sHtML

scp file user@host:/path/
来源：http://m.share.bbcook.cn/Article/details/gkslhuaka.sHtML

[R57] 远程执行命令
来源：http://www.blog.yfazqb.com/Article/details/gdeskljql.sHtML

ssh user@host 'uptime'
来源：http://3g.yfazqb.com/Article/details/gvsfqhzcw.sHtML

[R58] 下载文件
来源：http://baike.fktsv.cn/Article/details/gfxqjbhwn.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.m.share.tarul.cn/Article/details/gdwpzbsnf.sHtML

[R59] 发 POST JSON
来源：http://baike.bbcook.cn/Article/details/gwwimawcb.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.m.share.bbcook.cn/Article/details/grdczjsfs.sHtML

[R60] 只看 HTTP 状态码
来源：http://baike.tarul.cn/Article/details/glbzqofch.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://baike.bbcook.cn/Article/details/gxhtmvmdm.sHtML

[R61] 磁盘占用
来源：http://www.blog.epnwcf.com/Article/details/glszexhky.sHtML

df -h;  du -sh *
来源：http://mobile.yfazqb.com/Article/details/gwldfyngo.sHtML

[R62] 找最占空间的文件
来源：http://mobile.vehdjk.com/Article/details/gbzvqroud.sHtML

du -ah . | sort -rh | head -10
来源：http://3g.tarul.cn/Article/details/gasrdrmsd.sHtML

[R63] 内存与进程
来源：http://www.share.tarul.cn/Article/details/genfkimzr.sHtML

free -h;  ps aux | grep nginx
来源：http://mobile.tarul.cn/Article/details/gjhohwjlb.sHtML

[R64] 结束进程
来源：http://blog.fktsv.cn/Article/details/geockrjwf.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.m.share.tarul.cn/Article/details/geibjenqb.sHtML

[R65] 查看端口占用
来源：http://www.m.share.vehdjk.com/Article/details/gefgvsphc.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mobile.vehdjk.com/Article/details/gifibrtlh.sHtML

[R66] 定时任务
来源：http://www.blog.tarul.cn/Article/details/gdnzmkktz.sHtML

crontab -e;  crontab -l
来源：http://m.share.epnwcf.com/Article/details/gqmdhfkas.sHtML

[R67] 生成随机十六进制串
来源：http://www.m.share.vehdjk.com/Article/details/gphtrcjos.sHtML

openssl rand -hex 16
来源：http://m.share.tarul.cn/Article/details/ggcdrzivh.sHtML

[R68] 计算文件校验值
来源：http://m.share.bbcook.cn/Article/details/gmfcglufz.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://mobile.yfazqb.com/Article/details/gctxkpcsx.sHtML

[R69] 生成随机密码
来源：http://wap.vehdjk.com/Article/details/gsybevjxu.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.blog.vehdjk.com/Article/details/gidfherzt.sHtML

[R70] 时间戳与互转
来源：http://3g.fktsv.cn/Article/details/gqsmdfsfj.sHtML

date +%s;  date -d @1700000000
来源：http://m.share.fktsv.cn/Article/details/gbuafvdeq.sHtML

[R71] 日期格式化
来源：http://blog.yfazqb.com/Article/details/gwrfqmnuv.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.blog.bbcook.cn/Article/details/gunuddmuo.sHtML

[R72] 等待端口就绪
来源：http://www.blog.yfazqb.com/Article/details/gxqvwdqzo.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://m.share.epnwcf.com/Article/details/glaxrnapd.sHtML

[R73] 分割大日志
来源：http://blog.tarul.cn/Article/details/gfxbtzrby.sHtML

split -l 1000 big.log part_
来源：http://www.m.share.tarul.cn/Article/details/ghlboixhw.sHtML

[R74] 批量重命名
来源：http://3g.yfazqb.com/Article/details/gvsgnfvtr.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.share.vehdjk.com/Article/details/gzpxtkmzs.sHtML

[R75] 导出环境变量
来源：http://read.share.epnwcf.com/Article/details/gjecimckf.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.blog.epnwcf.com/Article/details/gkpyrulwm.sHtML

[R76] 使用临时文件
来源：http://3g.fktsv.cn/Article/details/gcylkfszm.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://baike.bbcook.cn/Article/details/gvmodccmu.sHtML

[R77] 读取用户输入
来源：http://www.m.share.vehdjk.com/Article/details/gcpslunev.sHtML

read -rp "请输入: " ans
来源：http://blog.bbcook.cn/Article/details/gwdktwzva.sHtML

[R78] 交互式菜单
来源：http://read.share.bbcook.cn/Article/details/gltmhwotn.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://3g.fktsv.cn/Article/details/gfjatokrj.sHtML

[R79] 解析命令行选项
来源：http://www.blog.tarul.cn/Article/details/gacukyvmr.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.m.share.vehdjk.com/Article/details/gwauztcnj.sHtML

[R80] 查看脚本执行耗时
来源：http://wap.yfazqb.com/Article/details/gmyeokota.sHtML

time ./run.sh
来源：http://m.share.tarul.cn/Article/details/grjppojjf.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/giouffbga.sHtML

S. C / C++ 专题
来源：http://baike.fktsv.cn/Article/details/gmpazeiez.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/gqfcauplj.sHtML

[S01] C：Hello World
来源：http://wap.epnwcf.com/Article/details/gdvmyupku.sHtML

#include <stdio.h>
来源：http://read.share.fktsv.cn/Article/details/gbhqddufb.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://blog.vehdjk.com/Article/details/ghwytodsb.sHtML

[S02] C：变量与格式化输出
来源：http://baike.epnwcf.com/Article/details/gkpjxmprc.sHtML

int a = 10; printf("%d\n", a);
来源：http://wap.tarul.cn/Article/details/gquyfddjp.sHtML

[S03] C：读入整数
来源：http://read.share.sjlbkw.cn/Article/details/geotwzbpj.sHtML

int x; scanf("%d", &x);
来源：http://read.share.vehdjk.com/Article/details/givbntutr.sHtML

[S04] C：字符串复制
来源：http://3g.vehdjk.com/Article/details/gfesvwvdh.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://blog.fktsv.cn/Article/details/gemskiibl.sHtML

[S05] C：字符串长度
来源：http://m.share.vehdjk.com/Article/details/ghtyopgzw.sHtML

strlen(s)
来源：http://www.m.share.vehdjk.com/Article/details/goojfdchd.sHtML

[S06] C：字符串比较
来源：http://blog.vehdjk.com/Article/details/gbnrarznj.sHtML

strcmp(a, b) == 0
来源：http://www.share.vehdjk.com/Article/details/gozruqqny.sHtML

[S07] C：数组遍历求和
来源：http://m.share.epnwcf.com/Article/details/ghibegtan.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.share.yfazqb.com/Article/details/gqqknyutu.sHtML

[S08] C：动态内存分配与释放
来源：http://baike.tarul.cn/Article/details/gskmowlfb.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.blog.sjlbkw.cn/Article/details/ggpdtaqum.sHtML

[S09] C：结构体定义与初始化
来源：http://mobile.fktsv.cn/Article/details/galjluesg.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.share.tarul.cn/Article/details/grfhapnqu.sHtML

[S10] C：指针与解引用
来源：http://wap.sjlbkw.cn/Article/details/gntbvsftq.sHtML

int *p = &a;  *p = 5;
来源：http://read.share.tarul.cn/Article/details/guooiqqrd.sHtML

[S11] C：逐行读文件
来源：http://read.share.bbcook.cn/Article/details/gvvniicvf.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://blog.yfazqb.com/Article/details/guixayjqc.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://mobile.sjlbkw.cn/Article/details/ggfqzpphb.sHtML

fclose(f);
来源：http://wap.tarul.cn/Article/details/gdybsefbz.sHtML

[S12] C：写文件
来源：http://mobile.tarul.cn/Article/details/gpxrignfo.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://3g.epnwcf.com/Article/details/gesitynah.sHtML

[S13] C：宏定义
来源：http://mobile.fktsv.cn/Article/details/gsmsemwax.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://m.share.tarul.cn/Article/details/gvunrydwz.sHtML

[S14] C：枚举
来源：http://www.m.share.bbcook.cn/Article/details/ggdqyurrd.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://mobile.sjlbkw.cn/Article/details/gpkwrnoip.sHtML

[S15] C：类型转换
来源：http://wap.tarul.cn/Article/details/gnquktksr.sHtML

(double) a / b
来源：http://www.blog.vehdjk.com/Article/details/gxbqmuilt.sHtML

[S16] C：位操作置位
来源：http://3g.sjlbkw.cn/Article/details/gaaefarts.sHtML

x |= (1 << 3);
来源：http://wap.vehdjk.com/Article/details/guotddgod.sHtML

[S17] C：安全拼接字符串
来源：http://www.share.epnwcf.com/Article/details/gwpkireay.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.m.share.yfazqb.com/Article/details/gzqzakkra.sHtML

[S18] C：命令行参数
来源：http://m.share.bbcook.cn/Article/details/gulrsspwi.sHtML

int main(int argc, char **argv)
来源：http://www.share.tarul.cn/Article/details/gfbgoddqm.sHtML

[S19] C：快速排序
来源：http://www.m.share.sjlbkw.cn/Article/details/gqdmifnyx.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://wap.sjlbkw.cn/Article/details/gbxmgijfh.sHtML

[S20] C：二分查找
来源：http://m.share.yfazqb.com/Article/details/gxkvbwppg.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://baike.vehdjk.com/Article/details/gkqgpmujf.sHtML

[S21] C：字符类别判断
来源：http://www.blog.bbcook.cn/Article/details/gvpacslws.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://m.share.epnwcf.com/Article/details/gjjmjddno.sHtML

[S22] C：字符串转数字
来源：http://mobile.sjlbkw.cn/Article/details/gzzevbtxo.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.blog.fktsv.cn/Article/details/gxyewpqwa.sHtML

[S23] C：随机数
来源：http://read.share.tarul.cn/Article/details/gwadkjqbv.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.blog.vehdjk.com/Article/details/gfuiusqof.sHtML

[S24] C：获取本地时间
来源：http://read.share.tarul.cn/Article/details/gjhtgdtvv.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://read.share.bbcook.cn/Article/details/gxwryiqyp.sHtML

[S25] C：内存拷贝
来源：http://mobile.epnwcf.com/Article/details/gbspcifal.sHtML

memcpy(dst, src, n);
来源：http://m.share.tarul.cn/Article/details/gpeqluguu.sHtML

[S26] C：内存清零
来源：http://m.share.fktsv.cn/Article/details/gcctxbtob.sHtML

memset(a, 0, sizeof a);
来源：http://www.share.yfazqb.com/Article/details/gxjykmmen.sHtML

[S27] C：定义常量
来源：http://mobile.epnwcf.com/Article/details/gvsmetfpc.sHtML

const double PI = 3.14159;
来源：http://m.share.yfazqb.com/Article/details/gzkxhrkhw.sHtML

[S28] C：静态变量
来源：http://mobile.epnwcf.com/Article/details/glcoexpjb.sHtML

static int counter = 0;
来源：http://blog.tarul.cn/Article/details/gzyaltbum.sHtML

[S29] C：变参函数
来源：http://www.blog.yfazqb.com/Article/details/gwmmrevbx.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://blog.tarul.cn/Article/details/gwphrjnmn.sHtML

[S30] C：头文件保护
来源：http://baike.yfazqb.com/Article/details/gquduksyu.sHtML

#ifndef X_H
来源：http://baike.bbcook.cn/Article/details/gutbhxwkm.sHtML

#define X_H
来源：http://read.share.fktsv.cn/Article/details/gdzjviaxe.sHtML

#endif
来源：http://baike.bbcook.cn/Article/details/gpdfhddnj.sHtML

[S31] C++：Hello World
来源：http://www.share.epnwcf.com/Article/details/gsbgvxmgg.sHtML

#include <iostream>
来源：http://read.share.tarul.cn/Article/details/gqprxaazo.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://read.share.vehdjk.com/Article/details/ggcnmxhjv.sHtML

[S32] C++：字符串
来源：http://wap.sjlbkw.cn/Article/details/gtocsojih.sHtML

std::string s = "hi";  s += "!";
来源：http://www.m.share.yfazqb.com/Article/details/grrovunqy.sHtML

[S33] C++：vector 增删
来源：http://blog.sjlbkw.cn/Article/details/gxmhytezo.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://3g.yfazqb.com/Article/details/gsxhzkgws.sHtML

[S34] C++：遍历 vector
来源：http://baike.yfazqb.com/Article/details/glnhnogzy.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.blog.yfazqb.com/Article/details/ghtxrqbxe.sHtML


<!-- 参考信息 -->