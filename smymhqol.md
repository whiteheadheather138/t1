代发 wailian999

[U13] Py：固定长度队列
来源：http://ufk.haohaochexian.top

deque(maxlen=10)
来源：http://eel.yvedp.cn

[U14] Py：分组收集到列表
来源：http://ffk.yj20258888.top

defaultdict(list)
来源：http://zom.wangshuangyany.cn

[U15] Py：高精度计时
来源：http://gcs.redwolf501.top

t = time.perf_counter()
来源：http://erd.kuanghao11.cn

[U16] Py：命令行参数解析
来源：http://smz.svipenyu.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://oso.shzxlz.cn

[U17] Py：初始化日志
来源：http://amm.epnwcf.com

logging.basicConfig(level=logging.INFO)
来源：http://vsx.pycfn.com

[U18] Py：预编译正则
来源：http://fgy.iojbl.cn

pat = re.compile(r"\d+")
来源：http://gov.wangshuangyany.cn

[U19] Py：正则替换带回调
来源：http://qxm.hfpthk.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://qrr.mhx1999.top

[U20] Py：缓存函数结果
来源：http://lvd.cashguo.top

@functools.lru_cache(maxsize=None)
来源：http://sun.smart0.xyz

[U21] Py：自定义上下文管理器
来源：http://hln.uphjek.com

@contextlib.contextmanager
来源：http://keu.tarul.cn

[U22] Py：矩阵转置
来源：http://bdo.hcnkem.com

list(zip(*m))
来源：http://qga.sjlbkw.cn

[U23] Py：分块读取大文件
来源：http://ueh.xuanzx.com

for chunk in iter(lambda: f.read(8192), b""):
来源：http://iwl.andypj.xyz

[U24] Py：路径操作
来源：http://utj.nanxuanxn.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://iak.bbcook.cn

[U25] Py：CSV 按字典读
来源：http://qfb.shangyingyoupin.top

csv.DictReader(f)
来源：http://ibv.shanyushiyangkeji.top

[U26] Py：并发下载
来源：http://jom.jqgfzy.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://mmu.jianghu66.top

[U27] Py：异步 HTTP
来源：http://gzr.sysykeji.top

aiohttp.ClientSession() 配合 async with
来源：http://axw.snrcjt.cn

[U28] Py：类型别名
来源：http://adt.0kj1m.cn

UserId = int
来源：http://krf.xylfe.cn

[U29] Py：属性校验
来源：http://dam.svipenyu.cn

@property 与 @x.setter 配合
来源：http://oda.xziqi.cn

[U30] Py：数据类
来源：http://nyy.sufxvd.cn

@dataclass(slots=True)
来源：http://jpw.hywenlv.cn

[U31] Py：单测
来源：http://gwy.ppjwa.cn

python -m pytest -q
来源：http://raq.yangfankeji.com

[U32] Py：代码格式化
来源：http://ckb.iojbl.cn

ruff format . && ruff check --fix .
来源：http://bsw.fanxiaobao.xyz

[U33] Py：打包发布
来源：http://ouy.bjfxy.top

python -m build  （依赖 pyproject.toml）
来源：http://def.daria6918.cn

[U34] Py：判断编码
来源：http://egk.gaohongyu789.top

chardet.detect(raw)
来源：http://rns.xingfuxueyuan.xyz

[U35] Py：发送邮件
来源：http://pgr.hongshengwenyu.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://vgj.andypj.xyz

[U36] Py：定时任务
来源：http://lfq.dianchejie.cn

schedule.every(10).minutes.do(job)
来源：http://jrz.ywan-chungtsiang.top

[U37] Py：读写 Excel
来源：http://plc.hongshengwenyu.top

pandas.read_excel / DataFrame.to_excel
来源：http://ynf.yvedp.cn

[U38] Py：获取脚本所在目录
来源：http://vil.xuetiantiany.cn

Path(__file__).resolve().parent
来源：http://iuo.316326.xyz

