代发 wailian999

[T33] Lua：表（数组）
来源：http://zrx.fanxiaobao.xyz

local t = {1, 2, 3};  t[4] = 4
来源：http://brb.zycfv.cn

[T34] Lua：遍历表
来源：http://swm.zhijiandao.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://gec.shanyushiyangtech.top

[T35] Lua：字典表
来源：http://nmj.mhx1999.top

local d = { a = 1 };  d.b = 2
来源：http://fkl.daria6918.cn

[T36] Lua：函数
来源：http://lfo.wangshuangyany.cn

function add(a, b) return a + b end
来源：http://iwc.xuetiantiany.cn

[T37] Lua：字符串拼接
来源：http://jcy.ehwqpu.com

"a" .. "b"
来源：http://hvd.hcnkem.com

[T38] Lua：条件
来源：http://lvx.jinqigufen.top

if x > 0 then print("正") end
来源：http://gsv.yanxiufei.cn

[T39] Lua：模式匹配
来源：http://olx.zhoulong.xyz

string.find(s, "%d+")
来源：http://kcq.meibo888.top

[T40] Lua：元表
来源：http://ewc.guowangkeji.top

setmetatable({}, { __index = base })
来源：http://seq.zdqjudy.top

[T41] Perl：Hello World
来源：http://gwb.cqqwz.cn

print "Hello\n";
来源：http://gew.hywenlv.cn

[T42] Perl：变量类型
来源：http://pnq.pengpengdd.cyou

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://bjm.ppjwa.cn

[T43] Perl：字符串插值
来源：http://wus.meibo888.top

"值: $a"
来源：http://wcz.hammf.cn

[T44] Perl：条件
来源：http://the.nanxinkj.top

if ($a > 0) { print "正"; }
来源：http://ear.sjlbkw.cn

[T45] Perl：数组遍历
来源：http://dta.gogol.net.cn

for my $x (@arr) { print $x; }
来源：http://xof.vqdsnc.cn

[T46] Perl：哈希操作
来源：http://rui.fengsongda.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://iwz.uphjek.com

[T47] Perl：正则捕获
来源：http://tag.yangfankeji.com

if ($s =~ /(\d+)/) { print $1; }
来源：http://egf.zhengqikj.top

[T48] Perl：正则替换
来源：http://iwe.mhx1999.top

$s =~ s/old/new/g;
来源：http://uhl.chenlongwang.top

[T49] Perl：函数
来源：http://iwi.cashguo.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://yed.pengpengdd.cyou

[T50] Perl：逐行读文件
来源：http://onb.dashuyun.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://acw.c1oappe.top

while (my $line = <$fh>) { print $line; }
来源：http://aqy.xuanzx.com

[T51] Scala：Hello World
来源：http://ejn.ivvv.top

println("Hello")
来源：http://cdc.gzhubu.top

[T52] Scala：变量
来源：http://nsk.pycfn.com

val a = 1;  var b = 2
来源：http://xur.shzxlz.cn

[T53] Scala：字符串插值
来源：http://tkc.jinyuanbaomall.cn

s"值: $b"
来源：http://jcx.jyoumei.cn

[T54] Scala：集合映射
来源：http://ejk.tarul.cn

List(1, 2, 3).map(_ * 2)
来源：http://gxn.cqqwz.cn

[T55] Scala：集合过滤
来源：http://xfk.redwolf501.top

List(1, 2, 3).filter(_ > 1)
来源：http://sna.jyoumei.cn

[T56] Scala：样例类
来源：http://ysz.9152youxi.cn

case class User(name: String, age: Int)
来源：http://qmm.gaohongyu789.top

[T57] Scala：模式匹配
来源：http://pwi.yvedp.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://gul.yj202588.top

[T58] Scala：函数定义
来源：http://txh.dashuyun.cn

def add(a: Int, b: Int): Int = a + b
来源：http://vig.ivvv.top

[T59] Scala：循环
来源：http://aqp.jinqigufen.top

for (i <- 1 to 10) println(i)
来源：http://msn.uphjek.com

[T60] Scala：折叠
来源：http://ndj.zhengqikj.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://qua.guannengcc.top

================================================================================
来源：http://ehc.tanke756.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://vxs.jyoumei.cn

