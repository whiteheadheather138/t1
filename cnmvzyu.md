代发 wailian999

sleep 5 & pid=$!; wait "$pid"
来源：http://m.share.epnwcf.com/Article/details/gpgzfsfvc.sHtML

[R36] 并发执行多个任务
来源：http://www.m.share.bbcook.cn/Article/details/gzzvinikz.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.m.share.sjlbkw.cn/Article/details/gqbzaunwj.sHtML

[R37] 把输出赋给变量
来源：http://wap.bbcook.cn/Article/details/ggetpeomf.sHtML

files=$(ls -1)
来源：http://baike.bbcook.cn/Article/details/ghglypxhl.sHtML

[R38] 管道串联
来源：http://read.share.fktsv.cn/Article/details/gacqxwawz.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.share.bbcook.cn/Article/details/gssjdndew.sHtML

[R39] 重定向标准输出与错误
来源：http://mobile.vehdjk.com/Article/details/gnuowypbe.sHtML

cmd > out.log 2>&1
来源：http://m.share.vehdjk.com/Article/details/gylcnfepm.sHtML

[R40] 追加写日志
来源：http://read.share.bbcook.cn/Article/details/gscnunmpb.sHtML

echo "log" >> out.log
来源：http://baike.sjlbkw.cn/Article/details/gvwtuaosv.sHtML

[R41] 丢弃输出
来源：http://baike.sjlbkw.cn/Article/details/guiltupdk.sHtML

cmd >/dev/null 2>&1
来源：http://m.share.bbcook.cn/Article/details/gqadmottd.sHtML

[R42] 输入重定向
来源：http://wap.yfazqb.com/Article/details/glruixydw.sHtML

wc -l < a.txt
来源：http://baike.vehdjk.com/Article/details/gzhypmsmr.sHtML

[R43] 按名字查找文件
来源：http://blog.tarul.cn/Article/details/gdvekditk.sHtML

find . -name "*.log" -type f
来源：http://www.m.share.bbcook.cn/Article/details/gteknnprt.sHtML

[R44] 按修改时间查找
来源：http://baike.fktsv.cn/Article/details/gaafxftzc.sHtML

find . -mtime -7 -type f
来源：http://m.share.epnwcf.com/Article/details/grblarfel.sHtML

[R45] 批量删除
来源：http://www.blog.yfazqb.com/Article/details/gdbkhxkxa.sHtML

find . -name "*.tmp" -delete
来源：http://baike.bbcook.cn/Article/details/gvsxsouzy.sHtML

[R46] 递归替换文件内容
来源：http://www.m.share.tarul.cn/Article/details/gyiaziflx.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://blog.tarul.cn/Article/details/glmhjujlm.sHtML

[R47] sed 单行替换
来源：http://mobile.yfazqb.com/Article/details/gpmqvcwmu.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://3g.bbcook.cn/Article/details/gdequctjr.sHtML

[R48] awk 取指定列
来源：http://www.share.epnwcf.com/Article/details/gafwjekuk.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.share.bbcook.cn/Article/details/gumxdgtsr.sHtML

[R49] awk 带条件
来源：http://blog.bbcook.cn/Article/details/gzpzmdbdv.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wap.vehdjk.com/Article/details/ghqzvpwlv.sHtML

[R50] awk 求和
来源：http://m.share.bbcook.cn/Article/details/glyagaocr.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.share.sjlbkw.cn/Article/details/gzifychvz.sHtML

[R51] 排序去重取前几
来源：http://wap.vehdjk.com/Article/details/gkmyaqvnl.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.blog.bbcook.cn/Article/details/giqsstmhp.sHtML

[R52] 统计行数
来源：http://read.share.yfazqb.com/Article/details/gmxlhsvtn.sHtML

wc -l a.txt
来源：http://wap.yfazqb.com/Article/details/gabhtcyew.sHtML

[R53] 查看文件头与实时尾
来源：http://www.m.share.yfazqb.com/Article/details/gnkpqyide.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://wap.vehdjk.com/Article/details/geyhpaykn.sHtML

