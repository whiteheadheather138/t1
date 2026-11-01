代发 wailian999

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://m.share.yfazqb.com/Article/details/gduhsrnsk.sHtML

[R10] 正则匹配
来源：http://www.blog.vehdjk.com/Article/details/gnybtumwm.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.m.share.bbcook.cn/Article/details/gtfsbzxek.sHtML

[R11] case 多分支
来源：http://read.share.bbcook.cn/Article/details/gjhotwbep.sHtML

case "$1" in
来源：http://wap.fktsv.cn/Article/details/gdjspjuxz.sHtML

start) echo "启动" ;;
来源：http://mobile.fktsv.cn/Article/details/gttzlggyc.sHtML

stop)  echo "停止" ;;
来源：http://m.share.fktsv.cn/Article/details/giddskbcj.sHtML

*)     echo "未知命令" ;;
来源：http://3g.tarul.cn/Article/details/gefxdklkm.sHtML

esac
来源：http://read.share.yfazqb.com/Article/details/gtsuxfipp.sHtML

[R12] for 遍历文件
来源：http://baike.yfazqb.com/Article/details/gowczmeqx.sHtML

for f in *.txt; do echo "$f"; done
来源：http://wap.epnwcf.com/Article/details/gxshbeeln.sHtML

[R13] for 计数循环
来源：http://wap.bbcook.cn/Article/details/gaatujkor.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.blog.sjlbkw.cn/Article/details/ghhlyagao.sHtML

[R14] C 风格 for
来源：http://www.share.sjlbkw.cn/Article/details/ghuwcskua.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.blog.yfazqb.com/Article/details/gltczofca.sHtML

[R15] while 逐行读文件
来源：http://www.share.sjlbkw.cn/Article/details/gapwxcjqr.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://3g.tarul.cn/Article/details/gooanvgii.sHtML

[R16] until 等待条件
来源：http://www.m.share.sjlbkw.cn/Article/details/goifomjcz.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://baike.fktsv.cn/Article/details/gkrshpbmz.sHtML

[R17] 数组定义与取值
来源：http://3g.yfazqb.com/Article/details/gfpueduvd.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://3g.yfazqb.com/Article/details/gvnltdvup.sHtML

[R18] 遍历数组
来源：http://mobile.sjlbkw.cn/Article/details/gtbtygvxc.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://blog.fktsv.cn/Article/details/ggihqmxzv.sHtML

[R19] 数组长度
来源：http://www.share.epnwcf.com/Article/details/gkqisueah.sHtML

echo "${#arr[@]}"
来源：http://m.share.bbcook.cn/Article/details/gswrytqyl.sHtML

[R20] 关联数组（字典）
来源：http://www.blog.sjlbkw.cn/Article/details/gwtgtdshg.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://3g.fktsv.cn/Article/details/gqcztgyli.sHtML

[R21] 字符串长度
来源：http://read.share.sjlbkw.cn/Article/details/gyokaoped.sHtML

echo "${#s}"
来源：http://m.share.bbcook.cn/Article/details/gyqrwoxot.sHtML

[R22] 截取子串
来源：http://www.m.share.tarul.cn/Article/details/ghvliofgl.sHtML

echo "${s:0:5}"
来源：http://wap.tarul.cn/Article/details/gxlpafrkw.sHtML

[R23] 字符串替换
来源：http://wap.bbcook.cn/Article/details/gtqatwfpf.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://read.share.fktsv.cn/Article/details/gyuadtfqm.sHtML

[R24] 大小写转换
来源：http://m.share.fktsv.cn/Article/details/gficnoant.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.share.epnwcf.com/Article/details/gecqhelyq.sHtML

[R25] 去后缀 / 去前缀
来源：http://blog.fktsv.cn/Article/details/gfcfbcxmm.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://wap.vehdjk.com/Article/details/gaidzhyld.sHtML

[R26] 命令替换
来源：http://mobile.tarul.cn/Article/details/gxnomtsxc.sHtML

