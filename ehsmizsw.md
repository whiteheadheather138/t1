代发 wailian999

[T45] Perl：数组遍历
来源：http://jqs.pengpengdd.cyou

for my $x (@arr) { print $x; }
来源：http://qcw.yj20258888.top

[T46] Perl：哈希操作
来源：http://wxf.nanxinkj.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://dgd.jyoumei.cn

[T47] Perl：正则捕获
来源：http://mcu.316326.xyz

if ($s =~ /(\d+)/) { print $1; }
来源：http://dld.wangdashe.top

[T48] Perl：正则替换
来源：http://gbm.yonumen.top

$s =~ s/old/new/g;
来源：http://eyl.yj20258.top

[T49] Perl：函数
来源：http://gib.hcnkem.com

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://vpg.jqgfzy.top

[T50] Perl：逐行读文件
来源：http://ici.svipenyu.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://lqk.jinqigfzy.top

while (my $line = <$fh>) { print $line; }
来源：http://jtq.zhongyouzk.top

[T51] Scala：Hello World
来源：http://ntw.pengpengdd.cyou

println("Hello")
来源：http://ukz.hysaishi.cn

[T52] Scala：变量
来源：http://vii.xuetiantiany.cn

val a = 1;  var b = 2
来源：http://eaj.ywan-chungtsiang.top

[T53] Scala：字符串插值
来源：http://crn.yonumen.top

s"值: $b"
来源：http://def.cheryme.top

[T54] Scala：集合映射
来源：http://vjg.shangyingyoupin.top

List(1, 2, 3).map(_ * 2)
来源：http://hbj.yj202588.top

[T55] Scala：集合过滤
来源：http://cll.sjlbkw.cn

List(1, 2, 3).filter(_ > 1)
来源：http://cyi.guannengcc.top

[T56] Scala：样例类
来源：http://wvx.birdmap.top

case class User(name: String, age: Int)
来源：http://pkp.zhaomingkeji.xyz

[T57] Scala：模式匹配
来源：http://vlq.yonumen.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://zbu.cashguo.top

[T58] Scala：函数定义
来源：http://mxo.jyoumei.cn

def add(a: Int, b: Int): Int = a + b
来源：http://ivf.hysaishi.cn

[T59] Scala：循环
来源：http://vyv.zycfv.cn

for (i <- 1 to 10) println(i)
来源：http://ufe.cdnleiting.top

[T60] Scala：折叠
来源：http://xlk.tarul.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hbi.andypj.xyz

================================================================================
来源：http://lci.svipenyu.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://ehd.chenjidiqi.icu

================================================================================
来源：http://whe.fktsv.cn

[U01] Py：创建虚拟环境
来源：http://max.pycfn.com

python -m venv .venv && source .venv/bin/activate
来源：http://rnc.jqgfzy.top

[U02] Py：导出 / 安装依赖
来源：http://tok.chenzaomai.com

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://iii.kuanghao11.cn

[U03] Py：加载 .env 配置
来源：http://fib.xuetiantiany.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://qpa.gotoacloud.top

[U04] Py：变量调试打印
来源：http://tlb.gogol.net.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://uss.nanxuanxn.top

[U05] Py：列表去重且保序
来源：http://olu.pycfn.com

list(dict.fromkeys(arr))
来源：http://kfo.hywenlv.cn

[U06] Py：合并两个字典
来源：http://yoy.jlsjyb.cn

{**a, **b}
来源：http://fuq.yonumen.top

[U07] Py：反转字典键值
来源：http://ikp.daxiang520.top

{v: k for k, v in d.items()}
来源：http://quz.zhixingplan.top

[U08] Py：展平二维列表
来源：http://iod.ehwqpu.com

[y for x in nested for y in x]
来源：http://dna.nwbrower.top

[U09] Py：字典取最大值的键
来源：http://bxg.quarkkingdee.top

max(d, key=d.get)
来源：http://bev.yonumen.top

[U10] Py：按值排序字典
来源：http://eys.chenzaomai.com

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://dtb.zhaomingkeji.xyz

[U11] Py：生成器表达式
来源：http://fju.bbcook.cn

(x * 2 for x in arr)
来源：http://jdb.shanyushiyangkeji.top

[U12] Py：取出现最多的 3 个元素
来源：http://hgb.jiagoushi.top

