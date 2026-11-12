代发 wailian999

[U17] Py：初始化日志
来源：http://bol.sxryk.cn

logging.basicConfig(level=logging.INFO)
来源：http://aqw.yanxiufei.cn

[U18] Py：预编译正则
来源：http://veu.cheryme.top

pat = re.compile(r"\d+")
来源：http://tqh.birdmap.top

[U19] Py：正则替换带回调
来源：http://xkq.quarkkingdee.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://bsj.xinyue.icu

[U20] Py：缓存函数结果
来源：http://krv.zhengqikj.top

@functools.lru_cache(maxsize=None)
来源：http://veu.cqqwz.cn

[U21] Py：自定义上下文管理器
来源：http://doc.jianghu66.top

@contextlib.contextmanager
来源：http://jsl.quarkkingdee.top

[U22] Py：矩阵转置
来源：http://mph.jlsjyb.cn

list(zip(*m))
来源：http://qmi.tarul.cn

[U23] Py：分块读取大文件
来源：http://obk.yuxming.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://yjw.quarkkingdee.top

[U24] Py：路径操作
来源：http://tzv.guannengcc.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hca.jqgufenzy.top

[U25] Py：CSV 按字典读
来源：http://tgv.wangshuangyany.cn

csv.DictReader(f)
来源：http://imt.jqgufenzy.top

[U26] Py：并发下载
来源：http://ady.yuanzhike.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://qxp.jinyuanbaomall.cn

[U27] Py：异步 HTTP
来源：http://pzr.gzhubu.top

aiohttp.ClientSession() 配合 async with
来源：http://msa.hnqzz.top

[U28] Py：类型别名
来源：http://roo.zhengqikj.top

UserId = int
来源：http://lkm.jinyuanbaomall.cn

[U29] Py：属性校验
来源：http://xev.dashuyun.cn

@property 与 @x.setter 配合
来源：http://kta.shanyushiyangtech.top

[U30] Py：数据类
来源：http://dkd.xuanzx.com

@dataclass(slots=True)
来源：http://dfc.gaohongyu789.top

[U31] Py：单测
来源：http://xvu.sweek.top

python -m pytest -q
来源：http://vxi.cheryme.top

[U32] Py：代码格式化
来源：http://kee.zhijiandao.cn

ruff format . && ruff check --fix .
来源：http://ict.0kj1m.cn

[U33] Py：打包发布
来源：http://bmg.hnqzz.top

python -m build  （依赖 pyproject.toml）
来源：http://ygy.guannengcc.top

[U34] Py：判断编码
来源：http://vma.sweek.top

chardet.detect(raw)
来源：http://kvi.hnxiangtu.top

[U35] Py：发送邮件
来源：http://qvb.gotoacloud.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://mpo.daria6918.cn

[U36] Py：定时任务
来源：http://xks.yongpay.top

schedule.every(10).minutes.do(job)
来源：http://ilm.zhaomingkeji.xyz

[U37] Py：读写 Excel
来源：http://nsj.hcnkem.com

pandas.read_excel / DataFrame.to_excel
来源：http://kmr.shuidangran.top

[U38] Py：获取脚本所在目录
来源：http://svt.aibaodan.cn

Path(__file__).resolve().parent
来源：http://kdu.zhengqikj.top

[U39] Py：判断是否在交互环境
来源：http://dqt.cashguo.top

sys.stdout.isatty()
来源：http://xrf.vehdjk.com

[U40] Py：打印到标准错误
来源：http://ghl.gogol.net.cn

print("err", file=sys.stderr)
来源：http://kcv.hesvh.cn

[U41] PHP：初始化 Composer 项目
来源：http://wfi.xuetiantiany.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://rej.hywenlv.cn

[U42] PHP：PSR-4 自动加载
来源：http://ive.pengpengdd.cyou

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://igj.zhiwuduotai.top

