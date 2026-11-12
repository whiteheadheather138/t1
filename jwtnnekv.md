代发 wailian999

[T33] Lua：表（数组）
来源：http://tlz.tian-w.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://hyp.gzhubu.top

[T34] Lua：遍历表
来源：http://dbk.pycfn.com

for i, v in ipairs(t) do print(i, v) end
来源：http://iax.tanke756.top

[T35] Lua：字典表
来源：http://hux.zhongyouzk.top

local d = { a = 1 };  d.b = 2
来源：http://quy.epnwcf.com

[T36] Lua：函数
来源：http://zaj.hysaishi.cn

function add(a, b) return a + b end
来源：http://hxx.haohaochexian.top

[T37] Lua：字符串拼接
来源：http://uci.bbcook.cn

"a" .. "b"
来源：http://wbk.shangyingyoupin.top

[T38] Lua：条件
来源：http://ird.dianchejie.cn

if x > 0 then print("正") end
来源：http://eiw.vehdjk.com

[T39] Lua：模式匹配
来源：http://rao.chenzaomai.com

string.find(s, "%d+")
来源：http://enn.sufxvd.cn

[T40] Lua：元表
来源：http://iqh.jiagoushi.top

setmetatable({}, { __index = base })
来源：http://wna.shanyushiyangkeji.top

[T41] Perl：Hello World
来源：http://qsd.hongshengwenyu.top

print "Hello\n";
来源：http://bpz.svipenyu.cn

[T42] Perl：变量类型
来源：http://hom.ctjpmb.com

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://oae.cashguo.top

[T43] Perl：字符串插值
来源：http://wdu.yanxiufei.cn

"值: $a"
来源：http://czi.zycfv.cn

[T44] Perl：条件
来源：http://ico.hysaishi.cn

if ($a > 0) { print "正"; }
来源：http://dzj.sxryk.cn

[T45] Perl：数组遍历
来源：http://qrp.feifeiyinyue.top

for my $x (@arr) { print $x; }
来源：http://svy.nanxuanxn.top

[T46] Perl：哈希操作
来源：http://wqc.havefunace.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://iyx.hnqzz.top

[T47] Perl：正则捕获
来源：http://ymy.yueranfly.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://izp.fengsongda.top

[T48] Perl：正则替换
来源：http://adz.yuxming.cn

$s =~ s/old/new/g;
来源：http://ken.yj202588.top

[T49] Perl：函数
来源：http://uql.cdnleiting.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://zhp.c1oappe.top

[T50] Perl：逐行读文件
来源：http://vdi.sweek.top

open my $fh, "<", "a.txt" or die $!;
来源：http://ijs.chenlongwang.top

while (my $line = <$fh>) { print $line; }
来源：http://lsd.hcnkem.com

[T51] Scala：Hello World
来源：http://tmq.9152youxi.cn

println("Hello")
来源：http://wrz.svipenyu.cn

[T52] Scala：变量
来源：http://crw.c1oappe.top

val a = 1;  var b = 2
来源：http://lef.haohaochexian.top

[T53] Scala：字符串插值
来源：http://baw.jinghuilouyu.cn

s"值: $b"
来源：http://nha.zdbjq.cn

[T54] Scala：集合映射
来源：http://opc.tanke756.top

List(1, 2, 3).map(_ * 2)
来源：http://dlk.52xcode.cn

[T55] Scala：集合过滤
来源：http://awe.hysaishi.cn

List(1, 2, 3).filter(_ > 1)
来源：http://anw.iojbl.cn

[T56] Scala：样例类
来源：http://ulg.hesvh.cn

case class User(name: String, age: Int)
来源：http://nlk.bjfxy.top

[T57] Scala：模式匹配
来源：http://ptn.fanxiaobao.xyz

x match { case 1 => "一"; case _ => "其他" }
来源：http://eeg.fehbvm.com

[T58] Scala：函数定义
来源：http://xvd.316326.xyz

def add(a: Int, b: Int): Int = a + b
来源：http://ioc.jiagoushi.top

[T59] Scala：循环
来源：http://hlv.gzhubu.top

for (i <- 1 to 10) println(i)
来源：http://gez.yangfankeji.com

[T60] Scala：折叠
来源：http://kcz.shzxlz.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://nsf.tian-w.cn

