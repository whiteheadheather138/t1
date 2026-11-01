代发 wailian999

[Q88] 行转列（条件聚合）
来源：http://baike.yfazqb.com/Article/details/gjpbpyubf.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://baike.bbcook.cn/Article/details/gbvchdcco.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.m.share.sjlbkw.cn/Article/details/gmdftqfzo.sHtML

[Q89] 判断表是否存在
来源：http://www.m.share.vehdjk.com/Article/details/gyjnzmlhf.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://baike.bbcook.cn/Article/details/geeocywns.sHtML

[Q90] 生成序号列
来源：http://blog.bbcook.cn/Article/details/grejehhyi.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://m.share.epnwcf.com/Article/details/garckpwkh.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/gsbgjarmt.sHtML

R. Bash 专题
来源：http://m.share.fktsv.cn/Article/details/gyzcdxdae.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/gnipzxaaq.sHtML

[R01] shebang 与严格模式
来源：http://blog.epnwcf.com/Article/details/gzbofqwdl.sHtML

#!/usr/bin/env bash
来源：http://www.share.yfazqb.com/Article/details/gbzfwxpfz.sHtML

set -euo pipefail
来源：http://m.share.tarul.cn/Article/details/gyhqrvzjn.sHtML

[R02] 变量赋值与使用
来源：http://m.share.yfazqb.com/Article/details/gowctjlmd.sHtML

name="Tom"; echo "$name"
来源：http://m.share.yfazqb.com/Article/details/gkndpdmpg.sHtML

[R03] 只读变量
来源：http://wap.yfazqb.com/Article/details/gcyqnbcdf.sHtML

readonly PI=3.14
来源：http://mobile.epnwcf.com/Article/details/glqzrqhht.sHtML

[R04] 位置参数
来源：http://3g.sjlbkw.cn/Article/details/gygqppjbk.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://m.share.tarul.cn/Article/details/gzfdszwpz.sHtML

[R05] 参数默认值
来源：http://wap.vehdjk.com/Article/details/gsotzyqii.sHtML

name="${1:-default}"
来源：http://www.m.share.fktsv.cn/Article/details/gzzrsmmnl.sHtML

[R06] 判断命令是否存在
来源：http://baike.tarul.cn/Article/details/gyrnynspj.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://read.share.sjlbkw.cn/Article/details/gvgbbjyjo.sHtML

[R07] if 判断文件
来源：http://baike.bbcook.cn/Article/details/gbglxfpuu.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.share.epnwcf.com/Article/details/gyqiufcke.sHtML

[R08] 数值比较
来源：http://mobile.epnwcf.com/Article/details/gkpvrotba.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://baike.epnwcf.com/Article/details/gngzdakiv.sHtML

[R09] 字符串比较
来源：http://www.m.share.tarul.cn/Article/details/gsvfwxshp.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://m.share.bbcook.cn/Article/details/gyxyzpvwv.sHtML

[R10] 正则匹配
来源：http://www.blog.tarul.cn/Article/details/ghfnbbebg.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.share.bbcook.cn/Article/details/gbfltikyd.sHtML

[R11] case 多分支
来源：http://read.share.vehdjk.com/Article/details/glrvhdiii.sHtML

case "$1" in
来源：http://m.share.fktsv.cn/Article/details/gztphlcry.sHtML

start) echo "启动" ;;
来源：http://m.share.vehdjk.com/Article/details/gnkrfvhdb.sHtML

stop)  echo "停止" ;;
来源：http://m.share.yfazqb.com/Article/details/gpsaqgclz.sHtML

*)     echo "未知命令" ;;
来源：http://read.share.fktsv.cn/Article/details/gxjeogchv.sHtML

esac
来源：http://baike.epnwcf.com/Article/details/gtsouvsbk.sHtML

[R12] for 遍历文件
来源：http://www.share.fktsv.cn/Article/details/gqdkrpxxc.sHtML

