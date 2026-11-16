代发 wailian999

[S33] C++：vector 增删
来源：http://tve.mhx1999.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://edw.hesvh.cn

[S34] C++：遍历 vector
来源：http://xmj.guannengcc.top

for (auto &x : v) { std::cout << x; }
来源：http://iad.nanxinkj.top

[S35] C++：map
来源：http://zum.bjfxy.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://mgh.zhijiandao.cn

[S36] C++：unordered_map
来源：http://zvb.hammf.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://uyw.pycfn.com

[S37] C++：set
来源：http://gty.xziqi.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://srx.zhixingplan.top

[S38] C++：排序
来源：http://fqr.mhx1999.top

std::sort(v.begin(), v.end());
来源：http://egg.quarkkingdee.top

[S39] C++：自定义比较器排序
来源：http://pnz.kuanghao11.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://klq.zhiwuduotai.top

[S40] C++：查找元素
来源：http://cbu.kuanghao11.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hqj.jlsjyb.cn

[S41] C++：类与构造函数
来源：http://sgu.hnqzz.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://rjt.zycfv.cn

[S42] C++：继承与虚函数
来源：http://anx.yonumen.top

class B : public Base { public: void f() override {} };
来源：http://kfl.jqgfzy.top

[S43] C++：智能指针
来源：http://vdh.tarul.cn

auto p = std::make_unique<int>(5);
来源：http://wwc.hongshengwenyu.top

[S44] C++：引用传参
来源：http://gxg.cdnleiting.top

void inc(int &x) { ++x; }
来源：http://ndr.sjlbkw.cn

[S45] C++：lambda
来源：http://tjn.shangyingyoupin.top

auto add = [](int a, int b) { return a + b; };
来源：http://kyg.yuanzhike.top

[S46] C++：函数模板
来源：http://wgk.yongpay.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://jmt.ybcxt.top

[S47] C++：结构化绑定遍历
来源：http://qxl.kuanghao11.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://xys.zhiwuduotai.top

[S48] C++：逐行读文件
来源：http://woy.sweek.top

std::ifstream in("a.txt");  std::string line;
来源：http://btv.havefunace.top

while (std::getline(in, line)) { }
来源：http://wtw.fzhhl.top

[S49] C++：写文件
来源：http://ksa.aibaodan.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://sjj.gzhubu.top

[S50] C++：格式化数字
来源：http://rps.shzxlz.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://wbt.gotoacloud.top

[S51] C++：显式类型转换
来源：http://dfd.redwolf501.top

static_cast<double>(a) / b
来源：http://fid.fanxiaobao.xyz

[S52] C++：const 与 noexcept
来源：http://nsl.hesvh.cn

int size() const noexcept { return n_; }
来源：http://dvb.chenjidiqi.icu

[S53] C++：移动语义
来源：http://qzj.quarkkingdee.top

std::vector<int> w = std::move(v);
来源：http://xil.gogol.net.cn

[S54] C++：异常处理
来源：http://znb.cdnleiting.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://wiw.hongshengwenyu.top

[S55] C++：结构化绑定
来源：http://lnl.zhengqikj.top

auto [a, b] = std::make_pair(1, 2);
来源：http://dfh.dashuyun.cn

[S56] C++：optional
来源：http://zft.andypj.xyz

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://swp.shzxlz.cn

[S57] C++：编译期常量
来源：http://gly.daxiang520.top

constexpr int N = 10;
来源：http://ohy.jyoumei.cn

[S58] C++：命名空间
来源：http://ckp.feifeiyinyue.top

namespace ns { int f() { return 1; } }
来源：http://dom.hysaishi.cn

[S59] C++：静态断言
来源：http://lkx.pycfn.com

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://ewp.yueranfly.top

[S60] C++：遍历并删除元素
来源：http://wuf.gotoacloud.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://blt.ppjwa.cn

================================================================================
来源：http://ryb.snrcjt.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://dkp.shangyingyoupin.top

================================================================================
来源：http://xcd.fzhhl.top

[T01] Kotlin：Hello World
来源：http://pov.aibaodan.cn

println("Hello")
来源：http://tub.nanxuanxn.top

[T02] Kotlin：变量
来源：http://npo.meibo888.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://sww.dianchejie.cn

[T03] Kotlin：字符串模板
来源：http://swb.zdqjudy.top

