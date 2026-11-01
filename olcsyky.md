代发 wailian999

files=$(ls -1)
来源：http://baike.bbcook.cn/Article/details/gnjgtqccs.sHtML

[R38] 管道串联
来源：http://www.share.epnwcf.com/Article/details/grmppxwbm.sHtML

cat a.txt | grep -i error | wc -l
来源：http://m.share.bbcook.cn/Article/details/gjlwhokxo.sHtML

[R39] 重定向标准输出与错误
来源：http://www.m.share.fktsv.cn/Article/details/gnitigutl.sHtML

cmd > out.log 2>&1
来源：http://mobile.tarul.cn/Article/details/gcljjmmbt.sHtML

[R40] 追加写日志
来源：http://mobile.sjlbkw.cn/Article/details/grwhtxkyc.sHtML

echo "log" >> out.log
来源：http://blog.fktsv.cn/Article/details/gnypulbrq.sHtML

[R41] 丢弃输出
来源：http://baike.sjlbkw.cn/Article/details/gakobubwa.sHtML

cmd >/dev/null 2>&1
来源：http://wap.fktsv.cn/Article/details/gowwfjxgf.sHtML

[R42] 输入重定向
来源：http://baike.vehdjk.com/Article/details/geurvzmtw.sHtML

wc -l < a.txt
来源：http://m.share.yfazqb.com/Article/details/gicoeyxng.sHtML

[R43] 按名字查找文件
来源：http://read.share.bbcook.cn/Article/details/gznoyomdz.sHtML

find . -name "*.log" -type f
来源：http://m.share.epnwcf.com/Article/details/gkhtqxklf.sHtML

[R44] 按修改时间查找
来源：http://www.blog.sjlbkw.cn/Article/details/goirfdytz.sHtML

find . -mtime -7 -type f
来源：http://www.share.tarul.cn/Article/details/gaderqapw.sHtML

[R45] 批量删除
来源：http://www.share.sjlbkw.cn/Article/details/ghumgzsli.sHtML

find . -name "*.tmp" -delete
来源：http://read.share.yfazqb.com/Article/details/gujawjguw.sHtML

[R46] 递归替换文件内容
来源：http://www.blog.epnwcf.com/Article/details/gumsglgrd.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.blog.epnwcf.com/Article/details/gzknngjih.sHtML

[R47] sed 单行替换
来源：http://baike.fktsv.cn/Article/details/givktnuuh.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://m.share.bbcook.cn/Article/details/gqbypqoom.sHtML

[R48] awk 取指定列
来源：http://wap.yfazqb.com/Article/details/gbvgxmtdz.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.blog.vehdjk.com/Article/details/gzclkydcq.sHtML

[R49] awk 带条件
来源：http://m.share.tarul.cn/Article/details/gomuevhnj.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://blog.fktsv.cn/Article/details/gazzryurt.sHtML

[R50] awk 求和
来源：http://3g.sjlbkw.cn/Article/details/gyebjofbq.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://3g.sjlbkw.cn/Article/details/gjzxqkehc.sHtML

[R51] 排序去重取前几
来源：http://www.m.share.sjlbkw.cn/Article/details/gyccstxdt.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://3g.vehdjk.com/Article/details/gylkysvit.sHtML

[R52] 统计行数
来源：http://wap.sjlbkw.cn/Article/details/gozmnkgve.sHtML

wc -l a.txt
来源：http://m.share.bbcook.cn/Article/details/grumotgqx.sHtML

[R53] 查看文件头与实时尾
来源：http://www.blog.bbcook.cn/Article/details/gbwqoschc.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://m.share.yfazqb.com/Article/details/ghxnecbsh.sHtML

[R54] 比较两个文件
来源：http://www.share.tarul.cn/Article/details/gycrxdvhf.sHtML

diff a.txt b.txt
来源：http://read.share.epnwcf.com/Article/details/gylllhoaz.sHtML

[R55] 压缩与解压
来源：http://read.share.epnwcf.com/Article/details/gmldhvydo.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.m.share.epnwcf.com/Article/details/ghdfnyrys.sHtML

