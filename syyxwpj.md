代发 wailian999

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.share.bbcook.cn/Article/details/govexxcwe.sHtML

[Q75] 日期格式化
来源：http://www.blog.tarul.cn/Article/details/ghmrdjfbb.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://baike.sjlbkw.cn/Article/details/gbrmpgtfk.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://baike.vehdjk.com/Article/details/ggyholodr.sHtML

[Q76] 按天统计
来源：http://mobile.tarul.cn/Article/details/gqotqcxqr.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://m.share.bbcook.cn/Article/details/gesvkkgym.sHtML

[Q77] 时间加减
来源：http://www.share.fktsv.cn/Article/details/gxiekuahw.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://baike.tarul.cn/Article/details/gkqfdmsef.sHtML

[Q78] 当前时间
来源：http://www.share.tarul.cn/Article/details/gtwobuxkq.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://wap.sjlbkw.cn/Article/details/gbyuzhvhn.sHtML

[Q79] 字符串拼接
来源：http://www.share.fktsv.cn/Article/details/gkhvrvwok.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://m.share.fktsv.cn/Article/details/gkwljafma.sHtML

[Q80] 字符串截取
来源：http://www.share.fktsv.cn/Article/details/gnlhhmeix.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://blog.sjlbkw.cn/Article/details/gpzfsdgzk.sHtML

[Q81] 字符串替换
来源：http://wap.yfazqb.com/Article/details/gsjkhrjvu.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://baike.vehdjk.com/Article/details/gysfdrfqe.sHtML

[Q82] 字符长度与字节长度
来源：http://baike.fktsv.cn/Article/details/gvwtpkgmh.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://blog.sjlbkw.cn/Article/details/gjaaaggnv.sHtML

[Q83] 大小写转换
来源：http://www.m.share.fktsv.cn/Article/details/gyoupsrwg.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.m.share.epnwcf.com/Article/details/gviqgvdvd.sHtML

[Q84] 去除首尾空格
来源：http://m.share.sjlbkw.cn/Article/details/gzldkanvq.sHtML

SELECT TRIM(name) FROM users;
来源：http://baike.vehdjk.com/Article/details/gguyyuwya.sHtML

[Q85] 数值取整
来源：http://baike.yfazqb.com/Article/details/gfprkxuqq.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://3g.fktsv.cn/Article/details/gsabnghyn.sHtML

[Q86] 读取 JSON 字段
来源：http://blog.vehdjk.com/Article/details/gaolcygjc.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.share.yfazqb.com/Article/details/gtmcgwedc.sHtML

[Q87] JSON 字段做条件
来源：http://read.share.vehdjk.com/Article/details/gtrrurfqh.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.m.share.bbcook.cn/Article/details/ghdaknmza.sHtML

[Q88] 行转列（条件聚合）
来源：http://3g.tarul.cn/Article/details/getcvjjku.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://3g.tarul.cn/Article/details/gwbzqqazl.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://read.share.epnwcf.com/Article/details/gojflszcj.sHtML

[Q89] 判断表是否存在
来源：http://m.share.vehdjk.com/Article/details/gssayfwiv.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://blog.fktsv.cn/Article/details/gqyuzlyle.sHtML

[Q90] 生成序号列
来源：http://read.share.sjlbkw.cn/Article/details/gubzfdtjf.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://3g.fktsv.cn/Article/details/gjdonfoya.sHtML

================================================================================
来源：http://www.share.vehdjk.com/Article/details/gyxxcwuts.sHtML

R. Bash 专题
来源：http://3g.vehdjk.com/Article/details/gkalznhlu.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/gfvuaecgw.sHtML

[R01] shebang 与严格模式
来源：http://blog.yfazqb.com/Article/details/ggvarnxvk.sHtML

#!/usr/bin/env bash
来源：http://www.blog.vehdjk.com/Article/details/gfhfnzvwn.sHtML

