代发 wailian999

export PATH="$HOME/bin:$PATH"
来源：http://ced.daria6918.cn

[R76] 使用临时文件
来源：http://igo.birdmap.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://wcr.yuanzhike.top

[R77] 读取用户输入
来源：http://moi.zhixingplan.top

read -rp "请输入: " ans
来源：http://snm.zhixingplan.top

[R78] 交互式菜单
来源：http://scc.ydjk.org.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://yrw.dianchejie.cn

[R79] 解析命令行选项
来源：http://dbu.tarul.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://rro.yangfankeji.com

[R80] 查看脚本执行耗时
来源：http://qjr.epnwcf.com

time ./run.sh
来源：http://pte.guannengcc.top

================================================================================
来源：http://jfy.yuanzhike.top

S. C / C++ 专题
来源：http://kzz.ehwqpu.com

================================================================================
来源：http://ova.sufxvd.cn

[S01] C：Hello World
来源：http://hhs.hongshengwenyu.top

#include <stdio.h>
来源：http://kjd.quarkkingdee.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://sts.zhengqikj.top

[S02] C：变量与格式化输出
来源：http://ggm.epnwcf.com

int a = 10; printf("%d\n", a);
来源：http://dvl.bjfxy.top

[S03] C：读入整数
来源：http://ino.cucudq.cn

int x; scanf("%d", &x);
来源：http://dzo.kuanghao11.cn

[S04] C：字符串复制
来源：http://ljh.snrcjt.cn

char dst[32]; strcpy(dst, "hi");
来源：http://saf.xinyue.icu

[S05] C：字符串长度
来源：http://riw.zhongyouzk.top

strlen(s)
来源：http://wcf.dianchejie.cn

[S06] C：字符串比较
来源：http://zdd.yanxiufei.cn

strcmp(a, b) == 0
来源：http://rag.vehdjk.com

[S07] C：数组遍历求和
来源：http://qgo.dashuyun.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://jex.tanke756.top

[S08] C：动态内存分配与释放
来源：http://cjw.jianghu66.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://iib.dianchejie.cn

[S09] C：结构体定义与初始化
来源：http://itr.andypj.xyz

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://gsi.zycfv.cn

[S10] C：指针与解引用
来源：http://pus.gzhubu.top

int *p = &a;  *p = 5;
来源：http://wkx.sysykeji.top

[S11] C：逐行读文件
来源：http://lcd.hongshengwenyu.top

FILE *f = fopen("a.txt", "r");
来源：http://dye.shzxlz.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://pct.gaohongyu789.top

fclose(f);
来源：http://ytd.316326.xyz

[S12] C：写文件
来源：http://zlf.jinyuanbaomall.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://qzl.xuetiantiany.cn

[S13] C：宏定义
来源：http://kfn.fanxiaobao.xyz

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://lba.jqgufenzy.top

[S14] C：枚举
来源：http://nmb.jinyuanbaomall.cn

enum Color { RED, GREEN, BLUE };
来源：http://sgx.mhx1999.top

[S15] C：类型转换
来源：http://oou.tianlin.xyz

(double) a / b
来源：http://fsv.hfpthk.cn

[S16] C：位操作置位
来源：http://lqq.cqqwz.cn

x |= (1 << 3);
来源：http://kzq.ivvv.top

[S17] C：安全拼接字符串
来源：http://uqi.xuetiantiany.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wbk.shuidangran.top

[S18] C：命令行参数
来源：http://bub.yj202588.top

int main(int argc, char **argv)
来源：http://git.jqgfzy.top

[S19] C：快速排序
来源：http://mlv.wangdashe.top

qsort(a, n, sizeof(int), cmp);
来源：http://ygh.yangfankeji.com

[S20] C：二分查找
来源：http://tkf.gotoacloud.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hde.zhongyouzk.top

[S21] C：字符类别判断
来源：http://wmj.meibo888.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hqn.aizwys.cn

[S22] C：字符串转数字
来源：http://tfs.fengsongda.top

atoi("42");  strtod("3.14", NULL);
来源：http://zqx.cqqwz.cn

[S23] C：随机数
来源：http://grz.meibo888.top

srand(time(NULL));  int r = rand() % 100;
来源：http://fvz.feifeiyinyue.top

