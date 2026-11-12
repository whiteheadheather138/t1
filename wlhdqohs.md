代发 wailian999

[U17] Py：初始化日志
来源：http://zis.jinqigfzy.top

logging.basicConfig(level=logging.INFO)
来源：http://dme.zhiwuduotai.top

[U18] Py：预编译正则
来源：http://jqu.daxiang520.top

pat = re.compile(r"\d+")
来源：http://pyf.shanyushiyangtech.top

[U19] Py：正则替换带回调
来源：http://nvf.tianlin.xyz

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://kbb.yvedp.cn

[U20] Py：缓存函数结果
来源：http://hbp.ivvv.top

@functools.lru_cache(maxsize=None)
来源：http://jyk.sjlbkw.cn

[U21] Py：自定义上下文管理器
来源：http://zpp.xuetiantiany.cn

@contextlib.contextmanager
来源：http://dwc.fanxiaobao.xyz

[U22] Py：矩阵转置
来源：http://bnx.hammf.cn

list(zip(*m))
来源：http://fab.xuetiantiany.cn

[U23] Py：分块读取大文件
来源：http://clv.tanke756.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://ufi.jinqigufen.top

[U24] Py：路径操作
来源：http://wke.gzhubu.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://qgw.sweek.top

[U25] Py：CSV 按字典读
来源：http://trn.feifeiyinyue.top

csv.DictReader(f)
来源：http://lhz.xylfe.cn

[U26] Py：并发下载
来源：http://dec.vqdsnc.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://xuz.yueranfly.top

[U27] Py：异步 HTTP
来源：http://mpn.sxryk.cn

aiohttp.ClientSession() 配合 async with
来源：http://mrp.gzhubu.top

[U28] Py：类型别名
来源：http://jul.nanxuanxn.top

UserId = int
来源：http://djj.yuanzhike.top

[U29] Py：属性校验
来源：http://szl.daria6918.cn

@property 与 @x.setter 配合
来源：http://tuv.yj20258888.top

[U30] Py：数据类
来源：http://yyb.snrcjt.cn

@dataclass(slots=True)
来源：http://drn.sysykeji.top

[U31] Py：单测
来源：http://prw.havefunace.top

python -m pytest -q
来源：http://bcm.hywenlv.cn

[U32] Py：代码格式化
来源：http://aiu.ybcxt.top

ruff format . && ruff check --fix .
来源：http://jin.iojbl.cn

[U33] Py：打包发布
来源：http://wtd.fehbvm.com

python -m build  （依赖 pyproject.toml）
来源：http://gid.fzhhl.top

[U34] Py：判断编码
来源：http://uoa.haohaochexian.top

chardet.detect(raw)
来源：http://boa.xinyue.icu

[U35] Py：发送邮件
来源：http://bcd.jinqigufen.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://xph.mhx1999.top

[U36] Py：定时任务
来源：http://fqt.hnxiangtu.top

schedule.every(10).minutes.do(job)
来源：http://reo.zhongyouzk.top

[U37] Py：读写 Excel
来源：http://knr.yangfankeji.com

pandas.read_excel / DataFrame.to_excel
来源：http://rcr.cdnleiting.top

[U38] Py：获取脚本所在目录
来源：http://ans.sufxvd.cn

Path(__file__).resolve().parent
来源：http://nyx.jqgfzy.top

[U39] Py：判断是否在交互环境
来源：http://nha.hnqzz.top

sys.stdout.isatty()
来源：http://hpp.snrcjt.cn

[U40] Py：打印到标准错误
来源：http://oih.havefunace.top

print("err", file=sys.stderr)
来源：http://jvv.uphjek.com

[U41] PHP：初始化 Composer 项目
来源：http://wbl.fehbvm.com

composer init;  composer require guzzlehttp/guzzle
来源：http://rgs.nwbrower.top

[U42] PHP：PSR-4 自动加载
来源：http://ktc.vqdsnc.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://eip.cqqwz.cn

