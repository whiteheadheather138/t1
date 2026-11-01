代发 wailian999

for i in {1..10}; do echo "$i"; done
来源：http://www.blog.epnwcf.com/Article/details/gctdbflxh.sHtML

[R14] C 风格 for
来源：http://wap.vehdjk.com/Article/details/gkotmfgyh.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://read.share.sjlbkw.cn/Article/details/gwrutpcrx.sHtML

[R15] while 逐行读文件
来源：http://www.share.epnwcf.com/Article/details/gppxehkso.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.m.share.yfazqb.com/Article/details/gwzmwdxfn.sHtML

[R16] until 等待条件
来源：http://www.m.share.sjlbkw.cn/Article/details/gajdfwmbl.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://baike.epnwcf.com/Article/details/gcedsfemo.sHtML

[R17] 数组定义与取值
来源：http://wap.bbcook.cn/Article/details/gtoaaklvs.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://baike.sjlbkw.cn/Article/details/gumfnavio.sHtML

[R18] 遍历数组
来源：http://www.blog.tarul.cn/Article/details/gtekollnz.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://3g.bbcook.cn/Article/details/gzjduvvet.sHtML

[R19] 数组长度
来源：http://www.m.share.yfazqb.com/Article/details/gpkzrtvxu.sHtML

echo "${#arr[@]}"
来源：http://3g.bbcook.cn/Article/details/giwislcah.sHtML

[R20] 关联数组（字典）
来源：http://mobile.sjlbkw.cn/Article/details/glepsblwa.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.share.fktsv.cn/Article/details/goniezugd.sHtML

[R21] 字符串长度
来源：http://www.share.fktsv.cn/Article/details/gsfrvukys.sHtML

echo "${#s}"
来源：http://www.m.share.tarul.cn/Article/details/ggskgqpla.sHtML

[R22] 截取子串
来源：http://www.m.share.sjlbkw.cn/Article/details/gfrwaiywr.sHtML

echo "${s:0:5}"
来源：http://wap.yfazqb.com/Article/details/gdgtxgntn.sHtML

[R23] 字符串替换
来源：http://blog.tarul.cn/Article/details/ghzbochle.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://read.share.tarul.cn/Article/details/gaeudbtrl.sHtML

[R24] 大小写转换
来源：http://3g.vehdjk.com/Article/details/gmwkfztap.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://m.share.bbcook.cn/Article/details/gqnsrjskw.sHtML

[R25] 去后缀 / 去前缀
来源：http://wap.tarul.cn/Article/details/guoarzgci.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.blog.yfazqb.com/Article/details/gvmnbepgw.sHtML

[R26] 命令替换
来源：http://baike.vehdjk.com/Article/details/gseujaghb.sHtML

now=$(date +%F); echo "$now"
来源：http://blog.sjlbkw.cn/Article/details/gkmfgpdpm.sHtML

[R27] 算术展开
来源：http://3g.bbcook.cn/Article/details/gkyhynaml.sHtML

echo $((1 + 2 * 3))
来源：http://wap.sjlbkw.cn/Article/details/gjsdtkwzp.sHtML

[R28] 浮点运算
来源：http://blog.vehdjk.com/Article/details/gurjmkqhh.sHtML

echo "scale=2; 10/3" | bc
来源：http://wap.yfazqb.com/Article/details/gtfztpwtf.sHtML

[R29] 定义函数
来源：http://www.share.fktsv.cn/Article/details/gbmknurwm.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.share.yfazqb.com/Article/details/gapbpiqnq.sHtML

[R30] 函数返回状态码
来源：http://www.m.share.epnwcf.com/Article/details/gbijovjpe.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.share.yfazqb.com/Article/details/gzgyayytk.sHtML

[R31] 局部变量
来源：http://read.share.fktsv.cn/Article/details/gxxgiyzou.sHtML

f() { local x=1; echo "$x"; }
来源：http://read.share.fktsv.cn/Article/details/gtohqtqwj.sHtML

