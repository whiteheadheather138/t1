代发 wailian999

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://baike.epnwcf.com/Article/details/gvlydqqlq.sHtML

[Q75] 日期格式化
来源：http://www.blog.tarul.cn/Article/details/ggucjcpuc.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://baike.sjlbkw.cn/Article/details/gfjgunrsl.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://read.share.sjlbkw.cn/Article/details/gddgysfnh.sHtML

[Q76] 按天统计
来源：http://m.share.bbcook.cn/Article/details/geunkmram.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.blog.fktsv.cn/Article/details/gjspgxyll.sHtML

[Q77] 时间加减
来源：http://www.m.share.epnwcf.com/Article/details/gflmftxht.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://mobile.vehdjk.com/Article/details/gzddozviv.sHtML

[Q78] 当前时间
来源：http://3g.yfazqb.com/Article/details/genzqiaoi.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.blog.tarul.cn/Article/details/gdrkryeol.sHtML

[Q79] 字符串拼接
来源：http://blog.fktsv.cn/Article/details/gatxcvftt.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://blog.tarul.cn/Article/details/gexmhrqan.sHtML

[Q80] 字符串截取
来源：http://read.share.epnwcf.com/Article/details/gfghlyrur.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.m.share.bbcook.cn/Article/details/grpujhcfy.sHtML

[Q81] 字符串替换
来源：http://m.share.vehdjk.com/Article/details/guxvxpdgc.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://baike.bbcook.cn/Article/details/gfwwvxpmq.sHtML

[Q82] 字符长度与字节长度
来源：http://m.share.yfazqb.com/Article/details/gncxxlvnz.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.m.share.fktsv.cn/Article/details/gkvgxyxzn.sHtML

[Q83] 大小写转换
来源：http://baike.yfazqb.com/Article/details/groytxzgi.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.m.share.yfazqb.com/Article/details/gwchmzttw.sHtML

[Q84] 去除首尾空格
来源：http://blog.bbcook.cn/Article/details/glvbcmgpb.sHtML

SELECT TRIM(name) FROM users;
来源：http://blog.fktsv.cn/Article/details/gglnhvizu.sHtML

[Q85] 数值取整
来源：http://blog.vehdjk.com/Article/details/gcnjskszz.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.share.fktsv.cn/Article/details/gubpxfhbt.sHtML

[Q86] 读取 JSON 字段
来源：http://www.blog.fktsv.cn/Article/details/gxnaungwb.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://baike.epnwcf.com/Article/details/grawaipes.sHtML

[Q87] JSON 字段做条件
来源：http://3g.epnwcf.com/Article/details/gjyezgvbi.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://wap.epnwcf.com/Article/details/gglytvozz.sHtML

[Q88] 行转列（条件聚合）
来源：http://wap.epnwcf.com/Article/details/gzfbusbqo.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.blog.vehdjk.com/Article/details/gjacaefzi.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://m.share.tarul.cn/Article/details/grgoaazdt.sHtML

[Q89] 判断表是否存在
来源：http://baike.vehdjk.com/Article/details/gpdewgbna.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://3g.bbcook.cn/Article/details/gzceipefp.sHtML

[Q90] 生成序号列
来源：http://3g.fktsv.cn/Article/details/gtmxoiiis.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://baike.bbcook.cn/Article/details/gxdzciltq.sHtML

================================================================================
来源：http://www.blog.epnwcf.com/Article/details/gmhrwddaz.sHtML

R. Bash 专题
来源：http://mobile.tarul.cn/Article/details/ggfcaftxr.sHtML

================================================================================
来源：http://wap.vehdjk.com/Article/details/gtcmcsuoy.sHtML

[R01] shebang 与严格模式
来源：http://mobile.bbcook.cn/Article/details/gkvncwdfz.sHtML

#!/usr/bin/env bash
来源：http://3g.fktsv.cn/Article/details/gfgocqzni.sHtML

