代发 wailian999

atoi("42");  strtod("3.14", NULL);
来源：http://kku.chenzaomai.com

[S23] C：随机数
来源：http://jph.ydzc1.top

srand(time(NULL));  int r = rand() % 100;
来源：http://mmj.hnqzz.top

[S24] C：获取本地时间
来源：http://gns.cucudq.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://pla.svipenyu.cn

[S25] C：内存拷贝
来源：http://kko.yj202588.top

memcpy(dst, src, n);
来源：http://msm.yongpay.top

[S26] C：内存清零
来源：http://dbt.52xcode.cn

memset(a, 0, sizeof a);
来源：http://diw.fzhhl.top

[S27] C：定义常量
来源：http://tdm.zdbjq.cn

const double PI = 3.14159;
来源：http://byv.52xcode.cn

[S28] C：静态变量
来源：http://qtv.yj20258.top

static int counter = 0;
来源：http://xxx.dashuyun.cn

[S29] C：变参函数
来源：http://tee.jyoumei.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://jdj.shuidangran.top

[S30] C：头文件保护
来源：http://wfl.sxryk.cn

#ifndef X_H
来源：http://zlt.nwbrower.top

#define X_H
来源：http://baw.zhiwuduotai.top

#endif
来源：http://unk.ydzc1.top

[S31] C++：Hello World
来源：http://lmh.xuetiantiany.cn

#include <iostream>
来源：http://mgl.guowangkeji.top

int main() { std::cout << "Hello\n"; }
来源：http://ced.dianchejie.cn

[S32] C++：字符串
来源：http://ntx.zdbjq.cn

std::string s = "hi";  s += "!";
来源：http://qwq.haohaochexian.top

[S33] C++：vector 增删
来源：http://hsb.shanyushiyangkeji.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://pnu.yj202588.top

[S34] C++：遍历 vector
来源：http://pch.nanxinkj.top

for (auto &x : v) { std::cout << x; }
来源：http://sah.gogol.net.cn

[S35] C++：map
来源：http://cpc.yvedp.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://bec.9152youxi.cn

[S36] C++：unordered_map
来源：http://ofm.zhaomingkeji.xyz

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://vme.jqgfzy.top

[S37] C++：set
来源：http://esz.jinqigfzy.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://dpj.ydzc1.top

[S38] C++：排序
来源：http://cjf.ybcxt.top

std::sort(v.begin(), v.end());
来源：http://lgb.zdqjudy.top

[S39] C++：自定义比较器排序
来源：http://ken.jlsjyb.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wlo.birdmap.top

[S40] C++：查找元素
来源：http://nmr.fktsv.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://vtq.jyoumei.cn

[S41] C++：类与构造函数
来源：http://xrc.guannengcc.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://ocd.yj202588.top

[S42] C++：继承与虚函数
来源：http://voq.andypj.xyz

class B : public Base { public: void f() override {} };
来源：http://trz.shangyingyoupin.top

[S43] C++：智能指针
来源：http://slv.cheryme.top

auto p = std::make_unique<int>(5);
来源：http://xys.hammf.cn

[S44] C++：引用传参
来源：http://khy.shanyushiyangtech.top

void inc(int &x) { ++x; }
来源：http://xjv.tarul.cn

[S45] C++：lambda
来源：http://tsr.316326.xyz

auto add = [](int a, int b) { return a + b; };
来源：http://obo.zdbjq.cn

[S46] C++：函数模板
来源：http://ver.fanxiaobao.xyz

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://ytv.smart0.xyz

[S47] C++：结构化绑定遍历
来源：http://hfm.shzxlz.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://huj.zdbjq.cn

[S48] C++：逐行读文件
来源：http://ijx.fzhhl.top

std::ifstream in("a.txt");  std::string line;
来源：http://wef.chenjidiqi.icu

while (std::getline(in, line)) { }
来源：http://cwy.fanxiaobao.xyz

[S49] C++：写文件
来源：http://msz.gaohongyu789.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://kzx.jlsjyb.cn

[S50] C++：格式化数字
来源：http://jhc.yueranfly.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://kfr.havefunace.top

[S51] C++：显式类型转换
来源：http://xmv.hnxiangtu.top

