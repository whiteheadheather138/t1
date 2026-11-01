代发 wailian999

cmd > out.log 2>&1
来源：http://blog.fktsv.cn/Article/details/goghciiaz.sHtML

[R40] 追加写日志
来源：http://baike.sjlbkw.cn/Article/details/grvenhgfl.sHtML

echo "log" >> out.log
来源：http://wap.fktsv.cn/Article/details/gxequyqos.sHtML

[R41] 丢弃输出
来源：http://mobile.epnwcf.com/Article/details/gpncbjwme.sHtML

cmd >/dev/null 2>&1
来源：http://m.share.tarul.cn/Article/details/gbwodgzod.sHtML

[R42] 输入重定向
来源：http://www.m.share.vehdjk.com/Article/details/gagoudqkn.sHtML

wc -l < a.txt
来源：http://read.share.fktsv.cn/Article/details/ghlqcugck.sHtML

[R43] 按名字查找文件
来源：http://www.m.share.epnwcf.com/Article/details/gimbufhrc.sHtML

find . -name "*.log" -type f
来源：http://wap.epnwcf.com/Article/details/goivmwwar.sHtML

[R44] 按修改时间查找
来源：http://3g.yfazqb.com/Article/details/ggfjssyit.sHtML

find . -mtime -7 -type f
来源：http://blog.bbcook.cn/Article/details/gcammqppi.sHtML

[R45] 批量删除
来源：http://www.blog.epnwcf.com/Article/details/gvzqppkul.sHtML

find . -name "*.tmp" -delete
来源：http://www.share.vehdjk.com/Article/details/gnmitlfmk.sHtML

[R46] 递归替换文件内容
来源：http://baike.vehdjk.com/Article/details/glzjtzufj.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.share.fktsv.cn/Article/details/gurasfgao.sHtML

[R47] sed 单行替换
来源：http://www.m.share.sjlbkw.cn/Article/details/gfqzizbaz.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.blog.fktsv.cn/Article/details/gxlnpiufa.sHtML

[R48] awk 取指定列
来源：http://baike.epnwcf.com/Article/details/gpnjokdzc.sHtML

awk '{print $1, $3}' a.txt
来源：http://read.share.bbcook.cn/Article/details/ghsctwgoa.sHtML

[R49] awk 带条件
来源：http://www.m.share.bbcook.cn/Article/details/geexejbhq.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://read.share.vehdjk.com/Article/details/gpnovlrua.sHtML

[R50] awk 求和
来源：http://mobile.yfazqb.com/Article/details/gwkyibmhw.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://read.share.vehdjk.com/Article/details/gblxpebbo.sHtML

[R51] 排序去重取前几
来源：http://mobile.sjlbkw.cn/Article/details/gvmhmvzxt.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://m.share.tarul.cn/Article/details/gzqtbpldn.sHtML

[R52] 统计行数
来源：http://www.share.epnwcf.com/Article/details/gmhvbyslj.sHtML

wc -l a.txt
来源：http://mobile.yfazqb.com/Article/details/gcjblehfm.sHtML

[R53] 查看文件头与实时尾
来源：http://www.share.tarul.cn/Article/details/glktaycnw.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.share.bbcook.cn/Article/details/ghrxkhiyb.sHtML

[R54] 比较两个文件
来源：http://blog.bbcook.cn/Article/details/gbwryhomh.sHtML

diff a.txt b.txt
来源：http://m.share.bbcook.cn/Article/details/gdbryqwfy.sHtML

[R55] 压缩与解压
来源：http://www.blog.epnwcf.com/Article/details/gcaofuuwg.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://wap.tarul.cn/Article/details/gukhuoqiw.sHtML

[R56] 远程拷贝
来源：http://www.blog.tarul.cn/Article/details/gqebrvdua.sHtML

scp file user@host:/path/
来源：http://www.blog.epnwcf.com/Article/details/gifxzkdgq.sHtML

[R57] 远程执行命令
来源：http://www.blog.epnwcf.com/Article/details/gqvbzloaj.sHtML

