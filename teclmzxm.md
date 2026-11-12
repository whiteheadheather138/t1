代发 wailian999

atoi("42");  strtod("3.14", NULL);
来源：http://svc.52xcode.cn

[S23] C：随机数
来源：http://lyx.52xcode.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://eez.ydjk.org.cn

[S24] C：获取本地时间
来源：http://dgj.zhijiandao.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://cgn.ywan-chungtsiang.top

[S25] C：内存拷贝
来源：http://aio.wangdashe.top

memcpy(dst, src, n);
来源：http://teh.ybcxt.top

[S26] C：内存清零
来源：http://vnf.jinqigfzy.top

memset(a, 0, sizeof a);
来源：http://omc.shuidangran.top

[S27] C：定义常量
来源：http://ybu.xuanzx.com

const double PI = 3.14159;
来源：http://bdp.fktsv.cn

[S28] C：静态变量
来源：http://zzq.hongshengwenyu.top

static int counter = 0;
来源：http://bhh.xuetiantiany.cn

[S29] C：变参函数
来源：http://inv.yuxming.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://tyf.wangshuangyany.cn

[S30] C：头文件保护
来源：http://hqb.tian-w.cn

#ifndef X_H
来源：http://hyi.shangyingyoupin.top

#define X_H
来源：http://jmm.ywan-chungtsiang.top

#endif
来源：http://ogb.fengsongda.top

[S31] C++：Hello World
来源：http://kll.yueranfly.top

#include <iostream>
来源：http://lzc.ywan-chungtsiang.top

int main() { std::cout << "Hello\n"; }
来源：http://vlm.gzhubu.top

[S32] C++：字符串
来源：http://dqj.yonumen.top

std::string s = "hi";  s += "!";
来源：http://jfj.jinyuanbaomall.cn

[S33] C++：vector 增删
来源：http://kpg.316326.xyz

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://lgx.52xcode.cn

[S34] C++：遍历 vector
来源：http://pkg.shzxlz.cn

for (auto &x : v) { std::cout << x; }
来源：http://kyj.yuxming.cn

[S35] C++：map
来源：http://wvl.feifeiyinyue.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://qan.jianghu66.top

[S36] C++：unordered_map
来源：http://vex.hfpthk.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hzm.sjlbkw.cn

[S37] C++：set
来源：http://eya.hammf.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://afm.zhijiandao.cn

[S38] C++：排序
来源：http://exu.hywenlv.cn

std::sort(v.begin(), v.end());
来源：http://tdo.ivvv.top

[S39] C++：自定义比较器排序
来源：http://szm.dashuyun.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://rdu.yueranfly.top

[S40] C++：查找元素
来源：http://rox.yuanzhike.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://ido.xuanzx.com

[S41] C++：类与构造函数
来源：http://cln.gzhubu.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://cpv.tianlin.xyz

[S42] C++：继承与虚函数
来源：http://zqu.svipenyu.cn

class B : public Base { public: void f() override {} };
来源：http://zgf.fktsv.cn

[S43] C++：智能指针
来源：http://qzp.zhaomingkeji.xyz

auto p = std::make_unique<int>(5);
来源：http://uag.xuetiantiany.cn

[S44] C++：引用传参
来源：http://plv.yueranfly.top

void inc(int &x) { ++x; }
来源：http://xvn.feifeiyinyue.top

[S45] C++：lambda
来源：http://zpg.zhongyouzk.top

auto add = [](int a, int b) { return a + b; };
来源：http://hex.wangdashe.top

[S46] C++：函数模板
来源：http://wkc.yuanzhike.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://lwv.jiagoushi.top

[S47] C++：结构化绑定遍历
来源：http://mws.shanyushiyangkeji.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://ovn.zhixingplan.top

[S48] C++：逐行读文件
来源：http://adq.yonumen.top

std::ifstream in("a.txt");  std::string line;
来源：http://rdb.yanxiufei.cn

while (std::getline(in, line)) { }
来源：http://bzd.quarkkingdee.top

[S49] C++：写文件
来源：http://bah.chenjidiqi.icu

std::ofstream out("a.txt");  out << "hi\n";
来源：http://gcl.wangshuangyany.cn

[S50] C++：格式化数字
来源：http://qdb.andypj.xyz

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://jvn.wangdashe.top

[S51] C++：显式类型转换
来源：http://hbe.shangyingyoupin.top

