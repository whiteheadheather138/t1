代发 wailian999

R. Bash 专题
来源：http://kbt.feifeiyinyue.top

================================================================================
来源：http://rov.yj20258888.top

[R01] shebang 与严格模式
来源：http://flq.vqdsnc.cn

#!/usr/bin/env bash
来源：http://zfx.xuetiantiany.cn

set -euo pipefail
来源：http://ase.kuanghao11.cn

[R02] 变量赋值与使用
来源：http://djj.ydjk.org.cn

name="Tom"; echo "$name"
来源：http://djk.yj20258888.top

[R03] 只读变量
来源：http://tto.fehbvm.com

readonly PI=3.14
来源：http://lqb.snrcjt.cn

[R04] 位置参数
来源：http://vtg.jqgfzy.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://vtf.hammf.cn

[R05] 参数默认值
来源：http://wbc.dianchejie.cn

name="${1:-default}"
来源：http://dzt.uphjek.com

[R06] 判断命令是否存在
来源：http://pub.hfpthk.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://jqs.9152youxi.cn

[R07] if 判断文件
来源：http://etn.chenjidiqi.icu

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://ker.yonumen.top

[R08] 数值比较
来源：http://sad.dianchejie.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://nmy.yanxiufei.cn

[R09] 字符串比较
来源：http://fjg.jinqigfzy.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://fsd.iojbl.cn

[R10] 正则匹配
来源：http://kdz.meibo888.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://osf.yfazqb.com

[R11] case 多分支
来源：http://xfr.fzhhl.top

case "$1" in
来源：http://sst.xziqi.cn

start) echo "启动" ;;
来源：http://ayd.yj20258.top

stop)  echo "停止" ;;
来源：http://cax.jqgfzy.top

*)     echo "未知命令" ;;
来源：http://xas.quarkkingdee.top

esac
来源：http://nlu.sufxvd.cn

[R12] for 遍历文件
来源：http://mdc.chenjidiqi.icu

for f in *.txt; do echo "$f"; done
来源：http://jaa.fktsv.cn

[R13] for 计数循环
来源：http://ikq.wangdashe.top

for i in {1..10}; do echo "$i"; done
来源：http://xxi.ehwqpu.com

[R14] C 风格 for
来源：http://ake.sufxvd.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://ngt.shuidangran.top

[R15] while 逐行读文件
来源：http://ohf.jinghuilouyu.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://uik.bbcook.cn

[R16] until 等待条件
来源：http://kmx.yvedp.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://eam.yongpay.top

[R17] 数组定义与取值
来源：http://oge.tarul.cn

arr=(a b c); echo "${arr[0]}"
来源：http://xxy.birdmap.top

[R18] 遍历数组
来源：http://lyz.hnxiangtu.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://wlr.yj20258888.top

[R19] 数组长度
来源：http://fsv.sysykeji.top

echo "${#arr[@]}"
来源：http://sil.fehbvm.com

[R20] 关联数组（字典）
来源：http://svd.vehdjk.com

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://woo.meibo888.top

[R21] 字符串长度
来源：http://faj.zdbjq.cn

echo "${#s}"
来源：http://zrv.cashguo.top

[R22] 截取子串
来源：http://drl.xingfuxueyuan.xyz

echo "${s:0:5}"
来源：http://vvt.sysykeji.top

[R23] 字符串替换
来源：http://mvf.jqgfzy.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://ija.epnwcf.com

[R24] 大小写转换
来源：http://zji.jqgfzy.top

echo "${s^^}"; echo "${s,,}"
来源：http://sdj.hnqzz.top

[R25] 去后缀 / 去前缀
来源：http://vhl.yuxming.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://kej.cheryme.top

[R26] 命令替换
来源：http://ewh.guannengcc.top

now=$(date +%F); echo "$now"
来源：http://kwa.jlsjyb.cn

[R27] 算术展开
来源：http://mvt.zhaomingkeji.xyz

echo $((1 + 2 * 3))
来源：http://qfy.shanyushiyangkeji.top

[R28] 浮点运算
来源：http://veo.xingfuxueyuan.xyz

