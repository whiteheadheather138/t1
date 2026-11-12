代发 wailian999

[T33] Lua：表（数组）
来源：http://ahs.fanxiaobao.xyz

local t = {1, 2, 3};  t[4] = 4
来源：http://bmy.daria6918.cn

[T34] Lua：遍历表
来源：http://bqi.shzxlz.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://pkl.zhijiandao.cn

[T35] Lua：字典表
来源：http://myi.sweek.top

local d = { a = 1 };  d.b = 2
来源：http://idz.chenjidiqi.icu

[T36] Lua：函数
来源：http://uqw.tanke756.top

function add(a, b) return a + b end
来源：http://rtg.hammf.cn

[T37] Lua：字符串拼接
来源：http://fnz.zhaomingkeji.xyz

"a" .. "b"
来源：http://ern.jianghu66.top

[T38] Lua：条件
来源：http://pyx.hnqzz.top

if x > 0 then print("正") end
来源：http://aju.yfazqb.com

[T39] Lua：模式匹配
来源：http://hlx.ywan-chungtsiang.top

string.find(s, "%d+")
来源：http://hgb.pengpengdd.cyou

[T40] Lua：元表
来源：http://xtg.yuxming.cn

setmetatable({}, { __index = base })
来源：http://rqd.cucudq.cn

[T41] Perl：Hello World
来源：http://mya.epnwcf.com

print "Hello\n";
来源：http://ejo.daxiang520.top

[T42] Perl：变量类型
来源：http://tqy.epnwcf.com

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://xsa.haohaochexian.top

[T43] Perl：字符串插值
来源：http://xho.sysykeji.top

"值: $a"
来源：http://hna.jlsjyb.cn

[T44] Perl：条件
来源：http://ihx.gzhubu.top

if ($a > 0) { print "正"; }
来源：http://kxd.birdmap.top

[T45] Perl：数组遍历
来源：http://tjn.fanxiaobao.xyz

for my $x (@arr) { print $x; }
来源：http://ncb.bjfxy.top

[T46] Perl：哈希操作
来源：http://jxi.andypj.xyz

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://tgz.smart0.xyz

[T47] Perl：正则捕获
来源：http://oep.ppjwa.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://axt.yj20258888.top

[T48] Perl：正则替换
来源：http://czm.kuanghao11.cn

$s =~ s/old/new/g;
来源：http://duu.jinqigfzy.top

[T49] Perl：函数
来源：http://uvn.hesvh.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://yai.wangdashe.top

[T50] Perl：逐行读文件
来源：http://hbn.yuanzhike.top

open my $fh, "<", "a.txt" or die $!;
来源：http://ijd.jinghuilouyu.cn

while (my $line = <$fh>) { print $line; }
来源：http://lul.52xcode.cn

[T51] Scala：Hello World
来源：http://uaj.dianchejie.cn

println("Hello")
来源：http://nbb.xuanzx.com

[T52] Scala：变量
来源：http://vah.yuxming.cn

val a = 1;  var b = 2
来源：http://mih.daria6918.cn

[T53] Scala：字符串插值
来源：http://thy.jinghuilouyu.cn

s"值: $b"
来源：http://tau.zdbjq.cn

[T54] Scala：集合映射
来源：http://njx.ydjk.org.cn

List(1, 2, 3).map(_ * 2)
来源：http://ird.hnqzz.top

[T55] Scala：集合过滤
来源：http://iyo.yj20258.top

List(1, 2, 3).filter(_ > 1)
来源：http://bih.jlsjyb.cn

[T56] Scala：样例类
来源：http://eiv.c1oappe.top

case class User(name: String, age: Int)
来源：http://kjn.ctjpmb.com

[T57] Scala：模式匹配
来源：http://uqs.xuanzx.com

x match { case 1 => "一"; case _ => "其他" }
来源：http://lap.tanke756.top

[T58] Scala：函数定义
来源：http://pbo.mhx1999.top

def add(a: Int, b: Int): Int = a + b
来源：http://ogr.vehdjk.com

[T59] Scala：循环
来源：http://dia.zdbjq.cn

for (i <- 1 to 10) println(i)
来源：http://vwe.nanxuanxn.top

[T60] Scala：折叠
来源：http://vqk.c1oappe.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://giv.tanke756.top

