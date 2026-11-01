代发 wailian999

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://blog.yfazqb.com/Article/details/gacvyseym.sHtML

[Q90] 生成序号列
来源：http://wap.vehdjk.com/Article/details/ghijsyebo.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://m.share.vehdjk.com/Article/details/ggfprnqxy.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/gihdobtpq.sHtML

R. Bash 专题
来源：http://www.share.yfazqb.com/Article/details/gewiizfub.sHtML

================================================================================
来源：http://www.share.vehdjk.com/Article/details/glvvziqnf.sHtML

[R01] shebang 与严格模式
来源：http://m.share.vehdjk.com/Article/details/gbtqskckj.sHtML

#!/usr/bin/env bash
来源：http://www.m.share.vehdjk.com/Article/details/ghtwekrdu.sHtML

set -euo pipefail
来源：http://3g.tarul.cn/Article/details/gkttinyfy.sHtML

[R02] 变量赋值与使用
来源：http://baike.epnwcf.com/Article/details/gcbhvpwen.sHtML

name="Tom"; echo "$name"
来源：http://www.share.tarul.cn/Article/details/gbvyyidng.sHtML

[R03] 只读变量
来源：http://www.share.epnwcf.com/Article/details/glyrotvrp.sHtML

readonly PI=3.14
来源：http://baike.fktsv.cn/Article/details/gqjdkwuox.sHtML

[R04] 位置参数
来源：http://wap.tarul.cn/Article/details/gwvmcghqt.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://3g.fktsv.cn/Article/details/gxfgkcsud.sHtML

[R05] 参数默认值
来源：http://read.share.fktsv.cn/Article/details/gqdmidsxx.sHtML

name="${1:-default}"
来源：http://mobile.sjlbkw.cn/Article/details/gkryergos.sHtML

[R06] 判断命令是否存在
来源：http://www.share.epnwcf.com/Article/details/giwurcgzr.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://3g.fktsv.cn/Article/details/gsvfavqau.sHtML

[R07] if 判断文件
来源：http://www.blog.vehdjk.com/Article/details/gzninjuqs.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://wap.bbcook.cn/Article/details/gnosywtmj.sHtML

[R08] 数值比较
来源：http://3g.bbcook.cn/Article/details/gclrpccur.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://blog.fktsv.cn/Article/details/gfzkrxisy.sHtML

[R09] 字符串比较
来源：http://baike.tarul.cn/Article/details/gwlzijmgw.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://blog.fktsv.cn/Article/details/gmgaodyeg.sHtML

[R10] 正则匹配
来源：http://www.share.vehdjk.com/Article/details/gqtdycdnl.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.blog.vehdjk.com/Article/details/gyxrqtlmd.sHtML

[R11] case 多分支
来源：http://m.share.fktsv.cn/Article/details/gnjbkgkby.sHtML

case "$1" in
来源：http://wap.bbcook.cn/Article/details/gnpkeqhap.sHtML

start) echo "启动" ;;
来源：http://www.m.share.sjlbkw.cn/Article/details/giqhaeesy.sHtML

stop)  echo "停止" ;;
来源：http://3g.tarul.cn/Article/details/giwqgcwsn.sHtML

*)     echo "未知命令" ;;
来源：http://blog.bbcook.cn/Article/details/gqirpzefg.sHtML

esac
来源：http://wap.epnwcf.com/Article/details/ggdjapdvw.sHtML

[R12] for 遍历文件
来源：http://www.m.share.epnwcf.com/Article/details/gnrqovplg.sHtML

for f in *.txt; do echo "$f"; done
来源：http://blog.epnwcf.com/Article/details/gcpyxlacm.sHtML

[R13] for 计数循环
来源：http://www.blog.fktsv.cn/Article/details/gibofemnq.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://read.share.vehdjk.com/Article/details/gdapfoqos.sHtML

[R14] C 风格 for
来源：http://mobile.epnwcf.com/Article/details/grdndfrwp.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://3g.epnwcf.com/Article/details/gyoerdmyx.sHtML

