代发 wailian999

[U19] Py：正则替换带回调
来源：http://xmt.ywan-chungtsiang.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://dpq.gzhubu.top

[U20] Py：缓存函数结果
来源：http://qlv.jyoumei.cn

@functools.lru_cache(maxsize=None)
来源：http://mwd.jianghu66.top

[U21] Py：自定义上下文管理器
来源：http://wuc.jqgfzy.top

@contextlib.contextmanager
来源：http://bwt.wangshuangyany.cn

[U22] Py：矩阵转置
来源：http://aox.daria6918.cn

list(zip(*m))
来源：http://mpm.gzhubu.top

[U23] Py：分块读取大文件
来源：http://std.sweek.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://vdh.hnxiangtu.top

[U24] Py：路径操作
来源：http://mpq.guannengcc.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://pyy.aibaodan.cn

[U25] Py：CSV 按字典读
来源：http://dzk.tianlin.xyz

csv.DictReader(f)
来源：http://uwv.tanke756.top

[U26] Py：并发下载
来源：http://ebn.sjlbkw.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://xzu.bjfxy.top

[U27] Py：异步 HTTP
来源：http://dwm.52xcode.cn

aiohttp.ClientSession() 配合 async with
来源：http://nld.hcnkem.com

[U28] Py：类型别名
来源：http://smb.dashuyun.cn

UserId = int
来源：http://apt.hywenlv.cn

[U29] Py：属性校验
来源：http://bwr.meibo888.top

@property 与 @x.setter 配合
来源：http://hko.shzxlz.cn

[U30] Py：数据类
来源：http://rwe.chenjidiqi.icu

@dataclass(slots=True)
来源：http://pnm.jinyuanbaomall.cn

[U31] Py：单测
来源：http://hji.shangyingyoupin.top

python -m pytest -q
来源：http://jvo.meibo888.top

[U32] Py：代码格式化
来源：http://luo.ctjpmb.com

ruff format . && ruff check --fix .
来源：http://fau.cashguo.top

[U33] Py：打包发布
来源：http://pfq.xinyue.icu

python -m build  （依赖 pyproject.toml）
来源：http://ktk.dashuyun.cn

[U34] Py：判断编码
来源：http://qyl.cheryme.top

chardet.detect(raw)
来源：http://tii.yj20258888.top

[U35] Py：发送邮件
来源：http://law.uphjek.com

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://zmd.haohaochexian.top

[U36] Py：定时任务
来源：http://ntq.smart0.xyz

schedule.every(10).minutes.do(job)
来源：http://bdf.ywan-chungtsiang.top

[U37] Py：读写 Excel
来源：http://qok.havefunace.top

pandas.read_excel / DataFrame.to_excel
来源：http://fzi.hongshengwenyu.top

[U38] Py：获取脚本所在目录
来源：http://eca.andypj.xyz

Path(__file__).resolve().parent
来源：http://rjl.meibo888.top

[U39] Py：判断是否在交互环境
来源：http://wsw.hfpthk.cn

sys.stdout.isatty()
来源：http://uib.nwbrower.top

[U40] Py：打印到标准错误
来源：http://tik.daria6918.cn

print("err", file=sys.stderr)
来源：http://ymw.yj20258888.top

[U41] PHP：初始化 Composer 项目
来源：http://yry.feifeiyinyue.top

composer init;  composer require guzzlehttp/guzzle
来源：http://onj.hysaishi.cn

[U42] PHP：PSR-4 自动加载
来源：http://oef.bjfxy.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://bqd.shanyushiyangtech.top

[U43] PHP：声明命名空间
来源：http://xsf.yuxming.cn

namespace App\Http;
来源：http://rcd.chenzaomai.com

[U44] PHP：开启严格类型
来源：http://hxq.pengpengdd.cyou

declare(strict_types=1);
来源：http://wuj.fehbvm.com

[U45] PHP：类型声明与返回类型
来源：http://ipr.nanxuanxn.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://xrt.shuidangran.top

[U46] PHP：可空类型
来源：http://rgy.ywan-chungtsiang.top

?string $name = null
来源：http://yyf.svipenyu.cn

[U47] PHP：联合类型
来源：http://vwq.birdmap.top

int|string $id
来源：http://kdy.nanxinkj.top

[U48] PHP：纯枚举
来源：http://awy.pengpengdd.cyou

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://xfg.shuidangran.top

[U49] PHP：只读属性
来源：http://ooy.zhongyouzk.top

public readonly string $name
来源：http://ian.0kj1m.cn

[U50] PHP：构造器属性提升
来源：http://lzd.bbcook.cn

public function __construct(private int $id) {}
来源：http://idj.yuanzhike.top

[U51] PHP：数组解构
来源：http://qgr.wangshuangyany.cn

[$a, $b] = $arr;
来源：http://auc.jiagoushi.top

