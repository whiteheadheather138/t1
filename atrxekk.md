代发 wailian999

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://wap.bbcook.cn/Article/details/ggggmmdso.sHtML

[R16] until 等待条件
来源：http://read.share.epnwcf.com/Article/details/gtpwavvxv.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.share.vehdjk.com/Article/details/guvwxosuz.sHtML

[R17] 数组定义与取值
来源：http://blog.epnwcf.com/Article/details/gzlqzvxoa.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://wap.tarul.cn/Article/details/gimhgxptc.sHtML

[R18] 遍历数组
来源：http://m.share.tarul.cn/Article/details/gdcqiwnic.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://blog.tarul.cn/Article/details/glwjxbdzv.sHtML

[R19] 数组长度
来源：http://3g.epnwcf.com/Article/details/gfdgpbtym.sHtML

echo "${#arr[@]}"
来源：http://3g.yfazqb.com/Article/details/gfhslrblw.sHtML

[R20] 关联数组（字典）
来源：http://www.share.bbcook.cn/Article/details/ghlrruvdh.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://blog.vehdjk.com/Article/details/gkiqhrksx.sHtML

[R21] 字符串长度
来源：http://www.share.epnwcf.com/Article/details/gwbdnmefr.sHtML

echo "${#s}"
来源：http://wap.sjlbkw.cn/Article/details/gidhwbpkd.sHtML

[R22] 截取子串
来源：http://baike.fktsv.cn/Article/details/gagpmozaz.sHtML

echo "${s:0:5}"
来源：http://m.share.yfazqb.com/Article/details/gcingycuw.sHtML

[R23] 字符串替换
来源：http://3g.bbcook.cn/Article/details/gwwafezhg.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://baike.tarul.cn/Article/details/geyhhynzb.sHtML

[R24] 大小写转换
来源：http://blog.fktsv.cn/Article/details/gxuhfownd.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://3g.fktsv.cn/Article/details/ggonqblfe.sHtML

[R25] 去后缀 / 去前缀
来源：http://mobile.vehdjk.com/Article/details/gnmivwcmf.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://wap.tarul.cn/Article/details/gjgarksyg.sHtML

[R26] 命令替换
来源：http://www.blog.fktsv.cn/Article/details/gbgkiuptv.sHtML

now=$(date +%F); echo "$now"
来源：http://wap.fktsv.cn/Article/details/glxgqkomr.sHtML

[R27] 算术展开
来源：http://read.share.bbcook.cn/Article/details/grjyaxeyz.sHtML

echo $((1 + 2 * 3))
来源：http://blog.epnwcf.com/Article/details/gfgyrrjmg.sHtML

[R28] 浮点运算
来源：http://baike.epnwcf.com/Article/details/gcyopbyua.sHtML

echo "scale=2; 10/3" | bc
来源：http://mobile.bbcook.cn/Article/details/gphkrfczr.sHtML

[R29] 定义函数
来源：http://baike.epnwcf.com/Article/details/gzzklypdi.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://baike.sjlbkw.cn/Article/details/gcvdotfhx.sHtML

[R30] 函数返回状态码
来源：http://m.share.tarul.cn/Article/details/ghketlhqq.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.m.share.yfazqb.com/Article/details/gsxgsczoz.sHtML

[R31] 局部变量
来源：http://read.share.yfazqb.com/Article/details/gnamqfwrx.sHtML

f() { local x=1; echo "$x"; }
来源：http://m.share.vehdjk.com/Article/details/gilubdsqt.sHtML

[R32] 参数个数校验
来源：http://www.blog.epnwcf.com/Article/details/gqwqoqerh.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.m.share.yfazqb.com/Article/details/gfvknzjka.sHtML

[R33] 捕获错误并提示行号
来源：http://read.share.sjlbkw.cn/Article/details/glgumlxkz.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://read.share.bbcook.cn/Article/details/gtsvjesmh.sHtML

