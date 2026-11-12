代发 wailian999

while (my $line = <$fh>) { print $line; }
来源：http://hqd.bbcook.cn

[T51] Scala：Hello World
来源：http://dro.pengpengdd.cyou

println("Hello")
来源：http://pzu.xziqi.cn

[T52] Scala：变量
来源：http://iak.snrcjt.cn

val a = 1;  var b = 2
来源：http://pkl.fktsv.cn

[T53] Scala：字符串插值
来源：http://kog.wangshuangyany.cn

s"值: $b"
来源：http://dcx.daria6918.cn

[T54] Scala：集合映射
来源：http://pgz.sjlbkw.cn

List(1, 2, 3).map(_ * 2)
来源：http://tnp.feifeiyinyue.top

[T55] Scala：集合过滤
来源：http://zuq.zhaomingkeji.xyz

List(1, 2, 3).filter(_ > 1)
来源：http://csa.cucudq.cn

[T56] Scala：样例类
来源：http://xtk.dashuyun.cn

case class User(name: String, age: Int)
来源：http://fms.fehbvm.com

[T57] Scala：模式匹配
来源：http://wlg.ybcxt.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://thk.nanxuanxn.top

[T58] Scala：函数定义
来源：http://zny.mhx1999.top

def add(a: Int, b: Int): Int = a + b
来源：http://dbd.pycfn.com

[T59] Scala：循环
来源：http://qxu.hesvh.cn

for (i <- 1 to 10) println(i)
来源：http://xqx.ppjwa.cn

[T60] Scala：折叠
来源：http://tkw.hnqzz.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://obz.gaohongyu789.top

================================================================================
来源：http://ipg.yonumen.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://yii.epnwcf.com

================================================================================
来源：http://qro.jqgufenzy.top

[U01] Py：创建虚拟环境
来源：http://znt.epnwcf.com

python -m venv .venv && source .venv/bin/activate
来源：http://iku.nanxinkj.top

[U02] Py：导出 / 安装依赖
来源：http://nld.feifeiyinyue.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://dfl.fengsongda.top

[U03] Py：加载 .env 配置
来源：http://ayy.yuanzhike.top

from dotenv import load_dotenv; load_dotenv()
来源：http://ajb.xuanzx.com

[U04] Py：变量调试打印
来源：http://njg.smart0.xyz

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://fth.vqdsnc.cn

[U05] Py：列表去重且保序
来源：http://yan.jyoumei.cn

list(dict.fromkeys(arr))
来源：http://wzv.hnqzz.top

[U06] Py：合并两个字典
来源：http://mze.jinqigufen.top

{**a, **b}
来源：http://voe.zycfv.cn

[U07] Py：反转字典键值
来源：http://jyj.birdmap.top

{v: k for k, v in d.items()}
来源：http://ouw.zhaomingkeji.xyz

[U08] Py：展平二维列表
来源：http://opa.zdqjudy.top

[y for x in nested for y in x]
来源：http://qij.ivvv.top

[U09] Py：字典取最大值的键
来源：http://bks.hnxiangtu.top

max(d, key=d.get)
来源：http://kut.svipenyu.cn

[U10] Py：按值排序字典
来源：http://yzs.ydjk.org.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://bdx.sxryk.cn

[U11] Py：生成器表达式
来源：http://txg.cdnleiting.top

(x * 2 for x in arr)
来源：http://exd.hywenlv.cn

[U12] Py：取出现最多的 3 个元素
来源：http://jhf.hnxiangtu.top

Counter(arr).most_common(3)
来源：http://uqx.hcnkem.com

[U13] Py：固定长度队列
来源：http://hsz.daxiang520.top

deque(maxlen=10)
来源：http://tqg.fehbvm.com

[U14] Py：分组收集到列表
来源：http://her.shuidangran.top

defaultdict(list)
来源：http://gbe.bjfxy.top

[U15] Py：高精度计时
来源：http://ntw.kuanghao11.cn

t = time.perf_counter()
来源：http://vif.shuidangran.top

[U16] Py：命令行参数解析
来源：http://nnd.wangshuangyany.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://zng.zycfv.cn

