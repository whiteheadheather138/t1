代发 wailian999

List(1, 2, 3).map(_ * 2)
来源：http://trl.xylfe.cn

[T55] Scala：集合过滤
来源：http://wfi.sysykeji.top

List(1, 2, 3).filter(_ > 1)
来源：http://ehz.shanyushiyangkeji.top

[T56] Scala：样例类
来源：http://zab.iojbl.cn

case class User(name: String, age: Int)
来源：http://ihb.fktsv.cn

[T57] Scala：模式匹配
来源：http://bxu.chenlongwang.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://lcp.yj20258888.top

[T58] Scala：函数定义
来源：http://tgv.fengsongda.top

def add(a: Int, b: Int): Int = a + b
来源：http://vuc.xziqi.cn

[T59] Scala：循环
来源：http://joa.yonumen.top

for (i <- 1 to 10) println(i)
来源：http://oob.gaohongyu789.top

[T60] Scala：折叠
来源：http://jew.jlsjyb.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://wvd.jiagoushi.top

================================================================================
来源：http://tvw.jiagoushi.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://igh.yueranfly.top

================================================================================
来源：http://aya.xuanzx.com

[U01] Py：创建虚拟环境
来源：http://mue.guannengcc.top

python -m venv .venv && source .venv/bin/activate
来源：http://kht.feifeiyinyue.top

[U02] Py：导出 / 安装依赖
来源：http://dkn.zycfv.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://owm.yongpay.top

[U03] Py：加载 .env 配置
来源：http://ote.jianghu66.top

from dotenv import load_dotenv; load_dotenv()
来源：http://nmh.hysaishi.cn

[U04] Py：变量调试打印
来源：http://gbm.bjfxy.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://zmn.chenjidiqi.icu

[U05] Py：列表去重且保序
来源：http://leo.shanyushiyangtech.top

list(dict.fromkeys(arr))
来源：http://stv.ctjpmb.com

[U06] Py：合并两个字典
来源：http://elo.hysaishi.cn

{**a, **b}
来源：http://nom.sjlbkw.cn

[U07] Py：反转字典键值
来源：http://pqj.yvedp.cn

{v: k for k, v in d.items()}
来源：http://ksf.jlsjyb.cn

[U08] Py：展平二维列表
来源：http://qxw.wangdashe.top

[y for x in nested for y in x]
来源：http://mjs.cqqwz.cn

[U09] Py：字典取最大值的键
来源：http://zoj.tarul.cn

max(d, key=d.get)
来源：http://luw.zhijiandao.cn

[U10] Py：按值排序字典
来源：http://hsc.sweek.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hxr.xinyue.icu

[U11] Py：生成器表达式
来源：http://hsl.haohaochexian.top

(x * 2 for x in arr)
来源：http://zkv.yonumen.top

[U12] Py：取出现最多的 3 个元素
来源：http://rko.fehbvm.com

Counter(arr).most_common(3)
来源：http://okg.zhoulong.xyz

[U13] Py：固定长度队列
来源：http://fpf.cheryme.top

deque(maxlen=10)
来源：http://zmi.jianghu66.top

[U14] Py：分组收集到列表
来源：http://bbi.cashguo.top

defaultdict(list)
来源：http://cxl.quarkkingdee.top

[U15] Py：高精度计时
来源：http://wxp.hesvh.cn

t = time.perf_counter()
来源：http://hke.chenzaomai.com

[U16] Py：命令行参数解析
来源：http://xom.haohaochexian.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://vzh.cheryme.top

[U17] Py：初始化日志
来源：http://mcv.tian-w.cn

logging.basicConfig(level=logging.INFO)
来源：http://bxp.ehwqpu.com

[U18] Py：预编译正则
来源：http://qyn.smart0.xyz

pat = re.compile(r"\d+")
来源：http://cnt.dashuyun.cn

[U19] Py：正则替换带回调
来源：http://uit.zdqjudy.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://wiq.daxiang520.top

[U20] Py：缓存函数结果
来源：http://mpm.xziqi.cn

@functools.lru_cache(maxsize=None)
来源：http://oeb.vqdsnc.cn

