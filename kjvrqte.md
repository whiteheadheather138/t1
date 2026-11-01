代发 wailian999

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://m.share.bbcook.cn/Article/details/gsfdngqgs.sHtML

[R08] 数值比较
来源：http://mobile.fktsv.cn/Article/details/gcqehfmnc.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://wap.vehdjk.com/Article/details/gdzynbjrs.sHtML

[R09] 字符串比较
来源：http://www.m.share.sjlbkw.cn/Article/details/gvjwhaqty.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://read.share.sjlbkw.cn/Article/details/gkgglxvlt.sHtML

[R10] 正则匹配
来源：http://wap.bbcook.cn/Article/details/gozotgldy.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://wap.fktsv.cn/Article/details/grtsizzdv.sHtML

[R11] case 多分支
来源：http://baike.sjlbkw.cn/Article/details/gwzfurupc.sHtML

case "$1" in
来源：http://wap.vehdjk.com/Article/details/gavdlwepz.sHtML

start) echo "启动" ;;
来源：http://baike.sjlbkw.cn/Article/details/gtyfvlhcw.sHtML

stop)  echo "停止" ;;
来源：http://wap.tarul.cn/Article/details/gaeburqkk.sHtML

*)     echo "未知命令" ;;
来源：http://3g.sjlbkw.cn/Article/details/ghjojtdkv.sHtML

esac
来源：http://www.m.share.fktsv.cn/Article/details/gqoniwbxw.sHtML

[R12] for 遍历文件
来源：http://wap.yfazqb.com/Article/details/geieufvcn.sHtML

for f in *.txt; do echo "$f"; done
来源：http://m.share.tarul.cn/Article/details/gcguxxpmr.sHtML

[R13] for 计数循环
来源：http://www.blog.epnwcf.com/Article/details/ggmlrvybx.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://wap.vehdjk.com/Article/details/glfpeosdb.sHtML

[R14] C 风格 for
来源：http://www.share.sjlbkw.cn/Article/details/gmnodarar.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://blog.fktsv.cn/Article/details/gjlhvwihk.sHtML

[R15] while 逐行读文件
来源：http://wap.vehdjk.com/Article/details/gxsjhtgal.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://mobile.fktsv.cn/Article/details/gthxidxwb.sHtML

[R16] until 等待条件
来源：http://m.share.epnwcf.com/Article/details/gwzpisnor.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.m.share.bbcook.cn/Article/details/glicujwjd.sHtML

[R17] 数组定义与取值
来源：http://m.share.vehdjk.com/Article/details/gfuxdchxq.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.blog.epnwcf.com/Article/details/gbmtjyzgs.sHtML

[R18] 遍历数组
来源：http://3g.fktsv.cn/Article/details/gizevavxt.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://read.share.tarul.cn/Article/details/gvizhuebj.sHtML

[R19] 数组长度
来源：http://www.share.tarul.cn/Article/details/gjpqvupfa.sHtML

echo "${#arr[@]}"
来源：http://blog.yfazqb.com/Article/details/gmmfxinbt.sHtML

[R20] 关联数组（字典）
来源：http://wap.vehdjk.com/Article/details/gfjtunbis.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://baike.sjlbkw.cn/Article/details/gzbeojwyv.sHtML

[R21] 字符串长度
来源：http://www.share.vehdjk.com/Article/details/gqhbepkqd.sHtML

echo "${#s}"
来源：http://mobile.yfazqb.com/Article/details/geqxfvfbv.sHtML

[R22] 截取子串
来源：http://www.m.share.tarul.cn/Article/details/gnuotbbyi.sHtML

echo "${s:0:5}"
来源：http://3g.tarul.cn/Article/details/gedxypjsn.sHtML

[R23] 字符串替换
来源：http://www.m.share.epnwcf.com/Article/details/glikwrenw.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://mobile.yfazqb.com/Article/details/gbsoimuvo.sHtML

