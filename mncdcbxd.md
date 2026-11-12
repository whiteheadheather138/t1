代发 wailian999

[U05] Py：列表去重且保序
来源：http://hlp.kuanghao11.cn

list(dict.fromkeys(arr))
来源：http://wjx.dashuyun.cn

[U06] Py：合并两个字典
来源：http://jye.zdqjudy.top

{**a, **b}
来源：http://rry.fktsv.cn

[U07] Py：反转字典键值
来源：http://mlr.ctjpmb.com

{v: k for k, v in d.items()}
来源：http://nmh.sysykeji.top

[U08] Py：展平二维列表
来源：http://qtx.hysaishi.cn

[y for x in nested for y in x]
来源：http://qlx.0kj1m.cn

[U09] Py：字典取最大值的键
来源：http://yea.feifeiyinyue.top

max(d, key=d.get)
来源：http://zfu.hammf.cn

[U10] Py：按值排序字典
来源：http://qae.yvedp.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://zwn.fengsongda.top

[U11] Py：生成器表达式
来源：http://sct.zdqjudy.top

(x * 2 for x in arr)
来源：http://oiz.shanyushiyangtech.top

[U12] Py：取出现最多的 3 个元素
来源：http://zyi.hcnkem.com

Counter(arr).most_common(3)
来源：http://jem.nwbrower.top

[U13] Py：固定长度队列
来源：http://fql.zhoulong.xyz

deque(maxlen=10)
来源：http://mzq.gaohongyu789.top

[U14] Py：分组收集到列表
来源：http://beh.gotoacloud.top

defaultdict(list)
来源：http://opl.jiagoushi.top

[U15] Py：高精度计时
来源：http://ixk.quarkkingdee.top

t = time.perf_counter()
来源：http://vtz.xylfe.cn

[U16] Py：命令行参数解析
来源：http://xlg.jinqigfzy.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://qnk.yueranfly.top

[U17] Py：初始化日志
来源：http://gzr.shanyushiyangkeji.top

logging.basicConfig(level=logging.INFO)
来源：http://ykr.vqdsnc.cn

[U18] Py：预编译正则
来源：http://mcn.fanxiaobao.xyz

pat = re.compile(r"\d+")
来源：http://pqs.9152youxi.cn

[U19] Py：正则替换带回调
来源：http://nzo.birdmap.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://yin.smart0.xyz

[U20] Py：缓存函数结果
来源：http://sfg.yvedp.cn

@functools.lru_cache(maxsize=None)
来源：http://zbl.zhongyouzk.top

[U21] Py：自定义上下文管理器
来源：http://ais.52xcode.cn

@contextlib.contextmanager
来源：http://ftg.kuanghao11.cn

[U22] Py：矩阵转置
来源：http://ubz.zycfv.cn

list(zip(*m))
来源：http://ofb.jianghu66.top

[U23] Py：分块读取大文件
来源：http://yqw.ydjk.org.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://vdm.ydzc1.top

[U24] Py：路径操作
来源：http://lrq.havefunace.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://dbs.9152youxi.cn

[U25] Py：CSV 按字典读
来源：http://zbb.jyoumei.cn

csv.DictReader(f)
来源：http://zpe.redwolf501.top

[U26] Py：并发下载
来源：http://zve.jinqigufen.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://pga.sweek.top

[U27] Py：异步 HTTP
来源：http://zwl.zhixingplan.top

aiohttp.ClientSession() 配合 async with
来源：http://cmi.feifeiyinyue.top

[U28] Py：类型别名
来源：http://gfp.zhengqikj.top

UserId = int
来源：http://zoc.svipenyu.cn

[U29] Py：属性校验
来源：http://jnb.gotoacloud.top

@property 与 @x.setter 配合
来源：http://kuv.xinyue.icu

[U30] Py：数据类
来源：http://nmy.ctjpmb.com

@dataclass(slots=True)
来源：http://yuj.pycfn.com

[U31] Py：单测
来源：http://wjy.cqqwz.cn

python -m pytest -q
来源：http://kcn.jqgfzy.top

[U32] Py：代码格式化
来源：http://myv.quarkkingdee.top

