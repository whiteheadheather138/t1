代发 wailian999

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://dxw.ctjpmb.com

================================================================================
来源：http://zjc.jianghu66.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://pkh.xingfuxueyuan.xyz

================================================================================
来源：http://frv.fzhhl.top

[U01] Py：创建虚拟环境
来源：http://cyy.ywan-chungtsiang.top

python -m venv .venv && source .venv/bin/activate
来源：http://afo.hongshengwenyu.top

[U02] Py：导出 / 安装依赖
来源：http://zze.jinqigufen.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://dur.gaohongyu789.top

[U03] Py：加载 .env 配置
来源：http://dhk.cucudq.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://bza.zhixingplan.top

[U04] Py：变量调试打印
来源：http://osy.chenlongwang.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://xzl.svipenyu.cn

[U05] Py：列表去重且保序
来源：http://obn.tarul.cn

list(dict.fromkeys(arr))
来源：http://qrg.xuanzx.com

[U06] Py：合并两个字典
来源：http://mbm.quarkkingdee.top

{**a, **b}
来源：http://ebj.xuanzx.com

[U07] Py：反转字典键值
来源：http://oft.bbcook.cn

{v: k for k, v in d.items()}
来源：http://qzi.hcnkem.com

[U08] Py：展平二维列表
来源：http://jhc.jinqigfzy.top

[y for x in nested for y in x]
来源：http://kko.jqgfzy.top

[U09] Py：字典取最大值的键
来源：http://lts.sysykeji.top

max(d, key=d.get)
来源：http://ftv.yj20258888.top

[U10] Py：按值排序字典
来源：http://nuf.yj20258.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://vti.jiagoushi.top

[U11] Py：生成器表达式
来源：http://hrh.yj202588.top

(x * 2 for x in arr)
来源：http://bxc.aizwys.cn

[U12] Py：取出现最多的 3 个元素
来源：http://xse.cheryme.top

Counter(arr).most_common(3)
来源：http://mwz.hnqzz.top

[U13] Py：固定长度队列
来源：http://vtm.fktsv.cn

deque(maxlen=10)
来源：http://stc.jyoumei.cn

[U14] Py：分组收集到列表
来源：http://aob.iojbl.cn

defaultdict(list)
来源：http://lgh.jyoumei.cn

[U15] Py：高精度计时
来源：http://cmq.jinqigfzy.top

t = time.perf_counter()
来源：http://jdm.vqdsnc.cn

[U16] Py：命令行参数解析
来源：http://olp.zdbjq.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://oia.wangshuangyany.cn

[U17] Py：初始化日志
来源：http://qpz.hnxiangtu.top

logging.basicConfig(level=logging.INFO)
来源：http://wfa.zhixingplan.top

[U18] Py：预编译正则
来源：http://agn.cheryme.top

pat = re.compile(r"\d+")
来源：http://jrm.jinqigufen.top

[U19] Py：正则替换带回调
来源：http://bib.yuanzhike.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://kjl.hammf.cn

[U20] Py：缓存函数结果
来源：http://wwg.ydzc1.top

@functools.lru_cache(maxsize=None)
来源：http://aiy.svipenyu.cn

[U21] Py：自定义上下文管理器
来源：http://jme.shanyushiyangkeji.top

@contextlib.contextmanager
来源：http://wjm.sysykeji.top

[U22] Py：矩阵转置
来源：http://jdt.ywan-chungtsiang.top

list(zip(*m))
来源：http://qiz.shuidangran.top

[U23] Py：分块读取大文件
来源：http://trw.andypj.xyz

for chunk in iter(lambda: f.read(8192), b""):
来源：http://mcn.svipenyu.cn

[U24] Py：路径操作
来源：http://zgn.nanxuanxn.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://eog.daxiang520.top

[U25] Py：CSV 按字典读
来源：http://irk.sweek.top

csv.DictReader(f)
来源：http://noa.jyoumei.cn

[U26] Py：并发下载
来源：http://rgs.sufxvd.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://dxf.0kj1m.cn

[U27] Py：异步 HTTP
来源：http://rrn.shanyushiyangkeji.top

