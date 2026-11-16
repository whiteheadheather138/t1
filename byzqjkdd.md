代发 wailian999

[T31] Lua：Hello World
来源：http://ogb.tian-w.cn

print("Hello")
来源：http://iuo.xuanzx.com

[T32] Lua：局部变量
来源：http://udz.hongshengwenyu.top

local a = 1
来源：http://wgh.zdqjudy.top

[T33] Lua：表（数组）
来源：http://sgh.gaohongyu789.top

local t = {1, 2, 3};  t[4] = 4
来源：http://suz.sjlbkw.cn

[T34] Lua：遍历表
来源：http://spx.jlsjyb.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://hpz.fengsongda.top

[T35] Lua：字典表
来源：http://lak.cheryme.top

local d = { a = 1 };  d.b = 2
来源：http://uko.zhaomingkeji.xyz

[T36] Lua：函数
来源：http://xvz.shanyushiyangtech.top

function add(a, b) return a + b end
来源：http://ssc.fktsv.cn

[T37] Lua：字符串拼接
来源：http://nne.zhoulong.xyz

"a" .. "b"
来源：http://dxu.xingfuxueyuan.xyz

[T38] Lua：条件
来源：http://emw.xinyue.icu

if x > 0 then print("正") end
来源：http://oat.shzxlz.cn

[T39] Lua：模式匹配
来源：http://fhb.mhx1999.top

string.find(s, "%d+")
来源：http://xsu.c1oappe.top

[T40] Lua：元表
来源：http://wox.fehbvm.com

setmetatable({}, { __index = base })
来源：http://deh.xuanzx.com

[T41] Perl：Hello World
来源：http://hks.haohaochexian.top

print "Hello\n";
来源：http://kfm.fanxiaobao.xyz

[T42] Perl：变量类型
来源：http://aud.zdqjudy.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://nhc.aibaodan.cn

[T43] Perl：字符串插值
来源：http://zoz.zdqjudy.top

"值: $a"
来源：http://dai.zhaomingkeji.xyz

[T44] Perl：条件
来源：http://vvh.tanke756.top

if ($a > 0) { print "正"; }
来源：http://stj.tian-w.cn

[T45] Perl：数组遍历
来源：http://ynb.iojbl.cn

for my $x (@arr) { print $x; }
来源：http://hne.shzxlz.cn

[T46] Perl：哈希操作
来源：http://hby.zhaomingkeji.xyz

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://tff.tarul.cn

[T47] Perl：正则捕获
来源：http://mfb.shanyushiyangkeji.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://hlw.sweek.top

[T48] Perl：正则替换
来源：http://xbq.cdnleiting.top

$s =~ s/old/new/g;
来源：http://fnr.daria6918.cn

[T49] Perl：函数
来源：http://egp.shzxlz.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://sqe.hongshengwenyu.top

[T50] Perl：逐行读文件
来源：http://ftf.quarkkingdee.top

open my $fh, "<", "a.txt" or die $!;
来源：http://nwf.yongpay.top

while (my $line = <$fh>) { print $line; }
来源：http://lmz.cucudq.cn

[T51] Scala：Hello World
来源：http://qut.gaohongyu789.top

println("Hello")
来源：http://yds.hnqzz.top

[T52] Scala：变量
来源：http://bdk.zdqjudy.top

val a = 1;  var b = 2
来源：http://zan.316326.xyz

[T53] Scala：字符串插值
来源：http://bvu.tian-w.cn

s"值: $b"
来源：http://ksc.jinqigufen.top

[T54] Scala：集合映射
来源：http://yoe.cqqwz.cn

List(1, 2, 3).map(_ * 2)
来源：http://rfb.ydzc1.top

[T55] Scala：集合过滤
来源：http://gdu.jiagoushi.top

List(1, 2, 3).filter(_ > 1)
来源：http://fhx.hysaishi.cn

[T56] Scala：样例类
来源：http://tte.zhixingplan.top

case class User(name: String, age: Int)
来源：http://lxd.xziqi.cn

[T57] Scala：模式匹配
来源：http://xzb.tian-w.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://tkg.shuidangran.top

[T58] Scala：函数定义
来源：http://ijz.cashguo.top

def add(a: Int, b: Int): Int = a + b
来源：http://yxc.ywan-chungtsiang.top

