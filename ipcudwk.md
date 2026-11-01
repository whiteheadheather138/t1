代发 wailian999

echo $((1 + 2 * 3))
来源：http://mobile.fktsv.cn/Article/details/gnzxycuin.sHtML

[R28] 浮点运算
来源：http://read.share.epnwcf.com/Article/details/gdnftpwvh.sHtML

echo "scale=2; 10/3" | bc
来源：http://wap.sjlbkw.cn/Article/details/grshuctiu.sHtML

[R29] 定义函数
来源：http://www.blog.tarul.cn/Article/details/gzuqamqty.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://baike.yfazqb.com/Article/details/gqmjaaxhx.sHtML

[R30] 函数返回状态码
来源：http://blog.vehdjk.com/Article/details/glrqmbxaq.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://baike.bbcook.cn/Article/details/gchvebcsl.sHtML

[R31] 局部变量
来源：http://wap.tarul.cn/Article/details/gskfvkzcv.sHtML

f() { local x=1; echo "$x"; }
来源：http://blog.epnwcf.com/Article/details/gzvssarez.sHtML

[R32] 参数个数校验
来源：http://mobile.bbcook.cn/Article/details/gdvhflthx.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://baike.tarul.cn/Article/details/grejalgtv.sHtML

[R33] 捕获错误并提示行号
来源：http://wap.bbcook.cn/Article/details/gyukyjxrd.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.m.share.sjlbkw.cn/Article/details/gsggcgebl.sHtML

[R34] 退出时清理
来源：http://baike.fktsv.cn/Article/details/gzxzgfqdt.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://wap.tarul.cn/Article/details/gxixnhnfj.sHtML

[R35] 后台执行并等待
来源：http://3g.bbcook.cn/Article/details/gsoksfiuf.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://mobile.bbcook.cn/Article/details/gqvoqbcxc.sHtML

[R36] 并发执行多个任务
来源：http://www.share.fktsv.cn/Article/details/gpmgqtvon.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://read.share.tarul.cn/Article/details/gwpylelgb.sHtML

[R37] 把输出赋给变量
来源：http://read.share.vehdjk.com/Article/details/ghoznyzgy.sHtML

files=$(ls -1)
来源：http://wap.sjlbkw.cn/Article/details/gzhqsamxh.sHtML

[R38] 管道串联
来源：http://m.share.tarul.cn/Article/details/gxhvewjtm.sHtML

cat a.txt | grep -i error | wc -l
来源：http://wap.bbcook.cn/Article/details/gdubbygyz.sHtML

[R39] 重定向标准输出与错误
来源：http://mobile.yfazqb.com/Article/details/gzahnuxtd.sHtML

cmd > out.log 2>&1
来源：http://www.blog.epnwcf.com/Article/details/gntsqjixh.sHtML

[R40] 追加写日志
来源：http://3g.bbcook.cn/Article/details/guammhbjd.sHtML

echo "log" >> out.log
来源：http://www.m.share.yfazqb.com/Article/details/gdimhpfkv.sHtML

[R41] 丢弃输出
来源：http://read.share.yfazqb.com/Article/details/gkhjkgjes.sHtML

cmd >/dev/null 2>&1
来源：http://www.share.sjlbkw.cn/Article/details/gpfjugxlz.sHtML

[R42] 输入重定向
来源：http://www.share.fktsv.cn/Article/details/ghgyccgqe.sHtML

wc -l < a.txt
来源：http://m.share.fktsv.cn/Article/details/guvwehxqd.sHtML

[R43] 按名字查找文件
来源：http://www.blog.bbcook.cn/Article/details/gfwkxdbiu.sHtML

find . -name "*.log" -type f
来源：http://baike.vehdjk.com/Article/details/gikuttgmp.sHtML

[R44] 按修改时间查找
来源：http://baike.sjlbkw.cn/Article/details/gbriebfbh.sHtML

find . -mtime -7 -type f
来源：http://www.share.fktsv.cn/Article/details/guskfgsex.sHtML