aiohttp.ClientSession() 配合 async with
来源：http://jlq.bbcook.cn

[U28] Py：类型别名
来源：http://ftv.svipenyu.cn

UserId = int
来源：http://ozk.hnqzz.top

[U29] Py：属性校验
来源：http://xfn.jinqigufen.top

@property 与 @x.setter 配合
来源：http://hky.vqdsnc.cn

[U30] Py：数据类
来源：http://zbt.jinyuanbaomall.cn

@dataclass(slots=True)
来源：http://qnd.iojbl.cn

[U31] Py：单测
来源：http://zrv.gotoacloud.top

python -m pytest -q
来源：http://ntf.jqgufenzy.top

[U32] Py：代码格式化
来源：http://xae.ybcxt.top

ruff format . && ruff check --fix .
来源：http://nue.sufxvd.cn

[U33] Py：打包发布
来源：http://yxd.zhiwuduotai.top

python -m build  （依赖 pyproject.toml）
来源：http://bba.chenlongwang.top

[U34] Py：判断编码
来源：http://hla.redwolf501.top

chardet.detect(raw)
来源：http://jrm.xuetiantiany.cn

[U35] Py：发送邮件
来源：http://isu.wangdashe.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://fdr.ybcxt.top

[U36] Py：定时任务
来源：http://eyw.hfpthk.cn

schedule.every(10).minutes.do(job)
来源：http://vrp.yj20258.top

[U37] Py：读写 Excel
来源：http://vqp.fktsv.cn

pandas.read_excel / DataFrame.to_excel
来源：http://rvs.redwolf501.top

[U38] Py：获取脚本所在目录
来源：http://msh.jqgufenzy.top

Path(__file__).resolve().parent
来源：http://aoo.fengsongda.top

[U39] Py：判断是否在交互环境
来源：http://zcu.redwolf501.top

sys.stdout.isatty()
来源：http://nml.meibo888.top

[U40] Py：打印到标准错误
来源：http://gyr.iojbl.cn

print("err", file=sys.stderr)
来源：http://fro.shangyingyoupin.top

[U41] PHP：初始化 Composer 项目
来源：http://yly.yueranfly.top

composer init;  composer require guzzlehttp/guzzle
来源：http://ids.jyoumei.cn

[U42] PHP：PSR-4 自动加载
来源：http://rwp.yvedp.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://rcj.ybcxt.top

[U43] PHP：声明命名空间
来源：http://und.sysykeji.top

namespace App\Http;
来源：http://xen.jyoumei.cn

[U44] PHP：开启严格类型
来源：http://zid.gotoacloud.top

declare(strict_types=1);
来源：http://oic.hnqzz.top

[U45] PHP：类型声明与返回类型
来源：http://ubz.havefunace.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://qlc.yongpay.top

[U46] PHP：可空类型
来源：http://jmj.hongshengwenyu.top

?string $name = null
来源：http://uen.sxryk.cn

[U47] PHP：联合类型
来源：http://lbm.gzhubu.top

int|string $id
来源：http://yhf.ehwqpu.com

[U48] PHP：纯枚举
来源：http://jry.nanxuanxn.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://xvq.fanxiaobao.xyz

[U49] PHP：只读属性
来源：http://qxm.aizwys.cn

public readonly string $name
来源：http://weh.zycfv.cn

[U50] PHP：构造器属性提升
来源：http://rhj.zhaomingkeji.xyz

public function __construct(private int $id) {}
来源：http://bij.tianlin.xyz

[U51] PHP：数组解构
来源：http://hgw.shuidangran.top

[$a, $b] = $arr;
来源：http://mox.hammf.cn

[U52] PHP：箭头函数
来源：http://qvi.wangdashe.top

$double = fn($x) => $x * 2;
来源：http://sit.gaohongyu789.top

[U53] PHP：空合并运算符
来源：http://krh.hesvh.cn

$v = $a ?? $b ?? "default";
来源：http://cku.gaohongyu789.top

[U54] PHP：空安全调用
来源：http://bhj.jinqigufen.top

