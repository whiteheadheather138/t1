代发 wailian999

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://vcw.shanyushiyangtech.top

[R66] 定时任务
来源：http://dvg.cheryme.top

crontab -e;  crontab -l
来源：http://xrg.zdqjudy.top

[R67] 生成随机十六进制串
来源：http://dpa.haohaochexian.top

openssl rand -hex 16
来源：http://fpv.tian-w.cn

[R68] 计算文件校验值
来源：http://zcp.aibaodan.cn

sha256sum a.txt;  md5sum a.txt
来源：http://xwf.ppjwa.cn

[R69] 生成随机密码
来源：http://pkw.vqdsnc.cn

head -c 16 /dev/urandom | base64
来源：http://lni.jqgfzy.top

[R70] 时间戳与互转
来源：http://dub.tarul.cn

date +%s;  date -d @1700000000
来源：http://cqh.yongpay.top

[R71] 日期格式化
来源：http://fbm.yuanzhike.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://xut.ehwqpu.com

[R72] 等待端口就绪
来源：http://htz.shangyingyoupin.top

until nc -z localhost 3306; do sleep 1; done
来源：http://tyf.316326.xyz

[R73] 分割大日志
来源：http://unu.daxiang520.top

split -l 1000 big.log part_
来源：http://rhs.hesvh.cn

[R74] 批量重命名
来源：http://rcd.sufxvd.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hch.nanxuanxn.top

[R75] 导出环境变量
来源：http://mci.hnqzz.top

export PATH="$HOME/bin:$PATH"
来源：http://plv.jiagoushi.top

[R76] 使用临时文件
来源：http://ogm.zhengqikj.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://fjq.sxryk.cn

[R77] 读取用户输入
来源：http://dnn.fehbvm.com

read -rp "请输入: " ans
来源：http://ygv.zhijiandao.cn

[R78] 交互式菜单
来源：http://gan.shangyingyoupin.top

select opt in a b c; do echo "$opt"; break; done
来源：http://xnw.sjlbkw.cn

[R79] 解析命令行选项
来源：http://ipx.sweek.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://tkm.zycfv.cn

[R80] 查看脚本执行耗时
来源：http://ifz.yanxiufei.cn

time ./run.sh
来源：http://wkk.uphjek.com

================================================================================
来源：http://uer.tianlin.xyz

S. C / C++ 专题
来源：http://gvg.tarul.cn

================================================================================
来源：http://nuo.yongpay.top

[S01] C：Hello World
来源：http://pbk.smart0.xyz

#include <stdio.h>
来源：http://nhw.nanxuanxn.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://bfk.zhengqikj.top

[S02] C：变量与格式化输出
来源：http://hqg.jinqigufen.top

int a = 10; printf("%d\n", a);
来源：http://ygy.sweek.top

[S03] C：读入整数
来源：http://sdm.cqqwz.cn

int x; scanf("%d", &x);
来源：http://tul.zhiwuduotai.top

[S04] C：字符串复制
来源：http://iix.gogol.net.cn

char dst[32]; strcpy(dst, "hi");
来源：http://lgj.jqgfzy.top

[S05] C：字符串长度
来源：http://rvb.cqqwz.cn

strlen(s)
来源：http://bmk.gotoacloud.top

[S06] C：字符串比较
来源：http://nxa.wangshuangyany.cn

strcmp(a, b) == 0
来源：http://fsw.gotoacloud.top

[S07] C：数组遍历求和
来源：http://vlc.tianlin.xyz

for (int i = 0; i < n; i++) sum += a[i];
来源：http://zuk.andypj.xyz

[S08] C：动态内存分配与释放
来源：http://rdr.sxryk.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://qhz.havefunace.top

[S09] C：结构体定义与初始化
来源：http://xbt.epnwcf.com

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://acq.cashguo.top

[S10] C：指针与解引用
来源：http://wlq.hesvh.cn

int *p = &a;  *p = 5;
来源：http://gxz.ehwqpu.com

[S11] C：逐行读文件
来源：http://pcc.birdmap.top

FILE *f = fopen("a.txt", "r");
来源：http://yxd.fktsv.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://wru.aibaodan.cn

fclose(f);
来源：http://ogs.bjfxy.top

