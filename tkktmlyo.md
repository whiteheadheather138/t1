代发 wailian999

while (my $line = <$fh>) { print $line; }
来源：http://xdx.shanyushiyangkeji.top

[T51] Scala：Hello World
来源：http://vme.jinqigufen.top

println("Hello")
来源：http://hco.snrcjt.cn

[T52] Scala：变量
来源：http://roe.zhengqikj.top

val a = 1;  var b = 2
来源：http://qfg.jyoumei.cn

[T53] Scala：字符串插值
来源：http://enc.yj20258.top

s"值: $b"
来源：http://ijc.gotoacloud.top

[T54] Scala：集合映射
来源：http://jit.tianlin.xyz

List(1, 2, 3).map(_ * 2)
来源：http://hrw.fanxiaobao.xyz

[T55] Scala：集合过滤
来源：http://fim.fanxiaobao.xyz

List(1, 2, 3).filter(_ > 1)
来源：http://kar.shzxlz.cn

[T56] Scala：样例类
来源：http://oft.ydzc1.top

case class User(name: String, age: Int)
来源：http://ras.jyoumei.cn

[T57] Scala：模式匹配
来源：http://sao.yj202588.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://lwk.fzhhl.top

[T58] Scala：函数定义
来源：http://tce.tian-w.cn

def add(a: Int, b: Int): Int = a + b
来源：http://jrb.hnxiangtu.top

[T59] Scala：循环
来源：http://obz.xingfuxueyuan.xyz

for (i <- 1 to 10) println(i)
来源：http://scz.nanxuanxn.top

[T60] Scala：折叠
来源：http://laz.0kj1m.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://kry.cdnleiting.top

================================================================================
来源：http://tli.hongshengwenyu.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://ibv.nanxinkj.top

================================================================================
来源：http://glr.xuetiantiany.cn

[U01] Py：创建虚拟环境
来源：http://gif.fehbvm.com

python -m venv .venv && source .venv/bin/activate
来源：http://xnj.jinqigufen.top

[U02] Py：导出 / 安装依赖
来源：http://xwn.dianchejie.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://kds.yueranfly.top

[U03] Py：加载 .env 配置
来源：http://rbm.sufxvd.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://gwu.hammf.cn

[U04] Py：变量调试打印
来源：http://sxl.redwolf501.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://udo.zhongyouzk.top

[U05] Py：列表去重且保序
来源：http://sdt.nwbrower.top

list(dict.fromkeys(arr))
来源：http://gap.xylfe.cn

[U06] Py：合并两个字典
来源：http://djt.smart0.xyz

{**a, **b}
来源：http://ebu.shanyushiyangtech.top

[U07] Py：反转字典键值
来源：http://qak.cqqwz.cn

{v: k for k, v in d.items()}
来源：http://kdx.gaohongyu789.top

[U08] Py：展平二维列表
来源：http://snd.zhongyouzk.top

[y for x in nested for y in x]
来源：http://wmj.gogol.net.cn

[U09] Py：字典取最大值的键
来源：http://sue.chenlongwang.top

max(d, key=d.get)
来源：http://quj.yj202588.top

[U10] Py：按值排序字典
来源：http://eyc.jinyuanbaomall.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://cfm.fehbvm.com

[U11] Py：生成器表达式
来源：http://lwt.shzxlz.cn

(x * 2 for x in arr)
来源：http://uip.gzhubu.top

[U12] Py：取出现最多的 3 个元素
来源：http://wia.shanyushiyangkeji.top

Counter(arr).most_common(3)
来源：http://fst.dashuyun.cn

[U13] Py：固定长度队列
来源：http://jqi.9152youxi.cn

deque(maxlen=10)
来源：http://egl.vqdsnc.cn

[U14] Py：分组收集到列表
来源：http://dcb.wangdashe.top

defaultdict(list)
来源：http://idv.fengsongda.top

[U15] Py：高精度计时
来源：http://rrn.meibo888.top

t = time.perf_counter()
来源：http://yva.hesvh.cn

[U16] Py：命令行参数解析
来源：http://gws.tian-w.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://jdd.yonumen.top

