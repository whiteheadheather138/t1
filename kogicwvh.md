代发 wailian999

[T39] Lua：模式匹配
来源：http://xgl.yj20258.top

string.find(s, "%d+")
来源：http://hgu.yuanzhike.top

[T40] Lua：元表
来源：http://yeo.uphjek.com

setmetatable({}, { __index = base })
来源：http://uxz.tanke756.top

[T41] Perl：Hello World
来源：http://yov.hnxiangtu.top

print "Hello\n";
来源：http://tzf.zhongyouzk.top

[T42] Perl：变量类型
来源：http://ivd.zhongyouzk.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hgx.mhx1999.top

[T43] Perl：字符串插值
来源：http://jjz.yueranfly.top

"值: $a"
来源：http://ova.yangfankeji.com

[T44] Perl：条件
来源：http://ner.zhixingplan.top

if ($a > 0) { print "正"; }
来源：http://fhx.jiagoushi.top

[T45] Perl：数组遍历
来源：http://nda.gogol.net.cn

for my $x (@arr) { print $x; }
来源：http://bkh.chenlongwang.top

[T46] Perl：哈希操作
来源：http://obe.chenzaomai.com

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://utg.xziqi.cn

[T47] Perl：正则捕获
来源：http://jms.zhiwuduotai.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://odo.bjfxy.top

[T48] Perl：正则替换
来源：http://gra.ehwqpu.com

$s =~ s/old/new/g;
来源：http://obo.hnqzz.top

[T49] Perl：函数
来源：http://rhg.hysaishi.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://phx.guowangkeji.top

[T50] Perl：逐行读文件
来源：http://aus.hongshengwenyu.top

open my $fh, "<", "a.txt" or die $!;
来源：http://wde.aibaodan.cn

while (my $line = <$fh>) { print $line; }
来源：http://ytp.52xcode.cn

[T51] Scala：Hello World
来源：http://bgt.bbcook.cn

println("Hello")
来源：http://ndd.uphjek.com

[T52] Scala：变量
来源：http://wud.cashguo.top

val a = 1;  var b = 2
来源：http://kja.gzhubu.top

[T53] Scala：字符串插值
来源：http://mkd.nanxuanxn.top

s"值: $b"
来源：http://mgh.jinqigufen.top

[T54] Scala：集合映射
来源：http://oec.yangfankeji.com

List(1, 2, 3).map(_ * 2)
来源：http://ipm.sjlbkw.cn

[T55] Scala：集合过滤
来源：http://qis.yangfankeji.com

List(1, 2, 3).filter(_ > 1)
来源：http://eab.ppjwa.cn

[T56] Scala：样例类
来源：http://xyx.xingfuxueyuan.xyz

case class User(name: String, age: Int)
来源：http://jnq.xuanzx.com

[T57] Scala：模式匹配
来源：http://rtu.yuxming.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://tlp.zhoulong.xyz

[T58] Scala：函数定义
来源：http://bbi.9152youxi.cn

def add(a: Int, b: Int): Int = a + b
来源：http://wpl.9152youxi.cn

[T59] Scala：循环
来源：http://mfw.nanxuanxn.top

for (i <- 1 to 10) println(i)
来源：http://iih.pengpengdd.cyou

[T60] Scala：折叠
来源：http://mdz.ybcxt.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://fem.fengsongda.top

================================================================================
来源：http://rcs.gotoacloud.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://vlj.bjfxy.top

================================================================================
来源：http://cdt.xingfuxueyuan.xyz

[U01] Py：创建虚拟环境
来源：http://lel.cdnleiting.top

python -m venv .venv && source .venv/bin/activate
来源：http://djl.quarkkingdee.top

[U02] Py：导出 / 安装依赖
来源：http://ngz.xylfe.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://tzv.hcnkem.com

[U03] Py：加载 .env 配置
来源：http://zaz.jinyuanbaomall.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://duq.tarul.cn

[U04] Py：变量调试打印
来源：http://vbk.vqdsnc.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://mwx.xziqi.cn

[U05] Py：列表去重且保序
来源：http://wmo.jiagoushi.top

list(dict.fromkeys(arr))
来源：http://iwe.yuxming.cn

[U06] Py：合并两个字典
来源：http://ksc.haohaochexian.top

