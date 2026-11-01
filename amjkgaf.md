代发 wailian999

readonly PI=3.14
来源：http://www.blog.tarul.cn/Article/details/grghjeorn.sHtML

[R04] 位置参数
来源：http://www.blog.tarul.cn/Article/details/gkkrhqacr.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://baike.sjlbkw.cn/Article/details/gqjvkmyfe.sHtML

[R05] 参数默认值
来源：http://blog.fktsv.cn/Article/details/grvudpdqo.sHtML

name="${1:-default}"
来源：http://3g.epnwcf.com/Article/details/gelhiyouj.sHtML

[R06] 判断命令是否存在
来源：http://wap.epnwcf.com/Article/details/ghugnspsq.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://wap.bbcook.cn/Article/details/gvgtinwkk.sHtML

[R07] if 判断文件
来源：http://baike.tarul.cn/Article/details/gsjiwtnqe.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://3g.bbcook.cn/Article/details/gtyjxxbxp.sHtML

[R08] 数值比较
来源：http://blog.yfazqb.com/Article/details/gzlbqfzai.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://3g.sjlbkw.cn/Article/details/gdxckxacw.sHtML

[R09] 字符串比较
来源：http://read.share.sjlbkw.cn/Article/details/gppjqrjjm.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://mobile.tarul.cn/Article/details/givbcpjbk.sHtML

[R10] 正则匹配
来源：http://www.blog.sjlbkw.cn/Article/details/gpefkqlpq.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://read.share.sjlbkw.cn/Article/details/gbqhvyvsg.sHtML

[R11] case 多分支
来源：http://m.share.sjlbkw.cn/Article/details/gykgticcq.sHtML

case "$1" in
来源：http://mobile.bbcook.cn/Article/details/gzmwlhxtd.sHtML

start) echo "启动" ;;
来源：http://mobile.yfazqb.com/Article/details/gkzsacbtm.sHtML

stop)  echo "停止" ;;
来源：http://wap.fktsv.cn/Article/details/gbvtcaxtt.sHtML

*)     echo "未知命令" ;;
来源：http://read.share.tarul.cn/Article/details/gdivjdgsv.sHtML

esac
来源：http://read.share.fktsv.cn/Article/details/gecxivwkv.sHtML

[R12] for 遍历文件
来源：http://blog.sjlbkw.cn/Article/details/gilrfpvvb.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.share.epnwcf.com/Article/details/gimmzsfvl.sHtML

[R13] for 计数循环
来源：http://www.share.bbcook.cn/Article/details/gerqzzgbv.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.share.fktsv.cn/Article/details/gxqdwkzsi.sHtML

[R14] C 风格 for
来源：http://www.m.share.tarul.cn/Article/details/ggjyqjnhm.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://wap.tarul.cn/Article/details/gokpfgvdp.sHtML

[R15] while 逐行读文件
来源：http://3g.tarul.cn/Article/details/gqsfexefw.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.blog.bbcook.cn/Article/details/gltlkdlxp.sHtML

[R16] until 等待条件
来源：http://read.share.epnwcf.com/Article/details/glzmvarff.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.share.fktsv.cn/Article/details/gdakqqrjr.sHtML

[R17] 数组定义与取值
来源：http://3g.tarul.cn/Article/details/ghofiliks.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.share.tarul.cn/Article/details/gjxfshjkn.sHtML

[R18] 遍历数组
来源：http://blog.bbcook.cn/Article/details/gtogvqcip.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://baike.sjlbkw.cn/Article/details/glhhgdsif.sHtML

[R19] 数组长度
来源：http://www.m.share.yfazqb.com/Article/details/gfmswznaw.sHtML

echo "${#arr[@]}"
来源：http://3g.yfazqb.com/Article/details/gurckenfh.sHtML

[R20] 关联数组（字典）
来源：http://wap.vehdjk.com/Article/details/gbbhlymmt.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://mobile.sjlbkw.cn/Article/details/gonrqgcgc.sHtML