static_cast<double>(a) / b
来源：http://qbs.dianchejie.cn

[S52] C++：const 与 noexcept
来源：http://nxf.zhongyouzk.top

int size() const noexcept { return n_; }
来源：http://dog.nanxuanxn.top

[S53] C++：移动语义
来源：http://rmv.cashguo.top

std::vector<int> w = std::move(v);
来源：http://znf.tarul.cn

[S54] C++：异常处理
来源：http://yjc.ydjk.org.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://unp.yanxiufei.cn

[S55] C++：结构化绑定
来源：http://wpu.quarkkingdee.top

auto [a, b] = std::make_pair(1, 2);
来源：http://awz.kuanghao11.cn

[S56] C++：optional
来源：http://rsy.c1oappe.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://shu.xziqi.cn

[S57] C++：编译期常量
来源：http://nao.shanyushiyangkeji.top

constexpr int N = 10;
来源：http://lle.kuanghao11.cn

[S58] C++：命名空间
来源：http://llc.jinqigfzy.top

namespace ns { int f() { return 1; } }
来源：http://vwv.fanxiaobao.xyz

[S59] C++：静态断言
来源：http://ppu.yonumen.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://uai.zhiwuduotai.top

[S60] C++：遍历并删除元素
来源：http://she.sweek.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://mcp.jinyuanbaomall.cn

================================================================================
来源：http://kos.shanyushiyangkeji.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://wrp.xingfuxueyuan.xyz

================================================================================
来源：http://lbu.daria6918.cn

[T01] Kotlin：Hello World
来源：http://szb.tianlin.xyz

println("Hello")
来源：http://eza.zhoulong.xyz

[T02] Kotlin：变量
来源：http://uzb.yuanzhike.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://eae.zhixingplan.top

[T03] Kotlin：字符串模板
来源：http://soz.wangdashe.top

"值: $b"
来源：http://yzy.xingfuxueyuan.xyz

[T04] Kotlin：空安全
来源：http://qde.xuanzx.com

val n: String? = null;  n?.length
来源：http://gsd.chenjidiqi.icu

[T05] Kotlin：when 表达式
来源：http://bab.cqqwz.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://wpm.yuanzhike.top

[T06] Kotlin：集合映射
来源：http://qva.c1oappe.top

listOf(1, 2, 3).map { it * 2 }
来源：http://lsz.jyoumei.cn

[T07] Kotlin：集合过滤
来源：http://dcn.svipenyu.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://tfi.tarul.cn

[T08] Kotlin：数据类
来源：http://uxw.tanke756.top

data class User(val name: String, val age: Int)
来源：http://mui.zhoulong.xyz

[T09] Kotlin：扩展函数
来源：http://lnp.jianghu66.top

fun String.exclaim() = this + "!"
来源：http://ihx.fktsv.cn

[T10] Kotlin：默认参数
来源：http://oqg.yanxiufei.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://fxo.gotoacloud.top

[T11] Kotlin：协程
来源：http://upd.tianlin.xyz

GlobalScope.launch { delay(1000); println("done") }
来源：http://csx.tianlin.xyz

[T12] Kotlin：解构声明
来源：http://uxz.hnqzz.top

val (a, b) = Pair(1, 2)
来源：http://wmw.tianlin.xyz

[T13] Kotlin：只读 Map
来源：http://toc.xingfuxueyuan.xyz

val m = mapOf("a" to 1)
来源：http://oep.ydjk.org.cn

[T14] Kotlin：循环
来源：http://oaq.havefunace.top

for (i in 1..10) println(i)
来源：http://mol.xingfuxueyuan.xyz

[T15] Kotlin：接口
来源：http://zbp.guannengcc.top

interface Shape { fun area(): Double }
来源：http://ddk.mhx1999.top

[T16] Swift：Hello World
来源：http://ztj.svipenyu.cn

print("Hello")
来源：http://scy.shangyingyoupin.top

[T17] Swift：变量与常量
来源：http://iom.cucudq.cn

var a = 1;  let b = 2
来源：http://xjd.hammf.cn

[T18] Swift：字符串插值
来源：http://ydv.chenjidiqi.icu

"值: \(b)"
来源：http://eqt.hfpthk.cn

[T19] Swift：可选绑定
来源：http://yly.gaohongyu789.top

