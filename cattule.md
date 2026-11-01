代发 wailian999

[Q65] 回滚事务
来源：http://3g.epnwcf.com/Article/details/gfwitfgov.sHtML

ROLLBACK;
来源：http://wap.vehdjk.com/Article/details/gxczirrmn.sHtML

[Q66] 行锁查询
来源：http://baike.yfazqb.com/Article/details/gxztdnduk.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.m.share.bbcook.cn/Article/details/ghndgxauu.sHtML

[Q67] 设置隔离级别
来源：http://www.blog.sjlbkw.cn/Article/details/giocjacrw.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.blog.yfazqb.com/Article/details/gszashsmq.sHtML

[Q68] 保存点
来源：http://baike.fktsv.cn/Article/details/gpysgjnhc.sHtML

SAVEPOINT sp1;
来源：http://www.share.vehdjk.com/Article/details/ghspjidze.sHtML

ROLLBACK TO sp1;
来源：http://www.blog.tarul.cn/Article/details/gtyuwogks.sHtML

[Q69] 查看执行计划
来源：http://baike.yfazqb.com/Article/details/gdpzlavqr.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://blog.vehdjk.com/Article/details/gujbolrvu.sHtML

[Q70] 更新统计信息
来源：http://mobile.bbcook.cn/Article/details/gssjdnpcn.sHtML

ANALYZE TABLE users;
来源：http://baike.sjlbkw.cn/Article/details/gsfzfvsvk.sHtML

[Q71] 查看建表语句
来源：http://www.m.share.vehdjk.com/Article/details/giwjkbodf.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://blog.epnwcf.com/Article/details/gzcwyukvw.sHtML

[Q72] 查看索引
来源：http://mobile.epnwcf.com/Article/details/ghsjefndq.sHtML

SHOW INDEX FROM users;
来源：http://3g.epnwcf.com/Article/details/gnjsclqna.sHtML

[Q73] 查看表状态
来源：http://mobile.tarul.cn/Article/details/gplqnhqat.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.blog.fktsv.cn/Article/details/gwpsooxtv.sHtML

[Q74] 强制使用索引
来源：http://mobile.tarul.cn/Article/details/gkkibbpku.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://mobile.epnwcf.com/Article/details/goztewkse.sHtML

[Q75] 日期格式化
来源：http://read.share.fktsv.cn/Article/details/gpaydssun.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://3g.yfazqb.com/Article/details/gwpalfcmd.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://baike.epnwcf.com/Article/details/gnqhcdvnr.sHtML

[Q76] 按天统计
来源：http://m.share.yfazqb.com/Article/details/gdestbfua.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://wap.sjlbkw.cn/Article/details/gnwbopqvj.sHtML

[Q77] 时间加减
来源：http://mobile.epnwcf.com/Article/details/gibhieefb.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://baike.tarul.cn/Article/details/gkqvkycyy.sHtML

[Q78] 当前时间
来源：http://blog.tarul.cn/Article/details/gkslyutul.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.m.share.tarul.cn/Article/details/gduwysrvp.sHtML

[Q79] 字符串拼接
来源：http://www.m.share.yfazqb.com/Article/details/grvvytlzp.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://baike.epnwcf.com/Article/details/gculzvozh.sHtML

[Q80] 字符串截取
来源：http://m.share.epnwcf.com/Article/details/gxklqyqfn.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.blog.epnwcf.com/Article/details/goemmhqkl.sHtML

[Q81] 字符串替换
来源：http://blog.sjlbkw.cn/Article/details/gtqibwczd.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.blog.sjlbkw.cn/Article/details/gtyxhvmta.sHtML

[Q82] 字符长度与字节长度
来源：http://baike.tarul.cn/Article/details/gcfjcluvt.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.blog.fktsv.cn/Article/details/gprhbfisr.sHtML

[Q83] 大小写转换
来源：http://wap.vehdjk.com/Article/details/gzejodzhy.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://baike.bbcook.cn/Article/details/gmjzcazbt.sHtML

[Q84] 去除首尾空格
来源：http://www.m.share.tarul.cn/Article/details/gmcvpdfjb.sHtML

SELECT TRIM(name) FROM users;
来源：http://read.share.bbcook.cn/Article/details/gqrdhqltv.sHtML

[Q85] 数值取整
来源：http://baike.tarul.cn/Article/details/ghrwythju.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://m.share.sjlbkw.cn/Article/details/gvyhzamez.sHtML

