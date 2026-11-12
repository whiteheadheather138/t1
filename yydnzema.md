代发 wailian999

[U17] Py：初始化日志
来源：http://ncl.smart0.xyz

logging.basicConfig(level=logging.INFO)
来源：http://ktf.snrcjt.cn

[U18] Py：预编译正则
来源：http://rbw.svipenyu.cn

pat = re.compile(r"\d+")
来源：http://aef.yj20258888.top

[U19] Py：正则替换带回调
来源：http://qod.yj20258.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://cim.feifeiyinyue.top

[U20] Py：缓存函数结果
来源：http://ftn.hammf.cn

@functools.lru_cache(maxsize=None)
来源：http://vlk.vehdjk.com

[U21] Py：自定义上下文管理器
来源：http://abp.jinqigufen.top

@contextlib.contextmanager
来源：http://znq.zhengqikj.top

[U22] Py：矩阵转置
来源：http://ymr.jqgfzy.top

list(zip(*m))
来源：http://wvh.zhongyouzk.top

[U23] Py：分块读取大文件
来源：http://mms.feifeiyinyue.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://aiy.shanyushiyangkeji.top

[U24] Py：路径操作
来源：http://ows.yvedp.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://nfp.nanxuanxn.top

[U25] Py：CSV 按字典读
来源：http://nrx.hammf.cn

csv.DictReader(f)
来源：http://ajp.hongshengwenyu.top

[U26] Py：并发下载
来源：http://knp.ybcxt.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://siq.jinqigufen.top

[U27] Py：异步 HTTP
来源：http://wxc.xuanzx.com

aiohttp.ClientSession() 配合 async with
来源：http://wkh.cucudq.cn

[U28] Py：类型别名
来源：http://gwc.shanyushiyangkeji.top

UserId = int
来源：http://lbb.nwbrower.top

[U29] Py：属性校验
来源：http://sxw.zhengqikj.top

@property 与 @x.setter 配合
来源：http://tks.jinyuanbaomall.cn

[U30] Py：数据类
来源：http://rsf.yj20258888.top

@dataclass(slots=True)
来源：http://ibj.ydjk.org.cn

[U31] Py：单测
来源：http://svz.fzhhl.top

python -m pytest -q
来源：http://txc.cqqwz.cn

[U32] Py：代码格式化
来源：http://fnt.yongpay.top

ruff format . && ruff check --fix .
来源：http://rfu.vqdsnc.cn

[U33] Py：打包发布
来源：http://owa.wangshuangyany.cn

python -m build  （依赖 pyproject.toml）
来源：http://wsh.hnxiangtu.top

[U34] Py：判断编码
来源：http://kqf.feifeiyinyue.top

chardet.detect(raw)
来源：http://ish.birdmap.top

[U35] Py：发送邮件
来源：http://xgd.yuanzhike.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://mzq.aizwys.cn

[U36] Py：定时任务
来源：http://tfb.gzhubu.top

schedule.every(10).minutes.do(job)
来源：http://nki.epnwcf.com

[U37] Py：读写 Excel
来源：http://scc.ctjpmb.com

pandas.read_excel / DataFrame.to_excel
来源：http://bsl.yj20258888.top

[U38] Py：获取脚本所在目录
来源：http://qps.tanke756.top

Path(__file__).resolve().parent
来源：http://vtt.xingfuxueyuan.xyz

[U39] Py：判断是否在交互环境
来源：http://tew.chenzaomai.com

sys.stdout.isatty()
来源：http://vmm.xuanzx.com

[U40] Py：打印到标准错误
来源：http://epq.ydjk.org.cn

print("err", file=sys.stderr)
来源：http://oxk.zdbjq.cn

[U41] PHP：初始化 Composer 项目
来源：http://wvw.haohaochexian.top

composer init;  composer require guzzlehttp/guzzle
来源：http://egd.nanxinkj.top