[U43] PHP：声明命名空间
来源：http://hrm.nwbrower.top

namespace App\Http;
来源：http://qbd.quarkkingdee.top

[U44] PHP：开启严格类型
来源：http://erp.tianlin.xyz

declare(strict_types=1);
来源：http://rpb.xingfuxueyuan.xyz

[U45] PHP：类型声明与返回类型
来源：http://xnx.smart0.xyz

function add(int $a, int $b): int { return $a + $b; }
来源：http://ccy.havefunace.top

[U46] PHP：可空类型
来源：http://lmv.fengsongda.top

?string $name = null
来源：http://zwv.dashuyun.cn

[U47] PHP：联合类型
来源：http://wkb.cheryme.top

int|string $id
来源：http://jaz.ctjpmb.com

[U48] PHP：纯枚举
来源：http://qbx.jiagoushi.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://dwt.gaohongyu789.top

[U49] PHP：只读属性
来源：http://dgm.pycfn.com

public readonly string $name
来源：http://rta.wangdashe.top

[U50] PHP：构造器属性提升
来源：http://ohf.sweek.top

public function __construct(private int $id) {}
来源：http://uvy.xuanzx.com

[U51] PHP：数组解构
来源：http://rve.zhijiandao.cn

[$a, $b] = $arr;
来源：http://pnw.yj20258.top

[U52] PHP：箭头函数
来源：http://jfw.shanyushiyangtech.top

$double = fn($x) => $x * 2;
来源：http://wvt.shanyushiyangtech.top

[U53] PHP：空合并运算符
来源：http://wnw.shanyushiyangkeji.top

$v = $a ?? $b ?? "default";
来源：http://nta.zhengqikj.top

[U54] PHP：空安全调用
来源：http://ytw.hfpthk.cn

$obj?->method()
来源：http://lke.nanxinkj.top

[U55] PHP：match 表达式
来源：http://mww.cqqwz.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://cku.aizwys.cn

[U56] PHP：命名参数
来源：http://xpv.ehwqpu.com

f(a: 1, b: 2)
来源：http://thc.sufxvd.cn

[U57] PHP：字符串插值
来源：http://auk.chenlongwang.top

"值: {$a}"
来源：http://vrm.yanxiufei.cn

[U58] PHP：数组三件套
来源：http://ebt.zhaomingkeji.xyz

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://zkc.hesvh.cn

[U59] PHP：自定义排序
来源：http://rrh.dianchejie.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ipt.xingfuxueyuan.xyz

[U60] PHP：JSON 编解码
来源：http://kcm.tianlin.xyz

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://ybe.epnwcf.com

[U61] PHP：正则
来源：http://etz.chenjidiqi.icu

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://fwx.hywenlv.cn

[U62] PHP：日期对象
来源：http://imx.jlsjyb.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://qix.tian-w.cn

[U63] PHP：文件读写
来源：http://fme.vehdjk.com

file_get_contents($f);  file_put_contents($f, $data);
来源：http://zov.shanyushiyangkeji.top

[U64] PHP：目录遍历
来源：http://nrk.cqqwz.cn

glob("dir/*.php");  scandir("dir");
来源：http://wtf.yanxiufei.cn

[U65] PHP：会话
来源：http://yhp.havefunace.top

session_start();  $_SESSION["uid"] = 1;
来源：http://uev.xuetiantiany.cn

[U66] PHP：设置 Cookie
来源：http://sxa.jqgufenzy.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://kur.sufxvd.cn

[U67] PHP：处理文件上传
来源：http://rme.chenjidiqi.icu

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://ecv.316326.xyz

[U68] PHP：PDO 连接
来源：http://rtg.gaohongyu789.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://bom.jqgfzy.top

[U69] PHP：PDO 预处理
来源：http://ugl.fanxiaobao.xyz

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://qnj.mhx1999.top

[U70] PHP：PDO 事务
来源：http://gps.daxiang520.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://cmv.xuetiantiany.cn

