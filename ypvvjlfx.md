代发 wailian999

[U05] Py：列表去重且保序
来源：http://ivc.jiagoushi.top

list(dict.fromkeys(arr))
来源：http://aso.yuxming.cn

[U06] Py：合并两个字典
来源：http://boi.xuanzx.com

{**a, **b}
来源：http://aqb.yanxiufei.cn

[U07] Py：反转字典键值
来源：http://etf.hywenlv.cn

{v: k for k, v in d.items()}
来源：http://lxw.jqgufenzy.top

[U08] Py：展平二维列表
来源：http://wdj.fengsongda.top

[y for x in nested for y in x]
来源：http://yme.yj20258888.top

[U09] Py：字典取最大值的键
来源：http://nrs.tianlin.xyz

max(d, key=d.get)
来源：http://twa.ybcxt.top

[U10] Py：按值排序字典
来源：http://fwz.chenjidiqi.icu

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://pbg.fzhhl.top

[U11] Py：生成器表达式
来源：http://toh.vqdsnc.cn

(x * 2 for x in arr)
来源：http://tlr.yangfankeji.com

[U12] Py：取出现最多的 3 个元素
来源：http://esm.shanyushiyangkeji.top

Counter(arr).most_common(3)
来源：http://chw.xingfuxueyuan.xyz

[U13] Py：固定长度队列
来源：http://ukx.hysaishi.cn

deque(maxlen=10)
来源：http://oot.sxryk.cn

[U14] Py：分组收集到列表
来源：http://who.tian-w.cn

defaultdict(list)
来源：http://mky.yj202588.top

[U15] Py：高精度计时
来源：http://fzi.cqqwz.cn

t = time.perf_counter()
来源：http://ikb.guannengcc.top

[U16] Py：命令行参数解析
来源：http://eqm.shuidangran.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://tol.ywan-chungtsiang.top

[U17] Py：初始化日志
来源：http://fmt.jqgufenzy.top

logging.basicConfig(level=logging.INFO)
来源：http://zdc.yanxiufei.cn

[U18] Py：预编译正则
来源：http://enk.zhixingplan.top

pat = re.compile(r"\d+")
来源：http://bks.jlsjyb.cn

[U19] Py：正则替换带回调
来源：http://kpb.xuanzx.com

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://lxq.yonumen.top

[U20] Py：缓存函数结果
来源：http://pse.ppjwa.cn

@functools.lru_cache(maxsize=None)
来源：http://hda.feifeiyinyue.top

[U21] Py：自定义上下文管理器
来源：http://trg.9152youxi.cn

@contextlib.contextmanager
来源：http://ezo.yonumen.top

[U22] Py：矩阵转置
来源：http://xvc.zhoulong.xyz

list(zip(*m))
来源：http://wxg.meibo888.top

[U23] Py：分块读取大文件
来源：http://nse.svipenyu.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://acj.cucudq.cn

[U24] Py：路径操作
来源：http://wfi.jqgfzy.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://ceh.tanke756.top

[U25] Py：CSV 按字典读
来源：http://qed.fehbvm.com

csv.DictReader(f)
来源：http://lnk.shzxlz.cn

[U26] Py：并发下载
来源：http://cmv.ywan-chungtsiang.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://idp.ppjwa.cn

[U27] Py：异步 HTTP
来源：http://mzr.daria6918.cn

aiohttp.ClientSession() 配合 async with
来源：http://iir.nwbrower.top

[U28] Py：类型别名
来源：http://lkz.shanyushiyangtech.top

UserId = int
来源：http://ejp.pycfn.com

[U29] Py：属性校验
来源：http://wlo.bbcook.cn

@property 与 @x.setter 配合
来源：http://oyh.cheryme.top

[U30] Py：数据类
来源：http://ska.bjfxy.top

@dataclass(slots=True)
来源：http://eur.bjfxy.top

[U31] Py：单测
来源：http://ctp.ctjpmb.com

python -m pytest -q
来源：http://dns.ivvv.top

[U32] Py：代码格式化
来源：http://zch.zdqjudy.top

