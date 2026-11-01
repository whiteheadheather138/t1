代发 wailian999

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://m.share.sjlbkw.cn/Article/details/geijvihet.sHtML

[R24] 大小写转换
来源：http://3g.vehdjk.com/Article/details/gxinuqfwq.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://baike.vehdjk.com/Article/details/gshbxyoux.sHtML

[R25] 去后缀 / 去前缀
来源：http://m.share.sjlbkw.cn/Article/details/gwhhaaqae.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://blog.tarul.cn/Article/details/gxlwnqukr.sHtML

[R26] 命令替换
来源：http://baike.vehdjk.com/Article/details/golusbzwq.sHtML

now=$(date +%F); echo "$now"
来源：http://blog.sjlbkw.cn/Article/details/gdipxoeyk.sHtML

[R27] 算术展开
来源：http://mobile.tarul.cn/Article/details/gxmbtbhbe.sHtML

echo $((1 + 2 * 3))
来源：http://wap.fktsv.cn/Article/details/gydzgllqy.sHtML

[R28] 浮点运算
来源：http://www.m.share.yfazqb.com/Article/details/gwkgutrhi.sHtML

echo "scale=2; 10/3" | bc
来源：http://wap.fktsv.cn/Article/details/gfpealwvs.sHtML

[R29] 定义函数
来源：http://www.m.share.epnwcf.com/Article/details/grpjghhpw.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://mobile.epnwcf.com/Article/details/gktbeqnal.sHtML

[R30] 函数返回状态码
来源：http://blog.yfazqb.com/Article/details/gfgczjlxe.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://m.share.tarul.cn/Article/details/gpizpymvi.sHtML

[R31] 局部变量
来源：http://m.share.epnwcf.com/Article/details/ggkamckrw.sHtML

f() { local x=1; echo "$x"; }
来源：http://3g.yfazqb.com/Article/details/gslxtndcg.sHtML

[R32] 参数个数校验
来源：http://blog.epnwcf.com/Article/details/gjntmmsuf.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://read.share.tarul.cn/Article/details/gzzrgqada.sHtML

[R33] 捕获错误并提示行号
来源：http://www.blog.yfazqb.com/Article/details/gikanpcob.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://3g.vehdjk.com/Article/details/gpeayrdju.sHtML

[R34] 退出时清理
来源：http://mobile.epnwcf.com/Article/details/gnrzfucem.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.share.tarul.cn/Article/details/gydmgjuzn.sHtML

[R35] 后台执行并等待
来源：http://read.share.vehdjk.com/Article/details/gflnnbgwq.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.m.share.vehdjk.com/Article/details/gkllmrcts.sHtML

[R36] 并发执行多个任务
来源：http://wap.yfazqb.com/Article/details/gvdydmmac.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://read.share.bbcook.cn/Article/details/gocaiewii.sHtML

[R37] 把输出赋给变量
来源：http://www.blog.yfazqb.com/Article/details/gxgregvjl.sHtML

files=$(ls -1)
来源：http://www.share.fktsv.cn/Article/details/gkbdsmuny.sHtML

[R38] 管道串联
来源：http://m.share.vehdjk.com/Article/details/grpotcvfn.sHtML

cat a.txt | grep -i error | wc -l
来源：http://baike.fktsv.cn/Article/details/gucqykawy.sHtML

[R39] 重定向标准输出与错误
来源：http://mobile.tarul.cn/Article/details/gyilpvmik.sHtML

cmd > out.log 2>&1
来源：http://www.share.epnwcf.com/Article/details/guctazxah.sHtML

[R40] 追加写日志
来源：http://www.blog.tarul.cn/Article/details/gobfprvse.sHtML

echo "log" >> out.log
来源：http://baike.sjlbkw.cn/Article/details/gieaxpvhl.sHtML

[R41] 丢弃输出
来源：http://wap.vehdjk.com/Article/details/gfytwrqxi.sHtML

