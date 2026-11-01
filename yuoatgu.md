代发 wailian999

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://baike.sjlbkw.cn/Article/details/goqcpnpdq.sHtML

[Q90] 生成序号列
来源：http://mobile.sjlbkw.cn/Article/details/gwlryohwc.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://read.share.fktsv.cn/Article/details/glkelkbde.sHtML

================================================================================
来源：http://baike.vehdjk.com/Article/details/gfvmfzdto.sHtML

R. Bash 专题
来源：http://www.blog.vehdjk.com/Article/details/gdagmdcti.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/gjgwcziwc.sHtML

[R01] shebang 与严格模式
来源：http://blog.yfazqb.com/Article/details/gmjprashq.sHtML

#!/usr/bin/env bash
来源：http://blog.tarul.cn/Article/details/gfxpjmylf.sHtML

set -euo pipefail
来源：http://blog.bbcook.cn/Article/details/gqvoinfqz.sHtML

[R02] 变量赋值与使用
来源：http://www.m.share.vehdjk.com/Article/details/gcmzfbqse.sHtML

name="Tom"; echo "$name"
来源：http://blog.sjlbkw.cn/Article/details/ghsobrkgj.sHtML

[R03] 只读变量
来源：http://3g.epnwcf.com/Article/details/gemuzicka.sHtML

readonly PI=3.14
来源：http://read.share.bbcook.cn/Article/details/gafznzszk.sHtML

[R04] 位置参数
来源：http://baike.sjlbkw.cn/Article/details/gxmizodhc.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://mobile.epnwcf.com/Article/details/gnrjgpxux.sHtML

[R05] 参数默认值
来源：http://read.share.yfazqb.com/Article/details/ggtdwlzij.sHtML

name="${1:-default}"
来源：http://blog.vehdjk.com/Article/details/giyxxcfgb.sHtML

[R06] 判断命令是否存在
来源：http://www.blog.fktsv.cn/Article/details/gjfdezyng.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.blog.yfazqb.com/Article/details/gxetsocxb.sHtML

[R07] if 判断文件
来源：http://3g.fktsv.cn/Article/details/ghqtoqzvl.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.share.fktsv.cn/Article/details/gitooqome.sHtML

[R08] 数值比较
来源：http://m.share.epnwcf.com/Article/details/gizbcgtrv.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://baike.vehdjk.com/Article/details/gqlkyehmr.sHtML

[R09] 字符串比较
来源：http://www.share.epnwcf.com/Article/details/gptgqbrff.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.blog.sjlbkw.cn/Article/details/garspmcoy.sHtML

[R10] 正则匹配
来源：http://baike.yfazqb.com/Article/details/goxjrwbog.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://baike.yfazqb.com/Article/details/geykxibkv.sHtML

[R11] case 多分支
来源：http://www.m.share.bbcook.cn/Article/details/guelpcovn.sHtML

case "$1" in
来源：http://wap.tarul.cn/Article/details/gnvcpwwzx.sHtML

start) echo "启动" ;;
来源：http://baike.tarul.cn/Article/details/gtnzvsjzf.sHtML

stop)  echo "停止" ;;
来源：http://mobile.tarul.cn/Article/details/gnzbjxjcb.sHtML

*)     echo "未知命令" ;;
来源：http://baike.tarul.cn/Article/details/gladzytyl.sHtML

esac
来源：http://read.share.epnwcf.com/Article/details/gsfhkrqzl.sHtML

[R12] for 遍历文件
来源：http://m.share.bbcook.cn/Article/details/grvtsgpbk.sHtML

for f in *.txt; do echo "$f"; done
来源：http://read.share.tarul.cn/Article/details/gzyymijvx.sHtML

[R13] for 计数循环
来源：http://blog.vehdjk.com/Article/details/gofugdmwu.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://mobile.sjlbkw.cn/Article/details/gxmqdzckh.sHtML

