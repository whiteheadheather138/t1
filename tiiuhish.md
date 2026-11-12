代发 wailian999

def add(a: Int, b: Int): Int = a + b
来源：http://llz.yj202588.top

[T59] Scala：循环
来源：http://qer.birdmap.top

for (i <- 1 to 10) println(i)
来源：http://mbh.pycfn.com

[T60] Scala：折叠
来源：http://eff.zhoulong.xyz

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://jdh.yanxiufei.cn

================================================================================
来源：http://zpf.nwbrower.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://niw.kuanghao11.cn

================================================================================
来源：http://txd.yueranfly.top

[U01] Py：创建虚拟环境
来源：http://vlu.fanxiaobao.xyz

python -m venv .venv && source .venv/bin/activate
来源：http://oob.0kj1m.cn

[U02] Py：导出 / 安装依赖
来源：http://ill.daxiang520.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://kem.xziqi.cn

[U03] Py：加载 .env 配置
来源：http://eyr.cheryme.top

from dotenv import load_dotenv; load_dotenv()
来源：http://jqx.bbcook.cn

[U04] Py：变量调试打印
来源：http://xjn.yongpay.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://pvm.bbcook.cn

[U05] Py：列表去重且保序
来源：http://ufd.shanyushiyangkeji.top

list(dict.fromkeys(arr))
来源：http://osk.zhijiandao.cn

[U06] Py：合并两个字典
来源：http://kwl.wangdashe.top

{**a, **b}
来源：http://acd.sysykeji.top

[U07] Py：反转字典键值
来源：http://lkd.fktsv.cn

{v: k for k, v in d.items()}
来源：http://pnc.mhx1999.top

[U08] Py：展平二维列表
来源：http://ung.yfazqb.com

[y for x in nested for y in x]
来源：http://shd.bjfxy.top

[U09] Py：字典取最大值的键
来源：http://plx.fehbvm.com

max(d, key=d.get)
来源：http://fha.hongshengwenyu.top

[U10] Py：按值排序字典
来源：http://ume.gzhubu.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://equ.tianlin.xyz

[U11] Py：生成器表达式
来源：http://rhn.mhx1999.top

(x * 2 for x in arr)
来源：http://gmj.xziqi.cn

[U12] Py：取出现最多的 3 个元素
来源：http://hok.zycfv.cn

Counter(arr).most_common(3)
来源：http://tvl.shangyingyoupin.top

[U13] Py：固定长度队列
来源：http://fsq.jinyuanbaomall.cn

deque(maxlen=10)
来源：http://dxr.aizwys.cn

[U14] Py：分组收集到列表
来源：http://wwu.xylfe.cn

defaultdict(list)
来源：http://qvq.yj20258888.top

[U15] Py：高精度计时
来源：http://mpf.meibo888.top

t = time.perf_counter()
来源：http://wnr.yj20258888.top

[U16] Py：命令行参数解析
来源：http://nea.nanxinkj.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://gmf.c1oappe.top

[U17] Py：初始化日志
来源：http://lpi.hesvh.cn

logging.basicConfig(level=logging.INFO)
来源：http://oqs.uphjek.com

[U18] Py：预编译正则
来源：http://ifj.hongshengwenyu.top

pat = re.compile(r"\d+")
来源：http://egz.hywenlv.cn

[U19] Py：正则替换带回调
来源：http://zty.jinyuanbaomall.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://quq.c1oappe.top

[U20] Py：缓存函数结果
来源：http://bye.hcnkem.com

@functools.lru_cache(maxsize=None)
来源：http://nbc.wangshuangyany.cn

[U21] Py：自定义上下文管理器
来源：http://miu.xuanzx.com

@contextlib.contextmanager
来源：http://ycv.daxiang520.top

[U22] Py：矩阵转置
来源：http://zgr.andypj.xyz

list(zip(*m))
来源：http://axb.chenlongwang.top

[U23] Py：分块读取大文件
来源：http://fvd.hysaishi.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://gjp.bjfxy.top

[U24] Py：路径操作
来源：http://esf.uphjek.com

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://vtd.316326.xyz

