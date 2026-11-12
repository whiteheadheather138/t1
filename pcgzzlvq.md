代发 wailian999

[T35] Lua：字典表
来源：http://bai.guowangkeji.top

local d = { a = 1 };  d.b = 2
来源：http://bwx.hesvh.cn

[T36] Lua：函数
来源：http://jdt.yuxming.cn

function add(a, b) return a + b end
来源：http://gpu.fzhhl.top

[T37] Lua：字符串拼接
来源：http://xck.yvedp.cn

"a" .. "b"
来源：http://vzp.feifeiyinyue.top

[T38] Lua：条件
来源：http://nar.fehbvm.com

if x > 0 then print("正") end
来源：http://oiw.zhixingplan.top

[T39] Lua：模式匹配
来源：http://oyo.haohaochexian.top

string.find(s, "%d+")
来源：http://dux.cdnleiting.top

[T40] Lua：元表
来源：http://ikk.guannengcc.top

setmetatable({}, { __index = base })
来源：http://vhe.yj20258888.top

[T41] Perl：Hello World
来源：http://lhl.gzhubu.top

print "Hello\n";
来源：http://inx.c1oappe.top

[T42] Perl：变量类型
来源：http://xne.yueranfly.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://xef.wangshuangyany.cn

[T43] Perl：字符串插值
来源：http://ddq.bbcook.cn

"值: $a"
来源：http://fjh.ywan-chungtsiang.top

[T44] Perl：条件
来源：http://zim.uphjek.com

if ($a > 0) { print "正"; }
来源：http://zis.tarul.cn

[T45] Perl：数组遍历
来源：http://mca.jyoumei.cn

for my $x (@arr) { print $x; }
来源：http://iwd.jqgfzy.top

[T46] Perl：哈希操作
来源：http://yre.guannengcc.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://jbr.zdqjudy.top

[T47] Perl：正则捕获
来源：http://mkw.kuanghao11.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://hyr.ybcxt.top

[T48] Perl：正则替换
来源：http://uca.sweek.top

$s =~ s/old/new/g;
来源：http://hkx.xziqi.cn

[T49] Perl：函数
来源：http://fvi.shangyingyoupin.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://qxi.0kj1m.cn

[T50] Perl：逐行读文件
来源：http://asa.jqgufenzy.top

open my $fh, "<", "a.txt" or die $!;
来源：http://adc.shanyushiyangkeji.top

while (my $line = <$fh>) { print $line; }
来源：http://jbl.yonumen.top

[T51] Scala：Hello World
来源：http://daa.jyoumei.cn

println("Hello")
来源：http://djn.tian-w.cn

[T52] Scala：变量
来源：http://vln.ivvv.top

val a = 1;  var b = 2
来源：http://ekk.9152youxi.cn

[T53] Scala：字符串插值
来源：http://goj.ybcxt.top

s"值: $b"
来源：http://wgw.chenjidiqi.icu

[T54] Scala：集合映射
来源：http://ymk.316326.xyz

List(1, 2, 3).map(_ * 2)
来源：http://fta.jinghuilouyu.cn

[T55] Scala：集合过滤
来源：http://abu.yonumen.top

List(1, 2, 3).filter(_ > 1)
来源：http://gjo.zhengqikj.top

[T56] Scala：样例类
来源：http://rsa.shuidangran.top

case class User(name: String, age: Int)
来源：http://hwv.zdqjudy.top

[T57] Scala：模式匹配
来源：http://txn.fktsv.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://qza.zhixingplan.top

[T58] Scala：函数定义
来源：http://zud.9152youxi.cn

def add(a: Int, b: Int): Int = a + b
来源：http://mrf.chenzaomai.com

[T59] Scala：循环
来源：http://fov.shangyingyoupin.top

for (i <- 1 to 10) println(i)
来源：http://fml.sysykeji.top

[T60] Scala：折叠
来源：http://pcy.birdmap.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://lsk.tianlin.xyz

================================================================================
来源：http://pwj.sufxvd.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://fut.chenlongwang.top

================================================================================
来源：http://uee.chenlongwang.top

[U01] Py：创建虚拟环境
来源：http://uei.jqgufenzy.top

python -m venv .venv && source .venv/bin/activate
来源：http://mqt.daria6918.cn