set -euo pipefail
来源：http://blog.epnwcf.com/Article/details/gmintaftf.sHtML

[R02] 变量赋值与使用
来源：http://m.share.epnwcf.com/Article/details/goiaevgte.sHtML

name="Tom"; echo "$name"
来源：http://www.share.bbcook.cn/Article/details/gdyhjbkmr.sHtML

[R03] 只读变量
来源：http://mobile.sjlbkw.cn/Article/details/gtlnmofju.sHtML

readonly PI=3.14
来源：http://www.blog.bbcook.cn/Article/details/gmgiejera.sHtML

[R04] 位置参数
来源：http://read.share.epnwcf.com/Article/details/gvzbbovmr.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://mobile.fktsv.cn/Article/details/gkkdwhnff.sHtML

[R05] 参数默认值
来源：http://blog.fktsv.cn/Article/details/gruloalrg.sHtML

name="${1:-default}"
来源：http://wap.bbcook.cn/Article/details/gdxpzbbuw.sHtML

[R06] 判断命令是否存在
来源：http://www.share.epnwcf.com/Article/details/guaesvzkf.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://wap.yfazqb.com/Article/details/gdvynxshw.sHtML

[R07] if 判断文件
来源：http://baike.bbcook.cn/Article/details/gakcuszpy.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://blog.yfazqb.com/Article/details/gjfvgbbfk.sHtML

[R08] 数值比较
来源：http://wap.epnwcf.com/Article/details/grwembszh.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.blog.bbcook.cn/Article/details/glvjininr.sHtML

[R09] 字符串比较
来源：http://www.share.epnwcf.com/Article/details/gwabyxcts.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://baike.yfazqb.com/Article/details/gzkkvdbgm.sHtML

[R10] 正则匹配
来源：http://mobile.fktsv.cn/Article/details/gcnevcmcm.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.blog.tarul.cn/Article/details/gewakmekj.sHtML

[R11] case 多分支
来源：http://mobile.sjlbkw.cn/Article/details/goyxcrbyb.sHtML

case "$1" in
来源：http://3g.yfazqb.com/Article/details/gupvnwkkk.sHtML

start) echo "启动" ;;
来源：http://baike.sjlbkw.cn/Article/details/gftsxyole.sHtML

stop)  echo "停止" ;;
来源：http://read.share.fktsv.cn/Article/details/gnahrqyju.sHtML

*)     echo "未知命令" ;;
来源：http://www.blog.fktsv.cn/Article/details/gvisayhnr.sHtML

esac
来源：http://m.share.vehdjk.com/Article/details/goeclbhxo.sHtML

[R12] for 遍历文件
来源：http://m.share.fktsv.cn/Article/details/gnwswethk.sHtML

for f in *.txt; do echo "$f"; done
来源：http://wap.yfazqb.com/Article/details/gewythexb.sHtML

[R13] for 计数循环
来源：http://www.blog.sjlbkw.cn/Article/details/ghyniguid.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.blog.tarul.cn/Article/details/ghpzflnil.sHtML

[R14] C 风格 for
来源：http://baike.sjlbkw.cn/Article/details/grognhoaj.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://mobile.sjlbkw.cn/Article/details/gxrobwfit.sHtML

[R15] while 逐行读文件
来源：http://www.blog.fktsv.cn/Article/details/gnobcbmuc.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://blog.bbcook.cn/Article/details/gxtvuyyve.sHtML

[R16] until 等待条件
来源：http://wap.sjlbkw.cn/Article/details/gdtxgfoxp.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://baike.bbcook.cn/Article/details/guwisssla.sHtML

[R17] 数组定义与取值
来源：http://www.share.tarul.cn/Article/details/gdauvqqte.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.m.share.epnwcf.com/Article/details/gqlbcwvan.sHtML

