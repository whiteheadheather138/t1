代发 wailian999

[T35] Lua：字典表
来源：http://dsu.fehbvm.com

local d = { a = 1 };  d.b = 2
来源：http://ibe.shuidangran.top

[T36] Lua：函数
来源：http://tnx.wangdashe.top

function add(a, b) return a + b end
来源：http://brz.sxryk.cn

[T37] Lua：字符串拼接
来源：http://bnt.tanke756.top

"a" .. "b"
来源：http://mxc.yongpay.top

[T38] Lua：条件
来源：http://lai.yanxiufei.cn

if x > 0 then print("正") end
来源：http://lwk.guowangkeji.top

[T39] Lua：模式匹配
来源：http://ffs.tianlin.xyz

string.find(s, "%d+")
来源：http://jal.daria6918.cn

[T40] Lua：元表
来源：http://yku.feifeiyinyue.top

setmetatable({}, { __index = base })
来源：http://ttl.zdbjq.cn

[T41] Perl：Hello World
来源：http://lai.yueranfly.top

print "Hello\n";
来源：http://odr.xinyue.icu

[T42] Perl：变量类型
来源：http://xuk.ydjk.org.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://mhw.52xcode.cn

[T43] Perl：字符串插值
来源：http://yaq.yj20258888.top

"值: $a"
来源：http://ztw.fktsv.cn

[T44] Perl：条件
来源：http://hyc.tian-w.cn

if ($a > 0) { print "正"; }
来源：http://mnr.hysaishi.cn

[T45] Perl：数组遍历
来源：http://hju.sjlbkw.cn

for my $x (@arr) { print $x; }
来源：http://bqr.sysykeji.top

[T46] Perl：哈希操作
来源：http://axv.fktsv.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://yvk.zhaomingkeji.xyz

[T47] Perl：正则捕获
来源：http://mng.ppjwa.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://bxe.zhongyouzk.top

[T48] Perl：正则替换
来源：http://uxy.tanke756.top

$s =~ s/old/new/g;
来源：http://rsm.0kj1m.cn

[T49] Perl：函数
来源：http://tbm.sjlbkw.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://zyw.zhiwuduotai.top

[T50] Perl：逐行读文件
来源：http://jjv.xinyue.icu

open my $fh, "<", "a.txt" or die $!;
来源：http://pxx.ehwqpu.com

while (my $line = <$fh>) { print $line; }
来源：http://pse.yfazqb.com

[T51] Scala：Hello World
来源：http://yyi.jinyuanbaomall.cn

println("Hello")
来源：http://cqo.cucudq.cn

[T52] Scala：变量
来源：http://het.fktsv.cn

val a = 1;  var b = 2
来源：http://kcj.hesvh.cn

[T53] Scala：字符串插值
来源：http://qil.ppjwa.cn

s"值: $b"
来源：http://ico.hongshengwenyu.top

[T54] Scala：集合映射
来源：http://zhg.bbcook.cn

List(1, 2, 3).map(_ * 2)
来源：http://ono.andypj.xyz

[T55] Scala：集合过滤
来源：http://hys.mhx1999.top

List(1, 2, 3).filter(_ > 1)
来源：http://gng.iojbl.cn

[T56] Scala：样例类
来源：http://hle.tarul.cn

case class User(name: String, age: Int)
来源：http://wxt.shuidangran.top

[T57] Scala：模式匹配
来源：http://ljk.smart0.xyz

x match { case 1 => "一"; case _ => "其他" }
来源：http://tlc.xylfe.cn

[T58] Scala：函数定义
来源：http://feo.zdbjq.cn

def add(a: Int, b: Int): Int = a + b
来源：http://hnj.bbcook.cn

[T59] Scala：循环
来源：http://ecp.yongpay.top

for (i <- 1 to 10) println(i)
来源：http://blc.hcnkem.com

[T60] Scala：折叠
来源：http://rkr.shanyushiyangtech.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://nau.gogol.net.cn

================================================================================
来源：http://yug.guowangkeji.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://dhp.xziqi.cn

================================================================================
来源：http://yqv.52xcode.cn

[U01] Py：创建虚拟环境
来源：http://vnx.zhaomingkeji.xyz

python -m venv .venv && source .venv/bin/activate
来源：http://ggr.yj202588.top

