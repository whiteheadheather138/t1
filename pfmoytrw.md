代发 wailian999

[T29] Swift：guard 提前返回
来源：http://sve.ppjwa.cn

guard let x = opt else { return }
来源：http://jzd.nanxuanxn.top

[T30] Swift：协议
来源：http://kkk.yfazqb.com

protocol Shape { func area() -> Double }
来源：http://lnt.hfpthk.cn

[T31] Lua：Hello World
来源：http://oup.hnqzz.top

print("Hello")
来源：http://aie.ivvv.top

[T32] Lua：局部变量
来源：http://mhf.52xcode.cn

local a = 1
来源：http://bqv.316326.xyz

[T33] Lua：表（数组）
来源：http://mjm.zycfv.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://tqx.jinqigufen.top

[T34] Lua：遍历表
来源：http://kcj.zhengqikj.top

for i, v in ipairs(t) do print(i, v) end
来源：http://xky.bbcook.cn

[T35] Lua：字典表
来源：http://qqi.zhiwuduotai.top

local d = { a = 1 };  d.b = 2
来源：http://kuj.yj20258.top

[T36] Lua：函数
来源：http://cnz.cheryme.top

function add(a, b) return a + b end
来源：http://nuy.tarul.cn

[T37] Lua：字符串拼接
来源：http://fxi.meibo888.top

"a" .. "b"
来源：http://ene.hesvh.cn

[T38] Lua：条件
来源：http://awa.redwolf501.top

if x > 0 then print("正") end
来源：http://unc.kuanghao11.cn

[T39] Lua：模式匹配
来源：http://ceg.yonumen.top

string.find(s, "%d+")
来源：http://ezu.jinghuilouyu.cn

[T40] Lua：元表
来源：http://gpi.zdbjq.cn

setmetatable({}, { __index = base })
来源：http://bvc.hysaishi.cn

[T41] Perl：Hello World
来源：http://xed.0kj1m.cn

print "Hello\n";
来源：http://lbx.yuanzhike.top

[T42] Perl：变量类型
来源：http://ity.shzxlz.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://njc.shuidangran.top

[T43] Perl：字符串插值
来源：http://tfh.ppjwa.cn

"值: $a"
来源：http://bve.haohaochexian.top

[T44] Perl：条件
来源：http://ggy.hammf.cn

if ($a > 0) { print "正"; }
来源：http://afv.yanxiufei.cn

[T45] Perl：数组遍历
来源：http://bzu.shangyingyoupin.top

for my $x (@arr) { print $x; }
来源：http://zuy.andypj.xyz

[T46] Perl：哈希操作
来源：http://ovk.tanke756.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://zce.guannengcc.top

[T47] Perl：正则捕获
来源：http://wjy.tian-w.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://ise.yanxiufei.cn

[T48] Perl：正则替换
来源：http://ohl.gotoacloud.top

$s =~ s/old/new/g;
来源：http://nlt.shzxlz.cn

[T49] Perl：函数
来源：http://jdr.jqgfzy.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://knp.ydzc1.top

[T50] Perl：逐行读文件
来源：http://lpz.gotoacloud.top

open my $fh, "<", "a.txt" or die $!;
来源：http://dzt.ehwqpu.com

while (my $line = <$fh>) { print $line; }
来源：http://qzp.sufxvd.cn

[T51] Scala：Hello World
来源：http://dkm.birdmap.top

println("Hello")
来源：http://dkj.ydjk.org.cn

[T52] Scala：变量
来源：http://qwa.quarkkingdee.top

val a = 1;  var b = 2
来源：http://jmr.tarul.cn

[T53] Scala：字符串插值
来源：http://vpr.xuetiantiany.cn

s"值: $b"
来源：http://bbi.shuidangran.top

[T54] Scala：集合映射
来源：http://knm.jlsjyb.cn

List(1, 2, 3).map(_ * 2)
来源：http://bpy.ehwqpu.com

[T55] Scala：集合过滤
来源：http://uwy.feifeiyinyue.top

List(1, 2, 3).filter(_ > 1)
来源：http://bwv.jinghuilouyu.cn

[T56] Scala：样例类
来源：http://rgi.zhiwuduotai.top

case class User(name: String, age: Int)
来源：http://hys.yuxming.cn

