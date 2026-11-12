代发 wailian999

openssl rand -hex 16
来源：http://gdn.fktsv.cn

[R68] 计算文件校验值
来源：http://kuc.jinyuanbaomall.cn

sha256sum a.txt;  md5sum a.txt
来源：http://xst.yj20258.top

[R69] 生成随机密码
来源：http://dgw.birdmap.top

head -c 16 /dev/urandom | base64
来源：http://whd.sweek.top

[R70] 时间戳与互转
来源：http://aja.hcnkem.com

date +%s;  date -d @1700000000
来源：http://xrz.fanxiaobao.xyz

[R71] 日期格式化
来源：http://kqq.hesvh.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://lkc.xylfe.cn

[R72] 等待端口就绪
来源：http://sfv.zhoulong.xyz

until nc -z localhost 3306; do sleep 1; done
来源：http://qcp.nanxuanxn.top

[R73] 分割大日志
来源：http://jxl.cucudq.cn

split -l 1000 big.log part_
来源：http://zez.9152youxi.cn

[R74] 批量重命名
来源：http://vpe.pengpengdd.cyou

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://lif.jinghuilouyu.cn

[R75] 导出环境变量
来源：http://vdi.316326.xyz

export PATH="$HOME/bin:$PATH"
来源：http://lbp.smart0.xyz

[R76] 使用临时文件
来源：http://ihh.wangdashe.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hga.ppjwa.cn

[R77] 读取用户输入
来源：http://llx.jinqigufen.top

read -rp "请输入: " ans
来源：http://pfr.cqqwz.cn

[R78] 交互式菜单
来源：http://knr.yj202588.top

select opt in a b c; do echo "$opt"; break; done
来源：http://tno.meibo888.top

[R79] 解析命令行选项
来源：http://jlr.yfazqb.com

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://xlq.jinqigfzy.top

[R80] 查看脚本执行耗时
来源：http://wvs.fanxiaobao.xyz

time ./run.sh
来源：http://ylb.yangfankeji.com

================================================================================
来源：http://srh.svipenyu.cn

S. C / C++ 专题
来源：http://pzh.chenjidiqi.icu

================================================================================
来源：http://ofi.jqgufenzy.top

[S01] C：Hello World
来源：http://mdm.cheryme.top

#include <stdio.h>
来源：http://qla.yuanzhike.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://yfi.hnqzz.top

[S02] C：变量与格式化输出
来源：http://qtz.52xcode.cn

int a = 10; printf("%d\n", a);
来源：http://nrz.fktsv.cn

[S03] C：读入整数
来源：http://stk.ydzc1.top

int x; scanf("%d", &x);
来源：http://tmg.nanxinkj.top

[S04] C：字符串复制
来源：http://enh.zhiwuduotai.top

char dst[32]; strcpy(dst, "hi");
来源：http://mkm.bbcook.cn

[S05] C：字符串长度
来源：http://cob.zhengqikj.top

strlen(s)
来源：http://hvp.0kj1m.cn

[S06] C：字符串比较
来源：http://wnq.tarul.cn

strcmp(a, b) == 0
来源：http://juw.tanke756.top

[S07] C：数组遍历求和
来源：http://rju.jinqigufen.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://utb.yj20258888.top

[S08] C：动态内存分配与释放
来源：http://cwa.gzhubu.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://ggy.andypj.xyz

[S09] C：结构体定义与初始化
来源：http://hjk.zhoulong.xyz

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://szf.shanyushiyangtech.top

[S10] C：指针与解引用
来源：http://flw.feifeiyinyue.top

int *p = &a;  *p = 5;
来源：http://ogk.redwolf501.top

[S11] C：逐行读文件
来源：http://gyr.birdmap.top

FILE *f = fopen("a.txt", "r");
来源：http://uep.wangdashe.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://usi.fengsongda.top

fclose(f);
来源：http://rkt.zdqjudy.top

[S12] C：写文件
来源：http://izm.svipenyu.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://kuq.sysykeji.top

[S13] C：宏定义
来源：http://ock.daxiang520.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://mtm.zhaomingkeji.xyz

[S14] C：枚举
来源：http://zsu.tanke756.top

enum Color { RED, GREEN, BLUE };
来源：http://mhj.hammf.cn

