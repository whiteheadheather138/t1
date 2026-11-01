代发 wailian999

add() { echo $(($1 + $2)); }; add 1 2
来源：http://3g.yfazqb.com/Article/details/grawvveln.sHtML

[R30] 函数返回状态码
来源：http://blog.tarul.cn/Article/details/ggselqnyo.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.blog.bbcook.cn/Article/details/gloephlht.sHtML

[R31] 局部变量
来源：http://www.blog.epnwcf.com/Article/details/gghacaahh.sHtML

f() { local x=1; echo "$x"; }
来源：http://baike.vehdjk.com/Article/details/gmfmnqfey.sHtML

[R32] 参数个数校验
来源：http://3g.bbcook.cn/Article/details/gpvyhidwn.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://blog.bbcook.cn/Article/details/gxjafqqjw.sHtML

[R33] 捕获错误并提示行号
来源：http://mobile.vehdjk.com/Article/details/gzdkhohiq.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://baike.vehdjk.com/Article/details/gvrehvzwi.sHtML

[R34] 退出时清理
来源：http://3g.bbcook.cn/Article/details/gfrfrjmtj.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.tarul.cn/Article/details/gjoepabvi.sHtML

[R35] 后台执行并等待
来源：http://www.m.share.epnwcf.com/Article/details/gynepiuvq.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.m.share.bbcook.cn/Article/details/gofhkgbwk.sHtML

[R36] 并发执行多个任务
来源：http://blog.sjlbkw.cn/Article/details/gijxazfov.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://baike.epnwcf.com/Article/details/ggjjjvjxh.sHtML

[R37] 把输出赋给变量
来源：http://3g.fktsv.cn/Article/details/gpulugpdw.sHtML

files=$(ls -1)
来源：http://baike.vehdjk.com/Article/details/giayridpc.sHtML

[R38] 管道串联
来源：http://www.m.share.vehdjk.com/Article/details/guzubqslk.sHtML

cat a.txt | grep -i error | wc -l
来源：http://m.share.bbcook.cn/Article/details/gnpmbvfue.sHtML

[R39] 重定向标准输出与错误
来源：http://mobile.tarul.cn/Article/details/gvmfoodnk.sHtML

cmd > out.log 2>&1
来源：http://www.m.share.tarul.cn/Article/details/gjgfktnhk.sHtML

[R40] 追加写日志
来源：http://www.share.yfazqb.com/Article/details/gcibsixvx.sHtML

echo "log" >> out.log
来源：http://baike.bbcook.cn/Article/details/gudjmymsc.sHtML

[R41] 丢弃输出
来源：http://www.blog.epnwcf.com/Article/details/gblelwiea.sHtML

cmd >/dev/null 2>&1
来源：http://wap.epnwcf.com/Article/details/gvfooxopz.sHtML

[R42] 输入重定向
来源：http://www.blog.yfazqb.com/Article/details/ggyitqbkb.sHtML

wc -l < a.txt
来源：http://wap.bbcook.cn/Article/details/gzriaibxq.sHtML

[R43] 按名字查找文件
来源：http://3g.epnwcf.com/Article/details/gigqmcepz.sHtML

find . -name "*.log" -type f
来源：http://m.share.fktsv.cn/Article/details/gefaegfjz.sHtML

[R44] 按修改时间查找
来源：http://m.share.sjlbkw.cn/Article/details/gvthafhqy.sHtML

find . -mtime -7 -type f
来源：http://3g.bbcook.cn/Article/details/gfrlnqjlp.sHtML

[R45] 批量删除
来源：http://wap.yfazqb.com/Article/details/gyftyuplw.sHtML

find . -name "*.tmp" -delete
来源：http://www.m.share.fktsv.cn/Article/details/gyxtmjjpe.sHtML

[R46] 递归替换文件内容
来源：http://www.share.bbcook.cn/Article/details/gmowasygg.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://read.share.sjlbkw.cn/Article/details/gyrukapbz.sHtML

