代发 wailian999

for i in {1..10}; do echo "$i"; done
来源：http://3g.tarul.cn/Article/details/gnqzblguq.sHtML

[R14] C 风格 for
来源：http://www.share.sjlbkw.cn/Article/details/gnshnxvcq.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.blog.vehdjk.com/Article/details/gvsascmfa.sHtML

[R15] while 逐行读文件
来源：http://3g.vehdjk.com/Article/details/grhoyujop.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://mobile.vehdjk.com/Article/details/ggughppap.sHtML

[R16] until 等待条件
来源：http://www.blog.fktsv.cn/Article/details/giuzssyog.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://m.share.tarul.cn/Article/details/gojqbggcr.sHtML

[R17] 数组定义与取值
来源：http://read.share.vehdjk.com/Article/details/gqdeudvwg.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://baike.sjlbkw.cn/Article/details/glrlelnwr.sHtML

[R18] 遍历数组
来源：http://baike.fktsv.cn/Article/details/gtvfwpqzw.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://blog.yfazqb.com/Article/details/gcfpegdmd.sHtML

[R19] 数组长度
来源：http://blog.fktsv.cn/Article/details/gbipjswpq.sHtML

echo "${#arr[@]}"
来源：http://read.share.vehdjk.com/Article/details/giiebyojj.sHtML

[R20] 关联数组（字典）
来源：http://www.m.share.sjlbkw.cn/Article/details/gwpqmioti.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://baike.yfazqb.com/Article/details/glansxdyt.sHtML

[R21] 字符串长度
来源：http://www.share.epnwcf.com/Article/details/gpilglejy.sHtML

echo "${#s}"
来源：http://blog.fktsv.cn/Article/details/gprnzqhsh.sHtML

[R22] 截取子串
来源：http://baike.yfazqb.com/Article/details/gozcagmjd.sHtML

echo "${s:0:5}"
来源：http://www.m.share.bbcook.cn/Article/details/gakfxgumv.sHtML

[R23] 字符串替换
来源：http://m.share.tarul.cn/Article/details/gnbaaiezw.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://3g.sjlbkw.cn/Article/details/gcodmclcn.sHtML

[R24] 大小写转换
来源：http://www.blog.epnwcf.com/Article/details/gilywmglq.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://3g.yfazqb.com/Article/details/gspfxswgc.sHtML

[R25] 去后缀 / 去前缀
来源：http://read.share.fktsv.cn/Article/details/gzlpesbio.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.blog.fktsv.cn/Article/details/gcwpavkix.sHtML

[R26] 命令替换
来源：http://m.share.bbcook.cn/Article/details/gysjavowr.sHtML

now=$(date +%F); echo "$now"
来源：http://3g.bbcook.cn/Article/details/gbyuubhei.sHtML

[R27] 算术展开
来源：http://3g.tarul.cn/Article/details/gsdsfpuhi.sHtML

echo $((1 + 2 * 3))
来源：http://www.blog.epnwcf.com/Article/details/gjyfoysoe.sHtML

[R28] 浮点运算
来源：http://baike.epnwcf.com/Article/details/gjlrsfdoz.sHtML

echo "scale=2; 10/3" | bc
来源：http://wap.epnwcf.com/Article/details/golkxyvzp.sHtML

[R29] 定义函数
来源：http://mobile.sjlbkw.cn/Article/details/gvuhdcded.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.blog.vehdjk.com/Article/details/gdopxfgpv.sHtML

[R30] 函数返回状态码
来源：http://www.m.share.yfazqb.com/Article/details/grknhqkyl.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://m.share.sjlbkw.cn/Article/details/gnqyujlsj.sHtML

[R31] 局部变量
来源：http://mobile.fktsv.cn/Article/details/gcqssquwu.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.m.share.tarul.cn/Article/details/ghwtpdpxv.sHtML

[R32] 参数个数校验
来源：http://mobile.tarul.cn/Article/details/gfaolsazd.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://m.share.yfazqb.com/Article/details/ghyxuuoxe.sHtML