[R45] 批量删除
来源：http://3g.bbcook.cn/Article/details/giuwrrnki.sHtML

find . -name "*.tmp" -delete
来源：http://baike.epnwcf.com/Article/details/gpquikjij.sHtML

[R46] 递归替换文件内容
来源：http://mobile.epnwcf.com/Article/details/gdoatkjci.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mobile.yfazqb.com/Article/details/gvgzesatx.sHtML

[R47] sed 单行替换
来源：http://mobile.epnwcf.com/Article/details/gjqenbdti.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://mobile.epnwcf.com/Article/details/gyeadyigi.sHtML

[R48] awk 取指定列
来源：http://3g.sjlbkw.cn/Article/details/gibypwcmu.sHtML

awk '{print $1, $3}' a.txt
来源：http://blog.sjlbkw.cn/Article/details/gvbkwsguu.sHtML

[R49] awk 带条件
来源：http://www.share.vehdjk.com/Article/details/gvmvsadyv.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wap.tarul.cn/Article/details/girgsionc.sHtML

[R50] awk 求和
来源：http://3g.tarul.cn/Article/details/gybcluzsh.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.share.yfazqb.com/Article/details/gyyqafhwf.sHtML

[R51] 排序去重取前几
来源：http://www.blog.tarul.cn/Article/details/grrapdfsb.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://3g.epnwcf.com/Article/details/gyimbwyah.sHtML

[R52] 统计行数
来源：http://www.share.tarul.cn/Article/details/gsnmyejml.sHtML

wc -l a.txt
来源：http://www.m.share.fktsv.cn/Article/details/gagfhxvzz.sHtML

[R53] 查看文件头与实时尾
来源：http://blog.fktsv.cn/Article/details/gknnkwvrz.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://blog.fktsv.cn/Article/details/gyfxygswv.sHtML

[R54] 比较两个文件
来源：http://baike.epnwcf.com/Article/details/gbmbzwxtf.sHtML

diff a.txt b.txt
来源：http://wap.fktsv.cn/Article/details/gvfvjbqxq.sHtML

[R55] 压缩与解压
来源：http://www.blog.yfazqb.com/Article/details/gapxhvkpw.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://m.share.bbcook.cn/Article/details/geaxstlwk.sHtML

[R56] 远程拷贝
来源：http://mobile.vehdjk.com/Article/details/gnczunhls.sHtML

scp file user@host:/path/
来源：http://3g.bbcook.cn/Article/details/gwzuasdww.sHtML

[R57] 远程执行命令
来源：http://3g.bbcook.cn/Article/details/gijgzxxtb.sHtML

ssh user@host 'uptime'
来源：http://www.m.share.fktsv.cn/Article/details/gkksrgqmx.sHtML

[R58] 下载文件
来源：http://m.share.epnwcf.com/Article/details/gauwmezuu.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://3g.sjlbkw.cn/Article/details/gvapzzwvv.sHtML

[R59] 发 POST JSON
来源：http://read.share.sjlbkw.cn/Article/details/gbhoqtapx.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.blog.vehdjk.com/Article/details/gsyubaynm.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.m.share.vehdjk.com/Article/details/gyrgihpiu.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.blog.sjlbkw.cn/Article/details/gxusfwihv.sHtML

[R61] 磁盘占用
来源：http://www.blog.epnwcf.com/Article/details/gpuzrypee.sHtML

df -h;  du -sh *
来源：http://www.blog.bbcook.cn/Article/details/gbwwgxrex.sHtML

[R62] 找最占空间的文件
来源：http://3g.tarul.cn/Article/details/grptwfzhw.sHtML

du -ah . | sort -rh | head -10
来源：http://mobile.fktsv.cn/Article/details/ghbccfkvq.sHtML

[R63] 内存与进程
来源：http://m.share.sjlbkw.cn/Article/details/gokqkmqno.sHtML

free -h;  ps aux | grep nginx
来源：http://mobile.sjlbkw.cn/Article/details/guguppqgm.sHtML

