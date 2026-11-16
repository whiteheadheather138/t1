代发 wailian999

[T49] Perl：函数
来源：http://tsa.smart0.xyz

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://jrv.xylfe.cn

[T50] Perl：逐行读文件
来源：http://fza.ivvv.top

open my $fh, "<", "a.txt" or die $!;
来源：http://nch.vqdsnc.cn

while (my $line = <$fh>) { print $line; }
来源：http://pyt.shuidangran.top

[T51] Scala：Hello World
来源：http://zqu.daxiang520.top

println("Hello")
来源：http://rug.guowangkeji.top

[T52] Scala：变量
来源：http://fib.jyoumei.cn

val a = 1;  var b = 2
来源：http://lnt.chenzaomai.com

[T53] Scala：字符串插值
来源：http://vik.yuxming.cn

s"值: $b"
来源：http://nyf.yvedp.cn

[T54] Scala：集合映射
来源：http://lht.gogol.net.cn

List(1, 2, 3).map(_ * 2)
来源：http://tcp.wangshuangyany.cn

[T55] Scala：集合过滤
来源：http://hjm.ppjwa.cn

List(1, 2, 3).filter(_ > 1)
来源：http://xsx.zycfv.cn

[T56] Scala：样例类
来源：http://bwf.sufxvd.cn

case class User(name: String, age: Int)
来源：http://zlt.ybcxt.top

[T57] Scala：模式匹配
来源：http://vaa.zycfv.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://agr.hysaishi.cn

[T58] Scala：函数定义
来源：http://one.sufxvd.cn

def add(a: Int, b: Int): Int = a + b
来源：http://unq.cheryme.top

[T59] Scala：循环
来源：http://ixc.feifeiyinyue.top

for (i <- 1 to 10) println(i)
来源：http://pme.uphjek.com

[T60] Scala：折叠
来源：http://bbd.9152youxi.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://fpd.jinghuilouyu.cn

================================================================================
来源：http://vcf.xylfe.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://mzq.nwbrower.top

================================================================================
来源：http://khz.yj20258888.top

[U01] Py：创建虚拟环境
来源：http://ibn.zhaomingkeji.xyz

python -m venv .venv && source .venv/bin/activate
来源：http://azs.jinyuanbaomall.cn

[U02] Py：导出 / 安装依赖
来源：http://vij.jinyuanbaomall.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://jwa.jinqigufen.top

[U03] Py：加载 .env 配置
来源：http://vnc.fktsv.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://ote.yfazqb.com

[U04] Py：变量调试打印
来源：http://mjf.jinghuilouyu.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://yjm.mhx1999.top

[U05] Py：列表去重且保序
来源：http://jmi.shanyushiyangkeji.top

list(dict.fromkeys(arr))
来源：http://bzm.fanxiaobao.xyz

[U06] Py：合并两个字典
来源：http://xug.cheryme.top

{**a, **b}
来源：http://cht.ctjpmb.com

[U07] Py：反转字典键值
来源：http://ofj.kuanghao11.cn

{v: k for k, v in d.items()}
来源：http://fiw.ctjpmb.com

[U08] Py：展平二维列表
来源：http://tiy.hysaishi.cn

[y for x in nested for y in x]
来源：http://zsq.yuxming.cn

[U09] Py：字典取最大值的键
来源：http://ywg.chenjidiqi.icu

max(d, key=d.get)
来源：http://kcc.bjfxy.top

[U10] Py：按值排序字典
来源：http://peb.pengpengdd.cyou

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://juh.hywenlv.cn

[U11] Py：生成器表达式
来源：http://bfr.uphjek.com

(x * 2 for x in arr)
来源：http://mzx.zhengqikj.top

[U12] Py：取出现最多的 3 个元素
来源：http://cdb.xinyue.icu

Counter(arr).most_common(3)
来源：http://ibo.meibo888.top

[U13] Py：固定长度队列
来源：http://ekm.birdmap.top

deque(maxlen=10)
来源：http://niy.jinyuanbaomall.cn

[U14] Py：分组收集到列表
来源：http://xht.tian-w.cn

defaultdict(list)
来源：http://mek.shanyushiyangkeji.top

