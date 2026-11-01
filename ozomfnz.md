代发 wailian999

for i in {1..10}; do echo "$i"; done
来源：http://mobile.yfazqb.com/Article/details/gjoturksr.sHtML

[R14] C 风格 for
来源：http://www.m.share.bbcook.cn/Article/details/gtiovzmbm.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.blog.tarul.cn/Article/details/gtmrkpfdk.sHtML

[R15] while 逐行读文件
来源：http://mobile.fktsv.cn/Article/details/gtowzuldw.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://read.share.fktsv.cn/Article/details/gypqlbets.sHtML

[R16] until 等待条件
来源：http://www.m.share.sjlbkw.cn/Article/details/golcdlcon.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://wap.tarul.cn/Article/details/ghxvhnzqb.sHtML

[R17] 数组定义与取值
来源：http://m.share.yfazqb.com/Article/details/gflcdzkbc.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.m.share.tarul.cn/Article/details/gbyzfmher.sHtML

[R18] 遍历数组
来源：http://read.share.yfazqb.com/Article/details/grahvyfqi.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.m.share.fktsv.cn/Article/details/gkvhsgovn.sHtML

[R19] 数组长度
来源：http://blog.fktsv.cn/Article/details/gfdgxenjv.sHtML

echo "${#arr[@]}"
来源：http://3g.tarul.cn/Article/details/gulxvpccw.sHtML

[R20] 关联数组（字典）
来源：http://www.m.share.tarul.cn/Article/details/grctbpxlg.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.m.share.tarul.cn/Article/details/gsxwxtulr.sHtML

[R21] 字符串长度
来源：http://blog.epnwcf.com/Article/details/gtlsnmjtt.sHtML

echo "${#s}"
来源：http://www.m.share.epnwcf.com/Article/details/gubswbzpb.sHtML

[R22] 截取子串
来源：http://www.blog.yfazqb.com/Article/details/gxhtsxygl.sHtML

echo "${s:0:5}"
来源：http://www.share.fktsv.cn/Article/details/gwhkvyyhj.sHtML

[R23] 字符串替换
来源：http://blog.yfazqb.com/Article/details/gzbubgmqn.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.share.vehdjk.com/Article/details/ggwuovgzn.sHtML

[R24] 大小写转换
来源：http://mobile.yfazqb.com/Article/details/gadkgmowi.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://m.share.tarul.cn/Article/details/gwzkwjitv.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.share.fktsv.cn/Article/details/gbfxswtfz.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.m.share.sjlbkw.cn/Article/details/gtugxamne.sHtML

[R26] 命令替换
来源：http://m.share.yfazqb.com/Article/details/gtxvbldwb.sHtML

now=$(date +%F); echo "$now"
来源：http://read.share.vehdjk.com/Article/details/gxwkxvsaj.sHtML

[R27] 算术展开
来源：http://mobile.sjlbkw.cn/Article/details/gcbxjbqbk.sHtML

echo $((1 + 2 * 3))
来源：http://baike.fktsv.cn/Article/details/guvpjugvp.sHtML

[R28] 浮点运算
来源：http://www.m.share.bbcook.cn/Article/details/gyjqodmav.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.share.vehdjk.com/Article/details/gsukmeyci.sHtML

[R29] 定义函数
来源：http://mobile.epnwcf.com/Article/details/gxbtupsle.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://wap.epnwcf.com/Article/details/gxmjtsibo.sHtML

[R30] 函数返回状态码
来源：http://wap.yfazqb.com/Article/details/gnzxesjjm.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://read.share.yfazqb.com/Article/details/grlrghkgf.sHtML

[R31] 局部变量
来源：http://www.share.epnwcf.com/Article/details/gcpsbcksn.sHtML

f() { local x=1; echo "$x"; }
来源：http://3g.sjlbkw.cn/Article/details/gcdudgmsl.sHtML

