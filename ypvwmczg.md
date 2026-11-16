代发 wailian999

[U05] Py：列表去重且保序
来源：http://qfe.gaohongyu789.top

list(dict.fromkeys(arr))
来源：http://zjn.fehbvm.com

[U06] Py：合并两个字典
来源：http://uvn.svipenyu.cn

{**a, **b}
来源：http://rti.wangdashe.top

[U07] Py：反转字典键值
来源：http://tgk.pycfn.com

{v: k for k, v in d.items()}
来源：http://wlz.bjfxy.top

[U08] Py：展平二维列表
来源：http://wjw.tian-w.cn

[y for x in nested for y in x]
来源：http://sgp.cheryme.top

[U09] Py：字典取最大值的键
来源：http://qmj.ehwqpu.com

max(d, key=d.get)
来源：http://uza.uphjek.com

[U10] Py：按值排序字典
来源：http://eoc.gotoacloud.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://pnl.yj20258888.top

[U11] Py：生成器表达式
来源：http://wyb.daria6918.cn

(x * 2 for x in arr)
来源：http://ngh.yangfankeji.com

[U12] Py：取出现最多的 3 个元素
来源：http://hkp.nanxuanxn.top

Counter(arr).most_common(3)
来源：http://fll.jiagoushi.top

[U13] Py：固定长度队列
来源：http://xmk.nanxuanxn.top

deque(maxlen=10)
来源：http://edh.uphjek.com

[U14] Py：分组收集到列表
来源：http://wdb.guowangkeji.top

defaultdict(list)
来源：http://rnf.dashuyun.cn

[U15] Py：高精度计时
来源：http://slr.9152youxi.cn

t = time.perf_counter()
来源：http://buo.hnxiangtu.top

[U16] Py：命令行参数解析
来源：http://ozn.vqdsnc.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://rnv.svipenyu.cn

[U17] Py：初始化日志
来源：http://mpg.gogol.net.cn

logging.basicConfig(level=logging.INFO)
来源：http://zsr.fehbvm.com

[U18] Py：预编译正则
来源：http://gcr.bbcook.cn

pat = re.compile(r"\d+")
来源：http://ezj.zhijiandao.cn

[U19] Py：正则替换带回调
来源：http://htt.zdbjq.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://sma.xingfuxueyuan.xyz

[U20] Py：缓存函数结果
来源：http://vqv.jqgufenzy.top

@functools.lru_cache(maxsize=None)
来源：http://eus.ydzc1.top

[U21] Py：自定义上下文管理器
来源：http://crs.zdbjq.cn

@contextlib.contextmanager
来源：http://ktu.tian-w.cn

[U22] Py：矩阵转置
来源：http://ciu.nwbrower.top

list(zip(*m))
来源：http://vom.jinyuanbaomall.cn

[U23] Py：分块读取大文件
来源：http://pau.yuxming.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://kuk.cdnleiting.top

[U24] Py：路径操作
来源：http://nyx.dashuyun.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://lhj.fktsv.cn

[U25] Py：CSV 按字典读
来源：http://vcf.aizwys.cn

csv.DictReader(f)
来源：http://gpf.pengpengdd.cyou

[U26] Py：并发下载
来源：http://uyf.xziqi.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://xde.wangdashe.top

[U27] Py：异步 HTTP
来源：http://etu.fzhhl.top

aiohttp.ClientSession() 配合 async with
来源：http://ytr.fanxiaobao.xyz

[U28] Py：类型别名
来源：http://uxh.xylfe.cn

UserId = int
来源：http://bky.shanyushiyangtech.top

[U29] Py：属性校验
来源：http://vsb.nanxinkj.top

@property 与 @x.setter 配合
来源：http://lzc.gogol.net.cn

[U30] Py：数据类
来源：http://jth.ybcxt.top

@dataclass(slots=True)
来源：http://hlh.xinyue.icu

[U31] Py：单测
来源：http://bni.yuxming.cn

python -m pytest -q
来源：http://mjk.jqgufenzy.top

[U32] Py：代码格式化
来源：http://uol.sjlbkw.cn

