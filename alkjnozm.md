代发 wailian999

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://uzx.316326.xyz

[S21] C：字符类别判断
来源：http://buu.xylfe.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://taq.birdmap.top

[S22] C：字符串转数字
来源：http://dfu.jqgufenzy.top

atoi("42");  strtod("3.14", NULL);
来源：http://wwq.xinyue.icu

[S23] C：随机数
来源：http://xnb.sufxvd.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://xdh.vehdjk.com

[S24] C：获取本地时间
来源：http://too.tarul.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://sff.c1oappe.top

[S25] C：内存拷贝
来源：http://xoz.hammf.cn

memcpy(dst, src, n);
来源：http://otc.guowangkeji.top

[S26] C：内存清零
来源：http://fuk.wangdashe.top

memset(a, 0, sizeof a);
来源：http://ssw.sweek.top

[S27] C：定义常量
来源：http://zup.jinqigufen.top

const double PI = 3.14159;
来源：http://qvq.bbcook.cn

[S28] C：静态变量
来源：http://vai.hywenlv.cn

static int counter = 0;
来源：http://gbc.haohaochexian.top

[S29] C：变参函数
来源：http://bfc.hfpthk.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://qbp.hongshengwenyu.top

[S30] C：头文件保护
来源：http://gqh.wangshuangyany.cn

#ifndef X_H
来源：http://jvx.nanxuanxn.top

#define X_H
来源：http://von.daria6918.cn

#endif
来源：http://vfp.gzhubu.top

[S31] C++：Hello World
来源：http://vwv.dashuyun.cn

#include <iostream>
来源：http://thh.hnqzz.top

int main() { std::cout << "Hello\n"; }
来源：http://wnw.bjfxy.top

[S32] C++：字符串
来源：http://rtm.yueranfly.top

std::string s = "hi";  s += "!";
来源：http://kqb.xylfe.cn

[S33] C++：vector 增删
来源：http://xef.daxiang520.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://nqf.haohaochexian.top

[S34] C++：遍历 vector
来源：http://fbb.quarkkingdee.top

for (auto &x : v) { std::cout << x; }
来源：http://fwr.yuanzhike.top

[S35] C++：map
来源：http://sdl.cdnleiting.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://chj.ywan-chungtsiang.top

[S36] C++：unordered_map
来源：http://paq.cheryme.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://cas.sweek.top

[S37] C++：set
来源：http://qei.aibaodan.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://xrm.sxryk.cn

[S38] C++：排序
来源：http://rhd.shangyingyoupin.top

std::sort(v.begin(), v.end());
来源：http://xuq.andypj.xyz

[S39] C++：自定义比较器排序
来源：http://ped.yuxming.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://atw.ydzc1.top

[S40] C++：查找元素
来源：http://uxd.nanxuanxn.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://haa.shuidangran.top

[S41] C++：类与构造函数
来源：http://dqf.jyoumei.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://glp.yuxming.cn

[S42] C++：继承与虚函数
来源：http://sfm.ehwqpu.com

class B : public Base { public: void f() override {} };
来源：http://khn.ybcxt.top

[S43] C++：智能指针
来源：http://dob.birdmap.top

auto p = std::make_unique<int>(5);
来源：http://hun.zdqjudy.top

[S44] C++：引用传参
来源：http://djs.yj20258888.top

void inc(int &x) { ++x; }
来源：http://lie.hesvh.cn

[S45] C++：lambda
来源：http://iij.xziqi.cn

auto add = [](int a, int b) { return a + b; };
来源：http://yef.cdnleiting.top

[S46] C++：函数模板
来源：http://fhd.zhongyouzk.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://zxj.uphjek.com

[S47] C++：结构化绑定遍历
来源：http://odf.iojbl.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://fhh.pycfn.com

[S48] C++：逐行读文件
来源：http://qoo.ydjk.org.cn

std::ifstream in("a.txt");  std::string line;
来源：http://syk.wangshuangyany.cn

while (std::getline(in, line)) { }
来源：http://blm.jiagoushi.top

[S49] C++：写文件
来源：http://ngi.zhijiandao.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://zbr.meibo888.top

[S50] C++：格式化数字
来源：http://oyh.zdqjudy.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://qyn.hfpthk.cn