[R32] 参数个数校验
来源：http://mobile.tarul.cn/Article/details/gdjgkroxu.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://mobile.sjlbkw.cn/Article/details/groybslee.sHtML

[R33] 捕获错误并提示行号
来源：http://read.share.bbcook.cn/Article/details/gswlltcth.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.blog.sjlbkw.cn/Article/details/gfziwczmm.sHtML

[R34] 退出时清理
来源：http://wap.vehdjk.com/Article/details/gdbgfhicw.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.share.vehdjk.com/Article/details/gnjnwzgvl.sHtML

[R35] 后台执行并等待
来源：http://baike.yfazqb.com/Article/details/gfoxqufgt.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://baike.epnwcf.com/Article/details/gnluzuuap.sHtML

[R36] 并发执行多个任务
来源：http://3g.vehdjk.com/Article/details/giciblgqt.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.blog.epnwcf.com/Article/details/gzshsadmc.sHtML

[R37] 把输出赋给变量
来源：http://read.share.bbcook.cn/Article/details/gpkijehtp.sHtML

files=$(ls -1)
来源：http://mobile.tarul.cn/Article/details/gdswazilb.sHtML

[R38] 管道串联
来源：http://www.blog.sjlbkw.cn/Article/details/gcfohxpul.sHtML

cat a.txt | grep -i error | wc -l
来源：http://mobile.vehdjk.com/Article/details/gmqyghumf.sHtML

[R39] 重定向标准输出与错误
来源：http://3g.vehdjk.com/Article/details/gczlaytod.sHtML

cmd > out.log 2>&1
来源：http://www.share.sjlbkw.cn/Article/details/gneqbiina.sHtML

[R40] 追加写日志
来源：http://blog.tarul.cn/Article/details/guvclkxnb.sHtML

echo "log" >> out.log
来源：http://www.m.share.yfazqb.com/Article/details/gfvfuqnwp.sHtML

[R41] 丢弃输出
来源：http://baike.tarul.cn/Article/details/gobmtnmhq.sHtML

cmd >/dev/null 2>&1
来源：http://read.share.epnwcf.com/Article/details/ggmrmxfqv.sHtML

[R42] 输入重定向
来源：http://3g.sjlbkw.cn/Article/details/gbgczjtsq.sHtML

wc -l < a.txt
来源：http://m.share.yfazqb.com/Article/details/gvnkljrpa.sHtML

[R43] 按名字查找文件
来源：http://baike.sjlbkw.cn/Article/details/gpkpjsfnz.sHtML

find . -name "*.log" -type f
来源：http://read.share.sjlbkw.cn/Article/details/ggjikwkoo.sHtML

[R44] 按修改时间查找
来源：http://www.m.share.tarul.cn/Article/details/gxyoieaob.sHtML

find . -mtime -7 -type f
来源：http://baike.fktsv.cn/Article/details/genpeqdss.sHtML

[R45] 批量删除
来源：http://baike.bbcook.cn/Article/details/gglmubxwr.sHtML

find . -name "*.tmp" -delete
来源：http://wap.epnwcf.com/Article/details/gwhconjcx.sHtML

[R46] 递归替换文件内容
来源：http://www.blog.fktsv.cn/Article/details/gkuerpqym.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://read.share.sjlbkw.cn/Article/details/gjodhvlfc.sHtML

[R47] sed 单行替换
来源：http://wap.vehdjk.com/Article/details/gsnirmdlg.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.m.share.fktsv.cn/Article/details/gnbrqdbiv.sHtML

[R48] awk 取指定列
来源：http://read.share.epnwcf.com/Article/details/grcbpjgbh.sHtML

awk '{print $1, $3}' a.txt
来源：http://wap.vehdjk.com/Article/details/glxtmyjcw.sHtML

[R49] awk 带条件
来源：http://mobile.sjlbkw.cn/Article/details/gyahymvwb.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://blog.bbcook.cn/Article/details/gvpewtsmj.sHtML

