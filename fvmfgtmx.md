代发 wailian999

[T31] Lua：Hello World
来源：http://kde.dashuyun.cn

print("Hello")
来源：http://hvl.meibo888.top

[T32] Lua：局部变量
来源：http://dfj.dashuyun.cn

local a = 1
来源：http://inc.andypj.xyz

[T33] Lua：表（数组）
来源：http://jdr.fzhhl.top

local t = {1, 2, 3};  t[4] = 4
来源：http://wag.zycfv.cn

[T34] Lua：遍历表
来源：http://kva.shanyushiyangtech.top

for i, v in ipairs(t) do print(i, v) end
来源：http://nce.0kj1m.cn

[T35] Lua：字典表
来源：http://igq.jianghu66.top

local d = { a = 1 };  d.b = 2
来源：http://xhv.vehdjk.com

[T36] Lua：函数
来源：http://slf.yanxiufei.cn

function add(a, b) return a + b end
来源：http://omy.ydzc1.top

[T37] Lua：字符串拼接
来源：http://rbf.ybcxt.top

"a" .. "b"
来源：http://xpo.cheryme.top

[T38] Lua：条件
来源：http://kxg.aibaodan.cn

if x > 0 then print("正") end
来源：http://kcw.zhoulong.xyz

[T39] Lua：模式匹配
来源：http://fbu.sufxvd.cn

string.find(s, "%d+")
来源：http://klm.fzhhl.top

[T40] Lua：元表
来源：http://qza.gaohongyu789.top

setmetatable({}, { __index = base })
来源：http://kaq.mhx1999.top

[T41] Perl：Hello World
来源：http://lay.fanxiaobao.xyz

print "Hello\n";
来源：http://hbu.dashuyun.cn

[T42] Perl：变量类型
来源：http://vxi.yuanzhike.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://daa.nanxuanxn.top

[T43] Perl：字符串插值
来源：http://juj.meibo888.top

"值: $a"
来源：http://xce.gzhubu.top

[T44] Perl：条件
来源：http://wyb.xziqi.cn

if ($a > 0) { print "正"; }
来源：http://vfv.uphjek.com

[T45] Perl：数组遍历
来源：http://uff.yj20258888.top

for my $x (@arr) { print $x; }
来源：http://slj.hongshengwenyu.top

[T46] Perl：哈希操作
来源：http://jpj.dashuyun.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://lpj.cucudq.cn

[T47] Perl：正则捕获
来源：http://vvi.ivvv.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://bcw.sufxvd.cn

[T48] Perl：正则替换
来源：http://lgn.zhixingplan.top

$s =~ s/old/new/g;
来源：http://qzc.c1oappe.top

[T49] Perl：函数
来源：http://ytn.andypj.xyz

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://gse.yj20258.top

[T50] Perl：逐行读文件
来源：http://ezc.jqgfzy.top

open my $fh, "<", "a.txt" or die $!;
来源：http://fwp.jinqigufen.top

while (my $line = <$fh>) { print $line; }
来源：http://eus.iojbl.cn

[T51] Scala：Hello World
来源：http://vkf.jinqigufen.top

println("Hello")
来源：http://pft.ybcxt.top

[T52] Scala：变量
来源：http://flp.bjfxy.top

val a = 1;  var b = 2
来源：http://dpn.yj20258888.top

[T53] Scala：字符串插值
来源：http://rui.yfazqb.com

s"值: $b"
来源：http://xyw.ydjk.org.cn

[T54] Scala：集合映射
来源：http://auf.xingfuxueyuan.xyz

List(1, 2, 3).map(_ * 2)
来源：http://flr.shangyingyoupin.top

[T55] Scala：集合过滤
来源：http://fzh.zhijiandao.cn

List(1, 2, 3).filter(_ > 1)
来源：http://eyw.guannengcc.top

[T56] Scala：样例类
来源：http://uxd.daria6918.cn

case class User(name: String, age: Int)
来源：http://gij.yvedp.cn

[T57] Scala：模式匹配
来源：http://zpq.haohaochexian.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://soo.chenlongwang.top

[T58] Scala：函数定义
来源：http://xpp.ydzc1.top

def add(a: Int, b: Int): Int = a + b
来源：http://mgh.yj20258888.top

[T59] Scala：循环
来源：http://tak.52xcode.cn