[R56] 远程拷贝
来源：http://wap.fktsv.cn/Article/details/gclpcxrwx.sHtML

scp file user@host:/path/
来源：http://blog.yfazqb.com/Article/details/gwzwkxzhv.sHtML

[R57] 远程执行命令
来源：http://mobile.yfazqb.com/Article/details/gjfyrvmcd.sHtML

ssh user@host 'uptime'
来源：http://m.share.tarul.cn/Article/details/gdtmlvisb.sHtML

[R58] 下载文件
来源：http://3g.yfazqb.com/Article/details/gquzdfhnu.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.m.share.vehdjk.com/Article/details/glrpncfel.sHtML

[R59] 发 POST JSON
来源：http://mobile.sjlbkw.cn/Article/details/gadgqdxtp.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://baike.bbcook.cn/Article/details/gsyyhelvo.sHtML

[R60] 只看 HTTP 状态码
来源：http://m.share.epnwcf.com/Article/details/gumeebdwx.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://read.share.vehdjk.com/Article/details/gycofsiba.sHtML

[R61] 磁盘占用
来源：http://baike.bbcook.cn/Article/details/gdzpbypnn.sHtML

df -h;  du -sh *
来源：http://wap.epnwcf.com/Article/details/gtpgysrgy.sHtML

[R62] 找最占空间的文件
来源：http://www.share.yfazqb.com/Article/details/gmupekgtp.sHtML

du -ah . | sort -rh | head -10
来源：http://wap.fktsv.cn/Article/details/ggtjoslyb.sHtML

[R63] 内存与进程
来源：http://wap.fktsv.cn/Article/details/gjpfifcyp.sHtML

free -h;  ps aux | grep nginx
来源：http://m.share.vehdjk.com/Article/details/gvcukfbew.sHtML

[R64] 结束进程
来源：http://read.share.yfazqb.com/Article/details/ghfbekgnr.sHtML

kill -9 $(pgrep -f app.py)
来源：http://read.share.vehdjk.com/Article/details/gbnpujmtd.sHtML

[R65] 查看端口占用
来源：http://blog.tarul.cn/Article/details/gydexjxzz.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.share.epnwcf.com/Article/details/gfryidkpz.sHtML

[R66] 定时任务
来源：http://www.blog.sjlbkw.cn/Article/details/gpdbbhsyq.sHtML

crontab -e;  crontab -l
来源：http://www.share.epnwcf.com/Article/details/gfswqdjzh.sHtML

[R67] 生成随机十六进制串
来源：http://baike.epnwcf.com/Article/details/glyxyyoht.sHtML

openssl rand -hex 16
来源：http://mobile.epnwcf.com/Article/details/gucbpznpw.sHtML

[R68] 计算文件校验值
来源：http://www.blog.bbcook.cn/Article/details/gejivijyz.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://m.share.yfazqb.com/Article/details/gcnudofel.sHtML

[R69] 生成随机密码
来源：http://3g.vehdjk.com/Article/details/gkcxluiov.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.share.fktsv.cn/Article/details/gefcjebtd.sHtML

[R70] 时间戳与互转
来源：http://www.m.share.yfazqb.com/Article/details/gkscwokas.sHtML

date +%s;  date -d @1700000000
来源：http://www.share.vehdjk.com/Article/details/glsqkesvw.sHtML

[R71] 日期格式化
来源：http://blog.yfazqb.com/Article/details/gzfhjlbib.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://wap.bbcook.cn/Article/details/gyndvrgcg.sHtML

[R72] 等待端口就绪
来源：http://blog.fktsv.cn/Article/details/gblglduqw.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://read.share.bbcook.cn/Article/details/gvsptmzvk.sHtML

[R73] 分割大日志
来源：http://3g.yfazqb.com/Article/details/ghmuatfts.sHtML

split -l 1000 big.log part_
来源：http://read.share.yfazqb.com/Article/details/gewrsgrrx.sHtML

