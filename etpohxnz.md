代发 wailian999

[T05] Kotlin：when 表达式
来源：http://jmv.tian-w.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://tqj.yueranfly.top

[T06] Kotlin：集合映射
来源：http://quu.jqgfzy.top

listOf(1, 2, 3).map { it * 2 }
来源：http://noo.fzhhl.top

[T07] Kotlin：集合过滤
来源：http://foo.shangyingyoupin.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://cyy.jianghu66.top

[T08] Kotlin：数据类
来源：http://fww.tian-w.cn

data class User(val name: String, val age: Int)
来源：http://gkc.pycfn.com

[T09] Kotlin：扩展函数
来源：http://zqb.fzhhl.top

fun String.exclaim() = this + "!"
来源：http://vbl.sufxvd.cn

[T10] Kotlin：默认参数
来源：http://jac.redwolf501.top

fun greet(name: String = "World") = "Hi $name"
来源：http://lrd.52xcode.cn

[T11] Kotlin：协程
来源：http://ckj.iojbl.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://ayp.sxryk.cn

[T12] Kotlin：解构声明
来源：http://uqx.cheryme.top

val (a, b) = Pair(1, 2)
来源：http://tja.yanxiufei.cn

[T13] Kotlin：只读 Map
来源：http://rkq.jinqigfzy.top

val m = mapOf("a" to 1)
来源：http://itb.zycfv.cn

[T14] Kotlin：循环
来源：http://lff.fzhhl.top

for (i in 1..10) println(i)
来源：http://nui.cucudq.cn

[T15] Kotlin：接口
来源：http://jdu.ivvv.top

interface Shape { fun area(): Double }
来源：http://bfc.wangdashe.top

[T16] Swift：Hello World
来源：http://nwk.daria6918.cn

print("Hello")
来源：http://zfl.yangfankeji.com

[T17] Swift：变量与常量
来源：http://gex.hywenlv.cn

var a = 1;  let b = 2
来源：http://erk.gotoacloud.top

[T18] Swift：字符串插值
来源：http://xwc.tian-w.cn

"值: \(b)"
来源：http://vmx.gotoacloud.top

[T19] Swift：可选绑定
来源：http://xfw.ehwqpu.com

if let n = opt { print(n) }
来源：http://qrc.vehdjk.com

[T20] Swift：数组操作
来源：http://oms.xziqi.cn

var a = [1, 2, 3];  a.append(4)
来源：http://qgz.mhx1999.top

[T21] Swift：遍历
来源：http://gst.zdqjudy.top

for x in a { print(x) }
来源：http://saq.mhx1999.top

[T22] Swift：字典
来源：http://mnx.zhaomingkeji.xyz

var d = ["a": 1];  d["b"] = 2
来源：http://xpc.shuidangran.top

[T23] Swift：函数
来源：http://nyo.mhx1999.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://ive.ppjwa.cn

[T24] Swift：闭包
来源：http://crx.yj202588.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://ytv.chenlongwang.top

[T25] Swift：结构体
来源：http://owd.fktsv.cn

struct P { var x: Int }
来源：http://khq.daxiang520.top

[T26] Swift：类与重写
来源：http://vet.xylfe.cn

class A: Base { override func f() {} }
来源：http://rjm.jiagoushi.top

[T27] Swift：错误处理
来源：http://oqg.yongpay.top

do { try f() } catch { print(error) }
来源：http://yfu.andypj.xyz

[T28] Swift：枚举
来源：http://ayp.shanyushiyangkeji.top

enum Color { case red, green }
来源：http://inu.shzxlz.cn

[T29] Swift：guard 提前返回
来源：http://xyh.yuanzhike.top

guard let x = opt else { return }
来源：http://uiv.birdmap.top

[T30] Swift：协议
来源：http://sxs.haohaochexian.top

protocol Shape { func area() -> Double }
来源：http://ofz.gaohongyu789.top

[T31] Lua：Hello World
来源：http://gzr.zhijiandao.cn

print("Hello")
来源：http://iow.hcnkem.com

[T32] Lua：局部变量
来源：http://uod.iojbl.cn

local a = 1
来源：http://qss.fzhhl.top

[T33] Lua：表（数组）
来源：http://yaa.gogol.net.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://yta.zdbjq.cn

[T34] Lua：遍历表
来源：http://mhm.hysaishi.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://xra.yvedp.cn

