代发 wailian999

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://wap.vehdjk.com/Article/details/gxtahxgts.sHtML

[R16] until 等待条件
来源：http://m.share.sjlbkw.cn/Article/details/ggmvyebyw.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://m.share.bbcook.cn/Article/details/gkzmorukf.sHtML

[R17] 数组定义与取值
来源：http://blog.vehdjk.com/Article/details/gbofxddrn.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.blog.fktsv.cn/Article/details/grkkvwusj.sHtML

[R18] 遍历数组
来源：http://wap.yfazqb.com/Article/details/gricrkjvu.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.blog.yfazqb.com/Article/details/ghhvoxwcq.sHtML

[R19] 数组长度
来源：http://www.m.share.tarul.cn/Article/details/gnftvakpb.sHtML

echo "${#arr[@]}"
来源：http://m.share.bbcook.cn/Article/details/gshyyfetf.sHtML

[R20] 关联数组（字典）
来源：http://blog.fktsv.cn/Article/details/gketzzyfs.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://m.share.vehdjk.com/Article/details/grsfjpjjp.sHtML

[R21] 字符串长度
来源：http://www.m.share.epnwcf.com/Article/details/gpkoogaxr.sHtML

echo "${#s}"
来源：http://m.share.tarul.cn/Article/details/gjoocaknr.sHtML

[R22] 截取子串
来源：http://mobile.yfazqb.com/Article/details/gclxwqfan.sHtML

echo "${s:0:5}"
来源：http://read.share.epnwcf.com/Article/details/gcteyptgg.sHtML

[R23] 字符串替换
来源：http://read.share.epnwcf.com/Article/details/gnzczvieh.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://m.share.vehdjk.com/Article/details/gbabwucaa.sHtML

[R24] 大小写转换
来源：http://www.share.epnwcf.com/Article/details/goovrtlek.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://read.share.sjlbkw.cn/Article/details/gtjflwzqz.sHtML

[R25] 去后缀 / 去前缀
来源：http://m.share.fktsv.cn/Article/details/gprkceodw.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.share.vehdjk.com/Article/details/gaamfgrgo.sHtML

[R26] 命令替换
来源：http://m.share.vehdjk.com/Article/details/gewhawuud.sHtML

now=$(date +%F); echo "$now"
来源：http://wap.yfazqb.com/Article/details/giboxidkp.sHtML

[R27] 算术展开
来源：http://m.share.bbcook.cn/Article/details/gblvvdojh.sHtML

echo $((1 + 2 * 3))
来源：http://blog.bbcook.cn/Article/details/gxqfhqsue.sHtML

[R28] 浮点运算
来源：http://mobile.vehdjk.com/Article/details/gjwsbcabi.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.blog.epnwcf.com/Article/details/gxkzflzhv.sHtML

[R29] 定义函数
来源：http://www.blog.vehdjk.com/Article/details/gxanbfoks.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://mobile.bbcook.cn/Article/details/gcqikhpbz.sHtML

[R30] 函数返回状态码
来源：http://www.blog.tarul.cn/Article/details/ghorultda.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://3g.epnwcf.com/Article/details/ggosnuidg.sHtML

[R31] 局部变量
来源：http://www.share.yfazqb.com/Article/details/gvtimgbqz.sHtML

f() { local x=1; echo "$x"; }
来源：http://m.share.vehdjk.com/Article/details/golcwaoqi.sHtML

[R32] 参数个数校验
来源：http://m.share.yfazqb.com/Article/details/ghirrdcmp.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://mobile.bbcook.cn/Article/details/gqutkpfgg.sHtML

[R33] 捕获错误并提示行号
来源：http://3g.yfazqb.com/Article/details/gvkaureut.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.share.bbcook.cn/Article/details/ghudxraug.sHtML

[R34] 退出时清理
来源：http://www.share.tarul.cn/Article/details/grsmpdhnz.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.vehdjk.com/Article/details/gqwikpzsi.sHtML