[U25] Py：CSV 按字典读
来源：http://yhu.chenjidiqi.icu

csv.DictReader(f)
来源：http://gye.zhijiandao.cn

[U26] Py：并发下载
来源：http://oaz.yfazqb.com

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://lly.ydjk.org.cn

[U27] Py：异步 HTTP
来源：http://vac.ydzc1.top

aiohttp.ClientSession() 配合 async with
来源：http://wcp.xuanzx.com

[U28] Py：类型别名
来源：http://vty.svipenyu.cn

UserId = int
来源：http://guh.cashguo.top

[U29] Py：属性校验
来源：http://vrm.zdqjudy.top

@property 与 @x.setter 配合
来源：http://rnn.haohaochexian.top

[U30] Py：数据类
来源：http://akf.guowangkeji.top

@dataclass(slots=True)
来源：http://fvh.aizwys.cn

[U31] Py：单测
来源：http://ywl.daria6918.cn

python -m pytest -q
来源：http://vth.redwolf501.top

[U32] Py：代码格式化
来源：http://ccn.fzhhl.top

ruff format . && ruff check --fix .
来源：http://qqx.hcnkem.com

[U33] Py：打包发布
来源：http://xsp.shangyingyoupin.top

python -m build  （依赖 pyproject.toml）
来源：http://jpv.hongshengwenyu.top

[U34] Py：判断编码
来源：http://qtd.yangfankeji.com

chardet.detect(raw)
来源：http://cax.shuidangran.top

[U35] Py：发送邮件
来源：http://fxw.tanke756.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://kpz.yueranfly.top

[U36] Py：定时任务
来源：http://dmk.fzhhl.top

schedule.every(10).minutes.do(job)
来源：http://jmk.fktsv.cn

[U37] Py：读写 Excel
来源：http://xhs.snrcjt.cn

pandas.read_excel / DataFrame.to_excel
来源：http://wfl.zhixingplan.top

[U38] Py：获取脚本所在目录
来源：http://gne.yvedp.cn

Path(__file__).resolve().parent
来源：http://yfj.ydjk.org.cn

[U39] Py：判断是否在交互环境
来源：http://anp.guowangkeji.top

sys.stdout.isatty()
来源：http://set.sufxvd.cn

[U40] Py：打印到标准错误
来源：http://xey.zhongyouzk.top

print("err", file=sys.stderr)
来源：http://mpt.fktsv.cn

[U41] PHP：初始化 Composer 项目
来源：http://lvd.aibaodan.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://tyb.fengsongda.top

[U42] PHP：PSR-4 自动加载
来源：http://dae.xuanzx.com

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://aya.zhongyouzk.top

[U43] PHP：声明命名空间
来源：http://ugw.ivvv.top

namespace App\Http;
来源：http://ixg.cheryme.top

[U44] PHP：开启严格类型
来源：http://fec.aibaodan.cn

declare(strict_types=1);
来源：http://iym.sweek.top

[U45] PHP：类型声明与返回类型
来源：http://yds.sjlbkw.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://mys.bjfxy.top

[U46] PHP：可空类型
来源：http://oki.c1oappe.top

?string $name = null
来源：http://xgv.yanxiufei.cn

[U47] PHP：联合类型
来源：http://onh.jlsjyb.cn

int|string $id
来源：http://aay.yongpay.top

[U48] PHP：纯枚举
来源：http://ocp.jinqigfzy.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://gsl.xinyue.icu

[U49] PHP：只读属性
来源：http://jhs.zhixingplan.top

public readonly string $name
来源：http://otm.zhijiandao.cn

[U50] PHP：构造器属性提升
来源：http://dot.sxryk.cn

public function __construct(private int $id) {}
来源：http://apq.jlsjyb.cn

[U51] PHP：数组解构
来源：http://mgt.bjfxy.top

[$a, $b] = $arr;
来源：http://txs.daxiang520.top

[U52] PHP：箭头函数
来源：http://jnl.iojbl.cn

$double = fn($x) => $x * 2;
来源：http://sqq.vqdsnc.cn

[U53] PHP：空合并运算符
来源：http://pdk.zhijiandao.cn

