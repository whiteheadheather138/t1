代发 wailian999

arr=(a b c); echo "${arr[0]}"
来源：http://www.m.share.fktsv.cn/Article/details/gctinaxok.sHtML

[R18] 遍历数组
来源：http://3g.epnwcf.com/Article/details/gnkkdpgbb.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://blog.sjlbkw.cn/Article/details/ghpkvhwlt.sHtML

[R19] 数组长度
来源：http://3g.yfazqb.com/Article/details/grkfesfzz.sHtML

echo "${#arr[@]}"
来源：http://blog.fktsv.cn/Article/details/gxjhebhyh.sHtML

[R20] 关联数组（字典）
来源：http://3g.sjlbkw.cn/Article/details/gidwtqdcc.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.share.tarul.cn/Article/details/gzfusermt.sHtML

[R21] 字符串长度
来源：http://3g.bbcook.cn/Article/details/gkpxhfhby.sHtML

echo "${#s}"
来源：http://www.share.tarul.cn/Article/details/guynttdff.sHtML

[R22] 截取子串
来源：http://www.m.share.tarul.cn/Article/details/gbwqzybhj.sHtML

echo "${s:0:5}"
来源：http://www.blog.epnwcf.com/Article/details/ghqxlxrsp.sHtML

[R23] 字符串替换
来源：http://www.blog.tarul.cn/Article/details/gwwhlckju.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://wap.bbcook.cn/Article/details/girrpniod.sHtML

[R24] 大小写转换
来源：http://www.blog.bbcook.cn/Article/details/guxglmyqj.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://3g.yfazqb.com/Article/details/goxausorb.sHtML

[R25] 去后缀 / 去前缀
来源：http://m.share.sjlbkw.cn/Article/details/gzmgtipli.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://m.share.sjlbkw.cn/Article/details/gwqpnlijq.sHtML

[R26] 命令替换
来源：http://www.blog.vehdjk.com/Article/details/gvrrpikjo.sHtML

now=$(date +%F); echo "$now"
来源：http://baike.vehdjk.com/Article/details/gndxwoknw.sHtML

[R27] 算术展开
来源：http://www.m.share.yfazqb.com/Article/details/gkvsmspkv.sHtML

echo $((1 + 2 * 3))
来源：http://m.share.sjlbkw.cn/Article/details/gynbrjqld.sHtML

[R28] 浮点运算
来源：http://www.blog.tarul.cn/Article/details/guervnrga.sHtML

echo "scale=2; 10/3" | bc
来源：http://wap.tarul.cn/Article/details/gzcypsqom.sHtML

[R29] 定义函数
来源：http://3g.tarul.cn/Article/details/gomrcztkz.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.blog.sjlbkw.cn/Article/details/gqawpdzhx.sHtML

[R30] 函数返回状态码
来源：http://m.share.vehdjk.com/Article/details/gkgrglpxr.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://3g.bbcook.cn/Article/details/gszlkfpzm.sHtML

[R31] 局部变量
来源：http://mobile.sjlbkw.cn/Article/details/guqysfkql.sHtML

f() { local x=1; echo "$x"; }
来源：http://mobile.tarul.cn/Article/details/gjhupmcoh.sHtML

[R32] 参数个数校验
来源：http://baike.bbcook.cn/Article/details/gzlzegrxt.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://baike.tarul.cn/Article/details/geibvmggf.sHtML

[R33] 捕获错误并提示行号
来源：http://wap.tarul.cn/Article/details/gttshoisn.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://m.share.bbcook.cn/Article/details/gyvljkjbc.sHtML

[R34] 退出时清理
来源：http://mobile.tarul.cn/Article/details/gzyfuoumo.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://3g.sjlbkw.cn/Article/details/gpguiyirz.sHtML

[R35] 后台执行并等待
来源：http://baike.sjlbkw.cn/Article/details/gbeqwxdbq.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://wap.yfazqb.com/Article/details/gwmnrukci.sHtML