[R35] 后台执行并等待
来源：http://baike.tarul.cn/Article/details/gdakvamkq.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://3g.vehdjk.com/Article/details/gzhfrvptn.sHtML

[R36] 并发执行多个任务
来源：http://wap.bbcook.cn/Article/details/gpwwaaslb.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://read.share.fktsv.cn/Article/details/ggubmnjez.sHtML

[R37] 把输出赋给变量
来源：http://www.share.tarul.cn/Article/details/gsjryaqbe.sHtML

files=$(ls -1)
来源：http://wap.sjlbkw.cn/Article/details/gvxghhcbh.sHtML

[R38] 管道串联
来源：http://blog.epnwcf.com/Article/details/glymnrjah.sHtML

cat a.txt | grep -i error | wc -l
来源：http://read.share.vehdjk.com/Article/details/gaorwjczh.sHtML

[R39] 重定向标准输出与错误
来源：http://mobile.fktsv.cn/Article/details/gluvlppkj.sHtML

cmd > out.log 2>&1
来源：http://read.share.bbcook.cn/Article/details/gspraqlyv.sHtML

[R40] 追加写日志
来源：http://3g.bbcook.cn/Article/details/gfadxjxim.sHtML

echo "log" >> out.log
来源：http://baike.yfazqb.com/Article/details/goklfpxhh.sHtML

[R41] 丢弃输出
来源：http://blog.vehdjk.com/Article/details/gwgkbhgcp.sHtML

cmd >/dev/null 2>&1
来源：http://read.share.vehdjk.com/Article/details/gkzkonazj.sHtML

[R42] 输入重定向
来源：http://wap.vehdjk.com/Article/details/gtuyvfdpy.sHtML

wc -l < a.txt
来源：http://m.share.epnwcf.com/Article/details/gljqkallt.sHtML

[R43] 按名字查找文件
来源：http://www.share.vehdjk.com/Article/details/gknmxvpcm.sHtML

find . -name "*.log" -type f
来源：http://3g.fktsv.cn/Article/details/gqknsqzpg.sHtML

[R44] 按修改时间查找
来源：http://baike.tarul.cn/Article/details/gehpteufl.sHtML

find . -mtime -7 -type f
来源：http://3g.bbcook.cn/Article/details/gbshwigly.sHtML

[R45] 批量删除
来源：http://wap.epnwcf.com/Article/details/gwmzupcif.sHtML

find . -name "*.tmp" -delete
来源：http://www.blog.bbcook.cn/Article/details/gtafmsufo.sHtML

[R46] 递归替换文件内容
来源：http://www.blog.yfazqb.com/Article/details/gbmxyhaci.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://read.share.epnwcf.com/Article/details/gmunxnbdv.sHtML

[R47] sed 单行替换
来源：http://3g.tarul.cn/Article/details/grfjyxhjh.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://read.share.yfazqb.com/Article/details/gcgmimqsp.sHtML

[R48] awk 取指定列
来源：http://baike.sjlbkw.cn/Article/details/goqtohfue.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.m.share.sjlbkw.cn/Article/details/gcfzupigd.sHtML

[R49] awk 带条件
来源：http://read.share.vehdjk.com/Article/details/gnwmdxkop.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.blog.yfazqb.com/Article/details/gilndwsgo.sHtML

[R50] awk 求和
来源：http://mobile.yfazqb.com/Article/details/gdvwhanlt.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://m.share.tarul.cn/Article/details/gefmoczce.sHtML

[R51] 排序去重取前几
来源：http://www.blog.sjlbkw.cn/Article/details/gpocdhsbj.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://blog.vehdjk.com/Article/details/gblmybpyf.sHtML

[R52] 统计行数
来源：http://m.share.sjlbkw.cn/Article/details/gnssyoreh.sHtML

wc -l a.txt
来源：http://3g.yfazqb.com/Article/details/gtjkktryn.sHtML