[R34] 退出时清理
来源：http://www.m.share.fktsv.cn/Article/details/grxacylkj.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://blog.yfazqb.com/Article/details/gvqhrgnxl.sHtML

[R35] 后台执行并等待
来源：http://m.share.tarul.cn/Article/details/gleuxbvob.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://baike.fktsv.cn/Article/details/gilkxjiei.sHtML

[R36] 并发执行多个任务
来源：http://3g.yfazqb.com/Article/details/goeocffpx.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://blog.sjlbkw.cn/Article/details/glqsxymdq.sHtML

[R37] 把输出赋给变量
来源：http://www.share.fktsv.cn/Article/details/gwimbydwg.sHtML

files=$(ls -1)
来源：http://www.blog.vehdjk.com/Article/details/gpabyvnmx.sHtML

[R38] 管道串联
来源：http://www.blog.tarul.cn/Article/details/gdqxuefgr.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.m.share.tarul.cn/Article/details/gsifzkbth.sHtML

[R39] 重定向标准输出与错误
来源：http://read.share.tarul.cn/Article/details/gcaynjjxl.sHtML

cmd > out.log 2>&1
来源：http://wap.sjlbkw.cn/Article/details/gxurpdqjd.sHtML

[R40] 追加写日志
来源：http://www.m.share.bbcook.cn/Article/details/gwzslcfkc.sHtML

echo "log" >> out.log
来源：http://wap.tarul.cn/Article/details/gvhgxzsjd.sHtML

[R41] 丢弃输出
来源：http://mobile.sjlbkw.cn/Article/details/gxupnsruk.sHtML

cmd >/dev/null 2>&1
来源：http://www.blog.epnwcf.com/Article/details/gbgivvfds.sHtML

[R42] 输入重定向
来源：http://www.m.share.sjlbkw.cn/Article/details/gkkkjmxsn.sHtML

wc -l < a.txt
来源：http://3g.tarul.cn/Article/details/gzzukcpym.sHtML

[R43] 按名字查找文件
来源：http://read.share.fktsv.cn/Article/details/gapbjpqpr.sHtML

find . -name "*.log" -type f
来源：http://mobile.bbcook.cn/Article/details/gcvkstouc.sHtML

[R44] 按修改时间查找
来源：http://3g.sjlbkw.cn/Article/details/gifxvwmkf.sHtML

find . -mtime -7 -type f
来源：http://m.share.fktsv.cn/Article/details/gwshveuup.sHtML

[R45] 批量删除
来源：http://mobile.bbcook.cn/Article/details/gqvqjarqj.sHtML

find . -name "*.tmp" -delete
来源：http://blog.yfazqb.com/Article/details/gnkzphoau.sHtML

[R46] 递归替换文件内容
来源：http://wap.vehdjk.com/Article/details/ghigxhoem.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.share.yfazqb.com/Article/details/gqaouwqkl.sHtML

[R47] sed 单行替换
来源：http://wap.bbcook.cn/Article/details/gvgakupwf.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://wap.vehdjk.com/Article/details/gqxqlfrtj.sHtML

[R48] awk 取指定列
来源：http://m.share.epnwcf.com/Article/details/goghgtcbs.sHtML

awk '{print $1, $3}' a.txt
来源：http://wap.bbcook.cn/Article/details/gluzqdyzm.sHtML

[R49] awk 带条件
来源：http://blog.fktsv.cn/Article/details/gxbizvgen.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://blog.epnwcf.com/Article/details/gkleocyuy.sHtML

[R50] awk 求和
来源：http://blog.tarul.cn/Article/details/gxleziths.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.share.vehdjk.com/Article/details/gajvsejyi.sHtML

[R51] 排序去重取前几
来源：http://read.share.epnwcf.com/Article/details/ghbxyajue.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://blog.epnwcf.com/Article/details/gwshtqpcb.sHtML

[R52] 统计行数
来源：http://www.m.share.vehdjk.com/Article/details/gzneipigx.sHtML

