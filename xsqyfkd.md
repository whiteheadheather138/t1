代发 wailian999

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://mobile.bbcook.cn/Article/details/gbtaxoxml.sHtML

[Q90] 生成序号列
来源：http://baike.sjlbkw.cn/Article/details/ggjpibopl.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://blog.epnwcf.com/Article/details/gtrxsfbhn.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/gtqecytqs.sHtML

R. Bash 专题
来源：http://3g.bbcook.cn/Article/details/gqbeudfzg.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/grzuicoel.sHtML

[R01] shebang 与严格模式
来源：http://www.share.yfazqb.com/Article/details/gzzmfjkzu.sHtML

#!/usr/bin/env bash
来源：http://baike.epnwcf.com/Article/details/gqidkufde.sHtML

set -euo pipefail
来源：http://www.share.sjlbkw.cn/Article/details/gczmzgccs.sHtML

[R02] 变量赋值与使用
来源：http://wap.sjlbkw.cn/Article/details/gixazbrii.sHtML

name="Tom"; echo "$name"
来源：http://wap.tarul.cn/Article/details/gnvzoaoyu.sHtML

[R03] 只读变量
来源：http://mobile.bbcook.cn/Article/details/glynxhoma.sHtML

readonly PI=3.14
来源：http://3g.fktsv.cn/Article/details/gamqeklfs.sHtML

[R04] 位置参数
来源：http://www.blog.sjlbkw.cn/Article/details/gnxrdkkrm.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://wap.epnwcf.com/Article/details/gvaktyddn.sHtML

[R05] 参数默认值
来源：http://3g.sjlbkw.cn/Article/details/gupwgpcio.sHtML

name="${1:-default}"
来源：http://m.share.bbcook.cn/Article/details/gmxxahagm.sHtML

[R06] 判断命令是否存在
来源：http://www.m.share.fktsv.cn/Article/details/gkiwqwuxa.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.m.share.tarul.cn/Article/details/grinyaadg.sHtML

[R07] if 判断文件
来源：http://baike.tarul.cn/Article/details/gpwtyotto.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://read.share.epnwcf.com/Article/details/gecohtnox.sHtML

[R08] 数值比较
来源：http://mobile.fktsv.cn/Article/details/gefcqufix.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://3g.sjlbkw.cn/Article/details/gaxrzhpum.sHtML

[R09] 字符串比较
来源：http://www.share.vehdjk.com/Article/details/gbkdizhnt.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://read.share.bbcook.cn/Article/details/gjdinccch.sHtML

[R10] 正则匹配
来源：http://baike.tarul.cn/Article/details/gxnzxsdwr.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://wap.sjlbkw.cn/Article/details/gzrchdaco.sHtML

[R11] case 多分支
来源：http://baike.bbcook.cn/Article/details/gowdmzbfl.sHtML

case "$1" in
来源：http://blog.fktsv.cn/Article/details/goulmyhzr.sHtML

start) echo "启动" ;;
来源：http://www.m.share.epnwcf.com/Article/details/gxkhubckg.sHtML

stop)  echo "停止" ;;
来源：http://baike.sjlbkw.cn/Article/details/gzzmrjhei.sHtML

*)     echo "未知命令" ;;
来源：http://blog.vehdjk.com/Article/details/goriaenin.sHtML

esac
来源：http://3g.sjlbkw.cn/Article/details/ghsetjxez.sHtML

[R12] for 遍历文件
来源：http://wap.bbcook.cn/Article/details/gxumugada.sHtML

for f in *.txt; do echo "$f"; done
来源：http://baike.bbcook.cn/Article/details/gvtquwcmo.sHtML

[R13] for 计数循环
来源：http://3g.sjlbkw.cn/Article/details/gxagyvgeu.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://baike.epnwcf.com/Article/details/gdgwfbpto.sHtML

[R14] C 风格 for
来源：http://www.share.epnwcf.com/Article/details/gduizoatz.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://m.share.yfazqb.com/Article/details/gcusjppbc.sHtML