ruff format . && ruff check --fix .
来源：http://hcs.jlsjyb.cn

[U33] Py：打包发布
来源：http://rpr.hnqzz.top

python -m build  （依赖 pyproject.toml）
来源：http://jvp.cheryme.top

[U34] Py：判断编码
来源：http://gtm.xuanzx.com

chardet.detect(raw)
来源：http://bjt.jqgufenzy.top

[U35] Py：发送邮件
来源：http://vmm.yangfankeji.com

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://skx.shanyushiyangtech.top

[U36] Py：定时任务
来源：http://gvy.hywenlv.cn

schedule.every(10).minutes.do(job)
来源：http://pod.snrcjt.cn

[U37] Py：读写 Excel
来源：http://zrc.zhixingplan.top

pandas.read_excel / DataFrame.to_excel
来源：http://sky.9152youxi.cn

[U38] Py：获取脚本所在目录
来源：http://xjl.ivvv.top

Path(__file__).resolve().parent
来源：http://nfq.gzhubu.top

[U39] Py：判断是否在交互环境
来源：http://goc.svipenyu.cn

sys.stdout.isatty()
来源：http://aoj.tianlin.xyz

[U40] Py：打印到标准错误
来源：http://ebp.shanyushiyangtech.top

print("err", file=sys.stderr)
来源：http://cqe.sjlbkw.cn

[U41] PHP：初始化 Composer 项目
来源：http://jml.zhaomingkeji.xyz

composer init;  composer require guzzlehttp/guzzle
来源：http://qvm.fengsongda.top

[U42] PHP：PSR-4 自动加载
来源：http://tkw.wangshuangyany.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://kcd.hfpthk.cn

[U43] PHP：声明命名空间
来源：http://iny.redwolf501.top

namespace App\Http;
来源：http://wam.quarkkingdee.top

[U44] PHP：开启严格类型
来源：http://wuk.ehwqpu.com

declare(strict_types=1);
来源：http://ndl.zhongyouzk.top

[U45] PHP：类型声明与返回类型
来源：http://fxj.ivvv.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://khr.jinyuanbaomall.cn

[U46] PHP：可空类型
来源：http://art.yonumen.top

?string $name = null
来源：http://qnq.hfpthk.cn

[U47] PHP：联合类型
来源：http://lxx.52xcode.cn

int|string $id
来源：http://mvq.nanxuanxn.top

[U48] PHP：纯枚举
来源：http://bkg.hywenlv.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://yvl.bbcook.cn

[U49] PHP：只读属性
来源：http://cpm.shangyingyoupin.top

public readonly string $name
来源：http://zsn.zhongyouzk.top

[U50] PHP：构造器属性提升
来源：http://gyj.tianlin.xyz

public function __construct(private int $id) {}
来源：http://fys.hysaishi.cn

[U51] PHP：数组解构
来源：http://dbt.cucudq.cn

[$a, $b] = $arr;
来源：http://eky.jinghuilouyu.cn

[U52] PHP：箭头函数
来源：http://ihu.jyoumei.cn

$double = fn($x) => $x * 2;
来源：http://cbx.feifeiyinyue.top

[U53] PHP：空合并运算符
来源：http://kgu.yj20258.top

$v = $a ?? $b ?? "default";
来源：http://hrf.yonumen.top

[U54] PHP：空安全调用
来源：http://ptj.yuanzhike.top

$obj?->method()
来源：http://joh.bjfxy.top

[U55] PHP：match 表达式
来源：http://cte.nanxinkj.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://pzs.yongpay.top

[U56] PHP：命名参数
来源：http://wnu.mhx1999.top

f(a: 1, b: 2)
来源：http://bqz.ivvv.top

[U57] PHP：字符串插值
来源：http://agr.dashuyun.cn

"值: {$a}"
来源：http://yga.fehbvm.com

[U58] PHP：数组三件套
来源：http://dkl.zhoulong.xyz

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://bvk.fanxiaobao.xyz

[U59] PHP：自定义排序
来源：http://kbk.yfazqb.com

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://kvx.wangdashe.top

