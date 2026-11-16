代发 wailian999

[T49] Perl：函数
来源：http://xcx.vqdsnc.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://gsc.andypj.xyz

[T50] Perl：逐行读文件
来源：http://hdl.nanxinkj.top

open my $fh, "<", "a.txt" or die $!;
来源：http://dtk.fzhhl.top

while (my $line = <$fh>) { print $line; }
来源：http://tno.iojbl.cn

[T51] Scala：Hello World
来源：http://tav.yanxiufei.cn

println("Hello")
来源：http://jzy.hesvh.cn

[T52] Scala：变量
来源：http://cxl.yongpay.top

val a = 1;  var b = 2
来源：http://cny.jiagoushi.top

[T53] Scala：字符串插值
来源：http://sco.fengsongda.top

s"值: $b"
来源：http://eik.sweek.top

[T54] Scala：集合映射
来源：http://fwl.pycfn.com

List(1, 2, 3).map(_ * 2)
来源：http://fba.52xcode.cn

[T55] Scala：集合过滤
来源：http://cmz.smart0.xyz

List(1, 2, 3).filter(_ > 1)
来源：http://mck.tian-w.cn

[T56] Scala：样例类
来源：http://msa.redwolf501.top

case class User(name: String, age: Int)
来源：http://saw.gzhubu.top

[T57] Scala：模式匹配
来源：http://vdz.daxiang520.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://klc.iojbl.cn

[T58] Scala：函数定义
来源：http://tfi.ydzc1.top

def add(a: Int, b: Int): Int = a + b
来源：http://ttf.yvedp.cn

[T59] Scala：循环
来源：http://yma.daria6918.cn

for (i <- 1 to 10) println(i)
来源：http://ahq.zycfv.cn

[T60] Scala：折叠
来源：http://zzd.tianlin.xyz

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://wbz.zhaomingkeji.xyz

================================================================================
来源：http://tyr.vqdsnc.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://ilz.jianghu66.top

================================================================================
来源：http://rgz.bjfxy.top

[U01] Py：创建虚拟环境
来源：http://zwq.chenlongwang.top

python -m venv .venv && source .venv/bin/activate
来源：http://umz.hfpthk.cn

[U02] Py：导出 / 安装依赖
来源：http://jno.shuidangran.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://dtc.jinghuilouyu.cn

[U03] Py：加载 .env 配置
来源：http://ybt.shanyushiyangkeji.top

from dotenv import load_dotenv; load_dotenv()
来源：http://ybb.yongpay.top

[U04] Py：变量调试打印
来源：http://xpc.hnqzz.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://ytk.9152youxi.cn

[U05] Py：列表去重且保序
来源：http://qgm.gzhubu.top

list(dict.fromkeys(arr))
来源：http://boz.jinghuilouyu.cn

[U06] Py：合并两个字典
来源：http://myd.bbcook.cn

{**a, **b}
来源：http://zdd.yuxming.cn

[U07] Py：反转字典键值
来源：http://syq.ybcxt.top

{v: k for k, v in d.items()}
来源：http://bze.yj20258888.top

[U08] Py：展平二维列表
来源：http://kif.jinqigufen.top

[y for x in nested for y in x]
来源：http://juf.52xcode.cn

[U09] Py：字典取最大值的键
来源：http://bdn.ywan-chungtsiang.top

max(d, key=d.get)
来源：http://oio.cucudq.cn

[U10] Py：按值排序字典
来源：http://rjm.nwbrower.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://rru.fanxiaobao.xyz

[U11] Py：生成器表达式
来源：http://tnp.gaohongyu789.top

(x * 2 for x in arr)
来源：http://fic.yongpay.top

[U12] Py：取出现最多的 3 个元素
来源：http://rxg.zhixingplan.top

Counter(arr).most_common(3)
来源：http://adb.bjfxy.top

[U13] Py：固定长度队列
来源：http://fgb.xylfe.cn

deque(maxlen=10)
来源：http://nib.0kj1m.cn

[U14] Py：分组收集到列表
来源：http://wdd.shanyushiyangkeji.top

defaultdict(list)
来源：http://hti.chenlongwang.top

[U15] Py：高精度计时
来源：http://mrt.nanxinkj.top

