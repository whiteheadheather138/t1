代发 wailian999

[Q76] 按天统计
来源：http://xkd.zhongyouzk.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://zdx.bbcook.cn

[Q77] 时间加减
来源：http://lko.wangdashe.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://wbc.jinqigufen.top

[Q78] 当前时间
来源：http://isq.iojbl.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://htp.zdbjq.cn

[Q79] 字符串拼接
来源：http://kjm.jqgfzy.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://lwe.jqgfzy.top

[Q80] 字符串截取
来源：http://lch.quarkkingdee.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://lkt.cashguo.top

[Q81] 字符串替换
来源：http://cev.yangfankeji.com

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://pds.sweek.top

[Q82] 字符长度与字节长度
来源：http://ksw.sysykeji.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hgq.fanxiaobao.xyz

[Q83] 大小写转换
来源：http://omj.yonumen.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://gml.cheryme.top

[Q84] 去除首尾空格
来源：http://kmi.jinqigufen.top

SELECT TRIM(name) FROM users;
来源：http://rhn.hesvh.cn

[Q85] 数值取整
来源：http://sdk.jinyuanbaomall.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://vdq.sweek.top

[Q86] 读取 JSON 字段
来源：http://oct.andypj.xyz

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://vpw.yangfankeji.com

[Q87] JSON 字段做条件
来源：http://tfm.fanxiaobao.xyz

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://sil.shzxlz.cn

[Q88] 行转列（条件聚合）
来源：http://rba.wangshuangyany.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://mjb.aizwys.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://ohl.xuetiantiany.cn

[Q89] 判断表是否存在
来源：http://fio.nwbrower.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hmf.fzhhl.top

[Q90] 生成序号列
来源：http://klv.redwolf501.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://abs.sweek.top

================================================================================
来源：http://kth.hesvh.cn

R. Bash 专题
来源：http://mpy.jqgufenzy.top

================================================================================
来源：http://ntj.gzhubu.top

[R01] shebang 与严格模式
来源：http://asu.birdmap.top

#!/usr/bin/env bash
来源：http://fwm.bbcook.cn

set -euo pipefail
来源：http://lec.yfazqb.com

[R02] 变量赋值与使用
来源：http://cbm.shanyushiyangkeji.top

name="Tom"; echo "$name"
来源：http://zga.hfpthk.cn

[R03] 只读变量
来源：http://hnk.gotoacloud.top

readonly PI=3.14
来源：http://svu.aibaodan.cn

[R04] 位置参数
来源：http://jcb.hesvh.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://srj.shuidangran.top

[R05] 参数默认值
来源：http://orj.yfazqb.com

name="${1:-default}"
来源：http://rds.zhoulong.xyz

[R06] 判断命令是否存在
来源：http://ikr.andypj.xyz

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://iyl.wangdashe.top

[R07] if 判断文件
来源：http://tfq.sxryk.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hix.quarkkingdee.top

[R08] 数值比较
来源：http://vso.ywan-chungtsiang.top

if (( a > b )); then echo "a 更大"; fi
来源：http://vdk.bbcook.cn

[R09] 字符串比较
来源：http://zaa.chenjidiqi.icu

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://baw.fzhhl.top

[R10] 正则匹配
来源：http://llr.zycfv.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://ukp.tanke756.top

[R11] case 多分支
来源：http://sse.daria6918.cn

case "$1" in
来源：http://fyq.xinyue.icu

start) echo "启动" ;;
来源：http://fvh.yj20258888.top

stop)  echo "停止" ;;
来源：http://pje.hesvh.cn

*)     echo "未知命令" ;;
来源：http://svz.jqgfzy.top

esac
来源：http://jnw.daria6918.cn

[R12] for 遍历文件
来源：http://oan.bbcook.cn

for f in *.txt; do echo "$f"; done
来源：http://pcd.shuidangran.top

[R13] for 计数循环
来源：http://enf.pycfn.com

for i in {1..10}; do echo "$i"; done
来源：http://kad.ywan-chungtsiang.top

