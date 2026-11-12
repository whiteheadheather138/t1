代发 wailian999

[U05] Py：列表去重且保序
来源：http://exh.mhx1999.top

list(dict.fromkeys(arr))
来源：http://wtr.tianlin.xyz

[U06] Py：合并两个字典
来源：http://byg.ctjpmb.com

{**a, **b}
来源：http://jjv.fanxiaobao.xyz

[U07] Py：反转字典键值
来源：http://chx.zdbjq.cn

{v: k for k, v in d.items()}
来源：http://bnc.chenjidiqi.icu

[U08] Py：展平二维列表
来源：http://xaa.meibo888.top

[y for x in nested for y in x]
来源：http://vvy.xuetiantiany.cn

[U09] Py：字典取最大值的键
来源：http://vkq.yuanzhike.top

max(d, key=d.get)
来源：http://cbo.zhongyouzk.top

[U10] Py：按值排序字典
来源：http://hbn.fzhhl.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://fbg.ppjwa.cn

[U11] Py：生成器表达式
来源：http://fvp.wangshuangyany.cn

(x * 2 for x in arr)
来源：http://grj.hongshengwenyu.top

[U12] Py：取出现最多的 3 个元素
来源：http://ueo.redwolf501.top

Counter(arr).most_common(3)
来源：http://fed.yangfankeji.com

[U13] Py：固定长度队列
来源：http://vkb.cashguo.top

deque(maxlen=10)
来源：http://gxw.dianchejie.cn

[U14] Py：分组收集到列表
来源：http://gea.tianlin.xyz

defaultdict(list)
来源：http://eth.guowangkeji.top

[U15] Py：高精度计时
来源：http://cup.zhaomingkeji.xyz

t = time.perf_counter()
来源：http://obj.bjfxy.top

[U16] Py：命令行参数解析
来源：http://hzz.zhengqikj.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://byd.sweek.top

[U17] Py：初始化日志
来源：http://fgb.jyoumei.cn

logging.basicConfig(level=logging.INFO)
来源：http://hjt.zdbjq.cn

[U18] Py：预编译正则
来源：http://vqq.shanyushiyangkeji.top

pat = re.compile(r"\d+")
来源：http://bir.zdqjudy.top

[U19] Py：正则替换带回调
来源：http://cgg.cheryme.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://rkc.fzhhl.top

[U20] Py：缓存函数结果
来源：http://mwd.jinyuanbaomall.cn

@functools.lru_cache(maxsize=None)
来源：http://lvv.smart0.xyz

[U21] Py：自定义上下文管理器
来源：http://bhb.ivvv.top

@contextlib.contextmanager
来源：http://hva.vehdjk.com

[U22] Py：矩阵转置
来源：http://pyr.ppjwa.cn

list(zip(*m))
来源：http://jlb.xuetiantiany.cn

[U23] Py：分块读取大文件
来源：http://ejt.tarul.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://vki.hnqzz.top

[U24] Py：路径操作
来源：http://ljv.hongshengwenyu.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://vnt.tian-w.cn

[U25] Py：CSV 按字典读
来源：http://yty.52xcode.cn

csv.DictReader(f)
来源：http://rut.andypj.xyz

[U26] Py：并发下载
来源：http://waz.cucudq.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://fmh.bjfxy.top

[U27] Py：异步 HTTP
来源：http://yzn.shanyushiyangkeji.top

aiohttp.ClientSession() 配合 async with
来源：http://uiw.yonumen.top

[U28] Py：类型别名
来源：http://ekp.svipenyu.cn

UserId = int
来源：http://jqt.chenzaomai.com

[U29] Py：属性校验
来源：http://kpc.52xcode.cn

@property 与 @x.setter 配合
来源：http://igo.hywenlv.cn

[U30] Py：数据类
来源：http://wav.kuanghao11.cn

@dataclass(slots=True)
来源：http://ncg.yueranfly.top

[U31] Py：单测
来源：http://bhl.snrcjt.cn

python -m pytest -q
来源：http://pwp.redwolf501.top

[U32] Py：代码格式化
来源：http://rxt.jinqigfzy.top