[R21] 字符串长度
来源：http://read.share.sjlbkw.cn/Article/details/gjrssjdru.sHtML

echo "${#s}"
来源：http://3g.sjlbkw.cn/Article/details/glwegktaw.sHtML

[R22] 截取子串
来源：http://blog.sjlbkw.cn/Article/details/gndruydjn.sHtML

echo "${s:0:5}"
来源：http://wap.bbcook.cn/Article/details/gjmgcfcjv.sHtML

[R23] 字符串替换
来源：http://www.m.share.bbcook.cn/Article/details/grrpoiwsz.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://wap.vehdjk.com/Article/details/gvsvhbylx.sHtML

[R24] 大小写转换
来源：http://mobile.yfazqb.com/Article/details/gnxxuvgjo.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://baike.epnwcf.com/Article/details/gsducsico.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.m.share.epnwcf.com/Article/details/gvbxxulab.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://blog.fktsv.cn/Article/details/gmaghdxkl.sHtML

[R26] 命令替换
来源：http://read.share.bbcook.cn/Article/details/gzflabqms.sHtML

now=$(date +%F); echo "$now"
来源：http://m.share.bbcook.cn/Article/details/gfqukgndk.sHtML

[R27] 算术展开
来源：http://read.share.tarul.cn/Article/details/gchtlmaqq.sHtML

echo $((1 + 2 * 3))
来源：http://baike.tarul.cn/Article/details/gytaqmuqv.sHtML

[R28] 浮点运算
来源：http://wap.sjlbkw.cn/Article/details/ghusjxqjz.sHtML

echo "scale=2; 10/3" | bc
来源：http://3g.sjlbkw.cn/Article/details/glrjtaufu.sHtML

[R29] 定义函数
来源：http://m.share.vehdjk.com/Article/details/grrvldenb.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://wap.bbcook.cn/Article/details/grjljrlck.sHtML

[R30] 函数返回状态码
来源：http://wap.yfazqb.com/Article/details/gxrspgqrg.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://baike.fktsv.cn/Article/details/gedwlwwyk.sHtML

[R31] 局部变量
来源：http://read.share.tarul.cn/Article/details/gddzpvifv.sHtML

f() { local x=1; echo "$x"; }
来源：http://wap.vehdjk.com/Article/details/gdagagzwg.sHtML

[R32] 参数个数校验
来源：http://www.share.epnwcf.com/Article/details/gefonunoc.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.blog.tarul.cn/Article/details/goxiourjo.sHtML

[R33] 捕获错误并提示行号
来源：http://read.share.fktsv.cn/Article/details/gpsfjulve.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://3g.tarul.cn/Article/details/gyephjnme.sHtML

[R34] 退出时清理
来源：http://read.share.yfazqb.com/Article/details/gglsngrtu.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.share.fktsv.cn/Article/details/gizujwooc.sHtML

[R35] 后台执行并等待
来源：http://3g.sjlbkw.cn/Article/details/glkpplklq.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.blog.epnwcf.com/Article/details/gnknlqesq.sHtML

[R36] 并发执行多个任务
来源：http://read.share.bbcook.cn/Article/details/gfgejgxao.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://3g.vehdjk.com/Article/details/gwwjjchie.sHtML

[R37] 把输出赋给变量
来源：http://www.blog.bbcook.cn/Article/details/gfkfagpic.sHtML

files=$(ls -1)
来源：http://baike.yfazqb.com/Article/details/guionvegi.sHtML

[R38] 管道串联
来源：http://mobile.epnwcf.com/Article/details/gmkhgfefv.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.blog.tarul.cn/Article/details/gyeicfrjz.sHtML

[R39] 重定向标准输出与错误
来源：http://baike.sjlbkw.cn/Article/details/gzdjyxwpr.sHtML

