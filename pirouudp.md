代发 wailian999

[U05] Py：列表去重且保序
来源：http://vbx.xingfuxueyuan.xyz

list(dict.fromkeys(arr))
来源：http://gnr.shzxlz.cn

[U06] Py：合并两个字典
来源：http://yuz.yongpay.top

{**a, **b}
来源：http://ips.tianlin.xyz

[U07] Py：反转字典键值
来源：http://zch.yanxiufei.cn

{v: k for k, v in d.items()}
来源：http://xdl.jqgufenzy.top

[U08] Py：展平二维列表
来源：http://eev.zycfv.cn

[y for x in nested for y in x]
来源：http://jsu.dianchejie.cn

[U09] Py：字典取最大值的键
来源：http://tkn.guowangkeji.top

max(d, key=d.get)
来源：http://nzk.jlsjyb.cn

[U10] Py：按值排序字典
来源：http://onj.cqqwz.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://edb.ydzc1.top

[U11] Py：生成器表达式
来源：http://ofq.xinyue.icu

(x * 2 for x in arr)
来源：http://aim.vqdsnc.cn

[U12] Py：取出现最多的 3 个元素
来源：http://jsn.andypj.xyz

Counter(arr).most_common(3)
来源：http://vqn.daria6918.cn

[U13] Py：固定长度队列
来源：http://gtf.c1oappe.top

deque(maxlen=10)
来源：http://iqq.52xcode.cn

[U14] Py：分组收集到列表
来源：http://dso.zhongyouzk.top

defaultdict(list)
来源：http://mrd.sxryk.cn

[U15] Py：高精度计时
来源：http://kpx.zdbjq.cn

t = time.perf_counter()
来源：http://wfk.shanyushiyangtech.top

[U16] Py：命令行参数解析
来源：http://dfb.yangfankeji.com

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://yiw.xylfe.cn

[U17] Py：初始化日志
来源：http://bjy.hesvh.cn

logging.basicConfig(level=logging.INFO)
来源：http://dxh.zhongyouzk.top

[U18] Py：预编译正则
来源：http://wlu.chenzaomai.com

pat = re.compile(r"\d+")
来源：http://rrm.haohaochexian.top

[U19] Py：正则替换带回调
来源：http://mhb.xuanzx.com

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://ljz.zhixingplan.top

[U20] Py：缓存函数结果
来源：http://ljn.vqdsnc.cn

@functools.lru_cache(maxsize=None)
来源：http://yuu.yonumen.top

[U21] Py：自定义上下文管理器
来源：http://nmg.yuanzhike.top

@contextlib.contextmanager
来源：http://jlw.gotoacloud.top

[U22] Py：矩阵转置
来源：http://ikg.hywenlv.cn

list(zip(*m))
来源：http://gbw.hysaishi.cn

[U23] Py：分块读取大文件
来源：http://pkr.snrcjt.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://bwx.aibaodan.cn

[U24] Py：路径操作
来源：http://emi.yfazqb.com

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://chb.dashuyun.cn

[U25] Py：CSV 按字典读
来源：http://sdn.cheryme.top

csv.DictReader(f)
来源：http://ztn.gaohongyu789.top

[U26] Py：并发下载
来源：http://cnm.zycfv.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://ofo.aibaodan.cn

[U27] Py：异步 HTTP
来源：http://wef.svipenyu.cn

aiohttp.ClientSession() 配合 async with
来源：http://qqk.uphjek.com

[U28] Py：类型别名
来源：http://ozx.316326.xyz

UserId = int
来源：http://wvi.yvedp.cn

[U29] Py：属性校验
来源：http://ddg.ywan-chungtsiang.top

@property 与 @x.setter 配合
来源：http://xgh.yj202588.top

[U30] Py：数据类
来源：http://nkp.fktsv.cn

@dataclass(slots=True)
来源：http://mkh.xziqi.cn

[U31] Py：单测
来源：http://ivt.pycfn.com

python -m pytest -q
来源：http://upz.fktsv.cn

[U32] Py：代码格式化
来源：http://bqj.nwbrower.top

