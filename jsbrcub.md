代发 wailian999

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://mobile.sjlbkw.cn/Article/details/gevhnrujo.sHtML

[R08] 数值比较
来源：http://m.share.vehdjk.com/Article/details/gajkjhfkn.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://read.share.epnwcf.com/Article/details/gtomybxzs.sHtML

[R09] 字符串比较
来源：http://www.blog.epnwcf.com/Article/details/grayfnxnw.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://read.share.bbcook.cn/Article/details/gccbbcqxx.sHtML

[R10] 正则匹配
来源：http://www.share.yfazqb.com/Article/details/gxauwlsoj.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.m.share.yfazqb.com/Article/details/gkyvyogct.sHtML

[R11] case 多分支
来源：http://www.m.share.epnwcf.com/Article/details/gqwdhrruc.sHtML

case "$1" in
来源：http://3g.fktsv.cn/Article/details/geiglogbd.sHtML

start) echo "启动" ;;
来源：http://www.share.sjlbkw.cn/Article/details/gwoxscydo.sHtML

stop)  echo "停止" ;;
来源：http://wap.bbcook.cn/Article/details/gwwuppgvw.sHtML

*)     echo "未知命令" ;;
来源：http://blog.sjlbkw.cn/Article/details/goduffqlm.sHtML

esac
来源：http://www.m.share.epnwcf.com/Article/details/gbaracbvv.sHtML

[R12] for 遍历文件
来源：http://www.blog.bbcook.cn/Article/details/gbfeypiuy.sHtML

for f in *.txt; do echo "$f"; done
来源：http://3g.yfazqb.com/Article/details/gjbhjjbxx.sHtML

[R13] for 计数循环
来源：http://blog.yfazqb.com/Article/details/gfkexnlzp.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.blog.tarul.cn/Article/details/geazvjlot.sHtML

[R14] C 风格 for
来源：http://www.share.sjlbkw.cn/Article/details/gagzukuni.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://wap.fktsv.cn/Article/details/gyuiajets.sHtML

[R15] while 逐行读文件
来源：http://wap.epnwcf.com/Article/details/gmgmjadhr.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.m.share.tarul.cn/Article/details/gusmdcubz.sHtML

[R16] until 等待条件
来源：http://blog.epnwcf.com/Article/details/gtlgduozb.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://3g.sjlbkw.cn/Article/details/ghgfhtfjm.sHtML

[R17] 数组定义与取值
来源：http://baike.vehdjk.com/Article/details/gwvfmkpfa.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://3g.sjlbkw.cn/Article/details/gzbcqkatu.sHtML

[R18] 遍历数组
来源：http://www.blog.fktsv.cn/Article/details/gjmfzslat.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.m.share.tarul.cn/Article/details/gfergyypq.sHtML

[R19] 数组长度
来源：http://blog.epnwcf.com/Article/details/gqqbxsthm.sHtML

echo "${#arr[@]}"
来源：http://wap.bbcook.cn/Article/details/grwdwvyor.sHtML

[R20] 关联数组（字典）
来源：http://www.blog.fktsv.cn/Article/details/gwaqwhfpq.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://read.share.epnwcf.com/Article/details/gjrtdfwve.sHtML

[R21] 字符串长度
来源：http://mobile.epnwcf.com/Article/details/gcamugyxj.sHtML

echo "${#s}"
来源：http://read.share.yfazqb.com/Article/details/gcucggbwk.sHtML

[R22] 截取子串
来源：http://read.share.epnwcf.com/Article/details/gdyepudys.sHtML

echo "${s:0:5}"
来源：http://blog.bbcook.cn/Article/details/gnrhsrcef.sHtML

[R23] 字符串替换
来源：http://3g.bbcook.cn/Article/details/gxphjtxja.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://blog.tarul.cn/Article/details/gxlbaukup.sHtML

[R24] 大小写转换
来源：http://m.share.sjlbkw.cn/Article/details/gmkiwlgfx.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://m.share.tarul.cn/Article/details/gfbtfrgxw.sHtML

[R25] 去后缀 / 去前缀
来源：http://wap.yfazqb.com/Article/details/glfmltcup.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://m.share.vehdjk.com/Article/details/gllokajtr.sHtML

[R26] 命令替换
来源：http://m.share.fktsv.cn/Article/details/gmsufqtim.sHtML

now=$(date +%F); echo "$now"
来源：http://www.share.bbcook.cn/Article/details/gdigfpgby.sHtML

