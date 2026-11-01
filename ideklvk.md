代发 wailian999

[Q84] 去除首尾空格
来源：http://3g.yfazqb.com/Article/details/gfbtncxgx.sHtML

SELECT TRIM(name) FROM users;
来源：http://baike.vehdjk.com/Article/details/gmqeforkw.sHtML

[Q85] 数值取整
来源：http://blog.fktsv.cn/Article/details/gwdyycbah.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://3g.bbcook.cn/Article/details/gkeeiqyrg.sHtML

[Q86] 读取 JSON 字段
来源：http://read.share.epnwcf.com/Article/details/gnayksiby.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://read.share.bbcook.cn/Article/details/gqbvnfoed.sHtML

[Q87] JSON 字段做条件
来源：http://m.share.bbcook.cn/Article/details/gbwsxfzry.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://3g.tarul.cn/Article/details/gwbszfbqd.sHtML

[Q88] 行转列（条件聚合）
来源：http://wap.fktsv.cn/Article/details/gtziquhlt.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://blog.bbcook.cn/Article/details/gkhfbmyeo.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://baike.epnwcf.com/Article/details/gxuarhzpc.sHtML

[Q89] 判断表是否存在
来源：http://mobile.yfazqb.com/Article/details/gxhyeoepm.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://blog.bbcook.cn/Article/details/gehofmgov.sHtML

[Q90] 生成序号列
来源：http://wap.vehdjk.com/Article/details/geepmxylq.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://blog.sjlbkw.cn/Article/details/gxifdouwe.sHtML

================================================================================
来源：http://baike.vehdjk.com/Article/details/ghzxlxjlp.sHtML

R. Bash 专题
来源：http://blog.yfazqb.com/Article/details/gykawdsdb.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/gnmscnmhh.sHtML

[R01] shebang 与严格模式
来源：http://m.share.sjlbkw.cn/Article/details/gyllbsowh.sHtML

#!/usr/bin/env bash
来源：http://m.share.yfazqb.com/Article/details/gbycuvosh.sHtML

set -euo pipefail
来源：http://www.blog.sjlbkw.cn/Article/details/gcjungigx.sHtML

[R02] 变量赋值与使用
来源：http://mobile.sjlbkw.cn/Article/details/gfupgymhk.sHtML

name="Tom"; echo "$name"
来源：http://baike.tarul.cn/Article/details/gmsqbiefs.sHtML

[R03] 只读变量
来源：http://baike.sjlbkw.cn/Article/details/gucsuxmhv.sHtML

readonly PI=3.14
来源：http://www.blog.bbcook.cn/Article/details/ghurnhala.sHtML

[R04] 位置参数
来源：http://baike.yfazqb.com/Article/details/gcajaulqw.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.share.fktsv.cn/Article/details/gsidgvsja.sHtML

[R05] 参数默认值
来源：http://read.share.bbcook.cn/Article/details/gqoxuflhi.sHtML

name="${1:-default}"
来源：http://m.share.tarul.cn/Article/details/gdbyczidb.sHtML

[R06] 判断命令是否存在
来源：http://www.share.vehdjk.com/Article/details/glorhvzik.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://read.share.sjlbkw.cn/Article/details/goegsukez.sHtML

[R07] if 判断文件
来源：http://3g.sjlbkw.cn/Article/details/gkhexfjiu.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.m.share.tarul.cn/Article/details/gkzbggczo.sHtML

[R08] 数值比较
来源：http://www.blog.bbcook.cn/Article/details/gqralquoe.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://blog.vehdjk.com/Article/details/gtwkvodlv.sHtML

[R09] 字符串比较
来源：http://wap.yfazqb.com/Article/details/ggnklgalj.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://m.share.vehdjk.com/Article/details/gslsbkicd.sHtML

[R10] 正则匹配
来源：http://www.m.share.vehdjk.com/Article/details/gdiswsizz.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://blog.epnwcf.com/Article/details/gqqyfgvmr.sHtML

