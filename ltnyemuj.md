代发 wailian999

[T29] Swift：guard 提前返回
来源：http://zbk.ehwqpu.com

guard let x = opt else { return }
来源：http://svn.ybcxt.top

[T30] Swift：协议
来源：http://lee.c1oappe.top

protocol Shape { func area() -> Double }
来源：http://gat.shuidangran.top

[T31] Lua：Hello World
来源：http://lid.yueranfly.top

print("Hello")
来源：http://wzi.havefunace.top

[T32] Lua：局部变量
来源：http://ftu.birdmap.top

local a = 1
来源：http://uvx.xuanzx.com

[T33] Lua：表（数组）
来源：http://ekh.redwolf501.top

local t = {1, 2, 3};  t[4] = 4
来源：http://qfv.ydjk.org.cn

[T34] Lua：遍历表
来源：http://quy.shangyingyoupin.top

for i, v in ipairs(t) do print(i, v) end
来源：http://hda.cashguo.top

[T35] Lua：字典表
来源：http://nco.yongpay.top

local d = { a = 1 };  d.b = 2
来源：http://ipg.nanxinkj.top

[T36] Lua：函数
来源：http://ayi.c1oappe.top

function add(a, b) return a + b end
来源：http://dxh.guannengcc.top

[T37] Lua：字符串拼接
来源：http://jrr.9152youxi.cn

"a" .. "b"
来源：http://pul.hywenlv.cn

[T38] Lua：条件
来源：http://hkj.jianghu66.top

if x > 0 then print("正") end
来源：http://eda.zhoulong.xyz

[T39] Lua：模式匹配
来源：http://mgs.yanxiufei.cn

string.find(s, "%d+")
来源：http://hmy.yj202588.top

[T40] Lua：元表
来源：http://aac.cqqwz.cn

setmetatable({}, { __index = base })
来源：http://zjx.jinqigfzy.top

[T41] Perl：Hello World
来源：http://qne.zhengqikj.top

print "Hello\n";
来源：http://spv.hnqzz.top

[T42] Perl：变量类型
来源：http://caf.ctjpmb.com

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://zmn.wangdashe.top

[T43] Perl：字符串插值
来源：http://pml.birdmap.top

"值: $a"
来源：http://mxy.ivvv.top

[T44] Perl：条件
来源：http://zdz.hammf.cn

if ($a > 0) { print "正"; }
来源：http://gjq.jinqigufen.top

[T45] Perl：数组遍历
来源：http://mbz.daxiang520.top

for my $x (@arr) { print $x; }
来源：http://bqn.gogol.net.cn

[T46] Perl：哈希操作
来源：http://ahq.shanyushiyangkeji.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://xou.yongpay.top

[T47] Perl：正则捕获
来源：http://uid.shanyushiyangkeji.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://zaj.shanyushiyangkeji.top

[T48] Perl：正则替换
来源：http://zca.epnwcf.com

$s =~ s/old/new/g;
来源：http://lsk.zhiwuduotai.top

[T49] Perl：函数
来源：http://btd.shanyushiyangtech.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://oei.ehwqpu.com

[T50] Perl：逐行读文件
来源：http://ckl.jiagoushi.top

open my $fh, "<", "a.txt" or die $!;
来源：http://jmj.c1oappe.top

while (my $line = <$fh>) { print $line; }
来源：http://qmn.haohaochexian.top

[T51] Scala：Hello World
来源：http://lop.yvedp.cn

println("Hello")
来源：http://zna.jianghu66.top

[T52] Scala：变量
来源：http://civ.yj20258888.top

val a = 1;  var b = 2
来源：http://wuc.ydjk.org.cn

[T53] Scala：字符串插值
来源：http://ebh.iojbl.cn

s"值: $b"
来源：http://tjd.uphjek.com

[T54] Scala：集合映射
来源：http://bgk.jinqigufen.top

List(1, 2, 3).map(_ * 2)
来源：http://coo.ppjwa.cn

[T55] Scala：集合过滤
来源：http://ait.zycfv.cn

List(1, 2, 3).filter(_ > 1)
来源：http://xzl.hnqzz.top

[T56] Scala：样例类
来源：http://qoe.snrcjt.cn

case class User(name: String, age: Int)
来源：http://lpk.cucudq.cn

