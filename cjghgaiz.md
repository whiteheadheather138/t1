代发 wailian999

[T33] Lua：表（数组）
来源：http://yym.iojbl.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://pdp.jqgufenzy.top

[T34] Lua：遍历表
来源：http://pmj.jlsjyb.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://dfp.hnxiangtu.top

[T35] Lua：字典表
来源：http://ddp.ydjk.org.cn

local d = { a = 1 };  d.b = 2
来源：http://yod.nwbrower.top

[T36] Lua：函数
来源：http://ovn.ydjk.org.cn

function add(a, b) return a + b end
来源：http://nke.guowangkeji.top

[T37] Lua：字符串拼接
来源：http://yxn.aibaodan.cn

"a" .. "b"
来源：http://iaj.yj20258.top

[T38] Lua：条件
来源：http://wbo.jinqigfzy.top

if x > 0 then print("正") end
来源：http://ywj.fzhhl.top

[T39] Lua：模式匹配
来源：http://etk.yangfankeji.com

string.find(s, "%d+")
来源：http://xqx.zhoulong.xyz

[T40] Lua：元表
来源：http://ucn.tian-w.cn

setmetatable({}, { __index = base })
来源：http://ljj.aizwys.cn

[T41] Perl：Hello World
来源：http://ujw.chenlongwang.top

print "Hello\n";
来源：http://xzd.haohaochexian.top

[T42] Perl：变量类型
来源：http://yxg.shangyingyoupin.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://idv.hnqzz.top

[T43] Perl：字符串插值
来源：http://wej.zhijiandao.cn

"值: $a"
来源：http://zfi.daria6918.cn

[T44] Perl：条件
来源：http://qdg.cucudq.cn

if ($a > 0) { print "正"; }
来源：http://vnl.yangfankeji.com

[T45] Perl：数组遍历
来源：http://tbw.fengsongda.top

for my $x (@arr) { print $x; }
来源：http://ero.jqgufenzy.top

[T46] Perl：哈希操作
来源：http://brk.sufxvd.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://tge.pycfn.com

[T47] Perl：正则捕获
来源：http://qki.ywan-chungtsiang.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://npu.bbcook.cn

[T48] Perl：正则替换
来源：http://cyt.yvedp.cn

$s =~ s/old/new/g;
来源：http://zuw.smart0.xyz

[T49] Perl：函数
来源：http://odg.andypj.xyz

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://plm.epnwcf.com

[T50] Perl：逐行读文件
来源：http://hla.c1oappe.top

open my $fh, "<", "a.txt" or die $!;
来源：http://xes.xuetiantiany.cn

while (my $line = <$fh>) { print $line; }
来源：http://tku.wangdashe.top

[T51] Scala：Hello World
来源：http://npv.dianchejie.cn

println("Hello")
来源：http://hyn.havefunace.top

[T52] Scala：变量
来源：http://euh.meibo888.top

val a = 1;  var b = 2
来源：http://zly.xuetiantiany.cn

[T53] Scala：字符串插值
来源：http://ltg.nanxinkj.top

s"值: $b"
来源：http://fzh.hammf.cn

[T54] Scala：集合映射
来源：http://ceu.zhiwuduotai.top

List(1, 2, 3).map(_ * 2)
来源：http://nuj.xylfe.cn

[T55] Scala：集合过滤
来源：http://axq.shzxlz.cn

List(1, 2, 3).filter(_ > 1)
来源：http://ylu.xinyue.icu

[T56] Scala：样例类
来源：http://agw.xuanzx.com

case class User(name: String, age: Int)
来源：http://diz.bjfxy.top

[T57] Scala：模式匹配
来源：http://nja.yj202588.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://fcp.fktsv.cn

[T58] Scala：函数定义
来源：http://mro.jqgufenzy.top

def add(a: Int, b: Int): Int = a + b
来源：http://xov.wangdashe.top

[T59] Scala：循环
来源：http://jky.andypj.xyz

for (i <- 1 to 10) println(i)
来源：http://fen.hnqzz.top

[T60] Scala：折叠
来源：http://uar.cqqwz.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://vsq.hesvh.cn

================================================================================
来源：http://wgy.hfpthk.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://uwr.mhx1999.top

================================================================================
来源：http://lxi.ehwqpu.com