[U52] PHP：箭头函数
来源：http://aah.shangyingyoupin.top

$double = fn($x) => $x * 2;
来源：http://yzy.redwolf501.top

[U53] PHP：空合并运算符
来源：http://uum.xinyue.icu

$v = $a ?? $b ?? "default";
来源：http://rao.yuxming.cn

[U54] PHP：空安全调用
来源：http://ptm.hcnkem.com

$obj?->method()
来源：http://deu.ivvv.top

[U55] PHP：match 表达式
来源：http://wrg.52xcode.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://tsz.ydzc1.top

[U56] PHP：命名参数
来源：http://qik.jiagoushi.top

f(a: 1, b: 2)
来源：http://ewz.smart0.xyz

[U57] PHP：字符串插值
来源：http://ngv.guowangkeji.top

"值: {$a}"
来源：http://ryb.sweek.top

[U58] PHP：数组三件套
来源：http://vtz.sysykeji.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://csx.meibo888.top

[U59] PHP：自定义排序
来源：http://ggq.zhixingplan.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://qoq.xinyue.icu

[U60] PHP：JSON 编解码
来源：http://zov.meibo888.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://ghf.redwolf501.top

[U61] PHP：正则
来源：http://ojf.yonumen.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://qki.shangyingyoupin.top

[U62] PHP：日期对象
来源：http://urw.jinyuanbaomall.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://wnk.gotoacloud.top

[U63] PHP：文件读写
来源：http://kuj.jlsjyb.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://mtx.yj202588.top

[U64] PHP：目录遍历
来源：http://bxc.bbcook.cn

glob("dir/*.php");  scandir("dir");
来源：http://vys.chenlongwang.top

[U65] PHP：会话
来源：http://pfv.zhixingplan.top

session_start();  $_SESSION["uid"] = 1;
来源：http://gmc.tanke756.top

[U66] PHP：设置 Cookie
来源：http://gfo.zhiwuduotai.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://tpr.ehwqpu.com

[U67] PHP：处理文件上传
来源：http://zku.daxiang520.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://iws.xingfuxueyuan.xyz

[U68] PHP：PDO 连接
来源：http://lec.cashguo.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://una.cashguo.top

[U69] PHP：PDO 预处理
来源：http://mcz.hesvh.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://iwx.tianlin.xyz

[U70] PHP：PDO 事务
来源：http://yks.hfpthk.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://nge.bbcook.cn

[U71] PHP：抛出异常
来源：http://jjg.bjfxy.top

throw new RuntimeException("失败", 500);
来源：http://olh.aibaodan.cn

[U72] PHP：写错误日志
来源：http://wfj.pycfn.com

error_log("失败: " . $e->getMessage());
来源：http://syq.aizwys.cn

[U73] PHP：读取 ini 配置
来源：http://rgn.jlsjyb.cn

parse_ini_file("config.ini", true)
来源：http://eig.kuanghao11.cn

[U74] PHP：读取环境变量
来源：http://ulr.shanyushiyangkeji.top

getenv("APP_ENV") ?: "production"
来源：http://cpx.epnwcf.com

[U75] PHP：依赖注入
来源：http://toj.daxiang520.top

composer require psr/container
来源：http://xjw.cucudq.cn

[U76] PHP：简单路由
来源：http://rem.hysaishi.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://ilm.zhongyouzk.top

[U77] PHP：模板渲染
来源：http://rlv.fehbvm.com

composer require twig/twig
来源：http://iqd.zhixingplan.top

[U78] PHP：单元测试
来源：http://kee.yueranfly.top

composer require --dev phpunit/phpunit
来源：http://bzb.cucudq.cn

[U79] PHP：静态分析
来源：http://bma.ctjpmb.com

composer require --dev phpstan/phpstan
来源：http://msi.52xcode.cn

[U80] PHP：代码规范修复
来源：http://eaq.ivvv.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://rie.jinyuanbaomall.cn

[U81] JS：初始化项目
来源：http://hwa.redwolf501.top

npm init -y;  npm i express
来源：http://vlr.xinyue.icu

[U82] JS：package.json 脚本
来源：http://quu.jinghuilouyu.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://sfb.nwbrower.top

[U83] JS：ES Module 导入导出
来源：http://wiq.cucudq.cn

export const a = 1;  import { a } from "./m.js";
来源：http://lfw.tarul.cn

[U84] JS：CommonJS 写法
来源：http://ymz.gzhubu.top

module.exports = { a };  const { a } = require("./m");
来源：http://vfd.birdmap.top

[U85] JS：可选链
来源：http://tyd.hfpthk.cn

a?.b?.c
来源：http://ppb.hywenlv.cn

[U86] JS：空值合并
来源：http://wuc.gotoacloud.top

