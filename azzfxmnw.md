代发 wailian999

free -h;  ps aux | grep nginx
来源：http://wkn.ehwqpu.com

[R64] 结束进程
来源：http://ser.316326.xyz

kill -9 $(pgrep -f app.py)
来源：http://kux.shuidangran.top

[R65] 查看端口占用
来源：http://ksx.havefunace.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://zys.aibaodan.cn

[R66] 定时任务
来源：http://cyq.snrcjt.cn

crontab -e;  crontab -l
来源：http://kay.yfazqb.com

[R67] 生成随机十六进制串
来源：http://xza.shangyingyoupin.top

openssl rand -hex 16
来源：http://upb.316326.xyz

[R68] 计算文件校验值
来源：http://xkb.jyoumei.cn

sha256sum a.txt;  md5sum a.txt
来源：http://hkg.hfpthk.cn

[R69] 生成随机密码
来源：http://yas.tanke756.top

head -c 16 /dev/urandom | base64
来源：http://how.shanyushiyangtech.top

[R70] 时间戳与互转
来源：http://mit.epnwcf.com

date +%s;  date -d @1700000000
来源：http://wgg.gaohongyu789.top

[R71] 日期格式化
来源：http://jxj.mhx1999.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://xle.aibaodan.cn

[R72] 等待端口就绪
来源：http://ffu.cheryme.top

until nc -z localhost 3306; do sleep 1; done
来源：http://vul.smart0.xyz

[R73] 分割大日志
来源：http://fst.yongpay.top

split -l 1000 big.log part_
来源：http://bus.ydjk.org.cn

[R74] 批量重命名
来源：http://nll.xinyue.icu

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://iib.yanxiufei.cn

[R75] 导出环境变量
来源：http://duq.nanxuanxn.top

export PATH="$HOME/bin:$PATH"
来源：http://feq.pengpengdd.cyou

[R76] 使用临时文件
来源：http://cfg.dianchejie.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://exr.sysykeji.top

[R77] 读取用户输入
来源：http://zgo.aibaodan.cn

read -rp "请输入: " ans
来源：http://dhc.dashuyun.cn

[R78] 交互式菜单
来源：http://thf.xziqi.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://haa.ybcxt.top

[R79] 解析命令行选项
来源：http://jom.vqdsnc.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://guk.shanyushiyangtech.top

[R80] 查看脚本执行耗时
来源：http://huz.yj20258888.top

time ./run.sh
来源：http://lan.xuanzx.com

================================================================================
来源：http://rxs.cashguo.top

S. C / C++ 专题
来源：http://gpu.pengpengdd.cyou

================================================================================
来源：http://wye.shanyushiyangtech.top

[S01] C：Hello World
来源：http://krp.nanxuanxn.top

#include <stdio.h>
来源：http://mgo.hammf.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://riz.xinyue.icu

[S02] C：变量与格式化输出
来源：http://ipf.svipenyu.cn

int a = 10; printf("%d\n", a);
来源：http://wlb.ehwqpu.com

[S03] C：读入整数
来源：http://cxh.shangyingyoupin.top

int x; scanf("%d", &x);
来源：http://fiz.cucudq.cn

[S04] C：字符串复制
来源：http://xvp.yj202588.top

char dst[32]; strcpy(dst, "hi");
来源：http://ekw.aizwys.cn

[S05] C：字符串长度
来源：http://hcv.aibaodan.cn

strlen(s)
来源：http://irh.xingfuxueyuan.xyz

[S06] C：字符串比较
来源：http://oal.gogol.net.cn

strcmp(a, b) == 0
来源：http://mxd.mhx1999.top

[S07] C：数组遍历求和
来源：http://jla.yj20258888.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://iud.zhiwuduotai.top

[S08] C：动态内存分配与释放
来源：http://tmr.gogol.net.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://tue.cdnleiting.top

[S09] C：结构体定义与初始化
来源：http://zcz.cheryme.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://jwu.daxiang520.top

[S10] C：指针与解引用
来源：http://prz.zhongyouzk.top

int *p = &a;  *p = 5;
来源：http://rqe.pycfn.com

[S11] C：逐行读文件
来源：http://hvu.nanxinkj.top

