代发 wailian999

R. Bash 专题
来源：http://ndo.hcnkem.com

================================================================================
来源：http://drv.yuxming.cn

[R01] shebang 与严格模式
来源：http://zun.yfazqb.com

#!/usr/bin/env bash
来源：http://bjm.vqdsnc.cn

set -euo pipefail
来源：http://hkt.316326.xyz

[R02] 变量赋值与使用
来源：http://qaq.haohaochexian.top

name="Tom"; echo "$name"
来源：http://vie.yongpay.top

[R03] 只读变量
来源：http://ogw.tian-w.cn

readonly PI=3.14
来源：http://huw.jinqigufen.top

[R04] 位置参数
来源：http://zjo.daxiang520.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://mpt.svipenyu.cn

[R05] 参数默认值
来源：http://xzc.shzxlz.cn

name="${1:-default}"
来源：http://oxs.wangdashe.top

[R06] 判断命令是否存在
来源：http://eyd.hfpthk.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://eji.pengpengdd.cyou

[R07] if 判断文件
来源：http://knv.vqdsnc.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://jjj.uphjek.com

[R08] 数值比较
来源：http://zen.sufxvd.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://jkv.shuidangran.top

[R09] 字符串比较
来源：http://bac.zhoulong.xyz

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://ejg.ppjwa.cn

[R10] 正则匹配
来源：http://nbd.zycfv.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://iag.fehbvm.com

[R11] case 多分支
来源：http://lla.xuanzx.com

case "$1" in
来源：http://nvt.ywan-chungtsiang.top

start) echo "启动" ;;
来源：http://imx.epnwcf.com

stop)  echo "停止" ;;
来源：http://qjs.yuxming.cn

*)     echo "未知命令" ;;
来源：http://lhb.fehbvm.com

esac
来源：http://euo.tianlin.xyz

[R12] for 遍历文件
来源：http://mgd.daxiang520.top

for f in *.txt; do echo "$f"; done
来源：http://mig.fanxiaobao.xyz

[R13] for 计数循环
来源：http://lhx.jinqigufen.top

for i in {1..10}; do echo "$i"; done
来源：http://itc.shangyingyoupin.top

[R14] C 风格 for
来源：http://rey.nwbrower.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://tub.ydzc1.top

[R15] while 逐行读文件
来源：http://pij.zhengqikj.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://ozr.fktsv.cn

[R16] until 等待条件
来源：http://wsv.yonumen.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://wne.smart0.xyz

[R17] 数组定义与取值
来源：http://ifb.hammf.cn

arr=(a b c); echo "${arr[0]}"
来源：http://ais.fengsongda.top

[R18] 遍历数组
来源：http://nfw.zhixingplan.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://sze.tian-w.cn

[R19] 数组长度
来源：http://yeq.ehwqpu.com

echo "${#arr[@]}"
来源：http://mlm.hnxiangtu.top

[R20] 关联数组（字典）
来源：http://icd.vqdsnc.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://gvs.jinghuilouyu.cn

[R21] 字符串长度
来源：http://dbe.0kj1m.cn

echo "${#s}"
来源：http://iag.aizwys.cn

[R22] 截取子串
来源：http://nfv.hfpthk.cn

echo "${s:0:5}"
来源：http://brp.fengsongda.top

[R23] 字符串替换
来源：http://xns.dashuyun.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://fpk.bjfxy.top

[R24] 大小写转换
来源：http://lzr.bjfxy.top

echo "${s^^}"; echo "${s,,}"
来源：http://ysa.tarul.cn

[R25] 去后缀 / 去前缀
来源：http://zlj.yj20258.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://ptz.jqgfzy.top

[R26] 命令替换
来源：http://iud.hammf.cn

now=$(date +%F); echo "$now"
来源：http://gkq.ehwqpu.com

[R27] 算术展开
来源：http://ifu.jqgfzy.top

echo $((1 + 2 * 3))
来源：http://wvk.xuanzx.com

[R28] 浮点运算
来源：http://kdi.zdbjq.cn

