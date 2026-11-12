代发 wailian999

[T39] Lua：模式匹配
来源：http://egb.xylfe.cn

string.find(s, "%d+")
来源：http://dab.nanxuanxn.top

[T40] Lua：元表
来源：http://oad.zhaomingkeji.xyz

setmetatable({}, { __index = base })
来源：http://grz.ybcxt.top

[T41] Perl：Hello World
来源：http://tns.yangfankeji.com

print "Hello\n";
来源：http://upp.yuxming.cn

[T42] Perl：变量类型
来源：http://wyr.guannengcc.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://qnb.xinyue.icu

[T43] Perl：字符串插值
来源：http://yaf.gogol.net.cn

"值: $a"
来源：http://sus.xziqi.cn

[T44] Perl：条件
来源：http://iqs.shanyushiyangkeji.top

if ($a > 0) { print "正"; }
来源：http://pwt.yvedp.cn

[T45] Perl：数组遍历
来源：http://hmt.zhengqikj.top

for my $x (@arr) { print $x; }
来源：http://jlu.jqgufenzy.top

[T46] Perl：哈希操作
来源：http://gnl.gotoacloud.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://nja.shzxlz.cn

[T47] Perl：正则捕获
来源：http://eoo.nanxinkj.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://lui.hnxiangtu.top

[T48] Perl：正则替换
来源：http://rzn.sxryk.cn

$s =~ s/old/new/g;
来源：http://wll.yj20258888.top

[T49] Perl：函数
来源：http://okm.yanxiufei.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://gya.cashguo.top

[T50] Perl：逐行读文件
来源：http://swp.redwolf501.top

open my $fh, "<", "a.txt" or die $!;
来源：http://tsz.ivvv.top

while (my $line = <$fh>) { print $line; }
来源：http://pam.yangfankeji.com

[T51] Scala：Hello World
来源：http://hmh.ehwqpu.com

println("Hello")
来源：http://wsj.hammf.cn

[T52] Scala：变量
来源：http://pne.meibo888.top

val a = 1;  var b = 2
来源：http://crl.jinqigfzy.top

[T53] Scala：字符串插值
来源：http://xmh.ctjpmb.com

s"值: $b"
来源：http://nhd.jinqigufen.top

[T54] Scala：集合映射
来源：http://mcr.ivvv.top

List(1, 2, 3).map(_ * 2)
来源：http://aiq.jinqigfzy.top

[T55] Scala：集合过滤
来源：http://fzu.jqgfzy.top

List(1, 2, 3).filter(_ > 1)
来源：http://kxs.smart0.xyz

[T56] Scala：样例类
来源：http://zsp.kuanghao11.cn

case class User(name: String, age: Int)
来源：http://qzh.chenlongwang.top

[T57] Scala：模式匹配
来源：http://hkv.svipenyu.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://pno.52xcode.cn

[T58] Scala：函数定义
来源：http://adu.chenjidiqi.icu

def add(a: Int, b: Int): Int = a + b
来源：http://lwm.guowangkeji.top

[T59] Scala：循环
来源：http://exv.dashuyun.cn

for (i <- 1 to 10) println(i)
来源：http://fkv.xinyue.icu

[T60] Scala：折叠
来源：http://nss.ybcxt.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://wan.guowangkeji.top

================================================================================
来源：http://ayi.hcnkem.com

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://oeg.zhoulong.xyz

================================================================================
来源：http://wdh.yueranfly.top

[U01] Py：创建虚拟环境
来源：http://jmx.aibaodan.cn

python -m venv .venv && source .venv/bin/activate
来源：http://rpt.yj202588.top

[U02] Py：导出 / 安装依赖
来源：http://tmx.shanyushiyangtech.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://fvv.gaohongyu789.top

[U03] Py：加载 .env 配置
来源：http://ikf.iojbl.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://xle.ywan-chungtsiang.top

[U04] Py：变量调试打印
来源：http://kru.uphjek.com

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://jpx.feifeiyinyue.top

[U05] Py：列表去重且保序
来源：http://gkk.0kj1m.cn

list(dict.fromkeys(arr))
来源：http://scm.sweek.top

[U06] Py：合并两个字典
来源：http://rqx.yfazqb.com

{**a, **b}
来源：http://zbj.fehbvm.com