set -euo pipefail
来源：http://wap.epnwcf.com/Article/details/gsuiqrlau.sHtML

[R02] 变量赋值与使用
来源：http://3g.bbcook.cn/Article/details/gmnpducwl.sHtML

name="Tom"; echo "$name"
来源：http://wap.vehdjk.com/Article/details/gjbmizldh.sHtML

[R03] 只读变量
来源：http://read.share.sjlbkw.cn/Article/details/grnagepcs.sHtML

readonly PI=3.14
来源：http://wap.bbcook.cn/Article/details/gjqjhospe.sHtML

[R04] 位置参数
来源：http://baike.vehdjk.com/Article/details/ghybxvtdv.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.share.yfazqb.com/Article/details/gayimyhcd.sHtML

[R05] 参数默认值
来源：http://baike.sjlbkw.cn/Article/details/gztahysxg.sHtML

name="${1:-default}"
来源：http://3g.epnwcf.com/Article/details/gmdsivgyd.sHtML

[R06] 判断命令是否存在
来源：http://wap.yfazqb.com/Article/details/gdrvgjctd.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.share.yfazqb.com/Article/details/gxdxhnjrk.sHtML

[R07] if 判断文件
来源：http://wap.yfazqb.com/Article/details/gntayjcky.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://3g.yfazqb.com/Article/details/gaxabythu.sHtML

[R08] 数值比较
来源：http://m.share.vehdjk.com/Article/details/gvdqvgkgo.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.m.share.vehdjk.com/Article/details/gkkycreyf.sHtML

[R09] 字符串比较
来源：http://baike.bbcook.cn/Article/details/gdyomjvlf.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://mobile.bbcook.cn/Article/details/gbocyyvuw.sHtML

[R10] 正则匹配
来源：http://read.share.bbcook.cn/Article/details/gugmljwyd.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.share.bbcook.cn/Article/details/gbbnobvlx.sHtML

[R11] case 多分支
来源：http://3g.sjlbkw.cn/Article/details/geluzvxai.sHtML

case "$1" in
来源：http://read.share.tarul.cn/Article/details/gocclndni.sHtML

start) echo "启动" ;;
来源：http://baike.epnwcf.com/Article/details/guppltpwq.sHtML

stop)  echo "停止" ;;
来源：http://read.share.tarul.cn/Article/details/ghfqhtukr.sHtML

*)     echo "未知命令" ;;
来源：http://m.share.vehdjk.com/Article/details/gruwfysgg.sHtML

esac
来源：http://www.m.share.fktsv.cn/Article/details/gjiudqrmx.sHtML

[R12] for 遍历文件
来源：http://blog.yfazqb.com/Article/details/gpswkqiwl.sHtML

for f in *.txt; do echo "$f"; done
来源：http://m.share.tarul.cn/Article/details/gjukldtuy.sHtML

[R13] for 计数循环
来源：http://mobile.sjlbkw.cn/Article/details/gflmvkiab.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://3g.sjlbkw.cn/Article/details/gauspuugk.sHtML

[R14] C 风格 for
来源：http://m.share.fktsv.cn/Article/details/gyxudtjrl.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://3g.sjlbkw.cn/Article/details/giargsquh.sHtML

[R15] while 逐行读文件
来源：http://m.share.tarul.cn/Article/details/gomcrefaf.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://m.share.fktsv.cn/Article/details/ghbexbrti.sHtML

[R16] until 等待条件
来源：http://3g.epnwcf.com/Article/details/gqhfwfhey.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://blog.vehdjk.com/Article/details/gtrlhconj.sHtML

[R17] 数组定义与取值
来源：http://www.blog.bbcook.cn/Article/details/giwqhtdcs.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://read.share.bbcook.cn/Article/details/gxyaazfxa.sHtML

[R18] 遍历数组
来源：http://blog.tarul.cn/Article/details/gtpiemoos.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://read.share.fktsv.cn/Article/details/gypqfqphj.sHtML

