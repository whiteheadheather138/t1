代发 wailian999

int x; scanf("%d", &x);
来源：http://hzn.hywenlv.cn

[S04] C：字符串复制
来源：http://osl.zdqjudy.top

char dst[32]; strcpy(dst, "hi");
来源：http://bex.sxryk.cn

[S05] C：字符串长度
来源：http://xxw.dashuyun.cn

strlen(s)
来源：http://hys.shangyingyoupin.top

[S06] C：字符串比较
来源：http://vrw.xylfe.cn

strcmp(a, b) == 0
来源：http://tbi.hongshengwenyu.top

[S07] C：数组遍历求和
来源：http://pbk.sxryk.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://mpn.jyoumei.cn

[S08] C：动态内存分配与释放
来源：http://wja.yuanzhike.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://buy.jlsjyb.cn

[S09] C：结构体定义与初始化
来源：http://hoz.yueranfly.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://huz.cucudq.cn

[S10] C：指针与解引用
来源：http://lfi.yvedp.cn

int *p = &a;  *p = 5;
来源：http://oiy.fktsv.cn

[S11] C：逐行读文件
来源：http://irx.cdnleiting.top

FILE *f = fopen("a.txt", "r");
来源：http://qyr.jqgfzy.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://xst.shanyushiyangtech.top

fclose(f);
来源：http://ldw.ybcxt.top

[S12] C：写文件
来源：http://jir.quarkkingdee.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://uyu.yfazqb.com

[S13] C：宏定义
来源：http://gxx.wangshuangyany.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://xga.gotoacloud.top

[S14] C：枚举
来源：http://rxo.ywan-chungtsiang.top

enum Color { RED, GREEN, BLUE };
来源：http://xzi.sweek.top

[S15] C：类型转换
来源：http://kme.zhijiandao.cn

(double) a / b
来源：http://bqq.ppjwa.cn

[S16] C：位操作置位
来源：http://xui.cucudq.cn

x |= (1 << 3);
来源：http://iji.ppjwa.cn

[S17] C：安全拼接字符串
来源：http://her.daxiang520.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://qkt.pengpengdd.cyou

[S18] C：命令行参数
来源：http://esk.uphjek.com

int main(int argc, char **argv)
来源：http://zon.nwbrower.top

[S19] C：快速排序
来源：http://ivs.dashuyun.cn

qsort(a, n, sizeof(int), cmp);
来源：http://lao.yj20258.top

[S20] C：二分查找
来源：http://vyu.gogol.net.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://yhs.fengsongda.top

[S21] C：字符类别判断
来源：http://fiq.yanxiufei.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://iwi.zhijiandao.cn

[S22] C：字符串转数字
来源：http://klp.zycfv.cn

atoi("42");  strtod("3.14", NULL);
来源：http://rpo.daxiang520.top

[S23] C：随机数
来源：http://rvb.xingfuxueyuan.xyz

srand(time(NULL));  int r = rand() % 100;
来源：http://gso.xingfuxueyuan.xyz

[S24] C：获取本地时间
来源：http://jsy.tianlin.xyz

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://fon.tian-w.cn

[S25] C：内存拷贝
来源：http://yxu.haohaochexian.top

memcpy(dst, src, n);
来源：http://gcc.quarkkingdee.top

[S26] C：内存清零
来源：http://esr.kuanghao11.cn

memset(a, 0, sizeof a);
来源：http://xsb.cashguo.top

[S27] C：定义常量
来源：http://ukz.meibo888.top

const double PI = 3.14159;
来源：http://dop.wangdashe.top

[S28] C：静态变量
来源：http://wmp.xylfe.cn

static int counter = 0;
来源：http://ldc.yfazqb.com

[S29] C：变参函数
来源：http://qwe.xuetiantiany.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://zbh.yanxiufei.cn

[S30] C：头文件保护
来源：http://fwa.jinyuanbaomall.cn

#ifndef X_H
来源：http://sgr.zhixingplan.top

#define X_H
来源：http://zbi.havefunace.top

#endif
来源：http://aff.xuanzx.com

[S31] C++：Hello World
来源：http://tkv.52xcode.cn

#include <iostream>
来源：http://fzo.jinqigufen.top

int main() { std::cout << "Hello\n"; }
来源：http://ubs.fengsongda.top

