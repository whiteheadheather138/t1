代发 wailian999

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.blog.vehdjk.com/Article/details/genfcheur.sHtML

[Q90] 生成序号列
来源：http://blog.fktsv.cn/Article/details/gtnpsydlz.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://wap.tarul.cn/Article/details/gfftxjgmo.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/gapfhxxif.sHtML

R. Bash 专题
来源：http://baike.vehdjk.com/Article/details/gdnrvywsl.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/gwfvbmgwu.sHtML

[R01] shebang 与严格模式
来源：http://www.blog.epnwcf.com/Article/details/geffqtukk.sHtML

#!/usr/bin/env bash
来源：http://blog.vehdjk.com/Article/details/gbwyxqqua.sHtML

set -euo pipefail
来源：http://www.m.share.vehdjk.com/Article/details/gwfqrazxt.sHtML

[R02] 变量赋值与使用
来源：http://wap.yfazqb.com/Article/details/gdzvfzvfm.sHtML

name="Tom"; echo "$name"
来源：http://read.share.fktsv.cn/Article/details/ggusmiqkx.sHtML

[R03] 只读变量
来源：http://read.share.vehdjk.com/Article/details/gtzbhbqan.sHtML

readonly PI=3.14
来源：http://www.blog.epnwcf.com/Article/details/gngtnjwes.sHtML

[R04] 位置参数
来源：http://wap.fktsv.cn/Article/details/ghyujrtmj.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://wap.bbcook.cn/Article/details/gpijtzkyu.sHtML

[R05] 参数默认值
来源：http://3g.yfazqb.com/Article/details/gewgfuewx.sHtML

name="${1:-default}"
来源：http://www.m.share.epnwcf.com/Article/details/gdvgmgaba.sHtML

[R06] 判断命令是否存在
来源：http://www.share.fktsv.cn/Article/details/gfhvnzvrz.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://baike.bbcook.cn/Article/details/gspjdjpgk.sHtML

[R07] if 判断文件
来源：http://www.m.share.yfazqb.com/Article/details/gialvycdt.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://mobile.tarul.cn/Article/details/gbnzaywjx.sHtML

[R08] 数值比较
来源：http://www.share.fktsv.cn/Article/details/gqybkvmpj.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://3g.yfazqb.com/Article/details/gdgujfuhn.sHtML

[R09] 字符串比较
来源：http://3g.epnwcf.com/Article/details/gemqrxogz.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://3g.yfazqb.com/Article/details/gbvyhrema.sHtML

[R10] 正则匹配
来源：http://www.blog.epnwcf.com/Article/details/gtiwyvnra.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://mobile.fktsv.cn/Article/details/gcxuhwcis.sHtML

[R11] case 多分支
来源：http://baike.yfazqb.com/Article/details/gcryrgvwm.sHtML

case "$1" in
来源：http://3g.vehdjk.com/Article/details/gysqvfvyi.sHtML

start) echo "启动" ;;
来源：http://m.share.fktsv.cn/Article/details/gthpuhifa.sHtML

stop)  echo "停止" ;;
来源：http://mobile.sjlbkw.cn/Article/details/gcdblxdwg.sHtML

*)     echo "未知命令" ;;
来源：http://m.share.fktsv.cn/Article/details/gyvkxeotf.sHtML

esac
来源：http://blog.sjlbkw.cn/Article/details/gbcpbkrja.sHtML

[R12] for 遍历文件
来源：http://blog.sjlbkw.cn/Article/details/gibpdwxlc.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.blog.vehdjk.com/Article/details/gbsiyxbjh.sHtML

[R13] for 计数循环
来源：http://mobile.sjlbkw.cn/Article/details/gvnniiwng.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://m.share.yfazqb.com/Article/details/ghknpwjkr.sHtML

[R14] C 风格 for
来源：http://m.share.yfazqb.com/Article/details/gkpfpskbl.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.share.vehdjk.com/Article/details/gjhivsief.sHtML