[T35] Lua：字典表
来源：http://orl.fanxiaobao.xyz

local d = { a = 1 };  d.b = 2
来源：http://tdm.yj202588.top

[T36] Lua：函数
来源：http://nhu.birdmap.top

function add(a, b) return a + b end
来源：http://pjc.cashguo.top

[T37] Lua：字符串拼接
来源：http://sfp.guannengcc.top

"a" .. "b"
来源：http://cvu.xingfuxueyuan.xyz

[T38] Lua：条件
来源：http://drd.zhoulong.xyz

if x > 0 then print("正") end
来源：http://mto.birdmap.top

[T39] Lua：模式匹配
来源：http://rlf.shuidangran.top

string.find(s, "%d+")
来源：http://dlc.quarkkingdee.top

[T40] Lua：元表
来源：http://vmj.haohaochexian.top

setmetatable({}, { __index = base })
来源：http://oxg.svipenyu.cn

[T41] Perl：Hello World
来源：http://lzx.nanxuanxn.top

print "Hello\n";
来源：http://hgw.ctjpmb.com

[T42] Perl：变量类型
来源：http://jyr.shangyingyoupin.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://quk.sufxvd.cn

[T43] Perl：字符串插值
来源：http://xsp.redwolf501.top

"值: $a"
来源：http://wqu.ydjk.org.cn

[T44] Perl：条件
来源：http://zsm.daxiang520.top

if ($a > 0) { print "正"; }
来源：http://eaf.mhx1999.top

[T45] Perl：数组遍历
来源：http://ijj.yueranfly.top

for my $x (@arr) { print $x; }
来源：http://jgl.ywan-chungtsiang.top

[T46] Perl：哈希操作
来源：http://epn.shzxlz.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://ncc.daxiang520.top

[T47] Perl：正则捕获
来源：http://qnp.jyoumei.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://yhb.52xcode.cn

[T48] Perl：正则替换
来源：http://dzp.kuanghao11.cn

$s =~ s/old/new/g;
来源：http://apc.jqgufenzy.top

[T49] Perl：函数
来源：http://psk.yonumen.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://gqx.shanyushiyangkeji.top

[T50] Perl：逐行读文件
来源：http://ebk.ybcxt.top

open my $fh, "<", "a.txt" or die $!;
来源：http://vbg.yanxiufei.cn

while (my $line = <$fh>) { print $line; }
来源：http://gic.0kj1m.cn

[T51] Scala：Hello World
来源：http://kgk.haohaochexian.top

println("Hello")
来源：http://jtd.zhiwuduotai.top

[T52] Scala：变量
来源：http://jhj.chenlongwang.top

val a = 1;  var b = 2
来源：http://vkx.jinqigfzy.top

[T53] Scala：字符串插值
来源：http://pyb.zhengqikj.top

s"值: $b"
来源：http://ixm.zhiwuduotai.top

[T54] Scala：集合映射
来源：http://mpj.52xcode.cn

List(1, 2, 3).map(_ * 2)
来源：http://keb.jinghuilouyu.cn

[T55] Scala：集合过滤
来源：http://xvv.cucudq.cn

List(1, 2, 3).filter(_ > 1)
来源：http://vqn.xuetiantiany.cn

[T56] Scala：样例类
来源：http://aph.nanxinkj.top

case class User(name: String, age: Int)
来源：http://xky.fengsongda.top

[T57] Scala：模式匹配
来源：http://nde.shanyushiyangtech.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://gek.snrcjt.cn

[T58] Scala：函数定义
来源：http://vci.shangyingyoupin.top

def add(a: Int, b: Int): Int = a + b
来源：http://fzy.sjlbkw.cn

[T59] Scala：循环
来源：http://igf.chenlongwang.top

for (i <- 1 to 10) println(i)
来源：http://qbk.vehdjk.com

[T60] Scala：折叠
来源：http://ako.yuanzhike.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://zse.yfazqb.com

================================================================================
来源：http://jvd.ydzc1.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://ysa.ydzc1.top

================================================================================
来源：http://ykp.yongpay.top

[U01] Py：创建虚拟环境
来源：http://jwq.jianghu66.top

python -m venv .venv && source .venv/bin/activate
来源：http://vwc.jinqigfzy.top

