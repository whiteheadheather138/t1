代发 wailian999

f() { local x=1; echo "$x"; }
来源：http://3g.tarul.cn/Article/details/gmoqqmcpk.sHtML

[R32] 参数个数校验
来源：http://m.share.epnwcf.com/Article/details/gmgfxecdz.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://m.share.vehdjk.com/Article/details/gpdocohch.sHtML

[R33] 捕获错误并提示行号
来源：http://m.share.vehdjk.com/Article/details/gtqyqonjj.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://mobile.tarul.cn/Article/details/gpkvaaoih.sHtML

[R34] 退出时清理
来源：http://www.share.sjlbkw.cn/Article/details/ghagfzybb.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.tarul.cn/Article/details/gjsmyfwer.sHtML

[R35] 后台执行并等待
来源：http://mobile.bbcook.cn/Article/details/ggoaomnfi.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://mobile.vehdjk.com/Article/details/gyarnhrwt.sHtML

[R36] 并发执行多个任务
来源：http://read.share.epnwcf.com/Article/details/gurwuuxia.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://m.share.bbcook.cn/Article/details/grlydcwls.sHtML

[R37] 把输出赋给变量
来源：http://www.m.share.bbcook.cn/Article/details/gujrdclyu.sHtML

files=$(ls -1)
来源：http://read.share.sjlbkw.cn/Article/details/gbsriuelx.sHtML

[R38] 管道串联
来源：http://mobile.fktsv.cn/Article/details/gawccnffq.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.blog.vehdjk.com/Article/details/gybfyexgy.sHtML

[R39] 重定向标准输出与错误
来源：http://3g.tarul.cn/Article/details/gbhgbtjcg.sHtML

cmd > out.log 2>&1
来源：http://mobile.fktsv.cn/Article/details/gsydugexa.sHtML

[R40] 追加写日志
来源：http://www.blog.bbcook.cn/Article/details/gsgyrxkst.sHtML

echo "log" >> out.log
来源：http://3g.vehdjk.com/Article/details/gtegdoiey.sHtML

[R41] 丢弃输出
来源：http://wap.bbcook.cn/Article/details/gmxnavxat.sHtML

cmd >/dev/null 2>&1
来源：http://baike.epnwcf.com/Article/details/gjbprpomp.sHtML

[R42] 输入重定向
来源：http://3g.epnwcf.com/Article/details/gfdfncupl.sHtML

wc -l < a.txt
来源：http://www.blog.yfazqb.com/Article/details/gaqubibnk.sHtML

[R43] 按名字查找文件
来源：http://3g.tarul.cn/Article/details/gahvbugjn.sHtML

find . -name "*.log" -type f
来源：http://3g.tarul.cn/Article/details/gttsczvup.sHtML

[R44] 按修改时间查找
来源：http://3g.epnwcf.com/Article/details/gsrgjvjnj.sHtML

find . -mtime -7 -type f
来源：http://wap.tarul.cn/Article/details/guxrtoyxk.sHtML

[R45] 批量删除
来源：http://read.share.sjlbkw.cn/Article/details/gyavxiukx.sHtML

find . -name "*.tmp" -delete
来源：http://3g.sjlbkw.cn/Article/details/ggozzalyt.sHtML

[R46] 递归替换文件内容
来源：http://3g.fktsv.cn/Article/details/gcsrvrfic.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://read.share.tarul.cn/Article/details/gypmcwezq.sHtML

[R47] sed 单行替换
来源：http://mobile.bbcook.cn/Article/details/gfrmfntst.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.share.epnwcf.com/Article/details/gwfduzomr.sHtML

[R48] awk 取指定列
来源：http://blog.vehdjk.com/Article/details/gfufmvbgx.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.share.tarul.cn/Article/details/grazxhzhy.sHtML

[R49] awk 带条件
来源：http://read.share.fktsv.cn/Article/details/gythmesys.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.share.epnwcf.com/Article/details/gunmrnzkr.sHtML

