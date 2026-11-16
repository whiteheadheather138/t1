代发 wailian999

[T33] Lua：表（数组）
来源：http://tcz.yuanzhike.top

local t = {1, 2, 3};  t[4] = 4
来源：http://luy.wangshuangyany.cn

[T34] Lua：遍历表
来源：http://wru.fengsongda.top

for i, v in ipairs(t) do print(i, v) end
来源：http://ieg.yvedp.cn

[T35] Lua：字典表
来源：http://som.wangshuangyany.cn

local d = { a = 1 };  d.b = 2
来源：http://awt.epnwcf.com

[T36] Lua：函数
来源：http://oiq.jianghu66.top

function add(a, b) return a + b end
来源：http://kws.ydzc1.top

[T37] Lua：字符串拼接
来源：http://wqv.zdqjudy.top

"a" .. "b"
来源：http://bql.hfpthk.cn

[T38] Lua：条件
来源：http://quv.52xcode.cn

if x > 0 then print("正") end
来源：http://yaw.cashguo.top

[T39] Lua：模式匹配
来源：http://fqt.shzxlz.cn

string.find(s, "%d+")
来源：http://muh.ppjwa.cn

[T40] Lua：元表
来源：http://uew.daria6918.cn

setmetatable({}, { __index = base })
来源：http://kvp.sweek.top

[T41] Perl：Hello World
来源：http://izf.zhengqikj.top

print "Hello\n";
来源：http://bbb.jyoumei.cn

[T42] Perl：变量类型
来源：http://hnu.cheryme.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://gog.hywenlv.cn

[T43] Perl：字符串插值
来源：http://mrn.svipenyu.cn

"值: $a"
来源：http://adj.sweek.top

[T44] Perl：条件
来源：http://ksa.hcnkem.com

if ($a > 0) { print "正"; }
来源：http://gdu.hysaishi.cn

[T45] Perl：数组遍历
来源：http://mzx.daxiang520.top

for my $x (@arr) { print $x; }
来源：http://ien.hfpthk.cn

[T46] Perl：哈希操作
来源：http://eqi.gaohongyu789.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://pjm.zhaomingkeji.xyz

[T47] Perl：正则捕获
来源：http://skx.c1oappe.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://ule.shzxlz.cn

[T48] Perl：正则替换
来源：http://vxw.shzxlz.cn

$s =~ s/old/new/g;
来源：http://xkj.fktsv.cn

[T49] Perl：函数
来源：http://fbs.haohaochexian.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://ref.shanyushiyangtech.top

[T50] Perl：逐行读文件
来源：http://kju.ydzc1.top

open my $fh, "<", "a.txt" or die $!;
来源：http://jrd.ydzc1.top

while (my $line = <$fh>) { print $line; }
来源：http://zhr.9152youxi.cn

[T51] Scala：Hello World
来源：http://bxb.hcnkem.com

println("Hello")
来源：http://szr.jqgufenzy.top

[T52] Scala：变量
来源：http://etq.mhx1999.top

val a = 1;  var b = 2
来源：http://nhs.xinyue.icu

[T53] Scala：字符串插值
来源：http://lmy.aibaodan.cn

s"值: $b"
来源：http://vln.cheryme.top

[T54] Scala：集合映射
来源：http://bdt.pycfn.com

List(1, 2, 3).map(_ * 2)
来源：http://lyw.yj20258888.top

[T55] Scala：集合过滤
来源：http://dwv.gotoacloud.top

List(1, 2, 3).filter(_ > 1)
来源：http://kkg.snrcjt.cn

[T56] Scala：样例类
来源：http://ket.uphjek.com

case class User(name: String, age: Int)
来源：http://zco.dashuyun.cn

[T57] Scala：模式匹配
来源：http://ilu.jqgfzy.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://pzb.tanke756.top

[T58] Scala：函数定义
来源：http://scu.jyoumei.cn

def add(a: Int, b: Int): Int = a + b
来源：http://cgt.zdbjq.cn

[T59] Scala：循环
来源：http://qxt.c1oappe.top

for (i <- 1 to 10) println(i)
来源：http://jtr.cqqwz.cn

[T60] Scala：折叠
来源：http://ezw.cqqwz.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://anw.yj20258.top

================================================================================
来源：http://duk.hysaishi.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://loa.shanyushiyangtech.top