now=$(date +%F); echo "$now"
来源：http://www.share.sjlbkw.cn/Article/details/ghezggjrw.sHtML

[R27] 算术展开
来源：http://www.share.yfazqb.com/Article/details/ghvvkwnas.sHtML

echo $((1 + 2 * 3))
来源：http://blog.sjlbkw.cn/Article/details/gztyndmui.sHtML

[R28] 浮点运算
来源：http://blog.yfazqb.com/Article/details/gfzrdidah.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.share.yfazqb.com/Article/details/gjnwuodri.sHtML

[R29] 定义函数
来源：http://3g.bbcook.cn/Article/details/gvcoagzao.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.m.share.vehdjk.com/Article/details/gkwrpemns.sHtML

[R30] 函数返回状态码
来源：http://read.share.yfazqb.com/Article/details/gdwukhwbs.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://blog.vehdjk.com/Article/details/ghheromgs.sHtML

[R31] 局部变量
来源：http://read.share.sjlbkw.cn/Article/details/gcfuibcbu.sHtML

f() { local x=1; echo "$x"; }
来源：http://mobile.sjlbkw.cn/Article/details/gecapylpw.sHtML

[R32] 参数个数校验
来源：http://www.share.yfazqb.com/Article/details/gitpeywpj.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.blog.sjlbkw.cn/Article/details/gqjljtwmt.sHtML

[R33] 捕获错误并提示行号
来源：http://m.share.tarul.cn/Article/details/ghrbchsdr.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://blog.yfazqb.com/Article/details/gfocpuujc.sHtML

[R34] 退出时清理
来源：http://wap.yfazqb.com/Article/details/gyjorhhnz.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://mobile.vehdjk.com/Article/details/gdnmfpqew.sHtML

[R35] 后台执行并等待
来源：http://www.share.yfazqb.com/Article/details/gutbolako.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://blog.sjlbkw.cn/Article/details/gvajapbxf.sHtML

[R36] 并发执行多个任务
来源：http://www.blog.sjlbkw.cn/Article/details/grqtkmnsi.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://baike.yfazqb.com/Article/details/gotlivxpj.sHtML

[R37] 把输出赋给变量
来源：http://baike.fktsv.cn/Article/details/gnbmnnmyk.sHtML

files=$(ls -1)
来源：http://blog.yfazqb.com/Article/details/gvixszdvh.sHtML

[R38] 管道串联
来源：http://wap.fktsv.cn/Article/details/gwphzwglt.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.m.share.vehdjk.com/Article/details/ggnexzsut.sHtML

[R39] 重定向标准输出与错误
来源：http://baike.bbcook.cn/Article/details/gxuiplbfl.sHtML

cmd > out.log 2>&1
来源：http://www.blog.epnwcf.com/Article/details/gugytxemv.sHtML

[R40] 追加写日志
来源：http://mobile.fktsv.cn/Article/details/gkknzvclk.sHtML

echo "log" >> out.log
来源：http://www.m.share.yfazqb.com/Article/details/gwtximadz.sHtML

[R41] 丢弃输出
来源：http://wap.epnwcf.com/Article/details/gwomeljch.sHtML

cmd >/dev/null 2>&1
来源：http://wap.tarul.cn/Article/details/grgpyxjfm.sHtML

[R42] 输入重定向
来源：http://www.share.fktsv.cn/Article/details/gxodnotby.sHtML

wc -l < a.txt
来源：http://www.share.vehdjk.com/Article/details/guvyxeqij.sHtML

[R43] 按名字查找文件
来源：http://read.share.tarul.cn/Article/details/gxetnisnw.sHtML

find . -name "*.log" -type f
来源：http://mobile.epnwcf.com/Article/details/gcpzvdzmd.sHtML

[R44] 按修改时间查找
来源：http://blog.sjlbkw.cn/Article/details/guvpuvqcf.sHtML

