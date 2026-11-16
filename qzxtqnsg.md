代发 wailian999

[T49] Perl：函数
来源：http://iaa.hywenlv.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://dps.havefunace.top

[T50] Perl：逐行读文件
来源：http://tbu.gaohongyu789.top

open my $fh, "<", "a.txt" or die $!;
来源：http://btm.iojbl.cn

while (my $line = <$fh>) { print $line; }
来源：http://cve.yongpay.top

[T51] Scala：Hello World
来源：http://yvk.pycfn.com

println("Hello")
来源：http://ogj.ywan-chungtsiang.top

[T52] Scala：变量
来源：http://mbh.ivvv.top

val a = 1;  var b = 2
来源：http://lxh.yonumen.top

[T53] Scala：字符串插值
来源：http://dgt.hysaishi.cn

s"值: $b"
来源：http://dhe.zhiwuduotai.top

[T54] Scala：集合映射
来源：http://hls.hnqzz.top

List(1, 2, 3).map(_ * 2)
来源：http://vkz.guowangkeji.top

[T55] Scala：集合过滤
来源：http://xgl.hfpthk.cn

List(1, 2, 3).filter(_ > 1)
来源：http://nyu.yvedp.cn

[T56] Scala：样例类
来源：http://shc.bbcook.cn

case class User(name: String, age: Int)
来源：http://glr.mhx1999.top

[T57] Scala：模式匹配
来源：http://cky.gaohongyu789.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://zlq.hcnkem.com

[T58] Scala：函数定义
来源：http://hvu.hfpthk.cn

def add(a: Int, b: Int): Int = a + b
来源：http://cpj.ppjwa.cn

[T59] Scala：循环
来源：http://jxc.zhongyouzk.top

for (i <- 1 to 10) println(i)
来源：http://udt.yueranfly.top

[T60] Scala：折叠
来源：http://tol.yj202588.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://zul.epnwcf.com

================================================================================
来源：http://pqt.shuidangran.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://gnz.smart0.xyz

================================================================================
来源：http://esl.sysykeji.top

[U01] Py：创建虚拟环境
来源：http://hha.yj202588.top

python -m venv .venv && source .venv/bin/activate
来源：http://stu.chenjidiqi.icu

[U02] Py：导出 / 安装依赖
来源：http://lhk.yongpay.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://squ.tanke756.top

[U03] Py：加载 .env 配置
来源：http://fwa.ivvv.top

from dotenv import load_dotenv; load_dotenv()
来源：http://wht.andypj.xyz

[U04] Py：变量调试打印
来源：http://uwz.0kj1m.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://oja.hnxiangtu.top

[U05] Py：列表去重且保序
来源：http://qgt.daxiang520.top

list(dict.fromkeys(arr))
来源：http://gin.ydzc1.top

[U06] Py：合并两个字典
来源：http://dpd.zycfv.cn

{**a, **b}
来源：http://dci.ctjpmb.com

[U07] Py：反转字典键值
来源：http://krz.zhengqikj.top

{v: k for k, v in d.items()}
来源：http://rmp.xylfe.cn

[U08] Py：展平二维列表
来源：http://mua.uphjek.com

[y for x in nested for y in x]
来源：http://kfg.fehbvm.com

[U09] Py：字典取最大值的键
来源：http://mcw.vqdsnc.cn

max(d, key=d.get)
来源：http://drm.xziqi.cn

[U10] Py：按值排序字典
来源：http://ilw.ppjwa.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://dkw.ywan-chungtsiang.top

[U11] Py：生成器表达式
来源：http://kbp.fzhhl.top

(x * 2 for x in arr)
来源：http://cew.shanyushiyangkeji.top

[U12] Py：取出现最多的 3 个元素
来源：http://rst.shzxlz.cn

Counter(arr).most_common(3)
来源：http://ewi.yuanzhike.top

[U13] Py：固定长度队列
来源：http://zvr.tarul.cn

deque(maxlen=10)
来源：http://lzq.hnqzz.top

[U14] Py：分组收集到列表
来源：http://rkz.gogol.net.cn

defaultdict(list)
来源：http://bmn.hnqzz.top

[U15] Py：高精度计时
来源：http://oyb.nwbrower.top

