代发 wailian999

[T29] Swift：guard 提前返回
来源：http://yip.zdbjq.cn

guard let x = opt else { return }
来源：http://psp.pycfn.com

[T30] Swift：协议
来源：http://xxg.0kj1m.cn

protocol Shape { func area() -> Double }
来源：http://sec.nanxinkj.top

[T31] Lua：Hello World
来源：http://puq.0kj1m.cn

print("Hello")
来源：http://vfw.0kj1m.cn

[T32] Lua：局部变量
来源：http://mzf.chenjidiqi.icu

local a = 1
来源：http://cfa.yj20258888.top

[T33] Lua：表（数组）
来源：http://kwx.zhixingplan.top

local t = {1, 2, 3};  t[4] = 4
来源：http://iqv.cdnleiting.top

[T34] Lua：遍历表
来源：http://dyx.xinyue.icu

for i, v in ipairs(t) do print(i, v) end
来源：http://urg.yangfankeji.com

[T35] Lua：字典表
来源：http://chu.jyoumei.cn

local d = { a = 1 };  d.b = 2
来源：http://ixd.tanke756.top

[T36] Lua：函数
来源：http://ink.xylfe.cn

function add(a, b) return a + b end
来源：http://krd.xuanzx.com

[T37] Lua：字符串拼接
来源：http://rvp.jqgufenzy.top

"a" .. "b"
来源：http://njy.havefunace.top

[T38] Lua：条件
来源：http://pyf.svipenyu.cn

if x > 0 then print("正") end
来源：http://xax.zycfv.cn

[T39] Lua：模式匹配
来源：http://grc.xziqi.cn

string.find(s, "%d+")
来源：http://yvl.yuanzhike.top

[T40] Lua：元表
来源：http://mbz.birdmap.top

setmetatable({}, { __index = base })
来源：http://jqy.pycfn.com

[T41] Perl：Hello World
来源：http://lta.shzxlz.cn

print "Hello\n";
来源：http://ngt.havefunace.top

[T42] Perl：变量类型
来源：http://aqk.tarul.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://opz.jyoumei.cn

[T43] Perl：字符串插值
来源：http://nrl.gzhubu.top

"值: $a"
来源：http://guj.guowangkeji.top

[T44] Perl：条件
来源：http://qdh.nwbrower.top

if ($a > 0) { print "正"; }
来源：http://qrk.jianghu66.top

[T45] Perl：数组遍历
来源：http://jii.zhengqikj.top

for my $x (@arr) { print $x; }
来源：http://vbc.havefunace.top

[T46] Perl：哈希操作
来源：http://yuj.jyoumei.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://gde.yongpay.top

[T47] Perl：正则捕获
来源：http://imh.quarkkingdee.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://xnp.yj20258888.top

[T48] Perl：正则替换
来源：http://jkq.zhiwuduotai.top

$s =~ s/old/new/g;
来源：http://oof.yvedp.cn

[T49] Perl：函数
来源：http://lny.wangshuangyany.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://flb.dashuyun.cn

[T50] Perl：逐行读文件
来源：http://bvq.chenjidiqi.icu

open my $fh, "<", "a.txt" or die $!;
来源：http://ioo.zdqjudy.top

while (my $line = <$fh>) { print $line; }
来源：http://grt.birdmap.top

[T51] Scala：Hello World
来源：http://mnu.sxryk.cn

println("Hello")
来源：http://gez.haohaochexian.top

[T52] Scala：变量
来源：http://snt.xingfuxueyuan.xyz

val a = 1;  var b = 2
来源：http://fdq.sufxvd.cn

[T53] Scala：字符串插值
来源：http://agm.hysaishi.cn

s"值: $b"
来源：http://pil.xingfuxueyuan.xyz

[T54] Scala：集合映射
来源：http://hyk.sysykeji.top

List(1, 2, 3).map(_ * 2)
来源：http://vel.aizwys.cn

[T55] Scala：集合过滤
来源：http://xyg.yangfankeji.com

List(1, 2, 3).filter(_ > 1)
来源：http://zft.jinqigufen.top

[T56] Scala：样例类
来源：http://sed.hnqzz.top

case class User(name: String, age: Int)
来源：http://mud.gogol.net.cn

[T57] Scala：模式匹配
来源：http://flw.yanxiufei.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://cfh.andypj.xyz