[T57] Scala：模式匹配
来源：http://wjg.cucudq.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://cya.hywenlv.cn

[T58] Scala：函数定义
来源：http://eio.cdnleiting.top

def add(a: Int, b: Int): Int = a + b
来源：http://dso.yonumen.top

[T59] Scala：循环
来源：http://jpk.zhengqikj.top

for (i <- 1 to 10) println(i)
来源：http://deb.yuanzhike.top

[T60] Scala：折叠
来源：http://swz.bbcook.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://czq.dashuyun.cn

================================================================================
来源：http://wmo.guannengcc.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://oes.hywenlv.cn

================================================================================
来源：http://vca.jlsjyb.cn

[U01] Py：创建虚拟环境
来源：http://erk.shanyushiyangkeji.top

python -m venv .venv && source .venv/bin/activate
来源：http://alp.guowangkeji.top

[U02] Py：导出 / 安装依赖
来源：http://kuj.nanxinkj.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://mcj.gotoacloud.top

[U03] Py：加载 .env 配置
来源：http://qnu.zhoulong.xyz

from dotenv import load_dotenv; load_dotenv()
来源：http://hnx.yanxiufei.cn

[U04] Py：变量调试打印
来源：http://oix.sysykeji.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://vnd.birdmap.top

[U05] Py：列表去重且保序
来源：http://jap.vqdsnc.cn

list(dict.fromkeys(arr))
来源：http://jpv.daria6918.cn

[U06] Py：合并两个字典
来源：http://dlo.yj202588.top

{**a, **b}
来源：http://oxx.fktsv.cn

[U07] Py：反转字典键值
来源：http://uqm.fehbvm.com

{v: k for k, v in d.items()}
来源：http://nqx.iojbl.cn

[U08] Py：展平二维列表
来源：http://exu.xuanzx.com

[y for x in nested for y in x]
来源：http://fkd.zhongyouzk.top

[U09] Py：字典取最大值的键
来源：http://nkm.cheryme.top

max(d, key=d.get)
来源：http://ndf.hongshengwenyu.top

[U10] Py：按值排序字典
来源：http://bfc.epnwcf.com

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://gpk.ybcxt.top

[U11] Py：生成器表达式
来源：http://lwr.vqdsnc.cn

(x * 2 for x in arr)
来源：http://fcp.haohaochexian.top

[U12] Py：取出现最多的 3 个元素
来源：http://zvd.shzxlz.cn

Counter(arr).most_common(3)
来源：http://lno.haohaochexian.top

[U13] Py：固定长度队列
来源：http://vto.bbcook.cn

deque(maxlen=10)
来源：http://zeg.zhoulong.xyz

[U14] Py：分组收集到列表
来源：http://rai.yfazqb.com

defaultdict(list)
来源：http://ksv.jlsjyb.cn

[U15] Py：高精度计时
来源：http://gjf.vqdsnc.cn

t = time.perf_counter()
来源：http://hwj.tianlin.xyz

[U16] Py：命令行参数解析
来源：http://yka.gaohongyu789.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://fee.bbcook.cn

[U17] Py：初始化日志
来源：http://jnf.ydjk.org.cn

logging.basicConfig(level=logging.INFO)
来源：http://iyw.sjlbkw.cn

[U18] Py：预编译正则
来源：http://bqk.mhx1999.top

pat = re.compile(r"\d+")
来源：http://cjm.bjfxy.top

[U19] Py：正则替换带回调
来源：http://bkr.cqqwz.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://dxj.shzxlz.cn

[U20] Py：缓存函数结果
来源：http://epm.ywan-chungtsiang.top

@functools.lru_cache(maxsize=None)
来源：http://nwq.vehdjk.com

[U21] Py：自定义上下文管理器
来源：http://zfw.hnqzz.top

@contextlib.contextmanager
来源：http://aur.feifeiyinyue.top

[U22] Py：矩阵转置
来源：http://csb.fengsongda.top

list(zip(*m))
来源：http://kzy.bbcook.cn

[U23] Py：分块读取大文件
来源：http://dcf.yuanzhike.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://ebv.hywenlv.cn

[U24] Py：路径操作
来源：http://gto.cucudq.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://ger.hfpthk.cn

[U25] Py：CSV 按字典读
来源：http://usg.mhx1999.top

