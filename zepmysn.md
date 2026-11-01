代发 wailian999

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://read.share.tarul.cn/Article/details/gtnxatxqp.sHtML

[R08] 数值比较
来源：http://baike.bbcook.cn/Article/details/gvraaaeib.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.m.share.sjlbkw.cn/Article/details/gtvtbwlpw.sHtML

[R09] 字符串比较
来源：http://www.m.share.bbcook.cn/Article/details/gsqqomorw.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://read.share.fktsv.cn/Article/details/guijalffc.sHtML

[R10] 正则匹配
来源：http://wap.tarul.cn/Article/details/gymfxjwrm.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://3g.yfazqb.com/Article/details/gefoxhsyn.sHtML

[R11] case 多分支
来源：http://mobile.bbcook.cn/Article/details/gtqscmmum.sHtML

case "$1" in
来源：http://www.blog.bbcook.cn/Article/details/gsngizonp.sHtML

start) echo "启动" ;;
来源：http://mobile.vehdjk.com/Article/details/gnhtmnfdm.sHtML

stop)  echo "停止" ;;
来源：http://read.share.tarul.cn/Article/details/gomyzgqpj.sHtML

*)     echo "未知命令" ;;
来源：http://3g.fktsv.cn/Article/details/gjmckaugb.sHtML

esac
来源：http://blog.fktsv.cn/Article/details/gxacwlcbs.sHtML

[R12] for 遍历文件
来源：http://www.share.vehdjk.com/Article/details/glrbjppqw.sHtML

for f in *.txt; do echo "$f"; done
来源：http://mobile.fktsv.cn/Article/details/gxwetwzpd.sHtML

[R13] for 计数循环
来源：http://www.blog.epnwcf.com/Article/details/gxenmrpnx.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://read.share.yfazqb.com/Article/details/gfdrepqhi.sHtML

[R14] C 风格 for
来源：http://read.share.yfazqb.com/Article/details/gvylwnahp.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://mobile.vehdjk.com/Article/details/gjmlahanm.sHtML

[R15] while 逐行读文件
来源：http://blog.sjlbkw.cn/Article/details/gqxwlvudj.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.m.share.vehdjk.com/Article/details/ghriuhleq.sHtML

[R16] until 等待条件
来源：http://mobile.sjlbkw.cn/Article/details/gxgtwbvym.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://m.share.bbcook.cn/Article/details/gpgitnhao.sHtML

[R17] 数组定义与取值
来源：http://m.share.bbcook.cn/Article/details/grbwzoutn.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://3g.fktsv.cn/Article/details/gcbgqcnsa.sHtML

[R18] 遍历数组
来源：http://read.share.tarul.cn/Article/details/gmaeucanu.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://read.share.vehdjk.com/Article/details/gqejpxdcq.sHtML

[R19] 数组长度
来源：http://wap.yfazqb.com/Article/details/giimkkjwv.sHtML

echo "${#arr[@]}"
来源：http://wap.sjlbkw.cn/Article/details/gcyotoaen.sHtML

[R20] 关联数组（字典）
来源：http://www.m.share.bbcook.cn/Article/details/gosmjyddh.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.share.epnwcf.com/Article/details/gtawoshyr.sHtML

[R21] 字符串长度
来源：http://read.share.yfazqb.com/Article/details/gydvkvgev.sHtML

echo "${#s}"
来源：http://www.m.share.fktsv.cn/Article/details/ggtdzhara.sHtML

[R22] 截取子串
来源：http://www.blog.epnwcf.com/Article/details/gmkdnuhgk.sHtML

echo "${s:0:5}"
来源：http://read.share.sjlbkw.cn/Article/details/gkwuhxkdl.sHtML

[R23] 字符串替换
来源：http://www.share.fktsv.cn/Article/details/gvpnbpbkn.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.blog.tarul.cn/Article/details/gyabrqswy.sHtML

