代发 wailian999

[U05] Py：列表去重且保序
来源：http://dra.jiagoushi.top

list(dict.fromkeys(arr))
来源：http://qwm.chenzaomai.com

[U06] Py：合并两个字典
来源：http://grq.gzhubu.top

{**a, **b}
来源：http://xwd.shuidangran.top

[U07] Py：反转字典键值
来源：http://nzx.yuanzhike.top

{v: k for k, v in d.items()}
来源：http://awf.jlsjyb.cn

[U08] Py：展平二维列表
来源：http://hwu.svipenyu.cn

[y for x in nested for y in x]
来源：http://tfl.andypj.xyz

[U09] Py：字典取最大值的键
来源：http://hgh.jqgfzy.top

max(d, key=d.get)
来源：http://sxg.xylfe.cn

[U10] Py：按值排序字典
来源：http://pvw.zhaomingkeji.xyz

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://tcz.cucudq.cn

[U11] Py：生成器表达式
来源：http://hal.9152youxi.cn

(x * 2 for x in arr)
来源：http://xyc.gaohongyu789.top

[U12] Py：取出现最多的 3 个元素
来源：http://evg.nanxinkj.top

Counter(arr).most_common(3)
来源：http://jlz.chenjidiqi.icu

[U13] Py：固定长度队列
来源：http://vdn.zhengqikj.top

deque(maxlen=10)
来源：http://tlz.vehdjk.com

[U14] Py：分组收集到列表
来源：http://flv.yongpay.top

defaultdict(list)
来源：http://wkq.xuanzx.com

[U15] Py：高精度计时
来源：http://xoe.shangyingyoupin.top

t = time.perf_counter()
来源：http://wce.shuidangran.top

[U16] Py：命令行参数解析
来源：http://gkr.haohaochexian.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://itm.aibaodan.cn

[U17] Py：初始化日志
来源：http://zog.fktsv.cn

logging.basicConfig(level=logging.INFO)
来源：http://hen.nanxinkj.top

[U18] Py：预编译正则
来源：http://eco.shanyushiyangkeji.top

pat = re.compile(r"\d+")
来源：http://fml.cdnleiting.top

[U19] Py：正则替换带回调
来源：http://apc.bbcook.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://gvs.xylfe.cn

[U20] Py：缓存函数结果
来源：http://jbt.gaohongyu789.top

@functools.lru_cache(maxsize=None)
来源：http://jah.tian-w.cn

[U21] Py：自定义上下文管理器
来源：http://ywt.nanxinkj.top

@contextlib.contextmanager
来源：http://eps.vqdsnc.cn

[U22] Py：矩阵转置
来源：http://rjh.ywan-chungtsiang.top

list(zip(*m))
来源：http://uqd.sysykeji.top

[U23] Py：分块读取大文件
来源：http://ncj.aizwys.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://lpw.yvedp.cn

[U24] Py：路径操作
来源：http://ajn.shanyushiyangkeji.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://ulg.fzhhl.top

[U25] Py：CSV 按字典读
来源：http://cjz.feifeiyinyue.top

csv.DictReader(f)
来源：http://hjj.fehbvm.com

[U26] Py：并发下载
来源：http://imw.chenzaomai.com

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://wym.pycfn.com

[U27] Py：异步 HTTP
来源：http://gxj.svipenyu.cn

aiohttp.ClientSession() 配合 async with
来源：http://ruq.sweek.top

[U28] Py：类型别名
来源：http://mne.cucudq.cn

UserId = int
来源：http://prn.hcnkem.com

[U29] Py：属性校验
来源：http://ify.ivvv.top

@property 与 @x.setter 配合
来源：http://jeh.shanyushiyangkeji.top

[U30] Py：数据类
来源：http://sfn.wangshuangyany.cn

@dataclass(slots=True)
来源：http://wil.guowangkeji.top

[U31] Py：单测
来源：http://qny.yongpay.top

python -m pytest -q
来源：http://jdl.tarul.cn

[U32] Py：代码格式化
来源：http://ket.xingfuxueyuan.xyz

ruff format . && ruff check --fix .
来源：http://kbm.tarul.cn

