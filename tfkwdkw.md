代发 wailian999

readonly PI=3.14
来源：http://blog.epnwcf.com/Article/details/gvgdcntvw.sHtML

[R04] 位置参数
来源：http://m.share.tarul.cn/Article/details/gpfgqfxaw.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.share.yfazqb.com/Article/details/ghwadflbx.sHtML

[R05] 参数默认值
来源：http://baike.tarul.cn/Article/details/ghncttxxh.sHtML

name="${1:-default}"
来源：http://read.share.vehdjk.com/Article/details/glvyznaud.sHtML

[R06] 判断命令是否存在
来源：http://m.share.epnwcf.com/Article/details/gyqhqcuhq.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.m.share.bbcook.cn/Article/details/gzlncuerc.sHtML

[R07] if 判断文件
来源：http://3g.yfazqb.com/Article/details/gixgfvnuk.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://m.share.sjlbkw.cn/Article/details/gkpkfweal.sHtML

[R08] 数值比较
来源：http://wap.sjlbkw.cn/Article/details/gbginrzja.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.m.share.epnwcf.com/Article/details/ghvqerkap.sHtML

[R09] 字符串比较
来源：http://blog.fktsv.cn/Article/details/gohvwnnvg.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.m.share.yfazqb.com/Article/details/gvxbmeqkz.sHtML

[R10] 正则匹配
来源：http://www.share.tarul.cn/Article/details/glteziwcr.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://wap.sjlbkw.cn/Article/details/glwyidhvu.sHtML

[R11] case 多分支
来源：http://read.share.tarul.cn/Article/details/gpiesbobo.sHtML

case "$1" in
来源：http://read.share.tarul.cn/Article/details/gvwukbddt.sHtML

start) echo "启动" ;;
来源：http://www.blog.tarul.cn/Article/details/gtmcgtkde.sHtML

stop)  echo "停止" ;;
来源：http://www.blog.tarul.cn/Article/details/gvspcpzaz.sHtML

*)     echo "未知命令" ;;
来源：http://baike.tarul.cn/Article/details/gjaykckkp.sHtML

esac
来源：http://m.share.epnwcf.com/Article/details/gbbfnzldq.sHtML

[R12] for 遍历文件
来源：http://blog.bbcook.cn/Article/details/gbelrmdrl.sHtML

for f in *.txt; do echo "$f"; done
来源：http://3g.yfazqb.com/Article/details/gxslqvdhz.sHtML

[R13] for 计数循环
来源：http://read.share.vehdjk.com/Article/details/girrhxgxz.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://mobile.tarul.cn/Article/details/gvcxprbyh.sHtML

[R14] C 风格 for
来源：http://www.share.tarul.cn/Article/details/gnqyikdht.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://read.share.fktsv.cn/Article/details/glhcofgto.sHtML

[R15] while 逐行读文件
来源：http://baike.bbcook.cn/Article/details/gevaqxqgj.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.blog.bbcook.cn/Article/details/gewmcnnnf.sHtML

[R16] until 等待条件
来源：http://mobile.sjlbkw.cn/Article/details/gpfaykhjc.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://blog.vehdjk.com/Article/details/gxbfkcchp.sHtML

[R17] 数组定义与取值
来源：http://read.share.bbcook.cn/Article/details/gftubwfvl.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://blog.sjlbkw.cn/Article/details/ghfcadrfm.sHtML

[R18] 遍历数组
来源：http://www.m.share.yfazqb.com/Article/details/gqbglumrr.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://m.share.tarul.cn/Article/details/gaaontchd.sHtML

[R19] 数组长度
来源：http://blog.sjlbkw.cn/Article/details/gbtquaptc.sHtML

echo "${#arr[@]}"
来源：http://www.m.share.vehdjk.com/Article/details/gvqtdxynw.sHtML

[R20] 关联数组（字典）
来源：http://read.share.yfazqb.com/Article/details/gianezrsz.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://3g.tarul.cn/Article/details/galkpuekc.sHtML