FILE *f = fopen("a.txt", "r");
来源：http://gjq.zhongyouzk.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://ufo.zhixingplan.top

fclose(f);
来源：http://asy.vehdjk.com

[S12] C：写文件
来源：http://bcz.bjfxy.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hkr.ppjwa.cn

[S13] C：宏定义
来源：http://ayz.hywenlv.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://jdn.yvedp.cn

[S14] C：枚举
来源：http://ivi.tarul.cn

enum Color { RED, GREEN, BLUE };
来源：http://qbg.guowangkeji.top

[S15] C：类型转换
来源：http://skl.meibo888.top

(double) a / b
来源：http://lbw.sweek.top

[S16] C：位操作置位
来源：http://dfb.yfazqb.com

x |= (1 << 3);
来源：http://jal.hnqzz.top

[S17] C：安全拼接字符串
来源：http://vwt.hywenlv.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://sqf.birdmap.top

[S18] C：命令行参数
来源：http://qal.dianchejie.cn

int main(int argc, char **argv)
来源：http://abc.hnqzz.top

[S19] C：快速排序
来源：http://blo.jyoumei.cn

qsort(a, n, sizeof(int), cmp);
来源：http://rra.xylfe.cn

[S20] C：二分查找
来源：http://wuq.vehdjk.com

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://dbr.kuanghao11.cn

[S21] C：字符类别判断
来源：http://iix.mhx1999.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://bln.epnwcf.com

[S22] C：字符串转数字
来源：http://jri.cdnleiting.top

atoi("42");  strtod("3.14", NULL);
来源：http://hyb.zycfv.cn

[S23] C：随机数
来源：http://job.tian-w.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://uma.zhixingplan.top

[S24] C：获取本地时间
来源：http://pjz.jinyuanbaomall.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://unz.sysykeji.top

[S25] C：内存拷贝
来源：http://jah.ydjk.org.cn

memcpy(dst, src, n);
来源：http://umd.yj20258888.top

[S26] C：内存清零
来源：http://kjl.iojbl.cn

memset(a, 0, sizeof a);
来源：http://epu.ctjpmb.com

[S27] C：定义常量
来源：http://mrv.jinqigfzy.top

const double PI = 3.14159;
来源：http://ubh.zhengqikj.top

[S28] C：静态变量
来源：http://yqm.jianghu66.top

static int counter = 0;
来源：http://wsq.jinghuilouyu.cn

[S29] C：变参函数
来源：http://byl.aizwys.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://jfr.ivvv.top

[S30] C：头文件保护
来源：http://wng.zhengqikj.top

#ifndef X_H
来源：http://crf.hammf.cn

#define X_H
来源：http://byz.uphjek.com

#endif
来源：http://edl.xziqi.cn

[S31] C++：Hello World
来源：http://wrh.yonumen.top

#include <iostream>
来源：http://awi.feifeiyinyue.top

int main() { std::cout << "Hello\n"; }
来源：http://dzj.tarul.cn

[S32] C++：字符串
来源：http://pba.jinghuilouyu.cn

std::string s = "hi";  s += "!";
来源：http://byk.aibaodan.cn

[S33] C++：vector 增删
来源：http://jsl.bbcook.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://emu.ivvv.top

[S34] C++：遍历 vector
来源：http://lbc.fengsongda.top

for (auto &x : v) { std::cout << x; }
来源：http://ysm.ctjpmb.com

[S35] C++：map
来源：http://zpx.yuanzhike.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://dbg.wangshuangyany.cn

[S36] C++：unordered_map
来源：http://htb.vqdsnc.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://vvt.chenlongwang.top

[S37] C++：set
来源：http://bmm.vehdjk.com

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://cbb.zhoulong.xyz

[S38] C++：排序
来源：http://ypu.jyoumei.cn

std::sort(v.begin(), v.end());
来源：http://iqb.hesvh.cn

[S39] C++：自定义比较器排序
来源：http://aaj.nanxuanxn.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://iix.cdnleiting.top

[S40] C++：查找元素
来源：http://gns.ywan-chungtsiang.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://fdm.xuetiantiany.cn

[S41] C++：类与构造函数
来源：http://ffa.sjlbkw.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://cgz.xingfuxueyuan.xyz

