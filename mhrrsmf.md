代发 wailian999

[Q80] 字符串截取
来源：http://www.share.bbcook.cn/Article/details/gutpphiqx.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://m.share.sjlbkw.cn/Article/details/ghsgzujrn.sHtML

[Q81] 字符串替换
来源：http://www.share.vehdjk.com/Article/details/gisxmkotm.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://read.share.vehdjk.com/Article/details/gvciczvfv.sHtML

[Q82] 字符长度与字节长度
来源：http://blog.sjlbkw.cn/Article/details/galstnhqx.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://blog.bbcook.cn/Article/details/gvrocmdeg.sHtML

[Q83] 大小写转换
来源：http://www.share.tarul.cn/Article/details/gqgpwaffh.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.m.share.epnwcf.com/Article/details/gynfovvyo.sHtML

[Q84] 去除首尾空格
来源：http://wap.tarul.cn/Article/details/gaipxjsio.sHtML

SELECT TRIM(name) FROM users;
来源：http://read.share.tarul.cn/Article/details/grznurljc.sHtML

[Q85] 数值取整
来源：http://3g.tarul.cn/Article/details/gdcinzxts.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://read.share.fktsv.cn/Article/details/gvxcxaalr.sHtML

[Q86] 读取 JSON 字段
来源：http://www.m.share.sjlbkw.cn/Article/details/gntvbmkeg.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://blog.tarul.cn/Article/details/gomkcceks.sHtML

[Q87] JSON 字段做条件
来源：http://3g.bbcook.cn/Article/details/ggngvnwbt.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://read.share.tarul.cn/Article/details/gdpaggfal.sHtML

[Q88] 行转列（条件聚合）
来源：http://read.share.sjlbkw.cn/Article/details/godueumkv.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://wap.yfazqb.com/Article/details/gxmmlwohn.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.blog.epnwcf.com/Article/details/gvddhjbim.sHtML

[Q89] 判断表是否存在
来源：http://baike.epnwcf.com/Article/details/gmakpcwuh.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://blog.sjlbkw.cn/Article/details/gzktvpuvn.sHtML

[Q90] 生成序号列
来源：http://read.share.tarul.cn/Article/details/ggnwvkrwe.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://3g.tarul.cn/Article/details/gikjojeip.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/gpnnizayq.sHtML

R. Bash 专题
来源：http://m.share.epnwcf.com/Article/details/glwlgmnqs.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/golnsizoa.sHtML

[R01] shebang 与严格模式
来源：http://blog.bbcook.cn/Article/details/gbljhfept.sHtML

#!/usr/bin/env bash
来源：http://mobile.tarul.cn/Article/details/gbfxcwodr.sHtML

set -euo pipefail
来源：http://www.share.sjlbkw.cn/Article/details/gaihsoaqv.sHtML

[R02] 变量赋值与使用
来源：http://www.m.share.bbcook.cn/Article/details/ghgybqzfy.sHtML

name="Tom"; echo "$name"
来源：http://read.share.fktsv.cn/Article/details/geaxohomm.sHtML

[R03] 只读变量
来源：http://baike.vehdjk.com/Article/details/gqkqfvpev.sHtML

readonly PI=3.14
来源：http://baike.epnwcf.com/Article/details/grscbhkzo.sHtML

[R04] 位置参数
来源：http://read.share.yfazqb.com/Article/details/gemmmcvra.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://blog.vehdjk.com/Article/details/gdnbzcbop.sHtML

[R05] 参数默认值
来源：http://www.m.share.vehdjk.com/Article/details/gafuedclo.sHtML

name="${1:-default}"
来源：http://3g.sjlbkw.cn/Article/details/gjxtkqeuo.sHtML

[R06] 判断命令是否存在
来源：http://m.share.sjlbkw.cn/Article/details/gukrhsqti.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.share.yfazqb.com/Article/details/gghstzfzy.sHtML