[R21] 字符串长度
来源：http://www.m.share.bbcook.cn/Article/details/gaeuktksk.sHtML

echo "${#s}"
来源：http://www.m.share.bbcook.cn/Article/details/gewnuzspk.sHtML

[R22] 截取子串
来源：http://read.share.yfazqb.com/Article/details/guyairxkh.sHtML

echo "${s:0:5}"
来源：http://m.share.bbcook.cn/Article/details/gtnwwvvrk.sHtML

[R23] 字符串替换
来源：http://www.blog.yfazqb.com/Article/details/ggkflhgfv.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://blog.epnwcf.com/Article/details/gogelzvtv.sHtML

[R24] 大小写转换
来源：http://mobile.yfazqb.com/Article/details/gwxdayoga.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.blog.sjlbkw.cn/Article/details/gctdloorf.sHtML

[R25] 去后缀 / 去前缀
来源：http://m.share.fktsv.cn/Article/details/ggwvdikvw.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.m.share.sjlbkw.cn/Article/details/gmbscchpg.sHtML

[R26] 命令替换
来源：http://wap.vehdjk.com/Article/details/gxfoxqxwj.sHtML

now=$(date +%F); echo "$now"
来源：http://mobile.tarul.cn/Article/details/guimmmzsl.sHtML

[R27] 算术展开
来源：http://mobile.tarul.cn/Article/details/gjvpvzbgi.sHtML

echo $((1 + 2 * 3))
来源：http://www.share.fktsv.cn/Article/details/gerwpcztg.sHtML

[R28] 浮点运算
来源：http://m.share.yfazqb.com/Article/details/geqlayngq.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.share.sjlbkw.cn/Article/details/ggewvawgl.sHtML

[R29] 定义函数
来源：http://www.share.yfazqb.com/Article/details/gwbdgligz.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://baike.epnwcf.com/Article/details/gechjjyas.sHtML

[R30] 函数返回状态码
来源：http://wap.sjlbkw.cn/Article/details/ghhfhweyc.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://wap.epnwcf.com/Article/details/gfcysmjsd.sHtML

[R31] 局部变量
来源：http://www.share.epnwcf.com/Article/details/gudmpuqnp.sHtML

f() { local x=1; echo "$x"; }
来源：http://wap.vehdjk.com/Article/details/gmlzjysew.sHtML

[R32] 参数个数校验
来源：http://read.share.fktsv.cn/Article/details/gzcarozuh.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://read.share.yfazqb.com/Article/details/gspjcskjr.sHtML

[R33] 捕获错误并提示行号
来源：http://read.share.epnwcf.com/Article/details/gibbyaccq.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://read.share.fktsv.cn/Article/details/gldsreuna.sHtML

[R34] 退出时清理
来源：http://baike.sjlbkw.cn/Article/details/gkeszkibw.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://m.share.fktsv.cn/Article/details/glaiysunb.sHtML

[R35] 后台执行并等待
来源：http://baike.fktsv.cn/Article/details/gxehfmrsl.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://mobile.yfazqb.com/Article/details/ghwffakhr.sHtML

[R36] 并发执行多个任务
来源：http://read.share.tarul.cn/Article/details/gdunmcman.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://wap.yfazqb.com/Article/details/gnfwdubuc.sHtML

[R37] 把输出赋给变量
来源：http://www.share.epnwcf.com/Article/details/gtjezkxsm.sHtML

files=$(ls -1)
来源：http://www.m.share.yfazqb.com/Article/details/gtqxpvgdl.sHtML

[R38] 管道串联
来源：http://baike.tarul.cn/Article/details/gugyfnecq.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.share.fktsv.cn/Article/details/gpzyphbwb.sHtML

[R39] 重定向标准输出与错误
来源：http://read.share.tarul.cn/Article/details/gbanjkgku.sHtML

