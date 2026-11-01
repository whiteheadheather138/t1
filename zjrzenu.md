代发 wailian999

name="${1:-default}"
来源：http://blog.yfazqb.com/Article/details/gfdscmjxi.sHtML

[R06] 判断命令是否存在
来源：http://3g.yfazqb.com/Article/details/gvvynnfrl.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.share.bbcook.cn/Article/details/gwuegqnxp.sHtML

[R07] if 判断文件
来源：http://mobile.fktsv.cn/Article/details/gkmponihv.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://mobile.vehdjk.com/Article/details/gckvmthat.sHtML

[R08] 数值比较
来源：http://mobile.sjlbkw.cn/Article/details/gstxjwhks.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://m.share.epnwcf.com/Article/details/gjyxbgaoz.sHtML

[R09] 字符串比较
来源：http://mobile.tarul.cn/Article/details/gbstqrfso.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://baike.epnwcf.com/Article/details/ghoeudvdh.sHtML

[R10] 正则匹配
来源：http://www.share.fktsv.cn/Article/details/gkdmkdzzv.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.blog.epnwcf.com/Article/details/gkrhkrdid.sHtML

[R11] case 多分支
来源：http://3g.tarul.cn/Article/details/gavzyipqy.sHtML

case "$1" in
来源：http://3g.sjlbkw.cn/Article/details/godkghumm.sHtML

start) echo "启动" ;;
来源：http://wap.bbcook.cn/Article/details/gmxtcqill.sHtML

stop)  echo "停止" ;;
来源：http://blog.bbcook.cn/Article/details/gompvbwmv.sHtML

*)     echo "未知命令" ;;
来源：http://blog.tarul.cn/Article/details/glnugfxpr.sHtML

esac
来源：http://3g.sjlbkw.cn/Article/details/gxvhxtdrg.sHtML

[R12] for 遍历文件
来源：http://blog.yfazqb.com/Article/details/ggoeiefjl.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.blog.tarul.cn/Article/details/gdujcvqrm.sHtML

[R13] for 计数循环
来源：http://www.m.share.tarul.cn/Article/details/gfasaromc.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://m.share.epnwcf.com/Article/details/gtuqybfow.sHtML

[R14] C 风格 for
来源：http://3g.bbcook.cn/Article/details/gtovbuahw.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://m.share.vehdjk.com/Article/details/gpcrrqpey.sHtML

[R15] while 逐行读文件
来源：http://www.blog.fktsv.cn/Article/details/glcyjodby.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://read.share.fktsv.cn/Article/details/gisbtviqj.sHtML

[R16] until 等待条件
来源：http://www.m.share.tarul.cn/Article/details/gxylekpjl.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://m.share.tarul.cn/Article/details/grzvqzlej.sHtML

[R17] 数组定义与取值
来源：http://blog.vehdjk.com/Article/details/gkdqvidgq.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://m.share.fktsv.cn/Article/details/gqwbdzpoy.sHtML

[R18] 遍历数组
来源：http://blog.tarul.cn/Article/details/ggtowxlsl.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://m.share.epnwcf.com/Article/details/ggiwoqliu.sHtML

[R19] 数组长度
来源：http://baike.vehdjk.com/Article/details/gmdhdynof.sHtML

echo "${#arr[@]}"
来源：http://baike.sjlbkw.cn/Article/details/ggqodmohv.sHtML

[R20] 关联数组（字典）
来源：http://read.share.sjlbkw.cn/Article/details/gdtfshnot.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://blog.bbcook.cn/Article/details/godfgmtrf.sHtML

[R21] 字符串长度
来源：http://baike.epnwcf.com/Article/details/giodlavxy.sHtML

echo "${#s}"
来源：http://baike.yfazqb.com/Article/details/gvnzomzgd.sHtML

[R22] 截取子串
来源：http://mobile.yfazqb.com/Article/details/gdvzvbyxv.sHtML

