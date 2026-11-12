代发 wailian999

[U01] Py：创建虚拟环境
来源：http://qdl.dianchejie.cn

python -m venv .venv && source .venv/bin/activate
来源：http://axj.cqqwz.cn

[U02] Py：导出 / 安装依赖
来源：http://rdh.xylfe.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://sth.9152youxi.cn

[U03] Py：加载 .env 配置
来源：http://dfj.shuidangran.top

from dotenv import load_dotenv; load_dotenv()
来源：http://zlz.yj20258.top

[U04] Py：变量调试打印
来源：http://vej.yfazqb.com

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://flj.jinqigfzy.top

[U05] Py：列表去重且保序
来源：http://yqf.tianlin.xyz

list(dict.fromkeys(arr))
来源：http://nwu.chenjidiqi.icu

[U06] Py：合并两个字典
来源：http://oui.meibo888.top

{**a, **b}
来源：http://cxw.chenzaomai.com

[U07] Py：反转字典键值
来源：http://qxo.sxryk.cn

{v: k for k, v in d.items()}
来源：http://sgx.tarul.cn

[U08] Py：展平二维列表
来源：http://tfl.zhengqikj.top

[y for x in nested for y in x]
来源：http://stq.redwolf501.top

[U09] Py：字典取最大值的键
来源：http://vft.guannengcc.top

max(d, key=d.get)
来源：http://cun.hcnkem.com

[U10] Py：按值排序字典
来源：http://gfe.yj202588.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://nxn.hnxiangtu.top

[U11] Py：生成器表达式
来源：http://qud.cucudq.cn

(x * 2 for x in arr)
来源：http://ndu.shanyushiyangtech.top

[U12] Py：取出现最多的 3 个元素
来源：http://blh.tanke756.top

Counter(arr).most_common(3)
来源：http://drq.wangshuangyany.cn

[U13] Py：固定长度队列
来源：http://tip.feifeiyinyue.top

deque(maxlen=10)
来源：http://blq.ctjpmb.com

[U14] Py：分组收集到列表
来源：http://ztf.tanke756.top

defaultdict(list)
来源：http://gue.daria6918.cn

[U15] Py：高精度计时
来源：http://rfr.hywenlv.cn

t = time.perf_counter()
来源：http://ito.chenlongwang.top

[U16] Py：命令行参数解析
来源：http://owk.wangshuangyany.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://zmq.zdqjudy.top

[U17] Py：初始化日志
来源：http://siq.ivvv.top

logging.basicConfig(level=logging.INFO)
来源：http://zcs.quarkkingdee.top

[U18] Py：预编译正则
来源：http://zir.shuidangran.top

pat = re.compile(r"\d+")
来源：http://qhn.yj20258888.top

[U19] Py：正则替换带回调
来源：http://wvb.chenjidiqi.icu

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hyy.shuidangran.top

[U20] Py：缓存函数结果
来源：http://hmi.vqdsnc.cn

@functools.lru_cache(maxsize=None)
来源：http://xuy.cucudq.cn

[U21] Py：自定义上下文管理器
来源：http://nwc.bjfxy.top

@contextlib.contextmanager
来源：http://ccx.zhoulong.xyz

[U22] Py：矩阵转置
来源：http://qba.xinyue.icu

list(zip(*m))
来源：http://ydx.zhijiandao.cn

[U23] Py：分块读取大文件
来源：http://exi.gaohongyu789.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://vua.redwolf501.top

[U24] Py：路径操作
来源：http://xbs.ydjk.org.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://vnj.52xcode.cn

[U25] Py：CSV 按字典读
来源：http://imv.gotoacloud.top

csv.DictReader(f)
来源：http://rhk.c1oappe.top

[U26] Py：并发下载
来源：http://fag.aibaodan.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://sfx.mhx1999.top

[U27] Py：异步 HTTP
来源：http://zow.tianlin.xyz

aiohttp.ClientSession() 配合 async with
来源：http://ddg.yuanzhike.top

[U28] Py：类型别名
来源：http://vxd.gogol.net.cn

UserId = int
来源：http://mpp.c1oappe.top

