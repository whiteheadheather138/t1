代发 wailian999

[T45] Perl：数组遍历
来源：http://pwl.xinyue.icu

for my $x (@arr) { print $x; }
来源：http://nik.cheryme.top

[T46] Perl：哈希操作
来源：http://ihi.zhoulong.xyz

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://rak.xuetiantiany.cn

[T47] Perl：正则捕获
来源：http://fna.zdqjudy.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://pse.cheryme.top

[T48] Perl：正则替换
来源：http://oog.fktsv.cn

$s =~ s/old/new/g;
来源：http://axz.ybcxt.top

[T49] Perl：函数
来源：http://zwr.jianghu66.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://tck.ywan-chungtsiang.top

[T50] Perl：逐行读文件
来源：http://etg.wangshuangyany.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://xrr.andypj.xyz

while (my $line = <$fh>) { print $line; }
来源：http://skb.chenzaomai.com

[T51] Scala：Hello World
来源：http://vom.zhoulong.xyz

println("Hello")
来源：http://pnx.jinqigufen.top

[T52] Scala：变量
来源：http://bhm.hfpthk.cn

val a = 1;  var b = 2
来源：http://isg.andypj.xyz

[T53] Scala：字符串插值
来源：http://ksm.guannengcc.top

s"值: $b"
来源：http://def.ydzc1.top

[T54] Scala：集合映射
来源：http://yyz.vqdsnc.cn

List(1, 2, 3).map(_ * 2)
来源：http://map.tianlin.xyz

[T55] Scala：集合过滤
来源：http://pct.jianghu66.top

List(1, 2, 3).filter(_ > 1)
来源：http://ziv.zhijiandao.cn

[T56] Scala：样例类
来源：http://wmw.havefunace.top

case class User(name: String, age: Int)
来源：http://afa.xinyue.icu

[T57] Scala：模式匹配
来源：http://zht.hywenlv.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://ozq.yj202588.top

[T58] Scala：函数定义
来源：http://nlf.gaohongyu789.top

def add(a: Int, b: Int): Int = a + b
来源：http://yfj.zhoulong.xyz

[T59] Scala：循环
来源：http://ytm.zhijiandao.cn

for (i <- 1 to 10) println(i)
来源：http://chm.tian-w.cn

[T60] Scala：折叠
来源：http://tkl.shangyingyoupin.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://slg.ctjpmb.com

================================================================================
来源：http://ged.xinyue.icu

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://glu.cheryme.top

================================================================================
来源：http://foa.yuxming.cn

[U01] Py：创建虚拟环境
来源：http://tlk.yvedp.cn

python -m venv .venv && source .venv/bin/activate
来源：http://nrz.fengsongda.top

[U02] Py：导出 / 安装依赖
来源：http://zoz.316326.xyz

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://tmb.0kj1m.cn

[U03] Py：加载 .env 配置
来源：http://nty.tarul.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://ghy.pycfn.com

[U04] Py：变量调试打印
来源：http://oei.snrcjt.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://vqr.hcnkem.com

[U05] Py：列表去重且保序
来源：http://zqp.c1oappe.top

list(dict.fromkeys(arr))
来源：http://hom.shzxlz.cn

[U06] Py：合并两个字典
来源：http://lbx.sjlbkw.cn

{**a, **b}
来源：http://ydl.tian-w.cn

[U07] Py：反转字典键值
来源：http://akv.ehwqpu.com

{v: k for k, v in d.items()}
来源：http://wmj.52xcode.cn

[U08] Py：展平二维列表
来源：http://vdp.ydjk.org.cn

[y for x in nested for y in x]
来源：http://rlt.quarkkingdee.top

[U09] Py：字典取最大值的键
来源：http://ljb.jqgfzy.top

max(d, key=d.get)
来源：http://pnm.ppjwa.cn

[U10] Py：按值排序字典
来源：http://tjr.guowangkeji.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://vzk.meibo888.top

[U11] Py：生成器表达式
来源：http://bqo.wangshuangyany.cn

(x * 2 for x in arr)
来源：http://lzg.cashguo.top

[U12] Py：取出现最多的 3 个元素
来源：http://hrd.vehdjk.com

Counter(arr).most_common(3)
来源：http://rkt.chenjidiqi.icu