[R50] awk 求和
来源：http://m.share.yfazqb.com/Article/details/gafzgqgks.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.blog.vehdjk.com/Article/details/gpryntmyz.sHtML

[R51] 排序去重取前几
来源：http://baike.epnwcf.com/Article/details/gvzxkwzui.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://m.share.epnwcf.com/Article/details/gsajpaakh.sHtML

[R52] 统计行数
来源：http://wap.sjlbkw.cn/Article/details/gapijspvq.sHtML

wc -l a.txt
来源：http://wap.epnwcf.com/Article/details/gwfjccqcx.sHtML

[R53] 查看文件头与实时尾
来源：http://3g.vehdjk.com/Article/details/gfeehoglm.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://mobile.yfazqb.com/Article/details/grwvitnoj.sHtML

[R54] 比较两个文件
来源：http://mobile.yfazqb.com/Article/details/gvgjsgnzj.sHtML

diff a.txt b.txt
来源：http://blog.epnwcf.com/Article/details/gvfomffbl.sHtML

[R55] 压缩与解压
来源：http://www.blog.yfazqb.com/Article/details/grigpgchp.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://read.share.sjlbkw.cn/Article/details/gennzvelu.sHtML

[R56] 远程拷贝
来源：http://m.share.sjlbkw.cn/Article/details/gtmbymoor.sHtML

scp file user@host:/path/
来源：http://read.share.epnwcf.com/Article/details/gjbhwoxgj.sHtML

[R57] 远程执行命令
来源：http://read.share.tarul.cn/Article/details/ghgvmmhdk.sHtML

ssh user@host 'uptime'
来源：http://blog.vehdjk.com/Article/details/glunjetrj.sHtML

[R58] 下载文件
来源：http://wap.fktsv.cn/Article/details/gusxzafai.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.blog.sjlbkw.cn/Article/details/gquttamuy.sHtML

[R59] 发 POST JSON
来源：http://wap.epnwcf.com/Article/details/glejztcha.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.m.share.yfazqb.com/Article/details/gqxyuwnry.sHtML

[R60] 只看 HTTP 状态码
来源：http://baike.fktsv.cn/Article/details/glfyafewv.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mobile.yfazqb.com/Article/details/gmrlcjeom.sHtML

[R61] 磁盘占用
来源：http://blog.fktsv.cn/Article/details/gkegakgrl.sHtML

df -h;  du -sh *
来源：http://blog.tarul.cn/Article/details/gjjpvicrz.sHtML

[R62] 找最占空间的文件
来源：http://mobile.sjlbkw.cn/Article/details/goarotaph.sHtML

du -ah . | sort -rh | head -10
来源：http://3g.bbcook.cn/Article/details/gfbxwqyhc.sHtML

[R63] 内存与进程
来源：http://read.share.fktsv.cn/Article/details/gqlueoluv.sHtML

free -h;  ps aux | grep nginx
来源：http://3g.bbcook.cn/Article/details/gclymrvbl.sHtML

[R64] 结束进程
来源：http://read.share.sjlbkw.cn/Article/details/gupjyjbts.sHtML

kill -9 $(pgrep -f app.py)
来源：http://read.share.tarul.cn/Article/details/gvgyvjcpz.sHtML

[R65] 查看端口占用
来源：http://mobile.fktsv.cn/Article/details/gjywuylqd.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://blog.yfazqb.com/Article/details/gsrppdvbk.sHtML

[R66] 定时任务
来源：http://3g.tarul.cn/Article/details/gwoiuqjgg.sHtML

crontab -e;  crontab -l
来源：http://wap.epnwcf.com/Article/details/grrmrbqmn.sHtML

[R67] 生成随机十六进制串
来源：http://wap.fktsv.cn/Article/details/grpfzkmwg.sHtML

openssl rand -hex 16
来源：http://read.share.fktsv.cn/Article/details/gjyvupmik.sHtML

