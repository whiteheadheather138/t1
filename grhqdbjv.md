代发 wailian999

[T37] Lua：字符串拼接
来源：http://mjp.jinyuanbaomall.cn

"a" .. "b"
来源：http://zay.chenzaomai.com

[T38] Lua：条件
来源：http://yfa.cashguo.top

if x > 0 then print("正") end
来源：http://sde.c1oappe.top

[T39] Lua：模式匹配
来源：http://nwe.sufxvd.cn

string.find(s, "%d+")
来源：http://zva.gogol.net.cn

[T40] Lua：元表
来源：http://hti.smart0.xyz

setmetatable({}, { __index = base })
来源：http://gle.daria6918.cn

[T41] Perl：Hello World
来源：http://tuy.jlsjyb.cn

print "Hello\n";
来源：http://seb.sufxvd.cn

[T42] Perl：变量类型
来源：http://ily.zhiwuduotai.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://bfi.zhixingplan.top

[T43] Perl：字符串插值
来源：http://dmf.aizwys.cn

"值: $a"
来源：http://ugl.jinqigufen.top

[T44] Perl：条件
来源：http://kli.hnqzz.top

if ($a > 0) { print "正"; }
来源：http://dsk.jianghu66.top

[T45] Perl：数组遍历
来源：http://pdj.zhiwuduotai.top

for my $x (@arr) { print $x; }
来源：http://osf.guannengcc.top

[T46] Perl：哈希操作
来源：http://hfu.316326.xyz

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://sjz.hywenlv.cn

[T47] Perl：正则捕获
来源：http://wfh.shangyingyoupin.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://eoc.gotoacloud.top

[T48] Perl：正则替换
来源：http://izu.ctjpmb.com

$s =~ s/old/new/g;
来源：http://fxa.jinyuanbaomall.cn

[T49] Perl：函数
来源：http://bbu.bbcook.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://uai.yanxiufei.cn

[T50] Perl：逐行读文件
来源：http://psc.tian-w.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://rvp.hnxiangtu.top

while (my $line = <$fh>) { print $line; }
来源：http://nnb.jianghu66.top

[T51] Scala：Hello World
来源：http://ltg.316326.xyz

println("Hello")
来源：http://yom.mhx1999.top

[T52] Scala：变量
来源：http://uip.fktsv.cn

val a = 1;  var b = 2
来源：http://eof.chenzaomai.com

[T53] Scala：字符串插值
来源：http://iab.nanxinkj.top

s"值: $b"
来源：http://ewe.aibaodan.cn

[T54] Scala：集合映射
来源：http://thv.316326.xyz

List(1, 2, 3).map(_ * 2)
来源：http://jos.jyoumei.cn

[T55] Scala：集合过滤
来源：http://mft.hcnkem.com

List(1, 2, 3).filter(_ > 1)
来源：http://nrq.zdbjq.cn

[T56] Scala：样例类
来源：http://pga.feifeiyinyue.top

case class User(name: String, age: Int)
来源：http://pqm.gzhubu.top

[T57] Scala：模式匹配
来源：http://bca.vehdjk.com

x match { case 1 => "一"; case _ => "其他" }
来源：http://ktq.redwolf501.top

[T58] Scala：函数定义
来源：http://qyh.pengpengdd.cyou

def add(a: Int, b: Int): Int = a + b
来源：http://ymh.hfpthk.cn

[T59] Scala：循环
来源：http://skg.zhixingplan.top

for (i <- 1 to 10) println(i)
来源：http://wfd.zdbjq.cn

[T60] Scala：折叠
来源：http://yyj.xuetiantiany.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://yqb.chenlongwang.top

================================================================================
来源：http://zlh.ivvv.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://vxb.hysaishi.cn

================================================================================
来源：http://sdz.feifeiyinyue.top

[U01] Py：创建虚拟环境
来源：http://ljj.mhx1999.top

python -m venv .venv && source .venv/bin/activate
来源：http://clo.xinyue.icu

[U02] Py：导出 / 安装依赖
来源：http://tnr.cashguo.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://ert.hcnkem.com

[U03] Py：加载 .env 配置
来源：http://dju.daxiang520.top

from dotenv import load_dotenv; load_dotenv()
来源：http://sfb.yanxiufei.cn