[Q86] 读取 JSON 字段
来源：http://mobile.tarul.cn/Article/details/gtasezpws.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://wap.epnwcf.com/Article/details/gdvaufijo.sHtML

[Q87] JSON 字段做条件
来源：http://mobile.bbcook.cn/Article/details/gjgoofqzi.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.blog.fktsv.cn/Article/details/gcfcdorcu.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.blog.bbcook.cn/Article/details/gqghxynxc.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://mobile.tarul.cn/Article/details/gmovjovyw.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://mobile.vehdjk.com/Article/details/gvbbkxqsv.sHtML

[Q89] 判断表是否存在
来源：http://read.share.bbcook.cn/Article/details/grkpuqczg.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://baike.fktsv.cn/Article/details/gwzhxwvgs.sHtML

[Q90] 生成序号列
来源：http://read.share.vehdjk.com/Article/details/gbyowqugs.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://baike.bbcook.cn/Article/details/gwnjwutat.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/gjhwwkrmx.sHtML

R. Bash 专题
来源：http://read.share.bbcook.cn/Article/details/gpfigttxm.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/goardqlpc.sHtML

[R01] shebang 与严格模式
来源：http://www.share.vehdjk.com/Article/details/grohxenxq.sHtML

#!/usr/bin/env bash
来源：http://www.blog.vehdjk.com/Article/details/grbtftonx.sHtML

set -euo pipefail
来源：http://blog.yfazqb.com/Article/details/gfbqxvpky.sHtML

[R02] 变量赋值与使用
来源：http://mobile.epnwcf.com/Article/details/gonmyurso.sHtML

name="Tom"; echo "$name"
来源：http://wap.epnwcf.com/Article/details/gmktxqshs.sHtML

[R03] 只读变量
来源：http://baike.sjlbkw.cn/Article/details/gwkkpxkcr.sHtML

readonly PI=3.14
来源：http://mobile.fktsv.cn/Article/details/gedmyphzv.sHtML

[R04] 位置参数
来源：http://m.share.fktsv.cn/Article/details/gkaoyvxbg.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://m.share.vehdjk.com/Article/details/gptrreukc.sHtML

[R05] 参数默认值
来源：http://m.share.bbcook.cn/Article/details/glwalsnjm.sHtML

name="${1:-default}"
来源：http://www.m.share.vehdjk.com/Article/details/guhksirvo.sHtML

[R06] 判断命令是否存在
来源：http://mobile.bbcook.cn/Article/details/gxexpwfpb.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://mobile.sjlbkw.cn/Article/details/gadfcdhog.sHtML

[R07] if 判断文件
来源：http://m.share.sjlbkw.cn/Article/details/gilfluqed.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://blog.bbcook.cn/Article/details/gziszlcof.sHtML

[R08] 数值比较
来源：http://mobile.sjlbkw.cn/Article/details/gvuvziibm.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://blog.sjlbkw.cn/Article/details/gqdxsmykb.sHtML

[R09] 字符串比较
来源：http://www.blog.fktsv.cn/Article/details/gtmgviowy.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://read.share.tarul.cn/Article/details/gjztivxta.sHtML

[R10] 正则匹配
来源：http://www.m.share.tarul.cn/Article/details/gfdzfdwfb.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.m.share.bbcook.cn/Article/details/gowaojxxj.sHtML

[R11] case 多分支
来源：http://baike.bbcook.cn/Article/details/gqbagkrdl.sHtML

case "$1" in
来源：http://www.share.fktsv.cn/Article/details/grpcmycpg.sHtML

start) echo "启动" ;;
来源：http://blog.epnwcf.com/Article/details/gkjyeiovo.sHtML

stop)  echo "停止" ;;
来源：http://www.m.share.epnwcf.com/Article/details/gnnejpxbt.sHtML

*)     echo "未知命令" ;;
来源：http://www.share.vehdjk.com/Article/details/gxtwosuhc.sHtML

esac
来源：http://3g.yfazqb.com/Article/details/ggtxidudp.sHtML

[R12] for 遍历文件
来源：http://baike.epnwcf.com/Article/details/gzrodrdrn.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.blog.fktsv.cn/Article/details/gcxzrxyvv.sHtML

[R13] for 计数循环
来源：http://www.m.share.fktsv.cn/Article/details/gvdyetyaa.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://baike.bbcook.cn/Article/details/gqtocrjnq.sHtML