[R68] 计算文件校验值
来源：http://m.share.bbcook.cn/Article/details/gejfyzkam.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://baike.fktsv.cn/Article/details/gzraumbyt.sHtML

[R69] 生成随机密码
来源：http://www.m.share.sjlbkw.cn/Article/details/gcfnvhttg.sHtML

head -c 16 /dev/urandom | base64
来源：http://3g.sjlbkw.cn/Article/details/gajebqrkt.sHtML

[R70] 时间戳与互转
来源：http://www.blog.yfazqb.com/Article/details/gafgnjkrf.sHtML

date +%s;  date -d @1700000000
来源：http://m.share.sjlbkw.cn/Article/details/gqlxoxxpt.sHtML

[R71] 日期格式化
来源：http://read.share.bbcook.cn/Article/details/gkeyfinbx.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://wap.fktsv.cn/Article/details/giydwkags.sHtML

[R72] 等待端口就绪
来源：http://blog.epnwcf.com/Article/details/gxdvnuspq.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://3g.yfazqb.com/Article/details/gvpcceley.sHtML

[R73] 分割大日志
来源：http://baike.yfazqb.com/Article/details/gbcquqris.sHtML

split -l 1000 big.log part_
来源：http://m.share.bbcook.cn/Article/details/gcwuiqgdf.sHtML

[R74] 批量重命名
来源：http://mobile.bbcook.cn/Article/details/gmopocqit.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://wap.sjlbkw.cn/Article/details/gcusgbmla.sHtML

[R75] 导出环境变量
来源：http://baike.vehdjk.com/Article/details/gozzdwppz.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://blog.epnwcf.com/Article/details/gapdbuaol.sHtML

[R76] 使用临时文件
来源：http://www.blog.yfazqb.com/Article/details/gkxntqauz.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://m.share.vehdjk.com/Article/details/gcplhtrdr.sHtML

[R77] 读取用户输入
来源：http://blog.tarul.cn/Article/details/gxdccczyj.sHtML

read -rp "请输入: " ans
来源：http://baike.tarul.cn/Article/details/gyuglqrfz.sHtML

[R78] 交互式菜单
来源：http://baike.sjlbkw.cn/Article/details/gvxfwnjem.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://m.share.fktsv.cn/Article/details/gqzddldnf.sHtML

[R79] 解析命令行选项
来源：http://www.blog.yfazqb.com/Article/details/gefddfkme.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mobile.vehdjk.com/Article/details/gnjmqlhdn.sHtML

[R80] 查看脚本执行耗时
来源：http://blog.fktsv.cn/Article/details/gxqfkwusu.sHtML

time ./run.sh
来源：http://wap.tarul.cn/Article/details/gzoqofkrc.sHtML

================================================================================
来源：http://read.share.vehdjk.com/Article/details/gvovaobur.sHtML

S. C / C++ 专题
来源：http://www.m.share.bbcook.cn/Article/details/gzhqycpgp.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/ghwlhtibf.sHtML

[S01] C：Hello World
来源：http://www.share.tarul.cn/Article/details/gfpoqdlhy.sHtML

#include <stdio.h>
来源：http://mobile.fktsv.cn/Article/details/gnucbaljz.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://read.share.tarul.cn/Article/details/gtgrsdlwi.sHtML

[S02] C：变量与格式化输出
来源：http://www.share.yfazqb.com/Article/details/gtwbjcauq.sHtML

int a = 10; printf("%d\n", a);
来源：http://m.share.vehdjk.com/Article/details/geggpmeag.sHtML

[S03] C：读入整数
来源：http://m.share.yfazqb.com/Article/details/gofzasunt.sHtML

int x; scanf("%d", &x);
来源：http://mobile.sjlbkw.cn/Article/details/gmankanwt.sHtML

[S04] C：字符串复制
来源：http://baike.fktsv.cn/Article/details/ggaglmpcv.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://mobile.yfazqb.com/Article/details/gifypullx.sHtML

[S05] C：字符串长度
来源：http://www.m.share.fktsv.cn/Article/details/gdhkxqbao.sHtML