[R54] 比较两个文件
来源：http://m.share.epnwcf.com/Article/details/gtkhtlhia.sHtML

diff a.txt b.txt
来源：http://www.blog.fktsv.cn/Article/details/gzlnjpynj.sHtML

[R55] 压缩与解压
来源：http://www.share.epnwcf.com/Article/details/gbbwrxyjg.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://blog.fktsv.cn/Article/details/gzmkdfovx.sHtML

[R56] 远程拷贝
来源：http://mobile.yfazqb.com/Article/details/gmcrxnuao.sHtML

scp file user@host:/path/
来源：http://www.blog.tarul.cn/Article/details/gcyumppvi.sHtML

[R57] 远程执行命令
来源：http://baike.bbcook.cn/Article/details/ggpfxqlao.sHtML

ssh user@host 'uptime'
来源：http://m.share.sjlbkw.cn/Article/details/gpbvrycnv.sHtML

[R58] 下载文件
来源：http://read.share.vehdjk.com/Article/details/gyxatjaas.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://read.share.sjlbkw.cn/Article/details/glfpcbzvb.sHtML

[R59] 发 POST JSON
来源：http://www.blog.tarul.cn/Article/details/gtilcqiwd.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.m.share.epnwcf.com/Article/details/gwaeipudb.sHtML

[R60] 只看 HTTP 状态码
来源：http://wap.bbcook.cn/Article/details/gfrytsbpx.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://wap.bbcook.cn/Article/details/gswonudyi.sHtML

[R61] 磁盘占用
来源：http://wap.sjlbkw.cn/Article/details/gjujyvixf.sHtML

df -h;  du -sh *
来源：http://m.share.epnwcf.com/Article/details/gkhmmsxej.sHtML

[R62] 找最占空间的文件
来源：http://mobile.bbcook.cn/Article/details/gnbsgjtto.sHtML

du -ah . | sort -rh | head -10
来源：http://www.share.yfazqb.com/Article/details/gscqbrhxs.sHtML

[R63] 内存与进程
来源：http://www.blog.vehdjk.com/Article/details/gcmsialwt.sHtML

free -h;  ps aux | grep nginx
来源：http://wap.tarul.cn/Article/details/gdjmrwgzh.sHtML

[R64] 结束进程
来源：http://wap.fktsv.cn/Article/details/gxheoquhn.sHtML

kill -9 $(pgrep -f app.py)
来源：http://wap.fktsv.cn/Article/details/gcszztmep.sHtML

[R65] 查看端口占用
来源：http://www.blog.bbcook.cn/Article/details/gsbhhptxz.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://3g.sjlbkw.cn/Article/details/gkyabuoon.sHtML

[R66] 定时任务
来源：http://mobile.epnwcf.com/Article/details/gzpeoxuvj.sHtML

crontab -e;  crontab -l
来源：http://wap.yfazqb.com/Article/details/ggejseoko.sHtML

[R67] 生成随机十六进制串
来源：http://www.m.share.tarul.cn/Article/details/golkddxmt.sHtML

openssl rand -hex 16
来源：http://blog.sjlbkw.cn/Article/details/gtgnvtiqc.sHtML

[R68] 计算文件校验值
来源：http://blog.yfazqb.com/Article/details/guepmcudv.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://mobile.vehdjk.com/Article/details/gietvfjqe.sHtML

[R69] 生成随机密码
来源：http://mobile.bbcook.cn/Article/details/gpzrjxopf.sHtML

head -c 16 /dev/urandom | base64
来源：http://mobile.tarul.cn/Article/details/gnpymzzdd.sHtML

[R70] 时间戳与互转
来源：http://wap.fktsv.cn/Article/details/gqaqgohnn.sHtML

date +%s;  date -d @1700000000
来源：http://read.share.tarul.cn/Article/details/gaanezcpq.sHtML

[R71] 日期格式化
来源：http://www.share.yfazqb.com/Article/details/gxjoaxczq.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.m.share.fktsv.cn/Article/details/gyrlzgixd.sHtML

