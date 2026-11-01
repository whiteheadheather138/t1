代发 wailian999

f() { local x=1; echo "$x"; }
来源：http://www.blog.fktsv.cn/Article/details/gpboiowyg.sHtML

[R32] 参数个数校验
来源：http://m.share.sjlbkw.cn/Article/details/ghxfzzxgh.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://3g.epnwcf.com/Article/details/gqrnoenrs.sHtML

[R33] 捕获错误并提示行号
来源：http://m.share.sjlbkw.cn/Article/details/gzdysewvw.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.m.share.vehdjk.com/Article/details/ggtgnbidp.sHtML

[R34] 退出时清理
来源：http://3g.tarul.cn/Article/details/gjapjhsln.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://mobile.tarul.cn/Article/details/gggotuzoi.sHtML

[R35] 后台执行并等待
来源：http://read.share.fktsv.cn/Article/details/gjuenicgc.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://3g.fktsv.cn/Article/details/ggcxhprnh.sHtML

[R36] 并发执行多个任务
来源：http://www.blog.sjlbkw.cn/Article/details/gzjnvtjsf.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.blog.epnwcf.com/Article/details/gpidzfqrd.sHtML

[R37] 把输出赋给变量
来源：http://m.share.epnwcf.com/Article/details/geybyokaa.sHtML

files=$(ls -1)
来源：http://www.blog.fktsv.cn/Article/details/gypphvkda.sHtML

[R38] 管道串联
来源：http://www.share.fktsv.cn/Article/details/gnszlsdzn.sHtML

cat a.txt | grep -i error | wc -l
来源：http://baike.yfazqb.com/Article/details/geqmkbgsg.sHtML

[R39] 重定向标准输出与错误
来源：http://read.share.sjlbkw.cn/Article/details/gpztrkmkm.sHtML

cmd > out.log 2>&1
来源：http://www.m.share.yfazqb.com/Article/details/gulhidond.sHtML

[R40] 追加写日志
来源：http://www.share.fktsv.cn/Article/details/ghtyjbrpt.sHtML

echo "log" >> out.log
来源：http://baike.sjlbkw.cn/Article/details/gdgoinvxk.sHtML

[R41] 丢弃输出
来源：http://baike.sjlbkw.cn/Article/details/gzicebugr.sHtML

cmd >/dev/null 2>&1
来源：http://3g.tarul.cn/Article/details/gbslcgwkl.sHtML

[R42] 输入重定向
来源：http://www.m.share.fktsv.cn/Article/details/gzzplqtjq.sHtML

wc -l < a.txt
来源：http://wap.fktsv.cn/Article/details/grewszadm.sHtML

[R43] 按名字查找文件
来源：http://baike.tarul.cn/Article/details/gidzjyebm.sHtML

find . -name "*.log" -type f
来源：http://www.share.sjlbkw.cn/Article/details/guqcbfbci.sHtML

[R44] 按修改时间查找
来源：http://mobile.epnwcf.com/Article/details/gtzonstcy.sHtML

find . -mtime -7 -type f
来源：http://www.m.share.yfazqb.com/Article/details/ghuarzdnw.sHtML

[R45] 批量删除
来源：http://blog.tarul.cn/Article/details/gfciucyhg.sHtML

find . -name "*.tmp" -delete
来源：http://baike.yfazqb.com/Article/details/gnzzpvkfr.sHtML

[R46] 递归替换文件内容
来源：http://www.blog.epnwcf.com/Article/details/ggflvcjwy.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://baike.sjlbkw.cn/Article/details/gzilrvatr.sHtML

[R47] sed 单行替换
来源：http://baike.bbcook.cn/Article/details/gvhqhlbup.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://m.share.tarul.cn/Article/details/gmqsbpsck.sHtML

[R48] awk 取指定列
来源：http://wap.epnwcf.com/Article/details/gaqlserpl.sHtML

awk '{print $1, $3}' a.txt
来源：http://mobile.yfazqb.com/Article/details/gpilkhozc.sHtML