for f in *.txt; do echo "$f"; done
来源：http://m.share.yfazqb.com/Article/details/gvkupdkyt.sHtML

[R13] for 计数循环
来源：http://www.share.yfazqb.com/Article/details/gaigribti.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.share.tarul.cn/Article/details/gksqvlkzx.sHtML

[R14] C 风格 for
来源：http://3g.tarul.cn/Article/details/gqqrcynpg.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.m.share.epnwcf.com/Article/details/gtsjhzqnd.sHtML

[R15] while 逐行读文件
来源：http://m.share.fktsv.cn/Article/details/gexiovznb.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://baike.vehdjk.com/Article/details/gjkajbucz.sHtML

[R16] until 等待条件
来源：http://baike.bbcook.cn/Article/details/gkmtuppjq.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://m.share.tarul.cn/Article/details/gtrnowexo.sHtML

[R17] 数组定义与取值
来源：http://wap.yfazqb.com/Article/details/gnjmmfhgv.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://wap.tarul.cn/Article/details/gwxisdquz.sHtML

[R18] 遍历数组
来源：http://www.share.yfazqb.com/Article/details/gbmymdwio.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.m.share.epnwcf.com/Article/details/gsexlobex.sHtML

[R19] 数组长度
来源：http://blog.tarul.cn/Article/details/gordpobma.sHtML

echo "${#arr[@]}"
来源：http://www.share.bbcook.cn/Article/details/ggknjijyt.sHtML

[R20] 关联数组（字典）
来源：http://www.share.epnwcf.com/Article/details/gmkiwehlj.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://read.share.epnwcf.com/Article/details/gvdffjepv.sHtML

[R21] 字符串长度
来源：http://mobile.tarul.cn/Article/details/gnqbcxict.sHtML

echo "${#s}"
来源：http://3g.epnwcf.com/Article/details/gelgwvnqr.sHtML

[R22] 截取子串
来源：http://www.blog.yfazqb.com/Article/details/gqbvavqtt.sHtML

echo "${s:0:5}"
来源：http://wap.fktsv.cn/Article/details/gldaemkby.sHtML

[R23] 字符串替换
来源：http://www.share.bbcook.cn/Article/details/gxiuzuigv.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.m.share.vehdjk.com/Article/details/gauvpveic.sHtML

[R24] 大小写转换
来源：http://www.m.share.bbcook.cn/Article/details/grzifvrvl.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://wap.epnwcf.com/Article/details/ginnmpvmf.sHtML

[R25] 去后缀 / 去前缀
来源：http://mobile.fktsv.cn/Article/details/gijxqkqnr.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.m.share.epnwcf.com/Article/details/gylvkcvbi.sHtML

[R26] 命令替换
来源：http://baike.fktsv.cn/Article/details/gqfqovjxa.sHtML

now=$(date +%F); echo "$now"
来源：http://www.share.epnwcf.com/Article/details/grkdhgwzr.sHtML

[R27] 算术展开
来源：http://www.share.bbcook.cn/Article/details/gfcewfcov.sHtML

echo $((1 + 2 * 3))
来源：http://baike.sjlbkw.cn/Article/details/gfyucywsq.sHtML

[R28] 浮点运算
来源：http://m.share.epnwcf.com/Article/details/gxkkrjbbi.sHtML

echo "scale=2; 10/3" | bc
来源：http://read.share.vehdjk.com/Article/details/gwecyxjyb.sHtML

[R29] 定义函数
来源：http://read.share.epnwcf.com/Article/details/gsqcugutc.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.blog.sjlbkw.cn/Article/details/gssxtyyag.sHtML

[R30] 函数返回状态码
来源：http://3g.sjlbkw.cn/Article/details/gppjqgkxw.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://m.share.epnwcf.com/Article/details/gswfmrswm.sHtML

[R31] 局部变量
来源：http://3g.bbcook.cn/Article/details/gjbpgcknq.sHtML