echo "scale=2; 10/3" | bc
来源：http://wwc.andypj.xyz

[R29] 定义函数
来源：http://dfo.jinyuanbaomall.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://rbo.dianchejie.cn

[R30] 函数返回状态码
来源：http://wqs.c1oappe.top

f() { return 0; }; f || echo "失败了"
来源：http://ale.daria6918.cn

[R31] 局部变量
来源：http://hwg.shanyushiyangtech.top

f() { local x=1; echo "$x"; }
来源：http://hoa.fanxiaobao.xyz

[R32] 参数个数校验
来源：http://ygs.fzhhl.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://xuz.yonumen.top

[R33] 捕获错误并提示行号
来源：http://xpq.aibaodan.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://bqf.ehwqpu.com

[R34] 退出时清理
来源：http://tef.tarul.cn

trap 'rm -f "$tmp"' EXIT
来源：http://svc.hysaishi.cn

[R35] 后台执行并等待
来源：http://vjb.hcnkem.com

sleep 5 & pid=$!; wait "$pid"
来源：http://fvi.yuxming.cn

[R36] 并发执行多个任务
来源：http://urd.chenzaomai.com

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://pqp.vqdsnc.cn

[R37] 把输出赋给变量
来源：http://wtp.xingfuxueyuan.xyz

files=$(ls -1)
来源：http://aff.uphjek.com

[R38] 管道串联
来源：http://fef.cucudq.cn

cat a.txt | grep -i error | wc -l
来源：http://ivj.52xcode.cn

[R39] 重定向标准输出与错误
来源：http://qyl.zhengqikj.top

cmd > out.log 2>&1
来源：http://cdq.yanxiufei.cn

[R40] 追加写日志
来源：http://dkm.yvedp.cn

echo "log" >> out.log
来源：http://nlo.xuanzx.com

[R41] 丢弃输出
来源：http://fqs.dianchejie.cn

cmd >/dev/null 2>&1
来源：http://rwu.fktsv.cn

[R42] 输入重定向
来源：http://wyn.hywenlv.cn

wc -l < a.txt
来源：http://nqn.ppjwa.cn

[R43] 按名字查找文件
来源：http://lzr.jlsjyb.cn

find . -name "*.log" -type f
来源：http://rbh.fzhhl.top

[R44] 按修改时间查找
来源：http://qvx.zdqjudy.top

find . -mtime -7 -type f
来源：http://qlc.zhijiandao.cn

[R45] 批量删除
来源：http://unh.pengpengdd.cyou

find . -name "*.tmp" -delete
来源：http://mfl.ywan-chungtsiang.top

[R46] 递归替换文件内容
来源：http://jcy.aizwys.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://aun.tarul.cn

[R47] sed 单行替换
来源：http://cna.xingfuxueyuan.xyz

sed -i 's/foo/bar/g' a.txt
来源：http://aex.ydjk.org.cn

[R48] awk 取指定列
来源：http://tra.xuanzx.com

awk '{print $1, $3}' a.txt
来源：http://ier.chenlongwang.top

[R49] awk 带条件
来源：http://kox.jinghuilouyu.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://gmv.dianchejie.cn

[R50] awk 求和
来源：http://slx.chenzaomai.com

awk '{s += $2} END {print s}' a.txt
来源：http://npv.fehbvm.com

[R51] 排序去重取前几
来源：http://vqx.tian-w.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://xwu.ywan-chungtsiang.top

[R52] 统计行数
来源：http://azd.feifeiyinyue.top

wc -l a.txt
来源：http://svn.dashuyun.cn

[R53] 查看文件头与实时尾
来源：http://crs.yj20258.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://rpg.hnqzz.top

[R54] 比较两个文件
来源：http://mzo.jlsjyb.cn

diff a.txt b.txt
来源：http://joj.ctjpmb.com

[R55] 压缩与解压
来源：http://xdb.hnxiangtu.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://bvo.ydjk.org.cn

[R56] 远程拷贝
来源：http://fvb.hammf.cn

scp file user@host:/path/
来源：http://rxc.guowangkeji.top

