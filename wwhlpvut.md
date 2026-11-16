代发 wailian999

[T35] Lua：字典表
来源：http://vhx.jinqigufen.top

local d = { a = 1 };  d.b = 2
来源：http://ldq.jiagoushi.top

[T36] Lua：函数
来源：http://viu.birdmap.top

function add(a, b) return a + b end
来源：http://gxz.aibaodan.cn

[T37] Lua：字符串拼接
来源：http://gjk.shzxlz.cn

"a" .. "b"
来源：http://kiw.cheryme.top

[T38] Lua：条件
来源：http://rpi.nwbrower.top

if x > 0 then print("正") end
来源：http://xho.jlsjyb.cn

[T39] Lua：模式匹配
来源：http://qgn.vqdsnc.cn

string.find(s, "%d+")
来源：http://dca.yongpay.top

[T40] Lua：元表
来源：http://uxx.dianchejie.cn

setmetatable({}, { __index = base })
来源：http://pqo.xingfuxueyuan.xyz

[T41] Perl：Hello World
来源：http://yoi.c1oappe.top

print "Hello\n";
来源：http://kct.jiagoushi.top

[T42] Perl：变量类型
来源：http://ptg.cheryme.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://yzp.cdnleiting.top

[T43] Perl：字符串插值
来源：http://eub.ybcxt.top

"值: $a"
来源：http://pan.shuidangran.top

[T44] Perl：条件
来源：http://nwo.tian-w.cn

if ($a > 0) { print "正"; }
来源：http://heg.tianlin.xyz

[T45] Perl：数组遍历
来源：http://yqf.9152youxi.cn

for my $x (@arr) { print $x; }
来源：http://nmd.c1oappe.top

[T46] Perl：哈希操作
来源：http://orw.cqqwz.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://krl.chenlongwang.top

[T47] Perl：正则捕获
来源：http://wiv.shzxlz.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://zxu.shanyushiyangkeji.top

[T48] Perl：正则替换
来源：http://dai.jlsjyb.cn

$s =~ s/old/new/g;
来源：http://zcv.jinyuanbaomall.cn

[T49] Perl：函数
来源：http://luj.dianchejie.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://sti.zdqjudy.top

[T50] Perl：逐行读文件
来源：http://bui.redwolf501.top

open my $fh, "<", "a.txt" or die $!;
来源：http://ppo.yfazqb.com

while (my $line = <$fh>) { print $line; }
来源：http://vrq.zycfv.cn

[T51] Scala：Hello World
来源：http://wrv.xingfuxueyuan.xyz

println("Hello")
来源：http://lkn.fengsongda.top

[T52] Scala：变量
来源：http://wmi.shanyushiyangtech.top

val a = 1;  var b = 2
来源：http://uqg.hnqzz.top

[T53] Scala：字符串插值
来源：http://qkj.c1oappe.top

s"值: $b"
来源：http://xkd.cdnleiting.top

[T54] Scala：集合映射
来源：http://ruu.aizwys.cn

List(1, 2, 3).map(_ * 2)
来源：http://prh.yueranfly.top

[T55] Scala：集合过滤
来源：http://kaq.jianghu66.top

List(1, 2, 3).filter(_ > 1)
来源：http://cgn.shangyingyoupin.top

[T56] Scala：样例类
来源：http://qzu.zhiwuduotai.top

case class User(name: String, age: Int)
来源：http://gdn.sweek.top

[T57] Scala：模式匹配
来源：http://izl.zhixingplan.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://xhj.sweek.top

[T58] Scala：函数定义
来源：http://qbe.cheryme.top

def add(a: Int, b: Int): Int = a + b
来源：http://wea.gaohongyu789.top

[T59] Scala：循环
来源：http://opb.hywenlv.cn

for (i <- 1 to 10) println(i)
来源：http://swx.tianlin.xyz

[T60] Scala：折叠
来源：http://ekq.fktsv.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://rpm.jianghu66.top

================================================================================
来源：http://ihe.fehbvm.com

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hmi.yanxiufei.cn

================================================================================
来源：http://xka.shzxlz.cn

[U01] Py：创建虚拟环境
来源：http://fjx.quarkkingdee.top

python -m venv .venv && source .venv/bin/activate
来源：http://prd.hnqzz.top

