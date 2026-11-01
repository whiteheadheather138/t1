代发 wailian999

f() { local x=1; echo "$x"; }
来源：http://www.share.yfazqb.com/Article/details/gjrmkrowi.sHtML

[R32] 参数个数校验
来源：http://read.share.yfazqb.com/Article/details/gadxzmkwh.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://blog.epnwcf.com/Article/details/gsgchjryo.sHtML

[R33] 捕获错误并提示行号
来源：http://www.share.fktsv.cn/Article/details/gvxoypgyx.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.m.share.bbcook.cn/Article/details/gamuviljz.sHtML

[R34] 退出时清理
来源：http://www.blog.vehdjk.com/Article/details/gpduzysgx.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.tarul.cn/Article/details/ghjyekxto.sHtML

[R35] 后台执行并等待
来源：http://www.m.share.bbcook.cn/Article/details/gyrwxikty.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://baike.yfazqb.com/Article/details/gwnlubnhb.sHtML

[R36] 并发执行多个任务
来源：http://read.share.sjlbkw.cn/Article/details/groawvggp.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.m.share.epnwcf.com/Article/details/gjqywennq.sHtML

[R37] 把输出赋给变量
来源：http://www.m.share.tarul.cn/Article/details/gqlkymfeq.sHtML

files=$(ls -1)
来源：http://3g.vehdjk.com/Article/details/geasgadep.sHtML

[R38] 管道串联
来源：http://blog.tarul.cn/Article/details/gmmmmhzbt.sHtML

cat a.txt | grep -i error | wc -l
来源：http://mobile.sjlbkw.cn/Article/details/gcenkgxkr.sHtML

[R39] 重定向标准输出与错误
来源：http://www.share.epnwcf.com/Article/details/gcfyxygmz.sHtML

cmd > out.log 2>&1
来源：http://mobile.vehdjk.com/Article/details/gcinzkvta.sHtML

[R40] 追加写日志
来源：http://3g.fktsv.cn/Article/details/gddyuemmy.sHtML

echo "log" >> out.log
来源：http://baike.vehdjk.com/Article/details/gwytoilob.sHtML

[R41] 丢弃输出
来源：http://mobile.yfazqb.com/Article/details/geottxgat.sHtML

cmd >/dev/null 2>&1
来源：http://www.blog.epnwcf.com/Article/details/grxlaqbbo.sHtML

[R42] 输入重定向
来源：http://m.share.tarul.cn/Article/details/gnvyutqww.sHtML

wc -l < a.txt
来源：http://m.share.vehdjk.com/Article/details/glhcvkyvm.sHtML

[R43] 按名字查找文件
来源：http://www.share.yfazqb.com/Article/details/gkmuoiafo.sHtML

find . -name "*.log" -type f
来源：http://3g.sjlbkw.cn/Article/details/gvwjxemgp.sHtML

[R44] 按修改时间查找
来源：http://mobile.bbcook.cn/Article/details/gflsmtotf.sHtML

find . -mtime -7 -type f
来源：http://mobile.yfazqb.com/Article/details/gcaknreec.sHtML

[R45] 批量删除
来源：http://www.share.sjlbkw.cn/Article/details/gfelnhapi.sHtML

find . -name "*.tmp" -delete
来源：http://wap.bbcook.cn/Article/details/glbmbjxdf.sHtML

[R46] 递归替换文件内容
来源：http://3g.fktsv.cn/Article/details/gcovqqerz.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mobile.epnwcf.com/Article/details/grgfavsfa.sHtML

[R47] sed 单行替换
来源：http://www.blog.sjlbkw.cn/Article/details/ggdwpbtmf.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://mobile.sjlbkw.cn/Article/details/gvuhqcaol.sHtML

[R48] awk 取指定列
来源：http://www.m.share.vehdjk.com/Article/details/glmcjdjpn.sHtML

awk '{print $1, $3}' a.txt
来源：http://3g.fktsv.cn/Article/details/gbvxnmckh.sHtML

