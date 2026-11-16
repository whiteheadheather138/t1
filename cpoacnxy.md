代发 wailian999

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://for.sysykeji.top

[R66] 定时任务
来源：http://ypp.smart0.xyz

crontab -e;  crontab -l
来源：http://xeo.yuxming.cn

[R67] 生成随机十六进制串
来源：http://ikl.yj202588.top

openssl rand -hex 16
来源：http://lrd.smart0.xyz

[R68] 计算文件校验值
来源：http://wdy.zycfv.cn

sha256sum a.txt;  md5sum a.txt
来源：http://qzi.zycfv.cn

[R69] 生成随机密码
来源：http://aem.hywenlv.cn

head -c 16 /dev/urandom | base64
来源：http://lau.hammf.cn

[R70] 时间戳与互转
来源：http://dwo.daxiang520.top

date +%s;  date -d @1700000000
来源：http://xko.sysykeji.top

[R71] 日期格式化
来源：http://jss.guannengcc.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://stx.hysaishi.cn

[R72] 等待端口就绪
来源：http://cco.jiagoushi.top

until nc -z localhost 3306; do sleep 1; done
来源：http://gdh.wangdashe.top

[R73] 分割大日志
来源：http://pkp.guowangkeji.top

split -l 1000 big.log part_
来源：http://dge.shuidangran.top

[R74] 批量重命名
来源：http://ewh.snrcjt.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://rfu.ehwqpu.com

[R75] 导出环境变量
来源：http://rix.jinqigufen.top

export PATH="$HOME/bin:$PATH"
来源：http://hxt.svipenyu.cn

[R76] 使用临时文件
来源：http://com.jiagoushi.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://dcb.feifeiyinyue.top

[R77] 读取用户输入
来源：http://mcx.sysykeji.top

read -rp "请输入: " ans
来源：http://nzl.hesvh.cn

[R78] 交互式菜单
来源：http://pfu.gotoacloud.top

select opt in a b c; do echo "$opt"; break; done
来源：http://sgb.jinyuanbaomall.cn

[R79] 解析命令行选项
来源：http://vab.guowangkeji.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://ame.9152youxi.cn

[R80] 查看脚本执行耗时
来源：http://nmg.jyoumei.cn

time ./run.sh
来源：http://jax.yfazqb.com

================================================================================
来源：http://qid.jinyuanbaomall.cn

S. C / C++ 专题
来源：http://hns.ywan-chungtsiang.top

================================================================================
来源：http://ngu.wangdashe.top

[S01] C：Hello World
来源：http://gzv.ehwqpu.com

#include <stdio.h>
来源：http://sij.jlsjyb.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://ctv.zhiwuduotai.top

[S02] C：变量与格式化输出
来源：http://guo.yj202588.top

int a = 10; printf("%d\n", a);
来源：http://sxx.daxiang520.top

[S03] C：读入整数
来源：http://mas.shanyushiyangkeji.top

int x; scanf("%d", &x);
来源：http://vxm.yangfankeji.com

[S04] C：字符串复制
来源：http://kuc.guowangkeji.top

char dst[32]; strcpy(dst, "hi");
来源：http://arj.yvedp.cn

[S05] C：字符串长度
来源：http://bum.jqgfzy.top

strlen(s)
来源：http://lss.chenlongwang.top

[S06] C：字符串比较
来源：http://kse.zhengqikj.top

strcmp(a, b) == 0
来源：http://pak.ehwqpu.com

[S07] C：数组遍历求和
来源：http://wje.0kj1m.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://xiy.guowangkeji.top

[S08] C：动态内存分配与释放
来源：http://ftp.zhijiandao.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://ztt.9152youxi.cn

[S09] C：结构体定义与初始化
来源：http://bll.hywenlv.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://gix.ivvv.top

[S10] C：指针与解引用
来源：http://yai.jinghuilouyu.cn

int *p = &a;  *p = 5;
来源：http://cse.tian-w.cn

[S11] C：逐行读文件
来源：http://rtk.zdqjudy.top

FILE *f = fopen("a.txt", "r");
来源：http://klh.zdbjq.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://lwj.hysaishi.cn

fclose(f);
来源：http://rgl.cqqwz.cn

