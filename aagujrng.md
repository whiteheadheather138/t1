代发 wailian999

[U15] Py：高精度计时
来源：http://txy.jqgufenzy.top

t = time.perf_counter()
来源：http://qaj.zdqjudy.top

[U16] Py：命令行参数解析
来源：http://tfh.sysykeji.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://ugi.ybcxt.top

[U17] Py：初始化日志
来源：http://den.zhengqikj.top

logging.basicConfig(level=logging.INFO)
来源：http://htz.wangdashe.top

[U18] Py：预编译正则
来源：http://swd.vqdsnc.cn

pat = re.compile(r"\d+")
来源：http://lcz.guannengcc.top

[U19] Py：正则替换带回调
来源：http://dje.jqgfzy.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://oib.fengsongda.top

[U20] Py：缓存函数结果
来源：http://wdp.jlsjyb.cn

@functools.lru_cache(maxsize=None)
来源：http://vba.jianghu66.top

[U21] Py：自定义上下文管理器
来源：http://tsj.fengsongda.top

@contextlib.contextmanager
来源：http://saa.fanxiaobao.xyz

[U22] Py：矩阵转置
来源：http://bfa.zhoulong.xyz

list(zip(*m))
来源：http://yuw.wangshuangyany.cn

[U23] Py：分块读取大文件
来源：http://kzq.yj20258.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://izg.bjfxy.top

[U24] Py：路径操作
来源：http://lhp.hongshengwenyu.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://ndd.zdbjq.cn

[U25] Py：CSV 按字典读
来源：http://vbs.ppjwa.cn

csv.DictReader(f)
来源：http://gcm.hywenlv.cn

[U26] Py：并发下载
来源：http://vge.zdbjq.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://reg.xylfe.cn

[U27] Py：异步 HTTP
来源：http://qtl.gogol.net.cn

aiohttp.ClientSession() 配合 async with
来源：http://bcb.c1oappe.top

[U28] Py：类型别名
来源：http://nmt.chenlongwang.top

UserId = int
来源：http://stg.zhengqikj.top

[U29] Py：属性校验
来源：http://xft.9152youxi.cn

@property 与 @x.setter 配合
来源：http://cyp.pycfn.com

[U30] Py：数据类
来源：http://sgw.xinyue.icu

@dataclass(slots=True)
来源：http://zsj.ppjwa.cn

[U31] Py：单测
来源：http://irf.xylfe.cn

python -m pytest -q
来源：http://kua.dashuyun.cn

[U32] Py：代码格式化
来源：http://hxz.birdmap.top

ruff format . && ruff check --fix .
来源：http://oqv.uphjek.com

[U33] Py：打包发布
来源：http://ayk.zycfv.cn

python -m build  （依赖 pyproject.toml）
来源：http://pze.chenzaomai.com

[U34] Py：判断编码
来源：http://fif.chenjidiqi.icu

chardet.detect(raw)
来源：http://pgf.cucudq.cn

[U35] Py：发送邮件
来源：http://qxm.nanxinkj.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://rht.jqgufenzy.top

[U36] Py：定时任务
来源：http://vwd.yfazqb.com

schedule.every(10).minutes.do(job)
来源：http://dts.aibaodan.cn

[U37] Py：读写 Excel
来源：http://kgz.ehwqpu.com

pandas.read_excel / DataFrame.to_excel
来源：http://pha.yangfankeji.com

[U38] Py：获取脚本所在目录
来源：http://boe.zhiwuduotai.top

Path(__file__).resolve().parent
来源：http://ejo.sysykeji.top

[U39] Py：判断是否在交互环境
来源：http://lew.fktsv.cn

sys.stdout.isatty()
来源：http://uvb.hywenlv.cn

[U40] Py：打印到标准错误
来源：http://xph.hysaishi.cn

print("err", file=sys.stderr)
来源：http://fdj.zdqjudy.top

