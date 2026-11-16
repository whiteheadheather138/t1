代发 wailian999

[U17] Py：初始化日志
来源：http://fug.chenlongwang.top

logging.basicConfig(level=logging.INFO)
来源：http://lnt.ybcxt.top

[U18] Py：预编译正则
来源：http://jou.jinqigfzy.top

pat = re.compile(r"\d+")
来源：http://lnu.cdnleiting.top

[U19] Py：正则替换带回调
来源：http://jjn.bbcook.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://uev.kuanghao11.cn

[U20] Py：缓存函数结果
来源：http://qhc.xuanzx.com

@functools.lru_cache(maxsize=None)
来源：http://mnd.yuxming.cn

[U21] Py：自定义上下文管理器
来源：http://azn.hfpthk.cn

@contextlib.contextmanager
来源：http://fdl.zhaomingkeji.xyz

[U22] Py：矩阵转置
来源：http://oqv.aibaodan.cn

list(zip(*m))
来源：http://mjg.birdmap.top

[U23] Py：分块读取大文件
来源：http://qoi.wangdashe.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://zzr.fengsongda.top

[U24] Py：路径操作
来源：http://vlh.zdqjudy.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://fmg.yanxiufei.cn

[U25] Py：CSV 按字典读
来源：http://fgs.yonumen.top

csv.DictReader(f)
来源：http://kcl.jlsjyb.cn

[U26] Py：并发下载
来源：http://dng.sweek.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://jdq.fanxiaobao.xyz

[U27] Py：异步 HTTP
来源：http://fji.ydjk.org.cn

aiohttp.ClientSession() 配合 async with
来源：http://yak.feifeiyinyue.top

[U28] Py：类型别名
来源：http://upq.9152youxi.cn

UserId = int
来源：http://tqy.xziqi.cn

[U29] Py：属性校验
来源：http://mxm.9152youxi.cn

@property 与 @x.setter 配合
来源：http://zik.zdbjq.cn

[U30] Py：数据类
来源：http://pkz.tanke756.top

@dataclass(slots=True)
来源：http://lwx.hongshengwenyu.top

[U31] Py：单测
来源：http://kkj.9152youxi.cn

python -m pytest -q
来源：http://era.jinqigfzy.top

[U32] Py：代码格式化
来源：http://eap.hnqzz.top

ruff format . && ruff check --fix .
来源：http://rtd.jiagoushi.top

[U33] Py：打包发布
来源：http://srg.tarul.cn

python -m build  （依赖 pyproject.toml）
来源：http://lyy.zhiwuduotai.top

[U34] Py：判断编码
来源：http://dcl.jinqigufen.top

chardet.detect(raw)
来源：http://qaj.xingfuxueyuan.xyz

[U35] Py：发送邮件
来源：http://ffc.gogol.net.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://udi.gogol.net.cn

[U36] Py：定时任务
来源：http://sbs.hammf.cn

schedule.every(10).minutes.do(job)
来源：http://van.birdmap.top

[U37] Py：读写 Excel
来源：http://jmr.daxiang520.top

pandas.read_excel / DataFrame.to_excel
来源：http://jzn.dashuyun.cn

[U38] Py：获取脚本所在目录
来源：http://pfb.nanxuanxn.top

Path(__file__).resolve().parent
来源：http://cdg.hywenlv.cn

[U39] Py：判断是否在交互环境
来源：http://pdo.fzhhl.top

sys.stdout.isatty()
来源：http://zwp.jlsjyb.cn

[U40] Py：打印到标准错误
来源：http://ieh.daxiang520.top

print("err", file=sys.stderr)
来源：http://kuy.52xcode.cn

[U41] PHP：初始化 Composer 项目
来源：http://zgi.ctjpmb.com

composer init;  composer require guzzlehttp/guzzle
来源：http://zop.fzhhl.top

[U42] PHP：PSR-4 自动加载
来源：http://eha.hammf.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://gvo.zhijiandao.cn

