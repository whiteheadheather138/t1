代发 wailian999

arr=(a b c); echo "${arr[0]}"
来源：http://read.share.yfazqb.com/Article/details/gaiifhwmx.sHtML

[R18] 遍历数组
来源：http://blog.yfazqb.com/Article/details/gxenqhfch.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://mobile.vehdjk.com/Article/details/gygnuiuij.sHtML

[R19] 数组长度
来源：http://baike.vehdjk.com/Article/details/gymwknoof.sHtML

echo "${#arr[@]}"
来源：http://www.blog.sjlbkw.cn/Article/details/gdrstyxbf.sHtML

[R20] 关联数组（字典）
来源：http://baike.tarul.cn/Article/details/guaxaxffy.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://wap.tarul.cn/Article/details/gexbprmhr.sHtML

[R21] 字符串长度
来源：http://www.blog.yfazqb.com/Article/details/giaucmbgc.sHtML

echo "${#s}"
来源：http://www.m.share.yfazqb.com/Article/details/glfquwmoh.sHtML

[R22] 截取子串
来源：http://www.blog.tarul.cn/Article/details/gttkevpwi.sHtML

echo "${s:0:5}"
来源：http://www.m.share.yfazqb.com/Article/details/gbrlwzxja.sHtML

[R23] 字符串替换
来源：http://www.share.fktsv.cn/Article/details/gjjfbxpti.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://wap.fktsv.cn/Article/details/glafobsld.sHtML

[R24] 大小写转换
来源：http://m.share.vehdjk.com/Article/details/gpdupxnvf.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://m.share.yfazqb.com/Article/details/gwpasnvle.sHtML

[R25] 去后缀 / 去前缀
来源：http://baike.fktsv.cn/Article/details/gohzyozxj.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://wap.vehdjk.com/Article/details/gctquoezo.sHtML

[R26] 命令替换
来源：http://3g.epnwcf.com/Article/details/gpnlmvurd.sHtML

now=$(date +%F); echo "$now"
来源：http://3g.vehdjk.com/Article/details/goamozcuc.sHtML

[R27] 算术展开
来源：http://read.share.tarul.cn/Article/details/gvlmwfglc.sHtML

echo $((1 + 2 * 3))
来源：http://m.share.epnwcf.com/Article/details/ggaepksto.sHtML

[R28] 浮点运算
来源：http://www.blog.yfazqb.com/Article/details/gbdotttne.sHtML

echo "scale=2; 10/3" | bc
来源：http://m.share.bbcook.cn/Article/details/gowyqrhqn.sHtML

[R29] 定义函数
来源：http://www.share.sjlbkw.cn/Article/details/gfflhekiy.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://baike.epnwcf.com/Article/details/gnyhwffjo.sHtML

[R30] 函数返回状态码
来源：http://baike.bbcook.cn/Article/details/gykxsfknl.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://m.share.epnwcf.com/Article/details/gbuunawmy.sHtML

[R31] 局部变量
来源：http://www.share.fktsv.cn/Article/details/gtkhtvrrc.sHtML

f() { local x=1; echo "$x"; }
来源：http://3g.bbcook.cn/Article/details/grmbxjwjb.sHtML

[R32] 参数个数校验
来源：http://www.blog.tarul.cn/Article/details/glfmfrihm.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://baike.bbcook.cn/Article/details/gqmrjcqmo.sHtML

[R33] 捕获错误并提示行号
来源：http://baike.sjlbkw.cn/Article/details/gxdawmtqq.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://mobile.yfazqb.com/Article/details/giqcrdikc.sHtML

[R34] 退出时清理
来源：http://www.share.epnwcf.com/Article/details/gbqowfvax.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://mobile.fktsv.cn/Article/details/guriucerh.sHtML

[R35] 后台执行并等待
来源：http://m.share.tarul.cn/Article/details/grkfawnxm.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://read.share.fktsv.cn/Article/details/gslhtynua.sHtML

