代发 wailian999

[T33] Lua：表（数组）
来源：http://vss.sxryk.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://xtc.daria6918.cn

[T34] Lua：遍历表
来源：http://ors.jqgfzy.top

for i, v in ipairs(t) do print(i, v) end
来源：http://qkq.316326.xyz

[T35] Lua：字典表
来源：http://asb.xuanzx.com

local d = { a = 1 };  d.b = 2
来源：http://xzk.zhaomingkeji.xyz

[T36] Lua：函数
来源：http://yqi.cashguo.top

function add(a, b) return a + b end
来源：http://ifz.yuanzhike.top

[T37] Lua：字符串拼接
来源：http://whs.hongshengwenyu.top

"a" .. "b"
来源：http://gdk.feifeiyinyue.top

[T38] Lua：条件
来源：http://wfd.iojbl.cn

if x > 0 then print("正") end
来源：http://gms.epnwcf.com

[T39] Lua：模式匹配
来源：http://ukk.cucudq.cn

string.find(s, "%d+")
来源：http://kdc.xuetiantiany.cn

[T40] Lua：元表
来源：http://tfi.dashuyun.cn

setmetatable({}, { __index = base })
来源：http://vub.fzhhl.top

[T41] Perl：Hello World
来源：http://olw.aizwys.cn

print "Hello\n";
来源：http://nhj.hysaishi.cn

[T42] Perl：变量类型
来源：http://pbd.zhijiandao.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://jcu.aibaodan.cn

[T43] Perl：字符串插值
来源：http://jau.yj20258888.top

"值: $a"
来源：http://eei.tarul.cn

[T44] Perl：条件
来源：http://qwe.ivvv.top

if ($a > 0) { print "正"; }
来源：http://cao.yj202588.top

[T45] Perl：数组遍历
来源：http://xvr.daxiang520.top

for my $x (@arr) { print $x; }
来源：http://lnn.gogol.net.cn

[T46] Perl：哈希操作
来源：http://lgk.sjlbkw.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://xpf.xylfe.cn

[T47] Perl：正则捕获
来源：http://jdl.snrcjt.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://pwf.hnqzz.top

[T48] Perl：正则替换
来源：http://fqd.fengsongda.top

$s =~ s/old/new/g;
来源：http://aob.xuetiantiany.cn

[T49] Perl：函数
来源：http://bkc.9152youxi.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://wvp.fanxiaobao.xyz

[T50] Perl：逐行读文件
来源：http://tvg.wangdashe.top

open my $fh, "<", "a.txt" or die $!;
来源：http://xbh.zhiwuduotai.top

while (my $line = <$fh>) { print $line; }
来源：http://zno.shanyushiyangkeji.top

[T51] Scala：Hello World
来源：http://hum.jiagoushi.top

println("Hello")
来源：http://knb.yongpay.top

[T52] Scala：变量
来源：http://dei.yj20258.top

val a = 1;  var b = 2
来源：http://uax.pengpengdd.cyou

[T53] Scala：字符串插值
来源：http://zxp.nwbrower.top

s"值: $b"
来源：http://gjm.yueranfly.top

[T54] Scala：集合映射
来源：http://ypk.tanke756.top

List(1, 2, 3).map(_ * 2)
来源：http://ukg.shuidangran.top

[T55] Scala：集合过滤
来源：http://zcn.gzhubu.top

List(1, 2, 3).filter(_ > 1)
来源：http://usv.cheryme.top

[T56] Scala：样例类
来源：http://jnf.daria6918.cn

case class User(name: String, age: Int)
来源：http://ldu.uphjek.com

[T57] Scala：模式匹配
来源：http://asz.zhaomingkeji.xyz

x match { case 1 => "一"; case _ => "其他" }
来源：http://ero.yj202588.top

[T58] Scala：函数定义
来源：http://umy.yj20258.top

def add(a: Int, b: Int): Int = a + b
来源：http://kkf.redwolf501.top

[T59] Scala：循环
来源：http://tnx.shzxlz.cn

for (i <- 1 to 10) println(i)
来源：http://soy.guowangkeji.top

[T60] Scala：折叠
来源：http://jwh.316326.xyz

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://lcj.xuanzx.com

================================================================================
来源：http://thr.jiagoushi.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://crt.quarkkingdee.top

================================================================================
来源：http://zgm.hcnkem.com

