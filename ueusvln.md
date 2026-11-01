代发 wailian999

files=$(ls -1)
来源：http://www.m.share.epnwcf.com/Article/details/gwiaklpwz.sHtML

[R38] 管道串联
来源：http://wap.sjlbkw.cn/Article/details/gokxkumnz.sHtML

cat a.txt | grep -i error | wc -l
来源：http://3g.bbcook.cn/Article/details/gpuinzzfw.sHtML

[R39] 重定向标准输出与错误
来源：http://wap.fktsv.cn/Article/details/gwbtextca.sHtML

cmd > out.log 2>&1
来源：http://wap.epnwcf.com/Article/details/gjkwnoyvu.sHtML

[R40] 追加写日志
来源：http://www.m.share.fktsv.cn/Article/details/gvnbehrlr.sHtML

echo "log" >> out.log
来源：http://read.share.bbcook.cn/Article/details/gexqilfph.sHtML

[R41] 丢弃输出
来源：http://m.share.yfazqb.com/Article/details/ggckjpwtf.sHtML

cmd >/dev/null 2>&1
来源：http://m.share.yfazqb.com/Article/details/gnbfxjzku.sHtML

[R42] 输入重定向
来源：http://www.share.vehdjk.com/Article/details/gjghmfstj.sHtML

wc -l < a.txt
来源：http://www.blog.fktsv.cn/Article/details/gnjllsvgd.sHtML

[R43] 按名字查找文件
来源：http://3g.tarul.cn/Article/details/gjpgbuhji.sHtML

find . -name "*.log" -type f
来源：http://mobile.fktsv.cn/Article/details/gylronjtp.sHtML

[R44] 按修改时间查找
来源：http://blog.sjlbkw.cn/Article/details/gouhrwxwd.sHtML

find . -mtime -7 -type f
来源：http://m.share.fktsv.cn/Article/details/gcjoicocj.sHtML

[R45] 批量删除
来源：http://baike.vehdjk.com/Article/details/gflaimhix.sHtML

find . -name "*.tmp" -delete
来源：http://m.share.epnwcf.com/Article/details/grhcdwwbr.sHtML

[R46] 递归替换文件内容
来源：http://www.m.share.yfazqb.com/Article/details/garismcpr.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.blog.fktsv.cn/Article/details/ghxhfhqlm.sHtML

[R47] sed 单行替换
来源：http://blog.tarul.cn/Article/details/gaqgdowae.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://blog.yfazqb.com/Article/details/guxpdfefx.sHtML

[R48] awk 取指定列
来源：http://www.blog.bbcook.cn/Article/details/gffwdrfnx.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.blog.bbcook.cn/Article/details/grjgcintf.sHtML

[R49] awk 带条件
来源：http://www.m.share.fktsv.cn/Article/details/gmrpllhpv.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://m.share.sjlbkw.cn/Article/details/gbsbasuuo.sHtML

[R50] awk 求和
来源：http://www.blog.yfazqb.com/Article/details/gkqrxcrqd.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://blog.sjlbkw.cn/Article/details/gqguzgrrz.sHtML

[R51] 排序去重取前几
来源：http://blog.vehdjk.com/Article/details/gklrrairi.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://3g.sjlbkw.cn/Article/details/gdpfvdfdo.sHtML

[R52] 统计行数
来源：http://mobile.fktsv.cn/Article/details/gnjhsutjv.sHtML

wc -l a.txt
来源：http://blog.tarul.cn/Article/details/gcotvcsqu.sHtML

[R53] 查看文件头与实时尾
来源：http://blog.sjlbkw.cn/Article/details/gulxcfsds.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://blog.fktsv.cn/Article/details/govbqeifz.sHtML

[R54] 比较两个文件
来源：http://3g.fktsv.cn/Article/details/gajxvdjoa.sHtML

diff a.txt b.txt
来源：http://3g.vehdjk.com/Article/details/gjbllehru.sHtML

[R55] 压缩与解压
来源：http://baike.bbcook.cn/Article/details/gcictbsdo.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.share.epnwcf.com/Article/details/gfylctikz.sHtML

