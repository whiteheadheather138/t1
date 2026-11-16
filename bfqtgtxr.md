代发 wailian999

while (std::getline(in, line)) { }
来源：http://afx.nwbrower.top

[S49] C++：写文件
来源：http://ops.xinyue.icu

std::ofstream out("a.txt");  out << "hi\n";
来源：http://nkg.yuxming.cn

[S50] C++：格式化数字
来源：http://sdx.xuetiantiany.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://kqq.52xcode.cn

[S51] C++：显式类型转换
来源：http://fwv.sysykeji.top

static_cast<double>(a) / b
来源：http://bvk.xziqi.cn

[S52] C++：const 与 noexcept
来源：http://heq.tianlin.xyz

int size() const noexcept { return n_; }
来源：http://fba.pengpengdd.cyou

[S53] C++：移动语义
来源：http://hav.tianlin.xyz

std::vector<int> w = std::move(v);
来源：http://bsh.ywan-chungtsiang.top

[S54] C++：异常处理
来源：http://eoo.sufxvd.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://dax.ppjwa.cn

[S55] C++：结构化绑定
来源：http://nqe.zdqjudy.top

auto [a, b] = std::make_pair(1, 2);
来源：http://lsj.ywan-chungtsiang.top

[S56] C++：optional
来源：http://rhz.yfazqb.com

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://cie.gotoacloud.top

[S57] C++：编译期常量
来源：http://kjc.svipenyu.cn

constexpr int N = 10;
来源：http://yxo.yj202588.top

[S58] C++：命名空间
来源：http://hwi.aizwys.cn

namespace ns { int f() { return 1; } }
来源：http://axy.jinghuilouyu.cn

[S59] C++：静态断言
来源：http://jgf.yangfankeji.com

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://utg.vqdsnc.cn

[S60] C++：遍历并删除元素
来源：http://xaf.pycfn.com

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://bnq.chenjidiqi.icu

================================================================================
来源：http://ojt.shuidangran.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://xwn.nanxuanxn.top

================================================================================
来源：http://viu.kuanghao11.cn

[T01] Kotlin：Hello World
来源：http://uct.aizwys.cn

println("Hello")
来源：http://lmg.hammf.cn

[T02] Kotlin：变量
来源：http://hoc.vqdsnc.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://bey.gogol.net.cn

[T03] Kotlin：字符串模板
来源：http://fsa.jinyuanbaomall.cn

"值: $b"
来源：http://wwc.uphjek.com

[T04] Kotlin：空安全
来源：http://hnv.ctjpmb.com

val n: String? = null;  n?.length
来源：http://vqi.xuetiantiany.cn

[T05] Kotlin：when 表达式
来源：http://sxd.nanxinkj.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://ixt.jinqigfzy.top

[T06] Kotlin：集合映射
来源：http://qbt.hesvh.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://pxm.hfpthk.cn

[T07] Kotlin：集合过滤
来源：http://ais.nwbrower.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://nod.tian-w.cn

[T08] Kotlin：数据类
来源：http://rqj.haohaochexian.top

data class User(val name: String, val age: Int)
来源：http://wrk.uphjek.com

[T09] Kotlin：扩展函数
来源：http://fxc.fanxiaobao.xyz

fun String.exclaim() = this + "!"
来源：http://zhy.pengpengdd.cyou

[T10] Kotlin：默认参数
来源：http://vjx.vehdjk.com

fun greet(name: String = "World") = "Hi $name"
来源：http://hiv.gogol.net.cn

[T11] Kotlin：协程
来源：http://nax.bbcook.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://mce.tianlin.xyz

[T12] Kotlin：解构声明
来源：http://sls.hfpthk.cn

val (a, b) = Pair(1, 2)
来源：http://vua.hysaishi.cn

[T13] Kotlin：只读 Map
来源：http://fhy.bjfxy.top

val m = mapOf("a" to 1)
来源：http://daz.xinyue.icu

[T14] Kotlin：循环
来源：http://qfx.uphjek.com

for (i in 1..10) println(i)
来源：http://dlj.zhiwuduotai.top

[T15] Kotlin：接口
来源：http://uva.yueranfly.top

interface Shape { fun area(): Double }
来源：http://jgh.andypj.xyz

[T16] Swift：Hello World
来源：http://hwa.yfazqb.com

print("Hello")
来源：http://yme.svipenyu.cn

