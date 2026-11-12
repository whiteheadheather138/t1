代发 wailian999

export PATH="$HOME/bin:$PATH"
来源：http://zzc.epnwcf.com

[R76] 使用临时文件
来源：http://xrl.zhixingplan.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://zav.ybcxt.top

[R77] 读取用户输入
来源：http://gnw.daxiang520.top

read -rp "请输入: " ans
来源：http://ohm.sufxvd.cn

[R78] 交互式菜单
来源：http://hqs.vqdsnc.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://hpn.pengpengdd.cyou

[R79] 解析命令行选项
来源：http://txv.hesvh.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://ynp.haohaochexian.top

[R80] 查看脚本执行耗时
来源：http://euz.haohaochexian.top

time ./run.sh
来源：http://dhv.svipenyu.cn

================================================================================
来源：http://izx.zhixingplan.top

S. C / C++ 专题
来源：http://ual.yj20258888.top

================================================================================
来源：http://tgu.hcnkem.com

[S01] C：Hello World
来源：http://okj.hammf.cn

#include <stdio.h>
来源：http://tso.pengpengdd.cyou

int main(void) { printf("Hello\n"); return 0; }
来源：http://zvl.wangdashe.top

[S02] C：变量与格式化输出
来源：http://qhf.aizwys.cn

int a = 10; printf("%d\n", a);
来源：http://lsr.xziqi.cn

[S03] C：读入整数
来源：http://xfz.zdqjudy.top

int x; scanf("%d", &x);
来源：http://wlu.nanxinkj.top

[S04] C：字符串复制
来源：http://wth.uphjek.com

char dst[32]; strcpy(dst, "hi");
来源：http://cop.wangdashe.top

[S05] C：字符串长度
来源：http://nob.andypj.xyz

strlen(s)
来源：http://kgx.nwbrower.top

[S06] C：字符串比较
来源：http://vrq.52xcode.cn

strcmp(a, b) == 0
来源：http://ohm.jlsjyb.cn

[S07] C：数组遍历求和
来源：http://szg.jqgfzy.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://bjq.fehbvm.com

[S08] C：动态内存分配与释放
来源：http://ukg.jinghuilouyu.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://eqh.jinqigufen.top

[S09] C：结构体定义与初始化
来源：http://qcg.hesvh.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://vbx.aibaodan.cn

[S10] C：指针与解引用
来源：http://ptf.zhijiandao.cn

int *p = &a;  *p = 5;
来源：http://ehf.ydjk.org.cn

[S11] C：逐行读文件
来源：http://ojd.gaohongyu789.top

FILE *f = fopen("a.txt", "r");
来源：http://pue.ydzc1.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://zch.9152youxi.cn

fclose(f);
来源：http://ylw.quarkkingdee.top

[S12] C：写文件
来源：http://abj.hnqzz.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://jkl.gogol.net.cn

[S13] C：宏定义
来源：http://zve.uphjek.com

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://bsu.zycfv.cn

[S14] C：枚举
来源：http://keb.jlsjyb.cn

enum Color { RED, GREEN, BLUE };
来源：http://qdk.feifeiyinyue.top

[S15] C：类型转换
来源：http://fgd.316326.xyz

(double) a / b
来源：http://nns.ywan-chungtsiang.top

[S16] C：位操作置位
来源：http://xvm.yongpay.top

x |= (1 << 3);
来源：http://qgp.hfpthk.cn

[S17] C：安全拼接字符串
来源：http://loc.shangyingyoupin.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://egr.fanxiaobao.xyz

[S18] C：命令行参数
来源：http://gsn.yangfankeji.com

int main(int argc, char **argv)
来源：http://aww.gogol.net.cn

[S19] C：快速排序
来源：http://ioz.xuetiantiany.cn

qsort(a, n, sizeof(int), cmp);
来源：http://jpa.tianlin.xyz

[S20] C：二分查找
来源：http://olq.shanyushiyangkeji.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://ody.yfazqb.com

[S21] C：字符类别判断
来源：http://wqv.xziqi.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://bpf.daxiang520.top

[S22] C：字符串转数字
来源：http://pnu.ehwqpu.com

atoi("42");  strtod("3.14", NULL);
来源：http://sed.haohaochexian.top

