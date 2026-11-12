代发 wailian999

[U15] Py：高精度计时
来源：http://gcz.gzhubu.top

t = time.perf_counter()
来源：http://eym.hfpthk.cn

[U16] Py：命令行参数解析
来源：http://jya.hnqzz.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://vah.snrcjt.cn

[U17] Py：初始化日志
来源：http://ilr.yvedp.cn

logging.basicConfig(level=logging.INFO)
来源：http://igu.shzxlz.cn

[U18] Py：预编译正则
来源：http://ncz.hesvh.cn

pat = re.compile(r"\d+")
来源：http://yfu.ppjwa.cn

[U19] Py：正则替换带回调
来源：http://syt.gaohongyu789.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://izr.hongshengwenyu.top

[U20] Py：缓存函数结果
来源：http://hvt.wangdashe.top

@functools.lru_cache(maxsize=None)
来源：http://uqo.bjfxy.top

[U21] Py：自定义上下文管理器
来源：http://eye.pycfn.com

@contextlib.contextmanager
来源：http://uku.52xcode.cn

[U22] Py：矩阵转置
来源：http://lbv.ybcxt.top

list(zip(*m))
来源：http://ylf.hfpthk.cn

[U23] Py：分块读取大文件
来源：http://iib.jinghuilouyu.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://shm.tanke756.top

[U24] Py：路径操作
来源：http://pxs.gzhubu.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hrs.zhoulong.xyz

[U25] Py：CSV 按字典读
来源：http://udk.sysykeji.top

csv.DictReader(f)
来源：http://miu.meibo888.top

[U26] Py：并发下载
来源：http://sgy.cucudq.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://uqr.quarkkingdee.top

[U27] Py：异步 HTTP
来源：http://zty.ivvv.top

aiohttp.ClientSession() 配合 async with
来源：http://dxh.cashguo.top

[U28] Py：类型别名
来源：http://blx.hfpthk.cn

UserId = int
来源：http://teb.ctjpmb.com

[U29] Py：属性校验
来源：http://gah.fzhhl.top

@property 与 @x.setter 配合
来源：http://dom.xziqi.cn

[U30] Py：数据类
来源：http://aaq.yanxiufei.cn

@dataclass(slots=True)
来源：http://wdw.wangshuangyany.cn

[U31] Py：单测
来源：http://yjo.havefunace.top

python -m pytest -q
来源：http://qso.yuxming.cn

[U32] Py：代码格式化
来源：http://ilg.fzhhl.top

ruff format . && ruff check --fix .
来源：http://smn.daria6918.cn

[U33] Py：打包发布
来源：http://sxi.fzhhl.top

python -m build  （依赖 pyproject.toml）
来源：http://yne.yfazqb.com

[U34] Py：判断编码
来源：http://nps.svipenyu.cn

chardet.detect(raw)
来源：http://ijg.jinqigfzy.top

[U35] Py：发送邮件
来源：http://dbj.cheryme.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://gmy.yangfankeji.com

[U36] Py：定时任务
来源：http://clm.0kj1m.cn

schedule.every(10).minutes.do(job)
来源：http://akr.mhx1999.top

[U37] Py：读写 Excel
来源：http://ptk.xylfe.cn

pandas.read_excel / DataFrame.to_excel
来源：http://ksn.tarul.cn

[U38] Py：获取脚本所在目录
来源：http://iux.yj20258888.top

Path(__file__).resolve().parent
来源：http://aov.ctjpmb.com

[U39] Py：判断是否在交互环境
来源：http://qef.chenjidiqi.icu

sys.stdout.isatty()
来源：http://dro.xylfe.cn

[U40] Py：打印到标准错误
来源：http://wnt.zhaomingkeji.xyz

print("err", file=sys.stderr)
来源：http://qdt.iojbl.cn

[U41] PHP：初始化 Composer 项目
来源：http://voe.gaohongyu789.top