[R74] 批量重命名
来源：http://www.share.bbcook.cn/Article/details/govkududs.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://blog.sjlbkw.cn/Article/details/gkvkdonam.sHtML

[R75] 导出环境变量
来源：http://m.share.sjlbkw.cn/Article/details/gplnvnrzn.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://baike.tarul.cn/Article/details/gctnxzdok.sHtML

[R76] 使用临时文件
来源：http://blog.yfazqb.com/Article/details/gorslyvzb.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://baike.bbcook.cn/Article/details/gzubrbtjh.sHtML

[R77] 读取用户输入
来源：http://www.share.sjlbkw.cn/Article/details/gmmpdpzzv.sHtML

read -rp "请输入: " ans
来源：http://m.share.yfazqb.com/Article/details/gnbxgcgch.sHtML

[R78] 交互式菜单
来源：http://www.blog.yfazqb.com/Article/details/gdnriqsel.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.blog.fktsv.cn/Article/details/gstydsxrt.sHtML

[R79] 解析命令行选项
来源：http://m.share.yfazqb.com/Article/details/gbcegojfx.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.blog.epnwcf.com/Article/details/gusorlxqe.sHtML

[R80] 查看脚本执行耗时
来源：http://m.share.vehdjk.com/Article/details/ghlnrbbim.sHtML

time ./run.sh
来源：http://read.share.bbcook.cn/Article/details/grprquawy.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/gylbimnvm.sHtML

S. C / C++ 专题
来源：http://read.share.fktsv.cn/Article/details/gjbzbolcm.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/gzmummrft.sHtML

[S01] C：Hello World
来源：http://www.share.epnwcf.com/Article/details/gkmfchsfp.sHtML

#include <stdio.h>
来源：http://www.share.vehdjk.com/Article/details/gufzfvgao.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.share.epnwcf.com/Article/details/gqnoubrns.sHtML

[S02] C：变量与格式化输出
来源：http://3g.sjlbkw.cn/Article/details/gdfiblfyq.sHtML

int a = 10; printf("%d\n", a);
来源：http://wap.sjlbkw.cn/Article/details/ggdqnrtyi.sHtML

[S03] C：读入整数
来源：http://mobile.fktsv.cn/Article/details/gbjhoodbt.sHtML

int x; scanf("%d", &x);
来源：http://m.share.fktsv.cn/Article/details/gskhujtzt.sHtML

[S04] C：字符串复制
来源：http://wap.bbcook.cn/Article/details/gytbtibcp.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.m.share.bbcook.cn/Article/details/gpbqabdpa.sHtML

[S05] C：字符串长度
来源：http://www.m.share.tarul.cn/Article/details/gdxlueraz.sHtML

strlen(s)
来源：http://wap.vehdjk.com/Article/details/gfhgcwqpg.sHtML

[S06] C：字符串比较
来源：http://www.share.fktsv.cn/Article/details/gqtzwkhtc.sHtML

strcmp(a, b) == 0
来源：http://www.m.share.bbcook.cn/Article/details/gmrywguse.sHtML

[S07] C：数组遍历求和
来源：http://wap.tarul.cn/Article/details/gtxrlujik.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://wap.vehdjk.com/Article/details/glijevvmj.sHtML

[S08] C：动态内存分配与释放
来源：http://3g.fktsv.cn/Article/details/gpripmyur.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.share.epnwcf.com/Article/details/gjhecrozl.sHtML

[S09] C：结构体定义与初始化
来源：http://wap.epnwcf.com/Article/details/gjamhkvow.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://3g.epnwcf.com/Article/details/gksqdkgiq.sHtML

[S10] C：指针与解引用
来源：http://3g.vehdjk.com/Article/details/gbkqupnbu.sHtML

int *p = &a;  *p = 5;
来源：http://m.share.fktsv.cn/Article/details/gimoxgjdz.sHtML

[S11] C：逐行读文件
来源：http://mobile.tarul.cn/Article/details/ghwfscnjl.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.blog.tarul.cn/Article/details/gtrvcgtxr.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://m.share.fktsv.cn/Article/details/gktveaozg.sHtML