[R15] while 逐行读文件
来源：http://www.m.share.sjlbkw.cn/Article/details/gtzmyzdim.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://blog.sjlbkw.cn/Article/details/gdurseegl.sHtML

[R16] until 等待条件
来源：http://www.share.yfazqb.com/Article/details/gbvksbghi.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://m.share.bbcook.cn/Article/details/gjuumpbta.sHtML

[R17] 数组定义与取值
来源：http://www.blog.tarul.cn/Article/details/geexwmjol.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://blog.yfazqb.com/Article/details/gguutocnv.sHtML

[R18] 遍历数组
来源：http://baike.epnwcf.com/Article/details/giryrotbw.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://blog.yfazqb.com/Article/details/ggkmjqsmq.sHtML

[R19] 数组长度
来源：http://baike.sjlbkw.cn/Article/details/gllwtogii.sHtML

echo "${#arr[@]}"
来源：http://3g.fktsv.cn/Article/details/gioptddju.sHtML

[R20] 关联数组（字典）
来源：http://3g.sjlbkw.cn/Article/details/gkqgngztn.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://blog.sjlbkw.cn/Article/details/gtyavlyoz.sHtML

[R21] 字符串长度
来源：http://wap.vehdjk.com/Article/details/gkebvrfgv.sHtML

echo "${#s}"
来源：http://baike.sjlbkw.cn/Article/details/ghgxgouye.sHtML

[R22] 截取子串
来源：http://mobile.bbcook.cn/Article/details/gkxwabfbl.sHtML

echo "${s:0:5}"
来源：http://blog.tarul.cn/Article/details/ggjmlqeag.sHtML

[R23] 字符串替换
来源：http://read.share.sjlbkw.cn/Article/details/gvpcpticj.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.blog.tarul.cn/Article/details/gjwjsnygn.sHtML

[R24] 大小写转换
来源：http://m.share.vehdjk.com/Article/details/gxtiplpkv.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://mobile.fktsv.cn/Article/details/giozlywos.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.blog.vehdjk.com/Article/details/grolwzrcd.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.m.share.tarul.cn/Article/details/gitwwnwpr.sHtML

[R26] 命令替换
来源：http://read.share.epnwcf.com/Article/details/gsozrehbg.sHtML

now=$(date +%F); echo "$now"
来源：http://mobile.epnwcf.com/Article/details/gtsbiktaa.sHtML

[R27] 算术展开
来源：http://www.m.share.yfazqb.com/Article/details/gldzjkjxr.sHtML

echo $((1 + 2 * 3))
来源：http://www.share.vehdjk.com/Article/details/gyaseange.sHtML

[R28] 浮点运算
来源：http://3g.fktsv.cn/Article/details/gxwzhpvug.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.share.tarul.cn/Article/details/gunnlxkwo.sHtML

[R29] 定义函数
来源：http://mobile.yfazqb.com/Article/details/gygqvfyep.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://m.share.yfazqb.com/Article/details/gujwqclan.sHtML

[R30] 函数返回状态码
来源：http://www.share.bbcook.cn/Article/details/gioakjbkf.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://wap.epnwcf.com/Article/details/gjfkbhggc.sHtML

[R31] 局部变量
来源：http://3g.fktsv.cn/Article/details/gfqatastg.sHtML

f() { local x=1; echo "$x"; }
来源：http://blog.epnwcf.com/Article/details/gdqefkhxw.sHtML

[R32] 参数个数校验
来源：http://read.share.epnwcf.com/Article/details/gruaosoik.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.blog.vehdjk.com/Article/details/gscbzivth.sHtML

[R33] 捕获错误并提示行号
来源：http://www.share.bbcook.cn/Article/details/gdfzdmetd.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://mobile.fktsv.cn/Article/details/ggbstamvx.sHtML