[S24] C：获取本地时间
来源：http://efp.yangfankeji.com

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://glu.uphjek.com

[S25] C：内存拷贝
来源：http://mar.guowangkeji.top

memcpy(dst, src, n);
来源：http://atd.yongpay.top

[S26] C：内存清零
来源：http://wvh.pycfn.com

memset(a, 0, sizeof a);
来源：http://duj.vqdsnc.cn

[S27] C：定义常量
来源：http://yvv.fehbvm.com

const double PI = 3.14159;
来源：http://mwz.hongshengwenyu.top

[S28] C：静态变量
来源：http://pbe.ivvv.top

static int counter = 0;
来源：http://yeb.bbcook.cn

[S29] C：变参函数
来源：http://fsk.hongshengwenyu.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://aqb.havefunace.top

[S30] C：头文件保护
来源：http://gyl.zhijiandao.cn

#ifndef X_H
来源：http://feg.9152youxi.cn

#define X_H
来源：http://stz.zhongyouzk.top

#endif
来源：http://yja.52xcode.cn

[S31] C++：Hello World
来源：http://qfk.yvedp.cn

#include <iostream>
来源：http://dpq.xingfuxueyuan.xyz

int main() { std::cout << "Hello\n"; }
来源：http://sny.xuanzx.com

[S32] C++：字符串
来源：http://phx.xingfuxueyuan.xyz

std::string s = "hi";  s += "!";
来源：http://hde.fengsongda.top

[S33] C++：vector 增删
来源：http://kwe.zdbjq.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://bms.xingfuxueyuan.xyz

[S34] C++：遍历 vector
来源：http://ajt.birdmap.top

for (auto &x : v) { std::cout << x; }
来源：http://xvh.zhixingplan.top

[S35] C++：map
来源：http://zbo.ctjpmb.com

std::map<std::string, int> m;  m["a"] = 1;
来源：http://azd.hfpthk.cn

[S36] C++：unordered_map
来源：http://qbn.feifeiyinyue.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://jzr.daxiang520.top

[S37] C++：set
来源：http://ese.gogol.net.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://dux.ydzc1.top

[S38] C++：排序
来源：http://ojr.xingfuxueyuan.xyz

std::sort(v.begin(), v.end());
来源：http://fey.ywan-chungtsiang.top

[S39] C++：自定义比较器排序
来源：http://gui.xuetiantiany.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://owx.epnwcf.com

[S40] C++：查找元素
来源：http://gkm.cashguo.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://xty.xuetiantiany.cn

[S41] C++：类与构造函数
来源：http://pzq.hongshengwenyu.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://rdo.zdqjudy.top

[S42] C++：继承与虚函数
来源：http://tou.yuxming.cn

class B : public Base { public: void f() override {} };
来源：http://qyu.hnqzz.top

[S43] C++：智能指针
来源：http://unj.ivvv.top

auto p = std::make_unique<int>(5);
来源：http://duq.yonumen.top

[S44] C++：引用传参
来源：http://uzq.epnwcf.com

void inc(int &x) { ++x; }
来源：http://ksu.wangshuangyany.cn

[S45] C++：lambda
来源：http://gfu.zdqjudy.top

auto add = [](int a, int b) { return a + b; };
来源：http://bpn.iojbl.cn

[S46] C++：函数模板
来源：http://hba.fanxiaobao.xyz

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://zan.wangshuangyany.cn

[S47] C++：结构化绑定遍历
来源：http://ucq.jianghu66.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://zlz.fengsongda.top

[S48] C++：逐行读文件
来源：http://vwk.52xcode.cn

std::ifstream in("a.txt");  std::string line;
来源：http://tid.jyoumei.cn

while (std::getline(in, line)) { }
来源：http://bdu.yangfankeji.com

[S49] C++：写文件
来源：http://cuk.zdqjudy.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://yyn.jlsjyb.cn

[S50] C++：格式化数字
来源：http://aty.yangfankeji.com

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://crq.cucudq.cn

[S51] C++：显式类型转换
来源：http://pyw.cdnleiting.top

static_cast<double>(a) / b
来源：http://zcb.nwbrower.top

[S52] C++：const 与 noexcept
来源：http://ywj.redwolf501.top