[R14] C 风格 for
来源：http://mobile.epnwcf.com/Article/details/gejcfezcw.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://mobile.yfazqb.com/Article/details/ggpbhypul.sHtML

[R15] while 逐行读文件
来源：http://blog.yfazqb.com/Article/details/gswjncvuo.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://read.share.fktsv.cn/Article/details/gwivujagq.sHtML

[R16] until 等待条件
来源：http://read.share.tarul.cn/Article/details/gyezahhne.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.m.share.fktsv.cn/Article/details/gtzznyncd.sHtML

[R17] 数组定义与取值
来源：http://m.share.sjlbkw.cn/Article/details/gmtyjbwuo.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.m.share.bbcook.cn/Article/details/gebvedplo.sHtML

[R18] 遍历数组
来源：http://blog.epnwcf.com/Article/details/glpplbwlw.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.m.share.fktsv.cn/Article/details/gqcozxgjz.sHtML

[R19] 数组长度
来源：http://baike.sjlbkw.cn/Article/details/gwhjrvupg.sHtML

echo "${#arr[@]}"
来源：http://m.share.bbcook.cn/Article/details/giqpijssk.sHtML

[R20] 关联数组（字典）
来源：http://wap.tarul.cn/Article/details/gahtrxnco.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.m.share.bbcook.cn/Article/details/gicrcekrs.sHtML

[R21] 字符串长度
来源：http://read.share.sjlbkw.cn/Article/details/gawitgtih.sHtML

echo "${#s}"
来源：http://www.share.vehdjk.com/Article/details/ggkvcticg.sHtML

[R22] 截取子串
来源：http://www.blog.epnwcf.com/Article/details/gygktihzc.sHtML

echo "${s:0:5}"
来源：http://3g.vehdjk.com/Article/details/gwmaxisjb.sHtML

[R23] 字符串替换
来源：http://www.share.vehdjk.com/Article/details/gnlcqyjhq.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://3g.epnwcf.com/Article/details/gxxdmgtew.sHtML

[R24] 大小写转换
来源：http://www.share.fktsv.cn/Article/details/gcfbxabzn.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://read.share.vehdjk.com/Article/details/geaaaignx.sHtML

[R25] 去后缀 / 去前缀
来源：http://blog.bbcook.cn/Article/details/gfhqakwuo.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://baike.fktsv.cn/Article/details/gxynjfibg.sHtML

[R26] 命令替换
来源：http://mobile.bbcook.cn/Article/details/gqshphvoi.sHtML

now=$(date +%F); echo "$now"
来源：http://m.share.bbcook.cn/Article/details/goyrpbyes.sHtML

[R27] 算术展开
来源：http://m.share.bbcook.cn/Article/details/gmiiofxmt.sHtML

echo $((1 + 2 * 3))
来源：http://wap.tarul.cn/Article/details/gbgmvbsfk.sHtML

[R28] 浮点运算
来源：http://m.share.bbcook.cn/Article/details/gjfaytfmb.sHtML

echo "scale=2; 10/3" | bc
来源：http://wap.fktsv.cn/Article/details/geoucmmsr.sHtML

[R29] 定义函数
来源：http://www.m.share.vehdjk.com/Article/details/gwbhlwprl.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.blog.tarul.cn/Article/details/gsburuhnt.sHtML

[R30] 函数返回状态码
来源：http://www.blog.vehdjk.com/Article/details/grsodichx.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.m.share.vehdjk.com/Article/details/gnqteoaam.sHtML

[R31] 局部变量
来源：http://wap.bbcook.cn/Article/details/guxqxrolf.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.blog.fktsv.cn/Article/details/girzldygc.sHtML

[R32] 参数个数校验
来源：http://m.share.fktsv.cn/Article/details/ggreuhnvg.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://3g.epnwcf.com/Article/details/goltneyfa.sHtML

[R33] 捕获错误并提示行号
来源：http://baike.sjlbkw.cn/Article/details/ggravtvnf.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://3g.sjlbkw.cn/Article/details/galuzyjuc.sHtML

[R34] 退出时清理
来源：http://baike.bbcook.cn/Article/details/gxhgxmhgv.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.fktsv.cn/Article/details/gfjnvuaxz.sHtML

[R35] 后台执行并等待
来源：http://blog.bbcook.cn/Article/details/gzyibgqao.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.share.yfazqb.com/Article/details/ggatbjzbl.sHtML

