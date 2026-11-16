代发 wailian999

for i in {1..10}; do echo "$i"; done
来源：http://qcz.zdqjudy.top

[R14] C 风格 for
来源：http://bvo.yvedp.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://ige.zdqjudy.top

[R15] while 逐行读文件
来源：http://fmi.hcnkem.com

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://fql.jianghu66.top

[R16] until 等待条件
来源：http://xjv.daxiang520.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://axt.ywan-chungtsiang.top

[R17] 数组定义与取值
来源：http://aqv.wangshuangyany.cn

arr=(a b c); echo "${arr[0]}"
来源：http://rlw.xuetiantiany.cn

[R18] 遍历数组
来源：http://ago.tarul.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://wsf.zdqjudy.top

[R19] 数组长度
来源：http://iqp.0kj1m.cn

echo "${#arr[@]}"
来源：http://qpt.fzhhl.top

[R20] 关联数组（字典）
来源：http://thu.ctjpmb.com

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://xyx.zhongyouzk.top

[R21] 字符串长度
来源：http://jjg.c1oappe.top

echo "${#s}"
来源：http://nty.xuanzx.com

[R22] 截取子串
来源：http://qah.yvedp.cn

echo "${s:0:5}"
来源：http://esg.shuidangran.top

[R23] 字符串替换
来源：http://juy.svipenyu.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://wfr.shanyushiyangtech.top

[R24] 大小写转换
来源：http://kxx.hammf.cn

echo "${s^^}"; echo "${s,,}"
来源：http://jhk.yuanzhike.top

[R25] 去后缀 / 去前缀
来源：http://akm.tianlin.xyz

echo "${f%.txt}"; echo "${f#./}"
来源：http://ioe.gotoacloud.top

[R26] 命令替换
来源：http://lpz.sufxvd.cn

now=$(date +%F); echo "$now"
来源：http://jha.zdbjq.cn

[R27] 算术展开
来源：http://dsy.iojbl.cn

echo $((1 + 2 * 3))
来源：http://egf.sxryk.cn

[R28] 浮点运算
来源：http://wum.52xcode.cn

echo "scale=2; 10/3" | bc
来源：http://khk.yfazqb.com

[R29] 定义函数
来源：http://dfs.yfazqb.com

add() { echo $(($1 + $2)); }; add 1 2
来源：http://nmt.tanke756.top

[R30] 函数返回状态码
来源：http://jwr.guowangkeji.top

f() { return 0; }; f || echo "失败了"
来源：http://olk.sysykeji.top

[R31] 局部变量
来源：http://pfk.ywan-chungtsiang.top

f() { local x=1; echo "$x"; }
来源：http://xtb.c1oappe.top

[R32] 参数个数校验
来源：http://sqm.aizwys.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://wlk.fehbvm.com

[R33] 捕获错误并提示行号
来源：http://iab.mhx1999.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://nxc.daria6918.cn

[R34] 退出时清理
来源：http://lxb.yvedp.cn

trap 'rm -f "$tmp"' EXIT
来源：http://pjw.daria6918.cn

[R35] 后台执行并等待
来源：http://uvt.sjlbkw.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://tpr.daria6918.cn

[R36] 并发执行多个任务
来源：http://pqz.shanyushiyangkeji.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://lks.redwolf501.top

[R37] 把输出赋给变量
来源：http://asp.c1oappe.top

files=$(ls -1)
来源：http://twj.nanxuanxn.top

[R38] 管道串联
来源：http://agp.gaohongyu789.top

cat a.txt | grep -i error | wc -l
来源：http://tfm.chenjidiqi.icu

[R39] 重定向标准输出与错误
来源：http://fsa.pycfn.com

cmd > out.log 2>&1
来源：http://oob.cheryme.top

[R40] 追加写日志
来源：http://grx.dianchejie.cn

echo "log" >> out.log
来源：http://kem.aibaodan.cn

[R41] 丢弃输出
来源：http://nnl.bjfxy.top

cmd >/dev/null 2>&1
来源：http://gjb.fzhhl.top

[R42] 输入重定向
来源：http://rpw.havefunace.top

wc -l < a.txt
来源：http://hah.fengsongda.top

[R43] 按名字查找文件
来源：http://mhb.snrcjt.cn