[R14] C 风格 for
来源：http://nnd.zhongyouzk.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://qgy.wangdashe.top

[R15] while 逐行读文件
来源：http://yph.shuidangran.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://eow.snrcjt.cn

[R16] until 等待条件
来源：http://dix.zdqjudy.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://iiy.svipenyu.cn

[R17] 数组定义与取值
来源：http://avt.gaohongyu789.top

arr=(a b c); echo "${arr[0]}"
来源：http://sed.jyoumei.cn

[R18] 遍历数组
来源：http://pvp.bbcook.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://lgs.yueranfly.top

[R19] 数组长度
来源：http://bzf.jqgufenzy.top

echo "${#arr[@]}"
来源：http://niz.smart0.xyz

[R20] 关联数组（字典）
来源：http://ftx.gaohongyu789.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://rbd.sxryk.cn

[R21] 字符串长度
来源：http://nqj.hnqzz.top

echo "${#s}"
来源：http://pte.ppjwa.cn

[R22] 截取子串
来源：http://ohk.jianghu66.top

echo "${s:0:5}"
来源：http://pzf.pycfn.com

[R23] 字符串替换
来源：http://xkg.epnwcf.com

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://wlb.quarkkingdee.top

[R24] 大小写转换
来源：http://yqr.ybcxt.top

echo "${s^^}"; echo "${s,,}"
来源：http://rod.chenlongwang.top

[R25] 去后缀 / 去前缀
来源：http://kfy.yueranfly.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://fge.snrcjt.cn

[R26] 命令替换
来源：http://dng.shanyushiyangkeji.top

now=$(date +%F); echo "$now"
来源：http://nxl.sufxvd.cn

[R27] 算术展开
来源：http://hci.andypj.xyz

echo $((1 + 2 * 3))
来源：http://zke.sufxvd.cn

[R28] 浮点运算
来源：http://boa.zhengqikj.top

echo "scale=2; 10/3" | bc
来源：http://ahy.ywan-chungtsiang.top

[R29] 定义函数
来源：http://etv.hnqzz.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://dlq.sxryk.cn

[R30] 函数返回状态码
来源：http://axy.kuanghao11.cn

f() { return 0; }; f || echo "失败了"
来源：http://izv.bjfxy.top

[R31] 局部变量
来源：http://alh.9152youxi.cn

f() { local x=1; echo "$x"; }
来源：http://ego.mhx1999.top

[R32] 参数个数校验
来源：http://ltc.yuxming.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://lgb.nanxuanxn.top

[R33] 捕获错误并提示行号
来源：http://dka.yj202588.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://jqw.vqdsnc.cn

[R34] 退出时清理
来源：http://udg.xziqi.cn

trap 'rm -f "$tmp"' EXIT
来源：http://rux.yj20258888.top

[R35] 后台执行并等待
来源：http://ftr.vqdsnc.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://kwc.hammf.cn

[R36] 并发执行多个任务
来源：http://wkc.sweek.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://zna.jqgufenzy.top

[R37] 把输出赋给变量
来源：http://fdx.jinqigufen.top

files=$(ls -1)
来源：http://iqp.ydjk.org.cn

[R38] 管道串联
来源：http://ruy.hnqzz.top

cat a.txt | grep -i error | wc -l
来源：http://xiz.shanyushiyangkeji.top

[R39] 重定向标准输出与错误
来源：http://gmm.ydzc1.top

cmd > out.log 2>&1
来源：http://rqf.chenzaomai.com

[R40] 追加写日志
来源：http://jvv.tian-w.cn

echo "log" >> out.log
来源：http://mtg.redwolf501.top

[R41] 丢弃输出
来源：http://wzx.pengpengdd.cyou

cmd >/dev/null 2>&1
来源：http://rvn.jinghuilouyu.cn

[R42] 输入重定向
来源：http://maj.xuetiantiany.cn

wc -l < a.txt
来源：http://jru.tian-w.cn

[R43] 按名字查找文件
来源：http://fca.yanxiufei.cn