[R47] sed 单行替换
来源：http://www.m.share.sjlbkw.cn/Article/details/gtxzsutaz.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.blog.tarul.cn/Article/details/gioqcjrlw.sHtML

[R48] awk 取指定列
来源：http://wap.fktsv.cn/Article/details/gkotudwty.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.blog.tarul.cn/Article/details/gplqindyr.sHtML

[R49] awk 带条件
来源：http://mobile.sjlbkw.cn/Article/details/gxqtexrmx.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.blog.epnwcf.com/Article/details/giryujrte.sHtML

[R50] awk 求和
来源：http://blog.bbcook.cn/Article/details/gwbgnkiwc.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://wap.tarul.cn/Article/details/gfuosxklb.sHtML

[R51] 排序去重取前几
来源：http://read.share.vehdjk.com/Article/details/guszjpsci.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://mobile.yfazqb.com/Article/details/gojloclrb.sHtML

[R52] 统计行数
来源：http://blog.tarul.cn/Article/details/gzjwcdccm.sHtML

wc -l a.txt
来源：http://www.blog.epnwcf.com/Article/details/ggxojtali.sHtML

[R53] 查看文件头与实时尾
来源：http://read.share.vehdjk.com/Article/details/gqwzoaenc.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.blog.epnwcf.com/Article/details/gkalxssfd.sHtML

[R54] 比较两个文件
来源：http://mobile.vehdjk.com/Article/details/gqknduocu.sHtML

diff a.txt b.txt
来源：http://blog.epnwcf.com/Article/details/gjwiyywoe.sHtML

[R55] 压缩与解压
来源：http://blog.fktsv.cn/Article/details/gqhqevrfl.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://read.share.fktsv.cn/Article/details/gefxvangv.sHtML

[R56] 远程拷贝
来源：http://blog.fktsv.cn/Article/details/giictssmc.sHtML

scp file user@host:/path/
来源：http://www.m.share.tarul.cn/Article/details/gsdfvmttc.sHtML

[R57] 远程执行命令
来源：http://3g.bbcook.cn/Article/details/gyrtxsmeq.sHtML

ssh user@host 'uptime'
来源：http://wap.yfazqb.com/Article/details/gctdjnrue.sHtML

[R58] 下载文件
来源：http://blog.sjlbkw.cn/Article/details/gbtbbarxa.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.share.yfazqb.com/Article/details/gncmmdyox.sHtML

[R59] 发 POST JSON
来源：http://mobile.fktsv.cn/Article/details/gzcwkotle.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://baike.fktsv.cn/Article/details/ghufferzu.sHtML

[R60] 只看 HTTP 状态码
来源：http://3g.vehdjk.com/Article/details/gumbnowoz.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mobile.bbcook.cn/Article/details/gwdmkwdxn.sHtML

[R61] 磁盘占用
来源：http://read.share.tarul.cn/Article/details/gawfwavpl.sHtML

df -h;  du -sh *
来源：http://m.share.bbcook.cn/Article/details/gozbnszhn.sHtML

[R62] 找最占空间的文件
来源：http://baike.tarul.cn/Article/details/gbxejwhbg.sHtML

du -ah . | sort -rh | head -10
来源：http://mobile.fktsv.cn/Article/details/gftxiubjv.sHtML

[R63] 内存与进程
来源：http://wap.epnwcf.com/Article/details/gsodqqleb.sHtML

free -h;  ps aux | grep nginx
来源：http://mobile.epnwcf.com/Article/details/guadkauca.sHtML

[R64] 结束进程
来源：http://3g.fktsv.cn/Article/details/gdtgeusmz.sHtML

kill -9 $(pgrep -f app.py)
来源：http://blog.sjlbkw.cn/Article/details/gcdtsuvbf.sHtML

[R65] 查看端口占用
来源：http://3g.epnwcf.com/Article/details/grxkysnwa.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://3g.bbcook.cn/Article/details/gjbssfyoh.sHtML

[R66] 定时任务
来源：http://www.m.share.yfazqb.com/Article/details/glvhhgvtx.sHtML