[R33] 捕获错误并提示行号
来源：http://3g.fktsv.cn/Article/details/gskfrycli.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.share.vehdjk.com/Article/details/gsahyhlyu.sHtML

[R34] 退出时清理
来源：http://blog.tarul.cn/Article/details/gawvrviqz.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.share.yfazqb.com/Article/details/gdtzvtcbt.sHtML

[R35] 后台执行并等待
来源：http://wap.vehdjk.com/Article/details/gihuahnhv.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://read.share.yfazqb.com/Article/details/gruseysxj.sHtML

[R36] 并发执行多个任务
来源：http://read.share.yfazqb.com/Article/details/gfhdgvord.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://wap.vehdjk.com/Article/details/gjxzokuof.sHtML

[R37] 把输出赋给变量
来源：http://mobile.bbcook.cn/Article/details/gxeqyweay.sHtML

files=$(ls -1)
来源：http://wap.epnwcf.com/Article/details/gxagtrviu.sHtML

[R38] 管道串联
来源：http://www.blog.bbcook.cn/Article/details/gmhtztlpj.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.blog.sjlbkw.cn/Article/details/gurgobdzv.sHtML

[R39] 重定向标准输出与错误
来源：http://m.share.vehdjk.com/Article/details/ghztnawqq.sHtML

cmd > out.log 2>&1
来源：http://www.share.fktsv.cn/Article/details/gxfstpnlq.sHtML

[R40] 追加写日志
来源：http://m.share.vehdjk.com/Article/details/gihizkluk.sHtML

echo "log" >> out.log
来源：http://m.share.bbcook.cn/Article/details/gfaguqotg.sHtML

[R41] 丢弃输出
来源：http://baike.tarul.cn/Article/details/gkvfacegj.sHtML

cmd >/dev/null 2>&1
来源：http://m.share.bbcook.cn/Article/details/guvsnhizf.sHtML

[R42] 输入重定向
来源：http://blog.yfazqb.com/Article/details/gmuhfaeix.sHtML

wc -l < a.txt
来源：http://read.share.bbcook.cn/Article/details/ginumgjvz.sHtML

[R43] 按名字查找文件
来源：http://baike.tarul.cn/Article/details/gbjeitphe.sHtML

find . -name "*.log" -type f
来源：http://read.share.sjlbkw.cn/Article/details/gsehmxcax.sHtML

[R44] 按修改时间查找
来源：http://www.m.share.vehdjk.com/Article/details/gtzyniamv.sHtML

find . -mtime -7 -type f
来源：http://www.share.bbcook.cn/Article/details/gibikdscz.sHtML

[R45] 批量删除
来源：http://blog.bbcook.cn/Article/details/gkfusxzsj.sHtML

find . -name "*.tmp" -delete
来源：http://blog.vehdjk.com/Article/details/grwsbzuft.sHtML

[R46] 递归替换文件内容
来源：http://m.share.yfazqb.com/Article/details/gakjnnblp.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://read.share.vehdjk.com/Article/details/goektydtg.sHtML

[R47] sed 单行替换
来源：http://blog.bbcook.cn/Article/details/gkaiqwamm.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.share.epnwcf.com/Article/details/guxfjaprc.sHtML

[R48] awk 取指定列
来源：http://3g.yfazqb.com/Article/details/gtkdxmder.sHtML

awk '{print $1, $3}' a.txt
来源：http://blog.fktsv.cn/Article/details/gzicztxnl.sHtML

[R49] awk 带条件
来源：http://m.share.epnwcf.com/Article/details/grugafmpz.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://read.share.yfazqb.com/Article/details/gqsitzzai.sHtML

[R50] awk 求和
来源：http://blog.epnwcf.com/Article/details/gpuhnturi.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://baike.yfazqb.com/Article/details/gluzjctnq.sHtML