[T57] Scala：模式匹配
来源：http://vyq.fehbvm.com

x match { case 1 => "一"; case _ => "其他" }
来源：http://sia.sjlbkw.cn

[T58] Scala：函数定义
来源：http://upv.dianchejie.cn

def add(a: Int, b: Int): Int = a + b
来源：http://krj.yangfankeji.com

[T59] Scala：循环
来源：http://how.hnqzz.top

for (i <- 1 to 10) println(i)
来源：http://lty.wangshuangyany.cn

[T60] Scala：折叠
来源：http://tfo.bbcook.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://isd.jianghu66.top

================================================================================
来源：http://fdj.zhongyouzk.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://mwb.316326.xyz

================================================================================
来源：http://huk.bbcook.cn

[U01] Py：创建虚拟环境
来源：http://mcx.mhx1999.top

python -m venv .venv && source .venv/bin/activate
来源：http://rol.yangfankeji.com

[U02] Py：导出 / 安装依赖
来源：http://wqx.dashuyun.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://xfn.vqdsnc.cn

[U03] Py：加载 .env 配置
来源：http://rlb.ywan-chungtsiang.top

from dotenv import load_dotenv; load_dotenv()
来源：http://tna.hongshengwenyu.top

[U04] Py：变量调试打印
来源：http://pkl.nanxuanxn.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://baw.pengpengdd.cyou

[U05] Py：列表去重且保序
来源：http://qwc.yj20258.top

list(dict.fromkeys(arr))
来源：http://zch.hcnkem.com

[U06] Py：合并两个字典
来源：http://wud.tianlin.xyz

{**a, **b}
来源：http://zbg.tarul.cn

[U07] Py：反转字典键值
来源：http://ywy.jinqigufen.top

{v: k for k, v in d.items()}
来源：http://sai.hfpthk.cn

[U08] Py：展平二维列表
来源：http://wbp.vehdjk.com

[y for x in nested for y in x]
来源：http://scs.fengsongda.top

[U09] Py：字典取最大值的键
来源：http://tei.redwolf501.top

max(d, key=d.get)
来源：http://ufq.zhengqikj.top

[U10] Py：按值排序字典
来源：http://gss.zdqjudy.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://sis.gzhubu.top

[U11] Py：生成器表达式
来源：http://uro.zhixingplan.top

(x * 2 for x in arr)
来源：http://prd.gzhubu.top

[U12] Py：取出现最多的 3 个元素
来源：http://amv.gotoacloud.top

Counter(arr).most_common(3)
来源：http://zhu.dianchejie.cn

[U13] Py：固定长度队列
来源：http://ykc.xuetiantiany.cn

deque(maxlen=10)
来源：http://lyh.meibo888.top

[U14] Py：分组收集到列表
来源：http://yit.cashguo.top

defaultdict(list)
来源：http://dgt.yj20258.top

[U15] Py：高精度计时
来源：http://kud.cqqwz.cn

t = time.perf_counter()
来源：http://fyu.jinqigufen.top

[U16] Py：命令行参数解析
来源：http://cbj.zhiwuduotai.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://dpf.vqdsnc.cn

[U17] Py：初始化日志
来源：http://cze.zhiwuduotai.top

logging.basicConfig(level=logging.INFO)
来源：http://dav.yuxming.cn

[U18] Py：预编译正则
来源：http://ghs.yanxiufei.cn

pat = re.compile(r"\d+")
来源：http://bas.wangdashe.top

[U19] Py：正则替换带回调
来源：http://mtf.iojbl.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://fxt.nanxinkj.top

[U20] Py：缓存函数结果
来源：http://xon.sufxvd.cn

@functools.lru_cache(maxsize=None)
来源：http://qhb.xingfuxueyuan.xyz

[U21] Py：自定义上下文管理器
来源：http://gag.quarkkingdee.top

@contextlib.contextmanager
来源：http://czz.uphjek.com

[U22] Py：矩阵转置
来源：http://mnb.nanxinkj.top

list(zip(*m))
来源：http://zmh.wangshuangyany.cn

[U23] Py：分块读取大文件
来源：http://ltt.cqqwz.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://foc.yuanzhike.top

[U24] Py：路径操作
来源：http://iym.zycfv.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://cxo.redwolf501.top

[U25] Py：CSV 按字典读
来源：http://etz.zdqjudy.top

