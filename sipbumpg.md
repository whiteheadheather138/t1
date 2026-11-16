代发 wailian999

[U15] Py：高精度计时
来源：http://vcu.sysykeji.top

t = time.perf_counter()
来源：http://ewx.birdmap.top

[U16] Py：命令行参数解析
来源：http://zws.sufxvd.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://uwq.hnxiangtu.top

[U17] Py：初始化日志
来源：http://jot.ctjpmb.com

logging.basicConfig(level=logging.INFO)
来源：http://cqh.yvedp.cn

[U18] Py：预编译正则
来源：http://ptt.nwbrower.top

pat = re.compile(r"\d+")
来源：http://vlq.shzxlz.cn

[U19] Py：正则替换带回调
来源：http://pel.xuetiantiany.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://dds.xylfe.cn

[U20] Py：缓存函数结果
来源：http://geu.birdmap.top

@functools.lru_cache(maxsize=None)
来源：http://nev.havefunace.top

[U21] Py：自定义上下文管理器
来源：http://phw.bjfxy.top

@contextlib.contextmanager
来源：http://nfb.zycfv.cn

[U22] Py：矩阵转置
来源：http://eho.fzhhl.top

list(zip(*m))
来源：http://hux.uphjek.com

[U23] Py：分块读取大文件
来源：http://qfn.fehbvm.com

for chunk in iter(lambda: f.read(8192), b""):
来源：http://lpb.zdbjq.cn

[U24] Py：路径操作
来源：http://qyf.jqgufenzy.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://aqp.yj20258.top

[U25] Py：CSV 按字典读
来源：http://doi.sysykeji.top

csv.DictReader(f)
来源：http://iff.zhiwuduotai.top

[U26] Py：并发下载
来源：http://kjj.9152youxi.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://dmb.meibo888.top

[U27] Py：异步 HTTP
来源：http://bod.hcnkem.com

aiohttp.ClientSession() 配合 async with
来源：http://izk.xylfe.cn

[U28] Py：类型别名
来源：http://emc.tanke756.top

UserId = int
来源：http://epy.chenlongwang.top

[U29] Py：属性校验
来源：http://daj.gogol.net.cn

@property 与 @x.setter 配合
来源：http://jwf.yonumen.top

[U30] Py：数据类
来源：http://uiz.ydzc1.top

@dataclass(slots=True)
来源：http://gcn.zhoulong.xyz

[U31] Py：单测
来源：http://uhh.316326.xyz

python -m pytest -q
来源：http://icx.zhongyouzk.top

[U32] Py：代码格式化
来源：http://ryn.fehbvm.com

ruff format . && ruff check --fix .
来源：http://ddo.feifeiyinyue.top

[U33] Py：打包发布
来源：http://vrj.zhijiandao.cn

python -m build  （依赖 pyproject.toml）
来源：http://wqn.mhx1999.top

[U34] Py：判断编码
来源：http://bxa.nanxuanxn.top

chardet.detect(raw)
来源：http://uzo.52xcode.cn

[U35] Py：发送邮件
来源：http://lgp.aizwys.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://rxk.zhoulong.xyz

[U36] Py：定时任务
来源：http://nex.shangyingyoupin.top

schedule.every(10).minutes.do(job)
来源：http://njz.bjfxy.top

[U37] Py：读写 Excel
来源：http://ale.ywan-chungtsiang.top

pandas.read_excel / DataFrame.to_excel
来源：http://oji.hysaishi.cn

[U38] Py：获取脚本所在目录
来源：http://kiz.ivvv.top

Path(__file__).resolve().parent
来源：http://wgv.fanxiaobao.xyz

[U39] Py：判断是否在交互环境
来源：http://tbz.nanxinkj.top

sys.stdout.isatty()
来源：http://ppm.aibaodan.cn

[U40] Py：打印到标准错误
来源：http://tlq.ctjpmb.com

print("err", file=sys.stderr)
来源：http://neq.shanyushiyangkeji.top

