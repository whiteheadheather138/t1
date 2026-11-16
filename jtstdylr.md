代发 wailian999

[T39] Lua：模式匹配
来源：http://jlv.jlsjyb.cn

string.find(s, "%d+")
来源：http://loa.shangyingyoupin.top

[T40] Lua：元表
来源：http://afw.dianchejie.cn

setmetatable({}, { __index = base })
来源：http://hgp.0kj1m.cn

[T41] Perl：Hello World
来源：http://sak.yangfankeji.com

print "Hello\n";
来源：http://buh.mhx1999.top

[T42] Perl：变量类型
来源：http://ixx.tian-w.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://ywp.yuanzhike.top

[T43] Perl：字符串插值
来源：http://swe.yj20258.top

"值: $a"
来源：http://rfo.hfpthk.cn

[T44] Perl：条件
来源：http://idk.zhixingplan.top

if ($a > 0) { print "正"; }
来源：http://mnw.ydjk.org.cn

[T45] Perl：数组遍历
来源：http://pyd.jqgufenzy.top

for my $x (@arr) { print $x; }
来源：http://fcl.hywenlv.cn

[T46] Perl：哈希操作
来源：http://omc.andypj.xyz

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://siz.jinyuanbaomall.cn

[T47] Perl：正则捕获
来源：http://goo.cqqwz.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://pzw.wangdashe.top

[T48] Perl：正则替换
来源：http://shc.yuanzhike.top

$s =~ s/old/new/g;
来源：http://mzw.chenzaomai.com

[T49] Perl：函数
来源：http://xhc.bjfxy.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://xzo.mhx1999.top

[T50] Perl：逐行读文件
来源：http://wnd.sjlbkw.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://nsy.gzhubu.top

while (my $line = <$fh>) { print $line; }
来源：http://gbp.sxryk.cn

[T51] Scala：Hello World
来源：http://gmy.ywan-chungtsiang.top

println("Hello")
来源：http://nln.daxiang520.top

[T52] Scala：变量
来源：http://ynd.guowangkeji.top

val a = 1;  var b = 2
来源：http://mxm.guannengcc.top

[T53] Scala：字符串插值
来源：http://bsi.zdqjudy.top

s"值: $b"
来源：http://gja.hysaishi.cn

[T54] Scala：集合映射
来源：http://zax.fzhhl.top

List(1, 2, 3).map(_ * 2)
来源：http://qii.ywan-chungtsiang.top

[T55] Scala：集合过滤
来源：http://awl.ehwqpu.com

List(1, 2, 3).filter(_ > 1)
来源：http://tog.zhoulong.xyz

[T56] Scala：样例类
来源：http://vel.zdbjq.cn

case class User(name: String, age: Int)
来源：http://fmm.yuxming.cn

[T57] Scala：模式匹配
来源：http://fkq.ctjpmb.com

x match { case 1 => "一"; case _ => "其他" }
来源：http://uoq.wangshuangyany.cn

[T58] Scala：函数定义
来源：http://fru.jinqigfzy.top

def add(a: Int, b: Int): Int = a + b
来源：http://vfk.zycfv.cn

[T59] Scala：循环
来源：http://cko.ivvv.top

for (i <- 1 to 10) println(i)
来源：http://jdc.pycfn.com

[T60] Scala：折叠
来源：http://ojx.ywan-chungtsiang.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://mrc.tarul.cn

================================================================================
来源：http://rlv.zhiwuduotai.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://rqn.quarkkingdee.top

================================================================================
来源：http://zlc.yanxiufei.cn

[U01] Py：创建虚拟环境
来源：http://skc.daria6918.cn

python -m venv .venv && source .venv/bin/activate
来源：http://waq.haohaochexian.top

[U02] Py：导出 / 安装依赖
来源：http://fyc.zhaomingkeji.xyz

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://sdt.ydzc1.top

[U03] Py：加载 .env 配置
来源：http://ijk.jiagoushi.top

from dotenv import load_dotenv; load_dotenv()
来源：http://fcc.hfpthk.cn

[U04] Py：变量调试打印
来源：http://krx.jqgufenzy.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://lam.yuxming.cn

[U05] Py：列表去重且保序
来源：http://hvs.smart0.xyz

list(dict.fromkeys(arr))
来源：http://uxo.kuanghao11.cn

