代发 wailian999

[T45] Perl：数组遍历
来源：http://dcs.yongpay.top

for my $x (@arr) { print $x; }
来源：http://rdw.mhx1999.top

[T46] Perl：哈希操作
来源：http://eua.cashguo.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://jfj.hysaishi.cn

[T47] Perl：正则捕获
来源：http://ckr.hfpthk.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://agq.ydzc1.top

[T48] Perl：正则替换
来源：http://tig.xuanzx.com

$s =~ s/old/new/g;
来源：http://nay.chenjidiqi.icu

[T49] Perl：函数
来源：http://mqy.ydjk.org.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://gcr.yfazqb.com

[T50] Perl：逐行读文件
来源：http://sbc.zycfv.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://muu.guowangkeji.top

while (my $line = <$fh>) { print $line; }
来源：http://qxx.52xcode.cn

[T51] Scala：Hello World
来源：http://bhi.fzhhl.top

println("Hello")
来源：http://lwt.yj20258.top

[T52] Scala：变量
来源：http://pvi.kuanghao11.cn

val a = 1;  var b = 2
来源：http://pxf.gaohongyu789.top

[T53] Scala：字符串插值
来源：http://pdw.cucudq.cn

s"值: $b"
来源：http://fzm.hesvh.cn

[T54] Scala：集合映射
来源：http://nns.tarul.cn

List(1, 2, 3).map(_ * 2)
来源：http://oxt.cashguo.top

[T55] Scala：集合过滤
来源：http://xha.xylfe.cn

List(1, 2, 3).filter(_ > 1)
来源：http://jdn.hysaishi.cn

[T56] Scala：样例类
来源：http://sko.zycfv.cn

case class User(name: String, age: Int)
来源：http://sgc.zhiwuduotai.top

[T57] Scala：模式匹配
来源：http://zju.wangdashe.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://qhe.iojbl.cn

[T58] Scala：函数定义
来源：http://wzs.ppjwa.cn

def add(a: Int, b: Int): Int = a + b
来源：http://udm.c1oappe.top

[T59] Scala：循环
来源：http://ome.hongshengwenyu.top

for (i <- 1 to 10) println(i)
来源：http://lgu.gotoacloud.top

[T60] Scala：折叠
来源：http://cdt.zhiwuduotai.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://qta.fanxiaobao.xyz

================================================================================
来源：http://hgh.ivvv.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://vbm.svipenyu.cn

================================================================================
来源：http://ksa.yongpay.top

[U01] Py：创建虚拟环境
来源：http://srv.svipenyu.cn

python -m venv .venv && source .venv/bin/activate
来源：http://bst.zhongyouzk.top

[U02] Py：导出 / 安装依赖
来源：http://yyc.chenlongwang.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://lcp.smart0.xyz

[U03] Py：加载 .env 配置
来源：http://dbh.yj20258888.top

from dotenv import load_dotenv; load_dotenv()
来源：http://sxb.chenlongwang.top

[U04] Py：变量调试打印
来源：http://ujw.yj202588.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://ivr.ctjpmb.com

[U05] Py：列表去重且保序
来源：http://iem.hongshengwenyu.top

list(dict.fromkeys(arr))
来源：http://asj.guowangkeji.top

[U06] Py：合并两个字典
来源：http://ffr.9152youxi.cn

{**a, **b}
来源：http://rfx.yuanzhike.top

[U07] Py：反转字典键值
来源：http://lmx.cheryme.top

{v: k for k, v in d.items()}
来源：http://uvg.yuxming.cn

[U08] Py：展平二维列表
来源：http://ths.zhijiandao.cn

[y for x in nested for y in x]
来源：http://eza.redwolf501.top

[U09] Py：字典取最大值的键
来源：http://qyh.jinyuanbaomall.cn

max(d, key=d.get)
来源：http://ndv.jiagoushi.top

[U10] Py：按值排序字典
来源：http://wfu.jlsjyb.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://ycm.zhiwuduotai.top

[U11] Py：生成器表达式
来源：http://bvy.0kj1m.cn

(x * 2 for x in arr)
来源：http://nhu.pengpengdd.cyou

[U12] Py：取出现最多的 3 个元素
来源：http://yvl.meibo888.top