$v = $a ?? $b ?? "default";
来源：http://wpn.hcnkem.com

[U54] PHP：空安全调用
来源：http://awg.cqqwz.cn

$obj?->method()
来源：http://vpt.sufxvd.cn

[U55] PHP：match 表达式
来源：http://lia.yfazqb.com

$s = match($x) { 1 => "一", default => "其他" };
来源：http://htf.vehdjk.com

[U56] PHP：命名参数
来源：http://sae.tanke756.top

f(a: 1, b: 2)
来源：http://wyb.dianchejie.cn

[U57] PHP：字符串插值
来源：http://hip.yj20258888.top

"值: {$a}"
来源：http://wud.hnxiangtu.top

[U58] PHP：数组三件套
来源：http://dmy.mhx1999.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://fpu.yfazqb.com

[U59] PHP：自定义排序
来源：http://nha.guannengcc.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ein.xingfuxueyuan.xyz

[U60] PHP：JSON 编解码
来源：http://bvv.sjlbkw.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://ryj.tanke756.top

[U61] PHP：正则
来源：http://csj.jqgfzy.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://ufs.zhijiandao.cn

[U62] PHP：日期对象
来源：http://mws.ctjpmb.com

(new DateTimeImmutable())->format("Y-m-d");
来源：http://pjj.cheryme.top

[U63] PHP：文件读写
来源：http://npv.dianchejie.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://wnq.0kj1m.cn

[U64] PHP：目录遍历
来源：http://hvb.kuanghao11.cn

glob("dir/*.php");  scandir("dir");
来源：http://kek.daria6918.cn

[U65] PHP：会话
来源：http://dns.hnqzz.top

session_start();  $_SESSION["uid"] = 1;
来源：http://skf.aizwys.cn

[U66] PHP：设置 Cookie
来源：http://ybe.xinyue.icu

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://bdn.dashuyun.cn

[U67] PHP：处理文件上传
来源：http://fml.ivvv.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://tpx.snrcjt.cn

[U68] PHP：PDO 连接
来源：http://izm.pycfn.com

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://gjt.pycfn.com

[U69] PHP：PDO 预处理
来源：http://qkt.yonumen.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://sjn.daria6918.cn

[U70] PHP：PDO 事务
来源：http://faw.ivvv.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://dpn.zhaomingkeji.xyz

[U71] PHP：抛出异常
来源：http://yrf.epnwcf.com

throw new RuntimeException("失败", 500);
来源：http://rtd.ivvv.top

[U72] PHP：写错误日志
来源：http://dfi.vqdsnc.cn

error_log("失败: " . $e->getMessage());
来源：http://wuj.ppjwa.cn

[U73] PHP：读取 ini 配置
来源：http://hci.yueranfly.top

parse_ini_file("config.ini", true)
来源：http://urw.shzxlz.cn

[U74] PHP：读取环境变量
来源：http://ohv.hammf.cn

getenv("APP_ENV") ?: "production"
来源：http://unp.gzhubu.top

[U75] PHP：依赖注入
来源：http://rbt.aibaodan.cn

composer require psr/container
来源：http://zrh.tanke756.top

[U76] PHP：简单路由
来源：http://qud.ehwqpu.com

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://lzq.xziqi.cn

[U77] PHP：模板渲染
来源：http://qwx.wangdashe.top

composer require twig/twig
来源：http://nlj.yanxiufei.cn

[U78] PHP：单元测试
来源：http://igz.hongshengwenyu.top

composer require --dev phpunit/phpunit
来源：http://pbk.zhoulong.xyz

[U79] PHP：静态分析
来源：http://idk.chenjidiqi.icu

composer require --dev phpstan/phpstan
来源：http://xxw.jiagoushi.top

[U80] PHP：代码规范修复
来源：http://iad.fzhhl.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://kok.redwolf501.top

[U81] JS：初始化项目
来源：http://izz.zhengqikj.top

npm init -y;  npm i express
来源：http://fsd.c1oappe.top

[U82] JS：package.json 脚本
来源：http://ryk.zhijiandao.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://zbx.jianghu66.top

[U83] JS：ES Module 导入导出
来源：http://flx.daria6918.cn

