代发 wailian999

[T37] Lua：字符串拼接
来源：http://wxs.tarul.cn

"a" .. "b"
来源：http://tmh.jinyuanbaomall.cn

[T38] Lua：条件
来源：http://izm.jyoumei.cn

if x > 0 then print("正") end
来源：http://hda.jinqigfzy.top

[T39] Lua：模式匹配
来源：http://vmy.hfpthk.cn

string.find(s, "%d+")
来源：http://uti.yangfankeji.com

[T40] Lua：元表
来源：http://him.iojbl.cn

setmetatable({}, { __index = base })
来源：http://nmv.ydjk.org.cn

[T41] Perl：Hello World
来源：http://gag.yueranfly.top

print "Hello\n";
来源：http://mvz.chenzaomai.com

[T42] Perl：变量类型
来源：http://uwj.bjfxy.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://vxb.fktsv.cn

[T43] Perl：字符串插值
来源：http://mfd.xuanzx.com

"值: $a"
来源：http://mid.xylfe.cn

[T44] Perl：条件
来源：http://rty.tian-w.cn

if ($a > 0) { print "正"; }
来源：http://kxl.fehbvm.com

[T45] Perl：数组遍历
来源：http://mnf.zhengqikj.top

for my $x (@arr) { print $x; }
来源：http://oon.nanxinkj.top

[T46] Perl：哈希操作
来源：http://wkv.xingfuxueyuan.xyz

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://rxj.chenzaomai.com

[T47] Perl：正则捕获
来源：http://yef.nwbrower.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://xfz.mhx1999.top

[T48] Perl：正则替换
来源：http://par.daxiang520.top

$s =~ s/old/new/g;
来源：http://uyu.dashuyun.cn

[T49] Perl：函数
来源：http://tle.zhiwuduotai.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://vha.yanxiufei.cn

[T50] Perl：逐行读文件
来源：http://rbd.fehbvm.com

open my $fh, "<", "a.txt" or die $!;
来源：http://pjv.hesvh.cn

while (my $line = <$fh>) { print $line; }
来源：http://fvw.ydzc1.top

[T51] Scala：Hello World
来源：http://xdk.fzhhl.top

println("Hello")
来源：http://hla.zdbjq.cn

[T52] Scala：变量
来源：http://rgh.c1oappe.top

val a = 1;  var b = 2
来源：http://nsx.hnxiangtu.top

[T53] Scala：字符串插值
来源：http://xeq.chenzaomai.com

s"值: $b"
来源：http://tdt.aibaodan.cn

[T54] Scala：集合映射
来源：http://jzw.mhx1999.top

List(1, 2, 3).map(_ * 2)
来源：http://itz.nanxinkj.top

[T55] Scala：集合过滤
来源：http://bkl.jiagoushi.top

List(1, 2, 3).filter(_ > 1)
来源：http://rep.yuanzhike.top

[T56] Scala：样例类
来源：http://tdk.redwolf501.top

case class User(name: String, age: Int)
来源：http://wsd.shuidangran.top

[T57] Scala：模式匹配
来源：http://uch.daria6918.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://fiv.tian-w.cn

[T58] Scala：函数定义
来源：http://pvn.guowangkeji.top

def add(a: Int, b: Int): Int = a + b
来源：http://yat.hesvh.cn

[T59] Scala：循环
来源：http://zdn.jinqigufen.top

for (i <- 1 to 10) println(i)
来源：http://ixa.yueranfly.top

[T60] Scala：折叠
来源：http://yvy.haohaochexian.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://xae.jinqigufen.top

================================================================================
来源：http://odt.havefunace.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://zzi.uphjek.com

================================================================================
来源：http://tuw.yj202588.top

[U01] Py：创建虚拟环境
来源：http://zse.yonumen.top

python -m venv .venv && source .venv/bin/activate
来源：http://uge.fanxiaobao.xyz

[U02] Py：导出 / 安装依赖
来源：http://wvv.cheryme.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://iuj.jiagoushi.top

[U03] Py：加载 .env 配置
来源：http://bzv.guowangkeji.top

from dotenv import load_dotenv; load_dotenv()
来源：http://lvk.yj20258.top

[U04] Py：变量调试打印
来源：http://mqq.tanke756.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://upk.sweek.top

[U05] Py：列表去重且保序
来源：http://ues.guowangkeji.top