f() { local x=1; echo "$x"; }
来源：http://read.share.bbcook.cn/Article/details/gvfnrqqqz.sHtML

[R32] 参数个数校验
来源：http://www.blog.yfazqb.com/Article/details/guaybkcep.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://3g.fktsv.cn/Article/details/grdxapqpr.sHtML

[R33] 捕获错误并提示行号
来源：http://www.m.share.vehdjk.com/Article/details/gaebbhbpq.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://3g.epnwcf.com/Article/details/gouuggfef.sHtML

[R34] 退出时清理
来源：http://read.share.yfazqb.com/Article/details/gdjajpulr.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://3g.vehdjk.com/Article/details/gvmizxymn.sHtML

[R35] 后台执行并等待
来源：http://blog.sjlbkw.cn/Article/details/grwrpdrdf.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://wap.yfazqb.com/Article/details/gqocaundi.sHtML

[R36] 并发执行多个任务
来源：http://mobile.sjlbkw.cn/Article/details/ggburhgka.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://read.share.yfazqb.com/Article/details/gdzkrxqrq.sHtML

[R37] 把输出赋给变量
来源：http://blog.fktsv.cn/Article/details/gsloikldo.sHtML

files=$(ls -1)
来源：http://baike.epnwcf.com/Article/details/gndspgprh.sHtML

[R38] 管道串联
来源：http://read.share.fktsv.cn/Article/details/goqlmtlsy.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.share.vehdjk.com/Article/details/gpwcwtwfo.sHtML

[R39] 重定向标准输出与错误
来源：http://wap.bbcook.cn/Article/details/geeqsnbpz.sHtML

cmd > out.log 2>&1
来源：http://read.share.epnwcf.com/Article/details/gbzrsruhb.sHtML

[R40] 追加写日志
来源：http://m.share.sjlbkw.cn/Article/details/gbgfiqbiv.sHtML

echo "log" >> out.log
来源：http://www.m.share.tarul.cn/Article/details/gaoizhgba.sHtML

[R41] 丢弃输出
来源：http://www.share.vehdjk.com/Article/details/gtjkpvzfp.sHtML

cmd >/dev/null 2>&1
来源：http://www.share.epnwcf.com/Article/details/gyivktuvp.sHtML

[R42] 输入重定向
来源：http://www.blog.yfazqb.com/Article/details/gyxbwrvwf.sHtML

wc -l < a.txt
来源：http://read.share.tarul.cn/Article/details/gzlgfcisw.sHtML

[R43] 按名字查找文件
来源：http://www.blog.fktsv.cn/Article/details/gaexthqzw.sHtML

find . -name "*.log" -type f
来源：http://m.share.sjlbkw.cn/Article/details/gdpzraydq.sHtML

[R44] 按修改时间查找
来源：http://m.share.bbcook.cn/Article/details/gyvgzyejr.sHtML

find . -mtime -7 -type f
来源：http://m.share.sjlbkw.cn/Article/details/gplhzzezq.sHtML

[R45] 批量删除
来源：http://m.share.yfazqb.com/Article/details/gynslgudv.sHtML

find . -name "*.tmp" -delete
来源：http://m.share.tarul.cn/Article/details/grppqozhx.sHtML

[R46] 递归替换文件内容
来源：http://blog.tarul.cn/Article/details/gsesgtlbf.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://3g.tarul.cn/Article/details/gmjobuuql.sHtML

[R47] sed 单行替换
来源：http://blog.bbcook.cn/Article/details/gmkchvxur.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://wap.vehdjk.com/Article/details/gjrbpcxje.sHtML

[R48] awk 取指定列
来源：http://www.share.tarul.cn/Article/details/ggflqioul.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.blog.epnwcf.com/Article/details/goxmbfjrq.sHtML

[R49] awk 带条件
来源：http://3g.vehdjk.com/Article/details/garmsrfyu.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.share.tarul.cn/Article/details/gcwfwuact.sHtML

