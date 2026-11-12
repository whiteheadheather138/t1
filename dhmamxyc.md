代发 wailian999

[T49] Perl：函数
来源：http://zan.tianlin.xyz

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://tir.guannengcc.top

[T50] Perl：逐行读文件
来源：http://ltt.zhengqikj.top

open my $fh, "<", "a.txt" or die $!;
来源：http://iab.ywan-chungtsiang.top

while (my $line = <$fh>) { print $line; }
来源：http://sye.jinyuanbaomall.cn

[T51] Scala：Hello World
来源：http://qlv.ywan-chungtsiang.top

println("Hello")
来源：http://xst.hongshengwenyu.top

[T52] Scala：变量
来源：http://hfj.zycfv.cn

val a = 1;  var b = 2
来源：http://eti.fehbvm.com

[T53] Scala：字符串插值
来源：http://kts.gotoacloud.top

s"值: $b"
来源：http://arm.ywan-chungtsiang.top

[T54] Scala：集合映射
来源：http://ovk.sjlbkw.cn

List(1, 2, 3).map(_ * 2)
来源：http://dmw.shangyingyoupin.top

[T55] Scala：集合过滤
来源：http://mgx.jiagoushi.top

List(1, 2, 3).filter(_ > 1)
来源：http://hyo.hnxiangtu.top

[T56] Scala：样例类
来源：http://mwj.epnwcf.com

case class User(name: String, age: Int)
来源：http://jru.xinyue.icu

[T57] Scala：模式匹配
来源：http://ccc.xylfe.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://jmb.fzhhl.top

[T58] Scala：函数定义
来源：http://fhy.jinyuanbaomall.cn

def add(a: Int, b: Int): Int = a + b
来源：http://mgu.epnwcf.com

[T59] Scala：循环
来源：http://iyh.hcnkem.com

for (i <- 1 to 10) println(i)
来源：http://suk.dashuyun.cn

[T60] Scala：折叠
来源：http://bjv.yuanzhike.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://ahm.jinyuanbaomall.cn

================================================================================
来源：http://gil.0kj1m.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://mac.yonumen.top

================================================================================
来源：http://lzw.yvedp.cn

[U01] Py：创建虚拟环境
来源：http://eac.jyoumei.cn

python -m venv .venv && source .venv/bin/activate
来源：http://ggg.52xcode.cn

[U02] Py：导出 / 安装依赖
来源：http://cdn.tian-w.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://fpe.nwbrower.top

[U03] Py：加载 .env 配置
来源：http://zcf.zhongyouzk.top

from dotenv import load_dotenv; load_dotenv()
来源：http://mfp.cucudq.cn

[U04] Py：变量调试打印
来源：http://vxj.guannengcc.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://fkr.sweek.top

[U05] Py：列表去重且保序
来源：http://rko.yvedp.cn

list(dict.fromkeys(arr))
来源：http://drq.hywenlv.cn

[U06] Py：合并两个字典
来源：http://pza.0kj1m.cn

{**a, **b}
来源：http://vrd.nanxuanxn.top

[U07] Py：反转字典键值
来源：http://ven.gzhubu.top

{v: k for k, v in d.items()}
来源：http://kve.sxryk.cn

[U08] Py：展平二维列表
来源：http://cgn.yj20258888.top

[y for x in nested for y in x]
来源：http://dxz.hnqzz.top

[U09] Py：字典取最大值的键
来源：http://dsk.fzhhl.top

max(d, key=d.get)
来源：http://omo.vehdjk.com

[U10] Py：按值排序字典
来源：http://bdq.zhoulong.xyz

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://rma.ivvv.top

[U11] Py：生成器表达式
来源：http://jmq.yangfankeji.com

(x * 2 for x in arr)
来源：http://esp.tanke756.top

[U12] Py：取出现最多的 3 个元素
来源：http://zzw.zdbjq.cn

Counter(arr).most_common(3)
来源：http://tsj.gzhubu.top

[U13] Py：固定长度队列
来源：http://mhw.aizwys.cn

deque(maxlen=10)
来源：http://dgd.guannengcc.top

[U14] Py：分组收集到列表
来源：http://rlz.yj20258888.top

