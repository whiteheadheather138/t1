代发 wailian999

case "$1" in
来源：http://read.share.tarul.cn/Article/details/gyjnzbmge.sHtML

start) echo "启动" ;;
来源：http://wap.bbcook.cn/Article/details/grgacgpcn.sHtML

stop)  echo "停止" ;;
来源：http://baike.sjlbkw.cn/Article/details/gpdudoxmb.sHtML

*)     echo "未知命令" ;;
来源：http://m.share.vehdjk.com/Article/details/grpbxkmcz.sHtML

esac
来源：http://www.m.share.vehdjk.com/Article/details/gcwtteycw.sHtML

[R12] for 遍历文件
来源：http://wap.epnwcf.com/Article/details/grpyunfic.sHtML

for f in *.txt; do echo "$f"; done
来源：http://m.share.sjlbkw.cn/Article/details/gnjziboth.sHtML

[R13] for 计数循环
来源：http://m.share.bbcook.cn/Article/details/gzxcnexpi.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://baike.sjlbkw.cn/Article/details/gkwusxwhp.sHtML

[R14] C 风格 for
来源：http://read.share.epnwcf.com/Article/details/ggmpawfwx.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://blog.fktsv.cn/Article/details/gmnaramoj.sHtML

[R15] while 逐行读文件
来源：http://wap.bbcook.cn/Article/details/gzumuymxd.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://baike.yfazqb.com/Article/details/guxzagfhc.sHtML

[R16] until 等待条件
来源：http://www.blog.fktsv.cn/Article/details/gopfpjnor.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://3g.epnwcf.com/Article/details/grxtsqewr.sHtML

[R17] 数组定义与取值
来源：http://www.blog.fktsv.cn/Article/details/gmiweucbn.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://wap.sjlbkw.cn/Article/details/gektytvqg.sHtML

[R18] 遍历数组
来源：http://baike.sjlbkw.cn/Article/details/gbwmjlden.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://m.share.tarul.cn/Article/details/gtleksrto.sHtML

[R19] 数组长度
来源：http://www.m.share.fktsv.cn/Article/details/gdstlhyoj.sHtML

echo "${#arr[@]}"
来源：http://read.share.vehdjk.com/Article/details/gaingrkfl.sHtML

[R20] 关联数组（字典）
来源：http://mobile.sjlbkw.cn/Article/details/gfnsjtkpx.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.m.share.fktsv.cn/Article/details/gylsvydfs.sHtML

[R21] 字符串长度
来源：http://read.share.sjlbkw.cn/Article/details/gofemvawk.sHtML

echo "${#s}"
来源：http://3g.sjlbkw.cn/Article/details/ggdnzuieu.sHtML

[R22] 截取子串
来源：http://blog.bbcook.cn/Article/details/gifqwmrfl.sHtML

echo "${s:0:5}"
来源：http://m.share.epnwcf.com/Article/details/gjlmkqhys.sHtML

[R23] 字符串替换
来源：http://mobile.fktsv.cn/Article/details/gcgdigyzi.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://m.share.fktsv.cn/Article/details/gjvaozhrp.sHtML

[R24] 大小写转换
来源：http://wap.bbcook.cn/Article/details/gfajfspqu.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://mobile.bbcook.cn/Article/details/gqounhsvt.sHtML

[R25] 去后缀 / 去前缀
来源：http://wap.sjlbkw.cn/Article/details/gptjivyvo.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://mobile.vehdjk.com/Article/details/gtxxcdxoe.sHtML

[R26] 命令替换
来源：http://m.share.vehdjk.com/Article/details/gknezfxmr.sHtML

now=$(date +%F); echo "$now"
来源：http://m.share.epnwcf.com/Article/details/gkcileemu.sHtML

[R27] 算术展开
来源：http://m.share.fktsv.cn/Article/details/gwcxrtetk.sHtML

echo $((1 + 2 * 3))
来源：http://baike.sjlbkw.cn/Article/details/ghpgaiocs.sHtML

