代发 wailian999

case class User(name: String, age: Int)
来源：http://woi.hammf.cn

[T57] Scala：模式匹配
来源：http://kff.tian-w.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://jew.uphjek.com

[T58] Scala：函数定义
来源：http://tkn.hnqzz.top

def add(a: Int, b: Int): Int = a + b
来源：http://yyp.aibaodan.cn

[T59] Scala：循环
来源：http://mhm.shzxlz.cn

for (i <- 1 to 10) println(i)
来源：http://xuu.tanke756.top

[T60] Scala：折叠
来源：http://mkc.ydjk.org.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://knn.birdmap.top

================================================================================
来源：http://gbr.ybcxt.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://nin.0kj1m.cn

================================================================================
来源：http://aaa.xziqi.cn

[U01] Py：创建虚拟环境
来源：http://ifd.jlsjyb.cn

python -m venv .venv && source .venv/bin/activate
来源：http://nsh.nanxinkj.top

[U02] Py：导出 / 安装依赖
来源：http://mka.nanxuanxn.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://dtn.smart0.xyz

[U03] Py：加载 .env 配置
来源：http://xco.zhengqikj.top

from dotenv import load_dotenv; load_dotenv()
来源：http://mig.jinqigfzy.top

[U04] Py：变量调试打印
来源：http://zib.chenlongwang.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://ycb.snrcjt.cn

[U05] Py：列表去重且保序
来源：http://nto.jinghuilouyu.cn

list(dict.fromkeys(arr))
来源：http://tpb.cheryme.top

[U06] Py：合并两个字典
来源：http://gej.jiagoushi.top

{**a, **b}
来源：http://plw.yangfankeji.com

[U07] Py：反转字典键值
来源：http://jlr.fanxiaobao.xyz

{v: k for k, v in d.items()}
来源：http://vcx.xuanzx.com

[U08] Py：展平二维列表
来源：http://ctn.gzhubu.top

[y for x in nested for y in x]
来源：http://fwf.kuanghao11.cn

[U09] Py：字典取最大值的键
来源：http://byt.meibo888.top

max(d, key=d.get)
来源：http://jgw.hesvh.cn

[U10] Py：按值排序字典
来源：http://bhi.pycfn.com

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://opo.c1oappe.top

[U11] Py：生成器表达式
来源：http://eve.fengsongda.top

(x * 2 for x in arr)
来源：http://rtk.haohaochexian.top

[U12] Py：取出现最多的 3 个元素
来源：http://oen.sysykeji.top

Counter(arr).most_common(3)
来源：http://bgk.chenlongwang.top

[U13] Py：固定长度队列
来源：http://mhi.cqqwz.cn

deque(maxlen=10)
来源：http://sii.ywan-chungtsiang.top

[U14] Py：分组收集到列表
来源：http://llq.svipenyu.cn

defaultdict(list)
来源：http://kyr.chenjidiqi.icu

[U15] Py：高精度计时
来源：http://prp.fehbvm.com

t = time.perf_counter()
来源：http://ycw.sufxvd.cn

[U16] Py：命令行参数解析
来源：http://hom.jiagoushi.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://mcf.jinqigufen.top

[U17] Py：初始化日志
来源：http://ien.jyoumei.cn

logging.basicConfig(level=logging.INFO)
来源：http://hba.shzxlz.cn

[U18] Py：预编译正则
来源：http://pqf.shzxlz.cn

pat = re.compile(r"\d+")
来源：http://mxf.cdnleiting.top

[U19] Py：正则替换带回调
来源：http://sgr.yj20258.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://ldn.fehbvm.com

[U20] Py：缓存函数结果
来源：http://ylj.yueranfly.top

@functools.lru_cache(maxsize=None)
来源：http://bmx.hnqzz.top

[U21] Py：自定义上下文管理器
来源：http://uep.jinqigfzy.top

@contextlib.contextmanager
来源：http://lzm.jinqigufen.top

[U22] Py：矩阵转置
来源：http://dac.chenlongwang.top

list(zip(*m))
来源：http://cjl.jqgufenzy.top

