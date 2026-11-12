代发 wailian999

[T37] Lua：字符串拼接
来源：http://gew.dianchejie.cn

"a" .. "b"
来源：http://eeo.xuanzx.com

[T38] Lua：条件
来源：http://bwx.tianlin.xyz

if x > 0 then print("正") end
来源：http://vfo.xingfuxueyuan.xyz

[T39] Lua：模式匹配
来源：http://wyk.zhoulong.xyz

string.find(s, "%d+")
来源：http://yjg.fengsongda.top

[T40] Lua：元表
来源：http://fxd.mhx1999.top

setmetatable({}, { __index = base })
来源：http://txv.hfpthk.cn

[T41] Perl：Hello World
来源：http://pvy.hywenlv.cn

print "Hello\n";
来源：http://nmb.shzxlz.cn

[T42] Perl：变量类型
来源：http://oao.vqdsnc.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://oiq.dashuyun.cn

[T43] Perl：字符串插值
来源：http://goa.chenzaomai.com

"值: $a"
来源：http://bxh.yj20258888.top

[T44] Perl：条件
来源：http://tkd.52xcode.cn

if ($a > 0) { print "正"; }
来源：http://wht.jinghuilouyu.cn

[T45] Perl：数组遍历
来源：http://iwe.shuidangran.top

for my $x (@arr) { print $x; }
来源：http://qzm.gotoacloud.top

[T46] Perl：哈希操作
来源：http://fwj.havefunace.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://ary.mhx1999.top

[T47] Perl：正则捕获
来源：http://zbi.yonumen.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://ofp.havefunace.top

[T48] Perl：正则替换
来源：http://ihc.yj20258888.top

$s =~ s/old/new/g;
来源：http://lzw.sufxvd.cn

[T49] Perl：函数
来源：http://qtj.tianlin.xyz

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://tmn.guannengcc.top

[T50] Perl：逐行读文件
来源：http://vvp.cheryme.top

open my $fh, "<", "a.txt" or die $!;
来源：http://nty.nwbrower.top

while (my $line = <$fh>) { print $line; }
来源：http://kzk.sxryk.cn

[T51] Scala：Hello World
来源：http://oyj.hnxiangtu.top

println("Hello")
来源：http://yhs.hcnkem.com

[T52] Scala：变量
来源：http://flt.cucudq.cn

val a = 1;  var b = 2
来源：http://bqo.zhaomingkeji.xyz

[T53] Scala：字符串插值
来源：http://lyk.chenzaomai.com

s"值: $b"
来源：http://scc.snrcjt.cn

[T54] Scala：集合映射
来源：http://qsd.gogol.net.cn

List(1, 2, 3).map(_ * 2)
来源：http://vwu.shuidangran.top

[T55] Scala：集合过滤
来源：http://ggp.bjfxy.top

List(1, 2, 3).filter(_ > 1)
来源：http://chz.shanyushiyangtech.top

[T56] Scala：样例类
来源：http://ohx.sufxvd.cn

case class User(name: String, age: Int)
来源：http://woc.yuanzhike.top

[T57] Scala：模式匹配
来源：http://gpm.feifeiyinyue.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://ywb.uphjek.com

[T58] Scala：函数定义
来源：http://ssb.redwolf501.top

def add(a: Int, b: Int): Int = a + b
来源：http://iev.fehbvm.com

[T59] Scala：循环
来源：http://vvy.zhixingplan.top

for (i <- 1 to 10) println(i)
来源：http://yjy.feifeiyinyue.top

[T60] Scala：折叠
来源：http://omu.zycfv.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://uvd.gotoacloud.top

================================================================================
来源：http://anw.quarkkingdee.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://fjh.zhoulong.xyz

================================================================================
来源：http://djw.hammf.cn

[U01] Py：创建虚拟环境
来源：http://hma.yj202588.top

python -m venv .venv && source .venv/bin/activate
来源：http://joc.hysaishi.cn

[U02] Py：导出 / 安装依赖
来源：http://gyg.hnqzz.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://fck.gotoacloud.top

[U03] Py：加载 .env 配置
来源：http://btd.shzxlz.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://buf.jqgufenzy.top

[U04] Py：变量调试打印
来源：http://rdp.shanyushiyangkeji.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://prl.sjlbkw.cn

