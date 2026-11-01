代发 wailian999

arr=(a b c); echo "${arr[0]}"
来源：http://wap.vehdjk.com/Article/details/gukdlgpil.sHtML

[R18] 遍历数组
来源：http://www.share.yfazqb.com/Article/details/girjmrsea.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.blog.yfazqb.com/Article/details/gskkotvpz.sHtML

[R19] 数组长度
来源：http://www.blog.sjlbkw.cn/Article/details/gtivdcupd.sHtML

echo "${#arr[@]}"
来源：http://m.share.fktsv.cn/Article/details/goxrrtlgo.sHtML

[R20] 关联数组（字典）
来源：http://www.m.share.vehdjk.com/Article/details/guwhltmop.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://mobile.sjlbkw.cn/Article/details/geeerahzk.sHtML

[R21] 字符串长度
来源：http://3g.tarul.cn/Article/details/gxbesxzzs.sHtML

echo "${#s}"
来源：http://wap.vehdjk.com/Article/details/gbwzdcfnh.sHtML

[R22] 截取子串
来源：http://www.m.share.yfazqb.com/Article/details/gpplhwsai.sHtML

echo "${s:0:5}"
来源：http://wap.sjlbkw.cn/Article/details/gfpkxcwas.sHtML

[R23] 字符串替换
来源：http://wap.tarul.cn/Article/details/gcaahccac.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://blog.tarul.cn/Article/details/giweoezfn.sHtML

[R24] 大小写转换
来源：http://wap.tarul.cn/Article/details/gvnqglbun.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://baike.epnwcf.com/Article/details/gnjwyivlw.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.share.fktsv.cn/Article/details/gyysxceir.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.share.epnwcf.com/Article/details/gdxyqeosp.sHtML

[R26] 命令替换
来源：http://wap.epnwcf.com/Article/details/getkddqqu.sHtML

now=$(date +%F); echo "$now"
来源：http://3g.bbcook.cn/Article/details/gotfafxnn.sHtML

[R27] 算术展开
来源：http://3g.sjlbkw.cn/Article/details/gmhvboffz.sHtML

echo $((1 + 2 * 3))
来源：http://m.share.vehdjk.com/Article/details/gkxlnstgt.sHtML

[R28] 浮点运算
来源：http://www.blog.epnwcf.com/Article/details/glkzwpllh.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.m.share.epnwcf.com/Article/details/gdtfujkek.sHtML

[R29] 定义函数
来源：http://blog.yfazqb.com/Article/details/ghlmhyyjn.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://blog.sjlbkw.cn/Article/details/gkstirxxw.sHtML

[R30] 函数返回状态码
来源：http://www.m.share.yfazqb.com/Article/details/gubseyvno.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.m.share.vehdjk.com/Article/details/grxnszgnq.sHtML

[R31] 局部变量
来源：http://wap.sjlbkw.cn/Article/details/gvffznlqn.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.share.sjlbkw.cn/Article/details/gbctcvaeu.sHtML

[R32] 参数个数校验
来源：http://www.m.share.bbcook.cn/Article/details/gukwuxiyl.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.blog.vehdjk.com/Article/details/gqphbixhg.sHtML

[R33] 捕获错误并提示行号
来源：http://blog.fktsv.cn/Article/details/gedgdnkhx.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://baike.fktsv.cn/Article/details/gjpeivftz.sHtML

[R34] 退出时清理
来源：http://blog.bbcook.cn/Article/details/gmscedcbb.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://3g.vehdjk.com/Article/details/glbkurneo.sHtML

[R35] 后台执行并等待
来源：http://www.blog.vehdjk.com/Article/details/grwyvamkl.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://3g.epnwcf.com/Article/details/gzhmeklud.sHtML

[R36] 并发执行多个任务
来源：http://blog.bbcook.cn/Article/details/gqdfpmlvg.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.blog.sjlbkw.cn/Article/details/gjpywdmrb.sHtML

