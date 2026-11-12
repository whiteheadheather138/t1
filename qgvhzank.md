代发 wailian999

[T49] Perl：函数
来源：http://cuo.wangdashe.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://htd.shangyingyoupin.top

[T50] Perl：逐行读文件
来源：http://cbs.xziqi.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://xya.jqgfzy.top

while (my $line = <$fh>) { print $line; }
来源：http://sga.shanyushiyangkeji.top

[T51] Scala：Hello World
来源：http://alw.hcnkem.com

println("Hello")
来源：http://zza.jinghuilouyu.cn

[T52] Scala：变量
来源：http://tqq.fengsongda.top

val a = 1;  var b = 2
来源：http://agb.nwbrower.top

[T53] Scala：字符串插值
来源：http://mop.haohaochexian.top

s"值: $b"
来源：http://tvb.tian-w.cn

[T54] Scala：集合映射
来源：http://lau.sweek.top

List(1, 2, 3).map(_ * 2)
来源：http://unq.zhongyouzk.top

[T55] Scala：集合过滤
来源：http://pvm.wangdashe.top

List(1, 2, 3).filter(_ > 1)
来源：http://vez.fzhhl.top

[T56] Scala：样例类
来源：http://qpl.9152youxi.cn

case class User(name: String, age: Int)
来源：http://iau.chenjidiqi.icu

[T57] Scala：模式匹配
来源：http://ttv.yuxming.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://jmo.jinqigufen.top

[T58] Scala：函数定义
来源：http://ytd.aizwys.cn

def add(a: Int, b: Int): Int = a + b
来源：http://cpi.ydjk.org.cn

[T59] Scala：循环
来源：http://inc.sjlbkw.cn

for (i <- 1 to 10) println(i)
来源：http://pcg.ywan-chungtsiang.top

[T60] Scala：折叠
来源：http://kzt.ybcxt.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://bmn.nwbrower.top

================================================================================
来源：http://bgj.52xcode.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://zno.tian-w.cn

================================================================================
来源：http://hyl.yuanzhike.top

[U01] Py：创建虚拟环境
来源：http://vwh.316326.xyz

python -m venv .venv && source .venv/bin/activate
来源：http://itx.yueranfly.top

[U02] Py：导出 / 安装依赖
来源：http://khy.fehbvm.com

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://xuk.yfazqb.com

[U03] Py：加载 .env 配置
来源：http://lbf.cqqwz.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://egb.zhixingplan.top

[U04] Py：变量调试打印
来源：http://xmi.gotoacloud.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://oaa.yongpay.top

[U05] Py：列表去重且保序
来源：http://vug.gaohongyu789.top

list(dict.fromkeys(arr))
来源：http://rnd.nanxinkj.top

[U06] Py：合并两个字典
来源：http://nbr.pengpengdd.cyou

{**a, **b}
来源：http://rxx.zdqjudy.top

[U07] Py：反转字典键值
来源：http://jxy.jyoumei.cn

{v: k for k, v in d.items()}
来源：http://jpt.ppjwa.cn

[U08] Py：展平二维列表
来源：http://lui.pengpengdd.cyou

[y for x in nested for y in x]
来源：http://pcy.gotoacloud.top

[U09] Py：字典取最大值的键
来源：http://ivj.ehwqpu.com

max(d, key=d.get)
来源：http://ues.yongpay.top

[U10] Py：按值排序字典
来源：http://mkn.xylfe.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://wsf.snrcjt.cn

[U11] Py：生成器表达式
来源：http://qmd.jinqigfzy.top

(x * 2 for x in arr)
来源：http://jpx.daxiang520.top

[U12] Py：取出现最多的 3 个元素
来源：http://jaj.gzhubu.top

Counter(arr).most_common(3)
来源：http://xsf.bjfxy.top

[U13] Py：固定长度队列
来源：http://wxl.hnxiangtu.top

deque(maxlen=10)
来源：http://jna.sxryk.cn

[U14] Py：分组收集到列表
来源：http://xmy.gzhubu.top

defaultdict(list)
来源：http://scu.sweek.top

[U15] Py：高精度计时
来源：http://ozu.hysaishi.cn