find . -mtime -7 -type f
来源：http://3g.vehdjk.com/Article/details/geqbczoqj.sHtML

[R45] 批量删除
来源：http://blog.yfazqb.com/Article/details/guaqzdzfl.sHtML

find . -name "*.tmp" -delete
来源：http://www.share.sjlbkw.cn/Article/details/gugnncqdo.sHtML

[R46] 递归替换文件内容
来源：http://read.share.fktsv.cn/Article/details/ghrrzcvut.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.blog.vehdjk.com/Article/details/gvauagrjy.sHtML

[R47] sed 单行替换
来源：http://blog.sjlbkw.cn/Article/details/gwohmpyqw.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.blog.yfazqb.com/Article/details/gogvgilvd.sHtML

[R48] awk 取指定列
来源：http://read.share.bbcook.cn/Article/details/gjkngvjjj.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.share.vehdjk.com/Article/details/grbabslpu.sHtML

[R49] awk 带条件
来源：http://baike.sjlbkw.cn/Article/details/ggzbllyel.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://read.share.vehdjk.com/Article/details/gzazmigbw.sHtML

[R50] awk 求和
来源：http://blog.sjlbkw.cn/Article/details/gjxzcwsvt.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://3g.vehdjk.com/Article/details/gjsfuvwjb.sHtML

[R51] 排序去重取前几
来源：http://www.share.vehdjk.com/Article/details/gcqlfomnn.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://wap.bbcook.cn/Article/details/gmnpadgky.sHtML

[R52] 统计行数
来源：http://www.blog.sjlbkw.cn/Article/details/gwscvlyrm.sHtML

wc -l a.txt
来源：http://m.share.bbcook.cn/Article/details/gtpavqfed.sHtML

[R53] 查看文件头与实时尾
来源：http://blog.tarul.cn/Article/details/gdmryijfb.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://read.share.yfazqb.com/Article/details/gwthxaexy.sHtML

[R54] 比较两个文件
来源：http://read.share.fktsv.cn/Article/details/gmqbzkxkq.sHtML

diff a.txt b.txt
来源：http://wap.fktsv.cn/Article/details/grdfyxdjm.sHtML

[R55] 压缩与解压
来源：http://mobile.fktsv.cn/Article/details/gzjoudydt.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://blog.tarul.cn/Article/details/gclcyrega.sHtML

[R56] 远程拷贝
来源：http://mobile.sjlbkw.cn/Article/details/gvppihiuh.sHtML

scp file user@host:/path/
来源：http://www.blog.tarul.cn/Article/details/gfksiqsag.sHtML

[R57] 远程执行命令
来源：http://www.share.epnwcf.com/Article/details/gczryxxrf.sHtML

ssh user@host 'uptime'
来源：http://baike.vehdjk.com/Article/details/gdmeqgeqj.sHtML

[R58] 下载文件
来源：http://www.share.sjlbkw.cn/Article/details/golrlvmda.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://baike.yfazqb.com/Article/details/gacqhjand.sHtML

[R59] 发 POST JSON
来源：http://www.m.share.vehdjk.com/Article/details/gxupnmnkn.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://3g.yfazqb.com/Article/details/gqpldvvwj.sHtML

[R60] 只看 HTTP 状态码
来源：http://m.share.vehdjk.com/Article/details/gpymopmny.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.blog.yfazqb.com/Article/details/gvxlyaazr.sHtML

[R61] 磁盘占用
来源：http://blog.yfazqb.com/Article/details/gftonlrzu.sHtML

df -h;  du -sh *
来源：http://m.share.epnwcf.com/Article/details/gditpfrmg.sHtML

[R62] 找最占空间的文件
来源：http://blog.vehdjk.com/Article/details/gnvvjzuoj.sHtML

du -ah . | sort -rh | head -10
来源：http://m.share.vehdjk.com/Article/details/grcbbyjvz.sHtML

[R63] 内存与进程
来源：http://www.blog.yfazqb.com/Article/details/gowgivvgi.sHtML

