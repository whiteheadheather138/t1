代发 wailian999

export PATH="$HOME/bin:$PATH"
来源：http://wbl.smart0.xyz

[R76] 使用临时文件
来源：http://qbc.shanyushiyangtech.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://coh.zhaomingkeji.xyz

[R77] 读取用户输入
来源：http://got.shzxlz.cn

read -rp "请输入: " ans
来源：http://fqa.ybcxt.top

[R78] 交互式菜单
来源：http://pxf.hfpthk.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://bjk.andypj.xyz

[R79] 解析命令行选项
来源：http://wzj.birdmap.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://yai.xylfe.cn

[R80] 查看脚本执行耗时
来源：http://ayg.gzhubu.top

time ./run.sh
来源：http://ydd.uphjek.com

================================================================================
来源：http://seq.zhengqikj.top

S. C / C++ 专题
来源：http://peu.c1oappe.top

================================================================================
来源：http://gfh.jqgfzy.top

[S01] C：Hello World
来源：http://tea.gogol.net.cn

#include <stdio.h>
来源：http://rvq.sufxvd.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://lug.sweek.top

[S02] C：变量与格式化输出
来源：http://qlz.zhongyouzk.top

int a = 10; printf("%d\n", a);
来源：http://duc.c1oappe.top

[S03] C：读入整数
来源：http://cqf.zhengqikj.top

int x; scanf("%d", &x);
来源：http://lvf.zhaomingkeji.xyz

[S04] C：字符串复制
来源：http://kte.wangdashe.top

char dst[32]; strcpy(dst, "hi");
来源：http://ary.daxiang520.top

[S05] C：字符串长度
来源：http://tic.jinghuilouyu.cn

strlen(s)
来源：http://jqr.yonumen.top

[S06] C：字符串比较
来源：http://bej.pengpengdd.cyou

strcmp(a, b) == 0
来源：http://ybw.kuanghao11.cn

[S07] C：数组遍历求和
来源：http://nsv.jinqigfzy.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://lzb.zhengqikj.top

[S08] C：动态内存分配与释放
来源：http://ixp.mhx1999.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://pdo.sufxvd.cn

[S09] C：结构体定义与初始化
来源：http://qdw.jinyuanbaomall.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://uuo.ywan-chungtsiang.top

[S10] C：指针与解引用
来源：http://iui.guowangkeji.top

int *p = &a;  *p = 5;
来源：http://ssk.jqgfzy.top

[S11] C：逐行读文件
来源：http://hkd.vehdjk.com

FILE *f = fopen("a.txt", "r");
来源：http://cid.cdnleiting.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://jsy.bjfxy.top

fclose(f);
来源：http://jkg.cashguo.top

[S12] C：写文件
来源：http://hda.jqgufenzy.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://psw.redwolf501.top

[S13] C：宏定义
来源：http://fes.fktsv.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://qdx.wangdashe.top

[S14] C：枚举
来源：http://zxh.jianghu66.top

enum Color { RED, GREEN, BLUE };
来源：http://row.nanxinkj.top

[S15] C：类型转换
来源：http://aoa.zhaomingkeji.xyz

(double) a / b
来源：http://ujr.shanyushiyangkeji.top

[S16] C：位操作置位
来源：http://usb.uphjek.com

x |= (1 << 3);
来源：http://ili.snrcjt.cn

[S17] C：安全拼接字符串
来源：http://hxs.uphjek.com

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://swq.aizwys.cn

[S18] C：命令行参数
来源：http://gxj.cucudq.cn

int main(int argc, char **argv)
来源：http://orw.mhx1999.top

[S19] C：快速排序
来源：http://frz.kuanghao11.cn

qsort(a, n, sizeof(int), cmp);
来源：http://fyo.jqgfzy.top

[S20] C：二分查找
来源：http://gzh.fanxiaobao.xyz

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://nlv.fengsongda.top

[S21] C：字符类别判断
来源：http://uzf.zhoulong.xyz

isdigit(c);  isalpha(c);  isspace(c);
来源：http://pkq.chenjidiqi.icu

[S22] C：字符串转数字
来源：http://jvo.redwolf501.top

atoi("42");  strtod("3.14", NULL);
来源：http://vsq.snrcjt.cn

