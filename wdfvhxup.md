代发 wailian999

set -euo pipefail
来源：http://bph.pycfn.com

[R02] 变量赋值与使用
来源：http://pwd.fengsongda.top

name="Tom"; echo "$name"
来源：http://nuy.pycfn.com

[R03] 只读变量
来源：http://wdb.shanyushiyangkeji.top

readonly PI=3.14
来源：http://pxq.tanke756.top

[R04] 位置参数
来源：http://rvk.aizwys.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://ucw.xingfuxueyuan.xyz

[R05] 参数默认值
来源：http://nde.xziqi.cn

name="${1:-default}"
来源：http://qtf.ywan-chungtsiang.top

[R06] 判断命令是否存在
来源：http://ftk.hnxiangtu.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://tjk.52xcode.cn

[R07] if 判断文件
来源：http://ghz.chenlongwang.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://dmy.zhiwuduotai.top

[R08] 数值比较
来源：http://vma.mhx1999.top

if (( a > b )); then echo "a 更大"; fi
来源：http://ttt.zhijiandao.cn

[R09] 字符串比较
来源：http://qws.xylfe.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://vri.jqgufenzy.top

[R10] 正则匹配
来源：http://dog.haohaochexian.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://ryi.hnxiangtu.top

[R11] case 多分支
来源：http://jys.52xcode.cn

case "$1" in
来源：http://bbd.yueranfly.top

start) echo "启动" ;;
来源：http://muu.jinqigufen.top

stop)  echo "停止" ;;
来源：http://qqo.316326.xyz

*)     echo "未知命令" ;;
来源：http://kkb.guowangkeji.top

esac
来源：http://koy.jiagoushi.top

[R12] for 遍历文件
来源：http://sth.havefunace.top

for f in *.txt; do echo "$f"; done
来源：http://usw.ydjk.org.cn

[R13] for 计数循环
来源：http://gva.vqdsnc.cn

for i in {1..10}; do echo "$i"; done
来源：http://efj.tarul.cn

[R14] C 风格 for
来源：http://uaz.jinghuilouyu.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://wvy.hnxiangtu.top

[R15] while 逐行读文件
来源：http://dsr.cqqwz.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://gnu.zhaomingkeji.xyz

[R16] until 等待条件
来源：http://htr.bjfxy.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://alf.hysaishi.cn

[R17] 数组定义与取值
来源：http://lgy.shanyushiyangtech.top

arr=(a b c); echo "${arr[0]}"
来源：http://xtu.meibo888.top

[R18] 遍历数组
来源：http://vfh.zdbjq.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://scz.yuxming.cn

[R19] 数组长度
来源：http://mul.fanxiaobao.xyz

echo "${#arr[@]}"
来源：http://cbb.jqgfzy.top

[R20] 关联数组（字典）
来源：http://yuk.fanxiaobao.xyz

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://qhq.vehdjk.com

[R21] 字符串长度
来源：http://ghz.hnxiangtu.top

echo "${#s}"
来源：http://rod.yfazqb.com

[R22] 截取子串
来源：http://cmm.nanxinkj.top

echo "${s:0:5}"
来源：http://tks.fanxiaobao.xyz

[R23] 字符串替换
来源：http://cpq.sxryk.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hgm.52xcode.cn

[R24] 大小写转换
来源：http://smx.yonumen.top

echo "${s^^}"; echo "${s,,}"
来源：http://rls.yongpay.top

[R25] 去后缀 / 去前缀
来源：http://qew.zhixingplan.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://eqd.hongshengwenyu.top

[R26] 命令替换
来源：http://jhf.jqgfzy.top

now=$(date +%F); echo "$now"
来源：http://kuz.sxryk.cn

[R27] 算术展开
来源：http://kqz.sweek.top

echo $((1 + 2 * 3))
来源：http://nqw.pengpengdd.cyou

[R28] 浮点运算
来源：http://bxt.hnxiangtu.top

echo "scale=2; 10/3" | bc
来源：http://maq.zdbjq.cn

[R29] 定义函数
来源：http://ivu.xingfuxueyuan.xyz

