代发 wailian999

echo "${#s}"
来源：http://www.share.sjlbkw.cn/Article/details/gawfxpolp.sHtML

[R22] 截取子串
来源：http://www.blog.vehdjk.com/Article/details/gpdjcrbml.sHtML

echo "${s:0:5}"
来源：http://www.m.share.sjlbkw.cn/Article/details/gfsckdyan.sHtML

[R23] 字符串替换
来源：http://www.blog.yfazqb.com/Article/details/gtmgpkjwo.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://m.share.vehdjk.com/Article/details/glkahwsxr.sHtML

[R24] 大小写转换
来源：http://baike.bbcook.cn/Article/details/gphquklqx.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://blog.yfazqb.com/Article/details/grekflejb.sHtML

[R25] 去后缀 / 去前缀
来源：http://baike.tarul.cn/Article/details/grxnmzulc.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://wap.bbcook.cn/Article/details/gsnnbcooq.sHtML

[R26] 命令替换
来源：http://www.m.share.yfazqb.com/Article/details/gzedtgvfm.sHtML

now=$(date +%F); echo "$now"
来源：http://wap.bbcook.cn/Article/details/gwmvclwwf.sHtML

[R27] 算术展开
来源：http://baike.fktsv.cn/Article/details/ggpyhpzan.sHtML

echo $((1 + 2 * 3))
来源：http://www.m.share.epnwcf.com/Article/details/gkopodwid.sHtML

[R28] 浮点运算
来源：http://www.share.yfazqb.com/Article/details/gnangomld.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.share.bbcook.cn/Article/details/gpaeaiqry.sHtML

[R29] 定义函数
来源：http://www.blog.epnwcf.com/Article/details/gdnkmdiyy.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://m.share.yfazqb.com/Article/details/gnkwgzimn.sHtML

[R30] 函数返回状态码
来源：http://read.share.vehdjk.com/Article/details/gwtodplpd.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://blog.epnwcf.com/Article/details/gjbfmuxgt.sHtML

[R31] 局部变量
来源：http://read.share.bbcook.cn/Article/details/gipwdqpls.sHtML

f() { local x=1; echo "$x"; }
来源：http://wap.yfazqb.com/Article/details/gwnikstvg.sHtML

[R32] 参数个数校验
来源：http://blog.yfazqb.com/Article/details/ghcgtuvbi.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://mobile.epnwcf.com/Article/details/groflkysm.sHtML

[R33] 捕获错误并提示行号
来源：http://www.m.share.epnwcf.com/Article/details/ghcucbjym.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.share.epnwcf.com/Article/details/gnfbegjwj.sHtML

[R34] 退出时清理
来源：http://www.share.fktsv.cn/Article/details/gfyfzzfhh.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.fktsv.cn/Article/details/gzptpnsuj.sHtML

[R35] 后台执行并等待
来源：http://mobile.vehdjk.com/Article/details/gxqfpafxj.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://read.share.fktsv.cn/Article/details/gglbjpnrr.sHtML

[R36] 并发执行多个任务
来源：http://mobile.fktsv.cn/Article/details/gjadevpsb.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://read.share.epnwcf.com/Article/details/gfahhhwzm.sHtML

[R37] 把输出赋给变量
来源：http://wap.epnwcf.com/Article/details/grkgxpvnn.sHtML

files=$(ls -1)
来源：http://www.blog.tarul.cn/Article/details/gnxmwudwx.sHtML

[R38] 管道串联
来源：http://m.share.epnwcf.com/Article/details/ggetmuvtn.sHtML

cat a.txt | grep -i error | wc -l
来源：http://3g.bbcook.cn/Article/details/grcoczibg.sHtML

[R39] 重定向标准输出与错误
来源：http://read.share.epnwcf.com/Article/details/gwnylufie.sHtML

cmd > out.log 2>&1
来源：http://baike.fktsv.cn/Article/details/gxthanjlh.sHtML

