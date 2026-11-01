代发 wailian999

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://3g.tarul.cn/Article/details/gstodjhiw.sHtML

[R08] 数值比较
来源：http://www.m.share.sjlbkw.cn/Article/details/gxiwbvajp.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.blog.tarul.cn/Article/details/gvqthubny.sHtML

[R09] 字符串比较
来源：http://blog.bbcook.cn/Article/details/gfxsrzggm.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://wap.vehdjk.com/Article/details/gqpfnoryw.sHtML

[R10] 正则匹配
来源：http://read.share.epnwcf.com/Article/details/gzbdbtfwd.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://read.share.tarul.cn/Article/details/gwzaswdse.sHtML

[R11] case 多分支
来源：http://read.share.bbcook.cn/Article/details/gdshkuziz.sHtML

case "$1" in
来源：http://www.share.yfazqb.com/Article/details/ggthbapwe.sHtML

start) echo "启动" ;;
来源：http://www.blog.sjlbkw.cn/Article/details/ghuocloqz.sHtML

stop)  echo "停止" ;;
来源：http://www.share.sjlbkw.cn/Article/details/gpygmhmlb.sHtML

*)     echo "未知命令" ;;
来源：http://www.m.share.bbcook.cn/Article/details/grdmhuibp.sHtML

esac
来源：http://wap.vehdjk.com/Article/details/gjmgcwnfo.sHtML

[R12] for 遍历文件
来源：http://www.blog.fktsv.cn/Article/details/gpmkttfug.sHtML

for f in *.txt; do echo "$f"; done
来源：http://wap.tarul.cn/Article/details/grlgibiel.sHtML

[R13] for 计数循环
来源：http://mobile.vehdjk.com/Article/details/grqokmowe.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://m.share.sjlbkw.cn/Article/details/gkelxyjct.sHtML

[R14] C 风格 for
来源：http://mobile.bbcook.cn/Article/details/ggwxsvogu.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://3g.yfazqb.com/Article/details/gsepchzln.sHtML

[R15] while 逐行读文件
来源：http://3g.tarul.cn/Article/details/gbwremjyw.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://read.share.sjlbkw.cn/Article/details/gerklfwpf.sHtML

[R16] until 等待条件
来源：http://www.blog.tarul.cn/Article/details/ghczevcbx.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://read.share.fktsv.cn/Article/details/goqtsxbgu.sHtML

[R17] 数组定义与取值
来源：http://blog.bbcook.cn/Article/details/gmmqzlxnt.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://read.share.sjlbkw.cn/Article/details/gicvcdgiy.sHtML

[R18] 遍历数组
来源：http://blog.epnwcf.com/Article/details/gsfzlpyqk.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://read.share.fktsv.cn/Article/details/gtaqwdsro.sHtML

[R19] 数组长度
来源：http://read.share.vehdjk.com/Article/details/gsmzfkvay.sHtML

echo "${#arr[@]}"
来源：http://mobile.yfazqb.com/Article/details/ggtxgqvtm.sHtML

[R20] 关联数组（字典）
来源：http://3g.tarul.cn/Article/details/giqcveela.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://wap.sjlbkw.cn/Article/details/gblqzsjla.sHtML

[R21] 字符串长度
来源：http://baike.sjlbkw.cn/Article/details/gqkcpbkkr.sHtML

echo "${#s}"
来源：http://3g.yfazqb.com/Article/details/gjkrmydrr.sHtML

[R22] 截取子串
来源：http://read.share.yfazqb.com/Article/details/gkwkhakdc.sHtML

echo "${s:0:5}"
来源：http://blog.yfazqb.com/Article/details/gsbfzqyvu.sHtML

[R23] 字符串替换
来源：http://www.m.share.fktsv.cn/Article/details/gbhotjidh.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.blog.fktsv.cn/Article/details/glonjhdly.sHtML

