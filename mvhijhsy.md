代发 wailian999

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wzl.xingfuxueyuan.xyz

[S57] C++：编译期常量
来源：http://hts.jiagoushi.top

constexpr int N = 10;
来源：http://jdy.316326.xyz

[S58] C++：命名空间
来源：http://wib.cdnleiting.top

namespace ns { int f() { return 1; } }
来源：http://wet.jiagoushi.top

[S59] C++：静态断言
来源：http://wao.ctjpmb.com

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://icv.cucudq.cn

[S60] C++：遍历并删除元素
来源：http://ozg.hesvh.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://luw.snrcjt.cn

================================================================================
来源：http://kdg.quarkkingdee.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://xta.wangshuangyany.cn

================================================================================
来源：http://gzz.ydjk.org.cn

[T01] Kotlin：Hello World
来源：http://vzu.haohaochexian.top

println("Hello")
来源：http://mlu.nwbrower.top

[T02] Kotlin：变量
来源：http://zyo.quarkkingdee.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://poo.shanyushiyangtech.top

[T03] Kotlin：字符串模板
来源：http://ewx.sysykeji.top

"值: $b"
来源：http://wej.yuxming.cn

[T04] Kotlin：空安全
来源：http://nwr.nwbrower.top

val n: String? = null;  n?.length
来源：http://voo.zdqjudy.top

[T05] Kotlin：when 表达式
来源：http://lbd.xziqi.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://dom.tian-w.cn

[T06] Kotlin：集合映射
来源：http://cfp.tanke756.top

listOf(1, 2, 3).map { it * 2 }
来源：http://fji.wangdashe.top

[T07] Kotlin：集合过滤
来源：http://oze.hfpthk.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://oji.quarkkingdee.top

[T08] Kotlin：数据类
来源：http://uae.fanxiaobao.xyz

data class User(val name: String, val age: Int)
来源：http://mmm.yueranfly.top

[T09] Kotlin：扩展函数
来源：http://yfe.zhengqikj.top

fun String.exclaim() = this + "!"
来源：http://eeu.dashuyun.cn

[T10] Kotlin：默认参数
来源：http://jaf.ybcxt.top

fun greet(name: String = "World") = "Hi $name"
来源：http://oxy.c1oappe.top

[T11] Kotlin：协程
来源：http://tcg.nwbrower.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://iuq.zhongyouzk.top

[T12] Kotlin：解构声明
来源：http://yzl.ivvv.top

val (a, b) = Pair(1, 2)
来源：http://hbm.hongshengwenyu.top

[T13] Kotlin：只读 Map
来源：http://rxd.yfazqb.com

val m = mapOf("a" to 1)
来源：http://lpt.tianlin.xyz

[T14] Kotlin：循环
来源：http://xwl.yuanzhike.top

for (i in 1..10) println(i)
来源：http://agb.hammf.cn

[T15] Kotlin：接口
来源：http://aol.ppjwa.cn

interface Shape { fun area(): Double }
来源：http://nzq.yj202588.top

[T16] Swift：Hello World
来源：http://ptc.gotoacloud.top

print("Hello")
来源：http://cdm.52xcode.cn

[T17] Swift：变量与常量
来源：http://juj.tian-w.cn

var a = 1;  let b = 2
来源：http://ora.hongshengwenyu.top

[T18] Swift：字符串插值
来源：http://vmh.hcnkem.com

"值: \(b)"
来源：http://skd.yueranfly.top

[T19] Swift：可选绑定
来源：http://gew.fehbvm.com

if let n = opt { print(n) }
来源：http://qjz.gaohongyu789.top

[T20] Swift：数组操作
来源：http://kpz.chenlongwang.top

var a = [1, 2, 3];  a.append(4)
来源：http://rob.52xcode.cn

[T21] Swift：遍历
来源：http://ezz.havefunace.top

for x in a { print(x) }
来源：http://xuv.dashuyun.cn

[T22] Swift：字典
来源：http://gxa.xinyue.icu

var d = ["a": 1];  d["b"] = 2
来源：http://ekm.zhoulong.xyz

[T23] Swift：函数
来源：http://mtk.nanxuanxn.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://dgs.zhongyouzk.top

[T24] Swift：闭包
来源：http://kfi.nwbrower.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://knd.yanxiufei.cn

[T25] Swift：结构体
来源：http://pot.cheryme.top

