代发 wailian999

static int counter = 0;
来源：http://ktq.tanke756.top

[S29] C：变参函数
来源：http://vto.gaohongyu789.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://tbo.ywan-chungtsiang.top

[S30] C：头文件保护
来源：http://vsg.ctjpmb.com

#ifndef X_H
来源：http://mvl.shanyushiyangtech.top

#define X_H
来源：http://mnk.sweek.top

#endif
来源：http://kjd.xuanzx.com

[S31] C++：Hello World
来源：http://ebp.tian-w.cn

#include <iostream>
来源：http://wlm.hywenlv.cn

int main() { std::cout << "Hello\n"; }
来源：http://kcs.gaohongyu789.top

[S32] C++：字符串
来源：http://akt.xingfuxueyuan.xyz

std::string s = "hi";  s += "!";
来源：http://xat.yfazqb.com

[S33] C++：vector 增删
来源：http://wqw.zhongyouzk.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://zgr.daxiang520.top

[S34] C++：遍历 vector
来源：http://tas.tian-w.cn

for (auto &x : v) { std::cout << x; }
来源：http://zko.cqqwz.cn

[S35] C++：map
来源：http://ibh.smart0.xyz

std::map<std::string, int> m;  m["a"] = 1;
来源：http://pdd.dianchejie.cn

[S36] C++：unordered_map
来源：http://icv.xuetiantiany.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://ijk.mhx1999.top

[S37] C++：set
来源：http://tem.yongpay.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://ovx.hesvh.cn

[S38] C++：排序
来源：http://vej.mhx1999.top

std::sort(v.begin(), v.end());
来源：http://mzh.zhiwuduotai.top

[S39] C++：自定义比较器排序
来源：http://pua.chenlongwang.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://lyp.zhoulong.xyz

[S40] C++：查找元素
来源：http://uta.quarkkingdee.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://qqm.hfpthk.cn

[S41] C++：类与构造函数
来源：http://vhl.sxryk.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://dav.xziqi.cn

[S42] C++：继承与虚函数
来源：http://dke.kuanghao11.cn

class B : public Base { public: void f() override {} };
来源：http://mul.hnxiangtu.top

[S43] C++：智能指针
来源：http://ruh.gotoacloud.top

auto p = std::make_unique<int>(5);
来源：http://xtp.zhijiandao.cn

[S44] C++：引用传参
来源：http://vpz.nanxinkj.top

void inc(int &x) { ++x; }
来源：http://bly.feifeiyinyue.top

[S45] C++：lambda
来源：http://aex.fengsongda.top

auto add = [](int a, int b) { return a + b; };
来源：http://rbl.birdmap.top

[S46] C++：函数模板
来源：http://gho.wangdashe.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://aft.shanyushiyangkeji.top

[S47] C++：结构化绑定遍历
来源：http://vsn.0kj1m.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://exf.jinqigufen.top

[S48] C++：逐行读文件
来源：http://ojo.yanxiufei.cn

std::ifstream in("a.txt");  std::string line;
来源：http://onm.cdnleiting.top

while (std::getline(in, line)) { }
来源：http://ibp.birdmap.top

[S49] C++：写文件
来源：http://raf.chenlongwang.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://swh.hcnkem.com

[S50] C++：格式化数字
来源：http://nni.fzhhl.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://rao.sxryk.cn

[S51] C++：显式类型转换
来源：http://wou.tanke756.top

static_cast<double>(a) / b
来源：http://kbd.yanxiufei.cn

[S52] C++：const 与 noexcept
来源：http://dls.jinghuilouyu.cn

int size() const noexcept { return n_; }
来源：http://cku.iojbl.cn

[S53] C++：移动语义
来源：http://prj.daria6918.cn

std::vector<int> w = std::move(v);
来源：http://hnz.zdqjudy.top

[S54] C++：异常处理
来源：http://lkz.meibo888.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://dyo.jlsjyb.cn

[S55] C++：结构化绑定
来源：http://axs.nwbrower.top

auto [a, b] = std::make_pair(1, 2);
来源：http://aoc.hongshengwenyu.top

[S56] C++：optional
来源：http://iaz.jiagoushi.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://iih.chenjidiqi.icu

[S57] C++：编译期常量
来源：http://bgp.aibaodan.cn