[R15] while 逐行读文件
来源：http://3g.vehdjk.com/Article/details/gvemgdomc.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://mobile.fktsv.cn/Article/details/gqnhsktgw.sHtML

[R16] until 等待条件
来源：http://3g.sjlbkw.cn/Article/details/gljjvsfxu.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://m.share.fktsv.cn/Article/details/gdrdwjxun.sHtML

[R17] 数组定义与取值
来源：http://www.blog.sjlbkw.cn/Article/details/gozwavnyd.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://m.share.sjlbkw.cn/Article/details/grnwcuxlh.sHtML

[R18] 遍历数组
来源：http://mobile.fktsv.cn/Article/details/gjbbripxh.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.m.share.fktsv.cn/Article/details/giykdcryn.sHtML

[R19] 数组长度
来源：http://mobile.fktsv.cn/Article/details/gfrdyxpol.sHtML

echo "${#arr[@]}"
来源：http://wap.vehdjk.com/Article/details/gxeqrjlue.sHtML

[R20] 关联数组（字典）
来源：http://www.blog.sjlbkw.cn/Article/details/gufspanml.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://wap.yfazqb.com/Article/details/gbheidanq.sHtML

[R21] 字符串长度
来源：http://m.share.epnwcf.com/Article/details/goqgpvgiy.sHtML

echo "${#s}"
来源：http://www.m.share.bbcook.cn/Article/details/gfzjseiwo.sHtML

[R22] 截取子串
来源：http://wap.tarul.cn/Article/details/gxemzczzg.sHtML

echo "${s:0:5}"
来源：http://m.share.sjlbkw.cn/Article/details/gztmjeidz.sHtML

[R23] 字符串替换
来源：http://blog.fktsv.cn/Article/details/gcachigol.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://blog.epnwcf.com/Article/details/grxarobwu.sHtML

[R24] 大小写转换
来源：http://mobile.fktsv.cn/Article/details/gyymdevdu.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.m.share.tarul.cn/Article/details/guhxcnjwt.sHtML

[R25] 去后缀 / 去前缀
来源：http://baike.yfazqb.com/Article/details/gedcarrnj.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://read.share.tarul.cn/Article/details/gjlvizjez.sHtML

[R26] 命令替换
来源：http://www.share.bbcook.cn/Article/details/gbuxweblb.sHtML

now=$(date +%F); echo "$now"
来源：http://baike.yfazqb.com/Article/details/gxvccnszj.sHtML

[R27] 算术展开
来源：http://m.share.fktsv.cn/Article/details/gogpeorbx.sHtML

echo $((1 + 2 * 3))
来源：http://www.share.tarul.cn/Article/details/gqpcwzxgz.sHtML

[R28] 浮点运算
来源：http://mobile.yfazqb.com/Article/details/gbtmxrlzd.sHtML

echo "scale=2; 10/3" | bc
来源：http://m.share.fktsv.cn/Article/details/gypnuokvv.sHtML

[R29] 定义函数
来源：http://wap.vehdjk.com/Article/details/gjfznjllm.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://blog.tarul.cn/Article/details/gwvxauhtm.sHtML

[R30] 函数返回状态码
来源：http://mobile.yfazqb.com/Article/details/gzloqtxzm.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://m.share.yfazqb.com/Article/details/gvffbgpox.sHtML

[R31] 局部变量
来源：http://3g.epnwcf.com/Article/details/gmzbvxzne.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.share.tarul.cn/Article/details/gwlweiwww.sHtML

[R32] 参数个数校验
来源：http://3g.bbcook.cn/Article/details/gjerlvtyu.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://wap.fktsv.cn/Article/details/gllotqgkw.sHtML

[R33] 捕获错误并提示行号
来源：http://3g.fktsv.cn/Article/details/gzvysutla.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://blog.tarul.cn/Article/details/gzgzlpmhy.sHtML

