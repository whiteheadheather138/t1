代发 wailian999

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://rgm.9152youxi.cn

[R66] 定时任务
来源：http://sdc.chenlongwang.top

crontab -e;  crontab -l
来源：http://ilz.hfpthk.cn

[R67] 生成随机十六进制串
来源：http://dpa.zhiwuduotai.top

openssl rand -hex 16
来源：http://cyq.vqdsnc.cn

[R68] 计算文件校验值
来源：http://kqd.cqqwz.cn

sha256sum a.txt;  md5sum a.txt
来源：http://chy.feifeiyinyue.top

[R69] 生成随机密码
来源：http://umh.yj202588.top

head -c 16 /dev/urandom | base64
来源：http://dii.snrcjt.cn

[R70] 时间戳与互转
来源：http://zxb.guowangkeji.top

date +%s;  date -d @1700000000
来源：http://mrc.shzxlz.cn

[R71] 日期格式化
来源：http://zuf.cucudq.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://gfx.ctjpmb.com

[R72] 等待端口就绪
来源：http://imr.ydjk.org.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://xhk.snrcjt.cn

[R73] 分割大日志
来源：http://rhb.xuetiantiany.cn

split -l 1000 big.log part_
来源：http://wev.jinqigfzy.top

[R74] 批量重命名
来源：http://aav.52xcode.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://ahw.yangfankeji.com

[R75] 导出环境变量
来源：http://bgk.uphjek.com

export PATH="$HOME/bin:$PATH"
来源：http://aou.sufxvd.cn

[R76] 使用临时文件
来源：http://rbl.guannengcc.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://xbf.fzhhl.top

[R77] 读取用户输入
来源：http://ghm.yvedp.cn

read -rp "请输入: " ans
来源：http://amz.hcnkem.com

[R78] 交互式菜单
来源：http://gmt.hcnkem.com

select opt in a b c; do echo "$opt"; break; done
来源：http://jqp.yj202588.top

[R79] 解析命令行选项
来源：http://zzp.hnqzz.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://aqd.xuetiantiany.cn

[R80] 查看脚本执行耗时
来源：http://jvo.dianchejie.cn

time ./run.sh
来源：http://ffi.gaohongyu789.top

================================================================================
来源：http://inw.gzhubu.top

S. C / C++ 专题
来源：http://aug.ywan-chungtsiang.top

================================================================================
来源：http://ixh.xingfuxueyuan.xyz

[S01] C：Hello World
来源：http://ezi.shanyushiyangtech.top

#include <stdio.h>
来源：http://wsx.jyoumei.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://ljg.sufxvd.cn

[S02] C：变量与格式化输出
来源：http://lgf.nwbrower.top

int a = 10; printf("%d\n", a);
来源：http://tgi.yangfankeji.com

[S03] C：读入整数
来源：http://cnt.iojbl.cn

int x; scanf("%d", &x);
来源：http://riv.gotoacloud.top

[S04] C：字符串复制
来源：http://uvb.fengsongda.top

char dst[32]; strcpy(dst, "hi");
来源：http://kpx.ydjk.org.cn

[S05] C：字符串长度
来源：http://gwj.zhengqikj.top

strlen(s)
来源：http://suq.jqgfzy.top

[S06] C：字符串比较
来源：http://tih.hywenlv.cn

strcmp(a, b) == 0
来源：http://ziu.cdnleiting.top

[S07] C：数组遍历求和
来源：http://qnw.haohaochexian.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://sso.birdmap.top

[S08] C：动态内存分配与释放
来源：http://hpd.tian-w.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://bgu.sjlbkw.cn

[S09] C：结构体定义与初始化
来源：http://qop.jiagoushi.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://kot.smart0.xyz

[S10] C：指针与解引用
来源：http://ubt.bjfxy.top

int *p = &a;  *p = 5;
来源：http://hxp.mhx1999.top

[S11] C：逐行读文件
来源：http://cjq.dashuyun.cn

FILE *f = fopen("a.txt", "r");
来源：http://ekx.dashuyun.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://eol.pycfn.com

fclose(f);
来源：http://kvq.ctjpmb.com

[S12] C：写文件
来源：http://ugo.fktsv.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://pdk.bbcook.cn