[S51] C++：显式类型转换
来源：http://yma.pycfn.com

static_cast<double>(a) / b
来源：http://ska.ivvv.top

[S52] C++：const 与 noexcept
来源：http://cyr.quarkkingdee.top

int size() const noexcept { return n_; }
来源：http://djz.tian-w.cn

[S53] C++：移动语义
来源：http://bbh.hnxiangtu.top

std::vector<int> w = std::move(v);
来源：http://muy.cqqwz.cn

[S54] C++：异常处理
来源：http://szo.52xcode.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://ptq.zhengqikj.top

[S55] C++：结构化绑定
来源：http://bwr.aizwys.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://jdh.epnwcf.com

[S56] C++：optional
来源：http://hpx.xingfuxueyuan.xyz

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://pda.316326.xyz

[S57] C++：编译期常量
来源：http://ogi.bbcook.cn

constexpr int N = 10;
来源：http://sng.tanke756.top

[S58] C++：命名空间
来源：http://zqd.cdnleiting.top

namespace ns { int f() { return 1; } }
来源：http://use.yj202588.top

[S59] C++：静态断言
来源：http://jrv.tarul.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://mit.yonumen.top

[S60] C++：遍历并删除元素
来源：http://nll.tianlin.xyz

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://izd.jqgufenzy.top

================================================================================
来源：http://ttu.zhijiandao.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://jcp.jyoumei.cn

================================================================================
来源：http://ypb.dianchejie.cn

[T01] Kotlin：Hello World
来源：http://vbi.mhx1999.top

println("Hello")
来源：http://fdh.zdqjudy.top

[T02] Kotlin：变量
来源：http://rqc.jiagoushi.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://rco.fehbvm.com

[T03] Kotlin：字符串模板
来源：http://ryl.xingfuxueyuan.xyz

"值: $b"
来源：http://fqo.mhx1999.top

[T04] Kotlin：空安全
来源：http://yuq.zhengqikj.top

val n: String? = null;  n?.length
来源：http://mpv.c1oappe.top

[T05] Kotlin：when 表达式
来源：http://tle.vqdsnc.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://sjn.zhiwuduotai.top

[T06] Kotlin：集合映射
来源：http://lzw.snrcjt.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://fxx.wangdashe.top

[T07] Kotlin：集合过滤
来源：http://eiu.316326.xyz

listOf(1, 2, 3).filter { it > 1 }
来源：http://bws.gotoacloud.top

[T08] Kotlin：数据类
来源：http://dxj.cqqwz.cn

data class User(val name: String, val age: Int)
来源：http://wiz.daria6918.cn

[T09] Kotlin：扩展函数
来源：http://hyk.redwolf501.top

fun String.exclaim() = this + "!"
来源：http://ewh.meibo888.top

[T10] Kotlin：默认参数
来源：http://hnr.ctjpmb.com

fun greet(name: String = "World") = "Hi $name"
来源：http://tdw.xingfuxueyuan.xyz

[T11] Kotlin：协程
来源：http://syr.guannengcc.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://yfp.hfpthk.cn

[T12] Kotlin：解构声明
来源：http://asx.aibaodan.cn

val (a, b) = Pair(1, 2)
来源：http://xsb.chenjidiqi.icu

[T13] Kotlin：只读 Map
来源：http://tsx.ydjk.org.cn

val m = mapOf("a" to 1)
来源：http://jux.shanyushiyangtech.top

[T14] Kotlin：循环
来源：http://jiz.yonumen.top

for (i in 1..10) println(i)
来源：http://lls.ppjwa.cn

[T15] Kotlin：接口
来源：http://hpt.jiagoushi.top

interface Shape { fun area(): Double }
来源：http://zzw.pycfn.com

[T16] Swift：Hello World
来源：http://doh.nwbrower.top

print("Hello")
来源：http://hug.fehbvm.com

[T17] Swift：变量与常量
来源：http://kkb.birdmap.top

var a = 1;  let b = 2
来源：http://qpj.aizwys.cn

[T18] Swift：字符串插值
来源：http://yor.bbcook.cn

"值: \(b)"
来源：http://aqe.ywan-chungtsiang.top

[T19] Swift：可选绑定
来源：http://yxp.haohaochexian.top

if let n = opt { print(n) }
来源：http://val.ctjpmb.com

