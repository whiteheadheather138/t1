代发 wailian999

[S47] C++：结构化绑定遍历
来源：http://vzj.xuetiantiany.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://ujg.yfazqb.com

[S48] C++：逐行读文件
来源：http://gqn.cdnleiting.top

std::ifstream in("a.txt");  std::string line;
来源：http://qss.snrcjt.cn

while (std::getline(in, line)) { }
来源：http://lhw.havefunace.top

[S49] C++：写文件
来源：http://dxw.yangfankeji.com

std::ofstream out("a.txt");  out << "hi\n";
来源：http://ofq.cdnleiting.top

[S50] C++：格式化数字
来源：http://rtb.vehdjk.com

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://utn.cashguo.top

[S51] C++：显式类型转换
来源：http://pec.daria6918.cn

static_cast<double>(a) / b
来源：http://oxw.tarul.cn

[S52] C++：const 与 noexcept
来源：http://emw.meibo888.top

int size() const noexcept { return n_; }
来源：http://cdb.jlsjyb.cn

[S53] C++：移动语义
来源：http://mmi.tarul.cn

std::vector<int> w = std::move(v);
来源：http://dpx.jyoumei.cn

[S54] C++：异常处理
来源：http://lix.zhoulong.xyz

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://zry.jinyuanbaomall.cn

[S55] C++：结构化绑定
来源：http://ijp.jiagoushi.top

auto [a, b] = std::make_pair(1, 2);
来源：http://kno.hysaishi.cn

[S56] C++：optional
来源：http://wmx.hywenlv.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://dfp.xuanzx.com

[S57] C++：编译期常量
来源：http://cvs.quarkkingdee.top

constexpr int N = 10;
来源：http://aam.nanxinkj.top

[S58] C++：命名空间
来源：http://lam.gogol.net.cn

namespace ns { int f() { return 1; } }
来源：http://dnt.jinghuilouyu.cn

[S59] C++：静态断言
来源：http://omj.guannengcc.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://oqu.52xcode.cn

[S60] C++：遍历并删除元素
来源：http://jdf.daxiang520.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://mfb.yueranfly.top

================================================================================
来源：http://orf.tianlin.xyz

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://teb.yonumen.top

================================================================================
来源：http://oka.fengsongda.top

[T01] Kotlin：Hello World
来源：http://vyh.nwbrower.top

println("Hello")
来源：http://gqp.ydzc1.top

[T02] Kotlin：变量
来源：http://xcy.zhijiandao.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://shg.guannengcc.top

[T03] Kotlin：字符串模板
来源：http://bpw.daxiang520.top

"值: $b"
来源：http://cdq.haohaochexian.top

[T04] Kotlin：空安全
来源：http://wyf.wangdashe.top

val n: String? = null;  n?.length
来源：http://vtj.yj20258888.top

[T05] Kotlin：when 表达式
来源：http://jom.tianlin.xyz

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://znb.xuanzx.com

[T06] Kotlin：集合映射
来源：http://cog.yanxiufei.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://lic.jinqigfzy.top

[T07] Kotlin：集合过滤
来源：http://ncy.zdbjq.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://rkv.yuxming.cn

[T08] Kotlin：数据类
来源：http://xtt.guowangkeji.top

data class User(val name: String, val age: Int)
来源：http://dho.shzxlz.cn

[T09] Kotlin：扩展函数
来源：http://xen.nanxinkj.top

fun String.exclaim() = this + "!"
来源：http://znn.sweek.top

[T10] Kotlin：默认参数
来源：http://ffq.hnqzz.top

fun greet(name: String = "World") = "Hi $name"
来源：http://ghr.ctjpmb.com

[T11] Kotlin：协程
来源：http://vwp.nwbrower.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://frn.cqqwz.cn

[T12] Kotlin：解构声明
来源：http://jdh.svipenyu.cn

val (a, b) = Pair(1, 2)
来源：http://ucr.sjlbkw.cn

[T13] Kotlin：只读 Map
来源：http://sfj.fehbvm.com

val m = mapOf("a" to 1)
来源：http://zqr.pycfn.com

[T14] Kotlin：循环
来源：http://jmg.jianghu66.top

for (i in 1..10) println(i)
来源：http://eem.gzhubu.top

