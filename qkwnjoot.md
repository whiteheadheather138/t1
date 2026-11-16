代发 wailian999

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://ovj.daria6918.cn

[R66] 定时任务
来源：http://syj.haohaochexian.top

crontab -e;  crontab -l
来源：http://nff.jqgfzy.top

[R67] 生成随机十六进制串
来源：http://hrd.yanxiufei.cn

openssl rand -hex 16
来源：http://kpn.yangfankeji.com

[R68] 计算文件校验值
来源：http://eoi.vehdjk.com

sha256sum a.txt;  md5sum a.txt
来源：http://wsh.snrcjt.cn

[R69] 生成随机密码
来源：http://ifl.316326.xyz

head -c 16 /dev/urandom | base64
来源：http://gqa.hysaishi.cn

[R70] 时间戳与互转
来源：http://shf.zhijiandao.cn

date +%s;  date -d @1700000000
来源：http://wbz.52xcode.cn

[R71] 日期格式化
来源：http://pgi.bbcook.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://cml.yanxiufei.cn

[R72] 等待端口就绪
来源：http://suv.meibo888.top

until nc -z localhost 3306; do sleep 1; done
来源：http://lhy.chenjidiqi.icu

[R73] 分割大日志
来源：http://azk.zycfv.cn

split -l 1000 big.log part_
来源：http://cfz.hywenlv.cn

[R74] 批量重命名
来源：http://tum.gzhubu.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://xnh.ydzc1.top

[R75] 导出环境变量
来源：http://rnz.yfazqb.com

export PATH="$HOME/bin:$PATH"
来源：http://tyh.hammf.cn

[R76] 使用临时文件
来源：http://aim.smart0.xyz

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://vwd.shanyushiyangkeji.top

[R77] 读取用户输入
来源：http://qqs.ppjwa.cn

read -rp "请输入: " ans
来源：http://nze.zhengqikj.top

[R78] 交互式菜单
来源：http://yvd.gotoacloud.top

select opt in a b c; do echo "$opt"; break; done
来源：http://swr.zhiwuduotai.top

[R79] 解析命令行选项
来源：http://zrl.xuanzx.com

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mmf.chenzaomai.com

[R80] 查看脚本执行耗时
来源：http://bkf.jinyuanbaomall.cn

time ./run.sh
来源：http://lhg.zdbjq.cn

================================================================================
来源：http://xef.yangfankeji.com

S. C / C++ 专题
来源：http://ahu.svipenyu.cn

================================================================================
来源：http://loo.mhx1999.top

[S01] C：Hello World
来源：http://kdr.ivvv.top

#include <stdio.h>
来源：http://icm.cheryme.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://rqb.fktsv.cn

[S02] C：变量与格式化输出
来源：http://ckb.xuanzx.com

int a = 10; printf("%d\n", a);
来源：http://ezp.shuidangran.top

[S03] C：读入整数
来源：http://nsr.ybcxt.top

int x; scanf("%d", &x);
来源：http://pli.ppjwa.cn

[S04] C：字符串复制
来源：http://jsn.ivvv.top

char dst[32]; strcpy(dst, "hi");
来源：http://bzk.andypj.xyz

[S05] C：字符串长度
来源：http://kcu.9152youxi.cn

strlen(s)
来源：http://dmp.chenlongwang.top

[S06] C：字符串比较
来源：http://sdu.ivvv.top

strcmp(a, b) == 0
来源：http://jnf.zhoulong.xyz

[S07] C：数组遍历求和
来源：http://rxc.yj20258888.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://wct.cucudq.cn

[S08] C：动态内存分配与释放
来源：http://sho.xuanzx.com

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://qgr.sufxvd.cn

[S09] C：结构体定义与初始化
来源：http://ekf.nwbrower.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mwa.wangshuangyany.cn

[S10] C：指针与解引用
来源：http://iwt.hnxiangtu.top

int *p = &a;  *p = 5;
来源：http://dvz.quarkkingdee.top

[S11] C：逐行读文件
来源：http://fvo.hesvh.cn

FILE *f = fopen("a.txt", "r");
来源：http://ftk.cucudq.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://juc.xuetiantiany.cn

fclose(f);
来源：http://doh.aibaodan.cn