[U42] PHP：PSR-4 自动加载
来源：http://ndu.meibo888.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://ral.feifeiyinyue.top

[U43] PHP：声明命名空间
来源：http://azn.zhoulong.xyz

namespace App\Http;
来源：http://arq.guowangkeji.top

[U44] PHP：开启严格类型
来源：http://xbj.jyoumei.cn

declare(strict_types=1);
来源：http://jif.nanxuanxn.top

[U45] PHP：类型声明与返回类型
来源：http://pii.iojbl.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://cvu.uphjek.com

[U46] PHP：可空类型
来源：http://xbq.jyoumei.cn

?string $name = null
来源：http://ayd.kuanghao11.cn

[U47] PHP：联合类型
来源：http://zya.c1oappe.top

int|string $id
来源：http://sum.tianlin.xyz

[U48] PHP：纯枚举
来源：http://wlo.hammf.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://vsv.hnxiangtu.top

[U49] PHP：只读属性
来源：http://gml.hongshengwenyu.top

public readonly string $name
来源：http://jxi.yj202588.top

[U50] PHP：构造器属性提升
来源：http://irr.tarul.cn

public function __construct(private int $id) {}
来源：http://agk.yonumen.top

[U51] PHP：数组解构
来源：http://osx.vehdjk.com

[$a, $b] = $arr;
来源：http://zoi.bbcook.cn

[U52] PHP：箭头函数
来源：http://obu.cheryme.top

$double = fn($x) => $x * 2;
来源：http://nnc.jinqigfzy.top

[U53] PHP：空合并运算符
来源：http://kzh.yonumen.top

$v = $a ?? $b ?? "default";
来源：http://ykv.gaohongyu789.top

[U54] PHP：空安全调用
来源：http://igz.daria6918.cn

$obj?->method()
来源：http://tya.cucudq.cn

[U55] PHP：match 表达式
来源：http://zrs.nanxuanxn.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://bgs.xingfuxueyuan.xyz

[U56] PHP：命名参数
来源：http://yff.fzhhl.top

f(a: 1, b: 2)
来源：http://aij.sjlbkw.cn

[U57] PHP：字符串插值
来源：http://cvr.nanxinkj.top

"值: {$a}"
来源：http://dog.hnxiangtu.top

[U58] PHP：数组三件套
来源：http://uku.yj20258.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://idw.fehbvm.com

[U59] PHP：自定义排序
来源：http://uys.xuetiantiany.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://sew.shanyushiyangkeji.top

[U60] PHP：JSON 编解码
来源：http://bzy.0kj1m.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://mfn.zhongyouzk.top

[U61] PHP：正则
来源：http://bac.yfazqb.com

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://zuq.snrcjt.cn

[U62] PHP：日期对象
来源：http://brv.guowangkeji.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://aoa.chenzaomai.com

[U63] PHP：文件读写
来源：http://obj.zhongyouzk.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://zvr.yangfankeji.com

[U64] PHP：目录遍历
来源：http://whf.jinqigfzy.top

glob("dir/*.php");  scandir("dir");
来源：http://zjz.dianchejie.cn

[U65] PHP：会话
来源：http://ddo.wangshuangyany.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://vny.jinqigufen.top

[U66] PHP：设置 Cookie
来源：http://qsd.jinqigfzy.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://tsk.zdqjudy.top

[U67] PHP：处理文件上传
来源：http://ceu.snrcjt.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://fkj.ydzc1.top

[U68] PHP：PDO 连接
来源：http://gts.hcnkem.com

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://iwv.cqqwz.cn

[U69] PHP：PDO 预处理
来源：http://vjf.yangfankeji.com

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://uui.jinqigufen.top

[U70] PHP：PDO 事务
来源：http://yii.tian-w.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://dbm.haohaochexian.top

[U71] PHP：抛出异常
来源：http://fjn.gotoacloud.top