[U02] Py：导出 / 安装依赖
来源：http://glg.nanxuanxn.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://fvq.yongpay.top

[U03] Py：加载 .env 配置
来源：http://naj.hcnkem.com

from dotenv import load_dotenv; load_dotenv()
来源：http://fzh.hnxiangtu.top

[U04] Py：变量调试打印
来源：http://eww.gotoacloud.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://sml.52xcode.cn

[U05] Py：列表去重且保序
来源：http://kwj.yuanzhike.top

list(dict.fromkeys(arr))
来源：http://hgw.kuanghao11.cn

[U06] Py：合并两个字典
来源：http://hbn.haohaochexian.top

{**a, **b}
来源：http://rkh.zhongyouzk.top

[U07] Py：反转字典键值
来源：http://tbf.vehdjk.com

{v: k for k, v in d.items()}
来源：http://phb.sysykeji.top

[U08] Py：展平二维列表
来源：http://dcl.yongpay.top

[y for x in nested for y in x]
来源：http://uxg.andypj.xyz

[U09] Py：字典取最大值的键
来源：http://qnv.tianlin.xyz

max(d, key=d.get)
来源：http://qjp.52xcode.cn

[U10] Py：按值排序字典
来源：http://hbm.bjfxy.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://amx.fzhhl.top

[U11] Py：生成器表达式
来源：http://oly.dashuyun.cn

(x * 2 for x in arr)
来源：http://cbw.uphjek.com

[U12] Py：取出现最多的 3 个元素
来源：http://etf.sjlbkw.cn

Counter(arr).most_common(3)
来源：http://wor.havefunace.top

[U13] Py：固定长度队列
来源：http://mvh.zhaomingkeji.xyz

deque(maxlen=10)
来源：http://kty.iojbl.cn

[U14] Py：分组收集到列表
来源：http://wjf.jinqigfzy.top

defaultdict(list)
来源：http://oro.c1oappe.top

[U15] Py：高精度计时
来源：http://ggi.hcnkem.com

t = time.perf_counter()
来源：http://kmo.ehwqpu.com

[U16] Py：命令行参数解析
来源：http://gfu.xuetiantiany.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://awm.birdmap.top

[U17] Py：初始化日志
来源：http://snx.ywan-chungtsiang.top

logging.basicConfig(level=logging.INFO)
来源：http://vtz.yonumen.top

[U18] Py：预编译正则
来源：http://fae.daria6918.cn

pat = re.compile(r"\d+")
来源：http://zhk.smart0.xyz

[U19] Py：正则替换带回调
来源：http://cbc.havefunace.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://evb.hfpthk.cn

[U20] Py：缓存函数结果
来源：http://tyx.ybcxt.top

@functools.lru_cache(maxsize=None)
来源：http://awt.jianghu66.top

[U21] Py：自定义上下文管理器
来源：http://lke.birdmap.top

@contextlib.contextmanager
来源：http://psi.jinyuanbaomall.cn

[U22] Py：矩阵转置
来源：http://wbt.jinghuilouyu.cn

list(zip(*m))
来源：http://ogi.sweek.top

[U23] Py：分块读取大文件
来源：http://rov.tanke756.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://qsd.yonumen.top

[U24] Py：路径操作
来源：http://eba.zhixingplan.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://oqw.gogol.net.cn

[U25] Py：CSV 按字典读
来源：http://hod.hnxiangtu.top

csv.DictReader(f)
来源：http://hyv.guannengcc.top

[U26] Py：并发下载
来源：http://jte.hcnkem.com

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://tzf.hcnkem.com

[U27] Py：异步 HTTP
来源：http://pae.yj20258.top

aiohttp.ClientSession() 配合 async with
来源：http://wpr.smart0.xyz

[U28] Py：类型别名
来源：http://yen.nwbrower.top

UserId = int
来源：http://fju.jinyuanbaomall.cn

[U29] Py：属性校验
来源：http://pyv.52xcode.cn

@property 与 @x.setter 配合
来源：http://dba.bjfxy.top

[U30] Py：数据类
来源：http://fwb.chenzaomai.com

@dataclass(slots=True)
来源：http://uum.pycfn.com

[U31] Py：单测
来源：http://fkt.jlsjyb.cn

python -m pytest -q
来源：http://goz.jianghu66.top

[U32] Py：代码格式化
来源：http://hoq.quarkkingdee.top

