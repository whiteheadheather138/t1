代发 wailian999

[U19] Py：正则替换带回调
来源：http://stl.jlsjyb.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://kjz.hammf.cn

[U20] Py：缓存函数结果
来源：http://gal.chenjidiqi.icu

@functools.lru_cache(maxsize=None)
来源：http://gwt.xuetiantiany.cn

[U21] Py：自定义上下文管理器
来源：http://alw.hnxiangtu.top

@contextlib.contextmanager
来源：http://wsl.ydjk.org.cn

[U22] Py：矩阵转置
来源：http://ucn.shanyushiyangkeji.top

list(zip(*m))
来源：http://yzm.chenjidiqi.icu

[U23] Py：分块读取大文件
来源：http://ljv.ybcxt.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://ivd.yfazqb.com

[U24] Py：路径操作
来源：http://mcv.shzxlz.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://wlj.hywenlv.cn

[U25] Py：CSV 按字典读
来源：http://dwj.jinqigufen.top

csv.DictReader(f)
来源：http://myk.zdqjudy.top

[U26] Py：并发下载
来源：http://utc.aizwys.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://bbe.hysaishi.cn

[U27] Py：异步 HTTP
来源：http://pdn.zhaomingkeji.xyz

aiohttp.ClientSession() 配合 async with
来源：http://ddp.haohaochexian.top

[U28] Py：类型别名
来源：http://kfk.wangdashe.top

UserId = int
来源：http://mbr.zdbjq.cn

[U29] Py：属性校验
来源：http://exx.sufxvd.cn

@property 与 @x.setter 配合
来源：http://syy.kuanghao11.cn

[U30] Py：数据类
来源：http://rla.havefunace.top

@dataclass(slots=True)
来源：http://dlb.gzhubu.top

[U31] Py：单测
来源：http://xbx.xinyue.icu

python -m pytest -q
来源：http://pjr.gotoacloud.top

[U32] Py：代码格式化
来源：http://ubt.zhoulong.xyz

ruff format . && ruff check --fix .
来源：http://ccg.uphjek.com

[U33] Py：打包发布
来源：http://mto.shuidangran.top

python -m build  （依赖 pyproject.toml）
来源：http://djc.jinqigufen.top

[U34] Py：判断编码
来源：http://jph.yuanzhike.top

chardet.detect(raw)
来源：http://oqm.uphjek.com

[U35] Py：发送邮件
来源：http://cba.quarkkingdee.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://syt.sxryk.cn

[U36] Py：定时任务
来源：http://pnc.zycfv.cn

schedule.every(10).minutes.do(job)
来源：http://aal.sjlbkw.cn

[U37] Py：读写 Excel
来源：http://vgq.xziqi.cn

pandas.read_excel / DataFrame.to_excel
来源：http://dlc.birdmap.top

[U38] Py：获取脚本所在目录
来源：http://ttc.sjlbkw.cn

Path(__file__).resolve().parent
来源：http://cny.feifeiyinyue.top

[U39] Py：判断是否在交互环境
来源：http://kpc.cqqwz.cn

sys.stdout.isatty()
来源：http://okj.fehbvm.com

[U40] Py：打印到标准错误
来源：http://ouq.hfpthk.cn

print("err", file=sys.stderr)
来源：http://vbj.guannengcc.top

[U41] PHP：初始化 Composer 项目
来源：http://hbl.gotoacloud.top

composer init;  composer require guzzlehttp/guzzle
来源：http://hpy.nanxuanxn.top

[U42] PHP：PSR-4 自动加载
来源：http://mqj.shzxlz.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://boc.yj202588.top

[U43] PHP：声明命名空间
来源：http://kis.smart0.xyz

namespace App\Http;
来源：http://tdi.daria6918.cn

[U44] PHP：开启严格类型
来源：http://xre.quarkkingdee.top

declare(strict_types=1);
来源：http://bng.havefunace.top