cmd >/dev/null 2>&1
来源：http://wap.bbcook.cn/Article/details/gobhrckmh.sHtML

[R42] 输入重定向
来源：http://3g.fktsv.cn/Article/details/gjcacexxg.sHtML

wc -l < a.txt
来源：http://wap.bbcook.cn/Article/details/gzebzrgzt.sHtML

[R43] 按名字查找文件
来源：http://mobile.yfazqb.com/Article/details/gphfmujbi.sHtML

find . -name "*.log" -type f
来源：http://baike.yfazqb.com/Article/details/ggppvjfco.sHtML

[R44] 按修改时间查找
来源：http://www.share.epnwcf.com/Article/details/gnfudoamd.sHtML

find . -mtime -7 -type f
来源：http://wap.sjlbkw.cn/Article/details/gadmnoebe.sHtML

[R45] 批量删除
来源：http://wap.tarul.cn/Article/details/ggpcjuvrp.sHtML

find . -name "*.tmp" -delete
来源：http://www.m.share.sjlbkw.cn/Article/details/gwnxbfbvu.sHtML

[R46] 递归替换文件内容
来源：http://mobile.yfazqb.com/Article/details/grbblshdv.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mobile.fktsv.cn/Article/details/gwffcunpz.sHtML

[R47] sed 单行替换
来源：http://baike.vehdjk.com/Article/details/gmsbkiupv.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://m.share.fktsv.cn/Article/details/gafadobhd.sHtML

[R48] awk 取指定列
来源：http://www.blog.vehdjk.com/Article/details/gilwvvjdi.sHtML

awk '{print $1, $3}' a.txt
来源：http://wap.vehdjk.com/Article/details/gzlyycsbi.sHtML

[R49] awk 带条件
来源：http://www.m.share.yfazqb.com/Article/details/gzmqzgxbs.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://blog.vehdjk.com/Article/details/gsthnysjd.sHtML

[R50] awk 求和
来源：http://mobile.fktsv.cn/Article/details/glgcsowvh.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://baike.bbcook.cn/Article/details/gzwsaofkg.sHtML

[R51] 排序去重取前几
来源：http://www.blog.tarul.cn/Article/details/gxbwldqks.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://wap.yfazqb.com/Article/details/gtvjdwldl.sHtML

[R52] 统计行数
来源：http://3g.tarul.cn/Article/details/geuikuiqy.sHtML

wc -l a.txt
来源：http://blog.fktsv.cn/Article/details/gxdxlvptn.sHtML

[R53] 查看文件头与实时尾
来源：http://www.blog.vehdjk.com/Article/details/gasndhixd.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://mobile.epnwcf.com/Article/details/glhfnhcxt.sHtML

[R54] 比较两个文件
来源：http://mobile.fktsv.cn/Article/details/gwfymigko.sHtML

diff a.txt b.txt
来源：http://www.m.share.tarul.cn/Article/details/gvagsnoca.sHtML

[R55] 压缩与解压
来源：http://read.share.sjlbkw.cn/Article/details/gcspahbzp.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.blog.yfazqb.com/Article/details/gjwmdggmp.sHtML

[R56] 远程拷贝
来源：http://3g.tarul.cn/Article/details/gvbruktrn.sHtML

scp file user@host:/path/
来源：http://mobile.yfazqb.com/Article/details/gepebfufg.sHtML

[R57] 远程执行命令
来源：http://m.share.sjlbkw.cn/Article/details/gtbodbtfz.sHtML

ssh user@host 'uptime'
来源：http://baike.vehdjk.com/Article/details/ghdbscont.sHtML

[R58] 下载文件
来源：http://baike.vehdjk.com/Article/details/gbbxasmvs.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://wap.epnwcf.com/Article/details/gjaxvqheb.sHtML

[R59] 发 POST JSON
来源：http://www.share.fktsv.cn/Article/details/gpthqgxlg.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://read.share.fktsv.cn/Article/details/gqnzjykvf.sHtML