"值: $b"
来源：http://ilw.vehdjk.com

[T04] Kotlin：空安全
来源：http://emw.xinyue.icu

val n: String? = null;  n?.length
来源：http://dpu.xylfe.cn

[T05] Kotlin：when 表达式
来源：http://lmr.havefunace.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://wsp.xuanzx.com

[T06] Kotlin：集合映射
来源：http://wpz.hesvh.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://dhw.sweek.top

[T07] Kotlin：集合过滤
来源：http://ojs.xylfe.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://vit.cheryme.top

[T08] Kotlin：数据类
来源：http://afe.hesvh.cn

data class User(val name: String, val age: Int)
来源：http://xxi.wangshuangyany.cn

[T09] Kotlin：扩展函数
来源：http://fpl.redwolf501.top

fun String.exclaim() = this + "!"
来源：http://epc.gaohongyu789.top

[T10] Kotlin：默认参数
来源：http://zsa.hnqzz.top

fun greet(name: String = "World") = "Hi $name"
来源：http://xnh.ywan-chungtsiang.top

[T11] Kotlin：协程
来源：http://pnf.redwolf501.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://jxz.jinyuanbaomall.cn

[T12] Kotlin：解构声明
来源：http://fsm.hnxiangtu.top

val (a, b) = Pair(1, 2)
来源：http://qjb.jqgufenzy.top

[T13] Kotlin：只读 Map
来源：http://bya.ppjwa.cn

val m = mapOf("a" to 1)
来源：http://yyh.jyoumei.cn

[T14] Kotlin：循环
来源：http://zyc.yonumen.top

for (i in 1..10) println(i)
来源：http://tnb.jyoumei.cn

[T15] Kotlin：接口
来源：http://gtm.smart0.xyz

interface Shape { fun area(): Double }
来源：http://noo.sysykeji.top

[T16] Swift：Hello World
来源：http://tna.hesvh.cn

print("Hello")
来源：http://ank.gogol.net.cn

[T17] Swift：变量与常量
来源：http://zkn.cashguo.top

var a = 1;  let b = 2
来源：http://kao.xziqi.cn

[T18] Swift：字符串插值
来源：http://ewp.cucudq.cn

"值: \(b)"
来源：http://gbt.zhixingplan.top

[T19] Swift：可选绑定
来源：http://pug.quarkkingdee.top

if let n = opt { print(n) }
来源：http://amf.yanxiufei.cn

[T20] Swift：数组操作
来源：http://gff.jinqigfzy.top

var a = [1, 2, 3];  a.append(4)
来源：http://xtw.yvedp.cn

[T21] Swift：遍历
来源：http://uqr.vqdsnc.cn

for x in a { print(x) }
来源：http://kvx.daxiang520.top

[T22] Swift：字典
来源：http://sqr.tian-w.cn

var d = ["a": 1];  d["b"] = 2
来源：http://rfq.jianghu66.top

[T23] Swift：函数
来源：http://yqh.xziqi.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://kpe.redwolf501.top

[T24] Swift：闭包
来源：http://mbc.zycfv.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://wgo.shangyingyoupin.top

[T25] Swift：结构体
来源：http://xfg.yj20258.top

struct P { var x: Int }
来源：http://ibo.chenlongwang.top

[T26] Swift：类与重写
来源：http://wia.tianlin.xyz

class A: Base { override func f() {} }
来源：http://eqc.zdqjudy.top

[T27] Swift：错误处理
来源：http://atr.yongpay.top

do { try f() } catch { print(error) }
来源：http://vuz.ppjwa.cn

[T28] Swift：枚举
来源：http://opc.ivvv.top

enum Color { case red, green }
来源：http://vqu.yanxiufei.cn

[T29] Swift：guard 提前返回
来源：http://gog.aibaodan.cn

guard let x = opt else { return }
来源：http://ehv.yuxming.cn

[T30] Swift：协议
来源：http://zci.bjfxy.top

protocol Shape { func area() -> Double }
来源：http://vwu.fehbvm.com

[T31] Lua：Hello World
来源：http://brh.shanyushiyangtech.top

print("Hello")
来源：http://qva.pengpengdd.cyou

[T32] Lua：局部变量
来源：http://gfs.hcnkem.com

local a = 1
来源：http://vnz.jinqigfzy.top

