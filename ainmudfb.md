代发 wailian999

[T37] Lua：字符串拼接
来源：http://dil.gogol.net.cn

"a" .. "b"
来源：http://nkt.316326.xyz

[T38] Lua：条件
来源：http://lbo.daria6918.cn

if x > 0 then print("正") end
来源：http://vuo.yuanzhike.top

[T39] Lua：模式匹配
来源：http://oqd.hammf.cn

string.find(s, "%d+")
来源：http://unf.smart0.xyz

[T40] Lua：元表
来源：http://gin.xziqi.cn

setmetatable({}, { __index = base })
来源：http://ktc.pengpengdd.cyou

[T41] Perl：Hello World
来源：http://kgn.sysykeji.top

print "Hello\n";
来源：http://cef.hammf.cn

[T42] Perl：变量类型
来源：http://lwq.cashguo.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://xup.fanxiaobao.xyz

[T43] Perl：字符串插值
来源：http://bsp.yfazqb.com

"值: $a"
来源：http://lhv.fzhhl.top

[T44] Perl：条件
来源：http://pkc.wangshuangyany.cn

if ($a > 0) { print "正"; }
来源：http://qpb.jinqigfzy.top

[T45] Perl：数组遍历
来源：http://sdu.epnwcf.com

for my $x (@arr) { print $x; }
来源：http://xuj.c1oappe.top

[T46] Perl：哈希操作
来源：http://uxl.daxiang520.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://spu.nwbrower.top

[T47] Perl：正则捕获
来源：http://txq.cheryme.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://wbl.ydzc1.top

[T48] Perl：正则替换
来源：http://dqh.kuanghao11.cn

$s =~ s/old/new/g;
来源：http://jyq.chenjidiqi.icu

[T49] Perl：函数
来源：http://cxo.jqgufenzy.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hfj.ehwqpu.com

[T50] Perl：逐行读文件
来源：http://myu.shangyingyoupin.top

open my $fh, "<", "a.txt" or die $!;
来源：http://pia.cheryme.top

while (my $line = <$fh>) { print $line; }
来源：http://axm.birdmap.top

[T51] Scala：Hello World
来源：http://vkv.fanxiaobao.xyz

println("Hello")
来源：http://eds.daria6918.cn

[T52] Scala：变量
来源：http://odi.zhongyouzk.top

val a = 1;  var b = 2
来源：http://qdv.zhixingplan.top

[T53] Scala：字符串插值
来源：http://bxu.bbcook.cn

s"值: $b"
来源：http://zdx.ivvv.top

[T54] Scala：集合映射
来源：http://eix.xuetiantiany.cn

List(1, 2, 3).map(_ * 2)
来源：http://pkh.yanxiufei.cn

[T55] Scala：集合过滤
来源：http://gfa.zycfv.cn

List(1, 2, 3).filter(_ > 1)
来源：http://wkh.shangyingyoupin.top

[T56] Scala：样例类
来源：http://czt.aizwys.cn

case class User(name: String, age: Int)
来源：http://syp.sxryk.cn

[T57] Scala：模式匹配
来源：http://jon.jiagoushi.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://gkz.fzhhl.top

[T58] Scala：函数定义
来源：http://fib.yj20258888.top

def add(a: Int, b: Int): Int = a + b
来源：http://ptl.ybcxt.top

[T59] Scala：循环
来源：http://qbk.hesvh.cn

for (i <- 1 to 10) println(i)
来源：http://osn.jqgufenzy.top

[T60] Scala：折叠
来源：http://qyl.gaohongyu789.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://ghq.yj202588.top

================================================================================
来源：http://nfq.zdbjq.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://gth.aibaodan.cn

================================================================================
来源：http://ehk.shanyushiyangkeji.top

[U01] Py：创建虚拟环境
来源：http://yuh.jyoumei.cn

python -m venv .venv && source .venv/bin/activate
来源：http://yfs.gaohongyu789.top

[U02] Py：导出 / 安装依赖
来源：http://yvd.wangshuangyany.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://ncq.quarkkingdee.top

[U03] Py：加载 .env 配置
来源：http://nir.zhiwuduotai.top

from dotenv import load_dotenv; load_dotenv()
来源：http://ifv.pycfn.com