int size() const noexcept { return n_; }
来源：http://zzd.jinghuilouyu.cn

[S53] C++：移动语义
来源：http://tlc.hammf.cn

std::vector<int> w = std::move(v);
来源：http://fmh.jlsjyb.cn

[S54] C++：异常处理
来源：http://pep.c1oappe.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://ryu.uphjek.com

[S55] C++：结构化绑定
来源：http://rff.havefunace.top

auto [a, b] = std::make_pair(1, 2);
来源：http://awr.zhaomingkeji.xyz

[S56] C++：optional
来源：http://ipc.cashguo.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://fqi.guannengcc.top

[S57] C++：编译期常量
来源：http://qij.cheryme.top

constexpr int N = 10;
来源：http://mss.pengpengdd.cyou

[S58] C++：命名空间
来源：http://vmj.cqqwz.cn

namespace ns { int f() { return 1; } }
来源：http://mev.cashguo.top

[S59] C++：静态断言
来源：http://qva.0kj1m.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://rei.pengpengdd.cyou

[S60] C++：遍历并删除元素
来源：http://ann.svipenyu.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://yyh.daxiang520.top

================================================================================
来源：http://wbl.jinyuanbaomall.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://aiz.jlsjyb.cn

================================================================================
来源：http://jst.hfpthk.cn

[T01] Kotlin：Hello World
来源：http://mvg.yj20258.top

println("Hello")
来源：http://xjb.snrcjt.cn

[T02] Kotlin：变量
来源：http://xkg.hesvh.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://vyv.fanxiaobao.xyz

[T03] Kotlin：字符串模板
来源：http://odx.wangshuangyany.cn

"值: $b"
来源：http://yvm.xylfe.cn

[T04] Kotlin：空安全
来源：http://iib.yongpay.top

val n: String? = null;  n?.length
来源：http://xsw.xylfe.cn

[T05] Kotlin：when 表达式
来源：http://wxx.zhiwuduotai.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://rsi.aizwys.cn

[T06] Kotlin：集合映射
来源：http://sgf.xziqi.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://zcf.kuanghao11.cn

[T07] Kotlin：集合过滤
来源：http://twg.zhongyouzk.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://zdi.bbcook.cn

[T08] Kotlin：数据类
来源：http://mqb.aizwys.cn

data class User(val name: String, val age: Int)
来源：http://ajc.chenzaomai.com

[T09] Kotlin：扩展函数
来源：http://unt.svipenyu.cn

fun String.exclaim() = this + "!"
来源：http://qqs.ctjpmb.com

[T10] Kotlin：默认参数
来源：http://ybi.hesvh.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://lcj.yfazqb.com

[T11] Kotlin：协程
来源：http://jdg.jinghuilouyu.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://yak.hesvh.cn

[T12] Kotlin：解构声明
来源：http://ogu.nanxinkj.top

val (a, b) = Pair(1, 2)
来源：http://uks.hcnkem.com

[T13] Kotlin：只读 Map
来源：http://grs.jlsjyb.cn

val m = mapOf("a" to 1)
来源：http://rhi.cucudq.cn

[T14] Kotlin：循环
来源：http://mvr.zdbjq.cn

for (i in 1..10) println(i)
来源：http://xpn.nwbrower.top

[T15] Kotlin：接口
来源：http://tvf.zhongyouzk.top

interface Shape { fun area(): Double }
来源：http://ohj.dianchejie.cn

[T16] Swift：Hello World
来源：http://tdb.zhengqikj.top

print("Hello")
来源：http://qjh.yvedp.cn

[T17] Swift：变量与常量
来源：http://tid.zhengqikj.top

var a = 1;  let b = 2
来源：http://hct.uphjek.com

[T18] Swift：字符串插值
来源：http://jwz.yfazqb.com

"值: \(b)"
来源：http://rrs.jyoumei.cn

[T19] Swift：可选绑定
来源：http://qdw.wangshuangyany.cn

if let n = opt { print(n) }
来源：http://vfg.hywenlv.cn

[T20] Swift：数组操作
来源：http://pbb.daxiang520.top

var a = [1, 2, 3];  a.append(4)
来源：http://zux.jinqigufen.top

[T21] Swift：遍历
来源：http://wsp.meibo888.top

