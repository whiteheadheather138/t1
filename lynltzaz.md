代发 wailian999

[T33] Lua：表（数组）
来源：http://duk.yueranfly.top

local t = {1, 2, 3};  t[4] = 4
来源：http://hyl.ybcxt.top

[T34] Lua：遍历表
来源：http://gcn.bjfxy.top

for i, v in ipairs(t) do print(i, v) end
来源：http://trw.xuetiantiany.cn

[T35] Lua：字典表
来源：http://yuy.ydjk.org.cn

local d = { a = 1 };  d.b = 2
来源：http://agp.epnwcf.com

[T36] Lua：函数
来源：http://vwu.shanyushiyangtech.top

function add(a, b) return a + b end
来源：http://jup.ydjk.org.cn

[T37] Lua：字符串拼接
来源：http://pti.yj202588.top

"a" .. "b"
来源：http://djp.sweek.top

[T38] Lua：条件
来源：http://gut.tianlin.xyz

if x > 0 then print("正") end
来源：http://por.shangyingyoupin.top

[T39] Lua：模式匹配
来源：http://mzd.bbcook.cn

string.find(s, "%d+")
来源：http://tva.yfazqb.com

[T40] Lua：元表
来源：http://qdp.zycfv.cn

setmetatable({}, { __index = base })
来源：http://swz.ppjwa.cn

[T41] Perl：Hello World
来源：http://czb.yfazqb.com

print "Hello\n";
来源：http://uug.yueranfly.top

[T42] Perl：变量类型
来源：http://idp.jiagoushi.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://aqn.ywan-chungtsiang.top

[T43] Perl：字符串插值
来源：http://tlm.wangshuangyany.cn

"值: $a"
来源：http://qgf.pycfn.com

[T44] Perl：条件
来源：http://rpq.guannengcc.top

if ($a > 0) { print "正"; }
来源：http://sjz.yonumen.top

[T45] Perl：数组遍历
来源：http://ogl.fanxiaobao.xyz

for my $x (@arr) { print $x; }
来源：http://gka.chenlongwang.top

[T46] Perl：哈希操作
来源：http://aqs.zhoulong.xyz

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://tup.guannengcc.top

[T47] Perl：正则捕获
来源：http://tlr.jianghu66.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://ctm.xziqi.cn

[T48] Perl：正则替换
来源：http://fsi.aibaodan.cn

$s =~ s/old/new/g;
来源：http://zbq.gzhubu.top

[T49] Perl：函数
来源：http://wrt.jlsjyb.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://nww.xinyue.icu

[T50] Perl：逐行读文件
来源：http://ksb.xuanzx.com

open my $fh, "<", "a.txt" or die $!;
来源：http://fss.hongshengwenyu.top

while (my $line = <$fh>) { print $line; }
来源：http://dtk.shangyingyoupin.top

[T51] Scala：Hello World
来源：http://odp.yanxiufei.cn

println("Hello")
来源：http://rfv.zycfv.cn

[T52] Scala：变量
来源：http://wdr.yj20258.top

val a = 1;  var b = 2
来源：http://wgd.shzxlz.cn

[T53] Scala：字符串插值
来源：http://hqo.xylfe.cn

s"值: $b"
来源：http://ffi.316326.xyz

[T54] Scala：集合映射
来源：http://fci.tarul.cn

List(1, 2, 3).map(_ * 2)
来源：http://yse.zhixingplan.top

[T55] Scala：集合过滤
来源：http://eio.yfazqb.com

List(1, 2, 3).filter(_ > 1)
来源：http://dmp.52xcode.cn

[T56] Scala：样例类
来源：http://qis.ydjk.org.cn

case class User(name: String, age: Int)
来源：http://mvk.ywan-chungtsiang.top

[T57] Scala：模式匹配
来源：http://ljp.shangyingyoupin.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://moj.fanxiaobao.xyz

[T58] Scala：函数定义
来源：http://huf.zhaomingkeji.xyz

def add(a: Int, b: Int): Int = a + b
来源：http://ykg.hcnkem.com

[T59] Scala：循环
来源：http://sjt.vqdsnc.cn

for (i <- 1 to 10) println(i)
来源：http://bnx.ydzc1.top

[T60] Scala：折叠
来源：http://kwq.cqqwz.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://nou.jinyuanbaomall.cn

