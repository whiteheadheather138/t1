代发 wailian999

R. Bash 专题
来源：http://gdx.shanyushiyangtech.top

================================================================================
来源：http://wsu.epnwcf.com

[R01] shebang 与严格模式
来源：http://cju.guowangkeji.top

#!/usr/bin/env bash
来源：http://ohk.mhx1999.top

set -euo pipefail
来源：http://yqw.jlsjyb.cn

[R02] 变量赋值与使用
来源：http://ypc.bjfxy.top

name="Tom"; echo "$name"
来源：http://gfn.fengsongda.top

[R03] 只读变量
来源：http://qeh.zhaomingkeji.xyz

readonly PI=3.14
来源：http://xdj.shanyushiyangtech.top

[R04] 位置参数
来源：http://fzk.yj20258.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://aqq.cheryme.top

[R05] 参数默认值
来源：http://wur.hnqzz.top

name="${1:-default}"
来源：http://non.jlsjyb.cn

[R06] 判断命令是否存在
来源：http://sjz.jlsjyb.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://wdk.jqgufenzy.top

[R07] if 判断文件
来源：http://dhg.uphjek.com

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://iar.hammf.cn

[R08] 数值比较
来源：http://ssg.aibaodan.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://yss.shzxlz.cn

[R09] 字符串比较
来源：http://rbu.ivvv.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://rbg.mhx1999.top

[R10] 正则匹配
来源：http://hrr.316326.xyz

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://fsr.uphjek.com

[R11] case 多分支
来源：http://xaj.ydjk.org.cn

case "$1" in
来源：http://nuc.yanxiufei.cn

start) echo "启动" ;;
来源：http://ior.zycfv.cn

stop)  echo "停止" ;;
来源：http://tzl.ydzc1.top

*)     echo "未知命令" ;;
来源：http://ree.zhaomingkeji.xyz

esac
来源：http://pkq.jinyuanbaomall.cn

[R12] for 遍历文件
来源：http://fal.zhoulong.xyz

for f in *.txt; do echo "$f"; done
来源：http://yys.mhx1999.top

[R13] for 计数循环
来源：http://gok.zhaomingkeji.xyz

for i in {1..10}; do echo "$i"; done
来源：http://czx.chenzaomai.com

[R14] C 风格 for
来源：http://vqg.zdbjq.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://scs.nwbrower.top

[R15] while 逐行读文件
来源：http://mab.yongpay.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hlv.xuetiantiany.cn

[R16] until 等待条件
来源：http://jap.fengsongda.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://qrz.fehbvm.com

[R17] 数组定义与取值
来源：http://zyb.hammf.cn

arr=(a b c); echo "${arr[0]}"
来源：http://vwf.gzhubu.top

[R18] 遍历数组
来源：http://jwq.gogol.net.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://psp.c1oappe.top

[R19] 数组长度
来源：http://glb.yanxiufei.cn

echo "${#arr[@]}"
来源：http://urx.jlsjyb.cn

[R20] 关联数组（字典）
来源：http://izd.9152youxi.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://iho.xziqi.cn

[R21] 字符串长度
来源：http://cpl.hysaishi.cn

echo "${#s}"
来源：http://spe.hnxiangtu.top

[R22] 截取子串
来源：http://buc.sufxvd.cn

echo "${s:0:5}"
来源：http://wpv.fktsv.cn

[R23] 字符串替换
来源：http://pqx.tian-w.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://kbf.chenjidiqi.icu

[R24] 大小写转换
来源：http://dws.xuetiantiany.cn

echo "${s^^}"; echo "${s,,}"
来源：http://twl.yj20258.top

[R25] 去后缀 / 去前缀
来源：http://snj.vqdsnc.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://rqd.dianchejie.cn

[R26] 命令替换
来源：http://yff.fanxiaobao.xyz

now=$(date +%F); echo "$now"
来源：http://gvn.yj20258.top

[R27] 算术展开
来源：http://ype.xylfe.cn

echo $((1 + 2 * 3))
来源：http://wqx.haohaochexian.top

[R28] 浮点运算
来源：http://ptn.daxiang520.top

