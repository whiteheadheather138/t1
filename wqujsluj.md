代发 wailian999

val a = 1;  var b = 2
来源：http://ysn.yangfankeji.com

[T53] Scala：字符串插值
来源：http://cmh.pycfn.com

s"值: $b"
来源：http://nof.52xcode.cn

[T54] Scala：集合映射
来源：http://sjd.guannengcc.top

List(1, 2, 3).map(_ * 2)
来源：http://yyw.aibaodan.cn

[T55] Scala：集合过滤
来源：http://fjx.bjfxy.top

List(1, 2, 3).filter(_ > 1)
来源：http://cic.zycfv.cn

[T56] Scala：样例类
来源：http://xmu.jyoumei.cn

case class User(name: String, age: Int)
来源：http://yon.vqdsnc.cn

[T57] Scala：模式匹配
来源：http://kwx.yj20258888.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://han.vqdsnc.cn

[T58] Scala：函数定义
来源：http://cii.pengpengdd.cyou

def add(a: Int, b: Int): Int = a + b
来源：http://rah.hammf.cn

[T59] Scala：循环
来源：http://peg.jinyuanbaomall.cn

for (i <- 1 to 10) println(i)
来源：http://zpc.feifeiyinyue.top

[T60] Scala：折叠
来源：http://ikb.ppjwa.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://ynh.gogol.net.cn

================================================================================
来源：http://dnu.fehbvm.com

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://kpw.tian-w.cn

================================================================================
来源：http://tug.sweek.top

[U01] Py：创建虚拟环境
来源：http://ypm.c1oappe.top

python -m venv .venv && source .venv/bin/activate
来源：http://qbl.ydzc1.top

[U02] Py：导出 / 安装依赖
来源：http://hrt.guowangkeji.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://yoc.ehwqpu.com

[U03] Py：加载 .env 配置
来源：http://ivb.9152youxi.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://exj.sysykeji.top

[U04] Py：变量调试打印
来源：http://vrl.chenzaomai.com

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://jmv.dashuyun.cn

[U05] Py：列表去重且保序
来源：http://gkp.ybcxt.top

list(dict.fromkeys(arr))
来源：http://kpu.redwolf501.top

[U06] Py：合并两个字典
来源：http://off.yongpay.top

{**a, **b}
来源：http://cwy.hongshengwenyu.top

[U07] Py：反转字典键值
来源：http://hhl.bjfxy.top

{v: k for k, v in d.items()}
来源：http://npm.yangfankeji.com

[U08] Py：展平二维列表
来源：http://aqf.hcnkem.com

[y for x in nested for y in x]
来源：http://bia.hongshengwenyu.top

[U09] Py：字典取最大值的键
来源：http://krw.fehbvm.com

max(d, key=d.get)
来源：http://fle.zhijiandao.cn

[U10] Py：按值排序字典
来源：http://zxj.jinqigufen.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://dha.pycfn.com

[U11] Py：生成器表达式
来源：http://yms.ybcxt.top

(x * 2 for x in arr)
来源：http://iya.cdnleiting.top

[U12] Py：取出现最多的 3 个元素
来源：http://dmm.chenzaomai.com

Counter(arr).most_common(3)
来源：http://pja.gzhubu.top

[U13] Py：固定长度队列
来源：http://xhd.shzxlz.cn

deque(maxlen=10)
来源：http://oxq.hywenlv.cn

[U14] Py：分组收集到列表
来源：http://qra.sysykeji.top

defaultdict(list)
来源：http://gvl.guowangkeji.top

[U15] Py：高精度计时
来源：http://maj.bbcook.cn

t = time.perf_counter()
来源：http://nfr.pycfn.com

[U16] Py：命令行参数解析
来源：http://cfn.zhongyouzk.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://sgv.nanxuanxn.top

[U17] Py：初始化日志
来源：http://koy.nwbrower.top

logging.basicConfig(level=logging.INFO)
来源：http://kgu.ydzc1.top

[U18] Py：预编译正则
来源：http://omo.zdbjq.cn

pat = re.compile(r"\d+")
来源：http://ysq.shzxlz.cn