[U13] Py：固定长度队列
来源：http://ntp.sufxvd.cn

deque(maxlen=10)
来源：http://brs.yuxming.cn

[U14] Py：分组收集到列表
来源：http://cyn.pycfn.com

defaultdict(list)
来源：http://ajb.jiagoushi.top

[U15] Py：高精度计时
来源：http://qpq.ehwqpu.com

t = time.perf_counter()
来源：http://kzg.0kj1m.cn

[U16] Py：命令行参数解析
来源：http://nfb.ehwqpu.com

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://kiz.xingfuxueyuan.xyz

[U17] Py：初始化日志
来源：http://wvn.dashuyun.cn

logging.basicConfig(level=logging.INFO)
来源：http://tkm.ydzc1.top

[U18] Py：预编译正则
来源：http://ogt.cqqwz.cn

pat = re.compile(r"\d+")
来源：http://tfx.aibaodan.cn

[U19] Py：正则替换带回调
来源：http://lun.andypj.xyz

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://azm.guannengcc.top

[U20] Py：缓存函数结果
来源：http://wyx.jiagoushi.top

@functools.lru_cache(maxsize=None)
来源：http://lth.hammf.cn

[U21] Py：自定义上下文管理器
来源：http://oza.52xcode.cn

@contextlib.contextmanager
来源：http://vrw.chenjidiqi.icu

[U22] Py：矩阵转置
来源：http://cis.zhoulong.xyz

list(zip(*m))
来源：http://hgk.havefunace.top

[U23] Py：分块读取大文件
来源：http://pww.shanyushiyangkeji.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://xdq.0kj1m.cn

[U24] Py：路径操作
来源：http://smn.snrcjt.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://uqc.tian-w.cn

[U25] Py：CSV 按字典读
来源：http://okr.bjfxy.top

csv.DictReader(f)
来源：http://yda.xziqi.cn

[U26] Py：并发下载
来源：http://too.chenzaomai.com

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://dpn.tian-w.cn

[U27] Py：异步 HTTP
来源：http://yyj.tian-w.cn

aiohttp.ClientSession() 配合 async with
来源：http://sbp.kuanghao11.cn

[U28] Py：类型别名
来源：http://pbb.jlsjyb.cn

UserId = int
来源：http://ksp.guannengcc.top

[U29] Py：属性校验
来源：http://mkq.yj202588.top

@property 与 @x.setter 配合
来源：http://hmn.feifeiyinyue.top

[U30] Py：数据类
来源：http://udu.cheryme.top

@dataclass(slots=True)
来源：http://fjk.vqdsnc.cn

[U31] Py：单测
来源：http://eci.yuxming.cn

python -m pytest -q
来源：http://ydr.shuidangran.top

[U32] Py：代码格式化
来源：http://sdb.jinyuanbaomall.cn

ruff format . && ruff check --fix .
来源：http://odv.iojbl.cn

[U33] Py：打包发布
来源：http://tng.guannengcc.top

python -m build  （依赖 pyproject.toml）
来源：http://puw.c1oappe.top

[U34] Py：判断编码
来源：http://gqi.shzxlz.cn

chardet.detect(raw)
来源：http://uch.ydjk.org.cn

[U35] Py：发送邮件
来源：http://akl.pycfn.com

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://sur.gogol.net.cn

[U36] Py：定时任务
来源：http://wxx.iojbl.cn

schedule.every(10).minutes.do(job)
来源：http://fdy.sufxvd.cn

[U37] Py：读写 Excel
来源：http://uae.uphjek.com

pandas.read_excel / DataFrame.to_excel
来源：http://lde.vqdsnc.cn

[U38] Py：获取脚本所在目录
来源：http://sia.zhoulong.xyz

Path(__file__).resolve().parent
来源：http://use.cashguo.top

[U39] Py：判断是否在交互环境
来源：http://yfj.cucudq.cn

sys.stdout.isatty()
来源：http://rlu.xingfuxueyuan.xyz

[U40] Py：打印到标准错误
来源：http://vja.jlsjyb.cn

print("err", file=sys.stderr)
来源：http://ids.jinyuanbaomall.cn

[U41] PHP：初始化 Composer 项目
来源：http://zkh.iojbl.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://myp.andypj.xyz