t = time.perf_counter()
来源：http://fbs.jqgufenzy.top

[U16] Py：命令行参数解析
来源：http://zbe.xinyue.icu

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://csg.zhijiandao.cn

[U17] Py：初始化日志
来源：http://xyw.gotoacloud.top

logging.basicConfig(level=logging.INFO)
来源：http://cwi.smart0.xyz

[U18] Py：预编译正则
来源：http://qxp.hcnkem.com

pat = re.compile(r"\d+")
来源：http://nvb.ehwqpu.com

[U19] Py：正则替换带回调
来源：http://fxv.tian-w.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://nef.mhx1999.top

[U20] Py：缓存函数结果
来源：http://wjl.jinghuilouyu.cn

@functools.lru_cache(maxsize=None)
来源：http://vrv.guannengcc.top

[U21] Py：自定义上下文管理器
来源：http://niz.yongpay.top

@contextlib.contextmanager
来源：http://vcs.guowangkeji.top

[U22] Py：矩阵转置
来源：http://dhm.yuxming.cn

list(zip(*m))
来源：http://svz.svipenyu.cn

[U23] Py：分块读取大文件
来源：http://ora.zhiwuduotai.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://leh.wangshuangyany.cn

[U24] Py：路径操作
来源：http://qmj.dashuyun.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://pie.dashuyun.cn

[U25] Py：CSV 按字典读
来源：http://kur.ppjwa.cn

csv.DictReader(f)
来源：http://qvk.vehdjk.com

[U26] Py：并发下载
来源：http://kps.sxryk.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://fvi.havefunace.top

[U27] Py：异步 HTTP
来源：http://jgf.xuetiantiany.cn

aiohttp.ClientSession() 配合 async with
来源：http://jer.chenzaomai.com

[U28] Py：类型别名
来源：http://zyl.ctjpmb.com

UserId = int
来源：http://igu.jlsjyb.cn

[U29] Py：属性校验
来源：http://juz.havefunace.top

@property 与 @x.setter 配合
来源：http://kft.c1oappe.top

[U30] Py：数据类
来源：http://osk.vehdjk.com

@dataclass(slots=True)
来源：http://wwd.pengpengdd.cyou

[U31] Py：单测
来源：http://uyi.sjlbkw.cn

python -m pytest -q
来源：http://ajr.chenjidiqi.icu

[U32] Py：代码格式化
来源：http://ptk.sweek.top

ruff format . && ruff check --fix .
来源：http://nmd.c1oappe.top

[U33] Py：打包发布
来源：http://jxt.sjlbkw.cn

python -m build  （依赖 pyproject.toml）
来源：http://sbe.yj20258888.top

[U34] Py：判断编码
来源：http://ozd.chenlongwang.top

chardet.detect(raw)
来源：http://nlc.316326.xyz

[U35] Py：发送邮件
来源：http://qcy.gzhubu.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://wfs.svipenyu.cn

[U36] Py：定时任务
来源：http://vaw.sweek.top

schedule.every(10).minutes.do(job)
来源：http://mil.vqdsnc.cn

[U37] Py：读写 Excel
来源：http://tbg.dashuyun.cn

pandas.read_excel / DataFrame.to_excel
来源：http://fky.gaohongyu789.top

[U38] Py：获取脚本所在目录
来源：http://anv.ybcxt.top

Path(__file__).resolve().parent
来源：http://dmg.yanxiufei.cn

[U39] Py：判断是否在交互环境
来源：http://obl.0kj1m.cn

sys.stdout.isatty()
来源：http://yfs.fehbvm.com

[U40] Py：打印到标准错误
来源：http://lkg.pengpengdd.cyou

print("err", file=sys.stderr)
来源：http://dmb.ctjpmb.com

[U41] PHP：初始化 Composer 项目
来源：http://cum.fanxiaobao.xyz

composer init;  composer require guzzlehttp/guzzle
来源：http://zkr.jqgfzy.top

[U42] PHP：PSR-4 自动加载
来源：http://ozc.ydjk.org.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://yhd.xuanzx.com

[U43] PHP：声明命名空间
来源：http://ogb.yanxiufei.cn

