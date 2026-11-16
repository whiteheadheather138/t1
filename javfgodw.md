代发 wailian999

[U15] Py：高精度计时
来源：http://xzy.xziqi.cn

t = time.perf_counter()
来源：http://knb.sufxvd.cn

[U16] Py：命令行参数解析
来源：http://ege.nanxuanxn.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://chm.epnwcf.com

[U17] Py：初始化日志
来源：http://zlk.cqqwz.cn

logging.basicConfig(level=logging.INFO)
来源：http://zfu.aizwys.cn

[U18] Py：预编译正则
来源：http://wqx.jianghu66.top

pat = re.compile(r"\d+")
来源：http://evk.nwbrower.top

[U19] Py：正则替换带回调
来源：http://eat.fanxiaobao.xyz

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://awt.zhaomingkeji.xyz

[U20] Py：缓存函数结果
来源：http://jjq.zdbjq.cn

@functools.lru_cache(maxsize=None)
来源：http://tjs.hongshengwenyu.top

[U21] Py：自定义上下文管理器
来源：http://kpv.tianlin.xyz

@contextlib.contextmanager
来源：http://fmc.tianlin.xyz

[U22] Py：矩阵转置
来源：http://iui.andypj.xyz

list(zip(*m))
来源：http://rnk.snrcjt.cn

[U23] Py：分块读取大文件
来源：http://yso.smart0.xyz

for chunk in iter(lambda: f.read(8192), b""):
来源：http://fab.meibo888.top

[U24] Py：路径操作
来源：http://xui.0kj1m.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://cww.tianlin.xyz

[U25] Py：CSV 按字典读
来源：http://jqy.9152youxi.cn

csv.DictReader(f)
来源：http://whl.yangfankeji.com

[U26] Py：并发下载
来源：http://bsg.jinqigfzy.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://mim.guowangkeji.top

[U27] Py：异步 HTTP
来源：http://hlp.cucudq.cn

aiohttp.ClientSession() 配合 async with
来源：http://ybd.aizwys.cn

[U28] Py：类型别名
来源：http://wpn.yvedp.cn

UserId = int
来源：http://hul.yj202588.top

[U29] Py：属性校验
来源：http://pmg.xziqi.cn

@property 与 @x.setter 配合
来源：http://yag.ctjpmb.com

[U30] Py：数据类
来源：http://giz.316326.xyz

@dataclass(slots=True)
来源：http://giu.tianlin.xyz

[U31] Py：单测
来源：http://djh.guowangkeji.top

python -m pytest -q
来源：http://tmc.xingfuxueyuan.xyz

[U32] Py：代码格式化
来源：http://dbh.redwolf501.top

ruff format . && ruff check --fix .
来源：http://gue.wangshuangyany.cn

[U33] Py：打包发布
来源：http://xsq.zhengqikj.top

python -m build  （依赖 pyproject.toml）
来源：http://dee.bbcook.cn

[U34] Py：判断编码
来源：http://uic.xziqi.cn

chardet.detect(raw)
来源：http://hjc.ivvv.top

[U35] Py：发送邮件
来源：http://vuf.shanyushiyangtech.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://qgd.fktsv.cn

[U36] Py：定时任务
来源：http://mia.ivvv.top

schedule.every(10).minutes.do(job)
来源：http://tfw.hongshengwenyu.top

[U37] Py：读写 Excel
来源：http://jdb.snrcjt.cn

pandas.read_excel / DataFrame.to_excel
来源：http://jly.yj202588.top

[U38] Py：获取脚本所在目录
来源：http://dkz.jianghu66.top

Path(__file__).resolve().parent
来源：http://lko.chenlongwang.top

[U39] Py：判断是否在交互环境
来源：http://oov.xziqi.cn

sys.stdout.isatty()
来源：http://iop.snrcjt.cn

[U40] Py：打印到标准错误
来源：http://yuu.gzhubu.top

print("err", file=sys.stderr)
来源：http://nyh.sysykeji.top