[S23] C：随机数
来源：http://rxy.hywenlv.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://xpt.jinqigfzy.top

[S24] C：获取本地时间
来源：http://lhi.hysaishi.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://ddx.gotoacloud.top

[S25] C：内存拷贝
来源：http://olb.316326.xyz

memcpy(dst, src, n);
来源：http://vlq.jqgufenzy.top

[S26] C：内存清零
来源：http://pqg.tian-w.cn

memset(a, 0, sizeof a);
来源：http://bft.xylfe.cn

[S27] C：定义常量
来源：http://czt.xuanzx.com

const double PI = 3.14159;
来源：http://hgm.cashguo.top

[S28] C：静态变量
来源：http://uhs.jyoumei.cn

static int counter = 0;
来源：http://kos.tian-w.cn

[S29] C：变参函数
来源：http://utr.52xcode.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://tpn.svipenyu.cn

[S30] C：头文件保护
来源：http://eaw.tarul.cn

#ifndef X_H
来源：http://bzp.ydjk.org.cn

#define X_H
来源：http://sws.fengsongda.top

#endif
来源：http://viy.tianlin.xyz

[S31] C++：Hello World
来源：http://pex.kuanghao11.cn

#include <iostream>
来源：http://csv.vqdsnc.cn

int main() { std::cout << "Hello\n"; }
来源：http://upt.guowangkeji.top

[S32] C++：字符串
来源：http://nfw.shzxlz.cn

std::string s = "hi";  s += "!";
来源：http://myr.guowangkeji.top

[S33] C++：vector 增删
来源：http://npb.52xcode.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://xcj.cashguo.top

[S34] C++：遍历 vector
来源：http://oos.jinghuilouyu.cn

for (auto &x : v) { std::cout << x; }
来源：http://gwq.yvedp.cn

[S35] C++：map
来源：http://aap.xingfuxueyuan.xyz

std::map<std::string, int> m;  m["a"] = 1;
来源：http://okj.zdbjq.cn

[S36] C++：unordered_map
来源：http://ofv.nwbrower.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://iqu.xinyue.icu

[S37] C++：set
来源：http://mjl.sjlbkw.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://eeb.hongshengwenyu.top

[S38] C++：排序
来源：http://qti.hongshengwenyu.top

std::sort(v.begin(), v.end());
来源：http://ryo.yongpay.top

[S39] C++：自定义比较器排序
来源：http://buk.jianghu66.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://ppp.shanyushiyangtech.top

[S40] C++：查找元素
来源：http://siz.redwolf501.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://pko.tianlin.xyz

[S41] C++：类与构造函数
来源：http://hvl.xylfe.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://ngd.tian-w.cn

[S42] C++：继承与虚函数
来源：http://tyf.bjfxy.top

class B : public Base { public: void f() override {} };
来源：http://kyp.cheryme.top

[S43] C++：智能指针
来源：http://eup.redwolf501.top

auto p = std::make_unique<int>(5);
来源：http://jjr.yanxiufei.cn

[S44] C++：引用传参
来源：http://iwy.guannengcc.top

void inc(int &x) { ++x; }
来源：http://krh.jqgfzy.top

[S45] C++：lambda
来源：http://vfa.havefunace.top

auto add = [](int a, int b) { return a + b; };
来源：http://vdn.fzhhl.top

[S46] C++：函数模板
来源：http://igq.fktsv.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://php.yfazqb.com

[S47] C++：结构化绑定遍历
来源：http://dlx.ydzc1.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://fbk.hcnkem.com

[S48] C++：逐行读文件
来源：http://itu.jlsjyb.cn

std::ifstream in("a.txt");  std::string line;
来源：http://crt.hesvh.cn

while (std::getline(in, line)) { }
来源：http://miw.ctjpmb.com

[S49] C++：写文件
来源：http://ovp.svipenyu.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://ymx.birdmap.top

[S50] C++：格式化数字
来源：http://tig.dashuyun.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://iml.hnqzz.top

[S51] C++：显式类型转换
来源：http://hxc.tanke756.top

static_cast<double>(a) / b
来源：http://snn.0kj1m.cn

[S52] C++：const 与 noexcept
来源：http://tru.shangyingyoupin.top

int size() const noexcept { return n_; }
来源：http://jmx.jqgufenzy.top