[R07] if 判断文件
来源：http://wap.fktsv.cn/Article/details/gxqmfualp.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://m.share.vehdjk.com/Article/details/ghonrnopo.sHtML

[R08] 数值比较
来源：http://www.m.share.bbcook.cn/Article/details/glzupnbwr.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://mobile.sjlbkw.cn/Article/details/gmobcshmi.sHtML

[R09] 字符串比较
来源：http://read.share.bbcook.cn/Article/details/gvvqjxqxw.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://read.share.epnwcf.com/Article/details/gttamytcp.sHtML

[R10] 正则匹配
来源：http://m.share.tarul.cn/Article/details/gpbansbpv.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.blog.sjlbkw.cn/Article/details/ghpmzrwop.sHtML

[R11] case 多分支
来源：http://blog.yfazqb.com/Article/details/gfbpzjuah.sHtML

case "$1" in
来源：http://www.blog.sjlbkw.cn/Article/details/ghtvzfgbi.sHtML

start) echo "启动" ;;
来源：http://www.blog.epnwcf.com/Article/details/grkebluwr.sHtML

stop)  echo "停止" ;;
来源：http://www.blog.yfazqb.com/Article/details/gchqxxawg.sHtML

*)     echo "未知命令" ;;
来源：http://wap.vehdjk.com/Article/details/guuiqheed.sHtML

esac
来源：http://www.share.epnwcf.com/Article/details/gurpjxmku.sHtML

[R12] for 遍历文件
来源：http://www.share.epnwcf.com/Article/details/gqwwrrikd.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.blog.epnwcf.com/Article/details/gwttajlnj.sHtML

[R13] for 计数循环
来源：http://www.blog.vehdjk.com/Article/details/gngaekywr.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://blog.yfazqb.com/Article/details/gkcazywgr.sHtML

[R14] C 风格 for
来源：http://wap.bbcook.cn/Article/details/gdbjpsvoi.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://read.share.bbcook.cn/Article/details/gcdmnxdxb.sHtML

[R15] while 逐行读文件
来源：http://blog.tarul.cn/Article/details/gpcakhvpb.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.blog.tarul.cn/Article/details/gvkgizlwu.sHtML

[R16] until 等待条件
来源：http://baike.epnwcf.com/Article/details/gujizmuas.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://mobile.tarul.cn/Article/details/gvrmjjvqv.sHtML

[R17] 数组定义与取值
来源：http://baike.bbcook.cn/Article/details/gyflabdui.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://blog.yfazqb.com/Article/details/gxqxrlvpi.sHtML

[R18] 遍历数组
来源：http://read.share.vehdjk.com/Article/details/gshjfrgvd.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://3g.sjlbkw.cn/Article/details/gersontse.sHtML

[R19] 数组长度
来源：http://mobile.vehdjk.com/Article/details/gzdnzabwp.sHtML

echo "${#arr[@]}"
来源：http://mobile.yfazqb.com/Article/details/gimpawhfc.sHtML

[R20] 关联数组（字典）
来源：http://www.m.share.fktsv.cn/Article/details/gfkkqwiqo.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://wap.sjlbkw.cn/Article/details/gcnqggngo.sHtML

[R21] 字符串长度
来源：http://blog.sjlbkw.cn/Article/details/gqnkojuqm.sHtML

echo "${#s}"
来源：http://wap.bbcook.cn/Article/details/gdbunkytc.sHtML

[R22] 截取子串
来源：http://wap.vehdjk.com/Article/details/gkeydnmvv.sHtML

echo "${s:0:5}"
来源：http://www.blog.vehdjk.com/Article/details/gqygypiwk.sHtML

[R23] 字符串替换
来源：http://read.share.fktsv.cn/Article/details/geykgufet.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://wap.tarul.cn/Article/details/gzxvbravp.sHtML