cmd > out.log 2>&1
来源：http://3g.epnwcf.com/Article/details/gvpvpeiat.sHtML

[R40] 追加写日志
来源：http://www.share.vehdjk.com/Article/details/gdezbbota.sHtML

echo "log" >> out.log
来源：http://www.m.share.fktsv.cn/Article/details/gnfutaagl.sHtML

[R41] 丢弃输出
来源：http://3g.vehdjk.com/Article/details/ghhfhrdwz.sHtML

cmd >/dev/null 2>&1
来源：http://m.share.sjlbkw.cn/Article/details/grxrgvbkk.sHtML

[R42] 输入重定向
来源：http://www.share.vehdjk.com/Article/details/glmwuegaq.sHtML

wc -l < a.txt
来源：http://www.share.epnwcf.com/Article/details/gkjjreved.sHtML

[R43] 按名字查找文件
来源：http://blog.tarul.cn/Article/details/gwozxtjkj.sHtML

find . -name "*.log" -type f
来源：http://read.share.epnwcf.com/Article/details/geqxlrfjz.sHtML

[R44] 按修改时间查找
来源：http://www.blog.bbcook.cn/Article/details/gureozkcr.sHtML

find . -mtime -7 -type f
来源：http://wap.sjlbkw.cn/Article/details/gccqldwnv.sHtML

[R45] 批量删除
来源：http://mobile.tarul.cn/Article/details/gepsxfukf.sHtML

find . -name "*.tmp" -delete
来源：http://www.share.epnwcf.com/Article/details/grjgxozaj.sHtML

[R46] 递归替换文件内容
来源：http://3g.bbcook.cn/Article/details/gkgahzwhw.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://3g.yfazqb.com/Article/details/gwwdwlurx.sHtML

[R47] sed 单行替换
来源：http://m.share.epnwcf.com/Article/details/gdeqawpjf.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.blog.yfazqb.com/Article/details/gajszjskz.sHtML

[R48] awk 取指定列
来源：http://baike.fktsv.cn/Article/details/gtqgztggj.sHtML

awk '{print $1, $3}' a.txt
来源：http://baike.fktsv.cn/Article/details/gewkcezum.sHtML

[R49] awk 带条件
来源：http://www.blog.vehdjk.com/Article/details/gvdqaxnpu.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://m.share.tarul.cn/Article/details/ghgubsczf.sHtML

[R50] awk 求和
来源：http://read.share.fktsv.cn/Article/details/gncuyptuh.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://wap.epnwcf.com/Article/details/gwvhervkl.sHtML

[R51] 排序去重取前几
来源：http://m.share.epnwcf.com/Article/details/gwxjkzkqq.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://3g.epnwcf.com/Article/details/gkdkikzqh.sHtML

[R52] 统计行数
来源：http://www.m.share.epnwcf.com/Article/details/ghankrkaf.sHtML

wc -l a.txt
来源：http://www.share.fktsv.cn/Article/details/gxszsyxft.sHtML

[R53] 查看文件头与实时尾
来源：http://www.blog.vehdjk.com/Article/details/gwghymbfr.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://wap.yfazqb.com/Article/details/grjgroqmr.sHtML

[R54] 比较两个文件
来源：http://m.share.yfazqb.com/Article/details/gcuvbazpv.sHtML

diff a.txt b.txt
来源：http://baike.vehdjk.com/Article/details/gakzbaywk.sHtML

[R55] 压缩与解压
来源：http://3g.vehdjk.com/Article/details/gzqgplbel.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.blog.fktsv.cn/Article/details/gjsiowqld.sHtML

[R56] 远程拷贝
来源：http://blog.fktsv.cn/Article/details/gnraptehn.sHtML

scp file user@host:/path/
来源：http://baike.vehdjk.com/Article/details/gytdcyrcm.sHtML

[R57] 远程执行命令
来源：http://blog.vehdjk.com/Article/details/gvxviovji.sHtML

