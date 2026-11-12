代发 wailian999

[U19] Py：正则替换带回调
来源：http://yhb.jyoumei.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://mli.zhixingplan.top

[U20] Py：缓存函数结果
来源：http://dlf.fehbvm.com

@functools.lru_cache(maxsize=None)
来源：http://khr.andypj.xyz

[U21] Py：自定义上下文管理器
来源：http://elb.jinghuilouyu.cn

@contextlib.contextmanager
来源：http://hpe.sxryk.cn

[U22] Py：矩阵转置
来源：http://lfx.redwolf501.top

list(zip(*m))
来源：http://isx.cdnleiting.top

[U23] Py：分块读取大文件
来源：http://irj.shanyushiyangkeji.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://nsc.52xcode.cn

[U24] Py：路径操作
来源：http://yll.vehdjk.com

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://tst.zdqjudy.top

[U25] Py：CSV 按字典读
来源：http://iso.hnqzz.top

csv.DictReader(f)
来源：http://pov.yueranfly.top

[U26] Py：并发下载
来源：http://gri.feifeiyinyue.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://tfv.birdmap.top

[U27] Py：异步 HTTP
来源：http://hvs.redwolf501.top

aiohttp.ClientSession() 配合 async with
来源：http://mwq.hfpthk.cn

[U28] Py：类型别名
来源：http://rku.vqdsnc.cn

UserId = int
来源：http://leq.sxryk.cn

[U29] Py：属性校验
来源：http://nxi.quarkkingdee.top

@property 与 @x.setter 配合
来源：http://cjb.tarul.cn

[U30] Py：数据类
来源：http://sxt.sjlbkw.cn

@dataclass(slots=True)
来源：http://awf.shanyushiyangtech.top

[U31] Py：单测
来源：http://ctv.hnxiangtu.top

python -m pytest -q
来源：http://rnl.cdnleiting.top

[U32] Py：代码格式化
来源：http://soa.andypj.xyz

ruff format . && ruff check --fix .
来源：http://jpl.yongpay.top

[U33] Py：打包发布
来源：http://sss.jyoumei.cn

python -m build  （依赖 pyproject.toml）
来源：http://hjf.epnwcf.com

[U34] Py：判断编码
来源：http://pwl.ehwqpu.com

chardet.detect(raw)
来源：http://szk.cqqwz.cn

[U35] Py：发送邮件
来源：http://zuz.tian-w.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://bpu.zhijiandao.cn

[U36] Py：定时任务
来源：http://okf.zhoulong.xyz

schedule.every(10).minutes.do(job)
来源：http://sod.cheryme.top

[U37] Py：读写 Excel
来源：http://myj.jinghuilouyu.cn

pandas.read_excel / DataFrame.to_excel
来源：http://xlx.fanxiaobao.xyz

[U38] Py：获取脚本所在目录
来源：http://iud.tarul.cn

Path(__file__).resolve().parent
来源：http://ekd.haohaochexian.top

[U39] Py：判断是否在交互环境
来源：http://zkd.fengsongda.top

sys.stdout.isatty()
来源：http://jcd.shanyushiyangtech.top

[U40] Py：打印到标准错误
来源：http://ryy.nanxinkj.top

print("err", file=sys.stderr)
来源：http://ioe.hysaishi.cn

[U41] PHP：初始化 Composer 项目
来源：http://lzw.ydzc1.top

composer init;  composer require guzzlehttp/guzzle
来源：http://cww.yj20258.top

[U42] PHP：PSR-4 自动加载
来源：http://esb.cheryme.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://bap.aibaodan.cn

[U43] PHP：声明命名空间
来源：http://bkb.fehbvm.com

namespace App\Http;
来源：http://hcg.shangyingyoupin.top

[U44] PHP：开启严格类型
来源：http://ppf.yangfankeji.com

declare(strict_types=1);
来源：http://xyd.yj20258888.top

[U45] PHP：类型声明与返回类型
来源：http://hvq.zhaomingkeji.xyz

function add(int $a, int $b): int { return $a + $b; }
来源：http://xcr.yonumen.top

[U46] PHP：可空类型
来源：http://emw.zhaomingkeji.xyz

?string $name = null
来源：http://exx.zhijiandao.cn

[U47] PHP：联合类型
来源：http://zym.andypj.xyz

int|string $id
来源：http://lmo.yvedp.cn

[U48] PHP：纯枚举
来源：http://vvc.fanxiaobao.xyz

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://xws.tianlin.xyz

[U49] PHP：只读属性
来源：http://fwr.zhiwuduotai.top

public readonly string $name
来源：http://fyz.ydzc1.top

[U50] PHP：构造器属性提升
来源：http://tfv.haohaochexian.top

public function __construct(private int $id) {}
来源：http://dcs.ydjk.org.cn

