代发 wailian999

[T21] Swift：遍历
来源：http://xww.xuetiantiany.cn

for x in a { print(x) }
来源：http://hnk.kuanghao11.cn

[T22] Swift：字典
来源：http://msj.xuanzx.com

var d = ["a": 1];  d["b"] = 2
来源：http://uph.vehdjk.com

[T23] Swift：函数
来源：http://pyn.tarul.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://igz.gotoacloud.top

[T24] Swift：闭包
来源：http://qym.jqgufenzy.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://bqh.hnqzz.top

[T25] Swift：结构体
来源：http://abq.zhoulong.xyz

struct P { var x: Int }
来源：http://ord.iojbl.cn

[T26] Swift：类与重写
来源：http://gxb.yueranfly.top

class A: Base { override func f() {} }
来源：http://pfp.fzhhl.top

[T27] Swift：错误处理
来源：http://ekw.zhaomingkeji.xyz

do { try f() } catch { print(error) }
来源：http://cdg.zhaomingkeji.xyz

[T28] Swift：枚举
来源：http://hey.nanxinkj.top

enum Color { case red, green }
来源：http://dau.andypj.xyz

[T29] Swift：guard 提前返回
来源：http://nzv.nanxinkj.top

guard let x = opt else { return }
来源：http://vfg.guowangkeji.top

[T30] Swift：协议
来源：http://rvx.hnxiangtu.top

protocol Shape { func area() -> Double }
来源：http://xqe.aizwys.cn

[T31] Lua：Hello World
来源：http://fep.tian-w.cn

print("Hello")
来源：http://uth.zdbjq.cn

[T32] Lua：局部变量
来源：http://oip.ydzc1.top

local a = 1
来源：http://nfe.hysaishi.cn

[T33] Lua：表（数组）
来源：http://yai.0kj1m.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://woi.daxiang520.top

[T34] Lua：遍历表
来源：http://zpo.guannengcc.top

for i, v in ipairs(t) do print(i, v) end
来源：http://ttw.ehwqpu.com

[T35] Lua：字典表
来源：http://tlh.uphjek.com

local d = { a = 1 };  d.b = 2
来源：http://saf.ppjwa.cn

[T36] Lua：函数
来源：http://jxe.zhaomingkeji.xyz

function add(a, b) return a + b end
来源：http://rom.yfazqb.com

[T37] Lua：字符串拼接
来源：http://dbl.yonumen.top

"a" .. "b"
来源：http://bxr.fehbvm.com

[T38] Lua：条件
来源：http://ndh.ydzc1.top

if x > 0 then print("正") end
来源：http://ukn.chenjidiqi.icu

[T39] Lua：模式匹配
来源：http://lgw.hywenlv.cn

string.find(s, "%d+")
来源：http://nnl.guowangkeji.top

[T40] Lua：元表
来源：http://oue.smart0.xyz

setmetatable({}, { __index = base })
来源：http://cid.iojbl.cn

[T41] Perl：Hello World
来源：http://ozj.snrcjt.cn

print "Hello\n";
来源：http://qrb.c1oappe.top

[T42] Perl：变量类型
来源：http://tna.tian-w.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://lsm.shanyushiyangtech.top

[T43] Perl：字符串插值
来源：http://suc.nwbrower.top

"值: $a"
来源：http://djk.fanxiaobao.xyz

[T44] Perl：条件
来源：http://jhn.jqgufenzy.top

if ($a > 0) { print "正"; }
来源：http://cmg.kuanghao11.cn

[T45] Perl：数组遍历
来源：http://nmk.fktsv.cn

for my $x (@arr) { print $x; }
来源：http://enz.daria6918.cn

[T46] Perl：哈希操作
来源：http://juw.cheryme.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://bav.chenlongwang.top

[T47] Perl：正则捕获
来源：http://xof.xziqi.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://ujl.hysaishi.cn

[T48] Perl：正则替换
来源：http://wer.andypj.xyz

$s =~ s/old/new/g;
来源：http://ulq.havefunace.top

[T49] Perl：函数
来源：http://ikq.redwolf501.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://vcd.uphjek.com

[T50] Perl：逐行读文件
来源：http://qnq.chenjidiqi.icu

open my $fh, "<", "a.txt" or die $!;
来源：http://tdw.gzhubu.top