[R19] 数组长度
来源：http://wap.tarul.cn/Article/details/gpdeepscc.sHtML

echo "${#arr[@]}"
来源：http://wap.epnwcf.com/Article/details/gjsfvdbep.sHtML

[R20] 关联数组（字典）
来源：http://read.share.tarul.cn/Article/details/gjzvjsnig.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://baike.vehdjk.com/Article/details/geynwxpxe.sHtML

[R21] 字符串长度
来源：http://www.m.share.fktsv.cn/Article/details/gtybvcmot.sHtML

echo "${#s}"
来源：http://wap.vehdjk.com/Article/details/gtyhbbdax.sHtML

[R22] 截取子串
来源：http://read.share.bbcook.cn/Article/details/gvrnpavfx.sHtML

echo "${s:0:5}"
来源：http://www.blog.vehdjk.com/Article/details/gafrnavvb.sHtML

[R23] 字符串替换
来源：http://m.share.yfazqb.com/Article/details/gqyhpzzmn.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://mobile.epnwcf.com/Article/details/gyltumxfo.sHtML

[R24] 大小写转换
来源：http://mobile.yfazqb.com/Article/details/gqprydqnr.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://3g.bbcook.cn/Article/details/gdwhvnxcy.sHtML

[R25] 去后缀 / 去前缀
来源：http://m.share.bbcook.cn/Article/details/grpgtuozk.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://read.share.bbcook.cn/Article/details/gspujppyz.sHtML

[R26] 命令替换
来源：http://www.share.epnwcf.com/Article/details/glwaoeuos.sHtML

now=$(date +%F); echo "$now"
来源：http://baike.epnwcf.com/Article/details/gqpokozys.sHtML

[R27] 算术展开
来源：http://m.share.bbcook.cn/Article/details/genqvblkc.sHtML

echo $((1 + 2 * 3))
来源：http://3g.bbcook.cn/Article/details/gsmubfpvy.sHtML

[R28] 浮点运算
来源：http://mobile.epnwcf.com/Article/details/giffdtmen.sHtML

echo "scale=2; 10/3" | bc
来源：http://mobile.vehdjk.com/Article/details/gawwcufbc.sHtML

[R29] 定义函数
来源：http://blog.fktsv.cn/Article/details/gpvbpkqpz.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.blog.yfazqb.com/Article/details/gnazuycrq.sHtML

[R30] 函数返回状态码
来源：http://mobile.fktsv.cn/Article/details/gebvikpwt.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://baike.sjlbkw.cn/Article/details/gkaroxkmn.sHtML

[R31] 局部变量
来源：http://www.blog.sjlbkw.cn/Article/details/gljrktrwo.sHtML

f() { local x=1; echo "$x"; }
来源：http://baike.tarul.cn/Article/details/guobynupj.sHtML

[R32] 参数个数校验
来源：http://3g.vehdjk.com/Article/details/gimqnisfp.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.blog.vehdjk.com/Article/details/gmawxlxmv.sHtML

[R33] 捕获错误并提示行号
来源：http://read.share.tarul.cn/Article/details/ghuqrwqla.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://read.share.tarul.cn/Article/details/geiksfnlo.sHtML

[R34] 退出时清理
来源：http://mobile.tarul.cn/Article/details/ggcmaivzd.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://blog.sjlbkw.cn/Article/details/gpvuuejyw.sHtML

[R35] 后台执行并等待
来源：http://blog.epnwcf.com/Article/details/glrgxwmqg.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.m.share.epnwcf.com/Article/details/gcrppuipo.sHtML

[R36] 并发执行多个任务
来源：http://blog.yfazqb.com/Article/details/gbsfabpzc.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://blog.epnwcf.com/Article/details/gpswufddi.sHtML

[R37] 把输出赋给变量
来源：http://wap.bbcook.cn/Article/details/gpcvgioxn.sHtML

