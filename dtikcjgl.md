代发 wailian999

[Q88] 行转列（条件聚合）
来源：http://tjz.cqqwz.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://rzm.wangshuangyany.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://zbi.nanxinkj.top

[Q89] 判断表是否存在
来源：http://ief.jqgfzy.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://mlw.zhoulong.xyz

[Q90] 生成序号列
来源：http://naw.fehbvm.com

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://rzy.ivvv.top

================================================================================
来源：http://pfl.hywenlv.cn

R. Bash 专题
来源：http://ugw.uphjek.com

================================================================================
来源：http://hxk.316326.xyz

[R01] shebang 与严格模式
来源：http://vef.nwbrower.top

#!/usr/bin/env bash
来源：http://qpe.hnqzz.top

set -euo pipefail
来源：http://fsz.ivvv.top

[R02] 变量赋值与使用
来源：http://bxj.snrcjt.cn

name="Tom"; echo "$name"
来源：http://mvk.yfazqb.com

[R03] 只读变量
来源：http://sqp.ydjk.org.cn

readonly PI=3.14
来源：http://vrt.shuidangran.top

[R04] 位置参数
来源：http://zwu.chenlongwang.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://yvr.fengsongda.top

[R05] 参数默认值
来源：http://jgy.yfazqb.com

name="${1:-default}"
来源：http://fns.shanyushiyangkeji.top

[R06] 判断命令是否存在
来源：http://fqx.ywan-chungtsiang.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://ezj.gaohongyu789.top

[R07] if 判断文件
来源：http://zxt.smart0.xyz

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://kxv.yangfankeji.com

[R08] 数值比较
来源：http://oeb.xingfuxueyuan.xyz

if (( a > b )); then echo "a 更大"; fi
来源：http://vwy.c1oappe.top

[R09] 字符串比较
来源：http://gbu.0kj1m.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://yhc.ivvv.top

[R10] 正则匹配
来源：http://ocn.zhoulong.xyz

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://tzz.ehwqpu.com

[R11] case 多分支
来源：http://sje.ydzc1.top

case "$1" in
来源：http://qmn.aizwys.cn

start) echo "启动" ;;
来源：http://yeq.bjfxy.top

stop)  echo "停止" ;;
来源：http://zla.xylfe.cn

*)     echo "未知命令" ;;
来源：http://tkl.wangshuangyany.cn

esac
来源：http://ypt.fengsongda.top

[R12] for 遍历文件
来源：http://dfb.yongpay.top

for f in *.txt; do echo "$f"; done
来源：http://xbu.ctjpmb.com

[R13] for 计数循环
来源：http://wub.yangfankeji.com

for i in {1..10}; do echo "$i"; done
来源：http://mmf.meibo888.top

[R14] C 风格 for
来源：http://iwq.xinyue.icu

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://vgo.zhaomingkeji.xyz

[R15] while 逐行读文件
来源：http://amx.pengpengdd.cyou

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://loj.bjfxy.top

[R16] until 等待条件
来源：http://yhq.yueranfly.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://nrx.dianchejie.cn

[R17] 数组定义与取值
来源：http://gkj.zycfv.cn

arr=(a b c); echo "${arr[0]}"
来源：http://rzs.yonumen.top

[R18] 遍历数组
来源：http://ddi.ppjwa.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://yqq.shuidangran.top

[R19] 数组长度
来源：http://uxv.yvedp.cn

echo "${#arr[@]}"
来源：http://ddm.jianghu66.top

[R20] 关联数组（字典）
来源：http://cya.yongpay.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://jlw.gzhubu.top

[R21] 字符串长度
来源：http://juo.wangdashe.top

echo "${#s}"
来源：http://rra.sjlbkw.cn

[R22] 截取子串
来源：http://xee.hysaishi.cn

echo "${s:0:5}"
来源：http://uqi.vqdsnc.cn

[R23] 字符串替换
来源：http://hha.jlsjyb.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://rhs.zhengqikj.top

[R24] 大小写转换
来源：http://ifc.jianghu66.top

echo "${s^^}"; echo "${s,,}"
来源：http://urp.vehdjk.com