fclose(f);
来源：http://blog.epnwcf.com/Article/details/gvoxdkypl.sHtML

[S12] C：写文件
来源：http://baike.tarul.cn/Article/details/gwojpslap.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://baike.vehdjk.com/Article/details/grzixhyhj.sHtML

[S13] C：宏定义
来源：http://wap.vehdjk.com/Article/details/gzfsskgre.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wap.tarul.cn/Article/details/gjfolelvw.sHtML

[S14] C：枚举
来源：http://wap.epnwcf.com/Article/details/ghxneapqn.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://baike.yfazqb.com/Article/details/gfzfifeyt.sHtML

[S15] C：类型转换
来源：http://www.share.bbcook.cn/Article/details/gpfxcjbvu.sHtML

(double) a / b
来源：http://mobile.vehdjk.com/Article/details/ggxsohevd.sHtML

[S16] C：位操作置位
来源：http://read.share.vehdjk.com/Article/details/gnmmuzcrz.sHtML

x |= (1 << 3);
来源：http://mobile.bbcook.cn/Article/details/gahrdmumb.sHtML

[S17] C：安全拼接字符串
来源：http://www.m.share.yfazqb.com/Article/details/gvmperbye.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://3g.epnwcf.com/Article/details/ggdovypol.sHtML

[S18] C：命令行参数
来源：http://3g.sjlbkw.cn/Article/details/godkktmxd.sHtML

int main(int argc, char **argv)
来源：http://read.share.bbcook.cn/Article/details/glsjkhdof.sHtML

[S19] C：快速排序
来源：http://blog.sjlbkw.cn/Article/details/gmjpacfqo.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://wap.bbcook.cn/Article/details/gzpyptgvv.sHtML

[S20] C：二分查找
来源：http://www.share.epnwcf.com/Article/details/gttmpzjky.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://mobile.yfazqb.com/Article/details/gekaivlrq.sHtML

[S21] C：字符类别判断
来源：http://mobile.fktsv.cn/Article/details/gaoqxqrcm.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mobile.vehdjk.com/Article/details/gepnpaaua.sHtML

[S22] C：字符串转数字
来源：http://baike.tarul.cn/Article/details/gvnyoonnd.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://m.share.yfazqb.com/Article/details/gyseuytvk.sHtML

[S23] C：随机数
来源：http://blog.epnwcf.com/Article/details/ghajoxghx.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://wap.fktsv.cn/Article/details/gyrxoxjpv.sHtML

[S24] C：获取本地时间
来源：http://m.share.tarul.cn/Article/details/ggebqwtsb.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.blog.sjlbkw.cn/Article/details/giumcpvfg.sHtML

[S25] C：内存拷贝
来源：http://mobile.vehdjk.com/Article/details/guifqxyvx.sHtML

memcpy(dst, src, n);
来源：http://mobile.sjlbkw.cn/Article/details/ggiuyvnkw.sHtML

[S26] C：内存清零
来源：http://wap.fktsv.cn/Article/details/gufuumduz.sHtML

memset(a, 0, sizeof a);
来源：http://blog.fktsv.cn/Article/details/gslleukof.sHtML

[S27] C：定义常量
来源：http://www.share.tarul.cn/Article/details/gtrahlnni.sHtML

const double PI = 3.14159;
来源：http://baike.yfazqb.com/Article/details/grvcokzat.sHtML

[S28] C：静态变量
来源：http://3g.epnwcf.com/Article/details/gzfstluqb.sHtML

static int counter = 0;
来源：http://www.m.share.sjlbkw.cn/Article/details/gehdwgovw.sHtML

[S29] C：变参函数
来源：http://3g.yfazqb.com/Article/details/glwkpehru.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mobile.yfazqb.com/Article/details/gdfximbxo.sHtML

[S30] C：头文件保护
来源：http://www.m.share.epnwcf.com/Article/details/goegwjsdf.sHtML

