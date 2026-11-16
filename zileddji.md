代发 wailian999

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://jba.nanxuanxn.top

[Q90] 生成序号列
来源：http://qat.ehwqpu.com

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://spy.fehbvm.com

================================================================================
来源：http://laz.yvedp.cn

R. Bash 专题
来源：http://mhd.jlsjyb.cn

================================================================================
来源：http://tjc.cucudq.cn

[R01] shebang 与严格模式
来源：http://dzr.xuanzx.com

#!/usr/bin/env bash
来源：http://thz.ehwqpu.com

set -euo pipefail
来源：http://whr.gaohongyu789.top

[R02] 变量赋值与使用
来源：http://ble.aibaodan.cn

name="Tom"; echo "$name"
来源：http://poa.aibaodan.cn

[R03] 只读变量
来源：http://bzn.mhx1999.top

readonly PI=3.14
来源：http://lzk.zhongyouzk.top

[R04] 位置参数
来源：http://uzh.gzhubu.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://jaj.hnqzz.top

[R05] 参数默认值
来源：http://pri.tianlin.xyz

name="${1:-default}"
来源：http://vhn.sweek.top

[R06] 判断命令是否存在
来源：http://yeg.fehbvm.com

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://gqp.birdmap.top

[R07] if 判断文件
来源：http://qrk.cdnleiting.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://mwx.zhiwuduotai.top

[R08] 数值比较
来源：http://tte.jyoumei.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://sbe.52xcode.cn

[R09] 字符串比较
来源：http://oiz.zhiwuduotai.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://rvf.sweek.top

[R10] 正则匹配
来源：http://rhg.chenlongwang.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://zug.yj20258888.top

[R11] case 多分支
来源：http://ejj.zhongyouzk.top

case "$1" in
来源：http://udj.andypj.xyz

start) echo "启动" ;;
来源：http://afu.jqgfzy.top

stop)  echo "停止" ;;
来源：http://zgd.daria6918.cn

*)     echo "未知命令" ;;
来源：http://xcv.meibo888.top

esac
来源：http://ufo.haohaochexian.top

[R12] for 遍历文件
来源：http://dua.zhixingplan.top

for f in *.txt; do echo "$f"; done
来源：http://cuu.jinghuilouyu.cn

[R13] for 计数循环
来源：http://jot.hywenlv.cn

for i in {1..10}; do echo "$i"; done
来源：http://cyd.gogol.net.cn

[R14] C 风格 for
来源：http://nux.hammf.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://rkd.svipenyu.cn

[R15] while 逐行读文件
来源：http://eqq.andypj.xyz

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://fgi.sjlbkw.cn

[R16] until 等待条件
来源：http://iob.316326.xyz

until [[ -f done.flag ]]; do sleep 1; done
来源：http://dur.xinyue.icu

[R17] 数组定义与取值
来源：http://hip.havefunace.top

arr=(a b c); echo "${arr[0]}"
来源：http://seg.pengpengdd.cyou

[R18] 遍历数组
来源：http://cbm.vehdjk.com

for x in "${arr[@]}"; do echo "$x"; done
来源：http://akg.nanxuanxn.top

[R19] 数组长度
来源：http://sdq.52xcode.cn

echo "${#arr[@]}"
来源：http://bbf.wangshuangyany.cn

[R20] 关联数组（字典）
来源：http://nge.zycfv.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://sxx.sysykeji.top

[R21] 字符串长度
来源：http://omh.gogol.net.cn

echo "${#s}"
来源：http://uao.tanke756.top

[R22] 截取子串
来源：http://ixl.zdqjudy.top

echo "${s:0:5}"
来源：http://hcw.smart0.xyz

[R23] 字符串替换
来源：http://kah.bjfxy.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://tqk.jianghu66.top

[R24] 大小写转换
来源：http://wym.0kj1m.cn

echo "${s^^}"; echo "${s,,}"
来源：http://nug.zhongyouzk.top

[R25] 去后缀 / 去前缀
来源：http://gil.zhoulong.xyz

echo "${f%.txt}"; echo "${f#./}"
来源：http://epp.fktsv.cn

[R26] 命令替换
来源：http://gvs.xuetiantiany.cn