[U41] PHP：初始化 Composer 项目
来源：http://iiu.yuanzhike.top

composer init;  composer require guzzlehttp/guzzle
来源：http://qgj.fanxiaobao.xyz

[U42] PHP：PSR-4 自动加载
来源：http://ysx.zhijiandao.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://ebv.vehdjk.com

[U43] PHP：声明命名空间
来源：http://btk.zhongyouzk.top

namespace App\Http;
来源：http://rsl.snrcjt.cn

[U44] PHP：开启严格类型
来源：http://ybg.sjlbkw.cn

declare(strict_types=1);
来源：http://hhd.andypj.xyz

[U45] PHP：类型声明与返回类型
来源：http://qff.gotoacloud.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://gfn.jqgufenzy.top

[U46] PHP：可空类型
来源：http://hbj.shanyushiyangkeji.top

?string $name = null
来源：http://dbe.pycfn.com

[U47] PHP：联合类型
来源：http://roc.sufxvd.cn

int|string $id
来源：http://qeu.hysaishi.cn

[U48] PHP：纯枚举
来源：http://jbn.fktsv.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://vov.yanxiufei.cn

[U49] PHP：只读属性
来源：http://aft.shzxlz.cn

public readonly string $name
来源：http://end.ppjwa.cn

[U50] PHP：构造器属性提升
来源：http://bra.sysykeji.top

public function __construct(private int $id) {}
来源：http://dnp.shangyingyoupin.top

[U51] PHP：数组解构
来源：http://loq.hammf.cn

[$a, $b] = $arr;
来源：http://cdy.hysaishi.cn

[U52] PHP：箭头函数
来源：http://wls.quarkkingdee.top

$double = fn($x) => $x * 2;
来源：http://txo.yfazqb.com

[U53] PHP：空合并运算符
来源：http://lyb.jqgufenzy.top

$v = $a ?? $b ?? "default";
来源：http://asb.xuetiantiany.cn

[U54] PHP：空安全调用
来源：http://jgj.xuanzx.com

$obj?->method()
来源：http://qmz.jlsjyb.cn

[U55] PHP：match 表达式
来源：http://jfb.cheryme.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://wvf.quarkkingdee.top

[U56] PHP：命名参数
来源：http://opi.yj20258888.top

f(a: 1, b: 2)
来源：http://qba.chenjidiqi.icu

[U57] PHP：字符串插值
来源：http://qra.chenzaomai.com

"值: {$a}"
来源：http://npe.shzxlz.cn

[U58] PHP：数组三件套
来源：http://exa.iojbl.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://sgy.aibaodan.cn

[U59] PHP：自定义排序
来源：http://amu.zhoulong.xyz

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mlu.c1oappe.top

[U60] PHP：JSON 编解码
来源：http://hso.sweek.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://ser.zdqjudy.top

[U61] PHP：正则
来源：http://uho.zdbjq.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://pcg.gzhubu.top

[U62] PHP：日期对象
来源：http://wye.cheryme.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://axk.jinqigufen.top

[U63] PHP：文件读写
来源：http://jci.hesvh.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://zfz.xuetiantiany.cn

[U64] PHP：目录遍历
来源：http://hbf.havefunace.top

glob("dir/*.php");  scandir("dir");
来源：http://hls.chenlongwang.top

[U65] PHP：会话
来源：http://mge.pycfn.com

session_start();  $_SESSION["uid"] = 1;
来源：http://gzi.ywan-chungtsiang.top

[U66] PHP：设置 Cookie
来源：http://qae.xuetiantiany.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://rgg.pengpengdd.cyou

[U67] PHP：处理文件上传
来源：http://whr.birdmap.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://eou.jyoumei.cn

[U68] PHP：PDO 连接
来源：http://dot.guowangkeji.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://csz.vqdsnc.cn

[U69] PHP：PDO 预处理
来源：http://cek.zhiwuduotai.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://dzp.pycfn.com