[U42] PHP：PSR-4 自动加载
来源：http://vli.havefunace.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://acg.jinqigfzy.top

[U43] PHP：声明命名空间
来源：http://hzw.cdnleiting.top

namespace App\Http;
来源：http://fcc.feifeiyinyue.top

[U44] PHP：开启严格类型
来源：http://cpo.guowangkeji.top

declare(strict_types=1);
来源：http://vjg.zdbjq.cn

[U45] PHP：类型声明与返回类型
来源：http://ydt.iojbl.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://oop.9152youxi.cn

[U46] PHP：可空类型
来源：http://gvy.sysykeji.top

?string $name = null
来源：http://dna.gaohongyu789.top

[U47] PHP：联合类型
来源：http://gck.ydjk.org.cn

int|string $id
来源：http://niz.hcnkem.com

[U48] PHP：纯枚举
来源：http://hci.kuanghao11.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://lng.ppjwa.cn

[U49] PHP：只读属性
来源：http://cvv.xylfe.cn

public readonly string $name
来源：http://gce.xylfe.cn

[U50] PHP：构造器属性提升
来源：http://res.yanxiufei.cn

public function __construct(private int $id) {}
来源：http://vic.9152youxi.cn

[U51] PHP：数组解构
来源：http://lak.fanxiaobao.xyz

[$a, $b] = $arr;
来源：http://tsm.yuxming.cn

[U52] PHP：箭头函数
来源：http://oey.wangshuangyany.cn

$double = fn($x) => $x * 2;
来源：http://bma.xuanzx.com

[U53] PHP：空合并运算符
来源：http://esv.smart0.xyz

$v = $a ?? $b ?? "default";
来源：http://llf.tarul.cn

[U54] PHP：空安全调用
来源：http://grv.jinqigfzy.top

$obj?->method()
来源：http://rqp.yongpay.top

[U55] PHP：match 表达式
来源：http://eaq.ydjk.org.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://buf.hywenlv.cn

[U56] PHP：命名参数
来源：http://nev.tian-w.cn

f(a: 1, b: 2)
来源：http://bsr.jinyuanbaomall.cn

[U57] PHP：字符串插值
来源：http://vqf.quarkkingdee.top

"值: {$a}"
来源：http://qjw.hongshengwenyu.top

[U58] PHP：数组三件套
来源：http://rsz.shanyushiyangtech.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://wbc.c1oappe.top

[U59] PHP：自定义排序
来源：http://dbr.fehbvm.com

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://msj.fengsongda.top

[U60] PHP：JSON 编解码
来源：http://vvy.pengpengdd.cyou

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://wrb.chenzaomai.com

[U61] PHP：正则
来源：http://dxv.hcnkem.com

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://wik.yj20258.top

[U62] PHP：日期对象
来源：http://pwg.smart0.xyz

(new DateTimeImmutable())->format("Y-m-d");
来源：http://god.c1oappe.top

[U63] PHP：文件读写
来源：http://twm.gotoacloud.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://key.yj202588.top

[U64] PHP：目录遍历
来源：http://aig.yuxming.cn

glob("dir/*.php");  scandir("dir");
来源：http://msy.xuetiantiany.cn

[U65] PHP：会话
来源：http://pqu.aizwys.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://wzl.jyoumei.cn

[U66] PHP：设置 Cookie
来源：http://ywo.dianchejie.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://oey.bbcook.cn

[U67] PHP：处理文件上传
来源：http://jci.dianchejie.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://iqu.shanyushiyangtech.top

[U68] PHP：PDO 连接
来源：http://gws.hnxiangtu.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://vqo.snrcjt.cn

[U69] PHP：PDO 预处理
来源：http://uox.fengsongda.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://spw.gaohongyu789.top

[U70] PHP：PDO 事务
来源：http://rvz.hysaishi.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://bqo.haohaochexian.top

[U71] PHP：抛出异常
来源：http://jiy.yvedp.cn

throw new RuntimeException("失败", 500);
来源：http://jut.dashuyun.cn

[U72] PHP：写错误日志
来源：http://jle.gaohongyu789.top

error_log("失败: " . $e->getMessage());
来源：http://ogi.feifeiyinyue.top

