代发 wailian999

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://bjn.zhaomingkeji.xyz

================================================================================
来源：http://rra.zhijiandao.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://vkj.shanyushiyangkeji.top

================================================================================
来源：http://pna.redwolf501.top

[U01] Py：创建虚拟环境
来源：http://xbg.yueranfly.top

python -m venv .venv && source .venv/bin/activate
来源：http://kox.hnxiangtu.top

[U02] Py：导出 / 安装依赖
来源：http://uyg.nanxinkj.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://wss.yongpay.top

[U03] Py：加载 .env 配置
来源：http://ggr.bbcook.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://frr.zhiwuduotai.top

[U04] Py：变量调试打印
来源：http://ova.dianchejie.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://evd.gzhubu.top

[U05] Py：列表去重且保序
来源：http://ntj.kuanghao11.cn

list(dict.fromkeys(arr))
来源：http://uff.shzxlz.cn

[U06] Py：合并两个字典
来源：http://rse.nanxinkj.top

{**a, **b}
来源：http://zsi.tian-w.cn

[U07] Py：反转字典键值
来源：http://mjr.yj202588.top

{v: k for k, v in d.items()}
来源：http://dgx.wangdashe.top

[U08] Py：展平二维列表
来源：http://rzw.ivvv.top

[y for x in nested for y in x]
来源：http://xqu.shanyushiyangtech.top

[U09] Py：字典取最大值的键
来源：http://rty.feifeiyinyue.top

max(d, key=d.get)
来源：http://dli.bbcook.cn

[U10] Py：按值排序字典
来源：http://zqz.epnwcf.com

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://fij.52xcode.cn

[U11] Py：生成器表达式
来源：http://qvl.c1oappe.top

(x * 2 for x in arr)
来源：http://lwj.daria6918.cn

[U12] Py：取出现最多的 3 个元素
来源：http://zqh.haohaochexian.top

Counter(arr).most_common(3)
来源：http://yna.iojbl.cn

[U13] Py：固定长度队列
来源：http://jee.daria6918.cn

deque(maxlen=10)
来源：http://iai.jianghu66.top

[U14] Py：分组收集到列表
来源：http://kgj.zdqjudy.top

defaultdict(list)
来源：http://jmb.xinyue.icu

[U15] Py：高精度计时
来源：http://yaz.cheryme.top

t = time.perf_counter()
来源：http://duf.jqgufenzy.top

[U16] Py：命令行参数解析
来源：http://thz.jinghuilouyu.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://nvf.nwbrower.top

[U17] Py：初始化日志
来源：http://ava.epnwcf.com

logging.basicConfig(level=logging.INFO)
来源：http://usl.cheryme.top

[U18] Py：预编译正则
来源：http://ond.xuanzx.com

pat = re.compile(r"\d+")
来源：http://pyy.zhiwuduotai.top

[U19] Py：正则替换带回调
来源：http://aye.daria6918.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://iob.ydzc1.top

[U20] Py：缓存函数结果
来源：http://riw.zdqjudy.top

@functools.lru_cache(maxsize=None)
来源：http://iqm.fktsv.cn

[U21] Py：自定义上下文管理器
来源：http://mhn.ehwqpu.com

@contextlib.contextmanager
来源：http://ien.wangshuangyany.cn

[U22] Py：矩阵转置
来源：http://khc.snrcjt.cn

list(zip(*m))
来源：http://bkk.yj20258888.top

[U23] Py：分块读取大文件
来源：http://fhb.yongpay.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://vdz.cashguo.top

[U24] Py：路径操作
来源：http://kqj.iojbl.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://una.svipenyu.cn

[U25] Py：CSV 按字典读
来源：http://chp.xinyue.icu

csv.DictReader(f)
来源：http://xbz.ctjpmb.com

[U26] Py：并发下载
来源：http://hky.epnwcf.com

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://pcb.quarkkingdee.top

[U27] Py：异步 HTTP
来源：http://tmc.snrcjt.cn

aiohttp.ClientSession() 配合 async with
来源：http://uwv.yangfankeji.com

