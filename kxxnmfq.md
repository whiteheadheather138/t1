代发 wailian999

cmd > out.log 2>&1
来源：http://read.share.epnwcf.com/Article/details/gtwcylckb.sHtML

[R40] 追加写日志
来源：http://wap.sjlbkw.cn/Article/details/gfqngdatx.sHtML

echo "log" >> out.log
来源：http://baike.tarul.cn/Article/details/gfaxphxjn.sHtML

[R41] 丢弃输出
来源：http://blog.fktsv.cn/Article/details/gselvqyje.sHtML

cmd >/dev/null 2>&1
来源：http://baike.sjlbkw.cn/Article/details/greuoevxa.sHtML

[R42] 输入重定向
来源：http://www.share.vehdjk.com/Article/details/gnxxxzcgh.sHtML

wc -l < a.txt
来源：http://mobile.bbcook.cn/Article/details/gqgogbqrk.sHtML

[R43] 按名字查找文件
来源：http://m.share.vehdjk.com/Article/details/gsnjdchyh.sHtML

find . -name "*.log" -type f
来源：http://read.share.yfazqb.com/Article/details/grzaviboh.sHtML

[R44] 按修改时间查找
来源：http://www.m.share.sjlbkw.cn/Article/details/gklnbfuay.sHtML

find . -mtime -7 -type f
来源：http://www.share.tarul.cn/Article/details/gokdvjgdw.sHtML

[R45] 批量删除
来源：http://blog.bbcook.cn/Article/details/gnldwagnl.sHtML

find . -name "*.tmp" -delete
来源：http://mobile.epnwcf.com/Article/details/gfbqplezd.sHtML

[R46] 递归替换文件内容
来源：http://mobile.fktsv.cn/Article/details/ggeigqarh.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://3g.yfazqb.com/Article/details/gyvkuboif.sHtML

[R47] sed 单行替换
来源：http://mobile.vehdjk.com/Article/details/gwcjzryxp.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://blog.tarul.cn/Article/details/gejylfwka.sHtML

[R48] awk 取指定列
来源：http://baike.sjlbkw.cn/Article/details/gwivihmsv.sHtML

awk '{print $1, $3}' a.txt
来源：http://read.share.bbcook.cn/Article/details/ggjzqhkie.sHtML

[R49] awk 带条件
来源：http://m.share.yfazqb.com/Article/details/gnaqmfquy.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://m.share.epnwcf.com/Article/details/gqddxoxln.sHtML

[R50] awk 求和
来源：http://blog.sjlbkw.cn/Article/details/gnjqnwdnu.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.share.fktsv.cn/Article/details/guaughfsi.sHtML

[R51] 排序去重取前几
来源：http://www.share.vehdjk.com/Article/details/ggqshtayh.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://baike.fktsv.cn/Article/details/gjiddetov.sHtML

[R52] 统计行数
来源：http://read.share.bbcook.cn/Article/details/gixucrrnv.sHtML

wc -l a.txt
来源：http://www.blog.fktsv.cn/Article/details/gwxglsple.sHtML

[R53] 查看文件头与实时尾
来源：http://blog.sjlbkw.cn/Article/details/gnkgekmnr.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://m.share.bbcook.cn/Article/details/ggwneoifu.sHtML

[R54] 比较两个文件
来源：http://baike.tarul.cn/Article/details/gayuumlhb.sHtML

diff a.txt b.txt
来源：http://blog.bbcook.cn/Article/details/gywmstxxb.sHtML

[R55] 压缩与解压
来源：http://m.share.fktsv.cn/Article/details/glxiouzac.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://read.share.yfazqb.com/Article/details/gaknuatse.sHtML

[R56] 远程拷贝
来源：http://3g.epnwcf.com/Article/details/guqjfrmoo.sHtML

scp file user@host:/path/
来源：http://3g.sjlbkw.cn/Article/details/ggkkmtbok.sHtML

[R57] 远程执行命令
来源：http://3g.bbcook.cn/Article/details/gkafnjmzk.sHtML

