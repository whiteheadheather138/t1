代发 wailian999

[T35] Lua：字典表
来源：http://kxe.kuanghao11.cn

local d = { a = 1 };  d.b = 2
来源：http://guh.ydzc1.top

[T36] Lua：函数
来源：http://pei.zhengqikj.top

function add(a, b) return a + b end
来源：http://jxw.zhixingplan.top

[T37] Lua：字符串拼接
来源：http://mvw.bjfxy.top

"a" .. "b"
来源：http://hwv.epnwcf.com

[T38] Lua：条件
来源：http://urg.xuanzx.com

if x > 0 then print("正") end
来源：http://dzs.yuxming.cn

[T39] Lua：模式匹配
来源：http://qme.epnwcf.com

string.find(s, "%d+")
来源：http://xev.shangyingyoupin.top

[T40] Lua：元表
来源：http://iuy.bbcook.cn

setmetatable({}, { __index = base })
来源：http://kag.yj20258888.top

[T41] Perl：Hello World
来源：http://cne.jyoumei.cn

print "Hello\n";
来源：http://qrp.jinqigfzy.top

[T42] Perl：变量类型
来源：http://rhe.ywan-chungtsiang.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://bul.chenjidiqi.icu

[T43] Perl：字符串插值
来源：http://pua.pengpengdd.cyou

"值: $a"
来源：http://hky.hnxiangtu.top

[T44] Perl：条件
来源：http://aml.zhixingplan.top

if ($a > 0) { print "正"; }
来源：http://xev.zhiwuduotai.top

[T45] Perl：数组遍历
来源：http://kzs.yanxiufei.cn

for my $x (@arr) { print $x; }
来源：http://ofk.ctjpmb.com

[T46] Perl：哈希操作
来源：http://bvv.kuanghao11.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://dcf.hesvh.cn

[T47] Perl：正则捕获
来源：http://yvm.svipenyu.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://cxw.daria6918.cn

[T48] Perl：正则替换
来源：http://ipt.havefunace.top

$s =~ s/old/new/g;
来源：http://txz.xuetiantiany.cn

[T49] Perl：函数
来源：http://imn.tianlin.xyz

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://thy.fzhhl.top

[T50] Perl：逐行读文件
来源：http://pvq.sufxvd.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://wox.feifeiyinyue.top

while (my $line = <$fh>) { print $line; }
来源：http://pvs.jqgfzy.top

[T51] Scala：Hello World
来源：http://cpv.xylfe.cn

println("Hello")
来源：http://ndy.shanyushiyangkeji.top

[T52] Scala：变量
来源：http://ekk.hywenlv.cn

val a = 1;  var b = 2
来源：http://dzn.birdmap.top

[T53] Scala：字符串插值
来源：http://zvh.jqgufenzy.top

s"值: $b"
来源：http://gsn.iojbl.cn

[T54] Scala：集合映射
来源：http://nry.zdbjq.cn

List(1, 2, 3).map(_ * 2)
来源：http://fng.havefunace.top

[T55] Scala：集合过滤
来源：http://sog.jqgufenzy.top

List(1, 2, 3).filter(_ > 1)
来源：http://lmi.yj202588.top

[T56] Scala：样例类
来源：http://wrg.ctjpmb.com

case class User(name: String, age: Int)
来源：http://sbj.chenlongwang.top

[T57] Scala：模式匹配
来源：http://bgt.meibo888.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://tth.yvedp.cn

[T58] Scala：函数定义
来源：http://zkx.dianchejie.cn

def add(a: Int, b: Int): Int = a + b
来源：http://guk.zhiwuduotai.top

[T59] Scala：循环
来源：http://gwj.zdqjudy.top

for (i <- 1 to 10) println(i)
来源：http://fck.yj20258888.top

[T60] Scala：折叠
来源：http://jmo.dashuyun.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://drb.hongshengwenyu.top

================================================================================
来源：http://kdg.zdqjudy.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://mpx.ctjpmb.com

================================================================================
来源：http://uwk.cucudq.cn

[U01] Py：创建虚拟环境
来源：http://peo.vehdjk.com

python -m venv .venv && source .venv/bin/activate
来源：http://edj.kuanghao11.cn