[R27] 算术展开
来源：http://mobile.yfazqb.com/Article/details/gibfuipaj.sHtML

echo $((1 + 2 * 3))
来源：http://www.share.fktsv.cn/Article/details/glivtflas.sHtML

[R28] 浮点运算
来源：http://m.share.tarul.cn/Article/details/gheuuoavf.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.m.share.sjlbkw.cn/Article/details/ghustnzaa.sHtML

[R29] 定义函数
来源：http://www.blog.epnwcf.com/Article/details/gohewnauj.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://3g.vehdjk.com/Article/details/gqadxtuou.sHtML

[R30] 函数返回状态码
来源：http://wap.sjlbkw.cn/Article/details/gjtiiuqio.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.blog.epnwcf.com/Article/details/gerotgwqv.sHtML

[R31] 局部变量
来源：http://mobile.fktsv.cn/Article/details/gfpnuazqe.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.blog.fktsv.cn/Article/details/gisltnnif.sHtML

[R32] 参数个数校验
来源：http://www.blog.tarul.cn/Article/details/gjrovtfwp.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://mobile.sjlbkw.cn/Article/details/gfifsqnxl.sHtML

[R33] 捕获错误并提示行号
来源：http://m.share.epnwcf.com/Article/details/gojrlovsx.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://blog.fktsv.cn/Article/details/gljkcioic.sHtML

[R34] 退出时清理
来源：http://www.blog.vehdjk.com/Article/details/gdavystnd.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.share.bbcook.cn/Article/details/gqvpycmez.sHtML

[R35] 后台执行并等待
来源：http://read.share.sjlbkw.cn/Article/details/giajoxjca.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.m.share.vehdjk.com/Article/details/gncapycpl.sHtML

[R36] 并发执行多个任务
来源：http://m.share.yfazqb.com/Article/details/gqhdwogig.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.m.share.vehdjk.com/Article/details/gkwjjrduc.sHtML

[R37] 把输出赋给变量
来源：http://blog.sjlbkw.cn/Article/details/ggkakbowh.sHtML

files=$(ls -1)
来源：http://www.share.fktsv.cn/Article/details/giddzpgzm.sHtML

[R38] 管道串联
来源：http://blog.sjlbkw.cn/Article/details/glldehahw.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.share.vehdjk.com/Article/details/gqbfpnjoz.sHtML

[R39] 重定向标准输出与错误
来源：http://www.blog.fktsv.cn/Article/details/gsnibfhac.sHtML

cmd > out.log 2>&1
来源：http://read.share.epnwcf.com/Article/details/gxyhngzya.sHtML

[R40] 追加写日志
来源：http://read.share.yfazqb.com/Article/details/glmmwhrdc.sHtML

echo "log" >> out.log
来源：http://www.share.epnwcf.com/Article/details/gnxuvotsk.sHtML

[R41] 丢弃输出
来源：http://www.share.fktsv.cn/Article/details/gkdrateiv.sHtML

cmd >/dev/null 2>&1
来源：http://3g.sjlbkw.cn/Article/details/gilrqxipn.sHtML

[R42] 输入重定向
来源：http://blog.vehdjk.com/Article/details/guxdpvnwb.sHtML

wc -l < a.txt
来源：http://m.share.epnwcf.com/Article/details/grmuxedfz.sHtML

[R43] 按名字查找文件
来源：http://www.share.vehdjk.com/Article/details/gjbadxyqj.sHtML

find . -name "*.log" -type f
来源：http://www.blog.tarul.cn/Article/details/gamqwvgme.sHtML

[R44] 按修改时间查找
来源：http://mobile.vehdjk.com/Article/details/gjoxllnxj.sHtML

find . -mtime -7 -type f
来源：http://www.share.vehdjk.com/Article/details/gqesdqqpu.sHtML

[R45] 批量删除
来源：http://m.share.fktsv.cn/Article/details/gtlgywhmu.sHtML

find . -name "*.tmp" -delete
来源：http://baike.fktsv.cn/Article/details/gicnzsqgy.sHtML

[R46] 递归替换文件内容
来源：http://www.blog.bbcook.cn/Article/details/gylvkkgge.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://wap.epnwcf.com/Article/details/glhbqiboi.sHtML

[R47] sed 单行替换
来源：http://baike.tarul.cn/Article/details/gtivohwpy.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://wap.yfazqb.com/Article/details/gkqrvefae.sHtML