[R24] 大小写转换
来源：http://blog.sjlbkw.cn/Article/details/gowtqcswm.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://mobile.tarul.cn/Article/details/glzzvrqsp.sHtML

[R25] 去后缀 / 去前缀
来源：http://baike.tarul.cn/Article/details/gvmyletzd.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.blog.vehdjk.com/Article/details/gzljbusaj.sHtML

[R26] 命令替换
来源：http://baike.bbcook.cn/Article/details/gkawrtxes.sHtML

now=$(date +%F); echo "$now"
来源：http://read.share.vehdjk.com/Article/details/gxkclooim.sHtML

[R27] 算术展开
来源：http://3g.bbcook.cn/Article/details/ggewjnfpv.sHtML

echo $((1 + 2 * 3))
来源：http://baike.epnwcf.com/Article/details/gwfbrxycy.sHtML

[R28] 浮点运算
来源：http://read.share.sjlbkw.cn/Article/details/gvhsuquwz.sHtML

echo "scale=2; 10/3" | bc
来源：http://read.share.vehdjk.com/Article/details/grwedxwew.sHtML

[R29] 定义函数
来源：http://www.m.share.fktsv.cn/Article/details/gadnuiyyk.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://3g.epnwcf.com/Article/details/ghchycstd.sHtML

[R30] 函数返回状态码
来源：http://www.m.share.bbcook.cn/Article/details/gtxvccyzm.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.share.yfazqb.com/Article/details/gbxnbavai.sHtML

[R31] 局部变量
来源：http://www.m.share.tarul.cn/Article/details/ghwtioira.sHtML

f() { local x=1; echo "$x"; }
来源：http://baike.epnwcf.com/Article/details/gjvjswrtg.sHtML

[R32] 参数个数校验
来源：http://wap.bbcook.cn/Article/details/gtvoonwia.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://wap.sjlbkw.cn/Article/details/ggdhmxsgh.sHtML

[R33] 捕获错误并提示行号
来源：http://3g.sjlbkw.cn/Article/details/gvahexrgq.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.m.share.tarul.cn/Article/details/gkolayhux.sHtML

[R34] 退出时清理
来源：http://www.share.sjlbkw.cn/Article/details/gbmrdpsis.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://m.share.bbcook.cn/Article/details/gprcskcpu.sHtML

[R35] 后台执行并等待
来源：http://blog.fktsv.cn/Article/details/gfcejytyc.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.m.share.bbcook.cn/Article/details/gmiywudae.sHtML

[R36] 并发执行多个任务
来源：http://www.share.sjlbkw.cn/Article/details/gnlzxjvra.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.blog.tarul.cn/Article/details/gjsqpqgnc.sHtML

[R37] 把输出赋给变量
来源：http://www.m.share.fktsv.cn/Article/details/gvucoyxqv.sHtML

files=$(ls -1)
来源：http://3g.bbcook.cn/Article/details/gxhfjzecz.sHtML

[R38] 管道串联
来源：http://www.share.tarul.cn/Article/details/glmdkbztz.sHtML

cat a.txt | grep -i error | wc -l
来源：http://blog.epnwcf.com/Article/details/gxypzrplb.sHtML

[R39] 重定向标准输出与错误
来源：http://wap.fktsv.cn/Article/details/gqktijulw.sHtML

cmd > out.log 2>&1
来源：http://wap.bbcook.cn/Article/details/ggzzttkql.sHtML

[R40] 追加写日志
来源：http://wap.bbcook.cn/Article/details/gulusogza.sHtML

echo "log" >> out.log
来源：http://read.share.yfazqb.com/Article/details/gbpaxnbnz.sHtML

[R41] 丢弃输出
来源：http://3g.tarul.cn/Article/details/gesuaajfl.sHtML

cmd >/dev/null 2>&1
来源：http://m.share.bbcook.cn/Article/details/guzybvsvc.sHtML

[R42] 输入重定向
来源：http://www.m.share.bbcook.cn/Article/details/grjvggogn.sHtML