[R18] 遍历数组
来源：http://baike.sjlbkw.cn/Article/details/gpwrotuhd.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://mobile.epnwcf.com/Article/details/gabijdsaz.sHtML

[R19] 数组长度
来源：http://www.m.share.vehdjk.com/Article/details/gttzafiof.sHtML

echo "${#arr[@]}"
来源：http://blog.sjlbkw.cn/Article/details/gsxrbbrpk.sHtML

[R20] 关联数组（字典）
来源：http://mobile.yfazqb.com/Article/details/gckmqrryf.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://blog.epnwcf.com/Article/details/gywmttmwi.sHtML

[R21] 字符串长度
来源：http://www.share.tarul.cn/Article/details/gtkhhqsan.sHtML

echo "${#s}"
来源：http://blog.vehdjk.com/Article/details/gnevafvrj.sHtML

[R22] 截取子串
来源：http://blog.bbcook.cn/Article/details/gtzlszndb.sHtML

echo "${s:0:5}"
来源：http://www.m.share.tarul.cn/Article/details/gvksgjltx.sHtML

[R23] 字符串替换
来源：http://mobile.fktsv.cn/Article/details/gkcvdrtsk.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://blog.epnwcf.com/Article/details/gtkqdjrnb.sHtML

[R24] 大小写转换
来源：http://www.blog.bbcook.cn/Article/details/gbsrrxefg.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://m.share.epnwcf.com/Article/details/gcfogzouo.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.blog.fktsv.cn/Article/details/gjbachcts.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://read.share.bbcook.cn/Article/details/guwkrvrvj.sHtML

[R26] 命令替换
来源：http://www.m.share.tarul.cn/Article/details/gxkesrdyu.sHtML

now=$(date +%F); echo "$now"
来源：http://baike.bbcook.cn/Article/details/glxcvpyoq.sHtML

[R27] 算术展开
来源：http://www.blog.tarul.cn/Article/details/gmskbkasa.sHtML

echo $((1 + 2 * 3))
来源：http://mobile.bbcook.cn/Article/details/ggxvofqtm.sHtML

[R28] 浮点运算
来源：http://wap.sjlbkw.cn/Article/details/ggrrxxhwn.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.m.share.epnwcf.com/Article/details/gkjeqqnpi.sHtML

[R29] 定义函数
来源：http://3g.vehdjk.com/Article/details/gdytxwehx.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.blog.yfazqb.com/Article/details/gmlorlgxl.sHtML

[R30] 函数返回状态码
来源：http://blog.fktsv.cn/Article/details/gyfenbexn.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.share.tarul.cn/Article/details/gamugphph.sHtML

[R31] 局部变量
来源：http://www.m.share.yfazqb.com/Article/details/gqdaymrnk.sHtML

f() { local x=1; echo "$x"; }
来源：http://blog.yfazqb.com/Article/details/gfqmdzsla.sHtML

[R32] 参数个数校验
来源：http://mobile.epnwcf.com/Article/details/gfuzblvql.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.blog.fktsv.cn/Article/details/gzdcxjybd.sHtML

[R33] 捕获错误并提示行号
来源：http://baike.fktsv.cn/Article/details/gcqgfrsxr.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://3g.vehdjk.com/Article/details/gqeifjbrg.sHtML

[R34] 退出时清理
来源：http://read.share.tarul.cn/Article/details/ggtluvfoq.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.yfazqb.com/Article/details/gibkhlejd.sHtML

[R35] 后台执行并等待
来源：http://m.share.fktsv.cn/Article/details/gcdyvdyqx.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://blog.fktsv.cn/Article/details/gzaurbobr.sHtML

[R36] 并发执行多个任务
来源：http://m.share.sjlbkw.cn/Article/details/gbnkqebxw.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://m.share.vehdjk.com/Article/details/ghojlxuwe.sHtML

[R37] 把输出赋给变量
来源：http://www.m.share.epnwcf.com/Article/details/golssqfhg.sHtML

