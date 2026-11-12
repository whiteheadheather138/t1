代发 wailian999

[U19] Py：正则替换带回调
来源：http://fdl.guowangkeji.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://qlp.jianghu66.top

[U20] Py：缓存函数结果
来源：http://ipe.xuetiantiany.cn

@functools.lru_cache(maxsize=None)
来源：http://lnp.9152youxi.cn

[U21] Py：自定义上下文管理器
来源：http://cbw.fanxiaobao.xyz

@contextlib.contextmanager
来源：http://xzl.jqgufenzy.top

[U22] Py：矩阵转置
来源：http://cth.yuanzhike.top

list(zip(*m))
来源：http://jwy.dianchejie.cn

[U23] Py：分块读取大文件
来源：http://giv.jyoumei.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://ckc.jianghu66.top

[U24] Py：路径操作
来源：http://gcr.vqdsnc.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://dxu.hcnkem.com

[U25] Py：CSV 按字典读
来源：http://idx.xziqi.cn

csv.DictReader(f)
来源：http://xdt.gzhubu.top

[U26] Py：并发下载
来源：http://yyp.dianchejie.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://jib.fehbvm.com

[U27] Py：异步 HTTP
来源：http://bzr.nanxuanxn.top

aiohttp.ClientSession() 配合 async with
来源：http://caa.zhengqikj.top

[U28] Py：类型别名
来源：http://lbh.ywan-chungtsiang.top

UserId = int
来源：http://ajw.guowangkeji.top

[U29] Py：属性校验
来源：http://qvw.mhx1999.top

@property 与 @x.setter 配合
来源：http://ehl.epnwcf.com

[U30] Py：数据类
来源：http://onr.daxiang520.top

@dataclass(slots=True)
来源：http://cdq.zhixingplan.top

[U31] Py：单测
来源：http://uui.nanxuanxn.top

python -m pytest -q
来源：http://uvh.cheryme.top

[U32] Py：代码格式化
来源：http://ika.gogol.net.cn

ruff format . && ruff check --fix .
来源：http://stc.cheryme.top

[U33] Py：打包发布
来源：http://vou.52xcode.cn

python -m build  （依赖 pyproject.toml）
来源：http://fvk.yueranfly.top

[U34] Py：判断编码
来源：http://cmm.jqgufenzy.top

chardet.detect(raw)
来源：http://pdv.hywenlv.cn

[U35] Py：发送邮件
来源：http://jmj.shanyushiyangtech.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://ymv.gaohongyu789.top

[U36] Py：定时任务
来源：http://nrw.yangfankeji.com

schedule.every(10).minutes.do(job)
来源：http://qqg.cheryme.top

[U37] Py：读写 Excel
来源：http://eeo.aibaodan.cn

pandas.read_excel / DataFrame.to_excel
来源：http://bod.jinyuanbaomall.cn

[U38] Py：获取脚本所在目录
来源：http://lek.zdbjq.cn

Path(__file__).resolve().parent
来源：http://jez.cdnleiting.top

[U39] Py：判断是否在交互环境
来源：http://huo.tarul.cn

sys.stdout.isatty()
来源：http://jby.jinqigufen.top

[U40] Py：打印到标准错误
来源：http://cbj.redwolf501.top

print("err", file=sys.stderr)
来源：http://kub.jiagoushi.top

[U41] PHP：初始化 Composer 项目
来源：http://jxy.zhoulong.xyz

composer init;  composer require guzzlehttp/guzzle
来源：http://sjp.chenzaomai.com

[U42] PHP：PSR-4 自动加载
来源：http://kgs.gotoacloud.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://rgh.kuanghao11.cn

[U43] PHP：声明命名空间
来源：http://kbe.jinghuilouyu.cn

namespace App\Http;
来源：http://idm.redwolf501.top

[U44] PHP：开启严格类型
来源：http://net.fktsv.cn

declare(strict_types=1);
来源：http://pkm.vqdsnc.cn

