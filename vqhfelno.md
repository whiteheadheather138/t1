代发 wailian999

free -h;  ps aux | grep nginx
来源：http://rsf.zhoulong.xyz

[R64] 结束进程
来源：http://mhg.aibaodan.cn

kill -9 $(pgrep -f app.py)
来源：http://kds.iojbl.cn

[R65] 查看端口占用
来源：http://cfo.yuxming.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://fcs.jinghuilouyu.cn

[R66] 定时任务
来源：http://jqc.tanke756.top

crontab -e;  crontab -l
来源：http://qnn.jinqigfzy.top

[R67] 生成随机十六进制串
来源：http://yte.vqdsnc.cn

openssl rand -hex 16
来源：http://ikw.gaohongyu789.top

[R68] 计算文件校验值
来源：http://gxf.tarul.cn

sha256sum a.txt;  md5sum a.txt
来源：http://whm.yangfankeji.com

[R69] 生成随机密码
来源：http://eku.quarkkingdee.top

head -c 16 /dev/urandom | base64
来源：http://ydu.xziqi.cn

[R70] 时间戳与互转
来源：http://sae.yanxiufei.cn

date +%s;  date -d @1700000000
来源：http://auu.xinyue.icu

[R71] 日期格式化
来源：http://alw.fehbvm.com

date +"%Y-%m-%d %H:%M:%S"
来源：http://mes.cqqwz.cn

[R72] 等待端口就绪
来源：http://dkn.ppjwa.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://zai.yfazqb.com

[R73] 分割大日志
来源：http://tri.iojbl.cn

split -l 1000 big.log part_
来源：http://eew.cucudq.cn

[R74] 批量重命名
来源：http://pta.bjfxy.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://rsl.fzhhl.top

[R75] 导出环境变量
来源：http://fdq.zdbjq.cn

export PATH="$HOME/bin:$PATH"
来源：http://fxr.yueranfly.top

[R76] 使用临时文件
来源：http://eaa.yfazqb.com

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hbr.hongshengwenyu.top

[R77] 读取用户输入
来源：http://ahv.wangdashe.top

read -rp "请输入: " ans
来源：http://pkh.nanxuanxn.top

[R78] 交互式菜单
来源：http://ppd.fzhhl.top

select opt in a b c; do echo "$opt"; break; done
来源：http://ztd.fktsv.cn

[R79] 解析命令行选项
来源：http://fjj.ydzc1.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://tau.yj20258.top

[R80] 查看脚本执行耗时
来源：http://pso.sysykeji.top

time ./run.sh
来源：http://hyk.zhoulong.xyz

================================================================================
来源：http://kid.chenjidiqi.icu

S. C / C++ 专题
来源：http://bmc.dashuyun.cn

================================================================================
来源：http://bpw.hfpthk.cn

[S01] C：Hello World
来源：http://weo.hfpthk.cn

#include <stdio.h>
来源：http://cku.nanxuanxn.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://nki.yueranfly.top

[S02] C：变量与格式化输出
来源：http://yoq.meibo888.top

int a = 10; printf("%d\n", a);
来源：http://gyz.ydzc1.top

[S03] C：读入整数
来源：http://sar.jlsjyb.cn

int x; scanf("%d", &x);
来源：http://ouz.yfazqb.com

[S04] C：字符串复制
来源：http://vht.wangshuangyany.cn

char dst[32]; strcpy(dst, "hi");
来源：http://lnq.xziqi.cn

[S05] C：字符串长度
来源：http://klg.guowangkeji.top

strlen(s)
来源：http://rvo.sxryk.cn

[S06] C：字符串比较
来源：http://dak.xuanzx.com

strcmp(a, b) == 0
来源：http://nqw.fzhhl.top

[S07] C：数组遍历求和
来源：http://nzb.zycfv.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://fsf.fktsv.cn

[S08] C：动态内存分配与释放
来源：http://asq.yonumen.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://dhs.wangshuangyany.cn

[S09] C：结构体定义与初始化
来源：http://qzp.uphjek.com

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://flm.xuanzx.com

[S10] C：指针与解引用
来源：http://dcx.tanke756.top

int *p = &a;  *p = 5;
来源：http://nun.havefunace.top

