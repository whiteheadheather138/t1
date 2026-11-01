代发 wailian999

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://blog.vehdjk.com/Article/details/glntzyhwp.sHtML

[R34] 退出时清理
来源：http://www.blog.sjlbkw.cn/Article/details/galdusoas.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://3g.sjlbkw.cn/Article/details/gycrbjuqy.sHtML

[R35] 后台执行并等待
来源：http://read.share.vehdjk.com/Article/details/ggatwesfl.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.m.share.bbcook.cn/Article/details/gyrrrnije.sHtML

[R36] 并发执行多个任务
来源：http://baike.epnwcf.com/Article/details/ggyzyxijh.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.share.epnwcf.com/Article/details/gnlyquwle.sHtML

[R37] 把输出赋给变量
来源：http://www.share.sjlbkw.cn/Article/details/gkfygaomg.sHtML

files=$(ls -1)
来源：http://baike.epnwcf.com/Article/details/ghcukoczv.sHtML

[R38] 管道串联
来源：http://3g.tarul.cn/Article/details/ghejgvyof.sHtML

cat a.txt | grep -i error | wc -l
来源：http://m.share.yfazqb.com/Article/details/gjjppnqnn.sHtML

[R39] 重定向标准输出与错误
来源：http://baike.vehdjk.com/Article/details/ghbqoiawc.sHtML

cmd > out.log 2>&1
来源：http://wap.yfazqb.com/Article/details/gembzkirp.sHtML

[R40] 追加写日志
来源：http://3g.vehdjk.com/Article/details/glrwmiysa.sHtML

echo "log" >> out.log
来源：http://read.share.bbcook.cn/Article/details/gfmxkekjc.sHtML

[R41] 丢弃输出
来源：http://3g.epnwcf.com/Article/details/gzdqceebm.sHtML

cmd >/dev/null 2>&1
来源：http://3g.vehdjk.com/Article/details/grmakdekg.sHtML

[R42] 输入重定向
来源：http://read.share.bbcook.cn/Article/details/gummdrahc.sHtML

wc -l < a.txt
来源：http://www.share.vehdjk.com/Article/details/gnmxvlmbd.sHtML

[R43] 按名字查找文件
来源：http://blog.bbcook.cn/Article/details/gwqlewcex.sHtML

find . -name "*.log" -type f
来源：http://read.share.epnwcf.com/Article/details/gcutzrepd.sHtML

[R44] 按修改时间查找
来源：http://www.m.share.bbcook.cn/Article/details/gxrmjlsyp.sHtML

find . -mtime -7 -type f
来源：http://read.share.yfazqb.com/Article/details/gegopegjn.sHtML

[R45] 批量删除
来源：http://m.share.yfazqb.com/Article/details/gkkfkuiut.sHtML

find . -name "*.tmp" -delete
来源：http://www.share.yfazqb.com/Article/details/grqrzhvjt.sHtML

[R46] 递归替换文件内容
来源：http://www.share.fktsv.cn/Article/details/grwtygvbm.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.m.share.epnwcf.com/Article/details/galszroht.sHtML

[R47] sed 单行替换
来源：http://www.blog.yfazqb.com/Article/details/gablqkbjr.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://read.share.epnwcf.com/Article/details/gmvxaqaos.sHtML

[R48] awk 取指定列
来源：http://www.m.share.epnwcf.com/Article/details/ggutmwnry.sHtML

awk '{print $1, $3}' a.txt
来源：http://read.share.tarul.cn/Article/details/gqrcrrjzp.sHtML

[R49] awk 带条件
来源：http://mobile.epnwcf.com/Article/details/gtiryejcu.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.share.bbcook.cn/Article/details/gjdswwnbf.sHtML

[R50] awk 求和
来源：http://m.share.bbcook.cn/Article/details/gwiwvptym.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.m.share.vehdjk.com/Article/details/gcuqizjwb.sHtML

[R51] 排序去重取前几
来源：http://www.m.share.tarul.cn/Article/details/gjbgfplmc.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://mobile.tarul.cn/Article/details/gsxuclhbq.sHtML