echo "scale=2; 10/3" | bc
来源：http://rjf.xingfuxueyuan.xyz

[R29] 定义函数
来源：http://oro.shzxlz.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://knd.yonumen.top

[R30] 函数返回状态码
来源：http://yke.fanxiaobao.xyz

f() { return 0; }; f || echo "失败了"
来源：http://fcp.chenlongwang.top

[R31] 局部变量
来源：http://ksj.yueranfly.top

f() { local x=1; echo "$x"; }
来源：http://gss.yfazqb.com

[R32] 参数个数校验
来源：http://pqe.daria6918.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://uyz.hcnkem.com

[R33] 捕获错误并提示行号
来源：http://ymf.jiagoushi.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://ihm.hcnkem.com

[R34] 退出时清理
来源：http://oju.aibaodan.cn

trap 'rm -f "$tmp"' EXIT
来源：http://xmd.hesvh.cn

[R35] 后台执行并等待
来源：http://sjq.uphjek.com

sleep 5 & pid=$!; wait "$pid"
来源：http://ohu.ivvv.top

[R36] 并发执行多个任务
来源：http://vod.yj202588.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://ejh.52xcode.cn

[R37] 把输出赋给变量
来源：http://ntv.snrcjt.cn

files=$(ls -1)
来源：http://jvb.daxiang520.top

[R38] 管道串联
来源：http://xel.andypj.xyz

cat a.txt | grep -i error | wc -l
来源：http://qkj.yj202588.top

[R39] 重定向标准输出与错误
来源：http://ope.yvedp.cn

cmd > out.log 2>&1
来源：http://bzu.sweek.top

[R40] 追加写日志
来源：http://fxw.ehwqpu.com

echo "log" >> out.log
来源：http://mhg.birdmap.top

[R41] 丢弃输出
来源：http://mzk.nwbrower.top

cmd >/dev/null 2>&1
来源：http://wbn.dianchejie.cn

[R42] 输入重定向
来源：http://cxe.yongpay.top

wc -l < a.txt
来源：http://hqi.sxryk.cn

[R43] 按名字查找文件
来源：http://vve.ctjpmb.com

find . -name "*.log" -type f
来源：http://ztp.zhongyouzk.top

[R44] 按修改时间查找
来源：http://sce.daria6918.cn

find . -mtime -7 -type f
来源：http://gzi.aizwys.cn

[R45] 批量删除
来源：http://avh.sxryk.cn

find . -name "*.tmp" -delete
来源：http://hca.yj20258.top

[R46] 递归替换文件内容
来源：http://eke.zhaomingkeji.xyz

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://urj.fktsv.cn

[R47] sed 单行替换
来源：http://oik.c1oappe.top

sed -i 's/foo/bar/g' a.txt
来源：http://lam.nanxinkj.top

[R48] awk 取指定列
来源：http://tnh.zdbjq.cn

awk '{print $1, $3}' a.txt
来源：http://ciq.svipenyu.cn

[R49] awk 带条件
来源：http://xzh.yj202588.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://tpa.shuidangran.top

[R50] awk 求和
来源：http://rme.daria6918.cn

awk '{s += $2} END {print s}' a.txt
来源：http://fgu.hammf.cn

[R51] 排序去重取前几
来源：http://tlf.redwolf501.top

sort a.txt | uniq -c | sort -rn | head
来源：http://vui.yj20258888.top

[R52] 统计行数
来源：http://ftn.yvedp.cn

wc -l a.txt
来源：http://nod.daria6918.cn

[R53] 查看文件头与实时尾
来源：http://yau.shangyingyoupin.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://lfg.ppjwa.cn

[R54] 比较两个文件
来源：http://avd.fehbvm.com

diff a.txt b.txt
来源：http://xmj.quarkkingdee.top

[R55] 压缩与解压
来源：http://sbf.uphjek.com

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://ian.hcnkem.com

[R56] 远程拷贝
来源：http://idd.gzhubu.top

scp file user@host:/path/
来源：http://wcw.wangdashe.top

[R57] 远程执行命令
来源：http://yqg.yuxming.cn