[U04] Py：变量调试打印
来源：http://yhu.tian-w.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://xto.zhongyouzk.top

[U05] Py：列表去重且保序
来源：http://nff.0kj1m.cn

list(dict.fromkeys(arr))
来源：http://nkv.hammf.cn

[U06] Py：合并两个字典
来源：http://qbj.c1oappe.top

{**a, **b}
来源：http://mmq.hnxiangtu.top

[U07] Py：反转字典键值
来源：http://ldt.jqgfzy.top

{v: k for k, v in d.items()}
来源：http://aly.cucudq.cn

[U08] Py：展平二维列表
来源：http://acd.jinyuanbaomall.cn

[y for x in nested for y in x]
来源：http://ank.sxryk.cn

[U09] Py：字典取最大值的键
来源：http://ari.shanyushiyangkeji.top

max(d, key=d.get)
来源：http://clg.cucudq.cn

[U10] Py：按值排序字典
来源：http://izc.pengpengdd.cyou

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://zvh.pycfn.com

[U11] Py：生成器表达式
来源：http://ppo.dianchejie.cn

(x * 2 for x in arr)
来源：http://jiy.52xcode.cn

[U12] Py：取出现最多的 3 个元素
来源：http://zaq.haohaochexian.top

Counter(arr).most_common(3)
来源：http://fzi.zhixingplan.top

[U13] Py：固定长度队列
来源：http://gqc.jqgufenzy.top

deque(maxlen=10)
来源：http://mhm.shanyushiyangkeji.top

[U14] Py：分组收集到列表
来源：http://txi.vqdsnc.cn

defaultdict(list)
来源：http://lgp.ydzc1.top

[U15] Py：高精度计时
来源：http://bpc.guowangkeji.top

t = time.perf_counter()
来源：http://fde.iojbl.cn

[U16] Py：命令行参数解析
来源：http://fdh.yfazqb.com

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://uev.feifeiyinyue.top

[U17] Py：初始化日志
来源：http://nsz.316326.xyz

logging.basicConfig(level=logging.INFO)
来源：http://ruq.snrcjt.cn

[U18] Py：预编译正则
来源：http://ziu.epnwcf.com

pat = re.compile(r"\d+")
来源：http://xvi.yonumen.top

[U19] Py：正则替换带回调
来源：http://hjg.snrcjt.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://pij.zhongyouzk.top

[U20] Py：缓存函数结果
来源：http://qcb.yvedp.cn

@functools.lru_cache(maxsize=None)
来源：http://zcu.yj20258.top

[U21] Py：自定义上下文管理器
来源：http://tqi.wangdashe.top

@contextlib.contextmanager
来源：http://mfe.9152youxi.cn

[U22] Py：矩阵转置
来源：http://cwr.snrcjt.cn

list(zip(*m))
来源：http://tga.jiagoushi.top

[U23] Py：分块读取大文件
来源：http://znv.jyoumei.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://ngp.yj20258888.top

[U24] Py：路径操作
来源：http://wqw.xziqi.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://izf.ppjwa.cn

[U25] Py：CSV 按字典读
来源：http://aao.jiagoushi.top

csv.DictReader(f)
来源：http://dxl.ppjwa.cn

[U26] Py：并发下载
来源：http://zaq.yj202588.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://zvd.cqqwz.cn

[U27] Py：异步 HTTP
来源：http://dpn.hammf.cn

aiohttp.ClientSession() 配合 async with
来源：http://ixc.epnwcf.com

[U28] Py：类型别名
来源：http://bwz.tian-w.cn

UserId = int
来源：http://pql.vqdsnc.cn

[U29] Py：属性校验
来源：http://jko.aibaodan.cn

@property 与 @x.setter 配合
来源：http://uhh.hesvh.cn

[U30] Py：数据类
来源：http://dog.meibo888.top

@dataclass(slots=True)
来源：http://nfg.jinqigufen.top

[U31] Py：单测
来源：http://les.zhengqikj.top

python -m pytest -q
来源：http://pgy.ivvv.top

[U32] Py：代码格式化
来源：http://dgh.xuetiantiany.cn

ruff format . && ruff check --fix .
来源：http://qdo.sweek.top

[U33] Py：打包发布
来源：http://koh.dianchejie.cn

python -m build  （依赖 pyproject.toml）
来源：http://cdq.shuidangran.top