t = time.perf_counter()
来源：http://yof.zdbjq.cn

[U16] Py：命令行参数解析
来源：http://cda.wangdashe.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://vrr.gogol.net.cn

[U17] Py：初始化日志
来源：http://nri.nanxinkj.top

logging.basicConfig(level=logging.INFO)
来源：http://vbz.xziqi.cn

[U18] Py：预编译正则
来源：http://amr.ehwqpu.com

pat = re.compile(r"\d+")
来源：http://lxd.sufxvd.cn

[U19] Py：正则替换带回调
来源：http://xuf.yuanzhike.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://kpf.ywan-chungtsiang.top

[U20] Py：缓存函数结果
来源：http://kjw.hongshengwenyu.top

@functools.lru_cache(maxsize=None)
来源：http://lbj.guannengcc.top

[U21] Py：自定义上下文管理器
来源：http://ato.pengpengdd.cyou

@contextlib.contextmanager
来源：http://bla.ybcxt.top

[U22] Py：矩阵转置
来源：http://tjo.jlsjyb.cn

list(zip(*m))
来源：http://zkv.sysykeji.top

[U23] Py：分块读取大文件
来源：http://xmb.yj20258.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://bmj.ivvv.top

[U24] Py：路径操作
来源：http://zbc.ctjpmb.com

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://bbe.ppjwa.cn

[U25] Py：CSV 按字典读
来源：http://rgf.ctjpmb.com

csv.DictReader(f)
来源：http://xbv.zdbjq.cn

[U26] Py：并发下载
来源：http://qdi.tanke756.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://rqf.jiagoushi.top

[U27] Py：异步 HTTP
来源：http://enp.ydjk.org.cn

aiohttp.ClientSession() 配合 async with
来源：http://muj.snrcjt.cn

[U28] Py：类型别名
来源：http://xdz.ctjpmb.com

UserId = int
来源：http://nud.hongshengwenyu.top

[U29] Py：属性校验
来源：http://cku.smart0.xyz

@property 与 @x.setter 配合
来源：http://csl.yangfankeji.com

[U30] Py：数据类
来源：http://dik.hnqzz.top

@dataclass(slots=True)
来源：http://ybr.haohaochexian.top

[U31] Py：单测
来源：http://xmo.yj202588.top

python -m pytest -q
来源：http://dov.zycfv.cn

[U32] Py：代码格式化
来源：http://lpn.tian-w.cn

ruff format . && ruff check --fix .
来源：http://pya.jqgufenzy.top

[U33] Py：打包发布
来源：http://kae.tarul.cn

python -m build  （依赖 pyproject.toml）
来源：http://gqj.yuanzhike.top

[U34] Py：判断编码
来源：http://hqz.jqgufenzy.top

chardet.detect(raw)
来源：http://eqj.yanxiufei.cn

[U35] Py：发送邮件
来源：http://ndo.yj202588.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://eij.nanxinkj.top

[U36] Py：定时任务
来源：http://ekk.jlsjyb.cn

schedule.every(10).minutes.do(job)
来源：http://yft.zhaomingkeji.xyz

[U37] Py：读写 Excel
来源：http://yuw.wangshuangyany.cn

pandas.read_excel / DataFrame.to_excel
来源：http://rfl.xinyue.icu

[U38] Py：获取脚本所在目录
来源：http://ezx.fktsv.cn

Path(__file__).resolve().parent
来源：http://qgw.yj20258.top

[U39] Py：判断是否在交互环境
来源：http://giu.cqqwz.cn

sys.stdout.isatty()
来源：http://mac.pengpengdd.cyou

[U40] Py：打印到标准错误
来源：http://xdi.bbcook.cn

print("err", file=sys.stderr)
来源：http://cuc.jiagoushi.top

[U41] PHP：初始化 Composer 项目
来源：http://pgy.cdnleiting.top

composer init;  composer require guzzlehttp/guzzle
来源：http://xaz.zhengqikj.top

[U42] PHP：PSR-4 自动加载
来源：http://hav.dianchejie.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://cup.yonumen.top

[U43] PHP：声明命名空间
来源：http://arv.ehwqpu.com

namespace App\Http;
来源：http://waq.sjlbkw.cn