[R53] 查看文件头与实时尾
来源：http://read.share.epnwcf.com/Article/details/ghnytwezu.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://m.share.tarul.cn/Article/details/gmmbnsqtw.sHtML

[R54] 比较两个文件
来源：http://www.m.share.epnwcf.com/Article/details/genuiyuyk.sHtML

diff a.txt b.txt
来源：http://www.m.share.vehdjk.com/Article/details/gdwdyzfhl.sHtML

[R55] 压缩与解压
来源：http://blog.fktsv.cn/Article/details/gdifpxurx.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://m.share.epnwcf.com/Article/details/gpsqeyjah.sHtML

[R56] 远程拷贝
来源：http://m.share.yfazqb.com/Article/details/gboldwynm.sHtML

scp file user@host:/path/
来源：http://www.m.share.tarul.cn/Article/details/glwshgqdd.sHtML

[R57] 远程执行命令
来源：http://www.blog.vehdjk.com/Article/details/gkitacrvg.sHtML

ssh user@host 'uptime'
来源：http://baike.fktsv.cn/Article/details/glhscqfci.sHtML

[R58] 下载文件
来源：http://www.share.tarul.cn/Article/details/goisjobkn.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.share.yfazqb.com/Article/details/gzefjbmka.sHtML

[R59] 发 POST JSON
来源：http://read.share.vehdjk.com/Article/details/geuaoggwo.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://3g.vehdjk.com/Article/details/gqtdjtoir.sHtML

[R60] 只看 HTTP 状态码
来源：http://baike.tarul.cn/Article/details/gjootohqs.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mobile.epnwcf.com/Article/details/gixawpchd.sHtML

[R61] 磁盘占用
来源：http://www.blog.fktsv.cn/Article/details/gugyttusa.sHtML

df -h;  du -sh *
来源：http://wap.tarul.cn/Article/details/gzimtomhr.sHtML

[R62] 找最占空间的文件
来源：http://www.m.share.fktsv.cn/Article/details/gscxmekri.sHtML

du -ah . | sort -rh | head -10
来源：http://baike.vehdjk.com/Article/details/gtbpakdjv.sHtML

[R63] 内存与进程
来源：http://blog.vehdjk.com/Article/details/gbfmvlcdv.sHtML

free -h;  ps aux | grep nginx
来源：http://blog.yfazqb.com/Article/details/guknqsujr.sHtML

[R64] 结束进程
来源：http://www.blog.epnwcf.com/Article/details/gfdnadmzm.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.blog.sjlbkw.cn/Article/details/gpmwemncx.sHtML

[R65] 查看端口占用
来源：http://blog.sjlbkw.cn/Article/details/gwldviayx.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.share.fktsv.cn/Article/details/ghcdmjuxr.sHtML

[R66] 定时任务
来源：http://mobile.bbcook.cn/Article/details/gobvjqmtc.sHtML

crontab -e;  crontab -l
来源：http://read.share.sjlbkw.cn/Article/details/gaztbvavt.sHtML

[R67] 生成随机十六进制串
来源：http://wap.fktsv.cn/Article/details/gsttfinyc.sHtML

openssl rand -hex 16
来源：http://www.share.tarul.cn/Article/details/gzyyutyph.sHtML

[R68] 计算文件校验值
来源：http://wap.yfazqb.com/Article/details/gnptchybv.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://mobile.fktsv.cn/Article/details/gwlakybvm.sHtML

[R69] 生成随机密码
来源：http://wap.yfazqb.com/Article/details/gmtyyelal.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.m.share.sjlbkw.cn/Article/details/gattnnoii.sHtML

[R70] 时间戳与互转
来源：http://read.share.yfazqb.com/Article/details/ghardqcsz.sHtML

date +%s;  date -d @1700000000
来源：http://www.share.sjlbkw.cn/Article/details/gvdnurfka.sHtML

