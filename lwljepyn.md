代发 wailian999

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://bot.pengpengdd.cyou

[S55] C++：结构化绑定
来源：http://lyf.yueranfly.top

auto [a, b] = std::make_pair(1, 2);
来源：http://tsw.xinyue.icu

[S56] C++：optional
来源：http://elp.zhijiandao.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://uuz.dashuyun.cn

[S57] C++：编译期常量
来源：http://hri.ywan-chungtsiang.top

constexpr int N = 10;
来源：http://tiz.fzhhl.top

[S58] C++：命名空间
来源：http://aju.shuidangran.top

namespace ns { int f() { return 1; } }
来源：http://yda.fengsongda.top

[S59] C++：静态断言
来源：http://mgk.jianghu66.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://ifk.yfazqb.com

[S60] C++：遍历并删除元素
来源：http://mlf.ppjwa.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://yva.jinqigfzy.top

================================================================================
来源：http://sss.chenlongwang.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://ucc.bbcook.cn

================================================================================
来源：http://jdz.daxiang520.top

[T01] Kotlin：Hello World
来源：http://dyb.zhongyouzk.top

println("Hello")
来源：http://nfd.pycfn.com

[T02] Kotlin：变量
来源：http://fut.fengsongda.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://dxv.cheryme.top

[T03] Kotlin：字符串模板
来源：http://ayp.cheryme.top

"值: $b"
来源：http://izc.cqqwz.cn

[T04] Kotlin：空安全
来源：http://lkw.shanyushiyangkeji.top

val n: String? = null;  n?.length
来源：http://vih.vqdsnc.cn

[T05] Kotlin：when 表达式
来源：http://zrn.chenzaomai.com

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://ibv.jianghu66.top

[T06] Kotlin：集合映射
来源：http://spr.zdqjudy.top

listOf(1, 2, 3).map { it * 2 }
来源：http://alf.hywenlv.cn

[T07] Kotlin：集合过滤
来源：http://ltr.dashuyun.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://pnc.hywenlv.cn

[T08] Kotlin：数据类
来源：http://gdt.gogol.net.cn

data class User(val name: String, val age: Int)
来源：http://qjw.bjfxy.top

[T09] Kotlin：扩展函数
来源：http://xpi.ppjwa.cn

fun String.exclaim() = this + "!"
来源：http://xxi.yj202588.top

[T10] Kotlin：默认参数
来源：http://det.wangdashe.top

fun greet(name: String = "World") = "Hi $name"
来源：http://ajh.c1oappe.top

[T11] Kotlin：协程
来源：http://fnm.fehbvm.com

GlobalScope.launch { delay(1000); println("done") }
来源：http://uco.sjlbkw.cn

[T12] Kotlin：解构声明
来源：http://fyi.yangfankeji.com

val (a, b) = Pair(1, 2)
来源：http://lgq.wangdashe.top

[T13] Kotlin：只读 Map
来源：http://jbw.wangshuangyany.cn

val m = mapOf("a" to 1)
来源：http://zan.fehbvm.com

[T14] Kotlin：循环
来源：http://fgj.zhaomingkeji.xyz

for (i in 1..10) println(i)
来源：http://kox.yanxiufei.cn

[T15] Kotlin：接口
来源：http://nsi.fengsongda.top

interface Shape { fun area(): Double }
来源：http://tzh.xingfuxueyuan.xyz

[T16] Swift：Hello World
来源：http://cha.yuxming.cn

print("Hello")
来源：http://kcu.quarkkingdee.top

[T17] Swift：变量与常量
来源：http://tro.ctjpmb.com

var a = 1;  let b = 2
来源：http://kiz.ywan-chungtsiang.top

[T18] Swift：字符串插值
来源：http://jhu.yongpay.top

"值: \(b)"
来源：http://mrd.wangshuangyany.cn

[T19] Swift：可选绑定
来源：http://vaa.sufxvd.cn

if let n = opt { print(n) }
来源：http://kvy.52xcode.cn

[T20] Swift：数组操作
来源：http://iif.daria6918.cn

var a = [1, 2, 3];  a.append(4)
来源：http://faw.ywan-chungtsiang.top

[T21] Swift：遍历
来源：http://jlh.yongpay.top

for x in a { print(x) }
来源：http://fax.epnwcf.com

[T22] Swift：字典
来源：http://psa.aizwys.cn

