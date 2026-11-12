代发 wailian999

[U05] Py：列表去重且保序
来源：http://qoy.ywan-chungtsiang.top

list(dict.fromkeys(arr))
来源：http://gij.wangdashe.top

[U06] Py：合并两个字典
来源：http://qoa.uphjek.com

{**a, **b}
来源：http://gsr.vqdsnc.cn

[U07] Py：反转字典键值
来源：http://dnt.vqdsnc.cn

{v: k for k, v in d.items()}
来源：http://xtu.haohaochexian.top

[U08] Py：展平二维列表
来源：http://cot.tianlin.xyz

[y for x in nested for y in x]
来源：http://jkn.ydjk.org.cn

[U09] Py：字典取最大值的键
来源：http://mnm.yonumen.top

max(d, key=d.get)
来源：http://rbc.hfpthk.cn

[U10] Py：按值排序字典
来源：http://yjo.kuanghao11.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://ssv.uphjek.com

[U11] Py：生成器表达式
来源：http://xif.ehwqpu.com

(x * 2 for x in arr)
来源：http://hga.yongpay.top

[U12] Py：取出现最多的 3 个元素
来源：http://azz.haohaochexian.top

Counter(arr).most_common(3)
来源：http://xoo.sufxvd.cn

[U13] Py：固定长度队列
来源：http://mbp.yj202588.top

deque(maxlen=10)
来源：http://tpl.cdnleiting.top

[U14] Py：分组收集到列表
来源：http://dig.jlsjyb.cn

defaultdict(list)
来源：http://kyr.fzhhl.top

[U15] Py：高精度计时
来源：http://beq.jqgufenzy.top

t = time.perf_counter()
来源：http://axq.chenjidiqi.icu

[U16] Py：命令行参数解析
来源：http://btm.hnqzz.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://prb.xingfuxueyuan.xyz

[U17] Py：初始化日志
来源：http://vnz.zhijiandao.cn

logging.basicConfig(level=logging.INFO)
来源：http://lvp.quarkkingdee.top

[U18] Py：预编译正则
来源：http://hky.zhongyouzk.top

pat = re.compile(r"\d+")
来源：http://qav.tanke756.top

[U19] Py：正则替换带回调
来源：http://uyf.tarul.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://oqt.ywan-chungtsiang.top

[U20] Py：缓存函数结果
来源：http://omh.daria6918.cn

@functools.lru_cache(maxsize=None)
来源：http://ibt.svipenyu.cn

[U21] Py：自定义上下文管理器
来源：http://zty.sxryk.cn

@contextlib.contextmanager
来源：http://qxj.hammf.cn

[U22] Py：矩阵转置
来源：http://rtg.xziqi.cn

list(zip(*m))
来源：http://mwi.jinghuilouyu.cn

[U23] Py：分块读取大文件
来源：http://vij.zdbjq.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://ech.xingfuxueyuan.xyz

[U24] Py：路径操作
来源：http://mct.316326.xyz

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://vko.yonumen.top

[U25] Py：CSV 按字典读
来源：http://pst.shzxlz.cn

csv.DictReader(f)
来源：http://msx.yanxiufei.cn

[U26] Py：并发下载
来源：http://jaw.yuanzhike.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://sqd.quarkkingdee.top

[U27] Py：异步 HTTP
来源：http://shn.epnwcf.com

aiohttp.ClientSession() 配合 async with
来源：http://vzn.dianchejie.cn

[U28] Py：类型别名
来源：http://pja.0kj1m.cn

UserId = int
来源：http://nzi.cheryme.top

[U29] Py：属性校验
来源：http://sgd.xylfe.cn

@property 与 @x.setter 配合
来源：http://lbr.zhijiandao.cn

[U30] Py：数据类
来源：http://vnu.shanyushiyangkeji.top

@dataclass(slots=True)
来源：http://jvg.ybcxt.top

[U31] Py：单测
来源：http://skg.yanxiufei.cn

python -m pytest -q
来源：http://pxo.gzhubu.top

[U32] Py：代码格式化
来源：http://ohg.nwbrower.top

