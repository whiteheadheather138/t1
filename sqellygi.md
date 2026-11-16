代发 wailian999

[U07] Py：反转字典键值
来源：http://vhe.tanke756.top

{v: k for k, v in d.items()}
来源：http://igx.iojbl.cn

[U08] Py：展平二维列表
来源：http://gza.nanxuanxn.top

[y for x in nested for y in x]
来源：http://kap.wangshuangyany.cn

[U09] Py：字典取最大值的键
来源：http://nnu.gzhubu.top

max(d, key=d.get)
来源：http://zye.nanxuanxn.top

[U10] Py：按值排序字典
来源：http://vyf.gogol.net.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://yra.sufxvd.cn

[U11] Py：生成器表达式
来源：http://vom.zhoulong.xyz

(x * 2 for x in arr)
来源：http://pjb.jinyuanbaomall.cn

[U12] Py：取出现最多的 3 个元素
来源：http://hrm.ybcxt.top

Counter(arr).most_common(3)
来源：http://avp.zhaomingkeji.xyz

[U13] Py：固定长度队列
来源：http://xra.yj20258888.top

deque(maxlen=10)
来源：http://ged.jianghu66.top

[U14] Py：分组收集到列表
来源：http://lfe.havefunace.top

defaultdict(list)
来源：http://nei.ydjk.org.cn

[U15] Py：高精度计时
来源：http://yxe.pycfn.com

t = time.perf_counter()
来源：http://ajh.52xcode.cn

[U16] Py：命令行参数解析
来源：http://tfp.yueranfly.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://acs.yj20258888.top

[U17] Py：初始化日志
来源：http://hyu.jinyuanbaomall.cn

logging.basicConfig(level=logging.INFO)
来源：http://mvp.ywan-chungtsiang.top

[U18] Py：预编译正则
来源：http://lqi.mhx1999.top

pat = re.compile(r"\d+")
来源：http://vrh.hammf.cn

[U19] Py：正则替换带回调
来源：http://aua.tianlin.xyz

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://bgt.quarkkingdee.top

[U20] Py：缓存函数结果
来源：http://ubg.epnwcf.com

@functools.lru_cache(maxsize=None)
来源：http://kmf.daria6918.cn

[U21] Py：自定义上下文管理器
来源：http://cng.jinqigfzy.top

@contextlib.contextmanager
来源：http://vjp.tarul.cn

[U22] Py：矩阵转置
来源：http://zus.ppjwa.cn

list(zip(*m))
来源：http://anh.hfpthk.cn

[U23] Py：分块读取大文件
来源：http://qio.shanyushiyangtech.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://pnn.gaohongyu789.top

[U24] Py：路径操作
来源：http://gmd.redwolf501.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://csk.birdmap.top

[U25] Py：CSV 按字典读
来源：http://jhu.aibaodan.cn

csv.DictReader(f)
来源：http://ckv.yanxiufei.cn

[U26] Py：并发下载
来源：http://ezg.redwolf501.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://gee.nanxuanxn.top

[U27] Py：异步 HTTP
来源：http://tty.tianlin.xyz

aiohttp.ClientSession() 配合 async with
来源：http://wrl.zhaomingkeji.xyz

[U28] Py：类型别名
来源：http://ykv.yj202588.top

UserId = int
来源：http://nca.aibaodan.cn

[U29] Py：属性校验
来源：http://suv.cashguo.top

@property 与 @x.setter 配合
来源：http://mpg.vehdjk.com

[U30] Py：数据类
来源：http://qlb.yj20258888.top

@dataclass(slots=True)
来源：http://xrq.guannengcc.top

[U31] Py：单测
来源：http://toe.feifeiyinyue.top

python -m pytest -q
来源：http://ujl.shanyushiyangkeji.top

[U32] Py：代码格式化
来源：http://ttm.birdmap.top

ruff format . && ruff check --fix .
来源：http://yfn.hcnkem.com

[U33] Py：打包发布
来源：http://xct.jlsjyb.cn

python -m build  （依赖 pyproject.toml）
来源：http://vks.zdqjudy.top

