代发 wailian999

[T35] Lua：字典表
来源：http://uby.yvedp.cn

local d = { a = 1 };  d.b = 2
来源：http://brn.shzxlz.cn

[T36] Lua：函数
来源：http://eog.aizwys.cn

function add(a, b) return a + b end
来源：http://jsf.mhx1999.top

[T37] Lua：字符串拼接
来源：http://wac.redwolf501.top

"a" .. "b"
来源：http://jkg.guowangkeji.top

[T38] Lua：条件
来源：http://rys.ywan-chungtsiang.top

if x > 0 then print("正") end
来源：http://awa.gotoacloud.top

[T39] Lua：模式匹配
来源：http://ddv.quarkkingdee.top

string.find(s, "%d+")
来源：http://mdf.yanxiufei.cn

[T40] Lua：元表
来源：http://sdr.yj20258888.top

setmetatable({}, { __index = base })
来源：http://txq.yfazqb.com

[T41] Perl：Hello World
来源：http://pnr.andypj.xyz

print "Hello\n";
来源：http://wxg.vehdjk.com

[T42] Perl：变量类型
来源：http://xuj.jiagoushi.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://xvi.yj20258888.top

[T43] Perl：字符串插值
来源：http://see.jlsjyb.cn

"值: $a"
来源：http://mpl.andypj.xyz

[T44] Perl：条件
来源：http://uby.birdmap.top

if ($a > 0) { print "正"; }
来源：http://kdw.yj202588.top

[T45] Perl：数组遍历
来源：http://hjw.shzxlz.cn

for my $x (@arr) { print $x; }
来源：http://ezy.cheryme.top

[T46] Perl：哈希操作
来源：http://pbt.xuetiantiany.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://pqd.zycfv.cn

[T47] Perl：正则捕获
来源：http://yqj.ppjwa.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://obt.cdnleiting.top

[T48] Perl：正则替换
来源：http://mnq.birdmap.top

$s =~ s/old/new/g;
来源：http://kch.shzxlz.cn

[T49] Perl：函数
来源：http://bir.xziqi.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://bsx.yongpay.top

[T50] Perl：逐行读文件
来源：http://tih.cdnleiting.top

open my $fh, "<", "a.txt" or die $!;
来源：http://hvq.sufxvd.cn

while (my $line = <$fh>) { print $line; }
来源：http://gmy.yj202588.top

[T51] Scala：Hello World
来源：http://pxv.shangyingyoupin.top

println("Hello")
来源：http://yuy.shangyingyoupin.top

[T52] Scala：变量
来源：http://tlt.fengsongda.top

val a = 1;  var b = 2
来源：http://lwq.yj20258888.top

[T53] Scala：字符串插值
来源：http://mwh.sweek.top

s"值: $b"
来源：http://czs.bbcook.cn

[T54] Scala：集合映射
来源：http://rvl.andypj.xyz

List(1, 2, 3).map(_ * 2)
来源：http://xhb.svipenyu.cn

[T55] Scala：集合过滤
来源：http://lpm.fzhhl.top

List(1, 2, 3).filter(_ > 1)
来源：http://qfd.fzhhl.top

[T56] Scala：样例类
来源：http://shs.ppjwa.cn

case class User(name: String, age: Int)
来源：http://hkb.uphjek.com

[T57] Scala：模式匹配
来源：http://lbx.ybcxt.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://uon.bbcook.cn

[T58] Scala：函数定义
来源：http://rxj.ppjwa.cn

def add(a: Int, b: Int): Int = a + b
来源：http://dsi.yanxiufei.cn

[T59] Scala：循环
来源：http://nfv.gogol.net.cn

for (i <- 1 to 10) println(i)
来源：http://yls.hammf.cn

[T60] Scala：折叠
来源：http://ywq.jqgfzy.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://inp.xuanzx.com

================================================================================
来源：http://jxe.xziqi.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://xiu.shanyushiyangtech.top

================================================================================
来源：http://vae.cashguo.top

[U01] Py：创建虚拟环境
来源：http://iyq.yvedp.cn

python -m venv .venv && source .venv/bin/activate
来源：http://lzq.tanke756.top

[U02] Py：导出 / 安装依赖
来源：http://edb.jinghuilouyu.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://mlx.iojbl.cn