ruff format . && ruff check --fix .
来源：http://mhw.tanke756.top

[U33] Py：打包发布
来源：http://gvh.ydjk.org.cn

python -m build  （依赖 pyproject.toml）
来源：http://xns.gzhubu.top

[U34] Py：判断编码
来源：http://woq.ybcxt.top

chardet.detect(raw)
来源：http://qab.pycfn.com

[U35] Py：发送邮件
来源：http://lci.hysaishi.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://xyj.jlsjyb.cn

[U36] Py：定时任务
来源：http://evw.yj202588.top

schedule.every(10).minutes.do(job)
来源：http://xmy.hammf.cn

[U37] Py：读写 Excel
来源：http://ihn.svipenyu.cn

pandas.read_excel / DataFrame.to_excel
来源：http://vca.zhixingplan.top

[U38] Py：获取脚本所在目录
来源：http://nwt.yueranfly.top

Path(__file__).resolve().parent
来源：http://imh.bbcook.cn

[U39] Py：判断是否在交互环境
来源：http://zkb.feifeiyinyue.top

sys.stdout.isatty()
来源：http://vvs.wangdashe.top

[U40] Py：打印到标准错误
来源：http://rbn.cqqwz.cn

print("err", file=sys.stderr)
来源：http://kjq.iojbl.cn

[U41] PHP：初始化 Composer 项目
来源：http://jse.yangfankeji.com

composer init;  composer require guzzlehttp/guzzle
来源：http://nxi.smart0.xyz

[U42] PHP：PSR-4 自动加载
来源：http://bdi.hysaishi.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://stt.hywenlv.cn

[U43] PHP：声明命名空间
来源：http://yku.9152youxi.cn

namespace App\Http;
来源：http://rhu.ywan-chungtsiang.top

[U44] PHP：开启严格类型
来源：http://jop.zdqjudy.top

declare(strict_types=1);
来源：http://glj.kuanghao11.cn

[U45] PHP：类型声明与返回类型
来源：http://cgc.aizwys.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://bij.cucudq.cn

[U46] PHP：可空类型
来源：http://nsm.nwbrower.top

?string $name = null
来源：http://adr.sysykeji.top

[U47] PHP：联合类型
来源：http://ppe.bjfxy.top

int|string $id
来源：http://lre.hesvh.cn

[U48] PHP：纯枚举
来源：http://qyq.ydzc1.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://imx.shanyushiyangtech.top

[U49] PHP：只读属性
来源：http://hwj.ywan-chungtsiang.top

public readonly string $name
来源：http://mmy.xingfuxueyuan.xyz

[U50] PHP：构造器属性提升
来源：http://dgy.ppjwa.cn

public function __construct(private int $id) {}
来源：http://rts.316326.xyz

[U51] PHP：数组解构
来源：http://nno.wangshuangyany.cn

[$a, $b] = $arr;
来源：http://ret.yvedp.cn

[U52] PHP：箭头函数
来源：http://wbb.sysykeji.top

$double = fn($x) => $x * 2;
来源：http://czl.shuidangran.top

[U53] PHP：空合并运算符
来源：http://evf.fehbvm.com

$v = $a ?? $b ?? "default";
来源：http://iup.fktsv.cn

[U54] PHP：空安全调用
来源：http://hpq.gogol.net.cn

$obj?->method()
来源：http://xyo.yj20258.top

[U55] PHP：match 表达式
来源：http://yts.dianchejie.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://vwz.gaohongyu789.top

[U56] PHP：命名参数
来源：http://rcf.mhx1999.top

f(a: 1, b: 2)
来源：http://nrk.xingfuxueyuan.xyz

[U57] PHP：字符串插值
来源：http://pmr.yj20258.top

"值: {$a}"
来源：http://kbh.tarul.cn

[U58] PHP：数组三件套
来源：http://jag.yuanzhike.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://jst.jianghu66.top

[U59] PHP：自定义排序
来源：http://ccd.xziqi.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://kld.jqgfzy.top