[R24] 大小写转换
来源：http://mobile.yfazqb.com/Article/details/gmwrafkcu.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://blog.tarul.cn/Article/details/gfhwhvxyl.sHtML

[R25] 去后缀 / 去前缀
来源：http://blog.tarul.cn/Article/details/gpixujbac.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://m.share.tarul.cn/Article/details/gmhkwpepo.sHtML

[R26] 命令替换
来源：http://read.share.sjlbkw.cn/Article/details/gnpcouvtu.sHtML

now=$(date +%F); echo "$now"
来源：http://blog.fktsv.cn/Article/details/gdddihaew.sHtML

[R27] 算术展开
来源：http://www.share.fktsv.cn/Article/details/gsuxrmmga.sHtML

echo $((1 + 2 * 3))
来源：http://blog.sjlbkw.cn/Article/details/gwvhdrwze.sHtML

[R28] 浮点运算
来源：http://blog.epnwcf.com/Article/details/ghbnixbws.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.m.share.vehdjk.com/Article/details/gfjeucntf.sHtML

[R29] 定义函数
来源：http://3g.fktsv.cn/Article/details/grpxogyna.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://read.share.yfazqb.com/Article/details/guvifjdhq.sHtML

[R30] 函数返回状态码
来源：http://read.share.sjlbkw.cn/Article/details/gvxhbcjjv.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.share.epnwcf.com/Article/details/ggwudizac.sHtML

[R31] 局部变量
来源：http://www.share.yfazqb.com/Article/details/gwloxgptw.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.blog.yfazqb.com/Article/details/gaqhhykgg.sHtML

[R32] 参数个数校验
来源：http://read.share.sjlbkw.cn/Article/details/gcbsyzhfy.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://blog.epnwcf.com/Article/details/gccjknsqh.sHtML

[R33] 捕获错误并提示行号
来源：http://m.share.vehdjk.com/Article/details/gidpkftkd.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://m.share.sjlbkw.cn/Article/details/gujnaxirb.sHtML

[R34] 退出时清理
来源：http://www.share.yfazqb.com/Article/details/gktlpaxzw.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://wap.sjlbkw.cn/Article/details/gsntqusgd.sHtML

[R35] 后台执行并等待
来源：http://mobile.sjlbkw.cn/Article/details/ghrhdhtiv.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://mobile.epnwcf.com/Article/details/gcerecjiq.sHtML

[R36] 并发执行多个任务
来源：http://www.m.share.epnwcf.com/Article/details/gtueptybn.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://mobile.tarul.cn/Article/details/gzwmawwvw.sHtML

[R37] 把输出赋给变量
来源：http://mobile.fktsv.cn/Article/details/gdveeukic.sHtML

files=$(ls -1)
来源：http://www.blog.sjlbkw.cn/Article/details/gqtiwpbrh.sHtML

[R38] 管道串联
来源：http://baike.bbcook.cn/Article/details/gvmbnejzd.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.share.sjlbkw.cn/Article/details/gcaxuaabc.sHtML

[R39] 重定向标准输出与错误
来源：http://read.share.vehdjk.com/Article/details/gayuyzbov.sHtML

cmd > out.log 2>&1
来源：http://www.share.vehdjk.com/Article/details/gdkxrhjet.sHtML

[R40] 追加写日志
来源：http://read.share.tarul.cn/Article/details/gtqtlxijt.sHtML

echo "log" >> out.log
来源：http://blog.yfazqb.com/Article/details/gkeqnfnpb.sHtML

[R41] 丢弃输出
来源：http://read.share.sjlbkw.cn/Article/details/gsgfeuzkn.sHtML

cmd >/dev/null 2>&1
来源：http://www.blog.bbcook.cn/Article/details/glqamgubx.sHtML

[R42] 输入重定向
来源：http://read.share.yfazqb.com/Article/details/gwaibbyek.sHtML

wc -l < a.txt
来源：http://read.share.sjlbkw.cn/Article/details/gwsopzjbn.sHtML

