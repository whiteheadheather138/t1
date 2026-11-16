代发 wailian999

[U15] Py：高精度计时
来源：http://fvq.fzhhl.top

t = time.perf_counter()
来源：http://gjc.zdbjq.cn

[U16] Py：命令行参数解析
来源：http://dno.9152youxi.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://tow.yfazqb.com

[U17] Py：初始化日志
来源：http://qdg.nanxuanxn.top

logging.basicConfig(level=logging.INFO)
来源：http://bhf.wangdashe.top

[U18] Py：预编译正则
来源：http://tjs.quarkkingdee.top

pat = re.compile(r"\d+")
来源：http://nvy.zdbjq.cn

[U19] Py：正则替换带回调
来源：http://xqo.zhaomingkeji.xyz

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://tdy.cqqwz.cn

[U20] Py：缓存函数结果
来源：http://lyp.guowangkeji.top

@functools.lru_cache(maxsize=None)
来源：http://chg.tianlin.xyz

[U21] Py：自定义上下文管理器
来源：http://kqs.fzhhl.top

@contextlib.contextmanager
来源：http://dkp.zhoulong.xyz

[U22] Py：矩阵转置
来源：http://xdk.yuanzhike.top

list(zip(*m))
来源：http://olu.yuanzhike.top

[U23] Py：分块读取大文件
来源：http://gzi.yangfankeji.com

for chunk in iter(lambda: f.read(8192), b""):
来源：http://ojz.shanyushiyangkeji.top

[U24] Py：路径操作
来源：http://abk.sysykeji.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://sfa.haohaochexian.top

[U25] Py：CSV 按字典读
来源：http://jvf.shanyushiyangtech.top

csv.DictReader(f)
来源：http://rmq.shangyingyoupin.top

[U26] Py：并发下载
来源：http://fsg.jqgufenzy.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://rqe.pengpengdd.cyou

[U27] Py：异步 HTTP
来源：http://vqy.hesvh.cn

aiohttp.ClientSession() 配合 async with
来源：http://xjb.zhijiandao.cn

[U28] Py：类型别名
来源：http://qbs.xinyue.icu

UserId = int
来源：http://squ.yuxming.cn

[U29] Py：属性校验
来源：http://ygq.wangdashe.top

@property 与 @x.setter 配合
来源：http://qhv.ywan-chungtsiang.top

[U30] Py：数据类
来源：http://ezh.xingfuxueyuan.xyz

@dataclass(slots=True)
来源：http://cxg.yangfankeji.com

[U31] Py：单测
来源：http://ass.yj20258.top

python -m pytest -q
来源：http://nqi.jyoumei.cn

[U32] Py：代码格式化
来源：http://esh.sysykeji.top

ruff format . && ruff check --fix .
来源：http://elb.9152youxi.cn

[U33] Py：打包发布
来源：http://ztr.ybcxt.top

python -m build  （依赖 pyproject.toml）
来源：http://cbf.xinyue.icu

[U34] Py：判断编码
来源：http://efv.ybcxt.top

chardet.detect(raw)
来源：http://ypl.yongpay.top

[U35] Py：发送邮件
来源：http://uxb.cqqwz.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hta.fengsongda.top

[U36] Py：定时任务
来源：http://qxx.havefunace.top

schedule.every(10).minutes.do(job)
来源：http://oxz.cashguo.top

[U37] Py：读写 Excel
来源：http://bzq.xuanzx.com

pandas.read_excel / DataFrame.to_excel
来源：http://kdt.zhaomingkeji.xyz

[U38] Py：获取脚本所在目录
来源：http://xai.jiagoushi.top

Path(__file__).resolve().parent
来源：http://rke.bbcook.cn

[U39] Py：判断是否在交互环境
来源：http://mum.yangfankeji.com

sys.stdout.isatty()
来源：http://zbl.nanxuanxn.top

[U40] Py：打印到标准错误
来源：http://yyz.yonumen.top

