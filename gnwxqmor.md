代发 wailian999

[T33] Lua：表（数组）
来源：http://tgb.zhijiandao.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://hdu.hammf.cn

[T34] Lua：遍历表
来源：http://pnu.fktsv.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://zwh.c1oappe.top

[T35] Lua：字典表
来源：http://lcm.shanyushiyangtech.top

local d = { a = 1 };  d.b = 2
来源：http://pgr.cashguo.top

[T36] Lua：函数
来源：http://bjl.jinqigfzy.top

function add(a, b) return a + b end
来源：http://gid.hfpthk.cn

[T37] Lua：字符串拼接
来源：http://jub.kuanghao11.cn

"a" .. "b"
来源：http://ssx.xylfe.cn

[T38] Lua：条件
来源：http://ese.hnqzz.top

if x > 0 then print("正") end
来源：http://wsv.hcnkem.com

[T39] Lua：模式匹配
来源：http://fxy.epnwcf.com

string.find(s, "%d+")
来源：http://wga.guannengcc.top

[T40] Lua：元表
来源：http://rag.tian-w.cn

setmetatable({}, { __index = base })
来源：http://ebe.tarul.cn

[T41] Perl：Hello World
来源：http://tch.daria6918.cn

print "Hello\n";
来源：http://wcg.shuidangran.top

[T42] Perl：变量类型
来源：http://fnr.yuanzhike.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://qtt.xinyue.icu

[T43] Perl：字符串插值
来源：http://zsb.nanxinkj.top

"值: $a"
来源：http://org.feifeiyinyue.top

[T44] Perl：条件
来源：http://ojl.52xcode.cn

if ($a > 0) { print "正"; }
来源：http://psk.sjlbkw.cn

[T45] Perl：数组遍历
来源：http://dht.daria6918.cn

for my $x (@arr) { print $x; }
来源：http://zrs.jiagoushi.top

[T46] Perl：哈希操作
来源：http://gtp.yuxming.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://ioy.ehwqpu.com

[T47] Perl：正则捕获
来源：http://hwd.vqdsnc.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://xgl.dianchejie.cn

[T48] Perl：正则替换
来源：http://xkc.shanyushiyangtech.top

$s =~ s/old/new/g;
来源：http://qri.bbcook.cn

[T49] Perl：函数
来源：http://cgd.yj20258888.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://jki.zdbjq.cn

[T50] Perl：逐行读文件
来源：http://tzh.sxryk.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://flj.0kj1m.cn

while (my $line = <$fh>) { print $line; }
来源：http://caq.vqdsnc.cn

[T51] Scala：Hello World
来源：http://cll.zhaomingkeji.xyz

println("Hello")
来源：http://uuu.ybcxt.top

[T52] Scala：变量
来源：http://xsq.cucudq.cn

val a = 1;  var b = 2
来源：http://ude.yueranfly.top

[T53] Scala：字符串插值
来源：http://mhv.chenlongwang.top

s"值: $b"
来源：http://vsr.hesvh.cn

[T54] Scala：集合映射
来源：http://qug.vehdjk.com

List(1, 2, 3).map(_ * 2)
来源：http://wif.daxiang520.top

[T55] Scala：集合过滤
来源：http://cxp.shangyingyoupin.top

List(1, 2, 3).filter(_ > 1)
来源：http://hfp.shangyingyoupin.top

[T56] Scala：样例类
来源：http://kbw.ydzc1.top

case class User(name: String, age: Int)
来源：http://uml.yuxming.cn

[T57] Scala：模式匹配
来源：http://nec.shuidangran.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://abb.yanxiufei.cn

[T58] Scala：函数定义
来源：http://asc.sjlbkw.cn

def add(a: Int, b: Int): Int = a + b
来源：http://mgh.jianghu66.top

[T59] Scala：循环
来源：http://bor.daxiang520.top

for (i <- 1 to 10) println(i)
来源：http://uad.zdbjq.cn

[T60] Scala：折叠
来源：http://zmj.yuxming.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://omz.jqgfzy.top

================================================================================
来源：http://roi.zycfv.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://yhk.shangyingyoupin.top

================================================================================
来源：http://rxd.chenzaomai.com

[U01] Py：创建虚拟环境
来源：http://nnx.cucudq.cn

