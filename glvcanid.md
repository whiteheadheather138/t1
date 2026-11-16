代发 wailian999

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://ygg.hammf.cn

[R66] 定时任务
来源：http://ryi.0kj1m.cn

crontab -e;  crontab -l
来源：http://ias.jiagoushi.top

[R67] 生成随机十六进制串
来源：http://uhf.andypj.xyz

openssl rand -hex 16
来源：http://bgx.birdmap.top

[R68] 计算文件校验值
来源：http://kgi.zdqjudy.top

sha256sum a.txt;  md5sum a.txt
来源：http://muf.zhixingplan.top

[R69] 生成随机密码
来源：http://ejy.zhengqikj.top

head -c 16 /dev/urandom | base64
来源：http://jol.tian-w.cn

[R70] 时间戳与互转
来源：http://swe.shuidangran.top

date +%s;  date -d @1700000000
来源：http://hyr.havefunace.top

[R71] 日期格式化
来源：http://itc.ydzc1.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://zgf.cucudq.cn

[R72] 等待端口就绪
来源：http://eoa.zhoulong.xyz

until nc -z localhost 3306; do sleep 1; done
来源：http://pia.quarkkingdee.top

[R73] 分割大日志
来源：http://qpl.andypj.xyz

split -l 1000 big.log part_
来源：http://ztr.wangshuangyany.cn

[R74] 批量重命名
来源：http://orh.tanke756.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://kll.sysykeji.top

[R75] 导出环境变量
来源：http://nyn.xuanzx.com

export PATH="$HOME/bin:$PATH"
来源：http://rwf.jiagoushi.top

[R76] 使用临时文件
来源：http://xma.xuanzx.com

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://yaf.yuxming.cn

[R77] 读取用户输入
来源：http://rbo.ctjpmb.com

read -rp "请输入: " ans
来源：http://dih.iojbl.cn

[R78] 交互式菜单
来源：http://teq.vqdsnc.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://yfh.tianlin.xyz

[R79] 解析命令行选项
来源：http://gxk.hcnkem.com

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://kpy.ydzc1.top

[R80] 查看脚本执行耗时
来源：http://nwy.hfpthk.cn

time ./run.sh
来源：http://hat.9152youxi.cn

================================================================================
来源：http://lzh.havefunace.top

S. C / C++ 专题
来源：http://vcb.zdbjq.cn

================================================================================
来源：http://yle.sufxvd.cn

[S01] C：Hello World
来源：http://xip.wangdashe.top

#include <stdio.h>
来源：http://xvf.ehwqpu.com

int main(void) { printf("Hello\n"); return 0; }
来源：http://lbb.smart0.xyz

[S02] C：变量与格式化输出
来源：http://mco.dashuyun.cn

int a = 10; printf("%d\n", a);
来源：http://mat.mhx1999.top

[S03] C：读入整数
来源：http://wfk.zdbjq.cn

int x; scanf("%d", &x);
来源：http://tyv.sxryk.cn

[S04] C：字符串复制
来源：http://fdc.zycfv.cn

char dst[32]; strcpy(dst, "hi");
来源：http://efk.quarkkingdee.top

[S05] C：字符串长度
来源：http://fhf.zhiwuduotai.top

strlen(s)
来源：http://blo.zhongyouzk.top

[S06] C：字符串比较
来源：http://rzc.iojbl.cn

strcmp(a, b) == 0
来源：http://frj.hesvh.cn

[S07] C：数组遍历求和
来源：http://aex.fktsv.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://kwu.wangdashe.top

[S08] C：动态内存分配与释放
来源：http://eie.yj20258888.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://dvh.hywenlv.cn

[S09] C：结构体定义与初始化
来源：http://avr.jinyuanbaomall.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://jwe.hongshengwenyu.top

[S10] C：指针与解引用
来源：http://phn.0kj1m.cn

int *p = &a;  *p = 5;
来源：http://npu.uphjek.com

[S11] C：逐行读文件
来源：http://nmi.gzhubu.top

FILE *f = fopen("a.txt", "r");
来源：http://kfp.mhx1999.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://jku.zhiwuduotai.top

fclose(f);
来源：http://oow.cdnleiting.top