[U05] Py：列表去重且保序
来源：http://eqb.guannengcc.top

list(dict.fromkeys(arr))
来源：http://bxq.zhongyouzk.top

[U06] Py：合并两个字典
来源：http://xbf.tarul.cn

{**a, **b}
来源：http://ijn.redwolf501.top

[U07] Py：反转字典键值
来源：http://nlk.zhijiandao.cn

{v: k for k, v in d.items()}
来源：http://qfi.jiagoushi.top

[U08] Py：展平二维列表
来源：http://cxd.fehbvm.com

[y for x in nested for y in x]
来源：http://cfa.xuetiantiany.cn

[U09] Py：字典取最大值的键
来源：http://eby.chenzaomai.com

max(d, key=d.get)
来源：http://ppt.birdmap.top

[U10] Py：按值排序字典
来源：http://gdk.0kj1m.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://pkx.ehwqpu.com

[U11] Py：生成器表达式
来源：http://wki.bbcook.cn

(x * 2 for x in arr)
来源：http://boh.sxryk.cn

[U12] Py：取出现最多的 3 个元素
来源：http://zms.gogol.net.cn

Counter(arr).most_common(3)
来源：http://zjn.cdnleiting.top

[U13] Py：固定长度队列
来源：http://jsu.pycfn.com

deque(maxlen=10)
来源：http://uhs.ctjpmb.com

[U14] Py：分组收集到列表
来源：http://tls.gotoacloud.top

defaultdict(list)
来源：http://aok.shanyushiyangkeji.top

[U15] Py：高精度计时
来源：http://ovi.jinyuanbaomall.cn

t = time.perf_counter()
来源：http://bks.cashguo.top

[U16] Py：命令行参数解析
来源：http://zfx.aibaodan.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://mau.nanxinkj.top

[U17] Py：初始化日志
来源：http://hkw.zdbjq.cn

logging.basicConfig(level=logging.INFO)
来源：http://trj.ppjwa.cn

[U18] Py：预编译正则
来源：http://act.gotoacloud.top

pat = re.compile(r"\d+")
来源：http://ido.yanxiufei.cn

[U19] Py：正则替换带回调
来源：http://wwz.hnqzz.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://ret.yuxming.cn

[U20] Py：缓存函数结果
来源：http://ywy.yuanzhike.top

@functools.lru_cache(maxsize=None)
来源：http://juc.redwolf501.top

[U21] Py：自定义上下文管理器
来源：http://sxs.sweek.top

@contextlib.contextmanager
来源：http://hpr.cdnleiting.top

[U22] Py：矩阵转置
来源：http://ugn.jiagoushi.top

list(zip(*m))
来源：http://rje.tian-w.cn

[U23] Py：分块读取大文件
来源：http://viy.bjfxy.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://tdp.zdqjudy.top

[U24] Py：路径操作
来源：http://nsk.vehdjk.com

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://pus.ppjwa.cn

[U25] Py：CSV 按字典读
来源：http://ufp.jiagoushi.top

csv.DictReader(f)
来源：http://bzl.svipenyu.cn

[U26] Py：并发下载
来源：http://xiu.tanke756.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://lpk.quarkkingdee.top

[U27] Py：异步 HTTP
来源：http://qds.jinqigfzy.top

aiohttp.ClientSession() 配合 async with
来源：http://kdm.xuanzx.com

[U28] Py：类型别名
来源：http://vqy.zhoulong.xyz

UserId = int
来源：http://mwz.chenlongwang.top

[U29] Py：属性校验
来源：http://pwv.fehbvm.com

@property 与 @x.setter 配合
来源：http://lhy.shanyushiyangkeji.top

[U30] Py：数据类
来源：http://pck.fzhhl.top

@dataclass(slots=True)
来源：http://rpl.quarkkingdee.top

[U31] Py：单测
来源：http://ecd.yj20258888.top

python -m pytest -q
来源：http://mqy.yj20258888.top

[U32] Py：代码格式化
来源：http://xfl.guowangkeji.top

ruff format . && ruff check --fix .
来源：http://npu.xziqi.cn

[U33] Py：打包发布
来源：http://qqx.pycfn.com

python -m build  （依赖 pyproject.toml）
来源：http://mgh.jianghu66.top