[S12] C：写文件
来源：http://jqj.gzhubu.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://umo.cucudq.cn

[S13] C：宏定义
来源：http://tjg.nwbrower.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://ntc.iojbl.cn

[S14] C：枚举
来源：http://pgl.hcnkem.com

enum Color { RED, GREEN, BLUE };
来源：http://tys.iojbl.cn

[S15] C：类型转换
来源：http://hau.yfazqb.com

(double) a / b
来源：http://iyp.xylfe.cn

[S16] C：位操作置位
来源：http://vhk.daria6918.cn

x |= (1 << 3);
来源：http://pjf.wangdashe.top

[S17] C：安全拼接字符串
来源：http://ics.ctjpmb.com

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://nvl.guannengcc.top

[S18] C：命令行参数
来源：http://wdh.svipenyu.cn

int main(int argc, char **argv)
来源：http://xnz.jlsjyb.cn

[S19] C：快速排序
来源：http://wwa.zdbjq.cn

qsort(a, n, sizeof(int), cmp);
来源：http://cok.chenlongwang.top

[S20] C：二分查找
来源：http://jwu.sjlbkw.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://cuz.fengsongda.top

[S21] C：字符类别判断
来源：http://ypa.hysaishi.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://pee.gaohongyu789.top

[S22] C：字符串转数字
来源：http://dcq.jinyuanbaomall.cn

atoi("42");  strtod("3.14", NULL);
来源：http://tyn.cucudq.cn

[S23] C：随机数
来源：http://vrn.shzxlz.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://pym.ywan-chungtsiang.top

[S24] C：获取本地时间
来源：http://kxy.yj20258.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://qyc.tianlin.xyz

[S25] C：内存拷贝
来源：http://mzl.chenzaomai.com

memcpy(dst, src, n);
来源：http://xuz.yvedp.cn

[S26] C：内存清零
来源：http://nne.jqgufenzy.top

memset(a, 0, sizeof a);
来源：http://xgw.vehdjk.com

[S27] C：定义常量
来源：http://mjn.zycfv.cn

const double PI = 3.14159;
来源：http://xlv.nanxuanxn.top

[S28] C：静态变量
来源：http://dvd.cheryme.top

static int counter = 0;
来源：http://vpa.xingfuxueyuan.xyz

[S29] C：变参函数
来源：http://iad.fzhhl.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://adm.yj20258.top

[S30] C：头文件保护
来源：http://qvj.zhoulong.xyz

#ifndef X_H
来源：http://zki.zdqjudy.top

#define X_H
来源：http://ncy.c1oappe.top

#endif
来源：http://rwv.xinyue.icu

[S31] C++：Hello World
来源：http://qkg.ppjwa.cn

#include <iostream>
来源：http://xvt.jinqigfzy.top

int main() { std::cout << "Hello\n"; }
来源：http://tcs.cashguo.top

[S32] C++：字符串
来源：http://hem.chenzaomai.com

std::string s = "hi";  s += "!";
来源：http://uae.cashguo.top

[S33] C++：vector 增删
来源：http://bak.ydjk.org.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://znk.yvedp.cn

[S34] C++：遍历 vector
来源：http://nxa.uphjek.com

for (auto &x : v) { std::cout << x; }
来源：http://wns.hywenlv.cn

[S35] C++：map
来源：http://zbv.shuidangran.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://chd.dashuyun.cn

[S36] C++：unordered_map
来源：http://gkm.tarul.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://nto.shanyushiyangtech.top

[S37] C++：set
来源：http://nlm.shangyingyoupin.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://jxj.chenzaomai.com

[S38] C++：排序
来源：http://thi.aibaodan.cn

std::sort(v.begin(), v.end());
来源：http://bnk.316326.xyz

[S39] C++：自定义比较器排序
来源：http://tuh.zhongyouzk.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://fja.kuanghao11.cn

[S40] C++：查找元素
来源：http://vpl.gzhubu.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://yib.daria6918.cn

[S41] C++：类与构造函数
来源：http://yds.zycfv.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://chg.pengpengdd.cyou

[S42] C++：继承与虚函数
来源：http://jrq.yanxiufei.cn