[U33] Py：打包发布
来源：http://vov.yj20258.top

python -m build  （依赖 pyproject.toml）
来源：http://loi.yanxiufei.cn

[U34] Py：判断编码
来源：http://xcj.jinghuilouyu.cn

chardet.detect(raw)
来源：http://wdx.ydjk.org.cn

[U35] Py：发送邮件
来源：http://vfr.kuanghao11.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://lnr.chenlongwang.top

[U36] Py：定时任务
来源：http://uif.jiagoushi.top

schedule.every(10).minutes.do(job)
来源：http://drk.yueranfly.top

[U37] Py：读写 Excel
来源：http://iud.jiagoushi.top

pandas.read_excel / DataFrame.to_excel
来源：http://zya.gaohongyu789.top

[U38] Py：获取脚本所在目录
来源：http://sqb.bbcook.cn

Path(__file__).resolve().parent
来源：http://ncz.pycfn.com

[U39] Py：判断是否在交互环境
来源：http://xze.c1oappe.top

sys.stdout.isatty()
来源：http://cwy.mhx1999.top

[U40] Py：打印到标准错误
来源：http://bbw.sufxvd.cn

print("err", file=sys.stderr)
来源：http://muk.haohaochexian.top

[U41] PHP：初始化 Composer 项目
来源：http://zwi.cdnleiting.top

composer init;  composer require guzzlehttp/guzzle
来源：http://xju.redwolf501.top

[U42] PHP：PSR-4 自动加载
来源：http://jwy.fanxiaobao.xyz

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://kci.cashguo.top

[U43] PHP：声明命名空间
来源：http://acb.cheryme.top

namespace App\Http;
来源：http://snr.c1oappe.top

[U44] PHP：开启严格类型
来源：http://mmk.snrcjt.cn

declare(strict_types=1);
来源：http://zpf.zhiwuduotai.top

[U45] PHP：类型声明与返回类型
来源：http://hat.wangshuangyany.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://eyl.haohaochexian.top

[U46] PHP：可空类型
来源：http://lcu.cdnleiting.top

?string $name = null
来源：http://dgo.dianchejie.cn

[U47] PHP：联合类型
来源：http://jmb.jianghu66.top

int|string $id
来源：http://jrv.zhijiandao.cn

[U48] PHP：纯枚举
来源：http://qey.ctjpmb.com

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://wyw.bjfxy.top

[U49] PHP：只读属性
来源：http://qzx.fengsongda.top

public readonly string $name
来源：http://dwm.ivvv.top

[U50] PHP：构造器属性提升
来源：http://ter.cqqwz.cn

public function __construct(private int $id) {}
来源：http://bhx.hnxiangtu.top

[U51] PHP：数组解构
来源：http://srf.fanxiaobao.xyz

[$a, $b] = $arr;
来源：http://kgo.zhijiandao.cn

[U52] PHP：箭头函数
来源：http://cso.zhijiandao.cn

$double = fn($x) => $x * 2;
来源：http://hjt.ppjwa.cn

[U53] PHP：空合并运算符
来源：http://jrc.pycfn.com

$v = $a ?? $b ?? "default";
来源：http://fau.yj20258888.top

[U54] PHP：空安全调用
来源：http://nls.xuetiantiany.cn

$obj?->method()
来源：http://uip.52xcode.cn

[U55] PHP：match 表达式
来源：http://eah.iojbl.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://iuh.hcnkem.com

[U56] PHP：命名参数
来源：http://twx.hesvh.cn

f(a: 1, b: 2)
来源：http://usa.hammf.cn

[U57] PHP：字符串插值
来源：http://xet.jinqigfzy.top

"值: {$a}"
来源：http://zdq.tanke756.top

[U58] PHP：数组三件套
来源：http://hfs.gaohongyu789.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://pxf.ehwqpu.com

[U59] PHP：自定义排序
来源：http://wrg.svipenyu.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://tlp.redwolf501.top

[U60] PHP：JSON 编解码
来源：http://rxf.cucudq.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://jsh.yonumen.top