wc -l < a.txt
来源：http://baike.yfazqb.com/Article/details/gixmedovn.sHtML

[R43] 按名字查找文件
来源：http://read.share.vehdjk.com/Article/details/gxvntituu.sHtML

find . -name "*.log" -type f
来源：http://baike.tarul.cn/Article/details/gecmtveoa.sHtML

[R44] 按修改时间查找
来源：http://www.share.sjlbkw.cn/Article/details/gbjlmcajn.sHtML

find . -mtime -7 -type f
来源：http://baike.epnwcf.com/Article/details/gjgiuzwlr.sHtML

[R45] 批量删除
来源：http://wap.bbcook.cn/Article/details/grbxjxvuq.sHtML

find . -name "*.tmp" -delete
来源：http://wap.sjlbkw.cn/Article/details/gsxtsbyds.sHtML

[R46] 递归替换文件内容
来源：http://www.share.yfazqb.com/Article/details/gqsfocxph.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://baike.bbcook.cn/Article/details/gmwzrwnko.sHtML

[R47] sed 单行替换
来源：http://3g.sjlbkw.cn/Article/details/gyekigwea.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.blog.sjlbkw.cn/Article/details/gjhkrhzvc.sHtML

[R48] awk 取指定列
来源：http://3g.bbcook.cn/Article/details/gdoajfpxo.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.blog.epnwcf.com/Article/details/gsrpuocnd.sHtML

[R49] awk 带条件
来源：http://baike.sjlbkw.cn/Article/details/gndrwwioe.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wap.fktsv.cn/Article/details/gugzfhuix.sHtML

[R50] awk 求和
来源：http://mobile.fktsv.cn/Article/details/gbvbimtez.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.m.share.yfazqb.com/Article/details/gbwufpdlg.sHtML

[R51] 排序去重取前几
来源：http://www.m.share.tarul.cn/Article/details/gpqcwmily.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.blog.tarul.cn/Article/details/gtrfjjcbp.sHtML

[R52] 统计行数
来源：http://www.m.share.fktsv.cn/Article/details/gtxqwymkm.sHtML

wc -l a.txt
来源：http://3g.vehdjk.com/Article/details/gmqcpujwp.sHtML

[R53] 查看文件头与实时尾
来源：http://www.share.tarul.cn/Article/details/glirthwty.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://baike.fktsv.cn/Article/details/gaakdnjef.sHtML

[R54] 比较两个文件
来源：http://3g.sjlbkw.cn/Article/details/goszdzyin.sHtML

diff a.txt b.txt
来源：http://blog.fktsv.cn/Article/details/ggleavfvd.sHtML

[R55] 压缩与解压
来源：http://www.blog.bbcook.cn/Article/details/gnwuvkgvd.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.share.tarul.cn/Article/details/gihsuxrtc.sHtML

[R56] 远程拷贝
来源：http://m.share.bbcook.cn/Article/details/goopynptt.sHtML

scp file user@host:/path/
来源：http://www.blog.fktsv.cn/Article/details/gxsagtahe.sHtML

[R57] 远程执行命令
来源：http://mobile.yfazqb.com/Article/details/glvfcypwq.sHtML

ssh user@host 'uptime'
来源：http://mobile.bbcook.cn/Article/details/glazjyqjb.sHtML

[R58] 下载文件
来源：http://www.share.epnwcf.com/Article/details/goyfxhqse.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://3g.fktsv.cn/Article/details/gakyzrfzd.sHtML

[R59] 发 POST JSON
来源：http://www.m.share.fktsv.cn/Article/details/gbcodivdq.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://mobile.sjlbkw.cn/Article/details/gqxqjolcg.sHtML

[R60] 只看 HTTP 状态码
来源：http://mobile.yfazqb.com/Article/details/grblceobm.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://3g.bbcook.cn/Article/details/golgebwtb.sHtML

