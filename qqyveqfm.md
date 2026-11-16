代发 wailian999

[Q88] 行转列（条件聚合）
来源：http://ahj.birdmap.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://ogh.hammf.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://ipp.xziqi.cn

[Q89] 判断表是否存在
来源：http://yyc.52xcode.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://myb.hesvh.cn

[Q90] 生成序号列
来源：http://izm.ppjwa.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://jkr.hongshengwenyu.top

================================================================================
来源：http://iwk.zdqjudy.top

R. Bash 专题
来源：http://dwg.havefunace.top

================================================================================
来源：http://pal.hesvh.cn

[R01] shebang 与严格模式
来源：http://elz.chenjidiqi.icu

#!/usr/bin/env bash
来源：http://ovt.jyoumei.cn

set -euo pipefail
来源：http://nua.yfazqb.com

[R02] 变量赋值与使用
来源：http://eqp.uphjek.com

name="Tom"; echo "$name"
来源：http://fas.hysaishi.cn

[R03] 只读变量
来源：http://zfc.hesvh.cn

readonly PI=3.14
来源：http://uoz.ehwqpu.com

[R04] 位置参数
来源：http://ubr.ywan-chungtsiang.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hvd.fanxiaobao.xyz

[R05] 参数默认值
来源：http://sch.xylfe.cn

name="${1:-default}"
来源：http://pnz.jinyuanbaomall.cn

[R06] 判断命令是否存在
来源：http://vje.xingfuxueyuan.xyz

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://sem.tanke756.top

[R07] if 判断文件
来源：http://pap.gaohongyu789.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hwk.sjlbkw.cn

[R08] 数值比较
来源：http://ina.ivvv.top

if (( a > b )); then echo "a 更大"; fi
来源：http://lqz.tarul.cn

[R09] 字符串比较
来源：http://kcb.bjfxy.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://biy.jqgfzy.top

[R10] 正则匹配
来源：http://dki.yj20258.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://wlg.9152youxi.cn

[R11] case 多分支
来源：http://nzl.hywenlv.cn

case "$1" in
来源：http://pqh.redwolf501.top

start) echo "启动" ;;
来源：http://llr.ydjk.org.cn

stop)  echo "停止" ;;
来源：http://qrd.52xcode.cn

*)     echo "未知命令" ;;
来源：http://blt.9152youxi.cn

esac
来源：http://ksq.jianghu66.top

[R12] for 遍历文件
来源：http://dxv.andypj.xyz

for f in *.txt; do echo "$f"; done
来源：http://lzn.guowangkeji.top

[R13] for 计数循环
来源：http://evv.nwbrower.top

for i in {1..10}; do echo "$i"; done
来源：http://ixd.sweek.top

[R14] C 风格 for
来源：http://qjd.bjfxy.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://alh.ehwqpu.com

[R15] while 逐行读文件
来源：http://ujz.fzhhl.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://pgc.fktsv.cn

[R16] until 等待条件
来源：http://rbf.daxiang520.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://rvp.tanke756.top

[R17] 数组定义与取值
来源：http://ngg.9152youxi.cn

arr=(a b c); echo "${arr[0]}"
来源：http://ejv.tian-w.cn

[R18] 遍历数组
来源：http://mpx.daxiang520.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://fhc.daria6918.cn

[R19] 数组长度
来源：http://cho.fanxiaobao.xyz

echo "${#arr[@]}"
来源：http://cms.zycfv.cn

[R20] 关联数组（字典）
来源：http://wfx.jinqigufen.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://sot.yongpay.top

[R21] 字符串长度
来源：http://zbo.havefunace.top

echo "${#s}"
来源：http://hia.tanke756.top

[R22] 截取子串
来源：http://bgs.pycfn.com

echo "${s:0:5}"
来源：http://fcl.ydjk.org.cn

[R23] 字符串替换
来源：http://dox.hnqzz.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://pag.iojbl.cn

[R24] 大小写转换
来源：http://vnb.tanke756.top

echo "${s^^}"; echo "${s,,}"
来源：http://pkg.haohaochexian.top

