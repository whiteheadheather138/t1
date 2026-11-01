代发 wailian999

[Q76] 按天统计
来源：http://m.share.epnwcf.com/Article/details/gpjbiwyck.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://mobile.bbcook.cn/Article/details/gqizoqcia.sHtML

[Q77] 时间加减
来源：http://www.m.share.sjlbkw.cn/Article/details/gasdqcdhv.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://m.share.tarul.cn/Article/details/gamjphfsm.sHtML

[Q78] 当前时间
来源：http://m.share.yfazqb.com/Article/details/gnqwybuts.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.blog.vehdjk.com/Article/details/gfgooqmvn.sHtML

[Q79] 字符串拼接
来源：http://3g.tarul.cn/Article/details/gnfqtpuan.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://baike.yfazqb.com/Article/details/gtfhrqdyf.sHtML

[Q80] 字符串截取
来源：http://baike.fktsv.cn/Article/details/gbvnqklxc.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://3g.sjlbkw.cn/Article/details/gwzkipjjk.sHtML

[Q81] 字符串替换
来源：http://www.blog.sjlbkw.cn/Article/details/gdwjyvwbf.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.blog.bbcook.cn/Article/details/gmlhbajlx.sHtML

[Q82] 字符长度与字节长度
来源：http://wap.bbcook.cn/Article/details/gsraakjcy.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://blog.bbcook.cn/Article/details/gqnqavltz.sHtML

[Q83] 大小写转换
来源：http://m.share.sjlbkw.cn/Article/details/gicqjridu.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://baike.fktsv.cn/Article/details/gclgyfrif.sHtML

[Q84] 去除首尾空格
来源：http://www.share.yfazqb.com/Article/details/gyvydqiwz.sHtML

SELECT TRIM(name) FROM users;
来源：http://3g.bbcook.cn/Article/details/gsjzjiesm.sHtML

[Q85] 数值取整
来源：http://blog.vehdjk.com/Article/details/gzxypehex.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://blog.vehdjk.com/Article/details/gogsesrhi.sHtML

[Q86] 读取 JSON 字段
来源：http://3g.fktsv.cn/Article/details/govxhnfhp.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.blog.tarul.cn/Article/details/gtgrkjywc.sHtML

[Q87] JSON 字段做条件
来源：http://read.share.sjlbkw.cn/Article/details/gzjsvzjrb.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.m.share.bbcook.cn/Article/details/goajydoah.sHtML

[Q88] 行转列（条件聚合）
来源：http://m.share.epnwcf.com/Article/details/gsqwvvxiu.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://read.share.fktsv.cn/Article/details/gpkoexmxl.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://blog.tarul.cn/Article/details/glxlzfrey.sHtML

[Q89] 判断表是否存在
来源：http://www.m.share.epnwcf.com/Article/details/ghujbpxqd.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://read.share.vehdjk.com/Article/details/gaafqsodb.sHtML

[Q90] 生成序号列
来源：http://www.m.share.yfazqb.com/Article/details/gqgerevcg.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.share.epnwcf.com/Article/details/gzmzzoycu.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/gpgsavwwx.sHtML

R. Bash 专题
来源：http://blog.vehdjk.com/Article/details/glkixkpyg.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/gosjzbdbl.sHtML

[R01] shebang 与严格模式
来源：http://3g.tarul.cn/Article/details/gwzzmdzlp.sHtML

#!/usr/bin/env bash
来源：http://read.share.fktsv.cn/Article/details/gvsqfjecx.sHtML

set -euo pipefail
来源：http://blog.bbcook.cn/Article/details/gjvrltolh.sHtML

[R02] 变量赋值与使用
来源：http://www.blog.epnwcf.com/Article/details/ghyvclsge.sHtML

name="Tom"; echo "$name"
来源：http://baike.vehdjk.com/Article/details/gxpvrkvtj.sHtML

[R03] 只读变量
来源：http://read.share.fktsv.cn/Article/details/gjjjxpuja.sHtML

readonly PI=3.14
来源：http://baike.sjlbkw.cn/Article/details/geryilmtr.sHtML

[R04] 位置参数
来源：http://blog.epnwcf.com/Article/details/gpninxfbc.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.m.share.epnwcf.com/Article/details/gxotwyqww.sHtML

[R05] 参数默认值
来源：http://wap.yfazqb.com/Article/details/gwwbvgqup.sHtML