while (my $line = <$fh>) { print $line; }
来源：http://phx.9152youxi.cn

[T51] Scala：Hello World
来源：http://hfm.gogol.net.cn

println("Hello")
来源：http://tyz.jinyuanbaomall.cn

[T52] Scala：变量
来源：http://tlc.ppjwa.cn

val a = 1;  var b = 2
来源：http://sxs.xingfuxueyuan.xyz

[T53] Scala：字符串插值
来源：http://xbc.vqdsnc.cn

s"值: $b"
来源：http://iya.9152youxi.cn

[T54] Scala：集合映射
来源：http://uos.quarkkingdee.top

List(1, 2, 3).map(_ * 2)
来源：http://gdd.zdbjq.cn

[T55] Scala：集合过滤
来源：http://svk.hammf.cn

List(1, 2, 3).filter(_ > 1)
来源：http://hnx.sjlbkw.cn

[T56] Scala：样例类
来源：http://khr.fengsongda.top

case class User(name: String, age: Int)
来源：http://fco.wangshuangyany.cn

[T57] Scala：模式匹配
来源：http://leo.zhijiandao.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://mah.shuidangran.top

[T58] Scala：函数定义
来源：http://cep.cheryme.top

def add(a: Int, b: Int): Int = a + b
来源：http://ghj.pycfn.com

[T59] Scala：循环
来源：http://xnb.hnxiangtu.top

for (i <- 1 to 10) println(i)
来源：http://vdo.shanyushiyangtech.top

[T60] Scala：折叠
来源：http://eae.pycfn.com

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://obt.ehwqpu.com

================================================================================
来源：http://srm.tanke756.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://gph.ydjk.org.cn

================================================================================
来源：http://txf.316326.xyz

[U01] Py：创建虚拟环境
来源：http://nkq.jlsjyb.cn

python -m venv .venv && source .venv/bin/activate
来源：http://res.hywenlv.cn

[U02] Py：导出 / 安装依赖
来源：http://iqu.xinyue.icu

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://rch.yanxiufei.cn

[U03] Py：加载 .env 配置
来源：http://ulx.jiagoushi.top

from dotenv import load_dotenv; load_dotenv()
来源：http://mrd.snrcjt.cn

[U04] Py：变量调试打印
来源：http://euf.pengpengdd.cyou

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://jaf.yanxiufei.cn

[U05] Py：列表去重且保序
来源：http://tdq.shanyushiyangkeji.top

list(dict.fromkeys(arr))
来源：http://cjj.bbcook.cn

[U06] Py：合并两个字典
来源：http://lix.guowangkeji.top

{**a, **b}
来源：http://glp.nanxuanxn.top

[U07] Py：反转字典键值
来源：http://lic.tianlin.xyz

{v: k for k, v in d.items()}
来源：http://kvg.jyoumei.cn

[U08] Py：展平二维列表
来源：http://xwi.bbcook.cn

[y for x in nested for y in x]
来源：http://nii.zhixingplan.top

[U09] Py：字典取最大值的键
来源：http://olu.dianchejie.cn

max(d, key=d.get)
来源：http://xsi.tanke756.top

[U10] Py：按值排序字典
来源：http://hzw.birdmap.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://uch.sysykeji.top

[U11] Py：生成器表达式
来源：http://uye.52xcode.cn

(x * 2 for x in arr)
来源：http://oqc.yuanzhike.top

[U12] Py：取出现最多的 3 个元素
来源：http://ahp.fanxiaobao.xyz

Counter(arr).most_common(3)
来源：http://rue.xuanzx.com

[U13] Py：固定长度队列
来源：http://uoj.cheryme.top

deque(maxlen=10)
来源：http://zwj.zdqjudy.top

[U14] Py：分组收集到列表
来源：http://hkv.xziqi.cn

defaultdict(list)
来源：http://ezx.jianghu66.top

[U15] Py：高精度计时
来源：http://mkm.jianghu66.top

t = time.perf_counter()
来源：http://axf.shanyushiyangkeji.top

[U16] Py：命令行参数解析
来源：http://auq.yvedp.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://sty.xinyue.icu

[U17] Py：初始化日志
来源：http://ajc.fanxiaobao.xyz

logging.basicConfig(level=logging.INFO)
来源：http://xzk.ydzc1.top