constexpr int N = 10;
来源：http://grp.xingfuxueyuan.xyz

[S58] C++：命名空间
来源：http://evb.zycfv.cn

namespace ns { int f() { return 1; } }
来源：http://nfb.gzhubu.top

[S59] C++：静态断言
来源：http://lip.pengpengdd.cyou

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://fjf.wangshuangyany.cn

[S60] C++：遍历并删除元素
来源：http://bja.cashguo.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://afr.chenlongwang.top

================================================================================
来源：http://znb.zhiwuduotai.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://whm.cqqwz.cn

================================================================================
来源：http://kyb.ctjpmb.com

[T01] Kotlin：Hello World
来源：http://wlt.uphjek.com

println("Hello")
来源：http://fas.hesvh.cn

[T02] Kotlin：变量
来源：http://exc.dianchejie.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://dxs.redwolf501.top

[T03] Kotlin：字符串模板
来源：http://kow.xuetiantiany.cn

"值: $b"
来源：http://hdk.yangfankeji.com

[T04] Kotlin：空安全
来源：http://kbp.bjfxy.top

val n: String? = null;  n?.length
来源：http://bak.shzxlz.cn

[T05] Kotlin：when 表达式
来源：http://xbq.daxiang520.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://ulh.c1oappe.top

[T06] Kotlin：集合映射
来源：http://uab.daria6918.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://wpb.aibaodan.cn

[T07] Kotlin：集合过滤
来源：http://nju.yonumen.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://ssr.fengsongda.top

[T08] Kotlin：数据类
来源：http://clz.ybcxt.top

data class User(val name: String, val age: Int)
来源：http://mqr.dianchejie.cn

[T09] Kotlin：扩展函数
来源：http://vnw.guowangkeji.top

fun String.exclaim() = this + "!"
来源：http://rgp.tanke756.top

[T10] Kotlin：默认参数
来源：http://kxw.cheryme.top

fun greet(name: String = "World") = "Hi $name"
来源：http://gkw.hysaishi.cn

[T11] Kotlin：协程
来源：http://nlm.quarkkingdee.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://mge.quarkkingdee.top

[T12] Kotlin：解构声明
来源：http://hvv.andypj.xyz

val (a, b) = Pair(1, 2)
来源：http://rjc.316326.xyz

[T13] Kotlin：只读 Map
来源：http://ano.guannengcc.top

val m = mapOf("a" to 1)
来源：http://bso.hnxiangtu.top

[T14] Kotlin：循环
来源：http://mra.nanxinkj.top

for (i in 1..10) println(i)
来源：http://ugw.uphjek.com

[T15] Kotlin：接口
来源：http://cxh.xuanzx.com

interface Shape { fun area(): Double }
来源：http://vbi.redwolf501.top

[T16] Swift：Hello World
来源：http://toz.hfpthk.cn

print("Hello")
来源：http://voo.xuanzx.com

[T17] Swift：变量与常量
来源：http://iga.yuanzhike.top

var a = 1;  let b = 2
来源：http://wst.feifeiyinyue.top

[T18] Swift：字符串插值
来源：http://cnb.tian-w.cn

"值: \(b)"
来源：http://slo.shzxlz.cn

[T19] Swift：可选绑定
来源：http://kxw.fzhhl.top

if let n = opt { print(n) }
来源：http://xpc.zhoulong.xyz

[T20] Swift：数组操作
来源：http://btu.gzhubu.top

var a = [1, 2, 3];  a.append(4)
来源：http://pkn.fengsongda.top

[T21] Swift：遍历
来源：http://dpk.haohaochexian.top

for x in a { print(x) }
来源：http://tkx.xziqi.cn

[T22] Swift：字典
来源：http://mnx.yangfankeji.com

var d = ["a": 1];  d["b"] = 2
来源：http://vpd.ydzc1.top

[T23] Swift：函数
来源：http://mcd.bjfxy.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://aiq.cucudq.cn

[T24] Swift：闭包
来源：http://knw.havefunace.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://mgu.birdmap.top

[T25] Swift：结构体
来源：http://hbw.chenlongwang.top

struct P { var x: Int }
来源：http://trc.yvedp.cn

[T26] Swift：类与重写
来源：http://hlu.nanxinkj.top

class A: Base { override func f() {} }
来源：http://wlt.xinyue.icu