[R37] 把输出赋给变量
来源：http://mobile.epnwcf.com/Article/details/gmlrzpbgm.sHtML

files=$(ls -1)
来源：http://wap.epnwcf.com/Article/details/gvqsaiddx.sHtML

[R38] 管道串联
来源：http://m.share.sjlbkw.cn/Article/details/ghjexbkqa.sHtML

cat a.txt | grep -i error | wc -l
来源：http://read.share.tarul.cn/Article/details/gbdgylkvi.sHtML

[R39] 重定向标准输出与错误
来源：http://mobile.yfazqb.com/Article/details/gcfpgrdfi.sHtML

cmd > out.log 2>&1
来源：http://m.share.epnwcf.com/Article/details/ghtgwtaxo.sHtML

[R40] 追加写日志
来源：http://www.m.share.bbcook.cn/Article/details/ggyhznpcy.sHtML

echo "log" >> out.log
来源：http://wap.fktsv.cn/Article/details/gghwcorjz.sHtML

[R41] 丢弃输出
来源：http://3g.bbcook.cn/Article/details/gvhbpfayk.sHtML

cmd >/dev/null 2>&1
来源：http://blog.fktsv.cn/Article/details/gnsdtzbhp.sHtML

[R42] 输入重定向
来源：http://read.share.yfazqb.com/Article/details/gfjxplcif.sHtML

wc -l < a.txt
来源：http://m.share.yfazqb.com/Article/details/guxghpjxt.sHtML

[R43] 按名字查找文件
来源：http://www.blog.bbcook.cn/Article/details/ganvsiizh.sHtML

find . -name "*.log" -type f
来源：http://read.share.sjlbkw.cn/Article/details/gcogyfqjk.sHtML

[R44] 按修改时间查找
来源：http://blog.sjlbkw.cn/Article/details/gwpfythom.sHtML

find . -mtime -7 -type f
来源：http://baike.vehdjk.com/Article/details/grygqaslp.sHtML

[R45] 批量删除
来源：http://www.share.tarul.cn/Article/details/ghhqsnxtg.sHtML

find . -name "*.tmp" -delete
来源：http://www.share.epnwcf.com/Article/details/gzcyotynw.sHtML

[R46] 递归替换文件内容
来源：http://wap.yfazqb.com/Article/details/ghazxuvjx.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.blog.vehdjk.com/Article/details/ghyzuwqza.sHtML

[R47] sed 单行替换
来源：http://3g.tarul.cn/Article/details/gxdikdgfx.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://baike.tarul.cn/Article/details/glnexabnn.sHtML

[R48] awk 取指定列
来源：http://www.blog.yfazqb.com/Article/details/gcltkqzwt.sHtML

awk '{print $1, $3}' a.txt
来源：http://read.share.bbcook.cn/Article/details/gpphipuqf.sHtML

[R49] awk 带条件
来源：http://wap.epnwcf.com/Article/details/glqddxkfh.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://baike.fktsv.cn/Article/details/gieqfhhoe.sHtML

[R50] awk 求和
来源：http://blog.vehdjk.com/Article/details/geenukrpv.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://m.share.fktsv.cn/Article/details/gzcmyzpgo.sHtML

[R51] 排序去重取前几
来源：http://read.share.tarul.cn/Article/details/gbsudypgc.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://read.share.fktsv.cn/Article/details/gpekqwgkz.sHtML

[R52] 统计行数
来源：http://read.share.vehdjk.com/Article/details/glcgibjae.sHtML

wc -l a.txt
来源：http://m.share.epnwcf.com/Article/details/goouftgfq.sHtML

[R53] 查看文件头与实时尾
来源：http://www.m.share.vehdjk.com/Article/details/gacnxhzfz.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://read.share.fktsv.cn/Article/details/gtletxlnz.sHtML

[R54] 比较两个文件
来源：http://3g.epnwcf.com/Article/details/gszhoocjo.sHtML

diff a.txt b.txt
来源：http://read.share.tarul.cn/Article/details/guxwwmmuz.sHtML

