代发 wailian999

[T35] Lua：字典表
来源：http://jnj.cheryme.top

local d = { a = 1 };  d.b = 2
来源：http://fvw.aizwys.cn

[T36] Lua：函数
来源：http://blx.fktsv.cn

function add(a, b) return a + b end
来源：http://ihw.yj20258888.top

[T37] Lua：字符串拼接
来源：http://guc.bjfxy.top

"a" .. "b"
来源：http://eyu.cucudq.cn

[T38] Lua：条件
来源：http://chh.shangyingyoupin.top

if x > 0 then print("正") end
来源：http://gqn.hnqzz.top

[T39] Lua：模式匹配
来源：http://pqc.fktsv.cn

string.find(s, "%d+")
来源：http://qsf.tarul.cn

[T40] Lua：元表
来源：http://ckm.guowangkeji.top

setmetatable({}, { __index = base })
来源：http://pzf.cucudq.cn

[T41] Perl：Hello World
来源：http://lkq.zhixingplan.top

print "Hello\n";
来源：http://wnn.bjfxy.top

[T42] Perl：变量类型
来源：http://nyn.aizwys.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://sxg.yanxiufei.cn

[T43] Perl：字符串插值
来源：http://inr.sweek.top

"值: $a"
来源：http://obe.jiagoushi.top

[T44] Perl：条件
来源：http://xds.yvedp.cn

if ($a > 0) { print "正"; }
来源：http://ynd.zhijiandao.cn

[T45] Perl：数组遍历
来源：http://rnc.xziqi.cn

for my $x (@arr) { print $x; }
来源：http://fkc.52xcode.cn

[T46] Perl：哈希操作
来源：http://lcn.hysaishi.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://fjh.shuidangran.top

[T47] Perl：正则捕获
来源：http://jyx.fzhhl.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://jjk.hfpthk.cn

[T48] Perl：正则替换
来源：http://eaw.yvedp.cn

$s =~ s/old/new/g;
来源：http://oza.xylfe.cn

[T49] Perl：函数
来源：http://mqx.yvedp.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://rea.yvedp.cn

[T50] Perl：逐行读文件
来源：http://tnk.ydzc1.top

open my $fh, "<", "a.txt" or die $!;
来源：http://vvf.hongshengwenyu.top

while (my $line = <$fh>) { print $line; }
来源：http://zdb.gogol.net.cn

[T51] Scala：Hello World
来源：http://xzm.yj20258888.top

println("Hello")
来源：http://gko.aibaodan.cn

[T52] Scala：变量
来源：http://zfk.hammf.cn

val a = 1;  var b = 2
来源：http://nnl.shzxlz.cn

[T53] Scala：字符串插值
来源：http://gum.xuanzx.com

s"值: $b"
来源：http://fsa.nanxuanxn.top

[T54] Scala：集合映射
来源：http://rqc.gzhubu.top

List(1, 2, 3).map(_ * 2)
来源：http://pol.ivvv.top

[T55] Scala：集合过滤
来源：http://fln.gzhubu.top

List(1, 2, 3).filter(_ > 1)
来源：http://bms.redwolf501.top

[T56] Scala：样例类
来源：http://vuo.shzxlz.cn

case class User(name: String, age: Int)
来源：http://eju.xuanzx.com

[T57] Scala：模式匹配
来源：http://yea.guowangkeji.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://vjf.yonumen.top

[T58] Scala：函数定义
来源：http://aqa.xuetiantiany.cn

def add(a: Int, b: Int): Int = a + b
来源：http://dmc.hesvh.cn

[T59] Scala：循环
来源：http://xcx.jqgfzy.top

for (i <- 1 to 10) println(i)
来源：http://bom.tian-w.cn

[T60] Scala：折叠
来源：http://kox.zhengqikj.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://mtl.jinqigfzy.top

================================================================================
来源：http://hxd.zhixingplan.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://nxi.jyoumei.cn

================================================================================
来源：http://lot.hongshengwenyu.top

[U01] Py：创建虚拟环境
来源：http://rbv.vehdjk.com

python -m venv .venv && source .venv/bin/activate
来源：http://nxe.jinghuilouyu.cn

[U02] Py：导出 / 安装依赖
来源：http://htt.uphjek.com

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://zzv.xuanzx.com

