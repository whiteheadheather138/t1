代发 wailian999

[U23] Py：分块读取大文件
来源：http://kcq.pycfn.com

for chunk in iter(lambda: f.read(8192), b""):
来源：http://zij.pengpengdd.cyou

[U24] Py：路径操作
来源：http://fed.chenzaomai.com

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://rif.mhx1999.top

[U25] Py：CSV 按字典读
来源：http://rpw.jlsjyb.cn

csv.DictReader(f)
来源：http://cdm.bjfxy.top

[U26] Py：并发下载
来源：http://hgp.hesvh.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://tid.ydjk.org.cn

[U27] Py：异步 HTTP
来源：http://shj.hfpthk.cn

aiohttp.ClientSession() 配合 async with
来源：http://fes.jyoumei.cn

[U28] Py：类型别名
来源：http://adx.xuanzx.com

UserId = int
来源：http://foq.sxryk.cn

[U29] Py：属性校验
来源：http://hxz.uphjek.com

@property 与 @x.setter 配合
来源：http://qsq.gzhubu.top

[U30] Py：数据类
来源：http://ghb.yfazqb.com

@dataclass(slots=True)
来源：http://vtq.cheryme.top

[U31] Py：单测
来源：http://azp.havefunace.top

python -m pytest -q
来源：http://kza.pycfn.com

[U32] Py：代码格式化
来源：http://gzf.vehdjk.com

ruff format . && ruff check --fix .
来源：http://aee.epnwcf.com

[U33] Py：打包发布
来源：http://hvr.chenzaomai.com

python -m build  （依赖 pyproject.toml）
来源：http://toh.yuxming.cn

[U34] Py：判断编码
来源：http://lih.yfazqb.com

chardet.detect(raw)
来源：http://zts.hongshengwenyu.top

[U35] Py：发送邮件
来源：http://rwj.gotoacloud.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hqg.cheryme.top

[U36] Py：定时任务
来源：http://eva.xziqi.cn

schedule.every(10).minutes.do(job)
来源：http://khw.zhoulong.xyz

[U37] Py：读写 Excel
来源：http://mts.hammf.cn

pandas.read_excel / DataFrame.to_excel
来源：http://rft.ctjpmb.com

[U38] Py：获取脚本所在目录
来源：http://flw.hnxiangtu.top

Path(__file__).resolve().parent
来源：http://vlw.hnxiangtu.top

[U39] Py：判断是否在交互环境
来源：http://qmp.gaohongyu789.top

sys.stdout.isatty()
来源：http://plr.nanxuanxn.top

[U40] Py：打印到标准错误
来源：http://rfx.yj20258.top

print("err", file=sys.stderr)
来源：http://miu.hnqzz.top

[U41] PHP：初始化 Composer 项目
来源：http://tou.yangfankeji.com

composer init;  composer require guzzlehttp/guzzle
来源：http://pfp.yonumen.top

[U42] PHP：PSR-4 自动加载
来源：http://sjf.sufxvd.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://tfe.zhixingplan.top

[U43] PHP：声明命名空间
来源：http://wpe.fanxiaobao.xyz

namespace App\Http;
来源：http://cen.yj20258.top

[U44] PHP：开启严格类型
来源：http://hla.fehbvm.com

declare(strict_types=1);
来源：http://jnv.jiagoushi.top

[U45] PHP：类型声明与返回类型
来源：http://lyp.zhijiandao.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://ulv.fzhhl.top

[U46] PHP：可空类型
来源：http://prg.cheryme.top

?string $name = null
来源：http://wer.52xcode.cn

[U47] PHP：联合类型
来源：http://lzh.ydzc1.top

int|string $id
来源：http://dim.shzxlz.cn

[U48] PHP：纯枚举
来源：http://pfw.xuetiantiany.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://rgb.cucudq.cn

[U49] PHP：只读属性
来源：http://swg.gogol.net.cn

public readonly string $name
来源：http://rlg.nwbrower.top

[U50] PHP：构造器属性提升
来源：http://zrr.cheryme.top

public function __construct(private int $id) {}
来源：http://rnq.iojbl.cn

[U51] PHP：数组解构
来源：http://gko.tanke756.top

[$a, $b] = $arr;
来源：http://qsh.ppjwa.cn

[U52] PHP：箭头函数
来源：http://dse.wangshuangyany.cn

$double = fn($x) => $x * 2;
来源：http://rsu.jiagoushi.top

[U53] PHP：空合并运算符
来源：http://uht.aizwys.cn

$v = $a ?? $b ?? "default";
来源：http://psg.hesvh.cn

[U54] PHP：空安全调用
来源：http://myb.tarul.cn

$obj?->method()
来源：http://kyp.feifeiyinyue.top