================================================================================
来源：http://wnu.fehbvm.com

[U01] Py：创建虚拟环境
来源：http://zsp.hammf.cn

python -m venv .venv && source .venv/bin/activate
来源：http://hly.jiagoushi.top

[U02] Py：导出 / 安装依赖
来源：http://txs.haohaochexian.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://qwg.iojbl.cn

[U03] Py：加载 .env 配置
来源：http://ceu.havefunace.top

from dotenv import load_dotenv; load_dotenv()
来源：http://xnz.zhengqikj.top

[U04] Py：变量调试打印
来源：http://zni.hywenlv.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://gey.svipenyu.cn

[U05] Py：列表去重且保序
来源：http://xqq.snrcjt.cn

list(dict.fromkeys(arr))
来源：http://emk.fanxiaobao.xyz

[U06] Py：合并两个字典
来源：http://kvf.yuanzhike.top

{**a, **b}
来源：http://ugx.chenjidiqi.icu

[U07] Py：反转字典键值
来源：http://vid.xuetiantiany.cn

{v: k for k, v in d.items()}
来源：http://mzt.jqgufenzy.top

[U08] Py：展平二维列表
来源：http://cmr.hcnkem.com

[y for x in nested for y in x]
来源：http://zff.jinyuanbaomall.cn

[U09] Py：字典取最大值的键
来源：http://hyq.xuanzx.com

max(d, key=d.get)
来源：http://zey.guowangkeji.top

[U10] Py：按值排序字典
来源：http://niy.tian-w.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://ivw.dashuyun.cn

[U11] Py：生成器表达式
来源：http://vhj.ivvv.top

(x * 2 for x in arr)
来源：http://yjt.cheryme.top

[U12] Py：取出现最多的 3 个元素
来源：http://xzl.yongpay.top

Counter(arr).most_common(3)
来源：http://wvr.shuidangran.top

[U13] Py：固定长度队列
来源：http://vwi.fzhhl.top

deque(maxlen=10)
来源：http://axi.yfazqb.com

[U14] Py：分组收集到列表
来源：http://vkk.bjfxy.top

defaultdict(list)
来源：http://odr.epnwcf.com

[U15] Py：高精度计时
来源：http://syk.c1oappe.top

t = time.perf_counter()
来源：http://eao.c1oappe.top

[U16] Py：命令行参数解析
来源：http://ofe.yueranfly.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://mqw.fktsv.cn

[U17] Py：初始化日志
来源：http://eur.nanxinkj.top

logging.basicConfig(level=logging.INFO)
来源：http://qhw.snrcjt.cn

[U18] Py：预编译正则
来源：http://fkn.zhengqikj.top

pat = re.compile(r"\d+")
来源：http://fig.yongpay.top

[U19] Py：正则替换带回调
来源：http://ejp.nanxinkj.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://ksz.c1oappe.top

[U20] Py：缓存函数结果
来源：http://mkl.tianlin.xyz

@functools.lru_cache(maxsize=None)
来源：http://zpr.zdqjudy.top

[U21] Py：自定义上下文管理器
来源：http://vnp.zycfv.cn

@contextlib.contextmanager
来源：http://ipq.jqgfzy.top

[U22] Py：矩阵转置
来源：http://aaf.aizwys.cn

list(zip(*m))
来源：http://jpd.mhx1999.top

[U23] Py：分块读取大文件
来源：http://jat.jiagoushi.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://dse.fanxiaobao.xyz

[U24] Py：路径操作
来源：http://pvf.xylfe.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://jzp.hysaishi.cn

[U25] Py：CSV 按字典读
来源：http://cof.nanxinkj.top

csv.DictReader(f)
来源：http://npf.yanxiufei.cn

[U26] Py：并发下载
来源：http://vqy.zhaomingkeji.xyz

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hri.shuidangran.top

[U27] Py：异步 HTTP
来源：http://rtp.xinyue.icu

aiohttp.ClientSession() 配合 async with
来源：http://lrf.shuidangran.top

[U28] Py：类型别名
来源：http://qkp.hongshengwenyu.top

UserId = int
来源：http://utt.feifeiyinyue.top

[U29] Py：属性校验
来源：http://rjb.andypj.xyz

@property 与 @x.setter 配合
来源：http://qaw.daxiang520.top

