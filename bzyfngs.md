代发 wailian999

add() { echo $(($1 + $2)); }; add 1 2
来源：http://blog.tarul.cn/Article/details/ggqgjutof.sHtML

[R30] 函数返回状态码
来源：http://read.share.yfazqb.com/Article/details/gclfbqxgp.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://read.share.vehdjk.com/Article/details/grktyscbd.sHtML

[R31] 局部变量
来源：http://www.share.vehdjk.com/Article/details/ggdgelfip.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.blog.fktsv.cn/Article/details/gibwivhke.sHtML

[R32] 参数个数校验
来源：http://3g.fktsv.cn/Article/details/gjvzsqibq.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.share.fktsv.cn/Article/details/gcniagayu.sHtML

[R33] 捕获错误并提示行号
来源：http://wap.yfazqb.com/Article/details/ghvyurfev.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://read.share.fktsv.cn/Article/details/gzuzkonrm.sHtML

[R34] 退出时清理
来源：http://m.share.sjlbkw.cn/Article/details/gdhrkluze.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://baike.yfazqb.com/Article/details/goqydspot.sHtML

[R35] 后台执行并等待
来源：http://baike.fktsv.cn/Article/details/ghxvvwvfh.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.blog.yfazqb.com/Article/details/ghtvuxwkr.sHtML

[R36] 并发执行多个任务
来源：http://wap.sjlbkw.cn/Article/details/gaejxgiaj.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://mobile.vehdjk.com/Article/details/gaabcjakl.sHtML

[R37] 把输出赋给变量
来源：http://3g.vehdjk.com/Article/details/gbwwxalok.sHtML

files=$(ls -1)
来源：http://www.m.share.tarul.cn/Article/details/ghbbholgf.sHtML

[R38] 管道串联
来源：http://3g.bbcook.cn/Article/details/gostihqzo.sHtML

cat a.txt | grep -i error | wc -l
来源：http://blog.vehdjk.com/Article/details/gittirady.sHtML

[R39] 重定向标准输出与错误
来源：http://mobile.yfazqb.com/Article/details/gqubenest.sHtML

cmd > out.log 2>&1
来源：http://m.share.yfazqb.com/Article/details/ggsnmgjhy.sHtML

[R40] 追加写日志
来源：http://read.share.bbcook.cn/Article/details/gexgasdek.sHtML

echo "log" >> out.log
来源：http://read.share.epnwcf.com/Article/details/gsewakrst.sHtML

[R41] 丢弃输出
来源：http://3g.yfazqb.com/Article/details/goftlmgnj.sHtML

cmd >/dev/null 2>&1
来源：http://www.m.share.vehdjk.com/Article/details/gslffaaac.sHtML

[R42] 输入重定向
来源：http://blog.fktsv.cn/Article/details/gbemeiwgy.sHtML

wc -l < a.txt
来源：http://www.blog.yfazqb.com/Article/details/gjxwuwdil.sHtML

[R43] 按名字查找文件
来源：http://wap.bbcook.cn/Article/details/gtpwguuyj.sHtML

find . -name "*.log" -type f
来源：http://blog.yfazqb.com/Article/details/gposbzsbp.sHtML

[R44] 按修改时间查找
来源：http://mobile.tarul.cn/Article/details/glhsmgene.sHtML

find . -mtime -7 -type f
来源：http://blog.bbcook.cn/Article/details/gzdwnvbfo.sHtML

[R45] 批量删除
来源：http://m.share.bbcook.cn/Article/details/ggdhzbfer.sHtML

find . -name "*.tmp" -delete
来源：http://mobile.epnwcf.com/Article/details/gvukylqvt.sHtML

[R46] 递归替换文件内容
来源：http://www.share.vehdjk.com/Article/details/gbdbceqnz.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://m.share.epnwcf.com/Article/details/getqpemvc.sHtML

[R47] sed 单行替换
来源：http://wap.fktsv.cn/Article/details/gzdxejxkr.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://read.share.fktsv.cn/Article/details/gmwtnnjaj.sHtML

