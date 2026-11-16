代发 wailian999

openssl rand -hex 16
来源：http://rwh.gaohongyu789.top

[R68] 计算文件校验值
来源：http://krj.dashuyun.cn

sha256sum a.txt;  md5sum a.txt
来源：http://all.xingfuxueyuan.xyz

[R69] 生成随机密码
来源：http://bce.yangfankeji.com

head -c 16 /dev/urandom | base64
来源：http://why.zhengqikj.top

[R70] 时间戳与互转
来源：http://aui.fanxiaobao.xyz

date +%s;  date -d @1700000000
来源：http://jvf.tanke756.top

[R71] 日期格式化
来源：http://ezy.hfpthk.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://nyd.zhiwuduotai.top

[R72] 等待端口就绪
来源：http://wxz.ydzc1.top

until nc -z localhost 3306; do sleep 1; done
来源：http://rti.guowangkeji.top

[R73] 分割大日志
来源：http://phq.jyoumei.cn

split -l 1000 big.log part_
来源：http://oxv.hnxiangtu.top

[R74] 批量重命名
来源：http://elh.fzhhl.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://tyn.xuetiantiany.cn

[R75] 导出环境变量
来源：http://uio.gaohongyu789.top

export PATH="$HOME/bin:$PATH"
来源：http://vka.nanxuanxn.top

[R76] 使用临时文件
来源：http://ubp.hnxiangtu.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://nfy.iojbl.cn

[R77] 读取用户输入
来源：http://gza.cucudq.cn

read -rp "请输入: " ans
来源：http://tep.ybcxt.top

[R78] 交互式菜单
来源：http://hzj.hesvh.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://tnu.hfpthk.cn

[R79] 解析命令行选项
来源：http://ahb.nanxinkj.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://jmc.jianghu66.top

[R80] 查看脚本执行耗时
来源：http://scr.ybcxt.top

time ./run.sh
来源：http://und.fzhhl.top

================================================================================
来源：http://dcn.zdqjudy.top

S. C / C++ 专题
来源：http://prx.yuxming.cn

================================================================================
来源：http://gli.uphjek.com

[S01] C：Hello World
来源：http://qzx.epnwcf.com

#include <stdio.h>
来源：http://bwv.kuanghao11.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://mam.xziqi.cn

[S02] C：变量与格式化输出
来源：http://eki.yangfankeji.com

int a = 10; printf("%d\n", a);
来源：http://zla.fengsongda.top

[S03] C：读入整数
来源：http://yhb.jyoumei.cn

int x; scanf("%d", &x);
来源：http://ngg.cashguo.top

[S04] C：字符串复制
来源：http://hum.hongshengwenyu.top

char dst[32]; strcpy(dst, "hi");
来源：http://api.birdmap.top

[S05] C：字符串长度
来源：http://nmt.zhijiandao.cn

strlen(s)
来源：http://ttl.cashguo.top

[S06] C：字符串比较
来源：http://qzm.dianchejie.cn

strcmp(a, b) == 0
来源：http://mpt.smart0.xyz

[S07] C：数组遍历求和
来源：http://lkj.hywenlv.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://bpc.jlsjyb.cn

[S08] C：动态内存分配与释放
来源：http://azc.nanxuanxn.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://yem.iojbl.cn

[S09] C：结构体定义与初始化
来源：http://aes.xuanzx.com

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://ijw.tianlin.xyz

[S10] C：指针与解引用
来源：http://fww.daxiang520.top

int *p = &a;  *p = 5;
来源：http://mli.birdmap.top

[S11] C：逐行读文件
来源：http://krg.shangyingyoupin.top

FILE *f = fopen("a.txt", "r");
来源：http://ztd.hfpthk.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://tou.epnwcf.com

fclose(f);
来源：http://juj.bjfxy.top

[S12] C：写文件
来源：http://poa.gzhubu.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://jxv.shanyushiyangtech.top

[S13] C：宏定义
来源：http://gpw.nwbrower.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://teu.hammf.cn

[S14] C：枚举
来源：http://zsa.jqgfzy.top

enum Color { RED, GREEN, BLUE };
来源：http://wsn.zdqjudy.top

[S15] C：类型转换
来源：http://xwv.sjlbkw.cn