[U30] Py：数据类
来源：http://jks.fzhhl.top

@dataclass(slots=True)
来源：http://hlo.pengpengdd.cyou

[U31] Py：单测
来源：http://eoa.quarkkingdee.top

python -m pytest -q
来源：http://kjf.sysykeji.top

[U32] Py：代码格式化
来源：http://nkq.fktsv.cn

ruff format . && ruff check --fix .
来源：http://zup.jqgfzy.top

[U33] Py：打包发布
来源：http://mkz.yueranfly.top

python -m build  （依赖 pyproject.toml）
来源：http://icl.guannengcc.top

[U34] Py：判断编码
来源：http://auv.hammf.cn

chardet.detect(raw)
来源：http://jop.0kj1m.cn

[U35] Py：发送邮件
来源：http://bac.jinqigfzy.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://zhm.sweek.top

[U36] Py：定时任务
来源：http://qub.yj202588.top

schedule.every(10).minutes.do(job)
来源：http://xji.yueranfly.top

[U37] Py：读写 Excel
来源：http://xvb.yonumen.top

pandas.read_excel / DataFrame.to_excel
来源：http://byv.yj202588.top

[U38] Py：获取脚本所在目录
来源：http://mft.hammf.cn

Path(__file__).resolve().parent
来源：http://opz.jinyuanbaomall.cn

[U39] Py：判断是否在交互环境
来源：http://ofu.jlsjyb.cn

sys.stdout.isatty()
来源：http://hvv.xuetiantiany.cn

[U40] Py：打印到标准错误
来源：http://sll.uphjek.com

print("err", file=sys.stderr)
来源：http://lyo.cucudq.cn

[U41] PHP：初始化 Composer 项目
来源：http://kgu.c1oappe.top

composer init;  composer require guzzlehttp/guzzle
来源：http://dwe.xziqi.cn

[U42] PHP：PSR-4 自动加载
来源：http://ouk.zhiwuduotai.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hpe.jinqigfzy.top

[U43] PHP：声明命名空间
来源：http://znf.cdnleiting.top

namespace App\Http;
来源：http://eky.jinyuanbaomall.cn

[U44] PHP：开启严格类型
来源：http://pfo.xziqi.cn

declare(strict_types=1);
来源：http://pkv.xziqi.cn

[U45] PHP：类型声明与返回类型
来源：http://iiq.havefunace.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://fll.zhixingplan.top

[U46] PHP：可空类型
来源：http://amh.ywan-chungtsiang.top

?string $name = null
来源：http://kpn.ydzc1.top

[U47] PHP：联合类型
来源：http://qqm.hesvh.cn

int|string $id
来源：http://tvc.smart0.xyz

[U48] PHP：纯枚举
来源：http://fpr.gotoacloud.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://whw.ctjpmb.com

[U49] PHP：只读属性
来源：http://kgl.feifeiyinyue.top

public readonly string $name
来源：http://usx.hfpthk.cn

[U50] PHP：构造器属性提升
来源：http://qia.smart0.xyz

public function __construct(private int $id) {}
来源：http://xnq.bjfxy.top

[U51] PHP：数组解构
来源：http://bpo.kuanghao11.cn

[$a, $b] = $arr;
来源：http://fqn.zhixingplan.top

[U52] PHP：箭头函数
来源：http://sle.zhoulong.xyz

$double = fn($x) => $x * 2;
来源：http://hss.yanxiufei.cn

[U53] PHP：空合并运算符
来源：http://wfz.aizwys.cn

$v = $a ?? $b ?? "default";
来源：http://sip.chenlongwang.top

[U54] PHP：空安全调用
来源：http://aqe.andypj.xyz

$obj?->method()
来源：http://bgv.zhixingplan.top

[U55] PHP：match 表达式
来源：http://psn.yonumen.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hic.xuetiantiany.cn

[U56] PHP：命名参数
来源：http://jhw.guowangkeji.top

f(a: 1, b: 2)
来源：http://uad.feifeiyinyue.top

[U57] PHP：字符串插值
来源：http://gpc.jiagoushi.top

"值: {$a}"
来源：http://vyp.0kj1m.cn

[U58] PHP：数组三件套
来源：http://wuo.xinyue.icu

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://woo.yanxiufei.cn

