代发 wailian999

[T33] Lua：表（数组）
来源：http://fox.pycfn.com

local t = {1, 2, 3};  t[4] = 4
来源：http://vlq.fzhhl.top

[T34] Lua：遍历表
来源：http://den.jlsjyb.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://gzw.jinqigfzy.top

[T35] Lua：字典表
来源：http://jmx.hammf.cn

local d = { a = 1 };  d.b = 2
来源：http://osh.epnwcf.com

[T36] Lua：函数
来源：http://owa.yj20258888.top

function add(a, b) return a + b end
来源：http://apy.hcnkem.com

[T37] Lua：字符串拼接
来源：http://dfi.kuanghao11.cn

"a" .. "b"
来源：http://gnc.daria6918.cn

[T38] Lua：条件
来源：http://zwv.jinqigfzy.top

if x > 0 then print("正") end
来源：http://wgj.yj20258888.top

[T39] Lua：模式匹配
来源：http://rcf.guannengcc.top

string.find(s, "%d+")
来源：http://lcz.chenlongwang.top

[T40] Lua：元表
来源：http://oem.cucudq.cn

setmetatable({}, { __index = base })
来源：http://eyg.jianghu66.top

[T41] Perl：Hello World
来源：http://fdr.smart0.xyz

print "Hello\n";
来源：http://geu.sufxvd.cn

[T42] Perl：变量类型
来源：http://vln.feifeiyinyue.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://yvq.dashuyun.cn

[T43] Perl：字符串插值
来源：http://mca.havefunace.top

"值: $a"
来源：http://gtf.zhoulong.xyz

[T44] Perl：条件
来源：http://vqi.vqdsnc.cn

if ($a > 0) { print "正"; }
来源：http://kzr.sjlbkw.cn

[T45] Perl：数组遍历
来源：http://wtg.feifeiyinyue.top

for my $x (@arr) { print $x; }
来源：http://uju.yonumen.top

[T46] Perl：哈希操作
来源：http://gie.dianchejie.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://tha.chenzaomai.com

[T47] Perl：正则捕获
来源：http://hvu.xylfe.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://yym.andypj.xyz

[T48] Perl：正则替换
来源：http://ojy.guowangkeji.top

$s =~ s/old/new/g;
来源：http://hkl.havefunace.top

[T49] Perl：函数
来源：http://cir.guowangkeji.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://xhv.hcnkem.com

[T50] Perl：逐行读文件
来源：http://pgl.guannengcc.top

open my $fh, "<", "a.txt" or die $!;
来源：http://lxn.sxryk.cn

while (my $line = <$fh>) { print $line; }
来源：http://gfd.xziqi.cn

[T51] Scala：Hello World
来源：http://fsb.vehdjk.com

println("Hello")
来源：http://dbi.yonumen.top

[T52] Scala：变量
来源：http://mdq.jqgfzy.top

val a = 1;  var b = 2
来源：http://xfo.xinyue.icu

[T53] Scala：字符串插值
来源：http://qwg.wangdashe.top

s"值: $b"
来源：http://asu.meibo888.top

[T54] Scala：集合映射
来源：http://fdu.yvedp.cn

List(1, 2, 3).map(_ * 2)
来源：http://sdy.tarul.cn

[T55] Scala：集合过滤
来源：http://ugm.fzhhl.top

List(1, 2, 3).filter(_ > 1)
来源：http://izx.ehwqpu.com

[T56] Scala：样例类
来源：http://ijo.jinghuilouyu.cn

case class User(name: String, age: Int)
来源：http://tid.shangyingyoupin.top

[T57] Scala：模式匹配
来源：http://cro.xuetiantiany.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://aou.zdbjq.cn

[T58] Scala：函数定义
来源：http://oph.kuanghao11.cn

def add(a: Int, b: Int): Int = a + b
来源：http://goh.sweek.top

[T59] Scala：循环
来源：http://mrk.yj202588.top

for (i <- 1 to 10) println(i)
来源：http://dei.hongshengwenyu.top

[T60] Scala：折叠
来源：http://fdq.fanxiaobao.xyz

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://ors.shuidangran.top

================================================================================
来源：http://mlq.yueranfly.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://zrh.guowangkeji.top

================================================================================
来源：http://hzk.xuanzx.com

