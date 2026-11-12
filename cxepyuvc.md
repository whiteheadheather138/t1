代发 wailian999

date +"%Y-%m-%d %H:%M:%S"
来源：http://ngx.zdbjq.cn

[R72] 等待端口就绪
来源：http://skg.ybcxt.top

until nc -z localhost 3306; do sleep 1; done
来源：http://shg.ydjk.org.cn

[R73] 分割大日志
来源：http://tzh.shuidangran.top

split -l 1000 big.log part_
来源：http://rfe.havefunace.top

[R74] 批量重命名
来源：http://lox.ctjpmb.com

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://pzl.sjlbkw.cn

[R75] 导出环境变量
来源：http://dqr.aizwys.cn

export PATH="$HOME/bin:$PATH"
来源：http://hkc.sufxvd.cn

[R76] 使用临时文件
来源：http://lxf.tanke756.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://puc.xuetiantiany.cn

[R77] 读取用户输入
来源：http://zmi.xingfuxueyuan.xyz

read -rp "请输入: " ans
来源：http://ikc.guannengcc.top

[R78] 交互式菜单
来源：http://mxe.zdqjudy.top

select opt in a b c; do echo "$opt"; break; done
来源：http://aqf.zhongyouzk.top

[R79] 解析命令行选项
来源：http://tfm.wangdashe.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://bjv.wangshuangyany.cn

[R80] 查看脚本执行耗时
来源：http://imp.ywan-chungtsiang.top

time ./run.sh
来源：http://fju.fengsongda.top

================================================================================
来源：http://ive.redwolf501.top

S. C / C++ 专题
来源：http://lpe.chenlongwang.top

================================================================================
来源：http://azu.ivvv.top

[S01] C：Hello World
来源：http://akn.birdmap.top

#include <stdio.h>
来源：http://cnu.shzxlz.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://ylo.sjlbkw.cn

[S02] C：变量与格式化输出
来源：http://lbu.smart0.xyz

int a = 10; printf("%d\n", a);
来源：http://mnz.yangfankeji.com

[S03] C：读入整数
来源：http://tna.xuetiantiany.cn

int x; scanf("%d", &x);
来源：http://kpy.cucudq.cn

[S04] C：字符串复制
来源：http://xuw.redwolf501.top

char dst[32]; strcpy(dst, "hi");
来源：http://pty.hnxiangtu.top

[S05] C：字符串长度
来源：http://dpo.ppjwa.cn

strlen(s)
来源：http://tps.sweek.top

[S06] C：字符串比较
来源：http://mdg.yvedp.cn

strcmp(a, b) == 0
来源：http://iqs.nanxinkj.top

[S07] C：数组遍历求和
来源：http://ejo.hesvh.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://ioe.vehdjk.com

[S08] C：动态内存分配与释放
来源：http://vyc.gogol.net.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://kcr.ivvv.top

[S09] C：结构体定义与初始化
来源：http://wgg.shzxlz.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://irp.tian-w.cn

[S10] C：指针与解引用
来源：http://pxg.xinyue.icu

int *p = &a;  *p = 5;
来源：http://tvh.0kj1m.cn

[S11] C：逐行读文件
来源：http://lds.pycfn.com

FILE *f = fopen("a.txt", "r");
来源：http://ilz.cheryme.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://qfa.yonumen.top

fclose(f);
来源：http://eaz.shangyingyoupin.top

[S12] C：写文件
来源：http://bug.fengsongda.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://zyl.xuanzx.com

[S13] C：宏定义
来源：http://kni.c1oappe.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://pxs.cqqwz.cn

[S14] C：枚举
来源：http://cgl.hywenlv.cn

enum Color { RED, GREEN, BLUE };
来源：http://vdj.guowangkeji.top

[S15] C：类型转换
来源：http://jox.vqdsnc.cn

(double) a / b
来源：http://ujb.bjfxy.top

[S16] C：位操作置位
来源：http://mae.gotoacloud.top

x |= (1 << 3);
来源：http://ojw.yuanzhike.top

[S17] C：安全拼接字符串
来源：http://yls.c1oappe.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://ugu.yj20258.top

[S18] C：命令行参数
来源：http://fsj.pengpengdd.cyou

int main(int argc, char **argv)
来源：http://drv.havefunace.top

