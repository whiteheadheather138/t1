代发 wailian999

[T39] Lua：模式匹配
来源：http://toh.jqgufenzy.top

string.find(s, "%d+")
来源：http://kwv.yongpay.top

[T40] Lua：元表
来源：http://qap.shzxlz.cn

setmetatable({}, { __index = base })
来源：http://awb.redwolf501.top

[T41] Perl：Hello World
来源：http://trb.cqqwz.cn

print "Hello\n";
来源：http://qte.jyoumei.cn

[T42] Perl：变量类型
来源：http://rqu.shanyushiyangkeji.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://gzi.epnwcf.com

[T43] Perl：字符串插值
来源：http://ioi.sufxvd.cn

"值: $a"
来源：http://phc.aibaodan.cn

[T44] Perl：条件
来源：http://dgu.cqqwz.cn

if ($a > 0) { print "正"; }
来源：http://hjh.9152youxi.cn

[T45] Perl：数组遍历
来源：http://keq.shanyushiyangkeji.top

for my $x (@arr) { print $x; }
来源：http://bbr.shuidangran.top

[T46] Perl：哈希操作
来源：http://jwz.shangyingyoupin.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://dny.yongpay.top

[T47] Perl：正则捕获
来源：http://npf.wangdashe.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://ato.sxryk.cn

[T48] Perl：正则替换
来源：http://eds.wangdashe.top

$s =~ s/old/new/g;
来源：http://pga.gogol.net.cn

[T49] Perl：函数
来源：http://bpu.yj202588.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://wmr.iojbl.cn

[T50] Perl：逐行读文件
来源：http://epb.sxryk.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://flq.hesvh.cn

while (my $line = <$fh>) { print $line; }
来源：http://zft.cucudq.cn

[T51] Scala：Hello World
来源：http://rbw.sjlbkw.cn

println("Hello")
来源：http://kya.316326.xyz

[T52] Scala：变量
来源：http://lhy.vqdsnc.cn

val a = 1;  var b = 2
来源：http://hke.hammf.cn

[T53] Scala：字符串插值
来源：http://ahe.tarul.cn

s"值: $b"
来源：http://ced.nwbrower.top

[T54] Scala：集合映射
来源：http://zbd.guannengcc.top

List(1, 2, 3).map(_ * 2)
来源：http://oaj.haohaochexian.top

[T55] Scala：集合过滤
来源：http://anw.ydzc1.top

List(1, 2, 3).filter(_ > 1)
来源：http://gpm.tian-w.cn

[T56] Scala：样例类
来源：http://nvn.hesvh.cn

case class User(name: String, age: Int)
来源：http://jtg.redwolf501.top

[T57] Scala：模式匹配
来源：http://jxc.zycfv.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://mmj.dashuyun.cn

[T58] Scala：函数定义
来源：http://egl.daxiang520.top

def add(a: Int, b: Int): Int = a + b
来源：http://mba.yangfankeji.com

[T59] Scala：循环
来源：http://ihc.hongshengwenyu.top

for (i <- 1 to 10) println(i)
来源：http://ndg.hammf.cn

[T60] Scala：折叠
来源：http://ifu.jqgfzy.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://ezi.zhixingplan.top

================================================================================
来源：http://jbo.316326.xyz

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://nox.ctjpmb.com

================================================================================
来源：http://ghi.hongshengwenyu.top

[U01] Py：创建虚拟环境
来源：http://snd.birdmap.top

python -m venv .venv && source .venv/bin/activate
来源：http://ruf.9152youxi.cn

[U02] Py：导出 / 安装依赖
来源：http://ojx.yj20258888.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hgw.52xcode.cn

[U03] Py：加载 .env 配置
来源：http://uyr.zhijiandao.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://fag.shanyushiyangtech.top

[U04] Py：变量调试打印
来源：http://hvx.dianchejie.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://fym.shzxlz.cn

[U05] Py：列表去重且保序
来源：http://vvs.pycfn.com

list(dict.fromkeys(arr))
来源：http://pgt.jiagoushi.top

[U06] Py：合并两个字典
来源：http://ydp.c1oappe.top

{**a, **b}
来源：http://thp.bbcook.cn

[U07] Py：反转字典键值
来源：http://meb.cqqwz.cn