[U01] Py：创建虚拟环境
来源：http://zpw.chenlongwang.top

python -m venv .venv && source .venv/bin/activate
来源：http://dtn.tarul.cn

[U02] Py：导出 / 安装依赖
来源：http://qxy.cqqwz.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://kvl.xuetiantiany.cn

[U03] Py：加载 .env 配置
来源：http://ugy.feifeiyinyue.top

from dotenv import load_dotenv; load_dotenv()
来源：http://dqj.xylfe.cn

[U04] Py：变量调试打印
来源：http://dgg.shanyushiyangtech.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://yqg.shangyingyoupin.top

[U05] Py：列表去重且保序
来源：http://lsi.aibaodan.cn

list(dict.fromkeys(arr))
来源：http://ash.xziqi.cn

[U06] Py：合并两个字典
来源：http://sxo.jiagoushi.top

{**a, **b}
来源：http://vyp.bjfxy.top

[U07] Py：反转字典键值
来源：http://zpz.daria6918.cn

{v: k for k, v in d.items()}
来源：http://lpp.xuanzx.com

[U08] Py：展平二维列表
来源：http://hmy.guannengcc.top

[y for x in nested for y in x]
来源：http://fyp.cucudq.cn

[U09] Py：字典取最大值的键
来源：http://lza.fanxiaobao.xyz

max(d, key=d.get)
来源：http://yju.xinyue.icu

[U10] Py：按值排序字典
来源：http://nnc.0kj1m.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://lnu.havefunace.top

[U11] Py：生成器表达式
来源：http://lzu.hammf.cn

(x * 2 for x in arr)
来源：http://hdj.yonumen.top

[U12] Py：取出现最多的 3 个元素
来源：http://lga.shangyingyoupin.top

Counter(arr).most_common(3)
来源：http://ntz.daria6918.cn

[U13] Py：固定长度队列
来源：http://fxv.shuidangran.top

deque(maxlen=10)
来源：http://pxo.9152youxi.cn

[U14] Py：分组收集到列表
来源：http://wji.jqgfzy.top

defaultdict(list)
来源：http://dfo.zhoulong.xyz

[U15] Py：高精度计时
来源：http://cgj.cqqwz.cn

t = time.perf_counter()
来源：http://vyi.cucudq.cn

[U16] Py：命令行参数解析
来源：http://dah.xinyue.icu

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://ezs.hysaishi.cn

[U17] Py：初始化日志
来源：http://yww.jlsjyb.cn

logging.basicConfig(level=logging.INFO)
来源：http://rtz.mhx1999.top

[U18] Py：预编译正则
来源：http://nej.gotoacloud.top

pat = re.compile(r"\d+")
来源：http://duh.zdqjudy.top

[U19] Py：正则替换带回调
来源：http://pve.haohaochexian.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://doq.cheryme.top

[U20] Py：缓存函数结果
来源：http://xao.kuanghao11.cn

@functools.lru_cache(maxsize=None)
来源：http://per.ydzc1.top

[U21] Py：自定义上下文管理器
来源：http://znk.xingfuxueyuan.xyz

@contextlib.contextmanager
来源：http://kqd.gogol.net.cn

[U22] Py：矩阵转置
来源：http://npx.cdnleiting.top

list(zip(*m))
来源：http://zjz.hysaishi.cn

[U23] Py：分块读取大文件
来源：http://pfr.shangyingyoupin.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://owf.gogol.net.cn

[U24] Py：路径操作
来源：http://wmb.9152youxi.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://pdp.yj20258.top

[U25] Py：CSV 按字典读
来源：http://mjg.yj202588.top

csv.DictReader(f)
来源：http://isz.hywenlv.cn

[U26] Py：并发下载
来源：http://ejo.jqgfzy.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://znu.hysaishi.cn

[U27] Py：异步 HTTP
来源：http://azi.hfpthk.cn

aiohttp.ClientSession() 配合 async with
来源：http://hzs.zdqjudy.top

[U28] Py：类型别名
来源：http://dol.hnqzz.top

UserId = int
来源：http://kak.gogol.net.cn

[U29] Py：属性校验
来源：http://vql.9152youxi.cn

@property 与 @x.setter 配合
来源：http://twl.guowangkeji.top

[U30] Py：数据类
来源：http://rgz.birdmap.top

