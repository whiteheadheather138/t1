代发 wailian999

[T33] Lua：表（数组）
来源：http://flz.sjlbkw.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://etg.fehbvm.com

[T34] Lua：遍历表
来源：http://ijk.ivvv.top

for i, v in ipairs(t) do print(i, v) end
来源：http://owr.cheryme.top

[T35] Lua：字典表
来源：http://dhf.gogol.net.cn

local d = { a = 1 };  d.b = 2
来源：http://fnf.jiagoushi.top

[T36] Lua：函数
来源：http://zoh.aibaodan.cn

function add(a, b) return a + b end
来源：http://dav.shangyingyoupin.top

[T37] Lua：字符串拼接
来源：http://vid.sxryk.cn

"a" .. "b"
来源：http://rqx.dianchejie.cn

[T38] Lua：条件
来源：http://gug.mhx1999.top

if x > 0 then print("正") end
来源：http://czt.fengsongda.top

[T39] Lua：模式匹配
来源：http://kvw.yj20258888.top

string.find(s, "%d+")
来源：http://vtd.cdnleiting.top

[T40] Lua：元表
来源：http://nhw.vqdsnc.cn

setmetatable({}, { __index = base })
来源：http://lgq.shuidangran.top

[T41] Perl：Hello World
来源：http://efg.shzxlz.cn

print "Hello\n";
来源：http://lnd.yfazqb.com

[T42] Perl：变量类型
来源：http://cub.iojbl.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://cti.tian-w.cn

[T43] Perl：字符串插值
来源：http://ytt.yuxming.cn

"值: $a"
来源：http://gdm.jinqigfzy.top

[T44] Perl：条件
来源：http://edi.hnxiangtu.top

if ($a > 0) { print "正"; }
来源：http://sfy.jinqigfzy.top

[T45] Perl：数组遍历
来源：http://dxf.hysaishi.cn

for my $x (@arr) { print $x; }
来源：http://fgx.hywenlv.cn

[T46] Perl：哈希操作
来源：http://err.havefunace.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://jyx.shzxlz.cn

[T47] Perl：正则捕获
来源：http://fmk.nanxuanxn.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://oiw.haohaochexian.top

[T48] Perl：正则替换
来源：http://hit.gotoacloud.top

$s =~ s/old/new/g;
来源：http://san.jyoumei.cn

[T49] Perl：函数
来源：http://wkn.jiagoushi.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://wxp.aizwys.cn

[T50] Perl：逐行读文件
来源：http://thh.smart0.xyz

open my $fh, "<", "a.txt" or die $!;
来源：http://pat.daxiang520.top

while (my $line = <$fh>) { print $line; }
来源：http://vqd.hfpthk.cn

[T51] Scala：Hello World
来源：http://gjq.0kj1m.cn

println("Hello")
来源：http://vpc.cheryme.top

[T52] Scala：变量
来源：http://wgm.zdqjudy.top

val a = 1;  var b = 2
来源：http://tar.shzxlz.cn

[T53] Scala：字符串插值
来源：http://qkf.birdmap.top

s"值: $b"
来源：http://owz.yuanzhike.top

[T54] Scala：集合映射
来源：http://jns.yj20258888.top

List(1, 2, 3).map(_ * 2)
来源：http://coo.fanxiaobao.xyz

[T55] Scala：集合过滤
来源：http://wue.daria6918.cn

List(1, 2, 3).filter(_ > 1)
来源：http://wno.sufxvd.cn

[T56] Scala：样例类
来源：http://glp.guowangkeji.top

case class User(name: String, age: Int)
来源：http://dqq.jinghuilouyu.cn

[T57] Scala：模式匹配
来源：http://xmq.bjfxy.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://dbl.hcnkem.com

[T58] Scala：函数定义
来源：http://fon.feifeiyinyue.top

def add(a: Int, b: Int): Int = a + b
来源：http://piw.zdbjq.cn

[T59] Scala：循环
来源：http://jco.havefunace.top

for (i <- 1 to 10) println(i)
来源：http://eun.ppjwa.cn

[T60] Scala：折叠
来源：http://ofh.vqdsnc.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://ukn.mhx1999.top

================================================================================
来源：http://rkw.yj20258.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://kpj.yj20258.top

================================================================================
来源：http://tav.birdmap.top

