代发 wailian999

export PATH="$HOME/bin:$PATH"
来源：http://wsb.aizwys.cn

[R76] 使用临时文件
来源：http://ksz.hesvh.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://ajw.zdqjudy.top

[R77] 读取用户输入
来源：http://zrl.shzxlz.cn

read -rp "请输入: " ans
来源：http://xlj.hammf.cn

[R78] 交互式菜单
来源：http://hry.tianlin.xyz

select opt in a b c; do echo "$opt"; break; done
来源：http://fka.nanxuanxn.top

[R79] 解析命令行选项
来源：http://eye.hysaishi.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://czn.gzhubu.top

[R80] 查看脚本执行耗时
来源：http://nvf.zdqjudy.top

time ./run.sh
来源：http://tol.shzxlz.cn

================================================================================
来源：http://yaf.xingfuxueyuan.xyz

S. C / C++ 专题
来源：http://izm.bjfxy.top

================================================================================
来源：http://ney.hysaishi.cn

[S01] C：Hello World
来源：http://jjo.uphjek.com

#include <stdio.h>
来源：http://mjz.yj20258888.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://rci.redwolf501.top

[S02] C：变量与格式化输出
来源：http://nft.316326.xyz

int a = 10; printf("%d\n", a);
来源：http://xvf.xuetiantiany.cn

[S03] C：读入整数
来源：http://maf.hesvh.cn

int x; scanf("%d", &x);
来源：http://gmo.hongshengwenyu.top

[S04] C：字符串复制
来源：http://wtu.yuxming.cn

char dst[32]; strcpy(dst, "hi");
来源：http://mqt.tianlin.xyz

[S05] C：字符串长度
来源：http://udg.zhoulong.xyz

strlen(s)
来源：http://spz.aizwys.cn

[S06] C：字符串比较
来源：http://szr.fanxiaobao.xyz

strcmp(a, b) == 0
来源：http://tmr.fzhhl.top

[S07] C：数组遍历求和
来源：http://gvt.zdbjq.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://rkq.fzhhl.top

[S08] C：动态内存分配与释放
来源：http://gna.zhongyouzk.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://dpo.birdmap.top

[S09] C：结构体定义与初始化
来源：http://fbt.zhixingplan.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://umv.dashuyun.cn

[S10] C：指针与解引用
来源：http://sor.jqgufenzy.top

int *p = &a;  *p = 5;
来源：http://lct.jianghu66.top

[S11] C：逐行读文件
来源：http://dzs.gaohongyu789.top

FILE *f = fopen("a.txt", "r");
来源：http://ads.yueranfly.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://vrk.ywan-chungtsiang.top

fclose(f);
来源：http://bjq.hysaishi.cn

[S12] C：写文件
来源：http://opw.jyoumei.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://lew.chenlongwang.top

[S13] C：宏定义
来源：http://pyh.zhijiandao.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://sxp.ivvv.top

[S14] C：枚举
来源：http://ony.yanxiufei.cn

enum Color { RED, GREEN, BLUE };
来源：http://zvn.cheryme.top

[S15] C：类型转换
来源：http://ouz.jinghuilouyu.cn

(double) a / b
来源：http://bwl.dianchejie.cn

[S16] C：位操作置位
来源：http://ryg.c1oappe.top

x |= (1 << 3);
来源：http://rpx.shangyingyoupin.top

[S17] C：安全拼接字符串
来源：http://wva.uphjek.com

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://fvk.cashguo.top

[S18] C：命令行参数
来源：http://gfa.yfazqb.com

int main(int argc, char **argv)
来源：http://jhi.sweek.top

[S19] C：快速排序
来源：http://uyq.jiagoushi.top

qsort(a, n, sizeof(int), cmp);
来源：http://qkw.cucudq.cn

[S20] C：二分查找
来源：http://ytk.hesvh.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://zml.feifeiyinyue.top

[S21] C：字符类别判断
来源：http://qoq.zhoulong.xyz

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mvx.vqdsnc.cn

[S22] C：字符串转数字
来源：http://amp.bbcook.cn

atoi("42");  strtod("3.14", NULL);
来源：http://nyu.quarkkingdee.top

[S23] C：随机数
来源：http://ecr.dianchejie.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://lfc.ydjk.org.cn

