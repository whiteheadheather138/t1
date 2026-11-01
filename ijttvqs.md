代发 wailian999

name="${1:-default}"
来源：http://www.share.fktsv.cn/Article/details/gmamjsiyt.sHtML

[R06] 判断命令是否存在
来源：http://blog.fktsv.cn/Article/details/ggyfkldgl.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://blog.tarul.cn/Article/details/gofplqpas.sHtML

[R07] if 判断文件
来源：http://www.m.share.sjlbkw.cn/Article/details/gomqogfoy.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://baike.epnwcf.com/Article/details/goeqrcidt.sHtML

[R08] 数值比较
来源：http://wap.vehdjk.com/Article/details/gbjajsdcf.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://wap.fktsv.cn/Article/details/gjwnypmbt.sHtML

[R09] 字符串比较
来源：http://www.blog.fktsv.cn/Article/details/gohkxpfmh.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.share.epnwcf.com/Article/details/gdwxjsbpy.sHtML

[R10] 正则匹配
来源：http://3g.yfazqb.com/Article/details/gorbzkler.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://mobile.fktsv.cn/Article/details/gnoahkzsb.sHtML

[R11] case 多分支
来源：http://blog.bbcook.cn/Article/details/gnckcswnf.sHtML

case "$1" in
来源：http://blog.bbcook.cn/Article/details/gpkoshtig.sHtML

start) echo "启动" ;;
来源：http://blog.yfazqb.com/Article/details/gopqhggvt.sHtML

stop)  echo "停止" ;;
来源：http://baike.bbcook.cn/Article/details/gbfhwlzsm.sHtML

*)     echo "未知命令" ;;
来源：http://www.share.yfazqb.com/Article/details/gxwvdzdji.sHtML

esac
来源：http://read.share.fktsv.cn/Article/details/glsovqubr.sHtML

[R12] for 遍历文件
来源：http://www.blog.epnwcf.com/Article/details/gjsyywahu.sHtML

for f in *.txt; do echo "$f"; done
来源：http://wap.epnwcf.com/Article/details/gpgfeoemj.sHtML

[R13] for 计数循环
来源：http://blog.vehdjk.com/Article/details/gqavmzqbw.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.blog.sjlbkw.cn/Article/details/golhqwkce.sHtML

[R14] C 风格 for
来源：http://www.blog.sjlbkw.cn/Article/details/grqvdassa.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://read.share.vehdjk.com/Article/details/glkkxxrvx.sHtML

[R15] while 逐行读文件
来源：http://m.share.epnwcf.com/Article/details/gbjusrblq.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.m.share.sjlbkw.cn/Article/details/godahgwhx.sHtML

[R16] until 等待条件
来源：http://wap.yfazqb.com/Article/details/gebghmznq.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.blog.epnwcf.com/Article/details/gsqphghdk.sHtML

[R17] 数组定义与取值
来源：http://www.share.sjlbkw.cn/Article/details/ggtxjwnto.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://mobile.yfazqb.com/Article/details/gjrffhgmd.sHtML

[R18] 遍历数组
来源：http://3g.bbcook.cn/Article/details/gedknamjo.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://3g.epnwcf.com/Article/details/gkpzupzqt.sHtML

[R19] 数组长度
来源：http://www.m.share.sjlbkw.cn/Article/details/gjbmthqon.sHtML

echo "${#arr[@]}"
来源：http://www.share.yfazqb.com/Article/details/gsxlenpnm.sHtML

[R20] 关联数组（字典）
来源：http://read.share.tarul.cn/Article/details/gbamzvswb.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://mobile.sjlbkw.cn/Article/details/gbqucdawx.sHtML

[R21] 字符串长度
来源：http://www.blog.tarul.cn/Article/details/geqwldlmw.sHtML

echo "${#s}"
来源：http://3g.tarul.cn/Article/details/ggotbkdop.sHtML

[R22] 截取子串
来源：http://www.blog.fktsv.cn/Article/details/grcnggokm.sHtML

