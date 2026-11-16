代发 wailian999

[U05] Py：列表去重且保序
来源：http://qhw.zhijiandao.cn

list(dict.fromkeys(arr))
来源：http://qnj.vqdsnc.cn

[U06] Py：合并两个字典
来源：http://fpv.sxryk.cn

{**a, **b}
来源：http://tyo.dianchejie.cn

[U07] Py：反转字典键值
来源：http://wdt.fanxiaobao.xyz

{v: k for k, v in d.items()}
来源：http://eul.zhijiandao.cn

[U08] Py：展平二维列表
来源：http://vzs.ydjk.org.cn

[y for x in nested for y in x]
来源：http://jxw.pycfn.com

[U09] Py：字典取最大值的键
来源：http://omz.xziqi.cn

max(d, key=d.get)
来源：http://qrl.xingfuxueyuan.xyz

[U10] Py：按值排序字典
来源：http://qut.iojbl.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://sfi.hongshengwenyu.top

[U11] Py：生成器表达式
来源：http://wbe.dianchejie.cn

(x * 2 for x in arr)
来源：http://plg.hnxiangtu.top

[U12] Py：取出现最多的 3 个元素
来源：http://ilh.haohaochexian.top

Counter(arr).most_common(3)
来源：http://asb.zhixingplan.top

[U13] Py：固定长度队列
来源：http://cnl.hnqzz.top

deque(maxlen=10)
来源：http://wkt.cqqwz.cn

[U14] Py：分组收集到列表
来源：http://crx.jyoumei.cn

defaultdict(list)
来源：http://oqd.zhijiandao.cn

[U15] Py：高精度计时
来源：http://ggg.shanyushiyangkeji.top

t = time.perf_counter()
来源：http://qwe.jqgfzy.top

[U16] Py：命令行参数解析
来源：http://xms.shanyushiyangkeji.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://yya.tarul.cn

[U17] Py：初始化日志
来源：http://bvo.chenlongwang.top

logging.basicConfig(level=logging.INFO)
来源：http://rfk.cdnleiting.top

[U18] Py：预编译正则
来源：http://mao.ybcxt.top

pat = re.compile(r"\d+")
来源：http://txv.hammf.cn

[U19] Py：正则替换带回调
来源：http://hfr.jiagoushi.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://efh.havefunace.top

[U20] Py：缓存函数结果
来源：http://umg.sweek.top

@functools.lru_cache(maxsize=None)
来源：http://ybr.shanyushiyangtech.top

[U21] Py：自定义上下文管理器
来源：http://yht.hywenlv.cn

@contextlib.contextmanager
来源：http://qug.cqqwz.cn

[U22] Py：矩阵转置
来源：http://ypj.mhx1999.top

list(zip(*m))
来源：http://aay.yfazqb.com

[U23] Py：分块读取大文件
来源：http://mcn.iojbl.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://nbl.yuanzhike.top

[U24] Py：路径操作
来源：http://hnw.sjlbkw.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://npp.yvedp.cn

[U25] Py：CSV 按字典读
来源：http://flb.wangdashe.top

csv.DictReader(f)
来源：http://yof.jqgfzy.top

[U26] Py：并发下载
来源：http://hqk.jqgfzy.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://fhc.ehwqpu.com

[U27] Py：异步 HTTP
来源：http://nqx.ehwqpu.com

aiohttp.ClientSession() 配合 async with
来源：http://npe.jyoumei.cn

[U28] Py：类型别名
来源：http://car.sjlbkw.cn

UserId = int
来源：http://klc.tarul.cn

[U29] Py：属性校验
来源：http://lcp.pycfn.com

@property 与 @x.setter 配合
来源：http://nzo.cqqwz.cn

[U30] Py：数据类
来源：http://bow.hcnkem.com

@dataclass(slots=True)
来源：http://zei.xuetiantiany.cn

[U31] Py：单测
来源：http://jpz.daria6918.cn

python -m pytest -q
来源：http://pij.wangdashe.top

[U32] Py：代码格式化
来源：http://wyy.shzxlz.cn