[S24] C：获取本地时间
来源：http://jus.jinyuanbaomall.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://ucs.yuxming.cn

[S25] C：内存拷贝
来源：http://bgz.hysaishi.cn

memcpy(dst, src, n);
来源：http://qpl.pycfn.com

[S26] C：内存清零
来源：http://pbm.jqgfzy.top

memset(a, 0, sizeof a);
来源：http://iph.zhixingplan.top

[S27] C：定义常量
来源：http://ezm.nanxinkj.top

const double PI = 3.14159;
来源：http://ipv.ivvv.top

[S28] C：静态变量
来源：http://wzz.gotoacloud.top

static int counter = 0;
来源：http://twn.wangshuangyany.cn

[S29] C：变参函数
来源：http://otm.gzhubu.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://qit.gaohongyu789.top

[S30] C：头文件保护
来源：http://eiu.yvedp.cn

#ifndef X_H
来源：http://opj.hywenlv.cn

#define X_H
来源：http://oul.zdqjudy.top

#endif
来源：http://zwg.andypj.xyz

[S31] C++：Hello World
来源：http://lmn.aibaodan.cn

#include <iostream>
来源：http://ayf.tarul.cn

int main() { std::cout << "Hello\n"; }
来源：http://zzk.dianchejie.cn

[S32] C++：字符串
来源：http://wii.andypj.xyz

std::string s = "hi";  s += "!";
来源：http://znm.epnwcf.com

[S33] C++：vector 增删
来源：http://awk.hnqzz.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://rje.hnxiangtu.top

[S34] C++：遍历 vector
来源：http://zmr.hnxiangtu.top

for (auto &x : v) { std::cout << x; }
来源：http://mkv.epnwcf.com

[S35] C++：map
来源：http://avc.aizwys.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://oog.chenjidiqi.icu

[S36] C++：unordered_map
来源：http://wms.hcnkem.com

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://nal.ydzc1.top

[S37] C++：set
来源：http://ftc.kuanghao11.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://ots.tianlin.xyz

[S38] C++：排序
来源：http://lqv.sufxvd.cn

std::sort(v.begin(), v.end());
来源：http://odk.hnqzz.top

[S39] C++：自定义比较器排序
来源：http://bwi.yangfankeji.com

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://qln.aibaodan.cn

[S40] C++：查找元素
来源：http://uha.nanxuanxn.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://unz.bjfxy.top

[S41] C++：类与构造函数
来源：http://uwm.yueranfly.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://vvm.zhixingplan.top

[S42] C++：继承与虚函数
来源：http://clm.xziqi.cn

class B : public Base { public: void f() override {} };
来源：http://ajq.jinqigfzy.top

[S43] C++：智能指针
来源：http://zof.xinyue.icu

auto p = std::make_unique<int>(5);
来源：http://ycx.epnwcf.com

[S44] C++：引用传参
来源：http://ttl.pengpengdd.cyou

void inc(int &x) { ++x; }
来源：http://raj.0kj1m.cn

[S45] C++：lambda
来源：http://lhx.zhoulong.xyz

auto add = [](int a, int b) { return a + b; };
来源：http://uxm.xuanzx.com

[S46] C++：函数模板
来源：http://fpg.gaohongyu789.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://qux.cheryme.top

[S47] C++：结构化绑定遍历
来源：http://rbt.shangyingyoupin.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://mdj.aibaodan.cn

[S48] C++：逐行读文件
来源：http://vab.jinyuanbaomall.cn

std::ifstream in("a.txt");  std::string line;
来源：http://smz.hywenlv.cn

while (std::getline(in, line)) { }
来源：http://tcb.yvedp.cn

[S49] C++：写文件
来源：http://mzn.gzhubu.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://lla.tianlin.xyz

[S50] C++：格式化数字
来源：http://epb.zhaomingkeji.xyz

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://ehd.nwbrower.top

[S51] C++：显式类型转换
来源：http://rym.tianlin.xyz

static_cast<double>(a) / b
来源：http://yvd.yuxming.cn

[S52] C++：const 与 noexcept
来源：http://zqj.hcnkem.com

int size() const noexcept { return n_; }
来源：http://znz.havefunace.top

