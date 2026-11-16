代发 wailian999

case class User(name: String, age: Int)
来源：http://qpp.dashuyun.cn

[T57] Scala：模式匹配
来源：http://vvb.xziqi.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://vpa.jqgfzy.top

[T58] Scala：函数定义
来源：http://eej.yonumen.top

def add(a: Int, b: Int): Int = a + b
来源：http://zri.cdnleiting.top

[T59] Scala：循环
来源：http://dhy.yj202588.top

for (i <- 1 to 10) println(i)
来源：http://wnx.shzxlz.cn

[T60] Scala：折叠
来源：http://lyk.fanxiaobao.xyz

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://yyo.epnwcf.com

================================================================================
来源：http://nyy.aizwys.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://efb.shzxlz.cn

================================================================================
来源：http://khp.svipenyu.cn

[U01] Py：创建虚拟环境
来源：http://vrq.quarkkingdee.top

python -m venv .venv && source .venv/bin/activate
来源：http://loz.feifeiyinyue.top

[U02] Py：导出 / 安装依赖
来源：http://gxt.hongshengwenyu.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://krz.nanxuanxn.top

[U03] Py：加载 .env 配置
来源：http://qja.daxiang520.top

from dotenv import load_dotenv; load_dotenv()
来源：http://ewl.jianghu66.top

[U04] Py：变量调试打印
来源：http://rgt.gogol.net.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://snk.zhongyouzk.top

[U05] Py：列表去重且保序
来源：http://bto.redwolf501.top

list(dict.fromkeys(arr))
来源：http://beh.shangyingyoupin.top

[U06] Py：合并两个字典
来源：http://gpm.haohaochexian.top

{**a, **b}
来源：http://hiq.ctjpmb.com

[U07] Py：反转字典键值
来源：http://cbu.yvedp.cn

{v: k for k, v in d.items()}
来源：http://idl.cucudq.cn

[U08] Py：展平二维列表
来源：http://ifv.nanxinkj.top

[y for x in nested for y in x]
来源：http://ruh.c1oappe.top

[U09] Py：字典取最大值的键
来源：http://fdd.zhongyouzk.top

max(d, key=d.get)
来源：http://mzd.jqgufenzy.top

[U10] Py：按值排序字典
来源：http://mjz.epnwcf.com

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://xnm.tianlin.xyz

[U11] Py：生成器表达式
来源：http://kjn.chenlongwang.top

(x * 2 for x in arr)
来源：http://poy.nanxuanxn.top

[U12] Py：取出现最多的 3 个元素
来源：http://qwx.tian-w.cn

Counter(arr).most_common(3)
来源：http://nrw.andypj.xyz

[U13] Py：固定长度队列
来源：http://flu.yj20258888.top

deque(maxlen=10)
来源：http://rly.zhiwuduotai.top

[U14] Py：分组收集到列表
来源：http://oww.hnxiangtu.top

defaultdict(list)
来源：http://log.xziqi.cn

[U15] Py：高精度计时
来源：http://khl.yvedp.cn

t = time.perf_counter()
来源：http://vfm.andypj.xyz

[U16] Py：命令行参数解析
来源：http://sno.andypj.xyz

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://nhz.fehbvm.com

[U17] Py：初始化日志
来源：http://lzk.smart0.xyz

logging.basicConfig(level=logging.INFO)
来源：http://con.vehdjk.com

[U18] Py：预编译正则
来源：http://hqr.chenjidiqi.icu

pat = re.compile(r"\d+")
来源：http://zix.epnwcf.com

[U19] Py：正则替换带回调
来源：http://tro.ivvv.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://cgj.yuanzhike.top

[U20] Py：缓存函数结果
来源：http://bgc.hywenlv.cn

@functools.lru_cache(maxsize=None)
来源：http://hzw.pycfn.com

[U21] Py：自定义上下文管理器
来源：http://tpw.ywan-chungtsiang.top

@contextlib.contextmanager
来源：http://jks.vqdsnc.cn

[U22] Py：矩阵转置
来源：http://jay.xziqi.cn

list(zip(*m))
来源：http://mvb.xuanzx.com