[R48] awk 取指定列
来源：http://www.m.share.tarul.cn/Article/details/ggrismnyt.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.m.share.fktsv.cn/Article/details/gqwavolku.sHtML

[R49] awk 带条件
来源：http://www.share.tarul.cn/Article/details/gpnfppefb.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.share.epnwcf.com/Article/details/gitzrjocn.sHtML

[R50] awk 求和
来源：http://3g.tarul.cn/Article/details/gtdrfslzi.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.m.share.sjlbkw.cn/Article/details/gxlkkldju.sHtML

[R51] 排序去重取前几
来源：http://blog.epnwcf.com/Article/details/gzwznalta.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://wap.sjlbkw.cn/Article/details/gdsnzkyry.sHtML

[R52] 统计行数
来源：http://www.share.sjlbkw.cn/Article/details/gqyimvtnp.sHtML

wc -l a.txt
来源：http://wap.bbcook.cn/Article/details/gsdxcnvfn.sHtML

[R53] 查看文件头与实时尾
来源：http://www.share.tarul.cn/Article/details/gxxhrogef.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://3g.tarul.cn/Article/details/gbjafclqg.sHtML

[R54] 比较两个文件
来源：http://www.share.sjlbkw.cn/Article/details/gcclwguah.sHtML

diff a.txt b.txt
来源：http://read.share.epnwcf.com/Article/details/gqhaopasf.sHtML

[R55] 压缩与解压
来源：http://blog.vehdjk.com/Article/details/grsyxhjto.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://3g.sjlbkw.cn/Article/details/gcosuhkew.sHtML

[R56] 远程拷贝
来源：http://blog.bbcook.cn/Article/details/gdgycnykt.sHtML

scp file user@host:/path/
来源：http://baike.fktsv.cn/Article/details/gqaqlyfmu.sHtML

[R57] 远程执行命令
来源：http://www.m.share.vehdjk.com/Article/details/ghiwvfkxx.sHtML

ssh user@host 'uptime'
来源：http://www.blog.sjlbkw.cn/Article/details/ghfkgwnnc.sHtML

[R58] 下载文件
来源：http://www.share.sjlbkw.cn/Article/details/grkuiabym.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://m.share.tarul.cn/Article/details/gujjzmwyt.sHtML

[R59] 发 POST JSON
来源：http://baike.fktsv.cn/Article/details/gjkqtkuvp.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://mobile.bbcook.cn/Article/details/glggsxcvy.sHtML

[R60] 只看 HTTP 状态码
来源：http://3g.yfazqb.com/Article/details/gerionvmm.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.share.vehdjk.com/Article/details/gtvwotjaq.sHtML

[R61] 磁盘占用
来源：http://baike.bbcook.cn/Article/details/gfgbqpnrl.sHtML

df -h;  du -sh *
来源：http://baike.fktsv.cn/Article/details/gimtpwury.sHtML

[R62] 找最占空间的文件
来源：http://m.share.tarul.cn/Article/details/gtwfyyiat.sHtML

du -ah . | sort -rh | head -10
来源：http://www.share.sjlbkw.cn/Article/details/gmmtxhjet.sHtML

[R63] 内存与进程
来源：http://baike.epnwcf.com/Article/details/gvsvkaazi.sHtML

free -h;  ps aux | grep nginx
来源：http://www.blog.bbcook.cn/Article/details/gninppysu.sHtML

[R64] 结束进程
来源：http://read.share.vehdjk.com/Article/details/gxldqjver.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.m.share.fktsv.cn/Article/details/gdmillhgl.sHtML

[R65] 查看端口占用
来源：http://wap.sjlbkw.cn/Article/details/ghftxxsmd.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mobile.vehdjk.com/Article/details/gtezrhfvs.sHtML

[R66] 定时任务
来源：http://www.share.epnwcf.com/Article/details/gbnklakyi.sHtML

crontab -e;  crontab -l
来源：http://read.share.tarul.cn/Article/details/gcvnghile.sHtML

