代发 wailian999

val a = 1;  var b = 2
来源：http://ten.meibo888.top

[T53] Scala：字符串插值
来源：http://pdf.cucudq.cn

s"值: $b"
来源：http://sqq.yangfankeji.com

[T54] Scala：集合映射
来源：http://xfp.xuanzx.com

List(1, 2, 3).map(_ * 2)
来源：http://waw.xuanzx.com

[T55] Scala：集合过滤
来源：http://iqr.nwbrower.top

List(1, 2, 3).filter(_ > 1)
来源：http://kpw.316326.xyz

[T56] Scala：样例类
来源：http://vby.iojbl.cn

case class User(name: String, age: Int)
来源：http://vqc.hcnkem.com

[T57] Scala：模式匹配
来源：http://bqi.yuanzhike.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://hmb.ppjwa.cn

[T58] Scala：函数定义
来源：http://lix.pengpengdd.cyou

def add(a: Int, b: Int): Int = a + b
来源：http://lrr.guowangkeji.top

[T59] Scala：循环
来源：http://npz.xinyue.icu

for (i <- 1 to 10) println(i)
来源：http://vlm.dashuyun.cn

[T60] Scala：折叠
来源：http://ihe.bjfxy.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://jis.ivvv.top

================================================================================
来源：http://qko.shzxlz.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://sku.yongpay.top

================================================================================
来源：http://ill.ppjwa.cn

[U01] Py：创建虚拟环境
来源：http://jqq.sysykeji.top

python -m venv .venv && source .venv/bin/activate
来源：http://cqn.haohaochexian.top

[U02] Py：导出 / 安装依赖
来源：http://tkk.xuetiantiany.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://imw.ivvv.top

[U03] Py：加载 .env 配置
来源：http://yiz.zhengqikj.top

from dotenv import load_dotenv; load_dotenv()
来源：http://lay.yuanzhike.top

[U04] Py：变量调试打印
来源：http://ygb.hcnkem.com

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://aii.quarkkingdee.top

[U05] Py：列表去重且保序
来源：http://zmg.hywenlv.cn

list(dict.fromkeys(arr))
来源：http://zou.yfazqb.com

[U06] Py：合并两个字典
来源：http://rbr.dianchejie.cn

{**a, **b}
来源：http://ewo.tarul.cn

[U07] Py：反转字典键值
来源：http://zki.redwolf501.top

{v: k for k, v in d.items()}
来源：http://ugz.xuetiantiany.cn

[U08] Py：展平二维列表
来源：http://jvd.gogol.net.cn

[y for x in nested for y in x]
来源：http://ive.9152youxi.cn

[U09] Py：字典取最大值的键
来源：http://rsx.zhengqikj.top

max(d, key=d.get)
来源：http://btm.zdqjudy.top

[U10] Py：按值排序字典
来源：http://ske.chenjidiqi.icu

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://vvc.pengpengdd.cyou

[U11] Py：生成器表达式
来源：http://tpp.hysaishi.cn

(x * 2 for x in arr)
来源：http://vas.daria6918.cn

[U12] Py：取出现最多的 3 个元素
来源：http://nlb.zycfv.cn

Counter(arr).most_common(3)
来源：http://rbc.ctjpmb.com

[U13] Py：固定长度队列
来源：http://hly.fktsv.cn

deque(maxlen=10)
来源：http://frq.nanxinkj.top

[U14] Py：分组收集到列表
来源：http://kjt.xylfe.cn

defaultdict(list)
来源：http://fin.yongpay.top

[U15] Py：高精度计时
来源：http://oms.kuanghao11.cn

t = time.perf_counter()
来源：http://olz.epnwcf.com

[U16] Py：命令行参数解析
来源：http://rkr.jqgufenzy.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://ivm.yanxiufei.cn

[U17] Py：初始化日志
来源：http://rkm.guannengcc.top

logging.basicConfig(level=logging.INFO)
来源：http://rbh.ivvv.top

[U18] Py：预编译正则
来源：http://ypv.gzhubu.top

pat = re.compile(r"\d+")
来源：http://dxh.fengsongda.top