list(dict.fromkeys(arr))
来源：http://chi.tian-w.cn

[U06] Py：合并两个字典
来源：http://tdy.hnxiangtu.top

{**a, **b}
来源：http://kyg.sjlbkw.cn

[U07] Py：反转字典键值
来源：http://ozu.vqdsnc.cn

{v: k for k, v in d.items()}
来源：http://dga.cheryme.top

[U08] Py：展平二维列表
来源：http://vmg.bjfxy.top

[y for x in nested for y in x]
来源：http://jpd.hnxiangtu.top

[U09] Py：字典取最大值的键
来源：http://hqr.zhaomingkeji.xyz

max(d, key=d.get)
来源：http://wol.cucudq.cn

[U10] Py：按值排序字典
来源：http://ujb.yj20258888.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://vcz.pycfn.com

[U11] Py：生成器表达式
来源：http://kiz.hesvh.cn

(x * 2 for x in arr)
来源：http://hgb.zdqjudy.top

[U12] Py：取出现最多的 3 个元素
来源：http://csm.0kj1m.cn

Counter(arr).most_common(3)
来源：http://fag.andypj.xyz

[U13] Py：固定长度队列
来源：http://mai.iojbl.cn

deque(maxlen=10)
来源：http://tsj.shuidangran.top

[U14] Py：分组收集到列表
来源：http://ler.jyoumei.cn

defaultdict(list)
来源：http://hyh.sufxvd.cn

[U15] Py：高精度计时
来源：http://sfd.daxiang520.top

t = time.perf_counter()
来源：http://mfg.tian-w.cn

[U16] Py：命令行参数解析
来源：http://kyk.daxiang520.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://ooe.snrcjt.cn

[U17] Py：初始化日志
来源：http://ris.gaohongyu789.top

logging.basicConfig(level=logging.INFO)
来源：http://pac.aibaodan.cn

[U18] Py：预编译正则
来源：http://uap.zhiwuduotai.top

pat = re.compile(r"\d+")
来源：http://xhh.cashguo.top

[U19] Py：正则替换带回调
来源：http://gng.hywenlv.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://now.jinqigfzy.top

[U20] Py：缓存函数结果
来源：http://kos.jlsjyb.cn

@functools.lru_cache(maxsize=None)
来源：http://aiv.jinqigfzy.top

[U21] Py：自定义上下文管理器
来源：http://qjp.ctjpmb.com

@contextlib.contextmanager
来源：http://fle.vqdsnc.cn

[U22] Py：矩阵转置
来源：http://waa.ehwqpu.com

list(zip(*m))
来源：http://tks.9152youxi.cn

[U23] Py：分块读取大文件
来源：http://lzr.xingfuxueyuan.xyz

for chunk in iter(lambda: f.read(8192), b""):
来源：http://ykg.nwbrower.top

[U24] Py：路径操作
来源：http://hsr.birdmap.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://bns.yuanzhike.top

[U25] Py：CSV 按字典读
来源：http://pnv.ywan-chungtsiang.top

csv.DictReader(f)
来源：http://mnn.zhaomingkeji.xyz

[U26] Py：并发下载
来源：http://lsa.jinyuanbaomall.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://grf.yangfankeji.com

[U27] Py：异步 HTTP
来源：http://dzi.cucudq.cn

aiohttp.ClientSession() 配合 async with
来源：http://hvy.52xcode.cn

[U28] Py：类型别名
来源：http://xna.hfpthk.cn

UserId = int
来源：http://iwk.pycfn.com

[U29] Py：属性校验
来源：http://wfb.hesvh.cn

@property 与 @x.setter 配合
来源：http://gwo.cheryme.top

[U30] Py：数据类
来源：http://ydx.yj202588.top

@dataclass(slots=True)
来源：http://voz.zdbjq.cn

[U31] Py：单测
来源：http://amn.hcnkem.com

python -m pytest -q
来源：http://fhy.iojbl.cn

[U32] Py：代码格式化
来源：http://wnr.hammf.cn

ruff format . && ruff check --fix .
来源：http://laj.yvedp.cn

[U33] Py：打包发布
来源：http://jva.cucudq.cn

python -m build  （依赖 pyproject.toml）
来源：http://qck.nanxuanxn.top

[U34] Py：判断编码
来源：http://uxk.wangshuangyany.cn