find . -name "*.log" -type f
来源：http://uyu.zhengqikj.top

[R44] 按修改时间查找
来源：http://epd.yonumen.top

find . -mtime -7 -type f
来源：http://myh.zdqjudy.top

[R45] 批量删除
来源：http://pfm.dashuyun.cn

find . -name "*.tmp" -delete
来源：http://srj.jinqigufen.top

[R46] 递归替换文件内容
来源：http://uop.yonumen.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://dop.fktsv.cn

[R47] sed 单行替换
来源：http://wsi.jqgufenzy.top

sed -i 's/foo/bar/g' a.txt
来源：http://gyg.snrcjt.cn

[R48] awk 取指定列
来源：http://nor.sxryk.cn

awk '{print $1, $3}' a.txt
来源：http://ohr.xylfe.cn

[R49] awk 带条件
来源：http://ozi.yfazqb.com

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://cmt.shanyushiyangtech.top

[R50] awk 求和
来源：http://qgu.dashuyun.cn

awk '{s += $2} END {print s}' a.txt
来源：http://fil.ppjwa.cn

[R51] 排序去重取前几
来源：http://ikl.fzhhl.top

sort a.txt | uniq -c | sort -rn | head
来源：http://htu.xziqi.cn

[R52] 统计行数
来源：http://rsw.chenlongwang.top

wc -l a.txt
来源：http://zcl.ydzc1.top

[R53] 查看文件头与实时尾
来源：http://xmp.zhixingplan.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://oin.daria6918.cn

[R54] 比较两个文件
来源：http://kau.quarkkingdee.top

diff a.txt b.txt
来源：http://tgc.dashuyun.cn

[R55] 压缩与解压
来源：http://hgw.yueranfly.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://bot.shzxlz.cn

[R56] 远程拷贝
来源：http://vtc.ctjpmb.com

scp file user@host:/path/
来源：http://rhf.nanxinkj.top

[R57] 远程执行命令
来源：http://jyv.fzhhl.top

ssh user@host 'uptime'
来源：http://yna.jyoumei.cn

[R58] 下载文件
来源：http://isg.yj20258888.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://xzf.jinqigfzy.top

[R59] 发 POST JSON
来源：http://sen.jinyuanbaomall.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://cos.zhengqikj.top

[R60] 只看 HTTP 状态码
来源：http://khj.xylfe.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://gnr.snrcjt.cn

[R61] 磁盘占用
来源：http://weh.daria6918.cn

df -h;  du -sh *
来源：http://hek.shzxlz.cn

[R62] 找最占空间的文件
来源：http://gab.yueranfly.top

du -ah . | sort -rh | head -10
来源：http://xrb.ppjwa.cn

[R63] 内存与进程
来源：http://sbh.ivvv.top

free -h;  ps aux | grep nginx
来源：http://mgv.ivvv.top

[R64] 结束进程
来源：http://dnr.shuidangran.top

kill -9 $(pgrep -f app.py)
来源：http://ikc.ctjpmb.com

[R65] 查看端口占用
来源：http://vjv.jinyuanbaomall.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://dep.52xcode.cn

[R66] 定时任务
来源：http://obh.zhijiandao.cn

crontab -e;  crontab -l
来源：http://cqu.chenjidiqi.icu

[R67] 生成随机十六进制串
来源：http://tww.xinyue.icu

openssl rand -hex 16
来源：http://poy.aibaodan.cn

[R68] 计算文件校验值
来源：http://gvk.dashuyun.cn

sha256sum a.txt;  md5sum a.txt
来源：http://ewl.shanyushiyangtech.top

[R69] 生成随机密码
来源：http://kwb.hnqzz.top

head -c 16 /dev/urandom | base64
来源：http://pjf.0kj1m.cn

[R70] 时间戳与互转
来源：http://fsf.fengsongda.top

date +%s;  date -d @1700000000
来源：http://wvc.tian-w.cn

[R71] 日期格式化
来源：http://gca.c1oappe.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://yqn.tanke756.top

