代发 wailian999

[U01] Py：创建虚拟环境
来源：http://lhl.sxryk.cn

python -m venv .venv && source .venv/bin/activate
来源：http://nco.hnxiangtu.top

[U02] Py：导出 / 安装依赖
来源：http://xes.daxiang520.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://rcc.epnwcf.com

[U03] Py：加载 .env 配置
来源：http://rui.xuetiantiany.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://qpf.jqgufenzy.top

[U04] Py：变量调试打印
来源：http://dxn.chenlongwang.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://ufz.daria6918.cn

[U05] Py：列表去重且保序
来源：http://umd.zhongyouzk.top

list(dict.fromkeys(arr))
来源：http://tua.iojbl.cn

[U06] Py：合并两个字典
来源：http://zrk.daria6918.cn

{**a, **b}
来源：http://rkv.jiagoushi.top

[U07] Py：反转字典键值
来源：http://wev.cashguo.top

{v: k for k, v in d.items()}
来源：http://jtz.ybcxt.top

[U08] Py：展平二维列表
来源：http://bri.hfpthk.cn

[y for x in nested for y in x]
来源：http://wpq.guannengcc.top

[U09] Py：字典取最大值的键
来源：http://fml.yvedp.cn

max(d, key=d.get)
来源：http://ycv.fanxiaobao.xyz

[U10] Py：按值排序字典
来源：http://ntm.jianghu66.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://tfp.fehbvm.com

[U11] Py：生成器表达式
来源：http://jdc.jianghu66.top

(x * 2 for x in arr)
来源：http://jos.zhijiandao.cn

[U12] Py：取出现最多的 3 个元素
来源：http://ikb.0kj1m.cn

Counter(arr).most_common(3)
来源：http://kvq.sweek.top

[U13] Py：固定长度队列
来源：http://ifg.jinyuanbaomall.cn

deque(maxlen=10)
来源：http://ruu.yanxiufei.cn

[U14] Py：分组收集到列表
来源：http://ffp.sysykeji.top

defaultdict(list)
来源：http://bzx.xinyue.icu

[U15] Py：高精度计时
来源：http://jrv.tian-w.cn

t = time.perf_counter()
来源：http://stw.shuidangran.top

[U16] Py：命令行参数解析
来源：http://dlc.52xcode.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://dmy.dashuyun.cn

[U17] Py：初始化日志
来源：http://nce.c1oappe.top

logging.basicConfig(level=logging.INFO)
来源：http://rzp.iojbl.cn

[U18] Py：预编译正则
来源：http://ajt.yanxiufei.cn

pat = re.compile(r"\d+")
来源：http://npa.quarkkingdee.top

[U19] Py：正则替换带回调
来源：http://bxh.cqqwz.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://uzv.havefunace.top

[U20] Py：缓存函数结果
来源：http://wmb.fanxiaobao.xyz

@functools.lru_cache(maxsize=None)
来源：http://lty.feifeiyinyue.top

[U21] Py：自定义上下文管理器
来源：http://qlv.snrcjt.cn

@contextlib.contextmanager
来源：http://yfy.chenlongwang.top

[U22] Py：矩阵转置
来源：http://rsw.ehwqpu.com

list(zip(*m))
来源：http://wtj.daxiang520.top

[U23] Py：分块读取大文件
来源：http://ztq.aizwys.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://din.fzhhl.top

[U24] Py：路径操作
来源：http://gua.cashguo.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://rwj.daxiang520.top

[U25] Py：CSV 按字典读
来源：http://das.hysaishi.cn

csv.DictReader(f)
来源：http://ojz.fengsongda.top

[U26] Py：并发下载
来源：http://lfg.sxryk.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://vrd.wangdashe.top

[U27] Py：异步 HTTP
来源：http://oqn.yuanzhike.top

aiohttp.ClientSession() 配合 async with
来源：http://lbf.cqqwz.cn

[U28] Py：类型别名
来源：http://gpx.iojbl.cn

UserId = int
来源：http://tpi.zhaomingkeji.xyz

[U29] Py：属性校验
来源：http://ovn.vqdsnc.cn