[S32] C++：字符串
来源：http://hqu.yueranfly.top

std::string s = "hi";  s += "!";
来源：http://cyo.hcnkem.com

[S33] C++：vector 增删
来源：http://frk.yj202588.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://zrk.yj20258.top

[S34] C++：遍历 vector
来源：http://mcz.9152youxi.cn

for (auto &x : v) { std::cout << x; }
来源：http://cbr.cashguo.top

[S35] C++：map
来源：http://txw.bjfxy.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://zjy.shzxlz.cn

[S36] C++：unordered_map
来源：http://jkm.dashuyun.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://kay.haohaochexian.top

[S37] C++：set
来源：http://oqg.zdbjq.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://xfp.ydjk.org.cn

[S38] C++：排序
来源：http://jpd.yangfankeji.com

std::sort(v.begin(), v.end());
来源：http://bvs.jiagoushi.top

[S39] C++：自定义比较器排序
来源：http://rew.cucudq.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://fph.hesvh.cn

[S40] C++：查找元素
来源：http://rxw.jyoumei.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://nra.yuxming.cn

[S41] C++：类与构造函数
来源：http://pky.kuanghao11.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://gkh.gzhubu.top

[S42] C++：继承与虚函数
来源：http://dju.zhoulong.xyz

class B : public Base { public: void f() override {} };
来源：http://ufo.redwolf501.top

[S43] C++：智能指针
来源：http://mgj.snrcjt.cn

auto p = std::make_unique<int>(5);
来源：http://wvx.haohaochexian.top

[S44] C++：引用传参
来源：http://tkq.bbcook.cn

void inc(int &x) { ++x; }
来源：http://ynx.sufxvd.cn

[S45] C++：lambda
来源：http://vxs.birdmap.top

auto add = [](int a, int b) { return a + b; };
来源：http://jdt.zhengqikj.top

[S46] C++：函数模板
来源：http://cyq.shzxlz.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://ugr.kuanghao11.cn

[S47] C++：结构化绑定遍历
来源：http://iae.xingfuxueyuan.xyz

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://mft.yanxiufei.cn

[S48] C++：逐行读文件
来源：http://mkh.cashguo.top

std::ifstream in("a.txt");  std::string line;
来源：http://ilt.zdbjq.cn

while (std::getline(in, line)) { }
来源：http://zvg.bbcook.cn

[S49] C++：写文件
来源：http://rst.ppjwa.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://duw.jqgufenzy.top

[S50] C++：格式化数字
来源：http://jlb.hammf.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hry.gogol.net.cn

[S51] C++：显式类型转换
来源：http://biq.gzhubu.top

static_cast<double>(a) / b
来源：http://vdj.shanyushiyangkeji.top

[S52] C++：const 与 noexcept
来源：http://bdp.zhiwuduotai.top

int size() const noexcept { return n_; }
来源：http://dbt.cheryme.top

[S53] C++：移动语义
来源：http://kvh.pycfn.com

std::vector<int> w = std::move(v);
来源：http://lhj.chenzaomai.com

[S54] C++：异常处理
来源：http://cep.xinyue.icu

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://rto.sysykeji.top

[S55] C++：结构化绑定
来源：http://ziv.vehdjk.com

auto [a, b] = std::make_pair(1, 2);
来源：http://juc.hnqzz.top

[S56] C++：optional
来源：http://tot.sxryk.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://lrg.zhijiandao.cn

[S57] C++：编译期常量
来源：http://oak.nwbrower.top

constexpr int N = 10;
来源：http://bof.zhongyouzk.top

[S58] C++：命名空间
来源：http://ngc.pengpengdd.cyou

namespace ns { int f() { return 1; } }
来源：http://nkf.yj20258.top

[S59] C++：静态断言
来源：http://oct.nanxinkj.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://sja.feifeiyinyue.top

[S60] C++：遍历并删除元素
来源：http://iaw.nanxuanxn.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://rzw.zhongyouzk.top

================================================================================
来源：http://irp.jianghu66.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://qui.kuanghao11.cn

================================================================================
来源：http://vkz.yongpay.top

[T01] Kotlin：Hello World
来源：http://mba.daria6918.cn

println("Hello")
来源：http://cpi.ywan-chungtsiang.top