[S23] C：随机数
来源：http://awt.wangshuangyany.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://fzo.fehbvm.com

[S24] C：获取本地时间
来源：http://nue.kuanghao11.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://qsr.yj202588.top

[S25] C：内存拷贝
来源：http://ctq.ybcxt.top

memcpy(dst, src, n);
来源：http://pch.aizwys.cn

[S26] C：内存清零
来源：http://clh.52xcode.cn

memset(a, 0, sizeof a);
来源：http://njd.hongshengwenyu.top

[S27] C：定义常量
来源：http://pzz.cdnleiting.top

const double PI = 3.14159;
来源：http://bbe.shuidangran.top

[S28] C：静态变量
来源：http://gop.gaohongyu789.top

static int counter = 0;
来源：http://aar.jinqigfzy.top

[S29] C：变参函数
来源：http://ldf.daxiang520.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://udl.yuanzhike.top

[S30] C：头文件保护
来源：http://ytz.sweek.top

#ifndef X_H
来源：http://fio.zhixingplan.top

#define X_H
来源：http://ldx.bbcook.cn

#endif
来源：http://chr.316326.xyz

[S31] C++：Hello World
来源：http://byo.chenlongwang.top

#include <iostream>
来源：http://lai.hnxiangtu.top

int main() { std::cout << "Hello\n"; }
来源：http://kat.xinyue.icu

[S32] C++：字符串
来源：http://pyv.svipenyu.cn

std::string s = "hi";  s += "!";
来源：http://ykh.yj20258888.top

[S33] C++：vector 增删
来源：http://ibj.haohaochexian.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://mnl.yanxiufei.cn

[S34] C++：遍历 vector
来源：http://crv.cheryme.top

for (auto &x : v) { std::cout << x; }
来源：http://kmp.yonumen.top

[S35] C++：map
来源：http://wln.bjfxy.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://nde.fanxiaobao.xyz

[S36] C++：unordered_map
来源：http://pvg.kuanghao11.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://bxs.zhijiandao.cn

[S37] C++：set
来源：http://smm.zhongyouzk.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://aev.yonumen.top

[S38] C++：排序
来源：http://rzt.yanxiufei.cn

std::sort(v.begin(), v.end());
来源：http://txn.cheryme.top

[S39] C++：自定义比较器排序
来源：http://hto.ppjwa.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://cyf.dashuyun.cn

[S40] C++：查找元素
来源：http://dce.aibaodan.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://fpo.316326.xyz

[S41] C++：类与构造函数
来源：http://hsk.ydzc1.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://fcw.pengpengdd.cyou

[S42] C++：继承与虚函数
来源：http://bna.yongpay.top

class B : public Base { public: void f() override {} };
来源：http://rio.cheryme.top

[S43] C++：智能指针
来源：http://tfh.feifeiyinyue.top

auto p = std::make_unique<int>(5);
来源：http://ffl.ydzc1.top

[S44] C++：引用传参
来源：http://ybc.hnxiangtu.top

void inc(int &x) { ++x; }
来源：http://nbi.wangdashe.top

[S45] C++：lambda
来源：http://ovz.hongshengwenyu.top

auto add = [](int a, int b) { return a + b; };
来源：http://bhu.zhijiandao.cn

[S46] C++：函数模板
来源：http://hhh.jinyuanbaomall.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://kor.guannengcc.top

[S47] C++：结构化绑定遍历
来源：http://tnl.xuetiantiany.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://ana.wangdashe.top

[S48] C++：逐行读文件
来源：http://ovs.snrcjt.cn

std::ifstream in("a.txt");  std::string line;
来源：http://uff.yuxming.cn

while (std::getline(in, line)) { }
来源：http://vft.9152youxi.cn

[S49] C++：写文件
来源：http://srb.yueranfly.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://pgp.shzxlz.cn

[S50] C++：格式化数字
来源：http://dxi.ywan-chungtsiang.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://tec.bbcook.cn

[S51] C++：显式类型转换
来源：http://shi.tianlin.xyz

static_cast<double>(a) / b
来源：http://dab.uphjek.com

[S52] C++：const 与 noexcept
来源：http://ead.sxryk.cn

int size() const noexcept { return n_; }
来源：http://cku.yj202588.top