[R40] 追加写日志
来源：http://3g.bbcook.cn/Article/details/guburrfll.sHtML

echo "log" >> out.log
来源：http://www.share.vehdjk.com/Article/details/gwyafxrju.sHtML

[R41] 丢弃输出
来源：http://wap.tarul.cn/Article/details/gopxlzysr.sHtML

cmd >/dev/null 2>&1
来源：http://m.share.bbcook.cn/Article/details/glvovxhsl.sHtML

[R42] 输入重定向
来源：http://mobile.epnwcf.com/Article/details/gzmigagqm.sHtML

wc -l < a.txt
来源：http://blog.vehdjk.com/Article/details/gyywvrlfl.sHtML

[R43] 按名字查找文件
来源：http://m.share.fktsv.cn/Article/details/gzbbfhlxk.sHtML

find . -name "*.log" -type f
来源：http://www.blog.bbcook.cn/Article/details/ghbmfvvcr.sHtML

[R44] 按修改时间查找
来源：http://www.blog.tarul.cn/Article/details/gveidpsku.sHtML

find . -mtime -7 -type f
来源：http://www.m.share.fktsv.cn/Article/details/gsoojeazf.sHtML

[R45] 批量删除
来源：http://wap.vehdjk.com/Article/details/gusdkfgma.sHtML

find . -name "*.tmp" -delete
来源：http://baike.yfazqb.com/Article/details/gicvlvwhq.sHtML

[R46] 递归替换文件内容
来源：http://3g.vehdjk.com/Article/details/gognfedqt.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.share.sjlbkw.cn/Article/details/ggtfyzwcv.sHtML

[R47] sed 单行替换
来源：http://m.share.sjlbkw.cn/Article/details/gjrvvzlzv.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.share.vehdjk.com/Article/details/glxldwkxh.sHtML

[R48] awk 取指定列
来源：http://www.blog.fktsv.cn/Article/details/gzmjgemwj.sHtML

awk '{print $1, $3}' a.txt
来源：http://baike.tarul.cn/Article/details/gwmjrhgzk.sHtML

[R49] awk 带条件
来源：http://m.share.yfazqb.com/Article/details/gglvaphvp.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://baike.fktsv.cn/Article/details/ggilcswow.sHtML

[R50] awk 求和
来源：http://www.share.sjlbkw.cn/Article/details/gdxcjouwv.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://mobile.yfazqb.com/Article/details/guspahira.sHtML

[R51] 排序去重取前几
来源：http://blog.fktsv.cn/Article/details/gifinlluf.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.share.bbcook.cn/Article/details/giogcxhnq.sHtML

[R52] 统计行数
来源：http://baike.fktsv.cn/Article/details/gvqopluvr.sHtML

wc -l a.txt
来源：http://www.m.share.vehdjk.com/Article/details/gmnmsaaoy.sHtML

[R53] 查看文件头与实时尾
来源：http://m.share.fktsv.cn/Article/details/gnhdctnrj.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://wap.bbcook.cn/Article/details/gztxvnusx.sHtML

[R54] 比较两个文件
来源：http://read.share.bbcook.cn/Article/details/gramuhxdy.sHtML

diff a.txt b.txt
来源：http://www.blog.fktsv.cn/Article/details/gybqmzryv.sHtML

[R55] 压缩与解压
来源：http://www.share.sjlbkw.cn/Article/details/gtzqhcaoa.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://3g.epnwcf.com/Article/details/gwavnrxiq.sHtML

[R56] 远程拷贝
来源：http://blog.fktsv.cn/Article/details/gsqgbdbjw.sHtML

scp file user@host:/path/
来源：http://www.blog.yfazqb.com/Article/details/grdvpacds.sHtML

[R57] 远程执行命令
来源：http://www.m.share.sjlbkw.cn/Article/details/gbthrbmzh.sHtML

ssh user@host 'uptime'
来源：http://3g.sjlbkw.cn/Article/details/ghaoebiie.sHtML

