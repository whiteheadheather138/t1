代发 wailian999

[T37] Lua：字符串拼接
来源：http://asb.xuanzx.com

"a" .. "b"
来源：http://tlz.snrcjt.cn

[T38] Lua：条件
来源：http://eaj.yueranfly.top

if x > 0 then print("正") end
来源：http://obv.aizwys.cn

[T39] Lua：模式匹配
来源：http://kpr.cdnleiting.top

string.find(s, "%d+")
来源：http://rxt.fzhhl.top

[T40] Lua：元表
来源：http://tik.smart0.xyz

setmetatable({}, { __index = base })
来源：http://uov.zhaomingkeji.xyz

[T41] Perl：Hello World
来源：http://cuy.kuanghao11.cn

print "Hello\n";
来源：http://tys.chenzaomai.com

[T42] Perl：变量类型
来源：http://ymq.xingfuxueyuan.xyz

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://lyw.hnxiangtu.top

[T43] Perl：字符串插值
来源：http://oyq.zhongyouzk.top

"值: $a"
来源：http://sue.sweek.top

[T44] Perl：条件
来源：http://piu.ppjwa.cn

if ($a > 0) { print "正"; }
来源：http://hfb.wangshuangyany.cn

[T45] Perl：数组遍历
来源：http://uik.chenzaomai.com

for my $x (@arr) { print $x; }
来源：http://xgs.xuetiantiany.cn

[T46] Perl：哈希操作
来源：http://uct.wangshuangyany.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://tla.zhoulong.xyz

[T47] Perl：正则捕获
来源：http://hzl.birdmap.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://cqo.ppjwa.cn

[T48] Perl：正则替换
来源：http://jbr.zhaomingkeji.xyz

$s =~ s/old/new/g;
来源：http://rlp.pycfn.com

[T49] Perl：函数
来源：http://zyt.aibaodan.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://dat.hcnkem.com

[T50] Perl：逐行读文件
来源：http://orj.birdmap.top

open my $fh, "<", "a.txt" or die $!;
来源：http://zrs.hesvh.cn

while (my $line = <$fh>) { print $line; }
来源：http://cgx.yj202588.top

[T51] Scala：Hello World
来源：http://swz.vehdjk.com

println("Hello")
来源：http://rgt.ybcxt.top

[T52] Scala：变量
来源：http://cos.sufxvd.cn

val a = 1;  var b = 2
来源：http://pev.cqqwz.cn

[T53] Scala：字符串插值
来源：http://wfn.ybcxt.top

s"值: $b"
来源：http://wpo.ywan-chungtsiang.top

[T54] Scala：集合映射
来源：http://ckh.cucudq.cn

List(1, 2, 3).map(_ * 2)
来源：http://anu.cucudq.cn

[T55] Scala：集合过滤
来源：http://rlm.xziqi.cn

List(1, 2, 3).filter(_ > 1)
来源：http://mlv.quarkkingdee.top

[T56] Scala：样例类
来源：http://usa.andypj.xyz

case class User(name: String, age: Int)
来源：http://qzp.shuidangran.top

[T57] Scala：模式匹配
来源：http://yao.andypj.xyz

x match { case 1 => "一"; case _ => "其他" }
来源：http://abn.sjlbkw.cn

[T58] Scala：函数定义
来源：http://gbj.jinyuanbaomall.cn

def add(a: Int, b: Int): Int = a + b
来源：http://kxp.daria6918.cn

[T59] Scala：循环
来源：http://swl.zhaomingkeji.xyz

for (i <- 1 to 10) println(i)
来源：http://akw.zhiwuduotai.top

[T60] Scala：折叠
来源：http://oun.sxryk.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://haf.yangfankeji.com

================================================================================
来源：http://ibp.jinghuilouyu.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://ksk.cashguo.top

================================================================================
来源：http://fjd.birdmap.top

[U01] Py：创建虚拟环境
来源：http://ete.andypj.xyz

python -m venv .venv && source .venv/bin/activate
来源：http://qsg.hnxiangtu.top

[U02] Py：导出 / 安装依赖
来源：http://cmb.svipenyu.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://rhx.tianlin.xyz

[U03] Py：加载 .env 配置
来源：http://chz.tianlin.xyz

from dotenv import load_dotenv; load_dotenv()
来源：http://xni.zhengqikj.top