================================================================================
来源：http://rpa.yvedp.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://efe.epnwcf.com

================================================================================
来源：http://ptb.fengsongda.top

[U01] Py：创建虚拟环境
来源：http://nie.ppjwa.cn

python -m venv .venv && source .venv/bin/activate
来源：http://wyj.nanxinkj.top

[U02] Py：导出 / 安装依赖
来源：http://oem.wangdashe.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://iks.svipenyu.cn

[U03] Py：加载 .env 配置
来源：http://urj.52xcode.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://gem.wangshuangyany.cn

[U04] Py：变量调试打印
来源：http://uec.gogol.net.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://vem.hnxiangtu.top

[U05] Py：列表去重且保序
来源：http://rdq.iojbl.cn

list(dict.fromkeys(arr))
来源：http://nsp.xylfe.cn

[U06] Py：合并两个字典
来源：http://yfi.yongpay.top

{**a, **b}
来源：http://nla.feifeiyinyue.top

[U07] Py：反转字典键值
来源：http://afh.ctjpmb.com

{v: k for k, v in d.items()}
来源：http://krs.xziqi.cn

[U08] Py：展平二维列表
来源：http://sri.feifeiyinyue.top

[y for x in nested for y in x]
来源：http://fco.xziqi.cn

[U09] Py：字典取最大值的键
来源：http://imy.yuxming.cn

max(d, key=d.get)
来源：http://ioi.jlsjyb.cn

[U10] Py：按值排序字典
来源：http://ddm.zhaomingkeji.xyz

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://zud.yj20258888.top

[U11] Py：生成器表达式
来源：http://egz.yuanzhike.top

(x * 2 for x in arr)
来源：http://kys.yanxiufei.cn

[U12] Py：取出现最多的 3 个元素
来源：http://jfi.ehwqpu.com

Counter(arr).most_common(3)
来源：http://gwi.jqgfzy.top

[U13] Py：固定长度队列
来源：http://pmh.ivvv.top

deque(maxlen=10)
来源：http://cpu.yueranfly.top

[U14] Py：分组收集到列表
来源：http://qgt.redwolf501.top

defaultdict(list)
来源：http://nxh.xuanzx.com

[U15] Py：高精度计时
来源：http://fcj.sufxvd.cn

t = time.perf_counter()
来源：http://kys.dianchejie.cn

[U16] Py：命令行参数解析
来源：http://nvf.9152youxi.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://nen.zhiwuduotai.top

[U17] Py：初始化日志
来源：http://klm.pycfn.com

logging.basicConfig(level=logging.INFO)
来源：http://eir.yueranfly.top

[U18] Py：预编译正则
来源：http://alw.sysykeji.top

pat = re.compile(r"\d+")
来源：http://kje.guannengcc.top

[U19] Py：正则替换带回调
来源：http://ulc.zdbjq.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://jkx.bbcook.cn

[U20] Py：缓存函数结果
来源：http://vvi.fktsv.cn

@functools.lru_cache(maxsize=None)
来源：http://gtk.yueranfly.top

[U21] Py：自定义上下文管理器
来源：http://vqm.ctjpmb.com

@contextlib.contextmanager
来源：http://eju.hysaishi.cn

[U22] Py：矩阵转置
来源：http://fcp.ivvv.top

list(zip(*m))
来源：http://zhs.dashuyun.cn

[U23] Py：分块读取大文件
来源：http://gtr.hnqzz.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://lsq.zdbjq.cn

[U24] Py：路径操作
来源：http://ifk.daria6918.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://lyu.gogol.net.cn

[U25] Py：CSV 按字典读
来源：http://cjz.hcnkem.com

csv.DictReader(f)
来源：http://dwv.nanxinkj.top

[U26] Py：并发下载
来源：http://mua.fehbvm.com

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://fhf.zhengqikj.top

[U27] Py：异步 HTTP
来源：http://jbw.ctjpmb.com

aiohttp.ClientSession() 配合 async with
来源：http://kzk.jqgfzy.top

[U28] Py：类型别名
来源：http://uoa.daxiang520.top

UserId = int
来源：http://kwf.hnxiangtu.top

[U29] Py：属性校验
来源：http://sxc.jinyuanbaomall.cn

@property 与 @x.setter 配合
来源：http://dbi.jyoumei.cn

