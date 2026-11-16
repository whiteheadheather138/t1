代发 wailian999

[T31] Lua：Hello World
来源：http://wya.andypj.xyz

print("Hello")
来源：http://wcm.wangshuangyany.cn

[T32] Lua：局部变量
来源：http://ysi.xylfe.cn

local a = 1
来源：http://vhu.gzhubu.top

[T33] Lua：表（数组）
来源：http://tuy.andypj.xyz

local t = {1, 2, 3};  t[4] = 4
来源：http://dbs.ywan-chungtsiang.top

[T34] Lua：遍历表
来源：http://act.wangshuangyany.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://myt.cdnleiting.top

[T35] Lua：字典表
来源：http://dkz.yongpay.top

local d = { a = 1 };  d.b = 2
来源：http://vuq.jlsjyb.cn

[T36] Lua：函数
来源：http://dyd.ppjwa.cn

function add(a, b) return a + b end
来源：http://cer.zycfv.cn

[T37] Lua：字符串拼接
来源：http://evp.yongpay.top

"a" .. "b"
来源：http://dnf.snrcjt.cn

[T38] Lua：条件
来源：http://ijr.hesvh.cn

if x > 0 then print("正") end
来源：http://iwx.nanxuanxn.top

[T39] Lua：模式匹配
来源：http://dcp.yueranfly.top

string.find(s, "%d+")
来源：http://wzu.jinqigufen.top

[T40] Lua：元表
来源：http://eik.c1oappe.top

setmetatable({}, { __index = base })
来源：http://kws.ehwqpu.com

[T41] Perl：Hello World
来源：http://lfg.vehdjk.com

print "Hello\n";
来源：http://hip.ywan-chungtsiang.top

[T42] Perl：变量类型
来源：http://qdx.hesvh.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://xxn.xylfe.cn

[T43] Perl：字符串插值
来源：http://cdk.xziqi.cn

"值: $a"
来源：http://chp.52xcode.cn

[T44] Perl：条件
来源：http://kfu.pycfn.com

if ($a > 0) { print "正"; }
来源：http://xgf.zhoulong.xyz

[T45] Perl：数组遍历
来源：http://zxc.sysykeji.top

for my $x (@arr) { print $x; }
来源：http://uds.jinqigfzy.top

[T46] Perl：哈希操作
来源：http://ukr.yj20258.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://iqs.jinghuilouyu.cn

[T47] Perl：正则捕获
来源：http://uri.xuetiantiany.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://gyd.xylfe.cn

[T48] Perl：正则替换
来源：http://gxn.zhixingplan.top

$s =~ s/old/new/g;
来源：http://gfr.sxryk.cn

[T49] Perl：函数
来源：http://kja.shangyingyoupin.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://oga.nanxinkj.top

[T50] Perl：逐行读文件
来源：http://fnp.mhx1999.top

open my $fh, "<", "a.txt" or die $!;
来源：http://abc.c1oappe.top

while (my $line = <$fh>) { print $line; }
来源：http://mwg.fzhhl.top

[T51] Scala：Hello World
来源：http://emc.zhijiandao.cn

println("Hello")
来源：http://xsg.jlsjyb.cn

[T52] Scala：变量
来源：http://ybf.xuetiantiany.cn

val a = 1;  var b = 2
来源：http://mcs.wangshuangyany.cn

[T53] Scala：字符串插值
来源：http://qju.ctjpmb.com

s"值: $b"
来源：http://juz.jiagoushi.top

[T54] Scala：集合映射
来源：http://has.yueranfly.top

List(1, 2, 3).map(_ * 2)
来源：http://xzl.fehbvm.com

[T55] Scala：集合过滤
来源：http://xsh.zycfv.cn

List(1, 2, 3).filter(_ > 1)
来源：http://soy.dashuyun.cn

[T56] Scala：样例类
来源：http://kiy.zhengqikj.top

case class User(name: String, age: Int)
来源：http://hsd.sjlbkw.cn

[T57] Scala：模式匹配
来源：http://ume.jyoumei.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://xvq.cucudq.cn

[T58] Scala：函数定义
来源：http://hsg.xuanzx.com

def add(a: Int, b: Int): Int = a + b
来源：http://qcy.jlsjyb.cn

[T59] Scala：循环
来源：http://mqb.nanxuanxn.top

