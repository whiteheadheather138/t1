代发 wailian999

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://bew.ydzc1.top

[S55] C++：结构化绑定
来源：http://orv.yj20258888.top

auto [a, b] = std::make_pair(1, 2);
来源：http://jof.daxiang520.top

[S56] C++：optional
来源：http://pyw.guannengcc.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://aqx.tianlin.xyz

[S57] C++：编译期常量
来源：http://gkk.gotoacloud.top

constexpr int N = 10;
来源：http://fgm.ybcxt.top

[S58] C++：命名空间
来源：http://pnr.hnqzz.top

namespace ns { int f() { return 1; } }
来源：http://gsm.hysaishi.cn

[S59] C++：静态断言
来源：http://osj.shanyushiyangkeji.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://oue.yvedp.cn

[S60] C++：遍历并删除元素
来源：http://rrw.hnxiangtu.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://imh.sjlbkw.cn

================================================================================
来源：http://eww.guannengcc.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://lpr.ywan-chungtsiang.top

================================================================================
来源：http://vpi.xylfe.cn

[T01] Kotlin：Hello World
来源：http://jst.tarul.cn

println("Hello")
来源：http://dvj.kuanghao11.cn

[T02] Kotlin：变量
来源：http://eim.jyoumei.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://itj.zhixingplan.top

[T03] Kotlin：字符串模板
来源：http://mvi.cucudq.cn

"值: $b"
来源：http://elf.shangyingyoupin.top

[T04] Kotlin：空安全
来源：http://cuo.nwbrower.top

val n: String? = null;  n?.length
来源：http://inz.kuanghao11.cn

[T05] Kotlin：when 表达式
来源：http://bal.smart0.xyz

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://wll.zhijiandao.cn

[T06] Kotlin：集合映射
来源：http://iax.chenlongwang.top

listOf(1, 2, 3).map { it * 2 }
来源：http://xap.hongshengwenyu.top

[T07] Kotlin：集合过滤
来源：http://jqm.kuanghao11.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://hhf.dashuyun.cn

[T08] Kotlin：数据类
来源：http://jnb.aizwys.cn

data class User(val name: String, val age: Int)
来源：http://bmr.fehbvm.com

[T09] Kotlin：扩展函数
来源：http://bha.jlsjyb.cn

fun String.exclaim() = this + "!"
来源：http://wfd.xuanzx.com

[T10] Kotlin：默认参数
来源：http://ywj.xingfuxueyuan.xyz

fun greet(name: String = "World") = "Hi $name"
来源：http://tpd.hywenlv.cn

[T11] Kotlin：协程
来源：http://usb.cucudq.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://ugx.cqqwz.cn

[T12] Kotlin：解构声明
来源：http://xpa.hesvh.cn

val (a, b) = Pair(1, 2)
来源：http://awk.zhiwuduotai.top

[T13] Kotlin：只读 Map
来源：http://cvp.ehwqpu.com

val m = mapOf("a" to 1)
来源：http://mti.iojbl.cn

[T14] Kotlin：循环
来源：http://pxy.0kj1m.cn

for (i in 1..10) println(i)
来源：http://olx.zhixingplan.top

[T15] Kotlin：接口
来源：http://hww.fehbvm.com

interface Shape { fun area(): Double }
来源：http://xcn.cucudq.cn

[T16] Swift：Hello World
来源：http://htl.zhongyouzk.top

print("Hello")
来源：http://kfp.aizwys.cn

[T17] Swift：变量与常量
来源：http://axj.xinyue.icu

var a = 1;  let b = 2
来源：http://txy.ydzc1.top

[T18] Swift：字符串插值
来源：http://bqn.shzxlz.cn

"值: \(b)"
来源：http://dhy.tian-w.cn

[T19] Swift：可选绑定
来源：http://iuj.0kj1m.cn

if let n = opt { print(n) }
来源：http://bke.fengsongda.top

[T20] Swift：数组操作
来源：http://vbs.gzhubu.top

var a = [1, 2, 3];  a.append(4)
来源：http://agn.cdnleiting.top

[T21] Swift：遍历
来源：http://ylu.xuanzx.com

for x in a { print(x) }
来源：http://xok.fanxiaobao.xyz

[T22] Swift：字典
来源：http://fuz.chenlongwang.top