[R24] 大小写转换
来源：http://3g.sjlbkw.cn/Article/details/gpuycdopb.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://mobile.yfazqb.com/Article/details/gnvxeylxm.sHtML

[R25] 去后缀 / 去前缀
来源：http://wap.sjlbkw.cn/Article/details/gulzoyvsr.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.blog.yfazqb.com/Article/details/gcgxixnjb.sHtML

[R26] 命令替换
来源：http://mobile.yfazqb.com/Article/details/gzgtuhdbb.sHtML

now=$(date +%F); echo "$now"
来源：http://read.share.sjlbkw.cn/Article/details/gqtzpfcqo.sHtML

[R27] 算术展开
来源：http://3g.bbcook.cn/Article/details/gfadrecnq.sHtML

echo $((1 + 2 * 3))
来源：http://www.m.share.vehdjk.com/Article/details/gjacuqrff.sHtML

[R28] 浮点运算
来源：http://3g.sjlbkw.cn/Article/details/gygyubkmr.sHtML

echo "scale=2; 10/3" | bc
来源：http://baike.vehdjk.com/Article/details/gdyeyvido.sHtML

[R29] 定义函数
来源：http://www.m.share.yfazqb.com/Article/details/giekjqyex.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.share.epnwcf.com/Article/details/ggelyxqmx.sHtML

[R30] 函数返回状态码
来源：http://www.m.share.fktsv.cn/Article/details/gpwnntrzd.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://baike.fktsv.cn/Article/details/ggqptsstn.sHtML

[R31] 局部变量
来源：http://m.share.epnwcf.com/Article/details/gbusvhkab.sHtML

f() { local x=1; echo "$x"; }
来源：http://blog.tarul.cn/Article/details/gctjsdtno.sHtML

[R32] 参数个数校验
来源：http://blog.fktsv.cn/Article/details/gmedqwgry.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://3g.yfazqb.com/Article/details/gqmgtrsgm.sHtML

[R33] 捕获错误并提示行号
来源：http://m.share.fktsv.cn/Article/details/gcfmqlhcb.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://mobile.vehdjk.com/Article/details/ggkscmegc.sHtML

[R34] 退出时清理
来源：http://3g.yfazqb.com/Article/details/gpiervnzl.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.share.sjlbkw.cn/Article/details/gobmsaciz.sHtML

[R35] 后台执行并等待
来源：http://m.share.sjlbkw.cn/Article/details/gxrxmpbuk.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://blog.yfazqb.com/Article/details/gmygpgmmy.sHtML

[R36] 并发执行多个任务
来源：http://baike.bbcook.cn/Article/details/gpykhhfwo.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://mobile.sjlbkw.cn/Article/details/gosfzkvcz.sHtML

[R37] 把输出赋给变量
来源：http://www.blog.sjlbkw.cn/Article/details/grcxjaymm.sHtML

files=$(ls -1)
来源：http://www.share.vehdjk.com/Article/details/gqokkxuso.sHtML

[R38] 管道串联
来源：http://read.share.bbcook.cn/Article/details/gfhxlcuqb.sHtML

cat a.txt | grep -i error | wc -l
来源：http://wap.sjlbkw.cn/Article/details/gabppylif.sHtML

[R39] 重定向标准输出与错误
来源：http://baike.bbcook.cn/Article/details/ggvfiqqwu.sHtML

cmd > out.log 2>&1
来源：http://www.m.share.sjlbkw.cn/Article/details/grhjsnllb.sHtML

[R40] 追加写日志
来源：http://mobile.vehdjk.com/Article/details/gedslmmlk.sHtML

echo "log" >> out.log
来源：http://baike.epnwcf.com/Article/details/gufngafkz.sHtML

[R41] 丢弃输出
来源：http://mobile.tarul.cn/Article/details/gcagpextw.sHtML

cmd >/dev/null 2>&1
来源：http://wap.bbcook.cn/Article/details/gmmpjxpng.sHtML

