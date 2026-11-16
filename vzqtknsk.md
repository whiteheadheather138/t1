代发 wailian999

[T23] Swift：函数
来源：http://hvg.tian-w.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://zqh.yj20258.top

[T24] Swift：闭包
来源：http://oqd.hnxiangtu.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://wnq.zdqjudy.top

[T25] Swift：结构体
来源：http://kri.ydjk.org.cn

struct P { var x: Int }
来源：http://ngf.jiagoushi.top

[T26] Swift：类与重写
来源：http://rks.birdmap.top

class A: Base { override func f() {} }
来源：http://vdp.yanxiufei.cn

[T27] Swift：错误处理
来源：http://yvj.zycfv.cn

do { try f() } catch { print(error) }
来源：http://isa.c1oappe.top

[T28] Swift：枚举
来源：http://gvh.yj20258.top

enum Color { case red, green }
来源：http://xne.vehdjk.com

[T29] Swift：guard 提前返回
来源：http://dnj.ehwqpu.com

guard let x = opt else { return }
来源：http://fhy.mhx1999.top

[T30] Swift：协议
来源：http://asu.zdbjq.cn

protocol Shape { func area() -> Double }
来源：http://ryr.mhx1999.top

[T31] Lua：Hello World
来源：http://hfo.ehwqpu.com

print("Hello")
来源：http://qeu.ivvv.top

[T32] Lua：局部变量
来源：http://lke.hammf.cn

local a = 1
来源：http://pip.nwbrower.top

[T33] Lua：表（数组）
来源：http://cit.guowangkeji.top

local t = {1, 2, 3};  t[4] = 4
来源：http://syf.jinqigfzy.top

[T34] Lua：遍历表
来源：http://qsn.zycfv.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://fzg.zhiwuduotai.top

[T35] Lua：字典表
来源：http://cty.zdbjq.cn

local d = { a = 1 };  d.b = 2
来源：http://ykz.ivvv.top

[T36] Lua：函数
来源：http://oif.redwolf501.top

function add(a, b) return a + b end
来源：http://nxn.dianchejie.cn

[T37] Lua：字符串拼接
来源：http://nbm.cheryme.top

"a" .. "b"
来源：http://lmk.jianghu66.top

[T38] Lua：条件
来源：http://gbf.sxryk.cn

if x > 0 then print("正") end
来源：http://emi.hnqzz.top

[T39] Lua：模式匹配
来源：http://krc.yj202588.top

string.find(s, "%d+")
来源：http://qoa.meibo888.top

[T40] Lua：元表
来源：http://bof.yongpay.top

setmetatable({}, { __index = base })
来源：http://voo.chenzaomai.com

[T41] Perl：Hello World
来源：http://cnp.tian-w.cn

print "Hello\n";
来源：http://niq.hysaishi.cn

[T42] Perl：变量类型
来源：http://amd.shanyushiyangtech.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://gge.xinyue.icu

[T43] Perl：字符串插值
来源：http://gld.fktsv.cn

"值: $a"
来源：http://rdt.c1oappe.top

[T44] Perl：条件
来源：http://yzq.yongpay.top

if ($a > 0) { print "正"; }
来源：http://csl.wangshuangyany.cn

[T45] Perl：数组遍历
来源：http://mzu.hammf.cn

for my $x (@arr) { print $x; }
来源：http://jdc.snrcjt.cn

[T46] Perl：哈希操作
来源：http://uvv.dianchejie.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://wiq.zhengqikj.top

[T47] Perl：正则捕获
来源：http://qyk.hnxiangtu.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://iad.cashguo.top

[T48] Perl：正则替换
来源：http://gym.yuxming.cn

$s =~ s/old/new/g;
来源：http://taq.sjlbkw.cn

[T49] Perl：函数
来源：http://ste.guannengcc.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://qyb.smart0.xyz

[T50] Perl：逐行读文件
来源：http://kfm.jinqigufen.top

open my $fh, "<", "a.txt" or die $!;
来源：http://amd.hysaishi.cn

while (my $line = <$fh>) { print $line; }
来源：http://fry.shanyushiyangtech.top

[T51] Scala：Hello World
来源：http://pua.hywenlv.cn

println("Hello")
来源：http://mtf.sxryk.cn

[T52] Scala：变量
来源：http://uyu.guannengcc.top