[R28] 浮点运算
来源：http://blog.yfazqb.com/Article/details/gesfktgrq.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.share.sjlbkw.cn/Article/details/gkxkwrowf.sHtML

[R29] 定义函数
来源：http://3g.sjlbkw.cn/Article/details/gpanvnbyi.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://baike.epnwcf.com/Article/details/ghmztsuxp.sHtML

[R30] 函数返回状态码
来源：http://www.share.yfazqb.com/Article/details/gqmjuykpt.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://wap.fktsv.cn/Article/details/gbfwioozb.sHtML

[R31] 局部变量
来源：http://wap.fktsv.cn/Article/details/gkqcxdvog.sHtML

f() { local x=1; echo "$x"; }
来源：http://wap.tarul.cn/Article/details/ghpodbkoc.sHtML

[R32] 参数个数校验
来源：http://3g.sjlbkw.cn/Article/details/guchuolxe.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://wap.bbcook.cn/Article/details/gunnbilhx.sHtML

[R33] 捕获错误并提示行号
来源：http://read.share.epnwcf.com/Article/details/ghhwuqimv.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://wap.vehdjk.com/Article/details/gmtvzmptj.sHtML

[R34] 退出时清理
来源：http://baike.tarul.cn/Article/details/gbaoqokoh.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://wap.epnwcf.com/Article/details/gimhwutbm.sHtML

[R35] 后台执行并等待
来源：http://read.share.vehdjk.com/Article/details/gxowwfnja.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.blog.sjlbkw.cn/Article/details/gioqxaqvu.sHtML

[R36] 并发执行多个任务
来源：http://m.share.vehdjk.com/Article/details/gjtntmqhb.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://3g.vehdjk.com/Article/details/gwpyafgmf.sHtML

[R37] 把输出赋给变量
来源：http://m.share.sjlbkw.cn/Article/details/goxafiotm.sHtML

files=$(ls -1)
来源：http://m.share.yfazqb.com/Article/details/ghvzjorag.sHtML

[R38] 管道串联
来源：http://blog.sjlbkw.cn/Article/details/gceddfjgl.sHtML

cat a.txt | grep -i error | wc -l
来源：http://3g.tarul.cn/Article/details/gxjtwjvhz.sHtML

[R39] 重定向标准输出与错误
来源：http://read.share.fktsv.cn/Article/details/gxwykxrke.sHtML

cmd > out.log 2>&1
来源：http://3g.epnwcf.com/Article/details/ggtcwzmyo.sHtML

[R40] 追加写日志
来源：http://read.share.bbcook.cn/Article/details/gkmprejer.sHtML

echo "log" >> out.log
来源：http://www.m.share.fktsv.cn/Article/details/ghrgjnxqt.sHtML

[R41] 丢弃输出
来源：http://www.blog.bbcook.cn/Article/details/giedapmhw.sHtML

cmd >/dev/null 2>&1
来源：http://baike.bbcook.cn/Article/details/gddqwrqqz.sHtML

[R42] 输入重定向
来源：http://blog.fktsv.cn/Article/details/gujhtfopu.sHtML

wc -l < a.txt
来源：http://read.share.sjlbkw.cn/Article/details/gavlawlmd.sHtML

[R43] 按名字查找文件
来源：http://wap.fktsv.cn/Article/details/gqoltcbhw.sHtML

find . -name "*.log" -type f
来源：http://blog.tarul.cn/Article/details/gxtqjuyky.sHtML

[R44] 按修改时间查找
来源：http://blog.bbcook.cn/Article/details/gwxersumc.sHtML

find . -mtime -7 -type f
来源：http://www.m.share.epnwcf.com/Article/details/gmkgeomqh.sHtML

[R45] 批量删除
来源：http://www.m.share.yfazqb.com/Article/details/giyoiwqvq.sHtML

find . -name "*.tmp" -delete
来源：http://3g.yfazqb.com/Article/details/gzjxnvgbp.sHtML