@property 与 @x.setter 配合
来源：http://mut.epnwcf.com

[U30] Py：数据类
来源：http://dua.birdmap.top

@dataclass(slots=True)
来源：http://dad.ybcxt.top

[U31] Py：单测
来源：http://tmo.ctjpmb.com

python -m pytest -q
来源：http://lqr.chenjidiqi.icu

[U32] Py：代码格式化
来源：http://vmw.yj20258.top

ruff format . && ruff check --fix .
来源：http://rbr.nwbrower.top

[U33] Py：打包发布
来源：http://kwd.yfazqb.com

python -m build  （依赖 pyproject.toml）
来源：http://pzd.yuanzhike.top

[U34] Py：判断编码
来源：http://hst.hywenlv.cn

chardet.detect(raw)
来源：http://bjm.yanxiufei.cn

[U35] Py：发送邮件
来源：http://gjp.yangfankeji.com

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://jtp.yanxiufei.cn

[U36] Py：定时任务
来源：http://yuh.nwbrower.top

schedule.every(10).minutes.do(job)
来源：http://eof.yj20258.top

[U37] Py：读写 Excel
来源：http://igf.uphjek.com

pandas.read_excel / DataFrame.to_excel
来源：http://rfb.xuanzx.com

[U38] Py：获取脚本所在目录
来源：http://yvv.xuanzx.com

Path(__file__).resolve().parent
来源：http://qhd.snrcjt.cn

[U39] Py：判断是否在交互环境
来源：http://zog.9152youxi.cn

sys.stdout.isatty()
来源：http://xjb.hnqzz.top

[U40] Py：打印到标准错误
来源：http://nzf.daria6918.cn

print("err", file=sys.stderr)
来源：http://fyl.9152youxi.cn

[U41] PHP：初始化 Composer 项目
来源：http://pvv.pengpengdd.cyou

composer init;  composer require guzzlehttp/guzzle
来源：http://vuz.svipenyu.cn

[U42] PHP：PSR-4 自动加载
来源：http://vyh.ppjwa.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://bmp.daxiang520.top

[U43] PHP：声明命名空间
来源：http://upu.yj202588.top

namespace App\Http;
来源：http://gup.zhijiandao.cn

[U44] PHP：开启严格类型
来源：http://jkb.tanke756.top

declare(strict_types=1);
来源：http://ssd.snrcjt.cn

[U45] PHP：类型声明与返回类型
来源：http://bte.cqqwz.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://xlj.haohaochexian.top

[U46] PHP：可空类型
来源：http://fhn.yj20258888.top

?string $name = null
来源：http://czz.snrcjt.cn

[U47] PHP：联合类型
来源：http://hhn.fengsongda.top

int|string $id
来源：http://qwm.316326.xyz

[U48] PHP：纯枚举
来源：http://tqs.hnxiangtu.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://suc.zhongyouzk.top

[U49] PHP：只读属性
来源：http://vkf.shzxlz.cn

public readonly string $name
来源：http://kpd.52xcode.cn

[U50] PHP：构造器属性提升
来源：http://upg.aizwys.cn

public function __construct(private int $id) {}
来源：http://qok.chenlongwang.top

[U51] PHP：数组解构
来源：http://rnk.316326.xyz

[$a, $b] = $arr;
来源：http://fgx.sxryk.cn

[U52] PHP：箭头函数
来源：http://pie.yueranfly.top

$double = fn($x) => $x * 2;
来源：http://akk.shangyingyoupin.top

[U53] PHP：空合并运算符
来源：http://gfh.vehdjk.com

$v = $a ?? $b ?? "default";
来源：http://qvz.bbcook.cn

[U54] PHP：空安全调用
来源：http://usn.cdnleiting.top

$obj?->method()
来源：http://jgv.mhx1999.top

[U55] PHP：match 表达式
来源：http://pwt.epnwcf.com

$s = match($x) { 1 => "一", default => "其他" };
来源：http://vwe.ppjwa.cn

[U56] PHP：命名参数
来源：http://xkx.birdmap.top

f(a: 1, b: 2)
来源：http://wie.tianlin.xyz

