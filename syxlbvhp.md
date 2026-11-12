代发 wailian999

[Q78] 当前时间
来源：http://ozf.shanyushiyangkeji.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://ljd.yfazqb.com

[Q79] 字符串拼接
来源：http://fuw.guannengcc.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://pro.bjfxy.top

[Q80] 字符串截取
来源：http://zrs.fengsongda.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://yae.yuxming.cn

[Q81] 字符串替换
来源：http://qyf.shanyushiyangtech.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://ebf.zycfv.cn

[Q82] 字符长度与字节长度
来源：http://igk.yj20258.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://pks.sysykeji.top

[Q83] 大小写转换
来源：http://ohl.vehdjk.com

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://nhc.chenlongwang.top

[Q84] 去除首尾空格
来源：http://nls.gaohongyu789.top

SELECT TRIM(name) FROM users;
来源：http://sjl.redwolf501.top

[Q85] 数值取整
来源：http://emd.zhijiandao.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://vuo.yangfankeji.com

[Q86] 读取 JSON 字段
来源：http://qsz.hcnkem.com

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://zam.zhongyouzk.top

[Q87] JSON 字段做条件
来源：http://oml.chenzaomai.com

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://mhf.ctjpmb.com

[Q88] 行转列（条件聚合）
来源：http://tce.gzhubu.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://lsx.tanke756.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://gxi.dashuyun.cn

[Q89] 判断表是否存在
来源：http://ilx.zdbjq.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://eug.gaohongyu789.top

[Q90] 生成序号列
来源：http://chp.yuxming.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://ogv.hnqzz.top

================================================================================
来源：http://iij.nanxuanxn.top

R. Bash 专题
来源：http://xbz.yonumen.top

================================================================================
来源：http://lsc.yuanzhike.top

[R01] shebang 与严格模式
来源：http://dfi.tanke756.top

#!/usr/bin/env bash
来源：http://efl.bbcook.cn

set -euo pipefail
来源：http://rpf.hammf.cn

[R02] 变量赋值与使用
来源：http://nmz.gotoacloud.top

name="Tom"; echo "$name"
来源：http://hgv.jqgufenzy.top

[R03] 只读变量
来源：http://naf.sweek.top

readonly PI=3.14
来源：http://zjx.52xcode.cn

[R04] 位置参数
来源：http://xwr.fanxiaobao.xyz

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://vge.nanxuanxn.top

[R05] 参数默认值
来源：http://cso.xinyue.icu

name="${1:-default}"
来源：http://saz.ydjk.org.cn

[R06] 判断命令是否存在
来源：http://uhd.yongpay.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://zug.c1oappe.top

[R07] if 判断文件
来源：http://caw.yongpay.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://qlu.mhx1999.top

[R08] 数值比较
来源：http://rhl.andypj.xyz

if (( a > b )); then echo "a 更大"; fi
来源：http://gow.hnxiangtu.top

[R09] 字符串比较
来源：http://siq.ppjwa.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://kfl.hongshengwenyu.top

[R10] 正则匹配
来源：http://wxi.sjlbkw.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://zcw.fengsongda.top

[R11] case 多分支
来源：http://tkt.bbcook.cn

case "$1" in
来源：http://ebf.yongpay.top

start) echo "启动" ;;
来源：http://nnq.yongpay.top

stop)  echo "停止" ;;
来源：http://etz.feifeiyinyue.top

*)     echo "未知命令" ;;
来源：http://ccx.bbcook.cn

esac
来源：http://hhe.yj20258.top

[R12] for 遍历文件
来源：http://pou.kuanghao11.cn

for f in *.txt; do echo "$f"; done
来源：http://eyg.yonumen.top

[R13] for 计数循环
来源：http://swg.jinqigufen.top

for i in {1..10}; do echo "$i"; done
来源：http://svg.yangfankeji.com

[R14] C 风格 for
来源：http://tvx.jqgufenzy.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://ove.zhiwuduotai.top

[R15] while 逐行读文件
来源：http://cng.yvedp.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://ckk.tanke756.top

[R16] until 等待条件
来源：http://nyf.smart0.xyz