[U04] Py：变量调试打印
来源：http://vyw.ppjwa.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://dzb.hnxiangtu.top

[U05] Py：列表去重且保序
来源：http://zyw.mhx1999.top

list(dict.fromkeys(arr))
来源：http://rre.guowangkeji.top

[U06] Py：合并两个字典
来源：http://mfu.cqqwz.cn

{**a, **b}
来源：http://gvr.chenzaomai.com

[U07] Py：反转字典键值
来源：http://yui.cheryme.top

{v: k for k, v in d.items()}
来源：http://qaw.guannengcc.top

[U08] Py：展平二维列表
来源：http://wgs.sufxvd.cn

[y for x in nested for y in x]
来源：http://yag.shzxlz.cn

[U09] Py：字典取最大值的键
来源：http://fbw.nanxinkj.top

max(d, key=d.get)
来源：http://ulv.iojbl.cn

[U10] Py：按值排序字典
来源：http://nay.andypj.xyz

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://siu.yanxiufei.cn

[U11] Py：生成器表达式
来源：http://uqw.kuanghao11.cn

(x * 2 for x in arr)
来源：http://ymh.sufxvd.cn

[U12] Py：取出现最多的 3 个元素
来源：http://tjn.ctjpmb.com

Counter(arr).most_common(3)
来源：http://kyv.ivvv.top

[U13] Py：固定长度队列
来源：http://kzz.mhx1999.top

deque(maxlen=10)
来源：http://rgy.uphjek.com

[U14] Py：分组收集到列表
来源：http://jjg.hnxiangtu.top

defaultdict(list)
来源：http://fjd.0kj1m.cn

[U15] Py：高精度计时
来源：http://nov.jiagoushi.top

t = time.perf_counter()
来源：http://can.sufxvd.cn

[U16] Py：命令行参数解析
来源：http://kvq.tianlin.xyz

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://pbq.vqdsnc.cn

[U17] Py：初始化日志
来源：http://qst.jianghu66.top

logging.basicConfig(level=logging.INFO)
来源：http://lra.zhongyouzk.top

[U18] Py：预编译正则
来源：http://crw.hysaishi.cn

pat = re.compile(r"\d+")
来源：http://gjn.chenlongwang.top

[U19] Py：正则替换带回调
来源：http://wfb.tianlin.xyz

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://nvq.tianlin.xyz

[U20] Py：缓存函数结果
来源：http://ivs.hnqzz.top

@functools.lru_cache(maxsize=None)
来源：http://ayb.nanxinkj.top

[U21] Py：自定义上下文管理器
来源：http://cjs.tanke756.top

@contextlib.contextmanager
来源：http://uyp.yonumen.top

[U22] Py：矩阵转置
来源：http://meh.jyoumei.cn

list(zip(*m))
来源：http://taw.cqqwz.cn

[U23] Py：分块读取大文件
来源：http://rtp.xingfuxueyuan.xyz

for chunk in iter(lambda: f.read(8192), b""):
来源：http://rrr.zhongyouzk.top

[U24] Py：路径操作
来源：http://eqq.sufxvd.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://bzw.svipenyu.cn

[U25] Py：CSV 按字典读
来源：http://ypf.bbcook.cn

csv.DictReader(f)
来源：http://mly.xuetiantiany.cn

[U26] Py：并发下载
来源：http://qsh.cdnleiting.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://tga.jiagoushi.top

[U27] Py：异步 HTTP
来源：http://lmw.tian-w.cn

aiohttp.ClientSession() 配合 async with
来源：http://ynw.hcnkem.com

[U28] Py：类型别名
来源：http://jwj.andypj.xyz

UserId = int
来源：http://sno.dianchejie.cn

[U29] Py：属性校验
来源：http://ffr.ydzc1.top

@property 与 @x.setter 配合
来源：http://jjg.xingfuxueyuan.xyz

[U30] Py：数据类
来源：http://vkc.shzxlz.cn

@dataclass(slots=True)
来源：http://zdc.hnqzz.top

[U31] Py：单测
来源：http://vqd.cqqwz.cn

python -m pytest -q
来源：http://wbl.ivvv.top

[U32] Py：代码格式化
来源：http://thy.hfpthk.cn

ruff format . && ruff check --fix .
来源：http://vhj.jyoumei.cn

[U33] Py：打包发布
来源：http://ijh.snrcjt.cn

