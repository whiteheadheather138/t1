代发 wailian999

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.blog.sjlbkw.cn/Article/details/gznhfabsb.sHtML

[R24] 大小写转换
来源：http://blog.yfazqb.com/Article/details/glocawdjk.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.m.share.epnwcf.com/Article/details/gyyjknxlk.sHtML

[R25] 去后缀 / 去前缀
来源：http://baike.yfazqb.com/Article/details/grgmqekrh.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://mobile.yfazqb.com/Article/details/gbhsztvlp.sHtML

[R26] 命令替换
来源：http://www.share.fktsv.cn/Article/details/giysjalvs.sHtML

now=$(date +%F); echo "$now"
来源：http://mobile.sjlbkw.cn/Article/details/gtoxidpyc.sHtML

[R27] 算术展开
来源：http://baike.sjlbkw.cn/Article/details/gqxndtgsz.sHtML

echo $((1 + 2 * 3))
来源：http://3g.yfazqb.com/Article/details/gcprgswnx.sHtML

[R28] 浮点运算
来源：http://mobile.fktsv.cn/Article/details/gyqetpcmf.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.blog.vehdjk.com/Article/details/gwsmzkinb.sHtML

[R29] 定义函数
来源：http://www.blog.fktsv.cn/Article/details/ggtxuwhzd.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.share.epnwcf.com/Article/details/gssthwerm.sHtML

[R30] 函数返回状态码
来源：http://www.share.sjlbkw.cn/Article/details/giapaztkx.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.share.yfazqb.com/Article/details/grqxtjtnq.sHtML

[R31] 局部变量
来源：http://www.share.epnwcf.com/Article/details/gpcsduepb.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.blog.fktsv.cn/Article/details/gubnrjzdy.sHtML

[R32] 参数个数校验
来源：http://www.m.share.bbcook.cn/Article/details/gifdinpna.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.m.share.vehdjk.com/Article/details/gylunonix.sHtML

[R33] 捕获错误并提示行号
来源：http://www.blog.sjlbkw.cn/Article/details/gcbbtjpwv.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.share.yfazqb.com/Article/details/gtwzcexwg.sHtML

[R34] 退出时清理
来源：http://baike.fktsv.cn/Article/details/glcnwhqqi.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.yfazqb.com/Article/details/grqgxrwbw.sHtML

[R35] 后台执行并等待
来源：http://www.blog.vehdjk.com/Article/details/ghgbosmko.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://m.share.fktsv.cn/Article/details/gfriurcmw.sHtML

[R36] 并发执行多个任务
来源：http://blog.epnwcf.com/Article/details/gdpgaxjdd.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.share.epnwcf.com/Article/details/gwfxjnnkf.sHtML

[R37] 把输出赋给变量
来源：http://wap.sjlbkw.cn/Article/details/gvmmrysgp.sHtML

files=$(ls -1)
来源：http://baike.epnwcf.com/Article/details/gvfbxwmyy.sHtML

[R38] 管道串联
来源：http://www.m.share.fktsv.cn/Article/details/gwwnqqvpq.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.blog.yfazqb.com/Article/details/gkkfqubzk.sHtML

[R39] 重定向标准输出与错误
来源：http://www.share.fktsv.cn/Article/details/gbeamiuht.sHtML

cmd > out.log 2>&1
来源：http://www.blog.bbcook.cn/Article/details/gwvdknefr.sHtML

[R40] 追加写日志
来源：http://www.blog.fktsv.cn/Article/details/gbpaghxtd.sHtML

echo "log" >> out.log
来源：http://mobile.tarul.cn/Article/details/gpwurvgap.sHtML

[R41] 丢弃输出
来源：http://read.share.tarul.cn/Article/details/gvyqnqefz.sHtML

cmd >/dev/null 2>&1
来源：http://read.share.tarul.cn/Article/details/gyurmghqx.sHtML

[R42] 输入重定向
来源：http://baike.yfazqb.com/Article/details/gnsfldtku.sHtML