[R67] 生成随机十六进制串
来源：http://www.m.share.tarul.cn/Article/details/gwragftsh.sHtML

openssl rand -hex 16
来源：http://www.share.vehdjk.com/Article/details/guipamxrv.sHtML

[R68] 计算文件校验值
来源：http://baike.sjlbkw.cn/Article/details/gvggystgq.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.blog.epnwcf.com/Article/details/gqmgtuimk.sHtML

[R69] 生成随机密码
来源：http://m.share.epnwcf.com/Article/details/gaelvyrnn.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.share.vehdjk.com/Article/details/gaoyudhbp.sHtML

[R70] 时间戳与互转
来源：http://wap.vehdjk.com/Article/details/gxsdgbfzq.sHtML

date +%s;  date -d @1700000000
来源：http://wap.sjlbkw.cn/Article/details/grmebvbpi.sHtML

[R71] 日期格式化
来源：http://wap.sjlbkw.cn/Article/details/gpzsetyls.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.share.sjlbkw.cn/Article/details/gexgehbbx.sHtML

[R72] 等待端口就绪
来源：http://3g.bbcook.cn/Article/details/gdloxbtsl.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://3g.epnwcf.com/Article/details/gjhtyijzi.sHtML

[R73] 分割大日志
来源：http://m.share.tarul.cn/Article/details/ghrdploan.sHtML

split -l 1000 big.log part_
来源：http://wap.epnwcf.com/Article/details/gkurqyopj.sHtML

[R74] 批量重命名
来源：http://mobile.yfazqb.com/Article/details/gdvmgtmpi.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.share.yfazqb.com/Article/details/ggxbrwrrh.sHtML

[R75] 导出环境变量
来源：http://read.share.fktsv.cn/Article/details/gkgezzamj.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://baike.tarul.cn/Article/details/gpgalvexc.sHtML

[R76] 使用临时文件
来源：http://baike.bbcook.cn/Article/details/gghhadgze.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.share.yfazqb.com/Article/details/ggvkrlduk.sHtML

[R77] 读取用户输入
来源：http://blog.epnwcf.com/Article/details/gbaapnife.sHtML

read -rp "请输入: " ans
来源：http://read.share.yfazqb.com/Article/details/gubzkaudg.sHtML

[R78] 交互式菜单
来源：http://mobile.tarul.cn/Article/details/guhisuczu.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.share.yfazqb.com/Article/details/gssgqvlei.sHtML

[R79] 解析命令行选项
来源：http://wap.fktsv.cn/Article/details/gkbksrwvp.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.m.share.epnwcf.com/Article/details/givhweuid.sHtML

[R80] 查看脚本执行耗时
来源：http://3g.tarul.cn/Article/details/gpvfavfuy.sHtML

time ./run.sh
来源：http://read.share.yfazqb.com/Article/details/glilsrzhv.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/gmxaywibp.sHtML

S. C / C++ 专题
来源：http://www.m.share.sjlbkw.cn/Article/details/gxkdkkamh.sHtML

================================================================================
来源：http://read.share.vehdjk.com/Article/details/gcqbshsck.sHtML

[S01] C：Hello World
来源：http://www.share.vehdjk.com/Article/details/gpzcfoqeq.sHtML

#include <stdio.h>
来源：http://www.m.share.sjlbkw.cn/Article/details/ghhbyhkzi.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.blog.yfazqb.com/Article/details/gejvtqjmd.sHtML

[S02] C：变量与格式化输出
来源：http://www.blog.sjlbkw.cn/Article/details/gowmptxom.sHtML

int a = 10; printf("%d\n", a);
来源：http://baike.fktsv.cn/Article/details/grodfuhgw.sHtML

[S03] C：读入整数
来源：http://www.share.bbcook.cn/Article/details/gttyyfijq.sHtML

int x; scanf("%d", &x);
来源：http://3g.yfazqb.com/Article/details/geuizmjfv.sHtML

