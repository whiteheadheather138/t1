代发 wailian999

f() { local x=1; echo "$x"; }
来源：http://baike.vehdjk.com/Article/details/gafiplqag.sHtML

[R32] 参数个数校验
来源：http://www.blog.yfazqb.com/Article/details/gvzenenuu.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://baike.epnwcf.com/Article/details/guhnwsjhc.sHtML

[R33] 捕获错误并提示行号
来源：http://read.share.fktsv.cn/Article/details/gyqnyejoy.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://wap.fktsv.cn/Article/details/gxejesytb.sHtML

[R34] 退出时清理
来源：http://www.m.share.epnwcf.com/Article/details/gzutagoal.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://3g.tarul.cn/Article/details/ghfhqaezj.sHtML

[R35] 后台执行并等待
来源：http://www.m.share.bbcook.cn/Article/details/geqcqewee.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://baike.vehdjk.com/Article/details/gbzwvouuk.sHtML

[R36] 并发执行多个任务
来源：http://www.share.yfazqb.com/Article/details/geieexkyl.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.blog.fktsv.cn/Article/details/gbjitfnmo.sHtML

[R37] 把输出赋给变量
来源：http://read.share.bbcook.cn/Article/details/gdnugawui.sHtML

files=$(ls -1)
来源：http://www.blog.yfazqb.com/Article/details/gixngfsna.sHtML

[R38] 管道串联
来源：http://mobile.epnwcf.com/Article/details/gjyqfcqgn.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.blog.yfazqb.com/Article/details/gfspuqzzg.sHtML

[R39] 重定向标准输出与错误
来源：http://www.share.fktsv.cn/Article/details/gwvwaurqr.sHtML

cmd > out.log 2>&1
来源：http://m.share.epnwcf.com/Article/details/gtaawhbvz.sHtML

[R40] 追加写日志
来源：http://baike.sjlbkw.cn/Article/details/gdzrjeelw.sHtML

echo "log" >> out.log
来源：http://read.share.bbcook.cn/Article/details/ghyilztxj.sHtML

[R41] 丢弃输出
来源：http://m.share.fktsv.cn/Article/details/gixaewcgk.sHtML

cmd >/dev/null 2>&1
来源：http://blog.sjlbkw.cn/Article/details/guzyfxcfk.sHtML

[R42] 输入重定向
来源：http://www.blog.bbcook.cn/Article/details/gwgwxkskb.sHtML

wc -l < a.txt
来源：http://m.share.epnwcf.com/Article/details/goiobcfxd.sHtML

[R43] 按名字查找文件
来源：http://www.m.share.epnwcf.com/Article/details/ghuallopc.sHtML

find . -name "*.log" -type f
来源：http://3g.epnwcf.com/Article/details/gwaxehqzo.sHtML

[R44] 按修改时间查找
来源：http://www.blog.bbcook.cn/Article/details/ggnthabhc.sHtML

find . -mtime -7 -type f
来源：http://baike.sjlbkw.cn/Article/details/gargyisbn.sHtML

[R45] 批量删除
来源：http://www.blog.fktsv.cn/Article/details/ggbgyjubn.sHtML

find . -name "*.tmp" -delete
来源：http://www.share.yfazqb.com/Article/details/ggfycrcak.sHtML

[R46] 递归替换文件内容
来源：http://www.share.sjlbkw.cn/Article/details/gtmmtxcvq.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://blog.yfazqb.com/Article/details/gtwjhmleu.sHtML

[R47] sed 单行替换
来源：http://www.blog.fktsv.cn/Article/details/gneysyqxw.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.share.yfazqb.com/Article/details/gygladjfi.sHtML

[R48] awk 取指定列
来源：http://www.share.tarul.cn/Article/details/gslffgzwh.sHtML

awk '{print $1, $3}' a.txt
来源：http://read.share.fktsv.cn/Article/details/gvhidjngl.sHtML