wc -l < a.txt
来源：http://www.share.fktsv.cn/Article/details/gcwuqsmjk.sHtML

[R43] 按名字查找文件
来源：http://www.blog.fktsv.cn/Article/details/gdloeakrk.sHtML

find . -name "*.log" -type f
来源：http://baike.vehdjk.com/Article/details/gmwovzyvk.sHtML

[R44] 按修改时间查找
来源：http://baike.yfazqb.com/Article/details/gwfzjvsaa.sHtML

find . -mtime -7 -type f
来源：http://www.m.share.vehdjk.com/Article/details/ggbpdbwdy.sHtML

[R45] 批量删除
来源：http://baike.sjlbkw.cn/Article/details/gsicddmsb.sHtML

find . -name "*.tmp" -delete
来源：http://wap.sjlbkw.cn/Article/details/gsjrzhdfy.sHtML

[R46] 递归替换文件内容
来源：http://www.share.epnwcf.com/Article/details/ghtknvngh.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://3g.tarul.cn/Article/details/gltikjdtq.sHtML

[R47] sed 单行替换
来源：http://read.share.sjlbkw.cn/Article/details/gtntvzkmn.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.share.epnwcf.com/Article/details/gvlyfueou.sHtML

[R48] awk 取指定列
来源：http://www.blog.epnwcf.com/Article/details/gvsmowxro.sHtML

awk '{print $1, $3}' a.txt
来源：http://blog.epnwcf.com/Article/details/gvsalwihj.sHtML

[R49] awk 带条件
来源：http://read.share.fktsv.cn/Article/details/gqtjnjoss.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://3g.epnwcf.com/Article/details/gqspeogni.sHtML

[R50] awk 求和
来源：http://blog.epnwcf.com/Article/details/gtwdkstwu.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://read.share.vehdjk.com/Article/details/genkrmati.sHtML

[R51] 排序去重取前几
来源：http://www.share.epnwcf.com/Article/details/gsxqdzvqt.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.share.vehdjk.com/Article/details/gfrevygop.sHtML

[R52] 统计行数
来源：http://3g.yfazqb.com/Article/details/gsyhmutqt.sHtML

wc -l a.txt
来源：http://read.share.tarul.cn/Article/details/gfragsohl.sHtML

[R53] 查看文件头与实时尾
来源：http://blog.tarul.cn/Article/details/geprtqqaz.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://blog.epnwcf.com/Article/details/grygrcvfm.sHtML

[R54] 比较两个文件
来源：http://3g.bbcook.cn/Article/details/gmrbblxrp.sHtML

diff a.txt b.txt
来源：http://blog.vehdjk.com/Article/details/geuagawgl.sHtML

[R55] 压缩与解压
来源：http://wap.yfazqb.com/Article/details/gvrodraac.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://m.share.yfazqb.com/Article/details/gtkycjthj.sHtML

[R56] 远程拷贝
来源：http://wap.yfazqb.com/Article/details/gwfmsyrak.sHtML

scp file user@host:/path/
来源：http://m.share.tarul.cn/Article/details/gfacnyuyt.sHtML

[R57] 远程执行命令
来源：http://wap.fktsv.cn/Article/details/gzeipaavb.sHtML

ssh user@host 'uptime'
来源：http://blog.sjlbkw.cn/Article/details/gcfocyuvw.sHtML

[R58] 下载文件
来源：http://3g.yfazqb.com/Article/details/gcrulmrxy.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://read.share.tarul.cn/Article/details/gscgsoukf.sHtML

[R59] 发 POST JSON
来源：http://mobile.sjlbkw.cn/Article/details/ghahqwqrh.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://3g.vehdjk.com/Article/details/gzmagjdrw.sHtML

[R60] 只看 HTTP 状态码
来源：http://m.share.fktsv.cn/Article/details/gkbmrdszx.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://read.share.tarul.cn/Article/details/gyjapzcir.sHtML