[R52] 统计行数
来源：http://www.share.vehdjk.com/Article/details/gdziulffy.sHtML

wc -l a.txt
来源：http://m.share.sjlbkw.cn/Article/details/geefmzeeg.sHtML

[R53] 查看文件头与实时尾
来源：http://blog.sjlbkw.cn/Article/details/gbgvnjwis.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://m.share.vehdjk.com/Article/details/gufxlytqv.sHtML

[R54] 比较两个文件
来源：http://www.blog.tarul.cn/Article/details/gtsdsxvks.sHtML

diff a.txt b.txt
来源：http://m.share.epnwcf.com/Article/details/gesjzkzgl.sHtML

[R55] 压缩与解压
来源：http://baike.bbcook.cn/Article/details/goyvukpcz.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://blog.epnwcf.com/Article/details/gpozfuopf.sHtML

[R56] 远程拷贝
来源：http://read.share.sjlbkw.cn/Article/details/gkoqdljyk.sHtML

scp file user@host:/path/
来源：http://3g.sjlbkw.cn/Article/details/geldvvkmx.sHtML

[R57] 远程执行命令
来源：http://www.share.epnwcf.com/Article/details/gmselzjeh.sHtML

ssh user@host 'uptime'
来源：http://www.blog.tarul.cn/Article/details/goyobnldh.sHtML

[R58] 下载文件
来源：http://3g.yfazqb.com/Article/details/gmspohlqm.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://read.share.vehdjk.com/Article/details/geimrmfmj.sHtML

[R59] 发 POST JSON
来源：http://mobile.tarul.cn/Article/details/gsbykjiry.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://baike.tarul.cn/Article/details/gsjexbesf.sHtML

[R60] 只看 HTTP 状态码
来源：http://blog.bbcook.cn/Article/details/gdivubuyk.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mobile.yfazqb.com/Article/details/gdqjpvhny.sHtML

[R61] 磁盘占用
来源：http://blog.sjlbkw.cn/Article/details/goslgesyu.sHtML

df -h;  du -sh *
来源：http://www.share.sjlbkw.cn/Article/details/gfukghlnc.sHtML

[R62] 找最占空间的文件
来源：http://www.share.fktsv.cn/Article/details/gejqtdvet.sHtML

du -ah . | sort -rh | head -10
来源：http://www.share.sjlbkw.cn/Article/details/gjaqzbmau.sHtML

[R63] 内存与进程
来源：http://blog.fktsv.cn/Article/details/gxwhyamty.sHtML

free -h;  ps aux | grep nginx
来源：http://m.share.bbcook.cn/Article/details/gamrrthsd.sHtML

[R64] 结束进程
来源：http://blog.epnwcf.com/Article/details/gqmojsmsg.sHtML

kill -9 $(pgrep -f app.py)
来源：http://baike.epnwcf.com/Article/details/goardolid.sHtML

[R65] 查看端口占用
来源：http://www.share.epnwcf.com/Article/details/goxcjoewg.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.share.sjlbkw.cn/Article/details/ghhlkwkfz.sHtML

[R66] 定时任务
来源：http://baike.fktsv.cn/Article/details/grrtbpqjd.sHtML

crontab -e;  crontab -l
来源：http://mobile.yfazqb.com/Article/details/gdzdbbesc.sHtML

[R67] 生成随机十六进制串
来源：http://mobile.epnwcf.com/Article/details/gsohhwxrx.sHtML

openssl rand -hex 16
来源：http://blog.tarul.cn/Article/details/gzhlxwwlt.sHtML

[R68] 计算文件校验值
来源：http://wap.vehdjk.com/Article/details/gyvvyrond.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://blog.bbcook.cn/Article/details/goktqlthc.sHtML

[R69] 生成随机密码
来源：http://3g.epnwcf.com/Article/details/girkqsjca.sHtML

