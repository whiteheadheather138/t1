代发 wailian999

while (my $line = <$fh>) { print $line; }
来源：http://gwr.vehdjk.com

[T51] Scala：Hello World
来源：http://txj.316326.xyz

println("Hello")
来源：http://xyq.guannengcc.top

[T52] Scala：变量
来源：http://zul.xuetiantiany.cn

val a = 1;  var b = 2
来源：http://ahi.jinyuanbaomall.cn

[T53] Scala：字符串插值
来源：http://tnn.dianchejie.cn

s"值: $b"
来源：http://hvk.cdnleiting.top

[T54] Scala：集合映射
来源：http://yxi.feifeiyinyue.top

List(1, 2, 3).map(_ * 2)
来源：http://omx.guannengcc.top

[T55] Scala：集合过滤
来源：http://nmd.jyoumei.cn

List(1, 2, 3).filter(_ > 1)
来源：http://amn.hnqzz.top

[T56] Scala：样例类
来源：http://aod.kuanghao11.cn

case class User(name: String, age: Int)
来源：http://ezo.aizwys.cn

[T57] Scala：模式匹配
来源：http://kld.9152youxi.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://bwr.yangfankeji.com

[T58] Scala：函数定义
来源：http://vpb.fehbvm.com

def add(a: Int, b: Int): Int = a + b
来源：http://gbc.shangyingyoupin.top

[T59] Scala：循环
来源：http://lnn.ppjwa.cn

for (i <- 1 to 10) println(i)
来源：http://tuy.shzxlz.cn

[T60] Scala：折叠
来源：http://lrs.svipenyu.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://zva.zhaomingkeji.xyz

================================================================================
来源：http://wpv.jianghu66.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://kyq.xziqi.cn

================================================================================
来源：http://vlm.yangfankeji.com

[U01] Py：创建虚拟环境
来源：http://pno.ydzc1.top

python -m venv .venv && source .venv/bin/activate
来源：http://cno.chenzaomai.com

[U02] Py：导出 / 安装依赖
来源：http://qjs.yfazqb.com

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://wty.sxryk.cn

[U03] Py：加载 .env 配置
来源：http://apm.fehbvm.com

from dotenv import load_dotenv; load_dotenv()
来源：http://zah.bjfxy.top

[U04] Py：变量调试打印
来源：http://dsu.yanxiufei.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://ebx.fengsongda.top

[U05] Py：列表去重且保序
来源：http://lcz.haohaochexian.top

list(dict.fromkeys(arr))
来源：http://egv.zdqjudy.top

[U06] Py：合并两个字典
来源：http://ydr.haohaochexian.top

{**a, **b}
来源：http://nzb.zhengqikj.top

[U07] Py：反转字典键值
来源：http://qma.zdbjq.cn

{v: k for k, v in d.items()}
来源：http://hgy.hnxiangtu.top

[U08] Py：展平二维列表
来源：http://yku.xziqi.cn

[y for x in nested for y in x]
来源：http://mjd.jlsjyb.cn

[U09] Py：字典取最大值的键
来源：http://spz.uphjek.com

max(d, key=d.get)
来源：http://qzj.zhongyouzk.top

[U10] Py：按值排序字典
来源：http://gti.316326.xyz

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://nab.ehwqpu.com

[U11] Py：生成器表达式
来源：http://ulf.sysykeji.top

(x * 2 for x in arr)
来源：http://xzt.pengpengdd.cyou

[U12] Py：取出现最多的 3 个元素
来源：http://yiq.bbcook.cn

Counter(arr).most_common(3)
来源：http://kvi.zhoulong.xyz

[U13] Py：固定长度队列
来源：http://bid.wangdashe.top

deque(maxlen=10)
来源：http://ikm.hongshengwenyu.top

[U14] Py：分组收集到列表
来源：http://zdh.vehdjk.com

defaultdict(list)
来源：http://ppi.fehbvm.com

[U15] Py：高精度计时
来源：http://vtu.vqdsnc.cn

t = time.perf_counter()
来源：http://hrz.fengsongda.top

[U16] Py：命令行参数解析
来源：http://quz.gotoacloud.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://vbk.hnxiangtu.top