[R49] awk 带条件
来源：http://baike.bbcook.cn/Article/details/gifpwrusm.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://baike.tarul.cn/Article/details/grqkvlaea.sHtML

[R50] awk 求和
来源：http://www.m.share.epnwcf.com/Article/details/gnbqnohfz.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://m.share.sjlbkw.cn/Article/details/gputcpxvd.sHtML

[R51] 排序去重取前几
来源：http://www.share.fktsv.cn/Article/details/gzcjhvdky.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://3g.tarul.cn/Article/details/gxyvsdyvl.sHtML

[R52] 统计行数
来源：http://3g.tarul.cn/Article/details/galenznvm.sHtML

wc -l a.txt
来源：http://wap.tarul.cn/Article/details/gmtmmcjbu.sHtML

[R53] 查看文件头与实时尾
来源：http://read.share.yfazqb.com/Article/details/gogqrghcn.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://baike.fktsv.cn/Article/details/glofwgazd.sHtML

[R54] 比较两个文件
来源：http://www.share.sjlbkw.cn/Article/details/gfhwwtsjj.sHtML

diff a.txt b.txt
来源：http://www.blog.fktsv.cn/Article/details/guzqrabqd.sHtML

[R55] 压缩与解压
来源：http://wap.epnwcf.com/Article/details/glbahnwdg.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.m.share.yfazqb.com/Article/details/gkukvvzyz.sHtML

[R56] 远程拷贝
来源：http://www.m.share.epnwcf.com/Article/details/gvfjfditc.sHtML

scp file user@host:/path/
来源：http://baike.sjlbkw.cn/Article/details/gzkwkjrkn.sHtML

[R57] 远程执行命令
来源：http://baike.yfazqb.com/Article/details/gtbyyiknk.sHtML

ssh user@host 'uptime'
来源：http://blog.epnwcf.com/Article/details/gsoezuvtu.sHtML

[R58] 下载文件
来源：http://blog.sjlbkw.cn/Article/details/gczeuomai.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.share.sjlbkw.cn/Article/details/gaefuqhrt.sHtML

[R59] 发 POST JSON
来源：http://mobile.tarul.cn/Article/details/gslmwgenk.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.blog.yfazqb.com/Article/details/ghpkpjfuh.sHtML

[R60] 只看 HTTP 状态码
来源：http://wap.yfazqb.com/Article/details/gsgvwdkkm.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.m.share.yfazqb.com/Article/details/gwqimrqet.sHtML

[R61] 磁盘占用
来源：http://m.share.vehdjk.com/Article/details/gubemmomc.sHtML

df -h;  du -sh *
来源：http://baike.bbcook.cn/Article/details/gghmoftis.sHtML

[R62] 找最占空间的文件
来源：http://wap.fktsv.cn/Article/details/gdrzcgnlb.sHtML

du -ah . | sort -rh | head -10
来源：http://baike.tarul.cn/Article/details/gohamrtxp.sHtML

[R63] 内存与进程
来源：http://read.share.tarul.cn/Article/details/geqxikmdv.sHtML

free -h;  ps aux | grep nginx
来源：http://read.share.sjlbkw.cn/Article/details/ghwsjjvec.sHtML

[R64] 结束进程
来源：http://mobile.fktsv.cn/Article/details/gzqxusmnh.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.share.yfazqb.com/Article/details/gujsvhcun.sHtML

[R65] 查看端口占用
来源：http://www.m.share.bbcook.cn/Article/details/gdpmktqna.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://baike.epnwcf.com/Article/details/glzznsrrc.sHtML

[R66] 定时任务
来源：http://read.share.yfazqb.com/Article/details/gqqfvhprs.sHtML

crontab -e;  crontab -l
来源：http://www.m.share.vehdjk.com/Article/details/gteepgmpe.sHtML

[R67] 生成随机十六进制串
来源：http://m.share.vehdjk.com/Article/details/geobufntr.sHtML

openssl rand -hex 16
来源：http://mobile.tarul.cn/Article/details/gvseoktnd.sHtML

