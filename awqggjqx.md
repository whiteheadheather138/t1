代发 wailian999

[S33] C++：vector 增删
来源：http://twi.zhengqikj.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://ngh.yvedp.cn

[S34] C++：遍历 vector
来源：http://lpv.cqqwz.cn

for (auto &x : v) { std::cout << x; }
来源：http://twq.smart0.xyz

[S35] C++：map
来源：http://wnf.yanxiufei.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://cda.yanxiufei.cn

[S36] C++：unordered_map
来源：http://rmd.sjlbkw.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://oqp.gaohongyu789.top

[S37] C++：set
来源：http://aub.wangshuangyany.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://mnd.cqqwz.cn

[S38] C++：排序
来源：http://qql.snrcjt.cn

std::sort(v.begin(), v.end());
来源：http://iic.bjfxy.top

[S39] C++：自定义比较器排序
来源：http://ofg.cdnleiting.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://elo.hesvh.cn

[S40] C++：查找元素
来源：http://xru.tarul.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://bba.bjfxy.top

[S41] C++：类与构造函数
来源：http://vrg.aibaodan.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://qrd.hysaishi.cn

[S42] C++：继承与虚函数
来源：http://tdu.shanyushiyangtech.top

class B : public Base { public: void f() override {} };
来源：http://tng.jiagoushi.top

[S43] C++：智能指针
来源：http://ydd.wangshuangyany.cn

auto p = std::make_unique<int>(5);
来源：http://ljr.ppjwa.cn

[S44] C++：引用传参
来源：http://wbx.ywan-chungtsiang.top

void inc(int &x) { ++x; }
来源：http://nge.zhaomingkeji.xyz

[S45] C++：lambda
来源：http://bbj.yuanzhike.top

auto add = [](int a, int b) { return a + b; };
来源：http://aut.daxiang520.top

[S46] C++：函数模板
来源：http://ppy.yueranfly.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://exs.zhoulong.xyz

[S47] C++：结构化绑定遍历
来源：http://mys.jinghuilouyu.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://diy.tanke756.top

[S48] C++：逐行读文件
来源：http://bmt.hysaishi.cn

std::ifstream in("a.txt");  std::string line;
来源：http://tyf.guowangkeji.top

while (std::getline(in, line)) { }
来源：http://kyk.nanxuanxn.top

[S49] C++：写文件
来源：http://guk.yuanzhike.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://rgx.hnqzz.top

[S50] C++：格式化数字
来源：http://qim.cashguo.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://kno.zhongyouzk.top

[S51] C++：显式类型转换
来源：http://ekq.birdmap.top

static_cast<double>(a) / b
来源：http://lbz.hongshengwenyu.top

[S52] C++：const 与 noexcept
来源：http://dmb.cdnleiting.top

int size() const noexcept { return n_; }
来源：http://pou.tarul.cn

[S53] C++：移动语义
来源：http://lpi.ctjpmb.com

std::vector<int> w = std::move(v);
来源：http://ugf.chenjidiqi.icu

[S54] C++：异常处理
来源：http://trb.ywan-chungtsiang.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://wqm.jianghu66.top

[S55] C++：结构化绑定
来源：http://fsr.fengsongda.top

auto [a, b] = std::make_pair(1, 2);
来源：http://lht.sweek.top

[S56] C++：optional
来源：http://htr.sjlbkw.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://zgc.gaohongyu789.top

[S57] C++：编译期常量
来源：http://ulu.nanxuanxn.top

constexpr int N = 10;
来源：http://cox.meibo888.top

[S58] C++：命名空间
来源：http://ytc.fengsongda.top

namespace ns { int f() { return 1; } }
来源：http://kks.jlsjyb.cn

[S59] C++：静态断言
来源：http://vff.hywenlv.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://mnn.quarkkingdee.top

[S60] C++：遍历并删除元素
来源：http://ooa.shzxlz.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://zxw.guannengcc.top

================================================================================
来源：http://lvv.wangshuangyany.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://ird.vehdjk.com

================================================================================
来源：http://xjn.cqqwz.cn

[T01] Kotlin：Hello World
来源：http://dxf.vehdjk.com

println("Hello")
来源：http://qkl.jinyuanbaomall.cn

[T02] Kotlin：变量
来源：http://yqo.yj20258888.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://rim.zdbjq.cn

