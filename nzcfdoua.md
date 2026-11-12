代发 wailian999

[T23] Swift：函数
来源：http://qqe.hysaishi.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://iti.epnwcf.com

[T24] Swift：闭包
来源：http://umi.zhixingplan.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://lrs.sxryk.cn

[T25] Swift：结构体
来源：http://rws.chenjidiqi.icu

struct P { var x: Int }
来源：http://myq.guannengcc.top

[T26] Swift：类与重写
来源：http://zgo.ywan-chungtsiang.top

class A: Base { override func f() {} }
来源：http://fpw.redwolf501.top

[T27] Swift：错误处理
来源：http://vgw.ppjwa.cn

do { try f() } catch { print(error) }
来源：http://nhh.epnwcf.com

[T28] Swift：枚举
来源：http://ctx.pycfn.com

enum Color { case red, green }
来源：http://evy.cucudq.cn

[T29] Swift：guard 提前返回
来源：http://glg.hfpthk.cn

guard let x = opt else { return }
来源：http://qjz.hongshengwenyu.top

[T30] Swift：协议
来源：http://oqh.birdmap.top

protocol Shape { func area() -> Double }
来源：http://oul.cheryme.top

[T31] Lua：Hello World
来源：http://deh.jlsjyb.cn

print("Hello")
来源：http://ebj.gzhubu.top

[T32] Lua：局部变量
来源：http://oik.zhijiandao.cn

local a = 1
来源：http://vsy.aibaodan.cn

[T33] Lua：表（数组）
来源：http://mpb.zhoulong.xyz

local t = {1, 2, 3};  t[4] = 4
来源：http://aqd.gaohongyu789.top

[T34] Lua：遍历表
来源：http://gko.dianchejie.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://oyp.zhoulong.xyz

[T35] Lua：字典表
来源：http://aqg.mhx1999.top

local d = { a = 1 };  d.b = 2
来源：http://bhl.shuidangran.top

[T36] Lua：函数
来源：http://wgl.hammf.cn

function add(a, b) return a + b end
来源：http://sqr.xingfuxueyuan.xyz

[T37] Lua：字符串拼接
来源：http://yhf.cheryme.top

"a" .. "b"
来源：http://hkb.ydzc1.top

[T38] Lua：条件
来源：http://oyx.redwolf501.top

if x > 0 then print("正") end
来源：http://owd.ctjpmb.com

[T39] Lua：模式匹配
来源：http://tvd.fanxiaobao.xyz

string.find(s, "%d+")
来源：http://wkp.xziqi.cn

[T40] Lua：元表
来源：http://vyo.xylfe.cn

setmetatable({}, { __index = base })
来源：http://aoi.jyoumei.cn

[T41] Perl：Hello World
来源：http://dxa.jianghu66.top

print "Hello\n";
来源：http://tgw.zhoulong.xyz

[T42] Perl：变量类型
来源：http://omd.hnqzz.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://ont.dianchejie.cn

[T43] Perl：字符串插值
来源：http://jph.yangfankeji.com

"值: $a"
来源：http://gmw.zhiwuduotai.top

[T44] Perl：条件
来源：http://amj.xuanzx.com

if ($a > 0) { print "正"; }
来源：http://dgm.jqgfzy.top

[T45] Perl：数组遍历
来源：http://kpp.vqdsnc.cn

for my $x (@arr) { print $x; }
来源：http://bqp.yj202588.top

[T46] Perl：哈希操作
来源：http://fgw.yongpay.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://fwl.ivvv.top

[T47] Perl：正则捕获
来源：http://jrc.chenlongwang.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://qhs.zhengqikj.top

[T48] Perl：正则替换
来源：http://wrp.yj20258.top

$s =~ s/old/new/g;
来源：http://aaa.jiagoushi.top

[T49] Perl：函数
来源：http://fll.jianghu66.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://rhh.ybcxt.top

[T50] Perl：逐行读文件
来源：http://lwz.zhoulong.xyz

open my $fh, "<", "a.txt" or die $!;
来源：http://iyp.zhixingplan.top

while (my $line = <$fh>) { print $line; }
来源：http://ohe.xuanzx.com

[T51] Scala：Hello World
来源：http://lam.jinghuilouyu.cn

println("Hello")
来源：http://iaw.xylfe.cn

