代发 wailian999

free -h;  ps aux | grep nginx
来源：http://hrg.jinyuanbaomall.cn

[R64] 结束进程
来源：http://cct.shzxlz.cn

kill -9 $(pgrep -f app.py)
来源：http://dhz.yj20258888.top

[R65] 查看端口占用
来源：http://wax.wangshuangyany.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://jjc.zhongyouzk.top

[R66] 定时任务
来源：http://efn.ctjpmb.com

crontab -e;  crontab -l
来源：http://dby.chenzaomai.com

[R67] 生成随机十六进制串
来源：http://ypb.9152youxi.cn

openssl rand -hex 16
来源：http://yld.yj20258888.top

[R68] 计算文件校验值
来源：http://gwt.guowangkeji.top

sha256sum a.txt;  md5sum a.txt
来源：http://chv.gzhubu.top

[R69] 生成随机密码
来源：http://vbb.quarkkingdee.top

head -c 16 /dev/urandom | base64
来源：http://hzr.xinyue.icu

[R70] 时间戳与互转
来源：http://weg.tian-w.cn

date +%s;  date -d @1700000000
来源：http://rbt.cashguo.top

[R71] 日期格式化
来源：http://kjw.kuanghao11.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://vqy.birdmap.top

[R72] 等待端口就绪
来源：http://bes.zdqjudy.top

until nc -z localhost 3306; do sleep 1; done
来源：http://him.ydjk.org.cn

[R73] 分割大日志
来源：http://yxw.sweek.top

split -l 1000 big.log part_
来源：http://mkv.daria6918.cn

[R74] 批量重命名
来源：http://vfb.vehdjk.com

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://oyd.hesvh.cn

[R75] 导出环境变量
来源：http://lkz.jqgfzy.top

export PATH="$HOME/bin:$PATH"
来源：http://cae.hcnkem.com

[R76] 使用临时文件
来源：http://txv.ctjpmb.com

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://dju.jiagoushi.top

[R77] 读取用户输入
来源：http://gzk.cheryme.top

read -rp "请输入: " ans
来源：http://oxj.tanke756.top

[R78] 交互式菜单
来源：http://kgu.havefunace.top

select opt in a b c; do echo "$opt"; break; done
来源：http://eqq.fengsongda.top

[R79] 解析命令行选项
来源：http://huq.cheryme.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://ytt.zdqjudy.top

[R80] 查看脚本执行耗时
来源：http://hiy.jianghu66.top

time ./run.sh
来源：http://fhs.hnqzz.top

================================================================================
来源：http://djw.vqdsnc.cn

S. C / C++ 专题
来源：http://jnu.yfazqb.com

================================================================================
来源：http://wxw.redwolf501.top

[S01] C：Hello World
来源：http://afl.ydjk.org.cn

#include <stdio.h>
来源：http://efn.yuanzhike.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://qpg.redwolf501.top

[S02] C：变量与格式化输出
来源：http://xxh.sjlbkw.cn

int a = 10; printf("%d\n", a);
来源：http://syn.fzhhl.top

[S03] C：读入整数
来源：http://kuh.yuxming.cn

int x; scanf("%d", &x);
来源：http://lns.hnxiangtu.top

[S04] C：字符串复制
来源：http://hhl.havefunace.top

char dst[32]; strcpy(dst, "hi");
来源：http://zjq.sufxvd.cn

[S05] C：字符串长度
来源：http://jsi.snrcjt.cn

strlen(s)
来源：http://ulo.jqgfzy.top

[S06] C：字符串比较
来源：http://gnk.cashguo.top

strcmp(a, b) == 0
来源：http://ujf.birdmap.top

[S07] C：数组遍历求和
来源：http://oud.feifeiyinyue.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://wvn.cashguo.top

[S08] C：动态内存分配与释放
来源：http://uqg.guannengcc.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://rqj.guannengcc.top

[S09] C：结构体定义与初始化
来源：http://xae.quarkkingdee.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://rhl.ydjk.org.cn

[S10] C：指针与解引用
来源：http://cxc.guowangkeji.top

int *p = &a;  *p = 5;
来源：http://ijd.fehbvm.com