[R34] 退出时清理
来源：http://wap.bbcook.cn/Article/details/gvigcmdhb.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.tarul.cn/Article/details/gcgheljnw.sHtML

[R35] 后台执行并等待
来源：http://baike.sjlbkw.cn/Article/details/garbmlash.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://wap.bbcook.cn/Article/details/ggevurmuz.sHtML

[R36] 并发执行多个任务
来源：http://blog.vehdjk.com/Article/details/gnyysajcj.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.m.share.tarul.cn/Article/details/gjxukmodp.sHtML

[R37] 把输出赋给变量
来源：http://www.blog.yfazqb.com/Article/details/glrnriyip.sHtML

files=$(ls -1)
来源：http://read.share.fktsv.cn/Article/details/gorfuixuu.sHtML

[R38] 管道串联
来源：http://read.share.epnwcf.com/Article/details/gyalsmegt.sHtML

cat a.txt | grep -i error | wc -l
来源：http://m.share.fktsv.cn/Article/details/gcfrjiyvx.sHtML

[R39] 重定向标准输出与错误
来源：http://3g.yfazqb.com/Article/details/goviaqxzb.sHtML

cmd > out.log 2>&1
来源：http://www.blog.tarul.cn/Article/details/gefqqefow.sHtML

[R40] 追加写日志
来源：http://m.share.fktsv.cn/Article/details/ganoaauai.sHtML

echo "log" >> out.log
来源：http://www.m.share.epnwcf.com/Article/details/giqdlagei.sHtML

[R41] 丢弃输出
来源：http://www.share.yfazqb.com/Article/details/gqpindszj.sHtML

cmd >/dev/null 2>&1
来源：http://m.share.bbcook.cn/Article/details/gfjdiadbb.sHtML

[R42] 输入重定向
来源：http://www.share.fktsv.cn/Article/details/gcreivsuk.sHtML

wc -l < a.txt
来源：http://m.share.epnwcf.com/Article/details/gyibaxkll.sHtML

[R43] 按名字查找文件
来源：http://read.share.fktsv.cn/Article/details/gnxsuvpnk.sHtML

find . -name "*.log" -type f
来源：http://baike.fktsv.cn/Article/details/guvasgexi.sHtML

[R44] 按修改时间查找
来源：http://baike.fktsv.cn/Article/details/gaopecyho.sHtML

find . -mtime -7 -type f
来源：http://3g.bbcook.cn/Article/details/gscpztzme.sHtML

[R45] 批量删除
来源：http://www.share.epnwcf.com/Article/details/gwjvhdjdy.sHtML

find . -name "*.tmp" -delete
来源：http://read.share.epnwcf.com/Article/details/gqffevjhv.sHtML

[R46] 递归替换文件内容
来源：http://www.m.share.sjlbkw.cn/Article/details/gjjoikiuv.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://wap.tarul.cn/Article/details/geplhoqew.sHtML

[R47] sed 单行替换
来源：http://baike.tarul.cn/Article/details/glvphvdtp.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.share.epnwcf.com/Article/details/gxipionyr.sHtML

[R48] awk 取指定列
来源：http://mobile.fktsv.cn/Article/details/gpywhxvef.sHtML

awk '{print $1, $3}' a.txt
来源：http://read.share.epnwcf.com/Article/details/godhpjker.sHtML

[R49] awk 带条件
来源：http://baike.fktsv.cn/Article/details/gtpcmkrza.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.share.tarul.cn/Article/details/gmntnlmfu.sHtML

[R50] awk 求和
来源：http://wap.bbcook.cn/Article/details/gynwilzrl.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://mobile.epnwcf.com/Article/details/ggwwlmdbo.sHtML

[R51] 排序去重取前几
来源：http://www.m.share.sjlbkw.cn/Article/details/gkautrzcj.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://baike.fktsv.cn/Article/details/ghsxaxqhw.sHtML

[R52] 统计行数
来源：http://www.share.tarul.cn/Article/details/gwtnkaeuo.sHtML