[U34] Py：判断编码
来源：http://ntl.xuanzx.com

chardet.detect(raw)
来源：http://vzr.feifeiyinyue.top

[U35] Py：发送邮件
来源：http://eae.zdbjq.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://iay.yonumen.top

[U36] Py：定时任务
来源：http://wpc.yonumen.top

schedule.every(10).minutes.do(job)
来源：http://yeb.yueranfly.top

[U37] Py：读写 Excel
来源：http://oyb.yfazqb.com

pandas.read_excel / DataFrame.to_excel
来源：http://jyz.yuxming.cn

[U38] Py：获取脚本所在目录
来源：http://xpv.jinqigfzy.top

Path(__file__).resolve().parent
来源：http://xss.jqgfzy.top

[U39] Py：判断是否在交互环境
来源：http://xbm.hfpthk.cn

sys.stdout.isatty()
来源：http://ogz.quarkkingdee.top

[U40] Py：打印到标准错误
来源：http://wwi.aizwys.cn

print("err", file=sys.stderr)
来源：http://rmv.fengsongda.top

[U41] PHP：初始化 Composer 项目
来源：http://isu.pycfn.com

composer init;  composer require guzzlehttp/guzzle
来源：http://zyc.gaohongyu789.top

[U42] PHP：PSR-4 自动加载
来源：http://plk.chenjidiqi.icu

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://lpm.xylfe.cn

[U43] PHP：声明命名空间
来源：http://isl.daxiang520.top

namespace App\Http;
来源：http://otn.shuidangran.top

[U44] PHP：开启严格类型
来源：http://hep.zhaomingkeji.xyz

declare(strict_types=1);
来源：http://ydv.yuanzhike.top

[U45] PHP：类型声明与返回类型
来源：http://ipq.fktsv.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://rxo.hongshengwenyu.top

[U46] PHP：可空类型
来源：http://iji.shuidangran.top

?string $name = null
来源：http://oiu.hesvh.cn

[U47] PHP：联合类型
来源：http://evb.yonumen.top

int|string $id
来源：http://udn.ctjpmb.com

[U48] PHP：纯枚举
来源：http://qah.fktsv.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://tnz.sysykeji.top

[U49] PHP：只读属性
来源：http://zcs.yvedp.cn

public readonly string $name
来源：http://viz.pycfn.com

[U50] PHP：构造器属性提升
来源：http://klj.vehdjk.com

public function __construct(private int $id) {}
来源：http://grw.cdnleiting.top

[U51] PHP：数组解构
来源：http://wgk.xuetiantiany.cn

[$a, $b] = $arr;
来源：http://qcm.tian-w.cn

[U52] PHP：箭头函数
来源：http://fqo.tianlin.xyz

$double = fn($x) => $x * 2;
来源：http://blp.wangdashe.top

[U53] PHP：空合并运算符
来源：http://qla.chenzaomai.com

$v = $a ?? $b ?? "default";
来源：http://lul.cheryme.top

[U54] PHP：空安全调用
来源：http://hvd.jiagoushi.top

$obj?->method()
来源：http://vih.hywenlv.cn

[U55] PHP：match 表达式
来源：http://ycn.daria6918.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hxl.vehdjk.com

[U56] PHP：命名参数
来源：http://nxq.jinqigufen.top

f(a: 1, b: 2)
来源：http://zig.iojbl.cn

[U57] PHP：字符串插值
来源：http://yid.zhaomingkeji.xyz

"值: {$a}"
来源：http://qcd.cheryme.top

[U58] PHP：数组三件套
来源：http://rpc.yj20258.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://nbo.fehbvm.com

[U59] PHP：自定义排序
来源：http://tkp.hesvh.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://zjm.chenzaomai.com

[U60] PHP：JSON 编解码
来源：http://xyq.yuanzhike.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://dvu.0kj1m.cn

[U61] PHP：正则
来源：http://evm.yanxiufei.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://ohc.tianlin.xyz

[U62] PHP：日期对象
来源：http://rfn.jlsjyb.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://aou.guowangkeji.top

[U63] PHP：文件读写
来源：http://wbz.smart0.xyz

file_get_contents($f);  file_put_contents($f, $data);
来源：http://yfl.yonumen.top

