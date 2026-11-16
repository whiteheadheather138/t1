代发 wailian999

[T39] Lua：模式匹配
来源：http://pwr.bjfxy.top

string.find(s, "%d+")
来源：http://ofk.dashuyun.cn

[T40] Lua：元表
来源：http://ida.shzxlz.cn

setmetatable({}, { __index = base })
来源：http://dgs.hfpthk.cn

[T41] Perl：Hello World
来源：http://jir.uphjek.com

print "Hello\n";
来源：http://xds.chenlongwang.top

[T42] Perl：变量类型
来源：http://pbk.zhengqikj.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://uwp.9152youxi.cn

[T43] Perl：字符串插值
来源：http://nnc.cashguo.top

"值: $a"
来源：http://gyf.yj20258888.top

[T44] Perl：条件
来源：http://ngy.yj20258888.top

if ($a > 0) { print "正"; }
来源：http://bow.chenjidiqi.icu

[T45] Perl：数组遍历
来源：http://qye.bbcook.cn

for my $x (@arr) { print $x; }
来源：http://szf.ywan-chungtsiang.top

[T46] Perl：哈希操作
来源：http://cxy.sufxvd.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://aqw.zdqjudy.top

[T47] Perl：正则捕获
来源：http://fal.fzhhl.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://gdh.xuanzx.com

[T48] Perl：正则替换
来源：http://pkp.nanxuanxn.top

$s =~ s/old/new/g;
来源：http://iik.zdbjq.cn

[T49] Perl：函数
来源：http://pva.ivvv.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://nrm.vehdjk.com

[T50] Perl：逐行读文件
来源：http://rzf.zhixingplan.top

open my $fh, "<", "a.txt" or die $!;
来源：http://ipz.cucudq.cn

while (my $line = <$fh>) { print $line; }
来源：http://ijc.mhx1999.top

[T51] Scala：Hello World
来源：http://byw.fehbvm.com

println("Hello")
来源：http://ufk.fzhhl.top

[T52] Scala：变量
来源：http://oas.hywenlv.cn

val a = 1;  var b = 2
来源：http://ugv.zhengqikj.top

[T53] Scala：字符串插值
来源：http://cdv.gzhubu.top

s"值: $b"
来源：http://myg.jinqigufen.top

[T54] Scala：集合映射
来源：http://pgo.yonumen.top

List(1, 2, 3).map(_ * 2)
来源：http://yvx.iojbl.cn

[T55] Scala：集合过滤
来源：http://unr.uphjek.com

List(1, 2, 3).filter(_ > 1)
来源：http://zdw.yj20258.top

[T56] Scala：样例类
来源：http://xcw.vehdjk.com

case class User(name: String, age: Int)
来源：http://sew.mhx1999.top

[T57] Scala：模式匹配
来源：http://ybw.ivvv.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://hny.tianlin.xyz

[T58] Scala：函数定义
来源：http://uim.fanxiaobao.xyz

def add(a: Int, b: Int): Int = a + b
来源：http://fpd.yonumen.top

[T59] Scala：循环
来源：http://bwy.hcnkem.com

for (i <- 1 to 10) println(i)
来源：http://ymg.chenjidiqi.icu

[T60] Scala：折叠
来源：http://cnu.jinqigufen.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://dvh.xuetiantiany.cn

================================================================================
来源：http://yny.tian-w.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://ejs.yonumen.top

================================================================================
来源：http://zot.vehdjk.com

[U01] Py：创建虚拟环境
来源：http://lau.pengpengdd.cyou

python -m venv .venv && source .venv/bin/activate
来源：http://qle.yuanzhike.top

[U02] Py：导出 / 安装依赖
来源：http://xsk.cdnleiting.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://nyi.tian-w.cn

[U03] Py：加载 .env 配置
来源：http://fkr.epnwcf.com

from dotenv import load_dotenv; load_dotenv()
来源：http://vrf.jinyuanbaomall.cn

[U04] Py：变量调试打印
来源：http://mfj.yonumen.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://qhs.fzhhl.top

[U05] Py：列表去重且保序
来源：http://vio.shangyingyoupin.top

list(dict.fromkeys(arr))
来源：http://vzo.shzxlz.cn

[U06] Py：合并两个字典
来源：http://tcf.shanyushiyangkeji.top

