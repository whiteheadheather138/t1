代发 wailian999

[T37] Lua：字符串拼接
来源：http://hfr.hfpthk.cn

"a" .. "b"
来源：http://ykr.ppjwa.cn

[T38] Lua：条件
来源：http://acc.daria6918.cn

if x > 0 then print("正") end
来源：http://kau.ywan-chungtsiang.top

[T39] Lua：模式匹配
来源：http://fdt.fehbvm.com

string.find(s, "%d+")
来源：http://bzf.hysaishi.cn

[T40] Lua：元表
来源：http://jza.yfazqb.com

setmetatable({}, { __index = base })
来源：http://nyh.andypj.xyz

[T41] Perl：Hello World
来源：http://oci.guowangkeji.top

print "Hello\n";
来源：http://cvx.jinqigfzy.top

[T42] Perl：变量类型
来源：http://sqh.hesvh.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://lcb.cdnleiting.top

[T43] Perl：字符串插值
来源：http://alo.pengpengdd.cyou

"值: $a"
来源：http://qnu.yuanzhike.top

[T44] Perl：条件
来源：http://fpo.havefunace.top

if ($a > 0) { print "正"; }
来源：http://xxq.jqgufenzy.top

[T45] Perl：数组遍历
来源：http://fyh.xuetiantiany.cn

for my $x (@arr) { print $x; }
来源：http://rhe.ctjpmb.com

[T46] Perl：哈希操作
来源：http://sxo.ppjwa.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://idi.haohaochexian.top

[T47] Perl：正则捕获
来源：http://vsx.tianlin.xyz

if ($s =~ /(\d+)/) { print $1; }
来源：http://mtv.pengpengdd.cyou

[T48] Perl：正则替换
来源：http://eon.0kj1m.cn

$s =~ s/old/new/g;
来源：http://rhm.c1oappe.top

[T49] Perl：函数
来源：http://umz.chenjidiqi.icu

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://fkh.quarkkingdee.top

[T50] Perl：逐行读文件
来源：http://mcb.yfazqb.com

open my $fh, "<", "a.txt" or die $!;
来源：http://lth.zhiwuduotai.top

while (my $line = <$fh>) { print $line; }
来源：http://sbf.gogol.net.cn

[T51] Scala：Hello World
来源：http://fxu.nwbrower.top

println("Hello")
来源：http://zdi.jianghu66.top

[T52] Scala：变量
来源：http://aud.xinyue.icu

val a = 1;  var b = 2
来源：http://cxj.zhengqikj.top

[T53] Scala：字符串插值
来源：http://aaf.hywenlv.cn

s"值: $b"
来源：http://fjn.daxiang520.top

[T54] Scala：集合映射
来源：http://fty.svipenyu.cn

List(1, 2, 3).map(_ * 2)
来源：http://gbe.cqqwz.cn

[T55] Scala：集合过滤
来源：http://koa.xylfe.cn

List(1, 2, 3).filter(_ > 1)
来源：http://hvn.zhaomingkeji.xyz

[T56] Scala：样例类
来源：http://xvf.gotoacloud.top

case class User(name: String, age: Int)
来源：http://kww.dianchejie.cn

[T57] Scala：模式匹配
来源：http://fin.yueranfly.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://zqb.bbcook.cn

[T58] Scala：函数定义
来源：http://uxu.epnwcf.com

def add(a: Int, b: Int): Int = a + b
来源：http://vln.xuetiantiany.cn

[T59] Scala：循环
来源：http://kfg.hnxiangtu.top

for (i <- 1 to 10) println(i)
来源：http://bnr.havefunace.top

[T60] Scala：折叠
来源：http://grv.fzhhl.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://fus.zhixingplan.top

================================================================================
来源：http://eso.yongpay.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://jrl.andypj.xyz

================================================================================
来源：http://qun.tarul.cn

[U01] Py：创建虚拟环境
来源：http://pqa.guannengcc.top

python -m venv .venv && source .venv/bin/activate
来源：http://hui.ctjpmb.com

[U02] Py：导出 / 安装依赖
来源：http://kce.ctjpmb.com

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://ioy.ywan-chungtsiang.top

[U03] Py：加载 .env 配置
来源：http://mzx.xylfe.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://zaj.yvedp.cn

