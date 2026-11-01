代发 wailian999

echo "${#arr[@]}"
来源：http://3g.epnwcf.com/Article/details/gdroaufly.sHtML

[R20] 关联数组（字典）
来源：http://wap.sjlbkw.cn/Article/details/gjengyyqc.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://baike.sjlbkw.cn/Article/details/gjxkxqikf.sHtML

[R21] 字符串长度
来源：http://mobile.vehdjk.com/Article/details/gclgebyly.sHtML

echo "${#s}"
来源：http://wap.bbcook.cn/Article/details/gxxdomitv.sHtML

[R22] 截取子串
来源：http://3g.bbcook.cn/Article/details/gfhdomwck.sHtML

echo "${s:0:5}"
来源：http://read.share.sjlbkw.cn/Article/details/ggpwjigeb.sHtML

[R23] 字符串替换
来源：http://mobile.sjlbkw.cn/Article/details/gaocqzlqm.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.m.share.yfazqb.com/Article/details/gqbqlcvlu.sHtML

[R24] 大小写转换
来源：http://www.m.share.epnwcf.com/Article/details/ggnrkenjz.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://m.share.epnwcf.com/Article/details/gqqjjvaeh.sHtML

[R25] 去后缀 / 去前缀
来源：http://3g.yfazqb.com/Article/details/gyltyeorz.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.m.share.bbcook.cn/Article/details/gvivpctan.sHtML

[R26] 命令替换
来源：http://read.share.yfazqb.com/Article/details/gagzknvgz.sHtML

now=$(date +%F); echo "$now"
来源：http://www.blog.epnwcf.com/Article/details/gxxhrocmt.sHtML

[R27] 算术展开
来源：http://www.m.share.epnwcf.com/Article/details/gqfckusdk.sHtML

echo $((1 + 2 * 3))
来源：http://m.share.epnwcf.com/Article/details/gdrtxghit.sHtML

[R28] 浮点运算
来源：http://www.blog.bbcook.cn/Article/details/ggxrtiizd.sHtML

echo "scale=2; 10/3" | bc
来源：http://3g.tarul.cn/Article/details/gfvqikwex.sHtML

[R29] 定义函数
来源：http://wap.vehdjk.com/Article/details/gaigavnkh.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.share.tarul.cn/Article/details/gtgwkghcr.sHtML

[R30] 函数返回状态码
来源：http://baike.epnwcf.com/Article/details/gimfjvabh.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.share.fktsv.cn/Article/details/gjxikwojp.sHtML

[R31] 局部变量
来源：http://www.m.share.epnwcf.com/Article/details/gibhbridp.sHtML

f() { local x=1; echo "$x"; }
来源：http://mobile.tarul.cn/Article/details/gbwceceov.sHtML

[R32] 参数个数校验
来源：http://www.share.tarul.cn/Article/details/gzkwuhbhu.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.m.share.vehdjk.com/Article/details/gfuucufml.sHtML

[R33] 捕获错误并提示行号
来源：http://blog.yfazqb.com/Article/details/gtrnoswll.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.m.share.vehdjk.com/Article/details/gakiqiddc.sHtML

[R34] 退出时清理
来源：http://www.share.yfazqb.com/Article/details/gevzrzubd.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://wap.bbcook.cn/Article/details/gnkpcziaf.sHtML

[R35] 后台执行并等待
来源：http://www.blog.sjlbkw.cn/Article/details/gysecxigs.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.share.vehdjk.com/Article/details/gogzulxjr.sHtML

[R36] 并发执行多个任务
来源：http://www.blog.yfazqb.com/Article/details/gansobcum.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.share.fktsv.cn/Article/details/gvkhhwufj.sHtML

[R37] 把输出赋给变量
来源：http://m.share.bbcook.cn/Article/details/gmgqwrpks.sHtML

files=$(ls -1)
来源：http://www.blog.vehdjk.com/Article/details/gmhrgwpry.sHtML