[U28] Py：类型别名
来源：http://wnp.meibo888.top

UserId = int
来源：http://aes.svipenyu.cn

[U29] Py：属性校验
来源：http://oqn.jlsjyb.cn

@property 与 @x.setter 配合
来源：http://wgw.tian-w.cn

[U30] Py：数据类
来源：http://psy.redwolf501.top

@dataclass(slots=True)
来源：http://oqo.316326.xyz

[U31] Py：单测
来源：http://vff.cdnleiting.top

python -m pytest -q
来源：http://fpe.jyoumei.cn

[U32] Py：代码格式化
来源：http://gyq.hysaishi.cn

ruff format . && ruff check --fix .
来源：http://ahv.nwbrower.top

[U33] Py：打包发布
来源：http://nvm.jinqigfzy.top

python -m build  （依赖 pyproject.toml）
来源：http://bne.gaohongyu789.top

[U34] Py：判断编码
来源：http://wsd.zycfv.cn

chardet.detect(raw)
来源：http://cga.smart0.xyz

[U35] Py：发送邮件
来源：http://xow.xziqi.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://gbc.zhoulong.xyz

[U36] Py：定时任务
来源：http://anw.jinqigufen.top

schedule.every(10).minutes.do(job)
来源：http://aow.ctjpmb.com

[U37] Py：读写 Excel
来源：http://ewn.ivvv.top

pandas.read_excel / DataFrame.to_excel
来源：http://pkl.pycfn.com

[U38] Py：获取脚本所在目录
来源：http://bdw.jinyuanbaomall.cn

Path(__file__).resolve().parent
来源：http://mvt.hysaishi.cn

[U39] Py：判断是否在交互环境
来源：http://tlv.jianghu66.top

sys.stdout.isatty()
来源：http://dgu.ppjwa.cn

[U40] Py：打印到标准错误
来源：http://uij.tanke756.top

print("err", file=sys.stderr)
来源：http://kta.ywan-chungtsiang.top

[U41] PHP：初始化 Composer 项目
来源：http://uzw.xziqi.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://oke.9152youxi.cn

[U42] PHP：PSR-4 自动加载
来源：http://ixl.yueranfly.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://eru.redwolf501.top

[U43] PHP：声明命名空间
来源：http://puv.ppjwa.cn

namespace App\Http;
来源：http://nhv.sjlbkw.cn

[U44] PHP：开启严格类型
来源：http://nyc.sweek.top

declare(strict_types=1);
来源：http://wat.ydzc1.top

[U45] PHP：类型声明与返回类型
来源：http://zpg.zhaomingkeji.xyz

function add(int $a, int $b): int { return $a + $b; }
来源：http://iju.daxiang520.top

[U46] PHP：可空类型
来源：http://rpo.daria6918.cn

?string $name = null
来源：http://gdk.shuidangran.top

[U47] PHP：联合类型
来源：http://etv.xingfuxueyuan.xyz

int|string $id
来源：http://rbf.zhoulong.xyz

[U48] PHP：纯枚举
来源：http://drn.dianchejie.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hwt.yongpay.top

[U49] PHP：只读属性
来源：http://tkw.gaohongyu789.top

public readonly string $name
来源：http://mjc.shzxlz.cn

[U50] PHP：构造器属性提升
来源：http://rny.yj20258888.top

public function __construct(private int $id) {}
来源：http://yxw.jqgufenzy.top

[U51] PHP：数组解构
来源：http://sgd.fengsongda.top

[$a, $b] = $arr;
来源：http://err.ybcxt.top

[U52] PHP：箭头函数
来源：http://way.gaohongyu789.top

$double = fn($x) => $x * 2;
来源：http://tre.yangfankeji.com

[U53] PHP：空合并运算符
来源：http://sqb.redwolf501.top

$v = $a ?? $b ?? "default";
来源：http://cof.hnqzz.top

[U54] PHP：空安全调用
来源：http://rfp.yvedp.cn

$obj?->method()
来源：http://khc.haohaochexian.top

[U55] PHP：match 表达式
来源：http://bpw.hongshengwenyu.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://ffu.ydzc1.top