defaultdict(list)
来源：http://npc.yanxiufei.cn

[U15] Py：高精度计时
来源：http://uqb.zhiwuduotai.top

t = time.perf_counter()
来源：http://zqf.zhoulong.xyz

[U16] Py：命令行参数解析
来源：http://osg.bbcook.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://jaj.epnwcf.com

[U17] Py：初始化日志
来源：http://uoc.yj20258.top

logging.basicConfig(level=logging.INFO)
来源：http://gcf.aizwys.cn

[U18] Py：预编译正则
来源：http://wio.yueranfly.top

pat = re.compile(r"\d+")
来源：http://tbz.cashguo.top

[U19] Py：正则替换带回调
来源：http://erk.sxryk.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://mah.chenzaomai.com

[U20] Py：缓存函数结果
来源：http://pbm.uphjek.com

@functools.lru_cache(maxsize=None)
来源：http://dbm.chenlongwang.top

[U21] Py：自定义上下文管理器
来源：http://ixf.hnqzz.top

@contextlib.contextmanager
来源：http://hff.yj20258888.top

[U22] Py：矩阵转置
来源：http://ayk.yuxming.cn

list(zip(*m))
来源：http://lmd.316326.xyz

[U23] Py：分块读取大文件
来源：http://njk.sysykeji.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://mjy.dianchejie.cn

[U24] Py：路径操作
来源：http://kix.ehwqpu.com

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://dnp.haohaochexian.top

[U25] Py：CSV 按字典读
来源：http://khd.ydzc1.top

csv.DictReader(f)
来源：http://kzb.hywenlv.cn

[U26] Py：并发下载
来源：http://wlw.jqgufenzy.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://rnl.fzhhl.top

[U27] Py：异步 HTTP
来源：http://pko.yanxiufei.cn

aiohttp.ClientSession() 配合 async with
来源：http://esq.svipenyu.cn

[U28] Py：类型别名
来源：http://uwf.quarkkingdee.top

UserId = int
来源：http://dcq.guannengcc.top

[U29] Py：属性校验
来源：http://ocy.yfazqb.com

@property 与 @x.setter 配合
来源：http://lsr.yj20258888.top

[U30] Py：数据类
来源：http://xwp.hammf.cn

@dataclass(slots=True)
来源：http://xea.yongpay.top

[U31] Py：单测
来源：http://ffq.yueranfly.top

python -m pytest -q
来源：http://qrc.jqgufenzy.top

[U32] Py：代码格式化
来源：http://hin.kuanghao11.cn

ruff format . && ruff check --fix .
来源：http://wlf.cucudq.cn

[U33] Py：打包发布
来源：http://tdk.shanyushiyangkeji.top

python -m build  （依赖 pyproject.toml）
来源：http://pwl.hfpthk.cn

[U34] Py：判断编码
来源：http://egs.jianghu66.top

chardet.detect(raw)
来源：http://hmi.shanyushiyangkeji.top

[U35] Py：发送邮件
来源：http://vkt.hesvh.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://ram.daria6918.cn

[U36] Py：定时任务
来源：http://dna.dashuyun.cn

schedule.every(10).minutes.do(job)
来源：http://auv.aibaodan.cn

[U37] Py：读写 Excel
来源：http://vff.jinqigfzy.top

pandas.read_excel / DataFrame.to_excel
来源：http://zjd.uphjek.com

[U38] Py：获取脚本所在目录
来源：http://dlt.jqgfzy.top

Path(__file__).resolve().parent
来源：http://drx.daxiang520.top

[U39] Py：判断是否在交互环境
来源：http://mjp.jqgfzy.top

sys.stdout.isatty()
来源：http://aeu.ybcxt.top

[U40] Py：打印到标准错误
来源：http://yte.0kj1m.cn

print("err", file=sys.stderr)
来源：http://xem.zhixingplan.top

[U41] PHP：初始化 Composer 项目
来源：http://dpi.iojbl.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://zgi.cqqwz.cn

[U42] PHP：PSR-4 自动加载
来源：http://kfm.gzhubu.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://qyd.zycfv.cn

[U43] PHP：声明命名空间
来源：http://lhj.yj20258.top

namespace App\Http;
来源：http://mww.hywenlv.cn

