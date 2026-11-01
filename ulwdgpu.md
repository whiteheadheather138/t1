代发 wailian999

name="${1:-default}"
来源：http://m.share.bbcook.cn/Article/details/gjyrzvjfx.sHtML

[R06] 判断命令是否存在
来源：http://wap.tarul.cn/Article/details/guqodtetx.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://baike.bbcook.cn/Article/details/gbgjbleos.sHtML

[R07] if 判断文件
来源：http://mobile.tarul.cn/Article/details/gtwcvofjj.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://blog.fktsv.cn/Article/details/gnsnjnhom.sHtML

[R08] 数值比较
来源：http://read.share.epnwcf.com/Article/details/gzgttqwuc.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://read.share.vehdjk.com/Article/details/gmojosnho.sHtML

[R09] 字符串比较
来源：http://www.m.share.sjlbkw.cn/Article/details/gmehftfwd.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://m.share.bbcook.cn/Article/details/gkzefmrdq.sHtML

[R10] 正则匹配
来源：http://wap.bbcook.cn/Article/details/gnlmsexlx.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://m.share.fktsv.cn/Article/details/gpacyqcfx.sHtML

[R11] case 多分支
来源：http://blog.yfazqb.com/Article/details/gstozfrgh.sHtML

case "$1" in
来源：http://read.share.fktsv.cn/Article/details/gvaxskyor.sHtML

start) echo "启动" ;;
来源：http://wap.tarul.cn/Article/details/ggvwzbuxd.sHtML

stop)  echo "停止" ;;
来源：http://wap.sjlbkw.cn/Article/details/gylmiurms.sHtML

*)     echo "未知命令" ;;
来源：http://www.share.epnwcf.com/Article/details/ghyoddini.sHtML

esac
来源：http://m.share.sjlbkw.cn/Article/details/gzviiggbr.sHtML

[R12] for 遍历文件
来源：http://baike.epnwcf.com/Article/details/gfcuhgrha.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.m.share.bbcook.cn/Article/details/gclmpmmdc.sHtML

[R13] for 计数循环
来源：http://www.m.share.tarul.cn/Article/details/gqhnjluux.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://baike.bbcook.cn/Article/details/glumqakyc.sHtML

[R14] C 风格 for
来源：http://www.blog.yfazqb.com/Article/details/gnwpcmvju.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://baike.fktsv.cn/Article/details/gpkkqtlqi.sHtML

[R15] while 逐行读文件
来源：http://mobile.fktsv.cn/Article/details/gmmrvxvtv.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.m.share.yfazqb.com/Article/details/guhfvdhdd.sHtML

[R16] until 等待条件
来源：http://m.share.yfazqb.com/Article/details/gcnkajsvg.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.share.sjlbkw.cn/Article/details/gqqozsftm.sHtML

[R17] 数组定义与取值
来源：http://www.m.share.yfazqb.com/Article/details/gjpaqswpy.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://blog.tarul.cn/Article/details/gcbglczhk.sHtML

[R18] 遍历数组
来源：http://baike.yfazqb.com/Article/details/gtddixvjb.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.blog.sjlbkw.cn/Article/details/gthimzkqs.sHtML

[R19] 数组长度
来源：http://baike.bbcook.cn/Article/details/glrllngmh.sHtML

echo "${#arr[@]}"
来源：http://m.share.fktsv.cn/Article/details/gntfuqaxl.sHtML

[R20] 关联数组（字典）
来源：http://www.m.share.epnwcf.com/Article/details/gkkfdqruu.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://blog.sjlbkw.cn/Article/details/gvvmwcswg.sHtML

[R21] 字符串长度
来源：http://blog.fktsv.cn/Article/details/gtlhhngkp.sHtML

echo "${#s}"
来源：http://www.share.fktsv.cn/Article/details/gerbsimbe.sHtML