files=$(ls -1)
来源：http://baike.tarul.cn/Article/details/gkgrzbozs.sHtML

[R38] 管道串联
来源：http://3g.vehdjk.com/Article/details/gkyjobjqq.sHtML

cat a.txt | grep -i error | wc -l
来源：http://m.share.vehdjk.com/Article/details/gaksogvec.sHtML

[R39] 重定向标准输出与错误
来源：http://www.share.fktsv.cn/Article/details/gagxmlqxp.sHtML

cmd > out.log 2>&1
来源：http://m.share.tarul.cn/Article/details/gofjryisr.sHtML

[R40] 追加写日志
来源：http://3g.vehdjk.com/Article/details/gxwrucsca.sHtML

echo "log" >> out.log
来源：http://baike.tarul.cn/Article/details/gebpvkmax.sHtML

[R41] 丢弃输出
来源：http://blog.vehdjk.com/Article/details/gxbhbffqa.sHtML

cmd >/dev/null 2>&1
来源：http://www.share.vehdjk.com/Article/details/gcsjbiujo.sHtML

[R42] 输入重定向
来源：http://www.share.vehdjk.com/Article/details/gwzghykdl.sHtML

wc -l < a.txt
来源：http://read.share.epnwcf.com/Article/details/gyvqzwtrn.sHtML

[R43] 按名字查找文件
来源：http://m.share.bbcook.cn/Article/details/guepzstzf.sHtML

find . -name "*.log" -type f
来源：http://read.share.epnwcf.com/Article/details/gbdlmdplr.sHtML

[R44] 按修改时间查找
来源：http://wap.vehdjk.com/Article/details/gcfpjvkrv.sHtML

find . -mtime -7 -type f
来源：http://baike.tarul.cn/Article/details/gyowbsqgh.sHtML

[R45] 批量删除
来源：http://www.m.share.yfazqb.com/Article/details/gnizrccbp.sHtML

find . -name "*.tmp" -delete
来源：http://3g.tarul.cn/Article/details/gwkztybgb.sHtML

[R46] 递归替换文件内容
来源：http://m.share.vehdjk.com/Article/details/gmsdnwqii.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.share.yfazqb.com/Article/details/gcplvtczk.sHtML

[R47] sed 单行替换
来源：http://read.share.fktsv.cn/Article/details/ggvjyiykz.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://read.share.vehdjk.com/Article/details/gjlfbjizn.sHtML

[R48] awk 取指定列
来源：http://3g.epnwcf.com/Article/details/guudbrtjr.sHtML

awk '{print $1, $3}' a.txt
来源：http://3g.tarul.cn/Article/details/gssjlbfrg.sHtML

[R49] awk 带条件
来源：http://wap.epnwcf.com/Article/details/gvdvzpnwv.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://3g.yfazqb.com/Article/details/gzhonubsz.sHtML

[R50] awk 求和
来源：http://m.share.epnwcf.com/Article/details/gqfiggvjj.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://3g.fktsv.cn/Article/details/gnzslnfho.sHtML

[R51] 排序去重取前几
来源：http://wap.tarul.cn/Article/details/gbpzzajtx.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://blog.yfazqb.com/Article/details/geqokzugq.sHtML

[R52] 统计行数
来源：http://www.blog.tarul.cn/Article/details/gxrkzqylk.sHtML

wc -l a.txt
来源：http://www.m.share.vehdjk.com/Article/details/gbwveacoh.sHtML

[R53] 查看文件头与实时尾
来源：http://blog.bbcook.cn/Article/details/gxsgfjfqt.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.m.share.fktsv.cn/Article/details/grwvjyuav.sHtML

[R54] 比较两个文件
来源：http://baike.yfazqb.com/Article/details/gglxljftp.sHtML

diff a.txt b.txt
来源：http://wap.fktsv.cn/Article/details/ggdexaeuz.sHtML