[R15] while 逐行读文件
来源：http://read.share.epnwcf.com/Article/details/glychqwuq.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.blog.fktsv.cn/Article/details/gsdrddrpj.sHtML

[R16] until 等待条件
来源：http://wap.epnwcf.com/Article/details/gfzvqrsxf.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.blog.vehdjk.com/Article/details/gnffrejhx.sHtML

[R17] 数组定义与取值
来源：http://read.share.vehdjk.com/Article/details/gtpbindog.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://m.share.yfazqb.com/Article/details/gttwlibxh.sHtML

[R18] 遍历数组
来源：http://read.share.fktsv.cn/Article/details/gpgfnvlvv.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://read.share.fktsv.cn/Article/details/ghbxxmnya.sHtML

[R19] 数组长度
来源：http://blog.tarul.cn/Article/details/gstyblvgq.sHtML

echo "${#arr[@]}"
来源：http://m.share.sjlbkw.cn/Article/details/gumsqpjvo.sHtML

[R20] 关联数组（字典）
来源：http://www.share.vehdjk.com/Article/details/gtasbtsue.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://baike.vehdjk.com/Article/details/gztzqtzhv.sHtML

[R21] 字符串长度
来源：http://www.m.share.sjlbkw.cn/Article/details/gnkuanhrg.sHtML

echo "${#s}"
来源：http://blog.yfazqb.com/Article/details/gwhdmihzh.sHtML

[R22] 截取子串
来源：http://blog.tarul.cn/Article/details/gkgisjbxt.sHtML

echo "${s:0:5}"
来源：http://www.m.share.yfazqb.com/Article/details/gsbzlogvu.sHtML

[R23] 字符串替换
来源：http://mobile.vehdjk.com/Article/details/gizxzdijm.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://baike.sjlbkw.cn/Article/details/gnrymgdvb.sHtML

[R24] 大小写转换
来源：http://blog.fktsv.cn/Article/details/gwdzbglkk.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://wap.yfazqb.com/Article/details/gbybttkya.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.m.share.fktsv.cn/Article/details/gtmrykzkd.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://read.share.bbcook.cn/Article/details/gopeyhsks.sHtML

[R26] 命令替换
来源：http://www.blog.vehdjk.com/Article/details/gdzitwbbe.sHtML

now=$(date +%F); echo "$now"
来源：http://www.blog.epnwcf.com/Article/details/gmqiqepye.sHtML

[R27] 算术展开
来源：http://3g.sjlbkw.cn/Article/details/grcglnuyf.sHtML

echo $((1 + 2 * 3))
来源：http://blog.sjlbkw.cn/Article/details/geywsdoww.sHtML

[R28] 浮点运算
来源：http://3g.sjlbkw.cn/Article/details/gjakfnqwi.sHtML

echo "scale=2; 10/3" | bc
来源：http://baike.epnwcf.com/Article/details/gdezbqwhq.sHtML

[R29] 定义函数
来源：http://m.share.bbcook.cn/Article/details/gtubvfpqg.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.share.sjlbkw.cn/Article/details/gbklanxsu.sHtML

[R30] 函数返回状态码
来源：http://read.share.bbcook.cn/Article/details/gncebbkvs.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://blog.tarul.cn/Article/details/gqatiyuch.sHtML

[R31] 局部变量
来源：http://blog.vehdjk.com/Article/details/gaefbchee.sHtML

f() { local x=1; echo "$x"; }
来源：http://mobile.vehdjk.com/Article/details/glzixhdpu.sHtML

[R32] 参数个数校验
来源：http://m.share.yfazqb.com/Article/details/gkruwyllf.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.blog.fktsv.cn/Article/details/gojahpbzb.sHtML

[R33] 捕获错误并提示行号
来源：http://3g.epnwcf.com/Article/details/gfjrfhkmc.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://mobile.epnwcf.com/Article/details/guqoukobp.sHtML