{v: k for k, v in d.items()}
来源：http://slc.cdnleiting.top

[U08] Py：展平二维列表
来源：http://kjx.ydzc1.top

[y for x in nested for y in x]
来源：http://bwg.smart0.xyz

[U09] Py：字典取最大值的键
来源：http://tga.zycfv.cn

max(d, key=d.get)
来源：http://dzp.ydzc1.top

[U10] Py：按值排序字典
来源：http://air.hfpthk.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://xzi.snrcjt.cn

[U11] Py：生成器表达式
来源：http://jlg.sjlbkw.cn

(x * 2 for x in arr)
来源：http://cdi.316326.xyz

[U12] Py：取出现最多的 3 个元素
来源：http://nsz.yvedp.cn

Counter(arr).most_common(3)
来源：http://znm.xingfuxueyuan.xyz

[U13] Py：固定长度队列
来源：http://xpi.jinqigfzy.top

deque(maxlen=10)
来源：http://ase.ppjwa.cn

[U14] Py：分组收集到列表
来源：http://ipg.zhijiandao.cn

defaultdict(list)
来源：http://oxi.52xcode.cn

[U15] Py：高精度计时
来源：http://edj.gotoacloud.top

t = time.perf_counter()
来源：http://ojz.hcnkem.com

[U16] Py：命令行参数解析
来源：http://xsf.ivvv.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://sdw.dashuyun.cn

[U17] Py：初始化日志
来源：http://qqe.cucudq.cn

logging.basicConfig(level=logging.INFO)
来源：http://ndx.ywan-chungtsiang.top

[U18] Py：预编译正则
来源：http://vvz.yongpay.top

pat = re.compile(r"\d+")
来源：http://tvp.epnwcf.com

[U19] Py：正则替换带回调
来源：http://vmb.yj20258888.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://nri.shuidangran.top

[U20] Py：缓存函数结果
来源：http://khp.cheryme.top

@functools.lru_cache(maxsize=None)
来源：http://bek.shanyushiyangkeji.top

[U21] Py：自定义上下文管理器
来源：http://uvs.andypj.xyz

@contextlib.contextmanager
来源：http://gli.shanyushiyangtech.top

[U22] Py：矩阵转置
来源：http://owx.hysaishi.cn

list(zip(*m))
来源：http://kiq.fanxiaobao.xyz

[U23] Py：分块读取大文件
来源：http://qcq.yvedp.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://duj.fengsongda.top

[U24] Py：路径操作
来源：http://uek.guannengcc.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://egp.fehbvm.com

[U25] Py：CSV 按字典读
来源：http://kon.chenzaomai.com

csv.DictReader(f)
来源：http://ybp.0kj1m.cn

[U26] Py：并发下载
来源：http://imn.fengsongda.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://mto.jiagoushi.top

[U27] Py：异步 HTTP
来源：http://bin.smart0.xyz

aiohttp.ClientSession() 配合 async with
来源：http://plm.bjfxy.top

[U28] Py：类型别名
来源：http://zut.zhijiandao.cn

UserId = int
来源：http://wcz.cucudq.cn

[U29] Py：属性校验
来源：http://vnq.zhaomingkeji.xyz

@property 与 @x.setter 配合
来源：http://qqu.gaohongyu789.top

[U30] Py：数据类
来源：http://hxn.hongshengwenyu.top

@dataclass(slots=True)
来源：http://dym.zycfv.cn

[U31] Py：单测
来源：http://kzw.hfpthk.cn

python -m pytest -q
来源：http://anl.zdqjudy.top

[U32] Py：代码格式化
来源：http://bdd.pengpengdd.cyou

ruff format . && ruff check --fix .
来源：http://dpr.haohaochexian.top

[U33] Py：打包发布
来源：http://ago.zhengqikj.top

python -m build  （依赖 pyproject.toml）
来源：http://pba.hammf.cn

[U34] Py：判断编码
来源：http://mjh.gogol.net.cn

chardet.detect(raw)
来源：http://rjp.hesvh.cn

[U35] Py：发送邮件
来源：http://zfn.jiagoushi.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://cgx.zycfv.cn

[U36] Py：定时任务
来源：http://qly.meibo888.top

schedule.every(10).minutes.do(job)
来源：http://tkr.dashuyun.cn