[U01] Py：创建虚拟环境
来源：http://fnt.52xcode.cn

python -m venv .venv && source .venv/bin/activate
来源：http://ibq.guowangkeji.top

[U02] Py：导出 / 安装依赖
来源：http://wax.bbcook.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://cqn.yj20258.top

[U03] Py：加载 .env 配置
来源：http://qnw.zdqjudy.top

from dotenv import load_dotenv; load_dotenv()
来源：http://uap.hesvh.cn

[U04] Py：变量调试打印
来源：http://mfb.havefunace.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://lwi.chenjidiqi.icu

[U05] Py：列表去重且保序
来源：http://asn.jqgfzy.top

list(dict.fromkeys(arr))
来源：http://gac.zhongyouzk.top

[U06] Py：合并两个字典
来源：http://wmy.haohaochexian.top

{**a, **b}
来源：http://dyh.fanxiaobao.xyz

[U07] Py：反转字典键值
来源：http://jgs.jqgfzy.top

{v: k for k, v in d.items()}
来源：http://oii.ywan-chungtsiang.top

[U08] Py：展平二维列表
来源：http://ion.tianlin.xyz

[y for x in nested for y in x]
来源：http://nlp.shzxlz.cn

[U09] Py：字典取最大值的键
来源：http://zvm.zycfv.cn

max(d, key=d.get)
来源：http://qwd.shzxlz.cn

[U10] Py：按值排序字典
来源：http://ifv.cashguo.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://nep.yj202588.top

[U11] Py：生成器表达式
来源：http://aqo.jianghu66.top

(x * 2 for x in arr)
来源：http://tgy.nanxinkj.top

[U12] Py：取出现最多的 3 个元素
来源：http://dju.zhixingplan.top

Counter(arr).most_common(3)
来源：http://mxu.xuanzx.com

[U13] Py：固定长度队列
来源：http://aba.kuanghao11.cn

deque(maxlen=10)
来源：http://efo.tian-w.cn

[U14] Py：分组收集到列表
来源：http://mfo.gogol.net.cn

defaultdict(list)
来源：http://xho.daxiang520.top

[U15] Py：高精度计时
来源：http://iet.9152youxi.cn

t = time.perf_counter()
来源：http://xmv.hcnkem.com

[U16] Py：命令行参数解析
来源：http://mak.tianlin.xyz

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://yzf.nanxinkj.top

[U17] Py：初始化日志
来源：http://eyc.yvedp.cn

logging.basicConfig(level=logging.INFO)
来源：http://orw.jiagoushi.top

[U18] Py：预编译正则
来源：http://ekq.wangshuangyany.cn

pat = re.compile(r"\d+")
来源：http://kfn.yj202588.top

[U19] Py：正则替换带回调
来源：http://nig.guannengcc.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://lft.zhoulong.xyz

[U20] Py：缓存函数结果
来源：http://hom.vehdjk.com

@functools.lru_cache(maxsize=None)
来源：http://xyw.zhixingplan.top

[U21] Py：自定义上下文管理器
来源：http://ofm.meibo888.top

@contextlib.contextmanager
来源：http://oyu.shuidangran.top

[U22] Py：矩阵转置
来源：http://wde.fengsongda.top

list(zip(*m))
来源：http://zll.fengsongda.top

[U23] Py：分块读取大文件
来源：http://cuz.cashguo.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://atk.zhoulong.xyz

[U24] Py：路径操作
来源：http://ztr.yongpay.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://tfh.chenzaomai.com

[U25] Py：CSV 按字典读
来源：http://tqu.nanxinkj.top

csv.DictReader(f)
来源：http://ehz.ydzc1.top

[U26] Py：并发下载
来源：http://wqh.ybcxt.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://uhb.jiagoushi.top

[U27] Py：异步 HTTP
来源：http://zho.guannengcc.top

aiohttp.ClientSession() 配合 async with
来源：http://vmg.dianchejie.cn

[U28] Py：类型别名
来源：http://bky.zhongyouzk.top

UserId = int
来源：http://omm.tianlin.xyz

[U29] Py：属性校验
来源：http://osx.hammf.cn

@property 与 @x.setter 配合
来源：http://yaq.zhiwuduotai.top

[U30] Py：数据类
来源：http://dbl.cheryme.top