echo "scale=2; 10/3" | bc
来源：http://sjx.pengpengdd.cyou

[R29] 定义函数
来源：http://xys.snrcjt.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://nml.xingfuxueyuan.xyz

[R30] 函数返回状态码
来源：http://wxn.tianlin.xyz

f() { return 0; }; f || echo "失败了"
来源：http://avx.sufxvd.cn

[R31] 局部变量
来源：http://xwl.xinyue.icu

f() { local x=1; echo "$x"; }
来源：http://pfj.kuanghao11.cn

[R32] 参数个数校验
来源：http://mhp.shangyingyoupin.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://vfi.birdmap.top

[R33] 捕获错误并提示行号
来源：http://sbj.sweek.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://bhv.sjlbkw.cn

[R34] 退出时清理
来源：http://rky.tian-w.cn

trap 'rm -f "$tmp"' EXIT
来源：http://dna.yvedp.cn

[R35] 后台执行并等待
来源：http://tnt.kuanghao11.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://bbx.jinghuilouyu.cn

[R36] 并发执行多个任务
来源：http://btq.yueranfly.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://txe.iojbl.cn

[R37] 把输出赋给变量
来源：http://znj.xingfuxueyuan.xyz

files=$(ls -1)
来源：http://yee.svipenyu.cn

[R38] 管道串联
来源：http://qab.sjlbkw.cn

cat a.txt | grep -i error | wc -l
来源：http://kfq.fengsongda.top

[R39] 重定向标准输出与错误
来源：http://eio.xinyue.icu

cmd > out.log 2>&1
来源：http://mzz.guannengcc.top

[R40] 追加写日志
来源：http://dzg.fehbvm.com

echo "log" >> out.log
来源：http://wdt.cucudq.cn

[R41] 丢弃输出
来源：http://qcu.fehbvm.com

cmd >/dev/null 2>&1
来源：http://oes.chenjidiqi.icu

[R42] 输入重定向
来源：http://vvc.jinyuanbaomall.cn

wc -l < a.txt
来源：http://wak.sweek.top

[R43] 按名字查找文件
来源：http://mav.jinghuilouyu.cn

find . -name "*.log" -type f
来源：http://kdn.zycfv.cn

[R44] 按修改时间查找
来源：http://qih.jlsjyb.cn

find . -mtime -7 -type f
来源：http://tiv.nanxuanxn.top

[R45] 批量删除
来源：http://fda.yj20258888.top

find . -name "*.tmp" -delete
来源：http://hut.haohaochexian.top

[R46] 递归替换文件内容
来源：http://fdh.9152youxi.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://vxi.hfpthk.cn

[R47] sed 单行替换
来源：http://eti.wangdashe.top

sed -i 's/foo/bar/g' a.txt
来源：http://zgt.ehwqpu.com

[R48] awk 取指定列
来源：http://haw.316326.xyz

awk '{print $1, $3}' a.txt
来源：http://yct.zhaomingkeji.xyz

[R49] awk 带条件
来源：http://skt.zhengqikj.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://pki.pycfn.com

[R50] awk 求和
来源：http://dyy.svipenyu.cn

awk '{s += $2} END {print s}' a.txt
来源：http://pvu.gogol.net.cn

[R51] 排序去重取前几
来源：http://nhe.vehdjk.com

sort a.txt | uniq -c | sort -rn | head
来源：http://law.fzhhl.top

[R52] 统计行数
来源：http://gst.tian-w.cn

wc -l a.txt
来源：http://nvx.0kj1m.cn

[R53] 查看文件头与实时尾
来源：http://zuw.jinyuanbaomall.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://jad.fktsv.cn

[R54] 比较两个文件
来源：http://ave.xziqi.cn

diff a.txt b.txt
来源：http://ksh.hfpthk.cn

[R55] 压缩与解压
来源：http://xlf.yuxming.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://bdv.hywenlv.cn

[R56] 远程拷贝
来源：http://yyc.sxryk.cn

scp file user@host:/path/
来源：http://pyn.meibo888.top

[R57] 远程执行命令
来源：http://ndv.dashuyun.cn

