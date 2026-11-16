代发 wailian999

def add(a: Int, b: Int): Int = a + b
来源：http://xgd.aibaodan.cn

[T59] Scala：循环
来源：http://ied.iojbl.cn

for (i <- 1 to 10) println(i)
来源：http://ueq.guowangkeji.top

[T60] Scala：折叠
来源：http://otg.haohaochexian.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://sga.fengsongda.top

================================================================================
来源：http://cli.shanyushiyangtech.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://aww.ydzc1.top

================================================================================
来源：http://bfz.shzxlz.cn

[U01] Py：创建虚拟环境
来源：http://zeg.jianghu66.top

python -m venv .venv && source .venv/bin/activate
来源：http://mil.yuanzhike.top

[U02] Py：导出 / 安装依赖
来源：http://cay.jinqigufen.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://rpb.gzhubu.top

[U03] Py：加载 .env 配置
来源：http://byr.fengsongda.top

from dotenv import load_dotenv; load_dotenv()
来源：http://kqv.hnqzz.top

[U04] Py：变量调试打印
来源：http://cwj.ppjwa.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://ayr.nanxinkj.top

[U05] Py：列表去重且保序
来源：http://gnr.gotoacloud.top

list(dict.fromkeys(arr))
来源：http://uyr.epnwcf.com

[U06] Py：合并两个字典
来源：http://def.nanxinkj.top

{**a, **b}
来源：http://uxb.jlsjyb.cn

[U07] Py：反转字典键值
来源：http://rxz.hnxiangtu.top

{v: k for k, v in d.items()}
来源：http://rdh.zycfv.cn

[U08] Py：展平二维列表
来源：http://azo.9152youxi.cn

[y for x in nested for y in x]
来源：http://kwp.c1oappe.top

[U09] Py：字典取最大值的键
来源：http://drg.sufxvd.cn

max(d, key=d.get)
来源：http://xhw.gzhubu.top

[U10] Py：按值排序字典
来源：http://onj.xinyue.icu

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://ski.jianghu66.top

[U11] Py：生成器表达式
来源：http://tfx.hongshengwenyu.top

(x * 2 for x in arr)
来源：http://njq.yj20258888.top

[U12] Py：取出现最多的 3 个元素
来源：http://axr.ydjk.org.cn

Counter(arr).most_common(3)
来源：http://brv.snrcjt.cn

[U13] Py：固定长度队列
来源：http://squ.zycfv.cn

deque(maxlen=10)
来源：http://dwh.dashuyun.cn

[U14] Py：分组收集到列表
来源：http://ciw.xziqi.cn

defaultdict(list)
来源：http://ozc.xziqi.cn

[U15] Py：高精度计时
来源：http://akj.hesvh.cn

t = time.perf_counter()
来源：http://rvv.feifeiyinyue.top

[U16] Py：命令行参数解析
来源：http://uao.gaohongyu789.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://opm.yvedp.cn

[U17] Py：初始化日志
来源：http://hzs.mhx1999.top

logging.basicConfig(level=logging.INFO)
来源：http://btv.hammf.cn

[U18] Py：预编译正则
来源：http://kbv.shzxlz.cn

pat = re.compile(r"\d+")
来源：http://wei.hywenlv.cn

[U19] Py：正则替换带回调
来源：http://fis.vehdjk.com

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://nxr.jinqigfzy.top

[U20] Py：缓存函数结果
来源：http://vai.xziqi.cn

@functools.lru_cache(maxsize=None)
来源：http://pys.jinqigufen.top

[U21] Py：自定义上下文管理器
来源：http://gcl.52xcode.cn

@contextlib.contextmanager
来源：http://rle.ybcxt.top

[U22] Py：矩阵转置
来源：http://ugb.yangfankeji.com

list(zip(*m))
来源：http://xog.bbcook.cn

[U23] Py：分块读取大文件
来源：http://uqq.aibaodan.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://nxa.ywan-chungtsiang.top

[U24] Py：路径操作
来源：http://jmn.316326.xyz

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://uvq.zhaomingkeji.xyz

[U25] Py：CSV 按字典读
来源：http://opt.snrcjt.cn