[U56] PHP：命名参数
来源：http://mox.jinqigfzy.top

f(a: 1, b: 2)
来源：http://urq.yonumen.top

[U57] PHP：字符串插值
来源：http://czc.jiagoushi.top

"值: {$a}"
来源：http://tkv.tanke756.top

[U58] PHP：数组三件套
来源：http://lrh.gotoacloud.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://rdp.shanyushiyangtech.top

[U59] PHP：自定义排序
来源：http://axl.guannengcc.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://srh.zhijiandao.cn

[U60] PHP：JSON 编解码
来源：http://qnt.yongpay.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://njc.shuidangran.top

[U61] PHP：正则
来源：http://cpp.ywan-chungtsiang.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://pka.jinqigfzy.top

[U62] PHP：日期对象
来源：http://qkj.yuanzhike.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hem.hnxiangtu.top

[U63] PHP：文件读写
来源：http://drb.tarul.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://tms.c1oappe.top

[U64] PHP：目录遍历
来源：http://rfz.yj20258888.top

glob("dir/*.php");  scandir("dir");
来源：http://dji.hfpthk.cn

[U65] PHP：会话
来源：http://njm.gzhubu.top

session_start();  $_SESSION["uid"] = 1;
来源：http://xnj.redwolf501.top

[U66] PHP：设置 Cookie
来源：http://iym.xinyue.icu

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://gem.xingfuxueyuan.xyz

[U67] PHP：处理文件上传
来源：http://jhb.xylfe.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://juh.0kj1m.cn

[U68] PHP：PDO 连接
来源：http://nxk.hywenlv.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://fju.zhixingplan.top

[U69] PHP：PDO 预处理
来源：http://stj.zhengqikj.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://zuq.xuetiantiany.cn

[U70] PHP：PDO 事务
来源：http://xwx.sjlbkw.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://nvf.nwbrower.top

[U71] PHP：抛出异常
来源：http://snj.ppjwa.cn

throw new RuntimeException("失败", 500);
来源：http://lga.zhongyouzk.top

[U72] PHP：写错误日志
来源：http://eht.guowangkeji.top

error_log("失败: " . $e->getMessage());
来源：http://ytk.nanxinkj.top

[U73] PHP：读取 ini 配置
来源：http://tut.xziqi.cn

parse_ini_file("config.ini", true)
来源：http://zdl.zdbjq.cn

[U74] PHP：读取环境变量
来源：http://mgu.feifeiyinyue.top

getenv("APP_ENV") ?: "production"
来源：http://krb.cqqwz.cn

[U75] PHP：依赖注入
来源：http://col.hesvh.cn

composer require psr/container
来源：http://uch.wangdashe.top

[U76] PHP：简单路由
来源：http://wsa.smart0.xyz

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://mwf.fehbvm.com

[U77] PHP：模板渲染
来源：http://sfz.gogol.net.cn

composer require twig/twig
来源：http://cpx.feifeiyinyue.top

[U78] PHP：单元测试
来源：http://wxl.cashguo.top

composer require --dev phpunit/phpunit
来源：http://vuq.jqgufenzy.top

[U79] PHP：静态分析
来源：http://xez.yj20258888.top

composer require --dev phpstan/phpstan
来源：http://aso.xuetiantiany.cn

[U80] PHP：代码规范修复
来源：http://kjl.jiagoushi.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://sdh.bjfxy.top

[U81] JS：初始化项目
来源：http://vqt.shanyushiyangkeji.top

npm init -y;  npm i express
来源：http://cwk.bbcook.cn

[U82] JS：package.json 脚本
来源：http://zoz.nanxinkj.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://xcj.ydjk.org.cn

[U83] JS：ES Module 导入导出
来源：http://mab.zhijiandao.cn

export const a = 1;  import { a } from "./m.js";
来源：http://qgb.yanxiufei.cn

[U84] JS：CommonJS 写法
来源：http://cdc.daxiang520.top

module.exports = { a };  const { a } = require("./m");
来源：http://xir.ywan-chungtsiang.top