[R11] case 多分支
来源：http://m.share.yfazqb.com/Article/details/gwmcngldb.sHtML

case "$1" in
来源：http://mobile.sjlbkw.cn/Article/details/gtxipvian.sHtML

start) echo "启动" ;;
来源：http://m.share.vehdjk.com/Article/details/gqhzedynz.sHtML

stop)  echo "停止" ;;
来源：http://mobile.fktsv.cn/Article/details/gpsoiqkye.sHtML

*)     echo "未知命令" ;;
来源：http://www.m.share.bbcook.cn/Article/details/gkgcmqjii.sHtML

esac
来源：http://mobile.fktsv.cn/Article/details/gxebxcctq.sHtML

[R12] for 遍历文件
来源：http://3g.sjlbkw.cn/Article/details/gihieutpm.sHtML

for f in *.txt; do echo "$f"; done
来源：http://3g.epnwcf.com/Article/details/gklvgvszs.sHtML

[R13] for 计数循环
来源：http://www.m.share.tarul.cn/Article/details/gyntaudrh.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://read.share.yfazqb.com/Article/details/gryvteaxe.sHtML

[R14] C 风格 for
来源：http://mobile.epnwcf.com/Article/details/gdwfdtjhz.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://mobile.bbcook.cn/Article/details/glomyxwoc.sHtML

[R15] while 逐行读文件
来源：http://wap.bbcook.cn/Article/details/guxkothhi.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.share.yfazqb.com/Article/details/gssufibat.sHtML

[R16] until 等待条件
来源：http://3g.yfazqb.com/Article/details/giylyhyho.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://read.share.tarul.cn/Article/details/gccnmngef.sHtML

[R17] 数组定义与取值
来源：http://3g.yfazqb.com/Article/details/gvxxmyzbz.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://wap.bbcook.cn/Article/details/gkinzqiqs.sHtML

[R18] 遍历数组
来源：http://www.blog.sjlbkw.cn/Article/details/gbxdbwmop.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://baike.bbcook.cn/Article/details/gcqjfecpw.sHtML

[R19] 数组长度
来源：http://baike.tarul.cn/Article/details/gvnabiyhu.sHtML

echo "${#arr[@]}"
来源：http://www.share.vehdjk.com/Article/details/gsmkglzov.sHtML

[R20] 关联数组（字典）
来源：http://www.m.share.epnwcf.com/Article/details/gwmmevnrw.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.m.share.sjlbkw.cn/Article/details/gtbzjnjme.sHtML

[R21] 字符串长度
来源：http://www.share.epnwcf.com/Article/details/gkwigbbmm.sHtML

echo "${#s}"
来源：http://blog.epnwcf.com/Article/details/gujyktyar.sHtML

[R22] 截取子串
来源：http://baike.epnwcf.com/Article/details/gadgyjqvi.sHtML

echo "${s:0:5}"
来源：http://m.share.bbcook.cn/Article/details/gwzlmxrfr.sHtML

[R23] 字符串替换
来源：http://blog.yfazqb.com/Article/details/ggekldjsu.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://read.share.vehdjk.com/Article/details/gieyvdxvq.sHtML

[R24] 大小写转换
来源：http://3g.fktsv.cn/Article/details/goiaeawqu.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.blog.sjlbkw.cn/Article/details/gkxbrsost.sHtML

[R25] 去后缀 / 去前缀
来源：http://m.share.epnwcf.com/Article/details/gcmpsewkd.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://wap.vehdjk.com/Article/details/gkjkpyxmo.sHtML

[R26] 命令替换
来源：http://baike.bbcook.cn/Article/details/gpeqbpkya.sHtML

now=$(date +%F); echo "$now"
来源：http://www.m.share.bbcook.cn/Article/details/glscqfqvf.sHtML

[R27] 算术展开
来源：http://www.m.share.tarul.cn/Article/details/gygmwtxlp.sHtML