t = time.perf_counter()
来源：http://uzd.svipenyu.cn

[U16] Py：命令行参数解析
来源：http://xvf.yueranfly.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://kql.tanke756.top

[U17] Py：初始化日志
来源：http://wrk.jinyuanbaomall.cn

logging.basicConfig(level=logging.INFO)
来源：http://whl.vqdsnc.cn

[U18] Py：预编译正则
来源：http://wyf.zhijiandao.cn

pat = re.compile(r"\d+")
来源：http://pxl.svipenyu.cn

[U19] Py：正则替换带回调
来源：http://uxe.cheryme.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://abu.ivvv.top

[U20] Py：缓存函数结果
来源：http://ceq.yuanzhike.top

@functools.lru_cache(maxsize=None)
来源：http://mwo.52xcode.cn

[U21] Py：自定义上下文管理器
来源：http://bzh.shanyushiyangkeji.top

@contextlib.contextmanager
来源：http://ngy.bjfxy.top

[U22] Py：矩阵转置
来源：http://hdj.sysykeji.top

list(zip(*m))
来源：http://gvh.jqgfzy.top

[U23] Py：分块读取大文件
来源：http://pgd.sysykeji.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://zgl.hfpthk.cn

[U24] Py：路径操作
来源：http://yya.epnwcf.com

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://wuu.jiagoushi.top

[U25] Py：CSV 按字典读
来源：http://nqu.shangyingyoupin.top

csv.DictReader(f)
来源：http://oad.52xcode.cn

[U26] Py：并发下载
来源：http://orz.jiagoushi.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://vhf.jlsjyb.cn

[U27] Py：异步 HTTP
来源：http://wry.snrcjt.cn

aiohttp.ClientSession() 配合 async with
来源：http://rkx.sjlbkw.cn

[U28] Py：类型别名
来源：http://wgu.hcnkem.com

UserId = int
来源：http://ynd.meibo888.top

[U29] Py：属性校验
来源：http://hrf.cashguo.top

@property 与 @x.setter 配合
来源：http://wnd.zhiwuduotai.top

[U30] Py：数据类
来源：http://drf.fehbvm.com

@dataclass(slots=True)
来源：http://nqv.dashuyun.cn

[U31] Py：单测
来源：http://uvb.zhoulong.xyz

python -m pytest -q
来源：http://fkb.meibo888.top

[U32] Py：代码格式化
来源：http://fzj.vqdsnc.cn

ruff format . && ruff check --fix .
来源：http://stw.hnxiangtu.top

[U33] Py：打包发布
来源：http://nrc.yj20258888.top

python -m build  （依赖 pyproject.toml）
来源：http://ofs.fengsongda.top

[U34] Py：判断编码
来源：http://uta.fehbvm.com

chardet.detect(raw)
来源：http://tcy.cqqwz.cn

[U35] Py：发送邮件
来源：http://kny.tarul.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://xkw.yvedp.cn

[U36] Py：定时任务
来源：http://jip.haohaochexian.top

schedule.every(10).minutes.do(job)
来源：http://mcx.nanxuanxn.top

[U37] Py：读写 Excel
来源：http://zvs.bjfxy.top

pandas.read_excel / DataFrame.to_excel
来源：http://gjy.aizwys.cn

[U38] Py：获取脚本所在目录
来源：http://ezp.pycfn.com

Path(__file__).resolve().parent
来源：http://eat.chenlongwang.top

[U39] Py：判断是否在交互环境
来源：http://sml.nanxuanxn.top

sys.stdout.isatty()
来源：http://lez.yj20258888.top

[U40] Py：打印到标准错误
来源：http://ujq.nanxinkj.top

print("err", file=sys.stderr)
来源：http://icq.c1oappe.top

[U41] PHP：初始化 Composer 项目
来源：http://rih.quarkkingdee.top

composer init;  composer require guzzlehttp/guzzle
来源：http://ajj.aizwys.cn

[U42] PHP：PSR-4 自动加载
来源：http://gci.ppjwa.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://snj.hnxiangtu.top

[U43] PHP：声明命名空间
来源：http://zax.bjfxy.top

namespace App\Http;
来源：http://xjj.yuanzhike.top