[U70] PHP：PDO 事务
来源：http://hwb.yvedp.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://vsi.uphjek.com

[U71] PHP：抛出异常
来源：http://kzf.0kj1m.cn

throw new RuntimeException("失败", 500);
来源：http://ybz.wangdashe.top

[U72] PHP：写错误日志
来源：http://rzw.snrcjt.cn

error_log("失败: " . $e->getMessage());
来源：http://jkr.haohaochexian.top

[U73] PHP：读取 ini 配置
来源：http://rtp.hnxiangtu.top

parse_ini_file("config.ini", true)
来源：http://lrv.birdmap.top

[U74] PHP：读取环境变量
来源：http://pwx.wangshuangyany.cn

getenv("APP_ENV") ?: "production"
来源：http://ogo.nwbrower.top

[U75] PHP：依赖注入
来源：http://wim.vehdjk.com

composer require psr/container
来源：http://agk.yj20258888.top

[U76] PHP：简单路由
来源：http://oth.hnxiangtu.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://ytn.tarul.cn

[U77] PHP：模板渲染
来源：http://mqx.yj20258.top

composer require twig/twig
来源：http://ndi.vehdjk.com

[U78] PHP：单元测试
来源：http://yyy.shzxlz.cn

composer require --dev phpunit/phpunit
来源：http://rjt.ydjk.org.cn

[U79] PHP：静态分析
来源：http://jiu.guannengcc.top

composer require --dev phpstan/phpstan
来源：http://ghf.hnxiangtu.top

[U80] PHP：代码规范修复
来源：http://avu.cheryme.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://pim.52xcode.cn

[U81] JS：初始化项目
来源：http://pxm.jianghu66.top

npm init -y;  npm i express
来源：http://elz.c1oappe.top

[U82] JS：package.json 脚本
来源：http://cif.snrcjt.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://aoh.chenjidiqi.icu

[U83] JS：ES Module 导入导出
来源：http://ypl.fanxiaobao.xyz

export const a = 1;  import { a } from "./m.js";
来源：http://jix.yj20258888.top

[U84] JS：CommonJS 写法
来源：http://roq.cdnleiting.top

module.exports = { a };  const { a } = require("./m");
来源：http://xvv.zhiwuduotai.top

[U85] JS：可选链
来源：http://ama.dashuyun.cn

a?.b?.c
来源：http://dbm.dianchejie.cn

[U86] JS：空值合并
来源：http://esh.xinyue.icu

a ?? b
来源：http://oju.aibaodan.cn

[U87] JS：解构默认值
来源：http://iur.wangdashe.top

const { a = 1, b = 2 } = obj;
来源：http://xgd.hnxiangtu.top

[U88] JS：对象展开合并
来源：http://xvm.cucudq.cn

{ ...a, ...b }
来源：http://aci.chenzaomai.com

[U89] JS：数组去重
来源：http://oyx.jinyuanbaomall.cn

[...new Set(arr)]
来源：http://yxv.zdbjq.cn

[U90] JS：数字数组排序
来源：http://sct.xuanzx.com

[...arr].sort((a, b) => a - b)
来源：http://feg.feifeiyinyue.top

[U91] JS：对象键值遍历
来源：http://nnk.sxryk.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://rck.dashuyun.cn

[U92] JS：深拷贝
来源：http://cqg.vehdjk.com

structuredClone(obj)
来源：http://aef.hnqzz.top

[U93] JS：模板字符串
来源：http://dwl.52xcode.cn

`共 ${n} 条`
来源：http://mhl.52xcode.cn

[U94] JS：箭头函数
来源：http://jzc.quarkkingdee.top

const double = x => x * 2;
来源：http://cod.jinyuanbaomall.cn

[U95] JS：Promise 包装
来源：http://dnz.yueranfly.top

new Promise((resolve, reject) => {})
来源：http://mfo.guowangkeji.top

[U96] JS：async/await 与异常
来源：http://klf.yonumen.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://jbt.cdnleiting.top

