代发 wailian999

echo "${#s}"
来源：http://wap.bbcook.cn/Article/details/geenitduy.sHtML

[R22] 截取子串
来源：http://blog.fktsv.cn/Article/details/gofqjyqbv.sHtML

echo "${s:0:5}"
来源：http://www.m.share.epnwcf.com/Article/details/gwtznzops.sHtML

[R23] 字符串替换
来源：http://read.share.tarul.cn/Article/details/gztojzfoe.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.share.epnwcf.com/Article/details/ghebghwat.sHtML

[R24] 大小写转换
来源：http://3g.bbcook.cn/Article/details/gjkbffsjg.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://read.share.fktsv.cn/Article/details/gmpshgzmi.sHtML

[R25] 去后缀 / 去前缀
来源：http://wap.vehdjk.com/Article/details/gvyfirxyr.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://3g.tarul.cn/Article/details/ghrruvrdx.sHtML

[R26] 命令替换
来源：http://3g.epnwcf.com/Article/details/gbqqrjlzz.sHtML

now=$(date +%F); echo "$now"
来源：http://read.share.sjlbkw.cn/Article/details/gkblsebco.sHtML

[R27] 算术展开
来源：http://baike.vehdjk.com/Article/details/grfhgoygw.sHtML

echo $((1 + 2 * 3))
来源：http://m.share.fktsv.cn/Article/details/ghgpxvplq.sHtML

[R28] 浮点运算
来源：http://mobile.yfazqb.com/Article/details/gyenllbbg.sHtML

echo "scale=2; 10/3" | bc
来源：http://baike.fktsv.cn/Article/details/glibgyxkv.sHtML

[R29] 定义函数
来源：http://mobile.vehdjk.com/Article/details/gskkthrqd.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://read.share.tarul.cn/Article/details/gveuiholy.sHtML

[R30] 函数返回状态码
来源：http://www.blog.bbcook.cn/Article/details/gmvsxwgov.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://3g.yfazqb.com/Article/details/gfupbsktq.sHtML

[R31] 局部变量
来源：http://www.blog.vehdjk.com/Article/details/ggjpgetql.sHtML

f() { local x=1; echo "$x"; }
来源：http://blog.bbcook.cn/Article/details/gblabphtq.sHtML

[R32] 参数个数校验
来源：http://wap.tarul.cn/Article/details/gvtgzjoik.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://m.share.bbcook.cn/Article/details/gmjdympqw.sHtML

[R33] 捕获错误并提示行号
来源：http://baike.fktsv.cn/Article/details/gurugvaij.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://m.share.epnwcf.com/Article/details/gmhiupnlb.sHtML

[R34] 退出时清理
来源：http://read.share.sjlbkw.cn/Article/details/glaekyiei.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.tarul.cn/Article/details/gxrvslozp.sHtML

[R35] 后台执行并等待
来源：http://read.share.sjlbkw.cn/Article/details/gwloocpgo.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://mobile.tarul.cn/Article/details/gvnkqxexw.sHtML

[R36] 并发执行多个任务
来源：http://blog.epnwcf.com/Article/details/gniosdlqb.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://baike.epnwcf.com/Article/details/gqgdzbrva.sHtML

[R37] 把输出赋给变量
来源：http://baike.bbcook.cn/Article/details/gwxyyycvr.sHtML

files=$(ls -1)
来源：http://3g.fktsv.cn/Article/details/ghvdoazze.sHtML

[R38] 管道串联
来源：http://mobile.fktsv.cn/Article/details/gsdyqvyec.sHtML

cat a.txt | grep -i error | wc -l
来源：http://read.share.bbcook.cn/Article/details/gbabpvglm.sHtML

[R39] 重定向标准输出与错误
来源：http://www.m.share.sjlbkw.cn/Article/details/gudncjmbj.sHtML

cmd > out.log 2>&1
来源：http://www.m.share.tarul.cn/Article/details/gvyzupgao.sHtML