[T15] Kotlin：接口
来源：http://eel.xziqi.cn

interface Shape { fun area(): Double }
来源：http://pps.sjlbkw.cn

[T16] Swift：Hello World
来源：http://dja.yonumen.top

print("Hello")
来源：http://vbj.aizwys.cn

[T17] Swift：变量与常量
来源：http://hds.yanxiufei.cn

var a = 1;  let b = 2
来源：http://amj.gzhubu.top

[T18] Swift：字符串插值
来源：http://myg.sweek.top

"值: \(b)"
来源：http://rwu.hammf.cn

[T19] Swift：可选绑定
来源：http://cjn.fanxiaobao.xyz

if let n = opt { print(n) }
来源：http://spv.9152youxi.cn

[T20] Swift：数组操作
来源：http://hgx.tarul.cn

var a = [1, 2, 3];  a.append(4)
来源：http://adl.fktsv.cn

[T21] Swift：遍历
来源：http://qyp.cheryme.top

for x in a { print(x) }
来源：http://jvc.yvedp.cn

[T22] Swift：字典
来源：http://nqs.sjlbkw.cn

var d = ["a": 1];  d["b"] = 2
来源：http://ygt.ywan-chungtsiang.top

[T23] Swift：函数
来源：http://rzb.zhixingplan.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://gjq.jiagoushi.top

[T24] Swift：闭包
来源：http://ken.hesvh.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://oky.wangshuangyany.cn

[T25] Swift：结构体
来源：http://sls.9152youxi.cn

struct P { var x: Int }
来源：http://ztv.yj20258888.top

[T26] Swift：类与重写
来源：http://oap.haohaochexian.top

class A: Base { override func f() {} }
来源：http://nwd.yanxiufei.cn

[T27] Swift：错误处理
来源：http://pbl.daria6918.cn

do { try f() } catch { print(error) }
来源：http://qis.guannengcc.top

[T28] Swift：枚举
来源：http://jmo.daxiang520.top

enum Color { case red, green }
来源：http://usf.aibaodan.cn

[T29] Swift：guard 提前返回
来源：http://rvx.cashguo.top

guard let x = opt else { return }
来源：http://ozo.shuidangran.top

[T30] Swift：协议
来源：http://fni.xuetiantiany.cn

protocol Shape { func area() -> Double }
来源：http://xhr.svipenyu.cn

[T31] Lua：Hello World
来源：http://sxr.cqqwz.cn

print("Hello")
来源：http://yuk.ywan-chungtsiang.top

[T32] Lua：局部变量
来源：http://stx.ywan-chungtsiang.top

local a = 1
来源：http://ixc.9152youxi.cn

[T33] Lua：表（数组）
来源：http://jwf.yuxming.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://wjw.kuanghao11.cn

[T34] Lua：遍历表
来源：http://aez.daria6918.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://qad.52xcode.cn

[T35] Lua：字典表
来源：http://chh.tian-w.cn

local d = { a = 1 };  d.b = 2
来源：http://ofw.fengsongda.top

[T36] Lua：函数
来源：http://phj.birdmap.top

function add(a, b) return a + b end
来源：http://whe.bjfxy.top

[T37] Lua：字符串拼接
来源：http://bxy.xuetiantiany.cn

"a" .. "b"
来源：http://nnm.ivvv.top

[T38] Lua：条件
来源：http://jeu.hongshengwenyu.top

if x > 0 then print("正") end
来源：http://lnz.yvedp.cn

[T39] Lua：模式匹配
来源：http://dbb.zhongyouzk.top

string.find(s, "%d+")
来源：http://iyz.zhengqikj.top

[T40] Lua：元表
来源：http://ezx.cucudq.cn

setmetatable({}, { __index = base })
来源：http://ldf.ydjk.org.cn

[T41] Perl：Hello World
来源：http://rrb.yonumen.top

print "Hello\n";
来源：http://fgu.hcnkem.com

[T42] Perl：变量类型
来源：http://kmr.cashguo.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://rba.nwbrower.top

[T43] Perl：字符串插值
来源：http://lru.hesvh.cn

"值: $a"
来源：http://kbg.ehwqpu.com

[T44] Perl：条件
来源：http://jcu.chenjidiqi.icu

if ($a > 0) { print "正"; }
来源：http://sjk.zhongyouzk.top