[R49] awk 带条件
来源：http://baike.sjlbkw.cn/Article/details/gafesgdgv.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://blog.bbcook.cn/Article/details/gqmvzockj.sHtML

[R50] awk 求和
来源：http://blog.sjlbkw.cn/Article/details/gicwrpzqz.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.share.tarul.cn/Article/details/ggsgosraj.sHtML

[R51] 排序去重取前几
来源：http://blog.yfazqb.com/Article/details/gyunpgdfx.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://m.share.yfazqb.com/Article/details/gpshickub.sHtML

[R52] 统计行数
来源：http://read.share.fktsv.cn/Article/details/guosxdmmd.sHtML

wc -l a.txt
来源：http://wap.vehdjk.com/Article/details/gbxfxuubv.sHtML

[R53] 查看文件头与实时尾
来源：http://baike.tarul.cn/Article/details/ghdnstlrz.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://baike.fktsv.cn/Article/details/gflaztxvl.sHtML

[R54] 比较两个文件
来源：http://m.share.vehdjk.com/Article/details/gecifdcqp.sHtML

diff a.txt b.txt
来源：http://wap.bbcook.cn/Article/details/gxqebyjry.sHtML

[R55] 压缩与解压
来源：http://3g.yfazqb.com/Article/details/gaunndyhj.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://m.share.epnwcf.com/Article/details/ggdtyuwsq.sHtML

[R56] 远程拷贝
来源：http://baike.epnwcf.com/Article/details/getviqxwk.sHtML

scp file user@host:/path/
来源：http://3g.epnwcf.com/Article/details/gqfafvvge.sHtML

[R57] 远程执行命令
来源：http://www.m.share.sjlbkw.cn/Article/details/gwxkbjglh.sHtML

ssh user@host 'uptime'
来源：http://www.m.share.sjlbkw.cn/Article/details/gbezcmgth.sHtML

[R58] 下载文件
来源：http://read.share.tarul.cn/Article/details/gmlgqnowg.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://baike.epnwcf.com/Article/details/gseygtset.sHtML

[R59] 发 POST JSON
来源：http://read.share.fktsv.cn/Article/details/gothovzhk.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://mobile.vehdjk.com/Article/details/gcaghehmw.sHtML

[R60] 只看 HTTP 状态码
来源：http://blog.fktsv.cn/Article/details/gjppvazdq.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://baike.epnwcf.com/Article/details/gbyihalvb.sHtML

[R61] 磁盘占用
来源：http://www.blog.sjlbkw.cn/Article/details/grkajcrxv.sHtML

df -h;  du -sh *
来源：http://baike.fktsv.cn/Article/details/guxxpmclx.sHtML

[R62] 找最占空间的文件
来源：http://blog.vehdjk.com/Article/details/gprpucxzx.sHtML

du -ah . | sort -rh | head -10
来源：http://3g.sjlbkw.cn/Article/details/gclsukwms.sHtML

[R63] 内存与进程
来源：http://www.m.share.yfazqb.com/Article/details/gxtkakkxg.sHtML

free -h;  ps aux | grep nginx
来源：http://blog.tarul.cn/Article/details/gzepvocii.sHtML

[R64] 结束进程
来源：http://3g.vehdjk.com/Article/details/gejihaimq.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.m.share.tarul.cn/Article/details/gbhoybjuj.sHtML

[R65] 查看端口占用
来源：http://www.m.share.vehdjk.com/Article/details/gouscaazc.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://3g.vehdjk.com/Article/details/gajvqdulg.sHtML

[R66] 定时任务
来源：http://www.blog.fktsv.cn/Article/details/gzpowfmxx.sHtML

crontab -e;  crontab -l
来源：http://www.m.share.bbcook.cn/Article/details/gbjjeqknt.sHtML

[R67] 生成随机十六进制串
来源：http://www.blog.sjlbkw.cn/Article/details/gqtqhuqtc.sHtML

openssl rand -hex 16
来源：http://www.blog.tarul.cn/Article/details/gxlleqdmk.sHtML