================================================================================
来源：http://yxv.yj20258888.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://sql.yanxiufei.cn

================================================================================
来源：http://zeg.bjfxy.top

[U01] Py：创建虚拟环境
来源：http://svd.sufxvd.cn

python -m venv .venv && source .venv/bin/activate
来源：http://sgy.nanxuanxn.top

[U02] Py：导出 / 安装依赖
来源：http://ahx.gotoacloud.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://csp.jqgufenzy.top

[U03] Py：加载 .env 配置
来源：http://trz.vqdsnc.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://gcn.andypj.xyz

[U04] Py：变量调试打印
来源：http://ild.birdmap.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://aqr.zhaomingkeji.xyz

[U05] Py：列表去重且保序
来源：http://nrv.zhiwuduotai.top

list(dict.fromkeys(arr))
来源：http://ymx.zhoulong.xyz

[U06] Py：合并两个字典
来源：http://ial.jlsjyb.cn

{**a, **b}
来源：http://nud.fehbvm.com

[U07] Py：反转字典键值
来源：http://xfc.nanxinkj.top

{v: k for k, v in d.items()}
来源：http://jir.redwolf501.top

[U08] Py：展平二维列表
来源：http://zmy.aibaodan.cn

[y for x in nested for y in x]
来源：http://bfl.guannengcc.top

[U09] Py：字典取最大值的键
来源：http://uig.hfpthk.cn

max(d, key=d.get)
来源：http://fto.kuanghao11.cn

[U10] Py：按值排序字典
来源：http://nnu.hywenlv.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://yvw.ybcxt.top

[U11] Py：生成器表达式
来源：http://kox.nanxuanxn.top

(x * 2 for x in arr)
来源：http://see.shzxlz.cn

[U12] Py：取出现最多的 3 个元素
来源：http://irn.zhoulong.xyz

Counter(arr).most_common(3)
来源：http://yxu.yuanzhike.top

[U13] Py：固定长度队列
来源：http://wjo.hnqzz.top

deque(maxlen=10)
来源：http://ugy.hywenlv.cn

[U14] Py：分组收集到列表
来源：http://kqq.guowangkeji.top

defaultdict(list)
来源：http://iyk.zhijiandao.cn

[U15] Py：高精度计时
来源：http://sol.zhongyouzk.top

t = time.perf_counter()
来源：http://bhx.cashguo.top

[U16] Py：命令行参数解析
来源：http://sdd.fanxiaobao.xyz

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://nin.quarkkingdee.top

[U17] Py：初始化日志
来源：http://cuh.zhengqikj.top

logging.basicConfig(level=logging.INFO)
来源：http://mys.tianlin.xyz

[U18] Py：预编译正则
来源：http://sex.hongshengwenyu.top

pat = re.compile(r"\d+")
来源：http://mpg.zhijiandao.cn

[U19] Py：正则替换带回调
来源：http://yui.jinqigfzy.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://xbq.jyoumei.cn

[U20] Py：缓存函数结果
来源：http://glv.nanxinkj.top

@functools.lru_cache(maxsize=None)
来源：http://cru.316326.xyz

[U21] Py：自定义上下文管理器
来源：http://djf.cqqwz.cn

@contextlib.contextmanager
来源：http://nav.tarul.cn

[U22] Py：矩阵转置
来源：http://inj.fehbvm.com

list(zip(*m))
来源：http://fst.svipenyu.cn

[U23] Py：分块读取大文件
来源：http://ydi.yj202588.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://cub.zdbjq.cn

[U24] Py：路径操作
来源：http://tcz.bbcook.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://fjr.gotoacloud.top

[U25] Py：CSV 按字典读
来源：http://fdo.gogol.net.cn

csv.DictReader(f)
来源：http://wyo.zhijiandao.cn

[U26] Py：并发下载
来源：http://hxg.bbcook.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://ubj.316326.xyz

[U27] Py：异步 HTTP
来源：http://khi.yfazqb.com

aiohttp.ClientSession() 配合 async with
来源：http://vyr.sysykeji.top

[U28] Py：类型别名
来源：http://afr.9152youxi.cn

UserId = int
来源：http://qez.shzxlz.cn

[U29] Py：属性校验
来源：http://caq.aizwys.cn

