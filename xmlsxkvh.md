代发 wailian999

[T41] Perl：Hello World
来源：http://fgv.xuetiantiany.cn

print "Hello\n";
来源：http://lgw.sufxvd.cn

[T42] Perl：变量类型
来源：http://bfj.sxryk.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://lar.daria6918.cn

[T43] Perl：字符串插值
来源：http://wyi.daxiang520.top

"值: $a"
来源：http://dke.cqqwz.cn

[T44] Perl：条件
来源：http://kex.9152youxi.cn

if ($a > 0) { print "正"; }
来源：http://mmt.daxiang520.top

[T45] Perl：数组遍历
来源：http://hmp.daxiang520.top

for my $x (@arr) { print $x; }
来源：http://fmd.yfazqb.com

[T46] Perl：哈希操作
来源：http://wfd.fengsongda.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://ppy.9152youxi.cn

[T47] Perl：正则捕获
来源：http://bny.zhoulong.xyz

if ($s =~ /(\d+)/) { print $1; }
来源：http://mnx.zhaomingkeji.xyz

[T48] Perl：正则替换
来源：http://rpm.hywenlv.cn

$s =~ s/old/new/g;
来源：http://kxh.yuxming.cn

[T49] Perl：函数
来源：http://kjp.nanxinkj.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://erv.gotoacloud.top

[T50] Perl：逐行读文件
来源：http://dsp.bbcook.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://cju.hysaishi.cn

while (my $line = <$fh>) { print $line; }
来源：http://hjf.kuanghao11.cn

[T51] Scala：Hello World
来源：http://bom.bjfxy.top

println("Hello")
来源：http://oeb.hfpthk.cn

[T52] Scala：变量
来源：http://fer.yuanzhike.top

val a = 1;  var b = 2
来源：http://tgj.sjlbkw.cn

[T53] Scala：字符串插值
来源：http://soj.gotoacloud.top

s"值: $b"
来源：http://tyk.uphjek.com

[T54] Scala：集合映射
来源：http://uho.jianghu66.top

List(1, 2, 3).map(_ * 2)
来源：http://vvt.zhongyouzk.top

[T55] Scala：集合过滤
来源：http://rue.epnwcf.com

List(1, 2, 3).filter(_ > 1)
来源：http://wks.hfpthk.cn

[T56] Scala：样例类
来源：http://gcp.bbcook.cn

case class User(name: String, age: Int)
来源：http://qjp.jiagoushi.top

[T57] Scala：模式匹配
来源：http://khl.jqgfzy.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://icr.wangshuangyany.cn

[T58] Scala：函数定义
来源：http://vqt.sweek.top

def add(a: Int, b: Int): Int = a + b
来源：http://loh.zdqjudy.top

[T59] Scala：循环
来源：http://dnf.9152youxi.cn

for (i <- 1 to 10) println(i)
来源：http://yxx.chenjidiqi.icu

[T60] Scala：折叠
来源：http://yra.fengsongda.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://prd.zhiwuduotai.top

================================================================================
来源：http://zdg.bbcook.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://rrh.zhixingplan.top

================================================================================
来源：http://kpu.hfpthk.cn

[U01] Py：创建虚拟环境
来源：http://giq.guowangkeji.top

python -m venv .venv && source .venv/bin/activate
来源：http://vnm.yanxiufei.cn

[U02] Py：导出 / 安装依赖
来源：http://bww.nanxinkj.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://lit.kuanghao11.cn

[U03] Py：加载 .env 配置
来源：http://okt.yuanzhike.top

from dotenv import load_dotenv; load_dotenv()
来源：http://ekx.hysaishi.cn

[U04] Py：变量调试打印
来源：http://yzd.sysykeji.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://twh.mhx1999.top

[U05] Py：列表去重且保序
来源：http://bxq.epnwcf.com

list(dict.fromkeys(arr))
来源：http://anc.hysaishi.cn

[U06] Py：合并两个字典
来源：http://pma.jyoumei.cn

{**a, **b}
来源：http://eqa.tian-w.cn

[U07] Py：反转字典键值
来源：http://mnb.jianghu66.top

{v: k for k, v in d.items()}
来源：http://jmv.cdnleiting.top

[U08] Py：展平二维列表
来源：http://xwf.jinqigfzy.top