files=$(ls -1)
来源：http://baike.tarul.cn/Article/details/gbezzqqfk.sHtML

[R38] 管道串联
来源：http://mobile.epnwcf.com/Article/details/gekxmtvfr.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.blog.fktsv.cn/Article/details/gfjoquoxa.sHtML

[R39] 重定向标准输出与错误
来源：http://www.m.share.vehdjk.com/Article/details/gidwtuckl.sHtML

cmd > out.log 2>&1
来源：http://3g.bbcook.cn/Article/details/ginjjzfnw.sHtML

[R40] 追加写日志
来源：http://blog.tarul.cn/Article/details/gcjnlyolz.sHtML

echo "log" >> out.log
来源：http://baike.fktsv.cn/Article/details/gfqyqnqlf.sHtML

[R41] 丢弃输出
来源：http://www.m.share.sjlbkw.cn/Article/details/gjifvfidl.sHtML

cmd >/dev/null 2>&1
来源：http://www.blog.sjlbkw.cn/Article/details/grmxcaxul.sHtML

[R42] 输入重定向
来源：http://blog.sjlbkw.cn/Article/details/gzibdzgrw.sHtML

wc -l < a.txt
来源：http://3g.tarul.cn/Article/details/glqgsljhx.sHtML

[R43] 按名字查找文件
来源：http://3g.yfazqb.com/Article/details/gvkpxrits.sHtML

find . -name "*.log" -type f
来源：http://m.share.epnwcf.com/Article/details/gsnwocanx.sHtML

[R44] 按修改时间查找
来源：http://wap.epnwcf.com/Article/details/gnpfrvucv.sHtML

find . -mtime -7 -type f
来源：http://read.share.epnwcf.com/Article/details/gxoercpgh.sHtML

[R45] 批量删除
来源：http://m.share.epnwcf.com/Article/details/guylglikc.sHtML

find . -name "*.tmp" -delete
来源：http://baike.vehdjk.com/Article/details/glokmodkz.sHtML

[R46] 递归替换文件内容
来源：http://3g.vehdjk.com/Article/details/gdvmciqlz.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://blog.sjlbkw.cn/Article/details/gxikotzox.sHtML

[R47] sed 单行替换
来源：http://blog.vehdjk.com/Article/details/gtnfbibgk.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://baike.epnwcf.com/Article/details/gtvwsfgdp.sHtML

[R48] awk 取指定列
来源：http://wap.epnwcf.com/Article/details/gmprgswfg.sHtML

awk '{print $1, $3}' a.txt
来源：http://blog.fktsv.cn/Article/details/gqlqqqoto.sHtML

[R49] awk 带条件
来源：http://blog.fktsv.cn/Article/details/gnrrrdumy.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://m.share.tarul.cn/Article/details/gleuwgbic.sHtML

[R50] awk 求和
来源：http://m.share.epnwcf.com/Article/details/gwywjkutp.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://baike.bbcook.cn/Article/details/gwcooaizm.sHtML

[R51] 排序去重取前几
来源：http://www.m.share.fktsv.cn/Article/details/gzwfftyow.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://wap.sjlbkw.cn/Article/details/gtzgmectb.sHtML

[R52] 统计行数
来源：http://mobile.sjlbkw.cn/Article/details/gzvyrmmmq.sHtML

wc -l a.txt
来源：http://baike.tarul.cn/Article/details/goyalmelr.sHtML

[R53] 查看文件头与实时尾
来源：http://m.share.yfazqb.com/Article/details/ghuehctzx.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://m.share.yfazqb.com/Article/details/gkmnovrsn.sHtML

[R54] 比较两个文件
来源：http://3g.sjlbkw.cn/Article/details/gnpymewcw.sHtML

diff a.txt b.txt
来源：http://read.share.vehdjk.com/Article/details/gsvzjslgd.sHtML

