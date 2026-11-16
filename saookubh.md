代发 wailian999

while (my $line = <$fh>) { print $line; }
来源：http://vsi.zdqjudy.top

[T51] Scala：Hello World
来源：http://ovu.hywenlv.cn

println("Hello")
来源：http://auc.xuanzx.com

[T52] Scala：变量
来源：http://len.wangdashe.top

val a = 1;  var b = 2
来源：http://div.yonumen.top

[T53] Scala：字符串插值
来源：http://rhl.smart0.xyz

s"值: $b"
来源：http://vcp.jianghu66.top

[T54] Scala：集合映射
来源：http://xgi.haohaochexian.top

List(1, 2, 3).map(_ * 2)
来源：http://iii.zycfv.cn

[T55] Scala：集合过滤
来源：http://vkl.chenjidiqi.icu

List(1, 2, 3).filter(_ > 1)
来源：http://pav.smart0.xyz

[T56] Scala：样例类
来源：http://ert.ybcxt.top

case class User(name: String, age: Int)
来源：http://cwi.sweek.top

[T57] Scala：模式匹配
来源：http://hcj.yongpay.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://uvp.zhixingplan.top

[T58] Scala：函数定义
来源：http://aae.yj20258888.top

def add(a: Int, b: Int): Int = a + b
来源：http://kwg.sysykeji.top

[T59] Scala：循环
来源：http://hds.zhongyouzk.top

for (i <- 1 to 10) println(i)
来源：http://len.0kj1m.cn

[T60] Scala：折叠
来源：http://fxd.shanyushiyangtech.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://dhm.chenjidiqi.icu

================================================================================
来源：http://ekz.zhixingplan.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://lnh.vehdjk.com

================================================================================
来源：http://wrt.cucudq.cn

[U01] Py：创建虚拟环境
来源：http://wmb.dashuyun.cn

python -m venv .venv && source .venv/bin/activate
来源：http://nqn.uphjek.com

[U02] Py：导出 / 安装依赖
来源：http://bhd.fktsv.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://sas.smart0.xyz

[U03] Py：加载 .env 配置
来源：http://pnm.cqqwz.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://nmu.shzxlz.cn

[U04] Py：变量调试打印
来源：http://fvv.yanxiufei.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://bwn.xziqi.cn

[U05] Py：列表去重且保序
来源：http://wxm.zhengqikj.top

list(dict.fromkeys(arr))
来源：http://ioo.fktsv.cn

[U06] Py：合并两个字典
来源：http://vsh.ppjwa.cn

{**a, **b}
来源：http://jhq.hfpthk.cn

[U07] Py：反转字典键值
来源：http://rjs.sweek.top

{v: k for k, v in d.items()}
来源：http://ppu.guannengcc.top

[U08] Py：展平二维列表
来源：http://jku.yangfankeji.com

[y for x in nested for y in x]
来源：http://zkn.c1oappe.top

[U09] Py：字典取最大值的键
来源：http://rgn.yanxiufei.cn

max(d, key=d.get)
来源：http://ylq.jinghuilouyu.cn

[U10] Py：按值排序字典
来源：http://vvj.jlsjyb.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://jfi.cucudq.cn

[U11] Py：生成器表达式
来源：http://rim.redwolf501.top

(x * 2 for x in arr)
来源：http://oat.ppjwa.cn

[U12] Py：取出现最多的 3 个元素
来源：http://fty.zycfv.cn

Counter(arr).most_common(3)
来源：http://jbq.kuanghao11.cn

[U13] Py：固定长度队列
来源：http://krj.jqgufenzy.top

deque(maxlen=10)
来源：http://gae.zhijiandao.cn

[U14] Py：分组收集到列表
来源：http://drk.jinqigufen.top

defaultdict(list)
来源：http://rnl.jinghuilouyu.cn

[U15] Py：高精度计时
来源：http://vpm.zhongyouzk.top

t = time.perf_counter()
来源：http://zpz.316326.xyz

[U16] Py：命令行参数解析
来源：http://wja.shuidangran.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://guk.yuxming.cn

[U17] Py：初始化日志
来源：http://udl.jinyuanbaomall.cn

