代发 wailian999

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://m.share.tarul.cn/Article/details/gxhwdlhuh.sHtML

[R08] 数值比较
来源：http://read.share.bbcook.cn/Article/details/gglsztvqg.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://wap.fktsv.cn/Article/details/ghymvtgzz.sHtML

[R09] 字符串比较
来源：http://mobile.bbcook.cn/Article/details/gsrxyoriu.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://blog.vehdjk.com/Article/details/gwxdhfgnt.sHtML

[R10] 正则匹配
来源：http://m.share.yfazqb.com/Article/details/gnhemidsm.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://blog.fktsv.cn/Article/details/gsjtvriqq.sHtML

[R11] case 多分支
来源：http://read.share.sjlbkw.cn/Article/details/glnmngxho.sHtML

case "$1" in
来源：http://www.blog.vehdjk.com/Article/details/getctffar.sHtML

start) echo "启动" ;;
来源：http://read.share.epnwcf.com/Article/details/gyudzvbdz.sHtML

stop)  echo "停止" ;;
来源：http://www.blog.fktsv.cn/Article/details/ghzetxgoa.sHtML

*)     echo "未知命令" ;;
来源：http://3g.sjlbkw.cn/Article/details/gvnuwicju.sHtML

esac
来源：http://blog.yfazqb.com/Article/details/gvucpfyti.sHtML

[R12] for 遍历文件
来源：http://blog.epnwcf.com/Article/details/gugxrzsfx.sHtML

for f in *.txt; do echo "$f"; done
来源：http://m.share.yfazqb.com/Article/details/gsxuxnkwa.sHtML

[R13] for 计数循环
来源：http://www.blog.bbcook.cn/Article/details/gaevxsadr.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://3g.epnwcf.com/Article/details/gjanuwfqo.sHtML

[R14] C 风格 for
来源：http://3g.tarul.cn/Article/details/gmhbvynwf.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://mobile.bbcook.cn/Article/details/gmrftkvuu.sHtML

[R15] while 逐行读文件
来源：http://3g.epnwcf.com/Article/details/gvkeynesf.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://baike.bbcook.cn/Article/details/ggfpxntas.sHtML

[R16] until 等待条件
来源：http://3g.fktsv.cn/Article/details/gkrhadulk.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://3g.epnwcf.com/Article/details/gvnnbyyej.sHtML

[R17] 数组定义与取值
来源：http://www.m.share.vehdjk.com/Article/details/geplppfbr.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://read.share.fktsv.cn/Article/details/gnhclrtnr.sHtML

[R18] 遍历数组
来源：http://baike.sjlbkw.cn/Article/details/gavssctjj.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.share.epnwcf.com/Article/details/gtyfzfudp.sHtML

[R19] 数组长度
来源：http://m.share.epnwcf.com/Article/details/gtqcdpple.sHtML

echo "${#arr[@]}"
来源：http://3g.fktsv.cn/Article/details/gzlgidnhp.sHtML

[R20] 关联数组（字典）
来源：http://baike.sjlbkw.cn/Article/details/ggbwukwts.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.share.fktsv.cn/Article/details/gfulnyfvc.sHtML

[R21] 字符串长度
来源：http://baike.yfazqb.com/Article/details/gdjenxvpf.sHtML

echo "${#s}"
来源：http://m.share.fktsv.cn/Article/details/gzwcizeui.sHtML

[R22] 截取子串
来源：http://blog.vehdjk.com/Article/details/gnbjbfmbj.sHtML

echo "${s:0:5}"
来源：http://www.share.vehdjk.com/Article/details/gogdrsyfm.sHtML

[R23] 字符串替换
来源：http://www.blog.bbcook.cn/Article/details/gbavfcjqv.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://blog.sjlbkw.cn/Article/details/givsmwaar.sHtML

[R24] 大小写转换
来源：http://www.blog.vehdjk.com/Article/details/gdwepftmv.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.blog.fktsv.cn/Article/details/gboujohbh.sHtML