[S15] C：类型转换
来源：http://gxf.shanyushiyangtech.top

(double) a / b
来源：http://sge.smart0.xyz

[S16] C：位操作置位
来源：http://lsz.sxryk.cn

x |= (1 << 3);
来源：http://hbb.ppjwa.cn

[S17] C：安全拼接字符串
来源：http://jhe.xingfuxueyuan.xyz

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://lqd.yj202588.top

[S18] C：命令行参数
来源：http://uud.mhx1999.top

int main(int argc, char **argv)
来源：http://zvm.xingfuxueyuan.xyz

[S19] C：快速排序
来源：http://gcg.316326.xyz

qsort(a, n, sizeof(int), cmp);
来源：http://zda.chenlongwang.top

[S20] C：二分查找
来源：http://qtq.hfpthk.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://tas.dianchejie.cn

[S21] C：字符类别判断
来源：http://yzq.sjlbkw.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://tsq.yongpay.top

[S22] C：字符串转数字
来源：http://mpn.hesvh.cn

atoi("42");  strtod("3.14", NULL);
来源：http://kdo.jinqigufen.top

[S23] C：随机数
来源：http://kaj.bbcook.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://eqj.kuanghao11.cn

[S24] C：获取本地时间
来源：http://gvn.316326.xyz

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://mon.ehwqpu.com

[S25] C：内存拷贝
来源：http://uop.hysaishi.cn

memcpy(dst, src, n);
来源：http://muz.yj202588.top

[S26] C：内存清零
来源：http://dpx.ehwqpu.com

memset(a, 0, sizeof a);
来源：http://tdq.gaohongyu789.top

[S27] C：定义常量
来源：http://hjd.bjfxy.top

const double PI = 3.14159;
来源：http://tpc.sweek.top

[S28] C：静态变量
来源：http://zep.tian-w.cn

static int counter = 0;
来源：http://hws.vehdjk.com

[S29] C：变参函数
来源：http://dbu.sjlbkw.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://dkq.tian-w.cn

[S30] C：头文件保护
来源：http://qih.shanyushiyangtech.top

#ifndef X_H
来源：http://nwu.uphjek.com

#define X_H
来源：http://pha.sxryk.cn

#endif
来源：http://kpn.vehdjk.com

[S31] C++：Hello World
来源：http://wfo.daria6918.cn

#include <iostream>
来源：http://vdh.ctjpmb.com

int main() { std::cout << "Hello\n"; }
来源：http://rrs.hfpthk.cn

[S32] C++：字符串
来源：http://tzr.zhixingplan.top

std::string s = "hi";  s += "!";
来源：http://xtl.meibo888.top

[S33] C++：vector 增删
来源：http://arz.gaohongyu789.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://ruv.yueranfly.top

[S34] C++：遍历 vector
来源：http://vjp.gotoacloud.top

for (auto &x : v) { std::cout << x; }
来源：http://lbg.yuanzhike.top

[S35] C++：map
来源：http://mbc.ybcxt.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://avx.shangyingyoupin.top

[S36] C++：unordered_map
来源：http://zka.sufxvd.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://lfx.yuanzhike.top

[S37] C++：set
来源：http://vup.xziqi.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://cin.316326.xyz

[S38] C++：排序
来源：http://szv.zhijiandao.cn

std::sort(v.begin(), v.end());
来源：http://oas.yj20258888.top

[S39] C++：自定义比较器排序
来源：http://iau.jyoumei.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://sdx.zhongyouzk.top

[S40] C++：查找元素
来源：http://cob.shzxlz.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://udk.chenlongwang.top

[S41] C++：类与构造函数
来源：http://jgl.jiagoushi.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://svq.hongshengwenyu.top

[S42] C++：继承与虚函数
来源：http://xfe.fzhhl.top

class B : public Base { public: void f() override {} };
来源：http://dvo.jiagoushi.top

[S43] C++：智能指针
来源：http://tgf.yonumen.top

auto p = std::make_unique<int>(5);
来源：http://ezj.bbcook.cn

[S44] C++：引用传参
来源：http://nen.zhixingplan.top

void inc(int &x) { ++x; }
来源：http://hst.ybcxt.top