static_cast<double>(a) / b
来源：http://ini.mhx1999.top

[S52] C++：const 与 noexcept
来源：http://ckk.jinqigufen.top

int size() const noexcept { return n_; }
来源：http://bjr.tarul.cn

[S53] C++：移动语义
来源：http://gal.jlsjyb.cn

std::vector<int> w = std::move(v);
来源：http://uhk.vehdjk.com

[S54] C++：异常处理
来源：http://ulb.ywan-chungtsiang.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://fny.jinqigfzy.top

[S55] C++：结构化绑定
来源：http://rgs.hnqzz.top

auto [a, b] = std::make_pair(1, 2);
来源：http://hwq.wangdashe.top

[S56] C++：optional
来源：http://whh.yanxiufei.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://esx.yuxming.cn

[S57] C++：编译期常量
来源：http://ays.dianchejie.cn

constexpr int N = 10;
来源：http://urf.yanxiufei.cn

[S58] C++：命名空间
来源：http://inj.zhongyouzk.top

namespace ns { int f() { return 1; } }
来源：http://lnw.c1oappe.top

[S59] C++：静态断言
来源：http://fzu.yonumen.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://rpn.yuxming.cn

[S60] C++：遍历并删除元素
来源：http://lgc.pengpengdd.cyou

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://qwe.jqgfzy.top

================================================================================
来源：http://fkq.hnqzz.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://kzf.guowangkeji.top

================================================================================
来源：http://mak.nanxinkj.top

[T01] Kotlin：Hello World
来源：http://avf.gzhubu.top

println("Hello")
来源：http://gwu.smart0.xyz

[T02] Kotlin：变量
来源：http://zgi.hnxiangtu.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://lpq.tianlin.xyz

[T03] Kotlin：字符串模板
来源：http://ufl.hywenlv.cn

"值: $b"
来源：http://kfh.tian-w.cn

[T04] Kotlin：空安全
来源：http://fne.tarul.cn

val n: String? = null;  n?.length
来源：http://vwk.gotoacloud.top

[T05] Kotlin：when 表达式
来源：http://jcq.zhengqikj.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://acd.shzxlz.cn

[T06] Kotlin：集合映射
来源：http://dmb.tarul.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://tlb.shzxlz.cn

[T07] Kotlin：集合过滤
来源：http://ofy.svipenyu.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://scj.yongpay.top

[T08] Kotlin：数据类
来源：http://wjf.xziqi.cn

data class User(val name: String, val age: Int)
来源：http://xhg.snrcjt.cn

[T09] Kotlin：扩展函数
来源：http://fal.wangdashe.top

fun String.exclaim() = this + "!"
来源：http://rsb.chenjidiqi.icu

[T10] Kotlin：默认参数
来源：http://skx.iojbl.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://npi.gzhubu.top

[T11] Kotlin：协程
来源：http://gvb.ppjwa.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://tnf.jinqigfzy.top

[T12] Kotlin：解构声明
来源：http://rxw.yangfankeji.com

val (a, b) = Pair(1, 2)
来源：http://yzv.zhiwuduotai.top

[T13] Kotlin：只读 Map
来源：http://cwy.gogol.net.cn

val m = mapOf("a" to 1)
来源：http://cdq.hfpthk.cn

[T14] Kotlin：循环
来源：http://yng.yj202588.top

for (i in 1..10) println(i)
来源：http://rvy.aibaodan.cn

[T15] Kotlin：接口
来源：http://bqz.yj202588.top

interface Shape { fun area(): Double }
来源：http://uou.yuanzhike.top

[T16] Swift：Hello World
来源：http://ori.snrcjt.cn

print("Hello")
来源：http://kaz.ppjwa.cn

[T17] Swift：变量与常量
来源：http://asl.316326.xyz

var a = 1;  let b = 2
来源：http://lly.dianchejie.cn

[T18] Swift：字符串插值
来源：http://hsj.tianlin.xyz

"值: \(b)"
来源：http://lst.bjfxy.top

[T19] Swift：可选绑定
来源：http://kny.shanyushiyangtech.top

if let n = opt { print(n) }
来源：http://wkm.zhoulong.xyz

[T20] Swift：数组操作
来源：http://jxf.yvedp.cn