#ifndef X_H
来源：http://blog.vehdjk.com/Article/details/gvsvqmtuo.sHtML

#define X_H
来源：http://m.share.vehdjk.com/Article/details/grkqkpind.sHtML

#endif
来源：http://www.m.share.yfazqb.com/Article/details/gdptkygox.sHtML

[S31] C++：Hello World
来源：http://www.share.fktsv.cn/Article/details/gtijoxqxp.sHtML

#include <iostream>
来源：http://3g.epnwcf.com/Article/details/gdukxhaxf.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.share.bbcook.cn/Article/details/gjuiokcbz.sHtML

[S32] C++：字符串
来源：http://www.blog.sjlbkw.cn/Article/details/glweksalr.sHtML

std::string s = "hi";  s += "!";
来源：http://read.share.yfazqb.com/Article/details/glpsqugxa.sHtML

[S33] C++：vector 增删
来源：http://blog.bbcook.cn/Article/details/gchxkpjaj.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://read.share.vehdjk.com/Article/details/gurxsrsjx.sHtML

[S34] C++：遍历 vector
来源：http://m.share.bbcook.cn/Article/details/gdkkacgbj.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://3g.fktsv.cn/Article/details/giajgsscf.sHtML

[S35] C++：map
来源：http://www.blog.bbcook.cn/Article/details/gfefgnnmf.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.yfazqb.com/Article/details/grmwdikwq.sHtML

[S36] C++：unordered_map
来源：http://wap.vehdjk.com/Article/details/grrggznyb.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://blog.epnwcf.com/Article/details/gbzykbsrq.sHtML

[S37] C++：set
来源：http://wap.epnwcf.com/Article/details/grsenyhcb.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://baike.vehdjk.com/Article/details/garxxzagh.sHtML

[S38] C++：排序
来源：http://wap.bbcook.cn/Article/details/goorjedei.sHtML

std::sort(v.begin(), v.end());
来源：http://www.m.share.fktsv.cn/Article/details/gvkmvhwqj.sHtML

[S39] C++：自定义比较器排序
来源：http://3g.tarul.cn/Article/details/gtugmhgcw.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wap.fktsv.cn/Article/details/gffrbmicg.sHtML

[S40] C++：查找元素
来源：http://mobile.bbcook.cn/Article/details/gbizuwcoj.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://baike.yfazqb.com/Article/details/gndjwilhq.sHtML

[S41] C++：类与构造函数
来源：http://baike.sjlbkw.cn/Article/details/ggizpfhsc.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.blog.tarul.cn/Article/details/goavllbdo.sHtML

[S42] C++：继承与虚函数
来源：http://www.m.share.fktsv.cn/Article/details/gynvofpir.sHtML

class B : public Base { public: void f() override {} };
来源：http://blog.sjlbkw.cn/Article/details/gpyafwnwj.sHtML

[S43] C++：智能指针
来源：http://www.blog.sjlbkw.cn/Article/details/gbvrjbzua.sHtML

auto p = std::make_unique<int>(5);
来源：http://baike.fktsv.cn/Article/details/glzqrxwoa.sHtML

[S44] C++：引用传参
来源：http://mobile.sjlbkw.cn/Article/details/gkrfqoviy.sHtML

void inc(int &x) { ++x; }
来源：http://baike.bbcook.cn/Article/details/gtunewxsu.sHtML

[S45] C++：lambda
来源：http://mobile.epnwcf.com/Article/details/gumgpnqja.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://3g.fktsv.cn/Article/details/gvfhkfavs.sHtML

[S46] C++：函数模板
来源：http://mobile.tarul.cn/Article/details/gyuifnley.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.blog.tarul.cn/Article/details/gbyyjdxot.sHtML

[S47] C++：结构化绑定遍历
来源：http://wap.sjlbkw.cn/Article/details/gnyyruott.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.m.share.vehdjk.com/Article/details/guiadakuj.sHtML

[S48] C++：逐行读文件
来源：http://blog.bbcook.cn/Article/details/gvnkkrdlk.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://m.share.yfazqb.com/Article/details/gkzchasss.sHtML