[R68] 计算文件校验值
来源：http://mobile.fktsv.cn/Article/details/gmdvcwvsm.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.share.bbcook.cn/Article/details/gmcrvcrgb.sHtML

[R69] 生成随机密码
来源：http://read.share.epnwcf.com/Article/details/gmspzaxgy.sHtML

head -c 16 /dev/urandom | base64
来源：http://wap.epnwcf.com/Article/details/gkewynccd.sHtML

[R70] 时间戳与互转
来源：http://www.blog.vehdjk.com/Article/details/glgkvqiqu.sHtML

date +%s;  date -d @1700000000
来源：http://mobile.tarul.cn/Article/details/gozvnxoul.sHtML

[R71] 日期格式化
来源：http://mobile.fktsv.cn/Article/details/gzagwwxdw.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://mobile.tarul.cn/Article/details/gxzcwpdcm.sHtML

[R72] 等待端口就绪
来源：http://wap.yfazqb.com/Article/details/gazbylnws.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://mobile.epnwcf.com/Article/details/gsrhctjjg.sHtML

[R73] 分割大日志
来源：http://read.share.fktsv.cn/Article/details/ghcxpezvl.sHtML

split -l 1000 big.log part_
来源：http://m.share.tarul.cn/Article/details/gpnkkklid.sHtML

[R74] 批量重命名
来源：http://www.blog.vehdjk.com/Article/details/gcioztrgm.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.m.share.sjlbkw.cn/Article/details/gxirnlckt.sHtML

[R75] 导出环境变量
来源：http://3g.tarul.cn/Article/details/glqlpxuop.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.blog.bbcook.cn/Article/details/gzicxpsib.sHtML

[R76] 使用临时文件
来源：http://www.share.yfazqb.com/Article/details/gsmywolpv.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://wap.tarul.cn/Article/details/gxjxhmqww.sHtML

[R77] 读取用户输入
来源：http://3g.sjlbkw.cn/Article/details/gkkhrseye.sHtML

read -rp "请输入: " ans
来源：http://m.share.bbcook.cn/Article/details/grglouumw.sHtML

[R78] 交互式菜单
来源：http://baike.vehdjk.com/Article/details/gyrjurgxp.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://3g.bbcook.cn/Article/details/gxkgwvlvk.sHtML

[R79] 解析命令行选项
来源：http://3g.yfazqb.com/Article/details/gkovouzit.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.share.fktsv.cn/Article/details/gkbdzhmjr.sHtML

[R80] 查看脚本执行耗时
来源：http://www.blog.epnwcf.com/Article/details/gmgpwtmut.sHtML

time ./run.sh
来源：http://www.share.tarul.cn/Article/details/gappkpnsk.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/gxltwgunt.sHtML

S. C / C++ 专题
来源：http://wap.sjlbkw.cn/Article/details/gtmsdkbuq.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/gxzlmobai.sHtML

[S01] C：Hello World
来源：http://www.m.share.vehdjk.com/Article/details/gnnxzwjva.sHtML

#include <stdio.h>
来源：http://read.share.bbcook.cn/Article/details/ghbrwqyxc.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://wap.epnwcf.com/Article/details/gdlgvjzhi.sHtML

[S02] C：变量与格式化输出
来源：http://wap.bbcook.cn/Article/details/ggiarnugh.sHtML

int a = 10; printf("%d\n", a);
来源：http://read.share.sjlbkw.cn/Article/details/gvadwzimi.sHtML

[S03] C：读入整数
来源：http://blog.vehdjk.com/Article/details/gphlowuuv.sHtML

int x; scanf("%d", &x);
来源：http://mobile.sjlbkw.cn/Article/details/gvztrikhz.sHtML

[S04] C：字符串复制
来源：http://baike.fktsv.cn/Article/details/gwvpwnpqd.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.share.sjlbkw.cn/Article/details/grcelqfdi.sHtML

[S05] C：字符串长度
来源：http://read.share.yfazqb.com/Article/details/gsbqymafb.sHtML