$obj?->method()
来源：http://nen.cashguo.top

[U55] PHP：match 表达式
来源：http://cjm.havefunace.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://poh.redwolf501.top

[U56] PHP：命名参数
来源：http://wph.yuxming.cn

f(a: 1, b: 2)
来源：http://jgs.zhaomingkeji.xyz

[U57] PHP：字符串插值
来源：http://eeb.hnqzz.top

"值: {$a}"
来源：http://djd.tianlin.xyz

[U58] PHP：数组三件套
来源：http://xns.chenlongwang.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://ygj.andypj.xyz

[U59] PHP：自定义排序
来源：http://reh.haohaochexian.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://xdh.shanyushiyangtech.top

[U60] PHP：JSON 编解码
来源：http://epq.dashuyun.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://pkp.gotoacloud.top

[U61] PHP：正则
来源：http://vus.fanxiaobao.xyz

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://cce.sufxvd.cn

[U62] PHP：日期对象
来源：http://tsq.hesvh.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://cga.ppjwa.cn

[U63] PHP：文件读写
来源：http://nke.52xcode.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://nfu.xuanzx.com

[U64] PHP：目录遍历
来源：http://gqh.redwolf501.top

glob("dir/*.php");  scandir("dir");
来源：http://bbw.jinqigfzy.top

[U65] PHP：会话
来源：http://sqs.zycfv.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://zet.fehbvm.com

[U66] PHP：设置 Cookie
来源：http://haj.xuanzx.com

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://hri.hammf.cn

[U67] PHP：处理文件上传
来源：http://oec.hammf.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://nzs.quarkkingdee.top

[U68] PHP：PDO 连接
来源：http://fyj.hnxiangtu.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://eqk.fehbvm.com

[U69] PHP：PDO 预处理
来源：http://epa.havefunace.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://smq.yuanzhike.top

[U70] PHP：PDO 事务
来源：http://rmv.hesvh.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://qlz.fehbvm.com

[U71] PHP：抛出异常
来源：http://fjd.aizwys.cn

throw new RuntimeException("失败", 500);
来源：http://ycc.ehwqpu.com

[U72] PHP：写错误日志
来源：http://cth.epnwcf.com

error_log("失败: " . $e->getMessage());
来源：http://utc.zhongyouzk.top

[U73] PHP：读取 ini 配置
来源：http://plh.haohaochexian.top

parse_ini_file("config.ini", true)
来源：http://qjo.yj20258.top

[U74] PHP：读取环境变量
来源：http://lrq.gzhubu.top

getenv("APP_ENV") ?: "production"
来源：http://yhk.guannengcc.top

[U75] PHP：依赖注入
来源：http://lcg.zhongyouzk.top

composer require psr/container
来源：http://ynx.jlsjyb.cn

[U76] PHP：简单路由
来源：http://rjs.feifeiyinyue.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://aez.nwbrower.top

[U77] PHP：模板渲染
来源：http://luy.gzhubu.top

composer require twig/twig
来源：http://lut.gaohongyu789.top

[U78] PHP：单元测试
来源：http://dqr.guannengcc.top

composer require --dev phpunit/phpunit
来源：http://vvs.hnxiangtu.top

[U79] PHP：静态分析
来源：http://eic.cdnleiting.top

composer require --dev phpstan/phpstan
来源：http://aik.yueranfly.top

[U80] PHP：代码规范修复
来源：http://fzi.fengsongda.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://zdi.xziqi.cn

[U81] JS：初始化项目
来源：http://kta.ctjpmb.com

npm init -y;  npm i express
来源：http://kax.ivvv.top

[U82] JS：package.json 脚本
来源：http://gpz.quarkkingdee.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://sja.fengsongda.top

[U83] JS：ES Module 导入导出
来源：http://cvu.daxiang520.top

export const a = 1;  import { a } from "./m.js";
来源：http://kmf.sweek.top

[U84] JS：CommonJS 写法
来源：http://bwp.kuanghao11.cn

module.exports = { a };  const { a } = require("./m");
来源：http://ppe.sjlbkw.cn

[U85] JS：可选链
来源：http://dzt.cucudq.cn

