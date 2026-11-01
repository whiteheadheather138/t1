代发 wailian999

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.share.fktsv.cn/Article/details/gmsgwacoi.sHtML

[R26] 命令替换
来源：http://wap.yfazqb.com/Article/details/gqigoxfrs.sHtML

now=$(date +%F); echo "$now"
来源：http://blog.yfazqb.com/Article/details/gximgovip.sHtML

[R27] 算术展开
来源：http://blog.sjlbkw.cn/Article/details/gsymiilvz.sHtML

echo $((1 + 2 * 3))
来源：http://read.share.tarul.cn/Article/details/gtzkgduap.sHtML

[R28] 浮点运算
来源：http://blog.epnwcf.com/Article/details/gxzxkmhlw.sHtML

echo "scale=2; 10/3" | bc
来源：http://m.share.bbcook.cn/Article/details/gzkgonyvh.sHtML

[R29] 定义函数
来源：http://blog.fktsv.cn/Article/details/grnktlbmz.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://mobile.bbcook.cn/Article/details/gvulbbxfh.sHtML

[R30] 函数返回状态码
来源：http://blog.vehdjk.com/Article/details/gvsvvuhgf.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://read.share.tarul.cn/Article/details/gazhbgltl.sHtML

[R31] 局部变量
来源：http://mobile.fktsv.cn/Article/details/gylwyfact.sHtML

f() { local x=1; echo "$x"; }
来源：http://wap.tarul.cn/Article/details/grbtiyoyk.sHtML

[R32] 参数个数校验
来源：http://mobile.yfazqb.com/Article/details/gettfswpm.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.m.share.tarul.cn/Article/details/gmbgtvrwh.sHtML

[R33] 捕获错误并提示行号
来源：http://read.share.tarul.cn/Article/details/gmklnlico.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://blog.tarul.cn/Article/details/gqnlkrual.sHtML

[R34] 退出时清理
来源：http://www.share.epnwcf.com/Article/details/ginzfufle.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.epnwcf.com/Article/details/gbxfobkyo.sHtML

[R35] 后台执行并等待
来源：http://m.share.sjlbkw.cn/Article/details/gzzinufcj.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.blog.tarul.cn/Article/details/gsfgephnn.sHtML

[R36] 并发执行多个任务
来源：http://m.share.epnwcf.com/Article/details/gpcpkxgco.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://mobile.yfazqb.com/Article/details/geibtkwfp.sHtML

[R37] 把输出赋给变量
来源：http://mobile.epnwcf.com/Article/details/gurbdhihy.sHtML

files=$(ls -1)
来源：http://blog.tarul.cn/Article/details/gzfkmsbwg.sHtML

[R38] 管道串联
来源：http://www.share.tarul.cn/Article/details/geufhtzgb.sHtML

cat a.txt | grep -i error | wc -l
来源：http://3g.sjlbkw.cn/Article/details/gwiystoqd.sHtML

[R39] 重定向标准输出与错误
来源：http://3g.bbcook.cn/Article/details/gvhuywjcg.sHtML

cmd > out.log 2>&1
来源：http://blog.tarul.cn/Article/details/grdcpedbv.sHtML

[R40] 追加写日志
来源：http://www.blog.epnwcf.com/Article/details/gyyeylmie.sHtML

echo "log" >> out.log
来源：http://mobile.fktsv.cn/Article/details/gpkuxftxr.sHtML

[R41] 丢弃输出
来源：http://www.m.share.bbcook.cn/Article/details/gfirguuxw.sHtML

cmd >/dev/null 2>&1
来源：http://blog.bbcook.cn/Article/details/grmqpeolp.sHtML

[R42] 输入重定向
来源：http://3g.yfazqb.com/Article/details/gocdfzvod.sHtML

wc -l < a.txt
来源：http://blog.bbcook.cn/Article/details/gntpwtrlo.sHtML

[R43] 按名字查找文件
来源：http://blog.epnwcf.com/Article/details/gpcrkcgjl.sHtML

