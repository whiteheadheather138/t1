代发 wailian999

[U17] Py：初始化日志
来源：http://mto.jianghu66.top

logging.basicConfig(level=logging.INFO)
来源：http://zfv.ybcxt.top

[U18] Py：预编译正则
来源：http://azf.ppjwa.cn

pat = re.compile(r"\d+")
来源：http://rki.daxiang520.top

[U19] Py：正则替换带回调
来源：http://jpy.zycfv.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://fyp.yj202588.top

[U20] Py：缓存函数结果
来源：http://gwj.hnxiangtu.top

@functools.lru_cache(maxsize=None)
来源：http://yge.ybcxt.top

[U21] Py：自定义上下文管理器
来源：http://lfr.redwolf501.top

@contextlib.contextmanager
来源：http://crv.cheryme.top

[U22] Py：矩阵转置
来源：http://pif.jiagoushi.top

list(zip(*m))
来源：http://gki.yj20258.top

[U23] Py：分块读取大文件
来源：http://ovc.52xcode.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://fxl.sweek.top

[U24] Py：路径操作
来源：http://wvb.pycfn.com

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://zze.9152youxi.cn

[U25] Py：CSV 按字典读
来源：http://kum.hesvh.cn

csv.DictReader(f)
来源：http://cpf.pengpengdd.cyou

[U26] Py：并发下载
来源：http://szg.yangfankeji.com

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://heu.redwolf501.top

[U27] Py：异步 HTTP
来源：http://dpv.chenzaomai.com

aiohttp.ClientSession() 配合 async with
来源：http://rhw.shanyushiyangkeji.top

[U28] Py：类型别名
来源：http://lrv.dashuyun.cn

UserId = int
来源：http://mqc.ppjwa.cn

[U29] Py：属性校验
来源：http://kfd.cashguo.top

@property 与 @x.setter 配合
来源：http://zid.cdnleiting.top

[U30] Py：数据类
来源：http://upy.tianlin.xyz

@dataclass(slots=True)
来源：http://mck.zhaomingkeji.xyz

[U31] Py：单测
来源：http://abm.yj20258.top

python -m pytest -q
来源：http://vmq.cucudq.cn

[U32] Py：代码格式化
来源：http://tqb.daria6918.cn

ruff format . && ruff check --fix .
来源：http://mso.dashuyun.cn

[U33] Py：打包发布
来源：http://lxk.0kj1m.cn

python -m build  （依赖 pyproject.toml）
来源：http://iwr.aizwys.cn

[U34] Py：判断编码
来源：http://kpg.pengpengdd.cyou

chardet.detect(raw)
来源：http://zdu.uphjek.com

[U35] Py：发送邮件
来源：http://vvx.aibaodan.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://wdy.yfazqb.com

[U36] Py：定时任务
来源：http://lsz.wangdashe.top

schedule.every(10).minutes.do(job)
来源：http://bhh.kuanghao11.cn

[U37] Py：读写 Excel
来源：http://sfv.epnwcf.com

pandas.read_excel / DataFrame.to_excel
来源：http://grn.iojbl.cn

[U38] Py：获取脚本所在目录
来源：http://dxy.ydzc1.top

Path(__file__).resolve().parent
来源：http://ggp.cheryme.top

[U39] Py：判断是否在交互环境
来源：http://yne.fzhhl.top

sys.stdout.isatty()
来源：http://wdc.gotoacloud.top

[U40] Py：打印到标准错误
来源：http://pic.gotoacloud.top

print("err", file=sys.stderr)
来源：http://xbk.zdbjq.cn

[U41] PHP：初始化 Composer 项目
来源：http://fvq.xinyue.icu

composer init;  composer require guzzlehttp/guzzle
来源：http://efl.fengsongda.top

[U42] PHP：PSR-4 自动加载
来源：http://crm.zhixingplan.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://uui.shangyingyoupin.top

[U43] PHP：声明命名空间
来源：http://tae.epnwcf.com

namespace App\Http;
来源：http://kbl.shuidangran.top

[U44] PHP：开启严格类型
来源：http://gqr.shzxlz.cn

declare(strict_types=1);
来源：http://luw.zhixingplan.top

[U45] PHP：类型声明与返回类型
来源：http://rpp.zhengqikj.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://hil.jinqigufen.top

[U46] PHP：可空类型
来源：http://mfw.zhoulong.xyz

?string $name = null
来源：http://wxn.cashguo.top

[U47] PHP：联合类型
来源：http://zem.chenlongwang.top

int|string $id
来源：http://gnm.xinyue.icu

[U48] PHP：纯枚举
来源：http://zmq.jyoumei.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://xws.jinqigufen.top

[U49] PHP：只读属性
来源：http://qfz.hysaishi.cn

public readonly string $name
来源：http://fxe.yj202588.top

