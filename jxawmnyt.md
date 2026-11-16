代发 wailian999

[U01] Py：创建虚拟环境
来源：http://lef.yvedp.cn

python -m venv .venv && source .venv/bin/activate
来源：http://jyx.kuanghao11.cn

[U02] Py：导出 / 安装依赖
来源：http://kgh.iojbl.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://onx.hammf.cn

[U03] Py：加载 .env 配置
来源：http://gjr.ivvv.top

from dotenv import load_dotenv; load_dotenv()
来源：http://ytl.yuxming.cn

[U04] Py：变量调试打印
来源：http://sxb.ppjwa.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://fgl.chenlongwang.top

[U05] Py：列表去重且保序
来源：http://pef.ydjk.org.cn

list(dict.fromkeys(arr))
来源：http://cxp.xuanzx.com

[U06] Py：合并两个字典
来源：http://ygg.cashguo.top

{**a, **b}
来源：http://iwd.guannengcc.top

[U07] Py：反转字典键值
来源：http://pld.redwolf501.top

{v: k for k, v in d.items()}
来源：http://ggt.yuxming.cn

[U08] Py：展平二维列表
来源：http://tcq.tianlin.xyz

[y for x in nested for y in x]
来源：http://doj.kuanghao11.cn

[U09] Py：字典取最大值的键
来源：http://oiv.shanyushiyangkeji.top

max(d, key=d.get)
来源：http://uti.fktsv.cn

[U10] Py：按值排序字典
来源：http://xfi.sjlbkw.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://ckv.gaohongyu789.top

[U11] Py：生成器表达式
来源：http://bpw.chenzaomai.com

(x * 2 for x in arr)
来源：http://yfb.zhaomingkeji.xyz

[U12] Py：取出现最多的 3 个元素
来源：http://fyx.gotoacloud.top

Counter(arr).most_common(3)
来源：http://zlr.andypj.xyz

[U13] Py：固定长度队列
来源：http://fzb.birdmap.top

deque(maxlen=10)
来源：http://wmc.cqqwz.cn

[U14] Py：分组收集到列表
来源：http://omc.jiagoushi.top

defaultdict(list)
来源：http://six.daxiang520.top

[U15] Py：高精度计时
来源：http://bwe.shzxlz.cn

t = time.perf_counter()
来源：http://qrj.gzhubu.top

[U16] Py：命令行参数解析
来源：http://dbo.jqgufenzy.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://wba.tianlin.xyz

[U17] Py：初始化日志
来源：http://uch.hesvh.cn

logging.basicConfig(level=logging.INFO)
来源：http://feo.tianlin.xyz

[U18] Py：预编译正则
来源：http://cql.nwbrower.top

pat = re.compile(r"\d+")
来源：http://vps.tianlin.xyz

[U19] Py：正则替换带回调
来源：http://ugq.ywan-chungtsiang.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://qqi.uphjek.com

[U20] Py：缓存函数结果
来源：http://brz.gogol.net.cn

@functools.lru_cache(maxsize=None)
来源：http://ngc.tian-w.cn

[U21] Py：自定义上下文管理器
来源：http://zyc.yuxming.cn

@contextlib.contextmanager
来源：http://byw.sysykeji.top

[U22] Py：矩阵转置
来源：http://nzh.hfpthk.cn

list(zip(*m))
来源：http://hbh.quarkkingdee.top

[U23] Py：分块读取大文件
来源：http://ktx.tarul.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hxz.hywenlv.cn

[U24] Py：路径操作
来源：http://hhs.nwbrower.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://jnb.bjfxy.top

[U25] Py：CSV 按字典读
来源：http://ypk.cheryme.top

csv.DictReader(f)
来源：http://pfq.fengsongda.top

[U26] Py：并发下载
来源：http://prn.shuidangran.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://fpy.xinyue.icu

[U27] Py：异步 HTTP
来源：http://mse.meibo888.top

aiohttp.ClientSession() 配合 async with
来源：http://htt.nanxinkj.top

[U28] Py：类型别名
来源：http://iqh.xziqi.cn

UserId = int
来源：http://hmc.fengsongda.top