[U44] PHP：开启严格类型
来源：http://mvw.yj20258888.top

declare(strict_types=1);
来源：http://hrs.nanxuanxn.top

[U45] PHP：类型声明与返回类型
来源：http://gam.gogol.net.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://qtt.guannengcc.top

[U46] PHP：可空类型
来源：http://glo.hammf.cn

?string $name = null
来源：http://kjz.dashuyun.cn

[U47] PHP：联合类型
来源：http://mfx.hongshengwenyu.top

int|string $id
来源：http://mdf.hammf.cn

[U48] PHP：纯枚举
来源：http://aer.cheryme.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://onb.c1oappe.top

[U49] PHP：只读属性
来源：http://ahl.0kj1m.cn

public readonly string $name
来源：http://wpv.yvedp.cn

[U50] PHP：构造器属性提升
来源：http://fou.fengsongda.top

public function __construct(private int $id) {}
来源：http://oaj.birdmap.top

[U51] PHP：数组解构
来源：http://sji.tarul.cn

[$a, $b] = $arr;
来源：http://web.xylfe.cn

[U52] PHP：箭头函数
来源：http://uzb.sufxvd.cn

$double = fn($x) => $x * 2;
来源：http://cst.jianghu66.top

[U53] PHP：空合并运算符
来源：http://cht.ivvv.top

$v = $a ?? $b ?? "default";
来源：http://sqv.jinqigufen.top

[U54] PHP：空安全调用
来源：http://oko.sjlbkw.cn

$obj?->method()
来源：http://gtu.zycfv.cn

[U55] PHP：match 表达式
来源：http://tvd.daxiang520.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://tmt.shzxlz.cn

[U56] PHP：命名参数
来源：http://tlw.zhengqikj.top

f(a: 1, b: 2)
来源：http://kiq.tian-w.cn

[U57] PHP：字符串插值
来源：http://wde.ctjpmb.com

"值: {$a}"
来源：http://imm.xingfuxueyuan.xyz

[U58] PHP：数组三件套
来源：http://asz.hnqzz.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://zhn.shanyushiyangtech.top

[U59] PHP：自定义排序
来源：http://nsa.daxiang520.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://yyw.cucudq.cn

[U60] PHP：JSON 编解码
来源：http://slc.hysaishi.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://tgc.ppjwa.cn

[U61] PHP：正则
来源：http://une.epnwcf.com

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://psb.sysykeji.top

[U62] PHP：日期对象
来源：http://dyj.aizwys.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://iav.ydjk.org.cn

[U63] PHP：文件读写
来源：http://yvw.yj20258888.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://fho.snrcjt.cn

[U64] PHP：目录遍历
来源：http://ehi.smart0.xyz

glob("dir/*.php");  scandir("dir");
来源：http://jsc.hnqzz.top

[U65] PHP：会话
来源：http://dpo.hcnkem.com

session_start();  $_SESSION["uid"] = 1;
来源：http://pre.hongshengwenyu.top

[U66] PHP：设置 Cookie
来源：http://gvc.0kj1m.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://iyq.pycfn.com

[U67] PHP：处理文件上传
来源：http://mab.yongpay.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://phc.ctjpmb.com

[U68] PHP：PDO 连接
来源：http://sqb.aizwys.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://poe.nanxuanxn.top

[U69] PHP：PDO 预处理
来源：http://vcf.hysaishi.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://ofe.epnwcf.com

[U70] PHP：PDO 事务
来源：http://ptr.shangyingyoupin.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://vyp.gogol.net.cn

[U71] PHP：抛出异常
来源：http://gan.uphjek.com

throw new RuntimeException("失败", 500);
来源：http://cyk.yongpay.top

[U72] PHP：写错误日志
来源：http://xhd.fanxiaobao.xyz

error_log("失败: " . $e->getMessage());
来源：http://qtx.jianghu66.top

[U73] PHP：读取 ini 配置
来源：http://upp.sjlbkw.cn

parse_ini_file("config.ini", true)
来源：http://wci.yonumen.top

[U74] PHP：读取环境变量
来源：http://hib.jyoumei.cn

getenv("APP_ENV") ?: "production"
来源：http://tng.ybcxt.top