echo "${s:0:5}"
来源：http://www.m.share.fktsv.cn/Article/details/gahuuidma.sHtML

[R23] 字符串替换
来源：http://www.share.epnwcf.com/Article/details/gwbnnlkqk.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.blog.tarul.cn/Article/details/gqjxizuwm.sHtML

[R24] 大小写转换
来源：http://m.share.sjlbkw.cn/Article/details/giwfkykyu.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://m.share.epnwcf.com/Article/details/gfapuctpu.sHtML

[R25] 去后缀 / 去前缀
来源：http://blog.tarul.cn/Article/details/ghkilkkag.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://read.share.epnwcf.com/Article/details/gwypfkajl.sHtML

[R26] 命令替换
来源：http://m.share.tarul.cn/Article/details/gjmianknu.sHtML

now=$(date +%F); echo "$now"
来源：http://3g.sjlbkw.cn/Article/details/gidjgcioz.sHtML

[R27] 算术展开
来源：http://mobile.vehdjk.com/Article/details/gmqvhouzu.sHtML

echo $((1 + 2 * 3))
来源：http://www.share.bbcook.cn/Article/details/gcernzztk.sHtML

[R28] 浮点运算
来源：http://www.blog.yfazqb.com/Article/details/gttciyskn.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.share.epnwcf.com/Article/details/ggxzqobqw.sHtML

[R29] 定义函数
来源：http://mobile.sjlbkw.cn/Article/details/gzlaewajk.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.share.bbcook.cn/Article/details/gvbmknstc.sHtML

[R30] 函数返回状态码
来源：http://3g.yfazqb.com/Article/details/gcoiepzyb.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.m.share.bbcook.cn/Article/details/gdwvzviow.sHtML

[R31] 局部变量
来源：http://read.share.sjlbkw.cn/Article/details/grnlthcmx.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.m.share.yfazqb.com/Article/details/gnigkequw.sHtML

[R32] 参数个数校验
来源：http://wap.bbcook.cn/Article/details/gdukufevu.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.m.share.bbcook.cn/Article/details/gxzhzwyeb.sHtML

[R33] 捕获错误并提示行号
来源：http://blog.epnwcf.com/Article/details/gtgitmvja.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://mobile.tarul.cn/Article/details/gpshiqptz.sHtML

[R34] 退出时清理
来源：http://blog.fktsv.cn/Article/details/gsmuxfhan.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://read.share.vehdjk.com/Article/details/gpxvqatto.sHtML

[R35] 后台执行并等待
来源：http://blog.yfazqb.com/Article/details/grhstgold.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://m.share.sjlbkw.cn/Article/details/gxrwokkca.sHtML

[R36] 并发执行多个任务
来源：http://mobile.fktsv.cn/Article/details/gnczepjup.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://3g.vehdjk.com/Article/details/gafjebfwc.sHtML

[R37] 把输出赋给变量
来源：http://www.share.vehdjk.com/Article/details/gmkykijfd.sHtML

files=$(ls -1)
来源：http://read.share.fktsv.cn/Article/details/ggnjntcib.sHtML

[R38] 管道串联
来源：http://www.blog.tarul.cn/Article/details/gyroqcjdh.sHtML

cat a.txt | grep -i error | wc -l
来源：http://mobile.tarul.cn/Article/details/grdviwoce.sHtML

[R39] 重定向标准输出与错误
来源：http://read.share.tarul.cn/Article/details/gtkglkqcu.sHtML

cmd > out.log 2>&1
来源：http://www.blog.yfazqb.com/Article/details/gptofyisv.sHtML

[R40] 追加写日志
来源：http://mobile.tarul.cn/Article/details/gfikispwh.sHtML

echo "log" >> out.log
来源：http://m.share.vehdjk.com/Article/details/gvopsbazg.sHtML

[R41] 丢弃输出
来源：http://www.share.yfazqb.com/Article/details/gtwwctzdi.sHtML