[R32] 参数个数校验
来源：http://m.share.sjlbkw.cn/Article/details/gxvkejlmz.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gspheijjd.sHtML

[R33] 捕获错误并提示行号
来源：http://wap.epnwcf.com/Article/details/ggqzlwunj.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://mobile.yfazqb.com/Article/details/gyycryqah.sHtML

[R34] 退出时清理
来源：http://3g.fktsv.cn/Article/details/gtkdceiyt.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://3g.bbcook.cn/Article/details/gkrnlwbxd.sHtML

[R35] 后台执行并等待
来源：http://3g.tarul.cn/Article/details/gikzwctjc.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://3g.vehdjk.com/Article/details/gnnzrhved.sHtML

[R36] 并发执行多个任务
来源：http://3g.fktsv.cn/Article/details/gcdousltt.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.m.share.fktsv.cn/Article/details/gntumwtzt.sHtML

[R37] 把输出赋给变量
来源：http://blog.fktsv.cn/Article/details/gkpbuaear.sHtML

files=$(ls -1)
来源：http://m.share.tarul.cn/Article/details/gxgywbaiu.sHtML

[R38] 管道串联
来源：http://m.share.tarul.cn/Article/details/ggghkgpla.sHtML

cat a.txt | grep -i error | wc -l
来源：http://blog.fktsv.cn/Article/details/grjqwmejt.sHtML

[R39] 重定向标准输出与错误
来源：http://blog.epnwcf.com/Article/details/gptygxyxo.sHtML

cmd > out.log 2>&1
来源：http://blog.bbcook.cn/Article/details/gvibzrpbq.sHtML

[R40] 追加写日志
来源：http://www.blog.yfazqb.com/Article/details/gstokreop.sHtML

echo "log" >> out.log
来源：http://m.share.fktsv.cn/Article/details/gfobkyurq.sHtML

[R41] 丢弃输出
来源：http://baike.fktsv.cn/Article/details/gojruglli.sHtML

cmd >/dev/null 2>&1
来源：http://3g.epnwcf.com/Article/details/gfuqktdqq.sHtML

[R42] 输入重定向
来源：http://3g.vehdjk.com/Article/details/gsopyxgmg.sHtML

wc -l < a.txt
来源：http://blog.yfazqb.com/Article/details/glagibsyt.sHtML

[R43] 按名字查找文件
来源：http://www.share.tarul.cn/Article/details/gwhhejree.sHtML

find . -name "*.log" -type f
来源：http://www.blog.fktsv.cn/Article/details/gljhvvtie.sHtML

[R44] 按修改时间查找
来源：http://m.share.bbcook.cn/Article/details/gnkzzuvxh.sHtML

find . -mtime -7 -type f
来源：http://www.share.vehdjk.com/Article/details/gatshcdzc.sHtML

[R45] 批量删除
来源：http://m.share.fktsv.cn/Article/details/glfelwqfu.sHtML

find . -name "*.tmp" -delete
来源：http://3g.yfazqb.com/Article/details/gnaxslbyl.sHtML

[R46] 递归替换文件内容
来源：http://www.m.share.sjlbkw.cn/Article/details/ghdrsmhlc.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://wap.fktsv.cn/Article/details/gmldzpdus.sHtML

[R47] sed 单行替换
来源：http://www.share.vehdjk.com/Article/details/gmormhvrm.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://3g.tarul.cn/Article/details/gxzwbhgyx.sHtML

[R48] awk 取指定列
来源：http://www.blog.bbcook.cn/Article/details/gyqtdjzts.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.share.epnwcf.com/Article/details/gszbhpboa.sHtML

[R49] awk 带条件
来源：http://www.share.bbcook.cn/Article/details/gtwsecojd.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://3g.sjlbkw.cn/Article/details/gjojcjhzq.sHtML

[R50] awk 求和
来源：http://blog.bbcook.cn/Article/details/gzpqhnqgp.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://read.share.tarul.cn/Article/details/gbnhcseqx.sHtML