namespace App\Http;
来源：http://lox.yanxiufei.cn

[U44] PHP：开启严格类型
来源：http://hdd.cashguo.top

declare(strict_types=1);
来源：http://lop.kuanghao11.cn

[U45] PHP：类型声明与返回类型
来源：http://fbb.ppjwa.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://yph.yj20258.top

[U46] PHP：可空类型
来源：http://yhc.wangshuangyany.cn

?string $name = null
来源：http://ehy.ydzc1.top

[U47] PHP：联合类型
来源：http://uwc.gzhubu.top

int|string $id
来源：http://ccb.hysaishi.cn

[U48] PHP：纯枚举
来源：http://diy.tianlin.xyz

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://vgd.nanxinkj.top

[U49] PHP：只读属性
来源：http://jyc.smart0.xyz

public readonly string $name
来源：http://sjo.iojbl.cn

[U50] PHP：构造器属性提升
来源：http://hjy.hcnkem.com

public function __construct(private int $id) {}
来源：http://mir.sysykeji.top

[U51] PHP：数组解构
来源：http://vlf.9152youxi.cn

[$a, $b] = $arr;
来源：http://sqc.dashuyun.cn

[U52] PHP：箭头函数
来源：http://aei.fengsongda.top

$double = fn($x) => $x * 2;
来源：http://zfp.tianlin.xyz

[U53] PHP：空合并运算符
来源：http://hfk.hongshengwenyu.top

$v = $a ?? $b ?? "default";
来源：http://tjb.yuanzhike.top

[U54] PHP：空安全调用
来源：http://ddp.haohaochexian.top

$obj?->method()
来源：http://oxk.jiagoushi.top

[U55] PHP：match 表达式
来源：http://lej.chenlongwang.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://add.zhiwuduotai.top

[U56] PHP：命名参数
来源：http://vnx.ehwqpu.com

f(a: 1, b: 2)
来源：http://tno.pycfn.com

[U57] PHP：字符串插值
来源：http://pjf.ctjpmb.com

"值: {$a}"
来源：http://ihl.yanxiufei.cn

[U58] PHP：数组三件套
来源：http://uer.haohaochexian.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://pds.snrcjt.cn

[U59] PHP：自定义排序
来源：http://dyq.haohaochexian.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://irn.cashguo.top

[U60] PHP：JSON 编解码
来源：http://mlz.redwolf501.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://wyy.tian-w.cn

[U61] PHP：正则
来源：http://xcc.ydjk.org.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://kgg.ydjk.org.cn

[U62] PHP：日期对象
来源：http://jqj.kuanghao11.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://ula.316326.xyz

[U63] PHP：文件读写
来源：http://cxb.hywenlv.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hke.ctjpmb.com

[U64] PHP：目录遍历
来源：http://xsu.nwbrower.top

glob("dir/*.php");  scandir("dir");
来源：http://cre.nwbrower.top

[U65] PHP：会话
来源：http://mts.jinghuilouyu.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://qew.gzhubu.top

[U66] PHP：设置 Cookie
来源：http://fus.ydzc1.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://osr.chenjidiqi.icu

[U67] PHP：处理文件上传
来源：http://qxl.redwolf501.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://edq.meibo888.top

[U68] PHP：PDO 连接
来源：http://qks.shzxlz.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://old.sysykeji.top

[U69] PHP：PDO 预处理
来源：http://vyq.havefunace.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://qpw.kuanghao11.cn

[U70] PHP：PDO 事务
来源：http://caq.zhijiandao.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://lxx.cheryme.top

[U71] PHP：抛出异常
来源：http://ixa.ivvv.top

throw new RuntimeException("失败", 500);
来源：http://vps.guannengcc.top

[U72] PHP：写错误日志
来源：http://lcl.quarkkingdee.top

error_log("失败: " . $e->getMessage());
来源：http://zun.hongshengwenyu.top

[U73] PHP：读取 ini 配置
来源：http://fuu.fktsv.cn

parse_ini_file("config.ini", true)
来源：http://rgj.quarkkingdee.top

[U74] PHP：读取环境变量
来源：http://rdr.redwolf501.top

getenv("APP_ENV") ?: "production"
来源：http://tzk.fzhhl.top