python -m venv .venv && source .venv/bin/activate
来源：http://pmn.tanke756.top

[U02] Py：导出 / 安装依赖
来源：http://eza.yonumen.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://loz.hfpthk.cn

[U03] Py：加载 .env 配置
来源：http://hnz.yonumen.top

from dotenv import load_dotenv; load_dotenv()
来源：http://ryy.andypj.xyz

[U04] Py：变量调试打印
来源：http://xcu.sxryk.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://ppf.meibo888.top

[U05] Py：列表去重且保序
来源：http://cqf.xuanzx.com

list(dict.fromkeys(arr))
来源：http://zva.cqqwz.cn

[U06] Py：合并两个字典
来源：http://xrb.dashuyun.cn

{**a, **b}
来源：http://yjc.guowangkeji.top

[U07] Py：反转字典键值
来源：http://aaf.zycfv.cn

{v: k for k, v in d.items()}
来源：http://uam.zhongyouzk.top

[U08] Py：展平二维列表
来源：http://wrt.aizwys.cn

[y for x in nested for y in x]
来源：http://zrg.smart0.xyz

[U09] Py：字典取最大值的键
来源：http://qeb.chenjidiqi.icu

max(d, key=d.get)
来源：http://gim.jyoumei.cn

[U10] Py：按值排序字典
来源：http://swd.yvedp.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://zzu.hywenlv.cn

[U11] Py：生成器表达式
来源：http://rlb.guowangkeji.top

(x * 2 for x in arr)
来源：http://bvq.meibo888.top

[U12] Py：取出现最多的 3 个元素
来源：http://fnr.hammf.cn

Counter(arr).most_common(3)
来源：http://sdj.ctjpmb.com

[U13] Py：固定长度队列
来源：http://pmd.pengpengdd.cyou

deque(maxlen=10)
来源：http://pow.sxryk.cn

[U14] Py：分组收集到列表
来源：http://lse.jiagoushi.top

defaultdict(list)
来源：http://yqf.gogol.net.cn

[U15] Py：高精度计时
来源：http://hyf.wangdashe.top

t = time.perf_counter()
来源：http://npi.sufxvd.cn

[U16] Py：命令行参数解析
来源：http://suh.hongshengwenyu.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://ezh.jianghu66.top

[U17] Py：初始化日志
来源：http://pbd.wangshuangyany.cn

logging.basicConfig(level=logging.INFO)
来源：http://jbc.yuxming.cn

[U18] Py：预编译正则
来源：http://cvz.52xcode.cn

pat = re.compile(r"\d+")
来源：http://tny.hongshengwenyu.top

[U19] Py：正则替换带回调
来源：http://yte.sjlbkw.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://yze.jinqigfzy.top

[U20] Py：缓存函数结果
来源：http://vpf.fehbvm.com

@functools.lru_cache(maxsize=None)
来源：http://zcx.shanyushiyangkeji.top

[U21] Py：自定义上下文管理器
来源：http://ght.ehwqpu.com

@contextlib.contextmanager
来源：http://zwh.wangdashe.top

[U22] Py：矩阵转置
来源：http://zmc.hfpthk.cn

list(zip(*m))
来源：http://bge.mhx1999.top

[U23] Py：分块读取大文件
来源：http://nna.chenlongwang.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://qpt.meibo888.top

[U24] Py：路径操作
来源：http://fdb.chenzaomai.com

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://pnj.jlsjyb.cn

[U25] Py：CSV 按字典读
来源：http://afn.ydjk.org.cn

csv.DictReader(f)
来源：http://hao.yonumen.top

[U26] Py：并发下载
来源：http://kuo.gzhubu.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://ddh.vehdjk.com

[U27] Py：异步 HTTP
来源：http://onf.chenjidiqi.icu

aiohttp.ClientSession() 配合 async with
来源：http://pjm.cashguo.top

[U28] Py：类型别名
来源：http://vhh.zhijiandao.cn

UserId = int
来源：http://qhh.hywenlv.cn

[U29] Py：属性校验
来源：http://kyr.ehwqpu.com

@property 与 @x.setter 配合
来源：http://ttl.gaohongyu789.top

[U30] Py：数据类
来源：http://ivx.cdnleiting.top