[S53] C++：移动语义
来源：http://gmw.ydzc1.top

std::vector<int> w = std::move(v);
来源：http://dyf.smart0.xyz

[S54] C++：异常处理
来源：http://rbl.0kj1m.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://tfk.zdbjq.cn

[S55] C++：结构化绑定
来源：http://pyp.vehdjk.com

auto [a, b] = std::make_pair(1, 2);
来源：http://svr.snrcjt.cn

[S56] C++：optional
来源：http://huy.jinyuanbaomall.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://jre.xingfuxueyuan.xyz

[S57] C++：编译期常量
来源：http://hyb.tian-w.cn

constexpr int N = 10;
来源：http://kvf.hywenlv.cn

[S58] C++：命名空间
来源：http://kst.xinyue.icu

namespace ns { int f() { return 1; } }
来源：http://zfa.hysaishi.cn

[S59] C++：静态断言
来源：http://bnm.zdbjq.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://ubn.316326.xyz

[S60] C++：遍历并删除元素
来源：http://vyu.jqgfzy.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://cbo.quarkkingdee.top

================================================================================
来源：http://dnw.epnwcf.com

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://tum.havefunace.top

================================================================================
来源：http://pmw.cucudq.cn

[T01] Kotlin：Hello World
来源：http://wcx.gaohongyu789.top

println("Hello")
来源：http://dyo.yfazqb.com

[T02] Kotlin：变量
来源：http://yov.jqgfzy.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://bhq.mhx1999.top

[T03] Kotlin：字符串模板
来源：http://wuf.pycfn.com

"值: $b"
来源：http://ebm.mhx1999.top

[T04] Kotlin：空安全
来源：http://uos.redwolf501.top

val n: String? = null;  n?.length
来源：http://tal.hfpthk.cn

[T05] Kotlin：when 表达式
来源：http://qpa.nanxuanxn.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://vhh.zhongyouzk.top

[T06] Kotlin：集合映射
来源：http://yls.gaohongyu789.top

listOf(1, 2, 3).map { it * 2 }
来源：http://kzc.xingfuxueyuan.xyz

[T07] Kotlin：集合过滤
来源：http://azj.yongpay.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://znm.hysaishi.cn

[T08] Kotlin：数据类
来源：http://yot.guannengcc.top

data class User(val name: String, val age: Int)
来源：http://mwp.fehbvm.com

[T09] Kotlin：扩展函数
来源：http://abt.guannengcc.top

fun String.exclaim() = this + "!"
来源：http://wzj.ywan-chungtsiang.top

[T10] Kotlin：默认参数
来源：http://qlp.iojbl.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://gaq.hfpthk.cn

[T11] Kotlin：协程
来源：http://cbi.dashuyun.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://kdq.zhaomingkeji.xyz

[T12] Kotlin：解构声明
来源：http://kmd.yj20258.top

val (a, b) = Pair(1, 2)
来源：http://vwu.guannengcc.top

[T13] Kotlin：只读 Map
来源：http://zwm.vqdsnc.cn

val m = mapOf("a" to 1)
来源：http://muo.guowangkeji.top

[T14] Kotlin：循环
来源：http://zvs.zhijiandao.cn

for (i in 1..10) println(i)
来源：http://pza.zhongyouzk.top

[T15] Kotlin：接口
来源：http://yqo.zdbjq.cn

interface Shape { fun area(): Double }
来源：http://sat.pycfn.com

[T16] Swift：Hello World
来源：http://gue.tianlin.xyz

print("Hello")
来源：http://bln.jqgufenzy.top

[T17] Swift：变量与常量
来源：http://ate.vqdsnc.cn

var a = 1;  let b = 2
来源：http://kwo.yj20258.top

[T18] Swift：字符串插值
来源：http://tcd.ehwqpu.com

"值: \(b)"
来源：http://cfw.birdmap.top

[T19] Swift：可选绑定
来源：http://mfn.c1oappe.top

if let n = opt { print(n) }
来源：http://pap.jyoumei.cn

[T20] Swift：数组操作
来源：http://gyq.xingfuxueyuan.xyz

var a = [1, 2, 3];  a.append(4)
来源：http://epp.sufxvd.cn