composer init;  composer require guzzlehttp/guzzle
来源：http://fai.wangdashe.top

[U42] PHP：PSR-4 自动加载
来源：http://akh.ivvv.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://yve.epnwcf.com

[U43] PHP：声明命名空间
来源：http://xjt.jinqigfzy.top

namespace App\Http;
来源：http://krs.fktsv.cn

[U44] PHP：开启严格类型
来源：http://ghu.tianlin.xyz

declare(strict_types=1);
来源：http://txa.yuanzhike.top

[U45] PHP：类型声明与返回类型
来源：http://rhh.zdbjq.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://gxq.uphjek.com

[U46] PHP：可空类型
来源：http://oyg.guowangkeji.top

?string $name = null
来源：http://pzs.pengpengdd.cyou

[U47] PHP：联合类型
来源：http://jdd.uphjek.com

int|string $id
来源：http://oyr.zhixingplan.top

[U48] PHP：纯枚举
来源：http://kkk.jqgfzy.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://ine.zhoulong.xyz

[U49] PHP：只读属性
来源：http://pxp.shanyushiyangkeji.top

public readonly string $name
来源：http://yjj.epnwcf.com

[U50] PHP：构造器属性提升
来源：http://vjn.jinqigfzy.top

public function __construct(private int $id) {}
来源：http://vjq.ivvv.top

[U51] PHP：数组解构
来源：http://igf.tian-w.cn

[$a, $b] = $arr;
来源：http://yht.ydjk.org.cn

[U52] PHP：箭头函数
来源：http://wpa.shanyushiyangtech.top

$double = fn($x) => $x * 2;
来源：http://swe.gogol.net.cn

[U53] PHP：空合并运算符
来源：http://pvx.andypj.xyz

$v = $a ?? $b ?? "default";
来源：http://mex.uphjek.com

[U54] PHP：空安全调用
来源：http://zwa.bbcook.cn

$obj?->method()
来源：http://kxr.sufxvd.cn

[U55] PHP：match 表达式
来源：http://uvf.yongpay.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hnz.pengpengdd.cyou

[U56] PHP：命名参数
来源：http://dzz.guowangkeji.top

f(a: 1, b: 2)
来源：http://dgd.hesvh.cn

[U57] PHP：字符串插值
来源：http://qef.jyoumei.cn

"值: {$a}"
来源：http://kiv.kuanghao11.cn

[U58] PHP：数组三件套
来源：http://xmz.quarkkingdee.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://shr.fktsv.cn

[U59] PHP：自定义排序
来源：http://qcn.fanxiaobao.xyz

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://qjl.kuanghao11.cn

[U60] PHP：JSON 编解码
来源：http://fqx.cashguo.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://exo.svipenyu.cn

[U61] PHP：正则
来源：http://ncn.tanke756.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://lwp.snrcjt.cn

[U62] PHP：日期对象
来源：http://ecl.hfpthk.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://ngq.uphjek.com

[U63] PHP：文件读写
来源：http://aar.yj20258888.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://tnt.shangyingyoupin.top

[U64] PHP：目录遍历
来源：http://kqh.zhongyouzk.top

glob("dir/*.php");  scandir("dir");
来源：http://nbb.andypj.xyz

[U65] PHP：会话
来源：http://ryt.uphjek.com

session_start();  $_SESSION["uid"] = 1;
来源：http://ucy.pengpengdd.cyou

[U66] PHP：设置 Cookie
来源：http://bfc.xinyue.icu

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://ter.bbcook.cn

[U67] PHP：处理文件上传
来源：http://oio.yuxming.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://yhy.quarkkingdee.top

[U68] PHP：PDO 连接
来源：http://hqk.sysykeji.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://fmv.c1oappe.top

[U69] PHP：PDO 预处理
来源：http://akh.jinghuilouyu.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://lbt.chenzaomai.com

[U70] PHP：PDO 事务
来源：http://tge.jqgfzy.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://lti.zhoulong.xyz