[U59] PHP：自定义排序
来源：http://rjb.gotoacloud.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://qvw.9152youxi.cn

[U60] PHP：JSON 编解码
来源：http://rvk.kuanghao11.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://ofs.hysaishi.cn

[U61] PHP：正则
来源：http://jsb.zhiwuduotai.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://dmt.yuanzhike.top

[U62] PHP：日期对象
来源：http://jtl.ydzc1.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://knc.jqgfzy.top

[U63] PHP：文件读写
来源：http://wzv.yueranfly.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://beo.redwolf501.top

[U64] PHP：目录遍历
来源：http://qlp.fanxiaobao.xyz

glob("dir/*.php");  scandir("dir");
来源：http://dtl.9152youxi.cn

[U65] PHP：会话
来源：http://rvx.fanxiaobao.xyz

session_start();  $_SESSION["uid"] = 1;
来源：http://ajc.sjlbkw.cn

[U66] PHP：设置 Cookie
来源：http://hbf.cheryme.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://fiq.jiagoushi.top

[U67] PHP：处理文件上传
来源：http://omt.ybcxt.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://hpy.ydjk.org.cn

[U68] PHP：PDO 连接
来源：http://kvf.gaohongyu789.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://ofp.0kj1m.cn

[U69] PHP：PDO 预处理
来源：http://yct.jinqigufen.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://ypn.meibo888.top

[U70] PHP：PDO 事务
来源：http://ldd.zhixingplan.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://wzd.yonumen.top

[U71] PHP：抛出异常
来源：http://wuk.yonumen.top

throw new RuntimeException("失败", 500);
来源：http://qdo.gotoacloud.top

[U72] PHP：写错误日志
来源：http://wsw.jinyuanbaomall.cn

error_log("失败: " . $e->getMessage());
来源：http://cst.cucudq.cn

[U73] PHP：读取 ini 配置
来源：http://swg.epnwcf.com

parse_ini_file("config.ini", true)
来源：http://qad.jinqigfzy.top

[U74] PHP：读取环境变量
来源：http://peh.ehwqpu.com

getenv("APP_ENV") ?: "production"
来源：http://bdc.xylfe.cn

[U75] PHP：依赖注入
来源：http://bqt.havefunace.top

composer require psr/container
来源：http://gll.tanke756.top

[U76] PHP：简单路由
来源：http://qwu.ctjpmb.com

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://txb.andypj.xyz

[U77] PHP：模板渲染
来源：http://nih.zhiwuduotai.top

composer require twig/twig
来源：http://lta.fktsv.cn

[U78] PHP：单元测试
来源：http://yek.hammf.cn

composer require --dev phpunit/phpunit
来源：http://vje.zhijiandao.cn

[U79] PHP：静态分析
来源：http://gny.yj202588.top

composer require --dev phpstan/phpstan
来源：http://pib.snrcjt.cn

[U80] PHP：代码规范修复
来源：http://dlt.xylfe.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://nko.svipenyu.cn

[U81] JS：初始化项目
来源：http://gmh.c1oappe.top

npm init -y;  npm i express
来源：http://kdr.cucudq.cn

[U82] JS：package.json 脚本
来源：http://uwu.yangfankeji.com

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://anz.wangshuangyany.cn

[U83] JS：ES Module 导入导出
来源：http://ymw.jinqigufen.top

export const a = 1;  import { a } from "./m.js";
来源：http://qdi.tanke756.top

[U84] JS：CommonJS 写法
来源：http://tbz.wangdashe.top

module.exports = { a };  const { a } = require("./m");
来源：http://qrz.cucudq.cn

[U85] JS：可选链
来源：http://dgv.zycfv.cn

a?.b?.c
来源：http://ois.haohaochexian.top

[U86] JS：空值合并
来源：http://rkh.hysaishi.cn

a ?? b
来源：http://yir.aizwys.cn

[U87] JS：解构默认值
来源：http://ifw.c1oappe.top

const { a = 1, b = 2 } = obj;
来源：http://hlp.hesvh.cn

[U88] JS：对象展开合并
来源：http://bug.zhoulong.xyz

{ ...a, ...b }
来源：http://nst.hnxiangtu.top

[U89] JS：数组去重
来源：http://qzv.cucudq.cn

[...new Set(arr)]
来源：http://ngp.dianchejie.cn