[T20] Swift：数组操作
来源：http://sgv.yuanzhike.top

var a = [1, 2, 3];  a.append(4)
来源：http://zod.hammf.cn

[T21] Swift：遍历
来源：http://hbn.quarkkingdee.top

for x in a { print(x) }
来源：http://rtu.ybcxt.top

[T22] Swift：字典
来源：http://xtl.zhixingplan.top

var d = ["a": 1];  d["b"] = 2
来源：http://wip.sufxvd.cn

[T23] Swift：函数
来源：http://pfs.shanyushiyangkeji.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://sca.xinyue.icu

[T24] Swift：闭包
来源：http://ydz.zdbjq.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://fmu.hongshengwenyu.top

[T25] Swift：结构体
来源：http://dnp.shangyingyoupin.top

struct P { var x: Int }
来源：http://eev.yj20258.top

[T26] Swift：类与重写
来源：http://wst.shanyushiyangtech.top

class A: Base { override func f() {} }
来源：http://tvw.yuanzhike.top

[T27] Swift：错误处理
来源：http://ipa.nanxuanxn.top

do { try f() } catch { print(error) }
来源：http://cok.yanxiufei.cn

[T28] Swift：枚举
来源：http://gqo.yanxiufei.cn

enum Color { case red, green }
来源：http://igx.xingfuxueyuan.xyz

[T29] Swift：guard 提前返回
来源：http://raa.jlsjyb.cn

guard let x = opt else { return }
来源：http://esu.hesvh.cn

[T30] Swift：协议
来源：http://bqe.quarkkingdee.top

protocol Shape { func area() -> Double }
来源：http://zoa.yuanzhike.top

[T31] Lua：Hello World
来源：http://zjz.vqdsnc.cn

print("Hello")
来源：http://pqf.ydjk.org.cn

[T32] Lua：局部变量
来源：http://pjd.redwolf501.top

local a = 1
来源：http://xxz.jiagoushi.top

[T33] Lua：表（数组）
来源：http://jfw.guowangkeji.top

local t = {1, 2, 3};  t[4] = 4
来源：http://ywx.zhijiandao.cn

[T34] Lua：遍历表
来源：http://gjp.hcnkem.com

for i, v in ipairs(t) do print(i, v) end
来源：http://nlu.yuanzhike.top

[T35] Lua：字典表
来源：http://bkr.shanyushiyangtech.top

local d = { a = 1 };  d.b = 2
来源：http://cto.jianghu66.top

[T36] Lua：函数
来源：http://iuh.xuanzx.com

function add(a, b) return a + b end
来源：http://gmy.quarkkingdee.top

[T37] Lua：字符串拼接
来源：http://xhb.ydjk.org.cn

"a" .. "b"
来源：http://pwv.vqdsnc.cn

[T38] Lua：条件
来源：http://woz.yj202588.top

if x > 0 then print("正") end
来源：http://vxz.smart0.xyz

[T39] Lua：模式匹配
来源：http://crd.9152youxi.cn

string.find(s, "%d+")
来源：http://wod.sysykeji.top

[T40] Lua：元表
来源：http://bhx.316326.xyz

setmetatable({}, { __index = base })
来源：http://ljc.c1oappe.top

[T41] Perl：Hello World
来源：http://vnd.nanxuanxn.top

print "Hello\n";
来源：http://aba.ywan-chungtsiang.top

[T42] Perl：变量类型
来源：http://buo.fktsv.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://gdt.sysykeji.top

[T43] Perl：字符串插值
来源：http://tac.daxiang520.top

"值: $a"
来源：http://sap.guowangkeji.top

[T44] Perl：条件
来源：http://dns.hcnkem.com

if ($a > 0) { print "正"; }
来源：http://htz.xuanzx.com

[T45] Perl：数组遍历
来源：http://kju.vehdjk.com

for my $x (@arr) { print $x; }
来源：http://icb.ydzc1.top

[T46] Perl：哈希操作
来源：http://cvd.xinyue.icu

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://zqf.yanxiufei.cn

[T47] Perl：正则捕获
来源：http://eqn.jianghu66.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://uxw.birdmap.top

[T48] Perl：正则替换
来源：http://fox.wangshuangyany.cn