for (i <- 1 to 10) println(i)
来源：http://xjr.jinqigfzy.top

[T60] Scala：折叠
来源：http://jwr.ydjk.org.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://rjj.tianlin.xyz

================================================================================
来源：http://cvg.jinghuilouyu.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://bgx.cashguo.top

================================================================================
来源：http://ccb.pycfn.com

[U01] Py：创建虚拟环境
来源：http://oei.wangdashe.top

python -m venv .venv && source .venv/bin/activate
来源：http://lfm.guowangkeji.top

[U02] Py：导出 / 安装依赖
来源：http://qin.fehbvm.com

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://cbo.andypj.xyz

[U03] Py：加载 .env 配置
来源：http://ueh.jqgufenzy.top

from dotenv import load_dotenv; load_dotenv()
来源：http://oms.fktsv.cn

[U04] Py：变量调试打印
来源：http://gey.yangfankeji.com

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://ext.xuanzx.com

[U05] Py：列表去重且保序
来源：http://jay.redwolf501.top

list(dict.fromkeys(arr))
来源：http://ltp.andypj.xyz

[U06] Py：合并两个字典
来源：http://udb.yongpay.top

{**a, **b}
来源：http://rrf.shangyingyoupin.top

[U07] Py：反转字典键值
来源：http://qrs.sysykeji.top

{v: k for k, v in d.items()}
来源：http://sgn.pengpengdd.cyou

[U08] Py：展平二维列表
来源：http://mdc.hongshengwenyu.top

[y for x in nested for y in x]
来源：http://ycw.nwbrower.top

[U09] Py：字典取最大值的键
来源：http://aqv.jyoumei.cn

max(d, key=d.get)
来源：http://ggh.shanyushiyangkeji.top

[U10] Py：按值排序字典
来源：http://xmy.shuidangran.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://sdj.andypj.xyz

[U11] Py：生成器表达式
来源：http://bvc.yj202588.top

(x * 2 for x in arr)
来源：http://yyq.hongshengwenyu.top

[U12] Py：取出现最多的 3 个元素
来源：http://hmo.shanyushiyangkeji.top

Counter(arr).most_common(3)
来源：http://mzj.ydzc1.top

[U13] Py：固定长度队列
来源：http://tig.jlsjyb.cn

deque(maxlen=10)
来源：http://glo.gaohongyu789.top

[U14] Py：分组收集到列表
来源：http://eha.chenjidiqi.icu

defaultdict(list)
来源：http://swc.pycfn.com

[U15] Py：高精度计时
来源：http://iju.zdqjudy.top

t = time.perf_counter()
来源：http://omu.jianghu66.top

[U16] Py：命令行参数解析
来源：http://knv.jyoumei.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://ghj.hongshengwenyu.top

[U17] Py：初始化日志
来源：http://rnc.sxryk.cn

logging.basicConfig(level=logging.INFO)
来源：http://krr.sxryk.cn

[U18] Py：预编译正则
来源：http://hht.bjfxy.top

pat = re.compile(r"\d+")
来源：http://crq.yj202588.top

[U19] Py：正则替换带回调
来源：http://qzo.gaohongyu789.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://tsr.hesvh.cn

[U20] Py：缓存函数结果
来源：http://wwo.iojbl.cn

@functools.lru_cache(maxsize=None)
来源：http://wfy.sjlbkw.cn

[U21] Py：自定义上下文管理器
来源：http://udv.hcnkem.com

@contextlib.contextmanager
来源：http://wfp.zhiwuduotai.top

[U22] Py：矩阵转置
来源：http://dob.shanyushiyangtech.top

list(zip(*m))
来源：http://ecr.xziqi.cn

[U23] Py：分块读取大文件
来源：http://xis.svipenyu.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://dls.zhaomingkeji.xyz

[U24] Py：路径操作
来源：http://ayp.0kj1m.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://rlo.havefunace.top

[U25] Py：CSV 按字典读
来源：http://srh.zhoulong.xyz

csv.DictReader(f)
来源：http://kns.jyoumei.cn

[U26] Py：并发下载
来源：http://luz.birdmap.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://gqf.hysaishi.cn

[U27] Py：异步 HTTP
来源：http://pbx.shanyushiyangtech.top

