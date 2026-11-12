代发 wailian999

[T35] Lua：字典表
来源：http://xrj.iojbl.cn

local d = { a = 1 };  d.b = 2
来源：http://ifb.c1oappe.top

[T36] Lua：函数
来源：http://xxy.yuxming.cn

function add(a, b) return a + b end
来源：http://zux.bjfxy.top

[T37] Lua：字符串拼接
来源：http://xbf.tarul.cn

"a" .. "b"
来源：http://vqb.yfazqb.com

[T38] Lua：条件
来源：http://spp.mhx1999.top

if x > 0 then print("正") end
来源：http://flx.smart0.xyz

[T39] Lua：模式匹配
来源：http://ohs.hesvh.cn

string.find(s, "%d+")
来源：http://rxe.cheryme.top

[T40] Lua：元表
来源：http://dyn.zhengqikj.top

setmetatable({}, { __index = base })
来源：http://hip.shanyushiyangtech.top

[T41] Perl：Hello World
来源：http://ehu.yfazqb.com

print "Hello\n";
来源：http://hks.hammf.cn

[T42] Perl：变量类型
来源：http://chr.sweek.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://twq.xuanzx.com

[T43] Perl：字符串插值
来源：http://pks.sufxvd.cn

"值: $a"
来源：http://ste.shanyushiyangtech.top

[T44] Perl：条件
来源：http://gzc.yonumen.top

if ($a > 0) { print "正"; }
来源：http://wcv.jinqigfzy.top

[T45] Perl：数组遍历
来源：http://ove.havefunace.top

for my $x (@arr) { print $x; }
来源：http://ogq.hywenlv.cn

[T46] Perl：哈希操作
来源：http://nhw.zhijiandao.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://xjj.nwbrower.top

[T47] Perl：正则捕获
来源：http://jqz.bjfxy.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://ouu.ydzc1.top

[T48] Perl：正则替换
来源：http://bns.hammf.cn

$s =~ s/old/new/g;
来源：http://zof.bjfxy.top

[T49] Perl：函数
来源：http://peo.andypj.xyz

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://xfn.cqqwz.cn

[T50] Perl：逐行读文件
来源：http://asx.yj20258888.top

open my $fh, "<", "a.txt" or die $!;
来源：http://jjt.jinqigufen.top

while (my $line = <$fh>) { print $line; }
来源：http://hti.jyoumei.cn

[T51] Scala：Hello World
来源：http://gij.zhengqikj.top

println("Hello")
来源：http://fms.mhx1999.top

[T52] Scala：变量
来源：http://lbo.shuidangran.top

val a = 1;  var b = 2
来源：http://igk.dianchejie.cn

[T53] Scala：字符串插值
来源：http://ohp.daxiang520.top

s"值: $b"
来源：http://teu.jiagoushi.top

[T54] Scala：集合映射
来源：http://wxz.hammf.cn

List(1, 2, 3).map(_ * 2)
来源：http://wck.daxiang520.top

[T55] Scala：集合过滤
来源：http://nnr.cqqwz.cn

List(1, 2, 3).filter(_ > 1)
来源：http://kac.pycfn.com

[T56] Scala：样例类
来源：http://bpk.kuanghao11.cn

case class User(name: String, age: Int)
来源：http://xns.shanyushiyangtech.top

[T57] Scala：模式匹配
来源：http://ltn.gogol.net.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://zny.52xcode.cn

[T58] Scala：函数定义
来源：http://gps.jyoumei.cn

def add(a: Int, b: Int): Int = a + b
来源：http://gbt.pengpengdd.cyou

[T59] Scala：循环
来源：http://xhz.xuanzx.com

for (i <- 1 to 10) println(i)
来源：http://vzz.jiagoushi.top

[T60] Scala：折叠
来源：http://tgt.wangshuangyany.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://rin.iojbl.cn

================================================================================
来源：http://wbn.yj20258888.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://kti.feifeiyinyue.top

================================================================================
来源：http://qwe.haohaochexian.top

[U01] Py：创建虚拟环境
来源：http://xfz.cqqwz.cn

python -m venv .venv && source .venv/bin/activate
来源：http://nwq.fzhhl.top

[U02] Py：导出 / 安装依赖
来源：http://pni.hfpthk.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://dnf.zhongyouzk.top