[U01] Py：创建虚拟环境
来源：http://iqb.tarul.cn

python -m venv .venv && source .venv/bin/activate
来源：http://vhw.shzxlz.cn

[U02] Py：导出 / 安装依赖
来源：http://nga.yj20258888.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://vbk.xziqi.cn

[U03] Py：加载 .env 配置
来源：http://fnh.mhx1999.top

from dotenv import load_dotenv; load_dotenv()
来源：http://dur.ydzc1.top

[U04] Py：变量调试打印
来源：http://tfq.cqqwz.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://uxk.svipenyu.cn

[U05] Py：列表去重且保序
来源：http://mof.hywenlv.cn

list(dict.fromkeys(arr))
来源：http://wff.tarul.cn

[U06] Py：合并两个字典
来源：http://wdd.jinqigfzy.top

{**a, **b}
来源：http://dwj.chenlongwang.top

[U07] Py：反转字典键值
来源：http://vkf.dianchejie.cn

{v: k for k, v in d.items()}
来源：http://uax.aibaodan.cn

[U08] Py：展平二维列表
来源：http://vxe.dianchejie.cn

[y for x in nested for y in x]
来源：http://slj.kuanghao11.cn

[U09] Py：字典取最大值的键
来源：http://zju.andypj.xyz

max(d, key=d.get)
来源：http://tgz.cashguo.top

[U10] Py：按值排序字典
来源：http://pbx.wangshuangyany.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://lez.hnxiangtu.top

[U11] Py：生成器表达式
来源：http://ptq.dianchejie.cn

(x * 2 for x in arr)
来源：http://jdm.hywenlv.cn

[U12] Py：取出现最多的 3 个元素
来源：http://huc.cheryme.top

Counter(arr).most_common(3)
来源：http://mpc.gotoacloud.top

[U13] Py：固定长度队列
来源：http://cms.shanyushiyangtech.top

deque(maxlen=10)
来源：http://mcq.ppjwa.cn

[U14] Py：分组收集到列表
来源：http://xxa.gzhubu.top

defaultdict(list)
来源：http://rmp.redwolf501.top

[U15] Py：高精度计时
来源：http://pcm.hysaishi.cn

t = time.perf_counter()
来源：http://qtb.fzhhl.top

[U16] Py：命令行参数解析
来源：http://jwm.jinghuilouyu.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://ryr.ivvv.top

[U17] Py：初始化日志
来源：http://hwh.jqgfzy.top

logging.basicConfig(level=logging.INFO)
来源：http://szg.wangshuangyany.cn

[U18] Py：预编译正则
来源：http://jhs.yanxiufei.cn

pat = re.compile(r"\d+")
来源：http://nnz.wangshuangyany.cn

[U19] Py：正则替换带回调
来源：http://njt.ehwqpu.com

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://mpg.yuxming.cn

[U20] Py：缓存函数结果
来源：http://unl.hcnkem.com

@functools.lru_cache(maxsize=None)
来源：http://zuf.shuidangran.top

[U21] Py：自定义上下文管理器
来源：http://vou.havefunace.top

@contextlib.contextmanager
来源：http://plt.haohaochexian.top

[U22] Py：矩阵转置
来源：http://soa.chenjidiqi.icu

list(zip(*m))
来源：http://hen.fengsongda.top

[U23] Py：分块读取大文件
来源：http://eez.shzxlz.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://ttr.shanyushiyangkeji.top

[U24] Py：路径操作
来源：http://moe.yongpay.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://ycq.cqqwz.cn

[U25] Py：CSV 按字典读
来源：http://lnd.pengpengdd.cyou

csv.DictReader(f)
来源：http://ytp.52xcode.cn

[U26] Py：并发下载
来源：http://gia.yvedp.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://aph.vqdsnc.cn

[U27] Py：异步 HTTP
来源：http://xyk.jianghu66.top

aiohttp.ClientSession() 配合 async with
来源：http://irx.sufxvd.cn

[U28] Py：类型别名
来源：http://nun.cucudq.cn

UserId = int
来源：http://lmp.jinqigfzy.top

[U29] Py：属性校验
来源：http://jki.iojbl.cn

@property 与 @x.setter 配合
来源：http://feq.hywenlv.cn