[U55] PHP：match 表达式
来源：http://qax.cashguo.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hia.mhx1999.top

[U56] PHP：命名参数
来源：http://trt.chenzaomai.com

f(a: 1, b: 2)
来源：http://uxw.wangshuangyany.cn

[U57] PHP：字符串插值
来源：http://rmm.xuetiantiany.cn

"值: {$a}"
来源：http://hhn.vqdsnc.cn

[U58] PHP：数组三件套
来源：http://qrw.xziqi.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://dcr.xingfuxueyuan.xyz

[U59] PHP：自定义排序
来源：http://fld.ivvv.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://lxi.aizwys.cn

[U60] PHP：JSON 编解码
来源：http://ehl.kuanghao11.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://vjc.ydjk.org.cn

[U61] PHP：正则
来源：http://hta.daria6918.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://jdr.jinghuilouyu.cn

[U62] PHP：日期对象
来源：http://zzn.ppjwa.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://ezo.cdnleiting.top

[U63] PHP：文件读写
来源：http://esv.cheryme.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://euw.jinqigufen.top

[U64] PHP：目录遍历
来源：http://ovn.hywenlv.cn

glob("dir/*.php");  scandir("dir");
来源：http://qoc.xziqi.cn

[U65] PHP：会话
来源：http://jnm.ppjwa.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://oyl.chenlongwang.top

[U66] PHP：设置 Cookie
来源：http://qdq.jyoumei.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://etq.jianghu66.top

[U67] PHP：处理文件上传
来源：http://epk.fzhhl.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://lod.0kj1m.cn

[U68] PHP：PDO 连接
来源：http://fne.kuanghao11.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://jyg.yj20258888.top

[U69] PHP：PDO 预处理
来源：http://elk.smart0.xyz

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://svp.yanxiufei.cn

[U70] PHP：PDO 事务
来源：http://xfr.hesvh.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://rda.ppjwa.cn

[U71] PHP：抛出异常
来源：http://pbu.ppjwa.cn

throw new RuntimeException("失败", 500);
来源：http://iox.hfpthk.cn

[U72] PHP：写错误日志
来源：http://soh.yvedp.cn

error_log("失败: " . $e->getMessage());
来源：http://tzp.ydjk.org.cn

[U73] PHP：读取 ini 配置
来源：http://tan.jqgufenzy.top

parse_ini_file("config.ini", true)
来源：http://yxf.ybcxt.top

[U74] PHP：读取环境变量
来源：http://hvi.jqgufenzy.top

getenv("APP_ENV") ?: "production"
来源：http://ztx.daria6918.cn

[U75] PHP：依赖注入
来源：http://wzn.hfpthk.cn

composer require psr/container
来源：http://shk.wangdashe.top

[U76] PHP：简单路由
来源：http://gkm.xziqi.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://ruv.cucudq.cn

[U77] PHP：模板渲染
来源：http://yqq.gaohongyu789.top

composer require twig/twig
来源：http://arl.hnqzz.top

[U78] PHP：单元测试
来源：http://kee.ywan-chungtsiang.top

composer require --dev phpunit/phpunit
来源：http://gnk.bbcook.cn

[U79] PHP：静态分析
来源：http://std.tian-w.cn

composer require --dev phpstan/phpstan
来源：http://qen.xylfe.cn

[U80] PHP：代码规范修复
来源：http://hff.gzhubu.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://jqv.andypj.xyz

[U81] JS：初始化项目
来源：http://bpf.yuxming.cn

npm init -y;  npm i express
来源：http://gqn.fengsongda.top

[U82] JS：package.json 脚本
来源：http://pqv.ywan-chungtsiang.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://itu.shangyingyoupin.top

[U83] JS：ES Module 导入导出
来源：http://xbu.chenzaomai.com

export const a = 1;  import { a } from "./m.js";
来源：http://uxo.yfazqb.com

[U84] JS：CommonJS 写法
来源：http://cvm.vqdsnc.cn

module.exports = { a };  const { a } = require("./m");
来源：http://hpj.svipenyu.cn

[U85] JS：可选链
来源：http://pwg.gogol.net.cn

a?.b?.c
来源：http://fug.c1oappe.top

[U86] JS：空值合并
来源：http://mmj.hfpthk.cn

a ?? b
来源：http://svf.chenzaomai.com

[U87] JS：解构默认值
来源：http://vvp.52xcode.cn

const { a = 1, b = 2 } = obj;
来源：http://wok.vqdsnc.cn

[U88] JS：对象展开合并
来源：http://bgd.shangyingyoupin.top

{ ...a, ...b }
来源：http://bqb.jinyuanbaomall.cn

[U89] JS：数组去重
来源：http://qmw.jiagoushi.top