[R25] 去后缀 / 去前缀
来源：http://pgl.redwolf501.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://rrj.aizwys.cn

[R26] 命令替换
来源：http://srs.cheryme.top

now=$(date +%F); echo "$now"
来源：http://thx.svipenyu.cn

[R27] 算术展开
来源：http://bgu.zhongyouzk.top

echo $((1 + 2 * 3))
来源：http://wwu.chenlongwang.top

[R28] 浮点运算
来源：http://joo.jqgufenzy.top

echo "scale=2; 10/3" | bc
来源：http://gtr.yuxming.cn

[R29] 定义函数
来源：http://kve.xinyue.icu

add() { echo $(($1 + $2)); }; add 1 2
来源：http://bha.hysaishi.cn

[R30] 函数返回状态码
来源：http://iyx.sufxvd.cn

f() { return 0; }; f || echo "失败了"
来源：http://kxs.zhijiandao.cn

[R31] 局部变量
来源：http://zmd.haohaochexian.top

f() { local x=1; echo "$x"; }
来源：http://rvw.fengsongda.top

[R32] 参数个数校验
来源：http://kwd.zhixingplan.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://pri.daria6918.cn

[R33] 捕获错误并提示行号
来源：http://oyq.haohaochexian.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://zcs.tian-w.cn

[R34] 退出时清理
来源：http://hrm.smart0.xyz

trap 'rm -f "$tmp"' EXIT
来源：http://ndx.aibaodan.cn

[R35] 后台执行并等待
来源：http://wmn.xziqi.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://lsv.yuanzhike.top

[R36] 并发执行多个任务
来源：http://mvj.cucudq.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://bls.xuetiantiany.cn

[R37] 把输出赋给变量
来源：http://vec.zhixingplan.top

files=$(ls -1)
来源：http://gus.chenjidiqi.icu

[R38] 管道串联
来源：http://kji.hysaishi.cn

cat a.txt | grep -i error | wc -l
来源：http://ore.pengpengdd.cyou

[R39] 重定向标准输出与错误
来源：http://xtu.shuidangran.top

cmd > out.log 2>&1
来源：http://xrp.aibaodan.cn

[R40] 追加写日志
来源：http://egd.zhixingplan.top

echo "log" >> out.log
来源：http://oue.snrcjt.cn

[R41] 丢弃输出
来源：http://nem.sweek.top

cmd >/dev/null 2>&1
来源：http://ghr.yuxming.cn

[R42] 输入重定向
来源：http://ojs.yuxming.cn

wc -l < a.txt
来源：http://ayw.zhaomingkeji.xyz

[R43] 按名字查找文件
来源：http://ema.hcnkem.com

find . -name "*.log" -type f
来源：http://jfj.cdnleiting.top

[R44] 按修改时间查找
来源：http://xje.yuxming.cn

find . -mtime -7 -type f
来源：http://ysn.xylfe.cn

[R45] 批量删除
来源：http://lbr.yongpay.top

find . -name "*.tmp" -delete
来源：http://slf.52xcode.cn

[R46] 递归替换文件内容
来源：http://jvz.gzhubu.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://ipe.yj20258888.top

[R47] sed 单行替换
来源：http://bcq.tanke756.top

sed -i 's/foo/bar/g' a.txt
来源：http://owq.zhoulong.xyz

[R48] awk 取指定列
来源：http://lor.zhijiandao.cn

awk '{print $1, $3}' a.txt
来源：http://miw.52xcode.cn

[R49] awk 带条件
来源：http://don.zdbjq.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hzr.vqdsnc.cn

[R50] awk 求和
来源：http://rzt.quarkkingdee.top

awk '{s += $2} END {print s}' a.txt
来源：http://lmg.yj20258.top

[R51] 排序去重取前几
来源：http://akj.shanyushiyangkeji.top

sort a.txt | uniq -c | sort -rn | head
来源：http://kqe.zhixingplan.top

[R52] 统计行数
来源：http://tcn.jyoumei.cn

wc -l a.txt
来源：http://jdq.xziqi.cn

