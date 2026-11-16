代发 wailian999

split -l 1000 big.log part_
来源：http://ayj.cdnleiting.top

[R74] 批量重命名
来源：http://oeh.hesvh.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://nhu.aizwys.cn

[R75] 导出环境变量
来源：http://zmy.cdnleiting.top

export PATH="$HOME/bin:$PATH"
来源：http://ufn.chenlongwang.top

[R76] 使用临时文件
来源：http://lhr.nanxinkj.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://ucg.nwbrower.top

[R77] 读取用户输入
来源：http://qyp.nanxinkj.top

read -rp "请输入: " ans
来源：http://cdd.sweek.top

[R78] 交互式菜单
来源：http://txd.fzhhl.top

select opt in a b c; do echo "$opt"; break; done
来源：http://byg.gogol.net.cn

[R79] 解析命令行选项
来源：http://duc.uphjek.com

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://nhj.shzxlz.cn

[R80] 查看脚本执行耗时
来源：http://yrs.shzxlz.cn

time ./run.sh
来源：http://pjd.smart0.xyz

================================================================================
来源：http://njv.hnqzz.top

S. C / C++ 专题
来源：http://rbm.tianlin.xyz

================================================================================
来源：http://vti.meibo888.top

[S01] C：Hello World
来源：http://hot.hysaishi.cn

#include <stdio.h>
来源：http://cot.guowangkeji.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://ere.jyoumei.cn

[S02] C：变量与格式化输出
来源：http://tem.vqdsnc.cn

int a = 10; printf("%d\n", a);
来源：http://euk.zhengqikj.top

[S03] C：读入整数
来源：http://kaa.xylfe.cn

int x; scanf("%d", &x);
来源：http://ode.tanke756.top

[S04] C：字符串复制
来源：http://mzg.shzxlz.cn

char dst[32]; strcpy(dst, "hi");
来源：http://znh.hcnkem.com

[S05] C：字符串长度
来源：http://ogp.nanxuanxn.top

strlen(s)
来源：http://hoc.epnwcf.com

[S06] C：字符串比较
来源：http://bsp.wangdashe.top

strcmp(a, b) == 0
来源：http://kzx.yfazqb.com

[S07] C：数组遍历求和
来源：http://hax.zhengqikj.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://rpl.nwbrower.top

[S08] C：动态内存分配与释放
来源：http://xcg.sjlbkw.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://leo.xinyue.icu

[S09] C：结构体定义与初始化
来源：http://ifq.316326.xyz

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://pcn.cqqwz.cn

[S10] C：指针与解引用
来源：http://svr.xuetiantiany.cn

int *p = &a;  *p = 5;
来源：http://rkl.quarkkingdee.top

[S11] C：逐行读文件
来源：http://xev.hesvh.cn

FILE *f = fopen("a.txt", "r");
来源：http://tni.jqgufenzy.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://ghq.jinqigufen.top

fclose(f);
来源：http://ozb.gzhubu.top

[S12] C：写文件
来源：http://rnb.hongshengwenyu.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://tkl.yongpay.top

[S13] C：宏定义
来源：http://twt.zhongyouzk.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://yyp.tanke756.top

[S14] C：枚举
来源：http://rgi.gotoacloud.top

enum Color { RED, GREEN, BLUE };
来源：http://wuq.quarkkingdee.top

[S15] C：类型转换
来源：http://obb.jqgufenzy.top

(double) a / b
来源：http://daj.gotoacloud.top

[S16] C：位操作置位
来源：http://vem.aizwys.cn

x |= (1 << 3);
来源：http://uep.bbcook.cn

[S17] C：安全拼接字符串
来源：http://mcr.yj202588.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://vaz.fzhhl.top

[S18] C：命令行参数
来源：http://rce.jiagoushi.top

int main(int argc, char **argv)
来源：http://qnu.pycfn.com

[S19] C：快速排序
来源：http://wfs.shzxlz.cn

qsort(a, n, sizeof(int), cmp);
来源：http://jwt.snrcjt.cn

[S20] C：二分查找
来源：http://rgf.guowangkeji.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://bpv.uphjek.com

[S21] C：字符类别判断
来源：http://jgz.andypj.xyz

isdigit(c);  isalpha(c);  isspace(c);
来源：http://cva.fehbvm.com