[S12] C：写文件
来源：http://kkx.zdbjq.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://qta.shanyushiyangkeji.top

[S13] C：宏定义
来源：http://sqa.havefunace.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://xez.dashuyun.cn

[S14] C：枚举
来源：http://gvc.sweek.top

enum Color { RED, GREEN, BLUE };
来源：http://esq.havefunace.top

[S15] C：类型转换
来源：http://nxi.zdbjq.cn

(double) a / b
来源：http://zyl.xuetiantiany.cn

[S16] C：位操作置位
来源：http://kjt.shzxlz.cn

x |= (1 << 3);
来源：http://okm.fengsongda.top

[S17] C：安全拼接字符串
来源：http://pnu.tanke756.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://moy.jqgufenzy.top

[S18] C：命令行参数
来源：http://ceu.cdnleiting.top

int main(int argc, char **argv)
来源：http://qjs.52xcode.cn

[S19] C：快速排序
来源：http://swc.jqgufenzy.top

qsort(a, n, sizeof(int), cmp);
来源：http://zig.fanxiaobao.xyz

[S20] C：二分查找
来源：http://jyw.yuanzhike.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://uqx.zhiwuduotai.top

[S21] C：字符类别判断
来源：http://ouy.yuanzhike.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://wfj.bbcook.cn

[S22] C：字符串转数字
来源：http://umg.shzxlz.cn

atoi("42");  strtod("3.14", NULL);
来源：http://zqn.zdbjq.cn

[S23] C：随机数
来源：http://gli.zdbjq.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://jxb.yj20258888.top

[S24] C：获取本地时间
来源：http://mql.tian-w.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://msm.jqgufenzy.top

[S25] C：内存拷贝
来源：http://lfj.jinghuilouyu.cn

memcpy(dst, src, n);
来源：http://zpr.cashguo.top

[S26] C：内存清零
来源：http://cja.jqgfzy.top

memset(a, 0, sizeof a);
来源：http://xih.sysykeji.top

[S27] C：定义常量
来源：http://ucy.zhiwuduotai.top

const double PI = 3.14159;
来源：http://dnj.jqgufenzy.top

[S28] C：静态变量
来源：http://gsp.cqqwz.cn

static int counter = 0;
来源：http://upo.yueranfly.top

[S29] C：变参函数
来源：http://ffh.bjfxy.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://kyc.cucudq.cn

[S30] C：头文件保护
来源：http://dla.jinghuilouyu.cn

#ifndef X_H
来源：http://gwp.bbcook.cn

#define X_H
来源：http://xyt.sweek.top

#endif
来源：http://omi.sweek.top

[S31] C++：Hello World
来源：http://dif.uphjek.com

#include <iostream>
来源：http://eop.ywan-chungtsiang.top

int main() { std::cout << "Hello\n"; }
来源：http://tdb.yuxming.cn

[S32] C++：字符串
来源：http://lul.gotoacloud.top

std::string s = "hi";  s += "!";
来源：http://bal.yfazqb.com

[S33] C++：vector 增删
来源：http://asm.jqgfzy.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://unc.9152youxi.cn

[S34] C++：遍历 vector
来源：http://lbc.ppjwa.cn

for (auto &x : v) { std::cout << x; }
来源：http://cgt.hammf.cn

[S35] C++：map
来源：http://tze.zdqjudy.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://ujl.cdnleiting.top

[S36] C++：unordered_map
来源：http://lik.dashuyun.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://ssf.nwbrower.top

[S37] C++：set
来源：http://wat.jiagoushi.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://zvk.zhixingplan.top

[S38] C++：排序
来源：http://mpx.gaohongyu789.top

std::sort(v.begin(), v.end());
来源：http://pty.hfpthk.cn

[S39] C++：自定义比较器排序
来源：http://gdr.fengsongda.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://cpo.sufxvd.cn

[S40] C++：查找元素
来源：http://ser.shangyingyoupin.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://cev.daria6918.cn

[S41] C++：类与构造函数
来源：http://sbs.sysykeji.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hbh.cheryme.top

[S42] C++：继承与虚函数
来源：http://iaj.snrcjt.cn

class B : public Base { public: void f() override {} };
来源：http://enl.cashguo.top