[U51] PHP：数组解构
来源：http://ekm.ywan-chungtsiang.top

[$a, $b] = $arr;
来源：http://xnw.hesvh.cn

[U52] PHP：箭头函数
来源：http://onn.ppjwa.cn

$double = fn($x) => $x * 2;
来源：http://lwx.sxryk.cn

[U53] PHP：空合并运算符
来源：http://mro.yueranfly.top

$v = $a ?? $b ?? "default";
来源：http://czr.jyoumei.cn

[U54] PHP：空安全调用
来源：http://gag.sweek.top

$obj?->method()
来源：http://jmt.jqgufenzy.top

[U55] PHP：match 表达式
来源：http://veh.pycfn.com

$s = match($x) { 1 => "一", default => "其他" };
来源：http://huz.cdnleiting.top

[U56] PHP：命名参数
来源：http://jqa.svipenyu.cn

f(a: 1, b: 2)
来源：http://kux.daria6918.cn

[U57] PHP：字符串插值
来源：http://rqs.meibo888.top

"值: {$a}"
来源：http://apa.gogol.net.cn

[U58] PHP：数组三件套
来源：http://wdo.vehdjk.com

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://tqt.kuanghao11.cn

[U59] PHP：自定义排序
来源：http://mol.andypj.xyz

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://tfa.yanxiufei.cn

[U60] PHP：JSON 编解码
来源：http://tsj.wangshuangyany.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://app.cdnleiting.top

[U61] PHP：正则
来源：http://xpq.smart0.xyz

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://fgo.0kj1m.cn

[U62] PHP：日期对象
来源：http://joj.dashuyun.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://imi.hammf.cn

[U63] PHP：文件读写
来源：http://prp.yuxming.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://czd.yongpay.top

[U64] PHP：目录遍历
来源：http://yuy.nanxinkj.top

glob("dir/*.php");  scandir("dir");
来源：http://gsh.sysykeji.top

[U65] PHP：会话
来源：http://lsu.hfpthk.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://izd.zhaomingkeji.xyz

[U66] PHP：设置 Cookie
来源：http://pdr.bjfxy.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://ozw.fanxiaobao.xyz

[U67] PHP：处理文件上传
来源：http://ack.shuidangran.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://pyd.wangdashe.top

[U68] PHP：PDO 连接
来源：http://ksy.birdmap.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://nin.xinyue.icu

[U69] PHP：PDO 预处理
来源：http://izc.gaohongyu789.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://bit.epnwcf.com

[U70] PHP：PDO 事务
来源：http://gqd.iojbl.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://kyk.316326.xyz

[U71] PHP：抛出异常
来源：http://pvw.yanxiufei.cn

throw new RuntimeException("失败", 500);
来源：http://ewj.hesvh.cn

[U72] PHP：写错误日志
来源：http://khe.shzxlz.cn

error_log("失败: " . $e->getMessage());
来源：http://fxt.jinyuanbaomall.cn

[U73] PHP：读取 ini 配置
来源：http://qul.yangfankeji.com

parse_ini_file("config.ini", true)
来源：http://zoj.mhx1999.top

[U74] PHP：读取环境变量
来源：http://lkk.ywan-chungtsiang.top

getenv("APP_ENV") ?: "production"
来源：http://hgt.xziqi.cn

[U75] PHP：依赖注入
来源：http://duw.feifeiyinyue.top

composer require psr/container
来源：http://rfj.hcnkem.com

[U76] PHP：简单路由
来源：http://ghi.uphjek.com

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://hkw.hnxiangtu.top

[U77] PHP：模板渲染
来源：http://rom.sufxvd.cn

composer require twig/twig
来源：http://qcs.tanke756.top

[U78] PHP：单元测试
来源：http://din.xziqi.cn

composer require --dev phpunit/phpunit
来源：http://dvk.sysykeji.top

[U79] PHP：静态分析
来源：http://ksl.sxryk.cn

composer require --dev phpstan/phpstan
来源：http://goz.gotoacloud.top

[U80] PHP：代码规范修复
来源：http://mve.gotoacloud.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://sgr.xylfe.cn

[U81] JS：初始化项目
来源：http://dgu.jiagoushi.top

npm init -y;  npm i express
来源：http://cwv.guannengcc.top

[U82] JS：package.json 脚本
来源：http://wbf.gzhubu.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://wbs.guowangkeji.top

[U83] JS：ES Module 导入导出
来源：http://rxi.ehwqpu.com

export const a = 1;  import { a } from "./m.js";
来源：http://dow.jiagoushi.top

[U84] JS：CommonJS 写法
来源：http://atn.hnxiangtu.top

module.exports = { a };  const { a } = require("./m");
来源：http://hqo.tianlin.xyz

[U85] JS：可选链
来源：http://tis.jlsjyb.cn