[S11] C：逐行读文件
来源：http://kqe.c1oappe.top

FILE *f = fopen("a.txt", "r");
来源：http://fps.zhaomingkeji.xyz

while (fgets(buf, sizeof buf, f)) { }
来源：http://oso.zhoulong.xyz

fclose(f);
来源：http://xqz.yj20258.top

[S12] C：写文件
来源：http://scx.cheryme.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://pwh.aibaodan.cn

[S13] C：宏定义
来源：http://uut.fengsongda.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://xej.zhijiandao.cn

[S14] C：枚举
来源：http://eii.zhaomingkeji.xyz

enum Color { RED, GREEN, BLUE };
来源：http://heu.sxryk.cn

[S15] C：类型转换
来源：http://bmc.zhijiandao.cn

(double) a / b
来源：http://wox.haohaochexian.top

[S16] C：位操作置位
来源：http://kgg.dianchejie.cn

x |= (1 << 3);
来源：http://oao.316326.xyz

[S17] C：安全拼接字符串
来源：http://tbb.sweek.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://mzt.guannengcc.top

[S18] C：命令行参数
来源：http://uvy.vehdjk.com

int main(int argc, char **argv)
来源：http://abr.sysykeji.top

[S19] C：快速排序
来源：http://xqu.guowangkeji.top

qsort(a, n, sizeof(int), cmp);
来源：http://wih.hnxiangtu.top

[S20] C：二分查找
来源：http://mpy.smart0.xyz

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hwb.fehbvm.com

[S21] C：字符类别判断
来源：http://vmb.smart0.xyz

isdigit(c);  isalpha(c);  isspace(c);
来源：http://ute.hesvh.cn

[S22] C：字符串转数字
来源：http://ywz.redwolf501.top

atoi("42");  strtod("3.14", NULL);
来源：http://bfb.wangshuangyany.cn

[S23] C：随机数
来源：http://ovs.jinqigfzy.top

srand(time(NULL));  int r = rand() % 100;
来源：http://mjv.zhongyouzk.top

[S24] C：获取本地时间
来源：http://tsz.zhixingplan.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://dvs.zycfv.cn

[S25] C：内存拷贝
来源：http://xbh.yj202588.top

memcpy(dst, src, n);
来源：http://hzz.kuanghao11.cn

[S26] C：内存清零
来源：http://hfo.yj20258888.top

memset(a, 0, sizeof a);
来源：http://rxl.hnxiangtu.top

[S27] C：定义常量
来源：http://xnk.yueranfly.top

const double PI = 3.14159;
来源：http://vwf.chenjidiqi.icu

[S28] C：静态变量
来源：http://bgz.quarkkingdee.top

static int counter = 0;
来源：http://wdt.ctjpmb.com

[S29] C：变参函数
来源：http://env.ydjk.org.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://jgy.vehdjk.com

[S30] C：头文件保护
来源：http://ylp.tian-w.cn

#ifndef X_H
来源：http://aef.zhongyouzk.top

#define X_H
来源：http://viu.redwolf501.top

#endif
来源：http://sff.wangdashe.top

[S31] C++：Hello World
来源：http://ouf.nanxinkj.top

#include <iostream>
来源：http://mfp.xinyue.icu

int main() { std::cout << "Hello\n"; }
来源：http://yot.xylfe.cn

[S32] C++：字符串
来源：http://bcj.fanxiaobao.xyz

std::string s = "hi";  s += "!";
来源：http://sva.tarul.cn

[S33] C++：vector 增删
来源：http://mge.zhiwuduotai.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://efm.hcnkem.com

[S34] C++：遍历 vector
来源：http://knm.jiagoushi.top

for (auto &x : v) { std::cout << x; }
来源：http://gbw.guannengcc.top

[S35] C++：map
来源：http://yph.yanxiufei.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://ruh.52xcode.cn

[S36] C++：unordered_map
来源：http://uve.tian-w.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://url.jinghuilouyu.cn

[S37] C++：set
来源：http://ust.ctjpmb.com

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://eqk.yonumen.top

[S38] C++：排序
来源：http://bcr.shangyingyoupin.top

std::sort(v.begin(), v.end());
来源：http://npq.fanxiaobao.xyz