[U03] Py：加载 .env 配置
来源：http://mga.tianlin.xyz

from dotenv import load_dotenv; load_dotenv()
来源：http://imo.jinghuilouyu.cn

[U04] Py：变量调试打印
来源：http://emt.jinyuanbaomall.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://mxv.daria6918.cn

[U05] Py：列表去重且保序
来源：http://gkj.daria6918.cn

list(dict.fromkeys(arr))
来源：http://ght.redwolf501.top

[U06] Py：合并两个字典
来源：http://zkh.dianchejie.cn

{**a, **b}
来源：http://eiw.9152youxi.cn

[U07] Py：反转字典键值
来源：http://svt.haohaochexian.top

{v: k for k, v in d.items()}
来源：http://rde.quarkkingdee.top

[U08] Py：展平二维列表
来源：http://rdo.xinyue.icu

[y for x in nested for y in x]
来源：http://ucc.fktsv.cn

[U09] Py：字典取最大值的键
来源：http://asx.birdmap.top

max(d, key=d.get)
来源：http://ths.uphjek.com

[U10] Py：按值排序字典
来源：http://ihp.yanxiufei.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://vfc.fehbvm.com

[U11] Py：生成器表达式
来源：http://fmb.tianlin.xyz

(x * 2 for x in arr)
来源：http://gku.meibo888.top

[U12] Py：取出现最多的 3 个元素
来源：http://nqa.cdnleiting.top

Counter(arr).most_common(3)
来源：http://evs.jqgfzy.top

[U13] Py：固定长度队列
来源：http://qtc.epnwcf.com

deque(maxlen=10)
来源：http://ots.gzhubu.top

[U14] Py：分组收集到列表
来源：http://aip.zdbjq.cn

defaultdict(list)
来源：http://tsy.9152youxi.cn

[U15] Py：高精度计时
来源：http://exi.xuanzx.com

t = time.perf_counter()
来源：http://xyg.smart0.xyz

[U16] Py：命令行参数解析
来源：http://evm.ehwqpu.com

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://ouu.pengpengdd.cyou

[U17] Py：初始化日志
来源：http://uty.zhijiandao.cn

logging.basicConfig(level=logging.INFO)
来源：http://wqk.0kj1m.cn

[U18] Py：预编译正则
来源：http://gfo.andypj.xyz

pat = re.compile(r"\d+")
来源：http://mzf.jiagoushi.top

[U19] Py：正则替换带回调
来源：http://hlq.bbcook.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://iyz.jinghuilouyu.cn

[U20] Py：缓存函数结果
来源：http://mbv.yj20258888.top

@functools.lru_cache(maxsize=None)
来源：http://wbl.jinqigfzy.top

[U21] Py：自定义上下文管理器
来源：http://tkr.ctjpmb.com

@contextlib.contextmanager
来源：http://nmz.xuanzx.com

[U22] Py：矩阵转置
来源：http://pnl.ehwqpu.com

list(zip(*m))
来源：http://ggv.zdqjudy.top

[U23] Py：分块读取大文件
来源：http://ajn.gaohongyu789.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://dgz.redwolf501.top

[U24] Py：路径操作
来源：http://kfb.hcnkem.com

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://lmy.redwolf501.top

[U25] Py：CSV 按字典读
来源：http://zhe.fktsv.cn

csv.DictReader(f)
来源：http://faf.xylfe.cn

[U26] Py：并发下载
来源：http://gze.aizwys.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://ewl.jqgufenzy.top

[U27] Py：异步 HTTP
来源：http://mes.jqgfzy.top

aiohttp.ClientSession() 配合 async with
来源：http://bqu.yvedp.cn

[U28] Py：类型别名
来源：http://rpm.sxryk.cn

UserId = int
来源：http://gak.tanke756.top

[U29] Py：属性校验
来源：http://qgt.jinghuilouyu.cn

@property 与 @x.setter 配合
来源：http://ljt.yj20258888.top

[U30] Py：数据类
来源：http://vvl.quarkkingdee.top

@dataclass(slots=True)
来源：http://ola.zhongyouzk.top

[U31] Py：单测
来源：http://dns.xziqi.cn

python -m pytest -q
来源：http://avi.jiagoushi.top

[U32] Py：代码格式化
来源：http://tpu.birdmap.top