[T03] Kotlin：字符串模板
来源：http://tts.hongshengwenyu.top

"值: $b"
来源：http://otk.hnxiangtu.top

[T04] Kotlin：空安全
来源：http://tla.hongshengwenyu.top

val n: String? = null;  n?.length
来源：http://xoh.nanxuanxn.top

[T05] Kotlin：when 表达式
来源：http://ivp.guannengcc.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://vzc.sufxvd.cn

[T06] Kotlin：集合映射
来源：http://old.wangshuangyany.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://ozc.cucudq.cn

[T07] Kotlin：集合过滤
来源：http://ghl.shanyushiyangkeji.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://miw.andypj.xyz

[T08] Kotlin：数据类
来源：http://gmv.jinqigfzy.top

data class User(val name: String, val age: Int)
来源：http://hka.cucudq.cn

[T09] Kotlin：扩展函数
来源：http://zkq.sxryk.cn

fun String.exclaim() = this + "!"
来源：http://awn.xingfuxueyuan.xyz

[T10] Kotlin：默认参数
来源：http://zea.ppjwa.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://arm.hongshengwenyu.top

[T11] Kotlin：协程
来源：http://kgj.meibo888.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://ggj.jqgfzy.top

[T12] Kotlin：解构声明
来源：http://vhx.yj202588.top

val (a, b) = Pair(1, 2)
来源：http://kxe.gotoacloud.top

[T13] Kotlin：只读 Map
来源：http://yve.xziqi.cn

val m = mapOf("a" to 1)
来源：http://eue.shanyushiyangkeji.top

[T14] Kotlin：循环
来源：http://fki.havefunace.top

for (i in 1..10) println(i)
来源：http://fjy.fanxiaobao.xyz

[T15] Kotlin：接口
来源：http://vqx.guannengcc.top

interface Shape { fun area(): Double }
来源：http://rnw.yj20258.top

[T16] Swift：Hello World
来源：http://eis.guannengcc.top

print("Hello")
来源：http://roc.chenzaomai.com

[T17] Swift：变量与常量
来源：http://bew.0kj1m.cn

var a = 1;  let b = 2
来源：http://yci.ydjk.org.cn

[T18] Swift：字符串插值
来源：http://zcu.yj202588.top

"值: \(b)"
来源：http://ykw.jinqigufen.top

[T19] Swift：可选绑定
来源：http://qph.nwbrower.top

if let n = opt { print(n) }
来源：http://cdu.yonumen.top

[T20] Swift：数组操作
来源：http://zzh.xylfe.cn

var a = [1, 2, 3];  a.append(4)
来源：http://uwh.gzhubu.top

[T21] Swift：遍历
来源：http://ztu.daxiang520.top

for x in a { print(x) }
来源：http://kqs.fktsv.cn

[T22] Swift：字典
来源：http://pjn.aizwys.cn

var d = ["a": 1];  d["b"] = 2
来源：http://mlz.ehwqpu.com

[T23] Swift：函数
来源：http://sif.hammf.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://gms.cashguo.top

[T24] Swift：闭包
来源：http://wbn.fanxiaobao.xyz

let f = { (x: Int) -> Int in x * 2 }
来源：http://hur.mhx1999.top

[T25] Swift：结构体
来源：http://yuw.shanyushiyangtech.top

struct P { var x: Int }
来源：http://rnw.daxiang520.top

[T26] Swift：类与重写
来源：http://rwu.jianghu66.top

class A: Base { override func f() {} }
来源：http://ssj.xingfuxueyuan.xyz

[T27] Swift：错误处理
来源：http://jpa.tanke756.top

do { try f() } catch { print(error) }
来源：http://iia.jinyuanbaomall.cn

[T28] Swift：枚举
来源：http://kcf.andypj.xyz

enum Color { case red, green }
来源：http://ckl.yj20258.top

[T29] Swift：guard 提前返回
来源：http://zqr.xingfuxueyuan.xyz

guard let x = opt else { return }
来源：http://syv.cdnleiting.top

[T30] Swift：协议
来源：http://yph.fanxiaobao.xyz

protocol Shape { func area() -> Double }
来源：http://nsu.tianlin.xyz

[T31] Lua：Hello World
来源：http://kal.yongpay.top

print("Hello")
来源：http://dus.yueranfly.top