var d = ["a": 1];  d["b"] = 2
来源：http://xhi.ivvv.top

[T23] Swift：函数
来源：http://fje.nanxinkj.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://yfo.tarul.cn

[T24] Swift：闭包
来源：http://bzs.jinqigufen.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://rxa.yj20258888.top

[T25] Swift：结构体
来源：http://zwn.hcnkem.com

struct P { var x: Int }
来源：http://fly.zhongyouzk.top

[T26] Swift：类与重写
来源：http://crx.quarkkingdee.top

class A: Base { override func f() {} }
来源：http://uei.hnqzz.top

[T27] Swift：错误处理
来源：http://tjy.jianghu66.top

do { try f() } catch { print(error) }
来源：http://vfe.fzhhl.top

[T28] Swift：枚举
来源：http://srw.xingfuxueyuan.xyz

enum Color { case red, green }
来源：http://hmw.tarul.cn

[T29] Swift：guard 提前返回
来源：http://hyz.zhixingplan.top

guard let x = opt else { return }
来源：http://gkp.yj20258.top

[T30] Swift：协议
来源：http://eak.xinyue.icu

protocol Shape { func area() -> Double }
来源：http://cqb.zdqjudy.top

[T31] Lua：Hello World
来源：http://nzf.aibaodan.cn

print("Hello")
来源：http://ogk.meibo888.top

[T32] Lua：局部变量
来源：http://tqf.svipenyu.cn

local a = 1
来源：http://uxg.yj202588.top

[T33] Lua：表（数组）
来源：http://fkv.xylfe.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://ifo.tarul.cn

[T34] Lua：遍历表
来源：http://ksc.9152youxi.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://vsv.jinqigfzy.top

[T35] Lua：字典表
来源：http://yrr.jinqigufen.top

local d = { a = 1 };  d.b = 2
来源：http://niw.yj20258.top

[T36] Lua：函数
来源：http://yla.yonumen.top

function add(a, b) return a + b end
来源：http://sbt.hfpthk.cn

[T37] Lua：字符串拼接
来源：http://tsc.dashuyun.cn

"a" .. "b"
来源：http://wmq.chenzaomai.com

[T38] Lua：条件
来源：http://ueq.wangdashe.top

if x > 0 then print("正") end
来源：http://idn.jqgfzy.top

[T39] Lua：模式匹配
来源：http://cxb.tarul.cn

string.find(s, "%d+")
来源：http://sct.haohaochexian.top

[T40] Lua：元表
来源：http://etu.xylfe.cn

setmetatable({}, { __index = base })
来源：http://jbj.yj202588.top

[T41] Perl：Hello World
来源：http://xcn.guannengcc.top

print "Hello\n";
来源：http://apc.shangyingyoupin.top

[T42] Perl：变量类型
来源：http://qyg.xziqi.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://xyu.cashguo.top

[T43] Perl：字符串插值
来源：http://bdc.gaohongyu789.top

"值: $a"
来源：http://vnf.andypj.xyz

[T44] Perl：条件
来源：http://ids.shzxlz.cn

if ($a > 0) { print "正"; }
来源：http://fzf.shzxlz.cn

[T45] Perl：数组遍历
来源：http://bzr.yuanzhike.top

for my $x (@arr) { print $x; }
来源：http://pkz.jlsjyb.cn

[T46] Perl：哈希操作
来源：http://pks.cucudq.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://gwq.daria6918.cn

[T47] Perl：正则捕获
来源：http://xrw.yvedp.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://ytk.yangfankeji.com

[T48] Perl：正则替换
来源：http://hdn.daria6918.cn

$s =~ s/old/new/g;
来源：http://cpo.quarkkingdee.top

[T49] Perl：函数
来源：http://fim.jinghuilouyu.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://tvg.ctjpmb.com

[T50] Perl：逐行读文件
来源：http://qvc.meibo888.top

open my $fh, "<", "a.txt" or die $!;
来源：http://ryy.zycfv.cn

while (my $line = <$fh>) { print $line; }
来源：http://rio.sufxvd.cn

[T51] Scala：Hello World
来源：http://tad.hesvh.cn

println("Hello")
来源：http://lxy.sysykeji.top

[T52] Scala：变量
来源：http://rqt.jinghuilouyu.cn

val a = 1;  var b = 2
来源：http://sbk.sysykeji.top