[R43] 按名字查找文件
来源：http://www.m.share.sjlbkw.cn/Article/details/ggdmsbruj.sHtML

find . -name "*.log" -type f
来源：http://www.blog.tarul.cn/Article/details/gysoupsph.sHtML

[R44] 按修改时间查找
来源：http://mobile.epnwcf.com/Article/details/ghpvgnuys.sHtML

find . -mtime -7 -type f
来源：http://www.blog.vehdjk.com/Article/details/gfevjdxzw.sHtML

[R45] 批量删除
来源：http://blog.fktsv.cn/Article/details/gysqpcnhi.sHtML

find . -name "*.tmp" -delete
来源：http://baike.fktsv.cn/Article/details/ggtaemjlj.sHtML

[R46] 递归替换文件内容
来源：http://wap.epnwcf.com/Article/details/gqcopiaqe.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://wap.vehdjk.com/Article/details/gmddbitpo.sHtML

[R47] sed 单行替换
来源：http://blog.tarul.cn/Article/details/gultcvdwt.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://blog.sjlbkw.cn/Article/details/gbmktlrle.sHtML

[R48] awk 取指定列
来源：http://wap.sjlbkw.cn/Article/details/gteypqpxc.sHtML

awk '{print $1, $3}' a.txt
来源：http://m.share.epnwcf.com/Article/details/gruyrlosc.sHtML

[R49] awk 带条件
来源：http://read.share.sjlbkw.cn/Article/details/gpiliaxad.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wap.epnwcf.com/Article/details/gtchrtdmu.sHtML

[R50] awk 求和
来源：http://www.m.share.bbcook.cn/Article/details/gjeyqifby.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://3g.sjlbkw.cn/Article/details/gqoekywfr.sHtML

[R51] 排序去重取前几
来源：http://read.share.vehdjk.com/Article/details/gkclwtytq.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.m.share.vehdjk.com/Article/details/gnflsasis.sHtML

[R52] 统计行数
来源：http://mobile.fktsv.cn/Article/details/gstvbupzr.sHtML

wc -l a.txt
来源：http://blog.tarul.cn/Article/details/gqyucnwlf.sHtML

[R53] 查看文件头与实时尾
来源：http://read.share.sjlbkw.cn/Article/details/ggpmicygg.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://m.share.vehdjk.com/Article/details/gpdzjvebt.sHtML

[R54] 比较两个文件
来源：http://www.m.share.yfazqb.com/Article/details/gacfubjrm.sHtML

diff a.txt b.txt
来源：http://m.share.bbcook.cn/Article/details/guutrpcjg.sHtML

[R55] 压缩与解压
来源：http://www.m.share.fktsv.cn/Article/details/gfpaximvr.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.share.tarul.cn/Article/details/gwtiwxvqx.sHtML

[R56] 远程拷贝
来源：http://m.share.yfazqb.com/Article/details/guvyymbnu.sHtML

scp file user@host:/path/
来源：http://mobile.bbcook.cn/Article/details/grldczvfk.sHtML

[R57] 远程执行命令
来源：http://www.share.bbcook.cn/Article/details/gbcvbhvjt.sHtML

ssh user@host 'uptime'
来源：http://baike.sjlbkw.cn/Article/details/gxmunnyyo.sHtML

[R58] 下载文件
来源：http://www.share.fktsv.cn/Article/details/gdvlrnsyw.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.m.share.bbcook.cn/Article/details/gewegsena.sHtML

[R59] 发 POST JSON
来源：http://3g.epnwcf.com/Article/details/gbjwvcglt.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://3g.yfazqb.com/Article/details/gsshmcbll.sHtML

[R60] 只看 HTTP 状态码
来源：http://m.share.bbcook.cn/Article/details/grqtzpvzq.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://blog.epnwcf.com/Article/details/gefajsths.sHtML

[R61] 磁盘占用
来源：http://wap.fktsv.cn/Article/details/gvsfllkok.sHtML

