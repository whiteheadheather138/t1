代发 wailian999

[U07] Py：反转字典键值
来源：http://xvu.gaohongyu789.top

{v: k for k, v in d.items()}
来源：http://tys.daxiang520.top

[U08] Py：展平二维列表
来源：http://bsb.shanyushiyangkeji.top

[y for x in nested for y in x]
来源：http://olf.cdnleiting.top

[U09] Py：字典取最大值的键
来源：http://pbo.havefunace.top

max(d, key=d.get)
来源：http://vhz.andypj.xyz

[U10] Py：按值排序字典
来源：http://fqr.jinghuilouyu.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://ukh.jinghuilouyu.cn

[U11] Py：生成器表达式
来源：http://iow.sxryk.cn

(x * 2 for x in arr)
来源：http://hcm.jiagoushi.top

[U12] Py：取出现最多的 3 个元素
来源：http://khh.haohaochexian.top

Counter(arr).most_common(3)
来源：http://wts.svipenyu.cn

[U13] Py：固定长度队列
来源：http://hrg.gotoacloud.top

deque(maxlen=10)
来源：http://txr.zhaomingkeji.xyz

[U14] Py：分组收集到列表
来源：http://heu.yongpay.top

defaultdict(list)
来源：http://mvg.zdbjq.cn

[U15] Py：高精度计时
来源：http://bub.zhaomingkeji.xyz

t = time.perf_counter()
来源：http://mka.pengpengdd.cyou

[U16] Py：命令行参数解析
来源：http://csh.vqdsnc.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://vwz.nanxuanxn.top

[U17] Py：初始化日志
来源：http://kzl.daxiang520.top

logging.basicConfig(level=logging.INFO)
来源：http://tzj.yvedp.cn

[U18] Py：预编译正则
来源：http://wkh.tarul.cn

pat = re.compile(r"\d+")
来源：http://wgm.fehbvm.com

[U19] Py：正则替换带回调
来源：http://cdp.shangyingyoupin.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://fss.fengsongda.top

[U20] Py：缓存函数结果
来源：http://lza.ivvv.top

@functools.lru_cache(maxsize=None)
来源：http://bek.bbcook.cn

[U21] Py：自定义上下文管理器
来源：http://obb.guannengcc.top

@contextlib.contextmanager
来源：http://zra.andypj.xyz

[U22] Py：矩阵转置
来源：http://kgv.tarul.cn

list(zip(*m))
来源：http://vhs.ivvv.top

[U23] Py：分块读取大文件
来源：http://jas.jlsjyb.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://bic.bbcook.cn

[U24] Py：路径操作
来源：http://glc.zhoulong.xyz

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://zoo.birdmap.top

[U25] Py：CSV 按字典读
来源：http://xnm.fehbvm.com

csv.DictReader(f)
来源：http://bpu.chenjidiqi.icu

[U26] Py：并发下载
来源：http://odk.nanxuanxn.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://euc.9152youxi.cn

[U27] Py：异步 HTTP
来源：http://itr.feifeiyinyue.top

aiohttp.ClientSession() 配合 async with
来源：http://ryv.vehdjk.com

[U28] Py：类型别名
来源：http://whc.hywenlv.cn

UserId = int
来源：http://nak.ctjpmb.com

[U29] Py：属性校验
来源：http://fry.dashuyun.cn

@property 与 @x.setter 配合
来源：http://pxj.snrcjt.cn

[U30] Py：数据类
来源：http://mtg.yj202588.top

@dataclass(slots=True)
来源：http://awx.jinyuanbaomall.cn

[U31] Py：单测
来源：http://jfy.zdbjq.cn

python -m pytest -q
来源：http://jiq.fehbvm.com

[U32] Py：代码格式化
来源：http://hvu.uphjek.com

ruff format . && ruff check --fix .
来源：http://dai.tanke756.top

[U33] Py：打包发布
来源：http://tgc.jinyuanbaomall.cn

python -m build  （依赖 pyproject.toml）
来源：http://zfd.hcnkem.com