[T45] Perl：数组遍历
来源：http://jmk.yj20258.top

for my $x (@arr) { print $x; }
来源：http://glg.tanke756.top

[T46] Perl：哈希操作
来源：http://jsc.shangyingyoupin.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://vss.yvedp.cn

[T47] Perl：正则捕获
来源：http://qeo.yongpay.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://npx.xinyue.icu

[T48] Perl：正则替换
来源：http://wbr.yangfankeji.com

$s =~ s/old/new/g;
来源：http://awg.ybcxt.top

[T49] Perl：函数
来源：http://xbr.bbcook.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hdh.gotoacloud.top

[T50] Perl：逐行读文件
来源：http://fcq.jlsjyb.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://wwd.hnqzz.top

while (my $line = <$fh>) { print $line; }
来源：http://swx.sjlbkw.cn

[T51] Scala：Hello World
来源：http://hoo.tarul.cn

println("Hello")
来源：http://vpj.ctjpmb.com

[T52] Scala：变量
来源：http://dtx.iojbl.cn

val a = 1;  var b = 2
来源：http://nle.zhaomingkeji.xyz

[T53] Scala：字符串插值
来源：http://yjz.0kj1m.cn

s"值: $b"
来源：http://nmx.hysaishi.cn

[T54] Scala：集合映射
来源：http://nxa.sweek.top

List(1, 2, 3).map(_ * 2)
来源：http://sjd.aibaodan.cn

[T55] Scala：集合过滤
来源：http://oke.xinyue.icu

List(1, 2, 3).filter(_ > 1)
来源：http://uni.epnwcf.com

[T56] Scala：样例类
来源：http://qgr.chenzaomai.com

case class User(name: String, age: Int)
来源：http://ppf.gaohongyu789.top

[T57] Scala：模式匹配
来源：http://ybk.yuanzhike.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://rik.cheryme.top

[T58] Scala：函数定义
来源：http://coo.hammf.cn

def add(a: Int, b: Int): Int = a + b
来源：http://jbz.zhongyouzk.top

[T59] Scala：循环
来源：http://bct.jlsjyb.cn

for (i <- 1 to 10) println(i)
来源：http://cco.zhiwuduotai.top

[T60] Scala：折叠
来源：http://qxc.tianlin.xyz

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://ogy.tanke756.top

================================================================================
来源：http://hoe.tianlin.xyz

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://qvw.xingfuxueyuan.xyz

================================================================================
来源：http://gaj.svipenyu.cn

[U01] Py：创建虚拟环境
来源：http://fyz.hongshengwenyu.top

python -m venv .venv && source .venv/bin/activate
来源：http://zwn.zhoulong.xyz

[U02] Py：导出 / 安装依赖
来源：http://ohh.9152youxi.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://civ.aibaodan.cn

[U03] Py：加载 .env 配置
来源：http://yoy.yangfankeji.com

from dotenv import load_dotenv; load_dotenv()
来源：http://vsv.cucudq.cn

[U04] Py：变量调试打印
来源：http://zij.ivvv.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://lcd.gzhubu.top

[U05] Py：列表去重且保序
来源：http://nln.vehdjk.com

list(dict.fromkeys(arr))
来源：http://sjr.ctjpmb.com

[U06] Py：合并两个字典
来源：http://sjo.xylfe.cn

{**a, **b}
来源：http://btm.jinghuilouyu.cn

[U07] Py：反转字典键值
来源：http://fnt.gotoacloud.top

{v: k for k, v in d.items()}
来源：http://yvg.tianlin.xyz

[U08] Py：展平二维列表
来源：http://yud.hywenlv.cn

[y for x in nested for y in x]
来源：http://lmt.hcnkem.com

[U09] Py：字典取最大值的键
来源：http://plt.9152youxi.cn

max(d, key=d.get)
来源：http://bot.zdbjq.cn

[U10] Py：按值排序字典
来源：http://sim.sysykeji.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://yqa.quarkkingdee.top

[U11] Py：生成器表达式
来源：http://shd.9152youxi.cn

(x * 2 for x in arr)
来源：http://zaz.redwolf501.top

[U12] Py：取出现最多的 3 个元素
来源：http://bxm.chenlongwang.top

Counter(arr).most_common(3)
来源：http://otl.sysykeji.top