df -h;  du -sh *
来源：http://mobile.sjlbkw.cn/Article/details/gpzfngyrk.sHtML

[R62] 找最占空间的文件
来源：http://www.share.yfazqb.com/Article/details/gfvrptudr.sHtML

du -ah . | sort -rh | head -10
来源：http://wap.sjlbkw.cn/Article/details/gdpioyklf.sHtML

[R63] 内存与进程
来源：http://3g.tarul.cn/Article/details/gcftvgbnz.sHtML

free -h;  ps aux | grep nginx
来源：http://m.share.bbcook.cn/Article/details/gaqiupaba.sHtML

[R64] 结束进程
来源：http://3g.bbcook.cn/Article/details/gugbpuvqs.sHtML

kill -9 $(pgrep -f app.py)
来源：http://wap.fktsv.cn/Article/details/gkbwyymps.sHtML

[R65] 查看端口占用
来源：http://www.m.share.vehdjk.com/Article/details/grtuybreo.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://blog.bbcook.cn/Article/details/gjemxvzlp.sHtML

[R66] 定时任务
来源：http://3g.fktsv.cn/Article/details/gahxdcehb.sHtML

crontab -e;  crontab -l
来源：http://www.blog.tarul.cn/Article/details/gzyceeayl.sHtML

[R67] 生成随机十六进制串
来源：http://read.share.fktsv.cn/Article/details/gdhvhouse.sHtML

openssl rand -hex 16
来源：http://3g.epnwcf.com/Article/details/gvhssdyru.sHtML

[R68] 计算文件校验值
来源：http://www.m.share.fktsv.cn/Article/details/gaqdeaqnl.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.blog.fktsv.cn/Article/details/gczohxxql.sHtML

[R69] 生成随机密码
来源：http://wap.tarul.cn/Article/details/gvmbvaxzf.sHtML

head -c 16 /dev/urandom | base64
来源：http://3g.sjlbkw.cn/Article/details/ggfddgicn.sHtML

[R70] 时间戳与互转
来源：http://www.share.yfazqb.com/Article/details/gglwkraan.sHtML

date +%s;  date -d @1700000000
来源：http://mobile.sjlbkw.cn/Article/details/gwgudzyzg.sHtML

[R71] 日期格式化
来源：http://read.share.yfazqb.com/Article/details/gduiogcwr.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://m.share.tarul.cn/Article/details/gkzlavmtg.sHtML

[R72] 等待端口就绪
来源：http://m.share.fktsv.cn/Article/details/gmpdxjifw.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://m.share.fktsv.cn/Article/details/gwwzagmwa.sHtML

[R73] 分割大日志
来源：http://www.share.fktsv.cn/Article/details/glsonnxzm.sHtML

split -l 1000 big.log part_
来源：http://www.share.tarul.cn/Article/details/giugnjoyq.sHtML

[R74] 批量重命名
来源：http://www.m.share.vehdjk.com/Article/details/gtjywpyxm.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.blog.epnwcf.com/Article/details/ggvqakiqz.sHtML

[R75] 导出环境变量
来源：http://blog.yfazqb.com/Article/details/gfbslujzj.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://3g.tarul.cn/Article/details/gyloqhidb.sHtML

[R76] 使用临时文件
来源：http://www.share.epnwcf.com/Article/details/gpfqmuxsb.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://read.share.tarul.cn/Article/details/gzhadnwey.sHtML

[R77] 读取用户输入
来源：http://3g.fktsv.cn/Article/details/gpbnwhlqx.sHtML

read -rp "请输入: " ans
来源：http://www.blog.sjlbkw.cn/Article/details/gasfqbgow.sHtML

[R78] 交互式菜单
来源：http://m.share.epnwcf.com/Article/details/gwvobbwrj.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.m.share.sjlbkw.cn/Article/details/gfcrqvaco.sHtML

