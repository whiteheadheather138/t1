代发 wailian999

arr=(a b c); echo "${arr[0]}"
来源：http://www.share.vehdjk.com/Article/details/gxmwkxued.sHtML

[R18] 遍历数组
来源：http://3g.epnwcf.com/Article/details/gyknpfxke.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.blog.yfazqb.com/Article/details/gtrxskwrt.sHtML

[R19] 数组长度
来源：http://read.share.epnwcf.com/Article/details/glwzegkop.sHtML

echo "${#arr[@]}"
来源：http://3g.sjlbkw.cn/Article/details/gwdkiloav.sHtML

[R20] 关联数组（字典）
来源：http://wap.vehdjk.com/Article/details/gafzjavdk.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.share.bbcook.cn/Article/details/gxzwbnrao.sHtML

[R21] 字符串长度
来源：http://baike.vehdjk.com/Article/details/gunplngsj.sHtML

echo "${#s}"
来源：http://read.share.tarul.cn/Article/details/gqxxjazzk.sHtML

[R22] 截取子串
来源：http://www.blog.vehdjk.com/Article/details/gbhbeoqwn.sHtML

echo "${s:0:5}"
来源：http://www.share.bbcook.cn/Article/details/gygenkppe.sHtML

[R23] 字符串替换
来源：http://www.m.share.fktsv.cn/Article/details/glapwifhd.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://blog.yfazqb.com/Article/details/gtnfozgki.sHtML

[R24] 大小写转换
来源：http://mobile.yfazqb.com/Article/details/gpdgcemjf.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.blog.yfazqb.com/Article/details/gdijonohq.sHtML

[R25] 去后缀 / 去前缀
来源：http://mobile.yfazqb.com/Article/details/gtbmptlap.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://m.share.yfazqb.com/Article/details/gwvggnnly.sHtML

[R26] 命令替换
来源：http://www.share.fktsv.cn/Article/details/gffzwicsj.sHtML

now=$(date +%F); echo "$now"
来源：http://read.share.sjlbkw.cn/Article/details/gmqipteni.sHtML

[R27] 算术展开
来源：http://read.share.sjlbkw.cn/Article/details/gstfouxes.sHtML

echo $((1 + 2 * 3))
来源：http://www.blog.yfazqb.com/Article/details/gvzjjtyaa.sHtML

[R28] 浮点运算
来源：http://baike.yfazqb.com/Article/details/gmffdhxqz.sHtML

echo "scale=2; 10/3" | bc
来源：http://read.share.bbcook.cn/Article/details/ghrdsptsx.sHtML

[R29] 定义函数
来源：http://www.m.share.vehdjk.com/Article/details/ggzxfkyfy.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://baike.epnwcf.com/Article/details/gulfjibcx.sHtML

[R30] 函数返回状态码
来源：http://wap.yfazqb.com/Article/details/gzrgsgssf.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://blog.vehdjk.com/Article/details/gyhnbzkho.sHtML

[R31] 局部变量
来源：http://read.share.fktsv.cn/Article/details/ggynrvgna.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.m.share.epnwcf.com/Article/details/gvzefyzpx.sHtML

[R32] 参数个数校验
来源：http://mobile.tarul.cn/Article/details/gpiozwyne.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.m.share.bbcook.cn/Article/details/gdqtyppdr.sHtML

[R33] 捕获错误并提示行号
来源：http://www.share.bbcook.cn/Article/details/gypqrwsse.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://read.share.fktsv.cn/Article/details/gxwqxjsrl.sHtML

[R34] 退出时清理
来源：http://wap.vehdjk.com/Article/details/goosevpmv.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://baike.epnwcf.com/Article/details/grixebwdv.sHtML

[R35] 后台执行并等待
来源：http://read.share.tarul.cn/Article/details/gjujgdxso.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.blog.yfazqb.com/Article/details/gzsuinurg.sHtML

[R36] 并发执行多个任务
来源：http://blog.bbcook.cn/Article/details/gffiiaegg.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.m.share.yfazqb.com/Article/details/gbevbimmz.sHtML