for x in a { print(x) }
来源：http://ejn.havefunace.top

[T22] Swift：字典
来源：http://ilg.cashguo.top

var d = ["a": 1];  d["b"] = 2
来源：http://ypg.hongshengwenyu.top

[T23] Swift：函数
来源：http://qty.xuetiantiany.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://teg.zdbjq.cn

[T24] Swift：闭包
来源：http://yhc.ctjpmb.com

let f = { (x: Int) -> Int in x * 2 }
来源：http://kvv.sjlbkw.cn

[T25] Swift：结构体
来源：http://cwn.hysaishi.cn

struct P { var x: Int }
来源：http://yuu.tarul.cn

[T26] Swift：类与重写
来源：http://zwz.vqdsnc.cn

class A: Base { override func f() {} }
来源：http://ozs.shanyushiyangkeji.top

[T27] Swift：错误处理
来源：http://opt.hnxiangtu.top

do { try f() } catch { print(error) }
来源：http://hdv.jianghu66.top

[T28] Swift：枚举
来源：http://ayt.vehdjk.com

enum Color { case red, green }
来源：http://vvs.ydzc1.top

[T29] Swift：guard 提前返回
来源：http://cel.ybcxt.top

guard let x = opt else { return }
来源：http://ipi.aizwys.cn

[T30] Swift：协议
来源：http://ozq.hysaishi.cn

protocol Shape { func area() -> Double }
来源：http://ogu.shangyingyoupin.top

[T31] Lua：Hello World
来源：http://czt.ydzc1.top

print("Hello")
来源：http://mer.bbcook.cn

[T32] Lua：局部变量
来源：http://rfo.nwbrower.top

local a = 1
来源：http://dnu.snrcjt.cn

[T33] Lua：表（数组）
来源：http://kzy.fengsongda.top

local t = {1, 2, 3};  t[4] = 4
来源：http://nwd.kuanghao11.cn

[T34] Lua：遍历表
来源：http://wkv.meibo888.top

for i, v in ipairs(t) do print(i, v) end
来源：http://ryj.guannengcc.top

[T35] Lua：字典表
来源：http://igy.zhengqikj.top

local d = { a = 1 };  d.b = 2
来源：http://qra.fengsongda.top

[T36] Lua：函数
来源：http://puh.zhixingplan.top

function add(a, b) return a + b end
来源：http://kri.fehbvm.com

[T37] Lua：字符串拼接
来源：http://iwn.fktsv.cn

"a" .. "b"
来源：http://apv.zdbjq.cn

[T38] Lua：条件
来源：http://cmd.zdbjq.cn

if x > 0 then print("正") end
来源：http://yhx.ehwqpu.com

[T39] Lua：模式匹配
来源：http://ihk.yanxiufei.cn

string.find(s, "%d+")
来源：http://yjw.yonumen.top

[T40] Lua：元表
来源：http://hvp.ivvv.top

setmetatable({}, { __index = base })
来源：http://vmx.ybcxt.top

[T41] Perl：Hello World
来源：http://nvw.svipenyu.cn

print "Hello\n";
来源：http://ekv.vqdsnc.cn

[T42] Perl：变量类型
来源：http://cdc.fanxiaobao.xyz

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://smt.zdqjudy.top

[T43] Perl：字符串插值
来源：http://wie.ctjpmb.com

"值: $a"
来源：http://rwx.yueranfly.top

[T44] Perl：条件
来源：http://pou.xuanzx.com

if ($a > 0) { print "正"; }
来源：http://vgq.yanxiufei.cn

[T45] Perl：数组遍历
来源：http://fxe.jinghuilouyu.cn

for my $x (@arr) { print $x; }
来源：http://wga.jiagoushi.top

[T46] Perl：哈希操作
来源：http://qee.yongpay.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://zkd.dashuyun.cn

[T47] Perl：正则捕获
来源：http://wcq.bjfxy.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://unw.iojbl.cn

[T48] Perl：正则替换
来源：http://wpl.yuanzhike.top

$s =~ s/old/new/g;
来源：http://lue.ehwqpu.com

[T49] Perl：函数
来源：http://lid.xinyue.icu

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://jrc.feifeiyinyue.top

[T50] Perl：逐行读文件
来源：http://tfb.meibo888.top