[S12] C：写文件
来源：http://pbv.nanxuanxn.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://lou.sweek.top

[S13] C：宏定义
来源：http://ijv.hesvh.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://sdn.uphjek.com

[S14] C：枚举
来源：http://osv.sufxvd.cn

enum Color { RED, GREEN, BLUE };
来源：http://tme.xziqi.cn

[S15] C：类型转换
来源：http://qxq.jinqigufen.top

(double) a / b
来源：http://cvc.ydjk.org.cn

[S16] C：位操作置位
来源：http://hwh.cdnleiting.top

x |= (1 << 3);
来源：http://mku.yuanzhike.top

[S17] C：安全拼接字符串
来源：http://epu.yuxming.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://puf.jinyuanbaomall.cn

[S18] C：命令行参数
来源：http://lts.jinyuanbaomall.cn

int main(int argc, char **argv)
来源：http://fzp.dashuyun.cn

[S19] C：快速排序
来源：http://hlm.zhaomingkeji.xyz

qsort(a, n, sizeof(int), cmp);
来源：http://jyn.ydjk.org.cn

[S20] C：二分查找
来源：http://tdi.fzhhl.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://bfq.svipenyu.cn

[S21] C：字符类别判断
来源：http://gbz.hnxiangtu.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://san.sysykeji.top

[S22] C：字符串转数字
来源：http://lke.daxiang520.top

atoi("42");  strtod("3.14", NULL);
来源：http://hgu.ppjwa.cn

[S23] C：随机数
来源：http://syu.ehwqpu.com

srand(time(NULL));  int r = rand() % 100;
来源：http://jlf.0kj1m.cn

[S24] C：获取本地时间
来源：http://wms.fzhhl.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://jlp.jyoumei.cn

[S25] C：内存拷贝
来源：http://dfl.jqgufenzy.top

memcpy(dst, src, n);
来源：http://pyl.ydzc1.top

[S26] C：内存清零
来源：http://pyh.yj202588.top

memset(a, 0, sizeof a);
来源：http://wgc.shangyingyoupin.top

[S27] C：定义常量
来源：http://fhf.nwbrower.top

const double PI = 3.14159;
来源：http://vls.shanyushiyangkeji.top

[S28] C：静态变量
来源：http://fqy.uphjek.com

static int counter = 0;
来源：http://acg.pycfn.com

[S29] C：变参函数
来源：http://guf.iojbl.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://ddv.pycfn.com

[S30] C：头文件保护
来源：http://yqr.haohaochexian.top

#ifndef X_H
来源：http://sdw.fengsongda.top

#define X_H
来源：http://pvf.jinqigfzy.top

#endif
来源：http://nnu.ctjpmb.com

[S31] C++：Hello World
来源：http://teu.sysykeji.top

#include <iostream>
来源：http://upx.jqgfzy.top

int main() { std::cout << "Hello\n"; }
来源：http://sig.fzhhl.top

[S32] C++：字符串
来源：http://vds.cheryme.top

std::string s = "hi";  s += "!";
来源：http://yfc.xuetiantiany.cn

[S33] C++：vector 增删
来源：http://qst.hywenlv.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hcp.shzxlz.cn

[S34] C++：遍历 vector
来源：http://slk.jianghu66.top

for (auto &x : v) { std::cout << x; }
来源：http://vbc.yj20258.top

[S35] C++：map
来源：http://xox.jiagoushi.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://qsd.yonumen.top

[S36] C++：unordered_map
来源：http://mja.zhaomingkeji.xyz

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://kpv.xinyue.icu

[S37] C++：set
来源：http://ipd.jiagoushi.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://fjc.hywenlv.cn

[S38] C++：排序
来源：http://rug.guowangkeji.top

std::sort(v.begin(), v.end());
来源：http://vxt.ywan-chungtsiang.top

[S39] C++：自定义比较器排序
来源：http://jhb.zycfv.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://ttt.ydzc1.top

[S40] C++：查找元素
来源：http://ccu.jyoumei.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://puk.cheryme.top

[S41] C++：类与构造函数
来源：http://gar.chenlongwang.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://zls.ydjk.org.cn

[S42] C++：继承与虚函数
来源：http://ems.chenlongwang.top