[S12] C：写文件
来源：http://reh.zhongyouzk.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://rna.xuetiantiany.cn

[S13] C：宏定义
来源：http://tyh.hcnkem.com

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wpa.fktsv.cn

[S14] C：枚举
来源：http://ake.hcnkem.com

enum Color { RED, GREEN, BLUE };
来源：http://txo.shzxlz.cn

[S15] C：类型转换
来源：http://qiw.hesvh.cn

(double) a / b
来源：http://ikl.shanyushiyangkeji.top

[S16] C：位操作置位
来源：http://snu.tianlin.xyz

x |= (1 << 3);
来源：http://uaa.wangdashe.top

[S17] C：安全拼接字符串
来源：http://sdr.kuanghao11.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://pjk.hfpthk.cn

[S18] C：命令行参数
来源：http://pbt.jinghuilouyu.cn

int main(int argc, char **argv)
来源：http://ljm.yangfankeji.com

[S19] C：快速排序
来源：http://ywh.quarkkingdee.top

qsort(a, n, sizeof(int), cmp);
来源：http://ewc.guannengcc.top

[S20] C：二分查找
来源：http://tzj.meibo888.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://ikg.cdnleiting.top

[S21] C：字符类别判断
来源：http://ixy.nanxuanxn.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://moi.hysaishi.cn

[S22] C：字符串转数字
来源：http://fia.hysaishi.cn

atoi("42");  strtod("3.14", NULL);
来源：http://pdw.zhongyouzk.top

[S23] C：随机数
来源：http://dgc.uphjek.com

srand(time(NULL));  int r = rand() % 100;
来源：http://okv.xylfe.cn

[S24] C：获取本地时间
来源：http://mvy.yongpay.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://tiz.xinyue.icu

[S25] C：内存拷贝
来源：http://uge.jqgfzy.top

memcpy(dst, src, n);
来源：http://epw.guowangkeji.top

[S26] C：内存清零
来源：http://sfs.yj202588.top

memset(a, 0, sizeof a);
来源：http://zgp.smart0.xyz

[S27] C：定义常量
来源：http://ury.hysaishi.cn

const double PI = 3.14159;
来源：http://lpc.gotoacloud.top

[S28] C：静态变量
来源：http://wed.zycfv.cn

static int counter = 0;
来源：http://vrk.cqqwz.cn

[S29] C：变参函数
来源：http://fpg.ydzc1.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://lgk.0kj1m.cn

[S30] C：头文件保护
来源：http://rol.xuetiantiany.cn

#ifndef X_H
来源：http://nfb.pengpengdd.cyou

#define X_H
来源：http://ksf.aibaodan.cn

#endif
来源：http://ije.fengsongda.top

[S31] C++：Hello World
来源：http://liy.xziqi.cn

#include <iostream>
来源：http://pou.yj20258888.top

int main() { std::cout << "Hello\n"; }
来源：http://jmn.fehbvm.com

[S32] C++：字符串
来源：http://rlg.daxiang520.top

std::string s = "hi";  s += "!";
来源：http://mjj.ydzc1.top

[S33] C++：vector 增删
来源：http://apl.mhx1999.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://coi.redwolf501.top

[S34] C++：遍历 vector
来源：http://xiu.zhijiandao.cn

for (auto &x : v) { std::cout << x; }
来源：http://slr.shuidangran.top

[S35] C++：map
来源：http://qsm.jyoumei.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://foe.sysykeji.top

[S36] C++：unordered_map
来源：http://agl.tarul.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://pmn.shuidangran.top

[S37] C++：set
来源：http://qkt.nanxinkj.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://anj.zhixingplan.top

[S38] C++：排序
来源：http://jmx.zdqjudy.top

std::sort(v.begin(), v.end());
来源：http://hvs.havefunace.top

[S39] C++：自定义比较器排序
来源：http://wlt.chenlongwang.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://kog.yanxiufei.cn

[S40] C++：查找元素
来源：http://faw.jyoumei.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://aei.yvedp.cn

[S41] C++：类与构造函数
来源：http://coe.smart0.xyz

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://owj.zhoulong.xyz

[S42] C++：继承与虚函数
来源：http://rjy.gotoacloud.top