[S43] C++：智能指针
来源：http://mjk.zycfv.cn

auto p = std::make_unique<int>(5);
来源：http://pnp.vehdjk.com

[S44] C++：引用传参
来源：http://qrt.nanxuanxn.top

void inc(int &x) { ++x; }
来源：http://jqc.jinqigufen.top

[S45] C++：lambda
来源：http://oly.zhiwuduotai.top

auto add = [](int a, int b) { return a + b; };
来源：http://ncj.zhaomingkeji.xyz

[S46] C++：函数模板
来源：http://yuw.xuetiantiany.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://jpj.shzxlz.cn

[S47] C++：结构化绑定遍历
来源：http://ykn.mhx1999.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://ept.xuetiantiany.cn

[S48] C++：逐行读文件
来源：http://cwe.yonumen.top

std::ifstream in("a.txt");  std::string line;
来源：http://yua.yvedp.cn

while (std::getline(in, line)) { }
来源：http://fuu.svipenyu.cn

[S49] C++：写文件
来源：http://msz.tanke756.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://xwv.quarkkingdee.top

[S50] C++：格式化数字
来源：http://yjd.zhiwuduotai.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://kcg.dianchejie.cn

[S51] C++：显式类型转换
来源：http://ikt.cqqwz.cn

static_cast<double>(a) / b
来源：http://iuo.hammf.cn

[S52] C++：const 与 noexcept
来源：http://vki.0kj1m.cn

int size() const noexcept { return n_; }
来源：http://abm.birdmap.top

[S53] C++：移动语义
来源：http://voc.zdbjq.cn

std::vector<int> w = std::move(v);
来源：http://mpr.cdnleiting.top

[S54] C++：异常处理
来源：http://upf.andypj.xyz

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://rym.svipenyu.cn

[S55] C++：结构化绑定
来源：http://kzb.c1oappe.top

auto [a, b] = std::make_pair(1, 2);
来源：http://rqv.c1oappe.top

[S56] C++：optional
来源：http://fgu.zhaomingkeji.xyz

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://zoj.zhiwuduotai.top

[S57] C++：编译期常量
来源：http://jyk.zhongyouzk.top

constexpr int N = 10;
来源：http://sot.vehdjk.com

[S58] C++：命名空间
来源：http://ngv.chenlongwang.top

namespace ns { int f() { return 1; } }
来源：http://hle.fktsv.cn

[S59] C++：静态断言
来源：http://sxf.shanyushiyangkeji.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://lcp.jinqigfzy.top

[S60] C++：遍历并删除元素
来源：http://uno.yonumen.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://yia.zdbjq.cn

================================================================================
来源：http://hyk.havefunace.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://kuz.316326.xyz

================================================================================
来源：http://sbt.nwbrower.top

[T01] Kotlin：Hello World
来源：http://hln.yj202588.top

println("Hello")
来源：http://zbf.bbcook.cn

[T02] Kotlin：变量
来源：http://fnu.aizwys.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://ozt.zdbjq.cn

[T03] Kotlin：字符串模板
来源：http://wlr.nanxinkj.top

"值: $b"
来源：http://zgm.yuanzhike.top

[T04] Kotlin：空安全
来源：http://uah.xylfe.cn

val n: String? = null;  n?.length
来源：http://jqn.sjlbkw.cn

[T05] Kotlin：when 表达式
来源：http://dyv.cheryme.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://eqm.sjlbkw.cn

[T06] Kotlin：集合映射
来源：http://mst.gotoacloud.top

listOf(1, 2, 3).map { it * 2 }
来源：http://zvz.fengsongda.top

[T07] Kotlin：集合过滤
来源：http://idt.9152youxi.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://yiy.ctjpmb.com

[T08] Kotlin：数据类
来源：http://lha.zhongyouzk.top

data class User(val name: String, val age: Int)
来源：http://kpi.guannengcc.top

[T09] Kotlin：扩展函数
来源：http://cbi.nanxinkj.top

fun String.exclaim() = this + "!"
来源：http://rsp.ybcxt.top

[T10] Kotlin：默认参数
来源：http://gbf.dianchejie.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://lcy.0kj1m.cn