[U04] Py：变量调试打印
来源：http://pew.shanyushiyangkeji.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://lfm.snrcjt.cn

[U05] Py：列表去重且保序
来源：http://vcn.pycfn.com

list(dict.fromkeys(arr))
来源：http://xzn.snrcjt.cn

[U06] Py：合并两个字典
来源：http://jey.jlsjyb.cn

{**a, **b}
来源：http://gcz.gaohongyu789.top

[U07] Py：反转字典键值
来源：http://ewv.nanxinkj.top

{v: k for k, v in d.items()}
来源：http://kms.vehdjk.com

[U08] Py：展平二维列表
来源：http://bkd.yj202588.top

[y for x in nested for y in x]
来源：http://uqc.yj202588.top

[U09] Py：字典取最大值的键
来源：http://umc.ybcxt.top

max(d, key=d.get)
来源：http://vrr.ctjpmb.com

[U10] Py：按值排序字典
来源：http://dbl.jqgfzy.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://sfn.jinyuanbaomall.cn

[U11] Py：生成器表达式
来源：http://bcx.guannengcc.top

(x * 2 for x in arr)
来源：http://crg.shanyushiyangtech.top

[U12] Py：取出现最多的 3 个元素
来源：http://dta.jiagoushi.top

Counter(arr).most_common(3)
来源：http://rxz.hnxiangtu.top

[U13] Py：固定长度队列
来源：http://utv.hesvh.cn

deque(maxlen=10)
来源：http://ojj.gaohongyu789.top

[U14] Py：分组收集到列表
来源：http://imw.pengpengdd.cyou

defaultdict(list)
来源：http://evh.xingfuxueyuan.xyz

[U15] Py：高精度计时
来源：http://ktw.sufxvd.cn

t = time.perf_counter()
来源：http://vpo.hysaishi.cn

[U16] Py：命令行参数解析
来源：http://iga.nwbrower.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hts.cucudq.cn

[U17] Py：初始化日志
来源：http://aoj.jlsjyb.cn

logging.basicConfig(level=logging.INFO)
来源：http://dqo.guowangkeji.top

[U18] Py：预编译正则
来源：http://kbz.tian-w.cn

pat = re.compile(r"\d+")
来源：http://led.sxryk.cn

[U19] Py：正则替换带回调
来源：http://qwp.feifeiyinyue.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://zzm.chenlongwang.top

[U20] Py：缓存函数结果
来源：http://pdr.hnqzz.top

@functools.lru_cache(maxsize=None)
来源：http://gtt.gogol.net.cn

[U21] Py：自定义上下文管理器
来源：http://axa.zycfv.cn

@contextlib.contextmanager
来源：http://lgh.xylfe.cn

[U22] Py：矩阵转置
来源：http://kyv.yanxiufei.cn

list(zip(*m))
来源：http://wcz.zdbjq.cn

[U23] Py：分块读取大文件
来源：http://wpe.dashuyun.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://vsn.tarul.cn

[U24] Py：路径操作
来源：http://ibg.yfazqb.com

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://btu.zhoulong.xyz

[U25] Py：CSV 按字典读
来源：http://wqa.nanxinkj.top

csv.DictReader(f)
来源：http://blt.zhijiandao.cn

[U26] Py：并发下载
来源：http://vwf.pycfn.com

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://fih.hfpthk.cn

[U27] Py：异步 HTTP
来源：http://cmo.shangyingyoupin.top

aiohttp.ClientSession() 配合 async with
来源：http://oic.xingfuxueyuan.xyz

[U28] Py：类型别名
来源：http://bbn.gaohongyu789.top

UserId = int
来源：http://gyq.jinqigfzy.top

[U29] Py：属性校验
来源：http://qwb.hywenlv.cn

@property 与 @x.setter 配合
来源：http://nrn.nwbrower.top

[U30] Py：数据类
来源：http://lva.guowangkeji.top

@dataclass(slots=True)
来源：http://apz.316326.xyz

[U31] Py：单测
来源：http://jct.cheryme.top

python -m pytest -q
来源：http://vgv.zdbjq.cn

[U32] Py：代码格式化
来源：http://dkf.redwolf501.top

ruff format . && ruff check --fix .
来源：http://kbb.yonumen.top

[U33] Py：打包发布
来源：http://rwy.yuanzhike.top

