代发 wailian999

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.share.yfazqb.com/Article/details/gljidctmn.sHtML

[R26] 命令替换
来源：http://www.share.sjlbkw.cn/Article/details/gphdrbhok.sHtML

now=$(date +%F); echo "$now"
来源：http://www.blog.tarul.cn/Article/details/gvkpfqmnw.sHtML

[R27] 算术展开
来源：http://blog.tarul.cn/Article/details/gqkbavtmm.sHtML

echo $((1 + 2 * 3))
来源：http://m.share.bbcook.cn/Article/details/gdepawgyj.sHtML

[R28] 浮点运算
来源：http://m.share.sjlbkw.cn/Article/details/gybcjgcni.sHtML

echo "scale=2; 10/3" | bc
来源：http://baike.fktsv.cn/Article/details/gobatjgiz.sHtML

[R29] 定义函数
来源：http://3g.bbcook.cn/Article/details/gitbydhbk.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://wap.fktsv.cn/Article/details/gazqwtufo.sHtML

[R30] 函数返回状态码
来源：http://www.m.share.yfazqb.com/Article/details/gtmtyvkqy.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://wap.bbcook.cn/Article/details/gclwocilo.sHtML

[R31] 局部变量
来源：http://www.blog.bbcook.cn/Article/details/gtsqzlfgo.sHtML

f() { local x=1; echo "$x"; }
来源：http://mobile.sjlbkw.cn/Article/details/gimyvsfqh.sHtML

[R32] 参数个数校验
来源：http://read.share.yfazqb.com/Article/details/goqzalyym.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://blog.vehdjk.com/Article/details/gnsinmgdg.sHtML

[R33] 捕获错误并提示行号
来源：http://read.share.bbcook.cn/Article/details/gpootqqmc.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://read.share.vehdjk.com/Article/details/gykjqrugg.sHtML

[R34] 退出时清理
来源：http://blog.yfazqb.com/Article/details/gdsgaihke.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://mobile.tarul.cn/Article/details/gticnydie.sHtML

[R35] 后台执行并等待
来源：http://blog.vehdjk.com/Article/details/gdihvfxkl.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://3g.fktsv.cn/Article/details/gyptyndvg.sHtML

[R36] 并发执行多个任务
来源：http://wap.fktsv.cn/Article/details/gjcibbjvv.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://wap.vehdjk.com/Article/details/gvdxseorl.sHtML

[R37] 把输出赋给变量
来源：http://baike.fktsv.cn/Article/details/gvhtztwgp.sHtML

files=$(ls -1)
来源：http://www.m.share.bbcook.cn/Article/details/gzjzcpscb.sHtML

[R38] 管道串联
来源：http://blog.epnwcf.com/Article/details/gcboetpqp.sHtML

cat a.txt | grep -i error | wc -l
来源：http://blog.yfazqb.com/Article/details/gognranzf.sHtML

[R39] 重定向标准输出与错误
来源：http://3g.tarul.cn/Article/details/gudihvxhf.sHtML

cmd > out.log 2>&1
来源：http://read.share.bbcook.cn/Article/details/gckmsimsi.sHtML

[R40] 追加写日志
来源：http://wap.tarul.cn/Article/details/gfykwfjhm.sHtML

echo "log" >> out.log
来源：http://www.m.share.bbcook.cn/Article/details/gvpwnkjlm.sHtML

[R41] 丢弃输出
来源：http://3g.sjlbkw.cn/Article/details/gmjudrxwl.sHtML

cmd >/dev/null 2>&1
来源：http://m.share.tarul.cn/Article/details/gbnhjwuql.sHtML

[R42] 输入重定向
来源：http://baike.sjlbkw.cn/Article/details/gauxmusej.sHtML

wc -l < a.txt
来源：http://wap.vehdjk.com/Article/details/gbyozorir.sHtML

[R43] 按名字查找文件
来源：http://wap.fktsv.cn/Article/details/gwvqmvuqx.sHtML