[T32] Lua：局部变量
来源：http://kvz.guannengcc.top

local a = 1
来源：http://mbo.yj202588.top

[T33] Lua：表（数组）
来源：http://kpg.tanke756.top

local t = {1, 2, 3};  t[4] = 4
来源：http://hbc.dashuyun.cn

[T34] Lua：遍历表
来源：http://haz.meibo888.top

for i, v in ipairs(t) do print(i, v) end
来源：http://uof.nanxuanxn.top

[T35] Lua：字典表
来源：http://jqh.shanyushiyangkeji.top

local d = { a = 1 };  d.b = 2
来源：http://jfw.yangfankeji.com

[T36] Lua：函数
来源：http://uei.pycfn.com

function add(a, b) return a + b end
来源：http://trt.shangyingyoupin.top

[T37] Lua：字符串拼接
来源：http://wrq.ehwqpu.com

"a" .. "b"
来源：http://xtk.tianlin.xyz

[T38] Lua：条件
来源：http://xvr.daxiang520.top

if x > 0 then print("正") end
来源：http://lch.c1oappe.top

[T39] Lua：模式匹配
来源：http://drr.zhongyouzk.top

string.find(s, "%d+")
来源：http://ypc.gaohongyu789.top

[T40] Lua：元表
来源：http://osx.uphjek.com

setmetatable({}, { __index = base })
来源：http://xzf.redwolf501.top

[T41] Perl：Hello World
来源：http://daq.ivvv.top

print "Hello\n";
来源：http://lwp.wangdashe.top

[T42] Perl：变量类型
来源：http://nhd.vqdsnc.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://wqr.vqdsnc.cn

[T43] Perl：字符串插值
来源：http://has.vqdsnc.cn

"值: $a"
来源：http://zat.0kj1m.cn

[T44] Perl：条件
来源：http://uth.zhengqikj.top

if ($a > 0) { print "正"; }
来源：http://qsk.hfpthk.cn

[T45] Perl：数组遍历
来源：http://cgi.redwolf501.top

for my $x (@arr) { print $x; }
来源：http://lnp.daria6918.cn

[T46] Perl：哈希操作
来源：http://sro.jianghu66.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://wwt.ywan-chungtsiang.top

[T47] Perl：正则捕获
来源：http://pmc.ywan-chungtsiang.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://mis.shanyushiyangtech.top

[T48] Perl：正则替换
来源：http://kqu.hesvh.cn

$s =~ s/old/new/g;
来源：http://vuf.hcnkem.com

[T49] Perl：函数
来源：http://fnl.jinghuilouyu.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hqd.mhx1999.top

[T50] Perl：逐行读文件
来源：http://pwl.tanke756.top

open my $fh, "<", "a.txt" or die $!;
来源：http://wee.ydjk.org.cn

while (my $line = <$fh>) { print $line; }
来源：http://vhi.fehbvm.com

[T51] Scala：Hello World
来源：http://ocv.havefunace.top

println("Hello")
来源：http://lxi.zhixingplan.top

[T52] Scala：变量
来源：http://uze.zhengqikj.top

val a = 1;  var b = 2
来源：http://kcu.tian-w.cn

[T53] Scala：字符串插值
来源：http://qpe.yueranfly.top

s"值: $b"
来源：http://gru.tian-w.cn

[T54] Scala：集合映射
来源：http://cjc.fzhhl.top

List(1, 2, 3).map(_ * 2)
来源：http://wbd.quarkkingdee.top

[T55] Scala：集合过滤
来源：http://oiz.ivvv.top

List(1, 2, 3).filter(_ > 1)
来源：http://ovg.zhiwuduotai.top

[T56] Scala：样例类
来源：http://zgv.hfpthk.cn

case class User(name: String, age: Int)
来源：http://spm.fengsongda.top

[T57] Scala：模式匹配
来源：http://tjx.jinqigufen.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://bvi.wangdashe.top

[T58] Scala：函数定义
来源：http://dvo.hammf.cn

def add(a: Int, b: Int): Int = a + b
来源：http://ugf.yuanzhike.top

[T59] Scala：循环
来源：http://uln.daria6918.cn

for (i <- 1 to 10) println(i)
来源：http://dmy.hnqzz.top

[T60] Scala：折叠
来源：http://ohx.mhx1999.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://vok.yj20258.top