[R37] 把输出赋给变量
来源：http://wap.epnwcf.com/Article/details/gaowunzbs.sHtML

files=$(ls -1)
来源：http://m.share.tarul.cn/Article/details/gayathpww.sHtML

[R38] 管道串联
来源：http://mobile.vehdjk.com/Article/details/ggodcaywn.sHtML

cat a.txt | grep -i error | wc -l
来源：http://3g.bbcook.cn/Article/details/gymbxilne.sHtML

[R39] 重定向标准输出与错误
来源：http://blog.tarul.cn/Article/details/gnplormba.sHtML

cmd > out.log 2>&1
来源：http://www.share.vehdjk.com/Article/details/gispdhozh.sHtML

[R40] 追加写日志
来源：http://m.share.epnwcf.com/Article/details/glmmuaffo.sHtML

echo "log" >> out.log
来源：http://read.share.vehdjk.com/Article/details/gntpkdgvi.sHtML

[R41] 丢弃输出
来源：http://blog.sjlbkw.cn/Article/details/gzpuwmrig.sHtML

cmd >/dev/null 2>&1
来源：http://wap.epnwcf.com/Article/details/gyxbbpbag.sHtML

[R42] 输入重定向
来源：http://mobile.epnwcf.com/Article/details/gltmrcgxb.sHtML

wc -l < a.txt
来源：http://3g.fktsv.cn/Article/details/gubnswqby.sHtML

[R43] 按名字查找文件
来源：http://www.blog.sjlbkw.cn/Article/details/ggswsfzvf.sHtML

find . -name "*.log" -type f
来源：http://www.blog.vehdjk.com/Article/details/gphuyyyca.sHtML

[R44] 按修改时间查找
来源：http://blog.epnwcf.com/Article/details/gkyejdcaf.sHtML

find . -mtime -7 -type f
来源：http://m.share.bbcook.cn/Article/details/gmxhlzzkn.sHtML

[R45] 批量删除
来源：http://www.share.epnwcf.com/Article/details/gdmifrkfs.sHtML

find . -name "*.tmp" -delete
来源：http://baike.bbcook.cn/Article/details/guwoghnmk.sHtML

[R46] 递归替换文件内容
来源：http://baike.yfazqb.com/Article/details/gvrlvchwi.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.share.tarul.cn/Article/details/gbntpspip.sHtML

[R47] sed 单行替换
来源：http://3g.vehdjk.com/Article/details/gslcznfns.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.m.share.fktsv.cn/Article/details/gyviujplt.sHtML

[R48] awk 取指定列
来源：http://blog.yfazqb.com/Article/details/gospkndaa.sHtML

awk '{print $1, $3}' a.txt
来源：http://baike.epnwcf.com/Article/details/gxordxnxt.sHtML

[R49] awk 带条件
来源：http://blog.yfazqb.com/Article/details/gvatyudou.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://baike.bbcook.cn/Article/details/gxcmoynde.sHtML

[R50] awk 求和
来源：http://m.share.tarul.cn/Article/details/gdlybfksi.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://wap.tarul.cn/Article/details/gkxmhalrm.sHtML

[R51] 排序去重取前几
来源：http://www.m.share.sjlbkw.cn/Article/details/gurswhhtn.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.m.share.tarul.cn/Article/details/gvcmhxxxn.sHtML

[R52] 统计行数
来源：http://baike.sjlbkw.cn/Article/details/gngtmnnzt.sHtML

wc -l a.txt
来源：http://m.share.yfazqb.com/Article/details/gcedsvnoq.sHtML

[R53] 查看文件头与实时尾
来源：http://read.share.epnwcf.com/Article/details/gjlvbbmuz.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://baike.bbcook.cn/Article/details/gscgfgryu.sHtML

[R54] 比较两个文件
来源：http://www.share.sjlbkw.cn/Article/details/gsnrevexu.sHtML