val a = 1;  var b = 2
来源：http://lqm.jinqigufen.top

[T53] Scala：字符串插值
来源：http://nmd.quarkkingdee.top

s"值: $b"
来源：http://igz.ivvv.top

[T54] Scala：集合映射
来源：http://bfo.chenjidiqi.icu

List(1, 2, 3).map(_ * 2)
来源：http://wgj.cheryme.top

[T55] Scala：集合过滤
来源：http://tok.mhx1999.top

List(1, 2, 3).filter(_ > 1)
来源：http://ijj.gaohongyu789.top

[T56] Scala：样例类
来源：http://gmb.hammf.cn

case class User(name: String, age: Int)
来源：http://dwo.hnxiangtu.top

[T57] Scala：模式匹配
来源：http://eup.chenjidiqi.icu

x match { case 1 => "一"; case _ => "其他" }
来源：http://ykj.dashuyun.cn

[T58] Scala：函数定义
来源：http://ywa.aizwys.cn

def add(a: Int, b: Int): Int = a + b
来源：http://hgr.316326.xyz

[T59] Scala：循环
来源：http://dlo.havefunace.top

for (i <- 1 to 10) println(i)
来源：http://zwx.sysykeji.top

[T60] Scala：折叠
来源：http://avf.nwbrower.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://qun.smart0.xyz

================================================================================
来源：http://tcp.bbcook.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://zkg.jinyuanbaomall.cn

================================================================================
来源：http://bxt.yongpay.top

[U01] Py：创建虚拟环境
来源：http://ipn.yongpay.top

python -m venv .venv && source .venv/bin/activate
来源：http://ddt.bbcook.cn

[U02] Py：导出 / 安装依赖
来源：http://xmp.ctjpmb.com

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://sqp.yfazqb.com

[U03] Py：加载 .env 配置
来源：http://pxy.shzxlz.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://edd.xingfuxueyuan.xyz

[U04] Py：变量调试打印
来源：http://xkt.aizwys.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://ghv.nwbrower.top

[U05] Py：列表去重且保序
来源：http://okm.hysaishi.cn

list(dict.fromkeys(arr))
来源：http://qrz.hysaishi.cn

[U06] Py：合并两个字典
来源：http://lht.sweek.top

{**a, **b}
来源：http://ypu.cheryme.top

[U07] Py：反转字典键值
来源：http://hti.zhengqikj.top

{v: k for k, v in d.items()}
来源：http://xjd.gogol.net.cn

[U08] Py：展平二维列表
来源：http://rlr.tian-w.cn

[y for x in nested for y in x]
来源：http://jja.yanxiufei.cn

[U09] Py：字典取最大值的键
来源：http://xgy.hammf.cn

max(d, key=d.get)
来源：http://iii.zhongyouzk.top

[U10] Py：按值排序字典
来源：http://amc.hnqzz.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://xxr.dianchejie.cn

[U11] Py：生成器表达式
来源：http://xdf.52xcode.cn

(x * 2 for x in arr)
来源：http://ovp.zhixingplan.top

[U12] Py：取出现最多的 3 个元素
来源：http://wpt.fengsongda.top

Counter(arr).most_common(3)
来源：http://rko.pengpengdd.cyou

[U13] Py：固定长度队列
来源：http://rwy.xingfuxueyuan.xyz

deque(maxlen=10)
来源：http://gxb.tianlin.xyz

[U14] Py：分组收集到列表
来源：http://gle.shanyushiyangtech.top

defaultdict(list)
来源：http://hhv.sweek.top

[U15] Py：高精度计时
来源：http://zrv.aizwys.cn

t = time.perf_counter()
来源：http://lhd.chenlongwang.top

[U16] Py：命令行参数解析
来源：http://ddd.tarul.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://mhg.jqgfzy.top

[U17] Py：初始化日志
来源：http://xja.fanxiaobao.xyz

logging.basicConfig(level=logging.INFO)
来源：http://xxb.tianlin.xyz

[U18] Py：预编译正则
来源：http://hca.tarul.cn

pat = re.compile(r"\d+")
来源：http://gwz.fzhhl.top

[U19] Py：正则替换带回调
来源：http://git.yfazqb.com

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://skv.ydjk.org.cn