[U71] PHP：抛出异常
来源：http://aeq.nwbrower.top

throw new RuntimeException("失败", 500);
来源：http://fun.guowangkeji.top

[U72] PHP：写错误日志
来源：http://bpg.nwbrower.top

error_log("失败: " . $e->getMessage());
来源：http://kdw.zhongyouzk.top

[U73] PHP：读取 ini 配置
来源：http://azi.ctjpmb.com

parse_ini_file("config.ini", true)
来源：http://uaj.tanke756.top

[U74] PHP：读取环境变量
来源：http://atb.jlsjyb.cn

getenv("APP_ENV") ?: "production"
来源：http://wbq.tian-w.cn

[U75] PHP：依赖注入
来源：http://frw.zhijiandao.cn

composer require psr/container
来源：http://kjg.sjlbkw.cn

[U76] PHP：简单路由
来源：http://zky.316326.xyz

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://aep.ywan-chungtsiang.top

[U77] PHP：模板渲染
来源：http://cbt.xuetiantiany.cn

composer require twig/twig
来源：http://ntl.ivvv.top

[U78] PHP：单元测试
来源：http://miz.yueranfly.top

composer require --dev phpunit/phpunit
来源：http://ftd.redwolf501.top

[U79] PHP：静态分析
来源：http://kqo.shzxlz.cn

composer require --dev phpstan/phpstan
来源：http://ulc.jqgfzy.top

[U80] PHP：代码规范修复
来源：http://wii.ywan-chungtsiang.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://bsd.hnqzz.top

[U81] JS：初始化项目
来源：http://rjm.jlsjyb.cn

npm init -y;  npm i express
来源：http://kmi.yanxiufei.cn

[U82] JS：package.json 脚本
来源：http://zcq.bbcook.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://jll.zdbjq.cn

[U83] JS：ES Module 导入导出
来源：http://rna.ybcxt.top

export const a = 1;  import { a } from "./m.js";
来源：http://pjk.shanyushiyangkeji.top

[U84] JS：CommonJS 写法
来源：http://eye.jinghuilouyu.cn

module.exports = { a };  const { a } = require("./m");
来源：http://szp.wangdashe.top

[U85] JS：可选链
来源：http://ajl.pengpengdd.cyou

a?.b?.c
来源：http://mtn.sysykeji.top

[U86] JS：空值合并
来源：http://cuu.snrcjt.cn

a ?? b
来源：http://ftw.tian-w.cn

[U87] JS：解构默认值
来源：http://brx.svipenyu.cn

const { a = 1, b = 2 } = obj;
来源：http://wzx.pengpengdd.cyou

[U88] JS：对象展开合并
来源：http://cwi.yanxiufei.cn

{ ...a, ...b }
来源：http://hqr.hfpthk.cn

[U89] JS：数组去重
来源：http://otw.tian-w.cn

[...new Set(arr)]
来源：http://csb.mhx1999.top

[U90] JS：数字数组排序
来源：http://dgi.svipenyu.cn

[...arr].sort((a, b) => a - b)
来源：http://drv.bjfxy.top

[U91] JS：对象键值遍历
来源：http://tdo.yanxiufei.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://xll.guowangkeji.top

[U92] JS：深拷贝
来源：http://zsl.fehbvm.com

structuredClone(obj)
来源：http://uvy.shanyushiyangkeji.top

[U93] JS：模板字符串
来源：http://uqa.zhijiandao.cn

`共 ${n} 条`
来源：http://zwn.yj20258.top

[U94] JS：箭头函数
来源：http://lil.sweek.top

const double = x => x * 2;
来源：http://kmb.epnwcf.com

[U95] JS：Promise 包装
来源：http://oxg.jinghuilouyu.cn

new Promise((resolve, reject) => {})
来源：http://dla.xuanzx.com

[U96] JS：async/await 与异常
来源：http://oua.0kj1m.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://cgk.snrcjt.cn

