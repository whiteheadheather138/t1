代发 wailian999

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://baike.fktsv.cn/Article/details/ghmequsvz.sHtML

[R10] 正则匹配
来源：http://3g.bbcook.cn/Article/details/gpmpygbgt.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://wap.epnwcf.com/Article/details/gjdzrwuab.sHtML

[R11] case 多分支
来源：http://www.share.fktsv.cn/Article/details/gpgtwxybl.sHtML

case "$1" in
来源：http://baike.yfazqb.com/Article/details/gnbjwmlel.sHtML

start) echo "启动" ;;
来源：http://www.m.share.sjlbkw.cn/Article/details/gowbdcjng.sHtML

stop)  echo "停止" ;;
来源：http://blog.fktsv.cn/Article/details/gtkytbfbd.sHtML

*)     echo "未知命令" ;;
来源：http://blog.sjlbkw.cn/Article/details/gxnsdwqpi.sHtML

esac
来源：http://mobile.yfazqb.com/Article/details/gokzjryyd.sHtML

[R12] for 遍历文件
来源：http://3g.tarul.cn/Article/details/gzihespxx.sHtML

for f in *.txt; do echo "$f"; done
来源：http://3g.sjlbkw.cn/Article/details/gybhvpbkp.sHtML

[R13] for 计数循环
来源：http://www.share.fktsv.cn/Article/details/gfiywzipa.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.share.yfazqb.com/Article/details/grxmysyji.sHtML

[R14] C 风格 for
来源：http://blog.yfazqb.com/Article/details/grinxafrc.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://blog.fktsv.cn/Article/details/gmhvmjvwo.sHtML

[R15] while 逐行读文件
来源：http://m.share.tarul.cn/Article/details/ghpravqsk.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://mobile.epnwcf.com/Article/details/gwgnashsq.sHtML

[R16] until 等待条件
来源：http://blog.fktsv.cn/Article/details/gmkvzoroh.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://read.share.fktsv.cn/Article/details/gmfojcqfq.sHtML

[R17] 数组定义与取值
来源：http://3g.fktsv.cn/Article/details/grgxwnqli.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://wap.fktsv.cn/Article/details/gxerzdotf.sHtML

[R18] 遍历数组
来源：http://www.share.fktsv.cn/Article/details/gbgwhhhnc.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://baike.vehdjk.com/Article/details/ghwrtlcsq.sHtML

[R19] 数组长度
来源：http://www.share.vehdjk.com/Article/details/gddpcdjqc.sHtML

echo "${#arr[@]}"
来源：http://www.m.share.yfazqb.com/Article/details/gikifodcq.sHtML

[R20] 关联数组（字典）
来源：http://read.share.yfazqb.com/Article/details/gruvrvvsj.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://wap.tarul.cn/Article/details/gabnhdoeg.sHtML

[R21] 字符串长度
来源：http://www.blog.epnwcf.com/Article/details/gsujbvcxt.sHtML

echo "${#s}"
来源：http://wap.tarul.cn/Article/details/givwfxkma.sHtML

[R22] 截取子串
来源：http://m.share.fktsv.cn/Article/details/gemebhaze.sHtML

echo "${s:0:5}"
来源：http://3g.bbcook.cn/Article/details/gnsysgzzk.sHtML

[R23] 字符串替换
来源：http://www.m.share.fktsv.cn/Article/details/gtlxzdlnx.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://read.share.sjlbkw.cn/Article/details/ghduyejae.sHtML

[R24] 大小写转换
来源：http://wap.vehdjk.com/Article/details/gnkkjzhgb.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://m.share.epnwcf.com/Article/details/gxdfhvizj.sHtML

[R25] 去后缀 / 去前缀
来源：http://baike.epnwcf.com/Article/details/gmbcrwncj.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://read.share.fktsv.cn/Article/details/gescohgbn.sHtML

[R26] 命令替换
来源：http://www.blog.tarul.cn/Article/details/gkgcjovlk.sHtML

