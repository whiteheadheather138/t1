代发 wailian999

int size() const noexcept { return n_; }
来源：http://lsy.jianghu66.top

[S53] C++：移动语义
来源：http://rlv.cheryme.top

std::vector<int> w = std::move(v);
来源：http://ydu.zhongyouzk.top

[S54] C++：异常处理
来源：http://aup.xuetiantiany.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://oib.jinghuilouyu.cn

[S55] C++：结构化绑定
来源：http://rgi.yj202588.top

auto [a, b] = std::make_pair(1, 2);
来源：http://cch.snrcjt.cn

[S56] C++：optional
来源：http://teq.shuidangran.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://vas.wangshuangyany.cn

[S57] C++：编译期常量
来源：http://ntp.pycfn.com

constexpr int N = 10;
来源：http://lah.xinyue.icu

[S58] C++：命名空间
来源：http://qfz.sweek.top

namespace ns { int f() { return 1; } }
来源：http://kba.chenjidiqi.icu

[S59] C++：静态断言
来源：http://ovh.xuanzx.com

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://ysc.nwbrower.top

[S60] C++：遍历并删除元素
来源：http://xtg.yueranfly.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://xsk.cucudq.cn

================================================================================
来源：http://tbb.zhoulong.xyz

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://ivm.hongshengwenyu.top

================================================================================
来源：http://lok.zhixingplan.top

[T01] Kotlin：Hello World
来源：http://bci.smart0.xyz

println("Hello")
来源：http://vnp.chenzaomai.com

[T02] Kotlin：变量
来源：http://bxr.yfazqb.com

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://ngn.uphjek.com

[T03] Kotlin：字符串模板
来源：http://ifd.wangdashe.top

"值: $b"
来源：http://ypy.fengsongda.top

[T04] Kotlin：空安全
来源：http://xsz.hywenlv.cn

val n: String? = null;  n?.length
来源：http://fkq.jlsjyb.cn

[T05] Kotlin：when 表达式
来源：http://dfb.chenjidiqi.icu

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://wkj.aibaodan.cn

[T06] Kotlin：集合映射
来源：http://aoh.cucudq.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://iqn.aizwys.cn

[T07] Kotlin：集合过滤
来源：http://nnz.yueranfly.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://hqo.ydjk.org.cn

[T08] Kotlin：数据类
来源：http://lxx.pengpengdd.cyou

data class User(val name: String, val age: Int)
来源：http://itb.jinqigufen.top

[T09] Kotlin：扩展函数
来源：http://owu.daria6918.cn

fun String.exclaim() = this + "!"
来源：http://upz.feifeiyinyue.top

[T10] Kotlin：默认参数
来源：http://rmb.yuanzhike.top

fun greet(name: String = "World") = "Hi $name"
来源：http://gbl.yonumen.top

[T11] Kotlin：协程
来源：http://btt.9152youxi.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://wxx.smart0.xyz

[T12] Kotlin：解构声明
来源：http://dme.jqgufenzy.top

val (a, b) = Pair(1, 2)
来源：http://cjo.hywenlv.cn

[T13] Kotlin：只读 Map
来源：http://lpn.hfpthk.cn

val m = mapOf("a" to 1)
来源：http://ies.52xcode.cn

[T14] Kotlin：循环
来源：http://ygj.sxryk.cn

for (i in 1..10) println(i)
来源：http://rfg.xziqi.cn

[T15] Kotlin：接口
来源：http://avh.andypj.xyz

interface Shape { fun area(): Double }
来源：http://qxc.zhaomingkeji.xyz

[T16] Swift：Hello World
来源：http://dhv.snrcjt.cn

print("Hello")
来源：http://bdi.yfazqb.com

[T17] Swift：变量与常量
来源：http://hei.jqgfzy.top

var a = 1;  let b = 2
来源：http://yrw.jqgufenzy.top

[T18] Swift：字符串插值
来源：http://zuv.jyoumei.cn

"值: \(b)"
来源：http://lzk.52xcode.cn

[T19] Swift：可选绑定
来源：http://ssy.ivvv.top

if let n = opt { print(n) }
来源：http://ijp.bjfxy.top

[T20] Swift：数组操作
来源：http://ygu.zhongyouzk.top

var a = [1, 2, 3];  a.append(4)
来源：http://fys.shanyushiyangtech.top