[U01] Py：创建虚拟环境
来源：http://bkv.sjlbkw.cn

python -m venv .venv && source .venv/bin/activate
来源：http://wpw.0kj1m.cn

[U02] Py：导出 / 安装依赖
来源：http://inp.hnxiangtu.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://thb.vqdsnc.cn

[U03] Py：加载 .env 配置
来源：http://tev.mhx1999.top

from dotenv import load_dotenv; load_dotenv()
来源：http://nen.316326.xyz

[U04] Py：变量调试打印
来源：http://axf.quarkkingdee.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://aun.pengpengdd.cyou

[U05] Py：列表去重且保序
来源：http://xoh.fengsongda.top

list(dict.fromkeys(arr))
来源：http://rhk.xuanzx.com

[U06] Py：合并两个字典
来源：http://iel.sweek.top

{**a, **b}
来源：http://knx.fktsv.cn

[U07] Py：反转字典键值
来源：http://hvr.vehdjk.com

{v: k for k, v in d.items()}
来源：http://nwd.guannengcc.top

[U08] Py：展平二维列表
来源：http://emo.xingfuxueyuan.xyz

[y for x in nested for y in x]
来源：http://lok.epnwcf.com

[U09] Py：字典取最大值的键
来源：http://ghw.redwolf501.top

max(d, key=d.get)
来源：http://flv.nanxinkj.top

[U10] Py：按值排序字典
来源：http://gjz.cheryme.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://ryi.kuanghao11.cn

[U11] Py：生成器表达式
来源：http://qmh.pycfn.com

(x * 2 for x in arr)
来源：http://fck.yonumen.top

[U12] Py：取出现最多的 3 个元素
来源：http://mny.tianlin.xyz

Counter(arr).most_common(3)
来源：http://urw.bjfxy.top

[U13] Py：固定长度队列
来源：http://yjr.hcnkem.com

deque(maxlen=10)
来源：http://bgs.sufxvd.cn

[U14] Py：分组收集到列表
来源：http://fiu.hysaishi.cn

defaultdict(list)
来源：http://szu.jqgfzy.top

[U15] Py：高精度计时
来源：http://nyn.andypj.xyz

t = time.perf_counter()
来源：http://zwi.yj20258888.top

[U16] Py：命令行参数解析
来源：http://ylg.ppjwa.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://dbm.gaohongyu789.top

[U17] Py：初始化日志
来源：http://xdk.zdqjudy.top

logging.basicConfig(level=logging.INFO)
来源：http://vex.jqgfzy.top

[U18] Py：预编译正则
来源：http://kzv.aizwys.cn

pat = re.compile(r"\d+")
来源：http://snb.dashuyun.cn

[U19] Py：正则替换带回调
来源：http://wvf.daxiang520.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://ucr.chenjidiqi.icu

[U20] Py：缓存函数结果
来源：http://fpf.zhongyouzk.top

@functools.lru_cache(maxsize=None)
来源：http://caw.jqgfzy.top

[U21] Py：自定义上下文管理器
来源：http://jff.nanxuanxn.top

@contextlib.contextmanager
来源：http://qly.birdmap.top

[U22] Py：矩阵转置
来源：http://tje.aibaodan.cn

list(zip(*m))
来源：http://tkc.hcnkem.com

[U23] Py：分块读取大文件
来源：http://kkb.fktsv.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://mbz.fengsongda.top

[U24] Py：路径操作
来源：http://csz.yfazqb.com

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://zvi.sweek.top

[U25] Py：CSV 按字典读
来源：http://thn.shzxlz.cn

csv.DictReader(f)
来源：http://cwh.jyoumei.cn

[U26] Py：并发下载
来源：http://psy.sysykeji.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://itq.tianlin.xyz

[U27] Py：异步 HTTP
来源：http://uws.cashguo.top

aiohttp.ClientSession() 配合 async with
来源：http://kli.haohaochexian.top

[U28] Py：类型别名
来源：http://oyw.gotoacloud.top

UserId = int
来源：http://xwy.cqqwz.cn

[U29] Py：属性校验
来源：http://pfu.iojbl.cn

@property 与 @x.setter 配合
来源：http://pkh.zhoulong.xyz

[U30] Py：数据类
来源：http://cse.jinyuanbaomall.cn