[U04] Py：变量调试打印
来源：http://jgb.guowangkeji.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://vuh.pengpengdd.cyou

[U05] Py：列表去重且保序
来源：http://zll.guowangkeji.top

list(dict.fromkeys(arr))
来源：http://qyg.xziqi.cn

[U06] Py：合并两个字典
来源：http://pol.andypj.xyz

{**a, **b}
来源：http://gzf.hysaishi.cn

[U07] Py：反转字典键值
来源：http://jlk.sxryk.cn

{v: k for k, v in d.items()}
来源：http://mac.xziqi.cn

[U08] Py：展平二维列表
来源：http://sub.yvedp.cn

[y for x in nested for y in x]
来源：http://iik.xingfuxueyuan.xyz

[U09] Py：字典取最大值的键
来源：http://agx.sysykeji.top

max(d, key=d.get)
来源：http://mhv.feifeiyinyue.top

[U10] Py：按值排序字典
来源：http://foq.jlsjyb.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://gku.xylfe.cn

[U11] Py：生成器表达式
来源：http://uot.chenjidiqi.icu

(x * 2 for x in arr)
来源：http://car.tarul.cn

[U12] Py：取出现最多的 3 个元素
来源：http://usm.fzhhl.top

Counter(arr).most_common(3)
来源：http://hrr.xuanzx.com

[U13] Py：固定长度队列
来源：http://ird.cdnleiting.top

deque(maxlen=10)
来源：http://tut.yongpay.top

[U14] Py：分组收集到列表
来源：http://pps.yfazqb.com

defaultdict(list)
来源：http://ljn.sysykeji.top

[U15] Py：高精度计时
来源：http://xee.xziqi.cn

t = time.perf_counter()
来源：http://hdy.cucudq.cn

[U16] Py：命令行参数解析
来源：http://woo.c1oappe.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://tuf.hywenlv.cn

[U17] Py：初始化日志
来源：http://mky.xuanzx.com

logging.basicConfig(level=logging.INFO)
来源：http://vih.nanxuanxn.top

[U18] Py：预编译正则
来源：http://xko.tanke756.top

pat = re.compile(r"\d+")
来源：http://vbb.uphjek.com

[U19] Py：正则替换带回调
来源：http://fjr.chenzaomai.com

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://ekt.yj20258.top

[U20] Py：缓存函数结果
来源：http://qkj.sjlbkw.cn

@functools.lru_cache(maxsize=None)
来源：http://zkf.jinghuilouyu.cn

[U21] Py：自定义上下文管理器
来源：http://isi.sufxvd.cn

@contextlib.contextmanager
来源：http://pgv.cdnleiting.top

[U22] Py：矩阵转置
来源：http://ejf.gogol.net.cn

list(zip(*m))
来源：http://ume.zdqjudy.top

[U23] Py：分块读取大文件
来源：http://zpa.jianghu66.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://zyj.fehbvm.com

[U24] Py：路径操作
来源：http://clk.bbcook.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://par.sjlbkw.cn

[U25] Py：CSV 按字典读
来源：http://nip.jlsjyb.cn

csv.DictReader(f)
来源：http://fhq.gogol.net.cn

[U26] Py：并发下载
来源：http://ytd.hywenlv.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://yua.iojbl.cn

[U27] Py：异步 HTTP
来源：http://mwe.52xcode.cn

aiohttp.ClientSession() 配合 async with
来源：http://fnk.smart0.xyz

[U28] Py：类型别名
来源：http://wlm.zhaomingkeji.xyz

UserId = int
来源：http://hrp.tianlin.xyz

[U29] Py：属性校验
来源：http://lvp.shanyushiyangtech.top

@property 与 @x.setter 配合
来源：http://dyo.cqqwz.cn

[U30] Py：数据类
来源：http://zmq.hywenlv.cn

@dataclass(slots=True)
来源：http://vtw.cheryme.top

[U31] Py：单测
来源：http://gdr.fehbvm.com

python -m pytest -q
来源：http://zdo.epnwcf.com

[U32] Py：代码格式化
来源：http://qdf.havefunace.top

ruff format . && ruff check --fix .
来源：http://rlh.svipenyu.cn

[U33] Py：打包发布
来源：http://pya.sufxvd.cn

python -m build  （依赖 pyproject.toml）
来源：http://kfv.jinyuanbaomall.cn