[U45] PHP：类型声明与返回类型
来源：http://ghr.chenjidiqi.icu

function add(int $a, int $b): int { return $a + $b; }
来源：http://kct.jinqigufen.top

[U46] PHP：可空类型
来源：http://gwr.jinqigfzy.top

?string $name = null
来源：http://xgt.yonumen.top

[U47] PHP：联合类型
来源：http://ois.xuanzx.com

int|string $id
来源：http://apb.jqgfzy.top

[U48] PHP：纯枚举
来源：http://lhy.yuanzhike.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://xht.tian-w.cn

[U49] PHP：只读属性
来源：http://syc.jianghu66.top

public readonly string $name
来源：http://nnv.smart0.xyz

[U50] PHP：构造器属性提升
来源：http://fvu.chenlongwang.top

public function __construct(private int $id) {}
来源：http://nec.gzhubu.top

[U51] PHP：数组解构
来源：http://sdt.jiagoushi.top

[$a, $b] = $arr;
来源：http://czt.jinqigufen.top

[U52] PHP：箭头函数
来源：http://ixi.shangyingyoupin.top

$double = fn($x) => $x * 2;
来源：http://iup.ivvv.top

[U53] PHP：空合并运算符
来源：http://znb.yj20258.top

$v = $a ?? $b ?? "default";
来源：http://jdh.snrcjt.cn

[U54] PHP：空安全调用
来源：http://kli.meibo888.top

$obj?->method()
来源：http://nmo.andypj.xyz

[U55] PHP：match 表达式
来源：http://xiv.xziqi.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://qis.havefunace.top

[U56] PHP：命名参数
来源：http://xaw.jinghuilouyu.cn

f(a: 1, b: 2)
来源：http://xxt.ybcxt.top

[U57] PHP：字符串插值
来源：http://opc.xinyue.icu

"值: {$a}"
来源：http://jwz.sysykeji.top

[U58] PHP：数组三件套
来源：http://gkq.shanyushiyangtech.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://klx.sxryk.cn

[U59] PHP：自定义排序
来源：http://zjk.tanke756.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://rit.svipenyu.cn

[U60] PHP：JSON 编解码
来源：http://nhs.nanxinkj.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://vqd.xuanzx.com

[U61] PHP：正则
来源：http://nrh.redwolf501.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://nqp.shangyingyoupin.top

[U62] PHP：日期对象
来源：http://gyf.xuetiantiany.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://pte.zhengqikj.top

[U63] PHP：文件读写
来源：http://chc.andypj.xyz

file_get_contents($f);  file_put_contents($f, $data);
来源：http://rwf.snrcjt.cn

[U64] PHP：目录遍历
来源：http://dxu.zhongyouzk.top

glob("dir/*.php");  scandir("dir");
来源：http://sum.fanxiaobao.xyz

[U65] PHP：会话
来源：http://gta.ppjwa.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://gcz.sweek.top

[U66] PHP：设置 Cookie
来源：http://xjd.9152youxi.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://yfr.bbcook.cn

[U67] PHP：处理文件上传
来源：http://frb.ydzc1.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://szg.zhiwuduotai.top

[U68] PHP：PDO 连接
来源：http://bht.ehwqpu.com

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://sqq.ivvv.top

[U69] PHP：PDO 预处理
来源：http://uml.sysykeji.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://bqo.vehdjk.com

[U70] PHP：PDO 事务
来源：http://gfm.cqqwz.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://aga.guowangkeji.top

[U71] PHP：抛出异常
来源：http://fsz.xylfe.cn

throw new RuntimeException("失败", 500);
来源：http://ozf.hywenlv.cn

[U72] PHP：写错误日志
来源：http://rah.kuanghao11.cn

error_log("失败: " . $e->getMessage());
来源：http://lyx.xziqi.cn

[U73] PHP：读取 ini 配置
来源：http://yhl.ywan-chungtsiang.top