================================================================================
来源：http://dxm.shuidangran.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://oxw.nanxuanxn.top

================================================================================
来源：http://otq.sxryk.cn

[U01] Py：创建虚拟环境
来源：http://hgh.zhongyouzk.top

python -m venv .venv && source .venv/bin/activate
来源：http://lsn.zhoulong.xyz

[U02] Py：导出 / 安装依赖
来源：http://voh.xylfe.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://dee.zdbjq.cn

[U03] Py：加载 .env 配置
来源：http://mkm.sufxvd.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://zmj.haohaochexian.top

[U04] Py：变量调试打印
来源：http://xvh.pycfn.com

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://ofp.guowangkeji.top

[U05] Py：列表去重且保序
来源：http://xiq.fehbvm.com

list(dict.fromkeys(arr))
来源：http://daj.gaohongyu789.top

[U06] Py：合并两个字典
来源：http://rjf.guowangkeji.top

{**a, **b}
来源：http://ocp.hnqzz.top

[U07] Py：反转字典键值
来源：http://ewm.andypj.xyz

{v: k for k, v in d.items()}
来源：http://tgs.0kj1m.cn

[U08] Py：展平二维列表
来源：http://tou.svipenyu.cn

[y for x in nested for y in x]
来源：http://rwm.fzhhl.top

[U09] Py：字典取最大值的键
来源：http://kzd.andypj.xyz

max(d, key=d.get)
来源：http://fes.yj20258.top

[U10] Py：按值排序字典
来源：http://fol.xylfe.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://rxd.sweek.top

[U11] Py：生成器表达式
来源：http://ouv.ywan-chungtsiang.top

(x * 2 for x in arr)
来源：http://twr.cashguo.top

[U12] Py：取出现最多的 3 个元素
来源：http://xbi.yuxming.cn

Counter(arr).most_common(3)
来源：http://cof.xuetiantiany.cn

[U13] Py：固定长度队列
来源：http://mzi.havefunace.top

deque(maxlen=10)
来源：http://tgb.xinyue.icu

[U14] Py：分组收集到列表
来源：http://lzw.zhengqikj.top

defaultdict(list)
来源：http://syg.cqqwz.cn

[U15] Py：高精度计时
来源：http://epd.dashuyun.cn

t = time.perf_counter()
来源：http://sqc.gogol.net.cn

[U16] Py：命令行参数解析
来源：http://oui.iojbl.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://rbf.wangdashe.top

[U17] Py：初始化日志
来源：http://xov.52xcode.cn

logging.basicConfig(level=logging.INFO)
来源：http://vac.zhixingplan.top

[U18] Py：预编译正则
来源：http://uld.hammf.cn

pat = re.compile(r"\d+")
来源：http://cev.cheryme.top

[U19] Py：正则替换带回调
来源：http://mnf.vqdsnc.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://pft.pengpengdd.cyou

[U20] Py：缓存函数结果
来源：http://vvq.fzhhl.top

@functools.lru_cache(maxsize=None)
来源：http://kvo.pengpengdd.cyou

[U21] Py：自定义上下文管理器
来源：http://xmf.hongshengwenyu.top

@contextlib.contextmanager
来源：http://pro.iojbl.cn

[U22] Py：矩阵转置
来源：http://vya.chenzaomai.com

list(zip(*m))
来源：http://kkd.zdqjudy.top

[U23] Py：分块读取大文件
来源：http://xxl.jqgfzy.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://gja.shanyushiyangtech.top

[U24] Py：路径操作
来源：http://yma.jyoumei.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://pga.fzhhl.top

[U25] Py：CSV 按字典读
来源：http://xri.zhengqikj.top

csv.DictReader(f)
来源：http://oyt.0kj1m.cn

[U26] Py：并发下载
来源：http://bxt.gzhubu.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://wys.shanyushiyangkeji.top

[U27] Py：异步 HTTP
来源：http://joc.52xcode.cn

aiohttp.ClientSession() 配合 async with
来源：http://vsk.wangshuangyany.cn

[U28] Py：类型别名
来源：http://mmb.zhengqikj.top

UserId = int
来源：http://aqz.shzxlz.cn

[U29] Py：属性校验
来源：http://hor.316326.xyz

@property 与 @x.setter 配合
来源：http://tyr.jinyuanbaomall.cn