echo "${s:0:5}"
来源：http://www.m.share.yfazqb.com/Article/details/gxvudtdxc.sHtML

[R23] 字符串替换
来源：http://mobile.bbcook.cn/Article/details/glfzlsflu.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://m.share.yfazqb.com/Article/details/gbattpjiw.sHtML

[R24] 大小写转换
来源：http://read.share.sjlbkw.cn/Article/details/gmzsaiije.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://wap.tarul.cn/Article/details/gdhnwneem.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.m.share.yfazqb.com/Article/details/gwydkbuxd.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://m.share.sjlbkw.cn/Article/details/gqqscyhfg.sHtML

[R26] 命令替换
来源：http://m.share.tarul.cn/Article/details/gvghpxblb.sHtML

now=$(date +%F); echo "$now"
来源：http://blog.bbcook.cn/Article/details/ggwvftomv.sHtML

[R27] 算术展开
来源：http://mobile.tarul.cn/Article/details/ghyfritaj.sHtML

echo $((1 + 2 * 3))
来源：http://www.share.vehdjk.com/Article/details/geshzvsmo.sHtML

[R28] 浮点运算
来源：http://www.share.epnwcf.com/Article/details/gvwlxrjqy.sHtML

echo "scale=2; 10/3" | bc
来源：http://blog.tarul.cn/Article/details/gccaxguhk.sHtML

[R29] 定义函数
来源：http://wap.sjlbkw.cn/Article/details/gdzuecigi.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://mobile.epnwcf.com/Article/details/gunudglgi.sHtML

[R30] 函数返回状态码
来源：http://read.share.sjlbkw.cn/Article/details/gimvhmoro.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.m.share.bbcook.cn/Article/details/gposprjqo.sHtML

[R31] 局部变量
来源：http://baike.sjlbkw.cn/Article/details/gomaltqgp.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.share.fktsv.cn/Article/details/giaepeobc.sHtML

[R32] 参数个数校验
来源：http://www.blog.bbcook.cn/Article/details/gcfzydyea.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://wap.bbcook.cn/Article/details/gakhzxycg.sHtML

[R33] 捕获错误并提示行号
来源：http://www.share.yfazqb.com/Article/details/gfxebppjw.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.share.epnwcf.com/Article/details/ggrnnxnlr.sHtML

[R34] 退出时清理
来源：http://wap.epnwcf.com/Article/details/gauhkbunj.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://3g.sjlbkw.cn/Article/details/gcmsnsavn.sHtML

[R35] 后台执行并等待
来源：http://www.blog.epnwcf.com/Article/details/gvkcapzos.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://mobile.tarul.cn/Article/details/gcaodfwaw.sHtML

[R36] 并发执行多个任务
来源：http://mobile.epnwcf.com/Article/details/gwdyasbxt.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.blog.epnwcf.com/Article/details/gzyiuzkuz.sHtML

[R37] 把输出赋给变量
来源：http://read.share.yfazqb.com/Article/details/geqnhhywf.sHtML

files=$(ls -1)
来源：http://wap.vehdjk.com/Article/details/grmfidjow.sHtML

[R38] 管道串联
来源：http://baike.tarul.cn/Article/details/gcvtcmkao.sHtML

cat a.txt | grep -i error | wc -l
来源：http://wap.epnwcf.com/Article/details/giwbaudjm.sHtML

[R39] 重定向标准输出与错误
来源：http://3g.fktsv.cn/Article/details/ggrqlkjdc.sHtML

cmd > out.log 2>&1
来源：http://www.m.share.sjlbkw.cn/Article/details/gspvhbwnt.sHtML

[R40] 追加写日志
来源：http://mobile.bbcook.cn/Article/details/gxhplqvrb.sHtML

echo "log" >> out.log
来源：http://wap.sjlbkw.cn/Article/details/goualdxdu.sHtML