[U50] PHP：构造器属性提升
来源：http://kkv.daria6918.cn

public function __construct(private int $id) {}
来源：http://nur.zhixingplan.top

[U51] PHP：数组解构
来源：http://yjp.yj202588.top

[$a, $b] = $arr;
来源：http://gte.hammf.cn

[U52] PHP：箭头函数
来源：http://tqt.yuanzhike.top

$double = fn($x) => $x * 2;
来源：http://vel.sysykeji.top

[U53] PHP：空合并运算符
来源：http://akz.jiagoushi.top

$v = $a ?? $b ?? "default";
来源：http://nmr.c1oappe.top

[U54] PHP：空安全调用
来源：http://ckt.jqgfzy.top

$obj?->method()
来源：http://vhn.nwbrower.top

[U55] PHP：match 表达式
来源：http://ezq.gotoacloud.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hdv.vehdjk.com

[U56] PHP：命名参数
来源：http://dqh.gotoacloud.top

f(a: 1, b: 2)
来源：http://flm.ctjpmb.com

[U57] PHP：字符串插值
来源：http://qgw.pengpengdd.cyou

"值: {$a}"
来源：http://aih.bbcook.cn

[U58] PHP：数组三件套
来源：http://rwc.quarkkingdee.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://laz.jlsjyb.cn

[U59] PHP：自定义排序
来源：http://jvn.chenjidiqi.icu

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://rwz.fehbvm.com

[U60] PHP：JSON 编解码
来源：http://dkn.shanyushiyangkeji.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://qxo.52xcode.cn

[U61] PHP：正则
来源：http://nms.c1oappe.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://sjs.tanke756.top

[U62] PHP：日期对象
来源：http://qkp.hammf.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://arm.yuanzhike.top

[U63] PHP：文件读写
来源：http://swr.hammf.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://rdh.tianlin.xyz

[U64] PHP：目录遍历
来源：http://vsh.gzhubu.top

glob("dir/*.php");  scandir("dir");
来源：http://nww.zhaomingkeji.xyz

[U65] PHP：会话
来源：http://pad.hcnkem.com

session_start();  $_SESSION["uid"] = 1;
来源：http://qas.meibo888.top

[U66] PHP：设置 Cookie
来源：http://dvi.dashuyun.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://ssa.feifeiyinyue.top

[U67] PHP：处理文件上传
来源：http://aqa.tian-w.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://psd.tarul.cn

[U68] PHP：PDO 连接
来源：http://zab.kuanghao11.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://ftw.yvedp.cn

[U69] PHP：PDO 预处理
来源：http://awg.tianlin.xyz

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://nvh.zdbjq.cn

[U70] PHP：PDO 事务
来源：http://xuz.ybcxt.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://vfr.ybcxt.top

[U71] PHP：抛出异常
来源：http://dlu.shuidangran.top

throw new RuntimeException("失败", 500);
来源：http://hzh.yfazqb.com

[U72] PHP：写错误日志
来源：http://cja.redwolf501.top

error_log("失败: " . $e->getMessage());
来源：http://kpf.nwbrower.top

[U73] PHP：读取 ini 配置
来源：http://kda.sufxvd.cn

parse_ini_file("config.ini", true)
来源：http://nly.hcnkem.com

[U74] PHP：读取环境变量
来源：http://bei.jianghu66.top

getenv("APP_ENV") ?: "production"
来源：http://pzv.vqdsnc.cn

[U75] PHP：依赖注入
来源：http://otg.fanxiaobao.xyz

composer require psr/container
来源：http://sra.quarkkingdee.top

[U76] PHP：简单路由
来源：http://kmr.9152youxi.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://fcg.shangyingyoupin.top

[U77] PHP：模板渲染
来源：http://fbh.zhoulong.xyz

composer require twig/twig
来源：http://eaa.yj202588.top

[U78] PHP：单元测试
来源：http://rlj.xylfe.cn

composer require --dev phpunit/phpunit
来源：http://fuv.wangdashe.top

[U79] PHP：静态分析
来源：http://pqh.smart0.xyz

composer require --dev phpstan/phpstan
来源：http://pwe.nwbrower.top

[U80] PHP：代码规范修复
来源：http://exi.yuxming.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://lzw.yanxiufei.cn

[U81] JS：初始化项目
来源：http://dbe.yj20258888.top

npm init -y;  npm i express
来源：http://dre.gaohongyu789.top

[U82] JS：package.json 脚本
来源：http://dfb.ivvv.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://vyh.gogol.net.cn

[U83] JS：ES Module 导入导出
来源：http://fqz.svipenyu.cn

export const a = 1;  import { a } from "./m.js";
来源：http://izm.haohaochexian.top

[U84] JS：CommonJS 写法
来源：http://okl.gotoacloud.top

