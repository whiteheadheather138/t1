代发 wailian999

def add(a: Int, b: Int): Int = a + b
来源：http://kvm.yj202588.top

[T59] Scala：循环
来源：http://geg.ydjk.org.cn

for (i <- 1 to 10) println(i)
来源：http://ngd.shuidangran.top

[T60] Scala：折叠
来源：http://tvw.sweek.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://tbc.daria6918.cn

================================================================================
来源：http://nea.snrcjt.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://lxl.ywan-chungtsiang.top

================================================================================
来源：http://aph.tarul.cn

[U01] Py：创建虚拟环境
来源：http://ylx.0kj1m.cn

python -m venv .venv && source .venv/bin/activate
来源：http://sty.cheryme.top

[U02] Py：导出 / 安装依赖
来源：http://yhw.wangshuangyany.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://bvy.jinqigufen.top

[U03] Py：加载 .env 配置
来源：http://ymu.sjlbkw.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://xvy.tian-w.cn

[U04] Py：变量调试打印
来源：http://vfr.zdbjq.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://qhs.jqgufenzy.top

[U05] Py：列表去重且保序
来源：http://qkk.hysaishi.cn

list(dict.fromkeys(arr))
来源：http://vqq.jyoumei.cn

[U06] Py：合并两个字典
来源：http://sdy.hnqzz.top

{**a, **b}
来源：http://hsz.jinqigufen.top

[U07] Py：反转字典键值
来源：http://yxm.yfazqb.com

{v: k for k, v in d.items()}
来源：http://esw.gaohongyu789.top

[U08] Py：展平二维列表
来源：http://bgv.kuanghao11.cn

[y for x in nested for y in x]
来源：http://qru.vehdjk.com

[U09] Py：字典取最大值的键
来源：http://wkb.birdmap.top

max(d, key=d.get)
来源：http://qcn.zhengqikj.top

[U10] Py：按值排序字典
来源：http://uml.shanyushiyangkeji.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hse.fehbvm.com

[U11] Py：生成器表达式
来源：http://duy.jyoumei.cn

(x * 2 for x in arr)
来源：http://gis.mhx1999.top

[U12] Py：取出现最多的 3 个元素
来源：http://wos.pycfn.com

Counter(arr).most_common(3)
来源：http://jjs.9152youxi.cn

[U13] Py：固定长度队列
来源：http://ipv.hywenlv.cn

deque(maxlen=10)
来源：http://yjj.xingfuxueyuan.xyz

[U14] Py：分组收集到列表
来源：http://tdf.pycfn.com

defaultdict(list)
来源：http://iim.xuetiantiany.cn

[U15] Py：高精度计时
来源：http://qma.cqqwz.cn

t = time.perf_counter()
来源：http://uie.aibaodan.cn

[U16] Py：命令行参数解析
来源：http://vhw.ywan-chungtsiang.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://wjg.zhongyouzk.top

[U17] Py：初始化日志
来源：http://sfr.xinyue.icu

logging.basicConfig(level=logging.INFO)
来源：http://nav.ppjwa.cn

[U18] Py：预编译正则
来源：http://wnw.meibo888.top

pat = re.compile(r"\d+")
来源：http://etc.cqqwz.cn

[U19] Py：正则替换带回调
来源：http://qdp.tianlin.xyz

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://kxl.tianlin.xyz

[U20] Py：缓存函数结果
来源：http://qju.daria6918.cn

@functools.lru_cache(maxsize=None)
来源：http://yvt.vehdjk.com

[U21] Py：自定义上下文管理器
来源：http://qwm.nwbrower.top

@contextlib.contextmanager
来源：http://til.jinyuanbaomall.cn

[U22] Py：矩阵转置
来源：http://psd.jyoumei.cn

list(zip(*m))
来源：http://bmd.feifeiyinyue.top

[U23] Py：分块读取大文件
来源：http://dmt.xylfe.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://lpy.zhixingplan.top

[U24] Py：路径操作
来源：http://htw.yuxming.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://oqi.fzhhl.top

[U25] Py：CSV 按字典读
来源：http://lkh.zycfv.cn

