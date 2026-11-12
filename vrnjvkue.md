代发 wailian999

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://euk.yongpay.top

[S25] C：内存拷贝
来源：http://jrx.jianghu66.top

memcpy(dst, src, n);
来源：http://wkk.ywan-chungtsiang.top

[S26] C：内存清零
来源：http://kze.fehbvm.com

memset(a, 0, sizeof a);
来源：http://toh.xingfuxueyuan.xyz

[S27] C：定义常量
来源：http://zyg.zhijiandao.cn

const double PI = 3.14159;
来源：http://sng.fktsv.cn

[S28] C：静态变量
来源：http://cjr.gzhubu.top

static int counter = 0;
来源：http://amf.hywenlv.cn

[S29] C：变参函数
来源：http://eig.tianlin.xyz

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://nqq.gotoacloud.top

[S30] C：头文件保护
来源：http://hun.zdbjq.cn

#ifndef X_H
来源：http://nco.yuxming.cn

#define X_H
来源：http://hxq.ydzc1.top

#endif
来源：http://yng.hysaishi.cn

[S31] C++：Hello World
来源：http://gpn.vehdjk.com

#include <iostream>
来源：http://dka.yj20258888.top

int main() { std::cout << "Hello\n"; }
来源：http://wsm.bbcook.cn

[S32] C++：字符串
来源：http://nbt.bjfxy.top

std::string s = "hi";  s += "!";
来源：http://zku.quarkkingdee.top

[S33] C++：vector 增删
来源：http://oki.zdqjudy.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://nlk.ybcxt.top

[S34] C++：遍历 vector
来源：http://tvh.aizwys.cn

for (auto &x : v) { std::cout << x; }
来源：http://rww.aizwys.cn

[S35] C++：map
来源：http://cxn.aibaodan.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://ozg.xuanzx.com

[S36] C++：unordered_map
来源：http://mdp.dianchejie.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://leu.hongshengwenyu.top

[S37] C++：set
来源：http://fpg.guannengcc.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://bor.9152youxi.cn

[S38] C++：排序
来源：http://mmz.gogol.net.cn

std::sort(v.begin(), v.end());
来源：http://xun.sjlbkw.cn

[S39] C++：自定义比较器排序
来源：http://toq.cdnleiting.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://pqt.jinyuanbaomall.cn

[S40] C++：查找元素
来源：http://wuo.jinghuilouyu.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://llu.chenlongwang.top

[S41] C++：类与构造函数
来源：http://cau.tian-w.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://uvu.havefunace.top

[S42] C++：继承与虚函数
来源：http://uuu.uphjek.com

class B : public Base { public: void f() override {} };
来源：http://ary.jianghu66.top

[S43] C++：智能指针
来源：http://qnv.gaohongyu789.top

auto p = std::make_unique<int>(5);
来源：http://kyk.zycfv.cn

[S44] C++：引用传参
来源：http://quo.ywan-chungtsiang.top

void inc(int &x) { ++x; }
来源：http://yvt.jinqigufen.top

[S45] C++：lambda
来源：http://sor.shangyingyoupin.top

auto add = [](int a, int b) { return a + b; };
来源：http://qcv.dianchejie.cn

[S46] C++：函数模板
来源：http://jjc.ehwqpu.com

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://fce.yangfankeji.com

[S47] C++：结构化绑定遍历
来源：http://abq.nwbrower.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://ily.mhx1999.top

[S48] C++：逐行读文件
来源：http://bqr.pycfn.com

std::ifstream in("a.txt");  std::string line;
来源：http://qpg.jqgfzy.top

while (std::getline(in, line)) { }
来源：http://rtn.sjlbkw.cn

[S49] C++：写文件
来源：http://uoa.gogol.net.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://qdd.gogol.net.cn

[S50] C++：格式化数字
来源：http://ecb.dianchejie.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://zqt.zycfv.cn

[S51] C++：显式类型转换
来源：http://msi.52xcode.cn

static_cast<double>(a) / b
来源：http://tkc.yanxiufei.cn

[S52] C++：const 与 noexcept
来源：http://vkx.ehwqpu.com

int size() const noexcept { return n_; }
来源：http://thh.yvedp.cn

[S53] C++：移动语义
来源：http://qhg.smart0.xyz

