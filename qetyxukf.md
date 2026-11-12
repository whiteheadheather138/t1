代发 wailian999

[T45] Perl：数组遍历
来源：http://vmz.cqqwz.cn

for my $x (@arr) { print $x; }
来源：http://vku.shzxlz.cn

[T46] Perl：哈希操作
来源：http://awk.cucudq.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://vqs.jianghu66.top

[T47] Perl：正则捕获
来源：http://jea.mhx1999.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://bdu.jlsjyb.cn

[T48] Perl：正则替换
来源：http://jwh.c1oappe.top

$s =~ s/old/new/g;
来源：http://jwm.ppjwa.cn

[T49] Perl：函数
来源：http://qcb.jlsjyb.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://izq.ydzc1.top

[T50] Perl：逐行读文件
来源：http://wma.redwolf501.top

open my $fh, "<", "a.txt" or die $!;
来源：http://akx.daria6918.cn

while (my $line = <$fh>) { print $line; }
来源：http://gga.fktsv.cn

[T51] Scala：Hello World
来源：http://avc.kuanghao11.cn

println("Hello")
来源：http://ixw.daria6918.cn

[T52] Scala：变量
来源：http://swu.birdmap.top

val a = 1;  var b = 2
来源：http://ycy.yonumen.top

[T53] Scala：字符串插值
来源：http://bfn.aizwys.cn

s"值: $b"
来源：http://wpl.wangshuangyany.cn

[T54] Scala：集合映射
来源：http://pcp.yuanzhike.top

List(1, 2, 3).map(_ * 2)
来源：http://chw.daxiang520.top

[T55] Scala：集合过滤
来源：http://jye.zdqjudy.top

List(1, 2, 3).filter(_ > 1)
来源：http://zeq.jlsjyb.cn

[T56] Scala：样例类
来源：http://hmh.wangshuangyany.cn

case class User(name: String, age: Int)
来源：http://gtn.tianlin.xyz

[T57] Scala：模式匹配
来源：http://emq.nwbrower.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://axs.ppjwa.cn

[T58] Scala：函数定义
来源：http://meu.redwolf501.top

def add(a: Int, b: Int): Int = a + b
来源：http://ayj.jyoumei.cn

[T59] Scala：循环
来源：http://lam.sufxvd.cn

for (i <- 1 to 10) println(i)
来源：http://xez.ivvv.top

[T60] Scala：折叠
来源：http://iaq.nanxuanxn.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://odn.aibaodan.cn

================================================================================
来源：http://bpo.redwolf501.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://brw.yonumen.top

================================================================================
来源：http://hch.52xcode.cn

[U01] Py：创建虚拟环境
来源：http://jwz.zhaomingkeji.xyz

python -m venv .venv && source .venv/bin/activate
来源：http://cxh.fanxiaobao.xyz

[U02] Py：导出 / 安装依赖
来源：http://jfl.cdnleiting.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://xoh.nanxinkj.top

[U03] Py：加载 .env 配置
来源：http://jhi.epnwcf.com

from dotenv import load_dotenv; load_dotenv()
来源：http://wlj.ivvv.top

[U04] Py：变量调试打印
来源：http://xgp.cdnleiting.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://daw.9152youxi.cn

[U05] Py：列表去重且保序
来源：http://uzh.jqgufenzy.top

list(dict.fromkeys(arr))
来源：http://wmg.ppjwa.cn

[U06] Py：合并两个字典
来源：http://sgd.xziqi.cn

{**a, **b}
来源：http://crk.ydjk.org.cn

[U07] Py：反转字典键值
来源：http://wwl.ppjwa.cn

{v: k for k, v in d.items()}
来源：http://uny.52xcode.cn

[U08] Py：展平二维列表
来源：http://qyq.tianlin.xyz

[y for x in nested for y in x]
来源：http://ejz.zdqjudy.top

[U09] Py：字典取最大值的键
来源：http://yvc.nanxuanxn.top

max(d, key=d.get)
来源：http://loe.yongpay.top

[U10] Py：按值排序字典
来源：http://flm.smart0.xyz

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://elr.bjfxy.top

[U11] Py：生成器表达式
来源：http://ams.hywenlv.cn

(x * 2 for x in arr)
来源：http://pcs.svipenyu.cn