ruff format . && ruff check --fix .
来源：http://yet.yfazqb.com

[U33] Py：打包发布
来源：http://woq.cashguo.top

python -m build  （依赖 pyproject.toml）
来源：http://wtr.bjfxy.top

[U34] Py：判断编码
来源：http://wmp.dianchejie.cn

chardet.detect(raw)
来源：http://arl.jinyuanbaomall.cn

[U35] Py：发送邮件
来源：http://jyz.shzxlz.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://ots.zhoulong.xyz

[U36] Py：定时任务
来源：http://vvu.chenjidiqi.icu

schedule.every(10).minutes.do(job)
来源：http://mpx.snrcjt.cn

[U37] Py：读写 Excel
来源：http://ixo.sxryk.cn

pandas.read_excel / DataFrame.to_excel
来源：http://ixd.bbcook.cn

[U38] Py：获取脚本所在目录
来源：http://tej.jlsjyb.cn

Path(__file__).resolve().parent
来源：http://apl.meibo888.top

[U39] Py：判断是否在交互环境
来源：http://asn.vehdjk.com

sys.stdout.isatty()
来源：http://dbu.cashguo.top

[U40] Py：打印到标准错误
来源：http://bqd.mhx1999.top

print("err", file=sys.stderr)
来源：http://ifh.jqgufenzy.top

[U41] PHP：初始化 Composer 项目
来源：http://uxt.gzhubu.top

composer init;  composer require guzzlehttp/guzzle
来源：http://mpi.vqdsnc.cn

[U42] PHP：PSR-4 自动加载
来源：http://jcu.ydzc1.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://mbo.hongshengwenyu.top

[U43] PHP：声明命名空间
来源：http://ldx.chenjidiqi.icu

namespace App\Http;
来源：http://mzs.chenzaomai.com

[U44] PHP：开启严格类型
来源：http://vpc.zhaomingkeji.xyz

declare(strict_types=1);
来源：http://blw.fehbvm.com

[U45] PHP：类型声明与返回类型
来源：http://tqf.cdnleiting.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://wut.hnqzz.top

[U46] PHP：可空类型
来源：http://cke.ehwqpu.com

?string $name = null
来源：http://rlg.zhiwuduotai.top

[U47] PHP：联合类型
来源：http://pfe.zhoulong.xyz

int|string $id
来源：http://xmi.jqgufenzy.top

[U48] PHP：纯枚举
来源：http://epg.jqgfzy.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://xmj.shangyingyoupin.top

[U49] PHP：只读属性
来源：http://rms.epnwcf.com

public readonly string $name
来源：http://jde.zdqjudy.top

[U50] PHP：构造器属性提升
来源：http://iaw.gaohongyu789.top

public function __construct(private int $id) {}
来源：http://iir.chenjidiqi.icu

[U51] PHP：数组解构
来源：http://xep.xuetiantiany.cn

[$a, $b] = $arr;
来源：http://paw.yvedp.cn

[U52] PHP：箭头函数
来源：http://tkx.yfazqb.com

$double = fn($x) => $x * 2;
来源：http://awl.zhengqikj.top

[U53] PHP：空合并运算符
来源：http://npu.kuanghao11.cn

$v = $a ?? $b ?? "default";
来源：http://vnq.hongshengwenyu.top

[U54] PHP：空安全调用
来源：http://rxl.yueranfly.top

$obj?->method()
来源：http://tih.yj202588.top

[U55] PHP：match 表达式
来源：http://bdd.jinqigfzy.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://siv.kuanghao11.cn

[U56] PHP：命名参数
来源：http://adm.yangfankeji.com

f(a: 1, b: 2)
来源：http://ooq.hnxiangtu.top

[U57] PHP：字符串插值
来源：http://szc.dianchejie.cn

"值: {$a}"
来源：http://chm.zhaomingkeji.xyz

[U58] PHP：数组三件套
来源：http://ibj.hywenlv.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://jll.9152youxi.cn

[U59] PHP：自定义排序
来源：http://vpo.xziqi.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://vxo.daxiang520.top

[U60] PHP：JSON 编解码
来源：http://abr.sweek.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://jhe.yfazqb.com

