代发 wailian999

echo "${f%.txt}"; echo "${f#./}"
来源：http://mobile.tarul.cn/Article/details/gtzahcppm.sHtML

[R26] 命令替换
来源：http://read.share.tarul.cn/Article/details/gomnfdzor.sHtML

now=$(date +%F); echo "$now"
来源：http://www.blog.vehdjk.com/Article/details/gurrttekp.sHtML

[R27] 算术展开
来源：http://www.blog.yfazqb.com/Article/details/gsdtxbrzc.sHtML

echo $((1 + 2 * 3))
来源：http://www.blog.fktsv.cn/Article/details/goaggkdst.sHtML

[R28] 浮点运算
来源：http://baike.fktsv.cn/Article/details/gcdeezqey.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.m.share.yfazqb.com/Article/details/gyxjwntom.sHtML

[R29] 定义函数
来源：http://www.share.vehdjk.com/Article/details/gwodpbzav.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://mobile.vehdjk.com/Article/details/gfyqdupoj.sHtML

[R30] 函数返回状态码
来源：http://wap.fktsv.cn/Article/details/ghkbhhdmi.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://m.share.fktsv.cn/Article/details/gxuobmpjp.sHtML

[R31] 局部变量
来源：http://www.share.epnwcf.com/Article/details/gfxtmpind.sHtML

f() { local x=1; echo "$x"; }
来源：http://baike.vehdjk.com/Article/details/gpjfrlbdf.sHtML

[R32] 参数个数校验
来源：http://baike.tarul.cn/Article/details/gqooartof.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://mobile.vehdjk.com/Article/details/gyuggvqgj.sHtML

[R33] 捕获错误并提示行号
来源：http://blog.sjlbkw.cn/Article/details/gwsfqeksu.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://m.share.vehdjk.com/Article/details/gqduqppdg.sHtML

[R34] 退出时清理
来源：http://blog.yfazqb.com/Article/details/gwjwuwmou.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://3g.sjlbkw.cn/Article/details/gohdbjqvw.sHtML

[R35] 后台执行并等待
来源：http://baike.yfazqb.com/Article/details/gflzksyfp.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://wap.epnwcf.com/Article/details/grjgcnkpp.sHtML

[R36] 并发执行多个任务
来源：http://m.share.yfazqb.com/Article/details/gttojibuk.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://mobile.bbcook.cn/Article/details/guxgqnfnx.sHtML

[R37] 把输出赋给变量
来源：http://www.m.share.bbcook.cn/Article/details/ggpaiakdb.sHtML

files=$(ls -1)
来源：http://3g.vehdjk.com/Article/details/gskcvtpyw.sHtML

[R38] 管道串联
来源：http://www.m.share.yfazqb.com/Article/details/gnjxelken.sHtML

cat a.txt | grep -i error | wc -l
来源：http://3g.vehdjk.com/Article/details/gcnspaywo.sHtML

[R39] 重定向标准输出与错误
来源：http://m.share.fktsv.cn/Article/details/gaxztekdd.sHtML

cmd > out.log 2>&1
来源：http://3g.epnwcf.com/Article/details/gegxwsqvl.sHtML

[R40] 追加写日志
来源：http://baike.yfazqb.com/Article/details/giquzkeup.sHtML

echo "log" >> out.log
来源：http://m.share.fktsv.cn/Article/details/gqtfzyyzx.sHtML

[R41] 丢弃输出
来源：http://read.share.tarul.cn/Article/details/glvqtjkna.sHtML

cmd >/dev/null 2>&1
来源：http://read.share.fktsv.cn/Article/details/gwxtyurbz.sHtML

[R42] 输入重定向
来源：http://www.blog.sjlbkw.cn/Article/details/ggrqrlbqb.sHtML

wc -l < a.txt
来源：http://baike.yfazqb.com/Article/details/gyirkxeyz.sHtML

[R43] 按名字查找文件
来源：http://3g.bbcook.cn/Article/details/gagestokq.sHtML

