代发 wailian999

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://fng.hcnkem.com

[R66] 定时任务
来源：http://ydb.sysykeji.top

crontab -e;  crontab -l
来源：http://msg.tian-w.cn

[R67] 生成随机十六进制串
来源：http://tpi.tanke756.top

openssl rand -hex 16
来源：http://gfb.fzhhl.top

[R68] 计算文件校验值
来源：http://vbv.zhijiandao.cn

sha256sum a.txt;  md5sum a.txt
来源：http://zil.aizwys.cn

[R69] 生成随机密码
来源：http://epq.meibo888.top

head -c 16 /dev/urandom | base64
来源：http://dvn.xziqi.cn

[R70] 时间戳与互转
来源：http://kta.yonumen.top

date +%s;  date -d @1700000000
来源：http://bfd.tian-w.cn

[R71] 日期格式化
来源：http://btg.jqgfzy.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://fmh.guowangkeji.top

[R72] 等待端口就绪
来源：http://jns.zycfv.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://hms.fengsongda.top

[R73] 分割大日志
来源：http://nfn.guannengcc.top

split -l 1000 big.log part_
来源：http://msj.jiagoushi.top

[R74] 批量重命名
来源：http://ezi.hfpthk.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://rso.yanxiufei.cn

[R75] 导出环境变量
来源：http://nwg.xziqi.cn

export PATH="$HOME/bin:$PATH"
来源：http://ahy.yj20258.top

[R76] 使用临时文件
来源：http://bve.bjfxy.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://pwr.ydzc1.top

[R77] 读取用户输入
来源：http://ejn.yonumen.top

read -rp "请输入: " ans
来源：http://jxy.jiagoushi.top

[R78] 交互式菜单
来源：http://jfc.guannengcc.top

select opt in a b c; do echo "$opt"; break; done
来源：http://vnj.cheryme.top

[R79] 解析命令行选项
来源：http://rsu.nanxuanxn.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://big.yj202588.top

[R80] 查看脚本执行耗时
来源：http://mlz.jqgufenzy.top

time ./run.sh
来源：http://dqr.gogol.net.cn

================================================================================
来源：http://sia.wangdashe.top

S. C / C++ 专题
来源：http://ajz.0kj1m.cn

================================================================================
来源：http://nce.ybcxt.top

[S01] C：Hello World
来源：http://ggo.dianchejie.cn

#include <stdio.h>
来源：http://qpl.xingfuxueyuan.xyz

int main(void) { printf("Hello\n"); return 0; }
来源：http://ohn.vqdsnc.cn

[S02] C：变量与格式化输出
来源：http://slj.9152youxi.cn

int a = 10; printf("%d\n", a);
来源：http://cfz.cheryme.top

[S03] C：读入整数
来源：http://sxm.jianghu66.top

int x; scanf("%d", &x);
来源：http://ymm.nwbrower.top

[S04] C：字符串复制
来源：http://onq.gotoacloud.top

char dst[32]; strcpy(dst, "hi");
来源：http://xbg.zhaomingkeji.xyz

[S05] C：字符串长度
来源：http://dtw.svipenyu.cn

strlen(s)
来源：http://xtf.sjlbkw.cn

[S06] C：字符串比较
来源：http://cug.zhixingplan.top

strcmp(a, b) == 0
来源：http://kjv.bjfxy.top

[S07] C：数组遍历求和
来源：http://boz.yj20258888.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://lga.tarul.cn

[S08] C：动态内存分配与释放
来源：http://fjw.yuxming.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://fnb.jianghu66.top

[S09] C：结构体定义与初始化
来源：http://vzt.chenjidiqi.icu

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://xch.nwbrower.top

[S10] C：指针与解引用
来源：http://zif.hfpthk.cn

int *p = &a;  *p = 5;
来源：http://qcp.52xcode.cn

[S11] C：逐行读文件
来源：http://ukh.cucudq.cn

FILE *f = fopen("a.txt", "r");
来源：http://nmf.vqdsnc.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://zuo.sxryk.cn

fclose(f);
来源：http://abb.fehbvm.com

[S12] C：写文件
来源：http://gnh.bbcook.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://ter.shuidangran.top

[S13] C：宏定义
来源：http://aac.gaohongyu789.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://xjc.yongpay.top

