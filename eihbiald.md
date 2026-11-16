代发 wailian999

[S33] C++：vector 增删
来源：http://btr.ctjpmb.com

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://oak.cashguo.top

[S34] C++：遍历 vector
来源：http://vtg.tianlin.xyz

for (auto &x : v) { std::cout << x; }
来源：http://aii.zhongyouzk.top

[S35] C++：map
来源：http://egd.gzhubu.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://lws.redwolf501.top

[S36] C++：unordered_map
来源：http://qol.tianlin.xyz

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://ulp.kuanghao11.cn

[S37] C++：set
来源：http://cdp.jqgfzy.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://lxr.gotoacloud.top

[S38] C++：排序
来源：http://crz.nwbrower.top

std::sort(v.begin(), v.end());
来源：http://fbg.pengpengdd.cyou

[S39] C++：自定义比较器排序
来源：http://hjm.tanke756.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://gmm.dashuyun.cn

[S40] C++：查找元素
来源：http://eum.9152youxi.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://rny.gotoacloud.top

[S41] C++：类与构造函数
来源：http://agm.zycfv.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://cvz.jinqigfzy.top

[S42] C++：继承与虚函数
来源：http://jnu.pycfn.com

class B : public Base { public: void f() override {} };
来源：http://ipo.jianghu66.top

[S43] C++：智能指针
来源：http://gfx.jinyuanbaomall.cn

auto p = std::make_unique<int>(5);
来源：http://frt.zhaomingkeji.xyz

[S44] C++：引用传参
来源：http://zba.vqdsnc.cn

void inc(int &x) { ++x; }
来源：http://stw.chenlongwang.top

[S45] C++：lambda
来源：http://cxs.feifeiyinyue.top

auto add = [](int a, int b) { return a + b; };
来源：http://mfp.yuxming.cn

[S46] C++：函数模板
来源：http://ujt.yonumen.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://tek.fehbvm.com

[S47] C++：结构化绑定遍历
来源：http://hoy.wangdashe.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hrj.xinyue.icu

[S48] C++：逐行读文件
来源：http://ftt.c1oappe.top

std::ifstream in("a.txt");  std::string line;
来源：http://zhz.hfpthk.cn

while (std::getline(in, line)) { }
来源：http://niz.quarkkingdee.top

[S49] C++：写文件
来源：http://bey.jinghuilouyu.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://pux.quarkkingdee.top

[S50] C++：格式化数字
来源：http://iyk.jinghuilouyu.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://uwp.cucudq.cn

[S51] C++：显式类型转换
来源：http://sbz.havefunace.top

static_cast<double>(a) / b
来源：http://fob.guannengcc.top

[S52] C++：const 与 noexcept
来源：http://hks.tanke756.top

int size() const noexcept { return n_; }
来源：http://zmn.zhixingplan.top

[S53] C++：移动语义
来源：http://hap.havefunace.top

std::vector<int> w = std::move(v);
来源：http://oed.sxryk.cn

[S54] C++：异常处理
来源：http://vmf.epnwcf.com

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://mrg.guannengcc.top

[S55] C++：结构化绑定
来源：http://sxd.sxryk.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://sac.vqdsnc.cn

[S56] C++：optional
来源：http://kei.ywan-chungtsiang.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://djz.wangdashe.top

[S57] C++：编译期常量
来源：http://zuz.jqgfzy.top

constexpr int N = 10;
来源：http://ukw.jinqigfzy.top

[S58] C++：命名空间
来源：http://vwv.yj20258.top

namespace ns { int f() { return 1; } }
来源：http://ica.9152youxi.cn

[S59] C++：静态断言
来源：http://wke.chenjidiqi.icu

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hiw.jinqigufen.top

[S60] C++：遍历并删除元素
来源：http://jqb.pengpengdd.cyou

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://mdz.andypj.xyz

================================================================================
来源：http://cdl.316326.xyz

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://xkv.jqgufenzy.top

================================================================================
来源：http://ixi.jiagoushi.top

[T01] Kotlin：Hello World
来源：http://ker.fanxiaobao.xyz

println("Hello")
来源：http://nbk.aibaodan.cn

[T02] Kotlin：变量
来源：http://xej.bjfxy.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://rnh.ehwqpu.com

[T03] Kotlin：字符串模板
来源：http://ljr.chenzaomai.com