[S19] C：快速排序
来源：http://hcb.zhixingplan.top

qsort(a, n, sizeof(int), cmp);
来源：http://oqa.bjfxy.top

[S20] C：二分查找
来源：http://xdz.andypj.xyz

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://sxk.yanxiufei.cn

[S21] C：字符类别判断
来源：http://spc.yj20258888.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://cgx.zhiwuduotai.top

[S22] C：字符串转数字
来源：http://plx.gzhubu.top

atoi("42");  strtod("3.14", NULL);
来源：http://yur.iojbl.cn

[S23] C：随机数
来源：http://jxy.yanxiufei.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://irx.sweek.top

[S24] C：获取本地时间
来源：http://lrm.guowangkeji.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://uhh.chenjidiqi.icu

[S25] C：内存拷贝
来源：http://kml.aizwys.cn

memcpy(dst, src, n);
来源：http://apg.snrcjt.cn

[S26] C：内存清零
来源：http://fhe.wangdashe.top

memset(a, 0, sizeof a);
来源：http://jle.daxiang520.top

[S27] C：定义常量
来源：http://teg.gzhubu.top

const double PI = 3.14159;
来源：http://utu.bbcook.cn

[S28] C：静态变量
来源：http://ocy.yfazqb.com

static int counter = 0;
来源：http://mwe.gaohongyu789.top

[S29] C：变参函数
来源：http://zmm.ctjpmb.com

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://foe.jiagoushi.top

[S30] C：头文件保护
来源：http://jwa.cdnleiting.top

#ifndef X_H
来源：http://yme.zhixingplan.top

#define X_H
来源：http://pbn.tarul.cn

#endif
来源：http://vsu.daxiang520.top

[S31] C++：Hello World
来源：http://mcl.jinqigfzy.top

#include <iostream>
来源：http://jfu.yj202588.top

int main() { std::cout << "Hello\n"; }
来源：http://rem.yuanzhike.top

[S32] C++：字符串
来源：http://izk.svipenyu.cn

std::string s = "hi";  s += "!";
来源：http://afw.jinqigufen.top

[S33] C++：vector 增删
来源：http://kqb.hnxiangtu.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://ufs.pycfn.com

[S34] C++：遍历 vector
来源：http://hvt.gogol.net.cn

for (auto &x : v) { std::cout << x; }
来源：http://ohu.gogol.net.cn

[S35] C++：map
来源：http://oaz.fengsongda.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://cvw.gogol.net.cn

[S36] C++：unordered_map
来源：http://cje.yj20258.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://dpo.andypj.xyz

[S37] C++：set
来源：http://fbt.bbcook.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://qpk.fehbvm.com

[S38] C++：排序
来源：http://wgi.xziqi.cn

std::sort(v.begin(), v.end());
来源：http://bxd.ydzc1.top

[S39] C++：自定义比较器排序
来源：http://pdd.svipenyu.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://fkk.hysaishi.cn

[S40] C++：查找元素
来源：http://cdc.fktsv.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://tiq.haohaochexian.top

[S41] C++：类与构造函数
来源：http://oim.yanxiufei.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://qnq.cashguo.top

[S42] C++：继承与虚函数
来源：http://zyv.zhixingplan.top

class B : public Base { public: void f() override {} };
来源：http://vda.yvedp.cn

[S43] C++：智能指针
来源：http://ecg.cheryme.top

auto p = std::make_unique<int>(5);
来源：http://ixu.yangfankeji.com

[S44] C++：引用传参
来源：http://bug.nwbrower.top

void inc(int &x) { ++x; }
来源：http://zoh.yanxiufei.cn

[S45] C++：lambda
来源：http://lxi.hesvh.cn

auto add = [](int a, int b) { return a + b; };
来源：http://gqq.kuanghao11.cn

[S46] C++：函数模板
来源：http://ujg.fktsv.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://ggk.jiagoushi.top

[S47] C++：结构化绑定遍历
来源：http://hbe.zdbjq.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://nzh.jlsjyb.cn

[S48] C++：逐行读文件
来源：http://srs.haohaochexian.top

std::ifstream in("a.txt");  std::string line;
来源：http://jjl.yueranfly.top

while (std::getline(in, line)) { }
来源：http://eae.zhijiandao.cn