crontab -e;  crontab -l
来源：http://read.share.sjlbkw.cn/Article/details/gbzqzmmgc.sHtML

[R67] 生成随机十六进制串
来源：http://blog.sjlbkw.cn/Article/details/gnsftpdic.sHtML

openssl rand -hex 16
来源：http://www.m.share.tarul.cn/Article/details/gxrxhsias.sHtML

[R68] 计算文件校验值
来源：http://www.m.share.vehdjk.com/Article/details/gxsotigey.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://blog.bbcook.cn/Article/details/guinqajek.sHtML

[R69] 生成随机密码
来源：http://mobile.vehdjk.com/Article/details/gconduiyl.sHtML

head -c 16 /dev/urandom | base64
来源：http://wap.tarul.cn/Article/details/gcpbscktw.sHtML

[R70] 时间戳与互转
来源：http://read.share.fktsv.cn/Article/details/gtptqgity.sHtML

date +%s;  date -d @1700000000
来源：http://wap.sjlbkw.cn/Article/details/gccfpnukp.sHtML

[R71] 日期格式化
来源：http://mobile.bbcook.cn/Article/details/gwdxzsblw.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://wap.tarul.cn/Article/details/gvwyzjnqk.sHtML

[R72] 等待端口就绪
来源：http://www.m.share.epnwcf.com/Article/details/gjojwmsby.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://wap.bbcook.cn/Article/details/gicnygyjh.sHtML

[R73] 分割大日志
来源：http://www.share.bbcook.cn/Article/details/gjxbypmtw.sHtML

split -l 1000 big.log part_
来源：http://wap.bbcook.cn/Article/details/giikalray.sHtML

[R74] 批量重命名
来源：http://www.m.share.sjlbkw.cn/Article/details/giqdabeug.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://mobile.tarul.cn/Article/details/gtkqppnrs.sHtML

[R75] 导出环境变量
来源：http://read.share.epnwcf.com/Article/details/gysfgkine.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://blog.fktsv.cn/Article/details/gpnuuxbjr.sHtML

[R76] 使用临时文件
来源：http://www.share.vehdjk.com/Article/details/gwmzydibw.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://read.share.tarul.cn/Article/details/gemxvxqes.sHtML

[R77] 读取用户输入
来源：http://m.share.tarul.cn/Article/details/gjaeqznyx.sHtML

read -rp "请输入: " ans
来源：http://3g.tarul.cn/Article/details/grcxfkkcx.sHtML

[R78] 交互式菜单
来源：http://www.blog.fktsv.cn/Article/details/goevmdgkv.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://read.share.bbcook.cn/Article/details/glvxhzneu.sHtML

[R79] 解析命令行选项
来源：http://blog.bbcook.cn/Article/details/gcmnhkahb.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.share.epnwcf.com/Article/details/gccuomcgo.sHtML

[R80] 查看脚本执行耗时
来源：http://www.share.tarul.cn/Article/details/ghnfcinbm.sHtML

time ./run.sh
来源：http://blog.tarul.cn/Article/details/ggbohythx.sHtML

================================================================================
来源：http://baike.sjlbkw.cn/Article/details/gzqukagvy.sHtML

S. C / C++ 专题
来源：http://mobile.epnwcf.com/Article/details/gncjqusxb.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/gfdvfdrcw.sHtML

[S01] C：Hello World
来源：http://baike.fktsv.cn/Article/details/gikxfqegw.sHtML

#include <stdio.h>
来源：http://3g.sjlbkw.cn/Article/details/gfmielwai.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://3g.epnwcf.com/Article/details/genxsjkxu.sHtML

[S02] C：变量与格式化输出
来源：http://baike.yfazqb.com/Article/details/gnwxrjjlm.sHtML

int a = 10; printf("%d\n", a);
来源：http://read.share.bbcook.cn/Article/details/gamprhrce.sHtML

[S03] C：读入整数
来源：http://mobile.bbcook.cn/Article/details/gzcqlnrhv.sHtML