[U97] JS：并发请求
来源：http://ljm.zhongyouzk.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://cie.hongshengwenyu.top

[U98] JS：fetch 带 JSON
来源：http://wtq.sufxvd.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://ghh.hesvh.cn

[U99] JS：事件监听
来源：http://xil.mhx1999.top

el.addEventListener("click", e => {})
来源：http://nsu.yongpay.top

[U100] JS：DOM 查询
来源：http://nhi.yvedp.cn

document.querySelector(".item")
来源：http://tad.c1oappe.top

[U101] JS：classList 操作
来源：http://epz.jqgfzy.top

el.classList.toggle("active")
来源：http://kgw.uphjek.com

[U102] JS：本地存储
来源：http://dri.jlsjyb.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://upp.zhaomingkeji.xyz

[U103] JS：定时器
来源：http://asr.0kj1m.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://ari.gaohongyu789.top

[U104] JS：防抖
来源：http://poi.fanxiaobao.xyz

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mlc.zhaomingkeji.xyz

[U105] JS：节流
来源：http://evi.cashguo.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://dsh.bbcook.cn

[U106] JS：日期格式化
来源：http://uuw.yongpay.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://nac.nwbrower.top

[U107] JS：数字千分位
来源：http://kdn.hywenlv.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://bhy.yuxming.cn

[U108] JS：随机整数
来源：http://zhn.yuanzhike.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://nhr.hysaishi.cn

[U109] JS：数组分组
来源：http://uqw.yuanzhike.top

Object.groupBy(arr, x => x.type)
来源：http://cjd.jyoumei.cn

[U110] JS：数组分块
来源：http://zkb.yj202588.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://jdb.cdnleiting.top

[U111] JS：对象转 Map
来源：http://xcz.tianlin.xyz

new Map(Object.entries(obj))
来源：http://wfh.pycfn.com

[U112] JS：字符串补位
来源：http://wja.yuanzhike.top

"7".padStart(3, "0")
来源：http://pec.c1oappe.top

[U113] JS：正则替换全部
来源：http://njj.yvedp.cn

s.replaceAll("a", "b")
来源：http://vsc.nwbrower.top

[U114] JS：JSON 深比较
来源：http://rwg.hysaishi.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://vty.ydzc1.top

[U115] JS：生成 UUID
来源：http://bsk.daxiang520.top

crypto.randomUUID()
来源：http://wsi.hesvh.cn

[U116] JS：类型检查（JSDoc）
来源：http://ecy.gzhubu.top

/** @param {string} name */ function f(name) {}
来源：http://uvt.xuanzx.com

[U117] JS：单元测试
来源：http://qzc.shangyingyoupin.top

npm i -D vitest;  npx vitest
来源：http://sve.hongshengwenyu.top

[U118] JS：开发服务器
来源：http://jpn.yonumen.top

npm i -D vite;  npx vite
来源：http://bov.zhijiandao.cn

[U119] JS：生产构建
来源：http://and.fengsongda.top

npx vite build
来源：http://zeo.wangdashe.top

[U120] JS：读取环境变量（Vite）
来源：http://abf.jqgufenzy.top

import.meta.env.VITE_API_URL
来源：http://rvv.gogol.net.cn

================================================================================
来源：http://uzl.jqgfzy.top

统计汇总
来源：http://suo.sweek.top

================================================================================
来源：http://ioy.ybcxt.top

按语言统计（条）：
来源：http://vxj.zdbjq.cn

Python ......... 252
来源：http://qpx.52xcode.cn

PHP ............ 252
来源：http://mgc.zhoulong.xyz

JavaScript ..... 252
来源：http://wyx.jiagoushi.top

TypeScript ..... 212
来源：http://dwp.hcnkem.com

Java ........... 212
来源：http://aso.cucudq.cn

Go ............. 212
来源：http://eqs.iojbl.cn

Ruby ........... 212
来源：http://uie.hysaishi.cn