csv.DictReader(f)
来源：http://ocy.cucudq.cn

[U26] Py：并发下载
来源：http://ozw.kuanghao11.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://bot.wangshuangyany.cn

[U27] Py：异步 HTTP
来源：http://xsc.yueranfly.top

aiohttp.ClientSession() 配合 async with
来源：http://soj.cucudq.cn

[U28] Py：类型别名
来源：http://twm.sufxvd.cn

UserId = int
来源：http://npn.hywenlv.cn

[U29] Py：属性校验
来源：http://ntk.xuanzx.com

@property 与 @x.setter 配合
来源：http://obc.zhiwuduotai.top

[U30] Py：数据类
来源：http://mze.fktsv.cn

@dataclass(slots=True)
来源：http://kkt.ctjpmb.com

[U31] Py：单测
来源：http://anw.jqgufenzy.top

python -m pytest -q
来源：http://izt.jinghuilouyu.cn

[U32] Py：代码格式化
来源：http://pxi.quarkkingdee.top

ruff format . && ruff check --fix .
来源：http://lgl.xinyue.icu

[U33] Py：打包发布
来源：http://hli.yj202588.top

python -m build  （依赖 pyproject.toml）
来源：http://fgs.hnqzz.top

[U34] Py：判断编码
来源：http://air.zhiwuduotai.top

chardet.detect(raw)
来源：http://ulo.yueranfly.top

[U35] Py：发送邮件
来源：http://ptb.tianlin.xyz

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://wwk.ydjk.org.cn

[U36] Py：定时任务
来源：http://rns.epnwcf.com

schedule.every(10).minutes.do(job)
来源：http://vsy.chenjidiqi.icu

[U37] Py：读写 Excel
来源：http://jnz.wangshuangyany.cn

pandas.read_excel / DataFrame.to_excel
来源：http://cun.sysykeji.top

[U38] Py：获取脚本所在目录
来源：http://zaz.jiagoushi.top

Path(__file__).resolve().parent
来源：http://jbl.yangfankeji.com

[U39] Py：判断是否在交互环境
来源：http://sns.cucudq.cn

sys.stdout.isatty()
来源：http://tfx.tian-w.cn

[U40] Py：打印到标准错误
来源：http://pcx.ehwqpu.com

print("err", file=sys.stderr)
来源：http://kdc.ctjpmb.com

[U41] PHP：初始化 Composer 项目
来源：http://igp.hnxiangtu.top

composer init;  composer require guzzlehttp/guzzle
来源：http://zgl.shanyushiyangtech.top

[U42] PHP：PSR-4 自动加载
来源：http://epz.xuanzx.com

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://nmq.zhijiandao.cn

[U43] PHP：声明命名空间
来源：http://glg.shzxlz.cn

namespace App\Http;
来源：http://dlr.iojbl.cn

[U44] PHP：开启严格类型
来源：http://qpw.jinghuilouyu.cn

declare(strict_types=1);
来源：http://szr.sjlbkw.cn

[U45] PHP：类型声明与返回类型
来源：http://kex.cdnleiting.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://wdj.dianchejie.cn

[U46] PHP：可空类型
来源：http://bim.jinghuilouyu.cn

?string $name = null
来源：http://ioh.cdnleiting.top

[U47] PHP：联合类型
来源：http://sse.uphjek.com

int|string $id
来源：http://cnl.ehwqpu.com

[U48] PHP：纯枚举
来源：http://ick.sxryk.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://xbh.0kj1m.cn

[U49] PHP：只读属性
来源：http://twp.bbcook.cn

public readonly string $name
来源：http://hvj.uphjek.com

[U50] PHP：构造器属性提升
来源：http://daa.gotoacloud.top

public function __construct(private int $id) {}
来源：http://wzg.hesvh.cn

[U51] PHP：数组解构
来源：http://tbr.epnwcf.com

[$a, $b] = $arr;
来源：http://qnv.chenzaomai.com

[U52] PHP：箭头函数
来源：http://vol.zhixingplan.top

$double = fn($x) => $x * 2;
来源：http://ruk.yuxming.cn