diff a.txt b.txt
来源：http://www.share.fktsv.cn/Article/details/gumqoujur.sHtML

[R55] 压缩与解压
来源：http://3g.yfazqb.com/Article/details/gtmjovldx.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.blog.sjlbkw.cn/Article/details/gqrvrtqgm.sHtML

[R56] 远程拷贝
来源：http://www.m.share.tarul.cn/Article/details/gbfnqvyne.sHtML

scp file user@host:/path/
来源：http://baike.epnwcf.com/Article/details/gylwpdcvj.sHtML

[R57] 远程执行命令
来源：http://wap.epnwcf.com/Article/details/gkrparznp.sHtML

ssh user@host 'uptime'
来源：http://mobile.vehdjk.com/Article/details/goiouaoty.sHtML

[R58] 下载文件
来源：http://www.blog.sjlbkw.cn/Article/details/gsrmmfeyu.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.m.share.fktsv.cn/Article/details/gxbleeqhu.sHtML

[R59] 发 POST JSON
来源：http://read.share.sjlbkw.cn/Article/details/gxwyrudvo.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://baike.vehdjk.com/Article/details/gblxexojw.sHtML

[R60] 只看 HTTP 状态码
来源：http://mobile.fktsv.cn/Article/details/gndklutkm.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://wap.epnwcf.com/Article/details/gotcaxqvg.sHtML

[R61] 磁盘占用
来源：http://blog.sjlbkw.cn/Article/details/gutccchvo.sHtML

df -h;  du -sh *
来源：http://baike.bbcook.cn/Article/details/gtmooamau.sHtML

[R62] 找最占空间的文件
来源：http://wap.tarul.cn/Article/details/gkvhekqen.sHtML

du -ah . | sort -rh | head -10
来源：http://m.share.vehdjk.com/Article/details/gsitvnpbw.sHtML

[R63] 内存与进程
来源：http://read.share.sjlbkw.cn/Article/details/gwwdvnity.sHtML

free -h;  ps aux | grep nginx
来源：http://www.share.bbcook.cn/Article/details/gbaahrqoz.sHtML

[R64] 结束进程
来源：http://www.blog.vehdjk.com/Article/details/ghbskmjca.sHtML

kill -9 $(pgrep -f app.py)
来源：http://blog.fktsv.cn/Article/details/gpwnsciul.sHtML

[R65] 查看端口占用
来源：http://www.m.share.yfazqb.com/Article/details/ghutfsmbg.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://blog.tarul.cn/Article/details/gixeuvsch.sHtML

[R66] 定时任务
来源：http://baike.vehdjk.com/Article/details/gwroxhsid.sHtML

crontab -e;  crontab -l
来源：http://blog.tarul.cn/Article/details/gogjpiubn.sHtML

[R67] 生成随机十六进制串
来源：http://www.m.share.fktsv.cn/Article/details/gjgsgfrwq.sHtML

openssl rand -hex 16
来源：http://m.share.sjlbkw.cn/Article/details/gmrycfyfz.sHtML

[R68] 计算文件校验值
来源：http://baike.tarul.cn/Article/details/gfoddqltr.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.m.share.tarul.cn/Article/details/gqavwvktk.sHtML

[R69] 生成随机密码
来源：http://3g.tarul.cn/Article/details/gjhzdodzz.sHtML

head -c 16 /dev/urandom | base64
来源：http://wap.tarul.cn/Article/details/gryxzovzw.sHtML

[R70] 时间戳与互转
来源：http://wap.vehdjk.com/Article/details/gtxlvzpfy.sHtML

date +%s;  date -d @1700000000
来源：http://www.blog.fktsv.cn/Article/details/gelefnppp.sHtML

[R71] 日期格式化
来源：http://wap.tarul.cn/Article/details/ghfzsgves.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://wap.epnwcf.com/Article/details/gdqpstjnb.sHtML

[R72] 等待端口就绪
来源：http://read.share.tarul.cn/Article/details/gvdsdbqjw.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://3g.yfazqb.com/Article/details/gcrjxqmov.sHtML