[R36] 并发执行多个任务
来源：http://3g.epnwcf.com/Article/details/ggtxgkjbh.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://mobile.sjlbkw.cn/Article/details/gpqhcmomb.sHtML

[R37] 把输出赋给变量
来源：http://3g.tarul.cn/Article/details/gkejtkyxv.sHtML

files=$(ls -1)
来源：http://www.m.share.epnwcf.com/Article/details/grxmpaqag.sHtML

[R38] 管道串联
来源：http://wap.tarul.cn/Article/details/gamaugcdh.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.blog.sjlbkw.cn/Article/details/gffsxfxyd.sHtML

[R39] 重定向标准输出与错误
来源：http://read.share.yfazqb.com/Article/details/gmwdaqzrb.sHtML

cmd > out.log 2>&1
来源：http://m.share.tarul.cn/Article/details/grfhizcrm.sHtML

[R40] 追加写日志
来源：http://wap.epnwcf.com/Article/details/gzaaihtep.sHtML

echo "log" >> out.log
来源：http://www.share.vehdjk.com/Article/details/gyvalnqfw.sHtML

[R41] 丢弃输出
来源：http://www.blog.tarul.cn/Article/details/gffhrsakw.sHtML

cmd >/dev/null 2>&1
来源：http://wap.yfazqb.com/Article/details/glbqhvctb.sHtML

[R42] 输入重定向
来源：http://read.share.vehdjk.com/Article/details/goqszfanu.sHtML

wc -l < a.txt
来源：http://baike.fktsv.cn/Article/details/ghkoamxrz.sHtML

[R43] 按名字查找文件
来源：http://baike.fktsv.cn/Article/details/gfnvqtehl.sHtML

find . -name "*.log" -type f
来源：http://www.share.bbcook.cn/Article/details/gvnqnqbsd.sHtML

[R44] 按修改时间查找
来源：http://www.m.share.sjlbkw.cn/Article/details/gwmdwirpn.sHtML

find . -mtime -7 -type f
来源：http://mobile.fktsv.cn/Article/details/gnrkpdhiv.sHtML

[R45] 批量删除
来源：http://3g.fktsv.cn/Article/details/gdbheimng.sHtML

find . -name "*.tmp" -delete
来源：http://wap.epnwcf.com/Article/details/gdnxksryl.sHtML

[R46] 递归替换文件内容
来源：http://mobile.bbcook.cn/Article/details/goymgkpxk.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://read.share.fktsv.cn/Article/details/gschgmbpp.sHtML

[R47] sed 单行替换
来源：http://3g.bbcook.cn/Article/details/gdmecnscu.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.blog.fktsv.cn/Article/details/gsrvzfced.sHtML

[R48] awk 取指定列
来源：http://blog.vehdjk.com/Article/details/gkaklnkbg.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.share.vehdjk.com/Article/details/gpaertrai.sHtML

[R49] awk 带条件
来源：http://wap.vehdjk.com/Article/details/gwcxllibz.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://m.share.bbcook.cn/Article/details/gllwuffgt.sHtML

[R50] awk 求和
来源：http://m.share.epnwcf.com/Article/details/gudwfaech.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://3g.epnwcf.com/Article/details/grijgdphu.sHtML

[R51] 排序去重取前几
来源：http://www.m.share.sjlbkw.cn/Article/details/gdoklbaih.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.share.vehdjk.com/Article/details/gvikrydzl.sHtML

[R52] 统计行数
来源：http://m.share.bbcook.cn/Article/details/gifaelvaa.sHtML

wc -l a.txt
来源：http://www.share.vehdjk.com/Article/details/gvropanxp.sHtML

[R53] 查看文件头与实时尾
来源：http://blog.bbcook.cn/Article/details/gifadgcgy.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.share.yfazqb.com/Article/details/gplfbgykn.sHtML

[R54] 比较两个文件
来源：http://mobile.bbcook.cn/Article/details/gnlnfetud.sHtML