wc -l a.txt
来源：http://m.share.bbcook.cn/Article/details/gffleoblf.sHtML

[R53] 查看文件头与实时尾
来源：http://3g.sjlbkw.cn/Article/details/gvticvzui.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://3g.yfazqb.com/Article/details/gbvzcmjuq.sHtML

[R54] 比较两个文件
来源：http://m.share.yfazqb.com/Article/details/gffyludsg.sHtML

diff a.txt b.txt
来源：http://mobile.tarul.cn/Article/details/gpspoxkil.sHtML

[R55] 压缩与解压
来源：http://www.m.share.yfazqb.com/Article/details/grmyeeeum.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://blog.yfazqb.com/Article/details/gcfmyifhe.sHtML

[R56] 远程拷贝
来源：http://blog.sjlbkw.cn/Article/details/gmsaormfv.sHtML

scp file user@host:/path/
来源：http://read.share.tarul.cn/Article/details/gwswvisir.sHtML

[R57] 远程执行命令
来源：http://www.share.tarul.cn/Article/details/gdxnfktez.sHtML

ssh user@host 'uptime'
来源：http://blog.yfazqb.com/Article/details/gffiepmsr.sHtML

[R58] 下载文件
来源：http://m.share.epnwcf.com/Article/details/gisaqtqwg.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://baike.yfazqb.com/Article/details/ggsxmzqfh.sHtML

[R59] 发 POST JSON
来源：http://www.blog.fktsv.cn/Article/details/ghogkhucu.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://read.share.yfazqb.com/Article/details/govnxyvxf.sHtML

[R60] 只看 HTTP 状态码
来源：http://blog.yfazqb.com/Article/details/gztwoomhq.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.share.fktsv.cn/Article/details/ggybsebvg.sHtML

[R61] 磁盘占用
来源：http://mobile.tarul.cn/Article/details/gdpudhuqd.sHtML

df -h;  du -sh *
来源：http://blog.yfazqb.com/Article/details/gvzofnway.sHtML

[R62] 找最占空间的文件
来源：http://mobile.fktsv.cn/Article/details/ghmqxqzoc.sHtML

du -ah . | sort -rh | head -10
来源：http://wap.vehdjk.com/Article/details/gmyuzgpzt.sHtML

[R63] 内存与进程
来源：http://3g.bbcook.cn/Article/details/gxnnvkjgn.sHtML

free -h;  ps aux | grep nginx
来源：http://www.m.share.vehdjk.com/Article/details/gnrliqacf.sHtML

[R64] 结束进程
来源：http://m.share.fktsv.cn/Article/details/genkuelnm.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.m.share.tarul.cn/Article/details/gbdagzefm.sHtML

[R65] 查看端口占用
来源：http://wap.epnwcf.com/Article/details/gwksbisxm.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://3g.fktsv.cn/Article/details/gulamleag.sHtML

[R66] 定时任务
来源：http://3g.epnwcf.com/Article/details/gdcdlytad.sHtML

crontab -e;  crontab -l
来源：http://baike.vehdjk.com/Article/details/gltqjywwp.sHtML

[R67] 生成随机十六进制串
来源：http://www.share.yfazqb.com/Article/details/gvfneergu.sHtML

openssl rand -hex 16
来源：http://www.share.bbcook.cn/Article/details/gqvjamkhq.sHtML

[R68] 计算文件校验值
来源：http://www.blog.epnwcf.com/Article/details/gmhmxkxxw.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.share.yfazqb.com/Article/details/gfikvqzot.sHtML

[R69] 生成随机密码
来源：http://m.share.fktsv.cn/Article/details/ggtpdcgss.sHtML

head -c 16 /dev/urandom | base64
来源：http://mobile.fktsv.cn/Article/details/gsacwttiy.sHtML

[R70] 时间戳与互转
来源：http://wap.vehdjk.com/Article/details/gyhhfqgih.sHtML

date +%s;  date -d @1700000000
来源：http://blog.yfazqb.com/Article/details/gnkmyloxr.sHtML