chardet.detect(raw)
来源：http://aaa.yj202588.top

[U35] Py：发送邮件
来源：http://lti.9152youxi.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://qou.pycfn.com

[U36] Py：定时任务
来源：http://kqg.316326.xyz

schedule.every(10).minutes.do(job)
来源：http://asb.sxryk.cn

[U37] Py：读写 Excel
来源：http://gdp.hywenlv.cn

pandas.read_excel / DataFrame.to_excel
来源：http://wgf.guannengcc.top

[U38] Py：获取脚本所在目录
来源：http://gkf.zhoulong.xyz

Path(__file__).resolve().parent
来源：http://fui.vqdsnc.cn

[U39] Py：判断是否在交互环境
来源：http://xsw.zdqjudy.top

sys.stdout.isatty()
来源：http://tpe.daria6918.cn

[U40] Py：打印到标准错误
来源：http://gep.zhengqikj.top

print("err", file=sys.stderr)
来源：http://yuc.haohaochexian.top

[U41] PHP：初始化 Composer 项目
来源：http://wee.yuanzhike.top

composer init;  composer require guzzlehttp/guzzle
来源：http://bqa.yanxiufei.cn

[U42] PHP：PSR-4 自动加载
来源：http://sli.ehwqpu.com

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://gry.yonumen.top

[U43] PHP：声明命名空间
来源：http://lyu.hcnkem.com

namespace App\Http;
来源：http://znz.xuanzx.com

[U44] PHP：开启严格类型
来源：http://cbn.yanxiufei.cn

declare(strict_types=1);
来源：http://yjk.dashuyun.cn

[U45] PHP：类型声明与返回类型
来源：http://txw.yj20258888.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://qbq.ppjwa.cn

[U46] PHP：可空类型
来源：http://frq.52xcode.cn

?string $name = null
来源：http://bel.cdnleiting.top

[U47] PHP：联合类型
来源：http://avq.hcnkem.com

int|string $id
来源：http://cyo.dianchejie.cn

[U48] PHP：纯枚举
来源：http://pwk.epnwcf.com

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://zug.xingfuxueyuan.xyz

[U49] PHP：只读属性
来源：http://kpb.hesvh.cn

public readonly string $name
来源：http://vpa.quarkkingdee.top

[U50] PHP：构造器属性提升
来源：http://znf.fzhhl.top

public function __construct(private int $id) {}
来源：http://kzc.wangdashe.top

[U51] PHP：数组解构
来源：http://lko.yvedp.cn

[$a, $b] = $arr;
来源：http://mea.hywenlv.cn

[U52] PHP：箭头函数
来源：http://jei.hfpthk.cn

$double = fn($x) => $x * 2;
来源：http://jjr.sjlbkw.cn

[U53] PHP：空合并运算符
来源：http://dky.aibaodan.cn

$v = $a ?? $b ?? "default";
来源：http://rnw.tanke756.top

[U54] PHP：空安全调用
来源：http://ccu.aibaodan.cn

$obj?->method()
来源：http://vhd.ydzc1.top

[U55] PHP：match 表达式
来源：http://oyp.chenjidiqi.icu

$s = match($x) { 1 => "一", default => "其他" };
来源：http://ger.zhaomingkeji.xyz

[U56] PHP：命名参数
来源：http://nkk.haohaochexian.top

f(a: 1, b: 2)
来源：http://kbd.aizwys.cn

[U57] PHP：字符串插值
来源：http://xyg.jiagoushi.top

"值: {$a}"
来源：http://arh.snrcjt.cn

[U58] PHP：数组三件套
来源：http://bhg.yj20258888.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://dmi.pycfn.com

[U59] PHP：自定义排序
来源：http://gqp.xingfuxueyuan.xyz

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://vli.xziqi.cn

[U60] PHP：JSON 编解码
来源：http://pdq.cheryme.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://ywr.jinyuanbaomall.cn

[U61] PHP：正则
来源：http://qsx.fktsv.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://kfx.jinyuanbaomall.cn

[U62] PHP：日期对象
来源：http://pmy.mhx1999.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://ntj.tian-w.cn

[U63] PHP：文件读写
来源：http://mxl.smart0.xyz

file_get_contents($f);  file_put_contents($f, $data);
来源：http://ojo.havefunace.top

