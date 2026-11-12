代发 wailian999

split -l 1000 big.log part_
来源：http://cfx.birdmap.top

[R74] 批量重命名
来源：http://fci.quarkkingdee.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://snd.ybcxt.top

[R75] 导出环境变量
来源：http://uap.xylfe.cn

export PATH="$HOME/bin:$PATH"
来源：http://xof.zhixingplan.top

[R76] 使用临时文件
来源：http://exx.jinqigufen.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://rsj.feifeiyinyue.top

[R77] 读取用户输入
来源：http://prs.yj20258.top

read -rp "请输入: " ans
来源：http://uva.wangshuangyany.cn

[R78] 交互式菜单
来源：http://opc.jinqigfzy.top

select opt in a b c; do echo "$opt"; break; done
来源：http://tmt.jiagoushi.top

[R79] 解析命令行选项
来源：http://mye.zhengqikj.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://ofv.tianlin.xyz

[R80] 查看脚本执行耗时
来源：http://pnx.shuidangran.top

time ./run.sh
来源：http://bki.epnwcf.com

================================================================================
来源：http://pfp.jinqigfzy.top

S. C / C++ 专题
来源：http://gvn.hcnkem.com

================================================================================
来源：http://fzi.mhx1999.top

[S01] C：Hello World
来源：http://bbt.yuxming.cn

#include <stdio.h>
来源：http://pha.zhaomingkeji.xyz

int main(void) { printf("Hello\n"); return 0; }
来源：http://gtv.wangshuangyany.cn

[S02] C：变量与格式化输出
来源：http://zlj.hywenlv.cn

int a = 10; printf("%d\n", a);
来源：http://bew.dianchejie.cn

[S03] C：读入整数
来源：http://pma.andypj.xyz

int x; scanf("%d", &x);
来源：http://bwo.jinqigfzy.top

[S04] C：字符串复制
来源：http://xer.daria6918.cn

char dst[32]; strcpy(dst, "hi");
来源：http://ubs.havefunace.top

[S05] C：字符串长度
来源：http://fyr.cqqwz.cn

strlen(s)
来源：http://jdj.ctjpmb.com

[S06] C：字符串比较
来源：http://gnu.feifeiyinyue.top

strcmp(a, b) == 0
来源：http://lgr.nanxinkj.top

[S07] C：数组遍历求和
来源：http://itd.chenjidiqi.icu

for (int i = 0; i < n; i++) sum += a[i];
来源：http://kxe.meibo888.top

[S08] C：动态内存分配与释放
来源：http://tyv.yangfankeji.com

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://ted.redwolf501.top

[S09] C：结构体定义与初始化
来源：http://ddo.jlsjyb.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://cdd.shzxlz.cn

[S10] C：指针与解引用
来源：http://mit.yueranfly.top

int *p = &a;  *p = 5;
来源：http://mua.sxryk.cn

[S11] C：逐行读文件
来源：http://dmg.xuetiantiany.cn

FILE *f = fopen("a.txt", "r");
来源：http://lbx.yj20258888.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://wau.shanyushiyangkeji.top

fclose(f);
来源：http://boi.cdnleiting.top

[S12] C：写文件
来源：http://wmy.ydzc1.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://sru.redwolf501.top

[S13] C：宏定义
来源：http://ysf.hammf.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://qjx.nwbrower.top

[S14] C：枚举
来源：http://ltl.cheryme.top

enum Color { RED, GREEN, BLUE };
来源：http://gaa.wangdashe.top

[S15] C：类型转换
来源：http://gsj.wangdashe.top

(double) a / b
来源：http://edi.cashguo.top

[S16] C：位操作置位
来源：http://plx.chenlongwang.top

x |= (1 << 3);
来源：http://qqt.kuanghao11.cn

[S17] C：安全拼接字符串
来源：http://obk.nwbrower.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://kfd.tanke756.top

[S18] C：命令行参数
来源：http://xab.sjlbkw.cn

int main(int argc, char **argv)
来源：http://jym.nanxuanxn.top

[S19] C：快速排序
来源：http://yub.andypj.xyz

qsort(a, n, sizeof(int), cmp);
来源：http://guj.hysaishi.cn

[S20] C：二分查找
来源：http://ade.yvedp.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://erh.yvedp.cn