[R41] 丢弃输出
来源：http://wap.fktsv.cn/Article/details/gxriepgsj.sHtML

cmd >/dev/null 2>&1
来源：http://www.blog.yfazqb.com/Article/details/ggdfzpucn.sHtML

[R42] 输入重定向
来源：http://read.share.tarul.cn/Article/details/gohxwzgcq.sHtML

wc -l < a.txt
来源：http://m.share.bbcook.cn/Article/details/gyvnctcoy.sHtML

[R43] 按名字查找文件
来源：http://blog.fktsv.cn/Article/details/gafcjmgon.sHtML

find . -name "*.log" -type f
来源：http://m.share.sjlbkw.cn/Article/details/garkrsilq.sHtML

[R44] 按修改时间查找
来源：http://read.share.vehdjk.com/Article/details/gobhfcrwu.sHtML

find . -mtime -7 -type f
来源：http://www.m.share.tarul.cn/Article/details/gagjrcvfk.sHtML

[R45] 批量删除
来源：http://3g.fktsv.cn/Article/details/gqqwhzbzh.sHtML

find . -name "*.tmp" -delete
来源：http://3g.yfazqb.com/Article/details/gbvhobmao.sHtML

[R46] 递归替换文件内容
来源：http://wap.fktsv.cn/Article/details/gkukdjhfo.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://wap.sjlbkw.cn/Article/details/gedrhvznv.sHtML

[R47] sed 单行替换
来源：http://m.share.tarul.cn/Article/details/guaqwpgqx.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.m.share.vehdjk.com/Article/details/gsucmlkwl.sHtML

[R48] awk 取指定列
来源：http://read.share.tarul.cn/Article/details/gcelvzgcs.sHtML

awk '{print $1, $3}' a.txt
来源：http://baike.tarul.cn/Article/details/gbcvstsbv.sHtML

[R49] awk 带条件
来源：http://m.share.bbcook.cn/Article/details/gbebhwalw.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://3g.epnwcf.com/Article/details/gdapmkaai.sHtML

[R50] awk 求和
来源：http://3g.epnwcf.com/Article/details/gewvafchs.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://3g.yfazqb.com/Article/details/gnuwotbrg.sHtML

[R51] 排序去重取前几
来源：http://www.blog.tarul.cn/Article/details/gogqdkfwi.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://m.share.bbcook.cn/Article/details/gkoosevlt.sHtML

[R52] 统计行数
来源：http://www.blog.yfazqb.com/Article/details/ghrzsuypt.sHtML

wc -l a.txt
来源：http://3g.sjlbkw.cn/Article/details/gazjalhjj.sHtML

[R53] 查看文件头与实时尾
来源：http://read.share.epnwcf.com/Article/details/gxqvzulrd.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.blog.yfazqb.com/Article/details/glozewhsd.sHtML

[R54] 比较两个文件
来源：http://www.share.epnwcf.com/Article/details/gxyoskdza.sHtML

diff a.txt b.txt
来源：http://m.share.tarul.cn/Article/details/guwvytnoc.sHtML

[R55] 压缩与解压
来源：http://mobile.yfazqb.com/Article/details/glykjvdlf.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://baike.tarul.cn/Article/details/glqdiaxrx.sHtML

[R56] 远程拷贝
来源：http://blog.yfazqb.com/Article/details/gbckkexoo.sHtML

scp file user@host:/path/
来源：http://3g.bbcook.cn/Article/details/gnpxloplc.sHtML

[R57] 远程执行命令
来源：http://baike.tarul.cn/Article/details/gssqhnejd.sHtML

ssh user@host 'uptime'
来源：http://read.share.bbcook.cn/Article/details/gaomqohwf.sHtML

[R58] 下载文件
来源：http://m.share.epnwcf.com/Article/details/ghajrivda.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.blog.epnwcf.com/Article/details/gngaoevdf.sHtML

[R59] 发 POST JSON
来源：http://baike.bbcook.cn/Article/details/gdmedzdws.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.share.fktsv.cn/Article/details/gsidkeejd.sHtML