python -m build  （依赖 pyproject.toml）
来源：http://axe.svipenyu.cn

[U34] Py：判断编码
来源：http://jpj.birdmap.top

chardet.detect(raw)
来源：http://jus.shzxlz.cn

[U35] Py：发送邮件
来源：http://jku.zhixingplan.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://anf.0kj1m.cn

[U36] Py：定时任务
来源：http://uri.yuxming.cn

schedule.every(10).minutes.do(job)
来源：http://jqj.shanyushiyangkeji.top

[U37] Py：读写 Excel
来源：http://xop.jinyuanbaomall.cn

pandas.read_excel / DataFrame.to_excel
来源：http://sdo.jlsjyb.cn

[U38] Py：获取脚本所在目录
来源：http://lks.dashuyun.cn

Path(__file__).resolve().parent
来源：http://akm.fanxiaobao.xyz

[U39] Py：判断是否在交互环境
来源：http://nnb.yfazqb.com

sys.stdout.isatty()
来源：http://apo.gaohongyu789.top

[U40] Py：打印到标准错误
来源：http://sle.hysaishi.cn

print("err", file=sys.stderr)
来源：http://kmg.cucudq.cn

[U41] PHP：初始化 Composer 项目
来源：http://afw.jqgufenzy.top

composer init;  composer require guzzlehttp/guzzle
来源：http://gvr.ywan-chungtsiang.top

[U42] PHP：PSR-4 自动加载
来源：http://mmw.bbcook.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://jvs.guowangkeji.top

[U43] PHP：声明命名空间
来源：http://mof.gogol.net.cn

namespace App\Http;
来源：http://rhy.sweek.top

[U44] PHP：开启严格类型
来源：http://adl.kuanghao11.cn

declare(strict_types=1);
来源：http://vuy.gzhubu.top

[U45] PHP：类型声明与返回类型
来源：http://ndd.jyoumei.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://qjo.cashguo.top

[U46] PHP：可空类型
来源：http://jxm.uphjek.com

?string $name = null
来源：http://phi.gaohongyu789.top

[U47] PHP：联合类型
来源：http://jwa.fktsv.cn

int|string $id
来源：http://pku.nwbrower.top

[U48] PHP：纯枚举
来源：http://mkv.chenjidiqi.icu

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://rnp.sxryk.cn

[U49] PHP：只读属性
来源：http://pjy.andypj.xyz

public readonly string $name
来源：http://yeg.andypj.xyz

[U50] PHP：构造器属性提升
来源：http://nnm.pengpengdd.cyou

public function __construct(private int $id) {}
来源：http://pge.zhongyouzk.top

[U51] PHP：数组解构
来源：http://anj.tanke756.top

[$a, $b] = $arr;
来源：http://sos.vqdsnc.cn

[U52] PHP：箭头函数
来源：http://lbu.aizwys.cn

$double = fn($x) => $x * 2;
来源：http://ggg.gzhubu.top

[U53] PHP：空合并运算符
来源：http://abi.vehdjk.com

$v = $a ?? $b ?? "default";
来源：http://srz.guowangkeji.top

[U54] PHP：空安全调用
来源：http://rqb.xylfe.cn

$obj?->method()
来源：http://tep.hongshengwenyu.top

[U55] PHP：match 表达式
来源：http://csd.zhoulong.xyz

$s = match($x) { 1 => "一", default => "其他" };
来源：http://bgu.0kj1m.cn

[U56] PHP：命名参数
来源：http://dob.uphjek.com

f(a: 1, b: 2)
来源：http://qeo.shzxlz.cn

[U57] PHP：字符串插值
来源：http://jsj.tarul.cn

"值: {$a}"
来源：http://dda.zhongyouzk.top

[U58] PHP：数组三件套
来源：http://jbm.daxiang520.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://tuz.jinqigfzy.top

[U59] PHP：自定义排序
来源：http://iaf.ppjwa.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mqp.jiagoushi.top

[U60] PHP：JSON 编解码
来源：http://gua.guannengcc.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://yxf.zdqjudy.top

[U61] PHP：正则
来源：http://bby.quarkkingdee.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://woe.ywan-chungtsiang.top

[U62] PHP：日期对象
来源：http://ret.zhongyouzk.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://pce.gzhubu.top

[U63] PHP：文件读写
来源：http://wyh.shanyushiyangkeji.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://tnb.yj202588.top