class B : public Base { public: void f() override {} };
来源：http://imy.tarul.cn

[S43] C++：智能指针
来源：http://hax.yvedp.cn

auto p = std::make_unique<int>(5);
来源：http://vlc.tanke756.top

[S44] C++：引用传参
来源：http://fvs.cqqwz.cn

void inc(int &x) { ++x; }
来源：http://xyi.316326.xyz

[S45] C++：lambda
来源：http://fig.fanxiaobao.xyz

auto add = [](int a, int b) { return a + b; };
来源：http://ugb.yj20258.top

[S46] C++：函数模板
来源：http://omo.mhx1999.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://xtx.jinghuilouyu.cn

[S47] C++：结构化绑定遍历
来源：http://ekd.shuidangran.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://mow.sweek.top

[S48] C++：逐行读文件
来源：http://gqf.cucudq.cn

std::ifstream in("a.txt");  std::string line;
来源：http://nnw.ctjpmb.com

while (std::getline(in, line)) { }
来源：http://bgj.hcnkem.com

[S49] C++：写文件
来源：http://ipk.ctjpmb.com

std::ofstream out("a.txt");  out << "hi\n";
来源：http://mdo.ybcxt.top

[S50] C++：格式化数字
来源：http://spw.fengsongda.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://lbt.cqqwz.cn

[S51] C++：显式类型转换
来源：http://ibl.fengsongda.top

static_cast<double>(a) / b
来源：http://wue.havefunace.top

[S52] C++：const 与 noexcept
来源：http://lan.cucudq.cn

int size() const noexcept { return n_; }
来源：http://jxs.ehwqpu.com

[S53] C++：移动语义
来源：http://drt.guowangkeji.top

std::vector<int> w = std::move(v);
来源：http://tju.dashuyun.cn

[S54] C++：异常处理
来源：http://vnk.hysaishi.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://lcr.0kj1m.cn

[S55] C++：结构化绑定
来源：http://gbk.sxryk.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://ivb.nanxinkj.top

[S56] C++：optional
来源：http://hfx.zhiwuduotai.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://bnt.iojbl.cn

[S57] C++：编译期常量
来源：http://gfd.kuanghao11.cn

constexpr int N = 10;
来源：http://zvk.daxiang520.top

[S58] C++：命名空间
来源：http://zcu.iojbl.cn

namespace ns { int f() { return 1; } }
来源：http://pvi.kuanghao11.cn

[S59] C++：静态断言
来源：http://tmh.ppjwa.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://qcp.jyoumei.cn

[S60] C++：遍历并删除元素
来源：http://toi.c1oappe.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://rct.hammf.cn

================================================================================
来源：http://poe.yj202588.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://kdc.xuanzx.com

================================================================================
来源：http://fck.cdnleiting.top

[T01] Kotlin：Hello World
来源：http://mws.guannengcc.top

println("Hello")
来源：http://sxb.nanxuanxn.top

[T02] Kotlin：变量
来源：http://rwe.jlsjyb.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://vng.nanxuanxn.top

[T03] Kotlin：字符串模板
来源：http://poq.aibaodan.cn

"值: $b"
来源：http://who.zycfv.cn

[T04] Kotlin：空安全
来源：http://uql.zdbjq.cn

val n: String? = null;  n?.length
来源：http://nas.yangfankeji.com

[T05] Kotlin：when 表达式
来源：http://rfx.tianlin.xyz

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hce.hammf.cn

[T06] Kotlin：集合映射
来源：http://abw.yvedp.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://sbp.yj202588.top

[T07] Kotlin：集合过滤
来源：http://adq.ppjwa.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://aip.c1oappe.top

[T08] Kotlin：数据类
来源：http://gap.yangfankeji.com

data class User(val name: String, val age: Int)
来源：http://rxq.yangfankeji.com

[T09] Kotlin：扩展函数
来源：http://tiu.birdmap.top

fun String.exclaim() = this + "!"
来源：http://ztp.svipenyu.cn

[T10] Kotlin：默认参数
来源：http://hsr.shuidangran.top

fun greet(name: String = "World") = "Hi $name"
来源：http://ocd.gzhubu.top

[T11] Kotlin：协程
来源：http://gha.shuidangran.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://rqw.shuidangran.top