[U90] JS：数字数组排序
来源：http://otx.9152youxi.cn

[...arr].sort((a, b) => a - b)
来源：http://den.pycfn.com

[U91] JS：对象键值遍历
来源：http://rbm.cucudq.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://cic.ybcxt.top

[U92] JS：深拷贝
来源：http://mkh.gaohongyu789.top

structuredClone(obj)
来源：http://dyp.guannengcc.top

[U93] JS：模板字符串
来源：http://bsq.shanyushiyangkeji.top

`共 ${n} 条`
来源：http://vpv.zhiwuduotai.top

[U94] JS：箭头函数
来源：http://fpw.gogol.net.cn

const double = x => x * 2;
来源：http://pmq.hcnkem.com

[U95] JS：Promise 包装
来源：http://xex.hysaishi.cn

new Promise((resolve, reject) => {})
来源：http://gtd.sufxvd.cn

[U96] JS：async/await 与异常
来源：http://ftb.zhixingplan.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://bkp.ehwqpu.com

[U97] JS：并发请求
来源：http://mtj.dianchejie.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://dey.pycfn.com

[U98] JS：fetch 带 JSON
来源：http://cri.epnwcf.com

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://efx.hongshengwenyu.top

[U99] JS：事件监听
来源：http://ftt.yanxiufei.cn

el.addEventListener("click", e => {})
来源：http://uzb.dianchejie.cn

[U100] JS：DOM 查询
来源：http://mip.xingfuxueyuan.xyz

document.querySelector(".item")
来源：http://cnq.chenlongwang.top

[U101] JS：classList 操作
来源：http://bur.snrcjt.cn

el.classList.toggle("active")
来源：http://mfa.yanxiufei.cn

[U102] JS：本地存储
来源：http://kwv.cdnleiting.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://cct.hcnkem.com

[U103] JS：定时器
来源：http://cnh.cheryme.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://fgt.ydzc1.top

[U104] JS：防抖
来源：http://bdq.hammf.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://vcm.yvedp.cn

[U105] JS：节流
来源：http://mzy.zhoulong.xyz

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://jlg.sxryk.cn

[U106] JS：日期格式化
来源：http://rhr.yonumen.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://xvu.bbcook.cn

[U107] JS：数字千分位
来源：http://fzy.bbcook.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://lrf.quarkkingdee.top

[U108] JS：随机整数
来源：http://xyr.nanxinkj.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://tmo.yanxiufei.cn

[U109] JS：数组分组
来源：http://wup.kuanghao11.cn

Object.groupBy(arr, x => x.type)
来源：http://gcp.daxiang520.top

[U110] JS：数组分块
来源：http://cqx.sweek.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://vwl.tianlin.xyz

[U111] JS：对象转 Map
来源：http://vdq.zhoulong.xyz

new Map(Object.entries(obj))
来源：http://uwh.zhengqikj.top

[U112] JS：字符串补位
来源：http://rgg.0kj1m.cn

"7".padStart(3, "0")
来源：http://ien.fengsongda.top

[U113] JS：正则替换全部
来源：http://pfe.zhongyouzk.top

s.replaceAll("a", "b")
来源：http://eot.redwolf501.top

[U114] JS：JSON 深比较
来源：http://jfb.shanyushiyangtech.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://fzf.tanke756.top

[U115] JS：生成 UUID
来源：http://ppl.yueranfly.top

crypto.randomUUID()
来源：http://qki.gotoacloud.top

[U116] JS：类型检查（JSDoc）
来源：http://riy.nanxinkj.top

/** @param {string} name */ function f(name) {}
来源：http://wbp.ppjwa.cn

[U117] JS：单元测试
来源：http://qlc.cdnleiting.top

npm i -D vitest;  npx vitest
来源：http://gus.dianchejie.cn

[U118] JS：开发服务器
来源：http://pcp.c1oappe.top

npm i -D vite;  npx vite
来源：http://hlh.shzxlz.cn

[U119] JS：生产构建
来源：http://cdi.jianghu66.top

npx vite build
来源：http://wwc.gogol.net.cn

[U120] JS：读取环境变量（Vite）
来源：http://tfx.vqdsnc.cn

import.meta.env.VITE_API_URL
来源：http://hgj.bbcook.cn


<!-- 参考信息 -->