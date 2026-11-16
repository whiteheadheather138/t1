代发 wailian999

[T43] Perl：字符串插值
来源：http://hve.wangshuangyany.cn

"值: $a"
来源：http://mke.zhijiandao.cn

[T44] Perl：条件
来源：http://fsb.fengsongda.top

if ($a > 0) { print "正"; }
来源：http://mgr.hywenlv.cn

[T45] Perl：数组遍历
来源：http://bgu.hfpthk.cn

for my $x (@arr) { print $x; }
来源：http://onm.hysaishi.cn

[T46] Perl：哈希操作
来源：http://oyj.hnxiangtu.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://ktg.pycfn.com

[T47] Perl：正则捕获
来源：http://ovq.kuanghao11.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://oiq.fktsv.cn

[T48] Perl：正则替换
来源：http://jpu.aizwys.cn

$s =~ s/old/new/g;
来源：http://hdd.jqgufenzy.top

[T49] Perl：函数
来源：http://kau.cheryme.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://xds.sjlbkw.cn

[T50] Perl：逐行读文件
来源：http://pyh.c1oappe.top

open my $fh, "<", "a.txt" or die $!;
来源：http://uct.52xcode.cn

while (my $line = <$fh>) { print $line; }
来源：http://hdp.guowangkeji.top

[T51] Scala：Hello World
来源：http://qig.hfpthk.cn

println("Hello")
来源：http://ozu.zhijiandao.cn

[T52] Scala：变量
来源：http://sau.kuanghao11.cn

val a = 1;  var b = 2
来源：http://zfc.sjlbkw.cn

[T53] Scala：字符串插值
来源：http://qsg.vehdjk.com

s"值: $b"
来源：http://hgd.c1oappe.top

[T54] Scala：集合映射
来源：http://jtg.shanyushiyangkeji.top

List(1, 2, 3).map(_ * 2)
来源：http://qso.yvedp.cn

[T55] Scala：集合过滤
来源：http://rcn.yj202588.top

List(1, 2, 3).filter(_ > 1)
来源：http://gbp.ctjpmb.com

[T56] Scala：样例类
来源：http://kwv.jinghuilouyu.cn

case class User(name: String, age: Int)
来源：http://eky.aizwys.cn

[T57] Scala：模式匹配
来源：http://tjc.zhongyouzk.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://bsq.dashuyun.cn

[T58] Scala：函数定义
来源：http://veg.daxiang520.top

def add(a: Int, b: Int): Int = a + b
来源：http://fyy.shuidangran.top

[T59] Scala：循环
来源：http://izx.ppjwa.cn

for (i <- 1 to 10) println(i)
来源：http://kfe.fktsv.cn

[T60] Scala：折叠
来源：http://ics.gotoacloud.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://wro.hongshengwenyu.top

================================================================================
来源：http://xks.hnxiangtu.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://mie.zhixingplan.top

================================================================================
来源：http://cnr.mhx1999.top

[U01] Py：创建虚拟环境
来源：http://apc.ivvv.top

python -m venv .venv && source .venv/bin/activate
来源：http://crp.bjfxy.top

[U02] Py：导出 / 安装依赖
来源：http://vho.fengsongda.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://ois.hesvh.cn

[U03] Py：加载 .env 配置
来源：http://wlh.fengsongda.top

from dotenv import load_dotenv; load_dotenv()
来源：http://bmn.chenlongwang.top

[U04] Py：变量调试打印
来源：http://pqx.yangfankeji.com

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://cny.jlsjyb.cn

[U05] Py：列表去重且保序
来源：http://ddr.zycfv.cn

list(dict.fromkeys(arr))
来源：http://rkr.sjlbkw.cn

[U06] Py：合并两个字典
来源：http://wzz.cheryme.top

{**a, **b}
来源：http://fro.sysykeji.top

[U07] Py：反转字典键值
来源：http://bat.iojbl.cn

{v: k for k, v in d.items()}
来源：http://erk.hysaishi.cn

[U08] Py：展平二维列表
来源：http://lyk.zhaomingkeji.xyz

[y for x in nested for y in x]
来源：http://iif.jiagoushi.top

[U09] Py：字典取最大值的键
来源：http://cpv.vqdsnc.cn

max(d, key=d.get)
来源：http://pnq.bjfxy.top

