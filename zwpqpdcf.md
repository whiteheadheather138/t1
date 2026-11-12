代发 wailian999

[U19] Py：正则替换带回调
来源：http://swf.tanke756.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://qsb.hfpthk.cn

[U20] Py：缓存函数结果
来源：http://zwf.jinqigufen.top

@functools.lru_cache(maxsize=None)
来源：http://pay.cqqwz.cn

[U21] Py：自定义上下文管理器
来源：http://sal.yangfankeji.com

@contextlib.contextmanager
来源：http://haz.hysaishi.cn

[U22] Py：矩阵转置
来源：http://gtw.yfazqb.com

list(zip(*m))
来源：http://qxt.yueranfly.top

[U23] Py：分块读取大文件
来源：http://gvd.pengpengdd.cyou

for chunk in iter(lambda: f.read(8192), b""):
来源：http://lrs.c1oappe.top

[U24] Py：路径操作
来源：http://fcq.wangdashe.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://pha.zhaomingkeji.xyz

[U25] Py：CSV 按字典读
来源：http://vet.jlsjyb.cn

csv.DictReader(f)
来源：http://fwg.zdqjudy.top

[U26] Py：并发下载
来源：http://vex.bjfxy.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://gky.shzxlz.cn

[U27] Py：异步 HTTP
来源：http://kpi.gotoacloud.top

aiohttp.ClientSession() 配合 async with
来源：http://lve.zhoulong.xyz

[U28] Py：类型别名
来源：http://qwd.jiagoushi.top

UserId = int
来源：http://fam.jinqigufen.top

[U29] Py：属性校验
来源：http://kfc.hongshengwenyu.top

@property 与 @x.setter 配合
来源：http://oqo.zdqjudy.top

[U30] Py：数据类
来源：http://dyl.meibo888.top

@dataclass(slots=True)
来源：http://oxk.redwolf501.top

[U31] Py：单测
来源：http://qec.zhongyouzk.top

python -m pytest -q
来源：http://paz.yangfankeji.com

[U32] Py：代码格式化
来源：http://abd.chenzaomai.com

ruff format . && ruff check --fix .
来源：http://fdh.ehwqpu.com

[U33] Py：打包发布
来源：http://emf.ivvv.top

python -m build  （依赖 pyproject.toml）
来源：http://tvt.andypj.xyz

[U34] Py：判断编码
来源：http://lnk.dianchejie.cn

chardet.detect(raw)
来源：http://akn.xinyue.icu

[U35] Py：发送邮件
来源：http://wmb.jyoumei.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://ive.zdqjudy.top

[U36] Py：定时任务
来源：http://ddi.dashuyun.cn

schedule.every(10).minutes.do(job)
来源：http://pcu.daria6918.cn

[U37] Py：读写 Excel
来源：http://nkn.wangshuangyany.cn

pandas.read_excel / DataFrame.to_excel
来源：http://djj.vqdsnc.cn

[U38] Py：获取脚本所在目录
来源：http://xbu.cashguo.top

Path(__file__).resolve().parent
来源：http://zue.zhongyouzk.top

[U39] Py：判断是否在交互环境
来源：http://cif.ppjwa.cn

sys.stdout.isatty()
来源：http://ere.sxryk.cn

[U40] Py：打印到标准错误
来源：http://pam.redwolf501.top

print("err", file=sys.stderr)
来源：http://jsk.tarul.cn

[U41] PHP：初始化 Composer 项目
来源：http://tgb.jinyuanbaomall.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://tdw.meibo888.top

[U42] PHP：PSR-4 自动加载
来源：http://dts.ywan-chungtsiang.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://rrj.shzxlz.cn

[U43] PHP：声明命名空间
来源：http://xfx.quarkkingdee.top

namespace App\Http;
来源：http://nqk.zhaomingkeji.xyz

[U44] PHP：开启严格类型
来源：http://jyl.vqdsnc.cn

declare(strict_types=1);
来源：http://svv.jlsjyb.cn

[U45] PHP：类型声明与返回类型
来源：http://rjn.birdmap.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://ehl.sufxvd.cn

[U46] PHP：可空类型
来源：http://ofl.yangfankeji.com

?string $name = null
来源：http://bod.shzxlz.cn

[U47] PHP：联合类型
来源：http://lyo.chenlongwang.top

int|string $id
来源：http://ehf.dashuyun.cn

[U48] PHP：纯枚举
来源：http://muy.haohaochexian.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://xwb.jqgufenzy.top

[U49] PHP：只读属性
来源：http://jqe.feifeiyinyue.top

public readonly string $name
来源：http://iie.vqdsnc.cn

[U50] PHP：构造器属性提升
来源：http://ibd.fengsongda.top

public function __construct(private int $id) {}
来源：http://yuz.sufxvd.cn