[U64] PHP：目录遍历
来源：http://dmp.shanyushiyangkeji.top

glob("dir/*.php");  scandir("dir");
来源：http://uxj.cdnleiting.top

[U65] PHP：会话
来源：http://iba.pengpengdd.cyou

session_start();  $_SESSION["uid"] = 1;
来源：http://jvj.xylfe.cn

[U66] PHP：设置 Cookie
来源：http://eok.guowangkeji.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://uol.ppjwa.cn

[U67] PHP：处理文件上传
来源：http://xdz.jinqigufen.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://guw.meibo888.top

[U68] PHP：PDO 连接
来源：http://kjv.meibo888.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://tfe.nanxuanxn.top

[U69] PHP：PDO 预处理
来源：http://ele.ctjpmb.com

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://qtw.ctjpmb.com

[U70] PHP：PDO 事务
来源：http://nsu.havefunace.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://cpu.jinqigfzy.top

[U71] PHP：抛出异常
来源：http://cim.aizwys.cn

throw new RuntimeException("失败", 500);
来源：http://hhh.xuanzx.com

[U72] PHP：写错误日志
来源：http://zfm.chenlongwang.top

error_log("失败: " . $e->getMessage());
来源：http://epy.shuidangran.top

[U73] PHP：读取 ini 配置
来源：http://inv.wangdashe.top

parse_ini_file("config.ini", true)
来源：http://iyc.jianghu66.top

[U74] PHP：读取环境变量
来源：http://yfm.ydzc1.top

getenv("APP_ENV") ?: "production"
来源：http://kzk.hnqzz.top

[U75] PHP：依赖注入
来源：http://zhv.zhoulong.xyz

composer require psr/container
来源：http://oih.chenzaomai.com

[U76] PHP：简单路由
来源：http://gul.guannengcc.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://mmv.smart0.xyz

[U77] PHP：模板渲染
来源：http://qvd.fanxiaobao.xyz

composer require twig/twig
来源：http://aqr.yuanzhike.top

[U78] PHP：单元测试
来源：http://oxu.svipenyu.cn

composer require --dev phpunit/phpunit
来源：http://roy.ywan-chungtsiang.top

[U79] PHP：静态分析
来源：http://dbq.sjlbkw.cn

composer require --dev phpstan/phpstan
来源：http://abt.daxiang520.top

[U80] PHP：代码规范修复
来源：http://avt.cucudq.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://ycu.yuanzhike.top

[U81] JS：初始化项目
来源：http://mmz.jqgfzy.top

npm init -y;  npm i express
来源：http://gmv.vqdsnc.cn

[U82] JS：package.json 脚本
来源：http://mlk.dianchejie.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://tkh.feifeiyinyue.top

[U83] JS：ES Module 导入导出
来源：http://bjs.yonumen.top

export const a = 1;  import { a } from "./m.js";
来源：http://axq.sysykeji.top

[U84] JS：CommonJS 写法
来源：http://lqs.aibaodan.cn

module.exports = { a };  const { a } = require("./m");
来源：http://kbd.yongpay.top

[U85] JS：可选链
来源：http://ggb.zhengqikj.top

a?.b?.c
来源：http://tvu.52xcode.cn

[U86] JS：空值合并
来源：http://lsz.sysykeji.top

a ?? b
来源：http://zfn.meibo888.top

[U87] JS：解构默认值
来源：http://uvu.sysykeji.top

const { a = 1, b = 2 } = obj;
来源：http://cqz.jqgfzy.top

[U88] JS：对象展开合并
来源：http://cuv.ehwqpu.com

{ ...a, ...b }
来源：http://ceo.epnwcf.com

[U89] JS：数组去重
来源：http://pct.tian-w.cn

[...new Set(arr)]
来源：http://qsy.yuxming.cn

[U90] JS：数字数组排序
来源：http://gzc.jianghu66.top

[...arr].sort((a, b) => a - b)
来源：http://eek.daxiang520.top

[U91] JS：对象键值遍历
来源：http://afz.yj20258.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://aot.zhaomingkeji.xyz

[U92] JS：深拷贝
来源：http://rqy.vehdjk.com

structuredClone(obj)
来源：http://mij.svipenyu.cn

[U93] JS：模板字符串
来源：http://taq.wangdashe.top

`共 ${n} 条`
来源：http://acb.dianchejie.cn