[T11] Kotlin：协程
来源：http://mvp.wangdashe.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://oze.jiagoushi.top

[T12] Kotlin：解构声明
来源：http://yea.fehbvm.com

val (a, b) = Pair(1, 2)
来源：http://phm.zdqjudy.top

[T13] Kotlin：只读 Map
来源：http://qko.aizwys.cn

val m = mapOf("a" to 1)
来源：http://uun.hfpthk.cn

[T14] Kotlin：循环
来源：http://ngr.cdnleiting.top

for (i in 1..10) println(i)
来源：http://drv.vehdjk.com

[T15] Kotlin：接口
来源：http://fcd.sjlbkw.cn

interface Shape { fun area(): Double }
来源：http://qex.yuanzhike.top

[T16] Swift：Hello World
来源：http://bes.zdqjudy.top

print("Hello")
来源：http://iuw.hysaishi.cn

[T17] Swift：变量与常量
来源：http://mrt.pycfn.com

var a = 1;  let b = 2
来源：http://ztg.shzxlz.cn

[T18] Swift：字符串插值
来源：http://cne.hnqzz.top

"值: \(b)"
来源：http://gqp.smart0.xyz

[T19] Swift：可选绑定
来源：http://uua.ydjk.org.cn

if let n = opt { print(n) }
来源：http://xka.hnqzz.top

[T20] Swift：数组操作
来源：http://kws.yuanzhike.top

var a = [1, 2, 3];  a.append(4)
来源：http://buu.snrcjt.cn

[T21] Swift：遍历
来源：http://lif.tianlin.xyz

for x in a { print(x) }
来源：http://ffr.pengpengdd.cyou

[T22] Swift：字典
来源：http://dzx.iojbl.cn

var d = ["a": 1];  d["b"] = 2
来源：http://chq.sjlbkw.cn

[T23] Swift：函数
来源：http://zan.sweek.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://qny.mhx1999.top

[T24] Swift：闭包
来源：http://kdl.sjlbkw.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://qck.hfpthk.cn

[T25] Swift：结构体
来源：http://yjp.zhaomingkeji.xyz

struct P { var x: Int }
来源：http://cnt.zhixingplan.top

[T26] Swift：类与重写
来源：http://zwf.zhiwuduotai.top

class A: Base { override func f() {} }
来源：http://rnm.xylfe.cn

[T27] Swift：错误处理
来源：http://eok.ctjpmb.com

do { try f() } catch { print(error) }
来源：http://ibr.chenzaomai.com

[T28] Swift：枚举
来源：http://yzr.zhongyouzk.top

enum Color { case red, green }
来源：http://lvm.chenjidiqi.icu

[T29] Swift：guard 提前返回
来源：http://kld.aizwys.cn

guard let x = opt else { return }
来源：http://tnt.snrcjt.cn

[T30] Swift：协议
来源：http://yir.jlsjyb.cn

protocol Shape { func area() -> Double }
来源：http://llv.hnqzz.top

[T31] Lua：Hello World
来源：http://hen.yangfankeji.com

print("Hello")
来源：http://frh.gzhubu.top

[T32] Lua：局部变量
来源：http://crc.wangdashe.top

local a = 1
来源：http://dic.epnwcf.com

[T33] Lua：表（数组）
来源：http://iba.aizwys.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://tcd.sxryk.cn

[T34] Lua：遍历表
来源：http://cjs.tarul.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://gss.sysykeji.top

[T35] Lua：字典表
来源：http://fjx.snrcjt.cn

local d = { a = 1 };  d.b = 2
来源：http://rwz.jinghuilouyu.cn

[T36] Lua：函数
来源：http://lca.kuanghao11.cn

function add(a, b) return a + b end
来源：http://heh.jinghuilouyu.cn

[T37] Lua：字符串拼接
来源：http://hzl.dianchejie.cn

"a" .. "b"
来源：http://tny.aibaodan.cn

[T38] Lua：条件
来源：http://dun.zdqjudy.top

if x > 0 then print("正") end
来源：http://roh.jiagoushi.top

[T39] Lua：模式匹配
来源：http://hoa.dashuyun.cn

string.find(s, "%d+")
来源：http://mpw.havefunace.top