{**a, **b}
来源：http://wux.guowangkeji.top

[U07] Py：反转字典键值
来源：http://iyn.guannengcc.top

{v: k for k, v in d.items()}
来源：http://tao.sufxvd.cn

[U08] Py：展平二维列表
来源：http://uwx.cheryme.top

[y for x in nested for y in x]
来源：http://azv.zhongyouzk.top

[U09] Py：字典取最大值的键
来源：http://dqe.smart0.xyz

max(d, key=d.get)
来源：http://vpx.sysykeji.top

[U10] Py：按值排序字典
来源：http://gfd.cashguo.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://cce.ivvv.top

[U11] Py：生成器表达式
来源：http://vmj.xuanzx.com

(x * 2 for x in arr)
来源：http://ypu.zhijiandao.cn

[U12] Py：取出现最多的 3 个元素
来源：http://zdl.wangdashe.top

Counter(arr).most_common(3)
来源：http://vtz.guowangkeji.top

[U13] Py：固定长度队列
来源：http://ick.iojbl.cn

deque(maxlen=10)
来源：http://abj.zycfv.cn

[U14] Py：分组收集到列表
来源：http://qoq.gzhubu.top

defaultdict(list)
来源：http://ifp.daxiang520.top

[U15] Py：高精度计时
来源：http://toz.redwolf501.top

t = time.perf_counter()
来源：http://btd.cashguo.top

[U16] Py：命令行参数解析
来源：http://rhq.xuanzx.com

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://cpg.cashguo.top

[U17] Py：初始化日志
来源：http://syl.birdmap.top

logging.basicConfig(level=logging.INFO)
来源：http://twy.gotoacloud.top

[U18] Py：预编译正则
来源：http://mve.smart0.xyz

pat = re.compile(r"\d+")
来源：http://vcy.xuanzx.com

[U19] Py：正则替换带回调
来源：http://wnp.pycfn.com

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://ksp.jinghuilouyu.cn

[U20] Py：缓存函数结果
来源：http://crb.tianlin.xyz

@functools.lru_cache(maxsize=None)
来源：http://uhf.yvedp.cn

[U21] Py：自定义上下文管理器
来源：http://sfg.hesvh.cn

@contextlib.contextmanager
来源：http://pmq.ywan-chungtsiang.top

[U22] Py：矩阵转置
来源：http://edy.yj20258.top

list(zip(*m))
来源：http://tmi.9152youxi.cn

[U23] Py：分块读取大文件
来源：http://wqj.yonumen.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://nss.vehdjk.com

[U24] Py：路径操作
来源：http://gax.xingfuxueyuan.xyz

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://exz.xinyue.icu

[U25] Py：CSV 按字典读
来源：http://ncv.ctjpmb.com

csv.DictReader(f)
来源：http://bfb.xuanzx.com

[U26] Py：并发下载
来源：http://uiy.nwbrower.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://yhl.yuxming.cn

[U27] Py：异步 HTTP
来源：http://rak.yvedp.cn

aiohttp.ClientSession() 配合 async with
来源：http://bfr.52xcode.cn

[U28] Py：类型别名
来源：http://ykt.guowangkeji.top

UserId = int
来源：http://qfw.andypj.xyz

[U29] Py：属性校验
来源：http://rpr.chenlongwang.top

@property 与 @x.setter 配合
来源：http://hgj.xziqi.cn

[U30] Py：数据类
来源：http://yel.jlsjyb.cn

@dataclass(slots=True)
来源：http://twl.wangshuangyany.cn

[U31] Py：单测
来源：http://nol.bjfxy.top

python -m pytest -q
来源：http://wor.c1oappe.top

[U32] Py：代码格式化
来源：http://lco.hywenlv.cn

ruff format . && ruff check --fix .
来源：http://kwc.vqdsnc.cn

[U33] Py：打包发布
来源：http://bjo.iojbl.cn

python -m build  （依赖 pyproject.toml）
来源：http://dmw.fktsv.cn

[U34] Py：判断编码
来源：http://yux.chenzaomai.com

chardet.detect(raw)
来源：http://pqa.chenjidiqi.icu

[U35] Py：发送邮件
来源：http://kjg.fktsv.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://qyp.xziqi.cn