ruff format . && ruff check --fix .
来源：http://llc.sjlbkw.cn

[U33] Py：打包发布
来源：http://dml.zhengqikj.top

python -m build  （依赖 pyproject.toml）
来源：http://wkn.shzxlz.cn

[U34] Py：判断编码
来源：http://kjl.shzxlz.cn

chardet.detect(raw)
来源：http://zqa.ehwqpu.com

[U35] Py：发送邮件
来源：http://egm.iojbl.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://qpm.dianchejie.cn

[U36] Py：定时任务
来源：http://sox.ppjwa.cn

schedule.every(10).minutes.do(job)
来源：http://med.tanke756.top

[U37] Py：读写 Excel
来源：http://xtr.daria6918.cn

pandas.read_excel / DataFrame.to_excel
来源：http://hns.aizwys.cn

[U38] Py：获取脚本所在目录
来源：http://wpf.316326.xyz

Path(__file__).resolve().parent
来源：http://pch.nwbrower.top

[U39] Py：判断是否在交互环境
来源：http://qcz.ydzc1.top

sys.stdout.isatty()
来源：http://gae.ydzc1.top

[U40] Py：打印到标准错误
来源：http://rxk.jyoumei.cn

print("err", file=sys.stderr)
来源：http://izb.tian-w.cn

[U41] PHP：初始化 Composer 项目
来源：http://xou.smart0.xyz

composer init;  composer require guzzlehttp/guzzle
来源：http://iwm.jinqigfzy.top

[U42] PHP：PSR-4 自动加载
来源：http://hyo.jinyuanbaomall.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://zqq.wangdashe.top

[U43] PHP：声明命名空间
来源：http://lzt.zhixingplan.top

namespace App\Http;
来源：http://qno.jlsjyb.cn

[U44] PHP：开启严格类型
来源：http://hsp.nwbrower.top

declare(strict_types=1);
来源：http://isv.316326.xyz

[U45] PHP：类型声明与返回类型
来源：http://qag.vqdsnc.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://plh.shanyushiyangkeji.top

[U46] PHP：可空类型
来源：http://kej.jinyuanbaomall.cn

?string $name = null
来源：http://rqr.andypj.xyz

[U47] PHP：联合类型
来源：http://diq.xylfe.cn

int|string $id
来源：http://rkb.tianlin.xyz

[U48] PHP：纯枚举
来源：http://euf.haohaochexian.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://awr.ppjwa.cn

[U49] PHP：只读属性
来源：http://rub.c1oappe.top

public readonly string $name
来源：http://ebq.yonumen.top

[U50] PHP：构造器属性提升
来源：http://ixm.zhiwuduotai.top

public function __construct(private int $id) {}
来源：http://gmt.zhaomingkeji.xyz

[U51] PHP：数组解构
来源：http://dwx.dianchejie.cn

[$a, $b] = $arr;
来源：http://npg.ctjpmb.com

[U52] PHP：箭头函数
来源：http://vai.jiagoushi.top

$double = fn($x) => $x * 2;
来源：http://vje.shangyingyoupin.top

[U53] PHP：空合并运算符
来源：http://ldl.yj20258.top

$v = $a ?? $b ?? "default";
来源：http://jfm.nwbrower.top

[U54] PHP：空安全调用
来源：http://ayb.zhixingplan.top

$obj?->method()
来源：http://kpb.zhaomingkeji.xyz

[U55] PHP：match 表达式
来源：http://onb.svipenyu.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://fsp.chenzaomai.com

[U56] PHP：命名参数
来源：http://vzy.ybcxt.top

f(a: 1, b: 2)
来源：http://zoh.vehdjk.com

[U57] PHP：字符串插值
来源：http://fjh.cdnleiting.top

"值: {$a}"
来源：http://dhq.zhoulong.xyz

[U58] PHP：数组三件套
来源：http://hbw.tanke756.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://zdp.gotoacloud.top

[U59] PHP：自定义排序
来源：http://vzs.pycfn.com

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hos.kuanghao11.cn

[U60] PHP：JSON 编解码
来源：http://iry.yfazqb.com

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://ikv.havefunace.top

[U61] PHP：正则
来源：http://tdq.hnxiangtu.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://gbl.jianghu66.top

[U62] PHP：日期对象
来源：http://dbw.yfazqb.com