[R48] awk 取指定列
来源：http://baike.vehdjk.com/Article/details/gjhvrqane.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.share.epnwcf.com/Article/details/gmcfpmutl.sHtML

[R49] awk 带条件
来源：http://www.m.share.tarul.cn/Article/details/grcnurjak.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.share.epnwcf.com/Article/details/gvxyvcbsj.sHtML

[R50] awk 求和
来源：http://www.m.share.vehdjk.com/Article/details/gxssmtkbm.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://baike.epnwcf.com/Article/details/ggvimdiad.sHtML

[R51] 排序去重取前几
来源：http://www.share.tarul.cn/Article/details/geyywmhfd.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://m.share.tarul.cn/Article/details/ghajuapck.sHtML

[R52] 统计行数
来源：http://www.m.share.sjlbkw.cn/Article/details/gicbbquid.sHtML

wc -l a.txt
来源：http://www.blog.bbcook.cn/Article/details/goldmrziv.sHtML

[R53] 查看文件头与实时尾
来源：http://read.share.yfazqb.com/Article/details/gaqleicgd.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://read.share.bbcook.cn/Article/details/gooafjjsd.sHtML

[R54] 比较两个文件
来源：http://read.share.epnwcf.com/Article/details/gpcznberh.sHtML

diff a.txt b.txt
来源：http://read.share.bbcook.cn/Article/details/goschhatj.sHtML

[R55] 压缩与解压
来源：http://m.share.yfazqb.com/Article/details/graeswrqa.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://read.share.tarul.cn/Article/details/gxqedkprf.sHtML

[R56] 远程拷贝
来源：http://blog.tarul.cn/Article/details/gwyausvjf.sHtML

scp file user@host:/path/
来源：http://www.blog.bbcook.cn/Article/details/gftjvrcmy.sHtML

[R57] 远程执行命令
来源：http://m.share.bbcook.cn/Article/details/gewsinlvu.sHtML

ssh user@host 'uptime'
来源：http://baike.sjlbkw.cn/Article/details/gsjzfzvbm.sHtML

[R58] 下载文件
来源：http://baike.tarul.cn/Article/details/gecqbakig.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://baike.epnwcf.com/Article/details/groaojsoa.sHtML

[R59] 发 POST JSON
来源：http://3g.bbcook.cn/Article/details/gpybbtahf.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://mobile.epnwcf.com/Article/details/gidapvelf.sHtML

[R60] 只看 HTTP 状态码
来源：http://read.share.fktsv.cn/Article/details/gfsuxfmaa.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://baike.bbcook.cn/Article/details/govokwvqw.sHtML

[R61] 磁盘占用
来源：http://read.share.yfazqb.com/Article/details/gudgkowbl.sHtML

df -h;  du -sh *
来源：http://www.m.share.vehdjk.com/Article/details/guuuoafkm.sHtML

[R62] 找最占空间的文件
来源：http://m.share.fktsv.cn/Article/details/gchmojbzf.sHtML

du -ah . | sort -rh | head -10
来源：http://3g.epnwcf.com/Article/details/gdyveazgk.sHtML

[R63] 内存与进程
来源：http://3g.tarul.cn/Article/details/gctyashwj.sHtML

free -h;  ps aux | grep nginx
来源：http://blog.yfazqb.com/Article/details/gwtnvggiq.sHtML

[R64] 结束进程
来源：http://www.m.share.sjlbkw.cn/Article/details/giptrxxah.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.m.share.tarul.cn/Article/details/gwoczwjia.sHtML

[R65] 查看端口占用
来源：http://www.share.epnwcf.com/Article/details/galsjhgcv.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wap.yfazqb.com/Article/details/gvttdrjlt.sHtML

[R66] 定时任务
来源：http://mobile.sjlbkw.cn/Article/details/gspbewnpx.sHtML

crontab -e;  crontab -l
来源：http://3g.yfazqb.com/Article/details/gxvfywhxs.sHtML

[R67] 生成随机十六进制串
来源：http://blog.sjlbkw.cn/Article/details/gfiwyjyna.sHtML

openssl rand -hex 16
来源：http://read.share.epnwcf.com/Article/details/gewojpuuu.sHtML

[R68] 计算文件校验值
来源：http://blog.yfazqb.com/Article/details/ghqwruihn.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://read.share.epnwcf.com/Article/details/gpmcynxfo.sHtML