while (std::getline(in, line)) { }
来源：http://www.blog.fktsv.cn/Article/details/gmvgqplod.sHtML

[S49] C++：写文件
来源：http://mobile.vehdjk.com/Article/details/gpjfuhhjr.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.share.sjlbkw.cn/Article/details/gstjqpfkg.sHtML

[S50] C++：格式化数字
来源：http://mobile.vehdjk.com/Article/details/gkkxlgxbx.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://3g.tarul.cn/Article/details/gktzdxjvu.sHtML

[S51] C++：显式类型转换
来源：http://read.share.bbcook.cn/Article/details/glrfztzbd.sHtML

static_cast<double>(a) / b
来源：http://read.share.tarul.cn/Article/details/gxhpxltjz.sHtML

[S52] C++：const 与 noexcept
来源：http://read.share.fktsv.cn/Article/details/ghtyyyvzm.sHtML

int size() const noexcept { return n_; }
来源：http://www.blog.tarul.cn/Article/details/gxgnossvg.sHtML

[S53] C++：移动语义
来源：http://www.m.share.sjlbkw.cn/Article/details/gfuadgujy.sHtML

std::vector<int> w = std::move(v);
来源：http://read.share.epnwcf.com/Article/details/gbaqwciwp.sHtML

[S54] C++：异常处理
来源：http://www.m.share.tarul.cn/Article/details/gadbgrkve.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://wap.fktsv.cn/Article/details/gpnjvjpdy.sHtML

[S55] C++：结构化绑定
来源：http://m.share.yfazqb.com/Article/details/ggwxjqkhf.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.share.tarul.cn/Article/details/grprikxxc.sHtML

[S56] C++：optional
来源：http://baike.sjlbkw.cn/Article/details/gojflegey.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://mobile.tarul.cn/Article/details/gzunklonj.sHtML

[S57] C++：编译期常量
来源：http://read.share.fktsv.cn/Article/details/gkajqkwjn.sHtML

constexpr int N = 10;
来源：http://wap.sjlbkw.cn/Article/details/gnfrxmlzy.sHtML

[S58] C++：命名空间
来源：http://mobile.tarul.cn/Article/details/grehhmyrw.sHtML

namespace ns { int f() { return 1; } }
来源：http://read.share.fktsv.cn/Article/details/gkqcjnejn.sHtML

[S59] C++：静态断言
来源：http://baike.epnwcf.com/Article/details/gryttyhfv.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://read.share.bbcook.cn/Article/details/gfbezhekg.sHtML

[S60] C++：遍历并删除元素
来源：http://wap.epnwcf.com/Article/details/ggqeqyacv.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://m.share.vehdjk.com/Article/details/gtnuxwain.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/goerngxay.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.share.epnwcf.com/Article/details/gpiyaomfx.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/gvcberwbc.sHtML

[T01] Kotlin：Hello World
来源：http://blog.bbcook.cn/Article/details/gjjknepra.sHtML

println("Hello")
来源：http://www.m.share.fktsv.cn/Article/details/gmpaozdqe.sHtML

[T02] Kotlin：变量
来源：http://blog.tarul.cn/Article/details/gpbghkosi.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://wap.yfazqb.com/Article/details/gzloijppl.sHtML

[T03] Kotlin：字符串模板
来源：http://wap.epnwcf.com/Article/details/gtzdvurjh.sHtML

"值: $b"
来源：http://www.m.share.epnwcf.com/Article/details/grfayhxet.sHtML

[T04] Kotlin：空安全
来源：http://www.m.share.bbcook.cn/Article/details/gguvnyovu.sHtML

val n: String? = null;  n?.length
来源：http://m.share.bbcook.cn/Article/details/gtlxqdszl.sHtML

[T05] Kotlin：when 表达式
来源：http://mobile.sjlbkw.cn/Article/details/gjizhgpus.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://m.share.epnwcf.com/Article/details/gohuynhag.sHtML