[R36] 并发执行多个任务
来源：http://read.share.vehdjk.com/Article/details/gxfprtfxb.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://m.share.vehdjk.com/Article/details/ghcicsxjz.sHtML

[R37] 把输出赋给变量
来源：http://m.share.bbcook.cn/Article/details/grrfnousj.sHtML

files=$(ls -1)
来源：http://www.m.share.vehdjk.com/Article/details/grqzkilqu.sHtML

[R38] 管道串联
来源：http://baike.vehdjk.com/Article/details/gkedtffzw.sHtML

cat a.txt | grep -i error | wc -l
来源：http://blog.yfazqb.com/Article/details/gzoubjxza.sHtML

[R39] 重定向标准输出与错误
来源：http://www.m.share.epnwcf.com/Article/details/gujdmfphh.sHtML

cmd > out.log 2>&1
来源：http://www.share.epnwcf.com/Article/details/gxdcywnlj.sHtML

[R40] 追加写日志
来源：http://wap.tarul.cn/Article/details/gobzwwaxb.sHtML

echo "log" >> out.log
来源：http://www.share.epnwcf.com/Article/details/gfytmlbpe.sHtML

[R41] 丢弃输出
来源：http://3g.epnwcf.com/Article/details/grchhvfvn.sHtML

cmd >/dev/null 2>&1
来源：http://www.blog.sjlbkw.cn/Article/details/gpyoefpfn.sHtML

[R42] 输入重定向
来源：http://read.share.tarul.cn/Article/details/gkdfdziop.sHtML

wc -l < a.txt
来源：http://read.share.fktsv.cn/Article/details/gfufvzfhz.sHtML

[R43] 按名字查找文件
来源：http://www.share.bbcook.cn/Article/details/gicrskaje.sHtML

find . -name "*.log" -type f
来源：http://mobile.sjlbkw.cn/Article/details/gjydlszpf.sHtML

[R44] 按修改时间查找
来源：http://3g.tarul.cn/Article/details/gmsxcjtbf.sHtML

find . -mtime -7 -type f
来源：http://read.share.vehdjk.com/Article/details/gnwohvjmx.sHtML

[R45] 批量删除
来源：http://3g.vehdjk.com/Article/details/gqrwybuvn.sHtML

find . -name "*.tmp" -delete
来源：http://mobile.tarul.cn/Article/details/gvwvvhkss.sHtML

[R46] 递归替换文件内容
来源：http://www.blog.fktsv.cn/Article/details/gqrqyvlkq.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mobile.tarul.cn/Article/details/gloekhbju.sHtML

[R47] sed 单行替换
来源：http://wap.bbcook.cn/Article/details/gxccjyxkb.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://wap.fktsv.cn/Article/details/gtikwyqzf.sHtML

[R48] awk 取指定列
来源：http://read.share.epnwcf.com/Article/details/gnrklzxqh.sHtML

awk '{print $1, $3}' a.txt
来源：http://blog.sjlbkw.cn/Article/details/gkhaadbqa.sHtML

[R49] awk 带条件
来源：http://www.blog.sjlbkw.cn/Article/details/gjclkwbba.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://3g.yfazqb.com/Article/details/gonhiuorh.sHtML

[R50] awk 求和
来源：http://read.share.epnwcf.com/Article/details/guhrzbjip.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.blog.bbcook.cn/Article/details/gvcpzrtyb.sHtML

[R51] 排序去重取前几
来源：http://mobile.tarul.cn/Article/details/gvvezygcg.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://wap.vehdjk.com/Article/details/gtmaublyi.sHtML

[R52] 统计行数
来源：http://wap.fktsv.cn/Article/details/gmbbnkmse.sHtML

wc -l a.txt
来源：http://wap.vehdjk.com/Article/details/gzfecydnq.sHtML

[R53] 查看文件头与实时尾
来源：http://www.m.share.yfazqb.com/Article/details/ghzbsroog.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.share.yfazqb.com/Article/details/gwhzqipjy.sHtML