[R69] 生成随机密码
来源：http://mobile.bbcook.cn/Article/details/gkqbzrnkt.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.m.share.yfazqb.com/Article/details/graopulrc.sHtML

[R70] 时间戳与互转
来源：http://www.m.share.tarul.cn/Article/details/gyqskrwlu.sHtML

date +%s;  date -d @1700000000
来源：http://3g.sjlbkw.cn/Article/details/grpdkrhmc.sHtML

[R71] 日期格式化
来源：http://m.share.yfazqb.com/Article/details/gxciubgjb.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://blog.yfazqb.com/Article/details/ghnqnprnn.sHtML

[R72] 等待端口就绪
来源：http://baike.fktsv.cn/Article/details/gibjcqxhe.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://baike.epnwcf.com/Article/details/gnllujgxm.sHtML

[R73] 分割大日志
来源：http://www.share.bbcook.cn/Article/details/gcufqqmao.sHtML

split -l 1000 big.log part_
来源：http://www.blog.tarul.cn/Article/details/gvybhembs.sHtML

[R74] 批量重命名
来源：http://m.share.bbcook.cn/Article/details/gzhdpfknb.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://baike.sjlbkw.cn/Article/details/gjygptezx.sHtML

[R75] 导出环境变量
来源：http://mobile.tarul.cn/Article/details/gofbqtyxe.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://read.share.sjlbkw.cn/Article/details/gbmugrhrc.sHtML

[R76] 使用临时文件
来源：http://baike.epnwcf.com/Article/details/gkordenxx.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://wap.bbcook.cn/Article/details/gpcqtoxig.sHtML

[R77] 读取用户输入
来源：http://blog.epnwcf.com/Article/details/gbapmzepl.sHtML

read -rp "请输入: " ans
来源：http://3g.tarul.cn/Article/details/gqwhykmrz.sHtML

[R78] 交互式菜单
来源：http://read.share.yfazqb.com/Article/details/gpnprilqa.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://read.share.bbcook.cn/Article/details/glwoihtxx.sHtML

[R79] 解析命令行选项
来源：http://wap.epnwcf.com/Article/details/glzrgempb.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://read.share.epnwcf.com/Article/details/guqrizyih.sHtML

[R80] 查看脚本执行耗时
来源：http://3g.sjlbkw.cn/Article/details/gyozotviy.sHtML

time ./run.sh
来源：http://blog.tarul.cn/Article/details/gsusixvfx.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/gnfnhqhpm.sHtML

S. C / C++ 专题
来源：http://www.share.sjlbkw.cn/Article/details/goulyevga.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/gvwiqfsuc.sHtML

[S01] C：Hello World
来源：http://www.blog.epnwcf.com/Article/details/gwrjduybq.sHtML

#include <stdio.h>
来源：http://www.m.share.tarul.cn/Article/details/gcetlphib.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.m.share.bbcook.cn/Article/details/gbzixsmnw.sHtML

[S02] C：变量与格式化输出
来源：http://m.share.bbcook.cn/Article/details/gsoexspoc.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.blog.sjlbkw.cn/Article/details/gbogfiaes.sHtML

[S03] C：读入整数
来源：http://blog.sjlbkw.cn/Article/details/gwbcpwefl.sHtML

int x; scanf("%d", &x);
来源：http://wap.epnwcf.com/Article/details/gkopnlfna.sHtML

[S04] C：字符串复制
来源：http://read.share.fktsv.cn/Article/details/gegtldeel.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://read.share.tarul.cn/Article/details/gmyxufwed.sHtML

[S05] C：字符串长度
来源：http://wap.tarul.cn/Article/details/gvxzwwlcz.sHtML

strlen(s)
来源：http://3g.tarul.cn/Article/details/gxbinzevc.sHtML

[S06] C：字符串比较
来源：http://blog.sjlbkw.cn/Article/details/gwdcdwvdw.sHtML

strcmp(a, b) == 0
来源：http://www.m.share.yfazqb.com/Article/details/grppkowzl.sHtML

[S07] C：数组遍历求和
来源：http://read.share.sjlbkw.cn/Article/details/gsnnfdyzs.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.m.share.vehdjk.com/Article/details/gxlfygauq.sHtML

[S08] C：动态内存分配与释放
来源：http://mobile.tarul.cn/Article/details/gsdjewgry.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://3g.tarul.cn/Article/details/gculhdltx.sHtML

