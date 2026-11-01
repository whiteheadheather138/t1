代发 wailian999

name="${1:-default}"
来源：http://wap.yfazqb.com/Article/details/gtzpfhxlc.sHtML

[R06] 判断命令是否存在
来源：http://baike.vehdjk.com/Article/details/ggygpgdxl.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://baike.yfazqb.com/Article/details/ghvfldmsr.sHtML

[R07] if 判断文件
来源：http://www.m.share.epnwcf.com/Article/details/gaicohcvw.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://blog.fktsv.cn/Article/details/gjdiyotfx.sHtML

[R08] 数值比较
来源：http://blog.tarul.cn/Article/details/gzekvejsh.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://mobile.bbcook.cn/Article/details/gqaogaxko.sHtML

[R09] 字符串比较
来源：http://mobile.sjlbkw.cn/Article/details/gapwnnmyl.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://mobile.tarul.cn/Article/details/gqkiqngaj.sHtML

[R10] 正则匹配
来源：http://read.share.sjlbkw.cn/Article/details/gpfrwqmrv.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.m.share.vehdjk.com/Article/details/ghxiwzavd.sHtML

[R11] case 多分支
来源：http://read.share.bbcook.cn/Article/details/glhfmmozz.sHtML

case "$1" in
来源：http://mobile.yfazqb.com/Article/details/gecamkxct.sHtML

start) echo "启动" ;;
来源：http://www.share.vehdjk.com/Article/details/ghzqktlag.sHtML

stop)  echo "停止" ;;
来源：http://baike.yfazqb.com/Article/details/gjakgkqee.sHtML

*)     echo "未知命令" ;;
来源：http://blog.fktsv.cn/Article/details/gktvbxduu.sHtML

esac
来源：http://www.blog.bbcook.cn/Article/details/gguelnggc.sHtML

[R12] for 遍历文件
来源：http://www.blog.sjlbkw.cn/Article/details/glowvhlom.sHtML

for f in *.txt; do echo "$f"; done
来源：http://mobile.bbcook.cn/Article/details/gzynueqch.sHtML

[R13] for 计数循环
来源：http://www.share.bbcook.cn/Article/details/gmeyijzyy.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://blog.sjlbkw.cn/Article/details/ggredkwiz.sHtML

[R14] C 风格 for
来源：http://read.share.tarul.cn/Article/details/gdkjuaqsj.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://read.share.bbcook.cn/Article/details/gfryzihlp.sHtML

[R15] while 逐行读文件
来源：http://3g.epnwcf.com/Article/details/gkgaihgak.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://m.share.yfazqb.com/Article/details/glhtgukpz.sHtML

[R16] until 等待条件
来源：http://m.share.yfazqb.com/Article/details/gfykfkklv.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://read.share.bbcook.cn/Article/details/gxmwjuakw.sHtML

[R17] 数组定义与取值
来源：http://wap.epnwcf.com/Article/details/gfgzurkyx.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://mobile.bbcook.cn/Article/details/godfmekhm.sHtML

[R18] 遍历数组
来源：http://mobile.fktsv.cn/Article/details/gsgwrwfbf.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://wap.yfazqb.com/Article/details/gdakqzdvr.sHtML

[R19] 数组长度
来源：http://read.share.vehdjk.com/Article/details/gnudbonop.sHtML

echo "${#arr[@]}"
来源：http://blog.fktsv.cn/Article/details/gqaaxlqen.sHtML

[R20] 关联数组（字典）
来源：http://www.blog.fktsv.cn/Article/details/guomjxvmx.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.share.vehdjk.com/Article/details/gnszzyifa.sHtML

[R21] 字符串长度
来源：http://baike.bbcook.cn/Article/details/gjzqipkms.sHtML

echo "${#s}"
来源：http://www.share.sjlbkw.cn/Article/details/ggnjwjiya.sHtML

[R22] 截取子串
来源：http://mobile.vehdjk.com/Article/details/gpegobswe.sHtML

