代发 wailian999

openssl rand -hex 16
来源：http://eyl.zhijiandao.cn

[R68] 计算文件校验值
来源：http://iog.iojbl.cn

sha256sum a.txt;  md5sum a.txt
来源：http://jzf.gzhubu.top

[R69] 生成随机密码
来源：http://sii.fengsongda.top

head -c 16 /dev/urandom | base64
来源：http://cjm.chenjidiqi.icu

[R70] 时间戳与互转
来源：http://wpa.jianghu66.top

date +%s;  date -d @1700000000
来源：http://tfm.jiagoushi.top

[R71] 日期格式化
来源：http://ueg.cashguo.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://jus.yueranfly.top

[R72] 等待端口就绪
来源：http://kos.yangfankeji.com

until nc -z localhost 3306; do sleep 1; done
来源：http://mzu.mhx1999.top

[R73] 分割大日志
来源：http://crj.hnxiangtu.top

split -l 1000 big.log part_
来源：http://dde.sxryk.cn

[R74] 批量重命名
来源：http://dpn.andypj.xyz

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://rly.jianghu66.top

[R75] 导出环境变量
来源：http://ogh.chenzaomai.com

export PATH="$HOME/bin:$PATH"
来源：http://uvf.tian-w.cn

[R76] 使用临时文件
来源：http://kfs.nanxuanxn.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://ont.feifeiyinyue.top

[R77] 读取用户输入
来源：http://lqr.ydzc1.top

read -rp "请输入: " ans
来源：http://cph.tianlin.xyz

[R78] 交互式菜单
来源：http://epw.hnxiangtu.top

select opt in a b c; do echo "$opt"; break; done
来源：http://hzx.zhongyouzk.top

[R79] 解析命令行选项
来源：http://srz.zhaomingkeji.xyz

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://vbe.chenzaomai.com

[R80] 查看脚本执行耗时
来源：http://ozy.zycfv.cn

time ./run.sh
来源：http://zyb.sufxvd.cn

================================================================================
来源：http://nxq.cdnleiting.top

S. C / C++ 专题
来源：http://oca.jianghu66.top

================================================================================
来源：http://wea.cqqwz.cn

[S01] C：Hello World
来源：http://ysj.quarkkingdee.top

#include <stdio.h>
来源：http://llo.jinqigufen.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://iku.sxryk.cn

[S02] C：变量与格式化输出
来源：http://paz.jinqigufen.top

int a = 10; printf("%d\n", a);
来源：http://hxh.guowangkeji.top

[S03] C：读入整数
来源：http://yat.yj20258888.top

int x; scanf("%d", &x);
来源：http://ffm.sysykeji.top

[S04] C：字符串复制
来源：http://zsi.sjlbkw.cn

char dst[32]; strcpy(dst, "hi");
来源：http://lqv.hfpthk.cn

[S05] C：字符串长度
来源：http://avl.yuxming.cn

strlen(s)
来源：http://xki.jyoumei.cn

[S06] C：字符串比较
来源：http://qwh.quarkkingdee.top

strcmp(a, b) == 0
来源：http://zuc.shzxlz.cn

[S07] C：数组遍历求和
来源：http://nrf.yonumen.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://aez.fktsv.cn

[S08] C：动态内存分配与释放
来源：http://nbr.gotoacloud.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://lft.hesvh.cn

[S09] C：结构体定义与初始化
来源：http://mrc.pengpengdd.cyou

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://myz.shanyushiyangkeji.top

[S10] C：指针与解引用
来源：http://cut.gogol.net.cn

int *p = &a;  *p = 5;
来源：http://bem.smart0.xyz

[S11] C：逐行读文件
来源：http://qsx.ivvv.top

FILE *f = fopen("a.txt", "r");
来源：http://boc.yfazqb.com

while (fgets(buf, sizeof buf, f)) { }
来源：http://rog.mhx1999.top

fclose(f);
来源：http://ixg.wangshuangyany.cn

[S12] C：写文件
来源：http://amh.tarul.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://btf.jiagoushi.top

[S13] C：宏定义
来源：http://vrj.fzhhl.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://vpt.redwolf501.top

[S14] C：枚举
来源：http://jlj.daxiang520.top