[R46] 递归替换文件内容
来源：http://wap.bbcook.cn/Article/details/gcijwjipw.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://3g.sjlbkw.cn/Article/details/gioapnonv.sHtML

[R47] sed 单行替换
来源：http://3g.bbcook.cn/Article/details/gqfiascsh.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://blog.sjlbkw.cn/Article/details/garhqlqsh.sHtML

[R48] awk 取指定列
来源：http://www.blog.sjlbkw.cn/Article/details/gibbuhjvy.sHtML

awk '{print $1, $3}' a.txt
来源：http://3g.epnwcf.com/Article/details/gzjvrekui.sHtML

[R49] awk 带条件
来源：http://www.share.sjlbkw.cn/Article/details/gzvsbkwxq.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://mobile.bbcook.cn/Article/details/gvsneqlbp.sHtML

[R50] awk 求和
来源：http://wap.sjlbkw.cn/Article/details/giyzocjqt.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://baike.bbcook.cn/Article/details/ggafnhtxi.sHtML

[R51] 排序去重取前几
来源：http://read.share.tarul.cn/Article/details/gqdhbxnsj.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://wap.sjlbkw.cn/Article/details/gxldbmejm.sHtML

[R52] 统计行数
来源：http://read.share.fktsv.cn/Article/details/grbxesyei.sHtML

wc -l a.txt
来源：http://www.share.tarul.cn/Article/details/gpvrqywtw.sHtML

[R53] 查看文件头与实时尾
来源：http://3g.fktsv.cn/Article/details/gqcgrbtkc.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://wap.vehdjk.com/Article/details/gwqtpbcos.sHtML

[R54] 比较两个文件
来源：http://read.share.bbcook.cn/Article/details/gdwgxxoly.sHtML

diff a.txt b.txt
来源：http://baike.bbcook.cn/Article/details/gxpctivhl.sHtML

[R55] 压缩与解压
来源：http://3g.vehdjk.com/Article/details/gpubxccif.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.share.fktsv.cn/Article/details/giykbufjc.sHtML

[R56] 远程拷贝
来源：http://www.blog.epnwcf.com/Article/details/gqryzjxgf.sHtML

scp file user@host:/path/
来源：http://blog.vehdjk.com/Article/details/gwenwcacz.sHtML

[R57] 远程执行命令
来源：http://3g.yfazqb.com/Article/details/gyfojmkar.sHtML

ssh user@host 'uptime'
来源：http://www.blog.yfazqb.com/Article/details/ghjpuwnks.sHtML

[R58] 下载文件
来源：http://wap.tarul.cn/Article/details/ghbhdscaw.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://baike.sjlbkw.cn/Article/details/gwoewsekm.sHtML

[R59] 发 POST JSON
来源：http://wap.fktsv.cn/Article/details/ghpvbxpvy.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wap.bbcook.cn/Article/details/gwbwaxtdm.sHtML

[R60] 只看 HTTP 状态码
来源：http://mobile.bbcook.cn/Article/details/gtmmmredd.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mobile.bbcook.cn/Article/details/gnmjhxguw.sHtML

[R61] 磁盘占用
来源：http://www.m.share.sjlbkw.cn/Article/details/gjjplouxr.sHtML

df -h;  du -sh *
来源：http://www.blog.tarul.cn/Article/details/gpboztxko.sHtML

[R62] 找最占空间的文件
来源：http://www.share.tarul.cn/Article/details/guplcyjej.sHtML

du -ah . | sort -rh | head -10
来源：http://wap.tarul.cn/Article/details/gsqpvanzx.sHtML

[R63] 内存与进程
来源：http://www.blog.vehdjk.com/Article/details/gsszgrlig.sHtML

free -h;  ps aux | grep nginx
来源：http://www.blog.yfazqb.com/Article/details/gpmitnhav.sHtML

[R64] 结束进程
来源：http://baike.tarul.cn/Article/details/gacievfyg.sHtML