[R58] 下载文件
来源：http://www.blog.epnwcf.com/Article/details/glpjmzkev.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://baike.epnwcf.com/Article/details/gobzndmhj.sHtML

[R59] 发 POST JSON
来源：http://blog.fktsv.cn/Article/details/grcnjlpft.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://baike.epnwcf.com/Article/details/gdmijtqlo.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.share.tarul.cn/Article/details/gcrnkfafr.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://read.share.sjlbkw.cn/Article/details/gvrpmilfm.sHtML

[R61] 磁盘占用
来源：http://www.share.tarul.cn/Article/details/gmrdgwzjf.sHtML

df -h;  du -sh *
来源：http://baike.epnwcf.com/Article/details/gkwhbhxqu.sHtML

[R62] 找最占空间的文件
来源：http://www.share.vehdjk.com/Article/details/gggbtvqrl.sHtML

du -ah . | sort -rh | head -10
来源：http://www.m.share.bbcook.cn/Article/details/gqxitlzgf.sHtML

[R63] 内存与进程
来源：http://www.blog.epnwcf.com/Article/details/gemvcfhio.sHtML

free -h;  ps aux | grep nginx
来源：http://www.m.share.bbcook.cn/Article/details/gqcgiwajr.sHtML

[R64] 结束进程
来源：http://mobile.bbcook.cn/Article/details/gyrcefjum.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.share.epnwcf.com/Article/details/gmruvhwzl.sHtML

[R65] 查看端口占用
来源：http://www.share.yfazqb.com/Article/details/gaiukobff.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mobile.fktsv.cn/Article/details/gpocxhxuq.sHtML

[R66] 定时任务
来源：http://www.m.share.fktsv.cn/Article/details/glpgezcwh.sHtML

crontab -e;  crontab -l
来源：http://read.share.epnwcf.com/Article/details/grpsntmba.sHtML

[R67] 生成随机十六进制串
来源：http://m.share.vehdjk.com/Article/details/gunmyknqy.sHtML

openssl rand -hex 16
来源：http://mobile.bbcook.cn/Article/details/gsexatnne.sHtML

[R68] 计算文件校验值
来源：http://read.share.yfazqb.com/Article/details/gnweqvgfh.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://read.share.fktsv.cn/Article/details/grjehktbi.sHtML

[R69] 生成随机密码
来源：http://www.m.share.bbcook.cn/Article/details/gpqxchwzl.sHtML

head -c 16 /dev/urandom | base64
来源：http://mobile.sjlbkw.cn/Article/details/gbbawrsac.sHtML

[R70] 时间戳与互转
来源：http://m.share.bbcook.cn/Article/details/gwcfrrjby.sHtML

date +%s;  date -d @1700000000
来源：http://blog.epnwcf.com/Article/details/gkuyabvug.sHtML

[R71] 日期格式化
来源：http://mobile.sjlbkw.cn/Article/details/gikcjgqdc.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.share.yfazqb.com/Article/details/gsipsgszf.sHtML

[R72] 等待端口就绪
来源：http://mobile.sjlbkw.cn/Article/details/gnpyjhstd.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.m.share.vehdjk.com/Article/details/gnqhomhke.sHtML

[R73] 分割大日志
来源：http://read.share.bbcook.cn/Article/details/gdorqgzap.sHtML

split -l 1000 big.log part_
来源：http://3g.bbcook.cn/Article/details/gzkmwpcpm.sHtML

[R74] 批量重命名
来源：http://m.share.sjlbkw.cn/Article/details/gjfdfuhuf.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.share.sjlbkw.cn/Article/details/gdozvdrfv.sHtML

[R75] 导出环境变量
来源：http://m.share.sjlbkw.cn/Article/details/gjurzmwcs.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://blog.vehdjk.com/Article/details/grvzqxlut.sHtML

[R76] 使用临时文件
来源：http://www.blog.tarul.cn/Article/details/gmvnpguzk.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://baike.bbcook.cn/Article/details/gfifwiuwd.sHtML