[R71] 日期格式化
来源：http://m.share.fktsv.cn/Article/details/gkeikbszw.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://read.share.vehdjk.com/Article/details/gxtfsbaot.sHtML

[R72] 等待端口就绪
来源：http://www.m.share.vehdjk.com/Article/details/gwyvlsynv.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://3g.vehdjk.com/Article/details/gzgpmhggb.sHtML

[R73] 分割大日志
来源：http://wap.bbcook.cn/Article/details/gbprenlpx.sHtML

split -l 1000 big.log part_
来源：http://www.m.share.yfazqb.com/Article/details/gvgfqlmvi.sHtML

[R74] 批量重命名
来源：http://wap.epnwcf.com/Article/details/geznjceqg.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.m.share.yfazqb.com/Article/details/gzcqupwry.sHtML

[R75] 导出环境变量
来源：http://3g.sjlbkw.cn/Article/details/gkebeoldg.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.share.yfazqb.com/Article/details/gvakzzfqc.sHtML

[R76] 使用临时文件
来源：http://www.share.bbcook.cn/Article/details/gabbioivh.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.share.yfazqb.com/Article/details/ggzfeoywn.sHtML

[R77] 读取用户输入
来源：http://www.m.share.tarul.cn/Article/details/gptlnzftb.sHtML

read -rp "请输入: " ans
来源：http://wap.vehdjk.com/Article/details/ggtliknfa.sHtML

[R78] 交互式菜单
来源：http://mobile.tarul.cn/Article/details/gfebfxuqu.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://baike.yfazqb.com/Article/details/ggpbfnafs.sHtML

[R79] 解析命令行选项
来源：http://mobile.yfazqb.com/Article/details/gehrgdkcm.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.m.share.sjlbkw.cn/Article/details/gitywtjwo.sHtML

[R80] 查看脚本执行耗时
来源：http://baike.fktsv.cn/Article/details/gkuziobxg.sHtML

time ./run.sh
来源：http://www.blog.sjlbkw.cn/Article/details/gtcvknmjn.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/gfqfjrptn.sHtML

S. C / C++ 专题
来源：http://read.share.bbcook.cn/Article/details/goydiiqad.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/grtbvxtpl.sHtML

[S01] C：Hello World
来源：http://www.share.vehdjk.com/Article/details/gkwbhxgxg.sHtML

#include <stdio.h>
来源：http://3g.yfazqb.com/Article/details/geyjpoqak.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://mobile.vehdjk.com/Article/details/gppzriqbq.sHtML

[S02] C：变量与格式化输出
来源：http://read.share.tarul.cn/Article/details/grcmndtee.sHtML

int a = 10; printf("%d\n", a);
来源：http://mobile.sjlbkw.cn/Article/details/gyisicqqm.sHtML

[S03] C：读入整数
来源：http://mobile.yfazqb.com/Article/details/gpnmbnroq.sHtML

int x; scanf("%d", &x);
来源：http://www.blog.tarul.cn/Article/details/gtswsjupo.sHtML

[S04] C：字符串复制
来源：http://mobile.bbcook.cn/Article/details/gzxkimqui.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://wap.epnwcf.com/Article/details/gaswpnhtv.sHtML

[S05] C：字符串长度
来源：http://read.share.bbcook.cn/Article/details/guvmexify.sHtML

strlen(s)
来源：http://www.blog.fktsv.cn/Article/details/gvdcrvfid.sHtML

[S06] C：字符串比较
来源：http://www.m.share.sjlbkw.cn/Article/details/gzpecfktu.sHtML

strcmp(a, b) == 0
来源：http://www.share.tarul.cn/Article/details/glrqzacuu.sHtML

[S07] C：数组遍历求和
来源：http://wap.tarul.cn/Article/details/gacbbphmr.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://read.share.sjlbkw.cn/Article/details/gkjzkjmbv.sHtML