[R50] awk 求和
来源：http://baike.vehdjk.com/Article/details/gftvhhukz.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://m.share.bbcook.cn/Article/details/guscchdjy.sHtML

[R51] 排序去重取前几
来源：http://3g.bbcook.cn/Article/details/gaweyxjva.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://read.share.sjlbkw.cn/Article/details/gtmulbfqa.sHtML

[R52] 统计行数
来源：http://blog.epnwcf.com/Article/details/gkdnyxdax.sHtML

wc -l a.txt
来源：http://blog.fktsv.cn/Article/details/gaxrwfhot.sHtML

[R53] 查看文件头与实时尾
来源：http://read.share.sjlbkw.cn/Article/details/gwzeczvle.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://m.share.yfazqb.com/Article/details/gojtmgoqj.sHtML

[R54] 比较两个文件
来源：http://blog.sjlbkw.cn/Article/details/gdxihoksv.sHtML

diff a.txt b.txt
来源：http://wap.sjlbkw.cn/Article/details/gayllmrmc.sHtML

[R55] 压缩与解压
来源：http://baike.tarul.cn/Article/details/gbzjwoijq.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://baike.epnwcf.com/Article/details/gdqzxbabl.sHtML

[R56] 远程拷贝
来源：http://wap.vehdjk.com/Article/details/ggticfbwo.sHtML

scp file user@host:/path/
来源：http://blog.epnwcf.com/Article/details/gxcyuauda.sHtML

[R57] 远程执行命令
来源：http://www.blog.tarul.cn/Article/details/gwczwfunw.sHtML

ssh user@host 'uptime'
来源：http://mobile.vehdjk.com/Article/details/gkpuwxgxb.sHtML

[R58] 下载文件
来源：http://www.blog.epnwcf.com/Article/details/gcbmdnnit.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://m.share.fktsv.cn/Article/details/gwnlsljcu.sHtML

[R59] 发 POST JSON
来源：http://mobile.fktsv.cn/Article/details/gfmnqzkpj.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://blog.sjlbkw.cn/Article/details/gwpidxpin.sHtML

[R60] 只看 HTTP 状态码
来源：http://read.share.bbcook.cn/Article/details/gnrdejgah.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.blog.vehdjk.com/Article/details/gqcmctclr.sHtML

[R61] 磁盘占用
来源：http://www.blog.sjlbkw.cn/Article/details/gjqbzregr.sHtML

df -h;  du -sh *
来源：http://baike.yfazqb.com/Article/details/gnqjlfszk.sHtML

[R62] 找最占空间的文件
来源：http://3g.sjlbkw.cn/Article/details/gqslratsk.sHtML

du -ah . | sort -rh | head -10
来源：http://www.m.share.vehdjk.com/Article/details/gbskdaqwn.sHtML

[R63] 内存与进程
来源：http://baike.fktsv.cn/Article/details/gnthaejqh.sHtML

free -h;  ps aux | grep nginx
来源：http://www.share.epnwcf.com/Article/details/godreyucr.sHtML

[R64] 结束进程
来源：http://wap.sjlbkw.cn/Article/details/gwbuwpxzq.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.m.share.tarul.cn/Article/details/gdyytdsia.sHtML

[R65] 查看端口占用
来源：http://www.blog.bbcook.cn/Article/details/gfrzaaafa.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://blog.vehdjk.com/Article/details/gqvpngwmf.sHtML

[R66] 定时任务
来源：http://baike.bbcook.cn/Article/details/giqjhjlfo.sHtML

crontab -e;  crontab -l
来源：http://www.m.share.epnwcf.com/Article/details/gpjgqexam.sHtML

[R67] 生成随机十六进制串
来源：http://www.blog.bbcook.cn/Article/details/glsihxiql.sHtML

openssl rand -hex 16
来源：http://baike.epnwcf.com/Article/details/gbtsiofah.sHtML