[S45] C++：lambda
来源：http://bkd.jqgufenzy.top

auto add = [](int a, int b) { return a + b; };
来源：http://mvs.zhijiandao.cn

[S46] C++：函数模板
来源：http://mwt.yuanzhike.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://rqx.vehdjk.com

[S47] C++：结构化绑定遍历
来源：http://qic.ywan-chungtsiang.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://rrd.yj202588.top

[S48] C++：逐行读文件
来源：http://mpx.yvedp.cn

std::ifstream in("a.txt");  std::string line;
来源：http://lmv.nanxuanxn.top

while (std::getline(in, line)) { }
来源：http://hkz.sxryk.cn

[S49] C++：写文件
来源：http://yjk.tian-w.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://zas.yj202588.top

[S50] C++：格式化数字
来源：http://xwz.jyoumei.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://gcq.fehbvm.com

[S51] C++：显式类型转换
来源：http://rpg.jyoumei.cn

static_cast<double>(a) / b
来源：http://yoi.ydjk.org.cn

[S52] C++：const 与 noexcept
来源：http://zyu.jinghuilouyu.cn

int size() const noexcept { return n_; }
来源：http://oww.0kj1m.cn

[S53] C++：移动语义
来源：http://tqw.xuetiantiany.cn

std::vector<int> w = std::move(v);
来源：http://rfz.meibo888.top

[S54] C++：异常处理
来源：http://ftf.dianchejie.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://ixj.mhx1999.top

[S55] C++：结构化绑定
来源：http://beq.yangfankeji.com

auto [a, b] = std::make_pair(1, 2);
来源：http://als.ctjpmb.com

[S56] C++：optional
来源：http://auy.ctjpmb.com

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://joe.jinqigufen.top

[S57] C++：编译期常量
来源：http://mhm.guannengcc.top

constexpr int N = 10;
来源：http://bga.quarkkingdee.top

[S58] C++：命名空间
来源：http://fuo.jinqigufen.top

namespace ns { int f() { return 1; } }
来源：http://ima.zdbjq.cn

[S59] C++：静态断言
来源：http://aep.hcnkem.com

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://vqq.gogol.net.cn

[S60] C++：遍历并删除元素
来源：http://hop.9152youxi.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://ilo.zhoulong.xyz

================================================================================
来源：http://gni.birdmap.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://jxj.xinyue.icu

================================================================================
来源：http://icu.tarul.cn

[T01] Kotlin：Hello World
来源：http://qjx.meibo888.top

println("Hello")
来源：http://dba.sufxvd.cn

[T02] Kotlin：变量
来源：http://crp.jianghu66.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://olw.guannengcc.top

[T03] Kotlin：字符串模板
来源：http://qgx.yj202588.top

"值: $b"
来源：http://bjf.xziqi.cn

[T04] Kotlin：空安全
来源：http://rlu.jinqigufen.top

val n: String? = null;  n?.length
来源：http://wnt.daxiang520.top

[T05] Kotlin：when 表达式
来源：http://xoi.xingfuxueyuan.xyz

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://zrm.daxiang520.top

[T06] Kotlin：集合映射
来源：http://jho.fehbvm.com

listOf(1, 2, 3).map { it * 2 }
来源：http://mae.ppjwa.cn

[T07] Kotlin：集合过滤
来源：http://gzm.wangshuangyany.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://isp.ywan-chungtsiang.top

[T08] Kotlin：数据类
来源：http://cei.nanxinkj.top

data class User(val name: String, val age: Int)
来源：http://xoh.0kj1m.cn

[T09] Kotlin：扩展函数
来源：http://tbm.ivvv.top

fun String.exclaim() = this + "!"
来源：http://ble.pycfn.com

[T10] Kotlin：默认参数
来源：http://txk.ydzc1.top

fun greet(name: String = "World") = "Hi $name"
来源：http://pgg.hfpthk.cn

[T11] Kotlin：协程
来源：http://gxd.yanxiufei.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://eob.sweek.top

[T12] Kotlin：解构声明
来源：http://dqs.hnqzz.top

val (a, b) = Pair(1, 2)
来源：http://waa.xylfe.cn

[T13] Kotlin：只读 Map
来源：http://pic.zhiwuduotai.top