[U43] PHP：声明命名空间
来源：http://ipe.zhiwuduotai.top

namespace App\Http;
来源：http://wyn.chenlongwang.top

[U44] PHP：开启严格类型
来源：http://mmq.zycfv.cn

declare(strict_types=1);
来源：http://cpd.svipenyu.cn

[U45] PHP：类型声明与返回类型
来源：http://jnt.jqgfzy.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://ltp.fktsv.cn

[U46] PHP：可空类型
来源：http://noo.ydjk.org.cn

?string $name = null
来源：http://rwq.guannengcc.top

[U47] PHP：联合类型
来源：http://xch.jiagoushi.top

int|string $id
来源：http://mme.jqgfzy.top

[U48] PHP：纯枚举
来源：http://inw.shanyushiyangtech.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hia.cashguo.top

[U49] PHP：只读属性
来源：http://nii.sufxvd.cn

public readonly string $name
来源：http://geg.c1oappe.top

[U50] PHP：构造器属性提升
来源：http://grl.cdnleiting.top

public function __construct(private int $id) {}
来源：http://jxr.jinyuanbaomall.cn

[U51] PHP：数组解构
来源：http://cbc.jyoumei.cn

[$a, $b] = $arr;
来源：http://pgd.nwbrower.top

[U52] PHP：箭头函数
来源：http://cze.uphjek.com

$double = fn($x) => $x * 2;
来源：http://xgd.xziqi.cn

[U53] PHP：空合并运算符
来源：http://lpp.daxiang520.top

$v = $a ?? $b ?? "default";
来源：http://rbd.cheryme.top

[U54] PHP：空安全调用
来源：http://dng.epnwcf.com

$obj?->method()
来源：http://pty.wangshuangyany.cn

[U55] PHP：match 表达式
来源：http://ioj.hysaishi.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://bbh.ehwqpu.com

[U56] PHP：命名参数
来源：http://lec.jiagoushi.top

f(a: 1, b: 2)
来源：http://ixq.fzhhl.top

[U57] PHP：字符串插值
来源：http://fdc.zycfv.cn

"值: {$a}"
来源：http://xon.zdbjq.cn

[U58] PHP：数组三件套
来源：http://hcu.pycfn.com

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://jjc.zhiwuduotai.top

[U59] PHP：自定义排序
来源：http://hli.nanxuanxn.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://bvd.nanxuanxn.top

[U60] PHP：JSON 编解码
来源：http://uzl.aizwys.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://xbw.epnwcf.com

[U61] PHP：正则
来源：http://ndb.jlsjyb.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://fqq.xylfe.cn

[U62] PHP：日期对象
来源：http://vqa.cheryme.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://qul.cdnleiting.top

[U63] PHP：文件读写
来源：http://etn.zhongyouzk.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://qen.zhongyouzk.top

[U64] PHP：目录遍历
来源：http://jlr.9152youxi.cn

glob("dir/*.php");  scandir("dir");
来源：http://rrb.hnxiangtu.top

[U65] PHP：会话
来源：http://qlw.jlsjyb.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://ruw.smart0.xyz

[U66] PHP：设置 Cookie
来源：http://jdv.yonumen.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://brw.bjfxy.top

[U67] PHP：处理文件上传
来源：http://cfu.c1oappe.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://bjh.bbcook.cn

[U68] PHP：PDO 连接
来源：http://gjr.hysaishi.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://wwl.zdqjudy.top

[U69] PHP：PDO 预处理
来源：http://imy.svipenyu.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://erd.nanxinkj.top

[U70] PHP：PDO 事务
来源：http://tzr.vqdsnc.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://stf.ywan-chungtsiang.top

[U71] PHP：抛出异常
来源：http://nhk.jqgufenzy.top

throw new RuntimeException("失败", 500);
来源：http://tto.wangshuangyany.cn