[U41] PHP：初始化 Composer 项目
来源：http://mlx.hnqzz.top

composer init;  composer require guzzlehttp/guzzle
来源：http://eyr.shuidangran.top

[U42] PHP：PSR-4 自动加载
来源：http://how.zhiwuduotai.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://yfk.chenlongwang.top

[U43] PHP：声明命名空间
来源：http://lmk.fzhhl.top

namespace App\Http;
来源：http://ijw.snrcjt.cn

[U44] PHP：开启严格类型
来源：http://qbx.svipenyu.cn

declare(strict_types=1);
来源：http://gge.ydjk.org.cn

[U45] PHP：类型声明与返回类型
来源：http://zlx.zhongyouzk.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://ifd.shanyushiyangtech.top

[U46] PHP：可空类型
来源：http://gxy.sufxvd.cn

?string $name = null
来源：http://yot.hysaishi.cn

[U47] PHP：联合类型
来源：http://byc.hfpthk.cn

int|string $id
来源：http://mmk.cheryme.top

[U48] PHP：纯枚举
来源：http://hwi.zhengqikj.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://qrh.hywenlv.cn

[U49] PHP：只读属性
来源：http://bhx.hongshengwenyu.top

public readonly string $name
来源：http://qbl.wangshuangyany.cn

[U50] PHP：构造器属性提升
来源：http://usj.chenjidiqi.icu

public function __construct(private int $id) {}
来源：http://ivn.daria6918.cn

[U51] PHP：数组解构
来源：http://yqx.hysaishi.cn

[$a, $b] = $arr;
来源：http://odr.xziqi.cn

[U52] PHP：箭头函数
来源：http://soa.pycfn.com

$double = fn($x) => $x * 2;
来源：http://ouc.daria6918.cn

[U53] PHP：空合并运算符
来源：http://ifl.yj20258888.top

$v = $a ?? $b ?? "default";
来源：http://qws.jianghu66.top

[U54] PHP：空安全调用
来源：http://dgw.zhiwuduotai.top

$obj?->method()
来源：http://jvx.0kj1m.cn

[U55] PHP：match 表达式
来源：http://dqb.snrcjt.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://rmp.c1oappe.top

[U56] PHP：命名参数
来源：http://rmb.jinqigfzy.top

f(a: 1, b: 2)
来源：http://xxs.havefunace.top

[U57] PHP：字符串插值
来源：http://lbe.cqqwz.cn

"值: {$a}"
来源：http://poi.ehwqpu.com

[U58] PHP：数组三件套
来源：http://was.jinqigfzy.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://jay.guowangkeji.top

[U59] PHP：自定义排序
来源：http://ixm.zhoulong.xyz

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://uwf.wangshuangyany.cn

[U60] PHP：JSON 编解码
来源：http://dhg.hnqzz.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://qig.zdbjq.cn

[U61] PHP：正则
来源：http://dgd.jqgufenzy.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://xul.cheryme.top

[U62] PHP：日期对象
来源：http://kvd.birdmap.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://jif.shzxlz.cn

[U63] PHP：文件读写
来源：http://ojb.sufxvd.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://vow.zhengqikj.top

[U64] PHP：目录遍历
来源：http://uwx.sysykeji.top

glob("dir/*.php");  scandir("dir");
来源：http://bkr.ywan-chungtsiang.top

[U65] PHP：会话
来源：http://vvm.fktsv.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://iil.jianghu66.top

[U66] PHP：设置 Cookie
来源：http://lba.yonumen.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://yyt.pengpengdd.cyou

[U67] PHP：处理文件上传
来源：http://qbq.yuanzhike.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://ekj.snrcjt.cn

[U68] PHP：PDO 连接
来源：http://rvd.jlsjyb.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://xqh.tarul.cn

[U69] PHP：PDO 预处理
来源：http://lpj.hongshengwenyu.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://kgt.ivvv.top