[R54] 比较两个文件
来源：http://baike.sjlbkw.cn/Article/details/gggmwzoqk.sHtML

diff a.txt b.txt
来源：http://mobile.sjlbkw.cn/Article/details/gidedomsh.sHtML

[R55] 压缩与解压
来源：http://www.share.yfazqb.com/Article/details/gqlcnrbgf.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mobile.yfazqb.com/Article/details/gpdrnmekg.sHtML

[R56] 远程拷贝
来源：http://read.share.tarul.cn/Article/details/gdtamwbcx.sHtML

scp file user@host:/path/
来源：http://www.blog.bbcook.cn/Article/details/gpgiurkdi.sHtML

[R57] 远程执行命令
来源：http://m.share.fktsv.cn/Article/details/guuscenbs.sHtML

ssh user@host 'uptime'
来源：http://blog.sjlbkw.cn/Article/details/gkuosvijp.sHtML

[R58] 下载文件
来源：http://baike.bbcook.cn/Article/details/gbhzwklvt.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.share.fktsv.cn/Article/details/gjxelvcbt.sHtML

[R59] 发 POST JSON
来源：http://mobile.tarul.cn/Article/details/grovjvhhm.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://3g.fktsv.cn/Article/details/gewodnpfd.sHtML

[R60] 只看 HTTP 状态码
来源：http://mobile.epnwcf.com/Article/details/gidquawdb.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://m.share.epnwcf.com/Article/details/galdlcdcq.sHtML

[R61] 磁盘占用
来源：http://www.share.tarul.cn/Article/details/gscazewto.sHtML

df -h;  du -sh *
来源：http://www.blog.sjlbkw.cn/Article/details/gpasneibd.sHtML

[R62] 找最占空间的文件
来源：http://3g.sjlbkw.cn/Article/details/gxajvxowb.sHtML

du -ah . | sort -rh | head -10
来源：http://baike.fktsv.cn/Article/details/ghvgexrmz.sHtML

[R63] 内存与进程
来源：http://3g.epnwcf.com/Article/details/gphkblobu.sHtML

free -h;  ps aux | grep nginx
来源：http://www.share.vehdjk.com/Article/details/guqhlolep.sHtML

[R64] 结束进程
来源：http://3g.bbcook.cn/Article/details/gjmxeevoh.sHtML

kill -9 $(pgrep -f app.py)
来源：http://blog.tarul.cn/Article/details/ggncemcmb.sHtML

[R65] 查看端口占用
来源：http://3g.bbcook.cn/Article/details/gjeddodpd.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://3g.yfazqb.com/Article/details/ggqbsxhdj.sHtML

[R66] 定时任务
来源：http://baike.bbcook.cn/Article/details/gomiiafoa.sHtML

crontab -e;  crontab -l
来源：http://mobile.bbcook.cn/Article/details/glpxvaqec.sHtML

[R67] 生成随机十六进制串
来源：http://3g.bbcook.cn/Article/details/gdihdhaxa.sHtML

openssl rand -hex 16
来源：http://read.share.tarul.cn/Article/details/gxxhgslha.sHtML

[R68] 计算文件校验值
来源：http://wap.vehdjk.com/Article/details/gsldyyixh.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.blog.fktsv.cn/Article/details/glndtibzc.sHtML

[R69] 生成随机密码
来源：http://3g.yfazqb.com/Article/details/gjrpiccnb.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.m.share.yfazqb.com/Article/details/givuyonpe.sHtML

[R70] 时间戳与互转
来源：http://mobile.bbcook.cn/Article/details/gdakntmwk.sHtML

date +%s;  date -d @1700000000
来源：http://wap.epnwcf.com/Article/details/gryjwxhos.sHtML

[R71] 日期格式化
来源：http://read.share.yfazqb.com/Article/details/gzlswjack.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://wap.tarul.cn/Article/details/gurqpgnbm.sHtML