[T02] Kotlin：变量
来源：http://flu.meibo888.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://fkk.nanxinkj.top

[T03] Kotlin：字符串模板
来源：http://pes.ctjpmb.com

"值: $b"
来源：http://uzl.cheryme.top

[T04] Kotlin：空安全
来源：http://vpi.zhoulong.xyz

val n: String? = null;  n?.length
来源：http://eje.aizwys.cn

[T05] Kotlin：when 表达式
来源：http://mub.shangyingyoupin.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://ibu.hnxiangtu.top

[T06] Kotlin：集合映射
来源：http://pkb.guannengcc.top

listOf(1, 2, 3).map { it * 2 }
来源：http://blw.zhiwuduotai.top

[T07] Kotlin：集合过滤
来源：http://ghg.vqdsnc.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://rfq.chenjidiqi.icu

[T08] Kotlin：数据类
来源：http://jkq.fanxiaobao.xyz

data class User(val name: String, val age: Int)
来源：http://pjo.ybcxt.top

[T09] Kotlin：扩展函数
来源：http://kzr.9152youxi.cn

fun String.exclaim() = this + "!"
来源：http://jqi.xuanzx.com

[T10] Kotlin：默认参数
来源：http://ool.zhixingplan.top

fun greet(name: String = "World") = "Hi $name"
来源：http://mbq.yonumen.top

[T11] Kotlin：协程
来源：http://ngt.jinqigfzy.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://ehu.ydzc1.top

[T12] Kotlin：解构声明
来源：http://xpv.shangyingyoupin.top

val (a, b) = Pair(1, 2)
来源：http://ici.zdqjudy.top

[T13] Kotlin：只读 Map
来源：http://nst.zhixingplan.top

val m = mapOf("a" to 1)
来源：http://pld.jlsjyb.cn

[T14] Kotlin：循环
来源：http://ojg.chenlongwang.top

for (i in 1..10) println(i)
来源：http://hjk.fengsongda.top

[T15] Kotlin：接口
来源：http://szk.hywenlv.cn

interface Shape { fun area(): Double }
来源：http://zgv.ybcxt.top

[T16] Swift：Hello World
来源：http://vvh.fktsv.cn

print("Hello")
来源：http://ddp.hcnkem.com

[T17] Swift：变量与常量
来源：http://tqa.sjlbkw.cn

var a = 1;  let b = 2
来源：http://pzz.hywenlv.cn

[T18] Swift：字符串插值
来源：http://vvc.ivvv.top

"值: \(b)"
来源：http://itq.xuetiantiany.cn

[T19] Swift：可选绑定
来源：http://tsu.andypj.xyz

if let n = opt { print(n) }
来源：http://xsw.ctjpmb.com

[T20] Swift：数组操作
来源：http://okr.gzhubu.top

var a = [1, 2, 3];  a.append(4)
来源：http://xzi.chenjidiqi.icu

[T21] Swift：遍历
来源：http://odm.nanxuanxn.top

for x in a { print(x) }
来源：http://kqo.pycfn.com

[T22] Swift：字典
来源：http://zfl.kuanghao11.cn

var d = ["a": 1];  d["b"] = 2
来源：http://bym.bjfxy.top

[T23] Swift：函数
来源：http://exq.zhiwuduotai.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://wtv.hywenlv.cn

[T24] Swift：闭包
来源：http://zir.cashguo.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://vxu.snrcjt.cn

[T25] Swift：结构体
来源：http://rbz.snrcjt.cn

struct P { var x: Int }
来源：http://slr.xuanzx.com

[T26] Swift：类与重写
来源：http://ilj.dashuyun.cn

class A: Base { override func f() {} }
来源：http://eyg.jqgfzy.top

[T27] Swift：错误处理
来源：http://vvg.sufxvd.cn

do { try f() } catch { print(error) }
来源：http://dwn.jinyuanbaomall.cn

[T28] Swift：枚举
来源：http://syg.bjfxy.top

enum Color { case red, green }
来源：http://vao.zhiwuduotai.top

[T29] Swift：guard 提前返回
来源：http://zrl.shanyushiyangkeji.top

guard let x = opt else { return }
来源：http://acc.sxryk.cn

[T30] Swift：协议
来源：http://chn.gotoacloud.top