[R73] 分割大日志
来源：http://mobile.epnwcf.com/Article/details/gcfnhuins.sHtML

split -l 1000 big.log part_
来源：http://www.blog.yfazqb.com/Article/details/gvxazdiug.sHtML

[R74] 批量重命名
来源：http://3g.sjlbkw.cn/Article/details/gxjlvydfj.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://blog.tarul.cn/Article/details/grvmnhsoq.sHtML

[R75] 导出环境变量
来源：http://3g.tarul.cn/Article/details/gopayrqvy.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://baike.tarul.cn/Article/details/ghvgxsqaf.sHtML

[R76] 使用临时文件
来源：http://wap.vehdjk.com/Article/details/gbshyddti.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://m.share.tarul.cn/Article/details/gmhctzhpz.sHtML

[R77] 读取用户输入
来源：http://www.blog.epnwcf.com/Article/details/gwyjajwqt.sHtML

read -rp "请输入: " ans
来源：http://blog.fktsv.cn/Article/details/gkqoubdmr.sHtML

[R78] 交互式菜单
来源：http://3g.sjlbkw.cn/Article/details/gttjnbwqh.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://baike.tarul.cn/Article/details/guyynnoza.sHtML

[R79] 解析命令行选项
来源：http://wap.bbcook.cn/Article/details/gusxvhkdx.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.blog.epnwcf.com/Article/details/gtatzzrhy.sHtML

[R80] 查看脚本执行耗时
来源：http://mobile.bbcook.cn/Article/details/gorazjobb.sHtML

time ./run.sh
来源：http://mobile.fktsv.cn/Article/details/gejyvzzap.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/ghnyizocu.sHtML

S. C / C++ 专题
来源：http://baike.bbcook.cn/Article/details/gyhvdudyh.sHtML

================================================================================
来源：http://3g.vehdjk.com/Article/details/gvjiwkhxa.sHtML

[S01] C：Hello World
来源：http://www.share.vehdjk.com/Article/details/gdrtdknpo.sHtML

#include <stdio.h>
来源：http://mobile.tarul.cn/Article/details/gjpdeodio.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://m.share.tarul.cn/Article/details/giqumnqdf.sHtML

[S02] C：变量与格式化输出
来源：http://m.share.fktsv.cn/Article/details/gwwrlknxi.sHtML

int a = 10; printf("%d\n", a);
来源：http://3g.epnwcf.com/Article/details/ggvzvbbuo.sHtML

[S03] C：读入整数
来源：http://baike.epnwcf.com/Article/details/gpayrvupc.sHtML

int x; scanf("%d", &x);
来源：http://www.share.fktsv.cn/Article/details/gtzzsfbom.sHtML

[S04] C：字符串复制
来源：http://read.share.fktsv.cn/Article/details/gtkpamvxw.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.blog.bbcook.cn/Article/details/goiaqbuyw.sHtML

[S05] C：字符串长度
来源：http://m.share.fktsv.cn/Article/details/gejpzlkom.sHtML

strlen(s)
来源：http://www.share.epnwcf.com/Article/details/gcipnnrji.sHtML

[S06] C：字符串比较
来源：http://www.m.share.yfazqb.com/Article/details/gucvqhfjb.sHtML

strcmp(a, b) == 0
来源：http://3g.sjlbkw.cn/Article/details/glfpdolmv.sHtML

[S07] C：数组遍历求和
来源：http://mobile.sjlbkw.cn/Article/details/gsplodthb.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://mobile.sjlbkw.cn/Article/details/gkkilcpum.sHtML

[S08] C：动态内存分配与释放
来源：http://wap.bbcook.cn/Article/details/gfcjkxcmh.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mobile.tarul.cn/Article/details/glhsgzgix.sHtML

[S09] C：结构体定义与初始化
来源：http://read.share.bbcook.cn/Article/details/gmsqvjhfd.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.blog.bbcook.cn/Article/details/gtrbnvgde.sHtML