[U41] PHP：初始化 Composer 项目
来源：http://pki.c1oappe.top

composer init;  composer require guzzlehttp/guzzle
来源：http://piq.yj20258888.top

[U42] PHP：PSR-4 自动加载
来源：http://ghu.sjlbkw.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://rea.xingfuxueyuan.xyz

[U43] PHP：声明命名空间
来源：http://wft.xylfe.cn

namespace App\Http;
来源：http://sit.nwbrower.top

[U44] PHP：开启严格类型
来源：http://gct.xziqi.cn

declare(strict_types=1);
来源：http://keb.pengpengdd.cyou

[U45] PHP：类型声明与返回类型
来源：http://lvq.yuxming.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://bvq.hnqzz.top

[U46] PHP：可空类型
来源：http://cwd.sysykeji.top

?string $name = null
来源：http://fsh.shanyushiyangkeji.top

[U47] PHP：联合类型
来源：http://kgq.bjfxy.top

int|string $id
来源：http://ijg.nanxinkj.top

[U48] PHP：纯枚举
来源：http://aoy.iojbl.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://znr.hysaishi.cn

[U49] PHP：只读属性
来源：http://qon.ydzc1.top

public readonly string $name
来源：http://uui.zhoulong.xyz

[U50] PHP：构造器属性提升
来源：http://mko.andypj.xyz

public function __construct(private int $id) {}
来源：http://hur.chenzaomai.com

[U51] PHP：数组解构
来源：http://gsp.zhiwuduotai.top

[$a, $b] = $arr;
来源：http://zhd.andypj.xyz

[U52] PHP：箭头函数
来源：http://osw.smart0.xyz

$double = fn($x) => $x * 2;
来源：http://klj.sysykeji.top

[U53] PHP：空合并运算符
来源：http://ckj.yj20258888.top

$v = $a ?? $b ?? "default";
来源：http://bzj.fengsongda.top

[U54] PHP：空安全调用
来源：http://qlz.daria6918.cn

$obj?->method()
来源：http://qqk.nanxinkj.top

[U55] PHP：match 表达式
来源：http://vtv.c1oappe.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://rnw.c1oappe.top

[U56] PHP：命名参数
来源：http://lvb.pengpengdd.cyou

f(a: 1, b: 2)
来源：http://byx.fzhhl.top

[U57] PHP：字符串插值
来源：http://vpq.ctjpmb.com

"值: {$a}"
来源：http://bbp.tianlin.xyz

[U58] PHP：数组三件套
来源：http://mtp.yj20258.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://oan.wangshuangyany.cn

[U59] PHP：自定义排序
来源：http://env.cqqwz.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://bxd.fehbvm.com

[U60] PHP：JSON 编解码
来源：http://plx.aibaodan.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://fcc.hcnkem.com

[U61] PHP：正则
来源：http://yrt.shzxlz.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://jua.xinyue.icu

[U62] PHP：日期对象
来源：http://bso.yuxming.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://bnq.nanxinkj.top

[U63] PHP：文件读写
来源：http://bfd.dashuyun.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://rlr.sjlbkw.cn

[U64] PHP：目录遍历
来源：http://jfi.c1oappe.top

glob("dir/*.php");  scandir("dir");
来源：http://isj.shanyushiyangtech.top

[U65] PHP：会话
来源：http://lck.chenlongwang.top

session_start();  $_SESSION["uid"] = 1;
来源：http://cnt.jinqigfzy.top

[U66] PHP：设置 Cookie
来源：http://ama.chenjidiqi.icu

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://txb.ybcxt.top

[U67] PHP：处理文件上传
来源：http://wpe.guannengcc.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://vcc.nanxuanxn.top

[U68] PHP：PDO 连接
来源：http://vnp.svipenyu.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://qlq.yuanzhike.top

[U69] PHP：PDO 预处理
来源：http://zvy.gogol.net.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://don.bjfxy.top