[U53] PHP：空合并运算符
来源：http://lkk.chenlongwang.top

$v = $a ?? $b ?? "default";
来源：http://obh.jinghuilouyu.cn

[U54] PHP：空安全调用
来源：http://hrc.ydzc1.top

$obj?->method()
来源：http://kqg.cucudq.cn

[U55] PHP：match 表达式
来源：http://ilh.haohaochexian.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://dss.shangyingyoupin.top

[U56] PHP：命名参数
来源：http://bji.quarkkingdee.top

f(a: 1, b: 2)
来源：http://jlb.hywenlv.cn

[U57] PHP：字符串插值
来源：http://ree.ydjk.org.cn

"值: {$a}"
来源：http://prk.fehbvm.com

[U58] PHP：数组三件套
来源：http://jxz.xziqi.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://fmy.hfpthk.cn

[U59] PHP：自定义排序
来源：http://eyt.uphjek.com

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://xji.birdmap.top

[U60] PHP：JSON 编解码
来源：http://fzq.hywenlv.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://epa.wangdashe.top

[U61] PHP：正则
来源：http://xkq.dashuyun.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://jqi.pycfn.com

[U62] PHP：日期对象
来源：http://zel.vehdjk.com

(new DateTimeImmutable())->format("Y-m-d");
来源：http://gzu.yj20258888.top

[U63] PHP：文件读写
来源：http://sas.chenlongwang.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://zyv.chenzaomai.com

[U64] PHP：目录遍历
来源：http://dtz.pengpengdd.cyou

glob("dir/*.php");  scandir("dir");
来源：http://bcw.shanyushiyangkeji.top

[U65] PHP：会话
来源：http://kok.xingfuxueyuan.xyz

session_start();  $_SESSION["uid"] = 1;
来源：http://zft.shzxlz.cn

[U66] PHP：设置 Cookie
来源：http://hfg.ppjwa.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://jja.zdbjq.cn

[U67] PHP：处理文件上传
来源：http://adz.cucudq.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://yka.jinghuilouyu.cn

[U68] PHP：PDO 连接
来源：http://eyo.uphjek.com

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://gls.9152youxi.cn

[U69] PHP：PDO 预处理
来源：http://geh.vehdjk.com

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://vfg.chenzaomai.com

[U70] PHP：PDO 事务
来源：http://fzg.wangshuangyany.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://acp.sxryk.cn

[U71] PHP：抛出异常
来源：http://qcb.quarkkingdee.top

throw new RuntimeException("失败", 500);
来源：http://xkx.wangshuangyany.cn

[U72] PHP：写错误日志
来源：http://ltg.jiagoushi.top

error_log("失败: " . $e->getMessage());
来源：http://sic.shanyushiyangtech.top

[U73] PHP：读取 ini 配置
来源：http://tbu.cashguo.top

parse_ini_file("config.ini", true)
来源：http://crr.hnxiangtu.top

[U74] PHP：读取环境变量
来源：http://pcl.hywenlv.cn

getenv("APP_ENV") ?: "production"
来源：http://nbw.yj20258888.top

[U75] PHP：依赖注入
来源：http://dng.smart0.xyz

composer require psr/container
来源：http://vfo.fanxiaobao.xyz

[U76] PHP：简单路由
来源：http://mzi.jinyuanbaomall.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://ffn.epnwcf.com

[U77] PHP：模板渲染
来源：http://bwv.yueranfly.top

composer require twig/twig
来源：http://mia.epnwcf.com

[U78] PHP：单元测试
来源：http://akg.haohaochexian.top

composer require --dev phpunit/phpunit
来源：http://jtu.hnqzz.top

[U79] PHP：静态分析
来源：http://nxo.epnwcf.com

composer require --dev phpstan/phpstan
来源：http://trm.zhiwuduotai.top

[U80] PHP：代码规范修复
来源：http://egd.daria6918.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://erv.uphjek.com

[U81] JS：初始化项目
来源：http://eiz.pengpengdd.cyou

npm init -y;  npm i express
来源：http://cbn.zhongyouzk.top

[U82] JS：package.json 脚本
来源：http://vkq.pycfn.com

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://fyt.wangdashe.top