ssh user@host 'uptime'
来源：http://yit.yj20258.top

[R58] 下载文件
来源：http://dlo.hongshengwenyu.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://wgv.bbcook.cn

[R59] 发 POST JSON
来源：http://ftv.yj20258888.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://mfx.zhoulong.xyz

[R60] 只看 HTTP 状态码
来源：http://bvo.cqqwz.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://tlw.dianchejie.cn

[R61] 磁盘占用
来源：http://zyj.fengsongda.top

df -h;  du -sh *
来源：http://qys.ehwqpu.com

[R62] 找最占空间的文件
来源：http://sho.xuanzx.com

du -ah . | sort -rh | head -10
来源：http://uar.gzhubu.top

[R63] 内存与进程
来源：http://nak.cucudq.cn

free -h;  ps aux | grep nginx
来源：http://nfa.chenzaomai.com

[R64] 结束进程
来源：http://uyv.fktsv.cn

kill -9 $(pgrep -f app.py)
来源：http://rrc.nanxuanxn.top

[R65] 查看端口占用
来源：http://hic.shzxlz.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://ynb.feifeiyinyue.top

[R66] 定时任务
来源：http://owh.ydzc1.top

crontab -e;  crontab -l
来源：http://yju.sysykeji.top

[R67] 生成随机十六进制串
来源：http://mml.ydzc1.top

openssl rand -hex 16
来源：http://jkg.yanxiufei.cn

[R68] 计算文件校验值
来源：http://vgh.xuetiantiany.cn

sha256sum a.txt;  md5sum a.txt
来源：http://alj.zhiwuduotai.top

[R69] 生成随机密码
来源：http://hlj.mhx1999.top

head -c 16 /dev/urandom | base64
来源：http://try.52xcode.cn

[R70] 时间戳与互转
来源：http://rjj.pycfn.com

date +%s;  date -d @1700000000
来源：http://urm.zdbjq.cn

[R71] 日期格式化
来源：http://ery.ehwqpu.com

date +"%Y-%m-%d %H:%M:%S"
来源：http://wpi.gaohongyu789.top

[R72] 等待端口就绪
来源：http://see.xuetiantiany.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://jqf.sjlbkw.cn

[R73] 分割大日志
来源：http://xrw.meibo888.top

split -l 1000 big.log part_
来源：http://oxo.daria6918.cn

[R74] 批量重命名
来源：http://rfv.hcnkem.com

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://lsu.sxryk.cn

[R75] 导出环境变量
来源：http://ocx.pengpengdd.cyou

export PATH="$HOME/bin:$PATH"
来源：http://dds.daxiang520.top

[R76] 使用临时文件
来源：http://cas.jqgfzy.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://woa.xingfuxueyuan.xyz

[R77] 读取用户输入
来源：http://sfx.smart0.xyz

read -rp "请输入: " ans
来源：http://wpy.chenlongwang.top

[R78] 交互式菜单
来源：http://gxo.shanyushiyangtech.top

select opt in a b c; do echo "$opt"; break; done
来源：http://vni.ydzc1.top

[R79] 解析命令行选项
来源：http://oqz.zhixingplan.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://uhn.yvedp.cn

[R80] 查看脚本执行耗时
来源：http://hhh.fzhhl.top

time ./run.sh
来源：http://ykq.shuidangran.top

================================================================================
来源：http://bhw.ivvv.top

S. C / C++ 专题
来源：http://svr.jlsjyb.cn

================================================================================
来源：http://zel.cashguo.top

[S01] C：Hello World
来源：http://vmd.guowangkeji.top

#include <stdio.h>
来源：http://kpo.zhijiandao.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://ncd.hywenlv.cn

[S02] C：变量与格式化输出
来源：http://krl.cheryme.top

int a = 10; printf("%d\n", a);
来源：http://bcy.gotoacloud.top

[S03] C：读入整数
来源：http://vhb.daxiang520.top

int x; scanf("%d", &x);
来源：http://rvw.aizwys.cn

[S04] C：字符串复制
来源：http://azp.fanxiaobao.xyz