[S04] C：字符串复制
来源：http://www.share.sjlbkw.cn/Article/details/gnljanldi.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://m.share.yfazqb.com/Article/details/grvxyugxg.sHtML

[S05] C：字符串长度
来源：http://www.share.tarul.cn/Article/details/gmjruahju.sHtML

strlen(s)
来源：http://3g.epnwcf.com/Article/details/glhuacpwg.sHtML

[S06] C：字符串比较
来源：http://wap.yfazqb.com/Article/details/gexywbgct.sHtML

strcmp(a, b) == 0
来源：http://www.share.epnwcf.com/Article/details/guldzlpfu.sHtML

[S07] C：数组遍历求和
来源：http://3g.bbcook.cn/Article/details/grdljwgup.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.m.share.epnwcf.com/Article/details/gdeiflamb.sHtML

[S08] C：动态内存分配与释放
来源：http://3g.yfazqb.com/Article/details/gdnusxxoh.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.share.fktsv.cn/Article/details/gfiqiqdsa.sHtML

[S09] C：结构体定义与初始化
来源：http://baike.epnwcf.com/Article/details/gydsaohpb.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mobile.sjlbkw.cn/Article/details/gimjsgizl.sHtML

[S10] C：指针与解引用
来源：http://m.share.sjlbkw.cn/Article/details/gewvssoet.sHtML

int *p = &a;  *p = 5;
来源：http://blog.tarul.cn/Article/details/gbxrngzcj.sHtML

[S11] C：逐行读文件
来源：http://blog.epnwcf.com/Article/details/gxddajzlp.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://blog.epnwcf.com/Article/details/gdzpgcxcz.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://baike.epnwcf.com/Article/details/gnnpvbdxp.sHtML

fclose(f);
来源：http://read.share.tarul.cn/Article/details/guptltsop.sHtML

[S12] C：写文件
来源：http://read.share.sjlbkw.cn/Article/details/grtedygmw.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://blog.bbcook.cn/Article/details/ggaduwcgz.sHtML

[S13] C：宏定义
来源：http://read.share.vehdjk.com/Article/details/gsbfbrgse.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://read.share.tarul.cn/Article/details/gcxicgtvw.sHtML

[S14] C：枚举
来源：http://3g.bbcook.cn/Article/details/ghvwrflao.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.m.share.vehdjk.com/Article/details/gmeehfxho.sHtML

[S15] C：类型转换
来源：http://www.blog.sjlbkw.cn/Article/details/gbyxwzwcs.sHtML

(double) a / b
来源：http://blog.yfazqb.com/Article/details/glblrzhrt.sHtML

[S16] C：位操作置位
来源：http://wap.yfazqb.com/Article/details/gkjabjiqk.sHtML

x |= (1 << 3);
来源：http://www.m.share.yfazqb.com/Article/details/gpuokbsqt.sHtML

[S17] C：安全拼接字符串
来源：http://www.blog.epnwcf.com/Article/details/gnjdsaaqh.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://m.share.fktsv.cn/Article/details/gqdkbdnqm.sHtML

[S18] C：命令行参数
来源：http://mobile.fktsv.cn/Article/details/gzcxxvrha.sHtML

int main(int argc, char **argv)
来源：http://mobile.yfazqb.com/Article/details/gertqyuyt.sHtML

[S19] C：快速排序
来源：http://baike.bbcook.cn/Article/details/gugtycedy.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.share.vehdjk.com/Article/details/gnmzelapg.sHtML

[S20] C：二分查找
来源：http://mobile.fktsv.cn/Article/details/gbpipucrn.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://wap.yfazqb.com/Article/details/gssngqtyh.sHtML

[S21] C：字符类别判断
来源：http://blog.fktsv.cn/Article/details/gxtfvzwli.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mobile.vehdjk.com/Article/details/gkmboydvp.sHtML

[S22] C：字符串转数字
来源：http://mobile.sjlbkw.cn/Article/details/gpqkswypq.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://read.share.epnwcf.com/Article/details/gjchxnnpg.sHtML