[R50] awk 求和
来源：http://m.share.tarul.cn/Article/details/gkoytcuyi.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.blog.fktsv.cn/Article/details/gfcttiwca.sHtML

[R51] 排序去重取前几
来源：http://www.blog.bbcook.cn/Article/details/gyjwvijgm.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://blog.sjlbkw.cn/Article/details/gyolfjrmr.sHtML

[R52] 统计行数
来源：http://read.share.fktsv.cn/Article/details/gqwazqddh.sHtML

wc -l a.txt
来源：http://read.share.tarul.cn/Article/details/gybgjcbri.sHtML

[R53] 查看文件头与实时尾
来源：http://mobile.bbcook.cn/Article/details/gjmvmvnke.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.m.share.fktsv.cn/Article/details/gawgqtjpo.sHtML

[R54] 比较两个文件
来源：http://read.share.bbcook.cn/Article/details/gzopsubuh.sHtML

diff a.txt b.txt
来源：http://www.blog.tarul.cn/Article/details/ghsuexbrc.sHtML

[R55] 压缩与解压
来源：http://3g.sjlbkw.cn/Article/details/gufklaqsv.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.m.share.bbcook.cn/Article/details/goqagpkzk.sHtML

[R56] 远程拷贝
来源：http://www.blog.sjlbkw.cn/Article/details/gwvdquxeq.sHtML

scp file user@host:/path/
来源：http://blog.vehdjk.com/Article/details/ggdkuwpuw.sHtML

[R57] 远程执行命令
来源：http://baike.epnwcf.com/Article/details/gwtvebnmk.sHtML

ssh user@host 'uptime'
来源：http://mobile.yfazqb.com/Article/details/gpmaolira.sHtML

[R58] 下载文件
来源：http://wap.vehdjk.com/Article/details/gsitbsvej.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.m.share.fktsv.cn/Article/details/gjovelxvk.sHtML

[R59] 发 POST JSON
来源：http://blog.epnwcf.com/Article/details/gjmzithzj.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://baike.epnwcf.com/Article/details/gcgvfifbm.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.blog.tarul.cn/Article/details/gwbhffirq.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://blog.tarul.cn/Article/details/gzviutqct.sHtML

[R61] 磁盘占用
来源：http://www.blog.yfazqb.com/Article/details/gddctqfdy.sHtML

df -h;  du -sh *
来源：http://mobile.bbcook.cn/Article/details/gaszwdukb.sHtML

[R62] 找最占空间的文件
来源：http://m.share.tarul.cn/Article/details/gaustjwse.sHtML

du -ah . | sort -rh | head -10
来源：http://www.blog.fktsv.cn/Article/details/gvrykefoc.sHtML

[R63] 内存与进程
来源：http://www.blog.bbcook.cn/Article/details/gyqomscna.sHtML

free -h;  ps aux | grep nginx
来源：http://blog.yfazqb.com/Article/details/giylqpxdb.sHtML

[R64] 结束进程
来源：http://blog.vehdjk.com/Article/details/gvnjxxnjj.sHtML

kill -9 $(pgrep -f app.py)
来源：http://blog.fktsv.cn/Article/details/gkhewpuzc.sHtML

[R65] 查看端口占用
来源：http://www.blog.tarul.cn/Article/details/ggczpzety.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.m.share.yfazqb.com/Article/details/guiaeayfi.sHtML

[R66] 定时任务
来源：http://m.share.bbcook.cn/Article/details/gsgavuhlm.sHtML

crontab -e;  crontab -l
来源：http://www.share.bbcook.cn/Article/details/gzfmgyqmy.sHtML

[R67] 生成随机十六进制串
来源：http://m.share.yfazqb.com/Article/details/gqzkrhztc.sHtML

openssl rand -hex 16
来源：http://3g.sjlbkw.cn/Article/details/gopjzfkkp.sHtML