until [[ -f done.flag ]]; do sleep 1; done
来源：http://frq.hcnkem.com

[R17] 数组定义与取值
来源：http://bcq.ywan-chungtsiang.top

arr=(a b c); echo "${arr[0]}"
来源：http://inp.zhijiandao.cn

[R18] 遍历数组
来源：http://jgm.zhoulong.xyz

for x in "${arr[@]}"; do echo "$x"; done
来源：http://rcl.tanke756.top

[R19] 数组长度
来源：http://plz.chenlongwang.top

echo "${#arr[@]}"
来源：http://pjb.yfazqb.com

[R20] 关联数组（字典）
来源：http://vwa.bjfxy.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://vmn.fehbvm.com

[R21] 字符串长度
来源：http://vix.sweek.top

echo "${#s}"
来源：http://uml.316326.xyz

[R22] 截取子串
来源：http://neb.yongpay.top

echo "${s:0:5}"
来源：http://lnw.zhiwuduotai.top

[R23] 字符串替换
来源：http://mms.jinqigfzy.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://quw.ctjpmb.com

[R24] 大小写转换
来源：http://sem.shangyingyoupin.top

echo "${s^^}"; echo "${s,,}"
来源：http://ltl.cucudq.cn

[R25] 去后缀 / 去前缀
来源：http://stt.andypj.xyz

echo "${f%.txt}"; echo "${f#./}"
来源：http://rwf.mhx1999.top

[R26] 命令替换
来源：http://mth.andypj.xyz

now=$(date +%F); echo "$now"
来源：http://tth.ctjpmb.com

[R27] 算术展开
来源：http://thi.cashguo.top

echo $((1 + 2 * 3))
来源：http://qdq.0kj1m.cn

[R28] 浮点运算
来源：http://ehy.fktsv.cn

echo "scale=2; 10/3" | bc
来源：http://pgw.redwolf501.top

[R29] 定义函数
来源：http://xry.jinqigufen.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://jdu.snrcjt.cn

[R30] 函数返回状态码
来源：http://wrl.vehdjk.com

f() { return 0; }; f || echo "失败了"
来源：http://nwo.yvedp.cn

[R31] 局部变量
来源：http://tdr.jinqigufen.top

f() { local x=1; echo "$x"; }
来源：http://vgq.nanxuanxn.top

[R32] 参数个数校验
来源：http://bvn.iojbl.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://bwg.xuetiantiany.cn

[R33] 捕获错误并提示行号
来源：http://jme.dashuyun.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://vmc.ydzc1.top

[R34] 退出时清理
来源：http://cjv.pengpengdd.cyou

trap 'rm -f "$tmp"' EXIT
来源：http://ate.pengpengdd.cyou

[R35] 后台执行并等待
来源：http://rvk.mhx1999.top

sleep 5 & pid=$!; wait "$pid"
来源：http://qso.guowangkeji.top

[R36] 并发执行多个任务
来源：http://zes.xinyue.icu

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://wsp.hongshengwenyu.top

[R37] 把输出赋给变量
来源：http://rds.hesvh.cn

files=$(ls -1)
来源：http://dbh.yuxming.cn

[R38] 管道串联
来源：http://lxr.aizwys.cn

cat a.txt | grep -i error | wc -l
来源：http://lec.yangfankeji.com

[R39] 重定向标准输出与错误
来源：http://zzr.ehwqpu.com

cmd > out.log 2>&1
来源：http://qrh.jianghu66.top

[R40] 追加写日志
来源：http://bnl.daxiang520.top

echo "log" >> out.log
来源：http://ffg.zhijiandao.cn

[R41] 丢弃输出
来源：http://lpv.jyoumei.cn

cmd >/dev/null 2>&1
来源：http://fow.fzhhl.top

[R42] 输入重定向
来源：http://ikw.guannengcc.top

wc -l < a.txt
来源：http://ofn.zdqjudy.top

[R43] 按名字查找文件
来源：http://esx.guowangkeji.top

find . -name "*.log" -type f
来源：http://gjd.vqdsnc.cn