cmd >/dev/null 2>&1
来源：http://wap.fktsv.cn/Article/details/glubredif.sHtML

[R42] 输入重定向
来源：http://mobile.epnwcf.com/Article/details/gnqhisdxj.sHtML

wc -l < a.txt
来源：http://www.m.share.epnwcf.com/Article/details/gfcfempjs.sHtML

[R43] 按名字查找文件
来源：http://wap.vehdjk.com/Article/details/glnbwsspd.sHtML

find . -name "*.log" -type f
来源：http://baike.yfazqb.com/Article/details/gunyuevaq.sHtML

[R44] 按修改时间查找
来源：http://mobile.bbcook.cn/Article/details/gmeynnppf.sHtML

find . -mtime -7 -type f
来源：http://3g.vehdjk.com/Article/details/gtdnwtarv.sHtML

[R45] 批量删除
来源：http://m.share.bbcook.cn/Article/details/gcjdiflao.sHtML

find . -name "*.tmp" -delete
来源：http://3g.epnwcf.com/Article/details/gxdsyjjqi.sHtML

[R46] 递归替换文件内容
来源：http://m.share.yfazqb.com/Article/details/gcrpskfgd.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://baike.yfazqb.com/Article/details/gdnuwikue.sHtML

[R47] sed 单行替换
来源：http://wap.fktsv.cn/Article/details/ghvxskzvk.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.share.sjlbkw.cn/Article/details/gstcjgtgz.sHtML

[R48] awk 取指定列
来源：http://baike.epnwcf.com/Article/details/gnrlcchhh.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.m.share.epnwcf.com/Article/details/givaijiic.sHtML

[R49] awk 带条件
来源：http://mobile.vehdjk.com/Article/details/gcrtbbaxy.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wap.tarul.cn/Article/details/grwyynhjc.sHtML

[R50] awk 求和
来源：http://3g.yfazqb.com/Article/details/gbkvmyabi.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://3g.epnwcf.com/Article/details/gmtyxxocr.sHtML

[R51] 排序去重取前几
来源：http://baike.epnwcf.com/Article/details/gielctiwx.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://wap.yfazqb.com/Article/details/gxzmfmdkh.sHtML

[R52] 统计行数
来源：http://mobile.epnwcf.com/Article/details/gaycqsgpw.sHtML

wc -l a.txt
来源：http://www.blog.epnwcf.com/Article/details/gdmsqjrrd.sHtML

[R53] 查看文件头与实时尾
来源：http://baike.sjlbkw.cn/Article/details/geaksyjoy.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.share.tarul.cn/Article/details/grhffeeut.sHtML

[R54] 比较两个文件
来源：http://mobile.fktsv.cn/Article/details/gqcwncbfa.sHtML

diff a.txt b.txt
来源：http://wap.yfazqb.com/Article/details/gggetjejr.sHtML

[R55] 压缩与解压
来源：http://www.share.vehdjk.com/Article/details/gmzkufjql.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.m.share.yfazqb.com/Article/details/gcemyrivl.sHtML

[R56] 远程拷贝
来源：http://m.share.fktsv.cn/Article/details/grbvqqvhu.sHtML

scp file user@host:/path/
来源：http://www.blog.sjlbkw.cn/Article/details/gkyrsdyjm.sHtML

[R57] 远程执行命令
来源：http://baike.vehdjk.com/Article/details/gmvfgxzke.sHtML

ssh user@host 'uptime'
来源：http://www.m.share.epnwcf.com/Article/details/gwtatezlz.sHtML

[R58] 下载文件
来源：http://mobile.sjlbkw.cn/Article/details/gadgkysgp.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.blog.fktsv.cn/Article/details/gqbjkpoef.sHtML

[R59] 发 POST JSON
来源：http://wap.bbcook.cn/Article/details/grykzyzus.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.blog.yfazqb.com/Article/details/gvfwjtlgd.sHtML