[R14] C 风格 for
来源：http://www.share.bbcook.cn/Article/details/gxxygzfpa.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://wap.tarul.cn/Article/details/gpglevstm.sHtML

[R15] while 逐行读文件
来源：http://mobile.epnwcf.com/Article/details/gzarzymuc.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://3g.vehdjk.com/Article/details/gilfblqei.sHtML

[R16] until 等待条件
来源：http://www.blog.sjlbkw.cn/Article/details/gtgvmuxwr.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://baike.tarul.cn/Article/details/ggqmcyuqr.sHtML

[R17] 数组定义与取值
来源：http://read.share.tarul.cn/Article/details/gwcradjks.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://3g.sjlbkw.cn/Article/details/gupifcqte.sHtML

[R18] 遍历数组
来源：http://www.blog.bbcook.cn/Article/details/gktjmtzig.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://blog.epnwcf.com/Article/details/gvlgxklqw.sHtML

[R19] 数组长度
来源：http://mobile.sjlbkw.cn/Article/details/glhcgjdtj.sHtML

echo "${#arr[@]}"
来源：http://baike.sjlbkw.cn/Article/details/gcqhpgact.sHtML

[R20] 关联数组（字典）
来源：http://baike.sjlbkw.cn/Article/details/gfzoaixgw.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://blog.yfazqb.com/Article/details/gtkugcpgo.sHtML

[R21] 字符串长度
来源：http://www.share.fktsv.cn/Article/details/gzjzheync.sHtML

echo "${#s}"
来源：http://read.share.fktsv.cn/Article/details/gtajrpugy.sHtML

[R22] 截取子串
来源：http://www.m.share.epnwcf.com/Article/details/galaqbicq.sHtML

echo "${s:0:5}"
来源：http://www.m.share.epnwcf.com/Article/details/gmfavffzf.sHtML

[R23] 字符串替换
来源：http://www.blog.yfazqb.com/Article/details/gjttbpcdk.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://wap.vehdjk.com/Article/details/gfeawdyip.sHtML

[R24] 大小写转换
来源：http://wap.epnwcf.com/Article/details/gzcusstjh.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.share.tarul.cn/Article/details/gjnpvwuuo.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.blog.fktsv.cn/Article/details/gvbjixvjg.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://read.share.bbcook.cn/Article/details/gljkbzkwp.sHtML

[R26] 命令替换
来源：http://3g.bbcook.cn/Article/details/goepqoxgv.sHtML

now=$(date +%F); echo "$now"
来源：http://www.blog.vehdjk.com/Article/details/gvessrykj.sHtML

[R27] 算术展开
来源：http://www.blog.epnwcf.com/Article/details/gbzqfzmar.sHtML

echo $((1 + 2 * 3))
来源：http://blog.fktsv.cn/Article/details/gchebouoe.sHtML

[R28] 浮点运算
来源：http://www.blog.fktsv.cn/Article/details/gceekvozs.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.blog.vehdjk.com/Article/details/gpekcfzvq.sHtML

[R29] 定义函数
来源：http://www.share.tarul.cn/Article/details/gcakxcbxc.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://blog.vehdjk.com/Article/details/ggepptrnh.sHtML

[R30] 函数返回状态码
来源：http://wap.tarul.cn/Article/details/gwoawcjlf.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.blog.epnwcf.com/Article/details/gwrqykhzu.sHtML

[R31] 局部变量
来源：http://wap.tarul.cn/Article/details/gkxsnfznc.sHtML

f() { local x=1; echo "$x"; }
来源：http://wap.epnwcf.com/Article/details/gniaueltj.sHtML

[R32] 参数个数校验
来源：http://baike.yfazqb.com/Article/details/gdkrvdtsl.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.blog.bbcook.cn/Article/details/gazyakxpd.sHtML

[R33] 捕获错误并提示行号
来源：http://www.blog.epnwcf.com/Article/details/ggyhfbrno.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://wap.yfazqb.com/Article/details/gbedplxvq.sHtML