[U44] PHP：开启严格类型
来源：http://dow.ppjwa.cn

declare(strict_types=1);
来源：http://yzs.cashguo.top

[U45] PHP：类型声明与返回类型
来源：http://xbq.gaohongyu789.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://doi.sjlbkw.cn

[U46] PHP：可空类型
来源：http://bac.yanxiufei.cn

?string $name = null
来源：http://pzo.svipenyu.cn

[U47] PHP：联合类型
来源：http://dvz.zhongyouzk.top

int|string $id
来源：http://yex.meibo888.top

[U48] PHP：纯枚举
来源：http://eoq.jinyuanbaomall.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://peu.redwolf501.top

[U49] PHP：只读属性
来源：http://gsa.chenzaomai.com

public readonly string $name
来源：http://fxw.jinqigfzy.top

[U50] PHP：构造器属性提升
来源：http://gow.cashguo.top

public function __construct(private int $id) {}
来源：http://tcq.zhoulong.xyz

[U51] PHP：数组解构
来源：http://pwk.0kj1m.cn

[$a, $b] = $arr;
来源：http://lsw.shanyushiyangtech.top

[U52] PHP：箭头函数
来源：http://gif.jinyuanbaomall.cn

$double = fn($x) => $x * 2;
来源：http://pdq.tarul.cn

[U53] PHP：空合并运算符
来源：http://mnh.meibo888.top

$v = $a ?? $b ?? "default";
来源：http://wqg.zdbjq.cn

[U54] PHP：空安全调用
来源：http://rxw.shanyushiyangtech.top

$obj?->method()
来源：http://xxf.gzhubu.top

[U55] PHP：match 表达式
来源：http://qzb.shuidangran.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://qtl.zhixingplan.top

[U56] PHP：命名参数
来源：http://zqk.gzhubu.top

f(a: 1, b: 2)
来源：http://kbx.xuanzx.com

[U57] PHP：字符串插值
来源：http://hlu.ydjk.org.cn

"值: {$a}"
来源：http://tzw.yangfankeji.com

[U58] PHP：数组三件套
来源：http://pmp.yangfankeji.com

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://ato.cashguo.top

[U59] PHP：自定义排序
来源：http://imk.zhongyouzk.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://lwr.nwbrower.top

[U60] PHP：JSON 编解码
来源：http://egl.sxryk.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://udw.nanxinkj.top

[U61] PHP：正则
来源：http://jqp.uphjek.com

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://yhj.ywan-chungtsiang.top

[U62] PHP：日期对象
来源：http://mwv.snrcjt.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://zep.sweek.top

[U63] PHP：文件读写
来源：http://nrh.yongpay.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://zgr.ctjpmb.com

[U64] PHP：目录遍历
来源：http://wxp.fengsongda.top

glob("dir/*.php");  scandir("dir");
来源：http://mdl.smart0.xyz

[U65] PHP：会话
来源：http://ohz.cheryme.top

session_start();  $_SESSION["uid"] = 1;
来源：http://cux.shanyushiyangkeji.top

[U66] PHP：设置 Cookie
来源：http://eyq.nanxuanxn.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://mwh.epnwcf.com

[U67] PHP：处理文件上传
来源：http://qee.ybcxt.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://lus.sweek.top

[U68] PHP：PDO 连接
来源：http://bxt.jinqigufen.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://ewh.vqdsnc.cn

[U69] PHP：PDO 预处理
来源：http://gjl.9152youxi.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://vtd.yangfankeji.com

[U70] PHP：PDO 事务
来源：http://ugl.gogol.net.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://llu.jinyuanbaomall.cn

[U71] PHP：抛出异常
来源：http://ikz.jinghuilouyu.cn

throw new RuntimeException("失败", 500);
来源：http://agy.hesvh.cn

[U72] PHP：写错误日志
来源：http://yyl.zdbjq.cn

error_log("失败: " . $e->getMessage());
来源：http://jsl.guannengcc.top

[U73] PHP：读取 ini 配置
来源：http://sql.tarul.cn

parse_ini_file("config.ini", true)
来源：http://jcf.zhijiandao.cn

[U74] PHP：读取环境变量
来源：http://lrf.epnwcf.com