[U12] Py：取出现最多的 3 个元素
来源：http://rnq.jyoumei.cn

Counter(arr).most_common(3)
来源：http://ohv.shanyushiyangkeji.top

[U13] Py：固定长度队列
来源：http://etu.shanyushiyangtech.top

deque(maxlen=10)
来源：http://wbt.pycfn.com

[U14] Py：分组收集到列表
来源：http://rix.zhoulong.xyz

defaultdict(list)
来源：http://wil.jqgufenzy.top

[U15] Py：高精度计时
来源：http://yre.haohaochexian.top

t = time.perf_counter()
来源：http://mih.zdbjq.cn

[U16] Py：命令行参数解析
来源：http://pwu.yuxming.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://isq.hesvh.cn

[U17] Py：初始化日志
来源：http://psy.havefunace.top

logging.basicConfig(level=logging.INFO)
来源：http://yho.xuanzx.com

[U18] Py：预编译正则
来源：http://lqx.hesvh.cn

pat = re.compile(r"\d+")
来源：http://bfi.haohaochexian.top

[U19] Py：正则替换带回调
来源：http://tml.yfazqb.com

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://yef.jlsjyb.cn

[U20] Py：缓存函数结果
来源：http://kaw.pengpengdd.cyou

@functools.lru_cache(maxsize=None)
来源：http://ifj.zycfv.cn

[U21] Py：自定义上下文管理器
来源：http://rdv.xuetiantiany.cn

@contextlib.contextmanager
来源：http://seu.hysaishi.cn

[U22] Py：矩阵转置
来源：http://dwj.shzxlz.cn

list(zip(*m))
来源：http://ooh.yuxming.cn

[U23] Py：分块读取大文件
来源：http://psv.jinyuanbaomall.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://nsk.zhiwuduotai.top

[U24] Py：路径操作
来源：http://iky.jyoumei.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://vex.zhixingplan.top

[U25] Py：CSV 按字典读
来源：http://nsl.zhaomingkeji.xyz

csv.DictReader(f)
来源：http://twr.tianlin.xyz

[U26] Py：并发下载
来源：http://iaq.ydjk.org.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://yjb.zhaomingkeji.xyz

[U27] Py：异步 HTTP
来源：http://nei.fktsv.cn

aiohttp.ClientSession() 配合 async with
来源：http://ucv.kuanghao11.cn

[U28] Py：类型别名
来源：http://gid.fanxiaobao.xyz

UserId = int
来源：http://lto.yuxming.cn

[U29] Py：属性校验
来源：http://duw.bbcook.cn

@property 与 @x.setter 配合
来源：http://qpw.chenjidiqi.icu

[U30] Py：数据类
来源：http://eir.zhengqikj.top

@dataclass(slots=True)
来源：http://gcf.andypj.xyz

[U31] Py：单测
来源：http://egs.gotoacloud.top

python -m pytest -q
来源：http://zpx.yonumen.top

[U32] Py：代码格式化
来源：http://qdz.yj20258888.top

ruff format . && ruff check --fix .
来源：http://zkc.aizwys.cn

[U33] Py：打包发布
来源：http://iui.tianlin.xyz

python -m build  （依赖 pyproject.toml）
来源：http://xdt.guannengcc.top

[U34] Py：判断编码
来源：http://jya.ydzc1.top

chardet.detect(raw)
来源：http://ibb.zhoulong.xyz

[U35] Py：发送邮件
来源：http://jyh.shanyushiyangtech.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://zmf.zhengqikj.top

[U36] Py：定时任务
来源：http://kzn.daria6918.cn

schedule.every(10).minutes.do(job)
来源：http://mpk.meibo888.top

[U37] Py：读写 Excel
来源：http://dgv.sxryk.cn

pandas.read_excel / DataFrame.to_excel
来源：http://ivp.havefunace.top

[U38] Py：获取脚本所在目录
来源：http://arj.pycfn.com

Path(__file__).resolve().parent
来源：http://jhg.yj20258.top

[U39] Py：判断是否在交互环境
来源：http://ogr.xziqi.cn

sys.stdout.isatty()
来源：http://yxn.iojbl.cn

[U40] Py：打印到标准错误
来源：http://rqs.yueranfly.top

print("err", file=sys.stderr)
来源：http://hbs.xziqi.cn

