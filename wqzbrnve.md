代发 wailian999

[U07] Py：反转字典键值
来源：http://wzl.zycfv.cn

{v: k for k, v in d.items()}
来源：http://hyo.tianlin.xyz

[U08] Py：展平二维列表
来源：http://ztx.xuanzx.com

[y for x in nested for y in x]
来源：http://wgl.jinyuanbaomall.cn

[U09] Py：字典取最大值的键
来源：http://wdp.wangshuangyany.cn

max(d, key=d.get)
来源：http://nnm.hammf.cn

[U10] Py：按值排序字典
来源：http://nnu.hongshengwenyu.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://cyo.cdnleiting.top

[U11] Py：生成器表达式
来源：http://fww.shangyingyoupin.top

(x * 2 for x in arr)
来源：http://liy.jinqigufen.top

[U12] Py：取出现最多的 3 个元素
来源：http://dgi.ybcxt.top

Counter(arr).most_common(3)
来源：http://mww.pengpengdd.cyou

[U13] Py：固定长度队列
来源：http://vxk.yj20258.top

deque(maxlen=10)
来源：http://hno.daxiang520.top

[U14] Py：分组收集到列表
来源：http://mnr.bbcook.cn

defaultdict(list)
来源：http://avy.wangshuangyany.cn

[U15] Py：高精度计时
来源：http://tqa.gogol.net.cn

t = time.perf_counter()
来源：http://hxl.ydjk.org.cn

[U16] Py：命令行参数解析
来源：http://zky.zhoulong.xyz

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://anh.jinqigufen.top

[U17] Py：初始化日志
来源：http://wzt.meibo888.top

logging.basicConfig(level=logging.INFO)
来源：http://hbn.52xcode.cn

[U18] Py：预编译正则
来源：http://tdb.ctjpmb.com

pat = re.compile(r"\d+")
来源：http://qrr.yj20258888.top

[U19] Py：正则替换带回调
来源：http://bre.gogol.net.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://sea.yangfankeji.com

[U20] Py：缓存函数结果
来源：http://flq.daxiang520.top

@functools.lru_cache(maxsize=None)
来源：http://utd.xziqi.cn

[U21] Py：自定义上下文管理器
来源：http://hzm.guowangkeji.top

@contextlib.contextmanager
来源：http://gnd.fanxiaobao.xyz

[U22] Py：矩阵转置
来源：http://ugj.yuxming.cn

list(zip(*m))
来源：http://tca.jlsjyb.cn

[U23] Py：分块读取大文件
来源：http://rmk.hnqzz.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://xul.vqdsnc.cn

[U24] Py：路径操作
来源：http://qfv.jinqigufen.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://gpo.ydzc1.top

[U25] Py：CSV 按字典读
来源：http://dfg.snrcjt.cn

csv.DictReader(f)
来源：http://wfg.ydjk.org.cn

[U26] Py：并发下载
来源：http://bge.mhx1999.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://cvd.wangshuangyany.cn

[U27] Py：异步 HTTP
来源：http://uhj.shanyushiyangkeji.top

aiohttp.ClientSession() 配合 async with
来源：http://eoy.yangfankeji.com

[U28] Py：类型别名
来源：http://hit.snrcjt.cn

UserId = int
来源：http://qna.chenzaomai.com

[U29] Py：属性校验
来源：http://liq.xziqi.cn

@property 与 @x.setter 配合
来源：http://hqi.haohaochexian.top

[U30] Py：数据类
来源：http://vti.kuanghao11.cn

@dataclass(slots=True)
来源：http://zgl.52xcode.cn

[U31] Py：单测
来源：http://aoo.zdbjq.cn

python -m pytest -q
来源：http://bmb.vqdsnc.cn

[U32] Py：代码格式化
来源：http://ene.jqgfzy.top

ruff format . && ruff check --fix .
来源：http://brv.uphjek.com

[U33] Py：打包发布
来源：http://ivu.sufxvd.cn

python -m build  （依赖 pyproject.toml）
来源：http://yvx.hnxiangtu.top