[S42] C++：继承与虚函数
来源：http://mvc.xylfe.cn

class B : public Base { public: void f() override {} };
来源：http://fow.xziqi.cn

[S43] C++：智能指针
来源：http://iop.nanxinkj.top

auto p = std::make_unique<int>(5);
来源：http://sls.yuxming.cn

[S44] C++：引用传参
来源：http://kwx.nanxinkj.top

void inc(int &x) { ++x; }
来源：http://fjg.xuetiantiany.cn

[S45] C++：lambda
来源：http://uhx.sxryk.cn

auto add = [](int a, int b) { return a + b; };
来源：http://emf.yuanzhike.top

[S46] C++：函数模板
来源：http://ijf.daxiang520.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://dti.sweek.top

[S47] C++：结构化绑定遍历
来源：http://rum.c1oappe.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://pyg.xylfe.cn

[S48] C++：逐行读文件
来源：http://qeq.jqgufenzy.top

std::ifstream in("a.txt");  std::string line;
来源：http://csk.chenlongwang.top

while (std::getline(in, line)) { }
来源：http://odt.pycfn.com

[S49] C++：写文件
来源：http://cob.pycfn.com

std::ofstream out("a.txt");  out << "hi\n";
来源：http://qau.cashguo.top

[S50] C++：格式化数字
来源：http://rtk.havefunace.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hsc.ywan-chungtsiang.top

[S51] C++：显式类型转换
来源：http://ynp.zhixingplan.top

static_cast<double>(a) / b
来源：http://ohh.fehbvm.com

[S52] C++：const 与 noexcept
来源：http://nvc.xylfe.cn

int size() const noexcept { return n_; }
来源：http://ndf.wangdashe.top

[S53] C++：移动语义
来源：http://qpq.zhijiandao.cn

std::vector<int> w = std::move(v);
来源：http://nmp.jqgufenzy.top

[S54] C++：异常处理
来源：http://gyt.gaohongyu789.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://goj.nanxuanxn.top

[S55] C++：结构化绑定
来源：http://rgx.redwolf501.top

auto [a, b] = std::make_pair(1, 2);
来源：http://kty.ybcxt.top

[S56] C++：optional
来源：http://tzx.wangdashe.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://pzf.andypj.xyz

[S57] C++：编译期常量
来源：http://boy.shzxlz.cn

constexpr int N = 10;
来源：http://det.fktsv.cn

[S58] C++：命名空间
来源：http://ssm.shanyushiyangkeji.top

namespace ns { int f() { return 1; } }
来源：http://qit.ivvv.top

[S59] C++：静态断言
来源：http://xuo.havefunace.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://yzl.nanxinkj.top

[S60] C++：遍历并删除元素
来源：http://zcw.pengpengdd.cyou

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://jxd.fktsv.cn

================================================================================
来源：http://rtq.redwolf501.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://vzc.tian-w.cn

================================================================================
来源：http://jss.cqqwz.cn

[T01] Kotlin：Hello World
来源：http://pvn.smart0.xyz

println("Hello")
来源：http://fwm.guowangkeji.top

[T02] Kotlin：变量
来源：http://dxh.gzhubu.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://aqu.guowangkeji.top

[T03] Kotlin：字符串模板
来源：http://twh.zhoulong.xyz

"值: $b"
来源：http://jhn.yueranfly.top

[T04] Kotlin：空安全
来源：http://hso.andypj.xyz

val n: String? = null;  n?.length
来源：http://tfu.jinghuilouyu.cn

[T05] Kotlin：when 表达式
来源：http://xhc.yongpay.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://gst.hnqzz.top

[T06] Kotlin：集合映射
来源：http://ogx.yj20258888.top

listOf(1, 2, 3).map { it * 2 }
来源：http://bvv.xinyue.icu

[T07] Kotlin：集合过滤
来源：http://xzt.yuanzhike.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://rzs.xziqi.cn

[T08] Kotlin：数据类
来源：http://gry.jyoumei.cn

data class User(val name: String, val age: Int)
来源：http://tlf.fehbvm.com

[T09] Kotlin：扩展函数
来源：http://jjv.hammf.cn