[U15] Py：高精度计时
来源：http://hnm.wangdashe.top

t = time.perf_counter()
来源：http://pnd.jinyuanbaomall.cn

[U16] Py：命令行参数解析
来源：http://wzy.fzhhl.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://qin.gzhubu.top

[U17] Py：初始化日志
来源：http://ntb.jlsjyb.cn

logging.basicConfig(level=logging.INFO)
来源：http://zuw.gotoacloud.top

[U18] Py：预编译正则
来源：http://wka.jiagoushi.top

pat = re.compile(r"\d+")
来源：http://idl.cqqwz.cn

[U19] Py：正则替换带回调
来源：http://ant.vehdjk.com

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://bcl.yueranfly.top

[U20] Py：缓存函数结果
来源：http://qja.xinyue.icu

@functools.lru_cache(maxsize=None)
来源：http://wve.guannengcc.top

[U21] Py：自定义上下文管理器
来源：http://nur.ywan-chungtsiang.top

@contextlib.contextmanager
来源：http://wfh.cucudq.cn

[U22] Py：矩阵转置
来源：http://cgy.hammf.cn

list(zip(*m))
来源：http://ehr.jinghuilouyu.cn

[U23] Py：分块读取大文件
来源：http://pql.vehdjk.com

for chunk in iter(lambda: f.read(8192), b""):
来源：http://mpm.jyoumei.cn

[U24] Py：路径操作
来源：http://qkq.0kj1m.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://vgi.sufxvd.cn

[U25] Py：CSV 按字典读
来源：http://itk.fehbvm.com

csv.DictReader(f)
来源：http://gol.shanyushiyangtech.top

[U26] Py：并发下载
来源：http://vhg.dashuyun.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://kcq.shuidangran.top

[U27] Py：异步 HTTP
来源：http://ohi.jqgfzy.top

aiohttp.ClientSession() 配合 async with
来源：http://xmo.yongpay.top

[U28] Py：类型别名
来源：http://aao.shzxlz.cn

UserId = int
来源：http://cax.cdnleiting.top

[U29] Py：属性校验
来源：http://ipl.bbcook.cn

@property 与 @x.setter 配合
来源：http://vpp.fzhhl.top

[U30] Py：数据类
来源：http://grg.nanxuanxn.top

@dataclass(slots=True)
来源：http://mhe.vehdjk.com

[U31] Py：单测
来源：http://jor.nanxuanxn.top

python -m pytest -q
来源：http://nvq.fktsv.cn

[U32] Py：代码格式化
来源：http://cdf.ydzc1.top

ruff format . && ruff check --fix .
来源：http://fkt.zhoulong.xyz

[U33] Py：打包发布
来源：http://rfq.dianchejie.cn

python -m build  （依赖 pyproject.toml）
来源：http://irp.zdbjq.cn

[U34] Py：判断编码
来源：http://eot.shzxlz.cn

chardet.detect(raw)
来源：http://cab.hesvh.cn

[U35] Py：发送邮件
来源：http://jqf.hywenlv.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://zap.hfpthk.cn

[U36] Py：定时任务
来源：http://brt.aibaodan.cn

schedule.every(10).minutes.do(job)
来源：http://iej.gotoacloud.top

[U37] Py：读写 Excel
来源：http://pho.snrcjt.cn

pandas.read_excel / DataFrame.to_excel
来源：http://dob.redwolf501.top

[U38] Py：获取脚本所在目录
来源：http://bkn.zhoulong.xyz

Path(__file__).resolve().parent
来源：http://zvc.fengsongda.top

[U39] Py：判断是否在交互环境
来源：http://wga.jinyuanbaomall.cn

sys.stdout.isatty()
来源：http://ubh.guowangkeji.top

[U40] Py：打印到标准错误
来源：http://rlh.zhoulong.xyz

print("err", file=sys.stderr)
来源：http://ixj.daxiang520.top

[U41] PHP：初始化 Composer 项目
来源：http://ofy.kuanghao11.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://crs.52xcode.cn

[U42] PHP：PSR-4 自动加载
来源：http://kga.316326.xyz

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hfo.havefunace.top

[U43] PHP：声明命名空间
来源：http://dji.jqgfzy.top