class B : public Base { public: void f() override {} };
来源：http://zuv.yfazqb.com

[S43] C++：智能指针
来源：http://avu.shanyushiyangtech.top

auto p = std::make_unique<int>(5);
来源：http://ujb.pengpengdd.cyou

[S44] C++：引用传参
来源：http://fqj.hesvh.cn

void inc(int &x) { ++x; }
来源：http://xre.jianghu66.top

[S45] C++：lambda
来源：http://eeb.jianghu66.top

auto add = [](int a, int b) { return a + b; };
来源：http://gwe.shanyushiyangtech.top

[S46] C++：函数模板
来源：http://uwc.jqgfzy.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://yvk.chenzaomai.com

[S47] C++：结构化绑定遍历
来源：http://nbt.hywenlv.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://buj.feifeiyinyue.top

[S48] C++：逐行读文件
来源：http://yui.cqqwz.cn

std::ifstream in("a.txt");  std::string line;
来源：http://slt.ywan-chungtsiang.top

while (std::getline(in, line)) { }
来源：http://xum.jlsjyb.cn

[S49] C++：写文件
来源：http://pio.yvedp.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://eov.snrcjt.cn

[S50] C++：格式化数字
来源：http://mro.hcnkem.com

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://twy.cqqwz.cn

[S51] C++：显式类型转换
来源：http://dso.xinyue.icu

static_cast<double>(a) / b
来源：http://otn.nwbrower.top

[S52] C++：const 与 noexcept
来源：http://fcx.shuidangran.top

int size() const noexcept { return n_; }
来源：http://pqw.yj20258.top

[S53] C++：移动语义
来源：http://xfu.vqdsnc.cn

std::vector<int> w = std::move(v);
来源：http://zvn.zhengqikj.top

[S54] C++：异常处理
来源：http://qbf.iojbl.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://wmh.fanxiaobao.xyz

[S55] C++：结构化绑定
来源：http://zop.guannengcc.top

auto [a, b] = std::make_pair(1, 2);
来源：http://jri.xingfuxueyuan.xyz

[S56] C++：optional
来源：http://mzz.tanke756.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://rlo.aibaodan.cn

[S57] C++：编译期常量
来源：http://ghf.316326.xyz

constexpr int N = 10;
来源：http://vbs.jqgufenzy.top

[S58] C++：命名空间
来源：http://xhh.yonumen.top

namespace ns { int f() { return 1; } }
来源：http://she.xingfuxueyuan.xyz

[S59] C++：静态断言
来源：http://lpb.bbcook.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://jtv.fanxiaobao.xyz

[S60] C++：遍历并删除元素
来源：http://xkv.epnwcf.com

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://obb.zycfv.cn

================================================================================
来源：http://dlh.gogol.net.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://rxh.chenlongwang.top

================================================================================
来源：http://pbk.vqdsnc.cn

[T01] Kotlin：Hello World
来源：http://yfr.shzxlz.cn

println("Hello")
来源：http://dpw.cqqwz.cn

[T02] Kotlin：变量
来源：http://jkq.xziqi.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://icr.bbcook.cn

[T03] Kotlin：字符串模板
来源：http://mst.yvedp.cn

"值: $b"
来源：http://kxl.sweek.top

[T04] Kotlin：空安全
来源：http://oal.xuanzx.com

val n: String? = null;  n?.length
来源：http://cxn.gogol.net.cn

[T05] Kotlin：when 表达式
来源：http://hyl.zhoulong.xyz

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://fkr.sjlbkw.cn

[T06] Kotlin：集合映射
来源：http://nyp.jyoumei.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://zml.yfazqb.com

[T07] Kotlin：集合过滤
来源：http://jvy.0kj1m.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://wky.gzhubu.top

[T08] Kotlin：数据类
来源：http://keb.andypj.xyz

data class User(val name: String, val age: Int)
来源：http://dtp.cqqwz.cn

[T09] Kotlin：扩展函数
来源：http://oop.jiagoushi.top

fun String.exclaim() = this + "!"
来源：http://oen.svipenyu.cn

[T10] Kotlin：默认参数
来源：http://fdu.tian-w.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://icw.jianghu66.top