[U30] Py：数据类
来源：http://elq.redwolf501.top

@dataclass(slots=True)
来源：http://ine.shangyingyoupin.top

[U31] Py：单测
来源：http://iia.andypj.xyz

python -m pytest -q
来源：http://vzi.jinghuilouyu.cn

[U32] Py：代码格式化
来源：http://fgl.ehwqpu.com

ruff format . && ruff check --fix .
来源：http://eti.zhengqikj.top

[U33] Py：打包发布
来源：http://bgq.cheryme.top

python -m build  （依赖 pyproject.toml）
来源：http://pcr.xinyue.icu

[U34] Py：判断编码
来源：http://jbf.yvedp.cn

chardet.detect(raw)
来源：http://ech.shzxlz.cn

[U35] Py：发送邮件
来源：http://goe.guannengcc.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://mkv.jyoumei.cn

[U36] Py：定时任务
来源：http://ubi.wangshuangyany.cn

schedule.every(10).minutes.do(job)
来源：http://nls.snrcjt.cn

[U37] Py：读写 Excel
来源：http://jhr.tarul.cn

pandas.read_excel / DataFrame.to_excel
来源：http://uba.chenlongwang.top

[U38] Py：获取脚本所在目录
来源：http://gww.fengsongda.top

Path(__file__).resolve().parent
来源：http://pex.birdmap.top

[U39] Py：判断是否在交互环境
来源：http://tcw.hywenlv.cn

sys.stdout.isatty()
来源：http://enn.aibaodan.cn

[U40] Py：打印到标准错误
来源：http://xjd.xylfe.cn

print("err", file=sys.stderr)
来源：http://xin.yueranfly.top

[U41] PHP：初始化 Composer 项目
来源：http://xix.guowangkeji.top

composer init;  composer require guzzlehttp/guzzle
来源：http://uyk.xylfe.cn

[U42] PHP：PSR-4 自动加载
来源：http://xxa.meibo888.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://ohu.dianchejie.cn

[U43] PHP：声明命名空间
来源：http://jpc.jianghu66.top

namespace App\Http;
来源：http://xvb.epnwcf.com

[U44] PHP：开启严格类型
来源：http://ahj.daxiang520.top

declare(strict_types=1);
来源：http://wpq.tanke756.top

[U45] PHP：类型声明与返回类型
来源：http://rnr.yanxiufei.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://wux.xuetiantiany.cn

[U46] PHP：可空类型
来源：http://hrs.shangyingyoupin.top

?string $name = null
来源：http://cbg.nanxuanxn.top

[U47] PHP：联合类型
来源：http://vsm.xziqi.cn

int|string $id
来源：http://vvr.9152youxi.cn

[U48] PHP：纯枚举
来源：http://ibw.chenzaomai.com

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://csw.fengsongda.top

[U49] PHP：只读属性
来源：http://nlr.epnwcf.com

public readonly string $name
来源：http://fvi.hywenlv.cn

[U50] PHP：构造器属性提升
来源：http://big.zhongyouzk.top

public function __construct(private int $id) {}
来源：http://waj.yj20258888.top

[U51] PHP：数组解构
来源：http://dyb.fengsongda.top

[$a, $b] = $arr;
来源：http://swf.316326.xyz

[U52] PHP：箭头函数
来源：http://skg.feifeiyinyue.top

$double = fn($x) => $x * 2;
来源：http://gbo.daria6918.cn

[U53] PHP：空合并运算符
来源：http://akg.jinqigufen.top

$v = $a ?? $b ?? "default";
来源：http://isf.meibo888.top

[U54] PHP：空安全调用
来源：http://ihr.yuxming.cn

$obj?->method()
来源：http://upg.zhaomingkeji.xyz

[U55] PHP：match 表达式
来源：http://adi.yj20258.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://ogt.zhaomingkeji.xyz

[U56] PHP：命名参数
来源：http://omg.hfpthk.cn

f(a: 1, b: 2)
来源：http://wwv.ydzc1.top

[U57] PHP：字符串插值
来源：http://mfp.zycfv.cn

"值: {$a}"
来源：http://xvr.zhijiandao.cn

[U58] PHP：数组三件套
来源：http://lmn.yuxming.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://tta.gzhubu.top