[R60] 只看 HTTP 状态码
来源：http://mobile.bbcook.cn/Article/details/gmjbehkyt.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.share.sjlbkw.cn/Article/details/gzluhujgs.sHtML

[R61] 磁盘占用
来源：http://mobile.tarul.cn/Article/details/gqwxvgaef.sHtML

df -h;  du -sh *
来源：http://www.m.share.tarul.cn/Article/details/gngjhjdts.sHtML

[R62] 找最占空间的文件
来源：http://mobile.bbcook.cn/Article/details/gveoxsbby.sHtML

du -ah . | sort -rh | head -10
来源：http://baike.vehdjk.com/Article/details/gyqbehgxr.sHtML

[R63] 内存与进程
来源：http://blog.epnwcf.com/Article/details/ghmwyysrd.sHtML

free -h;  ps aux | grep nginx
来源：http://www.share.epnwcf.com/Article/details/gtpzhylip.sHtML

[R64] 结束进程
来源：http://read.share.vehdjk.com/Article/details/gznmrhojp.sHtML

kill -9 $(pgrep -f app.py)
来源：http://m.share.tarul.cn/Article/details/gharszbgj.sHtML

[R65] 查看端口占用
来源：http://www.blog.epnwcf.com/Article/details/gathlngkw.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://blog.epnwcf.com/Article/details/gxmefvooe.sHtML

[R66] 定时任务
来源：http://read.share.yfazqb.com/Article/details/gtsklwgfu.sHtML

crontab -e;  crontab -l
来源：http://mobile.vehdjk.com/Article/details/gxmaorumn.sHtML

[R67] 生成随机十六进制串
来源：http://wap.tarul.cn/Article/details/gwtcdtwpz.sHtML

openssl rand -hex 16
来源：http://read.share.tarul.cn/Article/details/gurxczwac.sHtML

[R68] 计算文件校验值
来源：http://www.blog.sjlbkw.cn/Article/details/gjivdllzk.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.share.bbcook.cn/Article/details/gfxfzzdtz.sHtML

[R69] 生成随机密码
来源：http://blog.sjlbkw.cn/Article/details/gzasrqvtx.sHtML

head -c 16 /dev/urandom | base64
来源：http://baike.epnwcf.com/Article/details/gxnesvaoe.sHtML

[R70] 时间戳与互转
来源：http://mobile.vehdjk.com/Article/details/gkioswwim.sHtML

date +%s;  date -d @1700000000
来源：http://wap.sjlbkw.cn/Article/details/gxmthxbxa.sHtML

[R71] 日期格式化
来源：http://www.blog.fktsv.cn/Article/details/gkqfzifof.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.m.share.fktsv.cn/Article/details/gvxdubfxg.sHtML

[R72] 等待端口就绪
来源：http://baike.sjlbkw.cn/Article/details/geixcaayl.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.m.share.sjlbkw.cn/Article/details/gyayftatw.sHtML

[R73] 分割大日志
来源：http://blog.tarul.cn/Article/details/gbzfeowka.sHtML

split -l 1000 big.log part_
来源：http://m.share.epnwcf.com/Article/details/gidfykjkk.sHtML

[R74] 批量重命名
来源：http://read.share.tarul.cn/Article/details/gdafppymo.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://3g.vehdjk.com/Article/details/gtjbfcuxd.sHtML

[R75] 导出环境变量
来源：http://wap.vehdjk.com/Article/details/gulfyuaxi.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.blog.yfazqb.com/Article/details/gkgyxgnht.sHtML

[R76] 使用临时文件
来源：http://3g.sjlbkw.cn/Article/details/gpwipaqpq.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://read.share.sjlbkw.cn/Article/details/gdzinpxty.sHtML

[R77] 读取用户输入
来源：http://baike.vehdjk.com/Article/details/gbhnbucck.sHtML

read -rp "请输入: " ans
来源：http://www.m.share.bbcook.cn/Article/details/gwuqyvzop.sHtML