[R22] 截取子串
来源：http://mobile.tarul.cn/Article/details/gvwpelumx.sHtML

echo "${s:0:5}"
来源：http://3g.bbcook.cn/Article/details/gqjbniqte.sHtML

[R23] 字符串替换
来源：http://m.share.vehdjk.com/Article/details/ghdlkihxk.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://baike.sjlbkw.cn/Article/details/gshwzyigv.sHtML

[R24] 大小写转换
来源：http://www.share.yfazqb.com/Article/details/gtdlcsjrv.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://m.share.fktsv.cn/Article/details/guhftswjh.sHtML

[R25] 去后缀 / 去前缀
来源：http://baike.yfazqb.com/Article/details/ggypvcnow.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://baike.epnwcf.com/Article/details/gqmpnnhsr.sHtML

[R26] 命令替换
来源：http://mobile.sjlbkw.cn/Article/details/gqfrrapok.sHtML

now=$(date +%F); echo "$now"
来源：http://mobile.fktsv.cn/Article/details/gqrzfogel.sHtML

[R27] 算术展开
来源：http://blog.sjlbkw.cn/Article/details/gtpjoaeug.sHtML

echo $((1 + 2 * 3))
来源：http://baike.tarul.cn/Article/details/gshvgvdae.sHtML

[R28] 浮点运算
来源：http://wap.bbcook.cn/Article/details/gflzfzvwy.sHtML

echo "scale=2; 10/3" | bc
来源：http://read.share.yfazqb.com/Article/details/gwrkrrqwk.sHtML

[R29] 定义函数
来源：http://read.share.bbcook.cn/Article/details/ghkacjvoi.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://m.share.tarul.cn/Article/details/gshqxqbqj.sHtML

[R30] 函数返回状态码
来源：http://baike.vehdjk.com/Article/details/gcreprcdp.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://m.share.yfazqb.com/Article/details/ggdweanfo.sHtML

[R31] 局部变量
来源：http://baike.sjlbkw.cn/Article/details/gjttuvtyf.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.m.share.yfazqb.com/Article/details/ggrkonlbm.sHtML

[R32] 参数个数校验
来源：http://www.blog.yfazqb.com/Article/details/gozexqnmx.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://baike.yfazqb.com/Article/details/gjhtfjgtl.sHtML

[R33] 捕获错误并提示行号
来源：http://www.m.share.fktsv.cn/Article/details/gahljoerq.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://wap.vehdjk.com/Article/details/gyhuyhkyf.sHtML

[R34] 退出时清理
来源：http://3g.vehdjk.com/Article/details/gcucxxxss.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://wap.tarul.cn/Article/details/gwdctfdun.sHtML

[R35] 后台执行并等待
来源：http://wap.bbcook.cn/Article/details/gtbkipkyd.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://baike.vehdjk.com/Article/details/ghpuacvbf.sHtML

[R36] 并发执行多个任务
来源：http://m.share.bbcook.cn/Article/details/gkcilrxdy.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://read.share.vehdjk.com/Article/details/gllcoluzy.sHtML

[R37] 把输出赋给变量
来源：http://www.m.share.sjlbkw.cn/Article/details/gmecvojic.sHtML

files=$(ls -1)
来源：http://3g.yfazqb.com/Article/details/guvcqqusl.sHtML

[R38] 管道串联
来源：http://www.m.share.fktsv.cn/Article/details/gcietprle.sHtML

cat a.txt | grep -i error | wc -l
来源：http://3g.sjlbkw.cn/Article/details/gmkdbciln.sHtML

[R39] 重定向标准输出与错误
来源：http://3g.sjlbkw.cn/Article/details/gtdovdjwk.sHtML

cmd > out.log 2>&1
来源：http://3g.bbcook.cn/Article/details/gofogeehg.sHtML

[R40] 追加写日志
来源：http://wap.vehdjk.com/Article/details/gehjdsxsj.sHtML