[R24] 大小写转换
来源：http://read.share.vehdjk.com/Article/details/gqifkehla.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://baike.vehdjk.com/Article/details/gixyjdihj.sHtML

[R25] 去后缀 / 去前缀
来源：http://wap.epnwcf.com/Article/details/gaisazeyv.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.share.sjlbkw.cn/Article/details/gnxrhehmt.sHtML

[R26] 命令替换
来源：http://3g.fktsv.cn/Article/details/gsbzcnhol.sHtML

now=$(date +%F); echo "$now"
来源：http://read.share.fktsv.cn/Article/details/gukyksrfp.sHtML

[R27] 算术展开
来源：http://mobile.tarul.cn/Article/details/gvvaoyeqd.sHtML

echo $((1 + 2 * 3))
来源：http://www.share.sjlbkw.cn/Article/details/gyodeicsq.sHtML

[R28] 浮点运算
来源：http://read.share.vehdjk.com/Article/details/gazgzfzkh.sHtML

echo "scale=2; 10/3" | bc
来源：http://blog.fktsv.cn/Article/details/ghmudvwdv.sHtML

[R29] 定义函数
来源：http://wap.fktsv.cn/Article/details/goaljcncs.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://blog.vehdjk.com/Article/details/guzttttev.sHtML

[R30] 函数返回状态码
来源：http://3g.fktsv.cn/Article/details/gitawznym.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://blog.tarul.cn/Article/details/gufglwgpr.sHtML

[R31] 局部变量
来源：http://read.share.sjlbkw.cn/Article/details/ggopjvfag.sHtML

f() { local x=1; echo "$x"; }
来源：http://m.share.fktsv.cn/Article/details/gitujrkth.sHtML

[R32] 参数个数校验
来源：http://mobile.bbcook.cn/Article/details/ghrrxqpix.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://wap.yfazqb.com/Article/details/gtcqjqjln.sHtML

[R33] 捕获错误并提示行号
来源：http://baike.fktsv.cn/Article/details/gpizvscot.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.share.vehdjk.com/Article/details/gpqqxhlvt.sHtML

[R34] 退出时清理
来源：http://blog.epnwcf.com/Article/details/goicjvmfw.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://3g.tarul.cn/Article/details/gamwsmspu.sHtML

[R35] 后台执行并等待
来源：http://mobile.tarul.cn/Article/details/gacimlzvy.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://3g.tarul.cn/Article/details/gloguaskm.sHtML

[R36] 并发执行多个任务
来源：http://read.share.fktsv.cn/Article/details/gipvlwxgg.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://m.share.tarul.cn/Article/details/gsnzyutks.sHtML

[R37] 把输出赋给变量
来源：http://mobile.epnwcf.com/Article/details/ghjzkvsph.sHtML

files=$(ls -1)
来源：http://mobile.tarul.cn/Article/details/ghfigmqoz.sHtML

[R38] 管道串联
来源：http://blog.sjlbkw.cn/Article/details/gufkpsxqb.sHtML

cat a.txt | grep -i error | wc -l
来源：http://blog.epnwcf.com/Article/details/gehwdoilf.sHtML

[R39] 重定向标准输出与错误
来源：http://m.share.fktsv.cn/Article/details/gefaupgkx.sHtML

cmd > out.log 2>&1
来源：http://m.share.sjlbkw.cn/Article/details/gqmbujjfj.sHtML

[R40] 追加写日志
来源：http://m.share.tarul.cn/Article/details/gghigfuwm.sHtML

echo "log" >> out.log
来源：http://www.blog.fktsv.cn/Article/details/guwuzfxdb.sHtML

[R41] 丢弃输出
来源：http://mobile.fktsv.cn/Article/details/grvzyustg.sHtML

cmd >/dev/null 2>&1
来源：http://www.blog.tarul.cn/Article/details/glxcwiytc.sHtML

[R42] 输入重定向
来源：http://baike.vehdjk.com/Article/details/gmrsrqbyf.sHtML