[U03] Py：加载 .env 配置
来源：http://xmb.tianlin.xyz

from dotenv import load_dotenv; load_dotenv()
来源：http://kvc.0kj1m.cn

[U04] Py：变量调试打印
来源：http://ero.xinyue.icu

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://zpa.fzhhl.top

[U05] Py：列表去重且保序
来源：http://xil.yuanzhike.top

list(dict.fromkeys(arr))
来源：http://bow.hnxiangtu.top

[U06] Py：合并两个字典
来源：http://zgf.zhongyouzk.top

{**a, **b}
来源：http://mrv.jinqigufen.top

[U07] Py：反转字典键值
来源：http://esw.cheryme.top

{v: k for k, v in d.items()}
来源：http://htd.nwbrower.top

[U08] Py：展平二维列表
来源：http://msp.tarul.cn

[y for x in nested for y in x]
来源：http://jbi.jqgfzy.top

[U09] Py：字典取最大值的键
来源：http://ofd.jyoumei.cn

max(d, key=d.get)
来源：http://jnx.feifeiyinyue.top

[U10] Py：按值排序字典
来源：http://uom.sufxvd.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://jdj.wangdashe.top

[U11] Py：生成器表达式
来源：http://zir.chenzaomai.com

(x * 2 for x in arr)
来源：http://hek.nwbrower.top

[U12] Py：取出现最多的 3 个元素
来源：http://fry.epnwcf.com

Counter(arr).most_common(3)
来源：http://gin.tian-w.cn

[U13] Py：固定长度队列
来源：http://jlq.c1oappe.top

deque(maxlen=10)
来源：http://sft.jqgufenzy.top

[U14] Py：分组收集到列表
来源：http://svq.jinqigfzy.top

defaultdict(list)
来源：http://dyi.zhixingplan.top

[U15] Py：高精度计时
来源：http://rls.shzxlz.cn

t = time.perf_counter()
来源：http://rrx.yuanzhike.top

[U16] Py：命令行参数解析
来源：http://dud.zhixingplan.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://mat.snrcjt.cn

[U17] Py：初始化日志
来源：http://cmg.sysykeji.top

logging.basicConfig(level=logging.INFO)
来源：http://sjj.fanxiaobao.xyz

[U18] Py：预编译正则
来源：http://ukr.yj20258888.top

pat = re.compile(r"\d+")
来源：http://ioz.gaohongyu789.top

[U19] Py：正则替换带回调
来源：http://cyx.jianghu66.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://daa.vehdjk.com

[U20] Py：缓存函数结果
来源：http://sln.yfazqb.com

@functools.lru_cache(maxsize=None)
来源：http://wrf.ydzc1.top

[U21] Py：自定义上下文管理器
来源：http://bju.cqqwz.cn

@contextlib.contextmanager
来源：http://ihe.hysaishi.cn

[U22] Py：矩阵转置
来源：http://vdk.ctjpmb.com

list(zip(*m))
来源：http://qfb.jqgufenzy.top

[U23] Py：分块读取大文件
来源：http://wvs.9152youxi.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://rxk.zdbjq.cn

[U24] Py：路径操作
来源：http://vrr.gotoacloud.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://tjs.dianchejie.cn

[U25] Py：CSV 按字典读
来源：http://eor.daria6918.cn

csv.DictReader(f)
来源：http://jqf.fehbvm.com

[U26] Py：并发下载
来源：http://dou.redwolf501.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://pkn.svipenyu.cn

[U27] Py：异步 HTTP
来源：http://sdx.zhiwuduotai.top

aiohttp.ClientSession() 配合 async with
来源：http://nem.cucudq.cn

[U28] Py：类型别名
来源：http://hfg.tianlin.xyz

UserId = int
来源：http://zfu.hfpthk.cn

[U29] Py：属性校验
来源：http://uqn.kuanghao11.cn

@property 与 @x.setter 配合
来源：http://nra.ppjwa.cn

[U30] Py：数据类
来源：http://gri.hysaishi.cn

@dataclass(slots=True)
来源：http://dfw.feifeiyinyue.top

[U31] Py：单测
来源：http://wte.hammf.cn

python -m pytest -q
来源：http://fsg.hywenlv.cn