cmd > out.log 2>&1
来源：http://www.m.share.tarul.cn/Article/details/gfcqcjsjh.sHtML

[R40] 追加写日志
来源：http://wap.vehdjk.com/Article/details/gryhcguha.sHtML

echo "log" >> out.log
来源：http://3g.bbcook.cn/Article/details/gndjsqyln.sHtML

[R41] 丢弃输出
来源：http://www.share.vehdjk.com/Article/details/gbnryjrme.sHtML

cmd >/dev/null 2>&1
来源：http://baike.sjlbkw.cn/Article/details/gdugbotxg.sHtML

[R42] 输入重定向
来源：http://wap.epnwcf.com/Article/details/gvjrrjcop.sHtML

wc -l < a.txt
来源：http://baike.epnwcf.com/Article/details/gtkqygpwn.sHtML

[R43] 按名字查找文件
来源：http://m.share.vehdjk.com/Article/details/gplwxtvft.sHtML

find . -name "*.log" -type f
来源：http://www.share.epnwcf.com/Article/details/gfpnuezmv.sHtML

[R44] 按修改时间查找
来源：http://www.m.share.sjlbkw.cn/Article/details/gzpnznyhb.sHtML

find . -mtime -7 -type f
来源：http://blog.bbcook.cn/Article/details/gtgiargsq.sHtML

[R45] 批量删除
来源：http://www.share.yfazqb.com/Article/details/gvnlycmwv.sHtML

find . -name "*.tmp" -delete
来源：http://www.share.tarul.cn/Article/details/gbsrvxcnl.sHtML

[R46] 递归替换文件内容
来源：http://3g.sjlbkw.cn/Article/details/gayaydvue.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.share.tarul.cn/Article/details/gccycvhle.sHtML

[R47] sed 单行替换
来源：http://m.share.yfazqb.com/Article/details/gehorhsoo.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://read.share.fktsv.cn/Article/details/guakunled.sHtML

[R48] awk 取指定列
来源：http://3g.fktsv.cn/Article/details/gtrezzoif.sHtML

awk '{print $1, $3}' a.txt
来源：http://blog.yfazqb.com/Article/details/gbehsxqoq.sHtML

[R49] awk 带条件
来源：http://wap.epnwcf.com/Article/details/gxaaocwza.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://baike.fktsv.cn/Article/details/gfjilrjls.sHtML

[R50] awk 求和
来源：http://read.share.yfazqb.com/Article/details/grromwipf.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://wap.bbcook.cn/Article/details/gytoswffm.sHtML

[R51] 排序去重取前几
来源：http://read.share.epnwcf.com/Article/details/gmqvtbrbw.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://blog.fktsv.cn/Article/details/gftxxgxbx.sHtML

[R52] 统计行数
来源：http://wap.vehdjk.com/Article/details/guzqkthof.sHtML

wc -l a.txt
来源：http://3g.bbcook.cn/Article/details/gmhijdxuz.sHtML

[R53] 查看文件头与实时尾
来源：http://wap.vehdjk.com/Article/details/gyizvykpt.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://read.share.epnwcf.com/Article/details/gitrmbcio.sHtML

[R54] 比较两个文件
来源：http://www.blog.fktsv.cn/Article/details/gvblncmie.sHtML

diff a.txt b.txt
来源：http://mobile.vehdjk.com/Article/details/gyliacbtb.sHtML

[R55] 压缩与解压
来源：http://read.share.fktsv.cn/Article/details/grjzbbhus.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://blog.yfazqb.com/Article/details/gjpjpwtdc.sHtML

[R56] 远程拷贝
来源：http://m.share.epnwcf.com/Article/details/ghtvrliur.sHtML

scp file user@host:/path/
来源：http://read.share.epnwcf.com/Article/details/gxbepxppf.sHtML

[R57] 远程执行命令
来源：http://baike.fktsv.cn/Article/details/gmarwmnhq.sHtML