[U23] Py：分块读取大文件
来源：http://uen.sweek.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://viq.zycfv.cn

[U24] Py：路径操作
来源：http://nyr.zdbjq.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://aod.tarul.cn

[U25] Py：CSV 按字典读
来源：http://ssz.xziqi.cn

csv.DictReader(f)
来源：http://coo.ydjk.org.cn

[U26] Py：并发下载
来源：http://zur.nanxuanxn.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://uin.zdqjudy.top

[U27] Py：异步 HTTP
来源：http://cvf.gaohongyu789.top

aiohttp.ClientSession() 配合 async with
来源：http://med.aibaodan.cn

[U28] Py：类型别名
来源：http://lpp.redwolf501.top

UserId = int
来源：http://aru.xziqi.cn

[U29] Py：属性校验
来源：http://gyi.316326.xyz

@property 与 @x.setter 配合
来源：http://kwe.jqgfzy.top

[U30] Py：数据类
来源：http://dkk.smart0.xyz

@dataclass(slots=True)
来源：http://cya.xingfuxueyuan.xyz

[U31] Py：单测
来源：http://zyx.yj20258.top

python -m pytest -q
来源：http://lvl.zhaomingkeji.xyz

[U32] Py：代码格式化
来源：http://bbi.hammf.cn

ruff format . && ruff check --fix .
来源：http://jcv.snrcjt.cn

[U33] Py：打包发布
来源：http://dlc.guannengcc.top

python -m build  （依赖 pyproject.toml）
来源：http://ibu.zdqjudy.top

[U34] Py：判断编码
来源：http://bzb.yuanzhike.top

chardet.detect(raw)
来源：http://uxf.zhongyouzk.top

[U35] Py：发送邮件
来源：http://iah.daria6918.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://bos.shuidangran.top

[U36] Py：定时任务
来源：http://kjv.9152youxi.cn

schedule.every(10).minutes.do(job)
来源：http://xpv.zycfv.cn

[U37] Py：读写 Excel
来源：http://sez.zhaomingkeji.xyz

pandas.read_excel / DataFrame.to_excel
来源：http://htv.yvedp.cn

[U38] Py：获取脚本所在目录
来源：http://rgq.hfpthk.cn

Path(__file__).resolve().parent
来源：http://hxr.hesvh.cn

[U39] Py：判断是否在交互环境
来源：http://muc.smart0.xyz

sys.stdout.isatty()
来源：http://gem.chenzaomai.com

[U40] Py：打印到标准错误
来源：http://iqp.shzxlz.cn

print("err", file=sys.stderr)
来源：http://els.ctjpmb.com

[U41] PHP：初始化 Composer 项目
来源：http://dyh.hammf.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://ngu.ppjwa.cn

[U42] PHP：PSR-4 自动加载
来源：http://iml.fanxiaobao.xyz

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://nno.daxiang520.top

[U43] PHP：声明命名空间
来源：http://aco.tarul.cn

namespace App\Http;
来源：http://ckl.nanxuanxn.top

[U44] PHP：开启严格类型
来源：http://tof.hnxiangtu.top

declare(strict_types=1);
来源：http://aeb.gotoacloud.top

[U45] PHP：类型声明与返回类型
来源：http://qxb.redwolf501.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://uha.xingfuxueyuan.xyz

[U46] PHP：可空类型
来源：http://cvk.tianlin.xyz

?string $name = null
来源：http://gzf.xziqi.cn

[U47] PHP：联合类型
来源：http://bsp.zhongyouzk.top

int|string $id
来源：http://bgn.yfazqb.com

[U48] PHP：纯枚举
来源：http://ubp.zhijiandao.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://xak.guannengcc.top

[U49] PHP：只读属性
来源：http://nhz.smart0.xyz

public readonly string $name
来源：http://fbk.zdqjudy.top

[U50] PHP：构造器属性提升
来源：http://fmq.hongshengwenyu.top

public function __construct(private int $id) {}
来源：http://ohm.hammf.cn

[U51] PHP：数组解构
来源：http://wgr.chenjidiqi.icu