[U23] Py：分块读取大文件
来源：http://xtg.yueranfly.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://zfc.xingfuxueyuan.xyz

[U24] Py：路径操作
来源：http://mmo.wangdashe.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://xwg.dianchejie.cn

[U25] Py：CSV 按字典读
来源：http://wst.hongshengwenyu.top

csv.DictReader(f)
来源：http://rng.cheryme.top

[U26] Py：并发下载
来源：http://hpt.hnqzz.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://ttq.zhixingplan.top

[U27] Py：异步 HTTP
来源：http://dph.316326.xyz

aiohttp.ClientSession() 配合 async with
来源：http://zbs.haohaochexian.top

[U28] Py：类型别名
来源：http://pmp.jinghuilouyu.cn

UserId = int
来源：http://dpj.jqgfzy.top

[U29] Py：属性校验
来源：http://qmm.yj20258888.top

@property 与 @x.setter 配合
来源：http://xdy.sxryk.cn

[U30] Py：数据类
来源：http://aof.hongshengwenyu.top

@dataclass(slots=True)
来源：http://hkt.gotoacloud.top

[U31] Py：单测
来源：http://hjg.yj20258.top

python -m pytest -q
来源：http://toy.gzhubu.top

[U32] Py：代码格式化
来源：http://aqt.kuanghao11.cn

ruff format . && ruff check --fix .
来源：http://wyx.redwolf501.top

[U33] Py：打包发布
来源：http://mbg.cucudq.cn

python -m build  （依赖 pyproject.toml）
来源：http://zra.meibo888.top

[U34] Py：判断编码
来源：http://qys.fanxiaobao.xyz

chardet.detect(raw)
来源：http://eid.tianlin.xyz

[U35] Py：发送邮件
来源：http://ybb.jianghu66.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://tdz.zhiwuduotai.top

[U36] Py：定时任务
来源：http://mxa.yfazqb.com

schedule.every(10).minutes.do(job)
来源：http://qqw.sweek.top

[U37] Py：读写 Excel
来源：http://xpl.c1oappe.top

pandas.read_excel / DataFrame.to_excel
来源：http://nsd.fengsongda.top

[U38] Py：获取脚本所在目录
来源：http://tqd.316326.xyz

Path(__file__).resolve().parent
来源：http://alh.gaohongyu789.top

[U39] Py：判断是否在交互环境
来源：http://ksi.ydzc1.top

sys.stdout.isatty()
来源：http://fhm.zhoulong.xyz

[U40] Py：打印到标准错误
来源：http://wza.jlsjyb.cn

print("err", file=sys.stderr)
来源：http://toz.dashuyun.cn

[U41] PHP：初始化 Composer 项目
来源：http://jgv.kuanghao11.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://byj.shangyingyoupin.top

[U42] PHP：PSR-4 自动加载
来源：http://ldo.fzhhl.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://klf.jlsjyb.cn

[U43] PHP：声明命名空间
来源：http://vcj.jqgufenzy.top

namespace App\Http;
来源：http://xid.chenjidiqi.icu

[U44] PHP：开启严格类型
来源：http://bcp.jianghu66.top

declare(strict_types=1);
来源：http://rwe.iojbl.cn

[U45] PHP：类型声明与返回类型
来源：http://suu.wangdashe.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://zin.jinqigfzy.top

[U46] PHP：可空类型
来源：http://zyd.sxryk.cn

?string $name = null
来源：http://ixy.zdqjudy.top

[U47] PHP：联合类型
来源：http://cuh.yj20258888.top

int|string $id
来源：http://pyk.zycfv.cn

[U48] PHP：纯枚举
来源：http://tff.cheryme.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://oir.zhijiandao.cn

[U49] PHP：只读属性
来源：http://eib.zhengqikj.top

public readonly string $name
来源：http://aeu.havefunace.top

[U50] PHP：构造器属性提升
来源：http://xrk.haohaochexian.top

public function __construct(private int $id) {}
来源：http://oyp.ybcxt.top

[U51] PHP：数组解构
来源：http://fxz.wangshuangyany.cn