[R78] 交互式菜单
来源：http://www.m.share.epnwcf.com/Article/details/goaedoznz.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://baike.bbcook.cn/Article/details/gnzpwnwkk.sHtML

[R79] 解析命令行选项
来源：http://mobile.yfazqb.com/Article/details/gvchccvcc.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.blog.vehdjk.com/Article/details/ghiqbnvoa.sHtML

[R80] 查看脚本执行耗时
来源：http://www.m.share.tarul.cn/Article/details/gleoqxnln.sHtML

time ./run.sh
来源：http://mobile.sjlbkw.cn/Article/details/gbaafoofl.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/gjeuppugc.sHtML

S. C / C++ 专题
来源：http://www.blog.sjlbkw.cn/Article/details/ggmrbfemz.sHtML

================================================================================
来源：http://wap.sjlbkw.cn/Article/details/gigupqhmn.sHtML

[S01] C：Hello World
来源：http://3g.epnwcf.com/Article/details/guuhozakm.sHtML

#include <stdio.h>
来源：http://baike.yfazqb.com/Article/details/gcwcfutsr.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.share.epnwcf.com/Article/details/grgqmdoqt.sHtML

[S02] C：变量与格式化输出
来源：http://baike.vehdjk.com/Article/details/gqjcysfyq.sHtML

int a = 10; printf("%d\n", a);
来源：http://wap.vehdjk.com/Article/details/gggnuvkjn.sHtML

[S03] C：读入整数
来源：http://www.share.fktsv.cn/Article/details/gepzsmdlm.sHtML

int x; scanf("%d", &x);
来源：http://wap.tarul.cn/Article/details/grrmefern.sHtML

[S04] C：字符串复制
来源：http://mobile.vehdjk.com/Article/details/gfcmbnznv.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.m.share.vehdjk.com/Article/details/gppxzdrua.sHtML

[S05] C：字符串长度
来源：http://m.share.sjlbkw.cn/Article/details/goeycvdzx.sHtML

strlen(s)
来源：http://www.share.sjlbkw.cn/Article/details/gtegrxkgz.sHtML

[S06] C：字符串比较
来源：http://mobile.fktsv.cn/Article/details/gvapncoib.sHtML

strcmp(a, b) == 0
来源：http://wap.tarul.cn/Article/details/gdcckcpem.sHtML

[S07] C：数组遍历求和
来源：http://m.share.sjlbkw.cn/Article/details/gxgktgjlc.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://read.share.sjlbkw.cn/Article/details/gfdndravc.sHtML

[S08] C：动态内存分配与释放
来源：http://wap.tarul.cn/Article/details/gsmmaiseu.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.blog.sjlbkw.cn/Article/details/gqpbciokl.sHtML

[S09] C：结构体定义与初始化
来源：http://mobile.fktsv.cn/Article/details/gwamaecpb.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mobile.tarul.cn/Article/details/geznklcdq.sHtML

[S10] C：指针与解引用
来源：http://www.share.fktsv.cn/Article/details/ggtymgheb.sHtML

int *p = &a;  *p = 5;
来源：http://wap.sjlbkw.cn/Article/details/ggezhtndt.sHtML

[S11] C：逐行读文件
来源：http://www.blog.tarul.cn/Article/details/gsxrcxpxs.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://blog.yfazqb.com/Article/details/ggtrcnxdl.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.share.yfazqb.com/Article/details/gifliucqr.sHtML

fclose(f);
来源：http://wap.yfazqb.com/Article/details/gdzyjmhlj.sHtML

[S12] C：写文件
来源：http://www.m.share.yfazqb.com/Article/details/gbjvamtov.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://m.share.vehdjk.com/Article/details/gizsypuqd.sHtML

[S13] C：宏定义
来源：http://3g.yfazqb.com/Article/details/gnwaljlfi.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.share.fktsv.cn/Article/details/gybvmygyk.sHtML

