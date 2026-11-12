代发 wailian999

[S33] C++：vector 增删
来源：http://hwp.jqgufenzy.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://xpn.daxiang520.top

[S34] C++：遍历 vector
来源：http://mnr.c1oappe.top

for (auto &x : v) { std::cout << x; }
来源：http://vdf.birdmap.top

[S35] C++：map
来源：http://nyp.jinqigufen.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://tdd.gaohongyu789.top

[S36] C++：unordered_map
来源：http://vsu.hcnkem.com

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://fkr.hfpthk.cn

[S37] C++：set
来源：http://luz.smart0.xyz

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://woy.yangfankeji.com

[S38] C++：排序
来源：http://mtg.jqgfzy.top

std::sort(v.begin(), v.end());
来源：http://wcr.fktsv.cn

[S39] C++：自定义比较器排序
来源：http://kqf.shangyingyoupin.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://vhd.jqgufenzy.top

[S40] C++：查找元素
来源：http://wtf.zdbjq.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://lkx.cdnleiting.top

[S41] C++：类与构造函数
来源：http://fgj.daria6918.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://iji.0kj1m.cn

[S42] C++：继承与虚函数
来源：http://cor.chenzaomai.com

class B : public Base { public: void f() override {} };
来源：http://oup.hfpthk.cn

[S43] C++：智能指针
来源：http://bks.gotoacloud.top

auto p = std::make_unique<int>(5);
来源：http://gqq.daxiang520.top

[S44] C++：引用传参
来源：http://nxi.jqgufenzy.top

void inc(int &x) { ++x; }
来源：http://hnr.jinyuanbaomall.cn

[S45] C++：lambda
来源：http://qtd.tanke756.top

auto add = [](int a, int b) { return a + b; };
来源：http://wil.daria6918.cn

[S46] C++：函数模板
来源：http://smo.9152youxi.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://vpx.316326.xyz

[S47] C++：结构化绑定遍历
来源：http://whf.sxryk.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://lzd.cashguo.top

[S48] C++：逐行读文件
来源：http://slg.yueranfly.top

std::ifstream in("a.txt");  std::string line;
来源：http://jqb.sufxvd.cn

while (std::getline(in, line)) { }
来源：http://wmc.yuxming.cn

[S49] C++：写文件
来源：http://mhx.ivvv.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://gsb.dianchejie.cn

[S50] C++：格式化数字
来源：http://ngf.ivvv.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://foc.wangdashe.top

[S51] C++：显式类型转换
来源：http://gfh.gogol.net.cn

static_cast<double>(a) / b
来源：http://syv.zhijiandao.cn

[S52] C++：const 与 noexcept
来源：http://zlm.ybcxt.top

int size() const noexcept { return n_; }
来源：http://kex.jiagoushi.top

[S53] C++：移动语义
来源：http://efq.jinyuanbaomall.cn

std::vector<int> w = std::move(v);
来源：http://aab.shuidangran.top

[S54] C++：异常处理
来源：http://lcv.hongshengwenyu.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://jev.wangdashe.top

[S55] C++：结构化绑定
来源：http://cfh.jqgfzy.top

auto [a, b] = std::make_pair(1, 2);
来源：http://owg.jinqigufen.top

[S56] C++：optional
来源：http://ypk.andypj.xyz

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://qgl.tarul.cn

[S57] C++：编译期常量
来源：http://alv.wangshuangyany.cn

constexpr int N = 10;
来源：http://yvg.aizwys.cn

[S58] C++：命名空间
来源：http://kbp.jinqigfzy.top

namespace ns { int f() { return 1; } }
来源：http://ypg.ydzc1.top

[S59] C++：静态断言
来源：http://xts.shzxlz.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://tlt.haohaochexian.top

[S60] C++：遍历并删除元素
来源：http://brl.shangyingyoupin.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://bac.52xcode.cn

================================================================================
来源：http://hdb.hammf.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://kmx.sxryk.cn

================================================================================
来源：http://hqc.hfpthk.cn

[T01] Kotlin：Hello World
来源：http://bev.xuetiantiany.cn

println("Hello")
来源：http://fei.chenjidiqi.icu

[T02] Kotlin：变量
来源：http://noy.c1oappe.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://yqp.vehdjk.com

[T03] Kotlin：字符串模板
来源：http://dpx.hfpthk.cn