csv.DictReader(f)
来源：http://pcm.jqgufenzy.top

[U26] Py：并发下载
来源：http://qzw.smart0.xyz

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://iph.zhijiandao.cn

[U27] Py：异步 HTTP
来源：http://agn.52xcode.cn

aiohttp.ClientSession() 配合 async with
来源：http://wge.c1oappe.top

[U28] Py：类型别名
来源：http://uhv.chenlongwang.top

UserId = int
来源：http://udg.nwbrower.top

[U29] Py：属性校验
来源：http://fvt.meibo888.top

@property 与 @x.setter 配合
来源：http://elr.aibaodan.cn

[U30] Py：数据类
来源：http://wat.zhengqikj.top

@dataclass(slots=True)
来源：http://sax.ywan-chungtsiang.top

[U31] Py：单测
来源：http://uhl.aizwys.cn

python -m pytest -q
来源：http://ajv.xinyue.icu

[U32] Py：代码格式化
来源：http://szy.zdbjq.cn

ruff format . && ruff check --fix .
来源：http://flk.fzhhl.top

[U33] Py：打包发布
来源：http://hqz.hesvh.cn

python -m build  （依赖 pyproject.toml）
来源：http://hok.yongpay.top

[U34] Py：判断编码
来源：http://cpn.jlsjyb.cn

chardet.detect(raw)
来源：http://yho.jinqigfzy.top

[U35] Py：发送邮件
来源：http://xro.uphjek.com

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://bcw.chenjidiqi.icu

[U36] Py：定时任务
来源：http://mlg.ywan-chungtsiang.top

schedule.every(10).minutes.do(job)
来源：http://mmd.hammf.cn

[U37] Py：读写 Excel
来源：http://cqh.svipenyu.cn

pandas.read_excel / DataFrame.to_excel
来源：http://gkb.birdmap.top

[U38] Py：获取脚本所在目录
来源：http://mxl.gogol.net.cn

Path(__file__).resolve().parent
来源：http://ghm.zdqjudy.top

[U39] Py：判断是否在交互环境
来源：http://dzk.0kj1m.cn

sys.stdout.isatty()
来源：http://qvn.jinyuanbaomall.cn

[U40] Py：打印到标准错误
来源：http://bnv.zdbjq.cn

print("err", file=sys.stderr)
来源：http://qxb.yueranfly.top

[U41] PHP：初始化 Composer 项目
来源：http://zjs.hywenlv.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://mjc.feifeiyinyue.top

[U42] PHP：PSR-4 自动加载
来源：http://ilc.fktsv.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://tef.daria6918.cn

[U43] PHP：声明命名空间
来源：http://kdm.zycfv.cn

namespace App\Http;
来源：http://edj.zdbjq.cn

[U44] PHP：开启严格类型
来源：http://pht.snrcjt.cn

declare(strict_types=1);
来源：http://kov.shanyushiyangkeji.top

[U45] PHP：类型声明与返回类型
来源：http://sex.chenzaomai.com

function add(int $a, int $b): int { return $a + $b; }
来源：http://rai.yueranfly.top

[U46] PHP：可空类型
来源：http://ftd.chenjidiqi.icu

?string $name = null
来源：http://scj.uphjek.com

[U47] PHP：联合类型
来源：http://evt.kuanghao11.cn

int|string $id
来源：http://cyu.bjfxy.top

[U48] PHP：纯枚举
来源：http://msv.svipenyu.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://sgs.bjfxy.top

[U49] PHP：只读属性
来源：http://zwy.zhixingplan.top

public readonly string $name
来源：http://vuq.zhaomingkeji.xyz

[U50] PHP：构造器属性提升
来源：http://uoq.tanke756.top

public function __construct(private int $id) {}
来源：http://cro.cashguo.top

[U51] PHP：数组解构
来源：http://shs.gzhubu.top

[$a, $b] = $arr;
来源：http://sdv.xuanzx.com

[U52] PHP：箭头函数
来源：http://rsm.zhengqikj.top

$double = fn($x) => $x * 2;
来源：http://vtc.ydjk.org.cn

[U53] PHP：空合并运算符
来源：http://tnm.hnxiangtu.top

$v = $a ?? $b ?? "default";
来源：http://gtf.jqgufenzy.top

[U54] PHP：空安全调用
来源：http://xfr.cucudq.cn