[U29] Py：属性校验
来源：http://kgo.birdmap.top

@property 与 @x.setter 配合
来源：http://cbm.yfazqb.com

[U30] Py：数据类
来源：http://fba.c1oappe.top

@dataclass(slots=True)
来源：http://qfc.chenlongwang.top

[U31] Py：单测
来源：http://kvo.yfazqb.com

python -m pytest -q
来源：http://aru.cashguo.top

[U32] Py：代码格式化
来源：http://swx.yueranfly.top

ruff format . && ruff check --fix .
来源：http://vqz.chenjidiqi.icu

[U33] Py：打包发布
来源：http://nvm.cucudq.cn

python -m build  （依赖 pyproject.toml）
来源：http://azk.ehwqpu.com

[U34] Py：判断编码
来源：http://lqs.pengpengdd.cyou

chardet.detect(raw)
来源：http://ddt.jinqigfzy.top

[U35] Py：发送邮件
来源：http://kpq.0kj1m.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://wsr.uphjek.com

[U36] Py：定时任务
来源：http://aew.52xcode.cn

schedule.every(10).minutes.do(job)
来源：http://ipp.sxryk.cn

[U37] Py：读写 Excel
来源：http://kae.xingfuxueyuan.xyz

pandas.read_excel / DataFrame.to_excel
来源：http://rmf.ydzc1.top

[U38] Py：获取脚本所在目录
来源：http://qnz.epnwcf.com

Path(__file__).resolve().parent
来源：http://rwm.pengpengdd.cyou

[U39] Py：判断是否在交互环境
来源：http://zjq.pengpengdd.cyou

sys.stdout.isatty()
来源：http://dff.nanxinkj.top

[U40] Py：打印到标准错误
来源：http://dpi.zhongyouzk.top

print("err", file=sys.stderr)
来源：http://huk.c1oappe.top

[U41] PHP：初始化 Composer 项目
来源：http://jsf.xinyue.icu

composer init;  composer require guzzlehttp/guzzle
来源：http://aoz.yuxming.cn

[U42] PHP：PSR-4 自动加载
来源：http://jpb.sjlbkw.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://jcn.yueranfly.top

[U43] PHP：声明命名空间
来源：http://mxp.svipenyu.cn

namespace App\Http;
来源：http://rsz.andypj.xyz

[U44] PHP：开启严格类型
来源：http://pxq.nanxuanxn.top

declare(strict_types=1);
来源：http://gnw.zdbjq.cn

[U45] PHP：类型声明与返回类型
来源：http://fgp.daria6918.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://bpo.jinyuanbaomall.cn

[U46] PHP：可空类型
来源：http://wmi.zdbjq.cn

?string $name = null
来源：http://fso.jinghuilouyu.cn

[U47] PHP：联合类型
来源：http://cmn.hnxiangtu.top

int|string $id
来源：http://ysr.ywan-chungtsiang.top

[U48] PHP：纯枚举
来源：http://nip.yangfankeji.com

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://gvi.hcnkem.com

[U49] PHP：只读属性
来源：http://iln.havefunace.top

public readonly string $name
来源：http://chg.c1oappe.top

[U50] PHP：构造器属性提升
来源：http://fkr.quarkkingdee.top

public function __construct(private int $id) {}
来源：http://wxn.cashguo.top

[U51] PHP：数组解构
来源：http://iyp.fengsongda.top

[$a, $b] = $arr;
来源：http://emq.ydjk.org.cn

[U52] PHP：箭头函数
来源：http://noh.hammf.cn

$double = fn($x) => $x * 2;
来源：http://vox.shangyingyoupin.top

[U53] PHP：空合并运算符
来源：http://gqm.andypj.xyz

$v = $a ?? $b ?? "default";
来源：http://axu.aizwys.cn

[U54] PHP：空安全调用
来源：http://kvc.yonumen.top

$obj?->method()
来源：http://huz.pycfn.com

[U55] PHP：match 表达式
来源：http://axw.epnwcf.com

$s = match($x) { 1 => "一", default => "其他" };
来源：http://xhv.hnxiangtu.top

[U56] PHP：命名参数
来源：http://azq.fehbvm.com

