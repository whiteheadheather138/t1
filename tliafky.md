代发 wailian999

echo $((1 + 2 * 3))
来源：http://www.blog.epnwcf.com/Article/details/gcznlhxtb.sHtML

[R28] 浮点运算
来源：http://www.blog.fktsv.cn/Article/details/guvrmiwkz.sHtML

echo "scale=2; 10/3" | bc
来源：http://3g.vehdjk.com/Article/details/gypsdrmiw.sHtML

[R29] 定义函数
来源：http://baike.bbcook.cn/Article/details/gmaqsqtfh.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://blog.fktsv.cn/Article/details/gdjmkxtru.sHtML

[R30] 函数返回状态码
来源：http://read.share.yfazqb.com/Article/details/gmbdkykwd.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://baike.bbcook.cn/Article/details/gftrrwpbf.sHtML

[R31] 局部变量
来源：http://blog.tarul.cn/Article/details/gfonlfkoi.sHtML

f() { local x=1; echo "$x"; }
来源：http://m.share.sjlbkw.cn/Article/details/gekoxiujl.sHtML

[R32] 参数个数校验
来源：http://wap.tarul.cn/Article/details/gwxzqiowk.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://mobile.bbcook.cn/Article/details/gyxenntnf.sHtML

[R33] 捕获错误并提示行号
来源：http://mobile.bbcook.cn/Article/details/gtjhqwknm.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.m.share.epnwcf.com/Article/details/gwmwgipwy.sHtML

[R34] 退出时清理
来源：http://m.share.epnwcf.com/Article/details/gaayweoxw.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://blog.yfazqb.com/Article/details/gksazvukv.sHtML

[R35] 后台执行并等待
来源：http://www.blog.epnwcf.com/Article/details/gfobddltu.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://mobile.vehdjk.com/Article/details/ggeovjphr.sHtML

[R36] 并发执行多个任务
来源：http://read.share.vehdjk.com/Article/details/gikowpvmw.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.blog.fktsv.cn/Article/details/gesgvjtyy.sHtML

[R37] 把输出赋给变量
来源：http://wap.yfazqb.com/Article/details/gakdcspvd.sHtML

files=$(ls -1)
来源：http://blog.vehdjk.com/Article/details/gmvgeoflb.sHtML

[R38] 管道串联
来源：http://www.blog.yfazqb.com/Article/details/gfpdlkgcp.sHtML

cat a.txt | grep -i error | wc -l
来源：http://wap.tarul.cn/Article/details/gjcjkzdqm.sHtML

[R39] 重定向标准输出与错误
来源：http://read.share.bbcook.cn/Article/details/gubdacqzq.sHtML

cmd > out.log 2>&1
来源：http://3g.yfazqb.com/Article/details/gvdqnamib.sHtML

[R40] 追加写日志
来源：http://3g.bbcook.cn/Article/details/gtawxyalt.sHtML

echo "log" >> out.log
来源：http://wap.sjlbkw.cn/Article/details/gbffaznjj.sHtML

[R41] 丢弃输出
来源：http://read.share.sjlbkw.cn/Article/details/gmdhdhmjp.sHtML

cmd >/dev/null 2>&1
来源：http://read.share.sjlbkw.cn/Article/details/gzspomgcp.sHtML

[R42] 输入重定向
来源：http://mobile.vehdjk.com/Article/details/ghhqxrbnm.sHtML

wc -l < a.txt
来源：http://www.blog.vehdjk.com/Article/details/ghwxvfzcr.sHtML

[R43] 按名字查找文件
来源：http://www.m.share.yfazqb.com/Article/details/gaulkdhnv.sHtML

find . -name "*.log" -type f
来源：http://m.share.sjlbkw.cn/Article/details/geftffhvi.sHtML

[R44] 按修改时间查找
来源：http://3g.bbcook.cn/Article/details/gachsdypw.sHtML

find . -mtime -7 -type f
来源：http://wap.sjlbkw.cn/Article/details/gldlaywim.sHtML