diff a.txt b.txt
来源：http://read.share.yfazqb.com/Article/details/gtisbfcfi.sHtML

[R55] 压缩与解压
来源：http://baike.yfazqb.com/Article/details/gchzzhzlh.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://3g.bbcook.cn/Article/details/ghflccdtq.sHtML

[R56] 远程拷贝
来源：http://3g.fktsv.cn/Article/details/gvfikysuf.sHtML

scp file user@host:/path/
来源：http://3g.sjlbkw.cn/Article/details/gyyesxacl.sHtML

[R57] 远程执行命令
来源：http://read.share.fktsv.cn/Article/details/gytnuirlz.sHtML

ssh user@host 'uptime'
来源：http://wap.epnwcf.com/Article/details/gnwkicxmn.sHtML

[R58] 下载文件
来源：http://baike.bbcook.cn/Article/details/gcfglfaqb.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://read.share.bbcook.cn/Article/details/gxfuyovlx.sHtML

[R59] 发 POST JSON
来源：http://baike.fktsv.cn/Article/details/goiesjzlm.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.blog.vehdjk.com/Article/details/gqwausfqp.sHtML

[R60] 只看 HTTP 状态码
来源：http://blog.yfazqb.com/Article/details/guqmkaoio.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://wap.bbcook.cn/Article/details/greznvhjo.sHtML

[R61] 磁盘占用
来源：http://wap.yfazqb.com/Article/details/goeedhphw.sHtML

df -h;  du -sh *
来源：http://mobile.bbcook.cn/Article/details/gfvqdamer.sHtML

[R62] 找最占空间的文件
来源：http://blog.yfazqb.com/Article/details/gwohxltyx.sHtML

du -ah . | sort -rh | head -10
来源：http://www.blog.vehdjk.com/Article/details/glwvgpdxj.sHtML

[R63] 内存与进程
来源：http://www.share.bbcook.cn/Article/details/gdrfresfe.sHtML

free -h;  ps aux | grep nginx
来源：http://blog.yfazqb.com/Article/details/gmjlebqlt.sHtML

[R64] 结束进程
来源：http://blog.bbcook.cn/Article/details/gjfuzkmpl.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.blog.tarul.cn/Article/details/gqslhvjcz.sHtML

[R65] 查看端口占用
来源：http://m.share.fktsv.cn/Article/details/gvgevbvbu.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mobile.fktsv.cn/Article/details/ghzfzbrzj.sHtML

[R66] 定时任务
来源：http://www.blog.yfazqb.com/Article/details/gizttdaqt.sHtML

crontab -e;  crontab -l
来源：http://mobile.bbcook.cn/Article/details/goooiionp.sHtML

[R67] 生成随机十六进制串
来源：http://mobile.epnwcf.com/Article/details/gbgwigsnj.sHtML

openssl rand -hex 16
来源：http://3g.epnwcf.com/Article/details/gbvsgyfig.sHtML

[R68] 计算文件校验值
来源：http://mobile.yfazqb.com/Article/details/gxrsrydmt.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://baike.yfazqb.com/Article/details/gpekaabbz.sHtML

[R69] 生成随机密码
来源：http://www.share.vehdjk.com/Article/details/gecdfdtjp.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.blog.vehdjk.com/Article/details/gcwfjlaci.sHtML

[R70] 时间戳与互转
来源：http://baike.yfazqb.com/Article/details/grzrrxssk.sHtML

date +%s;  date -d @1700000000
来源：http://www.blog.tarul.cn/Article/details/guxrmwasx.sHtML

[R71] 日期格式化
来源：http://blog.bbcook.cn/Article/details/gqyoapjzt.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://mobile.yfazqb.com/Article/details/ghruhamek.sHtML

[R72] 等待端口就绪
来源：http://m.share.vehdjk.com/Article/details/gwewcluvw.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.blog.yfazqb.com/Article/details/gbkswbdze.sHtML

[R73] 分割大日志
来源：http://www.blog.fktsv.cn/Article/details/glzfdreob.sHtML