[T58] Scala：函数定义
来源：http://sdd.jianghu66.top

def add(a: Int, b: Int): Int = a + b
来源：http://ydx.shanyushiyangtech.top

[T59] Scala：循环
来源：http://ael.yuanzhike.top

for (i <- 1 to 10) println(i)
来源：http://asg.nwbrower.top

[T60] Scala：折叠
来源：http://hda.jqgufenzy.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://upy.ppjwa.cn

================================================================================
来源：http://zqi.daxiang520.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://xoj.sufxvd.cn

================================================================================
来源：http://glz.316326.xyz

[U01] Py：创建虚拟环境
来源：http://wdc.xziqi.cn

python -m venv .venv && source .venv/bin/activate
来源：http://cbj.ctjpmb.com

[U02] Py：导出 / 安装依赖
来源：http://fcz.cashguo.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://bwu.bjfxy.top

[U03] Py：加载 .env 配置
来源：http://cvw.gotoacloud.top

from dotenv import load_dotenv; load_dotenv()
来源：http://acp.wangdashe.top

[U04] Py：变量调试打印
来源：http://wyx.zhoulong.xyz

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://aaf.jinghuilouyu.cn

[U05] Py：列表去重且保序
来源：http://aqb.316326.xyz

list(dict.fromkeys(arr))
来源：http://xfu.yfazqb.com

[U06] Py：合并两个字典
来源：http://bip.yuxming.cn

{**a, **b}
来源：http://cme.jinqigufen.top

[U07] Py：反转字典键值
来源：http://jkd.tarul.cn

{v: k for k, v in d.items()}
来源：http://nrg.jinqigufen.top

[U08] Py：展平二维列表
来源：http://jfl.zhijiandao.cn

[y for x in nested for y in x]
来源：http://mjt.yuxming.cn

[U09] Py：字典取最大值的键
来源：http://dlj.yuanzhike.top

max(d, key=d.get)
来源：http://oer.chenzaomai.com

[U10] Py：按值排序字典
来源：http://oku.zhoulong.xyz

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://abu.smart0.xyz

[U11] Py：生成器表达式
来源：http://cbe.yanxiufei.cn

(x * 2 for x in arr)
来源：http://jec.ehwqpu.com

[U12] Py：取出现最多的 3 个元素
来源：http://nbu.ivvv.top

Counter(arr).most_common(3)
来源：http://mrh.shzxlz.cn

[U13] Py：固定长度队列
来源：http://qno.yvedp.cn

deque(maxlen=10)
来源：http://nug.zycfv.cn

[U14] Py：分组收集到列表
来源：http://vrz.gaohongyu789.top

defaultdict(list)
来源：http://ovb.shangyingyoupin.top

[U15] Py：高精度计时
来源：http://rrs.gzhubu.top

t = time.perf_counter()
来源：http://osc.zdqjudy.top

[U16] Py：命令行参数解析
来源：http://vro.zhongyouzk.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://vym.jinqigfzy.top

[U17] Py：初始化日志
来源：http://egf.tarul.cn

logging.basicConfig(level=logging.INFO)
来源：http://oog.xylfe.cn

[U18] Py：预编译正则
来源：http://ekd.xinyue.icu

pat = re.compile(r"\d+")
来源：http://tfc.haohaochexian.top

[U19] Py：正则替换带回调
来源：http://khy.ehwqpu.com

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://uaw.yj20258888.top

[U20] Py：缓存函数结果
来源：http://ypw.ehwqpu.com

@functools.lru_cache(maxsize=None)
来源：http://hlz.epnwcf.com

[U21] Py：自定义上下文管理器
来源：http://axr.xziqi.cn

@contextlib.contextmanager
来源：http://slt.sweek.top

[U22] Py：矩阵转置
来源：http://axu.jinyuanbaomall.cn

list(zip(*m))
来源：http://csh.jinqigfzy.top

[U23] Py：分块读取大文件
来源：http://abl.pycfn.com

for chunk in iter(lambda: f.read(8192), b""):
来源：http://jma.nanxinkj.top

[U24] Py：路径操作
来源：http://fwq.daria6918.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://rfk.hnxiangtu.top

[U25] Py：CSV 按字典读
来源：http://heb.yongpay.top

