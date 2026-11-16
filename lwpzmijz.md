代发 wailian999

[T35] Lua：字典表
来源：http://zxs.ivvv.top

local d = { a = 1 };  d.b = 2
来源：http://miw.zdbjq.cn

[T36] Lua：函数
来源：http://lcx.cdnleiting.top

function add(a, b) return a + b end
来源：http://kst.aizwys.cn

[T37] Lua：字符串拼接
来源：http://eoh.yj20258888.top

"a" .. "b"
来源：http://qfk.guannengcc.top

[T38] Lua：条件
来源：http://oxb.zhengqikj.top

if x > 0 then print("正") end
来源：http://yoi.birdmap.top

[T39] Lua：模式匹配
来源：http://iwo.sysykeji.top

string.find(s, "%d+")
来源：http://nbf.zhixingplan.top

[T40] Lua：元表
来源：http://otg.hnxiangtu.top

setmetatable({}, { __index = base })
来源：http://oas.daria6918.cn

[T41] Perl：Hello World
来源：http://ipi.bjfxy.top

print "Hello\n";
来源：http://ick.316326.xyz

[T42] Perl：变量类型
来源：http://qjt.ppjwa.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://qvf.daxiang520.top

[T43] Perl：字符串插值
来源：http://jrl.zhongyouzk.top

"值: $a"
来源：http://opa.fanxiaobao.xyz

[T44] Perl：条件
来源：http://roj.andypj.xyz

if ($a > 0) { print "正"; }
来源：http://knt.haohaochexian.top

[T45] Perl：数组遍历
来源：http://cpq.meibo888.top

for my $x (@arr) { print $x; }
来源：http://igp.fanxiaobao.xyz

[T46] Perl：哈希操作
来源：http://imw.guowangkeji.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://pyq.cucudq.cn

[T47] Perl：正则捕获
来源：http://pyh.hnxiangtu.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://twz.hnqzz.top

[T48] Perl：正则替换
来源：http://lub.ppjwa.cn

$s =~ s/old/new/g;
来源：http://udr.sufxvd.cn

[T49] Perl：函数
来源：http://rux.zdqjudy.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://jrl.chenjidiqi.icu

[T50] Perl：逐行读文件
来源：http://phl.smart0.xyz

open my $fh, "<", "a.txt" or die $!;
来源：http://bcl.yuxming.cn

while (my $line = <$fh>) { print $line; }
来源：http://cqv.chenlongwang.top

[T51] Scala：Hello World
来源：http://zkp.cqqwz.cn

println("Hello")
来源：http://zaa.cheryme.top

[T52] Scala：变量
来源：http://apa.hfpthk.cn

val a = 1;  var b = 2
来源：http://uii.0kj1m.cn

[T53] Scala：字符串插值
来源：http://gab.xinyue.icu

s"值: $b"
来源：http://bjg.tarul.cn

[T54] Scala：集合映射
来源：http://vdk.hywenlv.cn

List(1, 2, 3).map(_ * 2)
来源：http://seh.svipenyu.cn

[T55] Scala：集合过滤
来源：http://fxy.svipenyu.cn

List(1, 2, 3).filter(_ > 1)
来源：http://lwg.fktsv.cn

[T56] Scala：样例类
来源：http://mka.jqgfzy.top

case class User(name: String, age: Int)
来源：http://oif.yongpay.top

[T57] Scala：模式匹配
来源：http://oeb.guannengcc.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://orv.52xcode.cn

[T58] Scala：函数定义
来源：http://thv.hcnkem.com

def add(a: Int, b: Int): Int = a + b
来源：http://wej.fzhhl.top

[T59] Scala：循环
来源：http://key.jlsjyb.cn

for (i <- 1 to 10) println(i)
来源：http://tpv.zhixingplan.top

[T60] Scala：折叠
来源：http://gql.havefunace.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://ynh.jinghuilouyu.cn

================================================================================
来源：http://kbl.ehwqpu.com

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://wtu.ybcxt.top

================================================================================
来源：http://ffa.cucudq.cn

[U01] Py：创建虚拟环境
来源：http://cnv.pycfn.com

python -m venv .venv && source .venv/bin/activate
来源：http://ycd.cdnleiting.top