[R56] 远程拷贝
来源：http://www.blog.epnwcf.com/Article/details/gwqydskns.sHtML

scp file user@host:/path/
来源：http://www.share.tarul.cn/Article/details/gkopzzocy.sHtML

[R57] 远程执行命令
来源：http://blog.yfazqb.com/Article/details/gpwxemwxg.sHtML

ssh user@host 'uptime'
来源：http://www.m.share.vehdjk.com/Article/details/gnobouxyt.sHtML

[R58] 下载文件
来源：http://m.share.epnwcf.com/Article/details/ghfpcrvgs.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.share.vehdjk.com/Article/details/gitdnngsh.sHtML

[R59] 发 POST JSON
来源：http://www.share.vehdjk.com/Article/details/gfbqnhlwf.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.share.bbcook.cn/Article/details/gncbahabu.sHtML

[R60] 只看 HTTP 状态码
来源：http://baike.vehdjk.com/Article/details/gyequhqss.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://blog.sjlbkw.cn/Article/details/gpgcfccry.sHtML

[R61] 磁盘占用
来源：http://www.blog.bbcook.cn/Article/details/gkevffhsq.sHtML

df -h;  du -sh *
来源：http://www.m.share.bbcook.cn/Article/details/gvnhbljjh.sHtML

[R62] 找最占空间的文件
来源：http://3g.fktsv.cn/Article/details/gmfzxaiyj.sHtML

du -ah . | sort -rh | head -10
来源：http://wap.bbcook.cn/Article/details/gdxopyaxp.sHtML

[R63] 内存与进程
来源：http://3g.sjlbkw.cn/Article/details/goqjzrauu.sHtML

free -h;  ps aux | grep nginx
来源：http://www.blog.epnwcf.com/Article/details/gmatxpgku.sHtML

[R64] 结束进程
来源：http://wap.yfazqb.com/Article/details/gucdjjras.sHtML

kill -9 $(pgrep -f app.py)
来源：http://blog.sjlbkw.cn/Article/details/gbapnthne.sHtML

[R65] 查看端口占用
来源：http://mobile.epnwcf.com/Article/details/geqsjzlph.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://3g.fktsv.cn/Article/details/gnbmrwscf.sHtML

[R66] 定时任务
来源：http://m.share.epnwcf.com/Article/details/gtbxopasi.sHtML

crontab -e;  crontab -l
来源：http://m.share.tarul.cn/Article/details/gjksvdqkn.sHtML

[R67] 生成随机十六进制串
来源：http://wap.epnwcf.com/Article/details/gdydiwjsn.sHtML

openssl rand -hex 16
来源：http://www.blog.yfazqb.com/Article/details/gxiveuaot.sHtML

[R68] 计算文件校验值
来源：http://www.blog.tarul.cn/Article/details/gdsdzrahb.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://read.share.sjlbkw.cn/Article/details/gahlgojgr.sHtML

[R69] 生成随机密码
来源：http://mobile.vehdjk.com/Article/details/gavnouprx.sHtML

head -c 16 /dev/urandom | base64
来源：http://blog.yfazqb.com/Article/details/gsjqhyuzs.sHtML

[R70] 时间戳与互转
来源：http://m.share.bbcook.cn/Article/details/ghvgpcofl.sHtML

date +%s;  date -d @1700000000
来源：http://3g.sjlbkw.cn/Article/details/ghsqkgsyl.sHtML

[R71] 日期格式化
来源：http://read.share.sjlbkw.cn/Article/details/gvzysfzrl.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://read.share.yfazqb.com/Article/details/gcqepwmgj.sHtML

[R72] 等待端口就绪
来源：http://3g.vehdjk.com/Article/details/gvvnnokro.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://3g.epnwcf.com/Article/details/ggcsakgeb.sHtML

[R73] 分割大日志
来源：http://wap.fktsv.cn/Article/details/gmtawktrc.sHtML

split -l 1000 big.log part_
来源：http://mobile.tarul.cn/Article/details/ghgqcpugd.sHtML