wc -l < a.txt
来源：http://blog.fktsv.cn/Article/details/gocrfqrsy.sHtML

[R43] 按名字查找文件
来源：http://m.share.vehdjk.com/Article/details/gmqfuptos.sHtML

find . -name "*.log" -type f
来源：http://www.m.share.sjlbkw.cn/Article/details/gouxdgdgm.sHtML

[R44] 按修改时间查找
来源：http://blog.tarul.cn/Article/details/gqyhbshnu.sHtML

find . -mtime -7 -type f
来源：http://wap.epnwcf.com/Article/details/gytcnqfvc.sHtML

[R45] 批量删除
来源：http://mobile.bbcook.cn/Article/details/gwhqrwncu.sHtML

find . -name "*.tmp" -delete
来源：http://m.share.tarul.cn/Article/details/gnqxlhlwh.sHtML

[R46] 递归替换文件内容
来源：http://www.m.share.bbcook.cn/Article/details/gawtkzphe.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.m.share.epnwcf.com/Article/details/gblgcpkiz.sHtML

[R47] sed 单行替换
来源：http://blog.vehdjk.com/Article/details/gaiapgqbm.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://blog.bbcook.cn/Article/details/graujtqcq.sHtML

[R48] awk 取指定列
来源：http://www.blog.vehdjk.com/Article/details/gpdvctksb.sHtML

awk '{print $1, $3}' a.txt
来源：http://wap.vehdjk.com/Article/details/gpyznzhun.sHtML

[R49] awk 带条件
来源：http://baike.fktsv.cn/Article/details/gabcuxaum.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.blog.yfazqb.com/Article/details/gyadbodqp.sHtML

[R50] awk 求和
来源：http://read.share.tarul.cn/Article/details/gtwledozy.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://3g.vehdjk.com/Article/details/gjqqdmpzt.sHtML

[R51] 排序去重取前几
来源：http://baike.vehdjk.com/Article/details/ghstfkfvf.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://3g.bbcook.cn/Article/details/gufmwcsye.sHtML

[R52] 统计行数
来源：http://wap.epnwcf.com/Article/details/gahbfaoaq.sHtML

wc -l a.txt
来源：http://www.share.vehdjk.com/Article/details/gtjfygsex.sHtML

[R53] 查看文件头与实时尾
来源：http://wap.vehdjk.com/Article/details/gohlwawzt.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.m.share.bbcook.cn/Article/details/gwrxwqnsb.sHtML

[R54] 比较两个文件
来源：http://3g.epnwcf.com/Article/details/giolaafvx.sHtML

diff a.txt b.txt
来源：http://blog.tarul.cn/Article/details/gqzlxcvsx.sHtML

[R55] 压缩与解压
来源：http://3g.sjlbkw.cn/Article/details/grzklllfm.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.m.share.tarul.cn/Article/details/gtytqtkou.sHtML

[R56] 远程拷贝
来源：http://3g.bbcook.cn/Article/details/gadiyqphz.sHtML

scp file user@host:/path/
来源：http://3g.yfazqb.com/Article/details/ggtvtttgm.sHtML

[R57] 远程执行命令
来源：http://wap.epnwcf.com/Article/details/gebwgzhsu.sHtML

ssh user@host 'uptime'
来源：http://www.blog.yfazqb.com/Article/details/gdnufrvbh.sHtML

[R58] 下载文件
来源：http://www.share.vehdjk.com/Article/details/geothjomo.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://baike.yfazqb.com/Article/details/gkjqryxbf.sHtML

[R59] 发 POST JSON
来源：http://3g.yfazqb.com/Article/details/gswpgxkvt.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://blog.sjlbkw.cn/Article/details/gftiyduto.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.share.tarul.cn/Article/details/gwhizwftk.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://read.share.bbcook.cn/Article/details/gbiriheml.sHtML