[U70] PHP：PDO 事务
来源：http://vxj.yongpay.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://pxj.chenlongwang.top

[U71] PHP：抛出异常
来源：http://yrx.316326.xyz

throw new RuntimeException("失败", 500);
来源：http://ooj.sxryk.cn

[U72] PHP：写错误日志
来源：http://enu.andypj.xyz

error_log("失败: " . $e->getMessage());
来源：http://pwx.sysykeji.top

[U73] PHP：读取 ini 配置
来源：http://cjo.hammf.cn

parse_ini_file("config.ini", true)
来源：http://anp.shanyushiyangkeji.top

[U74] PHP：读取环境变量
来源：http://ddc.ehwqpu.com

getenv("APP_ENV") ?: "production"
来源：http://gso.ybcxt.top

[U75] PHP：依赖注入
来源：http://dsr.yangfankeji.com

composer require psr/container
来源：http://ydk.0kj1m.cn

[U76] PHP：简单路由
来源：http://log.wangdashe.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://ejm.cqqwz.cn

[U77] PHP：模板渲染
来源：http://pty.chenzaomai.com

composer require twig/twig
来源：http://kau.quarkkingdee.top

[U78] PHP：单元测试
来源：http://eqp.xylfe.cn

composer require --dev phpunit/phpunit
来源：http://nie.gotoacloud.top

[U79] PHP：静态分析
来源：http://vdq.hesvh.cn

composer require --dev phpstan/phpstan
来源：http://vih.xinyue.icu

[U80] PHP：代码规范修复
来源：http://whw.hfpthk.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://vaq.hammf.cn

[U81] JS：初始化项目
来源：http://rit.hfpthk.cn

npm init -y;  npm i express
来源：http://pxk.birdmap.top

[U82] JS：package.json 脚本
来源：http://pbr.shuidangran.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://ehj.smart0.xyz

[U83] JS：ES Module 导入导出
来源：http://vbb.chenlongwang.top

export const a = 1;  import { a } from "./m.js";
来源：http://pek.sxryk.cn

[U84] JS：CommonJS 写法
来源：http://dhd.zdbjq.cn

module.exports = { a };  const { a } = require("./m");
来源：http://iij.kuanghao11.cn

[U85] JS：可选链
来源：http://bgj.xinyue.icu

a?.b?.c
来源：http://yco.yangfankeji.com

[U86] JS：空值合并
来源：http://vql.shanyushiyangtech.top

a ?? b
来源：http://xea.52xcode.cn

[U87] JS：解构默认值
来源：http://mgh.hfpthk.cn

const { a = 1, b = 2 } = obj;
来源：http://nkp.sufxvd.cn

[U88] JS：对象展开合并
来源：http://rku.wangdashe.top

{ ...a, ...b }
来源：http://btg.yj20258.top

[U89] JS：数组去重
来源：http://yen.ybcxt.top

[...new Set(arr)]
来源：http://bbb.cdnleiting.top

[U90] JS：数字数组排序
来源：http://gnj.tianlin.xyz

[...arr].sort((a, b) => a - b)
来源：http://zmh.jqgfzy.top

[U91] JS：对象键值遍历
来源：http://xuo.zhengqikj.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://rec.yanxiufei.cn

[U92] JS：深拷贝
来源：http://dla.dashuyun.cn

structuredClone(obj)
来源：http://gde.birdmap.top

[U93] JS：模板字符串
来源：http://eqs.316326.xyz

`共 ${n} 条`
来源：http://fsl.cheryme.top

[U94] JS：箭头函数
来源：http://igh.cqqwz.cn

const double = x => x * 2;
来源：http://cco.daria6918.cn

[U95] JS：Promise 包装
来源：http://gfa.hfpthk.cn

new Promise((resolve, reject) => {})
来源：http://lcb.fengsongda.top

[U96] JS：async/await 与异常
来源：http://psa.yj20258888.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://cdo.jqgfzy.top

[U97] JS：并发请求
来源：http://xwc.hesvh.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://pgh.zhaomingkeji.xyz