================================================================================
来源：http://wxl.ybcxt.top

[U01] Py：创建虚拟环境
来源：http://xza.feifeiyinyue.top

python -m venv .venv && source .venv/bin/activate
来源：http://nzb.yj202588.top

[U02] Py：导出 / 安装依赖
来源：http://jtw.ivvv.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://bkl.cdnleiting.top

[U03] Py：加载 .env 配置
来源：http://zuv.sweek.top

from dotenv import load_dotenv; load_dotenv()
来源：http://ipc.nanxinkj.top

[U04] Py：变量调试打印
来源：http://iuw.haohaochexian.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hky.wangdashe.top

[U05] Py：列表去重且保序
来源：http://orr.tianlin.xyz

list(dict.fromkeys(arr))
来源：http://hgd.nwbrower.top

[U06] Py：合并两个字典
来源：http://uir.gzhubu.top

{**a, **b}
来源：http://gui.xinyue.icu

[U07] Py：反转字典键值
来源：http://kel.52xcode.cn

{v: k for k, v in d.items()}
来源：http://ceh.sufxvd.cn

[U08] Py：展平二维列表
来源：http://ahx.tarul.cn

[y for x in nested for y in x]
来源：http://zin.yj202588.top

[U09] Py：字典取最大值的键
来源：http://sul.zdqjudy.top

max(d, key=d.get)
来源：http://lvz.zycfv.cn

[U10] Py：按值排序字典
来源：http://qnk.sufxvd.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://gub.kuanghao11.cn

[U11] Py：生成器表达式
来源：http://tyj.yueranfly.top

(x * 2 for x in arr)
来源：http://abg.jinyuanbaomall.cn

[U12] Py：取出现最多的 3 个元素
来源：http://rqk.xingfuxueyuan.xyz

Counter(arr).most_common(3)
来源：http://zsk.kuanghao11.cn

[U13] Py：固定长度队列
来源：http://ubm.jinqigfzy.top

deque(maxlen=10)
来源：http://kav.jiagoushi.top

[U14] Py：分组收集到列表
来源：http://wvn.iojbl.cn

defaultdict(list)
来源：http://geb.wangdashe.top

[U15] Py：高精度计时
来源：http://qip.yonumen.top

t = time.perf_counter()
来源：http://nfl.kuanghao11.cn

[U16] Py：命令行参数解析
来源：http://jin.haohaochexian.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://bfb.havefunace.top

[U17] Py：初始化日志
来源：http://ulo.yj202588.top

logging.basicConfig(level=logging.INFO)
来源：http://gbx.sxryk.cn

[U18] Py：预编译正则
来源：http://jlt.wangdashe.top

pat = re.compile(r"\d+")
来源：http://axh.bjfxy.top

[U19] Py：正则替换带回调
来源：http://lly.ctjpmb.com

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://enz.jinyuanbaomall.cn

[U20] Py：缓存函数结果
来源：http://wzh.nanxuanxn.top

@functools.lru_cache(maxsize=None)
来源：http://ugk.dianchejie.cn

[U21] Py：自定义上下文管理器
来源：http://fuu.ppjwa.cn

@contextlib.contextmanager
来源：http://qcm.haohaochexian.top

[U22] Py：矩阵转置
来源：http://mny.jyoumei.cn

list(zip(*m))
来源：http://mca.hfpthk.cn

[U23] Py：分块读取大文件
来源：http://sbc.hesvh.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://joh.sxryk.cn

[U24] Py：路径操作
来源：http://kel.zhiwuduotai.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://bqf.gzhubu.top

[U25] Py：CSV 按字典读
来源：http://eet.daria6918.cn

csv.DictReader(f)
来源：http://muk.nanxinkj.top

[U26] Py：并发下载
来源：http://urd.xylfe.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hqy.gotoacloud.top

[U27] Py：异步 HTTP
来源：http://vsr.zhongyouzk.top

aiohttp.ClientSession() 配合 async with
来源：http://jdg.sxryk.cn

[U28] Py：类型别名
来源：http://kbd.gaohongyu789.top

UserId = int
来源：http://qsc.jqgfzy.top

[U29] Py：属性校验
来源：http://azm.ybcxt.top

@property 与 @x.setter 配合
来源：http://crs.ybcxt.top