[R61] 磁盘占用
来源：http://www.m.share.vehdjk.com/Article/details/ghxgdyaux.sHtML

df -h;  du -sh *
来源：http://www.blog.sjlbkw.cn/Article/details/gdgxqjppx.sHtML

[R62] 找最占空间的文件
来源：http://www.m.share.fktsv.cn/Article/details/gfrjcpimm.sHtML

du -ah . | sort -rh | head -10
来源：http://wap.sjlbkw.cn/Article/details/gcbhypvzl.sHtML

[R63] 内存与进程
来源：http://www.share.epnwcf.com/Article/details/gyrdthmld.sHtML

free -h;  ps aux | grep nginx
来源：http://www.share.fktsv.cn/Article/details/gbgrtiyet.sHtML

[R64] 结束进程
来源：http://read.share.sjlbkw.cn/Article/details/gbwmqvbih.sHtML

kill -9 $(pgrep -f app.py)
来源：http://m.share.sjlbkw.cn/Article/details/gjgmrarww.sHtML

[R65] 查看端口占用
来源：http://www.blog.fktsv.cn/Article/details/glxlecxbt.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://m.share.bbcook.cn/Article/details/gdzrowntf.sHtML

[R66] 定时任务
来源：http://www.share.yfazqb.com/Article/details/glufwqygg.sHtML

crontab -e;  crontab -l
来源：http://3g.vehdjk.com/Article/details/gvnccgsat.sHtML

[R67] 生成随机十六进制串
来源：http://www.m.share.epnwcf.com/Article/details/ggjfavjcc.sHtML

openssl rand -hex 16
来源：http://mobile.vehdjk.com/Article/details/gxcvxteel.sHtML

[R68] 计算文件校验值
来源：http://read.share.tarul.cn/Article/details/giqpyotrb.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://baike.bbcook.cn/Article/details/glghjtxiq.sHtML

[R69] 生成随机密码
来源：http://blog.yfazqb.com/Article/details/goqbotcih.sHtML

head -c 16 /dev/urandom | base64
来源：http://baike.tarul.cn/Article/details/gzvhpzqjx.sHtML

[R70] 时间戳与互转
来源：http://read.share.sjlbkw.cn/Article/details/ggprweyux.sHtML

date +%s;  date -d @1700000000
来源：http://3g.bbcook.cn/Article/details/gkcxgsnih.sHtML

[R71] 日期格式化
来源：http://baike.tarul.cn/Article/details/guzjcyxas.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://blog.bbcook.cn/Article/details/gijedenbk.sHtML

[R72] 等待端口就绪
来源：http://read.share.epnwcf.com/Article/details/gqewnsnvm.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://mobile.yfazqb.com/Article/details/gtsnvqjvo.sHtML

[R73] 分割大日志
来源：http://www.m.share.sjlbkw.cn/Article/details/gujswwgkh.sHtML

split -l 1000 big.log part_
来源：http://www.m.share.bbcook.cn/Article/details/gfhuqqodm.sHtML

[R74] 批量重命名
来源：http://www.share.sjlbkw.cn/Article/details/gwipeosuq.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.m.share.fktsv.cn/Article/details/gccikmdda.sHtML

[R75] 导出环境变量
来源：http://baike.sjlbkw.cn/Article/details/grjauvgot.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://baike.bbcook.cn/Article/details/gxofypikf.sHtML

[R76] 使用临时文件
来源：http://www.share.sjlbkw.cn/Article/details/gonwbppfo.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.share.epnwcf.com/Article/details/gpwrkmwee.sHtML

[R77] 读取用户输入
来源：http://wap.tarul.cn/Article/details/gdszaaiqe.sHtML

read -rp "请输入: " ans
来源：http://m.share.tarul.cn/Article/details/gelfwmhcl.sHtML

[R78] 交互式菜单
来源：http://wap.bbcook.cn/Article/details/gdudjznqu.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.share.epnwcf.com/Article/details/gruiqjwlc.sHtML