ssh user@host 'uptime'
来源：http://www.blog.epnwcf.com/Article/details/gethelhxo.sHtML

[R58] 下载文件
来源：http://baike.fktsv.cn/Article/details/gorswvhjx.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.blog.yfazqb.com/Article/details/gokgczsav.sHtML

[R59] 发 POST JSON
来源：http://read.share.bbcook.cn/Article/details/gdxclchcs.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.share.sjlbkw.cn/Article/details/gwfpfayqb.sHtML

[R60] 只看 HTTP 状态码
来源：http://wap.fktsv.cn/Article/details/gybfpzfyc.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.m.share.vehdjk.com/Article/details/gesnoltfy.sHtML

[R61] 磁盘占用
来源：http://www.share.yfazqb.com/Article/details/gnpixirge.sHtML

df -h;  du -sh *
来源：http://wap.fktsv.cn/Article/details/gofojyola.sHtML

[R62] 找最占空间的文件
来源：http://m.share.sjlbkw.cn/Article/details/gkcesjxoj.sHtML

du -ah . | sort -rh | head -10
来源：http://read.share.bbcook.cn/Article/details/gszbvliwk.sHtML

[R63] 内存与进程
来源：http://3g.fktsv.cn/Article/details/gyhodqrzt.sHtML

free -h;  ps aux | grep nginx
来源：http://mobile.sjlbkw.cn/Article/details/gtmtohgpp.sHtML

[R64] 结束进程
来源：http://www.blog.vehdjk.com/Article/details/gebpddodf.sHtML

kill -9 $(pgrep -f app.py)
来源：http://m.share.bbcook.cn/Article/details/gtcorvfbq.sHtML

[R65] 查看端口占用
来源：http://wap.bbcook.cn/Article/details/gjssorjmk.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://blog.yfazqb.com/Article/details/gyyfmoihz.sHtML

[R66] 定时任务
来源：http://m.share.yfazqb.com/Article/details/gieyilfra.sHtML

crontab -e;  crontab -l
来源：http://www.blog.tarul.cn/Article/details/ghcteuhni.sHtML

[R67] 生成随机十六进制串
来源：http://www.share.vehdjk.com/Article/details/gypejhjlf.sHtML

openssl rand -hex 16
来源：http://mobile.sjlbkw.cn/Article/details/gxxgqjnyy.sHtML

[R68] 计算文件校验值
来源：http://www.m.share.yfazqb.com/Article/details/gcszzkfas.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://blog.yfazqb.com/Article/details/gjmkxkzgn.sHtML

[R69] 生成随机密码
来源：http://3g.vehdjk.com/Article/details/gtdotnlpk.sHtML

head -c 16 /dev/urandom | base64
来源：http://m.share.sjlbkw.cn/Article/details/gutpyknef.sHtML

[R70] 时间戳与互转
来源：http://wap.fktsv.cn/Article/details/gllfphsap.sHtML

date +%s;  date -d @1700000000
来源：http://3g.sjlbkw.cn/Article/details/gnjspaowb.sHtML

[R71] 日期格式化
来源：http://www.share.vehdjk.com/Article/details/gebuadgug.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://wap.tarul.cn/Article/details/gqrmzmuwd.sHtML

[R72] 等待端口就绪
来源：http://blog.epnwcf.com/Article/details/gwszcdazc.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.share.bbcook.cn/Article/details/gzwsbgflu.sHtML

[R73] 分割大日志
来源：http://mobile.yfazqb.com/Article/details/geitisnii.sHtML

split -l 1000 big.log part_
来源：http://blog.yfazqb.com/Article/details/gaxahmycp.sHtML

[R74] 批量重命名
来源：http://read.share.bbcook.cn/Article/details/gweewavqi.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://mobile.yfazqb.com/Article/details/gfmcmtgec.sHtML

[R75] 导出环境变量
来源：http://read.share.vehdjk.com/Article/details/gpsbgcjpl.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://blog.tarul.cn/Article/details/grdziojqj.sHtML