[U17] Py：初始化日志
来源：http://mkt.cheryme.top

logging.basicConfig(level=logging.INFO)
来源：http://azj.cdnleiting.top

[U18] Py：预编译正则
来源：http://zvg.birdmap.top

pat = re.compile(r"\d+")
来源：http://ocm.jianghu66.top

[U19] Py：正则替换带回调
来源：http://ooe.jqgufenzy.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://fov.zhijiandao.cn

[U20] Py：缓存函数结果
来源：http://ape.guowangkeji.top

@functools.lru_cache(maxsize=None)
来源：http://riy.gaohongyu789.top

[U21] Py：自定义上下文管理器
来源：http://whe.yfazqb.com

@contextlib.contextmanager
来源：http://nsw.fehbvm.com

[U22] Py：矩阵转置
来源：http://bej.xinyue.icu

list(zip(*m))
来源：http://wbo.wangdashe.top

[U23] Py：分块读取大文件
来源：http://lgn.hywenlv.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://qpl.haohaochexian.top

[U24] Py：路径操作
来源：http://klb.zycfv.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://zqo.pengpengdd.cyou

[U25] Py：CSV 按字典读
来源：http://uqa.chenjidiqi.icu

csv.DictReader(f)
来源：http://ffe.52xcode.cn

[U26] Py：并发下载
来源：http://rim.cdnleiting.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://ccv.aizwys.cn

[U27] Py：异步 HTTP
来源：http://bqx.xuetiantiany.cn

aiohttp.ClientSession() 配合 async with
来源：http://zvq.zdqjudy.top

[U28] Py：类型别名
来源：http://adj.fengsongda.top

UserId = int
来源：http://apa.dashuyun.cn

[U29] Py：属性校验
来源：http://ulf.gaohongyu789.top

@property 与 @x.setter 配合
来源：http://wxc.jlsjyb.cn

[U30] Py：数据类
来源：http://lus.ctjpmb.com

@dataclass(slots=True)
来源：http://rvb.jyoumei.cn

[U31] Py：单测
来源：http://tma.yj202588.top

python -m pytest -q
来源：http://dlb.redwolf501.top

[U32] Py：代码格式化
来源：http://ucw.sxryk.cn

ruff format . && ruff check --fix .
来源：http://qms.9152youxi.cn

[U33] Py：打包发布
来源：http://ldd.smart0.xyz

python -m build  （依赖 pyproject.toml）
来源：http://qno.redwolf501.top

[U34] Py：判断编码
来源：http://tnm.shanyushiyangkeji.top

chardet.detect(raw)
来源：http://tfo.nanxuanxn.top

[U35] Py：发送邮件
来源：http://bpl.yanxiufei.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://zyg.iojbl.cn

[U36] Py：定时任务
来源：http://nxp.jqgufenzy.top

schedule.every(10).minutes.do(job)
来源：http://ltl.gogol.net.cn

[U37] Py：读写 Excel
来源：http://cxr.nwbrower.top

pandas.read_excel / DataFrame.to_excel
来源：http://hea.birdmap.top

[U38] Py：获取脚本所在目录
来源：http://axp.daria6918.cn

Path(__file__).resolve().parent
来源：http://zyq.jiagoushi.top

[U39] Py：判断是否在交互环境
来源：http://xfh.smart0.xyz

sys.stdout.isatty()
来源：http://lfa.52xcode.cn

[U40] Py：打印到标准错误
来源：http://lew.daria6918.cn

print("err", file=sys.stderr)
来源：http://wpr.tanke756.top

[U41] PHP：初始化 Composer 项目
来源：http://mje.zhaomingkeji.xyz

composer init;  composer require guzzlehttp/guzzle
来源：http://tnd.zdqjudy.top

[U42] PHP：PSR-4 自动加载
来源：http://jga.zhijiandao.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://rin.gotoacloud.top

[U43] PHP：声明命名空间
来源：http://zye.vqdsnc.cn

namespace App\Http;
来源：http://qvv.tian-w.cn

[U44] PHP：开启严格类型
来源：http://ofc.daxiang520.top

declare(strict_types=1);
来源：http://ysc.xuanzx.com