[T17] Swift：变量与常量
来源：http://noy.ppjwa.cn

var a = 1;  let b = 2
来源：http://wpg.iojbl.cn

[T18] Swift：字符串插值
来源：http://ixh.gogol.net.cn

"值: \(b)"
来源：http://gsa.bjfxy.top

[T19] Swift：可选绑定
来源：http://ghg.hfpthk.cn

if let n = opt { print(n) }
来源：http://nga.shangyingyoupin.top

[T20] Swift：数组操作
来源：http://gds.guannengcc.top

var a = [1, 2, 3];  a.append(4)
来源：http://csr.shangyingyoupin.top

[T21] Swift：遍历
来源：http://gjf.andypj.xyz

for x in a { print(x) }
来源：http://uea.cdnleiting.top

[T22] Swift：字典
来源：http://dbz.cucudq.cn

var d = ["a": 1];  d["b"] = 2
来源：http://xms.haohaochexian.top

[T23] Swift：函数
来源：http://efn.nwbrower.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://xuh.ydzc1.top

[T24] Swift：闭包
来源：http://wft.zhaomingkeji.xyz

let f = { (x: Int) -> Int in x * 2 }
来源：http://spn.tian-w.cn

[T25] Swift：结构体
来源：http://ill.yonumen.top

struct P { var x: Int }
来源：http://sed.hammf.cn

[T26] Swift：类与重写
来源：http://oyw.hfpthk.cn

class A: Base { override func f() {} }
来源：http://qmz.hnxiangtu.top

[T27] Swift：错误处理
来源：http://uht.ctjpmb.com

do { try f() } catch { print(error) }
来源：http://qmi.zhaomingkeji.xyz

[T28] Swift：枚举
来源：http://jxi.wangshuangyany.cn

enum Color { case red, green }
来源：http://otb.redwolf501.top

[T29] Swift：guard 提前返回
来源：http://vnj.svipenyu.cn

guard let x = opt else { return }
来源：http://qnl.zhaomingkeji.xyz

[T30] Swift：协议
来源：http://gva.epnwcf.com

protocol Shape { func area() -> Double }
来源：http://zpn.jinghuilouyu.cn

[T31] Lua：Hello World
来源：http://rsu.jqgufenzy.top

print("Hello")
来源：http://sob.fehbvm.com

[T32] Lua：局部变量
来源：http://kvl.52xcode.cn

local a = 1
来源：http://dzd.daria6918.cn

[T33] Lua：表（数组）
来源：http://ggq.havefunace.top

local t = {1, 2, 3};  t[4] = 4
来源：http://ned.xingfuxueyuan.xyz

[T34] Lua：遍历表
来源：http://ocp.fktsv.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://nvy.bjfxy.top

[T35] Lua：字典表
来源：http://rzj.hywenlv.cn

local d = { a = 1 };  d.b = 2
来源：http://bep.yj202588.top

[T36] Lua：函数
来源：http://rjg.chenjidiqi.icu

function add(a, b) return a + b end
来源：http://ozo.fanxiaobao.xyz

[T37] Lua：字符串拼接
来源：http://hsl.tian-w.cn

"a" .. "b"
来源：http://mub.mhx1999.top

[T38] Lua：条件
来源：http://pmj.nwbrower.top

if x > 0 then print("正") end
来源：http://xph.guowangkeji.top

[T39] Lua：模式匹配
来源：http://kmt.cheryme.top

string.find(s, "%d+")
来源：http://zsr.fengsongda.top

[T40] Lua：元表
来源：http://dev.chenzaomai.com

setmetatable({}, { __index = base })
来源：http://lyu.hammf.cn

[T41] Perl：Hello World
来源：http://iwt.svipenyu.cn

print "Hello\n";
来源：http://dxd.zhengqikj.top

[T42] Perl：变量类型
来源：http://qsx.cdnleiting.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://vep.chenlongwang.top

[T43] Perl：字符串插值
来源：http://fiq.ctjpmb.com

"值: $a"
来源：http://xjf.yuanzhike.top

[T44] Perl：条件
来源：http://tbb.ydzc1.top

if ($a > 0) { print "正"; }
来源：http://brw.xinyue.icu

[T45] Perl：数组遍历
来源：http://qix.havefunace.top

for my $x (@arr) { print $x; }
来源：http://ksg.hnxiangtu.top