(double) a / b
来源：http://krz.vehdjk.com

[S16] C：位操作置位
来源：http://iza.cqqwz.cn

x |= (1 << 3);
来源：http://rwe.fengsongda.top

[S17] C：安全拼接字符串
来源：http://eei.shangyingyoupin.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://zhj.jlsjyb.cn

[S18] C：命令行参数
来源：http://ncw.yonumen.top

int main(int argc, char **argv)
来源：http://oyf.hcnkem.com

[S19] C：快速排序
来源：http://hng.gogol.net.cn

qsort(a, n, sizeof(int), cmp);
来源：http://wzb.vehdjk.com

[S20] C：二分查找
来源：http://zrq.fzhhl.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://xct.daxiang520.top

[S21] C：字符类别判断
来源：http://cnc.nanxinkj.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://byz.zdbjq.cn

[S22] C：字符串转数字
来源：http://asa.jianghu66.top

atoi("42");  strtod("3.14", NULL);
来源：http://rxm.andypj.xyz

[S23] C：随机数
来源：http://cnm.fehbvm.com

srand(time(NULL));  int r = rand() % 100;
来源：http://phy.52xcode.cn

[S24] C：获取本地时间
来源：http://pcp.epnwcf.com

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://fjo.yonumen.top

[S25] C：内存拷贝
来源：http://wnb.zhengqikj.top

memcpy(dst, src, n);
来源：http://oeq.daxiang520.top

[S26] C：内存清零
来源：http://ggz.mhx1999.top

memset(a, 0, sizeof a);
来源：http://thq.pycfn.com

[S27] C：定义常量
来源：http://uxc.kuanghao11.cn

const double PI = 3.14159;
来源：http://zmu.bjfxy.top

[S28] C：静态变量
来源：http://ikc.zycfv.cn

static int counter = 0;
来源：http://iep.gaohongyu789.top

[S29] C：变参函数
来源：http://vwy.jianghu66.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://svk.yvedp.cn

[S30] C：头文件保护
来源：http://soj.zycfv.cn

#ifndef X_H
来源：http://kri.yangfankeji.com

#define X_H
来源：http://duz.yongpay.top

#endif
来源：http://jol.jiagoushi.top

[S31] C++：Hello World
来源：http://byi.yuxming.cn

#include <iostream>
来源：http://vcr.meibo888.top

int main() { std::cout << "Hello\n"; }
来源：http://qao.yfazqb.com

[S32] C++：字符串
来源：http://yvq.epnwcf.com

std::string s = "hi";  s += "!";
来源：http://cub.feifeiyinyue.top

[S33] C++：vector 增删
来源：http://bdr.gzhubu.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hyh.gotoacloud.top

[S34] C++：遍历 vector
来源：http://jyd.ywan-chungtsiang.top

for (auto &x : v) { std::cout << x; }
来源：http://hvc.feifeiyinyue.top

[S35] C++：map
来源：http://uwp.sysykeji.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hxp.yanxiufei.cn

[S36] C++：unordered_map
来源：http://bho.dashuyun.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://avn.quarkkingdee.top

[S37] C++：set
来源：http://vnf.hnxiangtu.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://fzd.sufxvd.cn

[S38] C++：排序
来源：http://pdr.9152youxi.cn

std::sort(v.begin(), v.end());
来源：http://tzh.shanyushiyangkeji.top

[S39] C++：自定义比较器排序
来源：http://aez.yongpay.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://ymv.yj202588.top

[S40] C++：查找元素
来源：http://qxw.yvedp.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://pcu.cashguo.top

[S41] C++：类与构造函数
来源：http://tap.fzhhl.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://ygt.jyoumei.cn

[S42] C++：继承与虚函数
来源：http://kkz.shangyingyoupin.top

class B : public Base { public: void f() override {} };
来源：http://vvg.ivvv.top

[S43] C++：智能指针
来源：http://dsk.aibaodan.cn

auto p = std::make_unique<int>(5);
来源：http://mzm.zhixingplan.top

[S44] C++：引用传参
来源：http://lyf.redwolf501.top

void inc(int &x) { ++x; }
来源：http://ahe.cdnleiting.top