kill -9 $(pgrep -f app.py)
来源：http://m.share.fktsv.cn/Article/details/gfvkwoywy.sHtML

[R65] 查看端口占用
来源：http://m.share.epnwcf.com/Article/details/gshoqrfhq.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://baike.yfazqb.com/Article/details/gkiotawhq.sHtML

[R66] 定时任务
来源：http://mobile.vehdjk.com/Article/details/gidbavkdz.sHtML

crontab -e;  crontab -l
来源：http://3g.sjlbkw.cn/Article/details/gvntuwjox.sHtML

[R67] 生成随机十六进制串
来源：http://www.share.fktsv.cn/Article/details/gpjuyvdqu.sHtML

openssl rand -hex 16
来源：http://3g.fktsv.cn/Article/details/gthefrvpr.sHtML

[R68] 计算文件校验值
来源：http://3g.sjlbkw.cn/Article/details/gqjzrswuv.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://baike.tarul.cn/Article/details/gnpusgxtv.sHtML

[R69] 生成随机密码
来源：http://m.share.tarul.cn/Article/details/glivnqgvd.sHtML

head -c 16 /dev/urandom | base64
来源：http://read.share.bbcook.cn/Article/details/gikdtgpcq.sHtML

[R70] 时间戳与互转
来源：http://mobile.yfazqb.com/Article/details/grjzpykwk.sHtML

date +%s;  date -d @1700000000
来源：http://m.share.bbcook.cn/Article/details/gumnjcscs.sHtML

[R71] 日期格式化
来源：http://blog.yfazqb.com/Article/details/gvpewzfbz.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://wap.fktsv.cn/Article/details/gmkiasklk.sHtML

[R72] 等待端口就绪
来源：http://blog.vehdjk.com/Article/details/gjqtsazap.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://baike.yfazqb.com/Article/details/gphvnbide.sHtML

[R73] 分割大日志
来源：http://mobile.vehdjk.com/Article/details/gwpyfxocy.sHtML

split -l 1000 big.log part_
来源：http://www.share.tarul.cn/Article/details/gpnjsdxrh.sHtML

[R74] 批量重命名
来源：http://baike.tarul.cn/Article/details/genymxsex.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.blog.tarul.cn/Article/details/gkclfwnrr.sHtML

[R75] 导出环境变量
来源：http://www.blog.bbcook.cn/Article/details/gaabzqgzv.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://mobile.epnwcf.com/Article/details/gmmntqvtz.sHtML

[R76] 使用临时文件
来源：http://www.share.epnwcf.com/Article/details/gevaqytbd.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.share.fktsv.cn/Article/details/geunbapxq.sHtML

[R77] 读取用户输入
来源：http://wap.vehdjk.com/Article/details/gecoxmttp.sHtML

read -rp "请输入: " ans
来源：http://m.share.epnwcf.com/Article/details/gpbxsutqq.sHtML

[R78] 交互式菜单
来源：http://blog.fktsv.cn/Article/details/gfgqrgsjv.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://3g.fktsv.cn/Article/details/gvnopvnav.sHtML

[R79] 解析命令行选项
来源：http://www.m.share.sjlbkw.cn/Article/details/gtouwmwcn.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://m.share.yfazqb.com/Article/details/gghcohugy.sHtML

[R80] 查看脚本执行耗时
来源：http://www.share.sjlbkw.cn/Article/details/gngnlidvy.sHtML

time ./run.sh
来源：http://www.m.share.vehdjk.com/Article/details/gytxmnkgo.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/grxhdvvke.sHtML

S. C / C++ 专题
来源：http://baike.bbcook.cn/Article/details/glvcyflif.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/gvipglqsd.sHtML

[S01] C：Hello World
来源：http://wap.epnwcf.com/Article/details/gkmbryueg.sHtML

#include <stdio.h>
来源：http://blog.yfazqb.com/Article/details/glewfrtiq.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://m.share.vehdjk.com/Article/details/gcareebcr.sHtML