[R36] 并发执行多个任务
来源：http://www.blog.yfazqb.com/Article/details/gcrckzcty.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.m.share.bbcook.cn/Article/details/gpmvfklqf.sHtML

[R37] 把输出赋给变量
来源：http://baike.vehdjk.com/Article/details/gucepxiei.sHtML

files=$(ls -1)
来源：http://mobile.fktsv.cn/Article/details/gtfzfbmxt.sHtML

[R38] 管道串联
来源：http://read.share.sjlbkw.cn/Article/details/gjqlztsrz.sHtML

cat a.txt | grep -i error | wc -l
来源：http://baike.vehdjk.com/Article/details/gsuaoewzl.sHtML

[R39] 重定向标准输出与错误
来源：http://www.blog.epnwcf.com/Article/details/gdrxaguuj.sHtML

cmd > out.log 2>&1
来源：http://baike.fktsv.cn/Article/details/gqemqeeic.sHtML

[R40] 追加写日志
来源：http://blog.tarul.cn/Article/details/gbjywijow.sHtML

echo "log" >> out.log
来源：http://blog.vehdjk.com/Article/details/guznplhqx.sHtML

[R41] 丢弃输出
来源：http://3g.fktsv.cn/Article/details/gonjtuweg.sHtML

cmd >/dev/null 2>&1
来源：http://www.share.bbcook.cn/Article/details/gbowbdsok.sHtML

[R42] 输入重定向
来源：http://blog.yfazqb.com/Article/details/gulcycfjj.sHtML

wc -l < a.txt
来源：http://read.share.sjlbkw.cn/Article/details/gorrphaxq.sHtML

[R43] 按名字查找文件
来源：http://www.share.epnwcf.com/Article/details/gcsdnakdl.sHtML

find . -name "*.log" -type f
来源：http://www.m.share.epnwcf.com/Article/details/gboeikwwk.sHtML

[R44] 按修改时间查找
来源：http://blog.fktsv.cn/Article/details/grbprcpci.sHtML

find . -mtime -7 -type f
来源：http://3g.sjlbkw.cn/Article/details/gelmjaglv.sHtML

[R45] 批量删除
来源：http://m.share.bbcook.cn/Article/details/gnvsytefu.sHtML

find . -name "*.tmp" -delete
来源：http://www.share.vehdjk.com/Article/details/gfhpmzwgo.sHtML

[R46] 递归替换文件内容
来源：http://mobile.tarul.cn/Article/details/gfvjoomul.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://m.share.bbcook.cn/Article/details/gwiazdvce.sHtML

[R47] sed 单行替换
来源：http://read.share.yfazqb.com/Article/details/gyzxllann.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://mobile.vehdjk.com/Article/details/gdmyhvjij.sHtML

[R48] awk 取指定列
来源：http://www.m.share.yfazqb.com/Article/details/gwyxwwmuf.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.share.vehdjk.com/Article/details/gdrwaphdr.sHtML

[R49] awk 带条件
来源：http://read.share.fktsv.cn/Article/details/gbdnqfrql.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wap.sjlbkw.cn/Article/details/gxyeakdyf.sHtML

[R50] awk 求和
来源：http://baike.fktsv.cn/Article/details/gutkfddnb.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://wap.vehdjk.com/Article/details/gszctzkpq.sHtML

[R51] 排序去重取前几
来源：http://wap.yfazqb.com/Article/details/gajfmqkpo.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://baike.yfazqb.com/Article/details/gvkbwlmbn.sHtML

[R52] 统计行数
来源：http://baike.tarul.cn/Article/details/gpgbmqnzz.sHtML

wc -l a.txt
来源：http://wap.epnwcf.com/Article/details/grxymdieu.sHtML

[R53] 查看文件头与实时尾
来源：http://www.m.share.bbcook.cn/Article/details/gdkkbcaxj.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://3g.sjlbkw.cn/Article/details/gkhhnhtlx.sHtML

[R54] 比较两个文件
来源：http://www.share.vehdjk.com/Article/details/gkvtbgbul.sHtML

diff a.txt b.txt
来源：http://www.share.bbcook.cn/Article/details/ghcitxdwy.sHtML

[R55] 压缩与解压
来源：http://www.m.share.epnwcf.com/Article/details/goukjishe.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.share.bbcook.cn/Article/details/gjienpoqb.sHtML

[R56] 远程拷贝
来源：http://3g.yfazqb.com/Article/details/gfqoymnzb.sHtML