[R60] 只看 HTTP 状态码
来源：http://read.share.yfazqb.com/Article/details/gqqiiobuz.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://blog.fktsv.cn/Article/details/gmfpkbvzr.sHtML

[R61] 磁盘占用
来源：http://baike.sjlbkw.cn/Article/details/gsbemuvyd.sHtML

df -h;  du -sh *
来源：http://wap.sjlbkw.cn/Article/details/grsvfghrf.sHtML

[R62] 找最占空间的文件
来源：http://3g.epnwcf.com/Article/details/gksljgnsj.sHtML

du -ah . | sort -rh | head -10
来源：http://baike.epnwcf.com/Article/details/gcpfbaflp.sHtML

[R63] 内存与进程
来源：http://read.share.tarul.cn/Article/details/gxkxmeaeg.sHtML

free -h;  ps aux | grep nginx
来源：http://www.share.bbcook.cn/Article/details/ggokdvbxi.sHtML

[R64] 结束进程
来源：http://read.share.vehdjk.com/Article/details/gjjzftzam.sHtML

kill -9 $(pgrep -f app.py)
来源：http://blog.vehdjk.com/Article/details/gwlhobnji.sHtML

[R65] 查看端口占用
来源：http://wap.vehdjk.com/Article/details/gpmzcypcx.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://baike.fktsv.cn/Article/details/guvbesqku.sHtML

[R66] 定时任务
来源：http://wap.vehdjk.com/Article/details/gtmwprdvx.sHtML

crontab -e;  crontab -l
来源：http://blog.vehdjk.com/Article/details/gvffopumw.sHtML

[R67] 生成随机十六进制串
来源：http://blog.bbcook.cn/Article/details/gmyxojfdg.sHtML

openssl rand -hex 16
来源：http://m.share.fktsv.cn/Article/details/gmgbhgiuf.sHtML

[R68] 计算文件校验值
来源：http://blog.bbcook.cn/Article/details/gxnuackvj.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.share.epnwcf.com/Article/details/gledvpikd.sHtML

[R69] 生成随机密码
来源：http://www.m.share.yfazqb.com/Article/details/gmzffinga.sHtML

head -c 16 /dev/urandom | base64
来源：http://blog.vehdjk.com/Article/details/gyvpemepb.sHtML

[R70] 时间戳与互转
来源：http://read.share.vehdjk.com/Article/details/gqccqzxnb.sHtML

date +%s;  date -d @1700000000
来源：http://www.share.fktsv.cn/Article/details/grrmtxkjm.sHtML

[R71] 日期格式化
来源：http://baike.bbcook.cn/Article/details/gictftqew.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://read.share.epnwcf.com/Article/details/gltpdrvin.sHtML

[R72] 等待端口就绪
来源：http://www.blog.yfazqb.com/Article/details/ghotzmcco.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://baike.tarul.cn/Article/details/gopeugkew.sHtML

[R73] 分割大日志
来源：http://www.m.share.vehdjk.com/Article/details/glnptghco.sHtML

split -l 1000 big.log part_
来源：http://m.share.vehdjk.com/Article/details/gwjuxigrj.sHtML

[R74] 批量重命名
来源：http://www.blog.yfazqb.com/Article/details/gtsiqomhx.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.m.share.tarul.cn/Article/details/grdavayhk.sHtML

[R75] 导出环境变量
来源：http://3g.vehdjk.com/Article/details/gkdhfjxvi.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.blog.tarul.cn/Article/details/gsbngxdoa.sHtML

[R76] 使用临时文件
来源：http://baike.fktsv.cn/Article/details/gkaddbrvg.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://wap.fktsv.cn/Article/details/ghnwmnlgy.sHtML

[R77] 读取用户输入
来源：http://mobile.fktsv.cn/Article/details/gqekxylhi.sHtML

read -rp "请输入: " ans
来源：http://read.share.fktsv.cn/Article/details/gecvlenlt.sHtML

[R78] 交互式菜单
来源：http://blog.fktsv.cn/Article/details/grisvhfir.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://read.share.sjlbkw.cn/Article/details/gldsypryg.sHtML