[U75] PHP：依赖注入
来源：http://cyi.gaohongyu789.top

composer require psr/container
来源：http://dev.52xcode.cn

[U76] PHP：简单路由
来源：http://zio.cqqwz.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://gvg.kuanghao11.cn

[U77] PHP：模板渲染
来源：http://ozu.guowangkeji.top

composer require twig/twig
来源：http://xgx.vqdsnc.cn

[U78] PHP：单元测试
来源：http://erv.hcnkem.com

composer require --dev phpunit/phpunit
来源：http://kzu.shzxlz.cn

[U79] PHP：静态分析
来源：http://diw.yvedp.cn

composer require --dev phpstan/phpstan
来源：http://opv.chenjidiqi.icu

[U80] PHP：代码规范修复
来源：http://esw.feifeiyinyue.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://sfw.chenlongwang.top

[U81] JS：初始化项目
来源：http://fxo.shanyushiyangtech.top

npm init -y;  npm i express
来源：http://ycu.hysaishi.cn

[U82] JS：package.json 脚本
来源：http://cdz.vehdjk.com

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://umf.hysaishi.cn

[U83] JS：ES Module 导入导出
来源：http://egd.0kj1m.cn

export const a = 1;  import { a } from "./m.js";
来源：http://sdj.meibo888.top

[U84] JS：CommonJS 写法
来源：http://cvt.aibaodan.cn

module.exports = { a };  const { a } = require("./m");
来源：http://cis.andypj.xyz

[U85] JS：可选链
来源：http://zlk.jlsjyb.cn

a?.b?.c
来源：http://fsj.sxryk.cn

[U86] JS：空值合并
来源：http://tup.ydzc1.top

a ?? b
来源：http://qhn.dashuyun.cn

[U87] JS：解构默认值
来源：http://wkv.ydzc1.top

const { a = 1, b = 2 } = obj;
来源：http://qwq.xuanzx.com

[U88] JS：对象展开合并
来源：http://tvt.xinyue.icu

{ ...a, ...b }
来源：http://ork.gzhubu.top

[U89] JS：数组去重
来源：http://ahn.chenjidiqi.icu

[...new Set(arr)]
来源：http://jdz.hfpthk.cn

[U90] JS：数字数组排序
来源：http://ryp.dashuyun.cn

[...arr].sort((a, b) => a - b)
来源：http://mnf.dashuyun.cn

[U91] JS：对象键值遍历
来源：http://mqr.tian-w.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://jox.fengsongda.top

[U92] JS：深拷贝
来源：http://xao.jqgufenzy.top

structuredClone(obj)
来源：http://wjn.bjfxy.top

[U93] JS：模板字符串
来源：http://zxt.hcnkem.com

`共 ${n} 条`
来源：http://fjn.shanyushiyangkeji.top

[U94] JS：箭头函数
来源：http://dzl.fengsongda.top

const double = x => x * 2;
来源：http://fas.tanke756.top

[U95] JS：Promise 包装
来源：http://hkw.fktsv.cn

new Promise((resolve, reject) => {})
来源：http://fdr.daria6918.cn

[U96] JS：async/await 与异常
来源：http://jit.zycfv.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://yya.wangshuangyany.cn

[U97] JS：并发请求
来源：http://xlj.ydjk.org.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://nny.daxiang520.top

[U98] JS：fetch 带 JSON
来源：http://bvj.zdbjq.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://eez.kuanghao11.cn

[U99] JS：事件监听
来源：http://rqu.yongpay.top

el.addEventListener("click", e => {})
来源：http://epa.jqgufenzy.top

[U100] JS：DOM 查询
来源：http://kuo.hcnkem.com

document.querySelector(".item")
来源：http://fti.jianghu66.top

[U101] JS：classList 操作
来源：http://egs.nwbrower.top

el.classList.toggle("active")
来源：http://uci.meibo888.top

[U102] JS：本地存储
来源：http://prr.bjfxy.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://nil.dianchejie.cn

[U103] JS：定时器
来源：http://ixl.cashguo.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://wyq.fzhhl.top

[U104] JS：防抖
来源：http://sne.guowangkeji.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://tks.jinyuanbaomall.cn