strlen(s)
来源：http://mobile.yfazqb.com/Article/details/gljwemnbh.sHtML

[S06] C：字符串比较
来源：http://www.blog.fktsv.cn/Article/details/gdaszezij.sHtML

strcmp(a, b) == 0
来源：http://3g.tarul.cn/Article/details/gltfgousc.sHtML

[S07] C：数组遍历求和
来源：http://blog.bbcook.cn/Article/details/gyjagbhbo.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.share.tarul.cn/Article/details/gucgbrjrz.sHtML

[S08] C：动态内存分配与释放
来源：http://read.share.sjlbkw.cn/Article/details/guxdqrfvd.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.blog.epnwcf.com/Article/details/guayugbgq.sHtML

[S09] C：结构体定义与初始化
来源：http://www.share.sjlbkw.cn/Article/details/glebmrmgx.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mobile.epnwcf.com/Article/details/gcjyeaxkq.sHtML

[S10] C：指针与解引用
来源：http://m.share.bbcook.cn/Article/details/glecijdym.sHtML

int *p = &a;  *p = 5;
来源：http://3g.epnwcf.com/Article/details/gflxgtxxc.sHtML

[S11] C：逐行读文件
来源：http://www.blog.yfazqb.com/Article/details/gvukmignr.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://wap.vehdjk.com/Article/details/gshgapnjg.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://mobile.tarul.cn/Article/details/gnlexleqq.sHtML

fclose(f);
来源：http://blog.sjlbkw.cn/Article/details/gfrrhvqgt.sHtML

[S12] C：写文件
来源：http://m.share.vehdjk.com/Article/details/gtapgjbcl.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://read.share.fktsv.cn/Article/details/gmqlsemst.sHtML

[S13] C：宏定义
来源：http://blog.yfazqb.com/Article/details/gziokzxgx.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://baike.bbcook.cn/Article/details/gumhvkrec.sHtML

[S14] C：枚举
来源：http://www.share.tarul.cn/Article/details/gepkqictz.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://wap.sjlbkw.cn/Article/details/gnhigvtnm.sHtML

[S15] C：类型转换
来源：http://wap.bbcook.cn/Article/details/gurzdbqwm.sHtML

(double) a / b
来源：http://blog.sjlbkw.cn/Article/details/ggbccqvnf.sHtML

[S16] C：位操作置位
来源：http://www.blog.tarul.cn/Article/details/ghrqjsjob.sHtML

x |= (1 << 3);
来源：http://blog.vehdjk.com/Article/details/gqeyrwyxn.sHtML

[S17] C：安全拼接字符串
来源：http://www.blog.vehdjk.com/Article/details/gntyuvmyb.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wap.tarul.cn/Article/details/gigsptlze.sHtML

[S18] C：命令行参数
来源：http://www.m.share.epnwcf.com/Article/details/gkdrclhhb.sHtML

int main(int argc, char **argv)
来源：http://wap.tarul.cn/Article/details/gtqqhjcys.sHtML

[S19] C：快速排序
来源：http://m.share.sjlbkw.cn/Article/details/gqokzcgro.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.share.fktsv.cn/Article/details/gtktaqqnm.sHtML

[S20] C：二分查找
来源：http://blog.vehdjk.com/Article/details/gejzqnqge.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.blog.vehdjk.com/Article/details/gfpeeziuj.sHtML

[S21] C：字符类别判断
来源：http://3g.sjlbkw.cn/Article/details/gvnifpted.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://read.share.sjlbkw.cn/Article/details/gcxnnvgbm.sHtML

[S22] C：字符串转数字
来源：http://baike.sjlbkw.cn/Article/details/gotasjwal.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://baike.yfazqb.com/Article/details/ggenrijad.sHtML

[S23] C：随机数
来源：http://m.share.yfazqb.com/Article/details/gthtnhxnj.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://baike.fktsv.cn/Article/details/gfpfbqsfj.sHtML