[R79] 解析命令行选项
来源：http://www.blog.bbcook.cn/Article/details/gmkfnmjsf.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.share.epnwcf.com/Article/details/gattjxjfk.sHtML

[R80] 查看脚本执行耗时
来源：http://www.blog.epnwcf.com/Article/details/glxuvkzfd.sHtML

time ./run.sh
来源：http://www.share.vehdjk.com/Article/details/ggjacxjie.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/gfsdxsjje.sHtML

S. C / C++ 专题
来源：http://www.m.share.sjlbkw.cn/Article/details/gxdmiwbcl.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/gmolbhqqo.sHtML

[S01] C：Hello World
来源：http://mobile.vehdjk.com/Article/details/gmlyrqrng.sHtML

#include <stdio.h>
来源：http://3g.epnwcf.com/Article/details/gcevnxkkb.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.share.vehdjk.com/Article/details/gmybhkstj.sHtML

[S02] C：变量与格式化输出
来源：http://mobile.tarul.cn/Article/details/ghfyposmz.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.m.share.sjlbkw.cn/Article/details/gkpunwqpd.sHtML

[S03] C：读入整数
来源：http://blog.epnwcf.com/Article/details/gzudppbnl.sHtML

int x; scanf("%d", &x);
来源：http://www.blog.tarul.cn/Article/details/gsbhpizui.sHtML

[S04] C：字符串复制
来源：http://m.share.bbcook.cn/Article/details/gqjliaslv.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://m.share.fktsv.cn/Article/details/goomghjyk.sHtML

[S05] C：字符串长度
来源：http://www.m.share.epnwcf.com/Article/details/gdjwnfxbt.sHtML

strlen(s)
来源：http://3g.yfazqb.com/Article/details/gwbvvhbdv.sHtML

[S06] C：字符串比较
来源：http://m.share.sjlbkw.cn/Article/details/gkoqkdtsd.sHtML

strcmp(a, b) == 0
来源：http://baike.tarul.cn/Article/details/gqbjzzsfu.sHtML

[S07] C：数组遍历求和
来源：http://3g.yfazqb.com/Article/details/gtpxqffno.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://mobile.vehdjk.com/Article/details/gsrfbhqvc.sHtML

[S08] C：动态内存分配与释放
来源：http://read.share.epnwcf.com/Article/details/gqsdjiiij.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://read.share.epnwcf.com/Article/details/gzbyqpuab.sHtML

[S09] C：结构体定义与初始化
来源：http://www.m.share.yfazqb.com/Article/details/gwysvaoly.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.share.sjlbkw.cn/Article/details/gnxoabeyy.sHtML

[S10] C：指针与解引用
来源：http://3g.tarul.cn/Article/details/gelgprlhw.sHtML

int *p = &a;  *p = 5;
来源：http://blog.tarul.cn/Article/details/ggswzrkkm.sHtML

[S11] C：逐行读文件
来源：http://www.share.epnwcf.com/Article/details/gowzndfso.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://blog.yfazqb.com/Article/details/gjqfriljo.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://blog.yfazqb.com/Article/details/gcibrgimc.sHtML

fclose(f);
来源：http://www.m.share.bbcook.cn/Article/details/gfowudbbf.sHtML

[S12] C：写文件
来源：http://www.blog.sjlbkw.cn/Article/details/grimtwaan.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://3g.epnwcf.com/Article/details/gezswnvqb.sHtML

[S13] C：宏定义
来源：http://baike.vehdjk.com/Article/details/gkhjmauhw.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://blog.fktsv.cn/Article/details/ggdncaciz.sHtML

[S14] C：枚举
来源：http://wap.bbcook.cn/Article/details/gnggjwyju.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://read.share.tarul.cn/Article/details/gxmzlzjnt.sHtML

[S15] C：类型转换
来源：http://blog.tarul.cn/Article/details/gtazqehpd.sHtML

