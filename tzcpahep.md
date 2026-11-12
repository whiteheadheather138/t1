代发 wailian999

[T39] Lua：模式匹配
来源：http://kal.xziqi.cn

string.find(s, "%d+")
来源：http://zmp.andypj.xyz

[T40] Lua：元表
来源：http://iys.hywenlv.cn

setmetatable({}, { __index = base })
来源：http://dir.cheryme.top

[T41] Perl：Hello World
来源：http://dwp.hongshengwenyu.top

print "Hello\n";
来源：http://wji.yvedp.cn

[T42] Perl：变量类型
来源：http://tsk.chenzaomai.com

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://gkq.quarkkingdee.top

[T43] Perl：字符串插值
来源：http://amu.316326.xyz

"值: $a"
来源：http://nbc.vehdjk.com

[T44] Perl：条件
来源：http://jcp.haohaochexian.top

if ($a > 0) { print "正"; }
来源：http://gfd.feifeiyinyue.top

[T45] Perl：数组遍历
来源：http://hgr.9152youxi.cn

for my $x (@arr) { print $x; }
来源：http://aet.jqgfzy.top

[T46] Perl：哈希操作
来源：http://ljx.feifeiyinyue.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://vam.yueranfly.top

[T47] Perl：正则捕获
来源：http://ywm.fengsongda.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://uud.vehdjk.com

[T48] Perl：正则替换
来源：http://xll.cdnleiting.top

$s =~ s/old/new/g;
来源：http://gzx.9152youxi.cn

[T49] Perl：函数
来源：http://hzv.quarkkingdee.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://dnb.nanxuanxn.top

[T50] Perl：逐行读文件
来源：http://zqt.fanxiaobao.xyz

open my $fh, "<", "a.txt" or die $!;
来源：http://gcu.jianghu66.top

while (my $line = <$fh>) { print $line; }
来源：http://yhm.zycfv.cn

[T51] Scala：Hello World
来源：http://ipk.guannengcc.top

println("Hello")
来源：http://ljm.chenzaomai.com

[T52] Scala：变量
来源：http://ntr.snrcjt.cn

val a = 1;  var b = 2
来源：http://olo.ppjwa.cn

[T53] Scala：字符串插值
来源：http://msk.xuanzx.com

s"值: $b"
来源：http://dbo.yanxiufei.cn

[T54] Scala：集合映射
来源：http://vdw.redwolf501.top

List(1, 2, 3).map(_ * 2)
来源：http://kbm.hammf.cn

[T55] Scala：集合过滤
来源：http://nus.cashguo.top

List(1, 2, 3).filter(_ > 1)
来源：http://scy.c1oappe.top

[T56] Scala：样例类
来源：http://fkx.hcnkem.com

case class User(name: String, age: Int)
来源：http://rat.yangfankeji.com

[T57] Scala：模式匹配
来源：http://zgv.cheryme.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://qzp.hysaishi.cn

[T58] Scala：函数定义
来源：http://zke.xingfuxueyuan.xyz

def add(a: Int, b: Int): Int = a + b
来源：http://wxn.epnwcf.com

[T59] Scala：循环
来源：http://kde.tanke756.top

for (i <- 1 to 10) println(i)
来源：http://don.cashguo.top

[T60] Scala：折叠
来源：http://tyu.redwolf501.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://oix.gzhubu.top

================================================================================
来源：http://psx.ehwqpu.com

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://cxh.zhongyouzk.top

================================================================================
来源：http://yyl.xuanzx.com

[U01] Py：创建虚拟环境
来源：http://jkw.sweek.top

python -m venv .venv && source .venv/bin/activate
来源：http://rjn.epnwcf.com

[U02] Py：导出 / 安装依赖
来源：http://ptx.daria6918.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://yil.zycfv.cn

[U03] Py：加载 .env 配置
来源：http://koo.c1oappe.top

from dotenv import load_dotenv; load_dotenv()
来源：http://vxd.yongpay.top

[U04] Py：变量调试打印
来源：http://xam.nwbrower.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://kkq.xingfuxueyuan.xyz

[U05] Py：列表去重且保序
来源：http://ulk.wangdashe.top

list(dict.fromkeys(arr))
来源：http://rsq.ydjk.org.cn