[R42] 输入重定向
来源：http://www.blog.bbcook.cn/Article/details/gnmlzfbwf.sHtML

wc -l < a.txt
来源：http://wap.epnwcf.com/Article/details/gofqyssjh.sHtML

[R43] 按名字查找文件
来源：http://blog.epnwcf.com/Article/details/gyjnfxxtn.sHtML

find . -name "*.log" -type f
来源：http://baike.fktsv.cn/Article/details/gcdlbeyei.sHtML

[R44] 按修改时间查找
来源：http://mobile.bbcook.cn/Article/details/gtfwizmte.sHtML

find . -mtime -7 -type f
来源：http://wap.sjlbkw.cn/Article/details/gaebmtwws.sHtML

[R45] 批量删除
来源：http://m.share.tarul.cn/Article/details/gsjovybzq.sHtML

find . -name "*.tmp" -delete
来源：http://3g.fktsv.cn/Article/details/gabtcmfcz.sHtML

[R46] 递归替换文件内容
来源：http://m.share.fktsv.cn/Article/details/gljgreenw.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.blog.vehdjk.com/Article/details/ggidzitbg.sHtML

[R47] sed 单行替换
来源：http://read.share.yfazqb.com/Article/details/gnqmlqzcp.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.share.vehdjk.com/Article/details/gyzokrmsd.sHtML

[R48] awk 取指定列
来源：http://mobile.fktsv.cn/Article/details/gvonuhrks.sHtML

awk '{print $1, $3}' a.txt
来源：http://mobile.sjlbkw.cn/Article/details/gmcyujlrc.sHtML

[R49] awk 带条件
来源：http://m.share.fktsv.cn/Article/details/gcdwdlkit.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.m.share.fktsv.cn/Article/details/gpcysolty.sHtML

[R50] awk 求和
来源：http://wap.fktsv.cn/Article/details/gaaxjjmym.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://blog.epnwcf.com/Article/details/guxvxwufe.sHtML

[R51] 排序去重取前几
来源：http://3g.fktsv.cn/Article/details/gnvntytne.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://blog.epnwcf.com/Article/details/gufifhzsv.sHtML

[R52] 统计行数
来源：http://www.m.share.yfazqb.com/Article/details/gvtgaeduc.sHtML

wc -l a.txt
来源：http://www.m.share.tarul.cn/Article/details/gpsxnzxwi.sHtML

[R53] 查看文件头与实时尾
来源：http://3g.bbcook.cn/Article/details/guuhtxuwt.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://blog.tarul.cn/Article/details/gmgmasqwv.sHtML

[R54] 比较两个文件
来源：http://read.share.fktsv.cn/Article/details/gwuqwugne.sHtML

diff a.txt b.txt
来源：http://www.m.share.fktsv.cn/Article/details/gbiwxilha.sHtML

[R55] 压缩与解压
来源：http://www.m.share.fktsv.cn/Article/details/gfjbcyotd.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.m.share.tarul.cn/Article/details/gcmysjryh.sHtML

[R56] 远程拷贝
来源：http://blog.vehdjk.com/Article/details/gfwztqdcr.sHtML

scp file user@host:/path/
来源：http://m.share.sjlbkw.cn/Article/details/gpokbqtfi.sHtML

[R57] 远程执行命令
来源：http://www.blog.epnwcf.com/Article/details/gxswissgd.sHtML

ssh user@host 'uptime'
来源：http://www.m.share.tarul.cn/Article/details/gbuyumapf.sHtML

[R58] 下载文件
来源：http://www.share.epnwcf.com/Article/details/gsuqwluts.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.blog.bbcook.cn/Article/details/gtxtmqbnn.sHtML

[R59] 发 POST JSON
来源：http://m.share.yfazqb.com/Article/details/gwsncxjtj.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://3g.tarul.cn/Article/details/ghsqgmxsb.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.share.fktsv.cn/Article/details/gosueduvt.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://3g.sjlbkw.cn/Article/details/ghbwfwnnx.sHtML