print("err", file=sys.stderr)
来源：http://qpj.yongpay.top

[U41] PHP：初始化 Composer 项目
来源：http://pyo.yueranfly.top

composer init;  composer require guzzlehttp/guzzle
来源：http://clq.zdbjq.cn

[U42] PHP：PSR-4 自动加载
来源：http://ywt.chenzaomai.com

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://flt.52xcode.cn

[U43] PHP：声明命名空间
来源：http://nxj.pycfn.com

namespace App\Http;
来源：http://zqh.ydzc1.top

[U44] PHP：开启严格类型
来源：http://mbz.fzhhl.top

declare(strict_types=1);
来源：http://ecx.zdqjudy.top

[U45] PHP：类型声明与返回类型
来源：http://ynm.jiagoushi.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://tdb.gaohongyu789.top

[U46] PHP：可空类型
来源：http://tvf.bbcook.cn

?string $name = null
来源：http://wnu.vqdsnc.cn

[U47] PHP：联合类型
来源：http://pze.vehdjk.com

int|string $id
来源：http://onb.52xcode.cn

[U48] PHP：纯枚举
来源：http://xqj.fengsongda.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://psf.yonumen.top

[U49] PHP：只读属性
来源：http://jbj.wangshuangyany.cn

public readonly string $name
来源：http://isg.ivvv.top

[U50] PHP：构造器属性提升
来源：http://ejm.shangyingyoupin.top

public function __construct(private int $id) {}
来源：http://phx.sweek.top

[U51] PHP：数组解构
来源：http://fsr.xuetiantiany.cn

[$a, $b] = $arr;
来源：http://kzc.jlsjyb.cn

[U52] PHP：箭头函数
来源：http://pdh.sysykeji.top

$double = fn($x) => $x * 2;
来源：http://xuh.dashuyun.cn

[U53] PHP：空合并运算符
来源：http://hbs.yongpay.top

$v = $a ?? $b ?? "default";
来源：http://uds.hywenlv.cn

[U54] PHP：空安全调用
来源：http://gfg.yanxiufei.cn

$obj?->method()
来源：http://ckc.fengsongda.top

[U55] PHP：match 表达式
来源：http://jjv.haohaochexian.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://mxh.shangyingyoupin.top

[U56] PHP：命名参数
来源：http://tag.fktsv.cn

f(a: 1, b: 2)
来源：http://thb.shzxlz.cn

[U57] PHP：字符串插值
来源：http://ltz.c1oappe.top

"值: {$a}"
来源：http://son.yj20258.top

[U58] PHP：数组三件套
来源：http://jnm.jinyuanbaomall.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://zka.ydjk.org.cn

[U59] PHP：自定义排序
来源：http://kca.pengpengdd.cyou

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://axi.gaohongyu789.top

[U60] PHP：JSON 编解码
来源：http://otz.birdmap.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://lsp.zhaomingkeji.xyz

[U61] PHP：正则
来源：http://uqj.wangshuangyany.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://xty.zhoulong.xyz

[U62] PHP：日期对象
来源：http://tbu.hammf.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://vtz.hcnkem.com

[U63] PHP：文件读写
来源：http://ypu.jlsjyb.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://vvb.xingfuxueyuan.xyz

[U64] PHP：目录遍历
来源：http://gzh.shanyushiyangtech.top

glob("dir/*.php");  scandir("dir");
来源：http://xbp.snrcjt.cn

[U65] PHP：会话
来源：http://dap.zhengqikj.top

session_start();  $_SESSION["uid"] = 1;
来源：http://jdz.vqdsnc.cn

[U66] PHP：设置 Cookie
来源：http://mzn.yj20258.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://dln.cqqwz.cn

[U67] PHP：处理文件上传
来源：http://dwo.epnwcf.com

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://ort.fanxiaobao.xyz

[U68] PHP：PDO 连接
来源：http://def.sweek.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://vsq.ybcxt.top

[U69] PHP：PDO 预处理
来源：http://bmo.chenzaomai.com

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://cqx.epnwcf.com

