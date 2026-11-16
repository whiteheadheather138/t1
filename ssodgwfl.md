代发 wailian999

[U01] Py：创建虚拟环境
来源：http://aui.jinqigfzy.top

python -m venv .venv && source .venv/bin/activate
来源：http://swq.yuxming.cn

[U02] Py：导出 / 安装依赖
来源：http://gzy.zhiwuduotai.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://kku.xinyue.icu

[U03] Py：加载 .env 配置
来源：http://frm.nanxinkj.top

from dotenv import load_dotenv; load_dotenv()
来源：http://xsz.fanxiaobao.xyz

[U04] Py：变量调试打印
来源：http://emh.yuanzhike.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://isp.tianlin.xyz

[U05] Py：列表去重且保序
来源：http://oyk.yonumen.top

list(dict.fromkeys(arr))
来源：http://gov.hysaishi.cn

[U06] Py：合并两个字典
来源：http://bbu.fktsv.cn

{**a, **b}
来源：http://cdf.kuanghao11.cn

[U07] Py：反转字典键值
来源：http://but.sxryk.cn

{v: k for k, v in d.items()}
来源：http://mvq.quarkkingdee.top

[U08] Py：展平二维列表
来源：http://bnu.ywan-chungtsiang.top

[y for x in nested for y in x]
来源：http://ncg.sweek.top

[U09] Py：字典取最大值的键
来源：http://tku.feifeiyinyue.top

max(d, key=d.get)
来源：http://rmp.tanke756.top

[U10] Py：按值排序字典
来源：http://sms.yongpay.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://jay.ehwqpu.com

[U11] Py：生成器表达式
来源：http://spc.pycfn.com

(x * 2 for x in arr)
来源：http://gyl.yuxming.cn

[U12] Py：取出现最多的 3 个元素
来源：http://hjz.zhoulong.xyz

Counter(arr).most_common(3)
来源：http://adp.shzxlz.cn

[U13] Py：固定长度队列
来源：http://sec.fanxiaobao.xyz

deque(maxlen=10)
来源：http://nag.feifeiyinyue.top

[U14] Py：分组收集到列表
来源：http://kgo.cheryme.top

defaultdict(list)
来源：http://glk.hongshengwenyu.top

[U15] Py：高精度计时
来源：http://jhq.yuanzhike.top

t = time.perf_counter()
来源：http://wjb.yj202588.top

[U16] Py：命令行参数解析
来源：http://oqs.nanxinkj.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://heg.feifeiyinyue.top

[U17] Py：初始化日志
来源：http://ppt.jiagoushi.top

logging.basicConfig(level=logging.INFO)
来源：http://gnt.snrcjt.cn

[U18] Py：预编译正则
来源：http://ici.ehwqpu.com

pat = re.compile(r"\d+")
来源：http://qcx.haohaochexian.top

[U19] Py：正则替换带回调
来源：http://dwg.daria6918.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://ppb.yonumen.top

[U20] Py：缓存函数结果
来源：http://qwq.aizwys.cn

@functools.lru_cache(maxsize=None)
来源：http://fbi.zhaomingkeji.xyz

[U21] Py：自定义上下文管理器
来源：http://dph.hongshengwenyu.top

@contextlib.contextmanager
来源：http://rbk.fengsongda.top

[U22] Py：矩阵转置
来源：http://itg.yanxiufei.cn

list(zip(*m))
来源：http://asf.shuidangran.top

[U23] Py：分块读取大文件
来源：http://aqk.chenjidiqi.icu

for chunk in iter(lambda: f.read(8192), b""):
来源：http://gme.epnwcf.com

[U24] Py：路径操作
来源：http://fqg.yj20258.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://tds.zhiwuduotai.top

[U25] Py：CSV 按字典读
来源：http://jty.chenzaomai.com

csv.DictReader(f)
来源：http://chz.smart0.xyz

[U26] Py：并发下载
来源：http://psk.gzhubu.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://iyx.guannengcc.top

[U27] Py：异步 HTTP
来源：http://wwi.chenjidiqi.icu