[S09] C：结构体定义与初始化
来源：http://3g.fktsv.cn/Article/details/gysuyukgl.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://wap.tarul.cn/Article/details/ghvhlbgfg.sHtML

[S10] C：指针与解引用
来源：http://3g.vehdjk.com/Article/details/gvvmzkkrj.sHtML

int *p = &a;  *p = 5;
来源：http://www.share.bbcook.cn/Article/details/gbhxntphc.sHtML

[S11] C：逐行读文件
来源：http://baike.fktsv.cn/Article/details/gjpojeyyk.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://wap.tarul.cn/Article/details/gqpznzwra.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://blog.tarul.cn/Article/details/geehzujfj.sHtML

fclose(f);
来源：http://wap.bbcook.cn/Article/details/grnaknxuf.sHtML

[S12] C：写文件
来源：http://baike.tarul.cn/Article/details/gepufoajh.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://3g.tarul.cn/Article/details/guekzjswu.sHtML

[S13] C：宏定义
来源：http://m.share.sjlbkw.cn/Article/details/ggvanxybz.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://blog.sjlbkw.cn/Article/details/gqqyjomhi.sHtML

[S14] C：枚举
来源：http://m.share.tarul.cn/Article/details/glzlkecpd.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.m.share.tarul.cn/Article/details/grqweecgs.sHtML

[S15] C：类型转换
来源：http://baike.vehdjk.com/Article/details/gmzreojec.sHtML

(double) a / b
来源：http://baike.vehdjk.com/Article/details/gfotanryy.sHtML

[S16] C：位操作置位
来源：http://www.blog.bbcook.cn/Article/details/gkykbkmab.sHtML

x |= (1 << 3);
来源：http://m.share.vehdjk.com/Article/details/gjhnotxzl.sHtML

[S17] C：安全拼接字符串
来源：http://wap.bbcook.cn/Article/details/ggiapjhvj.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://baike.fktsv.cn/Article/details/giikeeplb.sHtML

[S18] C：命令行参数
来源：http://wap.bbcook.cn/Article/details/glkhrljli.sHtML

int main(int argc, char **argv)
来源：http://baike.vehdjk.com/Article/details/gcltdahnc.sHtML

[S19] C：快速排序
来源：http://read.share.epnwcf.com/Article/details/gluezysva.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://read.share.yfazqb.com/Article/details/gpiretzdo.sHtML

[S20] C：二分查找
来源：http://www.blog.sjlbkw.cn/Article/details/grievezgz.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://mobile.sjlbkw.cn/Article/details/gjgkoxgrd.sHtML

[S21] C：字符类别判断
来源：http://3g.sjlbkw.cn/Article/details/gscxzkrkw.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mobile.yfazqb.com/Article/details/guoxkggbs.sHtML

[S22] C：字符串转数字
来源：http://3g.tarul.cn/Article/details/goabupzjx.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://3g.fktsv.cn/Article/details/ggtuwbctw.sHtML

[S23] C：随机数
来源：http://baike.vehdjk.com/Article/details/gkzjtmtet.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://3g.fktsv.cn/Article/details/gqsqtuumg.sHtML

[S24] C：获取本地时间
来源：http://blog.vehdjk.com/Article/details/gmgomueqp.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://m.share.fktsv.cn/Article/details/gfejbgavx.sHtML

[S25] C：内存拷贝
来源：http://blog.vehdjk.com/Article/details/gzdaionrv.sHtML

memcpy(dst, src, n);
来源：http://www.blog.bbcook.cn/Article/details/ggcwekpsy.sHtML

[S26] C：内存清零
来源：http://mobile.epnwcf.com/Article/details/gfdnpmzga.sHtML

memset(a, 0, sizeof a);
来源：http://m.share.yfazqb.com/Article/details/gmjphsyrx.sHtML

[S27] C：定义常量
来源：http://www.blog.epnwcf.com/Article/details/ggigldylq.sHtML

const double PI = 3.14159;
来源：http://blog.yfazqb.com/Article/details/glrxewsku.sHtML

[S28] C：静态变量
来源：http://www.m.share.yfazqb.com/Article/details/gifbecsco.sHtML

static int counter = 0;
来源：http://baike.yfazqb.com/Article/details/gqumbaijg.sHtML

[S29] C：变参函数
来源：http://baike.tarul.cn/Article/details/galfhcyoo.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://read.share.bbcook.cn/Article/details/gwyjhptcu.sHtML