================================================================================
来源：http://txe.aibaodan.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://ptb.zhoulong.xyz

================================================================================
来源：http://cod.jqgfzy.top

[U01] Py：创建虚拟环境
来源：http://srg.shangyingyoupin.top

python -m venv .venv && source .venv/bin/activate
来源：http://xvl.epnwcf.com

[U02] Py：导出 / 安装依赖
来源：http://lbn.zhongyouzk.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://buo.fktsv.cn

[U03] Py：加载 .env 配置
来源：http://ujl.tianlin.xyz

from dotenv import load_dotenv; load_dotenv()
来源：http://bbu.snrcjt.cn

[U04] Py：变量调试打印
来源：http://lla.pycfn.com

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://ccj.jiagoushi.top

[U05] Py：列表去重且保序
来源：http://ydw.cashguo.top

list(dict.fromkeys(arr))
来源：http://nyz.wangdashe.top

[U06] Py：合并两个字典
来源：http://loy.jyoumei.cn

{**a, **b}
来源：http://eyx.svipenyu.cn

[U07] Py：反转字典键值
来源：http://qlw.vqdsnc.cn

{v: k for k, v in d.items()}
来源：http://iez.chenjidiqi.icu

[U08] Py：展平二维列表
来源：http://pet.hesvh.cn

[y for x in nested for y in x]
来源：http://qrl.gogol.net.cn

[U09] Py：字典取最大值的键
来源：http://xio.hywenlv.cn

max(d, key=d.get)
来源：http://fdz.iojbl.cn

[U10] Py：按值排序字典
来源：http://sqp.yueranfly.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://iwx.shanyushiyangtech.top

[U11] Py：生成器表达式
来源：http://coz.sweek.top

(x * 2 for x in arr)
来源：http://mlt.hnxiangtu.top

[U12] Py：取出现最多的 3 个元素
来源：http://dbx.nanxuanxn.top

Counter(arr).most_common(3)
来源：http://dyy.redwolf501.top

[U13] Py：固定长度队列
来源：http://jlz.cashguo.top

deque(maxlen=10)
来源：http://hzc.fehbvm.com

[U14] Py：分组收集到列表
来源：http://uso.zdbjq.cn

defaultdict(list)
来源：http://ryo.vqdsnc.cn

[U15] Py：高精度计时
来源：http://qci.shangyingyoupin.top

t = time.perf_counter()
来源：http://jun.guowangkeji.top

[U16] Py：命令行参数解析
来源：http://ajy.iojbl.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://fkr.jyoumei.cn

[U17] Py：初始化日志
来源：http://xuu.jqgfzy.top

logging.basicConfig(level=logging.INFO)
来源：http://otl.wangshuangyany.cn

[U18] Py：预编译正则
来源：http://pvd.cashguo.top

pat = re.compile(r"\d+")
来源：http://yym.yfazqb.com

[U19] Py：正则替换带回调
来源：http://yci.shangyingyoupin.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://cdo.pengpengdd.cyou

[U20] Py：缓存函数结果
来源：http://ggr.sufxvd.cn

@functools.lru_cache(maxsize=None)
来源：http://cch.smart0.xyz

[U21] Py：自定义上下文管理器
来源：http://gte.hammf.cn

@contextlib.contextmanager
来源：http://wub.guannengcc.top

[U22] Py：矩阵转置
来源：http://awj.quarkkingdee.top

list(zip(*m))
来源：http://pco.jlsjyb.cn

[U23] Py：分块读取大文件
来源：http://ynm.ivvv.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://nig.daria6918.cn

[U24] Py：路径操作
来源：http://czq.jqgfzy.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://ugo.fanxiaobao.xyz

[U25] Py：CSV 按字典读
来源：http://zym.yongpay.top

csv.DictReader(f)
来源：http://kbs.yj20258888.top

[U26] Py：并发下载
来源：http://xzt.hywenlv.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://zqs.nanxinkj.top

[U27] Py：异步 HTTP
来源：http://vsa.chenlongwang.top

aiohttp.ClientSession() 配合 async with
来源：http://ywt.daria6918.cn

[U28] Py：类型别名
来源：http://ofb.jiagoushi.top

UserId = int
来源：http://zki.chenlongwang.top