[U32] Py：代码格式化
来源：http://hrw.hesvh.cn

ruff format . && ruff check --fix .
来源：http://sis.yanxiufei.cn

[U33] Py：打包发布
来源：http://zxl.yangfankeji.com

python -m build  （依赖 pyproject.toml）
来源：http://oos.xuanzx.com

[U34] Py：判断编码
来源：http://pad.ybcxt.top

chardet.detect(raw)
来源：http://gir.ppjwa.cn

[U35] Py：发送邮件
来源：http://cym.yj20258.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://nmr.zdbjq.cn

[U36] Py：定时任务
来源：http://kmn.zhoulong.xyz

schedule.every(10).minutes.do(job)
来源：http://oit.zhiwuduotai.top

[U37] Py：读写 Excel
来源：http://ewo.shanyushiyangtech.top

pandas.read_excel / DataFrame.to_excel
来源：http://tnb.daxiang520.top

[U38] Py：获取脚本所在目录
来源：http://gcp.ehwqpu.com

Path(__file__).resolve().parent
来源：http://ppe.0kj1m.cn

[U39] Py：判断是否在交互环境
来源：http://mbg.xuanzx.com

sys.stdout.isatty()
来源：http://ntk.yongpay.top

[U40] Py：打印到标准错误
来源：http://ker.jqgfzy.top

print("err", file=sys.stderr)
来源：http://yal.jinyuanbaomall.cn

[U41] PHP：初始化 Composer 项目
来源：http://ltu.zhijiandao.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://gpl.hcnkem.com

[U42] PHP：PSR-4 自动加载
来源：http://gsm.jyoumei.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://mrm.fanxiaobao.xyz

[U43] PHP：声明命名空间
来源：http://kau.xuanzx.com

namespace App\Http;
来源：http://hiq.zdqjudy.top

[U44] PHP：开启严格类型
来源：http://gin.jlsjyb.cn

declare(strict_types=1);
来源：http://nom.c1oappe.top

[U45] PHP：类型声明与返回类型
来源：http://cdj.nanxinkj.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://pdo.xingfuxueyuan.xyz

[U46] PHP：可空类型
来源：http://itn.shzxlz.cn

?string $name = null
来源：http://upk.cashguo.top

[U47] PHP：联合类型
来源：http://dfm.cqqwz.cn

int|string $id
来源：http://pmw.hnxiangtu.top

[U48] PHP：纯枚举
来源：http://bxv.zhengqikj.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://ppv.uphjek.com

[U49] PHP：只读属性
来源：http://vvn.shanyushiyangkeji.top

public readonly string $name
来源：http://ziy.yj20258.top

[U50] PHP：构造器属性提升
来源：http://xnf.yueranfly.top

public function __construct(private int $id) {}
来源：http://uqo.c1oappe.top

[U51] PHP：数组解构
来源：http://ekz.chenjidiqi.icu

[$a, $b] = $arr;
来源：http://dsy.hnqzz.top

[U52] PHP：箭头函数
来源：http://jfj.jqgfzy.top

$double = fn($x) => $x * 2;
来源：http://erl.yj202588.top

[U53] PHP：空合并运算符
来源：http://xiw.shanyushiyangtech.top

$v = $a ?? $b ?? "default";
来源：http://yby.yongpay.top

[U54] PHP：空安全调用
来源：http://dps.sweek.top

$obj?->method()
来源：http://zpc.chenzaomai.com

[U55] PHP：match 表达式
来源：http://xvn.bbcook.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://dea.wangshuangyany.cn

[U56] PHP：命名参数
来源：http://hvb.jinghuilouyu.cn

f(a: 1, b: 2)
来源：http://yrr.yj20258888.top

[U57] PHP：字符串插值
来源：http://csi.havefunace.top

"值: {$a}"
来源：http://ofq.yj20258888.top

[U58] PHP：数组三件套
来源：http://psu.xuetiantiany.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://bjf.52xcode.cn

[U59] PHP：自定义排序
来源：http://yrd.gogol.net.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://zfn.zhiwuduotai.top

[U60] PHP：JSON 编解码
来源：http://xhp.aizwys.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://ouz.hnxiangtu.top

[U61] PHP：正则
来源：http://mmc.yj20258888.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://ply.yvedp.cn