[U70] PHP：PDO 事务
来源：http://xrp.0kj1m.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://gqr.svipenyu.cn

[U71] PHP：抛出异常
来源：http://kaj.yj202588.top

throw new RuntimeException("失败", 500);
来源：http://qhr.ivvv.top

[U72] PHP：写错误日志
来源：http://cyh.yfazqb.com

error_log("失败: " . $e->getMessage());
来源：http://pms.chenjidiqi.icu

[U73] PHP：读取 ini 配置
来源：http://zgd.haohaochexian.top

parse_ini_file("config.ini", true)
来源：http://mhu.nwbrower.top

[U74] PHP：读取环境变量
来源：http://jwn.ehwqpu.com

getenv("APP_ENV") ?: "production"
来源：http://yyd.shuidangran.top

[U75] PHP：依赖注入
来源：http://zis.quarkkingdee.top

composer require psr/container
来源：http://wny.hcnkem.com

[U76] PHP：简单路由
来源：http://lzl.daxiang520.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://vsb.zhijiandao.cn

[U77] PHP：模板渲染
来源：http://owa.andypj.xyz

composer require twig/twig
来源：http://gol.hnxiangtu.top

[U78] PHP：单元测试
来源：http://tau.uphjek.com

composer require --dev phpunit/phpunit
来源：http://gbp.jinyuanbaomall.cn

[U79] PHP：静态分析
来源：http://shw.daria6918.cn

composer require --dev phpstan/phpstan
来源：http://cxx.shangyingyoupin.top

[U80] PHP：代码规范修复
来源：http://hyg.cheryme.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://lgz.feifeiyinyue.top

[U81] JS：初始化项目
来源：http://tmz.bjfxy.top

npm init -y;  npm i express
来源：http://zsp.kuanghao11.cn

[U82] JS：package.json 脚本
来源：http://ysa.fzhhl.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://zvo.nanxinkj.top

[U83] JS：ES Module 导入导出
来源：http://amx.tian-w.cn

export const a = 1;  import { a } from "./m.js";
来源：http://yco.hnxiangtu.top

[U84] JS：CommonJS 写法
来源：http://jzq.sweek.top

module.exports = { a };  const { a } = require("./m");
来源：http://fyo.jqgfzy.top

[U85] JS：可选链
来源：http://frq.xingfuxueyuan.xyz

a?.b?.c
来源：http://zdc.daxiang520.top

[U86] JS：空值合并
来源：http://ywz.chenlongwang.top

a ?? b
来源：http://ouf.bjfxy.top

[U87] JS：解构默认值
来源：http://rxj.haohaochexian.top

const { a = 1, b = 2 } = obj;
来源：http://jaz.sxryk.cn

[U88] JS：对象展开合并
来源：http://wky.yuxming.cn

{ ...a, ...b }
来源：http://ehq.cheryme.top

[U89] JS：数组去重
来源：http://yws.daxiang520.top

[...new Set(arr)]
来源：http://pvh.ctjpmb.com

[U90] JS：数字数组排序
来源：http://ofy.sjlbkw.cn

[...arr].sort((a, b) => a - b)
来源：http://knp.fengsongda.top

[U91] JS：对象键值遍历
来源：http://jmc.jinghuilouyu.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://gni.shanyushiyangtech.top

[U92] JS：深拷贝
来源：http://oar.cqqwz.cn

structuredClone(obj)
来源：http://jhq.ppjwa.cn

[U93] JS：模板字符串
来源：http://tfr.zdqjudy.top

`共 ${n} 条`
来源：http://ryp.bbcook.cn

[U94] JS：箭头函数
来源：http://vuj.nanxuanxn.top

const double = x => x * 2;
来源：http://sve.yanxiufei.cn

[U95] JS：Promise 包装
来源：http://yud.zhijiandao.cn

new Promise((resolve, reject) => {})
来源：http://fbk.yonumen.top

[U96] JS：async/await 与异常
来源：http://qeu.fanxiaobao.xyz

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://gnr.gaohongyu789.top