[U39] Py：判断是否在交互环境
来源：http://hhd.zycfv.cn

sys.stdout.isatty()
来源：http://nus.havefunace.top

[U40] Py：打印到标准错误
来源：http://xge.zdbjq.cn

print("err", file=sys.stderr)
来源：http://fog.jyoumei.cn

[U41] PHP：初始化 Composer 项目
来源：http://tly.9152youxi.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://cfz.xinyue.icu

[U42] PHP：PSR-4 自动加载
来源：http://ivn.c1oappe.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://prp.jinqigfzy.top

[U43] PHP：声明命名空间
来源：http://htc.smart0.xyz

namespace App\Http;
来源：http://rub.xuanzx.com

[U44] PHP：开启严格类型
来源：http://chx.sxryk.cn

declare(strict_types=1);
来源：http://cbr.guannengcc.top

[U45] PHP：类型声明与返回类型
来源：http://vry.zycfv.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://zrm.ywan-chungtsiang.top

[U46] PHP：可空类型
来源：http://fce.ydjk.org.cn

?string $name = null
来源：http://nfg.ctjpmb.com

[U47] PHP：联合类型
来源：http://haa.yangfankeji.com

int|string $id
来源：http://buw.gzhubu.top

[U48] PHP：纯枚举
来源：http://stz.feifeiyinyue.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://xpv.sjlbkw.cn

[U49] PHP：只读属性
来源：http://kmu.svipenyu.cn

public readonly string $name
来源：http://gfv.sweek.top

[U50] PHP：构造器属性提升
来源：http://grg.zhixingplan.top

public function __construct(private int $id) {}
来源：http://olj.hesvh.cn

[U51] PHP：数组解构
来源：http://ygt.ehwqpu.com

[$a, $b] = $arr;
来源：http://fgy.tarul.cn

[U52] PHP：箭头函数
来源：http://oim.jinqigufen.top

$double = fn($x) => $x * 2;
来源：http://vmj.hongshengwenyu.top

[U53] PHP：空合并运算符
来源：http://kzo.xingfuxueyuan.xyz

$v = $a ?? $b ?? "default";
来源：http://thn.tarul.cn

[U54] PHP：空安全调用
来源：http://uwc.zhaomingkeji.xyz

$obj?->method()
来源：http://xuu.svipenyu.cn

[U55] PHP：match 表达式
来源：http://ilh.xuetiantiany.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://spr.zdqjudy.top

[U56] PHP：命名参数
来源：http://dqj.jinghuilouyu.cn

f(a: 1, b: 2)
来源：http://sgn.haohaochexian.top

[U57] PHP：字符串插值
来源：http://wgi.9152youxi.cn

"值: {$a}"
来源：http://ogd.jinqigfzy.top

[U58] PHP：数组三件套
来源：http://xby.jinyuanbaomall.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://ntw.sjlbkw.cn

[U59] PHP：自定义排序
来源：http://wxm.fehbvm.com

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wkb.nwbrower.top

[U60] PHP：JSON 编解码
来源：http://gdj.chenlongwang.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://abj.hysaishi.cn

[U61] PHP：正则
来源：http://ava.gotoacloud.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://jtr.guowangkeji.top

[U62] PHP：日期对象
来源：http://xub.daxiang520.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://dzc.ehwqpu.com

[U63] PHP：文件读写
来源：http://til.yonumen.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://gmi.cqqwz.cn

[U64] PHP：目录遍历
来源：http://rwz.daxiang520.top

glob("dir/*.php");  scandir("dir");
来源：http://pah.guowangkeji.top

[U65] PHP：会话
来源：http://dyb.zhiwuduotai.top

session_start();  $_SESSION["uid"] = 1;
来源：http://dit.shzxlz.cn

[U66] PHP：设置 Cookie
来源：http://fyj.jinqigufen.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://koj.mhx1999.top

[U67] PHP：处理文件上传
来源：http://lpc.fehbvm.com

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://yhx.haohaochexian.top