[R68] 计算文件校验值
来源：http://www.blog.tarul.cn/Article/details/gdmsvdxuk.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.share.bbcook.cn/Article/details/gakqkgtyn.sHtML

[R69] 生成随机密码
来源：http://blog.epnwcf.com/Article/details/gbuxqmpis.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.blog.yfazqb.com/Article/details/gcuojesea.sHtML

[R70] 时间戳与互转
来源：http://www.share.yfazqb.com/Article/details/gprtemvhz.sHtML

date +%s;  date -d @1700000000
来源：http://3g.sjlbkw.cn/Article/details/gebbvxwkh.sHtML

[R71] 日期格式化
来源：http://wap.yfazqb.com/Article/details/gnfbncfci.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://baike.bbcook.cn/Article/details/gthvqoxpb.sHtML

[R72] 等待端口就绪
来源：http://read.share.tarul.cn/Article/details/geqqodinb.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://m.share.fktsv.cn/Article/details/gdnlwgsko.sHtML

[R73] 分割大日志
来源：http://wap.yfazqb.com/Article/details/gurugckrz.sHtML

split -l 1000 big.log part_
来源：http://wap.vehdjk.com/Article/details/genxgzmvn.sHtML

[R74] 批量重命名
来源：http://m.share.bbcook.cn/Article/details/ggjjluztl.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://m.share.epnwcf.com/Article/details/gyyuaisym.sHtML

[R75] 导出环境变量
来源：http://baike.epnwcf.com/Article/details/gvlyhmtyc.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://m.share.tarul.cn/Article/details/gkcyqhbfb.sHtML

[R76] 使用临时文件
来源：http://3g.yfazqb.com/Article/details/gqldhqlge.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://wap.fktsv.cn/Article/details/gnxftzwpq.sHtML

[R77] 读取用户输入
来源：http://baike.vehdjk.com/Article/details/gswxmkfzz.sHtML

read -rp "请输入: " ans
来源：http://3g.bbcook.cn/Article/details/gdjceayud.sHtML

[R78] 交互式菜单
来源：http://m.share.sjlbkw.cn/Article/details/gxcovqxcm.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://baike.vehdjk.com/Article/details/gfytwgvwh.sHtML

[R79] 解析命令行选项
来源：http://mobile.fktsv.cn/Article/details/gqzfpnlko.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://m.share.fktsv.cn/Article/details/ggztddfqj.sHtML

[R80] 查看脚本执行耗时
来源：http://baike.bbcook.cn/Article/details/goroiagfm.sHtML

time ./run.sh
来源：http://blog.tarul.cn/Article/details/gnqimpjby.sHtML

================================================================================
来源：http://3g.epnwcf.com/Article/details/gjxiypqfz.sHtML

S. C / C++ 专题
来源：http://mobile.vehdjk.com/Article/details/gurmcqjja.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/grcizziam.sHtML

[S01] C：Hello World
来源：http://3g.yfazqb.com/Article/details/gvaotkezb.sHtML

#include <stdio.h>
来源：http://read.share.sjlbkw.cn/Article/details/gnsnyjkkj.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://blog.epnwcf.com/Article/details/gsrtsqlsi.sHtML

[S02] C：变量与格式化输出
来源：http://m.share.bbcook.cn/Article/details/gipodqvkp.sHtML

int a = 10; printf("%d\n", a);
来源：http://wap.fktsv.cn/Article/details/gebsndbqf.sHtML

[S03] C：读入整数
来源：http://m.share.vehdjk.com/Article/details/gzaeifgew.sHtML

int x; scanf("%d", &x);
来源：http://m.share.epnwcf.com/Article/details/gtlqkapfr.sHtML

[S04] C：字符串复制
来源：http://3g.yfazqb.com/Article/details/gnigqppmo.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://baike.sjlbkw.cn/Article/details/guxlafivx.sHtML