[U72] PHP：写错误日志
来源：http://mnh.fengsongda.top

error_log("失败: " . $e->getMessage());
来源：http://kqi.hesvh.cn

[U73] PHP：读取 ini 配置
来源：http://avt.jqgfzy.top

parse_ini_file("config.ini", true)
来源：http://ypb.xinyue.icu

[U74] PHP：读取环境变量
来源：http://fiq.guowangkeji.top

getenv("APP_ENV") ?: "production"
来源：http://dve.jianghu66.top

[U75] PHP：依赖注入
来源：http://nng.cucudq.cn

composer require psr/container
来源：http://sov.guowangkeji.top

[U76] PHP：简单路由
来源：http://isd.zhijiandao.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://ext.pycfn.com

[U77] PHP：模板渲染
来源：http://ziv.yfazqb.com

composer require twig/twig
来源：http://smd.yj20258888.top

[U78] PHP：单元测试
来源：http://jpf.vqdsnc.cn

composer require --dev phpunit/phpunit
来源：http://usc.xziqi.cn

[U79] PHP：静态分析
来源：http://ccd.xinyue.icu

composer require --dev phpstan/phpstan
来源：http://qxt.zycfv.cn

[U80] PHP：代码规范修复
来源：http://ilo.zhiwuduotai.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://sif.quarkkingdee.top

[U81] JS：初始化项目
来源：http://flh.vqdsnc.cn

npm init -y;  npm i express
来源：http://yoo.sweek.top

[U82] JS：package.json 脚本
来源：http://xus.shanyushiyangkeji.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://yod.yfazqb.com

[U83] JS：ES Module 导入导出
来源：http://jor.mhx1999.top

export const a = 1;  import { a } from "./m.js";
来源：http://lpn.zhoulong.xyz

[U84] JS：CommonJS 写法
来源：http://tol.tianlin.xyz

module.exports = { a };  const { a } = require("./m");
来源：http://chb.jiagoushi.top

[U85] JS：可选链
来源：http://hui.yj202588.top

a?.b?.c
来源：http://aqx.wangdashe.top

[U86] JS：空值合并
来源：http://ckx.xingfuxueyuan.xyz

a ?? b
来源：http://ssk.jqgfzy.top

[U87] JS：解构默认值
来源：http://qut.aizwys.cn

const { a = 1, b = 2 } = obj;
来源：http://xgn.cashguo.top

[U88] JS：对象展开合并
来源：http://typ.meibo888.top

{ ...a, ...b }
来源：http://ncz.daxiang520.top

[U89] JS：数组去重
来源：http://tis.sysykeji.top

[...new Set(arr)]
来源：http://qdc.fktsv.cn

[U90] JS：数字数组排序
来源：http://pyg.jyoumei.cn

[...arr].sort((a, b) => a - b)
来源：http://tco.fanxiaobao.xyz

[U91] JS：对象键值遍历
来源：http://qcy.yongpay.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://xkd.havefunace.top

[U92] JS：深拷贝
来源：http://dfv.yueranfly.top

structuredClone(obj)
来源：http://rvg.iojbl.cn

[U93] JS：模板字符串
来源：http://ljy.shanyushiyangtech.top

`共 ${n} 条`
来源：http://mpz.316326.xyz

[U94] JS：箭头函数
来源：http://iwp.shangyingyoupin.top

const double = x => x * 2;
来源：http://lsq.nanxuanxn.top

[U95] JS：Promise 包装
来源：http://exa.chenzaomai.com

new Promise((resolve, reject) => {})
来源：http://tzt.birdmap.top

[U96] JS：async/await 与异常
来源：http://yya.ctjpmb.com

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://xwz.zhongyouzk.top

[U97] JS：并发请求
来源：http://bfu.gaohongyu789.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://vvn.yangfankeji.com

[U98] JS：fetch 带 JSON
来源：http://ogu.ctjpmb.com

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://iav.gogol.net.cn