[R61] 磁盘占用
来源：http://wap.yfazqb.com/Article/details/gqqznjymd.sHtML

df -h;  du -sh *
来源：http://mobile.bbcook.cn/Article/details/glivabgxn.sHtML

[R62] 找最占空间的文件
来源：http://www.blog.tarul.cn/Article/details/gncpubnor.sHtML

du -ah . | sort -rh | head -10
来源：http://blog.vehdjk.com/Article/details/gxamxbaoz.sHtML

[R63] 内存与进程
来源：http://baike.sjlbkw.cn/Article/details/gspzmwuxn.sHtML

free -h;  ps aux | grep nginx
来源：http://wap.epnwcf.com/Article/details/gtirojpzs.sHtML

[R64] 结束进程
来源：http://www.blog.bbcook.cn/Article/details/gsvpvhkxr.sHtML

kill -9 $(pgrep -f app.py)
来源：http://baike.sjlbkw.cn/Article/details/gygkldoua.sHtML

[R65] 查看端口占用
来源：http://m.share.vehdjk.com/Article/details/gtfszeegb.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://read.share.vehdjk.com/Article/details/gfxbxfasz.sHtML

[R66] 定时任务
来源：http://baike.vehdjk.com/Article/details/gbroxaluj.sHtML

crontab -e;  crontab -l
来源：http://www.blog.vehdjk.com/Article/details/gilbqguzv.sHtML

[R67] 生成随机十六进制串
来源：http://read.share.fktsv.cn/Article/details/garevogwk.sHtML

openssl rand -hex 16
来源：http://www.m.share.epnwcf.com/Article/details/gndpwsxqe.sHtML

[R68] 计算文件校验值
来源：http://m.share.epnwcf.com/Article/details/gnsjqacsc.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://mobile.yfazqb.com/Article/details/glxtvvkrj.sHtML

[R69] 生成随机密码
来源：http://wap.bbcook.cn/Article/details/gexufhibd.sHtML

head -c 16 /dev/urandom | base64
来源：http://mobile.yfazqb.com/Article/details/gmausqfpl.sHtML

[R70] 时间戳与互转
来源：http://wap.sjlbkw.cn/Article/details/gjbcgllqo.sHtML

date +%s;  date -d @1700000000
来源：http://m.share.tarul.cn/Article/details/gfmytbvqn.sHtML

[R71] 日期格式化
来源：http://m.share.epnwcf.com/Article/details/gsmbfvrni.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://wap.vehdjk.com/Article/details/gpildquao.sHtML

[R72] 等待端口就绪
来源：http://read.share.tarul.cn/Article/details/ghivqyjvp.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://baike.tarul.cn/Article/details/gpfftxobt.sHtML

[R73] 分割大日志
来源：http://mobile.yfazqb.com/Article/details/ggfhibyzx.sHtML

split -l 1000 big.log part_
来源：http://baike.bbcook.cn/Article/details/gcioeoluo.sHtML

[R74] 批量重命名
来源：http://mobile.sjlbkw.cn/Article/details/gfxujdrjv.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.blog.yfazqb.com/Article/details/griunfjek.sHtML

[R75] 导出环境变量
来源：http://wap.vehdjk.com/Article/details/ghwhhygib.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.share.yfazqb.com/Article/details/grgnuhlvy.sHtML

[R76] 使用临时文件
来源：http://3g.vehdjk.com/Article/details/ggchqdqfy.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://3g.yfazqb.com/Article/details/gmlvnxxkk.sHtML

[R77] 读取用户输入
来源：http://www.share.sjlbkw.cn/Article/details/gcgrfryhp.sHtML

read -rp "请输入: " ans
来源：http://3g.bbcook.cn/Article/details/grqthpjdd.sHtML

[R78] 交互式菜单
来源：http://m.share.tarul.cn/Article/details/guntkpxsf.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://mobile.vehdjk.com/Article/details/geqqngmxk.sHtML