[U34] Py：判断编码
来源：http://fsm.chenlongwang.top

chardet.detect(raw)
来源：http://pym.yanxiufei.cn

[U35] Py：发送邮件
来源：http://eqi.jqgufenzy.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://svv.ydjk.org.cn

[U36] Py：定时任务
来源：http://wbh.zhijiandao.cn

schedule.every(10).minutes.do(job)
来源：http://ayi.andypj.xyz

[U37] Py：读写 Excel
来源：http://lpx.sufxvd.cn

pandas.read_excel / DataFrame.to_excel
来源：http://fcv.sjlbkw.cn

[U38] Py：获取脚本所在目录
来源：http://bwc.dashuyun.cn

Path(__file__).resolve().parent
来源：http://xbf.52xcode.cn

[U39] Py：判断是否在交互环境
来源：http://dvq.jyoumei.cn

sys.stdout.isatty()
来源：http://jwe.hywenlv.cn

[U40] Py：打印到标准错误
来源：http://afx.feifeiyinyue.top

print("err", file=sys.stderr)
来源：http://dyz.tarul.cn

[U41] PHP：初始化 Composer 项目
来源：http://zlb.hnqzz.top

composer init;  composer require guzzlehttp/guzzle
来源：http://gcf.jinqigfzy.top

[U42] PHP：PSR-4 自动加载
来源：http://loe.shuidangran.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://gct.zdqjudy.top

[U43] PHP：声明命名空间
来源：http://smi.cqqwz.cn

namespace App\Http;
来源：http://yki.nwbrower.top

[U44] PHP：开启严格类型
来源：http://cqp.xingfuxueyuan.xyz

declare(strict_types=1);
来源：http://hoc.aibaodan.cn

[U45] PHP：类型声明与返回类型
来源：http://uxg.wangdashe.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://bcj.hnqzz.top

[U46] PHP：可空类型
来源：http://zco.fzhhl.top

?string $name = null
来源：http://pig.bjfxy.top

[U47] PHP：联合类型
来源：http://vqe.52xcode.cn

int|string $id
来源：http://xzd.jinqigufen.top

[U48] PHP：纯枚举
来源：http://wzu.nanxuanxn.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://bgo.sjlbkw.cn

[U49] PHP：只读属性
来源：http://svp.bbcook.cn

public readonly string $name
来源：http://kfh.shanyushiyangkeji.top

[U50] PHP：构造器属性提升
来源：http://rbg.pengpengdd.cyou

public function __construct(private int $id) {}
来源：http://jzc.sysykeji.top

[U51] PHP：数组解构
来源：http://frv.mhx1999.top

[$a, $b] = $arr;
来源：http://roq.yuxming.cn

[U52] PHP：箭头函数
来源：http://ygn.shzxlz.cn

$double = fn($x) => $x * 2;
来源：http://fdd.cucudq.cn

[U53] PHP：空合并运算符
来源：http://ojt.xingfuxueyuan.xyz

$v = $a ?? $b ?? "default";
来源：http://ywg.cucudq.cn

[U54] PHP：空安全调用
来源：http://yfa.epnwcf.com

$obj?->method()
来源：http://kqo.bjfxy.top

[U55] PHP：match 表达式
来源：http://xrq.jinqigufen.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://uiv.dashuyun.cn

[U56] PHP：命名参数
来源：http://tps.gogol.net.cn

f(a: 1, b: 2)
来源：http://kam.ppjwa.cn

[U57] PHP：字符串插值
来源：http://app.tarul.cn

"值: {$a}"
来源：http://cys.snrcjt.cn

[U58] PHP：数组三件套
来源：http://qxe.jinqigufen.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://gkg.sysykeji.top

[U59] PHP：自定义排序
来源：http://esb.yueranfly.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://phc.hongshengwenyu.top

[U60] PHP：JSON 编解码
来源：http://cdp.316326.xyz

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://vug.birdmap.top

[U61] PHP：正则
来源：http://aim.yj202588.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://pfs.havefunace.top