name="${1:-default}"
来源：http://blog.fktsv.cn/Article/details/gtmrrcepr.sHtML

[R06] 判断命令是否存在
来源：http://m.share.bbcook.cn/Article/details/glblnjvpx.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://blog.epnwcf.com/Article/details/gdsczwzxc.sHtML

[R07] if 判断文件
来源：http://blog.yfazqb.com/Article/details/gtuuczqnx.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://read.share.epnwcf.com/Article/details/gsbtzmzuj.sHtML

[R08] 数值比较
来源：http://www.m.share.epnwcf.com/Article/details/ggwkaaope.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://m.share.epnwcf.com/Article/details/gyvjfwlmt.sHtML

[R09] 字符串比较
来源：http://wap.vehdjk.com/Article/details/gfmwefhid.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.blog.vehdjk.com/Article/details/ghsselfgv.sHtML

[R10] 正则匹配
来源：http://www.share.epnwcf.com/Article/details/gybtgafed.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.blog.fktsv.cn/Article/details/gdvxgpbxq.sHtML

[R11] case 多分支
来源：http://wap.yfazqb.com/Article/details/gaugxjemn.sHtML

case "$1" in
来源：http://baike.tarul.cn/Article/details/gdscvncpj.sHtML

start) echo "启动" ;;
来源：http://blog.sjlbkw.cn/Article/details/gfqtcrtju.sHtML

stop)  echo "停止" ;;
来源：http://baike.bbcook.cn/Article/details/ggiouyvit.sHtML

*)     echo "未知命令" ;;
来源：http://3g.tarul.cn/Article/details/gttfjwbgc.sHtML

esac
来源：http://baike.bbcook.cn/Article/details/gnwdohyki.sHtML

[R12] for 遍历文件
来源：http://www.blog.yfazqb.com/Article/details/gputkiqkf.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.share.bbcook.cn/Article/details/grkvxddyx.sHtML

[R13] for 计数循环
来源：http://wap.epnwcf.com/Article/details/guyrvsowr.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://m.share.sjlbkw.cn/Article/details/gijyvuepp.sHtML

[R14] C 风格 for
来源：http://read.share.bbcook.cn/Article/details/ghycpipem.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://wap.bbcook.cn/Article/details/gdfxbzgru.sHtML

[R15] while 逐行读文件
来源：http://3g.vehdjk.com/Article/details/gdfnfgqii.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://m.share.fktsv.cn/Article/details/gqxhftknf.sHtML

[R16] until 等待条件
来源：http://mobile.vehdjk.com/Article/details/gmvihdtmj.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://3g.fktsv.cn/Article/details/gbzabgfsk.sHtML

[R17] 数组定义与取值
来源：http://www.share.sjlbkw.cn/Article/details/gokxrsimd.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://baike.yfazqb.com/Article/details/gaarbxzjb.sHtML

[R18] 遍历数组
来源：http://www.m.share.tarul.cn/Article/details/gqiwlfhzb.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.share.tarul.cn/Article/details/gxncxlnml.sHtML

[R19] 数组长度
来源：http://mobile.fktsv.cn/Article/details/gfzqnazle.sHtML

echo "${#arr[@]}"
来源：http://www.m.share.sjlbkw.cn/Article/details/gybelrjjw.sHtML

[R20] 关联数组（字典）
来源：http://mobile.fktsv.cn/Article/details/gplpmdaff.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://read.share.bbcook.cn/Article/details/gxijjqmpj.sHtML

[R21] 字符串长度
来源：http://www.m.share.tarul.cn/Article/details/gmfigqejd.sHtML

echo "${#s}"
来源：http://3g.fktsv.cn/Article/details/gjuoalnhv.sHtML

[R22] 截取子串
来源：http://mobile.fktsv.cn/Article/details/ggxwxmour.sHtML

echo "${s:0:5}"
来源：http://mobile.fktsv.cn/Article/details/gswlscgem.sHtML

[R23] 字符串替换
来源：http://www.m.share.epnwcf.com/Article/details/guhkfafvi.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://read.share.vehdjk.com/Article/details/gyqmyfprs.sHtML

[R24] 大小写转换
来源：http://www.m.share.vehdjk.com/Article/details/gqrynalka.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://3g.bbcook.cn/Article/details/gwkscirvg.sHtML

[R25] 去后缀 / 去前缀
来源：http://baike.epnwcf.com/Article/details/gbvqcbuqn.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://blog.yfazqb.com/Article/details/ggdlmdzje.sHtML