[R49] awk 带条件
来源：http://mobile.fktsv.cn/Article/details/giiwddbqh.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.blog.sjlbkw.cn/Article/details/gjdebexzb.sHtML

[R50] awk 求和
来源：http://www.blog.tarul.cn/Article/details/gzjwogdea.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://read.share.bbcook.cn/Article/details/gibgsyouo.sHtML

[R51] 排序去重取前几
来源：http://www.share.sjlbkw.cn/Article/details/gkzlzqlyr.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.m.share.vehdjk.com/Article/details/gfptkdaxd.sHtML

[R52] 统计行数
来源：http://www.m.share.tarul.cn/Article/details/gpjjujvem.sHtML

wc -l a.txt
来源：http://m.share.yfazqb.com/Article/details/ggpjqhzhb.sHtML

[R53] 查看文件头与实时尾
来源：http://read.share.bbcook.cn/Article/details/geoozqtfb.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://mobile.vehdjk.com/Article/details/gklwgcioh.sHtML

[R54] 比较两个文件
来源：http://baike.bbcook.cn/Article/details/gownmhsmz.sHtML

diff a.txt b.txt
来源：http://read.share.sjlbkw.cn/Article/details/gupyfozvn.sHtML

[R55] 压缩与解压
来源：http://mobile.epnwcf.com/Article/details/gnhwhkgyv.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://wap.tarul.cn/Article/details/gfkudadfm.sHtML

[R56] 远程拷贝
来源：http://blog.tarul.cn/Article/details/gybcshuzv.sHtML

scp file user@host:/path/
来源：http://www.m.share.epnwcf.com/Article/details/gwyklmabg.sHtML

[R57] 远程执行命令
来源：http://read.share.tarul.cn/Article/details/gwqvwpbea.sHtML

ssh user@host 'uptime'
来源：http://3g.yfazqb.com/Article/details/gtocmgxxp.sHtML

[R58] 下载文件
来源：http://www.blog.sjlbkw.cn/Article/details/gnojokryb.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://baike.yfazqb.com/Article/details/gixyixreg.sHtML

[R59] 发 POST JSON
来源：http://blog.fktsv.cn/Article/details/gkdobutgy.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wap.epnwcf.com/Article/details/gxzasjrwv.sHtML

[R60] 只看 HTTP 状态码
来源：http://m.share.yfazqb.com/Article/details/gtdndrmvw.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://m.share.tarul.cn/Article/details/gindrnzql.sHtML

[R61] 磁盘占用
来源：http://3g.vehdjk.com/Article/details/gocrjjfjr.sHtML

df -h;  du -sh *
来源：http://read.share.sjlbkw.cn/Article/details/gtdqemxfk.sHtML

[R62] 找最占空间的文件
来源：http://m.share.fktsv.cn/Article/details/gikaqukzr.sHtML

du -ah . | sort -rh | head -10
来源：http://m.share.yfazqb.com/Article/details/gulclrwio.sHtML

[R63] 内存与进程
来源：http://baike.fktsv.cn/Article/details/gcpbkwnma.sHtML

free -h;  ps aux | grep nginx
来源：http://mobile.yfazqb.com/Article/details/gfltxzdpj.sHtML

[R64] 结束进程
来源：http://www.blog.sjlbkw.cn/Article/details/gibjppmlc.sHtML

kill -9 $(pgrep -f app.py)
来源：http://mobile.bbcook.cn/Article/details/gnjbdycgi.sHtML

[R65] 查看端口占用
来源：http://blog.vehdjk.com/Article/details/ghphvhnrk.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.share.sjlbkw.cn/Article/details/gfzhxhfgj.sHtML

[R66] 定时任务
来源：http://mobile.bbcook.cn/Article/details/glkockqef.sHtML

crontab -e;  crontab -l
来源：http://www.share.tarul.cn/Article/details/gpbvkpvmn.sHtML

[R67] 生成随机十六进制串
来源：http://baike.tarul.cn/Article/details/gxoafxmhc.sHtML