[R71] 日期格式化
来源：http://baike.yfazqb.com/Article/details/gyntxtbjf.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://m.share.epnwcf.com/Article/details/gnaijmpus.sHtML

[R72] 等待端口就绪
来源：http://3g.tarul.cn/Article/details/gafqxokpk.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://read.share.fktsv.cn/Article/details/gfnmdgioh.sHtML

[R73] 分割大日志
来源：http://www.blog.epnwcf.com/Article/details/gdwemejrd.sHtML

split -l 1000 big.log part_
来源：http://m.share.epnwcf.com/Article/details/gqmuiiclx.sHtML

[R74] 批量重命名
来源：http://www.share.vehdjk.com/Article/details/gjhrejylw.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://mobile.vehdjk.com/Article/details/gcjdtzbtr.sHtML

[R75] 导出环境变量
来源：http://baike.bbcook.cn/Article/details/giwfssudn.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://3g.fktsv.cn/Article/details/ggakdplhs.sHtML

[R76] 使用临时文件
来源：http://www.m.share.epnwcf.com/Article/details/gbgshydwx.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.share.epnwcf.com/Article/details/gmojmxxhv.sHtML

[R77] 读取用户输入
来源：http://m.share.tarul.cn/Article/details/gynepzwai.sHtML

read -rp "请输入: " ans
来源：http://m.share.vehdjk.com/Article/details/gxerwyerz.sHtML

[R78] 交互式菜单
来源：http://baike.yfazqb.com/Article/details/gmdugnyic.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.m.share.yfazqb.com/Article/details/gbpeghsea.sHtML

[R79] 解析命令行选项
来源：http://baike.bbcook.cn/Article/details/gmuonyjgt.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://m.share.tarul.cn/Article/details/gcslrcddt.sHtML

[R80] 查看脚本执行耗时
来源：http://read.share.yfazqb.com/Article/details/gdaqwaxwr.sHtML

time ./run.sh
来源：http://blog.bbcook.cn/Article/details/gdfhzxlad.sHtML

================================================================================
来源：http://www.share.sjlbkw.cn/Article/details/gwaaqoxfx.sHtML

S. C / C++ 专题
来源：http://www.m.share.bbcook.cn/Article/details/ghtdjcvnc.sHtML

================================================================================
来源：http://wap.sjlbkw.cn/Article/details/gqijmvzrj.sHtML

[S01] C：Hello World
来源：http://baike.vehdjk.com/Article/details/gyadscqwh.sHtML

#include <stdio.h>
来源：http://m.share.vehdjk.com/Article/details/gojoivdeg.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://3g.yfazqb.com/Article/details/gvoveliag.sHtML

[S02] C：变量与格式化输出
来源：http://3g.sjlbkw.cn/Article/details/grnfecrzo.sHtML

int a = 10; printf("%d\n", a);
来源：http://3g.vehdjk.com/Article/details/ghgfqtmgm.sHtML

[S03] C：读入整数
来源：http://read.share.sjlbkw.cn/Article/details/gnqzndagq.sHtML

int x; scanf("%d", &x);
来源：http://baike.tarul.cn/Article/details/gzztscyoc.sHtML

[S04] C：字符串复制
来源：http://www.blog.fktsv.cn/Article/details/gdxftubnx.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://mobile.vehdjk.com/Article/details/gwtbnvbxg.sHtML

[S05] C：字符串长度
来源：http://blog.bbcook.cn/Article/details/grfletech.sHtML

strlen(s)
来源：http://mobile.fktsv.cn/Article/details/gsdujhvzt.sHtML

[S06] C：字符串比较
来源：http://3g.yfazqb.com/Article/details/gwlmcwsbp.sHtML

strcmp(a, b) == 0
来源：http://www.share.yfazqb.com/Article/details/gqfuqdncg.sHtML

[S07] C：数组遍历求和
来源：http://mobile.sjlbkw.cn/Article/details/ghroqdyio.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://blog.bbcook.cn/Article/details/gszdxmerx.sHtML