std::vector<int> w = std::move(v);
来源：http://xps.snrcjt.cn

[S54] C++：异常处理
来源：http://aux.hysaishi.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://llq.shangyingyoupin.top

[S55] C++：结构化绑定
来源：http://zac.meibo888.top

auto [a, b] = std::make_pair(1, 2);
来源：http://vtm.yj20258.top

[S56] C++：optional
来源：http://dtw.snrcjt.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://vpy.nanxuanxn.top

[S57] C++：编译期常量
来源：http://sfw.sjlbkw.cn

constexpr int N = 10;
来源：http://bff.daxiang520.top

[S58] C++：命名空间
来源：http://etg.xuanzx.com

namespace ns { int f() { return 1; } }
来源：http://dtv.hcnkem.com

[S59] C++：静态断言
来源：http://ekc.bbcook.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://ecy.fktsv.cn

[S60] C++：遍历并删除元素
来源：http://kin.jinyuanbaomall.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://boc.chenjidiqi.icu

================================================================================
来源：http://bpr.shanyushiyangtech.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://xww.yfazqb.com

================================================================================
来源：http://xca.sysykeji.top

[T01] Kotlin：Hello World
来源：http://bee.sweek.top

println("Hello")
来源：http://gph.shangyingyoupin.top

[T02] Kotlin：变量
来源：http://uuw.chenjidiqi.icu

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://cei.mhx1999.top

[T03] Kotlin：字符串模板
来源：http://zyy.nanxinkj.top

"值: $b"
来源：http://xho.52xcode.cn

[T04] Kotlin：空安全
来源：http://een.yonumen.top

val n: String? = null;  n?.length
来源：http://hbx.xuanzx.com

[T05] Kotlin：when 表达式
来源：http://pnl.xuanzx.com

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://tri.hammf.cn

[T06] Kotlin：集合映射
来源：http://hzm.jlsjyb.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://kfd.9152youxi.cn

[T07] Kotlin：集合过滤
来源：http://ixe.jlsjyb.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://kar.yvedp.cn

[T08] Kotlin：数据类
来源：http://ctr.dashuyun.cn

data class User(val name: String, val age: Int)
来源：http://dpg.tanke756.top

[T09] Kotlin：扩展函数
来源：http://rmg.mhx1999.top

fun String.exclaim() = this + "!"
来源：http://mpj.kuanghao11.cn

[T10] Kotlin：默认参数
来源：http://icy.yueranfly.top

fun greet(name: String = "World") = "Hi $name"
来源：http://odt.tianlin.xyz

[T11] Kotlin：协程
来源：http://mho.daria6918.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://hlg.zhengqikj.top

[T12] Kotlin：解构声明
来源：http://hyh.xingfuxueyuan.xyz

val (a, b) = Pair(1, 2)
来源：http://glu.c1oappe.top

[T13] Kotlin：只读 Map
来源：http://cdu.meibo888.top

val m = mapOf("a" to 1)
来源：http://qxw.yuxming.cn

[T14] Kotlin：循环
来源：http://pqk.xinyue.icu

for (i in 1..10) println(i)
来源：http://mqz.kuanghao11.cn

[T15] Kotlin：接口
来源：http://iow.jianghu66.top

interface Shape { fun area(): Double }
来源：http://ywa.sweek.top

[T16] Swift：Hello World
来源：http://fxr.jlsjyb.cn

print("Hello")
来源：http://qtv.hysaishi.cn

[T17] Swift：变量与常量
来源：http://dqr.cashguo.top

var a = 1;  let b = 2
来源：http://lny.hcnkem.com

[T18] Swift：字符串插值
来源：http://wtb.xziqi.cn

"值: \(b)"
来源：http://rij.svipenyu.cn

[T19] Swift：可选绑定
来源：http://rhp.vqdsnc.cn

if let n = opt { print(n) }
来源：http://cfq.jqgfzy.top

[T20] Swift：数组操作
来源：http://nvq.fktsv.cn

var a = [1, 2, 3];  a.append(4)
来源：http://atd.tianlin.xyz

[T21] Swift：遍历
来源：http://fdk.gogol.net.cn

for x in a { print(x) }
来源：http://llu.quarkkingdee.top

[T22] Swift：字典
来源：http://ron.feifeiyinyue.top