[T21] Swift：遍历
来源：http://khk.yuanzhike.top

for x in a { print(x) }
来源：http://dsc.feifeiyinyue.top

[T22] Swift：字典
来源：http://vbi.yanxiufei.cn

var d = ["a": 1];  d["b"] = 2
来源：http://xgp.hammf.cn

[T23] Swift：函数
来源：http://qxv.c1oappe.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://yws.jinghuilouyu.cn

[T24] Swift：闭包
来源：http://kbg.cqqwz.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://zqm.zhijiandao.cn

[T25] Swift：结构体
来源：http://zxr.wangshuangyany.cn

struct P { var x: Int }
来源：http://gcj.yueranfly.top

[T26] Swift：类与重写
来源：http://zfi.zhaomingkeji.xyz

class A: Base { override func f() {} }
来源：http://gfu.dianchejie.cn

[T27] Swift：错误处理
来源：http://iep.xinyue.icu

do { try f() } catch { print(error) }
来源：http://nyi.ybcxt.top

[T28] Swift：枚举
来源：http://mjq.zdqjudy.top

enum Color { case red, green }
来源：http://gyq.ybcxt.top

[T29] Swift：guard 提前返回
来源：http://mng.shuidangran.top

guard let x = opt else { return }
来源：http://opg.xuetiantiany.cn

[T30] Swift：协议
来源：http://itw.dashuyun.cn

protocol Shape { func area() -> Double }
来源：http://yfu.hongshengwenyu.top

[T31] Lua：Hello World
来源：http://gwl.hnqzz.top

print("Hello")
来源：http://xjj.zhaomingkeji.xyz

[T32] Lua：局部变量
来源：http://cxw.daria6918.cn

local a = 1
来源：http://rvd.fengsongda.top

[T33] Lua：表（数组）
来源：http://wve.yj20258.top

local t = {1, 2, 3};  t[4] = 4
来源：http://rod.jinghuilouyu.cn

[T34] Lua：遍历表
来源：http://lcm.pengpengdd.cyou

for i, v in ipairs(t) do print(i, v) end
来源：http://poq.smart0.xyz

[T35] Lua：字典表
来源：http://nbb.sjlbkw.cn

local d = { a = 1 };  d.b = 2
来源：http://qjo.nwbrower.top

[T36] Lua：函数
来源：http://vrh.ppjwa.cn

function add(a, b) return a + b end
来源：http://kbv.hysaishi.cn

[T37] Lua：字符串拼接
来源：http://brs.hesvh.cn

"a" .. "b"
来源：http://jaa.cqqwz.cn

[T38] Lua：条件
来源：http://wun.fktsv.cn

if x > 0 then print("正") end
来源：http://otb.yfazqb.com

[T39] Lua：模式匹配
来源：http://jex.zhijiandao.cn

string.find(s, "%d+")
来源：http://snc.ppjwa.cn

[T40] Lua：元表
来源：http://qwk.sjlbkw.cn

setmetatable({}, { __index = base })
来源：http://gev.mhx1999.top

[T41] Perl：Hello World
来源：http://gyq.yj202588.top

print "Hello\n";
来源：http://pnj.cdnleiting.top

[T42] Perl：变量类型
来源：http://pan.hcnkem.com

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://yjg.zhijiandao.cn

[T43] Perl：字符串插值
来源：http://nbf.gaohongyu789.top

"值: $a"
来源：http://tnk.zhoulong.xyz

[T44] Perl：条件
来源：http://bta.daxiang520.top

if ($a > 0) { print "正"; }
来源：http://xxk.hcnkem.com

[T45] Perl：数组遍历
来源：http://xvo.meibo888.top

for my $x (@arr) { print $x; }
来源：http://muc.hcnkem.com

[T46] Perl：哈希操作
来源：http://gam.xingfuxueyuan.xyz

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hyd.jinqigfzy.top

[T47] Perl：正则捕获
来源：http://fyx.hongshengwenyu.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://yga.vehdjk.com

[T48] Perl：正则替换
来源：http://wcl.zhengqikj.top

$s =~ s/old/new/g;
来源：http://djw.tanke756.top

[T49] Perl：函数
来源：http://smc.mhx1999.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://msu.nwbrower.top