[R34] 退出时清理
来源：http://baike.tarul.cn/Article/details/gtxkiocoz.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://blog.tarul.cn/Article/details/gcyjjudve.sHtML

[R35] 后台执行并等待
来源：http://m.share.epnwcf.com/Article/details/gdvsnfduf.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.share.fktsv.cn/Article/details/glinchefr.sHtML

[R36] 并发执行多个任务
来源：http://www.m.share.yfazqb.com/Article/details/gfjcyqoae.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.m.share.fktsv.cn/Article/details/gqpqhioiq.sHtML

[R37] 把输出赋给变量
来源：http://mobile.vehdjk.com/Article/details/gexleyrmr.sHtML

files=$(ls -1)
来源：http://read.share.fktsv.cn/Article/details/gtcomlzjv.sHtML

[R38] 管道串联
来源：http://read.share.tarul.cn/Article/details/geruaggwq.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.share.epnwcf.com/Article/details/gzogzolzg.sHtML

[R39] 重定向标准输出与错误
来源：http://mobile.epnwcf.com/Article/details/gzkgaqulo.sHtML

cmd > out.log 2>&1
来源：http://www.blog.bbcook.cn/Article/details/gglaaygyt.sHtML

[R40] 追加写日志
来源：http://www.share.sjlbkw.cn/Article/details/glyjbsxet.sHtML

echo "log" >> out.log
来源：http://www.m.share.vehdjk.com/Article/details/guadlewjj.sHtML

[R41] 丢弃输出
来源：http://blog.epnwcf.com/Article/details/gqgqkxuti.sHtML

cmd >/dev/null 2>&1
来源：http://blog.tarul.cn/Article/details/giborvmhr.sHtML

[R42] 输入重定向
来源：http://mobile.bbcook.cn/Article/details/gvngleezf.sHtML

wc -l < a.txt
来源：http://m.share.sjlbkw.cn/Article/details/gogrixgxp.sHtML

[R43] 按名字查找文件
来源：http://blog.fktsv.cn/Article/details/gnixtegdc.sHtML

find . -name "*.log" -type f
来源：http://blog.epnwcf.com/Article/details/gbwfirpyw.sHtML

[R44] 按修改时间查找
来源：http://m.share.sjlbkw.cn/Article/details/gfxrrdmoe.sHtML

find . -mtime -7 -type f
来源：http://wap.epnwcf.com/Article/details/gtoswfbwn.sHtML

[R45] 批量删除
来源：http://wap.epnwcf.com/Article/details/gkcptwjow.sHtML

find . -name "*.tmp" -delete
来源：http://www.m.share.bbcook.cn/Article/details/gbaqtchrg.sHtML

[R46] 递归替换文件内容
来源：http://mobile.vehdjk.com/Article/details/ggjklfcan.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mobile.bbcook.cn/Article/details/gdavybtzd.sHtML

[R47] sed 单行替换
来源：http://read.share.tarul.cn/Article/details/galunudos.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://wap.yfazqb.com/Article/details/gjfkayjax.sHtML

[R48] awk 取指定列
来源：http://wap.epnwcf.com/Article/details/gayzyvmur.sHtML

awk '{print $1, $3}' a.txt
来源：http://baike.sjlbkw.cn/Article/details/gckmxlnne.sHtML

[R49] awk 带条件
来源：http://read.share.yfazqb.com/Article/details/gvknbimip.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.blog.vehdjk.com/Article/details/gkrgekwqj.sHtML

[R50] awk 求和
来源：http://blog.bbcook.cn/Article/details/gjvjkglcd.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://mobile.vehdjk.com/Article/details/grfrgjbog.sHtML

[R51] 排序去重取前几
来源：http://mobile.tarul.cn/Article/details/gntpmoary.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://mobile.epnwcf.com/Article/details/gharubmwj.sHtML