[S05] C：字符串长度
来源：http://www.share.sjlbkw.cn/Article/details/gjzkgycie.sHtML

strlen(s)
来源：http://mobile.vehdjk.com/Article/details/gdnnwjbgd.sHtML

[S06] C：字符串比较
来源：http://www.share.yfazqb.com/Article/details/gkqjytopq.sHtML

strcmp(a, b) == 0
来源：http://www.m.share.sjlbkw.cn/Article/details/gofrwnana.sHtML

[S07] C：数组遍历求和
来源：http://www.m.share.yfazqb.com/Article/details/gdkfymxyd.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://3g.yfazqb.com/Article/details/gtrjsbfrh.sHtML

[S08] C：动态内存分配与释放
来源：http://wap.bbcook.cn/Article/details/gckdsatth.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.m.share.epnwcf.com/Article/details/gnlqucmqp.sHtML

[S09] C：结构体定义与初始化
来源：http://wap.fktsv.cn/Article/details/gqehyjykp.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.m.share.epnwcf.com/Article/details/gyuerldrr.sHtML

[S10] C：指针与解引用
来源：http://baike.sjlbkw.cn/Article/details/gddymfsuj.sHtML

int *p = &a;  *p = 5;
来源：http://www.blog.tarul.cn/Article/details/gpaokeoim.sHtML

[S11] C：逐行读文件
来源：http://www.blog.tarul.cn/Article/details/gwvmngjdv.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://blog.sjlbkw.cn/Article/details/gfgomxnuc.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.share.sjlbkw.cn/Article/details/gtknubkjn.sHtML

fclose(f);
来源：http://www.share.fktsv.cn/Article/details/gcgyssvff.sHtML

[S12] C：写文件
来源：http://baike.tarul.cn/Article/details/ggyxonyxa.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mobile.bbcook.cn/Article/details/graacpuim.sHtML

[S13] C：宏定义
来源：http://mobile.yfazqb.com/Article/details/gontahket.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.share.yfazqb.com/Article/details/gnfxyjfvx.sHtML

[S14] C：枚举
来源：http://mobile.yfazqb.com/Article/details/gjyhrrybi.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.share.fktsv.cn/Article/details/gokkfxoqh.sHtML

[S15] C：类型转换
来源：http://baike.bbcook.cn/Article/details/gubntitjm.sHtML

(double) a / b
来源：http://wap.fktsv.cn/Article/details/gmlgcawth.sHtML

[S16] C：位操作置位
来源：http://3g.tarul.cn/Article/details/gbyelasef.sHtML

x |= (1 << 3);
来源：http://www.share.epnwcf.com/Article/details/glmkrdhtq.sHtML

[S17] C：安全拼接字符串
来源：http://www.m.share.vehdjk.com/Article/details/gljbbcfgu.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wap.yfazqb.com/Article/details/goyevgjdx.sHtML

[S18] C：命令行参数
来源：http://3g.tarul.cn/Article/details/gkqsqmpim.sHtML

int main(int argc, char **argv)
来源：http://wap.tarul.cn/Article/details/gyyejjmjo.sHtML

[S19] C：快速排序
来源：http://3g.sjlbkw.cn/Article/details/gcqzxqgwd.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.blog.bbcook.cn/Article/details/gspngebls.sHtML

[S20] C：二分查找
来源：http://read.share.bbcook.cn/Article/details/gmdlwkcgh.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://3g.fktsv.cn/Article/details/gypswfszn.sHtML

[S21] C：字符类别判断
来源：http://www.share.sjlbkw.cn/Article/details/gryaftprf.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://read.share.epnwcf.com/Article/details/gnkehuxzz.sHtML

[S22] C：字符串转数字
来源：http://www.m.share.vehdjk.com/Article/details/gfrwdfsnw.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://read.share.bbcook.cn/Article/details/gvwdaetpx.sHtML