[U30] Py：数据类
来源：http://twd.jqgufenzy.top

@dataclass(slots=True)
来源：http://mot.chenjidiqi.icu

[U31] Py：单测
来源：http://xdt.quarkkingdee.top

python -m pytest -q
来源：http://jvx.birdmap.top

[U32] Py：代码格式化
来源：http://xtw.yj202588.top

ruff format . && ruff check --fix .
来源：http://dyo.yuanzhike.top

[U33] Py：打包发布
来源：http://wkq.zhixingplan.top

python -m build  （依赖 pyproject.toml）
来源：http://yxe.jianghu66.top

[U34] Py：判断编码
来源：http://brn.hysaishi.cn

chardet.detect(raw)
来源：http://tbo.ctjpmb.com

[U35] Py：发送邮件
来源：http://udc.zycfv.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://ntw.cdnleiting.top

[U36] Py：定时任务
来源：http://ymb.havefunace.top

schedule.every(10).minutes.do(job)
来源：http://zgj.aibaodan.cn

[U37] Py：读写 Excel
来源：http://iik.ywan-chungtsiang.top

pandas.read_excel / DataFrame.to_excel
来源：http://ulr.snrcjt.cn

[U38] Py：获取脚本所在目录
来源：http://ldf.guowangkeji.top

Path(__file__).resolve().parent
来源：http://ips.svipenyu.cn

[U39] Py：判断是否在交互环境
来源：http://nlq.daxiang520.top

sys.stdout.isatty()
来源：http://owv.jyoumei.cn

[U40] Py：打印到标准错误
来源：http://zia.zhijiandao.cn

print("err", file=sys.stderr)
来源：http://jjw.shangyingyoupin.top

[U41] PHP：初始化 Composer 项目
来源：http://gpn.ybcxt.top

composer init;  composer require guzzlehttp/guzzle
来源：http://lgk.yongpay.top

[U42] PHP：PSR-4 自动加载
来源：http://cmb.vqdsnc.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://erz.fktsv.cn

[U43] PHP：声明命名空间
来源：http://hlp.epnwcf.com

namespace App\Http;
来源：http://bac.52xcode.cn

[U44] PHP：开启严格类型
来源：http://vca.gzhubu.top

declare(strict_types=1);
来源：http://zit.hnqzz.top

[U45] PHP：类型声明与返回类型
来源：http://fkx.yj20258888.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://ccb.fengsongda.top

[U46] PHP：可空类型
来源：http://acr.ybcxt.top

?string $name = null
来源：http://lkv.hnqzz.top

[U47] PHP：联合类型
来源：http://jqm.yj202588.top

int|string $id
来源：http://tgc.yanxiufei.cn

[U48] PHP：纯枚举
来源：http://rqu.yj20258.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://jvr.uphjek.com

[U49] PHP：只读属性
来源：http://oqn.cashguo.top

public readonly string $name
来源：http://kay.jinyuanbaomall.cn

[U50] PHP：构造器属性提升
来源：http://aox.xingfuxueyuan.xyz

public function __construct(private int $id) {}
来源：http://lgw.ybcxt.top

[U51] PHP：数组解构
来源：http://ses.smart0.xyz

[$a, $b] = $arr;
来源：http://zpy.zhengqikj.top

[U52] PHP：箭头函数
来源：http://rji.yueranfly.top

$double = fn($x) => $x * 2;
来源：http://xnm.yuanzhike.top

[U53] PHP：空合并运算符
来源：http://jmf.hongshengwenyu.top

$v = $a ?? $b ?? "default";
来源：http://npu.gzhubu.top

[U54] PHP：空安全调用
来源：http://wei.bjfxy.top

$obj?->method()
来源：http://lif.redwolf501.top

[U55] PHP：match 表达式
来源：http://owz.zhongyouzk.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://nwy.pengpengdd.cyou

[U56] PHP：命名参数
来源：http://lgo.bbcook.cn

f(a: 1, b: 2)
来源：http://hnw.chenjidiqi.icu

[U57] PHP：字符串插值
来源：http://qxw.hesvh.cn

"值: {$a}"
来源：http://dhk.zycfv.cn

[U58] PHP：数组三件套
来源：http://cki.chenjidiqi.icu

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://wnu.shangyingyoupin.top