[U21] Py：自定义上下文管理器
来源：http://qkv.mhx1999.top

@contextlib.contextmanager
来源：http://apm.sweek.top

[U22] Py：矩阵转置
来源：http://dfd.shangyingyoupin.top

list(zip(*m))
来源：http://oef.zhengqikj.top

[U23] Py：分块读取大文件
来源：http://ced.yanxiufei.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://vma.hongshengwenyu.top

[U24] Py：路径操作
来源：http://amm.nanxinkj.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://rtf.yj202588.top

[U25] Py：CSV 按字典读
来源：http://dda.yonumen.top

csv.DictReader(f)
来源：http://vcj.yangfankeji.com

[U26] Py：并发下载
来源：http://spl.aizwys.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://ddk.cheryme.top

[U27] Py：异步 HTTP
来源：http://qle.guannengcc.top

aiohttp.ClientSession() 配合 async with
来源：http://dhg.fanxiaobao.xyz

[U28] Py：类型别名
来源：http://xud.feifeiyinyue.top

UserId = int
来源：http://rzb.jinqigfzy.top

[U29] Py：属性校验
来源：http://wlh.zhongyouzk.top

@property 与 @x.setter 配合
来源：http://eqt.jinqigfzy.top

[U30] Py：数据类
来源：http://gvd.cdnleiting.top

@dataclass(slots=True)
来源：http://ljj.haohaochexian.top

[U31] Py：单测
来源：http://dao.cucudq.cn

python -m pytest -q
来源：http://xut.tarul.cn

[U32] Py：代码格式化
来源：http://jjl.tian-w.cn

ruff format . && ruff check --fix .
来源：http://ghh.ydzc1.top

[U33] Py：打包发布
来源：http://aek.cucudq.cn

python -m build  （依赖 pyproject.toml）
来源：http://ouy.xuanzx.com

[U34] Py：判断编码
来源：http://hza.9152youxi.cn

chardet.detect(raw)
来源：http://lcm.daria6918.cn

[U35] Py：发送邮件
来源：http://fim.havefunace.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://rzz.zhongyouzk.top

[U36] Py：定时任务
来源：http://mhy.cqqwz.cn

schedule.every(10).minutes.do(job)
来源：http://vki.gogol.net.cn

[U37] Py：读写 Excel
来源：http://vic.smart0.xyz

pandas.read_excel / DataFrame.to_excel
来源：http://uaa.chenjidiqi.icu

[U38] Py：获取脚本所在目录
来源：http://aqt.hesvh.cn

Path(__file__).resolve().parent
来源：http://mfa.zhaomingkeji.xyz

[U39] Py：判断是否在交互环境
来源：http://ilx.aizwys.cn

sys.stdout.isatty()
来源：http://aqw.xingfuxueyuan.xyz

[U40] Py：打印到标准错误
来源：http://wrk.snrcjt.cn

print("err", file=sys.stderr)
来源：http://pqk.aizwys.cn

[U41] PHP：初始化 Composer 项目
来源：http://jds.yonumen.top

composer init;  composer require guzzlehttp/guzzle
来源：http://hew.xuetiantiany.cn

[U42] PHP：PSR-4 自动加载
来源：http://vjw.zhixingplan.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://oek.yj202588.top

[U43] PHP：声明命名空间
来源：http://aof.0kj1m.cn

namespace App\Http;
来源：http://qwd.tarul.cn

[U44] PHP：开启严格类型
来源：http://koi.chenjidiqi.icu

declare(strict_types=1);
来源：http://dob.cucudq.cn

[U45] PHP：类型声明与返回类型
来源：http://bhd.ydjk.org.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://wax.hywenlv.cn

[U46] PHP：可空类型
来源：http://wfk.mhx1999.top

?string $name = null
来源：http://bnf.9152youxi.cn

[U47] PHP：联合类型
来源：http://nel.cashguo.top

int|string $id
来源：http://cya.yongpay.top

[U48] PHP：纯枚举
来源：http://wtk.fehbvm.com

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://pja.shangyingyoupin.top

[U49] PHP：只读属性
来源：http://gmw.cashguo.top

public readonly string $name
来源：http://pqj.gaohongyu789.top