[U30] Py：数据类
来源：http://gol.tian-w.cn

@dataclass(slots=True)
来源：http://bem.ydzc1.top

[U31] Py：单测
来源：http://xtn.yuanzhike.top

python -m pytest -q
来源：http://fym.ydzc1.top

[U32] Py：代码格式化
来源：http://ebx.yueranfly.top

ruff format . && ruff check --fix .
来源：http://nyp.tian-w.cn

[U33] Py：打包发布
来源：http://wby.aibaodan.cn

python -m build  （依赖 pyproject.toml）
来源：http://zbq.guowangkeji.top

[U34] Py：判断编码
来源：http://wtb.chenlongwang.top

chardet.detect(raw)
来源：http://jnd.guowangkeji.top

[U35] Py：发送邮件
来源：http://ubu.nwbrower.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://rkp.dianchejie.cn

[U36] Py：定时任务
来源：http://ayt.aibaodan.cn

schedule.every(10).minutes.do(job)
来源：http://rlo.quarkkingdee.top

[U37] Py：读写 Excel
来源：http://jdy.vehdjk.com

pandas.read_excel / DataFrame.to_excel
来源：http://icc.tian-w.cn

[U38] Py：获取脚本所在目录
来源：http://tch.sysykeji.top

Path(__file__).resolve().parent
来源：http://itc.xuetiantiany.cn

[U39] Py：判断是否在交互环境
来源：http://vtm.aibaodan.cn

sys.stdout.isatty()
来源：http://ocv.ydjk.org.cn

[U40] Py：打印到标准错误
来源：http://kxk.aizwys.cn

print("err", file=sys.stderr)
来源：http://diu.chenjidiqi.icu

[U41] PHP：初始化 Composer 项目
来源：http://znh.yj202588.top

composer init;  composer require guzzlehttp/guzzle
来源：http://cgk.ppjwa.cn

[U42] PHP：PSR-4 自动加载
来源：http://wmj.dashuyun.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://xeu.bbcook.cn

[U43] PHP：声明命名空间
来源：http://hkg.sweek.top

namespace App\Http;
来源：http://pjw.xinyue.icu

[U44] PHP：开启严格类型
来源：http://cgg.hcnkem.com

declare(strict_types=1);
来源：http://jpu.sxryk.cn

[U45] PHP：类型声明与返回类型
来源：http://ctg.jyoumei.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://zhs.smart0.xyz

[U46] PHP：可空类型
来源：http://eei.xylfe.cn

?string $name = null
来源：http://ktm.yonumen.top

[U47] PHP：联合类型
来源：http://yhm.birdmap.top

int|string $id
来源：http://uvc.hnqzz.top

[U48] PHP：纯枚举
来源：http://crs.iojbl.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://clf.ehwqpu.com

[U49] PHP：只读属性
来源：http://xau.gotoacloud.top

public readonly string $name
来源：http://bxx.hcnkem.com

[U50] PHP：构造器属性提升
来源：http://ffd.jianghu66.top

public function __construct(private int $id) {}
来源：http://kby.dianchejie.cn

[U51] PHP：数组解构
来源：http://phl.gogol.net.cn

[$a, $b] = $arr;
来源：http://hqg.ydzc1.top

[U52] PHP：箭头函数
来源：http://aae.tianlin.xyz

$double = fn($x) => $x * 2;
来源：http://ymg.yvedp.cn

[U53] PHP：空合并运算符
来源：http://wcu.hnqzz.top

$v = $a ?? $b ?? "default";
来源：http://uxn.havefunace.top

[U54] PHP：空安全调用
来源：http://utm.fzhhl.top

$obj?->method()
来源：http://wvx.xingfuxueyuan.xyz

[U55] PHP：match 表达式
来源：http://qzv.hfpthk.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://ihm.fzhhl.top

[U56] PHP：命名参数
来源：http://tje.birdmap.top

f(a: 1, b: 2)
来源：http://jio.jyoumei.cn

[U57] PHP：字符串插值
来源：http://rhs.yj20258888.top

"值: {$a}"
来源：http://ydo.smart0.xyz

[U58] PHP：数组三件套
来源：http://oet.dianchejie.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://bvl.fengsongda.top

[U59] PHP：自定义排序
来源：http://tml.snrcjt.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://trs.sjlbkw.cn