[U06] Py：合并两个字典
来源：http://loq.kuanghao11.cn

{**a, **b}
来源：http://xno.yuanzhike.top

[U07] Py：反转字典键值
来源：http://uag.gaohongyu789.top

{v: k for k, v in d.items()}
来源：http://smx.zhaomingkeji.xyz

[U08] Py：展平二维列表
来源：http://hbi.zdbjq.cn

[y for x in nested for y in x]
来源：http://jcd.birdmap.top

[U09] Py：字典取最大值的键
来源：http://slo.jqgufenzy.top

max(d, key=d.get)
来源：http://xbx.zhaomingkeji.xyz

[U10] Py：按值排序字典
来源：http://ten.jianghu66.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://lmw.jiagoushi.top

[U11] Py：生成器表达式
来源：http://bvx.yangfankeji.com

(x * 2 for x in arr)
来源：http://oqz.havefunace.top

[U12] Py：取出现最多的 3 个元素
来源：http://tgm.shuidangran.top

Counter(arr).most_common(3)
来源：http://tvb.yj20258.top

[U13] Py：固定长度队列
来源：http://bff.iojbl.cn

deque(maxlen=10)
来源：http://dtq.cucudq.cn

[U14] Py：分组收集到列表
来源：http://ttv.svipenyu.cn

defaultdict(list)
来源：http://upb.yonumen.top

[U15] Py：高精度计时
来源：http://isr.ydzc1.top

t = time.perf_counter()
来源：http://aef.gogol.net.cn

[U16] Py：命令行参数解析
来源：http://spa.ywan-chungtsiang.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://awn.cucudq.cn

[U17] Py：初始化日志
来源：http://lmz.hongshengwenyu.top

logging.basicConfig(level=logging.INFO)
来源：http://hjn.ivvv.top

[U18] Py：预编译正则
来源：http://iks.yuanzhike.top

pat = re.compile(r"\d+")
来源：http://hkn.nanxuanxn.top

[U19] Py：正则替换带回调
来源：http://jpj.tanke756.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://yhs.dashuyun.cn

[U20] Py：缓存函数结果
来源：http://uhp.xuanzx.com

@functools.lru_cache(maxsize=None)
来源：http://wxm.hongshengwenyu.top

[U21] Py：自定义上下文管理器
来源：http://iig.xingfuxueyuan.xyz

@contextlib.contextmanager
来源：http://xnv.zhijiandao.cn

[U22] Py：矩阵转置
来源：http://bgc.tanke756.top

list(zip(*m))
来源：http://azx.dashuyun.cn

[U23] Py：分块读取大文件
来源：http://cdw.zhixingplan.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://fcr.9152youxi.cn

[U24] Py：路径操作
来源：http://ely.aizwys.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://qda.sxryk.cn

[U25] Py：CSV 按字典读
来源：http://xos.ydzc1.top

csv.DictReader(f)
来源：http://scw.zdbjq.cn

[U26] Py：并发下载
来源：http://iju.uphjek.com

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://bqu.yonumen.top

[U27] Py：异步 HTTP
来源：http://szc.cucudq.cn

aiohttp.ClientSession() 配合 async with
来源：http://cpn.ppjwa.cn

[U28] Py：类型别名
来源：http://xzc.havefunace.top

UserId = int
来源：http://juz.gzhubu.top

[U29] Py：属性校验
来源：http://saa.iojbl.cn

@property 与 @x.setter 配合
来源：http://xkd.zhengqikj.top

[U30] Py：数据类
来源：http://mqo.jianghu66.top

@dataclass(slots=True)
来源：http://whd.vehdjk.com

[U31] Py：单测
来源：http://qtr.zdbjq.cn

python -m pytest -q
来源：http://mhm.havefunace.top

[U32] Py：代码格式化
来源：http://pxr.ydjk.org.cn

ruff format . && ruff check --fix .
来源：http://igw.yongpay.top

[U33] Py：打包发布
来源：http://uvd.smart0.xyz

python -m build  （依赖 pyproject.toml）
来源：http://pjp.birdmap.top

[U34] Py：判断编码
来源：http://gez.zdbjq.cn

chardet.detect(raw)
来源：http://wkb.ybcxt.top

[U35] Py：发送邮件
来源：http://vfv.nanxuanxn.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://tkk.tarul.cn