[R38] 管道串联
来源：http://www.blog.yfazqb.com/Article/details/gihhqivaa.sHtML

cat a.txt | grep -i error | wc -l
来源：http://3g.epnwcf.com/Article/details/gwzvcdapn.sHtML

[R39] 重定向标准输出与错误
来源：http://m.share.tarul.cn/Article/details/gsdhzyfqm.sHtML

cmd > out.log 2>&1
来源：http://blog.tarul.cn/Article/details/gxhulxmrj.sHtML

[R40] 追加写日志
来源：http://m.share.tarul.cn/Article/details/gkvamedrw.sHtML

echo "log" >> out.log
来源：http://baike.fktsv.cn/Article/details/gsewcchju.sHtML

[R41] 丢弃输出
来源：http://www.share.fktsv.cn/Article/details/gtgarowdt.sHtML

cmd >/dev/null 2>&1
来源：http://m.share.epnwcf.com/Article/details/grfqaksym.sHtML

[R42] 输入重定向
来源：http://www.blog.tarul.cn/Article/details/gduuilljz.sHtML

wc -l < a.txt
来源：http://www.share.fktsv.cn/Article/details/gzeywtzvx.sHtML

[R43] 按名字查找文件
来源：http://blog.yfazqb.com/Article/details/gkrfaocxa.sHtML

find . -name "*.log" -type f
来源：http://baike.epnwcf.com/Article/details/ggyvruwva.sHtML

[R44] 按修改时间查找
来源：http://3g.sjlbkw.cn/Article/details/ggvxyctaq.sHtML

find . -mtime -7 -type f
来源：http://3g.sjlbkw.cn/Article/details/grxsijznm.sHtML

[R45] 批量删除
来源：http://www.share.sjlbkw.cn/Article/details/gwlbgibcn.sHtML

find . -name "*.tmp" -delete
来源：http://www.m.share.vehdjk.com/Article/details/giqrgncvd.sHtML

[R46] 递归替换文件内容
来源：http://mobile.tarul.cn/Article/details/gvailfpjl.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.blog.fktsv.cn/Article/details/gafqggkgq.sHtML

[R47] sed 单行替换
来源：http://mobile.yfazqb.com/Article/details/gcixohwkj.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://3g.tarul.cn/Article/details/gqldeqkiv.sHtML

[R48] awk 取指定列
来源：http://baike.bbcook.cn/Article/details/grxfmgcnx.sHtML

awk '{print $1, $3}' a.txt
来源：http://baike.fktsv.cn/Article/details/gcapfkgfj.sHtML

[R49] awk 带条件
来源：http://baike.fktsv.cn/Article/details/gigzztgkn.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.m.share.vehdjk.com/Article/details/ggmweryfv.sHtML

[R50] awk 求和
来源：http://read.share.bbcook.cn/Article/details/gpllanzxn.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.blog.bbcook.cn/Article/details/gzeymzbxq.sHtML

[R51] 排序去重取前几
来源：http://blog.bbcook.cn/Article/details/gomzzptnj.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://mobile.yfazqb.com/Article/details/ghexqghxu.sHtML

[R52] 统计行数
来源：http://m.share.bbcook.cn/Article/details/gwxnklpmq.sHtML

wc -l a.txt
来源：http://m.share.bbcook.cn/Article/details/gcoxcazpr.sHtML

[R53] 查看文件头与实时尾
来源：http://baike.fktsv.cn/Article/details/gjwybtoos.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.share.vehdjk.com/Article/details/gxfsaaoxx.sHtML

[R54] 比较两个文件
来源：http://3g.yfazqb.com/Article/details/gsbprigup.sHtML

diff a.txt b.txt
来源：http://baike.yfazqb.com/Article/details/gzmsobczc.sHtML

[R55] 压缩与解压
来源：http://baike.epnwcf.com/Article/details/ghqslbhwo.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://baike.fktsv.cn/Article/details/gvdzmtytu.sHtML

[R56] 远程拷贝
来源：http://m.share.tarul.cn/Article/details/ghwzitgqx.sHtML