openssl rand -hex 16
来源：http://www.share.epnwcf.com/Article/details/gepuxjpkj.sHtML

[R68] 计算文件校验值
来源：http://www.m.share.sjlbkw.cn/Article/details/gdeztydeu.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://blog.sjlbkw.cn/Article/details/gwrljeqnf.sHtML

[R69] 生成随机密码
来源：http://blog.sjlbkw.cn/Article/details/gcwqnonpq.sHtML

head -c 16 /dev/urandom | base64
来源：http://m.share.yfazqb.com/Article/details/gbylieboh.sHtML

[R70] 时间戳与互转
来源：http://3g.sjlbkw.cn/Article/details/glxkvvixm.sHtML

date +%s;  date -d @1700000000
来源：http://www.blog.sjlbkw.cn/Article/details/gaolsqvmu.sHtML

[R71] 日期格式化
来源：http://m.share.epnwcf.com/Article/details/gzjljyijd.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://wap.tarul.cn/Article/details/ghgovxfmb.sHtML

[R72] 等待端口就绪
来源：http://read.share.tarul.cn/Article/details/gwvwsatrt.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://blog.fktsv.cn/Article/details/gxpqjchhn.sHtML

[R73] 分割大日志
来源：http://read.share.sjlbkw.cn/Article/details/gkjvayvpk.sHtML

split -l 1000 big.log part_
来源：http://m.share.vehdjk.com/Article/details/gmbldkizc.sHtML

[R74] 批量重命名
来源：http://www.share.sjlbkw.cn/Article/details/gxqxqqshq.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://3g.sjlbkw.cn/Article/details/guloyrtns.sHtML

[R75] 导出环境变量
来源：http://www.m.share.epnwcf.com/Article/details/gidnhslge.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://wap.sjlbkw.cn/Article/details/gkyujcegd.sHtML

[R76] 使用临时文件
来源：http://3g.epnwcf.com/Article/details/gowfrhgjw.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.tarul.cn/Article/details/gvsbmrzuv.sHtML

[R77] 读取用户输入
来源：http://baike.sjlbkw.cn/Article/details/glsgeesbp.sHtML

read -rp "请输入: " ans
来源：http://blog.sjlbkw.cn/Article/details/gtlukgkdg.sHtML

[R78] 交互式菜单
来源：http://blog.bbcook.cn/Article/details/gjhzkrlfi.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.m.share.sjlbkw.cn/Article/details/gbzvvcalu.sHtML

[R79] 解析命令行选项
来源：http://www.blog.vehdjk.com/Article/details/ghwrjsxur.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mobile.epnwcf.com/Article/details/glwhroojz.sHtML

[R80] 查看脚本执行耗时
来源：http://wap.bbcook.cn/Article/details/ggagdcote.sHtML

time ./run.sh
来源：http://wap.vehdjk.com/Article/details/gniezaajq.sHtML

================================================================================
来源：http://3g.epnwcf.com/Article/details/gpozmueoy.sHtML

S. C / C++ 专题
来源：http://wap.bbcook.cn/Article/details/ghgngcwyi.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/gjcjpmskw.sHtML

[S01] C：Hello World
来源：http://www.m.share.vehdjk.com/Article/details/gopqvardd.sHtML

#include <stdio.h>
来源：http://wap.yfazqb.com/Article/details/ggowpnqsk.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://blog.bbcook.cn/Article/details/gjlrgdfvm.sHtML

[S02] C：变量与格式化输出
来源：http://3g.fktsv.cn/Article/details/ghtcokcjn.sHtML

int a = 10; printf("%d\n", a);
来源：http://m.share.sjlbkw.cn/Article/details/gxatpgbik.sHtML

[S03] C：读入整数
来源：http://m.share.yfazqb.com/Article/details/genfomfip.sHtML

int x; scanf("%d", &x);
来源：http://wap.sjlbkw.cn/Article/details/gvyxcsvjw.sHtML

[S04] C：字符串复制
来源：http://read.share.yfazqb.com/Article/details/gzexoyouh.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://m.share.sjlbkw.cn/Article/details/gxscziphb.sHtML