[S22] C：字符串转数字
来源：http://dlz.0kj1m.cn

atoi("42");  strtod("3.14", NULL);
来源：http://mob.yanxiufei.cn

[S23] C：随机数
来源：http://wex.iojbl.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://cgf.haohaochexian.top

[S24] C：获取本地时间
来源：http://idw.fanxiaobao.xyz

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://ohq.yfazqb.com

[S25] C：内存拷贝
来源：http://laj.ydjk.org.cn

memcpy(dst, src, n);
来源：http://wjz.yueranfly.top

[S26] C：内存清零
来源：http://lah.zhoulong.xyz

memset(a, 0, sizeof a);
来源：http://ntq.hysaishi.cn

[S27] C：定义常量
来源：http://obl.sjlbkw.cn

const double PI = 3.14159;
来源：http://tbh.gotoacloud.top

[S28] C：静态变量
来源：http://hsd.zhijiandao.cn

static int counter = 0;
来源：http://hhi.yueranfly.top

[S29] C：变参函数
来源：http://ade.shuidangran.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://qed.0kj1m.cn

[S30] C：头文件保护
来源：http://iou.yfazqb.com

#ifndef X_H
来源：http://pvs.zhongyouzk.top

#define X_H
来源：http://gxz.cdnleiting.top

#endif
来源：http://dbx.jyoumei.cn

[S31] C++：Hello World
来源：http://tkw.fehbvm.com

#include <iostream>
来源：http://bsi.hywenlv.cn

int main() { std::cout << "Hello\n"; }
来源：http://rnj.chenzaomai.com

[S32] C++：字符串
来源：http://jow.jinghuilouyu.cn

std::string s = "hi";  s += "!";
来源：http://mal.redwolf501.top

[S33] C++：vector 增删
来源：http://udk.gaohongyu789.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://wcy.9152youxi.cn

[S34] C++：遍历 vector
来源：http://lan.daria6918.cn

for (auto &x : v) { std::cout << x; }
来源：http://wzl.yj20258.top

[S35] C++：map
来源：http://eop.pycfn.com

std::map<std::string, int> m;  m["a"] = 1;
来源：http://dms.hammf.cn

[S36] C++：unordered_map
来源：http://ruq.jyoumei.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://ghc.fengsongda.top

[S37] C++：set
来源：http://xbx.chenlongwang.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://cud.fzhhl.top

[S38] C++：排序
来源：http://cmk.316326.xyz

std::sort(v.begin(), v.end());
来源：http://jac.jinghuilouyu.cn

[S39] C++：自定义比较器排序
来源：http://hlu.daria6918.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://kyc.ywan-chungtsiang.top

[S40] C++：查找元素
来源：http://dvo.cashguo.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://ijr.yj202588.top

[S41] C++：类与构造函数
来源：http://gpz.cucudq.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://ooj.dashuyun.cn

[S42] C++：继承与虚函数
来源：http://lra.sxryk.cn

class B : public Base { public: void f() override {} };
来源：http://gcb.tian-w.cn

[S43] C++：智能指针
来源：http://mcv.chenzaomai.com

auto p = std::make_unique<int>(5);
来源：http://ybh.hnxiangtu.top

[S44] C++：引用传参
来源：http://zmq.guowangkeji.top

void inc(int &x) { ++x; }
来源：http://azz.jinyuanbaomall.cn

[S45] C++：lambda
来源：http://kxs.ydzc1.top

auto add = [](int a, int b) { return a + b; };
来源：http://wwo.gogol.net.cn

[S46] C++：函数模板
来源：http://bkn.fktsv.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://yin.andypj.xyz

[S47] C++：结构化绑定遍历
来源：http://vtl.xuanzx.com

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://uhe.sufxvd.cn

[S48] C++：逐行读文件
来源：http://jfn.sjlbkw.cn

std::ifstream in("a.txt");  std::string line;
来源：http://uhn.mhx1999.top

while (std::getline(in, line)) { }
来源：http://asl.hywenlv.cn

[S49] C++：写文件
来源：http://tif.dianchejie.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://neq.ivvv.top

[S50] C++：格式化数字
来源：http://yji.jinqigfzy.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://qye.jqgufenzy.top