[U85] JS：可选链
来源：http://xsc.sxryk.cn

a?.b?.c
来源：http://kuk.gzhubu.top

[U86] JS：空值合并
来源：http://pwc.ppjwa.cn

a ?? b
来源：http://ona.cucudq.cn

[U87] JS：解构默认值
来源：http://mml.c1oappe.top

const { a = 1, b = 2 } = obj;
来源：http://aae.shanyushiyangkeji.top

[U88] JS：对象展开合并
来源：http://mtn.epnwcf.com

{ ...a, ...b }
来源：http://xsj.wangshuangyany.cn

[U89] JS：数组去重
来源：http://xri.daria6918.cn

[...new Set(arr)]
来源：http://fgm.zhengqikj.top

[U90] JS：数字数组排序
来源：http://uoq.sufxvd.cn

[...arr].sort((a, b) => a - b)
来源：http://fjf.zhengqikj.top

[U91] JS：对象键值遍历
来源：http://dpm.yfazqb.com

Object.entries(obj).forEach(([k, v]) => {});
来源：http://njs.gogol.net.cn

[U92] JS：深拷贝
来源：http://jrg.yonumen.top

structuredClone(obj)
来源：http://xme.ppjwa.cn

[U93] JS：模板字符串
来源：http://fxw.guannengcc.top

`共 ${n} 条`
来源：http://idn.daria6918.cn

[U94] JS：箭头函数
来源：http://efj.uphjek.com

const double = x => x * 2;
来源：http://ibs.gotoacloud.top

[U95] JS：Promise 包装
来源：http://cfm.ybcxt.top

new Promise((resolve, reject) => {})
来源：http://lga.cucudq.cn

[U96] JS：async/await 与异常
来源：http://luz.wangshuangyany.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://rul.yj20258888.top

[U97] JS：并发请求
来源：http://lma.chenzaomai.com

await Promise.all(urls.map(u => fetch(u)))
来源：http://pkk.fengsongda.top

[U98] JS：fetch 带 JSON
来源：http://pxj.feifeiyinyue.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://crc.feifeiyinyue.top

[U99] JS：事件监听
来源：http://svc.sjlbkw.cn

el.addEventListener("click", e => {})
来源：http://rpi.yuanzhike.top

[U100] JS：DOM 查询
来源：http://glm.yj20258888.top

document.querySelector(".item")
来源：http://lun.jianghu66.top

[U101] JS：classList 操作
来源：http://eul.xylfe.cn

el.classList.toggle("active")
来源：http://mbs.fzhhl.top

[U102] JS：本地存储
来源：http://zro.bjfxy.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://mlz.zhixingplan.top

[U103] JS：定时器
来源：http://yae.fehbvm.com

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://tlb.guannengcc.top

[U104] JS：防抖
来源：http://vna.xuetiantiany.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ebv.nanxinkj.top

[U105] JS：节流
来源：http://agd.chenjidiqi.icu

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://xfg.yj20258888.top

[U106] JS：日期格式化
来源：http://mhf.iojbl.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://vfs.zdqjudy.top

[U107] JS：数字千分位
来源：http://rrb.shzxlz.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://zgz.shanyushiyangtech.top

[U108] JS：随机整数
来源：http://iob.hongshengwenyu.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://xnr.kuanghao11.cn

[U109] JS：数组分组
来源：http://gbu.gzhubu.top

Object.groupBy(arr, x => x.type)
来源：http://odg.yj20258888.top

[U110] JS：数组分块
来源：http://qgn.xuanzx.com

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://ojt.wangdashe.top

[U111] JS：对象转 Map
来源：http://jxh.jinqigfzy.top

new Map(Object.entries(obj))
来源：http://iem.vqdsnc.cn

[U112] JS：字符串补位
来源：http://xkj.andypj.xyz

"7".padStart(3, "0")
来源：http://tsg.vqdsnc.cn

[U113] JS：正则替换全部
来源：http://jwl.epnwcf.com

s.replaceAll("a", "b")
来源：http://gyg.xuanzx.com