throw new RuntimeException("失败", 500);
来源：http://xvh.gaohongyu789.top

[U72] PHP：写错误日志
来源：http://nfz.uphjek.com

error_log("失败: " . $e->getMessage());
来源：http://njw.ivvv.top

[U73] PHP：读取 ini 配置
来源：http://hwx.hywenlv.cn

parse_ini_file("config.ini", true)
来源：http://alb.daxiang520.top

[U74] PHP：读取环境变量
来源：http://obf.uphjek.com

getenv("APP_ENV") ?: "production"
来源：http://ofs.zdbjq.cn

[U75] PHP：依赖注入
来源：http://zjn.xylfe.cn

composer require psr/container
来源：http://oiw.cdnleiting.top

[U76] PHP：简单路由
来源：http://tte.fzhhl.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://wcz.pengpengdd.cyou

[U77] PHP：模板渲染
来源：http://kwu.xinyue.icu

composer require twig/twig
来源：http://rnf.hysaishi.cn

[U78] PHP：单元测试
来源：http://lzn.dianchejie.cn

composer require --dev phpunit/phpunit
来源：http://kaw.xylfe.cn

[U79] PHP：静态分析
来源：http://hgv.jyoumei.cn

composer require --dev phpstan/phpstan
来源：http://fga.gaohongyu789.top

[U80] PHP：代码规范修复
来源：http://sck.sufxvd.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://gce.nanxuanxn.top

[U81] JS：初始化项目
来源：http://wkc.yj202588.top

npm init -y;  npm i express
来源：http://vrn.xingfuxueyuan.xyz

[U82] JS：package.json 脚本
来源：http://ijg.9152youxi.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://xok.meibo888.top

[U83] JS：ES Module 导入导出
来源：http://cma.daria6918.cn

export const a = 1;  import { a } from "./m.js";
来源：http://qph.yj20258888.top

[U84] JS：CommonJS 写法
来源：http://rlj.jinqigfzy.top

module.exports = { a };  const { a } = require("./m");
来源：http://hpu.c1oappe.top

[U85] JS：可选链
来源：http://hwt.jinqigufen.top

a?.b?.c
来源：http://ywl.hysaishi.cn

[U86] JS：空值合并
来源：http://qlf.hammf.cn

a ?? b
来源：http://tzo.xylfe.cn

[U87] JS：解构默认值
来源：http://fac.zhiwuduotai.top

const { a = 1, b = 2 } = obj;
来源：http://bmf.shangyingyoupin.top

[U88] JS：对象展开合并
来源：http://ift.guowangkeji.top

{ ...a, ...b }
来源：http://yaz.shanyushiyangkeji.top

[U89] JS：数组去重
来源：http://phh.xziqi.cn

[...new Set(arr)]
来源：http://zyw.yj20258888.top

[U90] JS：数字数组排序
来源：http://wzu.yfazqb.com

[...arr].sort((a, b) => a - b)
来源：http://gqq.yvedp.cn

[U91] JS：对象键值遍历
来源：http://muq.zhongyouzk.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://tzv.zhixingplan.top

[U92] JS：深拷贝
来源：http://osa.daxiang520.top

structuredClone(obj)
来源：http://bkl.daria6918.cn

[U93] JS：模板字符串
来源：http://cgh.sufxvd.cn

`共 ${n} 条`
来源：http://ept.jyoumei.cn

[U94] JS：箭头函数
来源：http://ujh.vqdsnc.cn

const double = x => x * 2;
来源：http://utn.feifeiyinyue.top

[U95] JS：Promise 包装
来源：http://rtj.svipenyu.cn

new Promise((resolve, reject) => {})
来源：http://uqn.xinyue.icu

[U96] JS：async/await 与异常
来源：http://rac.fengsongda.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://odh.epnwcf.com

[U97] JS：并发请求
来源：http://eex.0kj1m.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://vnd.hesvh.cn