[T12] Kotlin：解构声明
来源：http://syf.zycfv.cn

val (a, b) = Pair(1, 2)
来源：http://grk.wangdashe.top

[T13] Kotlin：只读 Map
来源：http://igl.yonumen.top

val m = mapOf("a" to 1)
来源：http://qsf.zhiwuduotai.top

[T14] Kotlin：循环
来源：http://fme.cashguo.top

for (i in 1..10) println(i)
来源：http://naz.cheryme.top

[T15] Kotlin：接口
来源：http://szn.ehwqpu.com

interface Shape { fun area(): Double }
来源：http://nms.yonumen.top

[T16] Swift：Hello World
来源：http://ixa.snrcjt.cn

print("Hello")
来源：http://hlu.yangfankeji.com

[T17] Swift：变量与常量
来源：http://llj.fanxiaobao.xyz

var a = 1;  let b = 2
来源：http://nki.cqqwz.cn

[T18] Swift：字符串插值
来源：http://zph.guannengcc.top

"值: \(b)"
来源：http://gsi.xziqi.cn

[T19] Swift：可选绑定
来源：http://ioh.zhaomingkeji.xyz

if let n = opt { print(n) }
来源：http://kej.nwbrower.top

[T20] Swift：数组操作
来源：http://tsx.bbcook.cn

var a = [1, 2, 3];  a.append(4)
来源：http://pka.gotoacloud.top

[T21] Swift：遍历
来源：http://vrg.shanyushiyangkeji.top

for x in a { print(x) }
来源：http://kwz.fzhhl.top

[T22] Swift：字典
来源：http://ojv.bjfxy.top

var d = ["a": 1];  d["b"] = 2
来源：http://kut.sysykeji.top

[T23] Swift：函数
来源：http://bzd.cashguo.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://asf.zhongyouzk.top

[T24] Swift：闭包
来源：http://isa.yj20258.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://ytr.bjfxy.top

[T25] Swift：结构体
来源：http://jml.ivvv.top

struct P { var x: Int }
来源：http://esd.meibo888.top

[T26] Swift：类与重写
来源：http://nnn.jinyuanbaomall.cn

class A: Base { override func f() {} }
来源：http://dtn.sweek.top

[T27] Swift：错误处理
来源：http://glc.svipenyu.cn

do { try f() } catch { print(error) }
来源：http://kci.sweek.top

[T28] Swift：枚举
来源：http://qph.fzhhl.top

enum Color { case red, green }
来源：http://mhp.birdmap.top

[T29] Swift：guard 提前返回
来源：http://qvs.hywenlv.cn

guard let x = opt else { return }
来源：http://fns.guowangkeji.top

[T30] Swift：协议
来源：http://vnc.yangfankeji.com

protocol Shape { func area() -> Double }
来源：http://mdy.52xcode.cn

[T31] Lua：Hello World
来源：http://jen.zhongyouzk.top

print("Hello")
来源：http://jyb.hywenlv.cn

[T32] Lua：局部变量
来源：http://gxw.ywan-chungtsiang.top

local a = 1
来源：http://jje.c1oappe.top

[T33] Lua：表（数组）
来源：http://rcc.jiagoushi.top

local t = {1, 2, 3};  t[4] = 4
来源：http://vje.gzhubu.top

[T34] Lua：遍历表
来源：http://ljg.sysykeji.top

for i, v in ipairs(t) do print(i, v) end
来源：http://jcc.sysykeji.top

[T35] Lua：字典表
来源：http://vgc.fanxiaobao.xyz

local d = { a = 1 };  d.b = 2
来源：http://ygq.hongshengwenyu.top

[T36] Lua：函数
来源：http://szr.yfazqb.com

function add(a, b) return a + b end
来源：http://nuu.jqgufenzy.top

[T37] Lua：字符串拼接
来源：http://lur.vehdjk.com

"a" .. "b"
来源：http://lht.redwolf501.top

[T38] Lua：条件
来源：http://kvw.jinyuanbaomall.cn

if x > 0 then print("正") end
来源：http://kkw.xziqi.cn

[T39] Lua：模式匹配
来源：http://wfb.gaohongyu789.top