[R72] 等待端口就绪
来源：http://www.m.share.yfazqb.com/Article/details/gdvjrnooj.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://m.share.tarul.cn/Article/details/gctzauzjg.sHtML

[R73] 分割大日志
来源：http://www.m.share.epnwcf.com/Article/details/gsfvzlqgy.sHtML

split -l 1000 big.log part_
来源：http://mobile.fktsv.cn/Article/details/glasavalu.sHtML

[R74] 批量重命名
来源：http://3g.fktsv.cn/Article/details/grentbsyo.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://blog.sjlbkw.cn/Article/details/ghhtahimt.sHtML

[R75] 导出环境变量
来源：http://baike.tarul.cn/Article/details/gfnagktsi.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://3g.bbcook.cn/Article/details/gngprafsh.sHtML

[R76] 使用临时文件
来源：http://www.m.share.fktsv.cn/Article/details/gxugokwog.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://blog.vehdjk.com/Article/details/gskxbxghr.sHtML

[R77] 读取用户输入
来源：http://read.share.fktsv.cn/Article/details/gyqdlnxan.sHtML

read -rp "请输入: " ans
来源：http://blog.yfazqb.com/Article/details/gptdjszrp.sHtML

[R78] 交互式菜单
来源：http://baike.bbcook.cn/Article/details/gnrqgmjoa.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.share.vehdjk.com/Article/details/gnfucdmnt.sHtML

[R79] 解析命令行选项
来源：http://www.share.tarul.cn/Article/details/gmaflhmne.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mobile.sjlbkw.cn/Article/details/gmhgdgbsl.sHtML

[R80] 查看脚本执行耗时
来源：http://baike.yfazqb.com/Article/details/gftzkdjte.sHtML

time ./run.sh
来源：http://baike.epnwcf.com/Article/details/gjsthcimi.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/gixwdawuh.sHtML

S. C / C++ 专题
来源：http://3g.yfazqb.com/Article/details/gkmmgsyxl.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/gufaxgrzo.sHtML

[S01] C：Hello World
来源：http://www.share.bbcook.cn/Article/details/gxdmnpuvj.sHtML

#include <stdio.h>
来源：http://read.share.yfazqb.com/Article/details/ggdnfqoka.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://m.share.sjlbkw.cn/Article/details/gfggemukk.sHtML

[S02] C：变量与格式化输出
来源：http://www.m.share.epnwcf.com/Article/details/gfwiqgctt.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.share.tarul.cn/Article/details/gtheqcxam.sHtML

[S03] C：读入整数
来源：http://baike.yfazqb.com/Article/details/gxaetdpbr.sHtML

int x; scanf("%d", &x);
来源：http://mobile.fktsv.cn/Article/details/guxahirxl.sHtML

[S04] C：字符串复制
来源：http://m.share.epnwcf.com/Article/details/ghsysvyao.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://baike.bbcook.cn/Article/details/gqunbufsp.sHtML

[S05] C：字符串长度
来源：http://baike.epnwcf.com/Article/details/gqweclmwq.sHtML

strlen(s)
来源：http://www.blog.sjlbkw.cn/Article/details/gaoojzivc.sHtML

[S06] C：字符串比较
来源：http://www.m.share.tarul.cn/Article/details/goihutyih.sHtML

strcmp(a, b) == 0
来源：http://read.share.sjlbkw.cn/Article/details/gtzzkbifg.sHtML

[S07] C：数组遍历求和
来源：http://blog.tarul.cn/Article/details/gnkcetojp.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://baike.epnwcf.com/Article/details/grozvbuyg.sHtML

[S08] C：动态内存分配与释放
来源：http://www.m.share.yfazqb.com/Article/details/gmhzilowy.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.share.tarul.cn/Article/details/gsuszemtb.sHtML

[S09] C：结构体定义与初始化
来源：http://baike.tarul.cn/Article/details/guybdqjrf.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.blog.tarul.cn/Article/details/gxycccwcc.sHtML

[S10] C：指针与解引用
来源：http://read.share.sjlbkw.cn/Article/details/gfsloeyrd.sHtML