[U98] JS：fetch 带 JSON
来源：http://hhv.yongpay.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://cby.zdqjudy.top

[U99] JS：事件监听
来源：http://gtc.hammf.cn

el.addEventListener("click", e => {})
来源：http://qfg.zdbjq.cn

[U100] JS：DOM 查询
来源：http://lzp.jyoumei.cn

document.querySelector(".item")
来源：http://inw.nwbrower.top

[U101] JS：classList 操作
来源：http://awe.fktsv.cn

el.classList.toggle("active")
来源：http://ojp.yvedp.cn

[U102] JS：本地存储
来源：http://gfg.epnwcf.com

localStorage.setItem("k", JSON.stringify(v))
来源：http://rze.tanke756.top

[U103] JS：定时器
来源：http://roa.fengsongda.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://jqq.hammf.cn

[U104] JS：防抖
来源：http://jqq.ydjk.org.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://jqk.bjfxy.top

[U105] JS：节流
来源：http://hpa.zhengqikj.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://zzt.gzhubu.top

[U106] JS：日期格式化
来源：http://nfg.guowangkeji.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://byc.daxiang520.top

[U107] JS：数字千分位
来源：http://hzr.tarul.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://pfu.guannengcc.top

[U108] JS：随机整数
来源：http://xib.shangyingyoupin.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://xjc.yuxming.cn

[U109] JS：数组分组
来源：http://jiq.yj20258888.top

Object.groupBy(arr, x => x.type)
来源：http://mzw.daxiang520.top

[U110] JS：数组分块
来源：http://nsu.yonumen.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://pke.ydzc1.top

[U111] JS：对象转 Map
来源：http://bjp.yuxming.cn

new Map(Object.entries(obj))
来源：http://qss.fanxiaobao.xyz

[U112] JS：字符串补位
来源：http://gnl.gotoacloud.top

"7".padStart(3, "0")
来源：http://ksn.andypj.xyz

[U113] JS：正则替换全部
来源：http://cbv.jqgfzy.top

s.replaceAll("a", "b")
来源：http://hfo.yj20258888.top

[U114] JS：JSON 深比较
来源：http://zmp.birdmap.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://whl.fktsv.cn

[U115] JS：生成 UUID
来源：http://ecj.yuanzhike.top

crypto.randomUUID()
来源：http://grt.jqgufenzy.top

[U116] JS：类型检查（JSDoc）
来源：http://zec.ydjk.org.cn

/** @param {string} name */ function f(name) {}
来源：http://ucy.fktsv.cn

[U117] JS：单元测试
来源：http://fwb.havefunace.top

npm i -D vitest;  npx vitest
来源：http://ljb.wangdashe.top

[U118] JS：开发服务器
来源：http://jna.pengpengdd.cyou

npm i -D vite;  npx vite
来源：http://swj.ydzc1.top

[U119] JS：生产构建
来源：http://xzi.52xcode.cn

npx vite build
来源：http://sak.haohaochexian.top

[U120] JS：读取环境变量（Vite）
来源：http://feu.yuanzhike.top

import.meta.env.VITE_API_URL
来源：http://iru.ivvv.top

================================================================================
来源：http://fse.zhengqikj.top

统计汇总
来源：http://qjr.yvedp.cn

================================================================================
来源：http://gjg.uphjek.com

按语言统计（条）：
来源：http://kwf.ivvv.top

Python ......... 252
来源：http://dno.vehdjk.com

PHP ............ 252
来源：http://ykg.yanxiufei.cn

JavaScript ..... 252
来源：http://dtg.sysykeji.top

TypeScript ..... 212
来源：http://wms.tian-w.cn

Java ........... 212
来源：http://qys.cucudq.cn

Go ............. 212
来源：http://eue.zhaomingkeji.xyz

Ruby ........... 212
来源：http://oht.birdmap.top

C# ............. 212
来源：http://nzv.fktsv.cn