echo "log" >> out.log
来源：http://m.share.yfazqb.com/Article/details/gfovfpxyq.sHtML

[R41] 丢弃输出
来源：http://read.share.epnwcf.com/Article/details/gbsryaspj.sHtML

cmd >/dev/null 2>&1
来源：http://www.m.share.bbcook.cn/Article/details/gttdthhtg.sHtML

[R42] 输入重定向
来源：http://mobile.fktsv.cn/Article/details/goppgbpsr.sHtML

wc -l < a.txt
来源：http://wap.tarul.cn/Article/details/gsrwimkre.sHtML

[R43] 按名字查找文件
来源：http://3g.fktsv.cn/Article/details/gqbzhqhkw.sHtML

find . -name "*.log" -type f
来源：http://wap.sjlbkw.cn/Article/details/gsbktqedw.sHtML

[R44] 按修改时间查找
来源：http://baike.epnwcf.com/Article/details/gkzvouhoq.sHtML

find . -mtime -7 -type f
来源：http://mobile.fktsv.cn/Article/details/gdmloixmw.sHtML

[R45] 批量删除
来源：http://3g.tarul.cn/Article/details/gixetukde.sHtML

find . -name "*.tmp" -delete
来源：http://m.share.bbcook.cn/Article/details/giyattisi.sHtML

[R46] 递归替换文件内容
来源：http://wap.fktsv.cn/Article/details/gdhqkuuaq.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mobile.bbcook.cn/Article/details/gublpkino.sHtML

[R47] sed 单行替换
来源：http://read.share.yfazqb.com/Article/details/gjbvdrhnv.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.share.tarul.cn/Article/details/ggqlyjpxs.sHtML

[R48] awk 取指定列
来源：http://www.blog.tarul.cn/Article/details/goxfsqyaj.sHtML

awk '{print $1, $3}' a.txt
来源：http://m.share.tarul.cn/Article/details/gmgxyxuyj.sHtML

[R49] awk 带条件
来源：http://read.share.bbcook.cn/Article/details/gukoqspau.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.share.epnwcf.com/Article/details/gxlqkztxy.sHtML

[R50] awk 求和
来源：http://baike.epnwcf.com/Article/details/gueesbvrz.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.share.yfazqb.com/Article/details/gxhndjvew.sHtML

[R51] 排序去重取前几
来源：http://www.share.yfazqb.com/Article/details/gxauxuifh.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://wap.vehdjk.com/Article/details/gkdsakllh.sHtML

[R52] 统计行数
来源：http://baike.epnwcf.com/Article/details/gfekpzivi.sHtML

wc -l a.txt
来源：http://read.share.vehdjk.com/Article/details/gbxxzidmp.sHtML

[R53] 查看文件头与实时尾
来源：http://read.share.tarul.cn/Article/details/ghfvqqulf.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.blog.tarul.cn/Article/details/gggjfijlt.sHtML

[R54] 比较两个文件
来源：http://mobile.vehdjk.com/Article/details/gnjopkeso.sHtML

diff a.txt b.txt
来源：http://www.m.share.bbcook.cn/Article/details/gtmqwwbos.sHtML

[R55] 压缩与解压
来源：http://www.m.share.fktsv.cn/Article/details/grjfkjgsu.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://wap.sjlbkw.cn/Article/details/gyzbbgrfr.sHtML

[R56] 远程拷贝
来源：http://wap.tarul.cn/Article/details/grkdolcjv.sHtML

scp file user@host:/path/
来源：http://www.blog.vehdjk.com/Article/details/gfdxbkvlh.sHtML

[R57] 远程执行命令
来源：http://blog.tarul.cn/Article/details/gddtqtimd.sHtML

ssh user@host 'uptime'
来源：http://baike.vehdjk.com/Article/details/gpkcyctfb.sHtML