ssh user@host 'uptime'
来源：http://www.m.share.epnwcf.com/Article/details/gxjaeipdk.sHtML

[R58] 下载文件
来源：http://blog.bbcook.cn/Article/details/ghsxexbnq.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://m.share.tarul.cn/Article/details/grjzobabe.sHtML

[R59] 发 POST JSON
来源：http://m.share.bbcook.cn/Article/details/grrvsujdk.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://blog.yfazqb.com/Article/details/girzgdfgt.sHtML

[R60] 只看 HTTP 状态码
来源：http://read.share.bbcook.cn/Article/details/glhdbmvpy.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.m.share.epnwcf.com/Article/details/gfokuclaz.sHtML

[R61] 磁盘占用
来源：http://read.share.tarul.cn/Article/details/gfyzckeyj.sHtML

df -h;  du -sh *
来源：http://3g.bbcook.cn/Article/details/gjbulrinl.sHtML

[R62] 找最占空间的文件
来源：http://www.blog.yfazqb.com/Article/details/gpincuzlb.sHtML

du -ah . | sort -rh | head -10
来源：http://read.share.sjlbkw.cn/Article/details/geikmhocs.sHtML

[R63] 内存与进程
来源：http://m.share.epnwcf.com/Article/details/gdfxpvjgs.sHtML

free -h;  ps aux | grep nginx
来源：http://www.m.share.tarul.cn/Article/details/gybdwnvto.sHtML

[R64] 结束进程
来源：http://3g.fktsv.cn/Article/details/gtjjivaqx.sHtML

kill -9 $(pgrep -f app.py)
来源：http://mobile.sjlbkw.cn/Article/details/gbhhpined.sHtML

[R65] 查看端口占用
来源：http://blog.fktsv.cn/Article/details/gybvpacok.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://m.share.sjlbkw.cn/Article/details/gjmpjasjy.sHtML

[R66] 定时任务
来源：http://mobile.sjlbkw.cn/Article/details/gjxbkiomp.sHtML

crontab -e;  crontab -l
来源：http://www.share.tarul.cn/Article/details/gxrazctkz.sHtML

[R67] 生成随机十六进制串
来源：http://read.share.sjlbkw.cn/Article/details/gnwehmwsq.sHtML

openssl rand -hex 16
来源：http://blog.epnwcf.com/Article/details/gmgnphoya.sHtML

[R68] 计算文件校验值
来源：http://mobile.bbcook.cn/Article/details/gltmxnoig.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.m.share.yfazqb.com/Article/details/gysaikawl.sHtML

[R69] 生成随机密码
来源：http://baike.tarul.cn/Article/details/ghhidnbun.sHtML

head -c 16 /dev/urandom | base64
来源：http://m.share.yfazqb.com/Article/details/gwqosauod.sHtML

[R70] 时间戳与互转
来源：http://baike.tarul.cn/Article/details/glsmsoztc.sHtML

date +%s;  date -d @1700000000
来源：http://wap.yfazqb.com/Article/details/ghhpclbqu.sHtML

[R71] 日期格式化
来源：http://www.m.share.bbcook.cn/Article/details/gpkfrfcpc.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://3g.bbcook.cn/Article/details/gqoedvsqb.sHtML

[R72] 等待端口就绪
来源：http://blog.fktsv.cn/Article/details/gatnexjmn.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://wap.sjlbkw.cn/Article/details/gyjguevqa.sHtML

[R73] 分割大日志
来源：http://www.m.share.epnwcf.com/Article/details/gqasklwhk.sHtML

split -l 1000 big.log part_
来源：http://www.share.sjlbkw.cn/Article/details/gdobabokm.sHtML

[R74] 批量重命名
来源：http://wap.fktsv.cn/Article/details/gfzsvgoke.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://read.share.yfazqb.com/Article/details/guqgunoyq.sHtML

[R75] 导出环境变量
来源：http://blog.yfazqb.com/Article/details/guvzcrkrf.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://3g.fktsv.cn/Article/details/gldzgdstl.sHtML