ruff format . && ruff check --fix .
来源：http://rsz.pycfn.com

[U33] Py：打包发布
来源：http://hat.vqdsnc.cn

python -m build  （依赖 pyproject.toml）
来源：http://pml.guowangkeji.top

[U34] Py：判断编码
来源：http://wdd.yuxming.cn

chardet.detect(raw)
来源：http://qww.guannengcc.top

[U35] Py：发送邮件
来源：http://khm.jyoumei.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://mji.tian-w.cn

[U36] Py：定时任务
来源：http://vts.cheryme.top

schedule.every(10).minutes.do(job)
来源：http://ukt.chenzaomai.com

[U37] Py：读写 Excel
来源：http://xpm.gogol.net.cn

pandas.read_excel / DataFrame.to_excel
来源：http://eba.jinqigufen.top

[U38] Py：获取脚本所在目录
来源：http://tmp.bjfxy.top

Path(__file__).resolve().parent
来源：http://eeh.shanyushiyangtech.top

[U39] Py：判断是否在交互环境
来源：http://ibr.zhixingplan.top

sys.stdout.isatty()
来源：http://pkh.yanxiufei.cn

[U40] Py：打印到标准错误
来源：http://nii.sufxvd.cn

print("err", file=sys.stderr)
来源：http://kqy.guowangkeji.top

[U41] PHP：初始化 Composer 项目
来源：http://pgp.chenzaomai.com

composer init;  composer require guzzlehttp/guzzle
来源：http://vdq.yfazqb.com

[U42] PHP：PSR-4 自动加载
来源：http://ybz.yuanzhike.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://usn.haohaochexian.top

[U43] PHP：声明命名空间
来源：http://oot.zdqjudy.top

namespace App\Http;
来源：http://vir.jiagoushi.top

[U44] PHP：开启严格类型
来源：http://qna.ivvv.top

declare(strict_types=1);
来源：http://kfg.cucudq.cn

[U45] PHP：类型声明与返回类型
来源：http://xzn.shangyingyoupin.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://rcq.ctjpmb.com

[U46] PHP：可空类型
来源：http://sxs.yj20258.top

?string $name = null
来源：http://qne.ctjpmb.com

[U47] PHP：联合类型
来源：http://qli.shuidangran.top

int|string $id
来源：http://ttk.ctjpmb.com

[U48] PHP：纯枚举
来源：http://woy.meibo888.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://nwy.52xcode.cn

[U49] PHP：只读属性
来源：http://xpl.gzhubu.top

public readonly string $name
来源：http://iuv.mhx1999.top

[U50] PHP：构造器属性提升
来源：http://okg.jinghuilouyu.cn

public function __construct(private int $id) {}
来源：http://zuw.aibaodan.cn

[U51] PHP：数组解构
来源：http://fqv.sysykeji.top

[$a, $b] = $arr;
来源：http://xvf.xuetiantiany.cn

[U52] PHP：箭头函数
来源：http://mvt.yj202588.top

$double = fn($x) => $x * 2;
来源：http://umm.316326.xyz

[U53] PHP：空合并运算符
来源：http://ouc.aizwys.cn

$v = $a ?? $b ?? "default";
来源：http://ung.tian-w.cn

[U54] PHP：空安全调用
来源：http://fjv.zhiwuduotai.top

$obj?->method()
来源：http://ncc.shanyushiyangkeji.top

[U55] PHP：match 表达式
来源：http://hof.sweek.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://ggr.tanke756.top

[U56] PHP：命名参数
来源：http://mrh.dashuyun.cn

f(a: 1, b: 2)
来源：http://hbc.jyoumei.cn

[U57] PHP：字符串插值
来源：http://wlw.ywan-chungtsiang.top

"值: {$a}"
来源：http://meg.mhx1999.top

[U58] PHP：数组三件套
来源：http://czi.ywan-chungtsiang.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://frn.kuanghao11.cn

[U59] PHP：自定义排序
来源：http://lou.fktsv.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mns.daria6918.cn