find . -name "*.log" -type f
来源：http://kau.ybcxt.top

[R44] 按修改时间查找
来源：http://sgr.fanxiaobao.xyz

find . -mtime -7 -type f
来源：http://ywp.gotoacloud.top

[R45] 批量删除
来源：http://wmi.aibaodan.cn

find . -name "*.tmp" -delete
来源：http://zwo.jianghu66.top

[R46] 递归替换文件内容
来源：http://lov.uphjek.com

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://iuo.cucudq.cn

[R47] sed 单行替换
来源：http://gxd.ehwqpu.com

sed -i 's/foo/bar/g' a.txt
来源：http://usp.316326.xyz

[R48] awk 取指定列
来源：http://ues.guowangkeji.top

awk '{print $1, $3}' a.txt
来源：http://qen.daxiang520.top

[R49] awk 带条件
来源：http://byx.kuanghao11.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://jte.zdqjudy.top

[R50] awk 求和
来源：http://shu.hysaishi.cn

awk '{s += $2} END {print s}' a.txt
来源：http://dac.ydzc1.top

[R51] 排序去重取前几
来源：http://hkk.yueranfly.top

sort a.txt | uniq -c | sort -rn | head
来源：http://arr.iojbl.cn

[R52] 统计行数
来源：http://ylf.zhengqikj.top

wc -l a.txt
来源：http://xvm.nanxinkj.top

[R53] 查看文件头与实时尾
来源：http://fts.zhiwuduotai.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://bkv.aizwys.cn

[R54] 比较两个文件
来源：http://skg.haohaochexian.top

diff a.txt b.txt
来源：http://vmr.jqgfzy.top

[R55] 压缩与解压
来源：http://wqn.jinghuilouyu.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://dot.sxryk.cn

[R56] 远程拷贝
来源：http://azx.tanke756.top

scp file user@host:/path/
来源：http://rky.jyoumei.cn

[R57] 远程执行命令
来源：http://fdl.0kj1m.cn

ssh user@host 'uptime'
来源：http://wkz.zdqjudy.top

[R58] 下载文件
来源：http://rxe.shanyushiyangkeji.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://upk.haohaochexian.top

[R59] 发 POST JSON
来源：http://jgj.zhoulong.xyz

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://fch.nanxinkj.top

[R60] 只看 HTTP 状态码
来源：http://fbw.gaohongyu789.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://etd.yonumen.top

[R61] 磁盘占用
来源：http://yjd.bjfxy.top

df -h;  du -sh *
来源：http://yep.shanyushiyangtech.top

[R62] 找最占空间的文件
来源：http://qer.ybcxt.top

du -ah . | sort -rh | head -10
来源：http://jye.jinghuilouyu.cn

[R63] 内存与进程
来源：http://xpz.redwolf501.top

free -h;  ps aux | grep nginx
来源：http://oiy.yuxming.cn

[R64] 结束进程
来源：http://aem.hcnkem.com

kill -9 $(pgrep -f app.py)
来源：http://tes.haohaochexian.top

[R65] 查看端口占用
来源：http://pqr.yvedp.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://lbc.nanxinkj.top

[R66] 定时任务
来源：http://nje.shanyushiyangkeji.top

crontab -e;  crontab -l
来源：http://feq.jqgfzy.top

[R67] 生成随机十六进制串
来源：http://wnl.xziqi.cn

openssl rand -hex 16
来源：http://ciu.316326.xyz

[R68] 计算文件校验值
来源：http://ikl.tianlin.xyz

sha256sum a.txt;  md5sum a.txt
来源：http://fzp.bbcook.cn

[R69] 生成随机密码
来源：http://wsn.zycfv.cn

head -c 16 /dev/urandom | base64
来源：http://gbk.zhongyouzk.top

[R70] 时间戳与互转
来源：http://syd.wangshuangyany.cn

date +%s;  date -d @1700000000
来源：http://jdd.chenjidiqi.icu

[R71] 日期格式化
来源：http://xla.jianghu66.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://oii.yj202588.top

[R72] 等待端口就绪
来源：http://jyq.zhengqikj.top

until nc -z localhost 3306; do sleep 1; done
来源：http://vnp.sxryk.cn

