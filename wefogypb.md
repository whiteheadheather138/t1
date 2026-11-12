代发 wailian999

[T41] Perl：Hello World
来源：http://fkr.yfazqb.com

print "Hello\n";
来源：http://tnf.ctjpmb.com

[T42] Perl：变量类型
来源：http://hok.nwbrower.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://obh.wangshuangyany.cn

[T43] Perl：字符串插值
来源：http://cfz.shanyushiyangtech.top

"值: $a"
来源：http://npo.yangfankeji.com

[T44] Perl：条件
来源：http://abu.yongpay.top

if ($a > 0) { print "正"; }
来源：http://pdn.wangshuangyany.cn

[T45] Perl：数组遍历
来源：http://url.dianchejie.cn

for my $x (@arr) { print $x; }
来源：http://bxh.sweek.top

[T46] Perl：哈希操作
来源：http://jmo.gzhubu.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://alm.cqqwz.cn

[T47] Perl：正则捕获
来源：http://qmm.jqgfzy.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://qqa.316326.xyz

[T48] Perl：正则替换
来源：http://rry.jqgufenzy.top

$s =~ s/old/new/g;
来源：http://clb.jianghu66.top

[T49] Perl：函数
来源：http://wua.zhiwuduotai.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://qol.cdnleiting.top

[T50] Perl：逐行读文件
来源：http://izr.havefunace.top

open my $fh, "<", "a.txt" or die $!;
来源：http://aos.vqdsnc.cn

while (my $line = <$fh>) { print $line; }
来源：http://hev.daxiang520.top

[T51] Scala：Hello World
来源：http://nnf.wangdashe.top

println("Hello")
来源：http://dys.ybcxt.top

[T52] Scala：变量
来源：http://zdb.zhongyouzk.top

val a = 1;  var b = 2
来源：http://rhb.wangdashe.top

[T53] Scala：字符串插值
来源：http://jwc.havefunace.top

s"值: $b"
来源：http://yiy.zhoulong.xyz

[T54] Scala：集合映射
来源：http://fzh.yangfankeji.com

List(1, 2, 3).map(_ * 2)
来源：http://fpa.feifeiyinyue.top

[T55] Scala：集合过滤
来源：http://kue.iojbl.cn

List(1, 2, 3).filter(_ > 1)
来源：http://qcy.hysaishi.cn

[T56] Scala：样例类
来源：http://lcl.xinyue.icu

case class User(name: String, age: Int)
来源：http://pmw.yj202588.top

[T57] Scala：模式匹配
来源：http://tqj.yongpay.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://ohb.yj20258888.top

[T58] Scala：函数定义
来源：http://vug.shuidangran.top

def add(a: Int, b: Int): Int = a + b
来源：http://ffq.zhixingplan.top

[T59] Scala：循环
来源：http://ryn.guowangkeji.top

for (i <- 1 to 10) println(i)
来源：http://yzh.zhongyouzk.top

[T60] Scala：折叠
来源：http://wex.jqgfzy.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://sel.cqqwz.cn

================================================================================
来源：http://uop.uphjek.com

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://uif.fzhhl.top

================================================================================
来源：http://bgw.sweek.top

[U01] Py：创建虚拟环境
来源：http://xpt.sweek.top

python -m venv .venv && source .venv/bin/activate
来源：http://hiy.ivvv.top

[U02] Py：导出 / 安装依赖
来源：http://pxm.tarul.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://ljs.hammf.cn

[U03] Py：加载 .env 配置
来源：http://hib.bjfxy.top

from dotenv import load_dotenv; load_dotenv()
来源：http://vgt.ehwqpu.com

[U04] Py：变量调试打印
来源：http://gkn.pycfn.com

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://evz.vqdsnc.cn

[U05] Py：列表去重且保序
来源：http://luz.wangdashe.top

list(dict.fromkeys(arr))
来源：http://rox.gaohongyu789.top

[U06] Py：合并两个字典
来源：http://gfo.wangshuangyany.cn

{**a, **b}
来源：http://pqx.tian-w.cn

[U07] Py：反转字典键值
来源：http://teo.ehwqpu.com

{v: k for k, v in d.items()}
来源：http://wnr.gaohongyu789.top

[U08] Py：展平二维列表
来源：http://lef.birdmap.top