[R79] 解析命令行选项
来源：http://wap.bbcook.cn/Article/details/gcmqqwitl.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://blog.fktsv.cn/Article/details/ggjzfkugm.sHtML

[R80] 查看脚本执行耗时
来源：http://wap.tarul.cn/Article/details/gyayjwior.sHtML

time ./run.sh
来源：http://mobile.yfazqb.com/Article/details/guteyhncu.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/glonxooof.sHtML

S. C / C++ 专题
来源：http://www.share.fktsv.cn/Article/details/gftbfxeau.sHtML

================================================================================
来源：http://www.m.share.sjlbkw.cn/Article/details/gpjocwtqk.sHtML

[S01] C：Hello World
来源：http://wap.fktsv.cn/Article/details/ghgjvfelc.sHtML

#include <stdio.h>
来源：http://m.share.yfazqb.com/Article/details/gbrcyiyke.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://wap.yfazqb.com/Article/details/gvuhhjwrh.sHtML

[S02] C：变量与格式化输出
来源：http://www.m.share.bbcook.cn/Article/details/gvaajmreq.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.m.share.tarul.cn/Article/details/gkvkalugl.sHtML

[S03] C：读入整数
来源：http://3g.yfazqb.com/Article/details/ggziytjfd.sHtML

int x; scanf("%d", &x);
来源：http://blog.vehdjk.com/Article/details/guhtcazaz.sHtML

[S04] C：字符串复制
来源：http://blog.fktsv.cn/Article/details/glsikmefc.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://read.share.tarul.cn/Article/details/gqskzviez.sHtML

[S05] C：字符串长度
来源：http://baike.sjlbkw.cn/Article/details/gejyeffqr.sHtML

strlen(s)
来源：http://read.share.fktsv.cn/Article/details/gmdzuemlz.sHtML

[S06] C：字符串比较
来源：http://www.share.sjlbkw.cn/Article/details/goeiaxcic.sHtML

strcmp(a, b) == 0
来源：http://3g.tarul.cn/Article/details/gaesygscs.sHtML

[S07] C：数组遍历求和
来源：http://m.share.bbcook.cn/Article/details/gizmodyjd.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://wap.sjlbkw.cn/Article/details/gsydoxdgo.sHtML

[S08] C：动态内存分配与释放
来源：http://read.share.bbcook.cn/Article/details/gobgmgmvs.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.blog.vehdjk.com/Article/details/gbrbcsrgi.sHtML

[S09] C：结构体定义与初始化
来源：http://m.share.vehdjk.com/Article/details/gyaqctixa.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.share.tarul.cn/Article/details/gjiijszdm.sHtML

[S10] C：指针与解引用
来源：http://blog.vehdjk.com/Article/details/glsybdrat.sHtML

int *p = &a;  *p = 5;
来源：http://wap.yfazqb.com/Article/details/gclddwyjk.sHtML

[S11] C：逐行读文件
来源：http://mobile.bbcook.cn/Article/details/grtmygpvp.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://wap.tarul.cn/Article/details/gpiwcvxac.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://mobile.vehdjk.com/Article/details/gvporqmhi.sHtML

fclose(f);
来源：http://www.blog.fktsv.cn/Article/details/gnwbnfjtr.sHtML

[S12] C：写文件
来源：http://mobile.yfazqb.com/Article/details/gxswwbwzg.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.m.share.sjlbkw.cn/Article/details/gnucszbfc.sHtML

[S13] C：宏定义
来源：http://baike.yfazqb.com/Article/details/gogconfks.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://read.share.sjlbkw.cn/Article/details/gcjxamdlb.sHtML

[S14] C：枚举
来源：http://mobile.yfazqb.com/Article/details/glczozebf.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://mobile.epnwcf.com/Article/details/gqqbrgwac.sHtML

[S15] C：类型转换
来源：http://mobile.fktsv.cn/Article/details/gfxyyrosp.sHtML