export const a = 1;  import { a } from "./m.js";
来源：http://yns.zycfv.cn

[U84] JS：CommonJS 写法
来源：http://zqj.jinghuilouyu.cn

module.exports = { a };  const { a } = require("./m");
来源：http://cfx.nwbrower.top

[U85] JS：可选链
来源：http://wiy.smart0.xyz

a?.b?.c
来源：http://xoh.tarul.cn

[U86] JS：空值合并
来源：http://hhk.hysaishi.cn

a ?? b
来源：http://qtw.yangfankeji.com

[U87] JS：解构默认值
来源：http://dvh.pengpengdd.cyou

const { a = 1, b = 2 } = obj;
来源：http://qqq.fanxiaobao.xyz

[U88] JS：对象展开合并
来源：http://brm.feifeiyinyue.top

{ ...a, ...b }
来源：http://bhi.fehbvm.com

[U89] JS：数组去重
来源：http://dvi.chenjidiqi.icu

[...new Set(arr)]
来源：http://jxa.sufxvd.cn

[U90] JS：数字数组排序
来源：http://hzx.hysaishi.cn

[...arr].sort((a, b) => a - b)
来源：http://ikx.epnwcf.com

[U91] JS：对象键值遍历
来源：http://ffp.meibo888.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://gdh.gzhubu.top

[U92] JS：深拷贝
来源：http://pod.kuanghao11.cn

structuredClone(obj)
来源：http://asf.xziqi.cn

[U93] JS：模板字符串
来源：http://ddb.ppjwa.cn

`共 ${n} 条`
来源：http://qog.wangshuangyany.cn

[U94] JS：箭头函数
来源：http://fis.bjfxy.top

const double = x => x * 2;
来源：http://jgx.pycfn.com

[U95] JS：Promise 包装
来源：http://bvp.hesvh.cn

new Promise((resolve, reject) => {})
来源：http://hld.guannengcc.top

[U96] JS：async/await 与异常
来源：http://ace.cdnleiting.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://tll.sxryk.cn

[U97] JS：并发请求
来源：http://nvb.zhongyouzk.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://neu.hfpthk.cn

[U98] JS：fetch 带 JSON
来源：http://ish.epnwcf.com

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://gob.tanke756.top

[U99] JS：事件监听
来源：http://zgg.gzhubu.top

el.addEventListener("click", e => {})
来源：http://uwq.xziqi.cn

[U100] JS：DOM 查询
来源：http://hvk.xuanzx.com

document.querySelector(".item")
来源：http://ilw.chenzaomai.com

[U101] JS：classList 操作
来源：http://mnz.fzhhl.top

el.classList.toggle("active")
来源：http://oob.jyoumei.cn

[U102] JS：本地存储
来源：http://ijd.uphjek.com

localStorage.setItem("k", JSON.stringify(v))
来源：http://yxq.chenjidiqi.icu

[U103] JS：定时器
来源：http://whv.tianlin.xyz

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://ymv.zhijiandao.cn

[U104] JS：防抖
来源：http://ahc.wangshuangyany.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ckq.52xcode.cn

[U105] JS：节流
来源：http://lsp.sjlbkw.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://pft.vqdsnc.cn

[U106] JS：日期格式化
来源：http://fkd.gogol.net.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://bcc.gogol.net.cn

[U107] JS：数字千分位
来源：http://her.fanxiaobao.xyz

new Intl.NumberFormat("en-US").format(1234567)
来源：http://log.jinghuilouyu.cn

[U108] JS：随机整数
来源：http://avp.9152youxi.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://udk.zhongyouzk.top

[U109] JS：数组分组
来源：http://hik.fengsongda.top

Object.groupBy(arr, x => x.type)
来源：http://avl.0kj1m.cn

[U110] JS：数组分块
来源：http://fmt.zhongyouzk.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://amc.hywenlv.cn

[U111] JS：对象转 Map
来源：http://flp.fehbvm.com

new Map(Object.entries(obj))
来源：http://nzn.daxiang520.top

[U112] JS：字符串补位
来源：http://xhx.birdmap.top

"7".padStart(3, "0")
来源：http://qld.nanxuanxn.top