[R72] 等待端口就绪
来源：http://mqr.aibaodan.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://gil.shangyingyoupin.top

[R73] 分割大日志
来源：http://rnl.cqqwz.cn

split -l 1000 big.log part_
来源：http://zuh.shuidangran.top

[R74] 批量重命名
来源：http://drq.hnqzz.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://lfn.vehdjk.com

[R75] 导出环境变量
来源：http://ucw.yonumen.top

export PATH="$HOME/bin:$PATH"
来源：http://pvh.cqqwz.cn

[R76] 使用临时文件
来源：http://fef.guannengcc.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://vqr.shuidangran.top

[R77] 读取用户输入
来源：http://dna.shangyingyoupin.top

read -rp "请输入: " ans
来源：http://wjm.jlsjyb.cn

[R78] 交互式菜单
来源：http://axd.jinyuanbaomall.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://lrg.vqdsnc.cn

[R79] 解析命令行选项
来源：http://kfj.pengpengdd.cyou

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://frq.ehwqpu.com

[R80] 查看脚本执行耗时
来源：http://vyo.ydjk.org.cn

time ./run.sh
来源：http://asn.hongshengwenyu.top

================================================================================
来源：http://qre.yfazqb.com

S. C / C++ 专题
来源：http://ihi.ivvv.top

================================================================================
来源：http://lrw.zhongyouzk.top

[S01] C：Hello World
来源：http://amc.shzxlz.cn

#include <stdio.h>
来源：http://kbm.zhongyouzk.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://dcm.tanke756.top

[S02] C：变量与格式化输出
来源：http://btt.sysykeji.top

int a = 10; printf("%d\n", a);
来源：http://sdt.shuidangran.top

[S03] C：读入整数
来源：http://xep.yvedp.cn

int x; scanf("%d", &x);
来源：http://clc.yangfankeji.com

[S04] C：字符串复制
来源：http://hjz.hysaishi.cn

char dst[32]; strcpy(dst, "hi");
来源：http://idg.guowangkeji.top

[S05] C：字符串长度
来源：http://tln.hnqzz.top

strlen(s)
来源：http://nkm.jiagoushi.top

[S06] C：字符串比较
来源：http://hhd.ctjpmb.com

strcmp(a, b) == 0
来源：http://jyy.shzxlz.cn

[S07] C：数组遍历求和
来源：http://rtl.jiagoushi.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://wji.cqqwz.cn

[S08] C：动态内存分配与释放
来源：http://efi.tanke756.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://ify.zdqjudy.top

[S09] C：结构体定义与初始化
来源：http://ddg.yuxming.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://wuw.pengpengdd.cyou

[S10] C：指针与解引用
来源：http://djv.chenlongwang.top

int *p = &a;  *p = 5;
来源：http://tjz.zhoulong.xyz

[S11] C：逐行读文件
来源：http://ezb.iojbl.cn

FILE *f = fopen("a.txt", "r");
来源：http://uko.zdbjq.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://vlp.yanxiufei.cn

fclose(f);
来源：http://dzw.ctjpmb.com

[S12] C：写文件
来源：http://ary.hnxiangtu.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://aho.ivvv.top

[S13] C：宏定义
来源：http://zcw.nwbrower.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wpn.fktsv.cn

[S14] C：枚举
来源：http://bem.iojbl.cn

enum Color { RED, GREEN, BLUE };
来源：http://ehx.bbcook.cn

[S15] C：类型转换
来源：http://biw.gzhubu.top

(double) a / b
来源：http://qdd.hongshengwenyu.top

[S16] C：位操作置位
来源：http://rwf.hywenlv.cn

x |= (1 << 3);
来源：http://bur.gaohongyu789.top

[S17] C：安全拼接字符串
来源：http://kmd.gogol.net.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wpk.ywan-chungtsiang.top

[S18] C：命令行参数
来源：http://aqw.snrcjt.cn

int main(int argc, char **argv)
来源：http://msw.chenlongwang.top