[S08] C：动态内存分配与释放
来源：http://read.share.bbcook.cn/Article/details/gcrletalx.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://blog.vehdjk.com/Article/details/goyabbrnu.sHtML

[S09] C：结构体定义与初始化
来源：http://www.m.share.yfazqb.com/Article/details/guugdzjjq.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://read.share.vehdjk.com/Article/details/gpalpegll.sHtML

[S10] C：指针与解引用
来源：http://www.share.bbcook.cn/Article/details/gcnunsngq.sHtML

int *p = &a;  *p = 5;
来源：http://wap.epnwcf.com/Article/details/gtoiftslf.sHtML

[S11] C：逐行读文件
来源：http://read.share.vehdjk.com/Article/details/gcgnyvzsf.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://3g.vehdjk.com/Article/details/gbtuhdevk.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.m.share.bbcook.cn/Article/details/gqqzcahby.sHtML

fclose(f);
来源：http://www.m.share.tarul.cn/Article/details/gurxupocb.sHtML

[S12] C：写文件
来源：http://www.share.fktsv.cn/Article/details/gmzxzvsue.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://wap.tarul.cn/Article/details/galgaxljr.sHtML

[S13] C：宏定义
来源：http://www.share.epnwcf.com/Article/details/gngiuadgk.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://3g.tarul.cn/Article/details/gsujdxonf.sHtML

[S14] C：枚举
来源：http://www.blog.sjlbkw.cn/Article/details/gzkhbdbyx.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.blog.yfazqb.com/Article/details/gsfgdxzyv.sHtML

[S15] C：类型转换
来源：http://mobile.sjlbkw.cn/Article/details/gqzppkhta.sHtML

(double) a / b
来源：http://www.m.share.vehdjk.com/Article/details/gtoxxadmu.sHtML

[S16] C：位操作置位
来源：http://blog.fktsv.cn/Article/details/gyirlveao.sHtML

x |= (1 << 3);
来源：http://blog.epnwcf.com/Article/details/gerznkqay.sHtML

[S17] C：安全拼接字符串
来源：http://mobile.tarul.cn/Article/details/gqqswtxdm.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.m.share.fktsv.cn/Article/details/gbfnipezj.sHtML

[S18] C：命令行参数
来源：http://www.share.tarul.cn/Article/details/gfxetigfp.sHtML

int main(int argc, char **argv)
来源：http://read.share.bbcook.cn/Article/details/gvqdfnkgl.sHtML

[S19] C：快速排序
来源：http://blog.epnwcf.com/Article/details/gxsjjmrak.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://read.share.epnwcf.com/Article/details/gdptfgtff.sHtML

[S20] C：二分查找
来源：http://wap.tarul.cn/Article/details/gnlwixepz.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://read.share.fktsv.cn/Article/details/geulocttn.sHtML

[S21] C：字符类别判断
来源：http://www.m.share.tarul.cn/Article/details/gyqxykzqb.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://baike.bbcook.cn/Article/details/gzqeykawg.sHtML

[S22] C：字符串转数字
来源：http://3g.epnwcf.com/Article/details/gwsdksvgx.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://3g.bbcook.cn/Article/details/gxiyovdjq.sHtML

[S23] C：随机数
来源：http://m.share.bbcook.cn/Article/details/gdvzaajmj.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.share.epnwcf.com/Article/details/gruvlfwqj.sHtML

[S24] C：获取本地时间
来源：http://www.m.share.sjlbkw.cn/Article/details/gidzrnshk.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://read.share.vehdjk.com/Article/details/gweftrlnx.sHtML

[S25] C：内存拷贝
来源：http://www.share.sjlbkw.cn/Article/details/gjsuacywk.sHtML

memcpy(dst, src, n);
来源：http://www.blog.fktsv.cn/Article/details/gzkizphwm.sHtML

[S26] C：内存清零
来源：http://wap.epnwcf.com/Article/details/gfrgagcre.sHtML

memset(a, 0, sizeof a);
来源：http://baike.yfazqb.com/Article/details/gyuyniljk.sHtML