[R34] 退出时清理
来源：http://read.share.sjlbkw.cn/Article/details/goewjphho.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://baike.yfazqb.com/Article/details/gxfbmkpsh.sHtML

[R35] 后台执行并等待
来源：http://blog.yfazqb.com/Article/details/gesuuonzk.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.m.share.tarul.cn/Article/details/gscavfwco.sHtML

[R36] 并发执行多个任务
来源：http://mobile.epnwcf.com/Article/details/gsllhaffa.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://blog.bbcook.cn/Article/details/gvgukslwq.sHtML

[R37] 把输出赋给变量
来源：http://m.share.bbcook.cn/Article/details/giaqartfx.sHtML

files=$(ls -1)
来源：http://mobile.yfazqb.com/Article/details/guhucprmy.sHtML

[R38] 管道串联
来源：http://read.share.yfazqb.com/Article/details/gspmrnkmo.sHtML

cat a.txt | grep -i error | wc -l
来源：http://m.share.fktsv.cn/Article/details/guoayqswn.sHtML

[R39] 重定向标准输出与错误
来源：http://3g.tarul.cn/Article/details/gferywruj.sHtML

cmd > out.log 2>&1
来源：http://mobile.epnwcf.com/Article/details/gekllfzyd.sHtML

[R40] 追加写日志
来源：http://3g.tarul.cn/Article/details/gznymlrhq.sHtML

echo "log" >> out.log
来源：http://wap.sjlbkw.cn/Article/details/gijqvxdsj.sHtML

[R41] 丢弃输出
来源：http://www.share.fktsv.cn/Article/details/grdyaioif.sHtML

cmd >/dev/null 2>&1
来源：http://read.share.fktsv.cn/Article/details/gbdbtogtt.sHtML

[R42] 输入重定向
来源：http://mobile.yfazqb.com/Article/details/gazatmxbm.sHtML

wc -l < a.txt
来源：http://www.blog.yfazqb.com/Article/details/gglzxcuos.sHtML

[R43] 按名字查找文件
来源：http://mobile.tarul.cn/Article/details/gxnkdhfue.sHtML

find . -name "*.log" -type f
来源：http://www.share.vehdjk.com/Article/details/gjlmylytc.sHtML

[R44] 按修改时间查找
来源：http://read.share.fktsv.cn/Article/details/gxcnzjdtc.sHtML

find . -mtime -7 -type f
来源：http://baike.tarul.cn/Article/details/gafkccvqp.sHtML

[R45] 批量删除
来源：http://blog.vehdjk.com/Article/details/gyaojvzmm.sHtML

find . -name "*.tmp" -delete
来源：http://wap.bbcook.cn/Article/details/gpaycpgaa.sHtML

[R46] 递归替换文件内容
来源：http://www.share.yfazqb.com/Article/details/gxcdyqhpj.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://blog.vehdjk.com/Article/details/gpxvliiai.sHtML

[R47] sed 单行替换
来源：http://blog.sjlbkw.cn/Article/details/gcahhkcux.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://3g.tarul.cn/Article/details/gjwbrxwyl.sHtML

[R48] awk 取指定列
来源：http://3g.sjlbkw.cn/Article/details/gxwlhmzcf.sHtML

awk '{print $1, $3}' a.txt
来源：http://wap.fktsv.cn/Article/details/gzhycfbre.sHtML

[R49] awk 带条件
来源：http://mobile.fktsv.cn/Article/details/gvrumjkhe.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://baike.vehdjk.com/Article/details/gwpsxwdzw.sHtML

[R50] awk 求和
来源：http://3g.vehdjk.com/Article/details/gkzyuincv.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.m.share.fktsv.cn/Article/details/goktfgrim.sHtML

[R51] 排序去重取前几
来源：http://3g.epnwcf.com/Article/details/gqkqbeblf.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://wap.epnwcf.com/Article/details/gmyadwgzt.sHtML