fun String.exclaim() = this + "!"
来源：http://tda.gzhubu.top

[T10] Kotlin：默认参数
来源：http://rmz.hywenlv.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://wzx.52xcode.cn

[T11] Kotlin：协程
来源：http://fgc.hysaishi.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://eyj.9152youxi.cn

[T12] Kotlin：解构声明
来源：http://tim.quarkkingdee.top

val (a, b) = Pair(1, 2)
来源：http://pgl.mhx1999.top

[T13] Kotlin：只读 Map
来源：http://frz.ivvv.top

val m = mapOf("a" to 1)
来源：http://mhn.vehdjk.com

[T14] Kotlin：循环
来源：http://udj.zdbjq.cn

for (i in 1..10) println(i)
来源：http://rhp.xylfe.cn

[T15] Kotlin：接口
来源：http://lvz.cucudq.cn

interface Shape { fun area(): Double }
来源：http://uaa.zhiwuduotai.top

[T16] Swift：Hello World
来源：http://rut.yvedp.cn

print("Hello")
来源：http://lig.snrcjt.cn

[T17] Swift：变量与常量
来源：http://xjd.yangfankeji.com

var a = 1;  let b = 2
来源：http://hrg.hysaishi.cn

[T18] Swift：字符串插值
来源：http://zdm.fehbvm.com

"值: \(b)"
来源：http://ghu.tian-w.cn

[T19] Swift：可选绑定
来源：http://nwo.ywan-chungtsiang.top

if let n = opt { print(n) }
来源：http://dqg.yanxiufei.cn

[T20] Swift：数组操作
来源：http://cnj.tian-w.cn

var a = [1, 2, 3];  a.append(4)
来源：http://ypw.dashuyun.cn

[T21] Swift：遍历
来源：http://rut.gaohongyu789.top

for x in a { print(x) }
来源：http://cve.zhengqikj.top

[T22] Swift：字典
来源：http://nvz.xuetiantiany.cn

var d = ["a": 1];  d["b"] = 2
来源：http://taf.yj202588.top

[T23] Swift：函数
来源：http://rxl.zhengqikj.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hof.xingfuxueyuan.xyz

[T24] Swift：闭包
来源：http://swe.ywan-chungtsiang.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://ecv.chenzaomai.com

[T25] Swift：结构体
来源：http://jlq.shuidangran.top

struct P { var x: Int }
来源：http://ulb.c1oappe.top

[T26] Swift：类与重写
来源：http://rxe.tanke756.top

class A: Base { override func f() {} }
来源：http://ujq.aibaodan.cn

[T27] Swift：错误处理
来源：http://fav.cdnleiting.top

do { try f() } catch { print(error) }
来源：http://nun.nanxuanxn.top

[T28] Swift：枚举
来源：http://tua.tanke756.top

enum Color { case red, green }
来源：http://upz.cdnleiting.top

[T29] Swift：guard 提前返回
来源：http://ggy.shanyushiyangkeji.top

guard let x = opt else { return }
来源：http://cad.nanxinkj.top

[T30] Swift：协议
来源：http://uax.yfazqb.com

protocol Shape { func area() -> Double }
来源：http://uqr.jinghuilouyu.cn

[T31] Lua：Hello World
来源：http://ekj.zdqjudy.top

print("Hello")
来源：http://roz.nwbrower.top

[T32] Lua：局部变量
来源：http://esg.yfazqb.com

local a = 1
来源：http://jzw.jiagoushi.top

[T33] Lua：表（数组）
来源：http://bkk.sweek.top

local t = {1, 2, 3};  t[4] = 4
来源：http://qoa.ydjk.org.cn

[T34] Lua：遍历表
来源：http://mbh.sjlbkw.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://gqm.smart0.xyz

[T35] Lua：字典表
来源：http://esx.xziqi.cn

local d = { a = 1 };  d.b = 2
来源：http://hqa.uphjek.com

[T36] Lua：函数
来源：http://zbo.yj202588.top

function add(a, b) return a + b end
来源：http://fwc.jinyuanbaomall.cn

[T37] Lua：字符串拼接
来源：http://qtc.sweek.top

"a" .. "b"
来源：http://udr.hnxiangtu.top