[U45] PHP：类型声明与返回类型
来源：http://rmy.fzhhl.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://ctq.hammf.cn

[U46] PHP：可空类型
来源：http://tbg.shuidangran.top

?string $name = null
来源：http://jxm.feifeiyinyue.top

[U47] PHP：联合类型
来源：http://cyr.yuxming.cn

int|string $id
来源：http://rnq.chenzaomai.com

[U48] PHP：纯枚举
来源：http://kiw.zhijiandao.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://fhc.hammf.cn

[U49] PHP：只读属性
来源：http://uau.ydzc1.top

public readonly string $name
来源：http://qli.vehdjk.com

[U50] PHP：构造器属性提升
来源：http://fik.fengsongda.top

public function __construct(private int $id) {}
来源：http://ugl.zdbjq.cn

[U51] PHP：数组解构
来源：http://vto.feifeiyinyue.top

[$a, $b] = $arr;
来源：http://dxp.ybcxt.top

[U52] PHP：箭头函数
来源：http://odf.tianlin.xyz

$double = fn($x) => $x * 2;
来源：http://xry.sufxvd.cn

[U53] PHP：空合并运算符
来源：http://qws.zhijiandao.cn

$v = $a ?? $b ?? "default";
来源：http://jag.chenlongwang.top

[U54] PHP：空安全调用
来源：http://tvo.cucudq.cn

$obj?->method()
来源：http://wsf.jinqigfzy.top

[U55] PHP：match 表达式
来源：http://tkv.zhongyouzk.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://wak.jinqigufen.top

[U56] PHP：命名参数
来源：http://qxk.zhijiandao.cn

f(a: 1, b: 2)
来源：http://xai.epnwcf.com

[U57] PHP：字符串插值
来源：http://juk.zhongyouzk.top

"值: {$a}"
来源：http://jfq.daria6918.cn

[U58] PHP：数组三件套
来源：http://adw.fehbvm.com

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://jtr.ehwqpu.com

[U59] PHP：自定义排序
来源：http://yhy.snrcjt.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://qao.ybcxt.top

[U60] PHP：JSON 编解码
来源：http://wpd.svipenyu.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://pus.shzxlz.cn

[U61] PHP：正则
来源：http://roj.smart0.xyz

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://vik.zhijiandao.cn

[U62] PHP：日期对象
来源：http://vmz.zhaomingkeji.xyz

(new DateTimeImmutable())->format("Y-m-d");
来源：http://tbe.shanyushiyangkeji.top

[U63] PHP：文件读写
来源：http://rmv.hcnkem.com

file_get_contents($f);  file_put_contents($f, $data);
来源：http://xpf.xinyue.icu

[U64] PHP：目录遍历
来源：http://kyd.hfpthk.cn

glob("dir/*.php");  scandir("dir");
来源：http://caq.ivvv.top

[U65] PHP：会话
来源：http://dmo.gzhubu.top

session_start();  $_SESSION["uid"] = 1;
来源：http://shj.52xcode.cn

[U66] PHP：设置 Cookie
来源：http://yrv.sxryk.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://xtb.gzhubu.top

[U67] PHP：处理文件上传
来源：http://kcb.hfpthk.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://mcr.yongpay.top

[U68] PHP：PDO 连接
来源：http://vey.nanxuanxn.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://ruc.zhaomingkeji.xyz

[U69] PHP：PDO 预处理
来源：http://fmd.cheryme.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://jtw.ydjk.org.cn

[U70] PHP：PDO 事务
来源：http://gmy.jianghu66.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://eyp.pycfn.com

[U71] PHP：抛出异常
来源：http://gbl.kuanghao11.cn

throw new RuntimeException("失败", 500);
来源：http://fbs.fehbvm.com

[U72] PHP：写错误日志
来源：http://nlt.fengsongda.top

error_log("失败: " . $e->getMessage());
来源：http://ywg.zhixingplan.top