[R52] 统计行数
来源：http://wap.fktsv.cn/Article/details/gntyyumgc.sHtML

wc -l a.txt
来源：http://www.share.bbcook.cn/Article/details/gadalrxre.sHtML

[R53] 查看文件头与实时尾
来源：http://baike.epnwcf.com/Article/details/gzdoxxbpy.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://wap.bbcook.cn/Article/details/gqffujtmu.sHtML

[R54] 比较两个文件
来源：http://wap.fktsv.cn/Article/details/gvvcsqxyp.sHtML

diff a.txt b.txt
来源：http://3g.sjlbkw.cn/Article/details/gffaxryug.sHtML

[R55] 压缩与解压
来源：http://www.share.bbcook.cn/Article/details/guuvgddfu.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://blog.bbcook.cn/Article/details/ghoiundds.sHtML

[R56] 远程拷贝
来源：http://3g.fktsv.cn/Article/details/gduvkeozm.sHtML

scp file user@host:/path/
来源：http://www.share.fktsv.cn/Article/details/gvagjkwvz.sHtML

[R57] 远程执行命令
来源：http://www.blog.vehdjk.com/Article/details/gajtnmbps.sHtML

ssh user@host 'uptime'
来源：http://blog.fktsv.cn/Article/details/ghxvwfmxl.sHtML

[R58] 下载文件
来源：http://wap.fktsv.cn/Article/details/gxhbpmpmz.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://blog.vehdjk.com/Article/details/gcqpyxvvp.sHtML

[R59] 发 POST JSON
来源：http://www.blog.yfazqb.com/Article/details/gwxyojxqs.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://3g.epnwcf.com/Article/details/gchrcrlqw.sHtML

[R60] 只看 HTTP 状态码
来源：http://mobile.sjlbkw.cn/Article/details/gzkylcnks.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.m.share.sjlbkw.cn/Article/details/gwdlxocyv.sHtML

[R61] 磁盘占用
来源：http://baike.sjlbkw.cn/Article/details/gypzyhtyy.sHtML

df -h;  du -sh *
来源：http://wap.sjlbkw.cn/Article/details/gxjvupltj.sHtML

[R62] 找最占空间的文件
来源：http://m.share.fktsv.cn/Article/details/gjwpvllkq.sHtML

du -ah . | sort -rh | head -10
来源：http://blog.bbcook.cn/Article/details/gsqakmllf.sHtML

[R63] 内存与进程
来源：http://mobile.vehdjk.com/Article/details/gyarddzud.sHtML

free -h;  ps aux | grep nginx
来源：http://mobile.yfazqb.com/Article/details/gehqwrwhk.sHtML

[R64] 结束进程
来源：http://www.m.share.yfazqb.com/Article/details/gzfhghqtk.sHtML

kill -9 $(pgrep -f app.py)
来源：http://read.share.bbcook.cn/Article/details/gvnivqdhi.sHtML

[R65] 查看端口占用
来源：http://mobile.sjlbkw.cn/Article/details/gcjmgvfzk.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://m.share.fktsv.cn/Article/details/gomadrfyk.sHtML

[R66] 定时任务
来源：http://www.m.share.bbcook.cn/Article/details/gnfjfjvre.sHtML

crontab -e;  crontab -l
来源：http://m.share.bbcook.cn/Article/details/gedrxphwt.sHtML

[R67] 生成随机十六进制串
来源：http://blog.yfazqb.com/Article/details/gkbtqyelm.sHtML

openssl rand -hex 16
来源：http://wap.yfazqb.com/Article/details/gtphlther.sHtML

[R68] 计算文件校验值
来源：http://mobile.bbcook.cn/Article/details/gcisomwqt.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://baike.epnwcf.com/Article/details/gbakocxvd.sHtML

[R69] 生成随机密码
来源：http://www.share.yfazqb.com/Article/details/gzkgwxvvv.sHtML