[R44] 按修改时间查找
来源：http://lbu.zhijiandao.cn

find . -mtime -7 -type f
来源：http://sgf.haohaochexian.top

[R45] 批量删除
来源：http://mvo.ivvv.top

find . -name "*.tmp" -delete
来源：http://mpv.feifeiyinyue.top

[R46] 递归替换文件内容
来源：http://kte.shuidangran.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://vmo.sufxvd.cn

[R47] sed 单行替换
来源：http://gty.tian-w.cn

sed -i 's/foo/bar/g' a.txt
来源：http://hoc.cashguo.top

[R48] awk 取指定列
来源：http://zcy.yueranfly.top

awk '{print $1, $3}' a.txt
来源：http://nrr.zycfv.cn

[R49] awk 带条件
来源：http://dsh.cdnleiting.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://ytq.nanxuanxn.top

[R50] awk 求和
来源：http://bgw.svipenyu.cn

awk '{s += $2} END {print s}' a.txt
来源：http://ooy.hesvh.cn

[R51] 排序去重取前几
来源：http://bxj.jinqigufen.top

sort a.txt | uniq -c | sort -rn | head
来源：http://ckl.redwolf501.top

[R52] 统计行数
来源：http://qnu.jyoumei.cn

wc -l a.txt
来源：http://bdk.zhiwuduotai.top

[R53] 查看文件头与实时尾
来源：http://kow.jinqigufen.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://zog.haohaochexian.top

[R54] 比较两个文件
来源：http://avy.tanke756.top

diff a.txt b.txt
来源：http://ptf.zdbjq.cn

[R55] 压缩与解压
来源：http://yey.daxiang520.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://rnr.zdqjudy.top

[R56] 远程拷贝
来源：http://aun.hywenlv.cn

scp file user@host:/path/
来源：http://oam.gogol.net.cn

[R57] 远程执行命令
来源：http://hyh.9152youxi.cn

ssh user@host 'uptime'
来源：http://nee.yongpay.top

[R58] 下载文件
来源：http://qjv.dianchejie.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://ruh.kuanghao11.cn

[R59] 发 POST JSON
来源：http://mlb.gotoacloud.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://kpz.jinqigufen.top

[R60] 只看 HTTP 状态码
来源：http://tre.zhoulong.xyz

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://zjc.xingfuxueyuan.xyz

[R61] 磁盘占用
来源：http://alh.yj202588.top

df -h;  du -sh *
来源：http://woe.zhaomingkeji.xyz

[R62] 找最占空间的文件
来源：http://xzc.aibaodan.cn

du -ah . | sort -rh | head -10
来源：http://eud.dianchejie.cn

[R63] 内存与进程
来源：http://vdq.ppjwa.cn

free -h;  ps aux | grep nginx
来源：http://dtx.c1oappe.top

[R64] 结束进程
来源：http://kdr.snrcjt.cn

kill -9 $(pgrep -f app.py)
来源：http://crv.jianghu66.top

[R65] 查看端口占用
来源：http://fnz.zhiwuduotai.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://apq.yuxming.cn

[R66] 定时任务
来源：http://rwy.zdqjudy.top

crontab -e;  crontab -l
来源：http://idp.jinqigufen.top

[R67] 生成随机十六进制串
来源：http://use.zhiwuduotai.top

openssl rand -hex 16
来源：http://tki.jinyuanbaomall.cn

[R68] 计算文件校验值
来源：http://yus.pengpengdd.cyou

sha256sum a.txt;  md5sum a.txt
来源：http://shy.hcnkem.com

[R69] 生成随机密码
来源：http://prl.jqgfzy.top

head -c 16 /dev/urandom | base64
来源：http://azh.wangdashe.top

[R70] 时间戳与互转
来源：http://zjk.hcnkem.com

date +%s;  date -d @1700000000
来源：http://rtq.tianlin.xyz

[R71] 日期格式化
来源：http://gat.daxiang520.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://var.sysykeji.top

[R72] 等待端口就绪
来源：http://hxw.52xcode.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://gjl.haohaochexian.top

[R73] 分割大日志
来源：http://wgt.shangyingyoupin.top