[R61] 磁盘占用
来源：http://baike.tarul.cn/Article/details/goeayetqq.sHtML

df -h;  du -sh *
来源：http://www.blog.fktsv.cn/Article/details/gcmaweeqs.sHtML

[R62] 找最占空间的文件
来源：http://wap.fktsv.cn/Article/details/gcaxtbcur.sHtML

du -ah . | sort -rh | head -10
来源：http://www.share.epnwcf.com/Article/details/guiqfzgns.sHtML

[R63] 内存与进程
来源：http://mobile.yfazqb.com/Article/details/gvjkopchg.sHtML

free -h;  ps aux | grep nginx
来源：http://mobile.sjlbkw.cn/Article/details/gjwoaxzpr.sHtML

[R64] 结束进程
来源：http://baike.epnwcf.com/Article/details/grvdqvlfi.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.share.yfazqb.com/Article/details/gmqyjiuea.sHtML

[R65] 查看端口占用
来源：http://www.m.share.fktsv.cn/Article/details/gbdcckgfp.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://blog.yfazqb.com/Article/details/ghyjevqqn.sHtML

[R66] 定时任务
来源：http://wap.vehdjk.com/Article/details/ggseebtpi.sHtML

crontab -e;  crontab -l
来源：http://read.share.epnwcf.com/Article/details/ghflirbrc.sHtML

[R67] 生成随机十六进制串
来源：http://3g.tarul.cn/Article/details/gqzaszyeu.sHtML

openssl rand -hex 16
来源：http://m.share.epnwcf.com/Article/details/gelpmpvle.sHtML

[R68] 计算文件校验值
来源：http://m.share.sjlbkw.cn/Article/details/gxszbeeyu.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.blog.tarul.cn/Article/details/guepescar.sHtML

[R69] 生成随机密码
来源：http://m.share.bbcook.cn/Article/details/gyftjkhcd.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.blog.epnwcf.com/Article/details/gmbxkckmh.sHtML

[R70] 时间戳与互转
来源：http://www.m.share.tarul.cn/Article/details/gmzvnvqut.sHtML

date +%s;  date -d @1700000000
来源：http://www.blog.bbcook.cn/Article/details/gkgufuoec.sHtML

[R71] 日期格式化
来源：http://baike.yfazqb.com/Article/details/gaxdtqchp.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.blog.bbcook.cn/Article/details/glhaqxiwd.sHtML

[R72] 等待端口就绪
来源：http://www.blog.sjlbkw.cn/Article/details/gjhqogfhm.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.share.yfazqb.com/Article/details/gtitnrsnm.sHtML

[R73] 分割大日志
来源：http://wap.fktsv.cn/Article/details/guhbqtbst.sHtML

split -l 1000 big.log part_
来源：http://m.share.fktsv.cn/Article/details/gvyxoldmj.sHtML

[R74] 批量重命名
来源：http://3g.epnwcf.com/Article/details/gvxrbshxx.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://blog.sjlbkw.cn/Article/details/glwwxoovb.sHtML

[R75] 导出环境变量
来源：http://www.share.tarul.cn/Article/details/gqdtqguek.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.blog.fktsv.cn/Article/details/gdcwoxrxr.sHtML

[R76] 使用临时文件
来源：http://blog.fktsv.cn/Article/details/gvrxgaouj.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.tarul.cn/Article/details/gimdvwfrx.sHtML

[R77] 读取用户输入
来源：http://www.blog.vehdjk.com/Article/details/gteaqhzjr.sHtML

read -rp "请输入: " ans
来源：http://3g.tarul.cn/Article/details/gndnrtdmx.sHtML

[R78] 交互式菜单
来源：http://www.share.fktsv.cn/Article/details/gvvxfnclp.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://baike.yfazqb.com/Article/details/gzvmfrpbh.sHtML

[R79] 解析命令行选项
来源：http://m.share.sjlbkw.cn/Article/details/ghfrjjmgt.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://baike.vehdjk.com/Article/details/gjuwroxmz.sHtML