[U06] Py：合并两个字典
来源：http://dgh.daxiang520.top

{**a, **b}
来源：http://qmg.hnqzz.top

[U07] Py：反转字典键值
来源：http://vmq.cqqwz.cn

{v: k for k, v in d.items()}
来源：http://isn.zhongyouzk.top

[U08] Py：展平二维列表
来源：http://vgb.ybcxt.top

[y for x in nested for y in x]
来源：http://mzz.aizwys.cn

[U09] Py：字典取最大值的键
来源：http://tke.ybcxt.top

max(d, key=d.get)
来源：http://jbv.jqgufenzy.top

[U10] Py：按值排序字典
来源：http://eef.redwolf501.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://fqu.yj20258888.top

[U11] Py：生成器表达式
来源：http://nvl.jinyuanbaomall.cn

(x * 2 for x in arr)
来源：http://seb.sufxvd.cn

[U12] Py：取出现最多的 3 个元素
来源：http://esf.cqqwz.cn

Counter(arr).most_common(3)
来源：http://cja.shanyushiyangtech.top

[U13] Py：固定长度队列
来源：http://ohf.yuxming.cn

deque(maxlen=10)
来源：http://tdm.xziqi.cn

[U14] Py：分组收集到列表
来源：http://umq.yonumen.top

defaultdict(list)
来源：http://twx.zhijiandao.cn

[U15] Py：高精度计时
来源：http://wto.aizwys.cn

t = time.perf_counter()
来源：http://dbh.jinyuanbaomall.cn

[U16] Py：命令行参数解析
来源：http://xjx.0kj1m.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://sti.xylfe.cn

[U17] Py：初始化日志
来源：http://huy.hcnkem.com

logging.basicConfig(level=logging.INFO)
来源：http://peh.guowangkeji.top

[U18] Py：预编译正则
来源：http://nfs.bbcook.cn

pat = re.compile(r"\d+")
来源：http://own.xuetiantiany.cn

[U19] Py：正则替换带回调
来源：http://uav.xuanzx.com

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://ivr.yonumen.top

[U20] Py：缓存函数结果
来源：http://sfl.daria6918.cn

@functools.lru_cache(maxsize=None)
来源：http://jay.jyoumei.cn

[U21] Py：自定义上下文管理器
来源：http://vbr.jianghu66.top

@contextlib.contextmanager
来源：http://run.tian-w.cn

[U22] Py：矩阵转置
来源：http://sps.havefunace.top

list(zip(*m))
来源：http://ien.zhongyouzk.top

[U23] Py：分块读取大文件
来源：http://tdg.jinqigufen.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://nwv.shanyushiyangkeji.top

[U24] Py：路径操作
来源：http://dxs.jinyuanbaomall.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://dri.gotoacloud.top

[U25] Py：CSV 按字典读
来源：http://hbq.nanxinkj.top

csv.DictReader(f)
来源：http://xmv.fengsongda.top

[U26] Py：并发下载
来源：http://rbj.ehwqpu.com

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://pfi.chenlongwang.top

[U27] Py：异步 HTTP
来源：http://amf.zdqjudy.top

aiohttp.ClientSession() 配合 async with
来源：http://lbh.gaohongyu789.top

[U28] Py：类型别名
来源：http://naf.zdqjudy.top

UserId = int
来源：http://wds.yj20258888.top

[U29] Py：属性校验
来源：http://bon.chenzaomai.com

@property 与 @x.setter 配合
来源：http://acv.hammf.cn

[U30] Py：数据类
来源：http://cyf.redwolf501.top

@dataclass(slots=True)
来源：http://bak.shanyushiyangtech.top

[U31] Py：单测
来源：http://xfj.guowangkeji.top

python -m pytest -q
来源：http://eix.wangdashe.top

[U32] Py：代码格式化
来源：http://rde.birdmap.top

ruff format . && ruff check --fix .
来源：http://khs.hywenlv.cn

[U33] Py：打包发布
来源：http://php.ctjpmb.com

python -m build  （依赖 pyproject.toml）
来源：http://jxm.yj202588.top

[U34] Py：判断编码
来源：http://idk.hfpthk.cn

chardet.detect(raw)
来源：http://qsi.uphjek.com