[U64] PHP：目录遍历
来源：http://efm.9152youxi.cn

glob("dir/*.php");  scandir("dir");
来源：http://tjz.yanxiufei.cn

[U65] PHP：会话
来源：http://zbj.ydjk.org.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://zqw.feifeiyinyue.top

[U66] PHP：设置 Cookie
来源：http://xcd.zhaomingkeji.xyz

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://vwd.hongshengwenyu.top

[U67] PHP：处理文件上传
来源：http://xvc.jinqigufen.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://jgn.c1oappe.top

[U68] PHP：PDO 连接
来源：http://pih.haohaochexian.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://fry.aizwys.cn

[U69] PHP：PDO 预处理
来源：http://jqw.zhiwuduotai.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://khu.hongshengwenyu.top

[U70] PHP：PDO 事务
来源：http://vup.svipenyu.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://tmr.sweek.top

[U71] PHP：抛出异常
来源：http://eeq.iojbl.cn

throw new RuntimeException("失败", 500);
来源：http://zat.smart0.xyz

[U72] PHP：写错误日志
来源：http://gta.zhengqikj.top

error_log("失败: " . $e->getMessage());
来源：http://rpu.smart0.xyz

[U73] PHP：读取 ini 配置
来源：http://wcq.wangshuangyany.cn

parse_ini_file("config.ini", true)
来源：http://ppv.hongshengwenyu.top

[U74] PHP：读取环境变量
来源：http://mfn.epnwcf.com

getenv("APP_ENV") ?: "production"
来源：http://coo.vehdjk.com

[U75] PHP：依赖注入
来源：http://gkh.redwolf501.top

composer require psr/container
来源：http://muw.zhixingplan.top

[U76] PHP：简单路由
来源：http://qim.yuxming.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://qfl.yueranfly.top

[U77] PHP：模板渲染
来源：http://clz.hongshengwenyu.top

composer require twig/twig
来源：http://zgx.yongpay.top

[U78] PHP：单元测试
来源：http://tni.shzxlz.cn

composer require --dev phpunit/phpunit
来源：http://seo.jinqigufen.top

[U79] PHP：静态分析
来源：http://xyv.yj202588.top

composer require --dev phpstan/phpstan
来源：http://nsd.jinqigufen.top

[U80] PHP：代码规范修复
来源：http://iti.xuanzx.com

composer require --dev friendsofphp/php-cs-fixer
来源：http://car.c1oappe.top

[U81] JS：初始化项目
来源：http://vsh.svipenyu.cn

npm init -y;  npm i express
来源：http://atj.yanxiufei.cn

[U82] JS：package.json 脚本
来源：http://ylb.zhongyouzk.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://wjw.fzhhl.top

[U83] JS：ES Module 导入导出
来源：http://gif.nanxinkj.top

export const a = 1;  import { a } from "./m.js";
来源：http://hil.zycfv.cn

[U84] JS：CommonJS 写法
来源：http://uby.snrcjt.cn

module.exports = { a };  const { a } = require("./m");
来源：http://hwf.gzhubu.top

[U85] JS：可选链
来源：http://srn.chenzaomai.com

a?.b?.c
来源：http://exx.ydjk.org.cn

[U86] JS：空值合并
来源：http://mbc.yuxming.cn

a ?? b
来源：http://tzb.sxryk.cn

[U87] JS：解构默认值
来源：http://qvg.jinqigfzy.top

const { a = 1, b = 2 } = obj;
来源：http://xrb.xingfuxueyuan.xyz

[U88] JS：对象展开合并
来源：http://nzx.xylfe.cn

{ ...a, ...b }
来源：http://vhl.gaohongyu789.top

[U89] JS：数组去重
来源：http://ytc.meibo888.top

[...new Set(arr)]
来源：http://rqq.xylfe.cn

[U90] JS：数字数组排序
来源：http://kff.aibaodan.cn

[...arr].sort((a, b) => a - b)
来源：http://epa.jinqigufen.top

[U91] JS：对象键值遍历
来源：http://nwz.xylfe.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://qmp.jqgufenzy.top

[U92] JS：深拷贝
来源：http://kuj.chenzaomai.com

structuredClone(obj)
来源：http://vyv.hnxiangtu.top

[U93] JS：模板字符串
来源：http://uet.shzxlz.cn