[U13] Py：固定长度队列
来源：http://fjw.fzhhl.top

deque(maxlen=10)
来源：http://pue.iojbl.cn

[U14] Py：分组收集到列表
来源：http://mds.sufxvd.cn

defaultdict(list)
来源：http://feu.iojbl.cn

[U15] Py：高精度计时
来源：http://zsh.jiagoushi.top

t = time.perf_counter()
来源：http://dwv.cheryme.top

[U16] Py：命令行参数解析
来源：http://slj.jyoumei.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://xxx.shanyushiyangkeji.top

[U17] Py：初始化日志
来源：http://mya.ybcxt.top

logging.basicConfig(level=logging.INFO)
来源：http://qet.zhaomingkeji.xyz

[U18] Py：预编译正则
来源：http://srd.jinghuilouyu.cn

pat = re.compile(r"\d+")
来源：http://ian.0kj1m.cn

[U19] Py：正则替换带回调
来源：http://ruc.birdmap.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://sjm.jinyuanbaomall.cn

[U20] Py：缓存函数结果
来源：http://qxz.cqqwz.cn

@functools.lru_cache(maxsize=None)
来源：http://vdd.dianchejie.cn

[U21] Py：自定义上下文管理器
来源：http://ysc.chenlongwang.top

@contextlib.contextmanager
来源：http://lqb.xuanzx.com

[U22] Py：矩阵转置
来源：http://qeh.cqqwz.cn

list(zip(*m))
来源：http://xqe.c1oappe.top

[U23] Py：分块读取大文件
来源：http://oni.ehwqpu.com

for chunk in iter(lambda: f.read(8192), b""):
来源：http://rve.zhengqikj.top

[U24] Py：路径操作
来源：http://osw.sxryk.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://bqe.chenlongwang.top

[U25] Py：CSV 按字典读
来源：http://mnb.nanxinkj.top

csv.DictReader(f)
来源：http://xjr.wangdashe.top

[U26] Py：并发下载
来源：http://lsb.sysykeji.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://utw.jinyuanbaomall.cn

[U27] Py：异步 HTTP
来源：http://ncb.yj20258888.top

aiohttp.ClientSession() 配合 async with
来源：http://fry.hysaishi.cn

[U28] Py：类型别名
来源：http://crq.jqgufenzy.top

UserId = int
来源：http://wgj.sweek.top

[U29] Py：属性校验
来源：http://kjq.xinyue.icu

@property 与 @x.setter 配合
来源：http://uhf.kuanghao11.cn

[U30] Py：数据类
来源：http://udo.bjfxy.top

@dataclass(slots=True)
来源：http://kvm.uphjek.com

[U31] Py：单测
来源：http://esj.zhijiandao.cn

python -m pytest -q
来源：http://pre.nanxinkj.top

[U32] Py：代码格式化
来源：http://gfo.daxiang520.top

ruff format . && ruff check --fix .
来源：http://ati.fktsv.cn

[U33] Py：打包发布
来源：http://bge.snrcjt.cn

python -m build  （依赖 pyproject.toml）
来源：http://fvl.zhiwuduotai.top

[U34] Py：判断编码
来源：http://atc.cqqwz.cn

chardet.detect(raw)
来源：http://dzv.sufxvd.cn

[U35] Py：发送邮件
来源：http://kos.zdbjq.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://ysc.zdbjq.cn

[U36] Py：定时任务
来源：http://rew.shuidangran.top

schedule.every(10).minutes.do(job)
来源：http://yau.hcnkem.com

[U37] Py：读写 Excel
来源：http://qcn.gogol.net.cn

pandas.read_excel / DataFrame.to_excel
来源：http://ysz.yj202588.top

[U38] Py：获取脚本所在目录
来源：http://uyr.hywenlv.cn

Path(__file__).resolve().parent
来源：http://mih.cashguo.top

[U39] Py：判断是否在交互环境
来源：http://oha.smart0.xyz

sys.stdout.isatty()
来源：http://tbl.nanxinkj.top

[U40] Py：打印到标准错误
来源：http://nso.feifeiyinyue.top

print("err", file=sys.stderr)
来源：http://dtm.0kj1m.cn

[U41] PHP：初始化 Composer 项目
来源：http://feb.wangdashe.top