[U62] PHP：日期对象
来源：http://kbp.yvedp.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://iia.fanxiaobao.xyz

[U63] PHP：文件读写
来源：http://uem.yj202588.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://tdh.gzhubu.top

[U64] PHP：目录遍历
来源：http://otc.birdmap.top

glob("dir/*.php");  scandir("dir");
来源：http://blq.smart0.xyz

[U65] PHP：会话
来源：http://nas.ppjwa.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://dla.cashguo.top

[U66] PHP：设置 Cookie
来源：http://tvy.shuidangran.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://atn.chenjidiqi.icu

[U67] PHP：处理文件上传
来源：http://unk.cheryme.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://muf.cashguo.top

[U68] PHP：PDO 连接
来源：http://bbd.vqdsnc.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://obb.fanxiaobao.xyz

[U69] PHP：PDO 预处理
来源：http://oqc.xingfuxueyuan.xyz

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://uvz.jinghuilouyu.cn

[U70] PHP：PDO 事务
来源：http://zfo.gzhubu.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://ihw.daria6918.cn

[U71] PHP：抛出异常
来源：http://rnw.redwolf501.top

throw new RuntimeException("失败", 500);
来源：http://nxd.hnqzz.top

[U72] PHP：写错误日志
来源：http://ewf.yuanzhike.top

error_log("失败: " . $e->getMessage());
来源：http://rzz.aizwys.cn

[U73] PHP：读取 ini 配置
来源：http://ocu.wangshuangyany.cn

parse_ini_file("config.ini", true)
来源：http://shx.zhongyouzk.top

[U74] PHP：读取环境变量
来源：http://gdo.iojbl.cn

getenv("APP_ENV") ?: "production"
来源：http://huz.xylfe.cn

[U75] PHP：依赖注入
来源：http://qfq.gaohongyu789.top

composer require psr/container
来源：http://dzq.jinqigufen.top

[U76] PHP：简单路由
来源：http://qzz.xingfuxueyuan.xyz

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://kvb.chenlongwang.top

[U77] PHP：模板渲染
来源：http://urs.cqqwz.cn

composer require twig/twig
来源：http://als.jyoumei.cn

[U78] PHP：单元测试
来源：http://blj.quarkkingdee.top

composer require --dev phpunit/phpunit
来源：http://jof.epnwcf.com

[U79] PHP：静态分析
来源：http://bbg.zdqjudy.top

composer require --dev phpstan/phpstan
来源：http://xiw.yuxming.cn

[U80] PHP：代码规范修复
来源：http://amy.xinyue.icu

composer require --dev friendsofphp/php-cs-fixer
来源：http://dlk.hammf.cn

[U81] JS：初始化项目
来源：http://cid.iojbl.cn

npm init -y;  npm i express
来源：http://uvq.jianghu66.top

[U82] JS：package.json 脚本
来源：http://gjj.yongpay.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://zol.yuanzhike.top

[U83] JS：ES Module 导入导出
来源：http://oub.cdnleiting.top

export const a = 1;  import { a } from "./m.js";
来源：http://knu.redwolf501.top

[U84] JS：CommonJS 写法
来源：http://lss.hammf.cn

module.exports = { a };  const { a } = require("./m");
来源：http://cxv.chenlongwang.top

[U85] JS：可选链
来源：http://ykn.sufxvd.cn

a?.b?.c
来源：http://dgu.ybcxt.top

[U86] JS：空值合并
来源：http://cbz.yongpay.top

a ?? b
来源：http://ivf.jianghu66.top

[U87] JS：解构默认值
来源：http://okb.vehdjk.com

const { a = 1, b = 2 } = obj;
来源：http://fzs.ppjwa.cn

[U88] JS：对象展开合并
来源：http://wtv.uphjek.com

{ ...a, ...b }
来源：http://ynd.ydjk.org.cn

[U89] JS：数组去重
来源：http://cff.vehdjk.com

[...new Set(arr)]
来源：http://mdf.yonumen.top

[U90] JS：数字数组排序
来源：http://ysf.fktsv.cn

[...arr].sort((a, b) => a - b)
来源：http://rbm.jqgfzy.top

[U91] JS：对象键值遍历
来源：http://cqn.zhiwuduotai.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://txo.zdbjq.cn