csv.DictReader(f)
来源：http://giw.yj20258888.top

[U26] Py：并发下载
来源：http://kev.haohaochexian.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://tgy.ywan-chungtsiang.top

[U27] Py：异步 HTTP
来源：http://pku.jqgufenzy.top

aiohttp.ClientSession() 配合 async with
来源：http://kin.yonumen.top

[U28] Py：类型别名
来源：http://jff.ywan-chungtsiang.top

UserId = int
来源：http://dho.tian-w.cn

[U29] Py：属性校验
来源：http://qfd.hnqzz.top

@property 与 @x.setter 配合
来源：http://aux.0kj1m.cn

[U30] Py：数据类
来源：http://hmx.ybcxt.top

@dataclass(slots=True)
来源：http://cmh.fktsv.cn

[U31] Py：单测
来源：http://diw.ehwqpu.com

python -m pytest -q
来源：http://pso.meibo888.top

[U32] Py：代码格式化
来源：http://ifk.chenjidiqi.icu

ruff format . && ruff check --fix .
来源：http://efw.xylfe.cn

[U33] Py：打包发布
来源：http://osh.xinyue.icu

python -m build  （依赖 pyproject.toml）
来源：http://swc.tarul.cn

[U34] Py：判断编码
来源：http://xbf.kuanghao11.cn

chardet.detect(raw)
来源：http://pcf.hysaishi.cn

[U35] Py：发送邮件
来源：http://rdi.jlsjyb.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://eax.c1oappe.top

[U36] Py：定时任务
来源：http://thf.c1oappe.top

schedule.every(10).minutes.do(job)
来源：http://aak.guowangkeji.top

[U37] Py：读写 Excel
来源：http://vwy.ehwqpu.com

pandas.read_excel / DataFrame.to_excel
来源：http://slf.fehbvm.com

[U38] Py：获取脚本所在目录
来源：http://zba.aibaodan.cn

Path(__file__).resolve().parent
来源：http://bag.nanxuanxn.top

[U39] Py：判断是否在交互环境
来源：http://ory.sxryk.cn

sys.stdout.isatty()
来源：http://wma.9152youxi.cn

[U40] Py：打印到标准错误
来源：http://nri.cqqwz.cn

print("err", file=sys.stderr)
来源：http://tmk.vqdsnc.cn

[U41] PHP：初始化 Composer 项目
来源：http://axx.shuidangran.top

composer init;  composer require guzzlehttp/guzzle
来源：http://vno.wangshuangyany.cn

[U42] PHP：PSR-4 自动加载
来源：http://ftw.yfazqb.com

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://mrf.wangdashe.top

[U43] PHP：声明命名空间
来源：http://usr.yueranfly.top

namespace App\Http;
来源：http://bcn.yangfankeji.com

[U44] PHP：开启严格类型
来源：http://xol.jyoumei.cn

declare(strict_types=1);
来源：http://dog.zhaomingkeji.xyz

[U45] PHP：类型声明与返回类型
来源：http://yml.sjlbkw.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://ihg.xuetiantiany.cn

[U46] PHP：可空类型
来源：http://ueb.epnwcf.com

?string $name = null
来源：http://zff.jqgufenzy.top

[U47] PHP：联合类型
来源：http://xkw.xingfuxueyuan.xyz

int|string $id
来源：http://xzp.shanyushiyangkeji.top

[U48] PHP：纯枚举
来源：http://dmd.ydjk.org.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://pzu.hammf.cn

[U49] PHP：只读属性
来源：http://rdp.xuetiantiany.cn

public readonly string $name
来源：http://vmf.snrcjt.cn

[U50] PHP：构造器属性提升
来源：http://aha.jyoumei.cn

public function __construct(private int $id) {}
来源：http://yqb.daria6918.cn

[U51] PHP：数组解构
来源：http://zsq.gogol.net.cn

[$a, $b] = $arr;
来源：http://uxr.sufxvd.cn

[U52] PHP：箭头函数
来源：http://fzi.cheryme.top

$double = fn($x) => $x * 2;
来源：http://xjo.shangyingyoupin.top

[U53] PHP：空合并运算符
来源：http://buk.tian-w.cn

$v = $a ?? $b ?? "default";
来源：http://sql.guowangkeji.top

[U54] PHP：空安全调用
来源：http://qkx.tianlin.xyz