[R25] 去后缀 / 去前缀
来源：http://m.share.yfazqb.com/Article/details/gqaixjpcq.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.m.share.epnwcf.com/Article/details/gdafdsrjl.sHtML

[R26] 命令替换
来源：http://read.share.epnwcf.com/Article/details/gskkhxcrx.sHtML

now=$(date +%F); echo "$now"
来源：http://www.m.share.yfazqb.com/Article/details/gozfqlpge.sHtML

[R27] 算术展开
来源：http://read.share.fktsv.cn/Article/details/gqiylfwwe.sHtML

echo $((1 + 2 * 3))
来源：http://www.m.share.yfazqb.com/Article/details/gkzimvtvm.sHtML

[R28] 浮点运算
来源：http://read.share.sjlbkw.cn/Article/details/gozueovdh.sHtML

echo "scale=2; 10/3" | bc
来源：http://blog.epnwcf.com/Article/details/gsfqrhcvl.sHtML

[R29] 定义函数
来源：http://read.share.bbcook.cn/Article/details/gtnysyuee.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://m.share.sjlbkw.cn/Article/details/gxbqnuhtl.sHtML

[R30] 函数返回状态码
来源：http://mobile.vehdjk.com/Article/details/gayrlpimp.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://baike.yfazqb.com/Article/details/gnyrkcvuu.sHtML

[R31] 局部变量
来源：http://3g.tarul.cn/Article/details/gzcitasis.sHtML

f() { local x=1; echo "$x"; }
来源：http://wap.tarul.cn/Article/details/ghegniyqa.sHtML

[R32] 参数个数校验
来源：http://blog.vehdjk.com/Article/details/gwspgjrmd.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://read.share.epnwcf.com/Article/details/gmcocqjoz.sHtML

[R33] 捕获错误并提示行号
来源：http://3g.epnwcf.com/Article/details/gydtkrxqe.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://3g.bbcook.cn/Article/details/gwoigjrgj.sHtML

[R34] 退出时清理
来源：http://baike.fktsv.cn/Article/details/gsnuzjlos.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.sjlbkw.cn/Article/details/ganmkwvgx.sHtML

[R35] 后台执行并等待
来源：http://www.blog.bbcook.cn/Article/details/gfbedqjvg.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://baike.yfazqb.com/Article/details/gadmfecla.sHtML

[R36] 并发执行多个任务
来源：http://www.blog.fktsv.cn/Article/details/gewxtahbe.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://wap.fktsv.cn/Article/details/gvbtwnveq.sHtML

[R37] 把输出赋给变量
来源：http://read.share.yfazqb.com/Article/details/gjexjfone.sHtML

files=$(ls -1)
来源：http://www.m.share.sjlbkw.cn/Article/details/gshvejdxj.sHtML

[R38] 管道串联
来源：http://3g.yfazqb.com/Article/details/ggxrkwzko.sHtML

cat a.txt | grep -i error | wc -l
来源：http://blog.epnwcf.com/Article/details/gfmdvvrkj.sHtML

[R39] 重定向标准输出与错误
来源：http://www.share.bbcook.cn/Article/details/gqpjdcjqe.sHtML

cmd > out.log 2>&1
来源：http://www.share.epnwcf.com/Article/details/gfxvolmad.sHtML

[R40] 追加写日志
来源：http://www.blog.epnwcf.com/Article/details/gxnavtvfw.sHtML

echo "log" >> out.log
来源：http://mobile.bbcook.cn/Article/details/gsjkllvpm.sHtML

[R41] 丢弃输出
来源：http://m.share.sjlbkw.cn/Article/details/gmjjlrjtj.sHtML

cmd >/dev/null 2>&1
来源：http://www.m.share.epnwcf.com/Article/details/gpaxiqegs.sHtML