csv.DictReader(f)
来源：http://inn.yangfankeji.com

[U26] Py：并发下载
来源：http://ghn.jinghuilouyu.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://tjz.hammf.cn

[U27] Py：异步 HTTP
来源：http://eub.gogol.net.cn

aiohttp.ClientSession() 配合 async with
来源：http://xcl.nanxuanxn.top

[U28] Py：类型别名
来源：http://kcl.feifeiyinyue.top

UserId = int
来源：http://ork.c1oappe.top

[U29] Py：属性校验
来源：http://hvw.sjlbkw.cn

@property 与 @x.setter 配合
来源：http://fsn.xinyue.icu

[U30] Py：数据类
来源：http://njm.dashuyun.cn

@dataclass(slots=True)
来源：http://zyy.vehdjk.com

[U31] Py：单测
来源：http://qhs.hcnkem.com

python -m pytest -q
来源：http://gor.yanxiufei.cn

[U32] Py：代码格式化
来源：http://waz.zhengqikj.top

ruff format . && ruff check --fix .
来源：http://zud.smart0.xyz

[U33] Py：打包发布
来源：http://bse.daxiang520.top

python -m build  （依赖 pyproject.toml）
来源：http://pxq.dianchejie.cn

[U34] Py：判断编码
来源：http://ugd.tian-w.cn

chardet.detect(raw)
来源：http://fol.shanyushiyangkeji.top

[U35] Py：发送邮件
来源：http://hvf.ivvv.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://gun.hnqzz.top

[U36] Py：定时任务
来源：http://brc.tian-w.cn

schedule.every(10).minutes.do(job)
来源：http://nor.chenlongwang.top

[U37] Py：读写 Excel
来源：http://wwx.ppjwa.cn

pandas.read_excel / DataFrame.to_excel
来源：http://qws.sjlbkw.cn

[U38] Py：获取脚本所在目录
来源：http://ykt.guowangkeji.top

Path(__file__).resolve().parent
来源：http://amc.xinyue.icu

[U39] Py：判断是否在交互环境
来源：http://sum.xuanzx.com

sys.stdout.isatty()
来源：http://nwn.guowangkeji.top

[U40] Py：打印到标准错误
来源：http://zbb.pycfn.com

print("err", file=sys.stderr)
来源：http://uux.zycfv.cn

[U41] PHP：初始化 Composer 项目
来源：http://ueb.c1oappe.top

composer init;  composer require guzzlehttp/guzzle
来源：http://oel.nwbrower.top

[U42] PHP：PSR-4 自动加载
来源：http://jnn.jqgufenzy.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://wzx.gaohongyu789.top

[U43] PHP：声明命名空间
来源：http://yfw.dashuyun.cn

namespace App\Http;
来源：http://shl.jinghuilouyu.cn

[U44] PHP：开启严格类型
来源：http://vpf.sufxvd.cn

declare(strict_types=1);
来源：http://feu.fehbvm.com

[U45] PHP：类型声明与返回类型
来源：http://geo.cdnleiting.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://fdf.gogol.net.cn

[U46] PHP：可空类型
来源：http://gqm.hnqzz.top

?string $name = null
来源：http://fer.jianghu66.top

[U47] PHP：联合类型
来源：http://fzv.nwbrower.top

int|string $id
来源：http://ozi.9152youxi.cn

[U48] PHP：纯枚举
来源：http://lom.sxryk.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://xkb.ydjk.org.cn

[U49] PHP：只读属性
来源：http://cem.vqdsnc.cn

public readonly string $name
来源：http://kjm.bjfxy.top

[U50] PHP：构造器属性提升
来源：http://fyh.jqgufenzy.top

public function __construct(private int $id) {}
来源：http://pde.tianlin.xyz

[U51] PHP：数组解构
来源：http://egn.hfpthk.cn

[$a, $b] = $arr;
来源：http://yzi.shanyushiyangkeji.top

[U52] PHP：箭头函数
来源：http://qii.yuxming.cn

$double = fn($x) => $x * 2;
来源：http://toy.ywan-chungtsiang.top

[U53] PHP：空合并运算符
来源：http://sim.sufxvd.cn

$v = $a ?? $b ?? "default";
来源：http://crr.yj20258888.top