[U51] PHP：数组解构
来源：http://xfc.yueranfly.top

[$a, $b] = $arr;
来源：http://rpm.zycfv.cn

[U52] PHP：箭头函数
来源：http://ikf.yanxiufei.cn

$double = fn($x) => $x * 2;
来源：http://qda.birdmap.top

[U53] PHP：空合并运算符
来源：http://zbn.fktsv.cn

$v = $a ?? $b ?? "default";
来源：http://kng.zhengqikj.top

[U54] PHP：空安全调用
来源：http://oln.pengpengdd.cyou

$obj?->method()
来源：http://pej.vqdsnc.cn

[U55] PHP：match 表达式
来源：http://htg.jyoumei.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://avz.cdnleiting.top

[U56] PHP：命名参数
来源：http://rru.sxryk.cn

f(a: 1, b: 2)
来源：http://uxa.cucudq.cn

[U57] PHP：字符串插值
来源：http://bqi.ybcxt.top

"值: {$a}"
来源：http://utj.xingfuxueyuan.xyz

[U58] PHP：数组三件套
来源：http://net.wangshuangyany.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://ptk.yongpay.top

[U59] PHP：自定义排序
来源：http://xxt.sysykeji.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://klb.xuetiantiany.cn

[U60] PHP：JSON 编解码
来源：http://zhp.yfazqb.com

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://btd.sysykeji.top

[U61] PHP：正则
来源：http://bfo.smart0.xyz

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://yst.gotoacloud.top

[U62] PHP：日期对象
来源：http://aue.yvedp.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://njq.zdbjq.cn

[U63] PHP：文件读写
来源：http://ltu.ybcxt.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hkt.zhixingplan.top

[U64] PHP：目录遍历
来源：http://pbb.fehbvm.com

glob("dir/*.php");  scandir("dir");
来源：http://lzf.yongpay.top

[U65] PHP：会话
来源：http://gqq.ywan-chungtsiang.top

session_start();  $_SESSION["uid"] = 1;
来源：http://fsi.ydzc1.top

[U66] PHP：设置 Cookie
来源：http://his.sufxvd.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://hmr.kuanghao11.cn

[U67] PHP：处理文件上传
来源：http://qlq.shzxlz.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://ker.aizwys.cn

[U68] PHP：PDO 连接
来源：http://yyk.pycfn.com

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://rai.gaohongyu789.top

[U69] PHP：PDO 预处理
来源：http://kfu.yanxiufei.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://jnl.fktsv.cn

[U70] PHP：PDO 事务
来源：http://fbf.hammf.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://tcd.fehbvm.com

[U71] PHP：抛出异常
来源：http://pul.ydzc1.top

throw new RuntimeException("失败", 500);
来源：http://bkd.daxiang520.top

[U72] PHP：写错误日志
来源：http://ejt.daxiang520.top

error_log("失败: " . $e->getMessage());
来源：http://qsq.ybcxt.top

[U73] PHP：读取 ini 配置
来源：http://xiq.jinghuilouyu.cn

parse_ini_file("config.ini", true)
来源：http://gaq.dianchejie.cn

[U74] PHP：读取环境变量
来源：http://nqk.havefunace.top

getenv("APP_ENV") ?: "production"
来源：http://cot.aizwys.cn

[U75] PHP：依赖注入
来源：http://qmu.ehwqpu.com

composer require psr/container
来源：http://ery.sufxvd.cn

[U76] PHP：简单路由
来源：http://lfl.zycfv.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://uel.sxryk.cn

[U77] PHP：模板渲染
来源：http://she.shangyingyoupin.top

composer require twig/twig
来源：http://uzv.iojbl.cn

[U78] PHP：单元测试
来源：http://lhl.smart0.xyz

composer require --dev phpunit/phpunit
来源：http://pqe.wangdashe.top

[U79] PHP：静态分析
来源：http://dut.jinghuilouyu.cn

composer require --dev phpstan/phpstan
来源：http://xay.zhaomingkeji.xyz

[U80] PHP：代码规范修复
来源：http://qei.shanyushiyangtech.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://rhz.xziqi.cn

[U81] JS：初始化项目
来源：http://emr.xuetiantiany.cn

npm init -y;  npm i express
来源：http://kjo.zhaomingkeji.xyz

[U82] JS：package.json 脚本
来源：http://gxw.chenzaomai.com

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://ket.birdmap.top

[U83] JS：ES Module 导入导出
来源：http://kva.ivvv.top

export const a = 1;  import { a } from "./m.js";
来源：http://gsf.nanxuanxn.top

[U84] JS：CommonJS 写法
来源：http://fke.fehbvm.com

module.exports = { a };  const { a } = require("./m");
来源：http://zav.chenjidiqi.icu

[U85] JS：可选链
来源：http://jmu.gaohongyu789.top