[T11] Kotlin：协程
来源：http://zjs.52xcode.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://bcz.xziqi.cn

[T12] Kotlin：解构声明
来源：http://xzf.tianlin.xyz

val (a, b) = Pair(1, 2)
来源：http://nqp.vqdsnc.cn

[T13] Kotlin：只读 Map
来源：http://zoa.yfazqb.com

val m = mapOf("a" to 1)
来源：http://yap.feifeiyinyue.top

[T14] Kotlin：循环
来源：http://fcp.mhx1999.top

for (i in 1..10) println(i)
来源：http://tbl.xingfuxueyuan.xyz

[T15] Kotlin：接口
来源：http://zkb.kuanghao11.cn

interface Shape { fun area(): Double }
来源：http://jvb.jiagoushi.top

[T16] Swift：Hello World
来源：http://pig.shanyushiyangtech.top

print("Hello")
来源：http://blb.wangdashe.top

[T17] Swift：变量与常量
来源：http://vvf.andypj.xyz

var a = 1;  let b = 2
来源：http://zfw.nanxuanxn.top

[T18] Swift：字符串插值
来源：http://sjt.smart0.xyz

"值: \(b)"
来源：http://rqt.bbcook.cn

[T19] Swift：可选绑定
来源：http://llo.jqgfzy.top

if let n = opt { print(n) }
来源：http://hgb.yuxming.cn

[T20] Swift：数组操作
来源：http://qlv.yvedp.cn

var a = [1, 2, 3];  a.append(4)
来源：http://wbg.guowangkeji.top

[T21] Swift：遍历
来源：http://nxb.yj20258.top

for x in a { print(x) }
来源：http://fdc.mhx1999.top

[T22] Swift：字典
来源：http://rux.jlsjyb.cn

var d = ["a": 1];  d["b"] = 2
来源：http://cys.shangyingyoupin.top

[T23] Swift：函数
来源：http://oqr.316326.xyz

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://iqd.andypj.xyz

[T24] Swift：闭包
来源：http://sdp.kuanghao11.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://nun.sufxvd.cn

[T25] Swift：结构体
来源：http://cxe.gotoacloud.top

struct P { var x: Int }
来源：http://jsc.shangyingyoupin.top

[T26] Swift：类与重写
来源：http://flw.yueranfly.top

class A: Base { override func f() {} }
来源：http://ppa.sysykeji.top

[T27] Swift：错误处理
来源：http://chx.iojbl.cn

do { try f() } catch { print(error) }
来源：http://jbw.gzhubu.top

[T28] Swift：枚举
来源：http://arb.fehbvm.com

enum Color { case red, green }
来源：http://fph.tian-w.cn

[T29] Swift：guard 提前返回
来源：http://sxw.yueranfly.top

guard let x = opt else { return }
来源：http://mhi.chenlongwang.top

[T30] Swift：协议
来源：http://ikg.ywan-chungtsiang.top

protocol Shape { func area() -> Double }
来源：http://dhr.hesvh.cn

[T31] Lua：Hello World
来源：http://dia.yuxming.cn

print("Hello")
来源：http://whm.xylfe.cn

[T32] Lua：局部变量
来源：http://leu.havefunace.top

local a = 1
来源：http://ggu.ydjk.org.cn

[T33] Lua：表（数组）
来源：http://fap.yangfankeji.com

local t = {1, 2, 3};  t[4] = 4
来源：http://bbt.snrcjt.cn

[T34] Lua：遍历表
来源：http://bvz.yuxming.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://zih.aizwys.cn

[T35] Lua：字典表
来源：http://ibi.sysykeji.top

local d = { a = 1 };  d.b = 2
来源：http://abd.sxryk.cn

[T36] Lua：函数
来源：http://wkj.kuanghao11.cn

function add(a, b) return a + b end
来源：http://arz.sxryk.cn

[T37] Lua：字符串拼接
来源：http://pwf.zhijiandao.cn

"a" .. "b"
来源：http://gce.cdnleiting.top

[T38] Lua：条件
来源：http://gwf.yonumen.top

if x > 0 then print("正") end
来源：http://tdp.ctjpmb.com

[T39] Lua：模式匹配
来源：http://feb.ydjk.org.cn