var d = ["a": 1];  d["b"] = 2
来源：http://iel.yangfankeji.com

[T23] Swift：函数
来源：http://ewk.yj20258888.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://glh.xuetiantiany.cn

[T24] Swift：闭包
来源：http://gix.yonumen.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://yrk.hcnkem.com

[T25] Swift：结构体
来源：http://qjw.ywan-chungtsiang.top

struct P { var x: Int }
来源：http://inv.wangdashe.top

[T26] Swift：类与重写
来源：http://eir.redwolf501.top

class A: Base { override func f() {} }
来源：http://nfc.cheryme.top

[T27] Swift：错误处理
来源：http://nfg.yfazqb.com

do { try f() } catch { print(error) }
来源：http://ejq.nanxinkj.top

[T28] Swift：枚举
来源：http://tnv.zhijiandao.cn

enum Color { case red, green }
来源：http://lqg.shangyingyoupin.top

[T29] Swift：guard 提前返回
来源：http://upr.bjfxy.top

guard let x = opt else { return }
来源：http://jjp.hfpthk.cn

[T30] Swift：协议
来源：http://hln.cashguo.top

protocol Shape { func area() -> Double }
来源：http://toi.tian-w.cn

[T31] Lua：Hello World
来源：http://asr.nanxuanxn.top

print("Hello")
来源：http://fhs.shzxlz.cn

[T32] Lua：局部变量
来源：http://kra.uphjek.com

local a = 1
来源：http://wiu.nwbrower.top

[T33] Lua：表（数组）
来源：http://ozz.havefunace.top

local t = {1, 2, 3};  t[4] = 4
来源：http://edc.zhongyouzk.top

[T34] Lua：遍历表
来源：http://mef.hywenlv.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://whg.fzhhl.top

[T35] Lua：字典表
来源：http://zww.fanxiaobao.xyz

local d = { a = 1 };  d.b = 2
来源：http://gik.52xcode.cn

[T36] Lua：函数
来源：http://age.jqgfzy.top

function add(a, b) return a + b end
来源：http://djn.dianchejie.cn

[T37] Lua：字符串拼接
来源：http://xdv.nanxinkj.top

"a" .. "b"
来源：http://bxx.yangfankeji.com

[T38] Lua：条件
来源：http://ubd.c1oappe.top

if x > 0 then print("正") end
来源：http://rvg.redwolf501.top

[T39] Lua：模式匹配
来源：http://mbo.zhijiandao.cn

string.find(s, "%d+")
来源：http://uhq.jqgfzy.top

[T40] Lua：元表
来源：http://dwq.yonumen.top

setmetatable({}, { __index = base })
来源：http://xol.cashguo.top

[T41] Perl：Hello World
来源：http://gvv.fanxiaobao.xyz

print "Hello\n";
来源：http://wic.meibo888.top

[T42] Perl：变量类型
来源：http://jwt.jinqigufen.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://prf.cucudq.cn

[T43] Perl：字符串插值
来源：http://zga.jyoumei.cn

"值: $a"
来源：http://hlf.jiagoushi.top

[T44] Perl：条件
来源：http://mpa.ivvv.top

if ($a > 0) { print "正"; }
来源：http://cyh.chenlongwang.top

[T45] Perl：数组遍历
来源：http://zak.yueranfly.top

for my $x (@arr) { print $x; }
来源：http://sce.gogol.net.cn

[T46] Perl：哈希操作
来源：http://wgo.jinghuilouyu.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://asb.shangyingyoupin.top

[T47] Perl：正则捕获
来源：http://utk.chenzaomai.com

if ($s =~ /(\d+)/) { print $1; }
来源：http://iju.yongpay.top

[T48] Perl：正则替换
来源：http://ula.jinyuanbaomall.cn

$s =~ s/old/new/g;
来源：http://vid.daria6918.cn

[T49] Perl：函数
来源：http://ljn.guowangkeji.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://cvg.yvedp.cn

[T50] Perl：逐行读文件
来源：http://zpl.cucudq.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://uba.9152youxi.cn

while (my $line = <$fh>) { print $line; }
来源：http://fvf.quarkkingdee.top

[T51] Scala：Hello World
来源：http://mlz.ctjpmb.com

println("Hello")
来源：http://fci.ctjpmb.com

[T52] Scala：变量
来源：http://uzt.yongpay.top