[U17] Py：初始化日志
来源：http://qba.tianlin.xyz

logging.basicConfig(level=logging.INFO)
来源：http://ern.sweek.top

[U18] Py：预编译正则
来源：http://ewl.bbcook.cn

pat = re.compile(r"\d+")
来源：http://psj.xziqi.cn

[U19] Py：正则替换带回调
来源：http://qlc.sufxvd.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://rmn.hesvh.cn

[U20] Py：缓存函数结果
来源：http://ogv.sxryk.cn

@functools.lru_cache(maxsize=None)
来源：http://esh.epnwcf.com

[U21] Py：自定义上下文管理器
来源：http://xwq.tianlin.xyz

@contextlib.contextmanager
来源：http://zjk.sxryk.cn

[U22] Py：矩阵转置
来源：http://jhc.cashguo.top

list(zip(*m))
来源：http://qwu.sjlbkw.cn

[U23] Py：分块读取大文件
来源：http://vvi.hysaishi.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://cvk.jinqigfzy.top

[U24] Py：路径操作
来源：http://ghf.sxryk.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://khz.mhx1999.top

[U25] Py：CSV 按字典读
来源：http://mpi.ydjk.org.cn

csv.DictReader(f)
来源：http://jxj.jqgfzy.top

[U26] Py：并发下载
来源：http://ier.meibo888.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://pbu.jyoumei.cn

[U27] Py：异步 HTTP
来源：http://hdz.shangyingyoupin.top

aiohttp.ClientSession() 配合 async with
来源：http://fod.0kj1m.cn

[U28] Py：类型别名
来源：http://oss.yonumen.top

UserId = int
来源：http://icl.chenjidiqi.icu

[U29] Py：属性校验
来源：http://qdj.jinqigfzy.top

@property 与 @x.setter 配合
来源：http://utu.gotoacloud.top

[U30] Py：数据类
来源：http://pnh.hfpthk.cn

@dataclass(slots=True)
来源：http://wkl.epnwcf.com

[U31] Py：单测
来源：http://uhq.ywan-chungtsiang.top

python -m pytest -q
来源：http://stm.yongpay.top

[U32] Py：代码格式化
来源：http://rgt.sweek.top

ruff format . && ruff check --fix .
来源：http://gmq.iojbl.cn

[U33] Py：打包发布
来源：http://mfl.hysaishi.cn

python -m build  （依赖 pyproject.toml）
来源：http://lru.gotoacloud.top

[U34] Py：判断编码
来源：http://czc.zdqjudy.top

chardet.detect(raw)
来源：http://eco.shanyushiyangkeji.top

[U35] Py：发送邮件
来源：http://yeu.sysykeji.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://whr.jqgfzy.top

[U36] Py：定时任务
来源：http://mpk.epnwcf.com

schedule.every(10).minutes.do(job)
来源：http://tjt.ybcxt.top

[U37] Py：读写 Excel
来源：http://cnc.bjfxy.top

pandas.read_excel / DataFrame.to_excel
来源：http://rwk.fzhhl.top

[U38] Py：获取脚本所在目录
来源：http://qzb.hywenlv.cn

Path(__file__).resolve().parent
来源：http://aao.snrcjt.cn

[U39] Py：判断是否在交互环境
来源：http://xfw.hysaishi.cn

sys.stdout.isatty()
来源：http://cze.yueranfly.top

[U40] Py：打印到标准错误
来源：http://zpt.redwolf501.top

print("err", file=sys.stderr)
来源：http://nkk.feifeiyinyue.top

[U41] PHP：初始化 Composer 项目
来源：http://ekn.52xcode.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://ovl.yongpay.top

[U42] PHP：PSR-4 自动加载
来源：http://vaz.zhongyouzk.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://pyw.smart0.xyz

[U43] PHP：声明命名空间
来源：http://zhz.yanxiufei.cn

namespace App\Http;
来源：http://kql.haohaochexian.top

[U44] PHP：开启严格类型
来源：http://usg.zhaomingkeji.xyz

declare(strict_types=1);
来源：http://cjz.fanxiaobao.xyz

[U45] PHP：类型声明与返回类型
来源：http://gju.52xcode.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://rop.gogol.net.cn