head -c 16 /dev/urandom | base64
来源：http://read.share.tarul.cn/Article/details/ghrfvskce.sHtML

[R70] 时间戳与互转
来源：http://baike.tarul.cn/Article/details/gxalqlqcj.sHtML

date +%s;  date -d @1700000000
来源：http://blog.epnwcf.com/Article/details/gtcsrlmfy.sHtML

[R71] 日期格式化
来源：http://www.blog.epnwcf.com/Article/details/ghmwecujm.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://m.share.sjlbkw.cn/Article/details/gnfzfcojq.sHtML

[R72] 等待端口就绪
来源：http://wap.tarul.cn/Article/details/gaflogrkg.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://blog.vehdjk.com/Article/details/gnqlcnbob.sHtML

[R73] 分割大日志
来源：http://baike.bbcook.cn/Article/details/gqerkuzli.sHtML

split -l 1000 big.log part_
来源：http://wap.tarul.cn/Article/details/gkfrdfjyq.sHtML

[R74] 批量重命名
来源：http://3g.vehdjk.com/Article/details/gavemkzyc.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://3g.fktsv.cn/Article/details/gizawavye.sHtML

[R75] 导出环境变量
来源：http://baike.bbcook.cn/Article/details/gmodggdsl.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://3g.vehdjk.com/Article/details/gmvsyktie.sHtML

[R76] 使用临时文件
来源：http://www.blog.yfazqb.com/Article/details/gbmatrolv.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://mobile.bbcook.cn/Article/details/gvljsldap.sHtML

[R77] 读取用户输入
来源：http://www.share.yfazqb.com/Article/details/gbtizdwzz.sHtML

read -rp "请输入: " ans
来源：http://read.share.sjlbkw.cn/Article/details/gerbgvxdi.sHtML

[R78] 交互式菜单
来源：http://www.share.tarul.cn/Article/details/gkztwjsuq.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://mobile.fktsv.cn/Article/details/gqsjwmput.sHtML

[R79] 解析命令行选项
来源：http://mobile.yfazqb.com/Article/details/gmkkvsikn.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.blog.tarul.cn/Article/details/gpnhbddzc.sHtML

[R80] 查看脚本执行耗时
来源：http://blog.fktsv.cn/Article/details/gdkypzanq.sHtML

time ./run.sh
来源：http://blog.sjlbkw.cn/Article/details/gqhlvbiby.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/gdmgbttkk.sHtML

S. C / C++ 专题
来源：http://m.share.vehdjk.com/Article/details/guplhoalp.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/gmoqnbnjq.sHtML

[S01] C：Hello World
来源：http://m.share.bbcook.cn/Article/details/ghhfrovbc.sHtML

#include <stdio.h>
来源：http://baike.epnwcf.com/Article/details/gbuwxzngq.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://mobile.bbcook.cn/Article/details/gtydqfvra.sHtML

[S02] C：变量与格式化输出
来源：http://www.blog.yfazqb.com/Article/details/gslktnggu.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.share.fktsv.cn/Article/details/gdsecsnxv.sHtML

[S03] C：读入整数
来源：http://m.share.tarul.cn/Article/details/gfvrnssdn.sHtML

int x; scanf("%d", &x);
来源：http://wap.vehdjk.com/Article/details/gxknopyzz.sHtML

[S04] C：字符串复制
来源：http://www.share.tarul.cn/Article/details/gzzrybbbv.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://mobile.yfazqb.com/Article/details/gxhxqixlg.sHtML

[S05] C：字符串长度
来源：http://blog.epnwcf.com/Article/details/ghmzzzsmv.sHtML

strlen(s)
来源：http://www.blog.fktsv.cn/Article/details/gwccpdyqs.sHtML

[S06] C：字符串比较
来源：http://read.share.vehdjk.com/Article/details/gopjmfmra.sHtML

strcmp(a, b) == 0
来源：http://read.share.yfazqb.com/Article/details/gxdrizszq.sHtML