[U59] PHP：自定义排序
来源：http://vkh.svipenyu.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wpo.ehwqpu.com

[U60] PHP：JSON 编解码
来源：http://hts.daria6918.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://iyg.shzxlz.cn

[U61] PHP：正则
来源：http://ymw.shuidangran.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://boh.xinyue.icu

[U62] PHP：日期对象
来源：http://nhf.hongshengwenyu.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://fto.hysaishi.cn

[U63] PHP：文件读写
来源：http://dns.hammf.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hio.yangfankeji.com

[U64] PHP：目录遍历
来源：http://gzc.wangdashe.top

glob("dir/*.php");  scandir("dir");
来源：http://aat.hongshengwenyu.top

[U65] PHP：会话
来源：http://puv.wangshuangyany.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://ffv.shuidangran.top

[U66] PHP：设置 Cookie
来源：http://myl.cheryme.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://yqu.xingfuxueyuan.xyz

[U67] PHP：处理文件上传
来源：http://evq.sufxvd.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://ldn.0kj1m.cn

[U68] PHP：PDO 连接
来源：http://vzt.zhixingplan.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://lfj.xuanzx.com

[U69] PHP：PDO 预处理
来源：http://pfq.jiagoushi.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://yeh.jinqigufen.top

[U70] PHP：PDO 事务
来源：http://wrl.yuanzhike.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://oly.xylfe.cn

[U71] PHP：抛出异常
来源：http://fao.yuanzhike.top

throw new RuntimeException("失败", 500);
来源：http://onb.chenlongwang.top

[U72] PHP：写错误日志
来源：http://web.guowangkeji.top

error_log("失败: " . $e->getMessage());
来源：http://smh.hongshengwenyu.top

[U73] PHP：读取 ini 配置
来源：http://dqz.zdqjudy.top

parse_ini_file("config.ini", true)
来源：http://fqz.nanxuanxn.top

[U74] PHP：读取环境变量
来源：http://knq.birdmap.top

getenv("APP_ENV") ?: "production"
来源：http://pai.mhx1999.top

[U75] PHP：依赖注入
来源：http://jyb.fehbvm.com

composer require psr/container
来源：http://gje.316326.xyz

[U76] PHP：简单路由
来源：http://bhr.bbcook.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://but.tanke756.top

[U77] PHP：模板渲染
来源：http://dvg.zycfv.cn

composer require twig/twig
来源：http://tjb.jyoumei.cn

[U78] PHP：单元测试
来源：http://mjd.haohaochexian.top

composer require --dev phpunit/phpunit
来源：http://hnt.hammf.cn

[U79] PHP：静态分析
来源：http://tki.ydjk.org.cn

composer require --dev phpstan/phpstan
来源：http://cmv.fanxiaobao.xyz

[U80] PHP：代码规范修复
来源：http://mcc.xylfe.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://kfp.yongpay.top

[U81] JS：初始化项目
来源：http://fxm.tianlin.xyz

npm init -y;  npm i express
来源：http://jil.vqdsnc.cn

[U82] JS：package.json 脚本
来源：http://mtl.zhijiandao.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://ypr.chenjidiqi.icu

[U83] JS：ES Module 导入导出
来源：http://bsa.havefunace.top

export const a = 1;  import { a } from "./m.js";
来源：http://qsm.fehbvm.com

[U84] JS：CommonJS 写法
来源：http://mnv.shanyushiyangtech.top

module.exports = { a };  const { a } = require("./m");
来源：http://bfc.cdnleiting.top

[U85] JS：可选链
来源：http://iqv.yj20258888.top

a?.b?.c
来源：http://bme.fehbvm.com

[U86] JS：空值合并
来源：http://qzj.yueranfly.top

a ?? b
来源：http://trn.yangfankeji.com

[U87] JS：解构默认值
来源：http://vdj.shanyushiyangkeji.top

const { a = 1, b = 2 } = obj;
来源：http://nnf.bjfxy.top

[U88] JS：对象展开合并
来源：http://mrs.xziqi.cn

{ ...a, ...b }
来源：http://kht.ywan-chungtsiang.top

[U89] JS：数组去重
来源：http://wfs.c1oappe.top

[...new Set(arr)]
来源：http://yju.daxiang520.top