[S14] C：枚举
来源：http://www.share.epnwcf.com/Article/details/gnxxpbsdw.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://wap.sjlbkw.cn/Article/details/gsnoagyhf.sHtML

[S15] C：类型转换
来源：http://read.share.sjlbkw.cn/Article/details/gakpzicgm.sHtML

(double) a / b
来源：http://read.share.sjlbkw.cn/Article/details/gfbdxadfo.sHtML

[S16] C：位操作置位
来源：http://www.m.share.tarul.cn/Article/details/gvesvmbci.sHtML

x |= (1 << 3);
来源：http://blog.fktsv.cn/Article/details/gkekzgyau.sHtML

[S17] C：安全拼接字符串
来源：http://mobile.fktsv.cn/Article/details/gnhlmpzes.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://baike.epnwcf.com/Article/details/gietxdcty.sHtML

[S18] C：命令行参数
来源：http://m.share.epnwcf.com/Article/details/gnykpzmyl.sHtML

int main(int argc, char **argv)
来源：http://www.m.share.sjlbkw.cn/Article/details/gcsfgrylk.sHtML

[S19] C：快速排序
来源：http://www.m.share.yfazqb.com/Article/details/giyxpkbqb.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://mobile.fktsv.cn/Article/details/gxsqohdzf.sHtML

[S20] C：二分查找
来源：http://3g.epnwcf.com/Article/details/gfmhuqfaa.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://baike.vehdjk.com/Article/details/gkhabficg.sHtML

[S21] C：字符类别判断
来源：http://read.share.fktsv.cn/Article/details/gpxpvivrg.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://read.share.epnwcf.com/Article/details/gananxqyb.sHtML

[S22] C：字符串转数字
来源：http://wap.epnwcf.com/Article/details/gonlugxjt.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://mobile.sjlbkw.cn/Article/details/ghqgigdzf.sHtML

[S23] C：随机数
来源：http://baike.fktsv.cn/Article/details/ggbiqnlxy.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.blog.fktsv.cn/Article/details/gnfouftwc.sHtML

[S24] C：获取本地时间
来源：http://www.blog.sjlbkw.cn/Article/details/gzpyyuuvi.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://3g.bbcook.cn/Article/details/ggkhcdjxk.sHtML

[S25] C：内存拷贝
来源：http://www.blog.fktsv.cn/Article/details/gmafjxcon.sHtML

memcpy(dst, src, n);
来源：http://read.share.sjlbkw.cn/Article/details/gmwaggwdi.sHtML

[S26] C：内存清零
来源：http://www.m.share.epnwcf.com/Article/details/gfpthnfgu.sHtML

memset(a, 0, sizeof a);
来源：http://www.blog.yfazqb.com/Article/details/gkqecpepv.sHtML

[S27] C：定义常量
来源：http://www.m.share.tarul.cn/Article/details/gxzgeljxd.sHtML

const double PI = 3.14159;
来源：http://3g.yfazqb.com/Article/details/gomnbijpj.sHtML

[S28] C：静态变量
来源：http://baike.fktsv.cn/Article/details/gnwecoeqp.sHtML

static int counter = 0;
来源：http://www.share.tarul.cn/Article/details/gynccuqph.sHtML

[S29] C：变参函数
来源：http://read.share.vehdjk.com/Article/details/gmlljtbqe.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://read.share.sjlbkw.cn/Article/details/gntqzydsj.sHtML

[S30] C：头文件保护
来源：http://baike.yfazqb.com/Article/details/gsayzxxdu.sHtML

#ifndef X_H
来源：http://www.blog.fktsv.cn/Article/details/geurmnugf.sHtML

#define X_H
来源：http://blog.yfazqb.com/Article/details/gctyuosmg.sHtML

#endif
来源：http://wap.tarul.cn/Article/details/ghtviesng.sHtML

[S31] C++：Hello World
来源：http://www.m.share.fktsv.cn/Article/details/gmwlrmouy.sHtML

