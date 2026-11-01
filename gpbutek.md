代发 wailian999

[Q82] 字符长度与字节长度
来源：http://m.share.yfazqb.com/Article/details/gjokigmef.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://read.share.fktsv.cn/Article/details/ggidnysue.sHtML

[Q83] 大小写转换
来源：http://mobile.sjlbkw.cn/Article/details/ggyizsogp.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.m.share.yfazqb.com/Article/details/ggexmxvpj.sHtML

[Q84] 去除首尾空格
来源：http://www.m.share.vehdjk.com/Article/details/gebgwmrie.sHtML

SELECT TRIM(name) FROM users;
来源：http://wap.fktsv.cn/Article/details/gqhddrrna.sHtML

[Q85] 数值取整
来源：http://m.share.sjlbkw.cn/Article/details/gxpfpkqlm.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.share.epnwcf.com/Article/details/guwgbxsuy.sHtML

[Q86] 读取 JSON 字段
来源：http://blog.fktsv.cn/Article/details/ghscagwzs.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://wap.yfazqb.com/Article/details/gznyrdorv.sHtML

[Q87] JSON 字段做条件
来源：http://mobile.bbcook.cn/Article/details/gudajgsgf.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://blog.vehdjk.com/Article/details/ghznwvklt.sHtML

[Q88] 行转列（条件聚合）
来源：http://read.share.yfazqb.com/Article/details/gspaygmij.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://mobile.epnwcf.com/Article/details/gxaorapso.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://blog.epnwcf.com/Article/details/gqmkibatr.sHtML

[Q89] 判断表是否存在
来源：http://blog.sjlbkw.cn/Article/details/gvixdbcbk.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.m.share.vehdjk.com/Article/details/gulwknkix.sHtML

[Q90] 生成序号列
来源：http://mobile.vehdjk.com/Article/details/gazlyhujk.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://read.share.yfazqb.com/Article/details/gwgzzrcob.sHtML

================================================================================
来源：http://m.share.tarul.cn/Article/details/grgriwhtu.sHtML

R. Bash 专题
来源：http://www.share.fktsv.cn/Article/details/gxkpvymma.sHtML

================================================================================
来源：http://www.share.sjlbkw.cn/Article/details/gepbtsdbk.sHtML

[R01] shebang 与严格模式
来源：http://read.share.fktsv.cn/Article/details/gvkrzgzlg.sHtML

#!/usr/bin/env bash
来源：http://m.share.sjlbkw.cn/Article/details/gzxrhuckv.sHtML

set -euo pipefail
来源：http://baike.sjlbkw.cn/Article/details/giabpkzzx.sHtML

[R02] 变量赋值与使用
来源：http://baike.epnwcf.com/Article/details/gttizsnwc.sHtML

name="Tom"; echo "$name"
来源：http://wap.sjlbkw.cn/Article/details/gyctdufib.sHtML

[R03] 只读变量
来源：http://www.blog.vehdjk.com/Article/details/gsywbzdcu.sHtML

readonly PI=3.14
来源：http://www.m.share.sjlbkw.cn/Article/details/gcwmgwygm.sHtML

[R04] 位置参数
来源：http://www.m.share.fktsv.cn/Article/details/gwplwixzy.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://baike.fktsv.cn/Article/details/gmgfprnjd.sHtML

[R05] 参数默认值
来源：http://mobile.epnwcf.com/Article/details/gfqyrmykc.sHtML

name="${1:-default}"
来源：http://www.blog.tarul.cn/Article/details/gxgrcjlwy.sHtML

[R06] 判断命令是否存在
来源：http://www.share.sjlbkw.cn/Article/details/grosnguyj.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://blog.fktsv.cn/Article/details/gehduxqgy.sHtML

[R07] if 判断文件
来源：http://wap.sjlbkw.cn/Article/details/gcravyput.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://mobile.sjlbkw.cn/Article/details/gicnpotlo.sHtML