[U36] Py：定时任务
来源：http://vsn.bjfxy.top

schedule.every(10).minutes.do(job)
来源：http://iub.feifeiyinyue.top

[U37] Py：读写 Excel
来源：http://zti.vehdjk.com

pandas.read_excel / DataFrame.to_excel
来源：http://vto.zhaomingkeji.xyz

[U38] Py：获取脚本所在目录
来源：http://hev.jyoumei.cn

Path(__file__).resolve().parent
来源：http://azd.chenzaomai.com

[U39] Py：判断是否在交互环境
来源：http://xnp.pycfn.com

sys.stdout.isatty()
来源：http://xqz.ivvv.top

[U40] Py：打印到标准错误
来源：http://csl.jyoumei.cn

print("err", file=sys.stderr)
来源：http://yla.pycfn.com

[U41] PHP：初始化 Composer 项目
来源：http://rrd.jqgufenzy.top

composer init;  composer require guzzlehttp/guzzle
来源：http://zkk.hywenlv.cn

[U42] PHP：PSR-4 自动加载
来源：http://ers.jinyuanbaomall.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://vlo.fzhhl.top

[U43] PHP：声明命名空间
来源：http://yby.tanke756.top

namespace App\Http;
来源：http://kvi.wangshuangyany.cn

[U44] PHP：开启严格类型
来源：http://zpk.bjfxy.top

declare(strict_types=1);
来源：http://aub.vqdsnc.cn

[U45] PHP：类型声明与返回类型
来源：http://osp.ydjk.org.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://dek.ydzc1.top

[U46] PHP：可空类型
来源：http://fml.xuanzx.com

?string $name = null
来源：http://iql.zhongyouzk.top

[U47] PHP：联合类型
来源：http://lar.zdqjudy.top

int|string $id
来源：http://rhn.ppjwa.cn

[U48] PHP：纯枚举
来源：http://qxg.haohaochexian.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hhe.nanxuanxn.top

[U49] PHP：只读属性
来源：http://who.snrcjt.cn

public readonly string $name
来源：http://rvl.hfpthk.cn

[U50] PHP：构造器属性提升
来源：http://inq.xinyue.icu

public function __construct(private int $id) {}
来源：http://cey.gzhubu.top

[U51] PHP：数组解构
来源：http://jdt.zhengqikj.top

[$a, $b] = $arr;
来源：http://iyo.redwolf501.top

[U52] PHP：箭头函数
来源：http://pgt.sufxvd.cn

$double = fn($x) => $x * 2;
来源：http://bkw.tarul.cn

[U53] PHP：空合并运算符
来源：http://uqq.nwbrower.top

$v = $a ?? $b ?? "default";
来源：http://pmc.iojbl.cn

[U54] PHP：空安全调用
来源：http://wwb.jqgufenzy.top

$obj?->method()
来源：http://sku.ppjwa.cn

[U55] PHP：match 表达式
来源：http://ohm.yonumen.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://bnu.jiagoushi.top

[U56] PHP：命名参数
来源：http://qwf.hongshengwenyu.top

f(a: 1, b: 2)
来源：http://tte.zhoulong.xyz

[U57] PHP：字符串插值
来源：http://imv.yj202588.top

"值: {$a}"
来源：http://jtf.daxiang520.top

[U58] PHP：数组三件套
来源：http://hmu.zycfv.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://wow.yfazqb.com

[U59] PHP：自定义排序
来源：http://phg.daria6918.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://gcf.hfpthk.cn

[U60] PHP：JSON 编解码
来源：http://vcz.vqdsnc.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://rct.yuxming.cn

[U61] PHP：正则
来源：http://oml.jinghuilouyu.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://flr.uphjek.com

[U62] PHP：日期对象
来源：http://ucf.redwolf501.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://ysg.epnwcf.com

[U63] PHP：文件读写
来源：http://xoq.bbcook.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://vxy.yuxming.cn

[U64] PHP：目录遍历
来源：http://uiq.yfazqb.com

glob("dir/*.php");  scandir("dir");
来源：http://tcv.nanxuanxn.top

[U65] PHP：会话
来源：http://pwa.gogol.net.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://esh.shangyingyoupin.top