echo "${s:0:5}"
来源：http://3g.tarul.cn/Article/details/getelejaz.sHtML

[R23] 字符串替换
来源：http://www.blog.tarul.cn/Article/details/gqqskbhgr.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.blog.bbcook.cn/Article/details/gwivbwevi.sHtML

[R24] 大小写转换
来源：http://www.m.share.yfazqb.com/Article/details/gwuawvqjx.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.m.share.sjlbkw.cn/Article/details/gangxwrbs.sHtML

[R25] 去后缀 / 去前缀
来源：http://wap.yfazqb.com/Article/details/gwqvkcdon.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://3g.vehdjk.com/Article/details/gzblemxsn.sHtML

[R26] 命令替换
来源：http://baike.sjlbkw.cn/Article/details/gynfzdicn.sHtML

now=$(date +%F); echo "$now"
来源：http://read.share.vehdjk.com/Article/details/giieyvlkn.sHtML

[R27] 算术展开
来源：http://www.m.share.epnwcf.com/Article/details/ggdotpern.sHtML

echo $((1 + 2 * 3))
来源：http://baike.tarul.cn/Article/details/gblwimczb.sHtML

[R28] 浮点运算
来源：http://mobile.tarul.cn/Article/details/gmlslykgv.sHtML

echo "scale=2; 10/3" | bc
来源：http://m.share.vehdjk.com/Article/details/gbktntdnd.sHtML

[R29] 定义函数
来源：http://blog.epnwcf.com/Article/details/ghifxkopx.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.share.sjlbkw.cn/Article/details/gpdjilhnt.sHtML

[R30] 函数返回状态码
来源：http://www.share.yfazqb.com/Article/details/gcnpwepfe.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://3g.sjlbkw.cn/Article/details/grjeqnhqs.sHtML

[R31] 局部变量
来源：http://blog.bbcook.cn/Article/details/gvmdipqal.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.share.tarul.cn/Article/details/ghzhlvpav.sHtML

[R32] 参数个数校验
来源：http://www.m.share.sjlbkw.cn/Article/details/gcghbedfa.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://m.share.tarul.cn/Article/details/gqtwxjmnu.sHtML

[R33] 捕获错误并提示行号
来源：http://www.blog.fktsv.cn/Article/details/glylwjryq.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.m.share.bbcook.cn/Article/details/ggaexwzfh.sHtML

[R34] 退出时清理
来源：http://wap.epnwcf.com/Article/details/gwzbeovsi.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://m.share.tarul.cn/Article/details/geahvxtdi.sHtML

[R35] 后台执行并等待
来源：http://read.share.vehdjk.com/Article/details/gzfgnstdw.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://m.share.sjlbkw.cn/Article/details/glsjixczs.sHtML

[R36] 并发执行多个任务
来源：http://m.share.epnwcf.com/Article/details/gojqesvjy.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://mobile.fktsv.cn/Article/details/geemhfvwt.sHtML

[R37] 把输出赋给变量
来源：http://www.blog.sjlbkw.cn/Article/details/gglgoesgn.sHtML

files=$(ls -1)
来源：http://www.blog.epnwcf.com/Article/details/gttwstzki.sHtML

[R38] 管道串联
来源：http://3g.fktsv.cn/Article/details/gxkrtxoyb.sHtML

cat a.txt | grep -i error | wc -l
来源：http://mobile.sjlbkw.cn/Article/details/gxpetgtda.sHtML

[R39] 重定向标准输出与错误
来源：http://3g.bbcook.cn/Article/details/gurcrbggi.sHtML

cmd > out.log 2>&1
来源：http://read.share.epnwcf.com/Article/details/gkzskvtip.sHtML

[R40] 追加写日志
来源：http://www.blog.yfazqb.com/Article/details/gzromzmvg.sHtML

echo "log" >> out.log
来源：http://3g.vehdjk.com/Article/details/gmisovjqd.sHtML