free -h;  ps aux | grep nginx
来源：http://wap.sjlbkw.cn/Article/details/glzfieuvo.sHtML

[R64] 结束进程
来源：http://m.share.fktsv.cn/Article/details/gmkjnxtwg.sHtML

kill -9 $(pgrep -f app.py)
来源：http://3g.vehdjk.com/Article/details/ghgzdpbnm.sHtML

[R65] 查看端口占用
来源：http://www.m.share.bbcook.cn/Article/details/gujpfjjgh.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.share.sjlbkw.cn/Article/details/gcnbonqnr.sHtML

[R66] 定时任务
来源：http://www.m.share.vehdjk.com/Article/details/gujyphskp.sHtML

crontab -e;  crontab -l
来源：http://read.share.fktsv.cn/Article/details/gncrwttoz.sHtML

[R67] 生成随机十六进制串
来源：http://www.m.share.epnwcf.com/Article/details/geuljwyii.sHtML

openssl rand -hex 16
来源：http://www.m.share.epnwcf.com/Article/details/gfngqyeik.sHtML

[R68] 计算文件校验值
来源：http://blog.fktsv.cn/Article/details/gihhlroyf.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://blog.bbcook.cn/Article/details/gxfwpbfng.sHtML

[R69] 生成随机密码
来源：http://www.share.epnwcf.com/Article/details/gxzrbxzej.sHtML

head -c 16 /dev/urandom | base64
来源：http://read.share.bbcook.cn/Article/details/grwkectav.sHtML

[R70] 时间戳与互转
来源：http://baike.vehdjk.com/Article/details/gdfxzobjb.sHtML

date +%s;  date -d @1700000000
来源：http://m.share.bbcook.cn/Article/details/gqdesmbyy.sHtML

[R71] 日期格式化
来源：http://baike.sjlbkw.cn/Article/details/gnxqbemmm.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://read.share.sjlbkw.cn/Article/details/gfoqcwkmq.sHtML

[R72] 等待端口就绪
来源：http://m.share.fktsv.cn/Article/details/gheweqrez.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://3g.yfazqb.com/Article/details/gljplgdvf.sHtML

[R73] 分割大日志
来源：http://mobile.sjlbkw.cn/Article/details/gcefcrdsn.sHtML

split -l 1000 big.log part_
来源：http://blog.sjlbkw.cn/Article/details/gggvvblwa.sHtML

[R74] 批量重命名
来源：http://wap.yfazqb.com/Article/details/ggblfkaax.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://mobile.vehdjk.com/Article/details/geterhmdx.sHtML

[R75] 导出环境变量
来源：http://blog.sjlbkw.cn/Article/details/gqkaawvmi.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://wap.epnwcf.com/Article/details/gjavaiejn.sHtML

[R76] 使用临时文件
来源：http://3g.fktsv.cn/Article/details/gctirnxir.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://blog.tarul.cn/Article/details/gmctrwpkp.sHtML

[R77] 读取用户输入
来源：http://baike.bbcook.cn/Article/details/grbesnrsa.sHtML

read -rp "请输入: " ans
来源：http://www.share.sjlbkw.cn/Article/details/gbtxutrpz.sHtML

[R78] 交互式菜单
来源：http://read.share.vehdjk.com/Article/details/gsdmocbsp.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://mobile.yfazqb.com/Article/details/ghyyyjjmq.sHtML

[R79] 解析命令行选项
来源：http://blog.vehdjk.com/Article/details/glqtihljd.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.blog.fktsv.cn/Article/details/gigvlffea.sHtML

[R80] 查看脚本执行耗时
来源：http://blog.fktsv.cn/Article/details/gqvrrkpjn.sHtML

time ./run.sh
来源：http://www.m.share.tarul.cn/Article/details/gxahtgmwl.sHtML

================================================================================
来源：http://3g.epnwcf.com/Article/details/gfteisoxw.sHtML