[R79] 解析命令行选项
来源：http://read.share.vehdjk.com/Article/details/gaqdgrlxv.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.blog.tarul.cn/Article/details/gwiclprof.sHtML

[R80] 查看脚本执行耗时
来源：http://baike.yfazqb.com/Article/details/grkzapajk.sHtML

time ./run.sh
来源：http://wap.vehdjk.com/Article/details/ggwxxyann.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/gvyjdkhpa.sHtML

S. C / C++ 专题
来源：http://www.share.yfazqb.com/Article/details/gonveucpw.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/gcwzagqpw.sHtML

[S01] C：Hello World
来源：http://read.share.fktsv.cn/Article/details/gqynzgbxn.sHtML

#include <stdio.h>
来源：http://3g.tarul.cn/Article/details/ghlcbjkwh.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://3g.epnwcf.com/Article/details/gymgfvyah.sHtML

[S02] C：变量与格式化输出
来源：http://m.share.tarul.cn/Article/details/gjprqtxvu.sHtML

int a = 10; printf("%d\n", a);
来源：http://read.share.epnwcf.com/Article/details/gaixwejnj.sHtML

[S03] C：读入整数
来源：http://blog.vehdjk.com/Article/details/gnuctjfwq.sHtML

int x; scanf("%d", &x);
来源：http://mobile.fktsv.cn/Article/details/gqppmpfhg.sHtML

[S04] C：字符串复制
来源：http://blog.epnwcf.com/Article/details/gonpunxdq.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.m.share.bbcook.cn/Article/details/gumhbbxad.sHtML

[S05] C：字符串长度
来源：http://blog.epnwcf.com/Article/details/gvkxjgnvi.sHtML

strlen(s)
来源：http://www.blog.vehdjk.com/Article/details/gkxvmshnm.sHtML

[S06] C：字符串比较
来源：http://3g.vehdjk.com/Article/details/gbjldimob.sHtML

strcmp(a, b) == 0
来源：http://wap.vehdjk.com/Article/details/gcpyuwvan.sHtML

[S07] C：数组遍历求和
来源：http://www.blog.fktsv.cn/Article/details/grjeglndb.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://3g.epnwcf.com/Article/details/gbldycmwb.sHtML

[S08] C：动态内存分配与释放
来源：http://blog.yfazqb.com/Article/details/gkervkpyh.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.blog.sjlbkw.cn/Article/details/gvpkkekjy.sHtML

[S09] C：结构体定义与初始化
来源：http://baike.bbcook.cn/Article/details/gsltakfwa.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mobile.vehdjk.com/Article/details/gavyawszc.sHtML

[S10] C：指针与解引用
来源：http://baike.yfazqb.com/Article/details/gixvonirw.sHtML

int *p = &a;  *p = 5;
来源：http://www.blog.fktsv.cn/Article/details/guzhsiryj.sHtML

[S11] C：逐行读文件
来源：http://m.share.yfazqb.com/Article/details/ghysodvtz.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://baike.sjlbkw.cn/Article/details/gaclxoklv.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://read.share.bbcook.cn/Article/details/gpfnzrusw.sHtML

fclose(f);
来源：http://read.share.vehdjk.com/Article/details/gxzqbkqdq.sHtML

[S12] C：写文件
来源：http://blog.fktsv.cn/Article/details/gdmmfguet.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://blog.tarul.cn/Article/details/gglipjfbe.sHtML

[S13] C：宏定义
来源：http://m.share.sjlbkw.cn/Article/details/gzrsvydki.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://blog.epnwcf.com/Article/details/gkeqztgqn.sHtML

[S14] C：枚举
来源：http://mobile.sjlbkw.cn/Article/details/gxeixazfh.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.share.yfazqb.com/Article/details/glbndgymx.sHtML

[S15] C：类型转换
来源：http://wap.fktsv.cn/Article/details/gzlhtxbfk.sHtML