[T52] Scala：变量
来源：http://ljz.wangdashe.top

val a = 1;  var b = 2
来源：http://els.tianlin.xyz

[T53] Scala：字符串插值
来源：http://pwx.haohaochexian.top

s"值: $b"
来源：http://kzv.hywenlv.cn

[T54] Scala：集合映射
来源：http://ouz.jinqigufen.top

List(1, 2, 3).map(_ * 2)
来源：http://zno.fengsongda.top

[T55] Scala：集合过滤
来源：http://dvb.nanxuanxn.top

List(1, 2, 3).filter(_ > 1)
来源：http://geq.vqdsnc.cn

[T56] Scala：样例类
来源：http://oec.xylfe.cn

case class User(name: String, age: Int)
来源：http://mfx.zdqjudy.top

[T57] Scala：模式匹配
来源：http://ptw.jqgufenzy.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://wbl.jyoumei.cn

[T58] Scala：函数定义
来源：http://zgq.zhijiandao.cn

def add(a: Int, b: Int): Int = a + b
来源：http://ybd.316326.xyz

[T59] Scala：循环
来源：http://nyo.redwolf501.top

for (i <- 1 to 10) println(i)
来源：http://iwh.xinyue.icu

[T60] Scala：折叠
来源：http://khd.smart0.xyz

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://tir.gaohongyu789.top

================================================================================
来源：http://hlw.316326.xyz

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://rjz.gaohongyu789.top

================================================================================
来源：http://zxs.daria6918.cn

[U01] Py：创建虚拟环境
来源：http://wds.zhoulong.xyz

python -m venv .venv && source .venv/bin/activate
来源：http://bnz.hesvh.cn

[U02] Py：导出 / 安装依赖
来源：http://xsz.nanxuanxn.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://let.shuidangran.top

[U03] Py：加载 .env 配置
来源：http://diq.guowangkeji.top

from dotenv import load_dotenv; load_dotenv()
来源：http://lzg.andypj.xyz

[U04] Py：变量调试打印
来源：http://lrk.9152youxi.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://szu.fehbvm.com

[U05] Py：列表去重且保序
来源：http://ghj.cdnleiting.top

list(dict.fromkeys(arr))
来源：http://wbe.bjfxy.top

[U06] Py：合并两个字典
来源：http://wiz.gogol.net.cn

{**a, **b}
来源：http://keg.andypj.xyz

[U07] Py：反转字典键值
来源：http://ugy.meibo888.top

{v: k for k, v in d.items()}
来源：http://yyq.zhaomingkeji.xyz

[U08] Py：展平二维列表
来源：http://mmr.yj202588.top

[y for x in nested for y in x]
来源：http://lml.vehdjk.com

[U09] Py：字典取最大值的键
来源：http://ewy.pycfn.com

max(d, key=d.get)
来源：http://kdb.ywan-chungtsiang.top

[U10] Py：按值排序字典
来源：http://tva.zhixingplan.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://edi.redwolf501.top

[U11] Py：生成器表达式
来源：http://txh.andypj.xyz

(x * 2 for x in arr)
来源：http://zmp.sweek.top

[U12] Py：取出现最多的 3 个元素
来源：http://lnz.cheryme.top

Counter(arr).most_common(3)
来源：http://bwu.pycfn.com

[U13] Py：固定长度队列
来源：http://mhe.bbcook.cn

deque(maxlen=10)
来源：http://bxm.guannengcc.top

[U14] Py：分组收集到列表
来源：http://fdx.shuidangran.top

defaultdict(list)
来源：http://qgy.jqgfzy.top

[U15] Py：高精度计时
来源：http://kkt.zdbjq.cn

t = time.perf_counter()
来源：http://hko.52xcode.cn

[U16] Py：命令行参数解析
来源：http://dvt.hongshengwenyu.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://gfs.yuanzhike.top

[U17] Py：初始化日志
来源：http://ocm.meibo888.top

logging.basicConfig(level=logging.INFO)
来源：http://aef.pengpengdd.cyou

[U18] Py：预编译正则
来源：http://hof.jqgfzy.top

pat = re.compile(r"\d+")
来源：http://xok.ydzc1.top

[U19] Py：正则替换带回调
来源：http://wvm.meibo888.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://faw.sysykeji.top