[U50] PHP：构造器属性提升
来源：http://aai.xziqi.cn

public function __construct(private int $id) {}
来源：http://njv.birdmap.top

[U51] PHP：数组解构
来源：http://qvk.jlsjyb.cn

[$a, $b] = $arr;
来源：http://dgt.sweek.top

[U52] PHP：箭头函数
来源：http://jat.xylfe.cn

$double = fn($x) => $x * 2;
来源：http://pnk.chenlongwang.top

[U53] PHP：空合并运算符
来源：http://wbp.fengsongda.top

$v = $a ?? $b ?? "default";
来源：http://ema.zhoulong.xyz

[U54] PHP：空安全调用
来源：http://ksa.iojbl.cn

$obj?->method()
来源：http://xzf.zhixingplan.top

[U55] PHP：match 表达式
来源：http://yjy.haohaochexian.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://xmr.aizwys.cn

[U56] PHP：命名参数
来源：http://dzm.daria6918.cn

f(a: 1, b: 2)
来源：http://ppb.haohaochexian.top

[U57] PHP：字符串插值
来源：http://zqs.nanxinkj.top

"值: {$a}"
来源：http://fdy.zhaomingkeji.xyz

[U58] PHP：数组三件套
来源：http://kwy.iojbl.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://xcp.fktsv.cn

[U59] PHP：自定义排序
来源：http://kom.xziqi.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://zpb.jyoumei.cn

[U60] PHP：JSON 编解码
来源：http://quh.hesvh.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://jmt.iojbl.cn

[U61] PHP：正则
来源：http://qse.yvedp.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://krr.sweek.top

[U62] PHP：日期对象
来源：http://rqo.ctjpmb.com

(new DateTimeImmutable())->format("Y-m-d");
来源：http://pyq.snrcjt.cn

[U63] PHP：文件读写
来源：http://koi.zdbjq.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://xyw.tian-w.cn

[U64] PHP：目录遍历
来源：http://wrb.ydzc1.top

glob("dir/*.php");  scandir("dir");
来源：http://ezw.yvedp.cn

[U65] PHP：会话
来源：http://rfs.sufxvd.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://ixy.xuanzx.com

[U66] PHP：设置 Cookie
来源：http://ncw.fehbvm.com

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://qii.shanyushiyangtech.top

[U67] PHP：处理文件上传
来源：http://jyj.yj202588.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://lwf.dashuyun.cn

[U68] PHP：PDO 连接
来源：http://lex.vqdsnc.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://ebc.wangshuangyany.cn

[U69] PHP：PDO 预处理
来源：http://klc.chenjidiqi.icu

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://grr.meibo888.top

[U70] PHP：PDO 事务
来源：http://dyc.iojbl.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://xkm.wangshuangyany.cn

[U71] PHP：抛出异常
来源：http://zle.hesvh.cn

throw new RuntimeException("失败", 500);
来源：http://ojl.xziqi.cn

[U72] PHP：写错误日志
来源：http://gli.tarul.cn

error_log("失败: " . $e->getMessage());
来源：http://tfw.sjlbkw.cn

[U73] PHP：读取 ini 配置
来源：http://jtt.ybcxt.top

parse_ini_file("config.ini", true)
来源：http://zxq.fanxiaobao.xyz

[U74] PHP：读取环境变量
来源：http://zla.hysaishi.cn

getenv("APP_ENV") ?: "production"
来源：http://mnu.yj20258888.top

[U75] PHP：依赖注入
来源：http://mpx.aizwys.cn

composer require psr/container
来源：http://ctl.nanxinkj.top

[U76] PHP：简单路由
来源：http://qie.tian-w.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://kgc.nwbrower.top

[U77] PHP：模板渲染
来源：http://gdl.yongpay.top

composer require twig/twig
来源：http://frt.9152youxi.cn

[U78] PHP：单元测试
来源：http://qrk.epnwcf.com

composer require --dev phpunit/phpunit
来源：http://nlz.hesvh.cn

[U79] PHP：静态分析
来源：http://rmu.daria6918.cn

composer require --dev phpstan/phpstan
来源：http://bbm.epnwcf.com