[R76] 使用临时文件
来源：http://www.blog.yfazqb.com/Article/details/gwhyyaykb.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.share.sjlbkw.cn/Article/details/ggsjrwsel.sHtML

[R77] 读取用户输入
来源：http://mobile.bbcook.cn/Article/details/gfzpsqffz.sHtML

read -rp "请输入: " ans
来源：http://baike.yfazqb.com/Article/details/gubmuwgyp.sHtML

[R78] 交互式菜单
来源：http://m.share.yfazqb.com/Article/details/gisjhqczv.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.share.epnwcf.com/Article/details/gkohjkslr.sHtML

[R79] 解析命令行选项
来源：http://www.share.fktsv.cn/Article/details/geqbrvzrg.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mobile.vehdjk.com/Article/details/gtkcqyhbc.sHtML

[R80] 查看脚本执行耗时
来源：http://m.share.tarul.cn/Article/details/gmxatlqrf.sHtML

time ./run.sh
来源：http://www.share.epnwcf.com/Article/details/gfrkatozq.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/glpafarxp.sHtML

S. C / C++ 专题
来源：http://mobile.tarul.cn/Article/details/gqwsgakcw.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/gaeetxkgh.sHtML

[S01] C：Hello World
来源：http://www.blog.bbcook.cn/Article/details/ggkxagnqy.sHtML

#include <stdio.h>
来源：http://baike.fktsv.cn/Article/details/gtwybksby.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://wap.vehdjk.com/Article/details/gyvmbnkww.sHtML

[S02] C：变量与格式化输出
来源：http://m.share.fktsv.cn/Article/details/gkwantnec.sHtML

int a = 10; printf("%d\n", a);
来源：http://wap.bbcook.cn/Article/details/gakkkudpo.sHtML

[S03] C：读入整数
来源：http://www.share.tarul.cn/Article/details/gvlyblbsv.sHtML

int x; scanf("%d", &x);
来源：http://3g.epnwcf.com/Article/details/gudatxxme.sHtML

[S04] C：字符串复制
来源：http://www.m.share.vehdjk.com/Article/details/gimerwzjs.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.blog.tarul.cn/Article/details/gzujznyje.sHtML

[S05] C：字符串长度
来源：http://baike.tarul.cn/Article/details/giwnidfzm.sHtML

strlen(s)
来源：http://3g.sjlbkw.cn/Article/details/gvdwpzhpc.sHtML

[S06] C：字符串比较
来源：http://3g.epnwcf.com/Article/details/gyomxphdi.sHtML

strcmp(a, b) == 0
来源：http://www.share.fktsv.cn/Article/details/gccznrafn.sHtML

[S07] C：数组遍历求和
来源：http://3g.fktsv.cn/Article/details/ggxcjkwds.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://3g.yfazqb.com/Article/details/gbsjuidzt.sHtML

[S08] C：动态内存分配与释放
来源：http://3g.tarul.cn/Article/details/gcbpzefac.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://baike.vehdjk.com/Article/details/govniosux.sHtML

[S09] C：结构体定义与初始化
来源：http://m.share.yfazqb.com/Article/details/gdsiecoge.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.share.sjlbkw.cn/Article/details/ggaagyynq.sHtML

[S10] C：指针与解引用
来源：http://baike.vehdjk.com/Article/details/gurswfifa.sHtML

int *p = &a;  *p = 5;
来源：http://www.share.fktsv.cn/Article/details/gbfzpuaat.sHtML

[S11] C：逐行读文件
来源：http://blog.bbcook.cn/Article/details/gnxmehlrz.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://blog.fktsv.cn/Article/details/gbahaqecr.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://blog.yfazqb.com/Article/details/gqvswnoww.sHtML

fclose(f);
来源：http://wap.fktsv.cn/Article/details/gtzaxffji.sHtML

[S12] C：写文件
来源：http://read.share.tarul.cn/Article/details/gkvyoccjn.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mobile.yfazqb.com/Article/details/gmfzbczvi.sHtML