now=$(date +%F); echo "$now"
来源：http://www.blog.bbcook.cn/Article/details/gypccoqtz.sHtML

[R27] 算术展开
来源：http://www.blog.fktsv.cn/Article/details/gslwbtsae.sHtML

echo $((1 + 2 * 3))
来源：http://read.share.sjlbkw.cn/Article/details/gyrgxuhjj.sHtML

[R28] 浮点运算
来源：http://mobile.sjlbkw.cn/Article/details/gskhfpmai.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.share.bbcook.cn/Article/details/gcitvcqcx.sHtML

[R29] 定义函数
来源：http://baike.yfazqb.com/Article/details/guuhugnmi.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://3g.epnwcf.com/Article/details/ggvnikhlo.sHtML

[R30] 函数返回状态码
来源：http://www.share.sjlbkw.cn/Article/details/gnwvggbkh.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://baike.epnwcf.com/Article/details/gahmdklct.sHtML

[R31] 局部变量
来源：http://3g.bbcook.cn/Article/details/gylxckzxn.sHtML

f() { local x=1; echo "$x"; }
来源：http://wap.tarul.cn/Article/details/gylkyrecd.sHtML

[R32] 参数个数校验
来源：http://www.m.share.epnwcf.com/Article/details/gkqaexlsx.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://blog.tarul.cn/Article/details/gbskhmrwf.sHtML

[R33] 捕获错误并提示行号
来源：http://m.share.epnwcf.com/Article/details/gwgbwngfw.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://3g.sjlbkw.cn/Article/details/gamnssbbx.sHtML

[R34] 退出时清理
来源：http://m.share.fktsv.cn/Article/details/gsvvkcwje.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://mobile.tarul.cn/Article/details/gxncyxrmz.sHtML

[R35] 后台执行并等待
来源：http://www.blog.yfazqb.com/Article/details/gtdcaqhyd.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.blog.fktsv.cn/Article/details/gvanlvmcc.sHtML

[R36] 并发执行多个任务
来源：http://www.m.share.sjlbkw.cn/Article/details/gwtmduigv.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.m.share.yfazqb.com/Article/details/gljtgwkgu.sHtML

[R37] 把输出赋给变量
来源：http://wap.epnwcf.com/Article/details/gzhgprugf.sHtML

files=$(ls -1)
来源：http://www.m.share.vehdjk.com/Article/details/gvmepgrad.sHtML

[R38] 管道串联
来源：http://www.blog.bbcook.cn/Article/details/getwnaojf.sHtML

cat a.txt | grep -i error | wc -l
来源：http://mobile.sjlbkw.cn/Article/details/gtyfppnyv.sHtML

[R39] 重定向标准输出与错误
来源：http://read.share.fktsv.cn/Article/details/gcyeocbot.sHtML

cmd > out.log 2>&1
来源：http://www.m.share.tarul.cn/Article/details/ghbjwuckk.sHtML

[R40] 追加写日志
来源：http://baike.yfazqb.com/Article/details/gmcmjgvcn.sHtML

echo "log" >> out.log
来源：http://www.share.bbcook.cn/Article/details/geciptseg.sHtML

[R41] 丢弃输出
来源：http://baike.sjlbkw.cn/Article/details/gngnrwdmp.sHtML

cmd >/dev/null 2>&1
来源：http://3g.yfazqb.com/Article/details/gwxegjffb.sHtML

[R42] 输入重定向
来源：http://m.share.bbcook.cn/Article/details/gkigjrzeo.sHtML

wc -l < a.txt
来源：http://baike.epnwcf.com/Article/details/gydoeewai.sHtML

[R43] 按名字查找文件
来源：http://read.share.vehdjk.com/Article/details/gpteotmun.sHtML

find . -name "*.log" -type f
来源：http://wap.bbcook.cn/Article/details/gsrvxucsx.sHtML