[U73] PHP：读取 ini 配置
来源：http://lez.fzhhl.top

parse_ini_file("config.ini", true)
来源：http://zcy.fengsongda.top

[U74] PHP：读取环境变量
来源：http://gwy.zdqjudy.top

getenv("APP_ENV") ?: "production"
来源：http://jfv.jianghu66.top

[U75] PHP：依赖注入
来源：http://nze.redwolf501.top

composer require psr/container
来源：http://afa.bbcook.cn

[U76] PHP：简单路由
来源：http://uvp.yueranfly.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://fli.ydjk.org.cn

[U77] PHP：模板渲染
来源：http://yve.hnqzz.top

composer require twig/twig
来源：http://kwt.jyoumei.cn

[U78] PHP：单元测试
来源：http://gnj.pengpengdd.cyou

composer require --dev phpunit/phpunit
来源：http://uzc.guannengcc.top

[U79] PHP：静态分析
来源：http://tjw.xziqi.cn

composer require --dev phpstan/phpstan
来源：http://tyb.bjfxy.top

[U80] PHP：代码规范修复
来源：http://mwy.ctjpmb.com

composer require --dev friendsofphp/php-cs-fixer
来源：http://voi.mhx1999.top

[U81] JS：初始化项目
来源：http://iwp.vqdsnc.cn

npm init -y;  npm i express
来源：http://ism.ehwqpu.com

[U82] JS：package.json 脚本
来源：http://qze.yj20258.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://ifl.meibo888.top

[U83] JS：ES Module 导入导出
来源：http://mug.havefunace.top

export const a = 1;  import { a } from "./m.js";
来源：http://wpe.quarkkingdee.top

[U84] JS：CommonJS 写法
来源：http://zsr.yuanzhike.top

module.exports = { a };  const { a } = require("./m");
来源：http://mmu.dianchejie.cn

[U85] JS：可选链
来源：http://gfn.havefunace.top

a?.b?.c
来源：http://rei.yongpay.top

[U86] JS：空值合并
来源：http://fnx.jinqigfzy.top

a ?? b
来源：http://lzr.xingfuxueyuan.xyz

[U87] JS：解构默认值
来源：http://nva.yongpay.top

const { a = 1, b = 2 } = obj;
来源：http://ikz.zycfv.cn

[U88] JS：对象展开合并
来源：http://pmh.jianghu66.top

{ ...a, ...b }
来源：http://rkf.redwolf501.top

[U89] JS：数组去重
来源：http://bug.havefunace.top

[...new Set(arr)]
来源：http://jao.yanxiufei.cn

[U90] JS：数字数组排序
来源：http://uxy.sufxvd.cn

[...arr].sort((a, b) => a - b)
来源：http://pxo.pycfn.com

[U91] JS：对象键值遍历
来源：http://bcc.ivvv.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://qiw.xinyue.icu

[U92] JS：深拷贝
来源：http://ajm.chenlongwang.top

structuredClone(obj)
来源：http://tqc.nanxuanxn.top

[U93] JS：模板字符串
来源：http://wjy.yvedp.cn

`共 ${n} 条`
来源：http://cqb.iojbl.cn

[U94] JS：箭头函数
来源：http://kdv.zdqjudy.top

const double = x => x * 2;
来源：http://esy.0kj1m.cn

[U95] JS：Promise 包装
来源：http://oyk.iojbl.cn

new Promise((resolve, reject) => {})
来源：http://qfc.hammf.cn

[U96] JS：async/await 与异常
来源：http://nie.tanke756.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hfv.zhongyouzk.top

[U97] JS：并发请求
来源：http://gde.jinqigufen.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://dyd.guowangkeji.top

[U98] JS：fetch 带 JSON
来源：http://mcd.yfazqb.com

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://oua.iojbl.cn

[U99] JS：事件监听
来源：http://kmm.chenzaomai.com

el.addEventListener("click", e => {})
来源：http://bei.hesvh.cn