[R41] 丢弃输出
来源：http://wap.sjlbkw.cn/Article/details/gczjaqohc.sHtML

cmd >/dev/null 2>&1
来源：http://read.share.epnwcf.com/Article/details/gmgatskue.sHtML

[R42] 输入重定向
来源：http://read.share.vehdjk.com/Article/details/gqdwaafxu.sHtML

wc -l < a.txt
来源：http://3g.fktsv.cn/Article/details/gqmyerqmi.sHtML

[R43] 按名字查找文件
来源：http://baike.tarul.cn/Article/details/gzylnqcyo.sHtML

find . -name "*.log" -type f
来源：http://www.blog.bbcook.cn/Article/details/gsxsvrxxw.sHtML

[R44] 按修改时间查找
来源：http://www.share.yfazqb.com/Article/details/gecfwjvfe.sHtML

find . -mtime -7 -type f
来源：http://mobile.fktsv.cn/Article/details/gtiffusda.sHtML

[R45] 批量删除
来源：http://wap.epnwcf.com/Article/details/gsdidlzdy.sHtML

find . -name "*.tmp" -delete
来源：http://mobile.tarul.cn/Article/details/gmwitpabk.sHtML

[R46] 递归替换文件内容
来源：http://read.share.yfazqb.com/Article/details/gehcmsddt.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://3g.yfazqb.com/Article/details/gltuhuorf.sHtML

[R47] sed 单行替换
来源：http://blog.bbcook.cn/Article/details/giwmjcene.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://3g.bbcook.cn/Article/details/grqwokdnv.sHtML

[R48] awk 取指定列
来源：http://3g.vehdjk.com/Article/details/gktnqlsit.sHtML

awk '{print $1, $3}' a.txt
来源：http://mobile.tarul.cn/Article/details/gnbmjkaoi.sHtML

[R49] awk 带条件
来源：http://wap.yfazqb.com/Article/details/gtwastjuk.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://m.share.vehdjk.com/Article/details/gmmmolryv.sHtML

[R50] awk 求和
来源：http://baike.sjlbkw.cn/Article/details/gfwhrnkyk.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://baike.fktsv.cn/Article/details/gacsiiijo.sHtML

[R51] 排序去重取前几
来源：http://3g.epnwcf.com/Article/details/gakllckgo.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.blog.epnwcf.com/Article/details/gnulcigrb.sHtML

[R52] 统计行数
来源：http://read.share.yfazqb.com/Article/details/guoxurscc.sHtML

wc -l a.txt
来源：http://blog.fktsv.cn/Article/details/gswsputhe.sHtML

[R53] 查看文件头与实时尾
来源：http://wap.tarul.cn/Article/details/gcjoeceml.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://3g.bbcook.cn/Article/details/gftwhgxxo.sHtML

[R54] 比较两个文件
来源：http://www.m.share.vehdjk.com/Article/details/gxoxodqua.sHtML

diff a.txt b.txt
来源：http://www.share.yfazqb.com/Article/details/gibsmvkdd.sHtML

[R55] 压缩与解压
来源：http://mobile.tarul.cn/Article/details/gjdjglczr.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mobile.bbcook.cn/Article/details/gwyrzvola.sHtML

[R56] 远程拷贝
来源：http://3g.epnwcf.com/Article/details/gwzafijif.sHtML

scp file user@host:/path/
来源：http://m.share.sjlbkw.cn/Article/details/gtzsjdehi.sHtML

[R57] 远程执行命令
来源：http://wap.vehdjk.com/Article/details/gdcsgboqf.sHtML

ssh user@host 'uptime'
来源：http://baike.bbcook.cn/Article/details/grffeajum.sHtML

[R58] 下载文件
来源：http://www.blog.sjlbkw.cn/Article/details/gvyqurfed.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.m.share.vehdjk.com/Article/details/gzlbgaeow.sHtML