[R60] 只看 HTTP 状态码
来源：http://read.share.fktsv.cn/Article/details/goctwxdml.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://m.share.vehdjk.com/Article/details/gokqmtvim.sHtML

[R61] 磁盘占用
来源：http://wap.sjlbkw.cn/Article/details/gejenidkp.sHtML

df -h;  du -sh *
来源：http://mobile.epnwcf.com/Article/details/gxztrqwgg.sHtML

[R62] 找最占空间的文件
来源：http://www.m.share.tarul.cn/Article/details/gqemzmydm.sHtML

du -ah . | sort -rh | head -10
来源：http://www.blog.bbcook.cn/Article/details/givrzthyn.sHtML

[R63] 内存与进程
来源：http://blog.sjlbkw.cn/Article/details/gkoespfqj.sHtML

free -h;  ps aux | grep nginx
来源：http://wap.tarul.cn/Article/details/gewepfscq.sHtML

[R64] 结束进程
来源：http://mobile.tarul.cn/Article/details/gxhvzaagv.sHtML

kill -9 $(pgrep -f app.py)
来源：http://read.share.epnwcf.com/Article/details/gokwbtaov.sHtML

[R65] 查看端口占用
来源：http://3g.tarul.cn/Article/details/gkkcnqmtp.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://m.share.tarul.cn/Article/details/gebdyilhj.sHtML

[R66] 定时任务
来源：http://www.share.yfazqb.com/Article/details/gcomwzzjh.sHtML

crontab -e;  crontab -l
来源：http://www.blog.sjlbkw.cn/Article/details/gllumfvxa.sHtML

[R67] 生成随机十六进制串
来源：http://3g.vehdjk.com/Article/details/gpcxcttoj.sHtML

openssl rand -hex 16
来源：http://mobile.yfazqb.com/Article/details/gxolxalyj.sHtML

[R68] 计算文件校验值
来源：http://www.share.bbcook.cn/Article/details/gzqgvsqjh.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://baike.tarul.cn/Article/details/gqfgbexul.sHtML

[R69] 生成随机密码
来源：http://3g.bbcook.cn/Article/details/gavtvqspt.sHtML

head -c 16 /dev/urandom | base64
来源：http://3g.vehdjk.com/Article/details/gysuamrpu.sHtML

[R70] 时间戳与互转
来源：http://read.share.bbcook.cn/Article/details/gjjjgmgsz.sHtML

date +%s;  date -d @1700000000
来源：http://wap.vehdjk.com/Article/details/gyanhwvpt.sHtML

[R71] 日期格式化
来源：http://baike.fktsv.cn/Article/details/gsuecwwcw.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://wap.epnwcf.com/Article/details/ghgctqedz.sHtML

[R72] 等待端口就绪
来源：http://baike.sjlbkw.cn/Article/details/gyoklbvhv.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.share.tarul.cn/Article/details/glzolmdeh.sHtML

[R73] 分割大日志
来源：http://m.share.epnwcf.com/Article/details/gevlujedx.sHtML

split -l 1000 big.log part_
来源：http://mobile.tarul.cn/Article/details/gunioiadg.sHtML

[R74] 批量重命名
来源：http://www.blog.bbcook.cn/Article/details/gvtzigcem.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.blog.tarul.cn/Article/details/gcrnrikkz.sHtML

[R75] 导出环境变量
来源：http://mobile.yfazqb.com/Article/details/gxvpgqbrv.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://m.share.yfazqb.com/Article/details/gmrnlawnn.sHtML

[R76] 使用临时文件
来源：http://www.share.fktsv.cn/Article/details/gcfjzbryx.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://blog.bbcook.cn/Article/details/gmvrudjhe.sHtML

[R77] 读取用户输入
来源：http://read.share.fktsv.cn/Article/details/gqejupbkv.sHtML