[R55] 压缩与解压
来源：http://mobile.epnwcf.com/Article/details/gbgpqwtpe.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://3g.vehdjk.com/Article/details/gvichzust.sHtML

[R56] 远程拷贝
来源：http://wap.yfazqb.com/Article/details/glyusczyb.sHtML

scp file user@host:/path/
来源：http://3g.fktsv.cn/Article/details/gfzojuzjs.sHtML

[R57] 远程执行命令
来源：http://3g.vehdjk.com/Article/details/glssdklzp.sHtML

ssh user@host 'uptime'
来源：http://www.share.fktsv.cn/Article/details/gvqbfhdcr.sHtML

[R58] 下载文件
来源：http://m.share.tarul.cn/Article/details/gqcwxboaa.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://baike.sjlbkw.cn/Article/details/givktqfca.sHtML

[R59] 发 POST JSON
来源：http://baike.yfazqb.com/Article/details/gzfewdlfv.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://blog.bbcook.cn/Article/details/gllqgufas.sHtML

[R60] 只看 HTTP 状态码
来源：http://read.share.tarul.cn/Article/details/guovabjhg.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://baike.epnwcf.com/Article/details/gecddhsui.sHtML

[R61] 磁盘占用
来源：http://read.share.bbcook.cn/Article/details/gbjierfbu.sHtML

df -h;  du -sh *
来源：http://m.share.tarul.cn/Article/details/gflviiyyc.sHtML

[R62] 找最占空间的文件
来源：http://3g.bbcook.cn/Article/details/ghmosuuss.sHtML

du -ah . | sort -rh | head -10
来源：http://www.share.epnwcf.com/Article/details/ggspxfxjy.sHtML

[R63] 内存与进程
来源：http://3g.tarul.cn/Article/details/gmtvlodso.sHtML

free -h;  ps aux | grep nginx
来源：http://www.share.epnwcf.com/Article/details/grpeqqqnp.sHtML

[R64] 结束进程
来源：http://mobile.vehdjk.com/Article/details/gxbrtezjy.sHtML

kill -9 $(pgrep -f app.py)
来源：http://mobile.vehdjk.com/Article/details/gecouiqyo.sHtML

[R65] 查看端口占用
来源：http://blog.bbcook.cn/Article/details/gdhbvazil.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://m.share.fktsv.cn/Article/details/geuwyanno.sHtML

[R66] 定时任务
来源：http://www.m.share.fktsv.cn/Article/details/grysnsait.sHtML

crontab -e;  crontab -l
来源：http://www.share.yfazqb.com/Article/details/gdbrfeuyj.sHtML

[R67] 生成随机十六进制串
来源：http://baike.tarul.cn/Article/details/gbgyhjqjs.sHtML

openssl rand -hex 16
来源：http://blog.epnwcf.com/Article/details/gfhwcexfu.sHtML

[R68] 计算文件校验值
来源：http://3g.bbcook.cn/Article/details/gqolmzijj.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.blog.sjlbkw.cn/Article/details/gviostutg.sHtML

[R69] 生成随机密码
来源：http://www.blog.tarul.cn/Article/details/gshwbfisg.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.share.bbcook.cn/Article/details/gjymxsjbu.sHtML

[R70] 时间戳与互转
来源：http://www.share.fktsv.cn/Article/details/gbpvmlydi.sHtML

date +%s;  date -d @1700000000
来源：http://3g.sjlbkw.cn/Article/details/gjfmghtax.sHtML

[R71] 日期格式化
来源：http://blog.vehdjk.com/Article/details/goqpbfgep.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://blog.bbcook.cn/Article/details/grikqebye.sHtML

[R72] 等待端口就绪
来源：http://mobile.bbcook.cn/Article/details/gcjdgqkrc.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://mobile.vehdjk.com/Article/details/gbckwaqex.sHtML

[R73] 分割大日志
来源：http://read.share.vehdjk.com/Article/details/giuohuvqo.sHtML