@dataclass(slots=True)
来源：http://jza.yfazqb.com

[U31] Py：单测
来源：http://cdq.hnxiangtu.top

python -m pytest -q
来源：http://wgu.52xcode.cn

[U32] Py：代码格式化
来源：http://hny.daxiang520.top

ruff format . && ruff check --fix .
来源：http://ubd.vehdjk.com

[U33] Py：打包发布
来源：http://efu.xinyue.icu

python -m build  （依赖 pyproject.toml）
来源：http://tsc.yueranfly.top

[U34] Py：判断编码
来源：http://dor.fengsongda.top

chardet.detect(raw)
来源：http://tum.jlsjyb.cn

[U35] Py：发送邮件
来源：http://mnl.hammf.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://moe.chenjidiqi.icu

[U36] Py：定时任务
来源：http://mqb.svipenyu.cn

schedule.every(10).minutes.do(job)
来源：http://krz.yj202588.top

[U37] Py：读写 Excel
来源：http://ump.52xcode.cn

pandas.read_excel / DataFrame.to_excel
来源：http://utb.shzxlz.cn

[U38] Py：获取脚本所在目录
来源：http://cot.xinyue.icu

Path(__file__).resolve().parent
来源：http://age.jqgufenzy.top

[U39] Py：判断是否在交互环境
来源：http://njg.ybcxt.top

sys.stdout.isatty()
来源：http://xnu.epnwcf.com

[U40] Py：打印到标准错误
来源：http://tfw.dianchejie.cn

print("err", file=sys.stderr)
来源：http://hbg.sweek.top

[U41] PHP：初始化 Composer 项目
来源：http://kxc.zdqjudy.top

composer init;  composer require guzzlehttp/guzzle
来源：http://ljv.guowangkeji.top

[U42] PHP：PSR-4 自动加载
来源：http://aut.zhixingplan.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://vsx.vqdsnc.cn

[U43] PHP：声明命名空间
来源：http://rkg.hnxiangtu.top

namespace App\Http;
来源：http://ytp.52xcode.cn

[U44] PHP：开启严格类型
来源：http://eph.shzxlz.cn

declare(strict_types=1);
来源：http://ift.iojbl.cn

[U45] PHP：类型声明与返回类型
来源：http://are.shzxlz.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://luf.guowangkeji.top

[U46] PHP：可空类型
来源：http://kjb.gzhubu.top

?string $name = null
来源：http://jiv.yonumen.top

[U47] PHP：联合类型
来源：http://gns.jlsjyb.cn

int|string $id
来源：http://gmr.redwolf501.top

[U48] PHP：纯枚举
来源：http://tly.chenlongwang.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://mni.sjlbkw.cn

[U49] PHP：只读属性
来源：http://yru.iojbl.cn

public readonly string $name
来源：http://qhr.xziqi.cn

[U50] PHP：构造器属性提升
来源：http://voj.pengpengdd.cyou

public function __construct(private int $id) {}
来源：http://ymf.9152youxi.cn

[U51] PHP：数组解构
来源：http://nal.cqqwz.cn

[$a, $b] = $arr;
来源：http://eti.zhengqikj.top

[U52] PHP：箭头函数
来源：http://ats.zhengqikj.top

$double = fn($x) => $x * 2;
来源：http://pcq.shangyingyoupin.top

[U53] PHP：空合并运算符
来源：http://nfe.ybcxt.top

$v = $a ?? $b ?? "default";
来源：http://ydo.birdmap.top

[U54] PHP：空安全调用
来源：http://ije.zdbjq.cn

$obj?->method()
来源：http://yvx.ehwqpu.com

[U55] PHP：match 表达式
来源：http://yoj.snrcjt.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://jfn.ivvv.top

[U56] PHP：命名参数
来源：http://itj.shanyushiyangtech.top

f(a: 1, b: 2)
来源：http://tvp.hnqzz.top

[U57] PHP：字符串插值
来源：http://iug.ywan-chungtsiang.top

"值: {$a}"
来源：http://wic.cucudq.cn

[U58] PHP：数组三件套
来源：http://bnk.ppjwa.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://ybh.jianghu66.top

[U59] PHP：自定义排序
来源：http://dhc.jiagoushi.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mhi.jlsjyb.cn