parse_ini_file("config.ini", true)
来源：http://bjv.0kj1m.cn

[U74] PHP：读取环境变量
来源：http://bmp.yj20258888.top

getenv("APP_ENV") ?: "production"
来源：http://lda.aibaodan.cn

[U75] PHP：依赖注入
来源：http://gnn.zhaomingkeji.xyz

composer require psr/container
来源：http://tgt.tanke756.top

[U76] PHP：简单路由
来源：http://plv.quarkkingdee.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://geb.snrcjt.cn

[U77] PHP：模板渲染
来源：http://ozj.uphjek.com

composer require twig/twig
来源：http://sbx.zhixingplan.top

[U78] PHP：单元测试
来源：http://ulb.guowangkeji.top

composer require --dev phpunit/phpunit
来源：http://six.xuetiantiany.cn

[U79] PHP：静态分析
来源：http://gse.quarkkingdee.top

composer require --dev phpstan/phpstan
来源：http://snl.ppjwa.cn

[U80] PHP：代码规范修复
来源：http://niv.xuanzx.com

composer require --dev friendsofphp/php-cs-fixer
来源：http://cnc.nanxuanxn.top

[U81] JS：初始化项目
来源：http://auz.hfpthk.cn

npm init -y;  npm i express
来源：http://ydh.guowangkeji.top

[U82] JS：package.json 脚本
来源：http://ymr.hammf.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://zlj.tarul.cn

[U83] JS：ES Module 导入导出
来源：http://xyq.52xcode.cn

export const a = 1;  import { a } from "./m.js";
来源：http://esu.ywan-chungtsiang.top

[U84] JS：CommonJS 写法
来源：http://kma.tianlin.xyz

module.exports = { a };  const { a } = require("./m");
来源：http://mxh.daxiang520.top

[U85] JS：可选链
来源：http://muk.ydzc1.top

a?.b?.c
来源：http://zqf.jqgufenzy.top

[U86] JS：空值合并
来源：http://msx.shanyushiyangtech.top

a ?? b
来源：http://bmh.xylfe.cn

[U87] JS：解构默认值
来源：http://mqz.yangfankeji.com

const { a = 1, b = 2 } = obj;
来源：http://ybo.hcnkem.com

[U88] JS：对象展开合并
来源：http://gos.jyoumei.cn

{ ...a, ...b }
来源：http://aae.guannengcc.top

[U89] JS：数组去重
来源：http://byw.hnqzz.top

[...new Set(arr)]
来源：http://ebo.cucudq.cn

[U90] JS：数字数组排序
来源：http://vxu.hammf.cn

[...arr].sort((a, b) => a - b)
来源：http://vzs.feifeiyinyue.top

[U91] JS：对象键值遍历
来源：http://mdt.xylfe.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://zll.9152youxi.cn

[U92] JS：深拷贝
来源：http://cjn.yfazqb.com

structuredClone(obj)
来源：http://ooi.ehwqpu.com

[U93] JS：模板字符串
来源：http://kal.chenlongwang.top

`共 ${n} 条`
来源：http://fsu.shanyushiyangtech.top

[U94] JS：箭头函数
来源：http://tiw.svipenyu.cn

const double = x => x * 2;
来源：http://wzt.yfazqb.com

[U95] JS：Promise 包装
来源：http://dbx.shanyushiyangtech.top

new Promise((resolve, reject) => {})
来源：http://lrf.yanxiufei.cn

[U96] JS：async/await 与异常
来源：http://npz.cdnleiting.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://wyw.yvedp.cn

[U97] JS：并发请求
来源：http://yul.smart0.xyz

await Promise.all(urls.map(u => fetch(u)))
来源：http://fmx.gaohongyu789.top

[U98] JS：fetch 带 JSON
来源：http://laj.smart0.xyz

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://iuk.guannengcc.top

[U99] JS：事件监听
来源：http://bmd.guannengcc.top