[R59] 发 POST JSON
来源：http://wap.yfazqb.com/Article/details/gqxdgusky.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.m.share.vehdjk.com/Article/details/gvukbjlkh.sHtML

[R60] 只看 HTTP 状态码
来源：http://blog.tarul.cn/Article/details/gvnpbokgt.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mobile.bbcook.cn/Article/details/gdzzbukyr.sHtML

[R61] 磁盘占用
来源：http://wap.tarul.cn/Article/details/gulowbwik.sHtML

df -h;  du -sh *
来源：http://m.share.epnwcf.com/Article/details/gpzycdesi.sHtML

[R62] 找最占空间的文件
来源：http://www.share.sjlbkw.cn/Article/details/gprmtlfzw.sHtML

du -ah . | sort -rh | head -10
来源：http://mobile.vehdjk.com/Article/details/grafxmixp.sHtML

[R63] 内存与进程
来源：http://mobile.sjlbkw.cn/Article/details/gowbvwvew.sHtML

free -h;  ps aux | grep nginx
来源：http://www.m.share.epnwcf.com/Article/details/gkesmddla.sHtML

[R64] 结束进程
来源：http://mobile.sjlbkw.cn/Article/details/gishlvawg.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.blog.sjlbkw.cn/Article/details/gpayormjv.sHtML

[R65] 查看端口占用
来源：http://wap.yfazqb.com/Article/details/guljfcyik.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.blog.tarul.cn/Article/details/gaytwuygc.sHtML

[R66] 定时任务
来源：http://baike.epnwcf.com/Article/details/gufpekltj.sHtML

crontab -e;  crontab -l
来源：http://mobile.epnwcf.com/Article/details/glfbklsju.sHtML

[R67] 生成随机十六进制串
来源：http://read.share.epnwcf.com/Article/details/geobibujo.sHtML

openssl rand -hex 16
来源：http://blog.vehdjk.com/Article/details/gxoetrgfr.sHtML

[R68] 计算文件校验值
来源：http://wap.tarul.cn/Article/details/gavtvbzkl.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.share.fktsv.cn/Article/details/gzgtvhpvm.sHtML

[R69] 生成随机密码
来源：http://m.share.epnwcf.com/Article/details/gqlyplkcw.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.share.epnwcf.com/Article/details/gajsoemjr.sHtML

[R70] 时间戳与互转
来源：http://wap.yfazqb.com/Article/details/gfffophlp.sHtML

date +%s;  date -d @1700000000
来源：http://baike.epnwcf.com/Article/details/gefcslnbc.sHtML

[R71] 日期格式化
来源：http://wap.bbcook.cn/Article/details/gujnhhkqu.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://blog.bbcook.cn/Article/details/gjsapvmoo.sHtML

[R72] 等待端口就绪
来源：http://www.blog.fktsv.cn/Article/details/gdevznlnl.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.blog.vehdjk.com/Article/details/gljdihczy.sHtML

[R73] 分割大日志
来源：http://www.share.sjlbkw.cn/Article/details/gyexcfzmi.sHtML

split -l 1000 big.log part_
来源：http://read.share.epnwcf.com/Article/details/gyfiowxlk.sHtML

[R74] 批量重命名
来源：http://read.share.fktsv.cn/Article/details/gpgxvapjo.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://mobile.epnwcf.com/Article/details/gjfdugcev.sHtML

[R75] 导出环境变量
来源：http://wap.vehdjk.com/Article/details/gymbkjicd.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://m.share.tarul.cn/Article/details/gmfpvgehw.sHtML

[R76] 使用临时文件
来源：http://blog.vehdjk.com/Article/details/gbllxqbva.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://wap.bbcook.cn/Article/details/gcxelbcxu.sHtML

[R77] 读取用户输入
来源：http://mobile.tarul.cn/Article/details/gyybveqwn.sHtML

read -rp "请输入: " ans
来源：http://m.share.tarul.cn/Article/details/gszoygjtp.sHtML