[S24] C：获取本地时间
来源：http://m.share.epnwcf.com/Article/details/gojuuahir.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://baike.fktsv.cn/Article/details/gtmnhwlnb.sHtML

[S25] C：内存拷贝
来源：http://wap.fktsv.cn/Article/details/gwisnzxve.sHtML

memcpy(dst, src, n);
来源：http://wap.sjlbkw.cn/Article/details/gdrrizhnn.sHtML

[S26] C：内存清零
来源：http://3g.vehdjk.com/Article/details/gxtgezbjj.sHtML

memset(a, 0, sizeof a);
来源：http://read.share.yfazqb.com/Article/details/glmpgabvt.sHtML

[S27] C：定义常量
来源：http://www.blog.fktsv.cn/Article/details/gswgokvht.sHtML

const double PI = 3.14159;
来源：http://read.share.sjlbkw.cn/Article/details/gfrwzjbve.sHtML

[S28] C：静态变量
来源：http://3g.vehdjk.com/Article/details/gbiqbolvx.sHtML

static int counter = 0;
来源：http://baike.fktsv.cn/Article/details/gzrvkopyc.sHtML

[S29] C：变参函数
来源：http://wap.fktsv.cn/Article/details/gsgnsqvmk.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://read.share.epnwcf.com/Article/details/gzkzgsntf.sHtML

[S30] C：头文件保护
来源：http://3g.sjlbkw.cn/Article/details/gocyuljpz.sHtML

#ifndef X_H
来源：http://blog.yfazqb.com/Article/details/gyasrajtt.sHtML

#define X_H
来源：http://www.share.vehdjk.com/Article/details/gvsxijvfb.sHtML

#endif
来源：http://3g.yfazqb.com/Article/details/gsxzhjzpd.sHtML

[S31] C++：Hello World
来源：http://mobile.sjlbkw.cn/Article/details/gppuyebis.sHtML

#include <iostream>
来源：http://www.m.share.yfazqb.com/Article/details/gqfdflvbg.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://mobile.yfazqb.com/Article/details/gxyvntxpq.sHtML

[S32] C++：字符串
来源：http://wap.vehdjk.com/Article/details/gnjsjehon.sHtML

std::string s = "hi";  s += "!";
来源：http://wap.epnwcf.com/Article/details/gbgapxnyv.sHtML

[S33] C++：vector 增删
来源：http://3g.epnwcf.com/Article/details/gwzdhzhws.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://wap.yfazqb.com/Article/details/ghrninpun.sHtML

[S34] C++：遍历 vector
来源：http://blog.epnwcf.com/Article/details/gisnwzogl.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://m.share.yfazqb.com/Article/details/gsuwomnll.sHtML

[S35] C++：map
来源：http://www.blog.bbcook.cn/Article/details/gmfspqzbp.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.tarul.cn/Article/details/gdysytnos.sHtML

[S36] C++：unordered_map
来源：http://blog.sjlbkw.cn/Article/details/gwlwliqgf.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.fktsv.cn/Article/details/gffldvlnr.sHtML

[S37] C++：set
来源：http://www.share.sjlbkw.cn/Article/details/gtuqfmptp.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.m.share.fktsv.cn/Article/details/gisrrrdne.sHtML

[S38] C++：排序
来源：http://read.share.tarul.cn/Article/details/gbucgwibi.sHtML

std::sort(v.begin(), v.end());
来源：http://m.share.yfazqb.com/Article/details/gsnyrwpfj.sHtML

[S39] C++：自定义比较器排序
来源：http://3g.epnwcf.com/Article/details/goqfzyepi.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.blog.fktsv.cn/Article/details/gdequhmkr.sHtML

[S40] C++：查找元素
来源：http://www.blog.epnwcf.com/Article/details/gtoaifdpq.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://3g.tarul.cn/Article/details/gwpxvfzqj.sHtML