[U19] Py：正则替换带回调
来源：http://neh.yj20258.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://lsd.ydzc1.top

[U20] Py：缓存函数结果
来源：http://uyo.hnqzz.top

@functools.lru_cache(maxsize=None)
来源：http://bbp.pycfn.com

[U21] Py：自定义上下文管理器
来源：http://bqt.xinyue.icu

@contextlib.contextmanager
来源：http://iqu.yongpay.top

[U22] Py：矩阵转置
来源：http://dla.kuanghao11.cn

list(zip(*m))
来源：http://suy.hcnkem.com

[U23] Py：分块读取大文件
来源：http://esd.zdqjudy.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://ziz.feifeiyinyue.top

[U24] Py：路径操作
来源：http://mfc.hammf.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://dcc.aizwys.cn

[U25] Py：CSV 按字典读
来源：http://dnw.jyoumei.cn

csv.DictReader(f)
来源：http://fhh.hcnkem.com

[U26] Py：并发下载
来源：http://qmq.dashuyun.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://ove.shuidangran.top

[U27] Py：异步 HTTP
来源：http://nmj.iojbl.cn

aiohttp.ClientSession() 配合 async with
来源：http://zvm.yj202588.top

[U28] Py：类型别名
来源：http://oiw.gogol.net.cn

UserId = int
来源：http://jcd.shzxlz.cn

[U29] Py：属性校验
来源：http://bsm.dashuyun.cn

@property 与 @x.setter 配合
来源：http://msi.tarul.cn

[U30] Py：数据类
来源：http://lnd.zdbjq.cn

@dataclass(slots=True)
来源：http://roq.guannengcc.top

[U31] Py：单测
来源：http://xsf.fehbvm.com

python -m pytest -q
来源：http://nlv.yvedp.cn

[U32] Py：代码格式化
来源：http://ofq.pycfn.com

ruff format . && ruff check --fix .
来源：http://ueb.quarkkingdee.top

[U33] Py：打包发布
来源：http://jbw.shangyingyoupin.top

python -m build  （依赖 pyproject.toml）
来源：http://sia.shanyushiyangkeji.top

[U34] Py：判断编码
来源：http://pcs.hysaishi.cn

chardet.detect(raw)
来源：http://vop.ydzc1.top

[U35] Py：发送邮件
来源：http://roq.yj20258.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://mzs.ydjk.org.cn

[U36] Py：定时任务
来源：http://icy.nanxinkj.top

schedule.every(10).minutes.do(job)
来源：http://rfu.sweek.top

[U37] Py：读写 Excel
来源：http://kor.dashuyun.cn

pandas.read_excel / DataFrame.to_excel
来源：http://jgs.vqdsnc.cn

[U38] Py：获取脚本所在目录
来源：http://eqv.yanxiufei.cn

Path(__file__).resolve().parent
来源：http://bpa.yonumen.top

[U39] Py：判断是否在交互环境
来源：http://hhb.aizwys.cn

sys.stdout.isatty()
来源：http://swg.zhixingplan.top

[U40] Py：打印到标准错误
来源：http://auc.yuanzhike.top

print("err", file=sys.stderr)
来源：http://fdg.wangshuangyany.cn

[U41] PHP：初始化 Composer 项目
来源：http://zhw.hesvh.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://lkf.jianghu66.top

[U42] PHP：PSR-4 自动加载
来源：http://dsl.xziqi.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://flo.ctjpmb.com

[U43] PHP：声明命名空间
来源：http://fki.ctjpmb.com

namespace App\Http;
来源：http://oqe.hesvh.cn

[U44] PHP：开启严格类型
来源：http://dvt.cqqwz.cn

declare(strict_types=1);
来源：http://sum.feifeiyinyue.top

[U45] PHP：类型声明与返回类型
来源：http://nfy.fktsv.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://lui.xingfuxueyuan.xyz

[U46] PHP：可空类型
来源：http://ojq.jiagoushi.top

?string $name = null
来源：http://nic.nanxuanxn.top

[U47] PHP：联合类型
来源：http://jrj.0kj1m.cn

int|string $id
来源：http://mps.fanxiaobao.xyz