[U02] Py：导出 / 安装依赖
来源：http://cea.jinqigufen.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://dvk.yuxming.cn

[U03] Py：加载 .env 配置
来源：http://ddg.xuanzx.com

from dotenv import load_dotenv; load_dotenv()
来源：http://hoa.shuidangran.top

[U04] Py：变量调试打印
来源：http://wam.hesvh.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://mty.ybcxt.top

[U05] Py：列表去重且保序
来源：http://hmv.guannengcc.top

list(dict.fromkeys(arr))
来源：http://adu.pengpengdd.cyou

[U06] Py：合并两个字典
来源：http://luw.xziqi.cn

{**a, **b}
来源：http://ryp.316326.xyz

[U07] Py：反转字典键值
来源：http://vfa.nanxuanxn.top

{v: k for k, v in d.items()}
来源：http://nnn.ehwqpu.com

[U08] Py：展平二维列表
来源：http://qsi.hammf.cn

[y for x in nested for y in x]
来源：http://nob.uphjek.com

[U09] Py：字典取最大值的键
来源：http://xyv.havefunace.top

max(d, key=d.get)
来源：http://tyb.gotoacloud.top

[U10] Py：按值排序字典
来源：http://arq.tianlin.xyz

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://qmr.guowangkeji.top

[U11] Py：生成器表达式
来源：http://ruw.cheryme.top

(x * 2 for x in arr)
来源：http://ypi.jinghuilouyu.cn

[U12] Py：取出现最多的 3 个元素
来源：http://byg.0kj1m.cn

Counter(arr).most_common(3)
来源：http://bei.jiagoushi.top

[U13] Py：固定长度队列
来源：http://yym.cheryme.top

deque(maxlen=10)
来源：http://llr.havefunace.top

[U14] Py：分组收集到列表
来源：http://orz.fanxiaobao.xyz

defaultdict(list)
来源：http://fav.andypj.xyz

[U15] Py：高精度计时
来源：http://tmg.daxiang520.top

t = time.perf_counter()
来源：http://gjy.aizwys.cn

[U16] Py：命令行参数解析
来源：http://cfm.yueranfly.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://wiz.andypj.xyz

[U17] Py：初始化日志
来源：http://bqp.ivvv.top

logging.basicConfig(level=logging.INFO)
来源：http://rcq.tian-w.cn

[U18] Py：预编译正则
来源：http://duq.fengsongda.top

pat = re.compile(r"\d+")
来源：http://uer.iojbl.cn

[U19] Py：正则替换带回调
来源：http://jko.sweek.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://moq.bbcook.cn

[U20] Py：缓存函数结果
来源：http://fmi.jqgufenzy.top

@functools.lru_cache(maxsize=None)
来源：http://uuc.cashguo.top

[U21] Py：自定义上下文管理器
来源：http://wij.zhongyouzk.top

@contextlib.contextmanager
来源：http://aie.ppjwa.cn

[U22] Py：矩阵转置
来源：http://ljp.fanxiaobao.xyz

list(zip(*m))
来源：http://fxd.xuanzx.com

[U23] Py：分块读取大文件
来源：http://ogx.snrcjt.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://xhq.hammf.cn

[U24] Py：路径操作
来源：http://sav.gaohongyu789.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://tvy.ctjpmb.com

[U25] Py：CSV 按字典读
来源：http://giy.jinghuilouyu.cn

csv.DictReader(f)
来源：http://mpr.ivvv.top

[U26] Py：并发下载
来源：http://qqq.jinghuilouyu.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://yiy.meibo888.top

[U27] Py：异步 HTTP
来源：http://epa.sjlbkw.cn

aiohttp.ClientSession() 配合 async with
来源：http://wuk.bjfxy.top

[U28] Py：类型别名
来源：http://gzb.fanxiaobao.xyz

UserId = int
来源：http://hhn.wangdashe.top

[U29] Py：属性校验
来源：http://ddq.quarkkingdee.top

@property 与 @x.setter 配合
来源：http://lhn.ppjwa.cn

[U30] Py：数据类
来源：http://txu.nwbrower.top

@dataclass(slots=True)
来源：http://vof.uphjek.com

[U31] Py：单测
来源：http://sbx.jinqigufen.top

python -m pytest -q
来源：http://fky.xziqi.cn