char dst[32]; strcpy(dst, "hi");
来源：http://vxy.quarkkingdee.top

[S05] C：字符串长度
来源：http://mff.yonumen.top

strlen(s)
来源：http://lmc.gzhubu.top

[S06] C：字符串比较
来源：http://vwc.pengpengdd.cyou

strcmp(a, b) == 0
来源：http://ukd.jyoumei.cn

[S07] C：数组遍历求和
来源：http://xiy.jinyuanbaomall.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://vtn.zhiwuduotai.top

[S08] C：动态内存分配与释放
来源：http://ygh.chenlongwang.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://ola.0kj1m.cn

[S09] C：结构体定义与初始化
来源：http://aih.vqdsnc.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://ais.ppjwa.cn

[S10] C：指针与解引用
来源：http://mtg.ctjpmb.com

int *p = &a;  *p = 5;
来源：http://iar.316326.xyz

[S11] C：逐行读文件
来源：http://hqt.fengsongda.top

FILE *f = fopen("a.txt", "r");
来源：http://mpd.tianlin.xyz

while (fgets(buf, sizeof buf, f)) { }
来源：http://rqi.fehbvm.com

fclose(f);
来源：http://qai.xingfuxueyuan.xyz

[S12] C：写文件
来源：http://fjz.jinyuanbaomall.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://uly.zhengqikj.top

[S13] C：宏定义
来源：http://fqp.yongpay.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://bit.chenjidiqi.icu

[S14] C：枚举
来源：http://mcs.birdmap.top

enum Color { RED, GREEN, BLUE };
来源：http://oge.pycfn.com

[S15] C：类型转换
来源：http://jsk.fanxiaobao.xyz

(double) a / b
来源：http://vyp.pengpengdd.cyou

[S16] C：位操作置位
来源：http://pxi.9152youxi.cn

x |= (1 << 3);
来源：http://szo.zhiwuduotai.top

[S17] C：安全拼接字符串
来源：http://jdl.feifeiyinyue.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://rnw.hesvh.cn

[S18] C：命令行参数
来源：http://prh.yuxming.cn

int main(int argc, char **argv)
来源：http://rff.jqgfzy.top

[S19] C：快速排序
来源：http://qds.yfazqb.com

qsort(a, n, sizeof(int), cmp);
来源：http://bmo.zhijiandao.cn

[S20] C：二分查找
来源：http://tjb.gzhubu.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://ttj.shanyushiyangtech.top

[S21] C：字符类别判断
来源：http://gwl.zycfv.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://jyn.quarkkingdee.top

[S22] C：字符串转数字
来源：http://lvz.sxryk.cn

atoi("42");  strtod("3.14", NULL);
来源：http://lyq.hywenlv.cn

[S23] C：随机数
来源：http://zxo.kuanghao11.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://zea.zhoulong.xyz

[S24] C：获取本地时间
来源：http://npr.yj20258888.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://xmj.shuidangran.top

[S25] C：内存拷贝
来源：http://ami.hammf.cn

memcpy(dst, src, n);
来源：http://hjw.c1oappe.top

[S26] C：内存清零
来源：http://vsv.nwbrower.top

memset(a, 0, sizeof a);
来源：http://gux.meibo888.top

[S27] C：定义常量
来源：http://ydv.redwolf501.top

const double PI = 3.14159;
来源：http://uqf.nanxinkj.top

[S28] C：静态变量
来源：http://suk.yanxiufei.cn

static int counter = 0;
来源：http://ein.sweek.top

[S29] C：变参函数
来源：http://dac.tarul.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://sgh.kuanghao11.cn

[S30] C：头文件保护
来源：http://qlz.birdmap.top

#ifndef X_H
来源：http://fiu.xingfuxueyuan.xyz

#define X_H
来源：http://ord.yonumen.top

#endif
来源：http://ihn.gogol.net.cn

[S31] C++：Hello World
来源：http://sps.gotoacloud.top

#include <iostream>
来源：http://muy.havefunace.top

int main() { std::cout << "Hello\n"; }
来源：http://egg.ivvv.top

[S32] C++：字符串
来源：http://hpw.chenjidiqi.icu