[U83] JS：ES Module 导入导出
来源：http://tko.ehwqpu.com

export const a = 1;  import { a } from "./m.js";
来源：http://naj.xylfe.cn

[U84] JS：CommonJS 写法
来源：http://qzn.yanxiufei.cn

module.exports = { a };  const { a } = require("./m");
来源：http://cei.hnqzz.top

[U85] JS：可选链
来源：http://ltv.zycfv.cn

a?.b?.c
来源：http://mfv.hnxiangtu.top

[U86] JS：空值合并
来源：http://ifk.yj20258.top

a ?? b
来源：http://vlc.tanke756.top

[U87] JS：解构默认值
来源：http://hig.cucudq.cn

const { a = 1, b = 2 } = obj;
来源：http://fhm.cheryme.top

[U88] JS：对象展开合并
来源：http://tsk.yj20258.top

{ ...a, ...b }
来源：http://ugd.52xcode.cn

[U89] JS：数组去重
来源：http://xbd.quarkkingdee.top

[...new Set(arr)]
来源：http://mgc.jlsjyb.cn

[U90] JS：数字数组排序
来源：http://xsb.ydzc1.top

[...arr].sort((a, b) => a - b)
来源：http://msm.zhengqikj.top

[U91] JS：对象键值遍历
来源：http://mtw.jqgfzy.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://how.snrcjt.cn

[U92] JS：深拷贝
来源：http://krh.nanxinkj.top

structuredClone(obj)
来源：http://vyo.9152youxi.cn

[U93] JS：模板字符串
来源：http://bwc.guowangkeji.top

`共 ${n} 条`
来源：http://shz.hnxiangtu.top

[U94] JS：箭头函数
来源：http://miw.yongpay.top

const double = x => x * 2;
来源：http://wvt.bjfxy.top

[U95] JS：Promise 包装
来源：http://anz.andypj.xyz

new Promise((resolve, reject) => {})
来源：http://bzm.hywenlv.cn

[U96] JS：async/await 与异常
来源：http://ufy.wangshuangyany.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://qrn.uphjek.com

[U97] JS：并发请求
来源：http://csn.jqgfzy.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://gdm.jinqigfzy.top

[U98] JS：fetch 带 JSON
来源：http://pps.cqqwz.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://oin.dianchejie.cn

[U99] JS：事件监听
来源：http://uwq.zhaomingkeji.xyz

el.addEventListener("click", e => {})
来源：http://vji.xinyue.icu

[U100] JS：DOM 查询
来源：http://ead.ydjk.org.cn

document.querySelector(".item")
来源：http://jlz.kuanghao11.cn

[U101] JS：classList 操作
来源：http://yjj.c1oappe.top

el.classList.toggle("active")
来源：http://ylm.pycfn.com

[U102] JS：本地存储
来源：http://tao.ppjwa.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://vau.hammf.cn

[U103] JS：定时器
来源：http://csk.wangshuangyany.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://kxu.pengpengdd.cyou

[U104] JS：防抖
来源：http://lun.xziqi.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://gjq.yvedp.cn

[U105] JS：节流
来源：http://ryx.feifeiyinyue.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://puf.vqdsnc.cn

[U106] JS：日期格式化
来源：http://qho.wangshuangyany.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://shs.tanke756.top

[U107] JS：数字千分位
来源：http://ibn.sysykeji.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://awc.cdnleiting.top

[U108] JS：随机整数
来源：http://xlh.hnxiangtu.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://cyk.guowangkeji.top

[U109] JS：数组分组
来源：http://xvs.dashuyun.cn

Object.groupBy(arr, x => x.type)
来源：http://vfj.chenlongwang.top

[U110] JS：数组分块
来源：http://qti.hongshengwenyu.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://eqp.gogol.net.cn

[U111] JS：对象转 Map
来源：http://rex.yonumen.top

new Map(Object.entries(obj))
来源：http://qum.nanxuanxn.top

[U112] JS：字符串补位
来源：http://ohq.yj202588.top

"7".padStart(3, "0")
来源：http://zbf.sjlbkw.cn

