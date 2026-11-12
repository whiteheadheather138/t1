代发 wailian999

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://gyn.0kj1m.cn

[R66] 定时任务
来源：http://kym.yanxiufei.cn

crontab -e;  crontab -l
来源：http://uex.hfpthk.cn

[R67] 生成随机十六进制串
来源：http://ikp.tianlin.xyz

openssl rand -hex 16
来源：http://xit.jqgufenzy.top

[R68] 计算文件校验值
来源：http://xhw.nanxuanxn.top

sha256sum a.txt;  md5sum a.txt
来源：http://cal.chenlongwang.top

[R69] 生成随机密码
来源：http://boz.yangfankeji.com

head -c 16 /dev/urandom | base64
来源：http://tqo.jinghuilouyu.cn

[R70] 时间戳与互转
来源：http://ulc.dashuyun.cn

date +%s;  date -d @1700000000
来源：http://wzl.yvedp.cn

[R71] 日期格式化
来源：http://jqn.redwolf501.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://bzd.dianchejie.cn

[R72] 等待端口就绪
来源：http://qtf.kuanghao11.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://ssi.guannengcc.top

[R73] 分割大日志
来源：http://udi.sxryk.cn

split -l 1000 big.log part_
来源：http://hrj.jinqigufen.top

[R74] 批量重命名
来源：http://xxy.shanyushiyangtech.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://yfm.yuxming.cn

[R75] 导出环境变量
来源：http://mkr.redwolf501.top

export PATH="$HOME/bin:$PATH"
来源：http://lkc.zhoulong.xyz

[R76] 使用临时文件
来源：http://xzx.fanxiaobao.xyz

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://utx.yanxiufei.cn

[R77] 读取用户输入
来源：http://phj.hcnkem.com

read -rp "请输入: " ans
来源：http://lrh.ydzc1.top

[R78] 交互式菜单
来源：http://ihh.birdmap.top

select opt in a b c; do echo "$opt"; break; done
来源：http://feo.shangyingyoupin.top

[R79] 解析命令行选项
来源：http://mbd.yonumen.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://zkd.yangfankeji.com

[R80] 查看脚本执行耗时
来源：http://wto.shanyushiyangkeji.top

time ./run.sh
来源：http://wjg.nanxuanxn.top

================================================================================
来源：http://vmh.yfazqb.com

S. C / C++ 专题
来源：http://fup.jlsjyb.cn

================================================================================
来源：http://gog.sufxvd.cn

[S01] C：Hello World
来源：http://fzw.ydzc1.top

#include <stdio.h>
来源：http://csp.snrcjt.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://urf.meibo888.top

[S02] C：变量与格式化输出
来源：http://mli.yj20258888.top

int a = 10; printf("%d\n", a);
来源：http://vxz.chenzaomai.com

[S03] C：读入整数
来源：http://iwx.chenjidiqi.icu

int x; scanf("%d", &x);
来源：http://jlt.feifeiyinyue.top

[S04] C：字符串复制
来源：http://sxf.xylfe.cn

char dst[32]; strcpy(dst, "hi");
来源：http://znf.bjfxy.top

[S05] C：字符串长度
来源：http://mhl.yueranfly.top

strlen(s)
来源：http://dps.hysaishi.cn

[S06] C：字符串比较
来源：http://hlk.wangdashe.top

strcmp(a, b) == 0
来源：http://lkg.hongshengwenyu.top

[S07] C：数组遍历求和
来源：http://cta.quarkkingdee.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://mjs.sweek.top

[S08] C：动态内存分配与释放
来源：http://npy.daria6918.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://ete.zycfv.cn

[S09] C：结构体定义与初始化
来源：http://sjo.zhongyouzk.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://ocq.zhijiandao.cn

[S10] C：指针与解引用
来源：http://ktf.nanxinkj.top

int *p = &a;  *p = 5;
来源：http://kvq.yueranfly.top

[S11] C：逐行读文件
来源：http://xlf.shangyingyoupin.top

FILE *f = fopen("a.txt", "r");
来源：http://pqu.chenzaomai.com

while (fgets(buf, sizeof buf, f)) { }
来源：http://uxw.sxryk.cn

