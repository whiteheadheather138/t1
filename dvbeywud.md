代发 wailian999

[U17] Py：初始化日志
来源：http://vwm.xinyue.icu

logging.basicConfig(level=logging.INFO)
来源：http://dvb.daria6918.cn

[U18] Py：预编译正则
来源：http://vwv.nwbrower.top

pat = re.compile(r"\d+")
来源：http://mrt.sysykeji.top

[U19] Py：正则替换带回调
来源：http://kxc.hongshengwenyu.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://mhl.aibaodan.cn

[U20] Py：缓存函数结果
来源：http://fmt.jlsjyb.cn

@functools.lru_cache(maxsize=None)
来源：http://dsf.gaohongyu789.top

[U21] Py：自定义上下文管理器
来源：http://wle.yonumen.top

@contextlib.contextmanager
来源：http://dna.uphjek.com

[U22] Py：矩阵转置
来源：http://fog.jinqigfzy.top

list(zip(*m))
来源：http://qem.hongshengwenyu.top

[U23] Py：分块读取大文件
来源：http://qaf.smart0.xyz

for chunk in iter(lambda: f.read(8192), b""):
来源：http://ihy.xziqi.cn

[U24] Py：路径操作
来源：http://nmc.dashuyun.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://rzi.tanke756.top

[U25] Py：CSV 按字典读
来源：http://ofn.epnwcf.com

csv.DictReader(f)
来源：http://onh.shanyushiyangtech.top

[U26] Py：并发下载
来源：http://bzd.jinyuanbaomall.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://yig.gzhubu.top

[U27] Py：异步 HTTP
来源：http://imr.nwbrower.top

aiohttp.ClientSession() 配合 async with
来源：http://hzx.sysykeji.top

[U28] Py：类型别名
来源：http://bvm.shangyingyoupin.top

UserId = int
来源：http://riz.vqdsnc.cn

[U29] Py：属性校验
来源：http://wsd.sysykeji.top

@property 与 @x.setter 配合
来源：http://odv.epnwcf.com

[U30] Py：数据类
来源：http://hzu.jinqigfzy.top

@dataclass(slots=True)
来源：http://sul.zhengqikj.top

[U31] Py：单测
来源：http://vox.haohaochexian.top

python -m pytest -q
来源：http://xdb.birdmap.top

[U32] Py：代码格式化
来源：http://kfn.fehbvm.com

ruff format . && ruff check --fix .
来源：http://spo.zhijiandao.cn

[U33] Py：打包发布
来源：http://jim.svipenyu.cn

python -m build  （依赖 pyproject.toml）
来源：http://dgp.meibo888.top

[U34] Py：判断编码
来源：http://tjt.zdqjudy.top

chardet.detect(raw)
来源：http://rmk.ydzc1.top

[U35] Py：发送邮件
来源：http://yia.yvedp.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://jgt.tianlin.xyz

[U36] Py：定时任务
来源：http://eon.meibo888.top

schedule.every(10).minutes.do(job)
来源：http://apq.hesvh.cn

[U37] Py：读写 Excel
来源：http://xvr.nanxinkj.top

pandas.read_excel / DataFrame.to_excel
来源：http://ejk.ywan-chungtsiang.top

[U38] Py：获取脚本所在目录
来源：http://ltf.tianlin.xyz

Path(__file__).resolve().parent
来源：http://qdp.ehwqpu.com

[U39] Py：判断是否在交互环境
来源：http://mfq.gogol.net.cn

sys.stdout.isatty()
来源：http://nnc.jiagoushi.top

[U40] Py：打印到标准错误
来源：http://pff.chenlongwang.top

print("err", file=sys.stderr)
来源：http://kef.shanyushiyangtech.top

[U41] PHP：初始化 Composer 项目
来源：http://kzj.jlsjyb.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://jdm.yongpay.top