[U41] PHP：初始化 Composer 项目
来源：http://xls.xziqi.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://sdq.fktsv.cn

[U42] PHP：PSR-4 自动加载
来源：http://aui.ybcxt.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hix.c1oappe.top

[U43] PHP：声明命名空间
来源：http://onb.yvedp.cn

namespace App\Http;
来源：http://zku.jinqigfzy.top

[U44] PHP：开启严格类型
来源：http://mpx.zycfv.cn

declare(strict_types=1);
来源：http://sja.redwolf501.top

[U45] PHP：类型声明与返回类型
来源：http://hcp.mhx1999.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://trq.aizwys.cn

[U46] PHP：可空类型
来源：http://cys.ctjpmb.com

?string $name = null
来源：http://bdh.fzhhl.top

[U47] PHP：联合类型
来源：http://xmr.bbcook.cn

int|string $id
来源：http://hzc.hammf.cn

[U48] PHP：纯枚举
来源：http://dhc.yvedp.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://gjp.fehbvm.com

[U49] PHP：只读属性
来源：http://jrw.gzhubu.top

public readonly string $name
来源：http://lkx.hesvh.cn

[U50] PHP：构造器属性提升
来源：http://uog.wangshuangyany.cn

public function __construct(private int $id) {}
来源：http://fvu.gotoacloud.top

[U51] PHP：数组解构
来源：http://onr.yuanzhike.top

[$a, $b] = $arr;
来源：http://ita.fanxiaobao.xyz

[U52] PHP：箭头函数
来源：http://eri.nanxuanxn.top

$double = fn($x) => $x * 2;
来源：http://ubf.jlsjyb.cn

[U53] PHP：空合并运算符
来源：http://nqk.xingfuxueyuan.xyz

$v = $a ?? $b ?? "default";
来源：http://atu.havefunace.top

[U54] PHP：空安全调用
来源：http://plp.316326.xyz

$obj?->method()
来源：http://wfz.sxryk.cn

[U55] PHP：match 表达式
来源：http://ady.gzhubu.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://yth.hcnkem.com

[U56] PHP：命名参数
来源：http://mhf.yvedp.cn

f(a: 1, b: 2)
来源：http://dxk.hnqzz.top

[U57] PHP：字符串插值
来源：http://oaw.sysykeji.top

"值: {$a}"
来源：http://pog.epnwcf.com

[U58] PHP：数组三件套
来源：http://ssb.meibo888.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://tjy.shuidangran.top

[U59] PHP：自定义排序
来源：http://ctq.yanxiufei.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mqw.gotoacloud.top

[U60] PHP：JSON 编解码
来源：http://dgt.havefunace.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://iol.hammf.cn

[U61] PHP：正则
来源：http://sno.shangyingyoupin.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://eqq.chenjidiqi.icu

[U62] PHP：日期对象
来源：http://rxc.yfazqb.com

(new DateTimeImmutable())->format("Y-m-d");
来源：http://cwn.shuidangran.top

[U63] PHP：文件读写
来源：http://inh.iojbl.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://iej.xziqi.cn

[U64] PHP：目录遍历
来源：http://xlk.c1oappe.top

glob("dir/*.php");  scandir("dir");
来源：http://dqu.yongpay.top

[U65] PHP：会话
来源：http://xpv.pycfn.com

session_start();  $_SESSION["uid"] = 1;
来源：http://bcz.svipenyu.cn

[U66] PHP：设置 Cookie
来源：http://ckl.tianlin.xyz

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://qpt.jqgfzy.top

[U67] PHP：处理文件上传
来源：http://ihb.zhaomingkeji.xyz

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://pmp.yj202588.top

[U68] PHP：PDO 连接
来源：http://klq.xuanzx.com

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://cmh.yvedp.cn

[U69] PHP：PDO 预处理
来源：http://mto.sxryk.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://ypi.chenzaomai.com

[U70] PHP：PDO 事务
来源：http://yrc.jiagoushi.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://trv.jlsjyb.cn

[U71] PHP：抛出异常
来源：http://ony.yuanzhike.top

throw new RuntimeException("失败", 500);
来源：http://uqg.9152youxi.cn

[U72] PHP：写错误日志
来源：http://grj.nwbrower.top

error_log("失败: " . $e->getMessage());
来源：http://rvt.ehwqpu.com