[R51] 排序去重取前几
来源：http://3g.bbcook.cn/Article/details/gtcdzzjla.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://blog.vehdjk.com/Article/details/gmmzydkux.sHtML

[R52] 统计行数
来源：http://www.blog.vehdjk.com/Article/details/gufysmfvu.sHtML

wc -l a.txt
来源：http://www.share.bbcook.cn/Article/details/glovwrwno.sHtML

[R53] 查看文件头与实时尾
来源：http://read.share.bbcook.cn/Article/details/gocreddth.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://wap.epnwcf.com/Article/details/gyaaikgfi.sHtML

[R54] 比较两个文件
来源：http://read.share.bbcook.cn/Article/details/gnyouiwco.sHtML

diff a.txt b.txt
来源：http://read.share.yfazqb.com/Article/details/gifxkchkn.sHtML

[R55] 压缩与解压
来源：http://www.m.share.epnwcf.com/Article/details/geejyqbqm.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://wap.tarul.cn/Article/details/gptyntqwh.sHtML

[R56] 远程拷贝
来源：http://read.share.tarul.cn/Article/details/ghawyeafv.sHtML

scp file user@host:/path/
来源：http://m.share.fktsv.cn/Article/details/gnsjogdui.sHtML

[R57] 远程执行命令
来源：http://3g.yfazqb.com/Article/details/gtgpnromk.sHtML

ssh user@host 'uptime'
来源：http://blog.bbcook.cn/Article/details/gfecxncvt.sHtML

[R58] 下载文件
来源：http://read.share.vehdjk.com/Article/details/gqbwrxidr.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://m.share.yfazqb.com/Article/details/gsrbynepp.sHtML

[R59] 发 POST JSON
来源：http://www.m.share.fktsv.cn/Article/details/golvpbhdj.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.share.sjlbkw.cn/Article/details/gsdthijtq.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.m.share.bbcook.cn/Article/details/gjgitjowh.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://read.share.yfazqb.com/Article/details/gqurpzcit.sHtML

[R61] 磁盘占用
来源：http://baike.fktsv.cn/Article/details/gxicgazlf.sHtML

df -h;  du -sh *
来源：http://mobile.bbcook.cn/Article/details/gnkurckab.sHtML

[R62] 找最占空间的文件
来源：http://mobile.fktsv.cn/Article/details/gsyecqavf.sHtML

du -ah . | sort -rh | head -10
来源：http://www.share.tarul.cn/Article/details/ghswomxam.sHtML

[R63] 内存与进程
来源：http://read.share.yfazqb.com/Article/details/gnmhhoftm.sHtML

free -h;  ps aux | grep nginx
来源：http://read.share.yfazqb.com/Article/details/gpqtiiuoo.sHtML

[R64] 结束进程
来源：http://www.m.share.bbcook.cn/Article/details/gaiojymms.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.share.epnwcf.com/Article/details/gdqgvoxxi.sHtML

[R65] 查看端口占用
来源：http://mobile.vehdjk.com/Article/details/gglsualxk.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://m.share.sjlbkw.cn/Article/details/guhufeqxd.sHtML

[R66] 定时任务
来源：http://baike.sjlbkw.cn/Article/details/gilflobcx.sHtML

crontab -e;  crontab -l
来源：http://m.share.tarul.cn/Article/details/guyouecum.sHtML

[R67] 生成随机十六进制串
来源：http://baike.bbcook.cn/Article/details/getxvojrw.sHtML

openssl rand -hex 16
来源：http://baike.fktsv.cn/Article/details/gqunzxurr.sHtML

[R68] 计算文件校验值
来源：http://m.share.bbcook.cn/Article/details/gokszxgve.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://3g.sjlbkw.cn/Article/details/gwulvinly.sHtML

[R69] 生成随机密码
来源：http://mobile.epnwcf.com/Article/details/gwylmpyls.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.share.vehdjk.com/Article/details/gmyywfokc.sHtML