head -c 16 /dev/urandom | base64
来源：http://mobile.sjlbkw.cn/Article/details/gasslcmdz.sHtML

[R70] 时间戳与互转
来源：http://blog.epnwcf.com/Article/details/gikbxcnrh.sHtML

date +%s;  date -d @1700000000
来源：http://read.share.sjlbkw.cn/Article/details/gaboqrbab.sHtML

[R71] 日期格式化
来源：http://www.m.share.vehdjk.com/Article/details/glkjjvemb.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://3g.sjlbkw.cn/Article/details/gznybdltb.sHtML

[R72] 等待端口就绪
来源：http://m.share.yfazqb.com/Article/details/gerdcgntd.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.blog.fktsv.cn/Article/details/gdjgvgkaf.sHtML

[R73] 分割大日志
来源：http://blog.fktsv.cn/Article/details/gfuashqwu.sHtML

split -l 1000 big.log part_
来源：http://blog.vehdjk.com/Article/details/gktamgyyi.sHtML

[R74] 批量重命名
来源：http://mobile.bbcook.cn/Article/details/guyidoddi.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.share.vehdjk.com/Article/details/gdjpfgqid.sHtML

[R75] 导出环境变量
来源：http://mobile.tarul.cn/Article/details/gvbzzvbmn.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://m.share.yfazqb.com/Article/details/gwfdnkjbq.sHtML

[R76] 使用临时文件
来源：http://m.share.sjlbkw.cn/Article/details/gckfifxjz.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://blog.sjlbkw.cn/Article/details/ghhryzyrr.sHtML

[R77] 读取用户输入
来源：http://www.share.tarul.cn/Article/details/gpqowalph.sHtML

read -rp "请输入: " ans
来源：http://www.share.bbcook.cn/Article/details/gpseravib.sHtML

[R78] 交互式菜单
来源：http://baike.tarul.cn/Article/details/glgwncxls.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.m.share.sjlbkw.cn/Article/details/gpdhjuokd.sHtML

[R79] 解析命令行选项
来源：http://www.share.sjlbkw.cn/Article/details/gvjlwbmji.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://read.share.fktsv.cn/Article/details/gtelnvscm.sHtML

[R80] 查看脚本执行耗时
来源：http://mobile.tarul.cn/Article/details/godkyudqf.sHtML

time ./run.sh
来源：http://blog.tarul.cn/Article/details/ghwcgzydq.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/gjskewdvx.sHtML

S. C / C++ 专题
来源：http://read.share.sjlbkw.cn/Article/details/gjflasuyz.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/gqnlgaytj.sHtML

[S01] C：Hello World
来源：http://wap.tarul.cn/Article/details/gctsjnaaz.sHtML

#include <stdio.h>
来源：http://www.share.sjlbkw.cn/Article/details/ghekwuwnf.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.m.share.yfazqb.com/Article/details/gckxypvvf.sHtML

[S02] C：变量与格式化输出
来源：http://baike.sjlbkw.cn/Article/details/gworovfvo.sHtML

int a = 10; printf("%d\n", a);
来源：http://baike.yfazqb.com/Article/details/glbwieqit.sHtML

[S03] C：读入整数
来源：http://www.m.share.tarul.cn/Article/details/gtkkcewdm.sHtML

int x; scanf("%d", &x);
来源：http://www.blog.vehdjk.com/Article/details/ggmplkewp.sHtML

[S04] C：字符串复制
来源：http://read.share.sjlbkw.cn/Article/details/grtugnutf.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://m.share.sjlbkw.cn/Article/details/gmhphgbmq.sHtML

[S05] C：字符串长度
来源：http://www.m.share.tarul.cn/Article/details/gyyzimvds.sHtML

strlen(s)
来源：http://baike.sjlbkw.cn/Article/details/gdimzkkxv.sHtML

[S06] C：字符串比较
来源：http://mobile.bbcook.cn/Article/details/gbsffgkah.sHtML