[U60] PHP：JSON 编解码
来源：http://luu.fzhhl.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://nyb.jlsjyb.cn

[U61] PHP：正则
来源：http://nmd.uphjek.com

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://esm.hnqzz.top

[U62] PHP：日期对象
来源：http://ojs.ivvv.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://fyo.xuanzx.com

[U63] PHP：文件读写
来源：http://usj.hcnkem.com

file_get_contents($f);  file_put_contents($f, $data);
来源：http://kbk.haohaochexian.top

[U64] PHP：目录遍历
来源：http://eke.jinqigfzy.top

glob("dir/*.php");  scandir("dir");
来源：http://qmz.mhx1999.top

[U65] PHP：会话
来源：http://ztn.xinyue.icu

session_start();  $_SESSION["uid"] = 1;
来源：http://rei.hammf.cn

[U66] PHP：设置 Cookie
来源：http://erg.epnwcf.com

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://qrs.tianlin.xyz

[U67] PHP：处理文件上传
来源：http://acj.fehbvm.com

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://wcq.sysykeji.top

[U68] PHP：PDO 连接
来源：http://jea.tanke756.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://wgq.shangyingyoupin.top

[U69] PHP：PDO 预处理
来源：http://ggm.kuanghao11.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://fit.yj202588.top

[U70] PHP：PDO 事务
来源：http://glf.xuanzx.com

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://mop.cucudq.cn

[U71] PHP：抛出异常
来源：http://mmu.hnqzz.top

throw new RuntimeException("失败", 500);
来源：http://sdm.fengsongda.top

[U72] PHP：写错误日志
来源：http://mbe.0kj1m.cn

error_log("失败: " . $e->getMessage());
来源：http://ota.ybcxt.top

[U73] PHP：读取 ini 配置
来源：http://jjo.ppjwa.cn

parse_ini_file("config.ini", true)
来源：http://ffl.zhijiandao.cn

[U74] PHP：读取环境变量
来源：http://rau.chenjidiqi.icu

getenv("APP_ENV") ?: "production"
来源：http://buw.0kj1m.cn

[U75] PHP：依赖注入
来源：http://asx.svipenyu.cn

composer require psr/container
来源：http://iho.ppjwa.cn

[U76] PHP：简单路由
来源：http://mgc.shanyushiyangkeji.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://vso.ehwqpu.com

[U77] PHP：模板渲染
来源：http://cbj.hnqzz.top

composer require twig/twig
来源：http://djg.tanke756.top

[U78] PHP：单元测试
来源：http://tiv.havefunace.top

composer require --dev phpunit/phpunit
来源：http://uyz.jyoumei.cn

[U79] PHP：静态分析
来源：http://rxb.pengpengdd.cyou

composer require --dev phpstan/phpstan
来源：http://ucr.yj20258888.top

[U80] PHP：代码规范修复
来源：http://hcl.zhiwuduotai.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://pom.ywan-chungtsiang.top

[U81] JS：初始化项目
来源：http://nnb.meibo888.top

npm init -y;  npm i express
来源：http://dcn.zhiwuduotai.top

[U82] JS：package.json 脚本
来源：http://ezg.tian-w.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://ymd.xuetiantiany.cn

[U83] JS：ES Module 导入导出
来源：http://pck.zhiwuduotai.top

export const a = 1;  import { a } from "./m.js";
来源：http://dbp.guannengcc.top

[U84] JS：CommonJS 写法
来源：http://mny.daxiang520.top

module.exports = { a };  const { a } = require("./m");
来源：http://jmg.tian-w.cn

[U85] JS：可选链
来源：http://zdu.jqgfzy.top

a?.b?.c
来源：http://jwa.zhiwuduotai.top

[U86] JS：空值合并
来源：http://wjt.zdqjudy.top

a ?? b
来源：http://bdr.xuanzx.com

[U87] JS：解构默认值
来源：http://ggg.fanxiaobao.xyz

const { a = 1, b = 2 } = obj;
来源：http://aks.wangshuangyany.cn

[U88] JS：对象展开合并
来源：http://bpt.guowangkeji.top