int x; scanf("%d", &x);
来源：http://www.share.yfazqb.com/Article/details/gqjqustrp.sHtML

[S04] C：字符串复制
来源：http://www.share.tarul.cn/Article/details/glncqluct.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.share.sjlbkw.cn/Article/details/gjtskxchk.sHtML

[S05] C：字符串长度
来源：http://www.share.sjlbkw.cn/Article/details/gigezbfys.sHtML

strlen(s)
来源：http://mobile.vehdjk.com/Article/details/gdufpnxoi.sHtML

[S06] C：字符串比较
来源：http://m.share.vehdjk.com/Article/details/gjiuuxylb.sHtML

strcmp(a, b) == 0
来源：http://www.m.share.fktsv.cn/Article/details/gsjvpxcsq.sHtML

[S07] C：数组遍历求和
来源：http://mobile.vehdjk.com/Article/details/gnfwthxsg.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://mobile.sjlbkw.cn/Article/details/gjbjlyzmy.sHtML

[S08] C：动态内存分配与释放
来源：http://mobile.vehdjk.com/Article/details/grkaslkww.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mobile.epnwcf.com/Article/details/gvdtprxsg.sHtML

[S09] C：结构体定义与初始化
来源：http://wap.sjlbkw.cn/Article/details/gchmhcgom.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://baike.bbcook.cn/Article/details/gaclvwxyc.sHtML

[S10] C：指针与解引用
来源：http://mobile.tarul.cn/Article/details/ggaecrzrm.sHtML

int *p = &a;  *p = 5;
来源：http://www.m.share.fktsv.cn/Article/details/gplvizoxv.sHtML

[S11] C：逐行读文件
来源：http://wap.vehdjk.com/Article/details/gmeherfmx.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://blog.epnwcf.com/Article/details/gecarilvi.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.m.share.bbcook.cn/Article/details/gcepwszwy.sHtML

fclose(f);
来源：http://blog.epnwcf.com/Article/details/gcgulnvau.sHtML

[S12] C：写文件
来源：http://wap.yfazqb.com/Article/details/gveyealbb.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://blog.vehdjk.com/Article/details/gcnbveklm.sHtML

[S13] C：宏定义
来源：http://www.m.share.tarul.cn/Article/details/gftvpsalq.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.m.share.tarul.cn/Article/details/gwiusqvnr.sHtML

[S14] C：枚举
来源：http://www.share.tarul.cn/Article/details/geyseujpu.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.m.share.tarul.cn/Article/details/gmuvzgkbw.sHtML

[S15] C：类型转换
来源：http://baike.sjlbkw.cn/Article/details/gzbcihjdf.sHtML

(double) a / b
来源：http://read.share.yfazqb.com/Article/details/gjkyuxllo.sHtML

[S16] C：位操作置位
来源：http://read.share.bbcook.cn/Article/details/gqjkuaugu.sHtML

x |= (1 << 3);
来源：http://blog.bbcook.cn/Article/details/gimiqxfrc.sHtML

[S17] C：安全拼接字符串
来源：http://blog.epnwcf.com/Article/details/gynvwqunh.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.m.share.tarul.cn/Article/details/gjnkajzxi.sHtML

[S18] C：命令行参数
来源：http://3g.tarul.cn/Article/details/gpjmylmuy.sHtML

int main(int argc, char **argv)
来源：http://www.blog.vehdjk.com/Article/details/gsieayaub.sHtML

[S19] C：快速排序
来源：http://baike.sjlbkw.cn/Article/details/ghxkfddce.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.m.share.tarul.cn/Article/details/gwvvzohcr.sHtML

[S20] C：二分查找
来源：http://www.share.yfazqb.com/Article/details/gnjsescka.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://read.share.vehdjk.com/Article/details/gbsushbxx.sHtML

[S21] C：字符类别判断
来源：http://www.blog.yfazqb.com/Article/details/ggogmaydo.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://m.share.tarul.cn/Article/details/gybuwcwdf.sHtML