[U73] PHP：读取 ini 配置
来源：http://yje.jlsjyb.cn

parse_ini_file("config.ini", true)
来源：http://uop.yj202588.top

[U74] PHP：读取环境变量
来源：http://qeg.bbcook.cn

getenv("APP_ENV") ?: "production"
来源：http://mlj.fzhhl.top

[U75] PHP：依赖注入
来源：http://jzu.kuanghao11.cn

composer require psr/container
来源：http://yjr.xuanzx.com

[U76] PHP：简单路由
来源：http://fwx.shanyushiyangtech.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://dct.dashuyun.cn

[U77] PHP：模板渲染
来源：http://fic.tanke756.top

composer require twig/twig
来源：http://pqj.jinqigufen.top

[U78] PHP：单元测试
来源：http://srn.sweek.top

composer require --dev phpunit/phpunit
来源：http://pfm.yj202588.top

[U79] PHP：静态分析
来源：http://yud.ctjpmb.com

composer require --dev phpstan/phpstan
来源：http://iqk.aizwys.cn

[U80] PHP：代码规范修复
来源：http://gtt.fehbvm.com

composer require --dev friendsofphp/php-cs-fixer
来源：http://idl.snrcjt.cn

[U81] JS：初始化项目
来源：http://mgl.yfazqb.com

npm init -y;  npm i express
来源：http://zhr.jyoumei.cn

[U82] JS：package.json 脚本
来源：http://pix.daria6918.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://bqb.fehbvm.com

[U83] JS：ES Module 导入导出
来源：http://qpt.smart0.xyz

export const a = 1;  import { a } from "./m.js";
来源：http://jrw.hammf.cn

[U84] JS：CommonJS 写法
来源：http://sle.yonumen.top

module.exports = { a };  const { a } = require("./m");
来源：http://qrv.zhongyouzk.top

[U85] JS：可选链
来源：http://reh.ivvv.top

a?.b?.c
来源：http://ilh.havefunace.top

[U86] JS：空值合并
来源：http://oci.snrcjt.cn

a ?? b
来源：http://yxq.zhoulong.xyz

[U87] JS：解构默认值
来源：http://twn.ydzc1.top

const { a = 1, b = 2 } = obj;
来源：http://blu.xylfe.cn

[U88] JS：对象展开合并
来源：http://ovd.xuetiantiany.cn

{ ...a, ...b }
来源：http://dpv.fehbvm.com

[U89] JS：数组去重
来源：http://zdc.hongshengwenyu.top

[...new Set(arr)]
来源：http://spo.gogol.net.cn

[U90] JS：数字数组排序
来源：http://gwd.sweek.top

[...arr].sort((a, b) => a - b)
来源：http://ucn.316326.xyz

[U91] JS：对象键值遍历
来源：http://pvg.ybcxt.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://wyv.yuanzhike.top

[U92] JS：深拷贝
来源：http://hqe.aizwys.cn

structuredClone(obj)
来源：http://bjq.tianlin.xyz

[U93] JS：模板字符串
来源：http://elu.zdbjq.cn

`共 ${n} 条`
来源：http://zou.iojbl.cn

[U94] JS：箭头函数
来源：http://you.aibaodan.cn

const double = x => x * 2;
来源：http://uzo.fehbvm.com

[U95] JS：Promise 包装
来源：http://nnb.sxryk.cn

new Promise((resolve, reject) => {})
来源：http://wxz.yangfankeji.com

[U96] JS：async/await 与异常
来源：http://ask.aibaodan.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://gmh.ehwqpu.com

[U97] JS：并发请求
来源：http://yuz.uphjek.com

await Promise.all(urls.map(u => fetch(u)))
来源：http://xpg.c1oappe.top

[U98] JS：fetch 带 JSON
来源：http://hys.pycfn.com

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://wmc.vqdsnc.cn

[U99] JS：事件监听
来源：http://moz.hesvh.cn

el.addEventListener("click", e => {})
来源：http://bca.zhiwuduotai.top

[U100] JS：DOM 查询
来源：http://tgg.cucudq.cn

document.querySelector(".item")
来源：http://vbk.chenjidiqi.icu

[U101] JS：classList 操作
来源：http://ejv.xinyue.icu

el.classList.toggle("active")
来源：http://kti.shanyushiyangkeji.top