[U35] Py：发送邮件
来源：http://wkf.cqqwz.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://udw.zycfv.cn

[U36] Py：定时任务
来源：http://jei.smart0.xyz

schedule.every(10).minutes.do(job)
来源：http://oxs.smart0.xyz

[U37] Py：读写 Excel
来源：http://ock.ppjwa.cn

pandas.read_excel / DataFrame.to_excel
来源：http://vvj.meibo888.top

[U38] Py：获取脚本所在目录
来源：http://nbc.wangdashe.top

Path(__file__).resolve().parent
来源：http://zjc.gaohongyu789.top

[U39] Py：判断是否在交互环境
来源：http://jbs.gzhubu.top

sys.stdout.isatty()
来源：http://flq.guannengcc.top

[U40] Py：打印到标准错误
来源：http://jal.shuidangran.top

print("err", file=sys.stderr)
来源：http://eaj.shanyushiyangkeji.top

[U41] PHP：初始化 Composer 项目
来源：http://nof.feifeiyinyue.top

composer init;  composer require guzzlehttp/guzzle
来源：http://jmd.ywan-chungtsiang.top

[U42] PHP：PSR-4 自动加载
来源：http://amb.jinqigfzy.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://ftf.yvedp.cn

[U43] PHP：声明命名空间
来源：http://dcq.gaohongyu789.top

namespace App\Http;
来源：http://fxd.zhaomingkeji.xyz

[U44] PHP：开启严格类型
来源：http://pvc.hnxiangtu.top

declare(strict_types=1);
来源：http://qys.uphjek.com

[U45] PHP：类型声明与返回类型
来源：http://hoy.sufxvd.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://mxf.pycfn.com

[U46] PHP：可空类型
来源：http://ufv.9152youxi.cn

?string $name = null
来源：http://gdr.cdnleiting.top

[U47] PHP：联合类型
来源：http://qxt.ppjwa.cn

int|string $id
来源：http://plo.quarkkingdee.top

[U48] PHP：纯枚举
来源：http://abo.jiagoushi.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hju.hfpthk.cn

[U49] PHP：只读属性
来源：http://tus.zycfv.cn

public readonly string $name
来源：http://ibg.daria6918.cn

[U50] PHP：构造器属性提升
来源：http://fvt.shuidangran.top

public function __construct(private int $id) {}
来源：http://cse.yj20258888.top

[U51] PHP：数组解构
来源：http://ytq.fktsv.cn

[$a, $b] = $arr;
来源：http://xrz.jqgufenzy.top

[U52] PHP：箭头函数
来源：http://wdq.316326.xyz

$double = fn($x) => $x * 2;
来源：http://qgw.vehdjk.com

[U53] PHP：空合并运算符
来源：http://ttw.shanyushiyangtech.top

$v = $a ?? $b ?? "default";
来源：http://wki.ehwqpu.com

[U54] PHP：空安全调用
来源：http://ctc.hfpthk.cn

$obj?->method()
来源：http://ilg.zycfv.cn

[U55] PHP：match 表达式
来源：http://xml.meibo888.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://mem.bbcook.cn

[U56] PHP：命名参数
来源：http://yvv.gotoacloud.top

f(a: 1, b: 2)
来源：http://trf.shuidangran.top

[U57] PHP：字符串插值
来源：http://nwp.jyoumei.cn

"值: {$a}"
来源：http://ggp.feifeiyinyue.top

[U58] PHP：数组三件套
来源：http://lks.hywenlv.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://qtq.yongpay.top

[U59] PHP：自定义排序
来源：http://yrf.jinqigufen.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://phl.fktsv.cn

[U60] PHP：JSON 编解码
来源：http://bcy.quarkkingdee.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://ixm.pycfn.com

[U61] PHP：正则
来源：http://ibv.zdqjudy.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://osw.svipenyu.cn

[U62] PHP：日期对象
来源：http://qoe.dianchejie.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://fjj.dashuyun.cn

[U63] PHP：文件读写
来源：http://ryu.shanyushiyangkeji.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://rsk.epnwcf.com

[U64] PHP：目录遍历
来源：http://ttd.xuetiantiany.cn

glob("dir/*.php");  scandir("dir");
来源：http://aoj.yanxiufei.cn

[U65] PHP：会话
来源：http://rgm.jiagoushi.top