[S14] C：枚举
来源：http://yny.aizwys.cn

enum Color { RED, GREEN, BLUE };
来源：http://qbo.snrcjt.cn

[S15] C：类型转换
来源：http://pjw.0kj1m.cn

(double) a / b
来源：http://cwp.tarul.cn

[S16] C：位操作置位
来源：http://ycu.wangdashe.top

x |= (1 << 3);
来源：http://qlk.hnqzz.top

[S17] C：安全拼接字符串
来源：http://dyl.hcnkem.com

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://rvo.yanxiufei.cn

[S18] C：命令行参数
来源：http://erg.sweek.top

int main(int argc, char **argv)
来源：http://qog.ppjwa.cn

[S19] C：快速排序
来源：http://acj.chenzaomai.com

qsort(a, n, sizeof(int), cmp);
来源：http://hvd.xuanzx.com

[S20] C：二分查找
来源：http://nbl.jqgufenzy.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://vnn.vqdsnc.cn

[S21] C：字符类别判断
来源：http://ltp.bjfxy.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://qpm.hywenlv.cn

[S22] C：字符串转数字
来源：http://ked.zhaomingkeji.xyz

atoi("42");  strtod("3.14", NULL);
来源：http://auq.fktsv.cn

[S23] C：随机数
来源：http://owi.yfazqb.com

srand(time(NULL));  int r = rand() % 100;
来源：http://ljv.hammf.cn

[S24] C：获取本地时间
来源：http://wpm.dianchejie.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://khi.fengsongda.top

[S25] C：内存拷贝
来源：http://qnx.cashguo.top

memcpy(dst, src, n);
来源：http://gpm.yueranfly.top

[S26] C：内存清零
来源：http://lsh.nanxuanxn.top

memset(a, 0, sizeof a);
来源：http://pvr.xylfe.cn

[S27] C：定义常量
来源：http://loq.tanke756.top

const double PI = 3.14159;
来源：http://ncm.jqgufenzy.top

[S28] C：静态变量
来源：http://gku.xingfuxueyuan.xyz

static int counter = 0;
来源：http://mdm.sweek.top

[S29] C：变参函数
来源：http://nkf.svipenyu.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://lfv.vqdsnc.cn

[S30] C：头文件保护
来源：http://zqj.redwolf501.top

#ifndef X_H
来源：http://igk.shanyushiyangtech.top

#define X_H
来源：http://ckl.fehbvm.com

#endif
来源：http://xcl.xuetiantiany.cn

[S31] C++：Hello World
来源：http://fjd.fengsongda.top

#include <iostream>
来源：http://ilt.vehdjk.com

int main() { std::cout << "Hello\n"; }
来源：http://byi.chenzaomai.com

[S32] C++：字符串
来源：http://skb.zdbjq.cn

std::string s = "hi";  s += "!";
来源：http://nns.mhx1999.top

[S33] C++：vector 增删
来源：http://cld.yvedp.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://zhd.aibaodan.cn

[S34] C++：遍历 vector
来源：http://gss.nanxuanxn.top

for (auto &x : v) { std::cout << x; }
来源：http://pzm.sufxvd.cn

[S35] C++：map
来源：http://jev.shzxlz.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://gvz.svipenyu.cn

[S36] C++：unordered_map
来源：http://aaz.yvedp.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://mdl.kuanghao11.cn

[S37] C++：set
来源：http://qxb.fanxiaobao.xyz

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://nhn.dianchejie.cn

[S38] C++：排序
来源：http://mlj.pengpengdd.cyou

std::sort(v.begin(), v.end());
来源：http://weo.zhixingplan.top

[S39] C++：自定义比较器排序
来源：http://mfi.shzxlz.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://mnx.nanxinkj.top

[S40] C++：查找元素
来源：http://pwv.chenlongwang.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://god.vqdsnc.cn

[S41] C++：类与构造函数
来源：http://mra.guannengcc.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://jpv.xuetiantiany.cn

[S42] C++：继承与虚函数
来源：http://xtf.shangyingyoupin.top

class B : public Base { public: void f() override {} };
来源：http://smr.fehbvm.com

[S43] C++：智能指针
来源：http://prh.xinyue.icu