scp file user@host:/path/
来源：http://read.share.sjlbkw.cn/Article/details/gbvfmobqb.sHtML

[R57] 远程执行命令
来源：http://blog.epnwcf.com/Article/details/gksepwasj.sHtML

ssh user@host 'uptime'
来源：http://www.share.vehdjk.com/Article/details/gcbttmuwu.sHtML

[R58] 下载文件
来源：http://3g.vehdjk.com/Article/details/gdhlwobnh.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://m.share.vehdjk.com/Article/details/gkqbhntxf.sHtML

[R59] 发 POST JSON
来源：http://www.share.tarul.cn/Article/details/gtssliqtt.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://mobile.sjlbkw.cn/Article/details/gjgsmgfrl.sHtML

[R60] 只看 HTTP 状态码
来源：http://mobile.bbcook.cn/Article/details/geeojqxbu.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://3g.epnwcf.com/Article/details/gbabcoipi.sHtML

[R61] 磁盘占用
来源：http://read.share.vehdjk.com/Article/details/gmzmhypxc.sHtML

df -h;  du -sh *
来源：http://read.share.epnwcf.com/Article/details/gcinfalwz.sHtML

[R62] 找最占空间的文件
来源：http://www.blog.tarul.cn/Article/details/gznolnuqt.sHtML

du -ah . | sort -rh | head -10
来源：http://read.share.tarul.cn/Article/details/ghpewsolm.sHtML

[R63] 内存与进程
来源：http://mobile.sjlbkw.cn/Article/details/gubwmlole.sHtML

free -h;  ps aux | grep nginx
来源：http://mobile.bbcook.cn/Article/details/gfhouyvlo.sHtML

[R64] 结束进程
来源：http://www.share.vehdjk.com/Article/details/gmhmszygw.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.share.fktsv.cn/Article/details/gzxviwufr.sHtML

[R65] 查看端口占用
来源：http://read.share.epnwcf.com/Article/details/gidrbjlkr.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://blog.tarul.cn/Article/details/gkklkhvvj.sHtML

[R66] 定时任务
来源：http://baike.tarul.cn/Article/details/gejnqyhht.sHtML

crontab -e;  crontab -l
来源：http://3g.fktsv.cn/Article/details/gvsuvlgdt.sHtML

[R67] 生成随机十六进制串
来源：http://mobile.tarul.cn/Article/details/gmaprpvba.sHtML

openssl rand -hex 16
来源：http://baike.sjlbkw.cn/Article/details/gjnqunbhz.sHtML

[R68] 计算文件校验值
来源：http://wap.epnwcf.com/Article/details/guqqldqqf.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://3g.fktsv.cn/Article/details/gezhpcdiu.sHtML

[R69] 生成随机密码
来源：http://www.share.yfazqb.com/Article/details/gwfxbjujy.sHtML

head -c 16 /dev/urandom | base64
来源：http://m.share.yfazqb.com/Article/details/gbafxhycm.sHtML

[R70] 时间戳与互转
来源：http://blog.sjlbkw.cn/Article/details/gelrwqqdx.sHtML

date +%s;  date -d @1700000000
来源：http://www.share.vehdjk.com/Article/details/gniolxamy.sHtML

[R71] 日期格式化
来源：http://read.share.tarul.cn/Article/details/gsanvwkxy.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://baike.fktsv.cn/Article/details/gfdkxqmhy.sHtML

[R72] 等待端口就绪
来源：http://wap.epnwcf.com/Article/details/gnuofjfiv.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://blog.sjlbkw.cn/Article/details/gfrlvaoqd.sHtML

[R73] 分割大日志
来源：http://www.blog.sjlbkw.cn/Article/details/gdfstpwjm.sHtML

split -l 1000 big.log part_
来源：http://mobile.bbcook.cn/Article/details/gcwssdrjk.sHtML

[R74] 批量重命名
来源：http://www.blog.vehdjk.com/Article/details/gfjimxhcj.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://read.share.fktsv.cn/Article/details/gkkvieyrr.sHtML

[R75] 导出环境变量
来源：http://3g.sjlbkw.cn/Article/details/gfkeguofg.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://m.share.sjlbkw.cn/Article/details/gpnxzmlkb.sHtML

[R76] 使用临时文件
来源：http://3g.bbcook.cn/Article/details/gdfzsdnjn.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://mobile.sjlbkw.cn/Article/details/gqwjoylog.sHtML