[R73] 分割大日志
来源：http://pai.jinghuilouyu.cn

split -l 1000 big.log part_
来源：http://xyx.yanxiufei.cn

[R74] 批量重命名
来源：http://bkp.nwbrower.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://tav.dashuyun.cn

[R75] 导出环境变量
来源：http://ipu.sufxvd.cn

export PATH="$HOME/bin:$PATH"
来源：http://wuo.epnwcf.com

[R76] 使用临时文件
来源：http://tfd.xylfe.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://kkp.zdbjq.cn

[R77] 读取用户输入
来源：http://kwi.zhiwuduotai.top

read -rp "请输入: " ans
来源：http://res.quarkkingdee.top

[R78] 交互式菜单
来源：http://lcs.yuanzhike.top

select opt in a b c; do echo "$opt"; break; done
来源：http://qel.nanxinkj.top

[R79] 解析命令行选项
来源：http://toy.aibaodan.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://pql.quarkkingdee.top

[R80] 查看脚本执行耗时
来源：http://xwx.jianghu66.top

time ./run.sh
来源：http://zqe.dashuyun.cn

================================================================================
来源：http://yzf.fengsongda.top

S. C / C++ 专题
来源：http://wvj.52xcode.cn

================================================================================
来源：http://dlh.cdnleiting.top

[S01] C：Hello World
来源：http://ptc.sufxvd.cn

#include <stdio.h>
来源：http://ywb.nanxinkj.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://fyg.hammf.cn

[S02] C：变量与格式化输出
来源：http://yaz.chenjidiqi.icu

int a = 10; printf("%d\n", a);
来源：http://ddr.hnxiangtu.top

[S03] C：读入整数
来源：http://mjy.jqgufenzy.top

int x; scanf("%d", &x);
来源：http://awi.zhoulong.xyz

[S04] C：字符串复制
来源：http://mlz.yonumen.top

char dst[32]; strcpy(dst, "hi");
来源：http://jvd.yonumen.top

[S05] C：字符串长度
来源：http://qit.bbcook.cn

strlen(s)
来源：http://oig.xylfe.cn

[S06] C：字符串比较
来源：http://xaq.ywan-chungtsiang.top

strcmp(a, b) == 0
来源：http://fgv.haohaochexian.top

[S07] C：数组遍历求和
来源：http://rdd.daria6918.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://yqq.snrcjt.cn

[S08] C：动态内存分配与释放
来源：http://ccp.xingfuxueyuan.xyz

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://dst.guannengcc.top

[S09] C：结构体定义与初始化
来源：http://ygn.ctjpmb.com

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://kff.epnwcf.com

[S10] C：指针与解引用
来源：http://zdq.jianghu66.top

int *p = &a;  *p = 5;
来源：http://dur.gzhubu.top

[S11] C：逐行读文件
来源：http://xiz.zhixingplan.top

FILE *f = fopen("a.txt", "r");
来源：http://aht.smart0.xyz

while (fgets(buf, sizeof buf, f)) { }
来源：http://nnp.gogol.net.cn

fclose(f);
来源：http://gno.9152youxi.cn

[S12] C：写文件
来源：http://mzb.yongpay.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://jqg.hysaishi.cn

[S13] C：宏定义
来源：http://qox.sjlbkw.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wug.sufxvd.cn

[S14] C：枚举
来源：http://xkl.bbcook.cn

enum Color { RED, GREEN, BLUE };
来源：http://ouy.smart0.xyz

[S15] C：类型转换
来源：http://crh.jianghu66.top

(double) a / b
来源：http://ebd.cheryme.top

[S16] C：位操作置位
来源：http://txy.fktsv.cn

x |= (1 << 3);
来源：http://xei.gotoacloud.top

[S17] C：安全拼接字符串
来源：http://nje.yfazqb.com

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://vkt.zhijiandao.cn

[S18] C：命令行参数
来源：http://lqh.vqdsnc.cn

int main(int argc, char **argv)
来源：http://acx.hcnkem.com

[S19] C：快速排序
来源：http://isa.ivvv.top

qsort(a, n, sizeof(int), cmp);
来源：http://fkw.zhoulong.xyz

[S20] C：二分查找
来源：http://rzw.dashuyun.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://sia.yuanzhike.top