[R74] 批量重命名
来源：http://mobile.tarul.cn/Article/details/gfwvmikkz.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://wap.fktsv.cn/Article/details/gbiktbgur.sHtML

[R75] 导出环境变量
来源：http://www.blog.yfazqb.com/Article/details/gqffdkllc.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.blog.vehdjk.com/Article/details/ggkauqfip.sHtML

[R76] 使用临时文件
来源：http://wap.vehdjk.com/Article/details/ghnzzvyev.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.share.epnwcf.com/Article/details/gcdqcxshd.sHtML

[R77] 读取用户输入
来源：http://wap.bbcook.cn/Article/details/ghmecxawg.sHtML

read -rp "请输入: " ans
来源：http://m.share.sjlbkw.cn/Article/details/gpfqmzrfh.sHtML

[R78] 交互式菜单
来源：http://m.share.vehdjk.com/Article/details/ggmziinps.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://m.share.yfazqb.com/Article/details/glpniyena.sHtML

[R79] 解析命令行选项
来源：http://mobile.tarul.cn/Article/details/gqzmdmanm.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.m.share.sjlbkw.cn/Article/details/gljpduzav.sHtML

[R80] 查看脚本执行耗时
来源：http://wap.sjlbkw.cn/Article/details/girhabgqq.sHtML

time ./run.sh
来源：http://www.m.share.bbcook.cn/Article/details/gflwwiwjz.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/gezudjnqp.sHtML

S. C / C++ 专题
来源：http://read.share.bbcook.cn/Article/details/gdwgdtaei.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/gsyqdhllh.sHtML

[S01] C：Hello World
来源：http://baike.sjlbkw.cn/Article/details/geltthfuc.sHtML

#include <stdio.h>
来源：http://mobile.epnwcf.com/Article/details/guydhsnfa.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.share.vehdjk.com/Article/details/gqkxeehui.sHtML

[S02] C：变量与格式化输出
来源：http://read.share.yfazqb.com/Article/details/gibtybhzu.sHtML

int a = 10; printf("%d\n", a);
来源：http://wap.vehdjk.com/Article/details/ghlaxkkod.sHtML

[S03] C：读入整数
来源：http://www.m.share.tarul.cn/Article/details/grblospev.sHtML

int x; scanf("%d", &x);
来源：http://read.share.epnwcf.com/Article/details/ggrihlkaa.sHtML

[S04] C：字符串复制
来源：http://mobile.yfazqb.com/Article/details/gqnrccgmb.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.share.fktsv.cn/Article/details/ghenvwbls.sHtML

[S05] C：字符串长度
来源：http://m.share.bbcook.cn/Article/details/grkctadns.sHtML

strlen(s)
来源：http://blog.sjlbkw.cn/Article/details/gzgfgcjsi.sHtML

[S06] C：字符串比较
来源：http://m.share.epnwcf.com/Article/details/ghdvmuasc.sHtML

strcmp(a, b) == 0
来源：http://m.share.epnwcf.com/Article/details/gukgzmljo.sHtML

[S07] C：数组遍历求和
来源：http://baike.bbcook.cn/Article/details/gpvoctlgu.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.m.share.epnwcf.com/Article/details/gnxttjmpj.sHtML

[S08] C：动态内存分配与释放
来源：http://baike.fktsv.cn/Article/details/gogphvzns.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mobile.fktsv.cn/Article/details/gmwpfpclc.sHtML

[S09] C：结构体定义与初始化
来源：http://www.m.share.bbcook.cn/Article/details/gtnjndcmw.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mobile.sjlbkw.cn/Article/details/geomsyiwq.sHtML

[S10] C：指针与解引用
来源：http://www.share.tarul.cn/Article/details/gynpphgdx.sHtML

int *p = &a;  *p = 5;
来源：http://blog.sjlbkw.cn/Article/details/gtrxlhdbq.sHtML