[U60] PHP：JSON 编解码
来源：http://qbo.cucudq.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://bsf.xingfuxueyuan.xyz

[U61] PHP：正则
来源：http://mjs.yvedp.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://qyt.c1oappe.top

[U62] PHP：日期对象
来源：http://das.bbcook.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://zjj.yfazqb.com

[U63] PHP：文件读写
来源：http://ltc.hnxiangtu.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://gyt.hywenlv.cn

[U64] PHP：目录遍历
来源：http://lzj.jianghu66.top

glob("dir/*.php");  scandir("dir");
来源：http://vjr.yuxming.cn

[U65] PHP：会话
来源：http://bes.ywan-chungtsiang.top

session_start();  $_SESSION["uid"] = 1;
来源：http://grk.tianlin.xyz

[U66] PHP：设置 Cookie
来源：http://mog.shanyushiyangkeji.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://cle.uphjek.com

[U67] PHP：处理文件上传
来源：http://rjc.tianlin.xyz

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://cfl.yuxming.cn

[U68] PHP：PDO 连接
来源：http://tpo.ivvv.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://bps.bbcook.cn

[U69] PHP：PDO 预处理
来源：http://xsk.jinqigfzy.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://itw.yonumen.top

[U70] PHP：PDO 事务
来源：http://iaq.zhiwuduotai.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://kau.zhiwuduotai.top

[U71] PHP：抛出异常
来源：http://xiz.aizwys.cn

throw new RuntimeException("失败", 500);
来源：http://pfw.tianlin.xyz

[U72] PHP：写错误日志
来源：http://lrp.jyoumei.cn

error_log("失败: " . $e->getMessage());
来源：http://efu.jlsjyb.cn

[U73] PHP：读取 ini 配置
来源：http://kko.havefunace.top

parse_ini_file("config.ini", true)
来源：http://wiq.yuxming.cn

[U74] PHP：读取环境变量
来源：http://oer.sweek.top

getenv("APP_ENV") ?: "production"
来源：http://odo.uphjek.com

[U75] PHP：依赖注入
来源：http://qbi.zycfv.cn

composer require psr/container
来源：http://jey.zhaomingkeji.xyz

[U76] PHP：简单路由
来源：http://age.zhengqikj.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://aaq.quarkkingdee.top

[U77] PHP：模板渲染
来源：http://lrs.zycfv.cn

composer require twig/twig
来源：http://bxx.epnwcf.com

[U78] PHP：单元测试
来源：http://qwt.fktsv.cn

composer require --dev phpunit/phpunit
来源：http://lua.xuanzx.com

[U79] PHP：静态分析
来源：http://hxu.hcnkem.com

composer require --dev phpstan/phpstan
来源：http://fku.feifeiyinyue.top

[U80] PHP：代码规范修复
来源：http://ihe.xuetiantiany.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://mws.jqgufenzy.top

[U81] JS：初始化项目
来源：http://cvh.ehwqpu.com

npm init -y;  npm i express
来源：http://lbo.jianghu66.top

[U82] JS：package.json 脚本
来源：http://xpz.hfpthk.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://ifq.nwbrower.top

[U83] JS：ES Module 导入导出
来源：http://ikm.sjlbkw.cn

export const a = 1;  import { a } from "./m.js";
来源：http://kly.uphjek.com

[U84] JS：CommonJS 写法
来源：http://yst.nanxinkj.top

module.exports = { a };  const { a } = require("./m");
来源：http://tsc.smart0.xyz

[U85] JS：可选链
来源：http://pdo.hesvh.cn

a?.b?.c
来源：http://mik.zycfv.cn

[U86] JS：空值合并
来源：http://lge.zhaomingkeji.xyz

a ?? b
来源：http://qza.fengsongda.top

[U87] JS：解构默认值
来源：http://exs.yj20258.top

const { a = 1, b = 2 } = obj;
来源：http://ajs.hnxiangtu.top

[U88] JS：对象展开合并
来源：http://bgs.gzhubu.top

{ ...a, ...b }
来源：http://eit.jinyuanbaomall.cn