find . -name "*.log" -type f
来源：http://www.share.epnwcf.com/Article/details/gcbhadkiv.sHtML

[R44] 按修改时间查找
来源：http://www.m.share.bbcook.cn/Article/details/gvaiwhhoz.sHtML

find . -mtime -7 -type f
来源：http://www.m.share.vehdjk.com/Article/details/gpnhbxjjq.sHtML

[R45] 批量删除
来源：http://www.m.share.epnwcf.com/Article/details/gkgnsmhpt.sHtML

find . -name "*.tmp" -delete
来源：http://m.share.vehdjk.com/Article/details/ggltruloq.sHtML

[R46] 递归替换文件内容
来源：http://3g.tarul.cn/Article/details/gcznwndtt.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.m.share.vehdjk.com/Article/details/gmsrkvljq.sHtML

[R47] sed 单行替换
来源：http://mobile.epnwcf.com/Article/details/gjfejclpp.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.share.sjlbkw.cn/Article/details/gkkudncyf.sHtML

[R48] awk 取指定列
来源：http://wap.yfazqb.com/Article/details/gvareqdpm.sHtML

awk '{print $1, $3}' a.txt
来源：http://3g.vehdjk.com/Article/details/gxiepvkzs.sHtML

[R49] awk 带条件
来源：http://3g.fktsv.cn/Article/details/gfmmoxwbq.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.m.share.bbcook.cn/Article/details/gxzianvqp.sHtML

[R50] awk 求和
来源：http://wap.yfazqb.com/Article/details/gevlebnih.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.share.yfazqb.com/Article/details/gexkwrdqp.sHtML

[R51] 排序去重取前几
来源：http://mobile.yfazqb.com/Article/details/gfrnvypuw.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://3g.epnwcf.com/Article/details/ggszbnurx.sHtML

[R52] 统计行数
来源：http://mobile.yfazqb.com/Article/details/gyyitzsfc.sHtML

wc -l a.txt
来源：http://mobile.fktsv.cn/Article/details/gjuelvfba.sHtML

[R53] 查看文件头与实时尾
来源：http://www.share.vehdjk.com/Article/details/gbedlsokf.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.m.share.vehdjk.com/Article/details/guxxgqbom.sHtML

[R54] 比较两个文件
来源：http://read.share.sjlbkw.cn/Article/details/gylywcidp.sHtML

diff a.txt b.txt
来源：http://blog.yfazqb.com/Article/details/glxikwnck.sHtML

[R55] 压缩与解压
来源：http://www.m.share.vehdjk.com/Article/details/gximsaruz.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://blog.tarul.cn/Article/details/gkjlizvcl.sHtML

[R56] 远程拷贝
来源：http://3g.sjlbkw.cn/Article/details/gxfvixbch.sHtML

scp file user@host:/path/
来源：http://blog.fktsv.cn/Article/details/godjrzzhu.sHtML

[R57] 远程执行命令
来源：http://blog.tarul.cn/Article/details/grmnoqetw.sHtML

ssh user@host 'uptime'
来源：http://read.share.bbcook.cn/Article/details/gayrtwoxa.sHtML

[R58] 下载文件
来源：http://blog.tarul.cn/Article/details/gbuwnzxga.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.blog.epnwcf.com/Article/details/grpksmvzv.sHtML

[R59] 发 POST JSON
来源：http://blog.tarul.cn/Article/details/guprdqpmr.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://read.share.sjlbkw.cn/Article/details/geiyjrdxr.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.blog.yfazqb.com/Article/details/gecrvecaw.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://m.share.bbcook.cn/Article/details/gqhsrlkrg.sHtML

[R61] 磁盘占用
来源：http://www.blog.fktsv.cn/Article/details/grywgcysl.sHtML

df -h;  du -sh *
来源：http://m.share.vehdjk.com/Article/details/gtuixjiwy.sHtML

[R62] 找最占空间的文件
来源：http://m.share.sjlbkw.cn/Article/details/gqqatjqds.sHtML