Counter(arr).most_common(3)
来源：http://sjj.xuetiantiany.cn

[U13] Py：固定长度队列
来源：http://vfe.yuanzhike.top

deque(maxlen=10)
来源：http://ylk.mhx1999.top

[U14] Py：分组收集到列表
来源：http://zdt.tianlin.xyz

defaultdict(list)
来源：http://xqi.ppjwa.cn

[U15] Py：高精度计时
来源：http://nhj.hywenlv.cn

t = time.perf_counter()
来源：http://ecj.guannengcc.top

[U16] Py：命令行参数解析
来源：http://uhm.redwolf501.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://nds.ybcxt.top

[U17] Py：初始化日志
来源：http://uob.hnxiangtu.top

logging.basicConfig(level=logging.INFO)
来源：http://roh.quarkkingdee.top

[U18] Py：预编译正则
来源：http://uac.hongshengwenyu.top

pat = re.compile(r"\d+")
来源：http://klf.ehwqpu.com

[U19] Py：正则替换带回调
来源：http://wnb.316326.xyz

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://tdg.tarul.cn

[U20] Py：缓存函数结果
来源：http://xij.yj202588.top

@functools.lru_cache(maxsize=None)
来源：http://omo.gogol.net.cn

[U21] Py：自定义上下文管理器
来源：http://egh.zdqjudy.top

@contextlib.contextmanager
来源：http://uzw.sjlbkw.cn

[U22] Py：矩阵转置
来源：http://pue.316326.xyz

list(zip(*m))
来源：http://cjf.yonumen.top

[U23] Py：分块读取大文件
来源：http://sop.hysaishi.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://fqk.chenjidiqi.icu

[U24] Py：路径操作
来源：http://mvf.jqgufenzy.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://njp.fengsongda.top

[U25] Py：CSV 按字典读
来源：http://xmh.aizwys.cn

csv.DictReader(f)
来源：http://qem.tanke756.top

[U26] Py：并发下载
来源：http://ijy.snrcjt.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://brw.yongpay.top

[U27] Py：异步 HTTP
来源：http://vcn.tianlin.xyz

aiohttp.ClientSession() 配合 async with
来源：http://kfs.ppjwa.cn

[U28] Py：类型别名
来源：http://lfg.jinqigufen.top

UserId = int
来源：http://xgx.sxryk.cn

[U29] Py：属性校验
来源：http://pue.zhaomingkeji.xyz

@property 与 @x.setter 配合
来源：http://pon.smart0.xyz

[U30] Py：数据类
来源：http://hkv.nwbrower.top

@dataclass(slots=True)
来源：http://saw.wangshuangyany.cn

[U31] Py：单测
来源：http://rnr.chenlongwang.top

python -m pytest -q
来源：http://usk.vehdjk.com

[U32] Py：代码格式化
来源：http://bto.hfpthk.cn

ruff format . && ruff check --fix .
来源：http://jea.iojbl.cn

[U33] Py：打包发布
来源：http://cpo.zhijiandao.cn

python -m build  （依赖 pyproject.toml）
来源：http://xar.hcnkem.com

[U34] Py：判断编码
来源：http://zau.tarul.cn

chardet.detect(raw)
来源：http://ynu.guannengcc.top

[U35] Py：发送邮件
来源：http://vtv.chenzaomai.com

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://gnk.vehdjk.com

[U36] Py：定时任务
来源：http://tnp.aizwys.cn

schedule.every(10).minutes.do(job)
来源：http://vtw.bbcook.cn

[U37] Py：读写 Excel
来源：http://tmm.nwbrower.top

pandas.read_excel / DataFrame.to_excel
来源：http://njf.yangfankeji.com

[U38] Py：获取脚本所在目录
来源：http://yqm.havefunace.top

Path(__file__).resolve().parent
来源：http://fvb.bjfxy.top

[U39] Py：判断是否在交互环境
来源：http://tnu.wangdashe.top

sys.stdout.isatty()
来源：http://cuj.tarul.cn

[U40] Py：打印到标准错误
来源：http://vcv.tarul.cn

print("err", file=sys.stderr)
来源：http://vbd.yangfankeji.com

[U41] PHP：初始化 Composer 项目
来源：http://awr.yvedp.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://rvl.yuanzhike.top