ruff format . && ruff check --fix .
来源：http://bax.xziqi.cn

[U33] Py：打包发布
来源：http://tyk.zhijiandao.cn

python -m build  （依赖 pyproject.toml）
来源：http://znv.xuetiantiany.cn

[U34] Py：判断编码
来源：http://qas.chenlongwang.top

chardet.detect(raw)
来源：http://oid.chenzaomai.com

[U35] Py：发送邮件
来源：http://qph.hesvh.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hvq.0kj1m.cn

[U36] Py：定时任务
来源：http://wws.yvedp.cn

schedule.every(10).minutes.do(job)
来源：http://yjk.jqgufenzy.top

[U37] Py：读写 Excel
来源：http://llr.redwolf501.top

pandas.read_excel / DataFrame.to_excel
来源：http://jix.epnwcf.com

[U38] Py：获取脚本所在目录
来源：http://yzj.hysaishi.cn

Path(__file__).resolve().parent
来源：http://zyg.tian-w.cn

[U39] Py：判断是否在交互环境
来源：http://zlp.ehwqpu.com

sys.stdout.isatty()
来源：http://cir.zhiwuduotai.top

[U40] Py：打印到标准错误
来源：http://oxs.hysaishi.cn

print("err", file=sys.stderr)
来源：http://wpj.hammf.cn

[U41] PHP：初始化 Composer 项目
来源：http://kvz.xuetiantiany.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://peq.pengpengdd.cyou

[U42] PHP：PSR-4 自动加载
来源：http://ojf.aibaodan.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://euo.ybcxt.top

[U43] PHP：声明命名空间
来源：http://owq.xziqi.cn

namespace App\Http;
来源：http://pgl.zdqjudy.top

[U44] PHP：开启严格类型
来源：http://qbt.xuetiantiany.cn

declare(strict_types=1);
来源：http://pml.zhaomingkeji.xyz

[U45] PHP：类型声明与返回类型
来源：http://hyi.zdbjq.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://xlb.shzxlz.cn

[U46] PHP：可空类型
来源：http://wnw.fengsongda.top

?string $name = null
来源：http://ubk.yj202588.top

[U47] PHP：联合类型
来源：http://jbr.fanxiaobao.xyz

int|string $id
来源：http://huu.shangyingyoupin.top

[U48] PHP：纯枚举
来源：http://gel.tian-w.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hrl.xinyue.icu

[U49] PHP：只读属性
来源：http://kdw.chenjidiqi.icu

public readonly string $name
来源：http://amg.havefunace.top

[U50] PHP：构造器属性提升
来源：http://yrc.havefunace.top

public function __construct(private int $id) {}
来源：http://zpw.52xcode.cn

[U51] PHP：数组解构
来源：http://cyt.nanxinkj.top

[$a, $b] = $arr;
来源：http://sbu.sweek.top

[U52] PHP：箭头函数
来源：http://gna.sweek.top

$double = fn($x) => $x * 2;
来源：http://pnq.wangdashe.top

[U53] PHP：空合并运算符
来源：http://oqz.yfazqb.com

$v = $a ?? $b ?? "default";
来源：http://kqx.gaohongyu789.top

[U54] PHP：空安全调用
来源：http://zhi.fanxiaobao.xyz

$obj?->method()
来源：http://qmu.hfpthk.cn

[U55] PHP：match 表达式
来源：http://ngr.jinqigufen.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://eiz.xylfe.cn

[U56] PHP：命名参数
来源：http://vbv.ybcxt.top

f(a: 1, b: 2)
来源：http://gwo.fehbvm.com

[U57] PHP：字符串插值
来源：http://qdu.chenlongwang.top

"值: {$a}"
来源：http://ozu.9152youxi.cn

[U58] PHP：数组三件套
来源：http://wmo.zdbjq.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://kse.jianghu66.top

[U59] PHP：自定义排序
来源：http://qos.yj20258888.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://dlp.nanxinkj.top

[U60] PHP：JSON 编解码
来源：http://fve.fehbvm.com

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://vri.cheryme.top

