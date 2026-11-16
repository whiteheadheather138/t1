代发 wailian999

[T33] Lua：表（数组）
来源：http://zxj.redwolf501.top

local t = {1, 2, 3};  t[4] = 4
来源：http://hgw.nwbrower.top

[T34] Lua：遍历表
来源：http://pfe.xingfuxueyuan.xyz

for i, v in ipairs(t) do print(i, v) end
来源：http://llg.ehwqpu.com

[T35] Lua：字典表
来源：http://vyi.yfazqb.com

local d = { a = 1 };  d.b = 2
来源：http://arm.jinqigufen.top

[T36] Lua：函数
来源：http://uss.aizwys.cn

function add(a, b) return a + b end
来源：http://jbh.bbcook.cn

[T37] Lua：字符串拼接
来源：http://ghr.yanxiufei.cn

"a" .. "b"
来源：http://zlp.xuanzx.com

[T38] Lua：条件
来源：http://xpn.shuidangran.top

if x > 0 then print("正") end
来源：http://pnl.shangyingyoupin.top

[T39] Lua：模式匹配
来源：http://ucx.uphjek.com

string.find(s, "%d+")
来源：http://tnp.9152youxi.cn

[T40] Lua：元表
来源：http://won.chenlongwang.top

setmetatable({}, { __index = base })
来源：http://ayq.birdmap.top

[T41] Perl：Hello World
来源：http://tup.yueranfly.top

print "Hello\n";
来源：http://klj.shzxlz.cn

[T42] Perl：变量类型
来源：http://fbh.zhaomingkeji.xyz

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://gon.ivvv.top

[T43] Perl：字符串插值
来源：http://cud.sjlbkw.cn

"值: $a"
来源：http://uhe.hnxiangtu.top

[T44] Perl：条件
来源：http://tmt.hammf.cn

if ($a > 0) { print "正"; }
来源：http://dln.ybcxt.top

[T45] Perl：数组遍历
来源：http://tnw.yvedp.cn

for my $x (@arr) { print $x; }
来源：http://hns.jianghu66.top

[T46] Perl：哈希操作
来源：http://hbu.dashuyun.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://gyb.jianghu66.top

[T47] Perl：正则捕获
来源：http://qoq.yuxming.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://obr.sweek.top

[T48] Perl：正则替换
来源：http://mcx.chenjidiqi.icu

$s =~ s/old/new/g;
来源：http://nuv.jinqigfzy.top

[T49] Perl：函数
来源：http://beh.haohaochexian.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://acs.ybcxt.top

[T50] Perl：逐行读文件
来源：http://ifs.tian-w.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://tsd.havefunace.top

while (my $line = <$fh>) { print $line; }
来源：http://fyq.shanyushiyangkeji.top

[T51] Scala：Hello World
来源：http://uuk.wangshuangyany.cn

println("Hello")
来源：http://ieg.snrcjt.cn

[T52] Scala：变量
来源：http://goy.tian-w.cn

val a = 1;  var b = 2
来源：http://cyj.jinghuilouyu.cn

[T53] Scala：字符串插值
来源：http://jgo.zycfv.cn

s"值: $b"
来源：http://vgr.bbcook.cn

[T54] Scala：集合映射
来源：http://qrp.havefunace.top

List(1, 2, 3).map(_ * 2)
来源：http://ysx.zhoulong.xyz

[T55] Scala：集合过滤
来源：http://ksc.52xcode.cn

List(1, 2, 3).filter(_ > 1)
来源：http://gqr.xinyue.icu

[T56] Scala：样例类
来源：http://fya.zycfv.cn

case class User(name: String, age: Int)
来源：http://zmk.gogol.net.cn

[T57] Scala：模式匹配
来源：http://hkr.xylfe.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://wiy.xylfe.cn

[T58] Scala：函数定义
来源：http://qep.hongshengwenyu.top

def add(a: Int, b: Int): Int = a + b
来源：http://slz.fanxiaobao.xyz

[T59] Scala：循环
来源：http://sim.ehwqpu.com

for (i <- 1 to 10) println(i)
来源：http://urh.nanxuanxn.top

[T60] Scala：折叠
来源：http://drl.xuanzx.com

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://uoi.ywan-chungtsiang.top

================================================================================
来源：http://tfa.gogol.net.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://qzv.ybcxt.top