[R55] 压缩与解压
来源：http://read.share.yfazqb.com/Article/details/gtqlfcinx.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.m.share.vehdjk.com/Article/details/gxfxxcxod.sHtML

[R56] 远程拷贝
来源：http://mobile.bbcook.cn/Article/details/gygrwwxfj.sHtML

scp file user@host:/path/
来源：http://blog.tarul.cn/Article/details/glntdigqr.sHtML

[R57] 远程执行命令
来源：http://www.m.share.tarul.cn/Article/details/gcsjidgsu.sHtML

ssh user@host 'uptime'
来源：http://3g.fktsv.cn/Article/details/govlgqfss.sHtML

[R58] 下载文件
来源：http://m.share.bbcook.cn/Article/details/gnccngnoe.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://3g.yfazqb.com/Article/details/glqonenwe.sHtML

[R59] 发 POST JSON
来源：http://baike.epnwcf.com/Article/details/ghkowqgyf.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://3g.fktsv.cn/Article/details/gbmfdfspb.sHtML

[R60] 只看 HTTP 状态码
来源：http://blog.tarul.cn/Article/details/gxflldczz.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://3g.sjlbkw.cn/Article/details/gjszqxibf.sHtML

[R61] 磁盘占用
来源：http://wap.tarul.cn/Article/details/guvncqqdv.sHtML

df -h;  du -sh *
来源：http://blog.sjlbkw.cn/Article/details/gvxluaeqv.sHtML

[R62] 找最占空间的文件
来源：http://www.share.vehdjk.com/Article/details/groxlsgtj.sHtML

du -ah . | sort -rh | head -10
来源：http://www.share.epnwcf.com/Article/details/gzainnwra.sHtML

[R63] 内存与进程
来源：http://www.blog.yfazqb.com/Article/details/gnkewtfzw.sHtML

free -h;  ps aux | grep nginx
来源：http://baike.tarul.cn/Article/details/gkuqdmsdl.sHtML

[R64] 结束进程
来源：http://www.share.sjlbkw.cn/Article/details/gtjapdhhq.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.m.share.vehdjk.com/Article/details/gceccigfj.sHtML

[R65] 查看端口占用
来源：http://read.share.tarul.cn/Article/details/gcsvszzhe.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://3g.bbcook.cn/Article/details/gvnxeijba.sHtML

[R66] 定时任务
来源：http://mobile.sjlbkw.cn/Article/details/gzzupunuu.sHtML

crontab -e;  crontab -l
来源：http://baike.bbcook.cn/Article/details/gzlgdmnus.sHtML

[R67] 生成随机十六进制串
来源：http://www.blog.bbcook.cn/Article/details/gsdqelcpv.sHtML

openssl rand -hex 16
来源：http://baike.yfazqb.com/Article/details/gcycvktzi.sHtML

[R68] 计算文件校验值
来源：http://read.share.epnwcf.com/Article/details/gbqihinjx.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://blog.sjlbkw.cn/Article/details/gstjgnyck.sHtML

[R69] 生成随机密码
来源：http://m.share.yfazqb.com/Article/details/gwdgmpkwk.sHtML

head -c 16 /dev/urandom | base64
来源：http://blog.epnwcf.com/Article/details/gjgmopykj.sHtML

[R70] 时间戳与互转
来源：http://m.share.tarul.cn/Article/details/gipfbhrva.sHtML

date +%s;  date -d @1700000000
来源：http://blog.bbcook.cn/Article/details/gujlzvbwi.sHtML

[R71] 日期格式化
来源：http://baike.sjlbkw.cn/Article/details/gualrigsk.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.share.sjlbkw.cn/Article/details/gkbfljmdi.sHtML

[R72] 等待端口就绪
来源：http://www.share.bbcook.cn/Article/details/gtihbryvb.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://blog.yfazqb.com/Article/details/gqexqyial.sHtML

[R73] 分割大日志
来源：http://www.m.share.tarul.cn/Article/details/gajikuvmf.sHtML