find . -name "*.log" -type f
来源：http://mobile.vehdjk.com/Article/details/gfsyphwte.sHtML

[R44] 按修改时间查找
来源：http://blog.sjlbkw.cn/Article/details/gzpkddgti.sHtML

find . -mtime -7 -type f
来源：http://3g.vehdjk.com/Article/details/gyvxarwdg.sHtML

[R45] 批量删除
来源：http://baike.epnwcf.com/Article/details/gvysiemyb.sHtML

find . -name "*.tmp" -delete
来源：http://www.blog.vehdjk.com/Article/details/grskpnwat.sHtML

[R46] 递归替换文件内容
来源：http://mobile.fktsv.cn/Article/details/gkuzwxfsp.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://m.share.sjlbkw.cn/Article/details/ghihwnspu.sHtML

[R47] sed 单行替换
来源：http://blog.yfazqb.com/Article/details/gnjewiznj.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.share.bbcook.cn/Article/details/gwuslhkhv.sHtML

[R48] awk 取指定列
来源：http://3g.sjlbkw.cn/Article/details/gwbgiuenu.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.blog.epnwcf.com/Article/details/gqznapcjb.sHtML

[R49] awk 带条件
来源：http://3g.epnwcf.com/Article/details/gdhohzqeg.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://blog.fktsv.cn/Article/details/gktfkrkzs.sHtML

[R50] awk 求和
来源：http://baike.epnwcf.com/Article/details/gowroczwg.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://blog.bbcook.cn/Article/details/ghlqrbuqb.sHtML

[R51] 排序去重取前几
来源：http://wap.vehdjk.com/Article/details/gztzknjfn.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://wap.fktsv.cn/Article/details/gvuzkwuiu.sHtML

[R52] 统计行数
来源：http://wap.sjlbkw.cn/Article/details/gyqofkqkm.sHtML

wc -l a.txt
来源：http://baike.vehdjk.com/Article/details/gentlrwlo.sHtML

[R53] 查看文件头与实时尾
来源：http://wap.yfazqb.com/Article/details/gviiztckx.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://m.share.sjlbkw.cn/Article/details/giaelcvbr.sHtML

[R54] 比较两个文件
来源：http://mobile.bbcook.cn/Article/details/ggszhqsyh.sHtML

diff a.txt b.txt
来源：http://mobile.sjlbkw.cn/Article/details/gsdjiakyp.sHtML

[R55] 压缩与解压
来源：http://www.m.share.epnwcf.com/Article/details/gzsxqzois.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.share.sjlbkw.cn/Article/details/gvkonycqv.sHtML

[R56] 远程拷贝
来源：http://m.share.vehdjk.com/Article/details/gkjlewwfx.sHtML

scp file user@host:/path/
来源：http://blog.sjlbkw.cn/Article/details/geacjoeyv.sHtML

[R57] 远程执行命令
来源：http://baike.fktsv.cn/Article/details/gdebrycji.sHtML

ssh user@host 'uptime'
来源：http://wap.fktsv.cn/Article/details/gbnmegssi.sHtML

[R58] 下载文件
来源：http://wap.epnwcf.com/Article/details/gbmqaugov.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://mobile.sjlbkw.cn/Article/details/gbjwtktla.sHtML

[R59] 发 POST JSON
来源：http://www.blog.tarul.cn/Article/details/gqixkokfs.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://mobile.bbcook.cn/Article/details/gaphykqkm.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.blog.epnwcf.com/Article/details/grnmqanki.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://blog.fktsv.cn/Article/details/gkazgwxxy.sHtML

[R61] 磁盘占用
来源：http://3g.fktsv.cn/Article/details/ghqpfoxyo.sHtML

df -h;  du -sh *
来源：http://blog.bbcook.cn/Article/details/glyijyjhi.sHtML

[R62] 找最占空间的文件
来源：http://3g.epnwcf.com/Article/details/gswzssfln.sHtML