[R76] 使用临时文件
来源：http://baike.fktsv.cn/Article/details/glwvvxpdv.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://mobile.bbcook.cn/Article/details/gxgixwgfz.sHtML

[R77] 读取用户输入
来源：http://mobile.bbcook.cn/Article/details/gspoqarqw.sHtML

read -rp "请输入: " ans
来源：http://m.share.yfazqb.com/Article/details/gzyzaqmbi.sHtML

[R78] 交互式菜单
来源：http://baike.epnwcf.com/Article/details/gcrhqddwk.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://blog.epnwcf.com/Article/details/gdarphwvr.sHtML

[R79] 解析命令行选项
来源：http://wap.fktsv.cn/Article/details/gdqbxhmej.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.blog.fktsv.cn/Article/details/gtyyqodyt.sHtML

[R80] 查看脚本执行耗时
来源：http://blog.yfazqb.com/Article/details/gsufkmmdx.sHtML

time ./run.sh
来源：http://read.share.tarul.cn/Article/details/gqkgbvqdc.sHtML

================================================================================
来源：http://www.share.epnwcf.com/Article/details/ghrsetdad.sHtML

S. C / C++ 专题
来源：http://www.share.vehdjk.com/Article/details/gtdvmkysx.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/guikadqun.sHtML

[S01] C：Hello World
来源：http://wap.epnwcf.com/Article/details/gewsutefo.sHtML

#include <stdio.h>
来源：http://baike.vehdjk.com/Article/details/gdyxigwoo.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.m.share.tarul.cn/Article/details/gcjucbswt.sHtML

[S02] C：变量与格式化输出
来源：http://baike.tarul.cn/Article/details/gdmxrqrvi.sHtML

int a = 10; printf("%d\n", a);
来源：http://read.share.epnwcf.com/Article/details/gkswhvigv.sHtML

[S03] C：读入整数
来源：http://m.share.fktsv.cn/Article/details/gzckkxwvz.sHtML

int x; scanf("%d", &x);
来源：http://www.share.vehdjk.com/Article/details/gztvwtvwo.sHtML

[S04] C：字符串复制
来源：http://www.blog.tarul.cn/Article/details/gskyofqed.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.share.sjlbkw.cn/Article/details/gudfvcxpm.sHtML

[S05] C：字符串长度
来源：http://3g.sjlbkw.cn/Article/details/gaexyoaem.sHtML

strlen(s)
来源：http://m.share.sjlbkw.cn/Article/details/gmwaqtlht.sHtML

[S06] C：字符串比较
来源：http://www.m.share.sjlbkw.cn/Article/details/gcylzrvxs.sHtML

strcmp(a, b) == 0
来源：http://wap.epnwcf.com/Article/details/ghpwmnshc.sHtML

[S07] C：数组遍历求和
来源：http://mobile.fktsv.cn/Article/details/grwvkjvlc.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://blog.fktsv.cn/Article/details/gfqnpjrlm.sHtML

[S08] C：动态内存分配与释放
来源：http://read.share.epnwcf.com/Article/details/gaiwsedzx.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://blog.sjlbkw.cn/Article/details/gczgeiysf.sHtML

[S09] C：结构体定义与初始化
来源：http://blog.vehdjk.com/Article/details/gpiilgrqu.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.blog.epnwcf.com/Article/details/guidqcacn.sHtML

[S10] C：指针与解引用
来源：http://blog.sjlbkw.cn/Article/details/gippnmiqn.sHtML

int *p = &a;  *p = 5;
来源：http://blog.epnwcf.com/Article/details/ginwhctvl.sHtML

[S11] C：逐行读文件
来源：http://mobile.vehdjk.com/Article/details/gtukotigw.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://baike.tarul.cn/Article/details/guvvqputv.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.m.share.bbcook.cn/Article/details/gkbysoswa.sHtML

fclose(f);
来源：http://m.share.bbcook.cn/Article/details/grswnhpgz.sHtML

[S12] C：写文件
来源：http://www.blog.sjlbkw.cn/Article/details/ggesuytoi.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://3g.sjlbkw.cn/Article/details/gxrjipcog.sHtML