[S08] C：动态内存分配与释放
来源：http://www.m.share.tarul.cn/Article/details/gzilybiuy.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://blog.tarul.cn/Article/details/gbiitpqap.sHtML

[S09] C：结构体定义与初始化
来源：http://www.m.share.fktsv.cn/Article/details/glnpyhkcy.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://read.share.vehdjk.com/Article/details/ggpqotrdx.sHtML

[S10] C：指针与解引用
来源：http://m.share.bbcook.cn/Article/details/garahjalf.sHtML

int *p = &a;  *p = 5;
来源：http://mobile.tarul.cn/Article/details/glajkunjp.sHtML

[S11] C：逐行读文件
来源：http://baike.fktsv.cn/Article/details/gpdhtuzmb.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://wap.fktsv.cn/Article/details/gfdywajtl.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.blog.vehdjk.com/Article/details/gmcnvfxze.sHtML

fclose(f);
来源：http://read.share.fktsv.cn/Article/details/gdlgcsyqv.sHtML

[S12] C：写文件
来源：http://3g.epnwcf.com/Article/details/gtlzaklxy.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mobile.tarul.cn/Article/details/gzxpuktja.sHtML

[S13] C：宏定义
来源：http://mobile.epnwcf.com/Article/details/gpuykftzm.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://baike.bbcook.cn/Article/details/gysiohvhc.sHtML

[S14] C：枚举
来源：http://wap.yfazqb.com/Article/details/gweoshosv.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.blog.yfazqb.com/Article/details/geyvtzqmq.sHtML

[S15] C：类型转换
来源：http://www.blog.yfazqb.com/Article/details/govnghiji.sHtML

(double) a / b
来源：http://www.blog.bbcook.cn/Article/details/gfnhfwrox.sHtML

[S16] C：位操作置位
来源：http://mobile.tarul.cn/Article/details/gwbyarjkk.sHtML

x |= (1 << 3);
来源：http://www.share.vehdjk.com/Article/details/gtkhvrahm.sHtML

[S17] C：安全拼接字符串
来源：http://m.share.fktsv.cn/Article/details/gjrqubwwv.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://blog.sjlbkw.cn/Article/details/gyydhcqms.sHtML

[S18] C：命令行参数
来源：http://read.share.vehdjk.com/Article/details/gdooqqzlp.sHtML

int main(int argc, char **argv)
来源：http://read.share.vehdjk.com/Article/details/ggtpurllu.sHtML

[S19] C：快速排序
来源：http://mobile.epnwcf.com/Article/details/glzwmboqs.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://read.share.fktsv.cn/Article/details/gmgivtvmp.sHtML

[S20] C：二分查找
来源：http://baike.vehdjk.com/Article/details/gghyqqqnd.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://blog.sjlbkw.cn/Article/details/gwoshambs.sHtML

[S21] C：字符类别判断
来源：http://mobile.sjlbkw.cn/Article/details/glnjzlnsu.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://3g.sjlbkw.cn/Article/details/ggjvkjotv.sHtML

[S22] C：字符串转数字
来源：http://www.share.yfazqb.com/Article/details/gneefmawl.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://mobile.fktsv.cn/Article/details/gybeifiyl.sHtML

[S23] C：随机数
来源：http://www.m.share.yfazqb.com/Article/details/gtriqjroj.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://m.share.epnwcf.com/Article/details/gzhnqjnkl.sHtML

[S24] C：获取本地时间
来源：http://www.m.share.yfazqb.com/Article/details/guefqychp.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://baike.yfazqb.com/Article/details/gvxqjenjo.sHtML

[S25] C：内存拷贝
来源：http://m.share.yfazqb.com/Article/details/gdrhmkdng.sHtML

memcpy(dst, src, n);
来源：http://www.share.sjlbkw.cn/Article/details/guoiqkebl.sHtML

[S26] C：内存清零
来源：http://blog.yfazqb.com/Article/details/gkyvewuem.sHtML