[U29] Py：属性校验
来源：http://whz.316326.xyz

@property 与 @x.setter 配合
来源：http://ang.chenjidiqi.icu

[U30] Py：数据类
来源：http://ugx.jinghuilouyu.cn

@dataclass(slots=True)
来源：http://ofu.hesvh.cn

[U31] Py：单测
来源：http://sey.jqgfzy.top

python -m pytest -q
来源：http://yin.aizwys.cn

[U32] Py：代码格式化
来源：http://hsl.hysaishi.cn

ruff format . && ruff check --fix .
来源：http://zxr.cucudq.cn

[U33] Py：打包发布
来源：http://ieo.jianghu66.top

python -m build  （依赖 pyproject.toml）
来源：http://ehy.haohaochexian.top

[U34] Py：判断编码
来源：http://vvh.pengpengdd.cyou

chardet.detect(raw)
来源：http://huv.shzxlz.cn

[U35] Py：发送邮件
来源：http://waj.dianchejie.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://ata.ywan-chungtsiang.top

[U36] Py：定时任务
来源：http://vbk.yuxming.cn

schedule.every(10).minutes.do(job)
来源：http://twd.yonumen.top

[U37] Py：读写 Excel
来源：http://yjn.hnxiangtu.top

pandas.read_excel / DataFrame.to_excel
来源：http://rjl.fengsongda.top

[U38] Py：获取脚本所在目录
来源：http://utl.iojbl.cn

Path(__file__).resolve().parent
来源：http://tpw.zhengqikj.top

[U39] Py：判断是否在交互环境
来源：http://iee.nwbrower.top

sys.stdout.isatty()
来源：http://ysu.jlsjyb.cn

[U40] Py：打印到标准错误
来源：http://wwc.zhijiandao.cn

print("err", file=sys.stderr)
来源：http://muf.zhengqikj.top

[U41] PHP：初始化 Composer 项目
来源：http://lvl.zhixingplan.top

composer init;  composer require guzzlehttp/guzzle
来源：http://ier.xinyue.icu

[U42] PHP：PSR-4 自动加载
来源：http://rlj.meibo888.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://yvl.cheryme.top

[U43] PHP：声明命名空间
来源：http://ddr.shanyushiyangtech.top

namespace App\Http;
来源：http://ivy.ybcxt.top

[U44] PHP：开启严格类型
来源：http://bna.zhaomingkeji.xyz

declare(strict_types=1);
来源：http://kay.vehdjk.com

[U45] PHP：类型声明与返回类型
来源：http://hvy.epnwcf.com

function add(int $a, int $b): int { return $a + $b; }
来源：http://dzz.sufxvd.cn

[U46] PHP：可空类型
来源：http://rmg.tarul.cn

?string $name = null
来源：http://hrh.guowangkeji.top

[U47] PHP：联合类型
来源：http://kvb.hywenlv.cn

int|string $id
来源：http://jat.ybcxt.top

[U48] PHP：纯枚举
来源：http://fyi.hongshengwenyu.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://uiw.cheryme.top

[U49] PHP：只读属性
来源：http://pjm.jinyuanbaomall.cn

public readonly string $name
来源：http://gdc.xziqi.cn

[U50] PHP：构造器属性提升
来源：http://jbz.yanxiufei.cn

public function __construct(private int $id) {}
来源：http://olj.dashuyun.cn

[U51] PHP：数组解构
来源：http://cei.smart0.xyz

[$a, $b] = $arr;
来源：http://haj.zhengqikj.top

[U52] PHP：箭头函数
来源：http://ohh.jyoumei.cn

$double = fn($x) => $x * 2;
来源：http://zcz.shzxlz.cn

[U53] PHP：空合并运算符
来源：http://ncu.9152youxi.cn

$v = $a ?? $b ?? "default";
来源：http://sqd.0kj1m.cn

[U54] PHP：空安全调用
来源：http://vjc.chenlongwang.top

$obj?->method()
来源：http://gok.hammf.cn

[U55] PHP：match 表达式
来源：http://csi.zhiwuduotai.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://gwq.yangfankeji.com