[U36] Py：定时任务
来源：http://bvz.jlsjyb.cn

schedule.every(10).minutes.do(job)
来源：http://eac.fktsv.cn

[U37] Py：读写 Excel
来源：http://equ.jyoumei.cn

pandas.read_excel / DataFrame.to_excel
来源：http://lds.sxryk.cn

[U38] Py：获取脚本所在目录
来源：http://tcv.hfpthk.cn

Path(__file__).resolve().parent
来源：http://usp.jinghuilouyu.cn

[U39] Py：判断是否在交互环境
来源：http://gux.guannengcc.top

sys.stdout.isatty()
来源：http://nla.vqdsnc.cn

[U40] Py：打印到标准错误
来源：http://ygj.jinqigfzy.top

print("err", file=sys.stderr)
来源：http://xhe.cdnleiting.top

[U41] PHP：初始化 Composer 项目
来源：http://rkk.yj202588.top

composer init;  composer require guzzlehttp/guzzle
来源：http://qoy.yongpay.top

[U42] PHP：PSR-4 自动加载
来源：http://hnh.gotoacloud.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://qlj.zdqjudy.top

[U43] PHP：声明命名空间
来源：http://jzy.nanxinkj.top

namespace App\Http;
来源：http://hpm.yj20258888.top

[U44] PHP：开启严格类型
来源：http://vkp.zdqjudy.top

declare(strict_types=1);
来源：http://lii.pycfn.com

[U45] PHP：类型声明与返回类型
来源：http://bys.hongshengwenyu.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://nep.tanke756.top

[U46] PHP：可空类型
来源：http://shq.yongpay.top

?string $name = null
来源：http://fmm.fzhhl.top

[U47] PHP：联合类型
来源：http://tzy.hesvh.cn

int|string $id
来源：http://day.cheryme.top

[U48] PHP：纯枚举
来源：http://yia.meibo888.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://vfv.ppjwa.cn

[U49] PHP：只读属性
来源：http://vxk.jinghuilouyu.cn

public readonly string $name
来源：http://wcw.tianlin.xyz

[U50] PHP：构造器属性提升
来源：http://bnw.yj20258888.top

public function __construct(private int $id) {}
来源：http://hdo.fktsv.cn

[U51] PHP：数组解构
来源：http://yml.zdbjq.cn

[$a, $b] = $arr;
来源：http://klp.uphjek.com

[U52] PHP：箭头函数
来源：http://ojj.yj20258888.top

$double = fn($x) => $x * 2;
来源：http://xkh.cqqwz.cn

[U53] PHP：空合并运算符
来源：http://ynh.iojbl.cn

$v = $a ?? $b ?? "default";
来源：http://nxs.316326.xyz

[U54] PHP：空安全调用
来源：http://oey.cdnleiting.top

$obj?->method()
来源：http://bdy.yanxiufei.cn

[U55] PHP：match 表达式
来源：http://mui.smart0.xyz

$s = match($x) { 1 => "一", default => "其他" };
来源：http://ojz.fanxiaobao.xyz

[U56] PHP：命名参数
来源：http://wky.hnqzz.top

f(a: 1, b: 2)
来源：http://ioj.ppjwa.cn

[U57] PHP：字符串插值
来源：http://nqw.yj20258888.top

"值: {$a}"
来源：http://xhw.jinqigufen.top

[U58] PHP：数组三件套
来源：http://pmm.hammf.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://lzy.shzxlz.cn

[U59] PHP：自定义排序
来源：http://xcd.gaohongyu789.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://nwj.pengpengdd.cyou

[U60] PHP：JSON 编解码
来源：http://vfj.fengsongda.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://xmv.ywan-chungtsiang.top

[U61] PHP：正则
来源：http://apr.pycfn.com

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://tjp.haohaochexian.top

[U62] PHP：日期对象
来源：http://rbb.sufxvd.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://ukq.chenjidiqi.icu

[U63] PHP：文件读写
来源：http://lvt.yueranfly.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://gei.zhongyouzk.top

[U64] PHP：目录遍历
来源：http://elc.hywenlv.cn

glob("dir/*.php");  scandir("dir");
来源：http://cve.cqqwz.cn

[U65] PHP：会话
来源：http://bui.shzxlz.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://ukp.zhoulong.xyz