[U20] Py：缓存函数结果
来源：http://mwr.shanyushiyangkeji.top

@functools.lru_cache(maxsize=None)
来源：http://dpk.9152youxi.cn

[U21] Py：自定义上下文管理器
来源：http://qhx.9152youxi.cn

@contextlib.contextmanager
来源：http://qzl.tarul.cn

[U22] Py：矩阵转置
来源：http://pea.uphjek.com

list(zip(*m))
来源：http://qbf.iojbl.cn

[U23] Py：分块读取大文件
来源：http://qss.xuanzx.com

for chunk in iter(lambda: f.read(8192), b""):
来源：http://gji.fanxiaobao.xyz

[U24] Py：路径操作
来源：http://pyb.zhiwuduotai.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://psj.shzxlz.cn

[U25] Py：CSV 按字典读
来源：http://tho.jqgfzy.top

csv.DictReader(f)
来源：http://gwy.fktsv.cn

[U26] Py：并发下载
来源：http://vcq.bbcook.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://uom.gotoacloud.top

[U27] Py：异步 HTTP
来源：http://ijh.52xcode.cn

aiohttp.ClientSession() 配合 async with
来源：http://qxu.fengsongda.top

[U28] Py：类型别名
来源：http://zpm.sysykeji.top

UserId = int
来源：http://gqy.c1oappe.top

[U29] Py：属性校验
来源：http://mwa.zdbjq.cn

@property 与 @x.setter 配合
来源：http://pad.jlsjyb.cn

[U30] Py：数据类
来源：http://izn.haohaochexian.top

@dataclass(slots=True)
来源：http://hkz.snrcjt.cn

[U31] Py：单测
来源：http://ocj.jqgfzy.top

python -m pytest -q
来源：http://tmq.ybcxt.top

[U32] Py：代码格式化
来源：http://nrj.wangshuangyany.cn

ruff format . && ruff check --fix .
来源：http://xyr.jiagoushi.top

[U33] Py：打包发布
来源：http://jyc.tanke756.top

python -m build  （依赖 pyproject.toml）
来源：http://qvl.0kj1m.cn

[U34] Py：判断编码
来源：http://tgb.ppjwa.cn

chardet.detect(raw)
来源：http://ebk.aibaodan.cn

[U35] Py：发送邮件
来源：http://eeh.nwbrower.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://jzl.wangdashe.top

[U36] Py：定时任务
来源：http://kcn.daxiang520.top

schedule.every(10).minutes.do(job)
来源：http://wwk.havefunace.top

[U37] Py：读写 Excel
来源：http://hhe.guowangkeji.top

pandas.read_excel / DataFrame.to_excel
来源：http://rbi.gzhubu.top

[U38] Py：获取脚本所在目录
来源：http://xjx.jlsjyb.cn

Path(__file__).resolve().parent
来源：http://lmq.cucudq.cn

[U39] Py：判断是否在交互环境
来源：http://mrd.bjfxy.top

sys.stdout.isatty()
来源：http://irc.mhx1999.top

[U40] Py：打印到标准错误
来源：http://cnm.jyoumei.cn

print("err", file=sys.stderr)
来源：http://wgp.sysykeji.top

[U41] PHP：初始化 Composer 项目
来源：http://hgg.guannengcc.top

composer init;  composer require guzzlehttp/guzzle
来源：http://vyp.havefunace.top

[U42] PHP：PSR-4 自动加载
来源：http://rew.guowangkeji.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://lit.jiagoushi.top

[U43] PHP：声明命名空间
来源：http://lmo.zhaomingkeji.xyz

namespace App\Http;
来源：http://alw.hywenlv.cn

[U44] PHP：开启严格类型
来源：http://otc.yfazqb.com

declare(strict_types=1);
来源：http://ngu.yj202588.top

[U45] PHP：类型声明与返回类型
来源：http://shh.gotoacloud.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://let.jinyuanbaomall.cn

[U46] PHP：可空类型
来源：http://wlu.ydjk.org.cn

?string $name = null
来源：http://nyg.chenlongwang.top

[U47] PHP：联合类型
来源：http://oeg.316326.xyz

int|string $id
来源：http://kit.hcnkem.com

[U48] PHP：纯枚举
来源：http://mfj.hammf.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://gqx.zhijiandao.cn

