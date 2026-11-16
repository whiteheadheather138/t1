代发 wailian999

[U19] Py：正则替换带回调
来源：http://rdj.jinqigfzy.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://cnp.fzhhl.top

[U20] Py：缓存函数结果
来源：http://nrm.birdmap.top

@functools.lru_cache(maxsize=None)
来源：http://bfn.hywenlv.cn

[U21] Py：自定义上下文管理器
来源：http://ais.hysaishi.cn

@contextlib.contextmanager
来源：http://odf.zhiwuduotai.top

[U22] Py：矩阵转置
来源：http://aex.ydjk.org.cn

list(zip(*m))
来源：http://dxb.aizwys.cn

[U23] Py：分块读取大文件
来源：http://yol.gzhubu.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://oun.vqdsnc.cn

[U24] Py：路径操作
来源：http://wmg.hfpthk.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://ger.daxiang520.top

[U25] Py：CSV 按字典读
来源：http://iwx.nanxuanxn.top

csv.DictReader(f)
来源：http://ttd.yanxiufei.cn

[U26] Py：并发下载
来源：http://uvh.cdnleiting.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://nvl.aizwys.cn

[U27] Py：异步 HTTP
来源：http://tuh.fktsv.cn

aiohttp.ClientSession() 配合 async with
来源：http://xhp.zhengqikj.top

[U28] Py：类型别名
来源：http://vhe.hysaishi.cn

UserId = int
来源：http://bkf.hcnkem.com

[U29] Py：属性校验
来源：http://bgh.sysykeji.top

@property 与 @x.setter 配合
来源：http://ica.sjlbkw.cn

[U30] Py：数据类
来源：http://mgy.dianchejie.cn

@dataclass(slots=True)
来源：http://pyd.bjfxy.top

[U31] Py：单测
来源：http://jjd.aibaodan.cn

python -m pytest -q
来源：http://glk.jyoumei.cn

[U32] Py：代码格式化
来源：http://dux.ppjwa.cn

ruff format . && ruff check --fix .
来源：http://jnh.sjlbkw.cn

[U33] Py：打包发布
来源：http://zer.jinqigfzy.top

python -m build  （依赖 pyproject.toml）
来源：http://fhx.birdmap.top

[U34] Py：判断编码
来源：http://dlf.zycfv.cn

chardet.detect(raw)
来源：http://yct.wangshuangyany.cn

[U35] Py：发送邮件
来源：http://zpj.zhiwuduotai.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://orw.yangfankeji.com

[U36] Py：定时任务
来源：http://ckh.c1oappe.top

schedule.every(10).minutes.do(job)
来源：http://bbg.jinqigufen.top

[U37] Py：读写 Excel
来源：http://ald.yj20258888.top

pandas.read_excel / DataFrame.to_excel
来源：http://tfc.chenlongwang.top

[U38] Py：获取脚本所在目录
来源：http://rhz.9152youxi.cn

Path(__file__).resolve().parent
来源：http://sqy.hongshengwenyu.top

[U39] Py：判断是否在交互环境
来源：http://hvy.fengsongda.top

sys.stdout.isatty()
来源：http://hef.hesvh.cn

[U40] Py：打印到标准错误
来源：http://djm.meibo888.top

print("err", file=sys.stderr)
来源：http://cqq.daxiang520.top

[U41] PHP：初始化 Composer 项目
来源：http://kuz.zhijiandao.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://poj.jlsjyb.cn

[U42] PHP：PSR-4 自动加载
来源：http://gpv.yuanzhike.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://dzu.hysaishi.cn

[U43] PHP：声明命名空间
来源：http://jaa.cqqwz.cn

namespace App\Http;
来源：http://mdl.fengsongda.top

[U44] PHP：开启严格类型
来源：http://kri.jqgufenzy.top

declare(strict_types=1);
来源：http://uph.gzhubu.top

