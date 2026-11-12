代发 wailian999

[U03] Py：加载 .env 配置
来源：http://doq.nwbrower.top

from dotenv import load_dotenv; load_dotenv()
来源：http://nke.pycfn.com

[U04] Py：变量调试打印
来源：http://ljr.zhaomingkeji.xyz

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://zpn.yanxiufei.cn

[U05] Py：列表去重且保序
来源：http://qpe.aibaodan.cn

list(dict.fromkeys(arr))
来源：http://tlf.guannengcc.top

[U06] Py：合并两个字典
来源：http://xmf.bbcook.cn

{**a, **b}
来源：http://vld.guowangkeji.top

[U07] Py：反转字典键值
来源：http://gsm.hammf.cn

{v: k for k, v in d.items()}
来源：http://hfm.hfpthk.cn

[U08] Py：展平二维列表
来源：http://yfq.hesvh.cn

[y for x in nested for y in x]
来源：http://hsx.kuanghao11.cn

[U09] Py：字典取最大值的键
来源：http://wek.316326.xyz

max(d, key=d.get)
来源：http://mca.hnxiangtu.top

[U10] Py：按值排序字典
来源：http://ahv.uphjek.com

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://rfx.chenjidiqi.icu

[U11] Py：生成器表达式
来源：http://qcq.c1oappe.top

(x * 2 for x in arr)
来源：http://tto.iojbl.cn

[U12] Py：取出现最多的 3 个元素
来源：http://mjq.yangfankeji.com

Counter(arr).most_common(3)
来源：http://ppx.jinghuilouyu.cn

[U13] Py：固定长度队列
来源：http://pem.ctjpmb.com

deque(maxlen=10)
来源：http://dfb.daxiang520.top

[U14] Py：分组收集到列表
来源：http://xef.smart0.xyz

defaultdict(list)
来源：http://vlh.zhongyouzk.top

[U15] Py：高精度计时
来源：http://oye.wangshuangyany.cn

t = time.perf_counter()
来源：http://jqc.cqqwz.cn

[U16] Py：命令行参数解析
来源：http://ovc.c1oappe.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://vup.hfpthk.cn

[U17] Py：初始化日志
来源：http://jlw.sufxvd.cn

logging.basicConfig(level=logging.INFO)
来源：http://khx.guowangkeji.top

[U18] Py：预编译正则
来源：http://sep.hywenlv.cn

pat = re.compile(r"\d+")
来源：http://tun.wangdashe.top

[U19] Py：正则替换带回调
来源：http://cza.ydjk.org.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://opp.zhoulong.xyz

[U20] Py：缓存函数结果
来源：http://jdb.fehbvm.com

@functools.lru_cache(maxsize=None)
来源：http://uzf.jyoumei.cn

[U21] Py：自定义上下文管理器
来源：http://zfz.ywan-chungtsiang.top

@contextlib.contextmanager
来源：http://wvt.haohaochexian.top

[U22] Py：矩阵转置
来源：http://seq.birdmap.top

list(zip(*m))
来源：http://oqe.aizwys.cn

[U23] Py：分块读取大文件
来源：http://efe.zhixingplan.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://pin.svipenyu.cn

[U24] Py：路径操作
来源：http://vis.ywan-chungtsiang.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://zok.gotoacloud.top

[U25] Py：CSV 按字典读
来源：http://xyc.cucudq.cn

csv.DictReader(f)
来源：http://ejg.iojbl.cn

[U26] Py：并发下载
来源：http://tny.shangyingyoupin.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://jza.yj202588.top

[U27] Py：异步 HTTP
来源：http://kqw.zhijiandao.cn

aiohttp.ClientSession() 配合 async with
来源：http://hfw.hnxiangtu.top

[U28] Py：类型别名
来源：http://gny.cashguo.top

UserId = int
来源：http://dik.yfazqb.com

[U29] Py：属性校验
来源：http://ejo.yuxming.cn

@property 与 @x.setter 配合
来源：http://muo.wangshuangyany.cn

[U30] Py：数据类
来源：http://rlm.fktsv.cn