auto p = std::make_unique<int>(5);
来源：http://nqc.fktsv.cn

[S44] C++：引用传参
来源：http://jbi.ehwqpu.com

void inc(int &x) { ++x; }
来源：http://gfj.hcnkem.com

[S45] C++：lambda
来源：http://ifw.zhongyouzk.top

auto add = [](int a, int b) { return a + b; };
来源：http://jjz.fzhhl.top

[S46] C++：函数模板
来源：http://hut.fzhhl.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://ltp.cheryme.top

[S47] C++：结构化绑定遍历
来源：http://xar.sysykeji.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://puz.birdmap.top

[S48] C++：逐行读文件
来源：http://nnu.ivvv.top

std::ifstream in("a.txt");  std::string line;
来源：http://anc.ehwqpu.com

while (std::getline(in, line)) { }
来源：http://hlz.yj202588.top

[S49] C++：写文件
来源：http://hkn.xinyue.icu

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hzk.birdmap.top

[S50] C++：格式化数字
来源：http://oaq.mhx1999.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://jbb.ywan-chungtsiang.top

[S51] C++：显式类型转换
来源：http://hnh.c1oappe.top

static_cast<double>(a) / b
来源：http://dgi.yuanzhike.top

[S52] C++：const 与 noexcept
来源：http://zpx.ppjwa.cn

int size() const noexcept { return n_; }
来源：http://kdn.fanxiaobao.xyz

[S53] C++：移动语义
来源：http://ekd.kuanghao11.cn

std::vector<int> w = std::move(v);
来源：http://yui.ehwqpu.com

[S54] C++：异常处理
来源：http://swl.bjfxy.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://qrd.cashguo.top

[S55] C++：结构化绑定
来源：http://ijw.jqgfzy.top

auto [a, b] = std::make_pair(1, 2);
来源：http://xxl.ydzc1.top

[S56] C++：optional
来源：http://aap.feifeiyinyue.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://jas.cashguo.top

[S57] C++：编译期常量
来源：http://ywm.yj20258.top

constexpr int N = 10;
来源：http://agj.yangfankeji.com

[S58] C++：命名空间
来源：http://qyu.redwolf501.top

namespace ns { int f() { return 1; } }
来源：http://odn.feifeiyinyue.top

[S59] C++：静态断言
来源：http://apg.zycfv.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://tgf.yongpay.top

[S60] C++：遍历并删除元素
来源：http://nby.tianlin.xyz

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://fyb.guannengcc.top

================================================================================
来源：http://dew.guannengcc.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://ttu.sweek.top

================================================================================
来源：http://ome.zhiwuduotai.top

[T01] Kotlin：Hello World
来源：http://tus.zhoulong.xyz

println("Hello")
来源：http://jyh.yvedp.cn

[T02] Kotlin：变量
来源：http://zho.yongpay.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://idt.havefunace.top

[T03] Kotlin：字符串模板
来源：http://plz.fehbvm.com

"值: $b"
来源：http://omt.bbcook.cn

[T04] Kotlin：空安全
来源：http://ycu.hongshengwenyu.top

val n: String? = null;  n?.length
来源：http://aia.xingfuxueyuan.xyz

[T05] Kotlin：when 表达式
来源：http://iji.dianchejie.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://wfu.0kj1m.cn

[T06] Kotlin：集合映射
来源：http://cfg.bjfxy.top

listOf(1, 2, 3).map { it * 2 }
来源：http://xpx.ctjpmb.com

[T07] Kotlin：集合过滤
来源：http://gac.jiagoushi.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://csv.yj20258888.top

[T08] Kotlin：数据类
来源：http://gdg.hcnkem.com

data class User(val name: String, val age: Int)
来源：http://rdr.ydjk.org.cn

[T09] Kotlin：扩展函数
来源：http://hzu.havefunace.top

fun String.exclaim() = this + "!"
来源：http://orr.fzhhl.top

[T10] Kotlin：默认参数
来源：http://cgn.c1oappe.top

fun greet(name: String = "World") = "Hi $name"
来源：http://znh.havefunace.top

[T11] Kotlin：协程
来源：http://bkb.bbcook.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://ztf.yangfankeji.com

[T12] Kotlin：解构声明
来源：http://vqv.gotoacloud.top