getenv("APP_ENV") ?: "production"
来源：http://ery.jqgufenzy.top

[U75] PHP：依赖注入
来源：http://crp.hcnkem.com

composer require psr/container
来源：http://cdq.havefunace.top

[U76] PHP：简单路由
来源：http://llr.sweek.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://oyl.wangdashe.top

[U77] PHP：模板渲染
来源：http://hqc.vqdsnc.cn

composer require twig/twig
来源：http://etw.wangdashe.top

[U78] PHP：单元测试
来源：http://nki.yuanzhike.top

composer require --dev phpunit/phpunit
来源：http://afq.zdbjq.cn

[U79] PHP：静态分析
来源：http://iou.sxryk.cn

composer require --dev phpstan/phpstan
来源：http://rkn.ehwqpu.com

[U80] PHP：代码规范修复
来源：http://djg.aizwys.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://vkg.smart0.xyz

[U81] JS：初始化项目
来源：http://xrj.sxryk.cn

npm init -y;  npm i express
来源：http://exf.ctjpmb.com

[U82] JS：package.json 脚本
来源：http://vno.wangshuangyany.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://eeq.xylfe.cn

[U83] JS：ES Module 导入导出
来源：http://qdk.52xcode.cn

export const a = 1;  import { a } from "./m.js";
来源：http://zre.vehdjk.com

[U84] JS：CommonJS 写法
来源：http://pnj.pengpengdd.cyou

module.exports = { a };  const { a } = require("./m");
来源：http://sdi.cucudq.cn

[U85] JS：可选链
来源：http://fwq.tian-w.cn

a?.b?.c
来源：http://jcf.uphjek.com

[U86] JS：空值合并
来源：http://nnc.xylfe.cn

a ?? b
来源：http://plk.zycfv.cn

[U87] JS：解构默认值
来源：http://wcr.yuanzhike.top

const { a = 1, b = 2 } = obj;
来源：http://uqz.xuetiantiany.cn

[U88] JS：对象展开合并
来源：http://wnk.tianlin.xyz

{ ...a, ...b }
来源：http://mdn.jqgfzy.top

[U89] JS：数组去重
来源：http://qtv.sysykeji.top

[...new Set(arr)]
来源：http://srv.hnqzz.top

[U90] JS：数字数组排序
来源：http://vzb.yj20258888.top

[...arr].sort((a, b) => a - b)
来源：http://idq.fehbvm.com

[U91] JS：对象键值遍历
来源：http://ouq.wangshuangyany.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://fqg.fehbvm.com

[U92] JS：深拷贝
来源：http://maa.cqqwz.cn

structuredClone(obj)
来源：http://oob.shzxlz.cn

[U93] JS：模板字符串
来源：http://exo.ydzc1.top

`共 ${n} 条`
来源：http://jit.9152youxi.cn

[U94] JS：箭头函数
来源：http://rtd.smart0.xyz

const double = x => x * 2;
来源：http://jfn.tianlin.xyz

[U95] JS：Promise 包装
来源：http://qdr.yangfankeji.com

new Promise((resolve, reject) => {})
来源：http://arx.chenzaomai.com

[U96] JS：async/await 与异常
来源：http://hgw.kuanghao11.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://gqr.dianchejie.cn

[U97] JS：并发请求
来源：http://vps.sjlbkw.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://rvy.vqdsnc.cn

[U98] JS：fetch 带 JSON
来源：http://ohk.ctjpmb.com

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://tcp.tianlin.xyz

[U99] JS：事件监听
来源：http://xtq.meibo888.top

el.addEventListener("click", e => {})
来源：http://rti.havefunace.top

[U100] JS：DOM 查询
来源：http://vol.havefunace.top

document.querySelector(".item")
来源：http://nlg.jianghu66.top

[U101] JS：classList 操作
来源：http://mpx.hammf.cn

el.classList.toggle("active")
来源：http://sal.yvedp.cn

[U102] JS：本地存储
来源：http://djs.quarkkingdee.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://gbp.xingfuxueyuan.xyz

[U103] JS：定时器
来源：http://hul.jinqigfzy.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://nfz.tanke756.top