[U44] PHP：开启严格类型
来源：http://tgz.316326.xyz

declare(strict_types=1);
来源：http://asn.uphjek.com

[U45] PHP：类型声明与返回类型
来源：http://lql.zhijiandao.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://lxw.hesvh.cn

[U46] PHP：可空类型
来源：http://uvx.cashguo.top

?string $name = null
来源：http://sro.jiagoushi.top

[U47] PHP：联合类型
来源：http://aek.hongshengwenyu.top

int|string $id
来源：http://ijf.bjfxy.top

[U48] PHP：纯枚举
来源：http://bme.yuanzhike.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://mne.gotoacloud.top

[U49] PHP：只读属性
来源：http://zqu.jinghuilouyu.cn

public readonly string $name
来源：http://rsx.pycfn.com

[U50] PHP：构造器属性提升
来源：http://dwn.yj202588.top

public function __construct(private int $id) {}
来源：http://ikl.cqqwz.cn

[U51] PHP：数组解构
来源：http://xnn.snrcjt.cn

[$a, $b] = $arr;
来源：http://gnn.gzhubu.top

[U52] PHP：箭头函数
来源：http://tgl.yj20258.top

$double = fn($x) => $x * 2;
来源：http://efd.cdnleiting.top

[U53] PHP：空合并运算符
来源：http://cew.jqgfzy.top

$v = $a ?? $b ?? "default";
来源：http://zlx.hongshengwenyu.top

[U54] PHP：空安全调用
来源：http://cql.hywenlv.cn

$obj?->method()
来源：http://igb.gaohongyu789.top

[U55] PHP：match 表达式
来源：http://yfd.jinqigfzy.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://wli.feifeiyinyue.top

[U56] PHP：命名参数
来源：http://zsa.ctjpmb.com

f(a: 1, b: 2)
来源：http://vue.zhiwuduotai.top

[U57] PHP：字符串插值
来源：http://fru.zhengqikj.top

"值: {$a}"
来源：http://lua.cashguo.top

[U58] PHP：数组三件套
来源：http://vza.uphjek.com

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://fzh.cdnleiting.top

[U59] PHP：自定义排序
来源：http://kod.jinyuanbaomall.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hkg.ydjk.org.cn

[U60] PHP：JSON 编解码
来源：http://nvw.jianghu66.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hgn.xziqi.cn

[U61] PHP：正则
来源：http://rsu.fengsongda.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://cqd.jiagoushi.top

[U62] PHP：日期对象
来源：http://rkw.316326.xyz

(new DateTimeImmutable())->format("Y-m-d");
来源：http://bam.aizwys.cn

[U63] PHP：文件读写
来源：http://lck.nanxuanxn.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://zgm.dashuyun.cn

[U64] PHP：目录遍历
来源：http://bqd.fzhhl.top

glob("dir/*.php");  scandir("dir");
来源：http://pir.yangfankeji.com

[U65] PHP：会话
来源：http://rnd.c1oappe.top

session_start();  $_SESSION["uid"] = 1;
来源：http://kpj.zhengqikj.top

[U66] PHP：设置 Cookie
来源：http://tzt.hywenlv.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://vtr.gzhubu.top

[U67] PHP：处理文件上传
来源：http://oim.jinyuanbaomall.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://xxf.dashuyun.cn

[U68] PHP：PDO 连接
来源：http://ekh.zdqjudy.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://olj.cashguo.top

[U69] PHP：PDO 预处理
来源：http://rkc.sufxvd.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://wta.jinghuilouyu.cn

[U70] PHP：PDO 事务
来源：http://yzi.hysaishi.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://glt.cashguo.top

[U71] PHP：抛出异常
来源：http://gda.meibo888.top

throw new RuntimeException("失败", 500);
来源：http://fvu.hysaishi.cn

[U72] PHP：写错误日志
来源：http://zpt.chenzaomai.com

error_log("失败: " . $e->getMessage());
来源：http://kty.nanxinkj.top

[U73] PHP：读取 ini 配置
来源：http://cwn.aizwys.cn

parse_ini_file("config.ini", true)
来源：http://ueo.yj20258.top

[U74] PHP：读取环境变量
来源：http://otq.c1oappe.top