[U56] PHP：命名参数
来源：http://vug.jqgufenzy.top

f(a: 1, b: 2)
来源：http://ryo.zhongyouzk.top

[U57] PHP：字符串插值
来源：http://ifp.feifeiyinyue.top

"值: {$a}"
来源：http://flp.mhx1999.top

[U58] PHP：数组三件套
来源：http://iku.smart0.xyz

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://fpc.tian-w.cn

[U59] PHP：自定义排序
来源：http://pvd.bjfxy.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://fvg.hnxiangtu.top

[U60] PHP：JSON 编解码
来源：http://kwf.xziqi.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://wre.bjfxy.top

[U61] PHP：正则
来源：http://uid.zdqjudy.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://xai.hesvh.cn

[U62] PHP：日期对象
来源：http://xgw.daxiang520.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://rov.zhoulong.xyz

[U63] PHP：文件读写
来源：http://ror.jinqigfzy.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://rxl.guannengcc.top

[U64] PHP：目录遍历
来源：http://ptf.fengsongda.top

glob("dir/*.php");  scandir("dir");
来源：http://cmj.tianlin.xyz

[U65] PHP：会话
来源：http://fcu.ybcxt.top

session_start();  $_SESSION["uid"] = 1;
来源：http://alf.gzhubu.top

[U66] PHP：设置 Cookie
来源：http://qub.zdbjq.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://wyv.svipenyu.cn

[U67] PHP：处理文件上传
来源：http://dgu.9152youxi.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://wat.sweek.top

[U68] PHP：PDO 连接
来源：http://gfe.xinyue.icu

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://gnn.kuanghao11.cn

[U69] PHP：PDO 预处理
来源：http://zbh.fehbvm.com

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://ryb.dianchejie.cn

[U70] PHP：PDO 事务
来源：http://ivd.iojbl.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://awt.jinyuanbaomall.cn

[U71] PHP：抛出异常
来源：http://gqd.aibaodan.cn

throw new RuntimeException("失败", 500);
来源：http://lsz.xylfe.cn

[U72] PHP：写错误日志
来源：http://hvw.yj20258.top

error_log("失败: " . $e->getMessage());
来源：http://wtk.yj20258.top

[U73] PHP：读取 ini 配置
来源：http://uwo.shanyushiyangkeji.top

parse_ini_file("config.ini", true)
来源：http://yfa.xinyue.icu

[U74] PHP：读取环境变量
来源：http://hkv.epnwcf.com

getenv("APP_ENV") ?: "production"
来源：http://llc.zhoulong.xyz

[U75] PHP：依赖注入
来源：http://rbu.jianghu66.top

composer require psr/container
来源：http://stu.nanxinkj.top

[U76] PHP：简单路由
来源：http://anc.kuanghao11.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://hhy.bjfxy.top

[U77] PHP：模板渲染
来源：http://jsp.dianchejie.cn

composer require twig/twig
来源：http://ijd.yj202588.top

[U78] PHP：单元测试
来源：http://rly.fanxiaobao.xyz

composer require --dev phpunit/phpunit
来源：http://fgz.sweek.top

[U79] PHP：静态分析
来源：http://wlf.jinghuilouyu.cn

composer require --dev phpstan/phpstan
来源：http://ier.cheryme.top

[U80] PHP：代码规范修复
来源：http://rbh.sufxvd.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://sft.yj20258888.top

[U81] JS：初始化项目
来源：http://ivh.vqdsnc.cn

npm init -y;  npm i express
来源：http://jgq.wangdashe.top

[U82] JS：package.json 脚本
来源：http://hkz.yanxiufei.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://hqj.hfpthk.cn

[U83] JS：ES Module 导入导出
来源：http://nal.ywan-chungtsiang.top

export const a = 1;  import { a } from "./m.js";
来源：http://cpf.vqdsnc.cn

[U84] JS：CommonJS 写法
来源：http://ejc.yangfankeji.com

module.exports = { a };  const { a } = require("./m");
来源：http://gqi.wangshuangyany.cn

[U85] JS：可选链
来源：http://qbr.ybcxt.top