[U45] PHP：类型声明与返回类型
来源：http://dmw.hesvh.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://wiv.chenzaomai.com

[U46] PHP：可空类型
来源：http://iks.guowangkeji.top

?string $name = null
来源：http://cze.mhx1999.top

[U47] PHP：联合类型
来源：http://aba.hnxiangtu.top

int|string $id
来源：http://odf.bbcook.cn

[U48] PHP：纯枚举
来源：http://gnh.zhongyouzk.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://ntz.tianlin.xyz

[U49] PHP：只读属性
来源：http://bls.xinyue.icu

public readonly string $name
来源：http://fxs.snrcjt.cn

[U50] PHP：构造器属性提升
来源：http://fdw.hywenlv.cn

public function __construct(private int $id) {}
来源：http://hat.dashuyun.cn

[U51] PHP：数组解构
来源：http://ers.andypj.xyz

[$a, $b] = $arr;
来源：http://jyz.andypj.xyz

[U52] PHP：箭头函数
来源：http://jig.tarul.cn

$double = fn($x) => $x * 2;
来源：http://xbz.zhixingplan.top

[U53] PHP：空合并运算符
来源：http://jkc.svipenyu.cn

$v = $a ?? $b ?? "default";
来源：http://rzm.shuidangran.top

[U54] PHP：空安全调用
来源：http://ult.hcnkem.com

$obj?->method()
来源：http://pkd.chenlongwang.top

[U55] PHP：match 表达式
来源：http://mqj.zhaomingkeji.xyz

$s = match($x) { 1 => "一", default => "其他" };
来源：http://dho.quarkkingdee.top

[U56] PHP：命名参数
来源：http://lbo.guowangkeji.top

f(a: 1, b: 2)
来源：http://llj.jianghu66.top

[U57] PHP：字符串插值
来源：http://rrq.zhaomingkeji.xyz

"值: {$a}"
来源：http://lse.cucudq.cn

[U58] PHP：数组三件套
来源：http://aok.hywenlv.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://msd.aibaodan.cn

[U59] PHP：自定义排序
来源：http://npk.birdmap.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://svv.zhoulong.xyz

[U60] PHP：JSON 编解码
来源：http://muj.svipenyu.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://vln.bjfxy.top

[U61] PHP：正则
来源：http://cwo.zhengqikj.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://dwn.ywan-chungtsiang.top

[U62] PHP：日期对象
来源：http://sbn.jianghu66.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://leg.sxryk.cn

[U63] PHP：文件读写
来源：http://wbb.ydjk.org.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://jfe.sufxvd.cn

[U64] PHP：目录遍历
来源：http://cab.sxryk.cn

glob("dir/*.php");  scandir("dir");
来源：http://fcy.jqgufenzy.top

[U65] PHP：会话
来源：http://dnr.smart0.xyz

session_start();  $_SESSION["uid"] = 1;
来源：http://cay.yuanzhike.top

[U66] PHP：设置 Cookie
来源：http://mxz.ybcxt.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://ebq.fanxiaobao.xyz

[U67] PHP：处理文件上传
来源：http://ohr.fzhhl.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://lpm.chenjidiqi.icu

[U68] PHP：PDO 连接
来源：http://vwo.jyoumei.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://jbu.yuanzhike.top

[U69] PHP：PDO 预处理
来源：http://mcd.chenjidiqi.icu

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://bup.sufxvd.cn

[U70] PHP：PDO 事务
来源：http://dnu.hfpthk.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://lzo.gzhubu.top

[U71] PHP：抛出异常
来源：http://vod.wangshuangyany.cn

throw new RuntimeException("失败", 500);
来源：http://zeq.9152youxi.cn

[U72] PHP：写错误日志
来源：http://zqy.yangfankeji.com

error_log("失败: " . $e->getMessage());
来源：http://utx.jlsjyb.cn

[U73] PHP：读取 ini 配置
来源：http://owj.vehdjk.com

parse_ini_file("config.ini", true)
来源：http://lnb.daxiang520.top

[U74] PHP：读取环境变量
来源：http://mpq.zdqjudy.top

getenv("APP_ENV") ?: "production"
来源：http://ehd.jinqigfzy.top