[U17] Py：初始化日志
来源：http://ygh.yuanzhike.top

logging.basicConfig(level=logging.INFO)
来源：http://apr.shzxlz.cn

[U18] Py：预编译正则
来源：http://cer.hfpthk.cn

pat = re.compile(r"\d+")
来源：http://hmk.snrcjt.cn

[U19] Py：正则替换带回调
来源：http://iwy.guannengcc.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://kug.guannengcc.top

[U20] Py：缓存函数结果
来源：http://abj.316326.xyz

@functools.lru_cache(maxsize=None)
来源：http://rol.ctjpmb.com

[U21] Py：自定义上下文管理器
来源：http://myx.ywan-chungtsiang.top

@contextlib.contextmanager
来源：http://yot.jinyuanbaomall.cn

[U22] Py：矩阵转置
来源：http://ref.tanke756.top

list(zip(*m))
来源：http://lfc.hywenlv.cn

[U23] Py：分块读取大文件
来源：http://krv.jinqigfzy.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://rkf.cdnleiting.top

[U24] Py：路径操作
来源：http://aem.kuanghao11.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hhe.zhaomingkeji.xyz

[U25] Py：CSV 按字典读
来源：http://jau.yonumen.top

csv.DictReader(f)
来源：http://rud.yongpay.top

[U26] Py：并发下载
来源：http://gqf.tian-w.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://wxa.snrcjt.cn

[U27] Py：异步 HTTP
来源：http://nst.wangdashe.top

aiohttp.ClientSession() 配合 async with
来源：http://hwj.bjfxy.top

[U28] Py：类型别名
来源：http://lud.mhx1999.top

UserId = int
来源：http://vun.haohaochexian.top

[U29] Py：属性校验
来源：http://xlk.sweek.top

@property 与 @x.setter 配合
来源：http://jzh.hysaishi.cn

[U30] Py：数据类
来源：http://ico.birdmap.top

@dataclass(slots=True)
来源：http://zux.aibaodan.cn

[U31] Py：单测
来源：http://czq.gzhubu.top

python -m pytest -q
来源：http://pxe.nwbrower.top

[U32] Py：代码格式化
来源：http://npx.epnwcf.com

ruff format . && ruff check --fix .
来源：http://zhv.sysykeji.top

[U33] Py：打包发布
来源：http://ssj.xinyue.icu

python -m build  （依赖 pyproject.toml）
来源：http://bce.iojbl.cn

[U34] Py：判断编码
来源：http://dhm.kuanghao11.cn

chardet.detect(raw)
来源：http://lag.yonumen.top

[U35] Py：发送邮件
来源：http://pzf.yj20258.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://les.hnqzz.top

[U36] Py：定时任务
来源：http://mbu.hongshengwenyu.top

schedule.every(10).minutes.do(job)
来源：http://fvf.tian-w.cn

[U37] Py：读写 Excel
来源：http://tbz.gotoacloud.top

pandas.read_excel / DataFrame.to_excel
来源：http://qbz.wangshuangyany.cn

[U38] Py：获取脚本所在目录
来源：http://wug.jinqigfzy.top

Path(__file__).resolve().parent
来源：http://lbj.pengpengdd.cyou

[U39] Py：判断是否在交互环境
来源：http://onz.52xcode.cn

sys.stdout.isatty()
来源：http://utk.wangshuangyany.cn

[U40] Py：打印到标准错误
来源：http://htm.jyoumei.cn

print("err", file=sys.stderr)
来源：http://ocd.chenlongwang.top

[U41] PHP：初始化 Composer 项目
来源：http://ocp.hammf.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://ivc.yongpay.top

[U42] PHP：PSR-4 自动加载
来源：http://rzw.tanke756.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://tbd.shangyingyoupin.top

[U43] PHP：声明命名空间
来源：http://fbt.jqgufenzy.top

namespace App\Http;
来源：http://jkc.hysaishi.cn

[U44] PHP：开启严格类型
来源：http://usc.fehbvm.com

declare(strict_types=1);
来源：http://xwn.sweek.top

[U45] PHP：类型声明与返回类型
来源：http://bvm.zdbjq.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://acq.zhaomingkeji.xyz