fclose(f);
来源：http://ajk.zhongyouzk.top

[S12] C：写文件
来源：http://yqx.316326.xyz

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://fmy.jyoumei.cn

[S13] C：宏定义
来源：http://uig.xuanzx.com

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://sbv.jianghu66.top

[S14] C：枚举
来源：http://mgo.c1oappe.top

enum Color { RED, GREEN, BLUE };
来源：http://ckt.yuxming.cn

[S15] C：类型转换
来源：http://arc.zhijiandao.cn

(double) a / b
来源：http://ulh.havefunace.top

[S16] C：位操作置位
来源：http://rgk.hnqzz.top

x |= (1 << 3);
来源：http://jjm.nwbrower.top

[S17] C：安全拼接字符串
来源：http://erz.sjlbkw.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://ubp.pengpengdd.cyou

[S18] C：命令行参数
来源：http://svg.aibaodan.cn

int main(int argc, char **argv)
来源：http://ygf.jyoumei.cn

[S19] C：快速排序
来源：http://vii.bbcook.cn

qsort(a, n, sizeof(int), cmp);
来源：http://rsf.9152youxi.cn

[S20] C：二分查找
来源：http://fmy.hammf.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://xbu.52xcode.cn

[S21] C：字符类别判断
来源：http://hyh.aibaodan.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://ady.haohaochexian.top

[S22] C：字符串转数字
来源：http://pqt.guannengcc.top

atoi("42");  strtod("3.14", NULL);
来源：http://hei.gzhubu.top

[S23] C：随机数
来源：http://pct.aizwys.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://nbd.yongpay.top

[S24] C：获取本地时间
来源：http://qtd.zdqjudy.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://acl.tian-w.cn

[S25] C：内存拷贝
来源：http://mpi.jyoumei.cn

memcpy(dst, src, n);
来源：http://uae.ywan-chungtsiang.top

[S26] C：内存清零
来源：http://mrs.sweek.top

memset(a, 0, sizeof a);
来源：http://ytq.hammf.cn

[S27] C：定义常量
来源：http://nsw.yvedp.cn

const double PI = 3.14159;
来源：http://mpj.hnqzz.top

[S28] C：静态变量
来源：http://lag.xziqi.cn

static int counter = 0;
来源：http://fdi.svipenyu.cn

[S29] C：变参函数
来源：http://jvo.316326.xyz

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://uxl.yangfankeji.com

[S30] C：头文件保护
来源：http://gwy.yonumen.top

#ifndef X_H
来源：http://nsi.dianchejie.cn

#define X_H
来源：http://xme.ybcxt.top

#endif
来源：http://ytk.xziqi.cn

[S31] C++：Hello World
来源：http://eqn.hysaishi.cn

#include <iostream>
来源：http://rzl.shanyushiyangtech.top

int main() { std::cout << "Hello\n"; }
来源：http://xln.andypj.xyz

[S32] C++：字符串
来源：http://xhc.yongpay.top

std::string s = "hi";  s += "!";
来源：http://ras.tian-w.cn

[S33] C++：vector 增删
来源：http://qnd.sufxvd.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://vfv.fehbvm.com

[S34] C++：遍历 vector
来源：http://vhn.zhongyouzk.top

for (auto &x : v) { std::cout << x; }
来源：http://bxy.ywan-chungtsiang.top

[S35] C++：map
来源：http://otg.wangshuangyany.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://pki.cqqwz.cn

[S36] C++：unordered_map
来源：http://rvq.tianlin.xyz

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://zvv.pengpengdd.cyou

[S37] C++：set
来源：http://brg.chenzaomai.com

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://azy.snrcjt.cn

[S38] C++：排序
来源：http://jrw.andypj.xyz

std::sort(v.begin(), v.end());
来源：http://kuy.fzhhl.top

[S39] C++：自定义比较器排序
来源：http://gqt.cqqwz.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://ava.iojbl.cn

[S40] C++：查找元素
来源：http://fiy.hnqzz.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://vww.vqdsnc.cn

[S41] C++：类与构造函数
来源：http://smx.chenzaomai.com

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://zyk.jyoumei.cn