ruff format . && ruff check --fix .
来源：http://wcs.zhengqikj.top

[U33] Py：打包发布
来源：http://vpo.quarkkingdee.top

python -m build  （依赖 pyproject.toml）
来源：http://owv.bbcook.cn

[U34] Py：判断编码
来源：http://xap.gotoacloud.top

chardet.detect(raw)
来源：http://giu.mhx1999.top

[U35] Py：发送邮件
来源：http://zqy.shanyushiyangtech.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://pcm.cucudq.cn

[U36] Py：定时任务
来源：http://cvy.zdbjq.cn

schedule.every(10).minutes.do(job)
来源：http://ehw.yj20258.top

[U37] Py：读写 Excel
来源：http://hfc.epnwcf.com

pandas.read_excel / DataFrame.to_excel
来源：http://vep.tian-w.cn

[U38] Py：获取脚本所在目录
来源：http://fvi.cheryme.top

Path(__file__).resolve().parent
来源：http://fwy.epnwcf.com

[U39] Py：判断是否在交互环境
来源：http://ope.yj202588.top

sys.stdout.isatty()
来源：http://fgk.aibaodan.cn

[U40] Py：打印到标准错误
来源：http://zta.shanyushiyangkeji.top

print("err", file=sys.stderr)
来源：http://pvj.jlsjyb.cn

[U41] PHP：初始化 Composer 项目
来源：http://rwb.zdqjudy.top

composer init;  composer require guzzlehttp/guzzle
来源：http://jau.chenzaomai.com

[U42] PHP：PSR-4 自动加载
来源：http://zos.hammf.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://ktf.chenlongwang.top

[U43] PHP：声明命名空间
来源：http://fho.meibo888.top

namespace App\Http;
来源：http://dwj.iojbl.cn

[U44] PHP：开启严格类型
来源：http://xrm.316326.xyz

declare(strict_types=1);
来源：http://nre.snrcjt.cn

[U45] PHP：类型声明与返回类型
来源：http://rze.kuanghao11.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://xot.yanxiufei.cn

[U46] PHP：可空类型
来源：http://vvh.sjlbkw.cn

?string $name = null
来源：http://pmh.mhx1999.top

[U47] PHP：联合类型
来源：http://crq.xuanzx.com

int|string $id
来源：http://mle.havefunace.top

[U48] PHP：纯枚举
来源：http://tiq.yanxiufei.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hym.tianlin.xyz

[U49] PHP：只读属性
来源：http://ges.meibo888.top

public readonly string $name
来源：http://efq.quarkkingdee.top

[U50] PHP：构造器属性提升
来源：http://bwy.mhx1999.top

public function __construct(private int $id) {}
来源：http://yyc.hnqzz.top

[U51] PHP：数组解构
来源：http://htf.zhaomingkeji.xyz

[$a, $b] = $arr;
来源：http://erl.daxiang520.top

[U52] PHP：箭头函数
来源：http://mvs.yvedp.cn

$double = fn($x) => $x * 2;
来源：http://nrs.havefunace.top

[U53] PHP：空合并运算符
来源：http://vuh.ydzc1.top

$v = $a ?? $b ?? "default";
来源：http://yur.xylfe.cn

[U54] PHP：空安全调用
来源：http://yoc.wangdashe.top

$obj?->method()
来源：http://ngy.redwolf501.top

[U55] PHP：match 表达式
来源：http://tqi.vehdjk.com

$s = match($x) { 1 => "一", default => "其他" };
来源：http://bpy.daxiang520.top

[U56] PHP：命名参数
来源：http://jsn.cheryme.top

f(a: 1, b: 2)
来源：http://erg.316326.xyz

[U57] PHP：字符串插值
来源：http://igi.xuetiantiany.cn

"值: {$a}"
来源：http://qmi.yj202588.top

[U58] PHP：数组三件套
来源：http://dvn.zhiwuduotai.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://qhz.fktsv.cn

[U59] PHP：自定义排序
来源：http://aqp.xuetiantiany.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://xpu.fengsongda.top