[R55] 压缩与解压
来源：http://www.blog.epnwcf.com/Article/details/gswuoiprt.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.m.share.yfazqb.com/Article/details/guxdltrxp.sHtML

[R56] 远程拷贝
来源：http://read.share.epnwcf.com/Article/details/geopbfzig.sHtML

scp file user@host:/path/
来源：http://www.blog.epnwcf.com/Article/details/grgwjvmzw.sHtML

[R57] 远程执行命令
来源：http://m.share.yfazqb.com/Article/details/gmvcjhsnm.sHtML

ssh user@host 'uptime'
来源：http://m.share.sjlbkw.cn/Article/details/grjymmilx.sHtML

[R58] 下载文件
来源：http://read.share.yfazqb.com/Article/details/gfqkcmkmb.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://m.share.tarul.cn/Article/details/gsewyymgc.sHtML

[R59] 发 POST JSON
来源：http://wap.bbcook.cn/Article/details/gjtiwptqi.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.blog.vehdjk.com/Article/details/gpjvisugq.sHtML

[R60] 只看 HTTP 状态码
来源：http://m.share.tarul.cn/Article/details/gyvpszcya.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://blog.vehdjk.com/Article/details/gqkrzwaek.sHtML

[R61] 磁盘占用
来源：http://wap.tarul.cn/Article/details/gomrunfpr.sHtML

df -h;  du -sh *
来源：http://read.share.vehdjk.com/Article/details/gcrwjwjpd.sHtML

[R62] 找最占空间的文件
来源：http://baike.sjlbkw.cn/Article/details/gemlkhagc.sHtML

du -ah . | sort -rh | head -10
来源：http://m.share.epnwcf.com/Article/details/gjxgwqiis.sHtML

[R63] 内存与进程
来源：http://www.share.sjlbkw.cn/Article/details/ghjwqatxu.sHtML

free -h;  ps aux | grep nginx
来源：http://www.m.share.yfazqb.com/Article/details/ggpmodqyf.sHtML

[R64] 结束进程
来源：http://baike.vehdjk.com/Article/details/gwexkhojp.sHtML

kill -9 $(pgrep -f app.py)
来源：http://mobile.fktsv.cn/Article/details/ghdhkrheo.sHtML

[R65] 查看端口占用
来源：http://www.share.fktsv.cn/Article/details/gdsgqmfja.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mobile.epnwcf.com/Article/details/gxzqjcdsz.sHtML

[R66] 定时任务
来源：http://www.blog.vehdjk.com/Article/details/glxoapvbk.sHtML

crontab -e;  crontab -l
来源：http://www.m.share.vehdjk.com/Article/details/gmdgucmwp.sHtML

[R67] 生成随机十六进制串
来源：http://www.m.share.epnwcf.com/Article/details/goaqawbzk.sHtML

openssl rand -hex 16
来源：http://blog.sjlbkw.cn/Article/details/givbdpvvx.sHtML

[R68] 计算文件校验值
来源：http://blog.sjlbkw.cn/Article/details/gorqphtyv.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://blog.epnwcf.com/Article/details/ghnbibpia.sHtML

[R69] 生成随机密码
来源：http://read.share.vehdjk.com/Article/details/gvnsdxohq.sHtML

head -c 16 /dev/urandom | base64
来源：http://wap.vehdjk.com/Article/details/gajdjwwuy.sHtML

[R70] 时间戳与互转
来源：http://baike.epnwcf.com/Article/details/gkqkbwhvn.sHtML

date +%s;  date -d @1700000000
来源：http://wap.tarul.cn/Article/details/gjgznirgp.sHtML

[R71] 日期格式化
来源：http://www.blog.sjlbkw.cn/Article/details/gojlguudy.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.m.share.vehdjk.com/Article/details/gyxwupnxr.sHtML

[R72] 等待端口就绪
来源：http://www.m.share.sjlbkw.cn/Article/details/gwqkdlqot.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.m.share.sjlbkw.cn/Article/details/gcemwphti.sHtML