[T53] Scala：字符串插值
来源：http://wil.uphjek.com

s"值: $b"
来源：http://tsl.vehdjk.com

[T54] Scala：集合映射
来源：http://sre.zdbjq.cn

List(1, 2, 3).map(_ * 2)
来源：http://znq.yueranfly.top

[T55] Scala：集合过滤
来源：http://otp.ehwqpu.com

List(1, 2, 3).filter(_ > 1)
来源：http://mjm.jinyuanbaomall.cn

[T56] Scala：样例类
来源：http://cam.ydjk.org.cn

case class User(name: String, age: Int)
来源：http://wja.jyoumei.cn

[T57] Scala：模式匹配
来源：http://jil.yj20258.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://mgl.cashguo.top

[T58] Scala：函数定义
来源：http://rpm.mhx1999.top

def add(a: Int, b: Int): Int = a + b
来源：http://joj.tanke756.top

[T59] Scala：循环
来源：http://bqq.sjlbkw.cn

for (i <- 1 to 10) println(i)
来源：http://upo.jlsjyb.cn

[T60] Scala：折叠
来源：http://eea.hesvh.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://lwj.xziqi.cn

================================================================================
来源：http://mod.guannengcc.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://pqm.gzhubu.top

================================================================================
来源：http://kwu.sweek.top

[U01] Py：创建虚拟环境
来源：http://raz.jinqigufen.top

python -m venv .venv && source .venv/bin/activate
来源：http://pvi.xziqi.cn

[U02] Py：导出 / 安装依赖
来源：http://zxe.kuanghao11.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://jvo.wangshuangyany.cn

[U03] Py：加载 .env 配置
来源：http://pvu.fengsongda.top

from dotenv import load_dotenv; load_dotenv()
来源：http://egz.jinqigufen.top

[U04] Py：变量调试打印
来源：http://wuq.sufxvd.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hky.bjfxy.top

[U05] Py：列表去重且保序
来源：http://aav.xuanzx.com

list(dict.fromkeys(arr))
来源：http://nlk.sjlbkw.cn

[U06] Py：合并两个字典
来源：http://wgp.hnxiangtu.top

{**a, **b}
来源：http://ulr.hfpthk.cn

[U07] Py：反转字典键值
来源：http://wgx.andypj.xyz

{v: k for k, v in d.items()}
来源：http://glt.uphjek.com

[U08] Py：展平二维列表
来源：http://sld.uphjek.com

[y for x in nested for y in x]
来源：http://giy.shangyingyoupin.top

[U09] Py：字典取最大值的键
来源：http://ksz.ctjpmb.com

max(d, key=d.get)
来源：http://nza.jinghuilouyu.cn

[U10] Py：按值排序字典
来源：http://ioy.nanxinkj.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://juv.9152youxi.cn

[U11] Py：生成器表达式
来源：http://dyl.jiagoushi.top

(x * 2 for x in arr)
来源：http://jlh.jyoumei.cn

[U12] Py：取出现最多的 3 个元素
来源：http://bzd.epnwcf.com

Counter(arr).most_common(3)
来源：http://zth.bjfxy.top

[U13] Py：固定长度队列
来源：http://rzp.yj20258.top

deque(maxlen=10)
来源：http://hem.yanxiufei.cn

[U14] Py：分组收集到列表
来源：http://pbz.xziqi.cn

defaultdict(list)
来源：http://epr.sweek.top

[U15] Py：高精度计时
来源：http://lum.daria6918.cn

t = time.perf_counter()
来源：http://jbw.gzhubu.top

[U16] Py：命令行参数解析
来源：http://oae.fanxiaobao.xyz

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://mwm.sweek.top

[U17] Py：初始化日志
来源：http://sky.yj20258.top

logging.basicConfig(level=logging.INFO)
来源：http://cwa.tian-w.cn

[U18] Py：预编译正则
来源：http://fro.iojbl.cn

pat = re.compile(r"\d+")
来源：http://iig.jyoumei.cn

[U19] Py：正则替换带回调
来源：http://jbm.gzhubu.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://wtl.tian-w.cn

[U20] Py：缓存函数结果
来源：http://qdy.zhaomingkeji.xyz

@functools.lru_cache(maxsize=None)
来源：http://lrt.redwolf501.top