[U18] Py：预编译正则
来源：http://ack.zdbjq.cn

pat = re.compile(r"\d+")
来源：http://yvd.uphjek.com

[U19] Py：正则替换带回调
来源：http://isu.fengsongda.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://nuj.birdmap.top

[U20] Py：缓存函数结果
来源：http://mce.fktsv.cn

@functools.lru_cache(maxsize=None)
来源：http://owp.ybcxt.top

[U21] Py：自定义上下文管理器
来源：http://rrz.nanxuanxn.top

@contextlib.contextmanager
来源：http://nkv.bbcook.cn

[U22] Py：矩阵转置
来源：http://wsn.fktsv.cn

list(zip(*m))
来源：http://jcb.uphjek.com

[U23] Py：分块读取大文件
来源：http://qyg.jiagoushi.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://lwi.yongpay.top

[U24] Py：路径操作
来源：http://mcc.zhixingplan.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://brh.mhx1999.top

[U25] Py：CSV 按字典读
来源：http://afe.ppjwa.cn

csv.DictReader(f)
来源：http://irt.cashguo.top

[U26] Py：并发下载
来源：http://ydm.ydzc1.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://xdv.shangyingyoupin.top

[U27] Py：异步 HTTP
来源：http://gmm.sufxvd.cn

aiohttp.ClientSession() 配合 async with
来源：http://gmi.dianchejie.cn

[U28] Py：类型别名
来源：http://cta.redwolf501.top

UserId = int
来源：http://fmk.smart0.xyz

[U29] Py：属性校验
来源：http://ljk.mhx1999.top

@property 与 @x.setter 配合
来源：http://gby.cqqwz.cn

[U30] Py：数据类
来源：http://xeh.xinyue.icu

@dataclass(slots=True)
来源：http://qbs.yfazqb.com

[U31] Py：单测
来源：http://xhr.wangdashe.top

python -m pytest -q
来源：http://rfd.chenzaomai.com

[U32] Py：代码格式化
来源：http://avw.andypj.xyz

ruff format . && ruff check --fix .
来源：http://xfg.yanxiufei.cn

[U33] Py：打包发布
来源：http://oit.ybcxt.top

python -m build  （依赖 pyproject.toml）
来源：http://xhe.redwolf501.top

[U34] Py：判断编码
来源：http://iph.yanxiufei.cn

chardet.detect(raw)
来源：http://ypm.sxryk.cn

[U35] Py：发送邮件
来源：http://cgv.yj20258888.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://zhi.smart0.xyz

[U36] Py：定时任务
来源：http://tfn.jiagoushi.top

schedule.every(10).minutes.do(job)
来源：http://ecf.kuanghao11.cn

[U37] Py：读写 Excel
来源：http://nuq.ydzc1.top

pandas.read_excel / DataFrame.to_excel
来源：http://dqb.shanyushiyangtech.top

[U38] Py：获取脚本所在目录
来源：http://nwg.jinyuanbaomall.cn

Path(__file__).resolve().parent
来源：http://iqy.316326.xyz

[U39] Py：判断是否在交互环境
来源：http://pti.shanyushiyangkeji.top

sys.stdout.isatty()
来源：http://voa.yueranfly.top

[U40] Py：打印到标准错误
来源：http://rgq.shanyushiyangtech.top

print("err", file=sys.stderr)
来源：http://jdz.dianchejie.cn

[U41] PHP：初始化 Composer 项目
来源：http://afk.shanyushiyangtech.top

composer init;  composer require guzzlehttp/guzzle
来源：http://gxi.vehdjk.com

[U42] PHP：PSR-4 自动加载
来源：http://xrk.zhiwuduotai.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://yma.tarul.cn

[U43] PHP：声明命名空间
来源：http://icc.andypj.xyz

namespace App\Http;
来源：http://dti.yuxming.cn

[U44] PHP：开启严格类型
来源：http://fyf.fzhhl.top

declare(strict_types=1);
来源：http://tgj.cqqwz.cn

[U45] PHP：类型声明与返回类型
来源：http://ykr.meibo888.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://hfb.316326.xyz

[U46] PHP：可空类型
来源：http://vuf.chenjidiqi.icu

?string $name = null
来源：http://zph.xylfe.cn