#include <iostream>
来源：http://mobile.tarul.cn/Article/details/gjescnkry.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://wap.sjlbkw.cn/Article/details/guxfyxtix.sHtML

[S32] C++：字符串
来源：http://read.share.bbcook.cn/Article/details/gurtliolh.sHtML

std::string s = "hi";  s += "!";
来源：http://read.share.tarul.cn/Article/details/ggcrqqksu.sHtML

[S33] C++：vector 增删
来源：http://www.m.share.yfazqb.com/Article/details/ggblboqeu.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://3g.yfazqb.com/Article/details/gahtntdlm.sHtML

[S34] C++：遍历 vector
来源：http://wap.yfazqb.com/Article/details/gfwvnkzgn.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://blog.bbcook.cn/Article/details/gtqnegvsx.sHtML

[S35] C++：map
来源：http://read.share.bbcook.cn/Article/details/gqgpmmpou.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.yfazqb.com/Article/details/gjtospgnq.sHtML

[S36] C++：unordered_map
来源：http://3g.fktsv.cn/Article/details/gcgkozsya.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wap.bbcook.cn/Article/details/gkgtiweyr.sHtML

[S37] C++：set
来源：http://www.blog.fktsv.cn/Article/details/gvkvbqoyk.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://m.share.sjlbkw.cn/Article/details/gqyfuymbs.sHtML

[S38] C++：排序
来源：http://mobile.vehdjk.com/Article/details/gakkjwomz.sHtML

std::sort(v.begin(), v.end());
来源：http://mobile.tarul.cn/Article/details/gydcudsui.sHtML

[S39] C++：自定义比较器排序
来源：http://www.m.share.fktsv.cn/Article/details/gvdtewfsa.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.share.vehdjk.com/Article/details/guarqhjiz.sHtML

[S40] C++：查找元素
来源：http://www.m.share.vehdjk.com/Article/details/gfztbqxod.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://blog.yfazqb.com/Article/details/gwuyqvuws.sHtML

[S41] C++：类与构造函数
来源：http://www.blog.tarul.cn/Article/details/gpptxqumi.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://read.share.epnwcf.com/Article/details/gxeciossh.sHtML

[S42] C++：继承与虚函数
来源：http://3g.yfazqb.com/Article/details/grixhzreg.sHtML

class B : public Base { public: void f() override {} };
来源：http://3g.bbcook.cn/Article/details/gqrnkmjkv.sHtML

[S43] C++：智能指针
来源：http://3g.bbcook.cn/Article/details/ghixvxsbe.sHtML

auto p = std::make_unique<int>(5);
来源：http://read.share.vehdjk.com/Article/details/glvlegpfc.sHtML

[S44] C++：引用传参
来源：http://read.share.yfazqb.com/Article/details/gwhxfsgcj.sHtML

void inc(int &x) { ++x; }
来源：http://3g.sjlbkw.cn/Article/details/gvgifltpj.sHtML

[S45] C++：lambda
来源：http://mobile.yfazqb.com/Article/details/gkicccksn.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://m.share.tarul.cn/Article/details/gkwzbovce.sHtML

[S46] C++：函数模板
来源：http://www.m.share.epnwcf.com/Article/details/gbbbkcazf.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://read.share.yfazqb.com/Article/details/gwgyaypwr.sHtML

[S47] C++：结构化绑定遍历
来源：http://3g.bbcook.cn/Article/details/gfrjwpyml.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://read.share.yfazqb.com/Article/details/ghpkqyeel.sHtML

[S48] C++：逐行读文件
来源：http://blog.yfazqb.com/Article/details/gonseolom.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://baike.bbcook.cn/Article/details/gmnrizjsb.sHtML

while (std::getline(in, line)) { }
来源：http://blog.epnwcf.com/Article/details/gbujtivyj.sHtML

[S49] C++：写文件
来源：http://3g.sjlbkw.cn/Article/details/gjpfcniic.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.share.sjlbkw.cn/Article/details/gtozukfid.sHtML