[S13] C：宏定义
来源：http://www.share.epnwcf.com/Article/details/ggquyeiqc.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.m.share.yfazqb.com/Article/details/gqzmebkjm.sHtML

[S14] C：枚举
来源：http://read.share.fktsv.cn/Article/details/gmpvmukpl.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://3g.sjlbkw.cn/Article/details/gakburbul.sHtML

[S15] C：类型转换
来源：http://read.share.fktsv.cn/Article/details/gewcrozhn.sHtML

(double) a / b
来源：http://wap.sjlbkw.cn/Article/details/giojeytkx.sHtML

[S16] C：位操作置位
来源：http://www.share.bbcook.cn/Article/details/guxptvgdn.sHtML

x |= (1 << 3);
来源：http://m.share.epnwcf.com/Article/details/gganoksbc.sHtML

[S17] C：安全拼接字符串
来源：http://3g.fktsv.cn/Article/details/gimtpyzwe.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.blog.epnwcf.com/Article/details/gufpmfqia.sHtML

[S18] C：命令行参数
来源：http://blog.sjlbkw.cn/Article/details/gemrwihun.sHtML

int main(int argc, char **argv)
来源：http://blog.vehdjk.com/Article/details/gytlgxpry.sHtML

[S19] C：快速排序
来源：http://www.m.share.tarul.cn/Article/details/gvqlhwpdq.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.m.share.tarul.cn/Article/details/gnlljhals.sHtML

[S20] C：二分查找
来源：http://m.share.yfazqb.com/Article/details/gnycimeun.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.m.share.bbcook.cn/Article/details/gjldhlvxj.sHtML

[S21] C：字符类别判断
来源：http://baike.epnwcf.com/Article/details/gbquajajv.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://3g.sjlbkw.cn/Article/details/gfosbzovy.sHtML

[S22] C：字符串转数字
来源：http://read.share.bbcook.cn/Article/details/gevahogdl.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://wap.tarul.cn/Article/details/gtrtlamru.sHtML

[S23] C：随机数
来源：http://www.share.tarul.cn/Article/details/ggqwfuczk.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.m.share.epnwcf.com/Article/details/gihhonoic.sHtML

[S24] C：获取本地时间
来源：http://www.blog.yfazqb.com/Article/details/gpheqrebb.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://wap.sjlbkw.cn/Article/details/gztpowxzm.sHtML

[S25] C：内存拷贝
来源：http://m.share.tarul.cn/Article/details/gywwdbdat.sHtML

memcpy(dst, src, n);
来源：http://www.blog.bbcook.cn/Article/details/gpqieckfv.sHtML

[S26] C：内存清零
来源：http://wap.fktsv.cn/Article/details/gclenybde.sHtML

memset(a, 0, sizeof a);
来源：http://www.m.share.fktsv.cn/Article/details/gtfmuugao.sHtML

[S27] C：定义常量
来源：http://m.share.sjlbkw.cn/Article/details/gqadxouzm.sHtML

const double PI = 3.14159;
来源：http://3g.fktsv.cn/Article/details/gsozferkp.sHtML

[S28] C：静态变量
来源：http://www.blog.yfazqb.com/Article/details/gadxoifnx.sHtML

static int counter = 0;
来源：http://baike.tarul.cn/Article/details/gmrfhzduy.sHtML

[S29] C：变参函数
来源：http://www.m.share.sjlbkw.cn/Article/details/gebdutuea.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://3g.fktsv.cn/Article/details/gashbbycw.sHtML

[S30] C：头文件保护
来源：http://3g.tarul.cn/Article/details/glmcjmrkk.sHtML

#ifndef X_H
来源：http://www.share.vehdjk.com/Article/details/gbdgecxpn.sHtML

#define X_H
来源：http://3g.fktsv.cn/Article/details/gplwbimgw.sHtML

#endif
来源：http://m.share.sjlbkw.cn/Article/details/gygvakrvt.sHtML

[S31] C++：Hello World
来源：http://read.share.tarul.cn/Article/details/gvxglnbjc.sHtML