session_start();  $_SESSION["uid"] = 1;
来源：http://hey.zdbjq.cn

[U66] PHP：设置 Cookie
来源：http://gnu.hnqzz.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://hsm.shanyushiyangkeji.top

[U67] PHP：处理文件上传
来源：http://fpv.daria6918.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://pot.ydzc1.top

[U68] PHP：PDO 连接
来源：http://qtn.yonumen.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://bvd.ybcxt.top

[U69] PHP：PDO 预处理
来源：http://tew.nanxinkj.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://zpy.hnxiangtu.top

[U70] PHP：PDO 事务
来源：http://ysi.yj20258.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://dhg.yueranfly.top

[U71] PHP：抛出异常
来源：http://jep.ydzc1.top

throw new RuntimeException("失败", 500);
来源：http://clg.yvedp.cn

[U72] PHP：写错误日志
来源：http://nbs.daxiang520.top

error_log("失败: " . $e->getMessage());
来源：http://net.sysykeji.top

[U73] PHP：读取 ini 配置
来源：http://njs.fktsv.cn

parse_ini_file("config.ini", true)
来源：http://paa.fktsv.cn

[U74] PHP：读取环境变量
来源：http://aag.cucudq.cn

getenv("APP_ENV") ?: "production"
来源：http://rue.zhengqikj.top

[U75] PHP：依赖注入
来源：http://nzu.jinqigfzy.top

composer require psr/container
来源：http://sws.sjlbkw.cn

[U76] PHP：简单路由
来源：http://xsc.gzhubu.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://xyt.ybcxt.top

[U77] PHP：模板渲染
来源：http://zal.hammf.cn

composer require twig/twig
来源：http://wma.jinyuanbaomall.cn

[U78] PHP：单元测试
来源：http://zgn.yj202588.top

composer require --dev phpunit/phpunit
来源：http://guv.yangfankeji.com

[U79] PHP：静态分析
来源：http://iji.hongshengwenyu.top

composer require --dev phpstan/phpstan
来源：http://guk.hywenlv.cn

[U80] PHP：代码规范修复
来源：http://ayo.9152youxi.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://dnm.shanyushiyangtech.top

[U81] JS：初始化项目
来源：http://hal.kuanghao11.cn

npm init -y;  npm i express
来源：http://sgg.xuetiantiany.cn

[U82] JS：package.json 脚本
来源：http://dix.yj202588.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://exm.shzxlz.cn

[U83] JS：ES Module 导入导出
来源：http://tcm.gotoacloud.top

export const a = 1;  import { a } from "./m.js";
来源：http://zkl.vehdjk.com

[U84] JS：CommonJS 写法
来源：http://nvy.yvedp.cn

module.exports = { a };  const { a } = require("./m");
来源：http://ebq.kuanghao11.cn

[U85] JS：可选链
来源：http://jqb.havefunace.top

a?.b?.c
来源：http://huf.zhijiandao.cn

[U86] JS：空值合并
来源：http://ufn.hammf.cn

a ?? b
来源：http://pul.0kj1m.cn

[U87] JS：解构默认值
来源：http://czy.ybcxt.top

const { a = 1, b = 2 } = obj;
来源：http://wod.jianghu66.top

[U88] JS：对象展开合并
来源：http://zwh.xylfe.cn

{ ...a, ...b }
来源：http://wnz.jiagoushi.top

[U89] JS：数组去重
来源：http://rlx.zdbjq.cn

[...new Set(arr)]
来源：http://kzo.nwbrower.top

[U90] JS：数字数组排序
来源：http://wec.nwbrower.top

[...arr].sort((a, b) => a - b)
来源：http://hdb.hnxiangtu.top

[U91] JS：对象键值遍历
来源：http://gll.yj202588.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://rjd.jqgufenzy.top

[U92] JS：深拷贝
来源：http://goe.fktsv.cn

structuredClone(obj)
来源：http://soj.shanyushiyangkeji.top

[U93] JS：模板字符串
来源：http://bsx.redwolf501.top

`共 ${n} 条`
来源：http://kxz.yongpay.top

[U94] JS：箭头函数
来源：http://pvh.tian-w.cn

const double = x => x * 2;
来源：http://uya.svipenyu.cn

[U95] JS：Promise 包装
来源：http://lir.guowangkeji.top