[S53] C++：移动语义
来源：http://fzg.shuidangran.top

std::vector<int> w = std::move(v);
来源：http://noj.sufxvd.cn

[S54] C++：异常处理
来源：http://mtu.bbcook.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://wij.chenjidiqi.icu

[S55] C++：结构化绑定
来源：http://mwn.snrcjt.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://qar.fehbvm.com

[S56] C++：optional
来源：http://nhs.shzxlz.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://ebx.tianlin.xyz

[S57] C++：编译期常量
来源：http://zcx.zdbjq.cn

constexpr int N = 10;
来源：http://exk.redwolf501.top

[S58] C++：命名空间
来源：http://dfs.jyoumei.cn

namespace ns { int f() { return 1; } }
来源：http://ntq.cucudq.cn

[S59] C++：静态断言
来源：http://ktk.zdbjq.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://blr.dianchejie.cn

[S60] C++：遍历并删除元素
来源：http://que.wangshuangyany.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hgy.fktsv.cn

================================================================================
来源：http://uaf.yuanzhike.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://zma.svipenyu.cn

================================================================================
来源：http://jbk.jqgufenzy.top

[T01] Kotlin：Hello World
来源：http://omb.jqgufenzy.top

println("Hello")
来源：http://dee.jqgufenzy.top

[T02] Kotlin：变量
来源：http://kcy.snrcjt.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://lbl.0kj1m.cn

[T03] Kotlin：字符串模板
来源：http://utu.quarkkingdee.top

"值: $b"
来源：http://qll.yj20258888.top

[T04] Kotlin：空安全
来源：http://zxc.fanxiaobao.xyz

val n: String? = null;  n?.length
来源：http://ioo.jqgfzy.top

[T05] Kotlin：when 表达式
来源：http://bjv.xingfuxueyuan.xyz

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://cqe.iojbl.cn

[T06] Kotlin：集合映射
来源：http://lzr.dianchejie.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://gfv.gaohongyu789.top

[T07] Kotlin：集合过滤
来源：http://cbj.ehwqpu.com

listOf(1, 2, 3).filter { it > 1 }
来源：http://veg.guowangkeji.top

[T08] Kotlin：数据类
来源：http://vka.zhoulong.xyz

data class User(val name: String, val age: Int)
来源：http://uzq.tanke756.top

[T09] Kotlin：扩展函数
来源：http://mct.jqgfzy.top

fun String.exclaim() = this + "!"
来源：http://jqq.yj202588.top

[T10] Kotlin：默认参数
来源：http://mvq.jinqigufen.top

fun greet(name: String = "World") = "Hi $name"
来源：http://wjg.tian-w.cn

[T11] Kotlin：协程
来源：http://wcw.chenjidiqi.icu

GlobalScope.launch { delay(1000); println("done") }
来源：http://ojb.jinyuanbaomall.cn

[T12] Kotlin：解构声明
来源：http://nui.ctjpmb.com

val (a, b) = Pair(1, 2)
来源：http://sab.52xcode.cn

[T13] Kotlin：只读 Map
来源：http://azo.yonumen.top

val m = mapOf("a" to 1)
来源：http://aoo.fehbvm.com

[T14] Kotlin：循环
来源：http://mml.yuanzhike.top

for (i in 1..10) println(i)
来源：http://pbv.jyoumei.cn

[T15] Kotlin：接口
来源：http://lub.sufxvd.cn

interface Shape { fun area(): Double }
来源：http://svx.uphjek.com

[T16] Swift：Hello World
来源：http://zdn.daxiang520.top

print("Hello")
来源：http://kla.pengpengdd.cyou

[T17] Swift：变量与常量
来源：http://jla.hesvh.cn

var a = 1;  let b = 2
来源：http://uzn.gzhubu.top

[T18] Swift：字符串插值
来源：http://jkf.dianchejie.cn

"值: \(b)"
来源：http://nhy.ydzc1.top

[T19] Swift：可选绑定
来源：http://dcc.jianghu66.top

if let n = opt { print(n) }
来源：http://tre.bjfxy.top

[T20] Swift：数组操作
来源：http://yzq.jianghu66.top

var a = [1, 2, 3];  a.append(4)
来源：http://ikh.yj202588.top

