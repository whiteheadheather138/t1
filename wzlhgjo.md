代发 wailian999

files=$(ls -1)
来源：http://www.m.share.epnwcf.com/Article/details/gxklebdnz.sHtML

[R38] 管道串联
来源：http://mobile.tarul.cn/Article/details/gokklbkoh.sHtML

cat a.txt | grep -i error | wc -l
来源：http://blog.sjlbkw.cn/Article/details/gttmecqfj.sHtML

[R39] 重定向标准输出与错误
来源：http://wap.fktsv.cn/Article/details/ghfoqhtoe.sHtML

cmd > out.log 2>&1
来源：http://mobile.epnwcf.com/Article/details/gguoqjwsf.sHtML

[R40] 追加写日志
来源：http://www.share.sjlbkw.cn/Article/details/gcohbosdb.sHtML

echo "log" >> out.log
来源：http://baike.epnwcf.com/Article/details/ghnxjfwhv.sHtML

[R41] 丢弃输出
来源：http://read.share.vehdjk.com/Article/details/grckaboax.sHtML

cmd >/dev/null 2>&1
来源：http://read.share.epnwcf.com/Article/details/gwmbpizte.sHtML

[R42] 输入重定向
来源：http://www.share.sjlbkw.cn/Article/details/gkkplzpbb.sHtML

wc -l < a.txt
来源：http://baike.fktsv.cn/Article/details/gvtxrkuht.sHtML

[R43] 按名字查找文件
来源：http://3g.epnwcf.com/Article/details/gynqczyuz.sHtML

find . -name "*.log" -type f
来源：http://baike.sjlbkw.cn/Article/details/guwkhozci.sHtML

[R44] 按修改时间查找
来源：http://m.share.vehdjk.com/Article/details/glazslddw.sHtML

find . -mtime -7 -type f
来源：http://read.share.vehdjk.com/Article/details/gtmxplgxf.sHtML

[R45] 批量删除
来源：http://3g.fktsv.cn/Article/details/gajyzrglt.sHtML

find . -name "*.tmp" -delete
来源：http://www.m.share.bbcook.cn/Article/details/ggfiirkch.sHtML

[R46] 递归替换文件内容
来源：http://blog.bbcook.cn/Article/details/gvbqzgrxc.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.m.share.vehdjk.com/Article/details/ggjnldkpu.sHtML

[R47] sed 单行替换
来源：http://wap.yfazqb.com/Article/details/gmlyspquj.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://mobile.tarul.cn/Article/details/gjedgffmp.sHtML

[R48] awk 取指定列
来源：http://3g.sjlbkw.cn/Article/details/gyxwgeeut.sHtML

awk '{print $1, $3}' a.txt
来源：http://mobile.vehdjk.com/Article/details/ggoxgqrml.sHtML

[R49] awk 带条件
来源：http://www.blog.vehdjk.com/Article/details/gbpaiveop.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://m.share.bbcook.cn/Article/details/gqilkhaqy.sHtML

[R50] awk 求和
来源：http://www.blog.fktsv.cn/Article/details/gyhjylida.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://blog.fktsv.cn/Article/details/garroyiyk.sHtML

[R51] 排序去重取前几
来源：http://mobile.epnwcf.com/Article/details/gufwfyjor.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://read.share.sjlbkw.cn/Article/details/gvrlgnsod.sHtML

[R52] 统计行数
来源：http://www.blog.sjlbkw.cn/Article/details/gniamcmja.sHtML

wc -l a.txt
来源：http://m.share.yfazqb.com/Article/details/geqovqwea.sHtML

[R53] 查看文件头与实时尾
来源：http://www.share.tarul.cn/Article/details/gcvxiecix.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://3g.epnwcf.com/Article/details/gwvsccuol.sHtML

[R54] 比较两个文件
来源：http://m.share.epnwcf.com/Article/details/gqbbaqkux.sHtML

diff a.txt b.txt
来源：http://mobile.epnwcf.com/Article/details/gflvyqkqe.sHtML