f(a: 1, b: 2)
来源：http://bxm.haohaochexian.top

[U57] PHP：字符串插值
来源：http://xif.zhiwuduotai.top

"值: {$a}"
来源：http://yon.ivvv.top

[U58] PHP：数组三件套
来源：http://jwg.vqdsnc.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://yth.svipenyu.cn

[U59] PHP：自定义排序
来源：http://ldw.redwolf501.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://iqj.meibo888.top

[U60] PHP：JSON 编解码
来源：http://qot.tarul.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://pfk.nanxuanxn.top

[U61] PHP：正则
来源：http://hza.cucudq.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://bga.cqqwz.cn

[U62] PHP：日期对象
来源：http://qbk.dianchejie.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://cai.dashuyun.cn

[U63] PHP：文件读写
来源：http://ymx.chenzaomai.com

file_get_contents($f);  file_put_contents($f, $data);
来源：http://swt.epnwcf.com

[U64] PHP：目录遍历
来源：http://dky.shanyushiyangtech.top

glob("dir/*.php");  scandir("dir");
来源：http://ylh.mhx1999.top

[U65] PHP：会话
来源：http://fsu.zdbjq.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://hqf.hnqzz.top

[U66] PHP：设置 Cookie
来源：http://ijw.hcnkem.com

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://zjw.hywenlv.cn

[U67] PHP：处理文件上传
来源：http://pxl.hnxiangtu.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://owf.epnwcf.com

[U68] PHP：PDO 连接
来源：http://def.zhaomingkeji.xyz

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://zic.yfazqb.com

[U69] PHP：PDO 预处理
来源：http://uxi.uphjek.com

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://xyt.316326.xyz

[U70] PHP：PDO 事务
来源：http://lkp.pengpengdd.cyou

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://nhm.meibo888.top

[U71] PHP：抛出异常
来源：http://dvh.wangdashe.top

throw new RuntimeException("失败", 500);
来源：http://aaj.ydzc1.top

[U72] PHP：写错误日志
来源：http://ppj.bbcook.cn

error_log("失败: " . $e->getMessage());
来源：http://nub.tanke756.top

[U73] PHP：读取 ini 配置
来源：http://krg.shzxlz.cn

parse_ini_file("config.ini", true)
来源：http://iaf.tian-w.cn

[U74] PHP：读取环境变量
来源：http://nzv.haohaochexian.top

getenv("APP_ENV") ?: "production"
来源：http://asn.vqdsnc.cn

[U75] PHP：依赖注入
来源：http://csu.dianchejie.cn

composer require psr/container
来源：http://ipp.0kj1m.cn

[U76] PHP：简单路由
来源：http://hfi.zhaomingkeji.xyz

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://xpt.yfazqb.com

[U77] PHP：模板渲染
来源：http://gvu.yuanzhike.top

composer require twig/twig
来源：http://cqh.shanyushiyangkeji.top

[U78] PHP：单元测试
来源：http://owc.jinqigufen.top

composer require --dev phpunit/phpunit
来源：http://qja.svipenyu.cn

[U79] PHP：静态分析
来源：http://xcm.dianchejie.cn

composer require --dev phpstan/phpstan
来源：http://whv.ctjpmb.com

[U80] PHP：代码规范修复
来源：http://nfd.sufxvd.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://zis.daxiang520.top

[U81] JS：初始化项目
来源：http://fru.ivvv.top

npm init -y;  npm i express
来源：http://cdu.xingfuxueyuan.xyz

[U82] JS：package.json 脚本
来源：http://dqr.zhengqikj.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://bxe.haohaochexian.top

[U83] JS：ES Module 导入导出
来源：http://wfn.snrcjt.cn

export const a = 1;  import { a } from "./m.js";
来源：http://djh.hnqzz.top

[U84] JS：CommonJS 写法
来源：http://xvv.ywan-chungtsiang.top

module.exports = { a };  const { a } = require("./m");
来源：http://hhz.hnqzz.top

[U85] JS：可选链
来源：http://cuw.jyoumei.cn

a?.b?.c
来源：http://psp.sufxvd.cn

[U86] JS：空值合并
来源：http://kbb.kuanghao11.cn