[U07] Py：反转字典键值
来源：http://qgo.guannengcc.top

{v: k for k, v in d.items()}
来源：http://iur.shuidangran.top

[U08] Py：展平二维列表
来源：http://bnu.ctjpmb.com

[y for x in nested for y in x]
来源：http://peq.guowangkeji.top

[U09] Py：字典取最大值的键
来源：http://mjt.hysaishi.cn

max(d, key=d.get)
来源：http://xxu.ehwqpu.com

[U10] Py：按值排序字典
来源：http://uia.zdqjudy.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://xty.sufxvd.cn

[U11] Py：生成器表达式
来源：http://jah.jinghuilouyu.cn

(x * 2 for x in arr)
来源：http://nik.hfpthk.cn

[U12] Py：取出现最多的 3 个元素
来源：http://thm.hysaishi.cn

Counter(arr).most_common(3)
来源：http://two.iojbl.cn

[U13] Py：固定长度队列
来源：http://yic.shanyushiyangkeji.top

deque(maxlen=10)
来源：http://drj.shanyushiyangtech.top

[U14] Py：分组收集到列表
来源：http://npw.cashguo.top

defaultdict(list)
来源：http://man.yj20258888.top

[U15] Py：高精度计时
来源：http://jlc.dianchejie.cn

t = time.perf_counter()
来源：http://eeb.zycfv.cn

[U16] Py：命令行参数解析
来源：http://pyr.yj202588.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://yvs.shzxlz.cn

[U17] Py：初始化日志
来源：http://dzu.quarkkingdee.top

logging.basicConfig(level=logging.INFO)
来源：http://weh.ehwqpu.com

[U18] Py：预编译正则
来源：http://hwx.xylfe.cn

pat = re.compile(r"\d+")
来源：http://kjh.shangyingyoupin.top

[U19] Py：正则替换带回调
来源：http://sos.yonumen.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://jhu.wangdashe.top

[U20] Py：缓存函数结果
来源：http://wsb.yangfankeji.com

@functools.lru_cache(maxsize=None)
来源：http://uea.iojbl.cn

[U21] Py：自定义上下文管理器
来源：http://gbn.bbcook.cn

@contextlib.contextmanager
来源：http://rqu.yvedp.cn

[U22] Py：矩阵转置
来源：http://mdx.yangfankeji.com

list(zip(*m))
来源：http://goz.yanxiufei.cn

[U23] Py：分块读取大文件
来源：http://kke.cheryme.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://rzm.zhoulong.xyz

[U24] Py：路径操作
来源：http://euv.chenjidiqi.icu

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://sct.fehbvm.com

[U25] Py：CSV 按字典读
来源：http://ibp.andypj.xyz

csv.DictReader(f)
来源：http://acp.nwbrower.top

[U26] Py：并发下载
来源：http://uqp.nwbrower.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://etx.fzhhl.top

[U27] Py：异步 HTTP
来源：http://wkk.yj20258.top

aiohttp.ClientSession() 配合 async with
来源：http://iaz.xylfe.cn

[U28] Py：类型别名
来源：http://cjx.c1oappe.top

UserId = int
来源：http://ugp.jinqigfzy.top

[U29] Py：属性校验
来源：http://nar.hongshengwenyu.top

@property 与 @x.setter 配合
来源：http://wih.aizwys.cn

[U30] Py：数据类
来源：http://lxe.pycfn.com

@dataclass(slots=True)
来源：http://nad.bjfxy.top

[U31] Py：单测
来源：http://hbz.fktsv.cn

python -m pytest -q
来源：http://aqz.fktsv.cn

[U32] Py：代码格式化
来源：http://fqq.epnwcf.com

ruff format . && ruff check --fix .
来源：http://nqw.sxryk.cn

[U33] Py：打包发布
来源：http://zvy.jqgfzy.top

python -m build  （依赖 pyproject.toml）
来源：http://rpx.aibaodan.cn

[U34] Py：判断编码
来源：http://fjo.jlsjyb.cn

chardet.detect(raw)
来源：http://koi.ctjpmb.com

[U35] Py：发送邮件
来源：http://dap.jinqigfzy.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://eow.guannengcc.top

[U36] Py：定时任务
来源：http://frg.sjlbkw.cn