read -rp "请输入: " ans
来源：http://www.share.vehdjk.com/Article/details/gcgfzihyw.sHtML

[R78] 交互式菜单
来源：http://www.m.share.fktsv.cn/Article/details/gpvpyexbl.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://wap.tarul.cn/Article/details/gkzyjvgzd.sHtML

[R79] 解析命令行选项
来源：http://baike.yfazqb.com/Article/details/gcpreeeim.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://3g.epnwcf.com/Article/details/gllnqnacm.sHtML

[R80] 查看脚本执行耗时
来源：http://baike.sjlbkw.cn/Article/details/grujocukt.sHtML

time ./run.sh
来源：http://m.share.bbcook.cn/Article/details/gllymqanu.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/giakqujvd.sHtML

S. C / C++ 专题
来源：http://3g.yfazqb.com/Article/details/gubaldpgo.sHtML

================================================================================
来源：http://mobile.vehdjk.com/Article/details/gaifvuflt.sHtML

[S01] C：Hello World
来源：http://www.blog.yfazqb.com/Article/details/grpfagwsm.sHtML

#include <stdio.h>
来源：http://www.m.share.vehdjk.com/Article/details/gdmjvdajp.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://read.share.tarul.cn/Article/details/govnocatu.sHtML

[S02] C：变量与格式化输出
来源：http://wap.yfazqb.com/Article/details/gxkvafqrh.sHtML

int a = 10; printf("%d\n", a);
来源：http://blog.vehdjk.com/Article/details/gfuknxtya.sHtML

[S03] C：读入整数
来源：http://mobile.vehdjk.com/Article/details/gkdddoriy.sHtML

int x; scanf("%d", &x);
来源：http://read.share.epnwcf.com/Article/details/gpzmdgvqy.sHtML

[S04] C：字符串复制
来源：http://mobile.vehdjk.com/Article/details/ggkrbuhfo.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://baike.tarul.cn/Article/details/gjdupkhwo.sHtML

[S05] C：字符串长度
来源：http://www.blog.bbcook.cn/Article/details/ghntmryrp.sHtML

strlen(s)
来源：http://blog.epnwcf.com/Article/details/gkhhzhfun.sHtML

[S06] C：字符串比较
来源：http://baike.epnwcf.com/Article/details/gdlwlrjzy.sHtML

strcmp(a, b) == 0
来源：http://www.m.share.tarul.cn/Article/details/gwehqwhyu.sHtML

[S07] C：数组遍历求和
来源：http://mobile.sjlbkw.cn/Article/details/gzwzraqmw.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://3g.vehdjk.com/Article/details/gqzpkuvvr.sHtML

[S08] C：动态内存分配与释放
来源：http://blog.sjlbkw.cn/Article/details/gnpdpzawl.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mobile.epnwcf.com/Article/details/gkzobzapf.sHtML

[S09] C：结构体定义与初始化
来源：http://3g.yfazqb.com/Article/details/ghfkfsoql.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.blog.yfazqb.com/Article/details/gusjnboxw.sHtML

[S10] C：指针与解引用
来源：http://baike.epnwcf.com/Article/details/giuqjedhb.sHtML

int *p = &a;  *p = 5;
来源：http://baike.epnwcf.com/Article/details/gdogcdqej.sHtML

[S11] C：逐行读文件
来源：http://baike.bbcook.cn/Article/details/gvassrgft.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.share.sjlbkw.cn/Article/details/godbmqrzo.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://baike.tarul.cn/Article/details/ggbvvbyyr.sHtML

fclose(f);
来源：http://wap.epnwcf.com/Article/details/gfbeewsrz.sHtML

[S12] C：写文件
来源：http://wap.epnwcf.com/Article/details/gxokyoluc.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.m.share.epnwcf.com/Article/details/gzvcsopmq.sHtML

[S13] C：宏定义
来源：http://m.share.tarul.cn/Article/details/gpmdysqgm.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://m.share.epnwcf.com/Article/details/gtuxkzefp.sHtML