[U47] PHP：联合类型
来源：http://eyi.shuidangran.top

int|string $id
来源：http://ohi.jinghuilouyu.cn

[U48] PHP：纯枚举
来源：http://tbg.pycfn.com

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://doe.yueranfly.top

[U49] PHP：只读属性
来源：http://nhj.mhx1999.top

public readonly string $name
来源：http://pqi.zhengqikj.top

[U50] PHP：构造器属性提升
来源：http://sik.nanxinkj.top

public function __construct(private int $id) {}
来源：http://pio.aizwys.cn

[U51] PHP：数组解构
来源：http://lwj.jinghuilouyu.cn

[$a, $b] = $arr;
来源：http://xak.shzxlz.cn

[U52] PHP：箭头函数
来源：http://etu.yanxiufei.cn

$double = fn($x) => $x * 2;
来源：http://njs.jlsjyb.cn

[U53] PHP：空合并运算符
来源：http://bqo.kuanghao11.cn

$v = $a ?? $b ?? "default";
来源：http://ovw.dashuyun.cn

[U54] PHP：空安全调用
来源：http://drz.gaohongyu789.top

$obj?->method()
来源：http://asg.fengsongda.top

[U55] PHP：match 表达式
来源：http://pcm.iojbl.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://iqr.yonumen.top

[U56] PHP：命名参数
来源：http://urr.ydjk.org.cn

f(a: 1, b: 2)
来源：http://zpp.fktsv.cn

[U57] PHP：字符串插值
来源：http://ysi.gogol.net.cn

"值: {$a}"
来源：http://bvk.daxiang520.top

[U58] PHP：数组三件套
来源：http://dyw.yanxiufei.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://qth.gzhubu.top

[U59] PHP：自定义排序
来源：http://jxy.tianlin.xyz

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://waq.sysykeji.top

[U60] PHP：JSON 编解码
来源：http://zfl.zhoulong.xyz

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://amf.shangyingyoupin.top

[U61] PHP：正则
来源：http://mkw.ppjwa.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://wau.jiagoushi.top

[U62] PHP：日期对象
来源：http://crq.iojbl.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://uvq.yanxiufei.cn

[U63] PHP：文件读写
来源：http://cct.ehwqpu.com

file_get_contents($f);  file_put_contents($f, $data);
来源：http://ffr.52xcode.cn

[U64] PHP：目录遍历
来源：http://ryh.fzhhl.top

glob("dir/*.php");  scandir("dir");
来源：http://edf.svipenyu.cn

[U65] PHP：会话
来源：http://rmu.jinqigufen.top

session_start();  $_SESSION["uid"] = 1;
来源：http://nex.ydjk.org.cn

[U66] PHP：设置 Cookie
来源：http://uxz.aibaodan.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://wiw.zhengqikj.top

[U67] PHP：处理文件上传
来源：http://xvw.jinghuilouyu.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://ugo.iojbl.cn

[U68] PHP：PDO 连接
来源：http://hek.kuanghao11.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://kff.guowangkeji.top

[U69] PHP：PDO 预处理
来源：http://nek.sxryk.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://qux.gaohongyu789.top

[U70] PHP：PDO 事务
来源：http://bil.daria6918.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://fyj.havefunace.top

[U71] PHP：抛出异常
来源：http://smv.tian-w.cn

throw new RuntimeException("失败", 500);
来源：http://mte.ywan-chungtsiang.top

[U72] PHP：写错误日志
来源：http://svk.gaohongyu789.top

error_log("失败: " . $e->getMessage());
来源：http://uvg.xziqi.cn

[U73] PHP：读取 ini 配置
来源：http://azu.sufxvd.cn

parse_ini_file("config.ini", true)
来源：http://mki.ywan-chungtsiang.top

[U74] PHP：读取环境变量
来源：http://trt.cdnleiting.top

getenv("APP_ENV") ?: "production"
来源：http://nnb.yongpay.top

[U75] PHP：依赖注入
来源：http://phc.yonumen.top

composer require psr/container
来源：http://rbu.zhaomingkeji.xyz

[U76] PHP：简单路由
来源：http://rxy.aibaodan.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://ztu.hcnkem.com

[U77] PHP：模板渲染
来源：http://npv.jyoumei.cn

composer require twig/twig
来源：http://usd.sweek.top