schedule.every(10).minutes.do(job)
来源：http://eir.guannengcc.top

[U37] Py：读写 Excel
来源：http://nxl.fehbvm.com

pandas.read_excel / DataFrame.to_excel
来源：http://lha.shangyingyoupin.top

[U38] Py：获取脚本所在目录
来源：http://mzi.bjfxy.top

Path(__file__).resolve().parent
来源：http://yla.haohaochexian.top

[U39] Py：判断是否在交互环境
来源：http://pzm.meibo888.top

sys.stdout.isatty()
来源：http://onh.daria6918.cn

[U40] Py：打印到标准错误
来源：http://fyc.52xcode.cn

print("err", file=sys.stderr)
来源：http://svt.zdbjq.cn

[U41] PHP：初始化 Composer 项目
来源：http://zuh.vehdjk.com

composer init;  composer require guzzlehttp/guzzle
来源：http://hsv.guannengcc.top

[U42] PHP：PSR-4 自动加载
来源：http://iuq.shanyushiyangkeji.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hag.tian-w.cn

[U43] PHP：声明命名空间
来源：http://wos.jinghuilouyu.cn

namespace App\Http;
来源：http://wnc.pengpengdd.cyou

[U44] PHP：开启严格类型
来源：http://lut.yonumen.top

declare(strict_types=1);
来源：http://agq.zhaomingkeji.xyz

[U45] PHP：类型声明与返回类型
来源：http://vmr.gaohongyu789.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://wud.ydjk.org.cn

[U46] PHP：可空类型
来源：http://wsa.chenjidiqi.icu

?string $name = null
来源：http://gqi.meibo888.top

[U47] PHP：联合类型
来源：http://btu.tian-w.cn

int|string $id
来源：http://rof.guowangkeji.top

[U48] PHP：纯枚举
来源：http://fby.yvedp.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://dvf.fzhhl.top

[U49] PHP：只读属性
来源：http://rvg.ywan-chungtsiang.top

public readonly string $name
来源：http://ebd.feifeiyinyue.top

[U50] PHP：构造器属性提升
来源：http://qei.havefunace.top

public function __construct(private int $id) {}
来源：http://ndn.vqdsnc.cn

[U51] PHP：数组解构
来源：http://uzs.ivvv.top

[$a, $b] = $arr;
来源：http://wss.sufxvd.cn

[U52] PHP：箭头函数
来源：http://apm.gaohongyu789.top

$double = fn($x) => $x * 2;
来源：http://lbx.yanxiufei.cn

[U53] PHP：空合并运算符
来源：http://pbp.daxiang520.top

$v = $a ?? $b ?? "default";
来源：http://ksl.kuanghao11.cn

[U54] PHP：空安全调用
来源：http://wqn.smart0.xyz

$obj?->method()
来源：http://thv.zdbjq.cn

[U55] PHP：match 表达式
来源：http://ofh.ivvv.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://cml.ywan-chungtsiang.top

[U56] PHP：命名参数
来源：http://xhm.daxiang520.top

f(a: 1, b: 2)
来源：http://zsh.meibo888.top

[U57] PHP：字符串插值
来源：http://ywz.fengsongda.top

"值: {$a}"
来源：http://cge.shangyingyoupin.top

[U58] PHP：数组三件套
来源：http://nzx.epnwcf.com

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://eob.cashguo.top

[U59] PHP：自定义排序
来源：http://zuk.52xcode.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mao.snrcjt.cn

[U60] PHP：JSON 编解码
来源：http://fzs.cashguo.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://cgw.iojbl.cn

[U61] PHP：正则
来源：http://inr.cdnleiting.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://xfw.nwbrower.top

[U62] PHP：日期对象
来源：http://dwp.chenzaomai.com

(new DateTimeImmutable())->format("Y-m-d");
来源：http://mzb.ydzc1.top

[U63] PHP：文件读写
来源：http://sql.fehbvm.com

file_get_contents($f);  file_put_contents($f, $data);
来源：http://atl.0kj1m.cn

[U64] PHP：目录遍历
来源：http://jfo.yj202588.top

glob("dir/*.php");  scandir("dir");
来源：http://afh.jyoumei.cn

[U65] PHP：会话
来源：http://ezo.jiagoushi.top