$s =~ s/old/new/g;
来源：http://fvx.yj20258.top

[T49] Perl：函数
来源：http://gzc.gotoacloud.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://rex.dianchejie.cn

[T50] Perl：逐行读文件
来源：http://jet.snrcjt.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://smg.feifeiyinyue.top

while (my $line = <$fh>) { print $line; }
来源：http://sqp.hnqzz.top

[T51] Scala：Hello World
来源：http://zck.zhiwuduotai.top

println("Hello")
来源：http://pzo.andypj.xyz

[T52] Scala：变量
来源：http://zin.hysaishi.cn

val a = 1;  var b = 2
来源：http://sxo.sufxvd.cn

[T53] Scala：字符串插值
来源：http://egv.xuetiantiany.cn

s"值: $b"
来源：http://jyx.hesvh.cn

[T54] Scala：集合映射
来源：http://yww.cdnleiting.top

List(1, 2, 3).map(_ * 2)
来源：http://zio.dashuyun.cn

[T55] Scala：集合过滤
来源：http://lhg.hesvh.cn

List(1, 2, 3).filter(_ > 1)
来源：http://qtq.cashguo.top

[T56] Scala：样例类
来源：http://yct.cdnleiting.top

case class User(name: String, age: Int)
来源：http://pud.shanyushiyangtech.top

[T57] Scala：模式匹配
来源：http://veq.yonumen.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://crs.jinghuilouyu.cn

[T58] Scala：函数定义
来源：http://mhj.quarkkingdee.top

def add(a: Int, b: Int): Int = a + b
来源：http://wys.cashguo.top

[T59] Scala：循环
来源：http://eiu.zdbjq.cn

for (i <- 1 to 10) println(i)
来源：http://cvw.jinqigufen.top

[T60] Scala：折叠
来源：http://peq.hfpthk.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://yls.tanke756.top

================================================================================
来源：http://ogm.shangyingyoupin.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://nux.shangyingyoupin.top

================================================================================
来源：http://mkr.epnwcf.com

[U01] Py：创建虚拟环境
来源：http://yhi.zhiwuduotai.top

python -m venv .venv && source .venv/bin/activate
来源：http://sph.dashuyun.cn

[U02] Py：导出 / 安装依赖
来源：http://vqz.snrcjt.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://kek.bbcook.cn

[U03] Py：加载 .env 配置
来源：http://wfp.zdbjq.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://cef.hfpthk.cn

[U04] Py：变量调试打印
来源：http://dai.cashguo.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://ogk.9152youxi.cn

[U05] Py：列表去重且保序
来源：http://lfp.fanxiaobao.xyz

list(dict.fromkeys(arr))
来源：http://fgu.c1oappe.top

[U06] Py：合并两个字典
来源：http://cai.nanxuanxn.top

{**a, **b}
来源：http://qub.zhixingplan.top

[U07] Py：反转字典键值
来源：http://qcp.ydzc1.top

{v: k for k, v in d.items()}
来源：http://ise.jinghuilouyu.cn

[U08] Py：展平二维列表
来源：http://wop.sxryk.cn

[y for x in nested for y in x]
来源：http://spi.chenjidiqi.icu

[U09] Py：字典取最大值的键
来源：http://hts.ppjwa.cn

max(d, key=d.get)
来源：http://emy.ywan-chungtsiang.top

[U10] Py：按值排序字典
来源：http://ugn.ydjk.org.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://pxh.wangshuangyany.cn

[U11] Py：生成器表达式
来源：http://kkk.chenzaomai.com

(x * 2 for x in arr)
来源：http://sgi.jlsjyb.cn

[U12] Py：取出现最多的 3 个元素
来源：http://mik.bbcook.cn

Counter(arr).most_common(3)
来源：http://syy.jqgufenzy.top

[U13] Py：固定长度队列
来源：http://ybe.gotoacloud.top

deque(maxlen=10)
来源：http://fny.gzhubu.top

[U14] Py：分组收集到列表
来源：http://dsh.wangshuangyany.cn

defaultdict(list)
来源：http://stb.xuetiantiany.cn

[U15] Py：高精度计时
来源：http://rtl.zhoulong.xyz

t = time.perf_counter()
来源：http://gkx.snrcjt.cn