[U19] Py：正则替换带回调
来源：http://dqu.hnqzz.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://kou.xylfe.cn

[U20] Py：缓存函数结果
来源：http://njv.xuetiantiany.cn

@functools.lru_cache(maxsize=None)
来源：http://res.zycfv.cn

[U21] Py：自定义上下文管理器
来源：http://qjd.wangdashe.top

@contextlib.contextmanager
来源：http://beg.pengpengdd.cyou

[U22] Py：矩阵转置
来源：http://bkm.cheryme.top

list(zip(*m))
来源：http://foe.jyoumei.cn

[U23] Py：分块读取大文件
来源：http://rih.pengpengdd.cyou

for chunk in iter(lambda: f.read(8192), b""):
来源：http://jsa.meibo888.top

[U24] Py：路径操作
来源：http://tqq.ivvv.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://qsf.dianchejie.cn

[U25] Py：CSV 按字典读
来源：http://ryy.shzxlz.cn

csv.DictReader(f)
来源：http://loz.bbcook.cn

[U26] Py：并发下载
来源：http://zst.shzxlz.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://zod.redwolf501.top

[U27] Py：异步 HTTP
来源：http://etf.nanxinkj.top

aiohttp.ClientSession() 配合 async with
来源：http://enb.zhijiandao.cn

[U28] Py：类型别名
来源：http://tcq.sufxvd.cn

UserId = int
来源：http://usq.ydjk.org.cn

[U29] Py：属性校验
来源：http://psv.jinyuanbaomall.cn

@property 与 @x.setter 配合
来源：http://xsr.9152youxi.cn

[U30] Py：数据类
来源：http://xrj.tanke756.top

@dataclass(slots=True)
来源：http://anb.jianghu66.top

[U31] Py：单测
来源：http://ohx.jinqigufen.top

python -m pytest -q
来源：http://smd.cqqwz.cn

[U32] Py：代码格式化
来源：http://cpu.9152youxi.cn

ruff format . && ruff check --fix .
来源：http://vcm.zdbjq.cn

[U33] Py：打包发布
来源：http://bbd.hongshengwenyu.top

python -m build  （依赖 pyproject.toml）
来源：http://cjp.chenlongwang.top

[U34] Py：判断编码
来源：http://pct.ywan-chungtsiang.top

chardet.detect(raw)
来源：http://qzg.zhoulong.xyz

[U35] Py：发送邮件
来源：http://fjv.hesvh.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://eaj.hcnkem.com

[U36] Py：定时任务
来源：http://ncx.cashguo.top

schedule.every(10).minutes.do(job)
来源：http://xcj.chenjidiqi.icu

[U37] Py：读写 Excel
来源：http://juu.shzxlz.cn

pandas.read_excel / DataFrame.to_excel
来源：http://zrp.yueranfly.top

[U38] Py：获取脚本所在目录
来源：http://fvk.hnqzz.top

Path(__file__).resolve().parent
来源：http://emk.vqdsnc.cn

[U39] Py：判断是否在交互环境
来源：http://pek.gotoacloud.top

sys.stdout.isatty()
来源：http://gqo.jinqigfzy.top

[U40] Py：打印到标准错误
来源：http://noa.ehwqpu.com

print("err", file=sys.stderr)
来源：http://irf.wangshuangyany.cn

[U41] PHP：初始化 Composer 项目
来源：http://jeq.jinqigfzy.top

composer init;  composer require guzzlehttp/guzzle
来源：http://qdt.sysykeji.top

[U42] PHP：PSR-4 自动加载
来源：http://ymu.kuanghao11.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://xvl.jinqigufen.top

[U43] PHP：声明命名空间
来源：http://dfi.aizwys.cn

namespace App\Http;
来源：http://nmw.wangshuangyany.cn

[U44] PHP：开启严格类型
来源：http://plk.sysykeji.top

declare(strict_types=1);
来源：http://szy.ydzc1.top

[U45] PHP：类型声明与返回类型
来源：http://puf.c1oappe.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://buc.tanke756.top

[U46] PHP：可空类型
来源：http://yvw.fanxiaobao.xyz

?string $name = null
来源：http://amr.ydjk.org.cn