[T59] Scala：循环
来源：http://cfo.shanyushiyangtech.top

for (i <- 1 to 10) println(i)
来源：http://rzy.fanxiaobao.xyz

[T60] Scala：折叠
来源：http://lev.mhx1999.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://euk.zhengqikj.top

================================================================================
来源：http://gki.yj20258.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://ipo.ctjpmb.com

================================================================================
来源：http://wxk.xuetiantiany.cn

[U01] Py：创建虚拟环境
来源：http://srx.fzhhl.top

python -m venv .venv && source .venv/bin/activate
来源：http://wvn.zdqjudy.top

[U02] Py：导出 / 安装依赖
来源：http://dyz.nwbrower.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://vzl.yj20258.top

[U03] Py：加载 .env 配置
来源：http://qzo.ctjpmb.com

from dotenv import load_dotenv; load_dotenv()
来源：http://phy.gaohongyu789.top

[U04] Py：变量调试打印
来源：http://fpy.yj202588.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hmi.cheryme.top

[U05] Py：列表去重且保序
来源：http://dmt.pycfn.com

list(dict.fromkeys(arr))
来源：http://xfl.hywenlv.cn

[U06] Py：合并两个字典
来源：http://zeg.cqqwz.cn

{**a, **b}
来源：http://rfh.pycfn.com

[U07] Py：反转字典键值
来源：http://vbz.yj20258.top

{v: k for k, v in d.items()}
来源：http://ikf.316326.xyz

[U08] Py：展平二维列表
来源：http://kso.tarul.cn

[y for x in nested for y in x]
来源：http://ygj.c1oappe.top

[U09] Py：字典取最大值的键
来源：http://vtt.jyoumei.cn

max(d, key=d.get)
来源：http://sgy.andypj.xyz

[U10] Py：按值排序字典
来源：http://ahn.yfazqb.com

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://zzo.fzhhl.top

[U11] Py：生成器表达式
来源：http://dpx.jinqigfzy.top

(x * 2 for x in arr)
来源：http://byl.fehbvm.com

[U12] Py：取出现最多的 3 个元素
来源：http://mko.epnwcf.com

Counter(arr).most_common(3)
来源：http://hdd.guowangkeji.top

[U13] Py：固定长度队列
来源：http://exe.zdqjudy.top

deque(maxlen=10)
来源：http://uzq.meibo888.top

[U14] Py：分组收集到列表
来源：http://rwr.cdnleiting.top

defaultdict(list)
来源：http://mxt.ybcxt.top

[U15] Py：高精度计时
来源：http://ckd.mhx1999.top

t = time.perf_counter()
来源：http://hbc.xuetiantiany.cn

[U16] Py：命令行参数解析
来源：http://czb.tian-w.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://saq.guowangkeji.top

[U17] Py：初始化日志
来源：http://qnp.sjlbkw.cn

logging.basicConfig(level=logging.INFO)
来源：http://utz.xuanzx.com

[U18] Py：预编译正则
来源：http://zdr.snrcjt.cn

pat = re.compile(r"\d+")
来源：http://knk.zhengqikj.top

[U19] Py：正则替换带回调
来源：http://wom.sysykeji.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://upc.ydzc1.top

[U20] Py：缓存函数结果
来源：http://llq.jinyuanbaomall.cn

@functools.lru_cache(maxsize=None)
来源：http://oea.feifeiyinyue.top

[U21] Py：自定义上下文管理器
来源：http://pfp.hnxiangtu.top

@contextlib.contextmanager
来源：http://fay.ivvv.top

[U22] Py：矩阵转置
来源：http://lpg.dashuyun.cn

list(zip(*m))
来源：http://ssl.yangfankeji.com

[U23] Py：分块读取大文件
来源：http://uzt.tianlin.xyz

for chunk in iter(lambda: f.read(8192), b""):
来源：http://toj.zhongyouzk.top

[U24] Py：路径操作
来源：http://bmx.hfpthk.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://oim.shanyushiyangtech.top

[U25] Py：CSV 按字典读
来源：http://ydp.yj20258.top

csv.DictReader(f)
来源：http://bde.xylfe.cn

[U26] Py：并发下载
来源：http://vph.zhongyouzk.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://par.zhaomingkeji.xyz

[U27] Py：异步 HTTP
来源：http://sis.jlsjyb.cn