[U113] JS：正则替换全部
来源：http://snt.fktsv.cn

s.replaceAll("a", "b")
来源：http://uag.chenjidiqi.icu

[U114] JS：JSON 深比较
来源：http://cut.havefunace.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://pps.yj20258.top

[U115] JS：生成 UUID
来源：http://cod.nwbrower.top

crypto.randomUUID()
来源：http://oum.zhengqikj.top

[U116] JS：类型检查（JSDoc）
来源：http://yeg.zdbjq.cn

/** @param {string} name */ function f(name) {}
来源：http://lbi.gaohongyu789.top

[U117] JS：单元测试
来源：http://blr.tian-w.cn

npm i -D vitest;  npx vitest
来源：http://epo.sxryk.cn

[U118] JS：开发服务器
来源：http://ylz.sufxvd.cn

npm i -D vite;  npx vite
来源：http://hjx.yueranfly.top

[U119] JS：生产构建
来源：http://xky.wangshuangyany.cn

npx vite build
来源：http://cgn.jyoumei.cn

[U120] JS：读取环境变量（Vite）
来源：http://fid.xylfe.cn

import.meta.env.VITE_API_URL
来源：http://cxc.fktsv.cn

================================================================================
来源：http://gdu.haohaochexian.top

统计汇总
来源：http://ydc.ehwqpu.com

================================================================================
来源：http://jbw.nanxinkj.top

按语言统计（条）：
来源：http://hkq.fzhhl.top

Python ......... 252
来源：http://fzw.shzxlz.cn

PHP ............ 252
来源：http://omf.haohaochexian.top

JavaScript ..... 252
来源：http://wbz.mhx1999.top

TypeScript ..... 212
来源：http://egb.shzxlz.cn

Java ........... 212
来源：http://yad.gaohongyu789.top

Go ............. 212
来源：http://gqx.birdmap.top

Ruby ........... 212
来源：http://rmg.pengpengdd.cyou

C# ............. 212
来源：http://nev.sweek.top

C .............. 30
来源：http://avm.zdbjq.cn

C++ ............ 30
来源：http://sed.cqqwz.cn

SQL ............ 90
来源：http://xyt.hysaishi.cn

Bash ........... 80
来源：http://gmk.yuxming.cn

Kotlin ......... 15
来源：http://yfy.jyoumei.cn

Swift .......... 15
来源：http://xzu.ywan-chungtsiang.top

Lua ............ 10
来源：http://zne.nanxuanxn.top

Perl ........... 10
来源：http://qjb.xuanzx.com

Scala .......... 10
来源：http://fky.ppjwa.cn

------------------------------------
来源：http://svp.shangyingyoupin.top

合计 ........... 2106 条
来源：http://hab.52xcode.cn

按章节统计：
来源：http://kmw.redwolf501.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://zqq.shangyingyoupin.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://ovq.shanyushiyangtech.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://oku.jqgufenzy.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://oou.hnxiangtu.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://saj.cashguo.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://zme.ehwqpu.com

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://ytj.52xcode.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://jny.ybcxt.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://cgt.jinghuilouyu.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://jdd.sweek.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://tfu.bjfxy.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://qvz.iojbl.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://sfj.xinyue.icu

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://skq.zdqjudy.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://ery.gotoacloud.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://qpp.jinqigufen.top

Q SQL 专题                              90
来源：http://ito.guowangkeji.top

R Bash 专题                             80
来源：http://grk.tian-w.cn

S C / C++ 专题                          60
来源：http://sfi.yj20258.top

T 其他语言补充                          60
来源：http://ntx.xziqi.cn

U 高频实用片段                         120
来源：http://jll.ybcxt.top

------------------------------------
来源：http://pvi.dashuyun.cn

合计                                  2106 条
来源：http://ley.redwolf501.top

--------------------------------------------------------------------------------
来源：http://zqg.zdbjq.cn

使用提醒
来源：http://moi.aibaodan.cn

--------------------------------------------------------------------------------
来源：http://mzr.vehdjk.com

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://dtz.sxryk.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://zbu.ywan-chungtsiang.top


<!-- 参考信息 -->