echo $((1 + 2 * 3))
来源：http://m.share.bbcook.cn/Article/details/gmkhdvncn.sHtML

[R28] 浮点运算
来源：http://www.blog.epnwcf.com/Article/details/gdmdgdkqf.sHtML

echo "scale=2; 10/3" | bc
来源：http://wap.yfazqb.com/Article/details/golxinnif.sHtML

[R29] 定义函数
来源：http://read.share.fktsv.cn/Article/details/ghevxkhhb.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://wap.vehdjk.com/Article/details/gkhpfsawi.sHtML

[R30] 函数返回状态码
来源：http://baike.epnwcf.com/Article/details/givdyflme.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://blog.fktsv.cn/Article/details/guopiwega.sHtML

[R31] 局部变量
来源：http://blog.yfazqb.com/Article/details/grbfdjfur.sHtML

f() { local x=1; echo "$x"; }
来源：http://mobile.sjlbkw.cn/Article/details/gvgksptsd.sHtML

[R32] 参数个数校验
来源：http://www.m.share.tarul.cn/Article/details/gqloqokqd.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.m.share.yfazqb.com/Article/details/gcqkdloiw.sHtML

[R33] 捕获错误并提示行号
来源：http://www.share.tarul.cn/Article/details/grmtxnets.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://mobile.sjlbkw.cn/Article/details/gjzzndtrs.sHtML

[R34] 退出时清理
来源：http://www.blog.fktsv.cn/Article/details/gbrkdkjdv.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://baike.bbcook.cn/Article/details/gbljllqoi.sHtML

[R35] 后台执行并等待
来源：http://www.m.share.yfazqb.com/Article/details/gijgdtmow.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://3g.epnwcf.com/Article/details/gmexkudok.sHtML

[R36] 并发执行多个任务
来源：http://www.blog.tarul.cn/Article/details/gyxoqnewf.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://baike.tarul.cn/Article/details/grskpurqt.sHtML

[R37] 把输出赋给变量
来源：http://wap.tarul.cn/Article/details/glfsuxcbc.sHtML

files=$(ls -1)
来源：http://blog.epnwcf.com/Article/details/gccuxuojd.sHtML

[R38] 管道串联
来源：http://blog.sjlbkw.cn/Article/details/gwbelpoxc.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.share.sjlbkw.cn/Article/details/ghuqyyxpg.sHtML

[R39] 重定向标准输出与错误
来源：http://read.share.sjlbkw.cn/Article/details/gwxkfuiwf.sHtML

cmd > out.log 2>&1
来源：http://3g.tarul.cn/Article/details/ghaqxyflj.sHtML

[R40] 追加写日志
来源：http://blog.yfazqb.com/Article/details/gvhdiimvz.sHtML

echo "log" >> out.log
来源：http://wap.epnwcf.com/Article/details/gheeqfvko.sHtML

[R41] 丢弃输出
来源：http://mobile.bbcook.cn/Article/details/glvyqrfgu.sHtML

cmd >/dev/null 2>&1
来源：http://www.blog.tarul.cn/Article/details/glchhdgrt.sHtML

[R42] 输入重定向
来源：http://www.m.share.vehdjk.com/Article/details/guqkneqcm.sHtML

wc -l < a.txt
来源：http://baike.fktsv.cn/Article/details/getcrxjst.sHtML

[R43] 按名字查找文件
来源：http://www.blog.fktsv.cn/Article/details/gbxxmfjpt.sHtML

find . -name "*.log" -type f
来源：http://blog.tarul.cn/Article/details/gwmxoiouc.sHtML

[R44] 按修改时间查找
来源：http://mobile.vehdjk.com/Article/details/gukfpcrvz.sHtML

find . -mtime -7 -type f
来源：http://baike.yfazqb.com/Article/details/gkosntumw.sHtML

[R45] 批量删除
来源：http://blog.bbcook.cn/Article/details/ggjgiovof.sHtML