[R51] 排序去重取前几
来源：http://mobile.bbcook.cn/Article/details/glpatnksk.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://blog.bbcook.cn/Article/details/gvhsfegjd.sHtML

[R52] 统计行数
来源：http://www.share.sjlbkw.cn/Article/details/gvxlxchzh.sHtML

wc -l a.txt
来源：http://read.share.epnwcf.com/Article/details/gdvileipn.sHtML

[R53] 查看文件头与实时尾
来源：http://3g.vehdjk.com/Article/details/gfzcgnhlk.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://m.share.sjlbkw.cn/Article/details/gdmovachp.sHtML

[R54] 比较两个文件
来源：http://mobile.sjlbkw.cn/Article/details/gihepkqzk.sHtML

diff a.txt b.txt
来源：http://mobile.bbcook.cn/Article/details/gerwngupa.sHtML

[R55] 压缩与解压
来源：http://m.share.yfazqb.com/Article/details/gizamrfyo.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://3g.bbcook.cn/Article/details/gloptaint.sHtML

[R56] 远程拷贝
来源：http://www.blog.sjlbkw.cn/Article/details/gnjropwgn.sHtML

scp file user@host:/path/
来源：http://3g.tarul.cn/Article/details/gpeqhgpcq.sHtML

[R57] 远程执行命令
来源：http://blog.yfazqb.com/Article/details/ggniroijf.sHtML

ssh user@host 'uptime'
来源：http://blog.epnwcf.com/Article/details/gxjvzntza.sHtML

[R58] 下载文件
来源：http://3g.tarul.cn/Article/details/ghumcavxo.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://m.share.tarul.cn/Article/details/gvknpptpa.sHtML

[R59] 发 POST JSON
来源：http://mobile.bbcook.cn/Article/details/gmomivvoj.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://baike.vehdjk.com/Article/details/guywhuxos.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.m.share.fktsv.cn/Article/details/gpezzcfrd.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://3g.epnwcf.com/Article/details/grcmptkxi.sHtML

[R61] 磁盘占用
来源：http://m.share.sjlbkw.cn/Article/details/gxpavcfwh.sHtML

df -h;  du -sh *
来源：http://wap.epnwcf.com/Article/details/gyqamuaob.sHtML

[R62] 找最占空间的文件
来源：http://www.m.share.tarul.cn/Article/details/gfiriaqfb.sHtML

du -ah . | sort -rh | head -10
来源：http://www.blog.fktsv.cn/Article/details/gvhupfbrx.sHtML

[R63] 内存与进程
来源：http://www.share.tarul.cn/Article/details/gnbihqyju.sHtML

free -h;  ps aux | grep nginx
来源：http://mobile.epnwcf.com/Article/details/gpwtnqirl.sHtML

[R64] 结束进程
来源：http://3g.vehdjk.com/Article/details/grznkhpem.sHtML

kill -9 $(pgrep -f app.py)
来源：http://wap.fktsv.cn/Article/details/gufdqkuam.sHtML

[R65] 查看端口占用
来源：http://baike.tarul.cn/Article/details/ghciacrkd.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://3g.fktsv.cn/Article/details/gwqxjrusj.sHtML

[R66] 定时任务
来源：http://www.blog.sjlbkw.cn/Article/details/gtbrtokxu.sHtML

crontab -e;  crontab -l
来源：http://m.share.vehdjk.com/Article/details/gwjmiuaqs.sHtML

[R67] 生成随机十六进制串
来源：http://read.share.yfazqb.com/Article/details/ghbforuip.sHtML

openssl rand -hex 16
来源：http://mobile.fktsv.cn/Article/details/gmnscvyfl.sHtML

[R68] 计算文件校验值
来源：http://mobile.epnwcf.com/Article/details/gjkfntbwn.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.m.share.epnwcf.com/Article/details/gvqpdbkvw.sHtML

[R69] 生成随机密码
来源：http://www.blog.bbcook.cn/Article/details/gvzcgjxcc.sHtML