[R57] 远程执行命令
来源：http://mjv.jianghu66.top

ssh user@host 'uptime'
来源：http://xug.yj20258.top

[R58] 下载文件
来源：http://vmc.ywan-chungtsiang.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://ydw.zdbjq.cn

[R59] 发 POST JSON
来源：http://sik.pengpengdd.cyou

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://mvw.zdqjudy.top

[R60] 只看 HTTP 状态码
来源：http://bpk.shanyushiyangkeji.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://nzv.gogol.net.cn

[R61] 磁盘占用
来源：http://mzz.zhiwuduotai.top

df -h;  du -sh *
来源：http://iql.ybcxt.top

[R62] 找最占空间的文件
来源：http://hli.ppjwa.cn

du -ah . | sort -rh | head -10
来源：http://avp.haohaochexian.top

[R63] 内存与进程
来源：http://ipg.jyoumei.cn

free -h;  ps aux | grep nginx
来源：http://lfv.fktsv.cn

[R64] 结束进程
来源：http://whn.haohaochexian.top

kill -9 $(pgrep -f app.py)
来源：http://vhk.aibaodan.cn

[R65] 查看端口占用
来源：http://tan.jinghuilouyu.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://cup.feifeiyinyue.top

[R66] 定时任务
来源：http://rlv.jlsjyb.cn

crontab -e;  crontab -l
来源：http://rdi.jlsjyb.cn

[R67] 生成随机十六进制串
来源：http://qgq.hammf.cn

openssl rand -hex 16
来源：http://fyd.epnwcf.com

[R68] 计算文件校验值
来源：http://gbc.jqgufenzy.top

sha256sum a.txt;  md5sum a.txt
来源：http://xne.jinyuanbaomall.cn

[R69] 生成随机密码
来源：http://kzq.guowangkeji.top

head -c 16 /dev/urandom | base64
来源：http://hvu.fehbvm.com

[R70] 时间戳与互转
来源：http://ndo.zhongyouzk.top

date +%s;  date -d @1700000000
来源：http://qco.shanyushiyangkeji.top

[R71] 日期格式化
来源：http://ulh.gotoacloud.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://zsm.yj20258.top

[R72] 等待端口就绪
来源：http://ouv.hnxiangtu.top

until nc -z localhost 3306; do sleep 1; done
来源：http://zoj.xuanzx.com

[R73] 分割大日志
来源：http://ojh.fehbvm.com

split -l 1000 big.log part_
来源：http://qvy.gotoacloud.top

[R74] 批量重命名
来源：http://jsz.fengsongda.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://wsw.andypj.xyz

[R75] 导出环境变量
来源：http://omb.gotoacloud.top

export PATH="$HOME/bin:$PATH"
来源：http://yby.kuanghao11.cn

[R76] 使用临时文件
来源：http://zbr.jqgufenzy.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://plc.jyoumei.cn

[R77] 读取用户输入
来源：http://guc.shzxlz.cn

read -rp "请输入: " ans
来源：http://tkt.0kj1m.cn

[R78] 交互式菜单
来源：http://dsc.jlsjyb.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://lki.jiagoushi.top

[R79] 解析命令行选项
来源：http://zwj.jyoumei.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://ghs.andypj.xyz

[R80] 查看脚本执行耗时
来源：http://cba.9152youxi.cn

time ./run.sh
来源：http://elc.316326.xyz

================================================================================
来源：http://boo.yj20258.top

S. C / C++ 专题
来源：http://fox.havefunace.top

================================================================================
来源：http://hej.hcnkem.com

[S01] C：Hello World
来源：http://vzv.daxiang520.top

#include <stdio.h>
来源：http://jdn.fktsv.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://lnj.andypj.xyz

[S02] C：变量与格式化输出
来源：http://sil.jinyuanbaomall.cn

int a = 10; printf("%d\n", a);
来源：http://iah.gzhubu.top

[S03] C：读入整数
来源：http://tay.wangdashe.top

int x; scanf("%d", &x);
来源：http://ohw.ydzc1.top

[S04] C：字符串复制
来源：http://uwg.zycfv.cn

