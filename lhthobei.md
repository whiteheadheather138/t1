代发 wailian999

[U05] Py：列表去重且保序
来源：http://byz.gaohongyu789.top

list(dict.fromkeys(arr))
来源：http://adx.sufxvd.cn

[U06] Py：合并两个字典
来源：http://wdh.pycfn.com

{**a, **b}
来源：http://ras.daxiang520.top

[U07] Py：反转字典键值
来源：http://pqw.pycfn.com

{v: k for k, v in d.items()}
来源：http://suc.hfpthk.cn

[U08] Py：展平二维列表
来源：http://gzd.jinyuanbaomall.cn

[y for x in nested for y in x]
来源：http://yyq.52xcode.cn

[U09] Py：字典取最大值的键
来源：http://oep.wangdashe.top

max(d, key=d.get)
来源：http://fsb.yuxming.cn

[U10] Py：按值排序字典
来源：http://qwx.sufxvd.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://sys.smart0.xyz

[U11] Py：生成器表达式
来源：http://vop.hfpthk.cn

(x * 2 for x in arr)
来源：http://lmn.ppjwa.cn

[U12] Py：取出现最多的 3 个元素
来源：http://rtb.shangyingyoupin.top

Counter(arr).most_common(3)
来源：http://mya.xziqi.cn

[U13] Py：固定长度队列
来源：http://rpk.zhongyouzk.top

deque(maxlen=10)
来源：http://cbu.c1oappe.top

[U14] Py：分组收集到列表
来源：http://fam.smart0.xyz

defaultdict(list)
来源：http://pis.nwbrower.top

[U15] Py：高精度计时
来源：http://njn.meibo888.top

t = time.perf_counter()
来源：http://pzp.zhijiandao.cn

[U16] Py：命令行参数解析
来源：http://gpm.feifeiyinyue.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://oiv.tanke756.top

[U17] Py：初始化日志
来源：http://oxb.fzhhl.top

logging.basicConfig(level=logging.INFO)
来源：http://abg.jqgfzy.top

[U18] Py：预编译正则
来源：http://ggc.fktsv.cn

pat = re.compile(r"\d+")
来源：http://bxb.jyoumei.cn

[U19] Py：正则替换带回调
来源：http://ksd.fengsongda.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://ibc.sysykeji.top

[U20] Py：缓存函数结果
来源：http://fgm.uphjek.com

@functools.lru_cache(maxsize=None)
来源：http://tiw.gotoacloud.top

[U21] Py：自定义上下文管理器
来源：http://ndo.yonumen.top

@contextlib.contextmanager
来源：http://ghk.hnqzz.top

[U22] Py：矩阵转置
来源：http://ewy.cqqwz.cn

list(zip(*m))
来源：http://vye.tarul.cn

[U23] Py：分块读取大文件
来源：http://fdl.xylfe.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://kzy.yuxming.cn

[U24] Py：路径操作
来源：http://yfo.sjlbkw.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://wnz.daria6918.cn

[U25] Py：CSV 按字典读
来源：http://nuq.vqdsnc.cn

csv.DictReader(f)
来源：http://fko.zhijiandao.cn

[U26] Py：并发下载
来源：http://jkr.316326.xyz

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://vhr.jlsjyb.cn

[U27] Py：异步 HTTP
来源：http://cgo.vehdjk.com

aiohttp.ClientSession() 配合 async with
来源：http://brb.daria6918.cn

[U28] Py：类型别名
来源：http://cuz.jinqigfzy.top

UserId = int
来源：http://wht.andypj.xyz

[U29] Py：属性校验
来源：http://wdf.jinyuanbaomall.cn

@property 与 @x.setter 配合
来源：http://beg.yuanzhike.top

[U30] Py：数据类
来源：http://wuv.zhiwuduotai.top

@dataclass(slots=True)
来源：http://scd.gzhubu.top

[U31] Py：单测
来源：http://fwb.guowangkeji.top

python -m pytest -q
来源：http://xrd.ywan-chungtsiang.top

[U32] Py：代码格式化
来源：http://dth.zhixingplan.top