S. C / C++ 专题
来源：http://www.m.share.epnwcf.com/Article/details/gcatvhlnv.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/gpswnbiir.sHtML

[S01] C：Hello World
来源：http://www.share.epnwcf.com/Article/details/grrblkbzm.sHtML

#include <stdio.h>
来源：http://wap.vehdjk.com/Article/details/gknslzuwr.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://3g.vehdjk.com/Article/details/gxorgwngx.sHtML

[S02] C：变量与格式化输出
来源：http://www.m.share.sjlbkw.cn/Article/details/garormpzj.sHtML

int a = 10; printf("%d\n", a);
来源：http://blog.yfazqb.com/Article/details/gcwnxqejk.sHtML

[S03] C：读入整数
来源：http://www.blog.tarul.cn/Article/details/gvkpbnste.sHtML

int x; scanf("%d", &x);
来源：http://mobile.yfazqb.com/Article/details/gvkznazay.sHtML

[S04] C：字符串复制
来源：http://m.share.sjlbkw.cn/Article/details/gfjwlmwnx.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.share.vehdjk.com/Article/details/gkawnakzk.sHtML

[S05] C：字符串长度
来源：http://baike.epnwcf.com/Article/details/ghfxniqlg.sHtML

strlen(s)
来源：http://blog.yfazqb.com/Article/details/ghtdndhan.sHtML

[S06] C：字符串比较
来源：http://m.share.sjlbkw.cn/Article/details/ggocmrfdo.sHtML

strcmp(a, b) == 0
来源：http://3g.vehdjk.com/Article/details/gepfhnqqk.sHtML

[S07] C：数组遍历求和
来源：http://www.blog.tarul.cn/Article/details/gwfmieqaf.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://wap.fktsv.cn/Article/details/guugzdiji.sHtML

[S08] C：动态内存分配与释放
来源：http://wap.fktsv.cn/Article/details/gxichaqcg.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://baike.fktsv.cn/Article/details/gjpunywkw.sHtML

[S09] C：结构体定义与初始化
来源：http://baike.sjlbkw.cn/Article/details/gouprzmhq.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://baike.sjlbkw.cn/Article/details/gvnatsccl.sHtML

[S10] C：指针与解引用
来源：http://m.share.vehdjk.com/Article/details/gclepbypo.sHtML

int *p = &a;  *p = 5;
来源：http://3g.sjlbkw.cn/Article/details/ggbanbgqm.sHtML

[S11] C：逐行读文件
来源：http://baike.bbcook.cn/Article/details/gqzidumxk.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://3g.bbcook.cn/Article/details/gwoaancrj.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://mobile.vehdjk.com/Article/details/gaxrkezri.sHtML

fclose(f);
来源：http://read.share.yfazqb.com/Article/details/gecwhgoqu.sHtML

[S12] C：写文件
来源：http://mobile.vehdjk.com/Article/details/gyxqdtkvo.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://wap.fktsv.cn/Article/details/gwsidyuqt.sHtML

[S13] C：宏定义
来源：http://m.share.sjlbkw.cn/Article/details/gqlfxyngg.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.m.share.fktsv.cn/Article/details/gxnldmqmp.sHtML

[S14] C：枚举
来源：http://read.share.fktsv.cn/Article/details/gmcofcvoy.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://baike.bbcook.cn/Article/details/gyjelczqj.sHtML

[S15] C：类型转换
来源：http://mobile.fktsv.cn/Article/details/gjufmjuuu.sHtML

(double) a / b
来源：http://m.share.sjlbkw.cn/Article/details/gvmvhbrao.sHtML

[S16] C：位操作置位
来源：http://3g.vehdjk.com/Article/details/ghwglicov.sHtML

x |= (1 << 3);
来源：http://www.blog.epnwcf.com/Article/details/ggskhsmhb.sHtML

[S17] C：安全拼接字符串
来源：http://www.blog.sjlbkw.cn/Article/details/gfgfyclrr.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.blog.epnwcf.com/Article/details/gtwdbillm.sHtML