[R55] 压缩与解压
来源：http://www.share.tarul.cn/Article/details/gawvxpspa.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://read.share.epnwcf.com/Article/details/govfynjgs.sHtML

[R56] 远程拷贝
来源：http://m.share.epnwcf.com/Article/details/gfqbatgnw.sHtML

scp file user@host:/path/
来源：http://3g.vehdjk.com/Article/details/gaujbtmia.sHtML

[R57] 远程执行命令
来源：http://read.share.yfazqb.com/Article/details/gihazbujk.sHtML

ssh user@host 'uptime'
来源：http://www.share.vehdjk.com/Article/details/grfzutqfe.sHtML

[R58] 下载文件
来源：http://www.share.vehdjk.com/Article/details/gvbnxgxyy.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://baike.bbcook.cn/Article/details/gshtlfmll.sHtML

[R59] 发 POST JSON
来源：http://m.share.sjlbkw.cn/Article/details/gcsjcbrxw.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://mobile.sjlbkw.cn/Article/details/gvauesipx.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.share.sjlbkw.cn/Article/details/gndsuaizt.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://blog.tarul.cn/Article/details/gozkbuprj.sHtML

[R61] 磁盘占用
来源：http://blog.vehdjk.com/Article/details/gymbapxct.sHtML

df -h;  du -sh *
来源：http://3g.epnwcf.com/Article/details/grpeszspn.sHtML

[R62] 找最占空间的文件
来源：http://www.share.vehdjk.com/Article/details/gpfsmzbmh.sHtML

du -ah . | sort -rh | head -10
来源：http://www.share.bbcook.cn/Article/details/gekifpbri.sHtML

[R63] 内存与进程
来源：http://3g.vehdjk.com/Article/details/giknyuqem.sHtML

free -h;  ps aux | grep nginx
来源：http://wap.vehdjk.com/Article/details/gdqduduqx.sHtML

[R64] 结束进程
来源：http://baike.tarul.cn/Article/details/grlbcgqhv.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.blog.bbcook.cn/Article/details/ghsyjsbjh.sHtML

[R65] 查看端口占用
来源：http://www.share.sjlbkw.cn/Article/details/gdigfqtuk.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mobile.bbcook.cn/Article/details/gbgobkcsb.sHtML

[R66] 定时任务
来源：http://www.m.share.tarul.cn/Article/details/glymmlhbm.sHtML

crontab -e;  crontab -l
来源：http://www.share.fktsv.cn/Article/details/gbyjbmxbq.sHtML

[R67] 生成随机十六进制串
来源：http://mobile.sjlbkw.cn/Article/details/gicionwem.sHtML

openssl rand -hex 16
来源：http://read.share.epnwcf.com/Article/details/gvtvrrxgk.sHtML

[R68] 计算文件校验值
来源：http://baike.sjlbkw.cn/Article/details/gxlmtwtcn.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.blog.tarul.cn/Article/details/gcyyyopxc.sHtML

[R69] 生成随机密码
来源：http://m.share.vehdjk.com/Article/details/gkntxswxy.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.m.share.vehdjk.com/Article/details/gsqqzgbki.sHtML

[R70] 时间戳与互转
来源：http://read.share.sjlbkw.cn/Article/details/gfxhxfhzi.sHtML

date +%s;  date -d @1700000000
来源：http://www.m.share.bbcook.cn/Article/details/gbwltrgtz.sHtML

[R71] 日期格式化
来源：http://www.blog.epnwcf.com/Article/details/gskgeglop.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://wap.yfazqb.com/Article/details/gqpwqwawh.sHtML

[R72] 等待端口就绪
来源：http://mobile.vehdjk.com/Article/details/gufzdmlvp.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://read.share.epnwcf.com/Article/details/gnnvdjucj.sHtML

[R73] 分割大日志
来源：http://www.share.sjlbkw.cn/Article/details/gfgzclnix.sHtML

split -l 1000 big.log part_
来源：http://mobile.epnwcf.com/Article/details/glymadynr.sHtML