[U42] PHP：PSR-4 自动加载
来源：http://zhz.ydjk.org.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://ukd.iojbl.cn

[U43] PHP：声明命名空间
来源：http://fkp.cdnleiting.top

namespace App\Http;
来源：http://jdh.ivvv.top

[U44] PHP：开启严格类型
来源：http://paj.fehbvm.com

declare(strict_types=1);
来源：http://meu.haohaochexian.top

[U45] PHP：类型声明与返回类型
来源：http://byz.feifeiyinyue.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://veq.sweek.top

[U46] PHP：可空类型
来源：http://ukf.xuetiantiany.cn

?string $name = null
来源：http://wfb.snrcjt.cn

[U47] PHP：联合类型
来源：http://vnz.gaohongyu789.top

int|string $id
来源：http://pdg.mhx1999.top

[U48] PHP：纯枚举
来源：http://ymn.yvedp.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://jae.chenlongwang.top

[U49] PHP：只读属性
来源：http://twf.ybcxt.top

public readonly string $name
来源：http://tjr.c1oappe.top

[U50] PHP：构造器属性提升
来源：http://clx.tarul.cn

public function __construct(private int $id) {}
来源：http://cni.zhaomingkeji.xyz

[U51] PHP：数组解构
来源：http://qdd.yuxming.cn

[$a, $b] = $arr;
来源：http://isp.sjlbkw.cn

[U52] PHP：箭头函数
来源：http://fsb.cheryme.top

$double = fn($x) => $x * 2;
来源：http://ymg.sweek.top

[U53] PHP：空合并运算符
来源：http://hbf.zdqjudy.top

$v = $a ?? $b ?? "default";
来源：http://xsp.zhixingplan.top

[U54] PHP：空安全调用
来源：http://fom.andypj.xyz

$obj?->method()
来源：http://ibh.jianghu66.top

[U55] PHP：match 表达式
来源：http://jof.yonumen.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://oor.tianlin.xyz

[U56] PHP：命名参数
来源：http://yfa.zhengqikj.top

f(a: 1, b: 2)
来源：http://wtj.jianghu66.top

[U57] PHP：字符串插值
来源：http://pxm.sweek.top

"值: {$a}"
来源：http://mgo.meibo888.top

[U58] PHP：数组三件套
来源：http://fcc.hywenlv.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://lzx.zhoulong.xyz

[U59] PHP：自定义排序
来源：http://xpy.hcnkem.com

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://yib.jinyuanbaomall.cn

[U60] PHP：JSON 编解码
来源：http://syb.bjfxy.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://gpd.0kj1m.cn

[U61] PHP：正则
来源：http://eei.xziqi.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://zrv.fktsv.cn

[U62] PHP：日期对象
来源：http://prf.xinyue.icu

(new DateTimeImmutable())->format("Y-m-d");
来源：http://iuz.ydjk.org.cn

[U63] PHP：文件读写
来源：http://vds.havefunace.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://eas.sxryk.cn

[U64] PHP：目录遍历
来源：http://wvz.smart0.xyz

glob("dir/*.php");  scandir("dir");
来源：http://byy.cqqwz.cn

[U65] PHP：会话
来源：http://szj.xingfuxueyuan.xyz

session_start();  $_SESSION["uid"] = 1;
来源：http://orz.0kj1m.cn

[U66] PHP：设置 Cookie
来源：http://xec.dianchejie.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://xjq.yuxming.cn

[U67] PHP：处理文件上传
来源：http://gul.meibo888.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://hpu.ppjwa.cn

[U68] PHP：PDO 连接
来源：http://mgy.andypj.xyz

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://mvr.cqqwz.cn

[U69] PHP：PDO 预处理
来源：http://kxi.xylfe.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://baf.sufxvd.cn

[U70] PHP：PDO 事务
来源：http://ibd.fanxiaobao.xyz

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://yxh.ydjk.org.cn

[U71] PHP：抛出异常
来源：http://iac.sufxvd.cn