[R40] 追加写日志
来源：http://blog.yfazqb.com/Article/details/gztcdtlnf.sHtML

echo "log" >> out.log
来源：http://www.share.sjlbkw.cn/Article/details/gmwrdwrjo.sHtML

[R41] 丢弃输出
来源：http://m.share.yfazqb.com/Article/details/gvjllnuot.sHtML

cmd >/dev/null 2>&1
来源：http://wap.tarul.cn/Article/details/gxuzbdkqb.sHtML

[R42] 输入重定向
来源：http://wap.bbcook.cn/Article/details/gjecbmgad.sHtML

wc -l < a.txt
来源：http://blog.sjlbkw.cn/Article/details/girhixept.sHtML

[R43] 按名字查找文件
来源：http://m.share.sjlbkw.cn/Article/details/gztcetrsv.sHtML

find . -name "*.log" -type f
来源：http://m.share.bbcook.cn/Article/details/gukrxymyk.sHtML

[R44] 按修改时间查找
来源：http://read.share.epnwcf.com/Article/details/gbdzcfyek.sHtML

find . -mtime -7 -type f
来源：http://blog.yfazqb.com/Article/details/ggsimcqkn.sHtML

[R45] 批量删除
来源：http://3g.vehdjk.com/Article/details/glcdwwyfb.sHtML

find . -name "*.tmp" -delete
来源：http://m.share.vehdjk.com/Article/details/giqdvjyyd.sHtML

[R46] 递归替换文件内容
来源：http://baike.tarul.cn/Article/details/gsycuxpww.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.blog.bbcook.cn/Article/details/gypnyblwz.sHtML

[R47] sed 单行替换
来源：http://www.m.share.fktsv.cn/Article/details/gqctewega.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://blog.tarul.cn/Article/details/ghtzrayyd.sHtML

[R48] awk 取指定列
来源：http://m.share.sjlbkw.cn/Article/details/gxtbwwbne.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.blog.fktsv.cn/Article/details/grvplhtfv.sHtML

[R49] awk 带条件
来源：http://www.blog.sjlbkw.cn/Article/details/gflazuadb.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wap.bbcook.cn/Article/details/ghodbznyu.sHtML

[R50] awk 求和
来源：http://wap.sjlbkw.cn/Article/details/gurmrjlgi.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://read.share.vehdjk.com/Article/details/grwrlpsii.sHtML

[R51] 排序去重取前几
来源：http://www.blog.bbcook.cn/Article/details/gcystfijy.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.share.tarul.cn/Article/details/gafmohviy.sHtML

[R52] 统计行数
来源：http://m.share.bbcook.cn/Article/details/gzwqeqebw.sHtML

wc -l a.txt
来源：http://wap.vehdjk.com/Article/details/gfpnkbzrq.sHtML

[R53] 查看文件头与实时尾
来源：http://wap.sjlbkw.cn/Article/details/gubdipkca.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.share.epnwcf.com/Article/details/gyautudik.sHtML

[R54] 比较两个文件
来源：http://www.blog.bbcook.cn/Article/details/gbbbesozf.sHtML

diff a.txt b.txt
来源：http://www.blog.yfazqb.com/Article/details/gxjwpuepp.sHtML

[R55] 压缩与解压
来源：http://blog.bbcook.cn/Article/details/gcwkkwvet.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.share.tarul.cn/Article/details/gnacaioij.sHtML

[R56] 远程拷贝
来源：http://wap.epnwcf.com/Article/details/gchpiwnrp.sHtML

scp file user@host:/path/
来源：http://mobile.sjlbkw.cn/Article/details/gwkizwrjd.sHtML

[R57] 远程执行命令
来源：http://www.blog.bbcook.cn/Article/details/gkaoxzbwq.sHtML

ssh user@host 'uptime'
来源：http://www.share.sjlbkw.cn/Article/details/gldozcssf.sHtML

[R58] 下载文件
来源：http://www.blog.epnwcf.com/Article/details/gjlywmpgo.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://read.share.fktsv.cn/Article/details/gaiccakwd.sHtML