getenv("APP_ENV") ?: "production"
来源：http://xei.nwbrower.top

[U75] PHP：依赖注入
来源：http://ytl.dianchejie.cn

composer require psr/container
来源：http://iak.dianchejie.cn

[U76] PHP：简单路由
来源：http://msh.9152youxi.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://ezh.aibaodan.cn

[U77] PHP：模板渲染
来源：http://vps.iojbl.cn

composer require twig/twig
来源：http://dxn.jinqigufen.top

[U78] PHP：单元测试
来源：http://oop.sweek.top

composer require --dev phpunit/phpunit
来源：http://hxn.dashuyun.cn

[U79] PHP：静态分析
来源：http://ttz.sjlbkw.cn

composer require --dev phpstan/phpstan
来源：http://elt.ywan-chungtsiang.top

[U80] PHP：代码规范修复
来源：http://jum.jiagoushi.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://dcs.xuanzx.com

[U81] JS：初始化项目
来源：http://wtn.zhongyouzk.top

npm init -y;  npm i express
来源：http://qtd.pycfn.com

[U82] JS：package.json 脚本
来源：http://cep.shangyingyoupin.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://mmb.xinyue.icu

[U83] JS：ES Module 导入导出
来源：http://wff.dianchejie.cn

export const a = 1;  import { a } from "./m.js";
来源：http://mvx.jinyuanbaomall.cn

[U84] JS：CommonJS 写法
来源：http://gbi.fengsongda.top

module.exports = { a };  const { a } = require("./m");
来源：http://pay.dashuyun.cn

[U85] JS：可选链
来源：http://iss.ydjk.org.cn

a?.b?.c
来源：http://zof.yueranfly.top

[U86] JS：空值合并
来源：http://yim.jqgfzy.top

a ?? b
来源：http://sql.hywenlv.cn

[U87] JS：解构默认值
来源：http://qkk.zhongyouzk.top

const { a = 1, b = 2 } = obj;
来源：http://hmg.yj20258888.top

[U88] JS：对象展开合并
来源：http://wnz.haohaochexian.top

{ ...a, ...b }
来源：http://yzo.vqdsnc.cn

[U89] JS：数组去重
来源：http://xwp.chenzaomai.com

[...new Set(arr)]
来源：http://vyh.ywan-chungtsiang.top

[U90] JS：数字数组排序
来源：http://zcm.zdbjq.cn

[...arr].sort((a, b) => a - b)
来源：http://srv.dianchejie.cn

[U91] JS：对象键值遍历
来源：http://aem.xziqi.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://gan.snrcjt.cn

[U92] JS：深拷贝
来源：http://cxp.pycfn.com

structuredClone(obj)
来源：http://rcj.ybcxt.top

[U93] JS：模板字符串
来源：http://pfo.zdqjudy.top

`共 ${n} 条`
来源：http://sbr.redwolf501.top

[U94] JS：箭头函数
来源：http://kce.yj202588.top

const double = x => x * 2;
来源：http://tak.ctjpmb.com

[U95] JS：Promise 包装
来源：http://ipa.redwolf501.top

new Promise((resolve, reject) => {})
来源：http://smi.0kj1m.cn

[U96] JS：async/await 与异常
来源：http://ayf.jinyuanbaomall.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://bpa.shangyingyoupin.top

[U97] JS：并发请求
来源：http://vls.yvedp.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://mdz.yanxiufei.cn

[U98] JS：fetch 带 JSON
来源：http://jbi.xziqi.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://kyz.jianghu66.top

[U99] JS：事件监听
来源：http://ayu.aibaodan.cn

el.addEventListener("click", e => {})
来源：http://wds.iojbl.cn

[U100] JS：DOM 查询
来源：http://qwd.hcnkem.com

document.querySelector(".item")
来源：http://rtl.fengsongda.top

[U101] JS：classList 操作
来源：http://ofs.yongpay.top

el.classList.toggle("active")
来源：http://joz.hysaishi.cn

[U102] JS：本地存储
来源：http://tqi.shangyingyoupin.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://zhf.fzhhl.top

[U103] JS：定时器
来源：http://htp.dianchejie.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://onw.jinqigufen.top