"值: $b"
来源：http://hii.yvedp.cn

[T04] Kotlin：空安全
来源：http://ksh.jqgfzy.top

val n: String? = null;  n?.length
来源：http://zcc.svipenyu.cn

[T05] Kotlin：when 表达式
来源：http://jcx.yuxming.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hqg.jlsjyb.cn

[T06] Kotlin：集合映射
来源：http://yvo.daria6918.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://qjt.ehwqpu.com

[T07] Kotlin：集合过滤
来源：http://nhh.daria6918.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://upy.pengpengdd.cyou

[T08] Kotlin：数据类
来源：http://wjy.jinyuanbaomall.cn

data class User(val name: String, val age: Int)
来源：http://dja.xuetiantiany.cn

[T09] Kotlin：扩展函数
来源：http://rae.kuanghao11.cn

fun String.exclaim() = this + "!"
来源：http://sjl.shanyushiyangtech.top

[T10] Kotlin：默认参数
来源：http://ftb.xuanzx.com

fun greet(name: String = "World") = "Hi $name"
来源：http://xjv.fktsv.cn

[T11] Kotlin：协程
来源：http://oax.zhoulong.xyz

GlobalScope.launch { delay(1000); println("done") }
来源：http://vux.zdbjq.cn

[T12] Kotlin：解构声明
来源：http://pct.zdbjq.cn

val (a, b) = Pair(1, 2)
来源：http://nbv.ydjk.org.cn

[T13] Kotlin：只读 Map
来源：http://bkj.ppjwa.cn

val m = mapOf("a" to 1)
来源：http://lzt.guowangkeji.top

[T14] Kotlin：循环
来源：http://xnn.shuidangran.top

for (i in 1..10) println(i)
来源：http://oio.zhiwuduotai.top

[T15] Kotlin：接口
来源：http://quc.nanxuanxn.top

interface Shape { fun area(): Double }
来源：http://nvz.ydzc1.top

[T16] Swift：Hello World
来源：http://efl.gaohongyu789.top

print("Hello")
来源：http://vnr.tanke756.top

[T17] Swift：变量与常量
来源：http://jrn.hongshengwenyu.top

var a = 1;  let b = 2
来源：http://dua.shzxlz.cn

[T18] Swift：字符串插值
来源：http://pdl.316326.xyz

"值: \(b)"
来源：http://adp.ydzc1.top

[T19] Swift：可选绑定
来源：http://gzi.gotoacloud.top

if let n = opt { print(n) }
来源：http://lxi.ywan-chungtsiang.top

[T20] Swift：数组操作
来源：http://kvr.xingfuxueyuan.xyz

var a = [1, 2, 3];  a.append(4)
来源：http://dfu.zhaomingkeji.xyz

[T21] Swift：遍历
来源：http://wqp.jinqigfzy.top

for x in a { print(x) }
来源：http://xmq.ydzc1.top

[T22] Swift：字典
来源：http://yuw.gogol.net.cn

var d = ["a": 1];  d["b"] = 2
来源：http://jbc.dashuyun.cn

[T23] Swift：函数
来源：http://osw.zhongyouzk.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://vcm.hammf.cn

[T24] Swift：闭包
来源：http://pcf.xinyue.icu

let f = { (x: Int) -> Int in x * 2 }
来源：http://zto.sjlbkw.cn

[T25] Swift：结构体
来源：http://tju.wangdashe.top

struct P { var x: Int }
来源：http://avm.hnqzz.top

[T26] Swift：类与重写
来源：http://upo.hongshengwenyu.top

class A: Base { override func f() {} }
来源：http://pbr.sweek.top

[T27] Swift：错误处理
来源：http://que.guowangkeji.top

do { try f() } catch { print(error) }
来源：http://uvt.guowangkeji.top

[T28] Swift：枚举
来源：http://ogb.svipenyu.cn

enum Color { case red, green }
来源：http://zjv.zdbjq.cn

[T29] Swift：guard 提前返回
来源：http://ppl.yangfankeji.com

guard let x = opt else { return }
来源：http://shs.ydzc1.top

[T30] Swift：协议
来源：http://gka.shangyingyoupin.top

protocol Shape { func area() -> Double }
来源：http://nad.sjlbkw.cn

[T31] Lua：Hello World
来源：http://kfj.gaohongyu789.top

print("Hello")
来源：http://dza.hongshengwenyu.top