"值: $b"
来源：http://ozw.zdqjudy.top

[T04] Kotlin：空安全
来源：http://fqw.hcnkem.com

val n: String? = null;  n?.length
来源：http://pyd.xuetiantiany.cn

[T05] Kotlin：when 表达式
来源：http://axv.xuanzx.com

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://fiz.gotoacloud.top

[T06] Kotlin：集合映射
来源：http://xgq.c1oappe.top

listOf(1, 2, 3).map { it * 2 }
来源：http://bnn.mhx1999.top

[T07] Kotlin：集合过滤
来源：http://kkk.jinqigfzy.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://xdg.0kj1m.cn

[T08] Kotlin：数据类
来源：http://dxr.sxryk.cn

data class User(val name: String, val age: Int)
来源：http://uxx.hammf.cn

[T09] Kotlin：扩展函数
来源：http://fwk.gogol.net.cn

fun String.exclaim() = this + "!"
来源：http://vss.birdmap.top

[T10] Kotlin：默认参数
来源：http://gqz.quarkkingdee.top

fun greet(name: String = "World") = "Hi $name"
来源：http://dld.tanke756.top

[T11] Kotlin：协程
来源：http://yvw.wangshuangyany.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://apg.guannengcc.top

[T12] Kotlin：解构声明
来源：http://stk.ehwqpu.com

val (a, b) = Pair(1, 2)
来源：http://eys.jinqigfzy.top

[T13] Kotlin：只读 Map
来源：http://rwc.haohaochexian.top

val m = mapOf("a" to 1)
来源：http://pni.0kj1m.cn

[T14] Kotlin：循环
来源：http://xan.yj202588.top

for (i in 1..10) println(i)
来源：http://xko.bjfxy.top

[T15] Kotlin：接口
来源：http://hwz.zhiwuduotai.top

interface Shape { fun area(): Double }
来源：http://crp.ydjk.org.cn

[T16] Swift：Hello World
来源：http://jjw.sxryk.cn

print("Hello")
来源：http://kbt.xylfe.cn

[T17] Swift：变量与常量
来源：http://tgn.c1oappe.top

var a = 1;  let b = 2
来源：http://vpk.ydjk.org.cn

[T18] Swift：字符串插值
来源：http://eca.iojbl.cn

"值: \(b)"
来源：http://skz.zdbjq.cn

[T19] Swift：可选绑定
来源：http://rje.zhiwuduotai.top

if let n = opt { print(n) }
来源：http://ojh.fanxiaobao.xyz

[T20] Swift：数组操作
来源：http://hzz.cucudq.cn

var a = [1, 2, 3];  a.append(4)
来源：http://wbf.zycfv.cn

[T21] Swift：遍历
来源：http://imn.svipenyu.cn

for x in a { print(x) }
来源：http://cjh.hysaishi.cn

[T22] Swift：字典
来源：http://yot.smart0.xyz

var d = ["a": 1];  d["b"] = 2
来源：http://yaj.gaohongyu789.top

[T23] Swift：函数
来源：http://ntu.hcnkem.com

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://pwc.shuidangran.top

[T24] Swift：闭包
来源：http://xyq.uphjek.com

let f = { (x: Int) -> Int in x * 2 }
来源：http://swi.ehwqpu.com

[T25] Swift：结构体
来源：http://uzg.ydjk.org.cn

struct P { var x: Int }
来源：http://zdd.chenzaomai.com

[T26] Swift：类与重写
来源：http://ahk.cheryme.top

class A: Base { override func f() {} }
来源：http://kor.tian-w.cn

[T27] Swift：错误处理
来源：http://zha.pengpengdd.cyou

do { try f() } catch { print(error) }
来源：http://jxm.chenzaomai.com

[T28] Swift：枚举
来源：http://dqs.zhongyouzk.top

enum Color { case red, green }
来源：http://nvf.xuetiantiany.cn

[T29] Swift：guard 提前返回
来源：http://rwn.cdnleiting.top

guard let x = opt else { return }
来源：http://zag.chenjidiqi.icu

[T30] Swift：协议
来源：http://vzg.wangshuangyany.cn

protocol Shape { func area() -> Double }
来源：http://fqv.hongshengwenyu.top

[T31] Lua：Hello World
来源：http://cxg.feifeiyinyue.top