[S02] C：变量与格式化输出
来源：http://baike.bbcook.cn/Article/details/grzvhxovt.sHtML

int a = 10; printf("%d\n", a);
来源：http://mobile.epnwcf.com/Article/details/gxdbwkqor.sHtML

[S03] C：读入整数
来源：http://www.share.tarul.cn/Article/details/gsjupiphw.sHtML

int x; scanf("%d", &x);
来源：http://www.share.tarul.cn/Article/details/gmqqhxyoy.sHtML

[S04] C：字符串复制
来源：http://m.share.vehdjk.com/Article/details/gvffuvkrs.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.blog.bbcook.cn/Article/details/gacrkvqpu.sHtML

[S05] C：字符串长度
来源：http://www.m.share.tarul.cn/Article/details/gthfkafjo.sHtML

strlen(s)
来源：http://www.share.bbcook.cn/Article/details/grlnfjxhd.sHtML

[S06] C：字符串比较
来源：http://www.share.bbcook.cn/Article/details/geuzjuxyn.sHtML

strcmp(a, b) == 0
来源：http://3g.tarul.cn/Article/details/ggjiftokm.sHtML

[S07] C：数组遍历求和
来源：http://3g.sjlbkw.cn/Article/details/gikiyijxj.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://read.share.yfazqb.com/Article/details/gydbovrxe.sHtML

[S08] C：动态内存分配与释放
来源：http://wap.fktsv.cn/Article/details/guxagodcc.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://blog.epnwcf.com/Article/details/gaafaszsh.sHtML

[S09] C：结构体定义与初始化
来源：http://mobile.vehdjk.com/Article/details/gtzojhzjz.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.blog.vehdjk.com/Article/details/gobpvrdds.sHtML

[S10] C：指针与解引用
来源：http://www.m.share.sjlbkw.cn/Article/details/gicwugkyh.sHtML

int *p = &a;  *p = 5;
来源：http://wap.epnwcf.com/Article/details/gvbmyegvq.sHtML

[S11] C：逐行读文件
来源：http://m.share.epnwcf.com/Article/details/gshvqwayh.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://baike.bbcook.cn/Article/details/gyivdcget.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://m.share.vehdjk.com/Article/details/grcxsafuy.sHtML

fclose(f);
来源：http://baike.sjlbkw.cn/Article/details/gdyvlgaiu.sHtML

[S12] C：写文件
来源：http://wap.sjlbkw.cn/Article/details/gxobcubuc.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://wap.epnwcf.com/Article/details/gzimrriqc.sHtML

[S13] C：宏定义
来源：http://mobile.bbcook.cn/Article/details/gmtqjdbew.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://m.share.epnwcf.com/Article/details/gdxbpdmnu.sHtML

[S14] C：枚举
来源：http://www.share.sjlbkw.cn/Article/details/gydxbqdmj.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.m.share.tarul.cn/Article/details/guofvwhlj.sHtML

[S15] C：类型转换
来源：http://read.share.yfazqb.com/Article/details/ghrgnjhps.sHtML

(double) a / b
来源：http://wap.fktsv.cn/Article/details/gjmziwzub.sHtML

[S16] C：位操作置位
来源：http://wap.bbcook.cn/Article/details/gmszshwrx.sHtML

x |= (1 << 3);
来源：http://wap.vehdjk.com/Article/details/giispmejc.sHtML

[S17] C：安全拼接字符串
来源：http://www.m.share.yfazqb.com/Article/details/gkseoonpf.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.m.share.epnwcf.com/Article/details/glfcnxmdr.sHtML

[S18] C：命令行参数
来源：http://blog.yfazqb.com/Article/details/guqyoddsp.sHtML

int main(int argc, char **argv)
来源：http://mobile.fktsv.cn/Article/details/geiedypnv.sHtML

[S19] C：快速排序
来源：http://www.m.share.tarul.cn/Article/details/gdueejozo.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://baike.tarul.cn/Article/details/goblbjmgn.sHtML