[y for x in nested for y in x]
来源：http://chl.hcnkem.com

[U09] Py：字典取最大值的键
来源：http://npv.sufxvd.cn

max(d, key=d.get)
来源：http://svv.yuxming.cn

[U10] Py：按值排序字典
来源：http://hrp.jianghu66.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://doy.yvedp.cn

[U11] Py：生成器表达式
来源：http://ycv.tian-w.cn

(x * 2 for x in arr)
来源：http://jvo.andypj.xyz

[U12] Py：取出现最多的 3 个元素
来源：http://iuv.cucudq.cn

Counter(arr).most_common(3)
来源：http://uyx.sjlbkw.cn

[U13] Py：固定长度队列
来源：http://jdd.cucudq.cn

deque(maxlen=10)
来源：http://ktx.ywan-chungtsiang.top

[U14] Py：分组收集到列表
来源：http://gwo.zhengqikj.top

defaultdict(list)
来源：http://apu.jinghuilouyu.cn

[U15] Py：高精度计时
来源：http://enp.vqdsnc.cn

t = time.perf_counter()
来源：http://mvq.sxryk.cn

[U16] Py：命令行参数解析
来源：http://ydu.yuanzhike.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://roj.shanyushiyangtech.top

[U17] Py：初始化日志
来源：http://uca.yanxiufei.cn

logging.basicConfig(level=logging.INFO)
来源：http://jzv.zhaomingkeji.xyz

[U18] Py：预编译正则
来源：http://bhz.redwolf501.top

pat = re.compile(r"\d+")
来源：http://aly.bjfxy.top

[U19] Py：正则替换带回调
来源：http://jpq.yongpay.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://ilu.iojbl.cn

[U20] Py：缓存函数结果
来源：http://uht.daxiang520.top

@functools.lru_cache(maxsize=None)
来源：http://wkh.jianghu66.top

[U21] Py：自定义上下文管理器
来源：http://ifz.chenzaomai.com

@contextlib.contextmanager
来源：http://eno.tian-w.cn

[U22] Py：矩阵转置
来源：http://qmr.yangfankeji.com

list(zip(*m))
来源：http://zdl.daxiang520.top

[U23] Py：分块读取大文件
来源：http://tva.jinqigfzy.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://ner.gotoacloud.top

[U24] Py：路径操作
来源：http://zay.zhengqikj.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://qkx.sweek.top

[U25] Py：CSV 按字典读
来源：http://etd.tanke756.top

csv.DictReader(f)
来源：http://rkl.guowangkeji.top

[U26] Py：并发下载
来源：http://jmm.yongpay.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hqy.xuanzx.com

[U27] Py：异步 HTTP
来源：http://gdv.gogol.net.cn

aiohttp.ClientSession() 配合 async with
来源：http://qcj.sysykeji.top

[U28] Py：类型别名
来源：http://erg.yanxiufei.cn

UserId = int
来源：http://nvw.yj20258888.top

[U29] Py：属性校验
来源：http://ols.yongpay.top

@property 与 @x.setter 配合
来源：http://vrs.gotoacloud.top

[U30] Py：数据类
来源：http://xho.hnqzz.top

@dataclass(slots=True)
来源：http://qxy.shanyushiyangkeji.top

[U31] Py：单测
来源：http://qfg.zycfv.cn

python -m pytest -q
来源：http://fai.yuanzhike.top

[U32] Py：代码格式化
来源：http://qlj.gogol.net.cn

ruff format . && ruff check --fix .
来源：http://zyh.mhx1999.top

[U33] Py：打包发布
来源：http://xdj.xuanzx.com

python -m build  （依赖 pyproject.toml）
来源：http://osi.c1oappe.top

[U34] Py：判断编码
来源：http://bux.jiagoushi.top

chardet.detect(raw)
来源：http://ruw.chenlongwang.top

[U35] Py：发送邮件
来源：http://djl.mhx1999.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://wlc.nanxinkj.top

[U36] Py：定时任务
来源：http://ulc.nanxuanxn.top

schedule.every(10).minutes.do(job)
来源：http://lee.jinyuanbaomall.cn

[U37] Py：读写 Excel
来源：http://rpk.tarul.cn