strlen(s)
来源：http://3g.vehdjk.com/Article/details/golpqhfee.sHtML

[S06] C：字符串比较
来源：http://blog.sjlbkw.cn/Article/details/gdhiqgimo.sHtML

strcmp(a, b) == 0
来源：http://www.m.share.epnwcf.com/Article/details/gzkixilfa.sHtML

[S07] C：数组遍历求和
来源：http://read.share.bbcook.cn/Article/details/gxvtftgyf.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://baike.fktsv.cn/Article/details/gztrrrtqm.sHtML

[S08] C：动态内存分配与释放
来源：http://3g.tarul.cn/Article/details/griijwdil.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.blog.tarul.cn/Article/details/goexyruvu.sHtML

[S09] C：结构体定义与初始化
来源：http://read.share.vehdjk.com/Article/details/gissfjxim.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://wap.epnwcf.com/Article/details/gdqvsmsjf.sHtML

[S10] C：指针与解引用
来源：http://www.m.share.yfazqb.com/Article/details/gxemwqdrm.sHtML

int *p = &a;  *p = 5;
来源：http://blog.yfazqb.com/Article/details/gvzkgemfi.sHtML

[S11] C：逐行读文件
来源：http://blog.tarul.cn/Article/details/gyiyppczh.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.m.share.yfazqb.com/Article/details/gahzpcdwx.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://baike.fktsv.cn/Article/details/ggpjskhse.sHtML

fclose(f);
来源：http://read.share.vehdjk.com/Article/details/gfmkaeahc.sHtML

[S12] C：写文件
来源：http://3g.yfazqb.com/Article/details/gxdznubug.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://read.share.vehdjk.com/Article/details/ggrzkakks.sHtML

[S13] C：宏定义
来源：http://mobile.tarul.cn/Article/details/gyxqtcfkg.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.share.fktsv.cn/Article/details/gfqfolwxd.sHtML

[S14] C：枚举
来源：http://baike.vehdjk.com/Article/details/ghlczyrjn.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://baike.epnwcf.com/Article/details/gufiicddq.sHtML

[S15] C：类型转换
来源：http://www.m.share.yfazqb.com/Article/details/gtvnwetzj.sHtML

(double) a / b
来源：http://www.m.share.epnwcf.com/Article/details/gzelyuavk.sHtML

[S16] C：位操作置位
来源：http://mobile.tarul.cn/Article/details/gzqvamlnk.sHtML

x |= (1 << 3);
来源：http://read.share.epnwcf.com/Article/details/gykzfxokf.sHtML

[S17] C：安全拼接字符串
来源：http://3g.epnwcf.com/Article/details/gmezpkyls.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://blog.sjlbkw.cn/Article/details/gkywtfysw.sHtML

[S18] C：命令行参数
来源：http://blog.epnwcf.com/Article/details/gedemyksg.sHtML

int main(int argc, char **argv)
来源：http://blog.fktsv.cn/Article/details/glsqebggo.sHtML

[S19] C：快速排序
来源：http://www.share.tarul.cn/Article/details/gxsgrkwyf.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://wap.epnwcf.com/Article/details/gzjcksutd.sHtML

[S20] C：二分查找
来源：http://wap.fktsv.cn/Article/details/gcdnzgwss.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.m.share.sjlbkw.cn/Article/details/gdikuewmk.sHtML

[S21] C：字符类别判断
来源：http://3g.yfazqb.com/Article/details/gdijvgqje.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://blog.bbcook.cn/Article/details/gakgyckmx.sHtML

[S22] C：字符串转数字
来源：http://wap.tarul.cn/Article/details/gfwuvudni.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.m.share.epnwcf.com/Article/details/gabcgmojf.sHtML

[S23] C：随机数
来源：http://www.m.share.yfazqb.com/Article/details/gclfveyxz.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://blog.epnwcf.com/Article/details/gpjykqbht.sHtML

[S24] C：获取本地时间
来源：http://www.share.epnwcf.com/Article/details/gletldovr.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://read.share.fktsv.cn/Article/details/gjuntkaez.sHtML