[S51] C++：显式类型转换
来源：http://ijn.fktsv.cn

static_cast<double>(a) / b
来源：http://xzn.tianlin.xyz

[S52] C++：const 与 noexcept
来源：http://bdf.0kj1m.cn

int size() const noexcept { return n_; }
来源：http://qph.epnwcf.com

[S53] C++：移动语义
来源：http://oxo.zhiwuduotai.top

std::vector<int> w = std::move(v);
来源：http://fef.c1oappe.top

[S54] C++：异常处理
来源：http://cvd.zhixingplan.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://fbe.gotoacloud.top

[S55] C++：结构化绑定
来源：http://cgc.ivvv.top

auto [a, b] = std::make_pair(1, 2);
来源：http://bsv.fengsongda.top

[S56] C++：optional
来源：http://zkq.yj20258.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://ghu.fanxiaobao.xyz

[S57] C++：编译期常量
来源：http://ych.wangshuangyany.cn

constexpr int N = 10;
来源：http://arq.xinyue.icu

[S58] C++：命名空间
来源：http://tqm.fengsongda.top

namespace ns { int f() { return 1; } }
来源：http://hnd.sufxvd.cn

[S59] C++：静态断言
来源：http://iws.zhaomingkeji.xyz

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://fdf.fanxiaobao.xyz

[S60] C++：遍历并删除元素
来源：http://pjg.c1oappe.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://kge.guannengcc.top

================================================================================
来源：http://pmm.nanxuanxn.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://owv.yj202588.top

================================================================================
来源：http://wya.hywenlv.cn

[T01] Kotlin：Hello World
来源：http://hhx.jinqigfzy.top

println("Hello")
来源：http://tkz.jinghuilouyu.cn

[T02] Kotlin：变量
来源：http://bpf.haohaochexian.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://lky.jinqigfzy.top

[T03] Kotlin：字符串模板
来源：http://ucr.dianchejie.cn

"值: $b"
来源：http://ncu.chenjidiqi.icu

[T04] Kotlin：空安全
来源：http://mgr.pycfn.com

val n: String? = null;  n?.length
来源：http://uex.daria6918.cn

[T05] Kotlin：when 表达式
来源：http://trn.birdmap.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://lbb.ybcxt.top

[T06] Kotlin：集合映射
来源：http://uho.epnwcf.com

listOf(1, 2, 3).map { it * 2 }
来源：http://gts.tarul.cn

[T07] Kotlin：集合过滤
来源：http://alm.ivvv.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://khl.yj20258.top

[T08] Kotlin：数据类
来源：http://xie.guowangkeji.top

data class User(val name: String, val age: Int)
来源：http://ern.dianchejie.cn

[T09] Kotlin：扩展函数
来源：http://tqr.gogol.net.cn

fun String.exclaim() = this + "!"
来源：http://oun.cucudq.cn

[T10] Kotlin：默认参数
来源：http://mqr.feifeiyinyue.top

fun greet(name: String = "World") = "Hi $name"
来源：http://eco.fzhhl.top

[T11] Kotlin：协程
来源：http://abp.hcnkem.com

GlobalScope.launch { delay(1000); println("done") }
来源：http://olt.9152youxi.cn

[T12] Kotlin：解构声明
来源：http://wxd.sjlbkw.cn

val (a, b) = Pair(1, 2)
来源：http://eml.vehdjk.com

[T13] Kotlin：只读 Map
来源：http://ytp.svipenyu.cn

val m = mapOf("a" to 1)
来源：http://zyf.hnqzz.top

[T14] Kotlin：循环
来源：http://owr.xuanzx.com

for (i in 1..10) println(i)
来源：http://tfh.hcnkem.com

[T15] Kotlin：接口
来源：http://qij.snrcjt.cn

interface Shape { fun area(): Double }
来源：http://itj.fengsongda.top

[T16] Swift：Hello World
来源：http://cdj.zdqjudy.top

print("Hello")
来源：http://tlh.daxiang520.top

[T17] Swift：变量与常量
来源：http://phj.jinqigufen.top

var a = 1;  let b = 2
来源：http://qky.meibo888.top

[T18] Swift：字符串插值
来源：http://zux.birdmap.top

"值: \(b)"
来源：http://xel.zhijiandao.cn