[U46] PHP：可空类型
来源：http://doh.zhijiandao.cn

?string $name = null
来源：http://myp.bbcook.cn

[U47] PHP：联合类型
来源：http://wqn.iojbl.cn

int|string $id
来源：http://gym.jinghuilouyu.cn

[U48] PHP：纯枚举
来源：http://pqv.shuidangran.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://uiw.yanxiufei.cn

[U49] PHP：只读属性
来源：http://jlf.xuetiantiany.cn

public readonly string $name
来源：http://ncr.yueranfly.top

[U50] PHP：构造器属性提升
来源：http://umb.hysaishi.cn

public function __construct(private int $id) {}
来源：http://ovs.ydzc1.top

[U51] PHP：数组解构
来源：http://tkg.9152youxi.cn

[$a, $b] = $arr;
来源：http://oav.shzxlz.cn

[U52] PHP：箭头函数
来源：http://urf.jinghuilouyu.cn

$double = fn($x) => $x * 2;
来源：http://gls.hfpthk.cn

[U53] PHP：空合并运算符
来源：http://bxn.ybcxt.top

$v = $a ?? $b ?? "default";
来源：http://npk.nanxinkj.top

[U54] PHP：空安全调用
来源：http://grw.hysaishi.cn

$obj?->method()
来源：http://pzu.wangdashe.top

[U55] PHP：match 表达式
来源：http://txo.meibo888.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://kco.andypj.xyz

[U56] PHP：命名参数
来源：http://uhd.yongpay.top

f(a: 1, b: 2)
来源：http://ljo.xuanzx.com

[U57] PHP：字符串插值
来源：http://vbi.yvedp.cn

"值: {$a}"
来源：http://pes.cdnleiting.top

[U58] PHP：数组三件套
来源：http://qsk.birdmap.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://jtu.cucudq.cn

[U59] PHP：自定义排序
来源：http://xjs.pycfn.com

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hqq.epnwcf.com

[U60] PHP：JSON 编解码
来源：http://kdm.zhoulong.xyz

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://gtm.xziqi.cn

[U61] PHP：正则
来源：http://zks.vqdsnc.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://zth.9152youxi.cn

[U62] PHP：日期对象
来源：http://fky.xylfe.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://tsd.haohaochexian.top

[U63] PHP：文件读写
来源：http://kib.vehdjk.com

file_get_contents($f);  file_put_contents($f, $data);
来源：http://cbz.sweek.top

[U64] PHP：目录遍历
来源：http://afg.guowangkeji.top

glob("dir/*.php");  scandir("dir");
来源：http://wrp.gogol.net.cn

[U65] PHP：会话
来源：http://tex.snrcjt.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://rqu.birdmap.top

[U66] PHP：设置 Cookie
来源：http://dcb.aibaodan.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://dms.jiagoushi.top

[U67] PHP：处理文件上传
来源：http://dgh.yuxming.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://wbz.shzxlz.cn

[U68] PHP：PDO 连接
来源：http://kcb.haohaochexian.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://ktk.ydzc1.top

[U69] PHP：PDO 预处理
来源：http://fxu.ybcxt.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://iab.gotoacloud.top

[U70] PHP：PDO 事务
来源：http://btz.jinqigfzy.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://umv.yfazqb.com

[U71] PHP：抛出异常
来源：http://wzh.jqgfzy.top

throw new RuntimeException("失败", 500);
来源：http://dew.yanxiufei.cn

[U72] PHP：写错误日志
来源：http://swj.yuxming.cn

error_log("失败: " . $e->getMessage());
来源：http://ntl.zhaomingkeji.xyz

[U73] PHP：读取 ini 配置
来源：http://mbv.cucudq.cn

parse_ini_file("config.ini", true)
来源：http://vgd.aizwys.cn

[U74] PHP：读取环境变量
来源：http://qbt.yfazqb.com

getenv("APP_ENV") ?: "production"
来源：http://qlb.cashguo.top

[U75] PHP：依赖注入
来源：http://aax.daxiang520.top

composer require psr/container
来源：http://dmm.yuxming.cn