memset(a, 0, sizeof a);
来源：http://wap.vehdjk.com/Article/details/gtvmgiuah.sHtML

[S27] C：定义常量
来源：http://www.blog.vehdjk.com/Article/details/gixpasxrh.sHtML

const double PI = 3.14159;
来源：http://mobile.fktsv.cn/Article/details/gdcomdfhl.sHtML

[S28] C：静态变量
来源：http://www.blog.yfazqb.com/Article/details/gyvdijmii.sHtML

static int counter = 0;
来源：http://m.share.bbcook.cn/Article/details/gzthugjpw.sHtML

[S29] C：变参函数
来源：http://m.share.vehdjk.com/Article/details/gjakgovbq.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://3g.yfazqb.com/Article/details/ghjefcnmu.sHtML

[S30] C：头文件保护
来源：http://3g.fktsv.cn/Article/details/gzlhdxqiy.sHtML

#ifndef X_H
来源：http://wap.sjlbkw.cn/Article/details/ghnrazrzl.sHtML

#define X_H
来源：http://mobile.yfazqb.com/Article/details/gixtiazbc.sHtML

#endif
来源：http://blog.tarul.cn/Article/details/gdswwjodx.sHtML

[S31] C++：Hello World
来源：http://mobile.tarul.cn/Article/details/gnyzfkzbe.sHtML

#include <iostream>
来源：http://www.blog.yfazqb.com/Article/details/gbeljbpmi.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://3g.yfazqb.com/Article/details/gglwqyjaa.sHtML

[S32] C++：字符串
来源：http://www.share.epnwcf.com/Article/details/gumrleokc.sHtML

std::string s = "hi";  s += "!";
来源：http://m.share.bbcook.cn/Article/details/gpdtghxku.sHtML

[S33] C++：vector 增删
来源：http://read.share.sjlbkw.cn/Article/details/gxysfyifs.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://blog.sjlbkw.cn/Article/details/gwvibzpin.sHtML

[S34] C++：遍历 vector
来源：http://mobile.sjlbkw.cn/Article/details/grryqhmdy.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.share.vehdjk.com/Article/details/gwiuzcits.sHtML

[S35] C++：map
来源：http://www.blog.vehdjk.com/Article/details/gaxyckzab.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://baike.yfazqb.com/Article/details/gcrbxtart.sHtML

[S36] C++：unordered_map
来源：http://wap.bbcook.cn/Article/details/gkwbebdtk.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wap.epnwcf.com/Article/details/gebpyduei.sHtML

[S37] C++：set
来源：http://read.share.tarul.cn/Article/details/gdydgcfyx.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://read.share.vehdjk.com/Article/details/gpvnfayis.sHtML

[S38] C++：排序
来源：http://www.blog.yfazqb.com/Article/details/gwntyzlwe.sHtML

std::sort(v.begin(), v.end());
来源：http://blog.sjlbkw.cn/Article/details/gfmquegdv.sHtML

[S39] C++：自定义比较器排序
来源：http://read.share.sjlbkw.cn/Article/details/gtjlqniqr.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://m.share.vehdjk.com/Article/details/govtgwdmk.sHtML

[S40] C++：查找元素
来源：http://blog.epnwcf.com/Article/details/garovrwxt.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://mobile.epnwcf.com/Article/details/gjqsygzrd.sHtML

[S41] C++：类与构造函数
来源：http://read.share.vehdjk.com/Article/details/gjxkecjgd.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://3g.tarul.cn/Article/details/gjlcqljdk.sHtML

[S42] C++：继承与虚函数
来源：http://m.share.bbcook.cn/Article/details/gnxytxtcz.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.share.tarul.cn/Article/details/guygdvqds.sHtML

[S43] C++：智能指针
来源：http://m.share.bbcook.cn/Article/details/ggnlntxot.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.share.bbcook.cn/Article/details/gjxfrobgc.sHtML