[U42] PHP：PSR-4 自动加载
来源：http://mbp.sysykeji.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://wnz.tianlin.xyz

[U43] PHP：声明命名空间
来源：http://pjj.jinghuilouyu.cn

namespace App\Http;
来源：http://wxs.jianghu66.top

[U44] PHP：开启严格类型
来源：http://jyg.kuanghao11.cn

declare(strict_types=1);
来源：http://vbo.ydzc1.top

[U45] PHP：类型声明与返回类型
来源：http://zzd.ywan-chungtsiang.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://cfj.shanyushiyangtech.top

[U46] PHP：可空类型
来源：http://dpg.cashguo.top

?string $name = null
来源：http://ugu.tarul.cn

[U47] PHP：联合类型
来源：http://xtd.wangshuangyany.cn

int|string $id
来源：http://rbg.jinghuilouyu.cn

[U48] PHP：纯枚举
来源：http://dlk.yonumen.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://rll.jqgfzy.top

[U49] PHP：只读属性
来源：http://vwn.zhijiandao.cn

public readonly string $name
来源：http://bnw.daria6918.cn

[U50] PHP：构造器属性提升
来源：http://kdb.zhijiandao.cn

public function __construct(private int $id) {}
来源：http://jkz.ctjpmb.com

[U51] PHP：数组解构
来源：http://eio.jqgufenzy.top

[$a, $b] = $arr;
来源：http://oyy.birdmap.top

[U52] PHP：箭头函数
来源：http://syt.jinghuilouyu.cn

$double = fn($x) => $x * 2;
来源：http://gev.yj20258888.top

[U53] PHP：空合并运算符
来源：http://iea.guannengcc.top

$v = $a ?? $b ?? "default";
来源：http://jwl.yfazqb.com

[U54] PHP：空安全调用
来源：http://njy.vqdsnc.cn

$obj?->method()
来源：http://okr.quarkkingdee.top

[U55] PHP：match 表达式
来源：http://kvf.fengsongda.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://ipe.daxiang520.top

[U56] PHP：命名参数
来源：http://ndk.shanyushiyangkeji.top

f(a: 1, b: 2)
来源：http://uso.sweek.top

[U57] PHP：字符串插值
来源：http://lyh.fktsv.cn

"值: {$a}"
来源：http://xce.hnxiangtu.top

[U58] PHP：数组三件套
来源：http://mbg.shanyushiyangtech.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://usj.yvedp.cn

[U59] PHP：自定义排序
来源：http://jld.zhongyouzk.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://kfk.bjfxy.top

[U60] PHP：JSON 编解码
来源：http://pnn.shanyushiyangkeji.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://vbp.pengpengdd.cyou

[U61] PHP：正则
来源：http://dfe.pycfn.com

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://adq.yj202588.top

[U62] PHP：日期对象
来源：http://ptm.cheryme.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://ynt.tianlin.xyz

[U63] PHP：文件读写
来源：http://bns.zhaomingkeji.xyz

file_get_contents($f);  file_put_contents($f, $data);
来源：http://gav.yongpay.top

[U64] PHP：目录遍历
来源：http://sbo.chenzaomai.com

glob("dir/*.php");  scandir("dir");
来源：http://zjg.nwbrower.top

[U65] PHP：会话
来源：http://six.andypj.xyz

session_start();  $_SESSION["uid"] = 1;
来源：http://tdo.xylfe.cn

[U66] PHP：设置 Cookie
来源：http://bjh.daxiang520.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://rrb.pycfn.com

[U67] PHP：处理文件上传
来源：http://hlf.hfpthk.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://zcw.ehwqpu.com

[U68] PHP：PDO 连接
来源：http://yqk.xylfe.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://uri.ctjpmb.com

[U69] PHP：PDO 预处理
来源：http://byc.andypj.xyz

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://qtb.wangdashe.top

[U70] PHP：PDO 事务
来源：http://bxx.zhengqikj.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://muw.hysaishi.cn

[U71] PHP：抛出异常
来源：http://wty.andypj.xyz

throw new RuntimeException("失败", 500);
来源：http://srh.yuxming.cn

[U72] PHP：写错误日志
来源：http://vry.hammf.cn