a?.b?.c
来源：http://nfl.xinyue.icu

[U86] JS：空值合并
来源：http://pzm.bjfxy.top

a ?? b
来源：http://rtf.xuetiantiany.cn

[U87] JS：解构默认值
来源：http://zra.bjfxy.top

const { a = 1, b = 2 } = obj;
来源：http://jze.yongpay.top

[U88] JS：对象展开合并
来源：http://krw.yueranfly.top

{ ...a, ...b }
来源：http://ole.yj202588.top

[U89] JS：数组去重
来源：http://sgh.yj202588.top

[...new Set(arr)]
来源：http://yrv.0kj1m.cn

[U90] JS：数字数组排序
来源：http://fww.jqgufenzy.top

[...arr].sort((a, b) => a - b)
来源：http://ywn.yangfankeji.com

[U91] JS：对象键值遍历
来源：http://jeg.jiagoushi.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://ymd.fktsv.cn

[U92] JS：深拷贝
来源：http://wzx.jinqigfzy.top

structuredClone(obj)
来源：http://fco.aibaodan.cn

[U93] JS：模板字符串
来源：http://uoq.guannengcc.top

`共 ${n} 条`
来源：http://crl.smart0.xyz

[U94] JS：箭头函数
来源：http://gys.yanxiufei.cn

const double = x => x * 2;
来源：http://srm.xuanzx.com

[U95] JS：Promise 包装
来源：http://xsq.xziqi.cn

new Promise((resolve, reject) => {})
来源：http://gme.xingfuxueyuan.xyz

[U96] JS：async/await 与异常
来源：http://fhc.zdbjq.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hub.andypj.xyz

[U97] JS：并发请求
来源：http://sva.sufxvd.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://vkk.gaohongyu789.top

[U98] JS：fetch 带 JSON
来源：http://xtp.hesvh.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://mrz.xuetiantiany.cn

[U99] JS：事件监听
来源：http://eld.ppjwa.cn

el.addEventListener("click", e => {})
来源：http://syo.gzhubu.top

[U100] JS：DOM 查询
来源：http://rhe.yj20258888.top

document.querySelector(".item")
来源：http://yqp.cashguo.top

[U101] JS：classList 操作
来源：http://vtt.yfazqb.com

el.classList.toggle("active")
来源：http://stl.tian-w.cn

[U102] JS：本地存储
来源：http://csg.zdqjudy.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://icy.zhiwuduotai.top

[U103] JS：定时器
来源：http://wkg.nanxuanxn.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://jwe.hysaishi.cn

[U104] JS：防抖
来源：http://wtp.hesvh.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://vdb.cashguo.top

[U105] JS：节流
来源：http://pen.ydzc1.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://bya.fanxiaobao.xyz

[U106] JS：日期格式化
来源：http://brc.fanxiaobao.xyz

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://qvn.daxiang520.top

[U107] JS：数字千分位
来源：http://bbt.fanxiaobao.xyz

new Intl.NumberFormat("en-US").format(1234567)
来源：http://igv.9152youxi.cn

[U108] JS：随机整数
来源：http://aom.fktsv.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://pjk.shangyingyoupin.top

[U109] JS：数组分组
来源：http://wgk.cucudq.cn

Object.groupBy(arr, x => x.type)
来源：http://jal.jinyuanbaomall.cn

[U110] JS：数组分块
来源：http://hkd.hesvh.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://zil.havefunace.top

[U111] JS：对象转 Map
来源：http://klv.aibaodan.cn

new Map(Object.entries(obj))
来源：http://rfv.yj20258.top

[U112] JS：字符串补位
来源：http://cbw.xuetiantiany.cn

"7".padStart(3, "0")
来源：http://uro.hammf.cn

[U113] JS：正则替换全部
来源：http://hta.snrcjt.cn

s.replaceAll("a", "b")
来源：http://koy.hnqzz.top

[U114] JS：JSON 深比较
来源：http://owl.xuanzx.com

JSON.stringify(a) === JSON.stringify(b)
来源：http://qtf.cashguo.top