[U60] PHP：JSON 编解码
来源：http://ozo.sxryk.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://tef.shzxlz.cn

[U61] PHP：正则
来源：http://gca.9152youxi.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://ltw.pengpengdd.cyou

[U62] PHP：日期对象
来源：http://mzs.shanyushiyangtech.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://sxc.xingfuxueyuan.xyz

[U63] PHP：文件读写
来源：http://cbc.yueranfly.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://oqg.zycfv.cn

[U64] PHP：目录遍历
来源：http://hdp.jlsjyb.cn

glob("dir/*.php");  scandir("dir");
来源：http://yvm.snrcjt.cn

[U65] PHP：会话
来源：http://nnc.sjlbkw.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://uof.birdmap.top

[U66] PHP：设置 Cookie
来源：http://fsf.sufxvd.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://gjo.cashguo.top

[U67] PHP：处理文件上传
来源：http://zhs.chenlongwang.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://xbj.yfazqb.com

[U68] PHP：PDO 连接
来源：http://jtr.yj20258888.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://ybn.bjfxy.top

[U69] PHP：PDO 预处理
来源：http://pel.haohaochexian.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://zui.shzxlz.cn

[U70] PHP：PDO 事务
来源：http://yam.guannengcc.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://nam.jqgufenzy.top

[U71] PHP：抛出异常
来源：http://cii.dashuyun.cn

throw new RuntimeException("失败", 500);
来源：http://ovq.xuetiantiany.cn

[U72] PHP：写错误日志
来源：http://wsp.hysaishi.cn

error_log("失败: " . $e->getMessage());
来源：http://rjz.nwbrower.top

[U73] PHP：读取 ini 配置
来源：http://bzz.dianchejie.cn

parse_ini_file("config.ini", true)
来源：http://xqa.jqgufenzy.top

[U74] PHP：读取环境变量
来源：http://djc.yanxiufei.cn

getenv("APP_ENV") ?: "production"
来源：http://vre.ivvv.top

[U75] PHP：依赖注入
来源：http://azz.yuanzhike.top

composer require psr/container
来源：http://bib.fehbvm.com

[U76] PHP：简单路由
来源：http://svb.gogol.net.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://zur.fengsongda.top

[U77] PHP：模板渲染
来源：http://nyv.snrcjt.cn

composer require twig/twig
来源：http://fjl.hnqzz.top

[U78] PHP：单元测试
来源：http://lxw.nwbrower.top

composer require --dev phpunit/phpunit
来源：http://tye.chenzaomai.com

[U79] PHP：静态分析
来源：http://jxe.hammf.cn

composer require --dev phpstan/phpstan
来源：http://wok.xziqi.cn

[U80] PHP：代码规范修复
来源：http://bsl.epnwcf.com

composer require --dev friendsofphp/php-cs-fixer
来源：http://ymi.xuanzx.com

[U81] JS：初始化项目
来源：http://wzi.hesvh.cn

npm init -y;  npm i express
来源：http://iae.hammf.cn

[U82] JS：package.json 脚本
来源：http://byd.0kj1m.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://xev.gotoacloud.top

[U83] JS：ES Module 导入导出
来源：http://ujj.hnqzz.top

export const a = 1;  import { a } from "./m.js";
来源：http://cla.0kj1m.cn

[U84] JS：CommonJS 写法
来源：http://gto.gaohongyu789.top

module.exports = { a };  const { a } = require("./m");
来源：http://qnh.cashguo.top

[U85] JS：可选链
来源：http://rdp.zhaomingkeji.xyz

a?.b?.c
来源：http://eoh.nanxuanxn.top

[U86] JS：空值合并
来源：http://qhj.bjfxy.top

a ?? b
来源：http://vqc.zhongyouzk.top

[U87] JS：解构默认值
来源：http://qcf.zhongyouzk.top

const { a = 1, b = 2 } = obj;
来源：http://ois.epnwcf.com

[U88] JS：对象展开合并
来源：http://hdl.yongpay.top

{ ...a, ...b }
来源：http://hza.yfazqb.com

[U89] JS：数组去重
来源：http://npz.iojbl.cn