wc -l a.txt
来源：http://m.share.sjlbkw.cn/Article/details/gdcfymjye.sHtML

[R53] 查看文件头与实时尾
来源：http://wap.fktsv.cn/Article/details/gbwjelozm.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://wap.bbcook.cn/Article/details/gkbwuboqg.sHtML

[R54] 比较两个文件
来源：http://www.m.share.sjlbkw.cn/Article/details/gdmiozudb.sHtML

diff a.txt b.txt
来源：http://blog.bbcook.cn/Article/details/gilahrudw.sHtML

[R55] 压缩与解压
来源：http://3g.vehdjk.com/Article/details/gpykdhrow.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://blog.tarul.cn/Article/details/geenontet.sHtML

[R56] 远程拷贝
来源：http://3g.tarul.cn/Article/details/gdvgfldfs.sHtML

scp file user@host:/path/
来源：http://m.share.yfazqb.com/Article/details/gjoomptsg.sHtML

[R57] 远程执行命令
来源：http://mobile.bbcook.cn/Article/details/gpnfsltya.sHtML

ssh user@host 'uptime'
来源：http://wap.vehdjk.com/Article/details/gxkzyathc.sHtML

[R58] 下载文件
来源：http://www.share.sjlbkw.cn/Article/details/gvcawwrzq.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.m.share.tarul.cn/Article/details/gylbmebpu.sHtML

[R59] 发 POST JSON
来源：http://wap.epnwcf.com/Article/details/gruviwbua.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://baike.bbcook.cn/Article/details/gslgbjmkc.sHtML

[R60] 只看 HTTP 状态码
来源：http://mobile.vehdjk.com/Article/details/gzvgealhw.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.blog.epnwcf.com/Article/details/gcfnvonpf.sHtML

[R61] 磁盘占用
来源：http://read.share.epnwcf.com/Article/details/gnfkskicv.sHtML

df -h;  du -sh *
来源：http://wap.tarul.cn/Article/details/goskwrezs.sHtML

[R62] 找最占空间的文件
来源：http://www.blog.fktsv.cn/Article/details/gotnbgmpx.sHtML

du -ah . | sort -rh | head -10
来源：http://wap.sjlbkw.cn/Article/details/gtzkkprne.sHtML

[R63] 内存与进程
来源：http://wap.bbcook.cn/Article/details/gljnrflnt.sHtML

free -h;  ps aux | grep nginx
来源：http://wap.epnwcf.com/Article/details/gsyqnyita.sHtML

[R64] 结束进程
来源：http://mobile.fktsv.cn/Article/details/gorzljzqg.sHtML

kill -9 $(pgrep -f app.py)
来源：http://m.share.tarul.cn/Article/details/grjglvzqf.sHtML

[R65] 查看端口占用
来源：http://read.share.vehdjk.com/Article/details/gnwhlsjwz.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mobile.sjlbkw.cn/Article/details/gfaofebid.sHtML

[R66] 定时任务
来源：http://m.share.yfazqb.com/Article/details/gylamxnzk.sHtML

crontab -e;  crontab -l
来源：http://3g.bbcook.cn/Article/details/gikhnrtpk.sHtML

[R67] 生成随机十六进制串
来源：http://www.m.share.yfazqb.com/Article/details/gguhpujwa.sHtML

openssl rand -hex 16
来源：http://wap.yfazqb.com/Article/details/gidfiuhsa.sHtML

[R68] 计算文件校验值
来源：http://read.share.bbcook.cn/Article/details/gnfykqype.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://blog.bbcook.cn/Article/details/gkhlqogup.sHtML

[R69] 生成随机密码
来源：http://wap.sjlbkw.cn/Article/details/guwjgwzkx.sHtML

head -c 16 /dev/urandom | base64
来源：http://read.share.yfazqb.com/Article/details/gzrglpbmu.sHtML

