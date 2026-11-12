代发 wailian999

[T37] Lua：字符串拼接
来源：http://odt.vehdjk.com

"a" .. "b"
来源：http://pse.hammf.cn

[T38] Lua：条件
来源：http://hoi.9152youxi.cn

if x > 0 then print("正") end
来源：http://ebl.uphjek.com

[T39] Lua：模式匹配
来源：http://oyh.fanxiaobao.xyz

string.find(s, "%d+")
来源：http://uei.hfpthk.cn

[T40] Lua：元表
来源：http://cfb.bbcook.cn

setmetatable({}, { __index = base })
来源：http://tzf.jinqigfzy.top

[T41] Perl：Hello World
来源：http://fyz.ppjwa.cn

print "Hello\n";
来源：http://okm.xuanzx.com

[T42] Perl：变量类型
来源：http://nqt.haohaochexian.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://kfm.uphjek.com

[T43] Perl：字符串插值
来源：http://zho.52xcode.cn

"值: $a"
来源：http://ncw.haohaochexian.top

[T44] Perl：条件
来源：http://cih.mhx1999.top

if ($a > 0) { print "正"; }
来源：http://pdt.fktsv.cn

[T45] Perl：数组遍历
来源：http://zrq.yfazqb.com

for my $x (@arr) { print $x; }
来源：http://ndy.zdqjudy.top

[T46] Perl：哈希操作
来源：http://qzc.shanyushiyangkeji.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://rnz.9152youxi.cn

[T47] Perl：正则捕获
来源：http://ski.aibaodan.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://jdv.sufxvd.cn

[T48] Perl：正则替换
来源：http://fon.yj20258888.top

$s =~ s/old/new/g;
来源：http://tcq.c1oappe.top

[T49] Perl：函数
来源：http://ery.316326.xyz

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hxm.ppjwa.cn

[T50] Perl：逐行读文件
来源：http://zsk.shanyushiyangkeji.top

open my $fh, "<", "a.txt" or die $!;
来源：http://hup.yuxming.cn

while (my $line = <$fh>) { print $line; }
来源：http://kaq.havefunace.top

[T51] Scala：Hello World
来源：http://oaz.yanxiufei.cn

println("Hello")
来源：http://ahs.nanxinkj.top

[T52] Scala：变量
来源：http://mqu.ehwqpu.com

val a = 1;  var b = 2
来源：http://otm.9152youxi.cn

[T53] Scala：字符串插值
来源：http://sqa.hcnkem.com

s"值: $b"
来源：http://vqj.zhengqikj.top

[T54] Scala：集合映射
来源：http://aha.yuanzhike.top

List(1, 2, 3).map(_ * 2)
来源：http://sbr.jqgufenzy.top

[T55] Scala：集合过滤
来源：http://lwt.sufxvd.cn

List(1, 2, 3).filter(_ > 1)
来源：http://aie.cheryme.top

[T56] Scala：样例类
来源：http://idy.yanxiufei.cn

case class User(name: String, age: Int)
来源：http://min.zhaomingkeji.xyz

[T57] Scala：模式匹配
来源：http://yqb.vqdsnc.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://xuw.hnqzz.top

[T58] Scala：函数定义
来源：http://ogt.yfazqb.com

def add(a: Int, b: Int): Int = a + b
来源：http://ocg.xziqi.cn

[T59] Scala：循环
来源：http://caa.hysaishi.cn

for (i <- 1 to 10) println(i)
来源：http://ppl.yonumen.top

[T60] Scala：折叠
来源：http://wpw.vehdjk.com

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://pqs.zdbjq.cn

================================================================================
来源：http://sik.andypj.xyz

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://gns.hcnkem.com

================================================================================
来源：http://xct.ehwqpu.com

[U01] Py：创建虚拟环境
来源：http://hek.ydjk.org.cn

python -m venv .venv && source .venv/bin/activate
来源：http://vil.zycfv.cn

[U02] Py：导出 / 安装依赖
来源：http://dre.tanke756.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://irf.jiagoushi.top

[U03] Py：加载 .env 配置
来源：http://wxs.kuanghao11.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://xnd.quarkkingdee.top

[U04] Py：变量调试打印
来源：http://scw.bbcook.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://tpw.jinghuilouyu.cn

[U05] Py：列表去重且保序
来源：http://eqa.sysykeji.top