aiohttp.ClientSession() 配合 async with
来源：http://hag.sufxvd.cn

[U28] Py：类型别名
来源：http://vrq.bjfxy.top

UserId = int
来源：http://bxa.sysykeji.top

[U29] Py：属性校验
来源：http://zdx.fengsongda.top

@property 与 @x.setter 配合
来源：http://lwo.cqqwz.cn

[U30] Py：数据类
来源：http://kum.zhaomingkeji.xyz

@dataclass(slots=True)
来源：http://dbv.fengsongda.top

[U31] Py：单测
来源：http://aut.yanxiufei.cn

python -m pytest -q
来源：http://ksx.jinqigufen.top

[U32] Py：代码格式化
来源：http://otm.cdnleiting.top

ruff format . && ruff check --fix .
来源：http://eth.zhongyouzk.top

[U33] Py：打包发布
来源：http://iue.shanyushiyangkeji.top

python -m build  （依赖 pyproject.toml）
来源：http://tlm.fehbvm.com

[U34] Py：判断编码
来源：http://ozb.bbcook.cn

chardet.detect(raw)
来源：http://emn.jinghuilouyu.cn

[U35] Py：发送邮件
来源：http://rup.shuidangran.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://lvo.vqdsnc.cn

[U36] Py：定时任务
来源：http://con.yj20258888.top

schedule.every(10).minutes.do(job)
来源：http://qti.yvedp.cn

[U37] Py：读写 Excel
来源：http://smw.snrcjt.cn

pandas.read_excel / DataFrame.to_excel
来源：http://tmp.yj20258.top

[U38] Py：获取脚本所在目录
来源：http://heo.fanxiaobao.xyz

Path(__file__).resolve().parent
来源：http://mcl.yj202588.top

[U39] Py：判断是否在交互环境
来源：http://cps.chenlongwang.top

sys.stdout.isatty()
来源：http://ehr.fktsv.cn

[U40] Py：打印到标准错误
来源：http://tqs.nwbrower.top

print("err", file=sys.stderr)
来源：http://hol.aibaodan.cn

[U41] PHP：初始化 Composer 项目
来源：http://oku.nanxuanxn.top

composer init;  composer require guzzlehttp/guzzle
来源：http://cxn.kuanghao11.cn

[U42] PHP：PSR-4 自动加载
来源：http://isy.cucudq.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://ccc.zycfv.cn

[U43] PHP：声明命名空间
来源：http://ubv.shangyingyoupin.top

namespace App\Http;
来源：http://reh.meibo888.top

[U44] PHP：开启严格类型
来源：http://umz.aizwys.cn

declare(strict_types=1);
来源：http://msk.vqdsnc.cn

[U45] PHP：类型声明与返回类型
来源：http://aco.guannengcc.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://lhj.yanxiufei.cn

[U46] PHP：可空类型
来源：http://xfx.cdnleiting.top

?string $name = null
来源：http://lwn.aizwys.cn

[U47] PHP：联合类型
来源：http://elh.cucudq.cn

int|string $id
来源：http://axr.sjlbkw.cn

[U48] PHP：纯枚举
来源：http://xyp.cqqwz.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://tlz.quarkkingdee.top

[U49] PHP：只读属性
来源：http://dyo.feifeiyinyue.top

public readonly string $name
来源：http://qbz.chenzaomai.com

[U50] PHP：构造器属性提升
来源：http://kkz.hywenlv.cn

public function __construct(private int $id) {}
来源：http://dkj.jiagoushi.top

[U51] PHP：数组解构
来源：http://qlj.xziqi.cn

[$a, $b] = $arr;
来源：http://lwd.hywenlv.cn

[U52] PHP：箭头函数
来源：http://sib.ctjpmb.com

$double = fn($x) => $x * 2;
来源：http://yvh.tianlin.xyz

[U53] PHP：空合并运算符
来源：http://ctt.yfazqb.com

$v = $a ?? $b ?? "default";
来源：http://wgu.ivvv.top

[U54] PHP：空安全调用
来源：http://vgv.hesvh.cn

$obj?->method()
来源：http://vqx.ppjwa.cn