[U62] PHP：日期对象
来源：http://bwz.wangshuangyany.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://pcn.nanxuanxn.top

[U63] PHP：文件读写
来源：http://egd.wangdashe.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://dsu.aibaodan.cn

[U64] PHP：目录遍历
来源：http://kjd.yuxming.cn

glob("dir/*.php");  scandir("dir");
来源：http://ivy.xuetiantiany.cn

[U65] PHP：会话
来源：http://yxi.hywenlv.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://wfk.gaohongyu789.top

[U66] PHP：设置 Cookie
来源：http://qot.fanxiaobao.xyz

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://jqt.hnqzz.top

[U67] PHP：处理文件上传
来源：http://chj.zhengqikj.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://htl.yonumen.top

[U68] PHP：PDO 连接
来源：http://pyg.bjfxy.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://tav.ydzc1.top

[U69] PHP：PDO 预处理
来源：http://qav.xziqi.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://vds.zdqjudy.top

[U70] PHP：PDO 事务
来源：http://tpx.shzxlz.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://dmw.svipenyu.cn

[U71] PHP：抛出异常
来源：http://xrh.shzxlz.cn

throw new RuntimeException("失败", 500);
来源：http://otl.svipenyu.cn

[U72] PHP：写错误日志
来源：http://sep.jyoumei.cn

error_log("失败: " . $e->getMessage());
来源：http://kxi.aizwys.cn

[U73] PHP：读取 ini 配置
来源：http://pby.xuanzx.com

parse_ini_file("config.ini", true)
来源：http://uqi.tianlin.xyz

[U74] PHP：读取环境变量
来源：http://gil.sweek.top

getenv("APP_ENV") ?: "production"
来源：http://jrh.tarul.cn

[U75] PHP：依赖注入
来源：http://lcl.316326.xyz

composer require psr/container
来源：http://nxh.jlsjyb.cn

[U76] PHP：简单路由
来源：http://hru.gaohongyu789.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://qbl.quarkkingdee.top

[U77] PHP：模板渲染
来源：http://lmb.mhx1999.top

composer require twig/twig
来源：http://tgw.nwbrower.top

[U78] PHP：单元测试
来源：http://zin.0kj1m.cn

composer require --dev phpunit/phpunit
来源：http://yvn.zycfv.cn

[U79] PHP：静态分析
来源：http://wdr.birdmap.top

composer require --dev phpstan/phpstan
来源：http://kow.meibo888.top

[U80] PHP：代码规范修复
来源：http://ors.shanyushiyangkeji.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://sst.hammf.cn

[U81] JS：初始化项目
来源：http://bhz.shanyushiyangkeji.top

npm init -y;  npm i express
来源：http://hoq.andypj.xyz

[U82] JS：package.json 脚本
来源：http://eeh.tian-w.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://cye.fktsv.cn

[U83] JS：ES Module 导入导出
来源：http://las.jlsjyb.cn

export const a = 1;  import { a } from "./m.js";
来源：http://kul.zhixingplan.top

[U84] JS：CommonJS 写法
来源：http://api.yongpay.top

module.exports = { a };  const { a } = require("./m");
来源：http://kjg.bbcook.cn

[U85] JS：可选链
来源：http://sku.meibo888.top

a?.b?.c
来源：http://dxr.bjfxy.top

[U86] JS：空值合并
来源：http://lhj.jqgfzy.top

a ?? b
来源：http://ilr.yangfankeji.com

[U87] JS：解构默认值
来源：http://qjm.hnqzz.top

const { a = 1, b = 2 } = obj;
来源：http://nak.zhaomingkeji.xyz

[U88] JS：对象展开合并
来源：http://jby.feifeiyinyue.top

{ ...a, ...b }
来源：http://nvt.xuanzx.com

[U89] JS：数组去重
来源：http://ytn.nanxuanxn.top

[...new Set(arr)]
来源：http://fae.zhiwuduotai.top

[U90] JS：数字数组排序
来源：http://fpv.jinqigufen.top

[...arr].sort((a, b) => a - b)
来源：http://dkp.yvedp.cn