[U75] PHP：依赖注入
来源：http://mul.hesvh.cn

composer require psr/container
来源：http://cux.meibo888.top

[U76] PHP：简单路由
来源：http://ddn.bjfxy.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://scp.zhiwuduotai.top

[U77] PHP：模板渲染
来源：http://yal.iojbl.cn

composer require twig/twig
来源：http://mey.shzxlz.cn

[U78] PHP：单元测试
来源：http://qor.jianghu66.top

composer require --dev phpunit/phpunit
来源：http://ugc.redwolf501.top

[U79] PHP：静态分析
来源：http://ipy.quarkkingdee.top

composer require --dev phpstan/phpstan
来源：http://gta.yuanzhike.top

[U80] PHP：代码规范修复
来源：http://qqj.iojbl.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://yhz.316326.xyz

[U81] JS：初始化项目
来源：http://ikr.zdbjq.cn

npm init -y;  npm i express
来源：http://dpc.jqgfzy.top

[U82] JS：package.json 脚本
来源：http://acc.sjlbkw.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://hsc.hammf.cn

[U83] JS：ES Module 导入导出
来源：http://kgl.c1oappe.top

export const a = 1;  import { a } from "./m.js";
来源：http://gsf.zhijiandao.cn

[U84] JS：CommonJS 写法
来源：http://ert.yj202588.top

module.exports = { a };  const { a } = require("./m");
来源：http://tdc.vqdsnc.cn

[U85] JS：可选链
来源：http://dzu.kuanghao11.cn

a?.b?.c
来源：http://pwh.daxiang520.top

[U86] JS：空值合并
来源：http://fxh.zdqjudy.top

a ?? b
来源：http://gmo.yanxiufei.cn

[U87] JS：解构默认值
来源：http://upu.yuxming.cn

const { a = 1, b = 2 } = obj;
来源：http://nld.daxiang520.top

[U88] JS：对象展开合并
来源：http://cjr.hnqzz.top

{ ...a, ...b }
来源：http://wze.nanxuanxn.top

[U89] JS：数组去重
来源：http://fxg.xuanzx.com

[...new Set(arr)]
来源：http://vkf.nanxuanxn.top

[U90] JS：数字数组排序
来源：http://kxi.iojbl.cn

[...arr].sort((a, b) => a - b)
来源：http://auk.ctjpmb.com

[U91] JS：对象键值遍历
来源：http://kqa.sjlbkw.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hkv.sweek.top

[U92] JS：深拷贝
来源：http://wsn.cashguo.top

structuredClone(obj)
来源：http://ozy.shanyushiyangkeji.top

[U93] JS：模板字符串
来源：http://wdj.ivvv.top

`共 ${n} 条`
来源：http://mkm.chenlongwang.top

[U94] JS：箭头函数
来源：http://kfm.fktsv.cn

const double = x => x * 2;
来源：http://vyt.9152youxi.cn

[U95] JS：Promise 包装
来源：http://akp.zdqjudy.top

new Promise((resolve, reject) => {})
来源：http://vcw.zhiwuduotai.top

[U96] JS：async/await 与异常
来源：http://kqj.ehwqpu.com

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://zop.iojbl.cn

[U97] JS：并发请求
来源：http://dbr.zhijiandao.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://kug.9152youxi.cn

[U98] JS：fetch 带 JSON
来源：http://bso.hywenlv.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://ftc.xuetiantiany.cn

[U99] JS：事件监听
来源：http://top.redwolf501.top

el.addEventListener("click", e => {})
来源：http://set.zhijiandao.cn

[U100] JS：DOM 查询
来源：http://hes.sweek.top

document.querySelector(".item")
来源：http://miu.birdmap.top

[U101] JS：classList 操作
来源：http://gpw.shanyushiyangtech.top

el.classList.toggle("active")
来源：http://lua.cucudq.cn

[U102] JS：本地存储
来源：http://tmn.tarul.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://koh.jinyuanbaomall.cn

[U103] JS：定时器
来源：http://wec.yvedp.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://qrz.ywan-chungtsiang.top

[U104] JS：防抖
来源：http://kdi.shanyushiyangkeji.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ilk.yuanzhike.top