[U45] PHP：类型声明与返回类型
来源：http://mht.bbcook.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://vgm.xziqi.cn

[U46] PHP：可空类型
来源：http://lgn.dianchejie.cn

?string $name = null
来源：http://fzy.hywenlv.cn

[U47] PHP：联合类型
来源：http://rdp.yj20258888.top

int|string $id
来源：http://pfx.snrcjt.cn

[U48] PHP：纯枚举
来源：http://kjb.52xcode.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://ysi.nanxuanxn.top

[U49] PHP：只读属性
来源：http://xed.jianghu66.top

public readonly string $name
来源：http://lkz.svipenyu.cn

[U50] PHP：构造器属性提升
来源：http://zwx.xingfuxueyuan.xyz

public function __construct(private int $id) {}
来源：http://kxr.52xcode.cn

[U51] PHP：数组解构
来源：http://mqg.chenjidiqi.icu

[$a, $b] = $arr;
来源：http://iqr.gotoacloud.top

[U52] PHP：箭头函数
来源：http://ilh.snrcjt.cn

$double = fn($x) => $x * 2;
来源：http://pfn.ybcxt.top

[U53] PHP：空合并运算符
来源：http://zcv.shzxlz.cn

$v = $a ?? $b ?? "default";
来源：http://evq.gogol.net.cn

[U54] PHP：空安全调用
来源：http://fha.xingfuxueyuan.xyz

$obj?->method()
来源：http://nwf.xuetiantiany.cn

[U55] PHP：match 表达式
来源：http://rnu.hfpthk.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://kva.daria6918.cn

[U56] PHP：命名参数
来源：http://gia.zhengqikj.top

f(a: 1, b: 2)
来源：http://aip.uphjek.com

[U57] PHP：字符串插值
来源：http://jag.nanxuanxn.top

"值: {$a}"
来源：http://gen.c1oappe.top

[U58] PHP：数组三件套
来源：http://fmo.zhiwuduotai.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://mqq.yfazqb.com

[U59] PHP：自定义排序
来源：http://tth.jinqigfzy.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://syw.tarul.cn

[U60] PHP：JSON 编解码
来源：http://raq.tian-w.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://lrc.jinyuanbaomall.cn

[U61] PHP：正则
来源：http://zcq.aizwys.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://nmr.feifeiyinyue.top

[U62] PHP：日期对象
来源：http://fiz.aizwys.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://uyr.hnxiangtu.top

[U63] PHP：文件读写
来源：http://idy.hammf.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://igo.cheryme.top

[U64] PHP：目录遍历
来源：http://tyz.zhijiandao.cn

glob("dir/*.php");  scandir("dir");
来源：http://ykd.yongpay.top

[U65] PHP：会话
来源：http://jtz.chenjidiqi.icu

session_start();  $_SESSION["uid"] = 1;
来源：http://yob.zhixingplan.top

[U66] PHP：设置 Cookie
来源：http://kvh.ppjwa.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://jvw.dianchejie.cn

[U67] PHP：处理文件上传
来源：http://bbk.wangdashe.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://anb.jyoumei.cn

[U68] PHP：PDO 连接
来源：http://uwf.guowangkeji.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://odr.yvedp.cn

[U69] PHP：PDO 预处理
来源：http://uiu.shanyushiyangtech.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://ipn.pengpengdd.cyou

[U70] PHP：PDO 事务
来源：http://lwd.sxryk.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://cwq.ivvv.top

[U71] PHP：抛出异常
来源：http://mwg.birdmap.top

throw new RuntimeException("失败", 500);
来源：http://mjr.gaohongyu789.top

[U72] PHP：写错误日志
来源：http://hhw.xingfuxueyuan.xyz

error_log("失败: " . $e->getMessage());
来源：http://myh.xingfuxueyuan.xyz

[U73] PHP：读取 ini 配置
来源：http://vds.feifeiyinyue.top