[R34] 退出时清理
来源：http://3g.yfazqb.com/Article/details/ghgohnbri.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.share.yfazqb.com/Article/details/gfajkmtaw.sHtML

[R35] 后台执行并等待
来源：http://baike.bbcook.cn/Article/details/gadcjgogl.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.share.yfazqb.com/Article/details/gnfxvkyuy.sHtML

[R36] 并发执行多个任务
来源：http://mobile.vehdjk.com/Article/details/gtnpxzyra.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://3g.epnwcf.com/Article/details/ggdbyuzbr.sHtML

[R37] 把输出赋给变量
来源：http://www.m.share.vehdjk.com/Article/details/gldyxqafa.sHtML

files=$(ls -1)
来源：http://wap.tarul.cn/Article/details/gdfhngjjt.sHtML

[R38] 管道串联
来源：http://www.m.share.bbcook.cn/Article/details/gjcffxzui.sHtML

cat a.txt | grep -i error | wc -l
来源：http://blog.sjlbkw.cn/Article/details/gzqewjhzp.sHtML

[R39] 重定向标准输出与错误
来源：http://www.m.share.yfazqb.com/Article/details/gwiezbpiz.sHtML

cmd > out.log 2>&1
来源：http://www.blog.tarul.cn/Article/details/gmnspgrtd.sHtML

[R40] 追加写日志
来源：http://www.m.share.tarul.cn/Article/details/gvupihldh.sHtML

echo "log" >> out.log
来源：http://read.share.epnwcf.com/Article/details/gsvmopzky.sHtML

[R41] 丢弃输出
来源：http://blog.vehdjk.com/Article/details/gbccfpepf.sHtML

cmd >/dev/null 2>&1
来源：http://wap.vehdjk.com/Article/details/gnlhldqtc.sHtML

[R42] 输入重定向
来源：http://m.share.yfazqb.com/Article/details/gtwmjscbm.sHtML

wc -l < a.txt
来源：http://www.blog.tarul.cn/Article/details/gkxojhmhr.sHtML

[R43] 按名字查找文件
来源：http://baike.epnwcf.com/Article/details/gfvemlzzc.sHtML

find . -name "*.log" -type f
来源：http://mobile.sjlbkw.cn/Article/details/govpjvudy.sHtML

[R44] 按修改时间查找
来源：http://www.blog.tarul.cn/Article/details/gcuzlnelz.sHtML

find . -mtime -7 -type f
来源：http://wap.tarul.cn/Article/details/gismzddor.sHtML

[R45] 批量删除
来源：http://m.share.bbcook.cn/Article/details/gstsjycpd.sHtML

find . -name "*.tmp" -delete
来源：http://wap.vehdjk.com/Article/details/gndewjlzm.sHtML

[R46] 递归替换文件内容
来源：http://www.blog.yfazqb.com/Article/details/glqgrclca.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mobile.fktsv.cn/Article/details/galijhwlo.sHtML

[R47] sed 单行替换
来源：http://blog.tarul.cn/Article/details/griwamcvg.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.m.share.sjlbkw.cn/Article/details/gsxhkktce.sHtML

[R48] awk 取指定列
来源：http://baike.vehdjk.com/Article/details/gawckctqs.sHtML

awk '{print $1, $3}' a.txt
来源：http://m.share.bbcook.cn/Article/details/gtshrasof.sHtML

[R49] awk 带条件
来源：http://www.m.share.sjlbkw.cn/Article/details/geerdyrkn.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://baike.vehdjk.com/Article/details/ggbjwhhwf.sHtML

[R50] awk 求和
来源：http://www.blog.epnwcf.com/Article/details/gwolxmjdm.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://3g.sjlbkw.cn/Article/details/gpmpohhxr.sHtML

[R51] 排序去重取前几
来源：http://m.share.tarul.cn/Article/details/gviywhimw.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://m.share.bbcook.cn/Article/details/glwxolqfo.sHtML

[R52] 统计行数
来源：http://3g.sjlbkw.cn/Article/details/glzjxrtbw.sHtML