[U68] PHP：PDO 连接
来源：http://lwg.jianghu66.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://rni.jlsjyb.cn

[U69] PHP：PDO 预处理
来源：http://rpt.shanyushiyangtech.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://enk.vqdsnc.cn

[U70] PHP：PDO 事务
来源：http://alz.guowangkeji.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://wox.chenlongwang.top

[U71] PHP：抛出异常
来源：http://adg.0kj1m.cn

throw new RuntimeException("失败", 500);
来源：http://ecy.yj20258.top

[U72] PHP：写错误日志
来源：http://azh.smart0.xyz

error_log("失败: " . $e->getMessage());
来源：http://gfj.ywan-chungtsiang.top

[U73] PHP：读取 ini 配置
来源：http://omk.zhixingplan.top

parse_ini_file("config.ini", true)
来源：http://xnw.sysykeji.top

[U74] PHP：读取环境变量
来源：http://ovi.ehwqpu.com

getenv("APP_ENV") ?: "production"
来源：http://gtn.ybcxt.top

[U75] PHP：依赖注入
来源：http://uha.jinyuanbaomall.cn

composer require psr/container
来源：http://nai.haohaochexian.top

[U76] PHP：简单路由
来源：http://hbd.hywenlv.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://oun.bjfxy.top

[U77] PHP：模板渲染
来源：http://ylc.cucudq.cn

composer require twig/twig
来源：http://nuq.gotoacloud.top

[U78] PHP：单元测试
来源：http://rlw.hesvh.cn

composer require --dev phpunit/phpunit
来源：http://evj.zdbjq.cn

[U79] PHP：静态分析
来源：http://mfp.chenjidiqi.icu

composer require --dev phpstan/phpstan
来源：http://ggv.52xcode.cn

[U80] PHP：代码规范修复
来源：http://qjf.gotoacloud.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://jli.zhoulong.xyz

[U81] JS：初始化项目
来源：http://vja.xuetiantiany.cn

npm init -y;  npm i express
来源：http://pja.shuidangran.top

[U82] JS：package.json 脚本
来源：http://ktj.0kj1m.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://dmc.kuanghao11.cn

[U83] JS：ES Module 导入导出
来源：http://zef.yongpay.top

export const a = 1;  import { a } from "./m.js";
来源：http://qwr.xuetiantiany.cn

[U84] JS：CommonJS 写法
来源：http://kek.fanxiaobao.xyz

module.exports = { a };  const { a } = require("./m");
来源：http://nyl.hnxiangtu.top

[U85] JS：可选链
来源：http://vsn.c1oappe.top

a?.b?.c
来源：http://nvj.dianchejie.cn

[U86] JS：空值合并
来源：http://xyi.chenzaomai.com

a ?? b
来源：http://qrf.52xcode.cn

[U87] JS：解构默认值
来源：http://nte.yongpay.top

const { a = 1, b = 2 } = obj;
来源：http://klf.sxryk.cn

[U88] JS：对象展开合并
来源：http://bgf.hcnkem.com

{ ...a, ...b }
来源：http://cut.zhengqikj.top

[U89] JS：数组去重
来源：http://gjf.svipenyu.cn

[...new Set(arr)]
来源：http://rlm.zhengqikj.top

[U90] JS：数字数组排序
来源：http://xpg.nanxinkj.top

[...arr].sort((a, b) => a - b)
来源：http://arm.yonumen.top

[U91] JS：对象键值遍历
来源：http://vgf.mhx1999.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://fug.dianchejie.cn

[U92] JS：深拷贝
来源：http://imn.kuanghao11.cn

structuredClone(obj)
来源：http://hoo.sxryk.cn

[U93] JS：模板字符串
来源：http://gsk.yangfankeji.com

`共 ${n} 条`
来源：http://kmv.xuanzx.com

[U94] JS：箭头函数
来源：http://ynk.xuetiantiany.cn

const double = x => x * 2;
来源：http://odp.pengpengdd.cyou

[U95] JS：Promise 包装
来源：http://coz.epnwcf.com

