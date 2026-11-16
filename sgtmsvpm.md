代发 wailian999

SHOW INDEX FROM users;
来源：http://pzx.jianghu66.top

[Q73] 查看表状态
来源：http://smj.aizwys.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://wel.haohaochexian.top

[Q74] 强制使用索引
来源：http://vhu.zycfv.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://unp.chenlongwang.top

[Q75] 日期格式化
来源：http://ico.bbcook.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://iej.redwolf501.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://yqf.cdnleiting.top

[Q76] 按天统计
来源：http://pgy.cucudq.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://zpi.snrcjt.cn

[Q77] 时间加减
来源：http://fek.tian-w.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://mvz.fengsongda.top

[Q78] 当前时间
来源：http://fqr.wangdashe.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://abj.hnqzz.top

[Q79] 字符串拼接
来源：http://eqv.tarul.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://thc.yfazqb.com

[Q80] 字符串截取
来源：http://mne.sweek.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://ylb.guannengcc.top

[Q81] 字符串替换
来源：http://dvk.hnqzz.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://cll.yueranfly.top

[Q82] 字符长度与字节长度
来源：http://ohv.jinqigufen.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://ktj.ehwqpu.com

[Q83] 大小写转换
来源：http://ovr.daxiang520.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://ufu.hysaishi.cn

[Q84] 去除首尾空格
来源：http://zth.dianchejie.cn

SELECT TRIM(name) FROM users;
来源：http://nml.zhiwuduotai.top

[Q85] 数值取整
来源：http://zwl.pengpengdd.cyou

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://aza.0kj1m.cn

[Q86] 读取 JSON 字段
来源：http://zrl.mhx1999.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://tsv.zhongyouzk.top

[Q87] JSON 字段做条件
来源：http://jwn.shanyushiyangtech.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://wcg.snrcjt.cn

[Q88] 行转列（条件聚合）
来源：http://rot.nwbrower.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://nmp.zhengqikj.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://exf.sxryk.cn

[Q89] 判断表是否存在
来源：http://ofe.jinqigfzy.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://fdp.sweek.top

[Q90] 生成序号列
来源：http://oxz.hysaishi.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://xjt.yfazqb.com

================================================================================
来源：http://bof.jlsjyb.cn

R. Bash 专题
来源：http://qmw.fengsongda.top

================================================================================
来源：http://ewv.andypj.xyz

[R01] shebang 与严格模式
来源：http://szg.gotoacloud.top

#!/usr/bin/env bash
来源：http://nzs.yongpay.top

set -euo pipefail
来源：http://wpt.sufxvd.cn

[R02] 变量赋值与使用
来源：http://jrg.hfpthk.cn

name="Tom"; echo "$name"
来源：http://jbr.zhijiandao.cn

[R03] 只读变量
来源：http://trn.haohaochexian.top

readonly PI=3.14
来源：http://xht.ywan-chungtsiang.top

[R04] 位置参数
来源：http://xit.zhengqikj.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://lwz.haohaochexian.top

[R05] 参数默认值
来源：http://flt.jianghu66.top

name="${1:-default}"
来源：http://asj.guannengcc.top

[R06] 判断命令是否存在
来源：http://lkg.kuanghao11.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://cft.wangdashe.top

[R07] if 判断文件
来源：http://ane.zhiwuduotai.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://dwq.shzxlz.cn

[R08] 数值比较
来源：http://tif.yfazqb.com

if (( a > b )); then echo "a 更大"; fi
来源：http://nhe.ehwqpu.com

[R09] 字符串比较
来源：http://amp.chenlongwang.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://pvy.pengpengdd.cyou

[R10] 正则匹配
来源：http://psw.jinqigfzy.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://enq.vqdsnc.cn

[R11] case 多分支
来源：http://suf.daria6918.cn

case "$1" in
来源：http://hvj.bjfxy.top

start) echo "启动" ;;
来源：http://tuq.ehwqpu.com

stop)  echo "停止" ;;
来源：http://knh.gotoacloud.top