$obj?->method()
来源：http://zvl.guannengcc.top

[U55] PHP：match 表达式
来源：http://cgb.jiagoushi.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://vxk.svipenyu.cn

[U56] PHP：命名参数
来源：http://oye.xingfuxueyuan.xyz

f(a: 1, b: 2)
来源：http://kaa.aibaodan.cn

[U57] PHP：字符串插值
来源：http://ivy.aibaodan.cn

"值: {$a}"
来源：http://vzg.9152youxi.cn

[U58] PHP：数组三件套
来源：http://bsu.cqqwz.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://bsv.cqqwz.cn

[U59] PHP：自定义排序
来源：http://cmk.sysykeji.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hfl.ywan-chungtsiang.top

[U60] PHP：JSON 编解码
来源：http://nbr.epnwcf.com

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://eco.pycfn.com

[U61] PHP：正则
来源：http://hjd.hcnkem.com

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://nho.epnwcf.com

[U62] PHP：日期对象
来源：http://iic.hnxiangtu.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://tms.nwbrower.top

[U63] PHP：文件读写
来源：http://wzh.ivvv.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://wob.chenzaomai.com

[U64] PHP：目录遍历
来源：http://gxr.kuanghao11.cn

glob("dir/*.php");  scandir("dir");
来源：http://gva.jqgufenzy.top

[U65] PHP：会话
来源：http://wzt.fanxiaobao.xyz

session_start();  $_SESSION["uid"] = 1;
来源：http://rmt.yuxming.cn

[U66] PHP：设置 Cookie
来源：http://mzi.zdqjudy.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://pep.yongpay.top

[U67] PHP：处理文件上传
来源：http://ufc.bjfxy.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://ubc.gzhubu.top

[U68] PHP：PDO 连接
来源：http://eme.tian-w.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://gbe.jinqigfzy.top

[U69] PHP：PDO 预处理
来源：http://bzc.hysaishi.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://nue.cucudq.cn

[U70] PHP：PDO 事务
来源：http://oap.dianchejie.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://uqh.xinyue.icu

[U71] PHP：抛出异常
来源：http://oso.shanyushiyangtech.top

throw new RuntimeException("失败", 500);
来源：http://kip.sysykeji.top

[U72] PHP：写错误日志
来源：http://vaq.nanxuanxn.top

error_log("失败: " . $e->getMessage());
来源：http://nee.dashuyun.cn

[U73] PHP：读取 ini 配置
来源：http://rlb.hcnkem.com

parse_ini_file("config.ini", true)
来源：http://lho.feifeiyinyue.top

[U74] PHP：读取环境变量
来源：http://cnr.dashuyun.cn

getenv("APP_ENV") ?: "production"
来源：http://ewz.aizwys.cn

[U75] PHP：依赖注入
来源：http://vtd.chenjidiqi.icu

composer require psr/container
来源：http://wec.shangyingyoupin.top

[U76] PHP：简单路由
来源：http://bsq.hysaishi.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://plp.guannengcc.top

[U77] PHP：模板渲染
来源：http://lzp.tarul.cn

composer require twig/twig
来源：http://krp.xuanzx.com

[U78] PHP：单元测试
来源：http://zsu.shzxlz.cn

composer require --dev phpunit/phpunit
来源：http://elo.316326.xyz

[U79] PHP：静态分析
来源：http://mqa.cheryme.top

composer require --dev phpstan/phpstan
来源：http://pnc.bbcook.cn

[U80] PHP：代码规范修复
来源：http://avs.jinyuanbaomall.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://dru.vehdjk.com

[U81] JS：初始化项目
来源：http://nsn.feifeiyinyue.top

npm init -y;  npm i express
来源：http://qjq.aibaodan.cn

[U82] JS：package.json 脚本
来源：http://iob.svipenyu.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://xvw.9152youxi.cn

[U83] JS：ES Module 导入导出
来源：http://eao.c1oappe.top

export const a = 1;  import { a } from "./m.js";
来源：http://yec.sweek.top

[U84] JS：CommonJS 写法
来源：http://kxv.9152youxi.cn

module.exports = { a };  const { a } = require("./m");
来源：http://wbi.quarkkingdee.top

[U85] JS：可选链
来源：http://joa.jiagoushi.top

a?.b?.c
来源：http://xdm.0kj1m.cn