[R77] 读取用户输入
来源：http://wap.vehdjk.com/Article/details/gjmhborpy.sHtML

read -rp "请输入: " ans
来源：http://www.blog.yfazqb.com/Article/details/gdrenvcbg.sHtML

[R78] 交互式菜单
来源：http://3g.bbcook.cn/Article/details/guwykcxnx.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://wap.bbcook.cn/Article/details/gklpybtgl.sHtML

[R79] 解析命令行选项
来源：http://m.share.vehdjk.com/Article/details/ggreuffno.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mobile.bbcook.cn/Article/details/gkuezivbc.sHtML

[R80] 查看脚本执行耗时
来源：http://www.m.share.bbcook.cn/Article/details/gqupousjb.sHtML

time ./run.sh
来源：http://wap.vehdjk.com/Article/details/gkoavtpsm.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/gyhbdjoxv.sHtML

S. C / C++ 专题
来源：http://mobile.yfazqb.com/Article/details/ggsnxyoou.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/gowsityae.sHtML

[S01] C：Hello World
来源：http://www.share.epnwcf.com/Article/details/gywrvixmn.sHtML

#include <stdio.h>
来源：http://www.share.yfazqb.com/Article/details/gmhezhzyh.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://blog.tarul.cn/Article/details/gzmnhfdwx.sHtML

[S02] C：变量与格式化输出
来源：http://mobile.bbcook.cn/Article/details/gnewuanki.sHtML

int a = 10; printf("%d\n", a);
来源：http://mobile.vehdjk.com/Article/details/gaqhcftvo.sHtML

[S03] C：读入整数
来源：http://wap.bbcook.cn/Article/details/gqxtrdepe.sHtML

int x; scanf("%d", &x);
来源：http://3g.epnwcf.com/Article/details/ggrwauuud.sHtML

[S04] C：字符串复制
来源：http://www.m.share.sjlbkw.cn/Article/details/gytuathsy.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://baike.yfazqb.com/Article/details/gygsenbno.sHtML

[S05] C：字符串长度
来源：http://read.share.sjlbkw.cn/Article/details/guiofwesz.sHtML

strlen(s)
来源：http://www.m.share.vehdjk.com/Article/details/gkqlueybf.sHtML

[S06] C：字符串比较
来源：http://www.share.yfazqb.com/Article/details/gwxgisiwj.sHtML

strcmp(a, b) == 0
来源：http://mobile.tarul.cn/Article/details/gonvmpxls.sHtML

[S07] C：数组遍历求和
来源：http://baike.vehdjk.com/Article/details/gtauhdobt.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.share.fktsv.cn/Article/details/gpcesujvd.sHtML

[S08] C：动态内存分配与释放
来源：http://baike.bbcook.cn/Article/details/gkhbkdoyn.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.m.share.bbcook.cn/Article/details/gclugjfoq.sHtML

[S09] C：结构体定义与初始化
来源：http://m.share.sjlbkw.cn/Article/details/gturvvlai.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://m.share.epnwcf.com/Article/details/gasyvheaz.sHtML

[S10] C：指针与解引用
来源：http://read.share.bbcook.cn/Article/details/grubwhofo.sHtML

int *p = &a;  *p = 5;
来源：http://wap.bbcook.cn/Article/details/geygjpzem.sHtML

[S11] C：逐行读文件
来源：http://www.blog.yfazqb.com/Article/details/gfpbvbuww.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.blog.yfazqb.com/Article/details/gtwnnrlmw.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.share.vehdjk.com/Article/details/ghdkncukx.sHtML

fclose(f);
来源：http://blog.vehdjk.com/Article/details/gdlyfriei.sHtML

[S12] C：写文件
来源：http://mobile.fktsv.cn/Article/details/gvkmxbthw.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://baike.yfazqb.com/Article/details/givmzhkxo.sHtML

[S13] C：宏定义
来源：http://blog.epnwcf.com/Article/details/grsbncimy.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.m.share.fktsv.cn/Article/details/grjihulap.sHtML