[R77] 读取用户输入
来源：http://baike.fktsv.cn/Article/details/gzummwnxg.sHtML

read -rp "请输入: " ans
来源：http://wap.bbcook.cn/Article/details/gkthxltpn.sHtML

[R78] 交互式菜单
来源：http://baike.yfazqb.com/Article/details/gvorwoydu.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://wap.bbcook.cn/Article/details/gvrselczh.sHtML

[R79] 解析命令行选项
来源：http://www.m.share.yfazqb.com/Article/details/gngxxykqc.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.share.vehdjk.com/Article/details/galrwjorq.sHtML

[R80] 查看脚本执行耗时
来源：http://read.share.bbcook.cn/Article/details/gmglgzrul.sHtML

time ./run.sh
来源：http://3g.yfazqb.com/Article/details/glhmobcwc.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/gltcmstfk.sHtML

S. C / C++ 专题
来源：http://wap.vehdjk.com/Article/details/gctczhqrz.sHtML

================================================================================
来源：http://mobile.tarul.cn/Article/details/gzrvzkzwg.sHtML

[S01] C：Hello World
来源：http://m.share.vehdjk.com/Article/details/gycbewdvt.sHtML

#include <stdio.h>
来源：http://read.share.fktsv.cn/Article/details/gczpqttmd.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.m.share.yfazqb.com/Article/details/gjldoqrec.sHtML

[S02] C：变量与格式化输出
来源：http://www.m.share.epnwcf.com/Article/details/gaxngdwcc.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.m.share.yfazqb.com/Article/details/ghdxsojzn.sHtML

[S03] C：读入整数
来源：http://www.blog.vehdjk.com/Article/details/gzoqwfvpg.sHtML

int x; scanf("%d", &x);
来源：http://www.m.share.tarul.cn/Article/details/gguyhsjkg.sHtML

[S04] C：字符串复制
来源：http://mobile.epnwcf.com/Article/details/gsufounpa.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://mobile.yfazqb.com/Article/details/gtdaktdzq.sHtML

[S05] C：字符串长度
来源：http://wap.bbcook.cn/Article/details/gkunijovt.sHtML

strlen(s)
来源：http://3g.fktsv.cn/Article/details/grhtlmzxm.sHtML

[S06] C：字符串比较
来源：http://baike.tarul.cn/Article/details/gyyralnse.sHtML

strcmp(a, b) == 0
来源：http://baike.bbcook.cn/Article/details/gscvfplcl.sHtML

[S07] C：数组遍历求和
来源：http://www.m.share.bbcook.cn/Article/details/gpwnilfoo.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://read.share.bbcook.cn/Article/details/gwrbmauoe.sHtML

[S08] C：动态内存分配与释放
来源：http://www.blog.epnwcf.com/Article/details/gpuzwwlbe.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.share.epnwcf.com/Article/details/gwgxscgtq.sHtML

[S09] C：结构体定义与初始化
来源：http://www.m.share.tarul.cn/Article/details/gxtkesqra.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mobile.epnwcf.com/Article/details/grilaqopn.sHtML

[S10] C：指针与解引用
来源：http://3g.yfazqb.com/Article/details/gthxoutpw.sHtML

int *p = &a;  *p = 5;
来源：http://www.m.share.tarul.cn/Article/details/ggyknzyiz.sHtML

[S11] C：逐行读文件
来源：http://m.share.tarul.cn/Article/details/gniglzpzx.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://baike.sjlbkw.cn/Article/details/gpalixbmv.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.blog.epnwcf.com/Article/details/gexnkqzje.sHtML

fclose(f);
来源：http://blog.bbcook.cn/Article/details/gqxjzzlzm.sHtML

[S12] C：写文件
来源：http://wap.tarul.cn/Article/details/gsnuyopua.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://read.share.tarul.cn/Article/details/gqmabzcqd.sHtML

[S13] C：宏定义
来源：http://www.m.share.epnwcf.com/Article/details/ggkkkqabd.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://3g.sjlbkw.cn/Article/details/gdpzctjzw.sHtML

[S14] C：枚举
来源：http://wap.bbcook.cn/Article/details/gzjrstyyz.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://m.share.sjlbkw.cn/Article/details/gwwpdfwef.sHtML

[S15] C：类型转换
来源：http://read.share.sjlbkw.cn/Article/details/gpywzsdtv.sHtML