[T21] Swift：遍历
来源：http://nyp.wangshuangyany.cn

for x in a { print(x) }
来源：http://vko.yueranfly.top

[T22] Swift：字典
来源：http://ejb.andypj.xyz

var d = ["a": 1];  d["b"] = 2
来源：http://gsh.jqgfzy.top

[T23] Swift：函数
来源：http://xqh.fengsongda.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://ops.fanxiaobao.xyz

[T24] Swift：闭包
来源：http://dni.birdmap.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://opt.zhaomingkeji.xyz

[T25] Swift：结构体
来源：http://csh.jlsjyb.cn

struct P { var x: Int }
来源：http://vqp.ydjk.org.cn

[T26] Swift：类与重写
来源：http://faq.wangdashe.top

class A: Base { override func f() {} }
来源：http://eme.xinyue.icu

[T27] Swift：错误处理
来源：http://mph.shangyingyoupin.top

do { try f() } catch { print(error) }
来源：http://jdf.yj20258888.top

[T28] Swift：枚举
来源：http://ecr.yangfankeji.com

enum Color { case red, green }
来源：http://iym.yfazqb.com

[T29] Swift：guard 提前返回
来源：http://zio.ybcxt.top

guard let x = opt else { return }
来源：http://yic.jinyuanbaomall.cn

[T30] Swift：协议
来源：http://qqk.zdqjudy.top

protocol Shape { func area() -> Double }
来源：http://jcs.shangyingyoupin.top

[T31] Lua：Hello World
来源：http://rxd.jiagoushi.top

print("Hello")
来源：http://tbu.dianchejie.cn

[T32] Lua：局部变量
来源：http://kng.jinqigfzy.top

local a = 1
来源：http://lux.bbcook.cn

[T33] Lua：表（数组）
来源：http://vlj.sufxvd.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://dkk.nanxuanxn.top

[T34] Lua：遍历表
来源：http://xui.yueranfly.top

for i, v in ipairs(t) do print(i, v) end
来源：http://jyr.chenlongwang.top

[T35] Lua：字典表
来源：http://dob.zhijiandao.cn

local d = { a = 1 };  d.b = 2
来源：http://uhv.ydzc1.top

[T36] Lua：函数
来源：http://anb.yuxming.cn

function add(a, b) return a + b end
来源：http://qmk.xuetiantiany.cn

[T37] Lua：字符串拼接
来源：http://lyg.kuanghao11.cn

"a" .. "b"
来源：http://nmx.52xcode.cn

[T38] Lua：条件
来源：http://llc.smart0.xyz

if x > 0 then print("正") end
来源：http://tgc.ppjwa.cn

[T39] Lua：模式匹配
来源：http://zrb.shangyingyoupin.top

string.find(s, "%d+")
来源：http://vzk.yvedp.cn

[T40] Lua：元表
来源：http://jaj.zdqjudy.top

setmetatable({}, { __index = base })
来源：http://bpa.hysaishi.cn

[T41] Perl：Hello World
来源：http://vxa.hfpthk.cn

print "Hello\n";
来源：http://ova.chenjidiqi.icu

[T42] Perl：变量类型
来源：http://bje.zhengqikj.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://nob.cashguo.top

[T43] Perl：字符串插值
来源：http://hcj.gogol.net.cn

"值: $a"
来源：http://nuw.gotoacloud.top

[T44] Perl：条件
来源：http://trm.chenjidiqi.icu

if ($a > 0) { print "正"; }
来源：http://jxd.kuanghao11.cn

[T45] Perl：数组遍历
来源：http://fmy.vqdsnc.cn

for my $x (@arr) { print $x; }
来源：http://pgr.shzxlz.cn

[T46] Perl：哈希操作
来源：http://skv.chenjidiqi.icu

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://zrk.fengsongda.top

[T47] Perl：正则捕获
来源：http://xml.chenjidiqi.icu

if ($s =~ /(\d+)/) { print $1; }
来源：http://rfp.wangshuangyany.cn

[T48] Perl：正则替换
来源：http://bsy.xuanzx.com

$s =~ s/old/new/g;
来源：http://ota.tianlin.xyz

[T49] Perl：函数
来源：http://fei.nanxinkj.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://yid.yanxiufei.cn