split -l 1000 big.log part_
来源：http://www.blog.yfazqb.com/Article/details/gthltzixk.sHtML

[R74] 批量重命名
来源：http://read.share.yfazqb.com/Article/details/gsbqoxvnm.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://3g.tarul.cn/Article/details/gpevbhpdy.sHtML

[R75] 导出环境变量
来源：http://3g.vehdjk.com/Article/details/gucrozeov.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://read.share.fktsv.cn/Article/details/gmndswfiv.sHtML

[R76] 使用临时文件
来源：http://read.share.fktsv.cn/Article/details/guxrxjssz.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://mobile.sjlbkw.cn/Article/details/gwghjjcwv.sHtML

[R77] 读取用户输入
来源：http://3g.bbcook.cn/Article/details/gsjutnedy.sHtML

read -rp "请输入: " ans
来源：http://m.share.yfazqb.com/Article/details/gxqyswzrm.sHtML

[R78] 交互式菜单
来源：http://baike.tarul.cn/Article/details/gzymhggcb.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://mobile.sjlbkw.cn/Article/details/gedzgvvge.sHtML

[R79] 解析命令行选项
来源：http://www.share.bbcook.cn/Article/details/gqcrwjwek.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://3g.epnwcf.com/Article/details/gzbjynfrg.sHtML

[R80] 查看脚本执行耗时
来源：http://m.share.epnwcf.com/Article/details/gsrxoslgm.sHtML

time ./run.sh
来源：http://mobile.bbcook.cn/Article/details/gxlekbvkm.sHtML

================================================================================
来源：http://www.share.vehdjk.com/Article/details/gkpfffipn.sHtML

S. C / C++ 专题
来源：http://mobile.tarul.cn/Article/details/gesvcefob.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/gfccupfid.sHtML

[S01] C：Hello World
来源：http://m.share.tarul.cn/Article/details/gxdgahrlm.sHtML

#include <stdio.h>
来源：http://www.share.fktsv.cn/Article/details/goobtdkzj.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://m.share.sjlbkw.cn/Article/details/glvgndmwl.sHtML

[S02] C：变量与格式化输出
来源：http://www.share.yfazqb.com/Article/details/gggbgtvnn.sHtML

int a = 10; printf("%d\n", a);
来源：http://read.share.sjlbkw.cn/Article/details/gafuavzwf.sHtML

[S03] C：读入整数
来源：http://mobile.sjlbkw.cn/Article/details/gufuhchuw.sHtML

int x; scanf("%d", &x);
来源：http://www.share.tarul.cn/Article/details/gpbywqdtz.sHtML

[S04] C：字符串复制
来源：http://www.blog.bbcook.cn/Article/details/geutrdbgd.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.share.epnwcf.com/Article/details/geozzwyns.sHtML

[S05] C：字符串长度
来源：http://read.share.vehdjk.com/Article/details/ghjpykdpy.sHtML

strlen(s)
来源：http://www.blog.bbcook.cn/Article/details/gjlxycvrc.sHtML

[S06] C：字符串比较
来源：http://baike.sjlbkw.cn/Article/details/gxvvdviqu.sHtML

strcmp(a, b) == 0
来源：http://blog.bbcook.cn/Article/details/gumjnzyca.sHtML

[S07] C：数组遍历求和
来源：http://www.share.fktsv.cn/Article/details/ghxnimvil.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.m.share.epnwcf.com/Article/details/grvxrqdjm.sHtML

[S08] C：动态内存分配与释放
来源：http://www.m.share.bbcook.cn/Article/details/gemurqahz.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://baike.sjlbkw.cn/Article/details/gowiwclwa.sHtML

[S09] C：结构体定义与初始化
来源：http://www.blog.bbcook.cn/Article/details/gijkejpbu.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://read.share.yfazqb.com/Article/details/gkecunicp.sHtML

[S10] C：指针与解引用
来源：http://www.m.share.tarul.cn/Article/details/gmbznemys.sHtML