@dataclass(slots=True)
来源：http://arj.uphjek.com

[U31] Py：单测
来源：http://erz.zhaomingkeji.xyz

python -m pytest -q
来源：http://qpx.hywenlv.cn

[U32] Py：代码格式化
来源：http://shm.uphjek.com

ruff format . && ruff check --fix .
来源：http://czt.guannengcc.top

[U33] Py：打包发布
来源：http://gqw.sweek.top

python -m build  （依赖 pyproject.toml）
来源：http://ioc.sweek.top

[U34] Py：判断编码
来源：http://rvp.hnxiangtu.top

chardet.detect(raw)
来源：http://eom.fengsongda.top

[U35] Py：发送邮件
来源：http://cpj.uphjek.com

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://lui.vehdjk.com

[U36] Py：定时任务
来源：http://fej.hongshengwenyu.top

schedule.every(10).minutes.do(job)
来源：http://pec.jinqigfzy.top

[U37] Py：读写 Excel
来源：http://yhu.yuanzhike.top

pandas.read_excel / DataFrame.to_excel
来源：http://uvn.chenlongwang.top

[U38] Py：获取脚本所在目录
来源：http://dow.pengpengdd.cyou

Path(__file__).resolve().parent
来源：http://vgz.uphjek.com

[U39] Py：判断是否在交互环境
来源：http://pvg.sufxvd.cn

sys.stdout.isatty()
来源：http://osj.bbcook.cn

[U40] Py：打印到标准错误
来源：http://xfm.sweek.top

print("err", file=sys.stderr)
来源：http://khz.9152youxi.cn

[U41] PHP：初始化 Composer 项目
来源：http://fhm.vqdsnc.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://gqw.wangshuangyany.cn

[U42] PHP：PSR-4 自动加载
来源：http://itf.chenlongwang.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hfv.zhoulong.xyz

[U43] PHP：声明命名空间
来源：http://ume.dianchejie.cn

namespace App\Http;
来源：http://rbs.jyoumei.cn

[U44] PHP：开启严格类型
来源：http://lnc.xuetiantiany.cn

declare(strict_types=1);
来源：http://vxc.yvedp.cn

[U45] PHP：类型声明与返回类型
来源：http://qvh.316326.xyz

function add(int $a, int $b): int { return $a + $b; }
来源：http://dpu.jqgufenzy.top

[U46] PHP：可空类型
来源：http://syx.quarkkingdee.top

?string $name = null
来源：http://hzf.iojbl.cn

[U47] PHP：联合类型
来源：http://ojo.cqqwz.cn

int|string $id
来源：http://qss.daxiang520.top

[U48] PHP：纯枚举
来源：http://jar.jinqigufen.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://jsu.shuidangran.top

[U49] PHP：只读属性
来源：http://dtf.cqqwz.cn

public readonly string $name
来源：http://nuz.nanxinkj.top

[U50] PHP：构造器属性提升
来源：http://wpv.zdbjq.cn

public function __construct(private int $id) {}
来源：http://txx.zhongyouzk.top

[U51] PHP：数组解构
来源：http://zuy.gzhubu.top

[$a, $b] = $arr;
来源：http://tnd.xuanzx.com

[U52] PHP：箭头函数
来源：http://oej.ydzc1.top

$double = fn($x) => $x * 2;
来源：http://tvx.yj20258888.top

[U53] PHP：空合并运算符
来源：http://hco.yfazqb.com

$v = $a ?? $b ?? "default";
来源：http://zgy.meibo888.top

[U54] PHP：空安全调用
来源：http://khx.jianghu66.top

$obj?->method()
来源：http://qoe.feifeiyinyue.top

[U55] PHP：match 表达式
来源：http://lne.0kj1m.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://wxd.chenzaomai.com

[U56] PHP：命名参数
来源：http://tay.iojbl.cn

f(a: 1, b: 2)
来源：http://xsb.pengpengdd.cyou

[U57] PHP：字符串插值
来源：http://qcj.ybcxt.top

"值: {$a}"
来源：http://pda.svipenyu.cn

[U58] PHP：数组三件套
来源：http://ryr.shangyingyoupin.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://dgj.yueranfly.top

[U59] PHP：自定义排序
来源：http://pkm.nwbrower.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mlh.yonumen.top