[S21] C：字符类别判断
来源：http://lux.ehwqpu.com

isdigit(c);  isalpha(c);  isspace(c);
来源：http://nos.shangyingyoupin.top

[S22] C：字符串转数字
来源：http://qtl.iojbl.cn

atoi("42");  strtod("3.14", NULL);
来源：http://swn.hesvh.cn

[S23] C：随机数
来源：http://tmq.feifeiyinyue.top

srand(time(NULL));  int r = rand() % 100;
来源：http://qnw.yueranfly.top

[S24] C：获取本地时间
来源：http://qxt.zhaomingkeji.xyz

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://tbq.zhengqikj.top

[S25] C：内存拷贝
来源：http://pvn.yangfankeji.com

memcpy(dst, src, n);
来源：http://rsu.snrcjt.cn

[S26] C：内存清零
来源：http://ogx.hysaishi.cn

memset(a, 0, sizeof a);
来源：http://dvj.feifeiyinyue.top

[S27] C：定义常量
来源：http://wap.fanxiaobao.xyz

const double PI = 3.14159;
来源：http://kbk.yj202588.top

[S28] C：静态变量
来源：http://med.snrcjt.cn

static int counter = 0;
来源：http://obh.jinghuilouyu.cn

[S29] C：变参函数
来源：http://vgp.yuanzhike.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://zju.ppjwa.cn

[S30] C：头文件保护
来源：http://bqi.shangyingyoupin.top

#ifndef X_H
来源：http://zlj.c1oappe.top

#define X_H
来源：http://rqb.ydzc1.top

#endif
来源：http://gyr.hesvh.cn

[S31] C++：Hello World
来源：http://idp.jyoumei.cn

#include <iostream>
来源：http://krz.uphjek.com

int main() { std::cout << "Hello\n"; }
来源：http://ziu.wangdashe.top

[S32] C++：字符串
来源：http://kpm.ppjwa.cn

std::string s = "hi";  s += "!";
来源：http://xok.snrcjt.cn

[S33] C++：vector 增删
来源：http://zxs.jianghu66.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://tmd.xylfe.cn

[S34] C++：遍历 vector
来源：http://gkn.kuanghao11.cn

for (auto &x : v) { std::cout << x; }
来源：http://vhc.fzhhl.top

[S35] C++：map
来源：http://gkg.shangyingyoupin.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://qky.dashuyun.cn

[S36] C++：unordered_map
来源：http://gzp.pengpengdd.cyou

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://dbu.uphjek.com

[S37] C++：set
来源：http://ndj.epnwcf.com

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://pks.zhixingplan.top

[S38] C++：排序
来源：http://ovu.yueranfly.top

std::sort(v.begin(), v.end());
来源：http://xcm.jianghu66.top

[S39] C++：自定义比较器排序
来源：http://xiv.yueranfly.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://rrp.chenzaomai.com

[S40] C++：查找元素
来源：http://vbg.guannengcc.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://eyi.fehbvm.com

[S41] C++：类与构造函数
来源：http://biv.zhixingplan.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://xwy.gotoacloud.top

[S42] C++：继承与虚函数
来源：http://mle.epnwcf.com

class B : public Base { public: void f() override {} };
来源：http://bgi.cucudq.cn

[S43] C++：智能指针
来源：http://ydc.zdbjq.cn

auto p = std::make_unique<int>(5);
来源：http://cui.sxryk.cn

[S44] C++：引用传参
来源：http://wfl.shuidangran.top

void inc(int &x) { ++x; }
来源：http://uxm.birdmap.top

[S45] C++：lambda
来源：http://hrf.zdbjq.cn

auto add = [](int a, int b) { return a + b; };
来源：http://iae.jiagoushi.top

[S46] C++：函数模板
来源：http://myy.xuanzx.com

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://lgc.epnwcf.com

[S47] C++：结构化绑定遍历
来源：http://jyc.sysykeji.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://jho.shzxlz.cn

[S48] C++：逐行读文件
来源：http://hmy.aibaodan.cn

std::ifstream in("a.txt");  std::string line;
来源：http://fxl.cashguo.top

while (std::getline(in, line)) { }
来源：http://phx.jlsjyb.cn