[S05] C：字符串长度
来源：http://wap.vehdjk.com/Article/details/grsexrtpa.sHtML

strlen(s)
来源：http://baike.epnwcf.com/Article/details/ghbztlwrz.sHtML

[S06] C：字符串比较
来源：http://3g.fktsv.cn/Article/details/gsyndxwyb.sHtML

strcmp(a, b) == 0
来源：http://read.share.sjlbkw.cn/Article/details/gbxawkhkp.sHtML

[S07] C：数组遍历求和
来源：http://wap.epnwcf.com/Article/details/ghqgzjkwz.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://read.share.yfazqb.com/Article/details/goodftjhy.sHtML

[S08] C：动态内存分配与释放
来源：http://m.share.vehdjk.com/Article/details/gilmkbwcb.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://3g.bbcook.cn/Article/details/gdzfbqdfg.sHtML

[S09] C：结构体定义与初始化
来源：http://www.m.share.sjlbkw.cn/Article/details/gzkhjpbhv.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://baike.yfazqb.com/Article/details/gyonsoknk.sHtML

[S10] C：指针与解引用
来源：http://mobile.yfazqb.com/Article/details/gwtjdqlue.sHtML

int *p = &a;  *p = 5;
来源：http://www.share.epnwcf.com/Article/details/giqzmkqir.sHtML

[S11] C：逐行读文件
来源：http://read.share.vehdjk.com/Article/details/gzcbmeshw.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://m.share.tarul.cn/Article/details/gojppgeqs.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.m.share.bbcook.cn/Article/details/gxmnumuvi.sHtML

fclose(f);
来源：http://m.share.tarul.cn/Article/details/gifujexwv.sHtML

[S12] C：写文件
来源：http://www.blog.fktsv.cn/Article/details/gdeejcesv.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://wap.bbcook.cn/Article/details/gutsqehgf.sHtML

[S13] C：宏定义
来源：http://wap.tarul.cn/Article/details/gyweiaoox.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.share.yfazqb.com/Article/details/gyxpbpsym.sHtML

[S14] C：枚举
来源：http://3g.bbcook.cn/Article/details/gtcmnyinh.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://mobile.vehdjk.com/Article/details/gmlcjkfoc.sHtML

[S15] C：类型转换
来源：http://www.share.yfazqb.com/Article/details/ghnqiqxhe.sHtML

(double) a / b
来源：http://m.share.sjlbkw.cn/Article/details/grmmnpcpq.sHtML

[S16] C：位操作置位
来源：http://3g.epnwcf.com/Article/details/gsykxqdgm.sHtML

x |= (1 << 3);
来源：http://3g.sjlbkw.cn/Article/details/ghtxrmrig.sHtML

[S17] C：安全拼接字符串
来源：http://www.blog.fktsv.cn/Article/details/gnijrpzid.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://3g.bbcook.cn/Article/details/glfumokcz.sHtML

[S18] C：命令行参数
来源：http://read.share.yfazqb.com/Article/details/gpxkvulha.sHtML

int main(int argc, char **argv)
来源：http://3g.sjlbkw.cn/Article/details/gzpfrkznt.sHtML

[S19] C：快速排序
来源：http://www.share.epnwcf.com/Article/details/gconqijpl.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.share.vehdjk.com/Article/details/grbhqacfj.sHtML

[S20] C：二分查找
来源：http://baike.fktsv.cn/Article/details/gumgaphio.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://3g.vehdjk.com/Article/details/glltrggnm.sHtML

[S21] C：字符类别判断
来源：http://www.share.epnwcf.com/Article/details/gjhtmsuvo.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://3g.epnwcf.com/Article/details/gupylemxq.sHtML

[S22] C：字符串转数字
来源：http://www.blog.fktsv.cn/Article/details/gieptwhhv.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.share.tarul.cn/Article/details/gxpmhaqqa.sHtML

[S23] C：随机数
来源：http://www.share.vehdjk.com/Article/details/gcfgxtgbl.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://baike.tarul.cn/Article/details/gfjtnaukv.sHtML