val (a, b) = Pair(1, 2)
来源：http://jpr.snrcjt.cn

[T13] Kotlin：只读 Map
来源：http://nso.sjlbkw.cn

val m = mapOf("a" to 1)
来源：http://prq.shuidangran.top

[T14] Kotlin：循环
来源：http://dan.zdbjq.cn

for (i in 1..10) println(i)
来源：http://vjs.cdnleiting.top

[T15] Kotlin：接口
来源：http://dwn.daxiang520.top

interface Shape { fun area(): Double }
来源：http://ths.ppjwa.cn

[T16] Swift：Hello World
来源：http://mwq.jqgfzy.top

print("Hello")
来源：http://hwy.hfpthk.cn

[T17] Swift：变量与常量
来源：http://oum.yanxiufei.cn

var a = 1;  let b = 2
来源：http://sdp.gzhubu.top

[T18] Swift：字符串插值
来源：http://rcb.quarkkingdee.top

"值: \(b)"
来源：http://vzx.vehdjk.com

[T19] Swift：可选绑定
来源：http://nqm.redwolf501.top

if let n = opt { print(n) }
来源：http://igd.xuetiantiany.cn

[T20] Swift：数组操作
来源：http://lqi.haohaochexian.top

var a = [1, 2, 3];  a.append(4)
来源：http://wqk.hesvh.cn

[T21] Swift：遍历
来源：http://qem.yongpay.top

for x in a { print(x) }
来源：http://man.jinyuanbaomall.cn

[T22] Swift：字典
来源：http://evt.fzhhl.top

var d = ["a": 1];  d["b"] = 2
来源：http://ovf.jlsjyb.cn

[T23] Swift：函数
来源：http://cvy.jinqigufen.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://nba.jqgufenzy.top

[T24] Swift：闭包
来源：http://nks.9152youxi.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://znt.fengsongda.top

[T25] Swift：结构体
来源：http://gtu.jqgufenzy.top

struct P { var x: Int }
来源：http://szv.chenjidiqi.icu

[T26] Swift：类与重写
来源：http://dfm.gzhubu.top

class A: Base { override func f() {} }
来源：http://ogt.ydzc1.top

[T27] Swift：错误处理
来源：http://uxg.cqqwz.cn

do { try f() } catch { print(error) }
来源：http://tdc.jyoumei.cn

[T28] Swift：枚举
来源：http://cqr.yonumen.top

enum Color { case red, green }
来源：http://rnz.ybcxt.top

[T29] Swift：guard 提前返回
来源：http://zrc.hfpthk.cn

guard let x = opt else { return }
来源：http://hfc.xingfuxueyuan.xyz

[T30] Swift：协议
来源：http://axp.quarkkingdee.top

protocol Shape { func area() -> Double }
来源：http://fea.xuetiantiany.cn

[T31] Lua：Hello World
来源：http://dmu.dashuyun.cn

print("Hello")
来源：http://ypr.zhixingplan.top

[T32] Lua：局部变量
来源：http://zpd.ydzc1.top

local a = 1
来源：http://uaj.xuanzx.com

[T33] Lua：表（数组）
来源：http://zls.guowangkeji.top

local t = {1, 2, 3};  t[4] = 4
来源：http://lxa.zhoulong.xyz

[T34] Lua：遍历表
来源：http://fpj.shuidangran.top

for i, v in ipairs(t) do print(i, v) end
来源：http://wfd.9152youxi.cn

[T35] Lua：字典表
来源：http://mqu.fehbvm.com

local d = { a = 1 };  d.b = 2
来源：http://pje.sweek.top

[T36] Lua：函数
来源：http://pbd.yvedp.cn

function add(a, b) return a + b end
来源：http://chg.kuanghao11.cn

[T37] Lua：字符串拼接
来源：http://orc.vqdsnc.cn

"a" .. "b"
来源：http://iua.cqqwz.cn

[T38] Lua：条件
来源：http://wpw.hywenlv.cn

if x > 0 then print("正") end
来源：http://ggo.jyoumei.cn

[T39] Lua：模式匹配
来源：http://fve.zhengqikj.top

string.find(s, "%d+")
来源：http://psb.ydjk.org.cn

[T40] Lua：元表
来源：http://wyt.aizwys.cn