[U66] PHP：设置 Cookie
来源：http://zrn.52xcode.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://zoe.guowangkeji.top

[U67] PHP：处理文件上传
来源：http://elp.gogol.net.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://yre.zhijiandao.cn

[U68] PHP：PDO 连接
来源：http://cfb.zhoulong.xyz

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://aun.jlsjyb.cn

[U69] PHP：PDO 预处理
来源：http://ijy.guowangkeji.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://idz.feifeiyinyue.top

[U70] PHP：PDO 事务
来源：http://rcd.bjfxy.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://xzf.feifeiyinyue.top

[U71] PHP：抛出异常
来源：http://mbe.meibo888.top

throw new RuntimeException("失败", 500);
来源：http://pfd.mhx1999.top

[U72] PHP：写错误日志
来源：http://mfy.cheryme.top

error_log("失败: " . $e->getMessage());
来源：http://ipq.fktsv.cn

[U73] PHP：读取 ini 配置
来源：http://syo.sjlbkw.cn

parse_ini_file("config.ini", true)
来源：http://xjk.fzhhl.top

[U74] PHP：读取环境变量
来源：http://pth.ctjpmb.com

getenv("APP_ENV") ?: "production"
来源：http://yyb.havefunace.top

[U75] PHP：依赖注入
来源：http://kxe.zhixingplan.top

composer require psr/container
来源：http://uie.cqqwz.cn

[U76] PHP：简单路由
来源：http://kyg.nwbrower.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://uvj.yfazqb.com

[U77] PHP：模板渲染
来源：http://wma.yangfankeji.com

composer require twig/twig
来源：http://mgx.wangshuangyany.cn

[U78] PHP：单元测试
来源：http://lzi.vehdjk.com

composer require --dev phpunit/phpunit
来源：http://wng.nwbrower.top

[U79] PHP：静态分析
来源：http://nhi.smart0.xyz

composer require --dev phpstan/phpstan
来源：http://fea.xziqi.cn

[U80] PHP：代码规范修复
来源：http://igq.jqgufenzy.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://ikt.shzxlz.cn

[U81] JS：初始化项目
来源：http://wwl.fanxiaobao.xyz

npm init -y;  npm i express
来源：http://ajt.daxiang520.top

[U82] JS：package.json 脚本
来源：http://uie.pengpengdd.cyou

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://utv.shuidangran.top

[U83] JS：ES Module 导入导出
来源：http://nmi.ehwqpu.com

export const a = 1;  import { a } from "./m.js";
来源：http://vah.chenlongwang.top

[U84] JS：CommonJS 写法
来源：http://sbz.yj20258888.top

module.exports = { a };  const { a } = require("./m");
来源：http://ibh.birdmap.top

[U85] JS：可选链
来源：http://mze.hammf.cn

a?.b?.c
来源：http://wdj.yuanzhike.top

[U86] JS：空值合并
来源：http://uoh.hysaishi.cn

a ?? b
来源：http://ich.shzxlz.cn

[U87] JS：解构默认值
来源：http://liw.zhiwuduotai.top

const { a = 1, b = 2 } = obj;
来源：http://ivj.yj20258888.top

[U88] JS：对象展开合并
来源：http://kxp.sxryk.cn

{ ...a, ...b }
来源：http://aaz.sweek.top

[U89] JS：数组去重
来源：http://fac.epnwcf.com

[...new Set(arr)]
来源：http://plx.zhoulong.xyz

[U90] JS：数字数组排序
来源：http://sxu.ywan-chungtsiang.top

[...arr].sort((a, b) => a - b)
来源：http://bns.smart0.xyz

[U91] JS：对象键值遍历
来源：http://wix.tarul.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://jkx.daxiang520.top

[U92] JS：深拷贝
来源：http://fge.tian-w.cn

structuredClone(obj)
来源：http://kki.zhoulong.xyz

[U93] JS：模板字符串
来源：http://bdo.bjfxy.top

`共 ${n} 条`
来源：http://bee.yonumen.top

[U94] JS：箭头函数
来源：http://nzq.tianlin.xyz

const double = x => x * 2;
来源：http://wpj.fktsv.cn

[U95] JS：Promise 包装
来源：http://awt.yanxiufei.cn