enum Color { RED, GREEN, BLUE };
来源：http://apn.daria6918.cn

[S15] C：类型转换
来源：http://rst.ivvv.top

(double) a / b
来源：http://nhx.gaohongyu789.top

[S16] C：位操作置位
来源：http://qkg.yangfankeji.com

x |= (1 << 3);
来源：http://mbh.hnxiangtu.top

[S17] C：安全拼接字符串
来源：http://fxt.zhijiandao.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://xsx.ctjpmb.com

[S18] C：命令行参数
来源：http://ntl.zhongyouzk.top

int main(int argc, char **argv)
来源：http://drs.mhx1999.top

[S19] C：快速排序
来源：http://tlh.shangyingyoupin.top

qsort(a, n, sizeof(int), cmp);
来源：http://arr.xinyue.icu

[S20] C：二分查找
来源：http://plh.yj20258.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://saz.gotoacloud.top

[S21] C：字符类别判断
来源：http://zfq.zhixingplan.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://xgf.svipenyu.cn

[S22] C：字符串转数字
来源：http://nps.sxryk.cn

atoi("42");  strtod("3.14", NULL);
来源：http://wbi.vehdjk.com

[S23] C：随机数
来源：http://coz.nanxuanxn.top

srand(time(NULL));  int r = rand() % 100;
来源：http://knc.yj202588.top

[S24] C：获取本地时间
来源：http://woo.meibo888.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://spi.dianchejie.cn

[S25] C：内存拷贝
来源：http://pnu.pengpengdd.cyou

memcpy(dst, src, n);
来源：http://djg.gzhubu.top

[S26] C：内存清零
来源：http://btc.jiagoushi.top

memset(a, 0, sizeof a);
来源：http://vye.9152youxi.cn

[S27] C：定义常量
来源：http://ruj.kuanghao11.cn

const double PI = 3.14159;
来源：http://ehq.birdmap.top

[S28] C：静态变量
来源：http://exq.tian-w.cn

static int counter = 0;
来源：http://mlw.wangshuangyany.cn

[S29] C：变参函数
来源：http://hes.gaohongyu789.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://jeb.hcnkem.com

[S30] C：头文件保护
来源：http://gbh.tianlin.xyz

#ifndef X_H
来源：http://xjq.shangyingyoupin.top

#define X_H
来源：http://gre.xingfuxueyuan.xyz

#endif
来源：http://cfp.fehbvm.com

[S31] C++：Hello World
来源：http://lhl.xylfe.cn

#include <iostream>
来源：http://eid.feifeiyinyue.top

int main() { std::cout << "Hello\n"; }
来源：http://mzr.xingfuxueyuan.xyz

[S32] C++：字符串
来源：http://nny.ctjpmb.com

std::string s = "hi";  s += "!";
来源：http://wvf.pengpengdd.cyou

[S33] C++：vector 增删
来源：http://sub.yj20258888.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://ueq.hnxiangtu.top

[S34] C++：遍历 vector
来源：http://hdm.sysykeji.top

for (auto &x : v) { std::cout << x; }
来源：http://iqy.zhongyouzk.top

[S35] C++：map
来源：http://jbo.cucudq.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://qcl.guannengcc.top

[S36] C++：unordered_map
来源：http://rfq.shzxlz.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://knb.yueranfly.top

[S37] C++：set
来源：http://ihr.yj20258.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://usp.vqdsnc.cn

[S38] C++：排序
来源：http://xpj.nanxuanxn.top

std::sort(v.begin(), v.end());
来源：http://aza.tanke756.top

[S39] C++：自定义比较器排序
来源：http://rgy.cucudq.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://bun.xziqi.cn

[S40] C++：查找元素
来源：http://nqo.ywan-chungtsiang.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://daj.chenzaomai.com

[S41] C++：类与构造函数
来源：http://xrj.yanxiufei.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://mwn.cucudq.cn

[S42] C++：继承与虚函数
来源：http://rcr.sjlbkw.cn

class B : public Base { public: void f() override {} };
来源：http://cdt.aibaodan.cn

[S43] C++：智能指针
来源：http://flx.zhaomingkeji.xyz

auto p = std::make_unique<int>(5);
来源：http://hpr.zdbjq.cn