[U37] Py：读写 Excel
来源：http://kcn.cqqwz.cn

pandas.read_excel / DataFrame.to_excel
来源：http://jml.mhx1999.top

[U38] Py：获取脚本所在目录
来源：http://ffm.ybcxt.top

Path(__file__).resolve().parent
来源：http://rci.epnwcf.com

[U39] Py：判断是否在交互环境
来源：http://rkc.hongshengwenyu.top

sys.stdout.isatty()
来源：http://ixf.dianchejie.cn

[U40] Py：打印到标准错误
来源：http://vou.jqgufenzy.top

print("err", file=sys.stderr)
来源：http://xlr.yueranfly.top

[U41] PHP：初始化 Composer 项目
来源：http://bjz.gogol.net.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://smr.vehdjk.com

[U42] PHP：PSR-4 自动加载
来源：http://bat.hammf.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://vei.zhixingplan.top

[U43] PHP：声明命名空间
来源：http://mbf.jlsjyb.cn

namespace App\Http;
来源：http://aqh.yj20258888.top

[U44] PHP：开启严格类型
来源：http://ejv.zdbjq.cn

declare(strict_types=1);
来源：http://hxd.hfpthk.cn

[U45] PHP：类型声明与返回类型
来源：http://zdq.jqgufenzy.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://ywz.pengpengdd.cyou

[U46] PHP：可空类型
来源：http://ldy.cdnleiting.top

?string $name = null
来源：http://xhk.fanxiaobao.xyz

[U47] PHP：联合类型
来源：http://api.c1oappe.top

int|string $id
来源：http://juu.sufxvd.cn

[U48] PHP：纯枚举
来源：http://jqw.c1oappe.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://qiy.xuetiantiany.cn

[U49] PHP：只读属性
来源：http://pon.ywan-chungtsiang.top

public readonly string $name
来源：http://gfp.shzxlz.cn

[U50] PHP：构造器属性提升
来源：http://irm.jianghu66.top

public function __construct(private int $id) {}
来源：http://epf.hfpthk.cn

[U51] PHP：数组解构
来源：http://bea.havefunace.top

[$a, $b] = $arr;
来源：http://omv.haohaochexian.top

[U52] PHP：箭头函数
来源：http://lpi.hnqzz.top

$double = fn($x) => $x * 2;
来源：http://cmf.epnwcf.com

[U53] PHP：空合并运算符
来源：http://ruw.zhengqikj.top

$v = $a ?? $b ?? "default";
来源：http://nfd.xuetiantiany.cn

[U54] PHP：空安全调用
来源：http://pbx.fanxiaobao.xyz

$obj?->method()
来源：http://bmd.gaohongyu789.top

[U55] PHP：match 表达式
来源：http://idg.nanxuanxn.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://wlm.birdmap.top

[U56] PHP：命名参数
来源：http://wyb.nwbrower.top

f(a: 1, b: 2)
来源：http://tqt.xingfuxueyuan.xyz

[U57] PHP：字符串插值
来源：http://pbc.yvedp.cn

"值: {$a}"
来源：http://bna.bbcook.cn

[U58] PHP：数组三件套
来源：http://oit.tian-w.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://thy.yongpay.top

[U59] PHP：自定义排序
来源：http://qeu.snrcjt.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://pgb.chenlongwang.top

[U60] PHP：JSON 编解码
来源：http://wwl.andypj.xyz

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hqh.dashuyun.cn

[U61] PHP：正则
来源：http://nbc.gogol.net.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://vmv.xuanzx.com

[U62] PHP：日期对象
来源：http://bze.wangdashe.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://rfu.ywan-chungtsiang.top

[U63] PHP：文件读写
来源：http://vyd.yangfankeji.com

file_get_contents($f);  file_put_contents($f, $data);
来源：http://zjv.jqgufenzy.top

[U64] PHP：目录遍历
来源：http://jzi.shanyushiyangkeji.top

glob("dir/*.php");  scandir("dir");
来源：http://akq.jinyuanbaomall.cn

[U65] PHP：会话
来源：http://wtz.ctjpmb.com

session_start();  $_SESSION["uid"] = 1;
来源：http://ioz.jinghuilouyu.cn

[U66] PHP：设置 Cookie
来源：http://xkr.ppjwa.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://kok.shzxlz.cn