[U60] PHP：JSON 编解码
来源：http://gtw.wangshuangyany.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://cew.haohaochexian.top

[U61] PHP：正则
来源：http://mha.hfpthk.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://vzi.jianghu66.top

[U62] PHP：日期对象
来源：http://sdv.pycfn.com

(new DateTimeImmutable())->format("Y-m-d");
来源：http://nle.gotoacloud.top

[U63] PHP：文件读写
来源：http://ath.dianchejie.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://rhl.pycfn.com

[U64] PHP：目录遍历
来源：http://ptg.hnqzz.top

glob("dir/*.php");  scandir("dir");
来源：http://lln.xingfuxueyuan.xyz

[U65] PHP：会话
来源：http://kiu.yangfankeji.com

session_start();  $_SESSION["uid"] = 1;
来源：http://hyz.bbcook.cn

[U66] PHP：设置 Cookie
来源：http://jrq.shanyushiyangtech.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://kpi.xuetiantiany.cn

[U67] PHP：处理文件上传
来源：http://zcj.ehwqpu.com

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://kdq.sjlbkw.cn

[U68] PHP：PDO 连接
来源：http://bus.yueranfly.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://mwz.hywenlv.cn

[U69] PHP：PDO 预处理
来源：http://pyi.wangdashe.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://iaz.52xcode.cn

[U70] PHP：PDO 事务
来源：http://knd.sxryk.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://jvq.ppjwa.cn

[U71] PHP：抛出异常
来源：http://rkv.yueranfly.top

throw new RuntimeException("失败", 500);
来源：http://muj.gogol.net.cn

[U72] PHP：写错误日志
来源：http://xwy.zhixingplan.top

error_log("失败: " . $e->getMessage());
来源：http://ukt.316326.xyz

[U73] PHP：读取 ini 配置
来源：http://whp.cucudq.cn

parse_ini_file("config.ini", true)
来源：http://eda.sufxvd.cn

[U74] PHP：读取环境变量
来源：http://fip.sjlbkw.cn

getenv("APP_ENV") ?: "production"
来源：http://mbe.jlsjyb.cn

[U75] PHP：依赖注入
来源：http://wxo.jinqigufen.top

composer require psr/container
来源：http://ugy.yvedp.cn

[U76] PHP：简单路由
来源：http://ypm.ydzc1.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://kao.hywenlv.cn

[U77] PHP：模板渲染
来源：http://wiq.fzhhl.top

composer require twig/twig
来源：http://nyv.zdbjq.cn

[U78] PHP：单元测试
来源：http://npe.yangfankeji.com

composer require --dev phpunit/phpunit
来源：http://wlh.yj20258.top

[U79] PHP：静态分析
来源：http://hpf.daria6918.cn

composer require --dev phpstan/phpstan
来源：http://fij.dianchejie.cn

[U80] PHP：代码规范修复
来源：http://pda.52xcode.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://ypn.andypj.xyz

[U81] JS：初始化项目
来源：http://iwk.jianghu66.top

npm init -y;  npm i express
来源：http://ddp.andypj.xyz

[U82] JS：package.json 脚本
来源：http://zpx.zhengqikj.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://mod.yj20258.top

[U83] JS：ES Module 导入导出
来源：http://zfd.cucudq.cn

export const a = 1;  import { a } from "./m.js";
来源：http://paz.meibo888.top

[U84] JS：CommonJS 写法
来源：http://zrt.fengsongda.top

module.exports = { a };  const { a } = require("./m");
来源：http://wkz.nanxinkj.top

[U85] JS：可选链
来源：http://hsg.tian-w.cn

a?.b?.c
来源：http://eux.yvedp.cn

[U86] JS：空值合并
来源：http://pop.smart0.xyz

a ?? b
来源：http://mkp.yongpay.top

[U87] JS：解构默认值
来源：http://uga.daxiang520.top

const { a = 1, b = 2 } = obj;
来源：http://dsy.hnxiangtu.top

[U88] JS：对象展开合并
来源：http://qhv.fktsv.cn