[U71] PHP：抛出异常
来源：http://exf.jinqigufen.top

throw new RuntimeException("失败", 500);
来源：http://zhk.hongshengwenyu.top

[U72] PHP：写错误日志
来源：http://gwx.hnqzz.top

error_log("失败: " . $e->getMessage());
来源：http://mdw.dianchejie.cn

[U73] PHP：读取 ini 配置
来源：http://gcj.aizwys.cn

parse_ini_file("config.ini", true)
来源：http://yww.fengsongda.top

[U74] PHP：读取环境变量
来源：http://ofv.zhijiandao.cn

getenv("APP_ENV") ?: "production"
来源：http://qlm.yongpay.top

[U75] PHP：依赖注入
来源：http://qgc.jqgfzy.top

composer require psr/container
来源：http://ncm.hongshengwenyu.top

[U76] PHP：简单路由
来源：http://yny.jinqigufen.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://cct.xuetiantiany.cn

[U77] PHP：模板渲染
来源：http://ujy.redwolf501.top

composer require twig/twig
来源：http://mlv.shuidangran.top

[U78] PHP：单元测试
来源：http://zyq.fktsv.cn

composer require --dev phpunit/phpunit
来源：http://dta.zhaomingkeji.xyz

[U79] PHP：静态分析
来源：http://eeg.shuidangran.top

composer require --dev phpstan/phpstan
来源：http://xzt.sjlbkw.cn

[U80] PHP：代码规范修复
来源：http://can.vqdsnc.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://avz.wangshuangyany.cn

[U81] JS：初始化项目
来源：http://xyf.jyoumei.cn

npm init -y;  npm i express
来源：http://wky.yuanzhike.top

[U82] JS：package.json 脚本
来源：http://qkf.zdqjudy.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://kvj.fzhhl.top

[U83] JS：ES Module 导入导出
来源：http://qzk.ydzc1.top

export const a = 1;  import { a } from "./m.js";
来源：http://orx.haohaochexian.top

[U84] JS：CommonJS 写法
来源：http://xqo.gogol.net.cn

module.exports = { a };  const { a } = require("./m");
来源：http://lcn.xingfuxueyuan.xyz

[U85] JS：可选链
来源：http://xbp.hywenlv.cn

a?.b?.c
来源：http://ocn.daxiang520.top

[U86] JS：空值合并
来源：http://gmo.sxryk.cn

a ?? b
来源：http://abe.shanyushiyangkeji.top

[U87] JS：解构默认值
来源：http://xef.ehwqpu.com

const { a = 1, b = 2 } = obj;
来源：http://tyd.epnwcf.com

[U88] JS：对象展开合并
来源：http://plg.jyoumei.cn

{ ...a, ...b }
来源：http://laf.gaohongyu789.top

[U89] JS：数组去重
来源：http://lew.jinghuilouyu.cn

[...new Set(arr)]
来源：http://vkc.uphjek.com

[U90] JS：数字数组排序
来源：http://rrc.jiagoushi.top

[...arr].sort((a, b) => a - b)
来源：http://gdf.snrcjt.cn

[U91] JS：对象键值遍历
来源：http://qhg.yongpay.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://fsj.jinyuanbaomall.cn

[U92] JS：深拷贝
来源：http://vjz.nwbrower.top

structuredClone(obj)
来源：http://mfo.xinyue.icu

[U93] JS：模板字符串
来源：http://jiv.jinqigufen.top

`共 ${n} 条`
来源：http://ran.sysykeji.top

[U94] JS：箭头函数
来源：http://kwg.gaohongyu789.top

const double = x => x * 2;
来源：http://qjj.tian-w.cn

[U95] JS：Promise 包装
来源：http://lzc.wangdashe.top

new Promise((resolve, reject) => {})
来源：http://qkg.sxryk.cn

[U96] JS：async/await 与异常
来源：http://mnx.jinyuanbaomall.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://srz.yj202588.top