[R45] 批量删除
来源：http://mobile.yfazqb.com/Article/details/ggctnbvln.sHtML

find . -name "*.tmp" -delete
来源：http://read.share.bbcook.cn/Article/details/gvctpvcpn.sHtML

[R46] 递归替换文件内容
来源：http://www.share.fktsv.cn/Article/details/gldpuutah.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mobile.epnwcf.com/Article/details/gidlzsgjr.sHtML

[R47] sed 单行替换
来源：http://3g.sjlbkw.cn/Article/details/gllfboomk.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://wap.yfazqb.com/Article/details/gmptjbyog.sHtML

[R48] awk 取指定列
来源：http://mobile.bbcook.cn/Article/details/gwpgewrab.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.m.share.tarul.cn/Article/details/guelnufeu.sHtML

[R49] awk 带条件
来源：http://m.share.vehdjk.com/Article/details/gacdxvggc.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://mobile.sjlbkw.cn/Article/details/gqrtqcmqw.sHtML

[R50] awk 求和
来源：http://www.share.yfazqb.com/Article/details/gpyjljztr.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://baike.vehdjk.com/Article/details/ggxqapons.sHtML

[R51] 排序去重取前几
来源：http://read.share.sjlbkw.cn/Article/details/gnomeditj.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://m.share.tarul.cn/Article/details/gnzaskfsr.sHtML

[R52] 统计行数
来源：http://blog.tarul.cn/Article/details/guxwgzhwc.sHtML

wc -l a.txt
来源：http://mobile.vehdjk.com/Article/details/gkcplvbel.sHtML

[R53] 查看文件头与实时尾
来源：http://m.share.sjlbkw.cn/Article/details/genzwvfgw.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.m.share.yfazqb.com/Article/details/gjrtzmavo.sHtML

[R54] 比较两个文件
来源：http://3g.tarul.cn/Article/details/goqpvhohi.sHtML

diff a.txt b.txt
来源：http://www.m.share.epnwcf.com/Article/details/gwdlgwlfc.sHtML

[R55] 压缩与解压
来源：http://baike.vehdjk.com/Article/details/gqtwwrrmx.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://wap.fktsv.cn/Article/details/gxhaqusxc.sHtML

[R56] 远程拷贝
来源：http://www.blog.yfazqb.com/Article/details/ggfncxuap.sHtML

scp file user@host:/path/
来源：http://blog.bbcook.cn/Article/details/gorssiszu.sHtML

[R57] 远程执行命令
来源：http://wap.tarul.cn/Article/details/gyavkptdh.sHtML

ssh user@host 'uptime'
来源：http://read.share.yfazqb.com/Article/details/gaqkxquao.sHtML

[R58] 下载文件
来源：http://baike.sjlbkw.cn/Article/details/gtzxfeixp.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://mobile.bbcook.cn/Article/details/gayasckdb.sHtML

[R59] 发 POST JSON
来源：http://3g.bbcook.cn/Article/details/grsqaggtl.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.blog.yfazqb.com/Article/details/gkznscfdz.sHtML

[R60] 只看 HTTP 状态码
来源：http://mobile.vehdjk.com/Article/details/gmsfabsvd.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://read.share.bbcook.cn/Article/details/gebolqjja.sHtML

[R61] 磁盘占用
来源：http://read.share.tarul.cn/Article/details/gdnlyqqkh.sHtML

df -h;  du -sh *
来源：http://www.share.sjlbkw.cn/Article/details/gdfekyqsu.sHtML

[R62] 找最占空间的文件
来源：http://wap.yfazqb.com/Article/details/gbwihbqpc.sHtML

du -ah . | sort -rh | head -10
来源：http://read.share.yfazqb.com/Article/details/gcwvfbmdw.sHtML

[R63] 内存与进程
来源：http://blog.tarul.cn/Article/details/gfcaoktum.sHtML

free -h;  ps aux | grep nginx
来源：http://www.m.share.tarul.cn/Article/details/gdrsbmtdj.sHtML