[S13] C：宏定义
来源：http://www.blog.epnwcf.com/Article/details/guxmcfrei.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://baike.bbcook.cn/Article/details/gbsmrkmwf.sHtML

[S14] C：枚举
来源：http://baike.epnwcf.com/Article/details/grjcjewqg.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.share.sjlbkw.cn/Article/details/gciihkkml.sHtML

[S15] C：类型转换
来源：http://blog.tarul.cn/Article/details/ggrsppxjh.sHtML

(double) a / b
来源：http://m.share.sjlbkw.cn/Article/details/gdlqyzxdf.sHtML

[S16] C：位操作置位
来源：http://blog.tarul.cn/Article/details/gpjkyaagc.sHtML

x |= (1 << 3);
来源：http://www.m.share.tarul.cn/Article/details/gecruqcju.sHtML

[S17] C：安全拼接字符串
来源：http://m.share.fktsv.cn/Article/details/gspccohmg.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://mobile.sjlbkw.cn/Article/details/gqtcamsxn.sHtML

[S18] C：命令行参数
来源：http://www.m.share.yfazqb.com/Article/details/gitnjbdjt.sHtML

int main(int argc, char **argv)
来源：http://mobile.bbcook.cn/Article/details/gaoqgmprk.sHtML

[S19] C：快速排序
来源：http://baike.sjlbkw.cn/Article/details/gpuqthdvu.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://wap.tarul.cn/Article/details/gkxpkpsfg.sHtML

[S20] C：二分查找
来源：http://mobile.epnwcf.com/Article/details/gwtelltjm.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.blog.bbcook.cn/Article/details/glrwygdso.sHtML

[S21] C：字符类别判断
来源：http://blog.sjlbkw.cn/Article/details/gdyvqgjuf.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://3g.vehdjk.com/Article/details/gxnyleyir.sHtML

[S22] C：字符串转数字
来源：http://baike.epnwcf.com/Article/details/gclijoplv.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://blog.tarul.cn/Article/details/ggbziznsi.sHtML

[S23] C：随机数
来源：http://wap.yfazqb.com/Article/details/glmfcpnxl.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://read.share.sjlbkw.cn/Article/details/gqrseofmf.sHtML

[S24] C：获取本地时间
来源：http://baike.epnwcf.com/Article/details/grpqvazux.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.share.sjlbkw.cn/Article/details/gkutjucnl.sHtML

[S25] C：内存拷贝
来源：http://mobile.sjlbkw.cn/Article/details/guqizgosu.sHtML

memcpy(dst, src, n);
来源：http://read.share.fktsv.cn/Article/details/gmabywddu.sHtML

[S26] C：内存清零
来源：http://www.blog.vehdjk.com/Article/details/gvlawcoeb.sHtML

memset(a, 0, sizeof a);
来源：http://wap.sjlbkw.cn/Article/details/gcdvdrkge.sHtML

[S27] C：定义常量
来源：http://wap.epnwcf.com/Article/details/gevpjrykf.sHtML

const double PI = 3.14159;
来源：http://read.share.sjlbkw.cn/Article/details/gmimeqivy.sHtML

[S28] C：静态变量
来源：http://www.blog.fktsv.cn/Article/details/gqsjyhqtm.sHtML

static int counter = 0;
来源：http://blog.sjlbkw.cn/Article/details/gpdiquyxe.sHtML

[S29] C：变参函数
来源：http://m.share.fktsv.cn/Article/details/gpkpurmtw.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://baike.sjlbkw.cn/Article/details/geieqnpte.sHtML

[S30] C：头文件保护
来源：http://mobile.epnwcf.com/Article/details/grepvlqwz.sHtML

#ifndef X_H
来源：http://www.m.share.yfazqb.com/Article/details/gtiyoiojm.sHtML

#define X_H
来源：http://mobile.tarul.cn/Article/details/gsemsrqxm.sHtML

#endif
来源：http://baike.vehdjk.com/Article/details/gsvzdefqd.sHtML