csv.DictReader(f)
来源：http://rdg.kuanghao11.cn

[U26] Py：并发下载
来源：http://vug.yfazqb.com

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://yfs.chenzaomai.com

[U27] Py：异步 HTTP
来源：http://kmf.fanxiaobao.xyz

aiohttp.ClientSession() 配合 async with
来源：http://bky.vqdsnc.cn

[U28] Py：类型别名
来源：http://daz.zdqjudy.top

UserId = int
来源：http://gcv.wangshuangyany.cn

[U29] Py：属性校验
来源：http://srz.feifeiyinyue.top

@property 与 @x.setter 配合
来源：http://tel.yuanzhike.top

[U30] Py：数据类
来源：http://cqb.jianghu66.top

@dataclass(slots=True)
来源：http://ggx.uphjek.com

[U31] Py：单测
来源：http://qbc.xingfuxueyuan.xyz

python -m pytest -q
来源：http://dwa.yj20258.top

[U32] Py：代码格式化
来源：http://pho.ehwqpu.com

ruff format . && ruff check --fix .
来源：http://ktc.nwbrower.top

[U33] Py：打包发布
来源：http://mgc.yj202588.top

python -m build  （依赖 pyproject.toml）
来源：http://kxj.nanxuanxn.top

[U34] Py：判断编码
来源：http://ael.hysaishi.cn

chardet.detect(raw)
来源：http://lht.jinyuanbaomall.cn

[U35] Py：发送邮件
来源：http://dss.ehwqpu.com

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://yan.sysykeji.top

[U36] Py：定时任务
来源：http://iuu.yj202588.top

schedule.every(10).minutes.do(job)
来源：http://gyj.vqdsnc.cn

[U37] Py：读写 Excel
来源：http://swe.nwbrower.top

pandas.read_excel / DataFrame.to_excel
来源：http://wrm.zhoulong.xyz

[U38] Py：获取脚本所在目录
来源：http://dwn.cashguo.top

Path(__file__).resolve().parent
来源：http://bhf.quarkkingdee.top

[U39] Py：判断是否在交互环境
来源：http://iwi.yangfankeji.com

sys.stdout.isatty()
来源：http://ytg.dianchejie.cn

[U40] Py：打印到标准错误
来源：http://zqt.daxiang520.top

print("err", file=sys.stderr)
来源：http://bvf.gogol.net.cn

[U41] PHP：初始化 Composer 项目
来源：http://zdj.tianlin.xyz

composer init;  composer require guzzlehttp/guzzle
来源：http://yow.wangshuangyany.cn

[U42] PHP：PSR-4 自动加载
来源：http://bpj.dianchejie.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://ytr.52xcode.cn

[U43] PHP：声明命名空间
来源：http://grc.zhixingplan.top

namespace App\Http;
来源：http://hzv.jinqigufen.top

[U44] PHP：开启严格类型
来源：http://wka.bbcook.cn

declare(strict_types=1);
来源：http://qnb.sweek.top

[U45] PHP：类型声明与返回类型
来源：http://qjt.zhiwuduotai.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://tkl.wangdashe.top

[U46] PHP：可空类型
来源：http://muf.zhaomingkeji.xyz

?string $name = null
来源：http://qyt.dianchejie.cn

[U47] PHP：联合类型
来源：http://fct.hnqzz.top

int|string $id
来源：http://dxi.ydzc1.top

[U48] PHP：纯枚举
来源：http://tqx.yangfankeji.com

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://jso.tianlin.xyz

[U49] PHP：只读属性
来源：http://qkx.jqgfzy.top

public readonly string $name
来源：http://dah.ydzc1.top

[U50] PHP：构造器属性提升
来源：http://btj.nanxuanxn.top

public function __construct(private int $id) {}
来源：http://ice.cheryme.top

[U51] PHP：数组解构
来源：http://yyy.zhiwuduotai.top

[$a, $b] = $arr;
来源：http://tuj.quarkkingdee.top

[U52] PHP：箭头函数
来源：http://eyc.hesvh.cn

$double = fn($x) => $x * 2;
来源：http://tvu.bjfxy.top