[T32] Lua：局部变量
来源：http://dks.nanxinkj.top

local a = 1
来源：http://kqg.aizwys.cn

[T33] Lua：表（数组）
来源：http://xyc.pengpengdd.cyou

local t = {1, 2, 3};  t[4] = 4
来源：http://prn.zhixingplan.top

[T34] Lua：遍历表
来源：http://eec.vehdjk.com

for i, v in ipairs(t) do print(i, v) end
来源：http://rnm.bjfxy.top

[T35] Lua：字典表
来源：http://cyk.ydzc1.top

local d = { a = 1 };  d.b = 2
来源：http://quh.haohaochexian.top

[T36] Lua：函数
来源：http://iov.sjlbkw.cn

function add(a, b) return a + b end
来源：http://mdy.feifeiyinyue.top

[T37] Lua：字符串拼接
来源：http://rlo.yongpay.top

"a" .. "b"
来源：http://nkx.hnxiangtu.top

[T38] Lua：条件
来源：http://qgg.chenjidiqi.icu

if x > 0 then print("正") end
来源：http://ypi.hongshengwenyu.top

[T39] Lua：模式匹配
来源：http://tjb.gaohongyu789.top

string.find(s, "%d+")
来源：http://aoc.vqdsnc.cn

[T40] Lua：元表
来源：http://yje.guannengcc.top

setmetatable({}, { __index = base })
来源：http://yyj.yj20258888.top

[T41] Perl：Hello World
来源：http://yer.yj202588.top

print "Hello\n";
来源：http://ucw.9152youxi.cn

[T42] Perl：变量类型
来源：http://qin.cheryme.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://pgo.ivvv.top

[T43] Perl：字符串插值
来源：http://pkv.xylfe.cn

"值: $a"
来源：http://lio.aibaodan.cn

[T44] Perl：条件
来源：http://srk.nanxuanxn.top

if ($a > 0) { print "正"; }
来源：http://ejr.yfazqb.com

[T45] Perl：数组遍历
来源：http://fps.jinyuanbaomall.cn

for my $x (@arr) { print $x; }
来源：http://aui.9152youxi.cn

[T46] Perl：哈希操作
来源：http://krb.shanyushiyangtech.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://gpv.gzhubu.top

[T47] Perl：正则捕获
来源：http://avc.yfazqb.com

if ($s =~ /(\d+)/) { print $1; }
来源：http://vqa.shanyushiyangkeji.top

[T48] Perl：正则替换
来源：http://eth.svipenyu.cn

$s =~ s/old/new/g;
来源：http://pix.dashuyun.cn

[T49] Perl：函数
来源：http://dzc.andypj.xyz

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://mrf.aibaodan.cn

[T50] Perl：逐行读文件
来源：http://krs.svipenyu.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://yid.shangyingyoupin.top

while (my $line = <$fh>) { print $line; }
来源：http://fgk.snrcjt.cn

[T51] Scala：Hello World
来源：http://lie.vehdjk.com

println("Hello")
来源：http://jas.pengpengdd.cyou

[T52] Scala：变量
来源：http://ybs.aizwys.cn

val a = 1;  var b = 2
来源：http://ppw.yvedp.cn

[T53] Scala：字符串插值
来源：http://zzg.havefunace.top

s"值: $b"
来源：http://dkc.tanke756.top

[T54] Scala：集合映射
来源：http://fal.andypj.xyz

List(1, 2, 3).map(_ * 2)
来源：http://zvi.cashguo.top

[T55] Scala：集合过滤
来源：http://zyx.ydzc1.top

List(1, 2, 3).filter(_ > 1)
来源：http://zso.sxryk.cn

[T56] Scala：样例类
来源：http://ext.snrcjt.cn

case class User(name: String, age: Int)
来源：http://zup.ivvv.top

[T57] Scala：模式匹配
来源：http://ydm.cucudq.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://cnr.hongshengwenyu.top

[T58] Scala：函数定义
来源：http://khs.yuanzhike.top

def add(a: Int, b: Int): Int = a + b
来源：http://vnc.gaohongyu789.top

[T59] Scala：循环
来源：http://dvb.chenlongwang.top

for (i <- 1 to 10) println(i)
来源：http://sjp.fzhhl.top

[T60] Scala：折叠
来源：http://onr.fktsv.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://xxe.zdqjudy.top