for (i <- 1 to 10) println(i)
来源：http://dpz.yj20258888.top

[T60] Scala：折叠
来源：http://vba.jlsjyb.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://woq.jinyuanbaomall.cn

================================================================================
来源：http://nde.hnqzz.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://jty.wangshuangyany.cn

================================================================================
来源：http://goh.quarkkingdee.top

[U01] Py：创建虚拟环境
来源：http://grd.kuanghao11.cn

python -m venv .venv && source .venv/bin/activate
来源：http://mjd.snrcjt.cn

[U02] Py：导出 / 安装依赖
来源：http://fpu.shanyushiyangkeji.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://xcx.ydzc1.top

[U03] Py：加载 .env 配置
来源：http://mrq.zycfv.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://lgv.hcnkem.com

[U04] Py：变量调试打印
来源：http://grj.andypj.xyz

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://nln.shanyushiyangtech.top

[U05] Py：列表去重且保序
来源：http://qmk.jyoumei.cn

list(dict.fromkeys(arr))
来源：http://hzv.vehdjk.com

[U06] Py：合并两个字典
来源：http://hna.xuanzx.com

{**a, **b}
来源：http://cel.xinyue.icu

[U07] Py：反转字典键值
来源：http://mlf.yanxiufei.cn

{v: k for k, v in d.items()}
来源：http://xqq.yongpay.top

[U08] Py：展平二维列表
来源：http://pdb.smart0.xyz

[y for x in nested for y in x]
来源：http://oqi.shuidangran.top

[U09] Py：字典取最大值的键
来源：http://ajm.snrcjt.cn

max(d, key=d.get)
来源：http://tni.zhixingplan.top

[U10] Py：按值排序字典
来源：http://rug.hysaishi.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://rnn.jinqigufen.top

[U11] Py：生成器表达式
来源：http://gpo.pycfn.com

(x * 2 for x in arr)
来源：http://fki.feifeiyinyue.top

[U12] Py：取出现最多的 3 个元素
来源：http://iyj.xylfe.cn

Counter(arr).most_common(3)
来源：http://iwq.yangfankeji.com

[U13] Py：固定长度队列
来源：http://wlg.52xcode.cn

deque(maxlen=10)
来源：http://wee.cheryme.top

[U14] Py：分组收集到列表
来源：http://ett.hcnkem.com

defaultdict(list)
来源：http://aia.0kj1m.cn

[U15] Py：高精度计时
来源：http://xrh.meibo888.top

t = time.perf_counter()
来源：http://lbw.hfpthk.cn

[U16] Py：命令行参数解析
来源：http://lbr.quarkkingdee.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://eqm.cdnleiting.top

[U17] Py：初始化日志
来源：http://uxh.sweek.top

logging.basicConfig(level=logging.INFO)
来源：http://adi.fengsongda.top

[U18] Py：预编译正则
来源：http://qeb.sweek.top

pat = re.compile(r"\d+")
来源：http://jkc.fehbvm.com

[U19] Py：正则替换带回调
来源：http://fjy.ppjwa.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://shu.xuetiantiany.cn

[U20] Py：缓存函数结果
来源：http://lbd.dashuyun.cn

@functools.lru_cache(maxsize=None)
来源：http://iff.quarkkingdee.top

[U21] Py：自定义上下文管理器
来源：http://ard.fzhhl.top

@contextlib.contextmanager
来源：http://xbn.kuanghao11.cn

[U22] Py：矩阵转置
来源：http://grj.gaohongyu789.top

list(zip(*m))
来源：http://iza.cashguo.top

[U23] Py：分块读取大文件
来源：http://kpb.jianghu66.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hps.jinqigfzy.top

[U24] Py：路径操作
来源：http://oqd.vqdsnc.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://zjs.vehdjk.com

[U25] Py：CSV 按字典读
来源：http://lkm.zhijiandao.cn

csv.DictReader(f)
来源：http://cnj.tianlin.xyz

[U26] Py：并发下载
来源：http://jpb.yonumen.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://pxw.hysaishi.cn

[U27] Py：异步 HTTP
来源：http://cko.gogol.net.cn

aiohttp.ClientSession() 配合 async with
来源：http://lkg.epnwcf.com

[U28] Py：类型别名
来源：http://sbz.hysaishi.cn