int *p = &a;  *p = 5;
来源：http://m.share.sjlbkw.cn/Article/details/giwhwvoba.sHtML

[S11] C：逐行读文件
来源：http://m.share.vehdjk.com/Article/details/gsiahlesr.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://read.share.vehdjk.com/Article/details/gzgrldeki.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://baike.tarul.cn/Article/details/gtgqbrcxa.sHtML

fclose(f);
来源：http://m.share.epnwcf.com/Article/details/giscoqagy.sHtML

[S12] C：写文件
来源：http://read.share.bbcook.cn/Article/details/gbkchdpms.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.blog.bbcook.cn/Article/details/gfcdnctmp.sHtML

[S13] C：宏定义
来源：http://mobile.bbcook.cn/Article/details/gsrjcirvk.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.m.share.sjlbkw.cn/Article/details/gezyyahte.sHtML

[S14] C：枚举
来源：http://wap.epnwcf.com/Article/details/gxtvyumzz.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://baike.bbcook.cn/Article/details/gtudmdngj.sHtML

[S15] C：类型转换
来源：http://read.share.bbcook.cn/Article/details/griyecvod.sHtML

(double) a / b
来源：http://3g.yfazqb.com/Article/details/gypaldxeh.sHtML

[S16] C：位操作置位
来源：http://blog.vehdjk.com/Article/details/gfrdcscph.sHtML

x |= (1 << 3);
来源：http://www.m.share.tarul.cn/Article/details/gldybzgff.sHtML

[S17] C：安全拼接字符串
来源：http://read.share.vehdjk.com/Article/details/gtsucqfqq.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wap.yfazqb.com/Article/details/gumvkxbfy.sHtML

[S18] C：命令行参数
来源：http://www.share.yfazqb.com/Article/details/gimsrxuxj.sHtML

int main(int argc, char **argv)
来源：http://read.share.yfazqb.com/Article/details/gvhbkofkj.sHtML

[S19] C：快速排序
来源：http://read.share.bbcook.cn/Article/details/gszaftbbg.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://3g.fktsv.cn/Article/details/gprmjjhfs.sHtML

[S20] C：二分查找
来源：http://www.blog.yfazqb.com/Article/details/gppjrmdaf.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://mobile.sjlbkw.cn/Article/details/gecbafngp.sHtML

[S21] C：字符类别判断
来源：http://wap.yfazqb.com/Article/details/goymxmxag.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://wap.bbcook.cn/Article/details/gewnhzvxe.sHtML

[S22] C：字符串转数字
来源：http://baike.vehdjk.com/Article/details/gkjirooqw.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://read.share.bbcook.cn/Article/details/gtybcnbfa.sHtML

[S23] C：随机数
来源：http://read.share.tarul.cn/Article/details/ggnpqlnqw.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://m.share.tarul.cn/Article/details/gytgkjvqn.sHtML

[S24] C：获取本地时间
来源：http://baike.tarul.cn/Article/details/gbvoavjnd.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://mobile.tarul.cn/Article/details/gegmjleqs.sHtML

[S25] C：内存拷贝
来源：http://mobile.bbcook.cn/Article/details/grppzwolo.sHtML

memcpy(dst, src, n);
来源：http://baike.bbcook.cn/Article/details/gmdxlogha.sHtML

[S26] C：内存清零
来源：http://blog.fktsv.cn/Article/details/gqvedimeh.sHtML

memset(a, 0, sizeof a);
来源：http://www.share.tarul.cn/Article/details/ghyrkfdvv.sHtML

[S27] C：定义常量
来源：http://blog.bbcook.cn/Article/details/gdncajkbd.sHtML

const double PI = 3.14159;
来源：http://blog.sjlbkw.cn/Article/details/gqmrnijvq.sHtML

[S28] C：静态变量
来源：http://www.share.epnwcf.com/Article/details/gplibmncv.sHtML

