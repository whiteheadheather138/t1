代发 wailian999

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://nez.zhoulong.xyz

[R66] 定时任务
来源：http://cgt.shuidangran.top

crontab -e;  crontab -l
来源：http://evo.vehdjk.com

[R67] 生成随机十六进制串
来源：http://spd.ydjk.org.cn

openssl rand -hex 16
来源：http://bkj.andypj.xyz

[R68] 计算文件校验值
来源：http://vys.ppjwa.cn

sha256sum a.txt;  md5sum a.txt
来源：http://rag.chenjidiqi.icu

[R69] 生成随机密码
来源：http://vat.jinghuilouyu.cn

head -c 16 /dev/urandom | base64
来源：http://btb.chenzaomai.com

[R70] 时间戳与互转
来源：http://hcq.fehbvm.com

date +%s;  date -d @1700000000
来源：http://iri.chenzaomai.com

[R71] 日期格式化
来源：http://wiq.ydjk.org.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://avy.shanyushiyangkeji.top

[R72] 等待端口就绪
来源：http://pxm.ydjk.org.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://mvk.wangshuangyany.cn

[R73] 分割大日志
来源：http://cch.cqqwz.cn

split -l 1000 big.log part_
来源：http://gdu.yuanzhike.top

[R74] 批量重命名
来源：http://ywn.zhengqikj.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://zcz.zycfv.cn

[R75] 导出环境变量
来源：http://pln.gotoacloud.top

export PATH="$HOME/bin:$PATH"
来源：http://aqn.uphjek.com

[R76] 使用临时文件
来源：http://uru.gaohongyu789.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://uok.yongpay.top

[R77] 读取用户输入
来源：http://xar.iojbl.cn

read -rp "请输入: " ans
来源：http://wgt.fengsongda.top

[R78] 交互式菜单
来源：http://rre.cucudq.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://zix.yfazqb.com

[R79] 解析命令行选项
来源：http://ohu.hcnkem.com

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://qfw.iojbl.cn

[R80] 查看脚本执行耗时
来源：http://bhj.yueranfly.top

time ./run.sh
来源：http://kfg.haohaochexian.top

================================================================================
来源：http://abw.shzxlz.cn

S. C / C++ 专题
来源：http://wnx.yuanzhike.top

================================================================================
来源：http://dni.ybcxt.top

[S01] C：Hello World
来源：http://rzn.xuetiantiany.cn

#include <stdio.h>
来源：http://lfu.vehdjk.com

int main(void) { printf("Hello\n"); return 0; }
来源：http://zbu.fehbvm.com

[S02] C：变量与格式化输出
来源：http://aph.tianlin.xyz

int a = 10; printf("%d\n", a);
来源：http://jgz.yuxming.cn

[S03] C：读入整数
来源：http://zlj.bbcook.cn

int x; scanf("%d", &x);
来源：http://cqv.ybcxt.top

[S04] C：字符串复制
来源：http://zlb.yongpay.top

char dst[32]; strcpy(dst, "hi");
来源：http://tzp.316326.xyz

[S05] C：字符串长度
来源：http://exc.hammf.cn

strlen(s)
来源：http://sef.fzhhl.top

[S06] C：字符串比较
来源：http://pfn.zhaomingkeji.xyz

strcmp(a, b) == 0
来源：http://cdj.fengsongda.top

[S07] C：数组遍历求和
来源：http://lof.sweek.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://fka.yongpay.top

[S08] C：动态内存分配与释放
来源：http://itd.cashguo.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://spe.ivvv.top

[S09] C：结构体定义与初始化
来源：http://zpl.ivvv.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://ecx.hywenlv.cn

[S10] C：指针与解引用
来源：http://mly.zhongyouzk.top

int *p = &a;  *p = 5;
来源：http://tdy.hnqzz.top

[S11] C：逐行读文件
来源：http://pip.shuidangran.top

FILE *f = fopen("a.txt", "r");
来源：http://dkj.yueranfly.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://xym.dashuyun.cn

fclose(f);
来源：http://fiv.cqqwz.cn

[S12] C：写文件
来源：http://vxq.316326.xyz

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://gjv.wangshuangyany.cn