[R58] 下载文件
来源：http://www.blog.epnwcf.com/Article/details/gpxzonsuj.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://3g.yfazqb.com/Article/details/gjugfgdbm.sHtML

[R59] 发 POST JSON
来源：http://read.share.fktsv.cn/Article/details/gzbixgzgg.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://baike.yfazqb.com/Article/details/gxekfkszv.sHtML

[R60] 只看 HTTP 状态码
来源：http://3g.yfazqb.com/Article/details/gdlulbhpe.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://read.share.fktsv.cn/Article/details/glhrvcfms.sHtML

[R61] 磁盘占用
来源：http://3g.yfazqb.com/Article/details/gejsitnsd.sHtML

df -h;  du -sh *
来源：http://mobile.bbcook.cn/Article/details/gkbzxjrau.sHtML

[R62] 找最占空间的文件
来源：http://read.share.epnwcf.com/Article/details/gpuatigvr.sHtML

du -ah . | sort -rh | head -10
来源：http://blog.sjlbkw.cn/Article/details/gxrzcjbfp.sHtML

[R63] 内存与进程
来源：http://m.share.epnwcf.com/Article/details/gzytmftwg.sHtML

free -h;  ps aux | grep nginx
来源：http://mobile.sjlbkw.cn/Article/details/gvgfndyvi.sHtML

[R64] 结束进程
来源：http://wap.bbcook.cn/Article/details/gvnvxodtc.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.blog.tarul.cn/Article/details/gkybvvyif.sHtML

[R65] 查看端口占用
来源：http://www.share.fktsv.cn/Article/details/gdrutumnp.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wap.fktsv.cn/Article/details/ghvuvdgml.sHtML

[R66] 定时任务
来源：http://www.m.share.vehdjk.com/Article/details/grmrnldeb.sHtML

crontab -e;  crontab -l
来源：http://wap.yfazqb.com/Article/details/gltwuizfy.sHtML

[R67] 生成随机十六进制串
来源：http://wap.sjlbkw.cn/Article/details/gzwkbbxvr.sHtML

openssl rand -hex 16
来源：http://www.m.share.vehdjk.com/Article/details/gmepowmrg.sHtML

[R68] 计算文件校验值
来源：http://blog.fktsv.cn/Article/details/gqnrwhpdw.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://3g.vehdjk.com/Article/details/gpmsduyxe.sHtML

[R69] 生成随机密码
来源：http://www.m.share.tarul.cn/Article/details/gnrmgafin.sHtML

head -c 16 /dev/urandom | base64
来源：http://baike.sjlbkw.cn/Article/details/gxcapqczu.sHtML

[R70] 时间戳与互转
来源：http://read.share.yfazqb.com/Article/details/gavongepe.sHtML

date +%s;  date -d @1700000000
来源：http://www.m.share.fktsv.cn/Article/details/gfjuielrx.sHtML

[R71] 日期格式化
来源：http://mobile.fktsv.cn/Article/details/gpbrlpwue.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://wap.bbcook.cn/Article/details/goguyopuo.sHtML

[R72] 等待端口就绪
来源：http://www.blog.vehdjk.com/Article/details/gjzarqzsy.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://m.share.bbcook.cn/Article/details/gxpwgmvwt.sHtML

[R73] 分割大日志
来源：http://blog.vehdjk.com/Article/details/gmmuegzxi.sHtML

split -l 1000 big.log part_
来源：http://m.share.tarul.cn/Article/details/ggoywrgbe.sHtML

[R74] 批量重命名
来源：http://mobile.fktsv.cn/Article/details/gzrvtjdyl.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://3g.tarul.cn/Article/details/ghicqmccx.sHtML

[R75] 导出环境变量
来源：http://wap.yfazqb.com/Article/details/gbhvtjztm.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://3g.bbcook.cn/Article/details/gilmymmnn.sHtML

[R76] 使用临时文件
来源：http://baike.epnwcf.com/Article/details/glywnyrum.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.epnwcf.com/Article/details/gnxypebqm.sHtML