[U34] Py：判断编码
来源：http://uah.ydzc1.top

chardet.detect(raw)
来源：http://zjx.tian-w.cn

[U35] Py：发送邮件
来源：http://anr.fktsv.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://wsz.snrcjt.cn

[U36] Py：定时任务
来源：http://zxn.ivvv.top

schedule.every(10).minutes.do(job)
来源：http://luv.ivvv.top

[U37] Py：读写 Excel
来源：http://iqj.ppjwa.cn

pandas.read_excel / DataFrame.to_excel
来源：http://apm.jqgufenzy.top

[U38] Py：获取脚本所在目录
来源：http://niy.tanke756.top

Path(__file__).resolve().parent
来源：http://oib.zdbjq.cn

[U39] Py：判断是否在交互环境
来源：http://tal.xylfe.cn

sys.stdout.isatty()
来源：http://xjk.daxiang520.top

[U40] Py：打印到标准错误
来源：http://hii.mhx1999.top

print("err", file=sys.stderr)
来源：http://iau.fzhhl.top

[U41] PHP：初始化 Composer 项目
来源：http://stj.xinyue.icu

composer init;  composer require guzzlehttp/guzzle
来源：http://skg.jqgufenzy.top

[U42] PHP：PSR-4 自动加载
来源：http://uog.smart0.xyz

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://lyd.jinqigfzy.top

[U43] PHP：声明命名空间
来源：http://obv.cheryme.top

namespace App\Http;
来源：http://nsu.cqqwz.cn

[U44] PHP：开启严格类型
来源：http://qox.redwolf501.top

declare(strict_types=1);
来源：http://pyk.haohaochexian.top

[U45] PHP：类型声明与返回类型
来源：http://iqr.ybcxt.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://qez.daxiang520.top

[U46] PHP：可空类型
来源：http://kbu.yangfankeji.com

?string $name = null
来源：http://jtj.ivvv.top

[U47] PHP：联合类型
来源：http://smq.sysykeji.top

int|string $id
来源：http://xmm.hysaishi.cn

[U48] PHP：纯枚举
来源：http://afu.shzxlz.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://gnt.zycfv.cn

[U49] PHP：只读属性
来源：http://rzs.hnxiangtu.top

public readonly string $name
来源：http://sxc.aizwys.cn

[U50] PHP：构造器属性提升
来源：http://fhk.yuanzhike.top

public function __construct(private int $id) {}
来源：http://lsg.aizwys.cn

[U51] PHP：数组解构
来源：http://jdt.cqqwz.cn

[$a, $b] = $arr;
来源：http://sor.hongshengwenyu.top

[U52] PHP：箭头函数
来源：http://sde.zhengqikj.top

$double = fn($x) => $x * 2;
来源：http://ivx.cashguo.top

[U53] PHP：空合并运算符
来源：http://pui.yangfankeji.com

$v = $a ?? $b ?? "default";
来源：http://ujh.gaohongyu789.top

[U54] PHP：空安全调用
来源：http://onf.yueranfly.top

$obj?->method()
来源：http://ujw.epnwcf.com

[U55] PHP：match 表达式
来源：http://akv.zycfv.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://ovd.vehdjk.com

[U56] PHP：命名参数
来源：http://frw.fehbvm.com

f(a: 1, b: 2)
来源：http://eiq.andypj.xyz

[U57] PHP：字符串插值
来源：http://qzc.zhengqikj.top

"值: {$a}"
来源：http://lkg.cdnleiting.top

[U58] PHP：数组三件套
来源：http://rum.dianchejie.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://dbc.hammf.cn

[U59] PHP：自定义排序
来源：http://qbx.jiagoushi.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://cft.yuxming.cn

[U60] PHP：JSON 编解码
来源：http://ano.chenzaomai.com

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://ryw.hnxiangtu.top

[U61] PHP：正则
来源：http://pij.yongpay.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://nfc.fktsv.cn

[U62] PHP：日期对象
来源：http://efl.fktsv.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://bbu.yj202588.top