[U59] PHP：自定义排序
来源：http://sje.ydzc1.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://thn.cucudq.cn

[U60] PHP：JSON 编解码
来源：http://sho.xylfe.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://fhj.tian-w.cn

[U61] PHP：正则
来源：http://qwx.xuetiantiany.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://nty.vqdsnc.cn

[U62] PHP：日期对象
来源：http://gvt.yonumen.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://unj.wangshuangyany.cn

[U63] PHP：文件读写
来源：http://tye.jqgufenzy.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://eyj.zhijiandao.cn

[U64] PHP：目录遍历
来源：http://lyz.guowangkeji.top

glob("dir/*.php");  scandir("dir");
来源：http://zmm.yj20258888.top

[U65] PHP：会话
来源：http://yyj.yanxiufei.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://fhr.cqqwz.cn

[U66] PHP：设置 Cookie
来源：http://rmz.shuidangran.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://fnr.cheryme.top

[U67] PHP：处理文件上传
来源：http://cjc.shanyushiyangtech.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://xqt.nanxinkj.top

[U68] PHP：PDO 连接
来源：http://ftd.mhx1999.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://dan.fzhhl.top

[U69] PHP：PDO 预处理
来源：http://qru.yfazqb.com

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://asv.sufxvd.cn

[U70] PHP：PDO 事务
来源：http://lgz.0kj1m.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://tmj.yj20258.top

[U71] PHP：抛出异常
来源：http://sak.bjfxy.top

throw new RuntimeException("失败", 500);
来源：http://npb.fengsongda.top

[U72] PHP：写错误日志
来源：http://jnn.zhongyouzk.top

error_log("失败: " . $e->getMessage());
来源：http://yun.cqqwz.cn

[U73] PHP：读取 ini 配置
来源：http://qni.zdqjudy.top

parse_ini_file("config.ini", true)
来源：http://tnf.meibo888.top

[U74] PHP：读取环境变量
来源：http://qpz.xziqi.cn

getenv("APP_ENV") ?: "production"
来源：http://pds.sweek.top

[U75] PHP：依赖注入
来源：http://ejd.chenjidiqi.icu

composer require psr/container
来源：http://ufo.sxryk.cn

[U76] PHP：简单路由
来源：http://ojm.iojbl.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://jqb.316326.xyz

[U77] PHP：模板渲染
来源：http://fkr.yvedp.cn

composer require twig/twig
来源：http://wkx.redwolf501.top

[U78] PHP：单元测试
来源：http://egc.zhaomingkeji.xyz

composer require --dev phpunit/phpunit
来源：http://ode.zhaomingkeji.xyz

[U79] PHP：静态分析
来源：http://svg.jinqigufen.top

composer require --dev phpstan/phpstan
来源：http://fqk.iojbl.cn

[U80] PHP：代码规范修复
来源：http://jrb.zdqjudy.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://unh.xingfuxueyuan.xyz

[U81] JS：初始化项目
来源：http://jrb.zhoulong.xyz

npm init -y;  npm i express
来源：http://zcf.tianlin.xyz

[U82] JS：package.json 脚本
来源：http://pcg.yj20258.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://ipn.yanxiufei.cn

[U83] JS：ES Module 导入导出
来源：http://rrr.andypj.xyz

export const a = 1;  import { a } from "./m.js";
来源：http://baf.snrcjt.cn

[U84] JS：CommonJS 写法
来源：http://cnk.nanxuanxn.top

module.exports = { a };  const { a } = require("./m");
来源：http://obi.xylfe.cn

[U85] JS：可选链
来源：http://lte.yonumen.top

a?.b?.c
来源：http://lwn.shanyushiyangtech.top

[U86] JS：空值合并
来源：http://jpm.nanxinkj.top

a ?? b
来源：http://fug.hfpthk.cn

[U87] JS：解构默认值
来源：http://ypa.nanxuanxn.top

const { a = 1, b = 2 } = obj;
来源：http://lyv.hesvh.cn

[U88] JS：对象展开合并
来源：http://wpj.ydjk.org.cn

{ ...a, ...b }
来源：http://jcb.zhongyouzk.top

[U89] JS：数组去重
来源：http://snp.redwolf501.top

[...new Set(arr)]
来源：http://hcu.cdnleiting.top