[S21] C：字符类别判断
来源：http://uet.zhixingplan.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://uol.jqgufenzy.top

[S22] C：字符串转数字
来源：http://joe.ctjpmb.com

atoi("42");  strtod("3.14", NULL);
来源：http://fds.yangfankeji.com

[S23] C：随机数
来源：http://fay.jinyuanbaomall.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://uwj.xziqi.cn

[S24] C：获取本地时间
来源：http://dob.hnxiangtu.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://zkn.fengsongda.top

[S25] C：内存拷贝
来源：http://sbc.hnxiangtu.top

memcpy(dst, src, n);
来源：http://vsy.sufxvd.cn

[S26] C：内存清零
来源：http://kwt.dianchejie.cn

memset(a, 0, sizeof a);
来源：http://usl.smart0.xyz

[S27] C：定义常量
来源：http://hwz.snrcjt.cn

const double PI = 3.14159;
来源：http://fax.bbcook.cn

[S28] C：静态变量
来源：http://fuq.yanxiufei.cn

static int counter = 0;
来源：http://bmp.bbcook.cn

[S29] C：变参函数
来源：http://upc.yonumen.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://ugp.nanxinkj.top

[S30] C：头文件保护
来源：http://kqi.meibo888.top

#ifndef X_H
来源：http://mzn.pycfn.com

#define X_H
来源：http://wgk.wangdashe.top

#endif
来源：http://dvi.snrcjt.cn

[S31] C++：Hello World
来源：http://fvo.ivvv.top

#include <iostream>
来源：http://vdf.hongshengwenyu.top

int main() { std::cout << "Hello\n"; }
来源：http://dsr.fengsongda.top

[S32] C++：字符串
来源：http://skn.wangdashe.top

std::string s = "hi";  s += "!";
来源：http://cqh.yj20258.top

[S33] C++：vector 增删
来源：http://hql.yj202588.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://mwe.xylfe.cn

[S34] C++：遍历 vector
来源：http://ost.ehwqpu.com

for (auto &x : v) { std::cout << x; }
来源：http://ofw.yfazqb.com

[S35] C++：map
来源：http://zmf.jinyuanbaomall.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://feu.dianchejie.cn

[S36] C++：unordered_map
来源：http://rwf.cheryme.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://qcm.bjfxy.top

[S37] C++：set
来源：http://coj.sufxvd.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://oju.jinyuanbaomall.cn

[S38] C++：排序
来源：http://nan.epnwcf.com

std::sort(v.begin(), v.end());
来源：http://uwe.meibo888.top

[S39] C++：自定义比较器排序
来源：http://hpg.sjlbkw.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://jza.ehwqpu.com

[S40] C++：查找元素
来源：http://jek.chenlongwang.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://tec.pycfn.com

[S41] C++：类与构造函数
来源：http://voo.hammf.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://ckn.jinqigfzy.top

[S42] C++：继承与虚函数
来源：http://shk.shanyushiyangtech.top

class B : public Base { public: void f() override {} };
来源：http://orf.gzhubu.top

[S43] C++：智能指针
来源：http://qed.andypj.xyz

auto p = std::make_unique<int>(5);
来源：http://bpi.yongpay.top

[S44] C++：引用传参
来源：http://cea.jinyuanbaomall.cn

void inc(int &x) { ++x; }
来源：http://ain.yonumen.top

[S45] C++：lambda
来源：http://bdb.jinyuanbaomall.cn

auto add = [](int a, int b) { return a + b; };
来源：http://pjk.shangyingyoupin.top

[S46] C++：函数模板
来源：http://ijn.wangshuangyany.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://rfl.bbcook.cn

[S47] C++：结构化绑定遍历
来源：http://bjs.shanyushiyangkeji.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://sgc.ppjwa.cn

[S48] C++：逐行读文件
来源：http://jsb.shanyushiyangtech.top

std::ifstream in("a.txt");  std::string line;
来源：http://yqw.shanyushiyangkeji.top

while (std::getline(in, line)) { }
来源：http://rva.yfazqb.com

[S49] C++：写文件
来源：http://epl.fktsv.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://tah.xingfuxueyuan.xyz

[S50] C++：格式化数字
来源：http://sgf.chenlongwang.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://gfv.fehbvm.com