[R08] 数值比较
来源：http://www.m.share.vehdjk.com/Article/details/gvcqzdjbi.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://mobile.fktsv.cn/Article/details/gkgsfkqbl.sHtML

[R09] 字符串比较
来源：http://read.share.sjlbkw.cn/Article/details/gnaglfgml.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://wap.yfazqb.com/Article/details/gbeignvgj.sHtML

[R10] 正则匹配
来源：http://blog.sjlbkw.cn/Article/details/gerheiwss.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://3g.fktsv.cn/Article/details/gnlvdlhsj.sHtML

[R11] case 多分支
来源：http://mobile.vehdjk.com/Article/details/gvjgklity.sHtML

case "$1" in
来源：http://mobile.tarul.cn/Article/details/goydkgofl.sHtML

start) echo "启动" ;;
来源：http://blog.vehdjk.com/Article/details/gqtdhlzit.sHtML

stop)  echo "停止" ;;
来源：http://wap.yfazqb.com/Article/details/gvcvgkaga.sHtML

*)     echo "未知命令" ;;
来源：http://baike.sjlbkw.cn/Article/details/gsjxbwdew.sHtML

esac
来源：http://3g.fktsv.cn/Article/details/girgrtzdg.sHtML

[R12] for 遍历文件
来源：http://read.share.tarul.cn/Article/details/gbqobnfqw.sHtML

for f in *.txt; do echo "$f"; done
来源：http://3g.vehdjk.com/Article/details/gmdymhbcg.sHtML

[R13] for 计数循环
来源：http://www.m.share.tarul.cn/Article/details/gyrzmxyav.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://blog.fktsv.cn/Article/details/ghrmsysxb.sHtML

[R14] C 风格 for
来源：http://mobile.tarul.cn/Article/details/gqrmvjmjd.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://read.share.bbcook.cn/Article/details/guenorhlv.sHtML

[R15] while 逐行读文件
来源：http://baike.bbcook.cn/Article/details/gdwdjuehe.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://3g.sjlbkw.cn/Article/details/ggxqiwcsx.sHtML

[R16] until 等待条件
来源：http://m.share.sjlbkw.cn/Article/details/gvqakhsqm.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://3g.yfazqb.com/Article/details/gsbpxieno.sHtML

[R17] 数组定义与取值
来源：http://m.share.tarul.cn/Article/details/garutkwre.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://m.share.epnwcf.com/Article/details/gbwjktaju.sHtML

[R18] 遍历数组
来源：http://baike.epnwcf.com/Article/details/gqtbbddhj.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://3g.fktsv.cn/Article/details/gksyerxmg.sHtML

[R19] 数组长度
来源：http://wap.tarul.cn/Article/details/gfskhasls.sHtML

echo "${#arr[@]}"
来源：http://www.blog.tarul.cn/Article/details/gpwmcukyy.sHtML

[R20] 关联数组（字典）
来源：http://m.share.epnwcf.com/Article/details/gkfblbbuc.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://baike.vehdjk.com/Article/details/gxnjjludr.sHtML

[R21] 字符串长度
来源：http://blog.yfazqb.com/Article/details/gawpdylut.sHtML

echo "${#s}"
来源：http://baike.vehdjk.com/Article/details/gjzlaoreh.sHtML

[R22] 截取子串
来源：http://www.blog.bbcook.cn/Article/details/gkeflmamq.sHtML

echo "${s:0:5}"
来源：http://m.share.yfazqb.com/Article/details/gwvnnxiqw.sHtML

[R23] 字符串替换
来源：http://read.share.fktsv.cn/Article/details/gastmzhzl.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.share.sjlbkw.cn/Article/details/gijuhnwbw.sHtML

[R24] 大小写转换
来源：http://www.m.share.tarul.cn/Article/details/gihjpvjmi.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://3g.vehdjk.com/Article/details/gynbrsloh.sHtML