a?.b?.c
来源：http://hbi.chenjidiqi.icu

[U86] JS：空值合并
来源：http://skz.jinqigufen.top

a ?? b
来源：http://ctc.daxiang520.top

[U87] JS：解构默认值
来源：http://fdj.gzhubu.top

const { a = 1, b = 2 } = obj;
来源：http://pei.guowangkeji.top

[U88] JS：对象展开合并
来源：http://dvc.yj20258888.top

{ ...a, ...b }
来源：http://oyw.tianlin.xyz

[U89] JS：数组去重
来源：http://puq.xuetiantiany.cn

[...new Set(arr)]
来源：http://dbi.shanyushiyangkeji.top

[U90] JS：数字数组排序
来源：http://qns.fktsv.cn

[...arr].sort((a, b) => a - b)
来源：http://xqe.shanyushiyangkeji.top

[U91] JS：对象键值遍历
来源：http://ark.yj202588.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://jzp.jlsjyb.cn

[U92] JS：深拷贝
来源：http://hor.dashuyun.cn

structuredClone(obj)
来源：http://pra.pengpengdd.cyou

[U93] JS：模板字符串
来源：http://zjd.yvedp.cn

`共 ${n} 条`
来源：http://ful.smart0.xyz

[U94] JS：箭头函数
来源：http://qxu.xuetiantiany.cn

const double = x => x * 2;
来源：http://vme.nwbrower.top

[U95] JS：Promise 包装
来源：http://zpn.guowangkeji.top

new Promise((resolve, reject) => {})
来源：http://flw.hammf.cn

[U96] JS：async/await 与异常
来源：http://sfl.xuanzx.com

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://dcz.shanyushiyangkeji.top

[U97] JS：并发请求
来源：http://kct.daxiang520.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://odl.shzxlz.cn

[U98] JS：fetch 带 JSON
来源：http://kdg.cashguo.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://sxn.xylfe.cn

[U99] JS：事件监听
来源：http://yzh.epnwcf.com

el.addEventListener("click", e => {})
来源：http://kfv.jianghu66.top

[U100] JS：DOM 查询
来源：http://fvw.yj202588.top

document.querySelector(".item")
来源：http://yua.meibo888.top

[U101] JS：classList 操作
来源：http://vcf.sjlbkw.cn

el.classList.toggle("active")
来源：http://hto.shangyingyoupin.top

[U102] JS：本地存储
来源：http://qbw.hnxiangtu.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://dxh.chenzaomai.com

[U103] JS：定时器
来源：http://tha.hysaishi.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://chy.yvedp.cn

[U104] JS：防抖
来源：http://lrj.fktsv.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://fze.fktsv.cn

[U105] JS：节流
来源：http://blx.pengpengdd.cyou

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://tcy.jqgufenzy.top

[U106] JS：日期格式化
来源：http://cng.shzxlz.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://jca.bbcook.cn

[U107] JS：数字千分位
来源：http://hmh.yj202588.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://bdm.zdbjq.cn

[U108] JS：随机整数
来源：http://lrf.zhiwuduotai.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://ulj.hysaishi.cn

[U109] JS：数组分组
来源：http://cuq.hcnkem.com

Object.groupBy(arr, x => x.type)
来源：http://cjn.fehbvm.com

[U110] JS：数组分块
来源：http://fzj.hnqzz.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://gvv.ehwqpu.com

[U111] JS：对象转 Map
来源：http://wzv.shzxlz.cn

new Map(Object.entries(obj))
来源：http://mkx.yongpay.top

[U112] JS：字符串补位
来源：http://nni.316326.xyz

"7".padStart(3, "0")
来源：http://kfz.meibo888.top

[U113] JS：正则替换全部
来源：http://cbd.chenzaomai.com

s.replaceAll("a", "b")
来源：http://mfb.yuxming.cn

[U114] JS：JSON 深比较
来源：http://ghh.ppjwa.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://zpf.zhijiandao.cn

[U115] JS：生成 UUID
来源：http://grm.bbcook.cn

crypto.randomUUID()
来源：http://pkr.hysaishi.cn

[U116] JS：类型检查（JSDoc）
来源：http://fbl.redwolf501.top

/** @param {string} name */ function f(name) {}
来源：http://exs.tarul.cn

[U117] JS：单元测试
来源：http://sah.zhaomingkeji.xyz

npm i -D vitest;  npx vitest
来源：http://rmm.sysykeji.top

[U118] JS：开发服务器
来源：http://sko.ywan-chungtsiang.top

npm i -D vite;  npx vite
来源：http://ynb.xziqi.cn

[U119] JS：生产构建
来源：http://avi.cucudq.cn

npx vite build
来源：http://mrh.ydjk.org.cn

[U120] JS：读取环境变量（Vite）
来源：http://hmq.yanxiufei.cn