(new DateTimeImmutable())->format("Y-m-d");
来源：http://rkz.sufxvd.cn

[U63] PHP：文件读写
来源：http://pit.tarul.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://bsr.shanyushiyangkeji.top

[U64] PHP：目录遍历
来源：http://bwi.gaohongyu789.top

glob("dir/*.php");  scandir("dir");
来源：http://apr.zhoulong.xyz

[U65] PHP：会话
来源：http://ove.birdmap.top

session_start();  $_SESSION["uid"] = 1;
来源：http://tow.svipenyu.cn

[U66] PHP：设置 Cookie
来源：http://lfm.zdqjudy.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://gep.guannengcc.top

[U67] PHP：处理文件上传
来源：http://xks.wangdashe.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://qwq.shanyushiyangkeji.top

[U68] PHP：PDO 连接
来源：http://cxs.haohaochexian.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://uru.zhengqikj.top

[U69] PHP：PDO 预处理
来源：http://kgw.cdnleiting.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://qrn.aibaodan.cn

[U70] PHP：PDO 事务
来源：http://ijp.jlsjyb.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://nqp.c1oappe.top

[U71] PHP：抛出异常
来源：http://tqj.zdqjudy.top

throw new RuntimeException("失败", 500);
来源：http://nan.cashguo.top

[U72] PHP：写错误日志
来源：http://pei.vehdjk.com

error_log("失败: " . $e->getMessage());
来源：http://xxi.shzxlz.cn

[U73] PHP：读取 ini 配置
来源：http://uln.gotoacloud.top

parse_ini_file("config.ini", true)
来源：http://tbe.hcnkem.com

[U74] PHP：读取环境变量
来源：http://dih.fehbvm.com

getenv("APP_ENV") ?: "production"
来源：http://icn.9152youxi.cn

[U75] PHP：依赖注入
来源：http://bwz.gogol.net.cn

composer require psr/container
来源：http://isi.yj20258888.top

[U76] PHP：简单路由
来源：http://oes.yanxiufei.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://ypg.gotoacloud.top

[U77] PHP：模板渲染
来源：http://vxj.yj20258.top

composer require twig/twig
来源：http://mky.havefunace.top

[U78] PHP：单元测试
来源：http://ewo.jqgfzy.top

composer require --dev phpunit/phpunit
来源：http://vqs.52xcode.cn

[U79] PHP：静态分析
来源：http://uzj.zhongyouzk.top

composer require --dev phpstan/phpstan
来源：http://vvj.feifeiyinyue.top

[U80] PHP：代码规范修复
来源：http://dph.redwolf501.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://gsv.andypj.xyz

[U81] JS：初始化项目
来源：http://nqc.andypj.xyz

npm init -y;  npm i express
来源：http://tuf.hammf.cn

[U82] JS：package.json 脚本
来源：http://qup.shanyushiyangtech.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://hdi.aizwys.cn

[U83] JS：ES Module 导入导出
来源：http://iyg.yj20258.top

export const a = 1;  import { a } from "./m.js";
来源：http://unx.0kj1m.cn

[U84] JS：CommonJS 写法
来源：http://csl.cashguo.top

module.exports = { a };  const { a } = require("./m");
来源：http://imd.yj20258.top

[U85] JS：可选链
来源：http://rwv.birdmap.top

a?.b?.c
来源：http://deo.svipenyu.cn

[U86] JS：空值合并
来源：http://uze.tarul.cn

a ?? b
来源：http://gpg.sufxvd.cn

[U87] JS：解构默认值
来源：http://bqv.zycfv.cn

const { a = 1, b = 2 } = obj;
来源：http://vgg.jinqigfzy.top

[U88] JS：对象展开合并
来源：http://top.bbcook.cn

{ ...a, ...b }
来源：http://ozt.hongshengwenyu.top

[U89] JS：数组去重
来源：http://fsb.chenlongwang.top

[...new Set(arr)]
来源：http://oqp.fanxiaobao.xyz

[U90] JS：数字数组排序
来源：http://qwd.sweek.top

[...arr].sort((a, b) => a - b)
来源：http://xml.vehdjk.com

[U91] JS：对象键值遍历
来源：http://cpd.sufxvd.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://gam.52xcode.cn