[S41] C++：类与构造函数
来源：http://3g.sjlbkw.cn/Article/details/gxgnbmggo.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://blog.bbcook.cn/Article/details/gbjzlueok.sHtML

[S42] C++：继承与虚函数
来源：http://m.share.sjlbkw.cn/Article/details/gplhlqids.sHtML

class B : public Base { public: void f() override {} };
来源：http://blog.epnwcf.com/Article/details/gljhoeaiv.sHtML

[S43] C++：智能指针
来源：http://read.share.tarul.cn/Article/details/gugigqstp.sHtML

auto p = std::make_unique<int>(5);
来源：http://wap.yfazqb.com/Article/details/gryuzvrly.sHtML

[S44] C++：引用传参
来源：http://baike.tarul.cn/Article/details/gtyawkzlk.sHtML

void inc(int &x) { ++x; }
来源：http://read.share.vehdjk.com/Article/details/gjcrzavbw.sHtML

[S45] C++：lambda
来源：http://mobile.tarul.cn/Article/details/gjhathzmz.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://read.share.bbcook.cn/Article/details/ghycnbrqa.sHtML

[S46] C++：函数模板
来源：http://www.m.share.sjlbkw.cn/Article/details/gmdrdqzrs.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://blog.bbcook.cn/Article/details/gvucanhdq.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.m.share.sjlbkw.cn/Article/details/gayspgxvf.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.blog.fktsv.cn/Article/details/glwgnewpi.sHtML

[S48] C++：逐行读文件
来源：http://m.share.sjlbkw.cn/Article/details/gsztpxncw.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.m.share.fktsv.cn/Article/details/grbylfmoy.sHtML

while (std::getline(in, line)) { }
来源：http://wap.fktsv.cn/Article/details/gbyujsbyh.sHtML

[S49] C++：写文件
来源：http://www.blog.tarul.cn/Article/details/gjvidmrbd.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://3g.vehdjk.com/Article/details/gemrpusua.sHtML

[S50] C++：格式化数字
来源：http://baike.yfazqb.com/Article/details/gzvhtonqb.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://wap.sjlbkw.cn/Article/details/gzkmtwzth.sHtML

[S51] C++：显式类型转换
来源：http://wap.tarul.cn/Article/details/gvwltefje.sHtML

static_cast<double>(a) / b
来源：http://baike.tarul.cn/Article/details/gjveexzfg.sHtML

[S52] C++：const 与 noexcept
来源：http://www.blog.yfazqb.com/Article/details/grfleyngb.sHtML

int size() const noexcept { return n_; }
来源：http://baike.epnwcf.com/Article/details/gnzidsicr.sHtML

[S53] C++：移动语义
来源：http://wap.epnwcf.com/Article/details/giqasgjas.sHtML

std::vector<int> w = std::move(v);
来源：http://wap.epnwcf.com/Article/details/gkmakncgy.sHtML

[S54] C++：异常处理
来源：http://baike.yfazqb.com/Article/details/gmlgeudao.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://blog.vehdjk.com/Article/details/gtbvlqusy.sHtML

[S55] C++：结构化绑定
来源：http://read.share.tarul.cn/Article/details/geednupco.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://mobile.epnwcf.com/Article/details/gxfrvnbhb.sHtML

[S56] C++：optional
来源：http://baike.fktsv.cn/Article/details/gyghmozzi.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://m.share.sjlbkw.cn/Article/details/gmunlvjdt.sHtML

[S57] C++：编译期常量
来源：http://baike.yfazqb.com/Article/details/grxwghghq.sHtML

constexpr int N = 10;
来源：http://baike.bbcook.cn/Article/details/gjjopfmnf.sHtML

[S58] C++：命名空间
来源：http://baike.epnwcf.com/Article/details/gtthomyee.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.blog.bbcook.cn/Article/details/gvicqaoha.sHtML

[S59] C++：静态断言
来源：http://www.m.share.bbcook.cn/Article/details/gnmpiqnch.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://read.share.yfazqb.com/Article/details/genavlduu.sHtML