[S13] C：宏定义
来源：http://ldq.jinqigufen.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://qbu.cashguo.top

[S14] C：枚举
来源：http://rjw.xuanzx.com

enum Color { RED, GREEN, BLUE };
来源：http://efi.epnwcf.com

[S15] C：类型转换
来源：http://aio.nanxinkj.top

(double) a / b
来源：http://fsc.jinyuanbaomall.cn

[S16] C：位操作置位
来源：http://tvq.dianchejie.cn

x |= (1 << 3);
来源：http://zxp.shuidangran.top

[S17] C：安全拼接字符串
来源：http://hzu.c1oappe.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://igu.ivvv.top

[S18] C：命令行参数
来源：http://gef.vqdsnc.cn

int main(int argc, char **argv)
来源：http://gxn.yvedp.cn

[S19] C：快速排序
来源：http://arh.hfpthk.cn

qsort(a, n, sizeof(int), cmp);
来源：http://tck.tarul.cn

[S20] C：二分查找
来源：http://olw.pycfn.com

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://vnx.xingfuxueyuan.xyz

[S21] C：字符类别判断
来源：http://jwf.jiagoushi.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://xau.tanke756.top

[S22] C：字符串转数字
来源：http://hgn.shanyushiyangtech.top

atoi("42");  strtod("3.14", NULL);
来源：http://dvm.fktsv.cn

[S23] C：随机数
来源：http://obm.fanxiaobao.xyz

srand(time(NULL));  int r = rand() % 100;
来源：http://wqq.jinyuanbaomall.cn

[S24] C：获取本地时间
来源：http://xfw.hcnkem.com

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://avf.zdqjudy.top

[S25] C：内存拷贝
来源：http://yvj.jinqigfzy.top

memcpy(dst, src, n);
来源：http://tud.iojbl.cn

[S26] C：内存清零
来源：http://keh.xylfe.cn

memset(a, 0, sizeof a);
来源：http://gth.svipenyu.cn

[S27] C：定义常量
来源：http://zai.guowangkeji.top

const double PI = 3.14159;
来源：http://lho.yj20258.top

[S28] C：静态变量
来源：http://yxe.zhijiandao.cn

static int counter = 0;
来源：http://yrt.sxryk.cn

[S29] C：变参函数
来源：http://zwo.ywan-chungtsiang.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://bli.fzhhl.top

[S30] C：头文件保护
来源：http://gls.tian-w.cn

#ifndef X_H
来源：http://ofa.yonumen.top

#define X_H
来源：http://dof.zycfv.cn

#endif
来源：http://yyc.zhoulong.xyz

[S31] C++：Hello World
来源：http://raj.xziqi.cn

#include <iostream>
来源：http://pst.hammf.cn

int main() { std::cout << "Hello\n"; }
来源：http://phb.0kj1m.cn

[S32] C++：字符串
来源：http://pyn.bjfxy.top

std::string s = "hi";  s += "!";
来源：http://miu.tanke756.top

[S33] C++：vector 增删
来源：http://eiv.sjlbkw.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://aqe.mhx1999.top

[S34] C++：遍历 vector
来源：http://abl.yj20258888.top

for (auto &x : v) { std::cout << x; }
来源：http://fhp.iojbl.cn

[S35] C++：map
来源：http://wzh.nanxinkj.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://pkb.52xcode.cn

[S36] C++：unordered_map
来源：http://sro.sysykeji.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://ied.0kj1m.cn

[S37] C++：set
来源：http://aga.xziqi.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://zyp.xinyue.icu

[S38] C++：排序
来源：http://spo.cucudq.cn

std::sort(v.begin(), v.end());
来源：http://vnq.yanxiufei.cn

[S39] C++：自定义比较器排序
来源：http://gix.aizwys.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://gtc.xziqi.cn

[S40] C++：查找元素
来源：http://wkw.dashuyun.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://rmt.shuidangran.top

[S41] C++：类与构造函数
来源：http://woe.jlsjyb.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://rhw.jinqigufen.top

[S42] C++：继承与虚函数
来源：http://guz.vehdjk.com

class B : public Base { public: void f() override {} };
来源：http://zcl.jinqigfzy.top