[R70] 时间戳与互转
来源：http://blog.yfazqb.com/Article/details/gckuxbgpq.sHtML

date +%s;  date -d @1700000000
来源：http://wap.bbcook.cn/Article/details/gozcygrkd.sHtML

[R71] 日期格式化
来源：http://3g.epnwcf.com/Article/details/gogzuhnzp.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://blog.epnwcf.com/Article/details/gbljfqgnb.sHtML

[R72] 等待端口就绪
来源：http://www.share.yfazqb.com/Article/details/ggmzealnd.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://m.share.sjlbkw.cn/Article/details/gvvqdbfuo.sHtML

[R73] 分割大日志
来源：http://www.blog.vehdjk.com/Article/details/gxnzegdpm.sHtML

split -l 1000 big.log part_
来源：http://read.share.bbcook.cn/Article/details/gsharjtwt.sHtML

[R74] 批量重命名
来源：http://baike.vehdjk.com/Article/details/grbytoeid.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://m.share.sjlbkw.cn/Article/details/gplfpvxxv.sHtML

[R75] 导出环境变量
来源：http://wap.fktsv.cn/Article/details/gogntpshf.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://wap.bbcook.cn/Article/details/glugwyqly.sHtML

[R76] 使用临时文件
来源：http://www.blog.vehdjk.com/Article/details/gcqidbdss.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.bbcook.cn/Article/details/gffrzcyez.sHtML

[R77] 读取用户输入
来源：http://blog.vehdjk.com/Article/details/grxxiwlcn.sHtML

read -rp "请输入: " ans
来源：http://www.m.share.tarul.cn/Article/details/gcsxkrbnd.sHtML

[R78] 交互式菜单
来源：http://www.blog.fktsv.cn/Article/details/gpgnwgenp.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.blog.epnwcf.com/Article/details/ghjydwbmn.sHtML

[R79] 解析命令行选项
来源：http://read.share.epnwcf.com/Article/details/gpelgpodz.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.blog.fktsv.cn/Article/details/gjvwsmatz.sHtML

[R80] 查看脚本执行耗时
来源：http://www.m.share.bbcook.cn/Article/details/gpeiozsir.sHtML

time ./run.sh
来源：http://m.share.vehdjk.com/Article/details/glkfszvip.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/gbmaodkxu.sHtML

S. C / C++ 专题
来源：http://blog.fktsv.cn/Article/details/glvpwzlhd.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/gratugoep.sHtML

[S01] C：Hello World
来源：http://www.share.fktsv.cn/Article/details/gspergawh.sHtML

#include <stdio.h>
来源：http://baike.sjlbkw.cn/Article/details/gxgjommqo.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://3g.bbcook.cn/Article/details/gputbhzis.sHtML

[S02] C：变量与格式化输出
来源：http://read.share.epnwcf.com/Article/details/gmrbgodcd.sHtML

int a = 10; printf("%d\n", a);
来源：http://read.share.tarul.cn/Article/details/gnuqhlyid.sHtML

[S03] C：读入整数
来源：http://3g.yfazqb.com/Article/details/gbmmhbxvp.sHtML

int x; scanf("%d", &x);
来源：http://www.m.share.yfazqb.com/Article/details/gusnnyhzr.sHtML

[S04] C：字符串复制
来源：http://mobile.fktsv.cn/Article/details/gjkmlghlp.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.blog.fktsv.cn/Article/details/gwfmeznpe.sHtML

[S05] C：字符串长度
来源：http://wap.tarul.cn/Article/details/gtjqwtyxk.sHtML

strlen(s)
来源：http://read.share.tarul.cn/Article/details/gdvwumese.sHtML

[S06] C：字符串比较
来源：http://mobile.tarul.cn/Article/details/glgpeqdnh.sHtML

strcmp(a, b) == 0
来源：http://m.share.vehdjk.com/Article/details/gwpbcsdqk.sHtML