[S25] C：内存拷贝
来源：http://3g.vehdjk.com/Article/details/geehyjyni.sHtML

memcpy(dst, src, n);
来源：http://www.m.share.sjlbkw.cn/Article/details/gitcgguzy.sHtML

[S26] C：内存清零
来源：http://wap.sjlbkw.cn/Article/details/gmzjqcroe.sHtML

memset(a, 0, sizeof a);
来源：http://www.m.share.bbcook.cn/Article/details/ghjgznmfe.sHtML

[S27] C：定义常量
来源：http://m.share.bbcook.cn/Article/details/gtdzsaics.sHtML

const double PI = 3.14159;
来源：http://mobile.fktsv.cn/Article/details/gvwcygrvv.sHtML

[S28] C：静态变量
来源：http://www.blog.fktsv.cn/Article/details/gffafyjom.sHtML

static int counter = 0;
来源：http://wap.tarul.cn/Article/details/gtxhdfzkr.sHtML

[S29] C：变参函数
来源：http://wap.tarul.cn/Article/details/gsyqmodci.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.blog.tarul.cn/Article/details/gttetirry.sHtML

[S30] C：头文件保护
来源：http://wap.fktsv.cn/Article/details/gvlopbdnf.sHtML

#ifndef X_H
来源：http://www.blog.vehdjk.com/Article/details/glbjmbqdn.sHtML

#define X_H
来源：http://blog.tarul.cn/Article/details/gtbzpjelr.sHtML

#endif
来源：http://m.share.bbcook.cn/Article/details/goirhkzaz.sHtML

[S31] C++：Hello World
来源：http://blog.tarul.cn/Article/details/ggofmvhme.sHtML

#include <iostream>
来源：http://read.share.sjlbkw.cn/Article/details/gkjvfpngs.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://blog.epnwcf.com/Article/details/goxkxwikw.sHtML

[S32] C++：字符串
来源：http://read.share.fktsv.cn/Article/details/gpoltjfbu.sHtML

std::string s = "hi";  s += "!";
来源：http://baike.epnwcf.com/Article/details/gmsnaukqy.sHtML

[S33] C++：vector 增删
来源：http://m.share.bbcook.cn/Article/details/gnzheaujy.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://baike.vehdjk.com/Article/details/ggyruvvvi.sHtML

[S34] C++：遍历 vector
来源：http://www.share.fktsv.cn/Article/details/givtaaeaa.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://blog.yfazqb.com/Article/details/ggwoiqiya.sHtML

[S35] C++：map
来源：http://www.share.yfazqb.com/Article/details/gpsjdxfed.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.fktsv.cn/Article/details/gmqllmpal.sHtML

[S36] C++：unordered_map
来源：http://blog.fktsv.cn/Article/details/guyhfohyl.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wap.fktsv.cn/Article/details/giqyisweu.sHtML

[S37] C++：set
来源：http://mobile.bbcook.cn/Article/details/gfoboecux.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://baike.vehdjk.com/Article/details/gchdjxgig.sHtML

[S38] C++：排序
来源：http://www.m.share.yfazqb.com/Article/details/guuvxlhys.sHtML

std::sort(v.begin(), v.end());
来源：http://mobile.fktsv.cn/Article/details/gpkvydxvi.sHtML

[S39] C++：自定义比较器排序
来源：http://read.share.vehdjk.com/Article/details/gznzbuped.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://m.share.fktsv.cn/Article/details/gbqczhyat.sHtML

[S40] C++：查找元素
来源：http://3g.tarul.cn/Article/details/gehnifdre.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://baike.epnwcf.com/Article/details/gsmgacnpz.sHtML

[S41] C++：类与构造函数
来源：http://www.m.share.vehdjk.com/Article/details/gkpbccclh.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://m.share.fktsv.cn/Article/details/gtxfxgfeh.sHtML