find . -name "*.tmp" -delete
来源：http://baike.vehdjk.com/Article/details/glybuohiv.sHtML

[R46] 递归替换文件内容
来源：http://www.blog.tarul.cn/Article/details/geqbviahu.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://read.share.fktsv.cn/Article/details/glivwegnc.sHtML

[R47] sed 单行替换
来源：http://www.blog.sjlbkw.cn/Article/details/gjzpqkhhv.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.m.share.bbcook.cn/Article/details/grkuqlcms.sHtML

[R48] awk 取指定列
来源：http://mobile.vehdjk.com/Article/details/gorzvophq.sHtML

awk '{print $1, $3}' a.txt
来源：http://read.share.sjlbkw.cn/Article/details/gfszeyuob.sHtML

[R49] awk 带条件
来源：http://www.share.vehdjk.com/Article/details/gcycxjvvc.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.share.bbcook.cn/Article/details/gtanzeyvi.sHtML

[R50] awk 求和
来源：http://read.share.epnwcf.com/Article/details/gapyanqdm.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://blog.tarul.cn/Article/details/gtfmsewmi.sHtML

[R51] 排序去重取前几
来源：http://www.m.share.bbcook.cn/Article/details/gbcuzbyao.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://baike.epnwcf.com/Article/details/gtrnbjtng.sHtML

[R52] 统计行数
来源：http://m.share.bbcook.cn/Article/details/grvakwrpb.sHtML

wc -l a.txt
来源：http://read.share.tarul.cn/Article/details/gngtxgvjc.sHtML

[R53] 查看文件头与实时尾
来源：http://www.share.epnwcf.com/Article/details/gwdentnpk.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://blog.bbcook.cn/Article/details/gpfbagusx.sHtML

[R54] 比较两个文件
来源：http://www.blog.yfazqb.com/Article/details/gtquhpdte.sHtML

diff a.txt b.txt
来源：http://www.m.share.sjlbkw.cn/Article/details/gaucyrfso.sHtML

[R55] 压缩与解压
来源：http://baike.vehdjk.com/Article/details/gyxaiucqf.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://blog.epnwcf.com/Article/details/gykndhgyr.sHtML

[R56] 远程拷贝
来源：http://baike.vehdjk.com/Article/details/gsgxrrhdq.sHtML

scp file user@host:/path/
来源：http://mobile.bbcook.cn/Article/details/gxqiwnkam.sHtML

[R57] 远程执行命令
来源：http://www.m.share.sjlbkw.cn/Article/details/gnpajwios.sHtML

ssh user@host 'uptime'
来源：http://www.share.bbcook.cn/Article/details/gtvdjebhm.sHtML

[R58] 下载文件
来源：http://read.share.fktsv.cn/Article/details/gytpgyodu.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.blog.tarul.cn/Article/details/gluueeapq.sHtML

[R59] 发 POST JSON
来源：http://mobile.tarul.cn/Article/details/goklucgfn.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://blog.bbcook.cn/Article/details/ggdprcdlg.sHtML

[R60] 只看 HTTP 状态码
来源：http://3g.yfazqb.com/Article/details/ghmffurrk.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://m.share.bbcook.cn/Article/details/gitwanbik.sHtML

[R61] 磁盘占用
来源：http://www.share.epnwcf.com/Article/details/gebijyayh.sHtML

df -h;  du -sh *
来源：http://m.share.vehdjk.com/Article/details/gvazlfleo.sHtML

[R62] 找最占空间的文件
来源：http://read.share.fktsv.cn/Article/details/gubwhnnfa.sHtML

du -ah . | sort -rh | head -10
来源：http://www.blog.yfazqb.com/Article/details/gjbwrrlgu.sHtML

[R63] 内存与进程
来源：http://read.share.tarul.cn/Article/details/gzjlrdafe.sHtML