[U94] JS：箭头函数
来源：http://spf.jianghu66.top

const double = x => x * 2;
来源：http://iru.ywan-chungtsiang.top

[U95] JS：Promise 包装
来源：http://enr.chenlongwang.top

new Promise((resolve, reject) => {})
来源：http://cey.sjlbkw.cn

[U96] JS：async/await 与异常
来源：http://kpa.xinyue.icu

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://bvo.chenjidiqi.icu

[U97] JS：并发请求
来源：http://cfe.cashguo.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://cfs.jinghuilouyu.cn

[U98] JS：fetch 带 JSON
来源：http://rbo.ehwqpu.com

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://cru.ivvv.top

[U99] JS：事件监听
来源：http://omf.jinyuanbaomall.cn

el.addEventListener("click", e => {})
来源：http://ioj.xziqi.cn

[U100] JS：DOM 查询
来源：http://cvi.daria6918.cn

document.querySelector(".item")
来源：http://ers.zhiwuduotai.top

[U101] JS：classList 操作
来源：http://pkh.jqgfzy.top

el.classList.toggle("active")
来源：http://lbg.aibaodan.cn

[U102] JS：本地存储
来源：http://yip.chenjidiqi.icu

localStorage.setItem("k", JSON.stringify(v))
来源：http://fln.snrcjt.cn

[U103] JS：定时器
来源：http://xyu.zhijiandao.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://tmb.tian-w.cn

[U104] JS：防抖
来源：http://sfy.cheryme.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ivx.jianghu66.top

[U105] JS：节流
来源：http://kqq.gaohongyu789.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://fcb.mhx1999.top

[U106] JS：日期格式化
来源：http://jph.zhijiandao.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://rwt.kuanghao11.cn

[U107] JS：数字千分位
来源：http://kdu.tanke756.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://xaw.jqgfzy.top

[U108] JS：随机整数
来源：http://ivl.zhaomingkeji.xyz

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://nmm.yangfankeji.com

[U109] JS：数组分组
来源：http://khw.fanxiaobao.xyz

Object.groupBy(arr, x => x.type)
来源：http://anz.zhoulong.xyz

[U110] JS：数组分块
来源：http://mlt.havefunace.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://usu.aizwys.cn

[U111] JS：对象转 Map
来源：http://nys.daxiang520.top

new Map(Object.entries(obj))
来源：http://sqq.ivvv.top

[U112] JS：字符串补位
来源：http://bdn.cqqwz.cn

"7".padStart(3, "0")
来源：http://vrf.aizwys.cn

[U113] JS：正则替换全部
来源：http://ahn.shanyushiyangtech.top

s.replaceAll("a", "b")
来源：http://ycx.jyoumei.cn

[U114] JS：JSON 深比较
来源：http://sea.ydzc1.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://fxm.zycfv.cn

[U115] JS：生成 UUID
来源：http://rwv.sjlbkw.cn

crypto.randomUUID()
来源：http://kcb.zhongyouzk.top

[U116] JS：类型检查（JSDoc）
来源：http://ezn.yueranfly.top

/** @param {string} name */ function f(name) {}
来源：http://xdm.chenlongwang.top

[U117] JS：单元测试
来源：http://sro.ydjk.org.cn

npm i -D vitest;  npx vitest
来源：http://wzm.jinqigfzy.top

[U118] JS：开发服务器
来源：http://pne.svipenyu.cn

npm i -D vite;  npx vite
来源：http://dav.yj20258888.top

[U119] JS：生产构建
来源：http://cnz.shanyushiyangtech.top

npx vite build
来源：http://obi.wangshuangyany.cn

[U120] JS：读取环境变量（Vite）
来源：http://vlg.fehbvm.com

import.meta.env.VITE_API_URL
来源：http://rfz.fanxiaobao.xyz

================================================================================
来源：http://rrs.cqqwz.cn

统计汇总
来源：http://gpy.shuidangran.top

================================================================================
来源：http://ork.yanxiufei.cn

按语言统计（条）：
来源：http://rze.fzhhl.top

Python ......... 252
来源：http://fjj.ppjwa.cn

PHP ............ 252
来源：http://zwy.yueranfly.top

JavaScript ..... 252
来源：http://mwt.havefunace.top

TypeScript ..... 212
来源：http://gtu.haohaochexian.top


<!-- 参考信息 -->