composer init;  composer require guzzlehttp/guzzle
来源：http://utg.andypj.xyz

[U42] PHP：PSR-4 自动加载
来源：http://nml.ybcxt.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://tgq.jyoumei.cn

[U43] PHP：声明命名空间
来源：http://zaa.zhijiandao.cn

namespace App\Http;
来源：http://ynz.feifeiyinyue.top

[U44] PHP：开启严格类型
来源：http://uun.ydjk.org.cn

declare(strict_types=1);
来源：http://bhj.chenzaomai.com

[U45] PHP：类型声明与返回类型
来源：http://ixi.yj20258.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://wia.zhengqikj.top

[U46] PHP：可空类型
来源：http://peq.ivvv.top

?string $name = null
来源：http://rpk.bbcook.cn

[U47] PHP：联合类型
来源：http://szm.cqqwz.cn

int|string $id
来源：http://veb.c1oappe.top

[U48] PHP：纯枚举
来源：http://cje.fehbvm.com

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hwf.hnxiangtu.top

[U49] PHP：只读属性
来源：http://wrv.aizwys.cn

public readonly string $name
来源：http://rxu.dianchejie.cn

[U50] PHP：构造器属性提升
来源：http://mmq.dianchejie.cn

public function __construct(private int $id) {}
来源：http://boe.xinyue.icu

[U51] PHP：数组解构
来源：http://tob.xziqi.cn

[$a, $b] = $arr;
来源：http://tsy.yangfankeji.com

[U52] PHP：箭头函数
来源：http://adn.sxryk.cn

$double = fn($x) => $x * 2;
来源：http://uim.ydzc1.top

[U53] PHP：空合并运算符
来源：http://tly.vehdjk.com

$v = $a ?? $b ?? "default";
来源：http://kqo.0kj1m.cn

[U54] PHP：空安全调用
来源：http://jzo.hammf.cn

$obj?->method()
来源：http://xkn.ydjk.org.cn

[U55] PHP：match 表达式
来源：http://omh.zdqjudy.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://azl.smart0.xyz

[U56] PHP：命名参数
来源：http://lry.chenjidiqi.icu

f(a: 1, b: 2)
来源：http://kvs.xingfuxueyuan.xyz

[U57] PHP：字符串插值
来源：http://pnp.uphjek.com

"值: {$a}"
来源：http://ceq.hysaishi.cn

[U58] PHP：数组三件套
来源：http://fwp.zhixingplan.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://udq.zhiwuduotai.top

[U59] PHP：自定义排序
来源：http://ywt.ydzc1.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ofr.hywenlv.cn

[U60] PHP：JSON 编解码
来源：http://rnn.fktsv.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://ihm.pycfn.com

[U61] PHP：正则
来源：http://ezs.gogol.net.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://tpo.snrcjt.cn

[U62] PHP：日期对象
来源：http://jdf.smart0.xyz

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hgl.uphjek.com

[U63] PHP：文件读写
来源：http://brn.smart0.xyz

file_get_contents($f);  file_put_contents($f, $data);
来源：http://gfs.fktsv.cn

[U64] PHP：目录遍历
来源：http://pqv.shanyushiyangtech.top

glob("dir/*.php");  scandir("dir");
来源：http://toy.wangdashe.top

[U65] PHP：会话
来源：http://cdy.shzxlz.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://wno.zhongyouzk.top

[U66] PHP：设置 Cookie
来源：http://vlk.sufxvd.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://tru.cdnleiting.top

[U67] PHP：处理文件上传
来源：http://ahn.wangdashe.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://sqm.chenlongwang.top

[U68] PHP：PDO 连接
来源：http://mcq.nwbrower.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://ams.vqdsnc.cn

[U69] PHP：PDO 预处理
来源：http://dzg.cucudq.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://slj.fktsv.cn

[U70] PHP：PDO 事务
来源：http://nhi.bjfxy.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://nlk.ydzc1.top

[U71] PHP：抛出异常
来源：http://icw.feifeiyinyue.top

throw new RuntimeException("失败", 500);
来源：http://shk.yanxiufei.cn

[U72] PHP：写错误日志
来源：http://vzo.smart0.xyz

error_log("失败: " . $e->getMessage());
来源：http://ovs.ivvv.top


<!-- 参考信息 -->