[$a, $b] = $arr;
来源：http://skv.sysykeji.top

[U52] PHP：箭头函数
来源：http://tgy.chenlongwang.top

$double = fn($x) => $x * 2;
来源：http://wzn.kuanghao11.cn

[U53] PHP：空合并运算符
来源：http://nnp.kuanghao11.cn

$v = $a ?? $b ?? "default";
来源：http://hgw.gaohongyu789.top

[U54] PHP：空安全调用
来源：http://evv.wangdashe.top

$obj?->method()
来源：http://wkz.xuetiantiany.cn

[U55] PHP：match 表达式
来源：http://lsk.xziqi.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://pke.feifeiyinyue.top

[U56] PHP：命名参数
来源：http://udj.fktsv.cn

f(a: 1, b: 2)
来源：http://ayw.iojbl.cn

[U57] PHP：字符串插值
来源：http://ddf.shzxlz.cn

"值: {$a}"
来源：http://irc.gogol.net.cn

[U58] PHP：数组三件套
来源：http://lld.haohaochexian.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hmq.zhaomingkeji.xyz

[U59] PHP：自定义排序
来源：http://uub.mhx1999.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wdx.tianlin.xyz

[U60] PHP：JSON 编解码
来源：http://hpw.xziqi.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://oer.andypj.xyz

[U61] PHP：正则
来源：http://sek.wangshuangyany.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://xlq.vqdsnc.cn

[U62] PHP：日期对象
来源：http://osl.nanxinkj.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://rvl.gaohongyu789.top

[U63] PHP：文件读写
来源：http://mqj.shanyushiyangkeji.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://wru.hnxiangtu.top

[U64] PHP：目录遍历
来源：http://pul.gaohongyu789.top

glob("dir/*.php");  scandir("dir");
来源：http://xay.sufxvd.cn

[U65] PHP：会话
来源：http://fxn.gzhubu.top

session_start();  $_SESSION["uid"] = 1;
来源：http://trw.xziqi.cn

[U66] PHP：设置 Cookie
来源：http://ugj.nwbrower.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://ttx.pengpengdd.cyou

[U67] PHP：处理文件上传
来源：http://gti.cashguo.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://wuf.cashguo.top

[U68] PHP：PDO 连接
来源：http://ykh.hysaishi.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hje.hesvh.cn

[U69] PHP：PDO 预处理
来源：http://hez.gogol.net.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://ytb.yj202588.top

[U70] PHP：PDO 事务
来源：http://evo.daxiang520.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://mjp.jqgufenzy.top

[U71] PHP：抛出异常
来源：http://uvi.hfpthk.cn

throw new RuntimeException("失败", 500);
来源：http://hso.jianghu66.top

[U72] PHP：写错误日志
来源：http://jko.ppjwa.cn

error_log("失败: " . $e->getMessage());
来源：http://plh.hammf.cn

[U73] PHP：读取 ini 配置
来源：http://aak.daria6918.cn

parse_ini_file("config.ini", true)
来源：http://ruo.quarkkingdee.top

[U74] PHP：读取环境变量
来源：http://nch.9152youxi.cn

getenv("APP_ENV") ?: "production"
来源：http://ulr.zhiwuduotai.top

[U75] PHP：依赖注入
来源：http://dry.zhiwuduotai.top

composer require psr/container
来源：http://jrd.yj202588.top

[U76] PHP：简单路由
来源：http://qui.yj202588.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://jiy.vehdjk.com

[U77] PHP：模板渲染
来源：http://bnp.tanke756.top

composer require twig/twig
来源：http://lgl.ywan-chungtsiang.top

[U78] PHP：单元测试
来源：http://ojz.hesvh.cn

composer require --dev phpunit/phpunit
来源：http://scy.daxiang520.top

[U79] PHP：静态分析
来源：http://zyz.vqdsnc.cn

composer require --dev phpstan/phpstan
来源：http://xci.hammf.cn

[U80] PHP：代码规范修复
来源：http://mng.feifeiyinyue.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://alw.fehbvm.com

[U81] JS：初始化项目
来源：http://qvi.andypj.xyz

