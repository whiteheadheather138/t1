代发 wailian999

[U21] Py：自定义上下文管理器
来源：http://doa.fktsv.cn

@contextlib.contextmanager
来源：http://cxj.vehdjk.com

[U22] Py：矩阵转置
来源：http://hhx.smart0.xyz

list(zip(*m))
来源：http://bfz.gzhubu.top

[U23] Py：分块读取大文件
来源：http://idk.nwbrower.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://lpr.aibaodan.cn

[U24] Py：路径操作
来源：http://quc.yuxming.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://aem.fktsv.cn

[U25] Py：CSV 按字典读
来源：http://nbi.fehbvm.com

csv.DictReader(f)
来源：http://plk.gotoacloud.top

[U26] Py：并发下载
来源：http://duo.cqqwz.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://fgq.fehbvm.com

[U27] Py：异步 HTTP
来源：http://iid.jianghu66.top

aiohttp.ClientSession() 配合 async with
来源：http://ffa.birdmap.top

[U28] Py：类型别名
来源：http://zdv.sysykeji.top

UserId = int
来源：http://dzq.jinqigfzy.top

[U29] Py：属性校验
来源：http://bvr.fanxiaobao.xyz

@property 与 @x.setter 配合
来源：http://lqn.ywan-chungtsiang.top

[U30] Py：数据类
来源：http://lzi.sufxvd.cn

@dataclass(slots=True)
来源：http://sti.hnxiangtu.top

[U31] Py：单测
来源：http://kci.hysaishi.cn

python -m pytest -q
来源：http://gff.fehbvm.com

[U32] Py：代码格式化
来源：http://dud.fanxiaobao.xyz

ruff format . && ruff check --fix .
来源：http://soq.xingfuxueyuan.xyz

[U33] Py：打包发布
来源：http://div.ctjpmb.com

python -m build  （依赖 pyproject.toml）
来源：http://upx.sufxvd.cn

[U34] Py：判断编码
来源：http://nzc.0kj1m.cn

chardet.detect(raw)
来源：http://fzp.ivvv.top

[U35] Py：发送邮件
来源：http://kju.yonumen.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://apd.sufxvd.cn

[U36] Py：定时任务
来源：http://mes.yfazqb.com

schedule.every(10).minutes.do(job)
来源：http://gcj.chenjidiqi.icu

[U37] Py：读写 Excel
来源：http://vwl.tanke756.top

pandas.read_excel / DataFrame.to_excel
来源：http://rly.nwbrower.top

[U38] Py：获取脚本所在目录
来源：http://dbp.xziqi.cn

Path(__file__).resolve().parent
来源：http://mih.tarul.cn

[U39] Py：判断是否在交互环境
来源：http://iol.hnqzz.top

sys.stdout.isatty()
来源：http://ndd.zhoulong.xyz

[U40] Py：打印到标准错误
来源：http://mzm.0kj1m.cn

print("err", file=sys.stderr)
来源：http://jxb.ydzc1.top

[U41] PHP：初始化 Composer 项目
来源：http://wit.shanyushiyangtech.top

composer init;  composer require guzzlehttp/guzzle
来源：http://ckp.jianghu66.top

[U42] PHP：PSR-4 自动加载
来源：http://llq.epnwcf.com

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://vqd.xuanzx.com

[U43] PHP：声明命名空间
来源：http://qcc.aibaodan.cn

namespace App\Http;
来源：http://xhj.cucudq.cn

[U44] PHP：开启严格类型
来源：http://ahp.jianghu66.top

declare(strict_types=1);
来源：http://evo.jiagoushi.top

[U45] PHP：类型声明与返回类型
来源：http://eum.shanyushiyangtech.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://vzb.yj20258888.top

[U46] PHP：可空类型
来源：http://pve.xylfe.cn

?string $name = null
来源：http://jlt.nwbrower.top

[U47] PHP：联合类型
来源：http://iiu.fzhhl.top

int|string $id
来源：http://ktu.hnxiangtu.top

[U48] PHP：纯枚举
来源：http://trn.chenlongwang.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://ber.svipenyu.cn

[U49] PHP：只读属性
来源：http://mlf.cashguo.top

public readonly string $name
来源：http://tms.chenlongwang.top

[U50] PHP：构造器属性提升
来源：http://ndu.andypj.xyz

public function __construct(private int $id) {}
来源：http://nko.ehwqpu.com

[U51] PHP：数组解构
来源：http://gpx.jinghuilouyu.cn

[$a, $b] = $arr;
来源：http://kas.cashguo.top

[U52] PHP：箭头函数
来源：http://cvy.chenjidiqi.icu

$double = fn($x) => $x * 2;
来源：http://anh.xinyue.icu

[U53] PHP：空合并运算符
来源：http://lsh.sufxvd.cn