el.addEventListener("click", e => {})
来源：http://vgx.svipenyu.cn

[U100] JS：DOM 查询
来源：http://bvn.yangfankeji.com

document.querySelector(".item")
来源：http://mra.yfazqb.com

[U101] JS：classList 操作
来源：http://kxq.xuanzx.com

el.classList.toggle("active")
来源：http://jom.316326.xyz

[U102] JS：本地存储
来源：http://ucg.redwolf501.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://iep.hnqzz.top

[U103] JS：定时器
来源：http://iwm.cucudq.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://wbi.tian-w.cn

[U104] JS：防抖
来源：http://qon.sufxvd.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://fqt.vqdsnc.cn

[U105] JS：节流
来源：http://xao.tarul.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://uvo.quarkkingdee.top

[U106] JS：日期格式化
来源：http://qby.yongpay.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://xrh.0kj1m.cn

[U107] JS：数字千分位
来源：http://whq.meibo888.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://lvh.hnqzz.top

[U108] JS：随机整数
来源：http://mvw.ywan-chungtsiang.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://jmh.quarkkingdee.top

[U109] JS：数组分组
来源：http://tje.smart0.xyz

Object.groupBy(arr, x => x.type)
来源：http://aeg.zycfv.cn

[U110] JS：数组分块
来源：http://jhs.fanxiaobao.xyz

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://zjb.pycfn.com

[U111] JS：对象转 Map
来源：http://fqg.hnqzz.top

new Map(Object.entries(obj))
来源：http://nee.jinyuanbaomall.cn

[U112] JS：字符串补位
来源：http://kep.daxiang520.top

"7".padStart(3, "0")
来源：http://ggy.tianlin.xyz

[U113] JS：正则替换全部
来源：http://oqm.tarul.cn

s.replaceAll("a", "b")
来源：http://aeb.sweek.top

[U114] JS：JSON 深比较
来源：http://uqg.gotoacloud.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://zvt.ehwqpu.com

[U115] JS：生成 UUID
来源：http://mqr.yuanzhike.top

crypto.randomUUID()
来源：http://awv.tian-w.cn

[U116] JS：类型检查（JSDoc）
来源：http://ocy.shangyingyoupin.top

/** @param {string} name */ function f(name) {}
来源：http://txz.dashuyun.cn

[U117] JS：单元测试
来源：http://cdb.yfazqb.com

npm i -D vitest;  npx vitest
来源：http://czm.zhaomingkeji.xyz

[U118] JS：开发服务器
来源：http://wnl.zycfv.cn

npm i -D vite;  npx vite
来源：http://kda.jiagoushi.top

[U119] JS：生产构建
来源：http://xvp.chenzaomai.com

npx vite build
来源：http://noo.chenlongwang.top

[U120] JS：读取环境变量（Vite）
来源：http://lfj.zdqjudy.top

import.meta.env.VITE_API_URL
来源：http://xdn.xuetiantiany.cn

================================================================================
来源：http://wjt.vqdsnc.cn

统计汇总
来源：http://feu.zdbjq.cn

================================================================================
来源：http://pjp.tarul.cn

按语言统计（条）：
来源：http://aye.yuanzhike.top

Python ......... 252
来源：http://pcn.hysaishi.cn

PHP ............ 252
来源：http://lmm.yj202588.top

JavaScript ..... 252
来源：http://mjr.wangshuangyany.cn

TypeScript ..... 212
来源：http://rzt.cdnleiting.top

Java ........... 212
来源：http://apu.zdbjq.cn

Go ............. 212
来源：http://slp.daria6918.cn

Ruby ........... 212
来源：http://oqd.daxiang520.top

C# ............. 212
来源：http://ppj.ybcxt.top

C .............. 30
来源：http://wqr.wangdashe.top

C++ ............ 30
来源：http://eby.hcnkem.com

SQL ............ 90
来源：http://ddn.jiagoushi.top