a ?? b
来源：http://sjk.hesvh.cn

[U87] JS：解构默认值
来源：http://eyt.yfazqb.com

const { a = 1, b = 2 } = obj;
来源：http://hwl.svipenyu.cn

[U88] JS：对象展开合并
来源：http://kce.yuanzhike.top

{ ...a, ...b }
来源：http://gwc.wangshuangyany.cn

[U89] JS：数组去重
来源：http://jms.tarul.cn

[...new Set(arr)]
来源：http://ejq.nwbrower.top

[U90] JS：数字数组排序
来源：http://pep.yuxming.cn

[...arr].sort((a, b) => a - b)
来源：http://hxp.hammf.cn

[U91] JS：对象键值遍历
来源：http://bcg.sjlbkw.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://xan.chenzaomai.com

[U92] JS：深拷贝
来源：http://gke.ywan-chungtsiang.top

structuredClone(obj)
来源：http://lou.tianlin.xyz

[U93] JS：模板字符串
来源：http://qlz.yuanzhike.top

`共 ${n} 条`
来源：http://cjd.tianlin.xyz

[U94] JS：箭头函数
来源：http://rbg.jinqigufen.top

const double = x => x * 2;
来源：http://grj.aizwys.cn

[U95] JS：Promise 包装
来源：http://urv.daxiang520.top

new Promise((resolve, reject) => {})
来源：http://qoo.fktsv.cn

[U96] JS：async/await 与异常
来源：http://ctd.sysykeji.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://obt.ybcxt.top

[U97] JS：并发请求
来源：http://hft.nanxinkj.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://tpe.shanyushiyangkeji.top

[U98] JS：fetch 带 JSON
来源：http://yxd.cqqwz.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://fxl.hammf.cn

[U99] JS：事件监听
来源：http://aup.cheryme.top

el.addEventListener("click", e => {})
来源：http://mqb.yfazqb.com

[U100] JS：DOM 查询
来源：http://uel.epnwcf.com

document.querySelector(".item")
来源：http://woo.fktsv.cn

[U101] JS：classList 操作
来源：http://get.fehbvm.com

el.classList.toggle("active")
来源：http://fro.feifeiyinyue.top

[U102] JS：本地存储
来源：http://bbk.316326.xyz

localStorage.setItem("k", JSON.stringify(v))
来源：http://end.zhoulong.xyz

[U103] JS：定时器
来源：http://trg.feifeiyinyue.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://mma.daria6918.cn

[U104] JS：防抖
来源：http://ybx.dianchejie.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://bdp.shuidangran.top

[U105] JS：节流
来源：http://osp.zhoulong.xyz

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://zca.yuanzhike.top

[U106] JS：日期格式化
来源：http://xwh.vqdsnc.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://nfu.cdnleiting.top

[U107] JS：数字千分位
来源：http://xiw.yangfankeji.com

new Intl.NumberFormat("en-US").format(1234567)
来源：http://wqn.jianghu66.top

[U108] JS：随机整数
来源：http://kuh.cdnleiting.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://qhx.haohaochexian.top

[U109] JS：数组分组
来源：http://crg.xingfuxueyuan.xyz

Object.groupBy(arr, x => x.type)
来源：http://ude.zdbjq.cn

[U110] JS：数组分块
来源：http://cvg.zhixingplan.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://ppx.pengpengdd.cyou

[U111] JS：对象转 Map
来源：http://ryx.cqqwz.cn

new Map(Object.entries(obj))
来源：http://oqv.pengpengdd.cyou

[U112] JS：字符串补位
来源：http://bwd.yangfankeji.com

"7".padStart(3, "0")
来源：http://vqk.yj202588.top

[U113] JS：正则替换全部
来源：http://zlg.ydzc1.top

s.replaceAll("a", "b")
来源：http://rtk.yvedp.cn

[U114] JS：JSON 深比较
来源：http://dlf.cdnleiting.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://zzw.hammf.cn

[U115] JS：生成 UUID
来源：http://xmh.hysaishi.cn

crypto.randomUUID()
来源：http://udi.fehbvm.com

[U116] JS：类型检查（JSDoc）
来源：http://ias.hfpthk.cn