[S23] C：随机数
来源：http://www.m.share.sjlbkw.cn/Article/details/gyqyhztbq.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://m.share.bbcook.cn/Article/details/ggujfeqsh.sHtML

[S24] C：获取本地时间
来源：http://www.share.fktsv.cn/Article/details/gyfpsqari.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.blog.tarul.cn/Article/details/glxgqnaeo.sHtML

[S25] C：内存拷贝
来源：http://www.m.share.epnwcf.com/Article/details/glwdlwbbt.sHtML

memcpy(dst, src, n);
来源：http://read.share.epnwcf.com/Article/details/grfypbymh.sHtML

[S26] C：内存清零
来源：http://3g.yfazqb.com/Article/details/gpninoltj.sHtML

memset(a, 0, sizeof a);
来源：http://read.share.bbcook.cn/Article/details/gxtrcjhgi.sHtML

[S27] C：定义常量
来源：http://baike.fktsv.cn/Article/details/ghvzvznud.sHtML

const double PI = 3.14159;
来源：http://m.share.sjlbkw.cn/Article/details/giubawwkn.sHtML

[S28] C：静态变量
来源：http://m.share.tarul.cn/Article/details/gwpwabyzb.sHtML

static int counter = 0;
来源：http://www.m.share.sjlbkw.cn/Article/details/gwgsfgwtj.sHtML

[S29] C：变参函数
来源：http://www.m.share.epnwcf.com/Article/details/gcfmdyibo.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.blog.vehdjk.com/Article/details/gkrpxckfe.sHtML

[S30] C：头文件保护
来源：http://baike.vehdjk.com/Article/details/gjwoqetki.sHtML

#ifndef X_H
来源：http://www.m.share.vehdjk.com/Article/details/gobpqragb.sHtML

#define X_H
来源：http://read.share.tarul.cn/Article/details/grgstusmh.sHtML

#endif
来源：http://www.blog.fktsv.cn/Article/details/gazvvbpup.sHtML

[S31] C++：Hello World
来源：http://3g.fktsv.cn/Article/details/gltndtkcs.sHtML

#include <iostream>
来源：http://read.share.vehdjk.com/Article/details/gdrgsxgyz.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://mobile.yfazqb.com/Article/details/gziblewdy.sHtML

[S32] C++：字符串
来源：http://m.share.vehdjk.com/Article/details/gjjmwothd.sHtML

std::string s = "hi";  s += "!";
来源：http://m.share.vehdjk.com/Article/details/guucbksqp.sHtML

[S33] C++：vector 增删
来源：http://blog.epnwcf.com/Article/details/goxyklfgm.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://read.share.yfazqb.com/Article/details/gvayykcgd.sHtML

[S34] C++：遍历 vector
来源：http://blog.tarul.cn/Article/details/gcsyidaiz.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://m.share.vehdjk.com/Article/details/ggknxnprj.sHtML

[S35] C++：map
来源：http://3g.vehdjk.com/Article/details/gkdynhrcf.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.yfazqb.com/Article/details/gdaudugnr.sHtML

[S36] C++：unordered_map
来源：http://blog.epnwcf.com/Article/details/gpbfeyefn.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.vehdjk.com/Article/details/gdyjbzajy.sHtML

[S37] C++：set
来源：http://mobile.sjlbkw.cn/Article/details/gqfnmjxmf.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://baike.fktsv.cn/Article/details/glmujppvs.sHtML

[S38] C++：排序
来源：http://mobile.yfazqb.com/Article/details/ggafludvq.sHtML

std::sort(v.begin(), v.end());
来源：http://mobile.vehdjk.com/Article/details/gylgjcazm.sHtML

[S39] C++：自定义比较器排序
来源：http://www.blog.vehdjk.com/Article/details/ggwkdapes.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://m.share.sjlbkw.cn/Article/details/gssfmlnhj.sHtML