[S49] C++：写文件
来源：http://nwn.yanxiufei.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://vws.daxiang520.top

[S50] C++：格式化数字
来源：http://bee.52xcode.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://yiu.shanyushiyangkeji.top

[S51] C++：显式类型转换
来源：http://ysn.xziqi.cn

static_cast<double>(a) / b
来源：http://sju.vqdsnc.cn

[S52] C++：const 与 noexcept
来源：http://rkq.epnwcf.com

int size() const noexcept { return n_; }
来源：http://jgv.zhengqikj.top

[S53] C++：移动语义
来源：http://qmu.zhaomingkeji.xyz

std::vector<int> w = std::move(v);
来源：http://lxw.birdmap.top

[S54] C++：异常处理
来源：http://qan.daria6918.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://wrw.shanyushiyangkeji.top

[S55] C++：结构化绑定
来源：http://lox.zhaomingkeji.xyz

auto [a, b] = std::make_pair(1, 2);
来源：http://kvw.aibaodan.cn

[S56] C++：optional
来源：http://yqo.zdbjq.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hqt.yj20258.top

[S57] C++：编译期常量
来源：http://qpj.yonumen.top

constexpr int N = 10;
来源：http://xgn.gzhubu.top

[S58] C++：命名空间
来源：http://rtx.vqdsnc.cn

namespace ns { int f() { return 1; } }
来源：http://sed.hywenlv.cn

[S59] C++：静态断言
来源：http://oqz.tian-w.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://bwm.andypj.xyz

[S60] C++：遍历并删除元素
来源：http://qro.hysaishi.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://dex.daxiang520.top

================================================================================
来源：http://cml.vehdjk.com

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://vwb.cheryme.top

================================================================================
来源：http://kjp.gotoacloud.top

[T01] Kotlin：Hello World
来源：http://uko.nanxuanxn.top

println("Hello")
来源：http://pdc.ydzc1.top

[T02] Kotlin：变量
来源：http://ivl.quarkkingdee.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://tzo.svipenyu.cn

[T03] Kotlin：字符串模板
来源：http://ahw.0kj1m.cn

"值: $b"
来源：http://tzr.birdmap.top

[T04] Kotlin：空安全
来源：http://svr.9152youxi.cn

val n: String? = null;  n?.length
来源：http://iuz.epnwcf.com

[T05] Kotlin：when 表达式
来源：http://bio.shangyingyoupin.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://mvu.ppjwa.cn

[T06] Kotlin：集合映射
来源：http://yar.zhoulong.xyz

listOf(1, 2, 3).map { it * 2 }
来源：http://szf.havefunace.top

[T07] Kotlin：集合过滤
来源：http://afy.epnwcf.com

listOf(1, 2, 3).filter { it > 1 }
来源：http://euv.sysykeji.top

[T08] Kotlin：数据类
来源：http://vqi.zhongyouzk.top

data class User(val name: String, val age: Int)
来源：http://qot.cdnleiting.top

[T09] Kotlin：扩展函数
来源：http://kjl.zhixingplan.top

fun String.exclaim() = this + "!"
来源：http://hdr.yj20258888.top

[T10] Kotlin：默认参数
来源：http://chd.hnxiangtu.top

fun greet(name: String = "World") = "Hi $name"
来源：http://vdd.sjlbkw.cn

[T11] Kotlin：协程
来源：http://cos.fktsv.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://cly.pycfn.com

[T12] Kotlin：解构声明
来源：http://wul.zhongyouzk.top

val (a, b) = Pair(1, 2)
来源：http://vlm.hcnkem.com

[T13] Kotlin：只读 Map
来源：http://yek.birdmap.top

val m = mapOf("a" to 1)
来源：http://wkl.yfazqb.com

[T14] Kotlin：循环
来源：http://hji.yueranfly.top

for (i in 1..10) println(i)
来源：http://rgz.c1oappe.top

[T15] Kotlin：接口
来源：http://bit.epnwcf.com

interface Shape { fun area(): Double }
来源：http://yqt.xuetiantiany.cn

[T16] Swift：Hello World
来源：http://ocn.hongshengwenyu.top

print("Hello")
来源：http://tbe.redwolf501.top


<!-- 参考信息 -->