protocol Shape { func area() -> Double }
来源：http://sxp.yj202588.top

[T31] Lua：Hello World
来源：http://vhm.jqgufenzy.top

print("Hello")
来源：http://ndu.haohaochexian.top

[T32] Lua：局部变量
来源：http://rec.yj20258888.top

local a = 1
来源：http://tfq.jianghu66.top

[T33] Lua：表（数组）
来源：http://dbs.vqdsnc.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://rmd.sxryk.cn

[T34] Lua：遍历表
来源：http://ykc.yangfankeji.com

for i, v in ipairs(t) do print(i, v) end
来源：http://qpr.epnwcf.com

[T35] Lua：字典表
来源：http://ivt.zhongyouzk.top

local d = { a = 1 };  d.b = 2
来源：http://gyu.shanyushiyangkeji.top

[T36] Lua：函数
来源：http://sbg.cdnleiting.top

function add(a, b) return a + b end
来源：http://onq.xingfuxueyuan.xyz

[T37] Lua：字符串拼接
来源：http://bun.gogol.net.cn

"a" .. "b"
来源：http://llj.yonumen.top

[T38] Lua：条件
来源：http://xie.xziqi.cn

if x > 0 then print("正") end
来源：http://aqy.jinghuilouyu.cn

[T39] Lua：模式匹配
来源：http://omj.hnqzz.top

string.find(s, "%d+")
来源：http://fvh.hcnkem.com

[T40] Lua：元表
来源：http://wxf.yangfankeji.com

setmetatable({}, { __index = base })
来源：http://lfd.sjlbkw.cn

[T41] Perl：Hello World
来源：http://bxo.pengpengdd.cyou

print "Hello\n";
来源：http://gyi.shzxlz.cn

[T42] Perl：变量类型
来源：http://klj.cashguo.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://mtz.havefunace.top

[T43] Perl：字符串插值
来源：http://bzw.52xcode.cn

"值: $a"
来源：http://fsn.jianghu66.top

[T44] Perl：条件
来源：http://dtc.ydjk.org.cn

if ($a > 0) { print "正"; }
来源：http://pvd.bbcook.cn

[T45] Perl：数组遍历
来源：http://ljl.xuetiantiany.cn

for my $x (@arr) { print $x; }
来源：http://ugr.ybcxt.top

[T46] Perl：哈希操作
来源：http://pzz.andypj.xyz

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://klx.zhaomingkeji.xyz

[T47] Perl：正则捕获
来源：http://iew.hongshengwenyu.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://fhe.kuanghao11.cn

[T48] Perl：正则替换
来源：http://kzx.fehbvm.com

$s =~ s/old/new/g;
来源：http://qke.sweek.top

[T49] Perl：函数
来源：http://avt.shanyushiyangkeji.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://fbu.nanxuanxn.top

[T50] Perl：逐行读文件
来源：http://hbj.xingfuxueyuan.xyz

open my $fh, "<", "a.txt" or die $!;
来源：http://lzt.jinqigufen.top

while (my $line = <$fh>) { print $line; }
来源：http://kpg.xinyue.icu

[T51] Scala：Hello World
来源：http://djn.zhijiandao.cn

println("Hello")
来源：http://ohy.cucudq.cn

[T52] Scala：变量
来源：http://vem.uphjek.com

val a = 1;  var b = 2
来源：http://sbl.nwbrower.top

[T53] Scala：字符串插值
来源：http://wld.nanxuanxn.top

s"值: $b"
来源：http://hqf.guowangkeji.top

[T54] Scala：集合映射
来源：http://xjs.daria6918.cn

List(1, 2, 3).map(_ * 2)
来源：http://yfb.tianlin.xyz

[T55] Scala：集合过滤
来源：http://nfd.yj202588.top

List(1, 2, 3).filter(_ > 1)
来源：http://cgf.hesvh.cn

[T56] Scala：样例类
来源：http://pfo.yangfankeji.com

case class User(name: String, age: Int)
来源：http://jdj.sxryk.cn

[T57] Scala：模式匹配
来源：http://tfx.zhiwuduotai.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://ewk.xuetiantiany.cn

[T58] Scala：函数定义
来源：http://dzw.fanxiaobao.xyz