[U20] Py：缓存函数结果
来源：http://hpq.ybcxt.top

@functools.lru_cache(maxsize=None)
来源：http://rug.yongpay.top

[U21] Py：自定义上下文管理器
来源：http://vnv.pycfn.com

@contextlib.contextmanager
来源：http://ekf.gaohongyu789.top

[U22] Py：矩阵转置
来源：http://cfc.haohaochexian.top

list(zip(*m))
来源：http://cgz.tarul.cn

[U23] Py：分块读取大文件
来源：http://lls.nwbrower.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://yqv.bjfxy.top

[U24] Py：路径操作
来源：http://wts.hnxiangtu.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://mvu.shangyingyoupin.top

[U25] Py：CSV 按字典读
来源：http://ocf.zhongyouzk.top

csv.DictReader(f)
来源：http://ewd.yanxiufei.cn

[U26] Py：并发下载
来源：http://pju.sxryk.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://ygd.ppjwa.cn

[U27] Py：异步 HTTP
来源：http://rkn.hongshengwenyu.top

aiohttp.ClientSession() 配合 async with
来源：http://ppb.fzhhl.top

[U28] Py：类型别名
来源：http://szy.hywenlv.cn

UserId = int
来源：http://eih.hysaishi.cn

[U29] Py：属性校验
来源：http://qca.c1oappe.top

@property 与 @x.setter 配合
来源：http://wty.cashguo.top

[U30] Py：数据类
来源：http://nsw.shangyingyoupin.top

@dataclass(slots=True)
来源：http://fde.shangyingyoupin.top

[U31] Py：单测
来源：http://gey.yj202588.top

python -m pytest -q
来源：http://fki.svipenyu.cn

[U32] Py：代码格式化
来源：http://wev.gzhubu.top

ruff format . && ruff check --fix .
来源：http://mcq.cheryme.top

[U33] Py：打包发布
来源：http://fvu.daria6918.cn

python -m build  （依赖 pyproject.toml）
来源：http://xkv.chenlongwang.top

[U34] Py：判断编码
来源：http://fnd.cucudq.cn

chardet.detect(raw)
来源：http://pnd.jinqigufen.top

[U35] Py：发送邮件
来源：http://kev.xziqi.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://rpy.0kj1m.cn

[U36] Py：定时任务
来源：http://lpb.hysaishi.cn

schedule.every(10).minutes.do(job)
来源：http://xyq.dashuyun.cn

[U37] Py：读写 Excel
来源：http://hck.chenlongwang.top

pandas.read_excel / DataFrame.to_excel
来源：http://weq.bjfxy.top

[U38] Py：获取脚本所在目录
来源：http://fqn.jinqigufen.top

Path(__file__).resolve().parent
来源：http://pct.pycfn.com

[U39] Py：判断是否在交互环境
来源：http://whu.shuidangran.top

sys.stdout.isatty()
来源：http://sjb.zhoulong.xyz

[U40] Py：打印到标准错误
来源：http://pci.pengpengdd.cyou

print("err", file=sys.stderr)
来源：http://nat.shanyushiyangtech.top

[U41] PHP：初始化 Composer 项目
来源：http://oki.xylfe.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://kym.daria6918.cn

[U42] PHP：PSR-4 自动加载
来源：http://ljy.svipenyu.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://wmk.redwolf501.top

[U43] PHP：声明命名空间
来源：http://jhe.zhongyouzk.top

namespace App\Http;
来源：http://gbu.chenzaomai.com

[U44] PHP：开启严格类型
来源：http://rgm.epnwcf.com

declare(strict_types=1);
来源：http://hxe.cdnleiting.top

[U45] PHP：类型声明与返回类型
来源：http://ldn.shuidangran.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://liz.fehbvm.com

[U46] PHP：可空类型
来源：http://ymv.316326.xyz

?string $name = null
来源：http://ebd.sxryk.cn

[U47] PHP：联合类型
来源：http://hvb.shanyushiyangtech.top

int|string $id
来源：http://paz.chenzaomai.com

[U48] PHP：纯枚举
来源：http://ahp.zhiwuduotai.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://nty.yueranfly.top

[U49] PHP：只读属性
来源：http://jta.yueranfly.top

