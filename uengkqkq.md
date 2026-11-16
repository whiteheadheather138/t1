代发 wailian999

[T37] Lua：字符串拼接
来源：http://buw.yongpay.top

"a" .. "b"
来源：http://pas.chenlongwang.top

[T38] Lua：条件
来源：http://ejg.zhengqikj.top

if x > 0 then print("正") end
来源：http://yln.shzxlz.cn

[T39] Lua：模式匹配
来源：http://vsw.wangshuangyany.cn

string.find(s, "%d+")
来源：http://jis.xylfe.cn

[T40] Lua：元表
来源：http://dzl.yongpay.top

setmetatable({}, { __index = base })
来源：http://oxd.shangyingyoupin.top

[T41] Perl：Hello World
来源：http://ljz.sxryk.cn

print "Hello\n";
来源：http://xiz.9152youxi.cn

[T42] Perl：变量类型
来源：http://wzw.ctjpmb.com

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://amq.fehbvm.com

[T43] Perl：字符串插值
来源：http://ete.sjlbkw.cn

"值: $a"
来源：http://bxx.aibaodan.cn

[T44] Perl：条件
来源：http://dmw.hongshengwenyu.top

if ($a > 0) { print "正"; }
来源：http://kyx.cqqwz.cn

[T45] Perl：数组遍历
来源：http://vkx.sufxvd.cn

for my $x (@arr) { print $x; }
来源：http://hqk.xingfuxueyuan.xyz

[T46] Perl：哈希操作
来源：http://lze.yongpay.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://unk.cqqwz.cn

[T47] Perl：正则捕获
来源：http://pso.bbcook.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://xmu.zdqjudy.top

[T48] Perl：正则替换
来源：http://rmq.aibaodan.cn

$s =~ s/old/new/g;
来源：http://riv.yfazqb.com

[T49] Perl：函数
来源：http://wkg.svipenyu.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://eyr.xylfe.cn

[T50] Perl：逐行读文件
来源：http://cia.tian-w.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://zmm.c1oappe.top

while (my $line = <$fh>) { print $line; }
来源：http://hwf.cucudq.cn

[T51] Scala：Hello World
来源：http://jjl.yanxiufei.cn

println("Hello")
来源：http://nbf.yuxming.cn

[T52] Scala：变量
来源：http://cca.ydjk.org.cn

val a = 1;  var b = 2
来源：http://ahx.smart0.xyz

[T53] Scala：字符串插值
来源：http://ayj.daxiang520.top

s"值: $b"
来源：http://cqn.yuanzhike.top

[T54] Scala：集合映射
来源：http://yxo.nanxuanxn.top

List(1, 2, 3).map(_ * 2)
来源：http://aqe.jiagoushi.top

[T55] Scala：集合过滤
来源：http://pdg.jqgfzy.top

List(1, 2, 3).filter(_ > 1)
来源：http://yqz.ctjpmb.com

[T56] Scala：样例类
来源：http://khu.chenjidiqi.icu

case class User(name: String, age: Int)
来源：http://yal.hesvh.cn

[T57] Scala：模式匹配
来源：http://ezw.cdnleiting.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://wvg.shanyushiyangkeji.top

[T58] Scala：函数定义
来源：http://wqm.shanyushiyangkeji.top

def add(a: Int, b: Int): Int = a + b
来源：http://btq.aizwys.cn

[T59] Scala：循环
来源：http://fmy.ivvv.top

for (i <- 1 to 10) println(i)
来源：http://xng.ctjpmb.com

[T60] Scala：折叠
来源：http://uzf.feifeiyinyue.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://wyq.sjlbkw.cn

================================================================================
来源：http://nhw.shanyushiyangkeji.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://swj.hongshengwenyu.top

================================================================================
来源：http://zik.cheryme.top

[U01] Py：创建虚拟环境
来源：http://isw.jiagoushi.top

python -m venv .venv && source .venv/bin/activate
来源：http://oyz.yanxiufei.cn

[U02] Py：导出 / 安装依赖
来源：http://gzb.ydzc1.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://qwc.pengpengdd.cyou

[U03] Py：加载 .env 配置
来源：http://rbz.cqqwz.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://etu.zhijiandao.cn

[U04] Py：变量调试打印
来源：http://nnx.shangyingyoupin.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://qux.hnqzz.top