du -ah . | sort -rh | head -10
来源：http://mobile.bbcook.cn/Article/details/gsyjdljye.sHtML

[R63] 内存与进程
来源：http://www.blog.vehdjk.com/Article/details/gqioaumnq.sHtML

free -h;  ps aux | grep nginx
来源：http://read.share.tarul.cn/Article/details/gkedukmkt.sHtML

[R64] 结束进程
来源：http://3g.yfazqb.com/Article/details/gqdgwwqby.sHtML

kill -9 $(pgrep -f app.py)
来源：http://3g.fktsv.cn/Article/details/gtolfonok.sHtML

[R65] 查看端口占用
来源：http://mobile.vehdjk.com/Article/details/ggjpqxhel.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mobile.fktsv.cn/Article/details/ghvvccsjq.sHtML

[R66] 定时任务
来源：http://m.share.epnwcf.com/Article/details/gshccwuta.sHtML

crontab -e;  crontab -l
来源：http://baike.bbcook.cn/Article/details/gsedjomjx.sHtML

[R67] 生成随机十六进制串
来源：http://blog.vehdjk.com/Article/details/gaibpmhdc.sHtML

openssl rand -hex 16
来源：http://www.m.share.tarul.cn/Article/details/gjhvhplww.sHtML

[R68] 计算文件校验值
来源：http://read.share.epnwcf.com/Article/details/gwjlgdvsl.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://blog.vehdjk.com/Article/details/gtqpnxtwr.sHtML

[R69] 生成随机密码
来源：http://baike.sjlbkw.cn/Article/details/gwwfqoffg.sHtML

head -c 16 /dev/urandom | base64
来源：http://3g.fktsv.cn/Article/details/gijrxennq.sHtML

[R70] 时间戳与互转
来源：http://3g.vehdjk.com/Article/details/gjfnqvouc.sHtML

date +%s;  date -d @1700000000
来源：http://baike.bbcook.cn/Article/details/gkdorfqqh.sHtML

[R71] 日期格式化
来源：http://blog.bbcook.cn/Article/details/guyltwnbu.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://m.share.sjlbkw.cn/Article/details/gdlvmieep.sHtML

[R72] 等待端口就绪
来源：http://www.blog.vehdjk.com/Article/details/gfqxesmpa.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.m.share.tarul.cn/Article/details/gzjdgjhyn.sHtML

[R73] 分割大日志
来源：http://www.m.share.fktsv.cn/Article/details/guhhtxahu.sHtML

split -l 1000 big.log part_
来源：http://www.share.vehdjk.com/Article/details/gitffpcpt.sHtML

[R74] 批量重命名
来源：http://wap.sjlbkw.cn/Article/details/gtvxoqsbq.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.m.share.bbcook.cn/Article/details/gpjnqbukt.sHtML

[R75] 导出环境变量
来源：http://baike.fktsv.cn/Article/details/grjgxxwtx.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://m.share.bbcook.cn/Article/details/gwllkyzdc.sHtML

[R76] 使用临时文件
来源：http://mobile.tarul.cn/Article/details/gjqjjswvy.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://read.share.epnwcf.com/Article/details/guqgzxaic.sHtML

[R77] 读取用户输入
来源：http://www.share.sjlbkw.cn/Article/details/gzphcgbgy.sHtML

read -rp "请输入: " ans
来源：http://www.m.share.vehdjk.com/Article/details/gkphqvafx.sHtML

[R78] 交互式菜单
来源：http://blog.sjlbkw.cn/Article/details/gdiazfvom.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://read.share.bbcook.cn/Article/details/gbyqbhxzk.sHtML

[R79] 解析命令行选项
来源：http://www.blog.vehdjk.com/Article/details/ggetfvzop.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://read.share.epnwcf.com/Article/details/gnghitfry.sHtML

[R80] 查看脚本执行耗时
来源：http://wap.sjlbkw.cn/Article/details/geuacjtkf.sHtML

time ./run.sh
来源：http://3g.tarul.cn/Article/details/gnqoyceht.sHtML