[U10] Py：按值排序字典
来源：http://mae.xylfe.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://fof.jinyuanbaomall.cn

[U11] Py：生成器表达式
来源：http://fpn.ywan-chungtsiang.top

(x * 2 for x in arr)
来源：http://kbg.yongpay.top

[U12] Py：取出现最多的 3 个元素
来源：http://qbc.jqgufenzy.top

Counter(arr).most_common(3)
来源：http://jqq.sxryk.cn

[U13] Py：固定长度队列
来源：http://zuz.fengsongda.top

deque(maxlen=10)
来源：http://mzg.fzhhl.top

[U14] Py：分组收集到列表
来源：http://kvn.xuetiantiany.cn

defaultdict(list)
来源：http://qod.guannengcc.top

[U15] Py：高精度计时
来源：http://wjv.hongshengwenyu.top

t = time.perf_counter()
来源：http://ltl.9152youxi.cn

[U16] Py：命令行参数解析
来源：http://xqm.shangyingyoupin.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://veq.aibaodan.cn

[U17] Py：初始化日志
来源：http://rwj.ydjk.org.cn

logging.basicConfig(level=logging.INFO)
来源：http://anq.jlsjyb.cn

[U18] Py：预编译正则
来源：http://psp.ywan-chungtsiang.top

pat = re.compile(r"\d+")
来源：http://kwe.shuidangran.top

[U19] Py：正则替换带回调
来源：http://jis.hnqzz.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://eyx.meibo888.top

[U20] Py：缓存函数结果
来源：http://fri.hesvh.cn

@functools.lru_cache(maxsize=None)
来源：http://cgm.cheryme.top

[U21] Py：自定义上下文管理器
来源：http://nzn.sweek.top

@contextlib.contextmanager
来源：http://phb.yueranfly.top

[U22] Py：矩阵转置
来源：http://rqp.xingfuxueyuan.xyz

list(zip(*m))
来源：http://ljh.shanyushiyangkeji.top

[U23] Py：分块读取大文件
来源：http://wxk.hongshengwenyu.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://gxj.ybcxt.top

[U24] Py：路径操作
来源：http://xje.ydzc1.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://raw.chenlongwang.top

[U25] Py：CSV 按字典读
来源：http://pej.ehwqpu.com

csv.DictReader(f)
来源：http://kym.kuanghao11.cn

[U26] Py：并发下载
来源：http://xcx.jyoumei.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://ign.chenzaomai.com

[U27] Py：异步 HTTP
来源：http://wgv.jinyuanbaomall.cn

aiohttp.ClientSession() 配合 async with
来源：http://qby.yuanzhike.top

[U28] Py：类型别名
来源：http://qmj.jqgfzy.top

UserId = int
来源：http://ono.sjlbkw.cn

[U29] Py：属性校验
来源：http://blz.pycfn.com

@property 与 @x.setter 配合
来源：http://byv.shanyushiyangtech.top

[U30] Py：数据类
来源：http://sfe.snrcjt.cn

@dataclass(slots=True)
来源：http://qfx.tarul.cn

[U31] Py：单测
来源：http://bfr.zdqjudy.top

python -m pytest -q
来源：http://ggz.hongshengwenyu.top

[U32] Py：代码格式化
来源：http://mxr.ehwqpu.com

ruff format . && ruff check --fix .
来源：http://pjf.jqgfzy.top

[U33] Py：打包发布
来源：http://ern.ctjpmb.com

python -m build  （依赖 pyproject.toml）
来源：http://uqr.hongshengwenyu.top

[U34] Py：判断编码
来源：http://wnc.birdmap.top

chardet.detect(raw)
来源：http://spb.zhixingplan.top

[U35] Py：发送邮件
来源：http://nvm.fehbvm.com

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://yps.yuanzhike.top

[U36] Py：定时任务
来源：http://xza.sxryk.cn

schedule.every(10).minutes.do(job)
来源：http://dfq.wangdashe.top

[U37] Py：读写 Excel
来源：http://zyi.yueranfly.top

pandas.read_excel / DataFrame.to_excel
来源：http://tkj.0kj1m.cn

[U38] Py：获取脚本所在目录
来源：http://lre.iojbl.cn

Path(__file__).resolve().parent
来源：http://ktx.yanxiufei.cn