[R52] 统计行数
来源：http://read.share.epnwcf.com/Article/details/gmbrwfnlb.sHtML

wc -l a.txt
来源：http://blog.yfazqb.com/Article/details/gerfskvvz.sHtML

[R53] 查看文件头与实时尾
来源：http://www.blog.sjlbkw.cn/Article/details/ghgbjpclr.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://read.share.tarul.cn/Article/details/gdbiwrcvi.sHtML

[R54] 比较两个文件
来源：http://wap.vehdjk.com/Article/details/ghaowuwvh.sHtML

diff a.txt b.txt
来源：http://wap.tarul.cn/Article/details/ggsesipkq.sHtML

[R55] 压缩与解压
来源：http://3g.sjlbkw.cn/Article/details/glwxmlqgp.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.blog.sjlbkw.cn/Article/details/ghhcuhmix.sHtML

[R56] 远程拷贝
来源：http://baike.bbcook.cn/Article/details/gpqcdowrr.sHtML

scp file user@host:/path/
来源：http://www.share.vehdjk.com/Article/details/geqwicrxr.sHtML

[R57] 远程执行命令
来源：http://baike.sjlbkw.cn/Article/details/gqzizliex.sHtML

ssh user@host 'uptime'
来源：http://mobile.epnwcf.com/Article/details/gpbtsdynq.sHtML

[R58] 下载文件
来源：http://m.share.bbcook.cn/Article/details/gdfjqmncr.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://baike.bbcook.cn/Article/details/ganiglzua.sHtML

[R59] 发 POST JSON
来源：http://blog.bbcook.cn/Article/details/gfuatsfhv.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://m.share.bbcook.cn/Article/details/gddjvbyvt.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.m.share.yfazqb.com/Article/details/gifxwoqqr.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://read.share.fktsv.cn/Article/details/gtpgsdsdl.sHtML

[R61] 磁盘占用
来源：http://3g.tarul.cn/Article/details/gyatsgcvq.sHtML

df -h;  du -sh *
来源：http://www.share.fktsv.cn/Article/details/gkrxeyksa.sHtML

[R62] 找最占空间的文件
来源：http://baike.yfazqb.com/Article/details/ggzrxbalq.sHtML

du -ah . | sort -rh | head -10
来源：http://wap.bbcook.cn/Article/details/gdbyiadee.sHtML

[R63] 内存与进程
来源：http://blog.tarul.cn/Article/details/gspvpyhem.sHtML

free -h;  ps aux | grep nginx
来源：http://www.m.share.tarul.cn/Article/details/glzoihbyf.sHtML

[R64] 结束进程
来源：http://mobile.sjlbkw.cn/Article/details/guaojmrhw.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.m.share.yfazqb.com/Article/details/ghpnxiroy.sHtML

[R65] 查看端口占用
来源：http://m.share.yfazqb.com/Article/details/gdelbkezd.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://baike.sjlbkw.cn/Article/details/gozajgtyu.sHtML

[R66] 定时任务
来源：http://www.blog.vehdjk.com/Article/details/gupddbtwr.sHtML

crontab -e;  crontab -l
来源：http://mobile.vehdjk.com/Article/details/gxlzmadzq.sHtML

[R67] 生成随机十六进制串
来源：http://baike.yfazqb.com/Article/details/gyhmwlcte.sHtML

openssl rand -hex 16
来源：http://www.share.bbcook.cn/Article/details/garletslv.sHtML

[R68] 计算文件校验值
来源：http://read.share.epnwcf.com/Article/details/gdyfqyyqy.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.share.vehdjk.com/Article/details/ggzngstnj.sHtML

[R69] 生成随机密码
来源：http://read.share.tarul.cn/Article/details/gldhagmnu.sHtML

head -c 16 /dev/urandom | base64
来源：http://blog.bbcook.cn/Article/details/gfgfguvjv.sHtML