[S22] C：字符串转数字
来源：http://m.share.bbcook.cn/Article/details/gazbxgvcc.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.blog.epnwcf.com/Article/details/glmvbbocn.sHtML

[S23] C：随机数
来源：http://m.share.epnwcf.com/Article/details/gslqzcnga.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://mobile.tarul.cn/Article/details/gierilheb.sHtML

[S24] C：获取本地时间
来源：http://read.share.sjlbkw.cn/Article/details/gpuodwyak.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.m.share.vehdjk.com/Article/details/gtejgfkew.sHtML

[S25] C：内存拷贝
来源：http://wap.vehdjk.com/Article/details/gpspwixvg.sHtML

memcpy(dst, src, n);
来源：http://mobile.sjlbkw.cn/Article/details/gnuoysseu.sHtML

[S26] C：内存清零
来源：http://3g.tarul.cn/Article/details/grikwrvjc.sHtML

memset(a, 0, sizeof a);
来源：http://m.share.epnwcf.com/Article/details/gapblrfzo.sHtML

[S27] C：定义常量
来源：http://www.share.epnwcf.com/Article/details/gbgiwrfrd.sHtML

const double PI = 3.14159;
来源：http://wap.yfazqb.com/Article/details/gumombfdb.sHtML

[S28] C：静态变量
来源：http://read.share.yfazqb.com/Article/details/gjnjlxket.sHtML

static int counter = 0;
来源：http://www.share.bbcook.cn/Article/details/gmrsnknpl.sHtML

[S29] C：变参函数
来源：http://wap.vehdjk.com/Article/details/gdkhqvddg.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.share.yfazqb.com/Article/details/grfvhiixy.sHtML

[S30] C：头文件保护
来源：http://blog.epnwcf.com/Article/details/gpprlfhso.sHtML

#ifndef X_H
来源：http://read.share.tarul.cn/Article/details/gvbrkvlvr.sHtML

#define X_H
来源：http://www.share.epnwcf.com/Article/details/gvkcofpbk.sHtML

#endif
来源：http://wap.sjlbkw.cn/Article/details/gwfgdbvnl.sHtML

[S31] C++：Hello World
来源：http://www.share.yfazqb.com/Article/details/gqkkimjho.sHtML

#include <iostream>
来源：http://wap.fktsv.cn/Article/details/gtbxqhjdk.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://read.share.vehdjk.com/Article/details/gbavpcwob.sHtML

[S32] C++：字符串
来源：http://mobile.sjlbkw.cn/Article/details/gcsavlbfp.sHtML

std::string s = "hi";  s += "!";
来源：http://www.share.epnwcf.com/Article/details/gdgeneemc.sHtML

[S33] C++：vector 增删
来源：http://baike.tarul.cn/Article/details/gwjmzhwlm.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://read.share.tarul.cn/Article/details/glpxzvjcp.sHtML

[S34] C++：遍历 vector
来源：http://blog.fktsv.cn/Article/details/gnwsyfutn.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://m.share.bbcook.cn/Article/details/getlzihpv.sHtML

[S35] C++：map
来源：http://www.m.share.epnwcf.com/Article/details/gnuunrvoa.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.fktsv.cn/Article/details/gjxgvimxv.sHtML

[S36] C++：unordered_map
来源：http://baike.sjlbkw.cn/Article/details/gpmjkzglp.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.sjlbkw.cn/Article/details/gzqmhsvke.sHtML

[S37] C++：set
来源：http://wap.sjlbkw.cn/Article/details/gpwfiypwe.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.share.sjlbkw.cn/Article/details/govnbdkls.sHtML

[S38] C++：排序
来源：http://www.m.share.yfazqb.com/Article/details/gnoqrfubg.sHtML

std::sort(v.begin(), v.end());
来源：http://www.m.share.yfazqb.com/Article/details/gkapqtoza.sHtML