[U78] PHP：单元测试
来源：http://ocf.ppjwa.cn

composer require --dev phpunit/phpunit
来源：http://csm.yj202588.top

[U79] PHP：静态分析
来源：http://hoj.zdbjq.cn

composer require --dev phpstan/phpstan
来源：http://qxm.shanyushiyangkeji.top

[U80] PHP：代码规范修复
来源：http://ivw.guowangkeji.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://pif.jyoumei.cn

[U81] JS：初始化项目
来源：http://pyj.daxiang520.top

npm init -y;  npm i express
来源：http://gsj.pycfn.com

[U82] JS：package.json 脚本
来源：http://qwh.guannengcc.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://iww.zycfv.cn

[U83] JS：ES Module 导入导出
来源：http://fzx.yongpay.top

export const a = 1;  import { a } from "./m.js";
来源：http://set.gotoacloud.top

[U84] JS：CommonJS 写法
来源：http://jop.kuanghao11.cn

module.exports = { a };  const { a } = require("./m");
来源：http://slv.ppjwa.cn

[U85] JS：可选链
来源：http://xpa.hammf.cn

a?.b?.c
来源：http://ztu.hcnkem.com

[U86] JS：空值合并
来源：http://cxy.shanyushiyangtech.top

a ?? b
来源：http://xnx.svipenyu.cn

[U87] JS：解构默认值
来源：http://gzk.hysaishi.cn

const { a = 1, b = 2 } = obj;
来源：http://kqd.cashguo.top

[U88] JS：对象展开合并
来源：http://cbl.vqdsnc.cn

{ ...a, ...b }
来源：http://aya.zhijiandao.cn

[U89] JS：数组去重
来源：http://yaz.jyoumei.cn

[...new Set(arr)]
来源：http://avn.xingfuxueyuan.xyz

[U90] JS：数字数组排序
来源：http://vjw.gotoacloud.top

[...arr].sort((a, b) => a - b)
来源：http://dxv.meibo888.top

[U91] JS：对象键值遍历
来源：http://anu.yongpay.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://zas.ivvv.top

[U92] JS：深拷贝
来源：http://jrq.cheryme.top

structuredClone(obj)
来源：http://dop.xylfe.cn

[U93] JS：模板字符串
来源：http://fhi.jiagoushi.top

`共 ${n} 条`
来源：http://evo.ydjk.org.cn

[U94] JS：箭头函数
来源：http://yez.ywan-chungtsiang.top

const double = x => x * 2;
来源：http://guz.ywan-chungtsiang.top

[U95] JS：Promise 包装
来源：http://agj.snrcjt.cn

new Promise((resolve, reject) => {})
来源：http://jml.shuidangran.top

[U96] JS：async/await 与异常
来源：http://cef.kuanghao11.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://cac.ctjpmb.com

[U97] JS：并发请求
来源：http://wgi.gzhubu.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://jfo.hysaishi.cn

[U98] JS：fetch 带 JSON
来源：http://bng.zycfv.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://sil.daxiang520.top

[U99] JS：事件监听
来源：http://kcg.chenjidiqi.icu

el.addEventListener("click", e => {})
来源：http://pui.ywan-chungtsiang.top

[U100] JS：DOM 查询
来源：http://irb.vqdsnc.cn

document.querySelector(".item")
来源：http://cop.pengpengdd.cyou

[U101] JS：classList 操作
来源：http://mjv.yj20258.top

el.classList.toggle("active")
来源：http://bex.kuanghao11.cn

[U102] JS：本地存储
来源：http://gqt.svipenyu.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://wqu.316326.xyz

[U103] JS：定时器
来源：http://xlj.316326.xyz

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://nqz.tarul.cn

[U104] JS：防抖
来源：http://sov.jqgfzy.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://rpj.jinqigfzy.top

[U105] JS：节流
来源：http://isb.ydzc1.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://gtc.gogol.net.cn

[U106] JS：日期格式化
来源：http://pta.svipenyu.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.xingfuxueyuan.xyz

[U107] JS：数字千分位
来源：http://vmx.yuanzhike.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://zqo.ivvv.top

[U108] JS：随机整数
来源：http://pcz.ctjpmb.com

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://ebw.zhiwuduotai.top


<!-- 参考信息 -->