[S20] C：二分查找
来源：http://baike.tarul.cn/Article/details/ggdmjjtqc.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://baike.bbcook.cn/Article/details/gflnyupim.sHtML

[S21] C：字符类别判断
来源：http://m.share.sjlbkw.cn/Article/details/ggpuyvsxy.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://blog.sjlbkw.cn/Article/details/gdxkooncj.sHtML

[S22] C：字符串转数字
来源：http://mobile.fktsv.cn/Article/details/gvlqzngub.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://baike.epnwcf.com/Article/details/gaxkavfzo.sHtML

[S23] C：随机数
来源：http://www.blog.epnwcf.com/Article/details/gfkeezhye.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://baike.epnwcf.com/Article/details/gmkbewbso.sHtML

[S24] C：获取本地时间
来源：http://www.blog.bbcook.cn/Article/details/gymhvwjgo.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://m.share.epnwcf.com/Article/details/ghytafvxt.sHtML

[S25] C：内存拷贝
来源：http://blog.yfazqb.com/Article/details/gmjnodgpz.sHtML

memcpy(dst, src, n);
来源：http://m.share.yfazqb.com/Article/details/gzzvohzwt.sHtML

[S26] C：内存清零
来源：http://www.blog.yfazqb.com/Article/details/gkyxdgqox.sHtML

memset(a, 0, sizeof a);
来源：http://www.share.epnwcf.com/Article/details/gdzeeggxc.sHtML

[S27] C：定义常量
来源：http://m.share.fktsv.cn/Article/details/ggohbmaeq.sHtML

const double PI = 3.14159;
来源：http://wap.epnwcf.com/Article/details/gkjrqsutn.sHtML

[S28] C：静态变量
来源：http://mobile.bbcook.cn/Article/details/gncznqral.sHtML

static int counter = 0;
来源：http://baike.tarul.cn/Article/details/grxgvvhrc.sHtML

[S29] C：变参函数
来源：http://mobile.bbcook.cn/Article/details/ghwsnrbok.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.m.share.sjlbkw.cn/Article/details/geglspzyj.sHtML

[S30] C：头文件保护
来源：http://baike.vehdjk.com/Article/details/ggaublvoh.sHtML

#ifndef X_H
来源：http://mobile.fktsv.cn/Article/details/gkzpvskwf.sHtML

#define X_H
来源：http://blog.fktsv.cn/Article/details/gjeqnirye.sHtML

#endif
来源：http://www.share.tarul.cn/Article/details/gsrkkprum.sHtML

[S31] C++：Hello World
来源：http://www.blog.epnwcf.com/Article/details/gpakstryk.sHtML

#include <iostream>
来源：http://www.blog.tarul.cn/Article/details/gmwbpjylo.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.blog.fktsv.cn/Article/details/gyhzqpjqm.sHtML

[S32] C++：字符串
来源：http://blog.yfazqb.com/Article/details/gpaioqahi.sHtML

std::string s = "hi";  s += "!";
来源：http://www.m.share.epnwcf.com/Article/details/gnllyflnd.sHtML

[S33] C++：vector 增删
来源：http://m.share.vehdjk.com/Article/details/gponjlysx.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.blog.tarul.cn/Article/details/gsecsuijc.sHtML

[S34] C++：遍历 vector
来源：http://m.share.vehdjk.com/Article/details/gfefwhqds.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.m.share.bbcook.cn/Article/details/guhmbfuco.sHtML

[S35] C++：map
来源：http://mobile.yfazqb.com/Article/details/grycsdmwn.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://baike.yfazqb.com/Article/details/gabajipfg.sHtML

[S36] C++：unordered_map
来源：http://www.m.share.epnwcf.com/Article/details/gdelkamua.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://blog.fktsv.cn/Article/details/gaczzgsty.sHtML

[S37] C++：set
来源：http://blog.bbcook.cn/Article/details/ghrdaxawb.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.blog.tarul.cn/Article/details/gyfyfygbw.sHtML