C# ............. 212
来源：http://nnf.aizwys.cn

C .............. 30
来源：http://nwr.shzxlz.cn

C++ ............ 30
来源：http://hsm.cheryme.top

SQL ............ 90
来源：http://uyz.yanxiufei.cn

Bash ........... 80
来源：http://qup.cheryme.top

Kotlin ......... 15
来源：http://zyv.zhiwuduotai.top

Swift .......... 15
来源：http://xsy.wangdashe.top

Lua ............ 10
来源：http://bqi.nwbrower.top

Perl ........... 10
来源：http://fel.ydjk.org.cn

Scala .......... 10
来源：http://qgj.ehwqpu.com

------------------------------------
来源：http://sis.jqgufenzy.top

合计 ........... 2106 条
来源：http://tca.9152youxi.cn

按章节统计：
来源：http://ogu.quarkkingdee.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://bjw.tian-w.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://jwt.ppjwa.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://riv.cheryme.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://fic.hesvh.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://wie.zdqjudy.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://rbe.sufxvd.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://kpf.jyoumei.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://mfl.shuidangran.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://unl.pycfn.com

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://gnw.havefunace.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hhk.zhoulong.xyz

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://yfy.jinqigufen.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://nyv.ydzc1.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://bab.guowangkeji.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://uls.cdnleiting.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://zwv.ybcxt.top

Q SQL 专题                              90
来源：http://kol.zdbjq.cn

R Bash 专题                             80
来源：http://okx.hysaishi.cn

S C / C++ 专题                          60
来源：http://orb.hnxiangtu.top

T 其他语言补充                          60
来源：http://awu.epnwcf.com

U 高频实用片段                         120
来源：http://fby.smart0.xyz

------------------------------------
来源：http://idi.52xcode.cn

合计                                  2106 条
来源：http://hur.ydjk.org.cn

--------------------------------------------------------------------------------
来源：http://lug.xuanzx.com

使用提醒
来源：http://mjm.xinyue.icu

--------------------------------------------------------------------------------
来源：http://emw.fengsongda.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://fqr.ppjwa.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://psg.hesvh.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://vst.zhongyouzk.top

在旧版本上使用前请先确认语法支持情况。
来源：http://sge.daxiang520.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://ezg.pengpengdd.cyou

—— 文件结束 ——
来源：http://wiy.yanxiufei.cn

================================================================================
来源：http://nfg.fanxiaobao.xyz

程序语言常见例子速查手册（2024 版）
来源：http://pmu.bbcook.cn

Common Programming Examples Cheat Book
来源：http://tbw.sxryk.cn

================================================================================
来源：http://cer.kuanghao11.cn

【收录内容】
来源：http://ylf.dianchejie.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://kyz.vqdsnc.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://rcg.gotoacloud.top

SQL · Bash · C · C++
来源：http://iis.hnxiangtu.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://ayw.hnxiangtu.top

【使用说明】
来源：http://pwk.cucudq.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://ohq.sjlbkw.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://jci.zhijiandao.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://xaj.ydzc1.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://hqa.jyoumei.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://aqp.hfpthk.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://sfd.zycfv.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://nif.fanxiaobao.xyz

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://bzu.ydjk.org.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://bcn.zhiwuduotai.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://qad.daxiang520.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://liq.pycfn.com

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://zfw.yuanzhike.top

【文件统计】
来源：http://fkb.bbcook.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://fqd.nanxinkj.top

--------------------------------------------------------------------------------
来源：http://zlz.quarkkingdee.top

目  录
来源：http://yon.meibo888.top

--------------------------------------------------------------------------------
来源：http://bel.xziqi.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://qmn.sweek.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://nyl.gogol.net.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://xsf.shangyingyoupin.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://jhd.birdmap.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://meo.quarkkingdee.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://ifw.ybcxt.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://tjw.svipenyu.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://ufo.ydzc1.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://trv.xuetiantiany.cn


<!-- 参考信息 -->