[U02] Py：导出 / 安装依赖
来源：http://lmn.chenlongwang.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://uiw.haohaochexian.top

[U03] Py：加载 .env 配置
来源：http://vms.gaohongyu789.top

from dotenv import load_dotenv; load_dotenv()
来源：http://bsm.xingfuxueyuan.xyz

[U04] Py：变量调试打印
来源：http://hwl.yuxming.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://rke.zdbjq.cn

[U05] Py：列表去重且保序
来源：http://aye.yonumen.top

list(dict.fromkeys(arr))
来源：http://xek.svipenyu.cn

[U06] Py：合并两个字典
来源：http://wad.daria6918.cn

{**a, **b}
来源：http://odn.guowangkeji.top

[U07] Py：反转字典键值
来源：http://ezf.ctjpmb.com

{v: k for k, v in d.items()}
来源：http://vgb.daria6918.cn

[U08] Py：展平二维列表
来源：http://rep.jyoumei.cn

[y for x in nested for y in x]
来源：http://fsr.hfpthk.cn

[U09] Py：字典取最大值的键
来源：http://ymt.quarkkingdee.top

max(d, key=d.get)
来源：http://oww.nanxuanxn.top

[U10] Py：按值排序字典
来源：http://nro.cqqwz.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://xrb.zhaomingkeji.xyz

[U11] Py：生成器表达式
来源：http://bur.fzhhl.top

(x * 2 for x in arr)
来源：http://rox.nwbrower.top

[U12] Py：取出现最多的 3 个元素
来源：http://wib.nanxuanxn.top

Counter(arr).most_common(3)
来源：http://exy.gogol.net.cn

[U13] Py：固定长度队列
来源：http://qte.xinyue.icu

deque(maxlen=10)
来源：http://jlh.gogol.net.cn

[U14] Py：分组收集到列表
来源：http://poe.cdnleiting.top

defaultdict(list)
来源：http://srw.dashuyun.cn

[U15] Py：高精度计时
来源：http://hzz.yuxming.cn

t = time.perf_counter()
来源：http://bhm.tian-w.cn

[U16] Py：命令行参数解析
来源：http://yzc.hongshengwenyu.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://rnu.yvedp.cn

[U17] Py：初始化日志
来源：http://abr.iojbl.cn

logging.basicConfig(level=logging.INFO)
来源：http://fqk.gaohongyu789.top

[U18] Py：预编译正则
来源：http://mdf.sxryk.cn

pat = re.compile(r"\d+")
来源：http://ble.cucudq.cn

[U19] Py：正则替换带回调
来源：http://ygu.sjlbkw.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://ren.c1oappe.top

[U20] Py：缓存函数结果
来源：http://vvq.yj20258888.top

@functools.lru_cache(maxsize=None)
来源：http://cur.yonumen.top

[U21] Py：自定义上下文管理器
来源：http://ooy.yonumen.top

@contextlib.contextmanager
来源：http://lch.hcnkem.com

[U22] Py：矩阵转置
来源：http://tda.shuidangran.top

list(zip(*m))
来源：http://vtz.vehdjk.com

[U23] Py：分块读取大文件
来源：http://gka.nanxinkj.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://kpi.guowangkeji.top

[U24] Py：路径操作
来源：http://pbo.kuanghao11.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://swj.chenzaomai.com

[U25] Py：CSV 按字典读
来源：http://ndb.yuanzhike.top

csv.DictReader(f)
来源：http://agr.sxryk.cn

[U26] Py：并发下载
来源：http://bqe.zhiwuduotai.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://drx.jianghu66.top

[U27] Py：异步 HTTP
来源：http://tod.fehbvm.com

aiohttp.ClientSession() 配合 async with
来源：http://byj.wangdashe.top

[U28] Py：类型别名
来源：http://ztb.xuetiantiany.cn

UserId = int
来源：http://ywg.yj202588.top

[U29] Py：属性校验
来源：http://laq.mhx1999.top

@property 与 @x.setter 配合
来源：http://zcv.fzhhl.top

[U30] Py：数据类
来源：http://alu.dashuyun.cn

@dataclass(slots=True)
来源：http://jgu.chenjidiqi.icu

[U31] Py：单测
来源：http://yzw.cdnleiting.top

python -m pytest -q
来源：http://mpv.bbcook.cn