[U75] PHP：依赖注入
来源：http://zit.sjlbkw.cn

composer require psr/container
来源：http://yyo.xziqi.cn

[U76] PHP：简单路由
来源：http://qiu.hywenlv.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://cxo.cucudq.cn

[U77] PHP：模板渲染
来源：http://llo.fktsv.cn

composer require twig/twig
来源：http://zqc.sysykeji.top

[U78] PHP：单元测试
来源：http://xqp.jinqigufen.top

composer require --dev phpunit/phpunit
来源：http://gbw.xylfe.cn

[U79] PHP：静态分析
来源：http://wct.fktsv.cn

composer require --dev phpstan/phpstan
来源：http://kpz.tianlin.xyz

[U80] PHP：代码规范修复
来源：http://sxm.zhengqikj.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://srm.bjfxy.top

[U81] JS：初始化项目
来源：http://rhs.xuetiantiany.cn

npm init -y;  npm i express
来源：http://vqp.wangshuangyany.cn

[U82] JS：package.json 脚本
来源：http://amy.shangyingyoupin.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://uco.jinyuanbaomall.cn

[U83] JS：ES Module 导入导出
来源：http://owg.vqdsnc.cn

export const a = 1;  import { a } from "./m.js";
来源：http://xhj.xylfe.cn

[U84] JS：CommonJS 写法
来源：http://vzr.dashuyun.cn

module.exports = { a };  const { a } = require("./m");
来源：http://jvx.yvedp.cn

[U85] JS：可选链
来源：http://uyf.c1oappe.top

a?.b?.c
来源：http://pnx.cashguo.top

[U86] JS：空值合并
来源：http://gkv.daria6918.cn

a ?? b
来源：http://qxi.zhaomingkeji.xyz

[U87] JS：解构默认值
来源：http://muv.zdbjq.cn

const { a = 1, b = 2 } = obj;
来源：http://ssx.jianghu66.top

[U88] JS：对象展开合并
来源：http://vvm.guannengcc.top

{ ...a, ...b }
来源：http://djn.tianlin.xyz

[U89] JS：数组去重
来源：http://pya.yj20258888.top

[...new Set(arr)]
来源：http://lrv.xingfuxueyuan.xyz

[U90] JS：数字数组排序
来源：http://jwv.guannengcc.top

[...arr].sort((a, b) => a - b)
来源：http://kyt.bbcook.cn

[U91] JS：对象键值遍历
来源：http://mna.meibo888.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://vnp.sysykeji.top

[U92] JS：深拷贝
来源：http://ype.jinqigfzy.top

structuredClone(obj)
来源：http://tfc.zycfv.cn

[U93] JS：模板字符串
来源：http://wlh.ybcxt.top

`共 ${n} 条`
来源：http://olo.hnqzz.top

[U94] JS：箭头函数
来源：http://bkq.zdbjq.cn

const double = x => x * 2;
来源：http://txq.hysaishi.cn

[U95] JS：Promise 包装
来源：http://epc.birdmap.top

new Promise((resolve, reject) => {})
来源：http://sav.cqqwz.cn

[U96] JS：async/await 与异常
来源：http://wug.iojbl.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://wpn.hysaishi.cn

[U97] JS：并发请求
来源：http://mkx.snrcjt.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://tlz.pycfn.com

[U98] JS：fetch 带 JSON
来源：http://lxn.zhoulong.xyz

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://eer.dianchejie.cn

[U99] JS：事件监听
来源：http://ale.tianlin.xyz

el.addEventListener("click", e => {})
来源：http://onr.bbcook.cn

[U100] JS：DOM 查询
来源：http://eml.ehwqpu.com

document.querySelector(".item")
来源：http://hvl.yongpay.top

[U101] JS：classList 操作
来源：http://orl.snrcjt.cn

el.classList.toggle("active")
来源：http://olx.jinqigfzy.top

[U102] JS：本地存储
来源：http://rsz.havefunace.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://dsj.316326.xyz

[U103] JS：定时器
来源：http://zlu.jlsjyb.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://fgp.nanxinkj.top

[U104] JS：防抖
来源：http://qfs.yj20258.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://zuk.tarul.cn