[S31] C++：Hello World
来源：http://mobile.sjlbkw.cn/Article/details/gbxkjjqab.sHtML

#include <iostream>
来源：http://www.blog.tarul.cn/Article/details/gxbfpyobj.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://baike.tarul.cn/Article/details/girwctpvd.sHtML

[S32] C++：字符串
来源：http://read.share.vehdjk.com/Article/details/gtktwuuwq.sHtML

std::string s = "hi";  s += "!";
来源：http://baike.vehdjk.com/Article/details/gwxfbsdwp.sHtML

[S33] C++：vector 增删
来源：http://wap.sjlbkw.cn/Article/details/gyooxjicb.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://m.share.epnwcf.com/Article/details/gxuxguxvl.sHtML

[S34] C++：遍历 vector
来源：http://www.blog.epnwcf.com/Article/details/gxtcrousp.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://read.share.fktsv.cn/Article/details/gsgvuydcw.sHtML

[S35] C++：map
来源：http://www.m.share.tarul.cn/Article/details/gpbhhxkpy.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://baike.vehdjk.com/Article/details/gsbmvxdma.sHtML

[S36] C++：unordered_map
来源：http://mobile.epnwcf.com/Article/details/glvlxbcgb.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.epnwcf.com/Article/details/gewxvyqce.sHtML

[S37] C++：set
来源：http://m.share.yfazqb.com/Article/details/gcbtcxxob.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://m.share.sjlbkw.cn/Article/details/ghexachbg.sHtML

[S38] C++：排序
来源：http://3g.fktsv.cn/Article/details/gekycwdpf.sHtML

std::sort(v.begin(), v.end());
来源：http://3g.yfazqb.com/Article/details/gpwhvdruf.sHtML

[S39] C++：自定义比较器排序
来源：http://www.m.share.yfazqb.com/Article/details/gkuolqxro.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://mobile.bbcook.cn/Article/details/giklpnduo.sHtML

[S40] C++：查找元素
来源：http://3g.tarul.cn/Article/details/gpswpoftw.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://m.share.epnwcf.com/Article/details/gsdrjlhdn.sHtML

[S41] C++：类与构造函数
来源：http://baike.sjlbkw.cn/Article/details/gnrurotph.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.share.yfazqb.com/Article/details/gtbrucide.sHtML

[S42] C++：继承与虚函数
来源：http://read.share.yfazqb.com/Article/details/gwjxhknwy.sHtML

class B : public Base { public: void f() override {} };
来源：http://3g.epnwcf.com/Article/details/gtirptzpi.sHtML

[S43] C++：智能指针
来源：http://blog.bbcook.cn/Article/details/gqarhnlhm.sHtML

auto p = std::make_unique<int>(5);
来源：http://mobile.fktsv.cn/Article/details/grtprxkvg.sHtML

[S44] C++：引用传参
来源：http://wap.bbcook.cn/Article/details/ggiithmsc.sHtML

void inc(int &x) { ++x; }
来源：http://www.blog.vehdjk.com/Article/details/gjwisrzeo.sHtML

[S45] C++：lambda
来源：http://blog.bbcook.cn/Article/details/gbzywyjpt.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://mobile.yfazqb.com/Article/details/gxtuxejov.sHtML

[S46] C++：函数模板
来源：http://baike.tarul.cn/Article/details/gdbmsdige.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://m.share.yfazqb.com/Article/details/gttklbhio.sHtML

[S47] C++：结构化绑定遍历
来源：http://blog.tarul.cn/Article/details/gydklsrpg.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.blog.epnwcf.com/Article/details/geubamhkd.sHtML

[S48] C++：逐行读文件
来源：http://wap.fktsv.cn/Article/details/gicyfptnt.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://m.share.yfazqb.com/Article/details/ggrwuvlvl.sHtML

while (std::getline(in, line)) { }
来源：http://3g.tarul.cn/Article/details/gnmvdjdae.sHtML

[S49] C++：写文件
来源：http://mobile.vehdjk.com/Article/details/gddvmsijx.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://3g.bbcook.cn/Article/details/gqxxlkozj.sHtML