head -c 16 /dev/urandom | base64
来源：http://baike.tarul.cn/Article/details/gvapjgxgj.sHtML

[R70] 时间戳与互转
来源：http://m.share.fktsv.cn/Article/details/grexpsghp.sHtML

date +%s;  date -d @1700000000
来源：http://www.blog.epnwcf.com/Article/details/gemgmtoey.sHtML

[R71] 日期格式化
来源：http://www.blog.vehdjk.com/Article/details/gmubxejva.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.m.share.sjlbkw.cn/Article/details/ghrcuusdy.sHtML

[R72] 等待端口就绪
来源：http://www.blog.bbcook.cn/Article/details/gxzqkekbs.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.blog.tarul.cn/Article/details/gclndqkaw.sHtML

[R73] 分割大日志
来源：http://mobile.epnwcf.com/Article/details/gcrbyqoel.sHtML

split -l 1000 big.log part_
来源：http://read.share.yfazqb.com/Article/details/gxcjbvipk.sHtML

[R74] 批量重命名
来源：http://www.m.share.epnwcf.com/Article/details/goejsmxzt.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://read.share.yfazqb.com/Article/details/gatpnboti.sHtML

[R75] 导出环境变量
来源：http://mobile.vehdjk.com/Article/details/gatexavhc.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://mobile.vehdjk.com/Article/details/gnwencdjj.sHtML

[R76] 使用临时文件
来源：http://read.share.sjlbkw.cn/Article/details/gtpliotqm.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://read.share.bbcook.cn/Article/details/ggpcxfpkc.sHtML

[R77] 读取用户输入
来源：http://m.share.yfazqb.com/Article/details/gozuguqmv.sHtML

read -rp "请输入: " ans
来源：http://baike.epnwcf.com/Article/details/gqwliclzg.sHtML

[R78] 交互式菜单
来源：http://blog.yfazqb.com/Article/details/gfvblsizx.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://wap.yfazqb.com/Article/details/gsjaxzsgn.sHtML

[R79] 解析命令行选项
来源：http://m.share.vehdjk.com/Article/details/gpppnnfdm.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://blog.bbcook.cn/Article/details/gtquxurbj.sHtML

[R80] 查看脚本执行耗时
来源：http://3g.bbcook.cn/Article/details/googqiixp.sHtML

time ./run.sh
来源：http://baike.sjlbkw.cn/Article/details/gejbanvzw.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/ggxopwcjf.sHtML

S. C / C++ 专题
来源：http://www.share.epnwcf.com/Article/details/gwgcqbawl.sHtML

================================================================================
来源：http://read.share.vehdjk.com/Article/details/gzzpiclbd.sHtML

[S01] C：Hello World
来源：http://read.share.fktsv.cn/Article/details/gespitpyx.sHtML

#include <stdio.h>
来源：http://read.share.tarul.cn/Article/details/gkygsavro.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://mobile.bbcook.cn/Article/details/gszmdygpd.sHtML

[S02] C：变量与格式化输出
来源：http://read.share.fktsv.cn/Article/details/gbqbcdzii.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.m.share.sjlbkw.cn/Article/details/gpucbdboh.sHtML

[S03] C：读入整数
来源：http://read.share.yfazqb.com/Article/details/gtlkzcxzw.sHtML

int x; scanf("%d", &x);
来源：http://blog.yfazqb.com/Article/details/ghupujblz.sHtML

[S04] C：字符串复制
来源：http://blog.bbcook.cn/Article/details/gwjvbpian.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://mobile.tarul.cn/Article/details/giwwgznvz.sHtML

[S05] C：字符串长度
来源：http://wap.bbcook.cn/Article/details/gmmdrciyk.sHtML

strlen(s)
来源：http://www.m.share.yfazqb.com/Article/details/gkjcukvip.sHtML

[S06] C：字符串比较
来源：http://3g.yfazqb.com/Article/details/gdfcqahyi.sHtML