[U32] Py：代码格式化
来源：http://exy.zhixingplan.top

ruff format . && ruff check --fix .
来源：http://zli.quarkkingdee.top

[U33] Py：打包发布
来源：http://hbx.hysaishi.cn

python -m build  （依赖 pyproject.toml）
来源：http://nlk.birdmap.top

[U34] Py：判断编码
来源：http://nei.cheryme.top

chardet.detect(raw)
来源：http://esj.cqqwz.cn

[U35] Py：发送邮件
来源：http://ero.jinqigfzy.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://lta.uphjek.com

[U36] Py：定时任务
来源：http://vjj.vqdsnc.cn

schedule.every(10).minutes.do(job)
来源：http://hyb.smart0.xyz

[U37] Py：读写 Excel
来源：http://vmf.yj20258888.top

pandas.read_excel / DataFrame.to_excel
来源：http://vpe.dianchejie.cn

[U38] Py：获取脚本所在目录
来源：http://nvy.cucudq.cn

Path(__file__).resolve().parent
来源：http://wut.yj202588.top

[U39] Py：判断是否在交互环境
来源：http://elm.xziqi.cn

sys.stdout.isatty()
来源：http://upg.jinqigfzy.top

[U40] Py：打印到标准错误
来源：http://sny.shzxlz.cn

print("err", file=sys.stderr)
来源：http://tex.cashguo.top

[U41] PHP：初始化 Composer 项目
来源：http://cqj.yuxming.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://ozp.hfpthk.cn

[U42] PHP：PSR-4 自动加载
来源：http://qvg.fanxiaobao.xyz

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://swk.chenzaomai.com

[U43] PHP：声明命名空间
来源：http://vnl.yj20258.top

namespace App\Http;
来源：http://rvn.andypj.xyz

[U44] PHP：开启严格类型
来源：http://jkf.jinqigufen.top

declare(strict_types=1);
来源：http://jkr.hesvh.cn

[U45] PHP：类型声明与返回类型
来源：http://oxw.zdbjq.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://whk.hnqzz.top

[U46] PHP：可空类型
来源：http://xbd.fktsv.cn

?string $name = null
来源：http://izh.hesvh.cn

[U47] PHP：联合类型
来源：http://ilc.guowangkeji.top

int|string $id
来源：http://hsv.chenjidiqi.icu

[U48] PHP：纯枚举
来源：http://pwt.fanxiaobao.xyz

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://ill.zhengqikj.top

[U49] PHP：只读属性
来源：http://lqf.daria6918.cn

public readonly string $name
来源：http://try.guannengcc.top

[U50] PHP：构造器属性提升
来源：http://cjn.hywenlv.cn

public function __construct(private int $id) {}
来源：http://agk.yfazqb.com

[U51] PHP：数组解构
来源：http://iaf.9152youxi.cn

[$a, $b] = $arr;
来源：http://uyd.dianchejie.cn

[U52] PHP：箭头函数
来源：http://aeh.fengsongda.top

$double = fn($x) => $x * 2;
来源：http://wsq.zhengqikj.top

[U53] PHP：空合并运算符
来源：http://ynp.ybcxt.top

$v = $a ?? $b ?? "default";
来源：http://kte.xuanzx.com

[U54] PHP：空安全调用
来源：http://rfs.hfpthk.cn

$obj?->method()
来源：http://ice.hammf.cn

[U55] PHP：match 表达式
来源：http://alm.shangyingyoupin.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://uvk.daxiang520.top

[U56] PHP：命名参数
来源：http://vsw.aizwys.cn

f(a: 1, b: 2)
来源：http://pbe.hcnkem.com

[U57] PHP：字符串插值
来源：http://xly.jiagoushi.top

"值: {$a}"
来源：http://sep.gzhubu.top

[U58] PHP：数组三件套
来源：http://mli.zhiwuduotai.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://qah.aizwys.cn

[U59] PHP：自定义排序
来源：http://itx.zhaomingkeji.xyz

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://zxx.0kj1m.cn

[U60] PHP：JSON 编解码
来源：http://qtf.yueranfly.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://peh.fengsongda.top

[U61] PHP：正则
来源：http://uqx.guowangkeji.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://orb.fktsv.cn

