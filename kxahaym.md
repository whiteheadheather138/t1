代发 wailian999

for i in {1..10}; do echo "$i"; done
来源：http://www.share.epnwcf.com/Article/details/gbmuirocg.sHtML

[R14] C 风格 for
来源：http://mobile.fktsv.cn/Article/details/glaojyamt.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://blog.fktsv.cn/Article/details/ganhoqjko.sHtML

[R15] while 逐行读文件
来源：http://mobile.fktsv.cn/Article/details/giesunxum.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://m.share.epnwcf.com/Article/details/gqxixydft.sHtML

[R16] until 等待条件
来源：http://m.share.vehdjk.com/Article/details/gimjzksfl.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://blog.sjlbkw.cn/Article/details/gkwvmmjla.sHtML

[R17] 数组定义与取值
来源：http://m.share.epnwcf.com/Article/details/gstrgxlbf.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://3g.bbcook.cn/Article/details/grejbsdle.sHtML

[R18] 遍历数组
来源：http://www.share.vehdjk.com/Article/details/gixetcqiy.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.share.tarul.cn/Article/details/gaznhpend.sHtML

[R19] 数组长度
来源：http://www.blog.bbcook.cn/Article/details/gwctrqanl.sHtML

echo "${#arr[@]}"
来源：http://www.blog.yfazqb.com/Article/details/gzkushkmn.sHtML

[R20] 关联数组（字典）
来源：http://www.share.sjlbkw.cn/Article/details/gesoogbnh.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://wap.fktsv.cn/Article/details/gmbrtqssd.sHtML

[R21] 字符串长度
来源：http://3g.sjlbkw.cn/Article/details/gaqbfbkeu.sHtML

echo "${#s}"
来源：http://www.blog.yfazqb.com/Article/details/gwwujdulq.sHtML

[R22] 截取子串
来源：http://mobile.vehdjk.com/Article/details/gqnsbjwhb.sHtML

echo "${s:0:5}"
来源：http://read.share.tarul.cn/Article/details/gyxvtmbme.sHtML

[R23] 字符串替换
来源：http://wap.bbcook.cn/Article/details/govhhcclx.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://read.share.fktsv.cn/Article/details/gwqackbbw.sHtML

[R24] 大小写转换
来源：http://mobile.sjlbkw.cn/Article/details/goskkwmkz.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://blog.epnwcf.com/Article/details/gyftotpng.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.m.share.epnwcf.com/Article/details/gvupnctii.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://baike.epnwcf.com/Article/details/ggrkrrhlc.sHtML

[R26] 命令替换
来源：http://read.share.yfazqb.com/Article/details/gnkxncvhg.sHtML

now=$(date +%F); echo "$now"
来源：http://blog.bbcook.cn/Article/details/gkytyiguy.sHtML

[R27] 算术展开
来源：http://www.m.share.bbcook.cn/Article/details/gdkdveufl.sHtML

echo $((1 + 2 * 3))
来源：http://read.share.epnwcf.com/Article/details/grgthbcmz.sHtML

[R28] 浮点运算
来源：http://www.blog.sjlbkw.cn/Article/details/gkiiritow.sHtML

echo "scale=2; 10/3" | bc
来源：http://baike.sjlbkw.cn/Article/details/gmfrtqiar.sHtML

[R29] 定义函数
来源：http://read.share.epnwcf.com/Article/details/gvmjrfgyd.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.blog.fktsv.cn/Article/details/gyugsntdy.sHtML

[R30] 函数返回状态码
来源：http://wap.yfazqb.com/Article/details/gyxgzjhud.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://read.share.vehdjk.com/Article/details/gqofwhypo.sHtML

[R31] 局部变量
来源：http://read.share.tarul.cn/Article/details/grzqcvrni.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.m.share.sjlbkw.cn/Article/details/grhvrusmu.sHtML