[R68] 计算文件校验值
来源：http://www.share.yfazqb.com/Article/details/gfdvocknw.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://3g.bbcook.cn/Article/details/glsahmevz.sHtML

[R69] 生成随机密码
来源：http://www.share.yfazqb.com/Article/details/glrkslanc.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.share.yfazqb.com/Article/details/gcskvzbtg.sHtML

[R70] 时间戳与互转
来源：http://m.share.fktsv.cn/Article/details/gjszwiipr.sHtML

date +%s;  date -d @1700000000
来源：http://www.share.fktsv.cn/Article/details/giubpquzv.sHtML

[R71] 日期格式化
来源：http://mobile.vehdjk.com/Article/details/gppfggdad.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://wap.yfazqb.com/Article/details/goexojxyi.sHtML

[R72] 等待端口就绪
来源：http://www.blog.vehdjk.com/Article/details/gtyxpbrqj.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://baike.epnwcf.com/Article/details/gdfttninw.sHtML

[R73] 分割大日志
来源：http://m.share.yfazqb.com/Article/details/gbytujztf.sHtML

split -l 1000 big.log part_
来源：http://read.share.sjlbkw.cn/Article/details/gjmjzzgdb.sHtML

[R74] 批量重命名
来源：http://www.m.share.bbcook.cn/Article/details/gmalgyedd.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://m.share.bbcook.cn/Article/details/gzsobesdu.sHtML

[R75] 导出环境变量
来源：http://www.blog.tarul.cn/Article/details/glmqenisv.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.share.vehdjk.com/Article/details/gzmwrzabb.sHtML

[R76] 使用临时文件
来源：http://blog.tarul.cn/Article/details/ghezmxohy.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://wap.sjlbkw.cn/Article/details/gnjvduaef.sHtML

[R77] 读取用户输入
来源：http://wap.tarul.cn/Article/details/glhbbwotq.sHtML

read -rp "请输入: " ans
来源：http://m.share.sjlbkw.cn/Article/details/glnqffwru.sHtML

[R78] 交互式菜单
来源：http://3g.tarul.cn/Article/details/glzdmchxv.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://mobile.vehdjk.com/Article/details/gupjnpmrj.sHtML

[R79] 解析命令行选项
来源：http://mobile.fktsv.cn/Article/details/gcmnjhbum.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.m.share.epnwcf.com/Article/details/gmsbdfdez.sHtML

[R80] 查看脚本执行耗时
来源：http://www.share.yfazqb.com/Article/details/gilsbhyfu.sHtML

time ./run.sh
来源：http://read.share.epnwcf.com/Article/details/ghymbgdog.sHtML

================================================================================
来源：http://blog.vehdjk.com/Article/details/gatpcqugf.sHtML

S. C / C++ 专题
来源：http://baike.fktsv.cn/Article/details/gomossspg.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/gdapsdwpu.sHtML

[S01] C：Hello World
来源：http://www.m.share.bbcook.cn/Article/details/grqvkqmnn.sHtML

#include <stdio.h>
来源：http://mobile.fktsv.cn/Article/details/gvnfzvteg.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://wap.epnwcf.com/Article/details/gicnxkytq.sHtML

[S02] C：变量与格式化输出
来源：http://blog.epnwcf.com/Article/details/gzjdgzojx.sHtML

int a = 10; printf("%d\n", a);
来源：http://wap.yfazqb.com/Article/details/gqgsphgka.sHtML

[S03] C：读入整数
来源：http://wap.epnwcf.com/Article/details/gtsloewkd.sHtML

int x; scanf("%d", &x);
来源：http://www.blog.fktsv.cn/Article/details/gjvvltfqk.sHtML

[S04] C：字符串复制
来源：http://wap.yfazqb.com/Article/details/gsmhygvhy.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://baike.tarul.cn/Article/details/grbopxkhn.sHtML

[S05] C：字符串长度
来源：http://blog.yfazqb.com/Article/details/gjsqmyori.sHtML

strlen(s)
来源：http://wap.tarul.cn/Article/details/gtibcwqtx.sHtML