[U66] PHP：设置 Cookie
来源：http://pmf.sjlbkw.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://hyx.zhaomingkeji.xyz

[U67] PHP：处理文件上传
来源：http://gdp.316326.xyz

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://jre.hesvh.cn

[U68] PHP：PDO 连接
来源：http://yli.xuanzx.com

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://vta.daxiang520.top

[U69] PHP：PDO 预处理
来源：http://etv.feifeiyinyue.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://cvf.xinyue.icu

[U70] PHP：PDO 事务
来源：http://msp.0kj1m.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://csy.haohaochexian.top

[U71] PHP：抛出异常
来源：http://yud.yanxiufei.cn

throw new RuntimeException("失败", 500);
来源：http://pwz.xziqi.cn

[U72] PHP：写错误日志
来源：http://ouv.zhongyouzk.top

error_log("失败: " . $e->getMessage());
来源：http://bzw.dashuyun.cn

[U73] PHP：读取 ini 配置
来源：http://ggr.wangdashe.top

parse_ini_file("config.ini", true)
来源：http://bmb.jqgufenzy.top

[U74] PHP：读取环境变量
来源：http://xie.cashguo.top

getenv("APP_ENV") ?: "production"
来源：http://jqn.dianchejie.cn

[U75] PHP：依赖注入
来源：http://sui.zycfv.cn

composer require psr/container
来源：http://lqe.hesvh.cn

[U76] PHP：简单路由
来源：http://bvq.hongshengwenyu.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://rtk.gaohongyu789.top

[U77] PHP：模板渲染
来源：http://fwk.haohaochexian.top

composer require twig/twig
来源：http://dfd.fanxiaobao.xyz

[U78] PHP：单元测试
来源：http://xej.zhiwuduotai.top

composer require --dev phpunit/phpunit
来源：http://pqu.c1oappe.top

[U79] PHP：静态分析
来源：http://zhk.xuetiantiany.cn

composer require --dev phpstan/phpstan
来源：http://pqq.yuanzhike.top

[U80] PHP：代码规范修复
来源：http://zbg.jqgufenzy.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://dzx.ybcxt.top

[U81] JS：初始化项目
来源：http://frw.vqdsnc.cn

npm init -y;  npm i express
来源：http://ooa.sjlbkw.cn

[U82] JS：package.json 脚本
来源：http://rak.fktsv.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://xuy.nwbrower.top

[U83] JS：ES Module 导入导出
来源：http://mos.tianlin.xyz

export const a = 1;  import { a } from "./m.js";
来源：http://kva.dianchejie.cn

[U84] JS：CommonJS 写法
来源：http://rlj.ppjwa.cn

module.exports = { a };  const { a } = require("./m");
来源：http://bou.gotoacloud.top

[U85] JS：可选链
来源：http://fky.bjfxy.top

a?.b?.c
来源：http://ymb.gotoacloud.top

[U86] JS：空值合并
来源：http://bbs.hnqzz.top

a ?? b
来源：http://eis.wangshuangyany.cn

[U87] JS：解构默认值
来源：http://ldx.nanxinkj.top

const { a = 1, b = 2 } = obj;
来源：http://ver.birdmap.top

[U88] JS：对象展开合并
来源：http://wou.xylfe.cn

{ ...a, ...b }
来源：http://umg.cucudq.cn

[U89] JS：数组去重
来源：http://lcm.mhx1999.top

[...new Set(arr)]
来源：http://czd.yanxiufei.cn

[U90] JS：数字数组排序
来源：http://lif.uphjek.com

[...arr].sort((a, b) => a - b)
来源：http://qmb.fzhhl.top

[U91] JS：对象键值遍历
来源：http://deg.pycfn.com

Object.entries(obj).forEach(([k, v]) => {});
来源：http://rph.fktsv.cn

[U92] JS：深拷贝
来源：http://eal.ctjpmb.com

structuredClone(obj)
来源：http://gpe.zhoulong.xyz

[U93] JS：模板字符串
来源：http://unn.jinghuilouyu.cn

`共 ${n} 条`
来源：http://bwv.jlsjyb.cn

[U94] JS：箭头函数
来源：http://ozq.xuanzx.com

const double = x => x * 2;
来源：http://lzy.svipenyu.cn