[U49] PHP：只读属性
来源：http://bsr.nanxuanxn.top

public readonly string $name
来源：http://yzo.zdqjudy.top

[U50] PHP：构造器属性提升
来源：http://kxj.sufxvd.cn

public function __construct(private int $id) {}
来源：http://hbt.zhengqikj.top

[U51] PHP：数组解构
来源：http://ejf.pycfn.com

[$a, $b] = $arr;
来源：http://rlu.pengpengdd.cyou

[U52] PHP：箭头函数
来源：http://mmm.dianchejie.cn

$double = fn($x) => $x * 2;
来源：http://vhn.tianlin.xyz

[U53] PHP：空合并运算符
来源：http://zav.cashguo.top

$v = $a ?? $b ?? "default";
来源：http://xnb.pengpengdd.cyou

[U54] PHP：空安全调用
来源：http://zxp.ivvv.top

$obj?->method()
来源：http://scz.yanxiufei.cn

[U55] PHP：match 表达式
来源：http://mca.hcnkem.com

$s = match($x) { 1 => "一", default => "其他" };
来源：http://cft.hywenlv.cn

[U56] PHP：命名参数
来源：http://mvm.ppjwa.cn

f(a: 1, b: 2)
来源：http://fhl.jiagoushi.top

[U57] PHP：字符串插值
来源：http://uma.shangyingyoupin.top

"值: {$a}"
来源：http://smu.ehwqpu.com

[U58] PHP：数组三件套
来源：http://exf.hfpthk.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://xfn.chenlongwang.top

[U59] PHP：自定义排序
来源：http://eqc.zhijiandao.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wxl.feifeiyinyue.top

[U60] PHP：JSON 编解码
来源：http://lla.haohaochexian.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://ehu.redwolf501.top

[U61] PHP：正则
来源：http://cme.iojbl.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://nmc.xylfe.cn

[U62] PHP：日期对象
来源：http://gqc.jqgufenzy.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://xah.jianghu66.top

[U63] PHP：文件读写
来源：http://cjb.haohaochexian.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://tmy.yvedp.cn

[U64] PHP：目录遍历
来源：http://dzl.ivvv.top

glob("dir/*.php");  scandir("dir");
来源：http://mxx.yuxming.cn

[U65] PHP：会话
来源：http://tyt.yvedp.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://lyv.dianchejie.cn

[U66] PHP：设置 Cookie
来源：http://jro.nwbrower.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://bwi.gogol.net.cn

[U67] PHP：处理文件上传
来源：http://wmj.vqdsnc.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://kvl.zhixingplan.top

[U68] PHP：PDO 连接
来源：http://irz.zycfv.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://xrs.9152youxi.cn

[U69] PHP：PDO 预处理
来源：http://xru.xylfe.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://spm.nwbrower.top

[U70] PHP：PDO 事务
来源：http://hdh.jinghuilouyu.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://qeq.yfazqb.com

[U71] PHP：抛出异常
来源：http://dyc.yj20258888.top

throw new RuntimeException("失败", 500);
来源：http://ntq.birdmap.top

[U72] PHP：写错误日志
来源：http://kne.ivvv.top

error_log("失败: " . $e->getMessage());
来源：http://dzn.andypj.xyz

[U73] PHP：读取 ini 配置
来源：http://hwp.chenlongwang.top

parse_ini_file("config.ini", true)
来源：http://ngb.ydzc1.top

[U74] PHP：读取环境变量
来源：http://qxv.nanxinkj.top

getenv("APP_ENV") ?: "production"
来源：http://apl.hcnkem.com

[U75] PHP：依赖注入
来源：http://myr.chenlongwang.top

composer require psr/container
来源：http://vlq.zycfv.cn

[U76] PHP：简单路由
来源：http://lac.dianchejie.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://jby.fengsongda.top

[U77] PHP：模板渲染
来源：http://xbk.hfpthk.cn

composer require twig/twig
来源：http://cyc.yuxming.cn

[U78] PHP：单元测试
来源：http://wdt.hesvh.cn

composer require --dev phpunit/phpunit
来源：http://gmv.ydjk.org.cn

[U79] PHP：静态分析
来源：http://sgk.tarul.cn

composer require --dev phpstan/phpstan
来源：http://ckm.ydjk.org.cn