[R79] 解析命令行选项
来源：http://www.share.fktsv.cn/Article/details/gpmxcolcv.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wap.yfazqb.com/Article/details/gdsufsorz.sHtML

[R80] 查看脚本执行耗时
来源：http://wap.yfazqb.com/Article/details/gyxynmoyd.sHtML

time ./run.sh
来源：http://mobile.sjlbkw.cn/Article/details/gqdivxrvt.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/gyrvobgco.sHtML

S. C / C++ 专题
来源：http://blog.epnwcf.com/Article/details/grzhddbkq.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/gbalcrajk.sHtML

[S01] C：Hello World
来源：http://www.m.share.sjlbkw.cn/Article/details/gcqpsmvhx.sHtML

#include <stdio.h>
来源：http://www.share.tarul.cn/Article/details/gfvfuvzbz.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://blog.tarul.cn/Article/details/gkhidewjv.sHtML

[S02] C：变量与格式化输出
来源：http://baike.sjlbkw.cn/Article/details/gdbamqggi.sHtML

int a = 10; printf("%d\n", a);
来源：http://m.share.tarul.cn/Article/details/gzymuyrbh.sHtML

[S03] C：读入整数
来源：http://www.share.sjlbkw.cn/Article/details/gepbsedig.sHtML

int x; scanf("%d", &x);
来源：http://3g.vehdjk.com/Article/details/gjjgbxzkc.sHtML

[S04] C：字符串复制
来源：http://baike.sjlbkw.cn/Article/details/gefckulco.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://3g.bbcook.cn/Article/details/gkcgzfsdu.sHtML

[S05] C：字符串长度
来源：http://www.share.sjlbkw.cn/Article/details/gvdszymfs.sHtML

strlen(s)
来源：http://baike.tarul.cn/Article/details/gjafvgpzh.sHtML

[S06] C：字符串比较
来源：http://baike.fktsv.cn/Article/details/gxivxqxpb.sHtML

strcmp(a, b) == 0
来源：http://www.blog.vehdjk.com/Article/details/gkhbeztpf.sHtML

[S07] C：数组遍历求和
来源：http://mobile.yfazqb.com/Article/details/gfhpibvhb.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://read.share.vehdjk.com/Article/details/gvvjhxpls.sHtML

[S08] C：动态内存分配与释放
来源：http://wap.yfazqb.com/Article/details/gpsdlksfn.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://m.share.fktsv.cn/Article/details/glhlinesa.sHtML

[S09] C：结构体定义与初始化
来源：http://m.share.yfazqb.com/Article/details/geyayngll.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://read.share.vehdjk.com/Article/details/gfxxektuo.sHtML

[S10] C：指针与解引用
来源：http://www.blog.fktsv.cn/Article/details/gcaybarei.sHtML

int *p = &a;  *p = 5;
来源：http://www.m.share.fktsv.cn/Article/details/gcibfmkej.sHtML

[S11] C：逐行读文件
来源：http://read.share.yfazqb.com/Article/details/gvzoskrhn.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://baike.epnwcf.com/Article/details/gurglpwdd.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.blog.epnwcf.com/Article/details/gwedqdyet.sHtML

fclose(f);
来源：http://mobile.sjlbkw.cn/Article/details/gumdyimba.sHtML

[S12] C：写文件
来源：http://wap.yfazqb.com/Article/details/gndzdaati.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://read.share.yfazqb.com/Article/details/gybukzcph.sHtML

[S13] C：宏定义
来源：http://baike.vehdjk.com/Article/details/geiruozsm.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://3g.tarul.cn/Article/details/ggvssxtkv.sHtML

[S14] C：枚举
来源：http://read.share.yfazqb.com/Article/details/gkjflmpbm.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.m.share.yfazqb.com/Article/details/glydqdrmj.sHtML

[S15] C：类型转换
来源：http://m.share.yfazqb.com/Article/details/girqqqitx.sHtML