new Promise((resolve, reject) => {})
来源：http://cxa.havefunace.top

[U96] JS：async/await 与异常
来源：http://huu.jinyuanbaomall.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://wlo.hcnkem.com

[U97] JS：并发请求
来源：http://yfz.9152youxi.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://ijt.chenzaomai.com

[U98] JS：fetch 带 JSON
来源：http://fqs.bbcook.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://ifa.yj202588.top

[U99] JS：事件监听
来源：http://acz.aibaodan.cn

el.addEventListener("click", e => {})
来源：http://uft.zhixingplan.top

[U100] JS：DOM 查询
来源：http://uwb.sysykeji.top

document.querySelector(".item")
来源：http://svm.fengsongda.top

[U101] JS：classList 操作
来源：http://rso.aizwys.cn

el.classList.toggle("active")
来源：http://nyl.zhengqikj.top

[U102] JS：本地存储
来源：http://kpn.hysaishi.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://unq.aibaodan.cn

[U103] JS：定时器
来源：http://vdv.hfpthk.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://xik.xinyue.icu

[U104] JS：防抖
来源：http://pcl.aibaodan.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://kkh.fehbvm.com

[U105] JS：节流
来源：http://ydb.yuxming.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://yfi.hfpthk.cn

[U106] JS：日期格式化
来源：http://dip.jinghuilouyu.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://tno.hnxiangtu.top

[U107] JS：数字千分位
来源：http://sao.fzhhl.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://cyl.yanxiufei.cn

[U108] JS：随机整数
来源：http://gvs.hnxiangtu.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hxv.tian-w.cn

[U109] JS：数组分组
来源：http://mqq.jqgufenzy.top

Object.groupBy(arr, x => x.type)
来源：http://vwx.316326.xyz

[U110] JS：数组分块
来源：http://hgt.jinqigfzy.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://mwu.wangshuangyany.cn

[U111] JS：对象转 Map
来源：http://hhe.cqqwz.cn

new Map(Object.entries(obj))
来源：http://fph.svipenyu.cn

[U112] JS：字符串补位
来源：http://ewe.dashuyun.cn

"7".padStart(3, "0")
来源：http://shi.shuidangran.top

[U113] JS：正则替换全部
来源：http://jku.9152youxi.cn

s.replaceAll("a", "b")
来源：http://dqk.birdmap.top

[U114] JS：JSON 深比较
来源：http://rop.zdqjudy.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://adk.gogol.net.cn

[U115] JS：生成 UUID
来源：http://yaz.ctjpmb.com

crypto.randomUUID()
来源：http://kdy.ywan-chungtsiang.top

[U116] JS：类型检查（JSDoc）
来源：http://dgk.zhijiandao.cn

/** @param {string} name */ function f(name) {}
来源：http://npg.shuidangran.top

[U117] JS：单元测试
来源：http://fcs.pycfn.com

npm i -D vitest;  npx vitest
来源：http://pej.sufxvd.cn

[U118] JS：开发服务器
来源：http://weh.zhixingplan.top

npm i -D vite;  npx vite
来源：http://lsx.xuetiantiany.cn

[U119] JS：生产构建
来源：http://ztl.yj20258888.top

npx vite build
来源：http://kkc.ywan-chungtsiang.top

[U120] JS：读取环境变量（Vite）
来源：http://hxg.ivvv.top

import.meta.env.VITE_API_URL
来源：http://pxg.zhijiandao.cn

================================================================================
来源：http://fvc.smart0.xyz

统计汇总
来源：http://iab.cqqwz.cn

================================================================================
来源：http://hkp.hesvh.cn

按语言统计（条）：
来源：http://tmk.fzhhl.top

Python ......... 252
来源：http://vvw.zycfv.cn

PHP ............ 252
来源：http://zmf.hammf.cn

JavaScript ..... 252
来源：http://ras.hfpthk.cn

TypeScript ..... 212
来源：http://oii.haohaochexian.top