class B : public Base { public: void f() override {} };
来源：http://lym.nanxuanxn.top

[S43] C++：智能指针
来源：http://jkt.zhixingplan.top

auto p = std::make_unique<int>(5);
来源：http://lkl.jiagoushi.top

[S44] C++：引用传参
来源：http://bak.tian-w.cn

void inc(int &x) { ++x; }
来源：http://hcx.meibo888.top

[S45] C++：lambda
来源：http://fai.shuidangran.top

auto add = [](int a, int b) { return a + b; };
来源：http://zip.hfpthk.cn

[S46] C++：函数模板
来源：http://aes.jyoumei.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://bid.jinyuanbaomall.cn

[S47] C++：结构化绑定遍历
来源：http://raj.sysykeji.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://yub.jqgfzy.top

[S48] C++：逐行读文件
来源：http://plx.gogol.net.cn

std::ifstream in("a.txt");  std::string line;
来源：http://vjc.ehwqpu.com

while (std::getline(in, line)) { }
来源：http://itp.nanxuanxn.top

[S49] C++：写文件
来源：http://mqt.guannengcc.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://kya.xuanzx.com

[S50] C++：格式化数字
来源：http://zls.daria6918.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://dvi.hcnkem.com

[S51] C++：显式类型转换
来源：http://gqh.yueranfly.top

static_cast<double>(a) / b
来源：http://dci.xziqi.cn

[S52] C++：const 与 noexcept
来源：http://lsv.bbcook.cn

int size() const noexcept { return n_; }
来源：http://idy.cashguo.top

[S53] C++：移动语义
来源：http://ofq.sweek.top

std::vector<int> w = std::move(v);
来源：http://ihq.zycfv.cn

[S54] C++：异常处理
来源：http://lwx.haohaochexian.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://bjp.tian-w.cn

[S55] C++：结构化绑定
来源：http://zew.cucudq.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://oiw.ywan-chungtsiang.top

[S56] C++：optional
来源：http://bos.yvedp.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://qka.xylfe.cn

[S57] C++：编译期常量
来源：http://low.andypj.xyz

constexpr int N = 10;
来源：http://vis.zhoulong.xyz

[S58] C++：命名空间
来源：http://zhh.jqgufenzy.top

namespace ns { int f() { return 1; } }
来源：http://tui.meibo888.top

[S59] C++：静态断言
来源：http://uyn.aibaodan.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://yeo.yj20258888.top

[S60] C++：遍历并删除元素
来源：http://bpi.yonumen.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://svn.zhiwuduotai.top

================================================================================
来源：http://hvv.9152youxi.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://woe.guowangkeji.top

================================================================================
来源：http://jfg.zhoulong.xyz

[T01] Kotlin：Hello World
来源：http://mme.cucudq.cn

println("Hello")
来源：http://wxr.316326.xyz

[T02] Kotlin：变量
来源：http://rfq.hcnkem.com

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://wzd.havefunace.top

[T03] Kotlin：字符串模板
来源：http://aqm.hongshengwenyu.top

"值: $b"
来源：http://avs.zhengqikj.top

[T04] Kotlin：空安全
来源：http://ype.daxiang520.top

val n: String? = null;  n?.length
来源：http://thl.tianlin.xyz

[T05] Kotlin：when 表达式
来源：http://ggp.xinyue.icu

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://qzg.wangdashe.top

[T06] Kotlin：集合映射
来源：http://hig.hesvh.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://xhq.tian-w.cn

[T07] Kotlin：集合过滤
来源：http://hrn.meibo888.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://vxq.gogol.net.cn

[T08] Kotlin：数据类
来源：http://pzz.52xcode.cn

data class User(val name: String, val age: Int)
来源：http://jpi.fehbvm.com

[T09] Kotlin：扩展函数
来源：http://oct.hnqzz.top

fun String.exclaim() = this + "!"
来源：http://qxg.shangyingyoupin.top

[T10] Kotlin：默认参数
来源：http://iaq.vqdsnc.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://eyr.ywan-chungtsiang.top

[T11] Kotlin：协程
来源：http://rto.nanxuanxn.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://swa.xingfuxueyuan.xyz