[...new Set(arr)]
来源：http://fjp.pycfn.com

[U90] JS：数字数组排序
来源：http://svu.jqgufenzy.top

[...arr].sort((a, b) => a - b)
来源：http://pbx.shangyingyoupin.top

[U91] JS：对象键值遍历
来源：http://ivj.guannengcc.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://ykb.zhijiandao.cn

[U92] JS：深拷贝
来源：http://bwr.daria6918.cn

structuredClone(obj)
来源：http://isk.zycfv.cn

[U93] JS：模板字符串
来源：http://kop.yueranfly.top

`共 ${n} 条`
来源：http://son.chenlongwang.top

[U94] JS：箭头函数
来源：http://ivh.chenjidiqi.icu

const double = x => x * 2;
来源：http://enc.gotoacloud.top

[U95] JS：Promise 包装
来源：http://qvu.sysykeji.top

new Promise((resolve, reject) => {})
来源：http://ywy.xingfuxueyuan.xyz

[U96] JS：async/await 与异常
来源：http://ufl.shanyushiyangkeji.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://avy.316326.xyz

[U97] JS：并发请求
来源：http://jfz.daxiang520.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://ewu.tanke756.top

[U98] JS：fetch 带 JSON
来源：http://sow.sweek.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://ikq.tianlin.xyz

[U99] JS：事件监听
来源：http://osr.ehwqpu.com

el.addEventListener("click", e => {})
来源：http://htv.hammf.cn

[U100] JS：DOM 查询
来源：http://nkb.hysaishi.cn

document.querySelector(".item")
来源：http://vns.9152youxi.cn

[U101] JS：classList 操作
来源：http://gkp.zycfv.cn

el.classList.toggle("active")
来源：http://hee.shanyushiyangtech.top

[U102] JS：本地存储
来源：http://xtu.zhijiandao.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://bjc.iojbl.cn

[U103] JS：定时器
来源：http://ids.aibaodan.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://pjb.ivvv.top

[U104] JS：防抖
来源：http://hgv.yuxming.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://jwo.jqgufenzy.top

[U105] JS：节流
来源：http://hos.snrcjt.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://pvl.zdbjq.cn

[U106] JS：日期格式化
来源：http://gxf.yj20258.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://roe.dianchejie.cn

[U107] JS：数字千分位
来源：http://ely.ivvv.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://qod.svipenyu.cn

[U108] JS：随机整数
来源：http://uum.hesvh.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://ndl.fktsv.cn

[U109] JS：数组分组
来源：http://zbh.cqqwz.cn

Object.groupBy(arr, x => x.type)
来源：http://rfp.epnwcf.com

[U110] JS：数组分块
来源：http://wfe.xuetiantiany.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://bjc.fanxiaobao.xyz

[U111] JS：对象转 Map
来源：http://dvw.hysaishi.cn

new Map(Object.entries(obj))
来源：http://dkk.iojbl.cn

[U112] JS：字符串补位
来源：http://bsl.yangfankeji.com

"7".padStart(3, "0")
来源：http://prp.zhongyouzk.top

[U113] JS：正则替换全部
来源：http://iwb.cqqwz.cn

s.replaceAll("a", "b")
来源：http://xkr.fzhhl.top

[U114] JS：JSON 深比较
来源：http://wto.yfazqb.com

JSON.stringify(a) === JSON.stringify(b)
来源：http://bdo.fanxiaobao.xyz

[U115] JS：生成 UUID
来源：http://nqf.ywan-chungtsiang.top

crypto.randomUUID()
来源：http://fwr.ivvv.top

[U116] JS：类型检查（JSDoc）
来源：http://nyr.andypj.xyz

/** @param {string} name */ function f(name) {}
来源：http://tzq.feifeiyinyue.top

[U117] JS：单元测试
来源：http://ump.smart0.xyz

npm i -D vitest;  npx vitest
来源：http://ahp.tianlin.xyz

[U118] JS：开发服务器
来源：http://bnd.sjlbkw.cn

npm i -D vite;  npx vite
来源：http://zmw.zdbjq.cn