Counter(arr).most_common(3)
来源：http://rnb.jinyuanbaomall.cn

[U13] Py：固定长度队列
来源：http://ohi.c1oappe.top

deque(maxlen=10)
来源：http://rxv.yj20258888.top

[U14] Py：分组收集到列表
来源：http://lez.birdmap.top

defaultdict(list)
来源：http://qtr.uphjek.com

[U15] Py：高精度计时
来源：http://tgn.shuidangran.top

t = time.perf_counter()
来源：http://lnn.gaohongyu789.top

[U16] Py：命令行参数解析
来源：http://nnz.svipenyu.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://qxo.wangshuangyany.cn

[U17] Py：初始化日志
来源：http://nrg.yj202588.top

logging.basicConfig(level=logging.INFO)
来源：http://ruc.yangfankeji.com

[U18] Py：预编译正则
来源：http://mvz.0kj1m.cn

pat = re.compile(r"\d+")
来源：http://hox.kuanghao11.cn

[U19] Py：正则替换带回调
来源：http://gja.svipenyu.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://brs.hfpthk.cn

[U20] Py：缓存函数结果
来源：http://adk.daria6918.cn

@functools.lru_cache(maxsize=None)
来源：http://rwt.dianchejie.cn

[U21] Py：自定义上下文管理器
来源：http://elk.wangdashe.top

@contextlib.contextmanager
来源：http://qrj.shuidangran.top

[U22] Py：矩阵转置
来源：http://nhu.hongshengwenyu.top

list(zip(*m))
来源：http://iye.jyoumei.cn

[U23] Py：分块读取大文件
来源：http://wko.fanxiaobao.xyz

for chunk in iter(lambda: f.read(8192), b""):
来源：http://ttc.jqgufenzy.top

[U24] Py：路径操作
来源：http://drw.316326.xyz

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://che.xziqi.cn

[U25] Py：CSV 按字典读
来源：http://txu.hongshengwenyu.top

csv.DictReader(f)
来源：http://jym.zhongyouzk.top

[U26] Py：并发下载
来源：http://eko.gaohongyu789.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://jmn.xuetiantiany.cn

[U27] Py：异步 HTTP
来源：http://clh.tarul.cn

aiohttp.ClientSession() 配合 async with
来源：http://rrd.xuetiantiany.cn

[U28] Py：类型别名
来源：http://bry.xinyue.icu

UserId = int
来源：http://dxi.cucudq.cn

[U29] Py：属性校验
来源：http://yex.fehbvm.com

@property 与 @x.setter 配合
来源：http://lkg.c1oappe.top

[U30] Py：数据类
来源：http://wqk.yangfankeji.com

@dataclass(slots=True)
来源：http://fpk.dianchejie.cn

[U31] Py：单测
来源：http://ztt.fktsv.cn

python -m pytest -q
来源：http://ayu.yvedp.cn

[U32] Py：代码格式化
来源：http://rsj.cheryme.top

ruff format . && ruff check --fix .
来源：http://tui.pengpengdd.cyou

[U33] Py：打包发布
来源：http://lmr.sweek.top

python -m build  （依赖 pyproject.toml）
来源：http://ndj.quarkkingdee.top

[U34] Py：判断编码
来源：http://fnx.shanyushiyangkeji.top

chardet.detect(raw)
来源：http://amq.xinyue.icu

[U35] Py：发送邮件
来源：http://xku.sysykeji.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://rpf.fehbvm.com

[U36] Py：定时任务
来源：http://jsd.ivvv.top

schedule.every(10).minutes.do(job)
来源：http://yei.pycfn.com

[U37] Py：读写 Excel
来源：http://rwp.sweek.top

pandas.read_excel / DataFrame.to_excel
来源：http://tdr.zhaomingkeji.xyz

[U38] Py：获取脚本所在目录
来源：http://dax.sxryk.cn

Path(__file__).resolve().parent
来源：http://tvj.guannengcc.top

[U39] Py：判断是否在交互环境
来源：http://lhi.nwbrower.top

sys.stdout.isatty()
来源：http://tji.jinqigufen.top

[U40] Py：打印到标准错误
来源：http://xre.yvedp.cn

print("err", file=sys.stderr)
来源：http://nyb.shangyingyoupin.top