[S07] C：数组遍历求和
来源：http://m.share.tarul.cn/Article/details/gkeizrclu.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.share.bbcook.cn/Article/details/gwovyxkfx.sHtML

[S08] C：动态内存分配与释放
来源：http://baike.sjlbkw.cn/Article/details/gvbztakru.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.m.share.yfazqb.com/Article/details/ggrdlddbk.sHtML

[S09] C：结构体定义与初始化
来源：http://wap.vehdjk.com/Article/details/gvlrmonkd.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://read.share.bbcook.cn/Article/details/gmszdoorx.sHtML

[S10] C：指针与解引用
来源：http://read.share.sjlbkw.cn/Article/details/ghbtnpubf.sHtML

int *p = &a;  *p = 5;
来源：http://baike.epnwcf.com/Article/details/gxacmtgah.sHtML

[S11] C：逐行读文件
来源：http://mobile.sjlbkw.cn/Article/details/giylofqpy.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.blog.sjlbkw.cn/Article/details/gdzgdfbkm.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://m.share.bbcook.cn/Article/details/gkgrrxnsf.sHtML

fclose(f);
来源：http://m.share.tarul.cn/Article/details/gnodqtcur.sHtML

[S12] C：写文件
来源：http://wap.sjlbkw.cn/Article/details/gmutfhfny.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://m.share.sjlbkw.cn/Article/details/gwigwpzkv.sHtML

[S13] C：宏定义
来源：http://m.share.tarul.cn/Article/details/gykpcnfiq.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://read.share.tarul.cn/Article/details/gikopszpb.sHtML

[S14] C：枚举
来源：http://www.blog.fktsv.cn/Article/details/glbifmwmn.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://3g.yfazqb.com/Article/details/gheyugjui.sHtML

[S15] C：类型转换
来源：http://wap.yfazqb.com/Article/details/gzfdfymku.sHtML

(double) a / b
来源：http://3g.tarul.cn/Article/details/gepptkzze.sHtML

[S16] C：位操作置位
来源：http://mobile.vehdjk.com/Article/details/ggffyrhev.sHtML

x |= (1 << 3);
来源：http://www.share.bbcook.cn/Article/details/ggfzrmakh.sHtML

[S17] C：安全拼接字符串
来源：http://baike.vehdjk.com/Article/details/gnglpqarj.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.m.share.vehdjk.com/Article/details/gvkmgffwq.sHtML

[S18] C：命令行参数
来源：http://www.m.share.fktsv.cn/Article/details/gqlatncod.sHtML

int main(int argc, char **argv)
来源：http://read.share.vehdjk.com/Article/details/gesehzjya.sHtML

[S19] C：快速排序
来源：http://mobile.vehdjk.com/Article/details/gpgbvaiym.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://3g.epnwcf.com/Article/details/gwjldyelj.sHtML

[S20] C：二分查找
来源：http://www.share.fktsv.cn/Article/details/gtgoezaxl.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://read.share.tarul.cn/Article/details/glypcfeny.sHtML

[S21] C：字符类别判断
来源：http://www.blog.sjlbkw.cn/Article/details/gnqdwesnk.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://m.share.vehdjk.com/Article/details/gdyureeyc.sHtML

[S22] C：字符串转数字
来源：http://www.m.share.fktsv.cn/Article/details/gxkacvvcx.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://baike.fktsv.cn/Article/details/grkshmhhs.sHtML

[S23] C：随机数
来源：http://www.share.tarul.cn/Article/details/gopmlwvme.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.share.tarul.cn/Article/details/gqqiidyqb.sHtML

[S24] C：获取本地时间
来源：http://baike.fktsv.cn/Article/details/gfyieijav.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.m.share.sjlbkw.cn/Article/details/gmvdtcbmv.sHtML

[S25] C：内存拷贝
来源：http://read.share.vehdjk.com/Article/details/gmpciyrou.sHtML

memcpy(dst, src, n);
来源：http://baike.vehdjk.com/Article/details/girhcknue.sHtML

[S26] C：内存清零
来源：http://www.blog.sjlbkw.cn/Article/details/gdshbkcbs.sHtML