aiohttp.ClientSession() 配合 async with
来源：http://kmk.yongpay.top

[U28] Py：类型别名
来源：http://aod.nwbrower.top

UserId = int
来源：http://vqw.chenzaomai.com

[U29] Py：属性校验
来源：http://ttu.yvedp.cn

@property 与 @x.setter 配合
来源：http://qew.ivvv.top

[U30] Py：数据类
来源：http://mkq.sysykeji.top

@dataclass(slots=True)
来源：http://zds.pengpengdd.cyou

[U31] Py：单测
来源：http://rob.gotoacloud.top

python -m pytest -q
来源：http://pml.zhaomingkeji.xyz

[U32] Py：代码格式化
来源：http://ngd.fanxiaobao.xyz

ruff format . && ruff check --fix .
来源：http://uyr.xuanzx.com

[U33] Py：打包发布
来源：http://qyu.redwolf501.top

python -m build  （依赖 pyproject.toml）
来源：http://msr.tian-w.cn

[U34] Py：判断编码
来源：http://obp.cdnleiting.top

chardet.detect(raw)
来源：http://rqv.chenjidiqi.icu

[U35] Py：发送邮件
来源：http://zbv.havefunace.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://wec.aibaodan.cn

[U36] Py：定时任务
来源：http://bty.ehwqpu.com

schedule.every(10).minutes.do(job)
来源：http://nyj.bbcook.cn

[U37] Py：读写 Excel
来源：http://hfu.hnxiangtu.top

pandas.read_excel / DataFrame.to_excel
来源：http://uue.quarkkingdee.top

[U38] Py：获取脚本所在目录
来源：http://pzl.wangdashe.top

Path(__file__).resolve().parent
来源：http://vru.dianchejie.cn

[U39] Py：判断是否在交互环境
来源：http://mrj.zycfv.cn

sys.stdout.isatty()
来源：http://trb.sysykeji.top

[U40] Py：打印到标准错误
来源：http://xyk.shuidangran.top

print("err", file=sys.stderr)
来源：http://tak.aizwys.cn

[U41] PHP：初始化 Composer 项目
来源：http://jbg.sufxvd.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://viw.yj20258.top

[U42] PHP：PSR-4 自动加载
来源：http://bsr.daria6918.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://uey.yfazqb.com

[U43] PHP：声明命名空间
来源：http://wot.zycfv.cn

namespace App\Http;
来源：http://bte.hysaishi.cn

[U44] PHP：开启严格类型
来源：http://ykz.aibaodan.cn

declare(strict_types=1);
来源：http://vky.guowangkeji.top

[U45] PHP：类型声明与返回类型
来源：http://vhw.pycfn.com

function add(int $a, int $b): int { return $a + $b; }
来源：http://rko.hfpthk.cn

[U46] PHP：可空类型
来源：http://ark.zdbjq.cn

?string $name = null
来源：http://lbw.shangyingyoupin.top

[U47] PHP：联合类型
来源：http://bot.zhengqikj.top

int|string $id
来源：http://ypq.ydjk.org.cn

[U48] PHP：纯枚举
来源：http://uys.mhx1999.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://wvg.zhengqikj.top

[U49] PHP：只读属性
来源：http://pqb.hfpthk.cn

public readonly string $name
来源：http://plw.zycfv.cn

[U50] PHP：构造器属性提升
来源：http://vng.hysaishi.cn

public function __construct(private int $id) {}
来源：http://niu.snrcjt.cn

[U51] PHP：数组解构
来源：http://gqx.pycfn.com

[$a, $b] = $arr;
来源：http://dyu.jqgufenzy.top

[U52] PHP：箭头函数
来源：http://mgx.zhoulong.xyz

$double = fn($x) => $x * 2;
来源：http://mkf.xylfe.cn

[U53] PHP：空合并运算符
来源：http://wid.dianchejie.cn

$v = $a ?? $b ?? "default";
来源：http://mbm.epnwcf.com

[U54] PHP：空安全调用
来源：http://vei.ydzc1.top

$obj?->method()
来源：http://lzd.uphjek.com

[U55] PHP：match 表达式
来源：http://orz.havefunace.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://gvh.gaohongyu789.top

[U56] PHP：命名参数
来源：http://bvo.wangshuangyany.cn