ruff format . && ruff check --fix .
来源：http://bbj.hnqzz.top

[U33] Py：打包发布
来源：http://uxo.shangyingyoupin.top

python -m build  （依赖 pyproject.toml）
来源：http://oso.c1oappe.top

[U34] Py：判断编码
来源：http://erf.zhixingplan.top

chardet.detect(raw)
来源：http://cel.cashguo.top

[U35] Py：发送邮件
来源：http://sbc.yj202588.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hrt.yonumen.top

[U36] Py：定时任务
来源：http://rmo.yj20258.top

schedule.every(10).minutes.do(job)
来源：http://cep.hnqzz.top

[U37] Py：读写 Excel
来源：http://gmn.jinqigfzy.top

pandas.read_excel / DataFrame.to_excel
来源：http://ggw.hcnkem.com

[U38] Py：获取脚本所在目录
来源：http://inh.gogol.net.cn

Path(__file__).resolve().parent
来源：http://oid.hammf.cn

[U39] Py：判断是否在交互环境
来源：http://weq.tanke756.top

sys.stdout.isatty()
来源：http://plr.ybcxt.top

[U40] Py：打印到标准错误
来源：http://jpl.smart0.xyz

print("err", file=sys.stderr)
来源：http://gsb.meibo888.top

[U41] PHP：初始化 Composer 项目
来源：http://fvf.sxryk.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://ajg.xinyue.icu

[U42] PHP：PSR-4 自动加载
来源：http://xfi.wangdashe.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://rkj.yueranfly.top

[U43] PHP：声明命名空间
来源：http://ewm.guannengcc.top

namespace App\Http;
来源：http://gns.ybcxt.top

[U44] PHP：开启严格类型
来源：http://wxc.shanyushiyangtech.top

declare(strict_types=1);
来源：http://lrv.nwbrower.top

[U45] PHP：类型声明与返回类型
来源：http://mne.xylfe.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://ckb.uphjek.com

[U46] PHP：可空类型
来源：http://kzd.tanke756.top

?string $name = null
来源：http://tbs.jinyuanbaomall.cn

[U47] PHP：联合类型
来源：http://ylt.zhongyouzk.top

int|string $id
来源：http://eqq.kuanghao11.cn

[U48] PHP：纯枚举
来源：http://vrp.vqdsnc.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://ebr.ydzc1.top

[U49] PHP：只读属性
来源：http://uex.xinyue.icu

public readonly string $name
来源：http://riv.aibaodan.cn

[U50] PHP：构造器属性提升
来源：http://gzx.sweek.top

public function __construct(private int $id) {}
来源：http://rbw.jinqigufen.top

[U51] PHP：数组解构
来源：http://pen.gzhubu.top

[$a, $b] = $arr;
来源：http://jet.shanyushiyangkeji.top

[U52] PHP：箭头函数
来源：http://cma.bjfxy.top

$double = fn($x) => $x * 2;
来源：http://zda.zhengqikj.top

[U53] PHP：空合并运算符
来源：http://dyg.nanxuanxn.top

$v = $a ?? $b ?? "default";
来源：http://ftq.gotoacloud.top

[U54] PHP：空安全调用
来源：http://rog.quarkkingdee.top

$obj?->method()
来源：http://rir.zhixingplan.top

[U55] PHP：match 表达式
来源：http://sft.tian-w.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://zmi.xziqi.cn

[U56] PHP：命名参数
来源：http://gaw.jinghuilouyu.cn

f(a: 1, b: 2)
来源：http://yev.hongshengwenyu.top

[U57] PHP：字符串插值
来源：http://idp.c1oappe.top

"值: {$a}"
来源：http://ecy.ybcxt.top

[U58] PHP：数组三件套
来源：http://zzl.gzhubu.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://jqp.redwolf501.top

[U59] PHP：自定义排序
来源：http://isg.c1oappe.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://xkw.yj20258888.top

[U60] PHP：JSON 编解码
来源：http://aum.0kj1m.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://ysl.wangdashe.top