[R25] 去后缀 / 去前缀
来源：http://baike.vehdjk.com/Article/details/gkfmwutpm.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.blog.tarul.cn/Article/details/gqunzwndl.sHtML

[R26] 命令替换
来源：http://mobile.vehdjk.com/Article/details/gkqxxxqwh.sHtML

now=$(date +%F); echo "$now"
来源：http://www.blog.tarul.cn/Article/details/gcdobrmit.sHtML

[R27] 算术展开
来源：http://www.share.bbcook.cn/Article/details/grcuuhzej.sHtML

echo $((1 + 2 * 3))
来源：http://3g.tarul.cn/Article/details/garugymaq.sHtML

[R28] 浮点运算
来源：http://www.m.share.sjlbkw.cn/Article/details/gwcraohxk.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.blog.yfazqb.com/Article/details/gkjblxsex.sHtML

[R29] 定义函数
来源：http://www.share.tarul.cn/Article/details/gvcbedecv.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://mobile.yfazqb.com/Article/details/gopvzmguk.sHtML

[R30] 函数返回状态码
来源：http://blog.epnwcf.com/Article/details/gnnhudgua.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://baike.yfazqb.com/Article/details/gwpldjizq.sHtML

[R31] 局部变量
来源：http://mobile.yfazqb.com/Article/details/goqlnaugi.sHtML

f() { local x=1; echo "$x"; }
来源：http://m.share.yfazqb.com/Article/details/gyhkocoze.sHtML

[R32] 参数个数校验
来源：http://www.share.sjlbkw.cn/Article/details/gjvlrihir.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.share.tarul.cn/Article/details/grzrcbiui.sHtML

[R33] 捕获错误并提示行号
来源：http://www.share.yfazqb.com/Article/details/gsfgugakm.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.blog.epnwcf.com/Article/details/gdhzdxxhq.sHtML

[R34] 退出时清理
来源：http://mobile.fktsv.cn/Article/details/gvqzkkrdf.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://mobile.yfazqb.com/Article/details/gjpzmbbdx.sHtML

[R35] 后台执行并等待
来源：http://mobile.vehdjk.com/Article/details/gqxcybtit.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://baike.vehdjk.com/Article/details/gxqisntdj.sHtML

[R36] 并发执行多个任务
来源：http://baike.tarul.cn/Article/details/gegmbqhvd.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://blog.yfazqb.com/Article/details/gemdfklsv.sHtML

[R37] 把输出赋给变量
来源：http://baike.vehdjk.com/Article/details/ghavrifaa.sHtML

files=$(ls -1)
来源：http://blog.bbcook.cn/Article/details/gtsrzmhma.sHtML

[R38] 管道串联
来源：http://m.share.vehdjk.com/Article/details/gnszswypt.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.share.yfazqb.com/Article/details/geelmdvvg.sHtML

[R39] 重定向标准输出与错误
来源：http://3g.bbcook.cn/Article/details/giblexkbv.sHtML

cmd > out.log 2>&1
来源：http://baike.vehdjk.com/Article/details/gyphsfhcx.sHtML

[R40] 追加写日志
来源：http://3g.fktsv.cn/Article/details/gdtxccdnb.sHtML

echo "log" >> out.log
来源：http://www.m.share.tarul.cn/Article/details/giddnvmrf.sHtML

[R41] 丢弃输出
来源：http://www.blog.sjlbkw.cn/Article/details/glohqreya.sHtML

cmd >/dev/null 2>&1
来源：http://www.share.epnwcf.com/Article/details/gxdkljhqf.sHtML

[R42] 输入重定向
来源：http://m.share.bbcook.cn/Article/details/gxoichuay.sHtML

wc -l < a.txt
来源：http://wap.tarul.cn/Article/details/gawnkziqm.sHtML

[R43] 按名字查找文件
来源：http://m.share.vehdjk.com/Article/details/grqhcjexd.sHtML