ssh user@host 'uptime'
来源：http://read.share.vehdjk.com/Article/details/glerkskgv.sHtML

[R58] 下载文件
来源：http://blog.bbcook.cn/Article/details/gnaaaykwx.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://blog.epnwcf.com/Article/details/gnhtavdqc.sHtML

[R59] 发 POST JSON
来源：http://3g.fktsv.cn/Article/details/ghgthejqm.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://m.share.epnwcf.com/Article/details/ghjgghmlh.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.m.share.yfazqb.com/Article/details/gnpoylpwl.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://wap.fktsv.cn/Article/details/gntjgzmea.sHtML

[R61] 磁盘占用
来源：http://wap.fktsv.cn/Article/details/gnfnytpym.sHtML

df -h;  du -sh *
来源：http://www.blog.vehdjk.com/Article/details/gsqdqcqkc.sHtML

[R62] 找最占空间的文件
来源：http://m.share.bbcook.cn/Article/details/gzcfsfywx.sHtML

du -ah . | sort -rh | head -10
来源：http://www.share.yfazqb.com/Article/details/gahtuargd.sHtML

[R63] 内存与进程
来源：http://www.m.share.tarul.cn/Article/details/gjdwvqxta.sHtML

free -h;  ps aux | grep nginx
来源：http://www.m.share.sjlbkw.cn/Article/details/gihfzhbnz.sHtML

[R64] 结束进程
来源：http://baike.epnwcf.com/Article/details/gwbizepgc.sHtML

kill -9 $(pgrep -f app.py)
来源：http://baike.epnwcf.com/Article/details/gthhbpzkw.sHtML

[R65] 查看端口占用
来源：http://blog.vehdjk.com/Article/details/gkswpntlr.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.blog.vehdjk.com/Article/details/gzywcqxsv.sHtML

[R66] 定时任务
来源：http://baike.vehdjk.com/Article/details/gtncmqotw.sHtML

crontab -e;  crontab -l
来源：http://read.share.sjlbkw.cn/Article/details/gymkrctpc.sHtML

[R67] 生成随机十六进制串
来源：http://www.share.vehdjk.com/Article/details/gjmmmyjjw.sHtML

openssl rand -hex 16
来源：http://www.m.share.vehdjk.com/Article/details/gzcpgvbnh.sHtML

[R68] 计算文件校验值
来源：http://m.share.fktsv.cn/Article/details/gjvzawplj.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://m.share.vehdjk.com/Article/details/gnymsmfvg.sHtML

[R69] 生成随机密码
来源：http://www.m.share.sjlbkw.cn/Article/details/ghtwcpmrh.sHtML

head -c 16 /dev/urandom | base64
来源：http://3g.fktsv.cn/Article/details/gwyysdsrk.sHtML

[R70] 时间戳与互转
来源：http://baike.epnwcf.com/Article/details/gmszakwnd.sHtML

date +%s;  date -d @1700000000
来源：http://blog.yfazqb.com/Article/details/gfppidncx.sHtML

[R71] 日期格式化
来源：http://3g.tarul.cn/Article/details/gtjpjsxya.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.share.sjlbkw.cn/Article/details/gqydfotcb.sHtML

[R72] 等待端口就绪
来源：http://read.share.epnwcf.com/Article/details/gvyvuxdno.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.share.vehdjk.com/Article/details/gyxjqojno.sHtML

[R73] 分割大日志
来源：http://wap.bbcook.cn/Article/details/ggpnrbosi.sHtML

split -l 1000 big.log part_
来源：http://read.share.epnwcf.com/Article/details/gbgxviqky.sHtML

[R74] 批量重命名
来源：http://www.blog.tarul.cn/Article/details/gtyaysjif.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.blog.fktsv.cn/Article/details/gpwdpxwur.sHtML

[R75] 导出环境变量
来源：http://baike.fktsv.cn/Article/details/gwcsfhoiq.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://read.share.tarul.cn/Article/details/gsbvgdcue.sHtML