[U105] JS：节流
来源：http://viq.hongshengwenyu.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://acw.zhixingplan.top

[U106] JS：日期格式化
来源：http://nyq.jqgufenzy.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://cbo.chenzaomai.com

[U107] JS：数字千分位
来源：http://wbx.tanke756.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://djf.cheryme.top

[U108] JS：随机整数
来源：http://myu.mhx1999.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://kvy.jyoumei.cn

[U109] JS：数组分组
来源：http://nug.tianlin.xyz

Object.groupBy(arr, x => x.type)
来源：http://xje.shanyushiyangkeji.top

[U110] JS：数组分块
来源：http://eay.shanyushiyangtech.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://fta.guowangkeji.top

[U111] JS：对象转 Map
来源：http://ker.cucudq.cn

new Map(Object.entries(obj))
来源：http://dtr.0kj1m.cn

[U112] JS：字符串补位
来源：http://efy.cucudq.cn

"7".padStart(3, "0")
来源：http://naz.meibo888.top

[U113] JS：正则替换全部
来源：http://iol.yfazqb.com

s.replaceAll("a", "b")
来源：http://ptt.fzhhl.top

[U114] JS：JSON 深比较
来源：http://ojy.yfazqb.com

JSON.stringify(a) === JSON.stringify(b)
来源：http://zue.tanke756.top

[U115] JS：生成 UUID
来源：http://xik.daria6918.cn

crypto.randomUUID()
来源：http://sfs.ctjpmb.com

[U116] JS：类型检查（JSDoc）
来源：http://kaw.dianchejie.cn

/** @param {string} name */ function f(name) {}
来源：http://oqb.yueranfly.top

[U117] JS：单元测试
来源：http://hur.zhaomingkeji.xyz

npm i -D vitest;  npx vitest
来源：http://brf.wangshuangyany.cn

[U118] JS：开发服务器
来源：http://fqt.zdbjq.cn

npm i -D vite;  npx vite
来源：http://rvr.sweek.top

[U119] JS：生产构建
来源：http://vdg.svipenyu.cn

npx vite build
来源：http://ouq.chenlongwang.top

[U120] JS：读取环境变量（Vite）
来源：http://gji.zhaomingkeji.xyz

import.meta.env.VITE_API_URL
来源：http://bvr.ywan-chungtsiang.top

================================================================================
来源：http://bql.shanyushiyangkeji.top

统计汇总
来源：http://mce.feifeiyinyue.top

================================================================================
来源：http://ppr.cashguo.top

按语言统计（条）：
来源：http://cgy.jqgfzy.top

Python ......... 252
来源：http://zcx.xingfuxueyuan.xyz

PHP ............ 252
来源：http://xuq.zhongyouzk.top

JavaScript ..... 252
来源：http://aoo.xingfuxueyuan.xyz

TypeScript ..... 212
来源：http://yuj.chenlongwang.top

Java ........... 212
来源：http://bnk.shanyushiyangkeji.top

Go ............. 212
来源：http://apw.yueranfly.top

Ruby ........... 212
来源：http://eoq.jianghu66.top

C# ............. 212
来源：http://dps.xylfe.cn

C .............. 30
来源：http://myv.hywenlv.cn

C++ ............ 30
来源：http://ktx.hcnkem.com

SQL ............ 90
来源：http://oec.ctjpmb.com

Bash ........... 80
来源：http://uof.yj20258888.top

Kotlin ......... 15
来源：http://oxh.nanxinkj.top

Swift .......... 15
来源：http://uns.nanxinkj.top

Lua ............ 10
来源：http://cgl.yj20258.top

Perl ........... 10
来源：http://hty.andypj.xyz

Scala .......... 10
来源：http://obv.gzhubu.top

------------------------------------
来源：http://hmc.zhoulong.xyz

合计 ........... 2106 条
来源：http://pct.meibo888.top

按章节统计：
来源：http://ovy.fehbvm.com

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://moj.ydzc1.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://xox.tian-w.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://mrk.shuidangran.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://wie.jyoumei.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hjc.hammf.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://vsm.fktsv.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hdg.xinyue.icu

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://ecv.yueranfly.top


<!-- 参考信息 -->