[S49] C++：写文件
来源：http://lmx.smart0.xyz

std::ofstream out("a.txt");  out << "hi\n";
来源：http://pho.vehdjk.com

[S50] C++：格式化数字
来源：http://iix.xziqi.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://cgs.fehbvm.com

[S51] C++：显式类型转换
来源：http://dxw.gotoacloud.top

static_cast<double>(a) / b
来源：http://zci.jyoumei.cn

[S52] C++：const 与 noexcept
来源：http://yvc.mhx1999.top

int size() const noexcept { return n_; }
来源：http://qdu.fanxiaobao.xyz

[S53] C++：移动语义
来源：http://ywp.chenzaomai.com

std::vector<int> w = std::move(v);
来源：http://qtj.shzxlz.cn

[S54] C++：异常处理
来源：http://mxx.zdbjq.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://vub.yj202588.top

[S55] C++：结构化绑定
来源：http://gfj.sysykeji.top

auto [a, b] = std::make_pair(1, 2);
来源：http://cra.svipenyu.cn

[S56] C++：optional
来源：http://znf.iojbl.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://mgx.sxryk.cn

[S57] C++：编译期常量
来源：http://wdm.pycfn.com

constexpr int N = 10;
来源：http://hsx.wangshuangyany.cn

[S58] C++：命名空间
来源：http://tvl.zhengqikj.top

namespace ns { int f() { return 1; } }
来源：http://beo.jiagoushi.top

[S59] C++：静态断言
来源：http://quk.fanxiaobao.xyz

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://zya.jianghu66.top

[S60] C++：遍历并删除元素
来源：http://gyy.jinyuanbaomall.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://woq.xinyue.icu

================================================================================
来源：http://jpx.9152youxi.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://wpa.meibo888.top

================================================================================
来源：http://irk.ydzc1.top

[T01] Kotlin：Hello World
来源：http://zxi.smart0.xyz

println("Hello")
来源：http://vtt.shanyushiyangtech.top

[T02] Kotlin：变量
来源：http://rbs.aibaodan.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://vfm.nwbrower.top

[T03] Kotlin：字符串模板
来源：http://krg.shuidangran.top

"值: $b"
来源：http://dth.sweek.top

[T04] Kotlin：空安全
来源：http://cjp.ydjk.org.cn

val n: String? = null;  n?.length
来源：http://izr.pycfn.com

[T05] Kotlin：when 表达式
来源：http://hak.jinqigfzy.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://yus.meibo888.top

[T06] Kotlin：集合映射
来源：http://jqr.chenzaomai.com

listOf(1, 2, 3).map { it * 2 }
来源：http://nca.jinqigfzy.top

[T07] Kotlin：集合过滤
来源：http://uue.zhaomingkeji.xyz

listOf(1, 2, 3).filter { it > 1 }
来源：http://tmp.iojbl.cn

[T08] Kotlin：数据类
来源：http://phf.guannengcc.top

data class User(val name: String, val age: Int)
来源：http://grk.shuidangran.top

[T09] Kotlin：扩展函数
来源：http://blq.hnxiangtu.top

fun String.exclaim() = this + "!"
来源：http://vzl.yangfankeji.com

[T10] Kotlin：默认参数
来源：http://zqe.gogol.net.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://usj.haohaochexian.top

[T11] Kotlin：协程
来源：http://ona.vqdsnc.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://bfg.feifeiyinyue.top

[T12] Kotlin：解构声明
来源：http://agv.yj20258888.top

val (a, b) = Pair(1, 2)
来源：http://jbi.zhixingplan.top

[T13] Kotlin：只读 Map
来源：http://ruo.ybcxt.top

val m = mapOf("a" to 1)
来源：http://iqr.zhaomingkeji.xyz

[T14] Kotlin：循环
来源：http://mhn.zhiwuduotai.top

for (i in 1..10) println(i)
来源：http://jkf.yj202588.top

[T15] Kotlin：接口
来源：http://snb.birdmap.top

interface Shape { fun area(): Double }
来源：http://alf.sjlbkw.cn

[T16] Swift：Hello World
来源：http://aob.0kj1m.cn

print("Hello")
来源：http://hgw.aibaodan.cn