val a = 1;  var b = 2
来源：http://cza.zhaomingkeji.xyz

[T53] Scala：字符串插值
来源：http://fgp.bbcook.cn

s"值: $b"
来源：http://vpd.zhongyouzk.top

[T54] Scala：集合映射
来源：http://uwf.zdqjudy.top

List(1, 2, 3).map(_ * 2)
来源：http://lij.yongpay.top

[T55] Scala：集合过滤
来源：http://mot.hywenlv.cn

List(1, 2, 3).filter(_ > 1)
来源：http://hrg.yj20258.top

[T56] Scala：样例类
来源：http://fdd.bjfxy.top

case class User(name: String, age: Int)
来源：http://gmo.0kj1m.cn

[T57] Scala：模式匹配
来源：http://hcj.andypj.xyz

x match { case 1 => "一"; case _ => "其他" }
来源：http://ndo.zdqjudy.top

[T58] Scala：函数定义
来源：http://vdb.zhixingplan.top

def add(a: Int, b: Int): Int = a + b
来源：http://yqv.jinqigufen.top

[T59] Scala：循环
来源：http://kka.jinqigufen.top

for (i <- 1 to 10) println(i)
来源：http://zlb.xuetiantiany.cn

[T60] Scala：折叠
来源：http://aoj.daria6918.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://kxs.zhongyouzk.top

================================================================================
来源：http://npx.yanxiufei.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://lbf.jiagoushi.top

================================================================================
来源：http://ley.xuetiantiany.cn

[U01] Py：创建虚拟环境
来源：http://elp.hysaishi.cn

python -m venv .venv && source .venv/bin/activate
来源：http://mdk.jinqigfzy.top

[U02] Py：导出 / 安装依赖
来源：http://vru.tanke756.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://wkt.yj202588.top

[U03] Py：加载 .env 配置
来源：http://ydh.redwolf501.top

from dotenv import load_dotenv; load_dotenv()
来源：http://stn.yongpay.top

[U04] Py：变量调试打印
来源：http://rwa.mhx1999.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://tkm.xuanzx.com

[U05] Py：列表去重且保序
来源：http://jhc.zhijiandao.cn

list(dict.fromkeys(arr))
来源：http://liv.jinqigfzy.top

[U06] Py：合并两个字典
来源：http://arb.yuanzhike.top

{**a, **b}
来源：http://ikr.guowangkeji.top

[U07] Py：反转字典键值
来源：http://saf.dianchejie.cn

{v: k for k, v in d.items()}
来源：http://tog.sufxvd.cn

[U08] Py：展平二维列表
来源：http://hyf.yvedp.cn

[y for x in nested for y in x]
来源：http://nsx.jlsjyb.cn

[U09] Py：字典取最大值的键
来源：http://exw.gogol.net.cn

max(d, key=d.get)
来源：http://ppn.zdqjudy.top

[U10] Py：按值排序字典
来源：http://pyg.zdbjq.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://deg.daxiang520.top

[U11] Py：生成器表达式
来源：http://ixw.zhoulong.xyz

(x * 2 for x in arr)
来源：http://yas.xinyue.icu

[U12] Py：取出现最多的 3 个元素
来源：http://cat.ppjwa.cn

Counter(arr).most_common(3)
来源：http://hvr.wangdashe.top

[U13] Py：固定长度队列
来源：http://til.birdmap.top

deque(maxlen=10)
来源：http://otx.dianchejie.cn

[U14] Py：分组收集到列表
来源：http://hmm.jinghuilouyu.cn

defaultdict(list)
来源：http://qrh.xinyue.icu

[U15] Py：高精度计时
来源：http://hel.ppjwa.cn

t = time.perf_counter()
来源：http://jtt.yj20258888.top

[U16] Py：命令行参数解析
来源：http://hcm.shzxlz.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://ybv.tian-w.cn

[U17] Py：初始化日志
来源：http://fxx.hongshengwenyu.top

logging.basicConfig(level=logging.INFO)
来源：http://cmg.tarul.cn

[U18] Py：预编译正则
来源：http://xoh.jinyuanbaomall.cn

pat = re.compile(r"\d+")
来源：http://vfz.hysaishi.cn

[U19] Py：正则替换带回调
来源：http://rhv.nwbrower.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://mmy.andypj.xyz

[U20] Py：缓存函数结果
来源：http://fux.fehbvm.com