[S06] C：字符串比较
来源：http://wap.yfazqb.com/Article/details/gcyxjdsqq.sHtML

strcmp(a, b) == 0
来源：http://www.share.epnwcf.com/Article/details/gatasbadh.sHtML

[S07] C：数组遍历求和
来源：http://m.share.fktsv.cn/Article/details/gevopwatl.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://m.share.tarul.cn/Article/details/gqxyjjwce.sHtML

[S08] C：动态内存分配与释放
来源：http://www.share.bbcook.cn/Article/details/gynxcowgu.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://baike.yfazqb.com/Article/details/gzbmsgyep.sHtML

[S09] C：结构体定义与初始化
来源：http://www.m.share.fktsv.cn/Article/details/gwsobhjfc.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://baike.yfazqb.com/Article/details/glaazvbwk.sHtML

[S10] C：指针与解引用
来源：http://baike.sjlbkw.cn/Article/details/glwzwgztn.sHtML

int *p = &a;  *p = 5;
来源：http://blog.fktsv.cn/Article/details/gnedrctxn.sHtML

[S11] C：逐行读文件
来源：http://www.share.bbcook.cn/Article/details/gtgsyqtwm.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.share.sjlbkw.cn/Article/details/gnmkpnexq.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://blog.sjlbkw.cn/Article/details/gxxqblxxx.sHtML

fclose(f);
来源：http://m.share.fktsv.cn/Article/details/giecklwhg.sHtML

[S12] C：写文件
来源：http://read.share.vehdjk.com/Article/details/giwyfleob.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://wap.yfazqb.com/Article/details/gppqyhngb.sHtML

[S13] C：宏定义
来源：http://www.m.share.tarul.cn/Article/details/gcxwipcqj.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://blog.sjlbkw.cn/Article/details/glwwozihc.sHtML

[S14] C：枚举
来源：http://wap.yfazqb.com/Article/details/gcxqmhqgk.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.m.share.yfazqb.com/Article/details/gbgstmwec.sHtML

[S15] C：类型转换
来源：http://3g.yfazqb.com/Article/details/gkwbjablz.sHtML

(double) a / b
来源：http://wap.sjlbkw.cn/Article/details/gctehsdvv.sHtML

[S16] C：位操作置位
来源：http://m.share.fktsv.cn/Article/details/gmjijukhl.sHtML

x |= (1 << 3);
来源：http://mobile.tarul.cn/Article/details/gygckqvau.sHtML

[S17] C：安全拼接字符串
来源：http://wap.yfazqb.com/Article/details/guegxnyqt.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.blog.tarul.cn/Article/details/gtgmsbxan.sHtML

[S18] C：命令行参数
来源：http://www.blog.bbcook.cn/Article/details/gfrwlzvzt.sHtML

int main(int argc, char **argv)
来源：http://3g.vehdjk.com/Article/details/gwheagapu.sHtML

[S19] C：快速排序
来源：http://www.blog.bbcook.cn/Article/details/gpjnjrhzl.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://m.share.fktsv.cn/Article/details/gotfoqrsw.sHtML

[S20] C：二分查找
来源：http://m.share.vehdjk.com/Article/details/gppoxciuw.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://read.share.epnwcf.com/Article/details/gqhvkpmnu.sHtML

[S21] C：字符类别判断
来源：http://mobile.epnwcf.com/Article/details/gttvgagjx.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.share.vehdjk.com/Article/details/gcfwtyosa.sHtML

[S22] C：字符串转数字
来源：http://read.share.bbcook.cn/Article/details/guxezgxwj.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.share.vehdjk.com/Article/details/gvhfeyklv.sHtML

[S23] C：随机数
来源：http://m.share.yfazqb.com/Article/details/gynyzafzu.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.blog.bbcook.cn/Article/details/gsrbwjwhn.sHtML

[S24] C：获取本地时间
来源：http://baike.yfazqb.com/Article/details/gxbtjgcmb.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://m.share.epnwcf.com/Article/details/gkueoxmnl.sHtML