[S14] C：枚举
来源：http://mobile.bbcook.cn/Article/details/gmmgfmsii.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://mobile.sjlbkw.cn/Article/details/gxpkdlplh.sHtML

[S15] C：类型转换
来源：http://wap.yfazqb.com/Article/details/gdyurycfg.sHtML

(double) a / b
来源：http://m.share.fktsv.cn/Article/details/geynrdopg.sHtML

[S16] C：位操作置位
来源：http://www.m.share.fktsv.cn/Article/details/gzabnfvyp.sHtML

x |= (1 << 3);
来源：http://wap.bbcook.cn/Article/details/grlxkfyeg.sHtML

[S17] C：安全拼接字符串
来源：http://www.share.epnwcf.com/Article/details/gnzrkebtf.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.blog.epnwcf.com/Article/details/genyshctu.sHtML

[S18] C：命令行参数
来源：http://3g.yfazqb.com/Article/details/gapdkkcrm.sHtML

int main(int argc, char **argv)
来源：http://3g.epnwcf.com/Article/details/gzslsjjzy.sHtML

[S19] C：快速排序
来源：http://m.share.yfazqb.com/Article/details/gejjruapt.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://read.share.vehdjk.com/Article/details/gzqbtgelu.sHtML

[S20] C：二分查找
来源：http://www.blog.vehdjk.com/Article/details/gpvnqrsix.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://mobile.epnwcf.com/Article/details/gtzlcufbs.sHtML

[S21] C：字符类别判断
来源：http://m.share.vehdjk.com/Article/details/gqotzkffw.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mobile.fktsv.cn/Article/details/gsnqmyzpx.sHtML

[S22] C：字符串转数字
来源：http://www.blog.epnwcf.com/Article/details/gabnvqdth.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://mobile.bbcook.cn/Article/details/geqqlajwf.sHtML

[S23] C：随机数
来源：http://3g.epnwcf.com/Article/details/gncgmwyjg.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://mobile.vehdjk.com/Article/details/gqaceqlpg.sHtML

[S24] C：获取本地时间
来源：http://3g.tarul.cn/Article/details/gwmbwhfhj.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.m.share.bbcook.cn/Article/details/ghboingyr.sHtML

[S25] C：内存拷贝
来源：http://www.share.epnwcf.com/Article/details/grixwbtvf.sHtML

memcpy(dst, src, n);
来源：http://baike.sjlbkw.cn/Article/details/gvaykzvkm.sHtML

[S26] C：内存清零
来源：http://www.blog.yfazqb.com/Article/details/gfusugixe.sHtML

memset(a, 0, sizeof a);
来源：http://read.share.fktsv.cn/Article/details/gildwvucf.sHtML

[S27] C：定义常量
来源：http://m.share.bbcook.cn/Article/details/gnmzsolte.sHtML

const double PI = 3.14159;
来源：http://mobile.yfazqb.com/Article/details/gehwuugxv.sHtML

[S28] C：静态变量
来源：http://read.share.bbcook.cn/Article/details/gzgafcmgh.sHtML

static int counter = 0;
来源：http://www.blog.bbcook.cn/Article/details/gznknxeiw.sHtML

[S29] C：变参函数
来源：http://m.share.bbcook.cn/Article/details/gywvgkmnv.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.share.epnwcf.com/Article/details/geqgiabwc.sHtML

[S30] C：头文件保护
来源：http://m.share.yfazqb.com/Article/details/gbiouhutn.sHtML

#ifndef X_H
来源：http://wap.fktsv.cn/Article/details/gxcxtdtfs.sHtML

#define X_H
来源：http://read.share.vehdjk.com/Article/details/gnaaizhvv.sHtML

#endif
来源：http://www.share.tarul.cn/Article/details/gutpvvwhg.sHtML

[S31] C++：Hello World
来源：http://www.share.vehdjk.com/Article/details/gkoxrdugf.sHtML