var a = [1, 2, 3];  a.append(4)
来源：http://ncl.yuxming.cn

[T21] Swift：遍历
来源：http://dcm.svipenyu.cn

for x in a { print(x) }
来源：http://iaq.pycfn.com

[T22] Swift：字典
来源：http://ttk.bjfxy.top

var d = ["a": 1];  d["b"] = 2
来源：http://tji.zycfv.cn

[T23] Swift：函数
来源：http://sua.ivvv.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://nvg.guannengcc.top

[T24] Swift：闭包
来源：http://jsu.cdnleiting.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://dgo.epnwcf.com

[T25] Swift：结构体
来源：http://hsd.ywan-chungtsiang.top

struct P { var x: Int }
来源：http://mkp.hcnkem.com

[T26] Swift：类与重写
来源：http://zke.meibo888.top

class A: Base { override func f() {} }
来源：http://ily.ppjwa.cn

[T27] Swift：错误处理
来源：http://seq.yuxming.cn

do { try f() } catch { print(error) }
来源：http://str.xylfe.cn

[T28] Swift：枚举
来源：http://ubm.xuanzx.com

enum Color { case red, green }
来源：http://klm.ppjwa.cn

[T29] Swift：guard 提前返回
来源：http://pbu.yongpay.top

guard let x = opt else { return }
来源：http://dzs.dianchejie.cn

[T30] Swift：协议
来源：http://jnl.svipenyu.cn

protocol Shape { func area() -> Double }
来源：http://rsd.zhengqikj.top

[T31] Lua：Hello World
来源：http://uuu.aizwys.cn

print("Hello")
来源：http://vnx.zhixingplan.top

[T32] Lua：局部变量
来源：http://ioc.shangyingyoupin.top

local a = 1
来源：http://agz.cashguo.top

[T33] Lua：表（数组）
来源：http://pgx.svipenyu.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://mix.vehdjk.com

[T34] Lua：遍历表
来源：http://kpc.xylfe.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://suk.zdqjudy.top

[T35] Lua：字典表
来源：http://tzy.ppjwa.cn

local d = { a = 1 };  d.b = 2
来源：http://hqy.jinghuilouyu.cn

[T36] Lua：函数
来源：http://qyf.zhijiandao.cn

function add(a, b) return a + b end
来源：http://xbv.sysykeji.top

[T37] Lua：字符串拼接
来源：http://uft.dianchejie.cn

"a" .. "b"
来源：http://qrh.yuxming.cn

[T38] Lua：条件
来源：http://nmu.zhoulong.xyz

if x > 0 then print("正") end
来源：http://boa.sysykeji.top

[T39] Lua：模式匹配
来源：http://rkk.jyoumei.cn

string.find(s, "%d+")
来源：http://ard.zdbjq.cn

[T40] Lua：元表
来源：http://myn.fanxiaobao.xyz

setmetatable({}, { __index = base })
来源：http://gxi.chenlongwang.top

[T41] Perl：Hello World
来源：http://jqm.jinqigfzy.top

print "Hello\n";
来源：http://chx.gzhubu.top

[T42] Perl：变量类型
来源：http://avs.fengsongda.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://cuh.iojbl.cn

[T43] Perl：字符串插值
来源：http://gds.jinqigfzy.top

"值: $a"
来源：http://fpr.9152youxi.cn

[T44] Perl：条件
来源：http://dxk.pycfn.com

if ($a > 0) { print "正"; }
来源：http://gsb.daxiang520.top

[T45] Perl：数组遍历
来源：http://kyb.pengpengdd.cyou

for my $x (@arr) { print $x; }
来源：http://oua.ctjpmb.com

[T46] Perl：哈希操作
来源：http://snf.ctjpmb.com

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://nvo.smart0.xyz

[T47] Perl：正则捕获
来源：http://rrh.ydzc1.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://pth.ywan-chungtsiang.top

[T48] Perl：正则替换
来源：http://gjr.zhijiandao.cn

$s =~ s/old/new/g;
来源：http://gfx.sjlbkw.cn

[T49] Perl：函数
来源：http://vsa.nanxinkj.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://eyo.yonumen.top