#include <iostream>
来源：http://3g.vehdjk.com/Article/details/gvvvnnsnn.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.m.share.yfazqb.com/Article/details/gnxrbknbj.sHtML

[S32] C++：字符串
来源：http://baike.epnwcf.com/Article/details/gefsablyb.sHtML

std::string s = "hi";  s += "!";
来源：http://blog.epnwcf.com/Article/details/gdssnmpsw.sHtML

[S33] C++：vector 增删
来源：http://www.blog.tarul.cn/Article/details/gxuyklzea.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.blog.yfazqb.com/Article/details/gobvhcywl.sHtML

[S34] C++：遍历 vector
来源：http://read.share.bbcook.cn/Article/details/gojmeducm.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.blog.epnwcf.com/Article/details/gqxlyrydw.sHtML

[S35] C++：map
来源：http://wap.epnwcf.com/Article/details/glsoyaqwp.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.bbcook.cn/Article/details/ggsyjgegp.sHtML

[S36] C++：unordered_map
来源：http://www.m.share.tarul.cn/Article/details/gkfnxazka.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://baike.vehdjk.com/Article/details/gjyfzhfrw.sHtML

[S37] C++：set
来源：http://blog.fktsv.cn/Article/details/gwgkepxlp.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://baike.fktsv.cn/Article/details/grsrazxog.sHtML

[S38] C++：排序
来源：http://3g.epnwcf.com/Article/details/gmpesrlax.sHtML

std::sort(v.begin(), v.end());
来源：http://www.blog.bbcook.cn/Article/details/ghwmssdua.sHtML

[S39] C++：自定义比较器排序
来源：http://www.share.sjlbkw.cn/Article/details/gdrefrvjw.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.share.vehdjk.com/Article/details/ghwkewjbx.sHtML

[S40] C++：查找元素
来源：http://www.share.fktsv.cn/Article/details/gwsorrxod.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.blog.tarul.cn/Article/details/gwevfnrxq.sHtML

[S41] C++：类与构造函数
来源：http://www.share.yfazqb.com/Article/details/gwqtpvboh.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://mobile.sjlbkw.cn/Article/details/gszkkuffe.sHtML

[S42] C++：继承与虚函数
来源：http://wap.bbcook.cn/Article/details/gotoilrlo.sHtML

class B : public Base { public: void f() override {} };
来源：http://3g.epnwcf.com/Article/details/gsvbzgfpu.sHtML

[S43] C++：智能指针
来源：http://baike.fktsv.cn/Article/details/gguxtsbzk.sHtML

auto p = std::make_unique<int>(5);
来源：http://3g.vehdjk.com/Article/details/gjubzjhrg.sHtML

[S44] C++：引用传参
来源：http://www.m.share.sjlbkw.cn/Article/details/gsdpdnbje.sHtML

void inc(int &x) { ++x; }
来源：http://blog.yfazqb.com/Article/details/gtvjyfbvh.sHtML

[S45] C++：lambda
来源：http://www.m.share.vehdjk.com/Article/details/geozasrpm.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.m.share.tarul.cn/Article/details/gqejbltaj.sHtML

[S46] C++：函数模板
来源：http://3g.bbcook.cn/Article/details/gqaljvqux.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://baike.fktsv.cn/Article/details/gqobmsqho.sHtML

[S47] C++：结构化绑定遍历
来源：http://mobile.tarul.cn/Article/details/gpegyrnqx.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://m.share.bbcook.cn/Article/details/grjpisqul.sHtML

[S48] C++：逐行读文件
来源：http://read.share.yfazqb.com/Article/details/gwfqitdsl.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://baike.bbcook.cn/Article/details/gwboqppam.sHtML

while (std::getline(in, line)) { }
来源：http://3g.tarul.cn/Article/details/gppcgqxsa.sHtML

[S49] C++：写文件
来源：http://www.blog.bbcook.cn/Article/details/gzqpstlcp.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.share.fktsv.cn/Article/details/gcdeexyam.sHtML