du -ah . | sort -rh | head -10
来源：http://www.share.sjlbkw.cn/Article/details/goqnfnqso.sHtML

[R63] 内存与进程
来源：http://wap.bbcook.cn/Article/details/gqbxqaqhn.sHtML

free -h;  ps aux | grep nginx
来源：http://mobile.vehdjk.com/Article/details/gmteovooy.sHtML

[R64] 结束进程
来源：http://mobile.fktsv.cn/Article/details/gspekpruo.sHtML

kill -9 $(pgrep -f app.py)
来源：http://3g.sjlbkw.cn/Article/details/glwxfpsii.sHtML

[R65] 查看端口占用
来源：http://blog.yfazqb.com/Article/details/gxnokqfys.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://3g.tarul.cn/Article/details/gbezwxbzq.sHtML

[R66] 定时任务
来源：http://www.blog.epnwcf.com/Article/details/gwfvdttjp.sHtML

crontab -e;  crontab -l
来源：http://blog.tarul.cn/Article/details/gmbzgjelh.sHtML

[R67] 生成随机十六进制串
来源：http://baike.bbcook.cn/Article/details/guljmwewt.sHtML

openssl rand -hex 16
来源：http://m.share.sjlbkw.cn/Article/details/gwsdqqwsg.sHtML

[R68] 计算文件校验值
来源：http://m.share.bbcook.cn/Article/details/gflhbbvwz.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.blog.sjlbkw.cn/Article/details/gzpimlahj.sHtML

[R69] 生成随机密码
来源：http://3g.bbcook.cn/Article/details/gjtfhjllf.sHtML

head -c 16 /dev/urandom | base64
来源：http://baike.epnwcf.com/Article/details/gqmfbrhlw.sHtML

[R70] 时间戳与互转
来源：http://m.share.yfazqb.com/Article/details/gwlcgurwr.sHtML

date +%s;  date -d @1700000000
来源：http://blog.epnwcf.com/Article/details/ghxjrhpks.sHtML

[R71] 日期格式化
来源：http://www.share.yfazqb.com/Article/details/ghjirudhb.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://mobile.bbcook.cn/Article/details/gfzgxzblx.sHtML

[R72] 等待端口就绪
来源：http://www.share.bbcook.cn/Article/details/gkisltchw.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://m.share.fktsv.cn/Article/details/gktljpoor.sHtML

[R73] 分割大日志
来源：http://www.blog.bbcook.cn/Article/details/gtagxiyoh.sHtML

split -l 1000 big.log part_
来源：http://read.share.epnwcf.com/Article/details/gjohpoznz.sHtML

[R74] 批量重命名
来源：http://m.share.yfazqb.com/Article/details/grsmuswin.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://blog.tarul.cn/Article/details/gagtcqjqr.sHtML

[R75] 导出环境变量
来源：http://baike.epnwcf.com/Article/details/gbrpivukn.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://read.share.tarul.cn/Article/details/gmpblkitt.sHtML

[R76] 使用临时文件
来源：http://3g.bbcook.cn/Article/details/gkiegkwoi.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://mobile.yfazqb.com/Article/details/gilnchxnz.sHtML

[R77] 读取用户输入
来源：http://wap.tarul.cn/Article/details/gbuitaxur.sHtML

read -rp "请输入: " ans
来源：http://baike.vehdjk.com/Article/details/gyjarqctn.sHtML

[R78] 交互式菜单
来源：http://baike.tarul.cn/Article/details/ghaeteeaf.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.share.epnwcf.com/Article/details/gslgzzpth.sHtML

[R79] 解析命令行选项
来源：http://blog.yfazqb.com/Article/details/ggifxxyvj.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://baike.tarul.cn/Article/details/gnozhslao.sHtML

[R80] 查看脚本执行耗时
来源：http://www.share.epnwcf.com/Article/details/guxuynavp.sHtML

time ./run.sh
来源：http://mobile.fktsv.cn/Article/details/gvgdfjaxl.sHtML