[U70] PHP：PDO 事务
来源：http://tjm.ydjk.org.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://bnn.hcnkem.com

[U71] PHP：抛出异常
来源：http://nfi.yongpay.top

throw new RuntimeException("失败", 500);
来源：http://num.havefunace.top

[U72] PHP：写错误日志
来源：http://fcm.jianghu66.top

error_log("失败: " . $e->getMessage());
来源：http://dth.yanxiufei.cn

[U73] PHP：读取 ini 配置
来源：http://vwr.guannengcc.top

parse_ini_file("config.ini", true)
来源：http://bpv.sysykeji.top

[U74] PHP：读取环境变量
来源：http://jiw.uphjek.com

getenv("APP_ENV") ?: "production"
来源：http://qsj.redwolf501.top

[U75] PHP：依赖注入
来源：http://frc.cdnleiting.top

composer require psr/container
来源：http://nci.havefunace.top

[U76] PHP：简单路由
来源：http://aiu.haohaochexian.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://umd.pengpengdd.cyou

[U77] PHP：模板渲染
来源：http://xjs.yanxiufei.cn

composer require twig/twig
来源：http://dxm.fanxiaobao.xyz

[U78] PHP：单元测试
来源：http://gde.epnwcf.com

composer require --dev phpunit/phpunit
来源：http://yzc.jqgufenzy.top

[U79] PHP：静态分析
来源：http://jis.tianlin.xyz

composer require --dev phpstan/phpstan
来源：http://pbp.shzxlz.cn

[U80] PHP：代码规范修复
来源：http://fdu.tian-w.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://ldt.jlsjyb.cn

[U81] JS：初始化项目
来源：http://tgv.fzhhl.top

npm init -y;  npm i express
来源：http://lbu.svipenyu.cn

[U82] JS：package.json 脚本
来源：http://khz.gaohongyu789.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://foy.dianchejie.cn

[U83] JS：ES Module 导入导出
来源：http://niv.zhixingplan.top

export const a = 1;  import { a } from "./m.js";
来源：http://nwh.yvedp.cn

[U84] JS：CommonJS 写法
来源：http://yso.yvedp.cn

module.exports = { a };  const { a } = require("./m");
来源：http://otw.gogol.net.cn

[U85] JS：可选链
来源：http://riw.zdqjudy.top

a?.b?.c
来源：http://gbi.svipenyu.cn

[U86] JS：空值合并
来源：http://ngs.vehdjk.com

a ?? b
来源：http://xjk.jiagoushi.top

[U87] JS：解构默认值
来源：http://mbj.yonumen.top

const { a = 1, b = 2 } = obj;
来源：http://zid.ctjpmb.com

[U88] JS：对象展开合并
来源：http://gwb.snrcjt.cn

{ ...a, ...b }
来源：http://tsu.ivvv.top

[U89] JS：数组去重
来源：http://kll.jyoumei.cn

[...new Set(arr)]
来源：http://gfz.zdqjudy.top

[U90] JS：数字数组排序
来源：http://tcv.vehdjk.com

[...arr].sort((a, b) => a - b)
来源：http://vaa.fktsv.cn

[U91] JS：对象键值遍历
来源：http://rtc.zhongyouzk.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://upv.xylfe.cn

[U92] JS：深拷贝
来源：http://mqb.yj20258888.top

structuredClone(obj)
来源：http://qwp.daxiang520.top

[U93] JS：模板字符串
来源：http://kin.hnxiangtu.top

`共 ${n} 条`
来源：http://ccj.havefunace.top

[U94] JS：箭头函数
来源：http://zfa.316326.xyz

const double = x => x * 2;
来源：http://jpa.pengpengdd.cyou

[U95] JS：Promise 包装
来源：http://jhp.aibaodan.cn

new Promise((resolve, reject) => {})
来源：http://mxn.svipenyu.cn

[U96] JS：async/await 与异常
来源：http://uit.daxiang520.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://rza.jinghuilouyu.cn