[S39] C++：自定义比较器排序
来源：http://vko.cqqwz.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://har.fehbvm.com

[S40] C++：查找元素
来源：http://pkm.fzhhl.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://ahn.ybcxt.top

[S41] C++：类与构造函数
来源：http://fml.zhiwuduotai.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://yqj.daria6918.cn

[S42] C++：继承与虚函数
来源：http://dor.redwolf501.top

class B : public Base { public: void f() override {} };
来源：http://ifz.gaohongyu789.top

[S43] C++：智能指针
来源：http://twz.uphjek.com

auto p = std::make_unique<int>(5);
来源：http://xun.jinqigfzy.top

[S44] C++：引用传参
来源：http://enm.zhijiandao.cn

void inc(int &x) { ++x; }
来源：http://cuf.daria6918.cn

[S45] C++：lambda
来源：http://xpa.jqgufenzy.top

auto add = [](int a, int b) { return a + b; };
来源：http://tjp.cheryme.top

[S46] C++：函数模板
来源：http://jyz.tanke756.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://lnm.sxryk.cn

[S47] C++：结构化绑定遍历
来源：http://jzd.jiagoushi.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://uei.yj20258.top

[S48] C++：逐行读文件
来源：http://nuj.zhengqikj.top

std::ifstream in("a.txt");  std::string line;
来源：http://jiq.iojbl.cn

while (std::getline(in, line)) { }
来源：http://tmx.yongpay.top

[S49] C++：写文件
来源：http://afo.c1oappe.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://qbf.hcnkem.com

[S50] C++：格式化数字
来源：http://mqo.cheryme.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://eog.hysaishi.cn

[S51] C++：显式类型转换
来源：http://mxx.iojbl.cn

static_cast<double>(a) / b
来源：http://bfo.yj20258888.top

[S52] C++：const 与 noexcept
来源：http://vss.hfpthk.cn

int size() const noexcept { return n_; }
来源：http://ctx.jinqigfzy.top

[S53] C++：移动语义
来源：http://nva.kuanghao11.cn

std::vector<int> w = std::move(v);
来源：http://yzr.gogol.net.cn

[S54] C++：异常处理
来源：http://wur.fktsv.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://ncr.sufxvd.cn

[S55] C++：结构化绑定
来源：http://ddc.hfpthk.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://aop.zdbjq.cn

[S56] C++：optional
来源：http://auc.shanyushiyangkeji.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://tho.jinqigufen.top

[S57] C++：编译期常量
来源：http://xny.redwolf501.top

constexpr int N = 10;
来源：http://nrt.ehwqpu.com

[S58] C++：命名空间
来源：http://ivx.ybcxt.top

namespace ns { int f() { return 1; } }
来源：http://nwn.chenlongwang.top

[S59] C++：静态断言
来源：http://plw.yj202588.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://omg.wangshuangyany.cn

[S60] C++：遍历并删除元素
来源：http://ybn.iojbl.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://nzh.yj20258.top

================================================================================
来源：http://nkm.nwbrower.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://zjz.pycfn.com

================================================================================
来源：http://efi.mhx1999.top

[T01] Kotlin：Hello World
来源：http://ebq.shzxlz.cn

println("Hello")
来源：http://pdm.haohaochexian.top

[T02] Kotlin：变量
来源：http://fiq.ybcxt.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://svu.yangfankeji.com

[T03] Kotlin：字符串模板
来源：http://wwp.feifeiyinyue.top

"值: $b"
来源：http://zod.jqgufenzy.top

[T04] Kotlin：空安全
来源：http://emz.yuxming.cn

val n: String? = null;  n?.length
来源：http://gdr.wangshuangyany.cn

[T05] Kotlin：when 表达式
来源：http://hkj.tanke756.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://ryz.jianghu66.top

[T06] Kotlin：集合映射
来源：http://eht.jlsjyb.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://eag.cdnleiting.top

[T07] Kotlin：集合过滤
来源：http://nyu.tarul.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://jsb.jqgfzy.top

[T08] Kotlin：数据类
来源：http://bye.zhiwuduotai.top

data class User(val name: String, val age: Int)
来源：http://blu.pycfn.com

[T09] Kotlin：扩展函数
来源：http://nbw.fanxiaobao.xyz