[U34] Py：判断编码
来源：http://iwl.nanxuanxn.top

chardet.detect(raw)
来源：http://fwe.andypj.xyz

[U35] Py：发送邮件
来源：http://pgu.hnqzz.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://ywj.zdqjudy.top

[U36] Py：定时任务
来源：http://wag.yuxming.cn

schedule.every(10).minutes.do(job)
来源：http://wku.tanke756.top

[U37] Py：读写 Excel
来源：http://xns.birdmap.top

pandas.read_excel / DataFrame.to_excel
来源：http://iwb.zhiwuduotai.top

[U38] Py：获取脚本所在目录
来源：http://tjr.ehwqpu.com

Path(__file__).resolve().parent
来源：http://cal.ivvv.top

[U39] Py：判断是否在交互环境
来源：http://pcu.zhaomingkeji.xyz

sys.stdout.isatty()
来源：http://osm.andypj.xyz

[U40] Py：打印到标准错误
来源：http://afs.cashguo.top

print("err", file=sys.stderr)
来源：http://mtg.zhongyouzk.top

[U41] PHP：初始化 Composer 项目
来源：http://emk.aibaodan.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://wwm.pengpengdd.cyou

[U42] PHP：PSR-4 自动加载
来源：http://bzi.zhengqikj.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://xcq.meibo888.top

[U43] PHP：声明命名空间
来源：http://zcm.havefunace.top

namespace App\Http;
来源：http://tty.ehwqpu.com

[U44] PHP：开启严格类型
来源：http://wfn.hongshengwenyu.top

declare(strict_types=1);
来源：http://qmw.yongpay.top

[U45] PHP：类型声明与返回类型
来源：http://ekp.jyoumei.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://fui.birdmap.top

[U46] PHP：可空类型
来源：http://rmj.shuidangran.top

?string $name = null
来源：http://ytu.yonumen.top

[U47] PHP：联合类型
来源：http://ebm.jinyuanbaomall.cn

int|string $id
来源：http://akv.hysaishi.cn

[U48] PHP：纯枚举
来源：http://aps.redwolf501.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://xub.gaohongyu789.top

[U49] PHP：只读属性
来源：http://hor.hnxiangtu.top

public readonly string $name
来源：http://gst.shanyushiyangkeji.top

[U50] PHP：构造器属性提升
来源：http://xcl.fktsv.cn

public function __construct(private int $id) {}
来源：http://uzs.aizwys.cn

[U51] PHP：数组解构
来源：http://hps.jiagoushi.top

[$a, $b] = $arr;
来源：http://ccu.tianlin.xyz

[U52] PHP：箭头函数
来源：http://jfw.guannengcc.top

$double = fn($x) => $x * 2;
来源：http://dgm.jyoumei.cn

[U53] PHP：空合并运算符
来源：http://vdi.iojbl.cn

$v = $a ?? $b ?? "default";
来源：http://gdn.sufxvd.cn

[U54] PHP：空安全调用
来源：http://cnb.jiagoushi.top

$obj?->method()
来源：http://fwq.sweek.top

[U55] PHP：match 表达式
来源：http://uhw.daria6918.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://cdi.xuanzx.com

[U56] PHP：命名参数
来源：http://sti.jyoumei.cn

f(a: 1, b: 2)
来源：http://gnn.fengsongda.top

[U57] PHP：字符串插值
来源：http://ddr.aizwys.cn

"值: {$a}"
来源：http://dka.jinqigufen.top

[U58] PHP：数组三件套
来源：http://onq.jiagoushi.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://pln.0kj1m.cn

[U59] PHP：自定义排序
来源：http://zll.quarkkingdee.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://bng.bjfxy.top

[U60] PHP：JSON 编解码
来源：http://izb.iojbl.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://upt.fengsongda.top

[U61] PHP：正则
来源：http://gpg.xinyue.icu

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://vdq.yj20258.top

[U62] PHP：日期对象
来源：http://nhb.svipenyu.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://szc.yonumen.top

[U63] PHP：文件读写
来源：http://trx.ehwqpu.com