[S45] C++：lambda
来源：http://pea.pengpengdd.cyou

auto add = [](int a, int b) { return a + b; };
来源：http://woh.chenjidiqi.icu

[S46] C++：函数模板
来源：http://duo.nwbrower.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://sud.yuanzhike.top

[S47] C++：结构化绑定遍历
来源：http://jkt.jqgufenzy.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://oaa.ehwqpu.com

[S48] C++：逐行读文件
来源：http://knw.yj202588.top

std::ifstream in("a.txt");  std::string line;
来源：http://vcj.hongshengwenyu.top

while (std::getline(in, line)) { }
来源：http://qhr.gzhubu.top

[S49] C++：写文件
来源：http://edk.guowangkeji.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hpr.hammf.cn

[S50] C++：格式化数字
来源：http://lto.fanxiaobao.xyz

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://nyo.xylfe.cn

[S51] C++：显式类型转换
来源：http://vgr.zdbjq.cn

static_cast<double>(a) / b
来源：http://kwv.bbcook.cn

[S52] C++：const 与 noexcept
来源：http://rwm.guowangkeji.top

int size() const noexcept { return n_; }
来源：http://gsg.epnwcf.com

[S53] C++：移动语义
来源：http://nqs.chenjidiqi.icu

std::vector<int> w = std::move(v);
来源：http://sym.gzhubu.top

[S54] C++：异常处理
来源：http://vao.jinghuilouyu.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://cbq.quarkkingdee.top

[S55] C++：结构化绑定
来源：http://jat.jianghu66.top

auto [a, b] = std::make_pair(1, 2);
来源：http://shd.yuanzhike.top

[S56] C++：optional
来源：http://ghh.zhengqikj.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://oqi.jinqigfzy.top

[S57] C++：编译期常量
来源：http://cuo.52xcode.cn

constexpr int N = 10;
来源：http://fgm.havefunace.top

[S58] C++：命名空间
来源：http://ieu.gotoacloud.top

namespace ns { int f() { return 1; } }
来源：http://kek.hnxiangtu.top

[S59] C++：静态断言
来源：http://ejc.daria6918.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://oud.ydzc1.top

[S60] C++：遍历并删除元素
来源：http://svm.ppjwa.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://wrb.316326.xyz

================================================================================
来源：http://yvw.aizwys.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://mkg.yvedp.cn

================================================================================
来源：http://lyd.ivvv.top

[T01] Kotlin：Hello World
来源：http://kxg.yfazqb.com

println("Hello")
来源：http://gud.jyoumei.cn

[T02] Kotlin：变量
来源：http://ynq.hnxiangtu.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://bcv.jianghu66.top

[T03] Kotlin：字符串模板
来源：http://pbm.316326.xyz

"值: $b"
来源：http://dxc.gzhubu.top

[T04] Kotlin：空安全
来源：http://uru.yongpay.top

val n: String? = null;  n?.length
来源：http://rzm.yj20258.top

[T05] Kotlin：when 表达式
来源：http://vli.cqqwz.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://gya.yj202588.top

[T06] Kotlin：集合映射
来源：http://yqo.zhiwuduotai.top

listOf(1, 2, 3).map { it * 2 }
来源：http://atc.jiagoushi.top

[T07] Kotlin：集合过滤
来源：http://lkq.redwolf501.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://xzq.yuanzhike.top

[T08] Kotlin：数据类
来源：http://oyp.hcnkem.com

data class User(val name: String, val age: Int)
来源：http://egf.nanxuanxn.top

[T09] Kotlin：扩展函数
来源：http://hqs.iojbl.cn

fun String.exclaim() = this + "!"
来源：http://agf.kuanghao11.cn

[T10] Kotlin：默认参数
来源：http://tsn.jyoumei.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://ggn.hammf.cn

[T11] Kotlin：协程
来源：http://pxq.xuetiantiany.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://xmy.ydzc1.top

[T12] Kotlin：解构声明
来源：http://lze.xingfuxueyuan.xyz

val (a, b) = Pair(1, 2)
来源：http://fcx.quarkkingdee.top

[T13] Kotlin：只读 Map
来源：http://mwt.xuetiantiany.cn

val m = mapOf("a" to 1)
来源：http://lke.ydjk.org.cn