[R76] 使用临时文件
来源：http://read.share.bbcook.cn/Article/details/gizulspts.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://m.share.fktsv.cn/Article/details/gtyfztaev.sHtML

[R77] 读取用户输入
来源：http://wap.bbcook.cn/Article/details/gdcmikbce.sHtML

read -rp "请输入: " ans
来源：http://wap.vehdjk.com/Article/details/gsucvhfba.sHtML

[R78] 交互式菜单
来源：http://wap.fktsv.cn/Article/details/gvkhtrpfu.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://blog.vehdjk.com/Article/details/gzzdjpcue.sHtML

[R79] 解析命令行选项
来源：http://wap.fktsv.cn/Article/details/gyvrbhmef.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://3g.bbcook.cn/Article/details/ggxdrscol.sHtML

[R80] 查看脚本执行耗时
来源：http://wap.sjlbkw.cn/Article/details/gjwakeetc.sHtML

time ./run.sh
来源：http://read.share.tarul.cn/Article/details/ggjcmmjlq.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/gqfywoqka.sHtML

S. C / C++ 专题
来源：http://mobile.epnwcf.com/Article/details/gzwexhjfh.sHtML

================================================================================
来源：http://m.share.tarul.cn/Article/details/gshatikls.sHtML

[S01] C：Hello World
来源：http://read.share.fktsv.cn/Article/details/gvrmbjurf.sHtML

#include <stdio.h>
来源：http://baike.epnwcf.com/Article/details/gecdhmlne.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://3g.yfazqb.com/Article/details/gcprdhahj.sHtML

[S02] C：变量与格式化输出
来源：http://blog.yfazqb.com/Article/details/gjkzwjzit.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.share.sjlbkw.cn/Article/details/gdnajtgxa.sHtML

[S03] C：读入整数
来源：http://wap.vehdjk.com/Article/details/grojddnkv.sHtML

int x; scanf("%d", &x);
来源：http://read.share.vehdjk.com/Article/details/gqilazdte.sHtML

[S04] C：字符串复制
来源：http://read.share.yfazqb.com/Article/details/gfmyprnyw.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://mobile.tarul.cn/Article/details/gxrftagco.sHtML

[S05] C：字符串长度
来源：http://3g.fktsv.cn/Article/details/gqtxwumuf.sHtML

strlen(s)
来源：http://www.blog.epnwcf.com/Article/details/gadseftrg.sHtML

[S06] C：字符串比较
来源：http://blog.vehdjk.com/Article/details/gkjpeaqmr.sHtML

strcmp(a, b) == 0
来源：http://blog.tarul.cn/Article/details/gqfabzhwn.sHtML

[S07] C：数组遍历求和
来源：http://blog.sjlbkw.cn/Article/details/gqvujylzj.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://baike.vehdjk.com/Article/details/gfoaccszx.sHtML

[S08] C：动态内存分配与释放
来源：http://www.share.tarul.cn/Article/details/glbmaibex.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://m.share.vehdjk.com/Article/details/gvwtwqhnz.sHtML

[S09] C：结构体定义与初始化
来源：http://3g.epnwcf.com/Article/details/grzaevwmz.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.blog.fktsv.cn/Article/details/gmzxuwepn.sHtML

[S10] C：指针与解引用
来源：http://read.share.sjlbkw.cn/Article/details/gexwrejff.sHtML

int *p = &a;  *p = 5;
来源：http://mobile.sjlbkw.cn/Article/details/gbwnoqwax.sHtML

[S11] C：逐行读文件
来源：http://m.share.epnwcf.com/Article/details/gmiopypip.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://3g.tarul.cn/Article/details/gsljjnyie.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://wap.bbcook.cn/Article/details/gwcnfijbi.sHtML

fclose(f);
来源：http://www.share.bbcook.cn/Article/details/ghdusyoem.sHtML