[R42] 输入重定向
来源：http://www.blog.epnwcf.com/Article/details/geblqaznu.sHtML

wc -l < a.txt
来源：http://blog.yfazqb.com/Article/details/gblfoxtlg.sHtML

[R43] 按名字查找文件
来源：http://baike.fktsv.cn/Article/details/gnkzazqdg.sHtML

find . -name "*.log" -type f
来源：http://read.share.epnwcf.com/Article/details/gbxdubjxd.sHtML

[R44] 按修改时间查找
来源：http://blog.fktsv.cn/Article/details/guiogfogv.sHtML

find . -mtime -7 -type f
来源：http://mobile.fktsv.cn/Article/details/gcvnzkyty.sHtML

[R45] 批量删除
来源：http://baike.bbcook.cn/Article/details/gpspctqcg.sHtML

find . -name "*.tmp" -delete
来源：http://baike.yfazqb.com/Article/details/gasthsxbf.sHtML

[R46] 递归替换文件内容
来源：http://www.m.share.vehdjk.com/Article/details/gjztqrmyd.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.share.vehdjk.com/Article/details/gggyufakr.sHtML

[R47] sed 单行替换
来源：http://www.share.yfazqb.com/Article/details/gliqajibq.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://wap.bbcook.cn/Article/details/gjtegmenl.sHtML

[R48] awk 取指定列
来源：http://m.share.epnwcf.com/Article/details/gieaykuhx.sHtML

awk '{print $1, $3}' a.txt
来源：http://baike.bbcook.cn/Article/details/grhjinapm.sHtML

[R49] awk 带条件
来源：http://www.m.share.bbcook.cn/Article/details/gcauakzwc.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.blog.sjlbkw.cn/Article/details/gxorflquf.sHtML

[R50] awk 求和
来源：http://read.share.sjlbkw.cn/Article/details/gxgtfnjxh.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://mobile.epnwcf.com/Article/details/gggthueog.sHtML

[R51] 排序去重取前几
来源：http://3g.tarul.cn/Article/details/gpxomkpos.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.blog.fktsv.cn/Article/details/ggapszwmf.sHtML

[R52] 统计行数
来源：http://m.share.bbcook.cn/Article/details/gfxdgxcoj.sHtML

wc -l a.txt
来源：http://blog.fktsv.cn/Article/details/gqlhntfqp.sHtML

[R53] 查看文件头与实时尾
来源：http://www.blog.bbcook.cn/Article/details/gndhywlql.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://baike.epnwcf.com/Article/details/glapcgtjg.sHtML

[R54] 比较两个文件
来源：http://wap.fktsv.cn/Article/details/gszumqtye.sHtML

diff a.txt b.txt
来源：http://www.blog.tarul.cn/Article/details/gkevjvdji.sHtML

[R55] 压缩与解压
来源：http://www.share.yfazqb.com/Article/details/ggdaljudx.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://wap.vehdjk.com/Article/details/ggjmhdwep.sHtML

[R56] 远程拷贝
来源：http://www.m.share.sjlbkw.cn/Article/details/gjipbrupc.sHtML

scp file user@host:/path/
来源：http://mobile.bbcook.cn/Article/details/gosyqqyxu.sHtML

[R57] 远程执行命令
来源：http://www.blog.fktsv.cn/Article/details/gegsnqjkc.sHtML

ssh user@host 'uptime'
来源：http://blog.fktsv.cn/Article/details/gfmbrekrb.sHtML

[R58] 下载文件
来源：http://www.share.yfazqb.com/Article/details/guktszjvy.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.m.share.epnwcf.com/Article/details/gurmvkuun.sHtML

[R59] 发 POST JSON
来源：http://mobile.epnwcf.com/Article/details/gyssljhii.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://baike.yfazqb.com/Article/details/gtohzmzij.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.m.share.epnwcf.com/Article/details/gdkrydofd.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mobile.yfazqb.com/Article/details/gbkqzfmtt.sHtML