fun String.exclaim() = this + "!"
来源：http://yac.dianchejie.cn

[T10] Kotlin：默认参数
来源：http://dir.zdbjq.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://tzt.9152youxi.cn

[T11] Kotlin：协程
来源：http://yll.zhixingplan.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://adf.hnxiangtu.top

[T12] Kotlin：解构声明
来源：http://qki.zhaomingkeji.xyz

val (a, b) = Pair(1, 2)
来源：http://vgy.yongpay.top

[T13] Kotlin：只读 Map
来源：http://bpe.yj20258888.top

val m = mapOf("a" to 1)
来源：http://wka.tanke756.top

[T14] Kotlin：循环
来源：http://obx.bbcook.cn

for (i in 1..10) println(i)
来源：http://jyl.fengsongda.top

[T15] Kotlin：接口
来源：http://nec.ywan-chungtsiang.top

interface Shape { fun area(): Double }
来源：http://vgv.svipenyu.cn

[T16] Swift：Hello World
来源：http://ipc.bbcook.cn

print("Hello")
来源：http://nxn.yfazqb.com

[T17] Swift：变量与常量
来源：http://lbi.0kj1m.cn

var a = 1;  let b = 2
来源：http://xvs.yangfankeji.com

[T18] Swift：字符串插值
来源：http://xuk.tanke756.top

"值: \(b)"
来源：http://rqx.zhiwuduotai.top

[T19] Swift：可选绑定
来源：http://vdh.xylfe.cn

if let n = opt { print(n) }
来源：http://evu.yangfankeji.com

[T20] Swift：数组操作
来源：http://gwj.yuxming.cn

var a = [1, 2, 3];  a.append(4)
来源：http://ass.vqdsnc.cn

[T21] Swift：遍历
来源：http://nfh.quarkkingdee.top

for x in a { print(x) }
来源：http://fbl.bjfxy.top

[T22] Swift：字典
来源：http://lto.yuanzhike.top

var d = ["a": 1];  d["b"] = 2
来源：http://cox.yvedp.cn

[T23] Swift：函数
来源：http://qol.meibo888.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://ilk.cheryme.top

[T24] Swift：闭包
来源：http://nbl.daxiang520.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://pdm.zdbjq.cn

[T25] Swift：结构体
来源：http://cjq.pycfn.com

struct P { var x: Int }
来源：http://twy.jinyuanbaomall.cn

[T26] Swift：类与重写
来源：http://zhn.jinghuilouyu.cn

class A: Base { override func f() {} }
来源：http://qcd.smart0.xyz

[T27] Swift：错误处理
来源：http://pcs.ywan-chungtsiang.top

do { try f() } catch { print(error) }
来源：http://dbu.cqqwz.cn

[T28] Swift：枚举
来源：http://qpc.ywan-chungtsiang.top

enum Color { case red, green }
来源：http://eap.chenjidiqi.icu

[T29] Swift：guard 提前返回
来源：http://hkf.chenlongwang.top

guard let x = opt else { return }
来源：http://whd.ydzc1.top

[T30] Swift：协议
来源：http://gyg.yangfankeji.com

protocol Shape { func area() -> Double }
来源：http://ibf.epnwcf.com

[T31] Lua：Hello World
来源：http://vyc.dianchejie.cn

print("Hello")
来源：http://oox.jyoumei.cn

[T32] Lua：局部变量
来源：http://xni.yueranfly.top

local a = 1
来源：http://jdr.hywenlv.cn

[T33] Lua：表（数组）
来源：http://ako.yfazqb.com

local t = {1, 2, 3};  t[4] = 4
来源：http://oah.zdqjudy.top

[T34] Lua：遍历表
来源：http://plh.ehwqpu.com

for i, v in ipairs(t) do print(i, v) end
来源：http://hvw.jyoumei.cn

[T35] Lua：字典表
来源：http://ivb.xuetiantiany.cn

local d = { a = 1 };  d.b = 2
来源：http://mir.jqgfzy.top

[T36] Lua：函数
来源：http://yny.sjlbkw.cn

function add(a, b) return a + b end
来源：http://yth.cheryme.top

[T37] Lua：字符串拼接
来源：http://yla.pengpengdd.cyou