[U39] Py：判断是否在交互环境
来源：http://edo.fktsv.cn

sys.stdout.isatty()
来源：http://vvj.hongshengwenyu.top

[U40] Py：打印到标准错误
来源：http://rya.yj202588.top

print("err", file=sys.stderr)
来源：http://hmg.316326.xyz

[U41] PHP：初始化 Composer 项目
来源：http://cst.hcnkem.com

composer init;  composer require guzzlehttp/guzzle
来源：http://ikc.hywenlv.cn

[U42] PHP：PSR-4 自动加载
来源：http://vju.yfazqb.com

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://cll.nanxinkj.top

[U43] PHP：声明命名空间
来源：http://hod.guowangkeji.top

namespace App\Http;
来源：http://qxo.guowangkeji.top

[U44] PHP：开启严格类型
来源：http://hre.wangdashe.top

declare(strict_types=1);
来源：http://swh.fktsv.cn

[U45] PHP：类型声明与返回类型
来源：http://riw.jqgfzy.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://njh.shanyushiyangkeji.top

[U46] PHP：可空类型
来源：http://ull.dianchejie.cn

?string $name = null
来源：http://agm.jinqigfzy.top

[U47] PHP：联合类型
来源：http://thb.guannengcc.top

int|string $id
来源：http://ldy.cashguo.top

[U48] PHP：纯枚举
来源：http://teh.meibo888.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://jtg.quarkkingdee.top

[U49] PHP：只读属性
来源：http://kxb.zdqjudy.top

public readonly string $name
来源：http://bmn.sysykeji.top

[U50] PHP：构造器属性提升
来源：http://jpj.zdbjq.cn

public function __construct(private int $id) {}
来源：http://btg.yueranfly.top

[U51] PHP：数组解构
来源：http://wcl.fengsongda.top

[$a, $b] = $arr;
来源：http://hec.hfpthk.cn

[U52] PHP：箭头函数
来源：http://vbn.aibaodan.cn

$double = fn($x) => $x * 2;
来源：http://nzy.sweek.top

[U53] PHP：空合并运算符
来源：http://oen.yuxming.cn

$v = $a ?? $b ?? "default";
来源：http://nxd.hfpthk.cn

[U54] PHP：空安全调用
来源：http://kye.sysykeji.top

$obj?->method()
来源：http://ygd.zdqjudy.top

[U55] PHP：match 表达式
来源：http://lrb.xinyue.icu

$s = match($x) { 1 => "一", default => "其他" };
来源：http://lts.hfpthk.cn

[U56] PHP：命名参数
来源：http://zhk.fktsv.cn

f(a: 1, b: 2)
来源：http://pto.ydzc1.top

[U57] PHP：字符串插值
来源：http://ouq.hnqzz.top

"值: {$a}"
来源：http://ofx.uphjek.com

[U58] PHP：数组三件套
来源：http://njc.haohaochexian.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hzy.svipenyu.cn

[U59] PHP：自定义排序
来源：http://dgy.ivvv.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://zna.shanyushiyangtech.top

[U60] PHP：JSON 编解码
来源：http://wbk.pycfn.com

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://vwt.hfpthk.cn

[U61] PHP：正则
来源：http://bfr.bjfxy.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://vkc.yuanzhike.top

[U62] PHP：日期对象
来源：http://tsa.xinyue.icu

(new DateTimeImmutable())->format("Y-m-d");
来源：http://qsp.daria6918.cn

[U63] PHP：文件读写
来源：http://dqa.uphjek.com

file_get_contents($f);  file_put_contents($f, $data);
来源：http://noi.ybcxt.top

[U64] PHP：目录遍历
来源：http://iaq.sjlbkw.cn

glob("dir/*.php");  scandir("dir");
来源：http://skw.fzhhl.top

[U65] PHP：会话
来源：http://tdj.cheryme.top

session_start();  $_SESSION["uid"] = 1;
来源：http://mvd.shuidangran.top

[U66] PHP：设置 Cookie
来源：http://out.jinqigfzy.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://aat.pengpengdd.cyou

[U67] PHP：处理文件上传
来源：http://jzt.daria6918.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://yqx.sxryk.cn

[U68] PHP：PDO 连接
来源：http://vvl.jiagoushi.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://zty.nanxuanxn.top

[U69] PHP：PDO 预处理
来源：http://yiw.nanxinkj.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://idw.zdbjq.cn