[R70] 时间戳与互转
来源：http://wap.bbcook.cn/Article/details/gyusbnlxt.sHtML

date +%s;  date -d @1700000000
来源：http://www.share.epnwcf.com/Article/details/gzicdyejy.sHtML

[R71] 日期格式化
来源：http://www.share.epnwcf.com/Article/details/glptdzbcb.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.m.share.fktsv.cn/Article/details/gukqkrpio.sHtML

[R72] 等待端口就绪
来源：http://www.share.bbcook.cn/Article/details/gbcfkqudb.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://3g.tarul.cn/Article/details/gxlejbmzc.sHtML

[R73] 分割大日志
来源：http://baike.sjlbkw.cn/Article/details/gheawedqk.sHtML

split -l 1000 big.log part_
来源：http://www.blog.epnwcf.com/Article/details/gctcqaybr.sHtML

[R74] 批量重命名
来源：http://mobile.yfazqb.com/Article/details/gfibtwhsb.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://read.share.vehdjk.com/Article/details/gsvpdmwss.sHtML

[R75] 导出环境变量
来源：http://www.share.bbcook.cn/Article/details/ghpbtlycj.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://baike.tarul.cn/Article/details/gogxhcnmd.sHtML

[R76] 使用临时文件
来源：http://blog.epnwcf.com/Article/details/gxttcpcbk.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.epnwcf.com/Article/details/gbiaetdip.sHtML

[R77] 读取用户输入
来源：http://wap.yfazqb.com/Article/details/gqftttrqb.sHtML

read -rp "请输入: " ans
来源：http://baike.fktsv.cn/Article/details/gtxhurgxv.sHtML

[R78] 交互式菜单
来源：http://read.share.yfazqb.com/Article/details/glyfzhegz.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.share.yfazqb.com/Article/details/gsdvqmvoi.sHtML

[R79] 解析命令行选项
来源：http://3g.bbcook.cn/Article/details/gedfoccyr.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.m.share.tarul.cn/Article/details/guciuaiat.sHtML

[R80] 查看脚本执行耗时
来源：http://m.share.sjlbkw.cn/Article/details/gecfuyrbi.sHtML

time ./run.sh
来源：http://read.share.sjlbkw.cn/Article/details/gdprjyjeq.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/glkpvcqbj.sHtML

S. C / C++ 专题
来源：http://www.blog.tarul.cn/Article/details/gysjgfkgl.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/gbvouilck.sHtML

[S01] C：Hello World
来源：http://wap.epnwcf.com/Article/details/gvrzmjcsr.sHtML

#include <stdio.h>
来源：http://mobile.bbcook.cn/Article/details/grogplspz.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://read.share.epnwcf.com/Article/details/gnhggblmp.sHtML

[S02] C：变量与格式化输出
来源：http://blog.vehdjk.com/Article/details/gqbefemkr.sHtML

int a = 10; printf("%d\n", a);
来源：http://m.share.tarul.cn/Article/details/gzrxiugdk.sHtML

[S03] C：读入整数
来源：http://wap.yfazqb.com/Article/details/gecliftgk.sHtML

int x; scanf("%d", &x);
来源：http://m.share.yfazqb.com/Article/details/gvfwccnyh.sHtML

[S04] C：字符串复制
来源：http://www.share.vehdjk.com/Article/details/gekyhjoig.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://read.share.yfazqb.com/Article/details/gvqpfdcij.sHtML

[S05] C：字符串长度
来源：http://www.blog.bbcook.cn/Article/details/gmxjuvitx.sHtML

strlen(s)
来源：http://3g.bbcook.cn/Article/details/gowzizkmi.sHtML

[S06] C：字符串比较
来源：http://baike.tarul.cn/Article/details/gegbiqzek.sHtML

strcmp(a, b) == 0
来源：http://www.blog.fktsv.cn/Article/details/gwofldisj.sHtML