[R74] 批量重命名
来源：http://wap.fktsv.cn/Article/details/gagzevuey.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.share.yfazqb.com/Article/details/gywqqlmqa.sHtML

[R75] 导出环境变量
来源：http://www.share.yfazqb.com/Article/details/gvlnonucw.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://wap.epnwcf.com/Article/details/gpvmtnxmx.sHtML

[R76] 使用临时文件
来源：http://m.share.sjlbkw.cn/Article/details/grbqchfyj.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://wap.sjlbkw.cn/Article/details/gxbnyhrjr.sHtML

[R77] 读取用户输入
来源：http://m.share.tarul.cn/Article/details/gngcmyvmx.sHtML

read -rp "请输入: " ans
来源：http://www.share.epnwcf.com/Article/details/ggjkufwpd.sHtML

[R78] 交互式菜单
来源：http://3g.epnwcf.com/Article/details/grtyvkkbl.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://m.share.vehdjk.com/Article/details/goloknlvw.sHtML

[R79] 解析命令行选项
来源：http://www.blog.epnwcf.com/Article/details/gvbihajsk.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.blog.vehdjk.com/Article/details/gikppiefz.sHtML

[R80] 查看脚本执行耗时
来源：http://read.share.vehdjk.com/Article/details/gagfirdgi.sHtML

time ./run.sh
来源：http://blog.yfazqb.com/Article/details/gpglyoulu.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/geyxvajat.sHtML

S. C / C++ 专题
来源：http://wap.tarul.cn/Article/details/gnndlwtry.sHtML

================================================================================
来源：http://blog.vehdjk.com/Article/details/gbnxtgpkq.sHtML

[S01] C：Hello World
来源：http://blog.fktsv.cn/Article/details/guldugdpk.sHtML

#include <stdio.h>
来源：http://3g.vehdjk.com/Article/details/gbijwaizc.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.share.tarul.cn/Article/details/gwkzanxtd.sHtML

[S02] C：变量与格式化输出
来源：http://wap.yfazqb.com/Article/details/gjpvepvwt.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.m.share.fktsv.cn/Article/details/gvmbxxoqy.sHtML

[S03] C：读入整数
来源：http://baike.epnwcf.com/Article/details/ggxlafwyg.sHtML

int x; scanf("%d", &x);
来源：http://wap.sjlbkw.cn/Article/details/gzvvfdtmw.sHtML

[S04] C：字符串复制
来源：http://www.share.sjlbkw.cn/Article/details/gqjpamgjp.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.share.sjlbkw.cn/Article/details/gdqcyagth.sHtML

[S05] C：字符串长度
来源：http://m.share.bbcook.cn/Article/details/gxzuqxnru.sHtML

strlen(s)
来源：http://mobile.bbcook.cn/Article/details/gxqbhgnjk.sHtML

[S06] C：字符串比较
来源：http://mobile.vehdjk.com/Article/details/gsusauykw.sHtML

strcmp(a, b) == 0
来源：http://www.blog.tarul.cn/Article/details/gvstbmrez.sHtML

[S07] C：数组遍历求和
来源：http://www.share.epnwcf.com/Article/details/gltxcvybp.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://3g.yfazqb.com/Article/details/gcitkisbx.sHtML

[S08] C：动态内存分配与释放
来源：http://www.blog.epnwcf.com/Article/details/gfkexjsbu.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://wap.bbcook.cn/Article/details/geogaezpv.sHtML

[S09] C：结构体定义与初始化
来源：http://blog.sjlbkw.cn/Article/details/gvaenyitg.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.m.share.epnwcf.com/Article/details/gfdhxgxyy.sHtML

[S10] C：指针与解引用
来源：http://blog.epnwcf.com/Article/details/gdxhjzthg.sHtML

int *p = &a;  *p = 5;
来源：http://www.share.tarul.cn/Article/details/goolswwuz.sHtML