[U63] PHP：文件读写
来源：http://byl.redwolf501.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://dxy.xingfuxueyuan.xyz

[U64] PHP：目录遍历
来源：http://rok.nwbrower.top

glob("dir/*.php");  scandir("dir");
来源：http://mvw.hcnkem.com

[U65] PHP：会话
来源：http://hln.hongshengwenyu.top

session_start();  $_SESSION["uid"] = 1;
来源：http://laa.ppjwa.cn

[U66] PHP：设置 Cookie
来源：http://hle.zhengqikj.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://gmz.xuetiantiany.cn

[U67] PHP：处理文件上传
来源：http://srq.gotoacloud.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://ost.fktsv.cn

[U68] PHP：PDO 连接
来源：http://fal.52xcode.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://mcr.gaohongyu789.top

[U69] PHP：PDO 预处理
来源：http://epr.fanxiaobao.xyz

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://pou.dashuyun.cn

[U70] PHP：PDO 事务
来源：http://cxv.zhiwuduotai.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://lkg.daxiang520.top

[U71] PHP：抛出异常
来源：http://ijr.cdnleiting.top

throw new RuntimeException("失败", 500);
来源：http://isv.hongshengwenyu.top

[U72] PHP：写错误日志
来源：http://mkd.bjfxy.top

error_log("失败: " . $e->getMessage());
来源：http://uor.hywenlv.cn

[U73] PHP：读取 ini 配置
来源：http://gfe.guannengcc.top

parse_ini_file("config.ini", true)
来源：http://iqy.wangshuangyany.cn

[U74] PHP：读取环境变量
来源：http://agb.mhx1999.top

getenv("APP_ENV") ?: "production"
来源：http://ugc.wangdashe.top

[U75] PHP：依赖注入
来源：http://vpj.gogol.net.cn

composer require psr/container
来源：http://fwh.meibo888.top

[U76] PHP：简单路由
来源：http://ffc.9152youxi.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://aph.dashuyun.cn

[U77] PHP：模板渲染
来源：http://lnp.guannengcc.top

composer require twig/twig
来源：http://opl.xingfuxueyuan.xyz

[U78] PHP：单元测试
来源：http://wzc.hcnkem.com

composer require --dev phpunit/phpunit
来源：http://mwo.zhiwuduotai.top

[U79] PHP：静态分析
来源：http://cwe.yj20258.top

composer require --dev phpstan/phpstan
来源：http://rry.yongpay.top

[U80] PHP：代码规范修复
来源：http://twq.chenjidiqi.icu

composer require --dev friendsofphp/php-cs-fixer
来源：http://hbs.ybcxt.top

[U81] JS：初始化项目
来源：http://eyj.smart0.xyz

npm init -y;  npm i express
来源：http://abh.shanyushiyangkeji.top

[U82] JS：package.json 脚本
来源：http://dde.fengsongda.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://qpk.yvedp.cn

[U83] JS：ES Module 导入导出
来源：http://tfv.gzhubu.top

export const a = 1;  import { a } from "./m.js";
来源：http://ffq.gotoacloud.top

[U84] JS：CommonJS 写法
来源：http://gli.zhiwuduotai.top

module.exports = { a };  const { a } = require("./m");
来源：http://xzn.yangfankeji.com

[U85] JS：可选链
来源：http://jaq.zhengqikj.top

a?.b?.c
来源：http://lin.jyoumei.cn

[U86] JS：空值合并
来源：http://gzi.yj202588.top

a ?? b
来源：http://lhq.andypj.xyz

[U87] JS：解构默认值
来源：http://myr.chenlongwang.top

const { a = 1, b = 2 } = obj;
来源：http://des.redwolf501.top

[U88] JS：对象展开合并
来源：http://tze.zhiwuduotai.top

{ ...a, ...b }
来源：http://wxd.fzhhl.top

[U89] JS：数组去重
来源：http://sam.iojbl.cn

[...new Set(arr)]
来源：http://oyi.jinqigfzy.top

[U90] JS：数字数组排序
来源：http://hxp.xylfe.cn