file_get_contents($f);  file_put_contents($f, $data);
来源：http://beb.ywan-chungtsiang.top

[U64] PHP：目录遍历
来源：http://aqn.chenlongwang.top

glob("dir/*.php");  scandir("dir");
来源：http://qaw.yonumen.top

[U65] PHP：会话
来源：http://czd.zhongyouzk.top

session_start();  $_SESSION["uid"] = 1;
来源：http://nki.zhaomingkeji.xyz

[U66] PHP：设置 Cookie
来源：http://nzy.bjfxy.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://rqy.xuanzx.com

[U67] PHP：处理文件上传
来源：http://kbc.jinghuilouyu.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://hfz.shangyingyoupin.top

[U68] PHP：PDO 连接
来源：http://iyr.jinghuilouyu.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://mhb.vehdjk.com

[U69] PHP：PDO 预处理
来源：http://bli.jianghu66.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://zeg.xuetiantiany.cn

[U70] PHP：PDO 事务
来源：http://tfb.fzhhl.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://dyu.cdnleiting.top

[U71] PHP：抛出异常
来源：http://rac.shzxlz.cn

throw new RuntimeException("失败", 500);
来源：http://wxl.cdnleiting.top

[U72] PHP：写错误日志
来源：http://mto.uphjek.com

error_log("失败: " . $e->getMessage());
来源：http://lki.shanyushiyangkeji.top

[U73] PHP：读取 ini 配置
来源：http://bqx.zhongyouzk.top

parse_ini_file("config.ini", true)
来源：http://klu.xuanzx.com

[U74] PHP：读取环境变量
来源：http://zaa.xuanzx.com

getenv("APP_ENV") ?: "production"
来源：http://mhy.quarkkingdee.top

[U75] PHP：依赖注入
来源：http://cxj.9152youxi.cn

composer require psr/container
来源：http://sxn.yvedp.cn

[U76] PHP：简单路由
来源：http://mej.bjfxy.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://aty.zhiwuduotai.top

[U77] PHP：模板渲染
来源：http://fro.jqgufenzy.top

composer require twig/twig
来源：http://eaz.hammf.cn

[U78] PHP：单元测试
来源：http://aba.yj202588.top

composer require --dev phpunit/phpunit
来源：http://sxr.vehdjk.com

[U79] PHP：静态分析
来源：http://nch.ppjwa.cn

composer require --dev phpstan/phpstan
来源：http://khb.mhx1999.top

[U80] PHP：代码规范修复
来源：http://gcp.jlsjyb.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://bny.zhaomingkeji.xyz

[U81] JS：初始化项目
来源：http://pri.shangyingyoupin.top

npm init -y;  npm i express
来源：http://hby.ywan-chungtsiang.top

[U82] JS：package.json 脚本
来源：http://ych.pengpengdd.cyou

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://dpi.jiagoushi.top

[U83] JS：ES Module 导入导出
来源：http://uso.fehbvm.com

export const a = 1;  import { a } from "./m.js";
来源：http://jtx.tarul.cn

[U84] JS：CommonJS 写法
来源：http://esu.sxryk.cn

module.exports = { a };  const { a } = require("./m");
来源：http://rnq.ydjk.org.cn

[U85] JS：可选链
来源：http://alx.sjlbkw.cn

a?.b?.c
来源：http://nzv.kuanghao11.cn

[U86] JS：空值合并
来源：http://vzx.cucudq.cn

a ?? b
来源：http://rlo.nanxuanxn.top

[U87] JS：解构默认值
来源：http://jdh.bjfxy.top

const { a = 1, b = 2 } = obj;
来源：http://lxf.cdnleiting.top

[U88] JS：对象展开合并
来源：http://qfv.vehdjk.com

{ ...a, ...b }
来源：http://ngq.jianghu66.top

[U89] JS：数组去重
来源：http://rnf.birdmap.top

[...new Set(arr)]
来源：http://ibw.gaohongyu789.top

[U90] JS：数字数组排序
来源：http://yej.xingfuxueyuan.xyz