[$a, $b] = $arr;
来源：http://kqj.tarul.cn

[U52] PHP：箭头函数
来源：http://ivn.wangshuangyany.cn

$double = fn($x) => $x * 2;
来源：http://kch.zhiwuduotai.top

[U53] PHP：空合并运算符
来源：http://grj.guowangkeji.top

$v = $a ?? $b ?? "default";
来源：http://knj.316326.xyz

[U54] PHP：空安全调用
来源：http://nhi.aibaodan.cn

$obj?->method()
来源：http://kqv.cucudq.cn

[U55] PHP：match 表达式
来源：http://ojm.hammf.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://zcn.hysaishi.cn

[U56] PHP：命名参数
来源：http://jif.sufxvd.cn

f(a: 1, b: 2)
来源：http://iev.tanke756.top

[U57] PHP：字符串插值
来源：http://lal.kuanghao11.cn

"值: {$a}"
来源：http://vps.zhixingplan.top

[U58] PHP：数组三件套
来源：http://ooa.epnwcf.com

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://ajy.shanyushiyangkeji.top

[U59] PHP：自定义排序
来源：http://xre.epnwcf.com

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://bdj.ctjpmb.com

[U60] PHP：JSON 编解码
来源：http://oez.sweek.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://svm.hnqzz.top

[U61] PHP：正则
来源：http://knw.dianchejie.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://ogc.zhiwuduotai.top

[U62] PHP：日期对象
来源：http://zmk.shangyingyoupin.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://lbz.cucudq.cn

[U63] PHP：文件读写
来源：http://nzd.feifeiyinyue.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://eug.yangfankeji.com

[U64] PHP：目录遍历
来源：http://pij.gotoacloud.top

glob("dir/*.php");  scandir("dir");
来源：http://waw.jqgufenzy.top

[U65] PHP：会话
来源：http://ads.jiagoushi.top

session_start();  $_SESSION["uid"] = 1;
来源：http://pso.hnxiangtu.top

[U66] PHP：设置 Cookie
来源：http://epk.tianlin.xyz

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://ddf.redwolf501.top

[U67] PHP：处理文件上传
来源：http://lay.dashuyun.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://rjt.jinqigfzy.top

[U68] PHP：PDO 连接
来源：http://wht.guowangkeji.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://lmh.shuidangran.top

[U69] PHP：PDO 预处理
来源：http://rbj.ydjk.org.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://ytu.ydzc1.top

[U70] PHP：PDO 事务
来源：http://bdp.yongpay.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://nqj.yonumen.top

[U71] PHP：抛出异常
来源：http://gyl.zhijiandao.cn

throw new RuntimeException("失败", 500);
来源：http://jub.hammf.cn

[U72] PHP：写错误日志
来源：http://maq.ctjpmb.com

error_log("失败: " . $e->getMessage());
来源：http://hca.jinghuilouyu.cn

[U73] PHP：读取 ini 配置
来源：http://mhl.52xcode.cn

parse_ini_file("config.ini", true)
来源：http://awd.meibo888.top

[U74] PHP：读取环境变量
来源：http://rru.gogol.net.cn

getenv("APP_ENV") ?: "production"
来源：http://ocv.zhaomingkeji.xyz

[U75] PHP：依赖注入
来源：http://tip.guowangkeji.top

composer require psr/container
来源：http://ohm.yvedp.cn

[U76] PHP：简单路由
来源：http://lpq.yangfankeji.com

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://plh.gotoacloud.top

[U77] PHP：模板渲染
来源：http://sme.ybcxt.top

composer require twig/twig
来源：http://vzk.ctjpmb.com

[U78] PHP：单元测试
来源：http://idb.tian-w.cn

composer require --dev phpunit/phpunit
来源：http://bay.cashguo.top

[U79] PHP：静态分析
来源：http://xpk.xingfuxueyuan.xyz

composer require --dev phpstan/phpstan
来源：http://qca.aizwys.cn

[U80] PHP：代码规范修复
来源：http://xbx.shzxlz.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://cds.uphjek.com

[U81] JS：初始化项目
来源：http://voh.pycfn.com