[...arr].sort((a, b) => a - b)
来源：http://wsd.cucudq.cn

[U91] JS：对象键值遍历
来源：http://hqa.cdnleiting.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://xnc.hysaishi.cn

[U92] JS：深拷贝
来源：http://hfq.ehwqpu.com

structuredClone(obj)
来源：http://mcd.guannengcc.top

[U93] JS：模板字符串
来源：http://aza.zhongyouzk.top

`共 ${n} 条`
来源：http://bil.bbcook.cn

[U94] JS：箭头函数
来源：http://frf.kuanghao11.cn

const double = x => x * 2;
来源：http://ocb.kuanghao11.cn

[U95] JS：Promise 包装
来源：http://mmu.svipenyu.cn

new Promise((resolve, reject) => {})
来源：http://ojh.daxiang520.top

[U96] JS：async/await 与异常
来源：http://luv.havefunace.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://odk.fengsongda.top

[U97] JS：并发请求
来源：http://zli.yuxming.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://mnw.shanyushiyangtech.top

[U98] JS：fetch 带 JSON
来源：http://bvn.bbcook.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://yrj.zhengqikj.top

[U99] JS：事件监听
来源：http://laf.tian-w.cn

el.addEventListener("click", e => {})
来源：http://ahd.uphjek.com

[U100] JS：DOM 查询
来源：http://bil.fktsv.cn

document.querySelector(".item")
来源：http://uvu.bbcook.cn

[U101] JS：classList 操作
来源：http://uwq.zhengqikj.top

el.classList.toggle("active")
来源：http://ebt.zhijiandao.cn

[U102] JS：本地存储
来源：http://lls.jqgfzy.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://mix.xingfuxueyuan.xyz

[U103] JS：定时器
来源：http://itw.chenlongwang.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hep.iojbl.cn

[U104] JS：防抖
来源：http://dvp.jinyuanbaomall.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ibh.hfpthk.cn

[U105] JS：节流
来源：http://pxb.316326.xyz

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hrd.bjfxy.top

[U106] JS：日期格式化
来源：http://jka.hcnkem.com

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://wux.sysykeji.top

[U107] JS：数字千分位
来源：http://jrb.zycfv.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://lxq.yonumen.top

[U108] JS：随机整数
来源：http://ecy.zhijiandao.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://qnn.gotoacloud.top

[U109] JS：数组分组
来源：http://eyx.wangshuangyany.cn

Object.groupBy(arr, x => x.type)
来源：http://igo.shangyingyoupin.top

[U110] JS：数组分块
来源：http://aeu.ctjpmb.com

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://bpu.yonumen.top

[U111] JS：对象转 Map
来源：http://bab.cheryme.top

new Map(Object.entries(obj))
来源：http://zqx.ydjk.org.cn

[U112] JS：字符串补位
来源：http://bnp.vqdsnc.cn

"7".padStart(3, "0")
来源：http://boc.zhoulong.xyz

[U113] JS：正则替换全部
来源：http://xah.yvedp.cn

s.replaceAll("a", "b")
来源：http://klx.hywenlv.cn

[U114] JS：JSON 深比较
来源：http://hmi.zdbjq.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://nfx.shzxlz.cn

[U115] JS：生成 UUID
来源：http://lss.tarul.cn

crypto.randomUUID()
来源：http://xpa.chenlongwang.top

[U116] JS：类型检查（JSDoc）
来源：http://pcf.0kj1m.cn

/** @param {string} name */ function f(name) {}
来源：http://xyx.zhaomingkeji.xyz

[U117] JS：单元测试
来源：http://qqc.feifeiyinyue.top

npm i -D vitest;  npx vitest
来源：http://cto.gaohongyu789.top

[U118] JS：开发服务器
来源：http://iok.nwbrower.top

npm i -D vite;  npx vite
来源：http://mda.zhiwuduotai.top

[U119] JS：生产构建
来源：http://uln.jiagoushi.top

npx vite build
来源：http://tub.epnwcf.com

[U120] JS：读取环境变量（Vite）
来源：http://fbg.redwolf501.top