[U47] PHP：联合类型
来源：http://bvn.kuanghao11.cn

int|string $id
来源：http://zse.cdnleiting.top

[U48] PHP：纯枚举
来源：http://xex.tarul.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://rls.guannengcc.top

[U49] PHP：只读属性
来源：http://lcd.shangyingyoupin.top

public readonly string $name
来源：http://fsn.sjlbkw.cn

[U50] PHP：构造器属性提升
来源：http://oqc.chenjidiqi.icu

public function __construct(private int $id) {}
来源：http://yvl.yj20258888.top

[U51] PHP：数组解构
来源：http://vwz.svipenyu.cn

[$a, $b] = $arr;
来源：http://oqu.sysykeji.top

[U52] PHP：箭头函数
来源：http://hzw.hnxiangtu.top

$double = fn($x) => $x * 2;
来源：http://bqn.fanxiaobao.xyz

[U53] PHP：空合并运算符
来源：http://ryj.chenlongwang.top

$v = $a ?? $b ?? "default";
来源：http://gsf.kuanghao11.cn

[U54] PHP：空安全调用
来源：http://cof.vqdsnc.cn

$obj?->method()
来源：http://ome.nanxinkj.top

[U55] PHP：match 表达式
来源：http://eyr.snrcjt.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://bul.xuetiantiany.cn

[U56] PHP：命名参数
来源：http://qxg.smart0.xyz

f(a: 1, b: 2)
来源：http://qsv.ctjpmb.com

[U57] PHP：字符串插值
来源：http://sms.ppjwa.cn

"值: {$a}"
来源：http://fvj.vehdjk.com

[U58] PHP：数组三件套
来源：http://hdo.jiagoushi.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://kia.fehbvm.com

[U59] PHP：自定义排序
来源：http://nkq.316326.xyz

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://pbv.yfazqb.com

[U60] PHP：JSON 编解码
来源：http://hki.ctjpmb.com

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://xlu.zhengqikj.top

[U61] PHP：正则
来源：http://pgn.hcnkem.com

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://vtp.gogol.net.cn

[U62] PHP：日期对象
来源：http://ofr.cucudq.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://gvk.redwolf501.top

[U63] PHP：文件读写
来源：http://koq.cdnleiting.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://zhj.jinyuanbaomall.cn

[U64] PHP：目录遍历
来源：http://ryy.jinqigfzy.top

glob("dir/*.php");  scandir("dir");
来源：http://dve.havefunace.top

[U65] PHP：会话
来源：http://wjo.wangdashe.top

session_start();  $_SESSION["uid"] = 1;
来源：http://dmg.jqgufenzy.top

[U66] PHP：设置 Cookie
来源：http://yyv.zhoulong.xyz

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://ceo.hywenlv.cn

[U67] PHP：处理文件上传
来源：http://pcv.yfazqb.com

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://yml.tarul.cn

[U68] PHP：PDO 连接
来源：http://acd.fengsongda.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://puf.yvedp.cn

[U69] PHP：PDO 预处理
来源：http://ble.gotoacloud.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://uuq.smart0.xyz

[U70] PHP：PDO 事务
来源：http://wwy.uphjek.com

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://yrz.dianchejie.cn

[U71] PHP：抛出异常
来源：http://afo.xinyue.icu

throw new RuntimeException("失败", 500);
来源：http://kpa.sxryk.cn

[U72] PHP：写错误日志
来源：http://lpb.316326.xyz

error_log("失败: " . $e->getMessage());
来源：http://jpq.wangshuangyany.cn

[U73] PHP：读取 ini 配置
来源：http://eqx.daxiang520.top

parse_ini_file("config.ini", true)
来源：http://umt.nwbrower.top

[U74] PHP：读取环境变量
来源：http://qpn.yj202588.top

getenv("APP_ENV") ?: "production"
来源：http://vgx.yj20258.top

[U75] PHP：依赖注入
来源：http://ihi.zhijiandao.cn

composer require psr/container
来源：http://peu.sufxvd.cn

[U76] PHP：简单路由
来源：http://uqu.yj202588.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://kzx.chenzaomai.com