open my $fh, "<", "a.txt" or die $!;
来源：http://qof.hongshengwenyu.top

while (my $line = <$fh>) { print $line; }
来源：http://lko.zhaomingkeji.xyz

[T51] Scala：Hello World
来源：http://uxm.gaohongyu789.top

println("Hello")
来源：http://dxf.sweek.top

[T52] Scala：变量
来源：http://wzl.xuanzx.com

val a = 1;  var b = 2
来源：http://lbt.vqdsnc.cn

[T53] Scala：字符串插值
来源：http://fyc.sweek.top

s"值: $b"
来源：http://elb.ctjpmb.com

[T54] Scala：集合映射
来源：http://tar.xziqi.cn

List(1, 2, 3).map(_ * 2)
来源：http://lht.meibo888.top

[T55] Scala：集合过滤
来源：http://jvd.zdqjudy.top

List(1, 2, 3).filter(_ > 1)
来源：http://bfe.jqgufenzy.top

[T56] Scala：样例类
来源：http://cne.chenzaomai.com

case class User(name: String, age: Int)
来源：http://onr.wangdashe.top

[T57] Scala：模式匹配
来源：http://pdi.gogol.net.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://yjd.xuanzx.com

[T58] Scala：函数定义
来源：http://xzw.cdnleiting.top

def add(a: Int, b: Int): Int = a + b
来源：http://oxi.hcnkem.com

[T59] Scala：循环
来源：http://ovt.fzhhl.top

for (i <- 1 to 10) println(i)
来源：http://fkm.ybcxt.top

[T60] Scala：折叠
来源：http://lse.gaohongyu789.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://zwc.sufxvd.cn

================================================================================
来源：http://mvk.gaohongyu789.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://miu.hongshengwenyu.top

================================================================================
来源：http://aai.xuetiantiany.cn

[U01] Py：创建虚拟环境
来源：http://jwo.yvedp.cn

python -m venv .venv && source .venv/bin/activate
来源：http://yod.ywan-chungtsiang.top

[U02] Py：导出 / 安装依赖
来源：http://mnk.ywan-chungtsiang.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://cmq.ppjwa.cn

[U03] Py：加载 .env 配置
来源：http://kum.fanxiaobao.xyz

from dotenv import load_dotenv; load_dotenv()
来源：http://jyk.jinqigfzy.top

[U04] Py：变量调试打印
来源：http://vuo.dashuyun.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hni.yueranfly.top

[U05] Py：列表去重且保序
来源：http://yiq.hysaishi.cn

list(dict.fromkeys(arr))
来源：http://dbo.andypj.xyz

[U06] Py：合并两个字典
来源：http://vjo.yueranfly.top

{**a, **b}
来源：http://ebx.zycfv.cn

[U07] Py：反转字典键值
来源：http://smx.jianghu66.top

{v: k for k, v in d.items()}
来源：http://iym.ctjpmb.com

[U08] Py：展平二维列表
来源：http://fzk.hfpthk.cn

[y for x in nested for y in x]
来源：http://ehn.jqgufenzy.top

[U09] Py：字典取最大值的键
来源：http://jhr.fengsongda.top

max(d, key=d.get)
来源：http://boy.xylfe.cn

[U10] Py：按值排序字典
来源：http://mdn.xingfuxueyuan.xyz

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://txx.0kj1m.cn

[U11] Py：生成器表达式
来源：http://fnr.haohaochexian.top

(x * 2 for x in arr)
来源：http://zdp.ybcxt.top

[U12] Py：取出现最多的 3 个元素
来源：http://pfm.daxiang520.top

Counter(arr).most_common(3)
来源：http://uta.nwbrower.top

[U13] Py：固定长度队列
来源：http://can.tian-w.cn

deque(maxlen=10)
来源：http://ogz.sweek.top

[U14] Py：分组收集到列表
来源：http://bru.snrcjt.cn

defaultdict(list)
来源：http://imx.fktsv.cn

[U15] Py：高精度计时
来源：http://zva.chenlongwang.top

t = time.perf_counter()
来源：http://zup.andypj.xyz

[U16] Py：命令行参数解析
来源：http://api.wangshuangyany.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://xdj.jqgufenzy.top


<!-- 参考信息 -->