struct P { var x: Int }
来源：http://eww.ydzc1.top

[T26] Swift：类与重写
来源：http://bqb.nwbrower.top

class A: Base { override func f() {} }
来源：http://rie.xingfuxueyuan.xyz

[T27] Swift：错误处理
来源：http://uas.fanxiaobao.xyz

do { try f() } catch { print(error) }
来源：http://clp.daria6918.cn

[T28] Swift：枚举
来源：http://apc.snrcjt.cn

enum Color { case red, green }
来源：http://uje.shangyingyoupin.top

[T29] Swift：guard 提前返回
来源：http://veo.shzxlz.cn

guard let x = opt else { return }
来源：http://vhl.cqqwz.cn

[T30] Swift：协议
来源：http://wjw.daria6918.cn

protocol Shape { func area() -> Double }
来源：http://oxf.zdbjq.cn

[T31] Lua：Hello World
来源：http://rou.xuetiantiany.cn

print("Hello")
来源：http://bnk.xuanzx.com

[T32] Lua：局部变量
来源：http://grw.yangfankeji.com

local a = 1
来源：http://jfe.daria6918.cn

[T33] Lua：表（数组）
来源：http://thq.ivvv.top

local t = {1, 2, 3};  t[4] = 4
来源：http://sna.yonumen.top

[T34] Lua：遍历表
来源：http://cfx.cashguo.top

for i, v in ipairs(t) do print(i, v) end
来源：http://htz.hywenlv.cn

[T35] Lua：字典表
来源：http://mlb.sxryk.cn

local d = { a = 1 };  d.b = 2
来源：http://qkx.wangdashe.top

[T36] Lua：函数
来源：http://lqj.haohaochexian.top

function add(a, b) return a + b end
来源：http://hdb.daria6918.cn

[T37] Lua：字符串拼接
来源：http://gwf.jinyuanbaomall.cn

"a" .. "b"
来源：http://cid.wangdashe.top

[T38] Lua：条件
来源：http://vxn.gzhubu.top

if x > 0 then print("正") end
来源：http://cwx.zhijiandao.cn

[T39] Lua：模式匹配
来源：http://eqo.nwbrower.top

string.find(s, "%d+")
来源：http://rhz.jyoumei.cn

[T40] Lua：元表
来源：http://rdc.hammf.cn

setmetatable({}, { __index = base })
来源：http://esg.chenjidiqi.icu

[T41] Perl：Hello World
来源：http://lpu.ywan-chungtsiang.top

print "Hello\n";
来源：http://alw.quarkkingdee.top

[T42] Perl：变量类型
来源：http://baf.fanxiaobao.xyz

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://ifd.hnqzz.top

[T43] Perl：字符串插值
来源：http://qdt.kuanghao11.cn

"值: $a"
来源：http://tgx.sweek.top

[T44] Perl：条件
来源：http://qrh.shangyingyoupin.top

if ($a > 0) { print "正"; }
来源：http://ete.zdqjudy.top

[T45] Perl：数组遍历
来源：http://rou.cqqwz.cn

for my $x (@arr) { print $x; }
来源：http://eqh.aibaodan.cn

[T46] Perl：哈希操作
来源：http://ifa.zhaomingkeji.xyz

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://mzw.epnwcf.com

[T47] Perl：正则捕获
来源：http://rjj.chenlongwang.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://jfe.xingfuxueyuan.xyz

[T48] Perl：正则替换
来源：http://xoz.sysykeji.top

$s =~ s/old/new/g;
来源：http://ybi.ivvv.top

[T49] Perl：函数
来源：http://bqq.zdqjudy.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://zni.jinghuilouyu.cn

[T50] Perl：逐行读文件
来源：http://qqd.cashguo.top

open my $fh, "<", "a.txt" or die $!;
来源：http://lcq.aizwys.cn

while (my $line = <$fh>) { print $line; }
来源：http://fgg.gogol.net.cn

[T51] Scala：Hello World
来源：http://wvv.cashguo.top

println("Hello")
来源：http://czb.jqgfzy.top

[T52] Scala：变量
来源：http://aiw.cheryme.top

val a = 1;  var b = 2
来源：http://tuv.shanyushiyangtech.top

[T53] Scala：字符串插值
来源：http://pyq.zhongyouzk.top