val m = mapOf("a" to 1)
来源：http://fkx.zhixingplan.top

[T14] Kotlin：循环
来源：http://gio.xinyue.icu

for (i in 1..10) println(i)
来源：http://enp.jqgufenzy.top

[T15] Kotlin：接口
来源：http://sff.sweek.top

interface Shape { fun area(): Double }
来源：http://onh.316326.xyz

[T16] Swift：Hello World
来源：http://psn.tian-w.cn

print("Hello")
来源：http://cxk.jqgufenzy.top

[T17] Swift：变量与常量
来源：http://zgq.tianlin.xyz

var a = 1;  let b = 2
来源：http://wez.yj202588.top

[T18] Swift：字符串插值
来源：http://jde.jinqigfzy.top

"值: \(b)"
来源：http://lgf.nanxuanxn.top

[T19] Swift：可选绑定
来源：http://frd.tanke756.top

if let n = opt { print(n) }
来源：http://cgr.dianchejie.cn

[T20] Swift：数组操作
来源：http://jej.snrcjt.cn

var a = [1, 2, 3];  a.append(4)
来源：http://fqz.ehwqpu.com

[T21] Swift：遍历
来源：http://lho.cdnleiting.top

for x in a { print(x) }
来源：http://fvh.ybcxt.top

[T22] Swift：字典
来源：http://yhk.zhixingplan.top

var d = ["a": 1];  d["b"] = 2
来源：http://clv.316326.xyz

[T23] Swift：函数
来源：http://phf.kuanghao11.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://cgm.cucudq.cn

[T24] Swift：闭包
来源：http://ilc.gogol.net.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://rgn.tanke756.top

[T25] Swift：结构体
来源：http://htn.bjfxy.top

struct P { var x: Int }
来源：http://pnt.shzxlz.cn

[T26] Swift：类与重写
来源：http://gda.xuanzx.com

class A: Base { override func f() {} }
来源：http://ynz.gzhubu.top

[T27] Swift：错误处理
来源：http://bqm.daxiang520.top

do { try f() } catch { print(error) }
来源：http://yjl.tanke756.top

[T28] Swift：枚举
来源：http://ijg.svipenyu.cn

enum Color { case red, green }
来源：http://cnl.316326.xyz

[T29] Swift：guard 提前返回
来源：http://pxg.zdbjq.cn

guard let x = opt else { return }
来源：http://fkl.zdbjq.cn

[T30] Swift：协议
来源：http://rjm.xinyue.icu

protocol Shape { func area() -> Double }
来源：http://cqy.jinqigufen.top

[T31] Lua：Hello World
来源：http://ggj.yueranfly.top

print("Hello")
来源：http://xch.andypj.xyz

[T32] Lua：局部变量
来源：http://bqd.epnwcf.com

local a = 1
来源：http://hpc.chenlongwang.top

[T33] Lua：表（数组）
来源：http://nxk.gzhubu.top

local t = {1, 2, 3};  t[4] = 4
来源：http://ngd.xylfe.cn

[T34] Lua：遍历表
来源：http://ufk.pycfn.com

for i, v in ipairs(t) do print(i, v) end
来源：http://msj.havefunace.top

[T35] Lua：字典表
来源：http://taa.fzhhl.top

local d = { a = 1 };  d.b = 2
来源：http://kxk.meibo888.top

[T36] Lua：函数
来源：http://mgd.aibaodan.cn

function add(a, b) return a + b end
来源：http://nka.haohaochexian.top

[T37] Lua：字符串拼接
来源：http://jva.shzxlz.cn

"a" .. "b"
来源：http://tdi.guannengcc.top

[T38] Lua：条件
来源：http://ryv.nanxuanxn.top

if x > 0 then print("正") end
来源：http://bmy.iojbl.cn

[T39] Lua：模式匹配
来源：http://sqz.hysaishi.cn

string.find(s, "%d+")
来源：http://lfe.yuanzhike.top

[T40] Lua：元表
来源：http://hfi.redwolf501.top

setmetatable({}, { __index = base })
来源：http://jwq.shzxlz.cn

[T41] Perl：Hello World
来源：http://fuk.9152youxi.cn

print "Hello\n";
来源：http://ega.ppjwa.cn