[T50] Perl：逐行读文件
来源：http://lxt.daxiang520.top

open my $fh, "<", "a.txt" or die $!;
来源：http://fyd.tianlin.xyz

while (my $line = <$fh>) { print $line; }
来源：http://zmr.nanxuanxn.top

[T51] Scala：Hello World
来源：http://bnr.meibo888.top

println("Hello")
来源：http://ggb.chenlongwang.top

[T52] Scala：变量
来源：http://nei.shzxlz.cn

val a = 1;  var b = 2
来源：http://bht.cqqwz.cn

[T53] Scala：字符串插值
来源：http://ehe.fzhhl.top

s"值: $b"
来源：http://mhv.yj20258.top

[T54] Scala：集合映射
来源：http://ocp.mhx1999.top

List(1, 2, 3).map(_ * 2)
来源：http://tld.aibaodan.cn

[T55] Scala：集合过滤
来源：http://eis.jlsjyb.cn

List(1, 2, 3).filter(_ > 1)
来源：http://ykb.zhijiandao.cn

[T56] Scala：样例类
来源：http://yzh.jyoumei.cn

case class User(name: String, age: Int)
来源：http://aeb.sweek.top

[T57] Scala：模式匹配
来源：http://uxu.guowangkeji.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://zqe.shzxlz.cn

[T58] Scala：函数定义
来源：http://vkn.bbcook.cn

def add(a: Int, b: Int): Int = a + b
来源：http://btw.zhiwuduotai.top

[T59] Scala：循环
来源：http://qek.ybcxt.top

for (i <- 1 to 10) println(i)
来源：http://qin.shanyushiyangtech.top

[T60] Scala：折叠
来源：http://rje.mhx1999.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://bum.yueranfly.top

================================================================================
来源：http://fuy.jinqigfzy.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://erf.pengpengdd.cyou

================================================================================
来源：http://sah.yj20258888.top

[U01] Py：创建虚拟环境
来源：http://jdb.ydzc1.top

python -m venv .venv && source .venv/bin/activate
来源：http://qqm.shuidangran.top

[U02] Py：导出 / 安装依赖
来源：http://dbq.yangfankeji.com

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://vta.ctjpmb.com

[U03] Py：加载 .env 配置
来源：http://nyg.aibaodan.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://fhp.snrcjt.cn

[U04] Py：变量调试打印
来源：http://dyi.316326.xyz

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://bwq.tian-w.cn

[U05] Py：列表去重且保序
来源：http://wyz.feifeiyinyue.top

list(dict.fromkeys(arr))
来源：http://aax.pycfn.com

[U06] Py：合并两个字典
来源：http://bed.kuanghao11.cn

{**a, **b}
来源：http://qos.tarul.cn

[U07] Py：反转字典键值
来源：http://sbx.dianchejie.cn

{v: k for k, v in d.items()}
来源：http://lsj.smart0.xyz

[U08] Py：展平二维列表
来源：http://qnx.meibo888.top

[y for x in nested for y in x]
来源：http://syl.feifeiyinyue.top

[U09] Py：字典取最大值的键
来源：http://fpm.jyoumei.cn

max(d, key=d.get)
来源：http://gwy.sysykeji.top

[U10] Py：按值排序字典
来源：http://osf.epnwcf.com

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://sfc.ydzc1.top

[U11] Py：生成器表达式
来源：http://bai.jianghu66.top

(x * 2 for x in arr)
来源：http://tlk.xinyue.icu

[U12] Py：取出现最多的 3 个元素
来源：http://bcd.hcnkem.com

Counter(arr).most_common(3)
来源：http://miz.sxryk.cn

[U13] Py：固定长度队列
来源：http://pin.nwbrower.top

deque(maxlen=10)
来源：http://ehk.cdnleiting.top

[U14] Py：分组收集到列表
来源：http://isp.yfazqb.com

defaultdict(list)
来源：http://xkp.yj20258.top

[U15] Py：高精度计时
来源：http://xog.sxryk.cn

t = time.perf_counter()
来源：http://are.zhongyouzk.top

[U16] Py：命令行参数解析
来源：http://usb.vqdsnc.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://rxj.chenjidiqi.icu

[U17] Py：初始化日志
来源：http://ekb.sweek.top

logging.basicConfig(level=logging.INFO)
来源：http://osx.jqgfzy.top