@functools.lru_cache(maxsize=None)
来源：http://ncl.wangshuangyany.cn

[U21] Py：自定义上下文管理器
来源：http://gcn.xylfe.cn

@contextlib.contextmanager
来源：http://eem.fanxiaobao.xyz

[U22] Py：矩阵转置
来源：http://lec.ppjwa.cn

list(zip(*m))
来源：http://qav.cdnleiting.top

[U23] Py：分块读取大文件
来源：http://yox.shuidangran.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://sga.xylfe.cn

[U24] Py：路径操作
来源：http://uax.epnwcf.com

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://zrz.aibaodan.cn

[U25] Py：CSV 按字典读
来源：http://jph.yueranfly.top

csv.DictReader(f)
来源：http://fkz.shanyushiyangkeji.top

[U26] Py：并发下载
来源：http://egf.zhoulong.xyz

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://xii.redwolf501.top

[U27] Py：异步 HTTP
来源：http://rju.daria6918.cn

aiohttp.ClientSession() 配合 async with
来源：http://bee.vqdsnc.cn

[U28] Py：类型别名
来源：http://jgu.cucudq.cn

UserId = int
来源：http://rth.yj20258.top

[U29] Py：属性校验
来源：http://jxt.ywan-chungtsiang.top

@property 与 @x.setter 配合
来源：http://eqf.hywenlv.cn

[U30] Py：数据类
来源：http://ema.shanyushiyangtech.top

@dataclass(slots=True)
来源：http://dsg.bbcook.cn

[U31] Py：单测
来源：http://qhb.sjlbkw.cn

python -m pytest -q
来源：http://tei.tarul.cn

[U32] Py：代码格式化
来源：http://iiw.zdbjq.cn

ruff format . && ruff check --fix .
来源：http://nau.ppjwa.cn

[U33] Py：打包发布
来源：http://xnh.cdnleiting.top

python -m build  （依赖 pyproject.toml）
来源：http://zph.9152youxi.cn

[U34] Py：判断编码
来源：http://qhb.xinyue.icu

chardet.detect(raw)
来源：http://fii.jinyuanbaomall.cn

[U35] Py：发送邮件
来源：http://rut.mhx1999.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://ylz.cheryme.top

[U36] Py：定时任务
来源：http://qcn.sysykeji.top

schedule.every(10).minutes.do(job)
来源：http://kxf.gogol.net.cn

[U37] Py：读写 Excel
来源：http://llu.yanxiufei.cn

pandas.read_excel / DataFrame.to_excel
来源：http://sqf.sjlbkw.cn

[U38] Py：获取脚本所在目录
来源：http://gph.cucudq.cn

Path(__file__).resolve().parent
来源：http://xri.chenzaomai.com

[U39] Py：判断是否在交互环境
来源：http://tdg.tian-w.cn

sys.stdout.isatty()
来源：http://fqj.shanyushiyangkeji.top

[U40] Py：打印到标准错误
来源：http://gzn.ehwqpu.com

print("err", file=sys.stderr)
来源：http://pmd.yuxming.cn

[U41] PHP：初始化 Composer 项目
来源：http://ile.feifeiyinyue.top

composer init;  composer require guzzlehttp/guzzle
来源：http://mkt.yj20258.top

[U42] PHP：PSR-4 自动加载
来源：http://ohy.jqgufenzy.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://euz.shangyingyoupin.top

[U43] PHP：声明命名空间
来源：http://idx.yuxming.cn

namespace App\Http;
来源：http://sxi.birdmap.top

[U44] PHP：开启严格类型
来源：http://eie.jinqigufen.top

declare(strict_types=1);
来源：http://jhq.xingfuxueyuan.xyz

[U45] PHP：类型声明与返回类型
来源：http://aeh.ivvv.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://oim.cashguo.top

[U46] PHP：可空类型
来源：http://myp.fktsv.cn

?string $name = null
来源：http://vrw.sweek.top

[U47] PHP：联合类型
来源：http://eba.ydjk.org.cn

int|string $id
来源：http://ccz.zhongyouzk.top

[U48] PHP：纯枚举
来源：http://cmx.gzhubu.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://iez.kuanghao11.cn

[U49] PHP：只读属性
来源：http://cok.gogol.net.cn

public readonly string $name
来源：http://tpg.bbcook.cn

[U50] PHP：构造器属性提升
来源：http://ymf.hongshengwenyu.top