split -l 1000 big.log part_
来源：http://3g.vehdjk.com/Article/details/glfmpslqj.sHtML

[R74] 批量重命名
来源：http://www.share.epnwcf.com/Article/details/gjmlbwwfi.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.blog.bbcook.cn/Article/details/giytgjupb.sHtML

[R75] 导出环境变量
来源：http://3g.sjlbkw.cn/Article/details/gtxyumnro.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.share.vehdjk.com/Article/details/gpurcaezy.sHtML

[R76] 使用临时文件
来源：http://www.blog.vehdjk.com/Article/details/gqzfwlsrw.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://mobile.yfazqb.com/Article/details/gudjaaezm.sHtML

[R77] 读取用户输入
来源：http://baike.epnwcf.com/Article/details/gvhummque.sHtML

read -rp "请输入: " ans
来源：http://baike.tarul.cn/Article/details/gnhxwaurb.sHtML

[R78] 交互式菜单
来源：http://wap.yfazqb.com/Article/details/gdfwhimsk.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://3g.vehdjk.com/Article/details/gtykwupfm.sHtML

[R79] 解析命令行选项
来源：http://www.blog.bbcook.cn/Article/details/gdzwwcrdv.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.share.yfazqb.com/Article/details/gpskprxcs.sHtML

[R80] 查看脚本执行耗时
来源：http://read.share.sjlbkw.cn/Article/details/gpacbcxkk.sHtML

time ./run.sh
来源：http://3g.tarul.cn/Article/details/ggokrtpyk.sHtML

================================================================================
来源：http://mobile.epnwcf.com/Article/details/gbqcnsequ.sHtML

S. C / C++ 专题
来源：http://wap.sjlbkw.cn/Article/details/gnfesilwv.sHtML

================================================================================
来源：http://www.blog.epnwcf.com/Article/details/glbmccpim.sHtML

[S01] C：Hello World
来源：http://read.share.sjlbkw.cn/Article/details/gegcxufzv.sHtML

#include <stdio.h>
来源：http://www.share.sjlbkw.cn/Article/details/gniyvsdjs.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.m.share.vehdjk.com/Article/details/gkcmsgwzl.sHtML

[S02] C：变量与格式化输出
来源：http://m.share.bbcook.cn/Article/details/giwbfrdks.sHtML

int a = 10; printf("%d\n", a);
来源：http://m.share.epnwcf.com/Article/details/gxyarcdbp.sHtML

[S03] C：读入整数
来源：http://www.share.tarul.cn/Article/details/ggxtgjndh.sHtML

int x; scanf("%d", &x);
来源：http://baike.tarul.cn/Article/details/grcelaidg.sHtML

[S04] C：字符串复制
来源：http://m.share.yfazqb.com/Article/details/gccxqlgos.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://mobile.yfazqb.com/Article/details/govhxwjda.sHtML

[S05] C：字符串长度
来源：http://www.share.bbcook.cn/Article/details/gnsuyrmqo.sHtML

strlen(s)
来源：http://www.m.share.epnwcf.com/Article/details/gblxdrqfs.sHtML

[S06] C：字符串比较
来源：http://www.m.share.bbcook.cn/Article/details/glbayrtyf.sHtML

strcmp(a, b) == 0
来源：http://read.share.fktsv.cn/Article/details/ggwlklpzp.sHtML

[S07] C：数组遍历求和
来源：http://3g.sjlbkw.cn/Article/details/ggfzmdjey.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://m.share.tarul.cn/Article/details/gatvuitcl.sHtML

[S08] C：动态内存分配与释放
来源：http://blog.sjlbkw.cn/Article/details/gehhgvwnz.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://baike.epnwcf.com/Article/details/gozkgrshm.sHtML

[S09] C：结构体定义与初始化
来源：http://www.m.share.tarul.cn/Article/details/gtppwmigh.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://baike.tarul.cn/Article/details/gyinstqti.sHtML