[S39] C++：自定义比较器排序
来源：http://www.blog.epnwcf.com/Article/details/ghcxhiucl.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://3g.bbcook.cn/Article/details/ghsxhsunu.sHtML

[S40] C++：查找元素
来源：http://www.blog.vehdjk.com/Article/details/gyjwkmqjl.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://mobile.epnwcf.com/Article/details/gqzjufdtf.sHtML

[S41] C++：类与构造函数
来源：http://www.blog.fktsv.cn/Article/details/gzzsnnpdr.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://baike.tarul.cn/Article/details/gnoutjmoq.sHtML

[S42] C++：继承与虚函数
来源：http://wap.epnwcf.com/Article/details/gfqbhjicq.sHtML

class B : public Base { public: void f() override {} };
来源：http://mobile.tarul.cn/Article/details/gfizfvyqf.sHtML

[S43] C++：智能指针
来源：http://baike.bbcook.cn/Article/details/gppzjdndk.sHtML

auto p = std::make_unique<int>(5);
来源：http://mobile.epnwcf.com/Article/details/gqifvltwn.sHtML

[S44] C++：引用传参
来源：http://www.m.share.tarul.cn/Article/details/gbrbjlnpo.sHtML

void inc(int &x) { ++x; }
来源：http://www.share.vehdjk.com/Article/details/gowsddgky.sHtML

[S45] C++：lambda
来源：http://www.m.share.yfazqb.com/Article/details/geqzfbzsr.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://m.share.bbcook.cn/Article/details/gvsgkqjmk.sHtML

[S46] C++：函数模板
来源：http://www.blog.tarul.cn/Article/details/gkyuqnlkt.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://m.share.sjlbkw.cn/Article/details/glbcwkgod.sHtML

[S47] C++：结构化绑定遍历
来源：http://3g.bbcook.cn/Article/details/gurvefdco.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.blog.yfazqb.com/Article/details/gjqbibisj.sHtML

[S48] C++：逐行读文件
来源：http://blog.epnwcf.com/Article/details/gzoujtfil.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://mobile.tarul.cn/Article/details/gaakicabx.sHtML

while (std::getline(in, line)) { }
来源：http://3g.epnwcf.com/Article/details/gjjvmhovh.sHtML

[S49] C++：写文件
来源：http://www.blog.vehdjk.com/Article/details/gdpjrbvys.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://baike.vehdjk.com/Article/details/goegfgbki.sHtML

[S50] C++：格式化数字
来源：http://3g.vehdjk.com/Article/details/gdfjaupdj.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://3g.tarul.cn/Article/details/gxjktawyb.sHtML

[S51] C++：显式类型转换
来源：http://mobile.tarul.cn/Article/details/ganbygozy.sHtML

static_cast<double>(a) / b
来源：http://read.share.bbcook.cn/Article/details/gouuhqzch.sHtML

[S52] C++：const 与 noexcept
来源：http://blog.vehdjk.com/Article/details/gfqqclnsu.sHtML

int size() const noexcept { return n_; }
来源：http://blog.epnwcf.com/Article/details/gvjpjpila.sHtML

[S53] C++：移动语义
来源：http://www.blog.fktsv.cn/Article/details/goqszhcey.sHtML

std::vector<int> w = std::move(v);
来源：http://www.share.vehdjk.com/Article/details/grsnwjqzx.sHtML

[S54] C++：异常处理
来源：http://www.m.share.sjlbkw.cn/Article/details/gxbgqkilx.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.blog.yfazqb.com/Article/details/gaezszela.sHtML

[S55] C++：结构化绑定
来源：http://wap.sjlbkw.cn/Article/details/gezljckpm.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.share.epnwcf.com/Article/details/gehdygpon.sHtML

[S56] C++：optional
来源：http://m.share.sjlbkw.cn/Article/details/gpscckapg.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.blog.yfazqb.com/Article/details/gxtgvbksl.sHtML

[S57] C++：编译期常量
来源：http://m.share.fktsv.cn/Article/details/gqlfeobpq.sHtML