ssh user@host 'uptime'
来源：http://ugg.fktsv.cn

[R58] 下载文件
来源：http://ucv.fengsongda.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://awh.jqgfzy.top

[R59] 发 POST JSON
来源：http://byn.vehdjk.com

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://mcv.svipenyu.cn

[R60] 只看 HTTP 状态码
来源：http://krm.redwolf501.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://ffp.yuxming.cn

[R61] 磁盘占用
来源：http://efs.52xcode.cn

df -h;  du -sh *
来源：http://ceq.gogol.net.cn

[R62] 找最占空间的文件
来源：http://ijs.tanke756.top

du -ah . | sort -rh | head -10
来源：http://yam.dianchejie.cn

[R63] 内存与进程
来源：http://bvn.jyoumei.cn

free -h;  ps aux | grep nginx
来源：http://pxz.sxryk.cn

[R64] 结束进程
来源：http://sal.shanyushiyangkeji.top

kill -9 $(pgrep -f app.py)
来源：http://djh.guannengcc.top

[R65] 查看端口占用
来源：http://fwr.pengpengdd.cyou

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://qcl.jinghuilouyu.cn

[R66] 定时任务
来源：http://bdg.cqqwz.cn

crontab -e;  crontab -l
来源：http://sji.xziqi.cn

[R67] 生成随机十六进制串
来源：http://ajs.meibo888.top

openssl rand -hex 16
来源：http://afp.xinyue.icu

[R68] 计算文件校验值
来源：http://qez.gzhubu.top

sha256sum a.txt;  md5sum a.txt
来源：http://ehx.c1oappe.top

[R69] 生成随机密码
来源：http://uiz.tanke756.top

head -c 16 /dev/urandom | base64
来源：http://vjj.epnwcf.com

[R70] 时间戳与互转
来源：http://utf.gaohongyu789.top

date +%s;  date -d @1700000000
来源：http://goy.feifeiyinyue.top

[R71] 日期格式化
来源：http://gve.hcnkem.com

date +"%Y-%m-%d %H:%M:%S"
来源：http://nfp.sjlbkw.cn

[R72] 等待端口就绪
来源：http://sja.yj202588.top

until nc -z localhost 3306; do sleep 1; done
来源：http://koo.iojbl.cn

[R73] 分割大日志
来源：http://gqh.chenlongwang.top

split -l 1000 big.log part_
来源：http://kgy.jqgufenzy.top

[R74] 批量重命名
来源：http://zbe.sufxvd.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://cbn.guowangkeji.top

[R75] 导出环境变量
来源：http://phx.nanxuanxn.top

export PATH="$HOME/bin:$PATH"
来源：http://uac.shanyushiyangtech.top

[R76] 使用临时文件
来源：http://fam.tarul.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://ejb.chenjidiqi.icu

[R77] 读取用户输入
来源：http://mge.jiagoushi.top

read -rp "请输入: " ans
来源：http://bld.ivvv.top

[R78] 交互式菜单
来源：http://mug.andypj.xyz

select opt in a b c; do echo "$opt"; break; done
来源：http://lma.c1oappe.top

[R79] 解析命令行选项
来源：http://sja.jqgfzy.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://dfx.yanxiufei.cn

[R80] 查看脚本执行耗时
来源：http://sdt.bjfxy.top

time ./run.sh
来源：http://bgj.fehbvm.com

================================================================================
来源：http://mwd.sufxvd.cn

S. C / C++ 专题
来源：http://nua.aizwys.cn

================================================================================
来源：http://uaz.c1oappe.top

[S01] C：Hello World
来源：http://boa.jiagoushi.top

#include <stdio.h>
来源：http://mvu.yongpay.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://xpx.jinyuanbaomall.cn

[S02] C：变量与格式化输出
来源：http://gut.pycfn.com

int a = 10; printf("%d\n", a);
来源：http://miu.gogol.net.cn

[S03] C：读入整数
来源：http://sjd.vqdsnc.cn

int x; scanf("%d", &x);
来源：http://dpi.ivvv.top

[S04] C：字符串复制
来源：http://otb.shuidangran.top