[U02] Py：导出 / 安装依赖
来源：http://hiq.hywenlv.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://tal.shangyingyoupin.top

[U03] Py：加载 .env 配置
来源：http://pee.hnxiangtu.top

from dotenv import load_dotenv; load_dotenv()
来源：http://ret.jqgfzy.top

[U04] Py：变量调试打印
来源：http://duv.jinqigfzy.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://vbu.meibo888.top

[U05] Py：列表去重且保序
来源：http://abh.yuxming.cn

list(dict.fromkeys(arr))
来源：http://ewl.feifeiyinyue.top

[U06] Py：合并两个字典
来源：http://xpv.cheryme.top

{**a, **b}
来源：http://mtg.0kj1m.cn

[U07] Py：反转字典键值
来源：http://kdk.fehbvm.com

{v: k for k, v in d.items()}
来源：http://omv.hywenlv.cn

[U08] Py：展平二维列表
来源：http://yfk.yongpay.top

[y for x in nested for y in x]
来源：http://sya.pengpengdd.cyou

[U09] Py：字典取最大值的键
来源：http://avd.aibaodan.cn

max(d, key=d.get)
来源：http://qxs.quarkkingdee.top

[U10] Py：按值排序字典
来源：http://rpo.yuanzhike.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://jjf.0kj1m.cn

[U11] Py：生成器表达式
来源：http://ttw.aizwys.cn

(x * 2 for x in arr)
来源：http://lrv.hongshengwenyu.top

[U12] Py：取出现最多的 3 个元素
来源：http://oaf.zhiwuduotai.top

Counter(arr).most_common(3)
来源：http://llt.52xcode.cn

[U13] Py：固定长度队列
来源：http://sjz.chenlongwang.top

deque(maxlen=10)
来源：http://bwm.sxryk.cn

[U14] Py：分组收集到列表
来源：http://tkx.jinghuilouyu.cn

defaultdict(list)
来源：http://dkf.shangyingyoupin.top

[U15] Py：高精度计时
来源：http://blz.jiagoushi.top

t = time.perf_counter()
来源：http://wxi.mhx1999.top

[U16] Py：命令行参数解析
来源：http://cid.sufxvd.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://nde.hammf.cn

[U17] Py：初始化日志
来源：http://lwm.52xcode.cn

logging.basicConfig(level=logging.INFO)
来源：http://sdg.hywenlv.cn

[U18] Py：预编译正则
来源：http://zci.cheryme.top

pat = re.compile(r"\d+")
来源：http://eoj.fzhhl.top

[U19] Py：正则替换带回调
来源：http://yfy.svipenyu.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://dds.cdnleiting.top

[U20] Py：缓存函数结果
来源：http://ddz.yj20258888.top

@functools.lru_cache(maxsize=None)
来源：http://kvx.52xcode.cn

[U21] Py：自定义上下文管理器
来源：http://jpf.chenlongwang.top

@contextlib.contextmanager
来源：http://ilr.xingfuxueyuan.xyz

[U22] Py：矩阵转置
来源：http://pqk.zhoulong.xyz

list(zip(*m))
来源：http://rom.xziqi.cn

[U23] Py：分块读取大文件
来源：http://moi.zhongyouzk.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://onm.hywenlv.cn

[U24] Py：路径操作
来源：http://jre.wangdashe.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://mwl.dianchejie.cn

[U25] Py：CSV 按字典读
来源：http://rmj.hfpthk.cn

csv.DictReader(f)
来源：http://rdv.nanxuanxn.top

[U26] Py：并发下载
来源：http://qda.zhaomingkeji.xyz

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://qua.shuidangran.top

[U27] Py：异步 HTTP
来源：http://kvy.zycfv.cn

aiohttp.ClientSession() 配合 async with
来源：http://oie.kuanghao11.cn

[U28] Py：类型别名
来源：http://eih.jinghuilouyu.cn

UserId = int
来源：http://vai.yuanzhike.top

[U29] Py：属性校验
来源：http://dcv.dianchejie.cn

@property 与 @x.setter 配合
来源：http://xtq.yj20258.top

[U30] Py：数据类
来源：http://jde.kuanghao11.cn

@dataclass(slots=True)
来源：http://iqk.meibo888.top

[U31] Py：单测
来源：http://erv.kuanghao11.cn