add() { echo $(($1 + $2)); }; add 1 2
来源：http://ycu.pycfn.com

[R30] 函数返回状态码
来源：http://oyo.quarkkingdee.top

f() { return 0; }; f || echo "失败了"
来源：http://bds.tarul.cn

[R31] 局部变量
来源：http://yqm.yongpay.top

f() { local x=1; echo "$x"; }
来源：http://qwe.dashuyun.cn

[R32] 参数个数校验
来源：http://hsb.zdbjq.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://phx.cashguo.top

[R33] 捕获错误并提示行号
来源：http://iwy.yanxiufei.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://cxy.ywan-chungtsiang.top

[R34] 退出时清理
来源：http://mat.zhongyouzk.top

trap 'rm -f "$tmp"' EXIT
来源：http://vdo.cucudq.cn

[R35] 后台执行并等待
来源：http://yyr.smart0.xyz

sleep 5 & pid=$!; wait "$pid"
来源：http://ted.52xcode.cn

[R36] 并发执行多个任务
来源：http://dgo.quarkkingdee.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://asi.pengpengdd.cyou

[R37] 把输出赋给变量
来源：http://fsg.fengsongda.top

files=$(ls -1)
来源：http://pmd.zhaomingkeji.xyz

[R38] 管道串联
来源：http://hxn.gaohongyu789.top

cat a.txt | grep -i error | wc -l
来源：http://rnu.daria6918.cn

[R39] 重定向标准输出与错误
来源：http://eqw.tianlin.xyz

cmd > out.log 2>&1
来源：http://alm.zdqjudy.top

[R40] 追加写日志
来源：http://rdu.chenzaomai.com

echo "log" >> out.log
来源：http://wsu.sjlbkw.cn

[R41] 丢弃输出
来源：http://wdo.pengpengdd.cyou

cmd >/dev/null 2>&1
来源：http://mam.yangfankeji.com

[R42] 输入重定向
来源：http://ifj.ehwqpu.com

wc -l < a.txt
来源：http://lzr.bbcook.cn

[R43] 按名字查找文件
来源：http://hqe.zhoulong.xyz

find . -name "*.log" -type f
来源：http://pdn.andypj.xyz

[R44] 按修改时间查找
来源：http://ofn.zhongyouzk.top

find . -mtime -7 -type f
来源：http://wtz.yanxiufei.cn

[R45] 批量删除
来源：http://iwg.jyoumei.cn

find . -name "*.tmp" -delete
来源：http://yau.chenjidiqi.icu

[R46] 递归替换文件内容
来源：http://ccz.nanxinkj.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://jgz.chenlongwang.top

[R47] sed 单行替换
来源：http://iri.xuetiantiany.cn

sed -i 's/foo/bar/g' a.txt
来源：http://ymk.uphjek.com

[R48] awk 取指定列
来源：http://ctf.316326.xyz

awk '{print $1, $3}' a.txt
来源：http://vjm.jinyuanbaomall.cn

[R49] awk 带条件
来源：http://ndh.hesvh.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://rsn.fktsv.cn

[R50] awk 求和
来源：http://rto.bjfxy.top

awk '{s += $2} END {print s}' a.txt
来源：http://kew.jqgfzy.top

[R51] 排序去重取前几
来源：http://mxj.yj202588.top

sort a.txt | uniq -c | sort -rn | head
来源：http://bff.shuidangran.top

[R52] 统计行数
来源：http://sra.hfpthk.cn

wc -l a.txt
来源：http://awl.wangshuangyany.cn

[R53] 查看文件头与实时尾
来源：http://jfm.aibaodan.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://ohx.hysaishi.cn

[R54] 比较两个文件
来源：http://imn.fengsongda.top

diff a.txt b.txt
来源：http://uqh.hysaishi.cn

[R55] 压缩与解压
来源：http://fab.svipenyu.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://qdj.haohaochexian.top

[R56] 远程拷贝
来源：http://bvs.zhoulong.xyz

scp file user@host:/path/
来源：http://ypu.zhongyouzk.top

[R57] 远程执行命令
来源：http://wul.jinyuanbaomall.cn

ssh user@host 'uptime'
来源：http://sgi.quarkkingdee.top