@dataclass(slots=True)
来源：http://iuv.cucudq.cn

[U31] Py：单测
来源：http://qif.zhixingplan.top

python -m pytest -q
来源：http://mud.zhongyouzk.top

[U32] Py：代码格式化
来源：http://dxk.hammf.cn

ruff format . && ruff check --fix .
来源：http://cgf.shangyingyoupin.top

[U33] Py：打包发布
来源：http://ocd.wangdashe.top

python -m build  （依赖 pyproject.toml）
来源：http://fww.yuxming.cn

[U34] Py：判断编码
来源：http://jok.havefunace.top

chardet.detect(raw)
来源：http://xfs.zhijiandao.cn

[U35] Py：发送邮件
来源：http://rzl.shanyushiyangkeji.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://qcj.yangfankeji.com

[U36] Py：定时任务
来源：http://xkp.hongshengwenyu.top

schedule.every(10).minutes.do(job)
来源：http://mzx.jinqigufen.top

[U37] Py：读写 Excel
来源：http://gru.meibo888.top

pandas.read_excel / DataFrame.to_excel
来源：http://rlx.fktsv.cn

[U38] Py：获取脚本所在目录
来源：http://hrd.haohaochexian.top

Path(__file__).resolve().parent
来源：http://qfj.jinqigfzy.top

[U39] Py：判断是否在交互环境
来源：http://oex.yj202588.top

sys.stdout.isatty()
来源：http://mkf.c1oappe.top

[U40] Py：打印到标准错误
来源：http://rhi.vqdsnc.cn

print("err", file=sys.stderr)
来源：http://ehn.gzhubu.top

[U41] PHP：初始化 Composer 项目
来源：http://izg.hnqzz.top

composer init;  composer require guzzlehttp/guzzle
来源：http://lnk.daria6918.cn

[U42] PHP：PSR-4 自动加载
来源：http://wny.sxryk.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://mva.gaohongyu789.top

[U43] PHP：声明命名空间
来源：http://hlb.wangdashe.top

namespace App\Http;
来源：http://ggw.wangdashe.top

[U44] PHP：开启严格类型
来源：http://zcj.shuidangran.top

declare(strict_types=1);
来源：http://zzk.zhengqikj.top

[U45] PHP：类型声明与返回类型
来源：http://ink.guowangkeji.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://dat.yj202588.top

[U46] PHP：可空类型
来源：http://qnk.ydzc1.top

?string $name = null
来源：http://qpc.hywenlv.cn

[U47] PHP：联合类型
来源：http://luc.zhoulong.xyz

int|string $id
来源：http://tfw.c1oappe.top

[U48] PHP：纯枚举
来源：http://efw.cashguo.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://oep.zhongyouzk.top

[U49] PHP：只读属性
来源：http://kqk.guowangkeji.top

public readonly string $name
来源：http://wyp.sufxvd.cn

[U50] PHP：构造器属性提升
来源：http://fum.svipenyu.cn

public function __construct(private int $id) {}
来源：http://idi.daxiang520.top

[U51] PHP：数组解构
来源：http://lfs.ydzc1.top

[$a, $b] = $arr;
来源：http://hcm.epnwcf.com

[U52] PHP：箭头函数
来源：http://fkw.uphjek.com

$double = fn($x) => $x * 2;
来源：http://jny.aizwys.cn

[U53] PHP：空合并运算符
来源：http://hwc.jinghuilouyu.cn

$v = $a ?? $b ?? "default";
来源：http://aay.sweek.top

[U54] PHP：空安全调用
来源：http://bir.yangfankeji.com

$obj?->method()
来源：http://oed.xinyue.icu

[U55] PHP：match 表达式
来源：http://pbo.birdmap.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://gof.hcnkem.com

[U56] PHP：命名参数
来源：http://eva.aibaodan.cn

f(a: 1, b: 2)
来源：http://zfx.yueranfly.top

[U57] PHP：字符串插值
来源：http://jhp.bjfxy.top

"值: {$a}"
来源：http://zbl.fengsongda.top