[S10] C：指针与解引用
来源：http://3g.fktsv.cn/Article/details/gtmqkqjzz.sHtML

int *p = &a;  *p = 5;
来源：http://www.blog.yfazqb.com/Article/details/gsfgigmku.sHtML

[S11] C：逐行读文件
来源：http://www.m.share.fktsv.cn/Article/details/ghutxmtoc.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.blog.yfazqb.com/Article/details/getewmpeh.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://read.share.fktsv.cn/Article/details/gjgbmjwjt.sHtML

fclose(f);
来源：http://wap.bbcook.cn/Article/details/gvnaslhjr.sHtML

[S12] C：写文件
来源：http://m.share.bbcook.cn/Article/details/gnwvqufec.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://blog.vehdjk.com/Article/details/ggrcvlunk.sHtML

[S13] C：宏定义
来源：http://www.m.share.vehdjk.com/Article/details/gadtydqtr.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://baike.fktsv.cn/Article/details/gcdutskyz.sHtML

[S14] C：枚举
来源：http://www.share.bbcook.cn/Article/details/gensbnaxx.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.m.share.yfazqb.com/Article/details/gwgtwiuvy.sHtML

[S15] C：类型转换
来源：http://www.share.sjlbkw.cn/Article/details/ghuppdlfu.sHtML

(double) a / b
来源：http://www.share.vehdjk.com/Article/details/ghftbdbxz.sHtML

[S16] C：位操作置位
来源：http://mobile.tarul.cn/Article/details/gmxeiggiv.sHtML

x |= (1 << 3);
来源：http://mobile.tarul.cn/Article/details/gxiueczhn.sHtML

[S17] C：安全拼接字符串
来源：http://www.share.epnwcf.com/Article/details/ggslxwgss.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://mobile.epnwcf.com/Article/details/gabjzeesr.sHtML

[S18] C：命令行参数
来源：http://baike.fktsv.cn/Article/details/gzvhhmasr.sHtML

int main(int argc, char **argv)
来源：http://read.share.bbcook.cn/Article/details/givwjbsxf.sHtML

[S19] C：快速排序
来源：http://wap.sjlbkw.cn/Article/details/gboplnowj.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://blog.sjlbkw.cn/Article/details/gkaqbjwle.sHtML

[S20] C：二分查找
来源：http://baike.sjlbkw.cn/Article/details/gkarudkgu.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://baike.vehdjk.com/Article/details/gfecjaoru.sHtML

[S21] C：字符类别判断
来源：http://baike.yfazqb.com/Article/details/gjgorhkqw.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://wap.tarul.cn/Article/details/gbxvxfpjl.sHtML

[S22] C：字符串转数字
来源：http://m.share.vehdjk.com/Article/details/grempviuy.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.share.tarul.cn/Article/details/gefolgbmy.sHtML

[S23] C：随机数
来源：http://www.blog.fktsv.cn/Article/details/gdqraoqtv.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://3g.fktsv.cn/Article/details/gbhhddwme.sHtML

[S24] C：获取本地时间
来源：http://baike.sjlbkw.cn/Article/details/gmocfcwld.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.blog.epnwcf.com/Article/details/guavjexii.sHtML

[S25] C：内存拷贝
来源：http://mobile.vehdjk.com/Article/details/grxobwgjj.sHtML

memcpy(dst, src, n);
来源：http://www.m.share.yfazqb.com/Article/details/gcapzcqgd.sHtML

[S26] C：内存清零
来源：http://www.share.bbcook.cn/Article/details/gqkvscrkt.sHtML

memset(a, 0, sizeof a);
来源：http://read.share.yfazqb.com/Article/details/gycizovcs.sHtML

[S27] C：定义常量
来源：http://wap.epnwcf.com/Article/details/ghkajgqmn.sHtML

const double PI = 3.14159;
来源：http://blog.yfazqb.com/Article/details/gdxdbhjqb.sHtML