[R58] 下载文件
来源：http://jsh.bjfxy.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://pyn.jyoumei.cn

[R59] 发 POST JSON
来源：http://etd.andypj.xyz

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://xyn.daxiang520.top

[R60] 只看 HTTP 状态码
来源：http://ukb.yj202588.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://uqj.vehdjk.com

[R61] 磁盘占用
来源：http://xhr.gzhubu.top

df -h;  du -sh *
来源：http://xmt.ehwqpu.com

[R62] 找最占空间的文件
来源：http://svv.guannengcc.top

du -ah . | sort -rh | head -10
来源：http://zxc.yj20258.top

[R63] 内存与进程
来源：http://crr.smart0.xyz

free -h;  ps aux | grep nginx
来源：http://zrp.haohaochexian.top

[R64] 结束进程
来源：http://ixh.yfazqb.com

kill -9 $(pgrep -f app.py)
来源：http://hek.feifeiyinyue.top

[R65] 查看端口占用
来源：http://qvv.sweek.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://zyw.ydjk.org.cn

[R66] 定时任务
来源：http://cuk.gotoacloud.top

crontab -e;  crontab -l
来源：http://qoc.bbcook.cn

[R67] 生成随机十六进制串
来源：http://gkq.yonumen.top

openssl rand -hex 16
来源：http://zkv.hfpthk.cn

[R68] 计算文件校验值
来源：http://zmv.sjlbkw.cn

sha256sum a.txt;  md5sum a.txt
来源：http://mpe.pengpengdd.cyou

[R69] 生成随机密码
来源：http://asb.yuanzhike.top

head -c 16 /dev/urandom | base64
来源：http://qqi.yueranfly.top

[R70] 时间戳与互转
来源：http://izt.cqqwz.cn

date +%s;  date -d @1700000000
来源：http://gbb.zycfv.cn

[R71] 日期格式化
来源：http://xgm.jinqigufen.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://yod.epnwcf.com

[R72] 等待端口就绪
来源：http://wyu.jinghuilouyu.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://poz.tarul.cn

[R73] 分割大日志
来源：http://esh.zhongyouzk.top

split -l 1000 big.log part_
来源：http://vrb.xuanzx.com

[R74] 批量重命名
来源：http://cbb.gaohongyu789.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://jvp.sufxvd.cn

[R75] 导出环境变量
来源：http://cis.pengpengdd.cyou

export PATH="$HOME/bin:$PATH"
来源：http://xqi.iojbl.cn

[R76] 使用临时文件
来源：http://sya.yongpay.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://mun.cucudq.cn

[R77] 读取用户输入
来源：http://dny.9152youxi.cn

read -rp "请输入: " ans
来源：http://zwj.sufxvd.cn

[R78] 交互式菜单
来源：http://hdx.epnwcf.com

select opt in a b c; do echo "$opt"; break; done
来源：http://zjz.wangdashe.top

[R79] 解析命令行选项
来源：http://dxl.zhaomingkeji.xyz

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://xkv.nwbrower.top

[R80] 查看脚本执行耗时
来源：http://sdf.zhiwuduotai.top

time ./run.sh
来源：http://rua.cheryme.top

================================================================================
来源：http://nsx.hammf.cn

S. C / C++ 专题
来源：http://sde.redwolf501.top

================================================================================
来源：http://zii.zdqjudy.top

[S01] C：Hello World
来源：http://zkp.pycfn.com

#include <stdio.h>
来源：http://ktr.sweek.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://epd.sweek.top

[S02] C：变量与格式化输出
来源：http://trl.yvedp.cn

int a = 10; printf("%d\n", a);
来源：http://ylh.xingfuxueyuan.xyz

[S03] C：读入整数
来源：http://xsd.xuetiantiany.cn

int x; scanf("%d", &x);
来源：http://abc.shanyushiyangkeji.top

[S04] C：字符串复制
来源：http://sqp.ydjk.org.cn

char dst[32]; strcpy(dst, "hi");
来源：http://msd.yongpay.top

[S05] C：字符串长度
来源：http://wse.daria6918.cn

strlen(s)
来源：http://wmy.jinqigfzy.top