[S51] C++：显式类型转换
来源：http://cob.nanxuanxn.top

static_cast<double>(a) / b
来源：http://mwc.yanxiufei.cn

[S52] C++：const 与 noexcept
来源：http://anx.zhiwuduotai.top

int size() const noexcept { return n_; }
来源：http://qqz.fktsv.cn

[S53] C++：移动语义
来源：http://bqd.yfazqb.com

std::vector<int> w = std::move(v);
来源：http://gfs.hywenlv.cn

[S54] C++：异常处理
来源：http://njy.shanyushiyangtech.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://ssw.hnxiangtu.top

[S55] C++：结构化绑定
来源：http://cce.0kj1m.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://qtn.yongpay.top

[S56] C++：optional
来源：http://zmh.gaohongyu789.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://fuc.tian-w.cn

[S57] C++：编译期常量
来源：http://lfr.kuanghao11.cn

constexpr int N = 10;
来源：http://ryx.9152youxi.cn

[S58] C++：命名空间
来源：http://yxo.aibaodan.cn

namespace ns { int f() { return 1; } }
来源：http://nty.pycfn.com

[S59] C++：静态断言
来源：http://amh.jqgufenzy.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://tnc.fzhhl.top

[S60] C++：遍历并删除元素
来源：http://ggu.zhongyouzk.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://nqc.redwolf501.top

================================================================================
来源：http://rcd.pycfn.com

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://twp.ywan-chungtsiang.top

================================================================================
来源：http://fkq.aizwys.cn

[T01] Kotlin：Hello World
来源：http://whq.hcnkem.com

println("Hello")
来源：http://gdl.yj20258888.top

[T02] Kotlin：变量
来源：http://xdw.sjlbkw.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://ylw.jiagoushi.top

[T03] Kotlin：字符串模板
来源：http://bee.c1oappe.top

"值: $b"
来源：http://jrp.sjlbkw.cn

[T04] Kotlin：空安全
来源：http://lco.c1oappe.top

val n: String? = null;  n?.length
来源：http://mjz.jianghu66.top

[T05] Kotlin：when 表达式
来源：http://vkl.smart0.xyz

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://ttb.nwbrower.top

[T06] Kotlin：集合映射
来源：http://zbb.9152youxi.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://ukn.xziqi.cn

[T07] Kotlin：集合过滤
来源：http://uwb.vehdjk.com

listOf(1, 2, 3).filter { it > 1 }
来源：http://jje.sxryk.cn

[T08] Kotlin：数据类
来源：http://nfc.guannengcc.top

data class User(val name: String, val age: Int)
来源：http://eqs.pengpengdd.cyou

[T09] Kotlin：扩展函数
来源：http://wks.uphjek.com

fun String.exclaim() = this + "!"
来源：http://phn.jlsjyb.cn

[T10] Kotlin：默认参数
来源：http://xvk.zhengqikj.top

fun greet(name: String = "World") = "Hi $name"
来源：http://cqp.cdnleiting.top

[T11] Kotlin：协程
来源：http://ofw.xuetiantiany.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://cvx.guannengcc.top

[T12] Kotlin：解构声明
来源：http://fru.cdnleiting.top

val (a, b) = Pair(1, 2)
来源：http://prk.iojbl.cn

[T13] Kotlin：只读 Map
来源：http://xlk.kuanghao11.cn

val m = mapOf("a" to 1)
来源：http://tfv.dashuyun.cn

[T14] Kotlin：循环
来源：http://vfg.zhoulong.xyz

for (i in 1..10) println(i)
来源：http://lwr.havefunace.top

[T15] Kotlin：接口
来源：http://rze.daria6918.cn

interface Shape { fun area(): Double }
来源：http://xqw.gaohongyu789.top

[T16] Swift：Hello World
来源：http://aud.c1oappe.top

print("Hello")
来源：http://tda.hysaishi.cn

[T17] Swift：变量与常量
来源：http://vos.jyoumei.cn

var a = 1;  let b = 2
来源：http://ezp.daxiang520.top

[T18] Swift：字符串插值
来源：http://spw.tianlin.xyz

"值: \(b)"
来源：http://adw.chenlongwang.top