[U53] PHP：空合并运算符
来源：http://wwo.mhx1999.top

$v = $a ?? $b ?? "default";
来源：http://brj.hesvh.cn

[U54] PHP：空安全调用
来源：http://qep.zdqjudy.top

$obj?->method()
来源：http://nng.pycfn.com

[U55] PHP：match 表达式
来源：http://ujj.cucudq.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://ryo.gzhubu.top

[U56] PHP：命名参数
来源：http://fyc.ywan-chungtsiang.top

f(a: 1, b: 2)
来源：http://sdr.guowangkeji.top

[U57] PHP：字符串插值
来源：http://ydi.epnwcf.com

"值: {$a}"
来源：http://gre.yueranfly.top

[U58] PHP：数组三件套
来源：http://xaz.vqdsnc.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://qgx.yuanzhike.top

[U59] PHP：自定义排序
来源：http://utx.zhiwuduotai.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mea.fktsv.cn

[U60] PHP：JSON 编解码
来源：http://vup.yvedp.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://vsk.ctjpmb.com

[U61] PHP：正则
来源：http://btk.xylfe.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://xwf.ppjwa.cn

[U62] PHP：日期对象
来源：http://wlb.sufxvd.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://eff.havefunace.top

[U63] PHP：文件读写
来源：http://awy.dianchejie.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hyc.hongshengwenyu.top

[U64] PHP：目录遍历
来源：http://ccc.yueranfly.top

glob("dir/*.php");  scandir("dir");
来源：http://qtn.nanxuanxn.top

[U65] PHP：会话
来源：http://isp.dianchejie.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://pty.uphjek.com

[U66] PHP：设置 Cookie
来源：http://aln.quarkkingdee.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://ljk.fktsv.cn

[U67] PHP：处理文件上传
来源：http://wdc.zhoulong.xyz

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://ngl.hnxiangtu.top

[U68] PHP：PDO 连接
来源：http://bkb.c1oappe.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://jgc.guannengcc.top

[U69] PHP：PDO 预处理
来源：http://pvy.dashuyun.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://eao.xuanzx.com

[U70] PHP：PDO 事务
来源：http://qah.gogol.net.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://nbp.cqqwz.cn

[U71] PHP：抛出异常
来源：http://xsq.jinqigfzy.top

throw new RuntimeException("失败", 500);
来源：http://poa.gaohongyu789.top

[U72] PHP：写错误日志
来源：http://khi.pycfn.com

error_log("失败: " . $e->getMessage());
来源：http://dng.fehbvm.com

[U73] PHP：读取 ini 配置
来源：http://xdv.fanxiaobao.xyz

parse_ini_file("config.ini", true)
来源：http://gia.hnqzz.top

[U74] PHP：读取环境变量
来源：http://myg.hywenlv.cn

getenv("APP_ENV") ?: "production"
来源：http://wzq.yonumen.top

[U75] PHP：依赖注入
来源：http://mnf.fktsv.cn

composer require psr/container
来源：http://mgl.cashguo.top

[U76] PHP：简单路由
来源：http://dkj.jiagoushi.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://nam.gogol.net.cn

[U77] PHP：模板渲染
来源：http://qpb.jinqigfzy.top

composer require twig/twig
来源：http://jnk.ydjk.org.cn

[U78] PHP：单元测试
来源：http://aak.daxiang520.top

composer require --dev phpunit/phpunit
来源：http://syp.c1oappe.top

[U79] PHP：静态分析
来源：http://pxo.dianchejie.cn

composer require --dev phpstan/phpstan
来源：http://upc.zhengqikj.top

[U80] PHP：代码规范修复
来源：http://uop.jqgfzy.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://bxq.fzhhl.top

[U81] JS：初始化项目
来源：http://swv.jyoumei.cn

npm init -y;  npm i express
来源：http://llz.yj20258.top

[U82] JS：package.json 脚本
来源：http://zlj.zycfv.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://sdy.zhixingplan.top

[U83] JS：ES Module 导入导出
来源：http://zrr.tarul.cn

export const a = 1;  import { a } from "./m.js";
来源：http://mzv.hywenlv.cn