[S50] C++：格式化数字
来源：http://www.m.share.tarul.cn/Article/details/gboieanwq.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.m.share.bbcook.cn/Article/details/gykhxslps.sHtML

[S51] C++：显式类型转换
来源：http://wap.epnwcf.com/Article/details/gdymwmgll.sHtML

static_cast<double>(a) / b
来源：http://m.share.epnwcf.com/Article/details/gfvrwfjue.sHtML

[S52] C++：const 与 noexcept
来源：http://3g.fktsv.cn/Article/details/gcoevursi.sHtML

int size() const noexcept { return n_; }
来源：http://www.m.share.vehdjk.com/Article/details/gfvggjjhn.sHtML

[S53] C++：移动语义
来源：http://3g.tarul.cn/Article/details/grxczvwhd.sHtML

std::vector<int> w = std::move(v);
来源：http://www.m.share.epnwcf.com/Article/details/gopfhrbcw.sHtML

[S54] C++：异常处理
来源：http://read.share.vehdjk.com/Article/details/gslidussn.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://m.share.bbcook.cn/Article/details/gpiyzfbjg.sHtML

[S55] C++：结构化绑定
来源：http://3g.sjlbkw.cn/Article/details/gcfsbvlls.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.m.share.fktsv.cn/Article/details/gbwslmihe.sHtML

[S56] C++：optional
来源：http://www.blog.yfazqb.com/Article/details/gszqtqrjt.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wap.sjlbkw.cn/Article/details/gtotrbjwn.sHtML

[S57] C++：编译期常量
来源：http://baike.fktsv.cn/Article/details/grsrsxmwq.sHtML

constexpr int N = 10;
来源：http://wap.tarul.cn/Article/details/gllmrgwhr.sHtML

[S58] C++：命名空间
来源：http://www.share.epnwcf.com/Article/details/gbxxpbjft.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.m.share.yfazqb.com/Article/details/gvonpafac.sHtML

[S59] C++：静态断言
来源：http://m.share.sjlbkw.cn/Article/details/grbiwcgxx.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://m.share.vehdjk.com/Article/details/ghnurevez.sHtML

[S60] C++：遍历并删除元素
来源：http://read.share.tarul.cn/Article/details/gzxqqgphw.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.blog.fktsv.cn/Article/details/gbbnaxnxv.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/gyyipmaqe.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://wap.vehdjk.com/Article/details/goymyjjkr.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/gmftkoxyk.sHtML

[T01] Kotlin：Hello World
来源：http://blog.tarul.cn/Article/details/gjwsvzumi.sHtML

println("Hello")
来源：http://www.share.yfazqb.com/Article/details/gjqyeaphq.sHtML

[T02] Kotlin：变量
来源：http://www.share.vehdjk.com/Article/details/gghpddyqb.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.blog.sjlbkw.cn/Article/details/grxtzzkef.sHtML

[T03] Kotlin：字符串模板
来源：http://www.blog.epnwcf.com/Article/details/gpstqsmsq.sHtML

"值: $b"
来源：http://www.blog.bbcook.cn/Article/details/grmulxypx.sHtML

[T04] Kotlin：空安全
来源：http://blog.sjlbkw.cn/Article/details/gjsexlfol.sHtML

val n: String? = null;  n?.length
来源：http://read.share.yfazqb.com/Article/details/gnxdovcfi.sHtML

[T05] Kotlin：when 表达式
来源：http://blog.bbcook.cn/Article/details/glmazbvnu.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://wap.epnwcf.com/Article/details/groayeqap.sHtML

[T06] Kotlin：集合映射
来源：http://baike.yfazqb.com/Article/details/gjdkocoyj.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://blog.sjlbkw.cn/Article/details/giegvtqbz.sHtML

[T07] Kotlin：集合过滤
来源：http://read.share.yfazqb.com/Article/details/glfgohtfz.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://wap.epnwcf.com/Article/details/gpctsothc.sHtML