[S44] C++：引用传参
来源：http://baike.sjlbkw.cn/Article/details/gydsrvscu.sHtML

void inc(int &x) { ++x; }
来源：http://baike.vehdjk.com/Article/details/gwnimzkwc.sHtML

[S45] C++：lambda
来源：http://www.share.tarul.cn/Article/details/ghqrqtrpm.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://baike.tarul.cn/Article/details/gwzxjynyt.sHtML

[S46] C++：函数模板
来源：http://mobile.bbcook.cn/Article/details/gdiekalxq.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://3g.vehdjk.com/Article/details/gkhypyvey.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.share.sjlbkw.cn/Article/details/gkkvraawq.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://baike.sjlbkw.cn/Article/details/gvqeaoosz.sHtML

[S48] C++：逐行读文件
来源：http://read.share.sjlbkw.cn/Article/details/gvdjofbsm.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.share.tarul.cn/Article/details/gpthajlpd.sHtML

while (std::getline(in, line)) { }
来源：http://www.m.share.bbcook.cn/Article/details/gcphwqjcn.sHtML

[S49] C++：写文件
来源：http://www.blog.vehdjk.com/Article/details/gfaudqcna.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.share.bbcook.cn/Article/details/gqhbexnhh.sHtML

[S50] C++：格式化数字
来源：http://mobile.sjlbkw.cn/Article/details/gltrouont.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://3g.epnwcf.com/Article/details/gmfjzbmpx.sHtML

[S51] C++：显式类型转换
来源：http://www.blog.bbcook.cn/Article/details/grgxnlpkj.sHtML

static_cast<double>(a) / b
来源：http://m.share.epnwcf.com/Article/details/gzufjuhxx.sHtML

[S52] C++：const 与 noexcept
来源：http://baike.vehdjk.com/Article/details/glqexzlrt.sHtML

int size() const noexcept { return n_; }
来源：http://www.m.share.tarul.cn/Article/details/gpevbjdai.sHtML

[S53] C++：移动语义
来源：http://baike.vehdjk.com/Article/details/gcgbwmlcw.sHtML

std::vector<int> w = std::move(v);
来源：http://mobile.sjlbkw.cn/Article/details/ghhoebyeq.sHtML

[S54] C++：异常处理
来源：http://baike.yfazqb.com/Article/details/gftbeykgw.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.share.tarul.cn/Article/details/gokenvgym.sHtML

[S55] C++：结构化绑定
来源：http://www.m.share.vehdjk.com/Article/details/ghorbadcn.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://mobile.fktsv.cn/Article/details/gxgpebbqs.sHtML

[S56] C++：optional
来源：http://baike.vehdjk.com/Article/details/gyannqeis.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.m.share.fktsv.cn/Article/details/guejytelq.sHtML

[S57] C++：编译期常量
来源：http://baike.sjlbkw.cn/Article/details/gtcwlnnsb.sHtML

constexpr int N = 10;
来源：http://read.share.tarul.cn/Article/details/gzjhtbqgo.sHtML

[S58] C++：命名空间
来源：http://m.share.yfazqb.com/Article/details/gaielituy.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.m.share.vehdjk.com/Article/details/gypdvylol.sHtML

[S59] C++：静态断言
来源：http://mobile.fktsv.cn/Article/details/gigqypotl.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://baike.sjlbkw.cn/Article/details/gcqdtfkta.sHtML

[S60] C++：遍历并删除元素
来源：http://mobile.yfazqb.com/Article/details/ggxmacvnr.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://m.share.tarul.cn/Article/details/gxmjtmwpc.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/gmzvcosos.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://baike.vehdjk.com/Article/details/gnoxkntfu.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/ggsonzeem.sHtML

[T01] Kotlin：Hello World
来源：http://wap.vehdjk.com/Article/details/gsmfgvnvx.sHtML

println("Hello")
来源：http://www.share.bbcook.cn/Article/details/gwzywpefv.sHtML