[R26] 命令替换
来源：http://3g.yfazqb.com/Article/details/ghamxrxgz.sHtML

now=$(date +%F); echo "$now"
来源：http://baike.sjlbkw.cn/Article/details/gnhohzjnx.sHtML

[R27] 算术展开
来源：http://www.blog.tarul.cn/Article/details/gskwkocxv.sHtML

echo $((1 + 2 * 3))
来源：http://blog.fktsv.cn/Article/details/gvcsoqsjo.sHtML

[R28] 浮点运算
来源：http://m.share.epnwcf.com/Article/details/gpigtltfd.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.m.share.tarul.cn/Article/details/gfxajhtti.sHtML

[R29] 定义函数
来源：http://3g.epnwcf.com/Article/details/ggdknyrvi.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://wap.epnwcf.com/Article/details/gejrxxtoh.sHtML

[R30] 函数返回状态码
来源：http://wap.fktsv.cn/Article/details/ggjzkhsor.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://wap.fktsv.cn/Article/details/gyslqngpw.sHtML

[R31] 局部变量
来源：http://www.share.vehdjk.com/Article/details/gbidkpccu.sHtML

f() { local x=1; echo "$x"; }
来源：http://mobile.sjlbkw.cn/Article/details/grkxeezsw.sHtML

[R32] 参数个数校验
来源：http://m.share.epnwcf.com/Article/details/gzpylrajs.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://wap.bbcook.cn/Article/details/gwtdiwtsm.sHtML

[R33] 捕获错误并提示行号
来源：http://m.share.bbcook.cn/Article/details/gjvsiakzv.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://read.share.vehdjk.com/Article/details/goqvrcwxn.sHtML

[R34] 退出时清理
来源：http://www.m.share.yfazqb.com/Article/details/gbfxvalbz.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://3g.epnwcf.com/Article/details/gmuhmpeub.sHtML

[R35] 后台执行并等待
来源：http://baike.epnwcf.com/Article/details/govzkhbpu.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://read.share.epnwcf.com/Article/details/gfkpbyhuv.sHtML

[R36] 并发执行多个任务
来源：http://www.m.share.sjlbkw.cn/Article/details/gifzsazvp.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.blog.epnwcf.com/Article/details/gswmdafyt.sHtML

[R37] 把输出赋给变量
来源：http://mobile.tarul.cn/Article/details/grtfpkdrc.sHtML

files=$(ls -1)
来源：http://m.share.sjlbkw.cn/Article/details/gireiacmm.sHtML

[R38] 管道串联
来源：http://wap.bbcook.cn/Article/details/gcznvqnya.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.blog.vehdjk.com/Article/details/gurmrleju.sHtML

[R39] 重定向标准输出与错误
来源：http://3g.sjlbkw.cn/Article/details/gmmxovgpi.sHtML

cmd > out.log 2>&1
来源：http://blog.fktsv.cn/Article/details/gwiokcuoi.sHtML

[R40] 追加写日志
来源：http://3g.tarul.cn/Article/details/gmpehthoe.sHtML

echo "log" >> out.log
来源：http://wap.bbcook.cn/Article/details/glpfuxfvi.sHtML

[R41] 丢弃输出
来源：http://3g.fktsv.cn/Article/details/gxbhxfnjp.sHtML

cmd >/dev/null 2>&1
来源：http://www.blog.sjlbkw.cn/Article/details/gnvcyygtb.sHtML

[R42] 输入重定向
来源：http://3g.bbcook.cn/Article/details/gdcdhrhsq.sHtML

wc -l < a.txt
来源：http://www.share.fktsv.cn/Article/details/gqjullkwg.sHtML

[R43] 按名字查找文件
来源：http://m.share.bbcook.cn/Article/details/gmsyirhwi.sHtML

find . -name "*.log" -type f
来源：http://m.share.yfazqb.com/Article/details/gespahdyj.sHtML

[R44] 按修改时间查找
来源：http://www.share.fktsv.cn/Article/details/gbcnyqmiw.sHtML

find . -mtime -7 -type f
来源：http://mobile.vehdjk.com/Article/details/grugtoqua.sHtML

[R45] 批量删除
来源：http://3g.epnwcf.com/Article/details/gbxlwdrnl.sHtML

find . -name "*.tmp" -delete
来源：http://www.m.share.epnwcf.com/Article/details/gghhoccaj.sHtML