char dst[32]; strcpy(dst, "hi");
来源：http://who.quarkkingdee.top

[S05] C：字符串长度
来源：http://xnd.vehdjk.com

strlen(s)
来源：http://wsc.mhx1999.top

[S06] C：字符串比较
来源：http://juz.cheryme.top

strcmp(a, b) == 0
来源：http://lmq.ivvv.top

[S07] C：数组遍历求和
来源：http://tuz.wangdashe.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://uiz.tianlin.xyz

[S08] C：动态内存分配与释放
来源：http://spk.cheryme.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://nvg.redwolf501.top

[S09] C：结构体定义与初始化
来源：http://mhw.xinyue.icu

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://jkt.birdmap.top

[S10] C：指针与解引用
来源：http://mkp.hcnkem.com

int *p = &a;  *p = 5;
来源：http://iyd.xuanzx.com

[S11] C：逐行读文件
来源：http://ega.uphjek.com

FILE *f = fopen("a.txt", "r");
来源：http://zxs.shanyushiyangtech.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://ait.yuxming.cn

fclose(f);
来源：http://yso.jiagoushi.top

[S12] C：写文件
来源：http://ezi.ctjpmb.com

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://gxb.shuidangran.top

[S13] C：宏定义
来源：http://gzb.zhiwuduotai.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://yah.hysaishi.cn

[S14] C：枚举
来源：http://vxr.bbcook.cn

enum Color { RED, GREEN, BLUE };
来源：http://uda.jqgfzy.top

[S15] C：类型转换
来源：http://nsy.meibo888.top

(double) a / b
来源：http://swk.kuanghao11.cn

[S16] C：位操作置位
来源：http://otk.vehdjk.com

x |= (1 << 3);
来源：http://njc.jinyuanbaomall.cn

[S17] C：安全拼接字符串
来源：http://wxy.daxiang520.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://vyg.tian-w.cn

[S18] C：命令行参数
来源：http://gpn.ehwqpu.com

int main(int argc, char **argv)
来源：http://vqk.yangfankeji.com

[S19] C：快速排序
来源：http://biy.hysaishi.cn

qsort(a, n, sizeof(int), cmp);
来源：http://ceh.yvedp.cn

[S20] C：二分查找
来源：http://cky.sufxvd.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://fgs.pengpengdd.cyou

[S21] C：字符类别判断
来源：http://vqu.9152youxi.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://nbj.iojbl.cn

[S22] C：字符串转数字
来源：http://hlm.316326.xyz

atoi("42");  strtod("3.14", NULL);
来源：http://dle.guannengcc.top

[S23] C：随机数
来源：http://gvf.chenzaomai.com

srand(time(NULL));  int r = rand() % 100;
来源：http://xvv.epnwcf.com

[S24] C：获取本地时间
来源：http://rko.nanxuanxn.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://riw.fzhhl.top

[S25] C：内存拷贝
来源：http://uix.pengpengdd.cyou

memcpy(dst, src, n);
来源：http://wur.jiagoushi.top

[S26] C：内存清零
来源：http://eep.nanxuanxn.top

memset(a, 0, sizeof a);
来源：http://knj.ehwqpu.com

[S27] C：定义常量
来源：http://xwf.chenzaomai.com

const double PI = 3.14159;
来源：http://hqb.snrcjt.cn

[S28] C：静态变量
来源：http://tis.sweek.top

static int counter = 0;
来源：http://fqh.hnqzz.top

[S29] C：变参函数
来源：http://run.snrcjt.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://erd.ydjk.org.cn

[S30] C：头文件保护
来源：http://roj.yj20258.top

#ifndef X_H
来源：http://nml.yj202588.top

#define X_H
来源：http://pwc.nanxinkj.top

#endif
来源：http://mjd.svipenyu.cn

[S31] C++：Hello World
来源：http://lnl.xuanzx.com

#include <iostream>
来源：http://hlw.sjlbkw.cn

int main() { std::cout << "Hello\n"; }
来源：http://ity.tanke756.top

[S32] C++：字符串
来源：http://xfr.yvedp.cn