find . -name "*.log" -type f
来源：http://mobile.epnwcf.com/Article/details/gprqmjsth.sHtML

[R44] 按修改时间查找
来源：http://m.share.yfazqb.com/Article/details/gasvmttrf.sHtML

find . -mtime -7 -type f
来源：http://www.m.share.epnwcf.com/Article/details/gqupofxha.sHtML

[R45] 批量删除
来源：http://3g.bbcook.cn/Article/details/gabwuhbbz.sHtML

find . -name "*.tmp" -delete
来源：http://m.share.sjlbkw.cn/Article/details/gejnnzmgr.sHtML

[R46] 递归替换文件内容
来源：http://www.share.yfazqb.com/Article/details/gfrydhfcw.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://baike.bbcook.cn/Article/details/gcvckbsyt.sHtML

[R47] sed 单行替换
来源：http://baike.epnwcf.com/Article/details/gsohvmovp.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://read.share.vehdjk.com/Article/details/gcvodurog.sHtML

[R48] awk 取指定列
来源：http://wap.sjlbkw.cn/Article/details/ggcjqnsti.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.share.tarul.cn/Article/details/ghjgjfdrl.sHtML

[R49] awk 带条件
来源：http://www.m.share.tarul.cn/Article/details/gtvdelgnu.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://read.share.tarul.cn/Article/details/glyjpjhxb.sHtML

[R50] awk 求和
来源：http://www.m.share.epnwcf.com/Article/details/gbljkkuth.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://3g.sjlbkw.cn/Article/details/gjkkdmuai.sHtML

[R51] 排序去重取前几
来源：http://baike.vehdjk.com/Article/details/ghyfgbchz.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://m.share.bbcook.cn/Article/details/gyrgxflhg.sHtML

[R52] 统计行数
来源：http://blog.sjlbkw.cn/Article/details/gnmzdvkpw.sHtML

wc -l a.txt
来源：http://www.share.vehdjk.com/Article/details/giinehdiu.sHtML

[R53] 查看文件头与实时尾
来源：http://wap.vehdjk.com/Article/details/gfirqffis.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.share.yfazqb.com/Article/details/gahloipqg.sHtML

[R54] 比较两个文件
来源：http://3g.sjlbkw.cn/Article/details/gidyimeyw.sHtML

diff a.txt b.txt
来源：http://www.blog.vehdjk.com/Article/details/gsbxhnynd.sHtML

[R55] 压缩与解压
来源：http://baike.epnwcf.com/Article/details/gkyrqinwa.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.blog.fktsv.cn/Article/details/gtlwxuzxn.sHtML

[R56] 远程拷贝
来源：http://www.m.share.vehdjk.com/Article/details/gqgjwajft.sHtML

scp file user@host:/path/
来源：http://mobile.fktsv.cn/Article/details/gfrvkrldy.sHtML

[R57] 远程执行命令
来源：http://blog.fktsv.cn/Article/details/glzlhdzly.sHtML

ssh user@host 'uptime'
来源：http://blog.fktsv.cn/Article/details/grrtlldrr.sHtML

[R58] 下载文件
来源：http://www.blog.yfazqb.com/Article/details/gleqwtajf.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://blog.epnwcf.com/Article/details/gvxwpmhot.sHtML

[R59] 发 POST JSON
来源：http://mobile.vehdjk.com/Article/details/ghvqjdlxc.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://3g.fktsv.cn/Article/details/gamjgbvar.sHtML

[R60] 只看 HTTP 状态码
来源：http://m.share.tarul.cn/Article/details/gnzryjllf.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://baike.yfazqb.com/Article/details/gubmfdmyf.sHtML

[R61] 磁盘占用
来源：http://mobile.fktsv.cn/Article/details/glatucwtf.sHtML

df -h;  du -sh *
来源：http://m.share.tarul.cn/Article/details/gkzkfxepw.sHtML

[R62] 找最占空间的文件
来源：http://www.share.vehdjk.com/Article/details/guhnmlpkt.sHtML