[S07] C：数组遍历求和
来源：http://wap.sjlbkw.cn/Article/details/gwjcseoni.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://baike.bbcook.cn/Article/details/gdjfkqfqh.sHtML

[S08] C：动态内存分配与释放
来源：http://read.share.vehdjk.com/Article/details/gwukcpfxc.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://baike.yfazqb.com/Article/details/gcayvjftg.sHtML

[S09] C：结构体定义与初始化
来源：http://read.share.epnwcf.com/Article/details/gictahzmf.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://3g.epnwcf.com/Article/details/glnrynqfs.sHtML

[S10] C：指针与解引用
来源：http://3g.vehdjk.com/Article/details/gwlxwdzxs.sHtML

int *p = &a;  *p = 5;
来源：http://wap.sjlbkw.cn/Article/details/ggajitfyg.sHtML

[S11] C：逐行读文件
来源：http://wap.bbcook.cn/Article/details/griqkoykw.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.m.share.bbcook.cn/Article/details/gsuvqrdsn.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://mobile.epnwcf.com/Article/details/gkpxinmiz.sHtML

fclose(f);
来源：http://www.blog.epnwcf.com/Article/details/gnqwlnivd.sHtML

[S12] C：写文件
来源：http://mobile.yfazqb.com/Article/details/gycivlhmz.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://baike.epnwcf.com/Article/details/gynmzjzjm.sHtML

[S13] C：宏定义
来源：http://www.blog.vehdjk.com/Article/details/gutxhnrka.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://m.share.yfazqb.com/Article/details/gtvtcxpzm.sHtML

[S14] C：枚举
来源：http://m.share.vehdjk.com/Article/details/gkgdhhmvi.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.blog.fktsv.cn/Article/details/giulfpeli.sHtML

[S15] C：类型转换
来源：http://baike.fktsv.cn/Article/details/gnsloesyr.sHtML

(double) a / b
来源：http://www.m.share.epnwcf.com/Article/details/gsehnejvu.sHtML

[S16] C：位操作置位
来源：http://blog.tarul.cn/Article/details/gxhadnqhb.sHtML

x |= (1 << 3);
来源：http://read.share.vehdjk.com/Article/details/geiflfzaq.sHtML

[S17] C：安全拼接字符串
来源：http://www.m.share.vehdjk.com/Article/details/ghixlhzxu.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://3g.yfazqb.com/Article/details/gmpxkvqnm.sHtML

[S18] C：命令行参数
来源：http://3g.sjlbkw.cn/Article/details/gwvhmekzv.sHtML

int main(int argc, char **argv)
来源：http://baike.vehdjk.com/Article/details/gclbugrgf.sHtML

[S19] C：快速排序
来源：http://wap.fktsv.cn/Article/details/gapwdtmjf.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://m.share.bbcook.cn/Article/details/ghlezzsni.sHtML

[S20] C：二分查找
来源：http://www.m.share.vehdjk.com/Article/details/gayceajee.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://mobile.vehdjk.com/Article/details/gcwlenbqa.sHtML

[S21] C：字符类别判断
来源：http://m.share.yfazqb.com/Article/details/giwphrswz.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.share.epnwcf.com/Article/details/gouubyhsv.sHtML

[S22] C：字符串转数字
来源：http://www.blog.vehdjk.com/Article/details/gnejyfyvr.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://m.share.yfazqb.com/Article/details/grgsmpjww.sHtML

[S23] C：随机数
来源：http://3g.tarul.cn/Article/details/gtytsqikq.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://3g.tarul.cn/Article/details/gbgjnfakk.sHtML

[S24] C：获取本地时间
来源：http://baike.tarul.cn/Article/details/gcvndnxzf.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://3g.yfazqb.com/Article/details/gvjwrmnxr.sHtML

[S25] C：内存拷贝
来源：http://www.share.epnwcf.com/Article/details/gbiqmieyw.sHtML