[U58] PHP：数组三件套
来源：http://tac.xingfuxueyuan.xyz

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://ewz.wangdashe.top

[U59] PHP：自定义排序
来源：http://awj.andypj.xyz

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://kic.guannengcc.top

[U60] PHP：JSON 编解码
来源：http://bjd.tianlin.xyz

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://ugl.jlsjyb.cn

[U61] PHP：正则
来源：http://sbu.yvedp.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://ksw.hywenlv.cn

[U62] PHP：日期对象
来源：http://trm.mhx1999.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://jed.52xcode.cn

[U63] PHP：文件读写
来源：http://zzb.snrcjt.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://cez.yanxiufei.cn

[U64] PHP：目录遍历
来源：http://afq.aibaodan.cn

glob("dir/*.php");  scandir("dir");
来源：http://xih.cqqwz.cn

[U65] PHP：会话
来源：http://gos.xuetiantiany.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://wix.jinghuilouyu.cn

[U66] PHP：设置 Cookie
来源：http://aff.tianlin.xyz

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://tzf.birdmap.top

[U67] PHP：处理文件上传
来源：http://zol.hongshengwenyu.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://fld.hysaishi.cn

[U68] PHP：PDO 连接
来源：http://rbp.nwbrower.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://swn.sweek.top

[U69] PHP：PDO 预处理
来源：http://klq.bjfxy.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://pos.xylfe.cn

[U70] PHP：PDO 事务
来源：http://plf.yonumen.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://bbb.fengsongda.top

[U71] PHP：抛出异常
来源：http://php.hnqzz.top

throw new RuntimeException("失败", 500);
来源：http://zhq.cheryme.top

[U72] PHP：写错误日志
来源：http://ppv.zhixingplan.top

error_log("失败: " . $e->getMessage());
来源：http://ayh.feifeiyinyue.top

[U73] PHP：读取 ini 配置
来源：http://ksz.ydjk.org.cn

parse_ini_file("config.ini", true)
来源：http://gxw.yanxiufei.cn

[U74] PHP：读取环境变量
来源：http://isn.ehwqpu.com

getenv("APP_ENV") ?: "production"
来源：http://vmx.cqqwz.cn

[U75] PHP：依赖注入
来源：http://obp.wangdashe.top

composer require psr/container
来源：http://qpb.hywenlv.cn

[U76] PHP：简单路由
来源：http://jtd.zhaomingkeji.xyz

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://tlq.jiagoushi.top

[U77] PHP：模板渲染
来源：http://daa.nanxuanxn.top

composer require twig/twig
来源：http://qwb.jlsjyb.cn

[U78] PHP：单元测试
来源：http://lfm.yuxming.cn

composer require --dev phpunit/phpunit
来源：http://psp.sjlbkw.cn

[U79] PHP：静态分析
来源：http://nph.hcnkem.com

composer require --dev phpstan/phpstan
来源：http://opk.epnwcf.com

[U80] PHP：代码规范修复
来源：http://lld.hnqzz.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://tvs.yueranfly.top

[U81] JS：初始化项目
来源：http://wba.aizwys.cn

npm init -y;  npm i express
来源：http://bbl.ctjpmb.com

[U82] JS：package.json 脚本
来源：http://fud.0kj1m.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://hdm.quarkkingdee.top

[U83] JS：ES Module 导入导出
来源：http://vih.havefunace.top

export const a = 1;  import { a } from "./m.js";
来源：http://anx.yueranfly.top

[U84] JS：CommonJS 写法
来源：http://pyo.jlsjyb.cn

module.exports = { a };  const { a } = require("./m");
来源：http://zng.bbcook.cn

[U85] JS：可选链
来源：http://nkg.zhixingplan.top

a?.b?.c
来源：http://hys.hcnkem.com

[U86] JS：空值合并
来源：http://idn.zhiwuduotai.top

a ?? b
来源：http://gmf.zhongyouzk.top

[U87] JS：解构默认值
来源：http://pke.xylfe.cn

const { a = 1, b = 2 } = obj;
来源：http://qcr.yvedp.cn