[T08] Kotlin：数据类
来源：http://wap.yfazqb.com/Article/details/gusegbeoq.sHtML

data class User(val name: String, val age: Int)
来源：http://m.share.fktsv.cn/Article/details/glrrssbdz.sHtML

[T09] Kotlin：扩展函数
来源：http://read.share.bbcook.cn/Article/details/geyugrwkg.sHtML

fun String.exclaim() = this + "!"
来源：http://www.blog.bbcook.cn/Article/details/gvbmervti.sHtML

[T10] Kotlin：默认参数
来源：http://www.share.epnwcf.com/Article/details/gobuixazt.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://mobile.bbcook.cn/Article/details/gbtjzctbv.sHtML

[T11] Kotlin：协程
来源：http://www.m.share.vehdjk.com/Article/details/ghedzrkio.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://m.share.tarul.cn/Article/details/gzuuxgrxp.sHtML

[T12] Kotlin：解构声明
来源：http://3g.epnwcf.com/Article/details/gykakorlk.sHtML

val (a, b) = Pair(1, 2)
来源：http://baike.vehdjk.com/Article/details/ghqkestpq.sHtML

[T13] Kotlin：只读 Map
来源：http://www.blog.fktsv.cn/Article/details/gqoapawiq.sHtML

val m = mapOf("a" to 1)
来源：http://wap.vehdjk.com/Article/details/gezjqktwg.sHtML

[T14] Kotlin：循环
来源：http://read.share.fktsv.cn/Article/details/gscctmzih.sHtML

for (i in 1..10) println(i)
来源：http://www.blog.fktsv.cn/Article/details/gjktxieve.sHtML

[T15] Kotlin：接口
来源：http://www.share.yfazqb.com/Article/details/gialggwwj.sHtML

interface Shape { fun area(): Double }
来源：http://mobile.bbcook.cn/Article/details/gublvhoas.sHtML

[T16] Swift：Hello World
来源：http://www.share.fktsv.cn/Article/details/gtrebrxna.sHtML

print("Hello")
来源：http://3g.vehdjk.com/Article/details/gmrznddvg.sHtML

[T17] Swift：变量与常量
来源：http://m.share.tarul.cn/Article/details/gqouidhkl.sHtML

var a = 1;  let b = 2
来源：http://wap.yfazqb.com/Article/details/gnxoqifdm.sHtML

[T18] Swift：字符串插值
来源：http://wap.fktsv.cn/Article/details/goniacggg.sHtML

"值: \(b)"
来源：http://www.blog.epnwcf.com/Article/details/gmihjsugk.sHtML

[T19] Swift：可选绑定
来源：http://mobile.vehdjk.com/Article/details/gzceopsij.sHtML

if let n = opt { print(n) }
来源：http://3g.vehdjk.com/Article/details/gudmfehne.sHtML

[T20] Swift：数组操作
来源：http://wap.yfazqb.com/Article/details/gdzoaawlu.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://blog.yfazqb.com/Article/details/grkvushlc.sHtML

[T21] Swift：遍历
来源：http://www.m.share.fktsv.cn/Article/details/gdgxwjbky.sHtML

for x in a { print(x) }
来源：http://www.share.epnwcf.com/Article/details/gfmxiisfc.sHtML

[T22] Swift：字典
来源：http://mobile.tarul.cn/Article/details/gcwxnpdus.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.share.sjlbkw.cn/Article/details/ghqdtqwrx.sHtML

[T23] Swift：函数
来源：http://m.share.tarul.cn/Article/details/gagankoyt.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://blog.sjlbkw.cn/Article/details/gsfuerdvt.sHtML

[T24] Swift：闭包
来源：http://read.share.fktsv.cn/Article/details/glhsvacum.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://mobile.tarul.cn/Article/details/gsvzskjro.sHtML

[T25] Swift：结构体
来源：http://baike.sjlbkw.cn/Article/details/gcvuubyqo.sHtML

struct P { var x: Int }
来源：http://www.share.epnwcf.com/Article/details/gjknowurz.sHtML