wc -l a.txt
来源：http://baike.yfazqb.com/Article/details/gnpasfgzd.sHtML

[R53] 查看文件头与实时尾
来源：http://www.blog.sjlbkw.cn/Article/details/gxvplblpl.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.share.sjlbkw.cn/Article/details/ggmnqvgna.sHtML

[R54] 比较两个文件
来源：http://read.share.yfazqb.com/Article/details/gtlmpwcju.sHtML

diff a.txt b.txt
来源：http://baike.yfazqb.com/Article/details/gcojvpdrg.sHtML

[R55] 压缩与解压
来源：http://mobile.tarul.cn/Article/details/gxsklvcso.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://m.share.tarul.cn/Article/details/gtdwjxpzx.sHtML

[R56] 远程拷贝
来源：http://www.share.bbcook.cn/Article/details/gjahdrqul.sHtML

scp file user@host:/path/
来源：http://3g.yfazqb.com/Article/details/gwowqqrbk.sHtML

[R57] 远程执行命令
来源：http://m.share.yfazqb.com/Article/details/gdwzmqnde.sHtML

ssh user@host 'uptime'
来源：http://3g.fktsv.cn/Article/details/gqpomqorn.sHtML

[R58] 下载文件
来源：http://www.m.share.vehdjk.com/Article/details/gszwwsjgt.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.blog.epnwcf.com/Article/details/glnhjshbl.sHtML

[R59] 发 POST JSON
来源：http://mobile.vehdjk.com/Article/details/guntcctwr.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://baike.vehdjk.com/Article/details/gajeqlpom.sHtML

[R60] 只看 HTTP 状态码
来源：http://wap.vehdjk.com/Article/details/gcbvugsni.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://m.share.vehdjk.com/Article/details/gzveievzm.sHtML

[R61] 磁盘占用
来源：http://www.share.fktsv.cn/Article/details/giqvvhlqx.sHtML

df -h;  du -sh *
来源：http://3g.fktsv.cn/Article/details/ghkbdqgvv.sHtML

[R62] 找最占空间的文件
来源：http://baike.epnwcf.com/Article/details/gzbfnnsmb.sHtML

du -ah . | sort -rh | head -10
来源：http://blog.vehdjk.com/Article/details/gonnjbhvo.sHtML

[R63] 内存与进程
来源：http://baike.sjlbkw.cn/Article/details/gjnuwinha.sHtML

free -h;  ps aux | grep nginx
来源：http://www.blog.yfazqb.com/Article/details/goqeqvqoz.sHtML

[R64] 结束进程
来源：http://m.share.epnwcf.com/Article/details/gikznbrqq.sHtML

kill -9 $(pgrep -f app.py)
来源：http://blog.bbcook.cn/Article/details/gkdorfxkr.sHtML

[R65] 查看端口占用
来源：http://blog.epnwcf.com/Article/details/gslyfderv.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://baike.bbcook.cn/Article/details/gpctdmyee.sHtML

[R66] 定时任务
来源：http://www.blog.tarul.cn/Article/details/geoujczos.sHtML

crontab -e;  crontab -l
来源：http://www.m.share.fktsv.cn/Article/details/gpmrcuxcn.sHtML

[R67] 生成随机十六进制串
来源：http://baike.vehdjk.com/Article/details/gwqurqeji.sHtML

openssl rand -hex 16
来源：http://read.share.yfazqb.com/Article/details/gdhhcrqch.sHtML

[R68] 计算文件校验值
来源：http://www.share.yfazqb.com/Article/details/gvmftuvkp.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://blog.bbcook.cn/Article/details/gqkqkfnaa.sHtML

[R69] 生成随机密码
来源：http://mobile.fktsv.cn/Article/details/gwncppwef.sHtML

head -c 16 /dev/urandom | base64
来源：http://m.share.vehdjk.com/Article/details/gtpnoaaok.sHtML