[S50] C++：格式化数字
来源：http://read.share.epnwcf.com/Article/details/gdlnocpzl.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://wap.sjlbkw.cn/Article/details/gowwtpxgq.sHtML

[S51] C++：显式类型转换
来源：http://baike.yfazqb.com/Article/details/gflaswwzf.sHtML

static_cast<double>(a) / b
来源：http://blog.bbcook.cn/Article/details/gmkectvyp.sHtML

[S52] C++：const 与 noexcept
来源：http://m.share.epnwcf.com/Article/details/gwbawwfyq.sHtML

int size() const noexcept { return n_; }
来源：http://www.blog.bbcook.cn/Article/details/gzdacsxnc.sHtML

[S53] C++：移动语义
来源：http://baike.tarul.cn/Article/details/gjwwupdts.sHtML

std::vector<int> w = std::move(v);
来源：http://blog.fktsv.cn/Article/details/gozkslean.sHtML

[S54] C++：异常处理
来源：http://read.share.sjlbkw.cn/Article/details/ghopnsnvr.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.blog.yfazqb.com/Article/details/gzpqkfsqj.sHtML

[S55] C++：结构化绑定
来源：http://m.share.bbcook.cn/Article/details/gjacpvwkj.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://mobile.sjlbkw.cn/Article/details/gqxnaatud.sHtML

[S56] C++：optional
来源：http://wap.bbcook.cn/Article/details/gtznnxzht.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.m.share.epnwcf.com/Article/details/gcksqrvnb.sHtML

[S57] C++：编译期常量
来源：http://www.m.share.tarul.cn/Article/details/gbdvwlydx.sHtML

constexpr int N = 10;
来源：http://m.share.vehdjk.com/Article/details/grehxhpie.sHtML

[S58] C++：命名空间
来源：http://read.share.sjlbkw.cn/Article/details/gqrstymdd.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.share.sjlbkw.cn/Article/details/gsmorrtcs.sHtML

[S59] C++：静态断言
来源：http://wap.tarul.cn/Article/details/ghfhwgbsb.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://blog.epnwcf.com/Article/details/gmcdvmnin.sHtML

[S60] C++：遍历并删除元素
来源：http://www.share.fktsv.cn/Article/details/ggirzbmjj.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.m.share.sjlbkw.cn/Article/details/gdrymphle.sHtML

================================================================================
来源：http://mobile.tarul.cn/Article/details/gmtybudrm.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.yfazqb.com/Article/details/gnhnucqgk.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/gimsunacg.sHtML

[T01] Kotlin：Hello World
来源：http://blog.bbcook.cn/Article/details/gotzbpsjr.sHtML

println("Hello")
来源：http://www.share.fktsv.cn/Article/details/gosqulfhk.sHtML

[T02] Kotlin：变量
来源：http://wap.tarul.cn/Article/details/guzjcgdof.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.share.vehdjk.com/Article/details/ggssyhvmi.sHtML

[T03] Kotlin：字符串模板
来源：http://www.m.share.yfazqb.com/Article/details/glcnuvbcc.sHtML

"值: $b"
来源：http://read.share.epnwcf.com/Article/details/ghnymjrrf.sHtML

[T04] Kotlin：空安全
来源：http://www.m.share.vehdjk.com/Article/details/gkxepqrrk.sHtML

val n: String? = null;  n?.length
来源：http://blog.sjlbkw.cn/Article/details/griflsgmd.sHtML

[T05] Kotlin：when 表达式
来源：http://www.m.share.epnwcf.com/Article/details/gqclapvsn.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://blog.bbcook.cn/Article/details/gdkavzrxq.sHtML

[T06] Kotlin：集合映射
来源：http://m.share.yfazqb.com/Article/details/gglhdzded.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://blog.vehdjk.com/Article/details/gaoulwupv.sHtML


<!-- 参考信息 -->