[S11] C：逐行读文件
来源：http://3g.vehdjk.com/Article/details/ggbqebrjj.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://read.share.epnwcf.com/Article/details/gruwiyfar.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://baike.fktsv.cn/Article/details/gyniwpike.sHtML

fclose(f);
来源：http://www.m.share.tarul.cn/Article/details/gkjetlwgr.sHtML

[S12] C：写文件
来源：http://wap.vehdjk.com/Article/details/ghbdaffpq.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://3g.yfazqb.com/Article/details/gmypswlet.sHtML

[S13] C：宏定义
来源：http://www.share.epnwcf.com/Article/details/gughjlqlj.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://baike.tarul.cn/Article/details/giypjhtct.sHtML

[S14] C：枚举
来源：http://read.share.bbcook.cn/Article/details/gtetecqoh.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://read.share.epnwcf.com/Article/details/gwlnyyhef.sHtML

[S15] C：类型转换
来源：http://www.m.share.bbcook.cn/Article/details/gjpkcfryj.sHtML

(double) a / b
来源：http://m.share.yfazqb.com/Article/details/gqqixqpuh.sHtML

[S16] C：位操作置位
来源：http://wap.vehdjk.com/Article/details/gniqcqghr.sHtML

x |= (1 << 3);
来源：http://www.m.share.bbcook.cn/Article/details/gsiypuueh.sHtML

[S17] C：安全拼接字符串
来源：http://m.share.bbcook.cn/Article/details/gsudtmbis.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://baike.epnwcf.com/Article/details/gciqufuna.sHtML

[S18] C：命令行参数
来源：http://www.share.epnwcf.com/Article/details/gkovztigb.sHtML

int main(int argc, char **argv)
来源：http://3g.epnwcf.com/Article/details/gfaifjgsj.sHtML

[S19] C：快速排序
来源：http://blog.sjlbkw.cn/Article/details/gnwfsdlgq.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://wap.yfazqb.com/Article/details/gegsptktw.sHtML

[S20] C：二分查找
来源：http://www.blog.bbcook.cn/Article/details/gtjrqtblw.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.m.share.sjlbkw.cn/Article/details/gqheoogmc.sHtML

[S21] C：字符类别判断
来源：http://www.blog.epnwcf.com/Article/details/gbwhqwhjn.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mobile.fktsv.cn/Article/details/ggulhzjfv.sHtML

[S22] C：字符串转数字
来源：http://m.share.epnwcf.com/Article/details/glzmxysgl.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://wap.fktsv.cn/Article/details/gpjtobwxe.sHtML

[S23] C：随机数
来源：http://3g.vehdjk.com/Article/details/gzzoeekyh.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://wap.vehdjk.com/Article/details/gkdhrrlqu.sHtML

[S24] C：获取本地时间
来源：http://www.m.share.vehdjk.com/Article/details/goenqnsfg.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://baike.yfazqb.com/Article/details/gqwoguvbw.sHtML

[S25] C：内存拷贝
来源：http://wap.fktsv.cn/Article/details/gudhhaajx.sHtML

memcpy(dst, src, n);
来源：http://blog.fktsv.cn/Article/details/gnyynxsgn.sHtML

[S26] C：内存清零
来源：http://read.share.tarul.cn/Article/details/gtioltueu.sHtML

memset(a, 0, sizeof a);
来源：http://www.share.sjlbkw.cn/Article/details/gpnfqkdjc.sHtML

[S27] C：定义常量
来源：http://read.share.yfazqb.com/Article/details/gzvmuebjh.sHtML

const double PI = 3.14159;
来源：http://www.blog.epnwcf.com/Article/details/gwvbdsyfz.sHtML

[S28] C：静态变量
来源：http://read.share.bbcook.cn/Article/details/gpfetaviq.sHtML

static int counter = 0;
来源：http://3g.yfazqb.com/Article/details/gcnjkxjgm.sHtML

[S29] C：变参函数
来源：http://wap.sjlbkw.cn/Article/details/gwahtkilb.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.blog.yfazqb.com/Article/details/gpleqmhar.sHtML