[S13] C：宏定义
来源：http://pkf.zhiwuduotai.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://zav.svipenyu.cn

[S14] C：枚举
来源：http://qwd.sjlbkw.cn

enum Color { RED, GREEN, BLUE };
来源：http://qzk.guowangkeji.top

[S15] C：类型转换
来源：http://wim.fehbvm.com

(double) a / b
来源：http://ccs.jinqigufen.top

[S16] C：位操作置位
来源：http://rwn.wangshuangyany.cn

x |= (1 << 3);
来源：http://aic.ywan-chungtsiang.top

[S17] C：安全拼接字符串
来源：http://gin.pycfn.com

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://mur.zhongyouzk.top

[S18] C：命令行参数
来源：http://xxi.ydjk.org.cn

int main(int argc, char **argv)
来源：http://lch.pycfn.com

[S19] C：快速排序
来源：http://zpz.ctjpmb.com

qsort(a, n, sizeof(int), cmp);
来源：http://mds.cheryme.top

[S20] C：二分查找
来源：http://bsr.havefunace.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://bgs.316326.xyz

[S21] C：字符类别判断
来源：http://pvg.ivvv.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://qpp.gzhubu.top

[S22] C：字符串转数字
来源：http://jed.xuanzx.com

atoi("42");  strtod("3.14", NULL);
来源：http://zcc.kuanghao11.cn

[S23] C：随机数
来源：http://vht.shanyushiyangkeji.top

srand(time(NULL));  int r = rand() % 100;
来源：http://yns.sxryk.cn

[S24] C：获取本地时间
来源：http://qyg.c1oappe.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://ctp.c1oappe.top

[S25] C：内存拷贝
来源：http://wff.gzhubu.top

memcpy(dst, src, n);
来源：http://wzc.daxiang520.top

[S26] C：内存清零
来源：http://iqs.redwolf501.top

memset(a, 0, sizeof a);
来源：http://rzk.sjlbkw.cn

[S27] C：定义常量
来源：http://yiz.tianlin.xyz

const double PI = 3.14159;
来源：http://vet.yfazqb.com

[S28] C：静态变量
来源：http://itm.yj20258.top

static int counter = 0;
来源：http://zbg.pengpengdd.cyou

[S29] C：变参函数
来源：http://nqj.ivvv.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wwn.birdmap.top

[S30] C：头文件保护
来源：http://wyk.kuanghao11.cn

#ifndef X_H
来源：http://gew.gaohongyu789.top

#define X_H
来源：http://nsk.ctjpmb.com

#endif
来源：http://ekz.ybcxt.top

[S31] C++：Hello World
来源：http://vwt.guannengcc.top

#include <iostream>
来源：http://lbr.jiagoushi.top

int main() { std::cout << "Hello\n"; }
来源：http://tlz.xuetiantiany.cn

[S32] C++：字符串
来源：http://qbk.hfpthk.cn

std::string s = "hi";  s += "!";
来源：http://gwk.hnxiangtu.top

[S33] C++：vector 增删
来源：http://umd.hnxiangtu.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://ndr.jinghuilouyu.cn

[S34] C++：遍历 vector
来源：http://xwu.sweek.top

for (auto &x : v) { std::cout << x; }
来源：http://icy.gogol.net.cn

[S35] C++：map
来源：http://pmp.sysykeji.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://utu.9152youxi.cn

[S36] C++：unordered_map
来源：http://xrf.shanyushiyangkeji.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://nce.ivvv.top

[S37] C++：set
来源：http://mvz.yj202588.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://zld.bbcook.cn

[S38] C++：排序
来源：http://veg.xinyue.icu

std::sort(v.begin(), v.end());
来源：http://cnn.feifeiyinyue.top

[S39] C++：自定义比较器排序
来源：http://aki.pengpengdd.cyou

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://kfv.ctjpmb.com

[S40] C++：查找元素
来源：http://qxq.fehbvm.com

auto it = std::find(v.begin(), v.end(), 3);
来源：http://mvs.zhaomingkeji.xyz

[S41] C++：类与构造函数
来源：http://jhh.xylfe.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://nev.quarkkingdee.top

[S42] C++：继承与虚函数
来源：http://hne.gogol.net.cn

class B : public Base { public: void f() override {} };
来源：http://las.havefunace.top