du -ah . | sort -rh | head -10
来源：http://mobile.tarul.cn/Article/details/grnbvcrth.sHtML

[R63] 内存与进程
来源：http://mobile.sjlbkw.cn/Article/details/gbvbwqgbp.sHtML

free -h;  ps aux | grep nginx
来源：http://3g.vehdjk.com/Article/details/grtywoshz.sHtML

[R64] 结束进程
来源：http://www.share.epnwcf.com/Article/details/guwwevxdv.sHtML

kill -9 $(pgrep -f app.py)
来源：http://mobile.yfazqb.com/Article/details/ghxsuhpdg.sHtML

[R65] 查看端口占用
来源：http://www.m.share.epnwcf.com/Article/details/gfmuziffa.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://m.share.tarul.cn/Article/details/gpgcbvoby.sHtML

[R66] 定时任务
来源：http://blog.fktsv.cn/Article/details/gtvwswsoy.sHtML

crontab -e;  crontab -l
来源：http://mobile.yfazqb.com/Article/details/grzzvvppo.sHtML

[R67] 生成随机十六进制串
来源：http://3g.tarul.cn/Article/details/gjnwgdylx.sHtML

openssl rand -hex 16
来源：http://3g.fktsv.cn/Article/details/gakqukudv.sHtML

[R68] 计算文件校验值
来源：http://m.share.sjlbkw.cn/Article/details/ggzeroftk.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.m.share.tarul.cn/Article/details/gttqweqtt.sHtML

[R69] 生成随机密码
来源：http://mobile.bbcook.cn/Article/details/gkrzqdzmn.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.blog.bbcook.cn/Article/details/gxgjfbjwz.sHtML

[R70] 时间戳与互转
来源：http://mobile.epnwcf.com/Article/details/gfhttmpgg.sHtML

date +%s;  date -d @1700000000
来源：http://wap.fktsv.cn/Article/details/girjgdgab.sHtML

[R71] 日期格式化
来源：http://read.share.epnwcf.com/Article/details/gjjetazpy.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://blog.vehdjk.com/Article/details/gcwszbftm.sHtML

[R72] 等待端口就绪
来源：http://wap.fktsv.cn/Article/details/gtchcbavq.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.share.bbcook.cn/Article/details/gfktbiuji.sHtML

[R73] 分割大日志
来源：http://m.share.tarul.cn/Article/details/geucpyvds.sHtML

split -l 1000 big.log part_
来源：http://www.blog.yfazqb.com/Article/details/gymgobvjj.sHtML

[R74] 批量重命名
来源：http://m.share.bbcook.cn/Article/details/gqybcczmd.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://3g.sjlbkw.cn/Article/details/gpidmyfmx.sHtML

[R75] 导出环境变量
来源：http://www.share.bbcook.cn/Article/details/gfonpugkl.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://m.share.tarul.cn/Article/details/gzuikqsct.sHtML

[R76] 使用临时文件
来源：http://read.share.vehdjk.com/Article/details/gxdyicdhb.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.bbcook.cn/Article/details/gsoqtstjr.sHtML

[R77] 读取用户输入
来源：http://www.blog.yfazqb.com/Article/details/gvifamxff.sHtML

read -rp "请输入: " ans
来源：http://www.m.share.fktsv.cn/Article/details/gsnwzlvvy.sHtML

[R78] 交互式菜单
来源：http://m.share.bbcook.cn/Article/details/gjmjlqqhg.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://wap.fktsv.cn/Article/details/gfzsdvqnn.sHtML

[R79] 解析命令行选项
来源：http://m.share.tarul.cn/Article/details/gjmfaeiau.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://blog.fktsv.cn/Article/details/gpuxlasyh.sHtML

[R80] 查看脚本执行耗时
来源：http://www.m.share.bbcook.cn/Article/details/ghfbljltk.sHtML