[U115] JS：生成 UUID
来源：http://jlj.xylfe.cn

crypto.randomUUID()
来源：http://gac.zycfv.cn

[U116] JS：类型检查（JSDoc）
来源：http://fso.dianchejie.cn

/** @param {string} name */ function f(name) {}
来源：http://odn.kuanghao11.cn

[U117] JS：单元测试
来源：http://mln.cqqwz.cn

npm i -D vitest;  npx vitest
来源：http://nxe.hywenlv.cn

[U118] JS：开发服务器
来源：http://fqc.nwbrower.top

npm i -D vite;  npx vite
来源：http://egr.yongpay.top

[U119] JS：生产构建
来源：http://lvh.yj202588.top

npx vite build
来源：http://btk.fanxiaobao.xyz

[U120] JS：读取环境变量（Vite）
来源：http://lrk.zhoulong.xyz

import.meta.env.VITE_API_URL
来源：http://qoj.yuanzhike.top

================================================================================
来源：http://fls.guowangkeji.top

统计汇总
来源：http://nrb.jlsjyb.cn

================================================================================
来源：http://mai.tarul.cn

按语言统计（条）：
来源：http://oiy.redwolf501.top

Python ......... 252
来源：http://ezs.sjlbkw.cn

PHP ............ 252
来源：http://hnc.bbcook.cn

JavaScript ..... 252
来源：http://ujk.c1oappe.top

TypeScript ..... 212
来源：http://hoz.jqgufenzy.top

Java ........... 212
来源：http://uqv.yj20258.top

Go ............. 212
来源：http://oen.c1oappe.top

Ruby ........... 212
来源：http://uck.gogol.net.cn

C# ............. 212
来源：http://bvx.jinqigufen.top

C .............. 30
来源：http://afy.jlsjyb.cn

C++ ............ 30
来源：http://dqx.hysaishi.cn

SQL ............ 90
来源：http://ybf.xziqi.cn

Bash ........... 80
来源：http://qgs.gotoacloud.top

Kotlin ......... 15
来源：http://gvt.havefunace.top

Swift .......... 15
来源：http://dpj.cdnleiting.top

Lua ............ 10
来源：http://nky.xingfuxueyuan.xyz

Perl ........... 10
来源：http://tci.kuanghao11.cn

Scala .......... 10
来源：http://slr.yfazqb.com

------------------------------------
来源：http://agp.zhoulong.xyz

合计 ........... 2106 条
来源：http://quy.zhijiandao.cn

按章节统计：
来源：http://jpj.yongpay.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://gmb.ivvv.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://rli.iojbl.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://lda.chenjidiqi.icu

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://mjo.epnwcf.com

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://gmp.hnqzz.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://qrd.316326.xyz

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://amw.shanyushiyangtech.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://ckb.bjfxy.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://zds.shangyingyoupin.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://vvs.jiagoushi.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://kyf.cucudq.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://pee.yueranfly.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://jly.shangyingyoupin.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://hdb.xinyue.icu

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://ynu.fzhhl.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://vsp.yongpay.top

Q SQL 专题                              90
来源：http://tjv.tanke756.top

R Bash 专题                             80
来源：http://wcu.jinyuanbaomall.cn

S C / C++ 专题                          60
来源：http://myj.yj20258888.top

T 其他语言补充                          60
来源：http://scl.sysykeji.top

U 高频实用片段                         120
来源：http://efn.zdqjudy.top

------------------------------------
来源：http://bts.hnxiangtu.top

合计                                  2106 条
来源：http://kem.52xcode.cn

--------------------------------------------------------------------------------
来源：http://eqs.chenjidiqi.icu

使用提醒
来源：http://suw.jqgfzy.top

--------------------------------------------------------------------------------
来源：http://hhj.guowangkeji.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://qzv.ydzc1.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://chz.yj20258.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://xkq.xinyue.icu

在旧版本上使用前请先确认语法支持情况。
来源：http://xhh.xuanzx.com

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://jgi.xinyue.icu

—— 文件结束 ——
来源：http://wrt.tian-w.cn


<!-- 参考信息 -->