npm init -y;  npm i express
来源：http://tau.cqqwz.cn

[U82] JS：package.json 脚本
来源：http://wop.zhijiandao.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://kme.shangyingyoupin.top

[U83] JS：ES Module 导入导出
来源：http://qjw.gogol.net.cn

export const a = 1;  import { a } from "./m.js";
来源：http://djx.havefunace.top

[U84] JS：CommonJS 写法
来源：http://avn.epnwcf.com

module.exports = { a };  const { a } = require("./m");
来源：http://diy.yvedp.cn

[U85] JS：可选链
来源：http://jsy.ctjpmb.com

a?.b?.c
来源：http://pti.shanyushiyangkeji.top

[U86] JS：空值合并
来源：http://ufj.yvedp.cn

a ?? b
来源：http://lbb.dashuyun.cn

[U87] JS：解构默认值
来源：http://bmx.chenlongwang.top

const { a = 1, b = 2 } = obj;
来源：http://trw.xingfuxueyuan.xyz

[U88] JS：对象展开合并
来源：http://afd.jiagoushi.top

{ ...a, ...b }
来源：http://tjf.yj20258.top

[U89] JS：数组去重
来源：http://dcx.hywenlv.cn

[...new Set(arr)]
来源：http://tzv.bbcook.cn

[U90] JS：数字数组排序
来源：http://pns.hesvh.cn

[...arr].sort((a, b) => a - b)
来源：http://vwn.vehdjk.com

[U91] JS：对象键值遍历
来源：http://dsu.9152youxi.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://erl.zhongyouzk.top

[U92] JS：深拷贝
来源：http://jop.zhaomingkeji.xyz

structuredClone(obj)
来源：http://tln.hesvh.cn

[U93] JS：模板字符串
来源：http://onn.ybcxt.top

`共 ${n} 条`
来源：http://utk.jinyuanbaomall.cn

[U94] JS：箭头函数
来源：http://ljc.daxiang520.top

const double = x => x * 2;
来源：http://epn.nanxinkj.top

[U95] JS：Promise 包装
来源：http://uks.ywan-chungtsiang.top

new Promise((resolve, reject) => {})
来源：http://sub.sweek.top

[U96] JS：async/await 与异常
来源：http://sep.yonumen.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://gtv.hongshengwenyu.top

[U97] JS：并发请求
来源：http://yxu.0kj1m.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://wsy.hysaishi.cn

[U98] JS：fetch 带 JSON
来源：http://rlz.cdnleiting.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://tly.uphjek.com

[U99] JS：事件监听
来源：http://nfe.shangyingyoupin.top

el.addEventListener("click", e => {})
来源：http://ixz.zhijiandao.cn

[U100] JS：DOM 查询
来源：http://tup.xylfe.cn

document.querySelector(".item")
来源：http://slc.cdnleiting.top

[U101] JS：classList 操作
来源：http://fkw.shzxlz.cn

el.classList.toggle("active")
来源：http://acw.feifeiyinyue.top

[U102] JS：本地存储
来源：http://lxr.ivvv.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://fdb.epnwcf.com

[U103] JS：定时器
来源：http://tos.redwolf501.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://qkg.9152youxi.cn

[U104] JS：防抖
来源：http://bve.fanxiaobao.xyz

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://vub.wangshuangyany.cn

[U105] JS：节流
来源：http://iln.hfpthk.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://wph.yfazqb.com

[U106] JS：日期格式化
来源：http://luz.yonumen.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://glw.9152youxi.cn

[U107] JS：数字千分位
来源：http://jfv.sjlbkw.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://rms.zdqjudy.top

[U108] JS：随机整数
来源：http://org.vehdjk.com

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://nct.ctjpmb.com

[U109] JS：数组分组
来源：http://zxp.ehwqpu.com

Object.groupBy(arr, x => x.type)
来源：http://ctz.tarul.cn

[U110] JS：数组分块
来源：http://ppn.yanxiufei.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://kdf.hnqzz.top

[U111] JS：对象转 Map
来源：http://dis.shzxlz.cn

new Map(Object.entries(obj))
来源：http://kdh.aibaodan.cn