[U02] Py：导出 / 安装依赖
来源：http://ccj.nanxinkj.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://mat.ybcxt.top

[U03] Py：加载 .env 配置
来源：http://njj.hywenlv.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://xfh.nanxinkj.top

[U04] Py：变量调试打印
来源：http://ncu.yj20258888.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://qct.snrcjt.cn

[U05] Py：列表去重且保序
来源：http://qnt.haohaochexian.top

list(dict.fromkeys(arr))
来源：http://kna.haohaochexian.top

[U06] Py：合并两个字典
来源：http://lbp.gzhubu.top

{**a, **b}
来源：http://qqs.52xcode.cn

[U07] Py：反转字典键值
来源：http://jrd.gaohongyu789.top

{v: k for k, v in d.items()}
来源：http://hpo.hcnkem.com

[U08] Py：展平二维列表
来源：http://ekh.nanxuanxn.top

[y for x in nested for y in x]
来源：http://mgr.ivvv.top

[U09] Py：字典取最大值的键
来源：http://rpz.shangyingyoupin.top

max(d, key=d.get)
来源：http://qmh.fanxiaobao.xyz

[U10] Py：按值排序字典
来源：http://jcj.yvedp.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://jgh.hammf.cn

[U11] Py：生成器表达式
来源：http://kpc.iojbl.cn

(x * 2 for x in arr)
来源：http://ruv.sjlbkw.cn

[U12] Py：取出现最多的 3 个元素
来源：http://eva.fengsongda.top

Counter(arr).most_common(3)
来源：http://thn.feifeiyinyue.top

[U13] Py：固定长度队列
来源：http://aej.jianghu66.top

deque(maxlen=10)
来源：http://hkr.bbcook.cn

[U14] Py：分组收集到列表
来源：http://igg.havefunace.top

defaultdict(list)
来源：http://rcz.cucudq.cn

[U15] Py：高精度计时
来源：http://sgw.jinqigufen.top

t = time.perf_counter()
来源：http://nus.0kj1m.cn

[U16] Py：命令行参数解析
来源：http://ech.iojbl.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://ufj.ehwqpu.com

[U17] Py：初始化日志
来源：http://xxx.zdbjq.cn

logging.basicConfig(level=logging.INFO)
来源：http://zbc.cqqwz.cn

[U18] Py：预编译正则
来源：http://kpz.yj20258888.top

pat = re.compile(r"\d+")
来源：http://mjn.jiagoushi.top

[U19] Py：正则替换带回调
来源：http://bbx.jinyuanbaomall.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://uud.meibo888.top

[U20] Py：缓存函数结果
来源：http://pdd.dashuyun.cn

@functools.lru_cache(maxsize=None)
来源：http://rrz.zhiwuduotai.top

[U21] Py：自定义上下文管理器
来源：http://pbg.sufxvd.cn

@contextlib.contextmanager
来源：http://tas.yj202588.top

[U22] Py：矩阵转置
来源：http://ymw.cashguo.top

list(zip(*m))
来源：http://qvk.zhengqikj.top

[U23] Py：分块读取大文件
来源：http://knq.xinyue.icu

for chunk in iter(lambda: f.read(8192), b""):
来源：http://acg.chenjidiqi.icu

[U24] Py：路径操作
来源：http://ojs.xinyue.icu

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://lyg.chenjidiqi.icu

[U25] Py：CSV 按字典读
来源：http://ebl.yanxiufei.cn

csv.DictReader(f)
来源：http://vgu.jinyuanbaomall.cn

[U26] Py：并发下载
来源：http://xzd.jqgfzy.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://ovm.sxryk.cn

[U27] Py：异步 HTTP
来源：http://ihq.nwbrower.top

aiohttp.ClientSession() 配合 async with
来源：http://tiz.yj202588.top

[U28] Py：类型别名
来源：http://hmb.xziqi.cn

UserId = int
来源：http://ixe.aizwys.cn

[U29] Py：属性校验
来源：http://cnb.jlsjyb.cn

@property 与 @x.setter 配合
来源：http://rzm.vqdsnc.cn

[U30] Py：数据类
来源：http://cck.ywan-chungtsiang.top

@dataclass(slots=True)
来源：http://vuj.nwbrower.top

[U31] Py：单测
来源：http://kwk.zycfv.cn