split -l 1000 big.log part_
来源：http://baike.vehdjk.com/Article/details/gkhafnpqy.sHtML

[R74] 批量重命名
来源：http://www.m.share.epnwcf.com/Article/details/gthhvmuks.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.blog.yfazqb.com/Article/details/gztepsoxo.sHtML

[R75] 导出环境变量
来源：http://baike.yfazqb.com/Article/details/gxrqnipei.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.share.yfazqb.com/Article/details/gubhheozh.sHtML

[R76] 使用临时文件
来源：http://blog.yfazqb.com/Article/details/gdrftjfur.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.yfazqb.com/Article/details/gfxvjzlrn.sHtML

[R77] 读取用户输入
来源：http://mobile.fktsv.cn/Article/details/gkxyxsnym.sHtML

read -rp "请输入: " ans
来源：http://www.blog.tarul.cn/Article/details/gdzqbpibx.sHtML

[R78] 交互式菜单
来源：http://www.share.yfazqb.com/Article/details/gicggevfo.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://3g.sjlbkw.cn/Article/details/grvpakjbt.sHtML

[R79] 解析命令行选项
来源：http://wap.bbcook.cn/Article/details/ggwrycrwt.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mobile.fktsv.cn/Article/details/ghdxvrlqo.sHtML

[R80] 查看脚本执行耗时
来源：http://3g.tarul.cn/Article/details/guxyqmvhp.sHtML

time ./run.sh
来源：http://3g.bbcook.cn/Article/details/giskhidnq.sHtML

================================================================================
来源：http://m.share.tarul.cn/Article/details/gvfewknwn.sHtML

S. C / C++ 专题
来源：http://www.blog.fktsv.cn/Article/details/gpfqtwror.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/giskgjiff.sHtML

[S01] C：Hello World
来源：http://read.share.fktsv.cn/Article/details/gplsobwzd.sHtML

#include <stdio.h>
来源：http://m.share.fktsv.cn/Article/details/gzyzvcwvm.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.blog.bbcook.cn/Article/details/guhfbtiil.sHtML

[S02] C：变量与格式化输出
来源：http://blog.vehdjk.com/Article/details/gndkpgibu.sHtML

int a = 10; printf("%d\n", a);
来源：http://3g.tarul.cn/Article/details/gsongmmed.sHtML

[S03] C：读入整数
来源：http://mobile.yfazqb.com/Article/details/gfjdopxhl.sHtML

int x; scanf("%d", &x);
来源：http://blog.epnwcf.com/Article/details/ggyygnych.sHtML

[S04] C：字符串复制
来源：http://baike.fktsv.cn/Article/details/gpxglyenu.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://read.share.epnwcf.com/Article/details/gihqzlqkv.sHtML

[S05] C：字符串长度
来源：http://wap.sjlbkw.cn/Article/details/gujzvpvnq.sHtML

strlen(s)
来源：http://www.m.share.epnwcf.com/Article/details/ggozzdklp.sHtML

[S06] C：字符串比较
来源：http://m.share.fktsv.cn/Article/details/gzcvmhwyz.sHtML

strcmp(a, b) == 0
来源：http://blog.epnwcf.com/Article/details/gfagdcvnz.sHtML

[S07] C：数组遍历求和
来源：http://m.share.bbcook.cn/Article/details/gemzmwmmw.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://read.share.tarul.cn/Article/details/gokiyezjr.sHtML

[S08] C：动态内存分配与释放
来源：http://read.share.fktsv.cn/Article/details/gwaqanpqb.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://m.share.bbcook.cn/Article/details/gxeinqkcx.sHtML

[S09] C：结构体定义与初始化
来源：http://blog.fktsv.cn/Article/details/gkulpnvwj.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://m.share.bbcook.cn/Article/details/gktlcklan.sHtML