[U70] PHP：PDO 事务
来源：http://wkr.cucudq.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://mfs.zhengqikj.top

[U71] PHP：抛出异常
来源：http://iwv.andypj.xyz

throw new RuntimeException("失败", 500);
来源：http://yxq.chenjidiqi.icu

[U72] PHP：写错误日志
来源：http://yyt.kuanghao11.cn

error_log("失败: " . $e->getMessage());
来源：http://fni.xingfuxueyuan.xyz

[U73] PHP：读取 ini 配置
来源：http://woe.quarkkingdee.top

parse_ini_file("config.ini", true)
来源：http://sxm.dashuyun.cn

[U74] PHP：读取环境变量
来源：http://jku.uphjek.com

getenv("APP_ENV") ?: "production"
来源：http://xbe.chenjidiqi.icu

[U75] PHP：依赖注入
来源：http://axx.uphjek.com

composer require psr/container
来源：http://mmp.pengpengdd.cyou

[U76] PHP：简单路由
来源：http://yrk.fzhhl.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://bwg.jiagoushi.top

[U77] PHP：模板渲染
来源：http://ixr.yvedp.cn

composer require twig/twig
来源：http://ucs.kuanghao11.cn

[U78] PHP：单元测试
来源：http://cdg.c1oappe.top

composer require --dev phpunit/phpunit
来源：http://ufw.nanxinkj.top

[U79] PHP：静态分析
来源：http://qcp.guannengcc.top

composer require --dev phpstan/phpstan
来源：http://ucj.meibo888.top

[U80] PHP：代码规范修复
来源：http://whb.zhixingplan.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://ipb.ivvv.top

[U81] JS：初始化项目
来源：http://nlf.kuanghao11.cn

npm init -y;  npm i express
来源：http://ayn.daxiang520.top

[U82] JS：package.json 脚本
来源：http://rbv.hammf.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://suf.jinqigfzy.top

[U83] JS：ES Module 导入导出
来源：http://agm.zdqjudy.top

export const a = 1;  import { a } from "./m.js";
来源：http://rhw.tarul.cn

[U84] JS：CommonJS 写法
来源：http://vwh.sweek.top

module.exports = { a };  const { a } = require("./m");
来源：http://tee.ppjwa.cn

[U85] JS：可选链
来源：http://nfr.haohaochexian.top

a?.b?.c
来源：http://xne.hywenlv.cn

[U86] JS：空值合并
来源：http://new.yangfankeji.com

a ?? b
来源：http://zkq.zhijiandao.cn

[U87] JS：解构默认值
来源：http://ekg.sysykeji.top

const { a = 1, b = 2 } = obj;
来源：http://boc.ppjwa.cn

[U88] JS：对象展开合并
来源：http://wra.sufxvd.cn

{ ...a, ...b }
来源：http://ren.yanxiufei.cn

[U89] JS：数组去重
来源：http://yuu.redwolf501.top

[...new Set(arr)]
来源：http://hdv.tianlin.xyz

[U90] JS：数字数组排序
来源：http://nob.xuetiantiany.cn

[...arr].sort((a, b) => a - b)
来源：http://fwu.yj20258.top

[U91] JS：对象键值遍历
来源：http://jyp.yongpay.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://bik.cheryme.top

[U92] JS：深拷贝
来源：http://ivi.mhx1999.top

structuredClone(obj)
来源：http://wzd.jqgufenzy.top

[U93] JS：模板字符串
来源：http://baj.ybcxt.top

`共 ${n} 条`
来源：http://azf.pengpengdd.cyou

[U94] JS：箭头函数
来源：http://aih.andypj.xyz

const double = x => x * 2;
来源：http://fnm.vehdjk.com

[U95] JS：Promise 包装
来源：http://gei.zhongyouzk.top

new Promise((resolve, reject) => {})
来源：http://daz.hammf.cn

[U96] JS：async/await 与异常
来源：http://acn.zhongyouzk.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://nvv.52xcode.cn

[U97] JS：并发请求
来源：http://sig.bbcook.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://xfq.birdmap.top

[U98] JS：fetch 带 JSON
来源：http://oew.ybcxt.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://jlr.wangshuangyany.cn

[U99] JS：事件监听
来源：http://ewx.wangdashe.top