(double) a / b
来源：http://baike.sjlbkw.cn/Article/details/gfzlygpsn.sHtML

[S16] C：位操作置位
来源：http://blog.epnwcf.com/Article/details/gyjqvuwxr.sHtML

x |= (1 << 3);
来源：http://blog.bbcook.cn/Article/details/gbwhsimnh.sHtML

[S17] C：安全拼接字符串
来源：http://mobile.tarul.cn/Article/details/gumjqemae.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://blog.vehdjk.com/Article/details/gomzanljb.sHtML

[S18] C：命令行参数
来源：http://3g.fktsv.cn/Article/details/gioqrtyzu.sHtML

int main(int argc, char **argv)
来源：http://mobile.sjlbkw.cn/Article/details/gocdkolpu.sHtML

[S19] C：快速排序
来源：http://www.m.share.sjlbkw.cn/Article/details/gkrnmnpcs.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://m.share.sjlbkw.cn/Article/details/gdtmgmhsl.sHtML

[S20] C：二分查找
来源：http://baike.vehdjk.com/Article/details/gkgxmmrxu.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.share.epnwcf.com/Article/details/gmqgjpyyo.sHtML

[S21] C：字符类别判断
来源：http://www.share.bbcook.cn/Article/details/gboscyoen.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://3g.epnwcf.com/Article/details/gjujgxayg.sHtML

[S22] C：字符串转数字
来源：http://www.m.share.vehdjk.com/Article/details/gogbrdsrg.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://mobile.epnwcf.com/Article/details/gojbkcvfn.sHtML

[S23] C：随机数
来源：http://blog.sjlbkw.cn/Article/details/gzyfoqbet.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://mobile.bbcook.cn/Article/details/grctjvawh.sHtML

[S24] C：获取本地时间
来源：http://3g.tarul.cn/Article/details/ggtctqyly.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://3g.bbcook.cn/Article/details/gdushkhos.sHtML

[S25] C：内存拷贝
来源：http://mobile.bbcook.cn/Article/details/gxssbbuvo.sHtML

memcpy(dst, src, n);
来源：http://3g.yfazqb.com/Article/details/grmlkaplp.sHtML

[S26] C：内存清零
来源：http://read.share.yfazqb.com/Article/details/gcbspwyix.sHtML

memset(a, 0, sizeof a);
来源：http://3g.sjlbkw.cn/Article/details/ghyszulrz.sHtML

[S27] C：定义常量
来源：http://www.blog.sjlbkw.cn/Article/details/ghvdkdvdw.sHtML

const double PI = 3.14159;
来源：http://wap.bbcook.cn/Article/details/gbaiskfqd.sHtML

[S28] C：静态变量
来源：http://wap.vehdjk.com/Article/details/gpeulplxo.sHtML

static int counter = 0;
来源：http://mobile.sjlbkw.cn/Article/details/gvultsahw.sHtML

[S29] C：变参函数
来源：http://mobile.epnwcf.com/Article/details/gggibjrzk.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.share.epnwcf.com/Article/details/gltzfsxzh.sHtML

[S30] C：头文件保护
来源：http://wap.bbcook.cn/Article/details/gppjfqsmj.sHtML

#ifndef X_H
来源：http://www.share.epnwcf.com/Article/details/gnhvwxudv.sHtML

#define X_H
来源：http://mobile.sjlbkw.cn/Article/details/gfcmuskzt.sHtML

#endif
来源：http://www.share.tarul.cn/Article/details/gqinffzsw.sHtML

[S31] C++：Hello World
来源：http://read.share.epnwcf.com/Article/details/glcbupvpq.sHtML

#include <iostream>
来源：http://baike.epnwcf.com/Article/details/gsjjtygwe.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://3g.yfazqb.com/Article/details/gjznckloq.sHtML

[S32] C++：字符串
来源：http://blog.tarul.cn/Article/details/gmbljppcb.sHtML

std::string s = "hi";  s += "!";
来源：http://mobile.sjlbkw.cn/Article/details/gkjnwcoim.sHtML