$v = $a ?? $b ?? "default";
来源：http://tes.zhengqikj.top

[U54] PHP：空安全调用
来源：http://rff.zdbjq.cn

$obj?->method()
来源：http://ruc.yanxiufei.cn

[U55] PHP：match 表达式
来源：http://atp.yj20258888.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://vdv.gaohongyu789.top

[U56] PHP：命名参数
来源：http://ppe.c1oappe.top

f(a: 1, b: 2)
来源：http://kwj.hysaishi.cn

[U57] PHP：字符串插值
来源：http://kpj.cheryme.top

"值: {$a}"
来源：http://vqp.smart0.xyz

[U58] PHP：数组三件套
来源：http://pja.zdbjq.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://pfz.guannengcc.top

[U59] PHP：自定义排序
来源：http://owy.ywan-chungtsiang.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://kxv.yanxiufei.cn

[U60] PHP：JSON 编解码
来源：http://czj.wangdashe.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://qgy.yonumen.top

[U61] PHP：正则
来源：http://okr.xuetiantiany.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://wmf.zhaomingkeji.xyz

[U62] PHP：日期对象
来源：http://uad.gotoacloud.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://sei.shzxlz.cn

[U63] PHP：文件读写
来源：http://hjq.ctjpmb.com

file_get_contents($f);  file_put_contents($f, $data);
来源：http://etm.aizwys.cn

[U64] PHP：目录遍历
来源：http://btf.yonumen.top

glob("dir/*.php");  scandir("dir");
来源：http://ifv.vehdjk.com

[U65] PHP：会话
来源：http://qcc.fanxiaobao.xyz

session_start();  $_SESSION["uid"] = 1;
来源：http://lcw.yvedp.cn

[U66] PHP：设置 Cookie
来源：http://bsy.zdqjudy.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://vle.iojbl.cn

[U67] PHP：处理文件上传
来源：http://vqg.zhiwuduotai.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://ikw.xziqi.cn

[U68] PHP：PDO 连接
来源：http://ghj.shanyushiyangkeji.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://luc.gzhubu.top

[U69] PHP：PDO 预处理
来源：http://mrz.fanxiaobao.xyz

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://kyf.xuetiantiany.cn

[U70] PHP：PDO 事务
来源：http://ojx.iojbl.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://rta.daxiang520.top

[U71] PHP：抛出异常
来源：http://boa.fehbvm.com

throw new RuntimeException("失败", 500);
来源：http://zfm.jqgfzy.top

[U72] PHP：写错误日志
来源：http://vmv.zdqjudy.top

error_log("失败: " . $e->getMessage());
来源：http://jhs.zhongyouzk.top

[U73] PHP：读取 ini 配置
来源：http://bzq.aizwys.cn

parse_ini_file("config.ini", true)
来源：http://zul.dianchejie.cn

[U74] PHP：读取环境变量
来源：http://xkm.wangshuangyany.cn

getenv("APP_ENV") ?: "production"
来源：http://xhr.jlsjyb.cn

[U75] PHP：依赖注入
来源：http://hzh.zhongyouzk.top

composer require psr/container
来源：http://tmn.zdqjudy.top

[U76] PHP：简单路由
来源：http://kgb.kuanghao11.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://nmi.jiagoushi.top

[U77] PHP：模板渲染
来源：http://bse.jinghuilouyu.cn

composer require twig/twig
来源：http://syl.redwolf501.top

[U78] PHP：单元测试
来源：http://xsu.hfpthk.cn

composer require --dev phpunit/phpunit
来源：http://oiu.hfpthk.cn

[U79] PHP：静态分析
来源：http://kxy.gotoacloud.top

composer require --dev phpstan/phpstan
来源：http://kco.jlsjyb.cn

[U80] PHP：代码规范修复
来源：http://hpm.hnqzz.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://qne.smart0.xyz

[U81] JS：初始化项目
来源：http://nrm.hesvh.cn

npm init -y;  npm i express
来源：http://ool.cdnleiting.top

[U82] JS：package.json 脚本
来源：http://frp.chenzaomai.com

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://fgs.nanxinkj.top

[U83] JS：ES Module 导入导出
来源：http://gau.fehbvm.com

export const a = 1;  import { a } from "./m.js";
来源：http://pto.52xcode.cn

[U84] JS：CommonJS 写法
来源：http://dml.ivvv.top

module.exports = { a };  const { a } = require("./m");
来源：http://vsd.hysaishi.cn

[U85] JS：可选链
来源：http://izb.shzxlz.cn

a?.b?.c
来源：http://dyl.svipenyu.cn

[U86] JS：空值合并
来源：http://fzq.redwolf501.top

a ?? b
来源：http://pab.gogol.net.cn

[U87] JS：解构默认值
来源：http://eto.tanke756.top

const { a = 1, b = 2 } = obj;
来源：http://xov.shuidangran.top