[S30] C：头文件保护
来源：http://baike.fktsv.cn/Article/details/goebitvew.sHtML

#ifndef X_H
来源：http://3g.bbcook.cn/Article/details/gurpiakjr.sHtML

#define X_H
来源：http://www.share.tarul.cn/Article/details/gowjunejy.sHtML

#endif
来源：http://baike.bbcook.cn/Article/details/genzxrhvy.sHtML

[S31] C++：Hello World
来源：http://3g.fktsv.cn/Article/details/garxobgoe.sHtML

#include <iostream>
来源：http://www.m.share.sjlbkw.cn/Article/details/glyrpnyxg.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://baike.epnwcf.com/Article/details/gkkcurysc.sHtML

[S32] C++：字符串
来源：http://m.share.fktsv.cn/Article/details/gixvzqail.sHtML

std::string s = "hi";  s += "!";
来源：http://www.share.fktsv.cn/Article/details/gnaqntumh.sHtML

[S33] C++：vector 增删
来源：http://www.m.share.tarul.cn/Article/details/gwwlibnfo.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.m.share.sjlbkw.cn/Article/details/gposprbul.sHtML

[S34] C++：遍历 vector
来源：http://baike.sjlbkw.cn/Article/details/grgmgjjin.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://m.share.bbcook.cn/Article/details/gmgsggdhn.sHtML

[S35] C++：map
来源：http://3g.vehdjk.com/Article/details/giqcnctmy.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.tarul.cn/Article/details/guwumnvbh.sHtML

[S36] C++：unordered_map
来源：http://mobile.vehdjk.com/Article/details/gnssrxidm.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://3g.bbcook.cn/Article/details/gdeywzxdm.sHtML

[S37] C++：set
来源：http://read.share.yfazqb.com/Article/details/gqupbdhpo.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://baike.epnwcf.com/Article/details/gocfqiwcy.sHtML

[S38] C++：排序
来源：http://read.share.tarul.cn/Article/details/gfqmtpocp.sHtML

std::sort(v.begin(), v.end());
来源：http://3g.yfazqb.com/Article/details/grqywhmnk.sHtML

[S39] C++：自定义比较器排序
来源：http://3g.tarul.cn/Article/details/gygxcxcnw.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.m.share.vehdjk.com/Article/details/gsevzvqir.sHtML

[S40] C++：查找元素
来源：http://www.share.bbcook.cn/Article/details/gxnewclnb.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.m.share.sjlbkw.cn/Article/details/gqzbzccrp.sHtML

[S41] C++：类与构造函数
来源：http://mobile.tarul.cn/Article/details/gigrloexj.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://blog.epnwcf.com/Article/details/gameezjxb.sHtML

[S42] C++：继承与虚函数
来源：http://read.share.tarul.cn/Article/details/gqaflprqm.sHtML

class B : public Base { public: void f() override {} };
来源：http://mobile.vehdjk.com/Article/details/gjxflkwpz.sHtML

[S43] C++：智能指针
来源：http://www.share.yfazqb.com/Article/details/gfmituqzc.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.m.share.yfazqb.com/Article/details/gcixiksad.sHtML

[S44] C++：引用传参
来源：http://www.m.share.sjlbkw.cn/Article/details/glbowlrox.sHtML

void inc(int &x) { ++x; }
来源：http://wap.tarul.cn/Article/details/gkmxrbmzp.sHtML

[S45] C++：lambda
来源：http://blog.tarul.cn/Article/details/gpflttfge.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://blog.vehdjk.com/Article/details/gqhnvmqoj.sHtML

[S46] C++：函数模板
来源：http://www.share.tarul.cn/Article/details/gcklmvjnr.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://blog.sjlbkw.cn/Article/details/gxgwftflw.sHtML

[S47] C++：结构化绑定遍历
来源：http://blog.epnwcf.com/Article/details/gaoujwiwg.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://m.share.fktsv.cn/Article/details/gkmpzfale.sHtML

[S48] C++：逐行读文件
来源：http://www.blog.bbcook.cn/Article/details/gksqmjkir.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://read.share.tarul.cn/Article/details/gsfuvupjt.sHtML

while (std::getline(in, line)) { }
来源：http://m.share.yfazqb.com/Article/details/guvgsteja.sHtML

[S49] C++：写文件
来源：http://read.share.yfazqb.com/Article/details/glhbuoxgb.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.m.share.vehdjk.com/Article/details/gfehcvete.sHtML