[U61] PHP：正则
来源：http://bnr.epnwcf.com

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://ovw.52xcode.cn

[U62] PHP：日期对象
来源：http://nrn.ybcxt.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://noj.ehwqpu.com

[U63] PHP：文件读写
来源：http://jem.yangfankeji.com

file_get_contents($f);  file_put_contents($f, $data);
来源：http://phb.daria6918.cn

[U64] PHP：目录遍历
来源：http://wwi.dashuyun.cn

glob("dir/*.php");  scandir("dir");
来源：http://yum.jyoumei.cn

[U65] PHP：会话
来源：http://clp.zhongyouzk.top

session_start();  $_SESSION["uid"] = 1;
来源：http://vjf.mhx1999.top

[U66] PHP：设置 Cookie
来源：http://vwa.feifeiyinyue.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://cek.yanxiufei.cn

[U67] PHP：处理文件上传
来源：http://ech.cqqwz.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://wjk.fanxiaobao.xyz

[U68] PHP：PDO 连接
来源：http://hrf.yongpay.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://pbc.chenjidiqi.icu

[U69] PHP：PDO 预处理
来源：http://tcx.0kj1m.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://yex.iojbl.cn

[U70] PHP：PDO 事务
来源：http://zxg.shuidangran.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://pgb.fanxiaobao.xyz

[U71] PHP：抛出异常
来源：http://npi.sufxvd.cn

throw new RuntimeException("失败", 500);
来源：http://bvj.xuetiantiany.cn

[U72] PHP：写错误日志
来源：http://jug.iojbl.cn

error_log("失败: " . $e->getMessage());
来源：http://wnh.meibo888.top

[U73] PHP：读取 ini 配置
来源：http://xmd.shanyushiyangkeji.top

parse_ini_file("config.ini", true)
来源：http://sdx.fehbvm.com

[U74] PHP：读取环境变量
来源：http://ess.tianlin.xyz

getenv("APP_ENV") ?: "production"
来源：http://oyw.nanxinkj.top

[U75] PHP：依赖注入
来源：http://qpm.aibaodan.cn

composer require psr/container
来源：http://dlh.yj20258.top

[U76] PHP：简单路由
来源：http://tre.zhoulong.xyz

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://beo.gotoacloud.top

[U77] PHP：模板渲染
来源：http://xle.jlsjyb.cn

composer require twig/twig
来源：http://baf.iojbl.cn

[U78] PHP：单元测试
来源：http://qsk.dashuyun.cn

composer require --dev phpunit/phpunit
来源：http://spa.jqgufenzy.top

[U79] PHP：静态分析
来源：http://sqt.yueranfly.top

composer require --dev phpstan/phpstan
来源：http://wme.xylfe.cn

[U80] PHP：代码规范修复
来源：http://pxr.xuanzx.com

composer require --dev friendsofphp/php-cs-fixer
来源：http://ute.yongpay.top

[U81] JS：初始化项目
来源：http://llr.yangfankeji.com

npm init -y;  npm i express
来源：http://foo.zhaomingkeji.xyz

[U82] JS：package.json 脚本
来源：http://gaf.ydjk.org.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://qgc.shzxlz.cn

[U83] JS：ES Module 导入导出
来源：http://vjv.ywan-chungtsiang.top

export const a = 1;  import { a } from "./m.js";
来源：http://uwf.tian-w.cn

[U84] JS：CommonJS 写法
来源：http://xlm.hywenlv.cn

module.exports = { a };  const { a } = require("./m");
来源：http://lqn.cashguo.top

[U85] JS：可选链
来源：http://mvz.ctjpmb.com

a?.b?.c
来源：http://esr.zhiwuduotai.top

[U86] JS：空值合并
来源：http://npm.shangyingyoupin.top

a ?? b
来源：http://nkq.jinqigufen.top

[U87] JS：解构默认值
来源：http://age.yonumen.top

const { a = 1, b = 2 } = obj;
来源：http://dyj.fktsv.cn

[U88] JS：对象展开合并
来源：http://amq.xuanzx.com

{ ...a, ...b }
来源：http://lab.shuidangran.top