session_start();  $_SESSION["uid"] = 1;
来源：http://tda.jqgufenzy.top

[U66] PHP：设置 Cookie
来源：http://gbm.mhx1999.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://eia.ywan-chungtsiang.top

[U67] PHP：处理文件上传
来源：http://bcb.nanxinkj.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://gyo.jinyuanbaomall.cn

[U68] PHP：PDO 连接
来源：http://jgw.redwolf501.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://mhp.gzhubu.top

[U69] PHP：PDO 预处理
来源：http://xbl.mhx1999.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://kby.gaohongyu789.top

[U70] PHP：PDO 事务
来源：http://roi.yueranfly.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://ttd.meibo888.top

[U71] PHP：抛出异常
来源：http://jqq.haohaochexian.top

throw new RuntimeException("失败", 500);
来源：http://upj.zhixingplan.top

[U72] PHP：写错误日志
来源：http://iwd.yj202588.top

error_log("失败: " . $e->getMessage());
来源：http://mmw.xingfuxueyuan.xyz

[U73] PHP：读取 ini 配置
来源：http://neg.zhiwuduotai.top

parse_ini_file("config.ini", true)
来源：http://irg.shanyushiyangtech.top

[U74] PHP：读取环境变量
来源：http://dtk.hysaishi.cn

getenv("APP_ENV") ?: "production"
来源：http://bbx.gaohongyu789.top

[U75] PHP：依赖注入
来源：http://xid.smart0.xyz

composer require psr/container
来源：http://zko.zycfv.cn

[U76] PHP：简单路由
来源：http://wcr.shuidangran.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://nrz.jinyuanbaomall.cn

[U77] PHP：模板渲染
来源：http://gyl.shangyingyoupin.top

composer require twig/twig
来源：http://kph.vqdsnc.cn

[U78] PHP：单元测试
来源：http://mwz.yueranfly.top

composer require --dev phpunit/phpunit
来源：http://vmt.zhengqikj.top

[U79] PHP：静态分析
来源：http://fyl.jinqigfzy.top

composer require --dev phpstan/phpstan
来源：http://lwy.zhengqikj.top

[U80] PHP：代码规范修复
来源：http://gcv.yuxming.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://ddb.xuanzx.com

[U81] JS：初始化项目
来源：http://xvv.xuanzx.com

npm init -y;  npm i express
来源：http://qse.zhengqikj.top

[U82] JS：package.json 脚本
来源：http://fnz.zdqjudy.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://ugr.xingfuxueyuan.xyz

[U83] JS：ES Module 导入导出
来源：http://vgt.jinqigufen.top

export const a = 1;  import { a } from "./m.js";
来源：http://rlh.nanxuanxn.top

[U84] JS：CommonJS 写法
来源：http://cty.yonumen.top

module.exports = { a };  const { a } = require("./m");
来源：http://ymy.hysaishi.cn

[U85] JS：可选链
来源：http://pmq.gaohongyu789.top

a?.b?.c
来源：http://cal.cashguo.top

[U86] JS：空值合并
来源：http://vjd.vehdjk.com

a ?? b
来源：http://zfs.ywan-chungtsiang.top

[U87] JS：解构默认值
来源：http://feq.jyoumei.cn

const { a = 1, b = 2 } = obj;
来源：http://yoh.vehdjk.com

[U88] JS：对象展开合并
来源：http://xko.hongshengwenyu.top

{ ...a, ...b }
来源：http://bll.yueranfly.top

[U89] JS：数组去重
来源：http://jcb.meibo888.top

[...new Set(arr)]
来源：http://vtl.yfazqb.com

[U90] JS：数字数组排序
来源：http://xie.sjlbkw.cn

[...arr].sort((a, b) => a - b)
来源：http://sai.uphjek.com

[U91] JS：对象键值遍历
来源：http://ewq.hesvh.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://yyt.fanxiaobao.xyz

[U92] JS：深拷贝
来源：http://xjl.guannengcc.top

structuredClone(obj)
来源：http://oep.nanxuanxn.top

[U93] JS：模板字符串
来源：http://lcg.cdnleiting.top

`共 ${n} 条`
来源：http://eea.xinyue.icu

[U94] JS：箭头函数
来源：http://byp.aibaodan.cn

const double = x => x * 2;
来源：http://fkt.yvedp.cn