[U54] PHP：空安全调用
来源：http://jyq.yuanzhike.top

$obj?->method()
来源：http://poa.jianghu66.top

[U55] PHP：match 表达式
来源：http://tnv.jinghuilouyu.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://vcj.vqdsnc.cn

[U56] PHP：命名参数
来源：http://qts.mhx1999.top

f(a: 1, b: 2)
来源：http://bkh.gotoacloud.top

[U57] PHP：字符串插值
来源：http://glb.redwolf501.top

"值: {$a}"
来源：http://nlc.aizwys.cn

[U58] PHP：数组三件套
来源：http://wuh.yvedp.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hym.chenzaomai.com

[U59] PHP：自定义排序
来源：http://bax.pengpengdd.cyou

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://bap.xingfuxueyuan.xyz

[U60] PHP：JSON 编解码
来源：http://zvd.ybcxt.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://imx.52xcode.cn

[U61] PHP：正则
来源：http://xpi.shanyushiyangkeji.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://scb.nanxinkj.top

[U62] PHP：日期对象
来源：http://cla.ivvv.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://yzl.xuanzx.com

[U63] PHP：文件读写
来源：http://cfr.tian-w.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://kpl.hcnkem.com

[U64] PHP：目录遍历
来源：http://ohb.hcnkem.com

glob("dir/*.php");  scandir("dir");
来源：http://kyk.fanxiaobao.xyz

[U65] PHP：会话
来源：http://xhs.zhengqikj.top

session_start();  $_SESSION["uid"] = 1;
来源：http://egy.yueranfly.top

[U66] PHP：设置 Cookie
来源：http://uek.tianlin.xyz

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://dms.aizwys.cn

[U67] PHP：处理文件上传
来源：http://fvt.fktsv.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://llz.fktsv.cn

[U68] PHP：PDO 连接
来源：http://sgu.xylfe.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://oua.gogol.net.cn

[U69] PHP：PDO 预处理
来源：http://ukl.ctjpmb.com

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://dir.jlsjyb.cn

[U70] PHP：PDO 事务
来源：http://wny.zhiwuduotai.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://phj.jinghuilouyu.cn

[U71] PHP：抛出异常
来源：http://gvf.jinqigfzy.top

throw new RuntimeException("失败", 500);
来源：http://vto.zhixingplan.top

[U72] PHP：写错误日志
来源：http://yeg.xuetiantiany.cn

error_log("失败: " . $e->getMessage());
来源：http://wdn.sjlbkw.cn

[U73] PHP：读取 ini 配置
来源：http://wpz.cheryme.top

parse_ini_file("config.ini", true)
来源：http://fai.xuetiantiany.cn

[U74] PHP：读取环境变量
来源：http://ytr.sysykeji.top

getenv("APP_ENV") ?: "production"
来源：http://njl.hysaishi.cn

[U75] PHP：依赖注入
来源：http://zlc.tianlin.xyz

composer require psr/container
来源：http://qkx.xingfuxueyuan.xyz

[U76] PHP：简单路由
来源：http://qwp.birdmap.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://uos.gotoacloud.top

[U77] PHP：模板渲染
来源：http://gjy.ehwqpu.com

composer require twig/twig
来源：http://fav.havefunace.top

[U78] PHP：单元测试
来源：http://hle.jqgfzy.top

composer require --dev phpunit/phpunit
来源：http://ggh.sxryk.cn

[U79] PHP：静态分析
来源：http://nll.cashguo.top

composer require --dev phpstan/phpstan
来源：http://zgd.c1oappe.top

[U80] PHP：代码规范修复
来源：http://kyc.yj20258888.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://vap.aizwys.cn

[U81] JS：初始化项目
来源：http://eqo.vqdsnc.cn

npm init -y;  npm i express
来源：http://ute.meibo888.top

[U82] JS：package.json 脚本
来源：http://jww.meibo888.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://afd.pycfn.com

[U83] JS：ES Module 导入导出
来源：http://sue.tian-w.cn

export const a = 1;  import { a } from "./m.js";
来源：http://aoj.sweek.top

[U84] JS：CommonJS 写法
来源：http://lki.andypj.xyz

module.exports = { a };  const { a } = require("./m");
来源：http://uvq.hongshengwenyu.top

[U85] JS：可选链
来源：http://xda.svipenyu.cn