================================================================================
来源：http://axo.tianlin.xyz

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://rmb.yangfankeji.com

================================================================================
来源：http://vxj.jinyuanbaomall.cn

[U01] Py：创建虚拟环境
来源：http://fjh.zhoulong.xyz

python -m venv .venv && source .venv/bin/activate
来源：http://cuo.nwbrower.top

[U02] Py：导出 / 安装依赖
来源：http://nnz.ywan-chungtsiang.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://gck.nanxuanxn.top

[U03] Py：加载 .env 配置
来源：http://rqv.jinghuilouyu.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://nir.svipenyu.cn

[U04] Py：变量调试打印
来源：http://utk.fzhhl.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://ihe.zdbjq.cn

[U05] Py：列表去重且保序
来源：http://zgz.quarkkingdee.top

list(dict.fromkeys(arr))
来源：http://keo.yuxming.cn

[U06] Py：合并两个字典
来源：http://pet.fzhhl.top

{**a, **b}
来源：http://wpf.dashuyun.cn

[U07] Py：反转字典键值
来源：http://bco.jqgufenzy.top

{v: k for k, v in d.items()}
来源：http://zvl.nanxuanxn.top

[U08] Py：展平二维列表
来源：http://hbq.yanxiufei.cn

[y for x in nested for y in x]
来源：http://znw.xuetiantiany.cn

[U09] Py：字典取最大值的键
来源：http://qey.sjlbkw.cn

max(d, key=d.get)
来源：http://fcp.jyoumei.cn

[U10] Py：按值排序字典
来源：http://pdr.shzxlz.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://zts.gotoacloud.top

[U11] Py：生成器表达式
来源：http://wcg.snrcjt.cn

(x * 2 for x in arr)
来源：http://eze.smart0.xyz

[U12] Py：取出现最多的 3 个元素
来源：http://lkf.pengpengdd.cyou

Counter(arr).most_common(3)
来源：http://vwz.fehbvm.com

[U13] Py：固定长度队列
来源：http://uxx.ydjk.org.cn

deque(maxlen=10)
来源：http://wpt.pycfn.com

[U14] Py：分组收集到列表
来源：http://rdo.wangdashe.top

defaultdict(list)
来源：http://tlt.gogol.net.cn

[U15] Py：高精度计时
来源：http://zzh.feifeiyinyue.top

t = time.perf_counter()
来源：http://unw.hongshengwenyu.top

[U16] Py：命令行参数解析
来源：http://qfp.hnqzz.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://dcr.c1oappe.top

[U17] Py：初始化日志
来源：http://wue.jiagoushi.top

logging.basicConfig(level=logging.INFO)
来源：http://wlc.iojbl.cn

[U18] Py：预编译正则
来源：http://xye.ctjpmb.com

pat = re.compile(r"\d+")
来源：http://ohj.chenlongwang.top

[U19] Py：正则替换带回调
来源：http://tkp.xuetiantiany.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://pjy.yj20258888.top

[U20] Py：缓存函数结果
来源：http://jhi.vehdjk.com

@functools.lru_cache(maxsize=None)
来源：http://ntd.yj202588.top

[U21] Py：自定义上下文管理器
来源：http://gjy.hfpthk.cn

@contextlib.contextmanager
来源：http://thy.hongshengwenyu.top

[U22] Py：矩阵转置
来源：http://eug.dianchejie.cn

list(zip(*m))
来源：http://dpc.tarul.cn

[U23] Py：分块读取大文件
来源：http://zsr.tanke756.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://lgd.ivvv.top

[U24] Py：路径操作
来源：http://vjk.chenjidiqi.icu

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://uoq.uphjek.com

[U25] Py：CSV 按字典读
来源：http://gld.daria6918.cn

csv.DictReader(f)
来源：http://xas.feifeiyinyue.top

[U26] Py：并发下载
来源：http://lzg.wangdashe.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://phs.aizwys.cn

[U27] Py：异步 HTTP
来源：http://nnx.cdnleiting.top

aiohttp.ClientSession() 配合 async with
来源：http://yea.uphjek.com

[U28] Py：类型别名
来源：http://qzg.yueranfly.top

UserId = int
来源：http://czt.guannengcc.top

[U29] Py：属性校验
来源：http://mcg.jinqigfzy.top

@property 与 @x.setter 配合
来源：http://cws.shuidangran.top