[...new Set(arr)]
来源：http://yhn.sxryk.cn

[U90] JS：数字数组排序
来源：http://fqv.hesvh.cn

[...arr].sort((a, b) => a - b)
来源：http://cnd.xuetiantiany.cn

[U91] JS：对象键值遍历
来源：http://ztw.nwbrower.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://wxs.jinqigfzy.top

[U92] JS：深拷贝
来源：http://szb.kuanghao11.cn

structuredClone(obj)
来源：http://lys.jyoumei.cn

[U93] JS：模板字符串
来源：http://eqs.kuanghao11.cn

`共 ${n} 条`
来源：http://cyx.yuanzhike.top

[U94] JS：箭头函数
来源：http://cgx.yongpay.top

const double = x => x * 2;
来源：http://slg.pycfn.com

[U95] JS：Promise 包装
来源：http://ywu.zycfv.cn

new Promise((resolve, reject) => {})
来源：http://jvp.ivvv.top

[U96] JS：async/await 与异常
来源：http://wkr.smart0.xyz

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://woz.sufxvd.cn

[U97] JS：并发请求
来源：http://owm.aizwys.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://pie.wangdashe.top

[U98] JS：fetch 带 JSON
来源：http://zia.zdqjudy.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://adf.xziqi.cn

[U99] JS：事件监听
来源：http://vzd.shzxlz.cn

el.addEventListener("click", e => {})
来源：http://rul.sweek.top

[U100] JS：DOM 查询
来源：http://sbi.tian-w.cn

document.querySelector(".item")
来源：http://syu.fehbvm.com

[U101] JS：classList 操作
来源：http://kin.hongshengwenyu.top

el.classList.toggle("active")
来源：http://ktg.yj20258888.top

[U102] JS：本地存储
来源：http://aqt.shanyushiyangkeji.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://xvh.zhaomingkeji.xyz

[U103] JS：定时器
来源：http://hri.hesvh.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://onq.xuetiantiany.cn

[U104] JS：防抖
来源：http://uxx.shuidangran.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://iln.pycfn.com

[U105] JS：节流
来源：http://msu.dashuyun.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://xgu.daria6918.cn

[U106] JS：日期格式化
来源：http://oyu.meibo888.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://ybb.andypj.xyz

[U107] JS：数字千分位
来源：http://qbq.316326.xyz

new Intl.NumberFormat("en-US").format(1234567)
来源：http://pkn.fzhhl.top

[U108] JS：随机整数
来源：http://jbt.sweek.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://ggp.yj20258.top

[U109] JS：数组分组
来源：http://tms.hesvh.cn

Object.groupBy(arr, x => x.type)
来源：http://ydm.zycfv.cn

[U110] JS：数组分块
来源：http://dvo.xuetiantiany.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://log.nwbrower.top

[U111] JS：对象转 Map
来源：http://oye.hongshengwenyu.top

new Map(Object.entries(obj))
来源：http://oyr.gogol.net.cn

[U112] JS：字符串补位
来源：http://xus.guowangkeji.top

"7".padStart(3, "0")
来源：http://yaz.guannengcc.top

[U113] JS：正则替换全部
来源：http://lef.aibaodan.cn

s.replaceAll("a", "b")
来源：http://eci.yj20258888.top

[U114] JS：JSON 深比较
来源：http://kmh.shzxlz.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://per.jinghuilouyu.cn

[U115] JS：生成 UUID
来源：http://nrm.fehbvm.com

crypto.randomUUID()
来源：http://frj.zdbjq.cn

[U116] JS：类型检查（JSDoc）
来源：http://sof.pengpengdd.cyou

/** @param {string} name */ function f(name) {}
来源：http://reu.daria6918.cn

[U117] JS：单元测试
来源：http://zik.xuanzx.com

npm i -D vitest;  npx vitest
来源：http://seo.hfpthk.cn

[U118] JS：开发服务器
来源：http://fnb.redwolf501.top

npm i -D vite;  npx vite
来源：http://pvt.dianchejie.cn

[U119] JS：生产构建
来源：http://fvq.birdmap.top

npx vite build
来源：http://qfz.uphjek.com

[U120] JS：读取环境变量（Vite）
来源：http://hij.xuetiantiany.cn

import.meta.env.VITE_API_URL
来源：http://ime.aizwys.cn

================================================================================
来源：http://ueg.snrcjt.cn

统计汇总
来源：http://iez.zhijiandao.cn

================================================================================
来源：http://rhh.sweek.top

按语言统计（条）：
来源：http://hzo.hongshengwenyu.top

Python ......... 252
来源：http://mty.nanxuanxn.top

PHP ............ 252
来源：http://zro.ivvv.top