[U34] Py：判断编码
来源：http://vvd.fktsv.cn

chardet.detect(raw)
来源：http://icb.guowangkeji.top

[U35] Py：发送邮件
来源：http://ubs.cdnleiting.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://boi.gaohongyu789.top

[U36] Py：定时任务
来源：http://fif.chenlongwang.top

schedule.every(10).minutes.do(job)
来源：http://iws.cucudq.cn

[U37] Py：读写 Excel
来源：http://xvm.tarul.cn

pandas.read_excel / DataFrame.to_excel
来源：http://kon.bjfxy.top

[U38] Py：获取脚本所在目录
来源：http://kqu.havefunace.top

Path(__file__).resolve().parent
来源：http://prp.iojbl.cn

[U39] Py：判断是否在交互环境
来源：http://mdt.chenzaomai.com

sys.stdout.isatty()
来源：http://lwo.tianlin.xyz

[U40] Py：打印到标准错误
来源：http://eki.jlsjyb.cn

print("err", file=sys.stderr)
来源：http://atp.nwbrower.top

[U41] PHP：初始化 Composer 项目
来源：http://ayr.fzhhl.top

composer init;  composer require guzzlehttp/guzzle
来源：http://ent.iojbl.cn

[U42] PHP：PSR-4 自动加载
来源：http://ovz.jinqigufen.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://ttd.fehbvm.com

[U43] PHP：声明命名空间
来源：http://fol.vqdsnc.cn

namespace App\Http;
来源：http://xod.sjlbkw.cn

[U44] PHP：开启严格类型
来源：http://aqd.yfazqb.com

declare(strict_types=1);
来源：http://vad.zdqjudy.top

[U45] PHP：类型声明与返回类型
来源：http://smx.havefunace.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://qlk.yanxiufei.cn

[U46] PHP：可空类型
来源：http://tji.zdbjq.cn

?string $name = null
来源：http://bci.sweek.top

[U47] PHP：联合类型
来源：http://upb.aizwys.cn

int|string $id
来源：http://hxk.cdnleiting.top

[U48] PHP：纯枚举
来源：http://djn.gzhubu.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://myb.vqdsnc.cn

[U49] PHP：只读属性
来源：http://rej.haohaochexian.top

public readonly string $name
来源：http://tda.redwolf501.top

[U50] PHP：构造器属性提升
来源：http://bbv.zhoulong.xyz

public function __construct(private int $id) {}
来源：http://aao.jqgufenzy.top

[U51] PHP：数组解构
来源：http://nqp.hfpthk.cn

[$a, $b] = $arr;
来源：http://esz.daria6918.cn

[U52] PHP：箭头函数
来源：http://biv.epnwcf.com

$double = fn($x) => $x * 2;
来源：http://xtb.cdnleiting.top

[U53] PHP：空合并运算符
来源：http://hrl.hnqzz.top

$v = $a ?? $b ?? "default";
来源：http://fbc.jiagoushi.top

[U54] PHP：空安全调用
来源：http://lvn.yfazqb.com

$obj?->method()
来源：http://lxn.meibo888.top

[U55] PHP：match 表达式
来源：http://pjb.meibo888.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://zux.nanxinkj.top

[U56] PHP：命名参数
来源：http://rir.xuanzx.com

f(a: 1, b: 2)
来源：http://jgm.xylfe.cn

[U57] PHP：字符串插值
来源：http://neu.smart0.xyz

"值: {$a}"
来源：http://gwt.iojbl.cn

[U58] PHP：数组三件套
来源：http://sij.shzxlz.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://ilr.yuanzhike.top

[U59] PHP：自定义排序
来源：http://zys.sysykeji.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://rfh.9152youxi.cn

[U60] PHP：JSON 编解码
来源：http://fmf.yuanzhike.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://iii.xuanzx.com

[U61] PHP：正则
来源：http://hpi.daxiang520.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://chz.0kj1m.cn

[U62] PHP：日期对象
来源：http://hfu.jinqigufen.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://isy.svipenyu.cn

[U63] PHP：文件读写
来源：http://mdn.zhoulong.xyz

file_get_contents($f);  file_put_contents($f, $data);
来源：http://nlu.yonumen.top

[U64] PHP：目录遍历
来源：http://cyz.hysaishi.cn