[U100] JS：DOM 查询
来源：http://xrd.meibo888.top

document.querySelector(".item")
来源：http://gau.0kj1m.cn

[U101] JS：classList 操作
来源：http://pqq.fanxiaobao.xyz

el.classList.toggle("active")
来源：http://xyi.ydjk.org.cn

[U102] JS：本地存储
来源：http://ekj.quarkkingdee.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://rtg.pengpengdd.cyou

[U103] JS：定时器
来源：http://grh.yueranfly.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://qcs.pengpengdd.cyou

[U104] JS：防抖
来源：http://fsl.kuanghao11.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://nrc.yanxiufei.cn

[U105] JS：节流
来源：http://lua.nanxuanxn.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://bfx.chenzaomai.com

[U106] JS：日期格式化
来源：http://yev.yj20258888.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://phr.quarkkingdee.top

[U107] JS：数字千分位
来源：http://enp.sxryk.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://bfs.yuanzhike.top

[U108] JS：随机整数
来源：http://nrw.tanke756.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://akm.sufxvd.cn

[U109] JS：数组分组
来源：http://upi.gotoacloud.top

Object.groupBy(arr, x => x.type)
来源：http://bcl.guowangkeji.top

[U110] JS：数组分块
来源：http://jzq.dianchejie.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://vss.zhongyouzk.top

[U111] JS：对象转 Map
来源：http://jmf.xingfuxueyuan.xyz

new Map(Object.entries(obj))
来源：http://hmd.cqqwz.cn

[U112] JS：字符串补位
来源：http://gfq.redwolf501.top

"7".padStart(3, "0")
来源：http://bru.hongshengwenyu.top

[U113] JS：正则替换全部
来源：http://flt.xuanzx.com

s.replaceAll("a", "b")
来源：http://set.jyoumei.cn

[U114] JS：JSON 深比较
来源：http://vfc.cqqwz.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://qgp.nanxuanxn.top

[U115] JS：生成 UUID
来源：http://uka.hcnkem.com

crypto.randomUUID()
来源：http://cec.vqdsnc.cn

[U116] JS：类型检查（JSDoc）
来源：http://sob.gotoacloud.top

/** @param {string} name */ function f(name) {}
来源：http://nha.guowangkeji.top

[U117] JS：单元测试
来源：http://dgy.yongpay.top

npm i -D vitest;  npx vitest
来源：http://mny.gaohongyu789.top

[U118] JS：开发服务器
来源：http://too.vqdsnc.cn

npm i -D vite;  npx vite
来源：http://rcr.0kj1m.cn

[U119] JS：生产构建
来源：http://sio.zdqjudy.top

npx vite build
来源：http://wdm.zhengqikj.top

[U120] JS：读取环境变量（Vite）
来源：http://tfe.jinqigfzy.top

import.meta.env.VITE_API_URL
来源：http://uoa.meibo888.top

================================================================================
来源：http://bmn.ydzc1.top

统计汇总
来源：http://hsv.hcnkem.com

================================================================================
来源：http://ryi.aibaodan.cn

按语言统计（条）：
来源：http://lmj.quarkkingdee.top

Python ......... 252
来源：http://qnj.gogol.net.cn

PHP ............ 252
来源：http://slv.jinqigufen.top

JavaScript ..... 252
来源：http://qtw.yuxming.cn

TypeScript ..... 212
来源：http://izx.sysykeji.top

Java ........... 212
来源：http://hri.hywenlv.cn

Go ............. 212
来源：http://erj.hysaishi.cn

Ruby ........... 212
来源：http://rvq.tarul.cn

C# ............. 212
来源：http://ade.sjlbkw.cn

C .............. 30
来源：http://mml.tian-w.cn

C++ ............ 30
来源：http://cle.zhengqikj.top

SQL ............ 90
来源：http://rep.dianchejie.cn

Bash ........... 80
来源：http://oqf.tarul.cn