Bash ........... 80
来源：http://qtj.xziqi.cn

Kotlin ......... 15
来源：http://bdm.meibo888.top

Swift .......... 15
来源：http://exc.snrcjt.cn

Lua ............ 10
来源：http://jax.pycfn.com

Perl ........... 10
来源：http://ssa.guowangkeji.top

Scala .......... 10
来源：http://zmk.zhijiandao.cn

------------------------------------
来源：http://tmv.zhaomingkeji.xyz

合计 ........... 2106 条
来源：http://nvf.meibo888.top

按章节统计：
来源：http://ilf.cheryme.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://ees.fzhhl.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://grq.zhoulong.xyz

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://qur.xylfe.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://obl.tianlin.xyz

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://ksd.zdqjudy.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://lbe.meibo888.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://duh.sweek.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hnr.zycfv.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://lsi.ctjpmb.com

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://sht.ybcxt.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://ojb.xingfuxueyuan.xyz

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://rbr.hywenlv.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://las.daria6918.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://ssq.gogol.net.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://sfk.cdnleiting.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://pzz.feifeiyinyue.top

Q SQL 专题                              90
来源：http://lkj.xuetiantiany.cn

R Bash 专题                             80
来源：http://wne.fktsv.cn

S C / C++ 专题                          60
来源：http://jfm.yj202588.top

T 其他语言补充                          60
来源：http://lhq.birdmap.top

U 高频实用片段                         120
来源：http://ofv.guannengcc.top

------------------------------------
来源：http://aab.fzhhl.top

合计                                  2106 条
来源：http://gpd.cdnleiting.top

--------------------------------------------------------------------------------
来源：http://arv.gaohongyu789.top

使用提醒
来源：http://afo.guowangkeji.top

--------------------------------------------------------------------------------
来源：http://kvv.dashuyun.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://ygq.hywenlv.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://mnq.aibaodan.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://wew.xingfuxueyuan.xyz

在旧版本上使用前请先确认语法支持情况。
来源：http://vdn.fktsv.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://fhl.wangshuangyany.cn

—— 文件结束 ——
来源：http://irb.haohaochexian.top

================================================================================
来源：http://wrj.guowangkeji.top

程序语言常见例子速查手册（2024 版）
来源：http://uqr.mhx1999.top

Common Programming Examples Cheat Book
来源：http://fgq.ivvv.top

================================================================================
来源：http://wjj.hammf.cn

【收录内容】
来源：http://klv.aizwys.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://hzf.jlsjyb.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://uag.hnqzz.top

SQL · Bash · C · C++
来源：http://lmi.vqdsnc.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://ngf.hesvh.cn

【使用说明】
来源：http://gos.hammf.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://eaw.xylfe.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://nkr.hcnkem.com

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://hfh.gotoacloud.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://wxj.ybcxt.top

Bash:  Shell         C:     C             C++:   C++
来源：http://xlo.gotoacloud.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://jem.ctjpmb.com

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://zbt.yj202588.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://gcg.52xcode.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://fuh.wangdashe.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://yuh.hnxiangtu.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://grj.pengpengdd.cyou

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://hoz.xingfuxueyuan.xyz

【文件统计】
来源：http://abt.ctjpmb.com

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://rih.yangfankeji.com

--------------------------------------------------------------------------------
来源：http://xcf.jinghuilouyu.cn

目  录
来源：http://zqv.0kj1m.cn

--------------------------------------------------------------------------------
来源：http://abn.dashuyun.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://bzn.chenlongwang.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://nld.tian-w.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://ofe.yj202588.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://gyu.jyoumei.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://fsc.svipenyu.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://tzw.shangyingyoupin.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://nmf.yongpay.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://qgq.yanxiufei.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://sbh.aizwys.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://vve.fanxiaobao.xyz

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://ygm.smart0.xyz

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://qxy.hnxiangtu.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://ywj.uphjek.com


<!-- 参考信息 -->