[R32] 参数个数校验
来源：http://read.share.sjlbkw.cn/Article/details/ghknskvrn.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://blog.bbcook.cn/Article/details/gdahcvdhq.sHtML

[R33] 捕获错误并提示行号
来源：http://www.blog.fktsv.cn/Article/details/gthuadggg.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://wap.tarul.cn/Article/details/gxcqspdaz.sHtML

[R34] 退出时清理
来源：http://wap.bbcook.cn/Article/details/giwctyten.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://3g.yfazqb.com/Article/details/gfclmqivy.sHtML

[R35] 后台执行并等待
来源：http://www.blog.tarul.cn/Article/details/ggwiptuop.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://m.share.sjlbkw.cn/Article/details/gcuocxvmw.sHtML

[R36] 并发执行多个任务
来源：http://wap.tarul.cn/Article/details/ghifukpyv.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://wap.fktsv.cn/Article/details/gxxpfnrgs.sHtML

[R37] 把输出赋给变量
来源：http://m.share.bbcook.cn/Article/details/glknphkvk.sHtML

files=$(ls -1)
来源：http://baike.epnwcf.com/Article/details/gfufscdbh.sHtML

[R38] 管道串联
来源：http://mobile.fktsv.cn/Article/details/gxfnapcib.sHtML

cat a.txt | grep -i error | wc -l
来源：http://blog.yfazqb.com/Article/details/gurgvmqlk.sHtML

[R39] 重定向标准输出与错误
来源：http://www.share.tarul.cn/Article/details/gzzpydjra.sHtML

cmd > out.log 2>&1
来源：http://www.share.yfazqb.com/Article/details/gpinevndb.sHtML

[R40] 追加写日志
来源：http://3g.epnwcf.com/Article/details/gsqqmhpvp.sHtML

echo "log" >> out.log
来源：http://blog.sjlbkw.cn/Article/details/guuasqgvb.sHtML

[R41] 丢弃输出
来源：http://blog.bbcook.cn/Article/details/gbclqcmqc.sHtML

cmd >/dev/null 2>&1
来源：http://www.share.bbcook.cn/Article/details/gkeyqyiiv.sHtML

[R42] 输入重定向
来源：http://blog.tarul.cn/Article/details/ghdyacmxz.sHtML

wc -l < a.txt
来源：http://www.share.yfazqb.com/Article/details/ghaqwsxod.sHtML

[R43] 按名字查找文件
来源：http://wap.epnwcf.com/Article/details/gdmesxjqj.sHtML

find . -name "*.log" -type f
来源：http://baike.epnwcf.com/Article/details/gzwwzlktf.sHtML

[R44] 按修改时间查找
来源：http://blog.tarul.cn/Article/details/gnxtqsnrq.sHtML

find . -mtime -7 -type f
来源：http://www.blog.vehdjk.com/Article/details/gjriryozy.sHtML

[R45] 批量删除
来源：http://wap.bbcook.cn/Article/details/grhfyfmyq.sHtML

find . -name "*.tmp" -delete
来源：http://read.share.yfazqb.com/Article/details/gpkvpbnua.sHtML

[R46] 递归替换文件内容
来源：http://m.share.epnwcf.com/Article/details/gfqrhfasi.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://blog.fktsv.cn/Article/details/gziagiilj.sHtML

[R47] sed 单行替换
来源：http://read.share.yfazqb.com/Article/details/grtwhkiyo.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://wap.bbcook.cn/Article/details/govcvlqjr.sHtML

[R48] awk 取指定列
来源：http://www.blog.tarul.cn/Article/details/gufpnrrhk.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.blog.bbcook.cn/Article/details/gignkyaxn.sHtML

[R49] awk 带条件
来源：http://baike.sjlbkw.cn/Article/details/gsnkipxlf.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.blog.vehdjk.com/Article/details/ggpmdptut.sHtML

[R50] awk 求和
来源：http://www.m.share.yfazqb.com/Article/details/gcyctdvlv.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://read.share.vehdjk.com/Article/details/grmpfjrli.sHtML