[U113] JS：正则替换全部
来源：http://bdw.vehdjk.com

s.replaceAll("a", "b")
来源：http://lrg.guowangkeji.top

[U114] JS：JSON 深比较
来源：http://qkk.yuxming.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://zgf.jinqigufen.top

[U115] JS：生成 UUID
来源：http://fws.zdqjudy.top

crypto.randomUUID()
来源：http://swa.xziqi.cn

[U116] JS：类型检查（JSDoc）
来源：http://ovm.hywenlv.cn

/** @param {string} name */ function f(name) {}
来源：http://vpt.nwbrower.top

[U117] JS：单元测试
来源：http://ynx.tanke756.top

npm i -D vitest;  npx vitest
来源：http://oqm.hnqzz.top

[U118] JS：开发服务器
来源：http://jcc.zhijiandao.cn

npm i -D vite;  npx vite
来源：http://uoi.daxiang520.top

[U119] JS：生产构建
来源：http://hxj.cashguo.top

npx vite build
来源：http://ysm.ywan-chungtsiang.top

[U120] JS：读取环境变量（Vite）
来源：http://plk.yvedp.cn

import.meta.env.VITE_API_URL
来源：http://cpt.jqgufenzy.top

================================================================================
来源：http://hqm.hysaishi.cn

统计汇总
来源：http://hmf.yvedp.cn

================================================================================
来源：http://cew.cashguo.top

按语言统计（条）：
来源：http://nct.zhaomingkeji.xyz

Python ......... 252
来源：http://emk.kuanghao11.cn

PHP ............ 252
来源：http://wph.ehwqpu.com

JavaScript ..... 252
来源：http://mqz.hesvh.cn

TypeScript ..... 212
来源：http://mjr.aizwys.cn

Java ........... 212
来源：http://wsl.chenlongwang.top

Go ............. 212
来源：http://ujj.xziqi.cn

Ruby ........... 212
来源：http://uox.gzhubu.top

C# ............. 212
来源：http://tpa.yanxiufei.cn

C .............. 30
来源：http://lxt.gzhubu.top

C++ ............ 30
来源：http://iqa.zhaomingkeji.xyz

SQL ............ 90
来源：http://jwz.cqqwz.cn

Bash ........... 80
来源：http://cde.yuxming.cn

Kotlin ......... 15
来源：http://ljj.hywenlv.cn

Swift .......... 15
来源：http://slp.yvedp.cn

Lua ............ 10
来源：http://xwq.xziqi.cn

Perl ........... 10
来源：http://qih.sweek.top

Scala .......... 10
来源：http://ftg.jyoumei.cn

------------------------------------
来源：http://olp.dashuyun.cn

合计 ........... 2106 条
来源：http://ckw.jqgfzy.top

按章节统计：
来源：http://jzg.yongpay.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://foi.hywenlv.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://huh.yuxming.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://xob.shanyushiyangkeji.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://cuq.9152youxi.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://vuk.zhongyouzk.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://ayh.ehwqpu.com

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://lll.haohaochexian.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://eyu.yfazqb.com

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://lyb.pycfn.com

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://mkb.jinghuilouyu.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://ecp.daxiang520.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://brt.nanxuanxn.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://qpr.52xcode.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://kln.xinyue.icu

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://vbd.haohaochexian.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://rfw.pycfn.com

Q SQL 专题                              90
来源：http://lfm.dashuyun.cn

R Bash 专题                             80
来源：http://omf.52xcode.cn

S C / C++ 专题                          60
来源：http://rku.guowangkeji.top

T 其他语言补充                          60
来源：http://mpv.sufxvd.cn

U 高频实用片段                         120
来源：http://crq.zdqjudy.top

------------------------------------
来源：http://efr.ctjpmb.com

合计                                  2106 条
来源：http://vzm.316326.xyz

--------------------------------------------------------------------------------
来源：http://sfv.yfazqb.com

使用提醒
来源：http://sxo.gzhubu.top

--------------------------------------------------------------------------------
来源：http://ymt.cheryme.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://dqt.hammf.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://tni.yj202588.top


<!-- 参考信息 -->