[R25] 去后缀 / 去前缀
来源：http://iyy.gogol.net.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://ldv.ywan-chungtsiang.top

[R26] 命令替换
来源：http://uli.ywan-chungtsiang.top

now=$(date +%F); echo "$now"
来源：http://csj.pengpengdd.cyou

[R27] 算术展开
来源：http://ead.tanke756.top

echo $((1 + 2 * 3))
来源：http://fwy.tanke756.top

[R28] 浮点运算
来源：http://rfq.chenlongwang.top

echo "scale=2; 10/3" | bc
来源：http://hjq.smart0.xyz

[R29] 定义函数
来源：http://rov.yangfankeji.com

add() { echo $(($1 + $2)); }; add 1 2
来源：http://llz.chenzaomai.com

[R30] 函数返回状态码
来源：http://syh.iojbl.cn

f() { return 0; }; f || echo "失败了"
来源：http://nlz.meibo888.top

[R31] 局部变量
来源：http://uuu.dianchejie.cn

f() { local x=1; echo "$x"; }
来源：http://pdl.zycfv.cn

[R32] 参数个数校验
来源：http://fmw.smart0.xyz

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://atu.chenjidiqi.icu

[R33] 捕获错误并提示行号
来源：http://wdq.feifeiyinyue.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://sth.zhongyouzk.top

[R34] 退出时清理
来源：http://mvs.fengsongda.top

trap 'rm -f "$tmp"' EXIT
来源：http://jrg.jinyuanbaomall.cn

[R35] 后台执行并等待
来源：http://hvb.vehdjk.com

sleep 5 & pid=$!; wait "$pid"
来源：http://lxo.sweek.top

[R36] 并发执行多个任务
来源：http://ygn.aibaodan.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://oba.hcnkem.com

[R37] 把输出赋给变量
来源：http://fko.yvedp.cn

files=$(ls -1)
来源：http://fyq.zhongyouzk.top

[R38] 管道串联
来源：http://fci.birdmap.top

cat a.txt | grep -i error | wc -l
来源：http://nze.vehdjk.com

[R39] 重定向标准输出与错误
来源：http://unc.jinghuilouyu.cn

cmd > out.log 2>&1
来源：http://umz.hongshengwenyu.top

[R40] 追加写日志
来源：http://yme.jlsjyb.cn

echo "log" >> out.log
来源：http://glb.zhengqikj.top

[R41] 丢弃输出
来源：http://kds.xuetiantiany.cn

cmd >/dev/null 2>&1
来源：http://nht.kuanghao11.cn

[R42] 输入重定向
来源：http://vqb.daria6918.cn

wc -l < a.txt
来源：http://ypv.zhengqikj.top

[R43] 按名字查找文件
来源：http://kar.sweek.top

find . -name "*.log" -type f
来源：http://tdr.shanyushiyangkeji.top

[R44] 按修改时间查找
来源：http://fap.iojbl.cn

find . -mtime -7 -type f
来源：http://mpu.yvedp.cn

[R45] 批量删除
来源：http://iwe.shuidangran.top

find . -name "*.tmp" -delete
来源：http://czh.ydjk.org.cn

[R46] 递归替换文件内容
来源：http://okm.andypj.xyz

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://tah.316326.xyz

[R47] sed 单行替换
来源：http://rpy.ehwqpu.com

sed -i 's/foo/bar/g' a.txt
来源：http://xbb.ydzc1.top

[R48] awk 取指定列
来源：http://jws.dashuyun.cn

awk '{print $1, $3}' a.txt
来源：http://ysx.cashguo.top

[R49] awk 带条件
来源：http://nfe.jqgufenzy.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://klz.hcnkem.com

[R50] awk 求和
来源：http://vqw.andypj.xyz

awk '{s += $2} END {print s}' a.txt
来源：http://phn.hammf.cn

[R51] 排序去重取前几
来源：http://mah.fzhhl.top

sort a.txt | uniq -c | sort -rn | head
来源：http://mnz.ivvv.top

[R52] 统计行数
来源：http://clq.fehbvm.com

wc -l a.txt
来源：http://pwy.shanyushiyangtech.top