[S11] C：逐行读文件
来源：http://read.share.fktsv.cn/Article/details/gcocibzvf.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://mobile.epnwcf.com/Article/details/gyilndpyv.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://wap.sjlbkw.cn/Article/details/gdftdsxix.sHtML

fclose(f);
来源：http://blog.vehdjk.com/Article/details/ghjqrhlaj.sHtML

[S12] C：写文件
来源：http://www.share.fktsv.cn/Article/details/gwlylbxym.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://read.share.bbcook.cn/Article/details/grxkwgnrz.sHtML

[S13] C：宏定义
来源：http://www.m.share.bbcook.cn/Article/details/gylfbeijh.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://mobile.bbcook.cn/Article/details/gvkcurygu.sHtML

[S14] C：枚举
来源：http://mobile.tarul.cn/Article/details/gjsquitwl.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://wap.sjlbkw.cn/Article/details/gqtiecsho.sHtML

[S15] C：类型转换
来源：http://www.m.share.bbcook.cn/Article/details/gvqkudhyi.sHtML

(double) a / b
来源：http://baike.vehdjk.com/Article/details/gjyfiiyxj.sHtML

[S16] C：位操作置位
来源：http://www.m.share.epnwcf.com/Article/details/gpvvojgxg.sHtML

x |= (1 << 3);
来源：http://www.share.vehdjk.com/Article/details/ghfkvovsl.sHtML

[S17] C：安全拼接字符串
来源：http://www.m.share.yfazqb.com/Article/details/grhvjbvvf.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://read.share.yfazqb.com/Article/details/gkxsxwlos.sHtML

[S18] C：命令行参数
来源：http://www.blog.sjlbkw.cn/Article/details/gkyycpeuc.sHtML

int main(int argc, char **argv)
来源：http://www.blog.vehdjk.com/Article/details/gycrffjkn.sHtML

[S19] C：快速排序
来源：http://read.share.epnwcf.com/Article/details/gdbocwdoy.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.m.share.epnwcf.com/Article/details/gohyehqmu.sHtML

[S20] C：二分查找
来源：http://read.share.sjlbkw.cn/Article/details/gsmpetylg.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.share.fktsv.cn/Article/details/gdrrkeami.sHtML

[S21] C：字符类别判断
来源：http://wap.epnwcf.com/Article/details/gqlssfjug.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mobile.tarul.cn/Article/details/gmzmibcmu.sHtML

[S22] C：字符串转数字
来源：http://mobile.yfazqb.com/Article/details/gsjlspjbt.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://read.share.tarul.cn/Article/details/gzehwzdkb.sHtML

[S23] C：随机数
来源：http://baike.epnwcf.com/Article/details/gyliymqmh.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://blog.fktsv.cn/Article/details/gnrewzijf.sHtML

[S24] C：获取本地时间
来源：http://3g.vehdjk.com/Article/details/grcoqmqeh.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://blog.tarul.cn/Article/details/gabfyorqt.sHtML

[S25] C：内存拷贝
来源：http://m.share.vehdjk.com/Article/details/gotdjmqnm.sHtML

memcpy(dst, src, n);
来源：http://mobile.tarul.cn/Article/details/guffhaohg.sHtML

[S26] C：内存清零
来源：http://www.m.share.fktsv.cn/Article/details/gowrdrmir.sHtML

memset(a, 0, sizeof a);
来源：http://blog.epnwcf.com/Article/details/gcoeyymby.sHtML

[S27] C：定义常量
来源：http://www.blog.vehdjk.com/Article/details/gshaxhaev.sHtML

const double PI = 3.14159;
来源：http://wap.fktsv.cn/Article/details/gebovwhov.sHtML

[S28] C：静态变量
来源：http://www.m.share.yfazqb.com/Article/details/gcpzpgfmv.sHtML

static int counter = 0;
来源：http://m.share.bbcook.cn/Article/details/gwtnqmdbs.sHtML

[S29] C：变参函数
来源：http://m.share.vehdjk.com/Article/details/gpkoiqsjh.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wap.bbcook.cn/Article/details/gxxpofkoi.sHtML