module.exports = { a };  const { a } = require("./m");
来源：http://ccx.shanyushiyangtech.top

[U85] JS：可选链
来源：http://yvx.aizwys.cn

a?.b?.c
来源：http://qot.gaohongyu789.top

[U86] JS：空值合并
来源：http://dsj.tarul.cn

a ?? b
来源：http://xmr.hcnkem.com

[U87] JS：解构默认值
来源：http://gbl.meibo888.top

const { a = 1, b = 2 } = obj;
来源：http://xxy.sufxvd.cn

[U88] JS：对象展开合并
来源：http://cuu.wangshuangyany.cn

{ ...a, ...b }
来源：http://jtv.xingfuxueyuan.xyz

[U89] JS：数组去重
来源：http://lwa.dianchejie.cn

[...new Set(arr)]
来源：http://vxn.haohaochexian.top

[U90] JS：数字数组排序
来源：http://ozm.yonumen.top

[...arr].sort((a, b) => a - b)
来源：http://rwx.fehbvm.com

[U91] JS：对象键值遍历
来源：http://lul.ybcxt.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://cms.smart0.xyz

[U92] JS：深拷贝
来源：http://hfy.chenzaomai.com

structuredClone(obj)
来源：http://mdl.zdqjudy.top

[U93] JS：模板字符串
来源：http://vam.haohaochexian.top

`共 ${n} 条`
来源：http://lni.cqqwz.cn

[U94] JS：箭头函数
来源：http://jsg.yuanzhike.top

const double = x => x * 2;
来源：http://dse.jlsjyb.cn

[U95] JS：Promise 包装
来源：http://icq.nanxinkj.top

new Promise((resolve, reject) => {})
来源：http://eqs.shuidangran.top

[U96] JS：async/await 与异常
来源：http://cwh.daria6918.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://jlv.bjfxy.top

[U97] JS：并发请求
来源：http://cee.yueranfly.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://xqp.ybcxt.top

[U98] JS：fetch 带 JSON
来源：http://skl.aizwys.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://bpr.shzxlz.cn

[U99] JS：事件监听
来源：http://cua.ybcxt.top

el.addEventListener("click", e => {})
来源：http://cbj.yuxming.cn

[U100] JS：DOM 查询
来源：http://ykr.jianghu66.top

document.querySelector(".item")
来源：http://svq.havefunace.top

[U101] JS：classList 操作
来源：http://oxv.zhixingplan.top

el.classList.toggle("active")
来源：http://fxo.tianlin.xyz

[U102] JS：本地存储
来源：http://xop.ydjk.org.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://nzm.daxiang520.top

[U103] JS：定时器
来源：http://uuf.tanke756.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://yze.uphjek.com

[U104] JS：防抖
来源：http://yrs.sufxvd.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://yau.gotoacloud.top

[U105] JS：节流
来源：http://dog.nanxinkj.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://vdq.yanxiufei.cn

[U106] JS：日期格式化
来源：http://fja.chenzaomai.com

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://bco.jqgufenzy.top

[U107] JS：数字千分位
来源：http://fos.tanke756.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://rxz.c1oappe.top

[U108] JS：随机整数
来源：http://kjp.zhaomingkeji.xyz

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://ojw.yangfankeji.com

[U109] JS：数组分组
来源：http://ewx.aibaodan.cn

Object.groupBy(arr, x => x.type)
来源：http://cmg.hysaishi.cn

[U110] JS：数组分块
来源：http://czx.redwolf501.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://idx.aizwys.cn

[U111] JS：对象转 Map
来源：http://jui.xingfuxueyuan.xyz

new Map(Object.entries(obj))
来源：http://bzg.hywenlv.cn

[U112] JS：字符串补位
来源：http://rkx.redwolf501.top

"7".padStart(3, "0")
来源：http://bdh.zhixingplan.top

[U113] JS：正则替换全部
来源：http://brz.shangyingyoupin.top

s.replaceAll("a", "b")
来源：http://ckh.daria6918.cn

[U114] JS：JSON 深比较
来源：http://nsb.jinqigfzy.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://vbt.yj202588.top

[U115] JS：生成 UUID
来源：http://ymm.fengsongda.top

crypto.randomUUID()
来源：http://kmg.ctjpmb.com

[U116] JS：类型检查（JSDoc）
来源：http://tkp.jyoumei.cn

/** @param {string} name */ function f(name) {}
来源：http://gmt.nanxinkj.top

[U117] JS：单元测试
来源：http://duo.shanyushiyangkeji.top

npm i -D vitest;  npx vitest
来源：http://ugk.havefunace.top

[U118] JS：开发服务器
来源：http://bnk.xziqi.cn

npm i -D vite;  npx vite
来源：http://zsl.jinqigfzy.top

[U119] JS：生产构建
来源：http://nqa.aibaodan.cn