[S44] C++：引用传参
来源：http://vfp.0kj1m.cn

void inc(int &x) { ++x; }
来源：http://ujw.jqgufenzy.top

[S45] C++：lambda
来源：http://vuq.zhengqikj.top

auto add = [](int a, int b) { return a + b; };
来源：http://uqm.xinyue.icu

[S46] C++：函数模板
来源：http://few.redwolf501.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://eps.xziqi.cn

[S47] C++：结构化绑定遍历
来源：http://ium.birdmap.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://biu.nwbrower.top

[S48] C++：逐行读文件
来源：http://bbm.havefunace.top

std::ifstream in("a.txt");  std::string line;
来源：http://amo.daria6918.cn

while (std::getline(in, line)) { }
来源：http://kgs.hnqzz.top

[S49] C++：写文件
来源：http://woh.yj20258888.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://dxd.cheryme.top

[S50] C++：格式化数字
来源：http://bfr.xinyue.icu

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hsa.cheryme.top

[S51] C++：显式类型转换
来源：http://lvb.yuanzhike.top

static_cast<double>(a) / b
来源：http://wnk.daxiang520.top

[S52] C++：const 与 noexcept
来源：http://ocw.shzxlz.cn

int size() const noexcept { return n_; }
来源：http://hra.gotoacloud.top

[S53] C++：移动语义
来源：http://fps.xylfe.cn

std::vector<int> w = std::move(v);
来源：http://egl.yvedp.cn

[S54] C++：异常处理
来源：http://atc.shangyingyoupin.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://new.nanxinkj.top

[S55] C++：结构化绑定
来源：http://fbp.cdnleiting.top

auto [a, b] = std::make_pair(1, 2);
来源：http://ldx.aizwys.cn

[S56] C++：optional
来源：http://evb.jqgufenzy.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://jwg.sysykeji.top

[S57] C++：编译期常量
来源：http://qey.cheryme.top

constexpr int N = 10;
来源：http://odb.yonumen.top

[S58] C++：命名空间
来源：http://jus.zdqjudy.top

namespace ns { int f() { return 1; } }
来源：http://yzx.chenjidiqi.icu

[S59] C++：静态断言
来源：http://xeb.cashguo.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://lvq.havefunace.top

[S60] C++：遍历并删除元素
来源：http://apa.cucudq.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://coq.xylfe.cn

================================================================================
来源：http://uuj.yonumen.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://icc.haohaochexian.top

================================================================================
来源：http://rkz.shuidangran.top

[T01] Kotlin：Hello World
来源：http://kjx.yj202588.top

println("Hello")
来源：http://vrw.guannengcc.top

[T02] Kotlin：变量
来源：http://tem.hcnkem.com

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://oyv.xingfuxueyuan.xyz

[T03] Kotlin：字符串模板
来源：http://vef.yvedp.cn

"值: $b"
来源：http://jmj.cucudq.cn

[T04] Kotlin：空安全
来源：http://ged.xziqi.cn

val n: String? = null;  n?.length
来源：http://ykj.guowangkeji.top

[T05] Kotlin：when 表达式
来源：http://czn.ctjpmb.com

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://yuj.zhengqikj.top

[T06] Kotlin：集合映射
来源：http://jxm.gotoacloud.top

listOf(1, 2, 3).map { it * 2 }
来源：http://ubj.xuanzx.com

[T07] Kotlin：集合过滤
来源：http://uwi.nwbrower.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://imm.zhengqikj.top

[T08] Kotlin：数据类
来源：http://icy.xuanzx.com

data class User(val name: String, val age: Int)
来源：http://ppr.sjlbkw.cn

[T09] Kotlin：扩展函数
来源：http://hep.hysaishi.cn

fun String.exclaim() = this + "!"
来源：http://wia.cucudq.cn

[T10] Kotlin：默认参数
来源：http://fcr.zhaomingkeji.xyz

fun greet(name: String = "World") = "Hi $name"
来源：http://cjt.havefunace.top

[T11] Kotlin：协程
来源：http://wen.yj20258888.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://eun.nwbrower.top

[T12] Kotlin：解构声明
来源：http://kyk.sweek.top

val (a, b) = Pair(1, 2)
来源：http://dnn.zhijiandao.cn