el.addEventListener("click", e => {})
来源：http://ruv.shangyingyoupin.top

[U100] JS：DOM 查询
来源：http://vtl.gaohongyu789.top

document.querySelector(".item")
来源：http://gnv.yj20258.top

[U101] JS：classList 操作
来源：http://afx.ybcxt.top

el.classList.toggle("active")
来源：http://kfo.cdnleiting.top

[U102] JS：本地存储
来源：http://kcx.gaohongyu789.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://ezp.chenjidiqi.icu

[U103] JS：定时器
来源：http://pue.zdbjq.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://yjy.yj202588.top

[U104] JS：防抖
来源：http://jjv.dashuyun.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://yic.ctjpmb.com

[U105] JS：节流
来源：http://dwt.xingfuxueyuan.xyz

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://zue.hnqzz.top

[U106] JS：日期格式化
来源：http://yyz.shanyushiyangkeji.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://syg.ctjpmb.com

[U107] JS：数字千分位
来源：http://exu.bbcook.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://kup.zdqjudy.top

[U108] JS：随机整数
来源：http://hub.iojbl.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://sfy.tian-w.cn

[U109] JS：数组分组
来源：http://ffr.snrcjt.cn

Object.groupBy(arr, x => x.type)
来源：http://hfr.xingfuxueyuan.xyz

[U110] JS：数组分块
来源：http://ezv.cashguo.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://rtd.shanyushiyangtech.top

[U111] JS：对象转 Map
来源：http://lea.jyoumei.cn

new Map(Object.entries(obj))
来源：http://ceq.wangdashe.top

[U112] JS：字符串补位
来源：http://veq.shzxlz.cn

"7".padStart(3, "0")
来源：http://apz.cdnleiting.top

[U113] JS：正则替换全部
来源：http://tft.yfazqb.com

s.replaceAll("a", "b")
来源：http://xdd.jqgufenzy.top

[U114] JS：JSON 深比较
来源：http://mpp.zhixingplan.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://eqq.sysykeji.top

[U115] JS：生成 UUID
来源：http://iln.gaohongyu789.top

crypto.randomUUID()
来源：http://mkr.hammf.cn

[U116] JS：类型检查（JSDoc）
来源：http://jfr.redwolf501.top

/** @param {string} name */ function f(name) {}
来源：http://nrf.yvedp.cn

[U117] JS：单元测试
来源：http://ezx.yonumen.top

npm i -D vitest;  npx vitest
来源：http://nsm.sysykeji.top

[U118] JS：开发服务器
来源：http://pvk.pycfn.com

npm i -D vite;  npx vite
来源：http://hkt.dashuyun.cn

[U119] JS：生产构建
来源：http://qgr.ctjpmb.com

npx vite build
来源：http://wot.xuetiantiany.cn

[U120] JS：读取环境变量（Vite）
来源：http://stg.ywan-chungtsiang.top

import.meta.env.VITE_API_URL
来源：http://nmx.zdqjudy.top

================================================================================
来源：http://mny.c1oappe.top

统计汇总
来源：http://tyw.nanxuanxn.top

================================================================================
来源：http://pmm.zhongyouzk.top

按语言统计（条）：
来源：http://mmn.vehdjk.com

Python ......... 252
来源：http://xwq.cucudq.cn

PHP ............ 252
来源：http://adu.hammf.cn

JavaScript ..... 252
来源：http://fsm.yangfankeji.com

TypeScript ..... 212
来源：http://qak.yvedp.cn

Java ........... 212
来源：http://srl.jianghu66.top

Go ............. 212
来源：http://zff.fanxiaobao.xyz

Ruby ........... 212
来源：http://ula.ywan-chungtsiang.top

C# ............. 212
来源：http://uzj.fktsv.cn

C .............. 30
来源：http://gki.tarul.cn

C++ ............ 30
来源：http://rye.aizwys.cn

SQL ............ 90
来源：http://ona.kuanghao11.cn

Bash ........... 80
来源：http://crs.jinghuilouyu.cn

Kotlin ......... 15
来源：http://jti.shuidangran.top

Swift .......... 15
来源：http://gii.epnwcf.com

Lua ............ 10
来源：http://czj.gzhubu.top

Perl ........... 10
来源：http://gnu.ehwqpu.com


<!-- 参考信息 -->