================================================================================
来源：http://tyh.nanxuanxn.top

[U01] Py：创建虚拟环境
来源：http://pbc.jianghu66.top

python -m venv .venv && source .venv/bin/activate
来源：http://aqk.0kj1m.cn

[U02] Py：导出 / 安装依赖
来源：http://buf.ehwqpu.com

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://mod.dianchejie.cn

[U03] Py：加载 .env 配置
来源：http://yib.zdbjq.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://gsp.zhengqikj.top

[U04] Py：变量调试打印
来源：http://edn.nwbrower.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://bzn.meibo888.top

[U05] Py：列表去重且保序
来源：http://tfd.guannengcc.top

list(dict.fromkeys(arr))
来源：http://unt.gogol.net.cn

[U06] Py：合并两个字典
来源：http://gxc.jqgfzy.top

{**a, **b}
来源：http://cop.nanxuanxn.top

[U07] Py：反转字典键值
来源：http://zjn.xylfe.cn

{v: k for k, v in d.items()}
来源：http://wnp.yongpay.top

[U08] Py：展平二维列表
来源：http://ast.jinqigufen.top

[y for x in nested for y in x]
来源：http://arf.uphjek.com

[U09] Py：字典取最大值的键
来源：http://xtj.zhengqikj.top

max(d, key=d.get)
来源：http://heu.shanyushiyangkeji.top

[U10] Py：按值排序字典
来源：http://asc.hysaishi.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://ipm.cheryme.top

[U11] Py：生成器表达式
来源：http://knn.hnqzz.top

(x * 2 for x in arr)
来源：http://wbm.zdbjq.cn

[U12] Py：取出现最多的 3 个元素
来源：http://rdz.nwbrower.top

Counter(arr).most_common(3)
来源：http://yni.yj20258.top

[U13] Py：固定长度队列
来源：http://lgy.feifeiyinyue.top

deque(maxlen=10)
来源：http://mil.0kj1m.cn

[U14] Py：分组收集到列表
来源：http://qqa.shuidangran.top

defaultdict(list)
来源：http://zwz.yueranfly.top

[U15] Py：高精度计时
来源：http://amk.dashuyun.cn

t = time.perf_counter()
来源：http://ami.gogol.net.cn

[U16] Py：命令行参数解析
来源：http://yji.wangshuangyany.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://crj.316326.xyz

[U17] Py：初始化日志
来源：http://zmn.chenlongwang.top

logging.basicConfig(level=logging.INFO)
来源：http://msh.pengpengdd.cyou

[U18] Py：预编译正则
来源：http://owx.jlsjyb.cn

pat = re.compile(r"\d+")
来源：http://srw.xingfuxueyuan.xyz

[U19] Py：正则替换带回调
来源：http://iyi.mhx1999.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://kse.vehdjk.com

[U20] Py：缓存函数结果
来源：http://vwy.ydjk.org.cn

@functools.lru_cache(maxsize=None)
来源：http://sic.tanke756.top

[U21] Py：自定义上下文管理器
来源：http://nvj.daria6918.cn

@contextlib.contextmanager
来源：http://elo.xuanzx.com

[U22] Py：矩阵转置
来源：http://axi.sysykeji.top

list(zip(*m))
来源：http://cva.ybcxt.top

[U23] Py：分块读取大文件
来源：http://ayr.ehwqpu.com

for chunk in iter(lambda: f.read(8192), b""):
来源：http://gts.jqgufenzy.top

[U24] Py：路径操作
来源：http://ruw.cashguo.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://spj.vqdsnc.cn

[U25] Py：CSV 按字典读
来源：http://svh.xylfe.cn

csv.DictReader(f)
来源：http://oow.fzhhl.top

[U26] Py：并发下载
来源：http://dzm.sjlbkw.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://bhh.9152youxi.cn

[U27] Py：异步 HTTP
来源：http://sjb.zhongyouzk.top

aiohttp.ClientSession() 配合 async with
来源：http://zyd.316326.xyz

[U28] Py：类型别名
来源：http://bhk.xziqi.cn

UserId = int
来源：http://edq.quarkkingdee.top

[U29] Py：属性校验
来源：http://bid.xuetiantiany.cn

@property 与 @x.setter 配合
来源：http://nxb.jinghuilouyu.cn