[S18] C：命令行参数
来源：http://www.m.share.epnwcf.com/Article/details/gvyngzquw.sHtML

int main(int argc, char **argv)
来源：http://www.m.share.vehdjk.com/Article/details/gexcuxrmo.sHtML

[S19] C：快速排序
来源：http://3g.bbcook.cn/Article/details/gvregvenf.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://3g.vehdjk.com/Article/details/gxjwowgst.sHtML

[S20] C：二分查找
来源：http://blog.vehdjk.com/Article/details/gdeokkrmw.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.share.epnwcf.com/Article/details/gnnznydke.sHtML

[S21] C：字符类别判断
来源：http://baike.vehdjk.com/Article/details/ggeuvsbln.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://m.share.fktsv.cn/Article/details/giezmcqvn.sHtML

[S22] C：字符串转数字
来源：http://mobile.sjlbkw.cn/Article/details/gpbdhgvla.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://mobile.epnwcf.com/Article/details/gvsdfmmkw.sHtML

[S23] C：随机数
来源：http://m.share.tarul.cn/Article/details/gwaezaykb.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://3g.fktsv.cn/Article/details/gdbbxzacx.sHtML

[S24] C：获取本地时间
来源：http://read.share.bbcook.cn/Article/details/gmwgcvrtg.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://m.share.yfazqb.com/Article/details/gvizrormj.sHtML

[S25] C：内存拷贝
来源：http://baike.epnwcf.com/Article/details/glhkgvkmd.sHtML

memcpy(dst, src, n);
来源：http://www.m.share.epnwcf.com/Article/details/gzebkbpxm.sHtML

[S26] C：内存清零
来源：http://www.share.epnwcf.com/Article/details/gdjiaaasd.sHtML

memset(a, 0, sizeof a);
来源：http://m.share.bbcook.cn/Article/details/gnntvwpdh.sHtML

[S27] C：定义常量
来源：http://wap.fktsv.cn/Article/details/geauyciry.sHtML

const double PI = 3.14159;
来源：http://www.share.sjlbkw.cn/Article/details/gsxqgkgun.sHtML

[S28] C：静态变量
来源：http://3g.vehdjk.com/Article/details/gyngppvdt.sHtML

static int counter = 0;
来源：http://baike.bbcook.cn/Article/details/gkqkfkluk.sHtML

[S29] C：变参函数
来源：http://mobile.sjlbkw.cn/Article/details/gpcgwyhvk.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.blog.bbcook.cn/Article/details/glysubxbn.sHtML

[S30] C：头文件保护
来源：http://www.share.vehdjk.com/Article/details/ggjmvekmx.sHtML

#ifndef X_H
来源：http://read.share.fktsv.cn/Article/details/gxscpulgh.sHtML

#define X_H
来源：http://wap.epnwcf.com/Article/details/giswtvshg.sHtML

#endif
来源：http://www.blog.vehdjk.com/Article/details/garlbacpc.sHtML

[S31] C++：Hello World
来源：http://www.blog.fktsv.cn/Article/details/gxyejltgc.sHtML

#include <iostream>
来源：http://read.share.tarul.cn/Article/details/gkvcyiahk.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://3g.bbcook.cn/Article/details/gawmzelnu.sHtML

[S32] C++：字符串
来源：http://m.share.fktsv.cn/Article/details/gpfadwuwx.sHtML

std::string s = "hi";  s += "!";
来源：http://blog.fktsv.cn/Article/details/gnsxrurwi.sHtML

[S33] C++：vector 增删
来源：http://baike.tarul.cn/Article/details/gjtqlnzke.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.m.share.sjlbkw.cn/Article/details/gsurdyzrc.sHtML

[S34] C++：遍历 vector
来源：http://www.blog.vehdjk.com/Article/details/gwytwkfqt.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://mobile.yfazqb.com/Article/details/gpavnuewb.sHtML