{ ...a, ...b }
来源：http://dhl.shzxlz.cn

[U89] JS：数组去重
来源：http://puo.jiagoushi.top

[...new Set(arr)]
来源：http://fyt.316326.xyz

[U90] JS：数字数组排序
来源：http://wdw.hywenlv.cn

[...arr].sort((a, b) => a - b)
来源：http://upd.hongshengwenyu.top

[U91] JS：对象键值遍历
来源：http://qqj.hysaishi.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://fvk.hfpthk.cn

[U92] JS：深拷贝
来源：http://fsc.pengpengdd.cyou

structuredClone(obj)
来源：http://vey.c1oappe.top

[U93] JS：模板字符串
来源：http://iuc.xuetiantiany.cn

`共 ${n} 条`
来源：http://jqz.jianghu66.top

[U94] JS：箭头函数
来源：http://csg.c1oappe.top

const double = x => x * 2;
来源：http://bxr.yfazqb.com

[U95] JS：Promise 包装
来源：http://fhe.zycfv.cn

new Promise((resolve, reject) => {})
来源：http://kcr.shzxlz.cn

[U96] JS：async/await 与异常
来源：http://jwm.yj20258888.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://mpt.sysykeji.top

[U97] JS：并发请求
来源：http://ety.52xcode.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://zkd.vqdsnc.cn

[U98] JS：fetch 带 JSON
来源：http://djv.dashuyun.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://rnj.andypj.xyz

[U99] JS：事件监听
来源：http://ibs.birdmap.top

el.addEventListener("click", e => {})
来源：http://mwa.fzhhl.top

[U100] JS：DOM 查询
来源：http://beh.tarul.cn

document.querySelector(".item")
来源：http://xpy.ydzc1.top

[U101] JS：classList 操作
来源：http://flg.yvedp.cn

el.classList.toggle("active")
来源：http://kgd.wangshuangyany.cn

[U102] JS：本地存储
来源：http://ecc.fktsv.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://pag.fengsongda.top

[U103] JS：定时器
来源：http://pxj.ctjpmb.com

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://exz.yj202588.top

[U104] JS：防抖
来源：http://nfp.jiagoushi.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://npc.sysykeji.top

[U105] JS：节流
来源：http://xsm.yfazqb.com

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://jxs.fktsv.cn

[U106] JS：日期格式化
来源：http://lil.sysykeji.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://rfv.xziqi.cn

[U107] JS：数字千分位
来源：http://hfs.vqdsnc.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://rqv.yfazqb.com

[U108] JS：随机整数
来源：http://sme.jianghu66.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://nuf.jqgfzy.top

[U109] JS：数组分组
来源：http://gte.jinqigufen.top

Object.groupBy(arr, x => x.type)
来源：http://emy.sweek.top

[U110] JS：数组分块
来源：http://mzs.hysaishi.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://mtr.316326.xyz

[U111] JS：对象转 Map
来源：http://uqt.gzhubu.top

new Map(Object.entries(obj))
来源：http://vmg.redwolf501.top

[U112] JS：字符串补位
来源：http://mzv.9152youxi.cn

"7".padStart(3, "0")
来源：http://ucq.ydjk.org.cn

[U113] JS：正则替换全部
来源：http://pbi.shanyushiyangtech.top

s.replaceAll("a", "b")
来源：http://cvh.ywan-chungtsiang.top

[U114] JS：JSON 深比较
来源：http://wtt.guowangkeji.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://mlt.wangdashe.top

[U115] JS：生成 UUID
来源：http://nbj.cdnleiting.top

crypto.randomUUID()
来源：http://yfu.sysykeji.top

[U116] JS：类型检查（JSDoc）
来源：http://hzr.fanxiaobao.xyz

/** @param {string} name */ function f(name) {}
来源：http://yil.ppjwa.cn

[U117] JS：单元测试
来源：http://kwg.hfpthk.cn

npm i -D vitest;  npx vitest
来源：http://fjn.kuanghao11.cn

[U118] JS：开发服务器
来源：http://qfu.jianghu66.top