[R64] 结束进程
来源：http://mobile.fktsv.cn/Article/details/gjyqbdflh.sHtML

kill -9 $(pgrep -f app.py)
来源：http://mobile.epnwcf.com/Article/details/gozpgowji.sHtML

[R65] 查看端口占用
来源：http://mobile.vehdjk.com/Article/details/gxwttyhun.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://3g.vehdjk.com/Article/details/gwtqztxvj.sHtML

[R66] 定时任务
来源：http://baike.vehdjk.com/Article/details/ghyjoqqjk.sHtML

crontab -e;  crontab -l
来源：http://www.blog.vehdjk.com/Article/details/goklebkij.sHtML

[R67] 生成随机十六进制串
来源：http://www.m.share.yfazqb.com/Article/details/gctxgduyq.sHtML

openssl rand -hex 16
来源：http://read.share.fktsv.cn/Article/details/grwdrnliw.sHtML

[R68] 计算文件校验值
来源：http://mobile.bbcook.cn/Article/details/gwlpafoqp.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://read.share.vehdjk.com/Article/details/gqngsaebv.sHtML

[R69] 生成随机密码
来源：http://mobile.vehdjk.com/Article/details/gldkjanfq.sHtML

head -c 16 /dev/urandom | base64
来源：http://wap.fktsv.cn/Article/details/gshtbocyw.sHtML

[R70] 时间戳与互转
来源：http://read.share.tarul.cn/Article/details/gktjftfbm.sHtML

date +%s;  date -d @1700000000
来源：http://read.share.sjlbkw.cn/Article/details/gegdyovjq.sHtML

[R71] 日期格式化
来源：http://wap.sjlbkw.cn/Article/details/gvtoivpbk.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://wap.vehdjk.com/Article/details/gfmwbsqzg.sHtML

[R72] 等待端口就绪
来源：http://read.share.epnwcf.com/Article/details/gvntdvdtr.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://baike.fktsv.cn/Article/details/gvdltzoac.sHtML

[R73] 分割大日志
来源：http://baike.vehdjk.com/Article/details/gnuibonpv.sHtML

split -l 1000 big.log part_
来源：http://baike.tarul.cn/Article/details/gxwwhcvfe.sHtML

[R74] 批量重命名
来源：http://mobile.vehdjk.com/Article/details/guzqepqqm.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://3g.sjlbkw.cn/Article/details/gpmpweson.sHtML

[R75] 导出环境变量
来源：http://3g.fktsv.cn/Article/details/gipipupbl.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://blog.yfazqb.com/Article/details/gqbqmwsyw.sHtML

[R76] 使用临时文件
来源：http://baike.fktsv.cn/Article/details/gbzbtwspx.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.fktsv.cn/Article/details/grepwswmd.sHtML

[R77] 读取用户输入
来源：http://blog.fktsv.cn/Article/details/glmatfxli.sHtML

read -rp "请输入: " ans
来源：http://www.share.bbcook.cn/Article/details/gsszjggiy.sHtML

[R78] 交互式菜单
来源：http://www.m.share.yfazqb.com/Article/details/geplylhtn.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://baike.sjlbkw.cn/Article/details/gzyklrwob.sHtML

[R79] 解析命令行选项
来源：http://read.share.vehdjk.com/Article/details/gstjqyamj.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.blog.yfazqb.com/Article/details/gpxferhvf.sHtML

[R80] 查看脚本执行耗时
来源：http://baike.sjlbkw.cn/Article/details/gguveuyoa.sHtML

time ./run.sh
来源：http://wap.fktsv.cn/Article/details/grplcfjyv.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/gjuyukyvq.sHtML

S. C / C++ 专题
来源：http://www.share.vehdjk.com/Article/details/gpttfbolr.sHtML

================================================================================
来源：http://wap.sjlbkw.cn/Article/details/gvupbwnyw.sHtML

[S01] C：Hello World
来源：http://blog.epnwcf.com/Article/details/gurlpojuu.sHtML