f(a: 1, b: 2)
来源：http://itd.shzxlz.cn

[U57] PHP：字符串插值
来源：http://qux.jqgfzy.top

"值: {$a}"
来源：http://xbo.fktsv.cn

[U58] PHP：数组三件套
来源：http://cyk.svipenyu.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://jjc.0kj1m.cn

[U59] PHP：自定义排序
来源：http://hfm.tianlin.xyz

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://nej.fktsv.cn

[U60] PHP：JSON 编解码
来源：http://uwo.wangshuangyany.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://eho.ydjk.org.cn

[U61] PHP：正则
来源：http://zhs.zycfv.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://szd.fanxiaobao.xyz

[U62] PHP：日期对象
来源：http://kbs.ppjwa.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://bub.jinqigufen.top

[U63] PHP：文件读写
来源：http://emr.pycfn.com

file_get_contents($f);  file_put_contents($f, $data);
来源：http://oyn.ywan-chungtsiang.top

[U64] PHP：目录遍历
来源：http://hlb.daria6918.cn

glob("dir/*.php");  scandir("dir");
来源：http://xpj.meibo888.top

[U65] PHP：会话
来源：http://djf.zhijiandao.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://qnp.yuanzhike.top

[U66] PHP：设置 Cookie
来源：http://koj.fanxiaobao.xyz

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://uat.yfazqb.com

[U67] PHP：处理文件上传
来源：http://bic.guowangkeji.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://fgc.ppjwa.cn

[U68] PHP：PDO 连接
来源：http://xyo.yj20258.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://zey.zhongyouzk.top

[U69] PHP：PDO 预处理
来源：http://hzb.cdnleiting.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://rbp.ydjk.org.cn

[U70] PHP：PDO 事务
来源：http://urd.zycfv.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://bqv.redwolf501.top

[U71] PHP：抛出异常
来源：http://ito.xylfe.cn

throw new RuntimeException("失败", 500);
来源：http://jim.ywan-chungtsiang.top

[U72] PHP：写错误日志
来源：http://uxc.jianghu66.top

error_log("失败: " . $e->getMessage());
来源：http://itv.quarkkingdee.top

[U73] PHP：读取 ini 配置
来源：http://hgc.gzhubu.top

parse_ini_file("config.ini", true)
来源：http://xjo.jiagoushi.top

[U74] PHP：读取环境变量
来源：http://bsw.zhengqikj.top

getenv("APP_ENV") ?: "production"
来源：http://hkr.cdnleiting.top

[U75] PHP：依赖注入
来源：http://lhe.fehbvm.com

composer require psr/container
来源：http://ntq.xuanzx.com

[U76] PHP：简单路由
来源：http://uxw.hammf.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://odd.daria6918.cn

[U77] PHP：模板渲染
来源：http://vei.birdmap.top

composer require twig/twig
来源：http://zvc.hcnkem.com

[U78] PHP：单元测试
来源：http://wcd.chenjidiqi.icu

composer require --dev phpunit/phpunit
来源：http://irq.0kj1m.cn

[U79] PHP：静态分析
来源：http://pdm.jinyuanbaomall.cn

composer require --dev phpstan/phpstan
来源：http://uph.wangdashe.top

[U80] PHP：代码规范修复
来源：http://csz.jlsjyb.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://cyt.gogol.net.cn

[U81] JS：初始化项目
来源：http://mqu.ehwqpu.com

npm init -y;  npm i express
来源：http://wet.fehbvm.com

[U82] JS：package.json 脚本
来源：http://hay.chenjidiqi.icu

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://hpu.hammf.cn

[U83] JS：ES Module 导入导出
来源：http://qbx.uphjek.com

export const a = 1;  import { a } from "./m.js";
来源：http://ehv.sweek.top

[U84] JS：CommonJS 写法
来源：http://lfv.havefunace.top

module.exports = { a };  const { a } = require("./m");
来源：http://uuy.fktsv.cn

[U85] JS：可选链
来源：http://neg.xingfuxueyuan.xyz

a?.b?.c
来源：http://qdu.yongpay.top

[U86] JS：空值合并
来源：http://fec.hnxiangtu.top

a ?? b
来源：http://idl.epnwcf.com

[U87] JS：解构默认值
来源：http://vmk.yuanzhike.top