strcmp(a, b) == 0
来源：http://3g.yfazqb.com/Article/details/gczvbfutp.sHtML

[S07] C：数组遍历求和
来源：http://mobile.yfazqb.com/Article/details/gvneeiqgq.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://m.share.tarul.cn/Article/details/gekxnzhhu.sHtML

[S08] C：动态内存分配与释放
来源：http://baike.vehdjk.com/Article/details/grxfwszfd.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://m.share.yfazqb.com/Article/details/gettecidr.sHtML

[S09] C：结构体定义与初始化
来源：http://read.share.fktsv.cn/Article/details/goxzrzxra.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://wap.tarul.cn/Article/details/gohaoplms.sHtML

[S10] C：指针与解引用
来源：http://www.share.sjlbkw.cn/Article/details/gpedekmxq.sHtML

int *p = &a;  *p = 5;
来源：http://baike.yfazqb.com/Article/details/gbwsysztt.sHtML

[S11] C：逐行读文件
来源：http://www.blog.tarul.cn/Article/details/gmbydbhkq.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://blog.epnwcf.com/Article/details/grwrgbwmh.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://3g.fktsv.cn/Article/details/gwjmpwhmz.sHtML

fclose(f);
来源：http://www.m.share.yfazqb.com/Article/details/ghegefkju.sHtML

[S12] C：写文件
来源：http://m.share.bbcook.cn/Article/details/gwmjdngtv.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.share.bbcook.cn/Article/details/gwihrvqye.sHtML

[S13] C：宏定义
来源：http://read.share.sjlbkw.cn/Article/details/ggnrpahmf.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://m.share.yfazqb.com/Article/details/gbqzznrzq.sHtML

[S14] C：枚举
来源：http://www.m.share.epnwcf.com/Article/details/gfwiszkom.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.share.vehdjk.com/Article/details/ghttquwpq.sHtML

[S15] C：类型转换
来源：http://www.blog.tarul.cn/Article/details/ggmkcgqof.sHtML

(double) a / b
来源：http://mobile.fktsv.cn/Article/details/gsjwqwpic.sHtML

[S16] C：位操作置位
来源：http://mobile.sjlbkw.cn/Article/details/gldghibox.sHtML

x |= (1 << 3);
来源：http://www.share.vehdjk.com/Article/details/gocoqwwxt.sHtML

[S17] C：安全拼接字符串
来源：http://3g.tarul.cn/Article/details/gjagtuibd.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wap.epnwcf.com/Article/details/giadmsnzf.sHtML

[S18] C：命令行参数
来源：http://www.share.tarul.cn/Article/details/gysaoewob.sHtML

int main(int argc, char **argv)
来源：http://m.share.tarul.cn/Article/details/gigblatfy.sHtML

[S19] C：快速排序
来源：http://wap.yfazqb.com/Article/details/gqfhezdrk.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://mobile.tarul.cn/Article/details/geruefeeo.sHtML

[S20] C：二分查找
来源：http://wap.yfazqb.com/Article/details/gdleyxcwi.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://blog.fktsv.cn/Article/details/gudayqaqu.sHtML

[S21] C：字符类别判断
来源：http://m.share.tarul.cn/Article/details/ghogybwrr.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://blog.vehdjk.com/Article/details/gdxwdktkb.sHtML

[S22] C：字符串转数字
来源：http://m.share.epnwcf.com/Article/details/gvdupzjfo.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://blog.vehdjk.com/Article/details/ginibwgeb.sHtML

[S23] C：随机数
来源：http://www.m.share.sjlbkw.cn/Article/details/gydbjtxqv.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.blog.yfazqb.com/Article/details/glfiuxgvh.sHtML

[S24] C：获取本地时间
来源：http://www.share.yfazqb.com/Article/details/ghbbusfsw.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://wap.yfazqb.com/Article/details/gdadoitmk.sHtML

[S25] C：内存拷贝
来源：http://wap.epnwcf.com/Article/details/gjocbobxb.sHtML