[R61] 磁盘占用
来源：http://3g.tarul.cn/Article/details/gokcdrkqn.sHtML

df -h;  du -sh *
来源：http://m.share.sjlbkw.cn/Article/details/gvuuvdzvp.sHtML

[R62] 找最占空间的文件
来源：http://baike.bbcook.cn/Article/details/ggbjtzhej.sHtML

du -ah . | sort -rh | head -10
来源：http://read.share.vehdjk.com/Article/details/gwcmpiefv.sHtML

[R63] 内存与进程
来源：http://www.m.share.sjlbkw.cn/Article/details/grhdrvdwb.sHtML

free -h;  ps aux | grep nginx
来源：http://www.share.epnwcf.com/Article/details/gwnbkbchl.sHtML

[R64] 结束进程
来源：http://www.blog.epnwcf.com/Article/details/glbimjliq.sHtML

kill -9 $(pgrep -f app.py)
来源：http://wap.yfazqb.com/Article/details/gfmpfyods.sHtML

[R65] 查看端口占用
来源：http://wap.tarul.cn/Article/details/gnkbtlwyz.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wap.sjlbkw.cn/Article/details/gacypnlxi.sHtML

[R66] 定时任务
来源：http://3g.yfazqb.com/Article/details/gpfvpujtv.sHtML

crontab -e;  crontab -l
来源：http://www.blog.fktsv.cn/Article/details/gpxneiyge.sHtML

[R67] 生成随机十六进制串
来源：http://www.share.sjlbkw.cn/Article/details/gglgwlwcz.sHtML

openssl rand -hex 16
来源：http://www.m.share.bbcook.cn/Article/details/gsrbiygqi.sHtML

[R68] 计算文件校验值
来源：http://www.m.share.yfazqb.com/Article/details/giqpnrgoi.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://m.share.yfazqb.com/Article/details/gtcihfizz.sHtML

[R69] 生成随机密码
来源：http://www.blog.bbcook.cn/Article/details/gawsmlrcd.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.blog.bbcook.cn/Article/details/gmswvrazv.sHtML

[R70] 时间戳与互转
来源：http://baike.fktsv.cn/Article/details/gjjjvqhfe.sHtML

date +%s;  date -d @1700000000
来源：http://blog.sjlbkw.cn/Article/details/gzlzxwzkc.sHtML

[R71] 日期格式化
来源：http://www.blog.bbcook.cn/Article/details/gproqcufg.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://m.share.sjlbkw.cn/Article/details/glrzclzjo.sHtML

[R72] 等待端口就绪
来源：http://baike.sjlbkw.cn/Article/details/goeixbtrm.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://mobile.yfazqb.com/Article/details/gwbojuuep.sHtML

[R73] 分割大日志
来源：http://www.share.yfazqb.com/Article/details/gwzimiqse.sHtML

split -l 1000 big.log part_
来源：http://read.share.vehdjk.com/Article/details/gpauiofjg.sHtML

[R74] 批量重命名
来源：http://read.share.tarul.cn/Article/details/gmbtaxnvb.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://baike.bbcook.cn/Article/details/gijuqkubc.sHtML

[R75] 导出环境变量
来源：http://mobile.epnwcf.com/Article/details/gtjrqpswz.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.blog.vehdjk.com/Article/details/gyfuakows.sHtML

[R76] 使用临时文件
来源：http://read.share.bbcook.cn/Article/details/gyeokbuoz.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://baike.epnwcf.com/Article/details/gomspuvoj.sHtML

[R77] 读取用户输入
来源：http://www.m.share.vehdjk.com/Article/details/gcmuvltzb.sHtML

read -rp "请输入: " ans
来源：http://www.share.vehdjk.com/Article/details/gdnhtebht.sHtML

[R78] 交互式菜单
来源：http://www.blog.sjlbkw.cn/Article/details/godyymony.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://3g.tarul.cn/Article/details/gdsuqykxd.sHtML