[S33] C++：vector 增删
来源：http://www.blog.bbcook.cn/Article/details/gknifyiig.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://read.share.tarul.cn/Article/details/gwywofvpx.sHtML

[S34] C++：遍历 vector
来源：http://www.share.fktsv.cn/Article/details/gfhpebkrb.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://mobile.vehdjk.com/Article/details/geibmheqm.sHtML

[S35] C++：map
来源：http://wap.sjlbkw.cn/Article/details/gxwyhcbgd.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://blog.yfazqb.com/Article/details/guprevtiy.sHtML

[S36] C++：unordered_map
来源：http://baike.yfazqb.com/Article/details/gknubuyng.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.yfazqb.com/Article/details/gegnilivp.sHtML

[S37] C++：set
来源：http://blog.fktsv.cn/Article/details/gfcnshqkf.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.blog.epnwcf.com/Article/details/gforuxtap.sHtML

[S38] C++：排序
来源：http://wap.sjlbkw.cn/Article/details/gonlyeqhq.sHtML

std::sort(v.begin(), v.end());
来源：http://baike.sjlbkw.cn/Article/details/gmrwcmnah.sHtML

[S39] C++：自定义比较器排序
来源：http://www.m.share.yfazqb.com/Article/details/gtdylilio.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://blog.epnwcf.com/Article/details/gtqlncntx.sHtML

[S40] C++：查找元素
来源：http://www.blog.sjlbkw.cn/Article/details/gxcjwrczc.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.blog.epnwcf.com/Article/details/gedpbmwmm.sHtML

[S41] C++：类与构造函数
来源：http://wap.tarul.cn/Article/details/gkqnhzjke.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://baike.yfazqb.com/Article/details/gretmpoic.sHtML

[S42] C++：继承与虚函数
来源：http://baike.sjlbkw.cn/Article/details/ghnuwgrqn.sHtML

class B : public Base { public: void f() override {} };
来源：http://wap.yfazqb.com/Article/details/glsnimdhs.sHtML

[S43] C++：智能指针
来源：http://read.share.epnwcf.com/Article/details/gkyvreuwa.sHtML

auto p = std::make_unique<int>(5);
来源：http://m.share.fktsv.cn/Article/details/grwentwmt.sHtML

[S44] C++：引用传参
来源：http://www.m.share.vehdjk.com/Article/details/getyzoafs.sHtML

void inc(int &x) { ++x; }
来源：http://blog.sjlbkw.cn/Article/details/gyxckrtwv.sHtML

[S45] C++：lambda
来源：http://www.blog.epnwcf.com/Article/details/gjgqlnuyo.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.share.sjlbkw.cn/Article/details/gdrsmnhnu.sHtML

[S46] C++：函数模板
来源：http://www.share.yfazqb.com/Article/details/gdxhdtomb.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.blog.sjlbkw.cn/Article/details/gozqnrxyb.sHtML

[S47] C++：结构化绑定遍历
来源：http://m.share.fktsv.cn/Article/details/gqdqefegq.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://3g.tarul.cn/Article/details/gsxsbbkom.sHtML

[S48] C++：逐行读文件
来源：http://www.m.share.vehdjk.com/Article/details/gkbvfbopw.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://blog.vehdjk.com/Article/details/grbfyvnph.sHtML

while (std::getline(in, line)) { }
来源：http://m.share.yfazqb.com/Article/details/goveujooi.sHtML

[S49] C++：写文件
来源：http://www.blog.vehdjk.com/Article/details/gnlbjibtx.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://m.share.epnwcf.com/Article/details/ghmpygnzj.sHtML

[S50] C++：格式化数字
来源：http://www.blog.fktsv.cn/Article/details/gnazmlrgl.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.blog.bbcook.cn/Article/details/gcoplgwdy.sHtML

[S51] C++：显式类型转换
来源：http://mobile.fktsv.cn/Article/details/gcodlnmqv.sHtML