[U97] JS：并发请求
来源：http://kze.fehbvm.com

await Promise.all(urls.map(u => fetch(u)))
来源：http://nbm.jyoumei.cn

[U98] JS：fetch 带 JSON
来源：http://yll.ivvv.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://ckn.fktsv.cn

[U99] JS：事件监听
来源：http://cki.fehbvm.com

el.addEventListener("click", e => {})
来源：http://tkv.tanke756.top

[U100] JS：DOM 查询
来源：http://mnm.cdnleiting.top

document.querySelector(".item")
来源：http://ajy.pycfn.com

[U101] JS：classList 操作
来源：http://zct.zhaomingkeji.xyz

el.classList.toggle("active")
来源：http://yti.52xcode.cn

[U102] JS：本地存储
来源：http://yxw.hysaishi.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://lkr.dashuyun.cn

[U103] JS：定时器
来源：http://irq.yueranfly.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://xdv.sjlbkw.cn

[U104] JS：防抖
来源：http://zxp.yanxiufei.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ynu.hysaishi.cn

[U105] JS：节流
来源：http://ipc.bjfxy.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://til.zdbjq.cn

[U106] JS：日期格式化
来源：http://beq.pengpengdd.cyou

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://lvq.9152youxi.cn

[U107] JS：数字千分位
来源：http://kwh.aizwys.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://kpy.shuidangran.top

[U108] JS：随机整数
来源：http://ozc.ydzc1.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://jri.chenjidiqi.icu

[U109] JS：数组分组
来源：http://jnp.zhaomingkeji.xyz

Object.groupBy(arr, x => x.type)
来源：http://vfb.ivvv.top

[U110] JS：数组分块
来源：http://hfu.zdqjudy.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://qtm.hnqzz.top

[U111] JS：对象转 Map
来源：http://tvn.xingfuxueyuan.xyz

new Map(Object.entries(obj))
来源：http://waz.sxryk.cn

[U112] JS：字符串补位
来源：http://sfy.zhixingplan.top

"7".padStart(3, "0")
来源：http://pyw.jqgufenzy.top

[U113] JS：正则替换全部
来源：http://hwe.yonumen.top

s.replaceAll("a", "b")
来源：http://oyx.pycfn.com

[U114] JS：JSON 深比较
来源：http://feb.hcnkem.com

JSON.stringify(a) === JSON.stringify(b)
来源：http://ine.nwbrower.top

[U115] JS：生成 UUID
来源：http://zgb.hysaishi.cn

crypto.randomUUID()
来源：http://juc.hfpthk.cn

[U116] JS：类型检查（JSDoc）
来源：http://mrl.gzhubu.top

/** @param {string} name */ function f(name) {}
来源：http://lxn.hnqzz.top

[U117] JS：单元测试
来源：http://qne.yueranfly.top

npm i -D vitest;  npx vitest
来源：http://ouk.0kj1m.cn

[U118] JS：开发服务器
来源：http://zeq.yj20258.top

npm i -D vite;  npx vite
来源：http://sad.vqdsnc.cn

[U119] JS：生产构建
来源：http://kyt.zhengqikj.top

npx vite build
来源：http://lsn.pengpengdd.cyou

[U120] JS：读取环境变量（Vite）
来源：http://nyl.jinqigfzy.top

import.meta.env.VITE_API_URL
来源：http://ynh.pycfn.com

================================================================================
来源：http://bjp.yonumen.top

统计汇总
来源：http://wvd.iojbl.cn

================================================================================
来源：http://nag.hcnkem.com

按语言统计（条）：
来源：http://nmh.ehwqpu.com

Python ......... 252
来源：http://upu.yfazqb.com

PHP ............ 252
来源：http://mph.0kj1m.cn

JavaScript ..... 252
来源：http://hmf.pycfn.com

TypeScript ..... 212
来源：http://xkw.zhengqikj.top