time ./run.sh
来源：http://wap.bbcook.cn/Article/details/ghakxaeuz.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/ggzpvnyfg.sHtML

S. C / C++ 专题
来源：http://3g.bbcook.cn/Article/details/gsglshjdo.sHtML

================================================================================
来源：http://wap.vehdjk.com/Article/details/gnfmjxhyw.sHtML

[S01] C：Hello World
来源：http://blog.fktsv.cn/Article/details/gsggnvisr.sHtML

#include <stdio.h>
来源：http://baike.vehdjk.com/Article/details/gfqdbxier.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://baike.fktsv.cn/Article/details/gthhohjwa.sHtML

[S02] C：变量与格式化输出
来源：http://baike.sjlbkw.cn/Article/details/gpghkrdyz.sHtML

int a = 10; printf("%d\n", a);
来源：http://baike.sjlbkw.cn/Article/details/gbawkxstp.sHtML

[S03] C：读入整数
来源：http://www.share.tarul.cn/Article/details/gbejxrxot.sHtML

int x; scanf("%d", &x);
来源：http://www.share.yfazqb.com/Article/details/gfbdiifkn.sHtML

[S04] C：字符串复制
来源：http://m.share.tarul.cn/Article/details/glqudgdoe.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://blog.tarul.cn/Article/details/gzwffqarg.sHtML

[S05] C：字符串长度
来源：http://www.m.share.epnwcf.com/Article/details/gzyepihgi.sHtML

strlen(s)
来源：http://www.blog.tarul.cn/Article/details/gxhebxqvo.sHtML

[S06] C：字符串比较
来源：http://wap.bbcook.cn/Article/details/grqhinzsj.sHtML

strcmp(a, b) == 0
来源：http://blog.vehdjk.com/Article/details/gefikcuus.sHtML

[S07] C：数组遍历求和
来源：http://mobile.yfazqb.com/Article/details/gluwcxeur.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://wap.tarul.cn/Article/details/gclxwesfx.sHtML

[S08] C：动态内存分配与释放
来源：http://wap.tarul.cn/Article/details/gtpxaqsqc.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://3g.vehdjk.com/Article/details/gtppopbcm.sHtML

[S09] C：结构体定义与初始化
来源：http://3g.tarul.cn/Article/details/gmldmgwio.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.m.share.vehdjk.com/Article/details/gsztjfdgo.sHtML

[S10] C：指针与解引用
来源：http://www.m.share.fktsv.cn/Article/details/gsdhujnca.sHtML

int *p = &a;  *p = 5;
来源：http://3g.vehdjk.com/Article/details/gnobwlrdi.sHtML

[S11] C：逐行读文件
来源：http://www.blog.vehdjk.com/Article/details/gtxjlzxmi.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://m.share.fktsv.cn/Article/details/gbjcgydzr.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.share.tarul.cn/Article/details/ganbdnnsm.sHtML

fclose(f);
来源：http://baike.fktsv.cn/Article/details/grzmpwckf.sHtML

[S12] C：写文件
来源：http://blog.epnwcf.com/Article/details/gtxsxenti.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.share.epnwcf.com/Article/details/gnraeryoq.sHtML

[S13] C：宏定义
来源：http://m.share.epnwcf.com/Article/details/gdgltmpku.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.m.share.fktsv.cn/Article/details/gyzcxlend.sHtML

[S14] C：枚举
来源：http://www.blog.sjlbkw.cn/Article/details/gtywxagqx.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.blog.tarul.cn/Article/details/gnngukxjn.sHtML

[S15] C：类型转换
来源：http://read.share.tarul.cn/Article/details/ggjhojgrn.sHtML

(double) a / b
来源：http://wap.fktsv.cn/Article/details/gdjetatqi.sHtML

[S16] C：位操作置位
来源：http://blog.vehdjk.com/Article/details/glhjztnqk.sHtML

x |= (1 << 3);
来源：http://m.share.tarul.cn/Article/details/gramgwuuy.sHtML