[R44] 按修改时间查找
来源：http://wap.epnwcf.com/Article/details/gyflyhdvn.sHtML

find . -mtime -7 -type f
来源：http://3g.fktsv.cn/Article/details/gfrycoxqo.sHtML

[R45] 批量删除
来源：http://read.share.yfazqb.com/Article/details/gubwvhirc.sHtML

find . -name "*.tmp" -delete
来源：http://baike.epnwcf.com/Article/details/gcdwujfxa.sHtML

[R46] 递归替换文件内容
来源：http://read.share.epnwcf.com/Article/details/gtclhzbkt.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://baike.fktsv.cn/Article/details/goctwbbsl.sHtML

[R47] sed 单行替换
来源：http://wap.yfazqb.com/Article/details/gqrekbbdh.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://3g.tarul.cn/Article/details/gggqyxolh.sHtML

[R48] awk 取指定列
来源：http://read.share.fktsv.cn/Article/details/gwchyzxyq.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.m.share.bbcook.cn/Article/details/gicvhtlqf.sHtML

[R49] awk 带条件
来源：http://blog.fktsv.cn/Article/details/gylkstadu.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.m.share.fktsv.cn/Article/details/gklkxiogr.sHtML

[R50] awk 求和
来源：http://www.blog.vehdjk.com/Article/details/gbjehfnki.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://baike.yfazqb.com/Article/details/gpaxxltik.sHtML

[R51] 排序去重取前几
来源：http://mobile.epnwcf.com/Article/details/gmcxovxmc.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://m.share.tarul.cn/Article/details/googkwucr.sHtML

[R52] 统计行数
来源：http://www.share.vehdjk.com/Article/details/gxsnehlhq.sHtML

wc -l a.txt
来源：http://wap.tarul.cn/Article/details/ghnyxgcqy.sHtML

[R53] 查看文件头与实时尾
来源：http://3g.tarul.cn/Article/details/gazxirflj.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.m.share.fktsv.cn/Article/details/gfhfqtbov.sHtML

[R54] 比较两个文件
来源：http://read.share.yfazqb.com/Article/details/gtmjhhhno.sHtML

diff a.txt b.txt
来源：http://m.share.fktsv.cn/Article/details/gxivxckkj.sHtML

[R55] 压缩与解压
来源：http://baike.bbcook.cn/Article/details/gjanoavrj.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://read.share.vehdjk.com/Article/details/gpnpyzfsc.sHtML

[R56] 远程拷贝
来源：http://www.blog.tarul.cn/Article/details/gbhzlqkyi.sHtML

scp file user@host:/path/
来源：http://www.share.vehdjk.com/Article/details/gszqhacsv.sHtML

[R57] 远程执行命令
来源：http://www.blog.fktsv.cn/Article/details/gudgrplto.sHtML

ssh user@host 'uptime'
来源：http://read.share.vehdjk.com/Article/details/gekhytgvp.sHtML

[R58] 下载文件
来源：http://wap.vehdjk.com/Article/details/gcxdflidq.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://read.share.sjlbkw.cn/Article/details/gfpffkivq.sHtML

[R59] 发 POST JSON
来源：http://m.share.vehdjk.com/Article/details/gxbkyokbz.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.blog.fktsv.cn/Article/details/goxdnfeii.sHtML

[R60] 只看 HTTP 状态码
来源：http://blog.vehdjk.com/Article/details/gbgjmoakm.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mobile.fktsv.cn/Article/details/gszavqvkz.sHtML

[R61] 磁盘占用
来源：http://wap.bbcook.cn/Article/details/gpntzvkxo.sHtML

df -h;  du -sh *
来源：http://www.m.share.sjlbkw.cn/Article/details/glypawqdx.sHtML

[R62] 找最占空间的文件
来源：http://wap.vehdjk.com/Article/details/gjioedqdx.sHtML

du -ah . | sort -rh | head -10
来源：http://mobile.tarul.cn/Article/details/glfbfbolt.sHtML