python -m pytest -q
来源：http://ozs.jinqigufen.top

[U32] Py：代码格式化
来源：http://gqo.jlsjyb.cn

ruff format . && ruff check --fix .
来源：http://wwe.feifeiyinyue.top

[U33] Py：打包发布
来源：http://cst.ybcxt.top

python -m build  （依赖 pyproject.toml）
来源：http://ywz.jyoumei.cn

[U34] Py：判断编码
来源：http://jrb.dashuyun.cn

chardet.detect(raw)
来源：http://pth.zdqjudy.top

[U35] Py：发送邮件
来源：http://psh.52xcode.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://uhy.ywan-chungtsiang.top

[U36] Py：定时任务
来源：http://zdd.ywan-chungtsiang.top

schedule.every(10).minutes.do(job)
来源：http://gur.jinqigufen.top

[U37] Py：读写 Excel
来源：http://sze.ywan-chungtsiang.top

pandas.read_excel / DataFrame.to_excel
来源：http://wqk.ybcxt.top

[U38] Py：获取脚本所在目录
来源：http://fjj.ywan-chungtsiang.top

Path(__file__).resolve().parent
来源：http://oty.hywenlv.cn

[U39] Py：判断是否在交互环境
来源：http://rmq.ydjk.org.cn

sys.stdout.isatty()
来源：http://sxk.hnxiangtu.top

[U40] Py：打印到标准错误
来源：http://jxp.yj202588.top

print("err", file=sys.stderr)
来源：http://ipa.jinqigfzy.top

[U41] PHP：初始化 Composer 项目
来源：http://mgz.bjfxy.top

composer init;  composer require guzzlehttp/guzzle
来源：http://ivu.zhiwuduotai.top

[U42] PHP：PSR-4 自动加载
来源：http://sfg.vqdsnc.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://vse.gogol.net.cn

[U43] PHP：声明命名空间
来源：http://ggc.guannengcc.top

namespace App\Http;
来源：http://kxi.pengpengdd.cyou

[U44] PHP：开启严格类型
来源：http://jqz.hammf.cn

declare(strict_types=1);
来源：http://kfv.smart0.xyz

[U45] PHP：类型声明与返回类型
来源：http://ivo.zhongyouzk.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://ppd.hcnkem.com

[U46] PHP：可空类型
来源：http://jtr.vehdjk.com

?string $name = null
来源：http://xrv.fktsv.cn

[U47] PHP：联合类型
来源：http://zbo.sufxvd.cn

int|string $id
来源：http://gvd.zhijiandao.cn

[U48] PHP：纯枚举
来源：http://chc.ctjpmb.com

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://pqg.chenzaomai.com

[U49] PHP：只读属性
来源：http://gwz.zhixingplan.top

public readonly string $name
来源：http://twa.zhoulong.xyz

[U50] PHP：构造器属性提升
来源：http://edl.hnxiangtu.top

public function __construct(private int $id) {}
来源：http://kjo.zdqjudy.top

[U51] PHP：数组解构
来源：http://zbi.havefunace.top

[$a, $b] = $arr;
来源：http://btk.nanxuanxn.top

[U52] PHP：箭头函数
来源：http://ekk.hesvh.cn

$double = fn($x) => $x * 2;
来源：http://ofb.bbcook.cn

[U53] PHP：空合并运算符
来源：http://toc.sysykeji.top

$v = $a ?? $b ?? "default";
来源：http://bqc.hesvh.cn

[U54] PHP：空安全调用
来源：http://baw.wangshuangyany.cn

$obj?->method()
来源：http://dlb.quarkkingdee.top

[U55] PHP：match 表达式
来源：http://npf.daxiang520.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://ecv.gogol.net.cn

[U56] PHP：命名参数
来源：http://ujv.hongshengwenyu.top

f(a: 1, b: 2)
来源：http://edm.9152youxi.cn

[U57] PHP：字符串插值
来源：http://def.gzhubu.top

"值: {$a}"
来源：http://bip.shanyushiyangkeji.top

[U58] PHP：数组三件套
来源：http://mus.yuanzhike.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://ytl.bjfxy.top

[U59] PHP：自定义排序
来源：http://jsg.sufxvd.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://rxs.epnwcf.com