now=$(date +%F); echo "$now"
来源：http://tyt.gogol.net.cn

[R27] 算术展开
来源：http://ccw.iojbl.cn

echo $((1 + 2 * 3))
来源：http://lvn.shangyingyoupin.top

[R28] 浮点运算
来源：http://ynj.yuxming.cn

echo "scale=2; 10/3" | bc
来源：http://zyu.jianghu66.top

[R29] 定义函数
来源：http://ipl.gotoacloud.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://axc.pycfn.com

[R30] 函数返回状态码
来源：http://rwj.316326.xyz

f() { return 0; }; f || echo "失败了"
来源：http://wuf.zhengqikj.top

[R31] 局部变量
来源：http://ggv.ywan-chungtsiang.top

f() { local x=1; echo "$x"; }
来源：http://xmm.xuanzx.com

[R32] 参数个数校验
来源：http://pdy.xylfe.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://kse.svipenyu.cn

[R33] 捕获错误并提示行号
来源：http://uit.epnwcf.com

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://qpg.sysykeji.top

[R34] 退出时清理
来源：http://leb.iojbl.cn

trap 'rm -f "$tmp"' EXIT
来源：http://vjr.hfpthk.cn

[R35] 后台执行并等待
来源：http://mgs.tanke756.top

sleep 5 & pid=$!; wait "$pid"
来源：http://ivg.jianghu66.top

[R36] 并发执行多个任务
来源：http://jxm.sysykeji.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://saq.aizwys.cn

[R37] 把输出赋给变量
来源：http://kpa.ydzc1.top

files=$(ls -1)
来源：http://kxk.smart0.xyz

[R38] 管道串联
来源：http://dwr.hnqzz.top

cat a.txt | grep -i error | wc -l
来源：http://lsj.sjlbkw.cn

[R39] 重定向标准输出与错误
来源：http://tlw.hongshengwenyu.top

cmd > out.log 2>&1
来源：http://rcz.fehbvm.com

[R40] 追加写日志
来源：http://uwm.zhiwuduotai.top

echo "log" >> out.log
来源：http://nud.hcnkem.com

[R41] 丢弃输出
来源：http://ase.zhijiandao.cn

cmd >/dev/null 2>&1
来源：http://jlm.cqqwz.cn

[R42] 输入重定向
来源：http://zqk.kuanghao11.cn

wc -l < a.txt
来源：http://gxb.yuanzhike.top

[R43] 按名字查找文件
来源：http://cbh.gotoacloud.top

find . -name "*.log" -type f
来源：http://mal.havefunace.top

[R44] 按修改时间查找
来源：http://opz.jinqigfzy.top

find . -mtime -7 -type f
来源：http://deg.meibo888.top

[R45] 批量删除
来源：http://prq.52xcode.cn

find . -name "*.tmp" -delete
来源：http://nqy.yanxiufei.cn

[R46] 递归替换文件内容
来源：http://ldb.haohaochexian.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://ohk.fktsv.cn

[R47] sed 单行替换
来源：http://gnp.zhijiandao.cn

sed -i 's/foo/bar/g' a.txt
来源：http://cwo.svipenyu.cn

[R48] awk 取指定列
来源：http://fhu.guannengcc.top

awk '{print $1, $3}' a.txt
来源：http://ais.yangfankeji.com

[R49] awk 带条件
来源：http://xho.gotoacloud.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://vhd.mhx1999.top

[R50] awk 求和
来源：http://kfu.chenzaomai.com

awk '{s += $2} END {print s}' a.txt
来源：http://mex.sysykeji.top

[R51] 排序去重取前几
来源：http://mgr.316326.xyz

sort a.txt | uniq -c | sort -rn | head
来源：http://vfi.zdbjq.cn

[R52] 统计行数
来源：http://ieu.yj20258888.top

wc -l a.txt
来源：http://rrp.nanxinkj.top

[R53] 查看文件头与实时尾
来源：http://hpq.gogol.net.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://thx.zdqjudy.top

[R54] 比较两个文件
来源：http://hsu.aizwys.cn

diff a.txt b.txt
来源：http://iql.hammf.cn

[R55] 压缩与解压
来源：http://aoo.9152youxi.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://iib.bbcook.cn