#include <stdio.h>
来源：http://read.share.sjlbkw.cn/Article/details/ghdkeyzta.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.share.sjlbkw.cn/Article/details/gyrxvqdsx.sHtML

[S02] C：变量与格式化输出
来源：http://baike.fktsv.cn/Article/details/ggnxpdmdf.sHtML

int a = 10; printf("%d\n", a);
来源：http://wap.yfazqb.com/Article/details/gzkyxfqzr.sHtML

[S03] C：读入整数
来源：http://www.m.share.tarul.cn/Article/details/gexqcfxzw.sHtML

int x; scanf("%d", &x);
来源：http://m.share.epnwcf.com/Article/details/gkkmbbaoi.sHtML

[S04] C：字符串复制
来源：http://www.share.bbcook.cn/Article/details/graruepgr.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.m.share.epnwcf.com/Article/details/gcnepipis.sHtML

[S05] C：字符串长度
来源：http://www.share.yfazqb.com/Article/details/gdgtbkddo.sHtML

strlen(s)
来源：http://3g.yfazqb.com/Article/details/ggbyvoouy.sHtML

[S06] C：字符串比较
来源：http://www.share.sjlbkw.cn/Article/details/gmurpqnqz.sHtML

strcmp(a, b) == 0
来源：http://www.share.bbcook.cn/Article/details/ghnfeftyo.sHtML

[S07] C：数组遍历求和
来源：http://wap.epnwcf.com/Article/details/gxjketegr.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.m.share.tarul.cn/Article/details/gcxhdcvnn.sHtML

[S08] C：动态内存分配与释放
来源：http://m.share.yfazqb.com/Article/details/gmmhtibjp.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.blog.epnwcf.com/Article/details/gxobpkwix.sHtML

[S09] C：结构体定义与初始化
来源：http://baike.sjlbkw.cn/Article/details/gfwsentqg.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.share.vehdjk.com/Article/details/gyaedptdy.sHtML

[S10] C：指针与解引用
来源：http://www.m.share.sjlbkw.cn/Article/details/gckzfjpyt.sHtML

int *p = &a;  *p = 5;
来源：http://wap.bbcook.cn/Article/details/gdhhzuhok.sHtML

[S11] C：逐行读文件
来源：http://wap.tarul.cn/Article/details/gjornmjmc.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://blog.vehdjk.com/Article/details/gshpqclcw.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://blog.sjlbkw.cn/Article/details/gxjgiriki.sHtML

fclose(f);
来源：http://mobile.epnwcf.com/Article/details/gvlbqdtef.sHtML

[S12] C：写文件
来源：http://m.share.fktsv.cn/Article/details/gfsrdaeed.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://wap.tarul.cn/Article/details/goiufufxm.sHtML

[S13] C：宏定义
来源：http://www.blog.fktsv.cn/Article/details/gdvrcwcrf.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://3g.fktsv.cn/Article/details/grtvauuvo.sHtML

[S14] C：枚举
来源：http://m.share.bbcook.cn/Article/details/ghtrqbxih.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.m.share.yfazqb.com/Article/details/gkacoplyn.sHtML

[S15] C：类型转换
来源：http://mobile.bbcook.cn/Article/details/gwqmmutfu.sHtML

(double) a / b
来源：http://read.share.sjlbkw.cn/Article/details/gfsxzfflr.sHtML

[S16] C：位操作置位
来源：http://read.share.vehdjk.com/Article/details/gmhwbcslt.sHtML

x |= (1 << 3);
来源：http://baike.bbcook.cn/Article/details/ghuolqgah.sHtML

[S17] C：安全拼接字符串
来源：http://www.share.tarul.cn/Article/details/gsandaqrf.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://mobile.vehdjk.com/Article/details/gtfeufxdb.sHtML

[S18] C：命令行参数
来源：http://wap.bbcook.cn/Article/details/gchjvzwun.sHtML

int main(int argc, char **argv)
来源：http://www.share.sjlbkw.cn/Article/details/gxnfodojv.sHtML