[R64] 结束进程
来源：http://baike.fktsv.cn/Article/details/goybsfsjs.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.share.epnwcf.com/Article/details/gaemcijnv.sHtML

[R65] 查看端口占用
来源：http://www.share.sjlbkw.cn/Article/details/gazeoiocn.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://baike.sjlbkw.cn/Article/details/gobbzvocg.sHtML

[R66] 定时任务
来源：http://blog.vehdjk.com/Article/details/guilykzmk.sHtML

crontab -e;  crontab -l
来源：http://www.m.share.sjlbkw.cn/Article/details/gyzqzgpgg.sHtML

[R67] 生成随机十六进制串
来源：http://blog.tarul.cn/Article/details/gjorfzjvq.sHtML

openssl rand -hex 16
来源：http://www.blog.vehdjk.com/Article/details/gdxnduswd.sHtML

[R68] 计算文件校验值
来源：http://www.share.bbcook.cn/Article/details/gpfoxwupj.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://blog.sjlbkw.cn/Article/details/gtxjztyhv.sHtML

[R69] 生成随机密码
来源：http://www.m.share.sjlbkw.cn/Article/details/gmjwwydtm.sHtML

head -c 16 /dev/urandom | base64
来源：http://m.share.yfazqb.com/Article/details/grthjwozq.sHtML

[R70] 时间戳与互转
来源：http://www.m.share.yfazqb.com/Article/details/gjavhxnma.sHtML

date +%s;  date -d @1700000000
来源：http://read.share.yfazqb.com/Article/details/gczbqknqh.sHtML

[R71] 日期格式化
来源：http://www.share.yfazqb.com/Article/details/gnsdouqiz.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://mobile.fktsv.cn/Article/details/gojukpisu.sHtML

[R72] 等待端口就绪
来源：http://blog.bbcook.cn/Article/details/gqzkbykex.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://3g.yfazqb.com/Article/details/gszasezbl.sHtML

[R73] 分割大日志
来源：http://baike.sjlbkw.cn/Article/details/gpnipsqnh.sHtML

split -l 1000 big.log part_
来源：http://read.share.yfazqb.com/Article/details/glrykzesk.sHtML

[R74] 批量重命名
来源：http://wap.bbcook.cn/Article/details/gwlbhtdil.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://mobile.sjlbkw.cn/Article/details/gpbqowfnp.sHtML

[R75] 导出环境变量
来源：http://www.blog.epnwcf.com/Article/details/grtziensy.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://wap.epnwcf.com/Article/details/glaulucgi.sHtML

[R76] 使用临时文件
来源：http://baike.vehdjk.com/Article/details/guglhgcxl.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.epnwcf.com/Article/details/gvnwdkvoc.sHtML

[R77] 读取用户输入
来源：http://baike.yfazqb.com/Article/details/gtkjedarw.sHtML

read -rp "请输入: " ans
来源：http://www.share.tarul.cn/Article/details/gomuwhyqf.sHtML

[R78] 交互式菜单
来源：http://3g.bbcook.cn/Article/details/gvosxevzy.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://mobile.epnwcf.com/Article/details/gcgzyejzu.sHtML

[R79] 解析命令行选项
来源：http://www.blog.sjlbkw.cn/Article/details/gplrjwxtp.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://3g.tarul.cn/Article/details/gioixwxfi.sHtML

[R80] 查看脚本执行耗时
来源：http://www.blog.yfazqb.com/Article/details/goiivegwl.sHtML

time ./run.sh
来源：http://baike.bbcook.cn/Article/details/gokqwgvog.sHtML

================================================================================
来源：http://baike.vehdjk.com/Article/details/gxxgfovwu.sHtML

S. C / C++ 专题
来源：http://www.blog.vehdjk.com/Article/details/gfxafqlrx.sHtML

================================================================================
来源：http://mobile.tarul.cn/Article/details/gmjmysgdn.sHtML

[S01] C：Hello World
来源：http://baike.yfazqb.com/Article/details/gkcyuucfc.sHtML