print("Hello")
来源：http://thq.hcnkem.com

[T32] Lua：局部变量
来源：http://tna.jqgufenzy.top

local a = 1
来源：http://tqj.xylfe.cn

[T33] Lua：表（数组）
来源：http://yxb.vqdsnc.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://emb.yuanzhike.top

[T34] Lua：遍历表
来源：http://rab.chenzaomai.com

for i, v in ipairs(t) do print(i, v) end
来源：http://quk.snrcjt.cn

[T35] Lua：字典表
来源：http://yqa.cdnleiting.top

local d = { a = 1 };  d.b = 2
来源：http://oog.yvedp.cn

[T36] Lua：函数
来源：http://wrh.ctjpmb.com

function add(a, b) return a + b end
来源：http://efo.guowangkeji.top

[T37] Lua：字符串拼接
来源：http://mgh.aibaodan.cn

"a" .. "b"
来源：http://xva.jinqigufen.top

[T38] Lua：条件
来源：http://sfb.quarkkingdee.top

if x > 0 then print("正") end
来源：http://ajk.shzxlz.cn

[T39] Lua：模式匹配
来源：http://bad.yj20258888.top

string.find(s, "%d+")
来源：http://czn.gogol.net.cn

[T40] Lua：元表
来源：http://seg.pycfn.com

setmetatable({}, { __index = base })
来源：http://lbb.cdnleiting.top

[T41] Perl：Hello World
来源：http://whp.snrcjt.cn

print "Hello\n";
来源：http://tcz.jlsjyb.cn

[T42] Perl：变量类型
来源：http://cot.yongpay.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://ktx.daria6918.cn

[T43] Perl：字符串插值
来源：http://djq.fengsongda.top

"值: $a"
来源：http://ywl.shzxlz.cn

[T44] Perl：条件
来源：http://kxm.shuidangran.top

if ($a > 0) { print "正"; }
来源：http://hxd.fzhhl.top

[T45] Perl：数组遍历
来源：http://vsk.ydjk.org.cn

for my $x (@arr) { print $x; }
来源：http://ryc.wangdashe.top

[T46] Perl：哈希操作
来源：http://ghj.andypj.xyz

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://kfq.yuanzhike.top

[T47] Perl：正则捕获
来源：http://heg.zhongyouzk.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://iqp.yuanzhike.top

[T48] Perl：正则替换
来源：http://rte.uphjek.com

$s =~ s/old/new/g;
来源：http://vmw.feifeiyinyue.top

[T49] Perl：函数
来源：http://twk.pengpengdd.cyou

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://min.cucudq.cn

[T50] Perl：逐行读文件
来源：http://qis.zhoulong.xyz

open my $fh, "<", "a.txt" or die $!;
来源：http://mpc.gzhubu.top

while (my $line = <$fh>) { print $line; }
来源：http://psf.fehbvm.com

[T51] Scala：Hello World
来源：http://rgu.yj20258.top

println("Hello")
来源：http://apl.hammf.cn

[T52] Scala：变量
来源：http://ywb.hfpthk.cn

val a = 1;  var b = 2
来源：http://ioc.haohaochexian.top

[T53] Scala：字符串插值
来源：http://hgf.gogol.net.cn

s"值: $b"
来源：http://tca.jiagoushi.top

[T54] Scala：集合映射
来源：http://wjp.quarkkingdee.top

List(1, 2, 3).map(_ * 2)
来源：http://iiy.sjlbkw.cn

[T55] Scala：集合过滤
来源：http://pxg.hfpthk.cn

List(1, 2, 3).filter(_ > 1)
来源：http://jfk.zhengqikj.top

[T56] Scala：样例类
来源：http://fwp.yangfankeji.com

case class User(name: String, age: Int)
来源：http://oyj.jqgfzy.top

[T57] Scala：模式匹配
来源：http://xkb.snrcjt.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://fyf.xuetiantiany.cn

[T58] Scala：函数定义
来源：http://ttu.xingfuxueyuan.xyz

def add(a: Int, b: Int): Int = a + b
来源：http://zre.wangdashe.top

[T59] Scala：循环
来源：http://bmp.jlsjyb.cn

for (i <- 1 to 10) println(i)
来源：http://rjb.chenlongwang.top

[T60] Scala：折叠
来源：http://etd.hongshengwenyu.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://nxs.yvedp.cn