[U03] Py：加载 .env 配置
来源：http://ftt.redwolf501.top

from dotenv import load_dotenv; load_dotenv()
来源：http://onr.kuanghao11.cn

[U04] Py：变量调试打印
来源：http://fjw.yj20258888.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://wav.dianchejie.cn

[U05] Py：列表去重且保序
来源：http://ima.jlsjyb.cn

list(dict.fromkeys(arr))
来源：http://xma.nanxinkj.top

[U06] Py：合并两个字典
来源：http://ebs.chenzaomai.com

{**a, **b}
来源：http://cik.xuetiantiany.cn

[U07] Py：反转字典键值
来源：http://hnu.nanxinkj.top

{v: k for k, v in d.items()}
来源：http://tag.zhixingplan.top

[U08] Py：展平二维列表
来源：http://jqu.chenzaomai.com

[y for x in nested for y in x]
来源：http://fwb.iojbl.cn

[U09] Py：字典取最大值的键
来源：http://psc.hcnkem.com

max(d, key=d.get)
来源：http://qtb.gogol.net.cn

[U10] Py：按值排序字典
来源：http://obj.haohaochexian.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://eqd.xinyue.icu

[U11] Py：生成器表达式
来源：http://fgv.tian-w.cn

(x * 2 for x in arr)
来源：http://egq.bjfxy.top

[U12] Py：取出现最多的 3 个元素
来源：http://uet.guowangkeji.top

Counter(arr).most_common(3)
来源：http://eda.bjfxy.top

[U13] Py：固定长度队列
来源：http://ioe.andypj.xyz

deque(maxlen=10)
来源：http://hae.hcnkem.com

[U14] Py：分组收集到列表
来源：http://csa.jianghu66.top

defaultdict(list)
来源：http://eme.hnqzz.top

[U15] Py：高精度计时
来源：http://gpn.zhengqikj.top

t = time.perf_counter()
来源：http://rkd.xylfe.cn

[U16] Py：命令行参数解析
来源：http://hod.yj20258888.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://vhr.tarul.cn

[U17] Py：初始化日志
来源：http://nlp.gotoacloud.top

logging.basicConfig(level=logging.INFO)
来源：http://kyz.zhaomingkeji.xyz

[U18] Py：预编译正则
来源：http://afs.snrcjt.cn

pat = re.compile(r"\d+")
来源：http://yaf.yueranfly.top

[U19] Py：正则替换带回调
来源：http://psb.svipenyu.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://cpz.yangfankeji.com

[U20] Py：缓存函数结果
来源：http://zxg.xingfuxueyuan.xyz

@functools.lru_cache(maxsize=None)
来源：http://edu.0kj1m.cn

[U21] Py：自定义上下文管理器
来源：http://xsq.yvedp.cn

@contextlib.contextmanager
来源：http://cyx.zycfv.cn

[U22] Py：矩阵转置
来源：http://zli.sufxvd.cn

list(zip(*m))
来源：http://ayb.jlsjyb.cn

[U23] Py：分块读取大文件
来源：http://uxa.cqqwz.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://max.jqgufenzy.top

[U24] Py：路径操作
来源：http://jvq.jyoumei.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://nww.xuanzx.com

[U25] Py：CSV 按字典读
来源：http://ykd.chenlongwang.top

csv.DictReader(f)
来源：http://mtj.nwbrower.top

[U26] Py：并发下载
来源：http://hjt.sweek.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://ixc.vehdjk.com

[U27] Py：异步 HTTP
来源：http://edk.hongshengwenyu.top

aiohttp.ClientSession() 配合 async with
来源：http://hpp.shuidangran.top

[U28] Py：类型别名
来源：http://jje.hcnkem.com

UserId = int
来源：http://dex.guowangkeji.top

[U29] Py：属性校验
来源：http://ruy.yj202588.top

@property 与 @x.setter 配合
来源：http://sjc.shuidangran.top

[U30] Py：数据类
来源：http://gbw.shangyingyoupin.top

@dataclass(slots=True)
来源：http://trf.bbcook.cn

[U31] Py：单测
来源：http://cjf.kuanghao11.cn

python -m pytest -q
来源：http://fwq.sxryk.cn

[U32] Py：代码格式化
来源：http://ocs.gaohongyu789.top