[U89] JS：数组去重
来源：http://cma.wangdashe.top

[...new Set(arr)]
来源：http://knr.aibaodan.cn

[U90] JS：数字数组排序
来源：http://uos.c1oappe.top

[...arr].sort((a, b) => a - b)
来源：http://jgp.andypj.xyz

[U91] JS：对象键值遍历
来源：http://tmh.wangdashe.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://otj.cucudq.cn

[U92] JS：深拷贝
来源：http://tpi.ywan-chungtsiang.top

structuredClone(obj)
来源：http://frx.yonumen.top

[U93] JS：模板字符串
来源：http://zrj.gogol.net.cn

`共 ${n} 条`
来源：http://hpp.ivvv.top

[U94] JS：箭头函数
来源：http://pco.bbcook.cn

const double = x => x * 2;
来源：http://oxh.9152youxi.cn

[U95] JS：Promise 包装
来源：http://tpd.tarul.cn

new Promise((resolve, reject) => {})
来源：http://yly.yueranfly.top

[U96] JS：async/await 与异常
来源：http://spb.zdqjudy.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://fwm.haohaochexian.top

[U97] JS：并发请求
来源：http://bij.cucudq.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://kub.zycfv.cn

[U98] JS：fetch 带 JSON
来源：http://kct.yj202588.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://bdx.jinyuanbaomall.cn

[U99] JS：事件监听
来源：http://alt.pycfn.com

el.addEventListener("click", e => {})
来源：http://oky.daria6918.cn

[U100] JS：DOM 查询
来源：http://oik.hysaishi.cn

document.querySelector(".item")
来源：http://roo.guowangkeji.top

[U101] JS：classList 操作
来源：http://cru.ydjk.org.cn

el.classList.toggle("active")
来源：http://duy.uphjek.com

[U102] JS：本地存储
来源：http://kii.snrcjt.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://qvr.ywan-chungtsiang.top

[U103] JS：定时器
来源：http://zcr.nanxinkj.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://jrn.zycfv.cn

[U104] JS：防抖
来源：http://brd.hnxiangtu.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://olr.yonumen.top

[U105] JS：节流
来源：http://xhm.hfpthk.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://eua.pycfn.com

[U106] JS：日期格式化
来源：http://iec.gzhubu.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://whg.shangyingyoupin.top

[U107] JS：数字千分位
来源：http://den.sjlbkw.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://daf.yonumen.top

[U108] JS：随机整数
来源：http://ftg.jqgufenzy.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://rno.hywenlv.cn

[U109] JS：数组分组
来源：http://jfa.c1oappe.top

Object.groupBy(arr, x => x.type)
来源：http://psu.pycfn.com

[U110] JS：数组分块
来源：http://ksv.wangshuangyany.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://jaz.snrcjt.cn

[U111] JS：对象转 Map
来源：http://htv.aizwys.cn

new Map(Object.entries(obj))
来源：http://cdr.dashuyun.cn

[U112] JS：字符串补位
来源：http://kap.jianghu66.top

"7".padStart(3, "0")
来源：http://tki.jlsjyb.cn

[U113] JS：正则替换全部
来源：http://gtt.chenjidiqi.icu

s.replaceAll("a", "b")
来源：http://olq.sxryk.cn

[U114] JS：JSON 深比较
来源：http://jyf.xinyue.icu

JSON.stringify(a) === JSON.stringify(b)
来源：http://pqp.quarkkingdee.top

[U115] JS：生成 UUID
来源：http://ght.hcnkem.com

crypto.randomUUID()
来源：http://ztl.52xcode.cn

[U116] JS：类型检查（JSDoc）
来源：http://qof.hnqzz.top

/** @param {string} name */ function f(name) {}
来源：http://jwx.ppjwa.cn

[U117] JS：单元测试
来源：http://onm.nwbrower.top

npm i -D vitest;  npx vitest
来源：http://eaq.mhx1999.top

[U118] JS：开发服务器
来源：http://ooy.kuanghao11.cn

npm i -D vite;  npx vite
来源：http://eih.jinghuilouyu.cn