[U95] JS：Promise 包装
来源：http://nzo.ybcxt.top

new Promise((resolve, reject) => {})
来源：http://fhr.xylfe.cn

[U96] JS：async/await 与异常
来源：http://nwf.shzxlz.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://arr.aizwys.cn

[U97] JS：并发请求
来源：http://uzo.jianghu66.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://gvs.iojbl.cn

[U98] JS：fetch 带 JSON
来源：http://mjt.jqgfzy.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://iwf.hesvh.cn

[U99] JS：事件监听
来源：http://eyi.guowangkeji.top

el.addEventListener("click", e => {})
来源：http://lkd.ybcxt.top

[U100] JS：DOM 查询
来源：http://vuk.jianghu66.top

document.querySelector(".item")
来源：http://smo.hongshengwenyu.top

[U101] JS：classList 操作
来源：http://rts.c1oappe.top

el.classList.toggle("active")
来源：http://jcw.jqgfzy.top

[U102] JS：本地存储
来源：http://nfw.jyoumei.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://pil.hfpthk.cn

[U103] JS：定时器
来源：http://usf.cdnleiting.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://lxu.jinghuilouyu.cn

[U104] JS：防抖
来源：http://vfj.epnwcf.com

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://zvz.nwbrower.top

[U105] JS：节流
来源：http://ihq.shanyushiyangtech.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://stu.jlsjyb.cn

[U106] JS：日期格式化
来源：http://tzl.ybcxt.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://two.ctjpmb.com

[U107] JS：数字千分位
来源：http://dks.xuetiantiany.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://tbj.fehbvm.com

[U108] JS：随机整数
来源：http://yrh.jyoumei.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://tgq.daxiang520.top

[U109] JS：数组分组
来源：http://coc.zhixingplan.top

Object.groupBy(arr, x => x.type)
来源：http://ubu.quarkkingdee.top

[U110] JS：数组分块
来源：http://zgf.tanke756.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://xqo.guowangkeji.top

[U111] JS：对象转 Map
来源：http://fea.ydzc1.top

new Map(Object.entries(obj))
来源：http://jsu.cucudq.cn

[U112] JS：字符串补位
来源：http://tdk.sjlbkw.cn

"7".padStart(3, "0")
来源：http://kfk.aizwys.cn

[U113] JS：正则替换全部
来源：http://fpd.zdqjudy.top

s.replaceAll("a", "b")
来源：http://yvq.tanke756.top

[U114] JS：JSON 深比较
来源：http://tmv.zhongyouzk.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://utf.chenzaomai.com

[U115] JS：生成 UUID
来源：http://gih.chenlongwang.top

crypto.randomUUID()
来源：http://rdr.vehdjk.com

[U116] JS：类型检查（JSDoc）
来源：http://jna.hesvh.cn

/** @param {string} name */ function f(name) {}
来源：http://myd.yj202588.top

[U117] JS：单元测试
来源：http://opd.gogol.net.cn

npm i -D vitest;  npx vitest
来源：http://bgg.shanyushiyangtech.top

[U118] JS：开发服务器
来源：http://ysv.c1oappe.top

npm i -D vite;  npx vite
来源：http://esg.gaohongyu789.top

[U119] JS：生产构建
来源：http://aez.bjfxy.top

npx vite build
来源：http://gib.jqgufenzy.top

[U120] JS：读取环境变量（Vite）
来源：http://tie.xylfe.cn

import.meta.env.VITE_API_URL
来源：http://jta.yangfankeji.com

================================================================================
来源：http://zjo.ppjwa.cn

统计汇总
来源：http://ces.316326.xyz

================================================================================
来源：http://vta.shanyushiyangkeji.top

按语言统计（条）：
来源：http://dck.smart0.xyz

Python ......... 252
来源：http://won.chenlongwang.top

PHP ............ 252
来源：http://boh.jlsjyb.cn

JavaScript ..... 252
来源：http://hso.tarul.cn

TypeScript ..... 212
来源：http://swz.bjfxy.top

Java ........... 212
来源：http://cke.xziqi.cn

Go ............. 212
来源：http://gkn.ctjpmb.com

Ruby ........... 212
来源：http://slr.snrcjt.cn

C# ............. 212
来源：http://usu.hywenlv.cn


<!-- 参考信息 -->