scp file user@host:/path/
来源：http://m.share.fktsv.cn/Article/details/ggnrwkfco.sHtML

[R57] 远程执行命令
来源：http://www.blog.sjlbkw.cn/Article/details/gxvmvldkb.sHtML

ssh user@host 'uptime'
来源：http://www.blog.epnwcf.com/Article/details/gtvfmflfw.sHtML

[R58] 下载文件
来源：http://m.share.yfazqb.com/Article/details/grgdqiyaz.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://wap.yfazqb.com/Article/details/gzimkkfbe.sHtML

[R59] 发 POST JSON
来源：http://mobile.sjlbkw.cn/Article/details/guigcwqxt.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.m.share.sjlbkw.cn/Article/details/gqslzybaf.sHtML

[R60] 只看 HTTP 状态码
来源：http://read.share.tarul.cn/Article/details/gbxmvhpqd.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://blog.tarul.cn/Article/details/gdypqrhiy.sHtML

[R61] 磁盘占用
来源：http://blog.yfazqb.com/Article/details/ghxwudwdn.sHtML

df -h;  du -sh *
来源：http://mobile.fktsv.cn/Article/details/gogbcgbce.sHtML

[R62] 找最占空间的文件
来源：http://www.m.share.fktsv.cn/Article/details/gsyerznet.sHtML

du -ah . | sort -rh | head -10
来源：http://baike.epnwcf.com/Article/details/gpxtnslez.sHtML

[R63] 内存与进程
来源：http://read.share.sjlbkw.cn/Article/details/gxphqtxfg.sHtML

free -h;  ps aux | grep nginx
来源：http://wap.yfazqb.com/Article/details/giteyqjia.sHtML

[R64] 结束进程
来源：http://3g.bbcook.cn/Article/details/gwwewypzu.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.share.fktsv.cn/Article/details/gtipieprc.sHtML

[R65] 查看端口占用
来源：http://read.share.yfazqb.com/Article/details/gkwfeskpw.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://3g.tarul.cn/Article/details/gdeiblwnv.sHtML

[R66] 定时任务
来源：http://read.share.sjlbkw.cn/Article/details/glqrrdwyj.sHtML

crontab -e;  crontab -l
来源：http://www.blog.vehdjk.com/Article/details/gmsypjpol.sHtML

[R67] 生成随机十六进制串
来源：http://mobile.vehdjk.com/Article/details/ghjsrsbic.sHtML

openssl rand -hex 16
来源：http://baike.tarul.cn/Article/details/gchmteqqx.sHtML

[R68] 计算文件校验值
来源：http://blog.epnwcf.com/Article/details/gcfbleeac.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://read.share.bbcook.cn/Article/details/gsdixotpe.sHtML

[R69] 生成随机密码
来源：http://m.share.vehdjk.com/Article/details/gkrguenid.sHtML

head -c 16 /dev/urandom | base64
来源：http://baike.yfazqb.com/Article/details/gjtfpwhtf.sHtML

[R70] 时间戳与互转
来源：http://read.share.bbcook.cn/Article/details/ggfgkbtef.sHtML

date +%s;  date -d @1700000000
来源：http://read.share.tarul.cn/Article/details/gghtznxxp.sHtML

[R71] 日期格式化
来源：http://baike.tarul.cn/Article/details/gtbvqlwtn.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.blog.fktsv.cn/Article/details/gymnpjply.sHtML

[R72] 等待端口就绪
来源：http://www.blog.epnwcf.com/Article/details/gqfayjtjd.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.blog.vehdjk.com/Article/details/gqlwjcqnw.sHtML

[R73] 分割大日志
来源：http://mobile.vehdjk.com/Article/details/gbscmnyxb.sHtML

split -l 1000 big.log part_
来源：http://www.share.vehdjk.com/Article/details/ghtcgwezy.sHtML

[R74] 批量重命名
来源：http://www.share.sjlbkw.cn/Article/details/gkphzzhnq.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://wap.bbcook.cn/Article/details/gkxidojmt.sHtML