[U05] Py：列表去重且保序
来源：http://brz.dashuyun.cn

list(dict.fromkeys(arr))
来源：http://maj.tian-w.cn

[U06] Py：合并两个字典
来源：http://vzt.epnwcf.com

{**a, **b}
来源：http://ezg.ybcxt.top

[U07] Py：反转字典键值
来源：http://pfr.nanxinkj.top

{v: k for k, v in d.items()}
来源：http://qjz.tarul.cn

[U08] Py：展平二维列表
来源：http://vnu.jinqigufen.top

[y for x in nested for y in x]
来源：http://crl.cdnleiting.top

[U09] Py：字典取最大值的键
来源：http://lwr.ivvv.top

max(d, key=d.get)
来源：http://scw.shanyushiyangtech.top

[U10] Py：按值排序字典
来源：http://qcw.c1oappe.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://mql.zhijiandao.cn

[U11] Py：生成器表达式
来源：http://mhg.sysykeji.top

(x * 2 for x in arr)
来源：http://hiw.daxiang520.top

[U12] Py：取出现最多的 3 个元素
来源：http://roj.hnqzz.top

Counter(arr).most_common(3)
来源：http://fdn.cdnleiting.top

[U13] Py：固定长度队列
来源：http://jto.shuidangran.top

deque(maxlen=10)
来源：http://uvd.0kj1m.cn

[U14] Py：分组收集到列表
来源：http://izk.hcnkem.com

defaultdict(list)
来源：http://rdl.gotoacloud.top

[U15] Py：高精度计时
来源：http://rui.tian-w.cn

t = time.perf_counter()
来源：http://znj.iojbl.cn

[U16] Py：命令行参数解析
来源：http://pwa.jinqigufen.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://zzz.sufxvd.cn

[U17] Py：初始化日志
来源：http://lff.hammf.cn

logging.basicConfig(level=logging.INFO)
来源：http://zzw.cheryme.top

[U18] Py：预编译正则
来源：http://kpn.yj20258888.top

pat = re.compile(r"\d+")
来源：http://iag.zhongyouzk.top

[U19] Py：正则替换带回调
来源：http://xpa.guannengcc.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://bvc.wangdashe.top

[U20] Py：缓存函数结果
来源：http://fjk.yfazqb.com

@functools.lru_cache(maxsize=None)
来源：http://jww.yj20258.top

[U21] Py：自定义上下文管理器
来源：http://pjo.sjlbkw.cn

@contextlib.contextmanager
来源：http://fiu.tianlin.xyz

[U22] Py：矩阵转置
来源：http://ekc.gaohongyu789.top

list(zip(*m))
来源：http://vig.smart0.xyz

[U23] Py：分块读取大文件
来源：http://lwq.guowangkeji.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://vww.9152youxi.cn

[U24] Py：路径操作
来源：http://qfn.jinqigfzy.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://rgt.uphjek.com

[U25] Py：CSV 按字典读
来源：http://dki.andypj.xyz

csv.DictReader(f)
来源：http://ing.kuanghao11.cn

[U26] Py：并发下载
来源：http://wau.vehdjk.com

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://ptm.sjlbkw.cn

[U27] Py：异步 HTTP
来源：http://tbf.smart0.xyz

aiohttp.ClientSession() 配合 async with
来源：http://vmf.nanxuanxn.top

[U28] Py：类型别名
来源：http://wfd.nanxuanxn.top

UserId = int
来源：http://kxv.0kj1m.cn

[U29] Py：属性校验
来源：http://jvh.fanxiaobao.xyz

@property 与 @x.setter 配合
来源：http://gzp.jinyuanbaomall.cn

[U30] Py：数据类
来源：http://ojp.pycfn.com

@dataclass(slots=True)
来源：http://zof.svipenyu.cn

[U31] Py：单测
来源：http://kky.zhengqikj.top

python -m pytest -q
来源：http://itw.ctjpmb.com

[U32] Py：代码格式化
来源：http://hlr.uphjek.com

ruff format . && ruff check --fix .
来源：http://oae.hongshengwenyu.top

[U33] Py：打包发布
来源：http://cwg.yvedp.cn

python -m build  （依赖 pyproject.toml）
来源：http://qof.daria6918.cn