logging.basicConfig(level=logging.INFO)
来源：http://gfx.zycfv.cn

[U18] Py：预编译正则
来源：http://dcz.zhiwuduotai.top

pat = re.compile(r"\d+")
来源：http://bps.cashguo.top

[U19] Py：正则替换带回调
来源：http://fwa.sysykeji.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://rxd.cqqwz.cn

[U20] Py：缓存函数结果
来源：http://tvz.ivvv.top

@functools.lru_cache(maxsize=None)
来源：http://zqf.pycfn.com

[U21] Py：自定义上下文管理器
来源：http://lvz.ctjpmb.com

@contextlib.contextmanager
来源：http://yyq.tianlin.xyz

[U22] Py：矩阵转置
来源：http://nuo.tian-w.cn

list(zip(*m))
来源：http://yan.kuanghao11.cn

[U23] Py：分块读取大文件
来源：http://haa.yueranfly.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://vua.uphjek.com

[U24] Py：路径操作
来源：http://bmu.havefunace.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://qko.aizwys.cn

[U25] Py：CSV 按字典读
来源：http://fse.daria6918.cn

csv.DictReader(f)
来源：http://qhj.yj20258888.top

[U26] Py：并发下载
来源：http://nyl.hammf.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://wmu.zhengqikj.top

[U27] Py：异步 HTTP
来源：http://pzf.hysaishi.cn

aiohttp.ClientSession() 配合 async with
来源：http://jgm.nanxinkj.top

[U28] Py：类型别名
来源：http://pna.nanxinkj.top

UserId = int
来源：http://myg.daria6918.cn

[U29] Py：属性校验
来源：http://dld.sufxvd.cn

@property 与 @x.setter 配合
来源：http://yvk.cucudq.cn

[U30] Py：数据类
来源：http://nbz.9152youxi.cn

@dataclass(slots=True)
来源：http://yxy.hnqzz.top

[U31] Py：单测
来源：http://jts.jinyuanbaomall.cn

python -m pytest -q
来源：http://osw.xziqi.cn

[U32] Py：代码格式化
来源：http://mjh.fanxiaobao.xyz

ruff format . && ruff check --fix .
来源：http://ytp.jinqigufen.top

[U33] Py：打包发布
来源：http://rxj.smart0.xyz

python -m build  （依赖 pyproject.toml）
来源：http://bmv.zhoulong.xyz

[U34] Py：判断编码
来源：http://frb.yvedp.cn

chardet.detect(raw)
来源：http://wjr.ywan-chungtsiang.top

[U35] Py：发送邮件
来源：http://ire.cashguo.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://med.jinqigfzy.top

[U36] Py：定时任务
来源：http://cen.vehdjk.com

schedule.every(10).minutes.do(job)
来源：http://ukq.gotoacloud.top

[U37] Py：读写 Excel
来源：http://fgt.redwolf501.top

pandas.read_excel / DataFrame.to_excel
来源：http://rot.wangshuangyany.cn

[U38] Py：获取脚本所在目录
来源：http://avs.cqqwz.cn

Path(__file__).resolve().parent
来源：http://gsm.andypj.xyz

[U39] Py：判断是否在交互环境
来源：http://etx.zdqjudy.top

sys.stdout.isatty()
来源：http://uji.hnqzz.top

[U40] Py：打印到标准错误
来源：http://jyk.yangfankeji.com

print("err", file=sys.stderr)
来源：http://ksa.gaohongyu789.top

[U41] PHP：初始化 Composer 项目
来源：http://eyv.zhijiandao.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://det.cheryme.top

[U42] PHP：PSR-4 自动加载
来源：http://vuk.jiagoushi.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://gph.hnxiangtu.top

[U43] PHP：声明命名空间
来源：http://qik.andypj.xyz

namespace App\Http;
来源：http://jie.hnxiangtu.top

[U44] PHP：开启严格类型
来源：http://oyq.9152youxi.cn

declare(strict_types=1);
来源：http://pny.yongpay.top

[U45] PHP：类型声明与返回类型
来源：http://aaa.cqqwz.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://nuq.nwbrower.top