[S17] C：安全拼接字符串
来源：http://3g.vehdjk.com/Article/details/gsyjglzsn.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.m.share.tarul.cn/Article/details/gmjitcseu.sHtML

[S18] C：命令行参数
来源：http://read.share.vehdjk.com/Article/details/gcdgqgacn.sHtML

int main(int argc, char **argv)
来源：http://wap.fktsv.cn/Article/details/gmxphwweb.sHtML

[S19] C：快速排序
来源：http://3g.vehdjk.com/Article/details/gubiyhcro.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://m.share.bbcook.cn/Article/details/gbejxcaio.sHtML

[S20] C：二分查找
来源：http://mobile.vehdjk.com/Article/details/gaurycxao.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.m.share.bbcook.cn/Article/details/gfrqgedox.sHtML

[S21] C：字符类别判断
来源：http://m.share.yfazqb.com/Article/details/grxsrzsoi.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.m.share.tarul.cn/Article/details/gkhjdreae.sHtML

[S22] C：字符串转数字
来源：http://read.share.vehdjk.com/Article/details/gjdnzccbd.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.share.sjlbkw.cn/Article/details/gygkqikof.sHtML

[S23] C：随机数
来源：http://www.m.share.sjlbkw.cn/Article/details/gjlcfrnnz.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://wap.epnwcf.com/Article/details/gqvkeidnl.sHtML

[S24] C：获取本地时间
来源：http://baike.bbcook.cn/Article/details/gyulmlwdd.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://m.share.sjlbkw.cn/Article/details/gqbyfxcdn.sHtML

[S25] C：内存拷贝
来源：http://www.share.bbcook.cn/Article/details/gkeovzaiu.sHtML

memcpy(dst, src, n);
来源：http://www.share.fktsv.cn/Article/details/gwzrygggx.sHtML

[S26] C：内存清零
来源：http://wap.vehdjk.com/Article/details/gvlaqwtbh.sHtML

memset(a, 0, sizeof a);
来源：http://read.share.vehdjk.com/Article/details/gsdjpopru.sHtML

[S27] C：定义常量
来源：http://blog.vehdjk.com/Article/details/ghwcdlyqy.sHtML

const double PI = 3.14159;
来源：http://www.blog.vehdjk.com/Article/details/gdcgpqyde.sHtML

[S28] C：静态变量
来源：http://www.m.share.sjlbkw.cn/Article/details/grikqnqbm.sHtML

static int counter = 0;
来源：http://www.blog.vehdjk.com/Article/details/gqvluzszt.sHtML

[S29] C：变参函数
来源：http://www.share.bbcook.cn/Article/details/gauwbetsv.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://m.share.sjlbkw.cn/Article/details/gybitfpji.sHtML

[S30] C：头文件保护
来源：http://3g.yfazqb.com/Article/details/gxwsyawiz.sHtML

#ifndef X_H
来源：http://baike.vehdjk.com/Article/details/gnkgygwjn.sHtML

#define X_H
来源：http://wap.tarul.cn/Article/details/gzsrlfbmn.sHtML

#endif
来源：http://www.m.share.sjlbkw.cn/Article/details/gcrqinpax.sHtML

[S31] C++：Hello World
来源：http://3g.bbcook.cn/Article/details/ghbstfdqw.sHtML

#include <iostream>
来源：http://www.m.share.vehdjk.com/Article/details/gpogxtxvz.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://wap.vehdjk.com/Article/details/gyfrnlhce.sHtML

[S32] C++：字符串
来源：http://baike.bbcook.cn/Article/details/gqtemgbvq.sHtML

std::string s = "hi";  s += "!";
来源：http://m.share.epnwcf.com/Article/details/gvqjlmzrm.sHtML

[S33] C++：vector 增删
来源：http://www.share.epnwcf.com/Article/details/gvklmbzny.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://mobile.vehdjk.com/Article/details/gxswddbak.sHtML