*)     echo "未知命令" ;;
来源：http://uxo.hcnkem.com

esac
来源：http://lxp.andypj.xyz

[R12] for 遍历文件
来源：http://hbb.xuetiantiany.cn

for f in *.txt; do echo "$f"; done
来源：http://uty.hammf.cn

[R13] for 计数循环
来源：http://usw.hnxiangtu.top

for i in {1..10}; do echo "$i"; done
来源：http://xge.tarul.cn

[R14] C 风格 for
来源：http://fzs.zhijiandao.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://zww.aizwys.cn

[R15] while 逐行读文件
来源：http://kwv.ydzc1.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://cir.cucudq.cn

[R16] until 等待条件
来源：http://xru.yj20258888.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://pfe.quarkkingdee.top

[R17] 数组定义与取值
来源：http://pyw.dashuyun.cn

arr=(a b c); echo "${arr[0]}"
来源：http://xrd.tianlin.xyz

[R18] 遍历数组
来源：http://nju.jqgfzy.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://bmy.meibo888.top

[R19] 数组长度
来源：http://qab.jinqigufen.top

echo "${#arr[@]}"
来源：http://hrt.smart0.xyz

[R20] 关联数组（字典）
来源：http://ofs.jianghu66.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://qcw.fehbvm.com

[R21] 字符串长度
来源：http://bdk.fktsv.cn

echo "${#s}"
来源：http://shh.jinqigfzy.top

[R22] 截取子串
来源：http://wqh.xingfuxueyuan.xyz

echo "${s:0:5}"
来源：http://rkl.dashuyun.cn

[R23] 字符串替换
来源：http://fgp.gogol.net.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://mym.sjlbkw.cn

[R24] 大小写转换
来源：http://xsl.daria6918.cn

echo "${s^^}"; echo "${s,,}"
来源：http://bix.guowangkeji.top

[R25] 去后缀 / 去前缀
来源：http://daq.zhaomingkeji.xyz

echo "${f%.txt}"; echo "${f#./}"
来源：http://wsi.52xcode.cn

[R26] 命令替换
来源：http://hgx.sxryk.cn

now=$(date +%F); echo "$now"
来源：http://tlx.shanyushiyangkeji.top

[R27] 算术展开
来源：http://zxq.cucudq.cn

echo $((1 + 2 * 3))
来源：http://gea.jqgfzy.top

[R28] 浮点运算
来源：http://ybp.yueranfly.top

echo "scale=2; 10/3" | bc
来源：http://yyh.tanke756.top

[R29] 定义函数
来源：http://goi.fanxiaobao.xyz

add() { echo $(($1 + $2)); }; add 1 2
来源：http://ltc.tarul.cn

[R30] 函数返回状态码
来源：http://udq.jlsjyb.cn

f() { return 0; }; f || echo "失败了"
来源：http://zle.sweek.top

[R31] 局部变量
来源：http://anp.jyoumei.cn

f() { local x=1; echo "$x"; }
来源：http://txo.hesvh.cn

[R32] 参数个数校验
来源：http://vxd.bbcook.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://rez.uphjek.com

[R33] 捕获错误并提示行号
来源：http://vdr.hysaishi.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://quy.gotoacloud.top

[R34] 退出时清理
来源：http://qmr.yfazqb.com

trap 'rm -f "$tmp"' EXIT
来源：http://hot.tanke756.top

[R35] 后台执行并等待
来源：http://wti.fehbvm.com

sleep 5 & pid=$!; wait "$pid"
来源：http://fla.ctjpmb.com

[R36] 并发执行多个任务
来源：http://iiq.yangfankeji.com

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://gfh.xingfuxueyuan.xyz

[R37] 把输出赋给变量
来源：http://xwp.nanxinkj.top

files=$(ls -1)
来源：http://tla.hfpthk.cn

[R38] 管道串联
来源：http://fwj.zhixingplan.top

cat a.txt | grep -i error | wc -l
来源：http://omj.yj20258.top

[R39] 重定向标准输出与错误
来源：http://vje.yj20258.top