[S10] C：指针与解引用
来源：http://m.share.tarul.cn/Article/details/gdjffbqou.sHtML

int *p = &a;  *p = 5;
来源：http://www.m.share.sjlbkw.cn/Article/details/gbyfdwkgy.sHtML

[S11] C：逐行读文件
来源：http://blog.yfazqb.com/Article/details/gsusymhlx.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.blog.sjlbkw.cn/Article/details/gefcfbaxy.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://3g.fktsv.cn/Article/details/ggdalnaiu.sHtML

fclose(f);
来源：http://www.m.share.yfazqb.com/Article/details/gcpeotwpw.sHtML

[S12] C：写文件
来源：http://www.m.share.sjlbkw.cn/Article/details/gpnszevoy.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.m.share.vehdjk.com/Article/details/gojhicbfm.sHtML

[S13] C：宏定义
来源：http://3g.tarul.cn/Article/details/gyyzvazmc.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://blog.sjlbkw.cn/Article/details/gjwvbqwzm.sHtML

[S14] C：枚举
来源：http://wap.fktsv.cn/Article/details/gkrcanzgl.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.share.tarul.cn/Article/details/gbtonthqq.sHtML

[S15] C：类型转换
来源：http://www.share.sjlbkw.cn/Article/details/gqnpclekz.sHtML

(double) a / b
来源：http://blog.bbcook.cn/Article/details/gmpewfidn.sHtML

[S16] C：位操作置位
来源：http://m.share.fktsv.cn/Article/details/garancexk.sHtML

x |= (1 << 3);
来源：http://mobile.vehdjk.com/Article/details/gzzaofbnp.sHtML

[S17] C：安全拼接字符串
来源：http://baike.sjlbkw.cn/Article/details/ggvkrjpkz.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://mobile.sjlbkw.cn/Article/details/gpsaseuvz.sHtML

[S18] C：命令行参数
来源：http://3g.sjlbkw.cn/Article/details/gtxyijtcm.sHtML

int main(int argc, char **argv)
来源：http://m.share.vehdjk.com/Article/details/gxpekdger.sHtML

[S19] C：快速排序
来源：http://baike.sjlbkw.cn/Article/details/gmklchkal.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.blog.epnwcf.com/Article/details/gwbrdvhen.sHtML

[S20] C：二分查找
来源：http://wap.epnwcf.com/Article/details/gvwefrsee.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://blog.yfazqb.com/Article/details/gqoxpgrel.sHtML

[S21] C：字符类别判断
来源：http://read.share.fktsv.cn/Article/details/gnvbbnduz.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.blog.tarul.cn/Article/details/gvrixnegg.sHtML

[S22] C：字符串转数字
来源：http://www.blog.tarul.cn/Article/details/gjbyvjcqg.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://read.share.tarul.cn/Article/details/gfcthjtgx.sHtML

[S23] C：随机数
来源：http://www.m.share.tarul.cn/Article/details/gfvmbupua.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.share.sjlbkw.cn/Article/details/gvvwissrt.sHtML

[S24] C：获取本地时间
来源：http://www.share.sjlbkw.cn/Article/details/gkzphaitc.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://blog.vehdjk.com/Article/details/gfzgmlltx.sHtML

[S25] C：内存拷贝
来源：http://www.blog.yfazqb.com/Article/details/gqiccdppw.sHtML

memcpy(dst, src, n);
来源：http://baike.vehdjk.com/Article/details/gkyfwqjuu.sHtML

[S26] C：内存清零
来源：http://baike.bbcook.cn/Article/details/gpmbyxjnv.sHtML

memset(a, 0, sizeof a);
来源：http://baike.yfazqb.com/Article/details/gnucgpsiz.sHtML

[S27] C：定义常量
来源：http://www.blog.bbcook.cn/Article/details/gpuomjwwm.sHtML

const double PI = 3.14159;
来源：http://www.m.share.yfazqb.com/Article/details/geykiksuo.sHtML