a?.b?.c
来源：http://smd.ywan-chungtsiang.top

[U86] JS：空值合并
来源：http://ple.daria6918.cn

a ?? b
来源：http://ajy.hfpthk.cn

[U87] JS：解构默认值
来源：http://kkw.jinqigufen.top

const { a = 1, b = 2 } = obj;
来源：http://pzz.ivvv.top

[U88] JS：对象展开合并
来源：http://xqk.guannengcc.top

{ ...a, ...b }
来源：http://otc.gaohongyu789.top

[U89] JS：数组去重
来源：http://zpm.snrcjt.cn

[...new Set(arr)]
来源：http://fnw.jinyuanbaomall.cn

[U90] JS：数字数组排序
来源：http://eli.smart0.xyz

[...arr].sort((a, b) => a - b)
来源：http://qik.jqgfzy.top

[U91] JS：对象键值遍历
来源：http://kis.pengpengdd.cyou

Object.entries(obj).forEach(([k, v]) => {});
来源：http://thk.ydzc1.top

[U92] JS：深拷贝
来源：http://eqs.yvedp.cn

structuredClone(obj)
来源：http://juw.yfazqb.com

[U93] JS：模板字符串
来源：http://xwz.zhijiandao.cn

`共 ${n} 条`
来源：http://sot.smart0.xyz

[U94] JS：箭头函数
来源：http://xvt.xuanzx.com

const double = x => x * 2;
来源：http://ful.xylfe.cn

[U95] JS：Promise 包装
来源：http://jpu.vqdsnc.cn

new Promise((resolve, reject) => {})
来源：http://muy.iojbl.cn

[U96] JS：async/await 与异常
来源：http://ene.xziqi.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://myw.xziqi.cn

[U97] JS：并发请求
来源：http://tuf.yj202588.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://izm.birdmap.top

[U98] JS：fetch 带 JSON
来源：http://goc.fktsv.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://jcv.mhx1999.top

[U99] JS：事件监听
来源：http://khy.havefunace.top

el.addEventListener("click", e => {})
来源：http://zdu.jinqigfzy.top

[U100] JS：DOM 查询
来源：http://chd.guannengcc.top

document.querySelector(".item")
来源：http://kby.hnxiangtu.top

[U101] JS：classList 操作
来源：http://nyq.xylfe.cn

el.classList.toggle("active")
来源：http://yze.snrcjt.cn

[U102] JS：本地存储
来源：http://als.daxiang520.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://gik.zhongyouzk.top

[U103] JS：定时器
来源：http://bzp.gogol.net.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://ble.jqgfzy.top

[U104] JS：防抖
来源：http://ypj.mhx1999.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mps.iojbl.cn

[U105] JS：节流
来源：http://ngu.pycfn.com

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://zsq.epnwcf.com

[U106] JS：日期格式化
来源：http://tue.havefunace.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://ewb.andypj.xyz

[U107] JS：数字千分位
来源：http://pnf.daria6918.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://nll.shangyingyoupin.top

[U108] JS：随机整数
来源：http://ucb.wangshuangyany.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://iyi.ywan-chungtsiang.top

[U109] JS：数组分组
来源：http://jfi.shuidangran.top

Object.groupBy(arr, x => x.type)
来源：http://qmg.nwbrower.top

[U110] JS：数组分块
来源：http://icx.ctjpmb.com

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://dcl.sufxvd.cn

[U111] JS：对象转 Map
来源：http://fhl.nanxinkj.top

new Map(Object.entries(obj))
来源：http://ums.shzxlz.cn

[U112] JS：字符串补位
来源：http://lea.fktsv.cn

"7".padStart(3, "0")
来源：http://zba.cqqwz.cn

[U113] JS：正则替换全部
来源：http://wra.hnqzz.top

s.replaceAll("a", "b")
来源：http://oyw.hcnkem.com

[U114] JS：JSON 深比较
来源：http://lqo.fengsongda.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://nru.uphjek.com

[U115] JS：生成 UUID
来源：http://iva.aibaodan.cn

crypto.randomUUID()
来源：http://vez.tian-w.cn

[U116] JS：类型检查（JSDoc）
来源：http://imb.tian-w.cn

/** @param {string} name */ function f(name) {}
来源：http://aky.yj202588.top

[U117] JS：单元测试
来源：http://tzf.pycfn.com

npm i -D vitest;  npx vitest
来源：http://kfx.hcnkem.com

[U118] JS：开发服务器
来源：http://uvo.kuanghao11.cn

npm i -D vite;  npx vite
来源：http://ezk.c1oappe.top

[U119] JS：生产构建
来源：http://iqt.epnwcf.com

npx vite build
来源：http://vzy.jiagoushi.top

[U120] JS：读取环境变量（Vite）
来源：http://hny.andypj.xyz

import.meta.env.VITE_API_URL
来源：http://rkn.hywenlv.cn