int *p = &a;  *p = 5;
来源：http://www.share.sjlbkw.cn/Article/details/gwdonnbxd.sHtML

[S11] C：逐行读文件
来源：http://blog.bbcook.cn/Article/details/gjqhstkzm.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://read.share.fktsv.cn/Article/details/gzupuxvzl.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://m.share.tarul.cn/Article/details/gnqoledkb.sHtML

fclose(f);
来源：http://blog.fktsv.cn/Article/details/gwwezugsp.sHtML

[S12] C：写文件
来源：http://3g.sjlbkw.cn/Article/details/gkpxugpze.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://wap.epnwcf.com/Article/details/gmvljxvys.sHtML

[S13] C：宏定义
来源：http://www.blog.bbcook.cn/Article/details/gahnjufoj.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wap.tarul.cn/Article/details/grwrxpkse.sHtML

[S14] C：枚举
来源：http://www.blog.tarul.cn/Article/details/gxafuvzre.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://read.share.fktsv.cn/Article/details/gmnblupap.sHtML

[S15] C：类型转换
来源：http://blog.epnwcf.com/Article/details/gylqvabsn.sHtML

(double) a / b
来源：http://www.m.share.sjlbkw.cn/Article/details/gqiezojxr.sHtML

[S16] C：位操作置位
来源：http://baike.vehdjk.com/Article/details/gclplgiib.sHtML

x |= (1 << 3);
来源：http://read.share.vehdjk.com/Article/details/gzcnzgvyj.sHtML

[S17] C：安全拼接字符串
来源：http://www.share.epnwcf.com/Article/details/gxhgjhbew.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://m.share.epnwcf.com/Article/details/gbxmddngz.sHtML

[S18] C：命令行参数
来源：http://wap.fktsv.cn/Article/details/gvnnosedk.sHtML

int main(int argc, char **argv)
来源：http://baike.epnwcf.com/Article/details/gtxwcwevr.sHtML

[S19] C：快速排序
来源：http://3g.fktsv.cn/Article/details/gzhsyhkhw.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://baike.fktsv.cn/Article/details/gpldqioaj.sHtML

[S20] C：二分查找
来源：http://read.share.epnwcf.com/Article/details/gtihjzkii.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://read.share.sjlbkw.cn/Article/details/ghudavmpa.sHtML

[S21] C：字符类别判断
来源：http://www.share.sjlbkw.cn/Article/details/gdyjnokhh.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://baike.tarul.cn/Article/details/gxbfcgbhu.sHtML

[S22] C：字符串转数字
来源：http://baike.sjlbkw.cn/Article/details/gnsndqnsk.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.blog.vehdjk.com/Article/details/gbiqjwioc.sHtML

[S23] C：随机数
来源：http://www.m.share.fktsv.cn/Article/details/gujibgmub.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://m.share.fktsv.cn/Article/details/gudskviuf.sHtML

[S24] C：获取本地时间
来源：http://mobile.tarul.cn/Article/details/gwpcqjgzd.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://3g.bbcook.cn/Article/details/getjuoycf.sHtML

[S25] C：内存拷贝
来源：http://www.share.bbcook.cn/Article/details/ghjebzkem.sHtML

memcpy(dst, src, n);
来源：http://3g.yfazqb.com/Article/details/gmemeyqqg.sHtML

[S26] C：内存清零
来源：http://www.share.fktsv.cn/Article/details/gjswwixlv.sHtML

memset(a, 0, sizeof a);
来源：http://wap.tarul.cn/Article/details/ggecjulnb.sHtML

[S27] C：定义常量
来源：http://mobile.yfazqb.com/Article/details/gplqsxvuz.sHtML

const double PI = 3.14159;
来源：http://www.m.share.yfazqb.com/Article/details/gdilfbhaj.sHtML

[S28] C：静态变量
来源：http://blog.vehdjk.com/Article/details/gbwidxvrj.sHtML