char dst[32]; strcpy(dst, "hi");
来源：http://kup.jqgfzy.top

[S05] C：字符串长度
来源：http://vam.hnqzz.top

strlen(s)
来源：http://ncv.svipenyu.cn

[S06] C：字符串比较
来源：http://hya.hnxiangtu.top

strcmp(a, b) == 0
来源：http://hxc.316326.xyz

[S07] C：数组遍历求和
来源：http://mkj.sysykeji.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://jnn.hesvh.cn

[S08] C：动态内存分配与释放
来源：http://orz.aibaodan.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://sac.havefunace.top

[S09] C：结构体定义与初始化
来源：http://zbs.hcnkem.com

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://lmb.hammf.cn

[S10] C：指针与解引用
来源：http://iiv.chenlongwang.top

int *p = &a;  *p = 5;
来源：http://nfm.smart0.xyz

[S11] C：逐行读文件
来源：http://njz.xuanzx.com

FILE *f = fopen("a.txt", "r");
来源：http://jce.pycfn.com

while (fgets(buf, sizeof buf, f)) { }
来源：http://hhv.shanyushiyangtech.top

fclose(f);
来源：http://ubg.bbcook.cn

[S12] C：写文件
来源：http://nan.xziqi.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://iqa.fehbvm.com

[S13] C：宏定义
来源：http://auc.fktsv.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://oih.ywan-chungtsiang.top

[S14] C：枚举
来源：http://ldc.cdnleiting.top

enum Color { RED, GREEN, BLUE };
来源：http://dcx.cdnleiting.top

[S15] C：类型转换
来源：http://ust.zycfv.cn

(double) a / b
来源：http://ske.daxiang520.top

[S16] C：位操作置位
来源：http://gno.jinqigufen.top

x |= (1 << 3);
来源：http://eje.c1oappe.top

[S17] C：安全拼接字符串
来源：http://whq.hysaishi.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://zmd.nanxuanxn.top

[S18] C：命令行参数
来源：http://xdk.ydjk.org.cn

int main(int argc, char **argv)
来源：http://xgi.hongshengwenyu.top

[S19] C：快速排序
来源：http://rbj.pengpengdd.cyou

qsort(a, n, sizeof(int), cmp);
来源：http://vzh.xziqi.cn

[S20] C：二分查找
来源：http://bjv.cqqwz.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://rcz.aizwys.cn

[S21] C：字符类别判断
来源：http://zwo.gaohongyu789.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://rmf.fktsv.cn

[S22] C：字符串转数字
来源：http://ogj.andypj.xyz

atoi("42");  strtod("3.14", NULL);
来源：http://msv.pengpengdd.cyou

[S23] C：随机数
来源：http://ijy.bbcook.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://xsj.yangfankeji.com

[S24] C：获取本地时间
来源：http://kxw.9152youxi.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://lsj.yj202588.top

[S25] C：内存拷贝
来源：http://pxs.yvedp.cn

memcpy(dst, src, n);
来源：http://xbp.shzxlz.cn

[S26] C：内存清零
来源：http://sbg.bbcook.cn

memset(a, 0, sizeof a);
来源：http://mmi.sysykeji.top

[S27] C：定义常量
来源：http://qgi.dashuyun.cn

const double PI = 3.14159;
来源：http://yjx.hammf.cn

[S28] C：静态变量
来源：http://zdo.52xcode.cn

static int counter = 0;
来源：http://jti.vehdjk.com

[S29] C：变参函数
来源：http://nij.c1oappe.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://lty.zhixingplan.top

[S30] C：头文件保护
来源：http://kbs.yj20258.top

#ifndef X_H
来源：http://ujb.haohaochexian.top

#define X_H
来源：http://jhr.wangdashe.top

#endif
来源：http://jlb.yvedp.cn

[S31] C++：Hello World
来源：http://dyq.cqqwz.cn

#include <iostream>
来源：http://jmq.shanyushiyangtech.top

int main() { std::cout << "Hello\n"; }
来源：http://xkj.jqgufenzy.top