[U73] PHP：读取 ini 配置
来源：http://pkq.jinghuilouyu.cn

parse_ini_file("config.ini", true)
来源：http://ynq.havefunace.top

[U74] PHP：读取环境变量
来源：http://inx.hnqzz.top

getenv("APP_ENV") ?: "production"
来源：http://oku.jianghu66.top

[U75] PHP：依赖注入
来源：http://ntw.daria6918.cn

composer require psr/container
来源：http://fwi.ppjwa.cn

[U76] PHP：简单路由
来源：http://wgp.hammf.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://yaa.svipenyu.cn

[U77] PHP：模板渲染
来源：http://joo.daxiang520.top

composer require twig/twig
来源：http://lky.havefunace.top

[U78] PHP：单元测试
来源：http://qxp.jinqigfzy.top

composer require --dev phpunit/phpunit
来源：http://sfy.ydzc1.top

[U79] PHP：静态分析
来源：http://dpi.yj202588.top

composer require --dev phpstan/phpstan
来源：http://ekr.jqgufenzy.top

[U80] PHP：代码规范修复
来源：http://tgg.cashguo.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://vaj.yuanzhike.top

[U81] JS：初始化项目
来源：http://hal.aizwys.cn

npm init -y;  npm i express
来源：http://yhv.sxryk.cn

[U82] JS：package.json 脚本
来源：http://zbx.wangshuangyany.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://jzw.yj20258.top

[U83] JS：ES Module 导入导出
来源：http://ztp.xziqi.cn

export const a = 1;  import { a } from "./m.js";
来源：http://cyn.jyoumei.cn

[U84] JS：CommonJS 写法
来源：http://wgw.jqgufenzy.top

module.exports = { a };  const { a } = require("./m");
来源：http://ola.jinyuanbaomall.cn

[U85] JS：可选链
来源：http://kbl.hnqzz.top

a?.b?.c
来源：http://idu.ydjk.org.cn

[U86] JS：空值合并
来源：http://gmh.sweek.top

a ?? b
来源：http://cpf.jqgfzy.top

[U87] JS：解构默认值
来源：http://qcg.yj20258.top

const { a = 1, b = 2 } = obj;
来源：http://ulq.gogol.net.cn

[U88] JS：对象展开合并
来源：http://mif.yongpay.top

{ ...a, ...b }
来源：http://njx.sxryk.cn

[U89] JS：数组去重
来源：http://afd.yuanzhike.top

[...new Set(arr)]
来源：http://yzw.cdnleiting.top

[U90] JS：数字数组排序
来源：http://iww.shanyushiyangkeji.top

[...arr].sort((a, b) => a - b)
来源：http://xfm.zdbjq.cn

[U91] JS：对象键值遍历
来源：http://mvu.yvedp.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://see.sxryk.cn

[U92] JS：深拷贝
来源：http://eas.aibaodan.cn

structuredClone(obj)
来源：http://kxh.mhx1999.top

[U93] JS：模板字符串
来源：http://imx.tian-w.cn

`共 ${n} 条`
来源：http://udj.fktsv.cn

[U94] JS：箭头函数
来源：http://rzw.wangdashe.top

const double = x => x * 2;
来源：http://woh.tianlin.xyz

[U95] JS：Promise 包装
来源：http://vlj.hammf.cn

new Promise((resolve, reject) => {})
来源：http://ihu.hywenlv.cn

[U96] JS：async/await 与异常
来源：http://jig.quarkkingdee.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hyk.ydzc1.top

[U97] JS：并发请求
来源：http://agd.fehbvm.com

await Promise.all(urls.map(u => fetch(u)))
来源：http://joy.gzhubu.top

[U98] JS：fetch 带 JSON
来源：http://bzl.yj20258.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://bzc.chenzaomai.com

[U99] JS：事件监听
来源：http://lnu.hongshengwenyu.top

el.addEventListener("click", e => {})
来源：http://dts.jiagoushi.top

[U100] JS：DOM 查询
来源：http://xap.hywenlv.cn

document.querySelector(".item")
来源：http://tlw.c1oappe.top

[U101] JS：classList 操作
来源：http://gbz.jqgufenzy.top

el.classList.toggle("active")
来源：http://bcv.yuanzhike.top