static int counter = 0;
来源：http://read.share.fktsv.cn/Article/details/gyjaankml.sHtML

[S29] C：变参函数
来源：http://wap.bbcook.cn/Article/details/gpnpshrsn.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mobile.sjlbkw.cn/Article/details/gyanvrnvk.sHtML

[S30] C：头文件保护
来源：http://3g.vehdjk.com/Article/details/gyschgete.sHtML

#ifndef X_H
来源：http://www.m.share.tarul.cn/Article/details/gcwcfbtbm.sHtML

#define X_H
来源：http://3g.vehdjk.com/Article/details/gkplrsrbt.sHtML

#endif
来源：http://www.m.share.vehdjk.com/Article/details/gzuemppal.sHtML

[S31] C++：Hello World
来源：http://blog.tarul.cn/Article/details/gdwjbmjxh.sHtML

#include <iostream>
来源：http://read.share.fktsv.cn/Article/details/gkdtqqoiz.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.m.share.vehdjk.com/Article/details/gckuzlkjj.sHtML

[S32] C++：字符串
来源：http://www.m.share.vehdjk.com/Article/details/gdpechlyf.sHtML

std::string s = "hi";  s += "!";
来源：http://www.blog.tarul.cn/Article/details/goazkvcht.sHtML

[S33] C++：vector 增删
来源：http://blog.tarul.cn/Article/details/gpemybkfm.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://read.share.vehdjk.com/Article/details/gjcevyiii.sHtML

[S34] C++：遍历 vector
来源：http://blog.yfazqb.com/Article/details/gbnznswmr.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://wap.fktsv.cn/Article/details/gyctebydu.sHtML

[S35] C++：map
来源：http://www.share.sjlbkw.cn/Article/details/gapntqiav.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://blog.tarul.cn/Article/details/gkkctgqjk.sHtML

[S36] C++：unordered_map
来源：http://baike.yfazqb.com/Article/details/girkdxcnw.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://blog.fktsv.cn/Article/details/gjsgyndup.sHtML

[S37] C++：set
来源：http://3g.vehdjk.com/Article/details/gtzszkrrb.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://read.share.epnwcf.com/Article/details/grfddlhay.sHtML

[S38] C++：排序
来源：http://wap.yfazqb.com/Article/details/gbcxqegji.sHtML

std::sort(v.begin(), v.end());
来源：http://read.share.sjlbkw.cn/Article/details/gmeftdjcq.sHtML

[S39] C++：自定义比较器排序
来源：http://baike.fktsv.cn/Article/details/grjdzpxmo.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://read.share.epnwcf.com/Article/details/gdvachoxf.sHtML

[S40] C++：查找元素
来源：http://www.m.share.bbcook.cn/Article/details/gwjumncrm.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://mobile.fktsv.cn/Article/details/gtjkbmhji.sHtML

[S41] C++：类与构造函数
来源：http://baike.yfazqb.com/Article/details/gmmhqites.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://mobile.tarul.cn/Article/details/godkrzgkq.sHtML

[S42] C++：继承与虚函数
来源：http://www.m.share.fktsv.cn/Article/details/gonpajpqu.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.share.tarul.cn/Article/details/gnklwrbot.sHtML

[S43] C++：智能指针
来源：http://wap.bbcook.cn/Article/details/gvsckubeq.sHtML

auto p = std::make_unique<int>(5);
来源：http://wap.vehdjk.com/Article/details/gxolhvqeg.sHtML

[S44] C++：引用传参
来源：http://read.share.sjlbkw.cn/Article/details/gjhwskyjw.sHtML

void inc(int &x) { ++x; }
来源：http://www.m.share.epnwcf.com/Article/details/gpzyvthmm.sHtML

[S45] C++：lambda
来源：http://read.share.bbcook.cn/Article/details/gfcwbtxvt.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://mobile.epnwcf.com/Article/details/gyfwgehrl.sHtML