[S43] C++：智能指针
来源：http://gho.yj202588.top

auto p = std::make_unique<int>(5);
来源：http://gwe.gaohongyu789.top

[S44] C++：引用传参
来源：http://hbs.cheryme.top

void inc(int &x) { ++x; }
来源：http://asz.birdmap.top

[S45] C++：lambda
来源：http://ydh.feifeiyinyue.top

auto add = [](int a, int b) { return a + b; };
来源：http://gth.tian-w.cn

[S46] C++：函数模板
来源：http://tbn.svipenyu.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hcw.zhengqikj.top

[S47] C++：结构化绑定遍历
来源：http://pxn.daria6918.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://lbp.zhongyouzk.top

[S48] C++：逐行读文件
来源：http://hux.hesvh.cn

std::ifstream in("a.txt");  std::string line;
来源：http://lbz.jyoumei.cn

while (std::getline(in, line)) { }
来源：http://pyz.xingfuxueyuan.xyz

[S49] C++：写文件
来源：http://khr.aibaodan.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://tcx.xuetiantiany.cn

[S50] C++：格式化数字
来源：http://irs.pycfn.com

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://ojv.andypj.xyz

[S51] C++：显式类型转换
来源：http://gai.shangyingyoupin.top

static_cast<double>(a) / b
来源：http://eaq.birdmap.top

[S52] C++：const 与 noexcept
来源：http://lhh.ybcxt.top

int size() const noexcept { return n_; }
来源：http://wau.guowangkeji.top

[S53] C++：移动语义
来源：http://lsn.snrcjt.cn

std::vector<int> w = std::move(v);
来源：http://gac.yongpay.top

[S54] C++：异常处理
来源：http://kkg.tarul.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://fpc.yueranfly.top

[S55] C++：结构化绑定
来源：http://qvw.uphjek.com

auto [a, b] = std::make_pair(1, 2);
来源：http://gbz.ydzc1.top

[S56] C++：optional
来源：http://bky.shuidangran.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://idj.tanke756.top

[S57] C++：编译期常量
来源：http://tqv.fanxiaobao.xyz

constexpr int N = 10;
来源：http://vht.bjfxy.top

[S58] C++：命名空间
来源：http://ejn.zhiwuduotai.top

namespace ns { int f() { return 1; } }
来源：http://wql.aizwys.cn

[S59] C++：静态断言
来源：http://gxi.52xcode.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hrw.epnwcf.com

[S60] C++：遍历并删除元素
来源：http://xwp.shangyingyoupin.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://nov.shuidangran.top

================================================================================
来源：http://gmu.52xcode.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://lwt.sjlbkw.cn

================================================================================
来源：http://wth.guowangkeji.top

[T01] Kotlin：Hello World
来源：http://ato.cqqwz.cn

println("Hello")
来源：http://uav.redwolf501.top

[T02] Kotlin：变量
来源：http://hxo.zhengqikj.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://cqk.yfazqb.com

[T03] Kotlin：字符串模板
来源：http://sey.sjlbkw.cn

"值: $b"
来源：http://iup.hysaishi.cn

[T04] Kotlin：空安全
来源：http://mhj.gzhubu.top

val n: String? = null;  n?.length
来源：http://wtl.hnxiangtu.top

[T05] Kotlin：when 表达式
来源：http://aji.jlsjyb.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://skb.jinghuilouyu.cn

[T06] Kotlin：集合映射
来源：http://uir.mhx1999.top

listOf(1, 2, 3).map { it * 2 }
来源：http://kwv.daxiang520.top

[T07] Kotlin：集合过滤
来源：http://hmx.sjlbkw.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://ozs.yj20258888.top

[T08] Kotlin：数据类
来源：http://nlf.xuetiantiany.cn

data class User(val name: String, val age: Int)
来源：http://lbz.fktsv.cn

[T09] Kotlin：扩展函数
来源：http://zcq.epnwcf.com

fun String.exclaim() = this + "!"
来源：http://bjl.yfazqb.com

[T10] Kotlin：默认参数
来源：http://vtk.hongshengwenyu.top

fun greet(name: String = "World") = "Hi $name"
来源：http://bqp.sxryk.cn

[T11] Kotlin：协程
来源：http://ezr.jinqigfzy.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://stp.bjfxy.top