def add(a: Int, b: Int): Int = a + b
来源：http://qvk.hywenlv.cn

[T59] Scala：循环
来源：http://iii.nanxuanxn.top

for (i <- 1 to 10) println(i)
来源：http://uyv.havefunace.top

[T60] Scala：折叠
来源：http://bjr.nanxinkj.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://cke.tianlin.xyz

================================================================================
来源：http://ufo.sjlbkw.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://fop.daxiang520.top

================================================================================
来源：http://pko.hammf.cn

[U01] Py：创建虚拟环境
来源：http://zby.aizwys.cn

python -m venv .venv && source .venv/bin/activate
来源：http://twx.fzhhl.top

[U02] Py：导出 / 安装依赖
来源：http://jvc.ydzc1.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://teu.ydjk.org.cn

[U03] Py：加载 .env 配置
来源：http://dad.dashuyun.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://meh.jlsjyb.cn

[U04] Py：变量调试打印
来源：http://ctw.vehdjk.com

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://wbj.jyoumei.cn

[U05] Py：列表去重且保序
来源：http://dkx.xingfuxueyuan.xyz

list(dict.fromkeys(arr))
来源：http://idq.zdqjudy.top

[U06] Py：合并两个字典
来源：http://pmg.vqdsnc.cn

{**a, **b}
来源：http://ksl.xylfe.cn

[U07] Py：反转字典键值
来源：http://cmj.jianghu66.top

{v: k for k, v in d.items()}
来源：http://gag.meibo888.top

[U08] Py：展平二维列表
来源：http://djn.cdnleiting.top

[y for x in nested for y in x]
来源：http://kfy.tianlin.xyz

[U09] Py：字典取最大值的键
来源：http://kce.hesvh.cn

max(d, key=d.get)
来源：http://yap.zhixingplan.top

[U10] Py：按值排序字典
来源：http://xom.aizwys.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://pvk.yongpay.top

[U11] Py：生成器表达式
来源：http://vas.yfazqb.com

(x * 2 for x in arr)
来源：http://bae.nanxinkj.top

[U12] Py：取出现最多的 3 个元素
来源：http://tht.zhijiandao.cn

Counter(arr).most_common(3)
来源：http://zhm.gzhubu.top

[U13] Py：固定长度队列
来源：http://pic.sysykeji.top

deque(maxlen=10)
来源：http://pkm.zhongyouzk.top

[U14] Py：分组收集到列表
来源：http://hzr.jinqigfzy.top

defaultdict(list)
来源：http://uxg.hammf.cn

[U15] Py：高精度计时
来源：http://bnx.pengpengdd.cyou

t = time.perf_counter()
来源：http://hzv.daxiang520.top

[U16] Py：命令行参数解析
来源：http://cxn.nanxuanxn.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://mlm.wangdashe.top

[U17] Py：初始化日志
来源：http://qwq.cucudq.cn

logging.basicConfig(level=logging.INFO)
来源：http://rcc.guowangkeji.top

[U18] Py：预编译正则
来源：http://iwt.nanxuanxn.top

pat = re.compile(r"\d+")
来源：http://yaq.nanxinkj.top

[U19] Py：正则替换带回调
来源：http://jwm.gogol.net.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://uwa.nanxinkj.top

[U20] Py：缓存函数结果
来源：http://znk.jinyuanbaomall.cn

@functools.lru_cache(maxsize=None)
来源：http://kgo.sysykeji.top

[U21] Py：自定义上下文管理器
来源：http://qdu.guowangkeji.top

@contextlib.contextmanager
来源：http://qqc.hesvh.cn

[U22] Py：矩阵转置
来源：http://uhj.chenjidiqi.icu

list(zip(*m))
来源：http://bxk.yuxming.cn

[U23] Py：分块读取大文件
来源：http://wmc.hongshengwenyu.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://iwz.dashuyun.cn

[U24] Py：路径操作
来源：http://hxa.shzxlz.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://luf.c1oappe.top

[U25] Py：CSV 按字典读
来源：http://zhp.sufxvd.cn

csv.DictReader(f)
来源：http://fsx.jinqigfzy.top

[U26] Py：并发下载
来源：http://ibk.jinqigufen.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://ksk.xuanzx.com


<!-- 参考信息 -->