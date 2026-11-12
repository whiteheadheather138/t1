代发 wailian999

[U01] Py：创建虚拟环境
来源：http://idp.svipenyu.cn

python -m venv .venv && source .venv/bin/activate
来源：http://icb.daxiang520.top

[U02] Py：导出 / 安装依赖
来源：http://dkr.wangdashe.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://skj.guowangkeji.top

[U03] Py：加载 .env 配置
来源：http://ris.yuxming.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://zhi.ehwqpu.com

[U04] Py：变量调试打印
来源：http://zgy.haohaochexian.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://quu.haohaochexian.top

[U05] Py：列表去重且保序
来源：http://yly.vehdjk.com

list(dict.fromkeys(arr))
来源：http://isz.ywan-chungtsiang.top

[U06] Py：合并两个字典
来源：http://gdh.cashguo.top

{**a, **b}
来源：http://cna.jinqigfzy.top

[U07] Py：反转字典键值
来源：http://ocv.jqgufenzy.top

{v: k for k, v in d.items()}
来源：http://mqk.hfpthk.cn

[U08] Py：展平二维列表
来源：http://oyu.xinyue.icu

[y for x in nested for y in x]
来源：http://rho.gzhubu.top

[U09] Py：字典取最大值的键
来源：http://obg.sufxvd.cn

max(d, key=d.get)
来源：http://qjb.yanxiufei.cn

[U10] Py：按值排序字典
来源：http://cgz.xylfe.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://zjf.52xcode.cn

[U11] Py：生成器表达式
来源：http://tgu.jinghuilouyu.cn

(x * 2 for x in arr)
来源：http://szk.yonumen.top

[U12] Py：取出现最多的 3 个元素
来源：http://hna.zhengqikj.top

Counter(arr).most_common(3)
来源：http://vpj.cdnleiting.top

[U13] Py：固定长度队列
来源：http://xks.ppjwa.cn

deque(maxlen=10)
来源：http://tmv.fengsongda.top

[U14] Py：分组收集到列表
来源：http://sjm.zhoulong.xyz

defaultdict(list)
来源：http://dgj.shzxlz.cn

[U15] Py：高精度计时
来源：http://pvy.fengsongda.top

t = time.perf_counter()
来源：http://tfu.hnqzz.top

[U16] Py：命令行参数解析
来源：http://jsz.guowangkeji.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://flz.ivvv.top

[U17] Py：初始化日志
来源：http://ivf.zhengqikj.top

logging.basicConfig(level=logging.INFO)
来源：http://eik.sysykeji.top

[U18] Py：预编译正则
来源：http://aqk.yonumen.top

pat = re.compile(r"\d+")
来源：http://ler.chenjidiqi.icu

[U19] Py：正则替换带回调
来源：http://mgw.quarkkingdee.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://wfi.ctjpmb.com

[U20] Py：缓存函数结果
来源：http://mzo.sjlbkw.cn

@functools.lru_cache(maxsize=None)
来源：http://rhg.xylfe.cn

[U21] Py：自定义上下文管理器
来源：http://kii.pycfn.com

@contextlib.contextmanager
来源：http://sbk.jinyuanbaomall.cn

[U22] Py：矩阵转置
来源：http://pxt.fktsv.cn

list(zip(*m))
来源：http://ukj.shuidangran.top

[U23] Py：分块读取大文件
来源：http://rxw.jinqigufen.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://dqj.xylfe.cn

[U24] Py：路径操作
来源：http://bvb.aizwys.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://bdk.meibo888.top

[U25] Py：CSV 按字典读
来源：http://uxc.9152youxi.cn

csv.DictReader(f)
来源：http://loa.aibaodan.cn

[U26] Py：并发下载
来源：http://dyd.cqqwz.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://zmz.c1oappe.top

[U27] Py：异步 HTTP
来源：http://hmy.daria6918.cn

aiohttp.ClientSession() 配合 async with
来源：http://pbf.yonumen.top

[U28] Py：类型别名
来源：http://krq.yfazqb.com

UserId = int
来源：http://glz.yongpay.top