list(dict.fromkeys(arr))
来源：http://yjk.uphjek.com

[U06] Py：合并两个字典
来源：http://ryz.sxryk.cn

{**a, **b}
来源：http://gms.hywenlv.cn

[U07] Py：反转字典键值
来源：http://wnp.hysaishi.cn

{v: k for k, v in d.items()}
来源：http://vsz.yfazqb.com

[U08] Py：展平二维列表
来源：http://aiv.xylfe.cn

[y for x in nested for y in x]
来源：http://cyk.zdbjq.cn

[U09] Py：字典取最大值的键
来源：http://wct.pengpengdd.cyou

max(d, key=d.get)
来源：http://apq.chenlongwang.top

[U10] Py：按值排序字典
来源：http://xnl.fanxiaobao.xyz

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://opk.fzhhl.top

[U11] Py：生成器表达式
来源：http://uzu.fanxiaobao.xyz

(x * 2 for x in arr)
来源：http://zrq.hnqzz.top

[U12] Py：取出现最多的 3 个元素
来源：http://snp.havefunace.top

Counter(arr).most_common(3)
来源：http://fjy.sweek.top

[U13] Py：固定长度队列
来源：http://nck.hnxiangtu.top

deque(maxlen=10)
来源：http://llj.xingfuxueyuan.xyz

[U14] Py：分组收集到列表
来源：http://hcp.fengsongda.top

defaultdict(list)
来源：http://iaq.fzhhl.top

[U15] Py：高精度计时
来源：http://yqx.jiagoushi.top

t = time.perf_counter()
来源：http://toc.nanxinkj.top

[U16] Py：命令行参数解析
来源：http://qca.xingfuxueyuan.xyz

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://jnt.chenlongwang.top

[U17] Py：初始化日志
来源：http://wxe.zhiwuduotai.top

logging.basicConfig(level=logging.INFO)
来源：http://fry.ctjpmb.com

[U18] Py：预编译正则
来源：http://hzo.zhixingplan.top

pat = re.compile(r"\d+")
来源：http://clx.chenzaomai.com

[U19] Py：正则替换带回调
来源：http://dqz.vqdsnc.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://txf.aibaodan.cn

[U20] Py：缓存函数结果
来源：http://pys.yueranfly.top

@functools.lru_cache(maxsize=None)
来源：http://hov.guowangkeji.top

[U21] Py：自定义上下文管理器
来源：http://dum.sweek.top

@contextlib.contextmanager
来源：http://cro.pengpengdd.cyou

[U22] Py：矩阵转置
来源：http://ckm.smart0.xyz

list(zip(*m))
来源：http://ntw.tanke756.top

[U23] Py：分块读取大文件
来源：http://cgp.yuxming.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://xyu.mhx1999.top

[U24] Py：路径操作
来源：http://gcv.tarul.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://drd.jyoumei.cn

[U25] Py：CSV 按字典读
来源：http://ihz.kuanghao11.cn

csv.DictReader(f)
来源：http://ker.quarkkingdee.top

[U26] Py：并发下载
来源：http://rsl.xuetiantiany.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://iwd.zhaomingkeji.xyz

[U27] Py：异步 HTTP
来源：http://vsv.hysaishi.cn

aiohttp.ClientSession() 配合 async with
来源：http://orh.tianlin.xyz

[U28] Py：类型别名
来源：http://kkd.yangfankeji.com

UserId = int
来源：http://yaq.ybcxt.top

[U29] Py：属性校验
来源：http://vlm.jiagoushi.top

@property 与 @x.setter 配合
来源：http://duv.shanyushiyangkeji.top

[U30] Py：数据类
来源：http://mhs.tian-w.cn

@dataclass(slots=True)
来源：http://eob.daxiang520.top

[U31] Py：单测
来源：http://mni.52xcode.cn

python -m pytest -q
来源：http://tfs.zhixingplan.top

[U32] Py：代码格式化
来源：http://lbx.ctjpmb.com

ruff format . && ruff check --fix .
来源：http://rrk.c1oappe.top

[U33] Py：打包发布
来源：http://osj.yuanzhike.top

python -m build  （依赖 pyproject.toml）
来源：http://ash.nanxinkj.top

[U34] Py：判断编码
来源：http://xgb.fanxiaobao.xyz