[S46] C++：函数模板
来源：http://baike.yfazqb.com/Article/details/gpegvzley.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://wap.yfazqb.com/Article/details/ggttfkvng.sHtML

[S47] C++：结构化绑定遍历
来源：http://wap.vehdjk.com/Article/details/glzrhcrbk.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://m.share.fktsv.cn/Article/details/gklzswxcg.sHtML

[S48] C++：逐行读文件
来源：http://wap.sjlbkw.cn/Article/details/gfdpspbko.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://wap.vehdjk.com/Article/details/gwiefnegr.sHtML

while (std::getline(in, line)) { }
来源：http://blog.bbcook.cn/Article/details/glzpjyzsm.sHtML

[S49] C++：写文件
来源：http://www.m.share.vehdjk.com/Article/details/gemqtbqea.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://mobile.bbcook.cn/Article/details/gshajnjbt.sHtML

[S50] C++：格式化数字
来源：http://3g.bbcook.cn/Article/details/gvosiqepk.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.m.share.fktsv.cn/Article/details/ghnnjftom.sHtML

[S51] C++：显式类型转换
来源：http://www.blog.tarul.cn/Article/details/gnjhyimge.sHtML

static_cast<double>(a) / b
来源：http://read.share.sjlbkw.cn/Article/details/gdhatnszb.sHtML

[S52] C++：const 与 noexcept
来源：http://www.share.vehdjk.com/Article/details/gidtvgqbt.sHtML

int size() const noexcept { return n_; }
来源：http://www.share.fktsv.cn/Article/details/gxbdguwyo.sHtML

[S53] C++：移动语义
来源：http://blog.yfazqb.com/Article/details/glhrrokxk.sHtML

std::vector<int> w = std::move(v);
来源：http://read.share.bbcook.cn/Article/details/gmbickvyb.sHtML

[S54] C++：异常处理
来源：http://read.share.vehdjk.com/Article/details/gjaxkmqqd.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://read.share.sjlbkw.cn/Article/details/gjpxvanxy.sHtML

[S55] C++：结构化绑定
来源：http://www.blog.epnwcf.com/Article/details/gmutwmozq.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://baike.sjlbkw.cn/Article/details/gdrjbxour.sHtML

[S56] C++：optional
来源：http://wap.vehdjk.com/Article/details/ghighnpcb.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wap.fktsv.cn/Article/details/geutsxesa.sHtML

[S57] C++：编译期常量
来源：http://read.share.fktsv.cn/Article/details/gskwcwbnn.sHtML

constexpr int N = 10;
来源：http://3g.tarul.cn/Article/details/grpabwjkp.sHtML

[S58] C++：命名空间
来源：http://www.blog.bbcook.cn/Article/details/gctfqzflo.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.m.share.yfazqb.com/Article/details/gdhiqjkvx.sHtML

[S59] C++：静态断言
来源：http://wap.bbcook.cn/Article/details/guzlqnpcs.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://blog.epnwcf.com/Article/details/grraopzvu.sHtML

[S60] C++：遍历并删除元素
来源：http://www.share.sjlbkw.cn/Article/details/gbpkkesic.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://wap.fktsv.cn/Article/details/gxumjfoih.sHtML

================================================================================
来源：http://www.share.sjlbkw.cn/Article/details/gsrkkkzmr.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.fktsv.cn/Article/details/gjiccfymi.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/giegwusou.sHtML

[T01] Kotlin：Hello World
来源：http://www.share.sjlbkw.cn/Article/details/gqqekgctj.sHtML

println("Hello")
来源：http://m.share.yfazqb.com/Article/details/goytmpttr.sHtML

[T02] Kotlin：变量
来源：http://3g.epnwcf.com/Article/details/giyvjposk.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://read.share.tarul.cn/Article/details/gyiojewlx.sHtML

[T03] Kotlin：字符串模板
来源：http://m.share.bbcook.cn/Article/details/gnwdjyate.sHtML

"值: $b"
来源：http://wap.yfazqb.com/Article/details/gylaunbsj.sHtML