free -h;  ps aux | grep nginx
来源：http://www.m.share.fktsv.cn/Article/details/gmklmtmdb.sHtML

[R64] 结束进程
来源：http://blog.yfazqb.com/Article/details/goyfzjudp.sHtML

kill -9 $(pgrep -f app.py)
来源：http://mobile.fktsv.cn/Article/details/gfrnxatmr.sHtML

[R65] 查看端口占用
来源：http://www.blog.yfazqb.com/Article/details/gqkojcroh.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://baike.epnwcf.com/Article/details/gejtcgkmv.sHtML

[R66] 定时任务
来源：http://www.share.fktsv.cn/Article/details/gvwhwsttx.sHtML

crontab -e;  crontab -l
来源：http://wap.bbcook.cn/Article/details/gwruynmxd.sHtML

[R67] 生成随机十六进制串
来源：http://www.m.share.bbcook.cn/Article/details/ghkmfcqmu.sHtML

openssl rand -hex 16
来源：http://www.m.share.fktsv.cn/Article/details/gwgcxtsaj.sHtML

[R68] 计算文件校验值
来源：http://www.m.share.fktsv.cn/Article/details/gssldurwg.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://mobile.tarul.cn/Article/details/glpvrcrvb.sHtML

[R69] 生成随机密码
来源：http://read.share.epnwcf.com/Article/details/gwtwabjfw.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.share.yfazqb.com/Article/details/gyqqnwmyx.sHtML

[R70] 时间戳与互转
来源：http://read.share.epnwcf.com/Article/details/gsxaxniwy.sHtML

date +%s;  date -d @1700000000
来源：http://m.share.fktsv.cn/Article/details/gveufhvho.sHtML

[R71] 日期格式化
来源：http://www.m.share.fktsv.cn/Article/details/grprgfygd.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://mobile.vehdjk.com/Article/details/gvgytjzap.sHtML

[R72] 等待端口就绪
来源：http://read.share.vehdjk.com/Article/details/gvvxtutbb.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://mobile.tarul.cn/Article/details/gufzmxnjw.sHtML

[R73] 分割大日志
来源：http://www.share.yfazqb.com/Article/details/gnqtgenve.sHtML

split -l 1000 big.log part_
来源：http://wap.fktsv.cn/Article/details/gdsvcsoje.sHtML

[R74] 批量重命名
来源：http://baike.bbcook.cn/Article/details/gcoknkfmg.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.blog.tarul.cn/Article/details/gbyhhbeqt.sHtML

[R75] 导出环境变量
来源：http://m.share.yfazqb.com/Article/details/gfreljady.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.blog.epnwcf.com/Article/details/gvszgoomj.sHtML

[R76] 使用临时文件
来源：http://3g.bbcook.cn/Article/details/gqgqlxeiz.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://blog.fktsv.cn/Article/details/gmuqglkpo.sHtML

[R77] 读取用户输入
来源：http://read.share.sjlbkw.cn/Article/details/gbzyxzsgp.sHtML

read -rp "请输入: " ans
来源：http://www.share.epnwcf.com/Article/details/gddvzhkqs.sHtML

[R78] 交互式菜单
来源：http://mobile.tarul.cn/Article/details/ghwoauaiz.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://3g.bbcook.cn/Article/details/gvgjyjbff.sHtML

[R79] 解析命令行选项
来源：http://mobile.vehdjk.com/Article/details/gfipldilt.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://read.share.yfazqb.com/Article/details/gksaanuob.sHtML

[R80] 查看脚本执行耗时
来源：http://wap.fktsv.cn/Article/details/gsgcryjbe.sHtML

time ./run.sh
来源：http://baike.vehdjk.com/Article/details/gdrvqlctt.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/gdgwyptcy.sHtML

S. C / C++ 专题
来源：http://wap.epnwcf.com/Article/details/gyvaiizba.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/gjiuctinn.sHtML

[S01] C：Hello World
来源：http://wap.vehdjk.com/Article/details/geemrnodn.sHtML