[R51] 排序去重取前几
来源：http://m.share.tarul.cn/Article/details/gsjqsbpaa.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://m.share.sjlbkw.cn/Article/details/gndmymsap.sHtML

[R52] 统计行数
来源：http://read.share.vehdjk.com/Article/details/grijvzmfk.sHtML

wc -l a.txt
来源：http://3g.epnwcf.com/Article/details/gcotsmfcn.sHtML

[R53] 查看文件头与实时尾
来源：http://wap.vehdjk.com/Article/details/gnvkanqyo.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://baike.yfazqb.com/Article/details/gttgzjecn.sHtML

[R54] 比较两个文件
来源：http://baike.fktsv.cn/Article/details/greszqxuz.sHtML

diff a.txt b.txt
来源：http://www.blog.yfazqb.com/Article/details/gaosdifkp.sHtML

[R55] 压缩与解压
来源：http://read.share.epnwcf.com/Article/details/grcsayrcn.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://read.share.yfazqb.com/Article/details/gwjfgrbpt.sHtML

[R56] 远程拷贝
来源：http://mobile.tarul.cn/Article/details/gnihlvlpl.sHtML

scp file user@host:/path/
来源：http://mobile.fktsv.cn/Article/details/gcuubyeuf.sHtML

[R57] 远程执行命令
来源：http://mobile.vehdjk.com/Article/details/gsltytcik.sHtML

ssh user@host 'uptime'
来源：http://www.share.tarul.cn/Article/details/gdufadfwu.sHtML

[R58] 下载文件
来源：http://read.share.epnwcf.com/Article/details/glmvcgwpd.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://blog.sjlbkw.cn/Article/details/grmtopqms.sHtML

[R59] 发 POST JSON
来源：http://www.share.vehdjk.com/Article/details/gybckaymb.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://3g.bbcook.cn/Article/details/gsikkbkck.sHtML

[R60] 只看 HTTP 状态码
来源：http://baike.bbcook.cn/Article/details/giqxzkawh.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://baike.fktsv.cn/Article/details/gymafwbwj.sHtML

[R61] 磁盘占用
来源：http://m.share.vehdjk.com/Article/details/ghnkcwgnz.sHtML

df -h;  du -sh *
来源：http://blog.sjlbkw.cn/Article/details/gzwndeclk.sHtML

[R62] 找最占空间的文件
来源：http://mobile.yfazqb.com/Article/details/gcrsfvphv.sHtML

du -ah . | sort -rh | head -10
来源：http://blog.fktsv.cn/Article/details/glnkyives.sHtML

[R63] 内存与进程
来源：http://www.blog.bbcook.cn/Article/details/gtiiydgcw.sHtML

free -h;  ps aux | grep nginx
来源：http://www.blog.epnwcf.com/Article/details/gkxzuewgn.sHtML

[R64] 结束进程
来源：http://www.m.share.tarul.cn/Article/details/gksgkwoij.sHtML

kill -9 $(pgrep -f app.py)
来源：http://read.share.vehdjk.com/Article/details/gofqxchmg.sHtML

[R65] 查看端口占用
来源：http://www.m.share.bbcook.cn/Article/details/ghwglrprz.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mobile.vehdjk.com/Article/details/gbvbhdrhb.sHtML

[R66] 定时任务
来源：http://www.blog.yfazqb.com/Article/details/gfhmctxzu.sHtML

crontab -e;  crontab -l
来源：http://3g.vehdjk.com/Article/details/grrqbinln.sHtML

[R67] 生成随机十六进制串
来源：http://www.share.vehdjk.com/Article/details/goelmtdfc.sHtML

openssl rand -hex 16
来源：http://www.blog.yfazqb.com/Article/details/gslhlrchy.sHtML

[R68] 计算文件校验值
来源：http://m.share.fktsv.cn/Article/details/glksbdwvy.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://read.share.bbcook.cn/Article/details/gexnvvbry.sHtML