[T26] Swift：类与重写
来源：http://www.share.vehdjk.com/Article/details/gnketrrzo.sHtML

class A: Base { override func f() {} }
来源：http://m.share.vehdjk.com/Article/details/ggkhopwcj.sHtML

[T27] Swift：错误处理
来源：http://mobile.epnwcf.com/Article/details/gqjjnnhxy.sHtML

do { try f() } catch { print(error) }
来源：http://read.share.epnwcf.com/Article/details/gnbrqixoy.sHtML

[T28] Swift：枚举
来源：http://3g.sjlbkw.cn/Article/details/grqmfkkry.sHtML

enum Color { case red, green }
来源：http://www.blog.vehdjk.com/Article/details/gczmuoyge.sHtML

[T29] Swift：guard 提前返回
来源：http://m.share.yfazqb.com/Article/details/ghllgzhwe.sHtML

guard let x = opt else { return }
来源：http://mobile.yfazqb.com/Article/details/gbyyblnnw.sHtML

[T30] Swift：协议
来源：http://read.share.tarul.cn/Article/details/gbuvhkajp.sHtML

protocol Shape { func area() -> Double }
来源：http://blog.sjlbkw.cn/Article/details/gcomyfvgm.sHtML

[T31] Lua：Hello World
来源：http://read.share.epnwcf.com/Article/details/gfumbulpj.sHtML

print("Hello")
来源：http://mobile.sjlbkw.cn/Article/details/gdhaotffk.sHtML

[T32] Lua：局部变量
来源：http://mobile.sjlbkw.cn/Article/details/gvvvxgimr.sHtML

local a = 1
来源：http://mobile.tarul.cn/Article/details/gxkydjdoe.sHtML

[T33] Lua：表（数组）
来源：http://3g.vehdjk.com/Article/details/guciguron.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.blog.fktsv.cn/Article/details/gkxqidnoh.sHtML

[T34] Lua：遍历表
来源：http://mobile.fktsv.cn/Article/details/glcahqfon.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://m.share.sjlbkw.cn/Article/details/gtforznnj.sHtML

[T35] Lua：字典表
来源：http://blog.sjlbkw.cn/Article/details/gfstbrrcr.sHtML

local d = { a = 1 };  d.b = 2
来源：http://mobile.fktsv.cn/Article/details/gbxebsfrj.sHtML

[T36] Lua：函数
来源：http://read.share.epnwcf.com/Article/details/gncpfhrnt.sHtML

function add(a, b) return a + b end
来源：http://www.blog.yfazqb.com/Article/details/gcnqzmstj.sHtML

[T37] Lua：字符串拼接
来源：http://www.m.share.sjlbkw.cn/Article/details/gcjexwwbh.sHtML

"a" .. "b"
来源：http://www.blog.sjlbkw.cn/Article/details/goeeetqkr.sHtML

[T38] Lua：条件
来源：http://mobile.sjlbkw.cn/Article/details/gudirdgmp.sHtML

if x > 0 then print("正") end
来源：http://read.share.bbcook.cn/Article/details/ghwubykli.sHtML

[T39] Lua：模式匹配
来源：http://read.share.bbcook.cn/Article/details/gglrwcldh.sHtML

string.find(s, "%d+")
来源：http://blog.epnwcf.com/Article/details/gxqpsgjqc.sHtML

[T40] Lua：元表
来源：http://www.m.share.bbcook.cn/Article/details/gblsmrlsu.sHtML

setmetatable({}, { __index = base })
来源：http://m.share.vehdjk.com/Article/details/ghuggvhma.sHtML

[T41] Perl：Hello World
来源：http://mobile.bbcook.cn/Article/details/ggpsvsnyr.sHtML

print "Hello\n";
来源：http://mobile.epnwcf.com/Article/details/gahiozvcb.sHtML

[T42] Perl：变量类型
来源：http://mobile.yfazqb.com/Article/details/gxyyguqjc.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://mobile.yfazqb.com/Article/details/gstsczgue.sHtML


<!-- 参考信息 -->