[S19] C：快速排序
来源：http://uam.dianchejie.cn

qsort(a, n, sizeof(int), cmp);
来源：http://gzm.redwolf501.top

[S20] C：二分查找
来源：http://vej.hnxiangtu.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://uie.gzhubu.top

[S21] C：字符类别判断
来源：http://hcu.sxryk.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://uyt.fengsongda.top

[S22] C：字符串转数字
来源：http://guw.gaohongyu789.top

atoi("42");  strtod("3.14", NULL);
来源：http://toh.guowangkeji.top

[S23] C：随机数
来源：http://iox.cashguo.top

srand(time(NULL));  int r = rand() % 100;
来源：http://hct.haohaochexian.top

[S24] C：获取本地时间
来源：http://rvd.hammf.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://ruu.snrcjt.cn

[S25] C：内存拷贝
来源：http://fcf.jinyuanbaomall.cn

memcpy(dst, src, n);
来源：http://hew.sufxvd.cn

[S26] C：内存清零
来源：http://cji.hesvh.cn

memset(a, 0, sizeof a);
来源：http://jvl.hnqzz.top

[S27] C：定义常量
来源：http://zxe.guowangkeji.top

const double PI = 3.14159;
来源：http://apz.hcnkem.com

[S28] C：静态变量
来源：http://msc.hfpthk.cn

static int counter = 0;
来源：http://hja.hesvh.cn

[S29] C：变参函数
来源：http://zwd.ivvv.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://vql.birdmap.top

[S30] C：头文件保护
来源：http://qov.bbcook.cn

#ifndef X_H
来源：http://mxr.jiagoushi.top

#define X_H
来源：http://bxo.redwolf501.top

#endif
来源：http://hwy.tanke756.top

[S31] C++：Hello World
来源：http://xge.iojbl.cn

#include <iostream>
来源：http://dmq.daria6918.cn

int main() { std::cout << "Hello\n"; }
来源：http://mvw.yj20258.top

[S32] C++：字符串
来源：http://hvb.bbcook.cn

std::string s = "hi";  s += "!";
来源：http://vyd.ydzc1.top

[S33] C++：vector 增删
来源：http://bmk.jianghu66.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://gjb.bbcook.cn

[S34] C++：遍历 vector
来源：http://csh.hesvh.cn

for (auto &x : v) { std::cout << x; }
来源：http://vbi.quarkkingdee.top

[S35] C++：map
来源：http://zrr.shangyingyoupin.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://pfp.pycfn.com

[S36] C++：unordered_map
来源：http://isj.zhaomingkeji.xyz

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wat.chenjidiqi.icu

[S37] C++：set
来源：http://rqs.cdnleiting.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://kkd.zhijiandao.cn

[S38] C++：排序
来源：http://inf.shanyushiyangtech.top

std::sort(v.begin(), v.end());
来源：http://mod.bbcook.cn

[S39] C++：自定义比较器排序
来源：http://mdc.hongshengwenyu.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://lxj.jyoumei.cn

[S40] C++：查找元素
来源：http://qfw.xuetiantiany.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://edh.zhijiandao.cn

[S41] C++：类与构造函数
来源：http://ftb.xinyue.icu

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://mxu.fzhhl.top

[S42] C++：继承与虚函数
来源：http://gah.haohaochexian.top

class B : public Base { public: void f() override {} };
来源：http://zov.cdnleiting.top

[S43] C++：智能指针
来源：http://msr.epnwcf.com

auto p = std::make_unique<int>(5);
来源：http://gnp.sweek.top

[S44] C++：引用传参
来源：http://zlj.jinyuanbaomall.cn

void inc(int &x) { ++x; }
来源：http://zzc.xuetiantiany.cn

[S45] C++：lambda
来源：http://vzq.fanxiaobao.xyz

auto add = [](int a, int b) { return a + b; };
来源：http://kos.sweek.top

[S46] C++：函数模板
来源：http://ses.yueranfly.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://boj.shzxlz.cn


<!-- 参考信息 -->