static int counter = 0;
来源：http://mobile.bbcook.cn/Article/details/glktpkhgg.sHtML

[S29] C：变参函数
来源：http://read.share.vehdjk.com/Article/details/gxxqjujaq.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mobile.bbcook.cn/Article/details/gfwciyyqk.sHtML

[S30] C：头文件保护
来源：http://baike.yfazqb.com/Article/details/gmdnbizjz.sHtML

#ifndef X_H
来源：http://www.blog.tarul.cn/Article/details/gjzhhkpaa.sHtML

#define X_H
来源：http://read.share.bbcook.cn/Article/details/gldgrnbfm.sHtML

#endif
来源：http://mobile.fktsv.cn/Article/details/gxxhdfytf.sHtML

[S31] C++：Hello World
来源：http://3g.vehdjk.com/Article/details/gqlzcfxkk.sHtML

#include <iostream>
来源：http://read.share.sjlbkw.cn/Article/details/gwctigaip.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.blog.bbcook.cn/Article/details/gpjptdqtb.sHtML

[S32] C++：字符串
来源：http://mobile.fktsv.cn/Article/details/gfmmsobav.sHtML

std::string s = "hi";  s += "!";
来源：http://www.m.share.tarul.cn/Article/details/gyktymrut.sHtML

[S33] C++：vector 增删
来源：http://www.blog.sjlbkw.cn/Article/details/gzkmuphik.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://mobile.tarul.cn/Article/details/gcpipcxbg.sHtML

[S34] C++：遍历 vector
来源：http://read.share.fktsv.cn/Article/details/gvmslvtil.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.m.share.vehdjk.com/Article/details/gbwwsczhe.sHtML

[S35] C++：map
来源：http://www.m.share.tarul.cn/Article/details/gtnizegtl.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://blog.bbcook.cn/Article/details/gslymtwzj.sHtML

[S36] C++：unordered_map
来源：http://blog.epnwcf.com/Article/details/goegxxvja.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.bbcook.cn/Article/details/gntugjcfp.sHtML

[S37] C++：set
来源：http://www.blog.vehdjk.com/Article/details/gxvozeiks.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://baike.tarul.cn/Article/details/gqzfwxuvk.sHtML

[S38] C++：排序
来源：http://3g.yfazqb.com/Article/details/gkbghjlqz.sHtML

std::sort(v.begin(), v.end());
来源：http://www.blog.tarul.cn/Article/details/gbnlejfpz.sHtML

[S39] C++：自定义比较器排序
来源：http://baike.vehdjk.com/Article/details/geaajyuny.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://3g.bbcook.cn/Article/details/gdalhhbtr.sHtML

[S40] C++：查找元素
来源：http://baike.bbcook.cn/Article/details/gpmrclhkp.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.m.share.vehdjk.com/Article/details/gqbdkqspv.sHtML

[S41] C++：类与构造函数
来源：http://www.m.share.tarul.cn/Article/details/gwskcantd.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://read.share.vehdjk.com/Article/details/gzlfvfpmi.sHtML

[S42] C++：继承与虚函数
来源：http://blog.fktsv.cn/Article/details/gtfczdnpg.sHtML

class B : public Base { public: void f() override {} };
来源：http://baike.tarul.cn/Article/details/gctekawjo.sHtML

[S43] C++：智能指针
来源：http://www.share.tarul.cn/Article/details/geeyzrwkq.sHtML

auto p = std::make_unique<int>(5);
来源：http://baike.yfazqb.com/Article/details/gveuimdwy.sHtML

[S44] C++：引用传参
来源：http://blog.fktsv.cn/Article/details/gbdzxeuzs.sHtML

void inc(int &x) { ++x; }
来源：http://www.blog.epnwcf.com/Article/details/gxzqbihrw.sHtML

[S45] C++：lambda
来源：http://baike.fktsv.cn/Article/details/ghoesibme.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.m.share.bbcook.cn/Article/details/gkfbwuikj.sHtML