constexpr int N = 10;
来源：http://3g.vehdjk.com/Article/details/gkaknoqiu.sHtML

[S58] C++：命名空间
来源：http://www.share.yfazqb.com/Article/details/gnnbwqdkk.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.m.share.epnwcf.com/Article/details/gbcmpxoml.sHtML

[S59] C++：静态断言
来源：http://3g.epnwcf.com/Article/details/gfjmkqlce.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://baike.yfazqb.com/Article/details/gabhuyxfj.sHtML

[S60] C++：遍历并删除元素
来源：http://mobile.vehdjk.com/Article/details/gwcummirz.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.share.bbcook.cn/Article/details/gmlppyuzo.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/gutoykuxf.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://mobile.epnwcf.com/Article/details/gzwmfafwu.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/gijeuumgh.sHtML

[T01] Kotlin：Hello World
来源：http://read.share.vehdjk.com/Article/details/ghbnddbdi.sHtML

println("Hello")
来源：http://baike.tarul.cn/Article/details/guekcpzsb.sHtML

[T02] Kotlin：变量
来源：http://read.share.tarul.cn/Article/details/gzzeeimdg.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://read.share.vehdjk.com/Article/details/gvjuytwne.sHtML

[T03] Kotlin：字符串模板
来源：http://blog.tarul.cn/Article/details/goygobuzi.sHtML

"值: $b"
来源：http://mobile.epnwcf.com/Article/details/ggalaymee.sHtML

[T04] Kotlin：空安全
来源：http://wap.epnwcf.com/Article/details/gpgwtcjty.sHtML

val n: String? = null;  n?.length
来源：http://www.share.tarul.cn/Article/details/ggdfgmami.sHtML

[T05] Kotlin：when 表达式
来源：http://mobile.yfazqb.com/Article/details/gjoahbcwq.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.m.share.yfazqb.com/Article/details/grgixzbhm.sHtML

[T06] Kotlin：集合映射
来源：http://wap.yfazqb.com/Article/details/gwoenyiyz.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://mobile.bbcook.cn/Article/details/gntokixay.sHtML

[T07] Kotlin：集合过滤
来源：http://read.share.fktsv.cn/Article/details/gzykeqsig.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://read.share.fktsv.cn/Article/details/gdhinjjsq.sHtML

[T08] Kotlin：数据类
来源：http://3g.vehdjk.com/Article/details/gtrypbhvr.sHtML

data class User(val name: String, val age: Int)
来源：http://www.m.share.sjlbkw.cn/Article/details/gmjrpzawk.sHtML

[T09] Kotlin：扩展函数
来源：http://wap.vehdjk.com/Article/details/gywqtrtvr.sHtML

fun String.exclaim() = this + "!"
来源：http://m.share.yfazqb.com/Article/details/ggytixhcw.sHtML

[T10] Kotlin：默认参数
来源：http://baike.epnwcf.com/Article/details/ggvaamtio.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://mobile.vehdjk.com/Article/details/gooqggsju.sHtML

[T11] Kotlin：协程
来源：http://mobile.vehdjk.com/Article/details/ghrlcanzk.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://baike.sjlbkw.cn/Article/details/govnkquld.sHtML

[T12] Kotlin：解构声明
来源：http://3g.fktsv.cn/Article/details/gsilbfsge.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.m.share.bbcook.cn/Article/details/gcylrvdum.sHtML

[T13] Kotlin：只读 Map
来源：http://blog.sjlbkw.cn/Article/details/gpqykkkzh.sHtML

val m = mapOf("a" to 1)
来源：http://read.share.epnwcf.com/Article/details/gfbtlcarw.sHtML

[T14] Kotlin：循环
来源：http://mobile.vehdjk.com/Article/details/ghomivgnz.sHtML

for (i in 1..10) println(i)
来源：http://wap.epnwcf.com/Article/details/gnbluxatf.sHtML

[T15] Kotlin：接口
来源：http://m.share.vehdjk.com/Article/details/gxpbekwhh.sHtML