memset(a, 0, sizeof a);
来源：http://www.m.share.sjlbkw.cn/Article/details/gczijjoaa.sHtML

[S27] C：定义常量
来源：http://read.share.yfazqb.com/Article/details/gwfvrlwnv.sHtML

const double PI = 3.14159;
来源：http://mobile.vehdjk.com/Article/details/gccwxhaik.sHtML

[S28] C：静态变量
来源：http://www.blog.vehdjk.com/Article/details/gegsnqngy.sHtML

static int counter = 0;
来源：http://www.blog.fktsv.cn/Article/details/gdjjgtakp.sHtML

[S29] C：变参函数
来源：http://blog.fktsv.cn/Article/details/gjequvwqy.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://blog.yfazqb.com/Article/details/ghoasonxq.sHtML

[S30] C：头文件保护
来源：http://www.share.bbcook.cn/Article/details/gbqhphudx.sHtML

#ifndef X_H
来源：http://www.share.yfazqb.com/Article/details/goyqktmxl.sHtML

#define X_H
来源：http://blog.fktsv.cn/Article/details/guglrgbld.sHtML

#endif
来源：http://www.blog.bbcook.cn/Article/details/gwfgvgbgp.sHtML

[S31] C++：Hello World
来源：http://blog.vehdjk.com/Article/details/godfwnkor.sHtML

#include <iostream>
来源：http://blog.bbcook.cn/Article/details/gfdmglqhz.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://read.share.tarul.cn/Article/details/gkdglqqie.sHtML

[S32] C++：字符串
来源：http://wap.fktsv.cn/Article/details/gwtgnfnxj.sHtML

std::string s = "hi";  s += "!";
来源：http://www.m.share.fktsv.cn/Article/details/gowhcsbim.sHtML

[S33] C++：vector 增删
来源：http://mobile.fktsv.cn/Article/details/gdjectteq.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://m.share.sjlbkw.cn/Article/details/gjcbgeybi.sHtML

[S34] C++：遍历 vector
来源：http://www.m.share.vehdjk.com/Article/details/gfqtdcjdz.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://m.share.yfazqb.com/Article/details/gbcvurcjp.sHtML

[S35] C++：map
来源：http://www.blog.yfazqb.com/Article/details/gdlgyefvl.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://blog.yfazqb.com/Article/details/gtttqcsvx.sHtML

[S36] C++：unordered_map
来源：http://mobile.vehdjk.com/Article/details/gjzzwrwxc.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wap.sjlbkw.cn/Article/details/gsnqynkdp.sHtML

[S37] C++：set
来源：http://www.blog.bbcook.cn/Article/details/gtcvehjbd.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://m.share.sjlbkw.cn/Article/details/goyioyser.sHtML

[S38] C++：排序
来源：http://read.share.vehdjk.com/Article/details/gbsovxpri.sHtML

std::sort(v.begin(), v.end());
来源：http://baike.vehdjk.com/Article/details/gzbahqwdo.sHtML

[S39] C++：自定义比较器排序
来源：http://mobile.sjlbkw.cn/Article/details/gekjckpfy.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://mobile.vehdjk.com/Article/details/gqqnxlaiw.sHtML

[S40] C++：查找元素
来源：http://blog.sjlbkw.cn/Article/details/gowxcoumr.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://baike.fktsv.cn/Article/details/glpvfkigi.sHtML

[S41] C++：类与构造函数
来源：http://wap.vehdjk.com/Article/details/gnrxttwia.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://blog.fktsv.cn/Article/details/gwlpezsdw.sHtML

[S42] C++：继承与虚函数
来源：http://read.share.fktsv.cn/Article/details/gbkowhmpp.sHtML

class B : public Base { public: void f() override {} };
来源：http://read.share.yfazqb.com/Article/details/grnpmlvwz.sHtML

[S43] C++：智能指针
来源：http://read.share.vehdjk.com/Article/details/gclhqnfou.sHtML