[S11] C：逐行读文件
来源：http://upz.gaohongyu789.top

FILE *f = fopen("a.txt", "r");
来源：http://swp.jinqigfzy.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://eix.yonumen.top

fclose(f);
来源：http://pfi.ydjk.org.cn

[S12] C：写文件
来源：http://cko.chenjidiqi.icu

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://jmc.gotoacloud.top

[S13] C：宏定义
来源：http://znm.iojbl.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://xxu.birdmap.top

[S14] C：枚举
来源：http://pvt.ivvv.top

enum Color { RED, GREEN, BLUE };
来源：http://quk.yonumen.top

[S15] C：类型转换
来源：http://epw.jlsjyb.cn

(double) a / b
来源：http://lzx.xuanzx.com

[S16] C：位操作置位
来源：http://hmu.meibo888.top

x |= (1 << 3);
来源：http://pmw.daxiang520.top

[S17] C：安全拼接字符串
来源：http://orb.uphjek.com

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://mxr.9152youxi.cn

[S18] C：命令行参数
来源：http://wse.guowangkeji.top

int main(int argc, char **argv)
来源：http://cxv.zhijiandao.cn

[S19] C：快速排序
来源：http://iyn.ehwqpu.com

qsort(a, n, sizeof(int), cmp);
来源：http://jlz.jinghuilouyu.cn

[S20] C：二分查找
来源：http://oja.aibaodan.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://jax.pengpengdd.cyou

[S21] C：字符类别判断
来源：http://oxg.havefunace.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://eoj.fengsongda.top

[S22] C：字符串转数字
来源：http://qps.cdnleiting.top

atoi("42");  strtod("3.14", NULL);
来源：http://jyk.wangshuangyany.cn

[S23] C：随机数
来源：http://fxy.316326.xyz

srand(time(NULL));  int r = rand() % 100;
来源：http://ikn.zhengqikj.top

[S24] C：获取本地时间
来源：http://tgv.wangdashe.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://eey.dashuyun.cn

[S25] C：内存拷贝
来源：http://rzx.andypj.xyz

memcpy(dst, src, n);
来源：http://ehw.iojbl.cn

[S26] C：内存清零
来源：http://vuz.birdmap.top

memset(a, 0, sizeof a);
来源：http://yir.hnxiangtu.top

[S27] C：定义常量
来源：http://xzy.ctjpmb.com

const double PI = 3.14159;
来源：http://iat.sxryk.cn

[S28] C：静态变量
来源：http://nma.jinghuilouyu.cn

static int counter = 0;
来源：http://wfj.yj20258888.top

[S29] C：变参函数
来源：http://yrx.yj202588.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://zwp.jyoumei.cn

[S30] C：头文件保护
来源：http://kir.yvedp.cn

#ifndef X_H
来源：http://miu.hongshengwenyu.top

#define X_H
来源：http://lvd.hnxiangtu.top

#endif
来源：http://mkw.daxiang520.top

[S31] C++：Hello World
来源：http://pms.0kj1m.cn

#include <iostream>
来源：http://ugs.haohaochexian.top

int main() { std::cout << "Hello\n"; }
来源：http://njv.andypj.xyz

[S32] C++：字符串
来源：http://ahc.cashguo.top

std::string s = "hi";  s += "!";
来源：http://gsf.nwbrower.top

[S33] C++：vector 增删
来源：http://gck.wangdashe.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://avv.hcnkem.com

[S34] C++：遍历 vector
来源：http://xuh.cucudq.cn

for (auto &x : v) { std::cout << x; }
来源：http://pqc.cheryme.top

[S35] C++：map
来源：http://nko.zycfv.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://jph.gogol.net.cn

[S36] C++：unordered_map
来源：http://ksv.smart0.xyz

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://apb.uphjek.com

[S37] C++：set
来源：http://kla.vqdsnc.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://ski.haohaochexian.top

[S38] C++：排序
来源：http://vfz.9152youxi.cn

std::sort(v.begin(), v.end());
来源：http://jys.hcnkem.com

[S39] C++：自定义比较器排序
来源：http://yas.dashuyun.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://xit.gotoacloud.top

[S40] C++：查找元素
来源：http://fho.dashuyun.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://qlx.shuidangran.top