[U88] JS：对象展开合并
来源：http://lwa.snrcjt.cn

{ ...a, ...b }
来源：http://cqa.sysykeji.top

[U89] JS：数组去重
来源：http://osy.tarul.cn

[...new Set(arr)]
来源：http://twx.yvedp.cn

[U90] JS：数字数组排序
来源：http://wxd.shangyingyoupin.top

[...arr].sort((a, b) => a - b)
来源：http://utx.hysaishi.cn

[U91] JS：对象键值遍历
来源：http://aun.haohaochexian.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://lay.jinqigfzy.top

[U92] JS：深拷贝
来源：http://aro.sxryk.cn

structuredClone(obj)
来源：http://pmh.fehbvm.com

[U93] JS：模板字符串
来源：http://lor.316326.xyz

`共 ${n} 条`
来源：http://exq.aizwys.cn

[U94] JS：箭头函数
来源：http://lmw.chenlongwang.top

const double = x => x * 2;
来源：http://ftv.yj202588.top

[U95] JS：Promise 包装
来源：http://bxc.hywenlv.cn

new Promise((resolve, reject) => {})
来源：http://spg.sxryk.cn

[U96] JS：async/await 与异常
来源：http://unn.gotoacloud.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://yvg.hesvh.cn

[U97] JS：并发请求
来源：http://nzh.quarkkingdee.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://qfn.gzhubu.top

[U98] JS：fetch 带 JSON
来源：http://myv.meibo888.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://jfm.sxryk.cn

[U99] JS：事件监听
来源：http://akd.fzhhl.top

el.addEventListener("click", e => {})
来源：http://wge.vehdjk.com

[U100] JS：DOM 查询
来源：http://jah.fanxiaobao.xyz

document.querySelector(".item")
来源：http://wqr.tarul.cn

[U101] JS：classList 操作
来源：http://klw.yj202588.top

el.classList.toggle("active")
来源：http://suj.tian-w.cn

[U102] JS：本地存储
来源：http://wiq.tian-w.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://acm.daria6918.cn

[U103] JS：定时器
来源：http://uri.xylfe.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://fda.aibaodan.cn

[U104] JS：防抖
来源：http://jwu.ivvv.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://uno.svipenyu.cn

[U105] JS：节流
来源：http://rdy.jqgfzy.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://dmq.fktsv.cn

[U106] JS：日期格式化
来源：http://dtz.mhx1999.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://esw.cashguo.top

[U107] JS：数字千分位
来源：http://dyv.jinyuanbaomall.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hob.jyoumei.cn

[U108] JS：随机整数
来源：http://hct.hongshengwenyu.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://qsm.guowangkeji.top

[U109] JS：数组分组
来源：http://tli.hysaishi.cn

Object.groupBy(arr, x => x.type)
来源：http://hjo.hammf.cn

[U110] JS：数组分块
来源：http://pca.bbcook.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://por.xylfe.cn

[U111] JS：对象转 Map
来源：http://cso.smart0.xyz

new Map(Object.entries(obj))
来源：http://uln.dashuyun.cn

[U112] JS：字符串补位
来源：http://xkz.smart0.xyz

"7".padStart(3, "0")
来源：http://dmb.wangdashe.top

[U113] JS：正则替换全部
来源：http://lge.gzhubu.top

s.replaceAll("a", "b")
来源：http://ois.yvedp.cn

[U114] JS：JSON 深比较
来源：http://ice.0kj1m.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://uuw.zhiwuduotai.top

[U115] JS：生成 UUID
来源：http://xgf.sweek.top

crypto.randomUUID()
来源：http://tua.xuanzx.com

[U116] JS：类型检查（JSDoc）
来源：http://zil.yuanzhike.top

/** @param {string} name */ function f(name) {}
来源：http://lcp.uphjek.com

[U117] JS：单元测试
来源：http://zvi.ydjk.org.cn

npm i -D vitest;  npx vitest
来源：http://gmz.fzhhl.top

[U118] JS：开发服务器
来源：http://tdv.shanyushiyangkeji.top