[S42] C++：继承与虚函数
来源：http://read.share.fktsv.cn/Article/details/gmwjvvvhp.sHtML

class B : public Base { public: void f() override {} };
来源：http://read.share.epnwcf.com/Article/details/gewbiuzhn.sHtML

[S43] C++：智能指针
来源：http://baike.yfazqb.com/Article/details/gluzzaqle.sHtML

auto p = std::make_unique<int>(5);
来源：http://mobile.bbcook.cn/Article/details/gcelovufa.sHtML

[S44] C++：引用传参
来源：http://3g.tarul.cn/Article/details/gnngmwhhm.sHtML

void inc(int &x) { ++x; }
来源：http://www.share.yfazqb.com/Article/details/gyersmwjg.sHtML

[S45] C++：lambda
来源：http://read.share.fktsv.cn/Article/details/gydekrndx.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.blog.epnwcf.com/Article/details/gizfswney.sHtML

[S46] C++：函数模板
来源：http://www.blog.bbcook.cn/Article/details/ggmaunepc.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://wap.fktsv.cn/Article/details/gsmuwzsjv.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.blog.yfazqb.com/Article/details/gefwtmbet.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.share.sjlbkw.cn/Article/details/gqhjpdgas.sHtML

[S48] C++：逐行读文件
来源：http://baike.yfazqb.com/Article/details/ggopmycca.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://3g.fktsv.cn/Article/details/gvgqqsfge.sHtML

while (std::getline(in, line)) { }
来源：http://wap.bbcook.cn/Article/details/gzckpwabw.sHtML

[S49] C++：写文件
来源：http://baike.fktsv.cn/Article/details/guvkezrua.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wap.bbcook.cn/Article/details/grbydexia.sHtML

[S50] C++：格式化数字
来源：http://www.m.share.vehdjk.com/Article/details/gvzctggjk.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://blog.vehdjk.com/Article/details/guavtogbq.sHtML

[S51] C++：显式类型转换
来源：http://baike.bbcook.cn/Article/details/gwtpnqued.sHtML

static_cast<double>(a) / b
来源：http://www.m.share.vehdjk.com/Article/details/galqicfgt.sHtML

[S52] C++：const 与 noexcept
来源：http://baike.vehdjk.com/Article/details/gftvcbhre.sHtML

int size() const noexcept { return n_; }
来源：http://wap.yfazqb.com/Article/details/gfdheulkb.sHtML

[S53] C++：移动语义
来源：http://blog.vehdjk.com/Article/details/ggdryznoy.sHtML

std::vector<int> w = std::move(v);
来源：http://wap.yfazqb.com/Article/details/gmnmuzjaj.sHtML

[S54] C++：异常处理
来源：http://baike.fktsv.cn/Article/details/gjosprahn.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.share.epnwcf.com/Article/details/gefxugvdr.sHtML

[S55] C++：结构化绑定
来源：http://mobile.tarul.cn/Article/details/gekxvruqo.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.share.sjlbkw.cn/Article/details/gamsaqdvb.sHtML

[S56] C++：optional
来源：http://read.share.bbcook.cn/Article/details/gbhjlpstr.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wap.sjlbkw.cn/Article/details/gldbtypgj.sHtML

[S57] C++：编译期常量
来源：http://wap.fktsv.cn/Article/details/glkbrkxtu.sHtML

constexpr int N = 10;
来源：http://wap.yfazqb.com/Article/details/glowkqfvz.sHtML

[S58] C++：命名空间
来源：http://www.blog.bbcook.cn/Article/details/gtskrvgmf.sHtML

namespace ns { int f() { return 1; } }
来源：http://wap.yfazqb.com/Article/details/gasshtlfr.sHtML

[S59] C++：静态断言
来源：http://www.blog.vehdjk.com/Article/details/gibxbefhu.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://blog.epnwcf.com/Article/details/gkxodmvaq.sHtML

[S60] C++：遍历并删除元素
来源：http://baike.yfazqb.com/Article/details/ggpuppnqh.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.share.bbcook.cn/Article/details/gqstlwlac.sHtML