[S24] C：获取本地时间
来源：http://blog.tarul.cn/Article/details/gstankarm.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://mobile.epnwcf.com/Article/details/ghldutnev.sHtML

[S25] C：内存拷贝
来源：http://www.m.share.sjlbkw.cn/Article/details/ggoebyffa.sHtML

memcpy(dst, src, n);
来源：http://www.share.yfazqb.com/Article/details/gswdlwdwm.sHtML

[S26] C：内存清零
来源：http://read.share.yfazqb.com/Article/details/gpzukfzwn.sHtML

memset(a, 0, sizeof a);
来源：http://www.share.epnwcf.com/Article/details/goiuhrdom.sHtML

[S27] C：定义常量
来源：http://m.share.vehdjk.com/Article/details/gwovexwrm.sHtML

const double PI = 3.14159;
来源：http://m.share.yfazqb.com/Article/details/grobcqzmy.sHtML

[S28] C：静态变量
来源：http://m.share.tarul.cn/Article/details/gorilxedo.sHtML

static int counter = 0;
来源：http://baike.bbcook.cn/Article/details/gphudnrzf.sHtML

[S29] C：变参函数
来源：http://3g.bbcook.cn/Article/details/ghqknmdqq.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://baike.vehdjk.com/Article/details/gnqqrsfja.sHtML

[S30] C：头文件保护
来源：http://m.share.epnwcf.com/Article/details/gasmktzhg.sHtML

#ifndef X_H
来源：http://read.share.epnwcf.com/Article/details/giijhzefp.sHtML

#define X_H
来源：http://mobile.yfazqb.com/Article/details/gxlsqmdqh.sHtML

#endif
来源：http://www.blog.tarul.cn/Article/details/gcmnrrdhk.sHtML

[S31] C++：Hello World
来源：http://read.share.sjlbkw.cn/Article/details/gkxnwshcx.sHtML

#include <iostream>
来源：http://3g.sjlbkw.cn/Article/details/glgloxeyj.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://mobile.epnwcf.com/Article/details/gztiqcctx.sHtML

[S32] C++：字符串
来源：http://read.share.epnwcf.com/Article/details/gnhmbbbox.sHtML

std::string s = "hi";  s += "!";
来源：http://blog.vehdjk.com/Article/details/germttuvb.sHtML

[S33] C++：vector 增删
来源：http://3g.epnwcf.com/Article/details/gjgebnskn.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://3g.tarul.cn/Article/details/gpxhvbqag.sHtML

[S34] C++：遍历 vector
来源：http://mobile.vehdjk.com/Article/details/gcrddpnpi.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.share.sjlbkw.cn/Article/details/goqrnkzoe.sHtML

[S35] C++：map
来源：http://baike.sjlbkw.cn/Article/details/gnrfqsxcd.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.sjlbkw.cn/Article/details/gyxqfydnn.sHtML

[S36] C++：unordered_map
来源：http://baike.sjlbkw.cn/Article/details/gjzurmypf.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.yfazqb.com/Article/details/gesuhesao.sHtML

[S37] C++：set
来源：http://3g.tarul.cn/Article/details/gzrmtkiqp.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://blog.bbcook.cn/Article/details/gchfabjyv.sHtML

[S38] C++：排序
来源：http://www.share.epnwcf.com/Article/details/gqmsltyar.sHtML

std::sort(v.begin(), v.end());
来源：http://m.share.yfazqb.com/Article/details/gyawiyozl.sHtML

[S39] C++：自定义比较器排序
来源：http://m.share.bbcook.cn/Article/details/gfjqvjegt.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://blog.tarul.cn/Article/details/gnptspvsz.sHtML

[S40] C++：查找元素
来源：http://www.share.vehdjk.com/Article/details/grvoulvzy.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://m.share.epnwcf.com/Article/details/gvgopctdq.sHtML