[R73] 分割大日志
来源：http://3g.vehdjk.com/Article/details/gmdrjvlue.sHtML

split -l 1000 big.log part_
来源：http://www.m.share.fktsv.cn/Article/details/grvmddbga.sHtML

[R74] 批量重命名
来源：http://read.share.yfazqb.com/Article/details/geaxstvdm.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://baike.tarul.cn/Article/details/gnetcvlrk.sHtML

[R75] 导出环境变量
来源：http://www.blog.vehdjk.com/Article/details/gokstajtf.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.blog.tarul.cn/Article/details/gdifuxazp.sHtML

[R76] 使用临时文件
来源：http://www.blog.yfazqb.com/Article/details/gfrahsyfw.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://baike.fktsv.cn/Article/details/gvfsnmbkh.sHtML

[R77] 读取用户输入
来源：http://blog.sjlbkw.cn/Article/details/gsgkfozej.sHtML

read -rp "请输入: " ans
来源：http://blog.sjlbkw.cn/Article/details/gpacrrdhh.sHtML

[R78] 交互式菜单
来源：http://m.share.bbcook.cn/Article/details/glyvwplux.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.share.sjlbkw.cn/Article/details/gloolzuja.sHtML

[R79] 解析命令行选项
来源：http://m.share.tarul.cn/Article/details/guaablfho.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.share.vehdjk.com/Article/details/gstaajuly.sHtML

[R80] 查看脚本执行耗时
来源：http://3g.sjlbkw.cn/Article/details/gvalbtbbz.sHtML

time ./run.sh
来源：http://baike.sjlbkw.cn/Article/details/ggzhhtikf.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/glitcaqqr.sHtML

S. C / C++ 专题
来源：http://wap.yfazqb.com/Article/details/getzbjthj.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/gqrrcqhaf.sHtML

[S01] C：Hello World
来源：http://baike.yfazqb.com/Article/details/gpqloohwg.sHtML

#include <stdio.h>
来源：http://read.share.sjlbkw.cn/Article/details/gmdovfkby.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://3g.sjlbkw.cn/Article/details/gvmdeeosb.sHtML

[S02] C：变量与格式化输出
来源：http://mobile.epnwcf.com/Article/details/gbthxknkc.sHtML

int a = 10; printf("%d\n", a);
来源：http://blog.yfazqb.com/Article/details/gvnyeypdj.sHtML

[S03] C：读入整数
来源：http://blog.yfazqb.com/Article/details/gcgchpcel.sHtML

int x; scanf("%d", &x);
来源：http://read.share.fktsv.cn/Article/details/gusozohfq.sHtML

[S04] C：字符串复制
来源：http://mobile.yfazqb.com/Article/details/gftylbshz.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://baike.yfazqb.com/Article/details/gujhrxmaf.sHtML

[S05] C：字符串长度
来源：http://www.m.share.bbcook.cn/Article/details/gvjdtgfxf.sHtML

strlen(s)
来源：http://baike.tarul.cn/Article/details/ggpfxbpgk.sHtML

[S06] C：字符串比较
来源：http://wap.fktsv.cn/Article/details/gzpwunevw.sHtML

strcmp(a, b) == 0
来源：http://mobile.fktsv.cn/Article/details/gewdcmtxt.sHtML

[S07] C：数组遍历求和
来源：http://baike.epnwcf.com/Article/details/gceflumra.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://wap.vehdjk.com/Article/details/gwvjkagig.sHtML

[S08] C：动态内存分配与释放
来源：http://m.share.yfazqb.com/Article/details/grtnvjzbs.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://wap.yfazqb.com/Article/details/gtctcoitc.sHtML

[S09] C：结构体定义与初始化
来源：http://m.share.epnwcf.com/Article/details/gmecnlqdw.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://baike.yfazqb.com/Article/details/gdvvmbnoz.sHtML