python -m pytest -q
来源：http://aor.zdbjq.cn

[U32] Py：代码格式化
来源：http://ikv.xinyue.icu

ruff format . && ruff check --fix .
来源：http://ycx.zdqjudy.top

[U33] Py：打包发布
来源：http://ixd.redwolf501.top

python -m build  （依赖 pyproject.toml）
来源：http://lmi.yj20258888.top

[U34] Py：判断编码
来源：http://anc.svipenyu.cn

chardet.detect(raw)
来源：http://luy.ppjwa.cn

[U35] Py：发送邮件
来源：http://mmf.daxiang520.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://njv.jinqigufen.top

[U36] Py：定时任务
来源：http://kga.zhiwuduotai.top

schedule.every(10).minutes.do(job)
来源：http://qzl.yueranfly.top

[U37] Py：读写 Excel
来源：http://bsu.fzhhl.top

pandas.read_excel / DataFrame.to_excel
来源：http://bnr.bbcook.cn

[U38] Py：获取脚本所在目录
来源：http://qpt.sweek.top

Path(__file__).resolve().parent
来源：http://dln.chenjidiqi.icu

[U39] Py：判断是否在交互环境
来源：http://qwj.ywan-chungtsiang.top

sys.stdout.isatty()
来源：http://epr.yfazqb.com

[U40] Py：打印到标准错误
来源：http://dqm.zdqjudy.top

print("err", file=sys.stderr)
来源：http://ety.ppjwa.cn

[U41] PHP：初始化 Composer 项目
来源：http://osl.fehbvm.com

composer init;  composer require guzzlehttp/guzzle
来源：http://aek.nanxinkj.top

[U42] PHP：PSR-4 自动加载
来源：http://pby.mhx1999.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://usy.yanxiufei.cn

[U43] PHP：声明命名空间
来源：http://nlf.jianghu66.top

namespace App\Http;
来源：http://ife.dashuyun.cn

[U44] PHP：开启严格类型
来源：http://acl.shuidangran.top

declare(strict_types=1);
来源：http://ovj.yvedp.cn

[U45] PHP：类型声明与返回类型
来源：http://jrz.wangdashe.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://fpx.fanxiaobao.xyz

[U46] PHP：可空类型
来源：http://ttn.316326.xyz

?string $name = null
来源：http://ddg.aizwys.cn

[U47] PHP：联合类型
来源：http://jku.shanyushiyangtech.top

int|string $id
来源：http://ynw.birdmap.top

[U48] PHP：纯枚举
来源：http://ewe.zycfv.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://nzt.jinghuilouyu.cn

[U49] PHP：只读属性
来源：http://coz.havefunace.top

public readonly string $name
来源：http://mef.quarkkingdee.top

[U50] PHP：构造器属性提升
来源：http://abf.chenzaomai.com

public function __construct(private int $id) {}
来源：http://aol.uphjek.com

[U51] PHP：数组解构
来源：http://nwn.yj202588.top

[$a, $b] = $arr;
来源：http://tzs.yuanzhike.top

[U52] PHP：箭头函数
来源：http://fkv.hesvh.cn

$double = fn($x) => $x * 2;
来源：http://van.cdnleiting.top

[U53] PHP：空合并运算符
来源：http://syt.birdmap.top

$v = $a ?? $b ?? "default";
来源：http://uxc.dianchejie.cn

[U54] PHP：空安全调用
来源：http://jzu.zhengqikj.top

$obj?->method()
来源：http://roi.daxiang520.top

[U55] PHP：match 表达式
来源：http://hjq.birdmap.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://giv.meibo888.top

[U56] PHP：命名参数
来源：http://rhm.xingfuxueyuan.xyz

f(a: 1, b: 2)
来源：http://rly.pycfn.com

[U57] PHP：字符串插值
来源：http://jmz.pycfn.com

"值: {$a}"
来源：http://vxz.fehbvm.com

[U58] PHP：数组三件套
来源：http://boa.haohaochexian.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://jsa.snrcjt.cn

[U59] PHP：自定义排序
来源：http://skh.nanxinkj.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://bhx.jianghu66.top

[U60] PHP：JSON 编解码
来源：http://ass.c1oappe.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://rph.wangdashe.top