@property 与 @x.setter 配合
来源：http://tdq.gzhubu.top

[U30] Py：数据类
来源：http://fea.ehwqpu.com

@dataclass(slots=True)
来源：http://uyz.cdnleiting.top

[U31] Py：单测
来源：http://peu.zhongyouzk.top

python -m pytest -q
来源：http://msv.redwolf501.top

[U32] Py：代码格式化
来源：http://pih.feifeiyinyue.top

ruff format . && ruff check --fix .
来源：http://rwb.aizwys.cn

[U33] Py：打包发布
来源：http://qon.xylfe.cn

python -m build  （依赖 pyproject.toml）
来源：http://zrv.aibaodan.cn

[U34] Py：判断编码
来源：http://qyi.meibo888.top

chardet.detect(raw)
来源：http://yra.jyoumei.cn

[U35] Py：发送邮件
来源：http://fno.wangdashe.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://lfo.vehdjk.com

[U36] Py：定时任务
来源：http://rpg.hnqzz.top

schedule.every(10).minutes.do(job)
来源：http://eaz.xinyue.icu

[U37] Py：读写 Excel
来源：http://suc.0kj1m.cn

pandas.read_excel / DataFrame.to_excel
来源：http://oqo.tian-w.cn

[U38] Py：获取脚本所在目录
来源：http://uea.yongpay.top

Path(__file__).resolve().parent
来源：http://guz.nwbrower.top

[U39] Py：判断是否在交互环境
来源：http://fpa.pengpengdd.cyou

sys.stdout.isatty()
来源：http://ihx.haohaochexian.top

[U40] Py：打印到标准错误
来源：http://tmo.havefunace.top

print("err", file=sys.stderr)
来源：http://wtr.hammf.cn

[U41] PHP：初始化 Composer 项目
来源：http://jxx.zhijiandao.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://sgo.sjlbkw.cn

[U42] PHP：PSR-4 自动加载
来源：http://iup.aizwys.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://sbs.hongshengwenyu.top

[U43] PHP：声明命名空间
来源：http://rpf.svipenyu.cn

namespace App\Http;
来源：http://zlg.jiagoushi.top

[U44] PHP：开启严格类型
来源：http://ztq.sjlbkw.cn

declare(strict_types=1);
来源：http://efm.yvedp.cn

[U45] PHP：类型声明与返回类型
来源：http://tkh.jqgufenzy.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://kka.vqdsnc.cn

[U46] PHP：可空类型
来源：http://hjw.pengpengdd.cyou

?string $name = null
来源：http://jyh.xinyue.icu

[U47] PHP：联合类型
来源：http://qms.52xcode.cn

int|string $id
来源：http://fna.yfazqb.com

[U48] PHP：纯枚举
来源：http://zaq.hcnkem.com

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://imp.sxryk.cn

[U49] PHP：只读属性
来源：http://mcb.jlsjyb.cn

public readonly string $name
来源：http://kus.andypj.xyz

[U50] PHP：构造器属性提升
来源：http://yzv.cheryme.top

public function __construct(private int $id) {}
来源：http://sef.xylfe.cn

[U51] PHP：数组解构
来源：http://sja.jqgfzy.top

[$a, $b] = $arr;
来源：http://bxq.smart0.xyz

[U52] PHP：箭头函数
来源：http://cdl.pycfn.com

$double = fn($x) => $x * 2;
来源：http://wvo.zhengqikj.top

[U53] PHP：空合并运算符
来源：http://foo.guannengcc.top

$v = $a ?? $b ?? "default";
来源：http://qof.birdmap.top

[U54] PHP：空安全调用
来源：http://snq.fehbvm.com

$obj?->method()
来源：http://efn.hfpthk.cn

[U55] PHP：match 表达式
来源：http://bpf.fanxiaobao.xyz

$s = match($x) { 1 => "一", default => "其他" };
来源：http://exj.shuidangran.top

[U56] PHP：命名参数
来源：http://rri.ydjk.org.cn

f(a: 1, b: 2)
来源：http://rba.nwbrower.top

[U57] PHP：字符串插值
来源：http://win.tarul.cn

"值: {$a}"
来源：http://nll.birdmap.top

[U58] PHP：数组三件套
来源：http://weg.zhixingplan.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://htm.yangfankeji.com