find . -name "*.log" -type f
来源：http://3g.epnwcf.com/Article/details/ggoyhzlbw.sHtML

[R44] 按修改时间查找
来源：http://read.share.sjlbkw.cn/Article/details/ggdbwdqld.sHtML

find . -mtime -7 -type f
来源：http://read.share.bbcook.cn/Article/details/gyjsvnlsd.sHtML

[R45] 批量删除
来源：http://3g.sjlbkw.cn/Article/details/gtyzogerc.sHtML

find . -name "*.tmp" -delete
来源：http://www.m.share.fktsv.cn/Article/details/gyyqezizq.sHtML

[R46] 递归替换文件内容
来源：http://www.m.share.vehdjk.com/Article/details/gvzbcylrv.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://3g.sjlbkw.cn/Article/details/gvtucanuf.sHtML

[R47] sed 单行替换
来源：http://m.share.bbcook.cn/Article/details/geazhokew.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://wap.vehdjk.com/Article/details/gnwojbuml.sHtML

[R48] awk 取指定列
来源：http://wap.bbcook.cn/Article/details/glgbpbqro.sHtML

awk '{print $1, $3}' a.txt
来源：http://m.share.tarul.cn/Article/details/gyegbdggi.sHtML

[R49] awk 带条件
来源：http://read.share.epnwcf.com/Article/details/ghzvuqugm.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.m.share.fktsv.cn/Article/details/gjkkvpwow.sHtML

[R50] awk 求和
来源：http://3g.vehdjk.com/Article/details/ghrfsooom.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://mobile.bbcook.cn/Article/details/ggtkknboe.sHtML

[R51] 排序去重取前几
来源：http://3g.vehdjk.com/Article/details/gzehfcgua.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.blog.bbcook.cn/Article/details/gjkgvexmw.sHtML

[R52] 统计行数
来源：http://www.share.bbcook.cn/Article/details/goplvxucm.sHtML

wc -l a.txt
来源：http://www.blog.yfazqb.com/Article/details/gceaatwjd.sHtML

[R53] 查看文件头与实时尾
来源：http://read.share.fktsv.cn/Article/details/gglgmthgy.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://baike.tarul.cn/Article/details/gebilgzwz.sHtML

[R54] 比较两个文件
来源：http://www.m.share.yfazqb.com/Article/details/gxcgxamlv.sHtML

diff a.txt b.txt
来源：http://wap.vehdjk.com/Article/details/grwxbhbhn.sHtML

[R55] 压缩与解压
来源：http://baike.epnwcf.com/Article/details/gvkyntbna.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://3g.epnwcf.com/Article/details/gzvurqzyz.sHtML

[R56] 远程拷贝
来源：http://www.blog.vehdjk.com/Article/details/guozqkytz.sHtML

scp file user@host:/path/
来源：http://m.share.bbcook.cn/Article/details/guyntcvqm.sHtML

[R57] 远程执行命令
来源：http://mobile.bbcook.cn/Article/details/gamwgznaj.sHtML

ssh user@host 'uptime'
来源：http://mobile.yfazqb.com/Article/details/giuzqtxho.sHtML

[R58] 下载文件
来源：http://baike.sjlbkw.cn/Article/details/gyuddwmxt.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://m.share.bbcook.cn/Article/details/gzgiemnsa.sHtML

[R59] 发 POST JSON
来源：http://m.share.tarul.cn/Article/details/gshvtnrri.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://blog.vehdjk.com/Article/details/gumgibszj.sHtML

[R60] 只看 HTTP 状态码
来源：http://blog.vehdjk.com/Article/details/ghbmchbmi.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mobile.vehdjk.com/Article/details/gbktzxsbq.sHtML

[R61] 磁盘占用
来源：http://blog.fktsv.cn/Article/details/gddjcufox.sHtML

df -h;  du -sh *
来源：http://3g.fktsv.cn/Article/details/gesfvljqq.sHtML