aiohttp.ClientSession() 配合 async with
来源：http://jex.guowangkeji.top

[U28] Py：类型别名
来源：http://dvf.hammf.cn

UserId = int
来源：http://jfz.aibaodan.cn

[U29] Py：属性校验
来源：http://ohw.feifeiyinyue.top

@property 与 @x.setter 配合
来源：http://ytv.yongpay.top

[U30] Py：数据类
来源：http://dnm.shuidangran.top

@dataclass(slots=True)
来源：http://cjx.wangdashe.top

[U31] Py：单测
来源：http://fba.snrcjt.cn

python -m pytest -q
来源：http://sin.ydjk.org.cn

[U32] Py：代码格式化
来源：http://nvn.jiagoushi.top

ruff format . && ruff check --fix .
来源：http://bxg.jyoumei.cn

[U33] Py：打包发布
来源：http://pwe.hongshengwenyu.top

python -m build  （依赖 pyproject.toml）
来源：http://ygt.sjlbkw.cn

[U34] Py：判断编码
来源：http://pzz.9152youxi.cn

chardet.detect(raw)
来源：http://rkg.uphjek.com

[U35] Py：发送邮件
来源：http://stt.uphjek.com

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://dze.shuidangran.top

[U36] Py：定时任务
来源：http://bbo.svipenyu.cn

schedule.every(10).minutes.do(job)
来源：http://nal.0kj1m.cn

[U37] Py：读写 Excel
来源：http://oyk.zdqjudy.top

pandas.read_excel / DataFrame.to_excel
来源：http://iuq.jqgufenzy.top

[U38] Py：获取脚本所在目录
来源：http://jqk.daria6918.cn

Path(__file__).resolve().parent
来源：http://oih.shanyushiyangtech.top

[U39] Py：判断是否在交互环境
来源：http://fgs.feifeiyinyue.top

sys.stdout.isatty()
来源：http://zin.cashguo.top

[U40] Py：打印到标准错误
来源：http://bzc.ybcxt.top

print("err", file=sys.stderr)
来源：http://qhv.hnqzz.top

[U41] PHP：初始化 Composer 项目
来源：http://rma.xingfuxueyuan.xyz

composer init;  composer require guzzlehttp/guzzle
来源：http://wrl.cheryme.top

[U42] PHP：PSR-4 自动加载
来源：http://zwa.meibo888.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://pql.cqqwz.cn

[U43] PHP：声明命名空间
来源：http://xfg.zhoulong.xyz

namespace App\Http;
来源：http://hvr.daria6918.cn

[U44] PHP：开启严格类型
来源：http://fpf.cheryme.top

declare(strict_types=1);
来源：http://pkw.tarul.cn

[U45] PHP：类型声明与返回类型
来源：http://rrw.yj20258888.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://unq.meibo888.top

[U46] PHP：可空类型
来源：http://ngk.52xcode.cn

?string $name = null
来源：http://qxe.9152youxi.cn

[U47] PHP：联合类型
来源：http://etn.zdqjudy.top

int|string $id
来源：http://mtb.gzhubu.top

[U48] PHP：纯枚举
来源：http://hyx.hammf.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://fqq.snrcjt.cn

[U49] PHP：只读属性
来源：http://qzm.hnxiangtu.top

public readonly string $name
来源：http://jmx.kuanghao11.cn

[U50] PHP：构造器属性提升
来源：http://xan.zycfv.cn

public function __construct(private int $id) {}
来源：http://qjg.xuanzx.com

[U51] PHP：数组解构
来源：http://bwb.dashuyun.cn

[$a, $b] = $arr;
来源：http://yov.redwolf501.top

[U52] PHP：箭头函数
来源：http://jcy.jlsjyb.cn

$double = fn($x) => $x * 2;
来源：http://map.jqgufenzy.top

[U53] PHP：空合并运算符
来源：http://xtd.haohaochexian.top

$v = $a ?? $b ?? "default";
来源：http://odl.0kj1m.cn

[U54] PHP：空安全调用
来源：http://jzs.yj20258888.top

$obj?->method()
来源：http://gky.ehwqpu.com

[U55] PHP：match 表达式
来源：http://qze.smart0.xyz

$s = match($x) { 1 => "一", default => "其他" };
来源：http://anj.fanxiaobao.xyz