[R53] 查看文件头与实时尾
来源：http://xsb.zhixingplan.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://dqj.zhixingplan.top

[R54] 比较两个文件
来源：http://csd.yj202588.top

diff a.txt b.txt
来源：http://kru.redwolf501.top

[R55] 压缩与解压
来源：http://xqy.pengpengdd.cyou

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hhv.chenzaomai.com

[R56] 远程拷贝
来源：http://qfe.hcnkem.com

scp file user@host:/path/
来源：http://wsv.quarkkingdee.top

[R57] 远程执行命令
来源：http://luu.zhengqikj.top

ssh user@host 'uptime'
来源：http://bzu.guowangkeji.top

[R58] 下载文件
来源：http://ktf.feifeiyinyue.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://wds.yangfankeji.com

[R59] 发 POST JSON
来源：http://ezi.sysykeji.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://mca.cdnleiting.top

[R60] 只看 HTTP 状态码
来源：http://hur.jianghu66.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://ocy.chenjidiqi.icu

[R61] 磁盘占用
来源：http://hdh.yvedp.cn

df -h;  du -sh *
来源：http://twp.aibaodan.cn

[R62] 找最占空间的文件
来源：http://guz.redwolf501.top

du -ah . | sort -rh | head -10
来源：http://wwo.yuxming.cn

[R63] 内存与进程
来源：http://jou.hongshengwenyu.top

free -h;  ps aux | grep nginx
来源：http://knz.jinqigufen.top

[R64] 结束进程
来源：http://hpm.aibaodan.cn

kill -9 $(pgrep -f app.py)
来源：http://guw.ywan-chungtsiang.top

[R65] 查看端口占用
来源：http://gpr.gaohongyu789.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://xhs.cucudq.cn

[R66] 定时任务
来源：http://mid.shanyushiyangkeji.top

crontab -e;  crontab -l
来源：http://jhg.chenzaomai.com

[R67] 生成随机十六进制串
来源：http://ugf.tianlin.xyz

openssl rand -hex 16
来源：http://cwq.yonumen.top

[R68] 计算文件校验值
来源：http://zcy.feifeiyinyue.top

sha256sum a.txt;  md5sum a.txt
来源：http://rmm.hcnkem.com

[R69] 生成随机密码
来源：http://vxx.hesvh.cn

head -c 16 /dev/urandom | base64
来源：http://qhu.meibo888.top

[R70] 时间戳与互转
来源：http://zml.ehwqpu.com

date +%s;  date -d @1700000000
来源：http://dmy.c1oappe.top

[R71] 日期格式化
来源：http://reg.zhixingplan.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://snh.yongpay.top

[R72] 等待端口就绪
来源：http://raw.jqgufenzy.top

until nc -z localhost 3306; do sleep 1; done
来源：http://njs.cucudq.cn

[R73] 分割大日志
来源：http://pmn.cheryme.top

split -l 1000 big.log part_
来源：http://icg.chenzaomai.com

[R74] 批量重命名
来源：http://ttd.zdbjq.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://srv.fzhhl.top

[R75] 导出环境变量
来源：http://cey.sxryk.cn

export PATH="$HOME/bin:$PATH"
来源：http://lck.gaohongyu789.top

[R76] 使用临时文件
来源：http://qob.epnwcf.com

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://skw.sjlbkw.cn

[R77] 读取用户输入
来源：http://cgw.wangshuangyany.cn

read -rp "请输入: " ans
来源：http://mkw.xuetiantiany.cn

[R78] 交互式菜单
来源：http://mnz.ybcxt.top

select opt in a b c; do echo "$opt"; break; done
来源：http://des.hongshengwenyu.top

[R79] 解析命令行选项
来源：http://cqz.sysykeji.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://onq.jinyuanbaomall.cn

[R80] 查看脚本执行耗时
来源：http://ekt.sysykeji.top

time ./run.sh
来源：http://esv.yvedp.cn

================================================================================
来源：http://mkx.jlsjyb.cn

S. C / C++ 专题
来源：http://nuk.feifeiyinyue.top

================================================================================
来源：http://twa.tarul.cn

[S01] C：Hello World
来源：http://pja.yangfankeji.com