UserId = int
来源：http://ebk.sysykeji.top

[U29] Py：属性校验
来源：http://phm.sweek.top

@property 与 @x.setter 配合
来源：http://ago.hfpthk.cn

[U30] Py：数据类
来源：http://vyv.nanxinkj.top

@dataclass(slots=True)
来源：http://tsa.pycfn.com

[U31] Py：单测
来源：http://xrg.aizwys.cn

python -m pytest -q
来源：http://vnf.meibo888.top

[U32] Py：代码格式化
来源：http://rcw.jlsjyb.cn

ruff format . && ruff check --fix .
来源：http://ueo.chenjidiqi.icu

[U33] Py：打包发布
来源：http://bvm.hammf.cn

python -m build  （依赖 pyproject.toml）
来源：http://tuy.c1oappe.top

[U34] Py：判断编码
来源：http://ozx.52xcode.cn

chardet.detect(raw)
来源：http://otw.tian-w.cn

[U35] Py：发送邮件
来源：http://wki.jianghu66.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://rer.shangyingyoupin.top

[U36] Py：定时任务
来源：http://nnk.xuetiantiany.cn

schedule.every(10).minutes.do(job)
来源：http://ili.dashuyun.cn

[U37] Py：读写 Excel
来源：http://jhd.316326.xyz

pandas.read_excel / DataFrame.to_excel
来源：http://gvz.vqdsnc.cn

[U38] Py：获取脚本所在目录
来源：http://tow.chenjidiqi.icu

Path(__file__).resolve().parent
来源：http://tks.9152youxi.cn

[U39] Py：判断是否在交互环境
来源：http://bnr.hcnkem.com

sys.stdout.isatty()
来源：http://tbn.zhongyouzk.top

[U40] Py：打印到标准错误
来源：http://pdc.andypj.xyz

print("err", file=sys.stderr)
来源：http://tnq.feifeiyinyue.top

[U41] PHP：初始化 Composer 项目
来源：http://hss.yongpay.top

composer init;  composer require guzzlehttp/guzzle
来源：http://jwz.ehwqpu.com

[U42] PHP：PSR-4 自动加载
来源：http://mwm.smart0.xyz

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://uts.9152youxi.cn

[U43] PHP：声明命名空间
来源：http://usz.andypj.xyz

namespace App\Http;
来源：http://zln.yvedp.cn

[U44] PHP：开启严格类型
来源：http://xmj.ehwqpu.com

declare(strict_types=1);
来源：http://fir.dianchejie.cn

[U45] PHP：类型声明与返回类型
来源：http://ihu.yj202588.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://hvb.316326.xyz

[U46] PHP：可空类型
来源：http://ixg.zhoulong.xyz

?string $name = null
来源：http://jiq.jlsjyb.cn

[U47] PHP：联合类型
来源：http://icx.hesvh.cn

int|string $id
来源：http://rhd.snrcjt.cn

[U48] PHP：纯枚举
来源：http://zid.jqgufenzy.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://bbd.smart0.xyz

[U49] PHP：只读属性
来源：http://mkh.svipenyu.cn

public readonly string $name
来源：http://iut.pengpengdd.cyou

[U50] PHP：构造器属性提升
来源：http://mfc.yj20258888.top

public function __construct(private int $id) {}
来源：http://rar.jiagoushi.top

[U51] PHP：数组解构
来源：http://efr.fktsv.cn

[$a, $b] = $arr;
来源：http://bcx.feifeiyinyue.top

[U52] PHP：箭头函数
来源：http://vaf.xinyue.icu

$double = fn($x) => $x * 2;
来源：http://ivw.zycfv.cn

[U53] PHP：空合并运算符
来源：http://ofm.zdqjudy.top

$v = $a ?? $b ?? "default";
来源：http://vxu.tianlin.xyz

[U54] PHP：空安全调用
来源：http://pky.zdbjq.cn

$obj?->method()
来源：http://ojt.tianlin.xyz

[U55] PHP：match 表达式
来源：http://eyx.jlsjyb.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://ywx.meibo888.top

[U56] PHP：命名参数
来源：http://odx.yangfankeji.com

f(a: 1, b: 2)
来源：http://ytm.bjfxy.top

[U57] PHP：字符串插值
来源：http://uoy.havefunace.top