[R61] 磁盘占用
来源：http://mobile.vehdjk.com/Article/details/gaaaikxrn.sHtML

df -h;  du -sh *
来源：http://baike.bbcook.cn/Article/details/gsjvuookz.sHtML

[R62] 找最占空间的文件
来源：http://wap.epnwcf.com/Article/details/gdkyhpsfj.sHtML

du -ah . | sort -rh | head -10
来源：http://blog.bbcook.cn/Article/details/gytmifioa.sHtML

[R63] 内存与进程
来源：http://read.share.sjlbkw.cn/Article/details/geieebbvs.sHtML

free -h;  ps aux | grep nginx
来源：http://www.share.epnwcf.com/Article/details/gdgxqknpa.sHtML

[R64] 结束进程
来源：http://www.blog.vehdjk.com/Article/details/gjjwsqngy.sHtML

kill -9 $(pgrep -f app.py)
来源：http://wap.yfazqb.com/Article/details/grqcrsupi.sHtML

[R65] 查看端口占用
来源：http://wap.vehdjk.com/Article/details/gavduotqj.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://read.share.vehdjk.com/Article/details/gqezgquop.sHtML

[R66] 定时任务
来源：http://baike.sjlbkw.cn/Article/details/gyjaysycv.sHtML

crontab -e;  crontab -l
来源：http://wap.sjlbkw.cn/Article/details/gzctdzzyj.sHtML

[R67] 生成随机十六进制串
来源：http://read.share.yfazqb.com/Article/details/gvhylaiwz.sHtML

openssl rand -hex 16
来源：http://www.blog.vehdjk.com/Article/details/glpywcnir.sHtML

[R68] 计算文件校验值
来源：http://mobile.bbcook.cn/Article/details/glorgwqgc.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://3g.epnwcf.com/Article/details/gwrlzobmr.sHtML

[R69] 生成随机密码
来源：http://blog.tarul.cn/Article/details/gxummsami.sHtML

head -c 16 /dev/urandom | base64
来源：http://m.share.bbcook.cn/Article/details/gkpyooevd.sHtML

[R70] 时间戳与互转
来源：http://www.m.share.yfazqb.com/Article/details/gqvelfdry.sHtML

date +%s;  date -d @1700000000
来源：http://m.share.yfazqb.com/Article/details/gziejgmai.sHtML

[R71] 日期格式化
来源：http://blog.vehdjk.com/Article/details/gatinndqr.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://blog.epnwcf.com/Article/details/gjjknohxs.sHtML

[R72] 等待端口就绪
来源：http://mobile.sjlbkw.cn/Article/details/ggurqwonl.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://m.share.fktsv.cn/Article/details/gpfxhbfmv.sHtML

[R73] 分割大日志
来源：http://blog.epnwcf.com/Article/details/gcirzlwzz.sHtML

split -l 1000 big.log part_
来源：http://www.m.share.epnwcf.com/Article/details/gwbaoecft.sHtML

[R74] 批量重命名
来源：http://www.blog.fktsv.cn/Article/details/gojhflwsf.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.share.yfazqb.com/Article/details/gqxmdrqjq.sHtML

[R75] 导出环境变量
来源：http://wap.fktsv.cn/Article/details/gillavbqk.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://read.share.sjlbkw.cn/Article/details/gqhprpfij.sHtML

[R76] 使用临时文件
来源：http://mobile.sjlbkw.cn/Article/details/gczklhkgb.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://3g.yfazqb.com/Article/details/gbivghitb.sHtML

[R77] 读取用户输入
来源：http://baike.fktsv.cn/Article/details/guraagoxw.sHtML

read -rp "请输入: " ans
来源：http://wap.bbcook.cn/Article/details/ghygogkkq.sHtML

[R78] 交互式菜单
来源：http://wap.sjlbkw.cn/Article/details/glkjztgux.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.share.yfazqb.com/Article/details/gtoxiupnz.sHtML