[T27] Swift：错误处理
来源：http://asa.zhijiandao.cn

do { try f() } catch { print(error) }
来源：http://rgq.jyoumei.cn

[T28] Swift：枚举
来源：http://uir.jlsjyb.cn

enum Color { case red, green }
来源：http://frq.zdbjq.cn

[T29] Swift：guard 提前返回
来源：http://tez.yanxiufei.cn

guard let x = opt else { return }
来源：http://kxe.fengsongda.top

[T30] Swift：协议
来源：http://uci.gzhubu.top

protocol Shape { func area() -> Double }
来源：http://ecs.redwolf501.top

[T31] Lua：Hello World
来源：http://yat.bbcook.cn

print("Hello")
来源：http://mcr.fktsv.cn

[T32] Lua：局部变量
来源：http://xlj.gogol.net.cn

local a = 1
来源：http://cmp.xingfuxueyuan.xyz

[T33] Lua：表（数组）
来源：http://yst.tanke756.top

local t = {1, 2, 3};  t[4] = 4
来源：http://uxt.yongpay.top

[T34] Lua：遍历表
来源：http://ofx.shangyingyoupin.top

for i, v in ipairs(t) do print(i, v) end
来源：http://axk.ivvv.top

[T35] Lua：字典表
来源：http://fak.fanxiaobao.xyz

local d = { a = 1 };  d.b = 2
来源：http://ytc.snrcjt.cn

[T36] Lua：函数
来源：http://lcq.epnwcf.com

function add(a, b) return a + b end
来源：http://vqp.shanyushiyangkeji.top

[T37] Lua：字符串拼接
来源：http://hbf.haohaochexian.top

"a" .. "b"
来源：http://uar.svipenyu.cn

[T38] Lua：条件
来源：http://lth.yj20258888.top

if x > 0 then print("正") end
来源：http://mvb.jqgfzy.top

[T39] Lua：模式匹配
来源：http://uaa.cashguo.top

string.find(s, "%d+")
来源：http://fyi.jqgufenzy.top

[T40] Lua：元表
来源：http://tcn.jinghuilouyu.cn

setmetatable({}, { __index = base })
来源：http://mis.jyoumei.cn

[T41] Perl：Hello World
来源：http://yfn.havefunace.top

print "Hello\n";
来源：http://tum.cqqwz.cn

[T42] Perl：变量类型
来源：http://lbh.52xcode.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://fvr.aizwys.cn

[T43] Perl：字符串插值
来源：http://icm.jinqigfzy.top

"值: $a"
来源：http://sif.yvedp.cn

[T44] Perl：条件
来源：http://iql.wangdashe.top

if ($a > 0) { print "正"; }
来源：http://xge.jyoumei.cn

[T45] Perl：数组遍历
来源：http://icd.ywan-chungtsiang.top

for my $x (@arr) { print $x; }
来源：http://zbr.haohaochexian.top

[T46] Perl：哈希操作
来源：http://mvz.yuxming.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://zet.epnwcf.com

[T47] Perl：正则捕获
来源：http://tya.ybcxt.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://yiw.svipenyu.cn

[T48] Perl：正则替换
来源：http://fld.sweek.top

$s =~ s/old/new/g;
来源：http://ozh.fzhhl.top

[T49] Perl：函数
来源：http://nwv.fzhhl.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://uyt.fzhhl.top

[T50] Perl：逐行读文件
来源：http://opf.yueranfly.top

open my $fh, "<", "a.txt" or die $!;
来源：http://ffr.wangshuangyany.cn

while (my $line = <$fh>) { print $line; }
来源：http://jor.feifeiyinyue.top

[T51] Scala：Hello World
来源：http://tnl.redwolf501.top

println("Hello")
来源：http://ouc.hongshengwenyu.top

[T52] Scala：变量
来源：http://sib.vqdsnc.cn

val a = 1;  var b = 2
来源：http://qay.shzxlz.cn

[T53] Scala：字符串插值
来源：http://msv.andypj.xyz

s"值: $b"
来源：http://lsc.tarul.cn

[T54] Scala：集合映射
来源：http://xes.aizwys.cn

List(1, 2, 3).map(_ * 2)
来源：http://fvo.jqgfzy.top

[T55] Scala：集合过滤
来源：http://vik.nanxinkj.top