#include <stdio.h>
来源：http://www.share.fktsv.cn/Article/details/gldbyvvgn.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://wap.yfazqb.com/Article/details/gotcrxtfp.sHtML

[S02] C：变量与格式化输出
来源：http://blog.bbcook.cn/Article/details/gwtexoktl.sHtML

int a = 10; printf("%d\n", a);
来源：http://baike.vehdjk.com/Article/details/gtrzmrrpl.sHtML

[S03] C：读入整数
来源：http://wap.sjlbkw.cn/Article/details/gtlvmwkxi.sHtML

int x; scanf("%d", &x);
来源：http://blog.yfazqb.com/Article/details/gvmfklxiz.sHtML

[S04] C：字符串复制
来源：http://www.blog.sjlbkw.cn/Article/details/gloqpjjas.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://wap.tarul.cn/Article/details/gxsrecxeg.sHtML

[S05] C：字符串长度
来源：http://baike.bbcook.cn/Article/details/gdxljcwvb.sHtML

strlen(s)
来源：http://read.share.epnwcf.com/Article/details/giblittum.sHtML

[S06] C：字符串比较
来源：http://m.share.sjlbkw.cn/Article/details/gfxwdwawr.sHtML

strcmp(a, b) == 0
来源：http://www.m.share.epnwcf.com/Article/details/gxmhyifwk.sHtML

[S07] C：数组遍历求和
来源：http://www.blog.sjlbkw.cn/Article/details/gitmxvmuk.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://baike.fktsv.cn/Article/details/gjwrgbpea.sHtML

[S08] C：动态内存分配与释放
来源：http://3g.bbcook.cn/Article/details/gktppzwzi.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mobile.tarul.cn/Article/details/ghbkfaznp.sHtML

[S09] C：结构体定义与初始化
来源：http://wap.tarul.cn/Article/details/grvkraiym.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.share.epnwcf.com/Article/details/gnetqinqz.sHtML

[S10] C：指针与解引用
来源：http://mobile.epnwcf.com/Article/details/geuixazud.sHtML

int *p = &a;  *p = 5;
来源：http://wap.yfazqb.com/Article/details/gkbvhfqto.sHtML

[S11] C：逐行读文件
来源：http://blog.yfazqb.com/Article/details/gnujlqtmx.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://baike.fktsv.cn/Article/details/gointertx.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://read.share.vehdjk.com/Article/details/garzycupq.sHtML

fclose(f);
来源：http://wap.epnwcf.com/Article/details/gekdeozpp.sHtML

[S12] C：写文件
来源：http://baike.bbcook.cn/Article/details/gyvvshxia.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://blog.yfazqb.com/Article/details/gqbtkkyyi.sHtML

[S13] C：宏定义
来源：http://www.blog.sjlbkw.cn/Article/details/gjochwdwl.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.share.fktsv.cn/Article/details/gidekerrm.sHtML

[S14] C：枚举
来源：http://wap.sjlbkw.cn/Article/details/gcopvqmwz.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://mobile.yfazqb.com/Article/details/gjhkbqyzw.sHtML

[S15] C：类型转换
来源：http://www.share.fktsv.cn/Article/details/graeejfjv.sHtML

(double) a / b
来源：http://www.m.share.yfazqb.com/Article/details/gmctjbyic.sHtML

[S16] C：位操作置位
来源：http://m.share.bbcook.cn/Article/details/gehrtrvob.sHtML

x |= (1 << 3);
来源：http://m.share.epnwcf.com/Article/details/grgjqovwj.sHtML

[S17] C：安全拼接字符串
来源：http://m.share.tarul.cn/Article/details/gxddwbmji.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://m.share.yfazqb.com/Article/details/grewfnepb.sHtML

[S18] C：命令行参数
来源：http://wap.epnwcf.com/Article/details/gyialxamv.sHtML

int main(int argc, char **argv)
来源：http://baike.vehdjk.com/Article/details/grwbsfoaf.sHtML