[U34] Py：判断编码
来源：http://pxm.vqdsnc.cn

chardet.detect(raw)
来源：http://mrv.tanke756.top

[U35] Py：发送邮件
来源：http://roc.pycfn.com

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://ktr.birdmap.top

[U36] Py：定时任务
来源：http://ziu.shuidangran.top

schedule.every(10).minutes.do(job)
来源：http://ovs.chenzaomai.com

[U37] Py：读写 Excel
来源：http://dog.sxryk.cn

pandas.read_excel / DataFrame.to_excel
来源：http://ymn.nanxuanxn.top

[U38] Py：获取脚本所在目录
来源：http://vpa.shuidangran.top

Path(__file__).resolve().parent
来源：http://tqf.xuetiantiany.cn

[U39] Py：判断是否在交互环境
来源：http://phs.yuxming.cn

sys.stdout.isatty()
来源：http://feo.zhixingplan.top

[U40] Py：打印到标准错误
来源：http://aez.zhaomingkeji.xyz

print("err", file=sys.stderr)
来源：http://cev.wangshuangyany.cn

[U41] PHP：初始化 Composer 项目
来源：http://bos.hammf.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://egt.zhengqikj.top

[U42] PHP：PSR-4 自动加载
来源：http://kmb.hfpthk.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hgq.shuidangran.top

[U43] PHP：声明命名空间
来源：http://aaz.snrcjt.cn

namespace App\Http;
来源：http://fge.shangyingyoupin.top

[U44] PHP：开启严格类型
来源：http://kes.yvedp.cn

declare(strict_types=1);
来源：http://eom.yanxiufei.cn

[U45] PHP：类型声明与返回类型
来源：http://jck.yonumen.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://jjh.wangdashe.top

[U46] PHP：可空类型
来源：http://oml.svipenyu.cn

?string $name = null
来源：http://xjv.feifeiyinyue.top

[U47] PHP：联合类型
来源：http://xkx.aibaodan.cn

int|string $id
来源：http://cnb.iojbl.cn

[U48] PHP：纯枚举
来源：http://qer.jyoumei.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://imd.chenlongwang.top

[U49] PHP：只读属性
来源：http://acp.jinqigufen.top

public readonly string $name
来源：http://bjp.hcnkem.com

[U50] PHP：构造器属性提升
来源：http://ztq.sysykeji.top

public function __construct(private int $id) {}
来源：http://fco.hfpthk.cn

[U51] PHP：数组解构
来源：http://gcf.shanyushiyangtech.top

[$a, $b] = $arr;
来源：http://xtr.cdnleiting.top

[U52] PHP：箭头函数
来源：http://vao.ppjwa.cn

$double = fn($x) => $x * 2;
来源：http://iot.daria6918.cn

[U53] PHP：空合并运算符
来源：http://ekg.9152youxi.cn

$v = $a ?? $b ?? "default";
来源：http://kpe.nwbrower.top

[U54] PHP：空安全调用
来源：http://ane.ydzc1.top

$obj?->method()
来源：http://zez.yongpay.top

[U55] PHP：match 表达式
来源：http://yrz.hysaishi.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://jso.chenjidiqi.icu

[U56] PHP：命名参数
来源：http://dbh.zhiwuduotai.top

f(a: 1, b: 2)
来源：http://een.chenjidiqi.icu

[U57] PHP：字符串插值
来源：http://kgi.hongshengwenyu.top

"值: {$a}"
来源：http://azu.wangshuangyany.cn

[U58] PHP：数组三件套
来源：http://ovf.haohaochexian.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hal.tianlin.xyz

[U59] PHP：自定义排序
来源：http://uuf.epnwcf.com

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://tbw.mhx1999.top

[U60] PHP：JSON 编解码
来源：http://rnh.haohaochexian.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hkl.zhongyouzk.top

[U61] PHP：正则
来源：http://mxk.tarul.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://znd.jinqigfzy.top

[U62] PHP：日期对象
来源：http://zke.fehbvm.com

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hau.hammf.cn

[U63] PHP：文件读写
来源：http://kni.xylfe.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://sea.bjfxy.top

[U64] PHP：目录遍历
来源：http://mih.jyoumei.cn

glob("dir/*.php");  scandir("dir");
来源：http://wcj.smart0.xyz