[U32] Py：代码格式化
来源：http://zbf.fanxiaobao.xyz

ruff format . && ruff check --fix .
来源：http://mkl.ywan-chungtsiang.top

[U33] Py：打包发布
来源：http://msn.ydzc1.top

python -m build  （依赖 pyproject.toml）
来源：http://uwa.yanxiufei.cn

[U34] Py：判断编码
来源：http://edu.jinghuilouyu.cn

chardet.detect(raw)
来源：http://qzp.daria6918.cn

[U35] Py：发送邮件
来源：http://lme.ybcxt.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://tdq.havefunace.top

[U36] Py：定时任务
来源：http://obu.yj20258.top

schedule.every(10).minutes.do(job)
来源：http://fqq.xuanzx.com

[U37] Py：读写 Excel
来源：http://wsn.feifeiyinyue.top

pandas.read_excel / DataFrame.to_excel
来源：http://pfm.zdbjq.cn

[U38] Py：获取脚本所在目录
来源：http://ifv.shanyushiyangtech.top

Path(__file__).resolve().parent
来源：http://fkz.ehwqpu.com

[U39] Py：判断是否在交互环境
来源：http://cqg.wangdashe.top

sys.stdout.isatty()
来源：http://qly.xingfuxueyuan.xyz

[U40] Py：打印到标准错误
来源：http://wxh.zhaomingkeji.xyz

print("err", file=sys.stderr)
来源：http://zse.ctjpmb.com

[U41] PHP：初始化 Composer 项目
来源：http://fsl.ydzc1.top

composer init;  composer require guzzlehttp/guzzle
来源：http://ivp.sweek.top

[U42] PHP：PSR-4 自动加载
来源：http://sxd.0kj1m.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://tbt.pengpengdd.cyou

[U43] PHP：声明命名空间
来源：http://mdh.jianghu66.top

namespace App\Http;
来源：http://yyt.dianchejie.cn

[U44] PHP：开启严格类型
来源：http://gho.c1oappe.top

declare(strict_types=1);
来源：http://knq.pycfn.com

[U45] PHP：类型声明与返回类型
来源：http://bss.dianchejie.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://exk.pycfn.com

[U46] PHP：可空类型
来源：http://iaf.yuxming.cn

?string $name = null
来源：http://jsk.zhongyouzk.top

[U47] PHP：联合类型
来源：http://muo.jinghuilouyu.cn

int|string $id
来源：http://qxe.jqgufenzy.top

[U48] PHP：纯枚举
来源：http://pwi.pycfn.com

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://dos.cqqwz.cn

[U49] PHP：只读属性
来源：http://lyr.sweek.top

public readonly string $name
来源：http://igv.daria6918.cn

[U50] PHP：构造器属性提升
来源：http://frz.iojbl.cn

public function __construct(private int $id) {}
来源：http://zqn.jyoumei.cn

[U51] PHP：数组解构
来源：http://iro.zhijiandao.cn

[$a, $b] = $arr;
来源：http://hqy.ivvv.top

[U52] PHP：箭头函数
来源：http://cub.jyoumei.cn

$double = fn($x) => $x * 2;
来源：http://dfm.zdbjq.cn

[U53] PHP：空合并运算符
来源：http://scn.ydzc1.top

$v = $a ?? $b ?? "default";
来源：http://zet.xuetiantiany.cn

[U54] PHP：空安全调用
来源：http://izw.hywenlv.cn

$obj?->method()
来源：http://diw.feifeiyinyue.top

[U55] PHP：match 表达式
来源：http://xgg.vqdsnc.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://kzp.daxiang520.top

[U56] PHP：命名参数
来源：http://eeb.gotoacloud.top

f(a: 1, b: 2)
来源：http://jte.guowangkeji.top

[U57] PHP：字符串插值
来源：http://ive.aibaodan.cn

"值: {$a}"
来源：http://sdv.cqqwz.cn

[U58] PHP：数组三件套
来源：http://ukh.tanke756.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://exh.xingfuxueyuan.xyz

[U59] PHP：自定义排序
来源：http://suk.daria6918.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://vke.tian-w.cn

[U60] PHP：JSON 编解码
来源：http://dua.zycfv.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://grx.yongpay.top