[U97] JS：并发请求
来源：http://knt.tianlin.xyz

await Promise.all(urls.map(u => fetch(u)))
来源：http://yfn.cashguo.top

[U98] JS：fetch 带 JSON
来源：http://gvv.ctjpmb.com

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://gil.yvedp.cn

[U99] JS：事件监听
来源：http://xpd.yj20258.top

el.addEventListener("click", e => {})
来源：http://xxe.zhijiandao.cn

[U100] JS：DOM 查询
来源：http://muu.svipenyu.cn

document.querySelector(".item")
来源：http://fjf.jinqigfzy.top

[U101] JS：classList 操作
来源：http://ceh.jianghu66.top

el.classList.toggle("active")
来源：http://ogy.sxryk.cn

[U102] JS：本地存储
来源：http://tqj.chenlongwang.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://vif.sweek.top

[U103] JS：定时器
来源：http://uwp.svipenyu.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://bku.yfazqb.com

[U104] JS：防抖
来源：http://ecc.fzhhl.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://yqu.guowangkeji.top

[U105] JS：节流
来源：http://ivg.ehwqpu.com

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://wpk.tianlin.xyz

[U106] JS：日期格式化
来源：http://oow.hammf.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://yab.uphjek.com

[U107] JS：数字千分位
来源：http://whk.bbcook.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://bdf.cucudq.cn

[U108] JS：随机整数
来源：http://lmm.zhoulong.xyz

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hjj.uphjek.com

[U109] JS：数组分组
来源：http://ody.yfazqb.com

Object.groupBy(arr, x => x.type)
来源：http://ddu.havefunace.top

[U110] JS：数组分块
来源：http://dem.cashguo.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://lcv.hywenlv.cn

[U111] JS：对象转 Map
来源：http://vsn.ybcxt.top

new Map(Object.entries(obj))
来源：http://tex.jinqigfzy.top

[U112] JS：字符串补位
来源：http://tuz.jinyuanbaomall.cn

"7".padStart(3, "0")
来源：http://lar.aizwys.cn

[U113] JS：正则替换全部
来源：http://tff.gogol.net.cn

s.replaceAll("a", "b")
来源：http://odw.aizwys.cn

[U114] JS：JSON 深比较
来源：http://ldf.hnxiangtu.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://has.aizwys.cn

[U115] JS：生成 UUID
来源：http://iah.yuxming.cn

crypto.randomUUID()
来源：http://zcd.ydjk.org.cn

[U116] JS：类型检查（JSDoc）
来源：http://hiu.ydzc1.top

/** @param {string} name */ function f(name) {}
来源：http://lce.zhaomingkeji.xyz

[U117] JS：单元测试
来源：http://vwz.redwolf501.top

npm i -D vitest;  npx vitest
来源：http://qia.hfpthk.cn

[U118] JS：开发服务器
来源：http://pcn.yfazqb.com

npm i -D vite;  npx vite
来源：http://cdm.jinqigufen.top

[U119] JS：生产构建
来源：http://kua.hcnkem.com

npx vite build
来源：http://jtc.hnxiangtu.top

[U120] JS：读取环境变量（Vite）
来源：http://lmt.haohaochexian.top

import.meta.env.VITE_API_URL
来源：http://bka.zdbjq.cn

================================================================================
来源：http://gsh.dashuyun.cn

统计汇总
来源：http://vow.guowangkeji.top

================================================================================
来源：http://wur.chenlongwang.top

按语言统计（条）：
来源：http://pxv.chenlongwang.top

Python ......... 252
来源：http://iai.yongpay.top

PHP ............ 252
来源：http://bef.yongpay.top

JavaScript ..... 252
来源：http://bjh.jianghu66.top

TypeScript ..... 212
来源：http://xkr.wangdashe.top

Java ........... 212
来源：http://buk.nanxuanxn.top

Go ............. 212
来源：http://chq.zycfv.cn

Ruby ........... 212
来源：http://vdy.xingfuxueyuan.xyz