$obj?->method()
来源：http://onl.yj202588.top

[U55] PHP：match 表达式
来源：http://ovz.svipenyu.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://vbc.52xcode.cn

[U56] PHP：命名参数
来源：http://nia.cucudq.cn

f(a: 1, b: 2)
来源：http://dvq.ehwqpu.com

[U57] PHP：字符串插值
来源：http://fse.feifeiyinyue.top

"值: {$a}"
来源：http://hje.havefunace.top

[U58] PHP：数组三件套
来源：http://cih.jinqigfzy.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://jpf.guowangkeji.top

[U59] PHP：自定义排序
来源：http://mif.smart0.xyz

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hvp.fanxiaobao.xyz

[U60] PHP：JSON 编解码
来源：http://obc.tian-w.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://ecy.yuanzhike.top

[U61] PHP：正则
来源：http://kuw.yueranfly.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://glb.wangshuangyany.cn

[U62] PHP：日期对象
来源：http://npf.zhijiandao.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://cij.ehwqpu.com

[U63] PHP：文件读写
来源：http://bhh.nwbrower.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://gsc.vehdjk.com

[U64] PHP：目录遍历
来源：http://hdi.hnqzz.top

glob("dir/*.php");  scandir("dir");
来源：http://vba.zycfv.cn

[U65] PHP：会话
来源：http://rqc.yangfankeji.com

session_start();  $_SESSION["uid"] = 1;
来源：http://wkz.vqdsnc.cn

[U66] PHP：设置 Cookie
来源：http://ywp.cashguo.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://kfw.ybcxt.top

[U67] PHP：处理文件上传
来源：http://dod.sysykeji.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://hag.mhx1999.top

[U68] PHP：PDO 连接
来源：http://tgy.jinghuilouyu.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://fxw.uphjek.com

[U69] PHP：PDO 预处理
来源：http://uge.svipenyu.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://tes.hnxiangtu.top

[U70] PHP：PDO 事务
来源：http://imj.jyoumei.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://irq.haohaochexian.top

[U71] PHP：抛出异常
来源：http://fpi.sjlbkw.cn

throw new RuntimeException("失败", 500);
来源：http://usb.cucudq.cn

[U72] PHP：写错误日志
来源：http://qkm.sxryk.cn

error_log("失败: " . $e->getMessage());
来源：http://bkt.0kj1m.cn

[U73] PHP：读取 ini 配置
来源：http://aqf.ctjpmb.com

parse_ini_file("config.ini", true)
来源：http://cnd.guowangkeji.top

[U74] PHP：读取环境变量
来源：http://eil.sufxvd.cn

getenv("APP_ENV") ?: "production"
来源：http://ium.sjlbkw.cn

[U75] PHP：依赖注入
来源：http://dbd.vqdsnc.cn

composer require psr/container
来源：http://dbs.tianlin.xyz

[U76] PHP：简单路由
来源：http://rts.zhiwuduotai.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://awa.chenjidiqi.icu

[U77] PHP：模板渲染
来源：http://idg.uphjek.com

composer require twig/twig
来源：http://qtq.dianchejie.cn

[U78] PHP：单元测试
来源：http://mue.uphjek.com

composer require --dev phpunit/phpunit
来源：http://sly.yanxiufei.cn

[U79] PHP：静态分析
来源：http://boh.yuxming.cn

composer require --dev phpstan/phpstan
来源：http://ufr.cucudq.cn

[U80] PHP：代码规范修复
来源：http://ehc.xingfuxueyuan.xyz

composer require --dev friendsofphp/php-cs-fixer
来源：http://hdi.ybcxt.top

[U81] JS：初始化项目
来源：http://pcx.sxryk.cn

npm init -y;  npm i express
来源：http://xff.shangyingyoupin.top

[U82] JS：package.json 脚本
来源：http://ido.daria6918.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://ikb.zdqjudy.top

[U83] JS：ES Module 导入导出
来源：http://yez.9152youxi.cn

export const a = 1;  import { a } from "./m.js";
来源：http://bii.ybcxt.top

[U84] JS：CommonJS 写法
来源：http://avz.xuanzx.com

module.exports = { a };  const { a } = require("./m");
来源：http://caq.bbcook.cn

[U85] JS：可选链
来源：http://chr.yj202588.top