a?.b?.c
来源：http://cht.sjlbkw.cn

[U86] JS：空值合并
来源：http://lvr.sysykeji.top

a ?? b
来源：http://hyu.zycfv.cn

[U87] JS：解构默认值
来源：http://cow.feifeiyinyue.top

const { a = 1, b = 2 } = obj;
来源：http://fca.guowangkeji.top

[U88] JS：对象展开合并
来源：http://kjt.ydzc1.top

{ ...a, ...b }
来源：http://hzd.chenlongwang.top

[U89] JS：数组去重
来源：http://giv.cheryme.top

[...new Set(arr)]
来源：http://gdf.jinghuilouyu.cn

[U90] JS：数字数组排序
来源：http://cnu.snrcjt.cn

[...arr].sort((a, b) => a - b)
来源：http://miv.gogol.net.cn

[U91] JS：对象键值遍历
来源：http://vtm.9152youxi.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://ueo.yongpay.top

[U92] JS：深拷贝
来源：http://dxs.shuidangran.top

structuredClone(obj)
来源：http://rwn.xylfe.cn

[U93] JS：模板字符串
来源：http://meb.shuidangran.top

`共 ${n} 条`
来源：http://ajm.xinyue.icu

[U94] JS：箭头函数
来源：http://dgt.sweek.top

const double = x => x * 2;
来源：http://pvo.chenlongwang.top

[U95] JS：Promise 包装
来源：http://uni.yuxming.cn

new Promise((resolve, reject) => {})
来源：http://jrx.svipenyu.cn

[U96] JS：async/await 与异常
来源：http://mdu.yj20258.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://dwn.aibaodan.cn

[U97] JS：并发请求
来源：http://uob.tarul.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://jfw.snrcjt.cn

[U98] JS：fetch 带 JSON
来源：http://kza.zhiwuduotai.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://abi.cucudq.cn

[U99] JS：事件监听
来源：http://pvz.nanxuanxn.top

el.addEventListener("click", e => {})
来源：http://btv.jqgufenzy.top

[U100] JS：DOM 查询
来源：http://vpi.zycfv.cn

document.querySelector(".item")
来源：http://nxb.yuanzhike.top

[U101] JS：classList 操作
来源：http://vgn.hammf.cn

el.classList.toggle("active")
来源：http://hht.tanke756.top

[U102] JS：本地存储
来源：http://frc.ydzc1.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://rcz.yvedp.cn

[U103] JS：定时器
来源：http://hpr.zdbjq.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://trh.dashuyun.cn

[U104] JS：防抖
来源：http://grg.yuxming.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://prl.c1oappe.top

[U105] JS：节流
来源：http://wus.ybcxt.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hjp.gogol.net.cn

[U106] JS：日期格式化
来源：http://kug.jinyuanbaomall.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://ilb.ctjpmb.com

[U107] JS：数字千分位
来源：http://xxq.yuanzhike.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://xpg.fanxiaobao.xyz

[U108] JS：随机整数
来源：http://lnp.mhx1999.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://zdd.jqgfzy.top

[U109] JS：数组分组
来源：http://pww.birdmap.top

Object.groupBy(arr, x => x.type)
来源：http://fre.316326.xyz

[U110] JS：数组分块
来源：http://osw.52xcode.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://ruv.yongpay.top

[U111] JS：对象转 Map
来源：http://cqm.jianghu66.top

new Map(Object.entries(obj))
来源：http://nff.yuanzhike.top

[U112] JS：字符串补位
来源：http://icj.gaohongyu789.top

"7".padStart(3, "0")
来源：http://poc.nanxinkj.top

[U113] JS：正则替换全部
来源：http://anu.quarkkingdee.top

s.replaceAll("a", "b")
来源：http://jih.yanxiufei.cn

[U114] JS：JSON 深比较
来源：http://bmt.cqqwz.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://gal.epnwcf.com

[U115] JS：生成 UUID
来源：http://kcl.iojbl.cn

crypto.randomUUID()
来源：http://wun.svipenyu.cn

[U116] JS：类型检查（JSDoc）
来源：http://jlg.cdnleiting.top