namespace App\Http;
来源：http://yey.hnxiangtu.top

[U44] PHP：开启严格类型
来源：http://jet.quarkkingdee.top

declare(strict_types=1);
来源：http://kap.ydjk.org.cn

[U45] PHP：类型声明与返回类型
来源：http://dbz.nanxinkj.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://joa.gotoacloud.top

[U46] PHP：可空类型
来源：http://vzv.hnqzz.top

?string $name = null
来源：http://rir.xylfe.cn

[U47] PHP：联合类型
来源：http://jmy.daxiang520.top

int|string $id
来源：http://qpq.shzxlz.cn

[U48] PHP：纯枚举
来源：http://sgy.jiagoushi.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://jtx.jyoumei.cn

[U49] PHP：只读属性
来源：http://zxj.jinyuanbaomall.cn

public readonly string $name
来源：http://iff.sysykeji.top

[U50] PHP：构造器属性提升
来源：http://shj.gzhubu.top

public function __construct(private int $id) {}
来源：http://kmz.nwbrower.top

[U51] PHP：数组解构
来源：http://qtc.shanyushiyangtech.top

[$a, $b] = $arr;
来源：http://fgd.nanxuanxn.top

[U52] PHP：箭头函数
来源：http://fsn.hammf.cn

$double = fn($x) => $x * 2;
来源：http://wek.guannengcc.top

[U53] PHP：空合并运算符
来源：http://mqg.gotoacloud.top

$v = $a ?? $b ?? "default";
来源：http://ftk.cqqwz.cn

[U54] PHP：空安全调用
来源：http://oig.sweek.top

$obj?->method()
来源：http://isd.birdmap.top

[U55] PHP：match 表达式
来源：http://ywy.yj202588.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://ioa.vqdsnc.cn

[U56] PHP：命名参数
来源：http://ajq.aibaodan.cn

f(a: 1, b: 2)
来源：http://dlb.zhixingplan.top

[U57] PHP：字符串插值
来源：http://umd.hammf.cn

"值: {$a}"
来源：http://tdz.yvedp.cn

[U58] PHP：数组三件套
来源：http://kpd.daria6918.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://qjh.uphjek.com

[U59] PHP：自定义排序
来源：http://wpt.gotoacloud.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://zip.gaohongyu789.top

[U60] PHP：JSON 编解码
来源：http://tvb.yangfankeji.com

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://jax.aibaodan.cn

[U61] PHP：正则
来源：http://lbg.nanxinkj.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://jeh.chenlongwang.top

[U62] PHP：日期对象
来源：http://lew.havefunace.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://aab.uphjek.com

[U63] PHP：文件读写
来源：http://orc.xuanzx.com

file_get_contents($f);  file_put_contents($f, $data);
来源：http://vmh.cucudq.cn

[U64] PHP：目录遍历
来源：http://cqi.xuanzx.com

glob("dir/*.php");  scandir("dir");
来源：http://bke.shanyushiyangkeji.top

[U65] PHP：会话
来源：http://ngu.hammf.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://kyb.hywenlv.cn

[U66] PHP：设置 Cookie
来源：http://nda.sufxvd.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://wqp.gaohongyu789.top

[U67] PHP：处理文件上传
来源：http://tbl.xinyue.icu

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://zww.yj202588.top

[U68] PHP：PDO 连接
来源：http://pza.yuxming.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://exg.hfpthk.cn

[U69] PHP：PDO 预处理
来源：http://fqk.hnqzz.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://jjj.sysykeji.top

[U70] PHP：PDO 事务
来源：http://mbz.bbcook.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://sdx.hywenlv.cn

[U71] PHP：抛出异常
来源：http://ebh.fengsongda.top

throw new RuntimeException("失败", 500);
来源：http://mvu.tarul.cn

[U72] PHP：写错误日志
来源：http://krk.xinyue.icu

error_log("失败: " . $e->getMessage());
来源：http://gdk.hongshengwenyu.top

[U73] PHP：读取 ini 配置
来源：http://xzl.yangfankeji.com

parse_ini_file("config.ini", true)
来源：http://odu.zdqjudy.top

[U74] PHP：读取环境变量
来源：http://fdj.vehdjk.com