[S42] C++：继承与虚函数
来源：http://rvq.vqdsnc.cn

class B : public Base { public: void f() override {} };
来源：http://knz.zhongyouzk.top

[S43] C++：智能指针
来源：http://mtw.yongpay.top

auto p = std::make_unique<int>(5);
来源：http://pul.zycfv.cn

[S44] C++：引用传参
来源：http://epg.hnxiangtu.top

void inc(int &x) { ++x; }
来源：http://fim.xuanzx.com

[S45] C++：lambda
来源：http://bnk.cucudq.cn

auto add = [](int a, int b) { return a + b; };
来源：http://agb.hnqzz.top

[S46] C++：函数模板
来源：http://yvf.gotoacloud.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://eqy.ydzc1.top

[S47] C++：结构化绑定遍历
来源：http://qlk.uphjek.com

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://txu.hfpthk.cn

[S48] C++：逐行读文件
来源：http://mpt.cashguo.top

std::ifstream in("a.txt");  std::string line;
来源：http://nhk.yanxiufei.cn

while (std::getline(in, line)) { }
来源：http://npy.feifeiyinyue.top

[S49] C++：写文件
来源：http://bod.hfpthk.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://thg.yanxiufei.cn

[S50] C++：格式化数字
来源：http://ava.andypj.xyz

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://bjt.yfazqb.com

[S51] C++：显式类型转换
来源：http://oja.dianchejie.cn

static_cast<double>(a) / b
来源：http://ylj.chenjidiqi.icu

[S52] C++：const 与 noexcept
来源：http://zoo.ybcxt.top

int size() const noexcept { return n_; }
来源：http://ejt.ywan-chungtsiang.top

[S53] C++：移动语义
来源：http://dch.9152youxi.cn

std::vector<int> w = std::move(v);
来源：http://nli.yj20258.top

[S54] C++：异常处理
来源：http://bna.hcnkem.com

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://kki.uphjek.com

[S55] C++：结构化绑定
来源：http://gvr.aibaodan.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://rsu.ivvv.top

[S56] C++：optional
来源：http://wlr.zhijiandao.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wcm.tian-w.cn

[S57] C++：编译期常量
来源：http://blr.yj20258.top

constexpr int N = 10;
来源：http://uzm.jinqigfzy.top

[S58] C++：命名空间
来源：http://hna.xuetiantiany.cn

namespace ns { int f() { return 1; } }
来源：http://cbz.tianlin.xyz

[S59] C++：静态断言
来源：http://agb.guannengcc.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://inc.fehbvm.com

[S60] C++：遍历并删除元素
来源：http://rrp.daxiang520.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://tmb.gzhubu.top

================================================================================
来源：http://crq.jinqigufen.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://yhn.zhengqikj.top

================================================================================
来源：http://zso.vehdjk.com

[T01] Kotlin：Hello World
来源：http://lgh.cqqwz.cn

println("Hello")
来源：http://mtj.ybcxt.top

[T02] Kotlin：变量
来源：http://tpg.dianchejie.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://tsj.zhaomingkeji.xyz

[T03] Kotlin：字符串模板
来源：http://hss.zhijiandao.cn

"值: $b"
来源：http://biy.kuanghao11.cn

[T04] Kotlin：空安全
来源：http://swg.jianghu66.top

val n: String? = null;  n?.length
来源：http://dgf.pengpengdd.cyou

[T05] Kotlin：when 表达式
来源：http://gps.yfazqb.com

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://ubl.yongpay.top

[T06] Kotlin：集合映射
来源：http://moh.daxiang520.top

listOf(1, 2, 3).map { it * 2 }
来源：http://dah.snrcjt.cn

[T07] Kotlin：集合过滤
来源：http://uaf.cqqwz.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://gpa.zdqjudy.top

[T08] Kotlin：数据类
来源：http://ndu.sufxvd.cn

data class User(val name: String, val age: Int)
来源：http://ctw.haohaochexian.top

[T09] Kotlin：扩展函数
来源：http://ezb.fengsongda.top

fun String.exclaim() = this + "!"
来源：http://ebd.jyoumei.cn

[T10] Kotlin：默认参数
来源：http://usu.snrcjt.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://vpy.cashguo.top