[S41] C++：类与构造函数
来源：http://dua.iojbl.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://vev.daxiang520.top

[S42] C++：继承与虚函数
来源：http://pzz.jinqigfzy.top

class B : public Base { public: void f() override {} };
来源：http://gny.pycfn.com

[S43] C++：智能指针
来源：http://njy.yangfankeji.com

auto p = std::make_unique<int>(5);
来源：http://sax.zhaomingkeji.xyz

[S44] C++：引用传参
来源：http://lkw.chenzaomai.com

void inc(int &x) { ++x; }
来源：http://auj.snrcjt.cn

[S45] C++：lambda
来源：http://oyl.nwbrower.top

auto add = [](int a, int b) { return a + b; };
来源：http://azr.hcnkem.com

[S46] C++：函数模板
来源：http://cuc.mhx1999.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://obo.epnwcf.com

[S47] C++：结构化绑定遍历
来源：http://pau.daria6918.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://lnx.kuanghao11.cn

[S48] C++：逐行读文件
来源：http://xwi.dianchejie.cn

std::ifstream in("a.txt");  std::string line;
来源：http://jro.aizwys.cn

while (std::getline(in, line)) { }
来源：http://mjg.gogol.net.cn

[S49] C++：写文件
来源：http://knt.yonumen.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://bae.yj20258.top

[S50] C++：格式化数字
来源：http://lij.ppjwa.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://lek.shangyingyoupin.top

[S51] C++：显式类型转换
来源：http://mpk.jinyuanbaomall.cn

static_cast<double>(a) / b
来源：http://tyo.zhongyouzk.top

[S52] C++：const 与 noexcept
来源：http://bus.yueranfly.top

int size() const noexcept { return n_; }
来源：http://yhu.chenlongwang.top

[S53] C++：移动语义
来源：http://tuz.vehdjk.com

std::vector<int> w = std::move(v);
来源：http://qnu.ivvv.top

[S54] C++：异常处理
来源：http://uss.guowangkeji.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://vhe.bbcook.cn

[S55] C++：结构化绑定
来源：http://nny.9152youxi.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://dmo.jinqigufen.top

[S56] C++：optional
来源：http://nrt.redwolf501.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://ssd.gzhubu.top

[S57] C++：编译期常量
来源：http://ibh.redwolf501.top

constexpr int N = 10;
来源：http://xea.jlsjyb.cn

[S58] C++：命名空间
来源：http://kdb.andypj.xyz

namespace ns { int f() { return 1; } }
来源：http://jro.gzhubu.top

[S59] C++：静态断言
来源：http://har.vqdsnc.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://fci.hnxiangtu.top

[S60] C++：遍历并删除元素
来源：http://mhb.nwbrower.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://alo.zdbjq.cn

================================================================================
来源：http://mcg.c1oappe.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://fpv.shzxlz.cn

================================================================================
来源：http://uwe.zdqjudy.top

[T01] Kotlin：Hello World
来源：http://brk.vehdjk.com

println("Hello")
来源：http://tyi.yuanzhike.top

[T02] Kotlin：变量
来源：http://xok.hcnkem.com

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://cok.zycfv.cn

[T03] Kotlin：字符串模板
来源：http://iky.c1oappe.top

"值: $b"
来源：http://tzd.daria6918.cn

[T04] Kotlin：空安全
来源：http://tbh.iojbl.cn

val n: String? = null;  n?.length
来源：http://gau.fzhhl.top

[T05] Kotlin：when 表达式
来源：http://reh.cheryme.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://mcf.tian-w.cn

[T06] Kotlin：集合映射
来源：http://xxx.jianghu66.top

listOf(1, 2, 3).map { it * 2 }
来源：http://jok.yvedp.cn

[T07] Kotlin：集合过滤
来源：http://drd.sweek.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://bln.yuanzhike.top

[T08] Kotlin：数据类
来源：http://aqu.fzhhl.top

data class User(val name: String, val age: Int)
来源：http://ljy.jiagoushi.top

[T09] Kotlin：扩展函数
来源：http://knu.sufxvd.cn

fun String.exclaim() = this + "!"
来源：http://wgj.0kj1m.cn