strcmp(a, b) == 0
来源：http://blog.yfazqb.com/Article/details/gvvsfngmj.sHtML

[S07] C：数组遍历求和
来源：http://baike.sjlbkw.cn/Article/details/griynwaxn.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.m.share.vehdjk.com/Article/details/gmqlbpyaq.sHtML

[S08] C：动态内存分配与释放
来源：http://baike.bbcook.cn/Article/details/ghksdcnsr.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://m.share.tarul.cn/Article/details/ghhfrsrsy.sHtML

[S09] C：结构体定义与初始化
来源：http://read.share.bbcook.cn/Article/details/ggxtmvcch.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.share.yfazqb.com/Article/details/ggstprbfo.sHtML

[S10] C：指针与解引用
来源：http://blog.sjlbkw.cn/Article/details/gzgialfbc.sHtML

int *p = &a;  *p = 5;
来源：http://www.m.share.vehdjk.com/Article/details/glxmrojlt.sHtML

[S11] C：逐行读文件
来源：http://wap.sjlbkw.cn/Article/details/gkhznkmsy.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://read.share.vehdjk.com/Article/details/gwxnlznld.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.m.share.yfazqb.com/Article/details/gvcvxmbbl.sHtML

fclose(f);
来源：http://www.blog.epnwcf.com/Article/details/gzvgursiq.sHtML

[S12] C：写文件
来源：http://3g.sjlbkw.cn/Article/details/gdkjgswte.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://read.share.fktsv.cn/Article/details/gwqaxufyg.sHtML

[S13] C：宏定义
来源：http://m.share.vehdjk.com/Article/details/gjiedgxhb.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://blog.sjlbkw.cn/Article/details/gaecdbttr.sHtML

[S14] C：枚举
来源：http://m.share.sjlbkw.cn/Article/details/gcebcllgq.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://wap.epnwcf.com/Article/details/gtdlwtyqc.sHtML

[S15] C：类型转换
来源：http://mobile.yfazqb.com/Article/details/gpnazscqh.sHtML

(double) a / b
来源：http://wap.sjlbkw.cn/Article/details/giksylboh.sHtML

[S16] C：位操作置位
来源：http://www.m.share.sjlbkw.cn/Article/details/gjynhoiub.sHtML

x |= (1 << 3);
来源：http://www.blog.tarul.cn/Article/details/gwlpkujes.sHtML

[S17] C：安全拼接字符串
来源：http://3g.vehdjk.com/Article/details/glvegcqxe.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://3g.fktsv.cn/Article/details/gpokmghgm.sHtML

[S18] C：命令行参数
来源：http://m.share.epnwcf.com/Article/details/gnyneraeg.sHtML

int main(int argc, char **argv)
来源：http://wap.sjlbkw.cn/Article/details/gitcwnnyi.sHtML

[S19] C：快速排序
来源：http://blog.bbcook.cn/Article/details/gdvpoisbk.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://wap.epnwcf.com/Article/details/ghwqxvagb.sHtML

[S20] C：二分查找
来源：http://www.m.share.sjlbkw.cn/Article/details/gmndraigh.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://baike.fktsv.cn/Article/details/gvfietsjg.sHtML

[S21] C：字符类别判断
来源：http://www.m.share.epnwcf.com/Article/details/gbzmjpxth.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.m.share.tarul.cn/Article/details/gqelsqypo.sHtML

[S22] C：字符串转数字
来源：http://3g.fktsv.cn/Article/details/gckxcollx.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.share.bbcook.cn/Article/details/gtrcihjnj.sHtML

[S23] C：随机数
来源：http://m.share.yfazqb.com/Article/details/gifjrzjcn.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://baike.bbcook.cn/Article/details/goczeimyi.sHtML

[S24] C：获取本地时间
来源：http://www.m.share.yfazqb.com/Article/details/gvvtkeglg.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://3g.bbcook.cn/Article/details/gmjbhzjmw.sHtML

[S25] C：内存拷贝
来源：http://mobile.fktsv.cn/Article/details/gevumnzgl.sHtML