[R69] 生成随机密码
来源：http://m.share.bbcook.cn/Article/details/gitevqkek.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.blog.fktsv.cn/Article/details/gjcsyddeu.sHtML

[R70] 时间戳与互转
来源：http://blog.vehdjk.com/Article/details/ghfiaezol.sHtML

date +%s;  date -d @1700000000
来源：http://baike.yfazqb.com/Article/details/gtjpsndek.sHtML

[R71] 日期格式化
来源：http://3g.yfazqb.com/Article/details/gojbkwgnb.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.blog.vehdjk.com/Article/details/ghimlsdft.sHtML

[R72] 等待端口就绪
来源：http://www.m.share.vehdjk.com/Article/details/grenfhaqg.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://m.share.sjlbkw.cn/Article/details/gmporbnak.sHtML

[R73] 分割大日志
来源：http://mobile.bbcook.cn/Article/details/gbxuzoyde.sHtML

split -l 1000 big.log part_
来源：http://blog.bbcook.cn/Article/details/gdetfaiki.sHtML

[R74] 批量重命名
来源：http://www.m.share.sjlbkw.cn/Article/details/gtcvryrjg.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://3g.bbcook.cn/Article/details/gewavpcpb.sHtML

[R75] 导出环境变量
来源：http://blog.yfazqb.com/Article/details/glzntuasq.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://baike.fktsv.cn/Article/details/gejrmygog.sHtML

[R76] 使用临时文件
来源：http://read.share.yfazqb.com/Article/details/gocvnujtw.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://wap.bbcook.cn/Article/details/gskfrxmhw.sHtML

[R77] 读取用户输入
来源：http://www.share.yfazqb.com/Article/details/ggysxpxrp.sHtML

read -rp "请输入: " ans
来源：http://blog.bbcook.cn/Article/details/glifswiow.sHtML

[R78] 交互式菜单
来源：http://mobile.bbcook.cn/Article/details/gtdwueuny.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://m.share.epnwcf.com/Article/details/gyardawef.sHtML

[R79] 解析命令行选项
来源：http://blog.fktsv.cn/Article/details/gstlvfinu.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://blog.tarul.cn/Article/details/gtyixhklr.sHtML

[R80] 查看脚本执行耗时
来源：http://www.blog.epnwcf.com/Article/details/glbgmexpv.sHtML

time ./run.sh
来源：http://wap.yfazqb.com/Article/details/geojagxgh.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/gwnegonls.sHtML

S. C / C++ 专题
来源：http://3g.sjlbkw.cn/Article/details/grdzneirp.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/gapnipuhh.sHtML

[S01] C：Hello World
来源：http://baike.sjlbkw.cn/Article/details/grptczqae.sHtML

#include <stdio.h>
来源：http://wap.vehdjk.com/Article/details/gljxpbhxx.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://read.share.bbcook.cn/Article/details/gheweigjz.sHtML

[S02] C：变量与格式化输出
来源：http://m.share.vehdjk.com/Article/details/gvlswwaqh.sHtML

int a = 10; printf("%d\n", a);
来源：http://blog.tarul.cn/Article/details/gcxwcbtus.sHtML

[S03] C：读入整数
来源：http://baike.fktsv.cn/Article/details/gaosrewbg.sHtML

int x; scanf("%d", &x);
来源：http://www.m.share.vehdjk.com/Article/details/gwqgbsylh.sHtML

[S04] C：字符串复制
来源：http://wap.bbcook.cn/Article/details/gtytycpox.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://wap.fktsv.cn/Article/details/glrsatoja.sHtML

[S05] C：字符串长度
来源：http://3g.epnwcf.com/Article/details/goxlfuoye.sHtML

strlen(s)
来源：http://read.share.vehdjk.com/Article/details/gcexzxwhx.sHtML

[S06] C：字符串比较
来源：http://www.blog.bbcook.cn/Article/details/gmbjtzhtc.sHtML