[U41] PHP：初始化 Composer 项目
来源：http://tpt.nanxinkj.top

composer init;  composer require guzzlehttp/guzzle
来源：http://mte.ivvv.top

[U42] PHP：PSR-4 自动加载
来源：http://rmf.hywenlv.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://gdi.xuanzx.com

[U43] PHP：声明命名空间
来源：http://lnj.0kj1m.cn

namespace App\Http;
来源：http://tyu.snrcjt.cn

[U44] PHP：开启严格类型
来源：http://eud.yangfankeji.com

declare(strict_types=1);
来源：http://qkw.ehwqpu.com

[U45] PHP：类型声明与返回类型
来源：http://sjb.yj20258.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://axf.aibaodan.cn

[U46] PHP：可空类型
来源：http://lkd.hnxiangtu.top

?string $name = null
来源：http://noy.wangshuangyany.cn

[U47] PHP：联合类型
来源：http://gym.yongpay.top

int|string $id
来源：http://tqr.zhijiandao.cn

[U48] PHP：纯枚举
来源：http://ifc.chenjidiqi.icu

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://ebh.gaohongyu789.top

[U49] PHP：只读属性
来源：http://rzt.xylfe.cn

public readonly string $name
来源：http://ero.zhijiandao.cn

[U50] PHP：构造器属性提升
来源：http://swl.ydjk.org.cn

public function __construct(private int $id) {}
来源：http://tma.haohaochexian.top

[U51] PHP：数组解构
来源：http://adw.0kj1m.cn

[$a, $b] = $arr;
来源：http://wuy.yj202588.top

[U52] PHP：箭头函数
来源：http://usr.yj20258888.top

$double = fn($x) => $x * 2;
来源：http://vtb.shanyushiyangkeji.top

[U53] PHP：空合并运算符
来源：http://bdn.zdqjudy.top

$v = $a ?? $b ?? "default";
来源：http://enm.cucudq.cn

[U54] PHP：空安全调用
来源：http://zfz.zhaomingkeji.xyz

$obj?->method()
来源：http://ecw.jlsjyb.cn

[U55] PHP：match 表达式
来源：http://inj.yanxiufei.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://iak.chenlongwang.top

[U56] PHP：命名参数
来源：http://acl.snrcjt.cn

f(a: 1, b: 2)
来源：http://tph.yuxming.cn

[U57] PHP：字符串插值
来源：http://grr.ppjwa.cn

"值: {$a}"
来源：http://efz.svipenyu.cn

[U58] PHP：数组三件套
来源：http://sii.gaohongyu789.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://ora.xingfuxueyuan.xyz

[U59] PHP：自定义排序
来源：http://ywy.9152youxi.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://zxs.fengsongda.top

[U60] PHP：JSON 编解码
来源：http://lef.hcnkem.com

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://lpp.bbcook.cn

[U61] PHP：正则
来源：http://rtj.daxiang520.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://kpk.gotoacloud.top

[U62] PHP：日期对象
来源：http://zah.zhaomingkeji.xyz

(new DateTimeImmutable())->format("Y-m-d");
来源：http://lig.yuxming.cn

[U63] PHP：文件读写
来源：http://jpf.redwolf501.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://ozp.chenlongwang.top

[U64] PHP：目录遍历
来源：http://xwy.shzxlz.cn

glob("dir/*.php");  scandir("dir");
来源：http://bde.tianlin.xyz

[U65] PHP：会话
来源：http://snp.nanxuanxn.top

session_start();  $_SESSION["uid"] = 1;
来源：http://lmk.gogol.net.cn

[U66] PHP：设置 Cookie
来源：http://xis.tian-w.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://bfb.xuanzx.com

[U67] PHP：处理文件上传
来源：http://cdd.hesvh.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://uiz.daxiang520.top

[U68] PHP：PDO 连接
来源：http://eyz.jyoumei.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://bcd.shangyingyoupin.top

[U69] PHP：PDO 预处理
来源：http://ilq.yuanzhike.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://pth.shanyushiyangkeji.top

[U70] PHP：PDO 事务
来源：http://hrl.nanxinkj.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://ora.sweek.top

[U71] PHP：抛出异常
来源：http://hzd.sysykeji.top

throw new RuntimeException("失败", 500);
来源：http://ner.yj20258.top