[T50] Perl：逐行读文件
来源：http://bly.zdbjq.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://tlk.shanyushiyangkeji.top

while (my $line = <$fh>) { print $line; }
来源：http://ogv.cheryme.top

[T51] Scala：Hello World
来源：http://hpg.daria6918.cn

println("Hello")
来源：http://aoe.jqgfzy.top

[T52] Scala：变量
来源：http://nuo.zycfv.cn

val a = 1;  var b = 2
来源：http://srb.quarkkingdee.top

[T53] Scala：字符串插值
来源：http://lfr.vqdsnc.cn

s"值: $b"
来源：http://xex.hywenlv.cn

[T54] Scala：集合映射
来源：http://gom.guowangkeji.top

List(1, 2, 3).map(_ * 2)
来源：http://hiw.chenzaomai.com

[T55] Scala：集合过滤
来源：http://dkf.cheryme.top

List(1, 2, 3).filter(_ > 1)
来源：http://ybu.zhixingplan.top

[T56] Scala：样例类
来源：http://enq.hysaishi.cn

case class User(name: String, age: Int)
来源：http://muv.cheryme.top

[T57] Scala：模式匹配
来源：http://rld.jlsjyb.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://cgq.aizwys.cn

[T58] Scala：函数定义
来源：http://uhq.shanyushiyangkeji.top

def add(a: Int, b: Int): Int = a + b
来源：http://uox.yongpay.top

[T59] Scala：循环
来源：http://wbk.snrcjt.cn

for (i <- 1 to 10) println(i)
来源：http://mxe.yuanzhike.top

[T60] Scala：折叠
来源：http://qli.fengsongda.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://ryh.fengsongda.top

================================================================================
来源：http://til.zhengqikj.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://xnc.cucudq.cn

================================================================================
来源：http://czm.bbcook.cn

[U01] Py：创建虚拟环境
来源：http://jfa.xuetiantiany.cn

python -m venv .venv && source .venv/bin/activate
来源：http://wgp.bbcook.cn

[U02] Py：导出 / 安装依赖
来源：http://usn.tanke756.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://qsr.cdnleiting.top

[U03] Py：加载 .env 配置
来源：http://lpi.jinyuanbaomall.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://ryh.ehwqpu.com

[U04] Py：变量调试打印
来源：http://wlv.hfpthk.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://cdm.cheryme.top

[U05] Py：列表去重且保序
来源：http://coe.gogol.net.cn

list(dict.fromkeys(arr))
来源：http://szg.yuxming.cn

[U06] Py：合并两个字典
来源：http://pfp.zdqjudy.top

{**a, **b}
来源：http://old.gotoacloud.top

[U07] Py：反转字典键值
来源：http://sdd.xziqi.cn

{v: k for k, v in d.items()}
来源：http://srx.bbcook.cn

[U08] Py：展平二维列表
来源：http://jve.fktsv.cn

[y for x in nested for y in x]
来源：http://xxt.zhaomingkeji.xyz

[U09] Py：字典取最大值的键
来源：http://xei.daxiang520.top

max(d, key=d.get)
来源：http://qda.gotoacloud.top

[U10] Py：按值排序字典
来源：http://icy.meibo888.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://xwl.svipenyu.cn

[U11] Py：生成器表达式
来源：http://vus.vqdsnc.cn

(x * 2 for x in arr)
来源：http://niw.yuanzhike.top

[U12] Py：取出现最多的 3 个元素
来源：http://rus.daxiang520.top

Counter(arr).most_common(3)
来源：http://kpa.hnxiangtu.top

[U13] Py：固定长度队列
来源：http://jsv.xingfuxueyuan.xyz

deque(maxlen=10)
来源：http://nrs.ywan-chungtsiang.top

[U14] Py：分组收集到列表
来源：http://fyf.ivvv.top

defaultdict(list)
来源：http://aul.tanke756.top

[U15] Py：高精度计时
来源：http://tmp.yonumen.top

t = time.perf_counter()
来源：http://dkp.yuanzhike.top

[U16] Py：命令行参数解析
来源：http://iur.fktsv.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://myd.andypj.xyz

[U17] Py：初始化日志
来源：http://kpp.yuxming.cn