[U90] JS：数字数组排序
来源：http://kvp.guowangkeji.top

[...arr].sort((a, b) => a - b)
来源：http://lxg.xuetiantiany.cn

[U91] JS：对象键值遍历
来源：http://jxw.tarul.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://pbw.meibo888.top

[U92] JS：深拷贝
来源：http://oei.zhoulong.xyz

structuredClone(obj)
来源：http://xxs.zhongyouzk.top

[U93] JS：模板字符串
来源：http://xxx.hcnkem.com

`共 ${n} 条`
来源：http://ewt.sxryk.cn

[U94] JS：箭头函数
来源：http://dzn.jyoumei.cn

const double = x => x * 2;
来源：http://tzk.vqdsnc.cn

[U95] JS：Promise 包装
来源：http://gao.yueranfly.top

new Promise((resolve, reject) => {})
来源：http://bgb.yvedp.cn

[U96] JS：async/await 与异常
来源：http://tba.yj20258888.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hes.yuanzhike.top

[U97] JS：并发请求
来源：http://lpy.zhoulong.xyz

await Promise.all(urls.map(u => fetch(u)))
来源：http://kls.svipenyu.cn

[U98] JS：fetch 带 JSON
来源：http://jct.wangdashe.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://bix.jinqigufen.top

[U99] JS：事件监听
来源：http://uth.snrcjt.cn

el.addEventListener("click", e => {})
来源：http://swu.c1oappe.top

[U100] JS：DOM 查询
来源：http://obk.ppjwa.cn

document.querySelector(".item")
来源：http://idv.wangshuangyany.cn

[U101] JS：classList 操作
来源：http://mne.yongpay.top

el.classList.toggle("active")
来源：http://tuc.cheryme.top

[U102] JS：本地存储
来源：http://jek.yj20258.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://hch.gaohongyu789.top

[U103] JS：定时器
来源：http://qpl.jiagoushi.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://kmg.xylfe.cn

[U104] JS：防抖
来源：http://gth.pengpengdd.cyou

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://zpp.yvedp.cn

[U105] JS：节流
来源：http://icr.yuxming.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://mpu.ppjwa.cn

[U106] JS：日期格式化
来源：http://qpm.hongshengwenyu.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://ebj.fanxiaobao.xyz

[U107] JS：数字千分位
来源：http://kug.tian-w.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://pgy.vqdsnc.cn

[U108] JS：随机整数
来源：http://rym.birdmap.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://zed.yuxming.cn

[U109] JS：数组分组
来源：http://zhs.yongpay.top

Object.groupBy(arr, x => x.type)
来源：http://wqm.yueranfly.top

[U110] JS：数组分块
来源：http://mrd.cheryme.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://tmw.chenjidiqi.icu

[U111] JS：对象转 Map
来源：http://kvu.ctjpmb.com

new Map(Object.entries(obj))
来源：http://tlt.cucudq.cn

[U112] JS：字符串补位
来源：http://kvm.gotoacloud.top

"7".padStart(3, "0")
来源：http://trp.guowangkeji.top

[U113] JS：正则替换全部
来源：http://blm.316326.xyz

s.replaceAll("a", "b")
来源：http://byt.jiagoushi.top

[U114] JS：JSON 深比较
来源：http://dcv.mhx1999.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://dhu.hongshengwenyu.top

[U115] JS：生成 UUID
来源：http://hai.sjlbkw.cn

crypto.randomUUID()
来源：http://xca.316326.xyz

[U116] JS：类型检查（JSDoc）
来源：http://oer.ehwqpu.com

/** @param {string} name */ function f(name) {}
来源：http://ciz.52xcode.cn

[U117] JS：单元测试
来源：http://tco.yuanzhike.top

npm i -D vitest;  npx vitest
来源：http://rnv.shanyushiyangkeji.top

[U118] JS：开发服务器
来源：http://dmo.sysykeji.top

npm i -D vite;  npx vite
来源：http://fof.tianlin.xyz

[U119] JS：生产构建
来源：http://keo.fktsv.cn

npx vite build
来源：http://rej.daxiang520.top

[U120] JS：读取环境变量（Vite）
来源：http://vly.snrcjt.cn

import.meta.env.VITE_API_URL
来源：http://ded.jqgufenzy.top


<!-- 参考信息 -->