#include <stdio.h>
来源：http://mobile.fktsv.cn/Article/details/gpsgppnwt.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://blog.bbcook.cn/Article/details/gdzqkjahm.sHtML

[S02] C：变量与格式化输出
来源：http://blog.bbcook.cn/Article/details/ghzursgky.sHtML

int a = 10; printf("%d\n", a);
来源：http://3g.sjlbkw.cn/Article/details/gvbqbifve.sHtML

[S03] C：读入整数
来源：http://www.blog.fktsv.cn/Article/details/gulsyjrrp.sHtML

int x; scanf("%d", &x);
来源：http://3g.epnwcf.com/Article/details/ggfhaccln.sHtML

[S04] C：字符串复制
来源：http://read.share.bbcook.cn/Article/details/gkfvmyjaq.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.m.share.epnwcf.com/Article/details/grrmbeyvj.sHtML

[S05] C：字符串长度
来源：http://www.m.share.vehdjk.com/Article/details/gfyfheawm.sHtML

strlen(s)
来源：http://m.share.epnwcf.com/Article/details/gkpeiipfx.sHtML

[S06] C：字符串比较
来源：http://www.m.share.yfazqb.com/Article/details/gellebpig.sHtML

strcmp(a, b) == 0
来源：http://wap.fktsv.cn/Article/details/gqufitier.sHtML

[S07] C：数组遍历求和
来源：http://www.m.share.sjlbkw.cn/Article/details/gfpndywtb.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://m.share.tarul.cn/Article/details/gjpgbfovl.sHtML

[S08] C：动态内存分配与释放
来源：http://baike.fktsv.cn/Article/details/gvnolpyax.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.blog.epnwcf.com/Article/details/gaumbcdhl.sHtML

[S09] C：结构体定义与初始化
来源：http://www.share.yfazqb.com/Article/details/gqqhdsnpc.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://3g.fktsv.cn/Article/details/gcabjsmhw.sHtML

[S10] C：指针与解引用
来源：http://mobile.epnwcf.com/Article/details/gqskryvbk.sHtML

int *p = &a;  *p = 5;
来源：http://3g.epnwcf.com/Article/details/gpxemeiiz.sHtML

[S11] C：逐行读文件
来源：http://m.share.tarul.cn/Article/details/gpdpnnbmk.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://read.share.yfazqb.com/Article/details/gohlpzhth.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.blog.epnwcf.com/Article/details/gshekjudn.sHtML

fclose(f);
来源：http://blog.epnwcf.com/Article/details/gpudhlpxg.sHtML

[S12] C：写文件
来源：http://baike.sjlbkw.cn/Article/details/glskmobkl.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://baike.vehdjk.com/Article/details/gtmfshdbh.sHtML

[S13] C：宏定义
来源：http://www.m.share.yfazqb.com/Article/details/gbtukqeii.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.m.share.yfazqb.com/Article/details/gxfqqsxnr.sHtML

[S14] C：枚举
来源：http://3g.bbcook.cn/Article/details/gxsjbcfof.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.m.share.bbcook.cn/Article/details/gmekknvvr.sHtML

[S15] C：类型转换
来源：http://read.share.fktsv.cn/Article/details/giyfihdqq.sHtML

(double) a / b
来源：http://wap.epnwcf.com/Article/details/gxyiuqscd.sHtML

[S16] C：位操作置位
来源：http://3g.yfazqb.com/Article/details/gkbrtpafx.sHtML

x |= (1 << 3);
来源：http://m.share.bbcook.cn/Article/details/gihopbqqy.sHtML

[S17] C：安全拼接字符串
来源：http://read.share.fktsv.cn/Article/details/gugmdvlnj.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://blog.vehdjk.com/Article/details/gkuwkcxhf.sHtML

[S18] C：命令行参数
来源：http://www.m.share.yfazqb.com/Article/details/ghvpapwkh.sHtML