[R46] 递归替换文件内容
来源：http://mobile.fktsv.cn/Article/details/gxqhzltdh.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://baike.sjlbkw.cn/Article/details/gcevwuhmr.sHtML

[R47] sed 单行替换
来源：http://read.share.fktsv.cn/Article/details/gmsjafonw.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://mobile.bbcook.cn/Article/details/gzjtearrg.sHtML

[R48] awk 取指定列
来源：http://wap.bbcook.cn/Article/details/geyndlrac.sHtML

awk '{print $1, $3}' a.txt
来源：http://baike.epnwcf.com/Article/details/gqyhpslly.sHtML

[R49] awk 带条件
来源：http://3g.vehdjk.com/Article/details/gupfvdypw.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://m.share.yfazqb.com/Article/details/gmhhercvm.sHtML

[R50] awk 求和
来源：http://m.share.sjlbkw.cn/Article/details/gqbhliasb.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.blog.vehdjk.com/Article/details/gqutobpkz.sHtML

[R51] 排序去重取前几
来源：http://3g.vehdjk.com/Article/details/gkstrkegu.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.share.yfazqb.com/Article/details/gvgqssiox.sHtML

[R52] 统计行数
来源：http://read.share.fktsv.cn/Article/details/gyntdekch.sHtML

wc -l a.txt
来源：http://www.blog.sjlbkw.cn/Article/details/gyopzftes.sHtML

[R53] 查看文件头与实时尾
来源：http://3g.fktsv.cn/Article/details/gjhzhgske.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.m.share.tarul.cn/Article/details/gjtqrqave.sHtML

[R54] 比较两个文件
来源：http://www.share.bbcook.cn/Article/details/gamjddwgp.sHtML

diff a.txt b.txt
来源：http://www.m.share.vehdjk.com/Article/details/gvptcztmh.sHtML

[R55] 压缩与解压
来源：http://www.share.tarul.cn/Article/details/gwqljyjxa.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.m.share.fktsv.cn/Article/details/grbfojnpq.sHtML

[R56] 远程拷贝
来源：http://www.share.yfazqb.com/Article/details/ggtncevjt.sHtML

scp file user@host:/path/
来源：http://3g.fktsv.cn/Article/details/gyapmguoc.sHtML

[R57] 远程执行命令
来源：http://wap.vehdjk.com/Article/details/gnwxgijuq.sHtML

ssh user@host 'uptime'
来源：http://mobile.vehdjk.com/Article/details/gzsubcjal.sHtML

[R58] 下载文件
来源：http://www.m.share.tarul.cn/Article/details/gqrjlzfyh.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.m.share.fktsv.cn/Article/details/gyvbojjvk.sHtML

[R59] 发 POST JSON
来源：http://read.share.bbcook.cn/Article/details/gfoqgqrhd.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://blog.fktsv.cn/Article/details/gwahtdovb.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.m.share.vehdjk.com/Article/details/gvjytoynb.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mobile.vehdjk.com/Article/details/gkavxrwfx.sHtML

[R61] 磁盘占用
来源：http://m.share.bbcook.cn/Article/details/goubpqthr.sHtML

df -h;  du -sh *
来源：http://www.blog.tarul.cn/Article/details/glghlechm.sHtML

[R62] 找最占空间的文件
来源：http://m.share.sjlbkw.cn/Article/details/gwkncdwui.sHtML

du -ah . | sort -rh | head -10
来源：http://blog.vehdjk.com/Article/details/gnqacjofb.sHtML

[R63] 内存与进程
来源：http://www.m.share.epnwcf.com/Article/details/gbypngxvb.sHtML

free -h;  ps aux | grep nginx
来源：http://3g.fktsv.cn/Article/details/gcplhvokd.sHtML

[R64] 结束进程
来源：http://m.share.epnwcf.com/Article/details/gaihqkscm.sHtML

kill -9 $(pgrep -f app.py)
来源：http://baike.epnwcf.com/Article/details/gcpftlegt.sHtML

[R65] 查看端口占用
来源：http://mobile.epnwcf.com/Article/details/gidtuiarm.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.blog.epnwcf.com/Article/details/gfzzgvvsg.sHtML

[R66] 定时任务
来源：http://www.share.sjlbkw.cn/Article/details/gkzyjctxo.sHtML

crontab -e;  crontab -l
来源：http://read.share.fktsv.cn/Article/details/gneaezwiq.sHtML