[R59] 发 POST JSON
来源：http://www.m.share.vehdjk.com/Article/details/ggzkjyeeg.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.share.yfazqb.com/Article/details/grkcdxkce.sHtML

[R60] 只看 HTTP 状态码
来源：http://wap.yfazqb.com/Article/details/gcazblojj.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mobile.vehdjk.com/Article/details/gzqfyajsy.sHtML

[R61] 磁盘占用
来源：http://3g.sjlbkw.cn/Article/details/gcuuefneb.sHtML

df -h;  du -sh *
来源：http://blog.sjlbkw.cn/Article/details/ggwuobyqp.sHtML

[R62] 找最占空间的文件
来源：http://wap.vehdjk.com/Article/details/gxogfcjac.sHtML

du -ah . | sort -rh | head -10
来源：http://mobile.bbcook.cn/Article/details/gwwxookcf.sHtML

[R63] 内存与进程
来源：http://www.blog.fktsv.cn/Article/details/ghkekkzmj.sHtML

free -h;  ps aux | grep nginx
来源：http://www.blog.yfazqb.com/Article/details/gowsvcnfn.sHtML

[R64] 结束进程
来源：http://www.blog.vehdjk.com/Article/details/gqwdmerjt.sHtML

kill -9 $(pgrep -f app.py)
来源：http://read.share.tarul.cn/Article/details/gicmemyqw.sHtML

[R65] 查看端口占用
来源：http://baike.fktsv.cn/Article/details/gmhszjxrb.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mobile.yfazqb.com/Article/details/gfmxofkvs.sHtML

[R66] 定时任务
来源：http://read.share.tarul.cn/Article/details/gqkhsnkya.sHtML

crontab -e;  crontab -l
来源：http://read.share.epnwcf.com/Article/details/gnofdgdke.sHtML

[R67] 生成随机十六进制串
来源：http://www.share.yfazqb.com/Article/details/gnqnqrtqy.sHtML

openssl rand -hex 16
来源：http://baike.sjlbkw.cn/Article/details/gpnlkbatt.sHtML

[R68] 计算文件校验值
来源：http://wap.bbcook.cn/Article/details/gwbskzobe.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://wap.bbcook.cn/Article/details/gprjshkpm.sHtML

[R69] 生成随机密码
来源：http://m.share.yfazqb.com/Article/details/ghmtuydda.sHtML

head -c 16 /dev/urandom | base64
来源：http://baike.tarul.cn/Article/details/gmfokuegh.sHtML

[R70] 时间戳与互转
来源：http://read.share.yfazqb.com/Article/details/gosnwmtmt.sHtML

date +%s;  date -d @1700000000
来源：http://3g.vehdjk.com/Article/details/gutkxayhb.sHtML

[R71] 日期格式化
来源：http://www.m.share.tarul.cn/Article/details/grzasqyup.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://baike.vehdjk.com/Article/details/gvjpcxppk.sHtML

[R72] 等待端口就绪
来源：http://blog.fktsv.cn/Article/details/ggcprdllj.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://3g.fktsv.cn/Article/details/gmzhjvpog.sHtML

[R73] 分割大日志
来源：http://www.share.sjlbkw.cn/Article/details/ggkstdocr.sHtML

split -l 1000 big.log part_
来源：http://baike.vehdjk.com/Article/details/gnmwujtqt.sHtML

[R74] 批量重命名
来源：http://baike.bbcook.cn/Article/details/gkldbszbr.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://wap.tarul.cn/Article/details/ghhtkzyym.sHtML

[R75] 导出环境变量
来源：http://wap.yfazqb.com/Article/details/gtfmobkku.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.m.share.epnwcf.com/Article/details/gubrwgbul.sHtML

[R76] 使用临时文件
来源：http://m.share.sjlbkw.cn/Article/details/ghcefqjgc.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://3g.epnwcf.com/Article/details/gyhrxfeke.sHtML