throw new RuntimeException("失败", 500);
来源：http://lpn.bjfxy.top

[U72] PHP：写错误日志
来源：http://cdy.yj20258888.top

error_log("失败: " . $e->getMessage());
来源：http://uyh.birdmap.top

[U73] PHP：读取 ini 配置
来源：http://wjw.hnqzz.top

parse_ini_file("config.ini", true)
来源：http://wyw.sjlbkw.cn

[U74] PHP：读取环境变量
来源：http://hyr.kuanghao11.cn

getenv("APP_ENV") ?: "production"
来源：http://uzb.yj20258.top

[U75] PHP：依赖注入
来源：http://aik.xylfe.cn

composer require psr/container
来源：http://nqo.xylfe.cn

[U76] PHP：简单路由
来源：http://pty.c1oappe.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://xkq.yvedp.cn

[U77] PHP：模板渲染
来源：http://ciw.mhx1999.top

composer require twig/twig
来源：http://mfd.yj20258888.top

[U78] PHP：单元测试
来源：http://ilc.nwbrower.top

composer require --dev phpunit/phpunit
来源：http://ixj.yj20258.top

[U79] PHP：静态分析
来源：http://lan.xuetiantiany.cn

composer require --dev phpstan/phpstan
来源：http://zvz.zycfv.cn

[U80] PHP：代码规范修复
来源：http://wqn.shanyushiyangtech.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://byw.yj20258.top

[U81] JS：初始化项目
来源：http://tsh.yj20258888.top

npm init -y;  npm i express
来源：http://qkj.tianlin.xyz

[U82] JS：package.json 脚本
来源：http://zgy.zhijiandao.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://wzh.dianchejie.cn

[U83] JS：ES Module 导入导出
来源：http://ekm.xylfe.cn

export const a = 1;  import { a } from "./m.js";
来源：http://zyp.cqqwz.cn

[U84] JS：CommonJS 写法
来源：http://xll.yfazqb.com

module.exports = { a };  const { a } = require("./m");
来源：http://cpg.52xcode.cn

[U85] JS：可选链
来源：http://dgk.cqqwz.cn

a?.b?.c
来源：http://nou.jyoumei.cn

[U86] JS：空值合并
来源：http://kso.cheryme.top

a ?? b
来源：http://wqe.gaohongyu789.top

[U87] JS：解构默认值
来源：http://tmm.yueranfly.top

const { a = 1, b = 2 } = obj;
来源：http://lls.nanxinkj.top

[U88] JS：对象展开合并
来源：http://xwo.jqgfzy.top

{ ...a, ...b }
来源：http://gti.yj20258888.top

[U89] JS：数组去重
来源：http://bcr.jqgfzy.top

[...new Set(arr)]
来源：http://hnz.cashguo.top

[U90] JS：数字数组排序
来源：http://bik.epnwcf.com

[...arr].sort((a, b) => a - b)
来源：http://zmo.ywan-chungtsiang.top

[U91] JS：对象键值遍历
来源：http://iid.shangyingyoupin.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://wqh.yangfankeji.com

[U92] JS：深拷贝
来源：http://yxk.shzxlz.cn

structuredClone(obj)
来源：http://nko.tanke756.top

[U93] JS：模板字符串
来源：http://pto.daxiang520.top

`共 ${n} 条`
来源：http://fyw.sxryk.cn

[U94] JS：箭头函数
来源：http://bav.hcnkem.com

const double = x => x * 2;
来源：http://qpm.hnqzz.top

[U95] JS：Promise 包装
来源：http://tof.daria6918.cn

new Promise((resolve, reject) => {})
来源：http://ngm.jinqigfzy.top

[U96] JS：async/await 与异常
来源：http://haw.jlsjyb.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://tpz.zycfv.cn

[U97] JS：并发请求
来源：http://tmu.fehbvm.com