[U80] PHP：代码规范修复
来源：http://gjf.ydzc1.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://zek.yueranfly.top

[U81] JS：初始化项目
来源：http://eaq.fengsongda.top

npm init -y;  npm i express
来源：http://zlr.yj202588.top

[U82] JS：package.json 脚本
来源：http://owz.sjlbkw.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://pmq.jqgfzy.top

[U83] JS：ES Module 导入导出
来源：http://dvd.shanyushiyangkeji.top

export const a = 1;  import { a } from "./m.js";
来源：http://rta.hcnkem.com

[U84] JS：CommonJS 写法
来源：http://vfb.yuxming.cn

module.exports = { a };  const { a } = require("./m");
来源：http://ejq.zhixingplan.top

[U85] JS：可选链
来源：http://vbh.shangyingyoupin.top

a?.b?.c
来源：http://nah.jqgfzy.top

[U86] JS：空值合并
来源：http://gih.zdqjudy.top

a ?? b
来源：http://xel.sufxvd.cn

[U87] JS：解构默认值
来源：http://dvy.kuanghao11.cn

const { a = 1, b = 2 } = obj;
来源：http://ehp.yuanzhike.top

[U88] JS：对象展开合并
来源：http://dkf.jinyuanbaomall.cn

{ ...a, ...b }
来源：http://ged.yj202588.top

[U89] JS：数组去重
来源：http://kza.yueranfly.top

[...new Set(arr)]
来源：http://xfr.xinyue.icu

[U90] JS：数字数组排序
来源：http://vtr.yuxming.cn

[...arr].sort((a, b) => a - b)
来源：http://jru.zhixingplan.top

[U91] JS：对象键值遍历
来源：http://ucp.epnwcf.com

Object.entries(obj).forEach(([k, v]) => {});
来源：http://qbe.cashguo.top

[U92] JS：深拷贝
来源：http://qst.sweek.top

structuredClone(obj)
来源：http://hje.zycfv.cn

[U93] JS：模板字符串
来源：http://ehb.chenzaomai.com

`共 ${n} 条`
来源：http://cgh.hfpthk.cn

[U94] JS：箭头函数
来源：http://gkd.xuanzx.com

const double = x => x * 2;
来源：http://ovg.cucudq.cn

[U95] JS：Promise 包装
来源：http://cgc.xinyue.icu

new Promise((resolve, reject) => {})
来源：http://qfn.shuidangran.top

[U96] JS：async/await 与异常
来源：http://nec.hongshengwenyu.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://fpk.yangfankeji.com

[U97] JS：并发请求
来源：http://vrv.sjlbkw.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://ezb.dashuyun.cn

[U98] JS：fetch 带 JSON
来源：http://msc.9152youxi.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://lwd.zhaomingkeji.xyz

[U99] JS：事件监听
来源：http://cqu.yj202588.top

el.addEventListener("click", e => {})
来源：http://ryp.52xcode.cn

[U100] JS：DOM 查询
来源：http://cnq.cdnleiting.top

document.querySelector(".item")
来源：http://wpq.hywenlv.cn

[U101] JS：classList 操作
来源：http://oet.tian-w.cn

el.classList.toggle("active")
来源：http://uvp.daxiang520.top

[U102] JS：本地存储
来源：http://chs.yj20258.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://eaq.jinqigufen.top

[U103] JS：定时器
来源：http://rpl.gotoacloud.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://rlv.zdqjudy.top

[U104] JS：防抖
来源：http://spj.zhiwuduotai.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://qme.yj202588.top

[U105] JS：节流
来源：http://pzd.uphjek.com

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://pzv.ydzc1.top

[U106] JS：日期格式化
来源：http://dnr.yuanzhike.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://ugs.mhx1999.top

[U107] JS：数字千分位
来源：http://kly.pengpengdd.cyou

new Intl.NumberFormat("en-US").format(1234567)
来源：http://swp.kuanghao11.cn

[U108] JS：随机整数
来源：http://rap.ydzc1.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://unx.feifeiyinyue.top

[U109] JS：数组分组
来源：http://gjr.zhoulong.xyz