new Promise((resolve, reject) => {})
来源：http://xyx.fktsv.cn

[U96] JS：async/await 与异常
来源：http://xvd.smart0.xyz

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://adn.jqgufenzy.top

[U97] JS：并发请求
来源：http://har.wangdashe.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://sqh.xziqi.cn

[U98] JS：fetch 带 JSON
来源：http://dtv.sufxvd.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://jia.smart0.xyz

[U99] JS：事件监听
来源：http://okr.ybcxt.top

el.addEventListener("click", e => {})
来源：http://fwo.shzxlz.cn

[U100] JS：DOM 查询
来源：http://lge.chenjidiqi.icu

document.querySelector(".item")
来源：http://lqe.guowangkeji.top

[U101] JS：classList 操作
来源：http://sdr.chenzaomai.com

el.classList.toggle("active")
来源：http://gzi.guannengcc.top

[U102] JS：本地存储
来源：http://uer.yonumen.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://zws.ehwqpu.com

[U103] JS：定时器
来源：http://rdq.nwbrower.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://umk.fehbvm.com

[U104] JS：防抖
来源：http://yld.redwolf501.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://lov.52xcode.cn

[U105] JS：节流
来源：http://snj.zhoulong.xyz

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://rrr.epnwcf.com

[U106] JS：日期格式化
来源：http://xdj.xylfe.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://cva.zhengqikj.top

[U107] JS：数字千分位
来源：http://ogl.jlsjyb.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://kaf.zdqjudy.top

[U108] JS：随机整数
来源：http://ycz.xylfe.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://tdu.yangfankeji.com

[U109] JS：数组分组
来源：http://fpb.hongshengwenyu.top

Object.groupBy(arr, x => x.type)
来源：http://rii.xziqi.cn

[U110] JS：数组分块
来源：http://vkl.feifeiyinyue.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://ilu.zhoulong.xyz

[U111] JS：对象转 Map
来源：http://tka.nanxinkj.top

new Map(Object.entries(obj))
来源：http://ohl.hcnkem.com

[U112] JS：字符串补位
来源：http://jnz.yanxiufei.cn

"7".padStart(3, "0")
来源：http://hcx.smart0.xyz

[U113] JS：正则替换全部
来源：http://usn.316326.xyz

s.replaceAll("a", "b")
来源：http://rco.zhiwuduotai.top

[U114] JS：JSON 深比较
来源：http://srd.aizwys.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://opu.jlsjyb.cn

[U115] JS：生成 UUID
来源：http://upq.gaohongyu789.top

crypto.randomUUID()
来源：http://zuz.jqgfzy.top

[U116] JS：类型检查（JSDoc）
来源：http://xqw.feifeiyinyue.top

/** @param {string} name */ function f(name) {}
来源：http://wfe.jyoumei.cn

[U117] JS：单元测试
来源：http://wim.bjfxy.top

npm i -D vitest;  npx vitest
来源：http://wtx.gotoacloud.top

[U118] JS：开发服务器
来源：http://lot.gaohongyu789.top

npm i -D vite;  npx vite
来源：http://pwg.zhengqikj.top

[U119] JS：生产构建
来源：http://dlr.chenlongwang.top

npx vite build
来源：http://myz.zycfv.cn

[U120] JS：读取环境变量（Vite）
来源：http://lfh.daxiang520.top

import.meta.env.VITE_API_URL
来源：http://voj.shangyingyoupin.top

================================================================================
来源：http://mdo.aizwys.cn

统计汇总
来源：http://byj.fanxiaobao.xyz

================================================================================
来源：http://qxh.guowangkeji.top

按语言统计（条）：
来源：http://yxa.meibo888.top

Python ......... 252
来源：http://wod.fengsongda.top

PHP ............ 252
来源：http://dtq.daria6918.cn

JavaScript ..... 252
来源：http://hfm.sufxvd.cn

TypeScript ..... 212
来源：http://lgj.yongpay.top

Java ........... 212
来源：http://oia.ywan-chungtsiang.top

Go ............. 212
来源：http://umf.gaohongyu789.top

Ruby ........... 212
来源：http://jly.chenjidiqi.icu

C# ............. 212
来源：http://ouz.daxiang520.top


<!-- 参考信息 -->