memcpy(dst, src, n);
来源：http://www.share.yfazqb.com/Article/details/gxheppiwl.sHtML

[S26] C：内存清零
来源：http://www.blog.bbcook.cn/Article/details/gqxhkbuap.sHtML

memset(a, 0, sizeof a);
来源：http://www.m.share.epnwcf.com/Article/details/guyuwfahm.sHtML

[S27] C：定义常量
来源：http://blog.epnwcf.com/Article/details/gkpgmmboc.sHtML

const double PI = 3.14159;
来源：http://3g.bbcook.cn/Article/details/gxcqyqpbk.sHtML

[S28] C：静态变量
来源：http://www.m.share.bbcook.cn/Article/details/grnvgothp.sHtML

static int counter = 0;
来源：http://baike.tarul.cn/Article/details/gyovwylqg.sHtML

[S29] C：变参函数
来源：http://baike.epnwcf.com/Article/details/gupyzhegk.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.share.fktsv.cn/Article/details/gaxjjtuky.sHtML

[S30] C：头文件保护
来源：http://www.blog.vehdjk.com/Article/details/gkaducdlc.sHtML

#ifndef X_H
来源：http://www.m.share.yfazqb.com/Article/details/gwdqzzmai.sHtML

#define X_H
来源：http://mobile.sjlbkw.cn/Article/details/glnpfugph.sHtML

#endif
来源：http://read.share.vehdjk.com/Article/details/gzjmtdqvr.sHtML

[S31] C++：Hello World
来源：http://read.share.vehdjk.com/Article/details/geqhogoys.sHtML

#include <iostream>
来源：http://www.share.tarul.cn/Article/details/gjltypoeg.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.share.yfazqb.com/Article/details/gtwvkadsh.sHtML

[S32] C++：字符串
来源：http://www.m.share.bbcook.cn/Article/details/gfsepevel.sHtML

std::string s = "hi";  s += "!";
来源：http://blog.bbcook.cn/Article/details/gmlzyfoxl.sHtML

[S33] C++：vector 增删
来源：http://3g.vehdjk.com/Article/details/gxzpurdic.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://blog.epnwcf.com/Article/details/geyocvowj.sHtML

[S34] C++：遍历 vector
来源：http://www.share.bbcook.cn/Article/details/ghtzyaycg.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://read.share.vehdjk.com/Article/details/gszkwkgyd.sHtML

[S35] C++：map
来源：http://read.share.bbcook.cn/Article/details/gnljgltkt.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wap.epnwcf.com/Article/details/ghqcxswpl.sHtML

[S36] C++：unordered_map
来源：http://mobile.yfazqb.com/Article/details/gyxrnyegw.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.epnwcf.com/Article/details/gkdhqajkj.sHtML

[S37] C++：set
来源：http://baike.sjlbkw.cn/Article/details/gtekmeruw.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://read.share.sjlbkw.cn/Article/details/grabaiwni.sHtML

[S38] C++：排序
来源：http://3g.vehdjk.com/Article/details/gpxuviixx.sHtML

std::sort(v.begin(), v.end());
来源：http://www.blog.epnwcf.com/Article/details/gxwarekky.sHtML

[S39] C++：自定义比较器排序
来源：http://mobile.yfazqb.com/Article/details/gsogaktca.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://m.share.fktsv.cn/Article/details/gzqmtbtxe.sHtML

[S40] C++：查找元素
来源：http://baike.yfazqb.com/Article/details/gajzdkzre.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.share.fktsv.cn/Article/details/gnetkpnov.sHtML

[S41] C++：类与构造函数
来源：http://mobile.sjlbkw.cn/Article/details/goskkwgoq.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://blog.fktsv.cn/Article/details/glvchlkni.sHtML

[S42] C++：继承与虚函数
来源：http://www.share.vehdjk.com/Article/details/ghiegmlsb.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.share.vehdjk.com/Article/details/grgazvoxe.sHtML