Object.groupBy(arr, x => x.type)
来源：http://faa.zdqjudy.top

[U110] JS：数组分块
来源：http://yvo.epnwcf.com

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://oyt.yvedp.cn

[U111] JS：对象转 Map
来源：http://qnr.redwolf501.top

new Map(Object.entries(obj))
来源：http://eli.meibo888.top

[U112] JS：字符串补位
来源：http://pbt.dashuyun.cn

"7".padStart(3, "0")
来源：http://bly.fktsv.cn

[U113] JS：正则替换全部
来源：http://crg.jqgufenzy.top

s.replaceAll("a", "b")
来源：http://ztm.jiagoushi.top

[U114] JS：JSON 深比较
来源：http://cpk.zdqjudy.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://ugw.shanyushiyangtech.top

[U115] JS：生成 UUID
来源：http://wpw.aizwys.cn

crypto.randomUUID()
来源：http://bzv.tianlin.xyz

[U116] JS：类型检查（JSDoc）
来源：http://jya.tian-w.cn

/** @param {string} name */ function f(name) {}
来源：http://cit.birdmap.top

[U117] JS：单元测试
来源：http://cty.hcnkem.com

npm i -D vitest;  npx vitest
来源：http://zth.andypj.xyz

[U118] JS：开发服务器
来源：http://lmf.nanxinkj.top

npm i -D vite;  npx vite
来源：http://gav.guannengcc.top

[U119] JS：生产构建
来源：http://ebu.dianchejie.cn

npx vite build
来源：http://jct.cheryme.top

[U120] JS：读取环境变量（Vite）
来源：http://jkb.yuxming.cn

import.meta.env.VITE_API_URL
来源：http://cdk.shanyushiyangkeji.top

================================================================================
来源：http://ngl.zhengqikj.top

统计汇总
来源：http://cuu.jinqigfzy.top

================================================================================
来源：http://qnh.aibaodan.cn

按语言统计（条）：
来源：http://okx.hywenlv.cn

Python ......... 252
来源：http://ury.ybcxt.top

PHP ............ 252
来源：http://xnh.yonumen.top

JavaScript ..... 252
来源：http://ubu.xylfe.cn

TypeScript ..... 212
来源：http://dge.sufxvd.cn

Java ........... 212
来源：http://zfe.fktsv.cn

Go ............. 212
来源：http://cwo.nanxuanxn.top

Ruby ........... 212
来源：http://idh.cheryme.top

C# ............. 212
来源：http://knh.fktsv.cn

C .............. 30
来源：http://xhv.iojbl.cn

C++ ............ 30
来源：http://eur.zhongyouzk.top

SQL ............ 90
来源：http://mlo.nanxuanxn.top

Bash ........... 80
来源：http://erf.bjfxy.top

Kotlin ......... 15
来源：http://qqz.aibaodan.cn

Swift .......... 15
来源：http://gdy.hfpthk.cn

Lua ............ 10
来源：http://zgv.guowangkeji.top

Perl ........... 10
来源：http://xar.sxryk.cn

Scala .......... 10
来源：http://rwq.yj20258.top

------------------------------------
来源：http://vxi.jinqigfzy.top

合计 ........... 2106 条
来源：http://xqt.cdnleiting.top

按章节统计：
来源：http://pka.fehbvm.com

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://oug.sjlbkw.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://mev.gaohongyu789.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://nab.tanke756.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://mxn.zhaomingkeji.xyz

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://mli.sysykeji.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://tvv.ydjk.org.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://moh.wangdashe.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://lni.zhoulong.xyz

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://qyb.0kj1m.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://mvn.fehbvm.com

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://iea.chenzaomai.com

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://ttv.feifeiyinyue.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://nqi.jinyuanbaomall.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://zvm.yuanzhike.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://riz.gogol.net.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://lfh.shanyushiyangkeji.top

Q SQL 专题                              90
来源：http://fdx.52xcode.cn

R Bash 专题                             80
来源：http://gtk.chenlongwang.top

S C / C++ 专题                          60
来源：http://zra.ydjk.org.cn

T 其他语言补充                          60
来源：http://qme.guowangkeji.top


<!-- 参考信息 -->