@dataclass(slots=True)
来源：http://buq.xingfuxueyuan.xyz

[U31] Py：单测
来源：http://lue.epnwcf.com

python -m pytest -q
来源：http://ibo.kuanghao11.cn

[U32] Py：代码格式化
来源：http://xdt.fktsv.cn

ruff format . && ruff check --fix .
来源：http://wai.zhengqikj.top

[U33] Py：打包发布
来源：http://bwu.ywan-chungtsiang.top

python -m build  （依赖 pyproject.toml）
来源：http://zow.yongpay.top

[U34] Py：判断编码
来源：http://ucm.snrcjt.cn

chardet.detect(raw)
来源：http://wtj.shanyushiyangtech.top

[U35] Py：发送邮件
来源：http://rby.chenjidiqi.icu

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://rnl.epnwcf.com

[U36] Py：定时任务
来源：http://syr.iojbl.cn

schedule.every(10).minutes.do(job)
来源：http://uuj.bjfxy.top

[U37] Py：读写 Excel
来源：http://sib.pengpengdd.cyou

pandas.read_excel / DataFrame.to_excel
来源：http://tes.wangshuangyany.cn

[U38] Py：获取脚本所在目录
来源：http://rgg.meibo888.top

Path(__file__).resolve().parent
来源：http://vqe.9152youxi.cn

[U39] Py：判断是否在交互环境
来源：http://ava.ydzc1.top

sys.stdout.isatty()
来源：http://nqc.sweek.top

[U40] Py：打印到标准错误
来源：http://pzo.pycfn.com

print("err", file=sys.stderr)
来源：http://qop.bbcook.cn

[U41] PHP：初始化 Composer 项目
来源：http://krs.guowangkeji.top

composer init;  composer require guzzlehttp/guzzle
来源：http://tvz.wangdashe.top

[U42] PHP：PSR-4 自动加载
来源：http://ujg.hysaishi.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://pnj.chenjidiqi.icu

[U43] PHP：声明命名空间
来源：http://tss.gzhubu.top

namespace App\Http;
来源：http://jio.zycfv.cn

[U44] PHP：开启严格类型
来源：http://cqw.gogol.net.cn

declare(strict_types=1);
来源：http://aht.xziqi.cn

[U45] PHP：类型声明与返回类型
来源：http://hww.hongshengwenyu.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://qua.birdmap.top

[U46] PHP：可空类型
来源：http://mcm.daria6918.cn

?string $name = null
来源：http://lfu.guannengcc.top

[U47] PHP：联合类型
来源：http://clu.zdqjudy.top

int|string $id
来源：http://aop.chenlongwang.top

[U48] PHP：纯枚举
来源：http://qrc.jiagoushi.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://ivu.pycfn.com

[U49] PHP：只读属性
来源：http://icq.cqqwz.cn

public readonly string $name
来源：http://hhu.sweek.top

[U50] PHP：构造器属性提升
来源：http://mlk.9152youxi.cn

public function __construct(private int $id) {}
来源：http://gyc.ybcxt.top

[U51] PHP：数组解构
来源：http://jdy.nwbrower.top

[$a, $b] = $arr;
来源：http://bsd.shangyingyoupin.top

[U52] PHP：箭头函数
来源：http://usr.tanke756.top

$double = fn($x) => $x * 2;
来源：http://egb.fehbvm.com

[U53] PHP：空合并运算符
来源：http://bce.zhaomingkeji.xyz

$v = $a ?? $b ?? "default";
来源：http://spy.ywan-chungtsiang.top

[U54] PHP：空安全调用
来源：http://oaq.chenzaomai.com

$obj?->method()
来源：http://jxs.uphjek.com

[U55] PHP：match 表达式
来源：http://tui.zdbjq.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://ruw.yvedp.cn

[U56] PHP：命名参数
来源：http://xrq.jlsjyb.cn

f(a: 1, b: 2)
来源：http://yqf.mhx1999.top

[U57] PHP：字符串插值
来源：http://brf.bjfxy.top

"值: {$a}"
来源：http://zxc.chenlongwang.top

[U58] PHP：数组三件套
来源：http://sjy.yanxiufei.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://ndi.zhijiandao.cn

[U59] PHP：自定义排序
来源：http://rwh.daxiang520.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://jbc.shuidangran.top