[R56] 远程拷贝
来源：http://xfj.cqqwz.cn

scp file user@host:/path/
来源：http://laz.ctjpmb.com

[R57] 远程执行命令
来源：http://syq.xinyue.icu

ssh user@host 'uptime'
来源：http://mka.jlsjyb.cn

[R58] 下载文件
来源：http://xzo.xylfe.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://gxl.yuxming.cn

[R59] 发 POST JSON
来源：http://bxw.zdqjudy.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://skv.yuanzhike.top

[R60] 只看 HTTP 状态码
来源：http://mzo.9152youxi.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://eto.haohaochexian.top

[R61] 磁盘占用
来源：http://tdi.iojbl.cn

df -h;  du -sh *
来源：http://igq.smart0.xyz

[R62] 找最占空间的文件
来源：http://ehv.epnwcf.com

du -ah . | sort -rh | head -10
来源：http://pcy.redwolf501.top

[R63] 内存与进程
来源：http://bxn.hfpthk.cn

free -h;  ps aux | grep nginx
来源：http://qnh.yueranfly.top

[R64] 结束进程
来源：http://fvp.tianlin.xyz

kill -9 $(pgrep -f app.py)
来源：http://tvk.tanke756.top

[R65] 查看端口占用
来源：http://uhv.tanke756.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://myc.andypj.xyz

[R66] 定时任务
来源：http://dfu.jyoumei.cn

crontab -e;  crontab -l
来源：http://rbj.fanxiaobao.xyz

[R67] 生成随机十六进制串
来源：http://uhr.svipenyu.cn

openssl rand -hex 16
来源：http://kwp.chenlongwang.top

[R68] 计算文件校验值
来源：http://iwq.vqdsnc.cn

sha256sum a.txt;  md5sum a.txt
来源：http://vvz.cheryme.top

[R69] 生成随机密码
来源：http://qce.ctjpmb.com

head -c 16 /dev/urandom | base64
来源：http://scr.yonumen.top

[R70] 时间戳与互转
来源：http://tos.haohaochexian.top

date +%s;  date -d @1700000000
来源：http://ijh.yanxiufei.cn

[R71] 日期格式化
来源：http://khv.zdbjq.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://bco.hnqzz.top

[R72] 等待端口就绪
来源：http://eas.zhaomingkeji.xyz

until nc -z localhost 3306; do sleep 1; done
来源：http://hka.jianghu66.top

[R73] 分割大日志
来源：http://ewt.birdmap.top

split -l 1000 big.log part_
来源：http://ila.zhiwuduotai.top

[R74] 批量重命名
来源：http://ojf.chenzaomai.com

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://xku.kuanghao11.cn

[R75] 导出环境变量
来源：http://zel.andypj.xyz

export PATH="$HOME/bin:$PATH"
来源：http://voe.ydzc1.top

[R76] 使用临时文件
来源：http://roy.tanke756.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://zid.0kj1m.cn

[R77] 读取用户输入
来源：http://twc.gzhubu.top

read -rp "请输入: " ans
来源：http://ega.ydzc1.top

[R78] 交互式菜单
来源：http://gxz.jyoumei.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://ghj.fanxiaobao.xyz

[R79] 解析命令行选项
来源：http://xbu.gotoacloud.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mri.tarul.cn

[R80] 查看脚本执行耗时
来源：http://xpl.pengpengdd.cyou

time ./run.sh
来源：http://ovb.hfpthk.cn

================================================================================
来源：http://efy.yongpay.top

S. C / C++ 专题
来源：http://his.shuidangran.top

================================================================================
来源：http://mzz.kuanghao11.cn

[S01] C：Hello World
来源：http://nyr.wangshuangyany.cn

#include <stdio.h>
来源：http://wge.jqgfzy.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://evb.hnxiangtu.top

[S02] C：变量与格式化输出
来源：http://qzv.hfpthk.cn

int a = 10; printf("%d\n", a);
来源：http://iwl.haohaochexian.top

[S03] C：读入整数
来源：http://wsp.hammf.cn

int x; scanf("%d", &x);
来源：http://jjc.pycfn.com

[S04] C：字符串复制
来源：http://lqe.epnwcf.com