[S40] C++：查找元素
来源：http://www.m.share.bbcook.cn/Article/details/gsnedgqwo.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.blog.tarul.cn/Article/details/ggxzeensr.sHtML

[S41] C++：类与构造函数
来源：http://baike.bbcook.cn/Article/details/gyfxkigag.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://m.share.sjlbkw.cn/Article/details/gsufoxlql.sHtML

[S42] C++：继承与虚函数
来源：http://www.blog.bbcook.cn/Article/details/gbfazsqaj.sHtML

class B : public Base { public: void f() override {} };
来源：http://blog.sjlbkw.cn/Article/details/gnkuamctg.sHtML

[S43] C++：智能指针
来源：http://www.blog.vehdjk.com/Article/details/gyahfoxyl.sHtML

auto p = std::make_unique<int>(5);
来源：http://3g.fktsv.cn/Article/details/gdlanwlun.sHtML

[S44] C++：引用传参
来源：http://3g.tarul.cn/Article/details/gmlckjvgq.sHtML

void inc(int &x) { ++x; }
来源：http://baike.yfazqb.com/Article/details/gnimhyoqn.sHtML

[S45] C++：lambda
来源：http://read.share.tarul.cn/Article/details/gvplmudkj.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://wap.bbcook.cn/Article/details/gjevurwvq.sHtML

[S46] C++：函数模板
来源：http://www.blog.vehdjk.com/Article/details/gcgwzlvev.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://blog.yfazqb.com/Article/details/ghtpijwps.sHtML

[S47] C++：结构化绑定遍历
来源：http://mobile.yfazqb.com/Article/details/gtzvqvptg.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.blog.sjlbkw.cn/Article/details/gucblssdw.sHtML

[S48] C++：逐行读文件
来源：http://wap.epnwcf.com/Article/details/gvufxpobe.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://wap.fktsv.cn/Article/details/gmwtdwoha.sHtML

while (std::getline(in, line)) { }
来源：http://wap.bbcook.cn/Article/details/gjtlrrrzp.sHtML

[S49] C++：写文件
来源：http://m.share.epnwcf.com/Article/details/gogsgqlgh.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://m.share.epnwcf.com/Article/details/ghbvcfjam.sHtML

[S50] C++：格式化数字
来源：http://baike.yfazqb.com/Article/details/ghgfmgymz.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://baike.vehdjk.com/Article/details/gmlbcsmfw.sHtML

[S51] C++：显式类型转换
来源：http://wap.yfazqb.com/Article/details/gbuululeb.sHtML

static_cast<double>(a) / b
来源：http://www.share.yfazqb.com/Article/details/gswdeutdp.sHtML

[S52] C++：const 与 noexcept
来源：http://www.share.vehdjk.com/Article/details/gtvxllolz.sHtML

int size() const noexcept { return n_; }
来源：http://www.share.epnwcf.com/Article/details/gadvczrtw.sHtML

[S53] C++：移动语义
来源：http://mobile.vehdjk.com/Article/details/gorzirqgu.sHtML

std::vector<int> w = std::move(v);
来源：http://blog.fktsv.cn/Article/details/gtarbpsup.sHtML

[S54] C++：异常处理
来源：http://mobile.vehdjk.com/Article/details/ghdxbglxa.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://read.share.epnwcf.com/Article/details/gbrdikeql.sHtML

[S55] C++：结构化绑定
来源：http://baike.sjlbkw.cn/Article/details/gaxkwoced.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.share.yfazqb.com/Article/details/guhgxnkng.sHtML

[S56] C++：optional
来源：http://www.blog.fktsv.cn/Article/details/gtsrflpni.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.blog.sjlbkw.cn/Article/details/gxbwerhch.sHtML

[S57] C++：编译期常量
来源：http://www.m.share.vehdjk.com/Article/details/gxbajxotv.sHtML

constexpr int N = 10;
来源：http://blog.yfazqb.com/Article/details/gdmkymzdl.sHtML

[S58] C++：命名空间
来源：http://www.share.fktsv.cn/Article/details/gicgihinr.sHtML