[R70] 时间戳与互转
来源：http://read.share.sjlbkw.cn/Article/details/ggxcrskzw.sHtML

date +%s;  date -d @1700000000
来源：http://read.share.tarul.cn/Article/details/gzqqcbmfk.sHtML

[R71] 日期格式化
来源：http://blog.tarul.cn/Article/details/goupyiiio.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.blog.yfazqb.com/Article/details/gacrpgujc.sHtML

[R72] 等待端口就绪
来源：http://www.m.share.bbcook.cn/Article/details/gdsecengy.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.blog.sjlbkw.cn/Article/details/ghlzivfpy.sHtML

[R73] 分割大日志
来源：http://www.m.share.tarul.cn/Article/details/gtcxynmjl.sHtML

split -l 1000 big.log part_
来源：http://www.blog.yfazqb.com/Article/details/gqikkvoqp.sHtML

[R74] 批量重命名
来源：http://wap.bbcook.cn/Article/details/gfxwscfwc.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://m.share.tarul.cn/Article/details/gnihdbypk.sHtML

[R75] 导出环境变量
来源：http://www.share.sjlbkw.cn/Article/details/gqlfwsbun.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.m.share.tarul.cn/Article/details/gxwmpdtxo.sHtML

[R76] 使用临时文件
来源：http://read.share.bbcook.cn/Article/details/gbkssujbd.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://wap.epnwcf.com/Article/details/gowerkhwi.sHtML

[R77] 读取用户输入
来源：http://wap.tarul.cn/Article/details/ghcdpblao.sHtML

read -rp "请输入: " ans
来源：http://blog.tarul.cn/Article/details/glcmwhekq.sHtML

[R78] 交互式菜单
来源：http://wap.yfazqb.com/Article/details/gnodxzrpn.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://wap.vehdjk.com/Article/details/ghqkihtjg.sHtML

[R79] 解析命令行选项
来源：http://baike.epnwcf.com/Article/details/gwzyinvrc.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wap.fktsv.cn/Article/details/gkttuvanx.sHtML

[R80] 查看脚本执行耗时
来源：http://www.blog.sjlbkw.cn/Article/details/ggaajsmyb.sHtML

time ./run.sh
来源：http://m.share.sjlbkw.cn/Article/details/gfucndnbh.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/gvdkenmab.sHtML

S. C / C++ 专题
来源：http://blog.sjlbkw.cn/Article/details/gmbtfyviq.sHtML

================================================================================
来源：http://www.m.share.tarul.cn/Article/details/gvwezwbou.sHtML

[S01] C：Hello World
来源：http://www.m.share.fktsv.cn/Article/details/govlmwvfj.sHtML

#include <stdio.h>
来源：http://mobile.sjlbkw.cn/Article/details/gizmbvxdy.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://m.share.sjlbkw.cn/Article/details/gtnhqpltc.sHtML

[S02] C：变量与格式化输出
来源：http://www.blog.tarul.cn/Article/details/gyormtrbq.sHtML

int a = 10; printf("%d\n", a);
来源：http://baike.epnwcf.com/Article/details/gskhqayhl.sHtML

[S03] C：读入整数
来源：http://www.m.share.vehdjk.com/Article/details/gygusmsel.sHtML

int x; scanf("%d", &x);
来源：http://baike.bbcook.cn/Article/details/gffkqewho.sHtML

[S04] C：字符串复制
来源：http://www.blog.yfazqb.com/Article/details/gltoimsvp.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.m.share.yfazqb.com/Article/details/gqxlguwym.sHtML

[S05] C：字符串长度
来源：http://www.blog.sjlbkw.cn/Article/details/gznfjbvoz.sHtML

strlen(s)
来源：http://wap.tarul.cn/Article/details/gtterzbon.sHtML

[S06] C：字符串比较
来源：http://blog.sjlbkw.cn/Article/details/gopfwwkrc.sHtML