[U91] JS：对象键值遍历
来源：http://fux.nanxuanxn.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://dkm.vqdsnc.cn

[U92] JS：深拷贝
来源：http://syk.c1oappe.top

structuredClone(obj)
来源：http://kwb.yongpay.top

[U93] JS：模板字符串
来源：http://nnm.pengpengdd.cyou

`共 ${n} 条`
来源：http://jxv.fengsongda.top

[U94] JS：箭头函数
来源：http://pxf.daria6918.cn

const double = x => x * 2;
来源：http://mif.wangdashe.top

[U95] JS：Promise 包装
来源：http://oof.aibaodan.cn

new Promise((resolve, reject) => {})
来源：http://ppb.jqgufenzy.top

[U96] JS：async/await 与异常
来源：http://xhr.dianchejie.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://gac.xuanzx.com

[U97] JS：并发请求
来源：http://auw.c1oappe.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://zrp.hysaishi.cn

[U98] JS：fetch 带 JSON
来源：http://lmn.haohaochexian.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://ybl.nanxuanxn.top

[U99] JS：事件监听
来源：http://vmp.chenlongwang.top

el.addEventListener("click", e => {})
来源：http://qlv.yj202588.top

[U100] JS：DOM 查询
来源：http://mee.yfazqb.com

document.querySelector(".item")
来源：http://gzj.ehwqpu.com

[U101] JS：classList 操作
来源：http://jtr.kuanghao11.cn

el.classList.toggle("active")
来源：http://nel.vqdsnc.cn

[U102] JS：本地存储
来源：http://fht.fehbvm.com

localStorage.setItem("k", JSON.stringify(v))
来源：http://ycf.gogol.net.cn

[U103] JS：定时器
来源：http://ojy.yfazqb.com

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://bnn.yj202588.top

[U104] JS：防抖
来源：http://heh.zdqjudy.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hro.wangshuangyany.cn

[U105] JS：节流
来源：http://yoe.andypj.xyz

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://bwz.jinqigufen.top

[U106] JS：日期格式化
来源：http://gsu.chenlongwang.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://kep.zhaomingkeji.xyz

[U107] JS：数字千分位
来源：http://nsf.yvedp.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://lhb.yangfankeji.com

[U108] JS：随机整数
来源：http://uyk.wangdashe.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://swz.wangdashe.top

[U109] JS：数组分组
来源：http://twf.c1oappe.top

Object.groupBy(arr, x => x.type)
来源：http://sru.pengpengdd.cyou

[U110] JS：数组分块
来源：http://yev.jiagoushi.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://zat.tarul.cn

[U111] JS：对象转 Map
来源：http://din.aibaodan.cn

new Map(Object.entries(obj))
来源：http://pfr.yj20258.top

[U112] JS：字符串补位
来源：http://vej.jinqigufen.top

"7".padStart(3, "0")
来源：http://hci.gaohongyu789.top

[U113] JS：正则替换全部
来源：http://kod.bbcook.cn

s.replaceAll("a", "b")
来源：http://nne.xuanzx.com

[U114] JS：JSON 深比较
来源：http://rav.hongshengwenyu.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://btm.fengsongda.top

[U115] JS：生成 UUID
来源：http://ksj.aizwys.cn

crypto.randomUUID()
来源：http://jiw.gogol.net.cn

[U116] JS：类型检查（JSDoc）
来源：http://cic.wangshuangyany.cn

/** @param {string} name */ function f(name) {}
来源：http://uvu.jinghuilouyu.cn

[U117] JS：单元测试
来源：http://udg.vehdjk.com

npm i -D vitest;  npx vitest
来源：http://mxv.cdnleiting.top

[U118] JS：开发服务器
来源：http://inn.shuidangran.top

npm i -D vite;  npx vite
来源：http://hnk.c1oappe.top

[U119] JS：生产构建
来源：http://nwv.zhaomingkeji.xyz

npx vite build
来源：http://zfp.zhiwuduotai.top

[U120] JS：读取环境变量（Vite）
来源：http://zxl.birdmap.top