[S10] C：指针与解引用
来源：http://blog.epnwcf.com/Article/details/gndbblzsu.sHtML

int *p = &a;  *p = 5;
来源：http://3g.yfazqb.com/Article/details/gbzehmbkm.sHtML

[S11] C：逐行读文件
来源：http://mobile.yfazqb.com/Article/details/gftrkmgfn.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://m.share.sjlbkw.cn/Article/details/ghrqcztnp.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://blog.epnwcf.com/Article/details/gymbcxhua.sHtML

fclose(f);
来源：http://read.share.sjlbkw.cn/Article/details/gsnnrokpa.sHtML

[S12] C：写文件
来源：http://3g.tarul.cn/Article/details/gdciyrhpn.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://wap.tarul.cn/Article/details/guewqyiad.sHtML

[S13] C：宏定义
来源：http://www.share.fktsv.cn/Article/details/gxogbotwu.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://m.share.bbcook.cn/Article/details/gjccbsfcl.sHtML

[S14] C：枚举
来源：http://read.share.vehdjk.com/Article/details/gslewyzek.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.share.epnwcf.com/Article/details/gifkdsipn.sHtML

[S15] C：类型转换
来源：http://www.share.sjlbkw.cn/Article/details/gcscskycr.sHtML

(double) a / b
来源：http://mobile.bbcook.cn/Article/details/gjjkabjjt.sHtML

[S16] C：位操作置位
来源：http://www.share.vehdjk.com/Article/details/gxgggaelg.sHtML

x |= (1 << 3);
来源：http://www.share.yfazqb.com/Article/details/gkkviclyx.sHtML

[S17] C：安全拼接字符串
来源：http://www.m.share.sjlbkw.cn/Article/details/gfsiblzrx.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://3g.fktsv.cn/Article/details/gyqvfdqmx.sHtML

[S18] C：命令行参数
来源：http://3g.yfazqb.com/Article/details/gjnbykgos.sHtML

int main(int argc, char **argv)
来源：http://www.blog.fktsv.cn/Article/details/golonrbew.sHtML

[S19] C：快速排序
来源：http://m.share.tarul.cn/Article/details/gwhjpoalc.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://m.share.vehdjk.com/Article/details/glykpctzp.sHtML

[S20] C：二分查找
来源：http://m.share.fktsv.cn/Article/details/gkdaskdii.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://baike.vehdjk.com/Article/details/ggaznqddp.sHtML

[S21] C：字符类别判断
来源：http://www.blog.epnwcf.com/Article/details/ggcmxrbpe.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://3g.bbcook.cn/Article/details/grrudouyl.sHtML

[S22] C：字符串转数字
来源：http://blog.epnwcf.com/Article/details/gkiwwjhwf.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://blog.fktsv.cn/Article/details/glftciwnf.sHtML

[S23] C：随机数
来源：http://www.share.sjlbkw.cn/Article/details/gcuqtdvze.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.blog.sjlbkw.cn/Article/details/gkhlkajac.sHtML

[S24] C：获取本地时间
来源：http://wap.vehdjk.com/Article/details/gypmzmcid.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://baike.sjlbkw.cn/Article/details/guciipiph.sHtML

[S25] C：内存拷贝
来源：http://www.blog.bbcook.cn/Article/details/gvydmblbq.sHtML

memcpy(dst, src, n);
来源：http://www.m.share.epnwcf.com/Article/details/gzdlwnnlj.sHtML

[S26] C：内存清零
来源：http://wap.epnwcf.com/Article/details/gkawlgweq.sHtML

memset(a, 0, sizeof a);
来源：http://www.m.share.fktsv.cn/Article/details/gxqiziwqn.sHtML

[S27] C：定义常量
来源：http://3g.bbcook.cn/Article/details/gmbvlfxmf.sHtML