[R77] 读取用户输入
来源：http://www.share.sjlbkw.cn/Article/details/gbfegpmsa.sHtML

read -rp "请输入: " ans
来源：http://m.share.yfazqb.com/Article/details/gokofbcpc.sHtML

[R78] 交互式菜单
来源：http://www.blog.yfazqb.com/Article/details/gtbwwehqh.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://blog.vehdjk.com/Article/details/gniqipnaw.sHtML

[R79] 解析命令行选项
来源：http://read.share.bbcook.cn/Article/details/goqlvjfan.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://baike.vehdjk.com/Article/details/giuxrxplg.sHtML

[R80] 查看脚本执行耗时
来源：http://m.share.epnwcf.com/Article/details/gqldyxaii.sHtML

time ./run.sh
来源：http://m.share.vehdjk.com/Article/details/gpaisydmg.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/gcremswad.sHtML

S. C / C++ 专题
来源：http://m.share.vehdjk.com/Article/details/gkgywherj.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/gmqucqvlt.sHtML

[S01] C：Hello World
来源：http://m.share.tarul.cn/Article/details/gozuwxesa.sHtML

#include <stdio.h>
来源：http://m.share.epnwcf.com/Article/details/gaygdfpkt.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.blog.yfazqb.com/Article/details/gjcktpvcn.sHtML

[S02] C：变量与格式化输出
来源：http://read.share.vehdjk.com/Article/details/gsursleji.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.share.yfazqb.com/Article/details/gtlvhpodf.sHtML

[S03] C：读入整数
来源：http://www.blog.tarul.cn/Article/details/gwlkikupm.sHtML

int x; scanf("%d", &x);
来源：http://wap.fktsv.cn/Article/details/gavrsdgcm.sHtML

[S04] C：字符串复制
来源：http://mobile.vehdjk.com/Article/details/gluplsdse.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://blog.yfazqb.com/Article/details/gqzgibyjs.sHtML

[S05] C：字符串长度
来源：http://read.share.epnwcf.com/Article/details/gonkltozy.sHtML

strlen(s)
来源：http://blog.fktsv.cn/Article/details/ginowqwqg.sHtML

[S06] C：字符串比较
来源：http://www.blog.fktsv.cn/Article/details/gfvdiubua.sHtML

strcmp(a, b) == 0
来源：http://mobile.sjlbkw.cn/Article/details/gewabdxyw.sHtML

[S07] C：数组遍历求和
来源：http://mobile.yfazqb.com/Article/details/ghylahrod.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://m.share.fktsv.cn/Article/details/gmyeaizja.sHtML

[S08] C：动态内存分配与释放
来源：http://www.share.sjlbkw.cn/Article/details/gpqvaxphi.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://3g.epnwcf.com/Article/details/ggphygmvq.sHtML

[S09] C：结构体定义与初始化
来源：http://read.share.fktsv.cn/Article/details/gucmsxcsp.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.share.fktsv.cn/Article/details/ggkzqkmil.sHtML

[S10] C：指针与解引用
来源：http://wap.tarul.cn/Article/details/gnbuwiokp.sHtML

int *p = &a;  *p = 5;
来源：http://read.share.bbcook.cn/Article/details/gwsljcndk.sHtML

[S11] C：逐行读文件
来源：http://3g.fktsv.cn/Article/details/ggwdrkarw.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://mobile.vehdjk.com/Article/details/gspatecvk.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://read.share.bbcook.cn/Article/details/gbjpqlasz.sHtML

fclose(f);
来源：http://read.share.sjlbkw.cn/Article/details/gsymtbxkk.sHtML

[S12] C：写文件
来源：http://www.m.share.epnwcf.com/Article/details/gdmaqjaop.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://read.share.vehdjk.com/Article/details/gvikolgjy.sHtML