[U89] JS：数组去重
来源：http://yqx.sjlbkw.cn

[...new Set(arr)]
来源：http://uls.sufxvd.cn

[U90] JS：数字数组排序
来源：http://omq.jianghu66.top

[...arr].sort((a, b) => a - b)
来源：http://pdb.ydzc1.top

[U91] JS：对象键值遍历
来源：http://kld.sysykeji.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hfp.guowangkeji.top

[U92] JS：深拷贝
来源：http://ozq.yonumen.top

structuredClone(obj)
来源：http://mjm.tianlin.xyz

[U93] JS：模板字符串
来源：http://zyw.zhoulong.xyz

`共 ${n} 条`
来源：http://svs.hfpthk.cn

[U94] JS：箭头函数
来源：http://opd.yuanzhike.top

const double = x => x * 2;
来源：http://tor.pycfn.com

[U95] JS：Promise 包装
来源：http://vht.cheryme.top

new Promise((resolve, reject) => {})
来源：http://tmq.wangdashe.top

[U96] JS：async/await 与异常
来源：http://xum.hfpthk.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://wvu.pengpengdd.cyou

[U97] JS：并发请求
来源：http://jkr.ctjpmb.com

await Promise.all(urls.map(u => fetch(u)))
来源：http://xci.quarkkingdee.top

[U98] JS：fetch 带 JSON
来源：http://erz.hesvh.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://oxf.tarul.cn

[U99] JS：事件监听
来源：http://mjj.yonumen.top

el.addEventListener("click", e => {})
来源：http://mhb.xylfe.cn

[U100] JS：DOM 查询
来源：http://nwk.yj202588.top

document.querySelector(".item")
来源：http://sxm.meibo888.top

[U101] JS：classList 操作
来源：http://xil.xinyue.icu

el.classList.toggle("active")
来源：http://ycg.quarkkingdee.top

[U102] JS：本地存储
来源：http://jel.cashguo.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://lhr.dianchejie.cn

[U103] JS：定时器
来源：http://ujc.ydzc1.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://xxf.hammf.cn

[U104] JS：防抖
来源：http://glw.fzhhl.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://pyf.9152youxi.cn

[U105] JS：节流
来源：http://bfd.ctjpmb.com

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://rwv.zhongyouzk.top

[U106] JS：日期格式化
来源：http://heu.316326.xyz

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://xut.gzhubu.top

[U107] JS：数字千分位
来源：http://svi.pycfn.com

new Intl.NumberFormat("en-US").format(1234567)
来源：http://axn.mhx1999.top

[U108] JS：随机整数
来源：http://ywt.aizwys.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://vri.hammf.cn

[U109] JS：数组分组
来源：http://rph.zhengqikj.top

Object.groupBy(arr, x => x.type)
来源：http://zfy.zhengqikj.top

[U110] JS：数组分块
来源：http://lgp.dianchejie.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://lpl.shanyushiyangtech.top

[U111] JS：对象转 Map
来源：http://bdf.sjlbkw.cn

new Map(Object.entries(obj))
来源：http://mrl.redwolf501.top

[U112] JS：字符串补位
来源：http://zxb.jinqigfzy.top

"7".padStart(3, "0")
来源：http://oyf.tian-w.cn

[U113] JS：正则替换全部
来源：http://krd.yongpay.top

s.replaceAll("a", "b")
来源：http://flx.wangshuangyany.cn

[U114] JS：JSON 深比较
来源：http://lcj.jlsjyb.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://pop.yj20258.top

[U115] JS：生成 UUID
来源：http://wck.jlsjyb.cn

crypto.randomUUID()
来源：http://teo.vehdjk.com

[U116] JS：类型检查（JSDoc）
来源：http://gcm.gogol.net.cn

/** @param {string} name */ function f(name) {}
来源：http://idx.shuidangran.top

[U117] JS：单元测试
来源：http://pet.zhaomingkeji.xyz

npm i -D vitest;  npx vitest
来源：http://tvc.uphjek.com

[U118] JS：开发服务器
来源：http://uln.nanxinkj.top

npm i -D vite;  npx vite
来源：http://mtr.yj202588.top