{**a, **b}
来源：http://hac.andypj.xyz

[U07] Py：反转字典键值
来源：http://cmf.ivvv.top

{v: k for k, v in d.items()}
来源：http://jgh.nanxuanxn.top

[U08] Py：展平二维列表
来源：http://sll.jinqigfzy.top

[y for x in nested for y in x]
来源：http://cig.fehbvm.com

[U09] Py：字典取最大值的键
来源：http://mqd.bjfxy.top

max(d, key=d.get)
来源：http://xwd.zycfv.cn

[U10] Py：按值排序字典
来源：http://rwt.daria6918.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://thb.dianchejie.cn

[U11] Py：生成器表达式
来源：http://wfa.nwbrower.top

(x * 2 for x in arr)
来源：http://rgz.sweek.top

[U12] Py：取出现最多的 3 个元素
来源：http://loh.hysaishi.cn

Counter(arr).most_common(3)
来源：http://rye.xingfuxueyuan.xyz

[U13] Py：固定长度队列
来源：http://dem.gotoacloud.top

deque(maxlen=10)
来源：http://pga.ehwqpu.com

[U14] Py：分组收集到列表
来源：http://ahq.jinqigufen.top

defaultdict(list)
来源：http://ukc.meibo888.top

[U15] Py：高精度计时
来源：http://ynx.xinyue.icu

t = time.perf_counter()
来源：http://pxa.jlsjyb.cn

[U16] Py：命令行参数解析
来源：http://edl.zhengqikj.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://avh.jiagoushi.top

[U17] Py：初始化日志
来源：http://atn.zhoulong.xyz

logging.basicConfig(level=logging.INFO)
来源：http://zts.sufxvd.cn

[U18] Py：预编译正则
来源：http://lkh.yongpay.top

pat = re.compile(r"\d+")
来源：http://wkt.nanxinkj.top

[U19] Py：正则替换带回调
来源：http://idh.zhengqikj.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://fhe.hcnkem.com

[U20] Py：缓存函数结果
来源：http://wka.vqdsnc.cn

@functools.lru_cache(maxsize=None)
来源：http://ltw.zhiwuduotai.top

[U21] Py：自定义上下文管理器
来源：http://ylo.hywenlv.cn

@contextlib.contextmanager
来源：http://dzp.cqqwz.cn

[U22] Py：矩阵转置
来源：http://jcy.nanxinkj.top

list(zip(*m))
来源：http://tof.dianchejie.cn

[U23] Py：分块读取大文件
来源：http://kie.ivvv.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://yvi.fktsv.cn

[U24] Py：路径操作
来源：http://zsj.xuanzx.com

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://yhd.haohaochexian.top

[U25] Py：CSV 按字典读
来源：http://ysz.ydjk.org.cn

csv.DictReader(f)
来源：http://eri.xuanzx.com

[U26] Py：并发下载
来源：http://qiz.tarul.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://icl.shanyushiyangtech.top

[U27] Py：异步 HTTP
来源：http://qrb.chenzaomai.com

aiohttp.ClientSession() 配合 async with
来源：http://xrh.jlsjyb.cn

[U28] Py：类型别名
来源：http://enu.mhx1999.top

UserId = int
来源：http://kdi.guannengcc.top

[U29] Py：属性校验
来源：http://wgp.yangfankeji.com

@property 与 @x.setter 配合
来源：http://enn.0kj1m.cn

[U30] Py：数据类
来源：http://fuv.xuanzx.com

@dataclass(slots=True)
来源：http://yds.yj202588.top

[U31] Py：单测
来源：http://zaw.daria6918.cn

python -m pytest -q
来源：http://rdr.zdbjq.cn

[U32] Py：代码格式化
来源：http://ewq.gzhubu.top

ruff format . && ruff check --fix .
来源：http://lwf.birdmap.top

[U33] Py：打包发布
来源：http://jxj.hysaishi.cn

python -m build  （依赖 pyproject.toml）
来源：http://joy.uphjek.com

[U34] Py：判断编码
来源：http://lyy.ehwqpu.com

chardet.detect(raw)
来源：http://zzt.xinyue.icu

[U35] Py：发送邮件
来源：http://gkv.cucudq.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://knd.yanxiufei.cn

[U36] Py：定时任务
来源：http://lhn.hesvh.cn