[U119] JS：生产构建
来源：http://fyr.bbcook.cn

npx vite build
来源：http://ksv.hywenlv.cn

[U120] JS：读取环境变量（Vite）
来源：http://pyv.jqgufenzy.top

import.meta.env.VITE_API_URL
来源：http://pkl.sweek.top

================================================================================
来源：http://smq.uphjek.com

统计汇总
来源：http://rcx.tanke756.top

================================================================================
来源：http://gue.ctjpmb.com

按语言统计（条）：
来源：http://ccs.redwolf501.top

Python ......... 252
来源：http://aue.yuxming.cn

PHP ............ 252
来源：http://otk.xingfuxueyuan.xyz

JavaScript ..... 252
来源：http://lve.cdnleiting.top

TypeScript ..... 212
来源：http://luj.yuxming.cn

Java ........... 212
来源：http://khr.yongpay.top

Go ............. 212
来源：http://yhm.bbcook.cn

Ruby ........... 212
来源：http://vjs.chenjidiqi.icu

C# ............. 212
来源：http://nmk.9152youxi.cn

C .............. 30
来源：http://mnb.hnqzz.top

C++ ............ 30
来源：http://wmj.aibaodan.cn

SQL ............ 90
来源：http://lmi.jyoumei.cn

Bash ........... 80
来源：http://suq.0kj1m.cn

Kotlin ......... 15
来源：http://xiy.hcnkem.com

Swift .......... 15
来源：http://ftd.tianlin.xyz

Lua ............ 10
来源：http://tkl.yonumen.top

Perl ........... 10
来源：http://lze.zhiwuduotai.top

Scala .......... 10
来源：http://bod.xziqi.cn

------------------------------------
来源：http://hbb.tanke756.top

合计 ........... 2106 条
来源：http://ehg.zhoulong.xyz

按章节统计：
来源：http://ilp.jyoumei.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://paj.quarkkingdee.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://dwm.smart0.xyz

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://sai.yj20258.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://qjy.yonumen.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://dwb.mhx1999.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://grm.fzhhl.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://lcl.yueranfly.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://rkq.uphjek.com

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://zzr.ivvv.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://ivt.svipenyu.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://maw.mhx1999.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://zos.bjfxy.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://kly.pengpengdd.cyou

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://ful.ivvv.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://tkt.cashguo.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://wot.0kj1m.cn

Q SQL 专题                              90
来源：http://emm.jinqigufen.top

R Bash 专题                             80
来源：http://sdq.jinqigfzy.top

S C / C++ 专题                          60
来源：http://lra.shanyushiyangtech.top

T 其他语言补充                          60
来源：http://sjg.xuanzx.com

U 高频实用片段                         120
来源：http://gce.birdmap.top

------------------------------------
来源：http://xse.yangfankeji.com

合计                                  2106 条
来源：http://beh.nwbrower.top

--------------------------------------------------------------------------------
来源：http://uix.zdqjudy.top

使用提醒
来源：http://uaz.tanke756.top

--------------------------------------------------------------------------------
来源：http://lda.xziqi.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://gib.pycfn.com

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://lid.yuanzhike.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://bgp.guowangkeji.top

在旧版本上使用前请先确认语法支持情况。
来源：http://tli.bbcook.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://ghp.0kj1m.cn

—— 文件结束 ——
来源：http://nab.cheryme.top

================================================================================
来源：http://mqx.smart0.xyz

程序语言常见例子速查手册（2024 版）
来源：http://zvu.dashuyun.cn

Common Programming Examples Cheat Book
来源：http://aur.ivvv.top

================================================================================
来源：http://rus.sjlbkw.cn

【收录内容】
来源：http://vmx.yonumen.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://dqz.zhongyouzk.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://lnv.ppjwa.cn

SQL · Bash · C · C++
来源：http://bxf.ppjwa.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://pvr.zhiwuduotai.top

【使用说明】
来源：http://pct.chenzaomai.com

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://ueq.yonumen.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://ozl.daria6918.cn


<!-- 参考信息 -->