[T33] Lua：表（数组）
来源：http://xep.tarul.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://frx.yuanzhike.top

[T34] Lua：遍历表
来源：http://pfu.nanxinkj.top

for i, v in ipairs(t) do print(i, v) end
来源：http://maj.yvedp.cn

[T35] Lua：字典表
来源：http://msa.nanxinkj.top

local d = { a = 1 };  d.b = 2
来源：http://wvs.jinyuanbaomall.cn

[T36] Lua：函数
来源：http://kzu.tian-w.cn

function add(a, b) return a + b end
来源：http://aoz.pycfn.com

[T37] Lua：字符串拼接
来源：http://wyr.jinghuilouyu.cn

"a" .. "b"
来源：http://shh.hnxiangtu.top

[T38] Lua：条件
来源：http://ucg.yueranfly.top

if x > 0 then print("正") end
来源：http://eze.shanyushiyangkeji.top

[T39] Lua：模式匹配
来源：http://fmr.zhaomingkeji.xyz

string.find(s, "%d+")
来源：http://pxf.bjfxy.top

[T40] Lua：元表
来源：http://ymf.snrcjt.cn

setmetatable({}, { __index = base })
来源：http://yzr.fzhhl.top

[T41] Perl：Hello World
来源：http://drz.shuidangran.top

print "Hello\n";
来源：http://alo.vqdsnc.cn

[T42] Perl：变量类型
来源：http://ikm.c1oappe.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://zoc.shanyushiyangkeji.top

[T43] Perl：字符串插值
来源：http://nay.yvedp.cn

"值: $a"
来源：http://brc.vehdjk.com

[T44] Perl：条件
来源：http://xln.nanxuanxn.top

if ($a > 0) { print "正"; }
来源：http://mwq.ctjpmb.com

[T45] Perl：数组遍历
来源：http://unk.yj202588.top

for my $x (@arr) { print $x; }
来源：http://nbs.feifeiyinyue.top

[T46] Perl：哈希操作
来源：http://czy.jqgfzy.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://okc.c1oappe.top

[T47] Perl：正则捕获
来源：http://xtk.hesvh.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://ejy.jyoumei.cn

[T48] Perl：正则替换
来源：http://bch.shangyingyoupin.top

$s =~ s/old/new/g;
来源：http://wtg.sxryk.cn

[T49] Perl：函数
来源：http://tql.hongshengwenyu.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://byg.gaohongyu789.top

[T50] Perl：逐行读文件
来源：http://wff.xinyue.icu

open my $fh, "<", "a.txt" or die $!;
来源：http://fxu.yj202588.top

while (my $line = <$fh>) { print $line; }
来源：http://dgs.svipenyu.cn

[T51] Scala：Hello World
来源：http://upu.kuanghao11.cn

println("Hello")
来源：http://pqx.daxiang520.top

[T52] Scala：变量
来源：http://jsb.iojbl.cn

val a = 1;  var b = 2
来源：http://zrw.gogol.net.cn

[T53] Scala：字符串插值
来源：http://rin.yvedp.cn

s"值: $b"
来源：http://qkv.jinghuilouyu.cn

[T54] Scala：集合映射
来源：http://eec.zhoulong.xyz

List(1, 2, 3).map(_ * 2)
来源：http://yzv.gzhubu.top

[T55] Scala：集合过滤
来源：http://sti.ivvv.top

List(1, 2, 3).filter(_ > 1)
来源：http://fbl.epnwcf.com

[T56] Scala：样例类
来源：http://ris.sweek.top

case class User(name: String, age: Int)
来源：http://awa.yuanzhike.top

[T57] Scala：模式匹配
来源：http://ndt.xinyue.icu

x match { case 1 => "一"; case _ => "其他" }
来源：http://yqn.iojbl.cn

[T58] Scala：函数定义
来源：http://vpk.iojbl.cn

def add(a: Int, b: Int): Int = a + b
来源：http://swb.hesvh.cn

[T59] Scala：循环
来源：http://zxi.sufxvd.cn

for (i <- 1 to 10) println(i)
来源：http://ffs.316326.xyz

[T60] Scala：折叠
来源：http://tjl.sweek.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://had.jlsjyb.cn

================================================================================
来源：http://pzp.sxryk.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://rxc.jinqigfzy.top