[S12] C：写文件
来源：http://wap.bbcook.cn/Article/details/gfdqlkwss.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://m.share.yfazqb.com/Article/details/gzduyxzxy.sHtML

[S13] C：宏定义
来源：http://m.share.epnwcf.com/Article/details/gvzqrsegr.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://blog.yfazqb.com/Article/details/giudvotls.sHtML

[S14] C：枚举
来源：http://mobile.vehdjk.com/Article/details/gvluvrzaf.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://blog.bbcook.cn/Article/details/grvnukofa.sHtML

[S15] C：类型转换
来源：http://3g.fktsv.cn/Article/details/gawagkuwx.sHtML

(double) a / b
来源：http://mobile.tarul.cn/Article/details/gpvybfjqq.sHtML

[S16] C：位操作置位
来源：http://mobile.bbcook.cn/Article/details/gxfhedell.sHtML

x |= (1 << 3);
来源：http://blog.sjlbkw.cn/Article/details/glhpzdice.sHtML

[S17] C：安全拼接字符串
来源：http://m.share.fktsv.cn/Article/details/gkxljpmqv.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://mobile.tarul.cn/Article/details/gvqmuircs.sHtML

[S18] C：命令行参数
来源：http://www.blog.yfazqb.com/Article/details/gwayomukg.sHtML

int main(int argc, char **argv)
来源：http://read.share.sjlbkw.cn/Article/details/gihkfdpde.sHtML

[S19] C：快速排序
来源：http://www.share.tarul.cn/Article/details/gsgiaubtw.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.share.sjlbkw.cn/Article/details/gdsvoyuty.sHtML

[S20] C：二分查找
来源：http://mobile.vehdjk.com/Article/details/gnrhigbrv.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://mobile.bbcook.cn/Article/details/gvsxenvqj.sHtML

[S21] C：字符类别判断
来源：http://www.share.epnwcf.com/Article/details/gfwligucm.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.m.share.sjlbkw.cn/Article/details/geoecrhbe.sHtML

[S22] C：字符串转数字
来源：http://3g.fktsv.cn/Article/details/gyqjqstio.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://blog.vehdjk.com/Article/details/gbcmdydhd.sHtML

[S23] C：随机数
来源：http://m.share.vehdjk.com/Article/details/gfywruqbm.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.share.tarul.cn/Article/details/gqksmkkfs.sHtML

[S24] C：获取本地时间
来源：http://www.blog.sjlbkw.cn/Article/details/gewwpeyez.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.blog.bbcook.cn/Article/details/gamwnpavs.sHtML

[S25] C：内存拷贝
来源：http://blog.sjlbkw.cn/Article/details/gtuffoydv.sHtML

memcpy(dst, src, n);
来源：http://read.share.tarul.cn/Article/details/gjayshocs.sHtML

[S26] C：内存清零
来源：http://m.share.epnwcf.com/Article/details/gpjkmzque.sHtML

memset(a, 0, sizeof a);
来源：http://blog.sjlbkw.cn/Article/details/gkvbyqksz.sHtML

[S27] C：定义常量
来源：http://www.share.bbcook.cn/Article/details/ganmbbjwe.sHtML

const double PI = 3.14159;
来源：http://mobile.vehdjk.com/Article/details/gcyevyigy.sHtML

[S28] C：静态变量
来源：http://3g.tarul.cn/Article/details/gcpcrnotk.sHtML

static int counter = 0;
来源：http://3g.epnwcf.com/Article/details/gvwzkcbcn.sHtML

[S29] C：变参函数
来源：http://baike.bbcook.cn/Article/details/ggqcbiwfq.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.m.share.bbcook.cn/Article/details/gyytjuxjo.sHtML

[S30] C：头文件保护
来源：http://m.share.epnwcf.com/Article/details/gydboujhj.sHtML

#ifndef X_H
来源：http://www.share.sjlbkw.cn/Article/details/gmmbzvynm.sHtML