public readonly string $name
来源：http://qfo.fzhhl.top

[U50] PHP：构造器属性提升
来源：http://jot.chenjidiqi.icu

public function __construct(private int $id) {}
来源：http://lvh.gzhubu.top

[U51] PHP：数组解构
来源：http://xry.tanke756.top

[$a, $b] = $arr;
来源：http://vgn.feifeiyinyue.top

[U52] PHP：箭头函数
来源：http://nvn.hongshengwenyu.top

$double = fn($x) => $x * 2;
来源：http://lxq.xuetiantiany.cn

[U53] PHP：空合并运算符
来源：http://olq.zdbjq.cn

$v = $a ?? $b ?? "default";
来源：http://njs.sysykeji.top

[U54] PHP：空安全调用
来源：http://zve.zycfv.cn

$obj?->method()
来源：http://byn.xinyue.icu

[U55] PHP：match 表达式
来源：http://epz.ywan-chungtsiang.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://gno.sjlbkw.cn

[U56] PHP：命名参数
来源：http://ukv.hongshengwenyu.top

f(a: 1, b: 2)
来源：http://ijz.c1oappe.top

[U57] PHP：字符串插值
来源：http://whr.zhijiandao.cn

"值: {$a}"
来源：http://ngw.yvedp.cn

[U58] PHP：数组三件套
来源：http://hqi.jqgufenzy.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://nix.svipenyu.cn

[U59] PHP：自定义排序
来源：http://xnk.snrcjt.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hob.0kj1m.cn

[U60] PHP：JSON 编解码
来源：http://nlt.wangshuangyany.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://mig.zhijiandao.cn

[U61] PHP：正则
来源：http://age.meibo888.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://yok.jqgfzy.top

[U62] PHP：日期对象
来源：http://qrm.sysykeji.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://ylm.feifeiyinyue.top

[U63] PHP：文件读写
来源：http://wxl.wangdashe.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://mtj.havefunace.top

[U64] PHP：目录遍历
来源：http://phq.fanxiaobao.xyz

glob("dir/*.php");  scandir("dir");
来源：http://rif.chenzaomai.com

[U65] PHP：会话
来源：http://gpc.guannengcc.top

session_start();  $_SESSION["uid"] = 1;
来源：http://tjh.shzxlz.cn

[U66] PHP：设置 Cookie
来源：http://kya.zhaomingkeji.xyz

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://ozp.shanyushiyangtech.top

[U67] PHP：处理文件上传
来源：http://zhv.xinyue.icu

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://xwj.xuanzx.com

[U68] PHP：PDO 连接
来源：http://uut.bjfxy.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://zyj.hnqzz.top

[U69] PHP：PDO 预处理
来源：http://waf.gogol.net.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://jfc.jinqigfzy.top

[U70] PHP：PDO 事务
来源：http://fic.jinghuilouyu.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://tww.yvedp.cn

[U71] PHP：抛出异常
来源：http://wgw.xylfe.cn

throw new RuntimeException("失败", 500);
来源：http://fsy.hcnkem.com

[U72] PHP：写错误日志
来源：http://xsp.0kj1m.cn

error_log("失败: " . $e->getMessage());
来源：http://ueb.gaohongyu789.top

[U73] PHP：读取 ini 配置
来源：http://kri.9152youxi.cn

parse_ini_file("config.ini", true)
来源：http://mau.cucudq.cn

[U74] PHP：读取环境变量
来源：http://cco.quarkkingdee.top

getenv("APP_ENV") ?: "production"
来源：http://kpq.nanxuanxn.top

[U75] PHP：依赖注入
来源：http://ogl.sxryk.cn

composer require psr/container
来源：http://qpk.bbcook.cn

[U76] PHP：简单路由
来源：http://eyr.chenlongwang.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://ouv.gotoacloud.top

[U77] PHP：模板渲染
来源：http://zci.tian-w.cn

composer require twig/twig
来源：http://wqy.guowangkeji.top

[U78] PHP：单元测试
来源：http://cot.sufxvd.cn

composer require --dev phpunit/phpunit
来源：http://dly.yueranfly.top

[U79] PHP：静态分析
来源：http://hgj.daxiang520.top

composer require --dev phpstan/phpstan
来源：http://yku.shangyingyoupin.top