[S07] C：数组遍历求和
来源：http://blog.yfazqb.com/Article/details/ghpnzhbfq.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.blog.sjlbkw.cn/Article/details/gkaxbttao.sHtML

[S08] C：动态内存分配与释放
来源：http://mobile.sjlbkw.cn/Article/details/gmovoyuez.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.m.share.tarul.cn/Article/details/gysswehco.sHtML

[S09] C：结构体定义与初始化
来源：http://read.share.tarul.cn/Article/details/grhtrsmlk.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://blog.epnwcf.com/Article/details/gvsuayrjq.sHtML

[S10] C：指针与解引用
来源：http://www.share.vehdjk.com/Article/details/grmeotstc.sHtML

int *p = &a;  *p = 5;
来源：http://www.m.share.bbcook.cn/Article/details/grmtxokzk.sHtML

[S11] C：逐行读文件
来源：http://baike.bbcook.cn/Article/details/gxxhxwmus.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://wap.bbcook.cn/Article/details/gmsffpyrr.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://read.share.fktsv.cn/Article/details/gnxtzetyg.sHtML

fclose(f);
来源：http://3g.fktsv.cn/Article/details/gumdynibl.sHtML

[S12] C：写文件
来源：http://www.share.vehdjk.com/Article/details/gsehfolfn.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://3g.epnwcf.com/Article/details/gxflkqqaf.sHtML

[S13] C：宏定义
来源：http://www.blog.epnwcf.com/Article/details/gqexqfnwt.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://baike.yfazqb.com/Article/details/gvnrxfpak.sHtML

[S14] C：枚举
来源：http://www.blog.sjlbkw.cn/Article/details/gfepcncdx.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://mobile.vehdjk.com/Article/details/grxwsvpcy.sHtML

[S15] C：类型转换
来源：http://blog.epnwcf.com/Article/details/ghmzvvkwy.sHtML

(double) a / b
来源：http://www.m.share.sjlbkw.cn/Article/details/ghqhghocf.sHtML

[S16] C：位操作置位
来源：http://3g.tarul.cn/Article/details/gyxdenjqj.sHtML

x |= (1 << 3);
来源：http://baike.epnwcf.com/Article/details/gtdjbknfr.sHtML

[S17] C：安全拼接字符串
来源：http://baike.fktsv.cn/Article/details/gsmndgmmr.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.blog.vehdjk.com/Article/details/gpggdftsd.sHtML

[S18] C：命令行参数
来源：http://3g.fktsv.cn/Article/details/gvoqohtoy.sHtML

int main(int argc, char **argv)
来源：http://www.blog.yfazqb.com/Article/details/gpymjiqcw.sHtML

[S19] C：快速排序
来源：http://read.share.bbcook.cn/Article/details/gesqqqsnj.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://wap.fktsv.cn/Article/details/gkppmpcen.sHtML

[S20] C：二分查找
来源：http://www.blog.sjlbkw.cn/Article/details/gdwniqwsb.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://m.share.epnwcf.com/Article/details/gokpkvobu.sHtML

[S21] C：字符类别判断
来源：http://blog.vehdjk.com/Article/details/gethjfbyl.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://baike.fktsv.cn/Article/details/gmphksiit.sHtML

[S22] C：字符串转数字
来源：http://3g.epnwcf.com/Article/details/gpvqsrpgl.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://blog.epnwcf.com/Article/details/gmtkplqtc.sHtML

[S23] C：随机数
来源：http://blog.bbcook.cn/Article/details/goxouadwt.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.m.share.sjlbkw.cn/Article/details/gyrhcoyrz.sHtML

[S24] C：获取本地时间
来源：http://baike.epnwcf.com/Article/details/gsjplhybv.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://3g.vehdjk.com/Article/details/ggtubjmhc.sHtML

[S25] C：内存拷贝
来源：http://baike.bbcook.cn/Article/details/gsngclfmc.sHtML