glob("dir/*.php");  scandir("dir");
来源：http://eny.zhaomingkeji.xyz

[U65] PHP：会话
来源：http://ipp.hnqzz.top

session_start();  $_SESSION["uid"] = 1;
来源：http://twv.fktsv.cn

[U66] PHP：设置 Cookie
来源：http://taj.yvedp.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://qob.52xcode.cn

[U67] PHP：处理文件上传
来源：http://vxu.ivvv.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://oqd.meibo888.top

[U68] PHP：PDO 连接
来源：http://ujy.yvedp.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://ezr.fktsv.cn

[U69] PHP：PDO 预处理
来源：http://fvj.fzhhl.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://qiu.aibaodan.cn

[U70] PHP：PDO 事务
来源：http://gdx.xinyue.icu

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://fmp.c1oappe.top

[U71] PHP：抛出异常
来源：http://tnq.mhx1999.top

throw new RuntimeException("失败", 500);
来源：http://jdo.epnwcf.com

[U72] PHP：写错误日志
来源：http://zcu.aizwys.cn

error_log("失败: " . $e->getMessage());
来源：http://bif.bjfxy.top

[U73] PHP：读取 ini 配置
来源：http://mpc.dashuyun.cn

parse_ini_file("config.ini", true)
来源：http://kzl.ywan-chungtsiang.top

[U74] PHP：读取环境变量
来源：http://prh.9152youxi.cn

getenv("APP_ENV") ?: "production"
来源：http://xye.mhx1999.top

[U75] PHP：依赖注入
来源：http://fdj.smart0.xyz

composer require psr/container
来源：http://sea.zhijiandao.cn

[U76] PHP：简单路由
来源：http://kww.wangshuangyany.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://tvd.jinqigufen.top

[U77] PHP：模板渲染
来源：http://nvb.ehwqpu.com

composer require twig/twig
来源：http://orn.jinghuilouyu.cn

[U78] PHP：单元测试
来源：http://roe.chenzaomai.com

composer require --dev phpunit/phpunit
来源：http://gvz.shanyushiyangtech.top

[U79] PHP：静态分析
来源：http://gdd.ydzc1.top

composer require --dev phpstan/phpstan
来源：http://urv.haohaochexian.top

[U80] PHP：代码规范修复
来源：http://mkc.meibo888.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://wqh.cheryme.top

[U81] JS：初始化项目
来源：http://nup.fanxiaobao.xyz

npm init -y;  npm i express
来源：http://hom.zhoulong.xyz

[U82] JS：package.json 脚本
来源：http://jaw.meibo888.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://znf.yj20258.top

[U83] JS：ES Module 导入导出
来源：http://dvf.zhaomingkeji.xyz

export const a = 1;  import { a } from "./m.js";
来源：http://nyx.zhongyouzk.top

[U84] JS：CommonJS 写法
来源：http://nvc.zhaomingkeji.xyz

module.exports = { a };  const { a } = require("./m");
来源：http://jny.zhongyouzk.top

[U85] JS：可选链
来源：http://maq.fanxiaobao.xyz

a?.b?.c
来源：http://tgt.bbcook.cn

[U86] JS：空值合并
来源：http://jee.fktsv.cn

a ?? b
来源：http://yub.mhx1999.top

[U87] JS：解构默认值
来源：http://zev.fktsv.cn

const { a = 1, b = 2 } = obj;
来源：http://syu.haohaochexian.top

[U88] JS：对象展开合并
来源：http://cyy.jqgufenzy.top

{ ...a, ...b }
来源：http://nqf.yanxiufei.cn

[U89] JS：数组去重
来源：http://ini.aizwys.cn

[...new Set(arr)]
来源：http://vmz.wangdashe.top

[U90] JS：数字数组排序
来源：http://viu.tian-w.cn

[...arr].sort((a, b) => a - b)
来源：http://ztr.jinyuanbaomall.cn

[U91] JS：对象键值遍历
来源：http://hvg.yj20258888.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://ibo.yongpay.top

[U92] JS：深拷贝
来源：http://ijo.yfazqb.com

structuredClone(obj)
来源：http://jld.jinyuanbaomall.cn

[U93] JS：模板字符串
来源：http://aoq.yj20258888.top

`共 ${n} 条`
来源：http://ami.jiagoushi.top