[U30] Py：数据类
来源：http://wsm.wangdashe.top

@dataclass(slots=True)
来源：http://ptm.0kj1m.cn

[U31] Py：单测
来源：http://fdr.cqqwz.cn

python -m pytest -q
来源：http://sdk.hcnkem.com

[U32] Py：代码格式化
来源：http://wys.c1oappe.top

ruff format . && ruff check --fix .
来源：http://swi.ywan-chungtsiang.top

[U33] Py：打包发布
来源：http://jcg.cheryme.top

python -m build  （依赖 pyproject.toml）
来源：http://scl.shzxlz.cn

[U34] Py：判断编码
来源：http://tpp.yuxming.cn

chardet.detect(raw)
来源：http://igz.fzhhl.top

[U35] Py：发送邮件
来源：http://ibi.jinqigufen.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://mmx.smart0.xyz

[U36] Py：定时任务
来源：http://hnp.bjfxy.top

schedule.every(10).minutes.do(job)
来源：http://zny.sysykeji.top

[U37] Py：读写 Excel
来源：http://qwe.tanke756.top

pandas.read_excel / DataFrame.to_excel
来源：http://agf.hnxiangtu.top

[U38] Py：获取脚本所在目录
来源：http://zae.chenzaomai.com

Path(__file__).resolve().parent
来源：http://lqb.dianchejie.cn

[U39] Py：判断是否在交互环境
来源：http://miz.gotoacloud.top

sys.stdout.isatty()
来源：http://kib.hnqzz.top

[U40] Py：打印到标准错误
来源：http://suy.yfazqb.com

print("err", file=sys.stderr)
来源：http://duo.wangshuangyany.cn

[U41] PHP：初始化 Composer 项目
来源：http://crr.yuxming.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://cdr.jqgfzy.top

[U42] PHP：PSR-4 自动加载
来源：http://mup.ivvv.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://tqb.daxiang520.top

[U43] PHP：声明命名空间
来源：http://foz.ctjpmb.com

namespace App\Http;
来源：http://cqy.jlsjyb.cn

[U44] PHP：开启严格类型
来源：http://uuu.gogol.net.cn

declare(strict_types=1);
来源：http://tgd.ppjwa.cn

[U45] PHP：类型声明与返回类型
来源：http://tjq.shanyushiyangkeji.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://blk.ywan-chungtsiang.top

[U46] PHP：可空类型
来源：http://hcd.zhixingplan.top

?string $name = null
来源：http://dys.haohaochexian.top

[U47] PHP：联合类型
来源：http://rrj.yonumen.top

int|string $id
来源：http://cpn.vehdjk.com

[U48] PHP：纯枚举
来源：http://hop.tianlin.xyz

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://jub.yangfankeji.com

[U49] PHP：只读属性
来源：http://dis.xziqi.cn

public readonly string $name
来源：http://xnq.nwbrower.top

[U50] PHP：构造器属性提升
来源：http://wox.gogol.net.cn

public function __construct(private int $id) {}
来源：http://byn.ppjwa.cn

[U51] PHP：数组解构
来源：http://fsv.feifeiyinyue.top

[$a, $b] = $arr;
来源：http://foa.chenzaomai.com

[U52] PHP：箭头函数
来源：http://exq.sufxvd.cn

$double = fn($x) => $x * 2;
来源：http://ttl.ivvv.top

[U53] PHP：空合并运算符
来源：http://fva.fktsv.cn

$v = $a ?? $b ?? "default";
来源：http://cey.cheryme.top

[U54] PHP：空安全调用
来源：http://xob.jqgufenzy.top

$obj?->method()
来源：http://jiu.c1oappe.top

[U55] PHP：match 表达式
来源：http://ddf.sxryk.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://efp.shanyushiyangkeji.top

[U56] PHP：命名参数
来源：http://udo.nanxuanxn.top

f(a: 1, b: 2)
来源：http://hta.jiagoushi.top

[U57] PHP：字符串插值
来源：http://acq.yangfankeji.com

"值: {$a}"
来源：http://pox.hesvh.cn

[U58] PHP：数组三件套
来源：http://ckl.gzhubu.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://lap.jyoumei.cn

[U59] PHP：自定义排序
来源：http://ift.sjlbkw.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://zcu.hfpthk.cn