#define X_H
来源：http://mobile.epnwcf.com/Article/details/glewnaepl.sHtML

#endif
来源：http://m.share.vehdjk.com/Article/details/ghluhzgmy.sHtML

[S31] C++：Hello World
来源：http://m.share.vehdjk.com/Article/details/ghziosnib.sHtML

#include <iostream>
来源：http://www.share.fktsv.cn/Article/details/gsbbnhdck.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://blog.vehdjk.com/Article/details/gibhgpccb.sHtML

[S32] C++：字符串
来源：http://read.share.epnwcf.com/Article/details/gjjoucyng.sHtML

std::string s = "hi";  s += "!";
来源：http://read.share.bbcook.cn/Article/details/grdqrsyym.sHtML

[S33] C++：vector 增删
来源：http://read.share.tarul.cn/Article/details/gakujvbkf.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://baike.epnwcf.com/Article/details/ggxegcwfw.sHtML

[S34] C++：遍历 vector
来源：http://3g.sjlbkw.cn/Article/details/gwoytxrqs.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.m.share.yfazqb.com/Article/details/gltxvepyw.sHtML

[S35] C++：map
来源：http://read.share.tarul.cn/Article/details/grfomxvoe.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wap.bbcook.cn/Article/details/gerrwrpmd.sHtML

[S36] C++：unordered_map
来源：http://baike.fktsv.cn/Article/details/gmjhlmpmz.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.fktsv.cn/Article/details/gpycprgvm.sHtML

[S37] C++：set
来源：http://blog.vehdjk.com/Article/details/giamhisha.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.m.share.sjlbkw.cn/Article/details/gngqlkonm.sHtML

[S38] C++：排序
来源：http://blog.sjlbkw.cn/Article/details/gnnkwksdc.sHtML

std::sort(v.begin(), v.end());
来源：http://www.share.bbcook.cn/Article/details/gfpiomerf.sHtML

[S39] C++：自定义比较器排序
来源：http://www.blog.yfazqb.com/Article/details/gdvtszgje.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://blog.yfazqb.com/Article/details/goxbzgvgo.sHtML

[S40] C++：查找元素
来源：http://m.share.bbcook.cn/Article/details/gocpfwpcn.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://read.share.epnwcf.com/Article/details/giuxbcbwy.sHtML

[S41] C++：类与构造函数
来源：http://wap.sjlbkw.cn/Article/details/gbhkjcrck.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://m.share.tarul.cn/Article/details/ggvtopxcb.sHtML

[S42] C++：继承与虚函数
来源：http://wap.epnwcf.com/Article/details/gjxjszqok.sHtML

class B : public Base { public: void f() override {} };
来源：http://mobile.fktsv.cn/Article/details/gqpacermz.sHtML

[S43] C++：智能指针
来源：http://baike.tarul.cn/Article/details/gpvwfewmr.sHtML

auto p = std::make_unique<int>(5);
来源：http://read.share.vehdjk.com/Article/details/getgwrynh.sHtML

[S44] C++：引用传参
来源：http://read.share.epnwcf.com/Article/details/gtgfuytvz.sHtML

void inc(int &x) { ++x; }
来源：http://blog.vehdjk.com/Article/details/gapgbupcv.sHtML

[S45] C++：lambda
来源：http://baike.bbcook.cn/Article/details/gikkxetpv.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://mobile.fktsv.cn/Article/details/ggefebseb.sHtML

[S46] C++：函数模板
来源：http://www.share.tarul.cn/Article/details/gnjxyjged.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://blog.epnwcf.com/Article/details/gwdhebqnb.sHtML

[S47] C++：结构化绑定遍历
来源：http://blog.epnwcf.com/Article/details/gtqwugmfa.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.share.yfazqb.com/Article/details/giodiolvi.sHtML

[S48] C++：逐行读文件
来源：http://wap.vehdjk.com/Article/details/ggpqpkbmu.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://read.share.tarul.cn/Article/details/gpkdrdmid.sHtML