[S06] C：字符串比较
来源：http://vpr.yj20258888.top

strcmp(a, b) == 0
来源：http://txj.ivvv.top

[S07] C：数组遍历求和
来源：http://aml.gogol.net.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://mps.ppjwa.cn

[S08] C：动态内存分配与释放
来源：http://izb.nwbrower.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://exp.kuanghao11.cn

[S09] C：结构体定义与初始化
来源：http://dmd.hammf.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://uot.jiagoushi.top

[S10] C：指针与解引用
来源：http://qgf.nanxuanxn.top

int *p = &a;  *p = 5;
来源：http://rgo.zhoulong.xyz

[S11] C：逐行读文件
来源：http://pfu.cqqwz.cn

FILE *f = fopen("a.txt", "r");
来源：http://ajo.zhaomingkeji.xyz

while (fgets(buf, sizeof buf, f)) { }
来源：http://dor.zhengqikj.top

fclose(f);
来源：http://riw.ydzc1.top

[S12] C：写文件
来源：http://wqf.zhixingplan.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://fbj.ydzc1.top

[S13] C：宏定义
来源：http://foy.jlsjyb.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://sbq.zhaomingkeji.xyz

[S14] C：枚举
来源：http://vvt.shanyushiyangkeji.top

enum Color { RED, GREEN, BLUE };
来源：http://ibc.hammf.cn

[S15] C：类型转换
来源：http://wgf.hesvh.cn

(double) a / b
来源：http://chj.yangfankeji.com

[S16] C：位操作置位
来源：http://uja.chenlongwang.top

x |= (1 << 3);
来源：http://stg.jiagoushi.top

[S17] C：安全拼接字符串
来源：http://txr.cashguo.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://zie.gaohongyu789.top

[S18] C：命令行参数
来源：http://xlv.cheryme.top

int main(int argc, char **argv)
来源：http://tph.epnwcf.com

[S19] C：快速排序
来源：http://bmb.jqgufenzy.top

qsort(a, n, sizeof(int), cmp);
来源：http://nlh.hnxiangtu.top

[S20] C：二分查找
来源：http://lhg.gzhubu.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://uuh.birdmap.top

[S21] C：字符类别判断
来源：http://sve.cqqwz.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://kst.jlsjyb.cn

[S22] C：字符串转数字
来源：http://bfc.fengsongda.top

atoi("42");  strtod("3.14", NULL);
来源：http://tky.zdbjq.cn

[S23] C：随机数
来源：http://jej.jqgfzy.top

srand(time(NULL));  int r = rand() % 100;
来源：http://nna.chenjidiqi.icu

[S24] C：获取本地时间
来源：http://wjq.xinyue.icu

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://wju.yongpay.top

[S25] C：内存拷贝
来源：http://bpf.xinyue.icu

memcpy(dst, src, n);
来源：http://vlu.fengsongda.top

[S26] C：内存清零
来源：http://ldb.sxryk.cn

memset(a, 0, sizeof a);
来源：http://rnp.tarul.cn

[S27] C：定义常量
来源：http://wky.shanyushiyangkeji.top

const double PI = 3.14159;
来源：http://qcb.cdnleiting.top

[S28] C：静态变量
来源：http://tpg.tanke756.top

static int counter = 0;
来源：http://cqd.zycfv.cn

[S29] C：变参函数
来源：http://qib.daxiang520.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://kjt.havefunace.top

[S30] C：头文件保护
来源：http://nyb.meibo888.top

#ifndef X_H
来源：http://yva.jinyuanbaomall.cn

#define X_H
来源：http://ert.sjlbkw.cn

#endif
来源：http://brw.jinghuilouyu.cn

[S31] C++：Hello World
来源：http://pdq.cdnleiting.top

#include <iostream>
来源：http://gpr.zhongyouzk.top

int main() { std::cout << "Hello\n"; }
来源：http://idl.zhengqikj.top

[S32] C++：字符串
来源：http://cqh.xylfe.cn

std::string s = "hi";  s += "!";
来源：http://zyn.pengpengdd.cyou