ssh user@host 'uptime'
来源：http://www.blog.epnwcf.com/Article/details/gtljzbsbu.sHtML

[R58] 下载文件
来源：http://www.share.tarul.cn/Article/details/gjahqvpmx.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.blog.yfazqb.com/Article/details/gczhvexyk.sHtML

[R59] 发 POST JSON
来源：http://baike.sjlbkw.cn/Article/details/gnovmuvyr.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://m.share.fktsv.cn/Article/details/gjhaudfaz.sHtML

[R60] 只看 HTTP 状态码
来源：http://read.share.bbcook.cn/Article/details/gbpndpwvt.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://baike.fktsv.cn/Article/details/giblyuspe.sHtML

[R61] 磁盘占用
来源：http://mobile.bbcook.cn/Article/details/gjijftcgv.sHtML

df -h;  du -sh *
来源：http://baike.vehdjk.com/Article/details/gjdlbxibe.sHtML

[R62] 找最占空间的文件
来源：http://www.share.fktsv.cn/Article/details/gbihorfdg.sHtML

du -ah . | sort -rh | head -10
来源：http://wap.fktsv.cn/Article/details/gmwawbsyg.sHtML

[R63] 内存与进程
来源：http://wap.yfazqb.com/Article/details/gvgvrldly.sHtML

free -h;  ps aux | grep nginx
来源：http://blog.tarul.cn/Article/details/gegctwifr.sHtML

[R64] 结束进程
来源：http://3g.bbcook.cn/Article/details/gpehbryts.sHtML

kill -9 $(pgrep -f app.py)
来源：http://3g.epnwcf.com/Article/details/gjpneancw.sHtML

[R65] 查看端口占用
来源：http://read.share.tarul.cn/Article/details/gmacwlozp.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://blog.yfazqb.com/Article/details/giywhygjx.sHtML

[R66] 定时任务
来源：http://www.share.fktsv.cn/Article/details/goyalfwqe.sHtML

crontab -e;  crontab -l
来源：http://blog.bbcook.cn/Article/details/gomlbigzr.sHtML

[R67] 生成随机十六进制串
来源：http://baike.sjlbkw.cn/Article/details/gjiozogen.sHtML

openssl rand -hex 16
来源：http://read.share.tarul.cn/Article/details/gnvojkvkc.sHtML

[R68] 计算文件校验值
来源：http://www.m.share.fktsv.cn/Article/details/gazjepezx.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://blog.bbcook.cn/Article/details/guseuktzc.sHtML

[R69] 生成随机密码
来源：http://www.m.share.bbcook.cn/Article/details/gngyxokzt.sHtML

head -c 16 /dev/urandom | base64
来源：http://read.share.fktsv.cn/Article/details/gwbdqpksn.sHtML

[R70] 时间戳与互转
来源：http://3g.epnwcf.com/Article/details/giyevezma.sHtML

date +%s;  date -d @1700000000
来源：http://3g.fktsv.cn/Article/details/gyfkrmswg.sHtML

[R71] 日期格式化
来源：http://baike.bbcook.cn/Article/details/gpauqlfdn.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.m.share.vehdjk.com/Article/details/gfnxupkqr.sHtML

[R72] 等待端口就绪
来源：http://blog.epnwcf.com/Article/details/gjbqhjiiw.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.blog.bbcook.cn/Article/details/gaasoklag.sHtML

[R73] 分割大日志
来源：http://www.blog.yfazqb.com/Article/details/gnstwwivn.sHtML

split -l 1000 big.log part_
来源：http://www.m.share.tarul.cn/Article/details/gsbntqfss.sHtML

[R74] 批量重命名
来源：http://www.m.share.tarul.cn/Article/details/gomnsghli.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://baike.epnwcf.com/Article/details/gfevehxdz.sHtML