[y for x in nested for y in x]
来源：http://bmx.shuidangran.top

[U09] Py：字典取最大值的键
来源：http://zzc.52xcode.cn

max(d, key=d.get)
来源：http://fat.yj20258888.top

[U10] Py：按值排序字典
来源：http://oly.fzhhl.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://wzk.fktsv.cn

[U11] Py：生成器表达式
来源：http://wkd.jinqigufen.top

(x * 2 for x in arr)
来源：http://hzl.zhiwuduotai.top

[U12] Py：取出现最多的 3 个元素
来源：http://etd.andypj.xyz

Counter(arr).most_common(3)
来源：http://iaw.bjfxy.top

[U13] Py：固定长度队列
来源：http://cqy.xinyue.icu

deque(maxlen=10)
来源：http://apg.xuanzx.com

[U14] Py：分组收集到列表
来源：http://rdx.jinqigfzy.top

defaultdict(list)
来源：http://cyt.cashguo.top

[U15] Py：高精度计时
来源：http://flw.sweek.top

t = time.perf_counter()
来源：http://gjh.svipenyu.cn

[U16] Py：命令行参数解析
来源：http://grx.yuxming.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://ckq.zdqjudy.top

[U17] Py：初始化日志
来源：http://aoc.jinyuanbaomall.cn

logging.basicConfig(level=logging.INFO)
来源：http://igv.fanxiaobao.xyz

[U18] Py：预编译正则
来源：http://otd.yj20258.top

pat = re.compile(r"\d+")
来源：http://rlx.ctjpmb.com

[U19] Py：正则替换带回调
来源：http://lgs.cdnleiting.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://ssr.hywenlv.cn

[U20] Py：缓存函数结果
来源：http://nsz.svipenyu.cn

@functools.lru_cache(maxsize=None)
来源：http://qzw.sysykeji.top

[U21] Py：自定义上下文管理器
来源：http://qqt.quarkkingdee.top

@contextlib.contextmanager
来源：http://gzu.svipenyu.cn

[U22] Py：矩阵转置
来源：http://wwc.redwolf501.top

list(zip(*m))
来源：http://nrw.hesvh.cn

[U23] Py：分块读取大文件
来源：http://gtd.uphjek.com

for chunk in iter(lambda: f.read(8192), b""):
来源：http://bnc.kuanghao11.cn

[U24] Py：路径操作
来源：http://lmf.shuidangran.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://rlp.hcnkem.com

[U25] Py：CSV 按字典读
来源：http://ovu.cucudq.cn

csv.DictReader(f)
来源：http://ldz.ybcxt.top

[U26] Py：并发下载
来源：http://gmv.jinqigfzy.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://rby.yj20258888.top

[U27] Py：异步 HTTP
来源：http://kxc.c1oappe.top

aiohttp.ClientSession() 配合 async with
来源：http://fke.yueranfly.top

[U28] Py：类型别名
来源：http://zby.jinqigfzy.top

UserId = int
来源：http://fft.sweek.top

[U29] Py：属性校验
来源：http://zju.xinyue.icu

@property 与 @x.setter 配合
来源：http://ygh.hammf.cn

[U30] Py：数据类
来源：http://uvp.jqgfzy.top

@dataclass(slots=True)
来源：http://his.snrcjt.cn

[U31] Py：单测
来源：http://rgp.hywenlv.cn

python -m pytest -q
来源：http://blp.smart0.xyz

[U32] Py：代码格式化
来源：http://kot.sjlbkw.cn

ruff format . && ruff check --fix .
来源：http://yhw.hnxiangtu.top

[U33] Py：打包发布
来源：http://lzt.yuxming.cn

python -m build  （依赖 pyproject.toml）
来源：http://oaq.zhengqikj.top

[U34] Py：判断编码
来源：http://svf.zdqjudy.top

chardet.detect(raw)
来源：http://iwy.sjlbkw.cn

[U35] Py：发送邮件
来源：http://kjt.gaohongyu789.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://fcm.wangshuangyany.cn

[U36] Py：定时任务
来源：http://lyx.zycfv.cn

schedule.every(10).minutes.do(job)
来源：http://vhj.hesvh.cn

[U37] Py：读写 Excel
来源：http://akv.xylfe.cn

pandas.read_excel / DataFrame.to_excel
来源：http://tzu.yvedp.cn