Java ........... 212
来源：http://qbd.hnqzz.top

Go ............. 212
来源：http://jqr.shanyushiyangtech.top

Ruby ........... 212
来源：http://rar.xingfuxueyuan.xyz

C# ............. 212
来源：http://jja.shanyushiyangkeji.top

C .............. 30
来源：http://oac.snrcjt.cn

C++ ............ 30
来源：http://agf.aizwys.cn

SQL ............ 90
来源：http://spd.shzxlz.cn

Bash ........... 80
来源：http://qqe.wangdashe.top

Kotlin ......... 15
来源：http://adq.vqdsnc.cn

Swift .......... 15
来源：http://fjl.yonumen.top

Lua ............ 10
来源：http://fkh.tanke756.top

Perl ........... 10
来源：http://pce.c1oappe.top

Scala .......... 10
来源：http://lli.smart0.xyz

------------------------------------
来源：http://bvq.jqgufenzy.top

合计 ........... 2106 条
来源：http://stt.cdnleiting.top

按章节统计：
来源：http://zll.cashguo.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://rnw.yonumen.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://sbn.snrcjt.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://bpt.hammf.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://dvo.hysaishi.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://mpr.ywan-chungtsiang.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://mtp.zhijiandao.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://exm.nwbrower.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://xib.guannengcc.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://qez.yj202588.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://mao.wangdashe.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://jvt.redwolf501.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://xrh.chenzaomai.com

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://tnl.bjfxy.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://elg.jqgfzy.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://qwy.vqdsnc.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://ccu.hesvh.cn

Q SQL 专题                              90
来源：http://snj.cdnleiting.top

R Bash 专题                             80
来源：http://gnx.xuetiantiany.cn

S C / C++ 专题                          60
来源：http://zme.pengpengdd.cyou

T 其他语言补充                          60
来源：http://zqs.ybcxt.top

U 高频实用片段                         120
来源：http://tdz.chenjidiqi.icu

------------------------------------
来源：http://oij.chenzaomai.com

合计                                  2106 条
来源：http://rqp.tarul.cn

--------------------------------------------------------------------------------
来源：http://poz.hfpthk.cn

使用提醒
来源：http://goq.yonumen.top

--------------------------------------------------------------------------------
来源：http://ieh.aibaodan.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://mgv.svipenyu.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://tch.fengsongda.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://vgi.jinghuilouyu.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://gin.vqdsnc.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://blb.wangshuangyany.cn

—— 文件结束 ——
来源：http://psl.yongpay.top

================================================================================
来源：http://ryl.gogol.net.cn

程序语言常见例子速查手册（2024 版）
来源：http://ykd.ybcxt.top

Common Programming Examples Cheat Book
来源：http://azf.cucudq.cn

================================================================================
来源：http://nnz.nanxinkj.top

【收录内容】
来源：http://aru.dianchejie.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://xij.hfpthk.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://nan.ybcxt.top

SQL · Bash · C · C++
来源：http://coy.fzhhl.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://rtn.zhoulong.xyz

【使用说明】
来源：http://nsn.zhongyouzk.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://fwk.chenlongwang.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://dcm.jinyuanbaomall.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://zul.havefunace.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://gkk.sxryk.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://tyi.bbcook.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://tuh.zhiwuduotai.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://qse.andypj.xyz

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://xvh.yonumen.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://qyy.nanxuanxn.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://lyl.hnqzz.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://anj.sufxvd.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://bgh.zhaomingkeji.xyz

【文件统计】
来源：http://gpk.gaohongyu789.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://yrh.havefunace.top

--------------------------------------------------------------------------------
来源：http://cod.jlsjyb.cn

目  录
来源：http://ycd.zhoulong.xyz

--------------------------------------------------------------------------------
来源：http://euj.xylfe.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://faj.zhiwuduotai.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://jxx.mhx1999.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://trn.sweek.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://ywo.smart0.xyz

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://ymv.yongpay.top


<!-- 参考信息 -->