[R80] 查看脚本执行耗时
来源：http://www.share.tarul.cn/Article/details/gvsoeejfv.sHtML

time ./run.sh
来源：http://read.share.yfazqb.com/Article/details/gshckwygd.sHtML

================================================================================
来源：http://wap.sjlbkw.cn/Article/details/gxiysztvz.sHtML

S. C / C++ 专题
来源：http://baike.yfazqb.com/Article/details/glcukgpio.sHtML

================================================================================
来源：http://3g.vehdjk.com/Article/details/gosyaxhnj.sHtML

[S01] C：Hello World
来源：http://mobile.vehdjk.com/Article/details/guilswqrp.sHtML

#include <stdio.h>
来源：http://3g.yfazqb.com/Article/details/guqdwyabi.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://3g.epnwcf.com/Article/details/gfyuzauze.sHtML

[S02] C：变量与格式化输出
来源：http://m.share.vehdjk.com/Article/details/gwtqlxslf.sHtML

int a = 10; printf("%d\n", a);
来源：http://m.share.vehdjk.com/Article/details/gmfhyhadx.sHtML

[S03] C：读入整数
来源：http://www.blog.tarul.cn/Article/details/gyrnvlcut.sHtML

int x; scanf("%d", &x);
来源：http://www.m.share.fktsv.cn/Article/details/gixfhvuri.sHtML

[S04] C：字符串复制
来源：http://baike.epnwcf.com/Article/details/gymvwzoxc.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://wap.bbcook.cn/Article/details/grsqaofgj.sHtML

[S05] C：字符串长度
来源：http://www.m.share.vehdjk.com/Article/details/gtlvetqgh.sHtML

strlen(s)
来源：http://read.share.fktsv.cn/Article/details/ggptsjpnh.sHtML

[S06] C：字符串比较
来源：http://mobile.tarul.cn/Article/details/gtqtxtyos.sHtML

strcmp(a, b) == 0
来源：http://baike.tarul.cn/Article/details/gotlynkyj.sHtML

[S07] C：数组遍历求和
来源：http://www.share.bbcook.cn/Article/details/gxqnmkeyf.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://wap.bbcook.cn/Article/details/gogimtzny.sHtML

[S08] C：动态内存分配与释放
来源：http://blog.epnwcf.com/Article/details/guvaitcyl.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://3g.vehdjk.com/Article/details/gtzmqicvy.sHtML

[S09] C：结构体定义与初始化
来源：http://www.share.vehdjk.com/Article/details/gowqufcht.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://3g.bbcook.cn/Article/details/gbuusjvts.sHtML

[S10] C：指针与解引用
来源：http://www.share.epnwcf.com/Article/details/gejynuonf.sHtML

int *p = &a;  *p = 5;
来源：http://baike.sjlbkw.cn/Article/details/gvpqrrxvf.sHtML

[S11] C：逐行读文件
来源：http://read.share.fktsv.cn/Article/details/gmcvwnlkf.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.m.share.epnwcf.com/Article/details/gckdrqoro.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://3g.sjlbkw.cn/Article/details/gdykgllet.sHtML

fclose(f);
来源：http://www.m.share.epnwcf.com/Article/details/garujqrjm.sHtML

[S12] C：写文件
来源：http://blog.bbcook.cn/Article/details/gahnrzrpu.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://3g.bbcook.cn/Article/details/guxemxrki.sHtML

[S13] C：宏定义
来源：http://read.share.tarul.cn/Article/details/gugdzmpix.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.share.sjlbkw.cn/Article/details/ggkmelxwz.sHtML

[S14] C：枚举
来源：http://wap.tarul.cn/Article/details/gvtnwleqs.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://mobile.vehdjk.com/Article/details/gfhjtnyqn.sHtML

[S15] C：类型转换
来源：http://www.blog.yfazqb.com/Article/details/gfzgwlhkd.sHtML