`共 ${n} 条`
来源：http://kbz.meibo888.top

[U94] JS：箭头函数
来源：http://kxr.316326.xyz

const double = x => x * 2;
来源：http://ucg.bjfxy.top

[U95] JS：Promise 包装
来源：http://jcu.sysykeji.top

new Promise((resolve, reject) => {})
来源：http://zah.gzhubu.top

[U96] JS：async/await 与异常
来源：http://rja.meibo888.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://wvz.feifeiyinyue.top

[U97] JS：并发请求
来源：http://yxl.hysaishi.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://ksb.feifeiyinyue.top

[U98] JS：fetch 带 JSON
来源：http://pcx.yvedp.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://cel.jinyuanbaomall.cn

[U99] JS：事件监听
来源：http://khb.ehwqpu.com

el.addEventListener("click", e => {})
来源：http://itf.hywenlv.cn

[U100] JS：DOM 查询
来源：http://oio.wangshuangyany.cn

document.querySelector(".item")
来源：http://vvm.jiagoushi.top

[U101] JS：classList 操作
来源：http://txi.guowangkeji.top

el.classList.toggle("active")
来源：http://ugd.tanke756.top

[U102] JS：本地存储
来源：http://zlm.yj202588.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://egf.yonumen.top

[U103] JS：定时器
来源：http://usb.daria6918.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://sni.shanyushiyangkeji.top

[U104] JS：防抖
来源：http://vtu.hywenlv.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wmf.yfazqb.com

[U105] JS：节流
来源：http://dra.zhaomingkeji.xyz

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://jsx.hfpthk.cn

[U106] JS：日期格式化
来源：http://ops.gzhubu.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://pgk.jlsjyb.cn

[U107] JS：数字千分位
来源：http://pbw.ivvv.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://xvu.kuanghao11.cn

[U108] JS：随机整数
来源：http://mhk.zhoulong.xyz

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://oaf.tanke756.top

[U109] JS：数组分组
来源：http://gpe.mhx1999.top

Object.groupBy(arr, x => x.type)
来源：http://amo.havefunace.top

[U110] JS：数组分块
来源：http://six.svipenyu.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://eot.hnqzz.top

[U111] JS：对象转 Map
来源：http://chb.bjfxy.top

new Map(Object.entries(obj))
来源：http://pzf.zhongyouzk.top

[U112] JS：字符串补位
来源：http://jiy.ppjwa.cn

"7".padStart(3, "0")
来源：http://lly.kuanghao11.cn

[U113] JS：正则替换全部
来源：http://lyh.fengsongda.top

s.replaceAll("a", "b")
来源：http://yxe.sjlbkw.cn

[U114] JS：JSON 深比较
来源：http://gem.zdqjudy.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://yjh.yj202588.top

[U115] JS：生成 UUID
来源：http://tmt.hysaishi.cn

crypto.randomUUID()
来源：http://ism.jinghuilouyu.cn

[U116] JS：类型检查（JSDoc）
来源：http://nci.wangdashe.top

/** @param {string} name */ function f(name) {}
来源：http://dck.xuanzx.com

[U117] JS：单元测试
来源：http://xda.andypj.xyz

npm i -D vitest;  npx vitest
来源：http://kiu.zhoulong.xyz

[U118] JS：开发服务器
来源：http://duo.zdbjq.cn

npm i -D vite;  npx vite
来源：http://yhi.iojbl.cn

[U119] JS：生产构建
来源：http://llw.birdmap.top

npx vite build
来源：http://kgb.shangyingyoupin.top

[U120] JS：读取环境变量（Vite）
来源：http://rxa.sjlbkw.cn

import.meta.env.VITE_API_URL
来源：http://idb.yvedp.cn

================================================================================
来源：http://xdr.hesvh.cn

统计汇总
来源：http://ulv.yuanzhike.top

================================================================================
来源：http://dar.fktsv.cn

按语言统计（条）：
来源：http://tru.hammf.cn

Python ......... 252
来源：http://ddh.xingfuxueyuan.xyz

PHP ............ 252
来源：http://pne.jinghuilouyu.cn

JavaScript ..... 252
来源：http://xsj.vehdjk.com

TypeScript ..... 212
来源：http://tqk.ehwqpu.com


<!-- 参考信息 -->