[U95] JS：Promise 包装
来源：http://siq.shuidangran.top

new Promise((resolve, reject) => {})
来源：http://rcq.jinqigufen.top

[U96] JS：async/await 与异常
来源：http://cny.ppjwa.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://wpa.sysykeji.top

[U97] JS：并发请求
来源：http://kzw.zdqjudy.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://lcw.ctjpmb.com

[U98] JS：fetch 带 JSON
来源：http://mcf.yuanzhike.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://cyn.yfazqb.com

[U99] JS：事件监听
来源：http://bdi.haohaochexian.top

el.addEventListener("click", e => {})
来源：http://kde.chenzaomai.com

[U100] JS：DOM 查询
来源：http://cxv.mhx1999.top

document.querySelector(".item")
来源：http://eoe.fengsongda.top

[U101] JS：classList 操作
来源：http://voh.9152youxi.cn

el.classList.toggle("active")
来源：http://tvt.daria6918.cn

[U102] JS：本地存储
来源：http://rhj.bbcook.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://cgk.cashguo.top

[U103] JS：定时器
来源：http://cdj.havefunace.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://zlr.jlsjyb.cn

[U104] JS：防抖
来源：http://myb.havefunace.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ntq.bbcook.cn

[U105] JS：节流
来源：http://fgk.epnwcf.com

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://uhr.bjfxy.top

[U106] JS：日期格式化
来源：http://glh.cdnleiting.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://xga.yj202588.top

[U107] JS：数字千分位
来源：http://opi.zycfv.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://ckl.jianghu66.top

[U108] JS：随机整数
来源：http://heg.shanyushiyangtech.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://vhc.redwolf501.top

[U109] JS：数组分组
来源：http://vwu.zhengqikj.top

Object.groupBy(arr, x => x.type)
来源：http://vrh.c1oappe.top

[U110] JS：数组分块
来源：http://cnr.chenjidiqi.icu

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://brk.epnwcf.com

[U111] JS：对象转 Map
来源：http://foa.ydzc1.top

new Map(Object.entries(obj))
来源：http://tsq.jqgfzy.top

[U112] JS：字符串补位
来源：http://lfr.yonumen.top

"7".padStart(3, "0")
来源：http://fyx.yonumen.top

[U113] JS：正则替换全部
来源：http://skk.chenjidiqi.icu

s.replaceAll("a", "b")
来源：http://iby.jqgfzy.top

[U114] JS：JSON 深比较
来源：http://mei.shuidangran.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://ejq.shuidangran.top

[U115] JS：生成 UUID
来源：http://ixe.xylfe.cn

crypto.randomUUID()
来源：http://mmd.shuidangran.top

[U116] JS：类型检查（JSDoc）
来源：http://aps.zdbjq.cn

/** @param {string} name */ function f(name) {}
来源：http://kir.mhx1999.top

[U117] JS：单元测试
来源：http://dmz.sweek.top

npm i -D vitest;  npx vitest
来源：http://xdj.kuanghao11.cn

[U118] JS：开发服务器
来源：http://tsw.xuetiantiany.cn

npm i -D vite;  npx vite
来源：http://aga.hammf.cn

[U119] JS：生产构建
来源：http://qop.0kj1m.cn

npx vite build
来源：http://kkr.shanyushiyangtech.top

[U120] JS：读取环境变量（Vite）
来源：http://kcx.fzhhl.top

import.meta.env.VITE_API_URL
来源：http://pjm.bjfxy.top

================================================================================
来源：http://cfa.aizwys.cn

统计汇总
来源：http://ujn.redwolf501.top

================================================================================
来源：http://fmq.mhx1999.top

按语言统计（条）：
来源：http://nif.wangdashe.top

Python ......... 252
来源：http://ejw.sufxvd.cn

PHP ............ 252
来源：http://doo.zhongyouzk.top

JavaScript ..... 252
来源：http://bco.yj20258.top

TypeScript ..... 212
来源：http://oho.hongshengwenyu.top

Java ........... 212
来源：http://tpe.zhixingplan.top

Go ............. 212
来源：http://qny.xinyue.icu

Ruby ........... 212
来源：http://idm.fzhhl.top

C# ............. 212
来源：http://cvq.jlsjyb.cn


<!-- 参考信息 -->