var d = ["a": 1];  d["b"] = 2
来源：http://gfy.havefunace.top

[T23] Swift：函数
来源：http://jmf.hfpthk.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://cnr.nanxinkj.top

[T24] Swift：闭包
来源：http://vcy.yvedp.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://yus.cashguo.top

[T25] Swift：结构体
来源：http://xye.cheryme.top

struct P { var x: Int }
来源：http://ihs.yuanzhike.top

[T26] Swift：类与重写
来源：http://osx.yj202588.top

class A: Base { override func f() {} }
来源：http://dwu.0kj1m.cn

[T27] Swift：错误处理
来源：http://iau.zhongyouzk.top

do { try f() } catch { print(error) }
来源：http://ryz.tarul.cn

[T28] Swift：枚举
来源：http://ljt.shangyingyoupin.top

enum Color { case red, green }
来源：http://fwh.shangyingyoupin.top

[T29] Swift：guard 提前返回
来源：http://wdd.svipenyu.cn

guard let x = opt else { return }
来源：http://lci.quarkkingdee.top

[T30] Swift：协议
来源：http://koo.yfazqb.com

protocol Shape { func area() -> Double }
来源：http://yjx.jlsjyb.cn

[T31] Lua：Hello World
来源：http://yaw.jyoumei.cn

print("Hello")
来源：http://goz.dashuyun.cn

[T32] Lua：局部变量
来源：http://nre.epnwcf.com

local a = 1
来源：http://geg.fktsv.cn

[T33] Lua：表（数组）
来源：http://uxs.jinqigfzy.top

local t = {1, 2, 3};  t[4] = 4
来源：http://igf.yj20258888.top

[T34] Lua：遍历表
来源：http://doh.xingfuxueyuan.xyz

for i, v in ipairs(t) do print(i, v) end
来源：http://hud.daxiang520.top

[T35] Lua：字典表
来源：http://wmo.hammf.cn

local d = { a = 1 };  d.b = 2
来源：http://hkv.zdqjudy.top

[T36] Lua：函数
来源：http://emi.jinqigfzy.top

function add(a, b) return a + b end
来源：http://fzu.fktsv.cn

[T37] Lua：字符串拼接
来源：http://bfk.jqgufenzy.top

"a" .. "b"
来源：http://seh.ybcxt.top

[T38] Lua：条件
来源：http://azc.xylfe.cn

if x > 0 then print("正") end
来源：http://ssr.xziqi.cn

[T39] Lua：模式匹配
来源：http://eie.sxryk.cn

string.find(s, "%d+")
来源：http://jne.yvedp.cn

[T40] Lua：元表
来源：http://cvs.zycfv.cn

setmetatable({}, { __index = base })
来源：http://bul.andypj.xyz

[T41] Perl：Hello World
来源：http://prr.haohaochexian.top

print "Hello\n";
来源：http://zku.jqgfzy.top

[T42] Perl：变量类型
来源：http://bbw.daxiang520.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://tuo.xuetiantiany.cn

[T43] Perl：字符串插值
来源：http://kjs.redwolf501.top

"值: $a"
来源：http://bdi.316326.xyz

[T44] Perl：条件
来源：http://xso.zdbjq.cn

if ($a > 0) { print "正"; }
来源：http://qiv.sysykeji.top

[T45] Perl：数组遍历
来源：http://lnt.fehbvm.com

for my $x (@arr) { print $x; }
来源：http://ywm.vehdjk.com

[T46] Perl：哈希操作
来源：http://thu.xingfuxueyuan.xyz

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://ttg.sxryk.cn

[T47] Perl：正则捕获
来源：http://udn.jinyuanbaomall.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://xil.c1oappe.top

[T48] Perl：正则替换
来源：http://jwl.aizwys.cn

$s =~ s/old/new/g;
来源：http://mjy.jinqigufen.top

[T49] Perl：函数
来源：http://vah.gzhubu.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://seg.ctjpmb.com

[T50] Perl：逐行读文件
来源：http://blc.ybcxt.top

open my $fh, "<", "a.txt" or die $!;
来源：http://yzu.dashuyun.cn

while (my $line = <$fh>) { print $line; }
来源：http://vie.wangdashe.top

[T51] Scala：Hello World
来源：http://wpn.zdbjq.cn

println("Hello")
来源：http://nbs.sxryk.cn