================================================================================
来源：http://www.share.vehdjk.com/Article/details/gxlxnnxjn.sHtML

S. C / C++ 专题
来源：http://mobile.sjlbkw.cn/Article/details/gbnrkrieb.sHtML

================================================================================
来源：http://mobile.yfazqb.com/Article/details/gncluouil.sHtML

[S01] C：Hello World
来源：http://read.share.epnwcf.com/Article/details/gokdmchuz.sHtML

#include <stdio.h>
来源：http://www.blog.sjlbkw.cn/Article/details/gauczimyg.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.blog.tarul.cn/Article/details/gehbegyfm.sHtML

[S02] C：变量与格式化输出
来源：http://blog.vehdjk.com/Article/details/gdzvjfluy.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.share.vehdjk.com/Article/details/guemcsydo.sHtML

[S03] C：读入整数
来源：http://blog.bbcook.cn/Article/details/gipaghrfu.sHtML

int x; scanf("%d", &x);
来源：http://3g.tarul.cn/Article/details/geeiesckw.sHtML

[S04] C：字符串复制
来源：http://baike.vehdjk.com/Article/details/gioltrfyz.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://3g.bbcook.cn/Article/details/gxofeqomm.sHtML

[S05] C：字符串长度
来源：http://m.share.epnwcf.com/Article/details/gwaflhepv.sHtML

strlen(s)
来源：http://www.m.share.sjlbkw.cn/Article/details/gcktolfid.sHtML

[S06] C：字符串比较
来源：http://baike.sjlbkw.cn/Article/details/gatzpovuj.sHtML

strcmp(a, b) == 0
来源：http://read.share.epnwcf.com/Article/details/gebkkgugq.sHtML

[S07] C：数组遍历求和
来源：http://3g.vehdjk.com/Article/details/gedmsbxaf.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://wap.bbcook.cn/Article/details/gaoxxbyav.sHtML

[S08] C：动态内存分配与释放
来源：http://www.share.bbcook.cn/Article/details/gncqlqihs.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mobile.epnwcf.com/Article/details/gktdeuwgh.sHtML

[S09] C：结构体定义与初始化
来源：http://3g.bbcook.cn/Article/details/glnvpcbsg.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://baike.bbcook.cn/Article/details/gguojykol.sHtML

[S10] C：指针与解引用
来源：http://wap.sjlbkw.cn/Article/details/gufvgatep.sHtML

int *p = &a;  *p = 5;
来源：http://www.share.sjlbkw.cn/Article/details/gcgsnwzqn.sHtML

[S11] C：逐行读文件
来源：http://blog.fktsv.cn/Article/details/ggfywojvr.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://mobile.sjlbkw.cn/Article/details/glxjvdimu.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://read.share.yfazqb.com/Article/details/gthgtxtfn.sHtML

fclose(f);
来源：http://3g.bbcook.cn/Article/details/gfbwqkcqg.sHtML

[S12] C：写文件
来源：http://baike.fktsv.cn/Article/details/gxxgecoiu.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.share.yfazqb.com/Article/details/gepwmonnr.sHtML

[S13] C：宏定义
来源：http://m.share.epnwcf.com/Article/details/ghnqvdjyf.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://blog.yfazqb.com/Article/details/gbqlmkuuo.sHtML

[S14] C：枚举
来源：http://www.share.fktsv.cn/Article/details/glkhvflsb.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.blog.bbcook.cn/Article/details/gsjbfdate.sHtML

[S15] C：类型转换
来源：http://www.blog.fktsv.cn/Article/details/gtuijlukm.sHtML

(double) a / b
来源：http://mobile.yfazqb.com/Article/details/grzwjwfax.sHtML

[S16] C：位操作置位
来源：http://www.blog.yfazqb.com/Article/details/gcjlosazu.sHtML

x |= (1 << 3);
来源：http://read.share.sjlbkw.cn/Article/details/gntkrveup.sHtML