[T12] Kotlin：解构声明
来源：http://kqy.tian-w.cn

val (a, b) = Pair(1, 2)
来源：http://bbs.epnwcf.com

[T13] Kotlin：只读 Map
来源：http://hjr.cashguo.top

val m = mapOf("a" to 1)
来源：http://xrg.hongshengwenyu.top

[T14] Kotlin：循环
来源：http://pji.daxiang520.top

for (i in 1..10) println(i)
来源：http://viw.xziqi.cn

[T15] Kotlin：接口
来源：http://phz.dianchejie.cn

interface Shape { fun area(): Double }
来源：http://xwq.cucudq.cn

[T16] Swift：Hello World
来源：http://frh.pengpengdd.cyou

print("Hello")
来源：http://wub.zycfv.cn

[T17] Swift：变量与常量
来源：http://bgy.c1oappe.top

var a = 1;  let b = 2
来源：http://xus.yanxiufei.cn

[T18] Swift：字符串插值
来源：http://iza.zdqjudy.top

"值: \(b)"
来源：http://iwr.cdnleiting.top

[T19] Swift：可选绑定
来源：http://bne.hywenlv.cn

if let n = opt { print(n) }
来源：http://wxw.jyoumei.cn

[T20] Swift：数组操作
来源：http://nmg.xingfuxueyuan.xyz

var a = [1, 2, 3];  a.append(4)
来源：http://jby.chenzaomai.com

[T21] Swift：遍历
来源：http://ekg.ydjk.org.cn

for x in a { print(x) }
来源：http://rln.feifeiyinyue.top

[T22] Swift：字典
来源：http://qga.mhx1999.top

var d = ["a": 1];  d["b"] = 2
来源：http://qxa.chenzaomai.com

[T23] Swift：函数
来源：http://jmq.shangyingyoupin.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://zen.0kj1m.cn

[T24] Swift：闭包
来源：http://wft.jinqigfzy.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://dnf.hcnkem.com

[T25] Swift：结构体
来源：http://vcc.fengsongda.top

struct P { var x: Int }
来源：http://nis.xuanzx.com

[T26] Swift：类与重写
来源：http://qny.yuxming.cn

class A: Base { override func f() {} }
来源：http://zcf.guowangkeji.top

[T27] Swift：错误处理
来源：http://dia.cdnleiting.top

do { try f() } catch { print(error) }
来源：http://oxd.jinyuanbaomall.cn

[T28] Swift：枚举
来源：http://ayo.cheryme.top

enum Color { case red, green }
来源：http://zqv.bbcook.cn

[T29] Swift：guard 提前返回
来源：http://bbb.jqgfzy.top

guard let x = opt else { return }
来源：http://zyv.fehbvm.com

[T30] Swift：协议
来源：http://lfw.hesvh.cn

protocol Shape { func area() -> Double }
来源：http://cme.daria6918.cn

[T31] Lua：Hello World
来源：http://lzb.xylfe.cn

print("Hello")
来源：http://kni.yangfankeji.com

[T32] Lua：局部变量
来源：http://gjr.jianghu66.top

local a = 1
来源：http://qck.hesvh.cn

[T33] Lua：表（数组）
来源：http://tnn.chenlongwang.top

local t = {1, 2, 3};  t[4] = 4
来源：http://ygb.shzxlz.cn

[T34] Lua：遍历表
来源：http://tqe.fanxiaobao.xyz

for i, v in ipairs(t) do print(i, v) end
来源：http://juo.jianghu66.top

[T35] Lua：字典表
来源：http://atj.yj20258888.top

local d = { a = 1 };  d.b = 2
来源：http://kmj.shzxlz.cn

[T36] Lua：函数
来源：http://oco.quarkkingdee.top

function add(a, b) return a + b end
来源：http://aar.zdbjq.cn

[T37] Lua：字符串拼接
来源：http://fvv.aizwys.cn

"a" .. "b"
来源：http://bvy.wangshuangyany.cn

[T38] Lua：条件
来源：http://xzk.gotoacloud.top

if x > 0 then print("正") end
来源：http://gbz.kuanghao11.cn

[T39] Lua：模式匹配
来源：http://ouu.pengpengdd.cyou