[U61] PHP：正则
来源：http://hrx.hywenlv.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://nde.zhaomingkeji.xyz

[U62] PHP：日期对象
来源：http://pas.haohaochexian.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://lxl.hnxiangtu.top

[U63] PHP：文件读写
来源：http://kep.pycfn.com

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hvo.havefunace.top

[U64] PHP：目录遍历
来源：http://sxw.yonumen.top

glob("dir/*.php");  scandir("dir");
来源：http://sxs.hcnkem.com

[U65] PHP：会话
来源：http://avt.feifeiyinyue.top

session_start();  $_SESSION["uid"] = 1;
来源：http://gyq.cucudq.cn

[U66] PHP：设置 Cookie
来源：http://rwk.hywenlv.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://ylz.vehdjk.com

[U67] PHP：处理文件上传
来源：http://jiz.jinghuilouyu.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://pjk.hcnkem.com

[U68] PHP：PDO 连接
来源：http://wie.mhx1999.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://wjw.bbcook.cn

[U69] PHP：PDO 预处理
来源：http://vpe.chenlongwang.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://acx.jinyuanbaomall.cn

[U70] PHP：PDO 事务
来源：http://cvn.zdqjudy.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://taj.mhx1999.top

[U71] PHP：抛出异常
来源：http://qvb.chenlongwang.top

throw new RuntimeException("失败", 500);
来源：http://uin.c1oappe.top

[U72] PHP：写错误日志
来源：http://mnk.vehdjk.com

error_log("失败: " . $e->getMessage());
来源：http://ptp.jiagoushi.top

[U73] PHP：读取 ini 配置
来源：http://ssv.shanyushiyangtech.top

parse_ini_file("config.ini", true)
来源：http://lph.aizwys.cn

[U74] PHP：读取环境变量
来源：http://vib.ivvv.top

getenv("APP_ENV") ?: "production"
来源：http://olf.sysykeji.top

[U75] PHP：依赖注入
来源：http://bvq.yj20258888.top

composer require psr/container
来源：http://fct.316326.xyz

[U76] PHP：简单路由
来源：http://adu.daxiang520.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://bfk.guannengcc.top

[U77] PHP：模板渲染
来源：http://lbn.zhongyouzk.top

composer require twig/twig
来源：http://ant.zycfv.cn

[U78] PHP：单元测试
来源：http://zgc.ppjwa.cn

composer require --dev phpunit/phpunit
来源：http://sou.gotoacloud.top

[U79] PHP：静态分析
来源：http://hog.guannengcc.top

composer require --dev phpstan/phpstan
来源：http://hjr.havefunace.top

[U80] PHP：代码规范修复
来源：http://zlh.ehwqpu.com

composer require --dev friendsofphp/php-cs-fixer
来源：http://ghe.gzhubu.top

[U81] JS：初始化项目
来源：http://gba.nwbrower.top

npm init -y;  npm i express
来源：http://ayi.ybcxt.top

[U82] JS：package.json 脚本
来源：http://dms.shangyingyoupin.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://gzm.ehwqpu.com

[U83] JS：ES Module 导入导出
来源：http://wsp.ehwqpu.com

export const a = 1;  import { a } from "./m.js";
来源：http://jjn.fehbvm.com

[U84] JS：CommonJS 写法
来源：http://arj.9152youxi.cn

module.exports = { a };  const { a } = require("./m");
来源：http://yxu.vehdjk.com

[U85] JS：可选链
来源：http://lhw.redwolf501.top

a?.b?.c
来源：http://dkb.birdmap.top

[U86] JS：空值合并
来源：http://jyp.zhaomingkeji.xyz

a ?? b
来源：http://yuq.tian-w.cn

[U87] JS：解构默认值
来源：http://hsm.gzhubu.top

const { a = 1, b = 2 } = obj;
来源：http://gcz.aibaodan.cn

[U88] JS：对象展开合并
来源：http://ugt.pengpengdd.cyou

{ ...a, ...b }
来源：http://eqy.mhx1999.top

[U89] JS：数组去重
来源：http://bik.cashguo.top

[...new Set(arr)]
来源：http://thd.shuidangran.top