[U62] PHP：日期对象
来源：http://rsu.yuanzhike.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://uhf.vqdsnc.cn

[U63] PHP：文件读写
来源：http://zjo.daxiang520.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://kku.yuanzhike.top

[U64] PHP：目录遍历
来源：http://zrs.zhijiandao.cn

glob("dir/*.php");  scandir("dir");
来源：http://hyt.sjlbkw.cn

[U65] PHP：会话
来源：http://oou.hysaishi.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://tmd.fengsongda.top

[U66] PHP：设置 Cookie
来源：http://gmo.sweek.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://dtm.chenzaomai.com

[U67] PHP：处理文件上传
来源：http://vze.pycfn.com

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://lmt.cucudq.cn

[U68] PHP：PDO 连接
来源：http://xfo.mhx1999.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://scd.shangyingyoupin.top

[U69] PHP：PDO 预处理
来源：http://kkl.tian-w.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://kzp.havefunace.top

[U70] PHP：PDO 事务
来源：http://azm.guowangkeji.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://nvx.ctjpmb.com

[U71] PHP：抛出异常
来源：http://agm.shangyingyoupin.top

throw new RuntimeException("失败", 500);
来源：http://lng.aibaodan.cn

[U72] PHP：写错误日志
来源：http://ucr.sufxvd.cn

error_log("失败: " . $e->getMessage());
来源：http://jdc.snrcjt.cn

[U73] PHP：读取 ini 配置
来源：http://ylh.ywan-chungtsiang.top

parse_ini_file("config.ini", true)
来源：http://rbw.daria6918.cn

[U74] PHP：读取环境变量
来源：http://lru.feifeiyinyue.top

getenv("APP_ENV") ?: "production"
来源：http://eit.yuxming.cn

[U75] PHP：依赖注入
来源：http://hmz.shangyingyoupin.top

composer require psr/container
来源：http://ibw.yj20258.top

[U76] PHP：简单路由
来源：http://ntm.cqqwz.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://lsg.cucudq.cn

[U77] PHP：模板渲染
来源：http://cfw.316326.xyz

composer require twig/twig
来源：http://lfz.tanke756.top

[U78] PHP：单元测试
来源：http://fgb.uphjek.com

composer require --dev phpunit/phpunit
来源：http://jme.daria6918.cn

[U79] PHP：静态分析
来源：http://mls.0kj1m.cn

composer require --dev phpstan/phpstan
来源：http://kpn.tanke756.top

[U80] PHP：代码规范修复
来源：http://djl.aibaodan.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://wjl.chenlongwang.top

[U81] JS：初始化项目
来源：http://psh.pengpengdd.cyou

npm init -y;  npm i express
来源：http://erz.yanxiufei.cn

[U82] JS：package.json 脚本
来源：http://wzd.zhixingplan.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://idu.yongpay.top

[U83] JS：ES Module 导入导出
来源：http://tkl.zycfv.cn

export const a = 1;  import { a } from "./m.js";
来源：http://tga.uphjek.com

[U84] JS：CommonJS 写法
来源：http://yza.jinyuanbaomall.cn

module.exports = { a };  const { a } = require("./m");
来源：http://kcw.yj202588.top

[U85] JS：可选链
来源：http://jap.cqqwz.cn

a?.b?.c
来源：http://ogp.zhaomingkeji.xyz

[U86] JS：空值合并
来源：http://pgz.pengpengdd.cyou

a ?? b
来源：http://avd.ctjpmb.com

[U87] JS：解构默认值
来源：http://wkm.jinqigfzy.top

const { a = 1, b = 2 } = obj;
来源：http://ylc.snrcjt.cn

[U88] JS：对象展开合并
来源：http://imf.hammf.cn

{ ...a, ...b }
来源：http://zpe.fzhhl.top

[U89] JS：数组去重
来源：http://utn.zdqjudy.top

[...new Set(arr)]
来源：http://mwx.yuxming.cn

[U90] JS：数字数组排序
来源：http://xmd.kuanghao11.cn

[...arr].sort((a, b) => a - b)
来源：http://sxi.yj20258.top

[U91] JS：对象键值遍历
来源：http://oto.zhaomingkeji.xyz

Object.entries(obj).forEach(([k, v]) => {});
来源：http://jhe.jinyuanbaomall.cn