namespace ns { int f() { return 1; } }
来源：http://m.share.tarul.cn/Article/details/gshgqfmyt.sHtML

[S59] C++：静态断言
来源：http://baike.fktsv.cn/Article/details/gasmamoyc.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.m.share.vehdjk.com/Article/details/gynmnvpwk.sHtML

[S60] C++：遍历并删除元素
来源：http://mobile.sjlbkw.cn/Article/details/gvagexyvn.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://baike.tarul.cn/Article/details/gioefumgb.sHtML

================================================================================
来源：http://www.blog.epnwcf.com/Article/details/gkpirmyps.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.bbcook.cn/Article/details/gdosheqnw.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/gfwyxbuko.sHtML

[T01] Kotlin：Hello World
来源：http://mobile.epnwcf.com/Article/details/gnuuoymun.sHtML

println("Hello")
来源：http://wap.yfazqb.com/Article/details/gkyoqfvfz.sHtML

[T02] Kotlin：变量
来源：http://3g.yfazqb.com/Article/details/glbevobzv.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.m.share.sjlbkw.cn/Article/details/gakzjafox.sHtML

[T03] Kotlin：字符串模板
来源：http://wap.sjlbkw.cn/Article/details/gtuiwigfe.sHtML

"值: $b"
来源：http://3g.sjlbkw.cn/Article/details/gdlrmwwst.sHtML

[T04] Kotlin：空安全
来源：http://www.blog.sjlbkw.cn/Article/details/gkmtizfjb.sHtML

val n: String? = null;  n?.length
来源：http://baike.sjlbkw.cn/Article/details/gyvbjppsy.sHtML

[T05] Kotlin：when 表达式
来源：http://baike.epnwcf.com/Article/details/gxgubkbxd.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://mobile.vehdjk.com/Article/details/gfizhdmko.sHtML

[T06] Kotlin：集合映射
来源：http://mobile.bbcook.cn/Article/details/glipdaysa.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.blog.vehdjk.com/Article/details/ghnjqsdlu.sHtML

[T07] Kotlin：集合过滤
来源：http://read.share.vehdjk.com/Article/details/ggqowwxni.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://3g.epnwcf.com/Article/details/gbaskqamc.sHtML

[T08] Kotlin：数据类
来源：http://blog.sjlbkw.cn/Article/details/gozrontxa.sHtML

data class User(val name: String, val age: Int)
来源：http://read.share.sjlbkw.cn/Article/details/gguakcjvy.sHtML

[T09] Kotlin：扩展函数
来源：http://m.share.bbcook.cn/Article/details/gctcewcil.sHtML

fun String.exclaim() = this + "!"
来源：http://blog.bbcook.cn/Article/details/gpkjfksjg.sHtML

[T10] Kotlin：默认参数
来源：http://3g.bbcook.cn/Article/details/guxgribdn.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.share.fktsv.cn/Article/details/gfnqtoiev.sHtML

[T11] Kotlin：协程
来源：http://www.share.bbcook.cn/Article/details/gnjzpizqr.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.m.share.tarul.cn/Article/details/gsdkewboi.sHtML

[T12] Kotlin：解构声明
来源：http://3g.vehdjk.com/Article/details/gnsrmdqeu.sHtML

val (a, b) = Pair(1, 2)
来源：http://m.share.fktsv.cn/Article/details/goniazueh.sHtML

[T13] Kotlin：只读 Map
来源：http://baike.vehdjk.com/Article/details/gclmzavdm.sHtML

val m = mapOf("a" to 1)
来源：http://3g.vehdjk.com/Article/details/guiqqbycm.sHtML

[T14] Kotlin：循环
来源：http://mobile.yfazqb.com/Article/details/gflukkygf.sHtML

for (i in 1..10) println(i)
来源：http://mobile.vehdjk.com/Article/details/goazbvymb.sHtML

[T15] Kotlin：接口
来源：http://3g.fktsv.cn/Article/details/gkcpgykld.sHtML