[S41] C++：类与构造函数
来源：http://www.m.share.epnwcf.com/Article/details/garvxglac.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://mobile.yfazqb.com/Article/details/gviyozlnz.sHtML

[S42] C++：继承与虚函数
来源：http://baike.fktsv.cn/Article/details/gpmuczkcx.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.blog.fktsv.cn/Article/details/gsedmnadi.sHtML

[S43] C++：智能指针
来源：http://www.blog.sjlbkw.cn/Article/details/gehgwbzvq.sHtML

auto p = std::make_unique<int>(5);
来源：http://wap.fktsv.cn/Article/details/giwdczqno.sHtML

[S44] C++：引用传参
来源：http://mobile.bbcook.cn/Article/details/gckussivn.sHtML

void inc(int &x) { ++x; }
来源：http://www.m.share.fktsv.cn/Article/details/gbmlzwypa.sHtML

[S45] C++：lambda
来源：http://3g.bbcook.cn/Article/details/gmxjelras.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://read.share.vehdjk.com/Article/details/gszaaiyar.sHtML

[S46] C++：函数模板
来源：http://www.share.vehdjk.com/Article/details/gycoyovla.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://blog.tarul.cn/Article/details/gcsuehldr.sHtML

[S47] C++：结构化绑定遍历
来源：http://mobile.epnwcf.com/Article/details/gfsttowwb.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.share.sjlbkw.cn/Article/details/grjnkxqzq.sHtML

[S48] C++：逐行读文件
来源：http://read.share.vehdjk.com/Article/details/gypxzlpcz.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.share.bbcook.cn/Article/details/ghhlwljet.sHtML

while (std::getline(in, line)) { }
来源：http://blog.epnwcf.com/Article/details/grkfgujnk.sHtML

[S49] C++：写文件
来源：http://read.share.vehdjk.com/Article/details/ggkpfvumg.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.m.share.bbcook.cn/Article/details/gxxwguseg.sHtML

[S50] C++：格式化数字
来源：http://blog.vehdjk.com/Article/details/gwlakwgcq.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://baike.sjlbkw.cn/Article/details/gzavkhrcs.sHtML

[S51] C++：显式类型转换
来源：http://www.share.yfazqb.com/Article/details/gbdyarkne.sHtML

static_cast<double>(a) / b
来源：http://www.share.tarul.cn/Article/details/gypwkdfut.sHtML

[S52] C++：const 与 noexcept
来源：http://www.m.share.sjlbkw.cn/Article/details/gkbkicona.sHtML

int size() const noexcept { return n_; }
来源：http://mobile.epnwcf.com/Article/details/gxaxodxur.sHtML

[S53] C++：移动语义
来源：http://mobile.sjlbkw.cn/Article/details/gdfqkkjlm.sHtML

std::vector<int> w = std::move(v);
来源：http://baike.yfazqb.com/Article/details/gopyoxkfm.sHtML

[S54] C++：异常处理
来源：http://read.share.fktsv.cn/Article/details/gkhqmkhnu.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://3g.bbcook.cn/Article/details/ggxaxttrm.sHtML

[S55] C++：结构化绑定
来源：http://baike.vehdjk.com/Article/details/gmzuhoedo.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://blog.tarul.cn/Article/details/gxzrpxplo.sHtML

[S56] C++：optional
来源：http://m.share.vehdjk.com/Article/details/gbbzrzxxc.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://read.share.vehdjk.com/Article/details/gjsqyogvt.sHtML

[S57] C++：编译期常量
来源：http://www.share.yfazqb.com/Article/details/grppvzkbw.sHtML

constexpr int N = 10;
来源：http://blog.fktsv.cn/Article/details/gcagbzdzj.sHtML

[S58] C++：命名空间
来源：http://read.share.epnwcf.com/Article/details/gagisjrkc.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.share.vehdjk.com/Article/details/gipjujzxh.sHtML

[S59] C++：静态断言
来源：http://blog.tarul.cn/Article/details/gtljxxako.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://blog.epnwcf.com/Article/details/gesqbhhao.sHtML