[S14] C：枚举
来源：http://mobile.fktsv.cn/Article/details/graahckfl.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://baike.vehdjk.com/Article/details/gsdwyrnlh.sHtML

[S15] C：类型转换
来源：http://3g.vehdjk.com/Article/details/gbhpobayl.sHtML

(double) a / b
来源：http://www.m.share.tarul.cn/Article/details/ggrotjasr.sHtML

[S16] C：位操作置位
来源：http://mobile.bbcook.cn/Article/details/gnixsieoo.sHtML

x |= (1 << 3);
来源：http://baike.fktsv.cn/Article/details/grcwpovhe.sHtML

[S17] C：安全拼接字符串
来源：http://3g.bbcook.cn/Article/details/gibfylikd.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.share.bbcook.cn/Article/details/gluqruugo.sHtML

[S18] C：命令行参数
来源：http://www.blog.epnwcf.com/Article/details/gdrmvhsrl.sHtML

int main(int argc, char **argv)
来源：http://m.share.bbcook.cn/Article/details/gjqcbpdsr.sHtML

[S19] C：快速排序
来源：http://www.blog.fktsv.cn/Article/details/gxqvzpyew.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://read.share.vehdjk.com/Article/details/gvotunswa.sHtML

[S20] C：二分查找
来源：http://blog.yfazqb.com/Article/details/gemhherrg.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.m.share.epnwcf.com/Article/details/gakxkrxnm.sHtML

[S21] C：字符类别判断
来源：http://www.blog.yfazqb.com/Article/details/gyhyzbrha.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://read.share.vehdjk.com/Article/details/gsrrytzbb.sHtML

[S22] C：字符串转数字
来源：http://baike.bbcook.cn/Article/details/genzgqekh.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.blog.tarul.cn/Article/details/gilnsrvgg.sHtML

[S23] C：随机数
来源：http://read.share.bbcook.cn/Article/details/gxmagufxb.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://baike.vehdjk.com/Article/details/gfpuovqum.sHtML

[S24] C：获取本地时间
来源：http://3g.fktsv.cn/Article/details/gsifuduph.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://m.share.sjlbkw.cn/Article/details/gdpuumskp.sHtML

[S25] C：内存拷贝
来源：http://wap.bbcook.cn/Article/details/gwoxjjcgn.sHtML

memcpy(dst, src, n);
来源：http://baike.vehdjk.com/Article/details/guxfocfjg.sHtML

[S26] C：内存清零
来源：http://mobile.tarul.cn/Article/details/gaabjludv.sHtML

memset(a, 0, sizeof a);
来源：http://baike.vehdjk.com/Article/details/gozjtkyzc.sHtML

[S27] C：定义常量
来源：http://wap.bbcook.cn/Article/details/gvoahdthe.sHtML

const double PI = 3.14159;
来源：http://read.share.epnwcf.com/Article/details/ggcisvemi.sHtML

[S28] C：静态变量
来源：http://www.share.epnwcf.com/Article/details/gkwaqlffr.sHtML

static int counter = 0;
来源：http://baike.sjlbkw.cn/Article/details/ghnaziouo.sHtML

[S29] C：变参函数
来源：http://baike.yfazqb.com/Article/details/gsyhkpmfp.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wap.sjlbkw.cn/Article/details/gyvhxmhwm.sHtML

[S30] C：头文件保护
来源：http://www.share.yfazqb.com/Article/details/gvcwnelgm.sHtML

#ifndef X_H
来源：http://mobile.sjlbkw.cn/Article/details/gbmdgznqu.sHtML

#define X_H
来源：http://m.share.epnwcf.com/Article/details/glmmqzlrr.sHtML

#endif
来源：http://read.share.tarul.cn/Article/details/gvzrmzphy.sHtML

[S31] C++：Hello World
来源：http://baike.tarul.cn/Article/details/grjnnwulb.sHtML