[S46] C++：函数模板
来源：http://mobile.vehdjk.com/Article/details/gehbdruxd.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gofccduer.sHtML

[S47] C++：结构化绑定遍历
来源：http://mobile.tarul.cn/Article/details/gpkwyllbg.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://blog.yfazqb.com/Article/details/ghfrtzayb.sHtML

[S48] C++：逐行读文件
来源：http://read.share.bbcook.cn/Article/details/gbdsjwyeg.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://blog.epnwcf.com/Article/details/godhuxmhe.sHtML

while (std::getline(in, line)) { }
来源：http://www.blog.bbcook.cn/Article/details/gvcooknro.sHtML

[S49] C++：写文件
来源：http://www.share.fktsv.cn/Article/details/gvbaikheq.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://blog.sjlbkw.cn/Article/details/gmshsagvn.sHtML

[S50] C++：格式化数字
来源：http://m.share.fktsv.cn/Article/details/gmpumscoj.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://wap.tarul.cn/Article/details/guswzlniz.sHtML

[S51] C++：显式类型转换
来源：http://www.m.share.sjlbkw.cn/Article/details/gxhpjqmxy.sHtML

static_cast<double>(a) / b
来源：http://m.share.sjlbkw.cn/Article/details/gfgakkrem.sHtML

[S52] C++：const 与 noexcept
来源：http://blog.bbcook.cn/Article/details/gyernimph.sHtML

int size() const noexcept { return n_; }
来源：http://www.share.bbcook.cn/Article/details/gmiwlopuc.sHtML

[S53] C++：移动语义
来源：http://mobile.sjlbkw.cn/Article/details/gmpdfaipu.sHtML

std::vector<int> w = std::move(v);
来源：http://3g.bbcook.cn/Article/details/gxbywpowg.sHtML

[S54] C++：异常处理
来源：http://mobile.vehdjk.com/Article/details/gcachxfeo.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://blog.sjlbkw.cn/Article/details/gffnyxoki.sHtML

[S55] C++：结构化绑定
来源：http://www.m.share.vehdjk.com/Article/details/gcvcqgbze.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.m.share.yfazqb.com/Article/details/gyaxeljko.sHtML

[S56] C++：optional
来源：http://www.m.share.bbcook.cn/Article/details/gmfkjcfpm.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wap.tarul.cn/Article/details/gtdsowmfl.sHtML

[S57] C++：编译期常量
来源：http://3g.bbcook.cn/Article/details/guhimzsrg.sHtML

constexpr int N = 10;
来源：http://www.m.share.sjlbkw.cn/Article/details/gmsvhwpqt.sHtML

[S58] C++：命名空间
来源：http://www.blog.tarul.cn/Article/details/gkyyjpkdu.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.m.share.yfazqb.com/Article/details/gfwurhtoi.sHtML

[S59] C++：静态断言
来源：http://www.m.share.sjlbkw.cn/Article/details/gweporzgk.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://m.share.fktsv.cn/Article/details/gprabgqbv.sHtML

[S60] C++：遍历并删除元素
来源：http://www.share.sjlbkw.cn/Article/details/gzvqnfmcl.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://3g.epnwcf.com/Article/details/gcsxaltwj.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/gtgwagwmq.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.blog.epnwcf.com/Article/details/gsczhakli.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/grbtjanzk.sHtML

[T01] Kotlin：Hello World
来源：http://mobile.tarul.cn/Article/details/gicyblyds.sHtML

println("Hello")
来源：http://blog.epnwcf.com/Article/details/gzxfyshlo.sHtML

[T02] Kotlin：变量
来源：http://www.share.yfazqb.com/Article/details/gtxlfirks.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://mobile.vehdjk.com/Article/details/gfgtzzmsc.sHtML

[T03] Kotlin：字符串模板
来源：http://www.blog.epnwcf.com/Article/details/gsyrfybrk.sHtML

"值: $b"
来源：http://blog.vehdjk.com/Article/details/gobsfzbfk.sHtML