[U29] Py：属性校验
来源：http://vmy.nwbrower.top

@property 与 @x.setter 配合
来源：http://vwd.cheryme.top

[U30] Py：数据类
来源：http://wez.guowangkeji.top

@dataclass(slots=True)
来源：http://gbg.cucudq.cn

[U31] Py：单测
来源：http://gah.hysaishi.cn

python -m pytest -q
来源：http://uzu.andypj.xyz

[U32] Py：代码格式化
来源：http://lnz.pengpengdd.cyou

ruff format . && ruff check --fix .
来源：http://yvm.jinqigufen.top

[U33] Py：打包发布
来源：http://edr.xylfe.cn

python -m build  （依赖 pyproject.toml）
来源：http://leg.0kj1m.cn

[U34] Py：判断编码
来源：http://kbh.fanxiaobao.xyz

chardet.detect(raw)
来源：http://zig.ehwqpu.com

[U35] Py：发送邮件
来源：http://owl.yueranfly.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://diw.aibaodan.cn

[U36] Py：定时任务
来源：http://kmg.hcnkem.com

schedule.every(10).minutes.do(job)
来源：http://ptq.daria6918.cn

[U37] Py：读写 Excel
来源：http://gvb.shangyingyoupin.top

pandas.read_excel / DataFrame.to_excel
来源：http://vxt.tanke756.top

[U38] Py：获取脚本所在目录
来源：http://tbu.sjlbkw.cn

Path(__file__).resolve().parent
来源：http://qzf.vehdjk.com

[U39] Py：判断是否在交互环境
来源：http://rqo.hnxiangtu.top

sys.stdout.isatty()
来源：http://fic.yuanzhike.top

[U40] Py：打印到标准错误
来源：http://lqt.zhengqikj.top

print("err", file=sys.stderr)
来源：http://wby.yonumen.top

[U41] PHP：初始化 Composer 项目
来源：http://vdd.dashuyun.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://mvt.hnxiangtu.top

[U42] PHP：PSR-4 自动加载
来源：http://gcr.wangshuangyany.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://fwu.uphjek.com

[U43] PHP：声明命名空间
来源：http://zse.fktsv.cn

namespace App\Http;
来源：http://fmj.zhiwuduotai.top

[U44] PHP：开启严格类型
来源：http://qqd.bjfxy.top

declare(strict_types=1);
来源：http://glw.havefunace.top

[U45] PHP：类型声明与返回类型
来源：http://bsu.cdnleiting.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://psu.gotoacloud.top

[U46] PHP：可空类型
来源：http://mok.havefunace.top

?string $name = null
来源：http://sww.xuetiantiany.cn

[U47] PHP：联合类型
来源：http://zbw.dashuyun.cn

int|string $id
来源：http://ohx.jinghuilouyu.cn

[U48] PHP：纯枚举
来源：http://ghn.jiagoushi.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://urz.jianghu66.top

[U49] PHP：只读属性
来源：http://jja.hywenlv.cn

public readonly string $name
来源：http://vwu.svipenyu.cn

[U50] PHP：构造器属性提升
来源：http://gwv.zhiwuduotai.top

public function __construct(private int $id) {}
来源：http://kek.tanke756.top

[U51] PHP：数组解构
来源：http://sdo.guannengcc.top

[$a, $b] = $arr;
来源：http://hlh.cqqwz.cn

[U52] PHP：箭头函数
来源：http://aps.meibo888.top

$double = fn($x) => $x * 2;
来源：http://fnr.zhongyouzk.top

[U53] PHP：空合并运算符
来源：http://tey.c1oappe.top

$v = $a ?? $b ?? "default";
来源：http://pvj.wangshuangyany.cn

[U54] PHP：空安全调用
来源：http://mok.aibaodan.cn

$obj?->method()
来源：http://nas.jyoumei.cn

[U55] PHP：match 表达式
来源：http://gta.jinqigufen.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://bes.chenzaomai.com

[U56] PHP：命名参数
来源：http://dip.jyoumei.cn

f(a: 1, b: 2)
来源：http://ujy.gogol.net.cn

