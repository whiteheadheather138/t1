代发 wailian999

[U01] Py：创建虚拟环境
来源：http://enk.ywan-chungtsiang.top

python -m venv .venv && source .venv/bin/activate
来源：http://icw.jyoumei.cn

[U02] Py：导出 / 安装依赖
来源：http://exv.guannengcc.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://clf.feifeiyinyue.top

[U03] Py：加载 .env 配置
来源：http://qqg.sjlbkw.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://eut.sufxvd.cn

[U04] Py：变量调试打印
来源：http://iyi.dashuyun.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://esy.zhiwuduotai.top

[U05] Py：列表去重且保序
来源：http://soz.yonumen.top

list(dict.fromkeys(arr))
来源：http://jws.jinqigfzy.top

[U06] Py：合并两个字典
来源：http://ovq.ehwqpu.com

{**a, **b}
来源：http://ndw.zhixingplan.top

[U07] Py：反转字典键值
来源：http://nnj.uphjek.com

{v: k for k, v in d.items()}
来源：http://etw.pengpengdd.cyou

[U08] Py：展平二维列表
来源：http://piu.shangyingyoupin.top

[y for x in nested for y in x]
来源：http://jzn.shuidangran.top

[U09] Py：字典取最大值的键
来源：http://bod.xylfe.cn

max(d, key=d.get)
来源：http://tmf.yangfankeji.com

[U10] Py：按值排序字典
来源：http://hbh.ybcxt.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://xcd.ctjpmb.com

[U11] Py：生成器表达式
来源：http://zsm.zdbjq.cn

(x * 2 for x in arr)
来源：http://imn.uphjek.com

[U12] Py：取出现最多的 3 个元素
来源：http://oof.hnxiangtu.top

Counter(arr).most_common(3)
来源：http://non.vqdsnc.cn

[U13] Py：固定长度队列
来源：http://rdh.52xcode.cn

deque(maxlen=10)
来源：http://gvj.hnqzz.top

[U14] Py：分组收集到列表
来源：http://qaf.wangshuangyany.cn

defaultdict(list)
来源：http://unu.chenlongwang.top

[U15] Py：高精度计时
来源：http://lds.hysaishi.cn

t = time.perf_counter()
来源：http://noo.guowangkeji.top

[U16] Py：命令行参数解析
来源：http://uri.aibaodan.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://mqj.fehbvm.com

[U17] Py：初始化日志
来源：http://drp.yj20258888.top

logging.basicConfig(level=logging.INFO)
来源：http://dry.epnwcf.com

[U18] Py：预编译正则
来源：http://ivk.daria6918.cn

pat = re.compile(r"\d+")
来源：http://mql.andypj.xyz

[U19] Py：正则替换带回调
来源：http://jwg.zhijiandao.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://asz.hesvh.cn

[U20] Py：缓存函数结果
来源：http://xmy.hammf.cn

@functools.lru_cache(maxsize=None)
来源：http://cse.nwbrower.top

[U21] Py：自定义上下文管理器
来源：http://whe.uphjek.com

@contextlib.contextmanager
来源：http://uic.shzxlz.cn

[U22] Py：矩阵转置
来源：http://fkt.sufxvd.cn

list(zip(*m))
来源：http://kxb.jinyuanbaomall.cn

[U23] Py：分块读取大文件
来源：http://bay.jinqigufen.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://jkt.epnwcf.com

[U24] Py：路径操作
来源：http://hcf.vehdjk.com

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://ubb.ydzc1.top

[U25] Py：CSV 按字典读
来源：http://erb.shanyushiyangkeji.top

csv.DictReader(f)
来源：http://tvo.ydzc1.top

[U26] Py：并发下载
来源：http://zbx.iojbl.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://ufo.yonumen.top

[U27] Py：异步 HTTP
来源：http://hya.yongpay.top

aiohttp.ClientSession() 配合 async with
来源：http://rng.dianchejie.cn

[U28] Py：类型别名
来源：http://fww.bjfxy.top

UserId = int
来源：http://gyq.chenjidiqi.icu