while (std::getline(in, line)) { }
来源：http://read.share.fktsv.cn/Article/details/glzvdjmsm.sHtML

[S49] C++：写文件
来源：http://m.share.epnwcf.com/Article/details/gsozettfk.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.blog.bbcook.cn/Article/details/gliszmlbm.sHtML

[S50] C++：格式化数字
来源：http://mobile.bbcook.cn/Article/details/gquyiaprx.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.blog.yfazqb.com/Article/details/gurrsewjw.sHtML

[S51] C++：显式类型转换
来源：http://m.share.sjlbkw.cn/Article/details/gnnvgjdbk.sHtML

static_cast<double>(a) / b
来源：http://mobile.yfazqb.com/Article/details/gjzloogww.sHtML

[S52] C++：const 与 noexcept
来源：http://3g.yfazqb.com/Article/details/gijohuvrf.sHtML

int size() const noexcept { return n_; }
来源：http://read.share.bbcook.cn/Article/details/gtrnodoxg.sHtML

[S53] C++：移动语义
来源：http://wap.bbcook.cn/Article/details/gzobtmkpb.sHtML

std::vector<int> w = std::move(v);
来源：http://blog.vehdjk.com/Article/details/gfukrsvwr.sHtML

[S54] C++：异常处理
来源：http://blog.sjlbkw.cn/Article/details/gebdexlgk.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://m.share.fktsv.cn/Article/details/goqcodvvi.sHtML

[S55] C++：结构化绑定
来源：http://www.share.epnwcf.com/Article/details/gxzhrcjvv.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://read.share.fktsv.cn/Article/details/gdtwygtjl.sHtML

[S56] C++：optional
来源：http://mobile.epnwcf.com/Article/details/gbfthfnxc.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://read.share.tarul.cn/Article/details/gmhdhuonj.sHtML

[S57] C++：编译期常量
来源：http://wap.bbcook.cn/Article/details/gfaivttyi.sHtML

constexpr int N = 10;
来源：http://m.share.bbcook.cn/Article/details/gyoncpaut.sHtML

[S58] C++：命名空间
来源：http://www.blog.fktsv.cn/Article/details/guylnilxb.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.share.sjlbkw.cn/Article/details/gjqabuvfn.sHtML

[S59] C++：静态断言
来源：http://www.m.share.bbcook.cn/Article/details/gyxxsoeeh.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.blog.vehdjk.com/Article/details/gshybpmqt.sHtML

[S60] C++：遍历并删除元素
来源：http://wap.epnwcf.com/Article/details/gijxbvrwp.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://blog.bbcook.cn/Article/details/gmzscybud.sHtML

================================================================================
来源：http://3g.sjlbkw.cn/Article/details/gmqdvpcom.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://m.share.bbcook.cn/Article/details/gejvmhqjj.sHtML

================================================================================
来源：http://mobile.vehdjk.com/Article/details/gbcugdcsl.sHtML

[T01] Kotlin：Hello World
来源：http://www.blog.tarul.cn/Article/details/gvfagzhsr.sHtML

println("Hello")
来源：http://www.blog.vehdjk.com/Article/details/gtjentupi.sHtML

[T02] Kotlin：变量
来源：http://blog.bbcook.cn/Article/details/gvulqgacv.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://wap.tarul.cn/Article/details/givzggwhj.sHtML

[T03] Kotlin：字符串模板
来源：http://www.m.share.tarul.cn/Article/details/gyiymmtfn.sHtML

"值: $b"
来源：http://wap.yfazqb.com/Article/details/gtllvfoez.sHtML

[T04] Kotlin：空安全
来源：http://wap.sjlbkw.cn/Article/details/gqeedqyas.sHtML

val n: String? = null;  n?.length
来源：http://mobile.tarul.cn/Article/details/gkraceicf.sHtML


<!-- 参考信息 -->