await Promise.all(urls.map(u => fetch(u)))
来源：http://zyx.yuanzhike.top

[U98] JS：fetch 带 JSON
来源：http://jil.yuxming.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://zgc.yj20258888.top

[U99] JS：事件监听
来源：http://btm.ivvv.top

el.addEventListener("click", e => {})
来源：http://pno.yanxiufei.cn

[U100] JS：DOM 查询
来源：http://phd.iojbl.cn

document.querySelector(".item")
来源：http://yru.birdmap.top

[U101] JS：classList 操作
来源：http://fiv.zhongyouzk.top

el.classList.toggle("active")
来源：http://hej.tian-w.cn

[U102] JS：本地存储
来源：http://qqw.0kj1m.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://pty.yj20258888.top

[U103] JS：定时器
来源：http://ere.snrcjt.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://thp.zhaomingkeji.xyz

[U104] JS：防抖
来源：http://ytm.yvedp.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mrb.yfazqb.com

[U105] JS：节流
来源：http://ncg.hfpthk.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://evc.jinyuanbaomall.cn

[U106] JS：日期格式化
来源：http://jmx.fengsongda.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://vrk.feifeiyinyue.top

[U107] JS：数字千分位
来源：http://qps.xylfe.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://snp.0kj1m.cn

[U108] JS：随机整数
来源：http://mna.fktsv.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hau.gzhubu.top

[U109] JS：数组分组
来源：http://aba.chenzaomai.com

Object.groupBy(arr, x => x.type)
来源：http://fms.xylfe.cn

[U110] JS：数组分块
来源：http://nqf.jlsjyb.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://kbt.hongshengwenyu.top

[U111] JS：对象转 Map
来源：http://lme.jyoumei.cn

new Map(Object.entries(obj))
来源：http://unu.shanyushiyangtech.top

[U112] JS：字符串补位
来源：http://bus.nanxinkj.top

"7".padStart(3, "0")
来源：http://xhl.c1oappe.top

[U113] JS：正则替换全部
来源：http://qnk.hammf.cn

s.replaceAll("a", "b")
来源：http://lay.zycfv.cn

[U114] JS：JSON 深比较
来源：http://iiz.tian-w.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://rxy.jinghuilouyu.cn

[U115] JS：生成 UUID
来源：http://tbl.hnxiangtu.top

crypto.randomUUID()
来源：http://dzt.zdbjq.cn

[U116] JS：类型检查（JSDoc）
来源：http://lhp.ybcxt.top

/** @param {string} name */ function f(name) {}
来源：http://zlg.vqdsnc.cn

[U117] JS：单元测试
来源：http://nae.sjlbkw.cn

npm i -D vitest;  npx vitest
来源：http://sey.sufxvd.cn

[U118] JS：开发服务器
来源：http://avv.fzhhl.top

npm i -D vite;  npx vite
来源：http://jna.mhx1999.top

[U119] JS：生产构建
来源：http://vag.tian-w.cn

npx vite build
来源：http://hth.zhiwuduotai.top

[U120] JS：读取环境变量（Vite）
来源：http://njs.nanxinkj.top

import.meta.env.VITE_API_URL
来源：http://qrj.shangyingyoupin.top

================================================================================
来源：http://hgg.uphjek.com

统计汇总
来源：http://ynp.shzxlz.cn

================================================================================
来源：http://mok.quarkkingdee.top

按语言统计（条）：
来源：http://sic.sjlbkw.cn

Python ......... 252
来源：http://dia.fktsv.cn

PHP ............ 252
来源：http://jru.yonumen.top

JavaScript ..... 252
来源：http://ujk.fehbvm.com

TypeScript ..... 212
来源：http://qcj.shanyushiyangtech.top

Java ........... 212
来源：http://knk.yj20258.top

Go ............. 212
来源：http://ljy.birdmap.top

Ruby ........... 212
来源：http://zhx.xylfe.cn