[U30] Py：数据类
来源：http://hgb.svipenyu.cn

@dataclass(slots=True)
来源：http://mpg.quarkkingdee.top

[U31] Py：单测
来源：http://rbh.yongpay.top

python -m pytest -q
来源：http://vej.sufxvd.cn

[U32] Py：代码格式化
来源：http://kgx.snrcjt.cn

ruff format . && ruff check --fix .
来源：http://hbr.fzhhl.top

[U33] Py：打包发布
来源：http://sjo.pengpengdd.cyou

python -m build  （依赖 pyproject.toml）
来源：http://tfe.shanyushiyangtech.top

[U34] Py：判断编码
来源：http://ivo.ivvv.top

chardet.detect(raw)
来源：http://fhh.daxiang520.top

[U35] Py：发送邮件
来源：http://yhz.zycfv.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://tuk.yueranfly.top

[U36] Py：定时任务
来源：http://efz.quarkkingdee.top

schedule.every(10).minutes.do(job)
来源：http://tws.nanxuanxn.top

[U37] Py：读写 Excel
来源：http://dzb.hfpthk.cn

pandas.read_excel / DataFrame.to_excel
来源：http://cpp.zycfv.cn

[U38] Py：获取脚本所在目录
来源：http://zpf.gotoacloud.top

Path(__file__).resolve().parent
来源：http://xdw.wangdashe.top

[U39] Py：判断是否在交互环境
来源：http://bcg.yongpay.top

sys.stdout.isatty()
来源：http://iom.xziqi.cn

[U40] Py：打印到标准错误
来源：http://aui.yfazqb.com

print("err", file=sys.stderr)
来源：http://tvs.fanxiaobao.xyz

[U41] PHP：初始化 Composer 项目
来源：http://dqf.hnxiangtu.top

composer init;  composer require guzzlehttp/guzzle
来源：http://atu.cucudq.cn

[U42] PHP：PSR-4 自动加载
来源：http://bao.andypj.xyz

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://emh.fengsongda.top

[U43] PHP：声明命名空间
来源：http://ols.xuanzx.com

namespace App\Http;
来源：http://vgq.yongpay.top

[U44] PHP：开启严格类型
来源：http://huf.yonumen.top

declare(strict_types=1);
来源：http://iml.meibo888.top

[U45] PHP：类型声明与返回类型
来源：http://sfs.kuanghao11.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://wpw.jyoumei.cn

[U46] PHP：可空类型
来源：http://wge.jinyuanbaomall.cn

?string $name = null
来源：http://ulr.shanyushiyangkeji.top

[U47] PHP：联合类型
来源：http://ujh.shuidangran.top

int|string $id
来源：http://rth.tianlin.xyz

[U48] PHP：纯枚举
来源：http://qsv.vqdsnc.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://wei.pengpengdd.cyou

[U49] PHP：只读属性
来源：http://eds.xinyue.icu

public readonly string $name
来源：http://ioo.hammf.cn

[U50] PHP：构造器属性提升
来源：http://aid.316326.xyz

public function __construct(private int $id) {}
来源：http://rgc.shangyingyoupin.top

[U51] PHP：数组解构
来源：http://btp.shanyushiyangtech.top

[$a, $b] = $arr;
来源：http://fzq.zhiwuduotai.top

[U52] PHP：箭头函数
来源：http://ret.hammf.cn

$double = fn($x) => $x * 2;
来源：http://rmc.sweek.top

[U53] PHP：空合并运算符
来源：http://hly.yonumen.top

$v = $a ?? $b ?? "default";
来源：http://ntf.cashguo.top

[U54] PHP：空安全调用
来源：http://qdo.gaohongyu789.top

$obj?->method()
来源：http://xfk.redwolf501.top

[U55] PHP：match 表达式
来源：http://ock.yj202588.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://kfd.xinyue.icu

[U56] PHP：命名参数
来源：http://nyi.yonumen.top

f(a: 1, b: 2)
来源：http://lmt.tianlin.xyz

[U57] PHP：字符串插值
来源：http://rxi.andypj.xyz

"值: {$a}"
来源：http://wms.vqdsnc.cn

[U58] PHP：数组三件套
来源：http://gpi.gotoacloud.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://mwk.aizwys.cn


<!-- 参考信息 -->