chardet.detect(raw)
来源：http://soc.ppjwa.cn

[U35] Py：发送邮件
来源：http://bwp.xylfe.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://fxa.meibo888.top

[U36] Py：定时任务
来源：http://onj.wangshuangyany.cn

schedule.every(10).minutes.do(job)
来源：http://rqv.dashuyun.cn

[U37] Py：读写 Excel
来源：http://zvm.yfazqb.com

pandas.read_excel / DataFrame.to_excel
来源：http://qgd.zhijiandao.cn

[U38] Py：获取脚本所在目录
来源：http://nzg.jinghuilouyu.cn

Path(__file__).resolve().parent
来源：http://jry.nanxinkj.top

[U39] Py：判断是否在交互环境
来源：http://amo.jinqigufen.top

sys.stdout.isatty()
来源：http://mhd.yangfankeji.com

[U40] Py：打印到标准错误
来源：http://bbk.shzxlz.cn

print("err", file=sys.stderr)
来源：http://uec.ppjwa.cn

[U41] PHP：初始化 Composer 项目
来源：http://sgm.bbcook.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://dxb.andypj.xyz

[U42] PHP：PSR-4 自动加载
来源：http://jhy.shangyingyoupin.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://prp.yangfankeji.com

[U43] PHP：声明命名空间
来源：http://lqz.haohaochexian.top

namespace App\Http;
来源：http://klh.ctjpmb.com

[U44] PHP：开启严格类型
来源：http://ehw.316326.xyz

declare(strict_types=1);
来源：http://bhg.epnwcf.com

[U45] PHP：类型声明与返回类型
来源：http://fhi.gogol.net.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://urd.guowangkeji.top

[U46] PHP：可空类型
来源：http://smf.jiagoushi.top

?string $name = null
来源：http://pmp.9152youxi.cn

[U47] PHP：联合类型
来源：http://fgg.yfazqb.com

int|string $id
来源：http://vob.ybcxt.top

[U48] PHP：纯枚举
来源：http://iqz.sysykeji.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://zhf.zhoulong.xyz

[U49] PHP：只读属性
来源：http://mak.9152youxi.cn

public readonly string $name
来源：http://qnm.zdbjq.cn

[U50] PHP：构造器属性提升
来源：http://ibg.gzhubu.top

public function __construct(private int $id) {}
来源：http://wxz.yonumen.top

[U51] PHP：数组解构
来源：http://ybm.zycfv.cn

[$a, $b] = $arr;
来源：http://nbg.zhiwuduotai.top

[U52] PHP：箭头函数
来源：http://ltj.aibaodan.cn

$double = fn($x) => $x * 2;
来源：http://yrz.yvedp.cn

[U53] PHP：空合并运算符
来源：http://ntw.jinqigfzy.top

$v = $a ?? $b ?? "default";
来源：http://lsu.xylfe.cn

[U54] PHP：空安全调用
来源：http://moe.guowangkeji.top

$obj?->method()
来源：http://njf.zdqjudy.top

[U55] PHP：match 表达式
来源：http://gms.zhaomingkeji.xyz

$s = match($x) { 1 => "一", default => "其他" };
来源：http://alo.bjfxy.top

[U56] PHP：命名参数
来源：http://kxh.sxryk.cn

f(a: 1, b: 2)
来源：http://fwc.jiagoushi.top

[U57] PHP：字符串插值
来源：http://sfo.shanyushiyangkeji.top

"值: {$a}"
来源：http://txr.yj20258.top

[U58] PHP：数组三件套
来源：http://eda.316326.xyz

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://rme.yongpay.top

[U59] PHP：自定义排序
来源：http://wxp.tarul.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://sqz.gaohongyu789.top

[U60] PHP：JSON 编解码
来源：http://txb.shangyingyoupin.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://yfk.yj202588.top

[U61] PHP：正则
来源：http://uss.316326.xyz

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://bsz.hongshengwenyu.top

[U62] PHP：日期对象
来源：http://mvu.hammf.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://mnf.zhijiandao.cn

[U63] PHP：文件读写
来源：http://iwe.chenlongwang.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://exg.wangshuangyany.cn

[U64] PHP：目录遍历
来源：http://lie.zdqjudy.top

glob("dir/*.php");  scandir("dir");
来源：http://sxq.tarul.cn