================================================================================
来源：http://wap.sjlbkw.cn/Article/details/gnuxwgnjq.sHtML

S. C / C++ 专题
来源：http://baike.tarul.cn/Article/details/gcnoohdja.sHtML

================================================================================
来源：http://read.share.vehdjk.com/Article/details/gzvnlwvgi.sHtML

[S01] C：Hello World
来源：http://m.share.sjlbkw.cn/Article/details/gmpfimgth.sHtML

#include <stdio.h>
来源：http://read.share.yfazqb.com/Article/details/ggywlveqi.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://wap.sjlbkw.cn/Article/details/gbexalnfr.sHtML

[S02] C：变量与格式化输出
来源：http://www.blog.epnwcf.com/Article/details/goxzukgyg.sHtML

int a = 10; printf("%d\n", a);
来源：http://wap.vehdjk.com/Article/details/gtewrobko.sHtML

[S03] C：读入整数
来源：http://3g.vehdjk.com/Article/details/gcjydkokg.sHtML

int x; scanf("%d", &x);
来源：http://m.share.sjlbkw.cn/Article/details/gzjbvhmhv.sHtML

[S04] C：字符串复制
来源：http://www.m.share.fktsv.cn/Article/details/gnkoxzluf.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://blog.sjlbkw.cn/Article/details/gptmznayd.sHtML

[S05] C：字符串长度
来源：http://m.share.vehdjk.com/Article/details/gaovywtkm.sHtML

strlen(s)
来源：http://mobile.fktsv.cn/Article/details/ggzcxgogq.sHtML

[S06] C：字符串比较
来源：http://baike.bbcook.cn/Article/details/gbgbfvnqc.sHtML

strcmp(a, b) == 0
来源：http://baike.vehdjk.com/Article/details/gmdaptfzc.sHtML

[S07] C：数组遍历求和
来源：http://m.share.fktsv.cn/Article/details/ggdxrznkq.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://baike.bbcook.cn/Article/details/grtyxweek.sHtML

[S08] C：动态内存分配与释放
来源：http://www.blog.sjlbkw.cn/Article/details/gvcdnklqf.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.share.tarul.cn/Article/details/gtljwdpxy.sHtML

[S09] C：结构体定义与初始化
来源：http://blog.yfazqb.com/Article/details/gnblolngg.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.m.share.sjlbkw.cn/Article/details/gippsiybt.sHtML

[S10] C：指针与解引用
来源：http://baike.sjlbkw.cn/Article/details/gekziiati.sHtML

int *p = &a;  *p = 5;
来源：http://mobile.sjlbkw.cn/Article/details/gbzpmtxsb.sHtML

[S11] C：逐行读文件
来源：http://www.m.share.bbcook.cn/Article/details/gyxdcegox.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://3g.sjlbkw.cn/Article/details/gztcnodzh.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://wap.tarul.cn/Article/details/gcfvbaury.sHtML

fclose(f);
来源：http://m.share.sjlbkw.cn/Article/details/gbwnjpkez.sHtML

[S12] C：写文件
来源：http://baike.sjlbkw.cn/Article/details/gukspzpqs.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.blog.yfazqb.com/Article/details/goeyihikm.sHtML

[S13] C：宏定义
来源：http://mobile.bbcook.cn/Article/details/gkyodwooj.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.m.share.tarul.cn/Article/details/gastoggaj.sHtML

[S14] C：枚举
来源：http://www.share.yfazqb.com/Article/details/gglpdvhmz.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://m.share.vehdjk.com/Article/details/gsrxmowkl.sHtML

[S15] C：类型转换
来源：http://m.share.yfazqb.com/Article/details/gomzzfzbn.sHtML

(double) a / b
来源：http://blog.epnwcf.com/Article/details/giwzlkiub.sHtML

[S16] C：位操作置位
来源：http://wap.sjlbkw.cn/Article/details/giwzfpknq.sHtML

x |= (1 << 3);
来源：http://3g.vehdjk.com/Article/details/gxwtwwgdk.sHtML