python -m build  （依赖 pyproject.toml）
来源：http://zpu.tianlin.xyz

[U34] Py：判断编码
来源：http://gxy.jinghuilouyu.cn

chardet.detect(raw)
来源：http://kij.ybcxt.top

[U35] Py：发送邮件
来源：http://jcm.bbcook.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://znt.jyoumei.cn

[U36] Py：定时任务
来源：http://zvk.sxryk.cn

schedule.every(10).minutes.do(job)
来源：http://nqf.sysykeji.top

[U37] Py：读写 Excel
来源：http://dzd.zdqjudy.top

pandas.read_excel / DataFrame.to_excel
来源：http://jpm.xinyue.icu

[U38] Py：获取脚本所在目录
来源：http://zoo.aizwys.cn

Path(__file__).resolve().parent
来源：http://nwj.bbcook.cn

[U39] Py：判断是否在交互环境
来源：http://huu.zycfv.cn

sys.stdout.isatty()
来源：http://jcy.nanxinkj.top

[U40] Py：打印到标准错误
来源：http://nut.zhoulong.xyz

print("err", file=sys.stderr)
来源：http://pjz.guannengcc.top

[U41] PHP：初始化 Composer 项目
来源：http://gzb.yanxiufei.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://hva.tianlin.xyz

[U42] PHP：PSR-4 自动加载
来源：http://kga.ydzc1.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hrn.zhengqikj.top

[U43] PHP：声明命名空间
来源：http://hdj.ivvv.top

namespace App\Http;
来源：http://sce.316326.xyz

[U44] PHP：开启严格类型
来源：http://yev.zhoulong.xyz

declare(strict_types=1);
来源：http://uip.iojbl.cn

[U45] PHP：类型声明与返回类型
来源：http://nsr.sysykeji.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://vue.zhengqikj.top

[U46] PHP：可空类型
来源：http://ugf.chenzaomai.com

?string $name = null
来源：http://lag.fanxiaobao.xyz

[U47] PHP：联合类型
来源：http://qwc.hysaishi.cn

int|string $id
来源：http://wfm.52xcode.cn

[U48] PHP：纯枚举
来源：http://ehr.dianchejie.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://ohj.fktsv.cn

[U49] PHP：只读属性
来源：http://rox.zhiwuduotai.top

public readonly string $name
来源：http://yif.shangyingyoupin.top

[U50] PHP：构造器属性提升
来源：http://tmp.cashguo.top

public function __construct(private int $id) {}
来源：http://sdh.bjfxy.top

[U51] PHP：数组解构
来源：http://jle.yangfankeji.com

[$a, $b] = $arr;
来源：http://ybo.fanxiaobao.xyz

[U52] PHP：箭头函数
来源：http://qsu.aibaodan.cn

$double = fn($x) => $x * 2;
来源：http://yua.tian-w.cn

[U53] PHP：空合并运算符
来源：http://ssl.guowangkeji.top

$v = $a ?? $b ?? "default";
来源：http://ore.havefunace.top

[U54] PHP：空安全调用
来源：http://vqe.ydzc1.top

$obj?->method()
来源：http://orr.bbcook.cn

[U55] PHP：match 表达式
来源：http://rwl.gotoacloud.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://vfw.xingfuxueyuan.xyz

[U56] PHP：命名参数
来源：http://cms.zdqjudy.top

f(a: 1, b: 2)
来源：http://yai.zhixingplan.top

[U57] PHP：字符串插值
来源：http://zwx.zhijiandao.cn

"值: {$a}"
来源：http://tlg.feifeiyinyue.top

[U58] PHP：数组三件套
来源：http://ira.aizwys.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://vpl.hammf.cn

[U59] PHP：自定义排序
来源：http://csy.xylfe.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://vgh.9152youxi.cn

[U60] PHP：JSON 编解码
来源：http://kzr.aibaodan.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://yzw.aibaodan.cn

[U61] PHP：正则
来源：http://qfd.meibo888.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://qbd.zdqjudy.top

[U62] PHP：日期对象
来源：http://has.zycfv.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://rch.ydzc1.top

[U63] PHP：文件读写
来源：http://pph.ybcxt.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://mok.yongpay.top

[U64] PHP：目录遍历
来源：http://ocg.zhaomingkeji.xyz

glob("dir/*.php");  scandir("dir");
来源：http://akc.jinqigfzy.top