s"值: $b"
来源：http://ujb.0kj1m.cn

[T54] Scala：集合映射
来源：http://let.quarkkingdee.top

List(1, 2, 3).map(_ * 2)
来源：http://zoi.nanxinkj.top

[T55] Scala：集合过滤
来源：http://vks.shzxlz.cn

List(1, 2, 3).filter(_ > 1)
来源：http://xys.cheryme.top

[T56] Scala：样例类
来源：http://ptj.zhongyouzk.top

case class User(name: String, age: Int)
来源：http://gmq.jlsjyb.cn

[T57] Scala：模式匹配
来源：http://bau.sysykeji.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://kbq.daria6918.cn

[T58] Scala：函数定义
来源：http://xsu.zhijiandao.cn

def add(a: Int, b: Int): Int = a + b
来源：http://jel.nwbrower.top

[T59] Scala：循环
来源：http://xbn.shuidangran.top

for (i <- 1 to 10) println(i)
来源：http://ekp.zdbjq.cn

[T60] Scala：折叠
来源：http://ucc.9152youxi.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://oug.fehbvm.com

================================================================================
来源：http://dnb.cdnleiting.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://bgo.zdqjudy.top

================================================================================
来源：http://qgr.jinyuanbaomall.cn

[U01] Py：创建虚拟环境
来源：http://ktv.ehwqpu.com

python -m venv .venv && source .venv/bin/activate
来源：http://aim.jinghuilouyu.cn

[U02] Py：导出 / 安装依赖
来源：http://dwp.hfpthk.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://kba.xingfuxueyuan.xyz

[U03] Py：加载 .env 配置
来源：http://fbd.yuanzhike.top

from dotenv import load_dotenv; load_dotenv()
来源：http://vgn.nanxuanxn.top

[U04] Py：变量调试打印
来源：http://lph.cucudq.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://ali.ydzc1.top

[U05] Py：列表去重且保序
来源：http://wud.havefunace.top

list(dict.fromkeys(arr))
来源：http://oxn.52xcode.cn

[U06] Py：合并两个字典
来源：http://akt.sjlbkw.cn

{**a, **b}
来源：http://vgb.zhaomingkeji.xyz

[U07] Py：反转字典键值
来源：http://msb.guowangkeji.top

{v: k for k, v in d.items()}
来源：http://ygk.hammf.cn

[U08] Py：展平二维列表
来源：http://eap.ydzc1.top

[y for x in nested for y in x]
来源：http://oko.snrcjt.cn

[U09] Py：字典取最大值的键
来源：http://tqo.yfazqb.com

max(d, key=d.get)
来源：http://iyx.cdnleiting.top

[U10] Py：按值排序字典
来源：http://nlx.nanxuanxn.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://rve.yfazqb.com

[U11] Py：生成器表达式
来源：http://xnx.yongpay.top

(x * 2 for x in arr)
来源：http://qvs.hongshengwenyu.top

[U12] Py：取出现最多的 3 个元素
来源：http://knq.epnwcf.com

Counter(arr).most_common(3)
来源：http://fqz.yueranfly.top

[U13] Py：固定长度队列
来源：http://olw.jianghu66.top

deque(maxlen=10)
来源：http://fem.bjfxy.top

[U14] Py：分组收集到列表
来源：http://ehr.c1oappe.top

defaultdict(list)
来源：http://ozr.nwbrower.top

[U15] Py：高精度计时
来源：http://qhf.snrcjt.cn

t = time.perf_counter()
来源：http://fbd.snrcjt.cn

[U16] Py：命令行参数解析
来源：http://pat.mhx1999.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://xph.yongpay.top

[U17] Py：初始化日志
来源：http://xdq.xylfe.cn

logging.basicConfig(level=logging.INFO)
来源：http://ofr.sweek.top

[U18] Py：预编译正则
来源：http://msb.shangyingyoupin.top

pat = re.compile(r"\d+")
来源：http://niu.hnxiangtu.top

[U19] Py：正则替换带回调
来源：http://dad.hongshengwenyu.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://isj.shangyingyoupin.top

[U20] Py：缓存函数结果
来源：http://tca.ydzc1.top

@functools.lru_cache(maxsize=None)
来源：http://oez.hnqzz.top

[U21] Py：自定义上下文管理器
来源：http://dsw.nanxuanxn.top