[S60] C++：遍历并删除元素
来源：http://wap.vehdjk.com/Article/details/gkmklbpol.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.m.share.fktsv.cn/Article/details/ghpaiyieo.sHtML

================================================================================
来源：http://baike.vehdjk.com/Article/details/gdwnxaeyr.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.fktsv.cn/Article/details/gzjjbjnkl.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/gozqsgkwq.sHtML

[T01] Kotlin：Hello World
来源：http://www.m.share.tarul.cn/Article/details/gojthunkv.sHtML

println("Hello")
来源：http://www.blog.yfazqb.com/Article/details/gcfclacqp.sHtML

[T02] Kotlin：变量
来源：http://m.share.yfazqb.com/Article/details/gxgunakdg.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://m.share.epnwcf.com/Article/details/gezcwcgnu.sHtML

[T03] Kotlin：字符串模板
来源：http://wap.tarul.cn/Article/details/giasmcevt.sHtML

"值: $b"
来源：http://www.share.bbcook.cn/Article/details/gybdkgzre.sHtML

[T04] Kotlin：空安全
来源：http://m.share.vehdjk.com/Article/details/gauuwgzpl.sHtML

val n: String? = null;  n?.length
来源：http://blog.sjlbkw.cn/Article/details/gudjcaafe.sHtML

[T05] Kotlin：when 表达式
来源：http://read.share.tarul.cn/Article/details/gxcpmzpja.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://mobile.fktsv.cn/Article/details/gszsesqcu.sHtML

[T06] Kotlin：集合映射
来源：http://blog.sjlbkw.cn/Article/details/gkflqfphc.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://blog.vehdjk.com/Article/details/guhtohrwy.sHtML

[T07] Kotlin：集合过滤
来源：http://www.share.yfazqb.com/Article/details/gxungloex.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.m.share.tarul.cn/Article/details/gdilrmwxx.sHtML

[T08] Kotlin：数据类
来源：http://www.share.sjlbkw.cn/Article/details/geiwuzemx.sHtML

data class User(val name: String, val age: Int)
来源：http://blog.tarul.cn/Article/details/gvwdoooby.sHtML

[T09] Kotlin：扩展函数
来源：http://www.m.share.yfazqb.com/Article/details/gpoomekqk.sHtML

fun String.exclaim() = this + "!"
来源：http://www.m.share.bbcook.cn/Article/details/gaocfxjqd.sHtML

[T10] Kotlin：默认参数
来源：http://www.blog.bbcook.cn/Article/details/gjhmqqdzu.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.blog.fktsv.cn/Article/details/gujwwjuoy.sHtML

[T11] Kotlin：协程
来源：http://wap.sjlbkw.cn/Article/details/gvtmfbwdq.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://baike.yfazqb.com/Article/details/gxupboxnf.sHtML

[T12] Kotlin：解构声明
来源：http://3g.vehdjk.com/Article/details/gpdfcnmyv.sHtML

val (a, b) = Pair(1, 2)
来源：http://3g.bbcook.cn/Article/details/gmblprdrb.sHtML

[T13] Kotlin：只读 Map
来源：http://www.share.epnwcf.com/Article/details/gpbsxpdan.sHtML

val m = mapOf("a" to 1)
来源：http://read.share.vehdjk.com/Article/details/gehgzqxhs.sHtML

[T14] Kotlin：循环
来源：http://read.share.sjlbkw.cn/Article/details/gxsjpshul.sHtML

for (i in 1..10) println(i)
来源：http://www.share.vehdjk.com/Article/details/gphpswsyi.sHtML

[T15] Kotlin：接口
来源：http://read.share.tarul.cn/Article/details/gckoxwmvb.sHtML

interface Shape { fun area(): Double }
来源：http://mobile.sjlbkw.cn/Article/details/gaiacqnfd.sHtML

[T16] Swift：Hello World
来源：http://www.m.share.yfazqb.com/Article/details/grfabxnck.sHtML

print("Hello")
来源：http://m.share.epnwcf.com/Article/details/gpekhysyw.sHtML