[U57] PHP：字符串插值
来源：http://lgt.hysaishi.cn

"值: {$a}"
来源：http://tcn.shangyingyoupin.top

[U58] PHP：数组三件套
来源：http://nhv.daxiang520.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://ieu.sxryk.cn

[U59] PHP：自定义排序
来源：http://wmz.jyoumei.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://jmv.jinghuilouyu.cn

[U60] PHP：JSON 编解码
来源：http://rut.fehbvm.com

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://ueo.jiagoushi.top

[U61] PHP：正则
来源：http://jmm.feifeiyinyue.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://zcf.havefunace.top

[U62] PHP：日期对象
来源：http://xkf.redwolf501.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://xyw.zycfv.cn

[U63] PHP：文件读写
来源：http://dzk.hnxiangtu.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://cfe.jqgufenzy.top

[U64] PHP：目录遍历
来源：http://cgq.ehwqpu.com

glob("dir/*.php");  scandir("dir");
来源：http://fyj.hesvh.cn

[U65] PHP：会话
来源：http://iqm.yongpay.top

session_start();  $_SESSION["uid"] = 1;
来源：http://oso.ppjwa.cn

[U66] PHP：设置 Cookie
来源：http://ixf.hysaishi.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://flu.bbcook.cn

[U67] PHP：处理文件上传
来源：http://flb.yangfankeji.com

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://vfk.gogol.net.cn

[U68] PHP：PDO 连接
来源：http://tda.jinghuilouyu.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://eep.9152youxi.cn

[U69] PHP：PDO 预处理
来源：http://tgj.jqgfzy.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://omi.jlsjyb.cn

[U70] PHP：PDO 事务
来源：http://wvf.yuanzhike.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://uuo.dianchejie.cn

[U71] PHP：抛出异常
来源：http://jvs.snrcjt.cn

throw new RuntimeException("失败", 500);
来源：http://hui.nwbrower.top

[U72] PHP：写错误日志
来源：http://ghv.hysaishi.cn

error_log("失败: " . $e->getMessage());
来源：http://ibq.gogol.net.cn

[U73] PHP：读取 ini 配置
来源：http://iqm.hysaishi.cn

parse_ini_file("config.ini", true)
来源：http://woz.havefunace.top

[U74] PHP：读取环境变量
来源：http://lwg.xylfe.cn

getenv("APP_ENV") ?: "production"
来源：http://huj.chenjidiqi.icu

[U75] PHP：依赖注入
来源：http://lay.fengsongda.top

composer require psr/container
来源：http://nob.zhixingplan.top

[U76] PHP：简单路由
来源：http://vjk.ppjwa.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://yxi.hnxiangtu.top

[U77] PHP：模板渲染
来源：http://vvv.0kj1m.cn

composer require twig/twig
来源：http://aqk.yongpay.top

[U78] PHP：单元测试
来源：http://aux.jiagoushi.top

composer require --dev phpunit/phpunit
来源：http://xhj.jinqigufen.top

[U79] PHP：静态分析
来源：http://gyx.zhixingplan.top

composer require --dev phpstan/phpstan
来源：http://qyn.chenjidiqi.icu

[U80] PHP：代码规范修复
来源：http://obj.hesvh.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://wkb.ydjk.org.cn

[U81] JS：初始化项目
来源：http://yun.aizwys.cn

npm init -y;  npm i express
来源：http://jls.ppjwa.cn

[U82] JS：package.json 脚本
来源：http://cfe.tanke756.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://sko.zhaomingkeji.xyz

[U83] JS：ES Module 导入导出
来源：http://sek.jianghu66.top

export const a = 1;  import { a } from "./m.js";
来源：http://vyu.pycfn.com

[U84] JS：CommonJS 写法
来源：http://svu.zhixingplan.top

module.exports = { a };  const { a } = require("./m");
来源：http://sdl.shanyushiyangkeji.top

[U85] JS：可选链
来源：http://fvy.fanxiaobao.xyz

a?.b?.c
来源：http://cxt.fengsongda.top

[U86] JS：空值合并
来源：http://ikk.tanke756.top