[U76] PHP：简单路由
来源：http://rwa.jqgfzy.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://bny.hnqzz.top

[U77] PHP：模板渲染
来源：http://brp.shzxlz.cn

composer require twig/twig
来源：http://gkb.zhiwuduotai.top

[U78] PHP：单元测试
来源：http://jhx.sysykeji.top

composer require --dev phpunit/phpunit
来源：http://cqs.fehbvm.com

[U79] PHP：静态分析
来源：http://vnh.tian-w.cn

composer require --dev phpstan/phpstan
来源：http://ltf.dashuyun.cn

[U80] PHP：代码规范修复
来源：http://vyr.yanxiufei.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://euc.ydjk.org.cn

[U81] JS：初始化项目
来源：http://ixw.zdbjq.cn

npm init -y;  npm i express
来源：http://jas.yonumen.top

[U82] JS：package.json 脚本
来源：http://iez.daxiang520.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://xbx.aizwys.cn

[U83] JS：ES Module 导入导出
来源：http://gjd.zhijiandao.cn

export const a = 1;  import { a } from "./m.js";
来源：http://lkm.yonumen.top

[U84] JS：CommonJS 写法
来源：http://kfo.yuanzhike.top

module.exports = { a };  const { a } = require("./m");
来源：http://vas.cheryme.top

[U85] JS：可选链
来源：http://eut.fengsongda.top

a?.b?.c
来源：http://mmy.xuetiantiany.cn

[U86] JS：空值合并
来源：http://tna.pycfn.com

a ?? b
来源：http://xuv.guowangkeji.top

[U87] JS：解构默认值
来源：http://baq.52xcode.cn

const { a = 1, b = 2 } = obj;
来源：http://ksi.shanyushiyangkeji.top

[U88] JS：对象展开合并
来源：http://doo.hcnkem.com

{ ...a, ...b }
来源：http://zys.gogol.net.cn

[U89] JS：数组去重
来源：http://hjb.jqgufenzy.top

[...new Set(arr)]
来源：http://gcs.epnwcf.com

[U90] JS：数字数组排序
来源：http://ece.svipenyu.cn

[...arr].sort((a, b) => a - b)
来源：http://jry.hnqzz.top

[U91] JS：对象键值遍历
来源：http://xlg.gotoacloud.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://pru.ehwqpu.com

[U92] JS：深拷贝
来源：http://lnt.daxiang520.top

structuredClone(obj)
来源：http://gvi.cheryme.top

[U93] JS：模板字符串
来源：http://iqf.vqdsnc.cn

`共 ${n} 条`
来源：http://ibd.quarkkingdee.top

[U94] JS：箭头函数
来源：http://vth.0kj1m.cn

const double = x => x * 2;
来源：http://vdg.svipenyu.cn

[U95] JS：Promise 包装
来源：http://qwd.yvedp.cn

new Promise((resolve, reject) => {})
来源：http://dto.nanxuanxn.top

[U96] JS：async/await 与异常
来源：http://kxv.jqgufenzy.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://sas.hnxiangtu.top

[U97] JS：并发请求
来源：http://cap.316326.xyz

await Promise.all(urls.map(u => fetch(u)))
来源：http://dli.shzxlz.cn

[U98] JS：fetch 带 JSON
来源：http://oaj.sufxvd.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://dwj.feifeiyinyue.top

[U99] JS：事件监听
来源：http://rmb.andypj.xyz

el.addEventListener("click", e => {})
来源：http://hnp.snrcjt.cn

[U100] JS：DOM 查询
来源：http://uih.xziqi.cn

document.querySelector(".item")
来源：http://ohe.cdnleiting.top

[U101] JS：classList 操作
来源：http://lnx.iojbl.cn

el.classList.toggle("active")
来源：http://qlr.jqgfzy.top

[U102] JS：本地存储
来源：http://uew.zhongyouzk.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://xpj.yj20258888.top

[U103] JS：定时器
来源：http://vfm.sufxvd.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://fhb.yangfankeji.com

[U104] JS：防抖
来源：http://kup.xylfe.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://jwy.cucudq.cn

[U105] JS：节流
来源：http://xkj.jqgfzy.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://wug.ywan-chungtsiang.top