ruff format . && ruff check --fix .
来源：http://ecx.zdbjq.cn

[U33] Py：打包发布
来源：http://ivq.yj202588.top

python -m build  （依赖 pyproject.toml）
来源：http://dht.zhengqikj.top

[U34] Py：判断编码
来源：http://wpx.hongshengwenyu.top

chardet.detect(raw)
来源：http://lrn.gaohongyu789.top

[U35] Py：发送邮件
来源：http://vtw.hysaishi.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://sbq.hfpthk.cn

[U36] Py：定时任务
来源：http://rqk.sufxvd.cn

schedule.every(10).minutes.do(job)
来源：http://bju.smart0.xyz

[U37] Py：读写 Excel
来源：http://fls.jinqigfzy.top

pandas.read_excel / DataFrame.to_excel
来源：http://qax.jinyuanbaomall.cn

[U38] Py：获取脚本所在目录
来源：http://bqg.ppjwa.cn

Path(__file__).resolve().parent
来源：http://ytk.shanyushiyangkeji.top

[U39] Py：判断是否在交互环境
来源：http://osy.daxiang520.top

sys.stdout.isatty()
来源：http://xof.guowangkeji.top

[U40] Py：打印到标准错误
来源：http://pew.shzxlz.cn

print("err", file=sys.stderr)
来源：http://fyd.yfazqb.com

[U41] PHP：初始化 Composer 项目
来源：http://lgm.cdnleiting.top

composer init;  composer require guzzlehttp/guzzle
来源：http://zgd.hcnkem.com

[U42] PHP：PSR-4 自动加载
来源：http://kfp.zhoulong.xyz

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://lhk.pengpengdd.cyou

[U43] PHP：声明命名空间
来源：http://qam.iojbl.cn

namespace App\Http;
来源：http://xxz.yongpay.top

[U44] PHP：开启严格类型
来源：http://qyc.zhaomingkeji.xyz

declare(strict_types=1);
来源：http://qjs.yonumen.top

[U45] PHP：类型声明与返回类型
来源：http://czd.meibo888.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://pou.jinqigfzy.top

[U46] PHP：可空类型
来源：http://acq.yangfankeji.com

?string $name = null
来源：http://sfe.yj20258888.top

[U47] PHP：联合类型
来源：http://tfk.ydjk.org.cn

int|string $id
来源：http://pqu.hysaishi.cn

[U48] PHP：纯枚举
来源：http://vgs.yanxiufei.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://jxm.ivvv.top

[U49] PHP：只读属性
来源：http://usi.ywan-chungtsiang.top

public readonly string $name
来源：http://pzj.pycfn.com

[U50] PHP：构造器属性提升
来源：http://wmj.kuanghao11.cn

public function __construct(private int $id) {}
来源：http://sxt.chenzaomai.com

[U51] PHP：数组解构
来源：http://zvv.hysaishi.cn

[$a, $b] = $arr;
来源：http://jmi.zhijiandao.cn

[U52] PHP：箭头函数
来源：http://pvd.redwolf501.top

$double = fn($x) => $x * 2;
来源：http://ouj.sweek.top

[U53] PHP：空合并运算符
来源：http://hid.tarul.cn

$v = $a ?? $b ?? "default";
来源：http://dpu.bjfxy.top

[U54] PHP：空安全调用
来源：http://fpy.sxryk.cn

$obj?->method()
来源：http://kwu.daxiang520.top

[U55] PHP：match 表达式
来源：http://cjg.andypj.xyz

$s = match($x) { 1 => "一", default => "其他" };
来源：http://idp.jinqigfzy.top

[U56] PHP：命名参数
来源：http://tsj.uphjek.com

f(a: 1, b: 2)
来源：http://rhz.birdmap.top

[U57] PHP：字符串插值
来源：http://wra.jinyuanbaomall.cn

"值: {$a}"
来源：http://rsp.guannengcc.top

[U58] PHP：数组三件套
来源：http://jna.hnxiangtu.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://zvd.birdmap.top

[U59] PHP：自定义排序
来源：http://lqe.chenlongwang.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://bsw.sjlbkw.cn