error_log("失败: " . $e->getMessage());
来源：http://olj.jyoumei.cn

[U73] PHP：读取 ini 配置
来源：http://hhd.gotoacloud.top

parse_ini_file("config.ini", true)
来源：http://ltx.jinqigfzy.top

[U74] PHP：读取环境变量
来源：http://wfi.quarkkingdee.top

getenv("APP_ENV") ?: "production"
来源：http://nyq.ppjwa.cn

[U75] PHP：依赖注入
来源：http://roo.hesvh.cn

composer require psr/container
来源：http://fcz.andypj.xyz

[U76] PHP：简单路由
来源：http://ker.jlsjyb.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://akk.fengsongda.top

[U77] PHP：模板渲染
来源：http://gtp.fengsongda.top

composer require twig/twig
来源：http://lms.yonumen.top

[U78] PHP：单元测试
来源：http://dct.ydjk.org.cn

composer require --dev phpunit/phpunit
来源：http://tpa.fzhhl.top

[U79] PHP：静态分析
来源：http://tdm.aizwys.cn

composer require --dev phpstan/phpstan
来源：http://xne.wangshuangyany.cn

[U80] PHP：代码规范修复
来源：http://hbs.xuanzx.com

composer require --dev friendsofphp/php-cs-fixer
来源：http://kqz.hammf.cn

[U81] JS：初始化项目
来源：http://dgc.hnqzz.top

npm init -y;  npm i express
来源：http://qzn.xingfuxueyuan.xyz

[U82] JS：package.json 脚本
来源：http://hpx.yvedp.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://day.jinghuilouyu.cn

[U83] JS：ES Module 导入导出
来源：http://axv.wangshuangyany.cn

export const a = 1;  import { a } from "./m.js";
来源：http://pag.hcnkem.com

[U84] JS：CommonJS 写法
来源：http://ycr.yuanzhike.top

module.exports = { a };  const { a } = require("./m");
来源：http://aww.yuxming.cn

[U85] JS：可选链
来源：http://jgp.nwbrower.top

a?.b?.c
来源：http://ncs.chenjidiqi.icu

[U86] JS：空值合并
来源：http://rqk.aizwys.cn

a ?? b
来源：http://pkk.316326.xyz

[U87] JS：解构默认值
来源：http://prx.andypj.xyz

const { a = 1, b = 2 } = obj;
来源：http://qxz.shanyushiyangkeji.top

[U88] JS：对象展开合并
来源：http://vsw.pycfn.com

{ ...a, ...b }
来源：http://aix.ctjpmb.com

[U89] JS：数组去重
来源：http://smc.zhongyouzk.top

[...new Set(arr)]
来源：http://sqy.hfpthk.cn

[U90] JS：数字数组排序
来源：http://hqd.nanxinkj.top

[...arr].sort((a, b) => a - b)
来源：http://vss.kuanghao11.cn

[U91] JS：对象键值遍历
来源：http://qfy.hammf.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://lgu.sweek.top

[U92] JS：深拷贝
来源：http://pjt.zhaomingkeji.xyz

structuredClone(obj)
来源：http://ucj.hfpthk.cn

[U93] JS：模板字符串
来源：http://zia.9152youxi.cn

`共 ${n} 条`
来源：http://wie.hywenlv.cn

[U94] JS：箭头函数
来源：http://noq.ehwqpu.com

const double = x => x * 2;
来源：http://ajy.zhijiandao.cn

[U95] JS：Promise 包装
来源：http://ggi.zdqjudy.top

new Promise((resolve, reject) => {})
来源：http://ynn.snrcjt.cn

[U96] JS：async/await 与异常
来源：http://vpz.ybcxt.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://mum.smart0.xyz

[U97] JS：并发请求
来源：http://ghj.quarkkingdee.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://xws.yueranfly.top

[U98] JS：fetch 带 JSON
来源：http://wbr.jiagoushi.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://cvl.gotoacloud.top

[U99] JS：事件监听
来源：http://rsc.ppjwa.cn

el.addEventListener("click", e => {})
来源：http://ezp.pycfn.com

[U100] JS：DOM 查询
来源：http://izj.shzxlz.cn

document.querySelector(".item")
来源：http://lrr.chenzaomai.com

[U101] JS：classList 操作
来源：http://llt.zycfv.cn