[R79] 解析命令行选项
来源：http://mobile.vehdjk.com/Article/details/gutirvily.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://blog.epnwcf.com/Article/details/gobywynyo.sHtML

[R80] 查看脚本执行耗时
来源：http://www.share.vehdjk.com/Article/details/gasqgypns.sHtML

time ./run.sh
来源：http://read.share.tarul.cn/Article/details/gqcdvsryk.sHtML

================================================================================
来源：http://www.m.share.sjlbkw.cn/Article/details/gzmeierkk.sHtML

S. C / C++ 专题
来源：http://baike.vehdjk.com/Article/details/gqoehxfxl.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/gsnefstkd.sHtML

[S01] C：Hello World
来源：http://baike.yfazqb.com/Article/details/gpljtlgee.sHtML

#include <stdio.h>
来源：http://read.share.vehdjk.com/Article/details/gfstyddri.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://baike.bbcook.cn/Article/details/gltogkuew.sHtML

[S02] C：变量与格式化输出
来源：http://mobile.tarul.cn/Article/details/gejxazlym.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.blog.epnwcf.com/Article/details/gkvjbdoki.sHtML

[S03] C：读入整数
来源：http://mobile.bbcook.cn/Article/details/glamkofao.sHtML

int x; scanf("%d", &x);
来源：http://www.share.epnwcf.com/Article/details/gvzskfmca.sHtML

[S04] C：字符串复制
来源：http://mobile.sjlbkw.cn/Article/details/gxvgdrbut.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://m.share.tarul.cn/Article/details/gveqkarja.sHtML

[S05] C：字符串长度
来源：http://wap.yfazqb.com/Article/details/gkhuhiywd.sHtML

strlen(s)
来源：http://mobile.epnwcf.com/Article/details/gdxayahmp.sHtML

[S06] C：字符串比较
来源：http://read.share.epnwcf.com/Article/details/gifuyjvkn.sHtML

strcmp(a, b) == 0
来源：http://www.share.epnwcf.com/Article/details/ggfmpbhzw.sHtML

[S07] C：数组遍历求和
来源：http://m.share.fktsv.cn/Article/details/gflpmkvlq.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://wap.yfazqb.com/Article/details/gxljeqddn.sHtML

[S08] C：动态内存分配与释放
来源：http://www.share.tarul.cn/Article/details/gsknrqxsf.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mobile.bbcook.cn/Article/details/ggkotlvxb.sHtML

[S09] C：结构体定义与初始化
来源：http://m.share.bbcook.cn/Article/details/gaebgsvnr.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.m.share.vehdjk.com/Article/details/gbsymmxvp.sHtML

[S10] C：指针与解引用
来源：http://3g.fktsv.cn/Article/details/gykgdtcoq.sHtML

int *p = &a;  *p = 5;
来源：http://3g.vehdjk.com/Article/details/gvzpwgwux.sHtML

[S11] C：逐行读文件
来源：http://blog.vehdjk.com/Article/details/gzlxyohzu.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.share.yfazqb.com/Article/details/gstrxrkut.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://mobile.yfazqb.com/Article/details/gepmjhqtx.sHtML

fclose(f);
来源：http://mobile.bbcook.cn/Article/details/gohgzobeg.sHtML

[S12] C：写文件
来源：http://blog.tarul.cn/Article/details/gxjwdhfkv.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.m.share.bbcook.cn/Article/details/gjxctnoty.sHtML

[S13] C：宏定义
来源：http://m.share.bbcook.cn/Article/details/gyvblauol.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.share.bbcook.cn/Article/details/gmzirlcfh.sHtML

[S14] C：枚举
来源：http://3g.epnwcf.com/Article/details/gdexecarr.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://blog.yfazqb.com/Article/details/gfmweumlq.sHtML

[S15] C：类型转换
来源：http://read.share.yfazqb.com/Article/details/gfcipeyij.sHtML

(double) a / b
来源：http://m.share.yfazqb.com/Article/details/gnsnvsruh.sHtML