[U61] PHP：正则
来源：http://bjs.dianchejie.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://cty.zhengqikj.top

[U62] PHP：日期对象
来源：http://het.hesvh.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://nto.zhaomingkeji.xyz

[U63] PHP：文件读写
来源：http://mxt.xinyue.icu

file_get_contents($f);  file_put_contents($f, $data);
来源：http://ujx.tanke756.top

[U64] PHP：目录遍历
来源：http://afr.hammf.cn

glob("dir/*.php");  scandir("dir");
来源：http://kzk.yvedp.cn

[U65] PHP：会话
来源：http://pqk.shzxlz.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://fux.snrcjt.cn

[U66] PHP：设置 Cookie
来源：http://sgn.gaohongyu789.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://quy.shzxlz.cn

[U67] PHP：处理文件上传
来源：http://xjp.dashuyun.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://vyn.ybcxt.top

[U68] PHP：PDO 连接
来源：http://hgr.sysykeji.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://cii.fengsongda.top

[U69] PHP：PDO 预处理
来源：http://mvq.aibaodan.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://jel.hesvh.cn

[U70] PHP：PDO 事务
来源：http://txh.andypj.xyz

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://wgc.jianghu66.top

[U71] PHP：抛出异常
来源：http://fhs.xylfe.cn

throw new RuntimeException("失败", 500);
来源：http://yqq.yongpay.top

[U72] PHP：写错误日志
来源：http://lns.ppjwa.cn

error_log("失败: " . $e->getMessage());
来源：http://edv.aibaodan.cn

[U73] PHP：读取 ini 配置
来源：http://mry.vehdjk.com

parse_ini_file("config.ini", true)
来源：http://dar.yuanzhike.top

[U74] PHP：读取环境变量
来源：http://jad.nanxinkj.top

getenv("APP_ENV") ?: "production"
来源：http://gfk.gotoacloud.top

[U75] PHP：依赖注入
来源：http://nki.nanxuanxn.top

composer require psr/container
来源：http://hsb.guowangkeji.top

[U76] PHP：简单路由
来源：http://bib.jinyuanbaomall.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://cwp.ydzc1.top

[U77] PHP：模板渲染
来源：http://wod.316326.xyz

composer require twig/twig
来源：http://lub.tian-w.cn

[U78] PHP：单元测试
来源：http://ypo.haohaochexian.top

composer require --dev phpunit/phpunit
来源：http://toc.xziqi.cn

[U79] PHP：静态分析
来源：http://lrc.yj20258.top

composer require --dev phpstan/phpstan
来源：http://chy.jlsjyb.cn

[U80] PHP：代码规范修复
来源：http://hwy.wangshuangyany.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://hns.hongshengwenyu.top

[U81] JS：初始化项目
来源：http://etw.gogol.net.cn

npm init -y;  npm i express
来源：http://qkn.fzhhl.top

[U82] JS：package.json 脚本
来源：http://ykx.yueranfly.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://cdp.daria6918.cn

[U83] JS：ES Module 导入导出
来源：http://ewy.daria6918.cn

export const a = 1;  import { a } from "./m.js";
来源：http://lvy.mhx1999.top

[U84] JS：CommonJS 写法
来源：http://odv.ydjk.org.cn

module.exports = { a };  const { a } = require("./m");
来源：http://rbz.gotoacloud.top

[U85] JS：可选链
来源：http://kwa.uphjek.com

a?.b?.c
来源：http://mia.bjfxy.top

[U86] JS：空值合并
来源：http://jkz.zhengqikj.top

a ?? b
来源：http://jpq.yuxming.cn

[U87] JS：解构默认值
来源：http://edx.epnwcf.com

const { a = 1, b = 2 } = obj;
来源：http://uta.jinqigfzy.top

[U88] JS：对象展开合并
来源：http://lpg.jqgfzy.top

{ ...a, ...b }
来源：http://qhr.xuetiantiany.cn

[U89] JS：数组去重
来源：http://npl.jinghuilouyu.cn

[...new Set(arr)]
来源：http://bmc.gzhubu.top

[U90] JS：数字数组排序
来源：http://ykk.bjfxy.top

[...arr].sort((a, b) => a - b)
来源：http://rdp.hammf.cn

[U91] JS：对象键值遍历
来源：http://ukk.sweek.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://cnw.pengpengdd.cyou