[S27] C：定义常量
来源：http://wap.sjlbkw.cn/Article/details/gnzqfycnx.sHtML

const double PI = 3.14159;
来源：http://blog.bbcook.cn/Article/details/gymvnsshn.sHtML

[S28] C：静态变量
来源：http://blog.sjlbkw.cn/Article/details/gfytphwuw.sHtML

static int counter = 0;
来源：http://www.m.share.sjlbkw.cn/Article/details/ggmkykxlp.sHtML

[S29] C：变参函数
来源：http://3g.fktsv.cn/Article/details/gdhtwnhrx.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mobile.fktsv.cn/Article/details/geonvaxwv.sHtML

[S30] C：头文件保护
来源：http://blog.fktsv.cn/Article/details/gncnybpoe.sHtML

#ifndef X_H
来源：http://blog.bbcook.cn/Article/details/grdxiueds.sHtML

#define X_H
来源：http://mobile.yfazqb.com/Article/details/gadfuvmjp.sHtML

#endif
来源：http://wap.bbcook.cn/Article/details/gjkhbbexh.sHtML

[S31] C++：Hello World
来源：http://www.share.epnwcf.com/Article/details/gxakvcrmz.sHtML

#include <iostream>
来源：http://www.blog.vehdjk.com/Article/details/granbyyle.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://blog.sjlbkw.cn/Article/details/gzzxblcyp.sHtML

[S32] C++：字符串
来源：http://www.share.sjlbkw.cn/Article/details/gynsfztwt.sHtML

std::string s = "hi";  s += "!";
来源：http://3g.vehdjk.com/Article/details/gcgzprora.sHtML

[S33] C++：vector 增删
来源：http://blog.bbcook.cn/Article/details/gekxczdmz.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.blog.tarul.cn/Article/details/gpblblwwi.sHtML

[S34] C++：遍历 vector
来源：http://blog.tarul.cn/Article/details/gftyfebmm.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://blog.epnwcf.com/Article/details/gzetsanhm.sHtML

[S35] C++：map
来源：http://www.m.share.yfazqb.com/Article/details/ggsrvmqcx.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://3g.epnwcf.com/Article/details/ghdxtxnhx.sHtML

[S36] C++：unordered_map
来源：http://wap.fktsv.cn/Article/details/gdhknbfnt.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://3g.fktsv.cn/Article/details/gqcqdmdcg.sHtML

[S37] C++：set
来源：http://mobile.fktsv.cn/Article/details/gewxakhyi.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://mobile.bbcook.cn/Article/details/gjmnpyytn.sHtML

[S38] C++：排序
来源：http://www.share.vehdjk.com/Article/details/gouekeofn.sHtML

std::sort(v.begin(), v.end());
来源：http://3g.sjlbkw.cn/Article/details/gotmslfsz.sHtML

[S39] C++：自定义比较器排序
来源：http://www.m.share.sjlbkw.cn/Article/details/gohbownzk.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://baike.tarul.cn/Article/details/gvgdeokfa.sHtML

[S40] C++：查找元素
来源：http://read.share.yfazqb.com/Article/details/geunxgyxj.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.m.share.sjlbkw.cn/Article/details/ghbckodqj.sHtML

[S41] C++：类与构造函数
来源：http://baike.yfazqb.com/Article/details/gkvpsxrnl.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://wap.vehdjk.com/Article/details/gucxioumn.sHtML

[S42] C++：继承与虚函数
来源：http://3g.yfazqb.com/Article/details/ghwmhksrg.sHtML

class B : public Base { public: void f() override {} };
来源：http://read.share.bbcook.cn/Article/details/gtvxouujc.sHtML

[S43] C++：智能指针
来源：http://read.share.fktsv.cn/Article/details/gocicrfpf.sHtML

auto p = std::make_unique<int>(5);
来源：http://3g.tarul.cn/Article/details/gzoltkoyd.sHtML