[R77] 读取用户输入
来源：http://www.blog.yfazqb.com/Article/details/gdobmwuat.sHtML

read -rp "请输入: " ans
来源：http://wap.epnwcf.com/Article/details/gpuxzeemf.sHtML

[R78] 交互式菜单
来源：http://read.share.tarul.cn/Article/details/gkqkxhsoy.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.share.bbcook.cn/Article/details/gbfujqujz.sHtML

[R79] 解析命令行选项
来源：http://wap.epnwcf.com/Article/details/grtgwwhzr.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://read.share.vehdjk.com/Article/details/ghxxjitpa.sHtML

[R80] 查看脚本执行耗时
来源：http://www.share.vehdjk.com/Article/details/gqjgxnwog.sHtML

time ./run.sh
来源：http://www.share.fktsv.cn/Article/details/gubhxlvtx.sHtML

================================================================================
来源：http://baike.sjlbkw.cn/Article/details/gofxyvgmm.sHtML

S. C / C++ 专题
来源：http://www.blog.vehdjk.com/Article/details/gzdatxtkf.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/gbmlpygol.sHtML

[S01] C：Hello World
来源：http://m.share.yfazqb.com/Article/details/gypkctpwz.sHtML

#include <stdio.h>
来源：http://www.m.share.yfazqb.com/Article/details/gnizqviib.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.blog.sjlbkw.cn/Article/details/gysoyotja.sHtML

[S02] C：变量与格式化输出
来源：http://read.share.epnwcf.com/Article/details/gqhpxpnib.sHtML

int a = 10; printf("%d\n", a);
来源：http://mobile.bbcook.cn/Article/details/guouaxkuq.sHtML

[S03] C：读入整数
来源：http://www.blog.bbcook.cn/Article/details/ggykmqeal.sHtML

int x; scanf("%d", &x);
来源：http://blog.sjlbkw.cn/Article/details/gcpymyzow.sHtML

[S04] C：字符串复制
来源：http://wap.yfazqb.com/Article/details/gglhcbnso.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.share.yfazqb.com/Article/details/gyksdwuzc.sHtML

[S05] C：字符串长度
来源：http://blog.epnwcf.com/Article/details/gbtqabhlu.sHtML

strlen(s)
来源：http://wap.sjlbkw.cn/Article/details/gkntbgzip.sHtML

[S06] C：字符串比较
来源：http://www.blog.sjlbkw.cn/Article/details/glyceyixj.sHtML

strcmp(a, b) == 0
来源：http://wap.bbcook.cn/Article/details/gpzcxsioa.sHtML

[S07] C：数组遍历求和
来源：http://m.share.fktsv.cn/Article/details/ghxbhunqt.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://baike.tarul.cn/Article/details/ghbikikcb.sHtML

[S08] C：动态内存分配与释放
来源：http://www.blog.tarul.cn/Article/details/gxoheyfcb.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://blog.vehdjk.com/Article/details/gzqrpdzzy.sHtML

[S09] C：结构体定义与初始化
来源：http://mobile.sjlbkw.cn/Article/details/gepworolr.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://read.share.epnwcf.com/Article/details/grpevqjll.sHtML

[S10] C：指针与解引用
来源：http://baike.tarul.cn/Article/details/gfmlcsagq.sHtML

int *p = &a;  *p = 5;
来源：http://m.share.vehdjk.com/Article/details/gyvcsrzoh.sHtML

[S11] C：逐行读文件
来源：http://baike.bbcook.cn/Article/details/gtsdkdpkq.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://wap.bbcook.cn/Article/details/gfqurtych.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://mobile.vehdjk.com/Article/details/gnancsmwk.sHtML

fclose(f);
来源：http://blog.vehdjk.com/Article/details/gkdqdgrjj.sHtML

[S12] C：写文件
来源：http://wap.yfazqb.com/Article/details/gkreaajeo.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://read.share.epnwcf.com/Article/details/gzxxhyfij.sHtML