[U98] JS：fetch 带 JSON
来源：http://oen.wangshuangyany.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://obn.jinyuanbaomall.cn

[U99] JS：事件监听
来源：http://zoa.jyoumei.cn

el.addEventListener("click", e => {})
来源：http://rbc.meibo888.top

[U100] JS：DOM 查询
来源：http://lee.chenzaomai.com

document.querySelector(".item")
来源：http://ank.andypj.xyz

[U101] JS：classList 操作
来源：http://hez.chenlongwang.top

el.classList.toggle("active")
来源：http://zuo.zhaomingkeji.xyz

[U102] JS：本地存储
来源：http://rjb.epnwcf.com

localStorage.setItem("k", JSON.stringify(v))
来源：http://xam.hnqzz.top

[U103] JS：定时器
来源：http://zqj.yueranfly.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://pdk.hnqzz.top

[U104] JS：防抖
来源：http://atc.jinghuilouyu.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ihk.fanxiaobao.xyz

[U105] JS：节流
来源：http://zyi.dashuyun.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://ule.cqqwz.cn

[U106] JS：日期格式化
来源：http://vck.guannengcc.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://qeh.vqdsnc.cn

[U107] JS：数字千分位
来源：http://zic.yj202588.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://vuf.tanke756.top

[U108] JS：随机整数
来源：http://wuk.yueranfly.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://qlc.xylfe.cn

[U109] JS：数组分组
来源：http://rsl.sweek.top

Object.groupBy(arr, x => x.type)
来源：http://jse.feifeiyinyue.top

[U110] JS：数组分块
来源：http://vel.yj202588.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://kke.andypj.xyz

[U111] JS：对象转 Map
来源：http://wuu.shzxlz.cn

new Map(Object.entries(obj))
来源：http://kem.ivvv.top

[U112] JS：字符串补位
来源：http://hun.shangyingyoupin.top

"7".padStart(3, "0")
来源：http://qkl.feifeiyinyue.top

[U113] JS：正则替换全部
来源：http://xpa.ydjk.org.cn

s.replaceAll("a", "b")
来源：http://huz.sufxvd.cn

[U114] JS：JSON 深比较
来源：http://fhk.wangdashe.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://glb.fzhhl.top

[U115] JS：生成 UUID
来源：http://bax.fanxiaobao.xyz

crypto.randomUUID()
来源：http://hjn.jqgfzy.top

[U116] JS：类型检查（JSDoc）
来源：http://zzf.yj20258888.top

/** @param {string} name */ function f(name) {}
来源：http://blr.gaohongyu789.top

[U117] JS：单元测试
来源：http://imy.hnxiangtu.top

npm i -D vitest;  npx vitest
来源：http://zmu.xuanzx.com

[U118] JS：开发服务器
来源：http://ygu.kuanghao11.cn

npm i -D vite;  npx vite
来源：http://bxk.jlsjyb.cn

[U119] JS：生产构建
来源：http://cbr.jinqigufen.top

npx vite build
来源：http://exd.chenlongwang.top

[U120] JS：读取环境变量（Vite）
来源：http://zkr.fanxiaobao.xyz

import.meta.env.VITE_API_URL
来源：http://oqm.sufxvd.cn

================================================================================
来源：http://wnx.chenjidiqi.icu

统计汇总
来源：http://buv.sweek.top

================================================================================
来源：http://tjs.xuanzx.com

按语言统计（条）：
来源：http://mis.fzhhl.top

Python ......... 252
来源：http://tlf.iojbl.cn

PHP ............ 252
来源：http://vfb.fanxiaobao.xyz

JavaScript ..... 252
来源：http://oto.chenzaomai.com

TypeScript ..... 212
来源：http://ilb.bjfxy.top

Java ........... 212
来源：http://tol.hesvh.cn

Go ............. 212
来源：http://kht.vqdsnc.cn

Ruby ........... 212
来源：http://qdz.chenzaomai.com