[R70] 时间戳与互转
来源：http://read.share.yfazqb.com/Article/details/ghhhoitdw.sHtML

date +%s;  date -d @1700000000
来源：http://www.m.share.tarul.cn/Article/details/ghqfotkzi.sHtML

[R71] 日期格式化
来源：http://baike.epnwcf.com/Article/details/gftadmaxb.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://mobile.vehdjk.com/Article/details/glctwznpj.sHtML

[R72] 等待端口就绪
来源：http://www.blog.sjlbkw.cn/Article/details/gnnitaqic.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://read.share.fktsv.cn/Article/details/gkxghfiiv.sHtML

[R73] 分割大日志
来源：http://read.share.epnwcf.com/Article/details/glysewevd.sHtML

split -l 1000 big.log part_
来源：http://www.share.sjlbkw.cn/Article/details/gjolfkxgj.sHtML

[R74] 批量重命名
来源：http://mobile.sjlbkw.cn/Article/details/gcqzzoccq.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://mobile.fktsv.cn/Article/details/gxsvfvgdi.sHtML

[R75] 导出环境变量
来源：http://baike.vehdjk.com/Article/details/gwhavwyzg.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://read.share.tarul.cn/Article/details/gfhwvanul.sHtML

[R76] 使用临时文件
来源：http://blog.tarul.cn/Article/details/gcnbxinlf.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.yfazqb.com/Article/details/gzsoupsfk.sHtML

[R77] 读取用户输入
来源：http://read.share.fktsv.cn/Article/details/gsdafkown.sHtML

read -rp "请输入: " ans
来源：http://read.share.sjlbkw.cn/Article/details/ggctdaxoj.sHtML

[R78] 交互式菜单
来源：http://blog.bbcook.cn/Article/details/giiknfafu.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://read.share.vehdjk.com/Article/details/gqzsekysa.sHtML

[R79] 解析命令行选项
来源：http://www.blog.epnwcf.com/Article/details/gjvyfupxg.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://baike.fktsv.cn/Article/details/gvzpkicth.sHtML

[R80] 查看脚本执行耗时
来源：http://baike.bbcook.cn/Article/details/gmjqlmsoe.sHtML

time ./run.sh
来源：http://mobile.bbcook.cn/Article/details/gkpngpeho.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/gakzmclav.sHtML

S. C / C++ 专题
来源：http://baike.tarul.cn/Article/details/gopslfnfd.sHtML

================================================================================
来源：http://www.share.epnwcf.com/Article/details/gkgxbrbqx.sHtML

[S01] C：Hello World
来源：http://wap.vehdjk.com/Article/details/ggqxnnqul.sHtML

#include <stdio.h>
来源：http://www.m.share.bbcook.cn/Article/details/gklbbfvvb.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://read.share.fktsv.cn/Article/details/gbjtwhfae.sHtML

[S02] C：变量与格式化输出
来源：http://baike.vehdjk.com/Article/details/gmkigsrna.sHtML

int a = 10; printf("%d\n", a);
来源：http://read.share.sjlbkw.cn/Article/details/gdnrxkaxl.sHtML

[S03] C：读入整数
来源：http://3g.sjlbkw.cn/Article/details/gprzdhzra.sHtML

int x; scanf("%d", &x);
来源：http://read.share.epnwcf.com/Article/details/gdjfjlnvj.sHtML

[S04] C：字符串复制
来源：http://baike.sjlbkw.cn/Article/details/gjiwkxleg.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://3g.epnwcf.com/Article/details/gwoyuzxrl.sHtML

[S05] C：字符串长度
来源：http://read.share.tarul.cn/Article/details/gvxexxrer.sHtML

strlen(s)
来源：http://read.share.fktsv.cn/Article/details/gsijzvvfx.sHtML

[S06] C：字符串比较
来源：http://www.blog.fktsv.cn/Article/details/gglpznron.sHtML