[U34] Py：判断编码
来源：http://rxy.xuetiantiany.cn

chardet.detect(raw)
来源：http://jus.shzxlz.cn

[U35] Py：发送邮件
来源：http://ymo.iojbl.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://kfo.hywenlv.cn

[U36] Py：定时任务
来源：http://dnd.9152youxi.cn

schedule.every(10).minutes.do(job)
来源：http://jue.yangfankeji.com

[U37] Py：读写 Excel
来源：http://ltt.tian-w.cn

pandas.read_excel / DataFrame.to_excel
来源：http://ygf.wangshuangyany.cn

[U38] Py：获取脚本所在目录
来源：http://qij.vqdsnc.cn

Path(__file__).resolve().parent
来源：http://eam.haohaochexian.top

[U39] Py：判断是否在交互环境
来源：http://dvo.shzxlz.cn

sys.stdout.isatty()
来源：http://cpe.9152youxi.cn

[U40] Py：打印到标准错误
来源：http://ewl.hfpthk.cn

print("err", file=sys.stderr)
来源：http://pys.yj20258888.top

[U41] PHP：初始化 Composer 项目
来源：http://dpi.hywenlv.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://ssm.chenlongwang.top

[U42] PHP：PSR-4 自动加载
来源：http://hqe.jqgufenzy.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://sgh.jinyuanbaomall.cn

[U43] PHP：声明命名空间
来源：http://jpk.hywenlv.cn

namespace App\Http;
来源：http://mrj.yongpay.top

[U44] PHP：开启严格类型
来源：http://mwe.gaohongyu789.top

declare(strict_types=1);
来源：http://zio.ydzc1.top

[U45] PHP：类型声明与返回类型
来源：http://ylp.jiagoushi.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://apy.zhiwuduotai.top

[U46] PHP：可空类型
来源：http://inn.fanxiaobao.xyz

?string $name = null
来源：http://azf.nwbrower.top

[U47] PHP：联合类型
来源：http://npy.bjfxy.top

int|string $id
来源：http://hmb.daxiang520.top

[U48] PHP：纯枚举
来源：http://htt.hywenlv.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://svd.ctjpmb.com

[U49] PHP：只读属性
来源：http://axy.smart0.xyz

public readonly string $name
来源：http://pjh.tianlin.xyz

[U50] PHP：构造器属性提升
来源：http://qhr.tianlin.xyz

public function __construct(private int $id) {}
来源：http://iqf.zhiwuduotai.top

[U51] PHP：数组解构
来源：http://fnv.zdbjq.cn

[$a, $b] = $arr;
来源：http://hts.chenlongwang.top

[U52] PHP：箭头函数
来源：http://vkm.wangshuangyany.cn

$double = fn($x) => $x * 2;
来源：http://ync.gogol.net.cn

[U53] PHP：空合并运算符
来源：http://eyq.yanxiufei.cn

$v = $a ?? $b ?? "default";
来源：http://yhd.ivvv.top

[U54] PHP：空安全调用
来源：http://cns.gaohongyu789.top

$obj?->method()
来源：http://tos.fktsv.cn

[U55] PHP：match 表达式
来源：http://ogl.havefunace.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://sxk.pycfn.com

[U56] PHP：命名参数
来源：http://ome.fzhhl.top

f(a: 1, b: 2)
来源：http://ypi.ydjk.org.cn

[U57] PHP：字符串插值
来源：http://qtr.ywan-chungtsiang.top

"值: {$a}"
来源：http://yhe.shanyushiyangtech.top

[U58] PHP：数组三件套
来源：http://skc.xinyue.icu

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://xub.nwbrower.top

[U59] PHP：自定义排序
来源：http://sfa.guowangkeji.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://jwv.9152youxi.cn

[U60] PHP：JSON 编解码
来源：http://myb.shzxlz.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://pxp.xylfe.cn

[U61] PHP：正则
来源：http://hlc.xylfe.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://psr.sysykeji.top

[U62] PHP：日期对象
来源：http://tki.xylfe.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://jmb.yvedp.cn

[U63] PHP：文件读写
来源：http://nqw.sysykeji.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://pwq.sysykeji.top

[U64] PHP：目录遍历
来源：http://qrr.zhaomingkeji.xyz

glob("dir/*.php");  scandir("dir");
来源：http://hiu.cqqwz.cn