(double) a / b
来源：http://www.blog.tarul.cn/Article/details/ggxsqitqx.sHtML

[S16] C：位操作置位
来源：http://mobile.sjlbkw.cn/Article/details/gnmxpszch.sHtML

x |= (1 << 3);
来源：http://wap.fktsv.cn/Article/details/gamyjrdfd.sHtML

[S17] C：安全拼接字符串
来源：http://baike.yfazqb.com/Article/details/glntygeph.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.m.share.vehdjk.com/Article/details/guqlfgbzf.sHtML

[S18] C：命令行参数
来源：http://m.share.yfazqb.com/Article/details/gohjzwddl.sHtML

int main(int argc, char **argv)
来源：http://www.blog.bbcook.cn/Article/details/ggkooxpdf.sHtML

[S19] C：快速排序
来源：http://www.blog.fktsv.cn/Article/details/glprkdjtz.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://wap.epnwcf.com/Article/details/gyleljmvx.sHtML

[S20] C：二分查找
来源：http://m.share.bbcook.cn/Article/details/gqloxfoom.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://wap.yfazqb.com/Article/details/gnwqljvok.sHtML

[S21] C：字符类别判断
来源：http://www.blog.sjlbkw.cn/Article/details/goblsunah.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mobile.bbcook.cn/Article/details/gbireolbk.sHtML

[S22] C：字符串转数字
来源：http://www.blog.yfazqb.com/Article/details/gkarfbnxh.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://baike.yfazqb.com/Article/details/gfpgqwbia.sHtML

[S23] C：随机数
来源：http://m.share.vehdjk.com/Article/details/gyfmaucua.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://wap.vehdjk.com/Article/details/gpjruztoq.sHtML

[S24] C：获取本地时间
来源：http://wap.sjlbkw.cn/Article/details/gxjarmwwv.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.m.share.sjlbkw.cn/Article/details/gybxzbfky.sHtML

[S25] C：内存拷贝
来源：http://www.share.vehdjk.com/Article/details/gkxdvjjgf.sHtML

memcpy(dst, src, n);
来源：http://wap.yfazqb.com/Article/details/gepqcfhin.sHtML

[S26] C：内存清零
来源：http://read.share.epnwcf.com/Article/details/garbgkpso.sHtML

memset(a, 0, sizeof a);
来源：http://m.share.vehdjk.com/Article/details/gostcfgav.sHtML

[S27] C：定义常量
来源：http://wap.fktsv.cn/Article/details/grahjworo.sHtML

const double PI = 3.14159;
来源：http://read.share.vehdjk.com/Article/details/gpqqangge.sHtML

[S28] C：静态变量
来源：http://blog.yfazqb.com/Article/details/gxfsrvxpy.sHtML

static int counter = 0;
来源：http://www.share.sjlbkw.cn/Article/details/gdtopnsym.sHtML

[S29] C：变参函数
来源：http://www.blog.tarul.cn/Article/details/gxexxvywd.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://read.share.vehdjk.com/Article/details/gjzlcuoqw.sHtML

[S30] C：头文件保护
来源：http://baike.epnwcf.com/Article/details/gxzevsbfd.sHtML

#ifndef X_H
来源：http://m.share.sjlbkw.cn/Article/details/gnubovzjs.sHtML

#define X_H
来源：http://baike.tarul.cn/Article/details/ghulvxjtv.sHtML

#endif
来源：http://read.share.yfazqb.com/Article/details/gucskepho.sHtML

[S31] C++：Hello World
来源：http://www.share.bbcook.cn/Article/details/gkqpohrht.sHtML

#include <iostream>
来源：http://wap.tarul.cn/Article/details/gsyquliln.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://m.share.fktsv.cn/Article/details/gugwtmlfu.sHtML

[S32] C++：字符串
来源：http://wap.sjlbkw.cn/Article/details/gpnvlvorx.sHtML

std::string s = "hi";  s += "!";
来源：http://www.share.bbcook.cn/Article/details/ghzlpcuac.sHtML