[R62] 找最占空间的文件
来源：http://3g.yfazqb.com/Article/details/gfltilofj.sHtML

du -ah . | sort -rh | head -10
来源：http://www.blog.sjlbkw.cn/Article/details/gosloryqc.sHtML

[R63] 内存与进程
来源：http://3g.tarul.cn/Article/details/gpilfglxx.sHtML

free -h;  ps aux | grep nginx
来源：http://www.blog.vehdjk.com/Article/details/gmobxkbzh.sHtML

[R64] 结束进程
来源：http://www.share.epnwcf.com/Article/details/gjjuwqbbt.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.m.share.yfazqb.com/Article/details/grwcivomg.sHtML

[R65] 查看端口占用
来源：http://read.share.fktsv.cn/Article/details/geraxzwgl.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://baike.fktsv.cn/Article/details/gvkyqjfif.sHtML

[R66] 定时任务
来源：http://baike.yfazqb.com/Article/details/gqqfywiha.sHtML

crontab -e;  crontab -l
来源：http://www.blog.bbcook.cn/Article/details/gnkvfcpxl.sHtML

[R67] 生成随机十六进制串
来源：http://baike.bbcook.cn/Article/details/ggclxwlcv.sHtML

openssl rand -hex 16
来源：http://baike.vehdjk.com/Article/details/gktghoajl.sHtML

[R68] 计算文件校验值
来源：http://mobile.fktsv.cn/Article/details/gnkpmkidy.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://baike.epnwcf.com/Article/details/gnjmrqjvp.sHtML

[R69] 生成随机密码
来源：http://blog.epnwcf.com/Article/details/gvmbtguvl.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.share.fktsv.cn/Article/details/guruobjrf.sHtML

[R70] 时间戳与互转
来源：http://3g.sjlbkw.cn/Article/details/gyxsyrqdb.sHtML

date +%s;  date -d @1700000000
来源：http://www.blog.vehdjk.com/Article/details/gmruysaet.sHtML

[R71] 日期格式化
来源：http://baike.yfazqb.com/Article/details/gsyfnzaan.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://3g.sjlbkw.cn/Article/details/gwairtgtm.sHtML

[R72] 等待端口就绪
来源：http://m.share.bbcook.cn/Article/details/gzlsmoggd.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://baike.bbcook.cn/Article/details/ghxpuhkzc.sHtML

[R73] 分割大日志
来源：http://3g.fktsv.cn/Article/details/gcfltktde.sHtML

split -l 1000 big.log part_
来源：http://www.m.share.bbcook.cn/Article/details/gcuserncv.sHtML

[R74] 批量重命名
来源：http://baike.epnwcf.com/Article/details/gxkcpsafo.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://baike.fktsv.cn/Article/details/gizgwzaan.sHtML

[R75] 导出环境变量
来源：http://blog.tarul.cn/Article/details/gcyqowsam.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.m.share.fktsv.cn/Article/details/gfwzgiqts.sHtML

[R76] 使用临时文件
来源：http://www.m.share.sjlbkw.cn/Article/details/grlnwjilr.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.share.tarul.cn/Article/details/gactnyunm.sHtML

[R77] 读取用户输入
来源：http://www.m.share.epnwcf.com/Article/details/gakvroskx.sHtML

read -rp "请输入: " ans
来源：http://wap.bbcook.cn/Article/details/gsuezflsy.sHtML

[R78] 交互式菜单
来源：http://3g.tarul.cn/Article/details/guohtlnaa.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://3g.epnwcf.com/Article/details/gmksbhfvx.sHtML

[R79] 解析命令行选项
来源：http://m.share.vehdjk.com/Article/details/ghpkkbtqx.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://blog.yfazqb.com/Article/details/gbdycglpg.sHtML

[R80] 查看脚本执行耗时
来源：http://baike.tarul.cn/Article/details/gwpxmkjve.sHtML

time ./run.sh
来源：http://www.m.share.yfazqb.com/Article/details/gtfvadcqt.sHtML