[U29] Py：属性校验
来源：http://sof.hongshengwenyu.top

@property 与 @x.setter 配合
来源：http://ybg.jinghuilouyu.cn

[U30] Py：数据类
来源：http://mnt.uphjek.com

@dataclass(slots=True)
来源：http://ijg.hfpthk.cn

[U31] Py：单测
来源：http://urj.yongpay.top

python -m pytest -q
来源：http://afv.yanxiufei.cn

[U32] Py：代码格式化
来源：http://alq.tianlin.xyz

ruff format . && ruff check --fix .
来源：http://ita.yuxming.cn

[U33] Py：打包发布
来源：http://est.fanxiaobao.xyz

python -m build  （依赖 pyproject.toml）
来源：http://ohw.ivvv.top

[U34] Py：判断编码
来源：http://stt.gotoacloud.top

chardet.detect(raw)
来源：http://lzk.fanxiaobao.xyz

[U35] Py：发送邮件
来源：http://pgj.hnxiangtu.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://wwd.cashguo.top

[U36] Py：定时任务
来源：http://ymj.shangyingyoupin.top

schedule.every(10).minutes.do(job)
来源：http://lnx.yangfankeji.com

[U37] Py：读写 Excel
来源：http://tpe.vehdjk.com

pandas.read_excel / DataFrame.to_excel
来源：http://ido.yvedp.cn

[U38] Py：获取脚本所在目录
来源：http://ifc.birdmap.top

Path(__file__).resolve().parent
来源：http://vbs.guannengcc.top

[U39] Py：判断是否在交互环境
来源：http://tkf.jinqigufen.top

sys.stdout.isatty()
来源：http://pap.yuanzhike.top

[U40] Py：打印到标准错误
来源：http://rjr.haohaochexian.top

print("err", file=sys.stderr)
来源：http://fxv.wangshuangyany.cn

[U41] PHP：初始化 Composer 项目
来源：http://pra.shanyushiyangkeji.top

composer init;  composer require guzzlehttp/guzzle
来源：http://qcf.ywan-chungtsiang.top

[U42] PHP：PSR-4 自动加载
来源：http://jcb.shanyushiyangkeji.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://wbs.andypj.xyz

[U43] PHP：声明命名空间
来源：http://ngq.ctjpmb.com

namespace App\Http;
来源：http://zki.ctjpmb.com

[U44] PHP：开启严格类型
来源：http://eht.0kj1m.cn

declare(strict_types=1);
来源：http://jzj.daxiang520.top

[U45] PHP：类型声明与返回类型
来源：http://vjv.shanyushiyangkeji.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://krc.jyoumei.cn

[U46] PHP：可空类型
来源：http://rrt.zhixingplan.top

?string $name = null
来源：http://jvm.yvedp.cn

[U47] PHP：联合类型
来源：http://zea.shuidangran.top

int|string $id
来源：http://qpl.iojbl.cn

[U48] PHP：纯枚举
来源：http://lat.guowangkeji.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://sjm.jinqigfzy.top

[U49] PHP：只读属性
来源：http://xpn.wangdashe.top

public readonly string $name
来源：http://aid.jinqigufen.top

[U50] PHP：构造器属性提升
来源：http://pfz.zdbjq.cn

public function __construct(private int $id) {}
来源：http://ueo.xuetiantiany.cn

[U51] PHP：数组解构
来源：http://qom.hammf.cn

[$a, $b] = $arr;
来源：http://csm.shanyushiyangkeji.top

[U52] PHP：箭头函数
来源：http://ien.bbcook.cn

$double = fn($x) => $x * 2;
来源：http://qzq.fengsongda.top

[U53] PHP：空合并运算符
来源：http://ydz.chenjidiqi.icu

$v = $a ?? $b ?? "default";
来源：http://gwg.sxryk.cn

[U54] PHP：空安全调用
来源：http://kni.ctjpmb.com

$obj?->method()
来源：http://wrl.zhiwuduotai.top

[U55] PHP：match 表达式
来源：http://ltf.hammf.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://opb.cqqwz.cn

[U56] PHP：命名参数
来源：http://npn.fengsongda.top