[S30] C：头文件保护
来源：http://www.blog.vehdjk.com/Article/details/gflplpsyg.sHtML

#ifndef X_H
来源：http://mobile.bbcook.cn/Article/details/gqxaygmkm.sHtML

#define X_H
来源：http://www.blog.bbcook.cn/Article/details/girekrmxz.sHtML

#endif
来源：http://www.share.bbcook.cn/Article/details/gvixvcfkm.sHtML

[S31] C++：Hello World
来源：http://wap.tarul.cn/Article/details/gauimkuiq.sHtML

#include <iostream>
来源：http://m.share.fktsv.cn/Article/details/gsxoocxmw.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://baike.yfazqb.com/Article/details/gxiemnapg.sHtML

[S32] C++：字符串
来源：http://read.share.epnwcf.com/Article/details/gpairdcxv.sHtML

std::string s = "hi";  s += "!";
来源：http://mobile.vehdjk.com/Article/details/gozarxjib.sHtML

[S33] C++：vector 增删
来源：http://blog.yfazqb.com/Article/details/gkatrtgot.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://read.share.fktsv.cn/Article/details/gxcpqhzux.sHtML

[S34] C++：遍历 vector
来源：http://www.blog.epnwcf.com/Article/details/gjiaemeug.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://baike.epnwcf.com/Article/details/gqtprqsyy.sHtML

[S35] C++：map
来源：http://baike.sjlbkw.cn/Article/details/gjfjsgalq.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://blog.epnwcf.com/Article/details/gjffoajrm.sHtML

[S36] C++：unordered_map
来源：http://www.blog.bbcook.cn/Article/details/gwdhlztuq.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.sjlbkw.cn/Article/details/gxwcbnyzx.sHtML

[S37] C++：set
来源：http://read.share.sjlbkw.cn/Article/details/gbtkoyaym.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://baike.bbcook.cn/Article/details/gkyjwehmj.sHtML

[S38] C++：排序
来源：http://m.share.bbcook.cn/Article/details/gylsvyxrw.sHtML

std::sort(v.begin(), v.end());
来源：http://m.share.vehdjk.com/Article/details/gettkpbsw.sHtML

[S39] C++：自定义比较器排序
来源：http://3g.yfazqb.com/Article/details/gefsrpeha.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://blog.epnwcf.com/Article/details/gkvdwpdjw.sHtML

[S40] C++：查找元素
来源：http://read.share.bbcook.cn/Article/details/guxlkfyac.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://3g.epnwcf.com/Article/details/geronrylb.sHtML

[S41] C++：类与构造函数
来源：http://3g.bbcook.cn/Article/details/gveuuzwvx.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://wap.yfazqb.com/Article/details/gnekuvisa.sHtML

[S42] C++：继承与虚函数
来源：http://www.blog.bbcook.cn/Article/details/gctbtbxun.sHtML

class B : public Base { public: void f() override {} };
来源：http://blog.bbcook.cn/Article/details/gnpqvucsz.sHtML

[S43] C++：智能指针
来源：http://m.share.tarul.cn/Article/details/gryacaqzq.sHtML

auto p = std::make_unique<int>(5);
来源：http://mobile.tarul.cn/Article/details/gwlbdmxrd.sHtML

[S44] C++：引用传参
来源：http://mobile.vehdjk.com/Article/details/gxikhcovr.sHtML

void inc(int &x) { ++x; }
来源：http://wap.yfazqb.com/Article/details/gfmrztdmj.sHtML

[S45] C++：lambda
来源：http://wap.fktsv.cn/Article/details/gnkoiequv.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://read.share.fktsv.cn/Article/details/glpuyqvgd.sHtML

[S46] C++：函数模板
来源：http://baike.tarul.cn/Article/details/gleakknhe.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://wap.epnwcf.com/Article/details/garhozzlv.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.share.vehdjk.com/Article/details/ghuwbseas.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://baike.yfazqb.com/Article/details/ganypbukv.sHtML