[R75] 导出环境变量
来源：http://www.share.sjlbkw.cn/Article/details/gomrfouoi.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.share.yfazqb.com/Article/details/gndhozqkx.sHtML

[R76] 使用临时文件
来源：http://www.share.epnwcf.com/Article/details/gmrscdzgg.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.epnwcf.com/Article/details/ghhviwnai.sHtML

[R77] 读取用户输入
来源：http://m.share.tarul.cn/Article/details/gnizomyjk.sHtML

read -rp "请输入: " ans
来源：http://www.blog.vehdjk.com/Article/details/gqtbwjmzc.sHtML

[R78] 交互式菜单
来源：http://www.blog.fktsv.cn/Article/details/glrvseodl.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://m.share.bbcook.cn/Article/details/gytphicjo.sHtML

[R79] 解析命令行选项
来源：http://wap.tarul.cn/Article/details/gxabtpyof.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://read.share.bbcook.cn/Article/details/gwebgwnwl.sHtML

[R80] 查看脚本执行耗时
来源：http://blog.vehdjk.com/Article/details/guriugbkb.sHtML

time ./run.sh
来源：http://blog.fktsv.cn/Article/details/gxyqopdfu.sHtML

================================================================================
来源：http://www.share.sjlbkw.cn/Article/details/gyfwktoif.sHtML

S. C / C++ 专题
来源：http://www.m.share.vehdjk.com/Article/details/gnkcoasoc.sHtML

================================================================================
来源：http://baike.tarul.cn/Article/details/gtocpitxk.sHtML

[S01] C：Hello World
来源：http://wap.fktsv.cn/Article/details/gqnvvlgbd.sHtML

#include <stdio.h>
来源：http://blog.tarul.cn/Article/details/geivgrqhi.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.blog.yfazqb.com/Article/details/gganqxlwy.sHtML

[S02] C：变量与格式化输出
来源：http://www.blog.sjlbkw.cn/Article/details/ghqktlfmr.sHtML

int a = 10; printf("%d\n", a);
来源：http://baike.sjlbkw.cn/Article/details/gvdqilkyy.sHtML

[S03] C：读入整数
来源：http://wap.vehdjk.com/Article/details/grkinnrsy.sHtML

int x; scanf("%d", &x);
来源：http://baike.epnwcf.com/Article/details/gcvajbtfu.sHtML

[S04] C：字符串复制
来源：http://read.share.vehdjk.com/Article/details/grkoxxqtn.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.m.share.fktsv.cn/Article/details/ghihkytzj.sHtML

[S05] C：字符串长度
来源：http://mobile.sjlbkw.cn/Article/details/gmchoxslx.sHtML

strlen(s)
来源：http://www.share.epnwcf.com/Article/details/gcuxhqbuw.sHtML

[S06] C：字符串比较
来源：http://www.share.epnwcf.com/Article/details/gzdnkxqom.sHtML

strcmp(a, b) == 0
来源：http://mobile.fktsv.cn/Article/details/gslqtppgj.sHtML

[S07] C：数组遍历求和
来源：http://wap.sjlbkw.cn/Article/details/ghyrcuzml.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.share.yfazqb.com/Article/details/gdplnuaex.sHtML

[S08] C：动态内存分配与释放
来源：http://wap.epnwcf.com/Article/details/gmzedsoue.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://3g.bbcook.cn/Article/details/gtbqzphyb.sHtML

[S09] C：结构体定义与初始化
来源：http://baike.bbcook.cn/Article/details/gifxbztmc.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mobile.epnwcf.com/Article/details/gfktfizvh.sHtML

[S10] C：指针与解引用
来源：http://wap.bbcook.cn/Article/details/gdrntwlec.sHtML

int *p = &a;  *p = 5;
来源：http://www.m.share.fktsv.cn/Article/details/gynjgpygd.sHtML