[U60] PHP：JSON 编解码
来源：http://mwj.cdnleiting.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://azl.cashguo.top

[U61] PHP：正则
来源：http://oya.wangshuangyany.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://dlx.birdmap.top

[U62] PHP：日期对象
来源：http://qxg.nanxinkj.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://djb.ivvv.top

[U63] PHP：文件读写
来源：http://kha.smart0.xyz

file_get_contents($f);  file_put_contents($f, $data);
来源：http://lmr.zhengqikj.top

[U64] PHP：目录遍历
来源：http://dvz.bbcook.cn

glob("dir/*.php");  scandir("dir");
来源：http://vww.yj20258.top

[U65] PHP：会话
来源：http://kag.yvedp.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://qyf.52xcode.cn

[U66] PHP：设置 Cookie
来源：http://eca.chenjidiqi.icu

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://wjf.316326.xyz

[U67] PHP：处理文件上传
来源：http://jhy.shanyushiyangkeji.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://jpj.52xcode.cn

[U68] PHP：PDO 连接
来源：http://bku.hammf.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://jbz.xuanzx.com

[U69] PHP：PDO 预处理
来源：http://cpn.guowangkeji.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://uzf.cashguo.top

[U70] PHP：PDO 事务
来源：http://ffa.zhongyouzk.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://ecn.hnqzz.top

[U71] PHP：抛出异常
来源：http://thi.yuanzhike.top

throw new RuntimeException("失败", 500);
来源：http://rff.iojbl.cn

[U72] PHP：写错误日志
来源：http://qeo.ywan-chungtsiang.top

error_log("失败: " . $e->getMessage());
来源：http://abb.hesvh.cn

[U73] PHP：读取 ini 配置
来源：http://hke.zycfv.cn

parse_ini_file("config.ini", true)
来源：http://lzb.jiagoushi.top

[U74] PHP：读取环境变量
来源：http://mmu.zhiwuduotai.top

getenv("APP_ENV") ?: "production"
来源：http://jjw.xziqi.cn

[U75] PHP：依赖注入
来源：http://hqk.yanxiufei.cn

composer require psr/container
来源：http://aft.jianghu66.top

[U76] PHP：简单路由
来源：http://yqh.zhengqikj.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://hxd.zhijiandao.cn

[U77] PHP：模板渲染
来源：http://vqf.redwolf501.top

composer require twig/twig
来源：http://bfi.gotoacloud.top

[U78] PHP：单元测试
来源：http://sxx.nwbrower.top

composer require --dev phpunit/phpunit
来源：http://ump.jiagoushi.top

[U79] PHP：静态分析
来源：http://uvd.aibaodan.cn

composer require --dev phpstan/phpstan
来源：http://tel.ivvv.top

[U80] PHP：代码规范修复
来源：http://mue.pycfn.com

composer require --dev friendsofphp/php-cs-fixer
来源：http://irp.zhixingplan.top

[U81] JS：初始化项目
来源：http://yod.jinqigufen.top

npm init -y;  npm i express
来源：http://ifm.ppjwa.cn

[U82] JS：package.json 脚本
来源：http://tbm.sysykeji.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://ikr.ivvv.top

[U83] JS：ES Module 导入导出
来源：http://oql.nanxuanxn.top

export const a = 1;  import { a } from "./m.js";
来源：http://akc.jinqigfzy.top

[U84] JS：CommonJS 写法
来源：http://sda.ppjwa.cn

module.exports = { a };  const { a } = require("./m");
来源：http://wvb.xziqi.cn

[U85] JS：可选链
来源：http://gww.sysykeji.top

a?.b?.c
来源：http://jfb.zhengqikj.top

[U86] JS：空值合并
来源：http://pyz.guowangkeji.top

a ?? b
来源：http://mig.yuanzhike.top

[U87] JS：解构默认值
来源：http://hrf.bbcook.cn

const { a = 1, b = 2 } = obj;
来源：http://ejy.daria6918.cn

[U88] JS：对象展开合并
来源：http://scg.0kj1m.cn

{ ...a, ...b }
来源：http://tjz.ydzc1.top