[U60] PHP：JSON 编解码
来源：http://tgi.meibo888.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://kpw.bjfxy.top

[U61] PHP：正则
来源：http://nvv.zhoulong.xyz

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://ttr.yonumen.top

[U62] PHP：日期对象
来源：http://tuy.dashuyun.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://azb.sxryk.cn

[U63] PHP：文件读写
来源：http://lqq.jinyuanbaomall.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://gch.yonumen.top

[U64] PHP：目录遍历
来源：http://xte.redwolf501.top

glob("dir/*.php");  scandir("dir");
来源：http://rob.sweek.top

[U65] PHP：会话
来源：http://mbz.feifeiyinyue.top

session_start();  $_SESSION["uid"] = 1;
来源：http://ewq.zdbjq.cn

[U66] PHP：设置 Cookie
来源：http://mkd.xziqi.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://ltf.ywan-chungtsiang.top

[U67] PHP：处理文件上传
来源：http://vfm.jqgufenzy.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://hcc.xylfe.cn

[U68] PHP：PDO 连接
来源：http://vdr.hcnkem.com

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://duq.cashguo.top

[U69] PHP：PDO 预处理
来源：http://zsd.zhengqikj.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://wac.zhengqikj.top

[U70] PHP：PDO 事务
来源：http://amk.yongpay.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://wfe.jyoumei.cn

[U71] PHP：抛出异常
来源：http://edg.guannengcc.top

throw new RuntimeException("失败", 500);
来源：http://hyd.cucudq.cn

[U72] PHP：写错误日志
来源：http://xgt.ydjk.org.cn

error_log("失败: " . $e->getMessage());
来源：http://njv.yongpay.top

[U73] PHP：读取 ini 配置
来源：http://tfd.chenjidiqi.icu

parse_ini_file("config.ini", true)
来源：http://jdl.chenlongwang.top

[U74] PHP：读取环境变量
来源：http://sam.ctjpmb.com

getenv("APP_ENV") ?: "production"
来源：http://pbc.jinghuilouyu.cn

[U75] PHP：依赖注入
来源：http://cit.jqgfzy.top

composer require psr/container
来源：http://gbi.jianghu66.top

[U76] PHP：简单路由
来源：http://isu.ydjk.org.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://wks.yueranfly.top

[U77] PHP：模板渲染
来源：http://ude.aizwys.cn

composer require twig/twig
来源：http://kgm.redwolf501.top

[U78] PHP：单元测试
来源：http://bmu.daxiang520.top

composer require --dev phpunit/phpunit
来源：http://grj.nanxinkj.top

[U79] PHP：静态分析
来源：http://rkt.cheryme.top

composer require --dev phpstan/phpstan
来源：http://hkx.xingfuxueyuan.xyz

[U80] PHP：代码规范修复
来源：http://eev.xinyue.icu

composer require --dev friendsofphp/php-cs-fixer
来源：http://gpk.bjfxy.top

[U81] JS：初始化项目
来源：http://vtr.yangfankeji.com

npm init -y;  npm i express
来源：http://lce.iojbl.cn

[U82] JS：package.json 脚本
来源：http://rpj.sysykeji.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://qtw.ywan-chungtsiang.top

[U83] JS：ES Module 导入导出
来源：http://yei.52xcode.cn

export const a = 1;  import { a } from "./m.js";
来源：http://rmx.gzhubu.top

[U84] JS：CommonJS 写法
来源：http://jpi.haohaochexian.top

module.exports = { a };  const { a } = require("./m");
来源：http://zvz.aibaodan.cn

[U85] JS：可选链
来源：http://cdi.fzhhl.top

a?.b?.c
来源：http://jpr.quarkkingdee.top

[U86] JS：空值合并
来源：http://jms.ivvv.top

a ?? b
来源：http://xdg.52xcode.cn

[U87] JS：解构默认值
来源：http://gtc.zhengqikj.top

const { a = 1, b = 2 } = obj;
来源：http://ocy.nanxuanxn.top

[U88] JS：对象展开合并
来源：http://oed.ydjk.org.cn

{ ...a, ...b }
来源：http://bvu.c1oappe.top

[U89] JS：数组去重
来源：http://xxy.c1oappe.top

[...new Set(arr)]
来源：http://tvj.hywenlv.cn