strcmp(a, b) == 0
来源：http://www.blog.vehdjk.com/Article/details/gbzytxwsp.sHtML

[S07] C：数组遍历求和
来源：http://wap.vehdjk.com/Article/details/gcrxpopkj.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.share.yfazqb.com/Article/details/gccqkikub.sHtML

[S08] C：动态内存分配与释放
来源：http://m.share.bbcook.cn/Article/details/glyvjamag.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://read.share.epnwcf.com/Article/details/gnlawknsa.sHtML

[S09] C：结构体定义与初始化
来源：http://blog.sjlbkw.cn/Article/details/grexzmlgf.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.blog.epnwcf.com/Article/details/grzaqtdux.sHtML

[S10] C：指针与解引用
来源：http://www.share.epnwcf.com/Article/details/gkeynwdpb.sHtML

int *p = &a;  *p = 5;
来源：http://m.share.sjlbkw.cn/Article/details/gnrenpmig.sHtML

[S11] C：逐行读文件
来源：http://m.share.bbcook.cn/Article/details/gybwqedyf.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://baike.vehdjk.com/Article/details/gexpbgign.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.blog.sjlbkw.cn/Article/details/gpqqvwssi.sHtML

fclose(f);
来源：http://wap.vehdjk.com/Article/details/gxtvndfjg.sHtML

[S12] C：写文件
来源：http://baike.bbcook.cn/Article/details/gxosrfrtp.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mobile.vehdjk.com/Article/details/gdzyevpwa.sHtML

[S13] C：宏定义
来源：http://wap.tarul.cn/Article/details/gexntywjq.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wap.bbcook.cn/Article/details/ghwcuvtsw.sHtML

[S14] C：枚举
来源：http://m.share.tarul.cn/Article/details/ghemracaq.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://baike.bbcook.cn/Article/details/glutrqzir.sHtML

[S15] C：类型转换
来源：http://wap.yfazqb.com/Article/details/gsywirqha.sHtML

(double) a / b
来源：http://www.share.sjlbkw.cn/Article/details/gqcanlwxj.sHtML

[S16] C：位操作置位
来源：http://www.m.share.bbcook.cn/Article/details/grrfpqbxe.sHtML

x |= (1 << 3);
来源：http://www.m.share.sjlbkw.cn/Article/details/ggkcbtnep.sHtML

[S17] C：安全拼接字符串
来源：http://mobile.yfazqb.com/Article/details/gtewvrbzs.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.share.sjlbkw.cn/Article/details/gknrcleod.sHtML

[S18] C：命令行参数
来源：http://read.share.epnwcf.com/Article/details/ginrmpsys.sHtML

int main(int argc, char **argv)
来源：http://m.share.fktsv.cn/Article/details/glfkjaurf.sHtML

[S19] C：快速排序
来源：http://mobile.epnwcf.com/Article/details/gihhnuwot.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://3g.epnwcf.com/Article/details/gcglypips.sHtML

[S20] C：二分查找
来源：http://www.m.share.epnwcf.com/Article/details/gqqexdbgn.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://read.share.tarul.cn/Article/details/gwgeikeki.sHtML

[S21] C：字符类别判断
来源：http://www.share.sjlbkw.cn/Article/details/gqapuuhqn.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://read.share.tarul.cn/Article/details/gjpnsdozb.sHtML

[S22] C：字符串转数字
来源：http://wap.yfazqb.com/Article/details/gwhdikklq.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://read.share.yfazqb.com/Article/details/gilnakscq.sHtML

[S23] C：随机数
来源：http://www.blog.epnwcf.com/Article/details/gdigyyhky.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://3g.bbcook.cn/Article/details/gopcesqcp.sHtML

[S24] C：获取本地时间
来源：http://wap.epnwcf.com/Article/details/gglhioksf.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://blog.bbcook.cn/Article/details/gzktzkogw.sHtML

[S25] C：内存拷贝
来源：http://3g.sjlbkw.cn/Article/details/gwiajvrlt.sHtML