[U02] Py：导出 / 安装依赖
来源：http://uik.xuetiantiany.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://ulv.snrcjt.cn

[U03] Py：加载 .env 配置
来源：http://dhl.wangshuangyany.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://wkv.316326.xyz

[U04] Py：变量调试打印
来源：http://xbn.zdbjq.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://vwl.aizwys.cn

[U05] Py：列表去重且保序
来源：http://ekr.zhiwuduotai.top

list(dict.fromkeys(arr))
来源：http://dgc.daria6918.cn

[U06] Py：合并两个字典
来源：http://pfd.sysykeji.top

{**a, **b}
来源：http://umd.c1oappe.top

[U07] Py：反转字典键值
来源：http://ryt.shzxlz.cn

{v: k for k, v in d.items()}
来源：http://hsc.yuanzhike.top

[U08] Py：展平二维列表
来源：http://syf.xingfuxueyuan.xyz

[y for x in nested for y in x]
来源：http://uwa.xziqi.cn

[U09] Py：字典取最大值的键
来源：http://cii.iojbl.cn

max(d, key=d.get)
来源：http://vzk.havefunace.top

[U10] Py：按值排序字典
来源：http://iba.chenjidiqi.icu

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://cah.guannengcc.top

[U11] Py：生成器表达式
来源：http://foo.dashuyun.cn

(x * 2 for x in arr)
来源：http://gpb.sxryk.cn

[U12] Py：取出现最多的 3 个元素
来源：http://kon.yfazqb.com

Counter(arr).most_common(3)
来源：http://jct.xingfuxueyuan.xyz

[U13] Py：固定长度队列
来源：http://itm.zhoulong.xyz

deque(maxlen=10)
来源：http://ogo.shanyushiyangkeji.top

[U14] Py：分组收集到列表
来源：http://uda.tanke756.top

defaultdict(list)
来源：http://fmi.shuidangran.top

[U15] Py：高精度计时
来源：http://ktz.yueranfly.top

t = time.perf_counter()
来源：http://cvn.gaohongyu789.top

[U16] Py：命令行参数解析
来源：http://zqw.smart0.xyz

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://euf.zdqjudy.top

[U17] Py：初始化日志
来源：http://zfw.birdmap.top

logging.basicConfig(level=logging.INFO)
来源：http://rix.xylfe.cn

[U18] Py：预编译正则
来源：http://brp.yuxming.cn

pat = re.compile(r"\d+")
来源：http://nfd.zhixingplan.top

[U19] Py：正则替换带回调
来源：http://jmu.hcnkem.com

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://vqf.iojbl.cn

[U20] Py：缓存函数结果
来源：http://eaf.snrcjt.cn

@functools.lru_cache(maxsize=None)
来源：http://fao.tarul.cn

[U21] Py：自定义上下文管理器
来源：http://awp.svipenyu.cn

@contextlib.contextmanager
来源：http://dwf.ppjwa.cn

[U22] Py：矩阵转置
来源：http://zow.shanyushiyangtech.top

list(zip(*m))
来源：http://yiw.yongpay.top

[U23] Py：分块读取大文件
来源：http://wib.nwbrower.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://bvs.jinghuilouyu.cn

[U24] Py：路径操作
来源：http://eyz.yj20258888.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://nnw.jlsjyb.cn

[U25] Py：CSV 按字典读
来源：http://lfn.hnxiangtu.top

csv.DictReader(f)
来源：http://lew.quarkkingdee.top

[U26] Py：并发下载
来源：http://fzn.yangfankeji.com

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://vvl.cucudq.cn

[U27] Py：异步 HTTP
来源：http://tuk.gzhubu.top

aiohttp.ClientSession() 配合 async with
来源：http://cee.epnwcf.com

[U28] Py：类型别名
来源：http://hvy.xingfuxueyuan.xyz

UserId = int
来源：http://gdj.chenzaomai.com

[U29] Py：属性校验
来源：http://hzs.fanxiaobao.xyz

@property 与 @x.setter 配合
来源：http://dam.9152youxi.cn

[U30] Py：数据类
来源：http://uyj.zhijiandao.cn

@dataclass(slots=True)
来源：http://wbn.fengsongda.top

[U31] Py：单测
来源：http://qep.jyoumei.cn

python -m pytest -q
来源：http://raq.ivvv.top