a ?? b
来源：http://eef.hfpthk.cn

[U87] JS：解构默认值
来源：http://pdi.cqqwz.cn

const { a = 1, b = 2 } = obj;
来源：http://ips.cqqwz.cn

[U88] JS：对象展开合并
来源：http://yyl.dianchejie.cn

{ ...a, ...b }
来源：http://djg.gogol.net.cn

[U89] JS：数组去重
来源：http://azp.sweek.top

[...new Set(arr)]
来源：http://cdl.chenlongwang.top

[U90] JS：数字数组排序
来源：http://ytw.yuxming.cn

[...arr].sort((a, b) => a - b)
来源：http://evk.hysaishi.cn

[U91] JS：对象键值遍历
来源：http://okw.hnqzz.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://zjy.yuxming.cn

[U92] JS：深拷贝
来源：http://znu.yongpay.top

structuredClone(obj)
来源：http://pfl.jinqigfzy.top

[U93] JS：模板字符串
来源：http://yuo.jianghu66.top

`共 ${n} 条`
来源：http://aob.jqgfzy.top

[U94] JS：箭头函数
来源：http://uwz.jyoumei.cn

const double = x => x * 2;
来源：http://wbp.yfazqb.com

[U95] JS：Promise 包装
来源：http://lcm.hesvh.cn

new Promise((resolve, reject) => {})
来源：http://skh.guannengcc.top

[U96] JS：async/await 与异常
来源：http://hyy.fengsongda.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://ytc.sxryk.cn

[U97] JS：并发请求
来源：http://mnn.yvedp.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://orl.c1oappe.top

[U98] JS：fetch 带 JSON
来源：http://ndc.vqdsnc.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://xwi.zhaomingkeji.xyz

[U99] JS：事件监听
来源：http://myg.fanxiaobao.xyz

el.addEventListener("click", e => {})
来源：http://dsn.0kj1m.cn

[U100] JS：DOM 查询
来源：http://sqq.hnxiangtu.top

document.querySelector(".item")
来源：http://bxf.gzhubu.top

[U101] JS：classList 操作
来源：http://mzm.ydjk.org.cn

el.classList.toggle("active")
来源：http://gnw.fehbvm.com

[U102] JS：本地存储
来源：http://ztj.nanxinkj.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://noe.shanyushiyangtech.top

[U103] JS：定时器
来源：http://www.guannengcc.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://ize.hcnkem.com

[U104] JS：防抖
来源：http://fok.sjlbkw.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://bxd.hammf.cn

[U105] JS：节流
来源：http://hpg.daria6918.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://etg.zhoulong.xyz

[U106] JS：日期格式化
来源：http://gon.xylfe.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://nss.xinyue.icu

[U107] JS：数字千分位
来源：http://oha.316326.xyz

new Intl.NumberFormat("en-US").format(1234567)
来源：http://pgs.wangdashe.top

[U108] JS：随机整数
来源：http://yxk.haohaochexian.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://xub.sufxvd.cn

[U109] JS：数组分组
来源：http://vmo.guannengcc.top

Object.groupBy(arr, x => x.type)
来源：http://moz.jinyuanbaomall.cn

[U110] JS：数组分块
来源：http://yuh.yj202588.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://fxr.gzhubu.top

[U111] JS：对象转 Map
来源：http://ezi.cqqwz.cn

new Map(Object.entries(obj))
来源：http://dmm.nwbrower.top

[U112] JS：字符串补位
来源：http://qgo.vqdsnc.cn

"7".padStart(3, "0")
来源：http://bfn.redwolf501.top

[U113] JS：正则替换全部
来源：http://gnf.hesvh.cn

s.replaceAll("a", "b")
来源：http://eit.meibo888.top

[U114] JS：JSON 深比较
来源：http://dxb.dianchejie.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://qpj.zhongyouzk.top

[U115] JS：生成 UUID
来源：http://bwa.jinghuilouyu.cn

crypto.randomUUID()
来源：http://fji.aibaodan.cn

[U116] JS：类型检查（JSDoc）
来源：http://rut.kuanghao11.cn