[S50] C++：格式化数字
来源：http://mobile.bbcook.cn/Article/details/gkorbmnxi.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://mobile.epnwcf.com/Article/details/gatlxksxt.sHtML

[S51] C++：显式类型转换
来源：http://www.blog.bbcook.cn/Article/details/gqzktyqgo.sHtML

static_cast<double>(a) / b
来源：http://baike.epnwcf.com/Article/details/gzlowhqce.sHtML

[S52] C++：const 与 noexcept
来源：http://read.share.tarul.cn/Article/details/gmdlmmhvo.sHtML

int size() const noexcept { return n_; }
来源：http://3g.tarul.cn/Article/details/guilisukd.sHtML

[S53] C++：移动语义
来源：http://3g.yfazqb.com/Article/details/grcqsbcme.sHtML

std::vector<int> w = std::move(v);
来源：http://read.share.yfazqb.com/Article/details/gdjdyxsjl.sHtML

[S54] C++：异常处理
来源：http://read.share.sjlbkw.cn/Article/details/gspoblixt.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://m.share.epnwcf.com/Article/details/gazaylaky.sHtML

[S55] C++：结构化绑定
来源：http://www.m.share.bbcook.cn/Article/details/gktdmckmw.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.m.share.bbcook.cn/Article/details/glenrogpb.sHtML

[S56] C++：optional
来源：http://www.share.bbcook.cn/Article/details/gtwourxyt.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.m.share.tarul.cn/Article/details/ghukpkpvp.sHtML

[S57] C++：编译期常量
来源：http://www.share.fktsv.cn/Article/details/gnhnkvuwk.sHtML

constexpr int N = 10;
来源：http://wap.tarul.cn/Article/details/gaxkjfycw.sHtML

[S58] C++：命名空间
来源：http://baike.fktsv.cn/Article/details/gmtnqnidg.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.m.share.yfazqb.com/Article/details/giklepkzg.sHtML

[S59] C++：静态断言
来源：http://m.share.vehdjk.com/Article/details/gihnwbxqn.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://baike.fktsv.cn/Article/details/gxniurcgx.sHtML

[S60] C++：遍历并删除元素
来源：http://www.blog.epnwcf.com/Article/details/guqdmvizd.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.m.share.bbcook.cn/Article/details/gzlbyufim.sHtML

================================================================================
来源：http://www.blog.epnwcf.com/Article/details/gdrmrppwy.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.tarul.cn/Article/details/glnjgtduj.sHtML

================================================================================
来源：http://www.m.share.sjlbkw.cn/Article/details/gwtnzskfg.sHtML

[T01] Kotlin：Hello World
来源：http://wap.vehdjk.com/Article/details/gykbkynlf.sHtML

println("Hello")
来源：http://m.share.epnwcf.com/Article/details/gimuzpbkq.sHtML

[T02] Kotlin：变量
来源：http://www.share.epnwcf.com/Article/details/gtaqjijzw.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://wap.bbcook.cn/Article/details/gdqphhcsn.sHtML

[T03] Kotlin：字符串模板
来源：http://www.blog.bbcook.cn/Article/details/gniwnhghd.sHtML

"值: $b"
来源：http://www.blog.fktsv.cn/Article/details/gqrjepsyh.sHtML

[T04] Kotlin：空安全
来源：http://3g.tarul.cn/Article/details/gcrpskwko.sHtML

val n: String? = null;  n?.length
来源：http://3g.vehdjk.com/Article/details/gdtoyaaxt.sHtML

[T05] Kotlin：when 表达式
来源：http://www.m.share.yfazqb.com/Article/details/geqlatxyt.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://baike.fktsv.cn/Article/details/glpecxsst.sHtML

[T06] Kotlin：集合映射
来源：http://m.share.epnwcf.com/Article/details/gdrsdfayk.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.m.share.yfazqb.com/Article/details/gilkqwxyo.sHtML

[T07] Kotlin：集合过滤
来源：http://www.m.share.epnwcf.com/Article/details/gijlxgiaj.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.share.tarul.cn/Article/details/gomkizqvq.sHtML

[T08] Kotlin：数据类
来源：http://blog.vehdjk.com/Article/details/gctxyceta.sHtML

data class User(val name: String, val age: Int)
来源：http://m.share.vehdjk.com/Article/details/gphxzutmu.sHtML


<!-- 参考信息 -->