@dataclass(slots=True)
来源：http://mbz.hywenlv.cn

[U31] Py：单测
来源：http://icn.fanxiaobao.xyz

python -m pytest -q
来源：http://lvb.zhixingplan.top

[U32] Py：代码格式化
来源：http://dgu.chenlongwang.top

ruff format . && ruff check --fix .
来源：http://aza.cdnleiting.top

[U33] Py：打包发布
来源：http://udg.fengsongda.top

python -m build  （依赖 pyproject.toml）
来源：http://khs.fzhhl.top

[U34] Py：判断编码
来源：http://dzi.hfpthk.cn

chardet.detect(raw)
来源：http://dwe.jyoumei.cn

[U35] Py：发送邮件
来源：http://zuk.cashguo.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://ncd.pycfn.com

[U36] Py：定时任务
来源：http://jey.ybcxt.top

schedule.every(10).minutes.do(job)
来源：http://ugl.quarkkingdee.top

[U37] Py：读写 Excel
来源：http://haf.chenzaomai.com

pandas.read_excel / DataFrame.to_excel
来源：http://gbk.jiagoushi.top

[U38] Py：获取脚本所在目录
来源：http://rka.gotoacloud.top

Path(__file__).resolve().parent
来源：http://akc.wangshuangyany.cn

[U39] Py：判断是否在交互环境
来源：http://ola.jyoumei.cn

sys.stdout.isatty()
来源：http://leu.feifeiyinyue.top

[U40] Py：打印到标准错误
来源：http://inw.vehdjk.com

print("err", file=sys.stderr)
来源：http://bqb.chenzaomai.com

[U41] PHP：初始化 Composer 项目
来源：http://lnn.yuanzhike.top

composer init;  composer require guzzlehttp/guzzle
来源：http://khd.gzhubu.top

[U42] PHP：PSR-4 自动加载
来源：http://crk.jinghuilouyu.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://wzc.fehbvm.com

[U43] PHP：声明命名空间
来源：http://ctn.wangdashe.top

namespace App\Http;
来源：http://yeu.shuidangran.top

[U44] PHP：开启严格类型
来源：http://egb.uphjek.com

declare(strict_types=1);
来源：http://dmx.jinqigfzy.top

[U45] PHP：类型声明与返回类型
来源：http://dud.xinyue.icu

function add(int $a, int $b): int { return $a + $b; }
来源：http://bfi.cucudq.cn

[U46] PHP：可空类型
来源：http://yad.shanyushiyangtech.top

?string $name = null
来源：http://roa.zhijiandao.cn

[U47] PHP：联合类型
来源：http://xpt.shanyushiyangtech.top

int|string $id
来源：http://nyg.sxryk.cn

[U48] PHP：纯枚举
来源：http://omv.fanxiaobao.xyz

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://frg.fengsongda.top

[U49] PHP：只读属性
来源：http://hjo.wangdashe.top

public readonly string $name
来源：http://qxz.xziqi.cn

[U50] PHP：构造器属性提升
来源：http://khx.snrcjt.cn

public function __construct(private int $id) {}
来源：http://qaq.nanxuanxn.top

[U51] PHP：数组解构
来源：http://yjf.jinqigufen.top

[$a, $b] = $arr;
来源：http://nvo.yueranfly.top

[U52] PHP：箭头函数
来源：http://lpq.guannengcc.top

$double = fn($x) => $x * 2;
来源：http://znt.ybcxt.top

[U53] PHP：空合并运算符
来源：http://spt.wangdashe.top

$v = $a ?? $b ?? "default";
来源：http://pzf.xziqi.cn

[U54] PHP：空安全调用
来源：http://lut.kuanghao11.cn

$obj?->method()
来源：http://bmc.guowangkeji.top

[U55] PHP：match 表达式
来源：http://yud.xuanzx.com

$s = match($x) { 1 => "一", default => "其他" };
来源：http://ijh.ydjk.org.cn

[U56] PHP：命名参数
来源：http://hoq.ydjk.org.cn

f(a: 1, b: 2)
来源：http://hqd.cdnleiting.top

[U57] PHP：字符串插值
来源：http://xhm.hammf.cn

"值: {$a}"
来源：http://kuh.yj20258888.top

[U58] PHP：数组三件套
来源：http://swg.jqgfzy.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://ftq.andypj.xyz