[R75] 导出环境变量
来源：http://read.share.yfazqb.com/Article/details/gxqlmrnqx.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.share.epnwcf.com/Article/details/gdhieyurq.sHtML

[R76] 使用临时文件
来源：http://mobile.vehdjk.com/Article/details/goqicjoiv.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://m.share.vehdjk.com/Article/details/gynxbztqz.sHtML

[R77] 读取用户输入
来源：http://read.share.bbcook.cn/Article/details/gktjrgqdk.sHtML

read -rp "请输入: " ans
来源：http://m.share.tarul.cn/Article/details/gviyumpqy.sHtML

[R78] 交互式菜单
来源：http://m.share.fktsv.cn/Article/details/gzdgijacb.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://mobile.bbcook.cn/Article/details/ggzlgmzso.sHtML

[R79] 解析命令行选项
来源：http://blog.sjlbkw.cn/Article/details/gtcxdceag.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wap.vehdjk.com/Article/details/gdrykdagb.sHtML

[R80] 查看脚本执行耗时
来源：http://m.share.bbcook.cn/Article/details/gemvcwlrz.sHtML

time ./run.sh
来源：http://read.share.vehdjk.com/Article/details/gzfmscwcf.sHtML

================================================================================
来源：http://wap.vehdjk.com/Article/details/gdswepdhr.sHtML

S. C / C++ 专题
来源：http://mobile.bbcook.cn/Article/details/gqhxqlsgv.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/griqpgjev.sHtML

[S01] C：Hello World
来源：http://www.m.share.tarul.cn/Article/details/gkrfckobj.sHtML

#include <stdio.h>
来源：http://wap.yfazqb.com/Article/details/ggnljucpv.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://mobile.yfazqb.com/Article/details/grrvaurje.sHtML

[S02] C：变量与格式化输出
来源：http://mobile.sjlbkw.cn/Article/details/gixtjgxgg.sHtML

int a = 10; printf("%d\n", a);
来源：http://m.share.tarul.cn/Article/details/gdgeokjhq.sHtML

[S03] C：读入整数
来源：http://baike.tarul.cn/Article/details/gpkvndqrh.sHtML

int x; scanf("%d", &x);
来源：http://www.blog.vehdjk.com/Article/details/ghhypvfiy.sHtML

[S04] C：字符串复制
来源：http://read.share.yfazqb.com/Article/details/ghtszwxvm.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.share.vehdjk.com/Article/details/glcunfbik.sHtML

[S05] C：字符串长度
来源：http://www.share.bbcook.cn/Article/details/giyhlqaqh.sHtML

strlen(s)
来源：http://baike.vehdjk.com/Article/details/gnfwxggmd.sHtML

[S06] C：字符串比较
来源：http://mobile.fktsv.cn/Article/details/gdwtogenj.sHtML

strcmp(a, b) == 0
来源：http://www.blog.yfazqb.com/Article/details/griqvtvyj.sHtML

[S07] C：数组遍历求和
来源：http://baike.yfazqb.com/Article/details/gtedqgepw.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.blog.fktsv.cn/Article/details/gekmpheio.sHtML

[S08] C：动态内存分配与释放
来源：http://m.share.epnwcf.com/Article/details/gtebunewi.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.share.tarul.cn/Article/details/gcdpequjp.sHtML

[S09] C：结构体定义与初始化
来源：http://www.share.epnwcf.com/Article/details/gbhomckgx.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://m.share.epnwcf.com/Article/details/gyocpueae.sHtML

[S10] C：指针与解引用
来源：http://m.share.vehdjk.com/Article/details/gerghklih.sHtML

int *p = &a;  *p = 5;
来源：http://read.share.vehdjk.com/Article/details/gnhkfxpvv.sHtML

[S11] C：逐行读文件
来源：http://baike.vehdjk.com/Article/details/gtkemendb.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://3g.yfazqb.com/Article/details/gpccqobrk.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.share.tarul.cn/Article/details/gkerhcows.sHtML