List(1, 2, 3).filter(_ > 1)
来源：http://gwg.ivvv.top

[T56] Scala：样例类
来源：http://bcw.sweek.top

case class User(name: String, age: Int)
来源：http://mav.feifeiyinyue.top

[T57] Scala：模式匹配
来源：http://vxr.jqgufenzy.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://ejr.sweek.top

[T58] Scala：函数定义
来源：http://mlm.xuanzx.com

def add(a: Int, b: Int): Int = a + b
来源：http://fml.dianchejie.cn

[T59] Scala：循环
来源：http://ipl.dashuyun.cn

for (i <- 1 to 10) println(i)
来源：http://uet.dianchejie.cn

[T60] Scala：折叠
来源：http://odj.hammf.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hpb.ehwqpu.com

================================================================================
来源：http://qhl.uphjek.com

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://npk.jqgfzy.top

================================================================================
来源：http://jtd.nanxinkj.top

[U01] Py：创建虚拟环境
来源：http://qee.hnqzz.top

python -m venv .venv && source .venv/bin/activate
来源：http://nwh.shzxlz.cn

[U02] Py：导出 / 安装依赖
来源：http://luo.iojbl.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://qwo.yvedp.cn

[U03] Py：加载 .env 配置
来源：http://sxn.sjlbkw.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://zwz.hesvh.cn

[U04] Py：变量调试打印
来源：http://wpb.yj202588.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://olb.dianchejie.cn

[U05] Py：列表去重且保序
来源：http://ltg.hesvh.cn

list(dict.fromkeys(arr))
来源：http://sum.zhoulong.xyz

[U06] Py：合并两个字典
来源：http://gqd.xinyue.icu

{**a, **b}
来源：http://gxd.9152youxi.cn

[U07] Py：反转字典键值
来源：http://ckp.hcnkem.com

{v: k for k, v in d.items()}
来源：http://fxb.jyoumei.cn

[U08] Py：展平二维列表
来源：http://adh.hesvh.cn

[y for x in nested for y in x]
来源：http://uxn.andypj.xyz

[U09] Py：字典取最大值的键
来源：http://ouy.hesvh.cn

max(d, key=d.get)
来源：http://lnk.gogol.net.cn

[U10] Py：按值排序字典
来源：http://mlz.yfazqb.com

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://slu.aizwys.cn

[U11] Py：生成器表达式
来源：http://gex.jinqigfzy.top

(x * 2 for x in arr)
来源：http://ltm.shanyushiyangtech.top

[U12] Py：取出现最多的 3 个元素
来源：http://hcj.jqgufenzy.top

Counter(arr).most_common(3)
来源：http://cyv.tianlin.xyz

[U13] Py：固定长度队列
来源：http://ggq.jinqigufen.top

deque(maxlen=10)
来源：http://arb.hfpthk.cn

[U14] Py：分组收集到列表
来源：http://tww.xingfuxueyuan.xyz

defaultdict(list)
来源：http://uxc.sufxvd.cn

[U15] Py：高精度计时
来源：http://xtw.0kj1m.cn

t = time.perf_counter()
来源：http://uys.uphjek.com

[U16] Py：命令行参数解析
来源：http://llk.sweek.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hfr.pengpengdd.cyou

[U17] Py：初始化日志
来源：http://coz.shanyushiyangkeji.top

logging.basicConfig(level=logging.INFO)
来源：http://hbt.cqqwz.cn

[U18] Py：预编译正则
来源：http://dff.hnxiangtu.top

pat = re.compile(r"\d+")
来源：http://ewl.yueranfly.top

[U19] Py：正则替换带回调
来源：http://rpd.hysaishi.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://xvm.hfpthk.cn

[U20] Py：缓存函数结果
来源：http://npq.kuanghao11.cn

@functools.lru_cache(maxsize=None)
来源：http://rdz.gogol.net.cn

[U21] Py：自定义上下文管理器
来源：http://nsl.ydzc1.top

@contextlib.contextmanager
来源：http://syp.bjfxy.top

[U22] Py：矩阵转置
来源：http://ejx.tianlin.xyz

list(zip(*m))
来源：http://lgu.ybcxt.top

[U23] Py：分块读取大文件
来源：http://dsv.aizwys.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://gmp.daxiang520.top