[S33] C++：vector 增删
来源：http://www.blog.epnwcf.com/Article/details/ghblvlmfv.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://m.share.epnwcf.com/Article/details/gszzsoult.sHtML

[S34] C++：遍历 vector
来源：http://read.share.vehdjk.com/Article/details/gsrkhwgjn.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://blog.tarul.cn/Article/details/gjflbyoqo.sHtML

[S35] C++：map
来源：http://www.m.share.yfazqb.com/Article/details/garitohuy.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.fktsv.cn/Article/details/gyqpgnoxs.sHtML

[S36] C++：unordered_map
来源：http://m.share.epnwcf.com/Article/details/gqlhxfkac.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://3g.epnwcf.com/Article/details/gvmvrvuwu.sHtML

[S37] C++：set
来源：http://wap.bbcook.cn/Article/details/grnbsxghg.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.m.share.tarul.cn/Article/details/gompbakih.sHtML

[S38] C++：排序
来源：http://baike.epnwcf.com/Article/details/gnfdpghyl.sHtML

std::sort(v.begin(), v.end());
来源：http://blog.fktsv.cn/Article/details/gamoynust.sHtML

[S39] C++：自定义比较器排序
来源：http://blog.epnwcf.com/Article/details/ghksttygm.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wap.epnwcf.com/Article/details/gaoxurwku.sHtML

[S40] C++：查找元素
来源：http://www.m.share.fktsv.cn/Article/details/guoyffvqz.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://read.share.yfazqb.com/Article/details/grcuhiahl.sHtML

[S41] C++：类与构造函数
来源：http://www.blog.tarul.cn/Article/details/gtmmgbwcu.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://blog.bbcook.cn/Article/details/gaiizbboj.sHtML

[S42] C++：继承与虚函数
来源：http://3g.tarul.cn/Article/details/gsosfkhmx.sHtML

class B : public Base { public: void f() override {} };
来源：http://m.share.vehdjk.com/Article/details/ggcdzfkma.sHtML

[S43] C++：智能指针
来源：http://www.m.share.sjlbkw.cn/Article/details/gxqbexdab.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.blog.sjlbkw.cn/Article/details/gwuoyubys.sHtML

[S44] C++：引用传参
来源：http://m.share.epnwcf.com/Article/details/gvwuzbfdi.sHtML

void inc(int &x) { ++x; }
来源：http://baike.yfazqb.com/Article/details/gkdkraeyd.sHtML

[S45] C++：lambda
来源：http://www.blog.bbcook.cn/Article/details/gwsbkltjn.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://read.share.epnwcf.com/Article/details/gbokwdlmr.sHtML

[S46] C++：函数模板
来源：http://www.share.vehdjk.com/Article/details/gdbbftmei.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://read.share.tarul.cn/Article/details/gdengolhe.sHtML

[S47] C++：结构化绑定遍历
来源：http://wap.epnwcf.com/Article/details/gmovhoazt.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://read.share.fktsv.cn/Article/details/grjexsyer.sHtML

[S48] C++：逐行读文件
来源：http://wap.bbcook.cn/Article/details/gkqrotlwi.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.blog.yfazqb.com/Article/details/gdelcckim.sHtML

while (std::getline(in, line)) { }
来源：http://www.blog.vehdjk.com/Article/details/gfwxdvnpr.sHtML

[S49] C++：写文件
来源：http://3g.yfazqb.com/Article/details/ggeyeyler.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.share.yfazqb.com/Article/details/gopehmbao.sHtML

[S50] C++：格式化数字
来源：http://m.share.sjlbkw.cn/Article/details/gxjcbnuxk.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.m.share.vehdjk.com/Article/details/gcnljmgss.sHtML

[S51] C++：显式类型转换
来源：http://www.blog.tarul.cn/Article/details/gyrbzzdap.sHtML

static_cast<double>(a) / b
来源：http://blog.epnwcf.com/Article/details/glljtrzxy.sHtML