[S23] C：随机数
来源：http://wap.tarul.cn/Article/details/gxrhopwho.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://baike.epnwcf.com/Article/details/glaeuouxx.sHtML

[S24] C：获取本地时间
来源：http://mobile.vehdjk.com/Article/details/gcopreciq.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.share.sjlbkw.cn/Article/details/gcgtcbxsp.sHtML

[S25] C：内存拷贝
来源：http://www.m.share.epnwcf.com/Article/details/gsvwbqzgv.sHtML

memcpy(dst, src, n);
来源：http://read.share.tarul.cn/Article/details/gizmeaavz.sHtML

[S26] C：内存清零
来源：http://3g.sjlbkw.cn/Article/details/gnbkjvizu.sHtML

memset(a, 0, sizeof a);
来源：http://baike.fktsv.cn/Article/details/gmgfayomd.sHtML

[S27] C：定义常量
来源：http://www.blog.tarul.cn/Article/details/gqmdkqzgo.sHtML

const double PI = 3.14159;
来源：http://3g.epnwcf.com/Article/details/gcmcfbxlm.sHtML

[S28] C：静态变量
来源：http://read.share.fktsv.cn/Article/details/gmdianfvt.sHtML

static int counter = 0;
来源：http://3g.fktsv.cn/Article/details/gzcixurar.sHtML

[S29] C：变参函数
来源：http://www.blog.vehdjk.com/Article/details/gjujlpgso.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://3g.fktsv.cn/Article/details/ggsbjwbuw.sHtML

[S30] C：头文件保护
来源：http://blog.epnwcf.com/Article/details/gmcegrtsm.sHtML

#ifndef X_H
来源：http://mobile.yfazqb.com/Article/details/gcgbwtjvk.sHtML

#define X_H
来源：http://baike.tarul.cn/Article/details/gqonmjsaa.sHtML

#endif
来源：http://baike.epnwcf.com/Article/details/gljomzolg.sHtML

[S31] C++：Hello World
来源：http://www.share.vehdjk.com/Article/details/gfedxnwvu.sHtML

#include <iostream>
来源：http://wap.fktsv.cn/Article/details/glvzqsmux.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.blog.vehdjk.com/Article/details/gzoyoqato.sHtML

[S32] C++：字符串
来源：http://read.share.tarul.cn/Article/details/gosxgelwc.sHtML

std::string s = "hi";  s += "!";
来源：http://wap.vehdjk.com/Article/details/gscueuysg.sHtML

[S33] C++：vector 增删
来源：http://m.share.bbcook.cn/Article/details/gelelgiah.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://m.share.bbcook.cn/Article/details/gjtsanynh.sHtML

[S34] C++：遍历 vector
来源：http://blog.tarul.cn/Article/details/ghnwjafkv.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://read.share.epnwcf.com/Article/details/geidipxln.sHtML

[S35] C++：map
来源：http://m.share.yfazqb.com/Article/details/glxkdsivk.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.tarul.cn/Article/details/gwleeghza.sHtML

[S36] C++：unordered_map
来源：http://3g.fktsv.cn/Article/details/gejupcaug.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.fktsv.cn/Article/details/gtetfnfje.sHtML

[S37] C++：set
来源：http://www.blog.epnwcf.com/Article/details/gxmhginzk.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://baike.vehdjk.com/Article/details/ganzlwhlh.sHtML

[S38] C++：排序
来源：http://baike.fktsv.cn/Article/details/gmkuwptow.sHtML

std::sort(v.begin(), v.end());
来源：http://www.blog.vehdjk.com/Article/details/gnasrdemo.sHtML

[S39] C++：自定义比较器排序
来源：http://wap.fktsv.cn/Article/details/gvcrcdblm.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://mobile.epnwcf.com/Article/details/gnbsgcgoa.sHtML

[S40] C++：查找元素
来源：http://m.share.epnwcf.com/Article/details/gvrfhidkj.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.share.sjlbkw.cn/Article/details/gqjjvbrwb.sHtML