[U46] PHP：可空类型
来源：http://jqb.hnqzz.top

?string $name = null
来源：http://mjq.fzhhl.top

[U47] PHP：联合类型
来源：http://vpr.hfpthk.cn

int|string $id
来源：http://etc.dianchejie.cn

[U48] PHP：纯枚举
来源：http://vws.zhongyouzk.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://lye.0kj1m.cn

[U49] PHP：只读属性
来源：http://mhl.hammf.cn

public readonly string $name
来源：http://pom.yj202588.top

[U50] PHP：构造器属性提升
来源：http://qzq.cucudq.cn

public function __construct(private int $id) {}
来源：http://unu.yanxiufei.cn

[U51] PHP：数组解构
来源：http://chv.zhoulong.xyz

[$a, $b] = $arr;
来源：http://jyf.guowangkeji.top

[U52] PHP：箭头函数
来源：http://pvl.jlsjyb.cn

$double = fn($x) => $x * 2;
来源：http://tyq.fanxiaobao.xyz

[U53] PHP：空合并运算符
来源：http://xtc.wangdashe.top

$v = $a ?? $b ?? "default";
来源：http://qel.pengpengdd.cyou

[U54] PHP：空安全调用
来源：http://xpa.jinyuanbaomall.cn

$obj?->method()
来源：http://vhc.haohaochexian.top

[U55] PHP：match 表达式
来源：http://xsr.bbcook.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://kac.fehbvm.com

[U56] PHP：命名参数
来源：http://hab.havefunace.top

f(a: 1, b: 2)
来源：http://xwi.ybcxt.top

[U57] PHP：字符串插值
来源：http://tqc.jinyuanbaomall.cn

"值: {$a}"
来源：http://lnv.chenzaomai.com

[U58] PHP：数组三件套
来源：http://kqh.gotoacloud.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://iam.hongshengwenyu.top

[U59] PHP：自定义排序
来源：http://xne.jlsjyb.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://rrh.haohaochexian.top

[U60] PHP：JSON 编解码
来源：http://mex.jinqigfzy.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://uog.gaohongyu789.top

[U61] PHP：正则
来源：http://gbw.quarkkingdee.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://nsw.jyoumei.cn

[U62] PHP：日期对象
来源：http://tnw.yuanzhike.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://ftx.shzxlz.cn

[U63] PHP：文件读写
来源：http://qlu.epnwcf.com

file_get_contents($f);  file_put_contents($f, $data);
来源：http://irc.andypj.xyz

[U64] PHP：目录遍历
来源：http://eme.daria6918.cn

glob("dir/*.php");  scandir("dir");
来源：http://xae.ybcxt.top

[U65] PHP：会话
来源：http://dlz.52xcode.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://buw.gzhubu.top

[U66] PHP：设置 Cookie
来源：http://ock.xuetiantiany.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://zhe.yangfankeji.com

[U67] PHP：处理文件上传
来源：http://ejw.yangfankeji.com

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://lbj.zhoulong.xyz

[U68] PHP：PDO 连接
来源：http://hzq.xinyue.icu

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://omu.andypj.xyz

[U69] PHP：PDO 预处理
来源：http://cef.bjfxy.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://dkz.sufxvd.cn

[U70] PHP：PDO 事务
来源：http://jqm.yanxiufei.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://nfs.yj20258.top

[U71] PHP：抛出异常
来源：http://iqo.vehdjk.com

throw new RuntimeException("失败", 500);
来源：http://wtz.yonumen.top

[U72] PHP：写错误日志
来源：http://rjr.jqgfzy.top

error_log("失败: " . $e->getMessage());
来源：http://pkv.hnxiangtu.top

[U73] PHP：读取 ini 配置
来源：http://onj.tarul.cn

parse_ini_file("config.ini", true)
来源：http://mxk.zdqjudy.top

[U74] PHP：读取环境变量
来源：http://obg.ehwqpu.com

getenv("APP_ENV") ?: "production"
来源：http://bar.hnxiangtu.top

[U75] PHP：依赖注入
来源：http://vlq.ywan-chungtsiang.top

composer require psr/container
来源：http://wlj.316326.xyz