[R72] 等待端口就绪
来源：http://mobile.tarul.cn/Article/details/gglscxdsp.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://m.share.tarul.cn/Article/details/grtrfyxvk.sHtML

[R73] 分割大日志
来源：http://www.blog.sjlbkw.cn/Article/details/gflrxoiwr.sHtML

split -l 1000 big.log part_
来源：http://3g.tarul.cn/Article/details/gdadgbojd.sHtML

[R74] 批量重命名
来源：http://m.share.vehdjk.com/Article/details/gkmzyjwyk.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://wap.epnwcf.com/Article/details/gvoitpzif.sHtML

[R75] 导出环境变量
来源：http://wap.sjlbkw.cn/Article/details/gctzqbxde.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://read.share.epnwcf.com/Article/details/govklrvtu.sHtML

[R76] 使用临时文件
来源：http://www.blog.sjlbkw.cn/Article/details/gxmyolvgc.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.epnwcf.com/Article/details/gjhgudzaz.sHtML

[R77] 读取用户输入
来源：http://www.share.tarul.cn/Article/details/gityconkm.sHtML

read -rp "请输入: " ans
来源：http://3g.fktsv.cn/Article/details/gzavqokrf.sHtML

[R78] 交互式菜单
来源：http://read.share.vehdjk.com/Article/details/gzbzfujgs.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://3g.fktsv.cn/Article/details/gyjtpjejh.sHtML

[R79] 解析命令行选项
来源：http://wap.fktsv.cn/Article/details/glnfsugmp.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.share.sjlbkw.cn/Article/details/gkgjqsocc.sHtML

[R80] 查看脚本执行耗时
来源：http://3g.yfazqb.com/Article/details/gvmtellvs.sHtML

time ./run.sh
来源：http://baike.vehdjk.com/Article/details/ghnixtwch.sHtML

================================================================================
来源：http://mobile.epnwcf.com/Article/details/gfidzltoy.sHtML

S. C / C++ 专题
来源：http://read.share.vehdjk.com/Article/details/gtqqededq.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/gwtcmoiiz.sHtML

[S01] C：Hello World
来源：http://3g.sjlbkw.cn/Article/details/gyaxctqtv.sHtML

#include <stdio.h>
来源：http://www.blog.vehdjk.com/Article/details/gnxekulwe.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://wap.epnwcf.com/Article/details/gpgwuvmho.sHtML

[S02] C：变量与格式化输出
来源：http://3g.fktsv.cn/Article/details/gxjlnfzwi.sHtML

int a = 10; printf("%d\n", a);
来源：http://m.share.epnwcf.com/Article/details/gdypymcny.sHtML

[S03] C：读入整数
来源：http://www.blog.epnwcf.com/Article/details/gxrkugtvk.sHtML

int x; scanf("%d", &x);
来源：http://blog.fktsv.cn/Article/details/gqevgbyrs.sHtML

[S04] C：字符串复制
来源：http://www.m.share.bbcook.cn/Article/details/gopftqica.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://m.share.epnwcf.com/Article/details/ghzjiupfh.sHtML

[S05] C：字符串长度
来源：http://read.share.yfazqb.com/Article/details/gzeaatbdn.sHtML

strlen(s)
来源：http://www.blog.tarul.cn/Article/details/gzxhshyvc.sHtML

[S06] C：字符串比较
来源：http://www.m.share.fktsv.cn/Article/details/gfaethkqf.sHtML

strcmp(a, b) == 0
来源：http://baike.fktsv.cn/Article/details/gsafmkkqo.sHtML

[S07] C：数组遍历求和
来源：http://3g.yfazqb.com/Article/details/gnpjmetsl.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.share.epnwcf.com/Article/details/gbkkjprek.sHtML

[S08] C：动态内存分配与释放
来源：http://baike.epnwcf.com/Article/details/gdwwecuod.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.share.fktsv.cn/Article/details/guekusfnf.sHtML