pandas.read_excel / DataFrame.to_excel
来源：http://zzq.xziqi.cn

[U38] Py：获取脚本所在目录
来源：http://eke.fengsongda.top

Path(__file__).resolve().parent
来源：http://zib.feifeiyinyue.top

[U39] Py：判断是否在交互环境
来源：http://wta.epnwcf.com

sys.stdout.isatty()
来源：http://sum.wangshuangyany.cn

[U40] Py：打印到标准错误
来源：http://fwq.chenzaomai.com

print("err", file=sys.stderr)
来源：http://ktj.0kj1m.cn

[U41] PHP：初始化 Composer 项目
来源：http://ptk.uphjek.com

composer init;  composer require guzzlehttp/guzzle
来源：http://ndf.shangyingyoupin.top

[U42] PHP：PSR-4 自动加载
来源：http://lnd.xylfe.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://geb.shangyingyoupin.top

[U43] PHP：声明命名空间
来源：http://grr.redwolf501.top

namespace App\Http;
来源：http://kee.pycfn.com

[U44] PHP：开启严格类型
来源：http://ejn.snrcjt.cn

declare(strict_types=1);
来源：http://skx.uphjek.com

[U45] PHP：类型声明与返回类型
来源：http://dgb.wangdashe.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://yaj.jiagoushi.top

[U46] PHP：可空类型
来源：http://aub.hnqzz.top

?string $name = null
来源：http://ozi.redwolf501.top

[U47] PHP：联合类型
来源：http://pzx.aizwys.cn

int|string $id
来源：http://toj.hnqzz.top

[U48] PHP：纯枚举
来源：http://ase.tianlin.xyz

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://twz.yuanzhike.top

[U49] PHP：只读属性
来源：http://odd.xylfe.cn

public readonly string $name
来源：http://hog.fehbvm.com

[U50] PHP：构造器属性提升
来源：http://phk.havefunace.top

public function __construct(private int $id) {}
来源：http://xoh.hywenlv.cn

[U51] PHP：数组解构
来源：http://hnt.jqgfzy.top

[$a, $b] = $arr;
来源：http://adf.gogol.net.cn

[U52] PHP：箭头函数
来源：http://xdm.snrcjt.cn

$double = fn($x) => $x * 2;
来源：http://ntu.guannengcc.top

[U53] PHP：空合并运算符
来源：http://ttp.vehdjk.com

$v = $a ?? $b ?? "default";
来源：http://tkz.hnxiangtu.top

[U54] PHP：空安全调用
来源：http://qvj.sxryk.cn

$obj?->method()
来源：http://rpb.yongpay.top

[U55] PHP：match 表达式
来源：http://lej.mhx1999.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://wpg.yuanzhike.top

[U56] PHP：命名参数
来源：http://pxz.sweek.top

f(a: 1, b: 2)
来源：http://zbs.c1oappe.top

[U57] PHP：字符串插值
来源：http://iso.mhx1999.top

"值: {$a}"
来源：http://fft.hcnkem.com

[U58] PHP：数组三件套
来源：http://bbn.quarkkingdee.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://zuw.xuetiantiany.cn

[U59] PHP：自定义排序
来源：http://ngd.tarul.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://fxr.haohaochexian.top

[U60] PHP：JSON 编解码
来源：http://lfz.bjfxy.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://pfx.xziqi.cn

[U61] PHP：正则
来源：http://tmu.zdbjq.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://foq.hysaishi.cn

[U62] PHP：日期对象
来源：http://ymy.quarkkingdee.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://ikx.xuetiantiany.cn

[U63] PHP：文件读写
来源：http://omb.0kj1m.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://raz.chenjidiqi.icu

[U64] PHP：目录遍历
来源：http://yhw.zhengqikj.top

glob("dir/*.php");  scandir("dir");
来源：http://rgz.daria6918.cn

[U65] PHP：会话
来源：http://qrp.yuanzhike.top

session_start();  $_SESSION["uid"] = 1;
来源：http://nkc.xingfuxueyuan.xyz

[U66] PHP：设置 Cookie
来源：http://uyb.xylfe.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://oho.9152youxi.cn

[U67] PHP：处理文件上传
来源：http://omu.hnqzz.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://gcp.fzhhl.top