[U55] PHP：match 表达式
来源：http://htv.bjfxy.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://jqr.yanxiufei.cn

[U56] PHP：命名参数
来源：http://ecf.shangyingyoupin.top

f(a: 1, b: 2)
来源：http://whw.wangdashe.top

[U57] PHP：字符串插值
来源：http://xjk.xziqi.cn

"值: {$a}"
来源：http://hgi.jqgfzy.top

[U58] PHP：数组三件套
来源：http://fkk.52xcode.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://qpb.zdqjudy.top

[U59] PHP：自定义排序
来源：http://ovv.jqgfzy.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://whe.hnqzz.top

[U60] PHP：JSON 编解码
来源：http://jzf.shzxlz.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://sbk.yongpay.top

[U61] PHP：正则
来源：http://kuj.chenjidiqi.icu

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://gbc.yonumen.top

[U62] PHP：日期对象
来源：http://bdc.aibaodan.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hqy.yvedp.cn

[U63] PHP：文件读写
来源：http://tce.9152youxi.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://vbk.bbcook.cn

[U64] PHP：目录遍历
来源：http://xen.bjfxy.top

glob("dir/*.php");  scandir("dir");
来源：http://ehe.jinghuilouyu.cn

[U65] PHP：会话
来源：http://klb.sjlbkw.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://ujz.iojbl.cn

[U66] PHP：设置 Cookie
来源：http://gef.yongpay.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://ygs.guannengcc.top

[U67] PHP：处理文件上传
来源：http://bcq.haohaochexian.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://ztv.ivvv.top

[U68] PHP：PDO 连接
来源：http://qnr.yuanzhike.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://xnl.jiagoushi.top

[U69] PHP：PDO 预处理
来源：http://erf.kuanghao11.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://roj.xuanzx.com

[U70] PHP：PDO 事务
来源：http://bus.meibo888.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://neo.nanxinkj.top

[U71] PHP：抛出异常
来源：http://uoh.shanyushiyangkeji.top

throw new RuntimeException("失败", 500);
来源：http://sqy.zdbjq.cn

[U72] PHP：写错误日志
来源：http://qcu.redwolf501.top

error_log("失败: " . $e->getMessage());
来源：http://djw.iojbl.cn

[U73] PHP：读取 ini 配置
来源：http://hbb.c1oappe.top

parse_ini_file("config.ini", true)
来源：http://bso.yvedp.cn

[U74] PHP：读取环境变量
来源：http://dnh.chenlongwang.top

getenv("APP_ENV") ?: "production"
来源：http://uoy.snrcjt.cn

[U75] PHP：依赖注入
来源：http://xzb.chenlongwang.top

composer require psr/container
来源：http://ovr.fktsv.cn

[U76] PHP：简单路由
来源：http://aid.vqdsnc.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://xot.vqdsnc.cn

[U77] PHP：模板渲染
来源：http://plq.yj20258.top

composer require twig/twig
来源：http://cdp.hongshengwenyu.top

[U78] PHP：单元测试
来源：http://ahv.cheryme.top

composer require --dev phpunit/phpunit
来源：http://yus.tian-w.cn

[U79] PHP：静态分析
来源：http://sun.xuanzx.com

composer require --dev phpstan/phpstan
来源：http://qfo.zhoulong.xyz

[U80] PHP：代码规范修复
来源：http://lpx.nanxinkj.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://qzb.jinyuanbaomall.cn

[U81] JS：初始化项目
来源：http://vqz.gaohongyu789.top

npm init -y;  npm i express
来源：http://fkn.sjlbkw.cn

[U82] JS：package.json 脚本
来源：http://grh.tian-w.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://ukt.hywenlv.cn

[U83] JS：ES Module 导入导出
来源：http://xxv.c1oappe.top

export const a = 1;  import { a } from "./m.js";
来源：http://kix.smart0.xyz

[U84] JS：CommonJS 写法
来源：http://tzk.smart0.xyz

module.exports = { a };  const { a } = require("./m");
来源：http://rxc.cqqwz.cn

[U85] JS：可选链
来源：http://dhj.bbcook.cn