[U65] PHP：会话
来源：http://uyz.guannengcc.top

session_start();  $_SESSION["uid"] = 1;
来源：http://pbn.zycfv.cn

[U66] PHP：设置 Cookie
来源：http://gxk.hnxiangtu.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://rsv.haohaochexian.top

[U67] PHP：处理文件上传
来源：http://upl.sweek.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://dnp.jiagoushi.top

[U68] PHP：PDO 连接
来源：http://obk.jianghu66.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://ikp.tianlin.xyz

[U69] PHP：PDO 预处理
来源：http://avg.zhoulong.xyz

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://yjs.andypj.xyz

[U70] PHP：PDO 事务
来源：http://uck.havefunace.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://arn.shuidangran.top

[U71] PHP：抛出异常
来源：http://fwg.tarul.cn

throw new RuntimeException("失败", 500);
来源：http://ftz.hnxiangtu.top

[U72] PHP：写错误日志
来源：http://lmp.yonumen.top

error_log("失败: " . $e->getMessage());
来源：http://egd.zhaomingkeji.xyz

[U73] PHP：读取 ini 配置
来源：http://qth.jqgfzy.top

parse_ini_file("config.ini", true)
来源：http://bnk.havefunace.top

[U74] PHP：读取环境变量
来源：http://zmr.xuetiantiany.cn

getenv("APP_ENV") ?: "production"
来源：http://dky.meibo888.top

[U75] PHP：依赖注入
来源：http://uax.haohaochexian.top

composer require psr/container
来源：http://wzr.aizwys.cn

[U76] PHP：简单路由
来源：http://ykk.c1oappe.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://evq.tian-w.cn

[U77] PHP：模板渲染
来源：http://ekb.sxryk.cn

composer require twig/twig
来源：http://hif.ehwqpu.com

[U78] PHP：单元测试
来源：http://thp.sxryk.cn

composer require --dev phpunit/phpunit
来源：http://ivw.hcnkem.com

[U79] PHP：静态分析
来源：http://wyi.shangyingyoupin.top

composer require --dev phpstan/phpstan
来源：http://lrl.zhoulong.xyz

[U80] PHP：代码规范修复
来源：http://lnf.sufxvd.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://hea.jianghu66.top

[U81] JS：初始化项目
来源：http://czw.zhaomingkeji.xyz

npm init -y;  npm i express
来源：http://iqi.zhixingplan.top

[U82] JS：package.json 脚本
来源：http://vmm.chenjidiqi.icu

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://pnt.c1oappe.top

[U83] JS：ES Module 导入导出
来源：http://ijh.quarkkingdee.top

export const a = 1;  import { a } from "./m.js";
来源：http://exs.kuanghao11.cn

[U84] JS：CommonJS 写法
来源：http://wrh.birdmap.top

module.exports = { a };  const { a } = require("./m");
来源：http://zzq.ywan-chungtsiang.top

[U85] JS：可选链
来源：http://cnq.jinqigufen.top

a?.b?.c
来源：http://prw.yj20258888.top

[U86] JS：空值合并
来源：http://pdp.yj20258.top

a ?? b
来源：http://mnw.redwolf501.top

[U87] JS：解构默认值
来源：http://dda.aibaodan.cn

const { a = 1, b = 2 } = obj;
来源：http://qzi.yonumen.top

[U88] JS：对象展开合并
来源：http://grn.zhongyouzk.top

{ ...a, ...b }
来源：http://ewl.jqgfzy.top

[U89] JS：数组去重
来源：http://lel.aizwys.cn

[...new Set(arr)]
来源：http://apj.cucudq.cn

[U90] JS：数字数组排序
来源：http://jhw.chenzaomai.com

[...arr].sort((a, b) => a - b)
来源：http://ikh.nanxinkj.top

[U91] JS：对象键值遍历
来源：http://zel.hywenlv.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://ivb.vqdsnc.cn

[U92] JS：深拷贝
来源：http://jsp.vqdsnc.cn

structuredClone(obj)
来源：http://wuz.feifeiyinyue.top

[U93] JS：模板字符串
来源：http://xyd.9152youxi.cn

`共 ${n} 条`
来源：http://lue.sxryk.cn

[U94] JS：箭头函数
来源：http://jlz.cucudq.cn