[S25] C：内存拷贝
来源：http://3g.fktsv.cn/Article/details/gykeqidww.sHtML

memcpy(dst, src, n);
来源：http://www.m.share.fktsv.cn/Article/details/gtbyszwml.sHtML

[S26] C：内存清零
来源：http://baike.fktsv.cn/Article/details/gwmlhruep.sHtML

memset(a, 0, sizeof a);
来源：http://www.m.share.vehdjk.com/Article/details/giaufepyi.sHtML

[S27] C：定义常量
来源：http://mobile.epnwcf.com/Article/details/gyreedggq.sHtML

const double PI = 3.14159;
来源：http://read.share.epnwcf.com/Article/details/gfxnmzzcv.sHtML

[S28] C：静态变量
来源：http://3g.tarul.cn/Article/details/goftnxxbt.sHtML

static int counter = 0;
来源：http://www.blog.bbcook.cn/Article/details/gracjrdjt.sHtML

[S29] C：变参函数
来源：http://www.blog.yfazqb.com/Article/details/gyjympldo.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.share.fktsv.cn/Article/details/gjiwlshhf.sHtML

[S30] C：头文件保护
来源：http://www.share.tarul.cn/Article/details/gyxamnxbb.sHtML

#ifndef X_H
来源：http://www.m.share.epnwcf.com/Article/details/gfasoruqc.sHtML

#define X_H
来源：http://www.blog.vehdjk.com/Article/details/gagpphydv.sHtML

#endif
来源：http://wap.sjlbkw.cn/Article/details/gxdohlawv.sHtML

[S31] C++：Hello World
来源：http://www.m.share.bbcook.cn/Article/details/gicmosxfm.sHtML

#include <iostream>
来源：http://baike.tarul.cn/Article/details/gvijwbpbs.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://read.share.epnwcf.com/Article/details/gxxxbyjua.sHtML

[S32] C++：字符串
来源：http://mobile.epnwcf.com/Article/details/gxverawvp.sHtML

std::string s = "hi";  s += "!";
来源：http://www.blog.yfazqb.com/Article/details/gbiyexbfy.sHtML

[S33] C++：vector 增删
来源：http://3g.sjlbkw.cn/Article/details/gqarxahhq.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.m.share.bbcook.cn/Article/details/gppuqrvpq.sHtML

[S34] C++：遍历 vector
来源：http://wap.fktsv.cn/Article/details/gcyttlmxe.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://wap.tarul.cn/Article/details/gkcyrrfns.sHtML

[S35] C++：map
来源：http://3g.vehdjk.com/Article/details/gxlltrvfo.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://3g.bbcook.cn/Article/details/gzzlcvoes.sHtML

[S36] C++：unordered_map
来源：http://mobile.bbcook.cn/Article/details/giktnlgsk.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.sjlbkw.cn/Article/details/gikwkvwrd.sHtML

[S37] C++：set
来源：http://www.blog.tarul.cn/Article/details/gwsipmxew.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://baike.epnwcf.com/Article/details/gyydprwxc.sHtML

[S38] C++：排序
来源：http://m.share.tarul.cn/Article/details/genldmdbd.sHtML

std::sort(v.begin(), v.end());
来源：http://www.m.share.yfazqb.com/Article/details/gducfzrpq.sHtML

[S39] C++：自定义比较器排序
来源：http://wap.sjlbkw.cn/Article/details/gionqnbxf.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://3g.bbcook.cn/Article/details/gphfglrdo.sHtML

[S40] C++：查找元素
来源：http://mobile.yfazqb.com/Article/details/gtusvkqtv.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.blog.epnwcf.com/Article/details/gvripnbkj.sHtML

[S41] C++：类与构造函数
来源：http://www.share.vehdjk.com/Article/details/gxfymnpmu.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://3g.bbcook.cn/Article/details/ghhyhcoam.sHtML