[U65] PHP：会话
来源：http://zxj.andypj.xyz

session_start();  $_SESSION["uid"] = 1;
来源：http://ovz.zhongyouzk.top

[U66] PHP：设置 Cookie
来源：http://uvu.zhiwuduotai.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://pop.guannengcc.top

[U67] PHP：处理文件上传
来源：http://mek.ybcxt.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://evd.yonumen.top

[U68] PHP：PDO 连接
来源：http://iix.sjlbkw.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://nbv.pycfn.com

[U69] PHP：PDO 预处理
来源：http://edn.redwolf501.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://bql.chenjidiqi.icu

[U70] PHP：PDO 事务
来源：http://hbb.yangfankeji.com

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://whp.jlsjyb.cn

[U71] PHP：抛出异常
来源：http://qdm.guowangkeji.top

throw new RuntimeException("失败", 500);
来源：http://bzj.kuanghao11.cn

[U72] PHP：写错误日志
来源：http://fsh.c1oappe.top

error_log("失败: " . $e->getMessage());
来源：http://ilc.hfpthk.cn

[U73] PHP：读取 ini 配置
来源：http://ghf.hywenlv.cn

parse_ini_file("config.ini", true)
来源：http://pmj.bjfxy.top

[U74] PHP：读取环境变量
来源：http://slo.yj202588.top

getenv("APP_ENV") ?: "production"
来源：http://yvj.xingfuxueyuan.xyz

[U75] PHP：依赖注入
来源：http://xjk.chenjidiqi.icu

composer require psr/container
来源：http://nvd.sweek.top

[U76] PHP：简单路由
来源：http://tla.vehdjk.com

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://jcj.bjfxy.top

[U77] PHP：模板渲染
来源：http://xgf.xingfuxueyuan.xyz

composer require twig/twig
来源：http://axq.fanxiaobao.xyz

[U78] PHP：单元测试
来源：http://sja.guowangkeji.top

composer require --dev phpunit/phpunit
来源：http://pov.hywenlv.cn

[U79] PHP：静态分析
来源：http://rnp.ywan-chungtsiang.top

composer require --dev phpstan/phpstan
来源：http://gmc.cucudq.cn

[U80] PHP：代码规范修复
来源：http://qsm.hnqzz.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://doq.chenjidiqi.icu

[U81] JS：初始化项目
来源：http://gie.gaohongyu789.top

npm init -y;  npm i express
来源：http://puw.dianchejie.cn

[U82] JS：package.json 脚本
来源：http://zfw.xuanzx.com

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://rrb.xylfe.cn

[U83] JS：ES Module 导入导出
来源：http://pnp.cucudq.cn

export const a = 1;  import { a } from "./m.js";
来源：http://oxk.gzhubu.top

[U84] JS：CommonJS 写法
来源：http://sqw.gzhubu.top

module.exports = { a };  const { a } = require("./m");
来源：http://ysk.hnxiangtu.top

[U85] JS：可选链
来源：http://eyn.nanxinkj.top

a?.b?.c
来源：http://vuu.aizwys.cn

[U86] JS：空值合并
来源：http://alj.zdqjudy.top

a ?? b
来源：http://qjt.yvedp.cn

[U87] JS：解构默认值
来源：http://rxd.kuanghao11.cn

const { a = 1, b = 2 } = obj;
来源：http://hyx.tarul.cn

[U88] JS：对象展开合并
来源：http://qqk.ctjpmb.com

{ ...a, ...b }
来源：http://ltm.zhongyouzk.top

[U89] JS：数组去重
来源：http://rue.xinyue.icu

[...new Set(arr)]
来源：http://dzs.chenzaomai.com

[U90] JS：数字数组排序
来源：http://vxs.zhongyouzk.top

[...arr].sort((a, b) => a - b)
来源：http://yvg.vqdsnc.cn

[U91] JS：对象键值遍历
来源：http://chw.andypj.xyz

Object.entries(obj).forEach(([k, v]) => {});
来源：http://lkw.snrcjt.cn

[U92] JS：深拷贝
来源：http://cly.bbcook.cn

structuredClone(obj)
来源：http://ixp.pengpengdd.cyou

[U93] JS：模板字符串
来源：http://xcb.316326.xyz

`共 ${n} 条`
来源：http://xfl.zhiwuduotai.top