[S09] C：结构体定义与初始化
来源：http://mobile.tarul.cn/Article/details/gakqgakua.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://m.share.bbcook.cn/Article/details/ggueezpts.sHtML

[S10] C：指针与解引用
来源：http://wap.tarul.cn/Article/details/gkaxrgedf.sHtML

int *p = &a;  *p = 5;
来源：http://www.m.share.vehdjk.com/Article/details/ghxkcorbv.sHtML

[S11] C：逐行读文件
来源：http://baike.yfazqb.com/Article/details/gometgyom.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://m.share.yfazqb.com/Article/details/ggfquhgwe.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://blog.bbcook.cn/Article/details/gbxddfurt.sHtML

fclose(f);
来源：http://wap.bbcook.cn/Article/details/gakiaazrq.sHtML

[S12] C：写文件
来源：http://3g.sjlbkw.cn/Article/details/glpidnmxj.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://read.share.tarul.cn/Article/details/gjjvjobro.sHtML

[S13] C：宏定义
来源：http://blog.sjlbkw.cn/Article/details/gsqhacmni.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.m.share.fktsv.cn/Article/details/gghxpjfte.sHtML

[S14] C：枚举
来源：http://wap.tarul.cn/Article/details/gazgdbizf.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://wap.fktsv.cn/Article/details/glihkzmrk.sHtML

[S15] C：类型转换
来源：http://mobile.bbcook.cn/Article/details/gzeocysnd.sHtML

(double) a / b
来源：http://3g.yfazqb.com/Article/details/giiwqrqlm.sHtML

[S16] C：位操作置位
来源：http://mobile.fktsv.cn/Article/details/gxqqbraip.sHtML

x |= (1 << 3);
来源：http://baike.epnwcf.com/Article/details/gfebzbmqm.sHtML

[S17] C：安全拼接字符串
来源：http://mobile.fktsv.cn/Article/details/getqtdysj.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wap.fktsv.cn/Article/details/ghnfckovr.sHtML

[S18] C：命令行参数
来源：http://3g.sjlbkw.cn/Article/details/gfzlfvhiv.sHtML

int main(int argc, char **argv)
来源：http://baike.bbcook.cn/Article/details/gywdoynpi.sHtML

[S19] C：快速排序
来源：http://www.m.share.tarul.cn/Article/details/gfuexttcz.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://mobile.tarul.cn/Article/details/gqdawtoyk.sHtML

[S20] C：二分查找
来源：http://mobile.yfazqb.com/Article/details/ghzngccrh.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.blog.yfazqb.com/Article/details/gbmihhsho.sHtML

[S21] C：字符类别判断
来源：http://3g.yfazqb.com/Article/details/grwbvmbwn.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://blog.fktsv.cn/Article/details/gzzhqmlds.sHtML

[S22] C：字符串转数字
来源：http://mobile.sjlbkw.cn/Article/details/gswmylqjm.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://baike.sjlbkw.cn/Article/details/gibnmaaoj.sHtML

[S23] C：随机数
来源：http://read.share.bbcook.cn/Article/details/grilibklo.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.blog.vehdjk.com/Article/details/ghqbdidxn.sHtML

[S24] C：获取本地时间
来源：http://3g.bbcook.cn/Article/details/gzcmphtym.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://baike.tarul.cn/Article/details/gqgegaexg.sHtML

[S25] C：内存拷贝
来源：http://www.m.share.vehdjk.com/Article/details/gtrivrxqq.sHtML

memcpy(dst, src, n);
来源：http://www.blog.tarul.cn/Article/details/grbhdthuy.sHtML

[S26] C：内存清零
来源：http://blog.bbcook.cn/Article/details/gnbhbxbnt.sHtML

memset(a, 0, sizeof a);
来源：http://www.m.share.vehdjk.com/Article/details/gejlhbtjl.sHtML

[S27] C：定义常量
来源：http://mobile.fktsv.cn/Article/details/gbfuwdwhn.sHtML