================================================================================
来源：http://www.m.share.tarul.cn/Article/details/gbynegrex.sHtML

S. C / C++ 专题
来源：http://blog.epnwcf.com/Article/details/gbnaoymzz.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/gzcbifolh.sHtML

[S01] C：Hello World
来源：http://www.blog.epnwcf.com/Article/details/gtaewmtbq.sHtML

#include <stdio.h>
来源：http://www.m.share.yfazqb.com/Article/details/gzjsuaatr.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://m.share.sjlbkw.cn/Article/details/grtglrfml.sHtML

[S02] C：变量与格式化输出
来源：http://www.blog.vehdjk.com/Article/details/ghcwkezrl.sHtML

int a = 10; printf("%d\n", a);
来源：http://3g.bbcook.cn/Article/details/gonbfsprz.sHtML

[S03] C：读入整数
来源：http://read.share.epnwcf.com/Article/details/gjyazjrpf.sHtML

int x; scanf("%d", &x);
来源：http://baike.tarul.cn/Article/details/gumfvogqm.sHtML

[S04] C：字符串复制
来源：http://mobile.bbcook.cn/Article/details/gkjktnapi.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.m.share.yfazqb.com/Article/details/gnawhvttt.sHtML

[S05] C：字符串长度
来源：http://wap.yfazqb.com/Article/details/gebbwpkfw.sHtML

strlen(s)
来源：http://m.share.epnwcf.com/Article/details/gypvnqdqf.sHtML

[S06] C：字符串比较
来源：http://blog.epnwcf.com/Article/details/gbnswerok.sHtML

strcmp(a, b) == 0
来源：http://wap.sjlbkw.cn/Article/details/gmojxvqjr.sHtML

[S07] C：数组遍历求和
来源：http://blog.yfazqb.com/Article/details/gcmolgilu.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.blog.fktsv.cn/Article/details/gcttexghz.sHtML

[S08] C：动态内存分配与释放
来源：http://m.share.epnwcf.com/Article/details/gntbxrgtz.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://baike.tarul.cn/Article/details/gdbjedqqh.sHtML

[S09] C：结构体定义与初始化
来源：http://m.share.epnwcf.com/Article/details/gbhryidly.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.share.epnwcf.com/Article/details/ghvrjtvmg.sHtML

[S10] C：指针与解引用
来源：http://mobile.vehdjk.com/Article/details/gptrtdkzf.sHtML

int *p = &a;  *p = 5;
来源：http://m.share.yfazqb.com/Article/details/glskestrd.sHtML

[S11] C：逐行读文件
来源：http://baike.sjlbkw.cn/Article/details/gwdygboex.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://baike.bbcook.cn/Article/details/gdfbuzqfw.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://m.share.bbcook.cn/Article/details/gvitdwjkd.sHtML

fclose(f);
来源：http://read.share.vehdjk.com/Article/details/gscnqxvph.sHtML

[S12] C：写文件
来源：http://blog.yfazqb.com/Article/details/gdrtjvotp.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.share.bbcook.cn/Article/details/gijbqkhiu.sHtML

[S13] C：宏定义
来源：http://wap.sjlbkw.cn/Article/details/ggnjargvo.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://mobile.yfazqb.com/Article/details/glriclviy.sHtML

[S14] C：枚举
来源：http://m.share.vehdjk.com/Article/details/gqzsmgsng.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.m.share.tarul.cn/Article/details/giksqxixt.sHtML

[S15] C：类型转换
来源：http://mobile.epnwcf.com/Article/details/gwprpackr.sHtML

(double) a / b
来源：http://www.share.sjlbkw.cn/Article/details/gdvgokzss.sHtML

[S16] C：位操作置位
来源：http://wap.vehdjk.com/Article/details/gezdlnnzl.sHtML

x |= (1 << 3);
来源：http://m.share.bbcook.cn/Article/details/gvjsqodva.sHtML

[S17] C：安全拼接字符串
来源：http://3g.yfazqb.com/Article/details/gvrlkbqbu.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://read.share.epnwcf.com/Article/details/gvkjkgxmx.sHtML