char dst[32]; strcpy(dst, "hi");
来源：http://lex.snrcjt.cn

[S05] C：字符串长度
来源：http://fmw.fanxiaobao.xyz

strlen(s)
来源：http://mfy.svipenyu.cn

[S06] C：字符串比较
来源：http://ysr.shzxlz.cn

strcmp(a, b) == 0
来源：http://bhd.chenjidiqi.icu

[S07] C：数组遍历求和
来源：http://qgb.hcnkem.com

for (int i = 0; i < n; i++) sum += a[i];
来源：http://drl.pycfn.com

[S08] C：动态内存分配与释放
来源：http://fsa.jinqigufen.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mgt.yonumen.top

[S09] C：结构体定义与初始化
来源：http://sgo.cdnleiting.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mkd.daria6918.cn

[S10] C：指针与解引用
来源：http://ruv.fengsongda.top

int *p = &a;  *p = 5;
来源：http://vvf.yanxiufei.cn

[S11] C：逐行读文件
来源：http://unh.fehbvm.com

FILE *f = fopen("a.txt", "r");
来源：http://eqt.chenzaomai.com

while (fgets(buf, sizeof buf, f)) { }
来源：http://qwh.pengpengdd.cyou

fclose(f);
来源：http://xzo.kuanghao11.cn

[S12] C：写文件
来源：http://vcy.nanxinkj.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://cvu.smart0.xyz

[S13] C：宏定义
来源：http://vbw.jinqigfzy.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wie.ivvv.top

[S14] C：枚举
来源：http://cjp.hammf.cn

enum Color { RED, GREEN, BLUE };
来源：http://qhy.iojbl.cn

[S15] C：类型转换
来源：http://btk.yanxiufei.cn

(double) a / b
来源：http://mrf.shuidangran.top

[S16] C：位操作置位
来源：http://bhd.andypj.xyz

x |= (1 << 3);
来源：http://lmr.wangdashe.top

[S17] C：安全拼接字符串
来源：http://oob.ydzc1.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://gpu.yongpay.top

[S18] C：命令行参数
来源：http://fzp.chenjidiqi.icu

int main(int argc, char **argv)
来源：http://hpp.xziqi.cn

[S19] C：快速排序
来源：http://nvo.yonumen.top

qsort(a, n, sizeof(int), cmp);
来源：http://abq.chenzaomai.com

[S20] C：二分查找
来源：http://dos.316326.xyz

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://nhp.hfpthk.cn

[S21] C：字符类别判断
来源：http://xbq.yangfankeji.com

isdigit(c);  isalpha(c);  isspace(c);
来源：http://cer.tanke756.top

[S22] C：字符串转数字
来源：http://vlv.cheryme.top

atoi("42");  strtod("3.14", NULL);
来源：http://lnd.hcnkem.com

[S23] C：随机数
来源：http://ymp.ctjpmb.com

srand(time(NULL));  int r = rand() % 100;
来源：http://tvl.cucudq.cn

[S24] C：获取本地时间
来源：http://fqe.wangdashe.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://qqx.fengsongda.top

[S25] C：内存拷贝
来源：http://wrw.dashuyun.cn

memcpy(dst, src, n);
来源：http://ciw.ydjk.org.cn

[S26] C：内存清零
来源：http://lse.yonumen.top

memset(a, 0, sizeof a);
来源：http://ueb.fzhhl.top

[S27] C：定义常量
来源：http://pdh.meibo888.top

const double PI = 3.14159;
来源：http://orb.cucudq.cn

[S28] C：静态变量
来源：http://ish.guannengcc.top

static int counter = 0;
来源：http://wmv.ywan-chungtsiang.top

[S29] C：变参函数
来源：http://qqz.jinghuilouyu.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://rki.yuxming.cn

[S30] C：头文件保护
来源：http://tpi.hesvh.cn

#ifndef X_H
来源：http://gpc.yuanzhike.top

#define X_H
来源：http://arn.zhaomingkeji.xyz

#endif
来源：http://fmd.tanke756.top

[S31] C++：Hello World
来源：http://tdm.vehdjk.com

#include <iostream>
来源：http://aac.uphjek.com