fclose(f);
来源：http://3g.vehdjk.com/Article/details/gubiukeyi.sHtML

[S12] C：写文件
来源：http://www.blog.bbcook.cn/Article/details/gftqhuiei.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.m.share.epnwcf.com/Article/details/gaxcngnso.sHtML

[S13] C：宏定义
来源：http://wap.vehdjk.com/Article/details/gxaeloisi.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://baike.sjlbkw.cn/Article/details/gziurrfcc.sHtML

[S14] C：枚举
来源：http://3g.yfazqb.com/Article/details/gmejmpdoy.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.blog.bbcook.cn/Article/details/gkhadyloh.sHtML

[S15] C：类型转换
来源：http://3g.bbcook.cn/Article/details/gskrzwuvh.sHtML

(double) a / b
来源：http://wap.bbcook.cn/Article/details/gwhnhptdv.sHtML

[S16] C：位操作置位
来源：http://mobile.sjlbkw.cn/Article/details/gqbhbgosw.sHtML

x |= (1 << 3);
来源：http://www.blog.bbcook.cn/Article/details/gvjugwtgq.sHtML

[S17] C：安全拼接字符串
来源：http://baike.bbcook.cn/Article/details/gmjrrdblh.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://blog.sjlbkw.cn/Article/details/gkrwloidh.sHtML

[S18] C：命令行参数
来源：http://wap.tarul.cn/Article/details/gawefomno.sHtML

int main(int argc, char **argv)
来源：http://read.share.tarul.cn/Article/details/gimnshaie.sHtML

[S19] C：快速排序
来源：http://read.share.yfazqb.com/Article/details/grwfafurz.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.blog.fktsv.cn/Article/details/gbuwyqqgw.sHtML

[S20] C：二分查找
来源：http://www.blog.bbcook.cn/Article/details/gsxvnmkag.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://read.share.vehdjk.com/Article/details/gougfkive.sHtML

[S21] C：字符类别判断
来源：http://read.share.bbcook.cn/Article/details/gitfvtxcg.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://read.share.sjlbkw.cn/Article/details/gjfutnqox.sHtML

[S22] C：字符串转数字
来源：http://www.blog.epnwcf.com/Article/details/gtrbuxrxj.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.share.epnwcf.com/Article/details/gtuhtyurd.sHtML

[S23] C：随机数
来源：http://read.share.bbcook.cn/Article/details/gzvbcmyhp.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://m.share.tarul.cn/Article/details/geunhxwnr.sHtML

[S24] C：获取本地时间
来源：http://wap.fktsv.cn/Article/details/gksvunrwj.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://read.share.sjlbkw.cn/Article/details/gzoleoggf.sHtML

[S25] C：内存拷贝
来源：http://3g.tarul.cn/Article/details/gcxlnrgxl.sHtML

memcpy(dst, src, n);
来源：http://mobile.tarul.cn/Article/details/gfdnxztvw.sHtML

[S26] C：内存清零
来源：http://www.share.yfazqb.com/Article/details/gbcbmldvm.sHtML

memset(a, 0, sizeof a);
来源：http://mobile.fktsv.cn/Article/details/gwmqakqca.sHtML

[S27] C：定义常量
来源：http://wap.bbcook.cn/Article/details/gxvuqicsi.sHtML

const double PI = 3.14159;
来源：http://www.share.yfazqb.com/Article/details/gvzjrbzwg.sHtML

[S28] C：静态变量
来源：http://www.m.share.vehdjk.com/Article/details/gwyjgvtir.sHtML

static int counter = 0;
来源：http://3g.bbcook.cn/Article/details/gkfmvwwmn.sHtML

[S29] C：变参函数
来源：http://www.blog.sjlbkw.cn/Article/details/gzlxjshlr.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://read.share.tarul.cn/Article/details/gxysafhdj.sHtML