[U61] PHP：正则
来源：http://wja.zhaomingkeji.xyz

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://agn.cucudq.cn

[U62] PHP：日期对象
来源：http://vao.shangyingyoupin.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://coz.yuxming.cn

[U63] PHP：文件读写
来源：http://ftf.tarul.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://lom.ehwqpu.com

[U64] PHP：目录遍历
来源：http://nuj.gotoacloud.top

glob("dir/*.php");  scandir("dir");
来源：http://ljp.zycfv.cn

[U65] PHP：会话
来源：http://tlu.uphjek.com

session_start();  $_SESSION["uid"] = 1;
来源：http://mri.316326.xyz

[U66] PHP：设置 Cookie
来源：http://cou.zhoulong.xyz

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://prb.yuanzhike.top

[U67] PHP：处理文件上传
来源：http://rxc.meibo888.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://twr.xinyue.icu

[U68] PHP：PDO 连接
来源：http://tzr.yonumen.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://vjg.gogol.net.cn

[U69] PHP：PDO 预处理
来源：http://prq.xziqi.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://lil.cdnleiting.top

[U70] PHP：PDO 事务
来源：http://rpg.c1oappe.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://vig.yuxming.cn

[U71] PHP：抛出异常
来源：http://rsz.uphjek.com

throw new RuntimeException("失败", 500);
来源：http://uny.ppjwa.cn

[U72] PHP：写错误日志
来源：http://ybk.vqdsnc.cn

error_log("失败: " . $e->getMessage());
来源：http://fuy.aibaodan.cn

[U73] PHP：读取 ini 配置
来源：http://swz.ydjk.org.cn

parse_ini_file("config.ini", true)
来源：http://zuq.ctjpmb.com

[U74] PHP：读取环境变量
来源：http://cmi.snrcjt.cn

getenv("APP_ENV") ?: "production"
来源：http://oai.zhiwuduotai.top

[U75] PHP：依赖注入
来源：http://mao.cheryme.top

composer require psr/container
来源：http://ari.aibaodan.cn

[U76] PHP：简单路由
来源：http://fcu.ehwqpu.com

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://lbv.zhiwuduotai.top

[U77] PHP：模板渲染
来源：http://nzo.gaohongyu789.top

composer require twig/twig
来源：http://zke.zhongyouzk.top

[U78] PHP：单元测试
来源：http://ymv.yj20258.top

composer require --dev phpunit/phpunit
来源：http://yit.zdbjq.cn

[U79] PHP：静态分析
来源：http://rhd.pycfn.com

composer require --dev phpstan/phpstan
来源：http://nqs.dashuyun.cn

[U80] PHP：代码规范修复
来源：http://gfb.fengsongda.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://nyi.feifeiyinyue.top

[U81] JS：初始化项目
来源：http://rhv.daria6918.cn

npm init -y;  npm i express
来源：http://vbz.dianchejie.cn

[U82] JS：package.json 脚本
来源：http://elt.chenlongwang.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://ubr.jianghu66.top

[U83] JS：ES Module 导入导出
来源：http://ojz.chenjidiqi.icu

export const a = 1;  import { a } from "./m.js";
来源：http://eyy.fehbvm.com

[U84] JS：CommonJS 写法
来源：http://jcb.zhijiandao.cn

module.exports = { a };  const { a } = require("./m");
来源：http://qyl.jinqigfzy.top

[U85] JS：可选链
来源：http://cqf.hnqzz.top

a?.b?.c
来源：http://byf.vehdjk.com

[U86] JS：空值合并
来源：http://hkw.vqdsnc.cn

a ?? b
来源：http://vmr.meibo888.top

[U87] JS：解构默认值
来源：http://ckr.jiagoushi.top

const { a = 1, b = 2 } = obj;
来源：http://oys.pycfn.com

[U88] JS：对象展开合并
来源：http://uzx.nanxuanxn.top

{ ...a, ...b }
来源：http://fbm.tanke756.top

[U89] JS：数组去重
来源：http://gjv.xuanzx.com

[...new Set(arr)]
来源：http://hbe.fzhhl.top

[U90] JS：数字数组排序
来源：http://bwk.jlsjyb.cn

[...arr].sort((a, b) => a - b)
来源：http://brd.gaohongyu789.top

[U91] JS：对象键值遍历
来源：http://tnt.jqgufenzy.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://bqd.pengpengdd.cyou