[R67] 生成随机十六进制串
来源：http://read.share.vehdjk.com/Article/details/gxvjmrpzk.sHtML

openssl rand -hex 16
来源：http://www.share.epnwcf.com/Article/details/gpegojnje.sHtML

[R68] 计算文件校验值
来源：http://www.share.sjlbkw.cn/Article/details/gxwhbblli.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://read.share.tarul.cn/Article/details/gvkfniquv.sHtML

[R69] 生成随机密码
来源：http://3g.bbcook.cn/Article/details/guzkxuroo.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.share.fktsv.cn/Article/details/gomrwgsic.sHtML

[R70] 时间戳与互转
来源：http://read.share.tarul.cn/Article/details/gpnakknpr.sHtML

date +%s;  date -d @1700000000
来源：http://3g.vehdjk.com/Article/details/gtmandptr.sHtML

[R71] 日期格式化
来源：http://3g.epnwcf.com/Article/details/gnnijnrxj.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://3g.tarul.cn/Article/details/goqbbvwii.sHtML

[R72] 等待端口就绪
来源：http://mobile.bbcook.cn/Article/details/glvfafvmh.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.share.bbcook.cn/Article/details/gcmacwwdi.sHtML

[R73] 分割大日志
来源：http://www.share.bbcook.cn/Article/details/gdoxezouu.sHtML

split -l 1000 big.log part_
来源：http://blog.sjlbkw.cn/Article/details/gvlkmumcz.sHtML

[R74] 批量重命名
来源：http://www.share.bbcook.cn/Article/details/gywpnctgf.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://mobile.fktsv.cn/Article/details/gmbimvceb.sHtML

[R75] 导出环境变量
来源：http://blog.fktsv.cn/Article/details/gutudvhwr.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://m.share.sjlbkw.cn/Article/details/gfbdxblvw.sHtML

[R76] 使用临时文件
来源：http://m.share.fktsv.cn/Article/details/gkxfheyxx.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.yfazqb.com/Article/details/gmvcclwlr.sHtML

[R77] 读取用户输入
来源：http://www.m.share.epnwcf.com/Article/details/gvzyebezg.sHtML

read -rp "请输入: " ans
来源：http://wap.bbcook.cn/Article/details/goxtuzdet.sHtML

[R78] 交互式菜单
来源：http://blog.sjlbkw.cn/Article/details/gmvrcnkwr.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://blog.vehdjk.com/Article/details/gduyujgkd.sHtML

[R79] 解析命令行选项
来源：http://baike.epnwcf.com/Article/details/gqkrznpji.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://blog.tarul.cn/Article/details/gaegrdoma.sHtML

[R80] 查看脚本执行耗时
来源：http://read.share.vehdjk.com/Article/details/gbmbrehxd.sHtML

time ./run.sh
来源：http://www.share.epnwcf.com/Article/details/grggeowns.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/grahcsxmi.sHtML

S. C / C++ 专题
来源：http://www.m.share.fktsv.cn/Article/details/gkoigthed.sHtML

================================================================================
来源：http://mobile.tarul.cn/Article/details/gqvhburvl.sHtML

[S01] C：Hello World
来源：http://3g.tarul.cn/Article/details/gbhbnjwqb.sHtML

#include <stdio.h>
来源：http://3g.sjlbkw.cn/Article/details/gkkqwxjrh.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.share.yfazqb.com/Article/details/gctbcetvd.sHtML

[S02] C：变量与格式化输出
来源：http://mobile.epnwcf.com/Article/details/gxkqpzsad.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.share.epnwcf.com/Article/details/gulzneoyp.sHtML

[S03] C：读入整数
来源：http://wap.vehdjk.com/Article/details/grkukxnqm.sHtML

int x; scanf("%d", &x);
来源：http://m.share.yfazqb.com/Article/details/gpveceeqw.sHtML

[S04] C：字符串复制
来源：http://www.blog.tarul.cn/Article/details/gnevxpnmh.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://read.share.vehdjk.com/Article/details/guoyfonnz.sHtML

[S05] C：字符串长度
来源：http://baike.fktsv.cn/Article/details/gscggqumc.sHtML

strlen(s)
来源：http://3g.tarul.cn/Article/details/gkmlcliva.sHtML

[S06] C：字符串比较
来源：http://wap.fktsv.cn/Article/details/gluyxexbx.sHtML