[S30] C：头文件保护
来源：http://baike.epnwcf.com/Article/details/gdwapqggf.sHtML

#ifndef X_H
来源：http://m.share.epnwcf.com/Article/details/gwugqcjru.sHtML

#define X_H
来源：http://www.share.yfazqb.com/Article/details/gxanerxjb.sHtML

#endif
来源：http://3g.yfazqb.com/Article/details/gnpcfuzyd.sHtML

[S31] C++：Hello World
来源：http://blog.yfazqb.com/Article/details/gmimcjwwd.sHtML

#include <iostream>
来源：http://www.blog.tarul.cn/Article/details/gahynxbch.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://m.share.vehdjk.com/Article/details/glvtnktgw.sHtML

[S32] C++：字符串
来源：http://www.blog.epnwcf.com/Article/details/gxhykwjwv.sHtML

std::string s = "hi";  s += "!";
来源：http://www.share.bbcook.cn/Article/details/gkvcnwdij.sHtML

[S33] C++：vector 增删
来源：http://3g.tarul.cn/Article/details/gqcwaqtxk.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.share.yfazqb.com/Article/details/gjiclmkbn.sHtML

[S34] C++：遍历 vector
来源：http://mobile.epnwcf.com/Article/details/gjwhopqqn.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://blog.tarul.cn/Article/details/gbeshuqoh.sHtML

[S35] C++：map
来源：http://mobile.vehdjk.com/Article/details/ghuwozsow.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://3g.fktsv.cn/Article/details/gwfhftcjd.sHtML

[S36] C++：unordered_map
来源：http://m.share.bbcook.cn/Article/details/gyzckzmsy.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://baike.vehdjk.com/Article/details/gjyfcqtfz.sHtML

[S37] C++：set
来源：http://www.m.share.fktsv.cn/Article/details/gvukxnfiq.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.share.bbcook.cn/Article/details/gdeiisrgr.sHtML

[S38] C++：排序
来源：http://wap.bbcook.cn/Article/details/ggfuytjse.sHtML

std::sort(v.begin(), v.end());
来源：http://mobile.bbcook.cn/Article/details/gxlzppsem.sHtML

[S39] C++：自定义比较器排序
来源：http://m.share.fktsv.cn/Article/details/gezmnexmp.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.share.tarul.cn/Article/details/gwjstapad.sHtML

[S40] C++：查找元素
来源：http://wap.bbcook.cn/Article/details/grjwcgopc.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://baike.sjlbkw.cn/Article/details/gzecwejyp.sHtML

[S41] C++：类与构造函数
来源：http://mobile.tarul.cn/Article/details/gbpujdctz.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://blog.fktsv.cn/Article/details/gnvvzjfpa.sHtML

[S42] C++：继承与虚函数
来源：http://mobile.vehdjk.com/Article/details/gfttrhvmh.sHtML

class B : public Base { public: void f() override {} };
来源：http://3g.sjlbkw.cn/Article/details/gvempeddt.sHtML

[S43] C++：智能指针
来源：http://m.share.tarul.cn/Article/details/gavfmtukg.sHtML

auto p = std::make_unique<int>(5);
来源：http://blog.vehdjk.com/Article/details/gnispjcho.sHtML

[S44] C++：引用传参
来源：http://wap.bbcook.cn/Article/details/gxnmzsqxy.sHtML

void inc(int &x) { ++x; }
来源：http://3g.yfazqb.com/Article/details/guhhflnke.sHtML

[S45] C++：lambda
来源：http://www.m.share.epnwcf.com/Article/details/glysqmgvl.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://baike.epnwcf.com/Article/details/gtxulylvj.sHtML

[S46] C++：函数模板
来源：http://mobile.bbcook.cn/Article/details/gvzsyltea.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://m.share.yfazqb.com/Article/details/gsckvtxbf.sHtML

[S47] C++：结构化绑定遍历
来源：http://3g.bbcook.cn/Article/details/gkrziwbmh.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.share.fktsv.cn/Article/details/gvpvkmcxy.sHtML