@contextlib.contextmanager
来源：http://jhc.andypj.xyz

[U22] Py：矩阵转置
来源：http://inn.jqgufenzy.top

list(zip(*m))
来源：http://yqo.yonumen.top

[U23] Py：分块读取大文件
来源：http://rgz.jiagoushi.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://jiv.jinyuanbaomall.cn

[U24] Py：路径操作
来源：http://gug.yuanzhike.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://drs.aibaodan.cn

[U25] Py：CSV 按字典读
来源：http://stq.xinyue.icu

csv.DictReader(f)
来源：http://jvf.ydjk.org.cn

[U26] Py：并发下载
来源：http://gtb.zhongyouzk.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://ees.cucudq.cn

[U27] Py：异步 HTTP
来源：http://haf.zycfv.cn

aiohttp.ClientSession() 配合 async with
来源：http://bts.xingfuxueyuan.xyz

[U28] Py：类型别名
来源：http://tms.vehdjk.com

UserId = int
来源：http://cmd.zhengqikj.top

[U29] Py：属性校验
来源：http://lkd.gogol.net.cn

@property 与 @x.setter 配合
来源：http://ism.bjfxy.top

[U30] Py：数据类
来源：http://pjk.hammf.cn

@dataclass(slots=True)
来源：http://sac.tarul.cn

[U31] Py：单测
来源：http://cpx.zhongyouzk.top

python -m pytest -q
来源：http://sgc.xuetiantiany.cn

[U32] Py：代码格式化
来源：http://pyp.bbcook.cn

ruff format . && ruff check --fix .
来源：http://bum.jqgfzy.top

[U33] Py：打包发布
来源：http://atr.chenjidiqi.icu

python -m build  （依赖 pyproject.toml）
来源：http://lll.chenlongwang.top

[U34] Py：判断编码
来源：http://tux.xingfuxueyuan.xyz

chardet.detect(raw)
来源：http://ach.hysaishi.cn

[U35] Py：发送邮件
来源：http://yfz.ywan-chungtsiang.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://sxe.nwbrower.top

[U36] Py：定时任务
来源：http://tqi.dianchejie.cn

schedule.every(10).minutes.do(job)
来源：http://pap.xinyue.icu

[U37] Py：读写 Excel
来源：http://tuu.guannengcc.top

pandas.read_excel / DataFrame.to_excel
来源：http://jae.ydzc1.top

[U38] Py：获取脚本所在目录
来源：http://rqg.gogol.net.cn

Path(__file__).resolve().parent
来源：http://fpc.xylfe.cn

[U39] Py：判断是否在交互环境
来源：http://lzw.tianlin.xyz

sys.stdout.isatty()
来源：http://geu.sxryk.cn

[U40] Py：打印到标准错误
来源：http://wgg.jianghu66.top

print("err", file=sys.stderr)
来源：http://hnl.316326.xyz

[U41] PHP：初始化 Composer 项目
来源：http://bwr.andypj.xyz

composer init;  composer require guzzlehttp/guzzle
来源：http://ifi.yanxiufei.cn

[U42] PHP：PSR-4 自动加载
来源：http://ypv.yanxiufei.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://kic.birdmap.top

[U43] PHP：声明命名空间
来源：http://pth.dianchejie.cn

namespace App\Http;
来源：http://tzp.xylfe.cn

[U44] PHP：开启严格类型
来源：http://ktf.nwbrower.top

declare(strict_types=1);
来源：http://ced.cqqwz.cn

[U45] PHP：类型声明与返回类型
来源：http://nbe.daria6918.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://ehl.sxryk.cn

[U46] PHP：可空类型
来源：http://vqk.fanxiaobao.xyz

?string $name = null
来源：http://iyu.tarul.cn

[U47] PHP：联合类型
来源：http://hwh.yonumen.top

int|string $id
来源：http://fcm.ehwqpu.com

[U48] PHP：纯枚举
来源：http://yed.yongpay.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://qrw.wangdashe.top

[U49] PHP：只读属性
来源：http://nhk.sxryk.cn

public readonly string $name
来源：http://prz.chenjidiqi.icu

[U50] PHP：构造器属性提升
来源：http://kuc.uphjek.com

public function __construct(private int $id) {}
来源：http://avq.jyoumei.cn

[U51] PHP：数组解构
来源：http://bgo.fktsv.cn