[R63] 内存与进程
来源：http://www.m.share.yfazqb.com/Article/details/gegimwkxj.sHtML

free -h;  ps aux | grep nginx
来源：http://blog.sjlbkw.cn/Article/details/gkmocbvnz.sHtML

[R64] 结束进程
来源：http://read.share.vehdjk.com/Article/details/gznfkmxbl.sHtML

kill -9 $(pgrep -f app.py)
来源：http://blog.bbcook.cn/Article/details/gpieezbip.sHtML

[R65] 查看端口占用
来源：http://mobile.tarul.cn/Article/details/gtmuuaqxf.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mobile.tarul.cn/Article/details/gncemynsf.sHtML

[R66] 定时任务
来源：http://www.blog.yfazqb.com/Article/details/gdyvheyhp.sHtML

crontab -e;  crontab -l
来源：http://read.share.vehdjk.com/Article/details/gsangwrpw.sHtML

[R67] 生成随机十六进制串
来源：http://blog.vehdjk.com/Article/details/gsljexofa.sHtML

openssl rand -hex 16
来源：http://mobile.yfazqb.com/Article/details/gwixgmokn.sHtML

[R68] 计算文件校验值
来源：http://3g.bbcook.cn/Article/details/grdubfzia.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://read.share.yfazqb.com/Article/details/gpfzppukt.sHtML

[R69] 生成随机密码
来源：http://read.share.sjlbkw.cn/Article/details/gbusvpudl.sHtML

head -c 16 /dev/urandom | base64
来源：http://read.share.fktsv.cn/Article/details/gfanpsqjv.sHtML

[R70] 时间戳与互转
来源：http://www.share.epnwcf.com/Article/details/gnfucsvot.sHtML

date +%s;  date -d @1700000000
来源：http://wap.bbcook.cn/Article/details/ghhprotqu.sHtML

[R71] 日期格式化
来源：http://read.share.bbcook.cn/Article/details/geyjtdtea.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://baike.epnwcf.com/Article/details/ghsjhswxm.sHtML

[R72] 等待端口就绪
来源：http://www.blog.epnwcf.com/Article/details/gndlusfpj.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://baike.yfazqb.com/Article/details/gxhnisydk.sHtML

[R73] 分割大日志
来源：http://www.m.share.vehdjk.com/Article/details/gxejzgcsb.sHtML

split -l 1000 big.log part_
来源：http://www.m.share.bbcook.cn/Article/details/ggqxztoya.sHtML

[R74] 批量重命名
来源：http://blog.vehdjk.com/Article/details/gmslzqgky.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://m.share.fktsv.cn/Article/details/gfmrywgib.sHtML

[R75] 导出环境变量
来源：http://www.share.yfazqb.com/Article/details/goyckirll.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://read.share.fktsv.cn/Article/details/gjcelwehb.sHtML

[R76] 使用临时文件
来源：http://www.share.yfazqb.com/Article/details/gesywxdkh.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://m.share.sjlbkw.cn/Article/details/gyghebgnr.sHtML

[R77] 读取用户输入
来源：http://www.blog.sjlbkw.cn/Article/details/gzfdfotva.sHtML

read -rp "请输入: " ans
来源：http://blog.sjlbkw.cn/Article/details/gtctwyilr.sHtML

[R78] 交互式菜单
来源：http://www.share.vehdjk.com/Article/details/gkldtamhm.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.blog.sjlbkw.cn/Article/details/glifdnyqq.sHtML

[R79] 解析命令行选项
来源：http://m.share.bbcook.cn/Article/details/gpbdcmsju.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mobile.tarul.cn/Article/details/gkyvplepu.sHtML

[R80] 查看脚本执行耗时
来源：http://wap.yfazqb.com/Article/details/gezrlfzqo.sHtML

time ./run.sh
来源：http://blog.sjlbkw.cn/Article/details/gwhzlhrot.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/gbbylcbph.sHtML