[U89] JS：数组去重
来源：http://pwe.jianghu66.top

[...new Set(arr)]
来源：http://oyo.quarkkingdee.top

[U90] JS：数字数组排序
来源：http://jva.guannengcc.top

[...arr].sort((a, b) => a - b)
来源：http://sqe.ivvv.top

[U91] JS：对象键值遍历
来源：http://fqv.sxryk.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://rdl.aibaodan.cn

[U92] JS：深拷贝
来源：http://hzi.hywenlv.cn

structuredClone(obj)
来源：http://lxq.jqgfzy.top

[U93] JS：模板字符串
来源：http://rgg.shanyushiyangtech.top

`共 ${n} 条`
来源：http://orw.jinqigfzy.top

[U94] JS：箭头函数
来源：http://zfz.nwbrower.top

const double = x => x * 2;
来源：http://lvc.cheryme.top

[U95] JS：Promise 包装
来源：http://ble.mhx1999.top

new Promise((resolve, reject) => {})
来源：http://ucv.0kj1m.cn

[U96] JS：async/await 与异常
来源：http://skq.ivvv.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://vtg.zhaomingkeji.xyz

[U97] JS：并发请求
来源：http://atq.hfpthk.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://vei.xylfe.cn

[U98] JS：fetch 带 JSON
来源：http://vab.wangshuangyany.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://cyk.ctjpmb.com

[U99] JS：事件监听
来源：http://wrk.jinyuanbaomall.cn

el.addEventListener("click", e => {})
来源：http://alm.yonumen.top

[U100] JS：DOM 查询
来源：http://fvt.ppjwa.cn

document.querySelector(".item")
来源：http://ohk.xingfuxueyuan.xyz

[U101] JS：classList 操作
来源：http://nnh.52xcode.cn

el.classList.toggle("active")
来源：http://nvt.xuetiantiany.cn

[U102] JS：本地存储
来源：http://noc.jyoumei.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://bxt.feifeiyinyue.top

[U103] JS：定时器
来源：http://ett.vqdsnc.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://kbz.uphjek.com

[U104] JS：防抖
来源：http://dkk.yanxiufei.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://dvx.meibo888.top

[U105] JS：节流
来源：http://fhq.yj20258888.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://pnv.tarul.cn

[U106] JS：日期格式化
来源：http://ybl.jianghu66.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hdu.hesvh.cn

[U107] JS：数字千分位
来源：http://caa.jqgufenzy.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://atc.mhx1999.top

[U108] JS：随机整数
来源：http://mbq.yangfankeji.com

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://foa.jinyuanbaomall.cn

[U109] JS：数组分组
来源：http://msa.fktsv.cn

Object.groupBy(arr, x => x.type)
来源：http://jzd.fanxiaobao.xyz

[U110] JS：数组分块
来源：http://oqy.zhaomingkeji.xyz

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://fnu.cucudq.cn

[U111] JS：对象转 Map
来源：http://kuz.shangyingyoupin.top

new Map(Object.entries(obj))
来源：http://bdq.jinqigfzy.top

[U112] JS：字符串补位
来源：http://gun.tian-w.cn

"7".padStart(3, "0")
来源：http://tql.316326.xyz

[U113] JS：正则替换全部
来源：http://tdo.sxryk.cn

s.replaceAll("a", "b")
来源：http://eml.zhiwuduotai.top

[U114] JS：JSON 深比较
来源：http://oxw.tianlin.xyz

JSON.stringify(a) === JSON.stringify(b)
来源：http://tgx.chenzaomai.com

[U115] JS：生成 UUID
来源：http://edy.zycfv.cn

crypto.randomUUID()
来源：http://zio.guannengcc.top

[U116] JS：类型检查（JSDoc）
来源：http://jet.tarul.cn

/** @param {string} name */ function f(name) {}
来源：http://ojn.mhx1999.top

[U117] JS：单元测试
来源：http://fla.hywenlv.cn

npm i -D vitest;  npx vitest
来源：http://fou.zhijiandao.cn

[U118] JS：开发服务器
来源：http://zfh.jinyuanbaomall.cn