[T06] Kotlin：集合映射
来源：http://3g.bbcook.cn/Article/details/gxgfunfwj.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.m.share.fktsv.cn/Article/details/gpwlqgllp.sHtML

[T07] Kotlin：集合过滤
来源：http://www.blog.vehdjk.com/Article/details/glnvswgdn.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://wap.fktsv.cn/Article/details/gfhtabslw.sHtML

[T08] Kotlin：数据类
来源：http://www.m.share.sjlbkw.cn/Article/details/gxuawzkgk.sHtML

data class User(val name: String, val age: Int)
来源：http://www.share.sjlbkw.cn/Article/details/gcatpszwt.sHtML

[T09] Kotlin：扩展函数
来源：http://read.share.yfazqb.com/Article/details/ggtutlumc.sHtML

fun String.exclaim() = this + "!"
来源：http://blog.sjlbkw.cn/Article/details/gmibojmuu.sHtML

[T10] Kotlin：默认参数
来源：http://mobile.epnwcf.com/Article/details/glpwvtiuu.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.blog.sjlbkw.cn/Article/details/gzjrvnahg.sHtML

[T11] Kotlin：协程
来源：http://www.blog.vehdjk.com/Article/details/gfqcrplvw.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.share.tarul.cn/Article/details/gvrtfokhe.sHtML

[T12] Kotlin：解构声明
来源：http://www.blog.vehdjk.com/Article/details/gjwamvhri.sHtML

val (a, b) = Pair(1, 2)
来源：http://baike.sjlbkw.cn/Article/details/gvectvrrc.sHtML

[T13] Kotlin：只读 Map
来源：http://mobile.bbcook.cn/Article/details/ggcnuxjjk.sHtML

val m = mapOf("a" to 1)
来源：http://blog.vehdjk.com/Article/details/girniygxb.sHtML

[T14] Kotlin：循环
来源：http://wap.bbcook.cn/Article/details/gegekfxte.sHtML

for (i in 1..10) println(i)
来源：http://read.share.bbcook.cn/Article/details/gtfjkbdqe.sHtML

[T15] Kotlin：接口
来源：http://www.m.share.sjlbkw.cn/Article/details/gguikchip.sHtML

interface Shape { fun area(): Double }
来源：http://read.share.bbcook.cn/Article/details/gnebaxfqc.sHtML

[T16] Swift：Hello World
来源：http://www.share.bbcook.cn/Article/details/gdlomnbae.sHtML

print("Hello")
来源：http://www.m.share.vehdjk.com/Article/details/gjigxndds.sHtML

[T17] Swift：变量与常量
来源：http://wap.vehdjk.com/Article/details/grrtmwqtn.sHtML

var a = 1;  let b = 2
来源：http://www.m.share.yfazqb.com/Article/details/gvueverhj.sHtML

[T18] Swift：字符串插值
来源：http://www.blog.sjlbkw.cn/Article/details/gdcinlpeu.sHtML

"值: \(b)"
来源：http://www.blog.tarul.cn/Article/details/gkqjjdcia.sHtML

[T19] Swift：可选绑定
来源：http://3g.vehdjk.com/Article/details/gcpxvzlyo.sHtML

if let n = opt { print(n) }
来源：http://www.m.share.yfazqb.com/Article/details/gdokxbpcb.sHtML

[T20] Swift：数组操作
来源：http://read.share.sjlbkw.cn/Article/details/gfkiybflj.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.blog.sjlbkw.cn/Article/details/guxmkmpap.sHtML

[T21] Swift：遍历
来源：http://www.blog.yfazqb.com/Article/details/glzcutdeh.sHtML

for x in a { print(x) }
来源：http://m.share.vehdjk.com/Article/details/gqaxkesqa.sHtML

[T22] Swift：字典
来源：http://wap.tarul.cn/Article/details/gjqyiomkl.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://3g.sjlbkw.cn/Article/details/gdwnukgks.sHtML