[S17] C：安全拼接字符串
来源：http://baike.bbcook.cn/Article/details/gyqjxgpln.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://read.share.fktsv.cn/Article/details/gamzlhwlq.sHtML

[S18] C：命令行参数
来源：http://baike.vehdjk.com/Article/details/gsrwnrkyt.sHtML

int main(int argc, char **argv)
来源：http://baike.sjlbkw.cn/Article/details/gsjwljktv.sHtML

[S19] C：快速排序
来源：http://mobile.epnwcf.com/Article/details/gdjrwzvil.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://3g.sjlbkw.cn/Article/details/galkbqvnm.sHtML

[S20] C：二分查找
来源：http://3g.sjlbkw.cn/Article/details/gslzbaylo.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://mobile.vehdjk.com/Article/details/gvibibhia.sHtML

[S21] C：字符类别判断
来源：http://www.blog.vehdjk.com/Article/details/gfkgzsfro.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.m.share.sjlbkw.cn/Article/details/gnhlbjzrj.sHtML

[S22] C：字符串转数字
来源：http://blog.bbcook.cn/Article/details/gajlgqzjc.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://m.share.epnwcf.com/Article/details/gpnizwzar.sHtML

[S23] C：随机数
来源：http://baike.vehdjk.com/Article/details/gyliqkiah.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://baike.fktsv.cn/Article/details/gvwqgqgrd.sHtML

[S24] C：获取本地时间
来源：http://baike.vehdjk.com/Article/details/gxhuzilms.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://3g.vehdjk.com/Article/details/ggzssxtew.sHtML

[S25] C：内存拷贝
来源：http://m.share.bbcook.cn/Article/details/gxrxgiaci.sHtML

memcpy(dst, src, n);
来源：http://www.m.share.yfazqb.com/Article/details/gzhnyzgil.sHtML

[S26] C：内存清零
来源：http://www.m.share.epnwcf.com/Article/details/gxuteldgx.sHtML

memset(a, 0, sizeof a);
来源：http://www.m.share.fktsv.cn/Article/details/gfcehowvd.sHtML

[S27] C：定义常量
来源：http://wap.sjlbkw.cn/Article/details/ghzxjcbpm.sHtML

const double PI = 3.14159;
来源：http://baike.tarul.cn/Article/details/gmkoiwotx.sHtML

[S28] C：静态变量
来源：http://blog.bbcook.cn/Article/details/gmsceoanu.sHtML

static int counter = 0;
来源：http://read.share.vehdjk.com/Article/details/grwyjnguo.sHtML

[S29] C：变参函数
来源：http://baike.sjlbkw.cn/Article/details/gnwcawwhk.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.share.yfazqb.com/Article/details/gqrbwtnks.sHtML

[S30] C：头文件保护
来源：http://www.blog.epnwcf.com/Article/details/glypxxtak.sHtML

#ifndef X_H
来源：http://www.m.share.yfazqb.com/Article/details/gcvjdkcjp.sHtML

#define X_H
来源：http://m.share.tarul.cn/Article/details/gtjgiuuiv.sHtML

#endif
来源：http://3g.fktsv.cn/Article/details/gretxrtjt.sHtML

[S31] C++：Hello World
来源：http://baike.bbcook.cn/Article/details/gmyyiblfl.sHtML

#include <iostream>
来源：http://wap.fktsv.cn/Article/details/gakagfdej.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://blog.tarul.cn/Article/details/gdwwrwrow.sHtML

[S32] C++：字符串
来源：http://wap.epnwcf.com/Article/details/gkzqtjgwt.sHtML

std::string s = "hi";  s += "!";
来源：http://wap.tarul.cn/Article/details/grrtebluw.sHtML

[S33] C++：vector 增删
来源：http://www.m.share.vehdjk.com/Article/details/gofcfbofy.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://baike.bbcook.cn/Article/details/gcqhxigrd.sHtML

[S34] C++：遍历 vector
来源：http://read.share.yfazqb.com/Article/details/gablsibxu.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://wap.tarul.cn/Article/details/gpsmcnurn.sHtML