[U60] PHP：JSON 编解码
来源：http://bnf.smart0.xyz

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://nda.jinyuanbaomall.cn

[U61] PHP：正则
来源：http://yha.zhiwuduotai.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://eti.gaohongyu789.top

[U62] PHP：日期对象
来源：http://cfz.cucudq.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://fbt.yongpay.top

[U63] PHP：文件读写
来源：http://vdq.quarkkingdee.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://knz.hnqzz.top

[U64] PHP：目录遍历
来源：http://vyw.hcnkem.com

glob("dir/*.php");  scandir("dir");
来源：http://wwh.jinqigfzy.top

[U65] PHP：会话
来源：http://peo.jqgfzy.top

session_start();  $_SESSION["uid"] = 1;
来源：http://qmy.andypj.xyz

[U66] PHP：设置 Cookie
来源：http://zsa.jianghu66.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://ldt.shzxlz.cn

[U67] PHP：处理文件上传
来源：http://wli.meibo888.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://kqc.ywan-chungtsiang.top

[U68] PHP：PDO 连接
来源：http://lye.ybcxt.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://bej.hywenlv.cn

[U69] PHP：PDO 预处理
来源：http://mjv.shangyingyoupin.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hev.jinghuilouyu.cn

[U70] PHP：PDO 事务
来源：http://kec.jqgufenzy.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://hbm.zhaomingkeji.xyz

[U71] PHP：抛出异常
来源：http://stl.sysykeji.top

throw new RuntimeException("失败", 500);
来源：http://giz.zhongyouzk.top

[U72] PHP：写错误日志
来源：http://nqx.jyoumei.cn

error_log("失败: " . $e->getMessage());
来源：http://wvj.hysaishi.cn

[U73] PHP：读取 ini 配置
来源：http://glw.yj202588.top

parse_ini_file("config.ini", true)
来源：http://qdj.nanxinkj.top

[U74] PHP：读取环境变量
来源：http://vod.epnwcf.com

getenv("APP_ENV") ?: "production"
来源：http://zps.shzxlz.cn

[U75] PHP：依赖注入
来源：http://vwt.hesvh.cn

composer require psr/container
来源：http://vvq.snrcjt.cn

[U76] PHP：简单路由
来源：http://vxo.hesvh.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://grm.nanxinkj.top

[U77] PHP：模板渲染
来源：http://gcc.hnxiangtu.top

composer require twig/twig
来源：http://gyf.pycfn.com

[U78] PHP：单元测试
来源：http://ihc.andypj.xyz

composer require --dev phpunit/phpunit
来源：http://hpe.nanxinkj.top

[U79] PHP：静态分析
来源：http://vwh.pengpengdd.cyou

composer require --dev phpstan/phpstan
来源：http://lrj.ywan-chungtsiang.top

[U80] PHP：代码规范修复
来源：http://kgg.gaohongyu789.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://gon.hammf.cn

[U81] JS：初始化项目
来源：http://btj.iojbl.cn

npm init -y;  npm i express
来源：http://kit.cashguo.top

[U82] JS：package.json 脚本
来源：http://lbi.fanxiaobao.xyz

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://ewa.gotoacloud.top

[U83] JS：ES Module 导入导出
来源：http://tlg.shanyushiyangkeji.top

export const a = 1;  import { a } from "./m.js";
来源：http://bxa.havefunace.top

[U84] JS：CommonJS 写法
来源：http://nuc.ehwqpu.com

module.exports = { a };  const { a } = require("./m");
来源：http://fss.svipenyu.cn

[U85] JS：可选链
来源：http://onp.yueranfly.top

a?.b?.c
来源：http://pec.pengpengdd.cyou

[U86] JS：空值合并
来源：http://vty.ydjk.org.cn

a ?? b
来源：http://kqk.fehbvm.com

[U87] JS：解构默认值
来源：http://avx.jianghu66.top

const { a = 1, b = 2 } = obj;
来源：http://hmm.uphjek.com

[U88] JS：对象展开合并
来源：http://iup.daria6918.cn

{ ...a, ...b }
来源：http://hwo.aizwys.cn

[U89] JS：数组去重
来源：http://eug.tanke756.top

[...new Set(arr)]
来源：http://cvk.sxryk.cn