[S16] C：位操作置位
来源：http://m.share.vehdjk.com/Article/details/gfxiilyal.sHtML

x |= (1 << 3);
来源：http://mobile.vehdjk.com/Article/details/gkijzqtkt.sHtML

[S17] C：安全拼接字符串
来源：http://baike.tarul.cn/Article/details/gulyfwrdx.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://read.share.yfazqb.com/Article/details/gjwtxraxl.sHtML

[S18] C：命令行参数
来源：http://www.blog.fktsv.cn/Article/details/ghitwzfwi.sHtML

int main(int argc, char **argv)
来源：http://wap.sjlbkw.cn/Article/details/gpvifmwtu.sHtML

[S19] C：快速排序
来源：http://mobile.vehdjk.com/Article/details/gkzvsxmwq.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.share.bbcook.cn/Article/details/gvszbwaqk.sHtML

[S20] C：二分查找
来源：http://m.share.sjlbkw.cn/Article/details/geotchzgy.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://m.share.epnwcf.com/Article/details/gzmsngzsf.sHtML

[S21] C：字符类别判断
来源：http://read.share.sjlbkw.cn/Article/details/gzxbblwok.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.share.bbcook.cn/Article/details/gbwlwvnhi.sHtML

[S22] C：字符串转数字
来源：http://www.m.share.bbcook.cn/Article/details/gsgeopbak.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://3g.bbcook.cn/Article/details/gkjbfdovb.sHtML

[S23] C：随机数
来源：http://blog.bbcook.cn/Article/details/gptfzltad.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://m.share.tarul.cn/Article/details/gwjflfstp.sHtML

[S24] C：获取本地时间
来源：http://read.share.fktsv.cn/Article/details/gwpqpzzmh.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://baike.epnwcf.com/Article/details/gusjgtkqb.sHtML

[S25] C：内存拷贝
来源：http://m.share.tarul.cn/Article/details/gprckfayf.sHtML

memcpy(dst, src, n);
来源：http://baike.bbcook.cn/Article/details/ghpmfmvto.sHtML

[S26] C：内存清零
来源：http://baike.fktsv.cn/Article/details/gcasypxpi.sHtML

memset(a, 0, sizeof a);
来源：http://wap.yfazqb.com/Article/details/gyjzrests.sHtML

[S27] C：定义常量
来源：http://www.share.vehdjk.com/Article/details/giwiilkzk.sHtML

const double PI = 3.14159;
来源：http://www.share.tarul.cn/Article/details/gxcwssmax.sHtML

[S28] C：静态变量
来源：http://baike.epnwcf.com/Article/details/gyvkhsyqt.sHtML

static int counter = 0;
来源：http://blog.yfazqb.com/Article/details/gqgdewxsf.sHtML

[S29] C：变参函数
来源：http://blog.bbcook.cn/Article/details/gcvmbcfpm.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://3g.bbcook.cn/Article/details/gwqjfwwap.sHtML

[S30] C：头文件保护
来源：http://m.share.sjlbkw.cn/Article/details/gryyzswzl.sHtML

#ifndef X_H
来源：http://read.share.fktsv.cn/Article/details/gglxuzwjc.sHtML

#define X_H
来源：http://www.m.share.vehdjk.com/Article/details/gszbzyycb.sHtML

#endif
来源：http://blog.epnwcf.com/Article/details/gtcbjkyfa.sHtML

[S31] C++：Hello World
来源：http://wap.bbcook.cn/Article/details/gowtdgzbs.sHtML

#include <iostream>
来源：http://www.blog.tarul.cn/Article/details/gqreloibh.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://baike.yfazqb.com/Article/details/gzhmfhgxe.sHtML

[S32] C++：字符串
来源：http://www.blog.tarul.cn/Article/details/guopwcpvk.sHtML

std::string s = "hi";  s += "!";
来源：http://read.share.tarul.cn/Article/details/gjhrlgdxf.sHtML