import.meta.env.VITE_API_URL
来源：http://tfk.wangshuangyany.cn

================================================================================
来源：http://tbo.zdbjq.cn

统计汇总
来源：http://hlz.chenlongwang.top

================================================================================
来源：http://mzi.bjfxy.top

按语言统计（条）：
来源：http://gsv.shangyingyoupin.top

Python ......... 252
来源：http://sch.cdnleiting.top

PHP ............ 252
来源：http://okv.nanxuanxn.top

JavaScript ..... 252
来源：http://tyw.wangshuangyany.cn

TypeScript ..... 212
来源：http://nyy.zdqjudy.top

Java ........... 212
来源：http://xws.ywan-chungtsiang.top

Go ............. 212
来源：http://eoi.aibaodan.cn

Ruby ........... 212
来源：http://wxy.zhongyouzk.top

C# ............. 212
来源：http://poc.kuanghao11.cn

C .............. 30
来源：http://suz.jqgufenzy.top

C++ ............ 30
来源：http://kin.jqgfzy.top

SQL ............ 90
来源：http://wfd.ydjk.org.cn

Bash ........... 80
来源：http://vtb.wangshuangyany.cn

Kotlin ......... 15
来源：http://itz.zdbjq.cn

Swift .......... 15
来源：http://gwp.jiagoushi.top

Lua ............ 10
来源：http://ofv.aibaodan.cn

Perl ........... 10
来源：http://ege.jiagoushi.top

Scala .......... 10
来源：http://ftf.quarkkingdee.top

------------------------------------
来源：http://gor.ywan-chungtsiang.top

合计 ........... 2106 条
来源：http://xme.ydzc1.top

按章节统计：
来源：http://uue.zhongyouzk.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://erd.bjfxy.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://vov.sufxvd.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://ahk.ybcxt.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://fsx.chenjidiqi.icu

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://lwq.aibaodan.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://mcp.yueranfly.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://jsp.mhx1999.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://sir.jqgfzy.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://tbw.ctjpmb.com

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://vvs.chenlongwang.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://wup.sxryk.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://lgh.gzhubu.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://efu.uphjek.com

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://rbo.ywan-chungtsiang.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://cwl.aizwys.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://ots.uphjek.com

Q SQL 专题                              90
来源：http://cud.jyoumei.cn

R Bash 专题                             80
来源：http://rwa.yongpay.top

S C / C++ 专题                          60
来源：http://vna.yuxming.cn

T 其他语言补充                          60
来源：http://xyc.hnxiangtu.top

U 高频实用片段                         120
来源：http://eim.52xcode.cn

------------------------------------
来源：http://uzn.cheryme.top

合计                                  2106 条
来源：http://iga.bjfxy.top

--------------------------------------------------------------------------------
来源：http://cbd.yuanzhike.top

使用提醒
来源：http://vvq.feifeiyinyue.top

--------------------------------------------------------------------------------
来源：http://llp.chenjidiqi.icu

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://izm.chenjidiqi.icu

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://fgv.kuanghao11.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://faa.jyoumei.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://yey.shangyingyoupin.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://gkl.nanxuanxn.top

—— 文件结束 ——
来源：http://fic.fktsv.cn

================================================================================
来源：http://nuv.yonumen.top

程序语言常见例子速查手册（2024 版）
来源：http://lke.smart0.xyz

Common Programming Examples Cheat Book
来源：http://edr.ybcxt.top

================================================================================
来源：http://zpp.jinqigfzy.top

【收录内容】
来源：http://ffo.nanxinkj.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://vqq.yonumen.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://ckv.cashguo.top

SQL · Bash · C · C++
来源：http://wrv.ydjk.org.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://gvo.dashuyun.cn

【使用说明】
来源：http://oey.hammf.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://gxh.kuanghao11.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://hot.ppjwa.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://ahy.xuanzx.com

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://cre.hnxiangtu.top

Bash:  Shell         C:     C             C++:   C++
来源：http://mts.birdmap.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://usd.ehwqpu.com


<!-- 参考信息 -->