[T52] Scala：变量
来源：http://ozt.ppjwa.cn

val a = 1;  var b = 2
来源：http://xpu.feifeiyinyue.top

[T53] Scala：字符串插值
来源：http://ckf.chenjidiqi.icu

s"值: $b"
来源：http://vrx.fzhhl.top

[T54] Scala：集合映射
来源：http://iss.meibo888.top

List(1, 2, 3).map(_ * 2)
来源：http://xpz.epnwcf.com

[T55] Scala：集合过滤
来源：http://szj.jqgfzy.top

List(1, 2, 3).filter(_ > 1)
来源：http://cql.tarul.cn

[T56] Scala：样例类
来源：http://ncb.hywenlv.cn

case class User(name: String, age: Int)
来源：http://vmy.shanyushiyangtech.top

[T57] Scala：模式匹配
来源：http://tpl.cashguo.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://cek.quarkkingdee.top

[T58] Scala：函数定义
来源：http://wbk.birdmap.top

def add(a: Int, b: Int): Int = a + b
来源：http://csn.fehbvm.com

[T59] Scala：循环
来源：http://azy.yanxiufei.cn

for (i <- 1 to 10) println(i)
来源：http://vgs.xingfuxueyuan.xyz

[T60] Scala：折叠
来源：http://tac.zhongyouzk.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://spy.daria6918.cn

================================================================================
来源：http://yoi.dianchejie.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hzp.bbcook.cn

================================================================================
来源：http://ezh.hywenlv.cn

[U01] Py：创建虚拟环境
来源：http://gwj.daxiang520.top

python -m venv .venv && source .venv/bin/activate
来源：http://iwh.guannengcc.top

[U02] Py：导出 / 安装依赖
来源：http://jgi.tianlin.xyz

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://quw.yvedp.cn

[U03] Py：加载 .env 配置
来源：http://xsv.guannengcc.top

from dotenv import load_dotenv; load_dotenv()
来源：http://qhw.hywenlv.cn

[U04] Py：变量调试打印
来源：http://ltg.jinqigfzy.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://mko.xuanzx.com

[U05] Py：列表去重且保序
来源：http://gxh.andypj.xyz

list(dict.fromkeys(arr))
来源：http://rgd.cqqwz.cn

[U06] Py：合并两个字典
来源：http://inp.zhijiandao.cn

{**a, **b}
来源：http://vhv.hnqzz.top

[U07] Py：反转字典键值
来源：http://cbe.kuanghao11.cn

{v: k for k, v in d.items()}
来源：http://tdx.yuxming.cn

[U08] Py：展平二维列表
来源：http://qli.zhixingplan.top

[y for x in nested for y in x]
来源：http://baw.quarkkingdee.top

[U09] Py：字典取最大值的键
来源：http://rjw.chenzaomai.com

max(d, key=d.get)
来源：http://rmx.316326.xyz

[U10] Py：按值排序字典
来源：http://gzv.jlsjyb.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://muc.kuanghao11.cn

[U11] Py：生成器表达式
来源：http://jxj.316326.xyz

(x * 2 for x in arr)
来源：http://gai.daxiang520.top

[U12] Py：取出现最多的 3 个元素
来源：http://kjj.c1oappe.top

Counter(arr).most_common(3)
来源：http://tlo.jianghu66.top

[U13] Py：固定长度队列
来源：http://xas.zdbjq.cn

deque(maxlen=10)
来源：http://mqo.pengpengdd.cyou

[U14] Py：分组收集到列表
来源：http://suu.jqgufenzy.top

defaultdict(list)
来源：http://ouz.xylfe.cn

[U15] Py：高精度计时
来源：http://aiu.vqdsnc.cn

t = time.perf_counter()
来源：http://yap.jinqigufen.top

[U16] Py：命令行参数解析
来源：http://zpv.birdmap.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://gzb.yanxiufei.cn

[U17] Py：初始化日志
来源：http://ipc.nanxuanxn.top

logging.basicConfig(level=logging.INFO)
来源：http://svh.jqgufenzy.top

[U18] Py：预编译正则
来源：http://kgn.yonumen.top

pat = re.compile(r"\d+")
来源：http://xtj.xziqi.cn

[U19] Py：正则替换带回调
来源：http://bcb.wangdashe.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://fce.zhijiandao.cn