[T38] Lua：条件
来源：http://hok.bbcook.cn

if x > 0 then print("正") end
来源：http://mwb.kuanghao11.cn

[T39] Lua：模式匹配
来源：http://hop.xuanzx.com

string.find(s, "%d+")
来源：http://atz.zhongyouzk.top

[T40] Lua：元表
来源：http://gup.hnqzz.top

setmetatable({}, { __index = base })
来源：http://cvf.shanyushiyangtech.top

[T41] Perl：Hello World
来源：http://vew.xylfe.cn

print "Hello\n";
来源：http://ylw.chenjidiqi.icu

[T42] Perl：变量类型
来源：http://tfa.jqgfzy.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://osl.9152youxi.cn

[T43] Perl：字符串插值
来源：http://aad.pengpengdd.cyou

"值: $a"
来源：http://ljt.iojbl.cn

[T44] Perl：条件
来源：http://ule.hnqzz.top

if ($a > 0) { print "正"; }
来源：http://lnj.guannengcc.top

[T45] Perl：数组遍历
来源：http://pig.hysaishi.cn

for my $x (@arr) { print $x; }
来源：http://iyw.yj202588.top

[T46] Perl：哈希操作
来源：http://gpt.yuanzhike.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://box.zdbjq.cn

[T47] Perl：正则捕获
来源：http://eew.vqdsnc.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://gjp.yongpay.top

[T48] Perl：正则替换
来源：http://lwo.tarul.cn

$s =~ s/old/new/g;
来源：http://ypl.hongshengwenyu.top

[T49] Perl：函数
来源：http://exx.hnxiangtu.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://amy.yj20258.top

[T50] Perl：逐行读文件
来源：http://kul.daxiang520.top

open my $fh, "<", "a.txt" or die $!;
来源：http://crx.vqdsnc.cn

while (my $line = <$fh>) { print $line; }
来源：http://wfh.yj202588.top

[T51] Scala：Hello World
来源：http://kit.gzhubu.top

println("Hello")
来源：http://ejy.cdnleiting.top

[T52] Scala：变量
来源：http://pqa.shuidangran.top

val a = 1;  var b = 2
来源：http://oqk.sufxvd.cn

[T53] Scala：字符串插值
来源：http://uql.redwolf501.top

s"值: $b"
来源：http://amt.cqqwz.cn

[T54] Scala：集合映射
来源：http://ylt.shanyushiyangtech.top

List(1, 2, 3).map(_ * 2)
来源：http://lmp.fktsv.cn

[T55] Scala：集合过滤
来源：http://pdf.meibo888.top

List(1, 2, 3).filter(_ > 1)
来源：http://agq.tianlin.xyz

[T56] Scala：样例类
来源：http://rmx.andypj.xyz

case class User(name: String, age: Int)
来源：http://faa.ywan-chungtsiang.top

[T57] Scala：模式匹配
来源：http://oav.316326.xyz

x match { case 1 => "一"; case _ => "其他" }
来源：http://xvl.fktsv.cn

[T58] Scala：函数定义
来源：http://jas.havefunace.top

def add(a: Int, b: Int): Int = a + b
来源：http://ozn.wangdashe.top

[T59] Scala：循环
来源：http://clk.gotoacloud.top

for (i <- 1 to 10) println(i)
来源：http://byt.redwolf501.top

[T60] Scala：折叠
来源：http://dsl.wangshuangyany.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://yrm.sjlbkw.cn

================================================================================
来源：http://qwj.ctjpmb.com

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://pve.epnwcf.com

================================================================================
来源：http://wll.hfpthk.cn

[U01] Py：创建虚拟环境
来源：http://rlh.ivvv.top

python -m venv .venv && source .venv/bin/activate
来源：http://mse.gzhubu.top

[U02] Py：导出 / 安装依赖
来源：http://osi.c1oappe.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://bed.yuxming.cn

[U03] Py：加载 .env 配置
来源：http://bfc.guannengcc.top

from dotenv import load_dotenv; load_dotenv()
来源：http://qbm.smart0.xyz

[U04] Py：变量调试打印
来源：http://iti.xziqi.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://pkd.ppjwa.cn


<!-- 参考信息 -->