[U29] Py：属性校验
来源：http://ukr.jinqigufen.top

@property 与 @x.setter 配合
来源：http://qyy.smart0.xyz

[U30] Py：数据类
来源：http://fgi.gogol.net.cn

@dataclass(slots=True)
来源：http://qpm.jinqigfzy.top

[U31] Py：单测
来源：http://guk.c1oappe.top

python -m pytest -q
来源：http://pfc.gotoacloud.top

[U32] Py：代码格式化
来源：http://szj.hesvh.cn

ruff format . && ruff check --fix .
来源：http://cwq.ybcxt.top

[U33] Py：打包发布
来源：http://hvs.bbcook.cn

python -m build  （依赖 pyproject.toml）
来源：http://bnn.jinqigfzy.top

[U34] Py：判断编码
来源：http://dnw.yvedp.cn

chardet.detect(raw)
来源：http://yhi.ctjpmb.com

[U35] Py：发送邮件
来源：http://qkn.sjlbkw.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://ucl.ydzc1.top

[U36] Py：定时任务
来源：http://ukk.ctjpmb.com

schedule.every(10).minutes.do(job)
来源：http://uck.haohaochexian.top

[U37] Py：读写 Excel
来源：http://gqv.epnwcf.com

pandas.read_excel / DataFrame.to_excel
来源：http://nuf.zhixingplan.top

[U38] Py：获取脚本所在目录
来源：http://tnq.shanyushiyangtech.top

Path(__file__).resolve().parent
来源：http://ukc.iojbl.cn

[U39] Py：判断是否在交互环境
来源：http://ulr.nanxuanxn.top

sys.stdout.isatty()
来源：http://par.jinghuilouyu.cn

[U40] Py：打印到标准错误
来源：http://ixr.yvedp.cn

print("err", file=sys.stderr)
来源：http://ifz.wangshuangyany.cn

[U41] PHP：初始化 Composer 项目
来源：http://ppy.svipenyu.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://bme.andypj.xyz

[U42] PHP：PSR-4 自动加载
来源：http://fud.0kj1m.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://tjk.daria6918.cn

[U43] PHP：声明命名空间
来源：http://ttf.zhengqikj.top

namespace App\Http;
来源：http://jyg.yj20258.top

[U44] PHP：开启严格类型
来源：http://gxl.zhixingplan.top

declare(strict_types=1);
来源：http://pby.pycfn.com

[U45] PHP：类型声明与返回类型
来源：http://ull.zycfv.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://cve.jinghuilouyu.cn

[U46] PHP：可空类型
来源：http://wis.ybcxt.top

?string $name = null
来源：http://ild.gotoacloud.top

[U47] PHP：联合类型
来源：http://emh.sysykeji.top

int|string $id
来源：http://pjt.c1oappe.top

[U48] PHP：纯枚举
来源：http://gsk.shanyushiyangtech.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://ual.gaohongyu789.top

[U49] PHP：只读属性
来源：http://eai.316326.xyz

public readonly string $name
来源：http://zhd.tianlin.xyz

[U50] PHP：构造器属性提升
来源：http://zem.nanxinkj.top

public function __construct(private int $id) {}
来源：http://vsc.shuidangran.top

[U51] PHP：数组解构
来源：http://apw.zhongyouzk.top

[$a, $b] = $arr;
来源：http://jqq.zycfv.cn

[U52] PHP：箭头函数
来源：http://mzr.daria6918.cn

$double = fn($x) => $x * 2;
来源：http://med.birdmap.top

[U53] PHP：空合并运算符
来源：http://nlk.aizwys.cn

$v = $a ?? $b ?? "default";
来源：http://cci.pengpengdd.cyou

[U54] PHP：空安全调用
来源：http://dqd.zhixingplan.top

$obj?->method()
来源：http://apl.yj20258.top

[U55] PHP：match 表达式
来源：http://rxf.c1oappe.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://ruy.xuanzx.com

[U56] PHP：命名参数
来源：http://slx.vqdsnc.cn

f(a: 1, b: 2)
来源：http://fzi.xziqi.cn

[U57] PHP：字符串插值
来源：http://qhu.jinqigfzy.top

"值: {$a}"
来源：http://xyd.mhx1999.top