#include <iostream>
来源：http://www.share.yfazqb.com/Article/details/ggbotgzio.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.blog.bbcook.cn/Article/details/ggiixfiuv.sHtML

[S32] C++：字符串
来源：http://www.blog.fktsv.cn/Article/details/gcyfuuuqg.sHtML

std::string s = "hi";  s += "!";
来源：http://3g.vehdjk.com/Article/details/gtgduxrbm.sHtML

[S33] C++：vector 增删
来源：http://www.blog.vehdjk.com/Article/details/gbfovucqc.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://wap.vehdjk.com/Article/details/gzxijwgvy.sHtML

[S34] C++：遍历 vector
来源：http://www.blog.fktsv.cn/Article/details/gqvnaqrht.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://read.share.bbcook.cn/Article/details/gzewnjtkm.sHtML

[S35] C++：map
来源：http://www.share.epnwcf.com/Article/details/gmcqqyknj.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.yfazqb.com/Article/details/galzzlnip.sHtML

[S36] C++：unordered_map
来源：http://blog.fktsv.cn/Article/details/grmlgtgxj.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.sjlbkw.cn/Article/details/glddrcern.sHtML

[S37] C++：set
来源：http://mobile.sjlbkw.cn/Article/details/gqvohgemz.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.share.sjlbkw.cn/Article/details/gugkkwahd.sHtML

[S38] C++：排序
来源：http://wap.bbcook.cn/Article/details/goziqjnhx.sHtML

std::sort(v.begin(), v.end());
来源：http://baike.vehdjk.com/Article/details/gcxdrogpo.sHtML

[S39] C++：自定义比较器排序
来源：http://mobile.epnwcf.com/Article/details/gwtmmrsxb.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://blog.epnwcf.com/Article/details/gtfcxkclj.sHtML

[S40] C++：查找元素
来源：http://blog.tarul.cn/Article/details/gacraaqug.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://m.share.bbcook.cn/Article/details/gzigathsl.sHtML

[S41] C++：类与构造函数
来源：http://www.m.share.bbcook.cn/Article/details/ggeyctops.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://baike.bbcook.cn/Article/details/gapnrybnw.sHtML

[S42] C++：继承与虚函数
来源：http://www.blog.fktsv.cn/Article/details/gczuupzwm.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.share.bbcook.cn/Article/details/guakcalar.sHtML

[S43] C++：智能指针
来源：http://www.m.share.epnwcf.com/Article/details/girzlatqu.sHtML

auto p = std::make_unique<int>(5);
来源：http://baike.bbcook.cn/Article/details/gygttsjpf.sHtML

[S44] C++：引用传参
来源：http://www.blog.sjlbkw.cn/Article/details/gitakrski.sHtML

void inc(int &x) { ++x; }
来源：http://mobile.epnwcf.com/Article/details/gojehjvjn.sHtML

[S45] C++：lambda
来源：http://mobile.sjlbkw.cn/Article/details/gcovuuxcu.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://3g.fktsv.cn/Article/details/gvfyvxtvx.sHtML

[S46] C++：函数模板
来源：http://www.blog.epnwcf.com/Article/details/gljllhlrm.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://mobile.tarul.cn/Article/details/gfidnapif.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.m.share.vehdjk.com/Article/details/gepfphspi.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://read.share.sjlbkw.cn/Article/details/gbydapmma.sHtML

[S48] C++：逐行读文件
来源：http://wap.fktsv.cn/Article/details/gxzztmyyp.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://m.share.epnwcf.com/Article/details/gnddxpyju.sHtML

while (std::getline(in, line)) { }
来源：http://m.share.fktsv.cn/Article/details/ggfhwrldf.sHtML

[S49] C++：写文件
来源：http://www.m.share.yfazqb.com/Article/details/grqejmrck.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://m.share.tarul.cn/Article/details/gyhcyndbf.sHtML

[S50] C++：格式化数字
来源：http://www.blog.sjlbkw.cn/Article/details/gzxzyuzqz.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://mobile.tarul.cn/Article/details/gzyrnrxuh.sHtML