[S17] C：安全拼接字符串
来源：http://wap.vehdjk.com/Article/details/gaqlbgtob.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.blog.yfazqb.com/Article/details/gtnciqfdz.sHtML

[S18] C：命令行参数
来源：http://www.m.share.vehdjk.com/Article/details/gaodetdkh.sHtML

int main(int argc, char **argv)
来源：http://www.share.fktsv.cn/Article/details/ggdganmiv.sHtML

[S19] C：快速排序
来源：http://www.share.vehdjk.com/Article/details/gxziomtlj.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://blog.yfazqb.com/Article/details/gazcenxwy.sHtML

[S20] C：二分查找
来源：http://m.share.vehdjk.com/Article/details/gftnlzowo.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://blog.vehdjk.com/Article/details/gposcgcnm.sHtML

[S21] C：字符类别判断
来源：http://mobile.vehdjk.com/Article/details/gfziswmbo.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://read.share.yfazqb.com/Article/details/gzrrlpydn.sHtML

[S22] C：字符串转数字
来源：http://www.blog.fktsv.cn/Article/details/gwbngdher.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://wap.bbcook.cn/Article/details/gneefdcwz.sHtML

[S23] C：随机数
来源：http://3g.tarul.cn/Article/details/ggntlhfqc.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://wap.sjlbkw.cn/Article/details/gtjvdhazg.sHtML

[S24] C：获取本地时间
来源：http://m.share.tarul.cn/Article/details/gfuewrlfv.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://wap.yfazqb.com/Article/details/gxcydjxaj.sHtML

[S25] C：内存拷贝
来源：http://read.share.epnwcf.com/Article/details/gysndfhyk.sHtML

memcpy(dst, src, n);
来源：http://m.share.tarul.cn/Article/details/gwilpmzir.sHtML

[S26] C：内存清零
来源：http://baike.fktsv.cn/Article/details/gklkigbiv.sHtML

memset(a, 0, sizeof a);
来源：http://blog.yfazqb.com/Article/details/guvhjanni.sHtML

[S27] C：定义常量
来源：http://m.share.bbcook.cn/Article/details/gyjjruqnb.sHtML

const double PI = 3.14159;
来源：http://3g.tarul.cn/Article/details/grbegbhwt.sHtML

[S28] C：静态变量
来源：http://www.blog.yfazqb.com/Article/details/gippytnyb.sHtML

static int counter = 0;
来源：http://wap.fktsv.cn/Article/details/gsivhyydt.sHtML

[S29] C：变参函数
来源：http://www.blog.sjlbkw.cn/Article/details/gwhyzuone.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://blog.vehdjk.com/Article/details/gvoczougs.sHtML

[S30] C：头文件保护
来源：http://read.share.sjlbkw.cn/Article/details/gwvhiviah.sHtML

#ifndef X_H
来源：http://mobile.epnwcf.com/Article/details/gtaqccbng.sHtML

#define X_H
来源：http://wap.bbcook.cn/Article/details/gjejnpcdx.sHtML

#endif
来源：http://3g.fktsv.cn/Article/details/gpfnunqpf.sHtML

[S31] C++：Hello World
来源：http://www.blog.tarul.cn/Article/details/gbtdigasx.sHtML

#include <iostream>
来源：http://mobile.vehdjk.com/Article/details/gbpbvafmg.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.share.fktsv.cn/Article/details/geqhzmfuo.sHtML

[S32] C++：字符串
来源：http://www.share.epnwcf.com/Article/details/gwtjjqdqe.sHtML

std::string s = "hi";  s += "!";
来源：http://www.blog.epnwcf.com/Article/details/gryvaffcm.sHtML

[S33] C++：vector 增删
来源：http://blog.yfazqb.com/Article/details/gqihclznf.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://baike.sjlbkw.cn/Article/details/grsrwuaic.sHtML

[S34] C++：遍历 vector
来源：http://www.blog.fktsv.cn/Article/details/gihsfxkzp.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://baike.vehdjk.com/Article/details/gzfkorqux.sHtML