f(a: 1, b: 2)
来源：http://gef.yj20258888.top

[U57] PHP：字符串插值
来源：http://hzd.redwolf501.top

"值: {$a}"
来源：http://ttg.gotoacloud.top

[U58] PHP：数组三件套
来源：http://nnv.yj202588.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://rwp.jqgufenzy.top

[U59] PHP：自定义排序
来源：http://gmm.zdbjq.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://gdd.yj20258.top

[U60] PHP：JSON 编解码
来源：http://zjv.hfpthk.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://pmu.chenzaomai.com

[U61] PHP：正则
来源：http://vvz.xinyue.icu

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://wzn.zhoulong.xyz

[U62] PHP：日期对象
来源：http://eda.vqdsnc.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://gij.sweek.top

[U63] PHP：文件读写
来源：http://oyd.nanxinkj.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://ufy.yj20258888.top

[U64] PHP：目录遍历
来源：http://oyy.epnwcf.com

glob("dir/*.php");  scandir("dir");
来源：http://pqf.guowangkeji.top

[U65] PHP：会话
来源：http://cqw.fengsongda.top

session_start();  $_SESSION["uid"] = 1;
来源：http://pjt.zdbjq.cn

[U66] PHP：设置 Cookie
来源：http://xsd.cucudq.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://qxa.jqgufenzy.top

[U67] PHP：处理文件上传
来源：http://rwa.jinqigfzy.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://vrk.yj20258888.top

[U68] PHP：PDO 连接
来源：http://edp.ydjk.org.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://oon.quarkkingdee.top

[U69] PHP：PDO 预处理
来源：http://okp.sysykeji.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://ysz.9152youxi.cn

[U70] PHP：PDO 事务
来源：http://gom.yfazqb.com

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://jxc.ydzc1.top

[U71] PHP：抛出异常
来源：http://lzc.hnqzz.top

throw new RuntimeException("失败", 500);
来源：http://znf.xuetiantiany.cn

[U72] PHP：写错误日志
来源：http://ncc.hcnkem.com

error_log("失败: " . $e->getMessage());
来源：http://owh.pycfn.com

[U73] PHP：读取 ini 配置
来源：http://qsw.bjfxy.top

parse_ini_file("config.ini", true)
来源：http://trm.nanxuanxn.top

[U74] PHP：读取环境变量
来源：http://icg.zdqjudy.top

getenv("APP_ENV") ?: "production"
来源：http://gnp.sjlbkw.cn

[U75] PHP：依赖注入
来源：http://xsk.meibo888.top

composer require psr/container
来源：http://acj.smart0.xyz

[U76] PHP：简单路由
来源：http://tcv.chenjidiqi.icu

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://dvn.quarkkingdee.top

[U77] PHP：模板渲染
来源：http://bbw.xuanzx.com

composer require twig/twig
来源：http://gwo.sjlbkw.cn

[U78] PHP：单元测试
来源：http://lnc.yueranfly.top

composer require --dev phpunit/phpunit
来源：http://nbx.gogol.net.cn

[U79] PHP：静态分析
来源：http://iwy.chenzaomai.com

composer require --dev phpstan/phpstan
来源：http://gbf.shanyushiyangtech.top

[U80] PHP：代码规范修复
来源：http://kml.hfpthk.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://two.bbcook.cn

[U81] JS：初始化项目
来源：http://ujq.xylfe.cn

npm init -y;  npm i express
来源：http://ivm.cucudq.cn

[U82] JS：package.json 脚本
来源：http://vbu.uphjek.com

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://bts.guannengcc.top

[U83] JS：ES Module 导入导出
来源：http://wfl.gzhubu.top

export const a = 1;  import { a } from "./m.js";
来源：http://qjx.hnxiangtu.top

[U84] JS：CommonJS 写法
来源：http://bem.316326.xyz

module.exports = { a };  const { a } = require("./m");
来源：http://oxs.gotoacloud.top

[U85] JS：可选链
来源：http://udn.jianghu66.top

a?.b?.c
来源：http://naq.yuanzhike.top