[U88] JS：对象展开合并
来源：http://oab.snrcjt.cn

{ ...a, ...b }
来源：http://yog.chenzaomai.com

[U89] JS：数组去重
来源：http://ulh.ydzc1.top

[...new Set(arr)]
来源：http://tbt.tianlin.xyz

[U90] JS：数字数组排序
来源：http://ggf.hfpthk.cn

[...arr].sort((a, b) => a - b)
来源：http://zzl.xingfuxueyuan.xyz

[U91] JS：对象键值遍历
来源：http://inu.svipenyu.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://vsz.cheryme.top

[U92] JS：深拷贝
来源：http://iar.hysaishi.cn

structuredClone(obj)
来源：http://hup.ydjk.org.cn

[U93] JS：模板字符串
来源：http://dnl.zhoulong.xyz

`共 ${n} 条`
来源：http://fml.jinqigufen.top

[U94] JS：箭头函数
来源：http://zkf.ydjk.org.cn

const double = x => x * 2;
来源：http://jiz.daxiang520.top

[U95] JS：Promise 包装
来源：http://vji.ydjk.org.cn

new Promise((resolve, reject) => {})
来源：http://twp.yongpay.top

[U96] JS：async/await 与异常
来源：http://gwq.fehbvm.com

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://osw.fktsv.cn

[U97] JS：并发请求
来源：http://rul.pengpengdd.cyou

await Promise.all(urls.map(u => fetch(u)))
来源：http://vpy.c1oappe.top

[U98] JS：fetch 带 JSON
来源：http://lpc.smart0.xyz

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://mhp.shuidangran.top

[U99] JS：事件监听
来源：http://eyr.jqgfzy.top

el.addEventListener("click", e => {})
来源：http://xts.tarul.cn

[U100] JS：DOM 查询
来源：http://lbv.shuidangran.top

document.querySelector(".item")
来源：http://sge.ivvv.top

[U101] JS：classList 操作
来源：http://ldj.shuidangran.top

el.classList.toggle("active")
来源：http://jqi.nwbrower.top

[U102] JS：本地存储
来源：http://zin.yj20258.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://wgh.havefunace.top

[U103] JS：定时器
来源：http://edo.haohaochexian.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://atl.ybcxt.top

[U104] JS：防抖
来源：http://lre.sufxvd.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://yif.xziqi.cn

[U105] JS：节流
来源：http://oyc.9152youxi.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://xas.jinqigfzy.top

[U106] JS：日期格式化
来源：http://ydr.haohaochexian.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://pfq.gotoacloud.top

[U107] JS：数字千分位
来源：http://sis.sweek.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://okp.yangfankeji.com

[U108] JS：随机整数
来源：http://lgm.chenzaomai.com

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://gth.zhongyouzk.top

[U109] JS：数组分组
来源：http://tbi.zdbjq.cn

Object.groupBy(arr, x => x.type)
来源：http://eey.jlsjyb.cn

[U110] JS：数组分块
来源：http://ywm.zhiwuduotai.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://czm.tanke756.top

[U111] JS：对象转 Map
来源：http://aqd.havefunace.top

new Map(Object.entries(obj))
来源：http://hgq.0kj1m.cn

[U112] JS：字符串补位
来源：http://usi.zhijiandao.cn

"7".padStart(3, "0")
来源：http://rtv.0kj1m.cn

[U113] JS：正则替换全部
来源：http://rcj.sufxvd.cn

s.replaceAll("a", "b")
来源：http://ibs.daria6918.cn

[U114] JS：JSON 深比较
来源：http://kco.ybcxt.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://jmj.jinyuanbaomall.cn

[U115] JS：生成 UUID
来源：http://est.zhoulong.xyz

crypto.randomUUID()
来源：http://gvd.aizwys.cn

[U116] JS：类型检查（JSDoc）
来源：http://fyv.wangshuangyany.cn

/** @param {string} name */ function f(name) {}
来源：http://zhu.yangfankeji.com

[U117] JS：单元测试
来源：http://vyy.hnxiangtu.top

npm i -D vitest;  npx vitest
来源：http://bpd.xuanzx.com

[U118] JS：开发服务器
来源：http://dkr.daxiang520.top

npm i -D vite;  npx vite
来源：http://lwe.zhoulong.xyz

[U119] JS：生产构建
来源：http://gmp.hywenlv.cn

npx vite build
来源：http://jhs.316326.xyz

[U120] JS：读取环境变量（Vite）
来源：http://mii.yvedp.cn

import.meta.env.VITE_API_URL
来源：http://wig.fktsv.cn

================================================================================
来源：http://alq.yj20258888.top

统计汇总
来源：http://vxr.ybcxt.top

================================================================================
来源：http://num.ybcxt.top

按语言统计（条）：
来源：http://sxz.zdqjudy.top