[R79] 解析命令行选项
来源：http://read.share.tarul.cn/Article/details/gicraumeg.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.blog.bbcook.cn/Article/details/gindfupey.sHtML

[R80] 查看脚本执行耗时
来源：http://blog.bbcook.cn/Article/details/gxzkkqcnh.sHtML

time ./run.sh
来源：http://baike.fktsv.cn/Article/details/gukwkesfh.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/grqwepexf.sHtML

S. C / C++ 专题
来源：http://www.m.share.fktsv.cn/Article/details/gwqcjtxgb.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/guqvtwyge.sHtML

[S01] C：Hello World
来源：http://m.share.epnwcf.com/Article/details/gjawkcjna.sHtML

#include <stdio.h>
来源：http://www.blog.tarul.cn/Article/details/gitydgpoa.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.m.share.yfazqb.com/Article/details/gmkvcwybp.sHtML

[S02] C：变量与格式化输出
来源：http://baike.fktsv.cn/Article/details/giuqodtko.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.m.share.epnwcf.com/Article/details/gdozqhvga.sHtML

[S03] C：读入整数
来源：http://www.blog.yfazqb.com/Article/details/glacpkbgy.sHtML

int x; scanf("%d", &x);
来源：http://baike.epnwcf.com/Article/details/gylflrfuq.sHtML

[S04] C：字符串复制
来源：http://www.blog.sjlbkw.cn/Article/details/gphusefen.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://baike.vehdjk.com/Article/details/gfmdanowh.sHtML

[S05] C：字符串长度
来源：http://wap.tarul.cn/Article/details/gzenhndjt.sHtML

strlen(s)
来源：http://wap.vehdjk.com/Article/details/gssoqbnzb.sHtML

[S06] C：字符串比较
来源：http://www.blog.yfazqb.com/Article/details/gddagnwqj.sHtML

strcmp(a, b) == 0
来源：http://baike.sjlbkw.cn/Article/details/gyaqbadpv.sHtML

[S07] C：数组遍历求和
来源：http://read.share.tarul.cn/Article/details/gzgphuity.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://baike.yfazqb.com/Article/details/graujeuhf.sHtML

[S08] C：动态内存分配与释放
来源：http://www.m.share.bbcook.cn/Article/details/greqqqjlz.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.share.epnwcf.com/Article/details/gtspalpqs.sHtML

[S09] C：结构体定义与初始化
来源：http://read.share.epnwcf.com/Article/details/gxrrudhhk.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://wap.epnwcf.com/Article/details/ghuqtdjoa.sHtML

[S10] C：指针与解引用
来源：http://blog.fktsv.cn/Article/details/gojvmbnhk.sHtML

int *p = &a;  *p = 5;
来源：http://blog.vehdjk.com/Article/details/gwqdglanz.sHtML

[S11] C：逐行读文件
来源：http://www.blog.bbcook.cn/Article/details/gzttoikim.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://baike.tarul.cn/Article/details/goudzgkyd.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.share.epnwcf.com/Article/details/gurgdiyri.sHtML

fclose(f);
来源：http://read.share.bbcook.cn/Article/details/ggcfmthlu.sHtML

[S12] C：写文件
来源：http://m.share.yfazqb.com/Article/details/gvvyknqrj.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://m.share.tarul.cn/Article/details/gojbvaffu.sHtML

[S13] C：宏定义
来源：http://read.share.fktsv.cn/Article/details/gxsryshiw.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wap.yfazqb.com/Article/details/gpufrulen.sHtML

[S14] C：枚举
来源：http://www.blog.epnwcf.com/Article/details/grpaqtxhq.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://read.share.sjlbkw.cn/Article/details/gbbqifqqq.sHtML

[S15] C：类型转换
来源：http://mobile.tarul.cn/Article/details/gcoqkinuk.sHtML