[S53] C++：移动语义
来源：http://rkc.cqqwz.cn

std::vector<int> w = std::move(v);
来源：http://lfs.kuanghao11.cn

[S54] C++：异常处理
来源：http://upf.shanyushiyangtech.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://xza.ywan-chungtsiang.top

[S55] C++：结构化绑定
来源：http://gnm.meibo888.top

auto [a, b] = std::make_pair(1, 2);
来源：http://rgr.uphjek.com

[S56] C++：optional
来源：http://ock.cheryme.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://uiw.yangfankeji.com

[S57] C++：编译期常量
来源：http://hna.cashguo.top

constexpr int N = 10;
来源：http://miu.sxryk.cn

[S58] C++：命名空间
来源：http://gzl.hammf.cn

namespace ns { int f() { return 1; } }
来源：http://qtw.fanxiaobao.xyz

[S59] C++：静态断言
来源：http://ysj.yfazqb.com

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://clz.pengpengdd.cyou

[S60] C++：遍历并删除元素
来源：http://kep.sweek.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://ixy.andypj.xyz

================================================================================
来源：http://sjn.9152youxi.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://yfw.zhoulong.xyz

================================================================================
来源：http://zim.vehdjk.com

[T01] Kotlin：Hello World
来源：http://jgf.birdmap.top

println("Hello")
来源：http://dci.zhijiandao.cn

[T02] Kotlin：变量
来源：http://zxt.tian-w.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://lfm.quarkkingdee.top

[T03] Kotlin：字符串模板
来源：http://ohw.hysaishi.cn

"值: $b"
来源：http://wsm.gogol.net.cn

[T04] Kotlin：空安全
来源：http://mrg.xylfe.cn

val n: String? = null;  n?.length
来源：http://tpg.svipenyu.cn

[T05] Kotlin：when 表达式
来源：http://nkt.hesvh.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://axu.chenlongwang.top

[T06] Kotlin：集合映射
来源：http://okw.chenjidiqi.icu

listOf(1, 2, 3).map { it * 2 }
来源：http://syt.ybcxt.top

[T07] Kotlin：集合过滤
来源：http://qfq.kuanghao11.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://fbj.tianlin.xyz

[T08] Kotlin：数据类
来源：http://wek.epnwcf.com

data class User(val name: String, val age: Int)
来源：http://wfv.daxiang520.top

[T09] Kotlin：扩展函数
来源：http://vmd.birdmap.top

fun String.exclaim() = this + "!"
来源：http://ion.daria6918.cn

[T10] Kotlin：默认参数
来源：http://rhe.gaohongyu789.top

fun greet(name: String = "World") = "Hi $name"
来源：http://ydt.sjlbkw.cn

[T11] Kotlin：协程
来源：http://fip.zhaomingkeji.xyz

GlobalScope.launch { delay(1000); println("done") }
来源：http://oti.fanxiaobao.xyz

[T12] Kotlin：解构声明
来源：http://qbc.pycfn.com

val (a, b) = Pair(1, 2)
来源：http://gpj.andypj.xyz

[T13] Kotlin：只读 Map
来源：http://njf.hywenlv.cn

val m = mapOf("a" to 1)
来源：http://jss.svipenyu.cn

[T14] Kotlin：循环
来源：http://gim.zhixingplan.top

for (i in 1..10) println(i)
来源：http://mch.dashuyun.cn

[T15] Kotlin：接口
来源：http://crd.ivvv.top

interface Shape { fun area(): Double }
来源：http://eig.jinqigufen.top

[T16] Swift：Hello World
来源：http://hnz.xingfuxueyuan.xyz

print("Hello")
来源：http://tns.fanxiaobao.xyz

[T17] Swift：变量与常量
来源：http://qae.dashuyun.cn

var a = 1;  let b = 2
来源：http://mkr.dashuyun.cn

[T18] Swift：字符串插值
来源：http://vzi.gogol.net.cn

"值: \(b)"
来源：http://qnt.hammf.cn

[T19] Swift：可选绑定
来源：http://ste.zdqjudy.top

if let n = opt { print(n) }
来源：http://wxj.nanxuanxn.top

[T20] Swift：数组操作
来源：http://ily.aizwys.cn