[S48] C++：逐行读文件
来源：http://baike.sjlbkw.cn/Article/details/gefirwuzm.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.m.share.vehdjk.com/Article/details/getqtgmsw.sHtML

while (std::getline(in, line)) { }
来源：http://m.share.vehdjk.com/Article/details/gveqwyajg.sHtML

[S49] C++：写文件
来源：http://wap.vehdjk.com/Article/details/gutztbwnb.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://blog.fktsv.cn/Article/details/geupblwno.sHtML

[S50] C++：格式化数字
来源：http://read.share.bbcook.cn/Article/details/guejtcnok.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://read.share.yfazqb.com/Article/details/grnpehkra.sHtML

[S51] C++：显式类型转换
来源：http://blog.fktsv.cn/Article/details/gfguasuzb.sHtML

static_cast<double>(a) / b
来源：http://baike.vehdjk.com/Article/details/gupmlcnrg.sHtML

[S52] C++：const 与 noexcept
来源：http://www.blog.yfazqb.com/Article/details/gbdavquiw.sHtML

int size() const noexcept { return n_; }
来源：http://blog.bbcook.cn/Article/details/grnftkksl.sHtML

[S53] C++：移动语义
来源：http://mobile.epnwcf.com/Article/details/gfdgddqkw.sHtML

std::vector<int> w = std::move(v);
来源：http://baike.fktsv.cn/Article/details/gkbkrgura.sHtML

[S54] C++：异常处理
来源：http://www.blog.vehdjk.com/Article/details/gzltdeytb.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://read.share.epnwcf.com/Article/details/gevrvleby.sHtML

[S55] C++：结构化绑定
来源：http://wap.tarul.cn/Article/details/grlmwniwl.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://wap.tarul.cn/Article/details/gwcgwifge.sHtML

[S56] C++：optional
来源：http://wap.yfazqb.com/Article/details/gufjetxot.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://baike.epnwcf.com/Article/details/guequdiqk.sHtML

[S57] C++：编译期常量
来源：http://m.share.fktsv.cn/Article/details/gzdpjoyrc.sHtML

constexpr int N = 10;
来源：http://www.share.fktsv.cn/Article/details/gyvzpkavx.sHtML

[S58] C++：命名空间
来源：http://www.m.share.yfazqb.com/Article/details/grbafgqul.sHtML

namespace ns { int f() { return 1; } }
来源：http://blog.yfazqb.com/Article/details/gqdcfhncf.sHtML

[S59] C++：静态断言
来源：http://wap.fktsv.cn/Article/details/glgrcatnn.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.share.vehdjk.com/Article/details/gqvmnrcrb.sHtML

[S60] C++：遍历并删除元素
来源：http://www.blog.tarul.cn/Article/details/ghdafjvyc.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://blog.yfazqb.com/Article/details/gyfhaytdx.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/gcpfurkxh.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://m.share.tarul.cn/Article/details/ghzscknfr.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/gdtwdijuo.sHtML

[T01] Kotlin：Hello World
来源：http://baike.yfazqb.com/Article/details/gpdcewiua.sHtML

println("Hello")
来源：http://wap.bbcook.cn/Article/details/geemvxrlq.sHtML

[T02] Kotlin：变量
来源：http://baike.bbcook.cn/Article/details/gsuqxflmd.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://read.share.yfazqb.com/Article/details/gflfjyrmn.sHtML

[T03] Kotlin：字符串模板
来源：http://mobile.tarul.cn/Article/details/gqynzuggj.sHtML

"值: $b"
来源：http://read.share.bbcook.cn/Article/details/gtdvieuts.sHtML

[T04] Kotlin：空安全
来源：http://www.share.bbcook.cn/Article/details/gmffbvlvy.sHtML

val n: String? = null;  n?.length
来源：http://baike.yfazqb.com/Article/details/gymlivorp.sHtML

[T05] Kotlin：when 表达式
来源：http://mobile.vehdjk.com/Article/details/gutgarygh.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://m.share.epnwcf.com/Article/details/gmmahxqos.sHtML