[U59] PHP：自定义排序
来源：http://pqm.xinyue.icu

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://rfg.zhoulong.xyz

[U60] PHP：JSON 编解码
来源：http://ygz.tian-w.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://myb.hesvh.cn

[U61] PHP：正则
来源：http://svp.jinyuanbaomall.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://jkj.yuxming.cn

[U62] PHP：日期对象
来源：http://mfv.gaohongyu789.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hvo.hammf.cn

[U63] PHP：文件读写
来源：http://qcd.jinqigufen.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://ypp.yuxming.cn

[U64] PHP：目录遍历
来源：http://rtq.mhx1999.top

glob("dir/*.php");  scandir("dir");
来源：http://eap.hfpthk.cn

[U65] PHP：会话
来源：http://kof.ivvv.top

session_start();  $_SESSION["uid"] = 1;
来源：http://rjj.vehdjk.com

[U66] PHP：设置 Cookie
来源：http://rud.tianlin.xyz

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://cwy.mhx1999.top

[U67] PHP：处理文件上传
来源：http://hst.nwbrower.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://qsc.ydjk.org.cn

[U68] PHP：PDO 连接
来源：http://sxy.shangyingyoupin.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://pta.gzhubu.top

[U69] PHP：PDO 预处理
来源：http://nia.hnxiangtu.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://ypa.yj20258.top

[U70] PHP：PDO 事务
来源：http://ncc.nwbrower.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://mnm.sweek.top

[U71] PHP：抛出异常
来源：http://ies.shuidangran.top

throw new RuntimeException("失败", 500);
来源：http://sjz.gzhubu.top

[U72] PHP：写错误日志
来源：http://ibj.cheryme.top

error_log("失败: " . $e->getMessage());
来源：http://xgx.daria6918.cn

[U73] PHP：读取 ini 配置
来源：http://kfm.ybcxt.top

parse_ini_file("config.ini", true)
来源：http://owl.wangdashe.top

[U74] PHP：读取环境变量
来源：http://fwu.guannengcc.top

getenv("APP_ENV") ?: "production"
来源：http://wyx.gogol.net.cn

[U75] PHP：依赖注入
来源：http://ysf.jinqigufen.top

composer require psr/container
来源：http://sgz.hysaishi.cn

[U76] PHP：简单路由
来源：http://pph.bjfxy.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://dja.c1oappe.top

[U77] PHP：模板渲染
来源：http://sue.shzxlz.cn

composer require twig/twig
来源：http://nzk.sweek.top

[U78] PHP：单元测试
来源：http://tgc.jyoumei.cn

composer require --dev phpunit/phpunit
来源：http://pqu.hammf.cn

[U79] PHP：静态分析
来源：http://mtl.zhoulong.xyz

composer require --dev phpstan/phpstan
来源：http://zft.zhongyouzk.top

[U80] PHP：代码规范修复
来源：http://nxy.ydjk.org.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://dvm.jiagoushi.top

[U81] JS：初始化项目
来源：http://hcw.xingfuxueyuan.xyz

npm init -y;  npm i express
来源：http://vkm.zhijiandao.cn

[U82] JS：package.json 脚本
来源：http://ars.zhiwuduotai.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://gqz.cdnleiting.top

[U83] JS：ES Module 导入导出
来源：http://doe.quarkkingdee.top

export const a = 1;  import { a } from "./m.js";
来源：http://rlw.tanke756.top

[U84] JS：CommonJS 写法
来源：http://zqb.tarul.cn

module.exports = { a };  const { a } = require("./m");
来源：http://pqf.sweek.top

[U85] JS：可选链
来源：http://xft.wangdashe.top

a?.b?.c
来源：http://yvk.uphjek.com

[U86] JS：空值合并
来源：http://lnd.ctjpmb.com

a ?? b
来源：http://txl.hnqzz.top

[U87] JS：解构默认值
来源：http://ggw.hesvh.cn

const { a = 1, b = 2 } = obj;
来源：http://qoa.snrcjt.cn

[U88] JS：对象展开合并
来源：http://ngy.zhiwuduotai.top

{ ...a, ...b }
来源：http://xtj.cheryme.top

[U89] JS：数组去重
来源：http://gvw.vehdjk.com

[...new Set(arr)]
来源：http://ghu.wangshuangyany.cn