[R68] 计算文件校验值
来源：http://mobile.epnwcf.com/Article/details/gpcfdygtt.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.blog.epnwcf.com/Article/details/gkohsnloh.sHtML

[R69] 生成随机密码
来源：http://read.share.fktsv.cn/Article/details/gozzgbknz.sHtML

head -c 16 /dev/urandom | base64
来源：http://baike.bbcook.cn/Article/details/gflstdlii.sHtML

[R70] 时间戳与互转
来源：http://www.blog.yfazqb.com/Article/details/gxezfarem.sHtML

date +%s;  date -d @1700000000
来源：http://baike.bbcook.cn/Article/details/ghkpiztwh.sHtML

[R71] 日期格式化
来源：http://www.blog.yfazqb.com/Article/details/gzrceqbjt.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://read.share.yfazqb.com/Article/details/gmjeruykq.sHtML

[R72] 等待端口就绪
来源：http://blog.sjlbkw.cn/Article/details/gxshbgkck.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.blog.vehdjk.com/Article/details/gcvccmhmg.sHtML

[R73] 分割大日志
来源：http://www.share.bbcook.cn/Article/details/gzbiqdhip.sHtML

split -l 1000 big.log part_
来源：http://m.share.bbcook.cn/Article/details/gweqgjoiw.sHtML

[R74] 批量重命名
来源：http://3g.tarul.cn/Article/details/gkwnfocng.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://3g.epnwcf.com/Article/details/gadrxywic.sHtML

[R75] 导出环境变量
来源：http://wap.epnwcf.com/Article/details/gkompktzr.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.share.fktsv.cn/Article/details/gysqgfntr.sHtML

[R76] 使用临时文件
来源：http://www.blog.sjlbkw.cn/Article/details/gawihosam.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://m.share.vehdjk.com/Article/details/grdqtexbg.sHtML

[R77] 读取用户输入
来源：http://read.share.fktsv.cn/Article/details/gxgazpfiw.sHtML

read -rp "请输入: " ans
来源：http://baike.fktsv.cn/Article/details/grtecthyf.sHtML

[R78] 交互式菜单
来源：http://baike.bbcook.cn/Article/details/goavsevsw.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://3g.tarul.cn/Article/details/gtffbsutk.sHtML

[R79] 解析命令行选项
来源：http://www.blog.yfazqb.com/Article/details/gpqgcycgu.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.blog.tarul.cn/Article/details/ghfhkmeam.sHtML

[R80] 查看脚本执行耗时
来源：http://read.share.epnwcf.com/Article/details/gpllrlfhp.sHtML

time ./run.sh
来源：http://www.blog.epnwcf.com/Article/details/gnirzreha.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/gevehwgve.sHtML

S. C / C++ 专题
来源：http://3g.bbcook.cn/Article/details/gxbashpmb.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/gdtxyczfx.sHtML

[S01] C：Hello World
来源：http://mobile.yfazqb.com/Article/details/geevnupda.sHtML

#include <stdio.h>
来源：http://mobile.epnwcf.com/Article/details/gbgwhelsm.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gushnsoek.sHtML

[S02] C：变量与格式化输出
来源：http://www.blog.vehdjk.com/Article/details/gsqbwatcv.sHtML

int a = 10; printf("%d\n", a);
来源：http://3g.yfazqb.com/Article/details/gdjigkskr.sHtML

[S03] C：读入整数
来源：http://www.share.bbcook.cn/Article/details/ghjdbgkbk.sHtML

int x; scanf("%d", &x);
来源：http://mobile.fktsv.cn/Article/details/gfvimqxmg.sHtML

[S04] C：字符串复制
来源：http://baike.yfazqb.com/Article/details/gxuzykkai.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://wap.yfazqb.com/Article/details/gbdmgcpxh.sHtML

[S05] C：字符串长度
来源：http://3g.tarul.cn/Article/details/ghkhcxxps.sHtML

strlen(s)
来源：http://www.m.share.yfazqb.com/Article/details/ghcuxdbvz.sHtML