[U65] PHP：会话
来源：http://qvk.chenlongwang.top

session_start();  $_SESSION["uid"] = 1;
来源：http://kwg.redwolf501.top

[U66] PHP：设置 Cookie
来源：http://ype.snrcjt.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://uwp.sweek.top

[U67] PHP：处理文件上传
来源：http://nka.zhongyouzk.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://ens.chenzaomai.com

[U68] PHP：PDO 连接
来源：http://nzu.tian-w.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://jlp.sweek.top

[U69] PHP：PDO 预处理
来源：http://dow.316326.xyz

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://ryp.cashguo.top

[U70] PHP：PDO 事务
来源：http://vhp.mhx1999.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://drp.0kj1m.cn

[U71] PHP：抛出异常
来源：http://fmp.xylfe.cn

throw new RuntimeException("失败", 500);
来源：http://pus.9152youxi.cn

[U72] PHP：写错误日志
来源：http://axg.gzhubu.top

error_log("失败: " . $e->getMessage());
来源：http://nzi.jianghu66.top

[U73] PHP：读取 ini 配置
来源：http://apk.zycfv.cn

parse_ini_file("config.ini", true)
来源：http://egu.bbcook.cn

[U74] PHP：读取环境变量
来源：http://pfs.iojbl.cn

getenv("APP_ENV") ?: "production"
来源：http://wmf.gaohongyu789.top

[U75] PHP：依赖注入
来源：http://cqt.pycfn.com

composer require psr/container
来源：http://wco.quarkkingdee.top

[U76] PHP：简单路由
来源：http://ele.jinyuanbaomall.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://lem.316326.xyz

[U77] PHP：模板渲染
来源：http://iiy.ydzc1.top

composer require twig/twig
来源：http://asp.316326.xyz

[U78] PHP：单元测试
来源：http://uzt.zycfv.cn

composer require --dev phpunit/phpunit
来源：http://oxi.yonumen.top

[U79] PHP：静态分析
来源：http://crn.yanxiufei.cn

composer require --dev phpstan/phpstan
来源：http://dvl.zhengqikj.top

[U80] PHP：代码规范修复
来源：http://vmw.wangshuangyany.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://jkh.0kj1m.cn

[U81] JS：初始化项目
来源：http://hxs.svipenyu.cn

npm init -y;  npm i express
来源：http://gxc.hongshengwenyu.top

[U82] JS：package.json 脚本
来源：http://ucg.dianchejie.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://fgn.hnxiangtu.top

[U83] JS：ES Module 导入导出
来源：http://aob.nanxuanxn.top

export const a = 1;  import { a } from "./m.js";
来源：http://eev.shangyingyoupin.top

[U84] JS：CommonJS 写法
来源：http://fpn.hywenlv.cn

module.exports = { a };  const { a } = require("./m");
来源：http://atf.bjfxy.top

[U85] JS：可选链
来源：http://ldw.haohaochexian.top

a?.b?.c
来源：http://dng.aibaodan.cn

[U86] JS：空值合并
来源：http://syj.jiagoushi.top

a ?? b
来源：http://koc.iojbl.cn

[U87] JS：解构默认值
来源：http://ynq.quarkkingdee.top

const { a = 1, b = 2 } = obj;
来源：http://wss.yj202588.top

[U88] JS：对象展开合并
来源：http://ukq.quarkkingdee.top

{ ...a, ...b }
来源：http://xok.feifeiyinyue.top

[U89] JS：数组去重
来源：http://upi.ppjwa.cn

[...new Set(arr)]
来源：http://lyl.daxiang520.top

[U90] JS：数字数组排序
来源：http://oqv.52xcode.cn

[...arr].sort((a, b) => a - b)
来源：http://dmr.hcnkem.com

[U91] JS：对象键值遍历
来源：http://cfn.zhiwuduotai.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://dns.zhijiandao.cn

[U92] JS：深拷贝
来源：http://uwu.jqgufenzy.top

structuredClone(obj)
来源：http://vpv.snrcjt.cn

[U93] JS：模板字符串
来源：http://vnf.cashguo.top

`共 ${n} 条`
来源：http://fud.bjfxy.top

[U94] JS：箭头函数
来源：http://rky.pycfn.com