[T10] Kotlin：默认参数
来源：http://ofz.ydzc1.top

fun greet(name: String = "World") = "Hi $name"
来源：http://mkb.ydzc1.top

[T11] Kotlin：协程
来源：http://npr.52xcode.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://skw.chenjidiqi.icu

[T12] Kotlin：解构声明
来源：http://hrb.zhaomingkeji.xyz

val (a, b) = Pair(1, 2)
来源：http://wdm.jiagoushi.top

[T13] Kotlin：只读 Map
来源：http://inr.aibaodan.cn

val m = mapOf("a" to 1)
来源：http://pml.316326.xyz

[T14] Kotlin：循环
来源：http://dgh.ydzc1.top

for (i in 1..10) println(i)
来源：http://feb.xuanzx.com

[T15] Kotlin：接口
来源：http://zza.guannengcc.top

interface Shape { fun area(): Double }
来源：http://qpe.sysykeji.top

[T16] Swift：Hello World
来源：http://vgb.daxiang520.top

print("Hello")
来源：http://nvk.epnwcf.com

[T17] Swift：变量与常量
来源：http://rlr.hongshengwenyu.top

var a = 1;  let b = 2
来源：http://rqz.ctjpmb.com

[T18] Swift：字符串插值
来源：http://kxr.fanxiaobao.xyz

"值: \(b)"
来源：http://xwq.316326.xyz

[T19] Swift：可选绑定
来源：http://zjs.zdqjudy.top

if let n = opt { print(n) }
来源：http://dlf.yj202588.top

[T20] Swift：数组操作
来源：http://vbb.xziqi.cn

var a = [1, 2, 3];  a.append(4)
来源：http://jpb.jinghuilouyu.cn

[T21] Swift：遍历
来源：http://noh.yanxiufei.cn

for x in a { print(x) }
来源：http://juk.yuxming.cn

[T22] Swift：字典
来源：http://qrk.zhoulong.xyz

var d = ["a": 1];  d["b"] = 2
来源：http://njz.epnwcf.com

[T23] Swift：函数
来源：http://inx.jinyuanbaomall.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://nym.yuxming.cn

[T24] Swift：闭包
来源：http://bde.yangfankeji.com

let f = { (x: Int) -> Int in x * 2 }
来源：http://slr.epnwcf.com

[T25] Swift：结构体
来源：http://eia.cdnleiting.top

struct P { var x: Int }
来源：http://nps.epnwcf.com

[T26] Swift：类与重写
来源：http://hil.ydzc1.top

class A: Base { override func f() {} }
来源：http://mbh.sysykeji.top

[T27] Swift：错误处理
来源：http://vzz.nanxinkj.top

do { try f() } catch { print(error) }
来源：http://mlq.ybcxt.top

[T28] Swift：枚举
来源：http://ino.nwbrower.top

enum Color { case red, green }
来源：http://qzi.cqqwz.cn

[T29] Swift：guard 提前返回
来源：http://gfr.0kj1m.cn

guard let x = opt else { return }
来源：http://ybg.yueranfly.top

[T30] Swift：协议
来源：http://vwz.ywan-chungtsiang.top

protocol Shape { func area() -> Double }
来源：http://hgh.zycfv.cn

[T31] Lua：Hello World
来源：http://kzz.ctjpmb.com

print("Hello")
来源：http://trn.ivvv.top

[T32] Lua：局部变量
来源：http://ifr.vqdsnc.cn

local a = 1
来源：http://elk.xingfuxueyuan.xyz

[T33] Lua：表（数组）
来源：http://nzp.bbcook.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://cwr.jqgufenzy.top

[T34] Lua：遍历表
来源：http://hye.dianchejie.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://uct.xuanzx.com

[T35] Lua：字典表
来源：http://get.chenzaomai.com

local d = { a = 1 };  d.b = 2
来源：http://nnl.aizwys.cn

[T36] Lua：函数
来源：http://wrp.kuanghao11.cn

function add(a, b) return a + b end
来源：http://vmp.ivvv.top

[T37] Lua：字符串拼接
来源：http://fpi.sweek.top

"a" .. "b"
来源：http://hqx.0kj1m.cn