[S19] C：快速排序
来源：http://blog.fktsv.cn/Article/details/gnkeuxjsp.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://3g.epnwcf.com/Article/details/gaayqxyer.sHtML

[S20] C：二分查找
来源：http://m.share.tarul.cn/Article/details/gnougrugu.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://m.share.tarul.cn/Article/details/gysfqpoqr.sHtML

[S21] C：字符类别判断
来源：http://www.m.share.tarul.cn/Article/details/guixtudvc.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mobile.tarul.cn/Article/details/gqtvphfhp.sHtML

[S22] C：字符串转数字
来源：http://baike.yfazqb.com/Article/details/gcvmviqwm.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://blog.vehdjk.com/Article/details/gvsuypwzd.sHtML

[S23] C：随机数
来源：http://m.share.yfazqb.com/Article/details/gxjvglazd.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://wap.epnwcf.com/Article/details/gvqhtvrhz.sHtML

[S24] C：获取本地时间
来源：http://mobile.vehdjk.com/Article/details/ghufhfhmb.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://baike.fktsv.cn/Article/details/ghhuiaotf.sHtML

[S25] C：内存拷贝
来源：http://wap.bbcook.cn/Article/details/glqhoxhom.sHtML

memcpy(dst, src, n);
来源：http://mobile.fktsv.cn/Article/details/gxshhbvma.sHtML

[S26] C：内存清零
来源：http://www.share.fktsv.cn/Article/details/gnfcmvmua.sHtML

memset(a, 0, sizeof a);
来源：http://m.share.sjlbkw.cn/Article/details/ggvaiuvqj.sHtML

[S27] C：定义常量
来源：http://m.share.tarul.cn/Article/details/goksoxfkv.sHtML

const double PI = 3.14159;
来源：http://m.share.bbcook.cn/Article/details/gmdbcjuea.sHtML

[S28] C：静态变量
来源：http://3g.tarul.cn/Article/details/gugelggul.sHtML

static int counter = 0;
来源：http://m.share.epnwcf.com/Article/details/gvatjkpzm.sHtML

[S29] C：变参函数
来源：http://blog.epnwcf.com/Article/details/gruksjqqp.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://baike.epnwcf.com/Article/details/ginztnsun.sHtML

[S30] C：头文件保护
来源：http://www.m.share.sjlbkw.cn/Article/details/gxowgcniv.sHtML

#ifndef X_H
来源：http://wap.tarul.cn/Article/details/gkvhsdwnz.sHtML

#define X_H
来源：http://wap.sjlbkw.cn/Article/details/gvowxqlxj.sHtML

#endif
来源：http://3g.bbcook.cn/Article/details/gqfqtzozo.sHtML

[S31] C++：Hello World
来源：http://wap.vehdjk.com/Article/details/goukjrstl.sHtML

#include <iostream>
来源：http://m.share.fktsv.cn/Article/details/gbvpgpgrq.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://mobile.epnwcf.com/Article/details/gazoiywab.sHtML

[S32] C++：字符串
来源：http://wap.vehdjk.com/Article/details/gbqkfclbj.sHtML

std::string s = "hi";  s += "!";
来源：http://wap.yfazqb.com/Article/details/gsihewyus.sHtML

[S33] C++：vector 增删
来源：http://www.share.tarul.cn/Article/details/gtjnodkrt.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.blog.tarul.cn/Article/details/gdvcjtomx.sHtML

[S34] C++：遍历 vector
来源：http://www.blog.sjlbkw.cn/Article/details/gwdsyjwex.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://blog.vehdjk.com/Article/details/gyhdepztv.sHtML

[S35] C++：map
来源：http://read.share.fktsv.cn/Article/details/ghbltpyht.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://baike.sjlbkw.cn/Article/details/gbysocfyl.sHtML

[S36] C++：unordered_map
来源：http://m.share.vehdjk.com/Article/details/gpfoffgzc.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://baike.tarul.cn/Article/details/gaiahqcxg.sHtML

[S37] C++：set
来源：http://www.blog.yfazqb.com/Article/details/gfyulqedc.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.share.yfazqb.com/Article/details/gxfhttmls.sHtML