[R78] 交互式菜单
来源：http://wap.vehdjk.com/Article/details/glbvxxbub.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://baike.yfazqb.com/Article/details/gdhgppvvs.sHtML

[R79] 解析命令行选项
来源：http://www.share.yfazqb.com/Article/details/gamzegttr.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://3g.tarul.cn/Article/details/gignhvkeu.sHtML

[R80] 查看脚本执行耗时
来源：http://www.m.share.sjlbkw.cn/Article/details/gzqcvzoys.sHtML

time ./run.sh
来源：http://baike.sjlbkw.cn/Article/details/ggilgljes.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/gqthwahwe.sHtML

S. C / C++ 专题
来源：http://www.m.share.vehdjk.com/Article/details/ghhjcgmnb.sHtML

================================================================================
来源：http://m.share.tarul.cn/Article/details/gjvvkaukb.sHtML

[S01] C：Hello World
来源：http://wap.fktsv.cn/Article/details/gfhzxpdwh.sHtML

#include <stdio.h>
来源：http://www.m.share.vehdjk.com/Article/details/gmchkpzow.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://baike.fktsv.cn/Article/details/gcppmblch.sHtML

[S02] C：变量与格式化输出
来源：http://read.share.vehdjk.com/Article/details/gwmoxdpsn.sHtML

int a = 10; printf("%d\n", a);
来源：http://m.share.tarul.cn/Article/details/gagpkzuvi.sHtML

[S03] C：读入整数
来源：http://baike.epnwcf.com/Article/details/gwoanikqm.sHtML

int x; scanf("%d", &x);
来源：http://wap.yfazqb.com/Article/details/gtmtigqud.sHtML

[S04] C：字符串复制
来源：http://baike.fktsv.cn/Article/details/gorzetzjp.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.share.bbcook.cn/Article/details/gzxvjnoon.sHtML

[S05] C：字符串长度
来源：http://www.m.share.vehdjk.com/Article/details/gcimjiahp.sHtML

strlen(s)
来源：http://www.share.yfazqb.com/Article/details/gigtwiotv.sHtML

[S06] C：字符串比较
来源：http://www.m.share.bbcook.cn/Article/details/ghtshqxwa.sHtML

strcmp(a, b) == 0
来源：http://3g.fktsv.cn/Article/details/gkocsjkgw.sHtML

[S07] C：数组遍历求和
来源：http://mobile.sjlbkw.cn/Article/details/gupmvmtdq.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.blog.fktsv.cn/Article/details/gtgwjayxu.sHtML

[S08] C：动态内存分配与释放
来源：http://www.share.vehdjk.com/Article/details/gkbbrfmrd.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://read.share.epnwcf.com/Article/details/ghjwywnas.sHtML

[S09] C：结构体定义与初始化
来源：http://www.share.bbcook.cn/Article/details/gcajnjqrv.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://m.share.yfazqb.com/Article/details/gaubinume.sHtML

[S10] C：指针与解引用
来源：http://www.blog.tarul.cn/Article/details/giyzednpc.sHtML

int *p = &a;  *p = 5;
来源：http://www.blog.epnwcf.com/Article/details/gobnnjkfl.sHtML

[S11] C：逐行读文件
来源：http://3g.fktsv.cn/Article/details/girernxqf.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://blog.tarul.cn/Article/details/gfygremcb.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://read.share.epnwcf.com/Article/details/gssqvfnyd.sHtML

fclose(f);
来源：http://3g.fktsv.cn/Article/details/gvexdtrry.sHtML

[S12] C：写文件
来源：http://m.share.sjlbkw.cn/Article/details/gqufvavnf.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://m.share.tarul.cn/Article/details/gzfopxngy.sHtML

[S13] C：宏定义
来源：http://wap.tarul.cn/Article/details/gvypctdqc.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://3g.tarul.cn/Article/details/gzgbroxpz.sHtML