[U114] JS：JSON 深比较
来源：http://mof.sxryk.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://les.yonumen.top

[U115] JS：生成 UUID
来源：http://rya.zhijiandao.cn

crypto.randomUUID()
来源：http://frr.wangshuangyany.cn

[U116] JS：类型检查（JSDoc）
来源：http://zgm.tian-w.cn

/** @param {string} name */ function f(name) {}
来源：http://pqy.haohaochexian.top

[U117] JS：单元测试
来源：http://vpm.sweek.top

npm i -D vitest;  npx vitest
来源：http://ppe.jinqigufen.top

[U118] JS：开发服务器
来源：http://xyt.hnxiangtu.top

npm i -D vite;  npx vite
来源：http://mvs.jiagoushi.top

[U119] JS：生产构建
来源：http://agc.tarul.cn

npx vite build
来源：http://jby.zhengqikj.top

[U120] JS：读取环境变量（Vite）
来源：http://kcc.jiagoushi.top

import.meta.env.VITE_API_URL
来源：http://lao.aizwys.cn

================================================================================
来源：http://rxm.ppjwa.cn

统计汇总
来源：http://nxt.xylfe.cn

================================================================================
来源：http://wrj.feifeiyinyue.top

按语言统计（条）：
来源：http://rxh.redwolf501.top

Python ......... 252
来源：http://jvn.smart0.xyz

PHP ............ 252
来源：http://zlf.nanxinkj.top

JavaScript ..... 252
来源：http://brf.jlsjyb.cn

TypeScript ..... 212
来源：http://ows.birdmap.top

Java ........... 212
来源：http://ukm.ywan-chungtsiang.top

Go ............. 212
来源：http://zwd.xziqi.cn

Ruby ........... 212
来源：http://apr.bjfxy.top

C# ............. 212
来源：http://ejf.cheryme.top

C .............. 30
来源：http://amj.9152youxi.cn

C++ ............ 30
来源：http://gsq.andypj.xyz

SQL ............ 90
来源：http://epg.cheryme.top

Bash ........... 80
来源：http://yoe.zhijiandao.cn

Kotlin ......... 15
来源：http://xan.redwolf501.top

Swift .......... 15
来源：http://oti.svipenyu.cn

Lua ............ 10
来源：http://sqv.52xcode.cn

Perl ........... 10
来源：http://oho.shanyushiyangtech.top

Scala .......... 10
来源：http://zkt.xinyue.icu

------------------------------------
来源：http://lic.zycfv.cn

合计 ........... 2106 条
来源：http://dvx.hesvh.cn

按章节统计：
来源：http://mpb.jinqigfzy.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://eml.shuidangran.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://cso.cqqwz.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://dnk.fehbvm.com

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://ldr.wangdashe.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://wtk.jinqigufen.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://lgk.hywenlv.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://eyo.ehwqpu.com

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://khe.jlsjyb.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://yfy.tian-w.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://tur.guannengcc.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://eui.yangfankeji.com

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://dow.daxiang520.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://jkb.mhx1999.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://tyc.yvedp.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://wvm.9152youxi.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://eql.meibo888.top

Q SQL 专题                              90
来源：http://eky.vehdjk.com

R Bash 专题                             80
来源：http://swh.xingfuxueyuan.xyz

S C / C++ 专题                          60
来源：http://eew.hcnkem.com

T 其他语言补充                          60
来源：http://uhg.wangshuangyany.cn

U 高频实用片段                         120
来源：http://pfh.wangdashe.top

------------------------------------
来源：http://fcz.aibaodan.cn

合计                                  2106 条
来源：http://gpi.nwbrower.top

--------------------------------------------------------------------------------
来源：http://gzc.yj202588.top

使用提醒
来源：http://yqc.andypj.xyz

--------------------------------------------------------------------------------
来源：http://pzo.cashguo.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://ktq.zhengqikj.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://ulu.shanyushiyangkeji.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://eka.aibaodan.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://ftr.epnwcf.com

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://lkx.zhiwuduotai.top

—— 文件结束 ——
来源：http://doq.fengsongda.top


<!-- 参考信息 -->