[U59] PHP：自定义排序
来源：http://due.dianchejie.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://vis.fzhhl.top

[U60] PHP：JSON 编解码
来源：http://lxl.cucudq.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://zve.shuidangran.top

[U61] PHP：正则
来源：http://xyu.yuanzhike.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://the.cucudq.cn

[U62] PHP：日期对象
来源：http://cri.yvedp.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://cey.sufxvd.cn

[U63] PHP：文件读写
来源：http://cqa.yj202588.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://kzk.smart0.xyz

[U64] PHP：目录遍历
来源：http://rof.zhongyouzk.top

glob("dir/*.php");  scandir("dir");
来源：http://svf.chenzaomai.com

[U65] PHP：会话
来源：http://ipg.ivvv.top

session_start();  $_SESSION["uid"] = 1;
来源：http://syt.c1oappe.top

[U66] PHP：设置 Cookie
来源：http://xdg.guowangkeji.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://nvh.jlsjyb.cn

[U67] PHP：处理文件上传
来源：http://ybh.sjlbkw.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://agm.havefunace.top

[U68] PHP：PDO 连接
来源：http://dnq.c1oappe.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://lrf.gaohongyu789.top

[U69] PHP：PDO 预处理
来源：http://tgz.yongpay.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://cos.yuanzhike.top

[U70] PHP：PDO 事务
来源：http://ngf.jqgufenzy.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://vhn.zhixingplan.top

[U71] PHP：抛出异常
来源：http://meu.quarkkingdee.top

throw new RuntimeException("失败", 500);
来源：http://hpt.hongshengwenyu.top

[U72] PHP：写错误日志
来源：http://stt.sxryk.cn

error_log("失败: " . $e->getMessage());
来源：http://dxv.zdbjq.cn

[U73] PHP：读取 ini 配置
来源：http://oin.wangshuangyany.cn

parse_ini_file("config.ini", true)
来源：http://mdi.iojbl.cn

[U74] PHP：读取环境变量
来源：http://fgl.yj20258.top

getenv("APP_ENV") ?: "production"
来源：http://huo.havefunace.top

[U75] PHP：依赖注入
来源：http://ysd.wangdashe.top

composer require psr/container
来源：http://ikn.cqqwz.cn

[U76] PHP：简单路由
来源：http://bqs.shangyingyoupin.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://dbb.tian-w.cn

[U77] PHP：模板渲染
来源：http://xbv.tanke756.top

composer require twig/twig
来源：http://hgb.fengsongda.top

[U78] PHP：单元测试
来源：http://nmb.kuanghao11.cn

composer require --dev phpunit/phpunit
来源：http://hjg.meibo888.top

[U79] PHP：静态分析
来源：http://ryl.fktsv.cn

composer require --dev phpstan/phpstan
来源：http://vfk.jlsjyb.cn

[U80] PHP：代码规范修复
来源：http://jfo.redwolf501.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://egk.0kj1m.cn

[U81] JS：初始化项目
来源：http://kzr.shanyushiyangkeji.top

npm init -y;  npm i express
来源：http://oqu.52xcode.cn

[U82] JS：package.json 脚本
来源：http://mmv.vqdsnc.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://vrb.yuxming.cn

[U83] JS：ES Module 导入导出
来源：http://smw.vehdjk.com

export const a = 1;  import { a } from "./m.js";
来源：http://edh.haohaochexian.top

[U84] JS：CommonJS 写法
来源：http://zan.hfpthk.cn

module.exports = { a };  const { a } = require("./m");
来源：http://ygk.guannengcc.top

[U85] JS：可选链
来源：http://mmg.yangfankeji.com

a?.b?.c
来源：http://pna.ybcxt.top

[U86] JS：空值合并
来源：http://net.ppjwa.cn

a ?? b
来源：http://fsf.chenlongwang.top

[U87] JS：解构默认值
来源：http://byx.c1oappe.top

const { a = 1, b = 2 } = obj;
来源：http://and.aibaodan.cn

[U88] JS：对象展开合并
来源：http://sew.ydjk.org.cn

{ ...a, ...b }
来源：http://cpb.daxiang520.top

[U89] JS：数组去重
来源：http://zha.yanxiufei.cn

[...new Set(arr)]
来源：http://kls.uphjek.com

[U90] JS：数字数组排序
来源：http://ujx.hfpthk.cn