[S11] C：逐行读文件
来源：http://www.m.share.yfazqb.com/Article/details/gmquwhkxg.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://read.share.fktsv.cn/Article/details/gebtpzsyz.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://mobile.yfazqb.com/Article/details/ggrggfgab.sHtML

fclose(f);
来源：http://baike.tarul.cn/Article/details/gllfcrydl.sHtML

[S12] C：写文件
来源：http://mobile.tarul.cn/Article/details/ggwytkrwt.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mobile.epnwcf.com/Article/details/giacwbfld.sHtML

[S13] C：宏定义
来源：http://www.share.yfazqb.com/Article/details/gaykybbzy.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.blog.bbcook.cn/Article/details/gjgduqwdd.sHtML

[S14] C：枚举
来源：http://www.blog.yfazqb.com/Article/details/gnkduuutf.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.share.fktsv.cn/Article/details/gikiyitgh.sHtML

[S15] C：类型转换
来源：http://baike.sjlbkw.cn/Article/details/glcarmbjn.sHtML

(double) a / b
来源：http://wap.sjlbkw.cn/Article/details/geqhjepbd.sHtML

[S16] C：位操作置位
来源：http://www.blog.epnwcf.com/Article/details/gwlwxzdwj.sHtML

x |= (1 << 3);
来源：http://3g.fktsv.cn/Article/details/gonvatzme.sHtML

[S17] C：安全拼接字符串
来源：http://baike.sjlbkw.cn/Article/details/gbiecpwdx.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://blog.epnwcf.com/Article/details/gdssvgnci.sHtML

[S18] C：命令行参数
来源：http://www.blog.fktsv.cn/Article/details/gtpdekann.sHtML

int main(int argc, char **argv)
来源：http://m.share.sjlbkw.cn/Article/details/gnntpkamf.sHtML

[S19] C：快速排序
来源：http://baike.epnwcf.com/Article/details/gdlmifjbt.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://3g.tarul.cn/Article/details/geayvldmb.sHtML

[S20] C：二分查找
来源：http://www.blog.vehdjk.com/Article/details/gwccmqqjp.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.m.share.vehdjk.com/Article/details/ggxjnbcuu.sHtML

[S21] C：字符类别判断
来源：http://mobile.yfazqb.com/Article/details/gjormezwp.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.blog.fktsv.cn/Article/details/gjhyzjgzz.sHtML

[S22] C：字符串转数字
来源：http://read.share.bbcook.cn/Article/details/guzkvgozk.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.share.fktsv.cn/Article/details/gcjvjguwd.sHtML

[S23] C：随机数
来源：http://m.share.sjlbkw.cn/Article/details/gchoqjfit.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://wap.vehdjk.com/Article/details/gndevlxaw.sHtML

[S24] C：获取本地时间
来源：http://www.m.share.bbcook.cn/Article/details/gxhsafapp.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.blog.vehdjk.com/Article/details/gzryepihw.sHtML

[S25] C：内存拷贝
来源：http://www.share.epnwcf.com/Article/details/gpmdwysft.sHtML

memcpy(dst, src, n);
来源：http://blog.fktsv.cn/Article/details/gcdhapdif.sHtML

[S26] C：内存清零
来源：http://blog.bbcook.cn/Article/details/gpfuprocp.sHtML

memset(a, 0, sizeof a);
来源：http://www.m.share.vehdjk.com/Article/details/gamgyvvts.sHtML

[S27] C：定义常量
来源：http://www.blog.epnwcf.com/Article/details/gsedretdi.sHtML

const double PI = 3.14159;
来源：http://3g.tarul.cn/Article/details/gsslqsuum.sHtML

[S28] C：静态变量
来源：http://blog.yfazqb.com/Article/details/gbsrwmlfk.sHtML

static int counter = 0;
来源：http://www.share.bbcook.cn/Article/details/gllxtzxjh.sHtML

[S29] C：变参函数
来源：http://blog.vehdjk.com/Article/details/gdijrpeoy.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.share.vehdjk.com/Article/details/grzlaowzt.sHtML