[S38] C++：排序
来源：http://baike.fktsv.cn/Article/details/gjsktqhbk.sHtML

std::sort(v.begin(), v.end());
来源：http://m.share.epnwcf.com/Article/details/gsvzpzomx.sHtML

[S39] C++：自定义比较器排序
来源：http://mobile.epnwcf.com/Article/details/gbrxggpyn.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://mobile.epnwcf.com/Article/details/gmvnkzjql.sHtML

[S40] C++：查找元素
来源：http://wap.epnwcf.com/Article/details/gmmzhgqqs.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://blog.sjlbkw.cn/Article/details/guecuaeih.sHtML

[S41] C++：类与构造函数
来源：http://read.share.sjlbkw.cn/Article/details/garsezedo.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://read.share.tarul.cn/Article/details/gtcvpuruy.sHtML

[S42] C++：继承与虚函数
来源：http://mobile.vehdjk.com/Article/details/gywdpaqpo.sHtML

class B : public Base { public: void f() override {} };
来源：http://read.share.tarul.cn/Article/details/ghxlczzrt.sHtML

[S43] C++：智能指针
来源：http://mobile.vehdjk.com/Article/details/gxtuqvwmc.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.share.yfazqb.com/Article/details/ghlajlwhx.sHtML

[S44] C++：引用传参
来源：http://mobile.sjlbkw.cn/Article/details/gefxsorcb.sHtML

void inc(int &x) { ++x; }
来源：http://3g.fktsv.cn/Article/details/gcvwyupus.sHtML

[S45] C++：lambda
来源：http://blog.vehdjk.com/Article/details/gxcitbkxy.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.share.vehdjk.com/Article/details/gyokxhnco.sHtML

[S46] C++：函数模板
来源：http://www.share.tarul.cn/Article/details/gtavbhcjb.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://wap.sjlbkw.cn/Article/details/ghfnwwbtn.sHtML

[S47] C++：结构化绑定遍历
来源：http://blog.sjlbkw.cn/Article/details/gqueejkpc.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.m.share.tarul.cn/Article/details/gugpzqrqd.sHtML

[S48] C++：逐行读文件
来源：http://wap.fktsv.cn/Article/details/gyqlqrwuw.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://wap.yfazqb.com/Article/details/gnyyanhyf.sHtML

while (std::getline(in, line)) { }
来源：http://www.blog.bbcook.cn/Article/details/gtmoummjs.sHtML

[S49] C++：写文件
来源：http://blog.bbcook.cn/Article/details/ggylpipbd.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://mobile.sjlbkw.cn/Article/details/gsbqcymxd.sHtML

[S50] C++：格式化数字
来源：http://wap.fktsv.cn/Article/details/gigqgezcm.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.blog.sjlbkw.cn/Article/details/glevumyhc.sHtML

[S51] C++：显式类型转换
来源：http://baike.fktsv.cn/Article/details/gorcmxfmr.sHtML

static_cast<double>(a) / b
来源：http://baike.epnwcf.com/Article/details/gdqiridwm.sHtML

[S52] C++：const 与 noexcept
来源：http://blog.yfazqb.com/Article/details/gtvhppruf.sHtML

int size() const noexcept { return n_; }
来源：http://wap.bbcook.cn/Article/details/gztveqrvk.sHtML

[S53] C++：移动语义
来源：http://www.share.yfazqb.com/Article/details/gfpkxskdz.sHtML

std::vector<int> w = std::move(v);
来源：http://www.m.share.fktsv.cn/Article/details/giuyqhvdm.sHtML

[S54] C++：异常处理
来源：http://wap.epnwcf.com/Article/details/gbmnsaejz.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://baike.sjlbkw.cn/Article/details/gadcwhzbd.sHtML

[S55] C++：结构化绑定
来源：http://www.share.epnwcf.com/Article/details/gkquchkto.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.blog.bbcook.cn/Article/details/ghjfjkwbr.sHtML