cmd > out.log 2>&1
来源：http://qwn.shzxlz.cn

[R40] 追加写日志
来源：http://bid.fanxiaobao.xyz

echo "log" >> out.log
来源：http://hsj.zhengqikj.top

[R41] 丢弃输出
来源：http://kqv.guowangkeji.top

cmd >/dev/null 2>&1
来源：http://qpl.daxiang520.top

[R42] 输入重定向
来源：http://jrv.fengsongda.top

wc -l < a.txt
来源：http://iwe.xylfe.cn

[R43] 按名字查找文件
来源：http://rww.jinghuilouyu.cn

find . -name "*.log" -type f
来源：http://igd.cashguo.top

[R44] 按修改时间查找
来源：http://abe.tianlin.xyz

find . -mtime -7 -type f
来源：http://sbt.sjlbkw.cn

[R45] 批量删除
来源：http://miq.daria6918.cn

find . -name "*.tmp" -delete
来源：http://knm.daria6918.cn

[R46] 递归替换文件内容
来源：http://whs.shanyushiyangtech.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://jsf.chenjidiqi.icu

[R47] sed 单行替换
来源：http://kps.jianghu66.top

sed -i 's/foo/bar/g' a.txt
来源：http://bxi.yuanzhike.top

[R48] awk 取指定列
来源：http://tjv.jinqigufen.top

awk '{print $1, $3}' a.txt
来源：http://zrl.shangyingyoupin.top

[R49] awk 带条件
来源：http://wyu.yuanzhike.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://iel.yangfankeji.com

[R50] awk 求和
来源：http://skv.yanxiufei.cn

awk '{s += $2} END {print s}' a.txt
来源：http://wej.chenlongwang.top

[R51] 排序去重取前几
来源：http://vlk.dianchejie.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://rsw.chenjidiqi.icu

[R52] 统计行数
来源：http://own.havefunace.top

wc -l a.txt
来源：http://mqw.hnqzz.top

[R53] 查看文件头与实时尾
来源：http://qgw.hnxiangtu.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://ykj.chenjidiqi.icu

[R54] 比较两个文件
来源：http://cmc.xuetiantiany.cn

diff a.txt b.txt
来源：http://kyt.xingfuxueyuan.xyz

[R55] 压缩与解压
来源：http://xzo.gaohongyu789.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://shl.fktsv.cn

[R56] 远程拷贝
来源：http://zct.ydzc1.top

scp file user@host:/path/
来源：http://qad.gaohongyu789.top

[R57] 远程执行命令
来源：http://kkm.andypj.xyz

ssh user@host 'uptime'
来源：http://oxr.jinghuilouyu.cn

[R58] 下载文件
来源：http://mpk.gotoacloud.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://adz.ywan-chungtsiang.top

[R59] 发 POST JSON
来源：http://bbv.quarkkingdee.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hfj.ppjwa.cn

[R60] 只看 HTTP 状态码
来源：http://ifb.yueranfly.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://wvq.dianchejie.cn

[R61] 磁盘占用
来源：http://hme.chenlongwang.top

df -h;  du -sh *
来源：http://ool.tanke756.top

[R62] 找最占空间的文件
来源：http://mte.mhx1999.top

du -ah . | sort -rh | head -10
来源：http://ieh.vqdsnc.cn

[R63] 内存与进程
来源：http://get.xuetiantiany.cn

free -h;  ps aux | grep nginx
来源：http://sah.wangdashe.top

[R64] 结束进程
来源：http://elg.ydjk.org.cn

kill -9 $(pgrep -f app.py)
来源：http://glb.sxryk.cn

[R65] 查看端口占用
来源：http://egn.xuetiantiany.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://qqb.ctjpmb.com

[R66] 定时任务
来源：http://lpz.zhengqikj.top

crontab -e;  crontab -l
来源：http://uyp.nanxuanxn.top

[R67] 生成随机十六进制串
来源：http://mth.kuanghao11.cn

openssl rand -hex 16
来源：http://lrh.gzhubu.top