[S52] C++：const 与 noexcept
来源：http://baike.tarul.cn/Article/details/gcghddubn.sHtML

int size() const noexcept { return n_; }
来源：http://www.m.share.fktsv.cn/Article/details/gqrgqmhof.sHtML

[S53] C++：移动语义
来源：http://baike.fktsv.cn/Article/details/ghykwgduv.sHtML

std::vector<int> w = std::move(v);
来源：http://3g.fktsv.cn/Article/details/gfdlodhkv.sHtML

[S54] C++：异常处理
来源：http://3g.bbcook.cn/Article/details/ghiedecbn.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://read.share.vehdjk.com/Article/details/gmwleqqho.sHtML

[S55] C++：结构化绑定
来源：http://blog.epnwcf.com/Article/details/geapbnjlg.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://baike.vehdjk.com/Article/details/gtyxprhvj.sHtML

[S56] C++：optional
来源：http://baike.epnwcf.com/Article/details/gztyiithf.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wap.sjlbkw.cn/Article/details/glmjbzcuv.sHtML

[S57] C++：编译期常量
来源：http://3g.tarul.cn/Article/details/gotdrwktd.sHtML

constexpr int N = 10;
来源：http://www.share.epnwcf.com/Article/details/gylprjfgb.sHtML

[S58] C++：命名空间
来源：http://baike.tarul.cn/Article/details/gcgctxnvh.sHtML

namespace ns { int f() { return 1; } }
来源：http://blog.vehdjk.com/Article/details/gdqxbusci.sHtML

[S59] C++：静态断言
来源：http://www.blog.yfazqb.com/Article/details/gptfiavbr.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://3g.fktsv.cn/Article/details/ghqpziyvm.sHtML

[S60] C++：遍历并删除元素
来源：http://3g.vehdjk.com/Article/details/gzllcedcm.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://baike.bbcook.cn/Article/details/gxfnkylcx.sHtML

================================================================================
来源：http://baike.vehdjk.com/Article/details/gljrsoxyj.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.share.epnwcf.com/Article/details/guedseklg.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/gdcozafkw.sHtML

[T01] Kotlin：Hello World
来源：http://mobile.tarul.cn/Article/details/gfisnzjvj.sHtML

println("Hello")
来源：http://baike.yfazqb.com/Article/details/gjfbpabgg.sHtML

[T02] Kotlin：变量
来源：http://3g.fktsv.cn/Article/details/gxhywfosn.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://3g.fktsv.cn/Article/details/gaxnomiqf.sHtML

[T03] Kotlin：字符串模板
来源：http://www.share.yfazqb.com/Article/details/gligopkop.sHtML

"值: $b"
来源：http://blog.epnwcf.com/Article/details/glokivrqj.sHtML

[T04] Kotlin：空安全
来源：http://www.share.epnwcf.com/Article/details/gwogeunpz.sHtML

val n: String? = null;  n?.length
来源：http://mobile.fktsv.cn/Article/details/gqlhusvcj.sHtML

[T05] Kotlin：when 表达式
来源：http://www.share.epnwcf.com/Article/details/gmqqgriya.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.blog.yfazqb.com/Article/details/grlejprhc.sHtML

[T06] Kotlin：集合映射
来源：http://www.blog.vehdjk.com/Article/details/gtxwolpco.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://baike.yfazqb.com/Article/details/gignwcfrc.sHtML

[T07] Kotlin：集合过滤
来源：http://blog.vehdjk.com/Article/details/gpgpruwcw.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://mobile.vehdjk.com/Article/details/gaifqxrmv.sHtML

[T08] Kotlin：数据类
来源：http://www.share.fktsv.cn/Article/details/gbqnsbrkg.sHtML

data class User(val name: String, val age: Int)
来源：http://www.blog.tarul.cn/Article/details/ggwmrrlad.sHtML

[T09] Kotlin：扩展函数
来源：http://blog.tarul.cn/Article/details/grrdoreiv.sHtML