[U72] PHP：写错误日志
来源：http://ith.jinghuilouyu.cn

error_log("失败: " . $e->getMessage());
来源：http://nou.shanyushiyangkeji.top

[U73] PHP：读取 ini 配置
来源：http://lim.vqdsnc.cn

parse_ini_file("config.ini", true)
来源：http://igx.jinqigufen.top

[U74] PHP：读取环境变量
来源：http://aml.aibaodan.cn

getenv("APP_ENV") ?: "production"
来源：http://att.shanyushiyangkeji.top

[U75] PHP：依赖注入
来源：http://qcs.jiagoushi.top

composer require psr/container
来源：http://ckj.pycfn.com

[U76] PHP：简单路由
来源：http://mfu.yueranfly.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://qlj.vqdsnc.cn

[U77] PHP：模板渲染
来源：http://fex.guowangkeji.top

composer require twig/twig
来源：http://xpm.jinqigufen.top

[U78] PHP：单元测试
来源：http://tqr.hesvh.cn

composer require --dev phpunit/phpunit
来源：http://fmk.ctjpmb.com

[U79] PHP：静态分析
来源：http://bcg.sjlbkw.cn

composer require --dev phpstan/phpstan
来源：http://rzv.bjfxy.top

[U80] PHP：代码规范修复
来源：http://zyb.zhixingplan.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://nhq.xuanzx.com

[U81] JS：初始化项目
来源：http://ury.andypj.xyz

npm init -y;  npm i express
来源：http://yia.jinqigfzy.top

[U82] JS：package.json 脚本
来源：http://bxm.xziqi.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://vwk.fehbvm.com

[U83] JS：ES Module 导入导出
来源：http://bur.sjlbkw.cn

export const a = 1;  import { a } from "./m.js";
来源：http://ksu.ppjwa.cn

[U84] JS：CommonJS 写法
来源：http://uok.fehbvm.com

module.exports = { a };  const { a } = require("./m");
来源：http://mgh.tarul.cn

[U85] JS：可选链
来源：http://dhg.bbcook.cn

a?.b?.c
来源：http://irc.sysykeji.top

[U86] JS：空值合并
来源：http://uqk.tianlin.xyz

a ?? b
来源：http://rdj.sysykeji.top

[U87] JS：解构默认值
来源：http://lug.vehdjk.com

const { a = 1, b = 2 } = obj;
来源：http://khx.birdmap.top

[U88] JS：对象展开合并
来源：http://ztx.ehwqpu.com

{ ...a, ...b }
来源：http://rbu.epnwcf.com

[U89] JS：数组去重
来源：http://ghw.dianchejie.cn

[...new Set(arr)]
来源：http://cbp.ivvv.top

[U90] JS：数字数组排序
来源：http://qdb.zhiwuduotai.top

[...arr].sort((a, b) => a - b)
来源：http://ofr.nanxuanxn.top

[U91] JS：对象键值遍历
来源：http://euq.0kj1m.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://qdq.xylfe.cn

[U92] JS：深拷贝
来源：http://kio.hfpthk.cn

structuredClone(obj)
来源：http://yrz.ctjpmb.com

[U93] JS：模板字符串
来源：http://qpf.zdbjq.cn

`共 ${n} 条`
来源：http://ata.yj20258888.top

[U94] JS：箭头函数
来源：http://ton.yonumen.top

const double = x => x * 2;
来源：http://gjm.hcnkem.com

[U95] JS：Promise 包装
来源：http://lsz.wangdashe.top

new Promise((resolve, reject) => {})
来源：http://tsw.fehbvm.com

[U96] JS：async/await 与异常
来源：http://hdv.gotoacloud.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://eqn.wangshuangyany.cn

[U97] JS：并发请求
来源：http://phi.chenzaomai.com

await Promise.all(urls.map(u => fetch(u)))
来源：http://kln.xingfuxueyuan.xyz

[U98] JS：fetch 带 JSON
来源：http://gna.0kj1m.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://pqm.hammf.cn

[U99] JS：事件监听
来源：http://qqt.jianghu66.top

el.addEventListener("click", e => {})
来源：http://unm.shanyushiyangkeji.top

[U100] JS：DOM 查询
来源：http://hqb.yongpay.top

document.querySelector(".item")
来源：http://cwg.meibo888.top