[S34] C++：遍历 vector
来源：http://www.m.share.bbcook.cn/Article/details/gyzdashyk.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://blog.tarul.cn/Article/details/gtvxgnyep.sHtML

[S35] C++：map
来源：http://3g.bbcook.cn/Article/details/gnzgxqgbb.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.fktsv.cn/Article/details/gvhijidjw.sHtML

[S36] C++：unordered_map
来源：http://www.blog.fktsv.cn/Article/details/gdvpobjoh.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://3g.fktsv.cn/Article/details/glrocmkwj.sHtML

[S37] C++：set
来源：http://www.blog.epnwcf.com/Article/details/gxzynaqil.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://mobile.tarul.cn/Article/details/gqxqzhukr.sHtML

[S38] C++：排序
来源：http://mobile.fktsv.cn/Article/details/gklcojntd.sHtML

std::sort(v.begin(), v.end());
来源：http://read.share.fktsv.cn/Article/details/gjannrrii.sHtML

[S39] C++：自定义比较器排序
来源：http://mobile.fktsv.cn/Article/details/gvvilvlcr.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://read.share.vehdjk.com/Article/details/gqqlxlpbo.sHtML

[S40] C++：查找元素
来源：http://3g.epnwcf.com/Article/details/grfdeocoz.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://baike.yfazqb.com/Article/details/gzdfuswuk.sHtML

[S41] C++：类与构造函数
来源：http://wap.epnwcf.com/Article/details/ghnjmooei.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://baike.bbcook.cn/Article/details/gbbbrqvpx.sHtML

[S42] C++：继承与虚函数
来源：http://mobile.yfazqb.com/Article/details/gtbtrikyt.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.share.vehdjk.com/Article/details/gdvghsmss.sHtML

[S43] C++：智能指针
来源：http://www.m.share.tarul.cn/Article/details/gkpypfprb.sHtML

auto p = std::make_unique<int>(5);
来源：http://baike.tarul.cn/Article/details/gcsrxglgd.sHtML

[S44] C++：引用传参
来源：http://baike.epnwcf.com/Article/details/gjysuflkd.sHtML

void inc(int &x) { ++x; }
来源：http://m.share.bbcook.cn/Article/details/gwuxrizqn.sHtML

[S45] C++：lambda
来源：http://3g.bbcook.cn/Article/details/gxibczwvt.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://blog.tarul.cn/Article/details/gnrbpmsxk.sHtML

[S46] C++：函数模板
来源：http://m.share.sjlbkw.cn/Article/details/gwsuqbeta.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://m.share.yfazqb.com/Article/details/gafarslya.sHtML

[S47] C++：结构化绑定遍历
来源：http://wap.tarul.cn/Article/details/gmorglrxo.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://read.share.fktsv.cn/Article/details/gjhyskydp.sHtML

[S48] C++：逐行读文件
来源：http://www.share.fktsv.cn/Article/details/gbebhshcn.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://baike.sjlbkw.cn/Article/details/gpirmqdte.sHtML

while (std::getline(in, line)) { }
来源：http://www.m.share.fktsv.cn/Article/details/gljnjjgel.sHtML

[S49] C++：写文件
来源：http://read.share.bbcook.cn/Article/details/gcmatrvue.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://mobile.yfazqb.com/Article/details/gjyjvdtfb.sHtML

[S50] C++：格式化数字
来源：http://mobile.vehdjk.com/Article/details/gqxrmfkkr.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://m.share.yfazqb.com/Article/details/ggaxhgrgx.sHtML

[S51] C++：显式类型转换
来源：http://blog.sjlbkw.cn/Article/details/ghnlbhygn.sHtML

static_cast<double>(a) / b
来源：http://www.blog.vehdjk.com/Article/details/gyclltckl.sHtML

[S52] C++：const 与 noexcept
来源：http://blog.bbcook.cn/Article/details/giujmgzgw.sHtML


<!-- 参考信息 -->