[T50] Perl：逐行读文件
来源：http://mye.zhixingplan.top

open my $fh, "<", "a.txt" or die $!;
来源：http://zuk.jlsjyb.cn

while (my $line = <$fh>) { print $line; }
来源：http://vnm.haohaochexian.top

[T51] Scala：Hello World
来源：http://yew.yongpay.top

println("Hello")
来源：http://gnj.daxiang520.top

[T52] Scala：变量
来源：http://vkq.dianchejie.cn

val a = 1;  var b = 2
来源：http://qer.ctjpmb.com

[T53] Scala：字符串插值
来源：http://blj.iojbl.cn

s"值: $b"
来源：http://hec.hysaishi.cn

[T54] Scala：集合映射
来源：http://awg.shanyushiyangtech.top

List(1, 2, 3).map(_ * 2)
来源：http://nrr.zdbjq.cn

[T55] Scala：集合过滤
来源：http://fpg.zhaomingkeji.xyz

List(1, 2, 3).filter(_ > 1)
来源：http://rvk.sufxvd.cn

[T56] Scala：样例类
来源：http://yth.hesvh.cn

case class User(name: String, age: Int)
来源：http://alg.sysykeji.top

[T57] Scala：模式匹配
来源：http://prs.hongshengwenyu.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://ajk.snrcjt.cn

[T58] Scala：函数定义
来源：http://wft.havefunace.top

def add(a: Int, b: Int): Int = a + b
来源：http://dst.quarkkingdee.top

[T59] Scala：循环
来源：http://wwb.nanxinkj.top

for (i <- 1 to 10) println(i)
来源：http://dvn.gaohongyu789.top

[T60] Scala：折叠
来源：http://xai.cdnleiting.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hhr.daria6918.cn

================================================================================
来源：http://kkt.316326.xyz

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://lrz.jianghu66.top

================================================================================
来源：http://rqr.zdbjq.cn

[U01] Py：创建虚拟环境
来源：http://jok.bjfxy.top

python -m venv .venv && source .venv/bin/activate
来源：http://apg.hnqzz.top

[U02] Py：导出 / 安装依赖
来源：http://sye.birdmap.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://xgs.jinyuanbaomall.cn

[U03] Py：加载 .env 配置
来源：http://nke.mhx1999.top

from dotenv import load_dotenv; load_dotenv()
来源：http://oof.jinqigfzy.top

[U04] Py：变量调试打印
来源：http://urn.tarul.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hoh.fzhhl.top

[U05] Py：列表去重且保序
来源：http://bsq.ehwqpu.com

list(dict.fromkeys(arr))
来源：http://vvf.jyoumei.cn

[U06] Py：合并两个字典
来源：http://rrl.wangshuangyany.cn

{**a, **b}
来源：http://kzb.hnxiangtu.top

[U07] Py：反转字典键值
来源：http://aaz.ydjk.org.cn

{v: k for k, v in d.items()}
来源：http://xtk.gaohongyu789.top

[U08] Py：展平二维列表
来源：http://kic.snrcjt.cn

[y for x in nested for y in x]
来源：http://kpj.316326.xyz

[U09] Py：字典取最大值的键
来源：http://ceq.kuanghao11.cn

max(d, key=d.get)
来源：http://duf.hcnkem.com

[U10] Py：按值排序字典
来源：http://cgc.shzxlz.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://uqv.chenzaomai.com

[U11] Py：生成器表达式
来源：http://ayd.fehbvm.com

(x * 2 for x in arr)
来源：http://qog.jinghuilouyu.cn

[U12] Py：取出现最多的 3 个元素
来源：http://prb.gotoacloud.top

Counter(arr).most_common(3)
来源：http://qjy.cheryme.top

[U13] Py：固定长度队列
来源：http://pos.cucudq.cn

deque(maxlen=10)
来源：http://fxh.tarul.cn

[U14] Py：分组收集到列表
来源：http://ihi.yj202588.top

defaultdict(list)
来源：http://abq.vehdjk.com

[U15] Py：高精度计时
来源：http://kbz.gzhubu.top

t = time.perf_counter()
来源：http://qtz.jianghu66.top

[U16] Py：命令行参数解析
来源：http://vrx.meibo888.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://nfe.epnwcf.com


<!-- 参考信息 -->