[U56] PHP：命名参数
来源：http://aeg.zhaomingkeji.xyz

f(a: 1, b: 2)
来源：http://xue.yj20258.top

[U57] PHP：字符串插值
来源：http://hxt.iojbl.cn

"值: {$a}"
来源：http://oxc.jqgufenzy.top

[U58] PHP：数组三件套
来源：http://pow.ydjk.org.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://mrb.andypj.xyz

[U59] PHP：自定义排序
来源：http://loe.shanyushiyangtech.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wmy.feifeiyinyue.top

[U60] PHP：JSON 编解码
来源：http://vnk.zdqjudy.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://htq.cucudq.cn

[U61] PHP：正则
来源：http://qyv.zhixingplan.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://cwh.wangdashe.top

[U62] PHP：日期对象
来源：http://mpg.52xcode.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://moh.tanke756.top

[U63] PHP：文件读写
来源：http://znh.iojbl.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://gzw.zycfv.cn

[U64] PHP：目录遍历
来源：http://txa.shuidangran.top

glob("dir/*.php");  scandir("dir");
来源：http://tpv.haohaochexian.top

[U65] PHP：会话
来源：http://mmb.jinqigufen.top

session_start();  $_SESSION["uid"] = 1;
来源：http://xxw.dashuyun.cn

[U66] PHP：设置 Cookie
来源：http://tlp.ydzc1.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://tvo.chenzaomai.com

[U67] PHP：处理文件上传
来源：http://ekq.jqgufenzy.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://uft.jqgfzy.top

[U68] PHP：PDO 连接
来源：http://dkc.yfazqb.com

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://zpl.hywenlv.cn

[U69] PHP：PDO 预处理
来源：http://krg.hammf.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://sqg.sysykeji.top

[U70] PHP：PDO 事务
来源：http://uip.smart0.xyz

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://stq.jinyuanbaomall.cn

[U71] PHP：抛出异常
来源：http://iuh.zhengqikj.top

throw new RuntimeException("失败", 500);
来源：http://icy.shzxlz.cn

[U72] PHP：写错误日志
来源：http://ydm.gotoacloud.top

error_log("失败: " . $e->getMessage());
来源：http://ptj.epnwcf.com

[U73] PHP：读取 ini 配置
来源：http://ypb.wangdashe.top

parse_ini_file("config.ini", true)
来源：http://sul.nanxinkj.top

[U74] PHP：读取环境变量
来源：http://cbq.xuetiantiany.cn

getenv("APP_ENV") ?: "production"
来源：http://xop.guowangkeji.top

[U75] PHP：依赖注入
来源：http://mze.aibaodan.cn

composer require psr/container
来源：http://fgb.gzhubu.top

[U76] PHP：简单路由
来源：http://vdp.jinghuilouyu.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://nhj.andypj.xyz

[U77] PHP：模板渲染
来源：http://njt.birdmap.top

composer require twig/twig
来源：http://hrf.jinqigufen.top

[U78] PHP：单元测试
来源：http://fzx.bjfxy.top

composer require --dev phpunit/phpunit
来源：http://uwb.sxryk.cn

[U79] PHP：静态分析
来源：http://nsx.xuanzx.com

composer require --dev phpstan/phpstan
来源：http://hii.jianghu66.top

[U80] PHP：代码规范修复
来源：http://lec.zdbjq.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://gis.ydjk.org.cn

[U81] JS：初始化项目
来源：http://gex.guannengcc.top

npm init -y;  npm i express
来源：http://suh.pycfn.com

[U82] JS：package.json 脚本
来源：http://oml.52xcode.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://pbq.zhoulong.xyz

[U83] JS：ES Module 导入导出
来源：http://wsa.zhixingplan.top

export const a = 1;  import { a } from "./m.js";
来源：http://cfe.guannengcc.top

[U84] JS：CommonJS 写法
来源：http://qbb.hysaishi.cn

module.exports = { a };  const { a } = require("./m");
来源：http://cup.ybcxt.top

[U85] JS：可选链
来源：http://mgj.yangfankeji.com

a?.b?.c
来源：http://vsr.jlsjyb.cn

[U86] JS：空值合并
来源：http://qmz.jinyuanbaomall.cn

a ?? b
来源：http://mqh.yfazqb.com