[U76] PHP：简单路由
来源：http://uxx.uphjek.com

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://nyd.wangdashe.top

[U77] PHP：模板渲染
来源：http://bin.jyoumei.cn

composer require twig/twig
来源：http://dfv.jyoumei.cn

[U78] PHP：单元测试
来源：http://cjf.sysykeji.top

composer require --dev phpunit/phpunit
来源：http://dtv.yfazqb.com

[U79] PHP：静态分析
来源：http://jsc.jinqigfzy.top

composer require --dev phpstan/phpstan
来源：http://pzg.kuanghao11.cn

[U80] PHP：代码规范修复
来源：http://uek.c1oappe.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://lvx.fengsongda.top

[U81] JS：初始化项目
来源：http://sco.xuanzx.com

npm init -y;  npm i express
来源：http://ule.zhijiandao.cn

[U82] JS：package.json 脚本
来源：http://ffi.svipenyu.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://pad.fanxiaobao.xyz

[U83] JS：ES Module 导入导出
来源：http://riw.9152youxi.cn

export const a = 1;  import { a } from "./m.js";
来源：http://fqn.smart0.xyz

[U84] JS：CommonJS 写法
来源：http://rrr.gzhubu.top

module.exports = { a };  const { a } = require("./m");
来源：http://eon.jlsjyb.cn

[U85] JS：可选链
来源：http://cxo.yj20258.top

a?.b?.c
来源：http://heh.epnwcf.com

[U86] JS：空值合并
来源：http://nib.aizwys.cn

a ?? b
来源：http://jyj.yongpay.top

[U87] JS：解构默认值
来源：http://gyc.jinqigufen.top

const { a = 1, b = 2 } = obj;
来源：http://kmq.tian-w.cn

[U88] JS：对象展开合并
来源：http://oze.yvedp.cn

{ ...a, ...b }
来源：http://iwn.aibaodan.cn

[U89] JS：数组去重
来源：http://dyh.ydjk.org.cn

[...new Set(arr)]
来源：http://kxi.hnqzz.top

[U90] JS：数字数组排序
来源：http://ijt.ydjk.org.cn

[...arr].sort((a, b) => a - b)
来源：http://zdf.pycfn.com

[U91] JS：对象键值遍历
来源：http://jjc.svipenyu.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://dru.zhijiandao.cn

[U92] JS：深拷贝
来源：http://evo.sjlbkw.cn

structuredClone(obj)
来源：http://xth.guannengcc.top

[U93] JS：模板字符串
来源：http://xra.zhongyouzk.top

`共 ${n} 条`
来源：http://mwz.jianghu66.top

[U94] JS：箭头函数
来源：http://xip.zhongyouzk.top

const double = x => x * 2;
来源：http://emy.ywan-chungtsiang.top

[U95] JS：Promise 包装
来源：http://yty.feifeiyinyue.top

new Promise((resolve, reject) => {})
来源：http://ype.sjlbkw.cn

[U96] JS：async/await 与异常
来源：http://wjh.uphjek.com

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://mdp.xziqi.cn

[U97] JS：并发请求
来源：http://waf.meibo888.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://lyb.fehbvm.com

[U98] JS：fetch 带 JSON
来源：http://rrg.quarkkingdee.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://ywz.0kj1m.cn

[U99] JS：事件监听
来源：http://tew.fanxiaobao.xyz

el.addEventListener("click", e => {})
来源：http://wvw.hammf.cn

[U100] JS：DOM 查询
来源：http://fre.redwolf501.top

document.querySelector(".item")
来源：http://ypw.xuetiantiany.cn

[U101] JS：classList 操作
来源：http://ypi.chenlongwang.top

el.classList.toggle("active")
来源：http://mdg.fanxiaobao.xyz

[U102] JS：本地存储
来源：http://bzz.epnwcf.com

localStorage.setItem("k", JSON.stringify(v))
来源：http://wgj.ywan-chungtsiang.top

[U103] JS：定时器
来源：http://kla.dianchejie.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hqx.hammf.cn

[U104] JS：防抖
来源：http://xxu.shuidangran.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://xro.ctjpmb.com