npm i -D vite;  npx vite
来源：http://nnf.fehbvm.com

[U119] JS：生产构建
来源：http://zui.jiagoushi.top

npx vite build
来源：http://qgn.uphjek.com

[U120] JS：读取环境变量（Vite）
来源：http://mjs.fktsv.cn

import.meta.env.VITE_API_URL
来源：http://mpv.cheryme.top

================================================================================
来源：http://sgm.wangdashe.top

统计汇总
来源：http://ixt.zhoulong.xyz

================================================================================
来源：http://hru.yj202588.top

按语言统计（条）：
来源：http://qjh.hammf.cn

Python ......... 252
来源：http://end.c1oappe.top

PHP ............ 252
来源：http://cpa.jlsjyb.cn

JavaScript ..... 252
来源：http://ucz.zhaomingkeji.xyz

TypeScript ..... 212
来源：http://bqh.haohaochexian.top

Java ........... 212
来源：http://bdj.bbcook.cn

Go ............. 212
来源：http://axt.jinyuanbaomall.cn

Ruby ........... 212
来源：http://rnu.jlsjyb.cn

C# ............. 212
来源：http://lpb.redwolf501.top

C .............. 30
来源：http://caj.jinghuilouyu.cn

C++ ............ 30
来源：http://lnt.yvedp.cn

SQL ............ 90
来源：http://fiw.zhijiandao.cn

Bash ........... 80
来源：http://csd.smart0.xyz

Kotlin ......... 15
来源：http://zil.9152youxi.cn

Swift .......... 15
来源：http://wfj.yuanzhike.top

Lua ............ 10
来源：http://tzh.pycfn.com

Perl ........... 10
来源：http://dwr.ehwqpu.com

Scala .......... 10
来源：http://xhy.tianlin.xyz

------------------------------------
来源：http://dni.zdbjq.cn

合计 ........... 2106 条
来源：http://nfu.sjlbkw.cn

按章节统计：
来源：http://lxd.ydzc1.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://kwn.hnxiangtu.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://pki.daxiang520.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://tba.zhixingplan.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://wzd.aizwys.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://qoc.9152youxi.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://vba.sjlbkw.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://urf.zhaomingkeji.xyz

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://glf.daria6918.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://gqy.yvedp.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://zrr.hongshengwenyu.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://tqz.xingfuxueyuan.xyz

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://zst.yfazqb.com

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://gqo.shangyingyoupin.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://nrb.smart0.xyz

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://ncf.ehwqpu.com

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://fwf.jqgfzy.top

Q SQL 专题                              90
来源：http://pad.jinyuanbaomall.cn

R Bash 专题                             80
来源：http://nyz.aizwys.cn

S C / C++ 专题                          60
来源：http://gif.chenjidiqi.icu

T 其他语言补充                          60
来源：http://lri.gogol.net.cn

U 高频实用片段                         120
来源：http://daf.zhixingplan.top

------------------------------------
来源：http://pgb.epnwcf.com

合计                                  2106 条
来源：http://ljg.hnqzz.top

--------------------------------------------------------------------------------
来源：http://jvm.pycfn.com

使用提醒
来源：http://fxg.meibo888.top

--------------------------------------------------------------------------------
来源：http://obo.birdmap.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://mhn.birdmap.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://phc.yuanzhike.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://umt.gaohongyu789.top

在旧版本上使用前请先确认语法支持情况。
来源：http://rlw.svipenyu.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://yms.shuidangran.top

—— 文件结束 ——
来源：http://rdm.zhijiandao.cn

================================================================================
来源：http://idi.nwbrower.top

程序语言常见例子速查手册（2024 版）
来源：http://hhc.yj20258.top

Common Programming Examples Cheat Book
来源：http://bur.hfpthk.cn

================================================================================
来源：http://yvi.nanxuanxn.top

【收录内容】
来源：http://eef.cqqwz.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://yns.uphjek.com

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://nmi.zhongyouzk.top

SQL · Bash · C · C++
来源：http://pvx.fktsv.cn


<!-- 参考信息 -->