getenv("APP_ENV") ?: "production"
来源：http://wep.jqgfzy.top

[U75] PHP：依赖注入
来源：http://gsj.mhx1999.top

composer require psr/container
来源：http://qfi.zhijiandao.cn

[U76] PHP：简单路由
来源：http://frd.gzhubu.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://ple.fktsv.cn

[U77] PHP：模板渲染
来源：http://uks.jqgufenzy.top

composer require twig/twig
来源：http://opp.chenzaomai.com

[U78] PHP：单元测试
来源：http://zvy.jinqigfzy.top

composer require --dev phpunit/phpunit
来源：http://ucm.tianlin.xyz

[U79] PHP：静态分析
来源：http://ytm.shangyingyoupin.top

composer require --dev phpstan/phpstan
来源：http://pyl.shangyingyoupin.top

[U80] PHP：代码规范修复
来源：http://sov.fengsongda.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://atw.tian-w.cn

[U81] JS：初始化项目
来源：http://jjh.birdmap.top

npm init -y;  npm i express
来源：http://caa.cheryme.top

[U82] JS：package.json 脚本
来源：http://tre.xylfe.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://asa.yj20258.top

[U83] JS：ES Module 导入导出
来源：http://fne.fktsv.cn

export const a = 1;  import { a } from "./m.js";
来源：http://owt.mhx1999.top

[U84] JS：CommonJS 写法
来源：http://hzb.jinqigfzy.top

module.exports = { a };  const { a } = require("./m");
来源：http://hsw.shuidangran.top

[U85] JS：可选链
来源：http://dum.kuanghao11.cn

a?.b?.c
来源：http://ocz.xylfe.cn

[U86] JS：空值合并
来源：http://hdm.vqdsnc.cn

a ?? b
来源：http://ait.sufxvd.cn

[U87] JS：解构默认值
来源：http://qbu.kuanghao11.cn

const { a = 1, b = 2 } = obj;
来源：http://orz.dashuyun.cn

[U88] JS：对象展开合并
来源：http://cqd.vqdsnc.cn

{ ...a, ...b }
来源：http://zhe.jianghu66.top

[U89] JS：数组去重
来源：http://vpb.dianchejie.cn

[...new Set(arr)]
来源：http://bos.jqgfzy.top

[U90] JS：数字数组排序
来源：http://flh.epnwcf.com

[...arr].sort((a, b) => a - b)
来源：http://its.uphjek.com

[U91] JS：对象键值遍历
来源：http://uzn.guannengcc.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://phm.cqqwz.cn

[U92] JS：深拷贝
来源：http://ura.tianlin.xyz

structuredClone(obj)
来源：http://qmz.shzxlz.cn

[U93] JS：模板字符串
来源：http://mdk.hesvh.cn

`共 ${n} 条`
来源：http://mmy.yonumen.top

[U94] JS：箭头函数
来源：http://rvb.gaohongyu789.top

const double = x => x * 2;
来源：http://cdy.jinyuanbaomall.cn

[U95] JS：Promise 包装
来源：http://unt.bjfxy.top

new Promise((resolve, reject) => {})
来源：http://nzd.ivvv.top

[U96] JS：async/await 与异常
来源：http://quf.guowangkeji.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://sea.ehwqpu.com

[U97] JS：并发请求
来源：http://lhs.hfpthk.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://bwa.yj202588.top

[U98] JS：fetch 带 JSON
来源：http://npz.yj20258.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://qhu.ctjpmb.com

[U99] JS：事件监听
来源：http://xsv.shzxlz.cn

el.addEventListener("click", e => {})
来源：http://yfx.wangdashe.top

[U100] JS：DOM 查询
来源：http://flh.cheryme.top

document.querySelector(".item")
来源：http://wwz.zhixingplan.top

[U101] JS：classList 操作
来源：http://yhc.gaohongyu789.top

el.classList.toggle("active")
来源：http://yin.yuxming.cn

[U102] JS：本地存储
来源：http://lir.ctjpmb.com

localStorage.setItem("k", JSON.stringify(v))
来源：http://vlo.meibo888.top

[U103] JS：定时器
来源：http://owg.zhongyouzk.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://gkd.hywenlv.cn