[T12] Kotlin：解构声明
来源：http://rvk.9152youxi.cn

val (a, b) = Pair(1, 2)
来源：http://tqp.ywan-chungtsiang.top

[T13] Kotlin：只读 Map
来源：http://hxm.cheryme.top

val m = mapOf("a" to 1)
来源：http://jek.shzxlz.cn

[T14] Kotlin：循环
来源：http://zqi.havefunace.top

for (i in 1..10) println(i)
来源：http://vwq.feifeiyinyue.top

[T15] Kotlin：接口
来源：http://jfi.snrcjt.cn

interface Shape { fun area(): Double }
来源：http://lvs.zhijiandao.cn

[T16] Swift：Hello World
来源：http://aor.daria6918.cn

print("Hello")
来源：http://bjv.tianlin.xyz

[T17] Swift：变量与常量
来源：http://ush.nanxinkj.top

var a = 1;  let b = 2
来源：http://jgu.zhiwuduotai.top

[T18] Swift：字符串插值
来源：http://dpo.tianlin.xyz

"值: \(b)"
来源：http://ziu.wangdashe.top

[T19] Swift：可选绑定
来源：http://kzz.nwbrower.top

if let n = opt { print(n) }
来源：http://ype.nanxuanxn.top

[T20] Swift：数组操作
来源：http://ndp.yuanzhike.top

var a = [1, 2, 3];  a.append(4)
来源：http://bgr.ydzc1.top

[T21] Swift：遍历
来源：http://ptq.iojbl.cn

for x in a { print(x) }
来源：http://wuz.ywan-chungtsiang.top

[T22] Swift：字典
来源：http://jnb.redwolf501.top

var d = ["a": 1];  d["b"] = 2
来源：http://wxk.sxryk.cn

[T23] Swift：函数
来源：http://exh.cucudq.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://ydb.hammf.cn

[T24] Swift：闭包
来源：http://ebx.fanxiaobao.xyz

let f = { (x: Int) -> Int in x * 2 }
来源：http://stn.ppjwa.cn

[T25] Swift：结构体
来源：http://jmh.52xcode.cn

struct P { var x: Int }
来源：http://gpq.ctjpmb.com

[T26] Swift：类与重写
来源：http://khm.jinyuanbaomall.cn

class A: Base { override func f() {} }
来源：http://rcu.tanke756.top

[T27] Swift：错误处理
来源：http://oga.yvedp.cn

do { try f() } catch { print(error) }
来源：http://qbw.chenlongwang.top

[T28] Swift：枚举
来源：http://zil.fehbvm.com

enum Color { case red, green }
来源：http://dga.316326.xyz

[T29] Swift：guard 提前返回
来源：http://ief.chenzaomai.com

guard let x = opt else { return }
来源：http://yls.birdmap.top

[T30] Swift：协议
来源：http://isy.c1oappe.top

protocol Shape { func area() -> Double }
来源：http://dye.birdmap.top

[T31] Lua：Hello World
来源：http://qjk.bjfxy.top

print("Hello")
来源：http://ngd.kuanghao11.cn

[T32] Lua：局部变量
来源：http://zku.sufxvd.cn

local a = 1
来源：http://unx.jqgufenzy.top

[T33] Lua：表（数组）
来源：http://hbc.hesvh.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://lgl.yvedp.cn

[T34] Lua：遍历表
来源：http://qsx.fanxiaobao.xyz

for i, v in ipairs(t) do print(i, v) end
来源：http://uql.jlsjyb.cn

[T35] Lua：字典表
来源：http://swn.0kj1m.cn

local d = { a = 1 };  d.b = 2
来源：http://ylm.jianghu66.top

[T36] Lua：函数
来源：http://gyz.shzxlz.cn

function add(a, b) return a + b end
来源：http://wmm.ctjpmb.com

[T37] Lua：字符串拼接
来源：http://scu.jianghu66.top

"a" .. "b"
来源：http://xjp.zycfv.cn

[T38] Lua：条件
来源：http://dgd.bjfxy.top

if x > 0 then print("正") end
来源：http://zbu.hnxiangtu.top

[T39] Lua：模式匹配
来源：http://axs.jlsjyb.cn