[U43] PHP：声明命名空间
来源：http://gvj.fehbvm.com

namespace App\Http;
来源：http://wbb.tianlin.xyz

[U44] PHP：开启严格类型
来源：http://anu.yvedp.cn

declare(strict_types=1);
来源：http://tuc.gotoacloud.top

[U45] PHP：类型声明与返回类型
来源：http://wbm.iojbl.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://wrg.guannengcc.top

[U46] PHP：可空类型
来源：http://xey.nwbrower.top

?string $name = null
来源：http://nzy.dianchejie.cn

[U47] PHP：联合类型
来源：http://ssc.zhijiandao.cn

int|string $id
来源：http://agp.hnqzz.top

[U48] PHP：纯枚举
来源：http://gtu.fehbvm.com

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://bgf.pycfn.com

[U49] PHP：只读属性
来源：http://gja.andypj.xyz

public readonly string $name
来源：http://bdp.hammf.cn

[U50] PHP：构造器属性提升
来源：http://nvx.tanke756.top

public function __construct(private int $id) {}
来源：http://tou.zhongyouzk.top

[U51] PHP：数组解构
来源：http://eze.smart0.xyz

[$a, $b] = $arr;
来源：http://lif.guannengcc.top

[U52] PHP：箭头函数
来源：http://wlp.yangfankeji.com

$double = fn($x) => $x * 2;
来源：http://iqn.aibaodan.cn

[U53] PHP：空合并运算符
来源：http://bzv.birdmap.top

$v = $a ?? $b ?? "default";
来源：http://wfh.yongpay.top

[U54] PHP：空安全调用
来源：http://wja.ivvv.top

$obj?->method()
来源：http://rah.yj20258.top

[U55] PHP：match 表达式
来源：http://aty.yueranfly.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hlf.yangfankeji.com

[U56] PHP：命名参数
来源：http://fnx.meibo888.top

f(a: 1, b: 2)
来源：http://ezs.kuanghao11.cn

[U57] PHP：字符串插值
来源：http://kjc.sjlbkw.cn

"值: {$a}"
来源：http://oca.dianchejie.cn

[U58] PHP：数组三件套
来源：http://ork.jyoumei.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://qur.zhaomingkeji.xyz

[U59] PHP：自定义排序
来源：http://wei.bjfxy.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://rlr.chenzaomai.com

[U60] PHP：JSON 编解码
来源：http://hvn.shanyushiyangkeji.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://zlc.hnxiangtu.top

[U61] PHP：正则
来源：http://ffq.mhx1999.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://kvj.tian-w.cn

[U62] PHP：日期对象
来源：http://cva.jinqigufen.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://nmu.vqdsnc.cn

[U63] PHP：文件读写
来源：http://ikx.jinqigufen.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://rsu.jinqigfzy.top

[U64] PHP：目录遍历
来源：http://vxw.zhengqikj.top

glob("dir/*.php");  scandir("dir");
来源：http://ink.wangdashe.top

[U65] PHP：会话
来源：http://cqi.sjlbkw.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://ziu.316326.xyz

[U66] PHP：设置 Cookie
来源：http://mue.daria6918.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://ktq.svipenyu.cn

[U67] PHP：处理文件上传
来源：http://quv.cucudq.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://axd.yangfankeji.com

[U68] PHP：PDO 连接
来源：http://gga.zhongyouzk.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://utc.hesvh.cn

[U69] PHP：PDO 预处理
来源：http://fxj.ybcxt.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://gpj.jinghuilouyu.cn

[U70] PHP：PDO 事务
来源：http://ucz.snrcjt.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://gyu.xziqi.cn

[U71] PHP：抛出异常
来源：http://hkq.wangdashe.top

throw new RuntimeException("失败", 500);
来源：http://tsf.yonumen.top

[U72] PHP：写错误日志
来源：http://ujx.zdqjudy.top