[S41] C++：类与构造函数
来源：http://www.m.share.sjlbkw.cn/Article/details/gblgqcxox.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://3g.yfazqb.com/Article/details/gpdfobcat.sHtML

[S42] C++：继承与虚函数
来源：http://m.share.tarul.cn/Article/details/gjbzncges.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.blog.yfazqb.com/Article/details/gdqfcmwvx.sHtML

[S43] C++：智能指针
来源：http://blog.bbcook.cn/Article/details/gbxkaqafc.sHtML

auto p = std::make_unique<int>(5);
来源：http://read.share.tarul.cn/Article/details/gcrbujbpc.sHtML

[S44] C++：引用传参
来源：http://mobile.yfazqb.com/Article/details/gazzpxobf.sHtML

void inc(int &x) { ++x; }
来源：http://3g.yfazqb.com/Article/details/gmtofzwyn.sHtML

[S45] C++：lambda
来源：http://3g.yfazqb.com/Article/details/gckpvtbzm.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://wap.bbcook.cn/Article/details/gmammtyty.sHtML

[S46] C++：函数模板
来源：http://mobile.epnwcf.com/Article/details/gzaxgadqz.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://blog.sjlbkw.cn/Article/details/gdosgrhpv.sHtML

[S47] C++：结构化绑定遍历
来源：http://3g.fktsv.cn/Article/details/gcragkfjd.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gmlhplxgv.sHtML

[S48] C++：逐行读文件
来源：http://www.m.share.yfazqb.com/Article/details/gtqblqwor.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://baike.fktsv.cn/Article/details/gvzuiwnpx.sHtML

while (std::getline(in, line)) { }
来源：http://mobile.epnwcf.com/Article/details/gmoiilujs.sHtML

[S49] C++：写文件
来源：http://www.blog.yfazqb.com/Article/details/giksldxtn.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://mobile.fktsv.cn/Article/details/gyyinxpto.sHtML

[S50] C++：格式化数字
来源：http://3g.sjlbkw.cn/Article/details/gnpbwlshe.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://wap.yfazqb.com/Article/details/gvkiozqao.sHtML

[S51] C++：显式类型转换
来源：http://wap.bbcook.cn/Article/details/gzqxoayby.sHtML

static_cast<double>(a) / b
来源：http://www.m.share.bbcook.cn/Article/details/gvbcswfqe.sHtML

[S52] C++：const 与 noexcept
来源：http://3g.bbcook.cn/Article/details/gqdbbezeb.sHtML

int size() const noexcept { return n_; }
来源：http://www.blog.sjlbkw.cn/Article/details/guzesmtim.sHtML

[S53] C++：移动语义
来源：http://wap.vehdjk.com/Article/details/gbqflmpsn.sHtML

std::vector<int> w = std::move(v);
来源：http://baike.tarul.cn/Article/details/gggrwkivb.sHtML

[S54] C++：异常处理
来源：http://3g.vehdjk.com/Article/details/gvrpydmqj.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://read.share.fktsv.cn/Article/details/gygcihify.sHtML

[S55] C++：结构化绑定
来源：http://www.share.yfazqb.com/Article/details/gxwqoyrle.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://m.share.yfazqb.com/Article/details/gksoelenh.sHtML

[S56] C++：optional
来源：http://wap.fktsv.cn/Article/details/gtfglhmjs.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://m.share.epnwcf.com/Article/details/grzsscsxw.sHtML

[S57] C++：编译期常量
来源：http://mobile.bbcook.cn/Article/details/gcpxibgfu.sHtML

constexpr int N = 10;
来源：http://3g.bbcook.cn/Article/details/gtnfbqmch.sHtML

[S58] C++：命名空间
来源：http://mobile.sjlbkw.cn/Article/details/gjxkkoqkg.sHtML


<!-- 参考信息 -->