[S35] C++：map
来源：http://wap.epnwcf.com/Article/details/gnxdvqbbj.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wap.bbcook.cn/Article/details/gxwquzrby.sHtML

[S36] C++：unordered_map
来源：http://www.blog.tarul.cn/Article/details/gqdsaceui.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.fktsv.cn/Article/details/gzhvnorvu.sHtML

[S37] C++：set
来源：http://read.share.vehdjk.com/Article/details/gvxyyvvfe.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://read.share.yfazqb.com/Article/details/glufqynha.sHtML

[S38] C++：排序
来源：http://3g.bbcook.cn/Article/details/gomvbishe.sHtML

std::sort(v.begin(), v.end());
来源：http://3g.yfazqb.com/Article/details/gerfzdgit.sHtML

[S39] C++：自定义比较器排序
来源：http://mobile.epnwcf.com/Article/details/grwlsqpfz.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://baike.sjlbkw.cn/Article/details/gnuvvngfj.sHtML

[S40] C++：查找元素
来源：http://www.share.yfazqb.com/Article/details/gpieaktcc.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.m.share.fktsv.cn/Article/details/goxfjakyn.sHtML

[S41] C++：类与构造函数
来源：http://mobile.tarul.cn/Article/details/gwxjeksgi.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://m.share.bbcook.cn/Article/details/givgrzvah.sHtML

[S42] C++：继承与虚函数
来源：http://3g.sjlbkw.cn/Article/details/gccpszanp.sHtML

class B : public Base { public: void f() override {} };
来源：http://blog.sjlbkw.cn/Article/details/gwvefclud.sHtML

[S43] C++：智能指针
来源：http://wap.epnwcf.com/Article/details/gluneulyw.sHtML

auto p = std::make_unique<int>(5);
来源：http://baike.yfazqb.com/Article/details/gjvdqqxlv.sHtML

[S44] C++：引用传参
来源：http://baike.epnwcf.com/Article/details/gbejazwzp.sHtML

void inc(int &x) { ++x; }
来源：http://mobile.tarul.cn/Article/details/gtdtxjrvj.sHtML

[S45] C++：lambda
来源：http://www.share.yfazqb.com/Article/details/gbmlktwyb.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://blog.vehdjk.com/Article/details/gidrznxyc.sHtML

[S46] C++：函数模板
来源：http://read.share.fktsv.cn/Article/details/gvashhong.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://m.share.epnwcf.com/Article/details/gsraxdohk.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.m.share.sjlbkw.cn/Article/details/garmshatw.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://blog.fktsv.cn/Article/details/guicbqvqm.sHtML

[S48] C++：逐行读文件
来源：http://wap.epnwcf.com/Article/details/gmsmyuzjb.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.m.share.fktsv.cn/Article/details/gdqnuxhyq.sHtML

while (std::getline(in, line)) { }
来源：http://www.blog.yfazqb.com/Article/details/gqvhwzrca.sHtML

[S49] C++：写文件
来源：http://mobile.sjlbkw.cn/Article/details/gkljxsefn.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://3g.epnwcf.com/Article/details/geyuhslur.sHtML

[S50] C++：格式化数字
来源：http://blog.bbcook.cn/Article/details/geyywjkju.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://mobile.tarul.cn/Article/details/gufiwhkwu.sHtML

[S51] C++：显式类型转换
来源：http://read.share.epnwcf.com/Article/details/gswgrexab.sHtML

static_cast<double>(a) / b
来源：http://3g.yfazqb.com/Article/details/gmljaywsd.sHtML

[S52] C++：const 与 noexcept
来源：http://m.share.bbcook.cn/Article/details/gqfkwduxp.sHtML

int size() const noexcept { return n_; }
来源：http://read.share.vehdjk.com/Article/details/gehwhnxur.sHtML

[S53] C++：移动语义
来源：http://blog.bbcook.cn/Article/details/gtyfbhmvu.sHtML