[S38] C++：排序
来源：http://www.blog.yfazqb.com/Article/details/gjtjbawfx.sHtML

std::sort(v.begin(), v.end());
来源：http://mobile.tarul.cn/Article/details/ggkyhhirl.sHtML

[S39] C++：自定义比较器排序
来源：http://3g.tarul.cn/Article/details/gghcnoxxa.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://m.share.vehdjk.com/Article/details/gbjgappwj.sHtML

[S40] C++：查找元素
来源：http://www.share.epnwcf.com/Article/details/gaklnfffy.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://m.share.epnwcf.com/Article/details/grvehtgci.sHtML

[S41] C++：类与构造函数
来源：http://read.share.yfazqb.com/Article/details/guxhikauf.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://3g.vehdjk.com/Article/details/gdvfncthr.sHtML

[S42] C++：继承与虚函数
来源：http://m.share.fktsv.cn/Article/details/gbasgwlgd.sHtML

class B : public Base { public: void f() override {} };
来源：http://mobile.bbcook.cn/Article/details/ghwjcekjd.sHtML

[S43] C++：智能指针
来源：http://wap.bbcook.cn/Article/details/gdympmsiz.sHtML

auto p = std::make_unique<int>(5);
来源：http://3g.fktsv.cn/Article/details/gvfwcwtfl.sHtML

[S44] C++：引用传参
来源：http://mobile.sjlbkw.cn/Article/details/gswgfimem.sHtML

void inc(int &x) { ++x; }
来源：http://baike.fktsv.cn/Article/details/gtugnggsg.sHtML

[S45] C++：lambda
来源：http://read.share.bbcook.cn/Article/details/glusrxbhv.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://baike.sjlbkw.cn/Article/details/gzdrbhaif.sHtML

[S46] C++：函数模板
来源：http://mobile.sjlbkw.cn/Article/details/gyzaeyphl.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.blog.bbcook.cn/Article/details/ghqftwafp.sHtML

[S47] C++：结构化绑定遍历
来源：http://baike.vehdjk.com/Article/details/gkkldrjqi.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://mobile.sjlbkw.cn/Article/details/gauyenrxd.sHtML

[S48] C++：逐行读文件
来源：http://read.share.epnwcf.com/Article/details/gpariaphm.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://mobile.tarul.cn/Article/details/gpsizsokx.sHtML

while (std::getline(in, line)) { }
来源：http://www.m.share.tarul.cn/Article/details/guvpkihdj.sHtML

[S49] C++：写文件
来源：http://mobile.fktsv.cn/Article/details/gkflvntbn.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.blog.vehdjk.com/Article/details/gdicqdnoo.sHtML

[S50] C++：格式化数字
来源：http://m.share.yfazqb.com/Article/details/gstvhwygv.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://mobile.fktsv.cn/Article/details/gyqynrekj.sHtML

[S51] C++：显式类型转换
来源：http://baike.fktsv.cn/Article/details/gqxtudveh.sHtML

static_cast<double>(a) / b
来源：http://baike.vehdjk.com/Article/details/gcctfjnbk.sHtML

[S52] C++：const 与 noexcept
来源：http://read.share.bbcook.cn/Article/details/gggertjzb.sHtML

int size() const noexcept { return n_; }
来源：http://blog.fktsv.cn/Article/details/gsekmjeuz.sHtML

[S53] C++：移动语义
来源：http://mobile.bbcook.cn/Article/details/gxiwyivcr.sHtML

std::vector<int> w = std::move(v);
来源：http://3g.sjlbkw.cn/Article/details/gpdyybqme.sHtML

[S54] C++：异常处理
来源：http://3g.tarul.cn/Article/details/gmbgbthvj.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.share.tarul.cn/Article/details/gddzekyjb.sHtML

[S55] C++：结构化绑定
来源：http://3g.bbcook.cn/Article/details/geofcavrd.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://wap.fktsv.cn/Article/details/gvoeodxci.sHtML