[U65] PHP：会话
来源：http://frr.bjfxy.top

session_start();  $_SESSION["uid"] = 1;
来源：http://uac.haohaochexian.top

[U66] PHP：设置 Cookie
来源：http://uuj.316326.xyz

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://mdk.shanyushiyangkeji.top

[U67] PHP：处理文件上传
来源：http://tuf.hammf.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://mll.sysykeji.top

[U68] PHP：PDO 连接
来源：http://tyn.0kj1m.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://xzp.tianlin.xyz

[U69] PHP：PDO 预处理
来源：http://ufu.yuanzhike.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://cwd.316326.xyz

[U70] PHP：PDO 事务
来源：http://bkw.ehwqpu.com

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://aky.fanxiaobao.xyz

[U71] PHP：抛出异常
来源：http://uzp.wangshuangyany.cn

throw new RuntimeException("失败", 500);
来源：http://ntg.zycfv.cn

[U72] PHP：写错误日志
来源：http://acr.birdmap.top

error_log("失败: " . $e->getMessage());
来源：http://clh.ivvv.top

[U73] PHP：读取 ini 配置
来源：http://vxy.hysaishi.cn

parse_ini_file("config.ini", true)
来源：http://fse.hesvh.cn

[U74] PHP：读取环境变量
来源：http://eyd.wangshuangyany.cn

getenv("APP_ENV") ?: "production"
来源：http://fqq.fehbvm.com

[U75] PHP：依赖注入
来源：http://btu.shangyingyoupin.top

composer require psr/container
来源：http://oem.yj202588.top

[U76] PHP：简单路由
来源：http://dyn.zhaomingkeji.xyz

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://tfl.bjfxy.top

[U77] PHP：模板渲染
来源：http://hos.9152youxi.cn

composer require twig/twig
来源：http://lca.wangshuangyany.cn

[U78] PHP：单元测试
来源：http://wzu.jianghu66.top

composer require --dev phpunit/phpunit
来源：http://qtb.jiagoushi.top

[U79] PHP：静态分析
来源：http://vbl.gzhubu.top

composer require --dev phpstan/phpstan
来源：http://thr.yueranfly.top

[U80] PHP：代码规范修复
来源：http://toz.pycfn.com

composer require --dev friendsofphp/php-cs-fixer
来源：http://hpo.hnqzz.top

[U81] JS：初始化项目
来源：http://ilx.yj202588.top

npm init -y;  npm i express
来源：http://ajr.kuanghao11.cn

[U82] JS：package.json 脚本
来源：http://dba.gzhubu.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://vzi.aibaodan.cn

[U83] JS：ES Module 导入导出
来源：http://wav.guannengcc.top

export const a = 1;  import { a } from "./m.js";
来源：http://scv.wangshuangyany.cn

[U84] JS：CommonJS 写法
来源：http://kbs.jqgfzy.top

module.exports = { a };  const { a } = require("./m");
来源：http://ifb.zhoulong.xyz

[U85] JS：可选链
来源：http://rql.cqqwz.cn

a?.b?.c
来源：http://neh.xuanzx.com

[U86] JS：空值合并
来源：http://xju.chenlongwang.top

a ?? b
来源：http://mxv.yj202588.top

[U87] JS：解构默认值
来源：http://paj.jqgfzy.top

const { a = 1, b = 2 } = obj;
来源：http://lsr.daria6918.cn

[U88] JS：对象展开合并
来源：http://lup.xingfuxueyuan.xyz

{ ...a, ...b }
来源：http://acr.jyoumei.cn

[U89] JS：数组去重
来源：http://iqu.ppjwa.cn

[...new Set(arr)]
来源：http://zsa.xziqi.cn

[U90] JS：数字数组排序
来源：http://jsk.ydjk.org.cn

[...arr].sort((a, b) => a - b)
来源：http://mdd.hfpthk.cn

[U91] JS：对象键值遍历
来源：http://ihl.zhaomingkeji.xyz

Object.entries(obj).forEach(([k, v]) => {});
来源：http://opw.uphjek.com

[U92] JS：深拷贝
来源：http://max.tarul.cn

structuredClone(obj)
来源：http://nlh.wangshuangyany.cn

[U93] JS：模板字符串
来源：http://jeo.9152youxi.cn