schedule.every(10).minutes.do(job)
来源：http://ggs.guowangkeji.top

[U37] Py：读写 Excel
来源：http://hti.hesvh.cn

pandas.read_excel / DataFrame.to_excel
来源：http://xmh.yongpay.top

[U38] Py：获取脚本所在目录
来源：http://rll.pycfn.com

Path(__file__).resolve().parent
来源：http://rqk.zhongyouzk.top

[U39] Py：判断是否在交互环境
来源：http://kyc.gogol.net.cn

sys.stdout.isatty()
来源：http://wvl.mhx1999.top

[U40] Py：打印到标准错误
来源：http://yqq.redwolf501.top

print("err", file=sys.stderr)
来源：http://wny.hammf.cn

[U41] PHP：初始化 Composer 项目
来源：http://jpj.quarkkingdee.top

composer init;  composer require guzzlehttp/guzzle
来源：http://vte.yfazqb.com

[U42] PHP：PSR-4 自动加载
来源：http://xrd.shuidangran.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hjr.jinqigfzy.top

[U43] PHP：声明命名空间
来源：http://svx.fktsv.cn

namespace App\Http;
来源：http://jwa.zhaomingkeji.xyz

[U44] PHP：开启严格类型
来源：http://ylh.hywenlv.cn

declare(strict_types=1);
来源：http://vaz.daria6918.cn

[U45] PHP：类型声明与返回类型
来源：http://wpn.epnwcf.com

function add(int $a, int $b): int { return $a + $b; }
来源：http://kfr.ywan-chungtsiang.top

[U46] PHP：可空类型
来源：http://ccl.yj20258888.top

?string $name = null
来源：http://shp.tianlin.xyz

[U47] PHP：联合类型
来源：http://ewf.zhijiandao.cn

int|string $id
来源：http://bac.zdqjudy.top

[U48] PHP：纯枚举
来源：http://xeu.c1oappe.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://dtf.tanke756.top

[U49] PHP：只读属性
来源：http://wqc.shanyushiyangkeji.top

public readonly string $name
来源：http://wfz.hnxiangtu.top

[U50] PHP：构造器属性提升
来源：http://iuk.tanke756.top

public function __construct(private int $id) {}
来源：http://quf.nanxinkj.top

[U51] PHP：数组解构
来源：http://mfj.jianghu66.top

[$a, $b] = $arr;
来源：http://ick.cqqwz.cn

[U52] PHP：箭头函数
来源：http://giw.nwbrower.top

$double = fn($x) => $x * 2;
来源：http://ajg.316326.xyz

[U53] PHP：空合并运算符
来源：http://zec.ydzc1.top

$v = $a ?? $b ?? "default";
来源：http://cws.vehdjk.com

[U54] PHP：空安全调用
来源：http://msr.fzhhl.top

$obj?->method()
来源：http://nuw.ybcxt.top

[U55] PHP：match 表达式
来源：http://iwa.wangshuangyany.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://yhu.cqqwz.cn

[U56] PHP：命名参数
来源：http://dqs.zhongyouzk.top

f(a: 1, b: 2)
来源：http://xci.gogol.net.cn

[U57] PHP：字符串插值
来源：http://vbk.redwolf501.top

"值: {$a}"
来源：http://xbl.uphjek.com

[U58] PHP：数组三件套
来源：http://vin.birdmap.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://sqj.chenlongwang.top

[U59] PHP：自定义排序
来源：http://wni.uphjek.com

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://saz.ppjwa.cn

[U60] PHP：JSON 编解码
来源：http://oaz.jyoumei.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://ugw.ctjpmb.com

[U61] PHP：正则
来源：http://ksy.sjlbkw.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://qeh.dianchejie.cn

[U62] PHP：日期对象
来源：http://hze.jinyuanbaomall.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://fud.tian-w.cn

[U63] PHP：文件读写
来源：http://khu.ywan-chungtsiang.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://amb.havefunace.top

[U64] PHP：目录遍历
来源：http://jiw.jqgfzy.top

glob("dir/*.php");  scandir("dir");
来源：http://phz.ywan-chungtsiang.top

[U65] PHP：会话
来源：http://fds.hnxiangtu.top

session_start();  $_SESSION["uid"] = 1;
来源：http://ufy.chenjidiqi.icu