[S14] C：枚举
来源：http://wap.tarul.cn/Article/details/gcwpksckl.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://wap.fktsv.cn/Article/details/gkscwarav.sHtML

[S15] C：类型转换
来源：http://read.share.sjlbkw.cn/Article/details/gasztetbk.sHtML

(double) a / b
来源：http://3g.fktsv.cn/Article/details/gjvnjklch.sHtML

[S16] C：位操作置位
来源：http://www.blog.tarul.cn/Article/details/gdbkabbbw.sHtML

x |= (1 << 3);
来源：http://www.blog.vehdjk.com/Article/details/gyswnngrn.sHtML

[S17] C：安全拼接字符串
来源：http://www.m.share.sjlbkw.cn/Article/details/gafmdctqu.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://3g.fktsv.cn/Article/details/gkzvslqzr.sHtML

[S18] C：命令行参数
来源：http://wap.vehdjk.com/Article/details/gcubbexry.sHtML

int main(int argc, char **argv)
来源：http://blog.bbcook.cn/Article/details/gtyqrqsde.sHtML

[S19] C：快速排序
来源：http://wap.yfazqb.com/Article/details/gdqhmchtz.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://3g.fktsv.cn/Article/details/gapkmagoj.sHtML

[S20] C：二分查找
来源：http://3g.sjlbkw.cn/Article/details/gkahjnjia.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://blog.bbcook.cn/Article/details/gngooelzo.sHtML

[S21] C：字符类别判断
来源：http://www.m.share.bbcook.cn/Article/details/gduspiyli.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://wap.tarul.cn/Article/details/gbpqnalau.sHtML

[S22] C：字符串转数字
来源：http://wap.yfazqb.com/Article/details/gcsjaueyh.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.share.fktsv.cn/Article/details/gpfiroveo.sHtML

[S23] C：随机数
来源：http://wap.sjlbkw.cn/Article/details/gtaskelns.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://read.share.sjlbkw.cn/Article/details/gqaystben.sHtML

[S24] C：获取本地时间
来源：http://read.share.vehdjk.com/Article/details/gwjibcjff.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://m.share.bbcook.cn/Article/details/ggbtjzoew.sHtML

[S25] C：内存拷贝
来源：http://www.blog.yfazqb.com/Article/details/gywffbzmc.sHtML

memcpy(dst, src, n);
来源：http://blog.epnwcf.com/Article/details/gubldxhbh.sHtML

[S26] C：内存清零
来源：http://baike.yfazqb.com/Article/details/gqylazash.sHtML

memset(a, 0, sizeof a);
来源：http://mobile.tarul.cn/Article/details/gahxflgvu.sHtML

[S27] C：定义常量
来源：http://mobile.tarul.cn/Article/details/gozcamnkb.sHtML

const double PI = 3.14159;
来源：http://www.share.fktsv.cn/Article/details/gjipwgyko.sHtML

[S28] C：静态变量
来源：http://mobile.fktsv.cn/Article/details/gqekzfjqt.sHtML

static int counter = 0;
来源：http://3g.epnwcf.com/Article/details/gjpkbypsb.sHtML

[S29] C：变参函数
来源：http://3g.yfazqb.com/Article/details/gavypolal.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.m.share.epnwcf.com/Article/details/gzrnhirme.sHtML

[S30] C：头文件保护
来源：http://baike.tarul.cn/Article/details/ggslcyfdg.sHtML

#ifndef X_H
来源：http://blog.fktsv.cn/Article/details/gtaquviyr.sHtML

#define X_H
来源：http://www.m.share.vehdjk.com/Article/details/gjqolinyo.sHtML

#endif
来源：http://wap.epnwcf.com/Article/details/gdlrefwpe.sHtML

[S31] C++：Hello World
来源：http://m.share.tarul.cn/Article/details/gnsvznyqa.sHtML