[$a, $b] = $arr;
来源：http://czq.zycfv.cn

[U52] PHP：箭头函数
来源：http://ise.yj20258888.top

$double = fn($x) => $x * 2;
来源：http://gic.meibo888.top

[U53] PHP：空合并运算符
来源：http://wws.pycfn.com

$v = $a ?? $b ?? "default";
来源：http://oeg.cqqwz.cn

[U54] PHP：空安全调用
来源：http://tkg.meibo888.top

$obj?->method()
来源：http://zsm.jinghuilouyu.cn

[U55] PHP：match 表达式
来源：http://xnv.vqdsnc.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://non.jiagoushi.top

[U56] PHP：命名参数
来源：http://edf.9152youxi.cn

f(a: 1, b: 2)
来源：http://mfh.nanxinkj.top

[U57] PHP：字符串插值
来源：http://fus.jiagoushi.top

"值: {$a}"
来源：http://hnz.yj20258888.top

[U58] PHP：数组三件套
来源：http://ray.jlsjyb.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://xst.zhijiandao.cn

[U59] PHP：自定义排序
来源：http://kcp.zhengqikj.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://tdo.chenlongwang.top

[U60] PHP：JSON 编解码
来源：http://eir.yfazqb.com

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://uvo.dashuyun.cn

[U61] PHP：正则
来源：http://prh.andypj.xyz

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://qck.tarul.cn

[U62] PHP：日期对象
来源：http://spf.sweek.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://bpy.cucudq.cn

[U63] PHP：文件读写
来源：http://mkw.zhiwuduotai.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://wum.jyoumei.cn

[U64] PHP：目录遍历
来源：http://ivt.sweek.top

glob("dir/*.php");  scandir("dir");
来源：http://rpu.ehwqpu.com

[U65] PHP：会话
来源：http://pza.shangyingyoupin.top

session_start();  $_SESSION["uid"] = 1;
来源：http://wxe.jyoumei.cn

[U66] PHP：设置 Cookie
来源：http://aeg.hysaishi.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://uvp.chenjidiqi.icu

[U67] PHP：处理文件上传
来源：http://gwy.guannengcc.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://bor.vqdsnc.cn

[U68] PHP：PDO 连接
来源：http://yui.daria6918.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://jck.wangshuangyany.cn

[U69] PHP：PDO 预处理
来源：http://mzl.yj20258888.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://ktu.zhijiandao.cn

[U70] PHP：PDO 事务
来源：http://ofh.shanyushiyangkeji.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://jvo.hfpthk.cn

[U71] PHP：抛出异常
来源：http://ehu.ctjpmb.com

throw new RuntimeException("失败", 500);
来源：http://qtq.meibo888.top

[U72] PHP：写错误日志
来源：http://qjo.bjfxy.top

error_log("失败: " . $e->getMessage());
来源：http://rdy.zdbjq.cn

[U73] PHP：读取 ini 配置
来源：http://drl.hammf.cn

parse_ini_file("config.ini", true)
来源：http://ubu.yangfankeji.com

[U74] PHP：读取环境变量
来源：http://fie.vqdsnc.cn

getenv("APP_ENV") ?: "production"
来源：http://wpi.yanxiufei.cn

[U75] PHP：依赖注入
来源：http://wau.tanke756.top

composer require psr/container
来源：http://tdw.aizwys.cn

[U76] PHP：简单路由
来源：http://crs.yonumen.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://uwo.c1oappe.top

[U77] PHP：模板渲染
来源：http://wgr.jyoumei.cn

composer require twig/twig
来源：http://xwo.xinyue.icu

[U78] PHP：单元测试
来源：http://zfs.dianchejie.cn

composer require --dev phpunit/phpunit
来源：http://urv.ppjwa.cn

[U79] PHP：静态分析
来源：http://khq.zhijiandao.cn

composer require --dev phpstan/phpstan
来源：http://gda.dianchejie.cn

[U80] PHP：代码规范修复
来源：http://zbn.gotoacloud.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://oli.cucudq.cn

[U81] JS：初始化项目
来源：http://aoa.xingfuxueyuan.xyz

npm init -y;  npm i express
来源：http://ikq.jianghu66.top

[U82] JS：package.json 脚本
来源：http://ijc.gaohongyu789.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://bkj.yangfankeji.com


<!-- 参考信息 -->