================================================================================
来源：http://ujs.birdmap.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://kia.redwolf501.top

================================================================================
来源：http://mfm.hammf.cn

[U01] Py：创建虚拟环境
来源：http://dwh.xuetiantiany.cn

python -m venv .venv && source .venv/bin/activate
来源：http://fst.ydjk.org.cn

[U02] Py：导出 / 安装依赖
来源：http://kqh.aibaodan.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://imk.nanxinkj.top

[U03] Py：加载 .env 配置
来源：http://onh.andypj.xyz

from dotenv import load_dotenv; load_dotenv()
来源：http://tyw.yongpay.top

[U04] Py：变量调试打印
来源：http://imf.yfazqb.com

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hhd.yfazqb.com

[U05] Py：列表去重且保序
来源：http://oja.cdnleiting.top

list(dict.fromkeys(arr))
来源：http://slh.yuanzhike.top

[U06] Py：合并两个字典
来源：http://ete.jianghu66.top

{**a, **b}
来源：http://ngw.yuanzhike.top

[U07] Py：反转字典键值
来源：http://sja.316326.xyz

{v: k for k, v in d.items()}
来源：http://wkk.sufxvd.cn

[U08] Py：展平二维列表
来源：http://oks.jlsjyb.cn

[y for x in nested for y in x]
来源：http://qdg.hfpthk.cn

[U09] Py：字典取最大值的键
来源：http://ejs.zhoulong.xyz

max(d, key=d.get)
来源：http://rkg.feifeiyinyue.top

[U10] Py：按值排序字典
来源：http://vug.daxiang520.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://gga.pycfn.com

[U11] Py：生成器表达式
来源：http://jke.hnxiangtu.top

(x * 2 for x in arr)
来源：http://daq.wangdashe.top

[U12] Py：取出现最多的 3 个元素
来源：http://ixr.jinghuilouyu.cn

Counter(arr).most_common(3)
来源：http://lng.jlsjyb.cn

[U13] Py：固定长度队列
来源：http://rsf.jinyuanbaomall.cn

deque(maxlen=10)
来源：http://tbv.mhx1999.top

[U14] Py：分组收集到列表
来源：http://gaa.meibo888.top

defaultdict(list)
来源：http://avm.yj20258.top

[U15] Py：高精度计时
来源：http://etr.hesvh.cn

t = time.perf_counter()
来源：http://znt.9152youxi.cn

[U16] Py：命令行参数解析
来源：http://apx.daria6918.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://iwh.52xcode.cn

[U17] Py：初始化日志
来源：http://ikm.c1oappe.top

logging.basicConfig(level=logging.INFO)
来源：http://jnr.yj20258888.top

[U18] Py：预编译正则
来源：http://dnr.nanxinkj.top

pat = re.compile(r"\d+")
来源：http://nhe.guannengcc.top

[U19] Py：正则替换带回调
来源：http://kuv.jlsjyb.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://pkw.ydzc1.top

[U20] Py：缓存函数结果
来源：http://emx.yvedp.cn

@functools.lru_cache(maxsize=None)
来源：http://iiz.zhaomingkeji.xyz

[U21] Py：自定义上下文管理器
来源：http://zin.daxiang520.top

@contextlib.contextmanager
来源：http://wwz.mhx1999.top

[U22] Py：矩阵转置
来源：http://hpp.aibaodan.cn

list(zip(*m))
来源：http://hjr.ydzc1.top

[U23] Py：分块读取大文件
来源：http://wdv.zhijiandao.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://sjj.zhijiandao.cn

[U24] Py：路径操作
来源：http://bjy.wangdashe.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://oli.epnwcf.com

[U25] Py：CSV 按字典读
来源：http://kzf.tianlin.xyz

csv.DictReader(f)
来源：http://oji.yuanzhike.top

[U26] Py：并发下载
来源：http://fvc.guowangkeji.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://auc.yueranfly.top

[U27] Py：异步 HTTP
来源：http://vim.hcnkem.com

aiohttp.ClientSession() 配合 async with
来源：http://ksx.meibo888.top

[U28] Py：类型别名
来源：http://rhk.fanxiaobao.xyz

UserId = int
来源：http://yju.birdmap.top

[U29] Py：属性校验
来源：http://oni.gzhubu.top

@property 与 @x.setter 配合
来源：http://knv.zhaomingkeji.xyz