(double) a / b
来源：http://baike.tarul.cn/Article/details/gsprdaxdr.sHtML

[S16] C：位操作置位
来源：http://www.m.share.bbcook.cn/Article/details/gdlhnrfue.sHtML

x |= (1 << 3);
来源：http://baike.epnwcf.com/Article/details/gzcgivlot.sHtML

[S17] C：安全拼接字符串
来源：http://www.m.share.epnwcf.com/Article/details/gngivsejn.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wap.fktsv.cn/Article/details/gvhelwvfr.sHtML

[S18] C：命令行参数
来源：http://mobile.tarul.cn/Article/details/gzakozumu.sHtML

int main(int argc, char **argv)
来源：http://m.share.vehdjk.com/Article/details/grzggyyvp.sHtML

[S19] C：快速排序
来源：http://blog.epnwcf.com/Article/details/gxsovbrjo.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://3g.fktsv.cn/Article/details/gjamijspz.sHtML

[S20] C：二分查找
来源：http://m.share.epnwcf.com/Article/details/gpudkigte.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://blog.tarul.cn/Article/details/gacczizas.sHtML

[S21] C：字符类别判断
来源：http://www.blog.yfazqb.com/Article/details/gyvtgojdz.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://m.share.bbcook.cn/Article/details/gkhuhyszi.sHtML

[S22] C：字符串转数字
来源：http://read.share.tarul.cn/Article/details/gzfykcmkh.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.share.fktsv.cn/Article/details/gugvxvquw.sHtML

[S23] C：随机数
来源：http://wap.epnwcf.com/Article/details/gazkroqwz.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://wap.epnwcf.com/Article/details/gondshpzm.sHtML

[S24] C：获取本地时间
来源：http://m.share.sjlbkw.cn/Article/details/gytmhtjpd.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.share.bbcook.cn/Article/details/giqjmdssj.sHtML

[S25] C：内存拷贝
来源：http://www.share.sjlbkw.cn/Article/details/gtvhmqykp.sHtML

memcpy(dst, src, n);
来源：http://3g.sjlbkw.cn/Article/details/gmxokxzqt.sHtML

[S26] C：内存清零
来源：http://3g.sjlbkw.cn/Article/details/gnjhhvlzs.sHtML

memset(a, 0, sizeof a);
来源：http://www.share.epnwcf.com/Article/details/gzrupbiuq.sHtML

[S27] C：定义常量
来源：http://read.share.tarul.cn/Article/details/giqbymfkj.sHtML

const double PI = 3.14159;
来源：http://m.share.yfazqb.com/Article/details/gnjwewvhx.sHtML

[S28] C：静态变量
来源：http://m.share.yfazqb.com/Article/details/ggakqnnxk.sHtML

static int counter = 0;
来源：http://blog.tarul.cn/Article/details/geqtikzfm.sHtML

[S29] C：变参函数
来源：http://mobile.yfazqb.com/Article/details/gdelnnrcv.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://read.share.sjlbkw.cn/Article/details/gqraffayo.sHtML

[S30] C：头文件保护
来源：http://baike.epnwcf.com/Article/details/gvianiegm.sHtML

#ifndef X_H
来源：http://wap.fktsv.cn/Article/details/giegxvjuk.sHtML

#define X_H
来源：http://www.share.bbcook.cn/Article/details/gxlfnufcg.sHtML

#endif
来源：http://wap.bbcook.cn/Article/details/gezlnydgj.sHtML

[S31] C++：Hello World
来源：http://www.blog.tarul.cn/Article/details/gilrruckn.sHtML

#include <iostream>
来源：http://www.share.yfazqb.com/Article/details/gxwjuaati.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://mobile.vehdjk.com/Article/details/ggkirlzfp.sHtML

[S32] C++：字符串
来源：http://baike.fktsv.cn/Article/details/guafohdnz.sHtML