[S33] C++：vector 增删
来源：http://goh.zhijiandao.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://zoa.shangyingyoupin.top

[S34] C++：遍历 vector
来源：http://lbq.xuanzx.com

for (auto &x : v) { std::cout << x; }
来源：http://csc.kuanghao11.cn

[S35] C++：map
来源：http://tht.redwolf501.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wwo.c1oappe.top

[S36] C++：unordered_map
来源：http://egb.sxryk.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://phk.shzxlz.cn

[S37] C++：set
来源：http://lxv.9152youxi.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://phk.zhoulong.xyz

[S38] C++：排序
来源：http://qlq.hysaishi.cn

std::sort(v.begin(), v.end());
来源：http://lyu.jqgufenzy.top

[S39] C++：自定义比较器排序
来源：http://jfz.yj202588.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://ehe.jqgufenzy.top

[S40] C++：查找元素
来源：http://uqg.xziqi.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://pvt.hysaishi.cn

[S41] C++：类与构造函数
来源：http://lmb.yangfankeji.com

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://ejz.chenjidiqi.icu

[S42] C++：继承与虚函数
来源：http://gdu.tanke756.top

class B : public Base { public: void f() override {} };
来源：http://bph.jinqigufen.top

[S43] C++：智能指针
来源：http://mwv.chenzaomai.com

auto p = std::make_unique<int>(5);
来源：http://iuk.gzhubu.top

[S44] C++：引用传参
来源：http://qem.wangdashe.top

void inc(int &x) { ++x; }
来源：http://lpr.tanke756.top

[S45] C++：lambda
来源：http://zqy.ydzc1.top

auto add = [](int a, int b) { return a + b; };
来源：http://uqs.redwolf501.top

[S46] C++：函数模板
来源：http://lor.shuidangran.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://cye.svipenyu.cn

[S47] C++：结构化绑定遍历
来源：http://awq.jinqigufen.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://qxb.yj202588.top

[S48] C++：逐行读文件
来源：http://vmq.jiagoushi.top

std::ifstream in("a.txt");  std::string line;
来源：http://puz.pengpengdd.cyou

while (std::getline(in, line)) { }
来源：http://tny.ydjk.org.cn

[S49] C++：写文件
来源：http://coq.nanxinkj.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://dkk.ydzc1.top

[S50] C++：格式化数字
来源：http://qdt.nanxinkj.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://kxt.vehdjk.com

[S51] C++：显式类型转换
来源：http://qbq.zhoulong.xyz

static_cast<double>(a) / b
来源：http://hwv.yueranfly.top

[S52] C++：const 与 noexcept
来源：http://knk.bjfxy.top

int size() const noexcept { return n_; }
来源：http://isx.yfazqb.com

[S53] C++：移动语义
来源：http://zva.mhx1999.top

std::vector<int> w = std::move(v);
来源：http://ahl.fehbvm.com

[S54] C++：异常处理
来源：http://lpz.hnqzz.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://fdj.jqgfzy.top

[S55] C++：结构化绑定
来源：http://tpv.zhengqikj.top

auto [a, b] = std::make_pair(1, 2);
来源：http://gaw.0kj1m.cn

[S56] C++：optional
来源：http://odd.wangshuangyany.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://ngk.dashuyun.cn

[S57] C++：编译期常量
来源：http://tyq.tanke756.top

constexpr int N = 10;
来源：http://pob.gzhubu.top

[S58] C++：命名空间
来源：http://ymo.zhengqikj.top

namespace ns { int f() { return 1; } }
来源：http://klf.fehbvm.com

[S59] C++：静态断言
来源：http://drk.yvedp.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://ztx.tarul.cn

[S60] C++：遍历并删除元素
来源：http://eps.gogol.net.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://kzh.xinyue.icu

================================================================================
来源：http://tcy.9152youxi.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://rpo.zhengqikj.top

================================================================================
来源：http://lnb.dianchejie.cn

[T01] Kotlin：Hello World
来源：http://zbk.316326.xyz

println("Hello")
来源：http://gqt.yueranfly.top

[T02] Kotlin：变量
来源：http://dyb.zhongyouzk.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://pou.yonumen.top


<!-- 参考信息 -->