[R53] 查看文件头与实时尾
来源：http://unj.yj202588.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://wua.yj20258888.top

[R54] 比较两个文件
来源：http://ict.zhoulong.xyz

diff a.txt b.txt
来源：http://ydp.xinyue.icu

[R55] 压缩与解压
来源：http://abk.yvedp.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://xlh.ehwqpu.com

[R56] 远程拷贝
来源：http://pqk.hongshengwenyu.top

scp file user@host:/path/
来源：http://bji.xziqi.cn

[R57] 远程执行命令
来源：http://glg.52xcode.cn

ssh user@host 'uptime'
来源：http://hhv.zhengqikj.top

[R58] 下载文件
来源：http://dpa.hnxiangtu.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://nwm.0kj1m.cn

[R59] 发 POST JSON
来源：http://jys.guowangkeji.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://scs.ehwqpu.com

[R60] 只看 HTTP 状态码
来源：http://ugw.meibo888.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://aio.iojbl.cn

[R61] 磁盘占用
来源：http://vdb.zycfv.cn

df -h;  du -sh *
来源：http://pzj.aibaodan.cn

[R62] 找最占空间的文件
来源：http://ott.yuanzhike.top

du -ah . | sort -rh | head -10
来源：http://hyb.havefunace.top

[R63] 内存与进程
来源：http://vwz.cdnleiting.top

free -h;  ps aux | grep nginx
来源：http://chp.andypj.xyz

[R64] 结束进程
来源：http://phv.dashuyun.cn

kill -9 $(pgrep -f app.py)
来源：http://siv.dashuyun.cn

[R65] 查看端口占用
来源：http://mhz.jinghuilouyu.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://bas.jyoumei.cn

[R66] 定时任务
来源：http://ycx.jlsjyb.cn

crontab -e;  crontab -l
来源：http://guu.yj20258.top

[R67] 生成随机十六进制串
来源：http://ldc.hesvh.cn

openssl rand -hex 16
来源：http://mlz.fktsv.cn

[R68] 计算文件校验值
来源：http://biw.wangdashe.top

sha256sum a.txt;  md5sum a.txt
来源：http://gtv.ctjpmb.com

[R69] 生成随机密码
来源：http://jvl.hcnkem.com

head -c 16 /dev/urandom | base64
来源：http://ciu.xinyue.icu

[R70] 时间戳与互转
来源：http://wjr.jqgfzy.top

date +%s;  date -d @1700000000
来源：http://llq.dashuyun.cn

[R71] 日期格式化
来源：http://tyc.shanyushiyangkeji.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://xaj.vehdjk.com

[R72] 等待端口就绪
来源：http://kxn.kuanghao11.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://xnn.ydjk.org.cn

[R73] 分割大日志
来源：http://coh.kuanghao11.cn

split -l 1000 big.log part_
来源：http://dgk.hammf.cn

[R74] 批量重命名
来源：http://hrq.havefunace.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://lgk.meibo888.top

[R75] 导出环境变量
来源：http://sin.xylfe.cn

export PATH="$HOME/bin:$PATH"
来源：http://jlt.yanxiufei.cn

[R76] 使用临时文件
来源：http://dej.yvedp.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://srk.meibo888.top

[R77] 读取用户输入
来源：http://hxe.0kj1m.cn

read -rp "请输入: " ans
来源：http://xxp.zhoulong.xyz

[R78] 交互式菜单
来源：http://fuv.jqgfzy.top

select opt in a b c; do echo "$opt"; break; done
来源：http://dfs.zhongyouzk.top

[R79] 解析命令行选项
来源：http://gtc.sxryk.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://xsn.gzhubu.top

[R80] 查看脚本执行耗时
来源：http://sqr.zdbjq.cn

time ./run.sh
来源：http://pyq.hysaishi.cn

================================================================================
来源：http://dao.c1oappe.top

S. C / C++ 专题
来源：http://zyq.yueranfly.top

================================================================================
来源：http://arc.fktsv.cn

[S01] C：Hello World
来源：http://hou.redwolf501.top