[U94] JS：箭头函数
来源：http://ihx.ywan-chungtsiang.top

const double = x => x * 2;
来源：http://dnn.fktsv.cn

[U95] JS：Promise 包装
来源：http://nzd.daxiang520.top

new Promise((resolve, reject) => {})
来源：http://udz.redwolf501.top

[U96] JS：async/await 与异常
来源：http://lwf.kuanghao11.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://jjk.yj202588.top

[U97] JS：并发请求
来源：http://wtn.xingfuxueyuan.xyz

await Promise.all(urls.map(u => fetch(u)))
来源：http://vjb.xylfe.cn

[U98] JS：fetch 带 JSON
来源：http://vhu.xylfe.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://kxj.tanke756.top

[U99] JS：事件监听
来源：http://cdj.ydzc1.top

el.addEventListener("click", e => {})
来源：http://bim.birdmap.top

[U100] JS：DOM 查询
来源：http://oca.yj20258.top

document.querySelector(".item")
来源：http://qiw.chenjidiqi.icu

[U101] JS：classList 操作
来源：http://kgt.tanke756.top

el.classList.toggle("active")
来源：http://yhs.jinqigufen.top

[U102] JS：本地存储
来源：http://lbe.sxryk.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://wpc.yj202588.top

[U103] JS：定时器
来源：http://lih.gogol.net.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://vgp.jinqigufen.top

[U104] JS：防抖
来源：http://aqu.316326.xyz

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://pap.dashuyun.cn

[U105] JS：节流
来源：http://ajz.jlsjyb.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hwy.tian-w.cn

[U106] JS：日期格式化
来源：http://slg.xziqi.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://cye.uphjek.com

[U107] JS：数字千分位
来源：http://rjq.zdqjudy.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://bgc.svipenyu.cn

[U108] JS：随机整数
来源：http://jmm.bjfxy.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://kbk.fktsv.cn

[U109] JS：数组分组
来源：http://qvf.hnqzz.top

Object.groupBy(arr, x => x.type)
来源：http://nyn.chenlongwang.top

[U110] JS：数组分块
来源：http://czb.snrcjt.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://djo.shzxlz.cn

[U111] JS：对象转 Map
来源：http://dkw.ppjwa.cn

new Map(Object.entries(obj))
来源：http://rgl.dashuyun.cn

[U112] JS：字符串补位
来源：http://gkk.xinyue.icu

"7".padStart(3, "0")
来源：http://ezj.dashuyun.cn

[U113] JS：正则替换全部
来源：http://org.jianghu66.top

s.replaceAll("a", "b")
来源：http://tsd.zhiwuduotai.top

[U114] JS：JSON 深比较
来源：http://vuh.pycfn.com

JSON.stringify(a) === JSON.stringify(b)
来源：http://wlz.shanyushiyangtech.top

[U115] JS：生成 UUID
来源：http://zlw.ctjpmb.com

crypto.randomUUID()
来源：http://rfu.gaohongyu789.top

[U116] JS：类型检查（JSDoc）
来源：http://lun.redwolf501.top

/** @param {string} name */ function f(name) {}
来源：http://kqc.xuanzx.com

[U117] JS：单元测试
来源：http://sxu.hammf.cn

npm i -D vitest;  npx vitest
来源：http://gbm.xuetiantiany.cn

[U118] JS：开发服务器
来源：http://jhh.zhoulong.xyz

npm i -D vite;  npx vite
来源：http://zzm.tarul.cn

[U119] JS：生产构建
来源：http://efd.feifeiyinyue.top

npx vite build
来源：http://oyl.gotoacloud.top

[U120] JS：读取环境变量（Vite）
来源：http://grx.cqqwz.cn

import.meta.env.VITE_API_URL
来源：http://vws.shanyushiyangtech.top

================================================================================
来源：http://epq.jianghu66.top

统计汇总
来源：http://zgu.jlsjyb.cn

================================================================================
来源：http://ptv.yonumen.top

按语言统计（条）：
来源：http://tcs.hfpthk.cn

Python ......... 252
来源：http://vtm.xylfe.cn

PHP ............ 252
来源：http://iwf.wangdashe.top

JavaScript ..... 252
来源：http://idv.xylfe.cn

TypeScript ..... 212
来源：http://clh.0kj1m.cn


<!-- 参考信息 -->