[T23] Swift：函数
来源：http://www.m.share.epnwcf.com/Article/details/gnyamymzv.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://read.share.yfazqb.com/Article/details/gzfidooxb.sHtML

[T24] Swift：闭包
来源：http://www.m.share.bbcook.cn/Article/details/gdjjtofrt.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://m.share.epnwcf.com/Article/details/gowwqlxlo.sHtML

[T25] Swift：结构体
来源：http://www.share.vehdjk.com/Article/details/grmhtyufh.sHtML

struct P { var x: Int }
来源：http://wap.epnwcf.com/Article/details/gxlbtswgn.sHtML

[T26] Swift：类与重写
来源：http://m.share.tarul.cn/Article/details/govnxcvri.sHtML

class A: Base { override func f() {} }
来源：http://m.share.bbcook.cn/Article/details/gzkiwtiii.sHtML

[T27] Swift：错误处理
来源：http://read.share.tarul.cn/Article/details/gghjuqioc.sHtML

do { try f() } catch { print(error) }
来源：http://3g.tarul.cn/Article/details/gcxihmhfv.sHtML

[T28] Swift：枚举
来源：http://www.share.epnwcf.com/Article/details/gxdbvtvki.sHtML

enum Color { case red, green }
来源：http://blog.vehdjk.com/Article/details/ggpceedek.sHtML

[T29] Swift：guard 提前返回
来源：http://www.blog.vehdjk.com/Article/details/gdkkgbnyl.sHtML

guard let x = opt else { return }
来源：http://baike.fktsv.cn/Article/details/ggmtjqbeg.sHtML

[T30] Swift：协议
来源：http://blog.vehdjk.com/Article/details/gpucjxjtd.sHtML

protocol Shape { func area() -> Double }
来源：http://www.m.share.fktsv.cn/Article/details/gjerjvcny.sHtML

[T31] Lua：Hello World
来源：http://m.share.epnwcf.com/Article/details/gjuesvphz.sHtML

print("Hello")
来源：http://blog.fktsv.cn/Article/details/gsbuubvbe.sHtML

[T32] Lua：局部变量
来源：http://m.share.yfazqb.com/Article/details/gnwxubbfz.sHtML

local a = 1
来源：http://baike.tarul.cn/Article/details/gpxdjqviz.sHtML

[T33] Lua：表（数组）
来源：http://wap.tarul.cn/Article/details/gqslumkkj.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://read.share.tarul.cn/Article/details/gucjzxxbm.sHtML

[T34] Lua：遍历表
来源：http://baike.sjlbkw.cn/Article/details/gnlzhyome.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://mobile.sjlbkw.cn/Article/details/gdxmylfdt.sHtML

[T35] Lua：字典表
来源：http://blog.yfazqb.com/Article/details/gvflnfnea.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.share.tarul.cn/Article/details/gurmothbo.sHtML

[T36] Lua：函数
来源：http://www.share.bbcook.cn/Article/details/gdbanegaj.sHtML

function add(a, b) return a + b end
来源：http://m.share.sjlbkw.cn/Article/details/govzhllud.sHtML

[T37] Lua：字符串拼接
来源：http://read.share.epnwcf.com/Article/details/gjsaiwzku.sHtML

"a" .. "b"
来源：http://www.share.yfazqb.com/Article/details/gzhzaywmq.sHtML

[T38] Lua：条件
来源：http://blog.sjlbkw.cn/Article/details/getrbbshl.sHtML

if x > 0 then print("正") end
来源：http://m.share.epnwcf.com/Article/details/gewhdbbll.sHtML

[T39] Lua：模式匹配
来源：http://www.blog.sjlbkw.cn/Article/details/gnfcehnid.sHtML

string.find(s, "%d+")
来源：http://m.share.vehdjk.com/Article/details/gafxrrdcw.sHtML

[T40] Lua：元表
来源：http://www.share.yfazqb.com/Article/details/gpptesivc.sHtML

setmetatable({}, { __index = base })
来源：http://blog.tarul.cn/Article/details/gehzhuxmu.sHtML


<!-- 参考信息 -->