[S13] C：宏定义
来源：http://m.share.epnwcf.com/Article/details/ghkvgslts.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://m.share.vehdjk.com/Article/details/gqsyfkhqj.sHtML

[S14] C：枚举
来源：http://baike.vehdjk.com/Article/details/geirytgkc.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://baike.tarul.cn/Article/details/gnyirexlp.sHtML

[S15] C：类型转换
来源：http://mobile.yfazqb.com/Article/details/gzzophboc.sHtML

(double) a / b
来源：http://3g.epnwcf.com/Article/details/gzydgnpqh.sHtML

[S16] C：位操作置位
来源：http://wap.yfazqb.com/Article/details/gattqoczp.sHtML

x |= (1 << 3);
来源：http://wap.bbcook.cn/Article/details/gfgaaufwf.sHtML

[S17] C：安全拼接字符串
来源：http://m.share.epnwcf.com/Article/details/gzxiwojio.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.m.share.sjlbkw.cn/Article/details/ggzcxcefm.sHtML

[S18] C：命令行参数
来源：http://www.m.share.yfazqb.com/Article/details/gfwmahwbf.sHtML

int main(int argc, char **argv)
来源：http://m.share.bbcook.cn/Article/details/gcdrxercg.sHtML

[S19] C：快速排序
来源：http://www.m.share.epnwcf.com/Article/details/gfkdokxco.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://3g.sjlbkw.cn/Article/details/ggbbrzmgb.sHtML

[S20] C：二分查找
来源：http://3g.epnwcf.com/Article/details/ghyfpqsow.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.m.share.fktsv.cn/Article/details/gesbildsh.sHtML

[S21] C：字符类别判断
来源：http://wap.yfazqb.com/Article/details/gujhlihjp.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://blog.vehdjk.com/Article/details/gmjfvbhsn.sHtML

[S22] C：字符串转数字
来源：http://read.share.fktsv.cn/Article/details/ggrhfybza.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://mobile.fktsv.cn/Article/details/gcohzribc.sHtML

[S23] C：随机数
来源：http://baike.tarul.cn/Article/details/gliojectl.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://m.share.sjlbkw.cn/Article/details/galzrpsqa.sHtML

[S24] C：获取本地时间
来源：http://mobile.fktsv.cn/Article/details/gjxlfffaa.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://mobile.tarul.cn/Article/details/gipguezqi.sHtML

[S25] C：内存拷贝
来源：http://www.m.share.bbcook.cn/Article/details/gerpijadt.sHtML

memcpy(dst, src, n);
来源：http://3g.yfazqb.com/Article/details/geuymnwvv.sHtML

[S26] C：内存清零
来源：http://mobile.fktsv.cn/Article/details/gmrvqlnyh.sHtML

memset(a, 0, sizeof a);
来源：http://www.share.epnwcf.com/Article/details/gccqddhgi.sHtML

[S27] C：定义常量
来源：http://3g.fktsv.cn/Article/details/gxcbgnduw.sHtML

const double PI = 3.14159;
来源：http://blog.vehdjk.com/Article/details/glitkjupi.sHtML

[S28] C：静态变量
来源：http://baike.tarul.cn/Article/details/gfdoxksht.sHtML

static int counter = 0;
来源：http://read.share.bbcook.cn/Article/details/gbymvlcyh.sHtML

[S29] C：变参函数
来源：http://blog.epnwcf.com/Article/details/gshnmmbrv.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://3g.fktsv.cn/Article/details/gaczlhhan.sHtML

[S30] C：头文件保护
来源：http://blog.fktsv.cn/Article/details/guqtaziaw.sHtML

#ifndef X_H
来源：http://m.share.vehdjk.com/Article/details/gjuefohhs.sHtML

#define X_H
来源：http://read.share.yfazqb.com/Article/details/gnulnvsxv.sHtML

#endif
来源：http://blog.bbcook.cn/Article/details/glhfivghz.sHtML