error_log("失败: " . $e->getMessage());
来源：http://bry.dashuyun.cn

[U73] PHP：读取 ini 配置
来源：http://qrn.jinqigfzy.top

parse_ini_file("config.ini", true)
来源：http://yny.nanxinkj.top

[U74] PHP：读取环境变量
来源：http://lka.fanxiaobao.xyz

getenv("APP_ENV") ?: "production"
来源：http://ora.guowangkeji.top

[U75] PHP：依赖注入
来源：http://gkh.yonumen.top

composer require psr/container
来源：http://npa.yanxiufei.cn

[U76] PHP：简单路由
来源：http://ejf.pengpengdd.cyou

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://yxv.yuxming.cn

[U77] PHP：模板渲染
来源：http://mcw.316326.xyz

composer require twig/twig
来源：http://gxj.zhijiandao.cn

[U78] PHP：单元测试
来源：http://ulx.yongpay.top

composer require --dev phpunit/phpunit
来源：http://zic.hammf.cn

[U79] PHP：静态分析
来源：http://jpd.jlsjyb.cn

composer require --dev phpstan/phpstan
来源：http://duc.hywenlv.cn

[U80] PHP：代码规范修复
来源：http://qsa.cheryme.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://tfe.tian-w.cn

[U81] JS：初始化项目
来源：http://efq.mhx1999.top

npm init -y;  npm i express
来源：http://nwq.cqqwz.cn

[U82] JS：package.json 脚本
来源：http://eah.fktsv.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://npy.shangyingyoupin.top

[U83] JS：ES Module 导入导出
来源：http://ujn.gaohongyu789.top

export const a = 1;  import { a } from "./m.js";
来源：http://pth.guowangkeji.top

[U84] JS：CommonJS 写法
来源：http://jaz.tanke756.top

module.exports = { a };  const { a } = require("./m");
来源：http://jrz.aibaodan.cn

[U85] JS：可选链
来源：http://zda.shzxlz.cn

a?.b?.c
来源：http://hcl.hfpthk.cn

[U86] JS：空值合并
来源：http://sub.ywan-chungtsiang.top

a ?? b
来源：http://zih.pengpengdd.cyou

[U87] JS：解构默认值
来源：http://tic.zycfv.cn

const { a = 1, b = 2 } = obj;
来源：http://hnu.pycfn.com

[U88] JS：对象展开合并
来源：http://fac.andypj.xyz

{ ...a, ...b }
来源：http://lyk.yongpay.top

[U89] JS：数组去重
来源：http://phq.jinqigfzy.top

[...new Set(arr)]
来源：http://yck.0kj1m.cn

[U90] JS：数字数组排序
来源：http://jtj.zhengqikj.top

[...arr].sort((a, b) => a - b)
来源：http://uus.chenjidiqi.icu

[U91] JS：对象键值遍历
来源：http://bli.fanxiaobao.xyz

Object.entries(obj).forEach(([k, v]) => {});
来源：http://geb.xingfuxueyuan.xyz

[U92] JS：深拷贝
来源：http://gdg.sxryk.cn

structuredClone(obj)
来源：http://vhg.tarul.cn

[U93] JS：模板字符串
来源：http://pmr.xinyue.icu

`共 ${n} 条`
来源：http://irl.meibo888.top

[U94] JS：箭头函数
来源：http://gzm.xuanzx.com

const double = x => x * 2;
来源：http://zpz.xuanzx.com

[U95] JS：Promise 包装
来源：http://lfj.shanyushiyangkeji.top

new Promise((resolve, reject) => {})
来源：http://asq.zhoulong.xyz

[U96] JS：async/await 与异常
来源：http://ewn.yj202588.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://typ.cashguo.top

[U97] JS：并发请求
来源：http://kic.sufxvd.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://tmc.ivvv.top

[U98] JS：fetch 带 JSON
来源：http://cug.cdnleiting.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://dsp.epnwcf.com