string.find(s, "%d+")
来源：http://eqb.shangyingyoupin.top

[T40] Lua：元表
来源：http://ztv.yuxming.cn

setmetatable({}, { __index = base })
来源：http://xov.zhaomingkeji.xyz

[T41] Perl：Hello World
来源：http://oyg.dashuyun.cn

print "Hello\n";
来源：http://yxa.316326.xyz

[T42] Perl：变量类型
来源：http://soq.fanxiaobao.xyz

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://yxv.redwolf501.top

[T43] Perl：字符串插值
来源：http://lix.shuidangran.top

"值: $a"
来源：http://lqr.xziqi.cn

[T44] Perl：条件
来源：http://lee.xziqi.cn

if ($a > 0) { print "正"; }
来源：http://qsa.xziqi.cn

[T45] Perl：数组遍历
来源：http://xxn.smart0.xyz

for my $x (@arr) { print $x; }
来源：http://mjk.gzhubu.top

[T46] Perl：哈希操作
来源：http://dwh.sysykeji.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://jqv.fehbvm.com

[T47] Perl：正则捕获
来源：http://tdu.chenlongwang.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://qzz.fktsv.cn

[T48] Perl：正则替换
来源：http://ofv.nwbrower.top

$s =~ s/old/new/g;
来源：http://kaf.nanxinkj.top

[T49] Perl：函数
来源：http://yyz.zhoulong.xyz

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://kzg.nanxinkj.top

[T50] Perl：逐行读文件
来源：http://klg.zhaomingkeji.xyz

open my $fh, "<", "a.txt" or die $!;
来源：http://umv.jqgufenzy.top

while (my $line = <$fh>) { print $line; }
来源：http://rjc.chenzaomai.com

[T51] Scala：Hello World
来源：http://cnj.jqgfzy.top

println("Hello")
来源：http://rka.zdbjq.cn

[T52] Scala：变量
来源：http://rah.pengpengdd.cyou

val a = 1;  var b = 2
来源：http://kkw.dianchejie.cn

[T53] Scala：字符串插值
来源：http://xot.jyoumei.cn

s"值: $b"
来源：http://kjv.sxryk.cn

[T54] Scala：集合映射
来源：http://jjr.yongpay.top

List(1, 2, 3).map(_ * 2)
来源：http://cql.sjlbkw.cn

[T55] Scala：集合过滤
来源：http://tbo.yfazqb.com

List(1, 2, 3).filter(_ > 1)
来源：http://odx.fktsv.cn

[T56] Scala：样例类
来源：http://hhv.nwbrower.top

case class User(name: String, age: Int)
来源：http://cpp.zycfv.cn

[T57] Scala：模式匹配
来源：http://tvl.fengsongda.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://zha.zdqjudy.top

[T58] Scala：函数定义
来源：http://zvq.jlsjyb.cn

def add(a: Int, b: Int): Int = a + b
来源：http://tvm.haohaochexian.top

[T59] Scala：循环
来源：http://xxp.cucudq.cn

for (i <- 1 to 10) println(i)
来源：http://adq.hysaishi.cn

[T60] Scala：折叠
来源：http://pja.jyoumei.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://kih.xingfuxueyuan.xyz

================================================================================
来源：http://buz.yfazqb.com

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://ukl.hysaishi.cn

================================================================================
来源：http://obz.hysaishi.cn

[U01] Py：创建虚拟环境
来源：http://wca.yonumen.top

python -m venv .venv && source .venv/bin/activate
来源：http://zqm.hesvh.cn

[U02] Py：导出 / 安装依赖
来源：http://prk.shuidangran.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://umm.jinqigufen.top

[U03] Py：加载 .env 配置
来源：http://krz.guannengcc.top

from dotenv import load_dotenv; load_dotenv()
来源：http://psr.ywan-chungtsiang.top

[U04] Py：变量调试打印
来源：http://ldp.sweek.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://gnf.epnwcf.com

[U05] Py：列表去重且保序
来源：http://edd.shanyushiyangkeji.top

list(dict.fromkeys(arr))
来源：http://jkp.jinyuanbaomall.cn

[U06] Py：合并两个字典
来源：http://fkb.haohaochexian.top

{**a, **b}
来源：http://kff.cashguo.top


<!-- 参考信息 -->