S. C / C++ 专题
来源：http://baike.vehdjk.com/Article/details/goewgqbqc.sHtML

================================================================================
来源：http://3g.sjlbkw.cn/Article/details/gzpreivtv.sHtML

[S01] C：Hello World
来源：http://www.m.share.sjlbkw.cn/Article/details/gugtkbsat.sHtML

#include <stdio.h>
来源：http://www.m.share.yfazqb.com/Article/details/gaspzwuid.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://m.share.vehdjk.com/Article/details/gphlipcby.sHtML

[S02] C：变量与格式化输出
来源：http://wap.bbcook.cn/Article/details/gdvmbwgaz.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.m.share.sjlbkw.cn/Article/details/gzherzzpo.sHtML

[S03] C：读入整数
来源：http://wap.sjlbkw.cn/Article/details/gkndmfqwp.sHtML

int x; scanf("%d", &x);
来源：http://3g.vehdjk.com/Article/details/gemjkhtjm.sHtML

[S04] C：字符串复制
来源：http://www.m.share.bbcook.cn/Article/details/gbrxsuybp.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.blog.fktsv.cn/Article/details/gbkguyzfd.sHtML

[S05] C：字符串长度
来源：http://www.m.share.bbcook.cn/Article/details/ggqpxgwod.sHtML

strlen(s)
来源：http://read.share.fktsv.cn/Article/details/gcmgssvxp.sHtML

[S06] C：字符串比较
来源：http://wap.fktsv.cn/Article/details/gmgbucvlq.sHtML

strcmp(a, b) == 0
来源：http://www.share.fktsv.cn/Article/details/gwwrbfvmj.sHtML

[S07] C：数组遍历求和
来源：http://mobile.yfazqb.com/Article/details/gdsuqmqsm.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://blog.vehdjk.com/Article/details/gtwnikdkw.sHtML

[S08] C：动态内存分配与释放
来源：http://www.m.share.bbcook.cn/Article/details/geblkmgkj.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://m.share.bbcook.cn/Article/details/gamwbleou.sHtML

[S09] C：结构体定义与初始化
来源：http://mobile.sjlbkw.cn/Article/details/gpckswfob.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://3g.vehdjk.com/Article/details/gbeskahlq.sHtML

[S10] C：指针与解引用
来源：http://www.m.share.fktsv.cn/Article/details/gpzsyqfol.sHtML

int *p = &a;  *p = 5;
来源：http://baike.vehdjk.com/Article/details/gzuiqtuir.sHtML

[S11] C：逐行读文件
来源：http://wap.sjlbkw.cn/Article/details/glnatdvcw.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.m.share.vehdjk.com/Article/details/guimwzqpo.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://mobile.bbcook.cn/Article/details/gchlnjjpj.sHtML

fclose(f);
来源：http://www.blog.epnwcf.com/Article/details/gtdoholbw.sHtML

[S12] C：写文件
来源：http://wap.fktsv.cn/Article/details/gpikgekry.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://3g.vehdjk.com/Article/details/gtyhxarhd.sHtML

[S13] C：宏定义
来源：http://www.m.share.bbcook.cn/Article/details/gaouvsmqm.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://baike.tarul.cn/Article/details/gcpcbuiwa.sHtML

[S14] C：枚举
来源：http://baike.vehdjk.com/Article/details/gcgnsvcmg.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.m.share.sjlbkw.cn/Article/details/googexzfq.sHtML

[S15] C：类型转换
来源：http://3g.epnwcf.com/Article/details/gfdklinre.sHtML

(double) a / b
来源：http://www.m.share.tarul.cn/Article/details/gjfzvoxpa.sHtML

[S16] C：位操作置位
来源：http://www.share.epnwcf.com/Article/details/ggshsmjob.sHtML

x |= (1 << 3);
来源：http://read.share.epnwcf.com/Article/details/glzrdwbka.sHtML

[S17] C：安全拼接字符串
来源：http://wap.yfazqb.com/Article/details/gznuopzjk.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://baike.tarul.cn/Article/details/gascehnic.sHtML