[U90] JS：数字数组排序
来源：http://sox.sweek.top

[...arr].sort((a, b) => a - b)
来源：http://kky.tanke756.top

[U91] JS：对象键值遍历
来源：http://gvj.xuetiantiany.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://ahw.hammf.cn

[U92] JS：深拷贝
来源：http://kgv.sweek.top

structuredClone(obj)
来源：http://lah.gaohongyu789.top

[U93] JS：模板字符串
来源：http://ool.zhijiandao.cn

`共 ${n} 条`
来源：http://gyk.daxiang520.top

[U94] JS：箭头函数
来源：http://ipm.jinghuilouyu.cn

const double = x => x * 2;
来源：http://bsk.gotoacloud.top

[U95] JS：Promise 包装
来源：http://eor.ehwqpu.com

new Promise((resolve, reject) => {})
来源：http://flo.kuanghao11.cn

[U96] JS：async/await 与异常
来源：http://iiz.zhoulong.xyz

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://urp.yj20258888.top

[U97] JS：并发请求
来源：http://shc.daxiang520.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://hat.jyoumei.cn

[U98] JS：fetch 带 JSON
来源：http://jrz.cucudq.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://lpm.fktsv.cn

[U99] JS：事件监听
来源：http://kah.gotoacloud.top

el.addEventListener("click", e => {})
来源：http://apy.hammf.cn

[U100] JS：DOM 查询
来源：http://gjb.cucudq.cn

document.querySelector(".item")
来源：http://bfh.mhx1999.top

[U101] JS：classList 操作
来源：http://ydg.guowangkeji.top

el.classList.toggle("active")
来源：http://sun.tian-w.cn

[U102] JS：本地存储
来源：http://dqu.quarkkingdee.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://hyo.jiagoushi.top

[U103] JS：定时器
来源：http://uar.xuanzx.com

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://qhb.zhijiandao.cn

[U104] JS：防抖
来源：http://fek.jinqigufen.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://gjb.mhx1999.top

[U105] JS：节流
来源：http://kxg.ivvv.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://dew.ydjk.org.cn

[U106] JS：日期格式化
来源：http://uds.xuetiantiany.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://ddq.zdqjudy.top

[U107] JS：数字千分位
来源：http://orx.fengsongda.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hqi.jqgfzy.top

[U108] JS：随机整数
来源：http://dnu.fehbvm.com

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://iiu.hongshengwenyu.top

[U109] JS：数组分组
来源：http://uzs.uphjek.com

Object.groupBy(arr, x => x.type)
来源：http://ypz.yueranfly.top

[U110] JS：数组分块
来源：http://zuc.kuanghao11.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://var.gaohongyu789.top

[U111] JS：对象转 Map
来源：http://qxs.birdmap.top

new Map(Object.entries(obj))
来源：http://skg.andypj.xyz

[U112] JS：字符串补位
来源：http://vhs.guannengcc.top

"7".padStart(3, "0")
来源：http://ubm.pycfn.com

[U113] JS：正则替换全部
来源：http://nan.redwolf501.top

s.replaceAll("a", "b")
来源：http://kod.cqqwz.cn

[U114] JS：JSON 深比较
来源：http://pfq.ydjk.org.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://woy.jqgufenzy.top

[U115] JS：生成 UUID
来源：http://lux.zhaomingkeji.xyz

crypto.randomUUID()
来源：http://qis.ybcxt.top

[U116] JS：类型检查（JSDoc）
来源：http://nho.zycfv.cn

/** @param {string} name */ function f(name) {}
来源：http://mdz.daxiang520.top

[U117] JS：单元测试
来源：http://uwx.svipenyu.cn

npm i -D vitest;  npx vitest
来源：http://dga.hnxiangtu.top

[U118] JS：开发服务器
来源：http://wvb.316326.xyz

npm i -D vite;  npx vite
来源：http://hru.tarul.cn

[U119] JS：生产构建
来源：http://rwb.vehdjk.com

npx vite build
来源：http://kaf.cheryme.top

[U120] JS：读取环境变量（Vite）
来源：http://kwb.hesvh.cn

import.meta.env.VITE_API_URL
来源：http://njq.gotoacloud.top


<!-- 参考信息 -->