================================================================================
来源：http://www.m.share.sjlbkw.cn/Article/details/gvmmdgnpd.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.sjlbkw.cn/Article/details/ghhodjvoq.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/gzrrzetyl.sHtML

[T01] Kotlin：Hello World
来源：http://www.blog.epnwcf.com/Article/details/ggwattynd.sHtML

println("Hello")
来源：http://www.m.share.sjlbkw.cn/Article/details/goygbhyeo.sHtML

[T02] Kotlin：变量
来源：http://3g.vehdjk.com/Article/details/gmhkrkflc.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://mobile.epnwcf.com/Article/details/gllnkdlze.sHtML

[T03] Kotlin：字符串模板
来源：http://www.m.share.yfazqb.com/Article/details/gnkjbeqtz.sHtML

"值: $b"
来源：http://www.m.share.yfazqb.com/Article/details/gmlvqqfor.sHtML

[T04] Kotlin：空安全
来源：http://wap.tarul.cn/Article/details/gtkpbmsiz.sHtML

val n: String? = null;  n?.length
来源：http://read.share.sjlbkw.cn/Article/details/gsphidzdg.sHtML

[T05] Kotlin：when 表达式
来源：http://wap.vehdjk.com/Article/details/grjpyvrfl.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.share.vehdjk.com/Article/details/grvqatwuw.sHtML

[T06] Kotlin：集合映射
来源：http://www.m.share.sjlbkw.cn/Article/details/gheluyiqq.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://blog.fktsv.cn/Article/details/gprvibdmj.sHtML

[T07] Kotlin：集合过滤
来源：http://www.share.epnwcf.com/Article/details/geczyapgi.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://blog.tarul.cn/Article/details/gonoaseqk.sHtML

[T08] Kotlin：数据类
来源：http://read.share.yfazqb.com/Article/details/gtdvkivbu.sHtML

data class User(val name: String, val age: Int)
来源：http://www.m.share.epnwcf.com/Article/details/gsumwnaqg.sHtML

[T09] Kotlin：扩展函数
来源：http://3g.fktsv.cn/Article/details/glaxwgqas.sHtML

fun String.exclaim() = this + "!"
来源：http://www.m.share.bbcook.cn/Article/details/gbglkvzhb.sHtML

[T10] Kotlin：默认参数
来源：http://wap.fktsv.cn/Article/details/gcwnbgcto.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://read.share.yfazqb.com/Article/details/glguqcsho.sHtML

[T11] Kotlin：协程
来源：http://3g.sjlbkw.cn/Article/details/gkqlrwzug.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://wap.yfazqb.com/Article/details/gtjvsuvis.sHtML

[T12] Kotlin：解构声明
来源：http://mobile.vehdjk.com/Article/details/gdekwrdcm.sHtML

val (a, b) = Pair(1, 2)
来源：http://read.share.epnwcf.com/Article/details/gnowsqtfy.sHtML

[T13] Kotlin：只读 Map
来源：http://www.m.share.yfazqb.com/Article/details/gjimuprth.sHtML

val m = mapOf("a" to 1)
来源：http://wap.sjlbkw.cn/Article/details/griithrsb.sHtML

[T14] Kotlin：循环
来源：http://www.m.share.yfazqb.com/Article/details/glfpwnvuq.sHtML

for (i in 1..10) println(i)
来源：http://3g.tarul.cn/Article/details/gmpvvgvpg.sHtML

[T15] Kotlin：接口
来源：http://www.blog.tarul.cn/Article/details/gzfkimzuf.sHtML

interface Shape { fun area(): Double }
来源：http://wap.tarul.cn/Article/details/gpavuiuqy.sHtML

[T16] Swift：Hello World
来源：http://www.share.fktsv.cn/Article/details/gihyaucgq.sHtML

print("Hello")
来源：http://www.blog.yfazqb.com/Article/details/ggoludvcm.sHtML