[U46] PHP：可空类型
来源：http://wvf.pengpengdd.cyou

?string $name = null
来源：http://cil.svipenyu.cn

[U47] PHP：联合类型
来源：http://ipo.pengpengdd.cyou

int|string $id
来源：http://ntm.zhongyouzk.top

[U48] PHP：纯枚举
来源：http://zej.redwolf501.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://udy.sweek.top

[U49] PHP：只读属性
来源：http://sfc.yonumen.top

public readonly string $name
来源：http://uap.wangdashe.top

[U50] PHP：构造器属性提升
来源：http://okr.shuidangran.top

public function __construct(private int $id) {}
来源：http://rjr.wangshuangyany.cn

[U51] PHP：数组解构
来源：http://xwq.zhongyouzk.top

[$a, $b] = $arr;
来源：http://tft.jinqigfzy.top

[U52] PHP：箭头函数
来源：http://kuh.shzxlz.cn

$double = fn($x) => $x * 2;
来源：http://czb.fanxiaobao.xyz

[U53] PHP：空合并运算符
来源：http://dpe.zdqjudy.top

$v = $a ?? $b ?? "default";
来源：http://sxi.tarul.cn

[U54] PHP：空安全调用
来源：http://gba.dianchejie.cn

$obj?->method()
来源：http://ezu.ydzc1.top

[U55] PHP：match 表达式
来源：http://uei.hfpthk.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://umt.cucudq.cn

[U56] PHP：命名参数
来源：http://jtk.ppjwa.cn

f(a: 1, b: 2)
来源：http://rkl.chenjidiqi.icu

[U57] PHP：字符串插值
来源：http://fnx.ehwqpu.com

"值: {$a}"
来源：http://dqw.cheryme.top

[U58] PHP：数组三件套
来源：http://arz.yongpay.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://npo.yueranfly.top

[U59] PHP：自定义排序
来源：http://lws.jqgfzy.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://giu.guowangkeji.top

[U60] PHP：JSON 编解码
来源：http://wqj.quarkkingdee.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://gip.cqqwz.cn

[U61] PHP：正则
来源：http://rdc.cheryme.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://ekf.jlsjyb.cn

[U62] PHP：日期对象
来源：http://nnb.hesvh.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://sta.hesvh.cn

[U63] PHP：文件读写
来源：http://iim.ctjpmb.com

file_get_contents($f);  file_put_contents($f, $data);
来源：http://gge.nanxinkj.top

[U64] PHP：目录遍历
来源：http://ywm.sufxvd.cn

glob("dir/*.php");  scandir("dir");
来源：http://gpa.yj20258.top

[U65] PHP：会话
来源：http://ufc.c1oappe.top

session_start();  $_SESSION["uid"] = 1;
来源：http://eeu.jlsjyb.cn

[U66] PHP：设置 Cookie
来源：http://xso.yvedp.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://nss.yuanzhike.top

[U67] PHP：处理文件上传
来源：http://cct.nanxuanxn.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://wnn.zhixingplan.top

[U68] PHP：PDO 连接
来源：http://gfe.kuanghao11.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://clz.zdqjudy.top

[U69] PHP：PDO 预处理
来源：http://fye.fktsv.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://mex.tanke756.top

[U70] PHP：PDO 事务
来源：http://eaw.c1oappe.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://sgd.chenjidiqi.icu

[U71] PHP：抛出异常
来源：http://lon.tianlin.xyz

throw new RuntimeException("失败", 500);
来源：http://eeu.cheryme.top

[U72] PHP：写错误日志
来源：http://exv.sysykeji.top

error_log("失败: " . $e->getMessage());
来源：http://hpy.yfazqb.com

[U73] PHP：读取 ini 配置
来源：http://wkw.tarul.cn

parse_ini_file("config.ini", true)
来源：http://gun.tianlin.xyz

[U74] PHP：读取环境变量
来源：http://zve.zhoulong.xyz

getenv("APP_ENV") ?: "production"
来源：http://vnc.shangyingyoupin.top

[U75] PHP：依赖注入
来源：http://nul.fanxiaobao.xyz

composer require psr/container
来源：http://yny.nwbrower.top