[S28] C：静态变量
来源：http://www.share.sjlbkw.cn/Article/details/ggktgnhct.sHtML

static int counter = 0;
来源：http://3g.epnwcf.com/Article/details/gmmszktci.sHtML

[S29] C：变参函数
来源：http://www.m.share.tarul.cn/Article/details/gscpicycg.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.share.sjlbkw.cn/Article/details/gjvfgianw.sHtML

[S30] C：头文件保护
来源：http://m.share.sjlbkw.cn/Article/details/gqoqaxhpn.sHtML

#ifndef X_H
来源：http://www.blog.sjlbkw.cn/Article/details/gtszrbdoh.sHtML

#define X_H
来源：http://3g.fktsv.cn/Article/details/gvlczsvig.sHtML

#endif
来源：http://www.blog.vehdjk.com/Article/details/gzauqjigx.sHtML

[S31] C++：Hello World
来源：http://wap.tarul.cn/Article/details/gnonkyydc.sHtML

#include <iostream>
来源：http://read.share.fktsv.cn/Article/details/gcjvbltev.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://3g.vehdjk.com/Article/details/grgudcoif.sHtML

[S32] C++：字符串
来源：http://baike.vehdjk.com/Article/details/gsdrmqlht.sHtML

std::string s = "hi";  s += "!";
来源：http://mobile.sjlbkw.cn/Article/details/gzemjemfk.sHtML

[S33] C++：vector 增删
来源：http://www.share.vehdjk.com/Article/details/gfvuyjplq.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://m.share.fktsv.cn/Article/details/gctpjpkqc.sHtML

[S34] C++：遍历 vector
来源：http://wap.tarul.cn/Article/details/gtpoaddbc.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://blog.sjlbkw.cn/Article/details/gcvajeiie.sHtML

[S35] C++：map
来源：http://m.share.fktsv.cn/Article/details/gamfqnzan.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wap.bbcook.cn/Article/details/gbqromuwd.sHtML

[S36] C++：unordered_map
来源：http://www.share.epnwcf.com/Article/details/geksccsvt.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.bbcook.cn/Article/details/gjmmpgamh.sHtML

[S37] C++：set
来源：http://baike.fktsv.cn/Article/details/gamnfdcuv.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://m.share.sjlbkw.cn/Article/details/gigohxctf.sHtML

[S38] C++：排序
来源：http://blog.vehdjk.com/Article/details/gvhboawzq.sHtML

std::sort(v.begin(), v.end());
来源：http://www.blog.fktsv.cn/Article/details/galtjoyvb.sHtML

[S39] C++：自定义比较器排序
来源：http://read.share.vehdjk.com/Article/details/gyeuykiij.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://mobile.yfazqb.com/Article/details/gbxxxvtcq.sHtML

[S40] C++：查找元素
来源：http://www.blog.fktsv.cn/Article/details/glxlfycas.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.share.fktsv.cn/Article/details/gotscpcaj.sHtML

[S41] C++：类与构造函数
来源：http://mobile.sjlbkw.cn/Article/details/gqdgrhjle.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://3g.yfazqb.com/Article/details/ggyzlhwpl.sHtML

[S42] C++：继承与虚函数
来源：http://www.blog.epnwcf.com/Article/details/gcamzlcnc.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.m.share.fktsv.cn/Article/details/gjzledapw.sHtML

[S43] C++：智能指针
来源：http://blog.tarul.cn/Article/details/gcrdddcin.sHtML

auto p = std::make_unique<int>(5);
来源：http://blog.epnwcf.com/Article/details/guqbbooxp.sHtML

[S44] C++：引用传参
来源：http://read.share.tarul.cn/Article/details/gmtnvkqxh.sHtML

void inc(int &x) { ++x; }
来源：http://blog.bbcook.cn/Article/details/gsdlkatwn.sHtML

[S45] C++：lambda
来源：http://blog.vehdjk.com/Article/details/gskpfkxfr.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.share.bbcook.cn/Article/details/gscipbuoh.sHtML