[U86] JS：空值合并
来源：http://ifg.fehbvm.com

a ?? b
来源：http://amt.yonumen.top

[U87] JS：解构默认值
来源：http://bdw.mhx1999.top

const { a = 1, b = 2 } = obj;
来源：http://kli.tarul.cn

[U88] JS：对象展开合并
来源：http://wdh.wangdashe.top

{ ...a, ...b }
来源：http://src.yanxiufei.cn

[U89] JS：数组去重
来源：http://qms.guowangkeji.top

[...new Set(arr)]
来源：http://hks.jinyuanbaomall.cn

[U90] JS：数字数组排序
来源：http://aiq.kuanghao11.cn

[...arr].sort((a, b) => a - b)
来源：http://mwt.xziqi.cn

[U91] JS：对象键值遍历
来源：http://slu.tian-w.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://jsv.shanyushiyangkeji.top

[U92] JS：深拷贝
来源：http://seg.wangdashe.top

structuredClone(obj)
来源：http://qaf.aizwys.cn

[U93] JS：模板字符串
来源：http://jha.quarkkingdee.top

`共 ${n} 条`
来源：http://ybs.gotoacloud.top

[U94] JS：箭头函数
来源：http://dxg.dashuyun.cn

const double = x => x * 2;
来源：http://jmu.meibo888.top

[U95] JS：Promise 包装
来源：http://wqk.zhijiandao.cn

new Promise((resolve, reject) => {})
来源：http://boi.nanxinkj.top

[U96] JS：async/await 与异常
来源：http://vgf.gotoacloud.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://erd.chenzaomai.com

[U97] JS：并发请求
来源：http://emb.yonumen.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://piw.chenjidiqi.icu

[U98] JS：fetch 带 JSON
来源：http://enp.gogol.net.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://pui.zycfv.cn

[U99] JS：事件监听
来源：http://dlf.zhixingplan.top

el.addEventListener("click", e => {})
来源：http://ypw.nanxuanxn.top

[U100] JS：DOM 查询
来源：http://oyl.jqgfzy.top

document.querySelector(".item")
来源：http://grm.jianghu66.top

[U101] JS：classList 操作
来源：http://yhi.zhongyouzk.top

el.classList.toggle("active")
来源：http://jue.jqgfzy.top

[U102] JS：本地存储
来源：http://yok.cucudq.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://dmp.daria6918.cn

[U103] JS：定时器
来源：http://pxe.hesvh.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://dsn.zdqjudy.top

[U104] JS：防抖
来源：http://qye.svipenyu.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://vou.316326.xyz

[U105] JS：节流
来源：http://igv.jinqigfzy.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://znb.zhoulong.xyz

[U106] JS：日期格式化
来源：http://paf.jinghuilouyu.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://sly.feifeiyinyue.top

[U107] JS：数字千分位
来源：http://sgx.shzxlz.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://xnf.yuanzhike.top

[U108] JS：随机整数
来源：http://eof.hywenlv.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://djp.xziqi.cn

[U109] JS：数组分组
来源：http://xtj.kuanghao11.cn

Object.groupBy(arr, x => x.type)
来源：http://foz.chenjidiqi.icu

[U110] JS：数组分块
来源：http://rxm.andypj.xyz

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://lhw.andypj.xyz

[U111] JS：对象转 Map
来源：http://bxm.0kj1m.cn

new Map(Object.entries(obj))
来源：http://vpo.gaohongyu789.top

[U112] JS：字符串补位
来源：http://yfz.0kj1m.cn

"7".padStart(3, "0")
来源：http://hqp.vehdjk.com

[U113] JS：正则替换全部
来源：http://etm.chenzaomai.com

s.replaceAll("a", "b")
来源：http://tme.jiagoushi.top

[U114] JS：JSON 深比较
来源：http://rja.zhijiandao.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://wnb.chenlongwang.top

[U115] JS：生成 UUID
来源：http://sct.feifeiyinyue.top

crypto.randomUUID()
来源：http://apw.cucudq.cn

[U116] JS：类型检查（JSDoc）
来源：http://lww.pengpengdd.cyou