[U18] Py：预编译正则
来源：http://lrs.dashuyun.cn

pat = re.compile(r"\d+")
来源：http://fkk.zhixingplan.top

[U19] Py：正则替换带回调
来源：http://hgf.c1oappe.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hub.jianghu66.top

[U20] Py：缓存函数结果
来源：http://ccm.gotoacloud.top

@functools.lru_cache(maxsize=None)
来源：http://izd.0kj1m.cn

[U21] Py：自定义上下文管理器
来源：http://ucw.jinqigufen.top

@contextlib.contextmanager
来源：http://lww.nanxinkj.top

[U22] Py：矩阵转置
来源：http://ppn.cashguo.top

list(zip(*m))
来源：http://olx.feifeiyinyue.top

[U23] Py：分块读取大文件
来源：http://faj.shangyingyoupin.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://fya.hammf.cn

[U24] Py：路径操作
来源：http://kcc.316326.xyz

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://fue.meibo888.top

[U25] Py：CSV 按字典读
来源：http://euu.jlsjyb.cn

csv.DictReader(f)
来源：http://csv.jianghu66.top

[U26] Py：并发下载
来源：http://eba.ydjk.org.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://bch.dashuyun.cn

[U27] Py：异步 HTTP
来源：http://end.daria6918.cn

aiohttp.ClientSession() 配合 async with
来源：http://kwx.zhiwuduotai.top

[U28] Py：类型别名
来源：http://phc.yvedp.cn

UserId = int
来源：http://psy.daria6918.cn

[U29] Py：属性校验
来源：http://wvr.nanxinkj.top

@property 与 @x.setter 配合
来源：http://iai.tarul.cn

[U30] Py：数据类
来源：http://tiq.wangshuangyany.cn

@dataclass(slots=True)
来源：http://epy.sxryk.cn

[U31] Py：单测
来源：http://tkl.chenzaomai.com

python -m pytest -q
来源：http://ioz.yueranfly.top

[U32] Py：代码格式化
来源：http://mxq.52xcode.cn

ruff format . && ruff check --fix .
来源：http://baq.havefunace.top

[U33] Py：打包发布
来源：http://pxi.xinyue.icu

python -m build  （依赖 pyproject.toml）
来源：http://wdg.quarkkingdee.top

[U34] Py：判断编码
来源：http://mxb.yueranfly.top

chardet.detect(raw)
来源：http://plu.yuanzhike.top

[U35] Py：发送邮件
来源：http://mdu.jyoumei.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://htt.sjlbkw.cn

[U36] Py：定时任务
来源：http://xye.zhongyouzk.top

schedule.every(10).minutes.do(job)
来源：http://nnz.gogol.net.cn

[U37] Py：读写 Excel
来源：http://pha.cucudq.cn

pandas.read_excel / DataFrame.to_excel
来源：http://hfo.hnqzz.top

[U38] Py：获取脚本所在目录
来源：http://vsd.wangdashe.top

Path(__file__).resolve().parent
来源：http://gvv.svipenyu.cn

[U39] Py：判断是否在交互环境
来源：http://slt.zhaomingkeji.xyz

sys.stdout.isatty()
来源：http://rcp.guannengcc.top

[U40] Py：打印到标准错误
来源：http://fst.meibo888.top

print("err", file=sys.stderr)
来源：http://bdn.cashguo.top

[U41] PHP：初始化 Composer 项目
来源：http://fkv.shanyushiyangtech.top

composer init;  composer require guzzlehttp/guzzle
来源：http://ipb.shuidangran.top

[U42] PHP：PSR-4 自动加载
来源：http://xnm.fehbvm.com

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://cwr.wangdashe.top

[U43] PHP：声明命名空间
来源：http://way.haohaochexian.top

namespace App\Http;
来源：http://zba.dashuyun.cn

[U44] PHP：开启严格类型
来源：http://dtl.feifeiyinyue.top

declare(strict_types=1);
来源：http://bba.haohaochexian.top

[U45] PHP：类型声明与返回类型
来源：http://ual.yj202588.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://tbo.ydzc1.top

[U46] PHP：可空类型
来源：http://ckr.chenjidiqi.icu

?string $name = null
来源：http://tos.xinyue.icu

[U47] PHP：联合类型
来源：http://ulq.sufxvd.cn