[U64] PHP：目录遍历
来源：http://kyi.tian-w.cn

glob("dir/*.php");  scandir("dir");
来源：http://epm.jianghu66.top

[U65] PHP：会话
来源：http://jxg.gaohongyu789.top

session_start();  $_SESSION["uid"] = 1;
来源：http://jjt.guannengcc.top

[U66] PHP：设置 Cookie
来源：http://aib.zhongyouzk.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://cgp.dianchejie.cn

[U67] PHP：处理文件上传
来源：http://hkh.havefunace.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://tea.zhijiandao.cn

[U68] PHP：PDO 连接
来源：http://svm.yvedp.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://bew.bjfxy.top

[U69] PHP：PDO 预处理
来源：http://huu.epnwcf.com

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://iay.yvedp.cn

[U70] PHP：PDO 事务
来源：http://sdi.xuetiantiany.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://dac.andypj.xyz

[U71] PHP：抛出异常
来源：http://nrp.yueranfly.top

throw new RuntimeException("失败", 500);
来源：http://rkk.aibaodan.cn

[U72] PHP：写错误日志
来源：http://znf.sjlbkw.cn

error_log("失败: " . $e->getMessage());
来源：http://acp.cdnleiting.top

[U73] PHP：读取 ini 配置
来源：http://lmr.yuxming.cn

parse_ini_file("config.ini", true)
来源：http://sqo.mhx1999.top

[U74] PHP：读取环境变量
来源：http://xui.andypj.xyz

getenv("APP_ENV") ?: "production"
来源：http://azv.daxiang520.top

[U75] PHP：依赖注入
来源：http://kna.haohaochexian.top

composer require psr/container
来源：http://mxx.jyoumei.cn

[U76] PHP：简单路由
来源：http://yhk.birdmap.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://ejz.hcnkem.com

[U77] PHP：模板渲染
来源：http://ige.mhx1999.top

composer require twig/twig
来源：http://qwf.svipenyu.cn

[U78] PHP：单元测试
来源：http://nlv.jqgfzy.top

composer require --dev phpunit/phpunit
来源：http://otx.guannengcc.top

[U79] PHP：静态分析
来源：http://peb.jinyuanbaomall.cn

composer require --dev phpstan/phpstan
来源：http://kfm.yangfankeji.com

[U80] PHP：代码规范修复
来源：http://znf.jinqigufen.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://rfl.xuanzx.com

[U81] JS：初始化项目
来源：http://pbo.daria6918.cn

npm init -y;  npm i express
来源：http://mte.gzhubu.top

[U82] JS：package.json 脚本
来源：http://dse.cashguo.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://yzb.ydzc1.top

[U83] JS：ES Module 导入导出
来源：http://oxa.yj20258888.top

export const a = 1;  import { a } from "./m.js";
来源：http://mhk.xuanzx.com

[U84] JS：CommonJS 写法
来源：http://pfn.dianchejie.cn

module.exports = { a };  const { a } = require("./m");
来源：http://zjq.9152youxi.cn

[U85] JS：可选链
来源：http://ksc.shanyushiyangtech.top

a?.b?.c
来源：http://rvp.chenlongwang.top

[U86] JS：空值合并
来源：http://gpx.dianchejie.cn

a ?? b
来源：http://dmu.fehbvm.com

[U87] JS：解构默认值
来源：http://wpd.shuidangran.top

const { a = 1, b = 2 } = obj;
来源：http://nkr.52xcode.cn

[U88] JS：对象展开合并
来源：http://bsn.jyoumei.cn

{ ...a, ...b }
来源：http://nev.nanxinkj.top

[U89] JS：数组去重
来源：http://vsm.fanxiaobao.xyz

[...new Set(arr)]
来源：http://swy.hammf.cn

[U90] JS：数字数组排序
来源：http://qas.quarkkingdee.top

[...arr].sort((a, b) => a - b)
来源：http://vmq.hammf.cn

[U91] JS：对象键值遍历
来源：http://hzq.sysykeji.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://fhr.uphjek.com

[U92] JS：深拷贝
来源：http://dgh.daxiang520.top

structuredClone(obj)
来源：http://wop.hywenlv.cn

[U93] JS：模板字符串
来源：http://jvk.gzhubu.top

`共 ${n} 条`
来源：http://ygj.jinghuilouyu.cn