[T19] Swift：可选绑定
来源：http://dwz.xuanzx.com

if let n = opt { print(n) }
来源：http://lir.fehbvm.com

[T20] Swift：数组操作
来源：http://url.hammf.cn

var a = [1, 2, 3];  a.append(4)
来源：http://aen.ydzc1.top

[T21] Swift：遍历
来源：http://yjn.fengsongda.top

for x in a { print(x) }
来源：http://dnc.hesvh.cn

[T22] Swift：字典
来源：http://lhf.havefunace.top

var d = ["a": 1];  d["b"] = 2
来源：http://psh.pycfn.com

[T23] Swift：函数
来源：http://afx.hammf.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://uvr.smart0.xyz

[T24] Swift：闭包
来源：http://fqj.chenzaomai.com

let f = { (x: Int) -> Int in x * 2 }
来源：http://uuz.fzhhl.top

[T25] Swift：结构体
来源：http://qbw.zhengqikj.top

struct P { var x: Int }
来源：http://wco.0kj1m.cn

[T26] Swift：类与重写
来源：http://xyl.fanxiaobao.xyz

class A: Base { override func f() {} }
来源：http://qfa.mhx1999.top

[T27] Swift：错误处理
来源：http://flq.vehdjk.com

do { try f() } catch { print(error) }
来源：http://yda.shangyingyoupin.top

[T28] Swift：枚举
来源：http://ipw.jinghuilouyu.cn

enum Color { case red, green }
来源：http://xnf.ydjk.org.cn

[T29] Swift：guard 提前返回
来源：http://oig.ydjk.org.cn

guard let x = opt else { return }
来源：http://esg.fktsv.cn

[T30] Swift：协议
来源：http://mxu.zdqjudy.top

protocol Shape { func area() -> Double }
来源：http://too.jyoumei.cn

[T31] Lua：Hello World
来源：http://btq.tian-w.cn

print("Hello")
来源：http://okn.9152youxi.cn

[T32] Lua：局部变量
来源：http://dzv.meibo888.top

local a = 1
来源：http://eij.ydjk.org.cn

[T33] Lua：表（数组）
来源：http://iqv.uphjek.com

local t = {1, 2, 3};  t[4] = 4
来源：http://wds.zhongyouzk.top

[T34] Lua：遍历表
来源：http://akr.shanyushiyangtech.top

for i, v in ipairs(t) do print(i, v) end
来源：http://gtg.jlsjyb.cn

[T35] Lua：字典表
来源：http://gsd.pycfn.com

local d = { a = 1 };  d.b = 2
来源：http://vvj.gotoacloud.top

[T36] Lua：函数
来源：http://bzl.xziqi.cn

function add(a, b) return a + b end
来源：http://uyv.jinyuanbaomall.cn

[T37] Lua：字符串拼接
来源：http://jov.xuanzx.com

"a" .. "b"
来源：http://afd.ctjpmb.com

[T38] Lua：条件
来源：http://ypk.sxryk.cn

if x > 0 then print("正") end
来源：http://xyc.jinghuilouyu.cn

[T39] Lua：模式匹配
来源：http://lbo.ehwqpu.com

string.find(s, "%d+")
来源：http://ceg.ctjpmb.com

[T40] Lua：元表
来源：http://vpj.gotoacloud.top

setmetatable({}, { __index = base })
来源：http://hkv.ehwqpu.com

[T41] Perl：Hello World
来源：http://nct.tarul.cn

print "Hello\n";
来源：http://gly.hnxiangtu.top

[T42] Perl：变量类型
来源：http://rql.redwolf501.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://uig.cucudq.cn

[T43] Perl：字符串插值
来源：http://mqq.epnwcf.com

"值: $a"
来源：http://dah.yvedp.cn

[T44] Perl：条件
来源：http://nlv.jiagoushi.top

if ($a > 0) { print "正"; }
来源：http://qgv.cucudq.cn

[T45] Perl：数组遍历
来源：http://lrt.andypj.xyz

for my $x (@arr) { print $x; }
来源：http://lgy.chenlongwang.top

[T46] Perl：哈希操作
来源：http://lvi.hnxiangtu.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://cxk.tanke756.top

[T47] Perl：正则捕获
来源：http://paq.daxiang520.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://vtg.shanyushiyangkeji.top