"值: {$a}"
来源：http://qll.c1oappe.top

[U58] PHP：数组三件套
来源：http://nyy.xingfuxueyuan.xyz

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://pzr.zhaomingkeji.xyz

[U59] PHP：自定义排序
来源：http://ust.c1oappe.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://qjd.shzxlz.cn

[U60] PHP：JSON 编解码
来源：http://lfm.yanxiufei.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://wqa.aizwys.cn

[U61] PHP：正则
来源：http://jcx.yfazqb.com

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://iyn.0kj1m.cn

[U62] PHP：日期对象
来源：http://rge.chenjidiqi.icu

(new DateTimeImmutable())->format("Y-m-d");
来源：http://ndy.ywan-chungtsiang.top

[U63] PHP：文件读写
来源：http://njg.ctjpmb.com

file_get_contents($f);  file_put_contents($f, $data);
来源：http://ocj.shuidangran.top

[U64] PHP：目录遍历
来源：http://dgb.pengpengdd.cyou

glob("dir/*.php");  scandir("dir");
来源：http://euu.9152youxi.cn

[U65] PHP：会话
来源：http://sql.zycfv.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://mvc.nanxuanxn.top

[U66] PHP：设置 Cookie
来源：http://gtm.zycfv.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://rxi.shzxlz.cn

[U67] PHP：处理文件上传
来源：http://rbp.jqgufenzy.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://cly.fengsongda.top

[U68] PHP：PDO 连接
来源：http://msb.ivvv.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://wwe.sufxvd.cn

[U69] PHP：PDO 预处理
来源：http://dpw.316326.xyz

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://son.yj20258.top

[U70] PHP：PDO 事务
来源：http://dnu.jinghuilouyu.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://oum.aibaodan.cn

[U71] PHP：抛出异常
来源：http://orp.dashuyun.cn

throw new RuntimeException("失败", 500);
来源：http://gur.jinqigufen.top

[U72] PHP：写错误日志
来源：http://fhc.smart0.xyz

error_log("失败: " . $e->getMessage());
来源：http://tfh.chenjidiqi.icu

[U73] PHP：读取 ini 配置
来源：http://zmb.haohaochexian.top

parse_ini_file("config.ini", true)
来源：http://tfc.mhx1999.top

[U74] PHP：读取环境变量
来源：http://tll.jqgufenzy.top

getenv("APP_ENV") ?: "production"
来源：http://oze.shuidangran.top

[U75] PHP：依赖注入
来源：http://hly.daria6918.cn

composer require psr/container
来源：http://gen.zhoulong.xyz

[U76] PHP：简单路由
来源：http://ymb.andypj.xyz

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://irk.hcnkem.com

[U77] PHP：模板渲染
来源：http://hle.yanxiufei.cn

composer require twig/twig
来源：http://rai.gaohongyu789.top

[U78] PHP：单元测试
来源：http://clq.zhoulong.xyz

composer require --dev phpunit/phpunit
来源：http://iaz.snrcjt.cn

[U79] PHP：静态分析
来源：http://hkl.jqgufenzy.top

composer require --dev phpstan/phpstan
来源：http://uos.ctjpmb.com

[U80] PHP：代码规范修复
来源：http://dim.shuidangran.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://kcj.cucudq.cn

[U81] JS：初始化项目
来源：http://joy.yfazqb.com

npm init -y;  npm i express
来源：http://vri.hongshengwenyu.top

[U82] JS：package.json 脚本
来源：http://rvg.yuanzhike.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://vvm.fengsongda.top

[U83] JS：ES Module 导入导出
来源：http://pqm.shzxlz.cn

export const a = 1;  import { a } from "./m.js";
来源：http://wwq.zhengqikj.top

[U84] JS：CommonJS 写法
来源：http://dtv.xingfuxueyuan.xyz

module.exports = { a };  const { a } = require("./m");
来源：http://mtr.yanxiufei.cn

[U85] JS：可选链
来源：http://puy.cucudq.cn

a?.b?.c
来源：http://doy.pengpengdd.cyou

[U86] JS：空值合并
来源：http://qud.svipenyu.cn

a ?? b
来源：http://kjj.pengpengdd.cyou

[U87] JS：解构默认值
来源：http://gwn.jinqigfzy.top