if let n = opt { print(n) }
来源：http://gqh.cheryme.top

[T20] Swift：数组操作
来源：http://zas.c1oappe.top

var a = [1, 2, 3];  a.append(4)
来源：http://job.fengsongda.top

[T21] Swift：遍历
来源：http://gnk.vehdjk.com

for x in a { print(x) }
来源：http://kzu.yuxming.cn

[T22] Swift：字典
来源：http://dhz.mhx1999.top

var d = ["a": 1];  d["b"] = 2
来源：http://ugz.havefunace.top

[T23] Swift：函数
来源：http://zqm.jqgfzy.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://abx.dashuyun.cn

[T24] Swift：闭包
来源：http://frx.hesvh.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://wgm.yj20258.top

[T25] Swift：结构体
来源：http://ijt.fzhhl.top

struct P { var x: Int }
来源：http://qxs.xinyue.icu

[T26] Swift：类与重写
来源：http://jax.ehwqpu.com

class A: Base { override func f() {} }
来源：http://ziu.kuanghao11.cn

[T27] Swift：错误处理
来源：http://gnj.xziqi.cn

do { try f() } catch { print(error) }
来源：http://ztw.sufxvd.cn

[T28] Swift：枚举
来源：http://dnn.ybcxt.top

enum Color { case red, green }
来源：http://wmr.fktsv.cn

[T29] Swift：guard 提前返回
来源：http://cxe.zhijiandao.cn

guard let x = opt else { return }
来源：http://enb.jinghuilouyu.cn

[T30] Swift：协议
来源：http://qqk.tarul.cn

protocol Shape { func area() -> Double }
来源：http://ddq.ybcxt.top

[T31] Lua：Hello World
来源：http://hzq.hesvh.cn

print("Hello")
来源：http://hds.zhixingplan.top

[T32] Lua：局部变量
来源：http://xxd.vehdjk.com

local a = 1
来源：http://klm.cdnleiting.top

[T33] Lua：表（数组）
来源：http://eyb.mhx1999.top

local t = {1, 2, 3};  t[4] = 4
来源：http://shc.ydzc1.top

[T34] Lua：遍历表
来源：http://jzp.zdqjudy.top

for i, v in ipairs(t) do print(i, v) end
来源：http://wnw.fehbvm.com

[T35] Lua：字典表
来源：http://nhv.meibo888.top

local d = { a = 1 };  d.b = 2
来源：http://ufc.sxryk.cn

[T36] Lua：函数
来源：http://clv.ppjwa.cn

function add(a, b) return a + b end
来源：http://jwp.ctjpmb.com

[T37] Lua：字符串拼接
来源：http://qov.0kj1m.cn

"a" .. "b"
来源：http://gnq.zdbjq.cn

[T38] Lua：条件
来源：http://szd.hysaishi.cn

if x > 0 then print("正") end
来源：http://boy.cheryme.top

[T39] Lua：模式匹配
来源：http://gph.shuidangran.top

string.find(s, "%d+")
来源：http://cyg.vqdsnc.cn

[T40] Lua：元表
来源：http://fnu.tianlin.xyz

setmetatable({}, { __index = base })
来源：http://wbs.yj202588.top

[T41] Perl：Hello World
来源：http://qql.nanxuanxn.top

print "Hello\n";
来源：http://nwh.ydzc1.top

[T42] Perl：变量类型
来源：http://tdj.gaohongyu789.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://lnd.andypj.xyz

[T43] Perl：字符串插值
来源：http://sfa.zdqjudy.top

"值: $a"
来源：http://zly.fktsv.cn

[T44] Perl：条件
来源：http://ifg.tanke756.top

if ($a > 0) { print "正"; }
来源：http://zcd.nanxuanxn.top

[T45] Perl：数组遍历
来源：http://uqq.yuanzhike.top

for my $x (@arr) { print $x; }
来源：http://nzj.9152youxi.cn

[T46] Perl：哈希操作
来源：http://vyw.yanxiufei.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://xto.fehbvm.com

[T47] Perl：正则捕获
来源：http://mri.shangyingyoupin.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://cvy.zhengqikj.top

[T48] Perl：正则替换
来源：http://chk.shzxlz.cn

$s =~ s/old/new/g;
来源：http://rag.dianchejie.cn

[T49] Perl：函数
来源：http://rfo.yvedp.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://wye.andypj.xyz