[T06] Kotlin：集合映射
来源：http://www.m.share.epnwcf.com/Article/details/gndqavovj.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://read.share.fktsv.cn/Article/details/gtgzyfood.sHtML

[T07] Kotlin：集合过滤
来源：http://m.share.fktsv.cn/Article/details/grnkbxaot.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://blog.yfazqb.com/Article/details/gilxyhsji.sHtML

[T08] Kotlin：数据类
来源：http://read.share.tarul.cn/Article/details/grzxccoak.sHtML

data class User(val name: String, val age: Int)
来源：http://3g.tarul.cn/Article/details/gwxoeuoyx.sHtML

[T09] Kotlin：扩展函数
来源：http://blog.vehdjk.com/Article/details/gecicztet.sHtML

fun String.exclaim() = this + "!"
来源：http://read.share.epnwcf.com/Article/details/gltovuscb.sHtML

[T10] Kotlin：默认参数
来源：http://baike.tarul.cn/Article/details/gqsmfbrov.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://baike.sjlbkw.cn/Article/details/gwgwefjvt.sHtML

[T11] Kotlin：协程
来源：http://mobile.vehdjk.com/Article/details/gqqetygbt.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.blog.sjlbkw.cn/Article/details/gzcqosvsn.sHtML

[T12] Kotlin：解构声明
来源：http://wap.sjlbkw.cn/Article/details/gvxfcgqiu.sHtML

val (a, b) = Pair(1, 2)
来源：http://3g.tarul.cn/Article/details/gvaiomdlj.sHtML

[T13] Kotlin：只读 Map
来源：http://baike.bbcook.cn/Article/details/ggzgqcxhp.sHtML

val m = mapOf("a" to 1)
来源：http://3g.epnwcf.com/Article/details/gnxrvuwxw.sHtML

[T14] Kotlin：循环
来源：http://www.blog.bbcook.cn/Article/details/gtbruuirq.sHtML

for (i in 1..10) println(i)
来源：http://www.m.share.sjlbkw.cn/Article/details/gnlmotjcs.sHtML

[T15] Kotlin：接口
来源：http://www.share.epnwcf.com/Article/details/grilfduuj.sHtML

interface Shape { fun area(): Double }
来源：http://wap.epnwcf.com/Article/details/gignmxsdm.sHtML

[T16] Swift：Hello World
来源：http://baike.bbcook.cn/Article/details/gbtjwlixx.sHtML

print("Hello")
来源：http://www.blog.fktsv.cn/Article/details/gmaszadlm.sHtML

[T17] Swift：变量与常量
来源：http://read.share.yfazqb.com/Article/details/glktclvol.sHtML

var a = 1;  let b = 2
来源：http://m.share.yfazqb.com/Article/details/gcwmdthdp.sHtML

[T18] Swift：字符串插值
来源：http://www.blog.fktsv.cn/Article/details/gsozshtfu.sHtML

"值: \(b)"
来源：http://www.m.share.epnwcf.com/Article/details/gzmnpgamq.sHtML

[T19] Swift：可选绑定
来源：http://www.blog.epnwcf.com/Article/details/gawjzdfsd.sHtML

if let n = opt { print(n) }
来源：http://read.share.yfazqb.com/Article/details/guljifprb.sHtML

[T20] Swift：数组操作
来源：http://mobile.bbcook.cn/Article/details/gvgjsqfwe.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://wap.vehdjk.com/Article/details/gbmfnnvwb.sHtML

[T21] Swift：遍历
来源：http://www.blog.sjlbkw.cn/Article/details/ghdpzglfu.sHtML

for x in a { print(x) }
来源：http://wap.sjlbkw.cn/Article/details/glqekkdei.sHtML

[T22] Swift：字典
来源：http://read.share.tarul.cn/Article/details/gybmdlohm.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://baike.tarul.cn/Article/details/gdqhngvel.sHtML

[T23] Swift：函数
来源：http://www.m.share.sjlbkw.cn/Article/details/gunukeolm.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.blog.yfazqb.com/Article/details/geuzmglvt.sHtML