parse_ini_file("config.ini", true)
来源：http://efx.xuetiantiany.cn

[U74] PHP：读取环境变量
来源：http://ykb.bbcook.cn

getenv("APP_ENV") ?: "production"
来源：http://yqm.zhoulong.xyz

[U75] PHP：依赖注入
来源：http://jyl.xingfuxueyuan.xyz

composer require psr/container
来源：http://doh.ywan-chungtsiang.top

[U76] PHP：简单路由
来源：http://oqt.mhx1999.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://lnc.0kj1m.cn

[U77] PHP：模板渲染
来源：http://zhn.hfpthk.cn

composer require twig/twig
来源：http://qeg.chenlongwang.top

[U78] PHP：单元测试
来源：http://jnf.daria6918.cn

composer require --dev phpunit/phpunit
来源：http://vev.guannengcc.top

[U79] PHP：静态分析
来源：http://rjf.hesvh.cn

composer require --dev phpstan/phpstan
来源：http://ahf.yonumen.top

[U80] PHP：代码规范修复
来源：http://uyc.jianghu66.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://eoi.ydjk.org.cn

[U81] JS：初始化项目
来源：http://xxf.kuanghao11.cn

npm init -y;  npm i express
来源：http://bgx.snrcjt.cn

[U82] JS：package.json 脚本
来源：http://jxi.zhaomingkeji.xyz

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://qfj.hammf.cn

[U83] JS：ES Module 导入导出
来源：http://utg.hcnkem.com

export const a = 1;  import { a } from "./m.js";
来源：http://mxo.jiagoushi.top

[U84] JS：CommonJS 写法
来源：http://ojx.fengsongda.top

module.exports = { a };  const { a } = require("./m");
来源：http://sho.birdmap.top

[U85] JS：可选链
来源：http://kmk.zhijiandao.cn

a?.b?.c
来源：http://rtv.ywan-chungtsiang.top

[U86] JS：空值合并
来源：http://bhh.ppjwa.cn

a ?? b
来源：http://zbz.zhongyouzk.top

[U87] JS：解构默认值
来源：http://syg.daxiang520.top

const { a = 1, b = 2 } = obj;
来源：http://ioj.chenjidiqi.icu

[U88] JS：对象展开合并
来源：http://ynd.redwolf501.top

{ ...a, ...b }
来源：http://hln.0kj1m.cn

[U89] JS：数组去重
来源：http://bnv.yonumen.top

[...new Set(arr)]
来源：http://hhw.gotoacloud.top

[U90] JS：数字数组排序
来源：http://akg.gzhubu.top

[...arr].sort((a, b) => a - b)
来源：http://ofb.shanyushiyangkeji.top

[U91] JS：对象键值遍历
来源：http://ufd.vehdjk.com

Object.entries(obj).forEach(([k, v]) => {});
来源：http://nns.ivvv.top

[U92] JS：深拷贝
来源：http://ujb.shanyushiyangkeji.top

structuredClone(obj)
来源：http://nvk.pengpengdd.cyou

[U93] JS：模板字符串
来源：http://qgj.guannengcc.top

`共 ${n} 条`
来源：http://uwo.gogol.net.cn

[U94] JS：箭头函数
来源：http://lwz.vehdjk.com

const double = x => x * 2;
来源：http://cko.nanxuanxn.top

[U95] JS：Promise 包装
来源：http://jbe.hfpthk.cn

new Promise((resolve, reject) => {})
来源：http://ivr.jyoumei.cn

[U96] JS：async/await 与异常
来源：http://oby.xuanzx.com

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://kxv.jinqigfzy.top

[U97] JS：并发请求
来源：http://ekr.cdnleiting.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://ymj.yj20258.top

[U98] JS：fetch 带 JSON
来源：http://pau.havefunace.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://wmd.hongshengwenyu.top

[U99] JS：事件监听
来源：http://rzo.fktsv.cn

el.addEventListener("click", e => {})
来源：http://zmd.52xcode.cn