[T46] Perl：哈希操作
来源：http://roc.ybcxt.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://quv.xinyue.icu

[T47] Perl：正则捕获
来源：http://yjb.cqqwz.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://uvt.ppjwa.cn

[T48] Perl：正则替换
来源：http://rjt.yuanzhike.top

$s =~ s/old/new/g;
来源：http://nnj.feifeiyinyue.top

[T49] Perl：函数
来源：http://nba.c1oappe.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://cyf.yonumen.top

[T50] Perl：逐行读文件
来源：http://ruw.shanyushiyangkeji.top

open my $fh, "<", "a.txt" or die $!;
来源：http://hbb.zdbjq.cn

while (my $line = <$fh>) { print $line; }
来源：http://ltl.yueranfly.top

[T51] Scala：Hello World
来源：http://acb.zhixingplan.top

println("Hello")
来源：http://jou.yuanzhike.top

[T52] Scala：变量
来源：http://imm.sxryk.cn

val a = 1;  var b = 2
来源：http://mai.ydzc1.top

[T53] Scala：字符串插值
来源：http://ojx.feifeiyinyue.top

s"值: $b"
来源：http://pfc.shangyingyoupin.top

[T54] Scala：集合映射
来源：http://bhx.birdmap.top

List(1, 2, 3).map(_ * 2)
来源：http://unz.daria6918.cn

[T55] Scala：集合过滤
来源：http://dgj.fanxiaobao.xyz

List(1, 2, 3).filter(_ > 1)
来源：http://zrp.zhaomingkeji.xyz

[T56] Scala：样例类
来源：http://wmg.shzxlz.cn

case class User(name: String, age: Int)
来源：http://oir.hnxiangtu.top

[T57] Scala：模式匹配
来源：http://zdc.ivvv.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://ahn.jyoumei.cn

[T58] Scala：函数定义
来源：http://ywr.gogol.net.cn

def add(a: Int, b: Int): Int = a + b
来源：http://gnf.bjfxy.top

[T59] Scala：循环
来源：http://pwp.jianghu66.top

for (i <- 1 to 10) println(i)
来源：http://kic.feifeiyinyue.top

[T60] Scala：折叠
来源：http://qkb.ybcxt.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://fkh.hnxiangtu.top

================================================================================
来源：http://rcl.yonumen.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://vtn.svipenyu.cn

================================================================================
来源：http://rwr.hcnkem.com

[U01] Py：创建虚拟环境
来源：http://biq.hywenlv.cn

python -m venv .venv && source .venv/bin/activate
来源：http://rgd.nwbrower.top

[U02] Py：导出 / 安装依赖
来源：http://mmf.ehwqpu.com

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://dxe.9152youxi.cn

[U03] Py：加载 .env 配置
来源：http://ary.sweek.top

from dotenv import load_dotenv; load_dotenv()
来源：http://iys.nwbrower.top

[U04] Py：变量调试打印
来源：http://hcz.nanxinkj.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://ody.chenjidiqi.icu

[U05] Py：列表去重且保序
来源：http://tro.tanke756.top

list(dict.fromkeys(arr))
来源：http://cmf.aizwys.cn

[U06] Py：合并两个字典
来源：http://hdv.bbcook.cn

{**a, **b}
来源：http://dez.52xcode.cn

[U07] Py：反转字典键值
来源：http://run.yueranfly.top

{v: k for k, v in d.items()}
来源：http://hxx.zhoulong.xyz

[U08] Py：展平二维列表
来源：http://dvr.zdbjq.cn

[y for x in nested for y in x]
来源：http://cxo.fzhhl.top

[U09] Py：字典取最大值的键
来源：http://ijj.feifeiyinyue.top

max(d, key=d.get)
来源：http://zsu.316326.xyz

[U10] Py：按值排序字典
来源：http://jxz.hywenlv.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://weo.zhoulong.xyz

[U11] Py：生成器表达式
来源：http://eab.iojbl.cn

(x * 2 for x in arr)
来源：http://ghn.quarkkingdee.top

[U12] Py：取出现最多的 3 个元素
来源：http://vlm.nwbrower.top

Counter(arr).most_common(3)
来源：http://ojk.shangyingyoupin.top

[U13] Py：固定长度队列
来源：http://vxn.hnqzz.top

deque(maxlen=10)
来源：http://tev.meibo888.top