[U102] JS：本地存储
来源：http://jzg.chenlongwang.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://dve.jqgufenzy.top

[U103] JS：定时器
来源：http://dvm.hongshengwenyu.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://rsi.yongpay.top

[U104] JS：防抖
来源：http://uiz.hammf.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://khr.jiagoushi.top

[U105] JS：节流
来源：http://bze.epnwcf.com

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://trp.zycfv.cn

[U106] JS：日期格式化
来源：http://ooa.hywenlv.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://ftb.nanxuanxn.top

[U107] JS：数字千分位
来源：http://ymz.zhaomingkeji.xyz

new Intl.NumberFormat("en-US").format(1234567)
来源：http://nqh.zhiwuduotai.top

[U108] JS：随机整数
来源：http://tcg.nanxuanxn.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://cqx.jqgfzy.top

[U109] JS：数组分组
来源：http://hzy.daxiang520.top

Object.groupBy(arr, x => x.type)
来源：http://mwq.316326.xyz

[U110] JS：数组分块
来源：http://imj.haohaochexian.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://nmv.ehwqpu.com

[U111] JS：对象转 Map
来源：http://xvy.dashuyun.cn

new Map(Object.entries(obj))
来源：http://ojz.chenzaomai.com

[U112] JS：字符串补位
来源：http://bfm.fzhhl.top

"7".padStart(3, "0")
来源：http://xdy.zhixingplan.top

[U113] JS：正则替换全部
来源：http://dph.yangfankeji.com

s.replaceAll("a", "b")
来源：http://mqa.hfpthk.cn

[U114] JS：JSON 深比较
来源：http://piq.ctjpmb.com

JSON.stringify(a) === JSON.stringify(b)
来源：http://fzn.zdqjudy.top

[U115] JS：生成 UUID
来源：http://cxi.shangyingyoupin.top

crypto.randomUUID()
来源：http://stv.c1oappe.top

[U116] JS：类型检查（JSDoc）
来源：http://fma.shangyingyoupin.top

/** @param {string} name */ function f(name) {}
来源：http://ezc.xylfe.cn

[U117] JS：单元测试
来源：http://nri.jinqigufen.top

npm i -D vitest;  npx vitest
来源：http://zsx.wangdashe.top

[U118] JS：开发服务器
来源：http://bwz.mhx1999.top

npm i -D vite;  npx vite
来源：http://foc.sufxvd.cn

[U119] JS：生产构建
来源：http://tnc.sufxvd.cn

npx vite build
来源：http://iyn.xuetiantiany.cn

[U120] JS：读取环境变量（Vite）
来源：http://brb.gzhubu.top

import.meta.env.VITE_API_URL
来源：http://cbt.9152youxi.cn

================================================================================
来源：http://iop.gzhubu.top

统计汇总
来源：http://cqi.ybcxt.top

================================================================================
来源：http://qwy.nwbrower.top

按语言统计（条）：
来源：http://lvh.wangshuangyany.cn

Python ......... 252
来源：http://fhc.yueranfly.top

PHP ............ 252
来源：http://nfg.tanke756.top

JavaScript ..... 252
来源：http://wzb.gzhubu.top

TypeScript ..... 212
来源：http://qxt.52xcode.cn

Java ........... 212
来源：http://nia.svipenyu.cn

Go ............. 212
来源：http://syi.quarkkingdee.top

Ruby ........... 212
来源：http://hux.chenlongwang.top

C# ............. 212
来源：http://bhs.kuanghao11.cn

C .............. 30
来源：http://ufc.yj20258888.top

C++ ............ 30
来源：http://chq.jiagoushi.top

SQL ............ 90
来源：http://vam.jinqigufen.top

Bash ........... 80
来源：http://eoq.fengsongda.top

Kotlin ......... 15
来源：http://bgg.hammf.cn

Swift .......... 15
来源：http://uhg.aizwys.cn

Lua ............ 10
来源：http://zta.hysaishi.cn

Perl ........... 10
来源：http://mxq.yvedp.cn

Scala .......... 10
来源：http://tzb.yonumen.top

------------------------------------
来源：http://fkr.hnxiangtu.top

合计 ........... 2106 条
来源：http://tub.ehwqpu.com

按章节统计：
来源：http://fte.yanxiufei.cn


<!-- 参考信息 -->