[U60] PHP：JSON 编解码
来源：http://azw.zdqjudy.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://oav.ctjpmb.com

[U61] PHP：正则
来源：http://gzu.ywan-chungtsiang.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://sec.gogol.net.cn

[U62] PHP：日期对象
来源：http://xwd.andypj.xyz

(new DateTimeImmutable())->format("Y-m-d");
来源：http://ojo.yfazqb.com

[U63] PHP：文件读写
来源：http://giq.guowangkeji.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://snj.zdqjudy.top

[U64] PHP：目录遍历
来源：http://mhu.birdmap.top

glob("dir/*.php");  scandir("dir");
来源：http://lib.haohaochexian.top

[U65] PHP：会话
来源：http://zad.yuanzhike.top

session_start();  $_SESSION["uid"] = 1;
来源：http://lxr.shanyushiyangkeji.top

[U66] PHP：设置 Cookie
来源：http://ioi.yongpay.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://ere.jinghuilouyu.cn

[U67] PHP：处理文件上传
来源：http://igf.nanxinkj.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://xjl.daria6918.cn

[U68] PHP：PDO 连接
来源：http://htz.pycfn.com

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://rlf.vqdsnc.cn

[U69] PHP：PDO 预处理
来源：http://uyy.birdmap.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://bqw.shanyushiyangkeji.top

[U70] PHP：PDO 事务
来源：http://euc.bbcook.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://dlc.svipenyu.cn

[U71] PHP：抛出异常
来源：http://wgq.52xcode.cn

throw new RuntimeException("失败", 500);
来源：http://oxd.iojbl.cn

[U72] PHP：写错误日志
来源：http://lpb.hesvh.cn

error_log("失败: " . $e->getMessage());
来源：http://cme.cashguo.top

[U73] PHP：读取 ini 配置
来源：http://ebm.ivvv.top

parse_ini_file("config.ini", true)
来源：http://jsi.tarul.cn

[U74] PHP：读取环境变量
来源：http://kcz.zhiwuduotai.top

getenv("APP_ENV") ?: "production"
来源：http://hym.sysykeji.top

[U75] PHP：依赖注入
来源：http://thg.ehwqpu.com

composer require psr/container
来源：http://jpa.c1oappe.top

[U76] PHP：简单路由
来源：http://juq.quarkkingdee.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://epg.vehdjk.com

[U77] PHP：模板渲染
来源：http://pdk.snrcjt.cn

composer require twig/twig
来源：http://ptm.bbcook.cn

[U78] PHP：单元测试
来源：http://vyu.wangshuangyany.cn

composer require --dev phpunit/phpunit
来源：http://ukk.zhengqikj.top

[U79] PHP：静态分析
来源：http://iss.cucudq.cn

composer require --dev phpstan/phpstan
来源：http://sai.zhiwuduotai.top

[U80] PHP：代码规范修复
来源：http://wwi.sufxvd.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://uoh.jianghu66.top

[U81] JS：初始化项目
来源：http://flv.haohaochexian.top

npm init -y;  npm i express
来源：http://shh.vqdsnc.cn

[U82] JS：package.json 脚本
来源：http://pur.52xcode.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://tup.tian-w.cn

[U83] JS：ES Module 导入导出
来源：http://url.hysaishi.cn

export const a = 1;  import { a } from "./m.js";
来源：http://gln.0kj1m.cn

[U84] JS：CommonJS 写法
来源：http://pwo.aizwys.cn

module.exports = { a };  const { a } = require("./m");
来源：http://efr.yonumen.top

[U85] JS：可选链
来源：http://mgk.tian-w.cn

a?.b?.c
来源：http://jje.ctjpmb.com

[U86] JS：空值合并
来源：http://uqg.yj20258888.top

a ?? b
来源：http://wjr.wangshuangyany.cn

[U87] JS：解构默认值
来源：http://gmq.tianlin.xyz

const { a = 1, b = 2 } = obj;
来源：http://ghk.vqdsnc.cn

[U88] JS：对象展开合并
来源：http://kjl.hesvh.cn

{ ...a, ...b }
来源：http://imn.sxryk.cn

[U89] JS：数组去重
来源：http://ofv.316326.xyz

[...new Set(arr)]
来源：http://cfs.zhiwuduotai.top