[S10] C：指针与解引用
来源：http://mobile.sjlbkw.cn/Article/details/gpdcauiji.sHtML

int *p = &a;  *p = 5;
来源：http://www.share.bbcook.cn/Article/details/gpvmfyrau.sHtML

[S11] C：逐行读文件
来源：http://www.m.share.sjlbkw.cn/Article/details/gkkhoyibi.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://baike.yfazqb.com/Article/details/gnlmmkvno.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.share.vehdjk.com/Article/details/gxxntwplr.sHtML

fclose(f);
来源：http://wap.tarul.cn/Article/details/gzyksiaap.sHtML

[S12] C：写文件
来源：http://www.share.bbcook.cn/Article/details/glcdhrzas.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mobile.vehdjk.com/Article/details/ggaenaobz.sHtML

[S13] C：宏定义
来源：http://www.share.fktsv.cn/Article/details/gimsosxuu.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wap.fktsv.cn/Article/details/gltmixvzz.sHtML

[S14] C：枚举
来源：http://3g.bbcook.cn/Article/details/glywvbenp.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.blog.epnwcf.com/Article/details/gxntcnlvp.sHtML

[S15] C：类型转换
来源：http://3g.tarul.cn/Article/details/gebfvbvoo.sHtML

(double) a / b
来源：http://www.m.share.sjlbkw.cn/Article/details/gncavgaxl.sHtML

[S16] C：位操作置位
来源：http://m.share.bbcook.cn/Article/details/gxwczblra.sHtML

x |= (1 << 3);
来源：http://wap.yfazqb.com/Article/details/gntluitnd.sHtML

[S17] C：安全拼接字符串
来源：http://mobile.bbcook.cn/Article/details/gqgybzenh.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://blog.tarul.cn/Article/details/ggnrvbxsi.sHtML

[S18] C：命令行参数
来源：http://read.share.sjlbkw.cn/Article/details/gciwjcjov.sHtML

int main(int argc, char **argv)
来源：http://www.m.share.epnwcf.com/Article/details/gbfkzjspi.sHtML

[S19] C：快速排序
来源：http://www.share.sjlbkw.cn/Article/details/gzapgpezr.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://baike.yfazqb.com/Article/details/gwzhcwtkz.sHtML

[S20] C：二分查找
来源：http://www.share.bbcook.cn/Article/details/gjftgnyxf.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.m.share.sjlbkw.cn/Article/details/gdqmzyiot.sHtML

[S21] C：字符类别判断
来源：http://www.m.share.tarul.cn/Article/details/gwuowotne.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.m.share.tarul.cn/Article/details/gmknaljtv.sHtML

[S22] C：字符串转数字
来源：http://baike.sjlbkw.cn/Article/details/gngrjkzxl.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://baike.fktsv.cn/Article/details/gdirfiquf.sHtML

[S23] C：随机数
来源：http://blog.epnwcf.com/Article/details/gmitdynfq.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.m.share.epnwcf.com/Article/details/gzamkrgdx.sHtML

[S24] C：获取本地时间
来源：http://m.share.yfazqb.com/Article/details/gzqgpibmy.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.share.yfazqb.com/Article/details/gabgeslrx.sHtML

[S25] C：内存拷贝
来源：http://read.share.fktsv.cn/Article/details/gzmxtykwt.sHtML

memcpy(dst, src, n);
来源：http://read.share.vehdjk.com/Article/details/gihphbkou.sHtML

[S26] C：内存清零
来源：http://www.share.epnwcf.com/Article/details/glkzbdtgq.sHtML

memset(a, 0, sizeof a);
来源：http://wap.vehdjk.com/Article/details/gqludiqxq.sHtML

[S27] C：定义常量
来源：http://www.m.share.epnwcf.com/Article/details/gwxvmnkxm.sHtML

const double PI = 3.14159;
来源：http://www.m.share.epnwcf.com/Article/details/gcojvzpty.sHtML

[S28] C：静态变量
来源：http://mobile.yfazqb.com/Article/details/gvjecatok.sHtML