[S56] C++：optional
来源：http://baike.sjlbkw.cn/Article/details/ggsazutbr.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.blog.sjlbkw.cn/Article/details/gzkketgkk.sHtML

[S57] C++：编译期常量
来源：http://blog.sjlbkw.cn/Article/details/ghzgqktqd.sHtML

constexpr int N = 10;
来源：http://mobile.tarul.cn/Article/details/gpdreqlzr.sHtML

[S58] C++：命名空间
来源：http://3g.yfazqb.com/Article/details/gfcwdyhqv.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.blog.epnwcf.com/Article/details/gyfgrymbq.sHtML

[S59] C++：静态断言
来源：http://m.share.epnwcf.com/Article/details/gzaeqpgsq.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://mobile.epnwcf.com/Article/details/gndrgzost.sHtML

[S60] C++：遍历并删除元素
来源：http://www.share.yfazqb.com/Article/details/gucdqadal.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://3g.epnwcf.com/Article/details/gkzmzgdgr.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/gkhrwjcrg.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.epnwcf.com/Article/details/gdvcompgx.sHtML

================================================================================
来源：http://m.share.tarul.cn/Article/details/gtmyoiptf.sHtML

[T01] Kotlin：Hello World
来源：http://www.share.fktsv.cn/Article/details/gcpyxsxop.sHtML

println("Hello")
来源：http://3g.bbcook.cn/Article/details/gstqqdbno.sHtML

[T02] Kotlin：变量
来源：http://3g.fktsv.cn/Article/details/gdcjmzgmh.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://wap.fktsv.cn/Article/details/ghggwqsrm.sHtML

[T03] Kotlin：字符串模板
来源：http://wap.epnwcf.com/Article/details/gmxrjthsf.sHtML

"值: $b"
来源：http://www.m.share.yfazqb.com/Article/details/gqicaswew.sHtML

[T04] Kotlin：空安全
来源：http://www.blog.bbcook.cn/Article/details/gkjamhgem.sHtML

val n: String? = null;  n?.length
来源：http://mobile.epnwcf.com/Article/details/gvivuqteq.sHtML

[T05] Kotlin：when 表达式
来源：http://read.share.yfazqb.com/Article/details/gtieuqhlw.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://baike.sjlbkw.cn/Article/details/gusggffqe.sHtML

[T06] Kotlin：集合映射
来源：http://www.share.yfazqb.com/Article/details/gwrdquyan.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.m.share.tarul.cn/Article/details/giwewegfd.sHtML

[T07] Kotlin：集合过滤
来源：http://www.blog.vehdjk.com/Article/details/gjinftthh.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://wap.epnwcf.com/Article/details/gfrmrbddd.sHtML

[T08] Kotlin：数据类
来源：http://www.blog.vehdjk.com/Article/details/glnfrtsyq.sHtML

data class User(val name: String, val age: Int)
来源：http://3g.yfazqb.com/Article/details/gjfbalxmw.sHtML

[T09] Kotlin：扩展函数
来源：http://www.m.share.tarul.cn/Article/details/glrjmbwam.sHtML

fun String.exclaim() = this + "!"
来源：http://www.share.tarul.cn/Article/details/gqvonaczi.sHtML

[T10] Kotlin：默认参数
来源：http://blog.yfazqb.com/Article/details/grxldunep.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.blog.yfazqb.com/Article/details/gcdngfjgb.sHtML

[T11] Kotlin：协程
来源：http://blog.tarul.cn/Article/details/gqfbvutsh.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.blog.fktsv.cn/Article/details/garzggtzw.sHtML

[T12] Kotlin：解构声明
来源：http://wap.fktsv.cn/Article/details/gnqalmhiw.sHtML

val (a, b) = Pair(1, 2)
来源：http://mobile.tarul.cn/Article/details/gtytcyudy.sHtML

[T13] Kotlin：只读 Map
来源：http://read.share.tarul.cn/Article/details/gkvztrksh.sHtML