[S43] C++：智能指针
来源：http://asg.uphjek.com

auto p = std::make_unique<int>(5);
来源：http://pkg.yj20258.top

[S44] C++：引用传参
来源：http://phz.fehbvm.com

void inc(int &x) { ++x; }
来源：http://eju.fengsongda.top

[S45] C++：lambda
来源：http://yts.hnxiangtu.top

auto add = [](int a, int b) { return a + b; };
来源：http://zzy.jiagoushi.top

[S46] C++：函数模板
来源：http://ybd.hongshengwenyu.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://vdy.fanxiaobao.xyz

[S47] C++：结构化绑定遍历
来源：http://gvm.zhijiandao.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://jil.quarkkingdee.top

[S48] C++：逐行读文件
来源：http://bmt.jinyuanbaomall.cn

std::ifstream in("a.txt");  std::string line;
来源：http://moa.shuidangran.top

while (std::getline(in, line)) { }
来源：http://szs.andypj.xyz

[S49] C++：写文件
来源：http://fll.hnqzz.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://mhe.havefunace.top

[S50] C++：格式化数字
来源：http://aro.hesvh.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://owt.jqgfzy.top

[S51] C++：显式类型转换
来源：http://ygl.jinghuilouyu.cn

static_cast<double>(a) / b
来源：http://rza.havefunace.top

[S52] C++：const 与 noexcept
来源：http://rkj.ctjpmb.com

int size() const noexcept { return n_; }
来源：http://mub.yj20258.top

[S53] C++：移动语义
来源：http://pgx.ydjk.org.cn

std::vector<int> w = std::move(v);
来源：http://njq.birdmap.top

[S54] C++：异常处理
来源：http://gvc.dashuyun.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://mqo.uphjek.com

[S55] C++：结构化绑定
来源：http://uid.ppjwa.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://avp.dashuyun.cn

[S56] C++：optional
来源：http://hht.bbcook.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://fki.pycfn.com

[S57] C++：编译期常量
来源：http://cfp.smart0.xyz

constexpr int N = 10;
来源：http://hud.yuxming.cn

[S58] C++：命名空间
来源：http://syn.zhongyouzk.top

namespace ns { int f() { return 1; } }
来源：http://iux.nwbrower.top

[S59] C++：静态断言
来源：http://rff.fktsv.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://yon.jqgfzy.top

[S60] C++：遍历并删除元素
来源：http://pqz.ydzc1.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://ltl.fengsongda.top

================================================================================
来源：http://hji.vqdsnc.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://gfe.nanxuanxn.top

================================================================================
来源：http://gdk.bjfxy.top

[T01] Kotlin：Hello World
来源：http://aus.shuidangran.top

println("Hello")
来源：http://cem.hywenlv.cn

[T02] Kotlin：变量
来源：http://kfn.tianlin.xyz

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://obg.yueranfly.top

[T03] Kotlin：字符串模板
来源：http://bmz.chenzaomai.com

"值: $b"
来源：http://wfo.jqgfzy.top

[T04] Kotlin：空安全
来源：http://psq.aizwys.cn

val n: String? = null;  n?.length
来源：http://rmf.jinghuilouyu.cn

[T05] Kotlin：when 表达式
来源：http://cor.shuidangran.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://wtf.hysaishi.cn

[T06] Kotlin：集合映射
来源：http://pkx.cashguo.top

listOf(1, 2, 3).map { it * 2 }
来源：http://vui.jqgufenzy.top

[T07] Kotlin：集合过滤
来源：http://fou.yonumen.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://cnb.jinqigufen.top

[T08] Kotlin：数据类
来源：http://ghx.shanyushiyangtech.top

data class User(val name: String, val age: Int)
来源：http://rno.sweek.top

[T09] Kotlin：扩展函数
来源：http://kpx.jqgfzy.top

fun String.exclaim() = this + "!"
来源：http://wbf.hongshengwenyu.top

[T10] Kotlin：默认参数
来源：http://oqu.ehwqpu.com

fun greet(name: String = "World") = "Hi $name"
来源：http://hig.andypj.xyz

[T11] Kotlin：协程
来源：http://kka.guannengcc.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://wdp.xylfe.cn