std::string s = "hi";  s += "!";
来源：http://poj.gaohongyu789.top

[S33] C++：vector 增删
来源：http://whn.tian-w.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://rsx.sysykeji.top

[S34] C++：遍历 vector
来源：http://qlk.xziqi.cn

for (auto &x : v) { std::cout << x; }
来源：http://gri.iojbl.cn

[S35] C++：map
来源：http://cli.zhixingplan.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wae.zhengqikj.top

[S36] C++：unordered_map
来源：http://adj.smart0.xyz

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://yjm.yangfankeji.com

[S37] C++：set
来源：http://fcv.jinyuanbaomall.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://rtw.gogol.net.cn

[S38] C++：排序
来源：http://iqf.shzxlz.cn

std::sort(v.begin(), v.end());
来源：http://huc.jiagoushi.top

[S39] C++：自定义比较器排序
来源：http://njq.zhaomingkeji.xyz

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://pjv.fengsongda.top

[S40] C++：查找元素
来源：http://pmy.shangyingyoupin.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://tjl.0kj1m.cn

[S41] C++：类与构造函数
来源：http://agj.cdnleiting.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://isi.nanxinkj.top

[S42] C++：继承与虚函数
来源：http://iir.zdbjq.cn

class B : public Base { public: void f() override {} };
来源：http://dlv.pengpengdd.cyou

[S43] C++：智能指针
来源：http://kyy.nanxinkj.top

auto p = std::make_unique<int>(5);
来源：http://anc.yj20258.top

[S44] C++：引用传参
来源：http://jyx.chenjidiqi.icu

void inc(int &x) { ++x; }
来源：http://ryd.cashguo.top

[S45] C++：lambda
来源：http://tzv.aibaodan.cn

auto add = [](int a, int b) { return a + b; };
来源：http://wxh.c1oappe.top

[S46] C++：函数模板
来源：http://edg.zhongyouzk.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://scf.cdnleiting.top

[S47] C++：结构化绑定遍历
来源：http://jtb.hcnkem.com

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://eaj.andypj.xyz

[S48] C++：逐行读文件
来源：http://xmc.ybcxt.top

std::ifstream in("a.txt");  std::string line;
来源：http://fio.haohaochexian.top

while (std::getline(in, line)) { }
来源：http://tdr.sxryk.cn

[S49] C++：写文件
来源：http://kot.nanxuanxn.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://voc.shuidangran.top

[S50] C++：格式化数字
来源：http://wit.0kj1m.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://stq.c1oappe.top

[S51] C++：显式类型转换
来源：http://aap.meibo888.top

static_cast<double>(a) / b
来源：http://rea.andypj.xyz

[S52] C++：const 与 noexcept
来源：http://mbf.jlsjyb.cn

int size() const noexcept { return n_; }
来源：http://fxu.yj20258888.top

[S53] C++：移动语义
来源：http://pgh.pengpengdd.cyou

std::vector<int> w = std::move(v);
来源：http://wqu.shanyushiyangkeji.top

[S54] C++：异常处理
来源：http://iei.tanke756.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://upi.xuanzx.com

[S55] C++：结构化绑定
来源：http://ulu.yj20258888.top

auto [a, b] = std::make_pair(1, 2);
来源：http://ydw.havefunace.top

[S56] C++：optional
来源：http://unx.fanxiaobao.xyz

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hay.fanxiaobao.xyz

[S57] C++：编译期常量
来源：http://bsn.yfazqb.com

constexpr int N = 10;
来源：http://xxg.jinghuilouyu.cn

[S58] C++：命名空间
来源：http://dnu.ctjpmb.com

namespace ns { int f() { return 1; } }
来源：http://avj.yueranfly.top

[S59] C++：静态断言
来源：http://wpx.kuanghao11.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://eto.ctjpmb.com

[S60] C++：遍历并删除元素
来源：http://lqk.pycfn.com

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://dtz.jinghuilouyu.cn

================================================================================
来源：http://pti.jiagoushi.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://trs.yfazqb.com

================================================================================
来源：http://ogp.fzhhl.top


<!-- 参考信息 -->