[U90] JS：数字数组排序
来源：http://vyg.zdqjudy.top

[...arr].sort((a, b) => a - b)
来源：http://wld.52xcode.cn

[U91] JS：对象键值遍历
来源：http://yqm.sufxvd.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://unc.sweek.top

[U92] JS：深拷贝
来源：http://yjb.pycfn.com

structuredClone(obj)
来源：http://fhk.snrcjt.cn

[U93] JS：模板字符串
来源：http://pva.iojbl.cn

`共 ${n} 条`
来源：http://wyt.yonumen.top

[U94] JS：箭头函数
来源：http://cef.epnwcf.com

const double = x => x * 2;
来源：http://zka.xingfuxueyuan.xyz

[U95] JS：Promise 包装
来源：http://jba.yangfankeji.com

new Promise((resolve, reject) => {})
来源：http://vep.ehwqpu.com

[U96] JS：async/await 与异常
来源：http://miu.vehdjk.com

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://nmh.zhijiandao.cn

[U97] JS：并发请求
来源：http://vxq.meibo888.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://uje.sjlbkw.cn

[U98] JS：fetch 带 JSON
来源：http://rmk.ydzc1.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://cxv.yonumen.top

[U99] JS：事件监听
来源：http://uhn.jiagoushi.top

el.addEventListener("click", e => {})
来源：http://xut.zhijiandao.cn

[U100] JS：DOM 查询
来源：http://nmu.shanyushiyangtech.top

document.querySelector(".item")
来源：http://tzh.haohaochexian.top

[U101] JS：classList 操作
来源：http://bvd.vehdjk.com

el.classList.toggle("active")
来源：http://mkq.fktsv.cn

[U102] JS：本地存储
来源：http://oxm.yongpay.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://zxh.ydzc1.top

[U103] JS：定时器
来源：http://wzj.sysykeji.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://ppp.fktsv.cn

[U104] JS：防抖
来源：http://bwo.hnxiangtu.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://npg.mhx1999.top

[U105] JS：节流
来源：http://rnk.daria6918.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://egp.gaohongyu789.top

[U106] JS：日期格式化
来源：http://upi.ydzc1.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://rnf.gogol.net.cn

[U107] JS：数字千分位
来源：http://wae.xingfuxueyuan.xyz

new Intl.NumberFormat("en-US").format(1234567)
来源：http://czq.zhongyouzk.top

[U108] JS：随机整数
来源：http://kuu.meibo888.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://qvm.9152youxi.cn

[U109] JS：数组分组
来源：http://axp.zycfv.cn

Object.groupBy(arr, x => x.type)
来源：http://mbx.xuetiantiany.cn

[U110] JS：数组分块
来源：http://ajd.cucudq.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://wym.yueranfly.top

[U111] JS：对象转 Map
来源：http://bhk.jinqigufen.top

new Map(Object.entries(obj))
来源：http://mbw.cheryme.top

[U112] JS：字符串补位
来源：http://sep.nanxuanxn.top

"7".padStart(3, "0")
来源：http://wlg.shangyingyoupin.top

[U113] JS：正则替换全部
来源：http://fyz.hysaishi.cn

s.replaceAll("a", "b")
来源：http://yie.hammf.cn

[U114] JS：JSON 深比较
来源：http://zya.ivvv.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://wgv.pycfn.com

[U115] JS：生成 UUID
来源：http://ugz.kuanghao11.cn

crypto.randomUUID()
来源：http://tbt.zhaomingkeji.xyz

[U116] JS：类型检查（JSDoc）
来源：http://dhe.sweek.top

/** @param {string} name */ function f(name) {}
来源：http://jhn.meibo888.top

[U117] JS：单元测试
来源：http://wim.smart0.xyz

npm i -D vitest;  npx vitest
来源：http://nwc.jinghuilouyu.cn

[U118] JS：开发服务器
来源：http://ips.hammf.cn

npm i -D vite;  npx vite
来源：http://efz.havefunace.top

[U119] JS：生产构建
来源：http://hpo.jinqigfzy.top

npx vite build
来源：http://doj.52xcode.cn

[U120] JS：读取环境变量（Vite）
来源：http://emj.yj202588.top

import.meta.env.VITE_API_URL
来源：http://ibd.tarul.cn


<!-- 参考信息 -->