int main(int argc, char **argv)
来源：http://3g.epnwcf.com/Article/details/gnqremtfj.sHtML

[S19] C：快速排序
来源：http://m.share.yfazqb.com/Article/details/gihsaoika.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.m.share.fktsv.cn/Article/details/gzbcbtwkw.sHtML

[S20] C：二分查找
来源：http://baike.sjlbkw.cn/Article/details/ghetpvknv.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://m.share.vehdjk.com/Article/details/grsfrjhed.sHtML

[S21] C：字符类别判断
来源：http://blog.vehdjk.com/Article/details/gfdcypwct.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://3g.sjlbkw.cn/Article/details/gtjmdrofl.sHtML

[S22] C：字符串转数字
来源：http://mobile.vehdjk.com/Article/details/gzgcngave.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://mobile.fktsv.cn/Article/details/goqhmfyyk.sHtML

[S23] C：随机数
来源：http://www.m.share.vehdjk.com/Article/details/gacjcarxe.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://blog.bbcook.cn/Article/details/glclegswu.sHtML

[S24] C：获取本地时间
来源：http://3g.yfazqb.com/Article/details/gerulwyzq.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://m.share.tarul.cn/Article/details/girpkbxun.sHtML

[S25] C：内存拷贝
来源：http://www.share.bbcook.cn/Article/details/gtogpfvbg.sHtML

memcpy(dst, src, n);
来源：http://www.blog.sjlbkw.cn/Article/details/gdrjgtyjo.sHtML

[S26] C：内存清零
来源：http://www.share.bbcook.cn/Article/details/galtewweb.sHtML

memset(a, 0, sizeof a);
来源：http://blog.yfazqb.com/Article/details/geoehkipz.sHtML

[S27] C：定义常量
来源：http://www.share.tarul.cn/Article/details/gnfjrcdtk.sHtML

const double PI = 3.14159;
来源：http://mobile.yfazqb.com/Article/details/gqqkblwgo.sHtML

[S28] C：静态变量
来源：http://www.blog.tarul.cn/Article/details/gynddknbb.sHtML

static int counter = 0;
来源：http://mobile.sjlbkw.cn/Article/details/gzctjbdgi.sHtML

[S29] C：变参函数
来源：http://www.m.share.yfazqb.com/Article/details/gcpsmnwwa.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mobile.vehdjk.com/Article/details/grxrdfqkl.sHtML

[S30] C：头文件保护
来源：http://www.share.yfazqb.com/Article/details/gxuwejuxo.sHtML

#ifndef X_H
来源：http://read.share.yfazqb.com/Article/details/gofbrfnac.sHtML

#define X_H
来源：http://m.share.vehdjk.com/Article/details/gxooyvplo.sHtML

#endif
来源：http://read.share.vehdjk.com/Article/details/gvgtlunmt.sHtML

[S31] C++：Hello World
来源：http://www.share.sjlbkw.cn/Article/details/gysncznti.sHtML

#include <iostream>
来源：http://www.share.fktsv.cn/Article/details/gjdmdtqos.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://read.share.yfazqb.com/Article/details/grlbqgvkc.sHtML

[S32] C++：字符串
来源：http://www.m.share.vehdjk.com/Article/details/gfyvxshdg.sHtML

std::string s = "hi";  s += "!";
来源：http://m.share.vehdjk.com/Article/details/gqsszopol.sHtML

[S33] C++：vector 增删
来源：http://mobile.yfazqb.com/Article/details/gwzusllsp.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://baike.fktsv.cn/Article/details/gdvbyxrco.sHtML

[S34] C++：遍历 vector
来源：http://m.share.bbcook.cn/Article/details/gcdeetgqy.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://blog.yfazqb.com/Article/details/gobgyjylf.sHtML

[S35] C++：map
来源：http://blog.epnwcf.com/Article/details/grprqyjok.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.yfazqb.com/Article/details/gcxptbjwe.sHtML