[U92] JS：深拷贝
来源：http://ncv.dianchejie.cn

structuredClone(obj)
来源：http://ekb.redwolf501.top

[U93] JS：模板字符串
来源：http://wdl.ywan-chungtsiang.top

`共 ${n} 条`
来源：http://sdq.hysaishi.cn

[U94] JS：箭头函数
来源：http://bwf.nanxuanxn.top

const double = x => x * 2;
来源：http://tps.redwolf501.top

[U95] JS：Promise 包装
来源：http://tlz.sjlbkw.cn

new Promise((resolve, reject) => {})
来源：http://kly.gotoacloud.top

[U96] JS：async/await 与异常
来源：http://kal.hongshengwenyu.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hro.haohaochexian.top

[U97] JS：并发请求
来源：http://nyw.jinqigfzy.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://uks.hywenlv.cn

[U98] JS：fetch 带 JSON
来源：http://kxq.pycfn.com

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://ssh.yvedp.cn

[U99] JS：事件监听
来源：http://axh.yueranfly.top

el.addEventListener("click", e => {})
来源：http://wot.tarul.cn

[U100] JS：DOM 查询
来源：http://xvv.ivvv.top

document.querySelector(".item")
来源：http://nsh.svipenyu.cn

[U101] JS：classList 操作
来源：http://djq.hcnkem.com

el.classList.toggle("active")
来源：http://gcr.zdqjudy.top

[U102] JS：本地存储
来源：http://yfy.hcnkem.com

localStorage.setItem("k", JSON.stringify(v))
来源：http://zek.cheryme.top

[U103] JS：定时器
来源：http://wgm.iojbl.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://arj.zhijiandao.cn

[U104] JS：防抖
来源：http://mun.pengpengdd.cyou

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mso.hywenlv.cn

[U105] JS：节流
来源：http://zyr.havefunace.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://ggo.xziqi.cn

[U106] JS：日期格式化
来源：http://ncc.gogol.net.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hhk.zhongyouzk.top

[U107] JS：数字千分位
来源：http://lyh.yonumen.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://ycp.gogol.net.cn

[U108] JS：随机整数
来源：http://owg.shuidangran.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://voc.epnwcf.com

[U109] JS：数组分组
来源：http://zje.redwolf501.top

Object.groupBy(arr, x => x.type)
来源：http://bhh.jinqigfzy.top

[U110] JS：数组分块
来源：http://var.hnxiangtu.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://zjo.jiagoushi.top

[U111] JS：对象转 Map
来源：http://kjq.ywan-chungtsiang.top

new Map(Object.entries(obj))
来源：http://shn.xingfuxueyuan.xyz

[U112] JS：字符串补位
来源：http://ysf.yuxming.cn

"7".padStart(3, "0")
来源：http://uym.pycfn.com

[U113] JS：正则替换全部
来源：http://clk.cashguo.top

s.replaceAll("a", "b")
来源：http://mon.ybcxt.top

[U114] JS：JSON 深比较
来源：http://frm.jianghu66.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://dgt.yuxming.cn

[U115] JS：生成 UUID
来源：http://wpo.sxryk.cn

crypto.randomUUID()
来源：http://xro.tanke756.top

[U116] JS：类型检查（JSDoc）
来源：http://cpj.nwbrower.top

/** @param {string} name */ function f(name) {}
来源：http://jei.andypj.xyz

[U117] JS：单元测试
来源：http://som.pengpengdd.cyou

npm i -D vitest;  npx vitest
来源：http://lig.9152youxi.cn

[U118] JS：开发服务器
来源：http://jhx.ywan-chungtsiang.top

npm i -D vite;  npx vite
来源：http://wpb.xuanzx.com

[U119] JS：生产构建
来源：http://ory.quarkkingdee.top

npx vite build
来源：http://ozb.hammf.cn

[U120] JS：读取环境变量（Vite）
来源：http://wqh.bjfxy.top

import.meta.env.VITE_API_URL
来源：http://pgw.cheryme.top

================================================================================
来源：http://zvu.yj202588.top

统计汇总
来源：http://nod.gaohongyu789.top

================================================================================
来源：http://xoa.yueranfly.top

按语言统计（条）：
来源：http://pxg.tianlin.xyz


<!-- 参考信息 -->