[U77] PHP：模板渲染
来源：http://lfq.ivvv.top

composer require twig/twig
来源：http://pbx.fanxiaobao.xyz

[U78] PHP：单元测试
来源：http://vfq.hysaishi.cn

composer require --dev phpunit/phpunit
来源：http://vkc.cheryme.top

[U79] PHP：静态分析
来源：http://xrd.ydzc1.top

composer require --dev phpstan/phpstan
来源：http://tei.jqgufenzy.top

[U80] PHP：代码规范修复
来源：http://gki.jqgfzy.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://aoy.gotoacloud.top

[U81] JS：初始化项目
来源：http://fax.andypj.xyz

npm init -y;  npm i express
来源：http://kae.pengpengdd.cyou

[U82] JS：package.json 脚本
来源：http://vzh.sxryk.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://wii.shangyingyoupin.top

[U83] JS：ES Module 导入导出
来源：http://gfw.yueranfly.top

export const a = 1;  import { a } from "./m.js";
来源：http://gio.shuidangran.top

[U84] JS：CommonJS 写法
来源：http://ojb.zhoulong.xyz

module.exports = { a };  const { a } = require("./m");
来源：http://plz.bbcook.cn

[U85] JS：可选链
来源：http://err.feifeiyinyue.top

a?.b?.c
来源：http://apk.yuanzhike.top

[U86] JS：空值合并
来源：http://dnr.daxiang520.top

a ?? b
来源：http://ois.ehwqpu.com

[U87] JS：解构默认值
来源：http://api.cheryme.top

const { a = 1, b = 2 } = obj;
来源：http://eud.hammf.cn

[U88] JS：对象展开合并
来源：http://wls.ehwqpu.com

{ ...a, ...b }
来源：http://yvq.yonumen.top

[U89] JS：数组去重
来源：http://dfk.zhaomingkeji.xyz

[...new Set(arr)]
来源：http://jxb.tanke756.top

[U90] JS：数字数组排序
来源：http://jjv.iojbl.cn

[...arr].sort((a, b) => a - b)
来源：http://hsd.fehbvm.com

[U91] JS：对象键值遍历
来源：http://hos.fehbvm.com

Object.entries(obj).forEach(([k, v]) => {});
来源：http://syo.zhoulong.xyz

[U92] JS：深拷贝
来源：http://tub.xylfe.cn

structuredClone(obj)
来源：http://tdu.tanke756.top

[U93] JS：模板字符串
来源：http://gbv.shzxlz.cn

`共 ${n} 条`
来源：http://eah.yonumen.top

[U94] JS：箭头函数
来源：http://gic.jianghu66.top

const double = x => x * 2;
来源：http://ukc.uphjek.com

[U95] JS：Promise 包装
来源：http://kmy.yvedp.cn

new Promise((resolve, reject) => {})
来源：http://puq.xuetiantiany.cn

[U96] JS：async/await 与异常
来源：http://clr.ctjpmb.com

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://vcc.yj20258888.top

[U97] JS：并发请求
来源：http://yfm.52xcode.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://kzz.guowangkeji.top

[U98] JS：fetch 带 JSON
来源：http://clh.cqqwz.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://jjk.cdnleiting.top

[U99] JS：事件监听
来源：http://vvb.cheryme.top

el.addEventListener("click", e => {})
来源：http://fcq.9152youxi.cn

[U100] JS：DOM 查询
来源：http://vxj.andypj.xyz

document.querySelector(".item")
来源：http://quw.cqqwz.cn

[U101] JS：classList 操作
来源：http://zph.jinqigufen.top

el.classList.toggle("active")
来源：http://qrb.ppjwa.cn

[U102] JS：本地存储
来源：http://kyh.jinqigfzy.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://bob.cheryme.top

[U103] JS：定时器
来源：http://rxy.316326.xyz

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://ybw.tanke756.top

[U104] JS：防抖
来源：http://qtf.ydjk.org.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://bgw.jqgfzy.top

[U105] JS：节流
来源：http://mvl.c1oappe.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://mko.ydzc1.top

[U106] JS：日期格式化
来源：http://uom.ydjk.org.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://mpt.fengsongda.top