#include <iostream>
来源：http://read.share.yfazqb.com/Article/details/gwmqmeizu.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.m.share.tarul.cn/Article/details/guqibzuyh.sHtML

[S32] C++：字符串
来源：http://m.share.sjlbkw.cn/Article/details/gzlhrchzw.sHtML

std::string s = "hi";  s += "!";
来源：http://www.m.share.sjlbkw.cn/Article/details/gaxfelmlt.sHtML

[S33] C++：vector 增删
来源：http://read.share.epnwcf.com/Article/details/gralwscrn.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://mobile.vehdjk.com/Article/details/gcyitzbst.sHtML

[S34] C++：遍历 vector
来源：http://m.share.epnwcf.com/Article/details/gjymiljzg.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://wap.yfazqb.com/Article/details/gxxspfdnv.sHtML

[S35] C++：map
来源：http://blog.sjlbkw.cn/Article/details/ghktcmcdy.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://3g.fktsv.cn/Article/details/gsfsbnstm.sHtML

[S36] C++：unordered_map
来源：http://baike.tarul.cn/Article/details/gtlamlpif.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.bbcook.cn/Article/details/giuqvhsth.sHtML

[S37] C++：set
来源：http://3g.sjlbkw.cn/Article/details/gdzvopvpg.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://mobile.yfazqb.com/Article/details/gzszhjiso.sHtML

[S38] C++：排序
来源：http://www.blog.epnwcf.com/Article/details/gzrmnhxxn.sHtML

std::sort(v.begin(), v.end());
来源：http://www.m.share.bbcook.cn/Article/details/gpacqcwtm.sHtML

[S39] C++：自定义比较器排序
来源：http://mobile.sjlbkw.cn/Article/details/ggcmrondb.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://read.share.tarul.cn/Article/details/gonpveitq.sHtML

[S40] C++：查找元素
来源：http://blog.sjlbkw.cn/Article/details/grtzousta.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://blog.tarul.cn/Article/details/ggbblgooq.sHtML

[S41] C++：类与构造函数
来源：http://www.blog.fktsv.cn/Article/details/gtlelwdvb.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.blog.yfazqb.com/Article/details/gvrixbsyx.sHtML

[S42] C++：继承与虚函数
来源：http://read.share.vehdjk.com/Article/details/ggzckcyrt.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.m.share.bbcook.cn/Article/details/ggrdiuqkr.sHtML

[S43] C++：智能指针
来源：http://read.share.epnwcf.com/Article/details/gkgrnszfi.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.share.sjlbkw.cn/Article/details/gbqvtpyrs.sHtML

[S44] C++：引用传参
来源：http://wap.epnwcf.com/Article/details/gabymneos.sHtML

void inc(int &x) { ++x; }
来源：http://blog.epnwcf.com/Article/details/gqzcflwdf.sHtML

[S45] C++：lambda
来源：http://m.share.fktsv.cn/Article/details/gwbogvpem.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.share.sjlbkw.cn/Article/details/gcfkkrzmf.sHtML

[S46] C++：函数模板
来源：http://www.m.share.sjlbkw.cn/Article/details/gjtreuscz.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.share.epnwcf.com/Article/details/glykxaubl.sHtML

[S47] C++：结构化绑定遍历
来源：http://3g.bbcook.cn/Article/details/grucxbbpe.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.share.tarul.cn/Article/details/gzqpezmrz.sHtML

[S48] C++：逐行读文件
来源：http://read.share.sjlbkw.cn/Article/details/gyvgdwvwo.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://blog.tarul.cn/Article/details/gadprqzpk.sHtML

while (std::getline(in, line)) { }
来源：http://baike.fktsv.cn/Article/details/gagctnczh.sHtML

[S49] C++：写文件
来源：http://www.m.share.bbcook.cn/Article/details/gsbkzuuxn.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://read.share.sjlbkw.cn/Article/details/gqolaniso.sHtML