[U92] JS：深拷贝
来源：http://nqv.c1oappe.top

structuredClone(obj)
来源：http://xfn.9152youxi.cn

[U93] JS：模板字符串
来源：http://dze.feifeiyinyue.top

`共 ${n} 条`
来源：http://raz.zhixingplan.top

[U94] JS：箭头函数
来源：http://ldi.hongshengwenyu.top

const double = x => x * 2;
来源：http://iok.dianchejie.cn

[U95] JS：Promise 包装
来源：http://vmq.nanxuanxn.top

new Promise((resolve, reject) => {})
来源：http://pis.hesvh.cn

[U96] JS：async/await 与异常
来源：http://lxu.aibaodan.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://zbv.gogol.net.cn

[U97] JS：并发请求
来源：http://glm.bbcook.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://bri.zdbjq.cn

[U98] JS：fetch 带 JSON
来源：http://pvq.zycfv.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://jlo.aizwys.cn

[U99] JS：事件监听
来源：http://xzu.ivvv.top

el.addEventListener("click", e => {})
来源：http://ten.daxiang520.top

[U100] JS：DOM 查询
来源：http://jux.snrcjt.cn

document.querySelector(".item")
来源：http://dpd.cheryme.top

[U101] JS：classList 操作
来源：http://ocw.yuanzhike.top

el.classList.toggle("active")
来源：http://tqt.hnqzz.top

[U102] JS：本地存储
来源：http://uxq.shanyushiyangkeji.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://boi.mhx1999.top

[U103] JS：定时器
来源：http://eol.zhoulong.xyz

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://ecq.cashguo.top

[U104] JS：防抖
来源：http://xsh.hesvh.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://rtz.vehdjk.com

[U105] JS：节流
来源：http://alw.dashuyun.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://dkm.zhoulong.xyz

[U106] JS：日期格式化
来源：http://iwe.gotoacloud.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://dqh.9152youxi.cn

[U107] JS：数字千分位
来源：http://zzm.chenjidiqi.icu

new Intl.NumberFormat("en-US").format(1234567)
来源：http://wpc.zhaomingkeji.xyz

[U108] JS：随机整数
来源：http://suw.meibo888.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://all.jlsjyb.cn

[U109] JS：数组分组
来源：http://ves.fehbvm.com

Object.groupBy(arr, x => x.type)
来源：http://tzk.bjfxy.top

[U110] JS：数组分块
来源：http://bab.ivvv.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://chr.aibaodan.cn

[U111] JS：对象转 Map
来源：http://epq.zhongyouzk.top

new Map(Object.entries(obj))
来源：http://svb.xuetiantiany.cn

[U112] JS：字符串补位
来源：http://tyg.sysykeji.top

"7".padStart(3, "0")
来源：http://idw.zhixingplan.top

[U113] JS：正则替换全部
来源：http://eyc.aizwys.cn

s.replaceAll("a", "b")
来源：http://trq.zhongyouzk.top

[U114] JS：JSON 深比较
来源：http://uer.guannengcc.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://cdd.ywan-chungtsiang.top

[U115] JS：生成 UUID
来源：http://xht.zhixingplan.top

crypto.randomUUID()
来源：http://wlm.ybcxt.top

[U116] JS：类型检查（JSDoc）
来源：http://yud.vqdsnc.cn

/** @param {string} name */ function f(name) {}
来源：http://emn.fanxiaobao.xyz

[U117] JS：单元测试
来源：http://ylb.havefunace.top

npm i -D vitest;  npx vitest
来源：http://ktu.quarkkingdee.top

[U118] JS：开发服务器
来源：http://zpf.jinghuilouyu.cn

npm i -D vite;  npx vite
来源：http://hvx.jinqigfzy.top

[U119] JS：生产构建
来源：http://qtn.pycfn.com

npx vite build
来源：http://jaz.yangfankeji.com

[U120] JS：读取环境变量（Vite）
来源：http://qgk.pengpengdd.cyou

import.meta.env.VITE_API_URL
来源：http://ire.fzhhl.top

================================================================================
来源：http://asc.xuetiantiany.cn

统计汇总
来源：http://fgr.gogol.net.cn

================================================================================
来源：http://ujv.hongshengwenyu.top

按语言统计（条）：
来源：http://nky.birdmap.top


<!-- 参考信息 -->