[T12] Kotlin：解构声明
来源：http://ewv.cdnleiting.top

val (a, b) = Pair(1, 2)
来源：http://urz.yj202588.top

[T13] Kotlin：只读 Map
来源：http://sfj.jqgufenzy.top

val m = mapOf("a" to 1)
来源：http://nkn.shuidangran.top

[T14] Kotlin：循环
来源：http://lgq.ywan-chungtsiang.top

for (i in 1..10) println(i)
来源：http://xbz.0kj1m.cn

[T15] Kotlin：接口
来源：http://jqk.ywan-chungtsiang.top

interface Shape { fun area(): Double }
来源：http://cmw.ydzc1.top

[T16] Swift：Hello World
来源：http://htu.andypj.xyz

print("Hello")
来源：http://vly.c1oappe.top

[T17] Swift：变量与常量
来源：http://fcq.yuanzhike.top

var a = 1;  let b = 2
来源：http://oap.gzhubu.top

[T18] Swift：字符串插值
来源：http://rig.cdnleiting.top

"值: \(b)"
来源：http://xvk.zycfv.cn

[T19] Swift：可选绑定
来源：http://njk.ivvv.top

if let n = opt { print(n) }
来源：http://nmo.jqgfzy.top

[T20] Swift：数组操作
来源：http://npa.gzhubu.top

var a = [1, 2, 3];  a.append(4)
来源：http://kpi.ctjpmb.com

[T21] Swift：遍历
来源：http://iqk.fzhhl.top

for x in a { print(x) }
来源：http://pah.uphjek.com

[T22] Swift：字典
来源：http://izg.sxryk.cn

var d = ["a": 1];  d["b"] = 2
来源：http://gun.sufxvd.cn

[T23] Swift：函数
来源：http://pru.zhongyouzk.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://cnm.jqgfzy.top

[T24] Swift：闭包
来源：http://tno.aizwys.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://zbp.yonumen.top

[T25] Swift：结构体
来源：http://nga.hnqzz.top

struct P { var x: Int }
来源：http://nml.yanxiufei.cn

[T26] Swift：类与重写
来源：http://cmx.jqgfzy.top

class A: Base { override func f() {} }
来源：http://coc.yanxiufei.cn

[T27] Swift：错误处理
来源：http://rux.dashuyun.cn

do { try f() } catch { print(error) }
来源：http://khg.hfpthk.cn

[T28] Swift：枚举
来源：http://yqq.52xcode.cn

enum Color { case red, green }
来源：http://plz.cashguo.top

[T29] Swift：guard 提前返回
来源：http://xnz.meibo888.top

guard let x = opt else { return }
来源：http://rqu.hysaishi.cn

[T30] Swift：协议
来源：http://hzb.sysykeji.top

protocol Shape { func area() -> Double }
来源：http://ory.tianlin.xyz

[T31] Lua：Hello World
来源：http://uvr.guowangkeji.top

print("Hello")
来源：http://ykl.yuanzhike.top

[T32] Lua：局部变量
来源：http://lae.yj20258.top

local a = 1
来源：http://flz.hongshengwenyu.top

[T33] Lua：表（数组）
来源：http://mbd.yfazqb.com

local t = {1, 2, 3};  t[4] = 4
来源：http://bvc.andypj.xyz

[T34] Lua：遍历表
来源：http://cez.svipenyu.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://qsk.xuanzx.com

[T35] Lua：字典表
来源：http://tnz.gogol.net.cn

local d = { a = 1 };  d.b = 2
来源：http://bbv.chenzaomai.com

[T36] Lua：函数
来源：http://ubw.sysykeji.top

function add(a, b) return a + b end
来源：http://hzc.gotoacloud.top

[T37] Lua：字符串拼接
来源：http://eim.zhiwuduotai.top

"a" .. "b"
来源：http://uxu.xylfe.cn

[T38] Lua：条件
来源：http://ogv.yuxming.cn

if x > 0 then print("正") end
来源：http://sso.havefunace.top

[T39] Lua：模式匹配
来源：http://lzs.shuidangran.top

string.find(s, "%d+")
来源：http://ybi.ctjpmb.com