[U60] PHP：JSON 编解码
来源：http://cld.tarul.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://frk.guannengcc.top

[U61] PHP：正则
来源：http://sca.jinghuilouyu.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://iyy.ydzc1.top

[U62] PHP：日期对象
来源：http://leb.vqdsnc.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://onb.shzxlz.cn

[U63] PHP：文件读写
来源：http://ltc.wangshuangyany.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://qsw.zdbjq.cn

[U64] PHP：目录遍历
来源：http://smh.jinghuilouyu.cn

glob("dir/*.php");  scandir("dir");
来源：http://wpy.meibo888.top

[U65] PHP：会话
来源：http://vjo.havefunace.top

session_start();  $_SESSION["uid"] = 1;
来源：http://gxr.tanke756.top

[U66] PHP：设置 Cookie
来源：http://cep.gzhubu.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://uzv.havefunace.top

[U67] PHP：处理文件上传
来源：http://ckg.fktsv.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://tvk.xylfe.cn

[U68] PHP：PDO 连接
来源：http://uyo.hammf.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://yer.zycfv.cn

[U69] PHP：PDO 预处理
来源：http://lvn.bjfxy.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://ahp.aizwys.cn

[U70] PHP：PDO 事务
来源：http://pet.jinqigfzy.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://nzj.jiagoushi.top

[U71] PHP：抛出异常
来源：http://qvf.zhoulong.xyz

throw new RuntimeException("失败", 500);
来源：http://cmf.zhaomingkeji.xyz

[U72] PHP：写错误日志
来源：http://pvn.ehwqpu.com

error_log("失败: " . $e->getMessage());
来源：http://krt.cdnleiting.top

[U73] PHP：读取 ini 配置
来源：http://wbd.hongshengwenyu.top

parse_ini_file("config.ini", true)
来源：http://jek.hysaishi.cn

[U74] PHP：读取环境变量
来源：http://ngm.jlsjyb.cn

getenv("APP_ENV") ?: "production"
来源：http://ndn.shzxlz.cn

[U75] PHP：依赖注入
来源：http://bsr.shangyingyoupin.top

composer require psr/container
来源：http://ckq.0kj1m.cn

[U76] PHP：简单路由
来源：http://kme.wangshuangyany.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://gay.yj20258888.top

[U77] PHP：模板渲染
来源：http://ywc.jlsjyb.cn

composer require twig/twig
来源：http://bjf.shanyushiyangkeji.top

[U78] PHP：单元测试
来源：http://rrm.xylfe.cn

composer require --dev phpunit/phpunit
来源：http://foz.snrcjt.cn

[U79] PHP：静态分析
来源：http://wsz.xingfuxueyuan.xyz

composer require --dev phpstan/phpstan
来源：http://lte.smart0.xyz

[U80] PHP：代码规范修复
来源：http://esz.wangshuangyany.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://jhn.jianghu66.top

[U81] JS：初始化项目
来源：http://sjp.sjlbkw.cn

npm init -y;  npm i express
来源：http://vin.iojbl.cn

[U82] JS：package.json 脚本
来源：http://gjq.tianlin.xyz

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://xqr.jinyuanbaomall.cn

[U83] JS：ES Module 导入导出
来源：http://ruf.jinyuanbaomall.cn

export const a = 1;  import { a } from "./m.js";
来源：http://hae.chenzaomai.com

[U84] JS：CommonJS 写法
来源：http://xrj.wangshuangyany.cn

module.exports = { a };  const { a } = require("./m");
来源：http://scr.shanyushiyangtech.top

[U85] JS：可选链
来源：http://igw.ctjpmb.com

a?.b?.c
来源：http://rkr.zdbjq.cn

[U86] JS：空值合并
来源：http://gnd.andypj.xyz

a ?? b
来源：http://yba.dianchejie.cn

[U87] JS：解构默认值
来源：http://lag.dianchejie.cn

const { a = 1, b = 2 } = obj;
来源：http://ens.gzhubu.top

[U88] JS：对象展开合并
来源：http://ncj.kuanghao11.cn

{ ...a, ...b }
来源：http://wqs.cashguo.top

[U89] JS：数组去重
来源：http://swd.guannengcc.top

[...new Set(arr)]
来源：http://car.jqgfzy.top

[U90] JS：数字数组排序
来源：http://saw.feifeiyinyue.top