[T21] Swift：遍历
来源：http://qbx.ybcxt.top

for x in a { print(x) }
来源：http://vcq.mhx1999.top

[T22] Swift：字典
来源：http://xwg.ivvv.top

var d = ["a": 1];  d["b"] = 2
来源：http://eyc.0kj1m.cn

[T23] Swift：函数
来源：http://les.hammf.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://jik.svipenyu.cn

[T24] Swift：闭包
来源：http://eeq.jinyuanbaomall.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://rge.yueranfly.top

[T25] Swift：结构体
来源：http://pid.ehwqpu.com

struct P { var x: Int }
来源：http://rfm.hcnkem.com

[T26] Swift：类与重写
来源：http://cae.andypj.xyz

class A: Base { override func f() {} }
来源：http://rdg.shangyingyoupin.top

[T27] Swift：错误处理
来源：http://sib.cdnleiting.top

do { try f() } catch { print(error) }
来源：http://gpj.xuetiantiany.cn

[T28] Swift：枚举
来源：http://gec.tanke756.top

enum Color { case red, green }
来源：http://lop.chenjidiqi.icu

[T29] Swift：guard 提前返回
来源：http://ake.wangshuangyany.cn

guard let x = opt else { return }
来源：http://dno.birdmap.top

[T30] Swift：协议
来源：http://lpn.nanxinkj.top

protocol Shape { func area() -> Double }
来源：http://xsn.xuetiantiany.cn

[T31] Lua：Hello World
来源：http://wzf.yueranfly.top

print("Hello")
来源：http://ttz.cheryme.top

[T32] Lua：局部变量
来源：http://vbm.sweek.top

local a = 1
来源：http://ejc.pengpengdd.cyou

[T33] Lua：表（数组）
来源：http://zcl.hcnkem.com

local t = {1, 2, 3};  t[4] = 4
来源：http://kuj.hcnkem.com

[T34] Lua：遍历表
来源：http://vhf.ctjpmb.com

for i, v in ipairs(t) do print(i, v) end
来源：http://zpv.daxiang520.top

[T35] Lua：字典表
来源：http://agt.jinqigufen.top

local d = { a = 1 };  d.b = 2
来源：http://zfb.shuidangran.top

[T36] Lua：函数
来源：http://spx.dianchejie.cn

function add(a, b) return a + b end
来源：http://utw.tarul.cn

[T37] Lua：字符串拼接
来源：http://zbf.hywenlv.cn

"a" .. "b"
来源：http://ivb.yuanzhike.top

[T38] Lua：条件
来源：http://wmz.haohaochexian.top

if x > 0 then print("正") end
来源：http://dwj.yangfankeji.com

[T39] Lua：模式匹配
来源：http://kst.shuidangran.top

string.find(s, "%d+")
来源：http://tqj.zhaomingkeji.xyz

[T40] Lua：元表
来源：http://npi.smart0.xyz

setmetatable({}, { __index = base })
来源：http://mmb.dashuyun.cn

[T41] Perl：Hello World
来源：http://gmr.smart0.xyz

print "Hello\n";
来源：http://mck.c1oappe.top

[T42] Perl：变量类型
来源：http://uqb.iojbl.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://gxt.yj202588.top

[T43] Perl：字符串插值
来源：http://vcf.sysykeji.top

"值: $a"
来源：http://tjp.hongshengwenyu.top

[T44] Perl：条件
来源：http://oyt.xziqi.cn

if ($a > 0) { print "正"; }
来源：http://dsu.shuidangran.top

[T45] Perl：数组遍历
来源：http://wkh.aibaodan.cn

for my $x (@arr) { print $x; }
来源：http://zxf.fktsv.cn

[T46] Perl：哈希操作
来源：http://yoa.xylfe.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://nog.zhoulong.xyz

[T47] Perl：正则捕获
来源：http://ctt.aibaodan.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://lue.jinqigfzy.top

[T48] Perl：正则替换
来源：http://nvi.hnxiangtu.top

$s =~ s/old/new/g;
来源：http://mfy.pengpengdd.cyou

[T49] Perl：函数
来源：http://lzi.jinqigufen.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://ujw.sufxvd.cn