[U61] PHP：正则
来源：http://pwt.snrcjt.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://cfb.sufxvd.cn

[U62] PHP：日期对象
来源：http://irh.ybcxt.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://mkl.fzhhl.top

[U63] PHP：文件读写
来源：http://hcy.vehdjk.com

file_get_contents($f);  file_put_contents($f, $data);
来源：http://mtr.ywan-chungtsiang.top

[U64] PHP：目录遍历
来源：http://kcd.9152youxi.cn

glob("dir/*.php");  scandir("dir");
来源：http://abk.hnqzz.top

[U65] PHP：会话
来源：http://vfc.ydzc1.top

session_start();  $_SESSION["uid"] = 1;
来源：http://pag.chenlongwang.top

[U66] PHP：设置 Cookie
来源：http://faa.yanxiufei.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://okp.wangshuangyany.cn

[U67] PHP：处理文件上传
来源：http://yrm.ybcxt.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://dxq.shzxlz.cn

[U68] PHP：PDO 连接
来源：http://ooo.jyoumei.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://moe.bjfxy.top

[U69] PHP：PDO 预处理
来源：http://pql.fehbvm.com

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://wfs.dashuyun.cn

[U70] PHP：PDO 事务
来源：http://ris.tarul.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://jff.daxiang520.top

[U71] PHP：抛出异常
来源：http://ycd.daxiang520.top

throw new RuntimeException("失败", 500);
来源：http://oxw.kuanghao11.cn

[U72] PHP：写错误日志
来源：http://juv.yj20258.top

error_log("失败: " . $e->getMessage());
来源：http://yhz.yvedp.cn

[U73] PHP：读取 ini 配置
来源：http://qjq.jqgfzy.top

parse_ini_file("config.ini", true)
来源：http://lol.xziqi.cn

[U74] PHP：读取环境变量
来源：http://xli.gotoacloud.top

getenv("APP_ENV") ?: "production"
来源：http://dcq.ppjwa.cn

[U75] PHP：依赖注入
来源：http://buk.hywenlv.cn

composer require psr/container
来源：http://emq.zycfv.cn

[U76] PHP：简单路由
来源：http://lwp.hammf.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://mxr.mhx1999.top

[U77] PHP：模板渲染
来源：http://wwq.pycfn.com

composer require twig/twig
来源：http://igv.cashguo.top

[U78] PHP：单元测试
来源：http://wez.zdqjudy.top

composer require --dev phpunit/phpunit
来源：http://xbf.bjfxy.top

[U79] PHP：静态分析
来源：http://pbb.sufxvd.cn

composer require --dev phpstan/phpstan
来源：http://tow.iojbl.cn

[U80] PHP：代码规范修复
来源：http://cqv.andypj.xyz

composer require --dev friendsofphp/php-cs-fixer
来源：http://hjq.jinyuanbaomall.cn

[U81] JS：初始化项目
来源：http://pxx.yj202588.top

npm init -y;  npm i express
来源：http://kks.feifeiyinyue.top

[U82] JS：package.json 脚本
来源：http://dnk.xuanzx.com

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://aef.zhoulong.xyz

[U83] JS：ES Module 导入导出
来源：http://gao.yj202588.top

export const a = 1;  import { a } from "./m.js";
来源：http://yrx.yj202588.top

[U84] JS：CommonJS 写法
来源：http://hmz.cheryme.top

module.exports = { a };  const { a } = require("./m");
来源：http://oho.wangshuangyany.cn

[U85] JS：可选链
来源：http://hsi.52xcode.cn

a?.b?.c
来源：http://rda.haohaochexian.top

[U86] JS：空值合并
来源：http://hhl.gaohongyu789.top

a ?? b
来源：http://ddv.jinyuanbaomall.cn

[U87] JS：解构默认值
来源：http://yiv.havefunace.top

const { a = 1, b = 2 } = obj;
来源：http://vuj.jyoumei.cn

[U88] JS：对象展开合并
来源：http://yzq.havefunace.top

{ ...a, ...b }
来源：http://quy.9152youxi.cn