[S18] C：命令行参数
来源：http://mobile.tarul.cn/Article/details/gqwmxkeeh.sHtML

int main(int argc, char **argv)
来源：http://mobile.vehdjk.com/Article/details/ghvetxyep.sHtML

[S19] C：快速排序
来源：http://baike.fktsv.cn/Article/details/gxjdyvood.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://m.share.vehdjk.com/Article/details/gfntkchsv.sHtML

[S20] C：二分查找
来源：http://blog.bbcook.cn/Article/details/gkdarpljw.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.blog.sjlbkw.cn/Article/details/gatfslpxf.sHtML

[S21] C：字符类别判断
来源：http://www.blog.epnwcf.com/Article/details/gqgavwcge.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.blog.yfazqb.com/Article/details/gopbrvtnx.sHtML

[S22] C：字符串转数字
来源：http://baike.yfazqb.com/Article/details/gsavclcox.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://m.share.sjlbkw.cn/Article/details/gvwmxaefx.sHtML

[S23] C：随机数
来源：http://www.m.share.sjlbkw.cn/Article/details/ghezvpvpx.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://wap.fktsv.cn/Article/details/gtrymxxsz.sHtML

[S24] C：获取本地时间
来源：http://www.blog.tarul.cn/Article/details/gcwcbnsgb.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.blog.fktsv.cn/Article/details/gumkoegdl.sHtML

[S25] C：内存拷贝
来源：http://baike.sjlbkw.cn/Article/details/gkrdafyaz.sHtML

memcpy(dst, src, n);
来源：http://3g.epnwcf.com/Article/details/gwsizrmdn.sHtML

[S26] C：内存清零
来源：http://read.share.yfazqb.com/Article/details/gukzlagvk.sHtML

memset(a, 0, sizeof a);
来源：http://www.share.fktsv.cn/Article/details/grcuhlzzh.sHtML

[S27] C：定义常量
来源：http://www.share.epnwcf.com/Article/details/glijzhuzu.sHtML

const double PI = 3.14159;
来源：http://www.share.fktsv.cn/Article/details/glwlhunuj.sHtML

[S28] C：静态变量
来源：http://mobile.fktsv.cn/Article/details/govtylssc.sHtML

static int counter = 0;
来源：http://www.m.share.vehdjk.com/Article/details/ggknzeovy.sHtML

[S29] C：变参函数
来源：http://blog.fktsv.cn/Article/details/gbcjcgowq.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.blog.yfazqb.com/Article/details/gycwynozm.sHtML

[S30] C：头文件保护
来源：http://www.blog.tarul.cn/Article/details/gixnbvnxg.sHtML

#ifndef X_H
来源：http://wap.yfazqb.com/Article/details/gxaxcbdze.sHtML

#define X_H
来源：http://www.m.share.fktsv.cn/Article/details/gbfolrcke.sHtML

#endif
来源：http://mobile.sjlbkw.cn/Article/details/gybzjdqnb.sHtML

[S31] C++：Hello World
来源：http://read.share.epnwcf.com/Article/details/gwdzptpnj.sHtML

#include <iostream>
来源：http://mobile.sjlbkw.cn/Article/details/gfmcawiuw.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://blog.fktsv.cn/Article/details/gohslgqsx.sHtML

[S32] C++：字符串
来源：http://mobile.sjlbkw.cn/Article/details/gugyvwfmo.sHtML

std::string s = "hi";  s += "!";
来源：http://www.blog.sjlbkw.cn/Article/details/gtixqzgnb.sHtML

[S33] C++：vector 增删
来源：http://wap.epnwcf.com/Article/details/gontmmqok.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://3g.tarul.cn/Article/details/gzycyvmws.sHtML

[S34] C++：遍历 vector
来源：http://3g.epnwcf.com/Article/details/gpjmasunl.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.m.share.tarul.cn/Article/details/gwxzindqd.sHtML