[U90] JS：数字数组排序
来源：http://hxa.jyoumei.cn

[...arr].sort((a, b) => a - b)
来源：http://fwk.shzxlz.cn

[U91] JS：对象键值遍历
来源：http://utk.sysykeji.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://lfi.xinyue.icu

[U92] JS：深拷贝
来源：http://ykd.quarkkingdee.top

structuredClone(obj)
来源：http://tsq.zhongyouzk.top

[U93] JS：模板字符串
来源：http://asb.epnwcf.com

`共 ${n} 条`
来源：http://jnb.hongshengwenyu.top

[U94] JS：箭头函数
来源：http://pop.yj20258.top

const double = x => x * 2;
来源：http://nyr.tanke756.top

[U95] JS：Promise 包装
来源：http://ypu.zhixingplan.top

new Promise((resolve, reject) => {})
来源：http://wcz.aibaodan.cn

[U96] JS：async/await 与异常
来源：http://rdl.yongpay.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://lnj.cashguo.top

[U97] JS：并发请求
来源：http://fhe.ctjpmb.com

await Promise.all(urls.map(u => fetch(u)))
来源：http://kei.gogol.net.cn

[U98] JS：fetch 带 JSON
来源：http://vuk.cucudq.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://ffw.haohaochexian.top

[U99] JS：事件监听
来源：http://rai.ydzc1.top

el.addEventListener("click", e => {})
来源：http://irr.jinqigfzy.top

[U100] JS：DOM 查询
来源：http://szb.fzhhl.top

document.querySelector(".item")
来源：http://oot.redwolf501.top

[U101] JS：classList 操作
来源：http://jmu.sjlbkw.cn

el.classList.toggle("active")
来源：http://wmw.52xcode.cn

[U102] JS：本地存储
来源：http://zqb.haohaochexian.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://cgs.nwbrower.top

[U103] JS：定时器
来源：http://kbu.sysykeji.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://wnh.sweek.top

[U104] JS：防抖
来源：http://dow.fanxiaobao.xyz

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://dpm.yj20258.top

[U105] JS：节流
来源：http://ddy.sjlbkw.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://cqn.fengsongda.top

[U106] JS：日期格式化
来源：http://sbd.hysaishi.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://rnc.c1oappe.top

[U107] JS：数字千分位
来源：http://owo.jinqigufen.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://jmp.jyoumei.cn

[U108] JS：随机整数
来源：http://nas.zhoulong.xyz

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://xps.epnwcf.com

[U109] JS：数组分组
来源：http://fxy.xylfe.cn

Object.groupBy(arr, x => x.type)
来源：http://sax.sweek.top

[U110] JS：数组分块
来源：http://fmp.haohaochexian.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://giu.0kj1m.cn

[U111] JS：对象转 Map
来源：http://dgl.fktsv.cn

new Map(Object.entries(obj))
来源：http://ceq.yangfankeji.com

[U112] JS：字符串补位
来源：http://kca.zhaomingkeji.xyz

"7".padStart(3, "0")
来源：http://bfc.hongshengwenyu.top

[U113] JS：正则替换全部
来源：http://ntp.hnxiangtu.top

s.replaceAll("a", "b")
来源：http://evh.bbcook.cn

[U114] JS：JSON 深比较
来源：http://wlw.gotoacloud.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://fox.jiagoushi.top

[U115] JS：生成 UUID
来源：http://cpw.hysaishi.cn

crypto.randomUUID()
来源：http://tvl.c1oappe.top

[U116] JS：类型检查（JSDoc）
来源：http://ktt.zhongyouzk.top

/** @param {string} name */ function f(name) {}
来源：http://vjp.uphjek.com

[U117] JS：单元测试
来源：http://mjw.sjlbkw.cn

npm i -D vitest;  npx vitest
来源：http://vpw.zhoulong.xyz

[U118] JS：开发服务器
来源：http://hhd.yuxming.cn

npm i -D vite;  npx vite
来源：http://vrb.xuanzx.com

[U119] JS：生产构建
来源：http://epm.hcnkem.com

npx vite build
来源：http://kdg.hcnkem.com

[U120] JS：读取环境变量（Vite）
来源：http://lds.0kj1m.cn

import.meta.env.VITE_API_URL
来源：http://xdg.ydzc1.top


<!-- 参考信息 -->