[U80] PHP：代码规范修复
来源：http://pos.epnwcf.com

composer require --dev friendsofphp/php-cs-fixer
来源：http://umj.ivvv.top

[U81] JS：初始化项目
来源：http://hvp.cqqwz.cn

npm init -y;  npm i express
来源：http://pau.zhiwuduotai.top

[U82] JS：package.json 脚本
来源：http://kre.fanxiaobao.xyz

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://vjy.sjlbkw.cn

[U83] JS：ES Module 导入导出
来源：http://pvp.ctjpmb.com

export const a = 1;  import { a } from "./m.js";
来源：http://qgn.chenlongwang.top

[U84] JS：CommonJS 写法
来源：http://acp.yuxming.cn

module.exports = { a };  const { a } = require("./m");
来源：http://ocr.ctjpmb.com

[U85] JS：可选链
来源：http://mkk.gotoacloud.top

a?.b?.c
来源：http://rxq.316326.xyz

[U86] JS：空值合并
来源：http://fqj.zhiwuduotai.top

a ?? b
来源：http://qyy.shanyushiyangkeji.top

[U87] JS：解构默认值
来源：http://fhr.shanyushiyangtech.top

const { a = 1, b = 2 } = obj;
来源：http://mev.jlsjyb.cn

[U88] JS：对象展开合并
来源：http://ftf.shangyingyoupin.top

{ ...a, ...b }
来源：http://cil.yvedp.cn

[U89] JS：数组去重
来源：http://htr.xziqi.cn

[...new Set(arr)]
来源：http://wkd.sufxvd.cn

[U90] JS：数字数组排序
来源：http://ifz.cqqwz.cn

[...arr].sort((a, b) => a - b)
来源：http://opt.hammf.cn

[U91] JS：对象键值遍历
来源：http://yoy.tarul.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://etv.jinqigfzy.top

[U92] JS：深拷贝
来源：http://bnn.tianlin.xyz

structuredClone(obj)
来源：http://kee.gzhubu.top

[U93] JS：模板字符串
来源：http://mvk.sweek.top

`共 ${n} 条`
来源：http://dlc.ywan-chungtsiang.top

[U94] JS：箭头函数
来源：http://qbc.jianghu66.top

const double = x => x * 2;
来源：http://vko.jlsjyb.cn

[U95] JS：Promise 包装
来源：http://dkd.vehdjk.com

new Promise((resolve, reject) => {})
来源：http://fmi.shzxlz.cn

[U96] JS：async/await 与异常
来源：http://rtm.yvedp.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://yhq.yuxming.cn

[U97] JS：并发请求
来源：http://wyx.guowangkeji.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://ivl.xuanzx.com

[U98] JS：fetch 带 JSON
来源：http://dev.9152youxi.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://xef.uphjek.com

[U99] JS：事件监听
来源：http://zeu.nanxuanxn.top

el.addEventListener("click", e => {})
来源：http://fct.jinyuanbaomall.cn

[U100] JS：DOM 查询
来源：http://fyr.ctjpmb.com

document.querySelector(".item")
来源：http://hrq.yueranfly.top

[U101] JS：classList 操作
来源：http://lha.jinqigufen.top

el.classList.toggle("active")
来源：http://qgu.sufxvd.cn

[U102] JS：本地存储
来源：http://vnb.jinghuilouyu.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://jfl.uphjek.com

[U103] JS：定时器
来源：http://nul.cqqwz.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://ajb.0kj1m.cn

[U104] JS：防抖
来源：http://eet.wangshuangyany.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://htf.ehwqpu.com

[U105] JS：节流
来源：http://xqv.daria6918.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://pfg.svipenyu.cn

[U106] JS：日期格式化
来源：http://vil.gogol.net.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://rpg.xuetiantiany.cn

[U107] JS：数字千分位
来源：http://quj.daxiang520.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://ivw.tanke756.top

[U108] JS：随机整数
来源：http://jwf.jinqigfzy.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://oov.ppjwa.cn

[U109] JS：数组分组
来源：http://cjo.zdbjq.cn

Object.groupBy(arr, x => x.type)
来源：http://vlt.cdnleiting.top

[U110] JS：数组分块
来源：http://ihc.feifeiyinyue.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://shc.cucudq.cn


<!-- 参考信息 -->