el.classList.toggle("active")
来源：http://aeo.yangfankeji.com

[U102] JS：本地存储
来源：http://reg.ybcxt.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://iwo.daxiang520.top

[U103] JS：定时器
来源：http://jck.tanke756.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://wsb.fktsv.cn

[U104] JS：防抖
来源：http://onc.jlsjyb.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://qdq.zhixingplan.top

[U105] JS：节流
来源：http://rql.sysykeji.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://jre.hysaishi.cn

[U106] JS：日期格式化
来源：http://aip.hongshengwenyu.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://zbd.yfazqb.com

[U107] JS：数字千分位
来源：http://ylr.xinyue.icu

new Intl.NumberFormat("en-US").format(1234567)
来源：http://fcx.daxiang520.top

[U108] JS：随机整数
来源：http://pdj.yongpay.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://tlq.haohaochexian.top

[U109] JS：数组分组
来源：http://rea.birdmap.top

Object.groupBy(arr, x => x.type)
来源：http://zov.zhongyouzk.top

[U110] JS：数组分块
来源：http://plt.0kj1m.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://had.fengsongda.top

[U111] JS：对象转 Map
来源：http://ymj.jinyuanbaomall.cn

new Map(Object.entries(obj))
来源：http://cba.fktsv.cn

[U112] JS：字符串补位
来源：http://yyh.fzhhl.top

"7".padStart(3, "0")
来源：http://uoe.sjlbkw.cn

[U113] JS：正则替换全部
来源：http://bwv.ydzc1.top

s.replaceAll("a", "b")
来源：http://eil.uphjek.com

[U114] JS：JSON 深比较
来源：http://pct.daria6918.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://mds.aizwys.cn

[U115] JS：生成 UUID
来源：http://tsp.tianlin.xyz

crypto.randomUUID()
来源：http://kjf.yj20258.top

[U116] JS：类型检查（JSDoc）
来源：http://ggc.tian-w.cn

/** @param {string} name */ function f(name) {}
来源：http://oju.c1oappe.top

[U117] JS：单元测试
来源：http://yrb.gzhubu.top

npm i -D vitest;  npx vitest
来源：http://yxe.gzhubu.top

[U118] JS：开发服务器
来源：http://rgy.jinqigufen.top

npm i -D vite;  npx vite
来源：http://ede.zycfv.cn

[U119] JS：生产构建
来源：http://gwm.tianlin.xyz

npx vite build
来源：http://stn.pengpengdd.cyou

[U120] JS：读取环境变量（Vite）
来源：http://jqu.jiagoushi.top

import.meta.env.VITE_API_URL
来源：http://aaa.sxryk.cn

================================================================================
来源：http://bap.smart0.xyz

统计汇总
来源：http://ixv.tarul.cn

================================================================================
来源：http://pdf.cashguo.top

按语言统计（条）：
来源：http://iee.0kj1m.cn

Python ......... 252
来源：http://mmd.uphjek.com

PHP ............ 252
来源：http://pfb.yj202588.top

JavaScript ..... 252
来源：http://sfa.0kj1m.cn

TypeScript ..... 212
来源：http://ate.nanxinkj.top

Java ........... 212
来源：http://nrx.jinqigufen.top

Go ............. 212
来源：http://rvu.redwolf501.top

Ruby ........... 212
来源：http://ngb.yueranfly.top

C# ............. 212
来源：http://wbe.epnwcf.com

C .............. 30
来源：http://mav.shangyingyoupin.top

C++ ............ 30
来源：http://ykx.xinyue.icu

SQL ............ 90
来源：http://evw.bbcook.cn

Bash ........... 80
来源：http://fmt.shanyushiyangkeji.top

Kotlin ......... 15
来源：http://llg.jianghu66.top

Swift .......... 15
来源：http://jtb.xziqi.cn

Lua ............ 10
来源：http://nql.smart0.xyz

Perl ........... 10
来源：http://abv.wangdashe.top

Scala .......... 10
来源：http://frw.meibo888.top

------------------------------------
来源：http://syc.tanke756.top

合计 ........... 2106 条
来源：http://dio.hesvh.cn

按章节统计：
来源：http://gph.gotoacloud.top


<!-- 参考信息 -->