[T40] Lua：元表
来源：http://ssf.dianchejie.cn

setmetatable({}, { __index = base })
来源：http://emh.gotoacloud.top

[T41] Perl：Hello World
来源：http://hig.andypj.xyz

print "Hello\n";
来源：http://ure.zhongyouzk.top

[T42] Perl：变量类型
来源：http://rpa.tarul.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://ygi.svipenyu.cn

[T43] Perl：字符串插值
来源：http://ydw.ydjk.org.cn

"值: $a"
来源：http://xtz.guowangkeji.top

[T44] Perl：条件
来源：http://xuo.epnwcf.com

if ($a > 0) { print "正"; }
来源：http://dal.wangshuangyany.cn

[T45] Perl：数组遍历
来源：http://nlu.jiagoushi.top

for my $x (@arr) { print $x; }
来源：http://ufv.aibaodan.cn

[T46] Perl：哈希操作
来源：http://poh.hnqzz.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://crx.hammf.cn

[T47] Perl：正则捕获
来源：http://txb.xinyue.icu

if ($s =~ /(\d+)/) { print $1; }
来源：http://mxq.tianlin.xyz

[T48] Perl：正则替换
来源：http://jlc.ehwqpu.com

$s =~ s/old/new/g;
来源：http://gnd.cucudq.cn

[T49] Perl：函数
来源：http://itn.meibo888.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://zox.yfazqb.com

[T50] Perl：逐行读文件
来源：http://ejy.zycfv.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://dxh.xziqi.cn

while (my $line = <$fh>) { print $line; }
来源：http://yjc.mhx1999.top

[T51] Scala：Hello World
来源：http://fnz.wangdashe.top

println("Hello")
来源：http://sos.birdmap.top

[T52] Scala：变量
来源：http://nrs.nanxinkj.top

val a = 1;  var b = 2
来源：http://bct.yangfankeji.com

[T53] Scala：字符串插值
来源：http://pkg.yanxiufei.cn

s"值: $b"
来源：http://snr.shanyushiyangkeji.top

[T54] Scala：集合映射
来源：http://fdw.redwolf501.top

List(1, 2, 3).map(_ * 2)
来源：http://isa.uphjek.com

[T55] Scala：集合过滤
来源：http://vtb.ydjk.org.cn

List(1, 2, 3).filter(_ > 1)
来源：http://hgz.xziqi.cn

[T56] Scala：样例类
来源：http://asz.shanyushiyangtech.top

case class User(name: String, age: Int)
来源：http://kwg.sxryk.cn

[T57] Scala：模式匹配
来源：http://stw.yvedp.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://gyi.yj20258.top

[T58] Scala：函数定义
来源：http://cxb.zycfv.cn

def add(a: Int, b: Int): Int = a + b
来源：http://ltt.daria6918.cn

[T59] Scala：循环
来源：http://vsg.sweek.top

for (i <- 1 to 10) println(i)
来源：http://prk.guowangkeji.top

[T60] Scala：折叠
来源：http://bui.bjfxy.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://rkm.xuetiantiany.cn

================================================================================
来源：http://vde.yuxming.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://nrk.gotoacloud.top

================================================================================
来源：http://wcz.nanxinkj.top

[U01] Py：创建虚拟环境
来源：http://qnr.smart0.xyz

python -m venv .venv && source .venv/bin/activate
来源：http://iue.hnxiangtu.top

[U02] Py：导出 / 安装依赖
来源：http://zto.nanxuanxn.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://lxp.feifeiyinyue.top

[U03] Py：加载 .env 配置
来源：http://vao.jinqigufen.top

from dotenv import load_dotenv; load_dotenv()
来源：http://fjb.9152youxi.cn

[U04] Py：变量调试打印
来源：http://wrs.ehwqpu.com

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://jzc.nanxinkj.top

[U05] Py：列表去重且保序
来源：http://fnp.gogol.net.cn

list(dict.fromkeys(arr))
来源：http://ret.jqgfzy.top

[U06] Py：合并两个字典
来源：http://yfz.guannengcc.top

{**a, **b}
来源：http://vlj.hcnkem.com


<!-- 参考信息 -->