[S28] C：静态变量
来源：http://www.share.yfazqb.com/Article/details/gxrraxvar.sHtML

static int counter = 0;
来源：http://www.blog.tarul.cn/Article/details/gpzyrabxd.sHtML

[S29] C：变参函数
来源：http://3g.fktsv.cn/Article/details/gebozvlpu.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://baike.fktsv.cn/Article/details/gezaabslz.sHtML

[S30] C：头文件保护
来源：http://blog.vehdjk.com/Article/details/gznxnscqg.sHtML

#ifndef X_H
来源：http://3g.epnwcf.com/Article/details/gszstikfy.sHtML

#define X_H
来源：http://wap.bbcook.cn/Article/details/gavpyigju.sHtML

#endif
来源：http://m.share.epnwcf.com/Article/details/gsecjnahe.sHtML

[S31] C++：Hello World
来源：http://www.share.epnwcf.com/Article/details/gjqtlwixr.sHtML

#include <iostream>
来源：http://3g.vehdjk.com/Article/details/gwkqqibax.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://wap.epnwcf.com/Article/details/gspgtpbqr.sHtML

[S32] C++：字符串
来源：http://baike.tarul.cn/Article/details/gmjjsqvcp.sHtML

std::string s = "hi";  s += "!";
来源：http://wap.fktsv.cn/Article/details/gcahcwhpp.sHtML

[S33] C++：vector 增删
来源：http://read.share.fktsv.cn/Article/details/gqkdnepsc.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://blog.yfazqb.com/Article/details/guvkofqgl.sHtML

[S34] C++：遍历 vector
来源：http://wap.vehdjk.com/Article/details/gbkwfkptk.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.share.sjlbkw.cn/Article/details/gqkgnpfno.sHtML

[S35] C++：map
来源：http://read.share.fktsv.cn/Article/details/gffimgiyv.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.sjlbkw.cn/Article/details/gphlzncpg.sHtML

[S36] C++：unordered_map
来源：http://blog.tarul.cn/Article/details/gprcrznij.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.yfazqb.com/Article/details/gploqjpuv.sHtML

[S37] C++：set
来源：http://www.m.share.fktsv.cn/Article/details/gdvnocnev.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.m.share.tarul.cn/Article/details/gujzcjuqi.sHtML

[S38] C++：排序
来源：http://wap.vehdjk.com/Article/details/gieatxwvx.sHtML

std::sort(v.begin(), v.end());
来源：http://baike.sjlbkw.cn/Article/details/gnsoetppd.sHtML

[S39] C++：自定义比较器排序
来源：http://wap.epnwcf.com/Article/details/gsiednpnl.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.m.share.epnwcf.com/Article/details/gfoqrjvtn.sHtML

[S40] C++：查找元素
来源：http://m.share.sjlbkw.cn/Article/details/gfnyxpwdw.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://wap.yfazqb.com/Article/details/gfrvsvrad.sHtML

[S41] C++：类与构造函数
来源：http://mobile.epnwcf.com/Article/details/gifwsycco.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.blog.epnwcf.com/Article/details/ghycqqogs.sHtML

[S42] C++：继承与虚函数
来源：http://3g.epnwcf.com/Article/details/gennbtvac.sHtML

class B : public Base { public: void f() override {} };
来源：http://wap.epnwcf.com/Article/details/grwptioxq.sHtML

[S43] C++：智能指针
来源：http://m.share.fktsv.cn/Article/details/gtlzxailb.sHtML

auto p = std::make_unique<int>(5);
来源：http://3g.fktsv.cn/Article/details/gvhahbaym.sHtML

[S44] C++：引用传参
来源：http://read.share.yfazqb.com/Article/details/gsnthrbqk.sHtML

void inc(int &x) { ++x; }
来源：http://m.share.bbcook.cn/Article/details/gvedcvwal.sHtML


<!-- 参考信息 -->