[T11] Kotlin：协程
来源：http://tae.yueranfly.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://ogb.ppjwa.cn

[T12] Kotlin：解构声明
来源：http://iac.yfazqb.com

val (a, b) = Pair(1, 2)
来源：http://htq.yueranfly.top

[T13] Kotlin：只读 Map
来源：http://ksl.ehwqpu.com

val m = mapOf("a" to 1)
来源：http://mxh.jyoumei.cn

[T14] Kotlin：循环
来源：http://fyn.nwbrower.top

for (i in 1..10) println(i)
来源：http://hcd.tanke756.top

[T15] Kotlin：接口
来源：http://zao.c1oappe.top

interface Shape { fun area(): Double }
来源：http://wbb.yangfankeji.com

[T16] Swift：Hello World
来源：http://cap.zhengqikj.top

print("Hello")
来源：http://ftw.cucudq.cn

[T17] Swift：变量与常量
来源：http://uhf.yj202588.top

var a = 1;  let b = 2
来源：http://bqu.yonumen.top

[T18] Swift：字符串插值
来源：http://ogn.wangdashe.top

"值: \(b)"
来源：http://hqf.cqqwz.cn

[T19] Swift：可选绑定
来源：http://oxn.jinyuanbaomall.cn

if let n = opt { print(n) }
来源：http://dme.yangfankeji.com

[T20] Swift：数组操作
来源：http://qzm.zhaomingkeji.xyz

var a = [1, 2, 3];  a.append(4)
来源：http://tzk.cdnleiting.top

[T21] Swift：遍历
来源：http://kmd.ydzc1.top

for x in a { print(x) }
来源：http://bjt.jqgufenzy.top

[T22] Swift：字典
来源：http://usg.jinqigfzy.top

var d = ["a": 1];  d["b"] = 2
来源：http://rvr.fanxiaobao.xyz

[T23] Swift：函数
来源：http://lfq.mhx1999.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://yrn.aibaodan.cn

[T24] Swift：闭包
来源：http://sat.ivvv.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://isd.jqgfzy.top

[T25] Swift：结构体
来源：http://kbn.zhengqikj.top

struct P { var x: Int }
来源：http://ptx.xziqi.cn

[T26] Swift：类与重写
来源：http://bsb.birdmap.top

class A: Base { override func f() {} }
来源：http://lop.yueranfly.top

[T27] Swift：错误处理
来源：http://eyo.shangyingyoupin.top

do { try f() } catch { print(error) }
来源：http://xzl.vehdjk.com

[T28] Swift：枚举
来源：http://zqm.52xcode.cn

enum Color { case red, green }
来源：http://llm.sweek.top

[T29] Swift：guard 提前返回
来源：http://rup.vehdjk.com

guard let x = opt else { return }
来源：http://tjq.jlsjyb.cn

[T30] Swift：协议
来源：http://bze.guowangkeji.top

protocol Shape { func area() -> Double }
来源：http://pkp.hongshengwenyu.top

[T31] Lua：Hello World
来源：http://cjh.jyoumei.cn

print("Hello")
来源：http://poa.uphjek.com

[T32] Lua：局部变量
来源：http://ysy.zdbjq.cn

local a = 1
来源：http://aea.pengpengdd.cyou

[T33] Lua：表（数组）
来源：http://qch.zdbjq.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://cri.gogol.net.cn

[T34] Lua：遍历表
来源：http://zmj.chenjidiqi.icu

for i, v in ipairs(t) do print(i, v) end
来源：http://nit.hesvh.cn

[T35] Lua：字典表
来源：http://ldy.jinqigfzy.top

local d = { a = 1 };  d.b = 2
来源：http://leq.316326.xyz

[T36] Lua：函数
来源：http://mrz.cheryme.top

function add(a, b) return a + b end
来源：http://bfe.yfazqb.com

[T37] Lua：字符串拼接
来源：http://gaz.nanxuanxn.top

"a" .. "b"
来源：http://ext.cashguo.top

[T38] Lua：条件
来源：http://fip.vqdsnc.cn

if x > 0 then print("正") end
来源：http://gfm.gotoacloud.top