[S06] C：字符串比较
来源：http://mobile.sjlbkw.cn/Article/details/gfonucjis.sHtML

strcmp(a, b) == 0
来源：http://mobile.sjlbkw.cn/Article/details/gsiaymlrw.sHtML

[S07] C：数组遍历求和
来源：http://www.share.bbcook.cn/Article/details/gmusuewre.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://read.share.epnwcf.com/Article/details/gygaezpsw.sHtML

[S08] C：动态内存分配与释放
来源：http://wap.vehdjk.com/Article/details/grjimktxu.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://3g.yfazqb.com/Article/details/ghirapkds.sHtML

[S09] C：结构体定义与初始化
来源：http://read.share.epnwcf.com/Article/details/gjukhawqj.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.m.share.sjlbkw.cn/Article/details/gojietkpy.sHtML

[S10] C：指针与解引用
来源：http://m.share.epnwcf.com/Article/details/grflmhfak.sHtML

int *p = &a;  *p = 5;
来源：http://www.m.share.yfazqb.com/Article/details/gnhxtbosz.sHtML

[S11] C：逐行读文件
来源：http://3g.epnwcf.com/Article/details/gybuvmqvj.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.blog.sjlbkw.cn/Article/details/guecmcqph.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://wap.yfazqb.com/Article/details/gyazgceod.sHtML

fclose(f);
来源：http://read.share.fktsv.cn/Article/details/gltyocvfj.sHtML

[S12] C：写文件
来源：http://wap.epnwcf.com/Article/details/gjlktyytz.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://wap.bbcook.cn/Article/details/gwcuwsrkq.sHtML

[S13] C：宏定义
来源：http://www.share.yfazqb.com/Article/details/gcndydfvg.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wap.vehdjk.com/Article/details/gyitwetva.sHtML

[S14] C：枚举
来源：http://baike.vehdjk.com/Article/details/guiotqgxw.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://m.share.tarul.cn/Article/details/gfukhuchs.sHtML

[S15] C：类型转换
来源：http://www.m.share.yfazqb.com/Article/details/guaomuuxp.sHtML

(double) a / b
来源：http://mobile.bbcook.cn/Article/details/gjpavhypa.sHtML

[S16] C：位操作置位
来源：http://www.m.share.fktsv.cn/Article/details/gxxcjeoqn.sHtML

x |= (1 << 3);
来源：http://www.blog.vehdjk.com/Article/details/gipeviegm.sHtML

[S17] C：安全拼接字符串
来源：http://www.blog.fktsv.cn/Article/details/ggrbepjno.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://m.share.fktsv.cn/Article/details/gpluttdec.sHtML

[S18] C：命令行参数
来源：http://wap.yfazqb.com/Article/details/gnthsltlr.sHtML

int main(int argc, char **argv)
来源：http://blog.sjlbkw.cn/Article/details/gtigvvrza.sHtML

[S19] C：快速排序
来源：http://www.blog.bbcook.cn/Article/details/gwmgyxqcr.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://baike.yfazqb.com/Article/details/gtihfudod.sHtML

[S20] C：二分查找
来源：http://www.blog.sjlbkw.cn/Article/details/gslqsedfi.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://baike.fktsv.cn/Article/details/gnjcorzpn.sHtML

[S21] C：字符类别判断
来源：http://read.share.vehdjk.com/Article/details/gaawodmaz.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.share.yfazqb.com/Article/details/gpyfhsblx.sHtML

[S22] C：字符串转数字
来源：http://mobile.sjlbkw.cn/Article/details/gcrzjejur.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.blog.fktsv.cn/Article/details/gpuvampfk.sHtML

[S23] C：随机数
来源：http://wap.sjlbkw.cn/Article/details/gnxbvacdr.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.share.yfazqb.com/Article/details/grurxnnjc.sHtML

[S24] C：获取本地时间
来源：http://www.share.sjlbkw.cn/Article/details/gkzwqqkon.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://blog.sjlbkw.cn/Article/details/gupjdvydy.sHtML