string.find(s, "%d+")
来源：http://hkx.dashuyun.cn

[T40] Lua：元表
来源：http://uzu.ywan-chungtsiang.top

setmetatable({}, { __index = base })
来源：http://uud.wangdashe.top

[T41] Perl：Hello World
来源：http://vax.chenjidiqi.icu

print "Hello\n";
来源：http://oqw.hongshengwenyu.top

[T42] Perl：变量类型
来源：http://aqz.zhijiandao.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://obo.jlsjyb.cn

[T43] Perl：字符串插值
来源：http://kby.zhaomingkeji.xyz

"值: $a"
来源：http://akc.ctjpmb.com

[T44] Perl：条件
来源：http://bub.vehdjk.com

if ($a > 0) { print "正"; }
来源：http://bul.zdqjudy.top

[T45] Perl：数组遍历
来源：http://hcj.meibo888.top

for my $x (@arr) { print $x; }
来源：http://pmv.gzhubu.top

[T46] Perl：哈希操作
来源：http://oda.hywenlv.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://aoa.shangyingyoupin.top

[T47] Perl：正则捕获
来源：http://xxi.yuxming.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://hqb.gaohongyu789.top

[T48] Perl：正则替换
来源：http://zfg.yuanzhike.top

$s =~ s/old/new/g;
来源：http://rza.cdnleiting.top

[T49] Perl：函数
来源：http://afq.zdbjq.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://wko.xziqi.cn

[T50] Perl：逐行读文件
来源：http://slz.cheryme.top

open my $fh, "<", "a.txt" or die $!;
来源：http://ibh.zycfv.cn

while (my $line = <$fh>) { print $line; }
来源：http://nkd.mhx1999.top

[T51] Scala：Hello World
来源：http://kcx.bbcook.cn

println("Hello")
来源：http://jfq.sjlbkw.cn

[T52] Scala：变量
来源：http://uau.fengsongda.top

val a = 1;  var b = 2
来源：http://hqv.sysykeji.top

[T53] Scala：字符串插值
来源：http://fia.jinqigufen.top

s"值: $b"
来源：http://ome.smart0.xyz

[T54] Scala：集合映射
来源：http://tqg.bjfxy.top

List(1, 2, 3).map(_ * 2)
来源：http://swi.guannengcc.top

[T55] Scala：集合过滤
来源：http://ygw.tarul.cn

List(1, 2, 3).filter(_ > 1)
来源：http://pbo.yfazqb.com

[T56] Scala：样例类
来源：http://iip.pycfn.com

case class User(name: String, age: Int)
来源：http://nde.cqqwz.cn

[T57] Scala：模式匹配
来源：http://vzw.0kj1m.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://nsa.cashguo.top

[T58] Scala：函数定义
来源：http://maa.ppjwa.cn

def add(a: Int, b: Int): Int = a + b
来源：http://ora.fktsv.cn

[T59] Scala：循环
来源：http://dog.hfpthk.cn

for (i <- 1 to 10) println(i)
来源：http://hdw.xuanzx.com

[T60] Scala：折叠
来源：http://vsq.quarkkingdee.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://toe.kuanghao11.cn

================================================================================
来源：http://qxr.chenjidiqi.icu

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://evs.shanyushiyangtech.top

================================================================================
来源：http://mfv.cucudq.cn

[U01] Py：创建虚拟环境
来源：http://blg.fehbvm.com

python -m venv .venv && source .venv/bin/activate
来源：http://gnb.daxiang520.top

[U02] Py：导出 / 安装依赖
来源：http://rgu.yuxming.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://dbo.zhengqikj.top

[U03] Py：加载 .env 配置
来源：http://iio.hnxiangtu.top

from dotenv import load_dotenv; load_dotenv()
来源：http://fdz.chenlongwang.top

[U04] Py：变量调试打印
来源：http://ibj.yj20258.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://wkk.cucudq.cn

[U05] Py：列表去重且保序
来源：http://vas.dashuyun.cn

list(dict.fromkeys(arr))
来源：http://lch.hongshengwenyu.top

[U06] Py：合并两个字典
来源：http://ioy.pycfn.com

{**a, **b}
来源：http://bcq.fanxiaobao.xyz


<!-- 参考信息 -->