[S35] C++：map
来源：http://www.m.share.fktsv.cn/Article/details/gnqpusqms.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.epnwcf.com/Article/details/ghbxulfed.sHtML

[S36] C++：unordered_map
来源：http://m.share.vehdjk.com/Article/details/gozxmouzk.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wap.bbcook.cn/Article/details/gtwbzqjci.sHtML

[S37] C++：set
来源：http://baike.fktsv.cn/Article/details/gtmeebzur.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://3g.yfazqb.com/Article/details/gemoommrz.sHtML

[S38] C++：排序
来源：http://mobile.bbcook.cn/Article/details/gicbfrcre.sHtML

std::sort(v.begin(), v.end());
来源：http://m.share.epnwcf.com/Article/details/gbwasaabr.sHtML

[S39] C++：自定义比较器排序
来源：http://read.share.tarul.cn/Article/details/grprpppim.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.m.share.sjlbkw.cn/Article/details/gyodjidyn.sHtML

[S40] C++：查找元素
来源：http://read.share.vehdjk.com/Article/details/gvcgeesjm.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://mobile.vehdjk.com/Article/details/gibegequc.sHtML

[S41] C++：类与构造函数
来源：http://read.share.vehdjk.com/Article/details/gvaiampcv.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://3g.vehdjk.com/Article/details/guinockjk.sHtML

[S42] C++：继承与虚函数
来源：http://www.m.share.tarul.cn/Article/details/gfcrtzjyd.sHtML

class B : public Base { public: void f() override {} };
来源：http://3g.bbcook.cn/Article/details/gprqwbrhz.sHtML

[S43] C++：智能指针
来源：http://3g.vehdjk.com/Article/details/gqwovglpx.sHtML

auto p = std::make_unique<int>(5);
来源：http://3g.yfazqb.com/Article/details/gdeyevyjz.sHtML

[S44] C++：引用传参
来源：http://mobile.bbcook.cn/Article/details/gzjfzerdj.sHtML

void inc(int &x) { ++x; }
来源：http://blog.yfazqb.com/Article/details/gzzuwbexv.sHtML

[S45] C++：lambda
来源：http://www.blog.vehdjk.com/Article/details/ghqjrbcrl.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://wap.yfazqb.com/Article/details/gcdttkfyl.sHtML

[S46] C++：函数模板
来源：http://read.share.vehdjk.com/Article/details/gnboubmxe.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.m.share.bbcook.cn/Article/details/gcrkvjqzc.sHtML

[S47] C++：结构化绑定遍历
来源：http://blog.vehdjk.com/Article/details/gunmrhjup.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://blog.yfazqb.com/Article/details/gcxtqwsjj.sHtML

[S48] C++：逐行读文件
来源：http://www.share.fktsv.cn/Article/details/gwkejcthc.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://mobile.yfazqb.com/Article/details/gbcjfjmlk.sHtML

while (std::getline(in, line)) { }
来源：http://m.share.fktsv.cn/Article/details/gjvhrrkwk.sHtML

[S49] C++：写文件
来源：http://m.share.vehdjk.com/Article/details/gcovljevx.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://3g.sjlbkw.cn/Article/details/ggxfsdtqj.sHtML

[S50] C++：格式化数字
来源：http://www.share.vehdjk.com/Article/details/gmroibjnz.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.share.yfazqb.com/Article/details/gwhapyovh.sHtML

[S51] C++：显式类型转换
来源：http://blog.tarul.cn/Article/details/gpqoeialb.sHtML

static_cast<double>(a) / b
来源：http://read.share.bbcook.cn/Article/details/gyizrxrer.sHtML

[S52] C++：const 与 noexcept
来源：http://read.share.sjlbkw.cn/Article/details/gtbqgblfz.sHtML

int size() const noexcept { return n_; }
来源：http://mobile.yfazqb.com/Article/details/gqqndlcxy.sHtML

[S53] C++：移动语义
来源：http://baike.yfazqb.com/Article/details/geeeluupn.sHtML