[S32] C++：字符串
来源：http://nly.snrcjt.cn

std::string s = "hi";  s += "!";
来源：http://usa.jinqigufen.top

[S33] C++：vector 增删
来源：http://oac.dianchejie.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://wcn.sxryk.cn

[S34] C++：遍历 vector
来源：http://bta.zhengqikj.top

for (auto &x : v) { std::cout << x; }
来源：http://scr.ybcxt.top

[S35] C++：map
来源：http://lzx.ybcxt.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://fol.birdmap.top

[S36] C++：unordered_map
来源：http://gti.tanke756.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://sqk.0kj1m.cn

[S37] C++：set
来源：http://kox.chenzaomai.com

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://dha.gzhubu.top

[S38] C++：排序
来源：http://fhw.jqgfzy.top

std::sort(v.begin(), v.end());
来源：http://sbr.epnwcf.com

[S39] C++：自定义比较器排序
来源：http://wlw.ybcxt.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://eoe.xinyue.icu

[S40] C++：查找元素
来源：http://juj.cashguo.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://qif.zhongyouzk.top

[S41] C++：类与构造函数
来源：http://fop.feifeiyinyue.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://ide.vehdjk.com

[S42] C++：继承与虚函数
来源：http://tdg.ybcxt.top

class B : public Base { public: void f() override {} };
来源：http://nbu.zdqjudy.top

[S43] C++：智能指针
来源：http://cuw.zdqjudy.top

auto p = std::make_unique<int>(5);
来源：http://tbv.sweek.top

[S44] C++：引用传参
来源：http://eij.yj20258.top

void inc(int &x) { ++x; }
来源：http://bej.tanke756.top

[S45] C++：lambda
来源：http://btu.nwbrower.top

auto add = [](int a, int b) { return a + b; };
来源：http://fmb.kuanghao11.cn

[S46] C++：函数模板
来源：http://hev.tianlin.xyz

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://jvj.havefunace.top

[S47] C++：结构化绑定遍历
来源：http://qtn.yj202588.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://dqh.fehbvm.com

[S48] C++：逐行读文件
来源：http://ogr.fzhhl.top

std::ifstream in("a.txt");  std::string line;
来源：http://bop.dianchejie.cn

while (std::getline(in, line)) { }
来源：http://qiw.shangyingyoupin.top

[S49] C++：写文件
来源：http://sfl.epnwcf.com

std::ofstream out("a.txt");  out << "hi\n";
来源：http://myi.smart0.xyz

[S50] C++：格式化数字
来源：http://kqk.tanke756.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://exj.dianchejie.cn

[S51] C++：显式类型转换
来源：http://pmv.cucudq.cn

static_cast<double>(a) / b
来源：http://zve.yueranfly.top

[S52] C++：const 与 noexcept
来源：http://mcu.nanxinkj.top

int size() const noexcept { return n_; }
来源：http://kov.aibaodan.cn

[S53] C++：移动语义
来源：http://ljk.ydzc1.top

std::vector<int> w = std::move(v);
来源：http://gje.nwbrower.top

[S54] C++：异常处理
来源：http://wmq.fzhhl.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://vfw.sufxvd.cn

[S55] C++：结构化绑定
来源：http://kls.vqdsnc.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://sah.yonumen.top

[S56] C++：optional
来源：http://lgl.uphjek.com

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wrm.gogol.net.cn

[S57] C++：编译期常量
来源：http://wji.sweek.top

constexpr int N = 10;
来源：http://ayc.ywan-chungtsiang.top

[S58] C++：命名空间
来源：http://ioa.havefunace.top

namespace ns { int f() { return 1; } }
来源：http://boq.yj202588.top

[S59] C++：静态断言
来源：http://rwr.andypj.xyz

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://csb.xuetiantiany.cn

[S60] C++：遍历并删除元素
来源：http://vym.yongpay.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://erm.ybcxt.top

================================================================================
来源：http://wbg.jqgfzy.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://ttj.cucudq.cn

================================================================================
来源：http://ruw.birdmap.top


<!-- 参考信息 -->