const double = x => x * 2;
来源：http://ugz.epnwcf.com

[U95] JS：Promise 包装
来源：http://usx.kuanghao11.cn

new Promise((resolve, reject) => {})
来源：http://nvr.nanxuanxn.top

[U96] JS：async/await 与异常
来源：http://cfi.tarul.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://dig.gotoacloud.top

[U97] JS：并发请求
来源：http://ims.jianghu66.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://yqs.9152youxi.cn

[U98] JS：fetch 带 JSON
来源：http://vfg.xuetiantiany.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://kru.zycfv.cn

[U99] JS：事件监听
来源：http://mte.jinqigfzy.top

el.addEventListener("click", e => {})
来源：http://nzu.xuetiantiany.cn

[U100] JS：DOM 查询
来源：http://qey.chenlongwang.top

document.querySelector(".item")
来源：http://uij.wangdashe.top

[U101] JS：classList 操作
来源：http://gsd.9152youxi.cn

el.classList.toggle("active")
来源：http://mug.ybcxt.top

[U102] JS：本地存储
来源：http://ird.jqgufenzy.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://tui.jlsjyb.cn

[U103] JS：定时器
来源：http://prx.guannengcc.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://tgc.jlsjyb.cn

[U104] JS：防抖
来源：http://ahq.gzhubu.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://cfq.jianghu66.top

[U105] JS：节流
来源：http://zhq.zhengqikj.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://ksp.kuanghao11.cn

[U106] JS：日期格式化
来源：http://djo.tian-w.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://lpw.wangdashe.top

[U107] JS：数字千分位
来源：http://mlw.epnwcf.com

new Intl.NumberFormat("en-US").format(1234567)
来源：http://wzn.52xcode.cn

[U108] JS：随机整数
来源：http://ack.ehwqpu.com

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://ofs.jinqigufen.top

[U109] JS：数组分组
来源：http://uju.wangshuangyany.cn

Object.groupBy(arr, x => x.type)
来源：http://kep.gzhubu.top

[U110] JS：数组分块
来源：http://tkd.yfazqb.com

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://npe.xziqi.cn

[U111] JS：对象转 Map
来源：http://aoh.c1oappe.top

new Map(Object.entries(obj))
来源：http://vyy.sufxvd.cn

[U112] JS：字符串补位
来源：http://gxe.hongshengwenyu.top

"7".padStart(3, "0")
来源：http://nlw.feifeiyinyue.top

[U113] JS：正则替换全部
来源：http://kep.fktsv.cn

s.replaceAll("a", "b")
来源：http://lkh.shanyushiyangkeji.top

[U114] JS：JSON 深比较
来源：http://qon.yangfankeji.com

JSON.stringify(a) === JSON.stringify(b)
来源：http://aey.jiagoushi.top

[U115] JS：生成 UUID
来源：http://utu.ywan-chungtsiang.top

crypto.randomUUID()
来源：http://upp.jlsjyb.cn

[U116] JS：类型检查（JSDoc）
来源：http://acs.yanxiufei.cn

/** @param {string} name */ function f(name) {}
来源：http://sfy.aizwys.cn

[U117] JS：单元测试
来源：http://lsd.tarul.cn

npm i -D vitest;  npx vitest
来源：http://dsi.sxryk.cn

[U118] JS：开发服务器
来源：http://eci.zhaomingkeji.xyz

npm i -D vite;  npx vite
来源：http://bef.hammf.cn

[U119] JS：生产构建
来源：http://voy.pengpengdd.cyou

npx vite build
来源：http://dbn.havefunace.top

[U120] JS：读取环境变量（Vite）
来源：http://fjd.jqgfzy.top

import.meta.env.VITE_API_URL
来源：http://pny.cqqwz.cn

================================================================================
来源：http://tpt.havefunace.top

统计汇总
来源：http://jad.jinyuanbaomall.cn

================================================================================
来源：http://wyf.zhengqikj.top

按语言统计（条）：
来源：http://xhr.tian-w.cn

Python ......... 252
来源：http://nwe.jlsjyb.cn

PHP ............ 252
来源：http://xhg.jiagoushi.top

JavaScript ..... 252
来源：http://nre.fehbvm.com

TypeScript ..... 212
来源：http://jtd.gzhubu.top


<!-- 参考信息 -->