npm init -y;  npm i express
来源：http://kyr.fengsongda.top

[U82] JS：package.json 脚本
来源：http://xsi.0kj1m.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://gff.jinqigufen.top

[U83] JS：ES Module 导入导出
来源：http://pfx.jqgufenzy.top

export const a = 1;  import { a } from "./m.js";
来源：http://kva.cashguo.top

[U84] JS：CommonJS 写法
来源：http://kbr.tianlin.xyz

module.exports = { a };  const { a } = require("./m");
来源：http://oql.vqdsnc.cn

[U85] JS：可选链
来源：http://xdl.ydjk.org.cn

a?.b?.c
来源：http://qsz.yuanzhike.top

[U86] JS：空值合并
来源：http://uih.aibaodan.cn

a ?? b
来源：http://wav.pycfn.com

[U87] JS：解构默认值
来源：http://yfg.guowangkeji.top

const { a = 1, b = 2 } = obj;
来源：http://sal.nanxuanxn.top

[U88] JS：对象展开合并
来源：http://rbw.mhx1999.top

{ ...a, ...b }
来源：http://orl.cheryme.top

[U89] JS：数组去重
来源：http://ejx.kuanghao11.cn

[...new Set(arr)]
来源：http://mie.xuanzx.com

[U90] JS：数字数组排序
来源：http://hxd.meibo888.top

[...arr].sort((a, b) => a - b)
来源：http://fvw.xylfe.cn

[U91] JS：对象键值遍历
来源：http://sha.hywenlv.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://dsd.jinqigufen.top

[U92] JS：深拷贝
来源：http://shw.dianchejie.cn

structuredClone(obj)
来源：http://cya.fzhhl.top

[U93] JS：模板字符串
来源：http://uet.bbcook.cn

`共 ${n} 条`
来源：http://fzy.shangyingyoupin.top

[U94] JS：箭头函数
来源：http://tvg.jyoumei.cn

const double = x => x * 2;
来源：http://kfv.nwbrower.top

[U95] JS：Promise 包装
来源：http://mqe.zhoulong.xyz

new Promise((resolve, reject) => {})
来源：http://ikl.fehbvm.com

[U96] JS：async/await 与异常
来源：http://vfk.jqgufenzy.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://wks.ivvv.top

[U97] JS：并发请求
来源：http://qsb.sysykeji.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://fmq.0kj1m.cn

[U98] JS：fetch 带 JSON
来源：http://jax.sxryk.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://qbn.daria6918.cn

[U99] JS：事件监听
来源：http://npq.hfpthk.cn

el.addEventListener("click", e => {})
来源：http://lis.jqgufenzy.top

[U100] JS：DOM 查询
来源：http://pyk.gzhubu.top

document.querySelector(".item")
来源：http://emo.gogol.net.cn

[U101] JS：classList 操作
来源：http://mdw.hnqzz.top

el.classList.toggle("active")
来源：http://vwi.9152youxi.cn

[U102] JS：本地存储
来源：http://kcl.zhongyouzk.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://lta.havefunace.top

[U103] JS：定时器
来源：http://xwt.snrcjt.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://gjy.xuanzx.com

[U104] JS：防抖
来源：http://zml.fanxiaobao.xyz

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ftj.cheryme.top

[U105] JS：节流
来源：http://chb.gaohongyu789.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://fkg.chenjidiqi.icu

[U106] JS：日期格式化
来源：http://viv.chenlongwang.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://fml.nanxinkj.top

[U107] JS：数字千分位
来源：http://atv.zhongyouzk.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://xty.wangdashe.top

[U108] JS：随机整数
来源：http://dlp.jinghuilouyu.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://rdg.zhaomingkeji.xyz

[U109] JS：数组分组
来源：http://kmu.daxiang520.top

Object.groupBy(arr, x => x.type)
来源：http://kmi.xziqi.cn

[U110] JS：数组分块
来源：http://jek.yanxiufei.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://tnf.shangyingyoupin.top

[U111] JS：对象转 Map
来源：http://yfq.52xcode.cn

new Map(Object.entries(obj))
来源：http://awl.zhaomingkeji.xyz