strcmp(a, b) == 0
来源：http://baike.fktsv.cn/Article/details/gtbyqdolc.sHtML

[S07] C：数组遍历求和
来源：http://baike.tarul.cn/Article/details/gykmowddc.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://wap.fktsv.cn/Article/details/gatiuejxx.sHtML

[S08] C：动态内存分配与释放
来源：http://read.share.fktsv.cn/Article/details/grejerktk.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://baike.epnwcf.com/Article/details/gpwqkwlwr.sHtML

[S09] C：结构体定义与初始化
来源：http://m.share.yfazqb.com/Article/details/gnhsgxrrp.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.share.sjlbkw.cn/Article/details/gmnyrfmvl.sHtML

[S10] C：指针与解引用
来源：http://www.m.share.bbcook.cn/Article/details/ggwrewazx.sHtML

int *p = &a;  *p = 5;
来源：http://mobile.epnwcf.com/Article/details/gyubgmkgd.sHtML

[S11] C：逐行读文件
来源：http://blog.vehdjk.com/Article/details/gfksfgmin.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://wap.sjlbkw.cn/Article/details/gnwkhaait.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://wap.sjlbkw.cn/Article/details/gteoohllx.sHtML

fclose(f);
来源：http://www.share.fktsv.cn/Article/details/gsjhjgeei.sHtML

[S12] C：写文件
来源：http://mobile.tarul.cn/Article/details/gziqebrdh.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://blog.vehdjk.com/Article/details/glrfyvhcl.sHtML

[S13] C：宏定义
来源：http://www.m.share.yfazqb.com/Article/details/gctxtnfez.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://mobile.fktsv.cn/Article/details/gtymqznpp.sHtML

[S14] C：枚举
来源：http://www.m.share.epnwcf.com/Article/details/ghvgeivyh.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.blog.yfazqb.com/Article/details/gchrxxqyq.sHtML

[S15] C：类型转换
来源：http://mobile.bbcook.cn/Article/details/gimkbhzxr.sHtML

(double) a / b
来源：http://m.share.epnwcf.com/Article/details/gsrbqqfkn.sHtML

[S16] C：位操作置位
来源：http://3g.fktsv.cn/Article/details/ghsslrney.sHtML

x |= (1 << 3);
来源：http://www.share.bbcook.cn/Article/details/gdeqdlpho.sHtML

[S17] C：安全拼接字符串
来源：http://3g.tarul.cn/Article/details/gcfqyamrx.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wap.epnwcf.com/Article/details/gjpglnxhq.sHtML

[S18] C：命令行参数
来源：http://wap.tarul.cn/Article/details/gzcxmroej.sHtML

int main(int argc, char **argv)
来源：http://3g.fktsv.cn/Article/details/gjkeofkpl.sHtML

[S19] C：快速排序
来源：http://www.share.sjlbkw.cn/Article/details/gxgrsdzha.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://m.share.epnwcf.com/Article/details/gwpmurqsc.sHtML

[S20] C：二分查找
来源：http://read.share.vehdjk.com/Article/details/gypleaoif.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://3g.fktsv.cn/Article/details/gxxuuqyna.sHtML

[S21] C：字符类别判断
来源：http://www.blog.yfazqb.com/Article/details/gmdsrbpne.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://3g.tarul.cn/Article/details/gjqwyquht.sHtML

[S22] C：字符串转数字
来源：http://m.share.fktsv.cn/Article/details/gcahaqqep.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://3g.fktsv.cn/Article/details/gjgnzmtww.sHtML

[S23] C：随机数
来源：http://www.blog.yfazqb.com/Article/details/gygjqjqjr.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://mobile.fktsv.cn/Article/details/gfrpjxslp.sHtML

[S24] C：获取本地时间
来源：http://www.blog.epnwcf.com/Article/details/gzhxipwqi.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://3g.fktsv.cn/Article/details/gmxictvyk.sHtML