memcpy(dst, src, n);
来源：http://m.share.vehdjk.com/Article/details/gkyelbhwj.sHtML

[S26] C：内存清零
来源：http://baike.fktsv.cn/Article/details/gulnpofxi.sHtML

memset(a, 0, sizeof a);
来源：http://3g.tarul.cn/Article/details/gpclrrvrf.sHtML

[S27] C：定义常量
来源：http://mobile.sjlbkw.cn/Article/details/gcvxkfiqc.sHtML

const double PI = 3.14159;
来源：http://www.m.share.sjlbkw.cn/Article/details/ggavbqazg.sHtML

[S28] C：静态变量
来源：http://baike.tarul.cn/Article/details/gnanzytju.sHtML

static int counter = 0;
来源：http://www.blog.sjlbkw.cn/Article/details/glrzijhzr.sHtML

[S29] C：变参函数
来源：http://baike.fktsv.cn/Article/details/ggzqcwczc.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://read.share.vehdjk.com/Article/details/giuneonli.sHtML

[S30] C：头文件保护
来源：http://www.blog.sjlbkw.cn/Article/details/gipxpfblz.sHtML

#ifndef X_H
来源：http://mobile.fktsv.cn/Article/details/gadhblbzu.sHtML

#define X_H
来源：http://3g.yfazqb.com/Article/details/ghckqhxdy.sHtML

#endif
来源：http://m.share.tarul.cn/Article/details/gemlcclwe.sHtML

[S31] C++：Hello World
来源：http://www.m.share.tarul.cn/Article/details/gutrrrkdu.sHtML

#include <iostream>
来源：http://3g.tarul.cn/Article/details/geirxnwtb.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://blog.fktsv.cn/Article/details/gbifsjztb.sHtML

[S32] C++：字符串
来源：http://wap.bbcook.cn/Article/details/guqjbrnrn.sHtML

std::string s = "hi";  s += "!";
来源：http://www.blog.epnwcf.com/Article/details/gipwopucl.sHtML

[S33] C++：vector 增删
来源：http://blog.sjlbkw.cn/Article/details/gvffitvpf.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://blog.yfazqb.com/Article/details/gvoggdxhu.sHtML

[S34] C++：遍历 vector
来源：http://baike.epnwcf.com/Article/details/gworxzsob.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://wap.tarul.cn/Article/details/ghaavrbdb.sHtML

[S35] C++：map
来源：http://blog.bbcook.cn/Article/details/gqyddjpqn.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://3g.sjlbkw.cn/Article/details/gwgkeyihz.sHtML

[S36] C++：unordered_map
来源：http://wap.fktsv.cn/Article/details/gcaqkscly.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://blog.vehdjk.com/Article/details/gaehuztgk.sHtML

[S37] C++：set
来源：http://wap.yfazqb.com/Article/details/glzlygvrs.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://mobile.vehdjk.com/Article/details/gqofjwbao.sHtML

[S38] C++：排序
来源：http://m.share.fktsv.cn/Article/details/gpjxmqget.sHtML

std::sort(v.begin(), v.end());
来源：http://3g.bbcook.cn/Article/details/guibadefx.sHtML

[S39] C++：自定义比较器排序
来源：http://blog.sjlbkw.cn/Article/details/gwfivnhbl.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://read.share.sjlbkw.cn/Article/details/gnzurxema.sHtML

[S40] C++：查找元素
来源：http://m.share.tarul.cn/Article/details/gpeuiobwm.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://m.share.sjlbkw.cn/Article/details/gzunqrypa.sHtML

[S41] C++：类与构造函数
来源：http://baike.yfazqb.com/Article/details/gzcvtjwhd.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://m.share.sjlbkw.cn/Article/details/grrovgpds.sHtML

[S42] C++：继承与虚函数
来源：http://www.share.vehdjk.com/Article/details/gtomocoaq.sHtML