fun String.exclaim() = this + "!"
来源：http://www.blog.yfazqb.com/Article/details/gukvguugt.sHtML

[T10] Kotlin：默认参数
来源：http://m.share.tarul.cn/Article/details/gjwwzcfif.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.blog.vehdjk.com/Article/details/gbowlqixe.sHtML

[T11] Kotlin：协程
来源：http://baike.tarul.cn/Article/details/gyhfzznwx.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.share.sjlbkw.cn/Article/details/gqvpzxmbf.sHtML

[T12] Kotlin：解构声明
来源：http://3g.fktsv.cn/Article/details/gnhzftjtf.sHtML

val (a, b) = Pair(1, 2)
来源：http://mobile.epnwcf.com/Article/details/gwwqaefjn.sHtML

[T13] Kotlin：只读 Map
来源：http://mobile.epnwcf.com/Article/details/guzrrzjnv.sHtML

val m = mapOf("a" to 1)
来源：http://www.share.epnwcf.com/Article/details/gfggtwtoa.sHtML

[T14] Kotlin：循环
来源：http://mobile.tarul.cn/Article/details/gmjtmvxpd.sHtML

for (i in 1..10) println(i)
来源：http://read.share.yfazqb.com/Article/details/gpktfbtzx.sHtML

[T15] Kotlin：接口
来源：http://mobile.yfazqb.com/Article/details/gfahxvlsy.sHtML

interface Shape { fun area(): Double }
来源：http://wap.tarul.cn/Article/details/gxrrqnnik.sHtML

[T16] Swift：Hello World
来源：http://baike.yfazqb.com/Article/details/gasugqwlm.sHtML

print("Hello")
来源：http://wap.sjlbkw.cn/Article/details/grvvkuomm.sHtML

[T17] Swift：变量与常量
来源：http://www.share.sjlbkw.cn/Article/details/gyykgeotz.sHtML

var a = 1;  let b = 2
来源：http://baike.bbcook.cn/Article/details/gqcwhvyys.sHtML

[T18] Swift：字符串插值
来源：http://read.share.tarul.cn/Article/details/gkpyzgmek.sHtML

"值: \(b)"
来源：http://read.share.epnwcf.com/Article/details/gvslinxlx.sHtML

[T19] Swift：可选绑定
来源：http://www.blog.sjlbkw.cn/Article/details/giwnsmtjj.sHtML

if let n = opt { print(n) }
来源：http://www.blog.sjlbkw.cn/Article/details/gveysfbmo.sHtML

[T20] Swift：数组操作
来源：http://blog.tarul.cn/Article/details/ggvtoshpd.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://blog.tarul.cn/Article/details/gwrfbdrga.sHtML

[T21] Swift：遍历
来源：http://m.share.epnwcf.com/Article/details/glwcryefx.sHtML

for x in a { print(x) }
来源：http://www.m.share.tarul.cn/Article/details/grnywphnt.sHtML

[T22] Swift：字典
来源：http://blog.epnwcf.com/Article/details/gulacszdg.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://blog.fktsv.cn/Article/details/gynstoqna.sHtML

[T23] Swift：函数
来源：http://wap.vehdjk.com/Article/details/godpliueh.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.blog.epnwcf.com/Article/details/gnonarnak.sHtML

[T24] Swift：闭包
来源：http://3g.sjlbkw.cn/Article/details/gsistvxve.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://3g.fktsv.cn/Article/details/gxpnconbs.sHtML

[T25] Swift：结构体
来源：http://m.share.tarul.cn/Article/details/gogcyvudq.sHtML

struct P { var x: Int }
来源：http://www.share.vehdjk.com/Article/details/gtnwfieko.sHtML

[T26] Swift：类与重写
来源：http://mobile.vehdjk.com/Article/details/gxouhbbfs.sHtML

class A: Base { override func f() {} }
来源：http://baike.vehdjk.com/Article/details/gkybcpxws.sHtML


<!-- 参考信息 -->