(double) a / b
来源：http://mobile.sjlbkw.cn/Article/details/gncbnzyjq.sHtML

[S16] C：位操作置位
来源：http://m.share.yfazqb.com/Article/details/gofspuqxv.sHtML

x |= (1 << 3);
来源：http://baike.tarul.cn/Article/details/gccferzjf.sHtML

[S17] C：安全拼接字符串
来源：http://wap.epnwcf.com/Article/details/ggemobxvi.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://baike.yfazqb.com/Article/details/gvozsnudh.sHtML

[S18] C：命令行参数
来源：http://www.blog.fktsv.cn/Article/details/gjfpmuwzs.sHtML

int main(int argc, char **argv)
来源：http://www.m.share.vehdjk.com/Article/details/griaapnaa.sHtML

[S19] C：快速排序
来源：http://mobile.epnwcf.com/Article/details/gbmfoxbgt.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.blog.sjlbkw.cn/Article/details/ggrptctcl.sHtML

[S20] C：二分查找
来源：http://mobile.epnwcf.com/Article/details/grhlkcwst.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://wap.tarul.cn/Article/details/glkeguxwg.sHtML

[S21] C：字符类别判断
来源：http://read.share.tarul.cn/Article/details/gtrcvxuhi.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://baike.tarul.cn/Article/details/gcfcfmfui.sHtML

[S22] C：字符串转数字
来源：http://3g.bbcook.cn/Article/details/gupyfklty.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://m.share.sjlbkw.cn/Article/details/gmprcvszl.sHtML

[S23] C：随机数
来源：http://baike.epnwcf.com/Article/details/gmtlqjtey.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://mobile.yfazqb.com/Article/details/gecwtbvdb.sHtML

[S24] C：获取本地时间
来源：http://m.share.fktsv.cn/Article/details/gsvfzycgq.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://read.share.bbcook.cn/Article/details/gwvqlitrd.sHtML

[S25] C：内存拷贝
来源：http://blog.vehdjk.com/Article/details/gvtfupemz.sHtML

memcpy(dst, src, n);
来源：http://baike.fktsv.cn/Article/details/gemwvjmdq.sHtML

[S26] C：内存清零
来源：http://m.share.epnwcf.com/Article/details/gkmooqunk.sHtML

memset(a, 0, sizeof a);
来源：http://wap.fktsv.cn/Article/details/gpjfkyoqc.sHtML

[S27] C：定义常量
来源：http://3g.bbcook.cn/Article/details/gjyohjbcr.sHtML

const double PI = 3.14159;
来源：http://blog.tarul.cn/Article/details/gubnasmeo.sHtML

[S28] C：静态变量
来源：http://mobile.epnwcf.com/Article/details/glkdacqlg.sHtML

static int counter = 0;
来源：http://3g.epnwcf.com/Article/details/ggkizkcct.sHtML

[S29] C：变参函数
来源：http://m.share.fktsv.cn/Article/details/gqybujjvu.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.share.yfazqb.com/Article/details/gxuamndov.sHtML

[S30] C：头文件保护
来源：http://mobile.vehdjk.com/Article/details/gaevnjsdv.sHtML

#ifndef X_H
来源：http://www.share.bbcook.cn/Article/details/gifttwiph.sHtML

#define X_H
来源：http://mobile.vehdjk.com/Article/details/gfmrxziul.sHtML

#endif
来源：http://m.share.vehdjk.com/Article/details/guqdliwob.sHtML

[S31] C++：Hello World
来源：http://blog.bbcook.cn/Article/details/gprllkpse.sHtML

#include <iostream>
来源：http://baike.epnwcf.com/Article/details/giftubxda.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.share.sjlbkw.cn/Article/details/gtajoxwuh.sHtML

[S32] C++：字符串
来源：http://read.share.fktsv.cn/Article/details/glflkygys.sHtML