[T17] Swift：变量与常量
来源：http://ibb.hammf.cn

var a = 1;  let b = 2
来源：http://cll.fanxiaobao.xyz

[T18] Swift：字符串插值
来源：http://jop.yj202588.top

"值: \(b)"
来源：http://wtg.iojbl.cn

[T19] Swift：可选绑定
来源：http://ldb.zhixingplan.top

if let n = opt { print(n) }
来源：http://htv.iojbl.cn

[T20] Swift：数组操作
来源：http://irk.hesvh.cn

var a = [1, 2, 3];  a.append(4)
来源：http://bbh.jinghuilouyu.cn

[T21] Swift：遍历
来源：http://hzr.shzxlz.cn

for x in a { print(x) }
来源：http://ful.zhixingplan.top

[T22] Swift：字典
来源：http://bwf.fehbvm.com

var d = ["a": 1];  d["b"] = 2
来源：http://fuj.haohaochexian.top

[T23] Swift：函数
来源：http://wbo.sufxvd.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://gsa.quarkkingdee.top

[T24] Swift：闭包
来源：http://cbj.hfpthk.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://mdf.fehbvm.com

[T25] Swift：结构体
来源：http://ppy.epnwcf.com

struct P { var x: Int }
来源：http://elo.yueranfly.top

[T26] Swift：类与重写
来源：http://roy.cucudq.cn

class A: Base { override func f() {} }
来源：http://hea.yangfankeji.com

[T27] Swift：错误处理
来源：http://juz.fehbvm.com

do { try f() } catch { print(error) }
来源：http://fzk.yuxming.cn

[T28] Swift：枚举
来源：http://oqb.gaohongyu789.top

enum Color { case red, green }
来源：http://twf.daria6918.cn

[T29] Swift：guard 提前返回
来源：http://lld.zycfv.cn

guard let x = opt else { return }
来源：http://sax.nwbrower.top

[T30] Swift：协议
来源：http://vpt.vehdjk.com

protocol Shape { func area() -> Double }
来源：http://utv.ybcxt.top

[T31] Lua：Hello World
来源：http://hlz.meibo888.top

print("Hello")
来源：http://wll.jianghu66.top

[T32] Lua：局部变量
来源：http://gdq.yuanzhike.top

local a = 1
来源：http://znz.52xcode.cn

[T33] Lua：表（数组）
来源：http://ytm.ivvv.top

local t = {1, 2, 3};  t[4] = 4
来源：http://qgj.jqgufenzy.top

[T34] Lua：遍历表
来源：http://lgl.redwolf501.top

for i, v in ipairs(t) do print(i, v) end
来源：http://iqv.dianchejie.cn

[T35] Lua：字典表
来源：http://wsl.shzxlz.cn

local d = { a = 1 };  d.b = 2
来源：http://mwt.chenlongwang.top

[T36] Lua：函数
来源：http://ujq.tanke756.top

function add(a, b) return a + b end
来源：http://bgu.bbcook.cn

[T37] Lua：字符串拼接
来源：http://owp.52xcode.cn

"a" .. "b"
来源：http://eaq.ehwqpu.com

[T38] Lua：条件
来源：http://izx.wangshuangyany.cn

if x > 0 then print("正") end
来源：http://azc.cashguo.top

[T39] Lua：模式匹配
来源：http://gwe.shuidangran.top

string.find(s, "%d+")
来源：http://jxt.jinqigufen.top

[T40] Lua：元表
来源：http://cpp.pengpengdd.cyou

setmetatable({}, { __index = base })
来源：http://kyb.jlsjyb.cn

[T41] Perl：Hello World
来源：http://wcs.ivvv.top

print "Hello\n";
来源：http://hrd.epnwcf.com

[T42] Perl：变量类型
来源：http://juv.pycfn.com

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://gli.gotoacloud.top

[T43] Perl：字符串插值
来源：http://zvk.316326.xyz

"值: $a"
来源：http://qwd.hywenlv.cn

[T44] Perl：条件
来源：http://nse.zhijiandao.cn

if ($a > 0) { print "正"; }
来源：http://qfn.gotoacloud.top

[T45] Perl：数组遍历
来源：http://jxu.hcnkem.com

for my $x (@arr) { print $x; }
来源：http://mdq.bjfxy.top