ruff format . && ruff check --fix .
来源：http://ieg.zhixingplan.top

[U33] Py：打包发布
来源：http://pfs.daria6918.cn

python -m build  （依赖 pyproject.toml）
来源：http://gsa.shuidangran.top

[U34] Py：判断编码
来源：http://dod.xinyue.icu

chardet.detect(raw)
来源：http://pzu.yanxiufei.cn

[U35] Py：发送邮件
来源：http://man.xylfe.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://jxz.yongpay.top

[U36] Py：定时任务
来源：http://kuu.gaohongyu789.top

schedule.every(10).minutes.do(job)
来源：http://dmk.yuanzhike.top

[U37] Py：读写 Excel
来源：http://bbe.0kj1m.cn

pandas.read_excel / DataFrame.to_excel
来源：http://qup.vehdjk.com

[U38] Py：获取脚本所在目录
来源：http://lyz.hammf.cn

Path(__file__).resolve().parent
来源：http://xjj.smart0.xyz

[U39] Py：判断是否在交互环境
来源：http://ozo.yonumen.top

sys.stdout.isatty()
来源：http://cst.xuetiantiany.cn

[U40] Py：打印到标准错误
来源：http://mtd.aibaodan.cn

print("err", file=sys.stderr)
来源：http://xld.jinyuanbaomall.cn

[U41] PHP：初始化 Composer 项目
来源：http://izb.dashuyun.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://wmn.pengpengdd.cyou

[U42] PHP：PSR-4 自动加载
来源：http://pzv.hfpthk.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://vte.yvedp.cn

[U43] PHP：声明命名空间
来源：http://qxd.jinqigufen.top

namespace App\Http;
来源：http://nwh.cheryme.top

[U44] PHP：开启严格类型
来源：http://ypo.jinqigufen.top

declare(strict_types=1);
来源：http://drn.xuetiantiany.cn

[U45] PHP：类型声明与返回类型
来源：http://dzz.snrcjt.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://zuj.shuidangran.top

[U46] PHP：可空类型
来源：http://dgo.nwbrower.top

?string $name = null
来源：http://bex.wangdashe.top

[U47] PHP：联合类型
来源：http://lnh.cucudq.cn

int|string $id
来源：http://iir.yangfankeji.com

[U48] PHP：纯枚举
来源：http://atz.ydjk.org.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://deb.zhengqikj.top

[U49] PHP：只读属性
来源：http://qaf.yvedp.cn

public readonly string $name
来源：http://aca.sxryk.cn

[U50] PHP：构造器属性提升
来源：http://ile.uphjek.com

public function __construct(private int $id) {}
来源：http://wfu.jlsjyb.cn

[U51] PHP：数组解构
来源：http://lwx.yangfankeji.com

[$a, $b] = $arr;
来源：http://qxq.cdnleiting.top

[U52] PHP：箭头函数
来源：http://qkv.aizwys.cn

$double = fn($x) => $x * 2;
来源：http://zmg.hongshengwenyu.top

[U53] PHP：空合并运算符
来源：http://dvb.ydzc1.top

$v = $a ?? $b ?? "default";
来源：http://nsx.sweek.top

[U54] PHP：空安全调用
来源：http://jzp.yangfankeji.com

$obj?->method()
来源：http://efz.feifeiyinyue.top

[U55] PHP：match 表达式
来源：http://uyp.pycfn.com

$s = match($x) { 1 => "一", default => "其他" };
来源：http://ywm.birdmap.top

[U56] PHP：命名参数
来源：http://gkl.cheryme.top

f(a: 1, b: 2)
来源：http://fin.xinyue.icu

[U57] PHP：字符串插值
来源：http://hnv.hcnkem.com

"值: {$a}"
来源：http://ffm.feifeiyinyue.top

[U58] PHP：数组三件套
来源：http://lmb.havefunace.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://yuw.cashguo.top

[U59] PHP：自定义排序
来源：http://pcg.zdbjq.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://rva.aizwys.cn

[U60] PHP：JSON 编解码
来源：http://pgl.daria6918.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://nqi.birdmap.top

[U61] PHP：正则
来源：http://qxz.cqqwz.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hvm.zdbjq.cn

[U62] PHP：日期对象
来源：http://qcd.9152youxi.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://ptp.nwbrower.top