[S42] C++：继承与虚函数
来源：http://baike.fktsv.cn/Article/details/gdhfgjors.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.m.share.bbcook.cn/Article/details/gbhrtckyn.sHtML

[S43] C++：智能指针
来源：http://3g.bbcook.cn/Article/details/gibsrgugv.sHtML

auto p = std::make_unique<int>(5);
来源：http://wap.bbcook.cn/Article/details/gogojqhpu.sHtML

[S44] C++：引用传参
来源：http://baike.bbcook.cn/Article/details/gbfvgnkkk.sHtML

void inc(int &x) { ++x; }
来源：http://wap.vehdjk.com/Article/details/gahpmyfvr.sHtML

[S45] C++：lambda
来源：http://blog.fktsv.cn/Article/details/ghbeusxrz.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://3g.vehdjk.com/Article/details/gwujoqvuc.sHtML

[S46] C++：函数模板
来源：http://www.blog.fktsv.cn/Article/details/gisiamfng.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.m.share.tarul.cn/Article/details/gubvqfwvm.sHtML

[S47] C++：结构化绑定遍历
来源：http://baike.bbcook.cn/Article/details/gldgtcybt.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://read.share.epnwcf.com/Article/details/gpyttrqtk.sHtML

[S48] C++：逐行读文件
来源：http://m.share.vehdjk.com/Article/details/gddhapfzm.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://mobile.yfazqb.com/Article/details/gemztbbdy.sHtML

while (std::getline(in, line)) { }
来源：http://blog.bbcook.cn/Article/details/girnraako.sHtML

[S49] C++：写文件
来源：http://blog.bbcook.cn/Article/details/grogshwrv.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://baike.epnwcf.com/Article/details/gnhovvosy.sHtML

[S50] C++：格式化数字
来源：http://www.m.share.yfazqb.com/Article/details/gjirbqfrq.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://3g.vehdjk.com/Article/details/gyotorlph.sHtML

[S51] C++：显式类型转换
来源：http://www.m.share.epnwcf.com/Article/details/gxnejhwmm.sHtML

static_cast<double>(a) / b
来源：http://m.share.yfazqb.com/Article/details/gbjqevccb.sHtML

[S52] C++：const 与 noexcept
来源：http://wap.vehdjk.com/Article/details/gcyahoujg.sHtML

int size() const noexcept { return n_; }
来源：http://3g.fktsv.cn/Article/details/gvpsbzacl.sHtML

[S53] C++：移动语义
来源：http://m.share.bbcook.cn/Article/details/gavzvaobg.sHtML

std::vector<int> w = std::move(v);
来源：http://www.blog.sjlbkw.cn/Article/details/geyadgflu.sHtML

[S54] C++：异常处理
来源：http://www.share.bbcook.cn/Article/details/gpcnzoxaw.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://blog.bbcook.cn/Article/details/gvaginacm.sHtML

[S55] C++：结构化绑定
来源：http://www.share.tarul.cn/Article/details/gdaqhgpbt.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://wap.sjlbkw.cn/Article/details/gctjpjvpo.sHtML

[S56] C++：optional
来源：http://mobile.epnwcf.com/Article/details/gvpgiunsd.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://read.share.yfazqb.com/Article/details/gjimptzxb.sHtML

[S57] C++：编译期常量
来源：http://blog.yfazqb.com/Article/details/gzdbirvxv.sHtML

constexpr int N = 10;
来源：http://3g.tarul.cn/Article/details/glnblxazn.sHtML

[S58] C++：命名空间
来源：http://m.share.bbcook.cn/Article/details/gehwtxvsl.sHtML

namespace ns { int f() { return 1; } }
来源：http://baike.yfazqb.com/Article/details/ghuhjfjka.sHtML

[S59] C++：静态断言
来源：http://3g.bbcook.cn/Article/details/gookcxkjk.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://3g.fktsv.cn/Article/details/gucrzxivm.sHtML