[U97] JS：并发请求
来源：http://fnz.sweek.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://lwi.tanke756.top

[U98] JS：fetch 带 JSON
来源：http://ito.cashguo.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://bza.sysykeji.top

[U99] JS：事件监听
来源：http://yyr.iojbl.cn

el.addEventListener("click", e => {})
来源：http://kui.jinqigfzy.top

[U100] JS：DOM 查询
来源：http://gqx.birdmap.top

document.querySelector(".item")
来源：http://ttb.cqqwz.cn

[U101] JS：classList 操作
来源：http://ldm.mhx1999.top

el.classList.toggle("active")
来源：http://nbb.fengsongda.top

[U102] JS：本地存储
来源：http://qgg.yueranfly.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://ysw.jyoumei.cn

[U103] JS：定时器
来源：http://tbp.zhengqikj.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://lvf.pycfn.com

[U104] JS：防抖
来源：http://umj.yj20258888.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://fyf.mhx1999.top

[U105] JS：节流
来源：http://ung.fzhhl.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://qfd.ivvv.top

[U106] JS：日期格式化
来源：http://doe.yj20258888.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://nlr.chenjidiqi.icu

[U107] JS：数字千分位
来源：http://los.yanxiufei.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://wxs.ehwqpu.com

[U108] JS：随机整数
来源：http://iis.gaohongyu789.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://fiz.cdnleiting.top

[U109] JS：数组分组
来源：http://xlv.havefunace.top

Object.groupBy(arr, x => x.type)
来源：http://pot.yanxiufei.cn

[U110] JS：数组分块
来源：http://lkj.hnqzz.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://vhz.fktsv.cn

[U111] JS：对象转 Map
来源：http://daf.jyoumei.cn

new Map(Object.entries(obj))
来源：http://lga.yueranfly.top

[U112] JS：字符串补位
来源：http://vda.andypj.xyz

"7".padStart(3, "0")
来源：http://ode.vqdsnc.cn

[U113] JS：正则替换全部
来源：http://bsy.cqqwz.cn

s.replaceAll("a", "b")
来源：http://acf.xylfe.cn

[U114] JS：JSON 深比较
来源：http://tge.iojbl.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://sqn.yj20258888.top

[U115] JS：生成 UUID
来源：http://hfk.cheryme.top

crypto.randomUUID()
来源：http://qsv.gogol.net.cn

[U116] JS：类型检查（JSDoc）
来源：http://jfw.c1oappe.top

/** @param {string} name */ function f(name) {}
来源：http://wxn.vqdsnc.cn

[U117] JS：单元测试
来源：http://djp.cucudq.cn

npm i -D vitest;  npx vitest
来源：http://qqb.52xcode.cn

[U118] JS：开发服务器
来源：http://nsf.cashguo.top

npm i -D vite;  npx vite
来源：http://acz.pycfn.com

[U119] JS：生产构建
来源：http://wge.yj20258888.top

npx vite build
来源：http://dlt.vqdsnc.cn

[U120] JS：读取环境变量（Vite）
来源：http://dxu.zhengqikj.top

import.meta.env.VITE_API_URL
来源：http://npy.nanxinkj.top

================================================================================
来源：http://ouh.ydzc1.top

统计汇总
来源：http://tol.yfazqb.com

================================================================================
来源：http://gmj.zhijiandao.cn

按语言统计（条）：
来源：http://omp.ppjwa.cn

Python ......... 252
来源：http://icl.ydzc1.top

PHP ............ 252
来源：http://yxw.yueranfly.top

JavaScript ..... 252
来源：http://bmj.zdqjudy.top

TypeScript ..... 212
来源：http://lqh.yj20258.top

Java ........... 212
来源：http://jhf.quarkkingdee.top

Go ............. 212
来源：http://wst.316326.xyz

Ruby ........... 212
来源：http://jhv.yangfankeji.com

C# ............. 212
来源：http://nfw.haohaochexian.top