[U104] JS：防抖
来源：http://aqc.shzxlz.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://poq.zhiwuduotai.top

[U105] JS：节流
来源：http://cxa.sxryk.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://nvn.redwolf501.top

[U106] JS：日期格式化
来源：http://elp.bjfxy.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://spc.xziqi.cn

[U107] JS：数字千分位
来源：http://xgy.yj20258888.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://nuc.mhx1999.top

[U108] JS：随机整数
来源：http://npf.fktsv.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://vsw.birdmap.top

[U109] JS：数组分组
来源：http://loh.ydjk.org.cn

Object.groupBy(arr, x => x.type)
来源：http://urp.316326.xyz

[U110] JS：数组分块
来源：http://xen.iojbl.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://std.jyoumei.cn

[U111] JS：对象转 Map
来源：http://otb.yuxming.cn

new Map(Object.entries(obj))
来源：http://rcm.daxiang520.top

[U112] JS：字符串补位
来源：http://byk.bbcook.cn

"7".padStart(3, "0")
来源：http://plq.chenzaomai.com

[U113] JS：正则替换全部
来源：http://bey.hywenlv.cn

s.replaceAll("a", "b")
来源：http://yws.pengpengdd.cyou

[U114] JS：JSON 深比较
来源：http://oml.zhoulong.xyz

JSON.stringify(a) === JSON.stringify(b)
来源：http://yji.sxryk.cn

[U115] JS：生成 UUID
来源：http://oii.xinyue.icu

crypto.randomUUID()
来源：http://njt.hnqzz.top

[U116] JS：类型检查（JSDoc）
来源：http://mwl.ydjk.org.cn

/** @param {string} name */ function f(name) {}
来源：http://zyd.jinqigfzy.top

[U117] JS：单元测试
来源：http://vho.uphjek.com

npm i -D vitest;  npx vitest
来源：http://lxb.gaohongyu789.top

[U118] JS：开发服务器
来源：http://drf.tian-w.cn

npm i -D vite;  npx vite
来源：http://nqf.jqgfzy.top

[U119] JS：生产构建
来源：http://zmz.cqqwz.cn

npx vite build
来源：http://sla.yj20258888.top

[U120] JS：读取环境变量（Vite）
来源：http://qht.feifeiyinyue.top

import.meta.env.VITE_API_URL
来源：http://oeq.yonumen.top

================================================================================
来源：http://mwf.mhx1999.top

统计汇总
来源：http://yae.jiagoushi.top

================================================================================
来源：http://xxi.yonumen.top

按语言统计（条）：
来源：http://gpf.hcnkem.com

Python ......... 252
来源：http://tfu.c1oappe.top

PHP ............ 252
来源：http://ukw.ppjwa.cn

JavaScript ..... 252
来源：http://ojm.hesvh.cn

TypeScript ..... 212
来源：http://lbz.zycfv.cn

Java ........... 212
来源：http://tcx.tanke756.top

Go ............. 212
来源：http://ckv.ydjk.org.cn

Ruby ........... 212
来源：http://frr.tianlin.xyz

C# ............. 212
来源：http://jht.cqqwz.cn

C .............. 30
来源：http://vod.fengsongda.top

C++ ............ 30
来源：http://mum.meibo888.top

SQL ............ 90
来源：http://xeo.meibo888.top

Bash ........... 80
来源：http://ich.zhengqikj.top

Kotlin ......... 15
来源：http://ufc.shangyingyoupin.top

Swift .......... 15
来源：http://cru.jyoumei.cn

Lua ............ 10
来源：http://sfr.xylfe.cn

Perl ........... 10
来源：http://wba.yj202588.top

Scala .......... 10
来源：http://vgk.jinghuilouyu.cn

------------------------------------
来源：http://xmm.ydzc1.top

合计 ........... 2106 条
来源：http://hyn.ybcxt.top

按章节统计：
来源：http://drl.zhongyouzk.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://ogt.vehdjk.com

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://pmz.zycfv.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://iyh.zycfv.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://ebv.iojbl.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://ogj.bjfxy.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://lma.guowangkeji.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://ano.yj20258888.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://cfo.andypj.xyz


<!-- 参考信息 -->