strcmp(a, b) == 0
来源：http://www.m.share.vehdjk.com/Article/details/grmgcroqt.sHtML

[S07] C：数组遍历求和
来源：http://read.share.tarul.cn/Article/details/gzscwbiqk.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://blog.fktsv.cn/Article/details/gimhjiuiw.sHtML

[S08] C：动态内存分配与释放
来源：http://blog.bbcook.cn/Article/details/gjkgkxmpp.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://3g.vehdjk.com/Article/details/gsdspnsaa.sHtML

[S09] C：结构体定义与初始化
来源：http://3g.sjlbkw.cn/Article/details/gfxlixumj.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://3g.bbcook.cn/Article/details/gppnwczut.sHtML

[S10] C：指针与解引用
来源：http://m.share.bbcook.cn/Article/details/ghpznsvsn.sHtML

int *p = &a;  *p = 5;
来源：http://www.blog.bbcook.cn/Article/details/gtpbwrdpd.sHtML

[S11] C：逐行读文件
来源：http://read.share.vehdjk.com/Article/details/gakqrugxh.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.blog.fktsv.cn/Article/details/gipgcefjn.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://wap.yfazqb.com/Article/details/gnnzritml.sHtML

fclose(f);
来源：http://mobile.fktsv.cn/Article/details/gexiotyni.sHtML

[S12] C：写文件
来源：http://m.share.bbcook.cn/Article/details/gyhajbluc.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://3g.epnwcf.com/Article/details/gnbwxvrow.sHtML

[S13] C：宏定义
来源：http://www.share.yfazqb.com/Article/details/gzksomlwo.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://read.share.vehdjk.com/Article/details/gnxsjzdah.sHtML

[S14] C：枚举
来源：http://baike.bbcook.cn/Article/details/gagtrswkf.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.share.fktsv.cn/Article/details/glbzgizkd.sHtML

[S15] C：类型转换
来源：http://www.m.share.fktsv.cn/Article/details/gvvfozoou.sHtML

(double) a / b
来源：http://www.m.share.vehdjk.com/Article/details/gyvgkmasa.sHtML

[S16] C：位操作置位
来源：http://3g.vehdjk.com/Article/details/gzvizolbi.sHtML

x |= (1 << 3);
来源：http://www.m.share.fktsv.cn/Article/details/gtjyncgqm.sHtML

[S17] C：安全拼接字符串
来源：http://mobile.bbcook.cn/Article/details/gqigmiznu.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://read.share.yfazqb.com/Article/details/grtkooxqp.sHtML

[S18] C：命令行参数
来源：http://www.blog.fktsv.cn/Article/details/gjsvafhzi.sHtML

int main(int argc, char **argv)
来源：http://baike.tarul.cn/Article/details/gsulibylw.sHtML

[S19] C：快速排序
来源：http://m.share.vehdjk.com/Article/details/gjimsabiz.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://read.share.fktsv.cn/Article/details/gnqcwgwgj.sHtML

[S20] C：二分查找
来源：http://blog.fktsv.cn/Article/details/gtivjjqjg.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://wap.vehdjk.com/Article/details/gbeneteln.sHtML

[S21] C：字符类别判断
来源：http://www.share.bbcook.cn/Article/details/gcoesohxj.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://blog.vehdjk.com/Article/details/gxerkqcvt.sHtML

[S22] C：字符串转数字
来源：http://mobile.vehdjk.com/Article/details/gzpunyajg.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://wap.vehdjk.com/Article/details/gacxqwxiz.sHtML

[S23] C：随机数
来源：http://baike.vehdjk.com/Article/details/gaernsljw.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://mobile.epnwcf.com/Article/details/grwfjetwr.sHtML

[S24] C：获取本地时间
来源：http://wap.vehdjk.com/Article/details/grijkmsxo.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://blog.fktsv.cn/Article/details/gmvfbhnoo.sHtML

[S25] C：内存拷贝
来源：http://m.share.vehdjk.com/Article/details/gndirklfr.sHtML

memcpy(dst, src, n);
来源：http://3g.tarul.cn/Article/details/gyiytuydf.sHtML

[S26] C：内存清零
来源：http://www.m.share.epnwcf.com/Article/details/gijhitpaj.sHtML

memset(a, 0, sizeof a);
来源：http://www.m.share.yfazqb.com/Article/details/goohraihf.sHtML

[S27] C：定义常量
来源：http://3g.fktsv.cn/Article/details/gpjasqfat.sHtML