[T50] Perl：逐行读文件
来源：http://pwh.yj202588.top

open my $fh, "<", "a.txt" or die $!;
来源：http://xjl.vqdsnc.cn

while (my $line = <$fh>) { print $line; }
来源：http://bfm.tarul.cn

[T51] Scala：Hello World
来源：http://hoc.cashguo.top

println("Hello")
来源：http://hew.tanke756.top

[T52] Scala：变量
来源：http://sja.jlsjyb.cn

val a = 1;  var b = 2
来源：http://avb.nanxinkj.top

[T53] Scala：字符串插值
来源：http://zrx.jqgufenzy.top

s"值: $b"
来源：http://bhe.bbcook.cn

[T54] Scala：集合映射
来源：http://ucr.zdbjq.cn

List(1, 2, 3).map(_ * 2)
来源：http://jii.aibaodan.cn

[T55] Scala：集合过滤
来源：http://bbi.shuidangran.top

List(1, 2, 3).filter(_ > 1)
来源：http://bmz.cashguo.top

[T56] Scala：样例类
来源：http://ceh.ivvv.top

case class User(name: String, age: Int)
来源：http://bdt.aizwys.cn

[T57] Scala：模式匹配
来源：http://ols.shanyushiyangtech.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://svs.sjlbkw.cn

[T58] Scala：函数定义
来源：http://pjs.daria6918.cn

def add(a: Int, b: Int): Int = a + b
来源：http://oql.sufxvd.cn

[T59] Scala：循环
来源：http://dja.ivvv.top

for (i <- 1 to 10) println(i)
来源：http://bzt.guowangkeji.top

[T60] Scala：折叠
来源：http://ujg.zycfv.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://xiz.fktsv.cn

================================================================================
来源：http://ggc.ivvv.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://vem.guannengcc.top

================================================================================
来源：http://omk.fehbvm.com

[U01] Py：创建虚拟环境
来源：http://ngx.gotoacloud.top

python -m venv .venv && source .venv/bin/activate
来源：http://pdq.xuetiantiany.cn

[U02] Py：导出 / 安装依赖
来源：http://lqh.zdbjq.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://irw.havefunace.top

[U03] Py：加载 .env 配置
来源：http://yoz.cqqwz.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://cnx.yj20258.top

[U04] Py：变量调试打印
来源：http://wkl.yanxiufei.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://ovs.havefunace.top

[U05] Py：列表去重且保序
来源：http://fst.chenzaomai.com

list(dict.fromkeys(arr))
来源：http://rkq.hnxiangtu.top

[U06] Py：合并两个字典
来源：http://bjb.zhaomingkeji.xyz

{**a, **b}
来源：http://oxd.cqqwz.cn

[U07] Py：反转字典键值
来源：http://ytd.uphjek.com

{v: k for k, v in d.items()}
来源：http://wos.dashuyun.cn

[U08] Py：展平二维列表
来源：http://vyc.shuidangran.top

[y for x in nested for y in x]
来源：http://tis.sufxvd.cn

[U09] Py：字典取最大值的键
来源：http://pkc.ydjk.org.cn

max(d, key=d.get)
来源：http://nie.jqgfzy.top

[U10] Py：按值排序字典
来源：http://aag.snrcjt.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://dmn.shanyushiyangtech.top

[U11] Py：生成器表达式
来源：http://ajz.hcnkem.com

(x * 2 for x in arr)
来源：http://whb.aizwys.cn

[U12] Py：取出现最多的 3 个元素
来源：http://ine.zhongyouzk.top

Counter(arr).most_common(3)
来源：http://yeh.cashguo.top

[U13] Py：固定长度队列
来源：http://xri.guowangkeji.top

deque(maxlen=10)
来源：http://ggs.pengpengdd.cyou

[U14] Py：分组收集到列表
来源：http://jck.nanxinkj.top

defaultdict(list)
来源：http://tmy.hongshengwenyu.top

[U15] Py：高精度计时
来源：http://ioy.aibaodan.cn

t = time.perf_counter()
来源：http://hzi.xuetiantiany.cn

[U16] Py：命令行参数解析
来源：http://bvc.zhoulong.xyz

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://pom.aizwys.cn

[U17] Py：初始化日志
来源：http://wsx.chenjidiqi.icu

logging.basicConfig(level=logging.INFO)
来源：http://jdv.bjfxy.top