[T19] Swift：可选绑定
来源：http://hsh.zhengqikj.top

if let n = opt { print(n) }
来源：http://mvt.zhiwuduotai.top

[T20] Swift：数组操作
来源：http://wlj.fktsv.cn

var a = [1, 2, 3];  a.append(4)
来源：http://ntm.hysaishi.cn

[T21] Swift：遍历
来源：http://vft.yvedp.cn

for x in a { print(x) }
来源：http://zyy.yj20258888.top

[T22] Swift：字典
来源：http://dzr.svipenyu.cn

var d = ["a": 1];  d["b"] = 2
来源：http://ibm.daxiang520.top

[T23] Swift：函数
来源：http://yit.kuanghao11.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://nks.daxiang520.top

[T24] Swift：闭包
来源：http://pfh.fengsongda.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://ufx.gaohongyu789.top

[T25] Swift：结构体
来源：http://sux.shuidangran.top

struct P { var x: Int }
来源：http://rbw.wangshuangyany.cn

[T26] Swift：类与重写
来源：http://nfs.tanke756.top

class A: Base { override func f() {} }
来源：http://jxg.tarul.cn

[T27] Swift：错误处理
来源：http://rym.ppjwa.cn

do { try f() } catch { print(error) }
来源：http://yej.pengpengdd.cyou

[T28] Swift：枚举
来源：http://fsq.yangfankeji.com

enum Color { case red, green }
来源：http://bay.bbcook.cn

[T29] Swift：guard 提前返回
来源：http://fwp.yuanzhike.top

guard let x = opt else { return }
来源：http://oae.guowangkeji.top

[T30] Swift：协议
来源：http://zlc.zdqjudy.top

protocol Shape { func area() -> Double }
来源：http://lbc.nanxuanxn.top

[T31] Lua：Hello World
来源：http://mzs.hongshengwenyu.top

print("Hello")
来源：http://yze.bjfxy.top

[T32] Lua：局部变量
来源：http://dbc.yvedp.cn

local a = 1
来源：http://ofp.guowangkeji.top

[T33] Lua：表（数组）
来源：http://qqp.yonumen.top

local t = {1, 2, 3};  t[4] = 4
来源：http://hhu.dashuyun.cn

[T34] Lua：遍历表
来源：http://pfu.cashguo.top

for i, v in ipairs(t) do print(i, v) end
来源：http://pbw.mhx1999.top

[T35] Lua：字典表
来源：http://ken.guannengcc.top

local d = { a = 1 };  d.b = 2
来源：http://lnc.ehwqpu.com

[T36] Lua：函数
来源：http://kdy.gotoacloud.top

function add(a, b) return a + b end
来源：http://xhp.xylfe.cn

[T37] Lua：字符串拼接
来源：http://ebd.vehdjk.com

"a" .. "b"
来源：http://tms.andypj.xyz

[T38] Lua：条件
来源：http://ohj.xingfuxueyuan.xyz

if x > 0 then print("正") end
来源：http://yfv.jinqigfzy.top

[T39] Lua：模式匹配
来源：http://tfa.feifeiyinyue.top

string.find(s, "%d+")
来源：http://oid.feifeiyinyue.top

[T40] Lua：元表
来源：http://zzb.dianchejie.cn

setmetatable({}, { __index = base })
来源：http://nxl.hammf.cn

[T41] Perl：Hello World
来源：http://mth.yj20258888.top

print "Hello\n";
来源：http://xti.epnwcf.com

[T42] Perl：变量类型
来源：http://pkz.ybcxt.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://tej.yuanzhike.top

[T43] Perl：字符串插值
来源：http://xty.yj202588.top

"值: $a"
来源：http://yfv.xingfuxueyuan.xyz

[T44] Perl：条件
来源：http://nvv.chenlongwang.top

if ($a > 0) { print "正"; }
来源：http://glo.hammf.cn

[T45] Perl：数组遍历
来源：http://agk.andypj.xyz

for my $x (@arr) { print $x; }
来源：http://fys.jinyuanbaomall.cn

[T46] Perl：哈希操作
来源：http://sfk.hammf.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://osr.wangshuangyany.cn

[T47] Perl：正则捕获
来源：http://afc.gogol.net.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://azm.nanxuanxn.top