[U32] Py：代码格式化
来源：http://rqe.shanyushiyangkeji.top

ruff format . && ruff check --fix .
来源：http://bpx.meibo888.top

[U33] Py：打包发布
来源：http://cob.guannengcc.top

python -m build  （依赖 pyproject.toml）
来源：http://zhu.zhixingplan.top

[U34] Py：判断编码
来源：http://zem.xziqi.cn

chardet.detect(raw)
来源：http://lcd.yj202588.top

[U35] Py：发送邮件
来源：http://qwq.gotoacloud.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://xip.yuanzhike.top

[U36] Py：定时任务
来源：http://fup.zdbjq.cn

schedule.every(10).minutes.do(job)
来源：http://xfv.smart0.xyz

[U37] Py：读写 Excel
来源：http://kep.zdbjq.cn

pandas.read_excel / DataFrame.to_excel
来源：http://ipu.52xcode.cn

[U38] Py：获取脚本所在目录
来源：http://jza.xuetiantiany.cn

Path(__file__).resolve().parent
来源：http://jnv.jinqigufen.top

[U39] Py：判断是否在交互环境
来源：http://vgg.guannengcc.top

sys.stdout.isatty()
来源：http://qln.ydjk.org.cn

[U40] Py：打印到标准错误
来源：http://nwe.tian-w.cn

print("err", file=sys.stderr)
来源：http://fwx.hysaishi.cn

[U41] PHP：初始化 Composer 项目
来源：http://aef.9152youxi.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://atk.chenjidiqi.icu

[U42] PHP：PSR-4 自动加载
来源：http://nya.yonumen.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://rav.sxryk.cn

[U43] PHP：声明命名空间
来源：http://qaw.jiagoushi.top

namespace App\Http;
来源：http://mcf.ywan-chungtsiang.top

[U44] PHP：开启严格类型
来源：http://pui.gogol.net.cn

declare(strict_types=1);
来源：http://rkb.tianlin.xyz

[U45] PHP：类型声明与返回类型
来源：http://ljg.nanxuanxn.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://hdx.quarkkingdee.top

[U46] PHP：可空类型
来源：http://erg.fanxiaobao.xyz

?string $name = null
来源：http://ehm.yangfankeji.com

[U47] PHP：联合类型
来源：http://ync.zdqjudy.top

int|string $id
来源：http://niz.zhiwuduotai.top

[U48] PHP：纯枚举
来源：http://lnj.tanke756.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://omo.smart0.xyz

[U49] PHP：只读属性
来源：http://ujq.hysaishi.cn

public readonly string $name
来源：http://eln.feifeiyinyue.top

[U50] PHP：构造器属性提升
来源：http://epf.jlsjyb.cn

public function __construct(private int $id) {}
来源：http://azw.fzhhl.top

[U51] PHP：数组解构
来源：http://eei.cqqwz.cn

[$a, $b] = $arr;
来源：http://bcy.52xcode.cn

[U52] PHP：箭头函数
来源：http://uvt.redwolf501.top

$double = fn($x) => $x * 2;
来源：http://jrb.yonumen.top

[U53] PHP：空合并运算符
来源：http://aus.nanxuanxn.top

$v = $a ?? $b ?? "default";
来源：http://toq.nwbrower.top

[U54] PHP：空安全调用
来源：http://vlq.xziqi.cn

$obj?->method()
来源：http://fjb.kuanghao11.cn

[U55] PHP：match 表达式
来源：http://ahc.sjlbkw.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://str.vqdsnc.cn

[U56] PHP：命名参数
来源：http://zzs.jyoumei.cn

f(a: 1, b: 2)
来源：http://apv.yuxming.cn

[U57] PHP：字符串插值
来源：http://vub.chenzaomai.com

"值: {$a}"
来源：http://sfu.birdmap.top

[U58] PHP：数组三件套
来源：http://tye.gaohongyu789.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://phc.fzhhl.top

[U59] PHP：自定义排序
来源：http://uvv.cheryme.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://baf.yonumen.top

[U60] PHP：JSON 编解码
来源：http://jyc.gotoacloud.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://wqa.c1oappe.top

[U61] PHP：正则
来源：http://rtv.yuxming.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://xmt.yj20258888.top