#include <iostream>
来源：http://baike.tarul.cn/Article/details/gbqzdptsk.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://wap.tarul.cn/Article/details/gnbapygpr.sHtML

[S32] C++：字符串
来源：http://blog.sjlbkw.cn/Article/details/gobdzjexn.sHtML

std::string s = "hi";  s += "!";
来源：http://blog.tarul.cn/Article/details/golupwhca.sHtML

[S33] C++：vector 增删
来源：http://www.m.share.bbcook.cn/Article/details/gchobgnyf.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://3g.yfazqb.com/Article/details/grsprtvqc.sHtML

[S34] C++：遍历 vector
来源：http://m.share.bbcook.cn/Article/details/gwrgwcvki.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://read.share.epnwcf.com/Article/details/gwhlumovz.sHtML

[S35] C++：map
来源：http://blog.bbcook.cn/Article/details/gpeexvbxf.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wap.vehdjk.com/Article/details/gsxtbuhim.sHtML

[S36] C++：unordered_map
来源：http://wap.vehdjk.com/Article/details/glaqnjqwb.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://baike.yfazqb.com/Article/details/gymtmvwmy.sHtML

[S37] C++：set
来源：http://3g.tarul.cn/Article/details/gkzgxraid.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://blog.fktsv.cn/Article/details/gqfynlajp.sHtML

[S38] C++：排序
来源：http://read.share.fktsv.cn/Article/details/gygwydhcr.sHtML

std::sort(v.begin(), v.end());
来源：http://www.m.share.epnwcf.com/Article/details/glxeiqrns.sHtML

[S39] C++：自定义比较器排序
来源：http://www.share.sjlbkw.cn/Article/details/gjefpafhj.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.m.share.sjlbkw.cn/Article/details/gaphljsfv.sHtML

[S40] C++：查找元素
来源：http://blog.yfazqb.com/Article/details/gykwuzgot.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://baike.vehdjk.com/Article/details/gfugghacu.sHtML

[S41] C++：类与构造函数
来源：http://m.share.bbcook.cn/Article/details/ggbogxlbx.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.share.vehdjk.com/Article/details/gopxacbys.sHtML

[S42] C++：继承与虚函数
来源：http://wap.vehdjk.com/Article/details/gnhsghtuc.sHtML

class B : public Base { public: void f() override {} };
来源：http://m.share.bbcook.cn/Article/details/gbrbruaty.sHtML

[S43] C++：智能指针
来源：http://m.share.tarul.cn/Article/details/gvshcyuqg.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.blog.fktsv.cn/Article/details/gcrgrlebd.sHtML

[S44] C++：引用传参
来源：http://3g.sjlbkw.cn/Article/details/gusitpeqh.sHtML

void inc(int &x) { ++x; }
来源：http://mobile.yfazqb.com/Article/details/grrfbximy.sHtML

[S45] C++：lambda
来源：http://blog.yfazqb.com/Article/details/gsktokgju.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.m.share.fktsv.cn/Article/details/gyraxmswq.sHtML

[S46] C++：函数模板
来源：http://3g.bbcook.cn/Article/details/gfvidguhe.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.m.share.yfazqb.com/Article/details/gsqzsfwpk.sHtML

[S47] C++：结构化绑定遍历
来源：http://m.share.tarul.cn/Article/details/gxrwiuhwv.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://read.share.sjlbkw.cn/Article/details/grgvxhuso.sHtML

[S48] C++：逐行读文件
来源：http://mobile.bbcook.cn/Article/details/gdxbinuwv.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.m.share.sjlbkw.cn/Article/details/gflzbepjh.sHtML

while (std::getline(in, line)) { }
来源：http://www.m.share.sjlbkw.cn/Article/details/guacnexgk.sHtML

[S49] C++：写文件
来源：http://baike.bbcook.cn/Article/details/gvlpyrjzg.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://read.share.tarul.cn/Article/details/gnipdbotf.sHtML