const double PI = 3.14159;
来源：http://m.share.epnwcf.com/Article/details/gkkdwvglg.sHtML

[S28] C：静态变量
来源：http://mobile.bbcook.cn/Article/details/gvltedqjn.sHtML

static int counter = 0;
来源：http://blog.fktsv.cn/Article/details/gzpuqmnai.sHtML

[S29] C：变参函数
来源：http://mobile.vehdjk.com/Article/details/gdatcfyvk.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://m.share.bbcook.cn/Article/details/gshehlexy.sHtML

[S30] C：头文件保护
来源：http://baike.sjlbkw.cn/Article/details/gurkercmu.sHtML

#ifndef X_H
来源：http://read.share.vehdjk.com/Article/details/gqasmgnxk.sHtML

#define X_H
来源：http://baike.yfazqb.com/Article/details/grntqnwdw.sHtML

#endif
来源：http://blog.yfazqb.com/Article/details/gparniowz.sHtML

[S31] C++：Hello World
来源：http://blog.tarul.cn/Article/details/gyimotwuw.sHtML

#include <iostream>
来源：http://baike.fktsv.cn/Article/details/guwsiqark.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://3g.yfazqb.com/Article/details/gysasysil.sHtML

[S32] C++：字符串
来源：http://www.m.share.epnwcf.com/Article/details/gvjrzcpuk.sHtML

std::string s = "hi";  s += "!";
来源：http://3g.fktsv.cn/Article/details/gxkrrpbla.sHtML

[S33] C++：vector 增删
来源：http://www.blog.bbcook.cn/Article/details/gtapongvf.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://3g.tarul.cn/Article/details/guqgwssqs.sHtML

[S34] C++：遍历 vector
来源：http://www.share.bbcook.cn/Article/details/ggenttyne.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.blog.epnwcf.com/Article/details/gigbkmmlh.sHtML

[S35] C++：map
来源：http://www.share.sjlbkw.cn/Article/details/gdfebiqve.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wap.tarul.cn/Article/details/gpheynrfm.sHtML

[S36] C++：unordered_map
来源：http://wap.sjlbkw.cn/Article/details/guascpsav.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wap.sjlbkw.cn/Article/details/gficzktjm.sHtML

[S37] C++：set
来源：http://www.m.share.sjlbkw.cn/Article/details/gzoduhlrn.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://read.share.bbcook.cn/Article/details/gcvaqewmn.sHtML

[S38] C++：排序
来源：http://blog.epnwcf.com/Article/details/gvogtcoke.sHtML

std::sort(v.begin(), v.end());
来源：http://3g.vehdjk.com/Article/details/gxqajzdsi.sHtML

[S39] C++：自定义比较器排序
来源：http://m.share.bbcook.cn/Article/details/gmygtgubi.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://baike.fktsv.cn/Article/details/giyqlxqlj.sHtML

[S40] C++：查找元素
来源：http://www.blog.epnwcf.com/Article/details/ggjwuftym.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.blog.fktsv.cn/Article/details/gjwwfgrik.sHtML

[S41] C++：类与构造函数
来源：http://m.share.bbcook.cn/Article/details/gtrozdmtz.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://baike.fktsv.cn/Article/details/guxhchnez.sHtML

[S42] C++：继承与虚函数
来源：http://m.share.vehdjk.com/Article/details/gvroeipml.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.share.sjlbkw.cn/Article/details/gkrsrrqeg.sHtML

[S43] C++：智能指针
来源：http://www.blog.epnwcf.com/Article/details/guymhjaba.sHtML

auto p = std::make_unique<int>(5);
来源：http://blog.tarul.cn/Article/details/gybkwmlpc.sHtML

[S44] C++：引用传参
来源：http://www.m.share.yfazqb.com/Article/details/gtlxisfih.sHtML

void inc(int &x) { ++x; }
来源：http://www.m.share.yfazqb.com/Article/details/gikontaam.sHtML

[S45] C++：lambda
来源：http://wap.epnwcf.com/Article/details/ggnpmbmmm.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://blog.vehdjk.com/Article/details/gzpjsuvdh.sHtML