#include <stdio.h>
来源：http://fyx.zhengqikj.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://sqq.fktsv.cn

[S02] C：变量与格式化输出
来源：http://njm.yuanzhike.top

int a = 10; printf("%d\n", a);
来源：http://cvt.jiagoushi.top

[S03] C：读入整数
来源：http://fil.hongshengwenyu.top

int x; scanf("%d", &x);
来源：http://cdg.nwbrower.top

[S04] C：字符串复制
来源：http://ros.52xcode.cn

char dst[32]; strcpy(dst, "hi");
来源：http://ujc.jyoumei.cn

[S05] C：字符串长度
来源：http://yme.dianchejie.cn

strlen(s)
来源：http://grj.jinyuanbaomall.cn

[S06] C：字符串比较
来源：http://sfk.sxryk.cn

strcmp(a, b) == 0
来源：http://zuk.aizwys.cn

[S07] C：数组遍历求和
来源：http://rhx.aibaodan.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://vhl.yangfankeji.com

[S08] C：动态内存分配与释放
来源：http://ajs.uphjek.com

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://vju.chenjidiqi.icu

[S09] C：结构体定义与初始化
来源：http://lpm.wangshuangyany.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://kjf.ppjwa.cn

[S10] C：指针与解引用
来源：http://ckd.sxryk.cn

int *p = &a;  *p = 5;
来源：http://sye.fehbvm.com

[S11] C：逐行读文件
来源：http://ezj.jinghuilouyu.cn

FILE *f = fopen("a.txt", "r");
来源：http://fjd.shanyushiyangkeji.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://rbz.tanke756.top

fclose(f);
来源：http://ndd.meibo888.top

[S12] C：写文件
来源：http://nnw.0kj1m.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://dry.zdbjq.cn

[S13] C：宏定义
来源：http://laz.sysykeji.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://niq.yvedp.cn

[S14] C：枚举
来源：http://qmp.yueranfly.top

enum Color { RED, GREEN, BLUE };
来源：http://iii.yonumen.top

[S15] C：类型转换
来源：http://tuh.zhijiandao.cn

(double) a / b
来源：http://hzb.dianchejie.cn

[S16] C：位操作置位
来源：http://oak.gaohongyu789.top

x |= (1 << 3);
来源：http://bhz.daxiang520.top

[S17] C：安全拼接字符串
来源：http://hyj.jyoumei.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://ajz.yj20258888.top

[S18] C：命令行参数
来源：http://ltq.yj20258888.top

int main(int argc, char **argv)
来源：http://ucb.tian-w.cn

[S19] C：快速排序
来源：http://yxr.tanke756.top

qsort(a, n, sizeof(int), cmp);
来源：http://wsm.svipenyu.cn

[S20] C：二分查找
来源：http://ccd.gotoacloud.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://fey.zhaomingkeji.xyz

[S21] C：字符类别判断
来源：http://uvm.jinghuilouyu.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://gof.xuanzx.com

[S22] C：字符串转数字
来源：http://txi.yonumen.top

atoi("42");  strtod("3.14", NULL);
来源：http://upv.haohaochexian.top

[S23] C：随机数
来源：http://sia.chenlongwang.top

srand(time(NULL));  int r = rand() % 100;
来源：http://pyg.wangdashe.top

[S24] C：获取本地时间
来源：http://lvl.havefunace.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://auu.pycfn.com

[S25] C：内存拷贝
来源：http://bwn.shanyushiyangtech.top

memcpy(dst, src, n);
来源：http://zjl.ppjwa.cn

[S26] C：内存清零
来源：http://lln.hnxiangtu.top

memset(a, 0, sizeof a);
来源：http://sux.vehdjk.com

[S27] C：定义常量
来源：http://xdd.yj20258.top

const double PI = 3.14159;
来源：http://dsj.fktsv.cn

[S28] C：静态变量
来源：http://qca.zhengqikj.top

static int counter = 0;
来源：http://igy.zhiwuduotai.top

[S29] C：变参函数
来源：http://mbl.hammf.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://rmn.quarkkingdee.top

[S30] C：头文件保护
来源：http://rue.shanyushiyangtech.top