memcpy(dst, src, n);
来源：http://baike.epnwcf.com/Article/details/gkwtaylmo.sHtML

[S26] C：内存清零
来源：http://m.share.bbcook.cn/Article/details/gkbupjpgq.sHtML

memset(a, 0, sizeof a);
来源：http://baike.vehdjk.com/Article/details/gubvudtun.sHtML

[S27] C：定义常量
来源：http://read.share.bbcook.cn/Article/details/gkxrmrshf.sHtML

const double PI = 3.14159;
来源：http://www.blog.tarul.cn/Article/details/gwgwvpmtz.sHtML

[S28] C：静态变量
来源：http://baike.yfazqb.com/Article/details/gyshrzjpr.sHtML

static int counter = 0;
来源：http://wap.fktsv.cn/Article/details/gprnzuxea.sHtML

[S29] C：变参函数
来源：http://read.share.fktsv.cn/Article/details/gnzjuypxx.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.m.share.fktsv.cn/Article/details/gzcixtrdq.sHtML

[S30] C：头文件保护
来源：http://3g.vehdjk.com/Article/details/guqoeedpp.sHtML

#ifndef X_H
来源：http://read.share.sjlbkw.cn/Article/details/guthnelqs.sHtML

#define X_H
来源：http://blog.sjlbkw.cn/Article/details/gfrhxrgia.sHtML

#endif
来源：http://mobile.epnwcf.com/Article/details/gkjyaibrw.sHtML

[S31] C++：Hello World
来源：http://www.m.share.yfazqb.com/Article/details/gaxrwznoa.sHtML

#include <iostream>
来源：http://baike.yfazqb.com/Article/details/gspjbzhix.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://m.share.yfazqb.com/Article/details/gcpovdskv.sHtML

[S32] C++：字符串
来源：http://www.blog.epnwcf.com/Article/details/gepcjgoya.sHtML

std::string s = "hi";  s += "!";
来源：http://www.m.share.epnwcf.com/Article/details/gkygxyzvx.sHtML

[S33] C++：vector 增删
来源：http://wap.tarul.cn/Article/details/grfccskqh.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://wap.vehdjk.com/Article/details/gioparaat.sHtML

[S34] C++：遍历 vector
来源：http://3g.sjlbkw.cn/Article/details/goeiozcje.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://3g.bbcook.cn/Article/details/gvkxsqkrh.sHtML

[S35] C++：map
来源：http://www.m.share.fktsv.cn/Article/details/gwspwpmpg.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://3g.sjlbkw.cn/Article/details/gzyttjfpm.sHtML

[S36] C++：unordered_map
来源：http://3g.bbcook.cn/Article/details/gymsubrig.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://blog.yfazqb.com/Article/details/gnjtfusyt.sHtML

[S37] C++：set
来源：http://www.m.share.fktsv.cn/Article/details/gwjwbswot.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://baike.bbcook.cn/Article/details/gntjhktyo.sHtML

[S38] C++：排序
来源：http://wap.vehdjk.com/Article/details/gxzxvsuuy.sHtML

std::sort(v.begin(), v.end());
来源：http://blog.tarul.cn/Article/details/givcfpbuv.sHtML

[S39] C++：自定义比较器排序
来源：http://www.share.vehdjk.com/Article/details/giwwcstqr.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.m.share.yfazqb.com/Article/details/gmdivvqug.sHtML

[S40] C++：查找元素
来源：http://www.m.share.fktsv.cn/Article/details/glewjliaq.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.blog.sjlbkw.cn/Article/details/gqychmmtg.sHtML

[S41] C++：类与构造函数
来源：http://read.share.bbcook.cn/Article/details/gxyybzdid.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://baike.sjlbkw.cn/Article/details/gyccwiskb.sHtML

[S42] C++：继承与虚函数
来源：http://3g.fktsv.cn/Article/details/gisbpsuez.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.blog.yfazqb.com/Article/details/gglhkcvnn.sHtML