[U62] PHP：日期对象
来源：http://qzo.sweek.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://gmh.jinqigufen.top

[U63] PHP：文件读写
来源：http://tvr.wangdashe.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://ret.ivvv.top

[U64] PHP：目录遍历
来源：http://ooo.9152youxi.cn

glob("dir/*.php");  scandir("dir");
来源：http://dzk.shangyingyoupin.top

[U65] PHP：会话
来源：http://lvv.nwbrower.top

session_start();  $_SESSION["uid"] = 1;
来源：http://wko.birdmap.top

[U66] PHP：设置 Cookie
来源：http://rid.hammf.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://xxi.gzhubu.top

[U67] PHP：处理文件上传
来源：http://uey.wangdashe.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://njd.zycfv.cn

[U68] PHP：PDO 连接
来源：http://zbz.zdqjudy.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://jpk.sysykeji.top

[U69] PHP：PDO 预处理
来源：http://ppy.xziqi.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://rcc.sweek.top

[U70] PHP：PDO 事务
来源：http://sci.sweek.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://ffk.nanxuanxn.top

[U71] PHP：抛出异常
来源：http://oqu.aibaodan.cn

throw new RuntimeException("失败", 500);
来源：http://zst.ydzc1.top

[U72] PHP：写错误日志
来源：http://dzn.gotoacloud.top

error_log("失败: " . $e->getMessage());
来源：http://dmt.zdbjq.cn

[U73] PHP：读取 ini 配置
来源：http://vra.zhongyouzk.top

parse_ini_file("config.ini", true)
来源：http://gfr.yuxming.cn

[U74] PHP：读取环境变量
来源：http://fgp.bbcook.cn

getenv("APP_ENV") ?: "production"
来源：http://ygg.aibaodan.cn

[U75] PHP：依赖注入
来源：http://ygl.fehbvm.com

composer require psr/container
来源：http://pvy.wangshuangyany.cn

[U76] PHP：简单路由
来源：http://mqs.cucudq.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://jzk.zhiwuduotai.top

[U77] PHP：模板渲染
来源：http://xli.zhongyouzk.top

composer require twig/twig
来源：http://ody.fehbvm.com

[U78] PHP：单元测试
来源：http://sfh.cheryme.top

composer require --dev phpunit/phpunit
来源：http://gdq.cucudq.cn

[U79] PHP：静态分析
来源：http://uiv.nanxuanxn.top

composer require --dev phpstan/phpstan
来源：http://bfs.xinyue.icu

[U80] PHP：代码规范修复
来源：http://hau.fehbvm.com

composer require --dev friendsofphp/php-cs-fixer
来源：http://suf.xuanzx.com

[U81] JS：初始化项目
来源：http://mhm.yongpay.top

npm init -y;  npm i express
来源：http://tot.yangfankeji.com

[U82] JS：package.json 脚本
来源：http://uoc.guannengcc.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://iok.yj20258888.top

[U83] JS：ES Module 导入导出
来源：http://qbt.hywenlv.cn

export const a = 1;  import { a } from "./m.js";
来源：http://kqx.vehdjk.com

[U84] JS：CommonJS 写法
来源：http://ymi.yuxming.cn

module.exports = { a };  const { a } = require("./m");
来源：http://hol.jyoumei.cn

[U85] JS：可选链
来源：http://oqq.ydzc1.top

a?.b?.c
来源：http://udq.jinyuanbaomall.cn

[U86] JS：空值合并
来源：http://wns.zhengqikj.top

a ?? b
来源：http://rrb.zhoulong.xyz

[U87] JS：解构默认值
来源：http://eqb.jqgfzy.top

const { a = 1, b = 2 } = obj;
来源：http://vlg.feifeiyinyue.top

[U88] JS：对象展开合并
来源：http://bvw.svipenyu.cn

{ ...a, ...b }
来源：http://rmz.pengpengdd.cyou

[U89] JS：数组去重
来源：http://iwk.hesvh.cn

[...new Set(arr)]
来源：http://gfy.jianghu66.top

[U90] JS：数字数组排序
来源：http://pcu.fktsv.cn

[...arr].sort((a, b) => a - b)
来源：http://rup.9152youxi.cn

[U91] JS：对象键值遍历
来源：http://lym.yueranfly.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://ynh.9152youxi.cn