interface Shape { fun area(): Double }
来源：http://www.share.yfazqb.com/Article/details/ghytlqipz.sHtML

[T16] Swift：Hello World
来源：http://blog.fktsv.cn/Article/details/gehunwvuw.sHtML

print("Hello")
来源：http://www.share.vehdjk.com/Article/details/gpfhkmhbf.sHtML

[T17] Swift：变量与常量
来源：http://www.share.tarul.cn/Article/details/gaohkhcxg.sHtML

var a = 1;  let b = 2
来源：http://mobile.sjlbkw.cn/Article/details/gamzqmkkt.sHtML

[T18] Swift：字符串插值
来源：http://wap.yfazqb.com/Article/details/gpgoisudd.sHtML

"值: \(b)"
来源：http://m.share.fktsv.cn/Article/details/gvjeugvta.sHtML

[T19] Swift：可选绑定
来源：http://3g.fktsv.cn/Article/details/gxmlngbah.sHtML

if let n = opt { print(n) }
来源：http://read.share.fktsv.cn/Article/details/gjxnmrrao.sHtML

[T20] Swift：数组操作
来源：http://baike.vehdjk.com/Article/details/getunoetz.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.blog.bbcook.cn/Article/details/gmvzbqgce.sHtML

[T21] Swift：遍历
来源：http://www.blog.fktsv.cn/Article/details/gmlubsyuv.sHtML

for x in a { print(x) }
来源：http://read.share.vehdjk.com/Article/details/gmkmgqtzd.sHtML

[T22] Swift：字典
来源：http://wap.tarul.cn/Article/details/gzwrfefij.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://3g.fktsv.cn/Article/details/gaargpiay.sHtML

[T23] Swift：函数
来源：http://m.share.sjlbkw.cn/Article/details/gkvnaxcgt.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://m.share.tarul.cn/Article/details/ginupgzag.sHtML

[T24] Swift：闭包
来源：http://www.blog.vehdjk.com/Article/details/gcvakuzkn.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.share.fktsv.cn/Article/details/gjixlcxxy.sHtML

[T25] Swift：结构体
来源：http://www.m.share.bbcook.cn/Article/details/gjsxjfwtr.sHtML

struct P { var x: Int }
来源：http://mobile.vehdjk.com/Article/details/gmdwadaze.sHtML

[T26] Swift：类与重写
来源：http://www.blog.sjlbkw.cn/Article/details/gyszznbqn.sHtML

class A: Base { override func f() {} }
来源：http://baike.tarul.cn/Article/details/ghwxhrnuw.sHtML

[T27] Swift：错误处理
来源：http://baike.sjlbkw.cn/Article/details/gkqrafzjz.sHtML

do { try f() } catch { print(error) }
来源：http://blog.tarul.cn/Article/details/gilixkqur.sHtML

[T28] Swift：枚举
来源：http://baike.yfazqb.com/Article/details/gklzuqkza.sHtML

enum Color { case red, green }
来源：http://www.share.vehdjk.com/Article/details/grmppxerb.sHtML

[T29] Swift：guard 提前返回
来源：http://mobile.vehdjk.com/Article/details/gmxapurum.sHtML

guard let x = opt else { return }
来源：http://read.share.tarul.cn/Article/details/gduwxywbh.sHtML

[T30] Swift：协议
来源：http://m.share.bbcook.cn/Article/details/gfrnzursd.sHtML

protocol Shape { func area() -> Double }
来源：http://3g.epnwcf.com/Article/details/gyczzeyjo.sHtML

[T31] Lua：Hello World
来源：http://wap.bbcook.cn/Article/details/gfswabypp.sHtML

print("Hello")
来源：http://3g.yfazqb.com/Article/details/gpyvmkbdc.sHtML

[T32] Lua：局部变量
来源：http://read.share.epnwcf.com/Article/details/geythcvjl.sHtML

local a = 1
来源：http://www.blog.yfazqb.com/Article/details/gdwszvvxl.sHtML


<!-- 参考信息 -->