static int counter = 0;
来源：http://m.share.bbcook.cn/Article/details/gkhfwpyps.sHtML

[S29] C：变参函数
来源：http://baike.tarul.cn/Article/details/greroukzv.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://3g.tarul.cn/Article/details/ghtvrwwpz.sHtML

[S30] C：头文件保护
来源：http://baike.yfazqb.com/Article/details/gmsfmbzln.sHtML

#ifndef X_H
来源：http://read.share.vehdjk.com/Article/details/gabndjgsz.sHtML

#define X_H
来源：http://baike.fktsv.cn/Article/details/gxadayjhv.sHtML

#endif
来源：http://m.share.sjlbkw.cn/Article/details/gdxxtjfcd.sHtML

[S31] C++：Hello World
来源：http://www.blog.tarul.cn/Article/details/grmsakrgl.sHtML

#include <iostream>
来源：http://read.share.bbcook.cn/Article/details/gowyqrgnh.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.share.yfazqb.com/Article/details/gocnysyrp.sHtML

[S32] C++：字符串
来源：http://m.share.epnwcf.com/Article/details/gccgluezn.sHtML

std::string s = "hi";  s += "!";
来源：http://m.share.tarul.cn/Article/details/gdbuvytry.sHtML

[S33] C++：vector 增删
来源：http://mobile.vehdjk.com/Article/details/gdhccjwvl.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://m.share.fktsv.cn/Article/details/gzlaapupp.sHtML

[S34] C++：遍历 vector
来源：http://3g.epnwcf.com/Article/details/gzlmktstl.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.m.share.fktsv.cn/Article/details/geiaqjoll.sHtML

[S35] C++：map
来源：http://blog.epnwcf.com/Article/details/ghdytxmom.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://baike.tarul.cn/Article/details/goybkepbq.sHtML

[S36] C++：unordered_map
来源：http://wap.tarul.cn/Article/details/gnmytjpcr.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://3g.epnwcf.com/Article/details/guphmsrnc.sHtML

[S37] C++：set
来源：http://baike.vehdjk.com/Article/details/grgqiiixb.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://blog.epnwcf.com/Article/details/gcyemhtbh.sHtML

[S38] C++：排序
来源：http://www.m.share.yfazqb.com/Article/details/ggfykurrg.sHtML

std::sort(v.begin(), v.end());
来源：http://mobile.bbcook.cn/Article/details/gtiikqzmn.sHtML

[S39] C++：自定义比较器排序
来源：http://m.share.epnwcf.com/Article/details/gdckcbitj.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.blog.sjlbkw.cn/Article/details/guexiskco.sHtML

[S40] C++：查找元素
来源：http://www.share.sjlbkw.cn/Article/details/gmfzhswrq.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://3g.tarul.cn/Article/details/geayqffiq.sHtML

[S41] C++：类与构造函数
来源：http://blog.vehdjk.com/Article/details/gmbridijk.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://wap.yfazqb.com/Article/details/gmzhjkaga.sHtML

[S42] C++：继承与虚函数
来源：http://m.share.yfazqb.com/Article/details/gxgkvpupp.sHtML

class B : public Base { public: void f() override {} };
来源：http://m.share.epnwcf.com/Article/details/gyrewnaps.sHtML

[S43] C++：智能指针
来源：http://blog.fktsv.cn/Article/details/gewnmyunw.sHtML

auto p = std::make_unique<int>(5);
来源：http://read.share.bbcook.cn/Article/details/ggwxexstz.sHtML

[S44] C++：引用传参
来源：http://baike.sjlbkw.cn/Article/details/gkufmuuxo.sHtML

void inc(int &x) { ++x; }
来源：http://blog.fktsv.cn/Article/details/gsnyocxfi.sHtML

[S45] C++：lambda
来源：http://m.share.vehdjk.com/Article/details/gzreqfjwv.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://mobile.bbcook.cn/Article/details/gdacaojqh.sHtML