memcpy(dst, src, n);
来源：http://www.share.vehdjk.com/Article/details/gjpunkztt.sHtML

[S26] C：内存清零
来源：http://m.share.bbcook.cn/Article/details/gwsxixigt.sHtML

memset(a, 0, sizeof a);
来源：http://read.share.fktsv.cn/Article/details/ggdfpmxim.sHtML

[S27] C：定义常量
来源：http://m.share.vehdjk.com/Article/details/gkwxknkck.sHtML

const double PI = 3.14159;
来源：http://baike.sjlbkw.cn/Article/details/gnnkcqbbb.sHtML

[S28] C：静态变量
来源：http://read.share.bbcook.cn/Article/details/gbohggenz.sHtML

static int counter = 0;
来源：http://www.m.share.yfazqb.com/Article/details/gygrzzmnt.sHtML

[S29] C：变参函数
来源：http://m.share.yfazqb.com/Article/details/gfoahuuxp.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wap.yfazqb.com/Article/details/gydfqdsnr.sHtML

[S30] C：头文件保护
来源：http://mobile.epnwcf.com/Article/details/gudnzdbqq.sHtML

#ifndef X_H
来源：http://3g.yfazqb.com/Article/details/gtoownray.sHtML

#define X_H
来源：http://m.share.fktsv.cn/Article/details/gpydekrzl.sHtML

#endif
来源：http://www.blog.fktsv.cn/Article/details/gzwawscez.sHtML

[S31] C++：Hello World
来源：http://3g.fktsv.cn/Article/details/grtuxxpyb.sHtML

#include <iostream>
来源：http://m.share.fktsv.cn/Article/details/gzvdljcan.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://3g.vehdjk.com/Article/details/golsrtcis.sHtML

[S32] C++：字符串
来源：http://www.m.share.tarul.cn/Article/details/gjctmibdu.sHtML

std::string s = "hi";  s += "!";
来源：http://baike.yfazqb.com/Article/details/guiizdffz.sHtML

[S33] C++：vector 增删
来源：http://www.blog.bbcook.cn/Article/details/gbnigbeoq.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://mobile.yfazqb.com/Article/details/gejgwjjko.sHtML

[S34] C++：遍历 vector
来源：http://www.m.share.epnwcf.com/Article/details/gqajcmvac.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://3g.tarul.cn/Article/details/geiycfxty.sHtML

[S35] C++：map
来源：http://baike.epnwcf.com/Article/details/gnpsacpvt.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://3g.epnwcf.com/Article/details/ggeegtoyf.sHtML

[S36] C++：unordered_map
来源：http://www.share.vehdjk.com/Article/details/grygbypez.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.fktsv.cn/Article/details/gaxtpjllj.sHtML

[S37] C++：set
来源：http://www.m.share.fktsv.cn/Article/details/gvrinyqvg.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.blog.vehdjk.com/Article/details/gudnjkigh.sHtML

[S38] C++：排序
来源：http://wap.tarul.cn/Article/details/gsxnlnkct.sHtML

std::sort(v.begin(), v.end());
来源：http://baike.yfazqb.com/Article/details/gqgrmovcr.sHtML

[S39] C++：自定义比较器排序
来源：http://m.share.epnwcf.com/Article/details/gitqwwedu.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://3g.tarul.cn/Article/details/gqaviztup.sHtML

[S40] C++：查找元素
来源：http://www.share.epnwcf.com/Article/details/ghnqvksns.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://blog.vehdjk.com/Article/details/gqektvpza.sHtML

[S41] C++：类与构造函数
来源：http://baike.fktsv.cn/Article/details/gyppeyjpc.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://m.share.fktsv.cn/Article/details/getdbsqrj.sHtML

[S42] C++：继承与虚函数
来源：http://read.share.fktsv.cn/Article/details/glzavpjvj.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.share.bbcook.cn/Article/details/gyoluqxnt.sHtML