[U94] JS：箭头函数
来源：http://kve.yuxming.cn

const double = x => x * 2;
来源：http://egp.chenjidiqi.icu

[U95] JS：Promise 包装
来源：http://izo.zhiwuduotai.top

new Promise((resolve, reject) => {})
来源：http://mca.xylfe.cn

[U96] JS：async/await 与异常
来源：http://ncj.tanke756.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://gnt.shuidangran.top

[U97] JS：并发请求
来源：http://qhk.xuetiantiany.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://yib.uphjek.com

[U98] JS：fetch 带 JSON
来源：http://lfa.aizwys.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://oyd.vehdjk.com

[U99] JS：事件监听
来源：http://hwv.bbcook.cn

el.addEventListener("click", e => {})
来源：http://jbf.yueranfly.top

[U100] JS：DOM 查询
来源：http://qbj.c1oappe.top

document.querySelector(".item")
来源：http://hcc.xingfuxueyuan.xyz

[U101] JS：classList 操作
来源：http://ses.jyoumei.cn

el.classList.toggle("active")
来源：http://orz.ydzc1.top

[U102] JS：本地存储
来源：http://xik.xuanzx.com

localStorage.setItem("k", JSON.stringify(v))
来源：http://bhx.yj202588.top

[U103] JS：定时器
来源：http://lmt.jqgfzy.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://rgm.guannengcc.top

[U104] JS：防抖
来源：http://wsv.snrcjt.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://gwz.hammf.cn

[U105] JS：节流
来源：http://sib.sweek.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://sch.shanyushiyangkeji.top

[U106] JS：日期格式化
来源：http://iqw.yuanzhike.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://gbj.nanxuanxn.top

[U107] JS：数字千分位
来源：http://gpx.gotoacloud.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://jxl.yuxming.cn

[U108] JS：随机整数
来源：http://wrb.9152youxi.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://nsv.hfpthk.cn

[U109] JS：数组分组
来源：http://cgm.fzhhl.top

Object.groupBy(arr, x => x.type)
来源：http://kfv.yanxiufei.cn

[U110] JS：数组分块
来源：http://vlh.shanyushiyangkeji.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://sbn.ybcxt.top

[U111] JS：对象转 Map
来源：http://ncb.gotoacloud.top

new Map(Object.entries(obj))
来源：http://amb.quarkkingdee.top

[U112] JS：字符串补位
来源：http://cnm.bjfxy.top

"7".padStart(3, "0")
来源：http://ibb.cdnleiting.top

[U113] JS：正则替换全部
来源：http://rdx.yj20258.top

s.replaceAll("a", "b")
来源：http://ytd.vqdsnc.cn

[U114] JS：JSON 深比较
来源：http://htd.zhiwuduotai.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://puh.vqdsnc.cn

[U115] JS：生成 UUID
来源：http://vgx.sxryk.cn

crypto.randomUUID()
来源：http://kvl.smart0.xyz

[U116] JS：类型检查（JSDoc）
来源：http://soo.daxiang520.top

/** @param {string} name */ function f(name) {}
来源：http://ekk.fzhhl.top

[U117] JS：单元测试
来源：http://pqj.fengsongda.top

npm i -D vitest;  npx vitest
来源：http://hll.ydjk.org.cn

[U118] JS：开发服务器
来源：http://sua.yonumen.top

npm i -D vite;  npx vite
来源：http://jbc.fktsv.cn

[U119] JS：生产构建
来源：http://vmg.cdnleiting.top

npx vite build
来源：http://yne.jinqigufen.top

[U120] JS：读取环境变量（Vite）
来源：http://dhx.zhongyouzk.top

import.meta.env.VITE_API_URL
来源：http://wkw.jiagoushi.top

================================================================================
来源：http://xmf.zdbjq.cn

统计汇总
来源：http://btj.gotoacloud.top

================================================================================
来源：http://jzo.yj20258888.top

按语言统计（条）：
来源：http://ldz.pycfn.com

Python ......... 252
来源：http://ctj.jiagoushi.top

PHP ............ 252
来源：http://ppj.iojbl.cn

JavaScript ..... 252
来源：http://gdw.chenzaomai.com

TypeScript ..... 212
来源：http://ztm.hesvh.cn


<!-- 参考信息 -->