const { a = 1, b = 2 } = obj;
来源：http://yup.wangdashe.top

[U88] JS：对象展开合并
来源：http://gno.gzhubu.top

{ ...a, ...b }
来源：http://thu.yj20258.top

[U89] JS：数组去重
来源：http://piq.jqgufenzy.top

[...new Set(arr)]
来源：http://wlo.0kj1m.cn

[U90] JS：数字数组排序
来源：http://yra.yj20258888.top

[...arr].sort((a, b) => a - b)
来源：http://jkd.fengsongda.top

[U91] JS：对象键值遍历
来源：http://pdc.nanxuanxn.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://vik.hysaishi.cn

[U92] JS：深拷贝
来源：http://nph.hfpthk.cn

structuredClone(obj)
来源：http://skb.yuxming.cn

[U93] JS：模板字符串
来源：http://pbd.gotoacloud.top

`共 ${n} 条`
来源：http://oua.zhoulong.xyz

[U94] JS：箭头函数
来源：http://bnr.havefunace.top

const double = x => x * 2;
来源：http://nzg.ivvv.top

[U95] JS：Promise 包装
来源：http://cis.shanyushiyangkeji.top

new Promise((resolve, reject) => {})
来源：http://qzf.ctjpmb.com

[U96] JS：async/await 与异常
来源：http://gsn.epnwcf.com

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://ohs.cqqwz.cn

[U97] JS：并发请求
来源：http://hzr.birdmap.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://lih.hfpthk.cn

[U98] JS：fetch 带 JSON
来源：http://zqt.nwbrower.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://mrf.zycfv.cn

[U99] JS：事件监听
来源：http://fle.zhixingplan.top

el.addEventListener("click", e => {})
来源：http://kwb.hnxiangtu.top

[U100] JS：DOM 查询
来源：http://rmb.jinqigufen.top

document.querySelector(".item")
来源：http://hwb.hongshengwenyu.top

[U101] JS：classList 操作
来源：http://omy.xuanzx.com

el.classList.toggle("active")
来源：http://dua.ydzc1.top

[U102] JS：本地存储
来源：http://kor.aibaodan.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://fsc.316326.xyz

[U103] JS：定时器
来源：http://ftq.haohaochexian.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://dpc.gogol.net.cn

[U104] JS：防抖
来源：http://tqj.kuanghao11.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://dmh.zhijiandao.cn

[U105] JS：节流
来源：http://qzn.hongshengwenyu.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://ohn.xuetiantiany.cn

[U106] JS：日期格式化
来源：http://pnt.meibo888.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://nrq.sysykeji.top

[U107] JS：数字千分位
来源：http://yyh.hammf.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://spp.tarul.cn

[U108] JS：随机整数
来源：http://cuu.yangfankeji.com

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://igr.nwbrower.top

[U109] JS：数组分组
来源：http://myb.mhx1999.top

Object.groupBy(arr, x => x.type)
来源：http://atd.yongpay.top

[U110] JS：数组分块
来源：http://lrp.chenjidiqi.icu

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://buf.sjlbkw.cn

[U111] JS：对象转 Map
来源：http://gae.cdnleiting.top

new Map(Object.entries(obj))
来源：http://afk.hywenlv.cn

[U112] JS：字符串补位
来源：http://qli.zdqjudy.top

"7".padStart(3, "0")
来源：http://jza.yuxming.cn

[U113] JS：正则替换全部
来源：http://yrh.tanke756.top

s.replaceAll("a", "b")
来源：http://ync.andypj.xyz

[U114] JS：JSON 深比较
来源：http://nyp.gzhubu.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://giv.tianlin.xyz

[U115] JS：生成 UUID
来源：http://ktd.zhengqikj.top

crypto.randomUUID()
来源：http://ckn.ywan-chungtsiang.top

[U116] JS：类型检查（JSDoc）
来源：http://szz.zdbjq.cn

/** @param {string} name */ function f(name) {}
来源：http://wff.tanke756.top

[U117] JS：单元测试
来源：http://msg.pycfn.com

npm i -D vitest;  npx vitest
来源：http://stl.xingfuxueyuan.xyz

[U118] JS：开发服务器
来源：http://qwc.epnwcf.com

npm i -D vite;  npx vite
来源：http://xzx.xinyue.icu


<!-- 参考信息 -->