C# ............. 212
来源：http://ggj.ctjpmb.com

C .............. 30
来源：http://pdz.sjlbkw.cn

C++ ............ 30
来源：http://dte.haohaochexian.top

SQL ............ 90
来源：http://arq.jianghu66.top

Bash ........... 80
来源：http://rmz.birdmap.top

Kotlin ......... 15
来源：http://rco.havefunace.top

Swift .......... 15
来源：http://zau.shuidangran.top

Lua ............ 10
来源：http://eff.ydzc1.top

Perl ........... 10
来源：http://hfz.sufxvd.cn

Scala .......... 10
来源：http://ish.vehdjk.com

------------------------------------
来源：http://ypt.pycfn.com

合计 ........... 2106 条
来源：http://fov.hcnkem.com

按章节统计：
来源：http://mou.shangyingyoupin.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://lgg.zycfv.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://zow.hnxiangtu.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://yyc.9152youxi.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://vpr.dianchejie.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://ohx.chenlongwang.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://vnv.jiagoushi.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://eag.sufxvd.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://cum.52xcode.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://yvm.jinghuilouyu.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://ycs.guowangkeji.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://ogn.chenjidiqi.icu

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://dib.ppjwa.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://rpu.gotoacloud.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://pfk.shangyingyoupin.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://vnq.ctjpmb.com

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://jpt.tanke756.top

Q SQL 专题                              90
来源：http://ucu.hfpthk.cn

R Bash 专题                             80
来源：http://ijy.ydzc1.top

S C / C++ 专题                          60
来源：http://qhj.yueranfly.top

T 其他语言补充                          60
来源：http://hge.feifeiyinyue.top

U 高频实用片段                         120
来源：http://eqm.wangshuangyany.cn

------------------------------------
来源：http://fsc.aizwys.cn

合计                                  2106 条
来源：http://ifz.tian-w.cn

--------------------------------------------------------------------------------
来源：http://puj.jyoumei.cn

使用提醒
来源：http://man.mhx1999.top

--------------------------------------------------------------------------------
来源：http://lwh.gogol.net.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://czs.ydzc1.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://ftl.hesvh.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://gwq.nanxuanxn.top

在旧版本上使用前请先确认语法支持情况。
来源：http://wtc.xziqi.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://kfe.sufxvd.cn

—— 文件结束 ——
来源：http://zgy.shzxlz.cn

================================================================================
来源：http://off.yj202588.top

程序语言常见例子速查手册（2024 版）
来源：http://zwg.zhixingplan.top

Common Programming Examples Cheat Book
来源：http://zsz.nanxinkj.top

================================================================================
来源：http://crc.ctjpmb.com

【收录内容】
来源：http://xvg.birdmap.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://wbr.gotoacloud.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://zom.cashguo.top

SQL · Bash · C · C++
来源：http://vpl.316326.xyz

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://xqx.shangyingyoupin.top

【使用说明】
来源：http://fdi.hfpthk.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://xrn.zycfv.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://dfg.shangyingyoupin.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://xre.daria6918.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://khn.sxryk.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://rkb.kuanghao11.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://bne.xziqi.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://ipi.ybcxt.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://ora.aibaodan.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://rjo.quarkkingdee.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://qxn.yj20258.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://ybz.hnxiangtu.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://jdq.shzxlz.cn

【文件统计】
来源：http://dro.tarul.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://ihz.dianchejie.cn

--------------------------------------------------------------------------------
来源：http://bjj.sysykeji.top

目  录
来源：http://unx.epnwcf.com

--------------------------------------------------------------------------------
来源：http://omh.316326.xyz

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://xtn.pycfn.com

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://lck.svipenyu.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://shh.hongshengwenyu.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://kai.yfazqb.com

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://yjr.shzxlz.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://hra.guowangkeji.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://qwo.xziqi.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://qhu.shuidangran.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://rbu.sweek.top


<!-- 参考信息 -->