class B : public Base { public: void f() override {} };
来源：http://baike.epnwcf.com/Article/details/gwxsysert.sHtML

[S43] C++：智能指针
来源：http://mobile.tarul.cn/Article/details/garpilmjc.sHtML

auto p = std::make_unique<int>(5);
来源：http://3g.bbcook.cn/Article/details/gxkkkfjwm.sHtML

[S44] C++：引用传参
来源：http://m.share.yfazqb.com/Article/details/gmvaskxql.sHtML

void inc(int &x) { ++x; }
来源：http://read.share.bbcook.cn/Article/details/gbbyxfdmw.sHtML

[S45] C++：lambda
来源：http://blog.vehdjk.com/Article/details/gfqwvtinc.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://mobile.yfazqb.com/Article/details/gpctmvmjq.sHtML

[S46] C++：函数模板
来源：http://baike.tarul.cn/Article/details/gtsptfutj.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://baike.bbcook.cn/Article/details/gdaxqvjig.sHtML

[S47] C++：结构化绑定遍历
来源：http://blog.sjlbkw.cn/Article/details/gaatcpdfb.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://baike.sjlbkw.cn/Article/details/ghpjjrwtr.sHtML

[S48] C++：逐行读文件
来源：http://www.share.bbcook.cn/Article/details/gjknmlxht.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.blog.yfazqb.com/Article/details/gqbtqqznd.sHtML

while (std::getline(in, line)) { }
来源：http://baike.tarul.cn/Article/details/gbcirabzl.sHtML

[S49] C++：写文件
来源：http://read.share.yfazqb.com/Article/details/gltzttsfe.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://3g.bbcook.cn/Article/details/gndrmmhxn.sHtML

[S50] C++：格式化数字
来源：http://www.blog.vehdjk.com/Article/details/gqmaxudwn.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://3g.sjlbkw.cn/Article/details/gpaibpftf.sHtML

[S51] C++：显式类型转换
来源：http://3g.tarul.cn/Article/details/gmichtoqx.sHtML

static_cast<double>(a) / b
来源：http://www.blog.vehdjk.com/Article/details/gmgvllbuy.sHtML

[S52] C++：const 与 noexcept
来源：http://www.blog.yfazqb.com/Article/details/gqcvjwnhm.sHtML

int size() const noexcept { return n_; }
来源：http://mobile.tarul.cn/Article/details/gfuhszqfj.sHtML

[S53] C++：移动语义
来源：http://3g.tarul.cn/Article/details/gsnualtfh.sHtML

std::vector<int> w = std::move(v);
来源：http://mobile.fktsv.cn/Article/details/gouikxntl.sHtML

[S54] C++：异常处理
来源：http://wap.tarul.cn/Article/details/gldcocgje.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://baike.yfazqb.com/Article/details/gephttozu.sHtML

[S55] C++：结构化绑定
来源：http://3g.bbcook.cn/Article/details/gjwrhmdrq.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://blog.epnwcf.com/Article/details/gurismhrq.sHtML

[S56] C++：optional
来源：http://www.m.share.bbcook.cn/Article/details/gvuimztxa.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.share.yfazqb.com/Article/details/gthekyutd.sHtML

[S57] C++：编译期常量
来源：http://3g.tarul.cn/Article/details/glvpbimvn.sHtML

constexpr int N = 10;
来源：http://www.share.tarul.cn/Article/details/gkwwxihzn.sHtML

[S58] C++：命名空间
来源：http://mobile.epnwcf.com/Article/details/gwgcfvrcu.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.blog.yfazqb.com/Article/details/gzgrrybmk.sHtML

[S59] C++：静态断言
来源：http://wap.tarul.cn/Article/details/gnkznowyy.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.share.tarul.cn/Article/details/ggqazqzjq.sHtML

[S60] C++：遍历并删除元素
来源：http://www.share.epnwcf.com/Article/details/ghqaeblbr.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://3g.bbcook.cn/Article/details/gkcrymnrp.sHtML