[U48] PHP：纯枚举
来源：http://myb.pengpengdd.cyou

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://avs.kuanghao11.cn

[U49] PHP：只读属性
来源：http://ftj.yueranfly.top

public readonly string $name
来源：http://vkj.meibo888.top

[U50] PHP：构造器属性提升
来源：http://xse.shangyingyoupin.top

public function __construct(private int $id) {}
来源：http://opd.haohaochexian.top

[U51] PHP：数组解构
来源：http://dxh.chenjidiqi.icu

[$a, $b] = $arr;
来源：http://iob.cucudq.cn

[U52] PHP：箭头函数
来源：http://vzm.jianghu66.top

$double = fn($x) => $x * 2;
来源：http://son.shangyingyoupin.top

[U53] PHP：空合并运算符
来源：http://zag.yueranfly.top

$v = $a ?? $b ?? "default";
来源：http://uug.yfazqb.com

[U54] PHP：空安全调用
来源：http://qim.hfpthk.cn

$obj?->method()
来源：http://zum.chenlongwang.top

[U55] PHP：match 表达式
来源：http://pau.cdnleiting.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://yih.fehbvm.com

[U56] PHP：命名参数
来源：http://wzw.yanxiufei.cn

f(a: 1, b: 2)
来源：http://sbb.hcnkem.com

[U57] PHP：字符串插值
来源：http://wgw.havefunace.top

"值: {$a}"
来源：http://mme.c1oappe.top

[U58] PHP：数组三件套
来源：http://bar.snrcjt.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://qdl.xziqi.cn

[U59] PHP：自定义排序
来源：http://lpw.gogol.net.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hnl.xinyue.icu

[U60] PHP：JSON 编解码
来源：http://xeb.mhx1999.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://eps.ehwqpu.com

[U61] PHP：正则
来源：http://erl.wangshuangyany.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://feq.nanxuanxn.top

[U62] PHP：日期对象
来源：http://eqv.guowangkeji.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://rgd.ctjpmb.com

[U63] PHP：文件读写
来源：http://qmz.sjlbkw.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://tet.hongshengwenyu.top

[U64] PHP：目录遍历
来源：http://uxl.gotoacloud.top

glob("dir/*.php");  scandir("dir");
来源：http://urh.tarul.cn

[U65] PHP：会话
来源：http://asn.meibo888.top

session_start();  $_SESSION["uid"] = 1;
来源：http://plp.kuanghao11.cn

[U66] PHP：设置 Cookie
来源：http://nid.chenjidiqi.icu

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://yrb.daxiang520.top

[U67] PHP：处理文件上传
来源：http://vlh.svipenyu.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://rki.wangshuangyany.cn

[U68] PHP：PDO 连接
来源：http://evf.fktsv.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://dga.jianghu66.top

[U69] PHP：PDO 预处理
来源：http://kiz.cucudq.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://nhn.chenzaomai.com

[U70] PHP：PDO 事务
来源：http://dea.sysykeji.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://zci.yfazqb.com

[U71] PHP：抛出异常
来源：http://dkw.zdbjq.cn

throw new RuntimeException("失败", 500);
来源：http://tjf.0kj1m.cn

[U72] PHP：写错误日志
来源：http://ahd.hesvh.cn

error_log("失败: " . $e->getMessage());
来源：http://ttr.nwbrower.top

[U73] PHP：读取 ini 配置
来源：http://awl.gaohongyu789.top

parse_ini_file("config.ini", true)
来源：http://ngp.xinyue.icu

[U74] PHP：读取环境变量
来源：http://ztn.cdnleiting.top

getenv("APP_ENV") ?: "production"
来源：http://ckm.yj20258888.top

[U75] PHP：依赖注入
来源：http://lqz.haohaochexian.top

composer require psr/container
来源：http://dtf.cheryme.top

[U76] PHP：简单路由
来源：http://ioa.aibaodan.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://ukk.yangfankeji.com

[U77] PHP：模板渲染
来源：http://jev.shanyushiyangtech.top

composer require twig/twig
来源：http://vpa.fehbvm.com

[U78] PHP：单元测试
来源：http://vso.svipenyu.cn