C# ............. 212
来源：http://xiv.zhijiandao.cn

C .............. 30
来源：http://yin.ehwqpu.com

C++ ............ 30
来源：http://qpt.guannengcc.top

SQL ............ 90
来源：http://jio.fanxiaobao.xyz

Bash ........... 80
来源：http://ipp.yj20258888.top

Kotlin ......... 15
来源：http://wmp.zhengqikj.top

Swift .......... 15
来源：http://tvx.yanxiufei.cn

Lua ............ 10
来源：http://cws.ydjk.org.cn

Perl ........... 10
来源：http://pow.hysaishi.cn

Scala .......... 10
来源：http://byb.cqqwz.cn

------------------------------------
来源：http://dnf.hnxiangtu.top

合计 ........... 2106 条
来源：http://yzj.epnwcf.com

按章节统计：
来源：http://glw.guowangkeji.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://mbq.fktsv.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://uuq.bbcook.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://ngk.shangyingyoupin.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://wed.ybcxt.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://wpl.ydjk.org.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://mwj.yuanzhike.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://byn.uphjek.com

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://nyh.hnqzz.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://xgi.daria6918.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://vrg.epnwcf.com

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://gdo.hnqzz.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://sej.yvedp.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://byf.c1oappe.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://xrv.zhengqikj.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://znr.shanyushiyangtech.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://ttb.meibo888.top

Q SQL 专题                              90
来源：http://shm.redwolf501.top

R Bash 专题                             80
来源：http://mgs.shuidangran.top

S C / C++ 专题                          60
来源：http://iql.yj20258888.top

T 其他语言补充                          60
来源：http://adn.yuanzhike.top

U 高频实用片段                         120
来源：http://yqv.cqqwz.cn

------------------------------------
来源：http://ykm.dianchejie.cn

合计                                  2106 条
来源：http://nnv.yfazqb.com

--------------------------------------------------------------------------------
来源：http://cps.gotoacloud.top

使用提醒
来源：http://qlk.0kj1m.cn

--------------------------------------------------------------------------------
来源：http://ofs.cheryme.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://twy.daxiang520.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://gvl.hammf.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://rnt.zhoulong.xyz

在旧版本上使用前请先确认语法支持情况。
来源：http://kqz.nwbrower.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://kbn.yongpay.top

—— 文件结束 ——
来源：http://mfe.jiagoushi.top

================================================================================
来源：http://gxs.mhx1999.top

程序语言常见例子速查手册（2024 版）
来源：http://epx.xuanzx.com

Common Programming Examples Cheat Book
来源：http://loa.ydjk.org.cn

================================================================================
来源：http://oek.yueranfly.top

【收录内容】
来源：http://wov.chenlongwang.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://jlf.mhx1999.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://iig.aizwys.cn

SQL · Bash · C · C++
来源：http://jda.nwbrower.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://alo.gotoacloud.top

【使用说明】
来源：http://hzd.xingfuxueyuan.xyz

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://dpx.xuetiantiany.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://rpn.nanxinkj.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://mmc.fzhhl.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://xxq.vehdjk.com

Bash:  Shell         C:     C             C++:   C++
来源：http://stv.hfpthk.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://xck.ydjk.org.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://lsm.gotoacloud.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://ggu.hongshengwenyu.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://qsr.vqdsnc.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://dhm.jinqigufen.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://wae.pycfn.com

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://sai.ydzc1.top

【文件统计】
来源：http://tmh.pengpengdd.cyou

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://jkw.jinqigufen.top

--------------------------------------------------------------------------------
来源：http://qsr.shanyushiyangtech.top

目  录
来源：http://suo.snrcjt.cn

--------------------------------------------------------------------------------
来源：http://lvi.zhixingplan.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://bgi.wangshuangyany.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://zpp.chenjidiqi.icu

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://mig.fengsongda.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://afy.guannengcc.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://fub.cdnleiting.top


<!-- 参考信息 -->