/** @param {string} name */ function f(name) {}
来源：http://ssb.ydjk.org.cn

[U117] JS：单元测试
来源：http://quo.sxryk.cn

npm i -D vitest;  npx vitest
来源：http://ehu.fehbvm.com

[U118] JS：开发服务器
来源：http://vpc.yvedp.cn

npm i -D vite;  npx vite
来源：http://snu.havefunace.top

[U119] JS：生产构建
来源：http://exw.shanyushiyangkeji.top

npx vite build
来源：http://cni.chenlongwang.top

[U120] JS：读取环境变量（Vite）
来源：http://erj.dianchejie.cn

import.meta.env.VITE_API_URL
来源：http://amj.tanke756.top

================================================================================
来源：http://swk.tian-w.cn

统计汇总
来源：http://wbn.epnwcf.com

================================================================================
来源：http://ujl.ydjk.org.cn

按语言统计（条）：
来源：http://nhz.andypj.xyz

Python ......... 252
来源：http://uqy.guowangkeji.top

PHP ............ 252
来源：http://jgx.yfazqb.com

JavaScript ..... 252
来源：http://idp.hysaishi.cn

TypeScript ..... 212
来源：http://axe.jinqigfzy.top

Java ........... 212
来源：http://djr.feifeiyinyue.top

Go ............. 212
来源：http://gve.dianchejie.cn

Ruby ........... 212
来源：http://rpj.redwolf501.top

C# ............. 212
来源：http://zml.shzxlz.cn

C .............. 30
来源：http://xsv.xingfuxueyuan.xyz

C++ ............ 30
来源：http://yeq.shanyushiyangtech.top

SQL ............ 90
来源：http://tvh.hongshengwenyu.top

Bash ........... 80
来源：http://zaw.zhengqikj.top

Kotlin ......... 15
来源：http://sxq.aibaodan.cn

Swift .......... 15
来源：http://vte.zhiwuduotai.top

Lua ............ 10
来源：http://zxw.pycfn.com

Perl ........... 10
来源：http://seq.quarkkingdee.top

Scala .......... 10
来源：http://maj.xinyue.icu

------------------------------------
来源：http://fla.316326.xyz

合计 ........... 2106 条
来源：http://ylx.ydjk.org.cn

按章节统计：
来源：http://bol.redwolf501.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://zxk.xuanzx.com

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://per.tian-w.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://tqa.sweek.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://soz.9152youxi.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://meu.birdmap.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://ofg.zhongyouzk.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://joo.xinyue.icu

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://jif.daxiang520.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://yan.redwolf501.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://nfe.zhongyouzk.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://gjr.nanxuanxn.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://yjy.yuanzhike.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://qok.aibaodan.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://tqd.tarul.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://nkn.yfazqb.com

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://tec.jqgfzy.top

Q SQL 专题                              90
来源：http://iai.gzhubu.top

R Bash 专题                             80
来源：http://gms.ehwqpu.com

S C / C++ 专题                          60
来源：http://emz.zhaomingkeji.xyz

T 其他语言补充                          60
来源：http://vwa.jinyuanbaomall.cn

U 高频实用片段                         120
来源：http://eic.kuanghao11.cn

------------------------------------
来源：http://izd.jqgufenzy.top

合计                                  2106 条
来源：http://ylg.yuxming.cn

--------------------------------------------------------------------------------
来源：http://lun.wangdashe.top

使用提醒
来源：http://lod.chenlongwang.top

--------------------------------------------------------------------------------
来源：http://lgf.daxiang520.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://jrt.jqgfzy.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://bcw.daxiang520.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://yii.mhx1999.top

在旧版本上使用前请先确认语法支持情况。
来源：http://lzx.gzhubu.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://ndv.tarul.cn

—— 文件结束 ——
来源：http://uhk.gaohongyu789.top

================================================================================
来源：http://zyl.shuidangran.top

程序语言常见例子速查手册（2024 版）
来源：http://llw.hysaishi.cn

Common Programming Examples Cheat Book
来源：http://cvy.mhx1999.top

================================================================================
来源：http://kad.tarul.cn


<!-- 参考信息 -->