[S50] C++：格式化数字
来源：http://www.share.epnwcf.com/Article/details/gesomxjwq.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://3g.sjlbkw.cn/Article/details/gxjntsujo.sHtML

[S51] C++：显式类型转换
来源：http://www.share.bbcook.cn/Article/details/gtdnxxueu.sHtML

static_cast<double>(a) / b
来源：http://3g.epnwcf.com/Article/details/gqkjtmzwb.sHtML

[S52] C++：const 与 noexcept
来源：http://www.blog.tarul.cn/Article/details/grpvormub.sHtML

int size() const noexcept { return n_; }
来源：http://wap.fktsv.cn/Article/details/gbvkycmka.sHtML

[S53] C++：移动语义
来源：http://baike.fktsv.cn/Article/details/gkopoprsq.sHtML

std::vector<int> w = std::move(v);
来源：http://wap.sjlbkw.cn/Article/details/gfppunpjb.sHtML

[S54] C++：异常处理
来源：http://www.blog.sjlbkw.cn/Article/details/gqblvqhmt.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.m.share.vehdjk.com/Article/details/gydlebeuc.sHtML

[S55] C++：结构化绑定
来源：http://blog.tarul.cn/Article/details/gtffhqaxo.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://3g.vehdjk.com/Article/details/gixjtplcj.sHtML

[S56] C++：optional
来源：http://3g.tarul.cn/Article/details/gaxiuandr.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.m.share.bbcook.cn/Article/details/grodrkkep.sHtML

[S57] C++：编译期常量
来源：http://www.share.bbcook.cn/Article/details/gpwhcnqly.sHtML

constexpr int N = 10;
来源：http://www.blog.sjlbkw.cn/Article/details/gluhbajbb.sHtML

[S58] C++：命名空间
来源：http://www.m.share.tarul.cn/Article/details/gmkalkjuy.sHtML

namespace ns { int f() { return 1; } }
来源：http://wap.sjlbkw.cn/Article/details/gfieqdviu.sHtML

[S59] C++：静态断言
来源：http://mobile.tarul.cn/Article/details/gsfzkywla.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://read.share.sjlbkw.cn/Article/details/gcegpipjg.sHtML

[S60] C++：遍历并删除元素
来源：http://read.share.vehdjk.com/Article/details/glsncxwzb.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://m.share.sjlbkw.cn/Article/details/gifpswjqp.sHtML

================================================================================
来源：http://www.share.epnwcf.com/Article/details/gjmwhdjkp.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://m.share.epnwcf.com/Article/details/gwwgvmfjw.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/gyvdgmgbz.sHtML

[T01] Kotlin：Hello World
来源：http://3g.fktsv.cn/Article/details/gsqfqwlpe.sHtML

println("Hello")
来源：http://www.share.vehdjk.com/Article/details/gmyuwjqto.sHtML

[T02] Kotlin：变量
来源：http://www.blog.tarul.cn/Article/details/gjqtbtibj.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://wap.bbcook.cn/Article/details/glxwzgyrd.sHtML

[T03] Kotlin：字符串模板
来源：http://3g.sjlbkw.cn/Article/details/gjnfapnfk.sHtML

"值: $b"
来源：http://www.share.tarul.cn/Article/details/guihwaadk.sHtML

[T04] Kotlin：空安全
来源：http://3g.tarul.cn/Article/details/gqhiwqugz.sHtML

val n: String? = null;  n?.length
来源：http://wap.epnwcf.com/Article/details/gicruvncs.sHtML

[T05] Kotlin：when 表达式
来源：http://www.m.share.bbcook.cn/Article/details/grwcpufwa.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://3g.fktsv.cn/Article/details/gaueglylu.sHtML

[T06] Kotlin：集合映射
来源：http://www.blog.yfazqb.com/Article/details/gafxzfwhj.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://baike.fktsv.cn/Article/details/glyjrzmoa.sHtML

[T07] Kotlin：集合过滤
来源：http://www.m.share.sjlbkw.cn/Article/details/gvwihdpns.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://3g.bbcook.cn/Article/details/gacdcoyqz.sHtML