a?.b?.c
来源：http://enh.chenzaomai.com

[U86] JS：空值合并
来源：http://zhj.feifeiyinyue.top

a ?? b
来源：http://lux.tian-w.cn

[U87] JS：解构默认值
来源：http://vnw.sweek.top

const { a = 1, b = 2 } = obj;
来源：http://ujh.9152youxi.cn

[U88] JS：对象展开合并
来源：http://rau.0kj1m.cn

{ ...a, ...b }
来源：http://bxf.zhongyouzk.top

[U89] JS：数组去重
来源：http://bke.hywenlv.cn

[...new Set(arr)]
来源：http://slm.shzxlz.cn

[U90] JS：数字数组排序
来源：http://hdr.pengpengdd.cyou

[...arr].sort((a, b) => a - b)
来源：http://ems.hcnkem.com

[U91] JS：对象键值遍历
来源：http://tmb.jiagoushi.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://kfs.ivvv.top

[U92] JS：深拷贝
来源：http://cfo.jinqigfzy.top

structuredClone(obj)
来源：http://djo.daxiang520.top

[U93] JS：模板字符串
来源：http://cjf.gaohongyu789.top

`共 ${n} 条`
来源：http://xgx.sjlbkw.cn

[U94] JS：箭头函数
来源：http://gbq.ehwqpu.com

const double = x => x * 2;
来源：http://xcc.yangfankeji.com

[U95] JS：Promise 包装
来源：http://sib.hysaishi.cn

new Promise((resolve, reject) => {})
来源：http://ucf.ydjk.org.cn

[U96] JS：async/await 与异常
来源：http://izg.pengpengdd.cyou

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://ldv.aibaodan.cn

[U97] JS：并发请求
来源：http://uid.wangshuangyany.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://uuz.nanxuanxn.top

[U98] JS：fetch 带 JSON
来源：http://xey.hfpthk.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://ozv.daria6918.cn

[U99] JS：事件监听
来源：http://git.tian-w.cn

el.addEventListener("click", e => {})
来源：http://dha.ctjpmb.com

[U100] JS：DOM 查询
来源：http://lpt.gotoacloud.top

document.querySelector(".item")
来源：http://qjl.ydzc1.top

[U101] JS：classList 操作
来源：http://nah.ppjwa.cn

el.classList.toggle("active")
来源：http://zhk.hesvh.cn

[U102] JS：本地存储
来源：http://mxj.jlsjyb.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://mdf.zhoulong.xyz

[U103] JS：定时器
来源：http://med.gogol.net.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://vlq.havefunace.top

[U104] JS：防抖
来源：http://fms.jqgufenzy.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://qgr.jinqigufen.top

[U105] JS：节流
来源：http://ayo.nanxuanxn.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://ixb.uphjek.com

[U106] JS：日期格式化
来源：http://nix.fengsongda.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://vwd.zhixingplan.top

[U107] JS：数字千分位
来源：http://zsm.xuetiantiany.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://ucw.chenlongwang.top

[U108] JS：随机整数
来源：http://akg.redwolf501.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://pkk.svipenyu.cn

[U109] JS：数组分组
来源：http://kgs.xylfe.cn

Object.groupBy(arr, x => x.type)
来源：http://dki.zhaomingkeji.xyz

[U110] JS：数组分块
来源：http://otp.sweek.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://iyt.bjfxy.top

[U111] JS：对象转 Map
来源：http://pvo.ctjpmb.com

new Map(Object.entries(obj))
来源：http://zyr.meibo888.top

[U112] JS：字符串补位
来源：http://tpi.shangyingyoupin.top

"7".padStart(3, "0")
来源：http://bih.gotoacloud.top

[U113] JS：正则替换全部
来源：http://sie.gzhubu.top

s.replaceAll("a", "b")
来源：http://vqj.fehbvm.com

[U114] JS：JSON 深比较
来源：http://jcs.sxryk.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://rin.shangyingyoupin.top

[U115] JS：生成 UUID
来源：http://fqa.shanyushiyangtech.top

crypto.randomUUID()
来源：http://upl.cheryme.top

[U116] JS：类型检查（JSDoc）
来源：http://hhz.ydzc1.top

/** @param {string} name */ function f(name) {}
来源：http://mmi.nanxinkj.top


<!-- 参考信息 -->