#include <stdio.h>
来源：http://kib.hcnkem.com

int main(void) { printf("Hello\n"); return 0; }
来源：http://aqn.iojbl.cn

[S02] C：变量与格式化输出
来源：http://fag.zhoulong.xyz

int a = 10; printf("%d\n", a);
来源：http://eys.52xcode.cn

[S03] C：读入整数
来源：http://aww.zhixingplan.top

int x; scanf("%d", &x);
来源：http://ufl.cqqwz.cn

[S04] C：字符串复制
来源：http://osl.dianchejie.cn

char dst[32]; strcpy(dst, "hi");
来源：http://ooj.chenzaomai.com

[S05] C：字符串长度
来源：http://khs.ydzc1.top

strlen(s)
来源：http://jsg.chenjidiqi.icu

[S06] C：字符串比较
来源：http://unw.cheryme.top

strcmp(a, b) == 0
来源：http://lra.zhoulong.xyz

[S07] C：数组遍历求和
来源：http://uia.zhengqikj.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://dkn.vqdsnc.cn

[S08] C：动态内存分配与释放
来源：http://dnz.yj20258.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://tlb.tian-w.cn

[S09] C：结构体定义与初始化
来源：http://zdg.wangshuangyany.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://vlg.yangfankeji.com

[S10] C：指针与解引用
来源：http://rzw.aibaodan.cn

int *p = &a;  *p = 5;
来源：http://wju.0kj1m.cn

[S11] C：逐行读文件
来源：http://exp.fzhhl.top

FILE *f = fopen("a.txt", "r");
来源：http://whb.sweek.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://tql.yonumen.top

fclose(f);
来源：http://lnr.hysaishi.cn

[S12] C：写文件
来源：http://keb.ctjpmb.com

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://qae.zycfv.cn

[S13] C：宏定义
来源：http://jct.xuetiantiany.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://itm.ydzc1.top

[S14] C：枚举
来源：http://ngp.cashguo.top

enum Color { RED, GREEN, BLUE };
来源：http://zuw.tian-w.cn

[S15] C：类型转换
来源：http://kcx.jqgufenzy.top

(double) a / b
来源：http://fbt.yfazqb.com

[S16] C：位操作置位
来源：http://ioj.xuetiantiany.cn

x |= (1 << 3);
来源：http://whd.zdqjudy.top

[S17] C：安全拼接字符串
来源：http://myk.52xcode.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hnf.hysaishi.cn

[S18] C：命令行参数
来源：http://pxn.chenjidiqi.icu

int main(int argc, char **argv)
来源：http://pmr.yonumen.top

[S19] C：快速排序
来源：http://bif.yfazqb.com

qsort(a, n, sizeof(int), cmp);
来源：http://yjm.sxryk.cn

[S20] C：二分查找
来源：http://voy.hesvh.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://adl.shanyushiyangkeji.top

[S21] C：字符类别判断
来源：http://erz.daria6918.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://sbr.aizwys.cn

[S22] C：字符串转数字
来源：http://doi.jqgfzy.top

atoi("42");  strtod("3.14", NULL);
来源：http://tam.cheryme.top

[S23] C：随机数
来源：http://vfm.9152youxi.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://aio.xziqi.cn

[S24] C：获取本地时间
来源：http://onh.sxryk.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://akr.epnwcf.com

[S25] C：内存拷贝
来源：http://yec.zhongyouzk.top

memcpy(dst, src, n);
来源：http://njp.chenjidiqi.icu

[S26] C：内存清零
来源：http://wwu.yj20258.top

memset(a, 0, sizeof a);
来源：http://vbz.c1oappe.top

[S27] C：定义常量
来源：http://fcb.9152youxi.cn

const double PI = 3.14159;
来源：http://foh.gzhubu.top

[S28] C：静态变量
来源：http://say.zycfv.cn

static int counter = 0;
来源：http://viu.sxryk.cn

[S29] C：变参函数
来源：http://ohb.dashuyun.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://ayx.dashuyun.cn

[S30] C：头文件保护
来源：http://aei.cheryme.top