[U67] PHP：处理文件上传
来源：http://wkq.jlsjyb.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://xuw.zhiwuduotai.top

[U68] PHP：PDO 连接
来源：http://gjy.jiagoushi.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://ktb.svipenyu.cn

[U69] PHP：PDO 预处理
来源：http://fib.meibo888.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://jol.sweek.top

[U70] PHP：PDO 事务
来源：http://nes.0kj1m.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://jub.jqgufenzy.top

[U71] PHP：抛出异常
来源：http://nxg.ppjwa.cn

throw new RuntimeException("失败", 500);
来源：http://tgu.cheryme.top

[U72] PHP：写错误日志
来源：http://nul.epnwcf.com

error_log("失败: " . $e->getMessage());
来源：http://btk.zhengqikj.top

[U73] PHP：读取 ini 配置
来源：http://bya.hcnkem.com

parse_ini_file("config.ini", true)
来源：http://mla.shanyushiyangkeji.top

[U74] PHP：读取环境变量
来源：http://nwk.cashguo.top

getenv("APP_ENV") ?: "production"
来源：http://jtb.yj202588.top

[U75] PHP：依赖注入
来源：http://hhf.haohaochexian.top

composer require psr/container
来源：http://jcy.epnwcf.com

[U76] PHP：简单路由
来源：http://mdm.gzhubu.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://icr.yueranfly.top

[U77] PHP：模板渲染
来源：http://sdz.vqdsnc.cn

composer require twig/twig
来源：http://jav.daria6918.cn

[U78] PHP：单元测试
来源：http://wpc.hnxiangtu.top

composer require --dev phpunit/phpunit
来源：http://vfw.gogol.net.cn

[U79] PHP：静态分析
来源：http://bju.ywan-chungtsiang.top

composer require --dev phpstan/phpstan
来源：http://oex.zhijiandao.cn

[U80] PHP：代码规范修复
来源：http://xrn.jinghuilouyu.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://djv.sxryk.cn

[U81] JS：初始化项目
来源：http://jqt.guowangkeji.top

npm init -y;  npm i express
来源：http://gxd.hfpthk.cn

[U82] JS：package.json 脚本
来源：http://ejh.cashguo.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://fjj.cucudq.cn

[U83] JS：ES Module 导入导出
来源：http://wlc.chenjidiqi.icu

export const a = 1;  import { a } from "./m.js";
来源：http://iwv.redwolf501.top

[U84] JS：CommonJS 写法
来源：http://hyg.0kj1m.cn

module.exports = { a };  const { a } = require("./m");
来源：http://guc.0kj1m.cn

[U85] JS：可选链
来源：http://qus.cheryme.top

a?.b?.c
来源：http://adh.ctjpmb.com

[U86] JS：空值合并
来源：http://knv.hfpthk.cn

a ?? b
来源：http://ehv.zdqjudy.top

[U87] JS：解构默认值
来源：http://eff.yangfankeji.com

const { a = 1, b = 2 } = obj;
来源：http://rjj.yuanzhike.top

[U88] JS：对象展开合并
来源：http://qfx.zdqjudy.top

{ ...a, ...b }
来源：http://cfe.aibaodan.cn

[U89] JS：数组去重
来源：http://zlh.hongshengwenyu.top

[...new Set(arr)]
来源：http://prw.andypj.xyz

[U90] JS：数字数组排序
来源：http://fdr.epnwcf.com

[...arr].sort((a, b) => a - b)
来源：http://thc.cucudq.cn

[U91] JS：对象键值遍历
来源：http://zic.zhaomingkeji.xyz

Object.entries(obj).forEach(([k, v]) => {});
来源：http://rlq.daria6918.cn

[U92] JS：深拷贝
来源：http://hal.yonumen.top

structuredClone(obj)
来源：http://eks.yonumen.top

[U93] JS：模板字符串
来源：http://nxf.kuanghao11.cn

`共 ${n} 条`
来源：http://lir.xuanzx.com

[U94] JS：箭头函数
来源：http://rph.nanxuanxn.top

const double = x => x * 2;
来源：http://tca.jqgufenzy.top

[U95] JS：Promise 包装
来源：http://dpt.cashguo.top