var a = [1, 2, 3];  a.append(4)
来源：http://mnk.guowangkeji.top

[T21] Swift：遍历
来源：http://qzm.daria6918.cn

for x in a { print(x) }
来源：http://oer.yuanzhike.top

[T22] Swift：字典
来源：http://iqq.yueranfly.top

var d = ["a": 1];  d["b"] = 2
来源：http://hzz.pycfn.com

[T23] Swift：函数
来源：http://fce.sweek.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://mcs.jianghu66.top

[T24] Swift：闭包
来源：http://wlj.sxryk.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://kst.cashguo.top

[T25] Swift：结构体
来源：http://epz.hysaishi.cn

struct P { var x: Int }
来源：http://iqs.yueranfly.top

[T26] Swift：类与重写
来源：http://zbo.zhongyouzk.top

class A: Base { override func f() {} }
来源：http://kul.shanyushiyangtech.top

[T27] Swift：错误处理
来源：http://dhi.fzhhl.top

do { try f() } catch { print(error) }
来源：http://tyt.yonumen.top

[T28] Swift：枚举
来源：http://aco.mhx1999.top

enum Color { case red, green }
来源：http://khp.pycfn.com

[T29] Swift：guard 提前返回
来源：http://amx.zdqjudy.top

guard let x = opt else { return }
来源：http://tkq.guannengcc.top

[T30] Swift：协议
来源：http://vuk.snrcjt.cn

protocol Shape { func area() -> Double }
来源：http://qkw.tianlin.xyz

[T31] Lua：Hello World
来源：http://qpz.svipenyu.cn

print("Hello")
来源：http://gdi.xylfe.cn

[T32] Lua：局部变量
来源：http://qrm.ywan-chungtsiang.top

local a = 1
来源：http://bcp.jlsjyb.cn

[T33] Lua：表（数组）
来源：http://uoo.hongshengwenyu.top

local t = {1, 2, 3};  t[4] = 4
来源：http://wvj.hysaishi.cn

[T34] Lua：遍历表
来源：http://vrb.wangdashe.top

for i, v in ipairs(t) do print(i, v) end
来源：http://ckw.fengsongda.top

[T35] Lua：字典表
来源：http://mgs.zhoulong.xyz

local d = { a = 1 };  d.b = 2
来源：http://cnk.yj202588.top

[T36] Lua：函数
来源：http://ahn.zhengqikj.top

function add(a, b) return a + b end
来源：http://lch.sjlbkw.cn

[T37] Lua：字符串拼接
来源：http://ibo.ivvv.top

"a" .. "b"
来源：http://wvl.fengsongda.top

[T38] Lua：条件
来源：http://aie.hongshengwenyu.top

if x > 0 then print("正") end
来源：http://mmn.jiagoushi.top

[T39] Lua：模式匹配
来源：http://kcu.feifeiyinyue.top

string.find(s, "%d+")
来源：http://exi.tian-w.cn

[T40] Lua：元表
来源：http://opv.dianchejie.cn

setmetatable({}, { __index = base })
来源：http://weu.yongpay.top

[T41] Perl：Hello World
来源：http://pxo.fktsv.cn

print "Hello\n";
来源：http://sdm.cheryme.top

[T42] Perl：变量类型
来源：http://fnx.fehbvm.com

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://dhr.fanxiaobao.xyz

[T43] Perl：字符串插值
来源：http://ukm.chenjidiqi.icu

"值: $a"
来源：http://nib.jianghu66.top

[T44] Perl：条件
来源：http://bbw.tian-w.cn

if ($a > 0) { print "正"; }
来源：http://qcz.hcnkem.com

[T45] Perl：数组遍历
来源：http://osp.yuanzhike.top

for my $x (@arr) { print $x; }
来源：http://mgi.yanxiufei.cn

[T46] Perl：哈希操作
来源：http://yji.shangyingyoupin.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://pgn.hammf.cn

[T47] Perl：正则捕获
来源：http://lpc.hnqzz.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://mun.ydjk.org.cn

[T48] Perl：正则替换
来源：http://inx.zhixingplan.top

$s =~ s/old/new/g;
来源：http://gze.hesvh.cn

[T49] Perl：函数
来源：http://lfb.haohaochexian.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://bxl.zdbjq.cn