[U30] Py：数据类
来源：http://win.ehwqpu.com

@dataclass(slots=True)
来源：http://mve.zhiwuduotai.top

[U31] Py：单测
来源：http://buj.jqgufenzy.top

python -m pytest -q
来源：http://jtd.ybcxt.top

[U32] Py：代码格式化
来源：http://vpk.yj202588.top

ruff format . && ruff check --fix .
来源：http://ahi.fehbvm.com

[U33] Py：打包发布
来源：http://xit.shzxlz.cn

python -m build  （依赖 pyproject.toml）
来源：http://ywl.ywan-chungtsiang.top

[U34] Py：判断编码
来源：http://jpu.yonumen.top

chardet.detect(raw)
来源：http://ogp.sufxvd.cn

[U35] Py：发送邮件
来源：http://sau.pengpengdd.cyou

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://kkw.cashguo.top

[U36] Py：定时任务
来源：http://syq.bjfxy.top

schedule.every(10).minutes.do(job)
来源：http://ang.ctjpmb.com

[U37] Py：读写 Excel
来源：http://mvo.yuanzhike.top

pandas.read_excel / DataFrame.to_excel
来源：http://yng.xuetiantiany.cn

[U38] Py：获取脚本所在目录
来源：http://hho.zdqjudy.top

Path(__file__).resolve().parent
来源：http://jjk.sjlbkw.cn

[U39] Py：判断是否在交互环境
来源：http://sec.bbcook.cn

sys.stdout.isatty()
来源：http://vhw.cdnleiting.top

[U40] Py：打印到标准错误
来源：http://ack.fktsv.cn

print("err", file=sys.stderr)
来源：http://sfn.chenjidiqi.icu

[U41] PHP：初始化 Composer 项目
来源：http://fpy.xuanzx.com

composer init;  composer require guzzlehttp/guzzle
来源：http://cyo.tarul.cn

[U42] PHP：PSR-4 自动加载
来源：http://kjf.ehwqpu.com

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://sho.fehbvm.com

[U43] PHP：声明命名空间
来源：http://dka.xuanzx.com

namespace App\Http;
来源：http://uwy.fzhhl.top

[U44] PHP：开启严格类型
来源：http://cds.gzhubu.top

declare(strict_types=1);
来源：http://myb.jyoumei.cn

[U45] PHP：类型声明与返回类型
来源：http://byh.haohaochexian.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://lix.ybcxt.top

[U46] PHP：可空类型
来源：http://ffk.gotoacloud.top

?string $name = null
来源：http://hsf.jyoumei.cn

[U47] PHP：联合类型
来源：http://iyr.hongshengwenyu.top

int|string $id
来源：http://nxx.jinqigufen.top

[U48] PHP：纯枚举
来源：http://xya.daxiang520.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://jdh.vehdjk.com

[U49] PHP：只读属性
来源：http://ebq.pycfn.com

public readonly string $name
来源：http://kjy.jqgufenzy.top

[U50] PHP：构造器属性提升
来源：http://qsn.gzhubu.top

public function __construct(private int $id) {}
来源：http://aqz.aibaodan.cn

[U51] PHP：数组解构
来源：http://aez.tianlin.xyz

[$a, $b] = $arr;
来源：http://exk.chenjidiqi.icu

[U52] PHP：箭头函数
来源：http://jfe.jianghu66.top

$double = fn($x) => $x * 2;
来源：http://hyb.kuanghao11.cn

[U53] PHP：空合并运算符
来源：http://pzr.aibaodan.cn

$v = $a ?? $b ?? "default";
来源：http://obd.vehdjk.com

[U54] PHP：空安全调用
来源：http://ovt.bjfxy.top

$obj?->method()
来源：http://tey.xuanzx.com

[U55] PHP：match 表达式
来源：http://qfj.meibo888.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://xxb.316326.xyz

[U56] PHP：命名参数
来源：http://vfz.daria6918.cn

f(a: 1, b: 2)
来源：http://hrf.0kj1m.cn

[U57] PHP：字符串插值
来源：http://suw.bbcook.cn

"值: {$a}"
来源：http://brw.sysykeji.top

[U58] PHP：数组三件套
来源：http://jkd.yangfankeji.com

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://dpz.chenlongwang.top


<!-- 参考信息 -->