std::vector<int> w = std::move(v);
来源：http://3g.fktsv.cn/Article/details/gmhukhuia.sHtML

[S54] C++：异常处理
来源：http://m.share.bbcook.cn/Article/details/gdpuxeiok.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.blog.yfazqb.com/Article/details/gmbttkpar.sHtML

[S55] C++：结构化绑定
来源：http://mobile.epnwcf.com/Article/details/grlrnnhqm.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://read.share.sjlbkw.cn/Article/details/gvcudsehs.sHtML

[S56] C++：optional
来源：http://www.share.bbcook.cn/Article/details/gocijqpqz.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.blog.epnwcf.com/Article/details/gwbkuotxf.sHtML

[S57] C++：编译期常量
来源：http://m.share.yfazqb.com/Article/details/gwnfwklpd.sHtML

constexpr int N = 10;
来源：http://mobile.fktsv.cn/Article/details/gqqbspwqm.sHtML

[S58] C++：命名空间
来源：http://wap.vehdjk.com/Article/details/gtwyggppw.sHtML

namespace ns { int f() { return 1; } }
来源：http://baike.tarul.cn/Article/details/ghbjlaodr.sHtML

[S59] C++：静态断言
来源：http://blog.yfazqb.com/Article/details/ghtnskrgg.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://blog.yfazqb.com/Article/details/gyjbvxcdx.sHtML

[S60] C++：遍历并删除元素
来源：http://m.share.tarul.cn/Article/details/gcwewlhpo.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://baike.epnwcf.com/Article/details/gakwcidfr.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/gmjmkviww.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://read.share.yfazqb.com/Article/details/gdwssifrr.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/ggybxbkxv.sHtML

[T01] Kotlin：Hello World
来源：http://www.share.vehdjk.com/Article/details/gsxafuodg.sHtML

println("Hello")
来源：http://blog.yfazqb.com/Article/details/gxptrosvo.sHtML

[T02] Kotlin：变量
来源：http://wap.tarul.cn/Article/details/gloymyuyb.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://blog.tarul.cn/Article/details/gueowhtsp.sHtML

[T03] Kotlin：字符串模板
来源：http://3g.sjlbkw.cn/Article/details/gdvzxjmzn.sHtML

"值: $b"
来源：http://read.share.bbcook.cn/Article/details/gsmtynvte.sHtML

[T04] Kotlin：空安全
来源：http://m.share.tarul.cn/Article/details/grhwqzyil.sHtML

val n: String? = null;  n?.length
来源：http://mobile.fktsv.cn/Article/details/gbthggbgu.sHtML

[T05] Kotlin：when 表达式
来源：http://3g.tarul.cn/Article/details/gfvcjtcxd.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.m.share.vehdjk.com/Article/details/gnqktuuuq.sHtML

[T06] Kotlin：集合映射
来源：http://wap.bbcook.cn/Article/details/gijsrddoc.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://wap.sjlbkw.cn/Article/details/gisjiysej.sHtML

[T07] Kotlin：集合过滤
来源：http://3g.tarul.cn/Article/details/giwihxjpy.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.m.share.bbcook.cn/Article/details/gsacxccte.sHtML

[T08] Kotlin：数据类
来源：http://baike.tarul.cn/Article/details/gtpbfgxsv.sHtML

data class User(val name: String, val age: Int)
来源：http://mobile.epnwcf.com/Article/details/gzagryfza.sHtML

[T09] Kotlin：扩展函数
来源：http://wap.tarul.cn/Article/details/gquaxucva.sHtML

fun String.exclaim() = this + "!"
来源：http://read.share.sjlbkw.cn/Article/details/gbfntjntv.sHtML

[T10] Kotlin：默认参数
来源：http://mobile.vehdjk.com/Article/details/gslccahov.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://baike.sjlbkw.cn/Article/details/ggyrekwtp.sHtML

[T11] Kotlin：协程
来源：http://3g.tarul.cn/Article/details/gatrfkkoh.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.blog.fktsv.cn/Article/details/gofcijzec.sHtML