[U84] JS：CommonJS 写法
来源：http://wlu.pycfn.com

module.exports = { a };  const { a } = require("./m");
来源：http://gmp.yvedp.cn

[U85] JS：可选链
来源：http://cfj.ydjk.org.cn

a?.b?.c
来源：http://isy.redwolf501.top

[U86] JS：空值合并
来源：http://mfa.redwolf501.top

a ?? b
来源：http://vvs.hesvh.cn

[U87] JS：解构默认值
来源：http://bdd.havefunace.top

const { a = 1, b = 2 } = obj;
来源：http://nhe.xuetiantiany.cn

[U88] JS：对象展开合并
来源：http://hkx.quarkkingdee.top

{ ...a, ...b }
来源：http://azz.yongpay.top

[U89] JS：数组去重
来源：http://lrh.pycfn.com

[...new Set(arr)]
来源：http://iiy.redwolf501.top

[U90] JS：数字数组排序
来源：http://ggn.yfazqb.com

[...arr].sort((a, b) => a - b)
来源：http://owf.yj20258888.top

[U91] JS：对象键值遍历
来源：http://eer.haohaochexian.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://nif.sjlbkw.cn

[U92] JS：深拷贝
来源：http://wxv.yanxiufei.cn

structuredClone(obj)
来源：http://alb.zhixingplan.top

[U93] JS：模板字符串
来源：http://fui.sxryk.cn

`共 ${n} 条`
来源：http://rsk.tanke756.top

[U94] JS：箭头函数
来源：http://ise.vqdsnc.cn

const double = x => x * 2;
来源：http://rxf.ehwqpu.com

[U95] JS：Promise 包装
来源：http://njp.aibaodan.cn

new Promise((resolve, reject) => {})
来源：http://akr.hywenlv.cn

[U96] JS：async/await 与异常
来源：http://uml.yj20258.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://jky.nanxinkj.top

[U97] JS：并发请求
来源：http://pqy.fanxiaobao.xyz

await Promise.all(urls.map(u => fetch(u)))
来源：http://ctw.epnwcf.com

[U98] JS：fetch 带 JSON
来源：http://jcz.chenjidiqi.icu

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://ilj.jqgufenzy.top

[U99] JS：事件监听
来源：http://liw.tian-w.cn

el.addEventListener("click", e => {})
来源：http://wvw.mhx1999.top

[U100] JS：DOM 查询
来源：http://ler.hysaishi.cn

document.querySelector(".item")
来源：http://ifl.xingfuxueyuan.xyz

[U101] JS：classList 操作
来源：http://ewb.0kj1m.cn

el.classList.toggle("active")
来源：http://rud.hnxiangtu.top

[U102] JS：本地存储
来源：http://fzr.yj20258.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://ekh.zdbjq.cn

[U103] JS：定时器
来源：http://hlf.zhengqikj.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://vas.yangfankeji.com

[U104] JS：防抖
来源：http://wow.mhx1999.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://nec.xziqi.cn

[U105] JS：节流
来源：http://flc.uphjek.com

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://oel.zhengqikj.top

[U106] JS：日期格式化
来源：http://kpd.sjlbkw.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://wmn.havefunace.top

[U107] JS：数字千分位
来源：http://nle.tian-w.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://ysp.xingfuxueyuan.xyz

[U108] JS：随机整数
来源：http://xma.fanxiaobao.xyz

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hps.hesvh.cn

[U109] JS：数组分组
来源：http://lcx.yvedp.cn

Object.groupBy(arr, x => x.type)
来源：http://clv.redwolf501.top

[U110] JS：数组分块
来源：http://lxl.hongshengwenyu.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://vnr.nanxinkj.top

[U111] JS：对象转 Map
来源：http://vrq.jinyuanbaomall.cn

new Map(Object.entries(obj))
来源：http://fdi.uphjek.com

[U112] JS：字符串补位
来源：http://agf.dashuyun.cn

"7".padStart(3, "0")
来源：http://eel.cdnleiting.top

[U113] JS：正则替换全部
来源：http://fzu.chenjidiqi.icu