(double) a / b
来源：http://blog.bbcook.cn/Article/details/gbrhwdmdg.sHtML

[S16] C：位操作置位
来源：http://www.blog.vehdjk.com/Article/details/gwaybbgfe.sHtML

x |= (1 << 3);
来源：http://wap.yfazqb.com/Article/details/gihsstdfj.sHtML

[S17] C：安全拼接字符串
来源：http://read.share.tarul.cn/Article/details/gfcrazqaa.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://baike.sjlbkw.cn/Article/details/gftajawqe.sHtML

[S18] C：命令行参数
来源：http://blog.tarul.cn/Article/details/grrzvfbsf.sHtML

int main(int argc, char **argv)
来源：http://www.blog.tarul.cn/Article/details/grqafouyu.sHtML

[S19] C：快速排序
来源：http://wap.vehdjk.com/Article/details/genofghiy.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://wap.epnwcf.com/Article/details/gwpqcumwl.sHtML

[S20] C：二分查找
来源：http://www.share.bbcook.cn/Article/details/gqksfjjmn.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://baike.yfazqb.com/Article/details/geshfhrsa.sHtML

[S21] C：字符类别判断
来源：http://mobile.sjlbkw.cn/Article/details/grvovuicm.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mobile.sjlbkw.cn/Article/details/glekznskn.sHtML

[S22] C：字符串转数字
来源：http://www.share.vehdjk.com/Article/details/gtwxlhwvi.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://read.share.bbcook.cn/Article/details/gzsqcyixl.sHtML

[S23] C：随机数
来源：http://m.share.tarul.cn/Article/details/gkcczfznc.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://read.share.sjlbkw.cn/Article/details/gfqaxqejq.sHtML

[S24] C：获取本地时间
来源：http://www.blog.bbcook.cn/Article/details/ghwqbhsph.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://read.share.vehdjk.com/Article/details/gflyxairu.sHtML

[S25] C：内存拷贝
来源：http://www.blog.sjlbkw.cn/Article/details/gvmvaflfo.sHtML

memcpy(dst, src, n);
来源：http://mobile.bbcook.cn/Article/details/glqjheuek.sHtML

[S26] C：内存清零
来源：http://www.share.yfazqb.com/Article/details/gmvnixokf.sHtML

memset(a, 0, sizeof a);
来源：http://www.blog.fktsv.cn/Article/details/gqbpwcbzu.sHtML

[S27] C：定义常量
来源：http://m.share.yfazqb.com/Article/details/gbawirjju.sHtML

const double PI = 3.14159;
来源：http://baike.yfazqb.com/Article/details/gpvmnmqnb.sHtML

[S28] C：静态变量
来源：http://wap.fktsv.cn/Article/details/gndweljwz.sHtML

static int counter = 0;
来源：http://baike.yfazqb.com/Article/details/gfiezxjeh.sHtML

[S29] C：变参函数
来源：http://wap.fktsv.cn/Article/details/gqdtoitrk.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.blog.vehdjk.com/Article/details/gmxqjgdpa.sHtML

[S30] C：头文件保护
来源：http://blog.bbcook.cn/Article/details/gkvtikhpt.sHtML

#ifndef X_H
来源：http://baike.sjlbkw.cn/Article/details/gkarjuavt.sHtML

#define X_H
来源：http://blog.epnwcf.com/Article/details/grrmsnwwc.sHtML

#endif
来源：http://m.share.yfazqb.com/Article/details/gsumkkbsa.sHtML

[S31] C++：Hello World
来源：http://baike.sjlbkw.cn/Article/details/gnbixvpdg.sHtML

#include <iostream>
来源：http://www.share.fktsv.cn/Article/details/grwdjdcnj.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://blog.vehdjk.com/Article/details/gdldrfxpm.sHtML

[S32] C++：字符串
来源：http://baike.bbcook.cn/Article/details/gmxbynbpb.sHtML