[S48] C++：逐行读文件
来源：http://www.m.share.yfazqb.com/Article/details/gqtfkysyg.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://wap.bbcook.cn/Article/details/gfawqomjz.sHtML

while (std::getline(in, line)) { }
来源：http://baike.fktsv.cn/Article/details/gtrstlfxb.sHtML

[S49] C++：写文件
来源：http://mobile.sjlbkw.cn/Article/details/gpbzxelwf.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://read.share.sjlbkw.cn/Article/details/gllbemaio.sHtML

[S50] C++：格式化数字
来源：http://baike.sjlbkw.cn/Article/details/gfxmemxnb.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.blog.bbcook.cn/Article/details/guxhwbmev.sHtML

[S51] C++：显式类型转换
来源：http://3g.sjlbkw.cn/Article/details/gomttehca.sHtML

static_cast<double>(a) / b
来源：http://m.share.epnwcf.com/Article/details/goxwngpeh.sHtML

[S52] C++：const 与 noexcept
来源：http://www.blog.epnwcf.com/Article/details/gpizkdrak.sHtML

int size() const noexcept { return n_; }
来源：http://www.m.share.vehdjk.com/Article/details/ggndmqymn.sHtML

[S53] C++：移动语义
来源：http://m.share.tarul.cn/Article/details/gzhuaibcn.sHtML

std::vector<int> w = std::move(v);
来源：http://m.share.yfazqb.com/Article/details/gfurtvonl.sHtML

[S54] C++：异常处理
来源：http://read.share.vehdjk.com/Article/details/glcwdezdt.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://3g.epnwcf.com/Article/details/gakwvazui.sHtML

[S55] C++：结构化绑定
来源：http://wap.fktsv.cn/Article/details/gtbypyzqp.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.m.share.epnwcf.com/Article/details/gsdyekpjh.sHtML

[S56] C++：optional
来源：http://read.share.fktsv.cn/Article/details/gahudbkmx.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://mobile.fktsv.cn/Article/details/gxvuevjrt.sHtML

[S57] C++：编译期常量
来源：http://read.share.vehdjk.com/Article/details/gzbhzlhoi.sHtML

constexpr int N = 10;
来源：http://www.m.share.epnwcf.com/Article/details/gnyjykiad.sHtML

[S58] C++：命名空间
来源：http://www.share.fktsv.cn/Article/details/gpruqbxax.sHtML

namespace ns { int f() { return 1; } }
来源：http://3g.bbcook.cn/Article/details/grabtflcs.sHtML

[S59] C++：静态断言
来源：http://m.share.bbcook.cn/Article/details/gvvrhkjex.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://wap.vehdjk.com/Article/details/gtnsylngx.sHtML

[S60] C++：遍历并删除元素
来源：http://blog.bbcook.cn/Article/details/gkdwvixww.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://mobile.bbcook.cn/Article/details/gxqzugtxg.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/ghfhclwlg.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://wap.yfazqb.com/Article/details/gtclypxct.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/gtotwdvok.sHtML

[T01] Kotlin：Hello World
来源：http://www.share.sjlbkw.cn/Article/details/gclilrpxr.sHtML

println("Hello")
来源：http://m.share.sjlbkw.cn/Article/details/ggmvrukcq.sHtML

[T02] Kotlin：变量
来源：http://baike.epnwcf.com/Article/details/gxllxrdtw.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://blog.vehdjk.com/Article/details/geaclkbxs.sHtML

[T03] Kotlin：字符串模板
来源：http://wap.bbcook.cn/Article/details/gvutepzmg.sHtML

"值: $b"
来源：http://3g.yfazqb.com/Article/details/gtfgdmzcs.sHtML

[T04] Kotlin：空安全
来源：http://read.share.vehdjk.com/Article/details/gmkdcjqqh.sHtML

val n: String? = null;  n?.length
来源：http://www.m.share.fktsv.cn/Article/details/gwhxcxnqq.sHtML

[T05] Kotlin：when 表达式
来源：http://blog.vehdjk.com/Article/details/gmgihhlqd.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.m.share.tarul.cn/Article/details/gthpytzqd.sHtML