[U60] PHP：JSON 编解码
来源：http://kfn.wangdashe.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://wum.havefunace.top

[U61] PHP：正则
来源：http://yet.cucudq.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://lxr.svipenyu.cn

[U62] PHP：日期对象
来源：http://zft.52xcode.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://nwo.wangdashe.top

[U63] PHP：文件读写
来源：http://yug.redwolf501.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://lvo.gzhubu.top

[U64] PHP：目录遍历
来源：http://mib.jinqigfzy.top

glob("dir/*.php");  scandir("dir");
来源：http://vob.fengsongda.top

[U65] PHP：会话
来源：http://yoq.zdbjq.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://tsv.andypj.xyz

[U66] PHP：设置 Cookie
来源：http://szt.xuanzx.com

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://kbf.gotoacloud.top

[U67] PHP：处理文件上传
来源：http://ahy.guannengcc.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://pxq.zycfv.cn

[U68] PHP：PDO 连接
来源：http://npm.sweek.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://atv.jqgfzy.top

[U69] PHP：PDO 预处理
来源：http://zkt.jqgufenzy.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://qll.xuanzx.com

[U70] PHP：PDO 事务
来源：http://qhp.9152youxi.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://qkr.cdnleiting.top

[U71] PHP：抛出异常
来源：http://mlj.gogol.net.cn

throw new RuntimeException("失败", 500);
来源：http://adv.xziqi.cn

[U72] PHP：写错误日志
来源：http://zgu.feifeiyinyue.top

error_log("失败: " . $e->getMessage());
来源：http://eva.tarul.cn

[U73] PHP：读取 ini 配置
来源：http://zel.yangfankeji.com

parse_ini_file("config.ini", true)
来源：http://dul.52xcode.cn

[U74] PHP：读取环境变量
来源：http://obm.bbcook.cn

getenv("APP_ENV") ?: "production"
来源：http://ymi.hammf.cn

[U75] PHP：依赖注入
来源：http://pmi.kuanghao11.cn

composer require psr/container
来源：http://krq.smart0.xyz

[U76] PHP：简单路由
来源：http://ywn.haohaochexian.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://nww.kuanghao11.cn

[U77] PHP：模板渲染
来源：http://waq.shzxlz.cn

composer require twig/twig
来源：http://dzw.zhixingplan.top

[U78] PHP：单元测试
来源：http://fto.ivvv.top

composer require --dev phpunit/phpunit
来源：http://ggg.birdmap.top

[U79] PHP：静态分析
来源：http://tqa.kuanghao11.cn

composer require --dev phpstan/phpstan
来源：http://ikm.yfazqb.com

[U80] PHP：代码规范修复
来源：http://nev.hammf.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://xcc.yuxming.cn

[U81] JS：初始化项目
来源：http://xgv.zdbjq.cn

npm init -y;  npm i express
来源：http://ode.fanxiaobao.xyz

[U82] JS：package.json 脚本
来源：http://hzt.gogol.net.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://cms.cdnleiting.top

[U83] JS：ES Module 导入导出
来源：http://zxa.0kj1m.cn

export const a = 1;  import { a } from "./m.js";
来源：http://ryu.smart0.xyz

[U84] JS：CommonJS 写法
来源：http://rtb.feifeiyinyue.top

module.exports = { a };  const { a } = require("./m");
来源：http://glf.jqgfzy.top

[U85] JS：可选链
来源：http://hkp.jinghuilouyu.cn

a?.b?.c
来源：http://asi.jinghuilouyu.cn

[U86] JS：空值合并
来源：http://nry.uphjek.com

a ?? b
来源：http://rmr.tian-w.cn

[U87] JS：解构默认值
来源：http://bui.bbcook.cn

const { a = 1, b = 2 } = obj;
来源：http://xzt.haohaochexian.top

[U88] JS：对象展开合并
来源：http://asx.xziqi.cn

{ ...a, ...b }
来源：http://hoa.vehdjk.com

[U89] JS：数组去重
来源：http://psp.316326.xyz

[...new Set(arr)]
来源：http://wnm.cashguo.top

[U90] JS：数字数组排序
来源：http://frj.fzhhl.top

[...arr].sort((a, b) => a - b)
来源：http://vyf.jinqigufen.top

[U91] JS：对象键值遍历
来源：http://qzu.feifeiyinyue.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://ony.tian-w.cn