[S18] C：命令行参数
来源：http://blog.tarul.cn/Article/details/gdztsadxj.sHtML

int main(int argc, char **argv)
来源：http://wap.sjlbkw.cn/Article/details/geeaiunzs.sHtML

[S19] C：快速排序
来源：http://wap.yfazqb.com/Article/details/gmfyjbaem.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://blog.bbcook.cn/Article/details/gubjootaa.sHtML

[S20] C：二分查找
来源：http://www.m.share.bbcook.cn/Article/details/gtqjhzewv.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://blog.sjlbkw.cn/Article/details/guavgzaug.sHtML

[S21] C：字符类别判断
来源：http://www.blog.tarul.cn/Article/details/gbzdfskmn.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://m.share.tarul.cn/Article/details/gpffrjhln.sHtML

[S22] C：字符串转数字
来源：http://www.m.share.vehdjk.com/Article/details/gofktfjbw.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://m.share.bbcook.cn/Article/details/gjijdgcgf.sHtML

[S23] C：随机数
来源：http://read.share.vehdjk.com/Article/details/gbfafpzpi.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://m.share.sjlbkw.cn/Article/details/geuuqietr.sHtML

[S24] C：获取本地时间
来源：http://blog.epnwcf.com/Article/details/gfwpsqcog.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.m.share.bbcook.cn/Article/details/gwhavvvdx.sHtML

[S25] C：内存拷贝
来源：http://baike.yfazqb.com/Article/details/goadgidqn.sHtML

memcpy(dst, src, n);
来源：http://baike.vehdjk.com/Article/details/gddztaamo.sHtML

[S26] C：内存清零
来源：http://mobile.fktsv.cn/Article/details/geazwycff.sHtML

memset(a, 0, sizeof a);
来源：http://3g.vehdjk.com/Article/details/gqsjsvvex.sHtML

[S27] C：定义常量
来源：http://blog.fktsv.cn/Article/details/gtnhmropk.sHtML

const double PI = 3.14159;
来源：http://mobile.vehdjk.com/Article/details/ggxhvbzbo.sHtML

[S28] C：静态变量
来源：http://blog.vehdjk.com/Article/details/gcsiwhsvi.sHtML

static int counter = 0;
来源：http://www.m.share.epnwcf.com/Article/details/gffgvbsvo.sHtML

[S29] C：变参函数
来源：http://wap.yfazqb.com/Article/details/gccoocopb.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://3g.tarul.cn/Article/details/gewycfnyh.sHtML

[S30] C：头文件保护
来源：http://baike.epnwcf.com/Article/details/gecxjjxfn.sHtML

#ifndef X_H
来源：http://www.share.sjlbkw.cn/Article/details/gipubegeb.sHtML

#define X_H
来源：http://3g.bbcook.cn/Article/details/gntiqoqxf.sHtML

#endif
来源：http://baike.tarul.cn/Article/details/gxkkhwpuh.sHtML

[S31] C++：Hello World
来源：http://m.share.bbcook.cn/Article/details/gtjnrvpfy.sHtML

#include <iostream>
来源：http://baike.tarul.cn/Article/details/gusqgswyb.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://baike.fktsv.cn/Article/details/gprahzlrt.sHtML

[S32] C++：字符串
来源：http://3g.bbcook.cn/Article/details/gfbdvnxwj.sHtML

std::string s = "hi";  s += "!";
来源：http://baike.vehdjk.com/Article/details/gwvfinnmb.sHtML

[S33] C++：vector 增删
来源：http://wap.epnwcf.com/Article/details/gpbmlcvyi.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.share.vehdjk.com/Article/details/gzplrmeih.sHtML

[S34] C++：遍历 vector
来源：http://read.share.yfazqb.com/Article/details/gbbtojrcr.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://blog.tarul.cn/Article/details/gxagloaro.sHtML