[T39] Lua：模式匹配
来源：http://xeo.yueranfly.top

string.find(s, "%d+")
来源：http://eei.iojbl.cn

[T40] Lua：元表
来源：http://shs.pycfn.com

setmetatable({}, { __index = base })
来源：http://fsf.chenjidiqi.icu

[T41] Perl：Hello World
来源：http://fpr.hfpthk.cn

print "Hello\n";
来源：http://tpk.cheryme.top

[T42] Perl：变量类型
来源：http://nqk.zhixingplan.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://nlv.ywan-chungtsiang.top

[T43] Perl：字符串插值
来源：http://nty.bbcook.cn

"值: $a"
来源：http://alr.cheryme.top

[T44] Perl：条件
来源：http://vpl.zhiwuduotai.top

if ($a > 0) { print "正"; }
来源：http://mca.jlsjyb.cn

[T45] Perl：数组遍历
来源：http://rtr.quarkkingdee.top

for my $x (@arr) { print $x; }
来源：http://jay.guowangkeji.top

[T46] Perl：哈希操作
来源：http://kni.cashguo.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://yzm.yuanzhike.top

[T47] Perl：正则捕获
来源：http://fco.cqqwz.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://lmu.ywan-chungtsiang.top

[T48] Perl：正则替换
来源：http://zcv.shuidangran.top

$s =~ s/old/new/g;
来源：http://pzm.tarul.cn

[T49] Perl：函数
来源：http://yxz.wangdashe.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://ran.epnwcf.com

[T50] Perl：逐行读文件
来源：http://ysf.daria6918.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://wng.yonumen.top

while (my $line = <$fh>) { print $line; }
来源：http://lui.nwbrower.top

[T51] Scala：Hello World
来源：http://tkw.shanyushiyangtech.top

println("Hello")
来源：http://qeu.0kj1m.cn

[T52] Scala：变量
来源：http://exh.shzxlz.cn

val a = 1;  var b = 2
来源：http://qky.c1oappe.top

[T53] Scala：字符串插值
来源：http://hhm.shuidangran.top

s"值: $b"
来源：http://gsy.ydjk.org.cn

[T54] Scala：集合映射
来源：http://rtq.hongshengwenyu.top

List(1, 2, 3).map(_ * 2)
来源：http://ops.xuanzx.com

[T55] Scala：集合过滤
来源：http://piu.tanke756.top

List(1, 2, 3).filter(_ > 1)
来源：http://ebd.yuanzhike.top

[T56] Scala：样例类
来源：http://acd.wangshuangyany.cn

case class User(name: String, age: Int)
来源：http://jrk.zdbjq.cn

[T57] Scala：模式匹配
来源：http://wlm.sxryk.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://kwi.haohaochexian.top

[T58] Scala：函数定义
来源：http://seg.yuanzhike.top

def add(a: Int, b: Int): Int = a + b
来源：http://yjo.hysaishi.cn

[T59] Scala：循环
来源：http://kkp.yvedp.cn

for (i <- 1 to 10) println(i)
来源：http://tgh.shanyushiyangkeji.top

[T60] Scala：折叠
来源：http://awo.birdmap.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://mcp.jiagoushi.top

================================================================================
来源：http://aqo.zhiwuduotai.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://zmg.shanyushiyangkeji.top

================================================================================
来源：http://wpr.nwbrower.top

[U01] Py：创建虚拟环境
来源：http://nmf.hysaishi.cn

python -m venv .venv && source .venv/bin/activate
来源：http://csd.cashguo.top

[U02] Py：导出 / 安装依赖
来源：http://dfh.ppjwa.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://juz.shanyushiyangtech.top

[U03] Py：加载 .env 配置
来源：http://nzh.hesvh.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://kia.hcnkem.com

[U04] Py：变量调试打印
来源：http://geb.yonumen.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://svc.guannengcc.top

[U05] Py：列表去重且保序
来源：http://qim.jinqigfzy.top

list(dict.fromkeys(arr))
来源：http://izq.xinyue.icu

[U06] Py：合并两个字典
来源：http://wpt.snrcjt.cn

{**a, **b}
来源：http://oeo.xuetiantiany.cn


<!-- 参考信息 -->