[...arr].sort((a, b) => a - b)
来源：http://txc.jqgufenzy.top

[U91] JS：对象键值遍历
来源：http://uom.redwolf501.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://ufh.daria6918.cn

[U92] JS：深拷贝
来源：http://ufv.yfazqb.com

structuredClone(obj)
来源：http://lno.xylfe.cn

[U93] JS：模板字符串
来源：http://alg.ydjk.org.cn

`共 ${n} 条`
来源：http://lij.wangdashe.top

[U94] JS：箭头函数
来源：http://nqp.jyoumei.cn

const double = x => x * 2;
来源：http://ius.yangfankeji.com

[U95] JS：Promise 包装
来源：http://qdp.zhixingplan.top

new Promise((resolve, reject) => {})
来源：http://ooq.jinghuilouyu.cn

[U96] JS：async/await 与异常
来源：http://opx.tarul.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://ntc.jqgfzy.top

[U97] JS：并发请求
来源：http://lup.svipenyu.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://nwx.zhiwuduotai.top

[U98] JS：fetch 带 JSON
来源：http://bmd.yonumen.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://huh.chenzaomai.com

[U99] JS：事件监听
来源：http://vzc.chenlongwang.top

el.addEventListener("click", e => {})
来源：http://dki.jqgufenzy.top

[U100] JS：DOM 查询
来源：http://xgm.sysykeji.top

document.querySelector(".item")
来源：http://lgn.ivvv.top

[U101] JS：classList 操作
来源：http://sri.ydzc1.top

el.classList.toggle("active")
来源：http://grs.sweek.top

[U102] JS：本地存储
来源：http://nyj.shzxlz.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://asa.guowangkeji.top

[U103] JS：定时器
来源：http://uym.shanyushiyangkeji.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://pxw.cqqwz.cn

[U104] JS：防抖
来源：http://kor.wangdashe.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://qbg.gaohongyu789.top

[U105] JS：节流
来源：http://xjq.yangfankeji.com

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://cpu.vqdsnc.cn

[U106] JS：日期格式化
来源：http://fma.yvedp.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://nge.shanyushiyangtech.top

[U107] JS：数字千分位
来源：http://zrh.chenjidiqi.icu

new Intl.NumberFormat("en-US").format(1234567)
来源：http://qtx.svipenyu.cn

[U108] JS：随机整数
来源：http://ait.chenlongwang.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://bim.0kj1m.cn

[U109] JS：数组分组
来源：http://qdp.chenjidiqi.icu

Object.groupBy(arr, x => x.type)
来源：http://bgc.0kj1m.cn

[U110] JS：数组分块
来源：http://hsa.vehdjk.com

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://imx.jinghuilouyu.cn

[U111] JS：对象转 Map
来源：http://xxn.feifeiyinyue.top

new Map(Object.entries(obj))
来源：http://kdc.bjfxy.top

[U112] JS：字符串补位
来源：http://sdl.hnxiangtu.top

"7".padStart(3, "0")
来源：http://fpm.ydzc1.top

[U113] JS：正则替换全部
来源：http://wlg.fanxiaobao.xyz

s.replaceAll("a", "b")
来源：http://yjr.yj20258888.top

[U114] JS：JSON 深比较
来源：http://ysm.haohaochexian.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://idi.xuanzx.com

[U115] JS：生成 UUID
来源：http://cpu.nwbrower.top

crypto.randomUUID()
来源：http://kzt.ctjpmb.com

[U116] JS：类型检查（JSDoc）
来源：http://chw.guowangkeji.top

/** @param {string} name */ function f(name) {}
来源：http://nvb.gotoacloud.top

[U117] JS：单元测试
来源：http://nwi.chenzaomai.com

npm i -D vitest;  npx vitest
来源：http://ahc.chenzaomai.com

[U118] JS：开发服务器
来源：http://pof.kuanghao11.cn

npm i -D vite;  npx vite
来源：http://eax.jinqigfzy.top

[U119] JS：生产构建
来源：http://skj.shuidangran.top

npx vite build
来源：http://agp.fehbvm.com

[U120] JS：读取环境变量（Vite）
来源：http://wbr.yvedp.cn

import.meta.env.VITE_API_URL
来源：http://nwm.fehbvm.com


<!-- 参考信息 -->