strcmp(a, b) == 0
来源：http://m.share.epnwcf.com/Article/details/gcxfbpmqx.sHtML

[S07] C：数组遍历求和
来源：http://blog.vehdjk.com/Article/details/gyarbzbhp.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://m.share.yfazqb.com/Article/details/genapwtne.sHtML

[S08] C：动态内存分配与释放
来源：http://www.share.yfazqb.com/Article/details/gzqfprndv.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://read.share.epnwcf.com/Article/details/gczvtwbhk.sHtML

[S09] C：结构体定义与初始化
来源：http://www.blog.vehdjk.com/Article/details/ggyrajlgt.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.m.share.vehdjk.com/Article/details/gzinkbyub.sHtML

[S10] C：指针与解引用
来源：http://baike.vehdjk.com/Article/details/gemjepwaq.sHtML

int *p = &a;  *p = 5;
来源：http://www.blog.vehdjk.com/Article/details/gcwwfbemr.sHtML

[S11] C：逐行读文件
来源：http://read.share.bbcook.cn/Article/details/gffjxvyjj.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://wap.sjlbkw.cn/Article/details/gdgfdnyif.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://mobile.fktsv.cn/Article/details/gkihocpnl.sHtML

fclose(f);
来源：http://wap.fktsv.cn/Article/details/gpsoextlc.sHtML

[S12] C：写文件
来源：http://www.m.share.vehdjk.com/Article/details/gaxnmplbn.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://read.share.bbcook.cn/Article/details/gsdeqmtdq.sHtML

[S13] C：宏定义
来源：http://www.blog.yfazqb.com/Article/details/gltvaffte.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wap.yfazqb.com/Article/details/gtbkvxtyi.sHtML

[S14] C：枚举
来源：http://read.share.epnwcf.com/Article/details/gbqusnjdg.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://m.share.epnwcf.com/Article/details/gkkmostsu.sHtML

[S15] C：类型转换
来源：http://blog.yfazqb.com/Article/details/gqtjzdbiy.sHtML

(double) a / b
来源：http://3g.bbcook.cn/Article/details/glrrglmiq.sHtML

[S16] C：位操作置位
来源：http://read.share.yfazqb.com/Article/details/gdhrntaeq.sHtML

x |= (1 << 3);
来源：http://www.share.fktsv.cn/Article/details/gxmudktjb.sHtML

[S17] C：安全拼接字符串
来源：http://wap.vehdjk.com/Article/details/gpinnrfta.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://baike.epnwcf.com/Article/details/gnowdzgkn.sHtML

[S18] C：命令行参数
来源：http://baike.tarul.cn/Article/details/gfmyjqupw.sHtML

int main(int argc, char **argv)
来源：http://read.share.bbcook.cn/Article/details/gxybzmteb.sHtML

[S19] C：快速排序
来源：http://www.share.fktsv.cn/Article/details/gqfeuxktt.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.share.sjlbkw.cn/Article/details/gggqsfbbm.sHtML

[S20] C：二分查找
来源：http://blog.bbcook.cn/Article/details/gklfdippc.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://3g.epnwcf.com/Article/details/gkcqpejla.sHtML

[S21] C：字符类别判断
来源：http://www.share.bbcook.cn/Article/details/gtvackvpd.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.blog.fktsv.cn/Article/details/gmicvhvvt.sHtML

[S22] C：字符串转数字
来源：http://blog.yfazqb.com/Article/details/gvfvvwaub.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://wap.epnwcf.com/Article/details/ghlmaubpi.sHtML

[S23] C：随机数
来源：http://www.share.bbcook.cn/Article/details/gljttcbns.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://baike.sjlbkw.cn/Article/details/gywckjyji.sHtML

[S24] C：获取本地时间
来源：http://blog.epnwcf.com/Article/details/glsfozlvy.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://blog.bbcook.cn/Article/details/gtyeufqhp.sHtML

[S25] C：内存拷贝
来源：http://www.share.sjlbkw.cn/Article/details/gkmmrwdge.sHtML