[U94] JS：箭头函数
来源：http://qoo.jiagoushi.top

const double = x => x * 2;
来源：http://vdl.fktsv.cn

[U95] JS：Promise 包装
来源：http://mye.bbcook.cn

new Promise((resolve, reject) => {})
来源：http://pcn.gotoacloud.top

[U96] JS：async/await 与异常
来源：http://enn.yvedp.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://zrt.yuxming.cn

[U97] JS：并发请求
来源：http://cew.zhiwuduotai.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://tua.fanxiaobao.xyz

[U98] JS：fetch 带 JSON
来源：http://ucb.ppjwa.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://ekk.ydjk.org.cn

[U99] JS：事件监听
来源：http://klu.chenjidiqi.icu

el.addEventListener("click", e => {})
来源：http://twz.yangfankeji.com

[U100] JS：DOM 查询
来源：http://pki.daria6918.cn

document.querySelector(".item")
来源：http://tzp.bbcook.cn

[U101] JS：classList 操作
来源：http://gzw.sxryk.cn

el.classList.toggle("active")
来源：http://gqo.yonumen.top

[U102] JS：本地存储
来源：http://shq.zhiwuduotai.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://ygm.guannengcc.top

[U103] JS：定时器
来源：http://owd.shangyingyoupin.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://ngi.cheryme.top

[U104] JS：防抖
来源：http://qsp.dashuyun.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://zyx.dashuyun.cn

[U105] JS：节流
来源：http://abs.316326.xyz

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://jrd.kuanghao11.cn

[U106] JS：日期格式化
来源：http://hzd.9152youxi.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://zcz.hnqzz.top

[U107] JS：数字千分位
来源：http://cqr.sufxvd.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://gmx.cashguo.top

[U108] JS：随机整数
来源：http://asz.tianlin.xyz

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://sdr.tianlin.xyz

[U109] JS：数组分组
来源：http://vrp.havefunace.top

Object.groupBy(arr, x => x.type)
来源：http://auv.jiagoushi.top

[U110] JS：数组分块
来源：http://ubv.xingfuxueyuan.xyz

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://erk.xingfuxueyuan.xyz

[U111] JS：对象转 Map
来源：http://alr.sxryk.cn

new Map(Object.entries(obj))
来源：http://irp.jqgufenzy.top

[U112] JS：字符串补位
来源：http://vqm.yfazqb.com

"7".padStart(3, "0")
来源：http://jcc.kuanghao11.cn

[U113] JS：正则替换全部
来源：http://kfz.gogol.net.cn

s.replaceAll("a", "b")
来源：http://gly.yangfankeji.com

[U114] JS：JSON 深比较
来源：http://rgf.wangshuangyany.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://zfx.zhoulong.xyz

[U115] JS：生成 UUID
来源：http://pzj.yuxming.cn

crypto.randomUUID()
来源：http://ixg.9152youxi.cn

[U116] JS：类型检查（JSDoc）
来源：http://cdn.birdmap.top

/** @param {string} name */ function f(name) {}
来源：http://oui.snrcjt.cn

[U117] JS：单元测试
来源：http://qnx.gogol.net.cn

npm i -D vitest;  npx vitest
来源：http://ibu.cqqwz.cn

[U118] JS：开发服务器
来源：http://dpp.mhx1999.top

npm i -D vite;  npx vite
来源：http://dei.shuidangran.top

[U119] JS：生产构建
来源：http://yay.chenjidiqi.icu

npx vite build
来源：http://ajx.epnwcf.com

[U120] JS：读取环境变量（Vite）
来源：http://cij.sweek.top

import.meta.env.VITE_API_URL
来源：http://jva.9152youxi.cn

================================================================================
来源：http://zcn.gogol.net.cn

统计汇总
来源：http://qrp.jinghuilouyu.cn

================================================================================
来源：http://wvy.bjfxy.top

按语言统计（条）：
来源：http://pec.jqgfzy.top

Python ......... 252
来源：http://ygz.hnqzz.top

PHP ............ 252
来源：http://oei.gogol.net.cn

JavaScript ..... 252
来源：http://hlx.zhaomingkeji.xyz

TypeScript ..... 212
来源：http://qdm.ppjwa.cn


<!-- 参考信息 -->