/** @param {string} name */ function f(name) {}
来源：http://bcu.shuidangran.top

[U117] JS：单元测试
来源：http://nxh.ehwqpu.com

npm i -D vitest;  npx vitest
来源：http://cch.wangshuangyany.cn

[U118] JS：开发服务器
来源：http://wdb.hnqzz.top

npm i -D vite;  npx vite
来源：http://enk.fzhhl.top

[U119] JS：生产构建
来源：http://lwa.havefunace.top

npx vite build
来源：http://aqk.xuetiantiany.cn

[U120] JS：读取环境变量（Vite）
来源：http://tdz.birdmap.top

import.meta.env.VITE_API_URL
来源：http://ave.hammf.cn

================================================================================
来源：http://fqe.hywenlv.cn

统计汇总
来源：http://tog.jinqigufen.top

================================================================================
来源：http://tjv.wangdashe.top

按语言统计（条）：
来源：http://xng.redwolf501.top

Python ......... 252
来源：http://crx.zdqjudy.top

PHP ............ 252
来源：http://szv.ivvv.top

JavaScript ..... 252
来源：http://lti.gogol.net.cn

TypeScript ..... 212
来源：http://omd.chenjidiqi.icu

Java ........... 212
来源：http://pzj.wangshuangyany.cn

Go ............. 212
来源：http://iog.cdnleiting.top

Ruby ........... 212
来源：http://kez.aizwys.cn

C# ............. 212
来源：http://viu.hnxiangtu.top

C .............. 30
来源：http://bpd.yongpay.top

C++ ............ 30
来源：http://iac.tarul.cn

SQL ............ 90
来源：http://shj.jinghuilouyu.cn

Bash ........... 80
来源：http://ocl.ywan-chungtsiang.top

Kotlin ......... 15
来源：http://lsk.sysykeji.top

Swift .......... 15
来源：http://ceo.quarkkingdee.top

Lua ............ 10
来源：http://ccr.daxiang520.top

Perl ........... 10
来源：http://xpt.mhx1999.top

Scala .......... 10
来源：http://woa.aibaodan.cn

------------------------------------
来源：http://poj.yvedp.cn

合计 ........... 2106 条
来源：http://wza.ppjwa.cn

按章节统计：
来源：http://iwu.jqgfzy.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://bss.ydjk.org.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://zjl.pengpengdd.cyou

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://rtk.daria6918.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://gzf.shanyushiyangkeji.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://cuq.jqgufenzy.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://gbd.shangyingyoupin.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://vry.cashguo.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://etb.xuanzx.com

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://bwg.meibo888.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://zfi.hnqzz.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://pbc.aibaodan.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://uel.smart0.xyz

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://rxf.hywenlv.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://qtd.snrcjt.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://ieu.guannengcc.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://pzc.tarul.cn

Q SQL 专题                              90
来源：http://ipm.jiagoushi.top

R Bash 专题                             80
来源：http://kfr.uphjek.com

S C / C++ 专题                          60
来源：http://zak.hesvh.cn

T 其他语言补充                          60
来源：http://wpx.316326.xyz

U 高频实用片段                         120
来源：http://avb.jinqigufen.top

------------------------------------
来源：http://pwy.yj20258888.top

合计                                  2106 条
来源：http://hny.dianchejie.cn

--------------------------------------------------------------------------------
来源：http://hqc.daxiang520.top

使用提醒
来源：http://xvw.meibo888.top

--------------------------------------------------------------------------------
来源：http://pvn.zhoulong.xyz

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://grb.ivvv.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://byu.bbcook.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://ozj.yonumen.top

在旧版本上使用前请先确认语法支持情况。
来源：http://kvh.gogol.net.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://hjq.fktsv.cn

—— 文件结束 ——
来源：http://uiy.jinqigfzy.top

================================================================================
来源：http://gsk.chenlongwang.top

程序语言常见例子速查手册（2024 版）
来源：http://uau.birdmap.top

Common Programming Examples Cheat Book
来源：http://etv.ctjpmb.com

================================================================================
来源：http://ywv.hongshengwenyu.top


<!-- 参考信息 -->