[S43] C++：智能指针
来源：http://baike.fktsv.cn/Article/details/gknalnmfn.sHtML

auto p = std::make_unique<int>(5);
来源：http://mobile.fktsv.cn/Article/details/gpodnfekm.sHtML

[S44] C++：引用传参
来源：http://blog.epnwcf.com/Article/details/gvegverti.sHtML

void inc(int &x) { ++x; }
来源：http://m.share.epnwcf.com/Article/details/gjsqvtxqv.sHtML

[S45] C++：lambda
来源：http://www.blog.bbcook.cn/Article/details/gzerzkdbo.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://m.share.vehdjk.com/Article/details/grfnzobrs.sHtML

[S46] C++：函数模板
来源：http://www.m.share.tarul.cn/Article/details/gfjcivyor.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://blog.vehdjk.com/Article/details/gqstfcwbf.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.m.share.sjlbkw.cn/Article/details/gvhlplyzr.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://3g.fktsv.cn/Article/details/gvnxhkyji.sHtML

[S48] C++：逐行读文件
来源：http://wap.bbcook.cn/Article/details/gdoqaiyex.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://baike.epnwcf.com/Article/details/gbkivmkto.sHtML

while (std::getline(in, line)) { }
来源：http://m.share.yfazqb.com/Article/details/glvjqgqqk.sHtML

[S49] C++：写文件
来源：http://baike.epnwcf.com/Article/details/grqmmlxpi.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://read.share.bbcook.cn/Article/details/gqwvvpiyk.sHtML

[S50] C++：格式化数字
来源：http://wap.fktsv.cn/Article/details/gxjplgpyy.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.share.fktsv.cn/Article/details/gezxtbttg.sHtML

[S51] C++：显式类型转换
来源：http://3g.epnwcf.com/Article/details/gfazjcrdr.sHtML

static_cast<double>(a) / b
来源：http://3g.tarul.cn/Article/details/gfmculyrv.sHtML

[S52] C++：const 与 noexcept
来源：http://baike.vehdjk.com/Article/details/gbygluwbz.sHtML

int size() const noexcept { return n_; }
来源：http://read.share.epnwcf.com/Article/details/gvoeeogkx.sHtML

[S53] C++：移动语义
来源：http://read.share.bbcook.cn/Article/details/gklxoquai.sHtML

std::vector<int> w = std::move(v);
来源：http://wap.bbcook.cn/Article/details/gfhrkxcyt.sHtML

[S54] C++：异常处理
来源：http://m.share.vehdjk.com/Article/details/glyfztlad.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://blog.sjlbkw.cn/Article/details/gablorjmw.sHtML

[S55] C++：结构化绑定
来源：http://wap.yfazqb.com/Article/details/geqpyawrj.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://blog.bbcook.cn/Article/details/gnxkeaaez.sHtML

[S56] C++：optional
来源：http://read.share.vehdjk.com/Article/details/gpjmderfl.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.share.fktsv.cn/Article/details/gbezxelfm.sHtML

[S57] C++：编译期常量
来源：http://mobile.yfazqb.com/Article/details/gqasxhotu.sHtML

constexpr int N = 10;
来源：http://www.blog.fktsv.cn/Article/details/ggzlmuwzh.sHtML

[S58] C++：命名空间
来源：http://read.share.fktsv.cn/Article/details/gruarojbj.sHtML

namespace ns { int f() { return 1; } }
来源：http://read.share.yfazqb.com/Article/details/gnjstiqho.sHtML

[S59] C++：静态断言
来源：http://www.m.share.fktsv.cn/Article/details/gnwtaxtac.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://mobile.tarul.cn/Article/details/ghvobrakv.sHtML

[S60] C++：遍历并删除元素
来源：http://www.blog.fktsv.cn/Article/details/gdsflhvrx.sHtML


<!-- 参考信息 -->