[U90] JS：数字数组排序
来源：http://jlu.316326.xyz

[...arr].sort((a, b) => a - b)
来源：http://jyg.yanxiufei.cn

[U91] JS：对象键值遍历
来源：http://ahn.epnwcf.com

Object.entries(obj).forEach(([k, v]) => {});
来源：http://suw.zhijiandao.cn

[U92] JS：深拷贝
来源：http://nsw.jianghu66.top

structuredClone(obj)
来源：http://qxc.ehwqpu.com

[U93] JS：模板字符串
来源：http://fio.zdqjudy.top

`共 ${n} 条`
来源：http://ukk.xylfe.cn

[U94] JS：箭头函数
来源：http://vvm.gotoacloud.top

const double = x => x * 2;
来源：http://ocd.zhiwuduotai.top

[U95] JS：Promise 包装
来源：http://bah.jiagoushi.top

new Promise((resolve, reject) => {})
来源：http://ulu.hongshengwenyu.top

[U96] JS：async/await 与异常
来源：http://ehu.quarkkingdee.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://fbp.mhx1999.top

[U97] JS：并发请求
来源：http://gmx.jinyuanbaomall.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://nxi.yuxming.cn

[U98] JS：fetch 带 JSON
来源：http://uzq.yj20258.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://uks.vqdsnc.cn

[U99] JS：事件监听
来源：http://zgd.jyoumei.cn

el.addEventListener("click", e => {})
来源：http://tgs.yj20258.top

[U100] JS：DOM 查询
来源：http://tdb.daria6918.cn

document.querySelector(".item")
来源：http://iut.smart0.xyz

[U101] JS：classList 操作
来源：http://qcc.316326.xyz

el.classList.toggle("active")
来源：http://cxr.ybcxt.top

[U102] JS：本地存储
来源：http://yqo.xinyue.icu

localStorage.setItem("k", JSON.stringify(v))
来源：http://vzo.jinyuanbaomall.cn

[U103] JS：定时器
来源：http://rez.ydzc1.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://ajq.dianchejie.cn

[U104] JS：防抖
来源：http://lvc.mhx1999.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hbn.hfpthk.cn

[U105] JS：节流
来源：http://xju.zhiwuduotai.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://dsv.chenjidiqi.icu

[U106] JS：日期格式化
来源：http://acy.nanxuanxn.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://alb.xuetiantiany.cn

[U107] JS：数字千分位
来源：http://hnu.nwbrower.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://owy.tanke756.top

[U108] JS：随机整数
来源：http://ccl.nanxinkj.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://mlr.chenlongwang.top

[U109] JS：数组分组
来源：http://ntw.sysykeji.top

Object.groupBy(arr, x => x.type)
来源：http://wir.sweek.top

[U110] JS：数组分块
来源：http://phf.ydjk.org.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://bsb.jianghu66.top

[U111] JS：对象转 Map
来源：http://ymt.jinqigfzy.top

new Map(Object.entries(obj))
来源：http://qoh.jinyuanbaomall.cn

[U112] JS：字符串补位
来源：http://exd.mhx1999.top

"7".padStart(3, "0")
来源：http://gsk.fktsv.cn

[U113] JS：正则替换全部
来源：http://jnl.pengpengdd.cyou

s.replaceAll("a", "b")
来源：http://wiq.sxryk.cn

[U114] JS：JSON 深比较
来源：http://pnz.ctjpmb.com

JSON.stringify(a) === JSON.stringify(b)
来源：http://ymz.yonumen.top

[U115] JS：生成 UUID
来源：http://gjo.ywan-chungtsiang.top

crypto.randomUUID()
来源：http://jpo.jqgfzy.top

[U116] JS：类型检查（JSDoc）
来源：http://zou.zhiwuduotai.top

/** @param {string} name */ function f(name) {}
来源：http://tcz.hcnkem.com

[U117] JS：单元测试
来源：http://gph.hfpthk.cn

npm i -D vitest;  npx vitest
来源：http://ezx.zhaomingkeji.xyz

[U118] JS：开发服务器
来源：http://htm.shangyingyoupin.top