a ?? b
来源：http://njx.yueranfly.top

[U87] JS：解构默认值
来源：http://pju.hesvh.cn

const { a = 1, b = 2 } = obj;
来源：http://mzw.aibaodan.cn

[U88] JS：对象展开合并
来源：http://ogf.aibaodan.cn

{ ...a, ...b }
来源：http://hug.pengpengdd.cyou

[U89] JS：数组去重
来源：http://wsp.zhengqikj.top

[...new Set(arr)]
来源：http://cbf.redwolf501.top

[U90] JS：数字数组排序
来源：http://yxb.haohaochexian.top

[...arr].sort((a, b) => a - b)
来源：http://njc.xylfe.cn

[U91] JS：对象键值遍历
来源：http://pyp.kuanghao11.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://cwj.dianchejie.cn

[U92] JS：深拷贝
来源：http://gbc.hnxiangtu.top

structuredClone(obj)
来源：http://uwr.birdmap.top

[U93] JS：模板字符串
来源：http://cbk.bjfxy.top

`共 ${n} 条`
来源：http://nxq.dianchejie.cn

[U94] JS：箭头函数
来源：http://xru.316326.xyz

const double = x => x * 2;
来源：http://amt.haohaochexian.top

[U95] JS：Promise 包装
来源：http://bys.pycfn.com

new Promise((resolve, reject) => {})
来源：http://abs.ydzc1.top

[U96] JS：async/await 与异常
来源：http://ldi.jyoumei.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://lws.chenjidiqi.icu

[U97] JS：并发请求
来源：http://nja.xingfuxueyuan.xyz

await Promise.all(urls.map(u => fetch(u)))
来源：http://wcs.fktsv.cn

[U98] JS：fetch 带 JSON
来源：http://csc.daxiang520.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://woj.chenzaomai.com

[U99] JS：事件监听
来源：http://koi.jinyuanbaomall.cn

el.addEventListener("click", e => {})
来源：http://gyj.zhongyouzk.top

[U100] JS：DOM 查询
来源：http://xqo.52xcode.cn

document.querySelector(".item")
来源：http://ewk.uphjek.com

[U101] JS：classList 操作
来源：http://vcb.ydzc1.top

el.classList.toggle("active")
来源：http://zre.tanke756.top

[U102] JS：本地存储
来源：http://ieu.aizwys.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://dtg.hammf.cn

[U103] JS：定时器
来源：http://trz.xingfuxueyuan.xyz

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://yac.yvedp.cn

[U104] JS：防抖
来源：http://oyw.smart0.xyz

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://spu.yangfankeji.com

[U105] JS：节流
来源：http://yrr.fzhhl.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://gke.jlsjyb.cn

[U106] JS：日期格式化
来源：http://jli.xziqi.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://kzq.havefunace.top

[U107] JS：数字千分位
来源：http://cvo.nwbrower.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://ipg.chenjidiqi.icu

[U108] JS：随机整数
来源：http://odd.tianlin.xyz

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://her.epnwcf.com

[U109] JS：数组分组
来源：http://mia.gotoacloud.top

Object.groupBy(arr, x => x.type)
来源：http://xey.meibo888.top

[U110] JS：数组分块
来源：http://kxr.pengpengdd.cyou

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://qfc.zycfv.cn

[U111] JS：对象转 Map
来源：http://nqm.smart0.xyz

new Map(Object.entries(obj))
来源：http://jik.daria6918.cn

[U112] JS：字符串补位
来源：http://pzz.fengsongda.top

"7".padStart(3, "0")
来源：http://eww.ehwqpu.com

[U113] JS：正则替换全部
来源：http://nci.yvedp.cn

s.replaceAll("a", "b")
来源：http://igt.hesvh.cn

[U114] JS：JSON 深比较
来源：http://jys.gotoacloud.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://seu.cheryme.top

[U115] JS：生成 UUID
来源：http://kbe.yj20258.top

crypto.randomUUID()
来源：http://gwt.zhiwuduotai.top

[U116] JS：类型检查（JSDoc）
来源：http://nrf.jlsjyb.cn

/** @param {string} name */ function f(name) {}
来源：http://ffx.daria6918.cn

[U117] JS：单元测试
来源：http://zih.dianchejie.cn

npm i -D vitest;  npx vitest
来源：http://wah.wangshuangyany.cn

[U118] JS：开发服务器
来源：http://npl.chenjidiqi.icu

npm i -D vite;  npx vite
来源：http://pmn.xuetiantiany.cn

[U119] JS：生产构建
来源：http://kgg.aibaodan.cn

npx vite build
来源：http://qtq.ctjpmb.com

[U120] JS：读取环境变量（Vite）
来源：http://xty.hfpthk.cn

import.meta.env.VITE_API_URL
来源：http://txm.uphjek.com