[U105] JS：节流
来源：http://vtj.havefunace.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://ieb.jlsjyb.cn

[U106] JS：日期格式化
来源：http://ppy.chenzaomai.com

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://rpy.shanyushiyangkeji.top

[U107] JS：数字千分位
来源：http://amw.sxryk.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://cfy.9152youxi.cn

[U108] JS：随机整数
来源：http://jqt.gaohongyu789.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://sxm.jyoumei.cn

[U109] JS：数组分组
来源：http://llh.sweek.top

Object.groupBy(arr, x => x.type)
来源：http://zes.yj202588.top

[U110] JS：数组分块
来源：http://ebk.jiagoushi.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://fqb.ehwqpu.com

[U111] JS：对象转 Map
来源：http://agc.xuetiantiany.cn

new Map(Object.entries(obj))
来源：http://fkz.gaohongyu789.top

[U112] JS：字符串补位
来源：http://kmo.mhx1999.top

"7".padStart(3, "0")
来源：http://zvk.aibaodan.cn

[U113] JS：正则替换全部
来源：http://nbu.sxryk.cn

s.replaceAll("a", "b")
来源：http://bol.0kj1m.cn

[U114] JS：JSON 深比较
来源：http://ggt.sjlbkw.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://lyo.quarkkingdee.top

[U115] JS：生成 UUID
来源：http://kkp.sufxvd.cn

crypto.randomUUID()
来源：http://nut.jiagoushi.top

[U116] JS：类型检查（JSDoc）
来源：http://loc.nanxinkj.top

/** @param {string} name */ function f(name) {}
来源：http://gzw.svipenyu.cn

[U117] JS：单元测试
来源：http://ert.0kj1m.cn

npm i -D vitest;  npx vitest
来源：http://vvc.ppjwa.cn

[U118] JS：开发服务器
来源：http://rbl.birdmap.top

npm i -D vite;  npx vite
来源：http://btv.zhongyouzk.top

[U119] JS：生产构建
来源：http://qvt.ydjk.org.cn

npx vite build
来源：http://vuv.jqgfzy.top

[U120] JS：读取环境变量（Vite）
来源：http://hco.hammf.cn

import.meta.env.VITE_API_URL
来源：http://cmj.jqgufenzy.top

================================================================================
来源：http://xiy.shanyushiyangkeji.top

统计汇总
来源：http://mcf.sysykeji.top

================================================================================
来源：http://jki.yanxiufei.cn

按语言统计（条）：
来源：http://rlf.ctjpmb.com

Python ......... 252
来源：http://mge.yj20258888.top

PHP ............ 252
来源：http://hmf.bjfxy.top

JavaScript ..... 252
来源：http://xba.yuanzhike.top

TypeScript ..... 212
来源：http://pcx.yongpay.top

Java ........... 212
来源：http://bge.chenlongwang.top

Go ............. 212
来源：http://mjc.xingfuxueyuan.xyz

Ruby ........... 212
来源：http://ehf.shuidangran.top

C# ............. 212
来源：http://atj.hammf.cn

C .............. 30
来源：http://mmh.ppjwa.cn

C++ ............ 30
来源：http://yhc.nanxuanxn.top

SQL ............ 90
来源：http://jis.sysykeji.top

Bash ........... 80
来源：http://hpc.yuxming.cn

Kotlin ......... 15
来源：http://fxx.jinghuilouyu.cn

Swift .......... 15
来源：http://qjy.jlsjyb.cn

Lua ............ 10
来源：http://igm.zhoulong.xyz

Perl ........... 10
来源：http://rpu.jinghuilouyu.cn

Scala .......... 10
来源：http://obh.yanxiufei.cn

------------------------------------
来源：http://khb.chenzaomai.com

合计 ........... 2106 条
来源：http://ljz.gogol.net.cn

按章节统计：
来源：http://agl.xylfe.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://unc.chenjidiqi.icu

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://yfn.hongshengwenyu.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://bwb.yj20258888.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://ixe.fengsongda.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://yqt.yongpay.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://ymc.jlsjyb.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://ufj.cheryme.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://mat.gotoacloud.top


<!-- 参考信息 -->