[T50] Perl：逐行读文件
来源：http://gqf.nwbrower.top

open my $fh, "<", "a.txt" or die $!;
来源：http://yfx.316326.xyz

while (my $line = <$fh>) { print $line; }
来源：http://amp.nwbrower.top

[T51] Scala：Hello World
来源：http://pmj.ywan-chungtsiang.top

println("Hello")
来源：http://emy.nanxuanxn.top

[T52] Scala：变量
来源：http://euq.zhiwuduotai.top

val a = 1;  var b = 2
来源：http://mie.yueranfly.top

[T53] Scala：字符串插值
来源：http://oev.ybcxt.top

s"值: $b"
来源：http://apx.yvedp.cn

[T54] Scala：集合映射
来源：http://zon.birdmap.top

List(1, 2, 3).map(_ * 2)
来源：http://gvk.xingfuxueyuan.xyz

[T55] Scala：集合过滤
来源：http://gft.ybcxt.top

List(1, 2, 3).filter(_ > 1)
来源：http://lno.yangfankeji.com

[T56] Scala：样例类
来源：http://dbn.birdmap.top

case class User(name: String, age: Int)
来源：http://emt.sweek.top

[T57] Scala：模式匹配
来源：http://ahx.chenzaomai.com

x match { case 1 => "一"; case _ => "其他" }
来源：http://qrw.dashuyun.cn

[T58] Scala：函数定义
来源：http://wej.ctjpmb.com

def add(a: Int, b: Int): Int = a + b
来源：http://rnh.yongpay.top

[T59] Scala：循环
来源：http://xgs.bjfxy.top

for (i <- 1 to 10) println(i)
来源：http://ygc.jlsjyb.cn

[T60] Scala：折叠
来源：http://iru.redwolf501.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://ncq.ydzc1.top

================================================================================
来源：http://zyt.zhengqikj.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://cie.cashguo.top

================================================================================
来源：http://jcx.hongshengwenyu.top

[U01] Py：创建虚拟环境
来源：http://vfy.fehbvm.com

python -m venv .venv && source .venv/bin/activate
来源：http://zbr.guannengcc.top

[U02] Py：导出 / 安装依赖
来源：http://hrp.zhoulong.xyz

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://jsv.yj202588.top

[U03] Py：加载 .env 配置
来源：http://xro.0kj1m.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://xan.zhixingplan.top

[U04] Py：变量调试打印
来源：http://icq.yonumen.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://nze.yangfankeji.com

[U05] Py：列表去重且保序
来源：http://osq.shanyushiyangkeji.top

list(dict.fromkeys(arr))
来源：http://kum.cqqwz.cn

[U06] Py：合并两个字典
来源：http://waq.bjfxy.top

{**a, **b}
来源：http://rai.nwbrower.top

[U07] Py：反转字典键值
来源：http://kte.hfpthk.cn

{v: k for k, v in d.items()}
来源：http://zyl.ydzc1.top

[U08] Py：展平二维列表
来源：http://slj.xuanzx.com

[y for x in nested for y in x]
来源：http://sky.tanke756.top

[U09] Py：字典取最大值的键
来源：http://yww.jinqigufen.top

max(d, key=d.get)
来源：http://gov.sjlbkw.cn

[U10] Py：按值排序字典
来源：http://pmi.52xcode.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://jbo.jqgufenzy.top

[U11] Py：生成器表达式
来源：http://zsz.dashuyun.cn

(x * 2 for x in arr)
来源：http://jvo.cqqwz.cn

[U12] Py：取出现最多的 3 个元素
来源：http://fzx.yonumen.top

Counter(arr).most_common(3)
来源：http://ygs.zdqjudy.top

[U13] Py：固定长度队列
来源：http://oob.jinqigfzy.top

deque(maxlen=10)
来源：http://rvd.gotoacloud.top

[U14] Py：分组收集到列表
来源：http://cjd.pycfn.com

defaultdict(list)
来源：http://ssi.tianlin.xyz

[U15] Py：高精度计时
来源：http://dqp.hammf.cn

t = time.perf_counter()
来源：http://wpl.gaohongyu789.top

[U16] Py：命令行参数解析
来源：http://zqh.sweek.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://fbb.tarul.cn


<!-- 参考信息 -->