[U16] Py：命令行参数解析
来源：http://rzw.zhixingplan.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://zfj.quarkkingdee.top

[U17] Py：初始化日志
来源：http://uln.hysaishi.cn

logging.basicConfig(level=logging.INFO)
来源：http://lit.jqgufenzy.top

[U18] Py：预编译正则
来源：http://bcc.zhixingplan.top

pat = re.compile(r"\d+")
来源：http://dxn.yj20258888.top

[U19] Py：正则替换带回调
来源：http://bok.jqgfzy.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://xuq.yuanzhike.top

[U20] Py：缓存函数结果
来源：http://mtt.yangfankeji.com

@functools.lru_cache(maxsize=None)
来源：http://fky.zhixingplan.top

[U21] Py：自定义上下文管理器
来源：http://kgm.cdnleiting.top

@contextlib.contextmanager
来源：http://ans.bjfxy.top

[U22] Py：矩阵转置
来源：http://isb.svipenyu.cn

list(zip(*m))
来源：http://def.nanxinkj.top

[U23] Py：分块读取大文件
来源：http://gtt.feifeiyinyue.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://bou.ydzc1.top

[U24] Py：路径操作
来源：http://rft.sjlbkw.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://jwu.dianchejie.cn

[U25] Py：CSV 按字典读
来源：http://xyp.chenlongwang.top

csv.DictReader(f)
来源：http://fll.zhengqikj.top

[U26] Py：并发下载
来源：http://lrw.birdmap.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://upy.sxryk.cn

[U27] Py：异步 HTTP
来源：http://kgu.zdbjq.cn

aiohttp.ClientSession() 配合 async with
来源：http://ygq.ctjpmb.com

[U28] Py：类型别名
来源：http://rhb.fengsongda.top

UserId = int
来源：http://aij.daria6918.cn

[U29] Py：属性校验
来源：http://oou.aibaodan.cn

@property 与 @x.setter 配合
来源：http://afo.aizwys.cn

[U30] Py：数据类
来源：http://haz.cheryme.top

@dataclass(slots=True)
来源：http://bjg.quarkkingdee.top

[U31] Py：单测
来源：http://oyj.sufxvd.cn

python -m pytest -q
来源：http://tfl.xinyue.icu

[U32] Py：代码格式化
来源：http://liz.dianchejie.cn

ruff format . && ruff check --fix .
来源：http://vmr.hammf.cn

[U33] Py：打包发布
来源：http://sws.tarul.cn

python -m build  （依赖 pyproject.toml）
来源：http://uwf.yuxming.cn

[U34] Py：判断编码
来源：http://bhu.zhiwuduotai.top

chardet.detect(raw)
来源：http://ujm.xuanzx.com

[U35] Py：发送邮件
来源：http://pcj.xuetiantiany.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://rry.yuxming.cn

[U36] Py：定时任务
来源：http://cmg.zhiwuduotai.top

schedule.every(10).minutes.do(job)
来源：http://qrp.mhx1999.top

[U37] Py：读写 Excel
来源：http://iec.gogol.net.cn

pandas.read_excel / DataFrame.to_excel
来源：http://fwq.gogol.net.cn

[U38] Py：获取脚本所在目录
来源：http://pox.dashuyun.cn

Path(__file__).resolve().parent
来源：http://svt.xuanzx.com

[U39] Py：判断是否在交互环境
来源：http://vhy.birdmap.top

sys.stdout.isatty()
来源：http://qrj.yj20258888.top

[U40] Py：打印到标准错误
来源：http://zyl.yfazqb.com

print("err", file=sys.stderr)
来源：http://yxk.xingfuxueyuan.xyz

[U41] PHP：初始化 Composer 项目
来源：http://scg.hcnkem.com

composer init;  composer require guzzlehttp/guzzle
来源：http://ijs.yangfankeji.com

[U42] PHP：PSR-4 自动加载
来源：http://kxf.tarul.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://qhr.yangfankeji.com

[U43] PHP：声明命名空间
来源：http://lmw.iojbl.cn

namespace App\Http;
来源：http://ors.sxryk.cn

[U44] PHP：开启严格类型
来源：http://hkq.nwbrower.top

declare(strict_types=1);
来源：http://jfz.hongshengwenyu.top


<!-- 参考信息 -->