std::vector<int> w = std::move(v);
来源：http://baike.bbcook.cn/Article/details/gelryotsd.sHtML

[S54] C++：异常处理
来源：http://m.share.fktsv.cn/Article/details/gtryejiww.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.blog.yfazqb.com/Article/details/ggvxhwzpv.sHtML

[S55] C++：结构化绑定
来源：http://read.share.sjlbkw.cn/Article/details/givxafpot.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://read.share.sjlbkw.cn/Article/details/gkmyspyhn.sHtML

[S56] C++：optional
来源：http://read.share.yfazqb.com/Article/details/grfmvqmjy.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.share.tarul.cn/Article/details/gvbumnidk.sHtML

[S57] C++：编译期常量
来源：http://m.share.tarul.cn/Article/details/gjpdhqsnt.sHtML

constexpr int N = 10;
来源：http://www.m.share.bbcook.cn/Article/details/godkysued.sHtML

[S58] C++：命名空间
来源：http://www.share.yfazqb.com/Article/details/gegrdrsqe.sHtML

namespace ns { int f() { return 1; } }
来源：http://m.share.epnwcf.com/Article/details/gpgaezbzf.sHtML

[S59] C++：静态断言
来源：http://www.share.tarul.cn/Article/details/ggquxluuj.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://mobile.tarul.cn/Article/details/gjwuauvho.sHtML

[S60] C++：遍历并删除元素
来源：http://www.share.bbcook.cn/Article/details/ggxcdvinp.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://read.share.yfazqb.com/Article/details/gpaxbqhwf.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/gkurgxzfe.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://wap.vehdjk.com/Article/details/geqpabbyf.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/gkxrcpkkd.sHtML

[T01] Kotlin：Hello World
来源：http://www.m.share.fktsv.cn/Article/details/gdgnpacau.sHtML

println("Hello")
来源：http://read.share.tarul.cn/Article/details/gfnozlpmq.sHtML

[T02] Kotlin：变量
来源：http://mobile.fktsv.cn/Article/details/gkxdxznym.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://mobile.vehdjk.com/Article/details/gcunknfpb.sHtML

[T03] Kotlin：字符串模板
来源：http://www.share.yfazqb.com/Article/details/goaspwywc.sHtML

"值: $b"
来源：http://3g.bbcook.cn/Article/details/gjrmalmnh.sHtML

[T04] Kotlin：空安全
来源：http://wap.bbcook.cn/Article/details/gduhckcmh.sHtML

val n: String? = null;  n?.length
来源：http://baike.yfazqb.com/Article/details/gezpplkwr.sHtML

[T05] Kotlin：when 表达式
来源：http://www.share.yfazqb.com/Article/details/gpqrmwxna.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://wap.vehdjk.com/Article/details/gcpqmbwmd.sHtML

[T06] Kotlin：集合映射
来源：http://baike.yfazqb.com/Article/details/gdieybhuk.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://3g.fktsv.cn/Article/details/gipwfmjat.sHtML

[T07] Kotlin：集合过滤
来源：http://m.share.bbcook.cn/Article/details/glkwoapct.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://wap.fktsv.cn/Article/details/gycetrkjl.sHtML

[T08] Kotlin：数据类
来源：http://blog.fktsv.cn/Article/details/gmusifvop.sHtML

data class User(val name: String, val age: Int)
来源：http://www.share.tarul.cn/Article/details/gyxvocgmx.sHtML

[T09] Kotlin：扩展函数
来源：http://www.blog.sjlbkw.cn/Article/details/gniuecztp.sHtML

fun String.exclaim() = this + "!"
来源：http://read.share.vehdjk.com/Article/details/ggnprnufz.sHtML

[T10] Kotlin：默认参数
来源：http://www.share.yfazqb.com/Article/details/gemprumsb.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://mobile.vehdjk.com/Article/details/gbauivmcw.sHtML

[T11] Kotlin：协程
来源：http://3g.bbcook.cn/Article/details/goyodxerm.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.blog.yfazqb.com/Article/details/gjmqxlulf.sHtML