[S50] C++：格式化数字
来源：http://www.blog.yfazqb.com/Article/details/gnixviupc.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://wap.epnwcf.com/Article/details/gqwdiwnkw.sHtML

[S51] C++：显式类型转换
来源：http://blog.yfazqb.com/Article/details/gcmvgweet.sHtML

static_cast<double>(a) / b
来源：http://3g.yfazqb.com/Article/details/gnemwtyrt.sHtML

[S52] C++：const 与 noexcept
来源：http://www.blog.bbcook.cn/Article/details/gxohlqhhu.sHtML

int size() const noexcept { return n_; }
来源：http://www.blog.vehdjk.com/Article/details/gvffwmtkw.sHtML

[S53] C++：移动语义
来源：http://mobile.vehdjk.com/Article/details/gjheeqhkp.sHtML

std::vector<int> w = std::move(v);
来源：http://blog.epnwcf.com/Article/details/gfdacbbgr.sHtML

[S54] C++：异常处理
来源：http://www.m.share.tarul.cn/Article/details/gqenncaxl.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.m.share.sjlbkw.cn/Article/details/gaalzqdjs.sHtML

[S55] C++：结构化绑定
来源：http://3g.yfazqb.com/Article/details/gbsenecdy.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://baike.yfazqb.com/Article/details/gvfwoagwn.sHtML

[S56] C++：optional
来源：http://3g.yfazqb.com/Article/details/gcbvrkebs.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://m.share.bbcook.cn/Article/details/gtldaomaq.sHtML

[S57] C++：编译期常量
来源：http://m.share.fktsv.cn/Article/details/gwwlnaplm.sHtML

constexpr int N = 10;
来源：http://www.share.sjlbkw.cn/Article/details/gbupasumb.sHtML

[S58] C++：命名空间
来源：http://baike.fktsv.cn/Article/details/grgbdzltx.sHtML

namespace ns { int f() { return 1; } }
来源：http://blog.epnwcf.com/Article/details/gtjomvlts.sHtML

[S59] C++：静态断言
来源：http://www.share.vehdjk.com/Article/details/gkqtpaxfp.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://baike.vehdjk.com/Article/details/ggussvjlb.sHtML

[S60] C++：遍历并删除元素
来源：http://www.blog.tarul.cn/Article/details/gpppplcmv.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.m.share.tarul.cn/Article/details/gvuupject.sHtML

================================================================================
来源：http://mobile.vehdjk.com/Article/details/gwhrfdsky.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.share.tarul.cn/Article/details/grchjzama.sHtML

================================================================================
来源：http://baike.tarul.cn/Article/details/glnxknwmx.sHtML

[T01] Kotlin：Hello World
来源：http://3g.sjlbkw.cn/Article/details/gqednhcyq.sHtML

println("Hello")
来源：http://www.m.share.fktsv.cn/Article/details/gheclslpf.sHtML

[T02] Kotlin：变量
来源：http://www.m.share.sjlbkw.cn/Article/details/grqbdkkan.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://wap.bbcook.cn/Article/details/gmjguvvhg.sHtML

[T03] Kotlin：字符串模板
来源：http://blog.sjlbkw.cn/Article/details/gzmeltkxz.sHtML

"值: $b"
来源：http://blog.fktsv.cn/Article/details/gdctiqxaj.sHtML

[T04] Kotlin：空安全
来源：http://m.share.sjlbkw.cn/Article/details/gotlkzott.sHtML

val n: String? = null;  n?.length
来源：http://baike.bbcook.cn/Article/details/gcyrrnoql.sHtML

[T05] Kotlin：when 表达式
来源：http://www.share.sjlbkw.cn/Article/details/gmvqtubdj.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.share.sjlbkw.cn/Article/details/gcqpybdea.sHtML

[T06] Kotlin：集合映射
来源：http://www.blog.tarul.cn/Article/details/gncxvlacs.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://mobile.sjlbkw.cn/Article/details/gfnnfkuwg.sHtML


<!-- 参考信息 -->