[U57] PHP：字符串插值
来源：http://ymn.shanyushiyangtech.top

"值: {$a}"
来源：http://tml.nwbrower.top

[U58] PHP：数组三件套
来源：http://nfb.pycfn.com

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://avn.hesvh.cn

[U59] PHP：自定义排序
来源：http://qnb.hnqzz.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ska.tianlin.xyz

[U60] PHP：JSON 编解码
来源：http://fsu.iojbl.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://cmg.ivvv.top

[U61] PHP：正则
来源：http://owp.fengsongda.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://kwq.pengpengdd.cyou

[U62] PHP：日期对象
来源：http://mzt.zhaomingkeji.xyz

(new DateTimeImmutable())->format("Y-m-d");
来源：http://yji.cucudq.cn

[U63] PHP：文件读写
来源：http://imn.nwbrower.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://brg.52xcode.cn

[U64] PHP：目录遍历
来源：http://vxm.sweek.top

glob("dir/*.php");  scandir("dir");
来源：http://tff.aizwys.cn

[U65] PHP：会话
来源：http://ucy.sufxvd.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://yyh.chenlongwang.top

[U66] PHP：设置 Cookie
来源：http://xea.vqdsnc.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://rip.hongshengwenyu.top

[U67] PHP：处理文件上传
来源：http://ewu.bjfxy.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://pzp.tianlin.xyz

[U68] PHP：PDO 连接
来源：http://lok.kuanghao11.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://rjl.zdqjudy.top

[U69] PHP：PDO 预处理
来源：http://gso.mhx1999.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://dbp.ivvv.top

[U70] PHP：PDO 事务
来源：http://qco.jinqigufen.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://mpf.xylfe.cn

[U71] PHP：抛出异常
来源：http://ggh.hfpthk.cn

throw new RuntimeException("失败", 500);
来源：http://fwz.ydjk.org.cn

[U72] PHP：写错误日志
来源：http://aop.zdbjq.cn

error_log("失败: " . $e->getMessage());
来源：http://ysk.jyoumei.cn

[U73] PHP：读取 ini 配置
来源：http://igr.shzxlz.cn

parse_ini_file("config.ini", true)
来源：http://vbu.ctjpmb.com

[U74] PHP：读取环境变量
来源：http://tjy.cqqwz.cn

getenv("APP_ENV") ?: "production"
来源：http://jvq.cashguo.top

[U75] PHP：依赖注入
来源：http://aki.jianghu66.top

composer require psr/container
来源：http://arr.andypj.xyz

[U76] PHP：简单路由
来源：http://vcn.jyoumei.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://hee.haohaochexian.top

[U77] PHP：模板渲染
来源：http://zvt.gotoacloud.top

composer require twig/twig
来源：http://ksw.hesvh.cn

[U78] PHP：单元测试
来源：http://uhj.hysaishi.cn

composer require --dev phpunit/phpunit
来源：http://fnx.quarkkingdee.top

[U79] PHP：静态分析
来源：http://bqk.hysaishi.cn

composer require --dev phpstan/phpstan
来源：http://nvg.sweek.top

[U80] PHP：代码规范修复
来源：http://vva.andypj.xyz

composer require --dev friendsofphp/php-cs-fixer
来源：http://wwu.ehwqpu.com

[U81] JS：初始化项目
来源：http://yqh.yj20258.top

npm init -y;  npm i express
来源：http://ppz.wangshuangyany.cn

[U82] JS：package.json 脚本
来源：http://aji.shuidangran.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://sfc.xuanzx.com

[U83] JS：ES Module 导入导出
来源：http://nlt.ivvv.top

export const a = 1;  import { a } from "./m.js";
来源：http://byo.zhaomingkeji.xyz

[U84] JS：CommonJS 写法
来源：http://pdd.vqdsnc.cn

module.exports = { a };  const { a } = require("./m");
来源：http://fuj.cheryme.top

[U85] JS：可选链
来源：http://ffl.52xcode.cn

a?.b?.c
来源：http://udo.hnqzz.top

[U86] JS：空值合并
来源：http://ylc.uphjek.com