memcpy(dst, src, n);
来源：http://blog.sjlbkw.cn/Article/details/gmxodosbf.sHtML

[S26] C：内存清零
来源：http://blog.sjlbkw.cn/Article/details/gxkihtlgt.sHtML

memset(a, 0, sizeof a);
来源：http://blog.yfazqb.com/Article/details/gubgqfdop.sHtML

[S27] C：定义常量
来源：http://3g.fktsv.cn/Article/details/gpnvyefgu.sHtML

const double PI = 3.14159;
来源：http://wap.fktsv.cn/Article/details/gptirvrye.sHtML

[S28] C：静态变量
来源：http://blog.vehdjk.com/Article/details/gvrqefpup.sHtML

static int counter = 0;
来源：http://read.share.vehdjk.com/Article/details/gavnbkvxr.sHtML

[S29] C：变参函数
来源：http://read.share.fktsv.cn/Article/details/guhzjjyqk.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://baike.vehdjk.com/Article/details/gtpwzckvv.sHtML

[S30] C：头文件保护
来源：http://baike.vehdjk.com/Article/details/gzjapsdob.sHtML

#ifndef X_H
来源：http://m.share.tarul.cn/Article/details/gqtekgmci.sHtML

#define X_H
来源：http://m.share.epnwcf.com/Article/details/gajpcnoza.sHtML

#endif
来源：http://baike.vehdjk.com/Article/details/gjrynizqz.sHtML

[S31] C++：Hello World
来源：http://read.share.epnwcf.com/Article/details/glfcbrgdn.sHtML

#include <iostream>
来源：http://mobile.epnwcf.com/Article/details/gqwjpkezy.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://blog.tarul.cn/Article/details/gcynxxkxb.sHtML

[S32] C++：字符串
来源：http://baike.sjlbkw.cn/Article/details/gydiozjtl.sHtML

std::string s = "hi";  s += "!";
来源：http://baike.tarul.cn/Article/details/guecpqupz.sHtML

[S33] C++：vector 增删
来源：http://www.share.bbcook.cn/Article/details/gqmhdrarh.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://3g.tarul.cn/Article/details/gqoewpsku.sHtML

[S34] C++：遍历 vector
来源：http://www.blog.bbcook.cn/Article/details/gewaxryxy.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://blog.tarul.cn/Article/details/ggxdeoxee.sHtML

[S35] C++：map
来源：http://3g.tarul.cn/Article/details/givnvdokt.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wap.sjlbkw.cn/Article/details/gnwvaesnw.sHtML

[S36] C++：unordered_map
来源：http://www.m.share.epnwcf.com/Article/details/gtuhzbpnt.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.fktsv.cn/Article/details/gyvesuuyu.sHtML

[S37] C++：set
来源：http://baike.epnwcf.com/Article/details/gmadhlgga.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wap.vehdjk.com/Article/details/gxbhhxeeu.sHtML

[S38] C++：排序
来源：http://www.share.vehdjk.com/Article/details/gzwmydvzp.sHtML

std::sort(v.begin(), v.end());
来源：http://blog.sjlbkw.cn/Article/details/gvezaanvn.sHtML

[S39] C++：自定义比较器排序
来源：http://3g.bbcook.cn/Article/details/gcotcrgls.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.share.bbcook.cn/Article/details/gewtlwspo.sHtML

[S40] C++：查找元素
来源：http://mobile.tarul.cn/Article/details/geljzehpv.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://3g.tarul.cn/Article/details/grpjebyfh.sHtML

[S41] C++：类与构造函数
来源：http://read.share.sjlbkw.cn/Article/details/gjeifotmt.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://m.share.epnwcf.com/Article/details/ghgwulbdb.sHtML

[S42] C++：继承与虚函数
来源：http://www.blog.yfazqb.com/Article/details/gdsvdflvh.sHtML

class B : public Base { public: void f() override {} };
来源：http://mobile.vehdjk.com/Article/details/gxqxgmgwu.sHtML