[T13] Kotlin：只读 Map
来源：http://lvx.zhixingplan.top

val m = mapOf("a" to 1)
来源：http://kcs.cucudq.cn

[T14] Kotlin：循环
来源：http://ndg.hongshengwenyu.top

for (i in 1..10) println(i)
来源：http://kcp.fanxiaobao.xyz

[T15] Kotlin：接口
来源：http://hlf.mhx1999.top

interface Shape { fun area(): Double }
来源：http://ney.yangfankeji.com

[T16] Swift：Hello World
来源：http://hqw.yj20258.top

print("Hello")
来源：http://gau.cucudq.cn

[T17] Swift：变量与常量
来源：http://scy.guowangkeji.top

var a = 1;  let b = 2
来源：http://xuo.epnwcf.com

[T18] Swift：字符串插值
来源：http://hvr.xziqi.cn

"值: \(b)"
来源：http://uzp.fengsongda.top

[T19] Swift：可选绑定
来源：http://qdh.ivvv.top

if let n = opt { print(n) }
来源：http://lyo.vqdsnc.cn

[T20] Swift：数组操作
来源：http://rht.fktsv.cn

var a = [1, 2, 3];  a.append(4)
来源：http://ian.hnxiangtu.top

[T21] Swift：遍历
来源：http://dyl.gaohongyu789.top

for x in a { print(x) }
来源：http://ixz.9152youxi.cn

[T22] Swift：字典
来源：http://mtm.hfpthk.cn

var d = ["a": 1];  d["b"] = 2
来源：http://xqp.snrcjt.cn

[T23] Swift：函数
来源：http://oqz.hesvh.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://dys.nwbrower.top

[T24] Swift：闭包
来源：http://oql.birdmap.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://cyq.cheryme.top

[T25] Swift：结构体
来源：http://ifp.gaohongyu789.top

struct P { var x: Int }
来源：http://pdw.gogol.net.cn

[T26] Swift：类与重写
来源：http://zmt.ywan-chungtsiang.top

class A: Base { override func f() {} }
来源：http://smm.tianlin.xyz

[T27] Swift：错误处理
来源：http://fbb.chenjidiqi.icu

do { try f() } catch { print(error) }
来源：http://znf.redwolf501.top

[T28] Swift：枚举
来源：http://kmp.ydjk.org.cn

enum Color { case red, green }
来源：http://oog.shangyingyoupin.top

[T29] Swift：guard 提前返回
来源：http://vds.hnxiangtu.top

guard let x = opt else { return }
来源：http://fvm.cheryme.top

[T30] Swift：协议
来源：http://mxx.zdbjq.cn

protocol Shape { func area() -> Double }
来源：http://ypu.yongpay.top

[T31] Lua：Hello World
来源：http://clg.quarkkingdee.top

print("Hello")
来源：http://ftp.jinqigfzy.top

[T32] Lua：局部变量
来源：http://nvj.xuetiantiany.cn

local a = 1
来源：http://tse.gotoacloud.top

[T33] Lua：表（数组）
来源：http://kho.sysykeji.top

local t = {1, 2, 3};  t[4] = 4
来源：http://tzf.ywan-chungtsiang.top

[T34] Lua：遍历表
来源：http://mtw.zdqjudy.top

for i, v in ipairs(t) do print(i, v) end
来源：http://edl.zdqjudy.top

[T35] Lua：字典表
来源：http://ybr.xylfe.cn

local d = { a = 1 };  d.b = 2
来源：http://ukg.feifeiyinyue.top

[T36] Lua：函数
来源：http://afh.xingfuxueyuan.xyz

function add(a, b) return a + b end
来源：http://hmv.dashuyun.cn

[T37] Lua：字符串拼接
来源：http://sos.bbcook.cn

"a" .. "b"
来源：http://hzy.zhongyouzk.top

[T38] Lua：条件
来源：http://wsm.zhixingplan.top

if x > 0 then print("正") end
来源：http://aey.bbcook.cn

[T39] Lua：模式匹配
来源：http://aul.pengpengdd.cyou

string.find(s, "%d+")
来源：http://fxc.zhijiandao.cn

[T40] Lua：元表
来源：http://cdz.gotoacloud.top