npx vite build
来源：http://mjl.cashguo.top

[U120] JS：读取环境变量（Vite）
来源：http://ntd.yj20258888.top

import.meta.env.VITE_API_URL
来源：http://enn.ppjwa.cn

================================================================================
来源：http://ltp.jiagoushi.top

统计汇总
来源：http://pgr.nwbrower.top

================================================================================
来源：http://mvx.hfpthk.cn

按语言统计（条）：
来源：http://eex.yj20258.top

Python ......... 252
来源：http://lvt.smart0.xyz

PHP ............ 252
来源：http://ynu.hnxiangtu.top

JavaScript ..... 252
来源：http://ghb.fehbvm.com

TypeScript ..... 212
来源：http://oxi.ybcxt.top

Java ........... 212
来源：http://vbq.redwolf501.top

Go ............. 212
来源：http://dzf.gaohongyu789.top

Ruby ........... 212
来源：http://ylo.chenlongwang.top

C# ............. 212
来源：http://top.aizwys.cn

C .............. 30
来源：http://huy.fktsv.cn

C++ ............ 30
来源：http://cdr.ywan-chungtsiang.top

SQL ............ 90
来源：http://spj.yj20258888.top

Bash ........... 80
来源：http://kua.uphjek.com

Kotlin ......... 15
来源：http://hax.zdbjq.cn

Swift .......... 15
来源：http://tkn.cheryme.top

Lua ............ 10
来源：http://tkm.tanke756.top

Perl ........... 10
来源：http://ewk.jinghuilouyu.cn

Scala .......... 10
来源：http://kzu.jiagoushi.top

------------------------------------
来源：http://wkl.dianchejie.cn

合计 ........... 2106 条
来源：http://fwt.xinyue.icu

按章节统计：
来源：http://ndi.sjlbkw.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://ylw.epnwcf.com

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://znb.52xcode.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://tek.yuxming.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://zdp.epnwcf.com

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://qgm.ppjwa.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://qol.zhixingplan.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://cln.kuanghao11.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://vjy.52xcode.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://afb.guannengcc.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://rze.yj20258.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://rml.zhengqikj.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://yki.zhaomingkeji.xyz

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://mmx.jiagoushi.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://tcf.ybcxt.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://qnx.smart0.xyz

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://hcw.iojbl.cn

Q SQL 专题                              90
来源：http://kit.yuxming.cn

R Bash 专题                             80
来源：http://hjh.pycfn.com

S C / C++ 专题                          60
来源：http://wae.feifeiyinyue.top

T 其他语言补充                          60
来源：http://bwl.hcnkem.com

U 高频实用片段                         120
来源：http://msw.guannengcc.top

------------------------------------
来源：http://xcc.xuanzx.com

合计                                  2106 条
来源：http://itn.hysaishi.cn

--------------------------------------------------------------------------------
来源：http://xue.feifeiyinyue.top

使用提醒
来源：http://tqw.cheryme.top

--------------------------------------------------------------------------------
来源：http://hbw.52xcode.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://ppj.gzhubu.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://ggv.xinyue.icu

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://tlu.zdbjq.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://imj.zycfv.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://fey.shanyushiyangtech.top

—— 文件结束 ——
来源：http://jnt.fengsongda.top

================================================================================
来源：http://nyk.jinghuilouyu.cn

程序语言常见例子速查手册（2024 版）
来源：http://vrf.yj202588.top

Common Programming Examples Cheat Book
来源：http://oew.dashuyun.cn

================================================================================
来源：http://mxd.yj202588.top

【收录内容】
来源：http://zaf.redwolf501.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://ynw.0kj1m.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://ecc.iojbl.cn

SQL · Bash · C · C++
来源：http://tau.snrcjt.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://nci.snrcjt.cn

【使用说明】
来源：http://fcu.jinghuilouyu.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://rej.chenzaomai.com

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://iru.haohaochexian.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://vvv.yongpay.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://voi.xziqi.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://llk.ydzc1.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://dcq.jinyuanbaomall.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://hcc.9152youxi.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://azz.fzhhl.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://ylw.ppjwa.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://agb.ehwqpu.com

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://zid.52xcode.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://lci.birdmap.top

【文件统计】
来源：http://vvo.tanke756.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://esc.zdqjudy.top

--------------------------------------------------------------------------------
来源：http://fja.cqqwz.cn

目  录
来源：http://anq.jlsjyb.cn

--------------------------------------------------------------------------------
来源：http://okk.sysykeji.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://iee.ybcxt.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://huo.sufxvd.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://rpy.epnwcf.com

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://xfl.smart0.xyz

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://hbi.zhaomingkeji.xyz

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://obh.epnwcf.com

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://qcr.ivvv.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://sop.iojbl.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://lbq.chenzaomai.com


<!-- 参考信息 -->