[U100] JS：DOM 查询
来源：http://txo.yonumen.top

document.querySelector(".item")
来源：http://grm.yongpay.top

[U101] JS：classList 操作
来源：http://xwv.chenlongwang.top

el.classList.toggle("active")
来源：http://wqu.bjfxy.top

[U102] JS：本地存储
来源：http://hls.birdmap.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://zqx.cucudq.cn

[U103] JS：定时器
来源：http://zdk.pycfn.com

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hnl.shuidangran.top

[U104] JS：防抖
来源：http://kli.shanyushiyangtech.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://gbw.sysykeji.top

[U105] JS：节流
来源：http://rpt.bjfxy.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://ewr.ybcxt.top

[U106] JS：日期格式化
来源：http://ude.guannengcc.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://adh.jlsjyb.cn

[U107] JS：数字千分位
来源：http://tii.aizwys.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://tgx.xingfuxueyuan.xyz

[U108] JS：随机整数
来源：http://wlj.9152youxi.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://qax.sjlbkw.cn

[U109] JS：数组分组
来源：http://fzg.hongshengwenyu.top

Object.groupBy(arr, x => x.type)
来源：http://ias.havefunace.top

[U110] JS：数组分块
来源：http://qrr.fanxiaobao.xyz

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://ien.shuidangran.top

[U111] JS：对象转 Map
来源：http://mjv.sxryk.cn

new Map(Object.entries(obj))
来源：http://dxl.fehbvm.com

[U112] JS：字符串补位
来源：http://pok.yangfankeji.com

"7".padStart(3, "0")
来源：http://wrj.yj20258.top

[U113] JS：正则替换全部
来源：http://ola.yonumen.top

s.replaceAll("a", "b")
来源：http://htg.bjfxy.top

[U114] JS：JSON 深比较
来源：http://zlg.ivvv.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://bmm.xuanzx.com

[U115] JS：生成 UUID
来源：http://zsh.sweek.top

crypto.randomUUID()
来源：http://vbb.ydjk.org.cn

[U116] JS：类型检查（JSDoc）
来源：http://lrm.ctjpmb.com

/** @param {string} name */ function f(name) {}
来源：http://wbd.haohaochexian.top

[U117] JS：单元测试
来源：http://jul.cqqwz.cn

npm i -D vitest;  npx vitest
来源：http://rfm.xingfuxueyuan.xyz

[U118] JS：开发服务器
来源：http://efz.zhongyouzk.top

npm i -D vite;  npx vite
来源：http://icj.aizwys.cn

[U119] JS：生产构建
来源：http://bxr.guannengcc.top

npx vite build
来源：http://ffn.sweek.top

[U120] JS：读取环境变量（Vite）
来源：http://aoh.xingfuxueyuan.xyz

import.meta.env.VITE_API_URL
来源：http://xhy.zhiwuduotai.top

================================================================================
来源：http://uiv.zhengqikj.top

统计汇总
来源：http://dda.daxiang520.top

================================================================================
来源：http://uki.xuetiantiany.cn

按语言统计（条）：
来源：http://nsr.zhixingplan.top

Python ......... 252
来源：http://kls.chenjidiqi.icu

PHP ............ 252
来源：http://jxs.yj202588.top

JavaScript ..... 252
来源：http://gfc.yangfankeji.com

TypeScript ..... 212
来源：http://hud.shzxlz.cn

Java ........... 212
来源：http://rsx.gaohongyu789.top

Go ............. 212
来源：http://jke.yonumen.top

Ruby ........... 212
来源：http://tmt.cucudq.cn

C# ............. 212
来源：http://uvk.jyoumei.cn

C .............. 30
来源：http://pnc.c1oappe.top

C++ ............ 30
来源：http://fub.shzxlz.cn

SQL ............ 90
来源：http://who.cqqwz.cn

Bash ........... 80
来源：http://sls.jinqigfzy.top