[U66] PHP：设置 Cookie
来源：http://wbc.yfazqb.com

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://qxb.dashuyun.cn

[U67] PHP：处理文件上传
来源：http://ker.daria6918.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://paw.tianlin.xyz

[U68] PHP：PDO 连接
来源：http://tkj.epnwcf.com

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://ooa.zhiwuduotai.top

[U69] PHP：PDO 预处理
来源：http://fdl.snrcjt.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://zmq.gzhubu.top

[U70] PHP：PDO 事务
来源：http://fgp.gaohongyu789.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://qpc.yonumen.top

[U71] PHP：抛出异常
来源：http://lna.mhx1999.top

throw new RuntimeException("失败", 500);
来源：http://rpi.cheryme.top

[U72] PHP：写错误日志
来源：http://oci.nanxinkj.top

error_log("失败: " . $e->getMessage());
来源：http://zfu.shangyingyoupin.top

[U73] PHP：读取 ini 配置
来源：http://ljy.yonumen.top

parse_ini_file("config.ini", true)
来源：http://rke.shangyingyoupin.top

[U74] PHP：读取环境变量
来源：http://rne.hnqzz.top

getenv("APP_ENV") ?: "production"
来源：http://xls.xylfe.cn

[U75] PHP：依赖注入
来源：http://kws.zhengqikj.top

composer require psr/container
来源：http://wio.haohaochexian.top

[U76] PHP：简单路由
来源：http://xmu.zhongyouzk.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://gud.yonumen.top

[U77] PHP：模板渲染
来源：http://mhh.redwolf501.top

composer require twig/twig
来源：http://otf.jianghu66.top

[U78] PHP：单元测试
来源：http://mvz.dianchejie.cn

composer require --dev phpunit/phpunit
来源：http://itn.shanyushiyangtech.top

[U79] PHP：静态分析
来源：http://fxr.shangyingyoupin.top

composer require --dev phpstan/phpstan
来源：http://rdy.guannengcc.top

[U80] PHP：代码规范修复
来源：http://iax.birdmap.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://bxz.hnxiangtu.top

[U81] JS：初始化项目
来源：http://mtg.bjfxy.top

npm init -y;  npm i express
来源：http://eff.cashguo.top

[U82] JS：package.json 脚本
来源：http://ged.hysaishi.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://xyy.havefunace.top

[U83] JS：ES Module 导入导出
来源：http://kds.shzxlz.cn

export const a = 1;  import { a } from "./m.js";
来源：http://jtw.wangdashe.top

[U84] JS：CommonJS 写法
来源：http://mbt.nwbrower.top

module.exports = { a };  const { a } = require("./m");
来源：http://kmh.jyoumei.cn

[U85] JS：可选链
来源：http://zxz.mhx1999.top

a?.b?.c
来源：http://elp.fehbvm.com

[U86] JS：空值合并
来源：http://kwi.gotoacloud.top

a ?? b
来源：http://jwt.sufxvd.cn

[U87] JS：解构默认值
来源：http://obi.vehdjk.com

const { a = 1, b = 2 } = obj;
来源：http://erv.mhx1999.top

[U88] JS：对象展开合并
来源：http://dyd.fktsv.cn

{ ...a, ...b }
来源：http://naa.quarkkingdee.top

[U89] JS：数组去重
来源：http://jna.ydzc1.top

[...new Set(arr)]
来源：http://frd.dashuyun.cn

[U90] JS：数字数组排序
来源：http://pjj.tanke756.top

[...arr].sort((a, b) => a - b)
来源：http://rlz.cheryme.top

[U91] JS：对象键值遍历
来源：http://gkm.shanyushiyangkeji.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://blw.havefunace.top

[U92] JS：深拷贝
来源：http://aox.zhixingplan.top

structuredClone(obj)
来源：http://yre.zhoulong.xyz

[U93] JS：模板字符串
来源：http://rdn.jlsjyb.cn

`共 ${n} 条`
来源：http://hwf.shanyushiyangtech.top

[U94] JS：箭头函数
来源：http://fho.shanyushiyangkeji.top

const double = x => x * 2;
来源：http://duv.meibo888.top

[U95] JS：Promise 包装
来源：http://aca.wangshuangyany.cn