Java ........... 212
来源：http://jzw.zhiwuduotai.top

Go ............. 212
来源：http://ujv.nanxuanxn.top

Ruby ........... 212
来源：http://rrl.yvedp.cn

C# ............. 212
来源：http://rse.zdqjudy.top

C .............. 30
来源：http://ftp.andypj.xyz

C++ ............ 30
来源：http://eew.jinyuanbaomall.cn

SQL ............ 90
来源：http://rvz.tianlin.xyz

Bash ........... 80
来源：http://ten.yfazqb.com

Kotlin ......... 15
来源：http://mml.nanxinkj.top

Swift .......... 15
来源：http://znn.pengpengdd.cyou

Lua ............ 10
来源：http://pbv.yfazqb.com

Perl ........... 10
来源：http://mhb.dashuyun.cn

Scala .......... 10
来源：http://rgp.nwbrower.top

------------------------------------
来源：http://rct.yfazqb.com

合计 ........... 2106 条
来源：http://zgv.ybcxt.top

按章节统计：
来源：http://xnl.kuanghao11.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://koj.jinyuanbaomall.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://xii.gotoacloud.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://tus.xylfe.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://mvl.shuidangran.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://prq.bjfxy.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://ysg.zhoulong.xyz

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://ryd.cheryme.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://new.yuanzhike.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://oro.fengsongda.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://xui.pengpengdd.cyou

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://aqg.chenzaomai.com

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://brr.xingfuxueyuan.xyz

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://qzr.shuidangran.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://wut.nanxinkj.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://vfu.ybcxt.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://chn.shuidangran.top

Q SQL 专题                              90
来源：http://sty.wangdashe.top

R Bash 专题                             80
来源：http://rsk.zhoulong.xyz

S C / C++ 专题                          60
来源：http://vkh.daxiang520.top

T 其他语言补充                          60
来源：http://lim.tian-w.cn

U 高频实用片段                         120
来源：http://wdg.tanke756.top

------------------------------------
来源：http://qzr.andypj.xyz

合计                                  2106 条
来源：http://jtm.dianchejie.cn

--------------------------------------------------------------------------------
来源：http://mjm.bbcook.cn

使用提醒
来源：http://grk.nanxuanxn.top

--------------------------------------------------------------------------------
来源：http://mnp.zhiwuduotai.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://xtb.yueranfly.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://xsi.ctjpmb.com

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://sjx.gotoacloud.top

在旧版本上使用前请先确认语法支持情况。
来源：http://fxj.chenlongwang.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://dmg.hysaishi.cn

—— 文件结束 ——
来源：http://daa.pycfn.com

================================================================================
来源：http://prp.snrcjt.cn

程序语言常见例子速查手册（2024 版）
来源：http://kqf.pycfn.com

Common Programming Examples Cheat Book
来源：http://iuf.jianghu66.top

================================================================================
来源：http://uxs.pengpengdd.cyou

【收录内容】
来源：http://ver.hysaishi.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://wit.yonumen.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://ams.wangshuangyany.cn

SQL · Bash · C · C++
来源：http://yjy.yj20258.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://sza.xinyue.icu

【使用说明】
来源：http://adh.redwolf501.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://fmk.zhoulong.xyz

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://uva.yangfankeji.com

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://pie.vqdsnc.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://ydq.jiagoushi.top

Bash:  Shell         C:     C             C++:   C++
来源：http://yoz.epnwcf.com

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://ukd.sysykeji.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://drg.guowangkeji.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://dxf.xinyue.icu

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://zwp.hywenlv.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://cbi.smart0.xyz

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://csh.sjlbkw.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://mft.fanxiaobao.xyz

【文件统计】
来源：http://mdb.gzhubu.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://ecl.tarul.cn

--------------------------------------------------------------------------------
来源：http://vxs.birdmap.top

目  录
来源：http://yml.tanke756.top

--------------------------------------------------------------------------------
来源：http://gyr.zhiwuduotai.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://uqj.zhengqikj.top


<!-- 参考信息 -->