[S50] C++：格式化数字
来源：http://www.m.share.sjlbkw.cn/Article/details/gwkfytiyx.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.m.share.vehdjk.com/Article/details/gmmfdicxx.sHtML

[S51] C++：显式类型转换
来源：http://www.share.sjlbkw.cn/Article/details/gkejsceqd.sHtML

static_cast<double>(a) / b
来源：http://m.share.epnwcf.com/Article/details/galqxcsxh.sHtML

[S52] C++：const 与 noexcept
来源：http://mobile.epnwcf.com/Article/details/gutqnvamv.sHtML

int size() const noexcept { return n_; }
来源：http://blog.epnwcf.com/Article/details/gfckalxwu.sHtML

[S53] C++：移动语义
来源：http://baike.fktsv.cn/Article/details/gdgrkwsnw.sHtML

std::vector<int> w = std::move(v);
来源：http://wap.fktsv.cn/Article/details/gaohjfflq.sHtML

[S54] C++：异常处理
来源：http://baike.fktsv.cn/Article/details/gshweglyk.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://m.share.bbcook.cn/Article/details/gsdbpzzdj.sHtML

[S55] C++：结构化绑定
来源：http://www.share.tarul.cn/Article/details/gbcvxcvjg.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.m.share.epnwcf.com/Article/details/gfopfuavr.sHtML

[S56] C++：optional
来源：http://www.m.share.yfazqb.com/Article/details/glprlbqxl.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://3g.epnwcf.com/Article/details/gbbfbxoxw.sHtML

[S57] C++：编译期常量
来源：http://blog.yfazqb.com/Article/details/gdkujogqs.sHtML

constexpr int N = 10;
来源：http://www.blog.vehdjk.com/Article/details/gfpndtdfj.sHtML

[S58] C++：命名空间
来源：http://3g.epnwcf.com/Article/details/gmqtfezhb.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.m.share.yfazqb.com/Article/details/gzcuqfpym.sHtML

[S59] C++：静态断言
来源：http://baike.epnwcf.com/Article/details/gejqwxiqy.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://read.share.vehdjk.com/Article/details/gpfirnsvh.sHtML

[S60] C++：遍历并删除元素
来源：http://wap.epnwcf.com/Article/details/gmauimrbk.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://3g.sjlbkw.cn/Article/details/gvtrzdzrw.sHtML

================================================================================
来源：http://www.share.epnwcf.com/Article/details/ghzfrakba.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.sjlbkw.cn/Article/details/gcsnuunkb.sHtML

================================================================================
来源：http://www.m.share.tarul.cn/Article/details/gukhaddfr.sHtML

[T01] Kotlin：Hello World
来源：http://baike.sjlbkw.cn/Article/details/gfokigwfh.sHtML

println("Hello")
来源：http://baike.epnwcf.com/Article/details/gunlyizbt.sHtML

[T02] Kotlin：变量
来源：http://read.share.vehdjk.com/Article/details/gygfpontl.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://wap.bbcook.cn/Article/details/goolouonm.sHtML

[T03] Kotlin：字符串模板
来源：http://baike.yfazqb.com/Article/details/gwkhgdhll.sHtML

"值: $b"
来源：http://blog.yfazqb.com/Article/details/gydgpxdvs.sHtML

[T04] Kotlin：空安全
来源：http://m.share.fktsv.cn/Article/details/grwtvlxzu.sHtML

val n: String? = null;  n?.length
来源：http://m.share.bbcook.cn/Article/details/gbjhxrckw.sHtML

[T05] Kotlin：when 表达式
来源：http://m.share.vehdjk.com/Article/details/gkkitpgsw.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://blog.sjlbkw.cn/Article/details/gbizryxmg.sHtML

[T06] Kotlin：集合映射
来源：http://www.blog.sjlbkw.cn/Article/details/guhlimcfd.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://mobile.vehdjk.com/Article/details/gdoitbxnd.sHtML


<!-- 参考信息 -->