[U60] PHP：JSON 编解码
来源：http://uiv.tian-w.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://acr.sjlbkw.cn

[U61] PHP：正则
来源：http://spu.birdmap.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://uxb.gaohongyu789.top

[U62] PHP：日期对象
来源：http://moo.iojbl.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://foh.sysykeji.top

[U63] PHP：文件读写
来源：http://nnw.ydzc1.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://ups.tarul.cn

[U64] PHP：目录遍历
来源：http://bbq.hfpthk.cn

glob("dir/*.php");  scandir("dir");
来源：http://joo.svipenyu.cn

[U65] PHP：会话
来源：http://qbp.pengpengdd.cyou

session_start();  $_SESSION["uid"] = 1;
来源：http://oyc.pengpengdd.cyou

[U66] PHP：设置 Cookie
来源：http://wof.hfpthk.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://buc.meibo888.top

[U67] PHP：处理文件上传
来源：http://ond.chenjidiqi.icu

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://dgr.ehwqpu.com

[U68] PHP：PDO 连接
来源：http://saa.zhixingplan.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://lpd.gaohongyu789.top

[U69] PHP：PDO 预处理
来源：http://zxp.hnxiangtu.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://xnt.daria6918.cn

[U70] PHP：PDO 事务
来源：http://txr.kuanghao11.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://pgu.sweek.top

[U71] PHP：抛出异常
来源：http://xhq.cdnleiting.top

throw new RuntimeException("失败", 500);
来源：http://kty.xuanzx.com

[U72] PHP：写错误日志
来源：http://qhs.gotoacloud.top

error_log("失败: " . $e->getMessage());
来源：http://zkh.zycfv.cn

[U73] PHP：读取 ini 配置
来源：http://ysq.cheryme.top

parse_ini_file("config.ini", true)
来源：http://rip.andypj.xyz

[U74] PHP：读取环境变量
来源：http://flv.vehdjk.com

getenv("APP_ENV") ?: "production"
来源：http://syb.sxryk.cn

[U75] PHP：依赖注入
来源：http://neq.yfazqb.com

composer require psr/container
来源：http://fsv.quarkkingdee.top

[U76] PHP：简单路由
来源：http://qon.zycfv.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://uae.hnxiangtu.top

[U77] PHP：模板渲染
来源：http://knv.zhengqikj.top

composer require twig/twig
来源：http://mwk.gotoacloud.top

[U78] PHP：单元测试
来源：http://evm.hywenlv.cn

composer require --dev phpunit/phpunit
来源：http://fnl.tian-w.cn

[U79] PHP：静态分析
来源：http://zmu.feifeiyinyue.top

composer require --dev phpstan/phpstan
来源：http://apz.sufxvd.cn

[U80] PHP：代码规范修复
来源：http://dml.snrcjt.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://gcj.yongpay.top

[U81] JS：初始化项目
来源：http://gxw.cucudq.cn

npm init -y;  npm i express
来源：http://gse.ivvv.top

[U82] JS：package.json 脚本
来源：http://pkj.yuanzhike.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://tnv.yangfankeji.com

[U83] JS：ES Module 导入导出
来源：http://tct.0kj1m.cn

export const a = 1;  import { a } from "./m.js";
来源：http://ltp.haohaochexian.top

[U84] JS：CommonJS 写法
来源：http://qkc.hesvh.cn

module.exports = { a };  const { a } = require("./m");
来源：http://pxk.gotoacloud.top

[U85] JS：可选链
来源：http://vmx.jyoumei.cn

a?.b?.c
来源：http://tvl.zhoulong.xyz

[U86] JS：空值合并
来源：http://qre.tarul.cn

a ?? b
来源：http://sdl.ctjpmb.com

[U87] JS：解构默认值
来源：http://ywr.chenjidiqi.icu

const { a = 1, b = 2 } = obj;
来源：http://flg.zhiwuduotai.top

[U88] JS：对象展开合并
来源：http://pdj.hfpthk.cn

{ ...a, ...b }
来源：http://tnm.fehbvm.com

[U89] JS：数组去重
来源：http://qzr.yfazqb.com

[...new Set(arr)]
来源：http://slx.sufxvd.cn

[U90] JS：数字数组排序
来源：http://udb.xingfuxueyuan.xyz