[U89] JS：数组去重
来源：http://xdw.svipenyu.cn

[...new Set(arr)]
来源：http://kez.cqqwz.cn

[U90] JS：数字数组排序
来源：http://wnr.feifeiyinyue.top

[...arr].sort((a, b) => a - b)
来源：http://eee.guowangkeji.top

[U91] JS：对象键值遍历
来源：http://dmw.jqgfzy.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://yxu.gotoacloud.top

[U92] JS：深拷贝
来源：http://lal.nwbrower.top

structuredClone(obj)
来源：http://lvo.52xcode.cn

[U93] JS：模板字符串
来源：http://vzz.snrcjt.cn

`共 ${n} 条`
来源：http://wzu.nanxuanxn.top

[U94] JS：箭头函数
来源：http://zju.iojbl.cn

const double = x => x * 2;
来源：http://fll.fehbvm.com

[U95] JS：Promise 包装
来源：http://yva.jinghuilouyu.cn

new Promise((resolve, reject) => {})
来源：http://rlr.guannengcc.top

[U96] JS：async/await 与异常
来源：http://onj.zhiwuduotai.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hzr.shanyushiyangtech.top

[U97] JS：并发请求
来源：http://qim.chenlongwang.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://vme.jinghuilouyu.cn

[U98] JS：fetch 带 JSON
来源：http://arl.cheryme.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hus.shuidangran.top

[U99] JS：事件监听
来源：http://jiz.nanxuanxn.top

el.addEventListener("click", e => {})
来源：http://mpj.zdqjudy.top

[U100] JS：DOM 查询
来源：http://gjk.yongpay.top

document.querySelector(".item")
来源：http://xlv.shanyushiyangtech.top

[U101] JS：classList 操作
来源：http://wqn.aibaodan.cn

el.classList.toggle("active")
来源：http://plo.hfpthk.cn

[U102] JS：本地存储
来源：http://bqh.yfazqb.com

localStorage.setItem("k", JSON.stringify(v))
来源：http://wol.cheryme.top

[U103] JS：定时器
来源：http://nim.xylfe.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://dsv.havefunace.top

[U104] JS：防抖
来源：http://tzy.mhx1999.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ymh.chenzaomai.com

[U105] JS：节流
来源：http://cml.hesvh.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://yyz.birdmap.top

[U106] JS：日期格式化
来源：http://fen.dianchejie.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://ojv.jiagoushi.top

[U107] JS：数字千分位
来源：http://rjd.hfpthk.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://mly.xinyue.icu

[U108] JS：随机整数
来源：http://zip.uphjek.com

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://fnk.jlsjyb.cn

[U109] JS：数组分组
来源：http://sqa.yj20258.top

Object.groupBy(arr, x => x.type)
来源：http://olx.ywan-chungtsiang.top

[U110] JS：数组分块
来源：http://ojd.fengsongda.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://qaw.kuanghao11.cn

[U111] JS：对象转 Map
来源：http://uqi.xuetiantiany.cn

new Map(Object.entries(obj))
来源：http://ccb.ivvv.top

[U112] JS：字符串补位
来源：http://chj.zhixingplan.top

"7".padStart(3, "0")
来源：http://zan.tarul.cn

[U113] JS：正则替换全部
来源：http://dfk.aibaodan.cn

s.replaceAll("a", "b")
来源：http://kew.hesvh.cn

[U114] JS：JSON 深比较
来源：http://vtb.hysaishi.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://tkf.ehwqpu.com

[U115] JS：生成 UUID
来源：http://mum.bbcook.cn

crypto.randomUUID()
来源：http://art.c1oappe.top

[U116] JS：类型检查（JSDoc）
来源：http://icb.aibaodan.cn

/** @param {string} name */ function f(name) {}
来源：http://vxr.feifeiyinyue.top

[U117] JS：单元测试
来源：http://obb.zhaomingkeji.xyz

npm i -D vitest;  npx vitest
来源：http://zby.xuanzx.com

[U118] JS：开发服务器
来源：http://qrj.birdmap.top

npm i -D vite;  npx vite
来源：http://kpd.bjfxy.top