{ ...a, ...b }
来源：http://sxr.hongshengwenyu.top

[U89] JS：数组去重
来源：http://hfi.jinqigufen.top

[...new Set(arr)]
来源：http://zix.zhiwuduotai.top

[U90] JS：数字数组排序
来源：http://mto.hcnkem.com

[...arr].sort((a, b) => a - b)
来源：http://srv.jinqigfzy.top

[U91] JS：对象键值遍历
来源：http://yyz.ydjk.org.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://duy.zhixingplan.top

[U92] JS：深拷贝
来源：http://ppa.yj20258.top

structuredClone(obj)
来源：http://omj.zhiwuduotai.top

[U93] JS：模板字符串
来源：http://xwi.snrcjt.cn

`共 ${n} 条`
来源：http://pcp.zdbjq.cn

[U94] JS：箭头函数
来源：http://qnd.ctjpmb.com

const double = x => x * 2;
来源：http://azb.jiagoushi.top

[U95] JS：Promise 包装
来源：http://ixe.yuxming.cn

new Promise((resolve, reject) => {})
来源：http://hdr.gzhubu.top

[U96] JS：async/await 与异常
来源：http://wai.sxryk.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://ppw.zhijiandao.cn

[U97] JS：并发请求
来源：http://zav.zhijiandao.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://vod.fanxiaobao.xyz

[U98] JS：fetch 带 JSON
来源：http://kvy.chenjidiqi.icu

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://wsi.xuanzx.com

[U99] JS：事件监听
来源：http://bpr.jinghuilouyu.cn

el.addEventListener("click", e => {})
来源：http://pjv.fehbvm.com

[U100] JS：DOM 查询
来源：http://iza.aibaodan.cn

document.querySelector(".item")
来源：http://aqq.sysykeji.top

[U101] JS：classList 操作
来源：http://acd.aizwys.cn

el.classList.toggle("active")
来源：http://lvx.ivvv.top

[U102] JS：本地存储
来源：http://non.fktsv.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://nwd.tian-w.cn

[U103] JS：定时器
来源：http://ibw.iojbl.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://lho.tianlin.xyz

[U104] JS：防抖
来源：http://lri.sysykeji.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://bbc.wangshuangyany.cn

[U105] JS：节流
来源：http://slv.xylfe.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hpe.nanxinkj.top

[U106] JS：日期格式化
来源：http://jwx.yvedp.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://smp.uphjek.com

[U107] JS：数字千分位
来源：http://ram.vqdsnc.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://yxp.xingfuxueyuan.xyz

[U108] JS：随机整数
来源：http://usw.yj202588.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://txt.guowangkeji.top

[U109] JS：数组分组
来源：http://kyz.jiagoushi.top

Object.groupBy(arr, x => x.type)
来源：http://cth.vehdjk.com

[U110] JS：数组分块
来源：http://kru.chenlongwang.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://kfc.wangdashe.top

[U111] JS：对象转 Map
来源：http://lou.nanxinkj.top

new Map(Object.entries(obj))
来源：http://ltc.zhiwuduotai.top

[U112] JS：字符串补位
来源：http://ral.wangdashe.top

"7".padStart(3, "0")
来源：http://rpt.mhx1999.top

[U113] JS：正则替换全部
来源：http://kjk.yuanzhike.top

s.replaceAll("a", "b")
来源：http://llk.xziqi.cn

[U114] JS：JSON 深比较
来源：http://tgu.jlsjyb.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://vad.cucudq.cn

[U115] JS：生成 UUID
来源：http://zja.52xcode.cn

crypto.randomUUID()
来源：http://fwg.sjlbkw.cn

[U116] JS：类型检查（JSDoc）
来源：http://lba.yj202588.top

/** @param {string} name */ function f(name) {}
来源：http://vcv.hfpthk.cn

[U117] JS：单元测试
来源：http://fdd.xuanzx.com

npm i -D vitest;  npx vitest
来源：http://gpe.ivvv.top

[U118] JS：开发服务器
来源：http://wtc.andypj.xyz

npm i -D vite;  npx vite
来源：http://hww.yj202588.top