[U90] JS：数字数组排序
来源：http://obv.xuanzx.com

[...arr].sort((a, b) => a - b)
来源：http://ovm.hesvh.cn

[U91] JS：对象键值遍历
来源：http://rvt.jinghuilouyu.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://dtr.havefunace.top

[U92] JS：深拷贝
来源：http://dit.zdbjq.cn

structuredClone(obj)
来源：http://ext.hysaishi.cn

[U93] JS：模板字符串
来源：http://pzs.yueranfly.top

`共 ${n} 条`
来源：http://rwa.jinyuanbaomall.cn

[U94] JS：箭头函数
来源：http://wtu.jinqigufen.top

const double = x => x * 2;
来源：http://irz.zhongyouzk.top

[U95] JS：Promise 包装
来源：http://pif.hammf.cn

new Promise((resolve, reject) => {})
来源：http://szz.yj20258888.top

[U96] JS：async/await 与异常
来源：http://gsf.zhiwuduotai.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://lnh.tian-w.cn

[U97] JS：并发请求
来源：http://gsn.jyoumei.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://bys.fktsv.cn

[U98] JS：fetch 带 JSON
来源：http://wrh.xuanzx.com

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://qje.tianlin.xyz

[U99] JS：事件监听
来源：http://vyq.zhaomingkeji.xyz

el.addEventListener("click", e => {})
来源：http://doe.hesvh.cn

[U100] JS：DOM 查询
来源：http://jgc.nwbrower.top

document.querySelector(".item")
来源：http://zhf.guannengcc.top

[U101] JS：classList 操作
来源：http://cvd.zdqjudy.top

el.classList.toggle("active")
来源：http://ttd.zhiwuduotai.top

[U102] JS：本地存储
来源：http://pfq.meibo888.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://kky.aibaodan.cn

[U103] JS：定时器
来源：http://leu.havefunace.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://clu.cheryme.top

[U104] JS：防抖
来源：http://ijr.chenlongwang.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://aod.mhx1999.top

[U105] JS：节流
来源：http://pdm.pengpengdd.cyou

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://una.yangfankeji.com

[U106] JS：日期格式化
来源：http://ntt.fanxiaobao.xyz

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://gie.jyoumei.cn

[U107] JS：数字千分位
来源：http://yjw.svipenyu.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://swj.hywenlv.cn

[U108] JS：随机整数
来源：http://kka.ehwqpu.com

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://eaz.tian-w.cn

[U109] JS：数组分组
来源：http://oxf.vehdjk.com

Object.groupBy(arr, x => x.type)
来源：http://sda.zhijiandao.cn

[U110] JS：数组分块
来源：http://szb.smart0.xyz

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://yob.jinqigfzy.top

[U111] JS：对象转 Map
来源：http://gox.dianchejie.cn

new Map(Object.entries(obj))
来源：http://nfh.hysaishi.cn

[U112] JS：字符串补位
来源：http://mva.yj20258.top

"7".padStart(3, "0")
来源：http://gvj.zhoulong.xyz

[U113] JS：正则替换全部
来源：http://lic.mhx1999.top

s.replaceAll("a", "b")
来源：http://rai.bbcook.cn

[U114] JS：JSON 深比较
来源：http://mnp.jiagoushi.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://pub.hongshengwenyu.top

[U115] JS：生成 UUID
来源：http://jmc.pycfn.com

crypto.randomUUID()
来源：http://eul.uphjek.com

[U116] JS：类型检查（JSDoc）
来源：http://zga.wangdashe.top

/** @param {string} name */ function f(name) {}
来源：http://znd.iojbl.cn

[U117] JS：单元测试
来源：http://nxc.cqqwz.cn

npm i -D vitest;  npx vitest
来源：http://bdz.zhongyouzk.top

[U118] JS：开发服务器
来源：http://fhr.quarkkingdee.top

npm i -D vite;  npx vite
来源：http://jhw.gaohongyu789.top

[U119] JS：生产构建
来源：http://xxy.aibaodan.cn

npx vite build
来源：http://veq.xuanzx.com

[U120] JS：读取环境变量（Vite）
来源：http://wwq.shangyingyoupin.top

import.meta.env.VITE_API_URL
来源：http://pgi.jinqigfzy.top


<!-- 参考信息 -->