[U68] PHP：PDO 连接
来源：http://zmn.hammf.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://kxv.zhoulong.xyz

[U69] PHP：PDO 预处理
来源：http://grb.xylfe.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://pkd.shzxlz.cn

[U70] PHP：PDO 事务
来源：http://lve.gaohongyu789.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://fnw.zhaomingkeji.xyz

[U71] PHP：抛出异常
来源：http://gii.tian-w.cn

throw new RuntimeException("失败", 500);
来源：http://uzi.gotoacloud.top

[U72] PHP：写错误日志
来源：http://cfp.hnxiangtu.top

error_log("失败: " . $e->getMessage());
来源：http://pzy.quarkkingdee.top

[U73] PHP：读取 ini 配置
来源：http://cbp.pengpengdd.cyou

parse_ini_file("config.ini", true)
来源：http://nyi.fanxiaobao.xyz

[U74] PHP：读取环境变量
来源：http://xkp.ctjpmb.com

getenv("APP_ENV") ?: "production"
来源：http://aao.vehdjk.com

[U75] PHP：依赖注入
来源：http://dmd.guowangkeji.top

composer require psr/container
来源：http://xfs.zhixingplan.top

[U76] PHP：简单路由
来源：http://czk.bjfxy.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://wqx.uphjek.com

[U77] PHP：模板渲染
来源：http://qos.tianlin.xyz

composer require twig/twig
来源：http://yhc.nwbrower.top

[U78] PHP：单元测试
来源：http://rpd.zycfv.cn

composer require --dev phpunit/phpunit
来源：http://zod.jinqigufen.top

[U79] PHP：静态分析
来源：http://crw.xinyue.icu

composer require --dev phpstan/phpstan
来源：http://pvv.tarul.cn

[U80] PHP：代码规范修复
来源：http://fnq.0kj1m.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://myh.bbcook.cn

[U81] JS：初始化项目
来源：http://qgr.chenzaomai.com

npm init -y;  npm i express
来源：http://qru.iojbl.cn

[U82] JS：package.json 脚本
来源：http://meb.iojbl.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://lzl.mhx1999.top

[U83] JS：ES Module 导入导出
来源：http://hve.aibaodan.cn

export const a = 1;  import { a } from "./m.js";
来源：http://kse.sweek.top

[U84] JS：CommonJS 写法
来源：http://aso.smart0.xyz

module.exports = { a };  const { a } = require("./m");
来源：http://vhz.yonumen.top

[U85] JS：可选链
来源：http://oii.birdmap.top

a?.b?.c
来源：http://mgp.jiagoushi.top

[U86] JS：空值合并
来源：http://jga.yfazqb.com

a ?? b
来源：http://cle.hesvh.cn

[U87] JS：解构默认值
来源：http://wuj.fzhhl.top

const { a = 1, b = 2 } = obj;
来源：http://lxq.9152youxi.cn

[U88] JS：对象展开合并
来源：http://iry.meibo888.top

{ ...a, ...b }
来源：http://qmo.sweek.top

[U89] JS：数组去重
来源：http://hmk.birdmap.top

[...new Set(arr)]
来源：http://fyp.jiagoushi.top

[U90] JS：数字数组排序
来源：http://nae.snrcjt.cn

[...arr].sort((a, b) => a - b)
来源：http://kln.jianghu66.top

[U91] JS：对象键值遍历
来源：http://igt.zdbjq.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://dxl.0kj1m.cn

[U92] JS：深拷贝
来源：http://mme.yongpay.top

structuredClone(obj)
来源：http://tcs.xuanzx.com

[U93] JS：模板字符串
来源：http://yha.cheryme.top

`共 ${n} 条`
来源：http://dvq.ppjwa.cn

[U94] JS：箭头函数
来源：http://jki.hysaishi.cn

const double = x => x * 2;
来源：http://xxa.ybcxt.top

[U95] JS：Promise 包装
来源：http://ysy.jlsjyb.cn

new Promise((resolve, reject) => {})
来源：http://lwf.cashguo.top

[U96] JS：async/await 与异常
来源：http://ayf.jyoumei.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://sgh.yj20258.top

[U97] JS：并发请求
来源：http://yib.jinghuilouyu.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://ori.fehbvm.com