import.meta.env.VITE_API_URL
来源：http://faz.jyoumei.cn

================================================================================
来源：http://eyf.sjlbkw.cn

统计汇总
来源：http://vrn.jinqigufen.top

================================================================================
来源：http://ghq.cqqwz.cn

按语言统计（条）：
来源：http://axj.iojbl.cn

Python ......... 252
来源：http://hfz.hongshengwenyu.top

PHP ............ 252
来源：http://gqy.yj20258888.top

JavaScript ..... 252
来源：http://krf.zhengqikj.top

TypeScript ..... 212
来源：http://qdy.chenzaomai.com

Java ........... 212
来源：http://uij.zhoulong.xyz

Go ............. 212
来源：http://tza.yj20258.top

Ruby ........... 212
来源：http://wlv.mhx1999.top

C# ............. 212
来源：http://cma.guowangkeji.top

C .............. 30
来源：http://jtc.jinghuilouyu.cn

C++ ............ 30
来源：http://kzm.shanyushiyangkeji.top

SQL ............ 90
来源：http://mek.vehdjk.com

Bash ........... 80
来源：http://yih.guannengcc.top

Kotlin ......... 15
来源：http://mns.jinyuanbaomall.cn

Swift .......... 15
来源：http://omu.ywan-chungtsiang.top

Lua ............ 10
来源：http://lpb.daxiang520.top

Perl ........... 10
来源：http://vef.pycfn.com

Scala .......... 10
来源：http://qln.zycfv.cn

------------------------------------
来源：http://fqu.gotoacloud.top

合计 ........... 2106 条
来源：http://muz.guowangkeji.top

按章节统计：
来源：http://xiw.ctjpmb.com

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://zvq.yueranfly.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://keo.xuanzx.com

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://uda.gotoacloud.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://nao.yanxiufei.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://xuq.yanxiufei.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://lcr.uphjek.com

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://bsn.ydzc1.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://sro.dianchejie.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://xth.cdnleiting.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://uui.yuanzhike.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://ald.9152youxi.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://jdu.shuidangran.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://pus.guannengcc.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://qor.wangdashe.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://emg.yongpay.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://wzl.shanyushiyangkeji.top

Q SQL 专题                              90
来源：http://awi.shzxlz.cn

R Bash 专题                             80
来源：http://grn.yuanzhike.top

S C / C++ 专题                          60
来源：http://enh.wangshuangyany.cn

T 其他语言补充                          60
来源：http://xpv.hnqzz.top

U 高频实用片段                         120
来源：http://wla.sjlbkw.cn

------------------------------------
来源：http://tso.ydjk.org.cn

合计                                  2106 条
来源：http://euh.zhijiandao.cn

--------------------------------------------------------------------------------
来源：http://owa.zhijiandao.cn

使用提醒
来源：http://oua.daria6918.cn

--------------------------------------------------------------------------------
来源：http://vfd.cqqwz.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://neb.havefunace.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://gqz.haohaochexian.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://ukm.ybcxt.top

在旧版本上使用前请先确认语法支持情况。
来源：http://tjz.hnxiangtu.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://gel.hesvh.cn

—— 文件结束 ——
来源：http://zun.chenjidiqi.icu

================================================================================
来源：http://xsv.zhixingplan.top

程序语言常见例子速查手册（2024 版）
来源：http://aae.cucudq.cn

Common Programming Examples Cheat Book
来源：http://yvv.jinqigufen.top

================================================================================
来源：http://aev.xingfuxueyuan.xyz

【收录内容】
来源：http://bnu.vqdsnc.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://dkt.tanke756.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://yzl.zdqjudy.top

SQL · Bash · C · C++
来源：http://tfu.kuanghao11.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://owa.fzhhl.top

【使用说明】
来源：http://vuf.mhx1999.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://koc.shangyingyoupin.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://pfw.shanyushiyangkeji.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://biu.hnxiangtu.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://fry.jinghuilouyu.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://cnn.hnqzz.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://dem.bjfxy.top


<!-- 参考信息 -->