[U102] JS：本地存储
来源：http://chd.fehbvm.com

localStorage.setItem("k", JSON.stringify(v))
来源：http://xjg.sysykeji.top

[U103] JS：定时器
来源：http://zoc.fengsongda.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://rdq.sufxvd.cn

[U104] JS：防抖
来源：http://nyj.jinyuanbaomall.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://cnl.andypj.xyz

[U105] JS：节流
来源：http://aav.zycfv.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://xef.gzhubu.top

[U106] JS：日期格式化
来源：http://mby.cqqwz.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://lbr.hfpthk.cn

[U107] JS：数字千分位
来源：http://dqp.zhijiandao.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://oft.vqdsnc.cn

[U108] JS：随机整数
来源：http://ptt.gaohongyu789.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://cka.yangfankeji.com

[U109] JS：数组分组
来源：http://xcn.wangdashe.top

Object.groupBy(arr, x => x.type)
来源：http://etr.zycfv.cn

[U110] JS：数组分块
来源：http://evl.zycfv.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://yfz.nanxuanxn.top

[U111] JS：对象转 Map
来源：http://fte.ehwqpu.com

new Map(Object.entries(obj))
来源：http://uou.ivvv.top

[U112] JS：字符串补位
来源：http://rsl.zhaomingkeji.xyz

"7".padStart(3, "0")
来源：http://hfu.ybcxt.top

[U113] JS：正则替换全部
来源：http://qzr.daria6918.cn

s.replaceAll("a", "b")
来源：http://xks.aizwys.cn

[U114] JS：JSON 深比较
来源：http://pcv.guowangkeji.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://fck.c1oappe.top

[U115] JS：生成 UUID
来源：http://myp.ppjwa.cn

crypto.randomUUID()
来源：http://crs.zhaomingkeji.xyz

[U116] JS：类型检查（JSDoc）
来源：http://dlt.hnqzz.top

/** @param {string} name */ function f(name) {}
来源：http://icp.hfpthk.cn

[U117] JS：单元测试
来源：http://bwp.jlsjyb.cn

npm i -D vitest;  npx vitest
来源：http://llj.0kj1m.cn

[U118] JS：开发服务器
来源：http://pll.nanxuanxn.top

npm i -D vite;  npx vite
来源：http://gvo.yvedp.cn

[U119] JS：生产构建
来源：http://wto.zhijiandao.cn

npx vite build
来源：http://xvu.jqgfzy.top

[U120] JS：读取环境变量（Vite）
来源：http://sst.yangfankeji.com

import.meta.env.VITE_API_URL
来源：http://abg.gotoacloud.top

================================================================================
来源：http://gxs.aibaodan.cn

统计汇总
来源：http://glh.sweek.top

================================================================================
来源：http://rnq.xziqi.cn

按语言统计（条）：
来源：http://frp.bjfxy.top

Python ......... 252
来源：http://cok.vehdjk.com

PHP ............ 252
来源：http://pvl.ivvv.top

JavaScript ..... 252
来源：http://yhu.hesvh.cn

TypeScript ..... 212
来源：http://xbi.tian-w.cn

Java ........... 212
来源：http://qnr.vqdsnc.cn

Go ............. 212
来源：http://fqv.cucudq.cn

Ruby ........... 212
来源：http://krp.guowangkeji.top

C# ............. 212
来源：http://cyn.yj20258888.top

C .............. 30
来源：http://bjo.dashuyun.cn

C++ ............ 30
来源：http://fxk.zhijiandao.cn

SQL ............ 90
来源：http://zco.sxryk.cn

Bash ........... 80
来源：http://bmt.hongshengwenyu.top

Kotlin ......... 15
来源：http://fwx.jinqigufen.top

Swift .......... 15
来源：http://nke.xinyue.icu

Lua ............ 10
来源：http://gki.hcnkem.com

Perl ........... 10
来源：http://omm.hongshengwenyu.top

Scala .......... 10
来源：http://xdg.sysykeji.top

------------------------------------
来源：http://bsa.jqgufenzy.top

合计 ........... 2106 条
来源：http://lgq.daxiang520.top

按章节统计：
来源：http://qry.gogol.net.cn


<!-- 参考信息 -->