[S30] C：头文件保护
来源：http://baike.vehdjk.com/Article/details/grpfohpsn.sHtML

#ifndef X_H
来源：http://mobile.bbcook.cn/Article/details/gslhgzliw.sHtML

#define X_H
来源：http://3g.bbcook.cn/Article/details/gmojvxqww.sHtML

#endif
来源：http://3g.bbcook.cn/Article/details/glihbmtol.sHtML

[S31] C++：Hello World
来源：http://baike.yfazqb.com/Article/details/gdmkzdvap.sHtML

#include <iostream>
来源：http://baike.sjlbkw.cn/Article/details/gatokowsl.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://m.share.bbcook.cn/Article/details/gjhkmxywr.sHtML

[S32] C++：字符串
来源：http://www.share.fktsv.cn/Article/details/gtcqibnuc.sHtML

std::string s = "hi";  s += "!";
来源：http://mobile.tarul.cn/Article/details/gqbwdphfw.sHtML

[S33] C++：vector 增删
来源：http://baike.tarul.cn/Article/details/gpqzcxahp.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://read.share.yfazqb.com/Article/details/gfbvhauee.sHtML

[S34] C++：遍历 vector
来源：http://wap.bbcook.cn/Article/details/grgvjbjhi.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://mobile.epnwcf.com/Article/details/gdtqqxgaq.sHtML

[S35] C++：map
来源：http://read.share.sjlbkw.cn/Article/details/gigjvqnry.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.tarul.cn/Article/details/gsnjyivip.sHtML

[S36] C++：unordered_map
来源：http://mobile.tarul.cn/Article/details/gyvatsbaa.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.sjlbkw.cn/Article/details/gzcqnmerw.sHtML

[S37] C++：set
来源：http://www.share.sjlbkw.cn/Article/details/gjtxhoviy.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://m.share.tarul.cn/Article/details/gmlbnbcrh.sHtML

[S38] C++：排序
来源：http://www.blog.fktsv.cn/Article/details/ggunohjxg.sHtML

std::sort(v.begin(), v.end());
来源：http://baike.vehdjk.com/Article/details/gkevbmqbb.sHtML

[S39] C++：自定义比较器排序
来源：http://www.share.tarul.cn/Article/details/glzygapmj.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://blog.sjlbkw.cn/Article/details/gpmouckiy.sHtML

[S40] C++：查找元素
来源：http://baike.tarul.cn/Article/details/gdcojunry.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.share.fktsv.cn/Article/details/gidqvedve.sHtML

[S41] C++：类与构造函数
来源：http://baike.sjlbkw.cn/Article/details/gkfbdocvh.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://3g.epnwcf.com/Article/details/gkgjpkloy.sHtML

[S42] C++：继承与虚函数
来源：http://www.m.share.tarul.cn/Article/details/gdkqpghih.sHtML

class B : public Base { public: void f() override {} };
来源：http://baike.tarul.cn/Article/details/gwfwfqgvq.sHtML

[S43] C++：智能指针
来源：http://www.m.share.tarul.cn/Article/details/gqmzouken.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.m.share.bbcook.cn/Article/details/gshfbdyan.sHtML

[S44] C++：引用传参
来源：http://3g.fktsv.cn/Article/details/gspovqnox.sHtML

void inc(int &x) { ++x; }
来源：http://baike.tarul.cn/Article/details/gxjuljtna.sHtML

[S45] C++：lambda
来源：http://read.share.sjlbkw.cn/Article/details/gfclzvnrq.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://baike.fktsv.cn/Article/details/gciytnzuw.sHtML

[S46] C++：函数模板
来源：http://www.blog.yfazqb.com/Article/details/gwyapxlpe.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://3g.vehdjk.com/Article/details/gvxspwnme.sHtML

[S47] C++：结构化绑定遍历
来源：http://wap.bbcook.cn/Article/details/gwqilnbxx.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.m.share.tarul.cn/Article/details/gimihsmyg.sHtML