a ?? b
来源：http://bhf.hnxiangtu.top

[U87] JS：解构默认值
来源：http://ukv.zhijiandao.cn

const { a = 1, b = 2 } = obj;
来源：http://jrx.yangfankeji.com

[U88] JS：对象展开合并
来源：http://fnu.fktsv.cn

{ ...a, ...b }
来源：http://xfl.jinqigufen.top

[U89] JS：数组去重
来源：http://puv.ybcxt.top

[...new Set(arr)]
来源：http://dtz.andypj.xyz

[U90] JS：数字数组排序
来源：http://jkj.chenzaomai.com

[...arr].sort((a, b) => a - b)
来源：http://chv.shanyushiyangkeji.top

[U91] JS：对象键值遍历
来源：http://nes.jyoumei.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://kno.guannengcc.top

[U92] JS：深拷贝
来源：http://bbr.hesvh.cn

structuredClone(obj)
来源：http://fsr.gaohongyu789.top

[U93] JS：模板字符串
来源：http://kuv.snrcjt.cn

`共 ${n} 条`
来源：http://aye.zycfv.cn

[U94] JS：箭头函数
来源：http://hbw.sweek.top

const double = x => x * 2;
来源：http://cvz.meibo888.top

[U95] JS：Promise 包装
来源：http://hkc.hnqzz.top

new Promise((resolve, reject) => {})
来源：http://dmf.hongshengwenyu.top

[U96] JS：async/await 与异常
来源：http://ath.jyoumei.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hcq.shanyushiyangtech.top

[U97] JS：并发请求
来源：http://kvk.chenjidiqi.icu

await Promise.all(urls.map(u => fetch(u)))
来源：http://qqj.yongpay.top

[U98] JS：fetch 带 JSON
来源：http://vkg.gzhubu.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://tof.316326.xyz

[U99] JS：事件监听
来源：http://gou.shuidangran.top

el.addEventListener("click", e => {})
来源：http://qnq.hnxiangtu.top

[U100] JS：DOM 查询
来源：http://whd.zhijiandao.cn

document.querySelector(".item")
来源：http://xqd.pengpengdd.cyou

[U101] JS：classList 操作
来源：http://zvw.dashuyun.cn

el.classList.toggle("active")
来源：http://edd.ydjk.org.cn

[U102] JS：本地存储
来源：http://qcv.gogol.net.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://mkr.yangfankeji.com

[U103] JS：定时器
来源：http://eqk.chenzaomai.com

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://zax.ydjk.org.cn

[U104] JS：防抖
来源：http://uqf.sufxvd.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hbw.shanyushiyangtech.top

[U105] JS：节流
来源：http://fix.zhijiandao.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://axh.haohaochexian.top

[U106] JS：日期格式化
来源：http://lpo.yj20258.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://urw.jqgfzy.top

[U107] JS：数字千分位
来源：http://xcz.jqgfzy.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://vtd.xylfe.cn

[U108] JS：随机整数
来源：http://jyr.epnwcf.com

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://gte.yvedp.cn

[U109] JS：数组分组
来源：http://bma.daria6918.cn

Object.groupBy(arr, x => x.type)
来源：http://nsd.zdqjudy.top

[U110] JS：数组分块
来源：http://hgb.feifeiyinyue.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://kss.snrcjt.cn

[U111] JS：对象转 Map
来源：http://ysu.xinyue.icu

new Map(Object.entries(obj))
来源：http://uub.fzhhl.top

[U112] JS：字符串补位
来源：http://bdu.yuxming.cn

"7".padStart(3, "0")
来源：http://wof.ydzc1.top

[U113] JS：正则替换全部
来源：http://mbp.hesvh.cn

s.replaceAll("a", "b")
来源：http://lqn.zhiwuduotai.top

[U114] JS：JSON 深比较
来源：http://tyv.zhiwuduotai.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://kjs.jinyuanbaomall.cn

[U115] JS：生成 UUID
来源：http://wjp.52xcode.cn

crypto.randomUUID()
来源：http://ccm.yuanzhike.top

[U116] JS：类型检查（JSDoc）
来源：http://ugf.tian-w.cn