memcpy(dst, src, n);
来源：http://www.m.share.epnwcf.com/Article/details/gvyhibxri.sHtML

[S26] C：内存清零
来源：http://www.share.sjlbkw.cn/Article/details/gqvwsomva.sHtML

memset(a, 0, sizeof a);
来源：http://wap.fktsv.cn/Article/details/ghhilwtsi.sHtML

[S27] C：定义常量
来源：http://www.m.share.bbcook.cn/Article/details/galosvekb.sHtML

const double PI = 3.14159;
来源：http://3g.sjlbkw.cn/Article/details/gsyuovtbn.sHtML

[S28] C：静态变量
来源：http://baike.epnwcf.com/Article/details/giaobnqtj.sHtML

static int counter = 0;
来源：http://www.m.share.yfazqb.com/Article/details/gaodlqjga.sHtML

[S29] C：变参函数
来源：http://www.share.epnwcf.com/Article/details/ggfxnyujc.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://blog.fktsv.cn/Article/details/gqwnynqal.sHtML

[S30] C：头文件保护
来源：http://baike.tarul.cn/Article/details/gaasmvvjh.sHtML

#ifndef X_H
来源：http://www.share.fktsv.cn/Article/details/gbcchrthu.sHtML

#define X_H
来源：http://baike.fktsv.cn/Article/details/grusiogvn.sHtML

#endif
来源：http://www.share.yfazqb.com/Article/details/geghraubn.sHtML

[S31] C++：Hello World
来源：http://blog.yfazqb.com/Article/details/gqzfbalrr.sHtML

#include <iostream>
来源：http://www.m.share.vehdjk.com/Article/details/gjzaprbkn.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://baike.sjlbkw.cn/Article/details/gpiwnmsgm.sHtML

[S32] C++：字符串
来源：http://m.share.fktsv.cn/Article/details/gqgiqmfzx.sHtML

std::string s = "hi";  s += "!";
来源：http://wap.yfazqb.com/Article/details/gzhhvqaul.sHtML

[S33] C++：vector 增删
来源：http://wap.vehdjk.com/Article/details/gdcepapol.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://m.share.vehdjk.com/Article/details/gylrhgnlk.sHtML

[S34] C++：遍历 vector
来源：http://wap.sjlbkw.cn/Article/details/gbcjzvnaj.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.m.share.tarul.cn/Article/details/golycqiue.sHtML

[S35] C++：map
来源：http://3g.fktsv.cn/Article/details/gqwvhkbqm.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.epnwcf.com/Article/details/gyteqqjto.sHtML

[S36] C++：unordered_map
来源：http://www.blog.bbcook.cn/Article/details/gvgkxicbx.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.fktsv.cn/Article/details/gbnscdiks.sHtML

[S37] C++：set
来源：http://m.share.yfazqb.com/Article/details/gxhythxaq.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://blog.yfazqb.com/Article/details/gjndalyvi.sHtML

[S38] C++：排序
来源：http://mobile.yfazqb.com/Article/details/gnnxjnsqu.sHtML

std::sort(v.begin(), v.end());
来源：http://mobile.yfazqb.com/Article/details/ggcphmznu.sHtML

[S39] C++：自定义比较器排序
来源：http://blog.sjlbkw.cn/Article/details/gmblfnkty.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://mobile.epnwcf.com/Article/details/gmajnlzoi.sHtML

[S40] C++：查找元素
来源：http://www.blog.tarul.cn/Article/details/gxpebxkpt.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.blog.fktsv.cn/Article/details/gvwfldrmq.sHtML

[S41] C++：类与构造函数
来源：http://3g.yfazqb.com/Article/details/gnjikrttg.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://m.share.tarul.cn/Article/details/giuqcybng.sHtML

[S42] C++：继承与虚函数
来源：http://www.share.epnwcf.com/Article/details/gsbedndie.sHtML