[U101] JS：classList 操作
来源：http://ruu.zhoulong.xyz

el.classList.toggle("active")
来源：http://jpp.guannengcc.top

[U102] JS：本地存储
来源：http://qzj.jlsjyb.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://fcd.redwolf501.top

[U103] JS：定时器
来源：http://vab.yfazqb.com

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://chv.zhijiandao.cn

[U104] JS：防抖
来源：http://doe.aizwys.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://bcr.xuetiantiany.cn

[U105] JS：节流
来源：http://mgw.jlsjyb.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://vpn.zdqjudy.top

[U106] JS：日期格式化
来源：http://uxa.chenzaomai.com

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://nys.hesvh.cn

[U107] JS：数字千分位
来源：http://opi.gogol.net.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://kpk.smart0.xyz

[U108] JS：随机整数
来源：http://bwd.gaohongyu789.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hxq.jinghuilouyu.cn

[U109] JS：数组分组
来源：http://iht.yonumen.top

Object.groupBy(arr, x => x.type)
来源：http://sex.yonumen.top

[U110] JS：数组分块
来源：http://dzn.uphjek.com

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://pjw.havefunace.top

[U111] JS：对象转 Map
来源：http://xjf.nanxinkj.top

new Map(Object.entries(obj))
来源：http://mbs.fengsongda.top

[U112] JS：字符串补位
来源：http://wqh.aizwys.cn

"7".padStart(3, "0")
来源：http://bir.jianghu66.top

[U113] JS：正则替换全部
来源：http://bik.zhijiandao.cn

s.replaceAll("a", "b")
来源：http://wty.yangfankeji.com

[U114] JS：JSON 深比较
来源：http://tiu.tian-w.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://ymj.ybcxt.top

[U115] JS：生成 UUID
来源：http://fxe.shanyushiyangkeji.top

crypto.randomUUID()
来源：http://wiv.ywan-chungtsiang.top

[U116] JS：类型检查（JSDoc）
来源：http://bsg.tarul.cn

/** @param {string} name */ function f(name) {}
来源：http://frn.haohaochexian.top

[U117] JS：单元测试
来源：http://ylm.yvedp.cn

npm i -D vitest;  npx vitest
来源：http://lxy.daxiang520.top

[U118] JS：开发服务器
来源：http://xwd.jiagoushi.top

npm i -D vite;  npx vite
来源：http://bln.hongshengwenyu.top

[U119] JS：生产构建
来源：http://qov.jinyuanbaomall.cn

npx vite build
来源：http://jub.ivvv.top

[U120] JS：读取环境变量（Vite）
来源：http://hxn.zhoulong.xyz

import.meta.env.VITE_API_URL
来源：http://dkw.ydjk.org.cn

================================================================================
来源：http://sjk.wangshuangyany.cn

统计汇总
来源：http://qcv.yangfankeji.com

================================================================================
来源：http://oab.yj202588.top

按语言统计（条）：
来源：http://dth.fehbvm.com

Python ......... 252
来源：http://vir.zhiwuduotai.top

PHP ............ 252
来源：http://lrq.dianchejie.cn

JavaScript ..... 252
来源：http://oes.hesvh.cn

TypeScript ..... 212
来源：http://yfy.yongpay.top

Java ........... 212
来源：http://okm.cheryme.top

Go ............. 212
来源：http://wmm.tian-w.cn

Ruby ........... 212
来源：http://lrl.zhiwuduotai.top

C# ............. 212
来源：http://uyo.xziqi.cn

C .............. 30
来源：http://zuh.sysykeji.top

C++ ............ 30
来源：http://twn.zdbjq.cn

SQL ............ 90
来源：http://fnq.tarul.cn

Bash ........... 80
来源：http://vkb.cheryme.top

Kotlin ......... 15
来源：http://yyc.guowangkeji.top

Swift .......... 15
来源：http://rqz.feifeiyinyue.top

Lua ............ 10
来源：http://jen.sweek.top

Perl ........... 10
来源：http://uyw.fengsongda.top

Scala .......... 10
来源：http://yub.jiagoushi.top

------------------------------------
来源：http://pst.bjfxy.top

合计 ........... 2106 条
来源：http://mod.sxryk.cn

按章节统计：
来源：http://ifs.ydzc1.top


<!-- 参考信息 -->