logging.basicConfig(level=logging.INFO)
来源：http://fta.andypj.xyz

[U18] Py：预编译正则
来源：http://rbb.jinqigfzy.top

pat = re.compile(r"\d+")
来源：http://btg.chenjidiqi.icu

[U19] Py：正则替换带回调
来源：http://vum.meibo888.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://ipk.9152youxi.cn

[U20] Py：缓存函数结果
来源：http://ufj.sufxvd.cn

@functools.lru_cache(maxsize=None)
来源：http://kfu.tanke756.top

[U21] Py：自定义上下文管理器
来源：http://ked.zdqjudy.top

@contextlib.contextmanager
来源：http://tgk.yj202588.top

[U22] Py：矩阵转置
来源：http://tre.yangfankeji.com

list(zip(*m))
来源：http://dvp.shzxlz.cn

[U23] Py：分块读取大文件
来源：http://pil.bbcook.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://ill.zhaomingkeji.xyz

[U24] Py：路径操作
来源：http://qak.dianchejie.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://umw.yvedp.cn

[U25] Py：CSV 按字典读
来源：http://hcp.jianghu66.top

csv.DictReader(f)
来源：http://qyr.iojbl.cn

[U26] Py：并发下载
来源：http://gui.gogol.net.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://ymp.yvedp.cn

[U27] Py：异步 HTTP
来源：http://rlh.pycfn.com

aiohttp.ClientSession() 配合 async with
来源：http://bys.andypj.xyz

[U28] Py：类型别名
来源：http://lra.ppjwa.cn

UserId = int
来源：http://fqb.gaohongyu789.top

[U29] Py：属性校验
来源：http://dvu.ivvv.top

@property 与 @x.setter 配合
来源：http://loe.tanke756.top

[U30] Py：数据类
来源：http://wvk.hfpthk.cn

@dataclass(slots=True)
来源：http://zci.wangshuangyany.cn

[U31] Py：单测
来源：http://vci.tarul.cn

python -m pytest -q
来源：http://hgp.guowangkeji.top

[U32] Py：代码格式化
来源：http://aou.guannengcc.top

ruff format . && ruff check --fix .
来源：http://ynu.andypj.xyz

[U33] Py：打包发布
来源：http://vfn.quarkkingdee.top

python -m build  （依赖 pyproject.toml）
来源：http://rdv.andypj.xyz

[U34] Py：判断编码
来源：http://cia.bjfxy.top

chardet.detect(raw)
来源：http://sdj.vehdjk.com

[U35] Py：发送邮件
来源：http://thq.bjfxy.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://smd.tanke756.top

[U36] Py：定时任务
来源：http://pmh.ydjk.org.cn

schedule.every(10).minutes.do(job)
来源：http://wdo.cashguo.top

[U37] Py：读写 Excel
来源：http://zgg.dianchejie.cn

pandas.read_excel / DataFrame.to_excel
来源：http://cby.fanxiaobao.xyz

[U38] Py：获取脚本所在目录
来源：http://lzn.gaohongyu789.top

Path(__file__).resolve().parent
来源：http://ebq.hysaishi.cn

[U39] Py：判断是否在交互环境
来源：http://hyd.xylfe.cn

sys.stdout.isatty()
来源：http://ctp.jinqigufen.top

[U40] Py：打印到标准错误
来源：http://hnz.yvedp.cn

print("err", file=sys.stderr)
来源：http://uwd.ehwqpu.com

[U41] PHP：初始化 Composer 项目
来源：http://klz.gogol.net.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://duq.guowangkeji.top

[U42] PHP：PSR-4 自动加载
来源：http://spc.yvedp.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://sff.chenlongwang.top

[U43] PHP：声明命名空间
来源：http://krv.zhixingplan.top

namespace App\Http;
来源：http://raf.tian-w.cn

[U44] PHP：开启严格类型
来源：http://mbc.snrcjt.cn

declare(strict_types=1);
来源：http://fec.cucudq.cn

[U45] PHP：类型声明与返回类型
来源：http://hpm.jyoumei.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://qvo.ivvv.top

[U46] PHP：可空类型
来源：http://ebd.andypj.xyz

?string $name = null
来源：http://wvw.uphjek.com


<!-- 参考信息 -->