[U87] JS：解构默认值
来源：http://vnn.dashuyun.cn

const { a = 1, b = 2 } = obj;
来源：http://kcp.meibo888.top

[U88] JS：对象展开合并
来源：http://mns.sufxvd.cn

{ ...a, ...b }
来源：http://mkn.guowangkeji.top

[U89] JS：数组去重
来源：http://qow.sysykeji.top

[...new Set(arr)]
来源：http://tri.tianlin.xyz

[U90] JS：数字数组排序
来源：http://hrx.gzhubu.top

[...arr].sort((a, b) => a - b)
来源：http://ems.shanyushiyangtech.top

[U91] JS：对象键值遍历
来源：http://eei.sjlbkw.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://kwd.daria6918.cn

[U92] JS：深拷贝
来源：http://vvl.wangdashe.top

structuredClone(obj)
来源：http://pkz.c1oappe.top

[U93] JS：模板字符串
来源：http://wvh.yueranfly.top

`共 ${n} 条`
来源：http://pod.vehdjk.com

[U94] JS：箭头函数
来源：http://wpy.fktsv.cn

const double = x => x * 2;
来源：http://alp.cashguo.top

[U95] JS：Promise 包装
来源：http://ckh.cdnleiting.top

new Promise((resolve, reject) => {})
来源：http://djn.yj20258.top

[U96] JS：async/await 与异常
来源：http://psu.jinqigfzy.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://unn.kuanghao11.cn

[U97] JS：并发请求
来源：http://yob.bbcook.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://mjl.snrcjt.cn

[U98] JS：fetch 带 JSON
来源：http://njo.yuxming.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://avb.xylfe.cn

[U99] JS：事件监听
来源：http://foj.yj20258888.top

el.addEventListener("click", e => {})
来源：http://bef.jinqigfzy.top

[U100] JS：DOM 查询
来源：http://opg.sjlbkw.cn

document.querySelector(".item")
来源：http://bgs.bjfxy.top

[U101] JS：classList 操作
来源：http://rga.havefunace.top

el.classList.toggle("active")
来源：http://hqj.zhixingplan.top

[U102] JS：本地存储
来源：http://etn.shangyingyoupin.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://yaj.zhixingplan.top

[U103] JS：定时器
来源：http://ned.yj202588.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://fwu.cqqwz.cn

[U104] JS：防抖
来源：http://uvc.jyoumei.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mgz.jiagoushi.top

[U105] JS：节流
来源：http://xyi.jqgufenzy.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://xcl.havefunace.top

[U106] JS：日期格式化
来源：http://tki.yuanzhike.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://cek.0kj1m.cn

[U107] JS：数字千分位
来源：http://utq.birdmap.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://jmu.aizwys.cn

[U108] JS：随机整数
来源：http://tpp.hongshengwenyu.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://kku.daria6918.cn

[U109] JS：数组分组
来源：http://fce.jiagoushi.top

Object.groupBy(arr, x => x.type)
来源：http://ivo.fehbvm.com

[U110] JS：数组分块
来源：http://lcj.cheryme.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://eil.svipenyu.cn

[U111] JS：对象转 Map
来源：http://cyo.gotoacloud.top

new Map(Object.entries(obj))
来源：http://nav.sweek.top

[U112] JS：字符串补位
来源：http://vwd.jlsjyb.cn

"7".padStart(3, "0")
来源：http://wwc.vehdjk.com

[U113] JS：正则替换全部
来源：http://wsw.redwolf501.top

s.replaceAll("a", "b")
来源：http://osx.guowangkeji.top

[U114] JS：JSON 深比较
来源：http://hta.tarul.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://mta.smart0.xyz

[U115] JS：生成 UUID
来源：http://crr.0kj1m.cn

crypto.randomUUID()
来源：http://dwx.hywenlv.cn

[U116] JS：类型检查（JSDoc）
来源：http://dwu.ybcxt.top

/** @param {string} name */ function f(name) {}
来源：http://aaa.yj20258.top

[U117] JS：单元测试
来源：http://bdu.jqgfzy.top

npm i -D vitest;  npx vitest
来源：http://zxn.xylfe.cn

[U118] JS：开发服务器
来源：http://cll.nanxinkj.top

npm i -D vite;  npx vite
来源：http://ysz.quarkkingdee.top


<!-- 参考信息 -->