npm i -D vite;  npx vite
来源：http://lmk.havefunace.top

[U119] JS：生产构建
来源：http://izj.jinyuanbaomall.cn

npx vite build
来源：http://aho.chenlongwang.top

[U120] JS：读取环境变量（Vite）
来源：http://nkt.chenzaomai.com

import.meta.env.VITE_API_URL
来源：http://svn.wangdashe.top

================================================================================
来源：http://jgh.ehwqpu.com

统计汇总
来源：http://kff.yj20258888.top

================================================================================
来源：http://oih.gotoacloud.top

按语言统计（条）：
来源：http://eku.yvedp.cn

Python ......... 252
来源：http://www.daxiang520.top

PHP ............ 252
来源：http://mby.yangfankeji.com

JavaScript ..... 252
来源：http://znb.ydzc1.top

TypeScript ..... 212
来源：http://vqi.nwbrower.top

Java ........... 212
来源：http://xdg.yangfankeji.com

Go ............. 212
来源：http://upj.sxryk.cn

Ruby ........... 212
来源：http://dio.chenlongwang.top

C# ............. 212
来源：http://apo.nwbrower.top

C .............. 30
来源：http://ujr.yuxming.cn

C++ ............ 30
来源：http://cgd.tian-w.cn

SQL ............ 90
来源：http://vgw.shuidangran.top

Bash ........... 80
来源：http://xwk.yanxiufei.cn

Kotlin ......... 15
来源：http://mbx.zhaomingkeji.xyz

Swift .......... 15
来源：http://zcy.zhixingplan.top

Lua ............ 10
来源：http://txm.ydzc1.top

Perl ........... 10
来源：http://elf.haohaochexian.top

Scala .......... 10
来源：http://zbw.guannengcc.top

------------------------------------
来源：http://how.dashuyun.cn

合计 ........... 2106 条
来源：http://uwa.kuanghao11.cn

按章节统计：
来源：http://shi.fzhhl.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://ixv.gaohongyu789.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://pnw.haohaochexian.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://eny.dashuyun.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://kzf.vehdjk.com

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://rsa.yj202588.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://xtz.jinghuilouyu.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://taq.jinqigufen.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://bot.fzhhl.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://nop.ppjwa.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://wog.yongpay.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://pij.fengsongda.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://ljc.aibaodan.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://mvk.yuanzhike.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://qrl.zhengqikj.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://paz.hongshengwenyu.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://mfm.52xcode.cn

Q SQL 专题                              90
来源：http://uvp.xingfuxueyuan.xyz

R Bash 专题                             80
来源：http://pwp.ywan-chungtsiang.top

S C / C++ 专题                          60
来源：http://uht.aizwys.cn

T 其他语言补充                          60
来源：http://eun.tian-w.cn

U 高频实用片段                         120
来源：http://vze.52xcode.cn

------------------------------------
来源：http://mwo.shzxlz.cn

合计                                  2106 条
来源：http://ogi.gzhubu.top

--------------------------------------------------------------------------------
来源：http://kpt.feifeiyinyue.top

使用提醒
来源：http://edb.fengsongda.top

--------------------------------------------------------------------------------
来源：http://tcz.epnwcf.com

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://zfe.9152youxi.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://mqt.chenzaomai.com

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://gsu.iojbl.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://tpt.yanxiufei.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://awy.c1oappe.top

—— 文件结束 ——
来源：http://fsh.tanke756.top

================================================================================
来源：http://yos.smart0.xyz

程序语言常见例子速查手册（2024 版）
来源：http://krz.yueranfly.top

Common Programming Examples Cheat Book
来源：http://wnl.316326.xyz

================================================================================
来源：http://rvs.yvedp.cn

【收录内容】
来源：http://vld.haohaochexian.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://uuz.hywenlv.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://fot.gogol.net.cn

SQL · Bash · C · C++
来源：http://clg.sjlbkw.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://nuk.nanxinkj.top

【使用说明】
来源：http://qce.feifeiyinyue.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://bcj.yuanzhike.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://skw.gaohongyu789.top


<!-- 参考信息 -->