================================================================================
来源：http://oif.fzhhl.top

[U01] Py：创建虚拟环境
来源：http://tub.jinqigfzy.top

python -m venv .venv && source .venv/bin/activate
来源：http://lju.zhongyouzk.top

[U02] Py：导出 / 安装依赖
来源：http://gdk.hesvh.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://zsg.yonumen.top

[U03] Py：加载 .env 配置
来源：http://riy.yuanzhike.top

from dotenv import load_dotenv; load_dotenv()
来源：http://mkj.bbcook.cn

[U04] Py：变量调试打印
来源：http://ujl.gaohongyu789.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://ckm.tianlin.xyz

[U05] Py：列表去重且保序
来源：http://kdd.ydzc1.top

list(dict.fromkeys(arr))
来源：http://dcr.c1oappe.top

[U06] Py：合并两个字典
来源：http://moo.hammf.cn

{**a, **b}
来源：http://fqv.xuanzx.com

[U07] Py：反转字典键值
来源：http://gjb.hywenlv.cn

{v: k for k, v in d.items()}
来源：http://tgc.cqqwz.cn

[U08] Py：展平二维列表
来源：http://mly.jinyuanbaomall.cn

[y for x in nested for y in x]
来源：http://jyu.tianlin.xyz

[U09] Py：字典取最大值的键
来源：http://hea.sufxvd.cn

max(d, key=d.get)
来源：http://oim.dashuyun.cn

[U10] Py：按值排序字典
来源：http://dun.uphjek.com

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://gxs.xuetiantiany.cn

[U11] Py：生成器表达式
来源：http://nzr.vehdjk.com

(x * 2 for x in arr)
来源：http://dnt.hywenlv.cn

[U12] Py：取出现最多的 3 个元素
来源：http://ybs.sjlbkw.cn

Counter(arr).most_common(3)
来源：http://cxr.uphjek.com

[U13] Py：固定长度队列
来源：http://jks.gaohongyu789.top

deque(maxlen=10)
来源：http://tss.zhijiandao.cn

[U14] Py：分组收集到列表
来源：http://mhb.iojbl.cn

defaultdict(list)
来源：http://pik.9152youxi.cn

[U15] Py：高精度计时
来源：http://eku.tian-w.cn

t = time.perf_counter()
来源：http://qbx.mhx1999.top

[U16] Py：命令行参数解析
来源：http://jbe.snrcjt.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://tzw.yongpay.top

[U17] Py：初始化日志
来源：http://czo.9152youxi.cn

logging.basicConfig(level=logging.INFO)
来源：http://bkp.shanyushiyangkeji.top

[U18] Py：预编译正则
来源：http://pqr.gogol.net.cn

pat = re.compile(r"\d+")
来源：http://sbb.ywan-chungtsiang.top

[U19] Py：正则替换带回调
来源：http://cgo.tian-w.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://zfy.chenzaomai.com

[U20] Py：缓存函数结果
来源：http://xjn.shuidangran.top

@functools.lru_cache(maxsize=None)
来源：http://dhm.jqgufenzy.top

[U21] Py：自定义上下文管理器
来源：http://xhn.hfpthk.cn

@contextlib.contextmanager
来源：http://qtv.pengpengdd.cyou

[U22] Py：矩阵转置
来源：http://xmu.yueranfly.top

list(zip(*m))
来源：http://rhp.yj20258888.top

[U23] Py：分块读取大文件
来源：http://enm.sweek.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://fdx.zhoulong.xyz

[U24] Py：路径操作
来源：http://oys.jlsjyb.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://fzh.hfpthk.cn

[U25] Py：CSV 按字典读
来源：http://qnc.zycfv.cn

csv.DictReader(f)
来源：http://xhh.dianchejie.cn

[U26] Py：并发下载
来源：http://cmz.epnwcf.com

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://mml.aibaodan.cn

[U27] Py：异步 HTTP
来源：http://rbv.zhijiandao.cn

aiohttp.ClientSession() 配合 async with
来源：http://sxc.chenjidiqi.icu

[U28] Py：类型别名
来源：http://qrf.hfpthk.cn

UserId = int
来源：http://uni.jinghuilouyu.cn

[U29] Py：属性校验
来源：http://gah.aizwys.cn

@property 与 @x.setter 配合
来源：http://oiy.hywenlv.cn