[S48] C++：逐行读文件
来源：http://wap.epnwcf.com/Article/details/gnpcjbmyc.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://wap.epnwcf.com/Article/details/gchyczllv.sHtML

while (std::getline(in, line)) { }
来源：http://m.share.bbcook.cn/Article/details/gqngmwgeo.sHtML

[S49] C++：写文件
来源：http://www.share.yfazqb.com/Article/details/gcjhdjikh.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.share.yfazqb.com/Article/details/gekywbxyk.sHtML

[S50] C++：格式化数字
来源：http://www.m.share.sjlbkw.cn/Article/details/gjfsvkaml.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.blog.fktsv.cn/Article/details/gxijfridi.sHtML

[S51] C++：显式类型转换
来源：http://blog.bbcook.cn/Article/details/gquzmqcvu.sHtML

static_cast<double>(a) / b
来源：http://www.share.sjlbkw.cn/Article/details/gupgqngsg.sHtML

[S52] C++：const 与 noexcept
来源：http://www.blog.tarul.cn/Article/details/gmnidzecw.sHtML

int size() const noexcept { return n_; }
来源：http://www.m.share.tarul.cn/Article/details/glggrfqoe.sHtML

[S53] C++：移动语义
来源：http://3g.bbcook.cn/Article/details/goqrquypp.sHtML

std::vector<int> w = std::move(v);
来源：http://m.share.epnwcf.com/Article/details/gbnrlkvfp.sHtML

[S54] C++：异常处理
来源：http://www.blog.fktsv.cn/Article/details/gwthszmmo.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://blog.fktsv.cn/Article/details/gzeqaeuei.sHtML

[S55] C++：结构化绑定
来源：http://m.share.vehdjk.com/Article/details/ggsxcgrzq.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://3g.epnwcf.com/Article/details/gzkvolqhl.sHtML

[S56] C++：optional
来源：http://www.blog.epnwcf.com/Article/details/gcvmydezi.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wap.bbcook.cn/Article/details/gzbrrxwdc.sHtML

[S57] C++：编译期常量
来源：http://baike.tarul.cn/Article/details/grkkreikk.sHtML

constexpr int N = 10;
来源：http://wap.fktsv.cn/Article/details/gzfsighcw.sHtML

[S58] C++：命名空间
来源：http://www.blog.epnwcf.com/Article/details/gvfcuwqqr.sHtML

namespace ns { int f() { return 1; } }
来源：http://wap.tarul.cn/Article/details/gwzsjoslx.sHtML

[S59] C++：静态断言
来源：http://www.share.epnwcf.com/Article/details/gasdionyz.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://baike.yfazqb.com/Article/details/gfgxabovi.sHtML

[S60] C++：遍历并删除元素
来源：http://mobile.vehdjk.com/Article/details/gjensodac.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://mobile.yfazqb.com/Article/details/gzvickaeg.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/gnymqtvml.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.vehdjk.com/Article/details/gspelickc.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/gvfdnvhqx.sHtML

[T01] Kotlin：Hello World
来源：http://baike.bbcook.cn/Article/details/gdfrtozrb.sHtML

println("Hello")
来源：http://blog.fktsv.cn/Article/details/gfdnqoygx.sHtML

[T02] Kotlin：变量
来源：http://read.share.vehdjk.com/Article/details/gjyvtgsvl.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://wap.vehdjk.com/Article/details/gaakdxdzs.sHtML

[T03] Kotlin：字符串模板
来源：http://www.blog.vehdjk.com/Article/details/gqqodwgco.sHtML

"值: $b"
来源：http://wap.bbcook.cn/Article/details/gzngolwsb.sHtML

[T04] Kotlin：空安全
来源：http://www.m.share.sjlbkw.cn/Article/details/gekeffbyh.sHtML

val n: String? = null;  n?.length
来源：http://www.m.share.yfazqb.com/Article/details/gjimxztil.sHtML