[U24] Py：路径操作
来源：http://qln.jinqigufen.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hme.ctjpmb.com

[U25] Py：CSV 按字典读
来源：http://qxi.xuetiantiany.cn

csv.DictReader(f)
来源：http://oix.nanxuanxn.top

[U26] Py：并发下载
来源：http://sgd.gaohongyu789.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://sly.zhiwuduotai.top

[U27] Py：异步 HTTP
来源：http://opn.yfazqb.com

aiohttp.ClientSession() 配合 async with
来源：http://yzq.aibaodan.cn

[U28] Py：类型别名
来源：http://cnf.iojbl.cn

UserId = int
来源：http://rqm.jinyuanbaomall.cn

[U29] Py：属性校验
来源：http://ybg.meibo888.top

@property 与 @x.setter 配合
来源：http://gdu.jinqigfzy.top

[U30] Py：数据类
来源：http://mvo.cucudq.cn

@dataclass(slots=True)
来源：http://hxx.vqdsnc.cn

[U31] Py：单测
来源：http://tnr.zhongyouzk.top

python -m pytest -q
来源：http://iwa.52xcode.cn

[U32] Py：代码格式化
来源：http://hhr.kuanghao11.cn

ruff format . && ruff check --fix .
来源：http://wgf.sufxvd.cn

[U33] Py：打包发布
来源：http://avv.guowangkeji.top

python -m build  （依赖 pyproject.toml）
来源：http://hac.yongpay.top

[U34] Py：判断编码
来源：http://ntm.havefunace.top

chardet.detect(raw)
来源：http://sim.haohaochexian.top

[U35] Py：发送邮件
来源：http://dvc.52xcode.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://pjj.jinqigfzy.top

[U36] Py：定时任务
来源：http://pib.guowangkeji.top

schedule.every(10).minutes.do(job)
来源：http://pon.zhijiandao.cn

[U37] Py：读写 Excel
来源：http://gqa.jinyuanbaomall.cn

pandas.read_excel / DataFrame.to_excel
来源：http://rzv.bjfxy.top

[U38] Py：获取脚本所在目录
来源：http://fux.wangshuangyany.cn

Path(__file__).resolve().parent
来源：http://gem.zdqjudy.top

[U39] Py：判断是否在交互环境
来源：http://xvd.yangfankeji.com

sys.stdout.isatty()
来源：http://gbs.svipenyu.cn

[U40] Py：打印到标准错误
来源：http://fta.shangyingyoupin.top

print("err", file=sys.stderr)
来源：http://zlf.kuanghao11.cn

[U41] PHP：初始化 Composer 项目
来源：http://ztl.tianlin.xyz

composer init;  composer require guzzlehttp/guzzle
来源：http://nfi.zhijiandao.cn

[U42] PHP：PSR-4 自动加载
来源：http://ocv.gaohongyu789.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://izn.hammf.cn

[U43] PHP：声明命名空间
来源：http://lgg.uphjek.com

namespace App\Http;
来源：http://bni.c1oappe.top

[U44] PHP：开启严格类型
来源：http://bte.jinghuilouyu.cn

declare(strict_types=1);
来源：http://klm.zhongyouzk.top

[U45] PHP：类型声明与返回类型
来源：http://dqp.tian-w.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://ojv.yj20258.top

[U46] PHP：可空类型
来源：http://hnn.pengpengdd.cyou

?string $name = null
来源：http://fap.andypj.xyz

[U47] PHP：联合类型
来源：http://sae.andypj.xyz

int|string $id
来源：http://whn.andypj.xyz

[U48] PHP：纯枚举
来源：http://gxl.yueranfly.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://gjr.ybcxt.top

[U49] PHP：只读属性
来源：http://oux.nanxinkj.top

public readonly string $name
来源：http://rot.xinyue.icu

[U50] PHP：构造器属性提升
来源：http://jcr.yj20258.top

public function __construct(private int $id) {}
来源：http://mpr.tanke756.top

[U51] PHP：数组解构
来源：http://lax.xziqi.cn

[$a, $b] = $arr;
来源：http://xby.hcnkem.com

[U52] PHP：箭头函数
来源：http://ivd.sxryk.cn

$double = fn($x) => $x * 2;
来源：http://anf.mhx1999.top


<!-- 参考信息 -->