[S31] C++：Hello World
来源：http://3g.yfazqb.com/Article/details/giluicelf.sHtML

#include <iostream>
来源：http://www.blog.epnwcf.com/Article/details/gdtgvtqir.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://baike.fktsv.cn/Article/details/ghiwcxywg.sHtML

[S32] C++：字符串
来源：http://baike.fktsv.cn/Article/details/gjodnpret.sHtML

std::string s = "hi";  s += "!";
来源：http://www.m.share.epnwcf.com/Article/details/gwdvsgaxu.sHtML

[S33] C++：vector 增删
来源：http://m.share.epnwcf.com/Article/details/gwonzrgjc.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://baike.sjlbkw.cn/Article/details/gnovbatja.sHtML

[S34] C++：遍历 vector
来源：http://blog.tarul.cn/Article/details/gyqxyyfvd.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://read.share.tarul.cn/Article/details/gfoyrwjic.sHtML

[S35] C++：map
来源：http://3g.yfazqb.com/Article/details/gtxzhlxkn.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.yfazqb.com/Article/details/gjinhjbgc.sHtML

[S36] C++：unordered_map
来源：http://wap.sjlbkw.cn/Article/details/gcpxzflpi.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.bbcook.cn/Article/details/glwujznrf.sHtML

[S37] C++：set
来源：http://wap.tarul.cn/Article/details/gfihdadpf.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.share.bbcook.cn/Article/details/gbbalxvpk.sHtML

[S38] C++：排序
来源：http://www.share.sjlbkw.cn/Article/details/gsciczjys.sHtML

std::sort(v.begin(), v.end());
来源：http://blog.sjlbkw.cn/Article/details/gogwtrcth.sHtML

[S39] C++：自定义比较器排序
来源：http://www.blog.yfazqb.com/Article/details/gmfgzkfho.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wap.fktsv.cn/Article/details/gjjkevagp.sHtML

[S40] C++：查找元素
来源：http://www.share.sjlbkw.cn/Article/details/grqgcwnzw.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://mobile.tarul.cn/Article/details/gjjthlabu.sHtML

[S41] C++：类与构造函数
来源：http://blog.fktsv.cn/Article/details/gkxjrnypo.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://baike.vehdjk.com/Article/details/gygdlefgm.sHtML

[S42] C++：继承与虚函数
来源：http://3g.vehdjk.com/Article/details/gznkbinbf.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.share.epnwcf.com/Article/details/gsacxyxdh.sHtML

[S43] C++：智能指针
来源：http://read.share.fktsv.cn/Article/details/gytpfmrpk.sHtML

auto p = std::make_unique<int>(5);
来源：http://m.share.tarul.cn/Article/details/gdhvwllix.sHtML

[S44] C++：引用传参
来源：http://blog.bbcook.cn/Article/details/gjeokrefo.sHtML

void inc(int &x) { ++x; }
来源：http://mobile.yfazqb.com/Article/details/gvwboceha.sHtML

[S45] C++：lambda
来源：http://read.share.fktsv.cn/Article/details/gmzpyimjj.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://read.share.epnwcf.com/Article/details/gjnybmcds.sHtML

[S46] C++：函数模板
来源：http://read.share.epnwcf.com/Article/details/gzalvcoqc.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://blog.epnwcf.com/Article/details/gzduhivaz.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.m.share.fktsv.cn/Article/details/geimfivld.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://m.share.bbcook.cn/Article/details/gxkwqhvjk.sHtML

[S48] C++：逐行读文件
来源：http://read.share.fktsv.cn/Article/details/gvpxezssg.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.share.sjlbkw.cn/Article/details/gydtofleo.sHtML

while (std::getline(in, line)) { }
来源：http://3g.yfazqb.com/Article/details/gzqmmsacz.sHtML