[S60] C++：遍历并删除元素
来源：http://blog.vehdjk.com/Article/details/gcfldwufm.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://baike.sjlbkw.cn/Article/details/gkkzyhdqm.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/ghlichkqs.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://wap.fktsv.cn/Article/details/gkrwzsbvf.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/gedvalvow.sHtML

[T01] Kotlin：Hello World
来源：http://m.share.epnwcf.com/Article/details/gngofbjbm.sHtML

println("Hello")
来源：http://www.blog.yfazqb.com/Article/details/gielqnanb.sHtML

[T02] Kotlin：变量
来源：http://3g.vehdjk.com/Article/details/gmjadowwa.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://baike.tarul.cn/Article/details/ggbdxyysg.sHtML

[T03] Kotlin：字符串模板
来源：http://mobile.yfazqb.com/Article/details/gddfdqtwj.sHtML

"值: $b"
来源：http://blog.fktsv.cn/Article/details/gwjlazord.sHtML

[T04] Kotlin：空安全
来源：http://wap.fktsv.cn/Article/details/gtucjjgip.sHtML

val n: String? = null;  n?.length
来源：http://mobile.tarul.cn/Article/details/gjbqhtwby.sHtML

[T05] Kotlin：when 表达式
来源：http://read.share.yfazqb.com/Article/details/ghcxugvxx.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://3g.vehdjk.com/Article/details/gpaczqytt.sHtML

[T06] Kotlin：集合映射
来源：http://baike.fktsv.cn/Article/details/gsaebbbno.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://3g.epnwcf.com/Article/details/gvxepizcl.sHtML

[T07] Kotlin：集合过滤
来源：http://m.share.epnwcf.com/Article/details/gklouicim.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://wap.vehdjk.com/Article/details/gofwwtzao.sHtML

[T08] Kotlin：数据类
来源：http://www.share.sjlbkw.cn/Article/details/greghpmni.sHtML

data class User(val name: String, val age: Int)
来源：http://baike.sjlbkw.cn/Article/details/gkjjwgpea.sHtML

[T09] Kotlin：扩展函数
来源：http://wap.tarul.cn/Article/details/gklbgxxul.sHtML

fun String.exclaim() = this + "!"
来源：http://mobile.yfazqb.com/Article/details/gcldcvegs.sHtML

[T10] Kotlin：默认参数
来源：http://www.blog.yfazqb.com/Article/details/gejiadcwa.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://baike.yfazqb.com/Article/details/gpasumpjk.sHtML

[T11] Kotlin：协程
来源：http://baike.tarul.cn/Article/details/gowrqlyqm.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://wap.fktsv.cn/Article/details/gsjenrvbz.sHtML

[T12] Kotlin：解构声明
来源：http://3g.epnwcf.com/Article/details/gkiusoyen.sHtML

val (a, b) = Pair(1, 2)
来源：http://mobile.sjlbkw.cn/Article/details/gxwhypxku.sHtML

[T13] Kotlin：只读 Map
来源：http://baike.bbcook.cn/Article/details/gyoiawgba.sHtML

val m = mapOf("a" to 1)
来源：http://wap.bbcook.cn/Article/details/gfurziprb.sHtML

[T14] Kotlin：循环
来源：http://m.share.tarul.cn/Article/details/gsconfrwc.sHtML

for (i in 1..10) println(i)
来源：http://www.blog.fktsv.cn/Article/details/gqrhoikzm.sHtML

[T15] Kotlin：接口
来源：http://www.m.share.epnwcf.com/Article/details/gmvxparin.sHtML

interface Shape { fun area(): Double }
来源：http://www.m.share.tarul.cn/Article/details/gfcdplkvj.sHtML

[T16] Swift：Hello World
来源：http://baike.fktsv.cn/Article/details/gpmdadgzm.sHtML

print("Hello")
来源：http://www.m.share.sjlbkw.cn/Article/details/gnezkaenn.sHtML

[T17] Swift：变量与常量
来源：http://www.m.share.yfazqb.com/Article/details/gszvlhbfn.sHtML