import.meta.env.VITE_API_URL
来源：http://inv.tanke756.top

================================================================================
来源：http://khv.zhixingplan.top

统计汇总
来源：http://kvc.yonumen.top

================================================================================
来源：http://ohj.jlsjyb.cn

按语言统计（条）：
来源：http://peu.hysaishi.cn

Python ......... 252
来源：http://fgd.yj202588.top

PHP ............ 252
来源：http://ofn.ydzc1.top

JavaScript ..... 252
来源：http://qkc.yj20258.top

TypeScript ..... 212
来源：http://iex.jinghuilouyu.cn

Java ........... 212
来源：http://lfz.quarkkingdee.top

Go ............. 212
来源：http://saf.chenzaomai.com

Ruby ........... 212
来源：http://dcs.xylfe.cn

C# ............. 212
来源：http://lzb.0kj1m.cn

C .............. 30
来源：http://iwh.52xcode.cn

C++ ............ 30
来源：http://ioj.guowangkeji.top

SQL ............ 90
来源：http://qzh.zhongyouzk.top

Bash ........... 80
来源：http://kin.xylfe.cn

Kotlin ......... 15
来源：http://ovl.tarul.cn

Swift .......... 15
来源：http://csx.shzxlz.cn

Lua ............ 10
来源：http://yun.zhaomingkeji.xyz

Perl ........... 10
来源：http://qyz.zhoulong.xyz

Scala .......... 10
来源：http://dmp.shuidangran.top

------------------------------------
来源：http://fxt.zycfv.cn

合计 ........... 2106 条
来源：http://bck.uphjek.com

按章节统计：
来源：http://afz.hongshengwenyu.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://rmg.vqdsnc.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://cel.yuanzhike.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://gja.gotoacloud.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://pnf.fehbvm.com

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://vap.hywenlv.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://dga.smart0.xyz

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://owg.uphjek.com

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://mre.xinyue.icu

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://mts.yongpay.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://mow.chenlongwang.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://gqr.xuetiantiany.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://jui.shanyushiyangtech.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://qxw.wangshuangyany.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://erj.vqdsnc.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://zdz.fktsv.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://inj.hammf.cn

Q SQL 专题                              90
来源：http://fas.fengsongda.top

R Bash 专题                             80
来源：http://rqp.chenzaomai.com

S C / C++ 专题                          60
来源：http://bcp.hnqzz.top

T 其他语言补充                          60
来源：http://idz.yfazqb.com

U 高频实用片段                         120
来源：http://bjn.uphjek.com

------------------------------------
来源：http://lhc.feifeiyinyue.top

合计                                  2106 条
来源：http://foo.zdbjq.cn

--------------------------------------------------------------------------------
来源：http://cox.hcnkem.com

使用提醒
来源：http://zxx.shanyushiyangkeji.top

--------------------------------------------------------------------------------
来源：http://erv.wangdashe.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://boi.birdmap.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://kus.fktsv.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://hck.sysykeji.top

在旧版本上使用前请先确认语法支持情况。
来源：http://lgb.sysykeji.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://drv.fzhhl.top

—— 文件结束 ——
来源：http://djf.wangdashe.top

================================================================================
来源：http://xpe.zhengqikj.top

程序语言常见例子速查手册（2024 版）
来源：http://acz.nwbrower.top

Common Programming Examples Cheat Book
来源：http://udo.cucudq.cn

================================================================================
来源：http://xmx.sjlbkw.cn

【收录内容】
来源：http://plj.tarul.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://kkd.yj202588.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://nlr.zhongyouzk.top

SQL · Bash · C · C++
来源：http://qrb.cdnleiting.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://grw.gogol.net.cn

【使用说明】
来源：http://knt.dashuyun.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://gjn.sjlbkw.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://ldq.hcnkem.com

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://qma.xziqi.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://tey.hysaishi.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://luh.yuxming.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://vhr.feifeiyinyue.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://psm.hnqzz.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://fpz.yuxming.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://avt.shzxlz.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://kkt.xylfe.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://iel.shzxlz.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://ftw.pengpengdd.cyou

【文件统计】
来源：http://cjh.ehwqpu.com

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://bny.ivvv.top

--------------------------------------------------------------------------------
来源：http://vlg.zhaomingkeji.xyz

目  录
来源：http://hkb.hysaishi.cn

--------------------------------------------------------------------------------
来源：http://kpe.bjfxy.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://jmw.svipenyu.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://hiv.jianghu66.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://jsi.nanxuanxn.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://mgl.jinyuanbaomall.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://vxq.zhiwuduotai.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://ome.fzhhl.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://ova.andypj.xyz

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://cvx.52xcode.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://xma.aibaodan.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://gkb.xziqi.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://ggq.yvedp.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://cds.yj20258.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://pob.zhiwuduotai.top


<!-- 参考信息 -->