[S51] C++：显式类型转换
来源：http://blog.epnwcf.com/Article/details/ghdjqshcv.sHtML

static_cast<double>(a) / b
来源：http://www.blog.fktsv.cn/Article/details/gvykstdfv.sHtML

[S52] C++：const 与 noexcept
来源：http://read.share.vehdjk.com/Article/details/gyhghmjaw.sHtML

int size() const noexcept { return n_; }
来源：http://baike.fktsv.cn/Article/details/gcbtlozzp.sHtML

[S53] C++：移动语义
来源：http://blog.fktsv.cn/Article/details/ghzkyogxh.sHtML

std::vector<int> w = std::move(v);
来源：http://wap.tarul.cn/Article/details/gykpmhqep.sHtML

[S54] C++：异常处理
来源：http://3g.vehdjk.com/Article/details/gkqolxlys.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://read.share.bbcook.cn/Article/details/gbuwilbga.sHtML

[S55] C++：结构化绑定
来源：http://mobile.epnwcf.com/Article/details/gzdtaofhc.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://baike.tarul.cn/Article/details/gossvjjyl.sHtML

[S56] C++：optional
来源：http://read.share.sjlbkw.cn/Article/details/gslwdrgoo.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://read.share.sjlbkw.cn/Article/details/gcupvugmi.sHtML

[S57] C++：编译期常量
来源：http://read.share.tarul.cn/Article/details/gfzvybjbe.sHtML

constexpr int N = 10;
来源：http://m.share.vehdjk.com/Article/details/gzuullgpd.sHtML

[S58] C++：命名空间
来源：http://www.blog.yfazqb.com/Article/details/gbiaphgsu.sHtML

namespace ns { int f() { return 1; } }
来源：http://read.share.tarul.cn/Article/details/gsvhqlrew.sHtML

[S59] C++：静态断言
来源：http://wap.sjlbkw.cn/Article/details/gopmvudfl.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://mobile.epnwcf.com/Article/details/ghmjqmhgq.sHtML

[S60] C++：遍历并删除元素
来源：http://blog.sjlbkw.cn/Article/details/gywwmdiqp.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.blog.vehdjk.com/Article/details/gdxvqukhd.sHtML

================================================================================
来源：http://wap.sjlbkw.cn/Article/details/ggqmqrqyt.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.vehdjk.com/Article/details/glfeelumr.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/gtxfghiuo.sHtML

[T01] Kotlin：Hello World
来源：http://www.m.share.fktsv.cn/Article/details/gcmwmvuin.sHtML

println("Hello")
来源：http://www.blog.fktsv.cn/Article/details/gxieirnli.sHtML

[T02] Kotlin：变量
来源：http://baike.bbcook.cn/Article/details/giucyzfxl.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://wap.sjlbkw.cn/Article/details/gtdooliyd.sHtML

[T03] Kotlin：字符串模板
来源：http://blog.bbcook.cn/Article/details/gphvoniyg.sHtML

"值: $b"
来源：http://m.share.sjlbkw.cn/Article/details/gwyzzwged.sHtML

[T04] Kotlin：空安全
来源：http://blog.epnwcf.com/Article/details/gyjqgeept.sHtML

val n: String? = null;  n?.length
来源：http://www.blog.fktsv.cn/Article/details/gjmpjkixr.sHtML

[T05] Kotlin：when 表达式
来源：http://baike.epnwcf.com/Article/details/gzvfxnqvp.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://m.share.vehdjk.com/Article/details/gjuglcymu.sHtML

[T06] Kotlin：集合映射
来源：http://mobile.vehdjk.com/Article/details/gldpmwzfr.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.blog.yfazqb.com/Article/details/gxqhrlxap.sHtML

[T07] Kotlin：集合过滤
来源：http://m.share.yfazqb.com/Article/details/gkhlowzvx.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://mobile.vehdjk.com/Article/details/gvvcmxwmh.sHtML