[U119] JS：生产构建
来源：http://gfj.ivvv.top

npx vite build
来源：http://hms.zycfv.cn

[U120] JS：读取环境变量（Vite）
来源：http://wkl.wangshuangyany.cn

import.meta.env.VITE_API_URL
来源：http://rzu.feifeiyinyue.top

================================================================================
来源：http://brd.sjlbkw.cn

统计汇总
来源：http://zbg.jinqigfzy.top

================================================================================
来源：http://eod.meibo888.top

按语言统计（条）：
来源：http://jdc.nwbrower.top

Python ......... 252
来源：http://dfr.havefunace.top

PHP ............ 252
来源：http://tsn.52xcode.cn

JavaScript ..... 252
来源：http://nwd.gogol.net.cn

TypeScript ..... 212
来源：http://wlv.shanyushiyangkeji.top

Java ........... 212
来源：http://atu.ywan-chungtsiang.top

Go ............. 212
来源：http://dcx.yueranfly.top

Ruby ........... 212
来源：http://nxt.shangyingyoupin.top

C# ............. 212
来源：http://uyo.guowangkeji.top

C .............. 30
来源：http://glg.ybcxt.top

C++ ............ 30
来源：http://dfq.xylfe.cn

SQL ............ 90
来源：http://amw.zhengqikj.top

Bash ........... 80
来源：http://rlc.ydzc1.top

Kotlin ......... 15
来源：http://cdq.smart0.xyz

Swift .......... 15
来源：http://dhf.uphjek.com

Lua ............ 10
来源：http://pzz.tanke756.top

Perl ........... 10
来源：http://hrk.sufxvd.cn

Scala .......... 10
来源：http://rod.hfpthk.cn

------------------------------------
来源：http://wfn.gogol.net.cn

合计 ........... 2106 条
来源：http://dnp.cdnleiting.top

按章节统计：
来源：http://nbk.shanyushiyangkeji.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://lay.yuanzhike.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://ovp.hnxiangtu.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://egt.uphjek.com

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://lje.nanxuanxn.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://ucn.haohaochexian.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://jhe.52xcode.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://lmv.jinqigfzy.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://fgi.smart0.xyz

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://cbb.shuidangran.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://hsl.yj202588.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://zjv.daxiang520.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://gnh.cheryme.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://dub.mhx1999.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://mvj.jinghuilouyu.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://anr.sufxvd.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://rny.daria6918.cn

Q SQL 专题                              90
来源：http://qoq.ydzc1.top

R Bash 专题                             80
来源：http://fdu.chenzaomai.com

S C / C++ 专题                          60
来源：http://meg.9152youxi.cn

T 其他语言补充                          60
来源：http://rli.yonumen.top

U 高频实用片段                         120
来源：http://fra.sweek.top

------------------------------------
来源：http://wni.snrcjt.cn

合计                                  2106 条
来源：http://gch.sweek.top

--------------------------------------------------------------------------------
来源：http://hok.zhixingplan.top

使用提醒
来源：http://usv.cqqwz.cn

--------------------------------------------------------------------------------
来源：http://ect.cashguo.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://ody.hywenlv.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://bjg.yvedp.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://dxu.yfazqb.com

在旧版本上使用前请先确认语法支持情况。
来源：http://mlj.xuetiantiany.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://vdj.gogol.net.cn

—— 文件结束 ——
来源：http://ict.guowangkeji.top

================================================================================
来源：http://pfh.birdmap.top

程序语言常见例子速查手册（2024 版）
来源：http://ich.gogol.net.cn

Common Programming Examples Cheat Book
来源：http://czk.yuxming.cn

================================================================================
来源：http://zoh.pycfn.com

【收录内容】
来源：http://jil.fzhhl.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://dpn.shanyushiyangkeji.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://kav.vqdsnc.cn

SQL · Bash · C · C++
来源：http://gal.c1oappe.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://txq.zhongyouzk.top

【使用说明】
来源：http://btp.zhijiandao.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://ubu.meibo888.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://wct.yj202588.top


<!-- 参考信息 -->