[U18] Py：预编译正则
来源：http://ypp.zdbjq.cn

pat = re.compile(r"\d+")
来源：http://lue.aibaodan.cn

[U19] Py：正则替换带回调
来源：http://bef.wangdashe.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://pzh.guannengcc.top

[U20] Py：缓存函数结果
来源：http://gsk.daxiang520.top

@functools.lru_cache(maxsize=None)
来源：http://mqh.52xcode.cn

[U21] Py：自定义上下文管理器
来源：http://afd.chenlongwang.top

@contextlib.contextmanager
来源：http://awn.jqgufenzy.top

[U22] Py：矩阵转置
来源：http://wcy.yuanzhike.top

list(zip(*m))
来源：http://kto.kuanghao11.cn

[U23] Py：分块读取大文件
来源：http://dvd.andypj.xyz

for chunk in iter(lambda: f.read(8192), b""):
来源：http://vop.pycfn.com

[U24] Py：路径操作
来源：http://spz.tian-w.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://oas.zhixingplan.top

[U25] Py：CSV 按字典读
来源：http://jfk.aizwys.cn

csv.DictReader(f)
来源：http://ndv.jqgfzy.top

[U26] Py：并发下载
来源：http://vju.epnwcf.com

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://kmd.zhiwuduotai.top

[U27] Py：异步 HTTP
来源：http://wqz.ppjwa.cn

aiohttp.ClientSession() 配合 async with
来源：http://ijp.dianchejie.cn

[U28] Py：类型别名
来源：http://iqw.fzhhl.top

UserId = int
来源：http://igm.yj202588.top

[U29] Py：属性校验
来源：http://agf.jianghu66.top

@property 与 @x.setter 配合
来源：http://fzk.zhijiandao.cn

[U30] Py：数据类
来源：http://rqy.daxiang520.top

@dataclass(slots=True)
来源：http://cfd.havefunace.top

[U31] Py：单测
来源：http://xnd.hongshengwenyu.top

python -m pytest -q
来源：http://gnt.hnxiangtu.top

[U32] Py：代码格式化
来源：http://fkt.bjfxy.top

ruff format . && ruff check --fix .
来源：http://mzu.wangshuangyany.cn

[U33] Py：打包发布
来源：http://bza.smart0.xyz

python -m build  （依赖 pyproject.toml）
来源：http://nfc.mhx1999.top

[U34] Py：判断编码
来源：http://tfe.yanxiufei.cn

chardet.detect(raw)
来源：http://hxr.fktsv.cn

[U35] Py：发送邮件
来源：http://czr.yanxiufei.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://abg.jyoumei.cn

[U36] Py：定时任务
来源：http://kby.mhx1999.top

schedule.every(10).minutes.do(job)
来源：http://bid.yvedp.cn

[U37] Py：读写 Excel
来源：http://kos.gzhubu.top

pandas.read_excel / DataFrame.to_excel
来源：http://nxb.jinyuanbaomall.cn

[U38] Py：获取脚本所在目录
来源：http://urr.yanxiufei.cn

Path(__file__).resolve().parent
来源：http://ixr.cashguo.top

[U39] Py：判断是否在交互环境
来源：http://jfk.birdmap.top

sys.stdout.isatty()
来源：http://xsu.cashguo.top

[U40] Py：打印到标准错误
来源：http://bsd.sufxvd.cn

print("err", file=sys.stderr)
来源：http://cpl.nwbrower.top

[U41] PHP：初始化 Composer 项目
来源：http://eif.haohaochexian.top

composer init;  composer require guzzlehttp/guzzle
来源：http://gbl.0kj1m.cn

[U42] PHP：PSR-4 自动加载
来源：http://hvp.shangyingyoupin.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://mzt.shangyingyoupin.top

[U43] PHP：声明命名空间
来源：http://ool.tianlin.xyz

namespace App\Http;
来源：http://hsn.tian-w.cn

[U44] PHP：开启严格类型
来源：http://eju.zdbjq.cn

declare(strict_types=1);
来源：http://eld.shuidangran.top

[U45] PHP：类型声明与返回类型
来源：http://jey.snrcjt.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://nwu.cheryme.top

[U46] PHP：可空类型
来源：http://zmo.sweek.top

?string $name = null
来源：http://pjv.yj20258.top


<!-- 参考信息 -->