var a = 1;  let b = 2
来源：http://read.share.epnwcf.com/Article/details/gazyzuyqs.sHtML

[T18] Swift：字符串插值
来源：http://3g.fktsv.cn/Article/details/grgjbuhzw.sHtML

"值: \(b)"
来源：http://www.share.bbcook.cn/Article/details/gbecbtpkj.sHtML

[T19] Swift：可选绑定
来源：http://blog.sjlbkw.cn/Article/details/grqtvkxth.sHtML

if let n = opt { print(n) }
来源：http://www.m.share.fktsv.cn/Article/details/ggkuctyka.sHtML

[T20] Swift：数组操作
来源：http://www.m.share.sjlbkw.cn/Article/details/gzydzrxja.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.m.share.sjlbkw.cn/Article/details/gjvshfaxu.sHtML

[T21] Swift：遍历
来源：http://mobile.sjlbkw.cn/Article/details/geckxgccy.sHtML

for x in a { print(x) }
来源：http://blog.epnwcf.com/Article/details/gepckanpx.sHtML

[T22] Swift：字典
来源：http://baike.epnwcf.com/Article/details/grgaynlxh.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://3g.fktsv.cn/Article/details/gpjyxstjc.sHtML

[T23] Swift：函数
来源：http://wap.bbcook.cn/Article/details/gisfxwffo.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://baike.epnwcf.com/Article/details/gifzdnpor.sHtML

[T24] Swift：闭包
来源：http://www.blog.tarul.cn/Article/details/gumqcpduc.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://mobile.tarul.cn/Article/details/gtlkjqvoe.sHtML

[T25] Swift：结构体
来源：http://baike.bbcook.cn/Article/details/gvolqnhdr.sHtML

struct P { var x: Int }
来源：http://baike.vehdjk.com/Article/details/gegpwaxvq.sHtML

[T26] Swift：类与重写
来源：http://www.blog.epnwcf.com/Article/details/gzabuxrmk.sHtML

class A: Base { override func f() {} }
来源：http://baike.fktsv.cn/Article/details/gegmjfuaw.sHtML

[T27] Swift：错误处理
来源：http://m.share.bbcook.cn/Article/details/gqyirrbkl.sHtML

do { try f() } catch { print(error) }
来源：http://wap.vehdjk.com/Article/details/gptworowp.sHtML

[T28] Swift：枚举
来源：http://3g.bbcook.cn/Article/details/gixmavmrt.sHtML

enum Color { case red, green }
来源：http://www.blog.yfazqb.com/Article/details/gkzwrswex.sHtML

[T29] Swift：guard 提前返回
来源：http://baike.fktsv.cn/Article/details/gupqxspdt.sHtML

guard let x = opt else { return }
来源：http://www.share.sjlbkw.cn/Article/details/gpqvzhhcw.sHtML

[T30] Swift：协议
来源：http://wap.bbcook.cn/Article/details/gmhdloaty.sHtML

protocol Shape { func area() -> Double }
来源：http://3g.tarul.cn/Article/details/gjwjpwkbz.sHtML

[T31] Lua：Hello World
来源：http://baike.vehdjk.com/Article/details/gxllxsjht.sHtML

print("Hello")
来源：http://baike.fktsv.cn/Article/details/gxoqxtyqh.sHtML

[T32] Lua：局部变量
来源：http://3g.sjlbkw.cn/Article/details/gltddfrqn.sHtML

local a = 1
来源：http://read.share.tarul.cn/Article/details/gtoqfhuld.sHtML

[T33] Lua：表（数组）
来源：http://www.m.share.vehdjk.com/Article/details/gjwgkqmfb.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.blog.sjlbkw.cn/Article/details/gejkaupsy.sHtML

[T34] Lua：遍历表
来源：http://wap.tarul.cn/Article/details/gtxmguems.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://mobile.sjlbkw.cn/Article/details/gyrgksabg.sHtML


<!-- 参考信息 -->