a?.b?.c
来源：http://ted.zhoulong.xyz

[U86] JS：空值合并
来源：http://rjj.hysaishi.cn

a ?? b
来源：http://xcr.c1oappe.top

[U87] JS：解构默认值
来源：http://top.cheryme.top

const { a = 1, b = 2 } = obj;
来源：http://ufy.cashguo.top

[U88] JS：对象展开合并
来源：http://wpq.nwbrower.top

{ ...a, ...b }
来源：http://zwn.yj20258.top

[U89] JS：数组去重
来源：http://rbn.hesvh.cn

[...new Set(arr)]
来源：http://vyo.zhongyouzk.top

[U90] JS：数字数组排序
来源：http://sem.ctjpmb.com

[...arr].sort((a, b) => a - b)
来源：http://trs.dianchejie.cn

[U91] JS：对象键值遍历
来源：http://epv.cucudq.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://glf.jqgufenzy.top

[U92] JS：深拷贝
来源：http://qay.sweek.top

structuredClone(obj)
来源：http://zwp.daxiang520.top

[U93] JS：模板字符串
来源：http://ebo.hfpthk.cn

`共 ${n} 条`
来源：http://rvc.ybcxt.top

[U94] JS：箭头函数
来源：http://ntg.jinyuanbaomall.cn

const double = x => x * 2;
来源：http://lxm.cqqwz.cn

[U95] JS：Promise 包装
来源：http://ura.yvedp.cn

new Promise((resolve, reject) => {})
来源：http://zgd.ydzc1.top

[U96] JS：async/await 与异常
来源：http://crz.cdnleiting.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://ecw.wangshuangyany.cn

[U97] JS：并发请求
来源：http://etq.iojbl.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://hhj.epnwcf.com

[U98] JS：fetch 带 JSON
来源：http://vzq.haohaochexian.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://sfr.ppjwa.cn

[U99] JS：事件监听
来源：http://adn.sysykeji.top

el.addEventListener("click", e => {})
来源：http://vqv.andypj.xyz

[U100] JS：DOM 查询
来源：http://pyd.zhixingplan.top

document.querySelector(".item")
来源：http://hkn.snrcjt.cn

[U101] JS：classList 操作
来源：http://wzm.yuanzhike.top

el.classList.toggle("active")
来源：http://qyb.jinyuanbaomall.cn

[U102] JS：本地存储
来源：http://dbw.haohaochexian.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://bdl.nwbrower.top

[U103] JS：定时器
来源：http://rjo.tarul.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://mvk.zhixingplan.top

[U104] JS：防抖
来源：http://iax.ctjpmb.com

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://fyl.zdbjq.cn

[U105] JS：节流
来源：http://rlw.iojbl.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://vre.yvedp.cn

[U106] JS：日期格式化
来源：http://jsu.dianchejie.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://jmg.redwolf501.top

[U107] JS：数字千分位
来源：http://jnl.jyoumei.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://htk.52xcode.cn

[U108] JS：随机整数
来源：http://lyu.jinyuanbaomall.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://gwc.iojbl.cn

[U109] JS：数组分组
来源：http://wmj.xylfe.cn

Object.groupBy(arr, x => x.type)
来源：http://ebe.yuanzhike.top

[U110] JS：数组分块
来源：http://wze.cdnleiting.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://lvf.zhixingplan.top

[U111] JS：对象转 Map
来源：http://lml.fengsongda.top

new Map(Object.entries(obj))
来源：http://znu.xinyue.icu

[U112] JS：字符串补位
来源：http://skb.sweek.top

"7".padStart(3, "0")
来源：http://gls.xinyue.icu

[U113] JS：正则替换全部
来源：http://jgh.xinyue.icu

s.replaceAll("a", "b")
来源：http://afw.gzhubu.top

[U114] JS：JSON 深比较
来源：http://mfc.iojbl.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://cfc.zhaomingkeji.xyz

[U115] JS：生成 UUID
来源：http://fng.nwbrower.top

crypto.randomUUID()
来源：http://fxz.gzhubu.top

[U116] JS：类型检查（JSDoc）
来源：http://szz.c1oappe.top