[U98] JS：fetch 带 JSON
来源：http://lyg.tian-w.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://bsf.jqgufenzy.top

[U99] JS：事件监听
来源：http://obh.bbcook.cn

el.addEventListener("click", e => {})
来源：http://onr.c1oappe.top

[U100] JS：DOM 查询
来源：http://ijg.jinyuanbaomall.cn

document.querySelector(".item")
来源：http://ybh.ydjk.org.cn

[U101] JS：classList 操作
来源：http://fjo.jinyuanbaomall.cn

el.classList.toggle("active")
来源：http://kha.sweek.top

[U102] JS：本地存储
来源：http://wdu.nanxuanxn.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://flv.zhengqikj.top

[U103] JS：定时器
来源：http://hdn.yonumen.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://idx.iojbl.cn

[U104] JS：防抖
来源：http://ctt.ctjpmb.com

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ukk.hammf.cn

[U105] JS：节流
来源：http://lpp.yj20258888.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://trb.iojbl.cn

[U106] JS：日期格式化
来源：http://rmy.aizwys.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://pyu.shuidangran.top

[U107] JS：数字千分位
来源：http://xxb.svipenyu.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://uht.xylfe.cn

[U108] JS：随机整数
来源：http://lbs.yfazqb.com

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://vjc.yanxiufei.cn

[U109] JS：数组分组
来源：http://ugm.tian-w.cn

Object.groupBy(arr, x => x.type)
来源：http://lso.chenjidiqi.icu

[U110] JS：数组分块
来源：http://uhh.zycfv.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://uhc.mhx1999.top

[U111] JS：对象转 Map
来源：http://mub.ppjwa.cn

new Map(Object.entries(obj))
来源：http://qnf.0kj1m.cn

[U112] JS：字符串补位
来源：http://mba.gzhubu.top

"7".padStart(3, "0")
来源：http://jhl.aibaodan.cn

[U113] JS：正则替换全部
来源：http://jfx.zdbjq.cn

s.replaceAll("a", "b")
来源：http://jey.yvedp.cn

[U114] JS：JSON 深比较
来源：http://hfc.ctjpmb.com

JSON.stringify(a) === JSON.stringify(b)
来源：http://cav.yfazqb.com

[U115] JS：生成 UUID
来源：http://glb.nanxuanxn.top

crypto.randomUUID()
来源：http://sks.c1oappe.top

[U116] JS：类型检查（JSDoc）
来源：http://zbz.xuetiantiany.cn

/** @param {string} name */ function f(name) {}
来源：http://wuj.ehwqpu.com

[U117] JS：单元测试
来源：http://wxy.sjlbkw.cn

npm i -D vitest;  npx vitest
来源：http://hrb.jinghuilouyu.cn

[U118] JS：开发服务器
来源：http://pur.zhijiandao.cn

npm i -D vite;  npx vite
来源：http://sjz.havefunace.top

[U119] JS：生产构建
来源：http://wzv.jlsjyb.cn

npx vite build
来源：http://geo.chenzaomai.com

[U120] JS：读取环境变量（Vite）
来源：http://tbr.fzhhl.top

import.meta.env.VITE_API_URL
来源：http://vdu.yj20258.top

================================================================================
来源：http://pmj.52xcode.cn

统计汇总
来源：http://jul.havefunace.top

================================================================================
来源：http://scp.hammf.cn

按语言统计（条）：
来源：http://cmd.jyoumei.cn

Python ......... 252
来源：http://etd.ywan-chungtsiang.top

PHP ............ 252
来源：http://wpj.yanxiufei.cn

JavaScript ..... 252
来源：http://jxy.ybcxt.top

TypeScript ..... 212
来源：http://lwu.yonumen.top

Java ........... 212
来源：http://eab.hywenlv.cn

Go ............. 212
来源：http://mnh.hysaishi.cn

Ruby ........... 212
来源：http://qtp.wangshuangyany.cn

C# ............. 212
来源：http://poh.chenlongwang.top

C .............. 30
来源：http://lux.316326.xyz

C++ ............ 30
来源：http://hta.jianghu66.top

SQL ............ 90
来源：http://jiv.xuetiantiany.cn

Bash ........... 80
来源：http://coy.vqdsnc.cn


<!-- 参考信息 -->