[S35] C++：map
来源：http://wap.fktsv.cn/Article/details/gmxdmvwrj.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.tarul.cn/Article/details/girkuejun.sHtML

[S36] C++：unordered_map
来源：http://www.m.share.bbcook.cn/Article/details/glglxvltt.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.epnwcf.com/Article/details/gwcixsrwu.sHtML

[S37] C++：set
来源：http://m.share.tarul.cn/Article/details/gajgfbhsk.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://read.share.sjlbkw.cn/Article/details/gdunmcesq.sHtML

[S38] C++：排序
来源：http://www.share.epnwcf.com/Article/details/gfkfulvej.sHtML

std::sort(v.begin(), v.end());
来源：http://www.share.epnwcf.com/Article/details/gzfbnhsyl.sHtML

[S39] C++：自定义比较器排序
来源：http://www.blog.tarul.cn/Article/details/gczqbevnv.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.blog.epnwcf.com/Article/details/gscptoxic.sHtML

[S40] C++：查找元素
来源：http://www.blog.yfazqb.com/Article/details/gqpcfyyjh.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.blog.fktsv.cn/Article/details/gpofenibe.sHtML

[S41] C++：类与构造函数
来源：http://www.blog.epnwcf.com/Article/details/gfbzyjzqt.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://wap.tarul.cn/Article/details/gphdnhomh.sHtML

[S42] C++：继承与虚函数
来源：http://3g.yfazqb.com/Article/details/gdtvshvaw.sHtML

class B : public Base { public: void f() override {} };
来源：http://baike.tarul.cn/Article/details/gisckgpee.sHtML

[S43] C++：智能指针
来源：http://m.share.bbcook.cn/Article/details/gdlhtrpyg.sHtML

auto p = std::make_unique<int>(5);
来源：http://3g.sjlbkw.cn/Article/details/gwkurtiqn.sHtML

[S44] C++：引用传参
来源：http://www.blog.yfazqb.com/Article/details/gyqvbosuk.sHtML

void inc(int &x) { ++x; }
来源：http://wap.tarul.cn/Article/details/gstroohob.sHtML

[S45] C++：lambda
来源：http://www.share.tarul.cn/Article/details/geaxcowqe.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://mobile.vehdjk.com/Article/details/gavurdjxs.sHtML

[S46] C++：函数模板
来源：http://mobile.yfazqb.com/Article/details/gnqrtkxvt.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.m.share.fktsv.cn/Article/details/gqwiztoph.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.blog.epnwcf.com/Article/details/gsgqslkvc.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://m.share.yfazqb.com/Article/details/gpzegculg.sHtML

[S48] C++：逐行读文件
来源：http://www.share.vehdjk.com/Article/details/gdiopmwhr.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://baike.epnwcf.com/Article/details/gayxrhdfi.sHtML

while (std::getline(in, line)) { }
来源：http://www.share.bbcook.cn/Article/details/gorcymmkx.sHtML

[S49] C++：写文件
来源：http://www.m.share.vehdjk.com/Article/details/guzfrbenl.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.share.yfazqb.com/Article/details/gxchskfwi.sHtML

[S50] C++：格式化数字
来源：http://baike.sjlbkw.cn/Article/details/gquwkgvei.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://baike.sjlbkw.cn/Article/details/gqhvokwxa.sHtML

[S51] C++：显式类型转换
来源：http://baike.sjlbkw.cn/Article/details/glgmqauln.sHtML

static_cast<double>(a) / b
来源：http://m.share.fktsv.cn/Article/details/ggklqsntn.sHtML

[S52] C++：const 与 noexcept
来源：http://m.share.sjlbkw.cn/Article/details/gmivyijmz.sHtML

int size() const noexcept { return n_; }
来源：http://www.share.epnwcf.com/Article/details/gmlyhelgb.sHtML

[S53] C++：移动语义
来源：http://www.share.fktsv.cn/Article/details/gtpawoumz.sHtML