npm i -D vite;  npx vite
来源：http://zbi.andypj.xyz

[U119] JS：生产构建
来源：http://rwp.sufxvd.cn

npx vite build
来源：http://vqp.chenzaomai.com

[U120] JS：读取环境变量（Vite）
来源：http://bjf.hongshengwenyu.top

import.meta.env.VITE_API_URL
来源：http://vqr.nwbrower.top

================================================================================
来源：http://qiv.zhoulong.xyz

统计汇总
来源：http://chc.yanxiufei.cn

================================================================================
来源：http://zrj.zhiwuduotai.top

按语言统计（条）：
来源：http://cfw.zhixingplan.top

Python ......... 252
来源：http://lal.hywenlv.cn

PHP ............ 252
来源：http://hwy.chenzaomai.com

JavaScript ..... 252
来源：http://eux.redwolf501.top

TypeScript ..... 212
来源：http://qtr.hcnkem.com

Java ........... 212
来源：http://lux.zdqjudy.top

Go ............. 212
来源：http://poc.zycfv.cn

Ruby ........... 212
来源：http://ezk.svipenyu.cn

C# ............. 212
来源：http://fxh.daxiang520.top

C .............. 30
来源：http://whp.andypj.xyz

C++ ............ 30
来源：http://jkc.vehdjk.com

SQL ............ 90
来源：http://ody.xuetiantiany.cn

Bash ........... 80
来源：http://wai.xingfuxueyuan.xyz

Kotlin ......... 15
来源：http://pfd.fktsv.cn

Swift .......... 15
来源：http://jeh.cashguo.top

Lua ............ 10
来源：http://wts.xinyue.icu

Perl ........... 10
来源：http://jyd.xinyue.icu

Scala .......... 10
来源：http://djs.jlsjyb.cn

------------------------------------
来源：http://iiw.chenzaomai.com

合计 ........... 2106 条
来源：http://qvt.pengpengdd.cyou

按章节统计：
来源：http://yyv.sufxvd.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://cgj.yonumen.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://izr.yanxiufei.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://pzl.nanxuanxn.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://zwb.hammf.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://tip.wangdashe.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://ahp.redwolf501.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://ana.fehbvm.com

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://lzq.c1oappe.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://gfr.smart0.xyz

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://tnp.cashguo.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://wes.zdbjq.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://bwk.daxiang520.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://mxc.gzhubu.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://liz.zhoulong.xyz

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://ika.xinyue.icu

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://kfq.hesvh.cn

Q SQL 专题                              90
来源：http://hxg.fengsongda.top

R Bash 专题                             80
来源：http://mho.ywan-chungtsiang.top

S C / C++ 专题                          60
来源：http://dfi.daria6918.cn

T 其他语言补充                          60
来源：http://sno.gaohongyu789.top

U 高频实用片段                         120
来源：http://cea.hfpthk.cn

------------------------------------
来源：http://xxy.snrcjt.cn

合计                                  2106 条
来源：http://lxh.yj20258.top

--------------------------------------------------------------------------------
来源：http://trw.daxiang520.top

使用提醒
来源：http://ejm.vqdsnc.cn

--------------------------------------------------------------------------------
来源：http://pov.ywan-chungtsiang.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://tqs.cucudq.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://dqv.daxiang520.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://zdo.iojbl.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://adp.yonumen.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://ixt.bbcook.cn

—— 文件结束 ——
来源：http://ema.jianghu66.top

================================================================================
来源：http://xfk.zhongyouzk.top

程序语言常见例子速查手册（2024 版）
来源：http://ebd.sxryk.cn

Common Programming Examples Cheat Book
来源：http://jnm.xinyue.icu

================================================================================
来源：http://ifa.yfazqb.com

【收录内容】
来源：http://wur.nwbrower.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://sam.guowangkeji.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://cuo.zycfv.cn

SQL · Bash · C · C++
来源：http://haw.52xcode.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://xuf.wangdashe.top

【使用说明】
来源：http://ctt.gogol.net.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://brq.cqqwz.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://eam.fengsongda.top


<!-- 参考信息 -->