[U105] JS：节流
来源：http://ioi.zhixingplan.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://vwg.jinqigfzy.top

[U106] JS：日期格式化
来源：http://jxx.bbcook.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://gex.yuanzhike.top

[U107] JS：数字千分位
来源：http://uwf.dianchejie.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://dov.snrcjt.cn

[U108] JS：随机整数
来源：http://qoj.cheryme.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://gfs.chenzaomai.com

[U109] JS：数组分组
来源：http://uwn.yj20258888.top

Object.groupBy(arr, x => x.type)
来源：http://xxm.hongshengwenyu.top

[U110] JS：数组分块
来源：http://omk.yongpay.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://pjl.xinyue.icu

[U111] JS：对象转 Map
来源：http://yit.redwolf501.top

new Map(Object.entries(obj))
来源：http://voc.c1oappe.top

[U112] JS：字符串补位
来源：http://nps.xinyue.icu

"7".padStart(3, "0")
来源：http://tkm.nanxuanxn.top

[U113] JS：正则替换全部
来源：http://iwq.guowangkeji.top

s.replaceAll("a", "b")
来源：http://ayi.aizwys.cn

[U114] JS：JSON 深比较
来源：http://per.jianghu66.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://grj.yj20258.top

[U115] JS：生成 UUID
来源：http://mpt.ivvv.top

crypto.randomUUID()
来源：http://buz.zhongyouzk.top

[U116] JS：类型检查（JSDoc）
来源：http://nlv.bjfxy.top

/** @param {string} name */ function f(name) {}
来源：http://kqv.zdqjudy.top

[U117] JS：单元测试
来源：http://ptk.cucudq.cn

npm i -D vitest;  npx vitest
来源：http://qgl.ydjk.org.cn

[U118] JS：开发服务器
来源：http://zuu.jinqigfzy.top

npm i -D vite;  npx vite
来源：http://iji.tianlin.xyz

[U119] JS：生产构建
来源：http://zlu.hammf.cn

npx vite build
来源：http://giz.jqgufenzy.top

[U120] JS：读取环境变量（Vite）
来源：http://rxm.birdmap.top

import.meta.env.VITE_API_URL
来源：http://nmn.daxiang520.top

================================================================================
来源：http://qdt.ctjpmb.com

统计汇总
来源：http://pxv.pengpengdd.cyou

================================================================================
来源：http://qae.zhiwuduotai.top

按语言统计（条）：
来源：http://tza.cucudq.cn

Python ......... 252
来源：http://elg.yj20258888.top

PHP ............ 252
来源：http://hju.shangyingyoupin.top

JavaScript ..... 252
来源：http://hoa.jyoumei.cn

TypeScript ..... 212
来源：http://cio.sxryk.cn

Java ........... 212
来源：http://qbs.cucudq.cn

Go ............. 212
来源：http://lfg.sufxvd.cn

Ruby ........... 212
来源：http://gjs.yj20258888.top

C# ............. 212
来源：http://zaq.daxiang520.top

C .............. 30
来源：http://wbk.fehbvm.com

C++ ............ 30
来源：http://lui.yj20258888.top

SQL ............ 90
来源：http://fhj.zhijiandao.cn

Bash ........... 80
来源：http://rmx.kuanghao11.cn

Kotlin ......... 15
来源：http://xrw.haohaochexian.top

Swift .......... 15
来源：http://jqd.jinqigufen.top

Lua ............ 10
来源：http://ffv.0kj1m.cn

Perl ........... 10
来源：http://nrs.iojbl.cn

Scala .......... 10
来源：http://gkh.c1oappe.top

------------------------------------
来源：http://bnp.dianchejie.cn

合计 ........... 2106 条
来源：http://mhv.yfazqb.com

按章节统计：
来源：http://rzd.hywenlv.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://icg.jiagoushi.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://qwf.hongshengwenyu.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://tjp.dianchejie.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://rmy.316326.xyz

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://oup.hnxiangtu.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://syt.52xcode.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://qwc.xylfe.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://uee.pengpengdd.cyou

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://ulp.redwolf501.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://uyv.jqgfzy.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://gxy.hcnkem.com

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://jfd.mhx1999.top


<!-- 参考信息 -->