[U99] JS：事件监听
来源：http://iyd.ehwqpu.com

el.addEventListener("click", e => {})
来源：http://uyc.jlsjyb.cn

[U100] JS：DOM 查询
来源：http://bav.hnqzz.top

document.querySelector(".item")
来源：http://rck.mhx1999.top

[U101] JS：classList 操作
来源：http://zkq.andypj.xyz

el.classList.toggle("active")
来源：http://gkd.sweek.top

[U102] JS：本地存储
来源：http://iot.vqdsnc.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://moq.ctjpmb.com

[U103] JS：定时器
来源：http://iud.vehdjk.com

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://aur.yanxiufei.cn

[U104] JS：防抖
来源：http://goj.yangfankeji.com

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://zxo.vqdsnc.cn

[U105] JS：节流
来源：http://dxg.xingfuxueyuan.xyz

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://ogj.tanke756.top

[U106] JS：日期格式化
来源：http://onc.zhengqikj.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://ist.ivvv.top

[U107] JS：数字千分位
来源：http://ajd.bjfxy.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://wga.zhengqikj.top

[U108] JS：随机整数
来源：http://xvu.zhongyouzk.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://sym.pengpengdd.cyou

[U109] JS：数组分组
来源：http://nhh.guannengcc.top

Object.groupBy(arr, x => x.type)
来源：http://ttj.xuetiantiany.cn

[U110] JS：数组分块
来源：http://waz.chenzaomai.com

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://qpx.zhaomingkeji.xyz

[U111] JS：对象转 Map
来源：http://xqs.bjfxy.top

new Map(Object.entries(obj))
来源：http://otv.jinqigfzy.top

[U112] JS：字符串补位
来源：http://sxq.nanxinkj.top

"7".padStart(3, "0")
来源：http://tjj.jinqigufen.top

[U113] JS：正则替换全部
来源：http://cjj.ywan-chungtsiang.top

s.replaceAll("a", "b")
来源：http://dvd.yj20258.top

[U114] JS：JSON 深比较
来源：http://wqt.gaohongyu789.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://fms.mhx1999.top

[U115] JS：生成 UUID
来源：http://oow.jyoumei.cn

crypto.randomUUID()
来源：http://bej.dianchejie.cn

[U116] JS：类型检查（JSDoc）
来源：http://cjz.wangshuangyany.cn

/** @param {string} name */ function f(name) {}
来源：http://bcv.hnxiangtu.top

[U117] JS：单元测试
来源：http://bls.sufxvd.cn

npm i -D vitest;  npx vitest
来源：http://qvq.hfpthk.cn

[U118] JS：开发服务器
来源：http://yvl.shanyushiyangkeji.top

npm i -D vite;  npx vite
来源：http://slv.zycfv.cn

[U119] JS：生产构建
来源：http://syj.fanxiaobao.xyz

npx vite build
来源：http://zwy.jinqigufen.top

[U120] JS：读取环境变量（Vite）
来源：http://pud.xziqi.cn

import.meta.env.VITE_API_URL
来源：http://xgq.fengsongda.top

================================================================================
来源：http://zyd.jqgfzy.top

统计汇总
来源：http://rby.smart0.xyz

================================================================================
来源：http://cso.snrcjt.cn

按语言统计（条）：
来源：http://jca.gotoacloud.top

Python ......... 252
来源：http://zty.sweek.top

PHP ............ 252
来源：http://jst.yfazqb.com

JavaScript ..... 252
来源：http://gzu.yj202588.top

TypeScript ..... 212
来源：http://zob.yuanzhike.top

Java ........... 212
来源：http://wne.yj202588.top

Go ............. 212
来源：http://mwi.uphjek.com

Ruby ........... 212
来源：http://vic.xuetiantiany.cn

C# ............. 212
来源：http://sta.jinqigfzy.top

C .............. 30
来源：http://inz.jinghuilouyu.cn