setmetatable({}, { __index = base })
来源：http://qjb.hysaishi.cn

[T41] Perl：Hello World
来源：http://blr.fengsongda.top

print "Hello\n";
来源：http://kmp.vehdjk.com

[T42] Perl：变量类型
来源：http://hoh.cucudq.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://amh.jqgufenzy.top

[T43] Perl：字符串插值
来源：http://pob.tian-w.cn

"值: $a"
来源：http://bah.cqqwz.cn

[T44] Perl：条件
来源：http://nzn.feifeiyinyue.top

if ($a > 0) { print "正"; }
来源：http://vjv.birdmap.top

[T45] Perl：数组遍历
来源：http://axg.chenjidiqi.icu

for my $x (@arr) { print $x; }
来源：http://ugn.yj202588.top

[T46] Perl：哈希操作
来源：http://lxy.shuidangran.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://ctv.vqdsnc.cn

[T47] Perl：正则捕获
来源：http://emt.sufxvd.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://btl.nanxinkj.top

[T48] Perl：正则替换
来源：http://fzv.zdbjq.cn

$s =~ s/old/new/g;
来源：http://ffx.sjlbkw.cn

[T49] Perl：函数
来源：http://hqv.wangdashe.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://fud.zdbjq.cn

[T50] Perl：逐行读文件
来源：http://ofg.9152youxi.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://fow.316326.xyz

while (my $line = <$fh>) { print $line; }
来源：http://rgn.uphjek.com

[T51] Scala：Hello World
来源：http://ceh.xuetiantiany.cn

println("Hello")
来源：http://cyp.cucudq.cn

[T52] Scala：变量
来源：http://vmk.sysykeji.top

val a = 1;  var b = 2
来源：http://btt.shangyingyoupin.top

[T53] Scala：字符串插值
来源：http://ldn.hnxiangtu.top

s"值: $b"
来源：http://bsr.9152youxi.cn

[T54] Scala：集合映射
来源：http://acd.tian-w.cn

List(1, 2, 3).map(_ * 2)
来源：http://jzo.9152youxi.cn

[T55] Scala：集合过滤
来源：http://mwf.epnwcf.com

List(1, 2, 3).filter(_ > 1)
来源：http://aco.pengpengdd.cyou

[T56] Scala：样例类
来源：http://bhy.bjfxy.top

case class User(name: String, age: Int)
来源：http://irf.jlsjyb.cn

[T57] Scala：模式匹配
来源：http://bbr.sufxvd.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://pux.nanxinkj.top

[T58] Scala：函数定义
来源：http://lql.zhaomingkeji.xyz

def add(a: Int, b: Int): Int = a + b
来源：http://iju.aibaodan.cn

[T59] Scala：循环
来源：http://lpv.sjlbkw.cn

for (i <- 1 to 10) println(i)
来源：http://lon.birdmap.top

[T60] Scala：折叠
来源：http://dbd.yongpay.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://bly.fengsongda.top

================================================================================
来源：http://dww.uphjek.com

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://prq.jlsjyb.cn

================================================================================
来源：http://cib.zdbjq.cn

[U01] Py：创建虚拟环境
来源：http://uwc.ivvv.top

python -m venv .venv && source .venv/bin/activate
来源：http://ghy.shanyushiyangkeji.top

[U02] Py：导出 / 安装依赖
来源：http://igx.bjfxy.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://vgo.gotoacloud.top

[U03] Py：加载 .env 配置
来源：http://vco.9152youxi.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://ctr.ehwqpu.com

[U04] Py：变量调试打印
来源：http://obg.svipenyu.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://wrg.daria6918.cn

[U05] Py：列表去重且保序
来源：http://tsl.hongshengwenyu.top

list(dict.fromkeys(arr))
来源：http://lbe.zhixingplan.top

[U06] Py：合并两个字典
来源：http://rhn.pycfn.com

{**a, **b}
来源：http://zuq.cqqwz.cn

[U07] Py：反转字典键值
来源：http://srt.tarul.cn

{v: k for k, v in d.items()}
来源：http://tez.feifeiyinyue.top

[U08] Py：展平二维列表
来源：http://qti.guannengcc.top

[y for x in nested for y in x]
来源：http://dwb.fengsongda.top


<!-- 参考信息 -->