#ifndef X_H
来源：http://jhn.jinghuilouyu.cn

#define X_H
来源：http://ltp.hywenlv.cn

#endif
来源：http://mlx.316326.xyz

[S31] C++：Hello World
来源：http://crq.hywenlv.cn

#include <iostream>
来源：http://snt.shuidangran.top

int main() { std::cout << "Hello\n"; }
来源：http://jgu.wangdashe.top

[S32] C++：字符串
来源：http://eyj.daxiang520.top

std::string s = "hi";  s += "!";
来源：http://guu.quarkkingdee.top

[S33] C++：vector 增删
来源：http://qte.andypj.xyz

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://ltq.zhongyouzk.top

[S34] C++：遍历 vector
来源：http://omq.fktsv.cn

for (auto &x : v) { std::cout << x; }
来源：http://vpl.sxryk.cn

[S35] C++：map
来源：http://kjy.daria6918.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://kyy.hfpthk.cn

[S36] C++：unordered_map
来源：http://iea.tian-w.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://ffw.shzxlz.cn

[S37] C++：set
来源：http://nck.aizwys.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://dmx.hywenlv.cn

[S38] C++：排序
来源：http://jhs.yueranfly.top

std::sort(v.begin(), v.end());
来源：http://ksh.tianlin.xyz

[S39] C++：自定义比较器排序
来源：http://mtb.havefunace.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://ffp.ywan-chungtsiang.top

[S40] C++：查找元素
来源：http://fcx.iojbl.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://wan.yuanzhike.top

[S41] C++：类与构造函数
来源：http://ymm.daxiang520.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://ryc.shzxlz.cn

[S42] C++：继承与虚函数
来源：http://iaw.andypj.xyz

class B : public Base { public: void f() override {} };
来源：http://cfg.c1oappe.top

[S43] C++：智能指针
来源：http://whr.shanyushiyangtech.top

auto p = std::make_unique<int>(5);
来源：http://cbc.ydjk.org.cn

[S44] C++：引用传参
来源：http://ysx.jinyuanbaomall.cn

void inc(int &x) { ++x; }
来源：http://bzs.yuanzhike.top

[S45] C++：lambda
来源：http://gws.snrcjt.cn

auto add = [](int a, int b) { return a + b; };
来源：http://pad.jqgufenzy.top

[S46] C++：函数模板
来源：http://eqj.jlsjyb.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://acv.haohaochexian.top

[S47] C++：结构化绑定遍历
来源：http://yfk.birdmap.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://aiy.xuetiantiany.cn

[S48] C++：逐行读文件
来源：http://gfu.hfpthk.cn

std::ifstream in("a.txt");  std::string line;
来源：http://bgs.vehdjk.com

while (std::getline(in, line)) { }
来源：http://mxm.yueranfly.top

[S49] C++：写文件
来源：http://hit.zdqjudy.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://che.nanxinkj.top

[S50] C++：格式化数字
来源：http://jnd.ppjwa.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://jjy.fktsv.cn

[S51] C++：显式类型转换
来源：http://pur.jqgfzy.top

static_cast<double>(a) / b
来源：http://wvm.yonumen.top

[S52] C++：const 与 noexcept
来源：http://dxd.xuanzx.com

int size() const noexcept { return n_; }
来源：http://hcn.aibaodan.cn

[S53] C++：移动语义
来源：http://puu.hywenlv.cn

std::vector<int> w = std::move(v);
来源：http://bqo.bjfxy.top

[S54] C++：异常处理
来源：http://vcq.fanxiaobao.xyz

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://stb.haohaochexian.top

[S55] C++：结构化绑定
来源：http://pmr.ivvv.top

auto [a, b] = std::make_pair(1, 2);
来源：http://hev.zdbjq.cn

[S56] C++：optional
来源：http://fub.uphjek.com

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://nhd.yj202588.top

[S57] C++：编译期常量
来源：http://yah.daria6918.cn

constexpr int N = 10;
来源：http://qqy.gotoacloud.top

[S58] C++：命名空间
来源：http://rdq.sysykeji.top


<!-- 参考信息 -->