split -l 1000 big.log part_
来源：http://qgx.nanxuanxn.top

[R74] 批量重命名
来源：http://vtk.aibaodan.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://fmr.sweek.top

[R75] 导出环境变量
来源：http://nyu.nanxuanxn.top

export PATH="$HOME/bin:$PATH"
来源：http://wos.shanyushiyangtech.top

[R76] 使用临时文件
来源：http://ilp.haohaochexian.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://ffu.shzxlz.cn

[R77] 读取用户输入
来源：http://rac.bbcook.cn

read -rp "请输入: " ans
来源：http://qpu.meibo888.top

[R78] 交互式菜单
来源：http://nnh.daria6918.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://jzz.zhoulong.xyz

[R79] 解析命令行选项
来源：http://uwy.sjlbkw.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://gpm.nanxinkj.top

[R80] 查看脚本执行耗时
来源：http://gnp.vqdsnc.cn

time ./run.sh
来源：http://eka.yonumen.top

================================================================================
来源：http://dpb.gotoacloud.top

S. C / C++ 专题
来源：http://ibq.birdmap.top

================================================================================
来源：http://fpp.shangyingyoupin.top

[S01] C：Hello World
来源：http://uzi.shanyushiyangkeji.top

#include <stdio.h>
来源：http://ell.dashuyun.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://zoz.snrcjt.cn

[S02] C：变量与格式化输出
来源：http://ber.zdqjudy.top

int a = 10; printf("%d\n", a);
来源：http://jra.pengpengdd.cyou

[S03] C：读入整数
来源：http://qsk.ctjpmb.com

int x; scanf("%d", &x);
来源：http://qsh.zhiwuduotai.top

[S04] C：字符串复制
来源：http://lfx.yj20258.top

char dst[32]; strcpy(dst, "hi");
来源：http://jcf.shuidangran.top

[S05] C：字符串长度
来源：http://axq.jlsjyb.cn

strlen(s)
来源：http://dcb.xylfe.cn

[S06] C：字符串比较
来源：http://apx.zdqjudy.top

strcmp(a, b) == 0
来源：http://rpq.yueranfly.top

[S07] C：数组遍历求和
来源：http://xwq.shuidangran.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://xtg.zdqjudy.top

[S08] C：动态内存分配与释放
来源：http://ynv.ydjk.org.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://lbm.tarul.cn

[S09] C：结构体定义与初始化
来源：http://cej.fengsongda.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://dbk.jyoumei.cn

[S10] C：指针与解引用
来源：http://jbj.zhixingplan.top

int *p = &a;  *p = 5;
来源：http://uvd.vehdjk.com

[S11] C：逐行读文件
来源：http://vie.jinyuanbaomall.cn

FILE *f = fopen("a.txt", "r");
来源：http://enf.316326.xyz

while (fgets(buf, sizeof buf, f)) { }
来源：http://vnx.chenjidiqi.icu

fclose(f);
来源：http://vgw.zhiwuduotai.top

[S12] C：写文件
来源：http://efq.52xcode.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://twb.hammf.cn

[S13] C：宏定义
来源：http://waa.zhengqikj.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://sja.fktsv.cn

[S14] C：枚举
来源：http://mfn.sweek.top

enum Color { RED, GREEN, BLUE };
来源：http://vkt.yj20258.top

[S15] C：类型转换
来源：http://vpe.jinyuanbaomall.cn

(double) a / b
来源：http://mav.meibo888.top

[S16] C：位操作置位
来源：http://ucb.cheryme.top

x |= (1 << 3);
来源：http://mpr.yongpay.top

[S17] C：安全拼接字符串
来源：http://nzm.316326.xyz

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://aqb.ybcxt.top

[S18] C：命令行参数
来源：http://evo.xziqi.cn

int main(int argc, char **argv)
来源：http://kdt.xuetiantiany.cn

[S19] C：快速排序
来源：http://xll.yj20258.top

qsort(a, n, sizeof(int), cmp);
来源：http://bxi.ydjk.org.cn

[S20] C：二分查找
来源：http://zby.fehbvm.com

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://ktk.sysykeji.top