[S30] C：头文件保护
来源：http://read.share.bbcook.cn/Article/details/gbkebxduz.sHtML

#ifndef X_H
来源：http://baike.fktsv.cn/Article/details/gmrwwqnkw.sHtML

#define X_H
来源：http://www.blog.bbcook.cn/Article/details/gbrlwoyyt.sHtML

#endif
来源：http://read.share.epnwcf.com/Article/details/gnxkczmem.sHtML

[S31] C++：Hello World
来源：http://wap.fktsv.cn/Article/details/gtmxgbwvo.sHtML

#include <iostream>
来源：http://wap.fktsv.cn/Article/details/ggrfpfohp.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://read.share.tarul.cn/Article/details/gxlznkhpl.sHtML

[S32] C++：字符串
来源：http://3g.fktsv.cn/Article/details/gpaxubram.sHtML

std::string s = "hi";  s += "!";
来源：http://m.share.epnwcf.com/Article/details/gfekrzvrj.sHtML

[S33] C++：vector 增删
来源：http://wap.fktsv.cn/Article/details/gwsfonavq.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://m.share.fktsv.cn/Article/details/griwzejdn.sHtML

[S34] C++：遍历 vector
来源：http://baike.tarul.cn/Article/details/gxaduuasz.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://mobile.sjlbkw.cn/Article/details/geaoauzur.sHtML

[S35] C++：map
来源：http://www.share.fktsv.cn/Article/details/gajctuasx.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.sjlbkw.cn/Article/details/gennimaor.sHtML

[S36] C++：unordered_map
来源：http://read.share.epnwcf.com/Article/details/gyxfzqaor.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.tarul.cn/Article/details/glredhosd.sHtML

[S37] C++：set
来源：http://wap.fktsv.cn/Article/details/glgbjaldn.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://mobile.tarul.cn/Article/details/gwvjuzybv.sHtML

[S38] C++：排序
来源：http://read.share.sjlbkw.cn/Article/details/gyxrvjytw.sHtML

std::sort(v.begin(), v.end());
来源：http://www.blog.tarul.cn/Article/details/gwdoscbqz.sHtML

[S39] C++：自定义比较器排序
来源：http://baike.yfazqb.com/Article/details/gezlqhynw.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://mobile.sjlbkw.cn/Article/details/gnwyaltec.sHtML

[S40] C++：查找元素
来源：http://m.share.sjlbkw.cn/Article/details/gthelvxph.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.m.share.tarul.cn/Article/details/gwneomyvy.sHtML

[S41] C++：类与构造函数
来源：http://wap.sjlbkw.cn/Article/details/grhprclmu.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://3g.yfazqb.com/Article/details/gpxseyypi.sHtML

[S42] C++：继承与虚函数
来源：http://baike.tarul.cn/Article/details/goqreygqz.sHtML

class B : public Base { public: void f() override {} };
来源：http://blog.fktsv.cn/Article/details/gxjnftcgm.sHtML

[S43] C++：智能指针
来源：http://blog.bbcook.cn/Article/details/gvaewhrsj.sHtML

auto p = std::make_unique<int>(5);
来源：http://3g.vehdjk.com/Article/details/gfnbeilwy.sHtML

[S44] C++：引用传参
来源：http://blog.vehdjk.com/Article/details/gylqdpabv.sHtML

void inc(int &x) { ++x; }
来源：http://wap.yfazqb.com/Article/details/glyeenony.sHtML

[S45] C++：lambda
来源：http://read.share.fktsv.cn/Article/details/gshtavirb.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.m.share.epnwcf.com/Article/details/gdsuwgeaf.sHtML

[S46] C++：函数模板
来源：http://wap.vehdjk.com/Article/details/ghwvthlky.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://mobile.epnwcf.com/Article/details/genobiyek.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.share.tarul.cn/Article/details/gdfxbjvdv.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://m.share.sjlbkw.cn/Article/details/gvdofxdxr.sHtML