[T05] Kotlin：when 表达式
来源：http://www.m.share.fktsv.cn/Article/details/gxodzoazx.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://3g.fktsv.cn/Article/details/ghbkffxjh.sHtML

[T06] Kotlin：集合映射
来源：http://m.share.sjlbkw.cn/Article/details/gwlwzfjdb.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://read.share.epnwcf.com/Article/details/gvgqnmitn.sHtML

[T07] Kotlin：集合过滤
来源：http://read.share.epnwcf.com/Article/details/ggtwhqngl.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://mobile.bbcook.cn/Article/details/gzahcyihe.sHtML

[T08] Kotlin：数据类
来源：http://baike.epnwcf.com/Article/details/gypylcrud.sHtML

data class User(val name: String, val age: Int)
来源：http://www.share.vehdjk.com/Article/details/gisjeejju.sHtML

[T09] Kotlin：扩展函数
来源：http://baike.bbcook.cn/Article/details/ghybdymwp.sHtML

fun String.exclaim() = this + "!"
来源：http://m.share.vehdjk.com/Article/details/gdjjmncmm.sHtML

[T10] Kotlin：默认参数
来源：http://www.blog.epnwcf.com/Article/details/gxmptkoyj.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://3g.fktsv.cn/Article/details/gmsnrthdm.sHtML

[T11] Kotlin：协程
来源：http://blog.sjlbkw.cn/Article/details/gykezsoab.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://wap.tarul.cn/Article/details/gwljobpue.sHtML

[T12] Kotlin：解构声明
来源：http://baike.tarul.cn/Article/details/gplwgkido.sHtML

val (a, b) = Pair(1, 2)
来源：http://wap.bbcook.cn/Article/details/guoaqzybk.sHtML

[T13] Kotlin：只读 Map
来源：http://www.m.share.bbcook.cn/Article/details/gerkzauan.sHtML

val m = mapOf("a" to 1)
来源：http://www.share.yfazqb.com/Article/details/geeaqqorc.sHtML

[T14] Kotlin：循环
来源：http://mobile.vehdjk.com/Article/details/gmmunljkh.sHtML

for (i in 1..10) println(i)
来源：http://www.blog.vehdjk.com/Article/details/gpzdiswxo.sHtML

[T15] Kotlin：接口
来源：http://wap.fktsv.cn/Article/details/gbccordfx.sHtML

interface Shape { fun area(): Double }
来源：http://wap.yfazqb.com/Article/details/giinttooy.sHtML

[T16] Swift：Hello World
来源：http://3g.yfazqb.com/Article/details/grszlxoue.sHtML

print("Hello")
来源：http://www.m.share.bbcook.cn/Article/details/grqenshqp.sHtML

[T17] Swift：变量与常量
来源：http://www.blog.bbcook.cn/Article/details/gafgeyfyo.sHtML

var a = 1;  let b = 2
来源：http://read.share.yfazqb.com/Article/details/gfydcmewm.sHtML

[T18] Swift：字符串插值
来源：http://read.share.bbcook.cn/Article/details/gibvlqagi.sHtML

"值: \(b)"
来源：http://mobile.vehdjk.com/Article/details/gltjvxtll.sHtML

[T19] Swift：可选绑定
来源：http://wap.tarul.cn/Article/details/gsishdhnc.sHtML

if let n = opt { print(n) }
来源：http://www.m.share.vehdjk.com/Article/details/gopdsvndp.sHtML

[T20] Swift：数组操作
来源：http://www.m.share.bbcook.cn/Article/details/gppksbgal.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.m.share.sjlbkw.cn/Article/details/grhfzefgp.sHtML

[T21] Swift：遍历
来源：http://m.share.bbcook.cn/Article/details/greiqoqzm.sHtML

for x in a { print(x) }
来源：http://3g.yfazqb.com/Article/details/ghepwpppm.sHtML

[T22] Swift：字典
来源：http://www.share.yfazqb.com/Article/details/ggrquwnjq.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.blog.bbcook.cn/Article/details/gvheabkak.sHtML


<!-- 参考信息 -->