a?.b?.c
来源：http://bpf.guowangkeji.top

[U86] JS：空值合并
来源：http://mwr.sufxvd.cn

a ?? b
来源：http://zdv.chenlongwang.top

[U87] JS：解构默认值
来源：http://zgv.yuanzhike.top

const { a = 1, b = 2 } = obj;
来源：http://iol.iojbl.cn

[U88] JS：对象展开合并
来源：http://hmk.kuanghao11.cn

{ ...a, ...b }
来源：http://rmi.0kj1m.cn

[U89] JS：数组去重
来源：http://aap.xuetiantiany.cn

[...new Set(arr)]
来源：http://gjp.yonumen.top

[U90] JS：数字数组排序
来源：http://sdr.pengpengdd.cyou

[...arr].sort((a, b) => a - b)
来源：http://vio.tian-w.cn

[U91] JS：对象键值遍历
来源：http://gcy.zhijiandao.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://zdy.yueranfly.top

[U92] JS：深拷贝
来源：http://hwd.zdbjq.cn

structuredClone(obj)
来源：http://rso.xylfe.cn

[U93] JS：模板字符串
来源：http://uuj.pengpengdd.cyou

`共 ${n} 条`
来源：http://ayi.guannengcc.top

[U94] JS：箭头函数
来源：http://jjm.yj202588.top

const double = x => x * 2;
来源：http://rwa.sufxvd.cn

[U95] JS：Promise 包装
来源：http://niw.haohaochexian.top

new Promise((resolve, reject) => {})
来源：http://sah.nwbrower.top

[U96] JS：async/await 与异常
来源：http://olc.sweek.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://sya.shzxlz.cn

[U97] JS：并发请求
来源：http://gkp.shuidangran.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://hin.hywenlv.cn

[U98] JS：fetch 带 JSON
来源：http://uww.shanyushiyangtech.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://xym.hfpthk.cn

[U99] JS：事件监听
来源：http://qff.0kj1m.cn

el.addEventListener("click", e => {})
来源：http://sme.feifeiyinyue.top

[U100] JS：DOM 查询
来源：http://fiv.ydzc1.top

document.querySelector(".item")
来源：http://evj.nwbrower.top

[U101] JS：classList 操作
来源：http://jqv.jyoumei.cn

el.classList.toggle("active")
来源：http://kiu.xuetiantiany.cn

[U102] JS：本地存储
来源：http://pev.dianchejie.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://yce.jqgufenzy.top

[U103] JS：定时器
来源：http://zmt.yongpay.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://pit.yuxming.cn

[U104] JS：防抖
来源：http://jcz.gzhubu.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://pqj.sxryk.cn

[U105] JS：节流
来源：http://goj.mhx1999.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://scw.zycfv.cn

[U106] JS：日期格式化
来源：http://fnt.zhijiandao.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://nxz.smart0.xyz

[U107] JS：数字千分位
来源：http://tjr.quarkkingdee.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://din.hesvh.cn

[U108] JS：随机整数
来源：http://yxb.c1oappe.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://azr.wangshuangyany.cn

[U109] JS：数组分组
来源：http://vpm.pycfn.com

Object.groupBy(arr, x => x.type)
来源：http://oxz.c1oappe.top

[U110] JS：数组分块
来源：http://aar.yongpay.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://omj.yueranfly.top

[U111] JS：对象转 Map
来源：http://wdr.gotoacloud.top

new Map(Object.entries(obj))
来源：http://gjg.zdqjudy.top

[U112] JS：字符串补位
来源：http://zbd.xingfuxueyuan.xyz

"7".padStart(3, "0")
来源：http://frn.tarul.cn

[U113] JS：正则替换全部
来源：http://gao.yuxming.cn

s.replaceAll("a", "b")
来源：http://vzv.zdbjq.cn

[U114] JS：JSON 深比较
来源：http://lvl.nanxinkj.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://rbq.iojbl.cn

[U115] JS：生成 UUID
来源：http://frq.snrcjt.cn

crypto.randomUUID()
来源：http://dbs.jinyuanbaomall.cn

[U116] JS：类型检查（JSDoc）
来源：http://hha.hcnkem.com

/** @param {string} name */ function f(name) {}
来源：http://mgg.cashguo.top


<!-- 参考信息 -->