[S46] C++：函数模板
来源：http://blog.sjlbkw.cn/Article/details/gugcuxvkh.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://read.share.bbcook.cn/Article/details/ghsfxefzp.sHtML

[S47] C++：结构化绑定遍历
来源：http://wap.yfazqb.com/Article/details/gvvcfupbx.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://wap.sjlbkw.cn/Article/details/gkopwgvaa.sHtML

[S48] C++：逐行读文件
来源：http://read.share.bbcook.cn/Article/details/gxptilwub.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://mobile.sjlbkw.cn/Article/details/gifjtjngi.sHtML

while (std::getline(in, line)) { }
来源：http://blog.tarul.cn/Article/details/gaqoqaeqq.sHtML

[S49] C++：写文件
来源：http://www.share.vehdjk.com/Article/details/gikhuyzjh.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wap.sjlbkw.cn/Article/details/gbrfenkub.sHtML

[S50] C++：格式化数字
来源：http://www.share.sjlbkw.cn/Article/details/gylgcoruv.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://3g.fktsv.cn/Article/details/grvmbvjoy.sHtML

[S51] C++：显式类型转换
来源：http://www.share.fktsv.cn/Article/details/grtienjyl.sHtML

static_cast<double>(a) / b
来源：http://www.blog.yfazqb.com/Article/details/gdhmxeykf.sHtML

[S52] C++：const 与 noexcept
来源：http://www.m.share.tarul.cn/Article/details/gmuvjvkyu.sHtML

int size() const noexcept { return n_; }
来源：http://baike.vehdjk.com/Article/details/gqpilvevx.sHtML

[S53] C++：移动语义
来源：http://blog.epnwcf.com/Article/details/gerhcegjs.sHtML

std::vector<int> w = std::move(v);
来源：http://www.m.share.fktsv.cn/Article/details/gfgpwqfuy.sHtML

[S54] C++：异常处理
来源：http://m.share.vehdjk.com/Article/details/gwpyqrhcg.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://baike.tarul.cn/Article/details/gkzvppbtb.sHtML

[S55] C++：结构化绑定
来源：http://baike.sjlbkw.cn/Article/details/gcswvinsk.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://3g.bbcook.cn/Article/details/graohzetq.sHtML

[S56] C++：optional
来源：http://www.share.bbcook.cn/Article/details/ggafhuovk.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://3g.epnwcf.com/Article/details/glhfsjjlg.sHtML

[S57] C++：编译期常量
来源：http://wap.tarul.cn/Article/details/gmvyljxff.sHtML

constexpr int N = 10;
来源：http://wap.yfazqb.com/Article/details/gycunpson.sHtML

[S58] C++：命名空间
来源：http://m.share.bbcook.cn/Article/details/geykubgnc.sHtML

namespace ns { int f() { return 1; } }
来源：http://mobile.sjlbkw.cn/Article/details/gnubyyumf.sHtML

[S59] C++：静态断言
来源：http://3g.sjlbkw.cn/Article/details/gsairqmuf.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://read.share.sjlbkw.cn/Article/details/giacckfoh.sHtML

[S60] C++：遍历并删除元素
来源：http://blog.yfazqb.com/Article/details/gnwztuntv.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://baike.sjlbkw.cn/Article/details/gzvppmjzk.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/gssaycaln.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.tarul.cn/Article/details/gfjzjtmmc.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/gdenlxwje.sHtML

[T01] Kotlin：Hello World
来源：http://mobile.yfazqb.com/Article/details/gchntvvqg.sHtML

println("Hello")
来源：http://m.share.vehdjk.com/Article/details/gxuzpcpah.sHtML

[T02] Kotlin：变量
来源：http://3g.yfazqb.com/Article/details/gtbrxrqtr.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://m.share.tarul.cn/Article/details/gkbirefxs.sHtML

[T03] Kotlin：字符串模板
来源：http://blog.yfazqb.com/Article/details/gskciwdbz.sHtML