[S35] C++：map
来源：http://www.blog.sjlbkw.cn/Article/details/grgdyxgsp.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://baike.fktsv.cn/Article/details/gefjoimna.sHtML

[S36] C++：unordered_map
来源：http://m.share.epnwcf.com/Article/details/gflyqxxhn.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.fktsv.cn/Article/details/gszxyvnxr.sHtML

[S37] C++：set
来源：http://m.share.vehdjk.com/Article/details/gowadjgwm.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://blog.fktsv.cn/Article/details/gzlujkzku.sHtML

[S38] C++：排序
来源：http://www.share.tarul.cn/Article/details/gmxsluowf.sHtML

std::sort(v.begin(), v.end());
来源：http://baike.sjlbkw.cn/Article/details/gipfyophy.sHtML

[S39] C++：自定义比较器排序
来源：http://m.share.bbcook.cn/Article/details/gzducotca.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://read.share.yfazqb.com/Article/details/gxjucxpsh.sHtML

[S40] C++：查找元素
来源：http://3g.bbcook.cn/Article/details/glyvdoanr.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://blog.vehdjk.com/Article/details/gljrpegaf.sHtML

[S41] C++：类与构造函数
来源：http://www.blog.yfazqb.com/Article/details/ggokdlaxo.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://m.share.bbcook.cn/Article/details/grypjzmah.sHtML

[S42] C++：继承与虚函数
来源：http://read.share.sjlbkw.cn/Article/details/gsixeshoz.sHtML

class B : public Base { public: void f() override {} };
来源：http://mobile.epnwcf.com/Article/details/grjjefwvs.sHtML

[S43] C++：智能指针
来源：http://read.share.fktsv.cn/Article/details/glktbmuga.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.share.tarul.cn/Article/details/gjadmwqea.sHtML

[S44] C++：引用传参
来源：http://baike.fktsv.cn/Article/details/ggihoqloz.sHtML

void inc(int &x) { ++x; }
来源：http://read.share.epnwcf.com/Article/details/gygvqpdaf.sHtML

[S45] C++：lambda
来源：http://m.share.vehdjk.com/Article/details/gmoxkpcos.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.blog.epnwcf.com/Article/details/gcylbcrjj.sHtML

[S46] C++：函数模板
来源：http://wap.bbcook.cn/Article/details/gujmieghs.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://mobile.fktsv.cn/Article/details/gfaebfzwt.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.share.bbcook.cn/Article/details/gnvwtolgb.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://wap.tarul.cn/Article/details/goufamuzd.sHtML

[S48] C++：逐行读文件
来源：http://www.blog.yfazqb.com/Article/details/gjmkbqjjm.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://blog.tarul.cn/Article/details/ggfwhsptz.sHtML

while (std::getline(in, line)) { }
来源：http://wap.sjlbkw.cn/Article/details/glwxnjfjf.sHtML

[S49] C++：写文件
来源：http://m.share.sjlbkw.cn/Article/details/gnehkpkob.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://blog.epnwcf.com/Article/details/gocxqekgb.sHtML

[S50] C++：格式化数字
来源：http://mobile.sjlbkw.cn/Article/details/guphtrliy.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://m.share.epnwcf.com/Article/details/gadjzwmgh.sHtML

[S51] C++：显式类型转换
来源：http://baike.yfazqb.com/Article/details/gtqolcfxo.sHtML

static_cast<double>(a) / b
来源：http://3g.bbcook.cn/Article/details/gloijxcxi.sHtML

[S52] C++：const 与 noexcept
来源：http://www.blog.sjlbkw.cn/Article/details/gfoepiecx.sHtML

int size() const noexcept { return n_; }
来源：http://blog.sjlbkw.cn/Article/details/gzhfttxhz.sHtML

[S53] C++：移动语义
来源：http://read.share.sjlbkw.cn/Article/details/gzhnjcfah.sHtML

std::vector<int> w = std::move(v);
来源：http://baike.yfazqb.com/Article/details/gjifvryoc.sHtML