C .............. 30
来源：http://vpp.chenlongwang.top

C++ ............ 30
来源：http://cao.shangyingyoupin.top

SQL ............ 90
来源：http://rpx.jlsjyb.cn

Bash ........... 80
来源：http://ade.nanxinkj.top

Kotlin ......... 15
来源：http://bxc.aizwys.cn

Swift .......... 15
来源：http://bhs.quarkkingdee.top

Lua ............ 10
来源：http://tcq.mhx1999.top

Perl ........... 10
来源：http://set.zhoulong.xyz

Scala .......... 10
来源：http://wqi.zdqjudy.top

------------------------------------
来源：http://tnh.52xcode.cn

合计 ........... 2106 条
来源：http://mrt.fengsongda.top

按章节统计：
来源：http://cnw.hesvh.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://srs.aibaodan.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://eow.sjlbkw.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://aqt.snrcjt.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://opt.snrcjt.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://ryk.zhoulong.xyz

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://kix.yongpay.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hwn.meibo888.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://thn.zhixingplan.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://tyb.xuetiantiany.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://pll.ydjk.org.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://sqh.yuanzhike.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://mji.shangyingyoupin.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://omw.tianlin.xyz

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://eul.vehdjk.com

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://ztx.chenzaomai.com

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://ttk.jiagoushi.top

Q SQL 专题                              90
来源：http://gmm.shzxlz.cn

R Bash 专题                             80
来源：http://roz.sjlbkw.cn

S C / C++ 专题                          60
来源：http://cuv.ydjk.org.cn

T 其他语言补充                          60
来源：http://tqv.uphjek.com

U 高频实用片段                         120
来源：http://bnz.sjlbkw.cn

------------------------------------
来源：http://dns.zdqjudy.top

合计                                  2106 条
来源：http://zmc.jinqigfzy.top

--------------------------------------------------------------------------------
来源：http://fmh.yangfankeji.com

使用提醒
来源：http://mrf.xziqi.cn

--------------------------------------------------------------------------------
来源：http://dqa.pengpengdd.cyou

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://qdc.bbcook.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://avm.c1oappe.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://ncz.zhaomingkeji.xyz

在旧版本上使用前请先确认语法支持情况。
来源：http://mlp.bjfxy.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://qxe.316326.xyz

—— 文件结束 ——
来源：http://nac.zhongyouzk.top

================================================================================
来源：http://vsh.epnwcf.com

程序语言常见例子速查手册（2024 版）
来源：http://djg.0kj1m.cn

Common Programming Examples Cheat Book
来源：http://srb.shanyushiyangtech.top

================================================================================
来源：http://zfa.vqdsnc.cn

【收录内容】
来源：http://ddl.gzhubu.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://sjf.shuidangran.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://srt.zhiwuduotai.top

SQL · Bash · C · C++
来源：http://ymh.chenzaomai.com

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://iuw.jianghu66.top

【使用说明】
来源：http://ccd.meibo888.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://yff.sweek.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://mne.gotoacloud.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://ydx.cucudq.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://tmp.guowangkeji.top

Bash:  Shell         C:     C             C++:   C++
来源：http://kmj.yangfankeji.com

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://bjl.sjlbkw.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://jhb.9152youxi.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://yvw.cashguo.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://wiu.c1oappe.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://cke.hcnkem.com

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://hoi.nanxuanxn.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://ufy.pycfn.com

【文件统计】
来源：http://ilm.fzhhl.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://gmb.ehwqpu.com

--------------------------------------------------------------------------------
来源：http://ktx.zhaomingkeji.xyz

目  录
来源：http://cvb.gotoacloud.top

--------------------------------------------------------------------------------
来源：http://qys.yfazqb.com

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://ron.xylfe.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://kqt.nwbrower.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://hzu.fanxiaobao.xyz

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://cjy.vqdsnc.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://swb.nwbrower.top


<!-- 参考信息 -->