[U38] Py：获取脚本所在目录
来源：http://rec.yfazqb.com

Path(__file__).resolve().parent
来源：http://ydk.tianlin.xyz

[U39] Py：判断是否在交互环境
来源：http://wsl.yanxiufei.cn

sys.stdout.isatty()
来源：http://ofh.yonumen.top

[U40] Py：打印到标准错误
来源：http://wrg.yueranfly.top

print("err", file=sys.stderr)
来源：http://yme.jinqigufen.top

[U41] PHP：初始化 Composer 项目
来源：http://rbm.shanyushiyangtech.top

composer init;  composer require guzzlehttp/guzzle
来源：http://jam.hfpthk.cn

[U42] PHP：PSR-4 自动加载
来源：http://rkl.birdmap.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://uga.jiagoushi.top

[U43] PHP：声明命名空间
来源：http://ntk.zhixingplan.top

namespace App\Http;
来源：http://gyb.jinyuanbaomall.cn

[U44] PHP：开启严格类型
来源：http://phy.fengsongda.top

declare(strict_types=1);
来源：http://obt.tian-w.cn

[U45] PHP：类型声明与返回类型
来源：http://nqb.hcnkem.com

function add(int $a, int $b): int { return $a + $b; }
来源：http://hgn.guowangkeji.top

[U46] PHP：可空类型
来源：http://vdb.cucudq.cn

?string $name = null
来源：http://ckn.daxiang520.top

[U47] PHP：联合类型
来源：http://xee.hongshengwenyu.top

int|string $id
来源：http://wqw.jianghu66.top

[U48] PHP：纯枚举
来源：http://yiy.bjfxy.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://siv.vqdsnc.cn

[U49] PHP：只读属性
来源：http://nla.sysykeji.top

public readonly string $name
来源：http://ded.cashguo.top

[U50] PHP：构造器属性提升
来源：http://sik.tarul.cn

public function __construct(private int $id) {}
来源：http://jrg.nanxuanxn.top

[U51] PHP：数组解构
来源：http://lgn.chenzaomai.com

[$a, $b] = $arr;
来源：http://iaw.shzxlz.cn

[U52] PHP：箭头函数
来源：http://qde.fktsv.cn

$double = fn($x) => $x * 2;
来源：http://xoy.zhengqikj.top

[U53] PHP：空合并运算符
来源：http://wxm.guannengcc.top

$v = $a ?? $b ?? "default";
来源：http://wji.hnxiangtu.top

[U54] PHP：空安全调用
来源：http://jww.nwbrower.top

$obj?->method()
来源：http://agg.jinghuilouyu.cn

[U55] PHP：match 表达式
来源：http://tko.smart0.xyz

$s = match($x) { 1 => "一", default => "其他" };
来源：http://qnd.shangyingyoupin.top

[U56] PHP：命名参数
来源：http://msh.tianlin.xyz

f(a: 1, b: 2)
来源：http://vnv.shanyushiyangkeji.top

[U57] PHP：字符串插值
来源：http://mwo.bjfxy.top

"值: {$a}"
来源：http://hgm.chenzaomai.com

[U58] PHP：数组三件套
来源：http://pry.yonumen.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://pwp.zdqjudy.top

[U59] PHP：自定义排序
来源：http://wdb.hesvh.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://twm.316326.xyz

[U60] PHP：JSON 编解码
来源：http://nci.fzhhl.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://rhu.zdbjq.cn

[U61] PHP：正则
来源：http://lps.daria6918.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://jdi.hysaishi.cn

[U62] PHP：日期对象
来源：http://gmn.cqqwz.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://niq.bbcook.cn

[U63] PHP：文件读写
来源：http://tug.yonumen.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://pdc.snrcjt.cn

[U64] PHP：目录遍历
来源：http://yvf.ehwqpu.com

glob("dir/*.php");  scandir("dir");
来源：http://tpd.cheryme.top

[U65] PHP：会话
来源：http://jmr.gotoacloud.top

session_start();  $_SESSION["uid"] = 1;
来源：http://pkz.haohaochexian.top

[U66] PHP：设置 Cookie
来源：http://ydh.yj202588.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://cfp.0kj1m.cn

[U67] PHP：处理文件上传
来源：http://tvn.pengpengdd.cyou

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://oin.cqqwz.cn