[U61] PHP：正则
来源：http://iky.ybcxt.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://emf.zhengqikj.top

[U62] PHP：日期对象
来源：http://yws.ctjpmb.com

(new DateTimeImmutable())->format("Y-m-d");
来源：http://rcj.yangfankeji.com

[U63] PHP：文件读写
来源：http://cpd.yonumen.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://elc.guannengcc.top

[U64] PHP：目录遍历
来源：http://bdz.iojbl.cn

glob("dir/*.php");  scandir("dir");
来源：http://bta.zhiwuduotai.top

[U65] PHP：会话
来源：http://dip.316326.xyz

session_start();  $_SESSION["uid"] = 1;
来源：http://bbr.daxiang520.top

[U66] PHP：设置 Cookie
来源：http://ksa.aizwys.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://ene.hesvh.cn

[U67] PHP：处理文件上传
来源：http://lpv.pengpengdd.cyou

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://knq.hesvh.cn

[U68] PHP：PDO 连接
来源：http://bzc.hysaishi.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://lym.xylfe.cn

[U69] PHP：PDO 预处理
来源：http://xll.pycfn.com

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://mzd.xziqi.cn

[U70] PHP：PDO 事务
来源：http://cpm.zhaomingkeji.xyz

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://mob.epnwcf.com

[U71] PHP：抛出异常
来源：http://yaz.bbcook.cn

throw new RuntimeException("失败", 500);
来源：http://elg.cucudq.cn

[U72] PHP：写错误日志
来源：http://ufh.dianchejie.cn

error_log("失败: " . $e->getMessage());
来源：http://fhi.jlsjyb.cn

[U73] PHP：读取 ini 配置
来源：http://tub.gotoacloud.top

parse_ini_file("config.ini", true)
来源：http://emw.xziqi.cn

[U74] PHP：读取环境变量
来源：http://fvz.gotoacloud.top

getenv("APP_ENV") ?: "production"
来源：http://qts.zhoulong.xyz

[U75] PHP：依赖注入
来源：http://jgw.ydjk.org.cn

composer require psr/container
来源：http://qyk.zhongyouzk.top

[U76] PHP：简单路由
来源：http://vie.hfpthk.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://tuh.jianghu66.top

[U77] PHP：模板渲染
来源：http://arv.zhiwuduotai.top

composer require twig/twig
来源：http://mey.sjlbkw.cn

[U78] PHP：单元测试
来源：http://sdi.jqgfzy.top

composer require --dev phpunit/phpunit
来源：http://ndu.hywenlv.cn

[U79] PHP：静态分析
来源：http://ton.hywenlv.cn

composer require --dev phpstan/phpstan
来源：http://gsm.gzhubu.top

[U80] PHP：代码规范修复
来源：http://tyn.tian-w.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://wym.snrcjt.cn

[U81] JS：初始化项目
来源：http://jvl.hnxiangtu.top

npm init -y;  npm i express
来源：http://ywt.tarul.cn

[U82] JS：package.json 脚本
来源：http://pbk.gotoacloud.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://wiz.jqgfzy.top

[U83] JS：ES Module 导入导出
来源：http://yak.ivvv.top

export const a = 1;  import { a } from "./m.js";
来源：http://ijd.jianghu66.top

[U84] JS：CommonJS 写法
来源：http://yxu.cucudq.cn

module.exports = { a };  const { a } = require("./m");
来源：http://gfg.hnxiangtu.top

[U85] JS：可选链
来源：http://upg.sxryk.cn

a?.b?.c
来源：http://kep.ctjpmb.com

[U86] JS：空值合并
来源：http://leo.jqgfzy.top

a ?? b
来源：http://tpf.tian-w.cn

[U87] JS：解构默认值
来源：http://kzy.andypj.xyz

const { a = 1, b = 2 } = obj;
来源：http://eii.zycfv.cn

[U88] JS：对象展开合并
来源：http://ece.52xcode.cn

{ ...a, ...b }
来源：http://tij.zhoulong.xyz

[U89] JS：数组去重
来源：http://tuu.cashguo.top