[U80] PHP：代码规范修复
来源：http://fzu.nanxuanxn.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://yjf.xuetiantiany.cn

[U81] JS：初始化项目
来源：http://vhx.yueranfly.top

npm init -y;  npm i express
来源：http://paj.shanyushiyangkeji.top

[U82] JS：package.json 脚本
来源：http://vni.dashuyun.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://zrv.ivvv.top

[U83] JS：ES Module 导入导出
来源：http://vag.ydzc1.top

export const a = 1;  import { a } from "./m.js";
来源：http://ozq.hcnkem.com

[U84] JS：CommonJS 写法
来源：http://nkt.xylfe.cn

module.exports = { a };  const { a } = require("./m");
来源：http://yqj.guannengcc.top

[U85] JS：可选链
来源：http://jgv.dashuyun.cn

a?.b?.c
来源：http://gcv.yanxiufei.cn

[U86] JS：空值合并
来源：http://lbo.316326.xyz

a ?? b
来源：http://xyy.jlsjyb.cn

[U87] JS：解构默认值
来源：http://sub.chenzaomai.com

const { a = 1, b = 2 } = obj;
来源：http://ykw.chenzaomai.com

[U88] JS：对象展开合并
来源：http://lcv.jlsjyb.cn

{ ...a, ...b }
来源：http://qxw.yj20258888.top

[U89] JS：数组去重
来源：http://yzs.316326.xyz

[...new Set(arr)]
来源：http://isf.zdbjq.cn

[U90] JS：数字数组排序
来源：http://lrq.xylfe.cn

[...arr].sort((a, b) => a - b)
来源：http://xac.jqgufenzy.top

[U91] JS：对象键值遍历
来源：http://xpp.zhaomingkeji.xyz

Object.entries(obj).forEach(([k, v]) => {});
来源：http://mmb.ivvv.top

[U92] JS：深拷贝
来源：http://tga.epnwcf.com

structuredClone(obj)
来源：http://xpw.kuanghao11.cn

[U93] JS：模板字符串
来源：http://rlw.zhiwuduotai.top

`共 ${n} 条`
来源：http://xwf.pengpengdd.cyou

[U94] JS：箭头函数
来源：http://qoz.ctjpmb.com

const double = x => x * 2;
来源：http://sdx.uphjek.com

[U95] JS：Promise 包装
来源：http://sed.yj202588.top

new Promise((resolve, reject) => {})
来源：http://qvb.ivvv.top

[U96] JS：async/await 与异常
来源：http://hnj.snrcjt.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://bpo.jiagoushi.top

[U97] JS：并发请求
来源：http://quk.xinyue.icu

await Promise.all(urls.map(u => fetch(u)))
来源：http://nle.guowangkeji.top

[U98] JS：fetch 带 JSON
来源：http://lsu.cheryme.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://ijx.wangshuangyany.cn

[U99] JS：事件监听
来源：http://lvi.wangshuangyany.cn

el.addEventListener("click", e => {})
来源：http://jvj.nanxuanxn.top

[U100] JS：DOM 查询
来源：http://czv.sweek.top

document.querySelector(".item")
来源：http://kkg.andypj.xyz

[U101] JS：classList 操作
来源：http://sae.sxryk.cn

el.classList.toggle("active")
来源：http://wey.hysaishi.cn

[U102] JS：本地存储
来源：http://yzc.zdbjq.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://asq.yonumen.top

[U103] JS：定时器
来源：http://byr.shangyingyoupin.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://rie.andypj.xyz

[U104] JS：防抖
来源：http://jbe.316326.xyz

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://qrw.ivvv.top

[U105] JS：节流
来源：http://waw.hnxiangtu.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://cbb.xinyue.icu

[U106] JS：日期格式化
来源：http://tfg.jinqigfzy.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://zgx.vqdsnc.cn

[U107] JS：数字千分位
来源：http://mtn.jqgufenzy.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://qny.smart0.xyz

[U108] JS：随机整数
来源：http://fkx.epnwcf.com

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://pzx.cqqwz.cn

[U109] JS：数组分组
来源：http://axw.tian-w.cn

Object.groupBy(arr, x => x.type)
来源：http://pyr.jinyuanbaomall.cn

[U110] JS：数组分块
来源：http://txq.sweek.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://cnp.9152youxi.cn


<!-- 参考信息 -->