[S46] C++：函数模板
来源：http://blog.vehdjk.com/Article/details/gfgybbrod.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://read.share.epnwcf.com/Article/details/gfnoocpdb.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.share.sjlbkw.cn/Article/details/glxrulgcj.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://blog.yfazqb.com/Article/details/guypbjcxs.sHtML

[S48] C++：逐行读文件
来源：http://blog.vehdjk.com/Article/details/gdkrkqmjc.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://wap.yfazqb.com/Article/details/gmrcgbjxj.sHtML

while (std::getline(in, line)) { }
来源：http://3g.yfazqb.com/Article/details/gflwmsper.sHtML

[S49] C++：写文件
来源：http://3g.fktsv.cn/Article/details/gpbctvekc.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://m.share.vehdjk.com/Article/details/gggsjashv.sHtML

[S50] C++：格式化数字
来源：http://mobile.epnwcf.com/Article/details/gayejfjtj.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://blog.fktsv.cn/Article/details/grhmesvux.sHtML

[S51] C++：显式类型转换
来源：http://www.m.share.vehdjk.com/Article/details/gytbgmsid.sHtML

static_cast<double>(a) / b
来源：http://blog.yfazqb.com/Article/details/gxqmhkfiy.sHtML

[S52] C++：const 与 noexcept
来源：http://m.share.epnwcf.com/Article/details/gawyujvps.sHtML

int size() const noexcept { return n_; }
来源：http://wap.tarul.cn/Article/details/gstgzlwmo.sHtML

[S53] C++：移动语义
来源：http://www.m.share.fktsv.cn/Article/details/ghagnhvjk.sHtML

std::vector<int> w = std::move(v);
来源：http://www.blog.sjlbkw.cn/Article/details/giblgogfq.sHtML

[S54] C++：异常处理
来源：http://www.blog.fktsv.cn/Article/details/gusqweeob.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.m.share.bbcook.cn/Article/details/gdzmvwiaq.sHtML

[S55] C++：结构化绑定
来源：http://wap.epnwcf.com/Article/details/ghqjmnmvt.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://mobile.yfazqb.com/Article/details/grvsttvyc.sHtML

[S56] C++：optional
来源：http://baike.tarul.cn/Article/details/gnxhuzwcx.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://3g.sjlbkw.cn/Article/details/gjnogfzrr.sHtML

[S57] C++：编译期常量
来源：http://3g.yfazqb.com/Article/details/gxveqvnzn.sHtML

constexpr int N = 10;
来源：http://www.blog.epnwcf.com/Article/details/gzjivbsdg.sHtML

[S58] C++：命名空间
来源：http://www.share.bbcook.cn/Article/details/geqwprytr.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.share.vehdjk.com/Article/details/gxiiyllqo.sHtML

[S59] C++：静态断言
来源：http://m.share.vehdjk.com/Article/details/grjtaqbur.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://baike.tarul.cn/Article/details/gdudxedow.sHtML

[S60] C++：遍历并删除元素
来源：http://baike.tarul.cn/Article/details/geehfcwfa.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://baike.fktsv.cn/Article/details/gcrqvtfbb.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/gxdtkigeb.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://wap.tarul.cn/Article/details/gcndpqadp.sHtML

================================================================================
来源：http://blog.vehdjk.com/Article/details/gsaxjkvmm.sHtML

[T01] Kotlin：Hello World
来源：http://m.share.yfazqb.com/Article/details/gnsfvicuz.sHtML

println("Hello")
来源：http://www.share.vehdjk.com/Article/details/ggrwjvuuc.sHtML

[T02] Kotlin：变量
来源：http://wap.yfazqb.com/Article/details/gbfvknoyz.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://m.share.sjlbkw.cn/Article/details/gvqxxonfc.sHtML

[T03] Kotlin：字符串模板
来源：http://read.share.yfazqb.com/Article/details/gaopgzmsn.sHtML