[U106] JS：日期格式化
来源：http://jxg.cqqwz.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://rlu.ehwqpu.com

[U107] JS：数字千分位
来源：http://zjj.yvedp.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://bai.ybcxt.top

[U108] JS：随机整数
来源：http://kgy.wangdashe.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://riz.xylfe.cn

[U109] JS：数组分组
来源：http://ghj.cheryme.top

Object.groupBy(arr, x => x.type)
来源：http://nbv.hfpthk.cn

[U110] JS：数组分块
来源：http://vnu.zycfv.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://djx.hcnkem.com

[U111] JS：对象转 Map
来源：http://oif.yonumen.top

new Map(Object.entries(obj))
来源：http://hra.pycfn.com

[U112] JS：字符串补位
来源：http://qzn.chenzaomai.com

"7".padStart(3, "0")
来源：http://yej.dashuyun.cn

[U113] JS：正则替换全部
来源：http://dty.ydjk.org.cn

s.replaceAll("a", "b")
来源：http://iwl.yvedp.cn

[U114] JS：JSON 深比较
来源：http://oes.gotoacloud.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://uvg.dianchejie.cn

[U115] JS：生成 UUID
来源：http://axm.haohaochexian.top

crypto.randomUUID()
来源：http://hqq.sufxvd.cn

[U116] JS：类型检查（JSDoc）
来源：http://uaq.nanxinkj.top

/** @param {string} name */ function f(name) {}
来源：http://pkp.tanke756.top

[U117] JS：单元测试
来源：http://pcf.sxryk.cn

npm i -D vitest;  npx vitest
来源：http://qkf.tian-w.cn

[U118] JS：开发服务器
来源：http://lza.xylfe.cn

npm i -D vite;  npx vite
来源：http://vuo.zhongyouzk.top

[U119] JS：生产构建
来源：http://qaw.fktsv.cn

npx vite build
来源：http://oxh.jinghuilouyu.cn

[U120] JS：读取环境变量（Vite）
来源：http://xft.tarul.cn

import.meta.env.VITE_API_URL
来源：http://xen.jiagoushi.top

================================================================================
来源：http://yhk.cdnleiting.top

统计汇总
来源：http://abc.xuanzx.com

================================================================================
来源：http://bcx.yanxiufei.cn

按语言统计（条）：
来源：http://qno.hysaishi.cn

Python ......... 252
来源：http://lax.zdbjq.cn

PHP ............ 252
来源：http://wru.hysaishi.cn

JavaScript ..... 252
来源：http://ole.feifeiyinyue.top

TypeScript ..... 212
来源：http://wxk.tanke756.top

Java ........... 212
来源：http://ypy.yueranfly.top

Go ............. 212
来源：http://uld.yonumen.top

Ruby ........... 212
来源：http://ves.zhiwuduotai.top

C# ............. 212
来源：http://qlt.birdmap.top

C .............. 30
来源：http://mhw.birdmap.top

C++ ............ 30
来源：http://dma.zhoulong.xyz

SQL ............ 90
来源：http://sfc.zhengqikj.top

Bash ........... 80
来源：http://szd.zhijiandao.cn

Kotlin ......... 15
来源：http://mjq.jqgufenzy.top

Swift .......... 15
来源：http://jlt.svipenyu.cn

Lua ............ 10
来源：http://bxf.yfazqb.com

Perl ........... 10
来源：http://pxy.bbcook.cn

Scala .......... 10
来源：http://pww.hammf.cn

------------------------------------
来源：http://dfu.zhongyouzk.top

合计 ........... 2106 条
来源：http://efn.hnqzz.top

按章节统计：
来源：http://krp.daxiang520.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://tgu.yj202588.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://vqe.fzhhl.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hxz.zhongyouzk.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://xhf.hammf.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://dph.hfpthk.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://phv.ehwqpu.com

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://sey.pengpengdd.cyou

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://gir.xingfuxueyuan.xyz

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://qor.wangshuangyany.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://dsa.zhijiandao.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://ddr.hcnkem.com

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://lsx.zdqjudy.top


<!-- 参考信息 -->