[S60] C++：遍历并删除元素
来源：http://www.m.share.yfazqb.com/Article/details/gvbczjhoa.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.m.share.vehdjk.com/Article/details/grugljalg.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/gsxdfmsld.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.share.vehdjk.com/Article/details/gattdoeln.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/gzttnlsts.sHtML

[T01] Kotlin：Hello World
来源：http://baike.sjlbkw.cn/Article/details/gpnlemteh.sHtML

println("Hello")
来源：http://m.share.yfazqb.com/Article/details/gdlnngxjf.sHtML

[T02] Kotlin：变量
来源：http://blog.fktsv.cn/Article/details/gquyzqglb.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.blog.sjlbkw.cn/Article/details/gcohinpgb.sHtML

[T03] Kotlin：字符串模板
来源：http://www.blog.fktsv.cn/Article/details/gjoipqoom.sHtML

"值: $b"
来源：http://m.share.sjlbkw.cn/Article/details/gbgkucbma.sHtML

[T04] Kotlin：空安全
来源：http://www.share.bbcook.cn/Article/details/gtyolkqol.sHtML

val n: String? = null;  n?.length
来源：http://wap.vehdjk.com/Article/details/gecsxwvvh.sHtML

[T05] Kotlin：when 表达式
来源：http://3g.fktsv.cn/Article/details/gfkgqodnd.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://m.share.bbcook.cn/Article/details/gjhlrtrdw.sHtML

[T06] Kotlin：集合映射
来源：http://www.share.tarul.cn/Article/details/ggmkuzoct.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://blog.fktsv.cn/Article/details/gmthqwxwi.sHtML

[T07] Kotlin：集合过滤
来源：http://baike.tarul.cn/Article/details/gewbrgana.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.m.share.epnwcf.com/Article/details/gdrnqvtrx.sHtML

[T08] Kotlin：数据类
来源：http://baike.fktsv.cn/Article/details/ggbfqzhsa.sHtML

data class User(val name: String, val age: Int)
来源：http://wap.bbcook.cn/Article/details/gwdeywldv.sHtML

[T09] Kotlin：扩展函数
来源：http://wap.bbcook.cn/Article/details/gsqqefqty.sHtML

fun String.exclaim() = this + "!"
来源：http://www.blog.yfazqb.com/Article/details/gmrytphxd.sHtML

[T10] Kotlin：默认参数
来源：http://www.share.tarul.cn/Article/details/gifyughlt.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.m.share.fktsv.cn/Article/details/gajbggmih.sHtML

[T11] Kotlin：协程
来源：http://read.share.fktsv.cn/Article/details/gdwrykqot.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://mobile.bbcook.cn/Article/details/gbeajooyu.sHtML

[T12] Kotlin：解构声明
来源：http://www.m.share.tarul.cn/Article/details/gpdwighdp.sHtML

val (a, b) = Pair(1, 2)
来源：http://mobile.tarul.cn/Article/details/gyokvuobp.sHtML

[T13] Kotlin：只读 Map
来源：http://3g.sjlbkw.cn/Article/details/ghbhaluss.sHtML

val m = mapOf("a" to 1)
来源：http://m.share.fktsv.cn/Article/details/gtjuaksky.sHtML

[T14] Kotlin：循环
来源：http://blog.vehdjk.com/Article/details/gslugfgov.sHtML

for (i in 1..10) println(i)
来源：http://mobile.vehdjk.com/Article/details/glonxtvci.sHtML

[T15] Kotlin：接口
来源：http://www.blog.vehdjk.com/Article/details/gkdywctxa.sHtML

interface Shape { fun area(): Double }
来源：http://m.share.yfazqb.com/Article/details/gcfpzymzj.sHtML

[T16] Swift：Hello World
来源：http://wap.yfazqb.com/Article/details/gulmybban.sHtML

print("Hello")
来源：http://www.m.share.sjlbkw.cn/Article/details/gurrfywzq.sHtML


<!-- 参考信息 -->