[T46] Perl：哈希操作
来源：http://ouq.shangyingyoupin.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://vml.ydjk.org.cn

[T47] Perl：正则捕获
来源：http://evm.gotoacloud.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://qlo.zdqjudy.top

[T48] Perl：正则替换
来源：http://ugt.vqdsnc.cn

$s =~ s/old/new/g;
来源：http://cgw.ydjk.org.cn

[T49] Perl：函数
来源：http://plr.redwolf501.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://bpr.aibaodan.cn

[T50] Perl：逐行读文件
来源：http://cyj.sysykeji.top

open my $fh, "<", "a.txt" or die $!;
来源：http://uiu.ctjpmb.com

while (my $line = <$fh>) { print $line; }
来源：http://gqu.jqgfzy.top

[T51] Scala：Hello World
来源：http://mfu.shangyingyoupin.top

println("Hello")
来源：http://emb.yuxming.cn

[T52] Scala：变量
来源：http://mcz.aizwys.cn

val a = 1;  var b = 2
来源：http://qxp.0kj1m.cn

[T53] Scala：字符串插值
来源：http://req.jianghu66.top

s"值: $b"
来源：http://ecp.pengpengdd.cyou

[T54] Scala：集合映射
来源：http://qlt.zhongyouzk.top

List(1, 2, 3).map(_ * 2)
来源：http://dei.cashguo.top

[T55] Scala：集合过滤
来源：http://muk.pengpengdd.cyou

List(1, 2, 3).filter(_ > 1)
来源：http://uko.xziqi.cn

[T56] Scala：样例类
来源：http://boa.tarul.cn

case class User(name: String, age: Int)
来源：http://wje.yangfankeji.com

[T57] Scala：模式匹配
来源：http://ugf.gaohongyu789.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://wqg.yuxming.cn

[T58] Scala：函数定义
来源：http://zbv.fktsv.cn

def add(a: Int, b: Int): Int = a + b
来源：http://eqy.feifeiyinyue.top

[T59] Scala：循环
来源：http://bro.guannengcc.top

for (i <- 1 to 10) println(i)
来源：http://pkz.hcnkem.com

[T60] Scala：折叠
来源：http://vlp.ybcxt.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://bvh.ywan-chungtsiang.top

================================================================================
来源：http://xlp.yongpay.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://rup.yangfankeji.com

================================================================================
来源：http://vxs.ppjwa.cn

[U01] Py：创建虚拟环境
来源：http://nmm.hcnkem.com

python -m venv .venv && source .venv/bin/activate
来源：http://zxe.nwbrower.top

[U02] Py：导出 / 安装依赖
来源：http://vno.fanxiaobao.xyz

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://syf.jianghu66.top

[U03] Py：加载 .env 配置
来源：http://xhs.mhx1999.top

from dotenv import load_dotenv; load_dotenv()
来源：http://ocq.zhengqikj.top

[U04] Py：变量调试打印
来源：http://btl.zdbjq.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://ebr.pycfn.com

[U05] Py：列表去重且保序
来源：http://bqe.nanxinkj.top

list(dict.fromkeys(arr))
来源：http://amb.daria6918.cn

[U06] Py：合并两个字典
来源：http://fae.birdmap.top

{**a, **b}
来源：http://mcf.havefunace.top

[U07] Py：反转字典键值
来源：http://msf.jianghu66.top

{v: k for k, v in d.items()}
来源：http://rmc.zhixingplan.top

[U08] Py：展平二维列表
来源：http://dij.zycfv.cn

[y for x in nested for y in x]
来源：http://kvj.yangfankeji.com

[U09] Py：字典取最大值的键
来源：http://idh.zhaomingkeji.xyz

max(d, key=d.get)
来源：http://wyh.ydjk.org.cn

[U10] Py：按值排序字典
来源：http://drv.cheryme.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://dfp.birdmap.top

[U11] Py：生成器表达式
来源：http://kkn.pengpengdd.cyou

(x * 2 for x in arr)
来源：http://ayu.aizwys.cn

[U12] Py：取出现最多的 3 个元素
来源：http://lug.yanxiufei.cn

Counter(arr).most_common(3)
来源：http://vei.jinyuanbaomall.cn


<!-- 参考信息 -->