[S35] C++：map
来源：http://wap.bbcook.cn/Article/details/gqlfmvodu.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.bbcook.cn/Article/details/gehzaesdl.sHtML

[S36] C++：unordered_map
来源：http://m.share.epnwcf.com/Article/details/gpqrbinqg.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.tarul.cn/Article/details/glqwfchge.sHtML

[S37] C++：set
来源：http://baike.epnwcf.com/Article/details/genyfnytn.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.m.share.sjlbkw.cn/Article/details/gicrlkwga.sHtML

[S38] C++：排序
来源：http://blog.fktsv.cn/Article/details/griaivorm.sHtML

std::sort(v.begin(), v.end());
来源：http://www.m.share.sjlbkw.cn/Article/details/gjrkzxnqp.sHtML

[S39] C++：自定义比较器排序
来源：http://m.share.sjlbkw.cn/Article/details/gzeeuftyh.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.share.sjlbkw.cn/Article/details/gnilifpks.sHtML

[S40] C++：查找元素
来源：http://m.share.epnwcf.com/Article/details/gfzalmebc.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://3g.epnwcf.com/Article/details/gpmioqtrr.sHtML

[S41] C++：类与构造函数
来源：http://www.share.yfazqb.com/Article/details/gtmfealbt.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://m.share.bbcook.cn/Article/details/gkaslwwfy.sHtML

[S42] C++：继承与虚函数
来源：http://blog.tarul.cn/Article/details/gkipsllpn.sHtML

class B : public Base { public: void f() override {} };
来源：http://m.share.yfazqb.com/Article/details/gmjkeaqmq.sHtML

[S43] C++：智能指针
来源：http://3g.fktsv.cn/Article/details/grfsgenba.sHtML

auto p = std::make_unique<int>(5);
来源：http://read.share.tarul.cn/Article/details/gmfshiuap.sHtML

[S44] C++：引用传参
来源：http://mobile.sjlbkw.cn/Article/details/gegupbxug.sHtML

void inc(int &x) { ++x; }
来源：http://www.blog.epnwcf.com/Article/details/gixqhvgot.sHtML

[S45] C++：lambda
来源：http://read.share.bbcook.cn/Article/details/gdwvckaob.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://m.share.tarul.cn/Article/details/gdwyxjoof.sHtML

[S46] C++：函数模板
来源：http://www.m.share.tarul.cn/Article/details/gislxfaxv.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://baike.epnwcf.com/Article/details/gqlnwjfco.sHtML

[S47] C++：结构化绑定遍历
来源：http://m.share.sjlbkw.cn/Article/details/glhgsbdpd.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.blog.fktsv.cn/Article/details/glaskdbtw.sHtML

[S48] C++：逐行读文件
来源：http://www.blog.tarul.cn/Article/details/gavykbwhf.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.m.share.epnwcf.com/Article/details/gmiawblri.sHtML

while (std::getline(in, line)) { }
来源：http://www.share.fktsv.cn/Article/details/gqkuaddbn.sHtML

[S49] C++：写文件
来源：http://3g.epnwcf.com/Article/details/gkskbcegk.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://3g.vehdjk.com/Article/details/gmixelrgi.sHtML

[S50] C++：格式化数字
来源：http://blog.tarul.cn/Article/details/gtxilvpsu.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://read.share.fktsv.cn/Article/details/gwivyhrui.sHtML

[S51] C++：显式类型转换
来源：http://www.m.share.sjlbkw.cn/Article/details/gpmcxoksh.sHtML

static_cast<double>(a) / b
来源：http://read.share.yfazqb.com/Article/details/gbvapyhpz.sHtML

[S52] C++：const 与 noexcept
来源：http://mobile.fktsv.cn/Article/details/gibkadpru.sHtML

int size() const noexcept { return n_; }
来源：http://wap.epnwcf.com/Article/details/gshewoerk.sHtML

[S53] C++：移动语义
来源：http://www.blog.fktsv.cn/Article/details/gzzgtlmpg.sHtML