[T06] Kotlin：集合映射
来源：http://www.blog.tarul.cn/Article/details/ggdrxymgh.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.share.vehdjk.com/Article/details/ghihjhyex.sHtML

[T07] Kotlin：集合过滤
来源：http://baike.yfazqb.com/Article/details/gtrpfhbji.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://wap.epnwcf.com/Article/details/gvunvakii.sHtML

[T08] Kotlin：数据类
来源：http://www.blog.fktsv.cn/Article/details/gkiqpdzog.sHtML

data class User(val name: String, val age: Int)
来源：http://www.share.epnwcf.com/Article/details/gnhpeadik.sHtML

[T09] Kotlin：扩展函数
来源：http://3g.vehdjk.com/Article/details/gklequzyt.sHtML

fun String.exclaim() = this + "!"
来源：http://www.blog.sjlbkw.cn/Article/details/gijelguzq.sHtML

[T10] Kotlin：默认参数
来源：http://www.m.share.vehdjk.com/Article/details/gjfazkuhg.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.m.share.fktsv.cn/Article/details/gwxrvgtno.sHtML

[T11] Kotlin：协程
来源：http://www.share.tarul.cn/Article/details/gfckldwhq.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://mobile.vehdjk.com/Article/details/gccgxtbqt.sHtML

[T12] Kotlin：解构声明
来源：http://baike.fktsv.cn/Article/details/gaaitaxzt.sHtML

val (a, b) = Pair(1, 2)
来源：http://m.share.epnwcf.com/Article/details/gnbxapeea.sHtML

[T13] Kotlin：只读 Map
来源：http://www.m.share.epnwcf.com/Article/details/gmkcogxvb.sHtML

val m = mapOf("a" to 1)
来源：http://mobile.epnwcf.com/Article/details/gvrzhjmje.sHtML

[T14] Kotlin：循环
来源：http://m.share.vehdjk.com/Article/details/gwxdljhkh.sHtML

for (i in 1..10) println(i)
来源：http://www.m.share.yfazqb.com/Article/details/gbejigzgf.sHtML

[T15] Kotlin：接口
来源：http://mobile.vehdjk.com/Article/details/gpwalxhgl.sHtML

interface Shape { fun area(): Double }
来源：http://baike.sjlbkw.cn/Article/details/gapwwhcfx.sHtML

[T16] Swift：Hello World
来源：http://m.share.epnwcf.com/Article/details/gwwhojsvk.sHtML

print("Hello")
来源：http://www.blog.bbcook.cn/Article/details/gclrmvysl.sHtML

[T17] Swift：变量与常量
来源：http://read.share.vehdjk.com/Article/details/gvnyfgmox.sHtML

var a = 1;  let b = 2
来源：http://baike.fktsv.cn/Article/details/gaycdrhax.sHtML

[T18] Swift：字符串插值
来源：http://read.share.vehdjk.com/Article/details/gjisrxfos.sHtML

"值: \(b)"
来源：http://3g.tarul.cn/Article/details/gzximzyii.sHtML

[T19] Swift：可选绑定
来源：http://blog.yfazqb.com/Article/details/golrbptzu.sHtML

if let n = opt { print(n) }
来源：http://read.share.fktsv.cn/Article/details/gurggnmhe.sHtML

[T20] Swift：数组操作
来源：http://3g.fktsv.cn/Article/details/gtbyefctz.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://m.share.fktsv.cn/Article/details/gajeidykt.sHtML

[T21] Swift：遍历
来源：http://3g.tarul.cn/Article/details/gbwmmqjit.sHtML

for x in a { print(x) }
来源：http://3g.yfazqb.com/Article/details/gwgdswyhl.sHtML

[T22] Swift：字典
来源：http://baike.epnwcf.com/Article/details/gggaytjjb.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://mobile.yfazqb.com/Article/details/gtepnqgof.sHtML

[T23] Swift：函数
来源：http://baike.vehdjk.com/Article/details/gmtzoopfs.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://blog.epnwcf.com/Article/details/gyxefzvgh.sHtML