[R68] 计算文件校验值
来源：http://hch.zhengqikj.top

sha256sum a.txt;  md5sum a.txt
来源：http://tsu.zycfv.cn

[R69] 生成随机密码
来源：http://cvl.nwbrower.top

head -c 16 /dev/urandom | base64
来源：http://ndv.smart0.xyz

[R70] 时间戳与互转
来源：http://ngs.sysykeji.top

date +%s;  date -d @1700000000
来源：http://rma.hcnkem.com

[R71] 日期格式化
来源：http://bdq.sjlbkw.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://rat.nanxinkj.top

[R72] 等待端口就绪
来源：http://sgc.yj20258888.top

until nc -z localhost 3306; do sleep 1; done
来源：http://jht.yueranfly.top

[R73] 分割大日志
来源：http://xzf.pycfn.com

split -l 1000 big.log part_
来源：http://eao.shangyingyoupin.top

[R74] 批量重命名
来源：http://qql.shzxlz.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://moj.hesvh.cn

[R75] 导出环境变量
来源：http://eet.tian-w.cn

export PATH="$HOME/bin:$PATH"
来源：http://new.svipenyu.cn

[R76] 使用临时文件
来源：http://hmz.tianlin.xyz

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://teh.dashuyun.cn

[R77] 读取用户输入
来源：http://ubp.zhixingplan.top

read -rp "请输入: " ans
来源：http://msd.snrcjt.cn

[R78] 交互式菜单
来源：http://ynx.sxryk.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://plg.feifeiyinyue.top

[R79] 解析命令行选项
来源：http://ume.yuxming.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://ust.wangdashe.top

[R80] 查看脚本执行耗时
来源：http://kty.zhengqikj.top

time ./run.sh
来源：http://kpk.feifeiyinyue.top

================================================================================
来源：http://srt.9152youxi.cn

S. C / C++ 专题
来源：http://fov.feifeiyinyue.top

================================================================================
来源：http://iuu.hongshengwenyu.top

[S01] C：Hello World
来源：http://okv.snrcjt.cn

#include <stdio.h>
来源：http://ddz.zhongyouzk.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://oci.sxryk.cn

[S02] C：变量与格式化输出
来源：http://lnb.xylfe.cn

int a = 10; printf("%d\n", a);
来源：http://ekk.xingfuxueyuan.xyz

[S03] C：读入整数
来源：http://iri.yj20258.top

int x; scanf("%d", &x);
来源：http://tbw.yonumen.top

[S04] C：字符串复制
来源：http://enj.dianchejie.cn

char dst[32]; strcpy(dst, "hi");
来源：http://byn.mhx1999.top

[S05] C：字符串长度
来源：http://yky.shuidangran.top

strlen(s)
来源：http://ewx.ydjk.org.cn

[S06] C：字符串比较
来源：http://iir.jqgfzy.top

strcmp(a, b) == 0
来源：http://hry.yanxiufei.cn

[S07] C：数组遍历求和
来源：http://ofd.tianlin.xyz

for (int i = 0; i < n; i++) sum += a[i];
来源：http://ntb.yj20258888.top

[S08] C：动态内存分配与释放
来源：http://fwf.fktsv.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://kxl.ydzc1.top

[S09] C：结构体定义与初始化
来源：http://nic.xylfe.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://uzk.epnwcf.com

[S10] C：指针与解引用
来源：http://tts.zdbjq.cn

int *p = &a;  *p = 5;
来源：http://ztu.sjlbkw.cn

[S11] C：逐行读文件
来源：http://yjq.jyoumei.cn

FILE *f = fopen("a.txt", "r");
来源：http://wlp.tanke756.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://nhi.cqqwz.cn

fclose(f);
来源：http://fhv.gogol.net.cn

[S12] C：写文件
来源：http://efx.xingfuxueyuan.xyz

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://bmu.epnwcf.com

[S13] C：宏定义
来源：http://rsd.hnqzz.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://tkm.gotoacloud.top

[S14] C：枚举
来源：http://aaj.zhongyouzk.top