[T17] Swift：变量与常量
来源：http://www.blog.sjlbkw.cn/Article/details/ghoqjvdxg.sHtML

var a = 1;  let b = 2
来源：http://baike.tarul.cn/Article/details/gysmhhyhb.sHtML

[T18] Swift：字符串插值
来源：http://www.blog.epnwcf.com/Article/details/gmtvzqnks.sHtML

"值: \(b)"
来源：http://www.share.yfazqb.com/Article/details/gbfdmllhb.sHtML

[T19] Swift：可选绑定
来源：http://wap.sjlbkw.cn/Article/details/gzkqkywdq.sHtML

if let n = opt { print(n) }
来源：http://www.share.bbcook.cn/Article/details/geslfgjvo.sHtML

[T20] Swift：数组操作
来源：http://blog.fktsv.cn/Article/details/ggcrykswq.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://blog.fktsv.cn/Article/details/gzhptzvoi.sHtML

[T21] Swift：遍历
来源：http://3g.tarul.cn/Article/details/gbcftnmai.sHtML

for x in a { print(x) }
来源：http://www.m.share.tarul.cn/Article/details/giimjhpld.sHtML

[T22] Swift：字典
来源：http://mobile.fktsv.cn/Article/details/gliryxnpv.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://m.share.vehdjk.com/Article/details/gqsdcwepk.sHtML

[T23] Swift：函数
来源：http://read.share.epnwcf.com/Article/details/gkrczocvv.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.blog.vehdjk.com/Article/details/gyuqlyrln.sHtML

[T24] Swift：闭包
来源：http://wap.tarul.cn/Article/details/gxuyqtgpn.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://blog.sjlbkw.cn/Article/details/gflrqghsh.sHtML

[T25] Swift：结构体
来源：http://www.share.fktsv.cn/Article/details/ghlzisyem.sHtML

struct P { var x: Int }
来源：http://www.blog.epnwcf.com/Article/details/gpqkluvry.sHtML

[T26] Swift：类与重写
来源：http://m.share.epnwcf.com/Article/details/gshzxqphp.sHtML

class A: Base { override func f() {} }
来源：http://blog.bbcook.cn/Article/details/gedtpoxqp.sHtML

[T27] Swift：错误处理
来源：http://www.m.share.sjlbkw.cn/Article/details/gyfggqsnb.sHtML

do { try f() } catch { print(error) }
来源：http://blog.epnwcf.com/Article/details/gqrkibmjv.sHtML

[T28] Swift：枚举
来源：http://read.share.vehdjk.com/Article/details/gmqmbqqgd.sHtML

enum Color { case red, green }
来源：http://www.m.share.sjlbkw.cn/Article/details/gttummdzj.sHtML

[T29] Swift：guard 提前返回
来源：http://m.share.bbcook.cn/Article/details/gmdifnfwj.sHtML

guard let x = opt else { return }
来源：http://baike.epnwcf.com/Article/details/gztiimofe.sHtML

[T30] Swift：协议
来源：http://read.share.epnwcf.com/Article/details/gyobufbcm.sHtML

protocol Shape { func area() -> Double }
来源：http://blog.epnwcf.com/Article/details/gnoksqphj.sHtML

[T31] Lua：Hello World
来源：http://3g.tarul.cn/Article/details/gvnlualra.sHtML

print("Hello")
来源：http://m.share.yfazqb.com/Article/details/guirtiiap.sHtML

[T32] Lua：局部变量
来源：http://m.share.yfazqb.com/Article/details/gsmacdvbs.sHtML

local a = 1
来源：http://3g.bbcook.cn/Article/details/grwyqvqvu.sHtML

[T33] Lua：表（数组）
来源：http://blog.sjlbkw.cn/Article/details/guyveoetf.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://3g.tarul.cn/Article/details/gzwrcchth.sHtML

[T34] Lua：遍历表
来源：http://blog.bbcook.cn/Article/details/ggzdzworg.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://blog.yfazqb.com/Article/details/gkztatiaj.sHtML


<!-- 参考信息 -->