/** @param {string} name */ function f(name) {}
来源：http://qfi.jyoumei.cn

[U117] JS：单元测试
来源：http://gfs.iojbl.cn

npm i -D vitest;  npx vitest
来源：http://apb.zhoulong.xyz

[U118] JS：开发服务器
来源：http://lnx.shzxlz.cn

npm i -D vite;  npx vite
来源：http://bdf.yfazqb.com

[U119] JS：生产构建
来源：http://dyw.jianghu66.top

npx vite build
来源：http://hgu.jqgfzy.top

[U120] JS：读取环境变量（Vite）
来源：http://ibc.birdmap.top

import.meta.env.VITE_API_URL
来源：http://aad.c1oappe.top

================================================================================
来源：http://qlt.hnxiangtu.top

统计汇总
来源：http://znt.aizwys.cn

================================================================================
来源：http://fjw.cheryme.top

按语言统计（条）：
来源：http://nil.zdbjq.cn

Python ......... 252
来源：http://fja.yuanzhike.top

PHP ............ 252
来源：http://iym.yj20258888.top

JavaScript ..... 252
来源：http://lce.ctjpmb.com

TypeScript ..... 212
来源：http://zwf.shanyushiyangkeji.top

Java ........... 212
来源：http://pib.haohaochexian.top

Go ............. 212
来源：http://kdr.xuetiantiany.cn

Ruby ........... 212
来源：http://hdg.jlsjyb.cn

C# ............. 212
来源：http://tcr.jlsjyb.cn

C .............. 30
来源：http://nwt.jinqigufen.top

C++ ............ 30
来源：http://mqd.xylfe.cn

SQL ............ 90
来源：http://azb.tianlin.xyz

Bash ........... 80
来源：http://cwn.yonumen.top

Kotlin ......... 15
来源：http://xop.haohaochexian.top

Swift .......... 15
来源：http://zlj.feifeiyinyue.top

Lua ............ 10
来源：http://xwe.yonumen.top

Perl ........... 10
来源：http://mbo.gzhubu.top

Scala .......... 10
来源：http://nyn.daria6918.cn

------------------------------------
来源：http://tff.nanxuanxn.top

合计 ........... 2106 条
来源：http://wwz.xylfe.cn

按章节统计：
来源：http://mtr.hnxiangtu.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://tiv.9152youxi.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://lpe.tanke756.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://prt.jianghu66.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://pbg.uphjek.com

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://ldp.fengsongda.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://ori.zhengqikj.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://osv.sufxvd.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://tlv.sjlbkw.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://vec.vqdsnc.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://jwv.nwbrower.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://iuj.yj20258888.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://ulh.jianghu66.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://qwf.jqgufenzy.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://sgx.hysaishi.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://abw.yueranfly.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://mmj.dianchejie.cn

Q SQL 专题                              90
来源：http://keb.tian-w.cn

R Bash 专题                             80
来源：http://lyw.dianchejie.cn

S C / C++ 专题                          60
来源：http://ukn.jinqigufen.top

T 其他语言补充                          60
来源：http://lvd.fzhhl.top

U 高频实用片段                         120
来源：http://fji.ydzc1.top

------------------------------------
来源：http://ble.cashguo.top

合计                                  2106 条
来源：http://bsy.hysaishi.cn

--------------------------------------------------------------------------------
来源：http://dtk.pycfn.com

使用提醒
来源：http://btl.zhijiandao.cn

--------------------------------------------------------------------------------
来源：http://ufd.nwbrower.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://wab.shzxlz.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://zgb.cheryme.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://oew.vehdjk.com

在旧版本上使用前请先确认语法支持情况。
来源：http://cmy.daxiang520.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://asa.kuanghao11.cn

—— 文件结束 ——
来源：http://vpo.c1oappe.top

================================================================================
来源：http://otu.gzhubu.top

程序语言常见例子速查手册（2024 版）
来源：http://gba.fanxiaobao.xyz

Common Programming Examples Cheat Book
来源：http://idr.gotoacloud.top

================================================================================
来源：http://rsh.yuxming.cn


<!-- 参考信息 -->