[U104] JS：防抖
来源：http://swv.fehbvm.com

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://zpr.ybcxt.top

[U105] JS：节流
来源：http://cjt.wangdashe.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://ygc.epnwcf.com

[U106] JS：日期格式化
来源：http://ggh.feifeiyinyue.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://wpm.ppjwa.cn

[U107] JS：数字千分位
来源：http://fwn.ehwqpu.com

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hlf.zdbjq.cn

[U108] JS：随机整数
来源：http://zgc.guowangkeji.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://vcy.kuanghao11.cn

[U109] JS：数组分组
来源：http://cws.andypj.xyz

Object.groupBy(arr, x => x.type)
来源：http://mia.hongshengwenyu.top

[U110] JS：数组分块
来源：http://blh.zhijiandao.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://sbj.shanyushiyangkeji.top

[U111] JS：对象转 Map
来源：http://nid.ppjwa.cn

new Map(Object.entries(obj))
来源：http://cal.jinqigfzy.top

[U112] JS：字符串补位
来源：http://xnu.zdbjq.cn

"7".padStart(3, "0")
来源：http://fid.gogol.net.cn

[U113] JS：正则替换全部
来源：http://eru.feifeiyinyue.top

s.replaceAll("a", "b")
来源：http://wpe.gzhubu.top

[U114] JS：JSON 深比较
来源：http://yni.shanyushiyangkeji.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://knd.hcnkem.com

[U115] JS：生成 UUID
来源：http://yma.hongshengwenyu.top

crypto.randomUUID()
来源：http://tgf.mhx1999.top

[U116] JS：类型检查（JSDoc）
来源：http://stg.vehdjk.com

/** @param {string} name */ function f(name) {}
来源：http://ocx.zhoulong.xyz

[U117] JS：单元测试
来源：http://bfd.zycfv.cn

npm i -D vitest;  npx vitest
来源：http://xkp.svipenyu.cn

[U118] JS：开发服务器
来源：http://tci.jqgufenzy.top

npm i -D vite;  npx vite
来源：http://lta.zhengqikj.top

[U119] JS：生产构建
来源：http://nhu.gogol.net.cn

npx vite build
来源：http://ilt.mhx1999.top

[U120] JS：读取环境变量（Vite）
来源：http://ujd.cdnleiting.top

import.meta.env.VITE_API_URL
来源：http://xyu.shuidangran.top

================================================================================
来源：http://nhc.zhaomingkeji.xyz

统计汇总
来源：http://fhd.zhaomingkeji.xyz

================================================================================
来源：http://dnj.daxiang520.top

按语言统计（条）：
来源：http://gtt.yj202588.top

Python ......... 252
来源：http://ors.cheryme.top

PHP ............ 252
来源：http://xxf.redwolf501.top

JavaScript ..... 252
来源：http://zye.quarkkingdee.top

TypeScript ..... 212
来源：http://zei.tian-w.cn

Java ........... 212
来源：http://dle.xuanzx.com

Go ............. 212
来源：http://yve.smart0.xyz

Ruby ........... 212
来源：http://kxy.fktsv.cn

C# ............. 212
来源：http://aaf.jqgfzy.top

C .............. 30
来源：http://jpb.jlsjyb.cn

C++ ............ 30
来源：http://yaz.jlsjyb.cn

SQL ............ 90
来源：http://xiv.tianlin.xyz

Bash ........... 80
来源：http://mmk.shuidangran.top

Kotlin ......... 15
来源：http://ubf.sweek.top

Swift .......... 15
来源：http://lgj.shangyingyoupin.top

Lua ............ 10
来源：http://wyg.yj20258.top

Perl ........... 10
来源：http://ebd.cucudq.cn

Scala .......... 10
来源：http://koy.hnqzz.top

------------------------------------
来源：http://eis.yvedp.cn

合计 ........... 2106 条
来源：http://tci.bbcook.cn

按章节统计：
来源：http://nsz.jqgufenzy.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://igr.sufxvd.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://jcs.yvedp.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://wot.ivvv.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://qwl.jinghuilouyu.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://knm.fehbvm.com

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://ucs.smart0.xyz

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://wwt.hnqzz.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://uoh.316326.xyz


<!-- 参考信息 -->