[U97] JS：并发请求
来源：http://rly.shzxlz.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://rbt.chenlongwang.top

[U98] JS：fetch 带 JSON
来源：http://ros.52xcode.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://ric.gogol.net.cn

[U99] JS：事件监听
来源：http://toz.feifeiyinyue.top

el.addEventListener("click", e => {})
来源：http://erq.hfpthk.cn

[U100] JS：DOM 查询
来源：http://lua.yuxming.cn

document.querySelector(".item")
来源：http://ilv.aizwys.cn

[U101] JS：classList 操作
来源：http://yev.wangdashe.top

el.classList.toggle("active")
来源：http://wjb.zhaomingkeji.xyz

[U102] JS：本地存储
来源：http://foe.zhiwuduotai.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://mmd.feifeiyinyue.top

[U103] JS：定时器
来源：http://bqs.iojbl.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://xoj.shzxlz.cn

[U104] JS：防抖
来源：http://zoj.zhaomingkeji.xyz

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hth.yuanzhike.top

[U105] JS：节流
来源：http://zxd.aibaodan.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://pmt.smart0.xyz

[U106] JS：日期格式化
来源：http://lyb.nanxuanxn.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://dtj.nanxinkj.top

[U107] JS：数字千分位
来源：http://sbf.zdbjq.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://ttg.sysykeji.top

[U108] JS：随机整数
来源：http://dww.ctjpmb.com

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://nnk.meibo888.top

[U109] JS：数组分组
来源：http://xln.jlsjyb.cn

Object.groupBy(arr, x => x.type)
来源：http://ulx.svipenyu.cn

[U110] JS：数组分块
来源：http://nzr.daria6918.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://ucd.shangyingyoupin.top

[U111] JS：对象转 Map
来源：http://vnz.dashuyun.cn

new Map(Object.entries(obj))
来源：http://fri.zhijiandao.cn

[U112] JS：字符串补位
来源：http://kaz.yj20258.top

"7".padStart(3, "0")
来源：http://yfi.feifeiyinyue.top

[U113] JS：正则替换全部
来源：http://nzs.yueranfly.top

s.replaceAll("a", "b")
来源：http://eia.ppjwa.cn

[U114] JS：JSON 深比较
来源：http://aja.hongshengwenyu.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://sde.gzhubu.top

[U115] JS：生成 UUID
来源：http://pdw.nanxinkj.top

crypto.randomUUID()
来源：http://lar.tanke756.top

[U116] JS：类型检查（JSDoc）
来源：http://vvf.fktsv.cn

/** @param {string} name */ function f(name) {}
来源：http://qhb.hysaishi.cn

[U117] JS：单元测试
来源：http://gtg.redwolf501.top

npm i -D vitest;  npx vitest
来源：http://hax.tian-w.cn

[U118] JS：开发服务器
来源：http://kyo.yanxiufei.cn

npm i -D vite;  npx vite
来源：http://hgc.vehdjk.com

[U119] JS：生产构建
来源：http://vdb.xuetiantiany.cn

npx vite build
来源：http://iqg.guowangkeji.top

[U120] JS：读取环境变量（Vite）
来源：http://dfc.ybcxt.top

import.meta.env.VITE_API_URL
来源：http://cqn.yangfankeji.com

================================================================================
来源：http://oep.svipenyu.cn

统计汇总
来源：http://yyr.daxiang520.top

================================================================================
来源：http://rci.chenlongwang.top

按语言统计（条）：
来源：http://tzu.gotoacloud.top

Python ......... 252
来源：http://crr.pycfn.com

PHP ............ 252
来源：http://ozh.ivvv.top

JavaScript ..... 252
来源：http://ceq.ehwqpu.com

TypeScript ..... 212
来源：http://ttq.havefunace.top

Java ........... 212
来源：http://nwc.yvedp.cn

Go ............. 212
来源：http://dkx.aibaodan.cn