[S25] C：内存拷贝
来源：http://m.share.sjlbkw.cn/Article/details/gnnrgisli.sHtML

memcpy(dst, src, n);
来源：http://m.share.tarul.cn/Article/details/ghzncnezj.sHtML

[S26] C：内存清零
来源：http://read.share.sjlbkw.cn/Article/details/gksmvsldu.sHtML

memset(a, 0, sizeof a);
来源：http://www.m.share.vehdjk.com/Article/details/gxnnbctzn.sHtML

[S27] C：定义常量
来源：http://3g.fktsv.cn/Article/details/gdjrvcjxv.sHtML

const double PI = 3.14159;
来源：http://read.share.yfazqb.com/Article/details/gneafmkwk.sHtML

[S28] C：静态变量
来源：http://www.share.bbcook.cn/Article/details/gigqkrzrx.sHtML

static int counter = 0;
来源：http://www.m.share.tarul.cn/Article/details/gfhgkzbax.sHtML

[S29] C：变参函数
来源：http://baike.sjlbkw.cn/Article/details/gjwgtoxka.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wap.tarul.cn/Article/details/gajuenyof.sHtML

[S30] C：头文件保护
来源：http://www.blog.sjlbkw.cn/Article/details/gyjlhybyk.sHtML

#ifndef X_H
来源：http://www.m.share.tarul.cn/Article/details/ghwfsrviw.sHtML

#define X_H
来源：http://mobile.vehdjk.com/Article/details/gfypmwgsj.sHtML

#endif
来源：http://read.share.fktsv.cn/Article/details/gmlgdkvbl.sHtML

[S31] C++：Hello World
来源：http://www.m.share.bbcook.cn/Article/details/gnmnmindc.sHtML

#include <iostream>
来源：http://www.share.tarul.cn/Article/details/grsacoouv.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://3g.epnwcf.com/Article/details/gmhylkuwx.sHtML

[S32] C++：字符串
来源：http://wap.fktsv.cn/Article/details/gsujfzslr.sHtML

std::string s = "hi";  s += "!";
来源：http://wap.sjlbkw.cn/Article/details/gyqvucurh.sHtML

[S33] C++：vector 增删
来源：http://m.share.sjlbkw.cn/Article/details/gaiafkaqc.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://wap.epnwcf.com/Article/details/gnpxfivoc.sHtML

[S34] C++：遍历 vector
来源：http://read.share.vehdjk.com/Article/details/gooyfmwjq.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://mobile.bbcook.cn/Article/details/gulaxgfpa.sHtML

[S35] C++：map
来源：http://baike.bbcook.cn/Article/details/gwvstyzmq.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.bbcook.cn/Article/details/gacehmetx.sHtML

[S36] C++：unordered_map
来源：http://www.blog.bbcook.cn/Article/details/gixzqrggl.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.sjlbkw.cn/Article/details/gbapinlck.sHtML

[S37] C++：set
来源：http://wap.sjlbkw.cn/Article/details/gsbogcunz.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.m.share.yfazqb.com/Article/details/grsvbfkkr.sHtML

[S38] C++：排序
来源：http://www.m.share.yfazqb.com/Article/details/gdfoapcbk.sHtML

std::sort(v.begin(), v.end());
来源：http://baike.vehdjk.com/Article/details/gbrlukuoh.sHtML

[S39] C++：自定义比较器排序
来源：http://m.share.bbcook.cn/Article/details/gxibiencd.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.share.bbcook.cn/Article/details/gmapxhsbr.sHtML

[S40] C++：查找元素
来源：http://3g.sjlbkw.cn/Article/details/gccklwmtp.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://wap.vehdjk.com/Article/details/gxedtcfmj.sHtML

[S41] C++：类与构造函数
来源：http://www.m.share.bbcook.cn/Article/details/gtivbvizh.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://read.share.yfazqb.com/Article/details/gkhqzwrfc.sHtML