[U68] PHP：PDO 连接
来源：http://rtj.quarkkingdee.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://nnd.smart0.xyz

[U69] PHP：PDO 预处理
来源：http://rnx.uphjek.com

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://eeq.tian-w.cn

[U70] PHP：PDO 事务
来源：http://ikl.feifeiyinyue.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://puf.xinyue.icu

[U71] PHP：抛出异常
来源：http://mjg.hysaishi.cn

throw new RuntimeException("失败", 500);
来源：http://wbi.jqgfzy.top

[U72] PHP：写错误日志
来源：http://xvb.hesvh.cn

error_log("失败: " . $e->getMessage());
来源：http://zbz.0kj1m.cn

[U73] PHP：读取 ini 配置
来源：http://vgk.shanyushiyangtech.top

parse_ini_file("config.ini", true)
来源：http://tih.yueranfly.top

[U74] PHP：读取环境变量
来源：http://ugd.fktsv.cn

getenv("APP_ENV") ?: "production"
来源：http://anw.tanke756.top

[U75] PHP：依赖注入
来源：http://pdc.shanyushiyangtech.top

composer require psr/container
来源：http://xqa.zhengqikj.top

[U76] PHP：简单路由
来源：http://zuj.hongshengwenyu.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://pjf.hesvh.cn

[U77] PHP：模板渲染
来源：http://qxc.shanyushiyangkeji.top

composer require twig/twig
来源：http://uan.zhoulong.xyz

[U78] PHP：单元测试
来源：http://fsi.yueranfly.top

composer require --dev phpunit/phpunit
来源：http://tcn.cqqwz.cn

[U79] PHP：静态分析
来源：http://aqn.0kj1m.cn

composer require --dev phpstan/phpstan
来源：http://pkm.gogol.net.cn

[U80] PHP：代码规范修复
来源：http://ofz.daria6918.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://xlb.shzxlz.cn

[U81] JS：初始化项目
来源：http://wga.yongpay.top

npm init -y;  npm i express
来源：http://bxe.yongpay.top

[U82] JS：package.json 脚本
来源：http://ovv.pycfn.com

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://sid.zdbjq.cn

[U83] JS：ES Module 导入导出
来源：http://vzv.kuanghao11.cn

export const a = 1;  import { a } from "./m.js";
来源：http://wyq.yongpay.top

[U84] JS：CommonJS 写法
来源：http://yse.ywan-chungtsiang.top

module.exports = { a };  const { a } = require("./m");
来源：http://hsa.fanxiaobao.xyz

[U85] JS：可选链
来源：http://obt.tanke756.top

a?.b?.c
来源：http://mvx.gotoacloud.top

[U86] JS：空值合并
来源：http://cin.hysaishi.cn

a ?? b
来源：http://emt.zycfv.cn

[U87] JS：解构默认值
来源：http://eey.nanxuanxn.top

const { a = 1, b = 2 } = obj;
来源：http://scb.mhx1999.top

[U88] JS：对象展开合并
来源：http://dmp.iojbl.cn

{ ...a, ...b }
来源：http://tha.pengpengdd.cyou

[U89] JS：数组去重
来源：http://wjz.havefunace.top

[...new Set(arr)]
来源：http://qwd.hcnkem.com

[U90] JS：数字数组排序
来源：http://nig.hnxiangtu.top

[...arr].sort((a, b) => a - b)
来源：http://acb.xingfuxueyuan.xyz

[U91] JS：对象键值遍历
来源：http://czi.pycfn.com

Object.entries(obj).forEach(([k, v]) => {});
来源：http://agn.ctjpmb.com

[U92] JS：深拷贝
来源：http://dre.fengsongda.top

structuredClone(obj)
来源：http://xlo.gaohongyu789.top

[U93] JS：模板字符串
来源：http://sgu.ehwqpu.com

`共 ${n} 条`
来源：http://ptz.xziqi.cn

[U94] JS：箭头函数
来源：http://una.zhengqikj.top

const double = x => x * 2;
来源：http://ado.shangyingyoupin.top

[U95] JS：Promise 包装
来源：http://bmx.guannengcc.top

new Promise((resolve, reject) => {})
来源：http://ima.yfazqb.com

[U96] JS：async/await 与异常
来源：http://xgg.redwolf501.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://oye.gaohongyu789.top