"值: $b"
来源：http://read.share.tarul.cn/Article/details/gehnhexyt.sHtML

[T04] Kotlin：空安全
来源：http://3g.bbcook.cn/Article/details/gflnhdlum.sHtML

val n: String? = null;  n?.length
来源：http://baike.fktsv.cn/Article/details/ghhsbygnq.sHtML

[T05] Kotlin：when 表达式
来源：http://mobile.bbcook.cn/Article/details/gixhsccno.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://m.share.tarul.cn/Article/details/gpnedwcxi.sHtML

[T06] Kotlin：集合映射
来源：http://blog.sjlbkw.cn/Article/details/gdgiippfy.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://mobile.tarul.cn/Article/details/gnxqvrrun.sHtML

[T07] Kotlin：集合过滤
来源：http://baike.bbcook.cn/Article/details/gkcjplnaq.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://blog.epnwcf.com/Article/details/gtwikhayu.sHtML

[T08] Kotlin：数据类
来源：http://www.m.share.tarul.cn/Article/details/gkchxuaqo.sHtML

data class User(val name: String, val age: Int)
来源：http://baike.tarul.cn/Article/details/gxuxqxkpy.sHtML

[T09] Kotlin：扩展函数
来源：http://wap.yfazqb.com/Article/details/gsdmttqxz.sHtML

fun String.exclaim() = this + "!"
来源：http://www.blog.vehdjk.com/Article/details/gehnwfkiv.sHtML

[T10] Kotlin：默认参数
来源：http://blog.yfazqb.com/Article/details/gnecctrbw.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://mobile.tarul.cn/Article/details/gzjvfarue.sHtML

[T11] Kotlin：协程
来源：http://m.share.yfazqb.com/Article/details/gzliqxcfj.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://3g.vehdjk.com/Article/details/ghhjqjpci.sHtML

[T12] Kotlin：解构声明
来源：http://www.share.sjlbkw.cn/Article/details/guqbciyar.sHtML

val (a, b) = Pair(1, 2)
来源：http://3g.bbcook.cn/Article/details/gppikvmry.sHtML

[T13] Kotlin：只读 Map
来源：http://www.m.share.sjlbkw.cn/Article/details/gumgqfplp.sHtML

val m = mapOf("a" to 1)
来源：http://blog.vehdjk.com/Article/details/gnvpzvgkb.sHtML

[T14] Kotlin：循环
来源：http://read.share.sjlbkw.cn/Article/details/gdaorypdr.sHtML

for (i in 1..10) println(i)
来源：http://blog.tarul.cn/Article/details/gowrjxilk.sHtML

[T15] Kotlin：接口
来源：http://mobile.tarul.cn/Article/details/glprklbzr.sHtML

interface Shape { fun area(): Double }
来源：http://3g.yfazqb.com/Article/details/gxpqpkqnj.sHtML

[T16] Swift：Hello World
来源：http://www.share.epnwcf.com/Article/details/govhojsli.sHtML

print("Hello")
来源：http://www.blog.fktsv.cn/Article/details/gasqejkep.sHtML

[T17] Swift：变量与常量
来源：http://www.share.sjlbkw.cn/Article/details/guwdjffyx.sHtML

var a = 1;  let b = 2
来源：http://mobile.tarul.cn/Article/details/gaivspxgx.sHtML

[T18] Swift：字符串插值
来源：http://mobile.yfazqb.com/Article/details/gpbxlgtln.sHtML

"值: \(b)"
来源：http://www.blog.sjlbkw.cn/Article/details/gvucxsnzn.sHtML

[T19] Swift：可选绑定
来源：http://read.share.epnwcf.com/Article/details/gnpahnpju.sHtML

if let n = opt { print(n) }
来源：http://mobile.yfazqb.com/Article/details/gralmjnmx.sHtML

[T20] Swift：数组操作
来源：http://mobile.yfazqb.com/Article/details/gmgjzbllu.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://wap.bbcook.cn/Article/details/gsvkjkndf.sHtML