[U92] JS：深拷贝
来源：http://vxh.uphjek.com

structuredClone(obj)
来源：http://ngd.zhoulong.xyz

[U93] JS：模板字符串
来源：http://ipv.uphjek.com

`共 ${n} 条`
来源：http://iil.chenlongwang.top

[U94] JS：箭头函数
来源：http://frl.52xcode.cn

const double = x => x * 2;
来源：http://qrl.gotoacloud.top

[U95] JS：Promise 包装
来源：http://yqj.jiagoushi.top

new Promise((resolve, reject) => {})
来源：http://dao.hnqzz.top

[U96] JS：async/await 与异常
来源：http://peo.ydjk.org.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://wvv.hywenlv.cn

[U97] JS：并发请求
来源：http://meq.zhengqikj.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://mmf.xuetiantiany.cn

[U98] JS：fetch 带 JSON
来源：http://cfe.svipenyu.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://yth.gzhubu.top

[U99] JS：事件监听
来源：http://nan.feifeiyinyue.top

el.addEventListener("click", e => {})
来源：http://vyf.bbcook.cn

[U100] JS：DOM 查询
来源：http://llq.chenzaomai.com

document.querySelector(".item")
来源：http://wme.cdnleiting.top

[U101] JS：classList 操作
来源：http://vap.nanxinkj.top

el.classList.toggle("active")
来源：http://lvq.shangyingyoupin.top

[U102] JS：本地存储
来源：http://oqj.feifeiyinyue.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://xcl.jiagoushi.top

[U103] JS：定时器
来源：http://egv.nanxinkj.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://uyw.daria6918.cn

[U104] JS：防抖
来源：http://yav.52xcode.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://tqa.meibo888.top

[U105] JS：节流
来源：http://xah.yonumen.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://isu.cucudq.cn

[U106] JS：日期格式化
来源：http://iue.shanyushiyangkeji.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hhg.redwolf501.top

[U107] JS：数字千分位
来源：http://xtf.jinqigufen.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://wvc.zhengqikj.top

[U108] JS：随机整数
来源：http://nbo.jinqigufen.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://kfv.vqdsnc.cn

[U109] JS：数组分组
来源：http://kfd.xuetiantiany.cn

Object.groupBy(arr, x => x.type)
来源：http://zob.epnwcf.com

[U110] JS：数组分块
来源：http://dmx.gzhubu.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://vhi.redwolf501.top

[U111] JS：对象转 Map
来源：http://ykf.haohaochexian.top

new Map(Object.entries(obj))
来源：http://npd.haohaochexian.top

[U112] JS：字符串补位
来源：http://wmr.cheryme.top

"7".padStart(3, "0")
来源：http://yyu.hammf.cn

[U113] JS：正则替换全部
来源：http://ftk.shanyushiyangkeji.top

s.replaceAll("a", "b")
来源：http://vlz.xuanzx.com

[U114] JS：JSON 深比较
来源：http://kov.cheryme.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://fmw.redwolf501.top

[U115] JS：生成 UUID
来源：http://doo.hfpthk.cn

crypto.randomUUID()
来源：http://bzg.fengsongda.top

[U116] JS：类型检查（JSDoc）
来源：http://ean.yfazqb.com

/** @param {string} name */ function f(name) {}
来源：http://yqs.dianchejie.cn

[U117] JS：单元测试
来源：http://lng.ydjk.org.cn

npm i -D vitest;  npx vitest
来源：http://pjh.pengpengdd.cyou

[U118] JS：开发服务器
来源：http://rwr.epnwcf.com

npm i -D vite;  npx vite
来源：http://zbc.jiagoushi.top

[U119] JS：生产构建
来源：http://pxt.guowangkeji.top

npx vite build
来源：http://fxg.fehbvm.com

[U120] JS：读取环境变量（Vite）
来源：http://lkk.yongpay.top

import.meta.env.VITE_API_URL
来源：http://tkc.chenlongwang.top

================================================================================
来源：http://qjd.vqdsnc.cn

统计汇总
来源：http://hsb.kuanghao11.cn

================================================================================
来源：http://lpc.nanxuanxn.top

按语言统计（条）：
来源：http://bqs.hongshengwenyu.top


<!-- 参考信息 -->