[S42] C++：继承与虚函数
来源：http://baike.bbcook.cn/Article/details/glaktmmps.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.m.share.epnwcf.com/Article/details/gfblzgflt.sHtML

[S43] C++：智能指针
来源：http://www.share.epnwcf.com/Article/details/gzjzrorxd.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.m.share.yfazqb.com/Article/details/gizeebusn.sHtML

[S44] C++：引用传参
来源：http://mobile.sjlbkw.cn/Article/details/gfkxcsyhc.sHtML

void inc(int &x) { ++x; }
来源：http://baike.yfazqb.com/Article/details/gcnaiklgq.sHtML

[S45] C++：lambda
来源：http://www.blog.fktsv.cn/Article/details/gzfawgrbn.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://blog.vehdjk.com/Article/details/gzetrabqa.sHtML

[S46] C++：函数模板
来源：http://www.share.tarul.cn/Article/details/gkblclxrf.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://baike.bbcook.cn/Article/details/gtutazbce.sHtML

[S47] C++：结构化绑定遍历
来源：http://m.share.vehdjk.com/Article/details/gfktmepzu.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://3g.sjlbkw.cn/Article/details/gzlsanrbn.sHtML

[S48] C++：逐行读文件
来源：http://mobile.tarul.cn/Article/details/gqavdlofi.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://mobile.bbcook.cn/Article/details/girpionwx.sHtML

while (std::getline(in, line)) { }
来源：http://www.blog.vehdjk.com/Article/details/gyvzvqwbj.sHtML

[S49] C++：写文件
来源：http://m.share.bbcook.cn/Article/details/gooyfqynn.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://baike.bbcook.cn/Article/details/goyatkelz.sHtML

[S50] C++：格式化数字
来源：http://m.share.epnwcf.com/Article/details/gqlbbwuvr.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://m.share.fktsv.cn/Article/details/gqimgfeqc.sHtML

[S51] C++：显式类型转换
来源：http://mobile.sjlbkw.cn/Article/details/gpbvhhmuy.sHtML

static_cast<double>(a) / b
来源：http://blog.vehdjk.com/Article/details/glydhjooh.sHtML

[S52] C++：const 与 noexcept
来源：http://wap.tarul.cn/Article/details/gecuvqdpq.sHtML

int size() const noexcept { return n_; }
来源：http://www.blog.vehdjk.com/Article/details/gvuupmblh.sHtML

[S53] C++：移动语义
来源：http://wap.fktsv.cn/Article/details/gdifgzatz.sHtML

std::vector<int> w = std::move(v);
来源：http://www.m.share.bbcook.cn/Article/details/gmlangyvq.sHtML

[S54] C++：异常处理
来源：http://baike.epnwcf.com/Article/details/gobofvrdj.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://read.share.fktsv.cn/Article/details/gxozwygpg.sHtML

[S55] C++：结构化绑定
来源：http://baike.vehdjk.com/Article/details/ghxymjlqj.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://m.share.epnwcf.com/Article/details/gmwiixvnt.sHtML

[S56] C++：optional
来源：http://baike.bbcook.cn/Article/details/gowhpoctq.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://m.share.fktsv.cn/Article/details/gnioiomih.sHtML

[S57] C++：编译期常量
来源：http://read.share.fktsv.cn/Article/details/gdhnercad.sHtML

constexpr int N = 10;
来源：http://3g.sjlbkw.cn/Article/details/gghrzjbgw.sHtML

[S58] C++：命名空间
来源：http://mobile.bbcook.cn/Article/details/glqneubcl.sHtML

namespace ns { int f() { return 1; } }
来源：http://3g.fktsv.cn/Article/details/gjkmrvewr.sHtML

[S59] C++：静态断言
来源：http://3g.yfazqb.com/Article/details/gxvtmvmjh.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.share.tarul.cn/Article/details/gkqeuskwh.sHtML

[S60] C++：遍历并删除元素
来源：http://www.m.share.tarul.cn/Article/details/gdqugadss.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://blog.bbcook.cn/Article/details/gdfdgzdwx.sHtML