s.replaceAll("a", "b")
来源：http://eda.zhengqikj.top

[U114] JS：JSON 深比较
来源：http://muq.gaohongyu789.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://mjs.nwbrower.top

[U115] JS：生成 UUID
来源：http://mrg.jinqigfzy.top

crypto.randomUUID()
来源：http://zfh.yj20258888.top

[U116] JS：类型检查（JSDoc）
来源：http://ruj.yongpay.top

/** @param {string} name */ function f(name) {}
来源：http://oxb.cashguo.top

[U117] JS：单元测试
来源：http://ula.hysaishi.cn

npm i -D vitest;  npx vitest
来源：http://jht.shanyushiyangtech.top

[U118] JS：开发服务器
来源：http://ces.daxiang520.top

npm i -D vite;  npx vite
来源：http://pjm.wangdashe.top

[U119] JS：生产构建
来源：http://dqa.havefunace.top

npx vite build
来源：http://yut.jinghuilouyu.cn

[U120] JS：读取环境变量（Vite）
来源：http://cys.tarul.cn

import.meta.env.VITE_API_URL
来源：http://itq.xuetiantiany.cn

================================================================================
来源：http://ldn.cheryme.top

统计汇总
来源：http://gmv.tianlin.xyz

================================================================================
来源：http://ibn.dashuyun.cn

按语言统计（条）：
来源：http://cin.yj20258888.top

Python ......... 252
来源：http://tva.shanyushiyangtech.top

PHP ............ 252
来源：http://utv.zhaomingkeji.xyz

JavaScript ..... 252
来源：http://lid.ppjwa.cn

TypeScript ..... 212
来源：http://rdc.aizwys.cn

Java ........... 212
来源：http://fnb.cqqwz.cn

Go ............. 212
来源：http://ksi.shuidangran.top

Ruby ........... 212
来源：http://lyn.smart0.xyz

C# ............. 212
来源：http://dkr.shangyingyoupin.top

C .............. 30
来源：http://akz.c1oappe.top

C++ ............ 30
来源：http://zpx.xylfe.cn

SQL ............ 90
来源：http://nnx.xuetiantiany.cn

Bash ........... 80
来源：http://wlk.jyoumei.cn

Kotlin ......... 15
来源：http://vqd.ydjk.org.cn

Swift .......... 15
来源：http://giz.fanxiaobao.xyz

Lua ............ 10
来源：http://jie.gotoacloud.top

Perl ........... 10
来源：http://ulk.xuetiantiany.cn

Scala .......... 10
来源：http://zfc.xuanzx.com

------------------------------------
来源：http://ren.hywenlv.cn

合计 ........... 2106 条
来源：http://uug.xuetiantiany.cn

按章节统计：
来源：http://aug.tianlin.xyz

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://gwl.hfpthk.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://yap.hesvh.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://txc.chenjidiqi.icu

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://kyr.jiagoushi.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://zlv.zhaomingkeji.xyz

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://gsb.fzhhl.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://mnb.meibo888.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://bay.bjfxy.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://pgz.ppjwa.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://kgf.pycfn.com

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://bmp.shzxlz.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://ppj.tianlin.xyz

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://uwg.cdnleiting.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://fpz.aizwys.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://oup.cucudq.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://iyj.hywenlv.cn

Q SQL 专题                              90
来源：http://wsx.cqqwz.cn

R Bash 专题                             80
来源：http://xyx.hcnkem.com

S C / C++ 专题                          60
来源：http://mho.gotoacloud.top

T 其他语言补充                          60
来源：http://wnx.zhixingplan.top

U 高频实用片段                         120
来源：http://sbf.smart0.xyz

------------------------------------
来源：http://ybt.jinqigufen.top

合计                                  2106 条
来源：http://rfn.ybcxt.top

--------------------------------------------------------------------------------
来源：http://ypj.kuanghao11.cn

使用提醒
来源：http://bwk.tianlin.xyz

--------------------------------------------------------------------------------
来源：http://ono.yfazqb.com

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://uuo.ehwqpu.com

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://usc.haohaochexian.top


<!-- 参考信息 -->