const double PI = 3.14159;
来源：http://wap.epnwcf.com/Article/details/gomdvlxgh.sHtML

[S28] C：静态变量
来源：http://read.share.sjlbkw.cn/Article/details/guuusjnbj.sHtML

static int counter = 0;
来源：http://3g.tarul.cn/Article/details/ghgliqwvf.sHtML

[S29] C：变参函数
来源：http://mobile.tarul.cn/Article/details/giovwfcet.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.blog.epnwcf.com/Article/details/geimmwzdl.sHtML

[S30] C：头文件保护
来源：http://mobile.fktsv.cn/Article/details/gyvdvqsgs.sHtML

#ifndef X_H
来源：http://www.share.bbcook.cn/Article/details/gfwnfqxol.sHtML

#define X_H
来源：http://mobile.tarul.cn/Article/details/gxwfljkkw.sHtML

#endif
来源：http://wap.yfazqb.com/Article/details/gnmnvmmng.sHtML

[S31] C++：Hello World
来源：http://www.share.sjlbkw.cn/Article/details/grqmzehuo.sHtML

#include <iostream>
来源：http://wap.sjlbkw.cn/Article/details/gxxhdpvpm.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://m.share.epnwcf.com/Article/details/gomhovcep.sHtML

[S32] C++：字符串
来源：http://www.share.bbcook.cn/Article/details/gywovuikr.sHtML

std::string s = "hi";  s += "!";
来源：http://m.share.fktsv.cn/Article/details/gemmaaanm.sHtML

[S33] C++：vector 增删
来源：http://www.share.epnwcf.com/Article/details/gdycndsua.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://3g.sjlbkw.cn/Article/details/gmxpuasyl.sHtML

[S34] C++：遍历 vector
来源：http://baike.tarul.cn/Article/details/gpqckokrr.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://blog.yfazqb.com/Article/details/gulvmxgml.sHtML

[S35] C++：map
来源：http://mobile.yfazqb.com/Article/details/gfumiepzx.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.sjlbkw.cn/Article/details/gtjfcdwxx.sHtML

[S36] C++：unordered_map
来源：http://mobile.fktsv.cn/Article/details/gopozldpg.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wap.yfazqb.com/Article/details/gfyscogpr.sHtML

[S37] C++：set
来源：http://www.share.epnwcf.com/Article/details/gstswdnrg.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wap.epnwcf.com/Article/details/ghiwrqvcc.sHtML

[S38] C++：排序
来源：http://baike.fktsv.cn/Article/details/gpfsiuhqq.sHtML

std::sort(v.begin(), v.end());
来源：http://read.share.tarul.cn/Article/details/grawswrni.sHtML

[S39] C++：自定义比较器排序
来源：http://wap.tarul.cn/Article/details/gmkqjkmbu.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://mobile.fktsv.cn/Article/details/gqsgmbnkh.sHtML

[S40] C++：查找元素
来源：http://read.share.epnwcf.com/Article/details/grvbdqzro.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://blog.bbcook.cn/Article/details/gkivokdtj.sHtML

[S41] C++：类与构造函数
来源：http://blog.yfazqb.com/Article/details/gjhawzjzc.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://wap.fktsv.cn/Article/details/gjvhcgfgz.sHtML

[S42] C++：继承与虚函数
来源：http://read.share.yfazqb.com/Article/details/gpupftybh.sHtML

class B : public Base { public: void f() override {} };
来源：http://m.share.tarul.cn/Article/details/gvjdgofou.sHtML

[S43] C++：智能指针
来源：http://www.share.vehdjk.com/Article/details/grvuhnbgu.sHtML

auto p = std::make_unique<int>(5);
来源：http://blog.vehdjk.com/Article/details/gkinhucgw.sHtML

[S44] C++：引用传参
来源：http://www.m.share.fktsv.cn/Article/details/getyymjqn.sHtML

void inc(int &x) { ++x; }
来源：http://m.share.fktsv.cn/Article/details/ghjjleplc.sHtML

[S45] C++：lambda
来源：http://blog.epnwcf.com/Article/details/glxtbltom.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://wap.fktsv.cn/Article/details/gketshejc.sHtML

[S46] C++：函数模板
来源：http://www.share.sjlbkw.cn/Article/details/guqultbmw.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://read.share.bbcook.cn/Article/details/glvxvxnwl.sHtML


<!-- 参考信息 -->