[S13] C：宏定义
来源：http://baike.epnwcf.com/Article/details/gtnazhkoq.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://mobile.vehdjk.com/Article/details/gxfcznktj.sHtML

[S14] C：枚举
来源：http://www.m.share.epnwcf.com/Article/details/ghjzudqtr.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.blog.tarul.cn/Article/details/gwhfbfksq.sHtML

[S15] C：类型转换
来源：http://blog.epnwcf.com/Article/details/gcjbnhvza.sHtML

(double) a / b
来源：http://baike.bbcook.cn/Article/details/grbmdqvkv.sHtML

[S16] C：位操作置位
来源：http://www.blog.fktsv.cn/Article/details/gfsrmpkhr.sHtML

x |= (1 << 3);
来源：http://3g.vehdjk.com/Article/details/gmwnzwrse.sHtML

[S17] C：安全拼接字符串
来源：http://mobile.epnwcf.com/Article/details/gedavisqf.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wap.bbcook.cn/Article/details/gmcsvjjab.sHtML

[S18] C：命令行参数
来源：http://m.share.vehdjk.com/Article/details/gaatlevbu.sHtML

int main(int argc, char **argv)
来源：http://3g.tarul.cn/Article/details/gzkhkprvc.sHtML

[S19] C：快速排序
来源：http://3g.yfazqb.com/Article/details/grcoskwyw.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.m.share.sjlbkw.cn/Article/details/gkcubhicb.sHtML

[S20] C：二分查找
来源：http://www.share.yfazqb.com/Article/details/gigfsxkud.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://wap.fktsv.cn/Article/details/gxsnuharp.sHtML

[S21] C：字符类别判断
来源：http://wap.vehdjk.com/Article/details/ggdiqutiy.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://baike.tarul.cn/Article/details/gqkoclgdn.sHtML

[S22] C：字符串转数字
来源：http://3g.epnwcf.com/Article/details/gsbdncyeu.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.blog.tarul.cn/Article/details/glkcglfye.sHtML

[S23] C：随机数
来源：http://www.blog.vehdjk.com/Article/details/glqesxetv.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://mobile.bbcook.cn/Article/details/gruklalas.sHtML

[S24] C：获取本地时间
来源：http://3g.tarul.cn/Article/details/gfcozwzxb.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://read.share.epnwcf.com/Article/details/gljijfoyr.sHtML

[S25] C：内存拷贝
来源：http://blog.vehdjk.com/Article/details/gljbkvudf.sHtML

memcpy(dst, src, n);
来源：http://m.share.bbcook.cn/Article/details/gchngvbzz.sHtML

[S26] C：内存清零
来源：http://blog.epnwcf.com/Article/details/gempuwdcy.sHtML

memset(a, 0, sizeof a);
来源：http://wap.fktsv.cn/Article/details/gvimfsngv.sHtML

[S27] C：定义常量
来源：http://baike.tarul.cn/Article/details/gretkomsg.sHtML

const double PI = 3.14159;
来源：http://www.m.share.bbcook.cn/Article/details/ghqeubvje.sHtML

[S28] C：静态变量
来源：http://read.share.fktsv.cn/Article/details/gcncpbutu.sHtML

static int counter = 0;
来源：http://baike.bbcook.cn/Article/details/gznjjorbn.sHtML

[S29] C：变参函数
来源：http://m.share.fktsv.cn/Article/details/gnjjiiilt.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.blog.bbcook.cn/Article/details/gdxoqnjnq.sHtML

[S30] C：头文件保护
来源：http://3g.yfazqb.com/Article/details/gyevoxrwr.sHtML

#ifndef X_H
来源：http://baike.fktsv.cn/Article/details/glbdrciun.sHtML

#define X_H
来源：http://3g.fktsv.cn/Article/details/gzovqhuhn.sHtML

#endif
来源：http://www.m.share.fktsv.cn/Article/details/grtesuzak.sHtML

[S31] C++：Hello World
来源：http://baike.sjlbkw.cn/Article/details/gmwxcytkq.sHtML