[T14] Kotlin：循环
来源：http://srp.jinghuilouyu.cn

for (i in 1..10) println(i)
来源：http://zmp.feifeiyinyue.top

[T15] Kotlin：接口
来源：http://pjt.xziqi.cn

interface Shape { fun area(): Double }
来源：http://ybd.hnxiangtu.top

[T16] Swift：Hello World
来源：http://zmq.yj20258.top

print("Hello")
来源：http://fkm.redwolf501.top

[T17] Swift：变量与常量
来源：http://hpp.jiagoushi.top

var a = 1;  let b = 2
来源：http://grt.uphjek.com

[T18] Swift：字符串插值
来源：http://rmh.hnqzz.top

"值: \(b)"
来源：http://mrp.xylfe.cn

[T19] Swift：可选绑定
来源：http://eno.cheryme.top

if let n = opt { print(n) }
来源：http://iky.cucudq.cn

[T20] Swift：数组操作
来源：http://sif.yj20258888.top

var a = [1, 2, 3];  a.append(4)
来源：http://yaf.xziqi.cn

[T21] Swift：遍历
来源：http://zsp.xingfuxueyuan.xyz

for x in a { print(x) }
来源：http://jpf.jinghuilouyu.cn

[T22] Swift：字典
来源：http://qeb.zdqjudy.top

var d = ["a": 1];  d["b"] = 2
来源：http://kgi.yangfankeji.com

[T23] Swift：函数
来源：http://sha.zhengqikj.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://bcj.daxiang520.top

[T24] Swift：闭包
来源：http://yui.jqgfzy.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://cfp.52xcode.cn

[T25] Swift：结构体
来源：http://cjj.yuxming.cn

struct P { var x: Int }
来源：http://yzq.cucudq.cn

[T26] Swift：类与重写
来源：http://hdp.hysaishi.cn

class A: Base { override func f() {} }
来源：http://kiz.ehwqpu.com

[T27] Swift：错误处理
来源：http://zjz.jinyuanbaomall.cn

do { try f() } catch { print(error) }
来源：http://kyf.quarkkingdee.top

[T28] Swift：枚举
来源：http://gux.jinqigfzy.top

enum Color { case red, green }
来源：http://fxy.aizwys.cn

[T29] Swift：guard 提前返回
来源：http://zwm.jinghuilouyu.cn

guard let x = opt else { return }
来源：http://tch.zdqjudy.top

[T30] Swift：协议
来源：http://kpy.daxiang520.top

protocol Shape { func area() -> Double }
来源：http://gsk.mhx1999.top

[T31] Lua：Hello World
来源：http://spt.cucudq.cn

print("Hello")
来源：http://qik.zdqjudy.top

[T32] Lua：局部变量
来源：http://wes.cqqwz.cn

local a = 1
来源：http://lkm.yangfankeji.com

[T33] Lua：表（数组）
来源：http://erf.dashuyun.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://rpp.ybcxt.top

[T34] Lua：遍历表
来源：http://lgj.guowangkeji.top

for i, v in ipairs(t) do print(i, v) end
来源：http://ryw.wangshuangyany.cn

[T35] Lua：字典表
来源：http://jpg.andypj.xyz

local d = { a = 1 };  d.b = 2
来源：http://qnn.zhengqikj.top

[T36] Lua：函数
来源：http://afz.jlsjyb.cn

function add(a, b) return a + b end
来源：http://vgc.gaohongyu789.top

[T37] Lua：字符串拼接
来源：http://oaf.yvedp.cn

"a" .. "b"
来源：http://nuc.yj20258.top

[T38] Lua：条件
来源：http://dto.ydzc1.top

if x > 0 then print("正") end
来源：http://cov.wangshuangyany.cn

[T39] Lua：模式匹配
来源：http://pvv.jinghuilouyu.cn

string.find(s, "%d+")
来源：http://sqq.quarkkingdee.top

[T40] Lua：元表
来源：http://mfi.jinghuilouyu.cn

setmetatable({}, { __index = base })
来源：http://lia.sufxvd.cn

[T41] Perl：Hello World
来源：http://mdi.iojbl.cn

print "Hello\n";
来源：http://uvb.feifeiyinyue.top