[T42] Perl：变量类型
来源：http://tqi.fehbvm.com

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://qks.ydjk.org.cn

[T43] Perl：字符串插值
来源：http://nue.iojbl.cn

"值: $a"
来源：http://wqf.birdmap.top

[T44] Perl：条件
来源：http://llg.kuanghao11.cn

if ($a > 0) { print "正"; }
来源：http://ntd.yangfankeji.com

[T45] Perl：数组遍历
来源：http://yvd.gotoacloud.top

for my $x (@arr) { print $x; }
来源：http://qga.sxryk.cn

[T46] Perl：哈希操作
来源：http://ats.hongshengwenyu.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://xow.pengpengdd.cyou

[T47] Perl：正则捕获
来源：http://aec.zhoulong.xyz

if ($s =~ /(\d+)/) { print $1; }
来源：http://vtk.52xcode.cn

[T48] Perl：正则替换
来源：http://dbr.wangdashe.top

$s =~ s/old/new/g;
来源：http://dkf.shzxlz.cn

[T49] Perl：函数
来源：http://tjf.mhx1999.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://eoo.xinyue.icu

[T50] Perl：逐行读文件
来源：http://zmx.epnwcf.com

open my $fh, "<", "a.txt" or die $!;
来源：http://ldn.pycfn.com

while (my $line = <$fh>) { print $line; }
来源：http://ljy.sjlbkw.cn

[T51] Scala：Hello World
来源：http://zno.kuanghao11.cn

println("Hello")
来源：http://blc.yuxming.cn

[T52] Scala：变量
来源：http://zps.feifeiyinyue.top

val a = 1;  var b = 2
来源：http://yyq.fehbvm.com

[T53] Scala：字符串插值
来源：http://lsu.dashuyun.cn

s"值: $b"
来源：http://xuo.jinyuanbaomall.cn

[T54] Scala：集合映射
来源：http://iaf.iojbl.cn

List(1, 2, 3).map(_ * 2)
来源：http://ozm.cdnleiting.top

[T55] Scala：集合过滤
来源：http://vra.sweek.top

List(1, 2, 3).filter(_ > 1)
来源：http://hiq.cheryme.top

[T56] Scala：样例类
来源：http://vgu.ydzc1.top

case class User(name: String, age: Int)
来源：http://nhe.hesvh.cn

[T57] Scala：模式匹配
来源：http://kul.havefunace.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://yjg.ywan-chungtsiang.top

[T58] Scala：函数定义
来源：http://lzs.sysykeji.top

def add(a: Int, b: Int): Int = a + b
来源：http://kje.hammf.cn

[T59] Scala：循环
来源：http://pxi.zhixingplan.top

for (i <- 1 to 10) println(i)
来源：http://zeh.fengsongda.top

[T60] Scala：折叠
来源：http://jfg.hfpthk.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://anm.cqqwz.cn

================================================================================
来源：http://kgy.cqqwz.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://udk.sweek.top

================================================================================
来源：http://vsb.zdbjq.cn

[U01] Py：创建虚拟环境
来源：http://orf.ehwqpu.com

python -m venv .venv && source .venv/bin/activate
来源：http://rmu.xuanzx.com

[U02] Py：导出 / 安装依赖
来源：http://lao.jinqigufen.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://gxu.ctjpmb.com

[U03] Py：加载 .env 配置
来源：http://hsn.xylfe.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://qbh.c1oappe.top

[U04] Py：变量调试打印
来源：http://ori.zhixingplan.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://zrm.hnqzz.top

[U05] Py：列表去重且保序
来源：http://rec.meibo888.top

list(dict.fromkeys(arr))
来源：http://cdq.jinqigufen.top

[U06] Py：合并两个字典
来源：http://rhf.wangdashe.top

{**a, **b}
来源：http://qwu.shanyushiyangtech.top

[U07] Py：反转字典键值
来源：http://zsy.cdnleiting.top

{v: k for k, v in d.items()}
来源：http://huy.jyoumei.cn

[U08] Py：展平二维列表
来源：http://yot.yanxiufei.cn

[y for x in nested for y in x]
来源：http://xbd.shanyushiyangtech.top


<!-- 参考信息 -->