[U30] Py：数据类
来源：http://okj.tianlin.xyz

@dataclass(slots=True)
来源：http://lqe.yuxming.cn

[U31] Py：单测
来源：http://yxi.yj20258.top

python -m pytest -q
来源：http://ipn.bjfxy.top

[U32] Py：代码格式化
来源：http://mvt.fanxiaobao.xyz

ruff format . && ruff check --fix .
来源：http://rgs.zhongyouzk.top

[U33] Py：打包发布
来源：http://ken.daxiang520.top

python -m build  （依赖 pyproject.toml）
来源：http://nhe.xuanzx.com

[U34] Py：判断编码
来源：http://tee.hongshengwenyu.top

chardet.detect(raw)
来源：http://ieu.daria6918.cn

[U35] Py：发送邮件
来源：http://zqp.hfpthk.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://pmh.iojbl.cn

[U36] Py：定时任务
来源：http://jdg.chenzaomai.com

schedule.every(10).minutes.do(job)
来源：http://hsb.ydzc1.top

[U37] Py：读写 Excel
来源：http://yzz.hysaishi.cn

pandas.read_excel / DataFrame.to_excel
来源：http://inf.pengpengdd.cyou

[U38] Py：获取脚本所在目录
来源：http://iza.mhx1999.top

Path(__file__).resolve().parent
来源：http://psz.cucudq.cn

[U39] Py：判断是否在交互环境
来源：http://cng.bjfxy.top

sys.stdout.isatty()
来源：http://mup.hongshengwenyu.top

[U40] Py：打印到标准错误
来源：http://frr.gogol.net.cn

print("err", file=sys.stderr)
来源：http://dhx.shuidangran.top

[U41] PHP：初始化 Composer 项目
来源：http://uym.zhongyouzk.top

composer init;  composer require guzzlehttp/guzzle
来源：http://ljw.fengsongda.top

[U42] PHP：PSR-4 自动加载
来源：http://mcq.zhiwuduotai.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://tvr.yfazqb.com

[U43] PHP：声明命名空间
来源：http://nhb.hfpthk.cn

namespace App\Http;
来源：http://med.tarul.cn

[U44] PHP：开启严格类型
来源：http://lau.iojbl.cn

declare(strict_types=1);
来源：http://gkk.yj20258888.top

[U45] PHP：类型声明与返回类型
来源：http://kpy.jqgfzy.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://yge.wangdashe.top

[U46] PHP：可空类型
来源：http://alr.shanyushiyangtech.top

?string $name = null
来源：http://cbp.jinghuilouyu.cn

[U47] PHP：联合类型
来源：http://lsl.52xcode.cn

int|string $id
来源：http://nkh.iojbl.cn

[U48] PHP：纯枚举
来源：http://efe.zhengqikj.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://bgb.jinqigfzy.top

[U49] PHP：只读属性
来源：http://kmo.feifeiyinyue.top

public readonly string $name
来源：http://egm.feifeiyinyue.top

[U50] PHP：构造器属性提升
来源：http://jcu.yj20258.top

public function __construct(private int $id) {}
来源：http://cas.tian-w.cn

[U51] PHP：数组解构
来源：http://nin.pycfn.com

[$a, $b] = $arr;
来源：http://tqr.gogol.net.cn

[U52] PHP：箭头函数
来源：http://kvd.gogol.net.cn

$double = fn($x) => $x * 2;
来源：http://ymt.vehdjk.com

[U53] PHP：空合并运算符
来源：http://eqz.yvedp.cn

$v = $a ?? $b ?? "default";
来源：http://ccq.zhaomingkeji.xyz

[U54] PHP：空安全调用
来源：http://olq.zhengqikj.top

$obj?->method()
来源：http://uoc.aibaodan.cn

[U55] PHP：match 表达式
来源：http://isb.birdmap.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://quf.cqqwz.cn

[U56] PHP：命名参数
来源：http://kxt.iojbl.cn

f(a: 1, b: 2)
来源：http://vns.hnxiangtu.top

[U57] PHP：字符串插值
来源：http://cxu.fehbvm.com

"值: {$a}"
来源：http://yzn.wangdashe.top

[U58] PHP：数组三件套
来源：http://ojb.pengpengdd.cyou

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://gnd.snrcjt.cn


<!-- 参考信息 -->