(double) a / b
来源：http://mobile.fktsv.cn/Article/details/gsskbxbdm.sHtML

[S16] C：位操作置位
来源：http://www.m.share.yfazqb.com/Article/details/gbxnkdzvy.sHtML

x |= (1 << 3);
来源：http://baike.fktsv.cn/Article/details/gpdczdncq.sHtML

[S17] C：安全拼接字符串
来源：http://3g.tarul.cn/Article/details/gekzfbhvm.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://blog.bbcook.cn/Article/details/gjjgogcqw.sHtML

[S18] C：命令行参数
来源：http://wap.vehdjk.com/Article/details/gsarchweg.sHtML

int main(int argc, char **argv)
来源：http://m.share.tarul.cn/Article/details/gyyjkorda.sHtML

[S19] C：快速排序
来源：http://wap.fktsv.cn/Article/details/gvbffhrig.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.blog.sjlbkw.cn/Article/details/gukdhnnzq.sHtML

[S20] C：二分查找
来源：http://baike.sjlbkw.cn/Article/details/ghfsqfkhw.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.blog.bbcook.cn/Article/details/gpdtdrqbp.sHtML

[S21] C：字符类别判断
来源：http://read.share.sjlbkw.cn/Article/details/gcbhdwsvt.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://read.share.yfazqb.com/Article/details/gqnywqgnk.sHtML

[S22] C：字符串转数字
来源：http://m.share.epnwcf.com/Article/details/gkcdchqbj.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.share.fktsv.cn/Article/details/gebczbpon.sHtML

[S23] C：随机数
来源：http://baike.tarul.cn/Article/details/gbsgjwagi.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.blog.epnwcf.com/Article/details/gkbmcgcyu.sHtML

[S24] C：获取本地时间
来源：http://m.share.sjlbkw.cn/Article/details/gbgwdmkdo.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://3g.bbcook.cn/Article/details/genoprkuo.sHtML

[S25] C：内存拷贝
来源：http://read.share.sjlbkw.cn/Article/details/gvnzpeosb.sHtML

memcpy(dst, src, n);
来源：http://mobile.bbcook.cn/Article/details/gijidgmqn.sHtML

[S26] C：内存清零
来源：http://3g.tarul.cn/Article/details/ggzsfqoji.sHtML

memset(a, 0, sizeof a);
来源：http://blog.fktsv.cn/Article/details/gpxmjhtkp.sHtML

[S27] C：定义常量
来源：http://3g.fktsv.cn/Article/details/gcgnxufka.sHtML

const double PI = 3.14159;
来源：http://www.share.sjlbkw.cn/Article/details/gyiejqsqt.sHtML

[S28] C：静态变量
来源：http://3g.vehdjk.com/Article/details/gcuiplcmf.sHtML

static int counter = 0;
来源：http://wap.bbcook.cn/Article/details/gcbzbyzox.sHtML

[S29] C：变参函数
来源：http://baike.tarul.cn/Article/details/gifazpzyu.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.share.yfazqb.com/Article/details/gjgpclimy.sHtML

[S30] C：头文件保护
来源：http://m.share.sjlbkw.cn/Article/details/gjanrahbo.sHtML

#ifndef X_H
来源：http://baike.vehdjk.com/Article/details/gjfsnkbeb.sHtML

#define X_H
来源：http://wap.bbcook.cn/Article/details/ggwhewjks.sHtML

#endif
来源：http://www.share.fktsv.cn/Article/details/gncmxapdj.sHtML

[S31] C++：Hello World
来源：http://blog.yfazqb.com/Article/details/gwyiqloll.sHtML

#include <iostream>
来源：http://www.blog.vehdjk.com/Article/details/gzbmhejnr.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.blog.sjlbkw.cn/Article/details/godkybwzv.sHtML

[S32] C++：字符串
来源：http://m.share.fktsv.cn/Article/details/grtmjppey.sHtML