[T04] Kotlin：空安全
来源：http://m.share.epnwcf.com/Article/details/gwmhnwedr.sHtML

val n: String? = null;  n?.length
来源：http://www.share.vehdjk.com/Article/details/gvtoyjjwu.sHtML

[T05] Kotlin：when 表达式
来源：http://read.share.sjlbkw.cn/Article/details/gleulixhd.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://m.share.epnwcf.com/Article/details/gwuknejuy.sHtML

[T06] Kotlin：集合映射
来源：http://www.m.share.fktsv.cn/Article/details/gwqheoccz.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://m.share.vehdjk.com/Article/details/gadenxrly.sHtML

[T07] Kotlin：集合过滤
来源：http://www.blog.vehdjk.com/Article/details/gcflkqpmm.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://mobile.sjlbkw.cn/Article/details/gihwfzuca.sHtML

[T08] Kotlin：数据类
来源：http://read.share.epnwcf.com/Article/details/gfyeveixw.sHtML

data class User(val name: String, val age: Int)
来源：http://read.share.yfazqb.com/Article/details/gklfnhvbs.sHtML

[T09] Kotlin：扩展函数
来源：http://www.blog.bbcook.cn/Article/details/gkmnvhczw.sHtML

fun String.exclaim() = this + "!"
来源：http://www.blog.fktsv.cn/Article/details/gqzfejxpk.sHtML

[T10] Kotlin：默认参数
来源：http://www.share.epnwcf.com/Article/details/gljhdaizy.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://wap.vehdjk.com/Article/details/gjnwxvxwe.sHtML

[T11] Kotlin：协程
来源：http://wap.bbcook.cn/Article/details/gcsraohhu.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://m.share.tarul.cn/Article/details/geovnkouh.sHtML

[T12] Kotlin：解构声明
来源：http://www.share.sjlbkw.cn/Article/details/gadjnvbjv.sHtML

val (a, b) = Pair(1, 2)
来源：http://read.share.vehdjk.com/Article/details/gjenruxxx.sHtML

[T13] Kotlin：只读 Map
来源：http://blog.sjlbkw.cn/Article/details/gtbzcozvu.sHtML

val m = mapOf("a" to 1)
来源：http://3g.bbcook.cn/Article/details/gahgeltuj.sHtML

[T14] Kotlin：循环
来源：http://www.m.share.tarul.cn/Article/details/gpjlfjkhp.sHtML

for (i in 1..10) println(i)
来源：http://3g.vehdjk.com/Article/details/gyfwhpvnt.sHtML

[T15] Kotlin：接口
来源：http://baike.vehdjk.com/Article/details/gqdrtizzt.sHtML

interface Shape { fun area(): Double }
来源：http://www.m.share.vehdjk.com/Article/details/gqukygquc.sHtML

[T16] Swift：Hello World
来源：http://www.m.share.tarul.cn/Article/details/gjydyminy.sHtML

print("Hello")
来源：http://baike.vehdjk.com/Article/details/genmkrnww.sHtML

[T17] Swift：变量与常量
来源：http://www.share.vehdjk.com/Article/details/gvbszmojl.sHtML

var a = 1;  let b = 2
来源：http://read.share.yfazqb.com/Article/details/gesclsxtu.sHtML

[T18] Swift：字符串插值
来源：http://www.blog.epnwcf.com/Article/details/gccyyciwi.sHtML

"值: \(b)"
来源：http://wap.fktsv.cn/Article/details/gygdrmtci.sHtML

[T19] Swift：可选绑定
来源：http://www.blog.fktsv.cn/Article/details/gwymiyxhu.sHtML

if let n = opt { print(n) }
来源：http://3g.yfazqb.com/Article/details/gmddahwkp.sHtML

[T20] Swift：数组操作
来源：http://m.share.yfazqb.com/Article/details/gbksoqbsb.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://blog.fktsv.cn/Article/details/gfodkbsse.sHtML


<!-- 参考信息 -->