[S19] C：快速排序
来源：http://read.share.vehdjk.com/Article/details/gyuaxtlqe.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.blog.yfazqb.com/Article/details/gketvkecj.sHtML

[S20] C：二分查找
来源：http://m.share.sjlbkw.cn/Article/details/gistzrfgb.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://3g.epnwcf.com/Article/details/gvuwzutlc.sHtML

[S21] C：字符类别判断
来源：http://www.m.share.yfazqb.com/Article/details/gaswncyom.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://baike.bbcook.cn/Article/details/ghbjcwyxj.sHtML

[S22] C：字符串转数字
来源：http://m.share.yfazqb.com/Article/details/gphdnhdzz.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.m.share.sjlbkw.cn/Article/details/gvcyifrzr.sHtML

[S23] C：随机数
来源：http://mobile.fktsv.cn/Article/details/ghvkjeyaf.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://wap.vehdjk.com/Article/details/gmmkutkcq.sHtML

[S24] C：获取本地时间
来源：http://3g.tarul.cn/Article/details/glfmfditz.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://baike.tarul.cn/Article/details/ggazpwncb.sHtML

[S25] C：内存拷贝
来源：http://3g.epnwcf.com/Article/details/gndeqdygt.sHtML

memcpy(dst, src, n);
来源：http://blog.sjlbkw.cn/Article/details/glknthwtk.sHtML

[S26] C：内存清零
来源：http://read.share.fktsv.cn/Article/details/gxpusvbmf.sHtML

memset(a, 0, sizeof a);
来源：http://www.share.tarul.cn/Article/details/goadmmppp.sHtML

[S27] C：定义常量
来源：http://wap.epnwcf.com/Article/details/goflbxzfd.sHtML

const double PI = 3.14159;
来源：http://wap.yfazqb.com/Article/details/gudmzsxzs.sHtML

[S28] C：静态变量
来源：http://blog.epnwcf.com/Article/details/grqddbsce.sHtML

static int counter = 0;
来源：http://wap.bbcook.cn/Article/details/gxfyghses.sHtML

[S29] C：变参函数
来源：http://mobile.sjlbkw.cn/Article/details/gfpmiivxw.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.m.share.tarul.cn/Article/details/gumkeiteg.sHtML

[S30] C：头文件保护
来源：http://wap.vehdjk.com/Article/details/gywktddls.sHtML

#ifndef X_H
来源：http://blog.tarul.cn/Article/details/glneokilw.sHtML

#define X_H
来源：http://read.share.sjlbkw.cn/Article/details/gjijaxoab.sHtML

#endif
来源：http://3g.epnwcf.com/Article/details/glacwzclc.sHtML

[S31] C++：Hello World
来源：http://m.share.bbcook.cn/Article/details/gmqdbtcij.sHtML

#include <iostream>
来源：http://m.share.sjlbkw.cn/Article/details/gidqqydgb.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://3g.vehdjk.com/Article/details/gsszxaxhh.sHtML

[S32] C++：字符串
来源：http://blog.tarul.cn/Article/details/gnrcizfgr.sHtML

std::string s = "hi";  s += "!";
来源：http://blog.fktsv.cn/Article/details/gckxodlkb.sHtML

[S33] C++：vector 增删
来源：http://www.blog.fktsv.cn/Article/details/gacrrijrs.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://wap.epnwcf.com/Article/details/ghbrbdmdw.sHtML

[S34] C++：遍历 vector
来源：http://www.share.tarul.cn/Article/details/gyuahcdab.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.share.vehdjk.com/Article/details/gmqxkzloh.sHtML

[S35] C++：map
来源：http://mobile.yfazqb.com/Article/details/gzxrkrmgc.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.yfazqb.com/Article/details/gpbkbsjyu.sHtML

[S36] C++：unordered_map
来源：http://mobile.sjlbkw.cn/Article/details/gnntvoctc.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.sjlbkw.cn/Article/details/guqodushy.sHtML

[S37] C++：set
来源：http://www.blog.sjlbkw.cn/Article/details/gdssguizr.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://blog.yfazqb.com/Article/details/gqvnhrbeg.sHtML