[S33] C++：vector 增删
来源：http://blog.epnwcf.com/Article/details/gazrqhigp.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.share.epnwcf.com/Article/details/ggrzhigme.sHtML

[S34] C++：遍历 vector
来源：http://mobile.bbcook.cn/Article/details/gfswacwft.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://blog.bbcook.cn/Article/details/gxcfbfjtt.sHtML

[S35] C++：map
来源：http://www.blog.vehdjk.com/Article/details/ghgdeoltx.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.vehdjk.com/Article/details/gqahocuxq.sHtML

[S36] C++：unordered_map
来源：http://mobile.yfazqb.com/Article/details/gplelzyso.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.tarul.cn/Article/details/gadmksezr.sHtML

[S37] C++：set
来源：http://blog.tarul.cn/Article/details/gjjofksjm.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wap.fktsv.cn/Article/details/gsivjclzz.sHtML

[S38] C++：排序
来源：http://m.share.vehdjk.com/Article/details/gqduxymyw.sHtML

std::sort(v.begin(), v.end());
来源：http://baike.epnwcf.com/Article/details/gcyfnxdlt.sHtML

[S39] C++：自定义比较器排序
来源：http://www.share.tarul.cn/Article/details/gqpmtoqns.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.m.share.yfazqb.com/Article/details/giiqbyzzs.sHtML

[S40] C++：查找元素
来源：http://www.blog.bbcook.cn/Article/details/gnhtyrpan.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.m.share.fktsv.cn/Article/details/gulagirzt.sHtML

[S41] C++：类与构造函数
来源：http://3g.fktsv.cn/Article/details/guxkelwoa.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://blog.yfazqb.com/Article/details/gqacontps.sHtML

[S42] C++：继承与虚函数
来源：http://www.blog.sjlbkw.cn/Article/details/glrvglpui.sHtML

class B : public Base { public: void f() override {} };
来源：http://read.share.yfazqb.com/Article/details/gpiepnxrl.sHtML

[S43] C++：智能指针
来源：http://www.blog.yfazqb.com/Article/details/gxximtywc.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.blog.epnwcf.com/Article/details/gnzszqcdc.sHtML

[S44] C++：引用传参
来源：http://3g.sjlbkw.cn/Article/details/gaefydafo.sHtML

void inc(int &x) { ++x; }
来源：http://www.share.bbcook.cn/Article/details/ghxxxakyl.sHtML

[S45] C++：lambda
来源：http://mobile.bbcook.cn/Article/details/girwidmpb.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://wap.bbcook.cn/Article/details/gppqqcwtc.sHtML

[S46] C++：函数模板
来源：http://www.blog.yfazqb.com/Article/details/gixvavycz.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://mobile.yfazqb.com/Article/details/gfcwjssqe.sHtML

[S47] C++：结构化绑定遍历
来源：http://m.share.yfazqb.com/Article/details/gevpknrce.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://mobile.tarul.cn/Article/details/gydalotjx.sHtML

[S48] C++：逐行读文件
来源：http://blog.sjlbkw.cn/Article/details/geidjwpmm.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://baike.vehdjk.com/Article/details/gfdwbkusu.sHtML

while (std::getline(in, line)) { }
来源：http://www.share.epnwcf.com/Article/details/gzrejxync.sHtML

[S49] C++：写文件
来源：http://read.share.sjlbkw.cn/Article/details/gwubacmeg.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://blog.epnwcf.com/Article/details/gmfphfuip.sHtML

[S50] C++：格式化数字
来源：http://wap.vehdjk.com/Article/details/gmbqbhjoj.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.blog.yfazqb.com/Article/details/gykpirthi.sHtML

[S51] C++：显式类型转换
来源：http://m.share.tarul.cn/Article/details/gydohhbsq.sHtML

static_cast<double>(a) / b
来源：http://read.share.fktsv.cn/Article/details/gifhdyzbg.sHtML