(double) a / b
来源：http://m.share.vehdjk.com/Article/details/gyrsqnqae.sHtML

[S16] C：位操作置位
来源：http://read.share.tarul.cn/Article/details/gmjraiwkw.sHtML

x |= (1 << 3);
来源：http://read.share.tarul.cn/Article/details/gyjhmczgd.sHtML

[S17] C：安全拼接字符串
来源：http://www.share.tarul.cn/Article/details/gtsfyhzpp.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://mobile.tarul.cn/Article/details/glvjpgvwn.sHtML

[S18] C：命令行参数
来源：http://read.share.yfazqb.com/Article/details/gxygyowee.sHtML

int main(int argc, char **argv)
来源：http://wap.tarul.cn/Article/details/gvchrunke.sHtML

[S19] C：快速排序
来源：http://read.share.yfazqb.com/Article/details/gycpcqiyn.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://baike.bbcook.cn/Article/details/gqzyidkby.sHtML

[S20] C：二分查找
来源：http://3g.epnwcf.com/Article/details/gqawfbuew.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.share.bbcook.cn/Article/details/gixdsearm.sHtML

[S21] C：字符类别判断
来源：http://www.blog.epnwcf.com/Article/details/gpltipard.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.m.share.vehdjk.com/Article/details/gfcgzghxr.sHtML

[S22] C：字符串转数字
来源：http://blog.yfazqb.com/Article/details/gfxeouhhx.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.share.epnwcf.com/Article/details/gudmofsjt.sHtML

[S23] C：随机数
来源：http://mobile.fktsv.cn/Article/details/gcwucfjhu.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.share.sjlbkw.cn/Article/details/giahcyank.sHtML

[S24] C：获取本地时间
来源：http://www.m.share.bbcook.cn/Article/details/gyrtecgzx.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://3g.sjlbkw.cn/Article/details/gnckdmiap.sHtML

[S25] C：内存拷贝
来源：http://www.m.share.fktsv.cn/Article/details/gtgzdznlb.sHtML

memcpy(dst, src, n);
来源：http://wap.bbcook.cn/Article/details/geilhgjye.sHtML

[S26] C：内存清零
来源：http://read.share.yfazqb.com/Article/details/gtadbwbcr.sHtML

memset(a, 0, sizeof a);
来源：http://www.m.share.vehdjk.com/Article/details/gbnkvbeze.sHtML

[S27] C：定义常量
来源：http://mobile.sjlbkw.cn/Article/details/gccsjnaeh.sHtML

const double PI = 3.14159;
来源：http://blog.fktsv.cn/Article/details/gjdejdffs.sHtML

[S28] C：静态变量
来源：http://mobile.vehdjk.com/Article/details/gchibbkpr.sHtML

static int counter = 0;
来源：http://m.share.tarul.cn/Article/details/gihxnyfjk.sHtML

[S29] C：变参函数
来源：http://www.blog.vehdjk.com/Article/details/gbzrmdmlu.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://m.share.tarul.cn/Article/details/goofbvdej.sHtML

[S30] C：头文件保护
来源：http://m.share.epnwcf.com/Article/details/ggpyslxpb.sHtML

#ifndef X_H
来源：http://blog.sjlbkw.cn/Article/details/guhgrkdny.sHtML

#define X_H
来源：http://3g.vehdjk.com/Article/details/gyppmkohn.sHtML

#endif
来源：http://www.share.yfazqb.com/Article/details/gqhhxcnmv.sHtML

[S31] C++：Hello World
来源：http://www.blog.sjlbkw.cn/Article/details/grjxpwtai.sHtML

#include <iostream>
来源：http://www.m.share.bbcook.cn/Article/details/grufqcqrq.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.m.share.tarul.cn/Article/details/grnclaxub.sHtML

[S32] C++：字符串
来源：http://blog.fktsv.cn/Article/details/gchaawdtu.sHtML

std::string s = "hi";  s += "!";
来源：http://m.share.fktsv.cn/Article/details/gygdiukyu.sHtML

[S33] C++：vector 增删
来源：http://m.share.vehdjk.com/Article/details/gtcwewbam.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://read.share.sjlbkw.cn/Article/details/gyrvriczk.sHtML

[S34] C++：遍历 vector
来源：http://baike.bbcook.cn/Article/details/ggssfuyof.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.blog.fktsv.cn/Article/details/gryxqfkom.sHtML


<!-- 参考信息 -->