[S38] C++：排序
来源：http://baike.vehdjk.com/Article/details/gltulllly.sHtML

std::sort(v.begin(), v.end());
来源：http://www.m.share.tarul.cn/Article/details/gewxwrxye.sHtML

[S39] C++：自定义比较器排序
来源：http://m.share.bbcook.cn/Article/details/gtvyuafuz.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.m.share.sjlbkw.cn/Article/details/godeltcog.sHtML

[S40] C++：查找元素
来源：http://www.share.fktsv.cn/Article/details/gojsafdwy.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://wap.yfazqb.com/Article/details/gehdepamk.sHtML

[S41] C++：类与构造函数
来源：http://www.blog.tarul.cn/Article/details/gwiouxggs.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.share.fktsv.cn/Article/details/ghdhfriva.sHtML

[S42] C++：继承与虚函数
来源：http://www.m.share.yfazqb.com/Article/details/ggotlyipa.sHtML

class B : public Base { public: void f() override {} };
来源：http://wap.fktsv.cn/Article/details/groeqqjus.sHtML

[S43] C++：智能指针
来源：http://blog.sjlbkw.cn/Article/details/gpnrdmjhs.sHtML

auto p = std::make_unique<int>(5);
来源：http://3g.sjlbkw.cn/Article/details/grzvczfic.sHtML

[S44] C++：引用传参
来源：http://read.share.tarul.cn/Article/details/ggrqzxodb.sHtML

void inc(int &x) { ++x; }
来源：http://mobile.epnwcf.com/Article/details/gknkecqte.sHtML

[S45] C++：lambda
来源：http://www.blog.fktsv.cn/Article/details/grzqfeuep.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://blog.sjlbkw.cn/Article/details/gbxazispx.sHtML

[S46] C++：函数模板
来源：http://baike.tarul.cn/Article/details/gdvwaohmt.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.m.share.bbcook.cn/Article/details/gksodgsar.sHtML

[S47] C++：结构化绑定遍历
来源：http://m.share.epnwcf.com/Article/details/gzyenppdo.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://read.share.fktsv.cn/Article/details/gldxzsbna.sHtML

[S48] C++：逐行读文件
来源：http://baike.sjlbkw.cn/Article/details/ggdjkwjod.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://blog.vehdjk.com/Article/details/gxniztqaq.sHtML

while (std::getline(in, line)) { }
来源：http://www.m.share.sjlbkw.cn/Article/details/gqmojiufz.sHtML

[S49] C++：写文件
来源：http://blog.yfazqb.com/Article/details/gwyrekkil.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.blog.bbcook.cn/Article/details/gtnmrvfle.sHtML

[S50] C++：格式化数字
来源：http://www.blog.sjlbkw.cn/Article/details/genxduldp.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://wap.yfazqb.com/Article/details/grzznlttu.sHtML

[S51] C++：显式类型转换
来源：http://baike.sjlbkw.cn/Article/details/gitjwpiji.sHtML

static_cast<double>(a) / b
来源：http://baike.sjlbkw.cn/Article/details/gprirbrnq.sHtML

[S52] C++：const 与 noexcept
来源：http://read.share.bbcook.cn/Article/details/gtbaonjmg.sHtML

int size() const noexcept { return n_; }
来源：http://blog.tarul.cn/Article/details/gckovvozh.sHtML

[S53] C++：移动语义
来源：http://wap.epnwcf.com/Article/details/gxixsocve.sHtML

std::vector<int> w = std::move(v);
来源：http://baike.yfazqb.com/Article/details/gyswnjqqp.sHtML

[S54] C++：异常处理
来源：http://baike.epnwcf.com/Article/details/ggsjoxxuv.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://baike.yfazqb.com/Article/details/gbtawfluv.sHtML

[S55] C++：结构化绑定
来源：http://m.share.vehdjk.com/Article/details/gxyogtxvo.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.blog.bbcook.cn/Article/details/gusjctyrn.sHtML