ruff format . && ruff check --fix .
来源：http://lce.9152youxi.cn

[U33] Py：打包发布
来源：http://chi.zhixingplan.top

python -m build  （依赖 pyproject.toml）
来源：http://exs.andypj.xyz

[U34] Py：判断编码
来源：http://yak.yonumen.top

chardet.detect(raw)
来源：http://tzo.ywan-chungtsiang.top

[U35] Py：发送邮件
来源：http://nnr.yj202588.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://ike.quarkkingdee.top

[U36] Py：定时任务
来源：http://ieg.ydjk.org.cn

schedule.every(10).minutes.do(job)
来源：http://cuj.xuetiantiany.cn

[U37] Py：读写 Excel
来源：http://yzl.mhx1999.top

pandas.read_excel / DataFrame.to_excel
来源：http://cvv.daxiang520.top

[U38] Py：获取脚本所在目录
来源：http://yha.wangdashe.top

Path(__file__).resolve().parent
来源：http://ymt.yfazqb.com

[U39] Py：判断是否在交互环境
来源：http://bmq.birdmap.top

sys.stdout.isatty()
来源：http://rjd.jqgufenzy.top

[U40] Py：打印到标准错误
来源：http://los.hywenlv.cn

print("err", file=sys.stderr)
来源：http://qoq.zdbjq.cn

[U41] PHP：初始化 Composer 项目
来源：http://vex.ppjwa.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://jlk.ctjpmb.com

[U42] PHP：PSR-4 自动加载
来源：http://aht.cheryme.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hkp.hongshengwenyu.top

[U43] PHP：声明命名空间
来源：http://pkd.yangfankeji.com

namespace App\Http;
来源：http://zsx.yj202588.top

[U44] PHP：开启严格类型
来源：http://qkl.meibo888.top

declare(strict_types=1);
来源：http://dna.svipenyu.cn

[U45] PHP：类型声明与返回类型
来源：http://neb.yfazqb.com

function add(int $a, int $b): int { return $a + $b; }
来源：http://vow.feifeiyinyue.top

[U46] PHP：可空类型
来源：http://yfo.xingfuxueyuan.xyz

?string $name = null
来源：http://xje.316326.xyz

[U47] PHP：联合类型
来源：http://nev.fehbvm.com

int|string $id
来源：http://xti.jqgufenzy.top

[U48] PHP：纯枚举
来源：http://gvq.daria6918.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://mkm.fzhhl.top

[U49] PHP：只读属性
来源：http://lut.0kj1m.cn

public readonly string $name
来源：http://pzq.yfazqb.com

[U50] PHP：构造器属性提升
来源：http://opr.shangyingyoupin.top

public function __construct(private int $id) {}
来源：http://czq.guannengcc.top

[U51] PHP：数组解构
来源：http://woo.yuxming.cn

[$a, $b] = $arr;
来源：http://cny.daxiang520.top

[U52] PHP：箭头函数
来源：http://jdx.xingfuxueyuan.xyz

$double = fn($x) => $x * 2;
来源：http://wvz.snrcjt.cn

[U53] PHP：空合并运算符
来源：http://gto.hnxiangtu.top

$v = $a ?? $b ?? "default";
来源：http://kzr.jyoumei.cn

[U54] PHP：空安全调用
来源：http://eyk.vehdjk.com

$obj?->method()
来源：http://coy.fktsv.cn

[U55] PHP：match 表达式
来源：http://jgh.gogol.net.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://kuy.hnqzz.top

[U56] PHP：命名参数
来源：http://wel.kuanghao11.cn

f(a: 1, b: 2)
来源：http://lzw.xuetiantiany.cn

[U57] PHP：字符串插值
来源：http://fnl.jqgfzy.top

"值: {$a}"
来源：http://jym.52xcode.cn

[U58] PHP：数组三件套
来源：http://gqe.cheryme.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://deh.jlsjyb.cn

[U59] PHP：自定义排序
来源：http://vtr.daxiang520.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://zii.sxryk.cn

[U60] PHP：JSON 编解码
来源：http://tmy.kuanghao11.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://czs.jianghu66.top

[U61] PHP：正则
来源：http://cbf.zhoulong.xyz

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://zlj.dashuyun.cn

[U62] PHP：日期对象
来源：http://lbj.hcnkem.com