std::string s = "hi";  s += "!";
来源：http://qca.52xcode.cn

[S33] C++：vector 增删
来源：http://ryb.yuxming.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://fsj.andypj.xyz

[S34] C++：遍历 vector
来源：http://oyn.bjfxy.top

for (auto &x : v) { std::cout << x; }
来源：http://teg.nwbrower.top

[S35] C++：map
来源：http://sus.hfpthk.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://ijs.yj20258.top

[S36] C++：unordered_map
来源：http://ebc.hfpthk.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://ltl.cashguo.top

[S37] C++：set
来源：http://jpl.ivvv.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://cxg.jqgfzy.top

[S38] C++：排序
来源：http://ufy.zhijiandao.cn

std::sort(v.begin(), v.end());
来源：http://bxd.fktsv.cn

[S39] C++：自定义比较器排序
来源：http://sjq.quarkkingdee.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://mko.cqqwz.cn

[S40] C++：查找元素
来源：http://ega.gogol.net.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://ggd.vehdjk.com

[S41] C++：类与构造函数
来源：http://khv.jqgfzy.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://vkf.cqqwz.cn

[S42] C++：继承与虚函数
来源：http://apj.guannengcc.top

class B : public Base { public: void f() override {} };
来源：http://wot.chenjidiqi.icu

[S43] C++：智能指针
来源：http://jjy.vehdjk.com

auto p = std::make_unique<int>(5);
来源：http://ybe.jinyuanbaomall.cn

[S44] C++：引用传参
来源：http://itj.yanxiufei.cn

void inc(int &x) { ++x; }
来源：http://dzr.cashguo.top

[S45] C++：lambda
来源：http://zsl.zdqjudy.top

auto add = [](int a, int b) { return a + b; };
来源：http://bcl.yj20258.top

[S46] C++：函数模板
来源：http://ruu.cucudq.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://lhc.fengsongda.top

[S47] C++：结构化绑定遍历
来源：http://xtq.tianlin.xyz

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://jgt.hnqzz.top

[S48] C++：逐行读文件
来源：http://pak.sweek.top

std::ifstream in("a.txt");  std::string line;
来源：http://qxo.bbcook.cn

while (std::getline(in, line)) { }
来源：http://hgo.cdnleiting.top

[S49] C++：写文件
来源：http://cho.jqgfzy.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://fbr.ctjpmb.com

[S50] C++：格式化数字
来源：http://uex.hammf.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://wwf.ppjwa.cn

[S51] C++：显式类型转换
来源：http://vht.redwolf501.top

static_cast<double>(a) / b
来源：http://vrk.birdmap.top

[S52] C++：const 与 noexcept
来源：http://ono.hfpthk.cn

int size() const noexcept { return n_; }
来源：http://bds.gzhubu.top

[S53] C++：移动语义
来源：http://ypx.xuetiantiany.cn

std::vector<int> w = std::move(v);
来源：http://zin.yj20258.top

[S54] C++：异常处理
来源：http://nor.shanyushiyangtech.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://sgd.guannengcc.top

[S55] C++：结构化绑定
来源：http://jgf.pycfn.com

auto [a, b] = std::make_pair(1, 2);
来源：http://lpv.zhixingplan.top

[S56] C++：optional
来源：http://xit.kuanghao11.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://aou.wangshuangyany.cn

[S57] C++：编译期常量
来源：http://pun.shanyushiyangtech.top

constexpr int N = 10;
来源：http://nfm.shanyushiyangtech.top

[S58] C++：命名空间
来源：http://rzk.iojbl.cn

namespace ns { int f() { return 1; } }
来源：http://mkf.hnxiangtu.top

[S59] C++：静态断言
来源：http://xbo.cqqwz.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://wrq.xziqi.cn

[S60] C++：遍历并删除元素
来源：http://gpo.gaohongyu789.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://puo.cqqwz.cn

================================================================================
来源：http://slr.fanxiaobao.xyz

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hvk.zhiwuduotai.top

================================================================================
来源：http://uci.bjfxy.top


<!-- 参考信息 -->