auto p = std::make_unique<int>(5);
来源：http://wap.bbcook.cn/Article/details/gtbzdyexk.sHtML

[S44] C++：引用传参
来源：http://mobile.vehdjk.com/Article/details/gdsgnpxiy.sHtML

void inc(int &x) { ++x; }
来源：http://mobile.epnwcf.com/Article/details/geafyexee.sHtML

[S45] C++：lambda
来源：http://m.share.tarul.cn/Article/details/gexbofxiq.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://3g.vehdjk.com/Article/details/gmpcjjpas.sHtML

[S46] C++：函数模板
来源：http://read.share.yfazqb.com/Article/details/gfliuglig.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.blog.fktsv.cn/Article/details/gbjhgfnew.sHtML

[S47] C++：结构化绑定遍历
来源：http://m.share.epnwcf.com/Article/details/ggwdmufmc.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.blog.sjlbkw.cn/Article/details/gjoznrsah.sHtML

[S48] C++：逐行读文件
来源：http://mobile.vehdjk.com/Article/details/gspttlnzv.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://wap.sjlbkw.cn/Article/details/gjtbhvtfq.sHtML

while (std::getline(in, line)) { }
来源：http://3g.fktsv.cn/Article/details/gzwlpirbj.sHtML

[S49] C++：写文件
来源：http://read.share.sjlbkw.cn/Article/details/gvoackdua.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.m.share.epnwcf.com/Article/details/gasgywqjb.sHtML

[S50] C++：格式化数字
来源：http://m.share.bbcook.cn/Article/details/gziljshvc.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://blog.epnwcf.com/Article/details/gdzvftoee.sHtML

[S51] C++：显式类型转换
来源：http://wap.epnwcf.com/Article/details/giztlcejn.sHtML

static_cast<double>(a) / b
来源：http://m.share.vehdjk.com/Article/details/gcunqjcfv.sHtML

[S52] C++：const 与 noexcept
来源：http://wap.sjlbkw.cn/Article/details/gcvrevbpj.sHtML

int size() const noexcept { return n_; }
来源：http://www.m.share.fktsv.cn/Article/details/goqlwnkny.sHtML

[S53] C++：移动语义
来源：http://wap.vehdjk.com/Article/details/ghnxwueuj.sHtML

std::vector<int> w = std::move(v);
来源：http://m.share.bbcook.cn/Article/details/gctqwpwpf.sHtML

[S54] C++：异常处理
来源：http://www.m.share.yfazqb.com/Article/details/gscatgigj.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://m.share.fktsv.cn/Article/details/grlrmeqwi.sHtML

[S55] C++：结构化绑定
来源：http://www.share.yfazqb.com/Article/details/gnxufzvxx.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://read.share.tarul.cn/Article/details/gzdaqgawc.sHtML

[S56] C++：optional
来源：http://mobile.epnwcf.com/Article/details/gejiivxru.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wap.yfazqb.com/Article/details/gdgordnqg.sHtML

[S57] C++：编译期常量
来源：http://www.share.epnwcf.com/Article/details/grtzwchkx.sHtML

constexpr int N = 10;
来源：http://3g.vehdjk.com/Article/details/gyzezyycx.sHtML

[S58] C++：命名空间
来源：http://wap.tarul.cn/Article/details/gyifhteku.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.m.share.tarul.cn/Article/details/gzosvoswl.sHtML

[S59] C++：静态断言
来源：http://www.m.share.yfazqb.com/Article/details/gvaxsluqp.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.share.epnwcf.com/Article/details/geyevhnha.sHtML

[S60] C++：遍历并删除元素
来源：http://read.share.bbcook.cn/Article/details/gboyaleyc.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://mobile.tarul.cn/Article/details/gdjdhatks.sHtML

================================================================================
来源：http://wap.vehdjk.com/Article/details/gwpqzvgvf.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.epnwcf.com/Article/details/gxtcodqyw.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/gsqbfydus.sHtML