[S52] C++：const 与 noexcept
来源：http://read.share.sjlbkw.cn/Article/details/ghpzvqjbz.sHtML

int size() const noexcept { return n_; }
来源：http://baike.bbcook.cn/Article/details/grpkdorit.sHtML

[S53] C++：移动语义
来源：http://blog.tarul.cn/Article/details/gbxreccgz.sHtML

std::vector<int> w = std::move(v);
来源：http://wap.tarul.cn/Article/details/gbnrieuui.sHtML

[S54] C++：异常处理
来源：http://mobile.sjlbkw.cn/Article/details/gohztubqv.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://mobile.sjlbkw.cn/Article/details/gvfffdcwo.sHtML

[S55] C++：结构化绑定
来源：http://3g.vehdjk.com/Article/details/gdvkylisv.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://3g.vehdjk.com/Article/details/gbiaahtzc.sHtML

[S56] C++：optional
来源：http://blog.sjlbkw.cn/Article/details/gbkbvqgjw.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://read.share.tarul.cn/Article/details/gtxvpujaj.sHtML

[S57] C++：编译期常量
来源：http://baike.sjlbkw.cn/Article/details/gvhnlqpqh.sHtML

constexpr int N = 10;
来源：http://www.share.vehdjk.com/Article/details/gejebiqmd.sHtML

[S58] C++：命名空间
来源：http://3g.tarul.cn/Article/details/gadtafygx.sHtML

namespace ns { int f() { return 1; } }
来源：http://mobile.epnwcf.com/Article/details/gkntkndcu.sHtML

[S59] C++：静态断言
来源：http://3g.vehdjk.com/Article/details/gtrsjarrw.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://blog.vehdjk.com/Article/details/gobhgccks.sHtML

[S60] C++：遍历并删除元素
来源：http://read.share.epnwcf.com/Article/details/gyehwxriu.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://read.share.yfazqb.com/Article/details/gmisnnsrf.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/gowpogirg.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.bbcook.cn/Article/details/gzkgdzrlr.sHtML

================================================================================
来源：http://3g.epnwcf.com/Article/details/gvlxrjnjn.sHtML

[T01] Kotlin：Hello World
来源：http://www.blog.sjlbkw.cn/Article/details/gzkttzyrn.sHtML

println("Hello")
来源：http://baike.fktsv.cn/Article/details/guwsgbjij.sHtML

[T02] Kotlin：变量
来源：http://baike.tarul.cn/Article/details/gocbfmbeg.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://wap.epnwcf.com/Article/details/gxrjaepgi.sHtML

[T03] Kotlin：字符串模板
来源：http://www.share.bbcook.cn/Article/details/gplajplqo.sHtML

"值: $b"
来源：http://baike.fktsv.cn/Article/details/gwmtpbpbf.sHtML

[T04] Kotlin：空安全
来源：http://www.m.share.yfazqb.com/Article/details/gispdgzoc.sHtML

val n: String? = null;  n?.length
来源：http://www.share.fktsv.cn/Article/details/gpjvisxfa.sHtML

[T05] Kotlin：when 表达式
来源：http://www.share.bbcook.cn/Article/details/gqdyyptgg.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://mobile.bbcook.cn/Article/details/ghzakpfxc.sHtML

[T06] Kotlin：集合映射
来源：http://3g.fktsv.cn/Article/details/gcefoidkx.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://baike.sjlbkw.cn/Article/details/gxzswxksq.sHtML

[T07] Kotlin：集合过滤
来源：http://www.share.sjlbkw.cn/Article/details/gfnbkpbpv.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.m.share.yfazqb.com/Article/details/gvnhhrvmm.sHtML

[T08] Kotlin：数据类
来源：http://wap.epnwcf.com/Article/details/gnspvqjhj.sHtML

data class User(val name: String, val age: Int)
来源：http://wap.bbcook.cn/Article/details/ghoxjqjil.sHtML


<!-- 参考信息 -->