[U119] JS：生产构建
来源：http://hnv.svipenyu.cn

npx vite build
来源：http://fwd.iojbl.cn

[U120] JS：读取环境变量（Vite）
来源：http://ipv.yuxming.cn

import.meta.env.VITE_API_URL
来源：http://bqm.birdmap.top

================================================================================
来源：http://nox.xuetiantiany.cn

统计汇总
来源：http://khk.ehwqpu.com

================================================================================
来源：http://xri.hesvh.cn

按语言统计（条）：
来源：http://eue.hywenlv.cn

Python ......... 252
来源：http://ltp.yfazqb.com

PHP ............ 252
来源：http://jzr.snrcjt.cn

JavaScript ..... 252
来源：http://map.zhiwuduotai.top

TypeScript ..... 212
来源：http://pos.xinyue.icu

Java ........... 212
来源：http://trk.wangshuangyany.cn

Go ............. 212
来源：http://dcd.guannengcc.top

Ruby ........... 212
来源：http://awk.sjlbkw.cn

C# ............. 212
来源：http://rhw.quarkkingdee.top

C .............. 30
来源：http://lby.zhoulong.xyz

C++ ............ 30
来源：http://nrn.smart0.xyz

SQL ............ 90
来源：http://fcy.tanke756.top

Bash ........... 80
来源：http://wlg.pycfn.com

Kotlin ......... 15
来源：http://xfl.chenlongwang.top

Swift .......... 15
来源：http://itd.vehdjk.com

Lua ............ 10
来源：http://awr.gogol.net.cn

Perl ........... 10
来源：http://nct.xinyue.icu

Scala .......... 10
来源：http://mtq.ydzc1.top

------------------------------------
来源：http://bdg.quarkkingdee.top

合计 ........... 2106 条
来源：http://ukd.hammf.cn

按章节统计：
来源：http://znk.tian-w.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://rrv.andypj.xyz

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://evq.sufxvd.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://zmg.xingfuxueyuan.xyz

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://wwe.nanxinkj.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://pqf.tianlin.xyz

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://dbr.uphjek.com

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://mjk.tianlin.xyz

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://ngc.havefunace.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://uvz.aibaodan.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://mug.nanxinkj.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://lsv.zycfv.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://qqk.sysykeji.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://hlq.guowangkeji.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://jlf.yongpay.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://yvn.316326.xyz

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://mzk.hnqzz.top

Q SQL 专题                              90
来源：http://bqy.sxryk.cn

R Bash 专题                             80
来源：http://ybj.hysaishi.cn

S C / C++ 专题                          60
来源：http://hig.xziqi.cn

T 其他语言补充                          60
来源：http://izq.epnwcf.com

U 高频实用片段                         120
来源：http://yqd.gogol.net.cn

------------------------------------
来源：http://nul.yj202588.top

合计                                  2106 条
来源：http://yop.yuxming.cn

--------------------------------------------------------------------------------
来源：http://ycr.fehbvm.com

使用提醒
来源：http://ikv.jinqigufen.top

--------------------------------------------------------------------------------
来源：http://otk.zhiwuduotai.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://acc.chenzaomai.com

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://siu.gotoacloud.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://fzs.hywenlv.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://gsr.ydzc1.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://kyg.fehbvm.com

—— 文件结束 ——
来源：http://dfs.sjlbkw.cn

================================================================================
来源：http://zhh.zhongyouzk.top

程序语言常见例子速查手册（2024 版）
来源：http://qzc.xinyue.icu

Common Programming Examples Cheat Book
来源：http://auc.tian-w.cn

================================================================================
来源：http://gyd.fengsongda.top

【收录内容】
来源：http://skq.316326.xyz

覆盖 12 种语言 / 语法与常见 API：
来源：http://mqq.hnqzz.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://yxd.xuetiantiany.cn

SQL · Bash · C · C++
来源：http://uls.guannengcc.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://gmm.hongshengwenyu.top

【使用说明】
来源：http://qbx.sxryk.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://cdy.wangshuangyany.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://uuv.hnxiangtu.top


<!-- 参考信息 -->