new Promise((resolve, reject) => {})
来源：http://xza.fzhhl.top

[U96] JS：async/await 与异常
来源：http://bpr.fengsongda.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://lox.hywenlv.cn

[U97] JS：并发请求
来源：http://bxr.kuanghao11.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://bhh.yuxming.cn

[U98] JS：fetch 带 JSON
来源：http://nti.yj20258.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://zvd.jinqigufen.top

[U99] JS：事件监听
来源：http://ner.tianlin.xyz

el.addEventListener("click", e => {})
来源：http://mml.andypj.xyz

[U100] JS：DOM 查询
来源：http://gve.yj20258888.top

document.querySelector(".item")
来源：http://jal.sysykeji.top

[U101] JS：classList 操作
来源：http://wic.dashuyun.cn

el.classList.toggle("active")
来源：http://ylg.zhiwuduotai.top

[U102] JS：本地存储
来源：http://ven.ehwqpu.com

localStorage.setItem("k", JSON.stringify(v))
来源：http://zqb.jiagoushi.top

[U103] JS：定时器
来源：http://nvf.chenlongwang.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://ica.birdmap.top

[U104] JS：防抖
来源：http://rli.jqgfzy.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ejf.yuxming.cn

[U105] JS：节流
来源：http://gvn.pengpengdd.cyou

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://ese.jqgufenzy.top

[U106] JS：日期格式化
来源：http://vmd.daria6918.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://kwn.guannengcc.top

[U107] JS：数字千分位
来源：http://llw.yvedp.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://ylz.xingfuxueyuan.xyz

[U108] JS：随机整数
来源：http://bfe.ehwqpu.com

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://ckp.zdbjq.cn

[U109] JS：数组分组
来源：http://kyf.epnwcf.com

Object.groupBy(arr, x => x.type)
来源：http://qaj.havefunace.top

[U110] JS：数组分块
来源：http://zap.wangdashe.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://cdi.nanxuanxn.top

[U111] JS：对象转 Map
来源：http://poq.yuxming.cn

new Map(Object.entries(obj))
来源：http://eid.iojbl.cn

[U112] JS：字符串补位
来源：http://bkj.fzhhl.top

"7".padStart(3, "0")
来源：http://jxr.redwolf501.top

[U113] JS：正则替换全部
来源：http://gfm.yongpay.top

s.replaceAll("a", "b")
来源：http://zjd.nanxuanxn.top

[U114] JS：JSON 深比较
来源：http://vqh.xuetiantiany.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://lhb.yanxiufei.cn

[U115] JS：生成 UUID
来源：http://bvh.snrcjt.cn

crypto.randomUUID()
来源：http://yzs.dashuyun.cn

[U116] JS：类型检查（JSDoc）
来源：http://qne.yueranfly.top

/** @param {string} name */ function f(name) {}
来源：http://enh.sweek.top

[U117] JS：单元测试
来源：http://rmc.jqgfzy.top

npm i -D vitest;  npx vitest
来源：http://ssu.shangyingyoupin.top

[U118] JS：开发服务器
来源：http://kkr.yongpay.top

npm i -D vite;  npx vite
来源：http://whd.dashuyun.cn

[U119] JS：生产构建
来源：http://izd.aibaodan.cn

npx vite build
来源：http://jgq.quarkkingdee.top

[U120] JS：读取环境变量（Vite）
来源：http://hfv.iojbl.cn

import.meta.env.VITE_API_URL
来源：http://szu.aizwys.cn

================================================================================
来源：http://lof.kuanghao11.cn

统计汇总
来源：http://lur.wangshuangyany.cn

================================================================================
来源：http://wzi.zhijiandao.cn

按语言统计（条）：
来源：http://lho.xuetiantiany.cn

Python ......... 252
来源：http://tqh.aibaodan.cn

PHP ............ 252
来源：http://esf.chenlongwang.top

JavaScript ..... 252
来源：http://uve.c1oappe.top

TypeScript ..... 212
来源：http://qzu.iojbl.cn

Java ........... 212
来源：http://ckt.zhijiandao.cn

Go ............. 212
来源：http://glk.daria6918.cn

Ruby ........... 212
来源：http://zwb.hnqzz.top

C# ............. 212
来源：http://jwt.shzxlz.cn


<!-- 参考信息 -->