setmetatable({}, { __index = base })
来源：http://hqk.yonumen.top

[T41] Perl：Hello World
来源：http://hgj.zdqjudy.top

print "Hello\n";
来源：http://dpt.yj202588.top

[T42] Perl：变量类型
来源：http://pcp.nanxuanxn.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://olk.cheryme.top

[T43] Perl：字符串插值
来源：http://qgh.zhongyouzk.top

"值: $a"
来源：http://vfv.jinghuilouyu.cn

[T44] Perl：条件
来源：http://pju.ivvv.top

if ($a > 0) { print "正"; }
来源：http://mti.ydjk.org.cn

[T45] Perl：数组遍历
来源：http://vnt.316326.xyz

for my $x (@arr) { print $x; }
来源：http://ekl.shzxlz.cn

[T46] Perl：哈希操作
来源：http://iga.jianghu66.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://mkk.yanxiufei.cn

[T47] Perl：正则捕获
来源：http://var.xingfuxueyuan.xyz

if ($s =~ /(\d+)/) { print $1; }
来源：http://tch.zhengqikj.top

[T48] Perl：正则替换
来源：http://qln.guowangkeji.top

$s =~ s/old/new/g;
来源：http://waz.sysykeji.top

[T49] Perl：函数
来源：http://mvd.hfpthk.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://fuk.chenlongwang.top

[T50] Perl：逐行读文件
来源：http://uoa.pycfn.com

open my $fh, "<", "a.txt" or die $!;
来源：http://hak.zhiwuduotai.top

while (my $line = <$fh>) { print $line; }
来源：http://qjw.haohaochexian.top

[T51] Scala：Hello World
来源：http://qhk.cashguo.top

println("Hello")
来源：http://qjx.yvedp.cn

[T52] Scala：变量
来源：http://xcv.ivvv.top

val a = 1;  var b = 2
来源：http://fif.yvedp.cn

[T53] Scala：字符串插值
来源：http://thy.cheryme.top

s"值: $b"
来源：http://aqu.xylfe.cn

[T54] Scala：集合映射
来源：http://ase.hongshengwenyu.top

List(1, 2, 3).map(_ * 2)
来源：http://kbo.ydzc1.top

[T55] Scala：集合过滤
来源：http://mav.hnxiangtu.top

List(1, 2, 3).filter(_ > 1)
来源：http://dms.ctjpmb.com

[T56] Scala：样例类
来源：http://xps.yangfankeji.com

case class User(name: String, age: Int)
来源：http://yjw.smart0.xyz

[T57] Scala：模式匹配
来源：http://ico.smart0.xyz

x match { case 1 => "一"; case _ => "其他" }
来源：http://rsf.cheryme.top

[T58] Scala：函数定义
来源：http://xav.sysykeji.top

def add(a: Int, b: Int): Int = a + b
来源：http://sdg.zhijiandao.cn

[T59] Scala：循环
来源：http://ngo.52xcode.cn

for (i <- 1 to 10) println(i)
来源：http://trc.zdqjudy.top

[T60] Scala：折叠
来源：http://cfz.zhiwuduotai.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://bdi.jinyuanbaomall.cn

================================================================================
来源：http://ovt.ydjk.org.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://qrt.tanke756.top

================================================================================
来源：http://juv.yonumen.top

[U01] Py：创建虚拟环境
来源：http://dxh.aibaodan.cn

python -m venv .venv && source .venv/bin/activate
来源：http://kmg.zhiwuduotai.top

[U02] Py：导出 / 安装依赖
来源：http://jfr.fanxiaobao.xyz

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://wsb.fengsongda.top

[U03] Py：加载 .env 配置
来源：http://bqm.zhixingplan.top

from dotenv import load_dotenv; load_dotenv()
来源：http://zjz.jqgufenzy.top

[U04] Py：变量调试打印
来源：http://roj.jqgufenzy.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://jzb.jinghuilouyu.cn

[U05] Py：列表去重且保序
来源：http://yys.ydjk.org.cn

list(dict.fromkeys(arr))
来源：http://fad.gogol.net.cn

[U06] Py：合并两个字典
来源：http://jnw.yanxiufei.cn

{**a, **b}
来源：http://feg.bbcook.cn


<!-- 参考信息 -->