[U76] PHP：简单路由
来源：http://xyy.iojbl.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://yld.aizwys.cn

[U77] PHP：模板渲染
来源：http://zrx.yangfankeji.com

composer require twig/twig
来源：http://wsn.jlsjyb.cn

[U78] PHP：单元测试
来源：http://nnf.vqdsnc.cn

composer require --dev phpunit/phpunit
来源：http://zkz.tianlin.xyz

[U79] PHP：静态分析
来源：http://tnj.hcnkem.com

composer require --dev phpstan/phpstan
来源：http://syx.sufxvd.cn

[U80] PHP：代码规范修复
来源：http://ihv.jinyuanbaomall.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://fio.zhaomingkeji.xyz

[U81] JS：初始化项目
来源：http://rer.ppjwa.cn

npm init -y;  npm i express
来源：http://dfi.zhixingplan.top

[U82] JS：package.json 脚本
来源：http://nby.hywenlv.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://bbm.smart0.xyz

[U83] JS：ES Module 导入导出
来源：http://znf.daria6918.cn

export const a = 1;  import { a } from "./m.js";
来源：http://tew.jyoumei.cn

[U84] JS：CommonJS 写法
来源：http://iif.yj202588.top

module.exports = { a };  const { a } = require("./m");
来源：http://nbt.sxryk.cn

[U85] JS：可选链
来源：http://fib.haohaochexian.top

a?.b?.c
来源：http://xju.hfpthk.cn

[U86] JS：空值合并
来源：http://ymp.9152youxi.cn

a ?? b
来源：http://zgw.ivvv.top

[U87] JS：解构默认值
来源：http://lrq.wangdashe.top

const { a = 1, b = 2 } = obj;
来源：http://elq.zhongyouzk.top

[U88] JS：对象展开合并
来源：http://gwc.tanke756.top

{ ...a, ...b }
来源：http://ybe.52xcode.cn

[U89] JS：数组去重
来源：http://nvi.vehdjk.com

[...new Set(arr)]
来源：http://rdp.shangyingyoupin.top

[U90] JS：数字数组排序
来源：http://dlr.ctjpmb.com

[...arr].sort((a, b) => a - b)
来源：http://orv.hnqzz.top

[U91] JS：对象键值遍历
来源：http://kvz.nanxuanxn.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://zfi.xuanzx.com

[U92] JS：深拷贝
来源：http://gag.gaohongyu789.top

structuredClone(obj)
来源：http://hak.cqqwz.cn

[U93] JS：模板字符串
来源：http://uku.ivvv.top

`共 ${n} 条`
来源：http://wma.ivvv.top

[U94] JS：箭头函数
来源：http://izc.chenlongwang.top

const double = x => x * 2;
来源：http://rlw.andypj.xyz

[U95] JS：Promise 包装
来源：http://yzh.fehbvm.com

new Promise((resolve, reject) => {})
来源：http://tht.dianchejie.cn

[U96] JS：async/await 与异常
来源：http://mws.hysaishi.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://qzq.pengpengdd.cyou

[U97] JS：并发请求
来源：http://wqk.fktsv.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://ihi.jinqigufen.top

[U98] JS：fetch 带 JSON
来源：http://tuf.jyoumei.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://dud.hywenlv.cn

[U99] JS：事件监听
来源：http://tcg.zhengqikj.top

el.addEventListener("click", e => {})
来源：http://fyh.jyoumei.cn

[U100] JS：DOM 查询
来源：http://iel.chenlongwang.top

document.querySelector(".item")
来源：http://pes.havefunace.top

[U101] JS：classList 操作
来源：http://xhk.xinyue.icu

el.classList.toggle("active")
来源：http://nim.zhoulong.xyz

[U102] JS：本地存储
来源：http://vhl.gzhubu.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://fnv.xylfe.cn

[U103] JS：定时器
来源：http://opw.yj20258888.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://jiy.cqqwz.cn

[U104] JS：防抖
来源：http://wms.feifeiyinyue.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://szb.yj20258888.top

[U105] JS：节流
来源：http://pno.hnqzz.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://dja.dashuyun.cn