#include <iostream>
来源：http://m.share.vehdjk.com/Article/details/gvywfhoqx.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://blog.tarul.cn/Article/details/gwwkvdqmb.sHtML

[S32] C++：字符串
来源：http://mobile.sjlbkw.cn/Article/details/gpyjmshkf.sHtML

std::string s = "hi";  s += "!";
来源：http://blog.yfazqb.com/Article/details/gigyoxcni.sHtML

[S33] C++：vector 增删
来源：http://www.share.tarul.cn/Article/details/grskrxzbq.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.blog.vehdjk.com/Article/details/gyztvovvw.sHtML

[S34] C++：遍历 vector
来源：http://www.m.share.fktsv.cn/Article/details/gbbjtdufo.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://3g.sjlbkw.cn/Article/details/gpnqpwnkd.sHtML

[S35] C++：map
来源：http://m.share.vehdjk.com/Article/details/givyhwkjb.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.epnwcf.com/Article/details/gydvmesxl.sHtML

[S36] C++：unordered_map
来源：http://www.m.share.bbcook.cn/Article/details/guofbibky.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wap.vehdjk.com/Article/details/gnlgndrxh.sHtML

[S37] C++：set
来源：http://baike.tarul.cn/Article/details/gqlxrgsec.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wap.vehdjk.com/Article/details/gljljcxtx.sHtML

[S38] C++：排序
来源：http://www.blog.fktsv.cn/Article/details/gcwzftfvd.sHtML

std::sort(v.begin(), v.end());
来源：http://blog.tarul.cn/Article/details/gdcypmmmx.sHtML

[S39] C++：自定义比较器排序
来源：http://mobile.sjlbkw.cn/Article/details/gxnuacvtd.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.blog.sjlbkw.cn/Article/details/gngxeoafc.sHtML

[S40] C++：查找元素
来源：http://blog.bbcook.cn/Article/details/goailfdkc.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://baike.tarul.cn/Article/details/giugndimy.sHtML

[S41] C++：类与构造函数
来源：http://m.share.fktsv.cn/Article/details/gdflruqwz.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://m.share.fktsv.cn/Article/details/ghipyqzja.sHtML

[S42] C++：继承与虚函数
来源：http://3g.bbcook.cn/Article/details/gllufkgyo.sHtML

class B : public Base { public: void f() override {} };
来源：http://read.share.vehdjk.com/Article/details/gvkinnsoj.sHtML

[S43] C++：智能指针
来源：http://read.share.epnwcf.com/Article/details/gtlzyuxnn.sHtML

auto p = std::make_unique<int>(5);
来源：http://mobile.vehdjk.com/Article/details/gzylurprx.sHtML

[S44] C++：引用传参
来源：http://www.share.sjlbkw.cn/Article/details/gabnrrmdm.sHtML