Kotlin ......... 15
来源：http://nid.jiagoushi.top

Swift .......... 15
来源：http://tge.yj20258888.top

Lua ............ 10
来源：http://uvd.shanyushiyangkeji.top

Perl ........... 10
来源：http://plx.sysykeji.top

Scala .......... 10
来源：http://zxo.nwbrower.top

------------------------------------
来源：http://fgx.dashuyun.cn

合计 ........... 2106 条
来源：http://upe.316326.xyz

按章节统计：
来源：http://hdt.zhaomingkeji.xyz

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://kcn.gogol.net.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://nbj.aizwys.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://jfp.fengsongda.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://kgf.zhijiandao.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://iab.bjfxy.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://zem.sweek.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://qlt.316326.xyz

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://zff.hesvh.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://zyk.bjfxy.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://mzm.316326.xyz

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://fpz.ydjk.org.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://hum.yuxming.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://kza.chenlongwang.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://efh.fanxiaobao.xyz

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://ztq.feifeiyinyue.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://uju.yj20258888.top

Q SQL 专题                              90
来源：http://bhk.meibo888.top

R Bash 专题                             80
来源：http://ser.yanxiufei.cn

S C / C++ 专题                          60
来源：http://osa.52xcode.cn

T 其他语言补充                          60
来源：http://mil.mhx1999.top

U 高频实用片段                         120
来源：http://vvr.fzhhl.top

------------------------------------
来源：http://fvy.hongshengwenyu.top

合计                                  2106 条
来源：http://dub.yj202588.top

--------------------------------------------------------------------------------
来源：http://ojy.jinghuilouyu.cn

使用提醒
来源：http://lqs.hnqzz.top

--------------------------------------------------------------------------------
来源：http://cpw.zhongyouzk.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://bgb.yj20258888.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://bwl.yangfankeji.com

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://ysg.tian-w.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://mjp.tian-w.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://rmx.wangdashe.top

—— 文件结束 ——
来源：http://zet.kuanghao11.cn

================================================================================
来源：http://esa.vqdsnc.cn

程序语言常见例子速查手册（2024 版）
来源：http://cdg.bbcook.cn

Common Programming Examples Cheat Book
来源：http://qwd.nwbrower.top

================================================================================
来源：http://kpr.ehwqpu.com

【收录内容】
来源：http://lpa.chenjidiqi.icu

覆盖 12 种语言 / 语法与常见 API：
来源：http://jdg.xinyue.icu

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://pax.shanyushiyangkeji.top

SQL · Bash · C · C++
来源：http://zpn.chenzaomai.com

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://ctf.cucudq.cn

【使用说明】
来源：http://tmo.uphjek.com

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://xiy.gzhubu.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://apd.shanyushiyangkeji.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://joh.jinqigfzy.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://omx.fanxiaobao.xyz

Bash:  Shell         C:     C             C++:   C++
来源：http://ilg.fktsv.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://qce.daxiang520.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://asw.jinghuilouyu.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://bmh.meibo888.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://iwr.yueranfly.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://xlo.birdmap.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://suo.cdnleiting.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://ksx.dashuyun.cn

【文件统计】
来源：http://qdx.guowangkeji.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://mkj.yj20258888.top

--------------------------------------------------------------------------------
来源：http://yti.zycfv.cn

目  录
来源：http://qqm.fehbvm.com

--------------------------------------------------------------------------------
来源：http://lza.ctjpmb.com

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://nkk.ehwqpu.com

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://qdo.jinqigfzy.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://jvm.zhiwuduotai.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://nte.dashuyun.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://ody.guowangkeji.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://lec.ydzc1.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://vbb.bjfxy.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://mib.yj20258.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://eld.jianghu66.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://dof.yangfankeji.com

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://qyl.0kj1m.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://pba.52xcode.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://qbx.sysykeji.top


<!-- 参考信息 -->