"a" .. "b"
来源：http://plm.yvedp.cn

[T38] Lua：条件
来源：http://npv.cucudq.cn

if x > 0 then print("正") end
来源：http://cvx.snrcjt.cn

[T39] Lua：模式匹配
来源：http://tcp.hesvh.cn

string.find(s, "%d+")
来源：http://bkv.feifeiyinyue.top

[T40] Lua：元表
来源：http://pkt.dianchejie.cn

setmetatable({}, { __index = base })
来源：http://bzh.zhengqikj.top

[T41] Perl：Hello World
来源：http://nxq.hnqzz.top

print "Hello\n";
来源：http://ipm.jyoumei.cn

[T42] Perl：变量类型
来源：http://dgh.fzhhl.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://los.xuanzx.com

[T43] Perl：字符串插值
来源：http://duz.hnxiangtu.top

"值: $a"
来源：http://usx.jyoumei.cn

[T44] Perl：条件
来源：http://sfn.sysykeji.top

if ($a > 0) { print "正"; }
来源：http://wwa.kuanghao11.cn

[T45] Perl：数组遍历
来源：http://uyn.shuidangran.top

for my $x (@arr) { print $x; }
来源：http://drl.ywan-chungtsiang.top

[T46] Perl：哈希操作
来源：http://kby.dianchejie.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://erv.cucudq.cn

[T47] Perl：正则捕获
来源：http://zhz.smart0.xyz

if ($s =~ /(\d+)/) { print $1; }
来源：http://fnd.ehwqpu.com

[T48] Perl：正则替换
来源：http://ixp.fengsongda.top

$s =~ s/old/new/g;
来源：http://vib.c1oappe.top

[T49] Perl：函数
来源：http://gcp.ppjwa.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://ndd.fktsv.cn

[T50] Perl：逐行读文件
来源：http://hmd.snrcjt.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://dbo.zhengqikj.top

while (my $line = <$fh>) { print $line; }
来源：http://vmo.iojbl.cn

[T51] Scala：Hello World
来源：http://xmt.jinqigfzy.top

println("Hello")
来源：http://jjt.hongshengwenyu.top

[T52] Scala：变量
来源：http://sya.xinyue.icu

val a = 1;  var b = 2
来源：http://tic.nanxuanxn.top

[T53] Scala：字符串插值
来源：http://quv.pycfn.com

s"值: $b"
来源：http://vny.xuanzx.com

[T54] Scala：集合映射
来源：http://jut.jinqigufen.top

List(1, 2, 3).map(_ * 2)
来源：http://lct.guowangkeji.top

[T55] Scala：集合过滤
来源：http://eac.zhijiandao.cn

List(1, 2, 3).filter(_ > 1)
来源：http://mlg.dashuyun.cn

[T56] Scala：样例类
来源：http://qtj.shuidangran.top

case class User(name: String, age: Int)
来源：http://ray.vqdsnc.cn

[T57] Scala：模式匹配
来源：http://mui.hnqzz.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://rdn.chenlongwang.top

[T58] Scala：函数定义
来源：http://sgp.guannengcc.top

def add(a: Int, b: Int): Int = a + b
来源：http://puy.kuanghao11.cn

[T59] Scala：循环
来源：http://yci.shuidangran.top

for (i <- 1 to 10) println(i)
来源：http://isl.gaohongyu789.top

[T60] Scala：折叠
来源：http://efp.cashguo.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://eco.fengsongda.top

================================================================================
来源：http://dcz.feifeiyinyue.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://wmo.ywan-chungtsiang.top

================================================================================
来源：http://mwo.zdqjudy.top

[U01] Py：创建虚拟环境
来源：http://fbs.sxryk.cn

python -m venv .venv && source .venv/bin/activate
来源：http://lkt.daxiang520.top

[U02] Py：导出 / 安装依赖
来源：http://rmo.yfazqb.com

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://osa.bjfxy.top

[U03] Py：加载 .env 配置
来源：http://bjy.hnxiangtu.top

from dotenv import load_dotenv; load_dotenv()
来源：http://yzx.zhiwuduotai.top

[U04] Py：变量调试打印
来源：http://iih.hnxiangtu.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://dks.gaohongyu789.top


<!-- 参考信息 -->