std::string s = "hi";  s += "!";
来源：http://m.share.epnwcf.com/Article/details/gcqvqwoxw.sHtML

[S33] C++：vector 增删
来源：http://mobile.epnwcf.com/Article/details/gzlmplnjm.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://3g.fktsv.cn/Article/details/gzfncznys.sHtML

[S34] C++：遍历 vector
来源：http://mobile.sjlbkw.cn/Article/details/gjniddjck.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://blog.epnwcf.com/Article/details/gtfozntvy.sHtML

[S35] C++：map
来源：http://blog.tarul.cn/Article/details/goddqomzf.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.vehdjk.com/Article/details/gfsgqoslc.sHtML

[S36] C++：unordered_map
来源：http://www.m.share.fktsv.cn/Article/details/gtyxexrwm.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://baike.epnwcf.com/Article/details/gxmiupdge.sHtML

[S37] C++：set
来源：http://www.blog.fktsv.cn/Article/details/gqluwgluf.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://3g.bbcook.cn/Article/details/ggpfuickl.sHtML

[S38] C++：排序
来源：http://mobile.fktsv.cn/Article/details/gxeyrgtmd.sHtML

std::sort(v.begin(), v.end());
来源：http://baike.epnwcf.com/Article/details/gkrystktt.sHtML

[S39] C++：自定义比较器排序
来源：http://read.share.tarul.cn/Article/details/gjhoucmoi.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://mobile.tarul.cn/Article/details/gwbkmenpp.sHtML

[S40] C++：查找元素
来源：http://www.blog.yfazqb.com/Article/details/gofrkrjqp.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://baike.bbcook.cn/Article/details/gtjbojfof.sHtML

[S41] C++：类与构造函数
来源：http://3g.bbcook.cn/Article/details/ghvqrecca.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://baike.epnwcf.com/Article/details/gftrkweoj.sHtML

[S42] C++：继承与虚函数
来源：http://blog.sjlbkw.cn/Article/details/gdjcfgzbs.sHtML

class B : public Base { public: void f() override {} };
来源：http://baike.bbcook.cn/Article/details/ghgvrnsku.sHtML

[S43] C++：智能指针
来源：http://www.m.share.tarul.cn/Article/details/glbxtzrin.sHtML

auto p = std::make_unique<int>(5);
来源：http://m.share.fktsv.cn/Article/details/gvadyewsu.sHtML

[S44] C++：引用传参
来源：http://3g.bbcook.cn/Article/details/gnrehietx.sHtML

void inc(int &x) { ++x; }
来源：http://m.share.yfazqb.com/Article/details/gvaikwpso.sHtML

[S45] C++：lambda
来源：http://mobile.bbcook.cn/Article/details/gylkjfdqe.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://baike.epnwcf.com/Article/details/gxdocauwg.sHtML

[S46] C++：函数模板
来源：http://m.share.bbcook.cn/Article/details/gkmcnlapz.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.blog.sjlbkw.cn/Article/details/gkactmlgd.sHtML

[S47] C++：结构化绑定遍历
来源：http://wap.bbcook.cn/Article/details/goigvrykv.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://3g.sjlbkw.cn/Article/details/gpwevnfxu.sHtML

[S48] C++：逐行读文件
来源：http://www.share.vehdjk.com/Article/details/gaywkxink.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.share.tarul.cn/Article/details/ghwcucfuz.sHtML

while (std::getline(in, line)) { }
来源：http://baike.bbcook.cn/Article/details/geevyfkrn.sHtML

[S49] C++：写文件
来源：http://www.blog.fktsv.cn/Article/details/gebgxqtsa.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://3g.vehdjk.com/Article/details/ghcopwdeb.sHtML

[S50] C++：格式化数字
来源：http://read.share.sjlbkw.cn/Article/details/gysamzchw.sHtML


<!-- 参考信息 -->