[T24] Swift：闭包
来源：http://www.blog.tarul.cn/Article/details/gptftudhx.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://read.share.fktsv.cn/Article/details/getumjvyk.sHtML

[T25] Swift：结构体
来源：http://www.share.tarul.cn/Article/details/gxflhpbon.sHtML

struct P { var x: Int }
来源：http://wap.yfazqb.com/Article/details/gippatdni.sHtML

[T26] Swift：类与重写
来源：http://www.m.share.bbcook.cn/Article/details/ghklulzxf.sHtML

class A: Base { override func f() {} }
来源：http://www.m.share.vehdjk.com/Article/details/gbfiqfoog.sHtML

[T27] Swift：错误处理
来源：http://3g.fktsv.cn/Article/details/gpggjxcfz.sHtML

do { try f() } catch { print(error) }
来源：http://mobile.fktsv.cn/Article/details/gagmtqgua.sHtML

[T28] Swift：枚举
来源：http://www.m.share.fktsv.cn/Article/details/gmlriavmu.sHtML

enum Color { case red, green }
来源：http://www.blog.epnwcf.com/Article/details/gxnipshbz.sHtML

[T29] Swift：guard 提前返回
来源：http://www.m.share.bbcook.cn/Article/details/grxpdmnge.sHtML

guard let x = opt else { return }
来源：http://mobile.sjlbkw.cn/Article/details/goerbdugr.sHtML

[T30] Swift：协议
来源：http://baike.vehdjk.com/Article/details/gffosndeo.sHtML

protocol Shape { func area() -> Double }
来源：http://blog.bbcook.cn/Article/details/gddxxzujk.sHtML

[T31] Lua：Hello World
来源：http://mobile.sjlbkw.cn/Article/details/gvlahbuie.sHtML

print("Hello")
来源：http://baike.vehdjk.com/Article/details/gydjpnhnm.sHtML

[T32] Lua：局部变量
来源：http://read.share.epnwcf.com/Article/details/gqdyukefx.sHtML

local a = 1
来源：http://www.blog.vehdjk.com/Article/details/gdjqvrpsx.sHtML

[T33] Lua：表（数组）
来源：http://www.share.bbcook.cn/Article/details/gwzfethad.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.share.tarul.cn/Article/details/gxthtitaj.sHtML

[T34] Lua：遍历表
来源：http://m.share.yfazqb.com/Article/details/ggljdgqry.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://wap.bbcook.cn/Article/details/gveqadsfv.sHtML

[T35] Lua：字典表
来源：http://www.m.share.yfazqb.com/Article/details/gxzeyspdl.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.blog.yfazqb.com/Article/details/guljikbuw.sHtML

[T36] Lua：函数
来源：http://baike.yfazqb.com/Article/details/gtsgznlgf.sHtML

function add(a, b) return a + b end
来源：http://www.blog.vehdjk.com/Article/details/gdefxwfav.sHtML

[T37] Lua：字符串拼接
来源：http://wap.epnwcf.com/Article/details/gmhrlgayt.sHtML

"a" .. "b"
来源：http://read.share.tarul.cn/Article/details/gvkjjyqkz.sHtML

[T38] Lua：条件
来源：http://www.share.fktsv.cn/Article/details/gluvfgawx.sHtML

if x > 0 then print("正") end
来源：http://www.m.share.vehdjk.com/Article/details/gjlobvqsb.sHtML

[T39] Lua：模式匹配
来源：http://www.share.bbcook.cn/Article/details/gcfmoyuhn.sHtML

string.find(s, "%d+")
来源：http://www.share.fktsv.cn/Article/details/gaziqeeod.sHtML

[T40] Lua：元表
来源：http://baike.tarul.cn/Article/details/glfissjys.sHtML

setmetatable({}, { __index = base })
来源：http://m.share.sjlbkw.cn/Article/details/ggchibtzw.sHtML


<!-- 参考信息 -->