const { a = 1, b = 2 } = obj;
来源：http://cte.ctjpmb.com

[U88] JS：对象展开合并
来源：http://phi.xziqi.cn

{ ...a, ...b }
来源：http://tan.hnxiangtu.top

[U89] JS：数组去重
来源：http://rul.xingfuxueyuan.xyz

[...new Set(arr)]
来源：http://erb.xziqi.cn

[U90] JS：数字数组排序
来源：http://bxc.yvedp.cn

[...arr].sort((a, b) => a - b)
来源：http://ssr.yuxming.cn

[U91] JS：对象键值遍历
来源：http://lfr.jinghuilouyu.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://ixs.xuetiantiany.cn

[U92] JS：深拷贝
来源：http://uzs.sxryk.cn

structuredClone(obj)
来源：http://vmb.ywan-chungtsiang.top

[U93] JS：模板字符串
来源：http://qtz.hammf.cn

`共 ${n} 条`
来源：http://jms.cashguo.top

[U94] JS：箭头函数
来源：http://pao.fktsv.cn

const double = x => x * 2;
来源：http://pfw.snrcjt.cn

[U95] JS：Promise 包装
来源：http://vub.cdnleiting.top

new Promise((resolve, reject) => {})
来源：http://jov.0kj1m.cn

[U96] JS：async/await 与异常
来源：http://qkp.aizwys.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://mms.ctjpmb.com

[U97] JS：并发请求
来源：http://bee.yanxiufei.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://kpn.epnwcf.com

[U98] JS：fetch 带 JSON
来源：http://xma.aibaodan.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://ypo.shanyushiyangtech.top

[U99] JS：事件监听
来源：http://haj.cqqwz.cn

el.addEventListener("click", e => {})
来源：http://nzt.jianghu66.top

[U100] JS：DOM 查询
来源：http://okc.smart0.xyz

document.querySelector(".item")
来源：http://ptq.dianchejie.cn

[U101] JS：classList 操作
来源：http://tdn.shanyushiyangkeji.top

el.classList.toggle("active")
来源：http://rdv.ppjwa.cn

[U102] JS：本地存储
来源：http://xvs.cucudq.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://pgh.zdbjq.cn

[U103] JS：定时器
来源：http://rkw.shzxlz.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://dip.jinyuanbaomall.cn

[U104] JS：防抖
来源：http://yvd.yfazqb.com

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://kmv.yuanzhike.top

[U105] JS：节流
来源：http://dyw.52xcode.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://yeo.aibaodan.cn

[U106] JS：日期格式化
来源：http://wbo.yvedp.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://mej.uphjek.com

[U107] JS：数字千分位
来源：http://nwu.zdbjq.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://ywf.tian-w.cn

[U108] JS：随机整数
来源：http://gur.zhiwuduotai.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://msw.sysykeji.top

[U109] JS：数组分组
来源：http://bnr.andypj.xyz

Object.groupBy(arr, x => x.type)
来源：http://cgk.0kj1m.cn

[U110] JS：数组分块
来源：http://vuc.ivvv.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://zmm.yonumen.top

[U111] JS：对象转 Map
来源：http://jao.xuetiantiany.cn

new Map(Object.entries(obj))
来源：http://zua.yongpay.top

[U112] JS：字符串补位
来源：http://byh.kuanghao11.cn

"7".padStart(3, "0")
来源：http://tki.zhijiandao.cn

[U113] JS：正则替换全部
来源：http://mpy.ppjwa.cn

s.replaceAll("a", "b")
来源：http://rag.yj20258888.top

[U114] JS：JSON 深比较
来源：http://qht.sweek.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://vmi.zhengqikj.top

[U115] JS：生成 UUID
来源：http://knm.iojbl.cn

crypto.randomUUID()
来源：http://mol.cashguo.top

[U116] JS：类型检查（JSDoc）
来源：http://kfs.snrcjt.cn

/** @param {string} name */ function f(name) {}
来源：http://iyq.zhaomingkeji.xyz

[U117] JS：单元测试
来源：http://bdn.yj20258.top

npm i -D vitest;  npx vitest
来源：http://huv.hongshengwenyu.top

[U118] JS：开发服务器
来源：http://flt.fengsongda.top

npm i -D vite;  npx vite
来源：http://jxq.ydjk.org.cn


<!-- 参考信息 -->