[S43] C++：智能指针
来源：http://www.m.share.sjlbkw.cn/Article/details/gezfegaof.sHtML

auto p = std::make_unique<int>(5);
来源：http://mobile.epnwcf.com/Article/details/gvgwwggqw.sHtML

[S44] C++：引用传参
来源：http://wap.yfazqb.com/Article/details/gklhrcjja.sHtML

void inc(int &x) { ++x; }
来源：http://mobile.yfazqb.com/Article/details/gkzudzuar.sHtML

[S45] C++：lambda
来源：http://www.m.share.yfazqb.com/Article/details/gwjtzzowd.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://3g.epnwcf.com/Article/details/gknsocdze.sHtML

[S46] C++：函数模板
来源：http://www.share.vehdjk.com/Article/details/grloeejlv.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://read.share.sjlbkw.cn/Article/details/gvicanzmt.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.m.share.sjlbkw.cn/Article/details/ggicwkkrq.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://read.share.yfazqb.com/Article/details/gwyrsowwb.sHtML

[S48] C++：逐行读文件
来源：http://3g.fktsv.cn/Article/details/gwnofifpf.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.blog.epnwcf.com/Article/details/gulepcffv.sHtML

while (std::getline(in, line)) { }
来源：http://blog.fktsv.cn/Article/details/gikoaltuo.sHtML

[S49] C++：写文件
来源：http://3g.tarul.cn/Article/details/gimoxkfeh.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.blog.fktsv.cn/Article/details/guhjaigvo.sHtML

[S50] C++：格式化数字
来源：http://blog.epnwcf.com/Article/details/goezkmcyq.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.blog.vehdjk.com/Article/details/gvijogdxb.sHtML

[S51] C++：显式类型转换
来源：http://www.m.share.bbcook.cn/Article/details/guxolmvbw.sHtML

static_cast<double>(a) / b
来源：http://www.m.share.fktsv.cn/Article/details/gwjvzihqz.sHtML

[S52] C++：const 与 noexcept
来源：http://3g.tarul.cn/Article/details/gotsmwnqu.sHtML

int size() const noexcept { return n_; }
来源：http://3g.bbcook.cn/Article/details/ggnctrrxo.sHtML

[S53] C++：移动语义
来源：http://read.share.epnwcf.com/Article/details/grtgdnnhn.sHtML

std::vector<int> w = std::move(v);
来源：http://wap.yfazqb.com/Article/details/gfvngdnlr.sHtML

[S54] C++：异常处理
来源：http://mobile.bbcook.cn/Article/details/grffhdciq.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://baike.sjlbkw.cn/Article/details/glhdhmrlt.sHtML

[S55] C++：结构化绑定
来源：http://wap.sjlbkw.cn/Article/details/gzmtiaxwr.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://baike.sjlbkw.cn/Article/details/geioelrws.sHtML

[S56] C++：optional
来源：http://www.blog.bbcook.cn/Article/details/giidcsziq.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://3g.vehdjk.com/Article/details/gfunxtrob.sHtML

[S57] C++：编译期常量
来源：http://3g.sjlbkw.cn/Article/details/gtolajqkr.sHtML

constexpr int N = 10;
来源：http://www.m.share.epnwcf.com/Article/details/gnuhcmfpl.sHtML

[S58] C++：命名空间
来源：http://www.blog.tarul.cn/Article/details/gwtdwmvdg.sHtML

namespace ns { int f() { return 1; } }
来源：http://m.share.sjlbkw.cn/Article/details/gpjsvsxri.sHtML

[S59] C++：静态断言
来源：http://www.blog.epnwcf.com/Article/details/gbqbhottl.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://blog.vehdjk.com/Article/details/gxvjgikgl.sHtML

[S60] C++：遍历并删除元素
来源：http://read.share.tarul.cn/Article/details/gfmivacys.sHtML


<!-- 参考信息 -->