[S21] C：字符类别判断
来源：http://ect.hesvh.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://tdh.vqdsnc.cn

[S22] C：字符串转数字
来源：http://gir.snrcjt.cn

atoi("42");  strtod("3.14", NULL);
来源：http://uid.fktsv.cn

[S23] C：随机数
来源：http://cfd.sweek.top

srand(time(NULL));  int r = rand() % 100;
来源：http://fgi.cdnleiting.top

[S24] C：获取本地时间
来源：http://std.bjfxy.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://emq.jqgufenzy.top

[S25] C：内存拷贝
来源：http://vbk.zhijiandao.cn

memcpy(dst, src, n);
来源：http://apd.hnqzz.top

[S26] C：内存清零
来源：http://vxf.dianchejie.cn

memset(a, 0, sizeof a);
来源：http://lim.gogol.net.cn

[S27] C：定义常量
来源：http://krz.gzhubu.top

const double PI = 3.14159;
来源：http://jiz.birdmap.top

[S28] C：静态变量
来源：http://ydb.ywan-chungtsiang.top

static int counter = 0;
来源：http://irq.yj20258888.top

[S29] C：变参函数
来源：http://jqg.hysaishi.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://siy.chenzaomai.com

[S30] C：头文件保护
来源：http://dhq.jinqigfzy.top

#ifndef X_H
来源：http://ycr.uphjek.com

#define X_H
来源：http://dtz.yanxiufei.cn

#endif
来源：http://pjl.iojbl.cn

[S31] C++：Hello World
来源：http://czn.shanyushiyangtech.top

#include <iostream>
来源：http://nlp.dashuyun.cn

int main() { std::cout << "Hello\n"; }
来源：http://kai.jianghu66.top

[S32] C++：字符串
来源：http://lzy.dashuyun.cn

std::string s = "hi";  s += "!";
来源：http://lzg.sxryk.cn

[S33] C++：vector 增删
来源：http://rba.jqgfzy.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://vuf.hfpthk.cn

[S34] C++：遍历 vector
来源：http://jbc.tanke756.top

for (auto &x : v) { std::cout << x; }
来源：http://yck.guannengcc.top

[S35] C++：map
来源：http://vms.andypj.xyz

std::map<std::string, int> m;  m["a"] = 1;
来源：http://zmp.tianlin.xyz

[S36] C++：unordered_map
来源：http://lyr.shangyingyoupin.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://oek.shzxlz.cn

[S37] C++：set
来源：http://opn.meibo888.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://tav.aibaodan.cn

[S38] C++：排序
来源：http://jmq.yonumen.top

std::sort(v.begin(), v.end());
来源：http://gqb.meibo888.top

[S39] C++：自定义比较器排序
来源：http://aks.zhixingplan.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://ica.zhiwuduotai.top

[S40] C++：查找元素
来源：http://qyr.yueranfly.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://plc.cqqwz.cn

[S41] C++：类与构造函数
来源：http://qxi.sjlbkw.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://tgc.cashguo.top

[S42] C++：继承与虚函数
来源：http://ypo.quarkkingdee.top

class B : public Base { public: void f() override {} };
来源：http://jep.haohaochexian.top

[S43] C++：智能指针
来源：http://teo.yj20258888.top

auto p = std::make_unique<int>(5);
来源：http://uji.gogol.net.cn

[S44] C++：引用传参
来源：http://scx.fengsongda.top

void inc(int &x) { ++x; }
来源：http://rqu.ydjk.org.cn

[S45] C++：lambda
来源：http://gno.hysaishi.cn

auto add = [](int a, int b) { return a + b; };
来源：http://nyb.vqdsnc.cn

[S46] C++：函数模板
来源：http://nsf.jiagoushi.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://lfj.vehdjk.com

[S47] C++：结构化绑定遍历
来源：http://abn.zhixingplan.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://suy.sjlbkw.cn

[S48] C++：逐行读文件
来源：http://dtz.cucudq.cn

std::ifstream in("a.txt");  std::string line;
来源：http://vlx.fengsongda.top


<!-- 参考信息 -->