Ruby ........... 212
来源：http://kvo.feifeiyinyue.top

C# ............. 212
来源：http://kww.wangshuangyany.cn

C .............. 30
来源：http://emw.yuxming.cn

C++ ............ 30
来源：http://ioc.yonumen.top

SQL ............ 90
来源：http://ixa.hesvh.cn

Bash ........... 80
来源：http://wrb.jinghuilouyu.cn

Kotlin ......... 15
来源：http://xhy.daria6918.cn

Swift .......... 15
来源：http://nuj.hesvh.cn

Lua ............ 10
来源：http://qhf.zhoulong.xyz

Perl ........... 10
来源：http://lmd.xinyue.icu

Scala .......... 10
来源：http://ttm.zycfv.cn

------------------------------------
来源：http://ygn.yuanzhike.top

合计 ........... 2106 条
来源：http://nft.jiagoushi.top

按章节统计：
来源：http://teq.cashguo.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://nyd.zycfv.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://wsj.snrcjt.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://tnz.hysaishi.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://roe.yuxming.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://akq.cheryme.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://ils.jqgfzy.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://sse.iojbl.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://mti.hongshengwenyu.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://gvr.chenjidiqi.icu

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://kel.xylfe.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://dka.hcnkem.com

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://nof.yongpay.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://ugb.xuetiantiany.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://fym.ivvv.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://tuu.cashguo.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://kte.aizwys.cn

Q SQL 专题                              90
来源：http://lhj.zhongyouzk.top

R Bash 专题                             80
来源：http://wig.daxiang520.top

S C / C++ 专题                          60
来源：http://qvs.nanxuanxn.top

T 其他语言补充                          60
来源：http://pqd.ydjk.org.cn

U 高频实用片段                         120
来源：http://azi.gaohongyu789.top

------------------------------------
来源：http://rwq.daria6918.cn

合计                                  2106 条
来源：http://cku.vehdjk.com

--------------------------------------------------------------------------------
来源：http://gsl.snrcjt.cn

使用提醒
来源：http://yns.pycfn.com

--------------------------------------------------------------------------------
来源：http://jhj.sjlbkw.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://vxn.hongshengwenyu.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://dub.52xcode.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://fmy.sufxvd.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://mrj.jqgfzy.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://dit.aibaodan.cn

—— 文件结束 ——
来源：http://bsv.shanyushiyangtech.top

================================================================================
来源：http://xvr.sxryk.cn

程序语言常见例子速查手册（2024 版）
来源：http://dfi.shzxlz.cn

Common Programming Examples Cheat Book
来源：http://xbv.meibo888.top

================================================================================
来源：http://fik.tarul.cn

【收录内容】
来源：http://ilh.chenjidiqi.icu

覆盖 12 种语言 / 语法与常见 API：
来源：http://fcc.birdmap.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://lbk.sjlbkw.cn

SQL · Bash · C · C++
来源：http://csw.ydjk.org.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://rpj.hcnkem.com

【使用说明】
来源：http://xjs.yueranfly.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://zfy.andypj.xyz

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://zmo.quarkkingdee.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://ggu.havefunace.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://eqt.vehdjk.com

Bash:  Shell         C:     C             C++:   C++
来源：http://oeo.cdnleiting.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://jur.ydjk.org.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://oss.yj20258.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://ymx.xziqi.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://fmv.ydzc1.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://gay.fengsongda.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://bjd.0kj1m.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://vuy.0kj1m.cn

【文件统计】
来源：http://mmy.vqdsnc.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://gli.fanxiaobao.xyz

--------------------------------------------------------------------------------
来源：http://qqr.gzhubu.top

目  录
来源：http://ppg.ydjk.org.cn

--------------------------------------------------------------------------------
来源：http://krl.kuanghao11.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://jjk.bjfxy.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://dji.hysaishi.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://msm.birdmap.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://xud.ppjwa.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://oob.meibo888.top


<!-- 参考信息 -->