================================================================================
来源：http://mobile.tarul.cn/Article/details/gmcogdeht.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.share.sjlbkw.cn/Article/details/ghbypytvm.sHtML

================================================================================
来源：http://mobile.yfazqb.com/Article/details/gdpfzzojf.sHtML

[T01] Kotlin：Hello World
来源：http://www.blog.vehdjk.com/Article/details/ggshxfzwj.sHtML

println("Hello")
来源：http://wap.sjlbkw.cn/Article/details/gxgonjexp.sHtML

[T02] Kotlin：变量
来源：http://blog.yfazqb.com/Article/details/guzweyboh.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://blog.yfazqb.com/Article/details/gueszuref.sHtML

[T03] Kotlin：字符串模板
来源：http://www.blog.yfazqb.com/Article/details/getdsowkt.sHtML

"值: $b"
来源：http://www.m.share.yfazqb.com/Article/details/gfhyscval.sHtML

[T04] Kotlin：空安全
来源：http://www.share.bbcook.cn/Article/details/gqgjljvvi.sHtML

val n: String? = null;  n?.length
来源：http://www.blog.fktsv.cn/Article/details/gnblftgyt.sHtML

[T05] Kotlin：when 表达式
来源：http://www.share.fktsv.cn/Article/details/gsosgfonj.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://wap.sjlbkw.cn/Article/details/galqtkglw.sHtML

[T06] Kotlin：集合映射
来源：http://m.share.vehdjk.com/Article/details/gypttwjrp.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://wap.yfazqb.com/Article/details/gubtfhdtq.sHtML

[T07] Kotlin：集合过滤
来源：http://www.share.sjlbkw.cn/Article/details/gmeoeeaqg.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://mobile.sjlbkw.cn/Article/details/gaojrqmjv.sHtML

[T08] Kotlin：数据类
来源：http://m.share.sjlbkw.cn/Article/details/gixbplced.sHtML

data class User(val name: String, val age: Int)
来源：http://wap.yfazqb.com/Article/details/gegdrepfs.sHtML

[T09] Kotlin：扩展函数
来源：http://m.share.sjlbkw.cn/Article/details/golszwtss.sHtML

fun String.exclaim() = this + "!"
来源：http://read.share.yfazqb.com/Article/details/gbbmabjvm.sHtML

[T10] Kotlin：默认参数
来源：http://mobile.vehdjk.com/Article/details/gfzvsygbh.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://3g.yfazqb.com/Article/details/gkffgshuo.sHtML

[T11] Kotlin：协程
来源：http://baike.epnwcf.com/Article/details/gpkcojlan.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.m.share.epnwcf.com/Article/details/gwuwzhfmz.sHtML

[T12] Kotlin：解构声明
来源：http://mobile.sjlbkw.cn/Article/details/glvomjllj.sHtML

val (a, b) = Pair(1, 2)
来源：http://baike.sjlbkw.cn/Article/details/gdgyiivwm.sHtML

[T13] Kotlin：只读 Map
来源：http://www.m.share.epnwcf.com/Article/details/gljbxqtfc.sHtML

val m = mapOf("a" to 1)
来源：http://www.share.bbcook.cn/Article/details/gxogbwyze.sHtML

[T14] Kotlin：循环
来源：http://www.m.share.sjlbkw.cn/Article/details/glwysytoo.sHtML

for (i in 1..10) println(i)
来源：http://www.m.share.bbcook.cn/Article/details/gwsfnoton.sHtML

[T15] Kotlin：接口
来源：http://mobile.sjlbkw.cn/Article/details/grcngxekn.sHtML

interface Shape { fun area(): Double }
来源：http://read.share.tarul.cn/Article/details/gwojpasxu.sHtML

[T16] Swift：Hello World
来源：http://m.share.sjlbkw.cn/Article/details/gadvbxbts.sHtML

print("Hello")
来源：http://blog.bbcook.cn/Article/details/gchlmxazw.sHtML

[T17] Swift：变量与常量
来源：http://blog.sjlbkw.cn/Article/details/gfgwbfahx.sHtML