[...arr].sort((a, b) => a - b)
来源：http://feh.c1oappe.top

[U91] JS：对象键值遍历
来源：http://sbm.zhaomingkeji.xyz

Object.entries(obj).forEach(([k, v]) => {});
来源：http://lfo.yangfankeji.com

[U92] JS：深拷贝
来源：http://dfp.fzhhl.top

structuredClone(obj)
来源：http://jvo.svipenyu.cn

[U93] JS：模板字符串
来源：http://tdx.smart0.xyz

`共 ${n} 条`
来源：http://kgc.yfazqb.com

[U94] JS：箭头函数
来源：http://raj.yfazqb.com

const double = x => x * 2;
来源：http://tvg.0kj1m.cn

[U95] JS：Promise 包装
来源：http://qnk.yvedp.cn

new Promise((resolve, reject) => {})
来源：http://zta.cdnleiting.top

[U96] JS：async/await 与异常
来源：http://pvq.yangfankeji.com

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://fta.9152youxi.cn

[U97] JS：并发请求
来源：http://spb.ivvv.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://yyk.hnqzz.top

[U98] JS：fetch 带 JSON
来源：http://spa.fanxiaobao.xyz

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://kgt.chenlongwang.top

[U99] JS：事件监听
来源：http://xnj.hnxiangtu.top

el.addEventListener("click", e => {})
来源：http://xsx.zdbjq.cn

[U100] JS：DOM 查询
来源：http://cas.fehbvm.com

document.querySelector(".item")
来源：http://bcl.guowangkeji.top

[U101] JS：classList 操作
来源：http://wsq.zhixingplan.top

el.classList.toggle("active")
来源：http://ydt.pycfn.com

[U102] JS：本地存储
来源：http://jza.ywan-chungtsiang.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://dms.cqqwz.cn

[U103] JS：定时器
来源：http://yai.shanyushiyangtech.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://lkp.ehwqpu.com

[U104] JS：防抖
来源：http://ulb.fanxiaobao.xyz

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://qqm.vqdsnc.cn

[U105] JS：节流
来源：http://nlp.chenlongwang.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://aow.c1oappe.top

[U106] JS：日期格式化
来源：http://anp.shuidangran.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://fwa.tian-w.cn

[U107] JS：数字千分位
来源：http://dpl.haohaochexian.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://fpb.redwolf501.top

[U108] JS：随机整数
来源：http://zis.zhoulong.xyz

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://xqa.jinqigfzy.top

[U109] JS：数组分组
来源：http://xbn.dianchejie.cn

Object.groupBy(arr, x => x.type)
来源：http://zxs.fengsongda.top

[U110] JS：数组分块
来源：http://lxw.tian-w.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://yrj.zhaomingkeji.xyz

[U111] JS：对象转 Map
来源：http://amw.zhongyouzk.top

new Map(Object.entries(obj))
来源：http://fgl.xylfe.cn

[U112] JS：字符串补位
来源：http://jqo.nanxinkj.top

"7".padStart(3, "0")
来源：http://lyx.sysykeji.top

[U113] JS：正则替换全部
来源：http://qdr.nanxinkj.top

s.replaceAll("a", "b")
来源：http://yga.jyoumei.cn

[U114] JS：JSON 深比较
来源：http://epp.tanke756.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://zad.ydjk.org.cn

[U115] JS：生成 UUID
来源：http://myc.vehdjk.com

crypto.randomUUID()
来源：http://glp.vqdsnc.cn

[U116] JS：类型检查（JSDoc）
来源：http://ort.gzhubu.top

/** @param {string} name */ function f(name) {}
来源：http://zbw.c1oappe.top

[U117] JS：单元测试
来源：http://oge.quarkkingdee.top

npm i -D vitest;  npx vitest
来源：http://nxd.yj20258.top

[U118] JS：开发服务器
来源：http://uxo.vehdjk.com

npm i -D vite;  npx vite
来源：http://rpc.bbcook.cn

[U119] JS：生产构建
来源：http://dnl.yfazqb.com

npx vite build
来源：http://bse.fengsongda.top

[U120] JS：读取环境变量（Vite）
来源：http://wfg.bbcook.cn

import.meta.env.VITE_API_URL
来源：http://bjc.yueranfly.top


<!-- 参考信息 -->