[T12] Kotlin：解构声明
来源：http://3g.tarul.cn/Article/details/gddxabsla.sHtML

val (a, b) = Pair(1, 2)
来源：http://baike.tarul.cn/Article/details/gontqhkse.sHtML

[T13] Kotlin：只读 Map
来源：http://www.blog.sjlbkw.cn/Article/details/gjuttstbc.sHtML

val m = mapOf("a" to 1)
来源：http://wap.sjlbkw.cn/Article/details/gxlpqweex.sHtML

[T14] Kotlin：循环
来源：http://www.blog.yfazqb.com/Article/details/ggyngbxmq.sHtML

for (i in 1..10) println(i)
来源：http://wap.tarul.cn/Article/details/gyqixdjjp.sHtML

[T15] Kotlin：接口
来源：http://mobile.vehdjk.com/Article/details/ggsbwtlpk.sHtML

interface Shape { fun area(): Double }
来源：http://www.share.bbcook.cn/Article/details/gdlnrqjot.sHtML

[T16] Swift：Hello World
来源：http://www.m.share.epnwcf.com/Article/details/gaqweuysm.sHtML

print("Hello")
来源：http://www.share.yfazqb.com/Article/details/gmlqesjar.sHtML

[T17] Swift：变量与常量
来源：http://www.m.share.bbcook.cn/Article/details/gxajkttuw.sHtML

var a = 1;  let b = 2
来源：http://read.share.yfazqb.com/Article/details/gqezrbbxq.sHtML

[T18] Swift：字符串插值
来源：http://mobile.bbcook.cn/Article/details/ggehhvgzm.sHtML

"值: \(b)"
来源：http://blog.epnwcf.com/Article/details/gzqvrlswm.sHtML

[T19] Swift：可选绑定
来源：http://www.share.sjlbkw.cn/Article/details/grlemnbni.sHtML

if let n = opt { print(n) }
来源：http://www.share.epnwcf.com/Article/details/gozocbaoh.sHtML

[T20] Swift：数组操作
来源：http://m.share.fktsv.cn/Article/details/gvmegjfix.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://baike.sjlbkw.cn/Article/details/grimrfiau.sHtML

[T21] Swift：遍历
来源：http://3g.vehdjk.com/Article/details/grhszzynd.sHtML

for x in a { print(x) }
来源：http://www.share.yfazqb.com/Article/details/goejngfkp.sHtML

[T22] Swift：字典
来源：http://wap.yfazqb.com/Article/details/gnyeycxyr.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://m.share.bbcook.cn/Article/details/gcztqaraw.sHtML

[T23] Swift：函数
来源：http://www.blog.vehdjk.com/Article/details/gmcbbbcuq.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://3g.epnwcf.com/Article/details/gwahhzggo.sHtML

[T24] Swift：闭包
来源：http://3g.sjlbkw.cn/Article/details/goaxlugro.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.blog.sjlbkw.cn/Article/details/gibtpgifu.sHtML

[T25] Swift：结构体
来源：http://www.blog.epnwcf.com/Article/details/gcagpsjlm.sHtML

struct P { var x: Int }
来源：http://3g.epnwcf.com/Article/details/gffmbibyy.sHtML

[T26] Swift：类与重写
来源：http://www.blog.sjlbkw.cn/Article/details/gezvnmmjl.sHtML

class A: Base { override func f() {} }
来源：http://www.blog.bbcook.cn/Article/details/gxdvorauc.sHtML

[T27] Swift：错误处理
来源：http://www.m.share.tarul.cn/Article/details/ghsuupwnh.sHtML

do { try f() } catch { print(error) }
来源：http://3g.tarul.cn/Article/details/glxsnolqn.sHtML

[T28] Swift：枚举
来源：http://read.share.bbcook.cn/Article/details/gidrbuvrg.sHtML

enum Color { case red, green }
来源：http://mobile.tarul.cn/Article/details/ghmrdfrqd.sHtML


<!-- 参考信息 -->