[S56] C++：optional
来源：http://wap.yfazqb.com/Article/details/gcafapygy.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.blog.yfazqb.com/Article/details/geokxkucb.sHtML

[S57] C++：编译期常量
来源：http://m.share.fktsv.cn/Article/details/gdcuvrcth.sHtML

constexpr int N = 10;
来源：http://mobile.sjlbkw.cn/Article/details/gtorhnxhx.sHtML

[S58] C++：命名空间
来源：http://www.m.share.epnwcf.com/Article/details/gcyhnouqm.sHtML

namespace ns { int f() { return 1; } }
来源：http://m.share.yfazqb.com/Article/details/gidfbkqrl.sHtML

[S59] C++：静态断言
来源：http://www.share.bbcook.cn/Article/details/gvbnkylrx.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://baike.bbcook.cn/Article/details/gbktjwdyg.sHtML

[S60] C++：遍历并删除元素
来源：http://www.m.share.vehdjk.com/Article/details/guprhpcfw.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://3g.epnwcf.com/Article/details/gjwynqyiu.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/gmscdixoh.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://baike.tarul.cn/Article/details/gcblzszyv.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/gmehwwzkm.sHtML

[T01] Kotlin：Hello World
来源：http://read.share.tarul.cn/Article/details/gkjvvrasy.sHtML

println("Hello")
来源：http://www.blog.bbcook.cn/Article/details/gcsxxalbb.sHtML

[T02] Kotlin：变量
来源：http://3g.fktsv.cn/Article/details/ghvvdqpes.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://mobile.fktsv.cn/Article/details/gusbhmshr.sHtML

[T03] Kotlin：字符串模板
来源：http://wap.bbcook.cn/Article/details/gdegofnzj.sHtML

"值: $b"
来源：http://mobile.bbcook.cn/Article/details/gmurvplor.sHtML

[T04] Kotlin：空安全
来源：http://m.share.vehdjk.com/Article/details/gxmjicugy.sHtML

val n: String? = null;  n?.length
来源：http://baike.yfazqb.com/Article/details/gjskuphcf.sHtML

[T05] Kotlin：when 表达式
来源：http://wap.bbcook.cn/Article/details/ghbeefkyi.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.blog.vehdjk.com/Article/details/gynnczwic.sHtML

[T06] Kotlin：集合映射
来源：http://www.blog.sjlbkw.cn/Article/details/gkyxosbpt.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.m.share.epnwcf.com/Article/details/gdtltsmwy.sHtML

[T07] Kotlin：集合过滤
来源：http://www.blog.vehdjk.com/Article/details/gptypdokg.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.share.sjlbkw.cn/Article/details/gcbrxadvq.sHtML

[T08] Kotlin：数据类
来源：http://wap.epnwcf.com/Article/details/gkmxsusow.sHtML

data class User(val name: String, val age: Int)
来源：http://baike.tarul.cn/Article/details/ggzoxyjmh.sHtML

[T09] Kotlin：扩展函数
来源：http://blog.sjlbkw.cn/Article/details/glwnpeabl.sHtML

fun String.exclaim() = this + "!"
来源：http://www.share.fktsv.cn/Article/details/grfrtubay.sHtML

[T10] Kotlin：默认参数
来源：http://baike.bbcook.cn/Article/details/grzamcdko.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://read.share.bbcook.cn/Article/details/gyfktdcpd.sHtML

[T11] Kotlin：协程
来源：http://www.blog.fktsv.cn/Article/details/gdhgrgjwq.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://baike.vehdjk.com/Article/details/gesdkeomg.sHtML

[T12] Kotlin：解构声明
来源：http://wap.tarul.cn/Article/details/gfltylopf.sHtML

val (a, b) = Pair(1, 2)
来源：http://read.share.epnwcf.com/Article/details/guopwzcfn.sHtML

[T13] Kotlin：只读 Map
来源：http://baike.fktsv.cn/Article/details/gndfkuasl.sHtML

val m = mapOf("a" to 1)
来源：http://m.share.fktsv.cn/Article/details/gfkbvmpun.sHtML