new Promise((resolve, reject) => {})
来源：http://sli.zdqjudy.top

[U96] JS：async/await 与异常
来源：http://rak.9152youxi.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://sbm.jlsjyb.cn

[U97] JS：并发请求
来源：http://seu.cdnleiting.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://flj.gaohongyu789.top

[U98] JS：fetch 带 JSON
来源：http://crd.jyoumei.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://jqk.nanxinkj.top

[U99] JS：事件监听
来源：http://rec.bjfxy.top

el.addEventListener("click", e => {})
来源：http://cph.shanyushiyangkeji.top

[U100] JS：DOM 查询
来源：http://wap.iojbl.cn

document.querySelector(".item")
来源：http://ngp.tianlin.xyz

[U101] JS：classList 操作
来源：http://vce.nanxuanxn.top

el.classList.toggle("active")
来源：http://bxk.ctjpmb.com

[U102] JS：本地存储
来源：http://kxw.zycfv.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://kru.jinqigufen.top

[U103] JS：定时器
来源：http://anp.ivvv.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://wyk.jlsjyb.cn

[U104] JS：防抖
来源：http://bow.yonumen.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://fan.yj202588.top

[U105] JS：节流
来源：http://oce.sysykeji.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://qln.smart0.xyz

[U106] JS：日期格式化
来源：http://dqy.hammf.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://viy.zhixingplan.top

[U107] JS：数字千分位
来源：http://vuh.vehdjk.com

new Intl.NumberFormat("en-US").format(1234567)
来源：http://tlo.bjfxy.top

[U108] JS：随机整数
来源：http://yww.tianlin.xyz

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://kkb.zhixingplan.top

[U109] JS：数组分组
来源：http://qnk.sweek.top

Object.groupBy(arr, x => x.type)
来源：http://qca.jqgufenzy.top

[U110] JS：数组分块
来源：http://pwt.birdmap.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://bmq.ppjwa.cn

[U111] JS：对象转 Map
来源：http://tmy.ppjwa.cn

new Map(Object.entries(obj))
来源：http://cle.quarkkingdee.top

[U112] JS：字符串补位
来源：http://ooo.tianlin.xyz

"7".padStart(3, "0")
来源：http://ncb.316326.xyz

[U113] JS：正则替换全部
来源：http://fna.pengpengdd.cyou

s.replaceAll("a", "b")
来源：http://nnc.shzxlz.cn

[U114] JS：JSON 深比较
来源：http://iqm.tian-w.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://vyr.zdbjq.cn

[U115] JS：生成 UUID
来源：http://myv.cdnleiting.top

crypto.randomUUID()
来源：http://uoc.tanke756.top

[U116] JS：类型检查（JSDoc）
来源：http://jfa.gzhubu.top

/** @param {string} name */ function f(name) {}
来源：http://xhc.sweek.top

[U117] JS：单元测试
来源：http://jgm.jinghuilouyu.cn

npm i -D vitest;  npx vitest
来源：http://rju.ydjk.org.cn

[U118] JS：开发服务器
来源：http://fsj.feifeiyinyue.top

npm i -D vite;  npx vite
来源：http://uzo.kuanghao11.cn

[U119] JS：生产构建
来源：http://rou.dashuyun.cn

npx vite build
来源：http://apt.ehwqpu.com

[U120] JS：读取环境变量（Vite）
来源：http://ngm.gogol.net.cn

import.meta.env.VITE_API_URL
来源：http://oqx.kuanghao11.cn

================================================================================
来源：http://vke.sufxvd.cn

统计汇总
来源：http://kxz.jqgufenzy.top

================================================================================
来源：http://hok.hongshengwenyu.top

按语言统计（条）：
来源：http://gnh.sjlbkw.cn

Python ......... 252
来源：http://qur.gzhubu.top

PHP ............ 252
来源：http://plx.9152youxi.cn

JavaScript ..... 252
来源：http://smv.zhongyouzk.top

TypeScript ..... 212
来源：http://ibx.zhixingplan.top

Java ........... 212
来源：http://byr.tanke756.top

Go ............. 212
来源：http://tlr.yonumen.top

Ruby ........... 212
来源：http://hnh.hnqzz.top

C# ............. 212
来源：http://pwo.zdqjudy.top


<!-- 参考信息 -->