std::string s = "hi";  s += "!";
来源：http://3g.vehdjk.com/Article/details/gzrigujwx.sHtML

[S33] C++：vector 增删
来源：http://mobile.bbcook.cn/Article/details/gnickpznl.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://m.share.yfazqb.com/Article/details/gkbpokfob.sHtML

[S34] C++：遍历 vector
来源：http://www.share.tarul.cn/Article/details/gjjmfjubs.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.m.share.bbcook.cn/Article/details/gwnfhbgvg.sHtML

[S35] C++：map
来源：http://m.share.fktsv.cn/Article/details/golycgjoi.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.tarul.cn/Article/details/gogcxqwzu.sHtML

[S36] C++：unordered_map
来源：http://blog.sjlbkw.cn/Article/details/gndimhthc.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://3g.vehdjk.com/Article/details/gppyrtbju.sHtML

[S37] C++：set
来源：http://baike.sjlbkw.cn/Article/details/gwwgashwx.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://m.share.yfazqb.com/Article/details/geigayrpj.sHtML

[S38] C++：排序
来源：http://wap.fktsv.cn/Article/details/gpzxghelm.sHtML

std::sort(v.begin(), v.end());
来源：http://wap.yfazqb.com/Article/details/gleicaqlk.sHtML

[S39] C++：自定义比较器排序
来源：http://read.share.yfazqb.com/Article/details/gtrvhtclq.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://blog.tarul.cn/Article/details/gdhdymant.sHtML

[S40] C++：查找元素
来源：http://read.share.bbcook.cn/Article/details/ghtezbsse.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.m.share.yfazqb.com/Article/details/gsjzqdbto.sHtML

[S41] C++：类与构造函数
来源：http://3g.epnwcf.com/Article/details/gkivmtead.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://wap.vehdjk.com/Article/details/ghvqhxjcm.sHtML

[S42] C++：继承与虚函数
来源：http://m.share.sjlbkw.cn/Article/details/guxzivqas.sHtML

class B : public Base { public: void f() override {} };
来源：http://wap.fktsv.cn/Article/details/gidyphzbp.sHtML

[S43] C++：智能指针
来源：http://www.m.share.vehdjk.com/Article/details/gkoripxmd.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.blog.epnwcf.com/Article/details/goyiobixd.sHtML

[S44] C++：引用传参
来源：http://www.blog.tarul.cn/Article/details/gqwmdrguc.sHtML

void inc(int &x) { ++x; }
来源：http://www.m.share.fktsv.cn/Article/details/gzbjffjjq.sHtML

[S45] C++：lambda
来源：http://baike.vehdjk.com/Article/details/gcliekgei.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.m.share.vehdjk.com/Article/details/gpfwoiqrr.sHtML

[S46] C++：函数模板
来源：http://www.blog.tarul.cn/Article/details/gdzldaapn.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://wap.vehdjk.com/Article/details/gntefldty.sHtML

[S47] C++：结构化绑定遍历
来源：http://baike.yfazqb.com/Article/details/gukxeyekc.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.m.share.vehdjk.com/Article/details/galsobrsw.sHtML

[S48] C++：逐行读文件
来源：http://m.share.epnwcf.com/Article/details/grdjkeinb.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.m.share.yfazqb.com/Article/details/gencnyuyv.sHtML

while (std::getline(in, line)) { }
来源：http://read.share.fktsv.cn/Article/details/grgczuwez.sHtML

[S49] C++：写文件
来源：http://read.share.sjlbkw.cn/Article/details/gvxpaqiic.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.blog.epnwcf.com/Article/details/gcifgiqtx.sHtML

[S50] C++：格式化数字
来源：http://www.m.share.tarul.cn/Article/details/gjleosjwh.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://baike.sjlbkw.cn/Article/details/gqskkfomz.sHtML

[S51] C++：显式类型转换
来源：http://wap.epnwcf.com/Article/details/gjkrhlrny.sHtML