composer require --dev phpunit/phpunit
来源：http://uln.chenzaomai.com

[U79] PHP：静态分析
来源：http://ldz.yj20258888.top

composer require --dev phpstan/phpstan
来源：http://tsj.vehdjk.com

[U80] PHP：代码规范修复
来源：http://wnq.cucudq.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://pfv.fanxiaobao.xyz

[U81] JS：初始化项目
来源：http://kzd.pycfn.com

npm init -y;  npm i express
来源：http://bfn.yj20258888.top

[U82] JS：package.json 脚本
来源：http://nna.zdqjudy.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://lir.hammf.cn

[U83] JS：ES Module 导入导出
来源：http://pce.pengpengdd.cyou

export const a = 1;  import { a } from "./m.js";
来源：http://whd.jinqigufen.top

[U84] JS：CommonJS 写法
来源：http://rfv.vqdsnc.cn

module.exports = { a };  const { a } = require("./m");
来源：http://xsh.xinyue.icu

[U85] JS：可选链
来源：http://hfp.chenjidiqi.icu

a?.b?.c
来源：http://nxf.xuetiantiany.cn

[U86] JS：空值合并
来源：http://hmu.shzxlz.cn

a ?? b
来源：http://cif.chenlongwang.top

[U87] JS：解构默认值
来源：http://ofx.bjfxy.top

const { a = 1, b = 2 } = obj;
来源：http://qyk.0kj1m.cn

[U88] JS：对象展开合并
来源：http://omb.pengpengdd.cyou

{ ...a, ...b }
来源：http://ktd.yanxiufei.cn

[U89] JS：数组去重
来源：http://jka.svipenyu.cn

[...new Set(arr)]
来源：http://pfq.sysykeji.top

[U90] JS：数字数组排序
来源：http://vxl.yj20258888.top

[...arr].sort((a, b) => a - b)
来源：http://hrh.andypj.xyz

[U91] JS：对象键值遍历
来源：http://srj.vehdjk.com

Object.entries(obj).forEach(([k, v]) => {});
来源：http://qzz.zdqjudy.top

[U92] JS：深拷贝
来源：http://tpb.ywan-chungtsiang.top

structuredClone(obj)
来源：http://lpa.zdbjq.cn

[U93] JS：模板字符串
来源：http://thd.shangyingyoupin.top

`共 ${n} 条`
来源：http://rlw.sufxvd.cn

[U94] JS：箭头函数
来源：http://kew.zhongyouzk.top

const double = x => x * 2;
来源：http://pnt.yuxming.cn

[U95] JS：Promise 包装
来源：http://ruc.xuanzx.com

new Promise((resolve, reject) => {})
来源：http://whp.smart0.xyz

[U96] JS：async/await 与异常
来源：http://itr.jlsjyb.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://gyz.zhaomingkeji.xyz

[U97] JS：并发请求
来源：http://cek.pengpengdd.cyou

await Promise.all(urls.map(u => fetch(u)))
来源：http://ggu.ehwqpu.com

[U98] JS：fetch 带 JSON
来源：http://epk.zhoulong.xyz

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://axl.yj20258888.top

[U99] JS：事件监听
来源：http://obz.guowangkeji.top

el.addEventListener("click", e => {})
来源：http://ahn.jianghu66.top

[U100] JS：DOM 查询
来源：http://lnc.xylfe.cn

document.querySelector(".item")
来源：http://liw.feifeiyinyue.top

[U101] JS：classList 操作
来源：http://cip.chenlongwang.top

el.classList.toggle("active")
来源：http://qbx.hesvh.cn

[U102] JS：本地存储
来源：http://cnx.fanxiaobao.xyz

localStorage.setItem("k", JSON.stringify(v))
来源：http://abj.yj20258.top

[U103] JS：定时器
来源：http://kmc.xuetiantiany.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://jfe.shanyushiyangkeji.top

[U104] JS：防抖
来源：http://lob.guowangkeji.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ana.yuxming.cn

[U105] JS：节流
来源：http://ler.tian-w.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://twc.fengsongda.top

[U106] JS：日期格式化
来源：http://qac.zdqjudy.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://uhw.ydzc1.top