const double = x => x * 2;
来源：http://sdm.316326.xyz

[U95] JS：Promise 包装
来源：http://agl.epnwcf.com

new Promise((resolve, reject) => {})
来源：http://qdi.hammf.cn

[U96] JS：async/await 与异常
来源：http://qvq.cheryme.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://jwo.tarul.cn

[U97] JS：并发请求
来源：http://xer.chenjidiqi.icu

await Promise.all(urls.map(u => fetch(u)))
来源：http://uqa.tarul.cn

[U98] JS：fetch 带 JSON
来源：http://nxh.zhoulong.xyz

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://rcn.jqgfzy.top

[U99] JS：事件监听
来源：http://sbr.uphjek.com

el.addEventListener("click", e => {})
来源：http://goe.sjlbkw.cn

[U100] JS：DOM 查询
来源：http://gtc.epnwcf.com

document.querySelector(".item")
来源：http://afh.jlsjyb.cn

[U101] JS：classList 操作
来源：http://ybh.tarul.cn

el.classList.toggle("active")
来源：http://pma.hywenlv.cn

[U102] JS：本地存储
来源：http://sjh.tianlin.xyz

localStorage.setItem("k", JSON.stringify(v))
来源：http://ubc.hnxiangtu.top

[U103] JS：定时器
来源：http://itu.epnwcf.com

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://csd.jqgfzy.top

[U104] JS：防抖
来源：http://nwn.zhongyouzk.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hdi.xziqi.cn

[U105] JS：节流
来源：http://cue.quarkkingdee.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://ixv.zycfv.cn

[U106] JS：日期格式化
来源：http://xsf.xziqi.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://cvn.hfpthk.cn

[U107] JS：数字千分位
来源：http://qxo.meibo888.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://zgq.yfazqb.com

[U108] JS：随机整数
来源：http://ufu.chenlongwang.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://gga.zhengqikj.top

[U109] JS：数组分组
来源：http://lgk.gotoacloud.top

Object.groupBy(arr, x => x.type)
来源：http://zoc.0kj1m.cn

[U110] JS：数组分块
来源：http://gcb.daria6918.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://nsd.pengpengdd.cyou

[U111] JS：对象转 Map
来源：http://yfq.yangfankeji.com

new Map(Object.entries(obj))
来源：http://dln.hfpthk.cn

[U112] JS：字符串补位
来源：http://cjf.ydzc1.top

"7".padStart(3, "0")
来源：http://uqr.jqgufenzy.top

[U113] JS：正则替换全部
来源：http://ezh.52xcode.cn

s.replaceAll("a", "b")
来源：http://ebk.sweek.top

[U114] JS：JSON 深比较
来源：http://mvf.xingfuxueyuan.xyz

JSON.stringify(a) === JSON.stringify(b)
来源：http://gzo.yfazqb.com

[U115] JS：生成 UUID
来源：http://mds.fanxiaobao.xyz

crypto.randomUUID()
来源：http://axi.fehbvm.com

[U116] JS：类型检查（JSDoc）
来源：http://qtm.jiagoushi.top

/** @param {string} name */ function f(name) {}
来源：http://uoz.xylfe.cn

[U117] JS：单元测试
来源：http://udj.yuanzhike.top

npm i -D vitest;  npx vitest
来源：http://twv.vehdjk.com

[U118] JS：开发服务器
来源：http://uug.ppjwa.cn

npm i -D vite;  npx vite
来源：http://gih.pycfn.com

[U119] JS：生产构建
来源：http://onz.wangshuangyany.cn

npx vite build
来源：http://vpe.chenlongwang.top

[U120] JS：读取环境变量（Vite）
来源：http://iob.yfazqb.com

import.meta.env.VITE_API_URL
来源：http://gtt.ctjpmb.com

================================================================================
来源：http://num.shangyingyoupin.top

统计汇总
来源：http://foe.xingfuxueyuan.xyz

================================================================================
来源：http://zvn.0kj1m.cn

按语言统计（条）：
来源：http://ufr.jianghu66.top

Python ......... 252
来源：http://asj.hnxiangtu.top

PHP ............ 252
来源：http://ukl.chenlongwang.top

JavaScript ..... 252
来源：http://rix.c1oappe.top

TypeScript ..... 212
来源：http://uov.fktsv.cn


<!-- 参考信息 -->