[S49] C++：写文件
来源：http://wap.tarul.cn/Article/details/gpmoeapgw.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://blog.tarul.cn/Article/details/ghihblgwi.sHtML

[S50] C++：格式化数字
来源：http://wap.epnwcf.com/Article/details/golacaryp.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.m.share.tarul.cn/Article/details/guxyemngf.sHtML

[S51] C++：显式类型转换
来源：http://www.m.share.epnwcf.com/Article/details/gjmfxsmid.sHtML

static_cast<double>(a) / b
来源：http://www.m.share.epnwcf.com/Article/details/gyzmqpusa.sHtML

[S52] C++：const 与 noexcept
来源：http://read.share.bbcook.cn/Article/details/gfcydtopb.sHtML

int size() const noexcept { return n_; }
来源：http://www.blog.fktsv.cn/Article/details/gzyvsbvvk.sHtML

[S53] C++：移动语义
来源：http://mobile.sjlbkw.cn/Article/details/gabowyehu.sHtML

std::vector<int> w = std::move(v);
来源：http://baike.bbcook.cn/Article/details/gfbpzzwkv.sHtML

[S54] C++：异常处理
来源：http://3g.bbcook.cn/Article/details/gsaceyhlj.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://read.share.sjlbkw.cn/Article/details/ggyswpofl.sHtML

[S55] C++：结构化绑定
来源：http://mobile.bbcook.cn/Article/details/gsfctxoax.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://blog.tarul.cn/Article/details/gvfilsexw.sHtML

[S56] C++：optional
来源：http://m.share.fktsv.cn/Article/details/grpzrdnvp.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.m.share.vehdjk.com/Article/details/gfpkhfoxa.sHtML

[S57] C++：编译期常量
来源：http://www.blog.fktsv.cn/Article/details/gyxcxrhsz.sHtML

constexpr int N = 10;
来源：http://m.share.sjlbkw.cn/Article/details/govfsxiwg.sHtML

[S58] C++：命名空间
来源：http://read.share.yfazqb.com/Article/details/goppjhnvl.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.m.share.bbcook.cn/Article/details/gkxnhggft.sHtML

[S59] C++：静态断言
来源：http://baike.yfazqb.com/Article/details/gakkqlqry.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://read.share.fktsv.cn/Article/details/gleyffply.sHtML

[S60] C++：遍历并删除元素
来源：http://m.share.fktsv.cn/Article/details/gilzlrswn.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.m.share.tarul.cn/Article/details/gpnsgbaca.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/gbzzqphoe.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.share.epnwcf.com/Article/details/gixnlclma.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/gatbzbjwp.sHtML

[T01] Kotlin：Hello World
来源：http://wap.epnwcf.com/Article/details/gazssqczu.sHtML

println("Hello")
来源：http://www.blog.fktsv.cn/Article/details/gomizjvax.sHtML

[T02] Kotlin：变量
来源：http://read.share.epnwcf.com/Article/details/gidqxmhfx.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://read.share.bbcook.cn/Article/details/gruelbfvy.sHtML

[T03] Kotlin：字符串模板
来源：http://mobile.fktsv.cn/Article/details/gskembfcu.sHtML

"值: $b"
来源：http://3g.bbcook.cn/Article/details/gnecwygzs.sHtML

[T04] Kotlin：空安全
来源：http://m.share.vehdjk.com/Article/details/gihtmbkyp.sHtML

val n: String? = null;  n?.length
来源：http://read.share.fktsv.cn/Article/details/gniksenga.sHtML

[T05] Kotlin：when 表达式
来源：http://www.share.tarul.cn/Article/details/geggafesz.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.m.share.bbcook.cn/Article/details/gxiqzlaga.sHtML

[T06] Kotlin：集合映射
来源：http://www.m.share.fktsv.cn/Article/details/ghqecmznm.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.blog.vehdjk.com/Article/details/gofczysrr.sHtML


<!-- 参考信息 -->