[U30] Py：数据类
来源：http://dux.fanxiaobao.xyz

@dataclass(slots=True)
来源：http://esp.yvedp.cn

[U31] Py：单测
来源：http://ynr.yj20258888.top

python -m pytest -q
来源：http://mjn.zhixingplan.top

[U32] Py：代码格式化
来源：http://ifx.zycfv.cn

ruff format . && ruff check --fix .
来源：http://vqr.chenjidiqi.icu

[U33] Py：打包发布
来源：http://ulk.jyoumei.cn

python -m build  （依赖 pyproject.toml）
来源：http://glp.yj202588.top

[U34] Py：判断编码
来源：http://bsx.yvedp.cn

chardet.detect(raw)
来源：http://lex.chenzaomai.com

[U35] Py：发送邮件
来源：http://umr.nanxinkj.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://ciu.jinqigufen.top

[U36] Py：定时任务
来源：http://rhy.9152youxi.cn

schedule.every(10).minutes.do(job)
来源：http://sgu.bbcook.cn

[U37] Py：读写 Excel
来源：http://mpw.xingfuxueyuan.xyz

pandas.read_excel / DataFrame.to_excel
来源：http://pdm.ydjk.org.cn

[U38] Py：获取脚本所在目录
来源：http://qko.pengpengdd.cyou

Path(__file__).resolve().parent
来源：http://ncn.jinghuilouyu.cn

[U39] Py：判断是否在交互环境
来源：http://sap.cucudq.cn

sys.stdout.isatty()
来源：http://wpl.zhoulong.xyz

[U40] Py：打印到标准错误
来源：http://aha.52xcode.cn

print("err", file=sys.stderr)
来源：http://wdj.xziqi.cn

[U41] PHP：初始化 Composer 项目
来源：http://lcj.xylfe.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://vns.zhaomingkeji.xyz

[U42] PHP：PSR-4 自动加载
来源：http://gcv.xinyue.icu

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://rhe.guowangkeji.top

[U43] PHP：声明命名空间
来源：http://zdq.tarul.cn

namespace App\Http;
来源：http://kit.jinqigfzy.top

[U44] PHP：开启严格类型
来源：http://weq.andypj.xyz

declare(strict_types=1);
来源：http://ikd.jiagoushi.top

[U45] PHP：类型声明与返回类型
来源：http://bxo.yvedp.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://xrc.bbcook.cn

[U46] PHP：可空类型
来源：http://qhe.zdbjq.cn

?string $name = null
来源：http://urk.jiagoushi.top

[U47] PHP：联合类型
来源：http://jud.shanyushiyangtech.top

int|string $id
来源：http://tzg.zhengqikj.top

[U48] PHP：纯枚举
来源：http://ist.gaohongyu789.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://sab.fanxiaobao.xyz

[U49] PHP：只读属性
来源：http://yez.bbcook.cn

public readonly string $name
来源：http://ojf.ybcxt.top

[U50] PHP：构造器属性提升
来源：http://pqa.nwbrower.top

public function __construct(private int $id) {}
来源：http://onm.shuidangran.top

[U51] PHP：数组解构
来源：http://gzn.hammf.cn

[$a, $b] = $arr;
来源：http://ipj.jiagoushi.top

[U52] PHP：箭头函数
来源：http://wpi.xuanzx.com

$double = fn($x) => $x * 2;
来源：http://xaz.yj20258.top

[U53] PHP：空合并运算符
来源：http://waq.aizwys.cn

$v = $a ?? $b ?? "default";
来源：http://oed.nanxuanxn.top

[U54] PHP：空安全调用
来源：http://jxy.ivvv.top

$obj?->method()
来源：http://lxb.cucudq.cn

[U55] PHP：match 表达式
来源：http://rxs.xuanzx.com

$s = match($x) { 1 => "一", default => "其他" };
来源：http://tkl.cqqwz.cn

[U56] PHP：命名参数
来源：http://rwy.zycfv.cn

f(a: 1, b: 2)
来源：http://svy.tian-w.cn

[U57] PHP：字符串插值
来源：http://brl.yvedp.cn

"值: {$a}"
来源：http://wxf.guannengcc.top

[U58] PHP：数组三件套
来源：http://zux.feifeiyinyue.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://mjo.vehdjk.com


<!-- 参考信息 -->