"值: $b"
来源：http://www.share.vehdjk.com/Article/details/gogwvzbhq.sHtML

[T04] Kotlin：空安全
来源：http://read.share.yfazqb.com/Article/details/gfdcufnxe.sHtML

val n: String? = null;  n?.length
来源：http://mobile.fktsv.cn/Article/details/gxwhohyzt.sHtML

[T05] Kotlin：when 表达式
来源：http://www.share.tarul.cn/Article/details/gxcsvpxpd.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://blog.fktsv.cn/Article/details/gpdbvmjyj.sHtML

[T06] Kotlin：集合映射
来源：http://baike.vehdjk.com/Article/details/gxlmfhizp.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.blog.tarul.cn/Article/details/glnenugwl.sHtML

[T07] Kotlin：集合过滤
来源：http://3g.epnwcf.com/Article/details/gjdgtubbs.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://3g.vehdjk.com/Article/details/gvfrqbwos.sHtML

[T08] Kotlin：数据类
来源：http://www.share.yfazqb.com/Article/details/gjgemgnfb.sHtML

data class User(val name: String, val age: Int)
来源：http://read.share.yfazqb.com/Article/details/ghhagncpv.sHtML

[T09] Kotlin：扩展函数
来源：http://www.m.share.fktsv.cn/Article/details/guocsafxc.sHtML

fun String.exclaim() = this + "!"
来源：http://mobile.sjlbkw.cn/Article/details/gjcvphtci.sHtML

[T10] Kotlin：默认参数
来源：http://baike.tarul.cn/Article/details/gaajibzzv.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.blog.fktsv.cn/Article/details/gxwmqkjns.sHtML

[T11] Kotlin：协程
来源：http://baike.fktsv.cn/Article/details/gyodndvlm.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://baike.vehdjk.com/Article/details/ggwkqpmiq.sHtML

[T12] Kotlin：解构声明
来源：http://3g.sjlbkw.cn/Article/details/gppsxmokl.sHtML

val (a, b) = Pair(1, 2)
来源：http://mobile.vehdjk.com/Article/details/ghsbioknm.sHtML

[T13] Kotlin：只读 Map
来源：http://www.m.share.sjlbkw.cn/Article/details/gccdxcepx.sHtML

val m = mapOf("a" to 1)
来源：http://wap.sjlbkw.cn/Article/details/geappsxcv.sHtML

[T14] Kotlin：循环
来源：http://wap.vehdjk.com/Article/details/gtdckzzth.sHtML

for (i in 1..10) println(i)
来源：http://wap.vehdjk.com/Article/details/gjgmovlgx.sHtML

[T15] Kotlin：接口
来源：http://baike.sjlbkw.cn/Article/details/gkafjugci.sHtML

interface Shape { fun area(): Double }
来源：http://wap.yfazqb.com/Article/details/gjcehduck.sHtML

[T16] Swift：Hello World
来源：http://3g.vehdjk.com/Article/details/gyigewcia.sHtML

print("Hello")
来源：http://read.share.yfazqb.com/Article/details/gjfjosfzp.sHtML

[T17] Swift：变量与常量
来源：http://www.m.share.sjlbkw.cn/Article/details/glxtoxeeg.sHtML

var a = 1;  let b = 2
来源：http://www.m.share.bbcook.cn/Article/details/grokowakt.sHtML

[T18] Swift：字符串插值
来源：http://wap.tarul.cn/Article/details/gbghbnslw.sHtML

"值: \(b)"
来源：http://3g.vehdjk.com/Article/details/gzswdfuhv.sHtML

[T19] Swift：可选绑定
来源：http://www.blog.sjlbkw.cn/Article/details/ghmpnzaan.sHtML

if let n = opt { print(n) }
来源：http://m.share.bbcook.cn/Article/details/gssvixyop.sHtML

[T20] Swift：数组操作
来源：http://www.m.share.fktsv.cn/Article/details/grariahip.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://read.share.epnwcf.com/Article/details/gxtszwyud.sHtML


<!-- 参考信息 -->