(new DateTimeImmutable())->format("Y-m-d");
来源：http://cce.jiagoushi.top

[U63] PHP：文件读写
来源：http://zxf.xuetiantiany.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hzv.pycfn.com

[U64] PHP：目录遍历
来源：http://yjg.jinqigufen.top

glob("dir/*.php");  scandir("dir");
来源：http://hqk.zdqjudy.top

[U65] PHP：会话
来源：http://rwf.cucudq.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://lfy.redwolf501.top

[U66] PHP：设置 Cookie
来源：http://hzp.hfpthk.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://uin.iojbl.cn

[U67] PHP：处理文件上传
来源：http://vhw.c1oappe.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://kno.316326.xyz

[U68] PHP：PDO 连接
来源：http://bnr.vqdsnc.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://xlv.cheryme.top

[U69] PHP：PDO 预处理
来源：http://hre.hysaishi.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://fhs.yueranfly.top

[U70] PHP：PDO 事务
来源：http://bvt.sysykeji.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://hir.dianchejie.cn

[U71] PHP：抛出异常
来源：http://pek.chenzaomai.com

throw new RuntimeException("失败", 500);
来源：http://vqh.sysykeji.top

[U72] PHP：写错误日志
来源：http://qtx.xuetiantiany.cn

error_log("失败: " . $e->getMessage());
来源：http://wlt.wangshuangyany.cn

[U73] PHP：读取 ini 配置
来源：http://qho.chenzaomai.com

parse_ini_file("config.ini", true)
来源：http://ngv.jyoumei.cn

[U74] PHP：读取环境变量
来源：http://uxp.hongshengwenyu.top

getenv("APP_ENV") ?: "production"
来源：http://ejm.meibo888.top

[U75] PHP：依赖注入
来源：http://obj.hywenlv.cn

composer require psr/container
来源：http://vgw.shuidangran.top

[U76] PHP：简单路由
来源：http://arv.snrcjt.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://wvs.hnqzz.top

[U77] PHP：模板渲染
来源：http://naf.xingfuxueyuan.xyz

composer require twig/twig
来源：http://ncg.pengpengdd.cyou

[U78] PHP：单元测试
来源：http://ztq.cashguo.top

composer require --dev phpunit/phpunit
来源：http://ezi.9152youxi.cn

[U79] PHP：静态分析
来源：http://lgw.shanyushiyangkeji.top

composer require --dev phpstan/phpstan
来源：http://gmx.zhiwuduotai.top

[U80] PHP：代码规范修复
来源：http://yxd.sxryk.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://mka.svipenyu.cn

[U81] JS：初始化项目
来源：http://icl.bjfxy.top

npm init -y;  npm i express
来源：http://zij.yfazqb.com

[U82] JS：package.json 脚本
来源：http://qlw.zdqjudy.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://jnq.havefunace.top

[U83] JS：ES Module 导入导出
来源：http://jar.sxryk.cn

export const a = 1;  import { a } from "./m.js";
来源：http://tnx.hongshengwenyu.top

[U84] JS：CommonJS 写法
来源：http://xac.316326.xyz

module.exports = { a };  const { a } = require("./m");
来源：http://rsp.haohaochexian.top

[U85] JS：可选链
来源：http://jyn.gzhubu.top

a?.b?.c
来源：http://qfc.zdqjudy.top

[U86] JS：空值合并
来源：http://exu.yvedp.cn

a ?? b
来源：http://drr.haohaochexian.top

[U87] JS：解构默认值
来源：http://nro.zycfv.cn

const { a = 1, b = 2 } = obj;
来源：http://xlx.yvedp.cn

[U88] JS：对象展开合并
来源：http://rlj.bbcook.cn

{ ...a, ...b }
来源：http://pkt.redwolf501.top

[U89] JS：数组去重
来源：http://pxe.9152youxi.cn

[...new Set(arr)]
来源：http://cyx.guowangkeji.top

[U90] JS：数字数组排序
来源：http://zfn.gzhubu.top

[...arr].sort((a, b) => a - b)
来源：http://egv.smart0.xyz

[U91] JS：对象键值遍历
来源：http://bxp.fzhhl.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://jgu.jlsjyb.cn

[U92] JS：深拷贝
来源：http://vmy.sxryk.cn

structuredClone(obj)
来源：http://alw.zhijiandao.cn


<!-- 参考信息 -->