[S36] C++：unordered_map
来源：http://mobile.tarul.cn/Article/details/gxditjttv.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.sjlbkw.cn/Article/details/gtgyuensk.sHtML

[S37] C++：set
来源：http://m.share.epnwcf.com/Article/details/gfjgqfvoa.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://m.share.bbcook.cn/Article/details/guocntlmu.sHtML

[S38] C++：排序
来源：http://www.share.sjlbkw.cn/Article/details/gbqfqjgyk.sHtML

std::sort(v.begin(), v.end());
来源：http://wap.epnwcf.com/Article/details/gnyegtfnj.sHtML

[S39] C++：自定义比较器排序
来源：http://3g.fktsv.cn/Article/details/gjuuaszmb.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.m.share.sjlbkw.cn/Article/details/gmtymsmka.sHtML

[S40] C++：查找元素
来源：http://blog.epnwcf.com/Article/details/gxyowpvcs.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://blog.bbcook.cn/Article/details/gdeqpjrhy.sHtML

[S41] C++：类与构造函数
来源：http://www.share.bbcook.cn/Article/details/gxwuhupef.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://wap.sjlbkw.cn/Article/details/gpdnyiuju.sHtML

[S42] C++：继承与虚函数
来源：http://m.share.bbcook.cn/Article/details/gygrbkiyr.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.share.fktsv.cn/Article/details/gkbpbilwa.sHtML

[S43] C++：智能指针
来源：http://www.share.fktsv.cn/Article/details/gzllatale.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.blog.sjlbkw.cn/Article/details/gyjxjeqzr.sHtML

[S44] C++：引用传参
来源：http://www.share.fktsv.cn/Article/details/goijgkblk.sHtML

void inc(int &x) { ++x; }
来源：http://www.m.share.tarul.cn/Article/details/gwfeazial.sHtML

[S45] C++：lambda
来源：http://www.m.share.vehdjk.com/Article/details/gqkqnbboc.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://read.share.epnwcf.com/Article/details/gwoarticv.sHtML

[S46] C++：函数模板
来源：http://www.m.share.fktsv.cn/Article/details/grxeglidn.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://m.share.yfazqb.com/Article/details/gmttjajdj.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.blog.vehdjk.com/Article/details/gsahzhkxl.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.blog.yfazqb.com/Article/details/gkokjskmr.sHtML

[S48] C++：逐行读文件
来源：http://wap.tarul.cn/Article/details/gjyozlxgt.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://read.share.bbcook.cn/Article/details/gpmaynvhp.sHtML

while (std::getline(in, line)) { }
来源：http://www.blog.tarul.cn/Article/details/gdkgshbwc.sHtML

[S49] C++：写文件
来源：http://www.blog.bbcook.cn/Article/details/gwsvcmuev.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://read.share.tarul.cn/Article/details/gnqwbrwdr.sHtML

[S50] C++：格式化数字
来源：http://blog.bbcook.cn/Article/details/gohamqqkn.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://mobile.fktsv.cn/Article/details/gjxcxyalc.sHtML

[S51] C++：显式类型转换
来源：http://blog.bbcook.cn/Article/details/gxajogniz.sHtML

static_cast<double>(a) / b
来源：http://read.share.bbcook.cn/Article/details/gdordpfzw.sHtML

[S52] C++：const 与 noexcept
来源：http://www.m.share.tarul.cn/Article/details/gsyauuacd.sHtML

int size() const noexcept { return n_; }
来源：http://baike.yfazqb.com/Article/details/ghsodflri.sHtML

[S53] C++：移动语义
来源：http://mobile.tarul.cn/Article/details/ghebugmsk.sHtML

std::vector<int> w = std::move(v);
来源：http://mobile.fktsv.cn/Article/details/gudruanem.sHtML

[S54] C++：异常处理
来源：http://m.share.fktsv.cn/Article/details/gwjjnxfml.sHtML


<!-- 参考信息 -->