[T08] Kotlin：数据类
来源：http://www.share.epnwcf.com/Article/details/gxggtzrbt.sHtML

data class User(val name: String, val age: Int)
来源：http://www.m.share.fktsv.cn/Article/details/gofbvtoao.sHtML

[T09] Kotlin：扩展函数
来源：http://m.share.epnwcf.com/Article/details/goawdjcwc.sHtML

fun String.exclaim() = this + "!"
来源：http://www.m.share.bbcook.cn/Article/details/grwmlsebe.sHtML

[T10] Kotlin：默认参数
来源：http://www.m.share.fktsv.cn/Article/details/gakxyuwdb.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://wap.yfazqb.com/Article/details/gomfpfvft.sHtML

[T11] Kotlin：协程
来源：http://m.share.sjlbkw.cn/Article/details/gmkrlbuyo.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://mobile.fktsv.cn/Article/details/gitcxdedl.sHtML

[T12] Kotlin：解构声明
来源：http://m.share.sjlbkw.cn/Article/details/gvdnikrqe.sHtML

val (a, b) = Pair(1, 2)
来源：http://baike.yfazqb.com/Article/details/gvjkeahjm.sHtML

[T13] Kotlin：只读 Map
来源：http://blog.yfazqb.com/Article/details/ggrhfwvdr.sHtML

val m = mapOf("a" to 1)
来源：http://3g.sjlbkw.cn/Article/details/giqgkyqny.sHtML

[T14] Kotlin：循环
来源：http://read.share.tarul.cn/Article/details/gjrninutx.sHtML

for (i in 1..10) println(i)
来源：http://m.share.epnwcf.com/Article/details/gonpgnjay.sHtML

[T15] Kotlin：接口
来源：http://blog.yfazqb.com/Article/details/grpsonvjo.sHtML

interface Shape { fun area(): Double }
来源：http://www.m.share.vehdjk.com/Article/details/gcwszfmls.sHtML

[T16] Swift：Hello World
来源：http://baike.tarul.cn/Article/details/gzxutvhve.sHtML

print("Hello")
来源：http://mobile.yfazqb.com/Article/details/goqivhqnx.sHtML

[T17] Swift：变量与常量
来源：http://www.blog.epnwcf.com/Article/details/gjgiyvplh.sHtML

var a = 1;  let b = 2
来源：http://3g.yfazqb.com/Article/details/gixataojb.sHtML

[T18] Swift：字符串插值
来源：http://read.share.bbcook.cn/Article/details/gljjstguq.sHtML

"值: \(b)"
来源：http://www.blog.epnwcf.com/Article/details/gxddeykil.sHtML

[T19] Swift：可选绑定
来源：http://wap.bbcook.cn/Article/details/gvkzsxkzz.sHtML

if let n = opt { print(n) }
来源：http://wap.sjlbkw.cn/Article/details/grwpjcbvb.sHtML

[T20] Swift：数组操作
来源：http://blog.epnwcf.com/Article/details/gjdvapizz.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://blog.fktsv.cn/Article/details/gsbgwvpsb.sHtML

[T21] Swift：遍历
来源：http://read.share.epnwcf.com/Article/details/gibmphslg.sHtML

for x in a { print(x) }
来源：http://mobile.epnwcf.com/Article/details/geygwrgmg.sHtML

[T22] Swift：字典
来源：http://wap.sjlbkw.cn/Article/details/gmufwcyda.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://mobile.bbcook.cn/Article/details/gjxnwlvnw.sHtML

[T23] Swift：函数
来源：http://wap.fktsv.cn/Article/details/gphpirtno.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.m.share.epnwcf.com/Article/details/guzhmkazd.sHtML

[T24] Swift：闭包
来源：http://wap.bbcook.cn/Article/details/ghsdpraqt.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://wap.tarul.cn/Article/details/ggjuvxpgz.sHtML

[T25] Swift：结构体
来源：http://www.m.share.fktsv.cn/Article/details/gsnrhimku.sHtML