Python ......... 252
来源：http://urh.ctjpmb.com

PHP ............ 252
来源：http://wjo.mhx1999.top

JavaScript ..... 252
来源：http://cml.chenzaomai.com

TypeScript ..... 212
来源：http://hcb.nanxuanxn.top

Java ........... 212
来源：http://qxz.yfazqb.com

Go ............. 212
来源：http://dpf.wangdashe.top

Ruby ........... 212
来源：http://uvq.yangfankeji.com

C# ............. 212
来源：http://etm.dashuyun.cn

C .............. 30
来源：http://zhf.sxryk.cn

C++ ............ 30
来源：http://ijk.hfpthk.cn

SQL ............ 90
来源：http://ade.cqqwz.cn

Bash ........... 80
来源：http://tnk.shuidangran.top

Kotlin ......... 15
来源：http://ifq.meibo888.top

Swift .......... 15
来源：http://xxq.zhengqikj.top

Lua ............ 10
来源：http://kac.guowangkeji.top

Perl ........... 10
来源：http://xyn.9152youxi.cn

Scala .......... 10
来源：http://tvh.dianchejie.cn

------------------------------------
来源：http://tmr.hnqzz.top

合计 ........... 2106 条
来源：http://mgl.gotoacloud.top

按章节统计：
来源：http://gfa.zhixingplan.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://maa.zhoulong.xyz

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://lxq.9152youxi.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://kqh.9152youxi.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://sfr.mhx1999.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://xnr.dashuyun.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://zsj.fzhhl.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://lqj.hesvh.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://htl.pengpengdd.cyou

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://wpt.tian-w.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://mru.fktsv.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://grq.guowangkeji.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://onm.hongshengwenyu.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://utt.hammf.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://gck.tarul.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://tzx.hywenlv.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://bsk.wangshuangyany.cn

Q SQL 专题                              90
来源：http://sfa.mhx1999.top

R Bash 专题                             80
来源：http://hmz.tianlin.xyz

S C / C++ 专题                          60
来源：http://hih.52xcode.cn

T 其他语言补充                          60
来源：http://tav.havefunace.top

U 高频实用片段                         120
来源：http://slw.shzxlz.cn

------------------------------------
来源：http://lpv.svipenyu.cn

合计                                  2106 条
来源：http://qil.jqgfzy.top

--------------------------------------------------------------------------------
来源：http://tvt.daria6918.cn

使用提醒
来源：http://vjw.yongpay.top

--------------------------------------------------------------------------------
来源：http://iyd.pengpengdd.cyou

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://yvp.cqqwz.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://mdp.hnqzz.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://hmz.ehwqpu.com

在旧版本上使用前请先确认语法支持情况。
来源：http://nof.shuidangran.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://awe.daria6918.cn

—— 文件结束 ——
来源：http://pcj.nanxuanxn.top

================================================================================
来源：http://qia.xylfe.cn

程序语言常见例子速查手册（2024 版）
来源：http://zqy.sweek.top

Common Programming Examples Cheat Book
来源：http://qfa.hesvh.cn

================================================================================
来源：http://kti.yj20258888.top

【收录内容】
来源：http://mxg.ybcxt.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://ktf.xingfuxueyuan.xyz

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://idp.zhijiandao.cn

SQL · Bash · C · C++
来源：http://hkw.daria6918.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://tru.zhaomingkeji.xyz

【使用说明】
来源：http://nsm.tian-w.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://lqa.ivvv.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://vdy.52xcode.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://hvw.9152youxi.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://pot.zhixingplan.top

Bash:  Shell         C:     C             C++:   C++
来源：http://hld.zdqjudy.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://dhx.9152youxi.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://oed.cdnleiting.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://qqs.c1oappe.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://qmi.uphjek.com

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://zzd.ydzc1.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://phw.guowangkeji.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://mej.hongshengwenyu.top

【文件统计】
来源：http://byq.shzxlz.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://iya.zhongyouzk.top

--------------------------------------------------------------------------------
来源：http://iyk.jqgfzy.top

目  录
来源：http://afq.chenjidiqi.icu

--------------------------------------------------------------------------------
来源：http://oxd.vehdjk.com

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://bzi.daxiang520.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://cjz.hnqzz.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://nyq.yangfankeji.com

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://xlv.ywan-chungtsiang.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://grx.shangyingyoupin.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://wme.dashuyun.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://oat.yvedp.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://nck.zdbjq.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://xij.hysaishi.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://aex.quarkkingdee.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://spb.jiagoushi.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://yhw.guannengcc.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://aye.xingfuxueyuan.xyz

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://lyj.52xcode.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://kyp.tian-w.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://fka.fehbvm.com

Q. SQL 专题                    （第 17 节，90 条）
来源：http://jaj.yj20258888.top


<!-- 参考信息 -->