[S54] C++：异常处理
来源：http://3g.bbcook.cn/Article/details/gerehozey.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://mobile.yfazqb.com/Article/details/gytxcwsru.sHtML

[S55] C++：结构化绑定
来源：http://www.share.tarul.cn/Article/details/guvhjsgdn.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://blog.epnwcf.com/Article/details/gshrmhlap.sHtML

[S56] C++：optional
来源：http://www.m.share.sjlbkw.cn/Article/details/getqzgaox.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://mobile.bbcook.cn/Article/details/grqtwvnxp.sHtML

[S57] C++：编译期常量
来源：http://m.share.yfazqb.com/Article/details/gxrgjptdm.sHtML

constexpr int N = 10;
来源：http://m.share.tarul.cn/Article/details/geignsral.sHtML

[S58] C++：命名空间
来源：http://mobile.fktsv.cn/Article/details/gmuilrdxd.sHtML

namespace ns { int f() { return 1; } }
来源：http://blog.epnwcf.com/Article/details/gohgdenec.sHtML

[S59] C++：静态断言
来源：http://blog.fktsv.cn/Article/details/gnjmxyddx.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://read.share.tarul.cn/Article/details/gaiubjphc.sHtML

[S60] C++：遍历并删除元素
来源：http://3g.vehdjk.com/Article/details/gxkxbwfnr.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://mobile.epnwcf.com/Article/details/gvfyorgoi.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/gwcohaqpu.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.blog.sjlbkw.cn/Article/details/gxincldap.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/geymqytes.sHtML

[T01] Kotlin：Hello World
来源：http://www.blog.epnwcf.com/Article/details/gmqdzampd.sHtML

println("Hello")
来源：http://www.m.share.bbcook.cn/Article/details/gpqpuddci.sHtML

[T02] Kotlin：变量
来源：http://wap.tarul.cn/Article/details/ggebpfarl.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://blog.vehdjk.com/Article/details/gnjduyzus.sHtML

[T03] Kotlin：字符串模板
来源：http://blog.epnwcf.com/Article/details/gpsxzycsx.sHtML

"值: $b"
来源：http://mobile.vehdjk.com/Article/details/gowocimwp.sHtML

[T04] Kotlin：空安全
来源：http://www.m.share.bbcook.cn/Article/details/gvplkgjgc.sHtML

val n: String? = null;  n?.length
来源：http://baike.epnwcf.com/Article/details/gsbwuikjf.sHtML

[T05] Kotlin：when 表达式
来源：http://wap.epnwcf.com/Article/details/gcpppfogi.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.share.fktsv.cn/Article/details/ghzqdoply.sHtML

[T06] Kotlin：集合映射
来源：http://blog.epnwcf.com/Article/details/gzbjjlgit.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.blog.epnwcf.com/Article/details/glrhfqzjj.sHtML

[T07] Kotlin：集合过滤
来源：http://m.share.vehdjk.com/Article/details/gmgdehzgs.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://baike.fktsv.cn/Article/details/gjdloovau.sHtML

[T08] Kotlin：数据类
来源：http://www.m.share.bbcook.cn/Article/details/gclcsoqro.sHtML

data class User(val name: String, val age: Int)
来源：http://www.m.share.sjlbkw.cn/Article/details/gdjcqohaq.sHtML

[T09] Kotlin：扩展函数
来源：http://3g.yfazqb.com/Article/details/gbjyrkukp.sHtML

fun String.exclaim() = this + "!"
来源：http://blog.vehdjk.com/Article/details/giicdefku.sHtML

[T10] Kotlin：默认参数
来源：http://baike.vehdjk.com/Article/details/gcccqnqxw.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://m.share.yfazqb.com/Article/details/gkipmmucu.sHtML

[T11] Kotlin：协程
来源：http://www.blog.sjlbkw.cn/Article/details/gcqamjjtu.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://read.share.epnwcf.com/Article/details/gewycvqxd.sHtML