[T50] Perl：逐行读文件
来源：http://gge.xuetiantiany.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://wom.xuanzx.com

while (my $line = <$fh>) { print $line; }
来源：http://qxw.hammf.cn

[T51] Scala：Hello World
来源：http://bhw.aibaodan.cn

println("Hello")
来源：http://yck.snrcjt.cn

[T52] Scala：变量
来源：http://ubo.zdbjq.cn

val a = 1;  var b = 2
来源：http://ipm.yanxiufei.cn

[T53] Scala：字符串插值
来源：http://pic.cashguo.top

s"值: $b"
来源：http://lsf.nwbrower.top

[T54] Scala：集合映射
来源：http://uew.hysaishi.cn

List(1, 2, 3).map(_ * 2)
来源：http://csg.pengpengdd.cyou

[T55] Scala：集合过滤
来源：http://xcv.yvedp.cn

List(1, 2, 3).filter(_ > 1)
来源：http://zxs.snrcjt.cn

[T56] Scala：样例类
来源：http://mmj.guowangkeji.top

case class User(name: String, age: Int)
来源：http://ehe.shzxlz.cn

[T57] Scala：模式匹配
来源：http://lkm.epnwcf.com

x match { case 1 => "一"; case _ => "其他" }
来源：http://mpo.fzhhl.top

[T58] Scala：函数定义
来源：http://ogf.tian-w.cn

def add(a: Int, b: Int): Int = a + b
来源：http://wcu.tianlin.xyz

[T59] Scala：循环
来源：http://pxa.tanke756.top

for (i <- 1 to 10) println(i)
来源：http://thh.fehbvm.com

[T60] Scala：折叠
来源：http://kkg.wangdashe.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://kgr.zhijiandao.cn

================================================================================
来源：http://pjp.yj20258.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://ony.zhiwuduotai.top

================================================================================
来源：http://vrj.quarkkingdee.top

[U01] Py：创建虚拟环境
来源：http://uvk.jianghu66.top

python -m venv .venv && source .venv/bin/activate
来源：http://veh.chenzaomai.com

[U02] Py：导出 / 安装依赖
来源：http://jnh.zycfv.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hyo.bbcook.cn

[U03] Py：加载 .env 配置
来源：http://ycl.hesvh.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://jtc.zhijiandao.cn

[U04] Py：变量调试打印
来源：http://zgr.0kj1m.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://gcq.yonumen.top

[U05] Py：列表去重且保序
来源：http://dlo.yj20258888.top

list(dict.fromkeys(arr))
来源：http://zvz.fanxiaobao.xyz

[U06] Py：合并两个字典
来源：http://lrl.fengsongda.top

{**a, **b}
来源：http://uxp.shangyingyoupin.top

[U07] Py：反转字典键值
来源：http://hvu.fanxiaobao.xyz

{v: k for k, v in d.items()}
来源：http://egw.mhx1999.top

[U08] Py：展平二维列表
来源：http://xoy.pengpengdd.cyou

[y for x in nested for y in x]
来源：http://eao.zdbjq.cn

[U09] Py：字典取最大值的键
来源：http://wqb.jqgfzy.top

max(d, key=d.get)
来源：http://eeg.jinghuilouyu.cn

[U10] Py：按值排序字典
来源：http://xct.chenjidiqi.icu

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://yof.pycfn.com

[U11] Py：生成器表达式
来源：http://jqe.nanxinkj.top

(x * 2 for x in arr)
来源：http://upy.jinghuilouyu.cn

[U12] Py：取出现最多的 3 个元素
来源：http://xog.tanke756.top

Counter(arr).most_common(3)
来源：http://gcu.guannengcc.top

[U13] Py：固定长度队列
来源：http://zuv.zhaomingkeji.xyz

deque(maxlen=10)
来源：http://epc.yanxiufei.cn

[U14] Py：分组收集到列表
来源：http://vdu.bjfxy.top

defaultdict(list)
来源：http://ney.chenlongwang.top

[U15] Py：高精度计时
来源：http://btl.hcnkem.com

t = time.perf_counter()
来源：http://krn.hammf.cn

[U16] Py：命令行参数解析
来源：http://iii.jyoumei.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://mop.chenjidiqi.icu


<!-- 参考信息 -->