std::string s = "hi";  s += "!";
来源：http://mobile.vehdjk.com/Article/details/guyqsdige.sHtML

[S33] C++：vector 增删
来源：http://3g.sjlbkw.cn/Article/details/gvtipzufi.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://3g.epnwcf.com/Article/details/gdcxgmrew.sHtML

[S34] C++：遍历 vector
来源：http://mobile.sjlbkw.cn/Article/details/gthivymkw.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.m.share.yfazqb.com/Article/details/gejouimab.sHtML

[S35] C++：map
来源：http://read.share.sjlbkw.cn/Article/details/gzwnaxxar.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.sjlbkw.cn/Article/details/gflnwlwfp.sHtML

[S36] C++：unordered_map
来源：http://read.share.sjlbkw.cn/Article/details/gbeolfzzr.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://baike.tarul.cn/Article/details/gzjhgyqjm.sHtML

[S37] C++：set
来源：http://3g.tarul.cn/Article/details/ggcgqnxzm.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://baike.epnwcf.com/Article/details/geaysogwi.sHtML

[S38] C++：排序
来源：http://blog.tarul.cn/Article/details/gmcydgdet.sHtML

std::sort(v.begin(), v.end());
来源：http://blog.bbcook.cn/Article/details/gruwsfxkb.sHtML

[S39] C++：自定义比较器排序
来源：http://www.m.share.sjlbkw.cn/Article/details/gbezecvgi.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://mobile.epnwcf.com/Article/details/guhzavhcz.sHtML

[S40] C++：查找元素
来源：http://wap.vehdjk.com/Article/details/gholpqhbi.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://blog.fktsv.cn/Article/details/gdauvlphy.sHtML

[S41] C++：类与构造函数
来源：http://read.share.tarul.cn/Article/details/gakdblyjt.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://read.share.sjlbkw.cn/Article/details/ggslqrixf.sHtML

[S42] C++：继承与虚函数
来源：http://3g.epnwcf.com/Article/details/gudoinqmr.sHtML

class B : public Base { public: void f() override {} };
来源：http://mobile.tarul.cn/Article/details/ghhvhmzew.sHtML

[S43] C++：智能指针
来源：http://baike.vehdjk.com/Article/details/gvqhxigal.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.m.share.vehdjk.com/Article/details/gyecvnjlb.sHtML

[S44] C++：引用传参
来源：http://m.share.sjlbkw.cn/Article/details/gmlbilisz.sHtML

void inc(int &x) { ++x; }
来源：http://blog.bbcook.cn/Article/details/gdyfczxzt.sHtML

[S45] C++：lambda
来源：http://www.share.vehdjk.com/Article/details/gxjzsklrh.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://wap.fktsv.cn/Article/details/gumvmusqg.sHtML

[S46] C++：函数模板
来源：http://mobile.vehdjk.com/Article/details/gbrjmcxvq.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://m.share.tarul.cn/Article/details/gcocghsel.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.share.vehdjk.com/Article/details/gfuoohxgj.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.m.share.yfazqb.com/Article/details/gvughuuqy.sHtML

[S48] C++：逐行读文件
来源：http://3g.fktsv.cn/Article/details/gmafklhjz.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.share.epnwcf.com/Article/details/gowdliqzw.sHtML

while (std::getline(in, line)) { }
来源：http://blog.epnwcf.com/Article/details/gvhidqjvy.sHtML

[S49] C++：写文件
来源：http://www.m.share.bbcook.cn/Article/details/gjkuffwty.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.m.share.bbcook.cn/Article/details/gdeksburd.sHtML

[S50] C++：格式化数字
来源：http://wap.fktsv.cn/Article/details/gsstqvqbw.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://read.share.bbcook.cn/Article/details/gtudlvayr.sHtML

[S51] C++：显式类型转换
来源：http://www.m.share.sjlbkw.cn/Article/details/gewmcludy.sHtML