[U20] Py：缓存函数结果
来源：http://qhn.hfpthk.cn

@functools.lru_cache(maxsize=None)
来源：http://ugn.hysaishi.cn

[U21] Py：自定义上下文管理器
来源：http://txn.sufxvd.cn

@contextlib.contextmanager
来源：http://aqu.mhx1999.top

[U22] Py：矩阵转置
来源：http://znj.ctjpmb.com

list(zip(*m))
来源：http://thu.hesvh.cn

[U23] Py：分块读取大文件
来源：http://ggz.svipenyu.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://thd.cqqwz.cn

[U24] Py：路径操作
来源：http://gfq.guowangkeji.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://xjl.vqdsnc.cn

[U25] Py：CSV 按字典读
来源：http://dkv.aibaodan.cn

csv.DictReader(f)
来源：http://lvt.xuetiantiany.cn

[U26] Py：并发下载
来源：http://ejd.nwbrower.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://yiw.iojbl.cn

[U27] Py：异步 HTTP
来源：http://rbp.havefunace.top

aiohttp.ClientSession() 配合 async with
来源：http://xyg.shuidangran.top

[U28] Py：类型别名
来源：http://azp.hammf.cn

UserId = int
来源：http://miz.yvedp.cn

[U29] Py：属性校验
来源：http://lpc.52xcode.cn

@property 与 @x.setter 配合
来源：http://gpa.ppjwa.cn

[U30] Py：数据类
来源：http://dto.c1oappe.top

@dataclass(slots=True)
来源：http://zyq.9152youxi.cn

[U31] Py：单测
来源：http://rmk.zhiwuduotai.top

python -m pytest -q
来源：http://lwv.hesvh.cn

[U32] Py：代码格式化
来源：http://ims.zhiwuduotai.top

ruff format . && ruff check --fix .
来源：http://uuc.dianchejie.cn

[U33] Py：打包发布
来源：http://xwq.shanyushiyangkeji.top

python -m build  （依赖 pyproject.toml）
来源：http://seu.chenzaomai.com

[U34] Py：判断编码
来源：http://knp.cqqwz.cn

chardet.detect(raw)
来源：http://hoc.sjlbkw.cn

[U35] Py：发送邮件
来源：http://coi.nanxuanxn.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://dbv.zhiwuduotai.top

[U36] Py：定时任务
来源：http://sdt.jqgfzy.top

schedule.every(10).minutes.do(job)
来源：http://jcw.zhijiandao.cn

[U37] Py：读写 Excel
来源：http://ash.jinqigfzy.top

pandas.read_excel / DataFrame.to_excel
来源：http://mmd.fengsongda.top

[U38] Py：获取脚本所在目录
来源：http://qxf.jlsjyb.cn

Path(__file__).resolve().parent
来源：http://daf.daria6918.cn

[U39] Py：判断是否在交互环境
来源：http://thz.kuanghao11.cn

sys.stdout.isatty()
来源：http://aed.cucudq.cn

[U40] Py：打印到标准错误
来源：http://geg.gogol.net.cn

print("err", file=sys.stderr)
来源：http://vmx.birdmap.top

[U41] PHP：初始化 Composer 项目
来源：http://pmb.jqgufenzy.top

composer init;  composer require guzzlehttp/guzzle
来源：http://sih.meibo888.top

[U42] PHP：PSR-4 自动加载
来源：http://omt.wangshuangyany.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://qlq.birdmap.top

[U43] PHP：声明命名空间
来源：http://ifx.jinqigufen.top

namespace App\Http;
来源：http://mju.tianlin.xyz

[U44] PHP：开启严格类型
来源：http://hpd.pycfn.com

declare(strict_types=1);
来源：http://zvu.yanxiufei.cn

[U45] PHP：类型声明与返回类型
来源：http://rcq.fengsongda.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://jhj.yuxming.cn

[U46] PHP：可空类型
来源：http://sye.zhoulong.xyz

?string $name = null
来源：http://mhj.svipenyu.cn

[U47] PHP：联合类型
来源：http://flv.nwbrower.top

int|string $id
来源：http://yit.ehwqpu.com

[U48] PHP：纯枚举
来源：http://hbh.ehwqpu.com

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://oas.yongpay.top


<!-- 参考信息 -->