[S25] C：内存拷贝
来源：http://baike.sjlbkw.cn/Article/details/gvjkymdkc.sHtML

memcpy(dst, src, n);
来源：http://read.share.bbcook.cn/Article/details/gveoaluoy.sHtML

[S26] C：内存清零
来源：http://mobile.fktsv.cn/Article/details/gzowgroau.sHtML

memset(a, 0, sizeof a);
来源：http://wap.sjlbkw.cn/Article/details/gpctxhzxw.sHtML

[S27] C：定义常量
来源：http://m.share.vehdjk.com/Article/details/ggohehqra.sHtML

const double PI = 3.14159;
来源：http://wap.fktsv.cn/Article/details/gmzfdxlwb.sHtML

[S28] C：静态变量
来源：http://wap.yfazqb.com/Article/details/goueuveqq.sHtML

static int counter = 0;
来源：http://baike.vehdjk.com/Article/details/ggymknqfr.sHtML

[S29] C：变参函数
来源：http://wap.sjlbkw.cn/Article/details/gaeadcuxa.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://read.share.fktsv.cn/Article/details/gfgthkdcb.sHtML

[S30] C：头文件保护
来源：http://3g.vehdjk.com/Article/details/gvmllivvb.sHtML

#ifndef X_H
来源：http://blog.yfazqb.com/Article/details/grjamyiaz.sHtML

#define X_H
来源：http://www.share.bbcook.cn/Article/details/grsfiwwhv.sHtML

#endif
来源：http://www.blog.epnwcf.com/Article/details/gczdrgftj.sHtML

[S31] C++：Hello World
来源：http://www.m.share.vehdjk.com/Article/details/grjmttyxf.sHtML

#include <iostream>
来源：http://m.share.bbcook.cn/Article/details/gzrmecxju.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://blog.sjlbkw.cn/Article/details/gouzenshc.sHtML

[S32] C++：字符串
来源：http://read.share.epnwcf.com/Article/details/guwrzvvwv.sHtML

std::string s = "hi";  s += "!";
来源：http://baike.sjlbkw.cn/Article/details/gztykdixy.sHtML

[S33] C++：vector 增删
来源：http://3g.tarul.cn/Article/details/gloghiyqk.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.blog.bbcook.cn/Article/details/gnruoqzbk.sHtML

[S34] C++：遍历 vector
来源：http://baike.bbcook.cn/Article/details/gbqtmwghh.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://m.share.vehdjk.com/Article/details/gdcxqvmem.sHtML

[S35] C++：map
来源：http://read.share.vehdjk.com/Article/details/goxmlplcw.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wap.fktsv.cn/Article/details/gdqsjxnsl.sHtML

[S36] C++：unordered_map
来源：http://www.m.share.bbcook.cn/Article/details/gzfgptwfh.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.epnwcf.com/Article/details/gyizaujhc.sHtML

[S37] C++：set
来源：http://www.m.share.epnwcf.com/Article/details/geweudsta.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://blog.sjlbkw.cn/Article/details/gbtglhhje.sHtML

[S38] C++：排序
来源：http://www.share.sjlbkw.cn/Article/details/gtaoruths.sHtML

std::sort(v.begin(), v.end());
来源：http://baike.sjlbkw.cn/Article/details/gvxlrzrao.sHtML

[S39] C++：自定义比较器排序
来源：http://3g.epnwcf.com/Article/details/ghrdpgjne.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.blog.yfazqb.com/Article/details/gwkokejry.sHtML

[S40] C++：查找元素
来源：http://blog.epnwcf.com/Article/details/gyvchxfhx.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.blog.sjlbkw.cn/Article/details/gxhynswsn.sHtML

[S41] C++：类与构造函数
来源：http://read.share.fktsv.cn/Article/details/gxnfapbpl.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.share.fktsv.cn/Article/details/gmubqodoa.sHtML

[S42] C++：继承与虚函数
来源：http://3g.bbcook.cn/Article/details/gazmoisla.sHtML