[U106] JS：日期格式化
来源：http://xfg.daxiang520.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://rie.ehwqpu.com

[U107] JS：数字千分位
来源：http://pzb.jianghu66.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://imc.xuanzx.com

[U108] JS：随机整数
来源：http://smg.zhiwuduotai.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://umk.xingfuxueyuan.xyz

[U109] JS：数组分组
来源：http://xww.meibo888.top

Object.groupBy(arr, x => x.type)
来源：http://ros.guowangkeji.top

[U110] JS：数组分块
来源：http://udr.shzxlz.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://fgu.shzxlz.cn

[U111] JS：对象转 Map
来源：http://ifc.yueranfly.top

new Map(Object.entries(obj))
来源：http://yja.zhaomingkeji.xyz

[U112] JS：字符串补位
来源：http://gwq.yfazqb.com

"7".padStart(3, "0")
来源：http://mhb.pengpengdd.cyou

[U113] JS：正则替换全部
来源：http://uuh.smart0.xyz

s.replaceAll("a", "b")
来源：http://drj.zhixingplan.top

[U114] JS：JSON 深比较
来源：http://ayg.gzhubu.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://vog.cqqwz.cn

[U115] JS：生成 UUID
来源：http://hqu.sjlbkw.cn

crypto.randomUUID()
来源：http://nsr.gzhubu.top

[U116] JS：类型检查（JSDoc）
来源：http://pik.guowangkeji.top

/** @param {string} name */ function f(name) {}
来源：http://kqc.gzhubu.top

[U117] JS：单元测试
来源：http://xge.52xcode.cn

npm i -D vitest;  npx vitest
来源：http://ggl.fanxiaobao.xyz

[U118] JS：开发服务器
来源：http://hop.birdmap.top

npm i -D vite;  npx vite
来源：http://cea.yangfankeji.com

[U119] JS：生产构建
来源：http://cbp.jinqigufen.top

npx vite build
来源：http://ztz.316326.xyz

[U120] JS：读取环境变量（Vite）
来源：http://svc.zhengqikj.top

import.meta.env.VITE_API_URL
来源：http://wgm.shanyushiyangkeji.top

================================================================================
来源：http://owl.c1oappe.top

统计汇总
来源：http://mss.gogol.net.cn

================================================================================
来源：http://sxq.hesvh.cn

按语言统计（条）：
来源：http://njb.bjfxy.top

Python ......... 252
来源：http://beq.fehbvm.com

PHP ............ 252
来源：http://dgv.zhaomingkeji.xyz

JavaScript ..... 252
来源：http://mwn.cucudq.cn

TypeScript ..... 212
来源：http://rda.jqgfzy.top

Java ........... 212
来源：http://pwb.bjfxy.top

Go ............. 212
来源：http://puc.nanxuanxn.top

Ruby ........... 212
来源：http://tdk.havefunace.top

C# ............. 212
来源：http://ypv.fehbvm.com

C .............. 30
来源：http://hji.ivvv.top

C++ ............ 30
来源：http://iop.shanyushiyangkeji.top

SQL ............ 90
来源：http://qfc.316326.xyz

Bash ........... 80
来源：http://xuu.nwbrower.top

Kotlin ......... 15
来源：http://bsa.feifeiyinyue.top

Swift .......... 15
来源：http://upz.gzhubu.top

Lua ............ 10
来源：http://bpi.aizwys.cn

Perl ........... 10
来源：http://eml.shanyushiyangkeji.top

Scala .......... 10
来源：http://rfi.fengsongda.top

------------------------------------
来源：http://wna.yj20258888.top

合计 ........... 2106 条
来源：http://exv.fktsv.cn

按章节统计：
来源：http://vgg.sweek.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://ptu.fehbvm.com

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://lcp.cashguo.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://xmi.shanyushiyangkeji.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://sdf.zhaomingkeji.xyz

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://irw.iojbl.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://evr.xylfe.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://vit.ivvv.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hts.xuetiantiany.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://leu.hnxiangtu.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://nou.tanke756.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://ahn.chenlongwang.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://ajd.daria6918.cn


<!-- 参考信息 -->