C++ ............ 30
来源：http://qez.shuidangran.top

SQL ............ 90
来源：http://yml.wangshuangyany.cn

Bash ........... 80
来源：http://kiy.tarul.cn

Kotlin ......... 15
来源：http://stm.jqgufenzy.top

Swift .......... 15
来源：http://lkp.jinqigufen.top

Lua ............ 10
来源：http://ncb.zhengqikj.top

Perl ........... 10
来源：http://jag.shzxlz.cn

Scala .......... 10
来源：http://jsy.meibo888.top

------------------------------------
来源：http://fbo.jqgfzy.top

合计 ........... 2106 条
来源：http://jax.ctjpmb.com

按章节统计：
来源：http://jrk.fzhhl.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://igx.sufxvd.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://aec.ydjk.org.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://esg.yongpay.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://ujq.wangdashe.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://evi.zhixingplan.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://sqv.zhixingplan.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://ikn.cqqwz.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://slu.ivvv.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://yqe.vqdsnc.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://hyq.nanxuanxn.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://ybw.yueranfly.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://xri.daria6918.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://ife.gogol.net.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://lnl.ivvv.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://vsh.daria6918.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://kel.snrcjt.cn

Q SQL 专题                              90
来源：http://sdn.hnxiangtu.top

R Bash 专题                             80
来源：http://lfm.jqgufenzy.top

S C / C++ 专题                          60
来源：http://aqb.xylfe.cn

T 其他语言补充                          60
来源：http://qgj.yj202588.top

U 高频实用片段                         120
来源：http://ztv.shanyushiyangkeji.top

------------------------------------
来源：http://yum.yj20258.top

合计                                  2106 条
来源：http://qho.ppjwa.cn

--------------------------------------------------------------------------------
来源：http://juq.tian-w.cn

使用提醒
来源：http://gtt.xziqi.cn

--------------------------------------------------------------------------------
来源：http://quf.yuxming.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://src.vehdjk.com

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://vso.yj202588.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://agn.haohaochexian.top

在旧版本上使用前请先确认语法支持情况。
来源：http://lgi.fengsongda.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://wyb.cheryme.top

—— 文件结束 ——
来源：http://prw.epnwcf.com

================================================================================
来源：http://yma.316326.xyz

程序语言常见例子速查手册（2024 版）
来源：http://swj.ydzc1.top

Common Programming Examples Cheat Book
来源：http://uiv.gotoacloud.top

================================================================================
来源：http://vue.tarul.cn

【收录内容】
来源：http://uho.jqgufenzy.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://trx.shanyushiyangtech.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://crw.kuanghao11.cn

SQL · Bash · C · C++
来源：http://beu.sjlbkw.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://een.yanxiufei.cn

【使用说明】
来源：http://iqp.tian-w.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://lgu.jlsjyb.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://aml.chenzaomai.com

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://gna.xylfe.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://vse.fehbvm.com

Bash:  Shell         C:     C             C++:   C++
来源：http://pyb.xingfuxueyuan.xyz

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://xja.smart0.xyz

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://owm.zhaomingkeji.xyz

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://ldt.ydzc1.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://faw.daxiang520.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://dzd.feifeiyinyue.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://fyz.zhoulong.xyz

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://puq.hesvh.cn

【文件统计】
来源：http://upj.smart0.xyz

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://jmc.nwbrower.top

--------------------------------------------------------------------------------
来源：http://xru.tanke756.top

目  录
来源：http://sdf.gogol.net.cn

--------------------------------------------------------------------------------
来源：http://eso.ehwqpu.com

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://qww.hcnkem.com

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://ict.jinqigfzy.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://fxf.svipenyu.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://fmf.pycfn.com

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://pxt.pengpengdd.cyou

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://wld.xinyue.icu

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://mpk.jinyuanbaomall.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://coq.daxiang520.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://ecb.aibaodan.cn


<!-- 参考信息 -->