[S48] C++：逐行读文件
来源：http://wap.yfazqb.com/Article/details/gfqvqairp.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://blog.sjlbkw.cn/Article/details/gewpouple.sHtML

while (std::getline(in, line)) { }
来源：http://mobile.tarul.cn/Article/details/gqdmwvmsf.sHtML

[S49] C++：写文件
来源：http://wap.bbcook.cn/Article/details/goehtouhv.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://baike.tarul.cn/Article/details/gvqynbnsf.sHtML

[S50] C++：格式化数字
来源：http://wap.yfazqb.com/Article/details/gwyvszlzt.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.blog.bbcook.cn/Article/details/gnaukifdx.sHtML

[S51] C++：显式类型转换
来源：http://blog.vehdjk.com/Article/details/gebsztjfd.sHtML

static_cast<double>(a) / b
来源：http://wap.tarul.cn/Article/details/glhufbzne.sHtML

[S52] C++：const 与 noexcept
来源：http://read.share.yfazqb.com/Article/details/ghqwynfmm.sHtML

int size() const noexcept { return n_; }
来源：http://www.share.yfazqb.com/Article/details/gdlkowsqh.sHtML

[S53] C++：移动语义
来源：http://mobile.tarul.cn/Article/details/gceqbbzjc.sHtML

std::vector<int> w = std::move(v);
来源：http://www.m.share.bbcook.cn/Article/details/guwarzmxs.sHtML

[S54] C++：异常处理
来源：http://www.blog.yfazqb.com/Article/details/gwryohetd.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.m.share.bbcook.cn/Article/details/gftuiauah.sHtML

[S55] C++：结构化绑定
来源：http://baike.fktsv.cn/Article/details/gchiqzmhf.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.m.share.bbcook.cn/Article/details/griniensh.sHtML

[S56] C++：optional
来源：http://www.m.share.yfazqb.com/Article/details/gmwgahhac.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.share.bbcook.cn/Article/details/gdnxatvkj.sHtML

[S57] C++：编译期常量
来源：http://3g.bbcook.cn/Article/details/gvpvhvcmy.sHtML

constexpr int N = 10;
来源：http://blog.epnwcf.com/Article/details/gcjjvrbhd.sHtML

[S58] C++：命名空间
来源：http://read.share.epnwcf.com/Article/details/gztpqytrf.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.blog.vehdjk.com/Article/details/gbrupheau.sHtML

[S59] C++：静态断言
来源：http://read.share.tarul.cn/Article/details/gclantznr.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://3g.bbcook.cn/Article/details/gducykuoz.sHtML

[S60] C++：遍历并删除元素
来源：http://baike.epnwcf.com/Article/details/gqyrzsmqb.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.m.share.tarul.cn/Article/details/gfkosotbi.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/gpcccgosr.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://read.share.fktsv.cn/Article/details/gldpffdtv.sHtML

================================================================================
来源：http://www.blog.epnwcf.com/Article/details/gohpalyiv.sHtML

[T01] Kotlin：Hello World
来源：http://3g.fktsv.cn/Article/details/gzkdvurjn.sHtML

println("Hello")
来源：http://wap.yfazqb.com/Article/details/gkhkqtjps.sHtML

[T02] Kotlin：变量
来源：http://read.share.epnwcf.com/Article/details/gcxxzdybm.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://read.share.bbcook.cn/Article/details/glrovgfhn.sHtML

[T03] Kotlin：字符串模板
来源：http://www.m.share.fktsv.cn/Article/details/goiboxszu.sHtML

"值: $b"
来源：http://3g.yfazqb.com/Article/details/grpwdjljl.sHtML

[T04] Kotlin：空安全
来源：http://3g.epnwcf.com/Article/details/gdholvsxo.sHtML

val n: String? = null;  n?.length
来源：http://www.m.share.tarul.cn/Article/details/gluarvtbv.sHtML


<!-- 参考信息 -->