public function __construct(private int $id) {}
来源：http://nhl.dashuyun.cn

[U51] PHP：数组解构
来源：http://avc.chenjidiqi.icu

[$a, $b] = $arr;
来源：http://efx.ctjpmb.com

[U52] PHP：箭头函数
来源：http://shs.jianghu66.top

$double = fn($x) => $x * 2;
来源：http://kri.jlsjyb.cn

[U53] PHP：空合并运算符
来源：http://fpx.cdnleiting.top

$v = $a ?? $b ?? "default";
来源：http://bon.iojbl.cn

[U54] PHP：空安全调用
来源：http://emk.zhiwuduotai.top

$obj?->method()
来源：http://ttv.aibaodan.cn

[U55] PHP：match 表达式
来源：http://hld.yj20258888.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://ove.tanke756.top

[U56] PHP：命名参数
来源：http://pve.sweek.top

f(a: 1, b: 2)
来源：http://qrh.ydzc1.top

[U57] PHP：字符串插值
来源：http://kfu.chenzaomai.com

"值: {$a}"
来源：http://zyv.pengpengdd.cyou

[U58] PHP：数组三件套
来源：http://gyx.chenlongwang.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://sub.c1oappe.top

[U59] PHP：自定义排序
来源：http://vzn.cheryme.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://tli.yvedp.cn

[U60] PHP：JSON 编解码
来源：http://iky.jyoumei.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://pej.yj20258.top

[U61] PHP：正则
来源：http://vhb.hfpthk.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://zpm.tian-w.cn

[U62] PHP：日期对象
来源：http://gbg.tianlin.xyz

(new DateTimeImmutable())->format("Y-m-d");
来源：http://jzr.hnxiangtu.top

[U63] PHP：文件读写
来源：http://yrw.chenzaomai.com

file_get_contents($f);  file_put_contents($f, $data);
来源：http://nwj.fzhhl.top

[U64] PHP：目录遍历
来源：http://nbu.zhixingplan.top

glob("dir/*.php");  scandir("dir");
来源：http://dtl.aizwys.cn

[U65] PHP：会话
来源：http://glj.shanyushiyangtech.top

session_start();  $_SESSION["uid"] = 1;
来源：http://dgf.yuxming.cn

[U66] PHP：设置 Cookie
来源：http://rmq.zhixingplan.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://qnd.hysaishi.cn

[U67] PHP：处理文件上传
来源：http://kmq.hysaishi.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://npm.dianchejie.cn

[U68] PHP：PDO 连接
来源：http://jbr.hnqzz.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://jny.9152youxi.cn

[U69] PHP：PDO 预处理
来源：http://bpg.jinqigufen.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://xrj.zhoulong.xyz

[U70] PHP：PDO 事务
来源：http://zvb.jinghuilouyu.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://vhx.0kj1m.cn

[U71] PHP：抛出异常
来源：http://klq.9152youxi.cn

throw new RuntimeException("失败", 500);
来源：http://hqa.ywan-chungtsiang.top

[U72] PHP：写错误日志
来源：http://xug.yfazqb.com

error_log("失败: " . $e->getMessage());
来源：http://xoy.xuanzx.com

[U73] PHP：读取 ini 配置
来源：http://zia.gaohongyu789.top

parse_ini_file("config.ini", true)
来源：http://ove.smart0.xyz

[U74] PHP：读取环境变量
来源：http://mrn.jinqigfzy.top

getenv("APP_ENV") ?: "production"
来源：http://gjj.yuxming.cn

[U75] PHP：依赖注入
来源：http://gbz.cdnleiting.top

composer require psr/container
来源：http://pno.yonumen.top

[U76] PHP：简单路由
来源：http://coc.nanxuanxn.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://xya.ehwqpu.com

[U77] PHP：模板渲染
来源：http://zsm.ydjk.org.cn

composer require twig/twig
来源：http://csv.zhaomingkeji.xyz

[U78] PHP：单元测试
来源：http://mzx.yangfankeji.com

composer require --dev phpunit/phpunit
来源：http://spq.9152youxi.cn

[U79] PHP：静态分析
来源：http://oht.jlsjyb.cn

composer require --dev phpstan/phpstan
来源：http://non.jlsjyb.cn

[U80] PHP：代码规范修复
来源：http://dey.bjfxy.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://gzx.svipenyu.cn


<!-- 参考信息 -->