npm i -D vite;  npx vite
来源：http://axg.shzxlz.cn

[U119] JS：生产构建
来源：http://ude.jinyuanbaomall.cn

npx vite build
来源：http://aon.zdbjq.cn

[U120] JS：读取环境变量（Vite）
来源：http://tpt.hesvh.cn

import.meta.env.VITE_API_URL
来源：http://nhk.jqgfzy.top

================================================================================
来源：http://isr.quarkkingdee.top

统计汇总
来源：http://yvr.wangdashe.top

================================================================================
来源：http://koz.xingfuxueyuan.xyz

按语言统计（条）：
来源：http://eiz.ehwqpu.com

Python ......... 252
来源：http://inh.haohaochexian.top

PHP ............ 252
来源：http://fnz.jiagoushi.top

JavaScript ..... 252
来源：http://vva.epnwcf.com

TypeScript ..... 212
来源：http://jok.ydjk.org.cn

Java ........... 212
来源：http://rhs.jinqigufen.top

Go ............. 212
来源：http://npb.shanyushiyangkeji.top

Ruby ........... 212
来源：http://mzy.jinyuanbaomall.cn

C# ............. 212
来源：http://afa.zhoulong.xyz

C .............. 30
来源：http://qqu.hcnkem.com

C++ ............ 30
来源：http://vpx.shangyingyoupin.top

SQL ............ 90
来源：http://lcx.yj20258888.top

Bash ........... 80
来源：http://seq.nanxinkj.top

Kotlin ......... 15
来源：http://rjr.shzxlz.cn

Swift .......... 15
来源：http://csf.havefunace.top

Lua ............ 10
来源：http://dfj.bbcook.cn

Perl ........... 10
来源：http://vzg.zhengqikj.top

Scala .......... 10
来源：http://wbi.yvedp.cn

------------------------------------
来源：http://cha.guowangkeji.top

合计 ........... 2106 条
来源：http://zel.daria6918.cn

按章节统计：
来源：http://bqd.316326.xyz

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://tjv.feifeiyinyue.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://kjv.jinqigfzy.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://czm.fktsv.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://gfk.xylfe.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hsp.iojbl.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://otn.9152youxi.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://xuo.dashuyun.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://sjv.pycfn.com

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://rld.jinyuanbaomall.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://vbl.jiagoushi.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://bzv.yj20258888.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://egj.0kj1m.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://cqz.gzhubu.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://njx.dashuyun.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://vno.meibo888.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://gah.yuanzhike.top

Q SQL 专题                              90
来源：http://iae.fehbvm.com

R Bash 专题                             80
来源：http://jai.shangyingyoupin.top

S C / C++ 专题                          60
来源：http://cwb.xinyue.icu

T 其他语言补充                          60
来源：http://yto.shzxlz.cn

U 高频实用片段                         120
来源：http://yoy.316326.xyz

------------------------------------
来源：http://hur.snrcjt.cn

合计                                  2106 条
来源：http://lbb.hongshengwenyu.top

--------------------------------------------------------------------------------
来源：http://rdk.bjfxy.top

使用提醒
来源：http://xcv.52xcode.cn

--------------------------------------------------------------------------------
来源：http://ptu.zhongyouzk.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://bnx.pengpengdd.cyou

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://zlq.shzxlz.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://toz.jinghuilouyu.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://qla.guannengcc.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://fhp.mhx1999.top

—— 文件结束 ——
来源：http://fwx.c1oappe.top

================================================================================
来源：http://wlf.daria6918.cn

程序语言常见例子速查手册（2024 版）
来源：http://cci.cashguo.top

Common Programming Examples Cheat Book
来源：http://dqu.chenzaomai.com

================================================================================
来源：http://afi.ydzc1.top

【收录内容】
来源：http://ngc.aizwys.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://zdj.cdnleiting.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://zfo.gotoacloud.top

SQL · Bash · C · C++
来源：http://mfe.jqgfzy.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://qou.fengsongda.top

【使用说明】
来源：http://aix.havefunace.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://jhb.52xcode.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://cby.cheryme.top


<!-- 参考信息 -->