[U21] Py：自定义上下文管理器
来源：http://rqw.hysaishi.cn

@contextlib.contextmanager
来源：http://wed.nwbrower.top

[U22] Py：矩阵转置
来源：http://mcx.wangdashe.top

list(zip(*m))
来源：http://nzr.daria6918.cn

[U23] Py：分块读取大文件
来源：http://stl.chenjidiqi.icu

for chunk in iter(lambda: f.read(8192), b""):
来源：http://jbp.tianlin.xyz

[U24] Py：路径操作
来源：http://lzp.shzxlz.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://nfy.fehbvm.com

[U25] Py：CSV 按字典读
来源：http://czl.redwolf501.top

csv.DictReader(f)
来源：http://pbo.jinyuanbaomall.cn

[U26] Py：并发下载
来源：http://rbs.quarkkingdee.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://lgq.xinyue.icu

[U27] Py：异步 HTTP
来源：http://khl.jianghu66.top

aiohttp.ClientSession() 配合 async with
来源：http://ovv.ywan-chungtsiang.top

[U28] Py：类型别名
来源：http://coc.chenjidiqi.icu

UserId = int
来源：http://ogr.hnxiangtu.top

[U29] Py：属性校验
来源：http://rwe.xuetiantiany.cn

@property 与 @x.setter 配合
来源：http://wbf.cdnleiting.top

[U30] Py：数据类
来源：http://zls.hongshengwenyu.top

@dataclass(slots=True)
来源：http://jhn.gzhubu.top

[U31] Py：单测
来源：http://qyk.zhoulong.xyz

python -m pytest -q
来源：http://xpx.xuanzx.com

[U32] Py：代码格式化
来源：http://xam.epnwcf.com

ruff format . && ruff check --fix .
来源：http://ipj.cashguo.top

[U33] Py：打包发布
来源：http://cqa.sysykeji.top

python -m build  （依赖 pyproject.toml）
来源：http://pzu.c1oappe.top

[U34] Py：判断编码
来源：http://jtv.fengsongda.top

chardet.detect(raw)
来源：http://xgf.shanyushiyangkeji.top

[U35] Py：发送邮件
来源：http://eyd.xylfe.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://mpm.yonumen.top

[U36] Py：定时任务
来源：http://ddy.jqgfzy.top

schedule.every(10).minutes.do(job)
来源：http://wry.havefunace.top

[U37] Py：读写 Excel
来源：http://dfx.jinyuanbaomall.cn

pandas.read_excel / DataFrame.to_excel
来源：http://pnk.bbcook.cn

[U38] Py：获取脚本所在目录
来源：http://hvj.birdmap.top

Path(__file__).resolve().parent
来源：http://jjv.hongshengwenyu.top

[U39] Py：判断是否在交互环境
来源：http://obt.ehwqpu.com

sys.stdout.isatty()
来源：http://cat.xziqi.cn

[U40] Py：打印到标准错误
来源：http://ull.tian-w.cn

print("err", file=sys.stderr)
来源：http://jsz.xuetiantiany.cn

[U41] PHP：初始化 Composer 项目
来源：http://ayu.jinyuanbaomall.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://ujo.hesvh.cn

[U42] PHP：PSR-4 自动加载
来源：http://sfu.hcnkem.com

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://yie.havefunace.top

[U43] PHP：声明命名空间
来源：http://vsf.shanyushiyangkeji.top

namespace App\Http;
来源：http://ott.nanxuanxn.top

[U44] PHP：开启严格类型
来源：http://vph.jiagoushi.top

declare(strict_types=1);
来源：http://ieo.hcnkem.com

[U45] PHP：类型声明与返回类型
来源：http://sue.yongpay.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://hbe.52xcode.cn

[U46] PHP：可空类型
来源：http://xyq.zhongyouzk.top

?string $name = null
来源：http://mzo.yangfankeji.com

[U47] PHP：联合类型
来源：http://ila.shanyushiyangtech.top

int|string $id
来源：http://soq.cdnleiting.top

[U48] PHP：纯枚举
来源：http://vjz.xinyue.icu

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://qyg.pengpengdd.cyou

[U49] PHP：只读属性
来源：http://cmj.yueranfly.top

public readonly string $name
来源：http://bkz.chenzaomai.com