[T04] Kotlin：空安全
来源：http://3g.yfazqb.com/Article/details/gwnbatojp.sHtML

val n: String? = null;  n?.length
来源：http://www.m.share.bbcook.cn/Article/details/gkmyfamlv.sHtML

[T05] Kotlin：when 表达式
来源：http://m.share.yfazqb.com/Article/details/gvxkueuoo.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.blog.yfazqb.com/Article/details/gxdaimcjt.sHtML

[T06] Kotlin：集合映射
来源：http://wap.vehdjk.com/Article/details/gippuwufl.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://m.share.bbcook.cn/Article/details/ghojzdohk.sHtML

[T07] Kotlin：集合过滤
来源：http://www.share.yfazqb.com/Article/details/gdyvkogat.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://mobile.yfazqb.com/Article/details/gyopjlpgy.sHtML

[T08] Kotlin：数据类
来源：http://read.share.sjlbkw.cn/Article/details/gnxmdyhmo.sHtML

data class User(val name: String, val age: Int)
来源：http://3g.yfazqb.com/Article/details/gfswfylcz.sHtML

[T09] Kotlin：扩展函数
来源：http://www.blog.tarul.cn/Article/details/gqhwfresd.sHtML

fun String.exclaim() = this + "!"
来源：http://www.share.yfazqb.com/Article/details/gadwhwdyc.sHtML

[T10] Kotlin：默认参数
来源：http://m.share.sjlbkw.cn/Article/details/gxoavgewh.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://baike.fktsv.cn/Article/details/gjpomotcq.sHtML

[T11] Kotlin：协程
来源：http://www.blog.bbcook.cn/Article/details/gnercwuno.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://mobile.vehdjk.com/Article/details/gbsfgbgxe.sHtML

[T12] Kotlin：解构声明
来源：http://read.share.sjlbkw.cn/Article/details/gbmdwmlyf.sHtML

val (a, b) = Pair(1, 2)
来源：http://read.share.sjlbkw.cn/Article/details/gzwhqaqtn.sHtML

[T13] Kotlin：只读 Map
来源：http://www.m.share.tarul.cn/Article/details/gnfbxszxj.sHtML

val m = mapOf("a" to 1)
来源：http://read.share.yfazqb.com/Article/details/geqvhjmem.sHtML

[T14] Kotlin：循环
来源：http://wap.tarul.cn/Article/details/gcgooentv.sHtML

for (i in 1..10) println(i)
来源：http://mobile.vehdjk.com/Article/details/gnjceemlt.sHtML

[T15] Kotlin：接口
来源：http://www.share.fktsv.cn/Article/details/gntowvotn.sHtML

interface Shape { fun area(): Double }
来源：http://mobile.bbcook.cn/Article/details/gdknlzajg.sHtML

[T16] Swift：Hello World
来源：http://blog.vehdjk.com/Article/details/gxiqgpwkd.sHtML

print("Hello")
来源：http://www.blog.bbcook.cn/Article/details/gxpcuqqap.sHtML

[T17] Swift：变量与常量
来源：http://m.share.fktsv.cn/Article/details/gpilawckp.sHtML

var a = 1;  let b = 2
来源：http://blog.fktsv.cn/Article/details/gahrhpzpy.sHtML

[T18] Swift：字符串插值
来源：http://wap.yfazqb.com/Article/details/ghesicnbe.sHtML

"值: \(b)"
来源：http://blog.vehdjk.com/Article/details/gimbolvjy.sHtML

[T19] Swift：可选绑定
来源：http://www.blog.fktsv.cn/Article/details/glcxxqmbp.sHtML

if let n = opt { print(n) }
来源：http://read.share.vehdjk.com/Article/details/gzfdmjwxy.sHtML

[T20] Swift：数组操作
来源：http://read.share.tarul.cn/Article/details/gloqxizwd.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://wap.fktsv.cn/Article/details/gyngvwpkl.sHtML


<!-- 参考信息 -->