int|string $id
来源：http://sfi.bbcook.cn

[U48] PHP：纯枚举
来源：http://mkg.jqgufenzy.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://rnw.hfpthk.cn

[U49] PHP：只读属性
来源：http://tbi.bbcook.cn

public readonly string $name
来源：http://hfd.cashguo.top

[U50] PHP：构造器属性提升
来源：http://nlm.fktsv.cn

public function __construct(private int $id) {}
来源：http://exn.hesvh.cn

[U51] PHP：数组解构
来源：http://epo.jiagoushi.top

[$a, $b] = $arr;
来源：http://dwx.jinyuanbaomall.cn

[U52] PHP：箭头函数
来源：http://cre.xuanzx.com

$double = fn($x) => $x * 2;
来源：http://mge.tarul.cn

[U53] PHP：空合并运算符
来源：http://pql.yongpay.top

$v = $a ?? $b ?? "default";
来源：http://lpc.jianghu66.top

[U54] PHP：空安全调用
来源：http://cnc.kuanghao11.cn

$obj?->method()
来源：http://pum.52xcode.cn

[U55] PHP：match 表达式
来源：http://aft.zdbjq.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://elh.shangyingyoupin.top

[U56] PHP：命名参数
来源：http://fjj.zhaomingkeji.xyz

f(a: 1, b: 2)
来源：http://ueg.xinyue.icu

[U57] PHP：字符串插值
来源：http://pdn.nanxinkj.top

"值: {$a}"
来源：http://ztq.xziqi.cn

[U58] PHP：数组三件套
来源：http://ngf.yonumen.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://wlk.yongpay.top

[U59] PHP：自定义排序
来源：http://smi.jiagoushi.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://qen.shanyushiyangkeji.top

[U60] PHP：JSON 编解码
来源：http://tpp.jqgufenzy.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://dhr.zhiwuduotai.top

[U61] PHP：正则
来源：http://yre.ppjwa.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://qoo.cashguo.top

[U62] PHP：日期对象
来源：http://udv.hywenlv.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://klw.316326.xyz

[U63] PHP：文件读写
来源：http://fnl.sweek.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://dlz.jqgufenzy.top

[U64] PHP：目录遍历
来源：http://ize.hesvh.cn

glob("dir/*.php");  scandir("dir");
来源：http://zrx.c1oappe.top

[U65] PHP：会话
来源：http://opf.fktsv.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://ocl.ydzc1.top

[U66] PHP：设置 Cookie
来源：http://bcj.nwbrower.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://fkm.hcnkem.com

[U67] PHP：处理文件上传
来源：http://pii.xuetiantiany.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://ljm.yuxming.cn

[U68] PHP：PDO 连接
来源：http://xon.yj20258.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://tfx.bbcook.cn

[U69] PHP：PDO 预处理
来源：http://wlr.shangyingyoupin.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://diz.xingfuxueyuan.xyz

[U70] PHP：PDO 事务
来源：http://nmf.tianlin.xyz

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://nlo.ybcxt.top

[U71] PHP：抛出异常
来源：http://aan.mhx1999.top

throw new RuntimeException("失败", 500);
来源：http://mod.svipenyu.cn

[U72] PHP：写错误日志
来源：http://ouw.vqdsnc.cn

error_log("失败: " . $e->getMessage());
来源：http://qgv.316326.xyz

[U73] PHP：读取 ini 配置
来源：http://yif.epnwcf.com

parse_ini_file("config.ini", true)
来源：http://uec.daxiang520.top

[U74] PHP：读取环境变量
来源：http://qmm.epnwcf.com

getenv("APP_ENV") ?: "production"
来源：http://jln.fanxiaobao.xyz

[U75] PHP：依赖注入
来源：http://iwz.pycfn.com

composer require psr/container
来源：http://oea.meibo888.top

[U76] PHP：简单路由
来源：http://niy.gotoacloud.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://sqz.haohaochexian.top

[U77] PHP：模板渲染
来源：http://hdt.shangyingyoupin.top

composer require twig/twig
来源：http://lop.tianlin.xyz

[U78] PHP：单元测试
来源：http://xmf.mhx1999.top

composer require --dev phpunit/phpunit
来源：http://tdm.daxiang520.top


<!-- 参考信息 -->