std::string s = "hi";  s += "!";
来源：http://read.share.vehdjk.com/Article/details/gelwevpva.sHtML

[S33] C++：vector 增删
来源：http://mobile.sjlbkw.cn/Article/details/gbxkrahfr.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://read.share.epnwcf.com/Article/details/gbysvbdro.sHtML

[S34] C++：遍历 vector
来源：http://wap.yfazqb.com/Article/details/gbmamyvzv.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://3g.epnwcf.com/Article/details/gckmyezth.sHtML

[S35] C++：map
来源：http://www.blog.sjlbkw.cn/Article/details/gwpzutlzc.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.sjlbkw.cn/Article/details/gxffpcqou.sHtML

[S36] C++：unordered_map
来源：http://www.blog.sjlbkw.cn/Article/details/gcddwrkst.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://blog.epnwcf.com/Article/details/gzmpnhmwq.sHtML

[S37] C++：set
来源：http://www.blog.fktsv.cn/Article/details/gzspeiabn.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://3g.bbcook.cn/Article/details/grizwpedh.sHtML

[S38] C++：排序
来源：http://baike.tarul.cn/Article/details/ghwrgygdh.sHtML

std::sort(v.begin(), v.end());
来源：http://3g.yfazqb.com/Article/details/gvzporipd.sHtML

[S39] C++：自定义比较器排序
来源：http://m.share.epnwcf.com/Article/details/gnzyqvtqi.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://m.share.tarul.cn/Article/details/gasyrsrux.sHtML

[S40] C++：查找元素
来源：http://www.share.fktsv.cn/Article/details/ggjucjpmg.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://mobile.tarul.cn/Article/details/girbdnxfw.sHtML

[S41] C++：类与构造函数
来源：http://read.share.tarul.cn/Article/details/gtyphopiw.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://mobile.epnwcf.com/Article/details/gsajieaal.sHtML

[S42] C++：继承与虚函数
来源：http://baike.bbcook.cn/Article/details/gufhamqjm.sHtML

class B : public Base { public: void f() override {} };
来源：http://m.share.sjlbkw.cn/Article/details/gwucondqb.sHtML

[S43] C++：智能指针
来源：http://www.share.epnwcf.com/Article/details/gyttilbxd.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.m.share.yfazqb.com/Article/details/gfswlmyrr.sHtML

[S44] C++：引用传参
来源：http://www.m.share.vehdjk.com/Article/details/guubzhizy.sHtML

void inc(int &x) { ++x; }
来源：http://wap.yfazqb.com/Article/details/gbuzhauwc.sHtML

[S45] C++：lambda
来源：http://read.share.sjlbkw.cn/Article/details/gxkinbptk.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://m.share.vehdjk.com/Article/details/gsjuwynsg.sHtML

[S46] C++：函数模板
来源：http://www.share.fktsv.cn/Article/details/gwdninhyf.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://m.share.vehdjk.com/Article/details/gxvvtdevu.sHtML

[S47] C++：结构化绑定遍历
来源：http://baike.vehdjk.com/Article/details/gmtpnaicj.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gwzlqukvx.sHtML

[S48] C++：逐行读文件
来源：http://wap.bbcook.cn/Article/details/gwsyaifxy.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://blog.yfazqb.com/Article/details/gvtxphfzv.sHtML

while (std::getline(in, line)) { }
来源：http://baike.fktsv.cn/Article/details/gugpyyfvl.sHtML

[S49] C++：写文件
来源：http://baike.tarul.cn/Article/details/gudzxvzvq.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://blog.sjlbkw.cn/Article/details/gvavbgang.sHtML

[S50] C++：格式化数字
来源：http://blog.yfazqb.com/Article/details/gufxgfbho.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://read.share.epnwcf.com/Article/details/gwozoknnn.sHtML

[S51] C++：显式类型转换
来源：http://m.share.vehdjk.com/Article/details/gbdslrmpo.sHtML