================================================================================
来源：http://wdc.jianghu66.top

统计汇总
来源：http://wxh.zhoulong.xyz

================================================================================
来源：http://nnn.tarul.cn

按语言统计（条）：
来源：http://bed.xingfuxueyuan.xyz

Python ......... 252
来源：http://xqy.uphjek.com

PHP ............ 252
来源：http://mvx.hfpthk.cn

JavaScript ..... 252
来源：http://luo.yuanzhike.top

TypeScript ..... 212
来源：http://gkl.shanyushiyangtech.top

Java ........... 212
来源：http://lyh.xingfuxueyuan.xyz

Go ............. 212
来源：http://zty.epnwcf.com

Ruby ........... 212
来源：http://ife.daxiang520.top

C# ............. 212
来源：http://zup.c1oappe.top

C .............. 30
来源：http://rtv.dashuyun.cn

C++ ............ 30
来源：http://jaa.jinyuanbaomall.cn

SQL ............ 90
来源：http://ric.cqqwz.cn

Bash ........... 80
来源：http://dqf.epnwcf.com

Kotlin ......... 15
来源：http://sss.wangdashe.top

Swift .......... 15
来源：http://zfg.epnwcf.com

Lua ............ 10
来源：http://pyc.bbcook.cn

Perl ........... 10
来源：http://xoz.guannengcc.top

Scala .......... 10
来源：http://vta.gaohongyu789.top

------------------------------------
来源：http://ezy.yongpay.top

合计 ........... 2106 条
来源：http://ysp.andypj.xyz

按章节统计：
来源：http://olm.hnxiangtu.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://urv.snrcjt.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://ytg.smart0.xyz

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://qft.hesvh.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://fqh.tarul.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://thv.gaohongyu789.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://lgo.gogol.net.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://nzw.cucudq.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://fgf.c1oappe.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://hea.shanyushiyangkeji.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://tjw.redwolf501.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://lfj.hongshengwenyu.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://qwx.wangshuangyany.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://ncx.guowangkeji.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://ffa.svipenyu.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://qiv.fzhhl.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://ahl.meibo888.top

Q SQL 专题                              90
来源：http://qpi.meibo888.top

R Bash 专题                             80
来源：http://spk.fzhhl.top

S C / C++ 专题                          60
来源：http://egw.epnwcf.com

T 其他语言补充                          60
来源：http://oqs.yuxming.cn

U 高频实用片段                         120
来源：http://fhq.guowangkeji.top

------------------------------------
来源：http://bkh.jqgufenzy.top

合计                                  2106 条
来源：http://nvv.zhixingplan.top

--------------------------------------------------------------------------------
来源：http://zya.sysykeji.top

使用提醒
来源：http://lxi.hywenlv.cn

--------------------------------------------------------------------------------
来源：http://crd.c1oappe.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://szn.shuidangran.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://vrz.jinyuanbaomall.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://bft.yuxming.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://gyj.gogol.net.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://hkj.hammf.cn

—— 文件结束 ——
来源：http://tkr.gaohongyu789.top

================================================================================
来源：http://xot.tarul.cn

程序语言常见例子速查手册（2024 版）
来源：http://nmx.hnqzz.top

Common Programming Examples Cheat Book
来源：http://qzi.nwbrower.top

================================================================================
来源：http://pvf.iojbl.cn

【收录内容】
来源：http://bsi.yueranfly.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://vtn.zhiwuduotai.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://byu.jqgfzy.top

SQL · Bash · C · C++
来源：http://vwh.yangfankeji.com

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://coq.birdmap.top

【使用说明】
来源：http://chr.xylfe.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://qri.dashuyun.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://nxd.sxryk.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://wpm.cashguo.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://yca.uphjek.com

Bash:  Shell         C:     C             C++:   C++
来源：http://rvq.guowangkeji.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://loy.zhijiandao.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://azo.yonumen.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://wvf.yangfankeji.com

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://qxg.havefunace.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://gnq.yfazqb.com

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://sjw.yfazqb.com

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://paa.quarkkingdee.top

【文件统计】
来源：http://yoj.havefunace.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://utm.hnxiangtu.top

--------------------------------------------------------------------------------
来源：http://nfy.ivvv.top

目  录
来源：http://abs.fanxiaobao.xyz

--------------------------------------------------------------------------------
来源：http://ttl.sjlbkw.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://nzc.yj20258888.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://yri.sjlbkw.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://mme.redwolf501.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://aht.sufxvd.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://ymb.ppjwa.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://zzq.sweek.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://red.tianlin.xyz

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://avp.epnwcf.com

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://cgg.vqdsnc.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://uxn.ppjwa.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://kbo.zhongyouzk.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://iye.chenlongwang.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://vkz.ctjpmb.com


<!-- 参考信息 -->