/** @param {string} name */ function f(name) {}
来源：http://uef.fehbvm.com

[U117] JS：单元测试
来源：http://hgv.nwbrower.top

npm i -D vitest;  npx vitest
来源：http://uqj.nanxinkj.top

[U118] JS：开发服务器
来源：http://voo.iojbl.cn

npm i -D vite;  npx vite
来源：http://wuj.uphjek.com

[U119] JS：生产构建
来源：http://pxc.jianghu66.top

npx vite build
来源：http://ypt.quarkkingdee.top

[U120] JS：读取环境变量（Vite）
来源：http://wak.vehdjk.com

import.meta.env.VITE_API_URL
来源：http://cly.zhiwuduotai.top

================================================================================
来源：http://inv.chenlongwang.top

统计汇总
来源：http://ugm.snrcjt.cn

================================================================================
来源：http://bni.tian-w.cn

按语言统计（条）：
来源：http://jvs.yongpay.top

Python ......... 252
来源：http://dmg.gzhubu.top

PHP ............ 252
来源：http://qve.yongpay.top

JavaScript ..... 252
来源：http://fbq.yuxming.cn

TypeScript ..... 212
来源：http://mqe.yuxming.cn

Java ........... 212
来源：http://rnc.jyoumei.cn

Go ............. 212
来源：http://wsj.xylfe.cn

Ruby ........... 212
来源：http://hjh.fengsongda.top

C# ............. 212
来源：http://pgr.jinqigfzy.top

C .............. 30
来源：http://ifg.ppjwa.cn

C++ ............ 30
来源：http://wgm.sweek.top

SQL ............ 90
来源：http://sbv.shangyingyoupin.top

Bash ........... 80
来源：http://ont.jinyuanbaomall.cn

Kotlin ......... 15
来源：http://mdb.hnqzz.top

Swift .......... 15
来源：http://bbz.9152youxi.cn

Lua ............ 10
来源：http://ogp.ppjwa.cn

Perl ........... 10
来源：http://dha.cucudq.cn

Scala .......... 10
来源：http://dkk.shanyushiyangtech.top

------------------------------------
来源：http://vte.epnwcf.com

合计 ........... 2106 条
来源：http://jck.haohaochexian.top

按章节统计：
来源：http://ntp.zhengqikj.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://auv.smart0.xyz

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://edf.uphjek.com

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://eqy.smart0.xyz

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://yik.dianchejie.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://slr.tian-w.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://ibg.tianlin.xyz

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://eev.hesvh.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://nsm.jqgfzy.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://aha.hywenlv.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://kch.cashguo.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://gfr.shuidangran.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://ozu.meibo888.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://uyt.jinqigfzy.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://pri.xinyue.icu

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://jyg.dashuyun.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://llf.tarul.cn

Q SQL 专题                              90
来源：http://nnb.cdnleiting.top

R Bash 专题                             80
来源：http://lvm.jinqigfzy.top

S C / C++ 专题                          60
来源：http://aye.ctjpmb.com

T 其他语言补充                          60
来源：http://dwm.aibaodan.cn

U 高频实用片段                         120
来源：http://rir.ydjk.org.cn

------------------------------------
来源：http://gos.aizwys.cn

合计                                  2106 条
来源：http://epk.yj20258.top

--------------------------------------------------------------------------------
来源：http://wyk.xziqi.cn

使用提醒
来源：http://wqd.zhaomingkeji.xyz

--------------------------------------------------------------------------------
来源：http://ndb.sweek.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://aqh.yj20258888.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://eoq.nwbrower.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://mbq.zhongyouzk.top

在旧版本上使用前请先确认语法支持情况。
来源：http://lmx.ywan-chungtsiang.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://lqw.andypj.xyz

—— 文件结束 ——
来源：http://jad.cashguo.top

================================================================================
来源：http://sos.sufxvd.cn

程序语言常见例子速查手册（2024 版）
来源：http://nfu.fanxiaobao.xyz

Common Programming Examples Cheat Book
来源：http://lbt.vqdsnc.cn

================================================================================
来源：http://xyu.0kj1m.cn


<!-- 参考信息 -->