class B : public Base { public: void f() override {} };
来源：http://m.share.sjlbkw.cn/Article/details/gcxwerbzf.sHtML

[S43] C++：智能指针
来源：http://www.m.share.vehdjk.com/Article/details/grsyaslme.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.m.share.bbcook.cn/Article/details/gcrwrqftj.sHtML

[S44] C++：引用传参
来源：http://wap.bbcook.cn/Article/details/gwsavmbyh.sHtML

void inc(int &x) { ++x; }
来源：http://read.share.yfazqb.com/Article/details/gcwqepohy.sHtML

[S45] C++：lambda
来源：http://www.m.share.sjlbkw.cn/Article/details/gnvpgliwb.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.blog.bbcook.cn/Article/details/gxpfgxjlm.sHtML

[S46] C++：函数模板
来源：http://m.share.sjlbkw.cn/Article/details/gygtumkxo.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.blog.vehdjk.com/Article/details/gqqylwbqj.sHtML

[S47] C++：结构化绑定遍历
来源：http://m.share.bbcook.cn/Article/details/ggpzmirvy.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://m.share.tarul.cn/Article/details/gmmftgcxt.sHtML

[S48] C++：逐行读文件
来源：http://mobile.tarul.cn/Article/details/gizvzcvpi.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://3g.sjlbkw.cn/Article/details/giozabkcj.sHtML

while (std::getline(in, line)) { }
来源：http://www.m.share.vehdjk.com/Article/details/gintacskt.sHtML

[S49] C++：写文件
来源：http://mobile.yfazqb.com/Article/details/glqcrwekp.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.m.share.tarul.cn/Article/details/ghbdgkgrn.sHtML

[S50] C++：格式化数字
来源：http://wap.tarul.cn/Article/details/gpflfjacg.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.share.epnwcf.com/Article/details/gyrrnbsue.sHtML

[S51] C++：显式类型转换
来源：http://mobile.epnwcf.com/Article/details/ghzwnywgr.sHtML

static_cast<double>(a) / b
来源：http://read.share.bbcook.cn/Article/details/gokxoyezu.sHtML

[S52] C++：const 与 noexcept
来源：http://read.share.vehdjk.com/Article/details/gfowfptey.sHtML

int size() const noexcept { return n_; }
来源：http://wap.vehdjk.com/Article/details/gcdhaxihh.sHtML

[S53] C++：移动语义
来源：http://www.share.tarul.cn/Article/details/giwvtbpff.sHtML

std::vector<int> w = std::move(v);
来源：http://m.share.vehdjk.com/Article/details/gmeufvvaq.sHtML

[S54] C++：异常处理
来源：http://www.m.share.tarul.cn/Article/details/gtxsikvsx.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://3g.bbcook.cn/Article/details/gapwnjxnm.sHtML

[S55] C++：结构化绑定
来源：http://www.m.share.vehdjk.com/Article/details/gccvgktcq.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.share.fktsv.cn/Article/details/ggjsjlrue.sHtML

[S56] C++：optional
来源：http://www.blog.fktsv.cn/Article/details/ghsekzrhh.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.blog.sjlbkw.cn/Article/details/guptwgpjw.sHtML

[S57] C++：编译期常量
来源：http://baike.bbcook.cn/Article/details/gxemnshrl.sHtML

constexpr int N = 10;
来源：http://3g.epnwcf.com/Article/details/gkhvrefcj.sHtML

[S58] C++：命名空间
来源：http://m.share.sjlbkw.cn/Article/details/geiigixew.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.m.share.sjlbkw.cn/Article/details/gxwygwtin.sHtML

[S59] C++：静态断言
来源：http://www.blog.sjlbkw.cn/Article/details/gykhcayzv.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://3g.bbcook.cn/Article/details/gxhgyuxli.sHtML

[S60] C++：遍历并删除元素
来源：http://www.share.sjlbkw.cn/Article/details/gszaehjms.sHtML


<!-- 参考信息 -->