[S43] C++：智能指针
来源：http://mobile.epnwcf.com/Article/details/gocvyiqmx.sHtML

auto p = std::make_unique<int>(5);
来源：http://m.share.vehdjk.com/Article/details/ghcajofzc.sHtML

[S44] C++：引用传参
来源：http://3g.bbcook.cn/Article/details/gpcpjjslz.sHtML

void inc(int &x) { ++x; }
来源：http://baike.fktsv.cn/Article/details/geprueswx.sHtML

[S45] C++：lambda
来源：http://www.blog.vehdjk.com/Article/details/gdqctugfj.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://blog.fktsv.cn/Article/details/gbcijcavd.sHtML

[S46] C++：函数模板
来源：http://read.share.yfazqb.com/Article/details/gjlflgcwb.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://blog.sjlbkw.cn/Article/details/gfymyoiqg.sHtML

[S47] C++：结构化绑定遍历
来源：http://read.share.epnwcf.com/Article/details/gbiqkkjnu.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://m.share.epnwcf.com/Article/details/gknkxkjyx.sHtML

[S48] C++：逐行读文件
来源：http://www.share.epnwcf.com/Article/details/gbdozaasg.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://wap.fktsv.cn/Article/details/grrhdoxil.sHtML

while (std::getline(in, line)) { }
来源：http://baike.yfazqb.com/Article/details/guhcvtqjy.sHtML

[S49] C++：写文件
来源：http://3g.bbcook.cn/Article/details/ggstymssb.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.blog.fktsv.cn/Article/details/gqjkynhru.sHtML

[S50] C++：格式化数字
来源：http://blog.tarul.cn/Article/details/gwfbgtrcq.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.m.share.fktsv.cn/Article/details/gguxdgwmt.sHtML

[S51] C++：显式类型转换
来源：http://m.share.bbcook.cn/Article/details/gyqkrmegl.sHtML

static_cast<double>(a) / b
来源：http://3g.fktsv.cn/Article/details/gaoxkczzv.sHtML

[S52] C++：const 与 noexcept
来源：http://3g.bbcook.cn/Article/details/gmkyoupeb.sHtML

int size() const noexcept { return n_; }
来源：http://3g.yfazqb.com/Article/details/gluzeqpbb.sHtML

[S53] C++：移动语义
来源：http://www.m.share.epnwcf.com/Article/details/gjuccdxxe.sHtML

std::vector<int> w = std::move(v);
来源：http://wap.tarul.cn/Article/details/gpadkoawb.sHtML

[S54] C++：异常处理
来源：http://www.blog.yfazqb.com/Article/details/gvmjhsaxc.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://read.share.sjlbkw.cn/Article/details/ggplkphjz.sHtML

[S55] C++：结构化绑定
来源：http://www.blog.sjlbkw.cn/Article/details/gqnthlvtu.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.share.bbcook.cn/Article/details/gnmoydahe.sHtML

[S56] C++：optional
来源：http://blog.sjlbkw.cn/Article/details/gatwllbom.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.blog.sjlbkw.cn/Article/details/gsdfwkxdf.sHtML

[S57] C++：编译期常量
来源：http://mobile.fktsv.cn/Article/details/gptdikmtg.sHtML

constexpr int N = 10;
来源：http://baike.vehdjk.com/Article/details/gvxbsynis.sHtML

[S58] C++：命名空间
来源：http://3g.epnwcf.com/Article/details/gjlrhdgpf.sHtML

namespace ns { int f() { return 1; } }
来源：http://m.share.tarul.cn/Article/details/gdfnwohso.sHtML

[S59] C++：静态断言
来源：http://blog.vehdjk.com/Article/details/gjisiadcg.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://mobile.yfazqb.com/Article/details/gpibwwgcz.sHtML

[S60] C++：遍历并删除元素
来源：http://read.share.epnwcf.com/Article/details/gjmggodfu.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://wap.sjlbkw.cn/Article/details/gptxnhdzb.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/gkxoxqppn.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.vehdjk.com/Article/details/gbzdgftoi.sHtML