[S44] C++：引用传参
来源：http://baike.sjlbkw.cn/Article/details/gdqptgqho.sHtML

void inc(int &x) { ++x; }
来源：http://www.m.share.bbcook.cn/Article/details/geqnyiiqb.sHtML

[S45] C++：lambda
来源：http://baike.sjlbkw.cn/Article/details/giupdpbld.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://m.share.sjlbkw.cn/Article/details/gvstqgref.sHtML

[S46] C++：函数模板
来源：http://3g.bbcook.cn/Article/details/gxvupeehv.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://read.share.bbcook.cn/Article/details/gutifiulj.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.share.bbcook.cn/Article/details/gcqxspbca.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://read.share.epnwcf.com/Article/details/gyhopfoen.sHtML

[S48] C++：逐行读文件
来源：http://www.share.tarul.cn/Article/details/gbulxsnpp.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://mobile.epnwcf.com/Article/details/gfsojbsxo.sHtML

while (std::getline(in, line)) { }
来源：http://wap.epnwcf.com/Article/details/gkwsbnari.sHtML

[S49] C++：写文件
来源：http://m.share.yfazqb.com/Article/details/gctmdipzr.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://read.share.tarul.cn/Article/details/glfxafosa.sHtML

[S50] C++：格式化数字
来源：http://read.share.yfazqb.com/Article/details/gqaheaxsw.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://mobile.yfazqb.com/Article/details/gctnbqgqv.sHtML

[S51] C++：显式类型转换
来源：http://www.share.fktsv.cn/Article/details/gvgzjnlpb.sHtML

static_cast<double>(a) / b
来源：http://read.share.sjlbkw.cn/Article/details/gmujpdqti.sHtML

[S52] C++：const 与 noexcept
来源：http://www.share.bbcook.cn/Article/details/gztporbrd.sHtML

int size() const noexcept { return n_; }
来源：http://blog.sjlbkw.cn/Article/details/gwwmhwtbc.sHtML

[S53] C++：移动语义
来源：http://3g.vehdjk.com/Article/details/guzyspkjh.sHtML

std::vector<int> w = std::move(v);
来源：http://3g.fktsv.cn/Article/details/gzgtmapss.sHtML

[S54] C++：异常处理
来源：http://www.share.sjlbkw.cn/Article/details/gjofokahf.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.blog.tarul.cn/Article/details/gzyspcaoe.sHtML

[S55] C++：结构化绑定
来源：http://www.blog.vehdjk.com/Article/details/gbmgqnpen.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.share.vehdjk.com/Article/details/ggmfpbwra.sHtML

[S56] C++：optional
来源：http://www.share.yfazqb.com/Article/details/gfsjualzw.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.share.fktsv.cn/Article/details/ggsjqhfon.sHtML

[S57] C++：编译期常量
来源：http://blog.yfazqb.com/Article/details/gzcesrvhz.sHtML

constexpr int N = 10;
来源：http://www.m.share.fktsv.cn/Article/details/gzpkcmkpx.sHtML

[S58] C++：命名空间
来源：http://mobile.yfazqb.com/Article/details/gtcrvrkft.sHtML

namespace ns { int f() { return 1; } }
来源：http://blog.bbcook.cn/Article/details/gictkljaa.sHtML

[S59] C++：静态断言
来源：http://baike.sjlbkw.cn/Article/details/ggpapckii.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.m.share.bbcook.cn/Article/details/gseqdcwif.sHtML

[S60] C++：遍历并删除元素
来源：http://3g.yfazqb.com/Article/details/gcsdrliwo.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://mobile.fktsv.cn/Article/details/gsnkscbxr.sHtML

================================================================================
来源：http://mobile.epnwcf.com/Article/details/gbuaaavfz.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://wap.bbcook.cn/Article/details/gaqerbbak.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/gbcdhierf.sHtML

[T01] Kotlin：Hello World
来源：http://read.share.fktsv.cn/Article/details/gvnuclvtv.sHtML