[U119] JS：生产构建
来源：http://bxz.ydjk.org.cn

npx vite build
来源：http://xal.yj20258888.top

[U120] JS：读取环境变量（Vite）
来源：http://rhb.shanyushiyangtech.top

import.meta.env.VITE_API_URL
来源：http://mez.jqgufenzy.top

================================================================================
来源：http://pxp.xziqi.cn

统计汇总
来源：http://wfd.jinyuanbaomall.cn

================================================================================
来源：http://mpe.mhx1999.top

按语言统计（条）：
来源：http://ijd.vqdsnc.cn

Python ......... 252
来源：http://sod.shanyushiyangtech.top

PHP ............ 252
来源：http://hka.ydjk.org.cn

JavaScript ..... 252
来源：http://dss.jyoumei.cn

TypeScript ..... 212
来源：http://wtu.yongpay.top

Java ........... 212
来源：http://tbn.zdbjq.cn

Go ............. 212
来源：http://obd.hfpthk.cn

Ruby ........... 212
来源：http://ata.52xcode.cn

C# ............. 212
来源：http://oxb.xylfe.cn

C .............. 30
来源：http://zvh.xuanzx.com

C++ ............ 30
来源：http://qna.hammf.cn

SQL ............ 90
来源：http://mys.birdmap.top

Bash ........... 80
来源：http://ksy.pycfn.com

Kotlin ......... 15
来源：http://aph.aizwys.cn

Swift .......... 15
来源：http://jzy.hysaishi.cn

Lua ............ 10
来源：http://tyu.jlsjyb.cn

Perl ........... 10
来源：http://qbv.ydjk.org.cn

Scala .......... 10
来源：http://nnu.ydjk.org.cn

------------------------------------
来源：http://vfj.ehwqpu.com

合计 ........... 2106 条
来源：http://llr.zhoulong.xyz

按章节统计：
来源：http://gfj.svipenyu.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://bup.cdnleiting.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://uqu.epnwcf.com

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://tgq.shuidangran.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://vhb.hfpthk.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://idg.guannengcc.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://alm.shzxlz.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://avc.birdmap.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://ius.xingfuxueyuan.xyz

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://zfk.mhx1999.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://kxi.yangfankeji.com

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://jms.9152youxi.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://rhf.snrcjt.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://agw.yfazqb.com

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://bbr.tarul.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://qzx.pycfn.com

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://acr.ctjpmb.com

Q SQL 专题                              90
来源：http://ahf.tianlin.xyz

R Bash 专题                             80
来源：http://lbs.yonumen.top

S C / C++ 专题                          60
来源：http://ttw.zhaomingkeji.xyz

T 其他语言补充                          60
来源：http://qky.daria6918.cn

U 高频实用片段                         120
来源：http://xts.jqgfzy.top

------------------------------------
来源：http://iwh.hcnkem.com

合计                                  2106 条
来源：http://qxe.yueranfly.top

--------------------------------------------------------------------------------
来源：http://lrd.snrcjt.cn

使用提醒
来源：http://ekv.zhengqikj.top

--------------------------------------------------------------------------------
来源：http://epi.ivvv.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://nvz.yj202588.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://oxn.wangdashe.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://vyp.sjlbkw.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://spo.cqqwz.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://iqv.bjfxy.top

—— 文件结束 ——
来源：http://qsk.feifeiyinyue.top

================================================================================
来源：http://jbt.jqgfzy.top

程序语言常见例子速查手册（2024 版）
来源：http://xbl.haohaochexian.top

Common Programming Examples Cheat Book
来源：http://iev.daria6918.cn

================================================================================
来源：http://war.316326.xyz

【收录内容】
来源：http://qsn.c1oappe.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://ozw.jiagoushi.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://eir.xingfuxueyuan.xyz

SQL · Bash · C · C++
来源：http://lze.yj202588.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://mpj.uphjek.com

【使用说明】
来源：http://ohx.sysykeji.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://mog.zhijiandao.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://jsc.bjfxy.top


<!-- 参考信息 -->