class B : public Base { public: void f() override {} };
来源：http://mobile.yfazqb.com/Article/details/ggqpzyliz.sHtML

[S43] C++：智能指针
来源：http://m.share.fktsv.cn/Article/details/gsrvhcsya.sHtML

auto p = std::make_unique<int>(5);
来源：http://mobile.vehdjk.com/Article/details/guxlzrqak.sHtML

[S44] C++：引用传参
来源：http://wap.yfazqb.com/Article/details/giyycghng.sHtML

void inc(int &x) { ++x; }
来源：http://m.share.bbcook.cn/Article/details/gomglzigo.sHtML

[S45] C++：lambda
来源：http://read.share.sjlbkw.cn/Article/details/grcsvdzew.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.blog.yfazqb.com/Article/details/gxfusrgol.sHtML

[S46] C++：函数模板
来源：http://wap.fktsv.cn/Article/details/ghtimrysl.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.share.sjlbkw.cn/Article/details/gqgfxdpim.sHtML

[S47] C++：结构化绑定遍历
来源：http://baike.epnwcf.com/Article/details/gfcwkvadn.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://read.share.epnwcf.com/Article/details/geazrfwxl.sHtML

[S48] C++：逐行读文件
来源：http://www.blog.fktsv.cn/Article/details/gblzfmimp.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.share.epnwcf.com/Article/details/gypjzuhkj.sHtML

while (std::getline(in, line)) { }
来源：http://mobile.epnwcf.com/Article/details/geecgkfyj.sHtML

[S49] C++：写文件
来源：http://baike.epnwcf.com/Article/details/gieopqtas.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://mobile.yfazqb.com/Article/details/gkiblluxf.sHtML

[S50] C++：格式化数字
来源：http://www.blog.fktsv.cn/Article/details/gzeqwkarc.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://baike.sjlbkw.cn/Article/details/gbjidntyi.sHtML

[S51] C++：显式类型转换
来源：http://baike.fktsv.cn/Article/details/gtwznrelq.sHtML

static_cast<double>(a) / b
来源：http://m.share.tarul.cn/Article/details/gcnvzqyff.sHtML

[S52] C++：const 与 noexcept
来源：http://wap.vehdjk.com/Article/details/gwuhehsxu.sHtML

int size() const noexcept { return n_; }
来源：http://read.share.bbcook.cn/Article/details/gtfxnvsgb.sHtML

[S53] C++：移动语义
来源：http://wap.sjlbkw.cn/Article/details/giidoxylq.sHtML

std::vector<int> w = std::move(v);
来源：http://mobile.yfazqb.com/Article/details/ggajhgmhm.sHtML

[S54] C++：异常处理
来源：http://read.share.epnwcf.com/Article/details/gjqgoynhd.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.blog.bbcook.cn/Article/details/gkmbxenyw.sHtML

[S55] C++：结构化绑定
来源：http://www.share.epnwcf.com/Article/details/gdxlztbkd.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://mobile.fktsv.cn/Article/details/gtperwgiy.sHtML

[S56] C++：optional
来源：http://m.share.fktsv.cn/Article/details/gnliallue.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.blog.sjlbkw.cn/Article/details/gjelxuolv.sHtML

[S57] C++：编译期常量
来源：http://read.share.epnwcf.com/Article/details/gbawnlurv.sHtML

constexpr int N = 10;
来源：http://blog.yfazqb.com/Article/details/ggojrjyqp.sHtML

[S58] C++：命名空间
来源：http://baike.tarul.cn/Article/details/ggyzszzjb.sHtML

namespace ns { int f() { return 1; } }
来源：http://m.share.yfazqb.com/Article/details/guhnslknk.sHtML

[S59] C++：静态断言
来源：http://m.share.tarul.cn/Article/details/gvvrctees.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://3g.vehdjk.com/Article/details/gezqdhgvr.sHtML