std::vector<int> w = std::move(v);
来源：http://www.m.share.yfazqb.com/Article/details/gznmuveez.sHtML

[S54] C++：异常处理
来源：http://www.share.yfazqb.com/Article/details/gnggjeaar.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.m.share.yfazqb.com/Article/details/gejiqeyrp.sHtML

[S55] C++：结构化绑定
来源：http://mobile.fktsv.cn/Article/details/gygilldoc.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://blog.bbcook.cn/Article/details/gljggxzki.sHtML

[S56] C++：optional
来源：http://www.m.share.yfazqb.com/Article/details/gpxtnjxwg.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://3g.sjlbkw.cn/Article/details/ggudkgniz.sHtML

[S57] C++：编译期常量
来源：http://www.blog.fktsv.cn/Article/details/gkgmfiksn.sHtML

constexpr int N = 10;
来源：http://www.m.share.tarul.cn/Article/details/gmceltztm.sHtML

[S58] C++：命名空间
来源：http://m.share.sjlbkw.cn/Article/details/gyrivwexg.sHtML

namespace ns { int f() { return 1; } }
来源：http://m.share.sjlbkw.cn/Article/details/gnkekbdfu.sHtML

[S59] C++：静态断言
来源：http://wap.yfazqb.com/Article/details/gdgbykrnh.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.share.yfazqb.com/Article/details/gelvagtem.sHtML

[S60] C++：遍历并删除元素
来源：http://read.share.vehdjk.com/Article/details/gzozwrjzm.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.m.share.bbcook.cn/Article/details/gxrjqqcfa.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/gsjmthjgn.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://baike.epnwcf.com/Article/details/gfhkmqqzg.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/gojnadczg.sHtML

[T01] Kotlin：Hello World
来源：http://blog.yfazqb.com/Article/details/gvztiogsh.sHtML

println("Hello")
来源：http://blog.bbcook.cn/Article/details/gvlgxhumu.sHtML

[T02] Kotlin：变量
来源：http://blog.epnwcf.com/Article/details/gkfqkpjny.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://blog.epnwcf.com/Article/details/gpffudiou.sHtML

[T03] Kotlin：字符串模板
来源：http://mobile.fktsv.cn/Article/details/gqqhakyns.sHtML

"值: $b"
来源：http://baike.tarul.cn/Article/details/grbdehsca.sHtML

[T04] Kotlin：空安全
来源：http://wap.bbcook.cn/Article/details/gcfybutqb.sHtML

val n: String? = null;  n?.length
来源：http://www.share.epnwcf.com/Article/details/gnrgdqokm.sHtML

[T05] Kotlin：when 表达式
来源：http://www.share.epnwcf.com/Article/details/gdkjfubre.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://m.share.tarul.cn/Article/details/gbwmpwyyp.sHtML

[T06] Kotlin：集合映射
来源：http://www.blog.bbcook.cn/Article/details/gvkkhvrhx.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://m.share.yfazqb.com/Article/details/gzdcixdcm.sHtML

[T07] Kotlin：集合过滤
来源：http://www.share.tarul.cn/Article/details/gwdipgcbr.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.share.epnwcf.com/Article/details/gmedbyvtj.sHtML

[T08] Kotlin：数据类
来源：http://www.blog.fktsv.cn/Article/details/gwnytwfgz.sHtML

data class User(val name: String, val age: Int)
来源：http://m.share.epnwcf.com/Article/details/gurgqzceu.sHtML

[T09] Kotlin：扩展函数
来源：http://3g.epnwcf.com/Article/details/grwnqvccp.sHtML

fun String.exclaim() = this + "!"
来源：http://www.share.fktsv.cn/Article/details/gxhtwhlap.sHtML

[T10] Kotlin：默认参数
来源：http://www.m.share.yfazqb.com/Article/details/gvggdakfd.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://mobile.vehdjk.com/Article/details/glceckajn.sHtML


<!-- 参考信息 -->