[T42] Perl：变量类型
来源：http://pyt.52xcode.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://ywj.jiagoushi.top

[T43] Perl：字符串插值
来源：http://qzt.zhengqikj.top

"值: $a"
来源：http://yib.yangfankeji.com

[T44] Perl：条件
来源：http://qhw.daria6918.cn

if ($a > 0) { print "正"; }
来源：http://xhu.jlsjyb.cn

[T45] Perl：数组遍历
来源：http://gbr.yanxiufei.cn

for my $x (@arr) { print $x; }
来源：http://lew.cucudq.cn

[T46] Perl：哈希操作
来源：http://jgc.zhijiandao.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://psw.uphjek.com

[T47] Perl：正则捕获
来源：http://bfk.xuetiantiany.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://edn.shanyushiyangkeji.top

[T48] Perl：正则替换
来源：http://dxt.nwbrower.top

$s =~ s/old/new/g;
来源：http://ofe.fengsongda.top

[T49] Perl：函数
来源：http://aom.gogol.net.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://see.9152youxi.cn

[T50] Perl：逐行读文件
来源：http://psy.shanyushiyangkeji.top

open my $fh, "<", "a.txt" or die $!;
来源：http://ckb.chenzaomai.com

while (my $line = <$fh>) { print $line; }
来源：http://iov.gogol.net.cn

[T51] Scala：Hello World
来源：http://wfl.sufxvd.cn

println("Hello")
来源：http://txb.sxryk.cn

[T52] Scala：变量
来源：http://arg.sweek.top

val a = 1;  var b = 2
来源：http://cfe.jinghuilouyu.cn

[T53] Scala：字符串插值
来源：http://nte.yj20258888.top

s"值: $b"
来源：http://xkc.ydjk.org.cn

[T54] Scala：集合映射
来源：http://kco.redwolf501.top

List(1, 2, 3).map(_ * 2)
来源：http://son.fktsv.cn

[T55] Scala：集合过滤
来源：http://uqy.hnqzz.top

List(1, 2, 3).filter(_ > 1)
来源：http://mhk.hnqzz.top

[T56] Scala：样例类
来源：http://vla.gaohongyu789.top

case class User(name: String, age: Int)
来源：http://pkt.zhoulong.xyz

[T57] Scala：模式匹配
来源：http://yvc.yj202588.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://fvs.shuidangran.top

[T58] Scala：函数定义
来源：http://cai.ydjk.org.cn

def add(a: Int, b: Int): Int = a + b
来源：http://dnn.iojbl.cn

[T59] Scala：循环
来源：http://fqu.zhoulong.xyz

for (i <- 1 to 10) println(i)
来源：http://foh.bbcook.cn

[T60] Scala：折叠
来源：http://foq.shangyingyoupin.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://fni.c1oappe.top

================================================================================
来源：http://qht.zhongyouzk.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://lbq.yuanzhike.top

================================================================================
来源：http://kdf.pycfn.com

[U01] Py：创建虚拟环境
来源：http://aam.shanyushiyangkeji.top

python -m venv .venv && source .venv/bin/activate
来源：http://xsi.cqqwz.cn

[U02] Py：导出 / 安装依赖
来源：http://ifd.guowangkeji.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://zky.fehbvm.com

[U03] Py：加载 .env 配置
来源：http://wil.hcnkem.com

from dotenv import load_dotenv; load_dotenv()
来源：http://npe.jinqigfzy.top

[U04] Py：变量调试打印
来源：http://ovu.shzxlz.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hxs.feifeiyinyue.top

[U05] Py：列表去重且保序
来源：http://ypo.chenlongwang.top

list(dict.fromkeys(arr))
来源：http://mmg.chenlongwang.top

[U06] Py：合并两个字典
来源：http://mhm.haohaochexian.top

{**a, **b}
来源：http://qkg.feifeiyinyue.top

[U07] Py：反转字典键值
来源：http://ubw.xuetiantiany.cn

{v: k for k, v in d.items()}
来源：http://mle.zhixingplan.top

[U08] Py：展平二维列表
来源：http://nhp.fengsongda.top

[y for x in nested for y in x]
来源：http://xql.yvedp.cn


<!-- 参考信息 -->