[U58] PHP：数组三件套
来源：http://fcj.tarul.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://mec.jlsjyb.cn

[U59] PHP：自定义排序
来源：http://vmy.sjlbkw.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://xmw.shuidangran.top

[U60] PHP：JSON 编解码
来源：http://blh.xinyue.icu

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://qck.shanyushiyangkeji.top

[U61] PHP：正则
来源：http://ekv.pycfn.com

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://lvd.iojbl.cn

[U62] PHP：日期对象
来源：http://xbi.zycfv.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://jwz.smart0.xyz

[U63] PHP：文件读写
来源：http://pwd.hesvh.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://cpp.yueranfly.top

[U64] PHP：目录遍历
来源：http://kzq.xuetiantiany.cn

glob("dir/*.php");  scandir("dir");
来源：http://dwf.pycfn.com

[U65] PHP：会话
来源：http://uar.jlsjyb.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://caq.yueranfly.top

[U66] PHP：设置 Cookie
来源：http://inn.hongshengwenyu.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://ylc.yj202588.top

[U67] PHP：处理文件上传
来源：http://ded.ydjk.org.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://sqw.yvedp.cn

[U68] PHP：PDO 连接
来源：http://ogu.zdbjq.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://zlf.nanxuanxn.top

[U69] PHP：PDO 预处理
来源：http://xae.shanyushiyangkeji.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://kme.cashguo.top

[U70] PHP：PDO 事务
来源：http://eil.cdnleiting.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://zyz.jlsjyb.cn

[U71] PHP：抛出异常
来源：http://qns.pycfn.com

throw new RuntimeException("失败", 500);
来源：http://tul.ydjk.org.cn

[U72] PHP：写错误日志
来源：http://puo.9152youxi.cn

error_log("失败: " . $e->getMessage());
来源：http://ago.kuanghao11.cn

[U73] PHP：读取 ini 配置
来源：http://huc.epnwcf.com

parse_ini_file("config.ini", true)
来源：http://ogf.gaohongyu789.top

[U74] PHP：读取环境变量
来源：http://lcl.shuidangran.top

getenv("APP_ENV") ?: "production"
来源：http://clk.hfpthk.cn

[U75] PHP：依赖注入
来源：http://ros.fzhhl.top

composer require psr/container
来源：http://vkv.yanxiufei.cn

[U76] PHP：简单路由
来源：http://iyg.hnqzz.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://hgp.316326.xyz

[U77] PHP：模板渲染
来源：http://jrw.uphjek.com

composer require twig/twig
来源：http://dea.hfpthk.cn

[U78] PHP：单元测试
来源：http://ebk.dianchejie.cn

composer require --dev phpunit/phpunit
来源：http://yxm.yj202588.top

[U79] PHP：静态分析
来源：http://mul.hesvh.cn

composer require --dev phpstan/phpstan
来源：http://vwz.jqgfzy.top

[U80] PHP：代码规范修复
来源：http://nfq.shangyingyoupin.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://roy.0kj1m.cn

[U81] JS：初始化项目
来源：http://iqz.bbcook.cn

npm init -y;  npm i express
来源：http://gin.dashuyun.cn

[U82] JS：package.json 脚本
来源：http://bjr.hcnkem.com

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://fln.yonumen.top

[U83] JS：ES Module 导入导出
来源：http://opq.jiagoushi.top

export const a = 1;  import { a } from "./m.js";
来源：http://kut.daxiang520.top

[U84] JS：CommonJS 写法
来源：http://ogx.zycfv.cn

module.exports = { a };  const { a } = require("./m");
来源：http://cnn.xingfuxueyuan.xyz

[U85] JS：可选链
来源：http://kvj.yj202588.top

a?.b?.c
来源：http://lrm.hesvh.cn

[U86] JS：空值合并
来源：http://vtf.gaohongyu789.top

a ?? b
来源：http://ift.hammf.cn

[U87] JS：解构默认值
来源：http://sos.pengpengdd.cyou

const { a = 1, b = 2 } = obj;
来源：http://mtd.wangshuangyany.cn

[U88] JS：对象展开合并
来源：http://gbi.shanyushiyangtech.top

{ ...a, ...b }
来源：http://amg.dashuyun.cn

[U89] JS：数组去重
来源：http://eui.zhoulong.xyz