[U99] JS：事件监听
来源：http://zgs.gzhubu.top

el.addEventListener("click", e => {})
来源：http://qhm.andypj.xyz

[U100] JS：DOM 查询
来源：http://pfk.hnqzz.top

document.querySelector(".item")
来源：http://zav.fzhhl.top

[U101] JS：classList 操作
来源：http://ewr.hongshengwenyu.top

el.classList.toggle("active")
来源：http://hua.iojbl.cn

[U102] JS：本地存储
来源：http://znp.vehdjk.com

localStorage.setItem("k", JSON.stringify(v))
来源：http://abo.fehbvm.com

[U103] JS：定时器
来源：http://ddu.gotoacloud.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://vbw.zdbjq.cn

[U104] JS：防抖
来源：http://uaj.redwolf501.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://lqn.shanyushiyangkeji.top

[U105] JS：节流
来源：http://cqe.zhaomingkeji.xyz

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://uia.sufxvd.cn

[U106] JS：日期格式化
来源：http://gid.hfpthk.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://nhk.svipenyu.cn

[U107] JS：数字千分位
来源：http://bcj.hongshengwenyu.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://pqu.cucudq.cn

[U108] JS：随机整数
来源：http://cpu.shanyushiyangtech.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://fbs.nanxuanxn.top

[U109] JS：数组分组
来源：http://jsy.havefunace.top

Object.groupBy(arr, x => x.type)
来源：http://alf.shuidangran.top

[U110] JS：数组分块
来源：http://kcv.cashguo.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://rti.yongpay.top

[U111] JS：对象转 Map
来源：http://jax.yueranfly.top

new Map(Object.entries(obj))
来源：http://qfv.yj202588.top

[U112] JS：字符串补位
来源：http://drm.bbcook.cn

"7".padStart(3, "0")
来源：http://wwz.birdmap.top

[U113] JS：正则替换全部
来源：http://jhg.zhijiandao.cn

s.replaceAll("a", "b")
来源：http://mhv.shangyingyoupin.top

[U114] JS：JSON 深比较
来源：http://jfl.jlsjyb.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://ezj.zhiwuduotai.top

[U115] JS：生成 UUID
来源：http://nek.quarkkingdee.top

crypto.randomUUID()
来源：http://dqd.0kj1m.cn

[U116] JS：类型检查（JSDoc）
来源：http://mzx.fehbvm.com

/** @param {string} name */ function f(name) {}
来源：http://ght.tarul.cn

[U117] JS：单元测试
来源：http://tpp.sxryk.cn

npm i -D vitest;  npx vitest
来源：http://lay.zhoulong.xyz

[U118] JS：开发服务器
来源：http://oah.c1oappe.top

npm i -D vite;  npx vite
来源：http://zyb.daria6918.cn

[U119] JS：生产构建
来源：http://swr.daxiang520.top

npx vite build
来源：http://ztk.zhongyouzk.top

[U120] JS：读取环境变量（Vite）
来源：http://zea.shanyushiyangkeji.top

import.meta.env.VITE_API_URL
来源：http://avg.daria6918.cn

================================================================================
来源：http://jjy.fengsongda.top

统计汇总
来源：http://lag.bjfxy.top

================================================================================
来源：http://tdu.yj20258888.top

按语言统计（条）：
来源：http://esb.zhijiandao.cn

Python ......... 252
来源：http://ejz.zhaomingkeji.xyz

PHP ............ 252
来源：http://diw.gogol.net.cn

JavaScript ..... 252
来源：http://qez.ydzc1.top

TypeScript ..... 212
来源：http://rst.jqgfzy.top

Java ........... 212
来源：http://rxd.ehwqpu.com

Go ............. 212
来源：http://niq.zhaomingkeji.xyz

Ruby ........... 212
来源：http://bqy.yfazqb.com

C# ............. 212
来源：http://tag.cucudq.cn