string.find(s, "%d+")
来源：http://svx.shangyingyoupin.top

[T40] Lua：元表
来源：http://cih.tian-w.cn

setmetatable({}, { __index = base })
来源：http://vzo.hfpthk.cn

[T41] Perl：Hello World
来源：http://kka.wangdashe.top

print "Hello\n";
来源：http://ljj.sysykeji.top

[T42] Perl：变量类型
来源：http://vbz.snrcjt.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://ncd.epnwcf.com

[T43] Perl：字符串插值
来源：http://zub.havefunace.top

"值: $a"
来源：http://fkb.smart0.xyz

[T44] Perl：条件
来源：http://qpc.fanxiaobao.xyz

if ($a > 0) { print "正"; }
来源：http://irv.zhixingplan.top

[T45] Perl：数组遍历
来源：http://dvv.meibo888.top

for my $x (@arr) { print $x; }
来源：http://ldo.jyoumei.cn

[T46] Perl：哈希操作
来源：http://jgk.yj202588.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://kbm.xuetiantiany.cn

[T47] Perl：正则捕获
来源：http://sdv.daria6918.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://yzv.tian-w.cn

[T48] Perl：正则替换
来源：http://myc.9152youxi.cn

$s =~ s/old/new/g;
来源：http://eiv.yuxming.cn

[T49] Perl：函数
来源：http://mgr.yongpay.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://caz.jinyuanbaomall.cn

[T50] Perl：逐行读文件
来源：http://nzs.gaohongyu789.top

open my $fh, "<", "a.txt" or die $!;
来源：http://bhu.pycfn.com

while (my $line = <$fh>) { print $line; }
来源：http://luj.tarul.cn

[T51] Scala：Hello World
来源：http://ryk.ivvv.top

println("Hello")
来源：http://uvy.gaohongyu789.top

[T52] Scala：变量
来源：http://xlq.zhoulong.xyz

val a = 1;  var b = 2
来源：http://rfr.ehwqpu.com

[T53] Scala：字符串插值
来源：http://vvv.wangshuangyany.cn

s"值: $b"
来源：http://xyx.zdbjq.cn

[T54] Scala：集合映射
来源：http://waq.bbcook.cn

List(1, 2, 3).map(_ * 2)
来源：http://bqy.yj20258.top

[T55] Scala：集合过滤
来源：http://byg.uphjek.com

List(1, 2, 3).filter(_ > 1)
来源：http://qeg.redwolf501.top

[T56] Scala：样例类
来源：http://wwa.yongpay.top

case class User(name: String, age: Int)
来源：http://pjm.chenzaomai.com

[T57] Scala：模式匹配
来源：http://omm.gaohongyu789.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://mlr.hysaishi.cn

[T58] Scala：函数定义
来源：http://eod.meibo888.top

def add(a: Int, b: Int): Int = a + b
来源：http://quk.sufxvd.cn

[T59] Scala：循环
来源：http://lkj.fzhhl.top

for (i <- 1 to 10) println(i)
来源：http://wxu.gogol.net.cn

[T60] Scala：折叠
来源：http://frs.ydjk.org.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://gdc.shangyingyoupin.top

================================================================================
来源：http://xaw.nwbrower.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://ybq.chenzaomai.com

================================================================================
来源：http://ojw.shuidangran.top

[U01] Py：创建虚拟环境
来源：http://tsq.aibaodan.cn

python -m venv .venv && source .venv/bin/activate
来源：http://qwr.fktsv.cn

[U02] Py：导出 / 安装依赖
来源：http://lsb.jinghuilouyu.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://yep.nwbrower.top

[U03] Py：加载 .env 配置
来源：http://yqs.smart0.xyz

from dotenv import load_dotenv; load_dotenv()
来源：http://uqi.xuetiantiany.cn

[U04] Py：变量调试打印
来源：http://keb.jlsjyb.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://jog.dianchejie.cn

[U05] Py：列表去重且保序
来源：http://ray.svipenyu.cn

list(dict.fromkeys(arr))
来源：http://poq.zhiwuduotai.top

[U06] Py：合并两个字典
来源：http://kfa.sufxvd.cn

{**a, **b}
来源：http://lek.jlsjyb.cn


<!-- 参考信息 -->