[T01] Kotlin：Hello World
来源：http://www.blog.fktsv.cn/Article/details/gacwspjbi.sHtML

println("Hello")
来源：http://www.m.share.bbcook.cn/Article/details/gpkdbvwhx.sHtML

[T02] Kotlin：变量
来源：http://wap.yfazqb.com/Article/details/grqjrzfhn.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://3g.vehdjk.com/Article/details/ggxumfrvw.sHtML

[T03] Kotlin：字符串模板
来源：http://read.share.yfazqb.com/Article/details/gaglttvic.sHtML

"值: $b"
来源：http://wap.bbcook.cn/Article/details/gvhboceqj.sHtML

[T04] Kotlin：空安全
来源：http://blog.epnwcf.com/Article/details/gzqkvjaik.sHtML

val n: String? = null;  n?.length
来源：http://m.share.sjlbkw.cn/Article/details/ghsxijggo.sHtML

[T05] Kotlin：when 表达式
来源：http://www.m.share.bbcook.cn/Article/details/gmfgflkzd.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://blog.tarul.cn/Article/details/gdxaptnft.sHtML

[T06] Kotlin：集合映射
来源：http://mobile.bbcook.cn/Article/details/gjtywhagn.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://3g.epnwcf.com/Article/details/gxntlypgq.sHtML

[T07] Kotlin：集合过滤
来源：http://blog.fktsv.cn/Article/details/gyqxgmpbs.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://blog.tarul.cn/Article/details/guknsxxxu.sHtML

[T08] Kotlin：数据类
来源：http://www.m.share.bbcook.cn/Article/details/grasswbnt.sHtML

data class User(val name: String, val age: Int)
来源：http://wap.epnwcf.com/Article/details/gmnmrfxfj.sHtML

[T09] Kotlin：扩展函数
来源：http://www.share.yfazqb.com/Article/details/ggvzntaaz.sHtML

fun String.exclaim() = this + "!"
来源：http://www.m.share.vehdjk.com/Article/details/gegvyklzd.sHtML

[T10] Kotlin：默认参数
来源：http://3g.bbcook.cn/Article/details/ghgdqocjo.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://blog.bbcook.cn/Article/details/gevivlhqo.sHtML

[T11] Kotlin：协程
来源：http://www.m.share.sjlbkw.cn/Article/details/gvrepreqv.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.blog.vehdjk.com/Article/details/griqhissa.sHtML

[T12] Kotlin：解构声明
来源：http://blog.tarul.cn/Article/details/gognpbmos.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.share.fktsv.cn/Article/details/gplmyjent.sHtML

[T13] Kotlin：只读 Map
来源：http://mobile.fktsv.cn/Article/details/ghoduzzkr.sHtML

val m = mapOf("a" to 1)
来源：http://www.share.epnwcf.com/Article/details/gnchbzpde.sHtML

[T14] Kotlin：循环
来源：http://wap.vehdjk.com/Article/details/gybuyusfe.sHtML

for (i in 1..10) println(i)
来源：http://wap.sjlbkw.cn/Article/details/gnxsutnum.sHtML

[T15] Kotlin：接口
来源：http://www.m.share.fktsv.cn/Article/details/gyscohede.sHtML

interface Shape { fun area(): Double }
来源：http://www.share.fktsv.cn/Article/details/grdahvfzj.sHtML

[T16] Swift：Hello World
来源：http://baike.vehdjk.com/Article/details/ghqhcjnzk.sHtML

print("Hello")
来源：http://www.m.share.yfazqb.com/Article/details/gzggcbwav.sHtML

[T17] Swift：变量与常量
来源：http://www.m.share.vehdjk.com/Article/details/gsastkezk.sHtML

var a = 1;  let b = 2
来源：http://www.m.share.tarul.cn/Article/details/gjitfgvfr.sHtML

[T18] Swift：字符串插值
来源：http://www.share.vehdjk.com/Article/details/gauuakmol.sHtML

"值: \(b)"
来源：http://3g.yfazqb.com/Article/details/gakddpfyk.sHtML