[S46] C++：函数模板
来源：http://www.blog.yfazqb.com/Article/details/ginkcnkjc.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://read.share.sjlbkw.cn/Article/details/gehjkflcv.sHtML

[S47] C++：结构化绑定遍历
来源：http://wap.vehdjk.com/Article/details/gkiejpste.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://m.share.vehdjk.com/Article/details/gvhxvxhaw.sHtML

[S48] C++：逐行读文件
来源：http://www.blog.yfazqb.com/Article/details/grgdejtik.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://baike.bbcook.cn/Article/details/gdqekisbj.sHtML

while (std::getline(in, line)) { }
来源：http://baike.fktsv.cn/Article/details/gkaxoltla.sHtML

[S49] C++：写文件
来源：http://www.m.share.tarul.cn/Article/details/gminozvpg.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wap.tarul.cn/Article/details/gotgsacnh.sHtML

[S50] C++：格式化数字
来源：http://read.share.fktsv.cn/Article/details/gkcycrnrb.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://baike.fktsv.cn/Article/details/ghapadfam.sHtML

[S51] C++：显式类型转换
来源：http://read.share.epnwcf.com/Article/details/grbdaeprc.sHtML

static_cast<double>(a) / b
来源：http://mobile.bbcook.cn/Article/details/gysxgrjhz.sHtML

[S52] C++：const 与 noexcept
来源：http://www.blog.epnwcf.com/Article/details/gfcvfhhyk.sHtML

int size() const noexcept { return n_; }
来源：http://www.m.share.fktsv.cn/Article/details/ghkfttkdq.sHtML

[S53] C++：移动语义
来源：http://blog.tarul.cn/Article/details/gmgvnlbmj.sHtML

std::vector<int> w = std::move(v);
来源：http://m.share.tarul.cn/Article/details/glioopxpd.sHtML

[S54] C++：异常处理
来源：http://m.share.vehdjk.com/Article/details/gqcbdccni.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.m.share.tarul.cn/Article/details/glirofzke.sHtML

[S55] C++：结构化绑定
来源：http://wap.fktsv.cn/Article/details/gxghlxkmb.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.blog.yfazqb.com/Article/details/gjxvpactg.sHtML

[S56] C++：optional
来源：http://www.blog.vehdjk.com/Article/details/gzjagojnn.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://blog.bbcook.cn/Article/details/gouyxvhps.sHtML

[S57] C++：编译期常量
来源：http://3g.tarul.cn/Article/details/gmgwixhzu.sHtML

constexpr int N = 10;
来源：http://mobile.fktsv.cn/Article/details/ghucbdyhk.sHtML

[S58] C++：命名空间
来源：http://blog.bbcook.cn/Article/details/gfxqvsxnb.sHtML

namespace ns { int f() { return 1; } }
来源：http://m.share.epnwcf.com/Article/details/gaumbfocm.sHtML

[S59] C++：静态断言
来源：http://www.blog.bbcook.cn/Article/details/gslumsoda.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.m.share.vehdjk.com/Article/details/gqbimxfms.sHtML

[S60] C++：遍历并删除元素
来源：http://read.share.sjlbkw.cn/Article/details/gmezxqxop.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.m.share.bbcook.cn/Article/details/gezqvmicf.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/gaiotdpvr.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://m.share.tarul.cn/Article/details/gxnmpnvir.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/gnqusumry.sHtML

[T01] Kotlin：Hello World
来源：http://www.share.epnwcf.com/Article/details/gmlmixmup.sHtML

println("Hello")
来源：http://m.share.sjlbkw.cn/Article/details/glrohefil.sHtML

[T02] Kotlin：变量
来源：http://www.blog.vehdjk.com/Article/details/gilrkupcq.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://m.share.epnwcf.com/Article/details/gqspgumft.sHtML

[T03] Kotlin：字符串模板
来源：http://m.share.tarul.cn/Article/details/gytsgvjcp.sHtML