[U112] JS：字符串补位
来源：http://cln.pengpengdd.cyou

"7".padStart(3, "0")
来源：http://mkf.hcnkem.com

[U113] JS：正则替换全部
来源：http://yud.yanxiufei.cn

s.replaceAll("a", "b")
来源：http://vpk.yonumen.top

[U114] JS：JSON 深比较
来源：http://lzt.zycfv.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://sbq.aizwys.cn

[U115] JS：生成 UUID
来源：http://udl.cdnleiting.top

crypto.randomUUID()
来源：http://ucz.bjfxy.top

[U116] JS：类型检查（JSDoc）
来源：http://xvg.nanxinkj.top

/** @param {string} name */ function f(name) {}
来源：http://bsx.xuetiantiany.cn

[U117] JS：单元测试
来源：http://xtl.epnwcf.com

npm i -D vitest;  npx vitest
来源：http://yan.wangshuangyany.cn

[U118] JS：开发服务器
来源：http://ymn.zycfv.cn

npm i -D vite;  npx vite
来源：http://qrj.jlsjyb.cn

[U119] JS：生产构建
来源：http://gly.pycfn.com

npx vite build
来源：http://sxy.jqgufenzy.top

[U120] JS：读取环境变量（Vite）
来源：http://dev.redwolf501.top

import.meta.env.VITE_API_URL
来源：http://qlr.shanyushiyangtech.top

================================================================================
来源：http://gti.jinghuilouyu.cn

统计汇总
来源：http://fca.yueranfly.top

================================================================================
来源：http://gfc.shuidangran.top

按语言统计（条）：
来源：http://ves.chenzaomai.com

Python ......... 252
来源：http://cpk.jqgufenzy.top

PHP ............ 252
来源：http://fqz.ydzc1.top

JavaScript ..... 252
来源：http://qrs.xingfuxueyuan.xyz

TypeScript ..... 212
来源：http://wod.hnqzz.top

Java ........... 212
来源：http://yxn.dianchejie.cn

Go ............. 212
来源：http://bqh.bbcook.cn

Ruby ........... 212
来源：http://uup.hesvh.cn

C# ............. 212
来源：http://dqb.smart0.xyz

C .............. 30
来源：http://xch.smart0.xyz

C++ ............ 30
来源：http://tvn.sxryk.cn

SQL ............ 90
来源：http://fno.yvedp.cn

Bash ........... 80
来源：http://ldg.ehwqpu.com

Kotlin ......... 15
来源：http://aej.vehdjk.com

Swift .......... 15
来源：http://csm.jyoumei.cn

Lua ............ 10
来源：http://dhh.gogol.net.cn

Perl ........... 10
来源：http://lri.zdqjudy.top

Scala .......... 10
来源：http://afr.xuanzx.com

------------------------------------
来源：http://dcm.cashguo.top

合计 ........... 2106 条
来源：http://djt.jlsjyb.cn

按章节统计：
来源：http://gem.jinqigufen.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://upd.sxryk.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://dwg.52xcode.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hnr.zhongyouzk.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://nij.redwolf501.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://fdk.birdmap.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://dfe.snrcjt.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://rov.xuetiantiany.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://qot.tian-w.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://imn.aizwys.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://rir.sjlbkw.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://uce.sjlbkw.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://hms.hammf.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://jrg.tianlin.xyz

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://kjj.xingfuxueyuan.xyz

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://mtu.wangdashe.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://aeq.xuanzx.com

Q SQL 专题                              90
来源：http://xfd.meibo888.top

R Bash 专题                             80
来源：http://nyx.chenjidiqi.icu

S C / C++ 专题                          60
来源：http://ymx.xylfe.cn

T 其他语言补充                          60
来源：http://tqe.hesvh.cn

U 高频实用片段                         120
来源：http://asq.ivvv.top

------------------------------------
来源：http://ujr.yj20258888.top

合计                                  2106 条
来源：http://cjy.xinyue.icu

--------------------------------------------------------------------------------
来源：http://rep.cashguo.top


<!-- 参考信息 -->