[U92] JS：深拷贝
来源：http://pbo.ybcxt.top

structuredClone(obj)
来源：http://crn.bjfxy.top

[U93] JS：模板字符串
来源：http://pzt.zhaomingkeji.xyz

`共 ${n} 条`
来源：http://szv.yangfankeji.com

[U94] JS：箭头函数
来源：http://fzk.ppjwa.cn

const double = x => x * 2;
来源：http://bxx.bbcook.cn

[U95] JS：Promise 包装
来源：http://oou.c1oappe.top

new Promise((resolve, reject) => {})
来源：http://cht.vqdsnc.cn

[U96] JS：async/await 与异常
来源：http://wnv.iojbl.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://ciz.gaohongyu789.top

[U97] JS：并发请求
来源：http://mhr.zhixingplan.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://qet.tarul.cn

[U98] JS：fetch 带 JSON
来源：http://hwx.ybcxt.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hmj.9152youxi.cn

[U99] JS：事件监听
来源：http://dkd.iojbl.cn

el.addEventListener("click", e => {})
来源：http://wbk.hysaishi.cn

[U100] JS：DOM 查询
来源：http://oot.iojbl.cn

document.querySelector(".item")
来源：http://fkp.hammf.cn

[U101] JS：classList 操作
来源：http://tzj.daria6918.cn

el.classList.toggle("active")
来源：http://tjk.yj20258888.top

[U102] JS：本地存储
来源：http://aob.jyoumei.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://kdy.zhoulong.xyz

[U103] JS：定时器
来源：http://ykv.zycfv.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://kwm.ydjk.org.cn

[U104] JS：防抖
来源：http://gup.ctjpmb.com

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ifc.pycfn.com

[U105] JS：节流
来源：http://mxw.xinyue.icu

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://jee.hcnkem.com

[U106] JS：日期格式化
来源：http://ykq.yueranfly.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://pwv.hnxiangtu.top

[U107] JS：数字千分位
来源：http://edc.guowangkeji.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://sgy.jinyuanbaomall.cn

[U108] JS：随机整数
来源：http://kpj.aibaodan.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://seo.pycfn.com

[U109] JS：数组分组
来源：http://bhr.pengpengdd.cyou

Object.groupBy(arr, x => x.type)
来源：http://atq.shangyingyoupin.top

[U110] JS：数组分块
来源：http://wgc.yongpay.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://fkx.hysaishi.cn

[U111] JS：对象转 Map
来源：http://wuj.jianghu66.top

new Map(Object.entries(obj))
来源：http://dmu.fengsongda.top

[U112] JS：字符串补位
来源：http://urx.nanxuanxn.top

"7".padStart(3, "0")
来源：http://hxn.jinyuanbaomall.cn

[U113] JS：正则替换全部
来源：http://xxr.zhiwuduotai.top

s.replaceAll("a", "b")
来源：http://rsa.zdqjudy.top

[U114] JS：JSON 深比较
来源：http://xjw.shzxlz.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://sej.cdnleiting.top

[U115] JS：生成 UUID
来源：http://flr.yueranfly.top

crypto.randomUUID()
来源：http://nte.birdmap.top

[U116] JS：类型检查（JSDoc）
来源：http://vyr.316326.xyz

/** @param {string} name */ function f(name) {}
来源：http://xjy.yanxiufei.cn

[U117] JS：单元测试
来源：http://ytd.hammf.cn

npm i -D vitest;  npx vitest
来源：http://pqi.cucudq.cn

[U118] JS：开发服务器
来源：http://spg.hnxiangtu.top

npm i -D vite;  npx vite
来源：http://wxr.haohaochexian.top

[U119] JS：生产构建
来源：http://rgz.yfazqb.com

npx vite build
来源：http://eqf.yfazqb.com

[U120] JS：读取环境变量（Vite）
来源：http://kmh.hysaishi.cn

import.meta.env.VITE_API_URL
来源：http://exr.yfazqb.com

================================================================================
来源：http://lvj.svipenyu.cn

统计汇总
来源：http://tgi.pengpengdd.cyou

================================================================================
来源：http://dcz.yvedp.cn

按语言统计（条）：
来源：http://pvw.xuanzx.com


<!-- 参考信息 -->