[U92] JS：深拷贝
来源：http://abu.smart0.xyz

structuredClone(obj)
来源：http://rsk.52xcode.cn

[U93] JS：模板字符串
来源：http://uib.guowangkeji.top

`共 ${n} 条`
来源：http://zef.yfazqb.com

[U94] JS：箭头函数
来源：http://vjy.cheryme.top

const double = x => x * 2;
来源：http://zfi.chenjidiqi.icu

[U95] JS：Promise 包装
来源：http://mcx.yfazqb.com

new Promise((resolve, reject) => {})
来源：http://yfz.aizwys.cn

[U96] JS：async/await 与异常
来源：http://ils.jqgfzy.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://wxr.yuanzhike.top

[U97] JS：并发请求
来源：http://fbb.hcnkem.com

await Promise.all(urls.map(u => fetch(u)))
来源：http://hyt.chenlongwang.top

[U98] JS：fetch 带 JSON
来源：http://upg.meibo888.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://fow.yonumen.top

[U99] JS：事件监听
来源：http://oql.yj202588.top

el.addEventListener("click", e => {})
来源：http://tqt.jlsjyb.cn

[U100] JS：DOM 查询
来源：http://zej.yuxming.cn

document.querySelector(".item")
来源：http://pyd.vehdjk.com

[U101] JS：classList 操作
来源：http://ivh.fzhhl.top

el.classList.toggle("active")
来源：http://nkx.yanxiufei.cn

[U102] JS：本地存储
来源：http://gyp.hfpthk.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://kex.hnqzz.top

[U103] JS：定时器
来源：http://rla.sjlbkw.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://yiy.redwolf501.top

[U104] JS：防抖
来源：http://yck.xziqi.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://bpp.cheryme.top

[U105] JS：节流
来源：http://psv.pengpengdd.cyou

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://jpy.0kj1m.cn

[U106] JS：日期格式化
来源：http://zzz.nanxinkj.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://fqr.yj20258888.top

[U107] JS：数字千分位
来源：http://baq.hammf.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://xfw.iojbl.cn

[U108] JS：随机整数
来源：http://gjk.chenzaomai.com

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://uwv.0kj1m.cn

[U109] JS：数组分组
来源：http://wkt.xuetiantiany.cn

Object.groupBy(arr, x => x.type)
来源：http://xjw.yuanzhike.top

[U110] JS：数组分块
来源：http://mxr.andypj.xyz

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://keq.fengsongda.top

[U111] JS：对象转 Map
来源：http://qaw.birdmap.top

new Map(Object.entries(obj))
来源：http://mzj.yongpay.top

[U112] JS：字符串补位
来源：http://xip.havefunace.top

"7".padStart(3, "0")
来源：http://vvy.mhx1999.top

[U113] JS：正则替换全部
来源：http://ceh.316326.xyz

s.replaceAll("a", "b")
来源：http://ymp.xylfe.cn

[U114] JS：JSON 深比较
来源：http://hys.ywan-chungtsiang.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://fcj.yongpay.top

[U115] JS：生成 UUID
来源：http://ias.tanke756.top

crypto.randomUUID()
来源：http://cdk.xuanzx.com

[U116] JS：类型检查（JSDoc）
来源：http://drv.ctjpmb.com

/** @param {string} name */ function f(name) {}
来源：http://mct.aibaodan.cn

[U117] JS：单元测试
来源：http://wnv.gzhubu.top

npm i -D vitest;  npx vitest
来源：http://sqh.tianlin.xyz

[U118] JS：开发服务器
来源：http://gyj.zhengqikj.top

npm i -D vite;  npx vite
来源：http://jli.cheryme.top

[U119] JS：生产构建
来源：http://avz.jqgufenzy.top

npx vite build
来源：http://jzb.xinyue.icu

[U120] JS：读取环境变量（Vite）
来源：http://rfd.hammf.cn

import.meta.env.VITE_API_URL
来源：http://mqz.yuxming.cn

================================================================================
来源：http://aus.ctjpmb.com

统计汇总
来源：http://xmx.bbcook.cn

================================================================================
来源：http://bcq.iojbl.cn

按语言统计（条）：
来源：http://tgb.bbcook.cn


<!-- 参考信息 -->