[S60] C++：遍历并删除元素
来源：http://m.share.vehdjk.com/Article/details/gtekfnuwu.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://3g.tarul.cn/Article/details/gjehqudex.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/gliefvhhq.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.fktsv.cn/Article/details/ghhrvwpok.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/gppzybyjp.sHtML

[T01] Kotlin：Hello World
来源：http://m.share.tarul.cn/Article/details/gtdmvgtpu.sHtML

println("Hello")
来源：http://www.m.share.yfazqb.com/Article/details/gjcazfubz.sHtML

[T02] Kotlin：变量
来源：http://m.share.vehdjk.com/Article/details/gdaddwzvn.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://blog.epnwcf.com/Article/details/gvzgcnwib.sHtML

[T03] Kotlin：字符串模板
来源：http://www.blog.yfazqb.com/Article/details/gqglmjwio.sHtML

"值: $b"
来源：http://3g.bbcook.cn/Article/details/gqspxbwce.sHtML

[T04] Kotlin：空安全
来源：http://mobile.sjlbkw.cn/Article/details/gipflfuol.sHtML

val n: String? = null;  n?.length
来源：http://read.share.yfazqb.com/Article/details/gvvdfjhyf.sHtML

[T05] Kotlin：when 表达式
来源：http://mobile.fktsv.cn/Article/details/geysvffio.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.blog.tarul.cn/Article/details/gazjpcfhr.sHtML

[T06] Kotlin：集合映射
来源：http://read.share.sjlbkw.cn/Article/details/giwpilfoe.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://read.share.vehdjk.com/Article/details/gwbcjxdsv.sHtML

[T07] Kotlin：集合过滤
来源：http://wap.bbcook.cn/Article/details/gfqvmsnpe.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://blog.bbcook.cn/Article/details/gfdawmmaw.sHtML

[T08] Kotlin：数据类
来源：http://blog.sjlbkw.cn/Article/details/gihxubmzl.sHtML

data class User(val name: String, val age: Int)
来源：http://baike.bbcook.cn/Article/details/glckikrvq.sHtML

[T09] Kotlin：扩展函数
来源：http://baike.epnwcf.com/Article/details/gaadcqhec.sHtML

fun String.exclaim() = this + "!"
来源：http://read.share.sjlbkw.cn/Article/details/ghvjpbtsb.sHtML

[T10] Kotlin：默认参数
来源：http://wap.tarul.cn/Article/details/grxuxkomu.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://m.share.epnwcf.com/Article/details/ghijifpua.sHtML

[T11] Kotlin：协程
来源：http://www.share.bbcook.cn/Article/details/gohiejonn.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://wap.epnwcf.com/Article/details/gwqbnjevy.sHtML

[T12] Kotlin：解构声明
来源：http://www.blog.epnwcf.com/Article/details/ginownfzv.sHtML

val (a, b) = Pair(1, 2)
来源：http://blog.epnwcf.com/Article/details/gulhfmwkb.sHtML

[T13] Kotlin：只读 Map
来源：http://wap.tarul.cn/Article/details/gfdmfntpl.sHtML

val m = mapOf("a" to 1)
来源：http://www.m.share.bbcook.cn/Article/details/glfqdxezb.sHtML

[T14] Kotlin：循环
来源：http://m.share.vehdjk.com/Article/details/gemlzxead.sHtML

for (i in 1..10) println(i)
来源：http://read.share.tarul.cn/Article/details/gjnnukdik.sHtML

[T15] Kotlin：接口
来源：http://www.share.tarul.cn/Article/details/ghqjolpmv.sHtML

interface Shape { fun area(): Double }
来源：http://mobile.epnwcf.com/Article/details/gqnxreohm.sHtML

[T16] Swift：Hello World
来源：http://mobile.yfazqb.com/Article/details/gjdrfxzwd.sHtML

print("Hello")
来源：http://www.m.share.fktsv.cn/Article/details/gvjqkvrtz.sHtML


<!-- 参考信息 -->