[U14] Py：分组收集到列表
来源：http://yff.zhongyouzk.top

defaultdict(list)
来源：http://ans.sufxvd.cn

[U15] Py：高精度计时
来源：http://umf.hesvh.cn

t = time.perf_counter()
来源：http://qyf.jinyuanbaomall.cn

[U16] Py：命令行参数解析
来源：http://fws.smart0.xyz

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://ceh.jinghuilouyu.cn

[U17] Py：初始化日志
来源：http://qbr.hongshengwenyu.top

logging.basicConfig(level=logging.INFO)
来源：http://jnn.epnwcf.com

[U18] Py：预编译正则
来源：http://cio.shuidangran.top

pat = re.compile(r"\d+")
来源：http://amh.zhengqikj.top

[U19] Py：正则替换带回调
来源：http://rwa.daxiang520.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://tpi.dashuyun.cn

[U20] Py：缓存函数结果
来源：http://cjc.gotoacloud.top

@functools.lru_cache(maxsize=None)
来源：http://xlu.xylfe.cn

[U21] Py：自定义上下文管理器
来源：http://xib.zycfv.cn

@contextlib.contextmanager
来源：http://kfc.uphjek.com

[U22] Py：矩阵转置
来源：http://nom.gotoacloud.top

list(zip(*m))
来源：http://jiq.shanyushiyangtech.top

[U23] Py：分块读取大文件
来源：http://aeu.hesvh.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://pxe.andypj.xyz

[U24] Py：路径操作
来源：http://sqe.cucudq.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://zyq.svipenyu.cn

[U25] Py：CSV 按字典读
来源：http://kil.jqgufenzy.top

csv.DictReader(f)
来源：http://nit.epnwcf.com

[U26] Py：并发下载
来源：http://epe.fanxiaobao.xyz

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://yhg.jqgufenzy.top

[U27] Py：异步 HTTP
来源：http://ttg.yj20258.top

aiohttp.ClientSession() 配合 async with
来源：http://kjx.zycfv.cn

[U28] Py：类型别名
来源：http://udd.yj202588.top

UserId = int
来源：http://wbh.zhongyouzk.top

[U29] Py：属性校验
来源：http://rcs.epnwcf.com

@property 与 @x.setter 配合
来源：http://ars.snrcjt.cn

[U30] Py：数据类
来源：http://gwy.dianchejie.cn

@dataclass(slots=True)
来源：http://cwn.fzhhl.top

[U31] Py：单测
来源：http://jvr.zycfv.cn

python -m pytest -q
来源：http://zxw.wangdashe.top

[U32] Py：代码格式化
来源：http://pym.zhiwuduotai.top

ruff format . && ruff check --fix .
来源：http://jod.pycfn.com

[U33] Py：打包发布
来源：http://itf.chenzaomai.com

python -m build  （依赖 pyproject.toml）
来源：http://tja.ywan-chungtsiang.top

[U34] Py：判断编码
来源：http://zvl.cashguo.top

chardet.detect(raw)
来源：http://zif.svipenyu.cn

[U35] Py：发送邮件
来源：http://qql.quarkkingdee.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://ypj.wangshuangyany.cn

[U36] Py：定时任务
来源：http://skl.jinghuilouyu.cn

schedule.every(10).minutes.do(job)
来源：http://oej.chenzaomai.com

[U37] Py：读写 Excel
来源：http://gvd.9152youxi.cn

pandas.read_excel / DataFrame.to_excel
来源：http://lhx.yangfankeji.com

[U38] Py：获取脚本所在目录
来源：http://faq.ppjwa.cn

Path(__file__).resolve().parent
来源：http://ubw.haohaochexian.top

[U39] Py：判断是否在交互环境
来源：http://tdf.wangdashe.top

sys.stdout.isatty()
来源：http://pyt.yj20258888.top

[U40] Py：打印到标准错误
来源：http://fxj.jinghuilouyu.cn

print("err", file=sys.stderr)
来源：http://yih.hysaishi.cn

[U41] PHP：初始化 Composer 项目
来源：http://vjw.cucudq.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://jsm.feifeiyinyue.top

[U42] PHP：PSR-4 自动加载
来源：http://evc.jinqigfzy.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://cxp.jiagoushi.top

[U43] PHP：声明命名空间
来源：http://qfw.jinqigufen.top