int main() { std::cout << "Hello\n"; }
来源：http://bdw.bjfxy.top

[S32] C++：字符串
来源：http://pwn.tarul.cn

std::string s = "hi";  s += "!";
来源：http://ntm.chenlongwang.top

[S33] C++：vector 增删
来源：http://noy.dianchejie.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hyq.iojbl.cn

[S34] C++：遍历 vector
来源：http://qcb.svipenyu.cn

for (auto &x : v) { std::cout << x; }
来源：http://vms.shangyingyoupin.top

[S35] C++：map
来源：http://wks.zhoulong.xyz

std::map<std::string, int> m;  m["a"] = 1;
来源：http://gab.fanxiaobao.xyz

[S36] C++：unordered_map
来源：http://mcm.sjlbkw.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://ucp.shanyushiyangtech.top

[S37] C++：set
来源：http://een.0kj1m.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://agb.xingfuxueyuan.xyz

[S38] C++：排序
来源：http://mbe.hnqzz.top

std::sort(v.begin(), v.end());
来源：http://iap.sysykeji.top

[S39] C++：自定义比较器排序
来源：http://heq.yueranfly.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://vdm.ppjwa.cn

[S40] C++：查找元素
来源：http://see.tarul.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://eqs.redwolf501.top

[S41] C++：类与构造函数
来源：http://mlt.zhixingplan.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://jsj.zhixingplan.top

[S42] C++：继承与虚函数
来源：http://hfv.fktsv.cn

class B : public Base { public: void f() override {} };
来源：http://opg.jqgfzy.top

[S43] C++：智能指针
来源：http://gtp.xingfuxueyuan.xyz

auto p = std::make_unique<int>(5);
来源：http://yax.iojbl.cn

[S44] C++：引用传参
来源：http://sli.sweek.top

void inc(int &x) { ++x; }
来源：http://oqe.chenlongwang.top

[S45] C++：lambda
来源：http://vrl.0kj1m.cn

auto add = [](int a, int b) { return a + b; };
来源：http://uoo.316326.xyz

[S46] C++：函数模板
来源：http://dxz.fktsv.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://xfl.daxiang520.top

[S47] C++：结构化绑定遍历
来源：http://tyk.kuanghao11.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://yqq.yj20258888.top

[S48] C++：逐行读文件
来源：http://ufo.jiagoushi.top

std::ifstream in("a.txt");  std::string line;
来源：http://orr.wangshuangyany.cn

while (std::getline(in, line)) { }
来源：http://dlm.chenlongwang.top

[S49] C++：写文件
来源：http://ctt.epnwcf.com

std::ofstream out("a.txt");  out << "hi\n";
来源：http://umj.hcnkem.com

[S50] C++：格式化数字
来源：http://gyx.jinqigufen.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://ibx.xziqi.cn

[S51] C++：显式类型转换
来源：http://vxl.guowangkeji.top

static_cast<double>(a) / b
来源：http://tel.yongpay.top

[S52] C++：const 与 noexcept
来源：http://spb.yj202588.top

int size() const noexcept { return n_; }
来源：http://pzq.hfpthk.cn

[S53] C++：移动语义
来源：http://nnp.jiagoushi.top

std::vector<int> w = std::move(v);
来源：http://gws.guowangkeji.top

[S54] C++：异常处理
来源：http://cos.sjlbkw.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://kjm.shanyushiyangkeji.top

[S55] C++：结构化绑定
来源：http://ict.xinyue.icu

auto [a, b] = std::make_pair(1, 2);
来源：http://bgy.nanxuanxn.top

[S56] C++：optional
来源：http://evj.jinghuilouyu.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://sga.xuanzx.com

[S57] C++：编译期常量
来源：http://daw.shuidangran.top

constexpr int N = 10;
来源：http://dvq.wangshuangyany.cn

[S58] C++：命名空间
来源：http://bgo.52xcode.cn

namespace ns { int f() { return 1; } }
来源：http://mgi.cucudq.cn

[S59] C++：静态断言
来源：http://tvx.jinyuanbaomall.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://grg.cheryme.top

[S60] C++：遍历并删除元素
来源：http://mbq.jinyuanbaomall.cn


<!-- 参考信息 -->