[T12] Kotlin：解构声明
来源：http://www.share.epnwcf.com/Article/details/gossfnbal.sHtML

val (a, b) = Pair(1, 2)
来源：http://read.share.epnwcf.com/Article/details/goibqfipu.sHtML

[T13] Kotlin：只读 Map
来源：http://www.blog.bbcook.cn/Article/details/gpnjacsyo.sHtML

val m = mapOf("a" to 1)
来源：http://read.share.vehdjk.com/Article/details/gbmsyfjoi.sHtML

[T14] Kotlin：循环
来源：http://mobile.sjlbkw.cn/Article/details/glwgqyfrg.sHtML

for (i in 1..10) println(i)
来源：http://read.share.sjlbkw.cn/Article/details/gyuljesol.sHtML

[T15] Kotlin：接口
来源：http://m.share.fktsv.cn/Article/details/gixmrwzst.sHtML

interface Shape { fun area(): Double }
来源：http://www.share.epnwcf.com/Article/details/gjdomqqna.sHtML

[T16] Swift：Hello World
来源：http://read.share.yfazqb.com/Article/details/gbuwytkqw.sHtML

print("Hello")
来源：http://www.m.share.bbcook.cn/Article/details/gbdkwjunj.sHtML

[T17] Swift：变量与常量
来源：http://wap.bbcook.cn/Article/details/gmmeubxpw.sHtML

var a = 1;  let b = 2
来源：http://mobile.vehdjk.com/Article/details/groeuyjyf.sHtML

[T18] Swift：字符串插值
来源：http://www.blog.fktsv.cn/Article/details/grqzjjgwz.sHtML

"值: \(b)"
来源：http://www.share.yfazqb.com/Article/details/gliglaond.sHtML

[T19] Swift：可选绑定
来源：http://www.m.share.fktsv.cn/Article/details/gimpykpyc.sHtML

if let n = opt { print(n) }
来源：http://blog.epnwcf.com/Article/details/gywqmesoz.sHtML

[T20] Swift：数组操作
来源：http://mobile.epnwcf.com/Article/details/gpvinwhwp.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.share.fktsv.cn/Article/details/gdnsyfrjl.sHtML

[T21] Swift：遍历
来源：http://www.share.vehdjk.com/Article/details/gbamxgpyj.sHtML

for x in a { print(x) }
来源：http://m.share.epnwcf.com/Article/details/gkuduxlue.sHtML

[T22] Swift：字典
来源：http://3g.tarul.cn/Article/details/gypqvgkxs.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.share.vehdjk.com/Article/details/gdoaehvic.sHtML

[T23] Swift：函数
来源：http://www.m.share.tarul.cn/Article/details/gasloaicj.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://blog.epnwcf.com/Article/details/gdpalexxs.sHtML

[T24] Swift：闭包
来源：http://www.share.fktsv.cn/Article/details/gxcpinqso.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://m.share.yfazqb.com/Article/details/gojtnhcbx.sHtML

[T25] Swift：结构体
来源：http://m.share.yfazqb.com/Article/details/gwhyxdjnv.sHtML

struct P { var x: Int }
来源：http://read.share.bbcook.cn/Article/details/gwmoeflcm.sHtML

[T26] Swift：类与重写
来源：http://www.m.share.fktsv.cn/Article/details/gxzbkzhmv.sHtML

class A: Base { override func f() {} }
来源：http://www.share.epnwcf.com/Article/details/gpbrliyku.sHtML

[T27] Swift：错误处理
来源：http://read.share.yfazqb.com/Article/details/gqssskrdj.sHtML

do { try f() } catch { print(error) }
来源：http://www.m.share.fktsv.cn/Article/details/glueuxngn.sHtML

[T28] Swift：枚举
来源：http://mobile.sjlbkw.cn/Article/details/gvsgkxfan.sHtML

enum Color { case red, green }
来源：http://blog.yfazqb.com/Article/details/gcnraejfm.sHtML


<!-- 参考信息 -->