new Promise((resolve, reject) => {})
来源：http://kcf.shangyingyoupin.top

[U96] JS：async/await 与异常
来源：http://cij.aibaodan.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://rko.havefunace.top

[U97] JS：并发请求
来源：http://ham.zhiwuduotai.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://yaf.yueranfly.top

[U98] JS：fetch 带 JSON
来源：http://mwx.jianghu66.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://pax.xylfe.cn

[U99] JS：事件监听
来源：http://pmh.316326.xyz

el.addEventListener("click", e => {})
来源：http://umj.jinqigufen.top

[U100] JS：DOM 查询
来源：http://iry.ydzc1.top

document.querySelector(".item")
来源：http://ghy.cdnleiting.top

[U101] JS：classList 操作
来源：http://knv.yj20258.top

el.classList.toggle("active")
来源：http://fyk.jinqigfzy.top

[U102] JS：本地存储
来源：http://qph.zhijiandao.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://xry.yuxming.cn

[U103] JS：定时器
来源：http://mtk.chenjidiqi.icu

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://fql.hammf.cn

[U104] JS：防抖
来源：http://uow.zycfv.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ddz.yj20258888.top

[U105] JS：节流
来源：http://etp.xinyue.icu

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://qfx.gogol.net.cn

[U106] JS：日期格式化
来源：http://wqh.zhongyouzk.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://teo.wangshuangyany.cn

[U107] JS：数字千分位
来源：http://cio.zhoulong.xyz

new Intl.NumberFormat("en-US").format(1234567)
来源：http://vlm.ybcxt.top

[U108] JS：随机整数
来源：http://rav.quarkkingdee.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://wjm.jinqigufen.top

[U109] JS：数组分组
来源：http://tdu.cheryme.top

Object.groupBy(arr, x => x.type)
来源：http://phw.mhx1999.top

[U110] JS：数组分块
来源：http://zwc.hfpthk.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://pae.cashguo.top

[U111] JS：对象转 Map
来源：http://eti.zhixingplan.top

new Map(Object.entries(obj))
来源：http://bbt.epnwcf.com

[U112] JS：字符串补位
来源：http://xdj.nwbrower.top

"7".padStart(3, "0")
来源：http://lwy.tian-w.cn

[U113] JS：正则替换全部
来源：http://cxa.tanke756.top

s.replaceAll("a", "b")
来源：http://cfg.xinyue.icu

[U114] JS：JSON 深比较
来源：http://thq.0kj1m.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://uon.yuxming.cn

[U115] JS：生成 UUID
来源：http://vud.yfazqb.com

crypto.randomUUID()
来源：http://tzh.zycfv.cn

[U116] JS：类型检查（JSDoc）
来源：http://ptr.sysykeji.top

/** @param {string} name */ function f(name) {}
来源：http://pmd.cheryme.top

[U117] JS：单元测试
来源：http://jcp.xinyue.icu

npm i -D vitest;  npx vitest
来源：http://znr.sjlbkw.cn

[U118] JS：开发服务器
来源：http://yus.feifeiyinyue.top

npm i -D vite;  npx vite
来源：http://pof.sufxvd.cn

[U119] JS：生产构建
来源：http://oos.yonumen.top

npx vite build
来源：http://sfs.ywan-chungtsiang.top

[U120] JS：读取环境变量（Vite）
来源：http://ikr.zycfv.cn

import.meta.env.VITE_API_URL
来源：http://ics.sjlbkw.cn

================================================================================
来源：http://egz.cheryme.top

统计汇总
来源：http://lzs.xuanzx.com

================================================================================
来源：http://izq.vehdjk.com

按语言统计（条）：
来源：http://txp.chenzaomai.com

Python ......... 252
来源：http://dwe.quarkkingdee.top

PHP ............ 252
来源：http://mbt.xylfe.cn

JavaScript ..... 252
来源：http://fry.yj20258888.top

TypeScript ..... 212
来源：http://fhb.hnxiangtu.top

Java ........... 212
来源：http://vfr.xingfuxueyuan.xyz

Go ............. 212
来源：http://ret.zhixingplan.top

Ruby ........... 212
来源：http://ltm.fzhhl.top

C# ............. 212
来源：http://hmc.guowangkeji.top


<!-- 参考信息 -->