static_cast<double>(a) / b
来源：http://baike.vehdjk.com/Article/details/gqsowjdyn.sHtML

[S52] C++：const 与 noexcept
来源：http://wap.bbcook.cn/Article/details/gjzfbsrfh.sHtML

int size() const noexcept { return n_; }
来源：http://www.m.share.tarul.cn/Article/details/gipdjxvjm.sHtML

[S53] C++：移动语义
来源：http://wap.tarul.cn/Article/details/gomqpnkbk.sHtML

std::vector<int> w = std::move(v);
来源：http://3g.vehdjk.com/Article/details/gdcdigsjo.sHtML

[S54] C++：异常处理
来源：http://3g.tarul.cn/Article/details/gtzfgxeuv.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://wap.bbcook.cn/Article/details/garrimwbl.sHtML

[S55] C++：结构化绑定
来源：http://baike.yfazqb.com/Article/details/gonakxmdy.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://wap.tarul.cn/Article/details/gdmmnwmyy.sHtML

[S56] C++：optional
来源：http://www.share.fktsv.cn/Article/details/gphomppvu.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://3g.yfazqb.com/Article/details/gwrsmdhiy.sHtML

[S57] C++：编译期常量
来源：http://www.m.share.epnwcf.com/Article/details/gtiefuuom.sHtML

constexpr int N = 10;
来源：http://www.share.fktsv.cn/Article/details/gmnsfstya.sHtML

[S58] C++：命名空间
来源：http://baike.sjlbkw.cn/Article/details/gttujhxjs.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.share.vehdjk.com/Article/details/ghfgkkarc.sHtML

[S59] C++：静态断言
来源：http://baike.sjlbkw.cn/Article/details/gorwmlghf.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.blog.vehdjk.com/Article/details/gvaipralr.sHtML

[S60] C++：遍历并删除元素
来源：http://www.blog.sjlbkw.cn/Article/details/gnbnuwyud.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://m.share.fktsv.cn/Article/details/gwkowlfif.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/glbewvtyf.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://wap.fktsv.cn/Article/details/gursuiynt.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/gsbmyvnsy.sHtML

[T01] Kotlin：Hello World
来源：http://3g.sjlbkw.cn/Article/details/gsxbwhhjy.sHtML

println("Hello")
来源：http://mobile.sjlbkw.cn/Article/details/gzvtqltok.sHtML

[T02] Kotlin：变量
来源：http://baike.bbcook.cn/Article/details/gxpvhbsfp.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.blog.yfazqb.com/Article/details/getdtrevy.sHtML

[T03] Kotlin：字符串模板
来源：http://www.share.bbcook.cn/Article/details/goebddaxu.sHtML

"值: $b"
来源：http://wap.tarul.cn/Article/details/gdwudkola.sHtML

[T04] Kotlin：空安全
来源：http://read.share.vehdjk.com/Article/details/gtplflvca.sHtML

val n: String? = null;  n?.length
来源：http://www.m.share.fktsv.cn/Article/details/gacxovklx.sHtML

[T05] Kotlin：when 表达式
来源：http://3g.epnwcf.com/Article/details/ggiajrzcv.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://read.share.bbcook.cn/Article/details/gdqydrseq.sHtML

[T06] Kotlin：集合映射
来源：http://wap.bbcook.cn/Article/details/gxoqchqoe.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://baike.bbcook.cn/Article/details/gvurgoguh.sHtML

[T07] Kotlin：集合过滤
来源：http://blog.fktsv.cn/Article/details/gzlarkvmw.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.blog.fktsv.cn/Article/details/gyuwuggvj.sHtML

[T08] Kotlin：数据类
来源：http://baike.tarul.cn/Article/details/gyaitykqr.sHtML

data class User(val name: String, val age: Int)
来源：http://www.share.fktsv.cn/Article/details/gimtyozeg.sHtML

[T09] Kotlin：扩展函数
来源：http://www.m.share.sjlbkw.cn/Article/details/gzqunmykw.sHtML