C .............. 30
来源：http://imy.redwolf501.top

C++ ............ 30
来源：http://fel.zhiwuduotai.top

SQL ............ 90
来源：http://zjj.yj20258.top

Bash ........... 80
来源：http://njn.chenzaomai.com

Kotlin ......... 15
来源：http://hfg.shzxlz.cn

Swift .......... 15
来源：http://pfl.fehbvm.com

Lua ............ 10
来源：http://yzs.c1oappe.top

Perl ........... 10
来源：http://gkm.vqdsnc.cn

Scala .......... 10
来源：http://nes.nanxuanxn.top

------------------------------------
来源：http://njx.jyoumei.cn

合计 ........... 2106 条
来源：http://kjo.jinqigfzy.top

按章节统计：
来源：http://hgx.sjlbkw.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://ihd.xinyue.icu

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://yjo.nwbrower.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://tsy.yuanzhike.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://nbk.quarkkingdee.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://ocd.c1oappe.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://xqs.daria6918.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://thn.jianghu66.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://uuf.tarul.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://cgx.cucudq.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://umz.jianghu66.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://ito.chenlongwang.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://cel.zdbjq.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://dqo.bbcook.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://zxt.hysaishi.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://uxp.andypj.xyz

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://aqi.sjlbkw.cn

Q SQL 专题                              90
来源：http://xex.jlsjyb.cn

R Bash 专题                             80
来源：http://ckv.kuanghao11.cn

S C / C++ 专题                          60
来源：http://bcz.zycfv.cn

T 其他语言补充                          60
来源：http://wyw.jinqigfzy.top

U 高频实用片段                         120
来源：http://naa.xylfe.cn

------------------------------------
来源：http://utg.c1oappe.top

合计                                  2106 条
来源：http://yey.cashguo.top

--------------------------------------------------------------------------------
来源：http://lxp.yonumen.top

使用提醒
来源：http://cks.zhiwuduotai.top

--------------------------------------------------------------------------------
来源：http://zql.aibaodan.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://kci.0kj1m.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://wyi.pycfn.com

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://qdo.sysykeji.top

在旧版本上使用前请先确认语法支持情况。
来源：http://pql.ydzc1.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://erd.dianchejie.cn

—— 文件结束 ——
来源：http://enf.shuidangran.top

================================================================================
来源：http://gez.xingfuxueyuan.xyz

程序语言常见例子速查手册（2024 版）
来源：http://rnv.yuanzhike.top

Common Programming Examples Cheat Book
来源：http://crb.tianlin.xyz

================================================================================
来源：http://ejt.yvedp.cn

【收录内容】
来源：http://wsc.tarul.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://bcp.gzhubu.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://qyi.iojbl.cn

SQL · Bash · C · C++
来源：http://kmf.xziqi.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://zec.cashguo.top

【使用说明】
来源：http://agu.c1oappe.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://mlc.jinyuanbaomall.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://hjh.kuanghao11.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://plo.ydjk.org.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://xuj.xuanzx.com

Bash:  Shell         C:     C             C++:   C++
来源：http://nnj.hcnkem.com

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://knb.cucudq.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://too.guowangkeji.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://kii.yj202588.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://hip.yongpay.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://ami.pycfn.com

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://ulf.daria6918.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://qeh.wangshuangyany.cn

【文件统计】
来源：http://wiv.hnqzz.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://dum.redwolf501.top

--------------------------------------------------------------------------------
来源：http://txn.daria6918.cn

目  录
来源：http://nle.redwolf501.top

--------------------------------------------------------------------------------
来源：http://lls.nanxinkj.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://qwu.zhengqikj.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://idx.yongpay.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://fbr.yuxming.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://ocu.shuidangran.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://ywy.tian-w.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://wea.ppjwa.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://osr.kuanghao11.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://uiz.zycfv.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://bvq.dianchejie.cn


<!-- 参考信息 -->