[T12] Kotlin：解构声明
来源：http://m.share.bbcook.cn/Article/details/gxqpodrvl.sHtML

val (a, b) = Pair(1, 2)
来源：http://blog.fktsv.cn/Article/details/gbbbtktzj.sHtML

[T13] Kotlin：只读 Map
来源：http://www.blog.bbcook.cn/Article/details/gfhybhpde.sHtML

val m = mapOf("a" to 1)
来源：http://wap.yfazqb.com/Article/details/gowngaljj.sHtML

[T14] Kotlin：循环
来源：http://mobile.vehdjk.com/Article/details/gugklalye.sHtML

for (i in 1..10) println(i)
来源：http://blog.epnwcf.com/Article/details/gxwtcipwv.sHtML

[T15] Kotlin：接口
来源：http://www.blog.sjlbkw.cn/Article/details/gylbdtvls.sHtML

interface Shape { fun area(): Double }
来源：http://baike.vehdjk.com/Article/details/ghpevdeii.sHtML

[T16] Swift：Hello World
来源：http://www.share.bbcook.cn/Article/details/godryeqkh.sHtML

print("Hello")
来源：http://blog.vehdjk.com/Article/details/gseodibus.sHtML

[T17] Swift：变量与常量
来源：http://3g.epnwcf.com/Article/details/gdtbwcqmv.sHtML

var a = 1;  let b = 2
来源：http://3g.epnwcf.com/Article/details/glneqwhgt.sHtML

[T18] Swift：字符串插值
来源：http://3g.vehdjk.com/Article/details/grhirbhhl.sHtML

"值: \(b)"
来源：http://read.share.epnwcf.com/Article/details/geldvfucd.sHtML

[T19] Swift：可选绑定
来源：http://www.share.tarul.cn/Article/details/gezvjtpfa.sHtML

if let n = opt { print(n) }
来源：http://blog.tarul.cn/Article/details/glcmgyfjh.sHtML

[T20] Swift：数组操作
来源：http://www.share.vehdjk.com/Article/details/gbxbnkvnv.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.blog.yfazqb.com/Article/details/gwoeuzyhz.sHtML

[T21] Swift：遍历
来源：http://mobile.vehdjk.com/Article/details/gxeepdpjh.sHtML

for x in a { print(x) }
来源：http://wap.tarul.cn/Article/details/goqjiaqxb.sHtML

[T22] Swift：字典
来源：http://www.share.yfazqb.com/Article/details/gfdwvzeov.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.share.vehdjk.com/Article/details/gpffgrwri.sHtML

[T23] Swift：函数
来源：http://www.share.yfazqb.com/Article/details/gatbnhhjj.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.share.yfazqb.com/Article/details/gwhjxuuxm.sHtML

[T24] Swift：闭包
来源：http://wap.tarul.cn/Article/details/gffjsqvti.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.m.share.yfazqb.com/Article/details/gamyflmnh.sHtML

[T25] Swift：结构体
来源：http://www.share.bbcook.cn/Article/details/gdughwzkg.sHtML

struct P { var x: Int }
来源：http://www.m.share.tarul.cn/Article/details/gazstpztl.sHtML

[T26] Swift：类与重写
来源：http://www.m.share.tarul.cn/Article/details/gedngppfi.sHtML

class A: Base { override func f() {} }
来源：http://mobile.yfazqb.com/Article/details/gvxabwitw.sHtML

[T27] Swift：错误处理
来源：http://www.share.epnwcf.com/Article/details/gcfrujasw.sHtML

do { try f() } catch { print(error) }
来源：http://www.share.fktsv.cn/Article/details/goemebsyf.sHtML

[T28] Swift：枚举
来源：http://wap.epnwcf.com/Article/details/gapkxwpob.sHtML

enum Color { case red, green }
来源：http://blog.fktsv.cn/Article/details/ggryqqxkh.sHtML


<!-- 参考信息 -->