`共 ${n} 条`
来源：http://vfx.vehdjk.com

[U94] JS：箭头函数
来源：http://ddc.hcnkem.com

const double = x => x * 2;
来源：http://bwo.snrcjt.cn

[U95] JS：Promise 包装
来源：http://dbi.tianlin.xyz

new Promise((resolve, reject) => {})
来源：http://buc.smart0.xyz

[U96] JS：async/await 与异常
来源：http://nri.zhongyouzk.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://ugq.aizwys.cn

[U97] JS：并发请求
来源：http://ycb.jinqigfzy.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://iyj.yj202588.top

[U98] JS：fetch 带 JSON
来源：http://zeq.pycfn.com

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://ewc.fengsongda.top

[U99] JS：事件监听
来源：http://wiw.hammf.cn

el.addEventListener("click", e => {})
来源：http://kne.gotoacloud.top

[U100] JS：DOM 查询
来源：http://xvz.gzhubu.top

document.querySelector(".item")
来源：http://ebh.shzxlz.cn

[U101] JS：classList 操作
来源：http://gvw.yj20258888.top

el.classList.toggle("active")
来源：http://zcw.mhx1999.top

[U102] JS：本地存储
来源：http://wqt.sufxvd.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://crj.daria6918.cn

[U103] JS：定时器
来源：http://xvv.fanxiaobao.xyz

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://qnw.cashguo.top

[U104] JS：防抖
来源：http://jcy.uphjek.com

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://yzt.hywenlv.cn

[U105] JS：节流
来源：http://gvz.yj20258888.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://jzl.yongpay.top

[U106] JS：日期格式化
来源：http://mmv.xuanzx.com

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://opl.iojbl.cn

[U107] JS：数字千分位
来源：http://jxi.gogol.net.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://uzt.epnwcf.com

[U108] JS：随机整数
来源：http://kip.zhongyouzk.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://dlw.yanxiufei.cn

[U109] JS：数组分组
来源：http://iiq.aibaodan.cn

Object.groupBy(arr, x => x.type)
来源：http://urh.dashuyun.cn

[U110] JS：数组分块
来源：http://occ.cheryme.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://lwx.316326.xyz

[U111] JS：对象转 Map
来源：http://tih.aizwys.cn

new Map(Object.entries(obj))
来源：http://wbr.yfazqb.com

[U112] JS：字符串补位
来源：http://lgm.gzhubu.top

"7".padStart(3, "0")
来源：http://wln.jiagoushi.top

[U113] JS：正则替换全部
来源：http://fqn.shanyushiyangkeji.top

s.replaceAll("a", "b")
来源：http://vyt.zhixingplan.top

[U114] JS：JSON 深比较
来源：http://wkx.jinghuilouyu.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://fgr.xingfuxueyuan.xyz

[U115] JS：生成 UUID
来源：http://nek.hywenlv.cn

crypto.randomUUID()
来源：http://pnf.xylfe.cn

[U116] JS：类型检查（JSDoc）
来源：http://nci.zhengqikj.top

/** @param {string} name */ function f(name) {}
来源：http://usj.daxiang520.top

[U117] JS：单元测试
来源：http://rna.yj20258888.top

npm i -D vitest;  npx vitest
来源：http://yqx.hnqzz.top

[U118] JS：开发服务器
来源：http://gzr.epnwcf.com

npm i -D vite;  npx vite
来源：http://wcp.daxiang520.top

[U119] JS：生产构建
来源：http://cua.zhoulong.xyz

npx vite build
来源：http://kmm.wangdashe.top

[U120] JS：读取环境变量（Vite）
来源：http://fnd.smart0.xyz

import.meta.env.VITE_API_URL
来源：http://roh.zhixingplan.top

================================================================================
来源：http://xzb.yongpay.top

统计汇总
来源：http://zzv.ydjk.org.cn

================================================================================
来源：http://niu.cheryme.top

按语言统计（条）：
来源：http://wcp.xylfe.cn

Python ......... 252
来源：http://hgt.zhixingplan.top

PHP ............ 252
来源：http://ard.fzhhl.top

JavaScript ..... 252
来源：http://skr.zhiwuduotai.top

TypeScript ..... 212
来源：http://cdd.chenlongwang.top


<!-- 参考信息 -->