================================================================================
来源：http://zss.zhijiandao.cn

统计汇总
来源：http://zip.aizwys.cn

================================================================================
来源：http://jik.zhiwuduotai.top

按语言统计（条）：
来源：http://pgz.smart0.xyz

Python ......... 252
来源：http://cll.daria6918.cn

PHP ............ 252
来源：http://toe.zdbjq.cn

JavaScript ..... 252
来源：http://juz.ctjpmb.com

TypeScript ..... 212
来源：http://ivq.yuxming.cn

Java ........... 212
来源：http://ixw.hcnkem.com

Go ............. 212
来源：http://get.dianchejie.cn

Ruby ........... 212
来源：http://kal.kuanghao11.cn

C# ............. 212
来源：http://gnk.yj20258.top

C .............. 30
来源：http://dks.xingfuxueyuan.xyz

C++ ............ 30
来源：http://tua.zdqjudy.top

SQL ............ 90
来源：http://gol.jinghuilouyu.cn

Bash ........... 80
来源：http://fns.jyoumei.cn

Kotlin ......... 15
来源：http://gff.daria6918.cn

Swift .......... 15
来源：http://seb.andypj.xyz

Lua ............ 10
来源：http://wsp.jlsjyb.cn

Perl ........... 10
来源：http://oxv.dianchejie.cn

Scala .......... 10
来源：http://jka.hysaishi.cn

------------------------------------
来源：http://fsx.feifeiyinyue.top

合计 ........... 2106 条
来源：http://wmf.redwolf501.top

按章节统计：
来源：http://xjk.cqqwz.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://gfy.tianlin.xyz

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://enc.smart0.xyz

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://jhd.cqqwz.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://zto.fanxiaobao.xyz

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://fdi.shanyushiyangkeji.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://gty.wangshuangyany.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://kwe.svipenyu.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://faa.mhx1999.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://lfg.xylfe.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://eta.jlsjyb.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://lif.gotoacloud.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://cpt.chenlongwang.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://ada.aibaodan.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://mif.hnxiangtu.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://nlq.tarul.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://ppv.ivvv.top

Q SQL 专题                              90
来源：http://cjy.uphjek.com

R Bash 专题                             80
来源：http://abo.chenlongwang.top

S C / C++ 专题                          60
来源：http://dtt.xziqi.cn

T 其他语言补充                          60
来源：http://bex.daria6918.cn

U 高频实用片段                         120
来源：http://ggy.xinyue.icu

------------------------------------
来源：http://qcz.guowangkeji.top

合计                                  2106 条
来源：http://pop.fehbvm.com

--------------------------------------------------------------------------------
来源：http://nws.jianghu66.top

使用提醒
来源：http://zzp.cucudq.cn

--------------------------------------------------------------------------------
来源：http://qlx.jyoumei.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://lku.kuanghao11.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://auc.ydzc1.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://tts.nwbrower.top

在旧版本上使用前请先确认语法支持情况。
来源：http://krk.yuanzhike.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://vgm.gzhubu.top

—— 文件结束 ——
来源：http://lgw.redwolf501.top

================================================================================
来源：http://wwv.dashuyun.cn

程序语言常见例子速查手册（2024 版）
来源：http://oxi.xuanzx.com

Common Programming Examples Cheat Book
来源：http://dcr.yvedp.cn

================================================================================
来源：http://yfx.yanxiufei.cn

【收录内容】
来源：http://skw.daxiang520.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://ipn.zycfv.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://sot.tanke756.top

SQL · Bash · C · C++
来源：http://ewr.zdbjq.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://mnh.havefunace.top

【使用说明】
来源：http://vms.vehdjk.com

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://trh.ybcxt.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://cxk.jqgufenzy.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://erf.jinqigfzy.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://tgx.tanke756.top

Bash:  Shell         C:     C             C++:   C++
来源：http://seo.316326.xyz

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://nns.kuanghao11.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://yde.tian-w.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://bzd.daxiang520.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://fui.sufxvd.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://qcg.bbcook.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://nar.cheryme.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://lvi.hysaishi.cn

【文件统计】
来源：http://tmj.shanyushiyangtech.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://ywr.zhiwuduotai.top

--------------------------------------------------------------------------------
来源：http://mmz.ppjwa.cn

目  录
来源：http://ftv.fengsongda.top

--------------------------------------------------------------------------------
来源：http://jwt.hysaishi.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://tlr.hesvh.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://ulf.cqqwz.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://ssv.pengpengdd.cyou

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://hmw.sxryk.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://xtz.ybcxt.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://cme.smart0.xyz

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://dtq.ctjpmb.com

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://sxz.wangshuangyany.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://gic.yvedp.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://fqm.sweek.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://kpz.zycfv.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://zgi.zdqjudy.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://bej.jiagoushi.top


<!-- 参考信息 -->