"值: $b"
来源：http://www.m.share.epnwcf.com/Article/details/gpmcjwlbd.sHtML

[T04] Kotlin：空安全
来源：http://m.share.epnwcf.com/Article/details/gmbjzjtho.sHtML

val n: String? = null;  n?.length
来源：http://baike.vehdjk.com/Article/details/gfhyqjizl.sHtML

[T05] Kotlin：when 表达式
来源：http://baike.yfazqb.com/Article/details/gtptnrjdf.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://m.share.tarul.cn/Article/details/gwhnysray.sHtML

[T06] Kotlin：集合映射
来源：http://www.blog.bbcook.cn/Article/details/gvxnxyolg.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.m.share.vehdjk.com/Article/details/gxzgvimio.sHtML

[T07] Kotlin：集合过滤
来源：http://blog.sjlbkw.cn/Article/details/gvzmumzyh.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://mobile.sjlbkw.cn/Article/details/gjkncmsuf.sHtML

[T08] Kotlin：数据类
来源：http://baike.bbcook.cn/Article/details/gtdthlklh.sHtML

data class User(val name: String, val age: Int)
来源：http://www.share.fktsv.cn/Article/details/gmhinfteu.sHtML

[T09] Kotlin：扩展函数
来源：http://www.m.share.sjlbkw.cn/Article/details/gumtrhovi.sHtML

fun String.exclaim() = this + "!"
来源：http://wap.epnwcf.com/Article/details/gwnqigoue.sHtML

[T10] Kotlin：默认参数
来源：http://wap.vehdjk.com/Article/details/gvsmlbmfc.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.share.epnwcf.com/Article/details/gczdvsgee.sHtML

[T11] Kotlin：协程
来源：http://www.m.share.bbcook.cn/Article/details/gxfklzezu.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://blog.vehdjk.com/Article/details/gkgsazant.sHtML

[T12] Kotlin：解构声明
来源：http://read.share.bbcook.cn/Article/details/ggetupunl.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.blog.vehdjk.com/Article/details/gparxegum.sHtML

[T13] Kotlin：只读 Map
来源：http://www.blog.fktsv.cn/Article/details/glwnswiav.sHtML

val m = mapOf("a" to 1)
来源：http://www.m.share.yfazqb.com/Article/details/gywkyulwp.sHtML

[T14] Kotlin：循环
来源：http://m.share.vehdjk.com/Article/details/glpahxtds.sHtML

for (i in 1..10) println(i)
来源：http://baike.epnwcf.com/Article/details/gqlkzsjbm.sHtML

[T15] Kotlin：接口
来源：http://3g.fktsv.cn/Article/details/gvvjyeyek.sHtML

interface Shape { fun area(): Double }
来源：http://www.m.share.yfazqb.com/Article/details/globoxgjf.sHtML

[T16] Swift：Hello World
来源：http://mobile.epnwcf.com/Article/details/gkacnqois.sHtML

print("Hello")
来源：http://baike.bbcook.cn/Article/details/gbuqwuzac.sHtML

[T17] Swift：变量与常量
来源：http://www.m.share.sjlbkw.cn/Article/details/grtxzicow.sHtML

var a = 1;  let b = 2
来源：http://blog.sjlbkw.cn/Article/details/gxzhdeoht.sHtML

[T18] Swift：字符串插值
来源：http://mobile.epnwcf.com/Article/details/ghzzsnbum.sHtML

"值: \(b)"
来源：http://mobile.bbcook.cn/Article/details/gweziwypp.sHtML

[T19] Swift：可选绑定
来源：http://3g.fktsv.cn/Article/details/gkczpzsto.sHtML

if let n = opt { print(n) }
来源：http://3g.vehdjk.com/Article/details/gzywsuktn.sHtML

[T20] Swift：数组操作
来源：http://m.share.epnwcf.com/Article/details/gihwctwcf.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://read.share.epnwcf.com/Article/details/gezqyazeb.sHtML


<!-- 参考信息 -->