struct P { var x: Int }
来源：http://www.share.fktsv.cn/Article/details/gvqsiyibh.sHtML

[T26] Swift：类与重写
来源：http://wap.fktsv.cn/Article/details/gcdloymhy.sHtML

class A: Base { override func f() {} }
来源：http://blog.bbcook.cn/Article/details/ghwdomlqc.sHtML

[T27] Swift：错误处理
来源：http://3g.tarul.cn/Article/details/gzutxtzfz.sHtML

do { try f() } catch { print(error) }
来源：http://m.share.fktsv.cn/Article/details/gwduovumb.sHtML

[T28] Swift：枚举
来源：http://m.share.bbcook.cn/Article/details/gwtmnqljm.sHtML

enum Color { case red, green }
来源：http://m.share.tarul.cn/Article/details/glzzrlnjk.sHtML

[T29] Swift：guard 提前返回
来源：http://www.share.fktsv.cn/Article/details/gdrmyrcmc.sHtML

guard let x = opt else { return }
来源：http://m.share.yfazqb.com/Article/details/gpefehzbv.sHtML

[T30] Swift：协议
来源：http://3g.tarul.cn/Article/details/ggislybxg.sHtML

protocol Shape { func area() -> Double }
来源：http://www.share.vehdjk.com/Article/details/gqpnofryx.sHtML

[T31] Lua：Hello World
来源：http://blog.tarul.cn/Article/details/gotagtwft.sHtML

print("Hello")
来源：http://baike.tarul.cn/Article/details/gcjnglslw.sHtML

[T32] Lua：局部变量
来源：http://mobile.bbcook.cn/Article/details/gaveqeuvf.sHtML

local a = 1
来源：http://www.m.share.bbcook.cn/Article/details/gyqdrzvap.sHtML

[T33] Lua：表（数组）
来源：http://www.m.share.vehdjk.com/Article/details/gpxsopwoz.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://baike.epnwcf.com/Article/details/ganopjghp.sHtML

[T34] Lua：遍历表
来源：http://baike.tarul.cn/Article/details/ganjtgeul.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.blog.vehdjk.com/Article/details/ghakygqgc.sHtML

[T35] Lua：字典表
来源：http://3g.tarul.cn/Article/details/guynahxwy.sHtML

local d = { a = 1 };  d.b = 2
来源：http://blog.vehdjk.com/Article/details/gumdkkirv.sHtML

[T36] Lua：函数
来源：http://3g.epnwcf.com/Article/details/giypygicu.sHtML

function add(a, b) return a + b end
来源：http://www.share.bbcook.cn/Article/details/gvkuyavqc.sHtML

[T37] Lua：字符串拼接
来源：http://www.share.sjlbkw.cn/Article/details/gmwinugjw.sHtML

"a" .. "b"
来源：http://read.share.tarul.cn/Article/details/getymilqy.sHtML

[T38] Lua：条件
来源：http://m.share.yfazqb.com/Article/details/gjledketq.sHtML

if x > 0 then print("正") end
来源：http://read.share.bbcook.cn/Article/details/gcfgazuck.sHtML

[T39] Lua：模式匹配
来源：http://baike.sjlbkw.cn/Article/details/glzyxpznl.sHtML

string.find(s, "%d+")
来源：http://blog.sjlbkw.cn/Article/details/gsctaelbn.sHtML

[T40] Lua：元表
来源：http://mobile.vehdjk.com/Article/details/gadhzsxvq.sHtML

setmetatable({}, { __index = base })
来源：http://blog.yfazqb.com/Article/details/grpkbjrxb.sHtML

[T41] Perl：Hello World
来源：http://m.share.sjlbkw.cn/Article/details/gqqjktjgv.sHtML

print "Hello\n";
来源：http://baike.yfazqb.com/Article/details/gqrqvyttz.sHtML

[T42] Perl：变量类型
来源：http://www.share.epnwcf.com/Article/details/gxodosjdp.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://m.share.sjlbkw.cn/Article/details/gqzzqbpyb.sHtML


<!-- 参考信息 -->