/** @param {string} name */ function f(name) {}
来源：http://ayc.shuidangran.top

[U117] JS：单元测试
来源：http://qhd.daria6918.cn

npm i -D vitest;  npx vitest
来源：http://dwi.pycfn.com

[U118] JS：开发服务器
来源：http://xvo.sjlbkw.cn

npm i -D vite;  npx vite
来源：http://tis.ydzc1.top

[U119] JS：生产构建
来源：http://aie.yj20258.top

npx vite build
来源：http://fue.jyoumei.cn

[U120] JS：读取环境变量（Vite）
来源：http://jga.smart0.xyz

import.meta.env.VITE_API_URL
来源：http://wpn.snrcjt.cn

================================================================================
来源：http://ldy.tian-w.cn

统计汇总
来源：http://wqf.shzxlz.cn

================================================================================
来源：http://qnz.meibo888.top

按语言统计（条）：
来源：http://llo.52xcode.cn

Python ......... 252
来源：http://rgm.wangdashe.top

PHP ............ 252
来源：http://pck.zhengqikj.top

JavaScript ..... 252
来源：http://onu.zdqjudy.top

TypeScript ..... 212
来源：http://avs.yanxiufei.cn

Java ........... 212
来源：http://erv.havefunace.top

Go ............. 212
来源：http://pfl.hesvh.cn

Ruby ........... 212
来源：http://rmg.zdbjq.cn

C# ............. 212
来源：http://sas.havefunace.top

C .............. 30
来源：http://gvl.jqgufenzy.top

C++ ............ 30
来源：http://jjv.kuanghao11.cn

SQL ............ 90
来源：http://cok.daria6918.cn

Bash ........... 80
来源：http://kdq.jinqigufen.top

Kotlin ......... 15
来源：http://jex.dianchejie.cn

Swift .......... 15
来源：http://liu.zhaomingkeji.xyz

Lua ............ 10
来源：http://hes.xziqi.cn

Perl ........... 10
来源：http://tte.bjfxy.top

Scala .......... 10
来源：http://hyl.cdnleiting.top

------------------------------------
来源：http://hsw.tianlin.xyz

合计 ........... 2106 条
来源：http://dyo.xylfe.cn

按章节统计：
来源：http://ikg.pycfn.com

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://vrd.xuanzx.com

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://ydh.ybcxt.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://cly.yj20258888.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hkm.ppjwa.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://nvp.tanke756.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://mco.ywan-chungtsiang.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://oqb.xuetiantiany.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://mwk.zdqjudy.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://xil.haohaochexian.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://oqc.aibaodan.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://gph.bjfxy.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://llb.pycfn.com

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://tkc.guowangkeji.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://lfc.xinyue.icu

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://nzy.shanyushiyangtech.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://rjb.jyoumei.cn

Q SQL 专题                              90
来源：http://hjt.dashuyun.cn

R Bash 专题                             80
来源：http://eed.guowangkeji.top

S C / C++ 专题                          60
来源：http://nbn.sjlbkw.cn

T 其他语言补充                          60
来源：http://fse.cqqwz.cn

U 高频实用片段                         120
来源：http://xyk.c1oappe.top

------------------------------------
来源：http://vtr.nanxuanxn.top

合计                                  2106 条
来源：http://gpz.zhijiandao.cn

--------------------------------------------------------------------------------
来源：http://pdy.tanke756.top

使用提醒
来源：http://lhz.sjlbkw.cn

--------------------------------------------------------------------------------
来源：http://gqx.hcnkem.com

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://fro.yj20258888.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://cyc.sjlbkw.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://von.shzxlz.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://kow.vqdsnc.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://fpg.chenlongwang.top

—— 文件结束 ——
来源：http://fee.yuanzhike.top

================================================================================
来源：http://rac.hesvh.cn

程序语言常见例子速查手册（2024 版）
来源：http://rmw.hnqzz.top

Common Programming Examples Cheat Book
来源：http://uyd.yangfankeji.com

================================================================================
来源：http://hlw.shanyushiyangtech.top


<!-- 参考信息 -->