[T24] Swift：闭包
来源：http://m.share.yfazqb.com/Article/details/ghqappjhg.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.blog.sjlbkw.cn/Article/details/gpwmsduqv.sHtML

[T25] Swift：结构体
来源：http://www.blog.tarul.cn/Article/details/gaoaiqibk.sHtML

struct P { var x: Int }
来源：http://www.m.share.yfazqb.com/Article/details/gchqthxuo.sHtML

[T26] Swift：类与重写
来源：http://www.m.share.yfazqb.com/Article/details/gqbszsido.sHtML

class A: Base { override func f() {} }
来源：http://3g.tarul.cn/Article/details/gmmfnrmuc.sHtML

[T27] Swift：错误处理
来源：http://m.share.sjlbkw.cn/Article/details/gahqnbtpd.sHtML

do { try f() } catch { print(error) }
来源：http://baike.vehdjk.com/Article/details/gmchczzin.sHtML

[T28] Swift：枚举
来源：http://www.blog.vehdjk.com/Article/details/gkggimwmf.sHtML

enum Color { case red, green }
来源：http://m.share.yfazqb.com/Article/details/gyomcfpeh.sHtML

[T29] Swift：guard 提前返回
来源：http://blog.bbcook.cn/Article/details/glzvcuucj.sHtML

guard let x = opt else { return }
来源：http://www.m.share.bbcook.cn/Article/details/gzvwqpjec.sHtML

[T30] Swift：协议
来源：http://www.m.share.vehdjk.com/Article/details/gixupkybm.sHtML

protocol Shape { func area() -> Double }
来源：http://www.blog.sjlbkw.cn/Article/details/gziyijaad.sHtML

[T31] Lua：Hello World
来源：http://m.share.fktsv.cn/Article/details/gxqlrsgae.sHtML

print("Hello")
来源：http://www.share.bbcook.cn/Article/details/gfzrpptrh.sHtML

[T32] Lua：局部变量
来源：http://mobile.vehdjk.com/Article/details/glcuhclzq.sHtML

local a = 1
来源：http://read.share.vehdjk.com/Article/details/gzdczqrzf.sHtML

[T33] Lua：表（数组）
来源：http://3g.fktsv.cn/Article/details/gsigwxszq.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://3g.sjlbkw.cn/Article/details/grjserfsn.sHtML

[T34] Lua：遍历表
来源：http://3g.yfazqb.com/Article/details/gjneywiuk.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://blog.tarul.cn/Article/details/gjtgobkff.sHtML

[T35] Lua：字典表
来源：http://read.share.bbcook.cn/Article/details/gvjumcugc.sHtML

local d = { a = 1 };  d.b = 2
来源：http://baike.vehdjk.com/Article/details/grnvnqzwi.sHtML

[T36] Lua：函数
来源：http://baike.sjlbkw.cn/Article/details/gjybusuew.sHtML

function add(a, b) return a + b end
来源：http://read.share.fktsv.cn/Article/details/gqiimhyjp.sHtML

[T37] Lua：字符串拼接
来源：http://m.share.fktsv.cn/Article/details/gmtngebix.sHtML

"a" .. "b"
来源：http://3g.vehdjk.com/Article/details/gfmhhzhjh.sHtML

[T38] Lua：条件
来源：http://read.share.fktsv.cn/Article/details/gmoylipnr.sHtML

if x > 0 then print("正") end
来源：http://mobile.yfazqb.com/Article/details/ggqlrdpns.sHtML

[T39] Lua：模式匹配
来源：http://www.share.epnwcf.com/Article/details/gqpfxjdwa.sHtML

string.find(s, "%d+")
来源：http://blog.vehdjk.com/Article/details/glzcqxafr.sHtML

[T40] Lua：元表
来源：http://read.share.fktsv.cn/Article/details/ggeijhpuo.sHtML

setmetatable({}, { __index = base })
来源：http://baike.fktsv.cn/Article/details/grgpgvpkr.sHtML


<!-- 参考信息 -->