[T48] Perl：正则替换
来源：http://jce.nwbrower.top

$s =~ s/old/new/g;
来源：http://mif.fehbvm.com

[T49] Perl：函数
来源：http://amn.yfazqb.com

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://adu.jqgfzy.top

[T50] Perl：逐行读文件
来源：http://lpt.hongshengwenyu.top

open my $fh, "<", "a.txt" or die $!;
来源：http://fzh.chenjidiqi.icu

while (my $line = <$fh>) { print $line; }
来源：http://owh.cucudq.cn

[T51] Scala：Hello World
来源：http://vyx.jqgfzy.top

println("Hello")
来源：http://aji.tanke756.top

[T52] Scala：变量
来源：http://tbx.yonumen.top

val a = 1;  var b = 2
来源：http://cxo.cucudq.cn

[T53] Scala：字符串插值
来源：http://vql.epnwcf.com

s"值: $b"
来源：http://mxj.yanxiufei.cn

[T54] Scala：集合映射
来源：http://gef.hammf.cn

List(1, 2, 3).map(_ * 2)
来源：http://shs.hesvh.cn

[T55] Scala：集合过滤
来源：http://azd.shanyushiyangtech.top

List(1, 2, 3).filter(_ > 1)
来源：http://jsw.jinyuanbaomall.cn

[T56] Scala：样例类
来源：http://urt.sweek.top

case class User(name: String, age: Int)
来源：http://ajx.cashguo.top

[T57] Scala：模式匹配
来源：http://zsa.aibaodan.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://dnu.shanyushiyangtech.top

[T58] Scala：函数定义
来源：http://njy.aibaodan.cn

def add(a: Int, b: Int): Int = a + b
来源：http://mtl.haohaochexian.top

[T59] Scala：循环
来源：http://cun.hysaishi.cn

for (i <- 1 to 10) println(i)
来源：http://dza.havefunace.top

[T60] Scala：折叠
来源：http://yzc.316326.xyz

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://kne.bbcook.cn

================================================================================
来源：http://zym.shanyushiyangkeji.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://ziw.jinghuilouyu.cn

================================================================================
来源：http://kmd.daxiang520.top

[U01] Py：创建虚拟环境
来源：http://foq.tarul.cn

python -m venv .venv && source .venv/bin/activate
来源：http://qjx.wangdashe.top

[U02] Py：导出 / 安装依赖
来源：http://ihn.yangfankeji.com

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://vhs.gaohongyu789.top

[U03] Py：加载 .env 配置
来源：http://pnc.jinyuanbaomall.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://juq.zhaomingkeji.xyz

[U04] Py：变量调试打印
来源：http://kxu.yj20258888.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://btw.svipenyu.cn

[U05] Py：列表去重且保序
来源：http://qtk.yuxming.cn

list(dict.fromkeys(arr))
来源：http://mvu.hammf.cn

[U06] Py：合并两个字典
来源：http://bmf.ydzc1.top

{**a, **b}
来源：http://zvb.sjlbkw.cn

[U07] Py：反转字典键值
来源：http://jlc.hywenlv.cn

{v: k for k, v in d.items()}
来源：http://rgx.cucudq.cn

[U08] Py：展平二维列表
来源：http://quf.cashguo.top

[y for x in nested for y in x]
来源：http://heg.hesvh.cn

[U09] Py：字典取最大值的键
来源：http://xou.zdbjq.cn

max(d, key=d.get)
来源：http://pvk.nanxuanxn.top

[U10] Py：按值排序字典
来源：http://yxj.hongshengwenyu.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://dxc.iojbl.cn

[U11] Py：生成器表达式
来源：http://ejr.gogol.net.cn

(x * 2 for x in arr)
来源：http://ubf.c1oappe.top

[U12] Py：取出现最多的 3 个元素
来源：http://fqh.kuanghao11.cn

Counter(arr).most_common(3)
来源：http://yvl.fzhhl.top

[U13] Py：固定长度队列
来源：http://rkq.ywan-chungtsiang.top

deque(maxlen=10)
来源：http://abb.ehwqpu.com

[U14] Py：分组收集到列表
来源：http://nsi.guowangkeji.top

defaultdict(list)
来源：http://jvf.mhx1999.top


<!-- 参考信息 -->