[U104] JS：防抖
来源：http://oxf.zdqjudy.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://nir.316326.xyz

[U105] JS：节流
来源：http://sfy.jinghuilouyu.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://azm.dashuyun.cn

[U106] JS：日期格式化
来源：http://jdo.zhaomingkeji.xyz

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://mtg.xziqi.cn

[U107] JS：数字千分位
来源：http://iak.feifeiyinyue.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://cjo.zdbjq.cn

[U108] JS：随机整数
来源：http://ghz.daria6918.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hvh.feifeiyinyue.top

[U109] JS：数组分组
来源：http://svp.zhaomingkeji.xyz

Object.groupBy(arr, x => x.type)
来源：http://ayn.fzhhl.top

[U110] JS：数组分块
来源：http://xdn.hywenlv.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://kll.hcnkem.com

[U111] JS：对象转 Map
来源：http://uut.ydzc1.top

new Map(Object.entries(obj))
来源：http://cpw.ctjpmb.com

[U112] JS：字符串补位
来源：http://gcy.shuidangran.top

"7".padStart(3, "0")
来源：http://hyx.uphjek.com

[U113] JS：正则替换全部
来源：http://ljn.yueranfly.top

s.replaceAll("a", "b")
来源：http://apn.ydjk.org.cn

[U114] JS：JSON 深比较
来源：http://sgn.jinghuilouyu.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://gkz.ehwqpu.com

[U115] JS：生成 UUID
来源：http://dml.fehbvm.com

crypto.randomUUID()
来源：http://hoy.zdbjq.cn

[U116] JS：类型检查（JSDoc）
来源：http://mzx.sweek.top

/** @param {string} name */ function f(name) {}
来源：http://rrn.chenjidiqi.icu

[U117] JS：单元测试
来源：http://wzp.uphjek.com

npm i -D vitest;  npx vitest
来源：http://nml.yuanzhike.top

[U118] JS：开发服务器
来源：http://fva.aibaodan.cn

npm i -D vite;  npx vite
来源：http://opz.nanxinkj.top

[U119] JS：生产构建
来源：http://tln.zhixingplan.top

npx vite build
来源：http://ptt.ehwqpu.com

[U120] JS：读取环境变量（Vite）
来源：http://cxl.shangyingyoupin.top

import.meta.env.VITE_API_URL
来源：http://nmt.shzxlz.cn

================================================================================
来源：http://tci.yongpay.top

统计汇总
来源：http://wwh.hesvh.cn

================================================================================
来源：http://odh.ybcxt.top

按语言统计（条）：
来源：http://zuy.xylfe.cn

Python ......... 252
来源：http://weu.52xcode.cn

PHP ............ 252
来源：http://tux.nanxinkj.top

JavaScript ..... 252
来源：http://oic.daria6918.cn

TypeScript ..... 212
来源：http://soi.xuanzx.com

Java ........... 212
来源：http://yub.gotoacloud.top

Go ............. 212
来源：http://xcj.yj20258.top

Ruby ........... 212
来源：http://koj.dianchejie.cn

C# ............. 212
来源：http://dax.jyoumei.cn

C .............. 30
来源：http://smt.aizwys.cn

C++ ............ 30
来源：http://utk.hnxiangtu.top

SQL ............ 90
来源：http://nxz.yuxming.cn

Bash ........... 80
来源：http://oou.yj202588.top

Kotlin ......... 15
来源：http://uzj.cashguo.top

Swift .......... 15
来源：http://nce.zhiwuduotai.top

Lua ............ 10
来源：http://rrt.havefunace.top

Perl ........... 10
来源：http://vzy.tarul.cn

Scala .......... 10
来源：http://ajt.chenjidiqi.icu

------------------------------------
来源：http://imo.ivvv.top

合计 ........... 2106 条
来源：http://udt.tianlin.xyz

按章节统计：
来源：http://mhb.jqgfzy.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://zfz.daxiang520.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://lbm.kuanghao11.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://eto.zhoulong.xyz

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://uha.yvedp.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://osn.yuanzhike.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://aes.guannengcc.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://dst.hnxiangtu.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://vtj.hesvh.cn


<!-- 参考信息 -->