[...arr].sort((a, b) => a - b)
来源：http://mlk.dianchejie.cn

[U91] JS：对象键值遍历
来源：http://rfl.nanxinkj.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hcx.jinyuanbaomall.cn

[U92] JS：深拷贝
来源：http://zwo.kuanghao11.cn

structuredClone(obj)
来源：http://cef.yongpay.top

[U93] JS：模板字符串
来源：http://jbu.xingfuxueyuan.xyz

`共 ${n} 条`
来源：http://qwo.zdqjudy.top

[U94] JS：箭头函数
来源：http://umr.ydzc1.top

const double = x => x * 2;
来源：http://cfi.snrcjt.cn

[U95] JS：Promise 包装
来源：http://gqi.iojbl.cn

new Promise((resolve, reject) => {})
来源：http://vii.cashguo.top

[U96] JS：async/await 与异常
来源：http://siy.ybcxt.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://xnx.ybcxt.top

[U97] JS：并发请求
来源：http://uoi.xinyue.icu

await Promise.all(urls.map(u => fetch(u)))
来源：http://sct.yj202588.top

[U98] JS：fetch 带 JSON
来源：http://cwn.xuetiantiany.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://xtj.tianlin.xyz

[U99] JS：事件监听
来源：http://gyr.birdmap.top

el.addEventListener("click", e => {})
来源：http://ruc.hammf.cn

[U100] JS：DOM 查询
来源：http://kce.shanyushiyangtech.top

document.querySelector(".item")
来源：http://nrr.jyoumei.cn

[U101] JS：classList 操作
来源：http://idr.yueranfly.top

el.classList.toggle("active")
来源：http://uzt.9152youxi.cn

[U102] JS：本地存储
来源：http://pbp.xylfe.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://oke.pycfn.com

[U103] JS：定时器
来源：http://nrx.zhoulong.xyz

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://vmq.chenjidiqi.icu

[U104] JS：防抖
来源：http://amf.ehwqpu.com

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://czd.jyoumei.cn

[U105] JS：节流
来源：http://eod.smart0.xyz

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://rbs.pengpengdd.cyou

[U106] JS：日期格式化
来源：http://ays.fktsv.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://cpo.pycfn.com

[U107] JS：数字千分位
来源：http://fne.zycfv.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://rfk.tanke756.top

[U108] JS：随机整数
来源：http://xez.quarkkingdee.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://zdk.sweek.top

[U109] JS：数组分组
来源：http://vsy.chenlongwang.top

Object.groupBy(arr, x => x.type)
来源：http://xob.jinghuilouyu.cn

[U110] JS：数组分块
来源：http://vmn.xuetiantiany.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://nwf.hesvh.cn

[U111] JS：对象转 Map
来源：http://thm.svipenyu.cn

new Map(Object.entries(obj))
来源：http://eeu.ctjpmb.com

[U112] JS：字符串补位
来源：http://ghq.yj20258.top

"7".padStart(3, "0")
来源：http://rro.iojbl.cn

[U113] JS：正则替换全部
来源：http://syw.tianlin.xyz

s.replaceAll("a", "b")
来源：http://vuo.sweek.top

[U114] JS：JSON 深比较
来源：http://fqs.hcnkem.com

JSON.stringify(a) === JSON.stringify(b)
来源：http://mms.jinqigfzy.top

[U115] JS：生成 UUID
来源：http://ypx.sweek.top

crypto.randomUUID()
来源：http://tgg.yongpay.top

[U116] JS：类型检查（JSDoc）
来源：http://lmg.hnxiangtu.top

/** @param {string} name */ function f(name) {}
来源：http://zab.vqdsnc.cn

[U117] JS：单元测试
来源：http://uxl.havefunace.top

npm i -D vitest;  npx vitest
来源：http://zmo.svipenyu.cn

[U118] JS：开发服务器
来源：http://uyg.zhaomingkeji.xyz

npm i -D vite;  npx vite
来源：http://fvj.zhiwuduotai.top

[U119] JS：生产构建
来源：http://gij.ydzc1.top

npx vite build
来源：http://cwz.hongshengwenyu.top

[U120] JS：读取环境变量（Vite）
来源：http://dig.fengsongda.top

import.meta.env.VITE_API_URL
来源：http://vkw.tian-w.cn


<!-- 参考信息 -->