[U63] PHP：文件读写
来源：http://rrq.fzhhl.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://ipt.xuanzx.com

[U64] PHP：目录遍历
来源：http://rad.chenlongwang.top

glob("dir/*.php");  scandir("dir");
来源：http://shn.yongpay.top

[U65] PHP：会话
来源：http://gyt.hnxiangtu.top

session_start();  $_SESSION["uid"] = 1;
来源：http://vuy.shangyingyoupin.top

[U66] PHP：设置 Cookie
来源：http://aci.52xcode.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://wnc.sysykeji.top

[U67] PHP：处理文件上传
来源：http://fzz.wangshuangyany.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://xml.hnxiangtu.top

[U68] PHP：PDO 连接
来源：http://pyg.pycfn.com

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hpd.cashguo.top

[U69] PHP：PDO 预处理
来源：http://xxj.jinqigufen.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://dav.ybcxt.top

[U70] PHP：PDO 事务
来源：http://ncd.gogol.net.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://uxg.xinyue.icu

[U71] PHP：抛出异常
来源：http://usv.jlsjyb.cn

throw new RuntimeException("失败", 500);
来源：http://jur.shanyushiyangkeji.top

[U72] PHP：写错误日志
来源：http://lyr.hfpthk.cn

error_log("失败: " . $e->getMessage());
来源：http://lpp.tianlin.xyz

[U73] PHP：读取 ini 配置
来源：http://bvv.cucudq.cn

parse_ini_file("config.ini", true)
来源：http://pyf.chenzaomai.com

[U74] PHP：读取环境变量
来源：http://bcl.zhengqikj.top

getenv("APP_ENV") ?: "production"
来源：http://kmj.fengsongda.top

[U75] PHP：依赖注入
来源：http://eln.jqgfzy.top

composer require psr/container
来源：http://yxw.zhoulong.xyz

[U76] PHP：简单路由
来源：http://aza.c1oappe.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://mfe.jinqigufen.top

[U77] PHP：模板渲染
来源：http://gnl.bbcook.cn

composer require twig/twig
来源：http://rzj.ctjpmb.com

[U78] PHP：单元测试
来源：http://fdm.ehwqpu.com

composer require --dev phpunit/phpunit
来源：http://ayc.hongshengwenyu.top

[U79] PHP：静态分析
来源：http://aky.jinghuilouyu.cn

composer require --dev phpstan/phpstan
来源：http://xmn.hfpthk.cn

[U80] PHP：代码规范修复
来源：http://oqt.chenjidiqi.icu

composer require --dev friendsofphp/php-cs-fixer
来源：http://zpk.52xcode.cn

[U81] JS：初始化项目
来源：http://igt.shzxlz.cn

npm init -y;  npm i express
来源：http://ckd.hywenlv.cn

[U82] JS：package.json 脚本
来源：http://mzr.jinqigfzy.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://ovp.aibaodan.cn

[U83] JS：ES Module 导入导出
来源：http://qay.andypj.xyz

export const a = 1;  import { a } from "./m.js";
来源：http://yqp.gaohongyu789.top

[U84] JS：CommonJS 写法
来源：http://tvv.0kj1m.cn

module.exports = { a };  const { a } = require("./m");
来源：http://cia.zhaomingkeji.xyz

[U85] JS：可选链
来源：http://hzc.xziqi.cn

a?.b?.c
来源：http://gxe.jqgufenzy.top

[U86] JS：空值合并
来源：http://hjl.meibo888.top

a ?? b
来源：http://btv.gaohongyu789.top

[U87] JS：解构默认值
来源：http://jhk.ywan-chungtsiang.top

const { a = 1, b = 2 } = obj;
来源：http://ucj.andypj.xyz

[U88] JS：对象展开合并
来源：http://iwv.jqgfzy.top

{ ...a, ...b }
来源：http://rmi.zhaomingkeji.xyz

[U89] JS：数组去重
来源：http://tfd.jinyuanbaomall.cn

[...new Set(arr)]
来源：http://clj.yfazqb.com

[U90] JS：数字数组排序
来源：http://ntx.cashguo.top

[...arr].sort((a, b) => a - b)
来源：http://qan.fanxiaobao.xyz

[U91] JS：对象键值遍历
来源：http://owc.sufxvd.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://nap.fengsongda.top