[T48] Perl：正则替换
来源：http://evs.yueranfly.top

$s =~ s/old/new/g;
来源：http://wma.xziqi.cn

[T49] Perl：函数
来源：http://ldx.gogol.net.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://lez.yangfankeji.com

[T50] Perl：逐行读文件
来源：http://dsl.jiagoushi.top

open my $fh, "<", "a.txt" or die $!;
来源：http://cmw.fengsongda.top

while (my $line = <$fh>) { print $line; }
来源：http://tmi.yuxming.cn

[T51] Scala：Hello World
来源：http://mef.yongpay.top

println("Hello")
来源：http://gpr.chenlongwang.top

[T52] Scala：变量
来源：http://pbv.gotoacloud.top

val a = 1;  var b = 2
来源：http://htk.jinyuanbaomall.cn

[T53] Scala：字符串插值
来源：http://feq.hammf.cn

s"值: $b"
来源：http://vug.vqdsnc.cn

[T54] Scala：集合映射
来源：http://pea.jinqigufen.top

List(1, 2, 3).map(_ * 2)
来源：http://ltu.hammf.cn

[T55] Scala：集合过滤
来源：http://krn.gzhubu.top

List(1, 2, 3).filter(_ > 1)
来源：http://gme.fanxiaobao.xyz

[T56] Scala：样例类
来源：http://pre.yvedp.cn

case class User(name: String, age: Int)
来源：http://yyu.svipenyu.cn

[T57] Scala：模式匹配
来源：http://nxq.gaohongyu789.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://xhu.wangshuangyany.cn

[T58] Scala：函数定义
来源：http://tjt.yueranfly.top

def add(a: Int, b: Int): Int = a + b
来源：http://erl.gzhubu.top

[T59] Scala：循环
来源：http://diw.jyoumei.cn

for (i <- 1 to 10) println(i)
来源：http://aub.pengpengdd.cyou

[T60] Scala：折叠
来源：http://kin.zhaomingkeji.xyz

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://boo.yvedp.cn

================================================================================
来源：http://wbx.nanxinkj.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://cmo.cashguo.top

================================================================================
来源：http://kam.shzxlz.cn

[U01] Py：创建虚拟环境
来源：http://nry.jinyuanbaomall.cn

python -m venv .venv && source .venv/bin/activate
来源：http://ttf.gogol.net.cn

[U02] Py：导出 / 安装依赖
来源：http://lod.nanxuanxn.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://jpi.jlsjyb.cn

[U03] Py：加载 .env 配置
来源：http://ksd.xylfe.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://scx.jqgfzy.top

[U04] Py：变量调试打印
来源：http://wyc.hysaishi.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://nru.andypj.xyz

[U05] Py：列表去重且保序
来源：http://rhh.fanxiaobao.xyz

list(dict.fromkeys(arr))
来源：http://izp.hnxiangtu.top

[U06] Py：合并两个字典
来源：http://bna.shanyushiyangtech.top

{**a, **b}
来源：http://kjk.cucudq.cn

[U07] Py：反转字典键值
来源：http://iaj.sxryk.cn

{v: k for k, v in d.items()}
来源：http://fbq.ybcxt.top

[U08] Py：展平二维列表
来源：http://xsl.guowangkeji.top

[y for x in nested for y in x]
来源：http://khp.fehbvm.com

[U09] Py：字典取最大值的键
来源：http://tse.gogol.net.cn

max(d, key=d.get)
来源：http://qnu.xuanzx.com

[U10] Py：按值排序字典
来源：http://oeh.vehdjk.com

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://bjz.fengsongda.top

[U11] Py：生成器表达式
来源：http://yfh.yj202588.top

(x * 2 for x in arr)
来源：http://ilr.shuidangran.top

[U12] Py：取出现最多的 3 个元素
来源：http://pte.sweek.top

Counter(arr).most_common(3)
来源：http://zvz.cdnleiting.top

[U13] Py：固定长度队列
来源：http://ivu.jqgfzy.top

deque(maxlen=10)
来源：http://uzo.jinqigfzy.top

[U14] Py：分组收集到列表
来源：http://swd.sweek.top

defaultdict(list)
来源：http://ihv.hesvh.cn


<!-- 参考信息 -->