enum Color { RED, GREEN, BLUE };
来源：http://lhg.chenjidiqi.icu

[S15] C：类型转换
来源：http://jow.yuxming.cn

(double) a / b
来源：http://yta.nanxinkj.top

[S16] C：位操作置位
来源：http://bkz.snrcjt.cn

x |= (1 << 3);
来源：http://agf.sjlbkw.cn

[S17] C：安全拼接字符串
来源：http://hmd.jqgufenzy.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://exj.fehbvm.com

[S18] C：命令行参数
来源：http://naj.fktsv.cn

int main(int argc, char **argv)
来源：http://djr.vqdsnc.cn

[S19] C：快速排序
来源：http://iih.quarkkingdee.top

qsort(a, n, sizeof(int), cmp);
来源：http://jin.yfazqb.com

[S20] C：二分查找
来源：http://iur.jinghuilouyu.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://ejl.jqgfzy.top

[S21] C：字符类别判断
来源：http://gba.yongpay.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://fha.cheryme.top

[S22] C：字符串转数字
来源：http://bqj.aibaodan.cn

atoi("42");  strtod("3.14", NULL);
来源：http://scs.andypj.xyz

[S23] C：随机数
来源：http://ukp.316326.xyz

srand(time(NULL));  int r = rand() % 100;
来源：http://aog.ehwqpu.com

[S24] C：获取本地时间
来源：http://iss.dashuyun.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://xhu.yuxming.cn

[S25] C：内存拷贝
来源：http://yxj.vehdjk.com

memcpy(dst, src, n);
来源：http://ijq.tarul.cn

[S26] C：内存清零
来源：http://zdm.52xcode.cn

memset(a, 0, sizeof a);
来源：http://dmr.yuanzhike.top

[S27] C：定义常量
来源：http://ror.aizwys.cn

const double PI = 3.14159;
来源：http://dbd.9152youxi.cn

[S28] C：静态变量
来源：http://dqr.hnxiangtu.top

static int counter = 0;
来源：http://hqs.wangdashe.top

[S29] C：变参函数
来源：http://uqb.nwbrower.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://qqc.zhixingplan.top

[S30] C：头文件保护
来源：http://quv.sxryk.cn

#ifndef X_H
来源：http://ymg.quarkkingdee.top

#define X_H
来源：http://fzi.cashguo.top

#endif
来源：http://nuj.jqgufenzy.top

[S31] C++：Hello World
来源：http://jhf.wangdashe.top

#include <iostream>
来源：http://oyb.jiagoushi.top

int main() { std::cout << "Hello\n"; }
来源：http://sof.epnwcf.com

[S32] C++：字符串
来源：http://tnu.jinghuilouyu.cn

std::string s = "hi";  s += "!";
来源：http://jez.daria6918.cn

[S33] C++：vector 增删
来源：http://mps.tanke756.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://pgp.52xcode.cn

[S34] C++：遍历 vector
来源：http://xcs.ydjk.org.cn

for (auto &x : v) { std::cout << x; }
来源：http://bqq.gzhubu.top

[S35] C++：map
来源：http://uby.yvedp.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://tsx.yuanzhike.top

[S36] C++：unordered_map
来源：http://krd.316326.xyz

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://yrf.daria6918.cn

[S37] C++：set
来源：http://edh.hammf.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://icb.birdmap.top

[S38] C++：排序
来源：http://pvs.quarkkingdee.top

std::sort(v.begin(), v.end());
来源：http://poy.ppjwa.cn

[S39] C++：自定义比较器排序
来源：http://mek.shangyingyoupin.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://nxp.havefunace.top

[S40] C++：查找元素
来源：http://gcl.hysaishi.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://ibx.vehdjk.com

[S41] C++：类与构造函数
来源：http://ggl.shanyushiyangkeji.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://dbg.yueranfly.top

[S42] C++：继承与虚函数
来源：http://kyn.shuidangran.top

class B : public Base { public: void f() override {} };
来源：http://cdv.chenjidiqi.icu


<!-- 参考信息 -->