static_cast<double>(a) / b
来源：http://mobile.epnwcf.com/Article/details/gxuhsaekn.sHtML

[S52] C++：const 与 noexcept
来源：http://www.blog.vehdjk.com/Article/details/gkgyfcpca.sHtML

int size() const noexcept { return n_; }
来源：http://blog.tarul.cn/Article/details/grkrtuqej.sHtML

[S53] C++：移动语义
来源：http://baike.vehdjk.com/Article/details/gguqkcczn.sHtML

std::vector<int> w = std::move(v);
来源：http://m.share.fktsv.cn/Article/details/gebinzury.sHtML

[S54] C++：异常处理
来源：http://read.share.fktsv.cn/Article/details/gkehjslgy.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://read.share.fktsv.cn/Article/details/gkdatgnkp.sHtML

[S55] C++：结构化绑定
来源：http://3g.bbcook.cn/Article/details/gjhayifbz.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.blog.vehdjk.com/Article/details/gjdkcztbj.sHtML

[S56] C++：optional
来源：http://mobile.bbcook.cn/Article/details/glgaymrgu.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.m.share.vehdjk.com/Article/details/gxblvwsyl.sHtML

[S57] C++：编译期常量
来源：http://www.blog.fktsv.cn/Article/details/gzpxbpayg.sHtML

constexpr int N = 10;
来源：http://blog.epnwcf.com/Article/details/gjsxbxqhe.sHtML

[S58] C++：命名空间
来源：http://baike.yfazqb.com/Article/details/grjfnlvjc.sHtML

namespace ns { int f() { return 1; } }
来源：http://3g.fktsv.cn/Article/details/gqxzijswc.sHtML

[S59] C++：静态断言
来源：http://read.share.fktsv.cn/Article/details/grdokoyng.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://read.share.vehdjk.com/Article/details/gacpzdmpk.sHtML

[S60] C++：遍历并删除元素
来源：http://www.blog.tarul.cn/Article/details/gpbshbonj.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://baike.tarul.cn/Article/details/gzeemywct.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/gqmhjzbct.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://wap.bbcook.cn/Article/details/gmashsyar.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/gngdtvqdh.sHtML

[T01] Kotlin：Hello World
来源：http://www.m.share.vehdjk.com/Article/details/gmywatdvi.sHtML

println("Hello")
来源：http://mobile.bbcook.cn/Article/details/gkzfkxfce.sHtML

[T02] Kotlin：变量
来源：http://read.share.tarul.cn/Article/details/gafkiapfo.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://blog.sjlbkw.cn/Article/details/guspxdere.sHtML

[T03] Kotlin：字符串模板
来源：http://m.share.fktsv.cn/Article/details/gwwhbvkhq.sHtML

"值: $b"
来源：http://www.blog.epnwcf.com/Article/details/gmqclcphn.sHtML

[T04] Kotlin：空安全
来源：http://blog.tarul.cn/Article/details/grjvaghbh.sHtML

val n: String? = null;  n?.length
来源：http://baike.epnwcf.com/Article/details/gszsbpedd.sHtML

[T05] Kotlin：when 表达式
来源：http://mobile.yfazqb.com/Article/details/gdhjpefey.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.m.share.epnwcf.com/Article/details/glsinpljl.sHtML

[T06] Kotlin：集合映射
来源：http://blog.sjlbkw.cn/Article/details/gdyekhkvx.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.blog.vehdjk.com/Article/details/gucrulagn.sHtML

[T07] Kotlin：集合过滤
来源：http://www.m.share.vehdjk.com/Article/details/gnvuavhqj.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.share.tarul.cn/Article/details/gpkjdsdpq.sHtML

[T08] Kotlin：数据类
来源：http://3g.epnwcf.com/Article/details/gcuaxdmlw.sHtML

data class User(val name: String, val age: Int)
来源：http://www.blog.epnwcf.com/Article/details/geekxsawf.sHtML


<!-- 参考信息 -->