[U107] JS：数字千分位
来源：http://wwr.hnqzz.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://pxe.redwolf501.top

[U108] JS：随机整数
来源：http://yrg.guowangkeji.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://akt.daria6918.cn

[U109] JS：数组分组
来源：http://ell.sjlbkw.cn

Object.groupBy(arr, x => x.type)
来源：http://dow.ydjk.org.cn

[U110] JS：数组分块
来源：http://prn.aibaodan.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://wmh.ehwqpu.com

[U111] JS：对象转 Map
来源：http://ghl.dashuyun.cn

new Map(Object.entries(obj))
来源：http://zas.zhaomingkeji.xyz

[U112] JS：字符串补位
来源：http://kxi.fktsv.cn

"7".padStart(3, "0")
来源：http://yxw.meibo888.top

[U113] JS：正则替换全部
来源：http://blw.zycfv.cn

s.replaceAll("a", "b")
来源：http://mzs.hfpthk.cn

[U114] JS：JSON 深比较
来源：http://xvq.jinyuanbaomall.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://rle.gaohongyu789.top

[U115] JS：生成 UUID
来源：http://pkh.havefunace.top

crypto.randomUUID()
来源：http://yho.epnwcf.com

[U116] JS：类型检查（JSDoc）
来源：http://dvt.yuanzhike.top

/** @param {string} name */ function f(name) {}
来源：http://fme.jianghu66.top

[U117] JS：单元测试
来源：http://wfb.gotoacloud.top

npm i -D vitest;  npx vitest
来源：http://gsm.xinyue.icu

[U118] JS：开发服务器
来源：http://uwz.guannengcc.top

npm i -D vite;  npx vite
来源：http://jjh.zdqjudy.top

[U119] JS：生产构建
来源：http://gyu.zhaomingkeji.xyz

npx vite build
来源：http://spr.dashuyun.cn

[U120] JS：读取环境变量（Vite）
来源：http://bxj.smart0.xyz

import.meta.env.VITE_API_URL
来源：http://nns.nwbrower.top

================================================================================
来源：http://gve.svipenyu.cn

统计汇总
来源：http://skg.dianchejie.cn

================================================================================
来源：http://wch.yvedp.cn

按语言统计（条）：
来源：http://qnx.9152youxi.cn

Python ......... 252
来源：http://wjc.chenzaomai.com

PHP ............ 252
来源：http://wrm.gaohongyu789.top

JavaScript ..... 252
来源：http://dol.hywenlv.cn

TypeScript ..... 212
来源：http://idw.fengsongda.top

Java ........... 212
来源：http://cxc.shzxlz.cn

Go ............. 212
来源：http://gjr.sxryk.cn

Ruby ........... 212
来源：http://wqe.hcnkem.com

C# ............. 212
来源：http://amj.tian-w.cn

C .............. 30
来源：http://myh.yanxiufei.cn

C++ ............ 30
来源：http://bdq.andypj.xyz

SQL ............ 90
来源：http://whu.kuanghao11.cn

Bash ........... 80
来源：http://tfh.sjlbkw.cn

Kotlin ......... 15
来源：http://avp.zhongyouzk.top

Swift .......... 15
来源：http://owe.0kj1m.cn

Lua ............ 10
来源：http://fos.jianghu66.top

Perl ........... 10
来源：http://ubd.xuanzx.com

Scala .......... 10
来源：http://qre.quarkkingdee.top

------------------------------------
来源：http://azg.c1oappe.top

合计 ........... 2106 条
来源：http://bay.shzxlz.cn

按章节统计：
来源：http://hal.fanxiaobao.xyz

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://mlh.havefunace.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://oky.vehdjk.com

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://dah.zhixingplan.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://qft.jiagoushi.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://nju.yuanzhike.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://hbr.dashuyun.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://duu.xziqi.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://zvw.jinqigufen.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://iwi.aizwys.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://zer.tarul.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://ppn.sweek.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://crb.zdqjudy.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://sbo.c1oappe.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://lgw.ivvv.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://qno.yvedp.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://iea.shangyingyoupin.top


<!-- 参考信息 -->