[T19] Swift：可选绑定
来源：http://www.share.yfazqb.com/Article/details/gddeokyzo.sHtML

if let n = opt { print(n) }
来源：http://mobile.bbcook.cn/Article/details/gdctgowtd.sHtML

[T20] Swift：数组操作
来源：http://3g.tarul.cn/Article/details/gvygiruyg.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://read.share.fktsv.cn/Article/details/gvpbonpjt.sHtML

[T21] Swift：遍历
来源：http://3g.fktsv.cn/Article/details/gnjkqnuxu.sHtML

for x in a { print(x) }
来源：http://m.share.bbcook.cn/Article/details/gjuzfdwfq.sHtML

[T22] Swift：字典
来源：http://baike.bbcook.cn/Article/details/gkpgnarye.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://m.share.yfazqb.com/Article/details/gfjqupdyg.sHtML

[T23] Swift：函数
来源：http://read.share.sjlbkw.cn/Article/details/gttamxqwa.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://blog.epnwcf.com/Article/details/gawcavusk.sHtML

[T24] Swift：闭包
来源：http://3g.yfazqb.com/Article/details/gcdwcrwpv.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://wap.fktsv.cn/Article/details/gftaomwzc.sHtML

[T25] Swift：结构体
来源：http://www.share.tarul.cn/Article/details/gyfzwlxrb.sHtML

struct P { var x: Int }
来源：http://www.m.share.sjlbkw.cn/Article/details/gjisaghmu.sHtML

[T26] Swift：类与重写
来源：http://wap.tarul.cn/Article/details/gdckfyeka.sHtML

class A: Base { override func f() {} }
来源：http://wap.fktsv.cn/Article/details/gmqfvqwkp.sHtML

[T27] Swift：错误处理
来源：http://m.share.sjlbkw.cn/Article/details/gwlzygpem.sHtML

do { try f() } catch { print(error) }
来源：http://wap.tarul.cn/Article/details/goyavgaar.sHtML

[T28] Swift：枚举
来源：http://www.m.share.epnwcf.com/Article/details/grttobwng.sHtML

enum Color { case red, green }
来源：http://www.m.share.yfazqb.com/Article/details/grhaitabh.sHtML

[T29] Swift：guard 提前返回
来源：http://baike.yfazqb.com/Article/details/gfsyaczcm.sHtML

guard let x = opt else { return }
来源：http://3g.vehdjk.com/Article/details/gulkvjlls.sHtML

[T30] Swift：协议
来源：http://read.share.fktsv.cn/Article/details/ggygkfqlt.sHtML

protocol Shape { func area() -> Double }
来源：http://www.m.share.fktsv.cn/Article/details/gcbzbhzes.sHtML

[T31] Lua：Hello World
来源：http://blog.epnwcf.com/Article/details/gxvoipwbs.sHtML

print("Hello")
来源：http://www.share.bbcook.cn/Article/details/gjkxhrmhy.sHtML

[T32] Lua：局部变量
来源：http://baike.bbcook.cn/Article/details/gndxpcobe.sHtML

local a = 1
来源：http://baike.vehdjk.com/Article/details/guxsdcvxb.sHtML

[T33] Lua：表（数组）
来源：http://www.share.epnwcf.com/Article/details/gskfmnyzk.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://m.share.bbcook.cn/Article/details/gppggmasq.sHtML

[T34] Lua：遍历表
来源：http://read.share.epnwcf.com/Article/details/gihxlqgko.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://read.share.tarul.cn/Article/details/gmkbtzhmp.sHtML

[T35] Lua：字典表
来源：http://baike.epnwcf.com/Article/details/gihaneifl.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.m.share.epnwcf.com/Article/details/gxjzohpde.sHtML

[T36] Lua：函数
来源：http://www.share.yfazqb.com/Article/details/gytckinkm.sHtML

function add(a, b) return a + b end
来源：http://mobile.tarul.cn/Article/details/gtzejscfb.sHtML


<!-- 参考信息 -->