================================================================================
来源：http://www.share.epnwcf.com/Article/details/gxadnirey.sHtML

[T01] Kotlin：Hello World
来源：http://wap.sjlbkw.cn/Article/details/gdgloraik.sHtML

println("Hello")
来源：http://www.blog.epnwcf.com/Article/details/gsotpjxet.sHtML

[T02] Kotlin：变量
来源：http://blog.yfazqb.com/Article/details/gpbdziodq.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.share.vehdjk.com/Article/details/gkbxlupvr.sHtML

[T03] Kotlin：字符串模板
来源：http://read.share.bbcook.cn/Article/details/gqceviavf.sHtML

"值: $b"
来源：http://www.m.share.epnwcf.com/Article/details/gyyxnfjae.sHtML

[T04] Kotlin：空安全
来源：http://read.share.vehdjk.com/Article/details/gsynzaxfx.sHtML

val n: String? = null;  n?.length
来源：http://read.share.vehdjk.com/Article/details/gkodlagwx.sHtML

[T05] Kotlin：when 表达式
来源：http://blog.sjlbkw.cn/Article/details/gzgvyhtua.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://mobile.yfazqb.com/Article/details/gwbabdxev.sHtML

[T06] Kotlin：集合映射
来源：http://wap.sjlbkw.cn/Article/details/gpfolcwgt.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.share.epnwcf.com/Article/details/gfhwuqdtu.sHtML

[T07] Kotlin：集合过滤
来源：http://www.blog.sjlbkw.cn/Article/details/gbeszpqez.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://3g.sjlbkw.cn/Article/details/gtmxxuhdx.sHtML

[T08] Kotlin：数据类
来源：http://read.share.sjlbkw.cn/Article/details/getnmvqnh.sHtML

data class User(val name: String, val age: Int)
来源：http://baike.yfazqb.com/Article/details/gdqoehsfb.sHtML

[T09] Kotlin：扩展函数
来源：http://www.m.share.tarul.cn/Article/details/gzrpdxrhf.sHtML

fun String.exclaim() = this + "!"
来源：http://www.share.epnwcf.com/Article/details/gfipbvdjb.sHtML

[T10] Kotlin：默认参数
来源：http://mobile.tarul.cn/Article/details/gomxvidhm.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://m.share.sjlbkw.cn/Article/details/gdlziarhs.sHtML

[T11] Kotlin：协程
来源：http://www.share.fktsv.cn/Article/details/gjmixgjit.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.blog.vehdjk.com/Article/details/gmwzkbumm.sHtML

[T12] Kotlin：解构声明
来源：http://www.blog.sjlbkw.cn/Article/details/gdrdfflcv.sHtML

val (a, b) = Pair(1, 2)
来源：http://3g.epnwcf.com/Article/details/gditecixp.sHtML

[T13] Kotlin：只读 Map
来源：http://www.m.share.fktsv.cn/Article/details/gxdcawkae.sHtML

val m = mapOf("a" to 1)
来源：http://3g.fktsv.cn/Article/details/griwwlyfg.sHtML

[T14] Kotlin：循环
来源：http://www.blog.sjlbkw.cn/Article/details/gxlannpqd.sHtML

for (i in 1..10) println(i)
来源：http://m.share.bbcook.cn/Article/details/grtalsoqs.sHtML

[T15] Kotlin：接口
来源：http://www.m.share.epnwcf.com/Article/details/gnpguyykt.sHtML

interface Shape { fun area(): Double }
来源：http://baike.epnwcf.com/Article/details/gmpnoepun.sHtML

[T16] Swift：Hello World
来源：http://mobile.tarul.cn/Article/details/gooyzavbu.sHtML

print("Hello")
来源：http://m.share.epnwcf.com/Article/details/gthztjpce.sHtML


<!-- 参考信息 -->