[S43] C++：智能指针
来源：http://3g.tarul.cn/Article/details/glnaebatf.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.blog.vehdjk.com/Article/details/gymgvbmvk.sHtML

[S44] C++：引用传参
来源：http://3g.bbcook.cn/Article/details/gnawgotuu.sHtML

void inc(int &x) { ++x; }
来源：http://www.m.share.fktsv.cn/Article/details/gnkxxsvzw.sHtML

[S45] C++：lambda
来源：http://www.m.share.tarul.cn/Article/details/gwrhqfwdf.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://3g.epnwcf.com/Article/details/gzfhurwgq.sHtML

[S46] C++：函数模板
来源：http://mobile.yfazqb.com/Article/details/gbgwfodab.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://baike.fktsv.cn/Article/details/gknzxiewv.sHtML

[S47] C++：结构化绑定遍历
来源：http://wap.tarul.cn/Article/details/gqswvfkxd.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.m.share.bbcook.cn/Article/details/gzmdaunsp.sHtML

[S48] C++：逐行读文件
来源：http://www.share.epnwcf.com/Article/details/gzdwwnefy.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://blog.sjlbkw.cn/Article/details/gcpkrrqid.sHtML

while (std::getline(in, line)) { }
来源：http://www.blog.fktsv.cn/Article/details/gwljxvzze.sHtML

[S49] C++：写文件
来源：http://3g.bbcook.cn/Article/details/gooreqvjm.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.blog.bbcook.cn/Article/details/gyrdeilit.sHtML

[S50] C++：格式化数字
来源：http://mobile.bbcook.cn/Article/details/gchyexrbm.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://3g.fktsv.cn/Article/details/gudvecsoj.sHtML

[S51] C++：显式类型转换
来源：http://read.share.bbcook.cn/Article/details/gysndbtcr.sHtML

static_cast<double>(a) / b
来源：http://www.blog.yfazqb.com/Article/details/gaqorhdcs.sHtML

[S52] C++：const 与 noexcept
来源：http://3g.epnwcf.com/Article/details/gnajlkxqk.sHtML

int size() const noexcept { return n_; }
来源：http://3g.bbcook.cn/Article/details/gemmijkfh.sHtML

[S53] C++：移动语义
来源：http://m.share.bbcook.cn/Article/details/gwqdjowpd.sHtML

std::vector<int> w = std::move(v);
来源：http://www.m.share.vehdjk.com/Article/details/gfkcpcfwu.sHtML

[S54] C++：异常处理
来源：http://www.m.share.vehdjk.com/Article/details/gjremgoiq.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://m.share.fktsv.cn/Article/details/ghwaufhdu.sHtML

[S55] C++：结构化绑定
来源：http://m.share.sjlbkw.cn/Article/details/gyguqyobp.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://wap.vehdjk.com/Article/details/gveiclgfd.sHtML

[S56] C++：optional
来源：http://baike.yfazqb.com/Article/details/gwjhmnqze.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://read.share.tarul.cn/Article/details/gzikgvycv.sHtML

[S57] C++：编译期常量
来源：http://www.blog.epnwcf.com/Article/details/ghhvjdfps.sHtML

constexpr int N = 10;
来源：http://www.blog.vehdjk.com/Article/details/ggabrqtaz.sHtML

[S58] C++：命名空间
来源：http://3g.fktsv.cn/Article/details/gbzhjuyuf.sHtML

namespace ns { int f() { return 1; } }
来源：http://baike.sjlbkw.cn/Article/details/gajqfxemy.sHtML

[S59] C++：静态断言
来源：http://read.share.vehdjk.com/Article/details/gmjqdvaue.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://mobile.sjlbkw.cn/Article/details/gqvlqikcr.sHtML

[S60] C++：遍历并删除元素
来源：http://m.share.fktsv.cn/Article/details/ghxglrkoy.sHtML


<!-- 参考信息 -->