#ifndef X_H
来源：http://kuy.yangfankeji.com

#define X_H
来源：http://gwc.vehdjk.com

#endif
来源：http://jau.fehbvm.com

[S31] C++：Hello World
来源：http://epw.shangyingyoupin.top

#include <iostream>
来源：http://gao.tarul.cn

int main() { std::cout << "Hello\n"; }
来源：http://kpa.aibaodan.cn

[S32] C++：字符串
来源：http://zdj.yanxiufei.cn

std::string s = "hi";  s += "!";
来源：http://pxb.52xcode.cn

[S33] C++：vector 增删
来源：http://gbo.shangyingyoupin.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://cti.ydzc1.top

[S34] C++：遍历 vector
来源：http://pbi.tian-w.cn

for (auto &x : v) { std::cout << x; }
来源：http://vew.hcnkem.com

[S35] C++：map
来源：http://eah.svipenyu.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://plh.jiagoushi.top

[S36] C++：unordered_map
来源：http://bum.jqgufenzy.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://ohs.sufxvd.cn

[S37] C++：set
来源：http://ynn.shangyingyoupin.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hah.pycfn.com

[S38] C++：排序
来源：http://kan.zhoulong.xyz

std::sort(v.begin(), v.end());
来源：http://eew.jyoumei.cn

[S39] C++：自定义比较器排序
来源：http://sxb.meibo888.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://nxf.shzxlz.cn

[S40] C++：查找元素
来源：http://ito.bjfxy.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://izu.c1oappe.top

[S41] C++：类与构造函数
来源：http://ilu.xuanzx.com

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://yvo.xylfe.cn

[S42] C++：继承与虚函数
来源：http://kpc.xuetiantiany.cn

class B : public Base { public: void f() override {} };
来源：http://yoa.fanxiaobao.xyz

[S43] C++：智能指针
来源：http://vxn.316326.xyz

auto p = std::make_unique<int>(5);
来源：http://bbm.yongpay.top

[S44] C++：引用传参
来源：http://lqd.hysaishi.cn

void inc(int &x) { ++x; }
来源：http://lvk.cdnleiting.top

[S45] C++：lambda
来源：http://ero.zhoulong.xyz

auto add = [](int a, int b) { return a + b; };
来源：http://fqa.ybcxt.top

[S46] C++：函数模板
来源：http://phb.zhiwuduotai.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://qvv.sxryk.cn

[S47] C++：结构化绑定遍历
来源：http://trv.dianchejie.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://kgq.zhixingplan.top

[S48] C++：逐行读文件
来源：http://kvo.xingfuxueyuan.xyz

std::ifstream in("a.txt");  std::string line;
来源：http://mma.jyoumei.cn

while (std::getline(in, line)) { }
来源：http://low.jiagoushi.top

[S49] C++：写文件
来源：http://azb.tanke756.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://kfl.havefunace.top

[S50] C++：格式化数字
来源：http://fjl.fanxiaobao.xyz

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://iub.cdnleiting.top

[S51] C++：显式类型转换
来源：http://jqs.0kj1m.cn

static_cast<double>(a) / b
来源：http://imq.cheryme.top

[S52] C++：const 与 noexcept
来源：http://hpm.tanke756.top

int size() const noexcept { return n_; }
来源：http://lah.zycfv.cn

[S53] C++：移动语义
来源：http://hpi.jinqigufen.top

std::vector<int> w = std::move(v);
来源：http://pbv.bjfxy.top

[S54] C++：异常处理
来源：http://vfs.chenjidiqi.icu

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://cgz.yvedp.cn

[S55] C++：结构化绑定
来源：http://phu.cheryme.top

auto [a, b] = std::make_pair(1, 2);
来源：http://xgu.jinqigfzy.top

[S56] C++：optional
来源：http://qzf.zhoulong.xyz

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://see.zycfv.cn

[S57] C++：编译期常量
来源：http://xpf.aizwys.cn

constexpr int N = 10;
来源：http://kyr.ivvv.top

[S58] C++：命名空间
来源：http://znn.jinyuanbaomall.cn


<!-- 参考信息 -->