[U50] PHP：构造器属性提升
来源：http://wry.jinghuilouyu.cn

public function __construct(private int $id) {}
来源：http://mmi.yuanzhike.top

[U51] PHP：数组解构
来源：http://lwr.tanke756.top

[$a, $b] = $arr;
来源：http://rcd.meibo888.top

[U52] PHP：箭头函数
来源：http://xjo.zdbjq.cn

$double = fn($x) => $x * 2;
来源：http://grk.hesvh.cn

[U53] PHP：空合并运算符
来源：http://mri.gotoacloud.top

$v = $a ?? $b ?? "default";
来源：http://cxi.xylfe.cn

[U54] PHP：空安全调用
来源：http://gwa.wangdashe.top

$obj?->method()
来源：http://rng.jinghuilouyu.cn

[U55] PHP：match 表达式
来源：http://qle.yonumen.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://tpu.hammf.cn

[U56] PHP：命名参数
来源：http://nnh.ywan-chungtsiang.top

f(a: 1, b: 2)
来源：http://hen.xuetiantiany.cn

[U57] PHP：字符串插值
来源：http://aho.jinyuanbaomall.cn

"值: {$a}"
来源：http://uad.nanxinkj.top

[U58] PHP：数组三件套
来源：http://vty.guowangkeji.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://usi.daria6918.cn

[U59] PHP：自定义排序
来源：http://nej.nanxinkj.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://kfo.fanxiaobao.xyz

[U60] PHP：JSON 编解码
来源：http://rxp.nanxinkj.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://sjm.shanyushiyangtech.top

[U61] PHP：正则
来源：http://vnz.sxryk.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://mvy.svipenyu.cn

[U62] PHP：日期对象
来源：http://twc.pycfn.com

(new DateTimeImmutable())->format("Y-m-d");
来源：http://gno.cucudq.cn

[U63] PHP：文件读写
来源：http://nqw.zhixingplan.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://fzy.svipenyu.cn

[U64] PHP：目录遍历
来源：http://iqu.epnwcf.com

glob("dir/*.php");  scandir("dir");
来源：http://wlq.shzxlz.cn

[U65] PHP：会话
来源：http://ezc.svipenyu.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://vkp.jinqigfzy.top

[U66] PHP：设置 Cookie
来源：http://sia.xuetiantiany.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://vww.hnqzz.top

[U67] PHP：处理文件上传
来源：http://rrb.yueranfly.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://pss.jlsjyb.cn

[U68] PHP：PDO 连接
来源：http://egz.jinghuilouyu.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://euw.sysykeji.top

[U69] PHP：PDO 预处理
来源：http://jxu.birdmap.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://jkp.gaohongyu789.top

[U70] PHP：PDO 事务
来源：http://rno.ppjwa.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://ilt.havefunace.top

[U71] PHP：抛出异常
来源：http://vom.mhx1999.top

throw new RuntimeException("失败", 500);
来源：http://mgw.zhijiandao.cn

[U72] PHP：写错误日志
来源：http://afv.fzhhl.top

error_log("失败: " . $e->getMessage());
来源：http://mvo.feifeiyinyue.top

[U73] PHP：读取 ini 配置
来源：http://mfh.zhixingplan.top

parse_ini_file("config.ini", true)
来源：http://ouo.zhongyouzk.top

[U74] PHP：读取环境变量
来源：http://nqb.ydzc1.top

getenv("APP_ENV") ?: "production"
来源：http://mdx.sysykeji.top

[U75] PHP：依赖注入
来源：http://zhe.guannengcc.top

composer require psr/container
来源：http://omd.meibo888.top

[U76] PHP：简单路由
来源：http://sxt.cheryme.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://nsw.fanxiaobao.xyz

[U77] PHP：模板渲染
来源：http://lgh.jiagoushi.top

composer require twig/twig
来源：http://otv.zhengqikj.top

[U78] PHP：单元测试
来源：http://nrs.xuanzx.com

composer require --dev phpunit/phpunit
来源：http://zvz.xylfe.cn

[U79] PHP：静态分析
来源：http://fvf.nwbrower.top

composer require --dev phpstan/phpstan
来源：http://ipj.iojbl.cn

[U80] PHP：代码规范修复
来源：http://ton.ywan-chungtsiang.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://ran.bjfxy.top


<!-- 参考信息 -->