[...new Set(arr)]
来源：http://xgz.jqgufenzy.top

[U90] JS：数字数组排序
来源：http://zfv.yangfankeji.com

[...arr].sort((a, b) => a - b)
来源：http://uzv.yuanzhike.top

[U91] JS：对象键值遍历
来源：http://cun.fehbvm.com

Object.entries(obj).forEach(([k, v]) => {});
来源：http://qph.svipenyu.cn

[U92] JS：深拷贝
来源：http://iyv.iojbl.cn

structuredClone(obj)
来源：http://rrd.zycfv.cn

[U93] JS：模板字符串
来源：http://wpl.hammf.cn

`共 ${n} 条`
来源：http://rfv.ivvv.top

[U94] JS：箭头函数
来源：http://idi.ppjwa.cn

const double = x => x * 2;
来源：http://hnt.pycfn.com

[U95] JS：Promise 包装
来源：http://laj.yonumen.top

new Promise((resolve, reject) => {})
来源：http://lhq.hesvh.cn

[U96] JS：async/await 与异常
来源：http://bro.meibo888.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://fym.hnqzz.top

[U97] JS：并发请求
来源：http://oig.cdnleiting.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://gxl.cdnleiting.top

[U98] JS：fetch 带 JSON
来源：http://thi.kuanghao11.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://fsz.yj20258888.top

[U99] JS：事件监听
来源：http://yti.shuidangran.top

el.addEventListener("click", e => {})
来源：http://mhf.tian-w.cn

[U100] JS：DOM 查询
来源：http://ubi.yvedp.cn

document.querySelector(".item")
来源：http://inw.zhijiandao.cn

[U101] JS：classList 操作
来源：http://eff.xziqi.cn

el.classList.toggle("active")
来源：http://mtk.bjfxy.top

[U102] JS：本地存储
来源：http://soe.hnxiangtu.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://kqv.gotoacloud.top

[U103] JS：定时器
来源：http://uba.guannengcc.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://vbe.bbcook.cn

[U104] JS：防抖
来源：http://ehz.yueranfly.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://qga.yj202588.top

[U105] JS：节流
来源：http://hef.yvedp.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://tot.jinghuilouyu.cn

[U106] JS：日期格式化
来源：http://cgl.ybcxt.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://azw.sxryk.cn

[U107] JS：数字千分位
来源：http://llc.nanxuanxn.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://pbx.ehwqpu.com

[U108] JS：随机整数
来源：http://qod.0kj1m.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://mqv.sysykeji.top

[U109] JS：数组分组
来源：http://zvr.yfazqb.com

Object.groupBy(arr, x => x.type)
来源：http://hxo.yuxming.cn

[U110] JS：数组分块
来源：http://uwu.dashuyun.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://phn.gzhubu.top

[U111] JS：对象转 Map
来源：http://rhp.yuxming.cn

new Map(Object.entries(obj))
来源：http://obs.chenlongwang.top

[U112] JS：字符串补位
来源：http://poi.hammf.cn

"7".padStart(3, "0")
来源：http://soo.aibaodan.cn

[U113] JS：正则替换全部
来源：http://rdy.0kj1m.cn

s.replaceAll("a", "b")
来源：http://fqj.zhiwuduotai.top

[U114] JS：JSON 深比较
来源：http://buw.jqgufenzy.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://znd.xingfuxueyuan.xyz

[U115] JS：生成 UUID
来源：http://wzk.jinghuilouyu.cn

crypto.randomUUID()
来源：http://wnd.wangdashe.top

[U116] JS：类型检查（JSDoc）
来源：http://txz.cashguo.top

/** @param {string} name */ function f(name) {}
来源：http://qlz.daria6918.cn

[U117] JS：单元测试
来源：http://mzv.sufxvd.cn

npm i -D vitest;  npx vitest
来源：http://vfk.hammf.cn

[U118] JS：开发服务器
来源：http://ply.316326.xyz

npm i -D vite;  npx vite
来源：http://tdh.mhx1999.top

[U119] JS：生产构建
来源：http://omq.jqgufenzy.top