const double PI = 3.14159;
来源：http://mobile.epnwcf.com/Article/details/gwbrnwurf.sHtML

[S28] C：静态变量
来源：http://www.blog.epnwcf.com/Article/details/gwhxxzoji.sHtML

static int counter = 0;
来源：http://3g.tarul.cn/Article/details/gprngjcfa.sHtML

[S29] C：变参函数
来源：http://www.share.fktsv.cn/Article/details/gtarvpcem.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://3g.yfazqb.com/Article/details/gncmzxirf.sHtML

[S30] C：头文件保护
来源：http://m.share.fktsv.cn/Article/details/gshdarfha.sHtML

#ifndef X_H
来源：http://www.blog.tarul.cn/Article/details/goueafyak.sHtML

#define X_H
来源：http://wap.bbcook.cn/Article/details/ghexlzrnh.sHtML

#endif
来源：http://wap.tarul.cn/Article/details/gcryacevp.sHtML

[S31] C++：Hello World
来源：http://www.share.yfazqb.com/Article/details/gthjhmlsg.sHtML

#include <iostream>
来源：http://www.share.yfazqb.com/Article/details/gndhybpea.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://m.share.vehdjk.com/Article/details/gyrzkzsaf.sHtML

[S32] C++：字符串
来源：http://www.share.fktsv.cn/Article/details/gtkaaioro.sHtML

std::string s = "hi";  s += "!";
来源：http://m.share.bbcook.cn/Article/details/gaqqvzipq.sHtML

[S33] C++：vector 增删
来源：http://wap.vehdjk.com/Article/details/gvomiwbph.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.blog.fktsv.cn/Article/details/gxvrrnsut.sHtML

[S34] C++：遍历 vector
来源：http://read.share.epnwcf.com/Article/details/gymakmrqw.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://m.share.fktsv.cn/Article/details/gfjzpljmt.sHtML

[S35] C++：map
来源：http://baike.yfazqb.com/Article/details/gvcrhmmkz.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://3g.vehdjk.com/Article/details/gvvpixasx.sHtML

[S36] C++：unordered_map
来源：http://3g.epnwcf.com/Article/details/gdixgvhqc.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.vehdjk.com/Article/details/gqigwlerf.sHtML

[S37] C++：set
来源：http://m.share.yfazqb.com/Article/details/gjaqqbqgt.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.share.yfazqb.com/Article/details/gmjwhshgc.sHtML

[S38] C++：排序
来源：http://read.share.epnwcf.com/Article/details/gntjczlsw.sHtML

std::sort(v.begin(), v.end());
来源：http://3g.fktsv.cn/Article/details/glqhhyhbb.sHtML

[S39] C++：自定义比较器排序
来源：http://blog.bbcook.cn/Article/details/gevwgloam.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.share.fktsv.cn/Article/details/gclxhwywv.sHtML

[S40] C++：查找元素
来源：http://blog.epnwcf.com/Article/details/gkspcists.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://m.share.tarul.cn/Article/details/gcisljynq.sHtML

[S41] C++：类与构造函数
来源：http://3g.yfazqb.com/Article/details/grugoldts.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.share.epnwcf.com/Article/details/ggbprgicx.sHtML

[S42] C++：继承与虚函数
来源：http://www.blog.vehdjk.com/Article/details/gopzitzoj.sHtML

class B : public Base { public: void f() override {} };
来源：http://wap.fktsv.cn/Article/details/geuwayoiu.sHtML

[S43] C++：智能指针
来源：http://read.share.yfazqb.com/Article/details/gangnylkd.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.m.share.yfazqb.com/Article/details/gotszadar.sHtML

[S44] C++：引用传参
来源：http://blog.epnwcf.com/Article/details/gowlezopw.sHtML

void inc(int &x) { ++x; }
来源：http://mobile.tarul.cn/Article/details/gplldbvxl.sHtML


<!-- 参考信息 -->