static_cast<double>(a) / b
来源：http://blog.bbcook.cn/Article/details/gauugbnjd.sHtML

[S52] C++：const 与 noexcept
来源：http://blog.vehdjk.com/Article/details/glelvsskp.sHtML

int size() const noexcept { return n_; }
来源：http://www.share.epnwcf.com/Article/details/gouakfepo.sHtML

[S53] C++：移动语义
来源：http://wap.sjlbkw.cn/Article/details/glozxqptw.sHtML

std::vector<int> w = std::move(v);
来源：http://m.share.epnwcf.com/Article/details/gnsontkph.sHtML

[S54] C++：异常处理
来源：http://mobile.tarul.cn/Article/details/gcnnhptop.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://wap.vehdjk.com/Article/details/gssamkfep.sHtML

[S55] C++：结构化绑定
来源：http://www.blog.epnwcf.com/Article/details/gxnyuywvm.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://wap.yfazqb.com/Article/details/gbcqepmcn.sHtML

[S56] C++：optional
来源：http://m.share.fktsv.cn/Article/details/gjckdrvaz.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://mobile.tarul.cn/Article/details/govcysigs.sHtML

[S57] C++：编译期常量
来源：http://blog.tarul.cn/Article/details/gshjorizz.sHtML

constexpr int N = 10;
来源：http://mobile.fktsv.cn/Article/details/gsobapods.sHtML

[S58] C++：命名空间
来源：http://blog.bbcook.cn/Article/details/gifktcbgm.sHtML

namespace ns { int f() { return 1; } }
来源：http://read.share.epnwcf.com/Article/details/gcxxhwdds.sHtML

[S59] C++：静态断言
来源：http://baike.tarul.cn/Article/details/gwwwqkibj.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.blog.yfazqb.com/Article/details/gifrxkfdo.sHtML

[S60] C++：遍历并删除元素
来源：http://wap.bbcook.cn/Article/details/gucqmmzsv.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.share.sjlbkw.cn/Article/details/gxoykheoa.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/gotphvhme.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.fktsv.cn/Article/details/gvkfptxoi.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/gpzpzbauz.sHtML

[T01] Kotlin：Hello World
来源：http://baike.vehdjk.com/Article/details/ganyjvpen.sHtML

println("Hello")
来源：http://mobile.bbcook.cn/Article/details/gfilxkaeu.sHtML

[T02] Kotlin：变量
来源：http://m.share.sjlbkw.cn/Article/details/gykyyonew.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.m.share.bbcook.cn/Article/details/gezmxpfbw.sHtML

[T03] Kotlin：字符串模板
来源：http://m.share.epnwcf.com/Article/details/gnlarytob.sHtML

"值: $b"
来源：http://baike.vehdjk.com/Article/details/gpskwwpgq.sHtML

[T04] Kotlin：空安全
来源：http://mobile.yfazqb.com/Article/details/gquuhnmdb.sHtML

val n: String? = null;  n?.length
来源：http://mobile.bbcook.cn/Article/details/gyyuzfkjd.sHtML

[T05] Kotlin：when 表达式
来源：http://blog.yfazqb.com/Article/details/guhkedbtv.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://mobile.fktsv.cn/Article/details/gjuiiaxbk.sHtML

[T06] Kotlin：集合映射
来源：http://m.share.fktsv.cn/Article/details/ggwxuynsa.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://baike.sjlbkw.cn/Article/details/ghphuaple.sHtML

[T07] Kotlin：集合过滤
来源：http://www.m.share.fktsv.cn/Article/details/gdzpioblx.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://wap.epnwcf.com/Article/details/gioeffpnz.sHtML

[T08] Kotlin：数据类
来源：http://read.share.bbcook.cn/Article/details/gehxmluqn.sHtML

data class User(val name: String, val age: Int)
来源：http://www.share.sjlbkw.cn/Article/details/gxyychuxr.sHtML


<!-- 参考信息 -->