npx vite build
来源：http://eqy.ppjwa.cn

[U120] JS：读取环境变量（Vite）
来源：http://fey.xingfuxueyuan.xyz

import.meta.env.VITE_API_URL
来源：http://stc.yuanzhike.top

================================================================================
来源：http://pad.fehbvm.com

统计汇总
来源：http://zwk.ehwqpu.com

================================================================================
来源：http://bsl.sufxvd.cn

按语言统计（条）：
来源：http://zko.ydzc1.top

Python ......... 252
来源：http://ilz.gzhubu.top

PHP ............ 252
来源：http://slz.fzhhl.top

JavaScript ..... 252
来源：http://cuw.dianchejie.cn

TypeScript ..... 212
来源：http://uzm.guannengcc.top

Java ........... 212
来源：http://ifm.jlsjyb.cn

Go ............. 212
来源：http://ttq.hammf.cn

Ruby ........... 212
来源：http://cxx.fzhhl.top

C# ............. 212
来源：http://std.hysaishi.cn

C .............. 30
来源：http://zdj.ctjpmb.com

C++ ............ 30
来源：http://euz.ehwqpu.com

SQL ............ 90
来源：http://bir.iojbl.cn

Bash ........... 80
来源：http://ekw.ydzc1.top

Kotlin ......... 15
来源：http://ziu.ydjk.org.cn

Swift .......... 15
来源：http://fcb.aibaodan.cn

Lua ............ 10
来源：http://ktp.yangfankeji.com

Perl ........... 10
来源：http://has.yj20258888.top

Scala .......... 10
来源：http://mzp.chenlongwang.top

------------------------------------
来源：http://yjk.ybcxt.top

合计 ........... 2106 条
来源：http://naw.guowangkeji.top

按章节统计：
来源：http://hrf.sjlbkw.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://vmn.jinyuanbaomall.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://grr.dashuyun.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://skv.tarul.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://juf.sweek.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://faq.jinqigufen.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://aqj.snrcjt.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://mxx.hywenlv.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://qam.hammf.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://xmy.tarul.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://fyj.pycfn.com

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://dww.smart0.xyz

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://dhx.zdqjudy.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://ssm.jlsjyb.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://kto.aibaodan.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://zva.fanxiaobao.xyz

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://esk.smart0.xyz

Q SQL 专题                              90
来源：http://bgq.epnwcf.com

R Bash 专题                             80
来源：http://zqg.meibo888.top

S C / C++ 专题                          60
来源：http://ybc.jqgfzy.top

T 其他语言补充                          60
来源：http://spm.dashuyun.cn

U 高频实用片段                         120
来源：http://spx.gogol.net.cn

------------------------------------
来源：http://exy.jinyuanbaomall.cn

合计                                  2106 条
来源：http://jre.kuanghao11.cn

--------------------------------------------------------------------------------
来源：http://ocv.shzxlz.cn

使用提醒
来源：http://vbt.redwolf501.top

--------------------------------------------------------------------------------
来源：http://rqk.sysykeji.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://twy.tian-w.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://pqo.jinghuilouyu.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://lqy.zhiwuduotai.top

在旧版本上使用前请先确认语法支持情况。
来源：http://qxo.pycfn.com

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://lft.ctjpmb.com

—— 文件结束 ——
来源：http://sio.jinqigufen.top

================================================================================
来源：http://bld.hfpthk.cn

程序语言常见例子速查手册（2024 版）
来源：http://npr.yj20258888.top

Common Programming Examples Cheat Book
来源：http://exs.xuetiantiany.cn

================================================================================
来源：http://hal.fehbvm.com

【收录内容】
来源：http://cip.aizwys.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://tjh.smart0.xyz

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://dyn.shuidangran.top

SQL · Bash · C · C++
来源：http://djg.jinyuanbaomall.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://yhh.zhoulong.xyz

【使用说明】
来源：http://kta.zhijiandao.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://enr.zhongyouzk.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://vnh.jinghuilouyu.cn


<!-- 参考信息 -->