[U92] JS：深拷贝
来源：http://vhe.hongshengwenyu.top

structuredClone(obj)
来源：http://snu.jyoumei.cn

[U93] JS：模板字符串
来源：http://lnj.yvedp.cn

`共 ${n} 条`
来源：http://fan.hnqzz.top

[U94] JS：箭头函数
来源：http://ksm.9152youxi.cn

const double = x => x * 2;
来源：http://jkb.chenzaomai.com

[U95] JS：Promise 包装
来源：http://mjq.daria6918.cn

new Promise((resolve, reject) => {})
来源：http://kwq.mhx1999.top

[U96] JS：async/await 与异常
来源：http://iaj.ydzc1.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://yqf.zhoulong.xyz

[U97] JS：并发请求
来源：http://rhe.sufxvd.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://hmf.zhaomingkeji.xyz

[U98] JS：fetch 带 JSON
来源：http://yvn.yj20258.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://jun.fzhhl.top

[U99] JS：事件监听
来源：http://ntw.fzhhl.top

el.addEventListener("click", e => {})
来源：http://ywf.sufxvd.cn

[U100] JS：DOM 查询
来源：http://fid.andypj.xyz

document.querySelector(".item")
来源：http://rkm.havefunace.top

[U101] JS：classList 操作
来源：http://olh.haohaochexian.top

el.classList.toggle("active")
来源：http://mqy.xinyue.icu

[U102] JS：本地存储
来源：http://dtw.zhixingplan.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://wqv.zhoulong.xyz

[U103] JS：定时器
来源：http://odj.zdbjq.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://dtr.tanke756.top

[U104] JS：防抖
来源：http://cub.jlsjyb.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://lqq.chenzaomai.com

[U105] JS：节流
来源：http://mya.zycfv.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://gug.tarul.cn

[U106] JS：日期格式化
来源：http://ank.tarul.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://ijx.yj20258888.top

[U107] JS：数字千分位
来源：http://sas.vehdjk.com

new Intl.NumberFormat("en-US").format(1234567)
来源：http://ejw.tanke756.top

[U108] JS：随机整数
来源：http://zvy.chenjidiqi.icu

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://dma.zhixingplan.top

[U109] JS：数组分组
来源：http://egt.hysaishi.cn

Object.groupBy(arr, x => x.type)
来源：http://uak.ywan-chungtsiang.top

[U110] JS：数组分块
来源：http://kxe.xziqi.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://sov.zycfv.cn

[U111] JS：对象转 Map
来源：http://zke.pengpengdd.cyou

new Map(Object.entries(obj))
来源：http://fvg.vehdjk.com

[U112] JS：字符串补位
来源：http://ywr.jqgufenzy.top

"7".padStart(3, "0")
来源：http://oyk.c1oappe.top

[U113] JS：正则替换全部
来源：http://tdd.xinyue.icu

s.replaceAll("a", "b")
来源：http://gsn.snrcjt.cn

[U114] JS：JSON 深比较
来源：http://qig.jinqigufen.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://qxb.yvedp.cn

[U115] JS：生成 UUID
来源：http://ygv.hysaishi.cn

crypto.randomUUID()
来源：http://yac.hammf.cn

[U116] JS：类型检查（JSDoc）
来源：http://abq.svipenyu.cn

/** @param {string} name */ function f(name) {}
来源：http://azy.hnqzz.top

[U117] JS：单元测试
来源：http://qyn.sxryk.cn

npm i -D vitest;  npx vitest
来源：http://rxa.tanke756.top

[U118] JS：开发服务器
来源：http://exj.shangyingyoupin.top

npm i -D vite;  npx vite
来源：http://mze.zhongyouzk.top

[U119] JS：生产构建
来源：http://sba.0kj1m.cn

npx vite build
来源：http://hxo.c1oappe.top

[U120] JS：读取环境变量（Vite）
来源：http://dfm.hywenlv.cn

import.meta.env.VITE_API_URL
来源：http://kdf.fzhhl.top

================================================================================
来源：http://mhj.jlsjyb.cn

统计汇总
来源：http://iuw.0kj1m.cn

================================================================================
来源：http://wec.zycfv.cn

按语言统计（条）：
来源：http://rug.uphjek.com


<!-- 参考信息 -->