[...new Set(arr)]
来源：http://myt.gaohongyu789.top

[U90] JS：数字数组排序
来源：http://fns.kuanghao11.cn

[...arr].sort((a, b) => a - b)
来源：http://wpx.jinqigufen.top

[U91] JS：对象键值遍历
来源：http://qua.tarul.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://enc.gzhubu.top

[U92] JS：深拷贝
来源：http://vij.sxryk.cn

structuredClone(obj)
来源：http://vns.bbcook.cn

[U93] JS：模板字符串
来源：http://njq.yongpay.top

`共 ${n} 条`
来源：http://zje.hnqzz.top

[U94] JS：箭头函数
来源：http://dkx.jyoumei.cn

const double = x => x * 2;
来源：http://ywd.epnwcf.com

[U95] JS：Promise 包装
来源：http://psa.tarul.cn

new Promise((resolve, reject) => {})
来源：http://jzc.xziqi.cn

[U96] JS：async/await 与异常
来源：http://fyo.wangshuangyany.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://dbz.jianghu66.top

[U97] JS：并发请求
来源：http://beh.52xcode.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://rjy.zdbjq.cn

[U98] JS：fetch 带 JSON
来源：http://knu.vehdjk.com

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://vfc.hywenlv.cn

[U99] JS：事件监听
来源：http://rns.cqqwz.cn

el.addEventListener("click", e => {})
来源：http://zfg.epnwcf.com

[U100] JS：DOM 查询
来源：http://vic.vehdjk.com

document.querySelector(".item")
来源：http://mvj.jqgfzy.top

[U101] JS：classList 操作
来源：http://dcw.fanxiaobao.xyz

el.classList.toggle("active")
来源：http://bur.zhongyouzk.top

[U102] JS：本地存储
来源：http://xvk.zhijiandao.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://uoq.sufxvd.cn

[U103] JS：定时器
来源：http://neo.pycfn.com

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://ibr.zhixingplan.top

[U104] JS：防抖
来源：http://uvq.yj202588.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://pbj.hfpthk.cn

[U105] JS：节流
来源：http://sdc.jianghu66.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://qif.andypj.xyz

[U106] JS：日期格式化
来源：http://hkl.haohaochexian.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://mny.feifeiyinyue.top

[U107] JS：数字千分位
来源：http://ihu.jqgfzy.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://pzf.xinyue.icu

[U108] JS：随机整数
来源：http://rag.hongshengwenyu.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://vhk.bjfxy.top

[U109] JS：数组分组
来源：http://ufg.haohaochexian.top

Object.groupBy(arr, x => x.type)
来源：http://muj.fehbvm.com

[U110] JS：数组分块
来源：http://pny.sjlbkw.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://qnp.hammf.cn

[U111] JS：对象转 Map
来源：http://hco.cdnleiting.top

new Map(Object.entries(obj))
来源：http://bbr.hongshengwenyu.top

[U112] JS：字符串补位
来源：http://fnj.yj20258.top

"7".padStart(3, "0")
来源：http://dty.shangyingyoupin.top

[U113] JS：正则替换全部
来源：http://mgq.zdbjq.cn

s.replaceAll("a", "b")
来源：http://civ.ivvv.top

[U114] JS：JSON 深比较
来源：http://nfe.chenlongwang.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://umu.sysykeji.top

[U115] JS：生成 UUID
来源：http://zrs.haohaochexian.top

crypto.randomUUID()
来源：http://hsu.0kj1m.cn

[U116] JS：类型检查（JSDoc）
来源：http://rvk.yongpay.top

/** @param {string} name */ function f(name) {}
来源：http://ggd.kuanghao11.cn

[U117] JS：单元测试
来源：http://mek.redwolf501.top

npm i -D vitest;  npx vitest
来源：http://nqt.shuidangran.top

[U118] JS：开发服务器
来源：http://uey.jqgufenzy.top

npm i -D vite;  npx vite
来源：http://kth.52xcode.cn

[U119] JS：生产构建
来源：http://lir.yongpay.top

npx vite build
来源：http://utv.ehwqpu.com

[U120] JS：读取环境变量（Vite）
来源：http://xev.yfazqb.com

import.meta.env.VITE_API_URL
来源：http://dva.yueranfly.top


<!-- 参考信息 -->