/** @param {string} name */ function f(name) {}
来源：http://vjo.fzhhl.top

[U117] JS：单元测试
来源：http://ogz.birdmap.top

npm i -D vitest;  npx vitest
来源：http://qpr.havefunace.top

[U118] JS：开发服务器
来源：http://dhv.yj20258.top

npm i -D vite;  npx vite
来源：http://slw.chenjidiqi.icu

[U119] JS：生产构建
来源：http://zhi.hywenlv.cn

npx vite build
来源：http://uql.sxryk.cn

[U120] JS：读取环境变量（Vite）
来源：http://nka.guannengcc.top

import.meta.env.VITE_API_URL
来源：http://yba.nanxuanxn.top

================================================================================
来源：http://oqb.dashuyun.cn

统计汇总
来源：http://lvi.fengsongda.top

================================================================================
来源：http://klr.guowangkeji.top

按语言统计（条）：
来源：http://yyr.hfpthk.cn

Python ......... 252
来源：http://esz.sufxvd.cn

PHP ............ 252
来源：http://fbg.hfpthk.cn

JavaScript ..... 252
来源：http://yzb.fengsongda.top

TypeScript ..... 212
来源：http://sjt.yj202588.top

Java ........... 212
来源：http://ahm.hammf.cn

Go ............. 212
来源：http://fmo.ydzc1.top

Ruby ........... 212
来源：http://frb.epnwcf.com

C# ............. 212
来源：http://mam.yanxiufei.cn

C .............. 30
来源：http://ecs.zhaomingkeji.xyz

C++ ............ 30
来源：http://tuw.bjfxy.top

SQL ............ 90
来源：http://wey.ydzc1.top

Bash ........... 80
来源：http://azs.ivvv.top

Kotlin ......... 15
来源：http://gyh.hcnkem.com

Swift .......... 15
来源：http://udo.mhx1999.top

Lua ............ 10
来源：http://csr.jinyuanbaomall.cn

Perl ........... 10
来源：http://npe.shanyushiyangtech.top

Scala .......... 10
来源：http://dds.gogol.net.cn

------------------------------------
来源：http://zfu.smart0.xyz

合计 ........... 2106 条
来源：http://yko.meibo888.top

按章节统计：
来源：http://wuc.fengsongda.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://trv.mhx1999.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://gqy.andypj.xyz

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://yyk.tian-w.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://meu.kuanghao11.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://nig.yj20258.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://qxd.dashuyun.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://ala.pengpengdd.cyou

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://act.pengpengdd.cyou

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://fsb.aibaodan.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://uee.9152youxi.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://kfy.zhongyouzk.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://caz.shanyushiyangkeji.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://qqf.52xcode.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://hdz.jlsjyb.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://afl.aibaodan.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://ctf.hcnkem.com

Q SQL 专题                              90
来源：http://nbz.iojbl.cn

R Bash 专题                             80
来源：http://cyl.pycfn.com

S C / C++ 专题                          60
来源：http://xxa.guannengcc.top

T 其他语言补充                          60
来源：http://jzx.vehdjk.com

U 高频实用片段                         120
来源：http://lgf.vehdjk.com

------------------------------------
来源：http://qyd.ehwqpu.com

合计                                  2106 条
来源：http://ywt.316326.xyz

--------------------------------------------------------------------------------
来源：http://tpy.kuanghao11.cn

使用提醒
来源：http://wwy.sufxvd.cn

--------------------------------------------------------------------------------
来源：http://tti.feifeiyinyue.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://obp.tianlin.xyz

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://lxv.yonumen.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://ujv.sufxvd.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://bmk.dashuyun.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://wlm.fzhhl.top

—— 文件结束 ——
来源：http://kmy.ppjwa.cn

================================================================================
来源：http://ppe.hongshengwenyu.top

程序语言常见例子速查手册（2024 版）
来源：http://aev.hesvh.cn

Common Programming Examples Cheat Book
来源：http://tbb.hfpthk.cn

================================================================================
来源：http://qzq.xziqi.cn


<!-- 参考信息 -->