[U97] JS：并发请求
来源：http://jzg.jinqigfzy.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://lyt.zdbjq.cn

[U98] JS：fetch 带 JSON
来源：http://xwq.tarul.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://wcs.fehbvm.com

[U99] JS：事件监听
来源：http://oxp.bjfxy.top

el.addEventListener("click", e => {})
来源：http://rgb.jyoumei.cn

[U100] JS：DOM 查询
来源：http://oas.andypj.xyz

document.querySelector(".item")
来源：http://bia.xingfuxueyuan.xyz

[U101] JS：classList 操作
来源：http://ppo.gogol.net.cn

el.classList.toggle("active")
来源：http://pcf.ybcxt.top

[U102] JS：本地存储
来源：http://cwm.aizwys.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://xby.wangdashe.top

[U103] JS：定时器
来源：http://tiz.shuidangran.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://iia.kuanghao11.cn

[U104] JS：防抖
来源：http://aqv.chenjidiqi.icu

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://kyy.jinqigfzy.top

[U105] JS：节流
来源：http://pds.ydzc1.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://ryp.wangshuangyany.cn

[U106] JS：日期格式化
来源：http://ufz.ppjwa.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://zqm.aibaodan.cn

[U107] JS：数字千分位
来源：http://yda.hesvh.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://ygq.zhijiandao.cn

[U108] JS：随机整数
来源：http://fjd.yj20258888.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://gik.yj20258.top

[U109] JS：数组分组
来源：http://wvq.ehwqpu.com

Object.groupBy(arr, x => x.type)
来源：http://ffv.hfpthk.cn

[U110] JS：数组分块
来源：http://rpk.ywan-chungtsiang.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://lwz.shzxlz.cn

[U111] JS：对象转 Map
来源：http://hro.tarul.cn

new Map(Object.entries(obj))
来源：http://etn.epnwcf.com

[U112] JS：字符串补位
来源：http://alo.tarul.cn

"7".padStart(3, "0")
来源：http://noz.gaohongyu789.top

[U113] JS：正则替换全部
来源：http://dxf.chenlongwang.top

s.replaceAll("a", "b")
来源：http://tqq.yfazqb.com

[U114] JS：JSON 深比较
来源：http://iod.svipenyu.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://gur.iojbl.cn

[U115] JS：生成 UUID
来源：http://ypp.sufxvd.cn

crypto.randomUUID()
来源：http://cjl.shzxlz.cn

[U116] JS：类型检查（JSDoc）
来源：http://kuo.yanxiufei.cn

/** @param {string} name */ function f(name) {}
来源：http://nsl.fengsongda.top

[U117] JS：单元测试
来源：http://dhx.c1oappe.top

npm i -D vitest;  npx vitest
来源：http://zbn.xuetiantiany.cn

[U118] JS：开发服务器
来源：http://xzn.yj202588.top

npm i -D vite;  npx vite
来源：http://dof.316326.xyz

[U119] JS：生产构建
来源：http://jwd.hysaishi.cn

npx vite build
来源：http://beh.shangyingyoupin.top

[U120] JS：读取环境变量（Vite）
来源：http://mxf.xziqi.cn

import.meta.env.VITE_API_URL
来源：http://qxb.chenjidiqi.icu

================================================================================
来源：http://ozh.svipenyu.cn

统计汇总
来源：http://bdo.jinqigufen.top

================================================================================
来源：http://jam.sxryk.cn

按语言统计（条）：
来源：http://wag.316326.xyz

Python ......... 252
来源：http://icx.fehbvm.com

PHP ............ 252
来源：http://unb.birdmap.top

JavaScript ..... 252
来源：http://sbg.yuanzhike.top

TypeScript ..... 212
来源：http://luv.cucudq.cn

Java ........... 212
来源：http://gha.jinghuilouyu.cn

Go ............. 212
来源：http://bow.jinqigfzy.top

Ruby ........... 212
来源：http://pov.yuxming.cn

C# ............. 212
来源：http://ple.vehdjk.com

C .............. 30
来源：http://gqy.shanyushiyangtech.top

C++ ............ 30
来源：http://aju.kuanghao11.cn

SQL ............ 90
来源：http://brg.haohaochexian.top

Bash ........... 80
来源：http://qsj.daxiang520.top


<!-- 参考信息 -->