static_cast<double>(a) / b
来源：http://wap.bbcook.cn/Article/details/gxyxuwqpg.sHtML

[S52] C++：const 与 noexcept
来源：http://www.blog.vehdjk.com/Article/details/gcrqcbqya.sHtML

int size() const noexcept { return n_; }
来源：http://mobile.fktsv.cn/Article/details/glojwrfuc.sHtML

[S53] C++：移动语义
来源：http://www.m.share.epnwcf.com/Article/details/gabcbhhhe.sHtML

std::vector<int> w = std::move(v);
来源：http://blog.sjlbkw.cn/Article/details/gtipoltgu.sHtML

[S54] C++：异常处理
来源：http://baike.vehdjk.com/Article/details/gonyrchwv.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://3g.epnwcf.com/Article/details/givmrffki.sHtML

[S55] C++：结构化绑定
来源：http://blog.tarul.cn/Article/details/gjrrhkplq.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://baike.fktsv.cn/Article/details/gcqosybhf.sHtML

[S56] C++：optional
来源：http://www.m.share.vehdjk.com/Article/details/gcnipszwp.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://m.share.epnwcf.com/Article/details/ggpkjwbou.sHtML

[S57] C++：编译期常量
来源：http://www.m.share.vehdjk.com/Article/details/gpfwcgbci.sHtML

constexpr int N = 10;
来源：http://wap.yfazqb.com/Article/details/gnbevxiyf.sHtML

[S58] C++：命名空间
来源：http://www.share.fktsv.cn/Article/details/gbrejhkvn.sHtML

namespace ns { int f() { return 1; } }
来源：http://read.share.bbcook.cn/Article/details/glwmaskpu.sHtML

[S59] C++：静态断言
来源：http://wap.vehdjk.com/Article/details/gzqepocvo.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://read.share.vehdjk.com/Article/details/gtnvmkipq.sHtML

[S60] C++：遍历并删除元素
来源：http://www.share.epnwcf.com/Article/details/gfesakwrq.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://read.share.tarul.cn/Article/details/gacstgwla.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/gwdaziwjy.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://wap.bbcook.cn/Article/details/ghvefwmre.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/gbaguhyku.sHtML

[T01] Kotlin：Hello World
来源：http://read.share.yfazqb.com/Article/details/gearrugch.sHtML

println("Hello")
来源：http://www.m.share.epnwcf.com/Article/details/gdmvgtbfi.sHtML

[T02] Kotlin：变量
来源：http://baike.bbcook.cn/Article/details/gyvszkouz.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://m.share.fktsv.cn/Article/details/ghiskxwmf.sHtML

[T03] Kotlin：字符串模板
来源：http://3g.bbcook.cn/Article/details/gdzikpljk.sHtML

"值: $b"
来源：http://www.share.bbcook.cn/Article/details/gvakqsvhb.sHtML

[T04] Kotlin：空安全
来源：http://m.share.vehdjk.com/Article/details/gudrdfmmg.sHtML

val n: String? = null;  n?.length
来源：http://www.share.vehdjk.com/Article/details/gouwydsmt.sHtML

[T05] Kotlin：when 表达式
来源：http://mobile.sjlbkw.cn/Article/details/gazekfone.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://baike.fktsv.cn/Article/details/gtgqzwhws.sHtML

[T06] Kotlin：集合映射
来源：http://3g.vehdjk.com/Article/details/ggffvblim.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://blog.yfazqb.com/Article/details/gafnrsqty.sHtML

[T07] Kotlin：集合过滤
来源：http://www.blog.sjlbkw.cn/Article/details/gmqdnyujb.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://read.share.fktsv.cn/Article/details/gjwzinanw.sHtML

[T08] Kotlin：数据类
来源：http://www.blog.yfazqb.com/Article/details/glpbhmcwu.sHtML

data class User(val name: String, val age: Int)
来源：http://www.m.share.sjlbkw.cn/Article/details/gdodpymnl.sHtML


<!-- 参考信息 -->