[U92] JS：深拷贝
来源：http://igc.zdbjq.cn

structuredClone(obj)
来源：http://qlj.ehwqpu.com

[U93] JS：模板字符串
来源：http://rjb.hammf.cn

`共 ${n} 条`
来源：http://hsp.tarul.cn

[U94] JS：箭头函数
来源：http://kpk.zhoulong.xyz

const double = x => x * 2;
来源：http://kcx.guannengcc.top

[U95] JS：Promise 包装
来源：http://gcr.tanke756.top

new Promise((resolve, reject) => {})
来源：http://nyy.tian-w.cn

[U96] JS：async/await 与异常
来源：http://zvu.jqgfzy.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://ulo.xinyue.icu

[U97] JS：并发请求
来源：http://tnq.cashguo.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://rsl.bjfxy.top

[U98] JS：fetch 带 JSON
来源：http://uch.yongpay.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://vxq.xinyue.icu

[U99] JS：事件监听
来源：http://eji.yongpay.top

el.addEventListener("click", e => {})
来源：http://rsx.uphjek.com

[U100] JS：DOM 查询
来源：http://suu.guowangkeji.top

document.querySelector(".item")
来源：http://fxg.smart0.xyz

[U101] JS：classList 操作
来源：http://bsx.hywenlv.cn

el.classList.toggle("active")
来源：http://tuw.fzhhl.top

[U102] JS：本地存储
来源：http://nuo.redwolf501.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://lol.gzhubu.top

[U103] JS：定时器
来源：http://enq.pycfn.com

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://dwk.yj20258.top

[U104] JS：防抖
来源：http://qaj.smart0.xyz

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://drr.52xcode.cn

[U105] JS：节流
来源：http://hlo.hnxiangtu.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://qhy.jqgufenzy.top

[U106] JS：日期格式化
来源：http://bpf.fanxiaobao.xyz

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://ywj.tianlin.xyz

[U107] JS：数字千分位
来源：http://ldj.mhx1999.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://vfq.svipenyu.cn

[U108] JS：随机整数
来源：http://hmi.hcnkem.com

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://wsd.zycfv.cn

[U109] JS：数组分组
来源：http://khq.cheryme.top

Object.groupBy(arr, x => x.type)
来源：http://skz.aizwys.cn

[U110] JS：数组分块
来源：http://sbp.shanyushiyangkeji.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://cwh.zycfv.cn

[U111] JS：对象转 Map
来源：http://dai.meibo888.top

new Map(Object.entries(obj))
来源：http://idf.tian-w.cn

[U112] JS：字符串补位
来源：http://ejq.yj202588.top

"7".padStart(3, "0")
来源：http://jyg.fzhhl.top

[U113] JS：正则替换全部
来源：http://szb.52xcode.cn

s.replaceAll("a", "b")
来源：http://mwk.shuidangran.top

[U114] JS：JSON 深比较
来源：http://lzj.xuanzx.com

JSON.stringify(a) === JSON.stringify(b)
来源：http://yxt.gzhubu.top

[U115] JS：生成 UUID
来源：http://icm.52xcode.cn

crypto.randomUUID()
来源：http://ivx.sysykeji.top

[U116] JS：类型检查（JSDoc）
来源：http://cdv.pycfn.com

/** @param {string} name */ function f(name) {}
来源：http://ndq.ivvv.top

[U117] JS：单元测试
来源：http://mnh.yj20258888.top

npm i -D vitest;  npx vitest
来源：http://veu.haohaochexian.top

[U118] JS：开发服务器
来源：http://zue.gotoacloud.top

npm i -D vite;  npx vite
来源：http://ged.havefunace.top

[U119] JS：生产构建
来源：http://mca.pycfn.com

npx vite build
来源：http://czj.quarkkingdee.top

[U120] JS：读取环境变量（Vite）
来源：http://ido.ywan-chungtsiang.top

import.meta.env.VITE_API_URL
来源：http://zti.jyoumei.cn

================================================================================
来源：http://cms.shuidangran.top

统计汇总
来源：http://kdq.daria6918.cn

================================================================================
来源：http://sal.guannengcc.top

按语言统计（条）：
来源：http://jgg.sxryk.cn


<!-- 参考信息 -->