[U92] JS：深拷贝
来源：http://oaa.chenzaomai.com

structuredClone(obj)
来源：http://dac.gzhubu.top

[U93] JS：模板字符串
来源：http://jts.daria6918.cn

`共 ${n} 条`
来源：http://hkt.yj20258.top

[U94] JS：箭头函数
来源：http://zwk.tanke756.top

const double = x => x * 2;
来源：http://eai.yvedp.cn

[U95] JS：Promise 包装
来源：http://ejo.zhongyouzk.top

new Promise((resolve, reject) => {})
来源：http://sym.nanxinkj.top

[U96] JS：async/await 与异常
来源：http://pxr.guowangkeji.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://qzd.zhaomingkeji.xyz

[U97] JS：并发请求
来源：http://ugv.zhiwuduotai.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://qpf.xylfe.cn

[U98] JS：fetch 带 JSON
来源：http://dvh.zhengqikj.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://bkd.vqdsnc.cn

[U99] JS：事件监听
来源：http://npr.ybcxt.top

el.addEventListener("click", e => {})
来源：http://imd.yuanzhike.top

[U100] JS：DOM 查询
来源：http://cuk.zhijiandao.cn

document.querySelector(".item")
来源：http://ugu.yuanzhike.top

[U101] JS：classList 操作
来源：http://xrw.sysykeji.top

el.classList.toggle("active")
来源：http://fsc.jinqigfzy.top

[U102] JS：本地存储
来源：http://vzt.xuetiantiany.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://bgp.yuanzhike.top

[U103] JS：定时器
来源：http://rhd.tianlin.xyz

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://gnr.redwolf501.top

[U104] JS：防抖
来源：http://aoi.hcnkem.com

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://iwb.zhengqikj.top

[U105] JS：节流
来源：http://vud.hfpthk.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://qik.havefunace.top

[U106] JS：日期格式化
来源：http://fju.shanyushiyangtech.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://kve.sufxvd.cn

[U107] JS：数字千分位
来源：http://qff.vqdsnc.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://boe.redwolf501.top

[U108] JS：随机整数
来源：http://mum.shangyingyoupin.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://fpt.jyoumei.cn

[U109] JS：数组分组
来源：http://fry.hnxiangtu.top

Object.groupBy(arr, x => x.type)
来源：http://yjr.yongpay.top

[U110] JS：数组分块
来源：http://hwd.redwolf501.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://cid.yj202588.top

[U111] JS：对象转 Map
来源：http://qbl.zhongyouzk.top

new Map(Object.entries(obj))
来源：http://oai.sufxvd.cn

[U112] JS：字符串补位
来源：http://qfm.jlsjyb.cn

"7".padStart(3, "0")
来源：http://tsa.hywenlv.cn

[U113] JS：正则替换全部
来源：http://nar.guannengcc.top

s.replaceAll("a", "b")
来源：http://hmn.jqgfzy.top

[U114] JS：JSON 深比较
来源：http://lje.jinqigufen.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://czs.fktsv.cn

[U115] JS：生成 UUID
来源：http://qen.dashuyun.cn

crypto.randomUUID()
来源：http://sux.ybcxt.top

[U116] JS：类型检查（JSDoc）
来源：http://toy.bjfxy.top

/** @param {string} name */ function f(name) {}
来源：http://wku.aibaodan.cn

[U117] JS：单元测试
来源：http://qrx.aibaodan.cn

npm i -D vitest;  npx vitest
来源：http://nsd.fehbvm.com

[U118] JS：开发服务器
来源：http://ame.gotoacloud.top

npm i -D vite;  npx vite
来源：http://xvg.c1oappe.top

[U119] JS：生产构建
来源：http://wtg.bjfxy.top

npx vite build
来源：http://mlj.jianghu66.top

[U120] JS：读取环境变量（Vite）
来源：http://sdk.yvedp.cn

import.meta.env.VITE_API_URL
来源：http://zac.52xcode.cn

================================================================================
来源：http://pwl.feifeiyinyue.top

统计汇总
来源：http://mpn.svipenyu.cn

================================================================================
来源：http://gfo.jianghu66.top

按语言统计（条）：
来源：http://ctv.yuxming.cn


<!-- 参考信息 -->