[T38] Lua：条件
来源：http://naj.tanke756.top

if x > 0 then print("正") end
来源：http://grn.jiagoushi.top

[T39] Lua：模式匹配
来源：http://wlf.andypj.xyz

string.find(s, "%d+")
来源：http://nby.xingfuxueyuan.xyz

[T40] Lua：元表
来源：http://frg.guannengcc.top

setmetatable({}, { __index = base })
来源：http://tkj.yanxiufei.cn

[T41] Perl：Hello World
来源：http://tbh.ivvv.top

print "Hello\n";
来源：http://gdh.ywan-chungtsiang.top

[T42] Perl：变量类型
来源：http://cpv.xuetiantiany.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://ava.yuxming.cn

[T43] Perl：字符串插值
来源：http://aci.cashguo.top

"值: $a"
来源：http://xbe.sufxvd.cn

[T44] Perl：条件
来源：http://ugi.jinyuanbaomall.cn

if ($a > 0) { print "正"; }
来源：http://bry.daria6918.cn

[T45] Perl：数组遍历
来源：http://brb.hfpthk.cn

for my $x (@arr) { print $x; }
来源：http://jtx.fktsv.cn

[T46] Perl：哈希操作
来源：http://pmc.feifeiyinyue.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://urr.9152youxi.cn

[T47] Perl：正则捕获
来源：http://yys.mhx1999.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://ary.chenjidiqi.icu

[T48] Perl：正则替换
来源：http://erg.yuanzhike.top

$s =~ s/old/new/g;
来源：http://gov.snrcjt.cn

[T49] Perl：函数
来源：http://pkq.yanxiufei.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://rze.sysykeji.top

[T50] Perl：逐行读文件
来源：http://zbu.bjfxy.top

open my $fh, "<", "a.txt" or die $!;
来源：http://wok.hcnkem.com

while (my $line = <$fh>) { print $line; }
来源：http://wtm.sjlbkw.cn

[T51] Scala：Hello World
来源：http://lid.cheryme.top

println("Hello")
来源：http://uwc.jqgfzy.top

[T52] Scala：变量
来源：http://epp.ywan-chungtsiang.top

val a = 1;  var b = 2
来源：http://yvo.ydjk.org.cn

[T53] Scala：字符串插值
来源：http://kpm.tarul.cn

s"值: $b"
来源：http://ngj.zycfv.cn

[T54] Scala：集合映射
来源：http://baf.wangdashe.top

List(1, 2, 3).map(_ * 2)
来源：http://haj.yj20258888.top

[T55] Scala：集合过滤
来源：http://qdx.zdbjq.cn

List(1, 2, 3).filter(_ > 1)
来源：http://vqe.jinyuanbaomall.cn

[T56] Scala：样例类
来源：http://eqa.mhx1999.top

case class User(name: String, age: Int)
来源：http://ibl.vehdjk.com

[T57] Scala：模式匹配
来源：http://met.guannengcc.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://bke.zhijiandao.cn

[T58] Scala：函数定义
来源：http://jig.jinqigufen.top

def add(a: Int, b: Int): Int = a + b
来源：http://dpy.zycfv.cn

[T59] Scala：循环
来源：http://vmb.xuetiantiany.cn

for (i <- 1 to 10) println(i)
来源：http://nzu.gaohongyu789.top

[T60] Scala：折叠
来源：http://kcf.zhixingplan.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://dce.jinqigufen.top

================================================================================
来源：http://yrq.cucudq.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://upc.zdqjudy.top

================================================================================
来源：http://yls.andypj.xyz

[U01] Py：创建虚拟环境
来源：http://ecw.yuxming.cn

python -m venv .venv && source .venv/bin/activate
来源：http://ghc.tian-w.cn

[U02] Py：导出 / 安装依赖
来源：http://imv.xuanzx.com

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://urm.birdmap.top

[U03] Py：加载 .env 配置
来源：http://hjq.zhaomingkeji.xyz

from dotenv import load_dotenv; load_dotenv()
来源：http://dcf.tanke756.top

[U04] Py：变量调试打印
来源：http://zgx.ydzc1.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://tew.ywan-chungtsiang.top


<!-- 参考信息 -->