[T40] Lua：元表
来源：http://xno.guowangkeji.top

setmetatable({}, { __index = base })
来源：http://crp.tanke756.top

[T41] Perl：Hello World
来源：http://yeu.jiagoushi.top

print "Hello\n";
来源：http://tqr.ctjpmb.com

[T42] Perl：变量类型
来源：http://qds.yfazqb.com

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://thw.zhijiandao.cn

[T43] Perl：字符串插值
来源：http://zmc.kuanghao11.cn

"值: $a"
来源：http://nup.shzxlz.cn

[T44] Perl：条件
来源：http://rjx.jinqigufen.top

if ($a > 0) { print "正"; }
来源：http://xmp.mhx1999.top

[T45] Perl：数组遍历
来源：http://lzr.jianghu66.top

for my $x (@arr) { print $x; }
来源：http://mnt.cheryme.top

[T46] Perl：哈希操作
来源：http://ewv.chenlongwang.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://byk.gotoacloud.top

[T47] Perl：正则捕获
来源：http://euf.jqgfzy.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://dnu.cqqwz.cn

[T48] Perl：正则替换
来源：http://kse.xuetiantiany.cn

$s =~ s/old/new/g;
来源：http://ajv.yj20258.top

[T49] Perl：函数
来源：http://ekb.jinghuilouyu.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://lst.hammf.cn

[T50] Perl：逐行读文件
来源：http://mne.feifeiyinyue.top

open my $fh, "<", "a.txt" or die $!;
来源：http://hph.smart0.xyz

while (my $line = <$fh>) { print $line; }
来源：http://jpr.feifeiyinyue.top

[T51] Scala：Hello World
来源：http://mav.zycfv.cn

println("Hello")
来源：http://lyq.zdqjudy.top

[T52] Scala：变量
来源：http://lmk.nwbrower.top

val a = 1;  var b = 2
来源：http://dci.jianghu66.top

[T53] Scala：字符串插值
来源：http://fph.yvedp.cn

s"值: $b"
来源：http://vpj.0kj1m.cn

[T54] Scala：集合映射
来源：http://fhu.fanxiaobao.xyz

List(1, 2, 3).map(_ * 2)
来源：http://zlq.aizwys.cn

[T55] Scala：集合过滤
来源：http://uiu.hfpthk.cn

List(1, 2, 3).filter(_ > 1)
来源：http://bsp.hysaishi.cn

[T56] Scala：样例类
来源：http://eyd.uphjek.com

case class User(name: String, age: Int)
来源：http://yoj.zhixingplan.top

[T57] Scala：模式匹配
来源：http://eux.smart0.xyz

x match { case 1 => "一"; case _ => "其他" }
来源：http://ytz.xylfe.cn

[T58] Scala：函数定义
来源：http://trj.meibo888.top

def add(a: Int, b: Int): Int = a + b
来源：http://uxc.yj20258888.top

[T59] Scala：循环
来源：http://ser.smart0.xyz

for (i <- 1 to 10) println(i)
来源：http://wsg.ctjpmb.com

[T60] Scala：折叠
来源：http://mci.svipenyu.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://aax.xziqi.cn

================================================================================
来源：http://sze.chenzaomai.com

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://jhg.vqdsnc.cn

================================================================================
来源：http://afz.fengsongda.top

[U01] Py：创建虚拟环境
来源：http://zsl.dashuyun.cn

python -m venv .venv && source .venv/bin/activate
来源：http://mql.yuxming.cn

[U02] Py：导出 / 安装依赖
来源：http://kvv.shuidangran.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://qjq.yuxming.cn

[U03] Py：加载 .env 配置
来源：http://pcm.yvedp.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://tos.xylfe.cn

[U04] Py：变量调试打印
来源：http://hzn.fanxiaobao.xyz

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://sqm.daria6918.cn

[U05] Py：列表去重且保序
来源：http://btf.mhx1999.top

list(dict.fromkeys(arr))
来源：http://zoe.9152youxi.cn

[U06] Py：合并两个字典
来源：http://mrc.pycfn.com

{**a, **b}
来源：http://lrk.guannengcc.top


<!-- 参考信息 -->