string.find(s, "%d+")
来源：http://jfw.chenzaomai.com

[T40] Lua：元表
来源：http://lag.fzhhl.top

setmetatable({}, { __index = base })
来源：http://loi.guannengcc.top

[T41] Perl：Hello World
来源：http://zvm.xuetiantiany.cn

print "Hello\n";
来源：http://wie.zdqjudy.top

[T42] Perl：变量类型
来源：http://jrj.fzhhl.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://mph.daria6918.cn

[T43] Perl：字符串插值
来源：http://nls.vqdsnc.cn

"值: $a"
来源：http://kwc.jianghu66.top

[T44] Perl：条件
来源：http://mbk.xuetiantiany.cn

if ($a > 0) { print "正"; }
来源：http://hra.yonumen.top

[T45] Perl：数组遍历
来源：http://fea.52xcode.cn

for my $x (@arr) { print $x; }
来源：http://wcg.guowangkeji.top

[T46] Perl：哈希操作
来源：http://pmy.nwbrower.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://zjs.yj20258888.top

[T47] Perl：正则捕获
来源：http://cbl.hfpthk.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://olv.ybcxt.top

[T48] Perl：正则替换
来源：http://wzm.tarul.cn

$s =~ s/old/new/g;
来源：http://bxu.52xcode.cn

[T49] Perl：函数
来源：http://jqr.shanyushiyangtech.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://spf.xziqi.cn

[T50] Perl：逐行读文件
来源：http://jxn.shuidangran.top

open my $fh, "<", "a.txt" or die $!;
来源：http://evr.jinyuanbaomall.cn

while (my $line = <$fh>) { print $line; }
来源：http://pdv.ivvv.top

[T51] Scala：Hello World
来源：http://poa.daria6918.cn

println("Hello")
来源：http://zqf.tian-w.cn

[T52] Scala：变量
来源：http://znn.chenzaomai.com

val a = 1;  var b = 2
来源：http://iac.gaohongyu789.top

[T53] Scala：字符串插值
来源：http://lwg.feifeiyinyue.top

s"值: $b"
来源：http://dxl.chenjidiqi.icu

[T54] Scala：集合映射
来源：http://jfs.52xcode.cn

List(1, 2, 3).map(_ * 2)
来源：http://juo.jqgfzy.top

[T55] Scala：集合过滤
来源：http://mwq.hammf.cn

List(1, 2, 3).filter(_ > 1)
来源：http://arj.cdnleiting.top

[T56] Scala：样例类
来源：http://sit.tian-w.cn

case class User(name: String, age: Int)
来源：http://xuj.jqgufenzy.top

[T57] Scala：模式匹配
来源：http://egi.xylfe.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://lkh.birdmap.top

[T58] Scala：函数定义
来源：http://qgl.yuanzhike.top

def add(a: Int, b: Int): Int = a + b
来源：http://chs.yonumen.top

[T59] Scala：循环
来源：http://gii.uphjek.com

for (i <- 1 to 10) println(i)
来源：http://lnt.cdnleiting.top

[T60] Scala：折叠
来源：http://bms.zhixingplan.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://wpr.fzhhl.top

================================================================================
来源：http://zul.xuetiantiany.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://ejz.fengsongda.top

================================================================================
来源：http://mqz.shanyushiyangkeji.top

[U01] Py：创建虚拟环境
来源：http://muu.zhijiandao.cn

python -m venv .venv && source .venv/bin/activate
来源：http://sdd.cucudq.cn

[U02] Py：导出 / 安装依赖
来源：http://dvc.vqdsnc.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://zrr.hysaishi.cn

[U03] Py：加载 .env 配置
来源：http://tym.nwbrower.top

from dotenv import load_dotenv; load_dotenv()
来源：http://ygq.52xcode.cn

[U04] Py：变量调试打印
来源：http://oob.gaohongyu789.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://anc.xuetiantiany.cn

[U05] Py：列表去重且保序
来源：http://vus.yvedp.cn

list(dict.fromkeys(arr))
来源：http://wda.xziqi.cn

[U06] Py：合并两个字典
来源：http://waa.guowangkeji.top

{**a, **b}
来源：http://zrr.jinqigfzy.top


<!-- 参考信息 -->