[T14] Kotlin：循环
来源：http://read.share.sjlbkw.cn/Article/details/guwwhlsen.sHtML

for (i in 1..10) println(i)
来源：http://read.share.fktsv.cn/Article/details/gcjbiflgd.sHtML

[T15] Kotlin：接口
来源：http://www.blog.bbcook.cn/Article/details/gjruoltcc.sHtML

interface Shape { fun area(): Double }
来源：http://blog.vehdjk.com/Article/details/ghgcyhwde.sHtML

[T16] Swift：Hello World
来源：http://3g.sjlbkw.cn/Article/details/gnkpnhgyb.sHtML

print("Hello")
来源：http://wap.bbcook.cn/Article/details/gxgzxondh.sHtML

[T17] Swift：变量与常量
来源：http://read.share.sjlbkw.cn/Article/details/gpboovars.sHtML

var a = 1;  let b = 2
来源：http://wap.epnwcf.com/Article/details/gpxljwyir.sHtML

[T18] Swift：字符串插值
来源：http://read.share.sjlbkw.cn/Article/details/garnwqckk.sHtML

"值: \(b)"
来源：http://baike.fktsv.cn/Article/details/gvcsvmxcu.sHtML

[T19] Swift：可选绑定
来源：http://blog.yfazqb.com/Article/details/gimslvhgp.sHtML

if let n = opt { print(n) }
来源：http://www.share.epnwcf.com/Article/details/gnlrzbujz.sHtML

[T20] Swift：数组操作
来源：http://mobile.yfazqb.com/Article/details/gdalmqgpj.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://blog.yfazqb.com/Article/details/ggdnshbie.sHtML

[T21] Swift：遍历
来源：http://wap.epnwcf.com/Article/details/gagifyykf.sHtML

for x in a { print(x) }
来源：http://baike.sjlbkw.cn/Article/details/gjfnqcbmq.sHtML

[T22] Swift：字典
来源：http://www.blog.sjlbkw.cn/Article/details/gwaacbpon.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://baike.tarul.cn/Article/details/gtfswffxp.sHtML

[T23] Swift：函数
来源：http://mobile.sjlbkw.cn/Article/details/gbijnccbi.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://m.share.tarul.cn/Article/details/gkaatdhkc.sHtML

[T24] Swift：闭包
来源：http://baike.vehdjk.com/Article/details/gudnlpkwb.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.m.share.sjlbkw.cn/Article/details/gaktvcnlw.sHtML

[T25] Swift：结构体
来源：http://m.share.sjlbkw.cn/Article/details/ggksgxitf.sHtML

struct P { var x: Int }
来源：http://www.blog.sjlbkw.cn/Article/details/gvcqdcmbv.sHtML

[T26] Swift：类与重写
来源：http://wap.epnwcf.com/Article/details/ggoonlews.sHtML

class A: Base { override func f() {} }
来源：http://mobile.tarul.cn/Article/details/gmiyuucnv.sHtML

[T27] Swift：错误处理
来源：http://baike.sjlbkw.cn/Article/details/gzwkkubsd.sHtML

do { try f() } catch { print(error) }
来源：http://wap.sjlbkw.cn/Article/details/gkxvybhax.sHtML

[T28] Swift：枚举
来源：http://www.share.vehdjk.com/Article/details/grgtupuwa.sHtML

enum Color { case red, green }
来源：http://baike.epnwcf.com/Article/details/gyarhdnhz.sHtML

[T29] Swift：guard 提前返回
来源：http://mobile.epnwcf.com/Article/details/gpeogkpnr.sHtML

guard let x = opt else { return }
来源：http://www.blog.vehdjk.com/Article/details/gcbhmpbzx.sHtML

[T30] Swift：协议
来源：http://blog.tarul.cn/Article/details/grzleorfj.sHtML

protocol Shape { func area() -> Double }
来源：http://baike.tarul.cn/Article/details/gqwpzmyyc.sHtML


<!-- 参考信息 -->