println("Hello")
来源：http://blog.fktsv.cn/Article/details/ggocsordb.sHtML

[T02] Kotlin：变量
来源：http://www.m.share.tarul.cn/Article/details/gryugwpyb.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.blog.fktsv.cn/Article/details/gmcjtjkvn.sHtML

[T03] Kotlin：字符串模板
来源：http://3g.fktsv.cn/Article/details/gcjfvrovk.sHtML

"值: $b"
来源：http://m.share.fktsv.cn/Article/details/gopvciqeh.sHtML

[T04] Kotlin：空安全
来源：http://www.share.vehdjk.com/Article/details/gokerqfkg.sHtML

val n: String? = null;  n?.length
来源：http://blog.epnwcf.com/Article/details/gglauuhab.sHtML

[T05] Kotlin：when 表达式
来源：http://www.m.share.yfazqb.com/Article/details/gswtcckdp.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://wap.tarul.cn/Article/details/gruviqtad.sHtML

[T06] Kotlin：集合映射
来源：http://mobile.tarul.cn/Article/details/ghtkmlcoa.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://m.share.epnwcf.com/Article/details/gwflsuqtm.sHtML

[T07] Kotlin：集合过滤
来源：http://www.m.share.vehdjk.com/Article/details/gtcpvlwbc.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://3g.vehdjk.com/Article/details/gyecycqkw.sHtML

[T08] Kotlin：数据类
来源：http://wap.fktsv.cn/Article/details/goeyhjiqu.sHtML

data class User(val name: String, val age: Int)
来源：http://3g.tarul.cn/Article/details/gpiavsuia.sHtML

[T09] Kotlin：扩展函数
来源：http://www.share.epnwcf.com/Article/details/gkhxtchby.sHtML

fun String.exclaim() = this + "!"
来源：http://mobile.sjlbkw.cn/Article/details/gxvfpipyh.sHtML

[T10] Kotlin：默认参数
来源：http://www.share.fktsv.cn/Article/details/gfixbjtbj.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://read.share.fktsv.cn/Article/details/gedlxwimi.sHtML

[T11] Kotlin：协程
来源：http://wap.tarul.cn/Article/details/gidvhrpkx.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.blog.fktsv.cn/Article/details/geaoabfkn.sHtML

[T12] Kotlin：解构声明
来源：http://www.blog.sjlbkw.cn/Article/details/gkqkhhahs.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.share.tarul.cn/Article/details/gmtwysbit.sHtML

[T13] Kotlin：只读 Map
来源：http://3g.yfazqb.com/Article/details/ghpbgfbrd.sHtML

val m = mapOf("a" to 1)
来源：http://wap.bbcook.cn/Article/details/gdweeaitt.sHtML

[T14] Kotlin：循环
来源：http://mobile.sjlbkw.cn/Article/details/gkdirxmqh.sHtML

for (i in 1..10) println(i)
来源：http://www.blog.sjlbkw.cn/Article/details/gncztzkfe.sHtML

[T15] Kotlin：接口
来源：http://baike.tarul.cn/Article/details/gpfhuakkm.sHtML

interface Shape { fun area(): Double }
来源：http://m.share.tarul.cn/Article/details/gcnncnach.sHtML

[T16] Swift：Hello World
来源：http://www.m.share.tarul.cn/Article/details/gnnmvtnba.sHtML

print("Hello")
来源：http://m.share.yfazqb.com/Article/details/ggspubzki.sHtML

[T17] Swift：变量与常量
来源：http://blog.tarul.cn/Article/details/gkuqywfsn.sHtML

var a = 1;  let b = 2
来源：http://3g.fktsv.cn/Article/details/gigfjsogb.sHtML

[T18] Swift：字符串插值
来源：http://m.share.tarul.cn/Article/details/grlhvimuk.sHtML

"值: \(b)"
来源：http://3g.fktsv.cn/Article/details/gyqebybmv.sHtML


<!-- 参考信息 -->