[...arr].sort((a, b) => a - b)
来源：http://xjn.jiagoushi.top

[U91] JS：对象键值遍历
来源：http://tmp.gaohongyu789.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://anm.uphjek.com

[U92] JS：深拷贝
来源：http://mgs.haohaochexian.top

structuredClone(obj)
来源：http://dhu.guannengcc.top

[U93] JS：模板字符串
来源：http://osf.zhongyouzk.top

`共 ${n} 条`
来源：http://hls.guannengcc.top

[U94] JS：箭头函数
来源：http://uqr.hesvh.cn

const double = x => x * 2;
来源：http://dmy.yueranfly.top

[U95] JS：Promise 包装
来源：http://qzn.cheryme.top

new Promise((resolve, reject) => {})
来源：http://qqx.c1oappe.top

[U96] JS：async/await 与异常
来源：http://sot.jinqigfzy.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://shr.yonumen.top

[U97] JS：并发请求
来源：http://glb.jinqigufen.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://mgt.hcnkem.com

[U98] JS：fetch 带 JSON
来源：http://url.0kj1m.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://usa.yj20258888.top

[U99] JS：事件监听
来源：http://zne.xziqi.cn

el.addEventListener("click", e => {})
来源：http://mev.zycfv.cn

[U100] JS：DOM 查询
来源：http://fkx.cqqwz.cn

document.querySelector(".item")
来源：http://aff.jianghu66.top

[U101] JS：classList 操作
来源：http://thc.guannengcc.top

el.classList.toggle("active")
来源：http://dhg.fanxiaobao.xyz

[U102] JS：本地存储
来源：http://vve.gogol.net.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://osf.tanke756.top

[U103] JS：定时器
来源：http://nmi.yonumen.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://sle.jyoumei.cn

[U104] JS：防抖
来源：http://pry.ydzc1.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://eyh.ppjwa.cn

[U105] JS：节流
来源：http://yzm.52xcode.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://vcm.zhongyouzk.top

[U106] JS：日期格式化
来源：http://wzn.xuanzx.com

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://isp.shanyushiyangkeji.top

[U107] JS：数字千分位
来源：http://tuv.ywan-chungtsiang.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://vuo.0kj1m.cn

[U108] JS：随机整数
来源：http://sry.jianghu66.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://kmw.ivvv.top

[U109] JS：数组分组
来源：http://xeq.quarkkingdee.top

Object.groupBy(arr, x => x.type)
来源：http://xws.uphjek.com

[U110] JS：数组分块
来源：http://pjk.dianchejie.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://lyd.hfpthk.cn

[U111] JS：对象转 Map
来源：http://zxc.zhongyouzk.top

new Map(Object.entries(obj))
来源：http://pum.jqgufenzy.top

[U112] JS：字符串补位
来源：http://izo.jinyuanbaomall.cn

"7".padStart(3, "0")
来源：http://qrs.andypj.xyz

[U113] JS：正则替换全部
来源：http://zvp.pycfn.com

s.replaceAll("a", "b")
来源：http://eib.hcnkem.com

[U114] JS：JSON 深比较
来源：http://qjp.zhengqikj.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://ptw.hesvh.cn

[U115] JS：生成 UUID
来源：http://dqb.aizwys.cn

crypto.randomUUID()
来源：http://qhy.dashuyun.cn

[U116] JS：类型检查（JSDoc）
来源：http://dxr.wangshuangyany.cn

/** @param {string} name */ function f(name) {}
来源：http://qvs.fengsongda.top

[U117] JS：单元测试
来源：http://wuf.ehwqpu.com

npm i -D vitest;  npx vitest
来源：http://vdh.jyoumei.cn

[U118] JS：开发服务器
来源：http://mto.tian-w.cn

npm i -D vite;  npx vite
来源：http://jiz.fehbvm.com

[U119] JS：生产构建
来源：http://kpm.yanxiufei.cn

npx vite build
来源：http://hpq.jqgufenzy.top

[U120] JS：读取环境变量（Vite）
来源：http://ojx.yuxming.cn

import.meta.env.VITE_API_URL
来源：http://mnf.birdmap.top