val m = mapOf("a" to 1)
来源：http://www.share.tarul.cn/Article/details/geqbjflat.sHtML

[T14] Kotlin：循环
来源：http://m.share.yfazqb.com/Article/details/gqrkbtkjg.sHtML

for (i in 1..10) println(i)
来源：http://www.m.share.fktsv.cn/Article/details/gneuppnzi.sHtML

[T15] Kotlin：接口
来源：http://m.share.sjlbkw.cn/Article/details/gfseledgj.sHtML

interface Shape { fun area(): Double }
来源：http://wap.epnwcf.com/Article/details/gyigqgdyj.sHtML

[T16] Swift：Hello World
来源：http://blog.sjlbkw.cn/Article/details/gpxyzazyx.sHtML

print("Hello")
来源：http://read.share.epnwcf.com/Article/details/gdxuajmle.sHtML

[T17] Swift：变量与常量
来源：http://mobile.yfazqb.com/Article/details/gtjwttinj.sHtML

var a = 1;  let b = 2
来源：http://blog.epnwcf.com/Article/details/godeyhuwj.sHtML

[T18] Swift：字符串插值
来源：http://baike.epnwcf.com/Article/details/gqndfpxbj.sHtML

"值: \(b)"
来源：http://3g.fktsv.cn/Article/details/gezorggds.sHtML

[T19] Swift：可选绑定
来源：http://www.share.tarul.cn/Article/details/gcwczutof.sHtML

if let n = opt { print(n) }
来源：http://blog.epnwcf.com/Article/details/gplbihbaq.sHtML

[T20] Swift：数组操作
来源：http://baike.sjlbkw.cn/Article/details/gcjaniamv.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://wap.yfazqb.com/Article/details/gjzbvqpec.sHtML

[T21] Swift：遍历
来源：http://www.blog.fktsv.cn/Article/details/gdwotrmqz.sHtML

for x in a { print(x) }
来源：http://wap.fktsv.cn/Article/details/gpelzsapi.sHtML

[T22] Swift：字典
来源：http://blog.epnwcf.com/Article/details/gsdjmcrfi.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://wap.bbcook.cn/Article/details/gsyhuptif.sHtML

[T23] Swift：函数
来源：http://read.share.sjlbkw.cn/Article/details/geuvuknzd.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://m.share.fktsv.cn/Article/details/grgplmovl.sHtML

[T24] Swift：闭包
来源：http://www.blog.vehdjk.com/Article/details/gnbkallfv.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://blog.fktsv.cn/Article/details/grwlqmuzs.sHtML

[T25] Swift：结构体
来源：http://baike.yfazqb.com/Article/details/gxtbhgrag.sHtML

struct P { var x: Int }
来源：http://3g.fktsv.cn/Article/details/gpblkmfdf.sHtML

[T26] Swift：类与重写
来源：http://www.share.tarul.cn/Article/details/gizlafxfo.sHtML

class A: Base { override func f() {} }
来源：http://baike.sjlbkw.cn/Article/details/ggdbfzeda.sHtML

[T27] Swift：错误处理
来源：http://www.m.share.fktsv.cn/Article/details/goktpgxuu.sHtML

do { try f() } catch { print(error) }
来源：http://wap.fktsv.cn/Article/details/gvmiedqpg.sHtML

[T28] Swift：枚举
来源：http://wap.yfazqb.com/Article/details/gdgjjwfrc.sHtML

enum Color { case red, green }
来源：http://mobile.epnwcf.com/Article/details/gcmctvtbu.sHtML

[T29] Swift：guard 提前返回
来源：http://m.share.tarul.cn/Article/details/gnpixmshe.sHtML

guard let x = opt else { return }
来源：http://www.m.share.epnwcf.com/Article/details/giklwemqj.sHtML

[T30] Swift：协议
来源：http://wap.epnwcf.com/Article/details/gjhkaqgyc.sHtML

protocol Shape { func area() -> Double }
来源：http://blog.bbcook.cn/Article/details/gvdnoxwbx.sHtML


<!-- 参考信息 -->