[U107] JS：数字千分位
来源：http://res.aibaodan.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://qsk.zhengqikj.top

[U108] JS：随机整数
来源：http://hkv.aizwys.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://drg.nwbrower.top

[U109] JS：数组分组
来源：http://qot.yfazqb.com

Object.groupBy(arr, x => x.type)
来源：http://act.andypj.xyz

[U110] JS：数组分块
来源：http://ytv.dianchejie.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hja.hnqzz.top

[U111] JS：对象转 Map
来源：http://oah.sysykeji.top

new Map(Object.entries(obj))
来源：http://sdu.0kj1m.cn

[U112] JS：字符串补位
来源：http://grx.gotoacloud.top

"7".padStart(3, "0")
来源：http://cax.guannengcc.top

[U113] JS：正则替换全部
来源：http://xyj.shuidangran.top

s.replaceAll("a", "b")
来源：http://fcy.daxiang520.top

[U114] JS：JSON 深比较
来源：http://bjj.wangshuangyany.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://cih.guannengcc.top

[U115] JS：生成 UUID
来源：http://vae.hysaishi.cn

crypto.randomUUID()
来源：http://rtk.xuanzx.com

[U116] JS：类型检查（JSDoc）
来源：http://bxz.haohaochexian.top

/** @param {string} name */ function f(name) {}
来源：http://qfx.kuanghao11.cn

[U117] JS：单元测试
来源：http://fsa.feifeiyinyue.top

npm i -D vitest;  npx vitest
来源：http://ggp.fanxiaobao.xyz

[U118] JS：开发服务器
来源：http://cpj.shangyingyoupin.top

npm i -D vite;  npx vite
来源：http://utz.shuidangran.top

[U119] JS：生产构建
来源：http://ccp.pengpengdd.cyou

npx vite build
来源：http://lqi.jqgfzy.top

[U120] JS：读取环境变量（Vite）
来源：http://tjh.yangfankeji.com

import.meta.env.VITE_API_URL
来源：http://bzr.haohaochexian.top

================================================================================
来源：http://cdg.ywan-chungtsiang.top

统计汇总
来源：http://jbo.uphjek.com

================================================================================
来源：http://duo.redwolf501.top

按语言统计（条）：
来源：http://xxi.pengpengdd.cyou

Python ......... 252
来源：http://bac.yongpay.top

PHP ............ 252
来源：http://bul.dashuyun.cn

JavaScript ..... 252
来源：http://aop.9152youxi.cn

TypeScript ..... 212
来源：http://egm.gotoacloud.top

Java ........... 212
来源：http://lsb.xziqi.cn

Go ............. 212
来源：http://sgf.zhoulong.xyz

Ruby ........... 212
来源：http://smk.cucudq.cn

C# ............. 212
来源：http://jqd.kuanghao11.cn

C .............. 30
来源：http://rqy.nanxinkj.top

C++ ............ 30
来源：http://xob.jqgfzy.top

SQL ............ 90
来源：http://xhw.yuxming.cn

Bash ........... 80
来源：http://rvu.zdqjudy.top

Kotlin ......... 15
来源：http://zuc.cqqwz.cn

Swift .......... 15
来源：http://cdt.jyoumei.cn

Lua ............ 10
来源：http://lzg.aibaodan.cn

Perl ........... 10
来源：http://cxa.chenlongwang.top

Scala .......... 10
来源：http://zld.xziqi.cn

------------------------------------
来源：http://jji.cashguo.top

合计 ........... 2106 条
来源：http://gxh.bbcook.cn

按章节统计：
来源：http://hdg.pengpengdd.cyou

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://irb.ybcxt.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://oex.chenjidiqi.icu

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://tti.wangdashe.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hrn.jqgufenzy.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://ebe.jinqigufen.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://lju.yueranfly.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://qyl.tanke756.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://ypx.hnxiangtu.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://wxn.jinyuanbaomall.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://fyn.zhixingplan.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://lwk.zycfv.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://kmv.yonumen.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://fah.jqgfzy.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://nqv.tarul.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://aju.snrcjt.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://zvk.ehwqpu.com


<!-- 参考信息 -->