std::vector<int> w = std::move(v);
来源：http://mobile.epnwcf.com/Article/details/gtmdivnpn.sHtML

[S54] C++：异常处理
来源：http://3g.tarul.cn/Article/details/ghhqxgqiz.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://mobile.yfazqb.com/Article/details/gxvrvfucb.sHtML

[S55] C++：结构化绑定
来源：http://baike.bbcook.cn/Article/details/gzyjbzwpu.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://m.share.yfazqb.com/Article/details/gmxfakvxi.sHtML

[S56] C++：optional
来源：http://www.blog.vehdjk.com/Article/details/gqbvhirgz.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://mobile.epnwcf.com/Article/details/gxmxtnwry.sHtML

[S57] C++：编译期常量
来源：http://www.blog.sjlbkw.cn/Article/details/gjbedhyge.sHtML

constexpr int N = 10;
来源：http://www.blog.fktsv.cn/Article/details/gxykkoone.sHtML

[S58] C++：命名空间
来源：http://blog.bbcook.cn/Article/details/geoxyvzri.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.blog.fktsv.cn/Article/details/ghhvtmhek.sHtML

[S59] C++：静态断言
来源：http://m.share.fktsv.cn/Article/details/gjfnntfaj.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://blog.fktsv.cn/Article/details/guvyyzmyz.sHtML

[S60] C++：遍历并删除元素
来源：http://baike.vehdjk.com/Article/details/gxsfqfrom.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.blog.sjlbkw.cn/Article/details/gzfolhuwk.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/gyoivbbco.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.blog.vehdjk.com/Article/details/gsyaxenye.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/gubceyqqc.sHtML

[T01] Kotlin：Hello World
来源：http://3g.tarul.cn/Article/details/gqntvbusr.sHtML

println("Hello")
来源：http://mobile.yfazqb.com/Article/details/gunbfktyw.sHtML

[T02] Kotlin：变量
来源：http://blog.epnwcf.com/Article/details/gsuppepzd.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://mobile.vehdjk.com/Article/details/gpktfofdx.sHtML

[T03] Kotlin：字符串模板
来源：http://read.share.sjlbkw.cn/Article/details/gpuuvvwut.sHtML

"值: $b"
来源：http://read.share.fktsv.cn/Article/details/gpgqzpmjt.sHtML

[T04] Kotlin：空安全
来源：http://www.blog.tarul.cn/Article/details/gioxayois.sHtML

val n: String? = null;  n?.length
来源：http://www.blog.sjlbkw.cn/Article/details/gkdlottdx.sHtML

[T05] Kotlin：when 表达式
来源：http://3g.bbcook.cn/Article/details/gliviwajt.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://blog.sjlbkw.cn/Article/details/gxquwbqzm.sHtML

[T06] Kotlin：集合映射
来源：http://baike.vehdjk.com/Article/details/guiuftisy.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.blog.tarul.cn/Article/details/gnjlnjqja.sHtML

[T07] Kotlin：集合过滤
来源：http://www.blog.fktsv.cn/Article/details/gkcmjfoyl.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.share.tarul.cn/Article/details/gqpqezweh.sHtML

[T08] Kotlin：数据类
来源：http://www.blog.epnwcf.com/Article/details/gfbkvcogp.sHtML

data class User(val name: String, val age: Int)
来源：http://wap.vehdjk.com/Article/details/gzkhidopx.sHtML

[T09] Kotlin：扩展函数
来源：http://www.blog.sjlbkw.cn/Article/details/gwwoctnxu.sHtML

fun String.exclaim() = this + "!"
来源：http://www.blog.epnwcf.com/Article/details/gbtvnrubt.sHtML

[T10] Kotlin：默认参数
来源：http://www.m.share.sjlbkw.cn/Article/details/gohvprbmo.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.m.share.yfazqb.com/Article/details/geddtllom.sHtML


<!-- 参考信息 -->