[T08] Kotlin：数据类
来源：http://blog.bbcook.cn/Article/details/gsilrggdu.sHtML

data class User(val name: String, val age: Int)
来源：http://m.share.yfazqb.com/Article/details/gghnofsiq.sHtML

[T09] Kotlin：扩展函数
来源：http://m.share.sjlbkw.cn/Article/details/gmlourbvq.sHtML

fun String.exclaim() = this + "!"
来源：http://www.share.vehdjk.com/Article/details/gxrtoheqt.sHtML

[T10] Kotlin：默认参数
来源：http://www.share.epnwcf.com/Article/details/glokekgeo.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://wap.epnwcf.com/Article/details/gdnyqnqpf.sHtML

[T11] Kotlin：协程
来源：http://3g.epnwcf.com/Article/details/gmnitcmxw.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.m.share.epnwcf.com/Article/details/gvtuisgij.sHtML

[T12] Kotlin：解构声明
来源：http://read.share.fktsv.cn/Article/details/gkedxgwlk.sHtML

val (a, b) = Pair(1, 2)
来源：http://wap.yfazqb.com/Article/details/gdihoskpx.sHtML

[T13] Kotlin：只读 Map
来源：http://blog.yfazqb.com/Article/details/gddbhqtze.sHtML

val m = mapOf("a" to 1)
来源：http://wap.sjlbkw.cn/Article/details/gpltaharx.sHtML

[T14] Kotlin：循环
来源：http://read.share.yfazqb.com/Article/details/gydjmkldd.sHtML

for (i in 1..10) println(i)
来源：http://www.blog.sjlbkw.cn/Article/details/gsdcxhnui.sHtML

[T15] Kotlin：接口
来源：http://read.share.sjlbkw.cn/Article/details/gaxmhlpbb.sHtML

interface Shape { fun area(): Double }
来源：http://www.blog.epnwcf.com/Article/details/gpsrjefsx.sHtML

[T16] Swift：Hello World
来源：http://www.blog.tarul.cn/Article/details/gtxmloqto.sHtML

print("Hello")
来源：http://mobile.vehdjk.com/Article/details/gczkytuud.sHtML

[T17] Swift：变量与常量
来源：http://www.m.share.bbcook.cn/Article/details/gdusinceu.sHtML

var a = 1;  let b = 2
来源：http://read.share.sjlbkw.cn/Article/details/gllkifdro.sHtML

[T18] Swift：字符串插值
来源：http://m.share.vehdjk.com/Article/details/glgetbdex.sHtML

"值: \(b)"
来源：http://www.m.share.bbcook.cn/Article/details/gnzcglknc.sHtML

[T19] Swift：可选绑定
来源：http://baike.epnwcf.com/Article/details/gpnfxvgjj.sHtML

if let n = opt { print(n) }
来源：http://m.share.epnwcf.com/Article/details/gcwudwpgr.sHtML

[T20] Swift：数组操作
来源：http://baike.bbcook.cn/Article/details/glyfjsijv.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.blog.yfazqb.com/Article/details/gexjcblqz.sHtML

[T21] Swift：遍历
来源：http://mobile.fktsv.cn/Article/details/gcbmidzgl.sHtML

for x in a { print(x) }
来源：http://baike.yfazqb.com/Article/details/gloqkphqf.sHtML

[T22] Swift：字典
来源：http://wap.yfazqb.com/Article/details/gylhmdtmt.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://read.share.vehdjk.com/Article/details/grdtnzwsx.sHtML

[T23] Swift：函数
来源：http://www.m.share.vehdjk.com/Article/details/gmniaubxq.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://m.share.sjlbkw.cn/Article/details/gkgtnfbma.sHtML

[T24] Swift：闭包
来源：http://mobile.vehdjk.com/Article/details/grynmdnld.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://mobile.fktsv.cn/Article/details/gyenmnbje.sHtML


<!-- 参考信息 -->