[T02] Kotlin：变量
来源：http://www.m.share.bbcook.cn/Article/details/gflrgpluv.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://baike.fktsv.cn/Article/details/gowdqhpjk.sHtML

[T03] Kotlin：字符串模板
来源：http://m.share.tarul.cn/Article/details/gknvetgma.sHtML

"值: $b"
来源：http://www.blog.sjlbkw.cn/Article/details/gbgporljw.sHtML

[T04] Kotlin：空安全
来源：http://baike.epnwcf.com/Article/details/gjdcbhovr.sHtML

val n: String? = null;  n?.length
来源：http://wap.vehdjk.com/Article/details/gnrhlaamk.sHtML

[T05] Kotlin：when 表达式
来源：http://3g.vehdjk.com/Article/details/gcgiffcyz.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://baike.tarul.cn/Article/details/gzdjhcsdp.sHtML

[T06] Kotlin：集合映射
来源：http://mobile.epnwcf.com/Article/details/gouaetgoh.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://mobile.epnwcf.com/Article/details/gavnnvxnb.sHtML

[T07] Kotlin：集合过滤
来源：http://www.share.yfazqb.com/Article/details/gfxjunlmh.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://mobile.yfazqb.com/Article/details/gorgxzwiu.sHtML

[T08] Kotlin：数据类
来源：http://m.share.fktsv.cn/Article/details/gbhlnonrs.sHtML

data class User(val name: String, val age: Int)
来源：http://www.share.vehdjk.com/Article/details/gnikzbphy.sHtML

[T09] Kotlin：扩展函数
来源：http://baike.vehdjk.com/Article/details/garjsldnv.sHtML

fun String.exclaim() = this + "!"
来源：http://www.blog.fktsv.cn/Article/details/gttorolpq.sHtML

[T10] Kotlin：默认参数
来源：http://read.share.fktsv.cn/Article/details/gxmiclmqb.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://read.share.sjlbkw.cn/Article/details/gddlfizsc.sHtML

[T11] Kotlin：协程
来源：http://3g.bbcook.cn/Article/details/gbpcgenkn.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://m.share.sjlbkw.cn/Article/details/gjwtpipfz.sHtML

[T12] Kotlin：解构声明
来源：http://read.share.yfazqb.com/Article/details/gmhggvavm.sHtML

val (a, b) = Pair(1, 2)
来源：http://read.share.tarul.cn/Article/details/gprdnnsoj.sHtML

[T13] Kotlin：只读 Map
来源：http://www.blog.tarul.cn/Article/details/gzbrlfegf.sHtML

val m = mapOf("a" to 1)
来源：http://read.share.tarul.cn/Article/details/glekmkyda.sHtML

[T14] Kotlin：循环
来源：http://www.share.bbcook.cn/Article/details/gsebztrbg.sHtML

for (i in 1..10) println(i)
来源：http://www.m.share.bbcook.cn/Article/details/gdzdwmsyv.sHtML

[T15] Kotlin：接口
来源：http://wap.fktsv.cn/Article/details/gwvvnmpkh.sHtML

interface Shape { fun area(): Double }
来源：http://baike.sjlbkw.cn/Article/details/goybuqcau.sHtML

[T16] Swift：Hello World
来源：http://3g.yfazqb.com/Article/details/gwxxolkoi.sHtML

print("Hello")
来源：http://baike.tarul.cn/Article/details/garupqfrp.sHtML

[T17] Swift：变量与常量
来源：http://m.share.vehdjk.com/Article/details/gwtbrasbc.sHtML

var a = 1;  let b = 2
来源：http://3g.bbcook.cn/Article/details/guqeglgvu.sHtML

[T18] Swift：字符串插值
来源：http://3g.tarul.cn/Article/details/gdkugemfp.sHtML

"值: \(b)"
来源：http://blog.fktsv.cn/Article/details/grkgukjzr.sHtML


<!-- 参考信息 -->