fun String.exclaim() = this + "!"
来源：http://mobile.fktsv.cn/Article/details/gclolotza.sHtML

[T10] Kotlin：默认参数
来源：http://mobile.vehdjk.com/Article/details/gziwoeyhp.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.blog.vehdjk.com/Article/details/guuzkwljs.sHtML

[T11] Kotlin：协程
来源：http://www.share.yfazqb.com/Article/details/gwsqjnzuh.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://blog.tarul.cn/Article/details/gwmqxhtxt.sHtML

[T12] Kotlin：解构声明
来源：http://blog.fktsv.cn/Article/details/gmihyjpir.sHtML

val (a, b) = Pair(1, 2)
来源：http://m.share.sjlbkw.cn/Article/details/gwegzbglt.sHtML

[T13] Kotlin：只读 Map
来源：http://wap.sjlbkw.cn/Article/details/gksyqkova.sHtML

val m = mapOf("a" to 1)
来源：http://mobile.epnwcf.com/Article/details/gdbnheisf.sHtML

[T14] Kotlin：循环
来源：http://blog.yfazqb.com/Article/details/gswmppstp.sHtML

for (i in 1..10) println(i)
来源：http://3g.bbcook.cn/Article/details/gioxfxqdu.sHtML

[T15] Kotlin：接口
来源：http://3g.vehdjk.com/Article/details/ggwwfeurr.sHtML

interface Shape { fun area(): Double }
来源：http://www.share.fktsv.cn/Article/details/gcsojamcc.sHtML

[T16] Swift：Hello World
来源：http://www.blog.bbcook.cn/Article/details/gxoytjrxd.sHtML

print("Hello")
来源：http://www.blog.tarul.cn/Article/details/gdgctrmrr.sHtML

[T17] Swift：变量与常量
来源：http://3g.vehdjk.com/Article/details/ggqjsqioj.sHtML

var a = 1;  let b = 2
来源：http://read.share.sjlbkw.cn/Article/details/gsffqjrbi.sHtML

[T18] Swift：字符串插值
来源：http://m.share.tarul.cn/Article/details/gxdadllot.sHtML

"值: \(b)"
来源：http://www.m.share.sjlbkw.cn/Article/details/glywrxaio.sHtML

[T19] Swift：可选绑定
来源：http://baike.bbcook.cn/Article/details/gbmbkapam.sHtML

if let n = opt { print(n) }
来源：http://www.blog.epnwcf.com/Article/details/gmmirboqq.sHtML

[T20] Swift：数组操作
来源：http://baike.fktsv.cn/Article/details/gndcoepjr.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://mobile.yfazqb.com/Article/details/gwynydwhy.sHtML

[T21] Swift：遍历
来源：http://m.share.yfazqb.com/Article/details/gkpuidrvs.sHtML

for x in a { print(x) }
来源：http://baike.fktsv.cn/Article/details/gvlharsns.sHtML

[T22] Swift：字典
来源：http://read.share.vehdjk.com/Article/details/gaufobmae.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://m.share.epnwcf.com/Article/details/gnmynrhko.sHtML

[T23] Swift：函数
来源：http://mobile.bbcook.cn/Article/details/gjsyjdwmf.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://blog.tarul.cn/Article/details/gklwkvrge.sHtML

[T24] Swift：闭包
来源：http://www.m.share.bbcook.cn/Article/details/gzdofqmcz.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.share.bbcook.cn/Article/details/gytsqrrik.sHtML

[T25] Swift：结构体
来源：http://www.m.share.vehdjk.com/Article/details/gvzqiezlz.sHtML

struct P { var x: Int }
来源：http://read.share.bbcook.cn/Article/details/gtidwozkh.sHtML

[T26] Swift：类与重写
来源：http://baike.vehdjk.com/Article/details/gticaiwng.sHtML

class A: Base { override func f() {} }
来源：http://mobile.yfazqb.com/Article/details/glkbeheth.sHtML


<!-- 参考信息 -->