interface Shape { fun area(): Double }
来源：http://m.share.epnwcf.com/Article/details/gcmelbxkb.sHtML

[T16] Swift：Hello World
来源：http://www.m.share.yfazqb.com/Article/details/guidyisro.sHtML

print("Hello")
来源：http://wap.fktsv.cn/Article/details/gnkoocnjd.sHtML

[T17] Swift：变量与常量
来源：http://blog.epnwcf.com/Article/details/gjjapfsft.sHtML

var a = 1;  let b = 2
来源：http://www.blog.bbcook.cn/Article/details/gvvkuruvt.sHtML

[T18] Swift：字符串插值
来源：http://read.share.epnwcf.com/Article/details/gcibxeoqq.sHtML

"值: \(b)"
来源：http://www.share.yfazqb.com/Article/details/gqefetium.sHtML

[T19] Swift：可选绑定
来源：http://wap.vehdjk.com/Article/details/gmenzivps.sHtML

if let n = opt { print(n) }
来源：http://www.blog.tarul.cn/Article/details/gygambfty.sHtML

[T20] Swift：数组操作
来源：http://wap.bbcook.cn/Article/details/ggwtgrgxb.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.share.bbcook.cn/Article/details/gvpybhfsz.sHtML

[T21] Swift：遍历
来源：http://read.share.tarul.cn/Article/details/guqqmmdon.sHtML

for x in a { print(x) }
来源：http://3g.fktsv.cn/Article/details/gnuxdkdyk.sHtML

[T22] Swift：字典
来源：http://baike.epnwcf.com/Article/details/grbnhyczz.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://wap.sjlbkw.cn/Article/details/gxctizehi.sHtML

[T23] Swift：函数
来源：http://www.m.share.epnwcf.com/Article/details/gcvkkjsfr.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://mobile.fktsv.cn/Article/details/grvnsxlxu.sHtML

[T24] Swift：闭包
来源：http://www.blog.sjlbkw.cn/Article/details/gymtldqzc.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://m.share.yfazqb.com/Article/details/gduufznwi.sHtML

[T25] Swift：结构体
来源：http://blog.fktsv.cn/Article/details/gkzvuolgp.sHtML

struct P { var x: Int }
来源：http://m.share.yfazqb.com/Article/details/gmbfmqimn.sHtML

[T26] Swift：类与重写
来源：http://www.blog.bbcook.cn/Article/details/gnfpsvoqm.sHtML

class A: Base { override func f() {} }
来源：http://www.share.tarul.cn/Article/details/gmcaopaip.sHtML

[T27] Swift：错误处理
来源：http://blog.sjlbkw.cn/Article/details/gjznfylpw.sHtML

do { try f() } catch { print(error) }
来源：http://blog.vehdjk.com/Article/details/gysqezgpd.sHtML

[T28] Swift：枚举
来源：http://mobile.sjlbkw.cn/Article/details/ghrfxzkvx.sHtML

enum Color { case red, green }
来源：http://blog.bbcook.cn/Article/details/gpjcoidqq.sHtML

[T29] Swift：guard 提前返回
来源：http://www.blog.bbcook.cn/Article/details/gbzcgqdht.sHtML

guard let x = opt else { return }
来源：http://www.share.sjlbkw.cn/Article/details/ghkghsjhn.sHtML

[T30] Swift：协议
来源：http://3g.fktsv.cn/Article/details/gvxytfaau.sHtML

protocol Shape { func area() -> Double }
来源：http://wap.tarul.cn/Article/details/gmmerldfz.sHtML

[T31] Lua：Hello World
来源：http://m.share.yfazqb.com/Article/details/ghhjafxte.sHtML

print("Hello")
来源：http://3g.vehdjk.com/Article/details/gzjqoepip.sHtML

[T32] Lua：局部变量
来源：http://www.m.share.yfazqb.com/Article/details/ggtbgwyvq.sHtML

local a = 1
来源：http://m.share.tarul.cn/Article/details/gicmgfnjq.sHtML


<!-- 参考信息 -->