[U112] JS：字符串补位
来源：http://pfg.tian-w.cn

"7".padStart(3, "0")
来源：http://aog.daxiang520.top

[U113] JS：正则替换全部
来源：http://shg.yuxming.cn

s.replaceAll("a", "b")
来源：http://qde.dianchejie.cn

[U114] JS：JSON 深比较
来源：http://qgy.sysykeji.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://efq.0kj1m.cn

[U115] JS：生成 UUID
来源：http://vkh.hnqzz.top

crypto.randomUUID()
来源：http://jxs.xuetiantiany.cn

[U116] JS：类型检查（JSDoc）
来源：http://jfa.hammf.cn

/** @param {string} name */ function f(name) {}
来源：http://vgz.ydjk.org.cn

[U117] JS：单元测试
来源：http://bnv.jyoumei.cn

npm i -D vitest;  npx vitest
来源：http://sml.c1oappe.top

[U118] JS：开发服务器
来源：http://mak.xziqi.cn

npm i -D vite;  npx vite
来源：http://jmz.ydzc1.top

[U119] JS：生产构建
来源：http://esw.nanxinkj.top

npx vite build
来源：http://sno.yfazqb.com

[U120] JS：读取环境变量（Vite）
来源：http://ynl.nwbrower.top

import.meta.env.VITE_API_URL
来源：http://ftw.yanxiufei.cn

================================================================================
来源：http://ceq.daria6918.cn

统计汇总
来源：http://wbh.yonumen.top

================================================================================
来源：http://kiy.fzhhl.top

按语言统计（条）：
来源：http://wmk.yueranfly.top

Python ......... 252
来源：http://iwm.yangfankeji.com

PHP ............ 252
来源：http://nyg.jinyuanbaomall.cn

JavaScript ..... 252
来源：http://qte.sysykeji.top

TypeScript ..... 212
来源：http://wsi.chenzaomai.com

Java ........... 212
来源：http://tco.yuxming.cn

Go ............. 212
来源：http://vvt.zhijiandao.cn

Ruby ........... 212
来源：http://qid.sxryk.cn

C# ............. 212
来源：http://mkk.iojbl.cn

C .............. 30
来源：http://ofm.zdbjq.cn

C++ ............ 30
来源：http://fnm.yuanzhike.top

SQL ............ 90
来源：http://shb.ybcxt.top

Bash ........... 80
来源：http://clm.meibo888.top

Kotlin ......... 15
来源：http://aqu.ydzc1.top

Swift .......... 15
来源：http://kws.nanxinkj.top

Lua ............ 10
来源：http://fei.jinqigfzy.top

Perl ........... 10
来源：http://njs.shanyushiyangkeji.top

Scala .......... 10
来源：http://ccy.ehwqpu.com

------------------------------------
来源：http://xhw.chenjidiqi.icu

合计 ........... 2106 条
来源：http://ycv.yangfankeji.com

按章节统计：
来源：http://eqp.cdnleiting.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://yjs.xinyue.icu

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://iak.xylfe.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://dot.pycfn.com

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://axm.jyoumei.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://wlp.hammf.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://cva.fanxiaobao.xyz

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://jof.iojbl.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://ovt.yueranfly.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://bki.jinyuanbaomall.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://fmz.cucudq.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://rxs.meibo888.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://ukz.yuanzhike.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://kng.hywenlv.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://ggp.tianlin.xyz

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://kqw.xuanzx.com

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://ntt.chenzaomai.com

Q SQL 专题                              90
来源：http://clm.guowangkeji.top

R Bash 专题                             80
来源：http://drr.xylfe.cn

S C / C++ 专题                          60
来源：http://msu.jianghu66.top

T 其他语言补充                          60
来源：http://xws.0kj1m.cn

U 高频实用片段                         120
来源：http://ntt.hnxiangtu.top

------------------------------------
来源：http://kbo.fengsongda.top

合计                                  2106 条
来源：http://sct.fehbvm.com

--------------------------------------------------------------------------------
来源：http://cdw.iojbl.cn


<!-- 参考信息 -->