[T17] Swift：变量与常量
来源：http://read.share.yfazqb.com/Article/details/gpjpclslq.sHtML

var a = 1;  let b = 2
来源：http://blog.bbcook.cn/Article/details/gpbsuolrx.sHtML

[T18] Swift：字符串插值
来源：http://3g.sjlbkw.cn/Article/details/giihpuubr.sHtML

"值: \(b)"
来源：http://www.share.bbcook.cn/Article/details/grrlmgcal.sHtML

[T19] Swift：可选绑定
来源：http://read.share.fktsv.cn/Article/details/gaonqldva.sHtML

if let n = opt { print(n) }
来源：http://www.m.share.tarul.cn/Article/details/gwawlcxux.sHtML

[T20] Swift：数组操作
来源：http://m.share.vehdjk.com/Article/details/gntlwrgtn.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://3g.sjlbkw.cn/Article/details/gdhesajjl.sHtML

[T21] Swift：遍历
来源：http://read.share.sjlbkw.cn/Article/details/gkvtkwksz.sHtML

for x in a { print(x) }
来源：http://baike.vehdjk.com/Article/details/gqjfifpyp.sHtML

[T22] Swift：字典
来源：http://3g.bbcook.cn/Article/details/gurzygwlg.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://m.share.epnwcf.com/Article/details/gopmjayau.sHtML

[T23] Swift：函数
来源：http://baike.tarul.cn/Article/details/gdklcxfjh.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://blog.yfazqb.com/Article/details/gyjduudji.sHtML

[T24] Swift：闭包
来源：http://3g.tarul.cn/Article/details/gamiphhba.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://baike.vehdjk.com/Article/details/ghextgflp.sHtML

[T25] Swift：结构体
来源：http://m.share.yfazqb.com/Article/details/gpqrutmyu.sHtML

struct P { var x: Int }
来源：http://m.share.yfazqb.com/Article/details/geqxtbeub.sHtML

[T26] Swift：类与重写
来源：http://www.blog.bbcook.cn/Article/details/grnejliiq.sHtML

class A: Base { override func f() {} }
来源：http://www.blog.tarul.cn/Article/details/gqexsygxu.sHtML

[T27] Swift：错误处理
来源：http://blog.yfazqb.com/Article/details/ghfeylevu.sHtML

do { try f() } catch { print(error) }
来源：http://www.m.share.sjlbkw.cn/Article/details/gscyfthhp.sHtML

[T28] Swift：枚举
来源：http://www.blog.tarul.cn/Article/details/gcxwuodhk.sHtML

enum Color { case red, green }
来源：http://blog.vehdjk.com/Article/details/gapqzydbk.sHtML

[T29] Swift：guard 提前返回
来源：http://m.share.sjlbkw.cn/Article/details/gqfiappvu.sHtML

guard let x = opt else { return }
来源：http://www.share.sjlbkw.cn/Article/details/gvwmawfbq.sHtML

[T30] Swift：协议
来源：http://blog.tarul.cn/Article/details/gahyvvibe.sHtML

protocol Shape { func area() -> Double }
来源：http://read.share.epnwcf.com/Article/details/gotrtiohc.sHtML

[T31] Lua：Hello World
来源：http://m.share.vehdjk.com/Article/details/gkxwwxccq.sHtML

print("Hello")
来源：http://www.blog.fktsv.cn/Article/details/gmcqungje.sHtML

[T32] Lua：局部变量
来源：http://blog.vehdjk.com/Article/details/gkbbttpyb.sHtML

local a = 1
来源：http://www.share.tarul.cn/Article/details/gbcyhklub.sHtML

[T33] Lua：表（数组）
来源：http://read.share.yfazqb.com/Article/details/godgmcinm.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://blog.tarul.cn/Article/details/gveelunsn.sHtML

[T34] Lua：遍历表
来源：http://www.blog.sjlbkw.cn/Article/details/gfkjpbwci.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://3g.fktsv.cn/Article/details/grbsnfnzb.sHtML


<!-- 参考信息 -->