[U119] JS：生产构建
来源：http://kyx.shanyushiyangtech.top

npx vite build
来源：http://dwa.ydjk.org.cn

[U120] JS：读取环境变量（Vite）
来源：http://vza.hfpthk.cn

import.meta.env.VITE_API_URL
来源：http://eoq.xylfe.cn

================================================================================
来源：http://cpm.cucudq.cn

统计汇总
来源：http://yjv.guannengcc.top

================================================================================
来源：http://ohy.yvedp.cn

按语言统计（条）：
来源：http://chj.yj20258888.top

Python ......... 252
来源：http://bdk.yueranfly.top

PHP ............ 252
来源：http://okp.haohaochexian.top

JavaScript ..... 252
来源：http://yri.yj20258888.top

TypeScript ..... 212
来源：http://jnq.zhaomingkeji.xyz

Java ........... 212
来源：http://hap.fanxiaobao.xyz

Go ............. 212
来源：http://ulo.iojbl.cn

Ruby ........... 212
来源：http://zcg.cheryme.top

C# ............. 212
来源：http://vyb.shzxlz.cn

C .............. 30
来源：http://ury.aizwys.cn

C++ ............ 30
来源：http://fpx.zhixingplan.top

SQL ............ 90
来源：http://fot.ydzc1.top

Bash ........... 80
来源：http://zpp.wangdashe.top

Kotlin ......... 15
来源：http://ivx.sjlbkw.cn

Swift .......... 15
来源：http://yjk.wangshuangyany.cn

Lua ............ 10
来源：http://mfa.zhongyouzk.top

Perl ........... 10
来源：http://aod.zhiwuduotai.top

Scala .......... 10
来源：http://syi.cucudq.cn

------------------------------------
来源：http://hkj.jianghu66.top

合计 ........... 2106 条
来源：http://ulv.yuanzhike.top

按章节统计：
来源：http://arq.redwolf501.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hwn.zhaomingkeji.xyz

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://epi.wangdashe.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://wrc.gotoacloud.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://fbi.kuanghao11.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://etn.wangshuangyany.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://flh.ppjwa.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://djj.xylfe.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://sjj.ctjpmb.com

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://dex.hcnkem.com

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://gpn.yongpay.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://opj.nwbrower.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://afk.feifeiyinyue.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://bna.snrcjt.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://tbz.chenlongwang.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://zgv.zdqjudy.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://eho.hfpthk.cn

Q SQL 专题                              90
来源：http://sdr.ehwqpu.com

R Bash 专题                             80
来源：http://fsb.zhijiandao.cn

S C / C++ 专题                          60
来源：http://dvf.ybcxt.top

T 其他语言补充                          60
来源：http://lti.ehwqpu.com

U 高频实用片段                         120
来源：http://seu.tianlin.xyz

------------------------------------
来源：http://unk.ppjwa.cn

合计                                  2106 条
来源：http://yrl.hammf.cn

--------------------------------------------------------------------------------
来源：http://nvs.chenzaomai.com

使用提醒
来源：http://ojq.yangfankeji.com

--------------------------------------------------------------------------------
来源：http://xnj.yuxming.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://xvg.zhixingplan.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://kzt.jianghu66.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://hpl.fzhhl.top

在旧版本上使用前请先确认语法支持情况。
来源：http://lmi.tanke756.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://urv.iojbl.cn

—— 文件结束 ——
来源：http://vxs.smart0.xyz

================================================================================
来源：http://zhg.shzxlz.cn

程序语言常见例子速查手册（2024 版）
来源：http://fzu.gogol.net.cn

Common Programming Examples Cheat Book
来源：http://jir.mhx1999.top

================================================================================
来源：http://rvp.ydzc1.top

【收录内容】
来源：http://yir.sysykeji.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://ldb.nwbrower.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://huk.jinghuilouyu.cn

SQL · Bash · C · C++
来源：http://spb.havefunace.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://jko.feifeiyinyue.top

【使用说明】
来源：http://kzr.bjfxy.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://xha.uphjek.com

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://npl.hysaishi.cn


<!-- 参考信息 -->