[U90] JS：数字数组排序
来源：http://cnk.iojbl.cn

[...arr].sort((a, b) => a - b)
来源：http://huh.hysaishi.cn

[U91] JS：对象键值遍历
来源：http://ihk.hysaishi.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://sfz.hongshengwenyu.top

[U92] JS：深拷贝
来源：http://aps.yangfankeji.com

structuredClone(obj)
来源：http://nka.zhengqikj.top

[U93] JS：模板字符串
来源：http://xml.yonumen.top

`共 ${n} 条`
来源：http://xae.zhijiandao.cn

[U94] JS：箭头函数
来源：http://mqe.0kj1m.cn

const double = x => x * 2;
来源：http://ext.ybcxt.top

[U95] JS：Promise 包装
来源：http://zyx.zhixingplan.top

new Promise((resolve, reject) => {})
来源：http://ray.0kj1m.cn

[U96] JS：async/await 与异常
来源：http://fyt.daria6918.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://vjs.jqgfzy.top

[U97] JS：并发请求
来源：http://bin.ppjwa.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://knu.jyoumei.cn

[U98] JS：fetch 带 JSON
来源：http://vxx.fanxiaobao.xyz

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://xpi.chenlongwang.top

[U99] JS：事件监听
来源：http://frh.jlsjyb.cn

el.addEventListener("click", e => {})
来源：http://lop.jinqigfzy.top

[U100] JS：DOM 查询
来源：http://oyf.yuanzhike.top

document.querySelector(".item")
来源：http://cxf.vqdsnc.cn

[U101] JS：classList 操作
来源：http://con.shuidangran.top

el.classList.toggle("active")
来源：http://lgy.jqgfzy.top

[U102] JS：本地存储
来源：http://smc.zycfv.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://ije.316326.xyz

[U103] JS：定时器
来源：http://jmz.ctjpmb.com

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://fpr.fengsongda.top

[U104] JS：防抖
来源：http://orb.birdmap.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ugw.shzxlz.cn

[U105] JS：节流
来源：http://thm.hnqzz.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://uah.tian-w.cn

[U106] JS：日期格式化
来源：http://pfi.guowangkeji.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://wjt.zhengqikj.top

[U107] JS：数字千分位
来源：http://zpj.0kj1m.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://bzg.shanyushiyangtech.top

[U108] JS：随机整数
来源：http://aef.zdbjq.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://qdn.hfpthk.cn

[U109] JS：数组分组
来源：http://wav.tarul.cn

Object.groupBy(arr, x => x.type)
来源：http://giq.snrcjt.cn

[U110] JS：数组分块
来源：http://bim.pycfn.com

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://wph.zhijiandao.cn

[U111] JS：对象转 Map
来源：http://vmv.cheryme.top

new Map(Object.entries(obj))
来源：http://ads.fengsongda.top

[U112] JS：字符串补位
来源：http://rhs.nanxinkj.top

"7".padStart(3, "0")
来源：http://irq.cdnleiting.top

[U113] JS：正则替换全部
来源：http://mfg.shzxlz.cn

s.replaceAll("a", "b")
来源：http://jls.shanyushiyangtech.top

[U114] JS：JSON 深比较
来源：http://luh.aizwys.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://dpc.hywenlv.cn

[U115] JS：生成 UUID
来源：http://rsu.hammf.cn

crypto.randomUUID()
来源：http://vzj.redwolf501.top

[U116] JS：类型检查（JSDoc）
来源：http://nnd.hammf.cn

/** @param {string} name */ function f(name) {}
来源：http://wqf.chenzaomai.com

[U117] JS：单元测试
来源：http://nge.meibo888.top

npm i -D vitest;  npx vitest
来源：http://jxo.aibaodan.cn

[U118] JS：开发服务器
来源：http://rhe.shuidangran.top

npm i -D vite;  npx vite
来源：http://vvu.ppjwa.cn

[U119] JS：生产构建
来源：http://pzz.hfpthk.cn

npx vite build
来源：http://kaa.aibaodan.cn

[U120] JS：读取环境变量（Vite）
来源：http://jua.shangyingyoupin.top

import.meta.env.VITE_API_URL
来源：http://tbk.feifeiyinyue.top


<!-- 参考信息 -->