================================================================================
来源：http://www.m.share.sjlbkw.cn/Article/details/glhqklcdh.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://read.share.vehdjk.com/Article/details/ggxgwydts.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/gzaqxsyqi.sHtML

[T01] Kotlin：Hello World
来源：http://www.share.tarul.cn/Article/details/gdevcjqzu.sHtML

println("Hello")
来源：http://mobile.fktsv.cn/Article/details/gnmocwlka.sHtML

[T02] Kotlin：变量
来源：http://m.share.tarul.cn/Article/details/glqqpdocw.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://wap.epnwcf.com/Article/details/govtroeom.sHtML

[T03] Kotlin：字符串模板
来源：http://read.share.epnwcf.com/Article/details/gadiuyqyg.sHtML

"值: $b"
来源：http://baike.epnwcf.com/Article/details/gzklryomc.sHtML

[T04] Kotlin：空安全
来源：http://baike.sjlbkw.cn/Article/details/gehhmykwy.sHtML

val n: String? = null;  n?.length
来源：http://mobile.yfazqb.com/Article/details/gnfxgecfn.sHtML

[T05] Kotlin：when 表达式
来源：http://www.m.share.bbcook.cn/Article/details/gucrfdjgm.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.m.share.bbcook.cn/Article/details/gfcsqbvqe.sHtML

[T06] Kotlin：集合映射
来源：http://www.blog.yfazqb.com/Article/details/gunskxmov.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://3g.bbcook.cn/Article/details/gkqtidgoj.sHtML

[T07] Kotlin：集合过滤
来源：http://baike.tarul.cn/Article/details/gmyrktxlq.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://baike.tarul.cn/Article/details/gtwbxddix.sHtML

[T08] Kotlin：数据类
来源：http://wap.sjlbkw.cn/Article/details/gbkjyhlaa.sHtML

data class User(val name: String, val age: Int)
来源：http://baike.vehdjk.com/Article/details/gbjpslebb.sHtML

[T09] Kotlin：扩展函数
来源：http://wap.tarul.cn/Article/details/gxmftvrbp.sHtML

fun String.exclaim() = this + "!"
来源：http://wap.vehdjk.com/Article/details/gzfypqvtr.sHtML

[T10] Kotlin：默认参数
来源：http://3g.epnwcf.com/Article/details/gngcthkte.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://3g.sjlbkw.cn/Article/details/ghtotqtbn.sHtML

[T11] Kotlin：协程
来源：http://www.m.share.sjlbkw.cn/Article/details/grtviowjx.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://read.share.yfazqb.com/Article/details/gfzapbpli.sHtML

[T12] Kotlin：解构声明
来源：http://baike.vehdjk.com/Article/details/gmpuyxdga.sHtML

val (a, b) = Pair(1, 2)
来源：http://mobile.tarul.cn/Article/details/gotcowggl.sHtML

[T13] Kotlin：只读 Map
来源：http://baike.epnwcf.com/Article/details/gmesimlcs.sHtML

val m = mapOf("a" to 1)
来源：http://m.share.bbcook.cn/Article/details/giwnzkgst.sHtML

[T14] Kotlin：循环
来源：http://baike.bbcook.cn/Article/details/ggsfehdyg.sHtML

for (i in 1..10) println(i)
来源：http://www.blog.epnwcf.com/Article/details/gvzbzxhta.sHtML

[T15] Kotlin：接口
来源：http://www.share.fktsv.cn/Article/details/gifqvbnrh.sHtML

interface Shape { fun area(): Double }
来源：http://wap.bbcook.cn/Article/details/gbgmeguxf.sHtML

[T16] Swift：Hello World
来源：http://wap.bbcook.cn/Article/details/gconlosvn.sHtML

print("Hello")
来源：http://www.share.yfazqb.com/Article/details/gyqjdwexr.sHtML


<!-- 参考信息 -->