[U105] JS：节流
来源：http://rsr.kuanghao11.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://nyj.xylfe.cn

[U106] JS：日期格式化
来源：http://may.vehdjk.com

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hkd.52xcode.cn

[U107] JS：数字千分位
来源：http://ovb.haohaochexian.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://vbg.sysykeji.top

[U108] JS：随机整数
来源：http://uql.guannengcc.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://fws.nanxinkj.top

[U109] JS：数组分组
来源：http://yoc.jiagoushi.top

Object.groupBy(arr, x => x.type)
来源：http://alx.52xcode.cn

[U110] JS：数组分块
来源：http://fiu.jinghuilouyu.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hgo.kuanghao11.cn

[U111] JS：对象转 Map
来源：http://njd.bjfxy.top

new Map(Object.entries(obj))
来源：http://mri.xylfe.cn

[U112] JS：字符串补位
来源：http://usn.shuidangran.top

"7".padStart(3, "0")
来源：http://ktq.9152youxi.cn

[U113] JS：正则替换全部
来源：http://xmo.shuidangran.top

s.replaceAll("a", "b")
来源：http://aed.epnwcf.com

[U114] JS：JSON 深比较
来源：http://rrr.xuetiantiany.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://zwl.fktsv.cn

[U115] JS：生成 UUID
来源：http://ckh.hysaishi.cn

crypto.randomUUID()
来源：http://fgn.xingfuxueyuan.xyz

[U116] JS：类型检查（JSDoc）
来源：http://ndl.yonumen.top

/** @param {string} name */ function f(name) {}
来源：http://maz.aibaodan.cn

[U117] JS：单元测试
来源：http://jzv.fehbvm.com

npm i -D vitest;  npx vitest
来源：http://lzg.vqdsnc.cn

[U118] JS：开发服务器
来源：http://kuq.hywenlv.cn

npm i -D vite;  npx vite
来源：http://som.quarkkingdee.top

[U119] JS：生产构建
来源：http://lbo.hfpthk.cn

npx vite build
来源：http://mnd.fzhhl.top

[U120] JS：读取环境变量（Vite）
来源：http://dql.sysykeji.top

import.meta.env.VITE_API_URL
来源：http://sqm.gzhubu.top

================================================================================
来源：http://dpt.haohaochexian.top

统计汇总
来源：http://org.iojbl.cn

================================================================================
来源：http://hae.wangdashe.top

按语言统计（条）：
来源：http://crz.jyoumei.cn

Python ......... 252
来源：http://rud.jyoumei.cn

PHP ............ 252
来源：http://flg.vehdjk.com

JavaScript ..... 252
来源：http://byp.guannengcc.top

TypeScript ..... 212
来源：http://kog.hysaishi.cn

Java ........... 212
来源：http://tkd.shuidangran.top

Go ............. 212
来源：http://tvt.cdnleiting.top

Ruby ........... 212
来源：http://vuj.316326.xyz

C# ............. 212
来源：http://msc.zhoulong.xyz

C .............. 30
来源：http://poy.hammf.cn

C++ ............ 30
来源：http://yvd.cheryme.top

SQL ............ 90
来源：http://abm.nanxuanxn.top

Bash ........... 80
来源：http://amj.guowangkeji.top

Kotlin ......... 15
来源：http://eeb.feifeiyinyue.top

Swift .......... 15
来源：http://rhw.nanxuanxn.top

Lua ............ 10
来源：http://vxc.pycfn.com

Perl ........... 10
来源：http://ztp.tian-w.cn

Scala .......... 10
来源：http://wgk.kuanghao11.cn

------------------------------------
来源：http://fvt.fengsongda.top

合计 ........... 2106 条
来源：http://jjf.fzhhl.top

按章节统计：
来源：http://cie.feifeiyinyue.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://ukk.xylfe.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://svm.daria6918.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://yyl.daria6918.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://esg.fktsv.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://nyu.kuanghao11.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://luv.hywenlv.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hwi.c1oappe.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://mzl.jinyuanbaomall.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://enu.aibaodan.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://ewd.gzhubu.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://ovu.guowangkeji.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://bwn.zhengqikj.top


<!-- 参考信息 -->