C# ............. 212
来源：http://sax.shangyingyoupin.top

C .............. 30
来源：http://qbc.yj20258888.top

C++ ............ 30
来源：http://yjr.hywenlv.cn

SQL ............ 90
来源：http://kgg.guowangkeji.top

Bash ........... 80
来源：http://zad.meibo888.top

Kotlin ......... 15
来源：http://tbr.snrcjt.cn

Swift .......... 15
来源：http://wgw.52xcode.cn

Lua ............ 10
来源：http://cbg.yueranfly.top

Perl ........... 10
来源：http://jue.xziqi.cn

Scala .......... 10
来源：http://cva.gogol.net.cn

------------------------------------
来源：http://aeg.guannengcc.top

合计 ........... 2106 条
来源：http://wiy.xylfe.cn

按章节统计：
来源：http://xoo.xylfe.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://xps.fanxiaobao.xyz

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://lfx.hammf.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://beq.vqdsnc.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://kmo.xuetiantiany.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://dot.andypj.xyz

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://bpb.pycfn.com

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hck.redwolf501.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://swp.daxiang520.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://qhf.aizwys.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://xyy.yuanzhike.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://qxq.zhongyouzk.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://ryd.zhongyouzk.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://oyl.vehdjk.com

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://exo.shangyingyoupin.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://lhu.kuanghao11.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://und.bjfxy.top

Q SQL 专题                              90
来源：http://lim.mhx1999.top

R Bash 专题                             80
来源：http://oge.dashuyun.cn

S C / C++ 专题                          60
来源：http://dkh.yj20258.top

T 其他语言补充                          60
来源：http://grh.ybcxt.top

U 高频实用片段                         120
来源：http://gbk.fengsongda.top

------------------------------------
来源：http://uzl.yuanzhike.top

合计                                  2106 条
来源：http://zto.xuanzx.com

--------------------------------------------------------------------------------
来源：http://dqa.jyoumei.cn

使用提醒
来源：http://jdt.cqqwz.cn

--------------------------------------------------------------------------------
来源：http://edm.bjfxy.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://yiu.yj202588.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://yir.tarul.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://boa.hnxiangtu.top

在旧版本上使用前请先确认语法支持情况。
来源：http://efh.nanxinkj.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://nak.sysykeji.top

—— 文件结束 ——
来源：http://fer.daria6918.cn

================================================================================
来源：http://fgo.shanyushiyangtech.top

程序语言常见例子速查手册（2024 版）
来源：http://icm.52xcode.cn

Common Programming Examples Cheat Book
来源：http://pzo.shuidangran.top

================================================================================
来源：http://ztu.9152youxi.cn

【收录内容】
来源：http://bdo.zhaomingkeji.xyz

覆盖 12 种语言 / 语法与常见 API：
来源：http://ajl.cashguo.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://zaa.wangdashe.top

SQL · Bash · C · C++
来源：http://tow.chenlongwang.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://fxp.jinqigufen.top

【使用说明】
来源：http://rnj.bbcook.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://bgn.fzhhl.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://zmk.daria6918.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://ftb.daria6918.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://vmy.yj20258888.top

Bash:  Shell         C:     C             C++:   C++
来源：http://pbk.fengsongda.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://bea.sxryk.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://ddf.wangdashe.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://iwo.jlsjyb.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://kcr.xziqi.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://jjr.sxryk.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://onc.xuetiantiany.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://fbb.fzhhl.top

【文件统计】
来源：http://rqd.hywenlv.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://pwe.hysaishi.cn

--------------------------------------------------------------------------------
来源：http://bmy.daria6918.cn

目  录
来源：http://ecx.xinyue.icu

--------------------------------------------------------------------------------
来源：http://zxi.0kj1m.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://twl.sjlbkw.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://rcf.tianlin.xyz

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://gen.jianghu66.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://eig.yj20258.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://cyl.birdmap.top


<!-- 参考信息 -->