Kotlin ......... 15
来源：http://rlw.chenzaomai.com

Swift .......... 15
来源：http://bvn.cqqwz.cn

Lua ............ 10
来源：http://dcq.shuidangran.top

Perl ........... 10
来源：http://vvv.tian-w.cn

Scala .......... 10
来源：http://myc.yj202588.top

------------------------------------
来源：http://miq.mhx1999.top

合计 ........... 2106 条
来源：http://tnp.sufxvd.cn

按章节统计：
来源：http://mhw.cashguo.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://url.zhijiandao.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://iig.zdbjq.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://lqd.yfazqb.com

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://zxr.uphjek.com

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://kdz.haohaochexian.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://tmq.daria6918.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://amn.ehwqpu.com

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://svj.sufxvd.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://umi.fanxiaobao.xyz

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://cvo.smart0.xyz

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://dgf.316326.xyz

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://rcm.chenzaomai.com

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://bqn.ybcxt.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://zpy.zhengqikj.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://pqo.cashguo.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://boh.gzhubu.top

Q SQL 专题                              90
来源：http://wcd.zhaomingkeji.xyz

R Bash 专题                             80
来源：http://rna.shuidangran.top

S C / C++ 专题                          60
来源：http://wsq.ehwqpu.com

T 其他语言补充                          60
来源：http://usc.smart0.xyz

U 高频实用片段                         120
来源：http://fhd.yj202588.top

------------------------------------
来源：http://xec.shanyushiyangtech.top

合计                                  2106 条
来源：http://qqt.jinqigfzy.top

--------------------------------------------------------------------------------
来源：http://vhf.cqqwz.cn

使用提醒
来源：http://hzt.feifeiyinyue.top

--------------------------------------------------------------------------------
来源：http://cfr.fehbvm.com

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://rag.guowangkeji.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://qqr.redwolf501.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://zbp.zhixingplan.top

在旧版本上使用前请先确认语法支持情况。
来源：http://dsi.hnxiangtu.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://jzt.hnxiangtu.top

—— 文件结束 ——
来源：http://opj.jqgfzy.top

================================================================================
来源：http://yjp.aibaodan.cn

程序语言常见例子速查手册（2024 版）
来源：http://zwb.9152youxi.cn

Common Programming Examples Cheat Book
来源：http://iqv.9152youxi.cn

================================================================================
来源：http://dab.52xcode.cn

【收录内容】
来源：http://lyr.jinghuilouyu.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://ipp.shuidangran.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://xdc.sjlbkw.cn

SQL · Bash · C · C++
来源：http://rlu.yvedp.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://xmj.yongpay.top

【使用说明】
来源：http://khp.shangyingyoupin.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://jam.gaohongyu789.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://xgj.tianlin.xyz

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://bfr.kuanghao11.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://mqb.tianlin.xyz

Bash:  Shell         C:     C             C++:   C++
来源：http://jdw.bjfxy.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://cdp.gotoacloud.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://mge.pengpengdd.cyou

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://csg.quarkkingdee.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://lrk.fehbvm.com

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://sek.xingfuxueyuan.xyz

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://xum.sysykeji.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://pje.yvedp.cn

【文件统计】
来源：http://mgj.jqgufenzy.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://lwl.wangdashe.top

--------------------------------------------------------------------------------
来源：http://qiw.aibaodan.cn

目  录
来源：http://nxz.xuanzx.com

--------------------------------------------------------------------------------
来源：http://uld.nanxinkj.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://jvj.feifeiyinyue.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://eel.zhixingplan.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://uox.smart0.xyz

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://lsb.jinqigfzy.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://uxc.ywan-chungtsiang.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://waz.nwbrower.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://kjs.jyoumei.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://ggj.9152youxi.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://tvk.iojbl.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://abq.havefunace.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://krn.gzhubu.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://rze.ybcxt.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://vhw.nanxuanxn.top


<!-- 参考信息 -->