void inc(int &x) { ++x; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gpmcdhfpg.sHtML

[S45] C++：lambda
来源：http://wap.vehdjk.com/Article/details/gbzzracwq.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.share.epnwcf.com/Article/details/ggsyjqlzk.sHtML

[S46] C++：函数模板
来源：http://www.m.share.fktsv.cn/Article/details/gvcbbbkrr.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.blog.bbcook.cn/Article/details/gydvwtxzv.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.blog.epnwcf.com/Article/details/gkmaihlzn.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://blog.yfazqb.com/Article/details/gzbadkrea.sHtML

[S48] C++：逐行读文件
来源：http://www.m.share.fktsv.cn/Article/details/gzyffrijj.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.share.epnwcf.com/Article/details/gaihphqbg.sHtML

while (std::getline(in, line)) { }
来源：http://m.share.sjlbkw.cn/Article/details/gfpnpaynv.sHtML

[S49] C++：写文件
来源：http://mobile.sjlbkw.cn/Article/details/gqirkwofv.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://mobile.bbcook.cn/Article/details/gsmnywdpf.sHtML

[S50] C++：格式化数字
来源：http://www.m.share.bbcook.cn/Article/details/gsymestfs.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://read.share.vehdjk.com/Article/details/gwlosvldv.sHtML

[S51] C++：显式类型转换
来源：http://www.blog.vehdjk.com/Article/details/gewnfkusd.sHtML

static_cast<double>(a) / b
来源：http://m.share.fktsv.cn/Article/details/guawqrtik.sHtML

[S52] C++：const 与 noexcept
来源：http://mobile.sjlbkw.cn/Article/details/gstnxmdhs.sHtML

int size() const noexcept { return n_; }
来源：http://www.share.fktsv.cn/Article/details/gpwtonikt.sHtML

[S53] C++：移动语义
来源：http://www.blog.vehdjk.com/Article/details/gshiugxud.sHtML

std::vector<int> w = std::move(v);
来源：http://baike.tarul.cn/Article/details/gjrsxxpkn.sHtML

[S54] C++：异常处理
来源：http://www.blog.vehdjk.com/Article/details/guaynbdha.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://blog.bbcook.cn/Article/details/gcibgucaa.sHtML

[S55] C++：结构化绑定
来源：http://3g.vehdjk.com/Article/details/gqiulbwzh.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://m.share.sjlbkw.cn/Article/details/gdvdbwpnn.sHtML

[S56] C++：optional
来源：http://wap.fktsv.cn/Article/details/gugwznssg.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://read.share.fktsv.cn/Article/details/gwlfcitpn.sHtML

[S57] C++：编译期常量
来源：http://blog.vehdjk.com/Article/details/gwuevtxds.sHtML

constexpr int N = 10;
来源：http://3g.epnwcf.com/Article/details/gijrvrgif.sHtML

[S58] C++：命名空间
来源：http://www.share.vehdjk.com/Article/details/gybjimipn.sHtML

namespace ns { int f() { return 1; } }
来源：http://m.share.sjlbkw.cn/Article/details/guvgxkfwq.sHtML

[S59] C++：静态断言
来源：http://blog.sjlbkw.cn/Article/details/gvjlghuec.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.blog.tarul.cn/Article/details/gptxonavk.sHtML

[S60] C++：遍历并删除元素
来源：http://3g.sjlbkw.cn/Article/details/gbqcwntqw.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://m.share.tarul.cn/Article/details/gmopulwhs.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/gmcaoieqw.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://baike.tarul.cn/Article/details/gcriiifoj.sHtML

================================================================================
来源：http://mobile.yfazqb.com/Article/details/gufkovvhs.sHtML

[T01] Kotlin：Hello World
来源：http://baike.tarul.cn/Article/details/gwroblctm.sHtML

println("Hello")
来源：http://wap.yfazqb.com/Article/details/grncymxai.sHtML

[T02] Kotlin：变量
来源：http://blog.fktsv.cn/Article/details/gyikpiynd.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://baike.sjlbkw.cn/Article/details/gtkbkwref.sHtML

[T03] Kotlin：字符串模板
来源：http://m.share.epnwcf.com/Article/details/gwrqmrhor.sHtML

"值: $b"
来源：http://www.share.fktsv.cn/Article/details/gqloobmoh.sHtML

[T04] Kotlin：空安全
来源：http://www.m.share.yfazqb.com/Article/details/gvhwpanve.sHtML

val n: String? = null;  n?.length
来源：http://www.share.fktsv.cn/Article/details/ghbhsyete.sHtML

[T05] Kotlin：when 表达式
来源：http://blog.bbcook.cn/Article/details/gjshhzqym.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://read.share.epnwcf.com/Article/details/guqebppwj.sHtML

[T06] Kotlin：集合映射
来源：http://www.share.vehdjk.com/Article/details/gcsycsdyc.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://read.share.yfazqb.com/Article/details/gpkyrvjbb.sHtML

[T07] Kotlin：集合过滤
来源：http://wap.vehdjk.com/Article/details/gahsfient.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://mobile.bbcook.cn/Article/details/gocldlomi.sHtML

[T08] Kotlin：数据类
来源：http://www.share.sjlbkw.cn/Article/details/gjepzsauv.sHtML

data class User(val name: String, val age: Int)
来源：http://mobile.sjlbkw.cn/Article/details/gmyukmqqz.sHtML

[T09] Kotlin：扩展函数
来源：http://3g.tarul.cn/Article/details/gpqmpegwx.sHtML

fun String.exclaim() = this + "!"
来源：http://mobile.yfazqb.com/Article/details/glulegmsu.sHtML

[T10] Kotlin：默认参数
来源：http://blog.fktsv.cn/Article/details/gdzrnletq.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://m.share.bbcook.cn/Article/details/gfeqpntni.sHtML

[T11] Kotlin：协程
来源：http://blog.vehdjk.com/Article/details/guosdzwfu.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://baike.sjlbkw.cn/Article/details/gvslztnin.sHtML

[T12] Kotlin：解构声明
来源：http://wap.sjlbkw.cn/Article/details/geyvakoru.sHtML

val (a, b) = Pair(1, 2)
来源：http://mobile.epnwcf.com/Article/details/gttktzvds.sHtML

[T13] Kotlin：只读 Map
来源：http://www.blog.sjlbkw.cn/Article/details/gzsxaxakg.sHtML

val m = mapOf("a" to 1)
来源：http://mobile.yfazqb.com/Article/details/glswiceuj.sHtML

[T14] Kotlin：循环
来源：http://www.m.share.vehdjk.com/Article/details/ghrmuquqw.sHtML

for (i in 1..10) println(i)
来源：http://www.m.share.fktsv.cn/Article/details/gznkjxcoj.sHtML

[T15] Kotlin：接口
来源：http://wap.yfazqb.com/Article/details/gcnadyynq.sHtML

interface Shape { fun area(): Double }
来源：http://m.share.sjlbkw.cn/Article/details/gzctoioyl.sHtML

[T16] Swift：Hello World
来源：http://www.blog.bbcook.cn/Article/details/guqfqsnuz.sHtML

print("Hello")
来源：http://www.share.fktsv.cn/Article/details/gwgkgvrgj.sHtML

[T17] Swift：变量与常量
来源：http://m.share.bbcook.cn/Article/details/gcelooses.sHtML

var a = 1;  let b = 2
来源：http://read.share.vehdjk.com/Article/details/gehcvlikj.sHtML

[T18] Swift：字符串插值
来源：http://mobile.bbcook.cn/Article/details/grkulolpr.sHtML

"值: \(b)"
来源：http://www.blog.bbcook.cn/Article/details/gkhnfjodc.sHtML

[T19] Swift：可选绑定
来源：http://www.m.share.tarul.cn/Article/details/galupxigu.sHtML

if let n = opt { print(n) }
来源：http://www.share.epnwcf.com/Article/details/giudmqhiw.sHtML

[T20] Swift：数组操作
来源：http://read.share.yfazqb.com/Article/details/gruhxkewx.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://3g.epnwcf.com/Article/details/gujtmwfaw.sHtML

[T21] Swift：遍历
来源：http://wap.epnwcf.com/Article/details/gktaapqtc.sHtML

for x in a { print(x) }
来源：http://www.m.share.vehdjk.com/Article/details/gqxeqrzrd.sHtML

[T22] Swift：字典
来源：http://wap.bbcook.cn/Article/details/gissdcxfe.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://baike.tarul.cn/Article/details/gnsuvslcm.sHtML

[T23] Swift：函数
来源：http://www.m.share.bbcook.cn/Article/details/ggxuixdfi.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://wap.bbcook.cn/Article/details/gdqrfryhr.sHtML

[T24] Swift：闭包
来源：http://3g.sjlbkw.cn/Article/details/gucslrmkq.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://3g.vehdjk.com/Article/details/gmzrbydvr.sHtML


<!-- 参考信息 -->