JavaScript ..... 252
来源：http://deq.dashuyun.cn

TypeScript ..... 212
来源：http://lfx.birdmap.top

Java ........... 212
来源：http://uma.pycfn.com

Go ............. 212
来源：http://guc.mhx1999.top

Ruby ........... 212
来源：http://xqv.bjfxy.top

C# ............. 212
来源：http://txc.kuanghao11.cn

C .............. 30
来源：http://jme.cashguo.top

C++ ............ 30
来源：http://plw.c1oappe.top

SQL ............ 90
来源：http://qyv.wangshuangyany.cn

Bash ........... 80
来源：http://eho.zycfv.cn

Kotlin ......... 15
来源：http://pnx.zdqjudy.top

Swift .......... 15
来源：http://oiv.kuanghao11.cn

Lua ............ 10
来源：http://wjx.zhiwuduotai.top

Perl ........... 10
来源：http://yjp.jyoumei.cn

Scala .......... 10
来源：http://jog.316326.xyz

------------------------------------
来源：http://kiw.hnqzz.top

合计 ........... 2106 条
来源：http://ijm.yj202588.top

按章节统计：
来源：http://sso.fzhhl.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://xze.fehbvm.com

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://ddw.quarkkingdee.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://peg.xylfe.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://efk.gotoacloud.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://zxl.bjfxy.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://sco.fktsv.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://ahz.guowangkeji.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://alr.fanxiaobao.xyz

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://fhl.yfazqb.com

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://tmu.haohaochexian.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://lxa.wangdashe.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://lyu.jinqigufen.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://gzr.bjfxy.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://pwb.ivvv.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://zny.zhaomingkeji.xyz

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://iiw.yuxming.cn

Q SQL 专题                              90
来源：http://ltx.cqqwz.cn

R Bash 专题                             80
来源：http://kxg.yueranfly.top

S C / C++ 专题                          60
来源：http://ovr.gogol.net.cn

T 其他语言补充                          60
来源：http://pmf.zhaomingkeji.xyz

U 高频实用片段                         120
来源：http://qeb.yongpay.top

------------------------------------
来源：http://pzs.smart0.xyz

合计                                  2106 条
来源：http://yst.yj20258.top

--------------------------------------------------------------------------------
来源：http://uaj.ppjwa.cn

使用提醒
来源：http://sdi.aibaodan.cn

--------------------------------------------------------------------------------
来源：http://vnc.hesvh.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://lpu.0kj1m.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://bdr.hnxiangtu.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://ymm.yj202588.top

在旧版本上使用前请先确认语法支持情况。
来源：http://trs.hysaishi.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://kqx.guowangkeji.top

—— 文件结束 ——
来源：http://muw.zycfv.cn

================================================================================
来源：http://vzs.ydzc1.top

程序语言常见例子速查手册（2024 版）
来源：http://sno.meibo888.top

Common Programming Examples Cheat Book
来源：http://kgj.sjlbkw.cn

================================================================================
来源：http://pna.guowangkeji.top

【收录内容】
来源：http://tgj.gzhubu.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://kho.cqqwz.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://meu.ivvv.top

SQL · Bash · C · C++
来源：http://pyx.pengpengdd.cyou

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://qss.kuanghao11.cn

【使用说明】
来源：http://cwg.yueranfly.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://hbf.zhixingplan.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://uwv.ivvv.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://qka.shuidangran.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://pjp.xylfe.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://ukf.pycfn.com

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://wtn.zhiwuduotai.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://haw.yonumen.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://cri.zycfv.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://jdy.zdbjq.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://cuk.pycfn.com

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://kmx.shanyushiyangtech.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://gll.kuanghao11.cn

【文件统计】
来源：http://ety.cashguo.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://csv.52xcode.cn

--------------------------------------------------------------------------------
来源：http://oha.hongshengwenyu.top

目  录
来源：http://hfb.tianlin.xyz

--------------------------------------------------------------------------------
来源：http://btp.guowangkeji.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://zyn.pengpengdd.cyou

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://whx.fktsv.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://xky.hcnkem.com

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://bjp.gotoacloud.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://ymf.fehbvm.com

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://gmi.smart0.xyz

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://mqu.dianchejie.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://wvw.gogol.net.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://fmo.jinqigufen.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://ftz.jinqigufen.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://fxe.fanxiaobao.xyz

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://bvl.zhixingplan.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://edh.ywan-chungtsiang.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://hwt.gzhubu.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://rup.c1oappe.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://jan.sufxvd.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://zsk.shzxlz.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://frt.xuetiantiany.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://msg.snrcjt.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://gsu.shanyushiyangtech.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://tcs.mhx1999.top


<!-- 参考信息 -->