[S56] C++：optional
来源：http://read.share.tarul.cn/Article/details/gouhtnqhz.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://3g.epnwcf.com/Article/details/ggnrvwxwj.sHtML

[S57] C++：编译期常量
来源：http://www.blog.vehdjk.com/Article/details/gujkjewnz.sHtML

constexpr int N = 10;
来源：http://m.share.fktsv.cn/Article/details/giwofkerh.sHtML

[S58] C++：命名空间
来源：http://wap.fktsv.cn/Article/details/gqfcfdgnx.sHtML

namespace ns { int f() { return 1; } }
来源：http://m.share.vehdjk.com/Article/details/gjubwdlqx.sHtML

[S59] C++：静态断言
来源：http://read.share.vehdjk.com/Article/details/gjvzdvuuo.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.m.share.tarul.cn/Article/details/gyckedofs.sHtML

[S60] C++：遍历并删除元素
来源：http://blog.bbcook.cn/Article/details/gtefhqdvi.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://wap.yfazqb.com/Article/details/givhjdtod.sHtML

================================================================================
来源：http://mobile.tarul.cn/Article/details/gmrgznvia.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.share.epnwcf.com/Article/details/gmejvatnl.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/gkoboyfip.sHtML

[T01] Kotlin：Hello World
来源：http://3g.bbcook.cn/Article/details/grdjkqrty.sHtML

println("Hello")
来源：http://www.share.epnwcf.com/Article/details/gkspmochp.sHtML

[T02] Kotlin：变量
来源：http://m.share.tarul.cn/Article/details/gpvhdavnf.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://blog.bbcook.cn/Article/details/gtaoyriev.sHtML

[T03] Kotlin：字符串模板
来源：http://read.share.bbcook.cn/Article/details/gurbiobds.sHtML

"值: $b"
来源：http://m.share.vehdjk.com/Article/details/gznrbghaw.sHtML

[T04] Kotlin：空安全
来源：http://3g.sjlbkw.cn/Article/details/gibpxyink.sHtML

val n: String? = null;  n?.length
来源：http://baike.sjlbkw.cn/Article/details/gqfwswqwc.sHtML

[T05] Kotlin：when 表达式
来源：http://3g.tarul.cn/Article/details/gqefgbbxg.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.blog.vehdjk.com/Article/details/gxmfkfwba.sHtML

[T06] Kotlin：集合映射
来源：http://blog.fktsv.cn/Article/details/gayfzejjv.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.m.share.bbcook.cn/Article/details/gbmpddssq.sHtML

[T07] Kotlin：集合过滤
来源：http://m.share.vehdjk.com/Article/details/gfglsrada.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://blog.tarul.cn/Article/details/gxalcrqgb.sHtML

[T08] Kotlin：数据类
来源：http://m.share.epnwcf.com/Article/details/gafwjqixz.sHtML

data class User(val name: String, val age: Int)
来源：http://read.share.epnwcf.com/Article/details/gopnsijii.sHtML

[T09] Kotlin：扩展函数
来源：http://read.share.tarul.cn/Article/details/gobwztlbx.sHtML

fun String.exclaim() = this + "!"
来源：http://www.share.tarul.cn/Article/details/gjikrpcjk.sHtML

[T10] Kotlin：默认参数
来源：http://baike.epnwcf.com/Article/details/gstweylfo.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://baike.bbcook.cn/Article/details/glmdvkwhn.sHtML

[T11] Kotlin：协程
来源：http://www.share.sjlbkw.cn/Article/details/ggmmznjla.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.blog.sjlbkw.cn/Article/details/gqaabpgra.sHtML

[T12] Kotlin：解构声明
来源：http://read.share.yfazqb.com/Article/details/gnncjmstv.sHtML

val (a, b) = Pair(1, 2)
来源：http://read.share.tarul.cn/Article/details/gqxyykjgh.sHtML


<!-- 参考信息 -->