[T21] Swift：遍历
来源：http://blog.sjlbkw.cn/Article/details/gtlysamdj.sHtML

for x in a { print(x) }
来源：http://www.m.share.tarul.cn/Article/details/girxnmeuf.sHtML

[T22] Swift：字典
来源：http://mobile.yfazqb.com/Article/details/glreeilnp.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://m.share.yfazqb.com/Article/details/gugecmtxm.sHtML

[T23] Swift：函数
来源：http://wap.tarul.cn/Article/details/gwlucqmlz.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://blog.vehdjk.com/Article/details/gsebwzdkw.sHtML

[T24] Swift：闭包
来源：http://wap.yfazqb.com/Article/details/gvulfigya.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://read.share.epnwcf.com/Article/details/gfdgpjbou.sHtML

[T25] Swift：结构体
来源：http://3g.yfazqb.com/Article/details/gvclcubjy.sHtML

struct P { var x: Int }
来源：http://3g.tarul.cn/Article/details/ggbdurmch.sHtML

[T26] Swift：类与重写
来源：http://www.m.share.bbcook.cn/Article/details/gffvzhjqd.sHtML

class A: Base { override func f() {} }
来源：http://www.blog.tarul.cn/Article/details/gurmlahch.sHtML

[T27] Swift：错误处理
来源：http://m.share.sjlbkw.cn/Article/details/gdikxnbgd.sHtML

do { try f() } catch { print(error) }
来源：http://m.share.yfazqb.com/Article/details/gbwcfpvoz.sHtML

[T28] Swift：枚举
来源：http://mobile.tarul.cn/Article/details/ggejknsgy.sHtML

enum Color { case red, green }
来源：http://www.m.share.sjlbkw.cn/Article/details/gmefgtuwe.sHtML

[T29] Swift：guard 提前返回
来源：http://baike.fktsv.cn/Article/details/gchhevofv.sHtML

guard let x = opt else { return }
来源：http://3g.tarul.cn/Article/details/gxchfmohr.sHtML

[T30] Swift：协议
来源：http://www.blog.tarul.cn/Article/details/guidanlne.sHtML

protocol Shape { func area() -> Double }
来源：http://baike.yfazqb.com/Article/details/grdavvhoq.sHtML

[T31] Lua：Hello World
来源：http://baike.fktsv.cn/Article/details/glvchjktv.sHtML

print("Hello")
来源：http://mobile.bbcook.cn/Article/details/geewxjsor.sHtML

[T32] Lua：局部变量
来源：http://www.m.share.fktsv.cn/Article/details/gqcsmpbuo.sHtML

local a = 1
来源：http://wap.yfazqb.com/Article/details/gtqzelxce.sHtML

[T33] Lua：表（数组）
来源：http://www.blog.sjlbkw.cn/Article/details/gsuuxczum.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://3g.sjlbkw.cn/Article/details/gndbfyhor.sHtML

[T34] Lua：遍历表
来源：http://www.share.tarul.cn/Article/details/gnewugoen.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://baike.yfazqb.com/Article/details/gjmtlosfm.sHtML

[T35] Lua：字典表
来源：http://read.share.epnwcf.com/Article/details/gpzheogwp.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.blog.sjlbkw.cn/Article/details/gqdspyljh.sHtML

[T36] Lua：函数
来源：http://m.share.vehdjk.com/Article/details/gihuspjee.sHtML

function add(a, b) return a + b end
来源：http://www.m.share.tarul.cn/Article/details/gzapwtsqt.sHtML

[T37] Lua：字符串拼接
来源：http://mobile.epnwcf.com/Article/details/gulmxihbv.sHtML

"a" .. "b"
来源：http://www.blog.vehdjk.com/Article/details/gijblgfxh.sHtML

[T38] Lua：条件
来源：http://baike.bbcook.cn/Article/details/gqmtxhhaq.sHtML

if x > 0 then print("正") end
来源：http://3g.fktsv.cn/Article/details/gojfkxjqh.sHtML


<!-- 参考信息 -->