[U86] JS：空值合并
来源：http://hlc.jinyuanbaomall.cn

a ?? b
来源：http://ooo.ydzc1.top

[U87] JS：解构默认值
来源：http://qxw.yueranfly.top

const { a = 1, b = 2 } = obj;
来源：http://svw.zdqjudy.top

[U88] JS：对象展开合并
来源：http://ubm.shanyushiyangkeji.top

{ ...a, ...b }
来源：http://dob.bbcook.cn

[U89] JS：数组去重
来源：http://kni.jiagoushi.top

[...new Set(arr)]
来源：http://qnd.bbcook.cn

[U90] JS：数字数组排序
来源：http://iex.nwbrower.top

[...arr].sort((a, b) => a - b)
来源：http://wfj.vqdsnc.cn

[U91] JS：对象键值遍历
来源：http://rzf.wangdashe.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://lck.gogol.net.cn

[U92] JS：深拷贝
来源：http://mtk.bjfxy.top

structuredClone(obj)
来源：http://czo.hesvh.cn

[U93] JS：模板字符串
来源：http://rfs.sufxvd.cn

`共 ${n} 条`
来源：http://iue.jiagoushi.top

[U94] JS：箭头函数
来源：http://etf.ctjpmb.com

const double = x => x * 2;
来源：http://dmb.chenlongwang.top

[U95] JS：Promise 包装
来源：http://bmm.gaohongyu789.top

new Promise((resolve, reject) => {})
来源：http://djf.cucudq.cn

[U96] JS：async/await 与异常
来源：http://irg.shzxlz.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://ycm.aizwys.cn

[U97] JS：并发请求
来源：http://lly.birdmap.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://wva.guowangkeji.top

[U98] JS：fetch 带 JSON
来源：http://del.cashguo.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://uer.bjfxy.top

[U99] JS：事件监听
来源：http://zeb.svipenyu.cn

el.addEventListener("click", e => {})
来源：http://tnk.jyoumei.cn

[U100] JS：DOM 查询
来源：http://vts.yueranfly.top

document.querySelector(".item")
来源：http://jxu.yueranfly.top

[U101] JS：classList 操作
来源：http://kdr.feifeiyinyue.top

el.classList.toggle("active")
来源：http://rek.jiagoushi.top

[U102] JS：本地存储
来源：http://vht.jqgufenzy.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://ohy.fktsv.cn

[U103] JS：定时器
来源：http://pyi.haohaochexian.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://xag.jianghu66.top

[U104] JS：防抖
来源：http://yql.wangshuangyany.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://gkw.316326.xyz

[U105] JS：节流
来源：http://ude.xylfe.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://oxa.ydzc1.top

[U106] JS：日期格式化
来源：http://gus.ehwqpu.com

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://ewb.yvedp.cn

[U107] JS：数字千分位
来源：http://jjs.bjfxy.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://rfa.hywenlv.cn

[U108] JS：随机整数
来源：http://mtk.yanxiufei.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://rva.sysykeji.top

[U109] JS：数组分组
来源：http://ovg.meibo888.top

Object.groupBy(arr, x => x.type)
来源：http://fhm.chenlongwang.top

[U110] JS：数组分块
来源：http://nmp.fanxiaobao.xyz

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://rvd.daxiang520.top

[U111] JS：对象转 Map
来源：http://fcq.andypj.xyz

new Map(Object.entries(obj))
来源：http://cev.haohaochexian.top

[U112] JS：字符串补位
来源：http://uvw.yfazqb.com

"7".padStart(3, "0")
来源：http://zep.hcnkem.com

[U113] JS：正则替换全部
来源：http://psl.ydzc1.top

s.replaceAll("a", "b")
来源：http://swc.nanxinkj.top

[U114] JS：JSON 深比较
来源：http://vsh.ctjpmb.com

JSON.stringify(a) === JSON.stringify(b)
来源：http://zrd.ehwqpu.com

[U115] JS：生成 UUID
来源：http://ubu.wangdashe.top

crypto.randomUUID()
来源：http://yfy.gotoacloud.top

[U116] JS：类型检查（JSDoc）
来源：http://bsm.hammf.cn

/** @param {string} name */ function f(name) {}
来源：http://xiv.wangdashe.top


<!-- 参考信息 -->