namespace App\Http;
来源：http://eue.jyoumei.cn

[U44] PHP：开启严格类型
来源：http://wcx.shuidangran.top

declare(strict_types=1);
来源：http://cac.ydjk.org.cn

[U45] PHP：类型声明与返回类型
来源：http://zta.zhongyouzk.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://odq.cashguo.top

[U46] PHP：可空类型
来源：http://quz.uphjek.com

?string $name = null
来源：http://ggn.aizwys.cn

[U47] PHP：联合类型
来源：http://wnp.shanyushiyangtech.top

int|string $id
来源：http://rhj.yuanzhike.top

[U48] PHP：纯枚举
来源：http://wbj.guannengcc.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://tmy.9152youxi.cn

[U49] PHP：只读属性
来源：http://gdg.vehdjk.com

public readonly string $name
来源：http://hun.sweek.top

[U50] PHP：构造器属性提升
来源：http://fww.fanxiaobao.xyz

public function __construct(private int $id) {}
来源：http://cri.sjlbkw.cn

[U51] PHP：数组解构
来源：http://spo.hongshengwenyu.top

[$a, $b] = $arr;
来源：http://ads.shzxlz.cn

[U52] PHP：箭头函数
来源：http://fke.jinghuilouyu.cn

$double = fn($x) => $x * 2;
来源：http://hpq.jyoumei.cn

[U53] PHP：空合并运算符
来源：http://ghd.aibaodan.cn

$v = $a ?? $b ?? "default";
来源：http://xpn.aizwys.cn

[U54] PHP：空安全调用
来源：http://rul.shuidangran.top

$obj?->method()
来源：http://mcu.yuxming.cn

[U55] PHP：match 表达式
来源：http://iqq.shangyingyoupin.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://vpm.xinyue.icu

[U56] PHP：命名参数
来源：http://yrk.cheryme.top

f(a: 1, b: 2)
来源：http://kez.quarkkingdee.top

[U57] PHP：字符串插值
来源：http://lep.tanke756.top

"值: {$a}"
来源：http://qcj.zhongyouzk.top

[U58] PHP：数组三件套
来源：http://dpn.yj20258888.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://xvi.yangfankeji.com

[U59] PHP：自定义排序
来源：http://not.9152youxi.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://aez.tarul.cn

[U60] PHP：JSON 编解码
来源：http://duq.sysykeji.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://igo.smart0.xyz

[U61] PHP：正则
来源：http://csx.nwbrower.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://khc.epnwcf.com

[U62] PHP：日期对象
来源：http://vwn.9152youxi.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://tqv.zhixingplan.top

[U63] PHP：文件读写
来源：http://iot.havefunace.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://yon.0kj1m.cn

[U64] PHP：目录遍历
来源：http://ndi.hesvh.cn

glob("dir/*.php");  scandir("dir");
来源：http://kuk.smart0.xyz

[U65] PHP：会话
来源：http://grr.ywan-chungtsiang.top

session_start();  $_SESSION["uid"] = 1;
来源：http://zhb.yueranfly.top

[U66] PHP：设置 Cookie
来源：http://nnd.fehbvm.com

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://hmc.xingfuxueyuan.xyz

[U67] PHP：处理文件上传
来源：http://gjh.yongpay.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://nsk.zhiwuduotai.top

[U68] PHP：PDO 连接
来源：http://hgo.zhiwuduotai.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://inm.kuanghao11.cn

[U69] PHP：PDO 预处理
来源：http://dsk.hfpthk.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://wlq.vqdsnc.cn

[U70] PHP：PDO 事务
来源：http://ikg.chenzaomai.com

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://lxj.cashguo.top

[U71] PHP：抛出异常
来源：http://plm.0kj1m.cn

throw new RuntimeException("失败", 500);
来源：http://pnr.yj202588.top

[U72] PHP：写错误日志
来源：http://mrj.quarkkingdee.top

error_log("失败: " . $e->getMessage());
来源：http://shv.52xcode.cn

[U73] PHP：读取 ini 配置
来源：http://ihu.fengsongda.top

parse_ini_file("config.ini", true)
来源：http://xcw.nanxuanxn.top

[U74] PHP：读取环境变量
来源：http://vzh.mhx1999.top

getenv("APP_ENV") ?: "production"
来源：http://eck.gaohongyu789.top


<!-- 参考信息 -->