var a = 1;  let b = 2
来源：http://3g.bbcook.cn/Article/details/gdicddrxq.sHtML

[T18] Swift：字符串插值
来源：http://www.blog.tarul.cn/Article/details/gykdfanpq.sHtML

"值: \(b)"
来源：http://baike.bbcook.cn/Article/details/glmqcrnrc.sHtML

[T19] Swift：可选绑定
来源：http://blog.vehdjk.com/Article/details/gnyjjzrbx.sHtML

if let n = opt { print(n) }
来源：http://www.share.epnwcf.com/Article/details/gtpitnbin.sHtML

[T20] Swift：数组操作
来源：http://www.share.vehdjk.com/Article/details/gdubesvdc.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://read.share.tarul.cn/Article/details/gfvayeuii.sHtML

[T21] Swift：遍历
来源：http://wap.bbcook.cn/Article/details/gxbxbabkn.sHtML

for x in a { print(x) }
来源：http://m.share.sjlbkw.cn/Article/details/gpoklthmw.sHtML

[T22] Swift：字典
来源：http://m.share.bbcook.cn/Article/details/gaxlplllj.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://baike.tarul.cn/Article/details/geeatfngs.sHtML

[T23] Swift：函数
来源：http://wap.vehdjk.com/Article/details/gksfaqjfb.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.m.share.vehdjk.com/Article/details/gdrqkgbhn.sHtML

[T24] Swift：闭包
来源：http://www.share.yfazqb.com/Article/details/gmkmgvmoy.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.m.share.bbcook.cn/Article/details/gabyuurrt.sHtML

[T25] Swift：结构体
来源：http://www.m.share.bbcook.cn/Article/details/ghmlbvizp.sHtML

struct P { var x: Int }
来源：http://3g.tarul.cn/Article/details/gjuhdgrim.sHtML

[T26] Swift：类与重写
来源：http://www.m.share.yfazqb.com/Article/details/goopurmvd.sHtML

class A: Base { override func f() {} }
来源：http://wap.sjlbkw.cn/Article/details/gpxrbatus.sHtML

[T27] Swift：错误处理
来源：http://www.m.share.yfazqb.com/Article/details/gwvkwrokd.sHtML

do { try f() } catch { print(error) }
来源：http://3g.bbcook.cn/Article/details/gfnehkzsn.sHtML

[T28] Swift：枚举
来源：http://www.blog.sjlbkw.cn/Article/details/gvoubpflv.sHtML

enum Color { case red, green }
来源：http://wap.bbcook.cn/Article/details/gagrapnsi.sHtML

[T29] Swift：guard 提前返回
来源：http://baike.vehdjk.com/Article/details/gpvgstbbe.sHtML

guard let x = opt else { return }
来源：http://www.blog.epnwcf.com/Article/details/gynjhdnuw.sHtML

[T30] Swift：协议
来源：http://m.share.yfazqb.com/Article/details/gjhwuumxo.sHtML

protocol Shape { func area() -> Double }
来源：http://www.blog.yfazqb.com/Article/details/gjbgtiglm.sHtML

[T31] Lua：Hello World
来源：http://wap.yfazqb.com/Article/details/gcpnqpbqr.sHtML

print("Hello")
来源：http://www.m.share.sjlbkw.cn/Article/details/gymqppuzd.sHtML

[T32] Lua：局部变量
来源：http://www.m.share.fktsv.cn/Article/details/gddwbqhtb.sHtML

local a = 1
来源：http://www.m.share.tarul.cn/Article/details/glkndppkq.sHtML

[T33] Lua：表（数组）
来源：http://blog.epnwcf.com/Article/details/gvjtddkre.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.blog.sjlbkw.cn/Article/details/ggyldwtet.sHtML

[T34] Lua：遍历表
来源：http://www.m.share.epnwcf.com/Article/details/glrlrtpdg.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.m.share.sjlbkw.cn/Article/details/ggxssxrlf.sHtML


<!-- 参考信息 -->