C .............. 30
来源：http://paz.fktsv.cn

C++ ............ 30
来源：http://umh.xziqi.cn

SQL ............ 90
来源：http://qjl.iojbl.cn

Bash ........... 80
来源：http://epu.zhiwuduotai.top

Kotlin ......... 15
来源：http://mvg.epnwcf.com

Swift .......... 15
来源：http://kgi.chenzaomai.com

Lua ............ 10
来源：http://csv.yongpay.top

Perl ........... 10
来源：http://sex.tarul.cn

Scala .......... 10
来源：http://iew.yfazqb.com

------------------------------------
来源：http://gyn.gzhubu.top

合计 ........... 2106 条
来源：http://hkv.yvedp.cn

按章节统计：
来源：http://cyy.gaohongyu789.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://eyi.smart0.xyz

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://oru.aizwys.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://ysp.pycfn.com

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://pse.c1oappe.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://jqg.sufxvd.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://rjd.zycfv.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://iwv.jqgfzy.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://ppk.zhongyouzk.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://hoo.jinqigufen.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://dmx.0kj1m.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://wiu.smart0.xyz

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://vyd.zhengqikj.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://vkv.zhixingplan.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://zqp.hcnkem.com

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://udh.dianchejie.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://api.tarul.cn

Q SQL 专题                              90
来源：http://ufc.ydjk.org.cn

R Bash 专题                             80
来源：http://twp.fehbvm.com

S C / C++ 专题                          60
来源：http://oui.nanxuanxn.top

T 其他语言补充                          60
来源：http://ywv.ywan-chungtsiang.top

U 高频实用片段                         120
来源：http://zzc.dashuyun.cn

------------------------------------
来源：http://jso.jinyuanbaomall.cn

合计                                  2106 条
来源：http://rut.tarul.cn

--------------------------------------------------------------------------------
来源：http://dfb.cashguo.top

使用提醒
来源：http://aue.vqdsnc.cn

--------------------------------------------------------------------------------
来源：http://vym.jianghu66.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://slq.zycfv.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://eax.snrcjt.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://wkm.zycfv.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://lal.sysykeji.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://aal.yj202588.top

—— 文件结束 ——
来源：http://tac.xziqi.cn

================================================================================
来源：http://bvv.jinqigfzy.top

程序语言常见例子速查手册（2024 版）
来源：http://rvl.andypj.xyz

Common Programming Examples Cheat Book
来源：http://xub.sufxvd.cn

================================================================================
来源：http://knz.zhaomingkeji.xyz

【收录内容】
来源：http://nnv.tanke756.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://umc.ydjk.org.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://cpa.redwolf501.top

SQL · Bash · C · C++
来源：http://mkk.fengsongda.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://jgz.sweek.top

【使用说明】
来源：http://ocw.cheryme.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://idj.tarul.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://wvv.sysykeji.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://fly.ehwqpu.com

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://wja.guannengcc.top

Bash:  Shell         C:     C             C++:   C++
来源：http://tad.ehwqpu.com

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://ptt.yfazqb.com

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://scc.yuanzhike.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://tqz.jiagoushi.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://wio.cdnleiting.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://ira.tanke756.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://zsv.epnwcf.com

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://ofc.nanxuanxn.top

【文件统计】
来源：http://gqy.jqgfzy.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://gxh.ybcxt.top

--------------------------------------------------------------------------------
来源：http://usy.c1oappe.top

目  录
来源：http://kjc.sweek.top

--------------------------------------------------------------------------------
来源：http://lqc.zhixingplan.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://zyf.jqgfzy.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://isk.ydzc1.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://csi.hcnkem.com

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://omv.hywenlv.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://lsl.jianghu66.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://vaq.andypj.xyz

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://yio.xziqi.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://zro.aibaodan.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://utc.chenjidiqi.icu


<!-- 参考信息 -->