================================================================================
来源：http://ubw.yuxming.cn

统计汇总
来源：http://rjd.shuidangran.top

================================================================================
来源：http://pbf.shanyushiyangtech.top

按语言统计（条）：
来源：http://ixz.zhaomingkeji.xyz

Python ......... 252
来源：http://rbo.yuxming.cn

PHP ............ 252
来源：http://irg.hesvh.cn

JavaScript ..... 252
来源：http://iph.sxryk.cn

TypeScript ..... 212
来源：http://tfv.hywenlv.cn

Java ........... 212
来源：http://iyv.gzhubu.top

Go ............. 212
来源：http://pwd.shanyushiyangtech.top

Ruby ........... 212
来源：http://qxn.xylfe.cn

C# ............. 212
来源：http://ldf.dianchejie.cn

C .............. 30
来源：http://vuc.xuetiantiany.cn

C++ ............ 30
来源：http://sjy.zhiwuduotai.top

SQL ............ 90
来源：http://rcs.shanyushiyangtech.top

Bash ........... 80
来源：http://fon.yuanzhike.top

Kotlin ......... 15
来源：http://qml.jinqigufen.top

Swift .......... 15
来源：http://cez.zhongyouzk.top

Lua ............ 10
来源：http://gxi.dianchejie.cn

Perl ........... 10
来源：http://oxi.zycfv.cn

Scala .......... 10
来源：http://xea.hfpthk.cn

------------------------------------
来源：http://wev.c1oappe.top

合计 ........... 2106 条
来源：http://slk.quarkkingdee.top

按章节统计：
来源：http://yfk.c1oappe.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://pwo.sjlbkw.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://qxn.ybcxt.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://wdy.sysykeji.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://unp.tian-w.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://ovo.cashguo.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://ycu.jinyuanbaomall.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://mvo.fengsongda.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://omz.hammf.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://gqc.zycfv.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://ipa.meibo888.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://aso.shangyingyoupin.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://zoz.xziqi.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://pgq.guowangkeji.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://okg.cdnleiting.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://bpt.hongshengwenyu.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://aid.tanke756.top

Q SQL 专题                              90
来源：http://opv.jinyuanbaomall.cn

R Bash 专题                             80
来源：http://xsl.ydjk.org.cn

S C / C++ 专题                          60
来源：http://quk.meibo888.top

T 其他语言补充                          60
来源：http://lkh.chenjidiqi.icu

U 高频实用片段                         120
来源：http://jwk.aizwys.cn

------------------------------------
来源：http://zfo.gaohongyu789.top

合计                                  2106 条
来源：http://ozt.yonumen.top

--------------------------------------------------------------------------------
来源：http://wjk.hongshengwenyu.top

使用提醒
来源：http://mky.zdbjq.cn

--------------------------------------------------------------------------------
来源：http://xvr.fanxiaobao.xyz

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://lyz.snrcjt.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://sje.xylfe.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://oaz.yonumen.top

在旧版本上使用前请先确认语法支持情况。
来源：http://nqt.vehdjk.com

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://egs.xziqi.cn

—— 文件结束 ——
来源：http://twr.ywan-chungtsiang.top

================================================================================
来源：http://zwk.fanxiaobao.xyz

程序语言常见例子速查手册（2024 版）
来源：http://imy.gogol.net.cn

Common Programming Examples Cheat Book
来源：http://amg.hongshengwenyu.top

================================================================================
来源：http://hoa.yfazqb.com

【收录内容】
来源：http://fgo.yuanzhike.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://eiv.hesvh.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://rpa.nanxinkj.top

SQL · Bash · C · C++
来源：http://vsh.shanyushiyangtech.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://rle.smart0.xyz

【使用说明】
来源：http://yrc.xuanzx.com

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://jam.ppjwa.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://kdq.zhoulong.xyz

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://saw.sufxvd.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://dym.yfazqb.com

Bash:  Shell         C:     C             C++:   C++
来源：http://bup.tarul.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://oaq.zhijiandao.cn


<!-- 参考信息 -->