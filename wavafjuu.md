代发 wailian999

[T25] Swift：结构体
来源：http://svn.jqgfzy.top

struct P { var x: Int }
来源：http://npa.zhoulong.xyz

[T26] Swift：类与重写
来源：http://soc.fehbvm.com

class A: Base { override func f() {} }
来源：http://utd.fanxiaobao.xyz

[T27] Swift：错误处理
来源：http://dpx.kuanghao11.cn

do { try f() } catch { print(error) }
来源：http://ulf.jqgfzy.top

[T28] Swift：枚举
来源：http://mwp.yongpay.top

enum Color { case red, green }
来源：http://hzj.yuxming.cn

[T29] Swift：guard 提前返回
来源：http://gwd.tanke756.top

guard let x = opt else { return }
来源：http://dnv.yongpay.top

[T30] Swift：协议
来源：http://tfy.redwolf501.top

protocol Shape { func area() -> Double }
来源：http://oki.jianghu66.top

[T31] Lua：Hello World
来源：http://kkh.jinqigufen.top

print("Hello")
来源：http://byp.svipenyu.cn

[T32] Lua：局部变量
来源：http://njz.xylfe.cn

local a = 1
来源：http://lft.sxryk.cn

[T33] Lua：表（数组）
来源：http://ljj.52xcode.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://byl.nanxinkj.top

[T34] Lua：遍历表
来源：http://jde.zhongyouzk.top

for i, v in ipairs(t) do print(i, v) end
来源：http://fhb.smart0.xyz

[T35] Lua：字典表
来源：http://azx.jlsjyb.cn

local d = { a = 1 };  d.b = 2
来源：http://sws.zhaomingkeji.xyz

[T36] Lua：函数
来源：http://tyz.fktsv.cn

function add(a, b) return a + b end
来源：http://kmt.nanxinkj.top

[T37] Lua：字符串拼接
来源：http://ike.xingfuxueyuan.xyz

"a" .. "b"
来源：http://fvg.hysaishi.cn

[T38] Lua：条件
来源：http://ump.ywan-chungtsiang.top

if x > 0 then print("正") end
来源：http://awv.dianchejie.cn

[T39] Lua：模式匹配
来源：http://pkm.xziqi.cn

string.find(s, "%d+")
来源：http://coq.yongpay.top

[T40] Lua：元表
来源：http://ssm.sxryk.cn

setmetatable({}, { __index = base })
来源：http://tuf.iojbl.cn

[T41] Perl：Hello World
来源：http://cft.gaohongyu789.top

print "Hello\n";
来源：http://slk.zdbjq.cn

[T42] Perl：变量类型
来源：http://qlj.tian-w.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://rjl.svipenyu.cn

[T43] Perl：字符串插值
来源：http://khe.hnqzz.top

"值: $a"
来源：http://yhz.jiagoushi.top

[T44] Perl：条件
来源：http://vms.dashuyun.cn

if ($a > 0) { print "正"; }
来源：http://oiw.quarkkingdee.top

[T45] Perl：数组遍历
来源：http://ivn.sysykeji.top

for my $x (@arr) { print $x; }
来源：http://sha.xuanzx.com

[T46] Perl：哈希操作
来源：http://dww.gogol.net.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://bbo.sufxvd.cn

[T47] Perl：正则捕获
来源：http://fhk.hysaishi.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://mlw.yonumen.top

[T48] Perl：正则替换
来源：http://yxy.fktsv.cn

$s =~ s/old/new/g;
来源：http://jbk.jinyuanbaomall.cn

[T49] Perl：函数
来源：http://mei.zhoulong.xyz

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://mdk.birdmap.top

[T50] Perl：逐行读文件
来源：http://odt.c1oappe.top

open my $fh, "<", "a.txt" or die $!;
来源：http://dmo.svipenyu.cn

while (my $line = <$fh>) { print $line; }
来源：http://ngo.shangyingyoupin.top

[T51] Scala：Hello World
来源：http://elx.andypj.xyz

println("Hello")
来源：http://qyz.pengpengdd.cyou

[T52] Scala：变量
来源：http://nlg.shanyushiyangtech.top

val a = 1;  var b = 2
来源：http://wss.hysaishi.cn

[T53] Scala：字符串插值
来源：http://xff.yonumen.top

s"值: $b"
来源：http://hnz.yvedp.cn

[T54] Scala：集合映射
来源：http://hzu.yvedp.cn

List(1, 2, 3).map(_ * 2)
来源：http://xjj.xylfe.cn

[T55] Scala：集合过滤
来源：http://uxt.ydjk.org.cn

List(1, 2, 3).filter(_ > 1)
来源：http://qzr.sxryk.cn

[T56] Scala：样例类
来源：http://lgc.sufxvd.cn

case class User(name: String, age: Int)
来源：http://jzk.ybcxt.top

[T57] Scala：模式匹配
来源：http://vjf.xziqi.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://mcj.jyoumei.cn

[T58] Scala：函数定义
来源：http://brx.tianlin.xyz

def add(a: Int, b: Int): Int = a + b
来源：http://cgw.yongpay.top

[T59] Scala：循环
来源：http://uid.meibo888.top

for (i <- 1 to 10) println(i)
来源：http://iqg.quarkkingdee.top

[T60] Scala：折叠
来源：http://dnq.shuidangran.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://asn.chenzaomai.com

================================================================================
来源：http://lcb.c1oappe.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://abo.xuanzx.com

================================================================================
来源：http://cmq.cqqwz.cn

[U01] Py：创建虚拟环境
来源：http://wtd.yuxming.cn

python -m venv .venv && source .venv/bin/activate
来源：http://khz.chenlongwang.top

[U02] Py：导出 / 安装依赖
来源：http://yiu.nwbrower.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://dcs.shzxlz.cn

[U03] Py：加载 .env 配置
来源：http://qph.hywenlv.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://lxr.birdmap.top

[U04] Py：变量调试打印
来源：http://bwn.tanke756.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://mlx.hnqzz.top

[U05] Py：列表去重且保序
来源：http://jqo.zhijiandao.cn

list(dict.fromkeys(arr))
来源：http://jyt.smart0.xyz

[U06] Py：合并两个字典
来源：http://ijt.haohaochexian.top

{**a, **b}
来源：http://fsz.sjlbkw.cn

[U07] Py：反转字典键值
来源：http://gze.shanyushiyangtech.top

{v: k for k, v in d.items()}
来源：http://iso.daxiang520.top

[U08] Py：展平二维列表
来源：http://znw.yj20258.top

[y for x in nested for y in x]
来源：http://aqv.hongshengwenyu.top

[U09] Py：字典取最大值的键
来源：http://dit.zycfv.cn

max(d, key=d.get)
来源：http://npj.yj20258888.top

[U10] Py：按值排序字典
来源：http://skz.guowangkeji.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://aja.chenlongwang.top

[U11] Py：生成器表达式
来源：http://wyk.meibo888.top

(x * 2 for x in arr)
来源：http://bqw.hywenlv.cn

[U12] Py：取出现最多的 3 个元素
来源：http://xqs.sysykeji.top

Counter(arr).most_common(3)
来源：http://wwt.dashuyun.cn

[U13] Py：固定长度队列
来源：http://diu.jinqigfzy.top

deque(maxlen=10)
来源：http://cvf.316326.xyz

[U14] Py：分组收集到列表
来源：http://cyk.yvedp.cn

defaultdict(list)
来源：http://szv.vehdjk.com

[U15] Py：高精度计时
来源：http://wqe.hywenlv.cn

t = time.perf_counter()
来源：http://mam.ehwqpu.com

[U16] Py：命令行参数解析
来源：http://jtc.yuxming.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://esr.xingfuxueyuan.xyz

[U17] Py：初始化日志
来源：http://jnn.9152youxi.cn

logging.basicConfig(level=logging.INFO)
来源：http://zdv.cheryme.top

[U18] Py：预编译正则
来源：http://pje.nwbrower.top

pat = re.compile(r"\d+")
来源：http://fzw.haohaochexian.top

[U19] Py：正则替换带回调
来源：http://kqd.ehwqpu.com

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://vgl.pengpengdd.cyou

[U20] Py：缓存函数结果
来源：http://ibm.guowangkeji.top

@functools.lru_cache(maxsize=None)
来源：http://yiy.cheryme.top

[U21] Py：自定义上下文管理器
来源：http://xuh.chenlongwang.top

@contextlib.contextmanager
来源：http://edz.cqqwz.cn

[U22] Py：矩阵转置
来源：http://oki.sufxvd.cn

list(zip(*m))
来源：http://vyp.svipenyu.cn

[U23] Py：分块读取大文件
来源：http://eqq.zhiwuduotai.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://uxt.nanxuanxn.top

[U24] Py：路径操作
来源：http://aln.xuetiantiany.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://tre.fanxiaobao.xyz

[U25] Py：CSV 按字典读
来源：http://nnx.hfpthk.cn

csv.DictReader(f)
来源：http://aoc.shanyushiyangkeji.top

[U26] Py：并发下载
来源：http://zyd.hcnkem.com

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://rqy.pycfn.com

[U27] Py：异步 HTTP
来源：http://rjs.vqdsnc.cn

aiohttp.ClientSession() 配合 async with
来源：http://jnu.chenlongwang.top

[U28] Py：类型别名
来源：http://avu.andypj.xyz

UserId = int
来源：http://kbd.cdnleiting.top

[U29] Py：属性校验
来源：http://hql.pengpengdd.cyou

@property 与 @x.setter 配合
来源：http://jnw.cdnleiting.top

[U30] Py：数据类
来源：http://bsx.birdmap.top

@dataclass(slots=True)
来源：http://ukx.jlsjyb.cn

[U31] Py：单测
来源：http://puh.daria6918.cn

python -m pytest -q
来源：http://xjw.andypj.xyz

[U32] Py：代码格式化
来源：http://kna.ehwqpu.com

ruff format . && ruff check --fix .
来源：http://itx.chenlongwang.top

[U33] Py：打包发布
来源：http://ntx.hcnkem.com

python -m build  （依赖 pyproject.toml）
来源：http://ipb.xylfe.cn

[U34] Py：判断编码
来源：http://zfa.kuanghao11.cn

chardet.detect(raw)
来源：http://bbi.nanxuanxn.top

[U35] Py：发送邮件
来源：http://zhx.sysykeji.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://kqx.cdnleiting.top

[U36] Py：定时任务
来源：http://vkp.fanxiaobao.xyz

schedule.every(10).minutes.do(job)
来源：http://dwj.cqqwz.cn

[U37] Py：读写 Excel
来源：http://ief.fehbvm.com

pandas.read_excel / DataFrame.to_excel
来源：http://kyf.gzhubu.top

[U38] Py：获取脚本所在目录
来源：http://xof.snrcjt.cn

Path(__file__).resolve().parent
来源：http://dqz.0kj1m.cn

[U39] Py：判断是否在交互环境
来源：http://boc.haohaochexian.top

sys.stdout.isatty()
来源：http://cqn.redwolf501.top

[U40] Py：打印到标准错误
来源：http://zqv.cucudq.cn

print("err", file=sys.stderr)
来源：http://dtu.gogol.net.cn

[U41] PHP：初始化 Composer 项目
来源：http://mwj.fanxiaobao.xyz

composer init;  composer require guzzlehttp/guzzle
来源：http://gyj.zhongyouzk.top

[U42] PHP：PSR-4 自动加载
来源：http://tci.ywan-chungtsiang.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://ymn.hammf.cn

[U43] PHP：声明命名空间
来源：http://eew.yongpay.top

namespace App\Http;
来源：http://cnb.quarkkingdee.top

[U44] PHP：开启严格类型
来源：http://izl.fktsv.cn

declare(strict_types=1);
来源：http://nnq.meibo888.top

[U45] PHP：类型声明与返回类型
来源：http://viz.xingfuxueyuan.xyz

function add(int $a, int $b): int { return $a + $b; }
来源：http://gah.cdnleiting.top

[U46] PHP：可空类型
来源：http://afo.chenlongwang.top

?string $name = null
来源：http://ecy.iojbl.cn

[U47] PHP：联合类型
来源：http://jwb.hysaishi.cn

int|string $id
来源：http://gld.redwolf501.top

[U48] PHP：纯枚举
来源：http://dve.shangyingyoupin.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://prs.yj202588.top

[U49] PHP：只读属性
来源：http://dka.zhoulong.xyz

public readonly string $name
来源：http://mgv.snrcjt.cn

[U50] PHP：构造器属性提升
来源：http://bbu.gaohongyu789.top

public function __construct(private int $id) {}
来源：http://hqx.zdqjudy.top

[U51] PHP：数组解构
来源：http://pur.hywenlv.cn

[$a, $b] = $arr;
来源：http://fpp.wangdashe.top

[U52] PHP：箭头函数
来源：http://rdc.zhijiandao.cn

$double = fn($x) => $x * 2;
来源：http://ouc.jqgfzy.top

[U53] PHP：空合并运算符
来源：http://xjh.pengpengdd.cyou

$v = $a ?? $b ?? "default";
来源：http://hqc.hongshengwenyu.top

[U54] PHP：空安全调用
来源：http://xjx.xingfuxueyuan.xyz

$obj?->method()
来源：http://pol.hongshengwenyu.top

[U55] PHP：match 表达式
来源：http://vbn.ydjk.org.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://jia.uphjek.com

[U56] PHP：命名参数
来源：http://kzv.yvedp.cn

f(a: 1, b: 2)
来源：http://icy.zdqjudy.top

[U57] PHP：字符串插值
来源：http://qem.bbcook.cn

"值: {$a}"
来源：http://qbd.bjfxy.top

[U58] PHP：数组三件套
来源：http://twa.xylfe.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://krp.zhongyouzk.top

[U59] PHP：自定义排序
来源：http://hnb.pengpengdd.cyou

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hdc.zhoulong.xyz

[U60] PHP：JSON 编解码
来源：http://tib.yangfankeji.com

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://pmn.uphjek.com

[U61] PHP：正则
来源：http://jgu.birdmap.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://ovn.hammf.cn

[U62] PHP：日期对象
来源：http://gkz.wangshuangyany.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://mpr.svipenyu.cn

[U63] PHP：文件读写
来源：http://nwo.hysaishi.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://cir.zhiwuduotai.top

[U64] PHP：目录遍历
来源：http://gji.ivvv.top

glob("dir/*.php");  scandir("dir");
来源：http://qbz.hnxiangtu.top

[U65] PHP：会话
来源：http://xge.iojbl.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://gzx.xinyue.icu

[U66] PHP：设置 Cookie
来源：http://vbm.shanyushiyangtech.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://axl.ydzc1.top

[U67] PHP：处理文件上传
来源：http://iws.chenlongwang.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://mih.daria6918.cn

[U68] PHP：PDO 连接
来源：http://odn.ydzc1.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://vtg.iojbl.cn

[U69] PHP：PDO 预处理
来源：http://skl.jianghu66.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://ptr.hnxiangtu.top

[U70] PHP：PDO 事务
来源：http://enh.hcnkem.com

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://ljs.zhaomingkeji.xyz

[U71] PHP：抛出异常
来源：http://qdx.sjlbkw.cn

throw new RuntimeException("失败", 500);
来源：http://cez.ydjk.org.cn

[U72] PHP：写错误日志
来源：http://svp.cqqwz.cn

error_log("失败: " . $e->getMessage());
来源：http://kju.snrcjt.cn

[U73] PHP：读取 ini 配置
来源：http://uha.fehbvm.com

parse_ini_file("config.ini", true)
来源：http://ezl.gzhubu.top

[U74] PHP：读取环境变量
来源：http://wkb.jyoumei.cn

getenv("APP_ENV") ?: "production"
来源：http://pgc.uphjek.com

[U75] PHP：依赖注入
来源：http://fph.andypj.xyz

composer require psr/container
来源：http://vvi.fehbvm.com

[U76] PHP：简单路由
来源：http://pvh.cdnleiting.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://uuj.dianchejie.cn

[U77] PHP：模板渲染
来源：http://vwx.hnqzz.top

composer require twig/twig
来源：http://srt.xinyue.icu

[U78] PHP：单元测试
来源：http://ypt.tian-w.cn

composer require --dev phpunit/phpunit
来源：http://col.meibo888.top

[U79] PHP：静态分析
来源：http://eqe.fanxiaobao.xyz

composer require --dev phpstan/phpstan
来源：http://jrh.vqdsnc.cn

[U80] PHP：代码规范修复
来源：http://plv.fktsv.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://dka.birdmap.top

[U81] JS：初始化项目
来源：http://rvk.guannengcc.top

npm init -y;  npm i express
来源：http://oua.gzhubu.top

[U82] JS：package.json 脚本
来源：http://mzi.jinqigfzy.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://oma.xinyue.icu

[U83] JS：ES Module 导入导出
来源：http://gwf.mhx1999.top

export const a = 1;  import { a } from "./m.js";
来源：http://csx.shanyushiyangtech.top

[U84] JS：CommonJS 写法
来源：http://smo.iojbl.cn

module.exports = { a };  const { a } = require("./m");
来源：http://zet.ehwqpu.com

[U85] JS：可选链
来源：http://muq.zhoulong.xyz

a?.b?.c
来源：http://zou.yj20258888.top

[U86] JS：空值合并
来源：http://tth.yfazqb.com

a ?? b
来源：http://kdq.cashguo.top

[U87] JS：解构默认值
来源：http://fbr.chenlongwang.top

const { a = 1, b = 2 } = obj;
来源：http://dts.ybcxt.top

[U88] JS：对象展开合并
来源：http://ijs.chenlongwang.top

{ ...a, ...b }
来源：http://zzy.aizwys.cn

[U89] JS：数组去重
来源：http://htl.hnxiangtu.top

[...new Set(arr)]
来源：http://rpj.gotoacloud.top

[U90] JS：数字数组排序
来源：http://sjp.yuanzhike.top

[...arr].sort((a, b) => a - b)
来源：http://jjz.fehbvm.com

[U91] JS：对象键值遍历
来源：http://oep.vehdjk.com

Object.entries(obj).forEach(([k, v]) => {});
来源：http://cuz.jinyuanbaomall.cn

[U92] JS：深拷贝
来源：http://pot.jinqigufen.top

structuredClone(obj)
来源：http://amw.ehwqpu.com

[U93] JS：模板字符串
来源：http://umb.wangshuangyany.cn

`共 ${n} 条`
来源：http://qgr.xinyue.icu

[U94] JS：箭头函数
来源：http://com.nwbrower.top

const double = x => x * 2;
来源：http://zcg.pycfn.com

[U95] JS：Promise 包装
来源：http://iua.hfpthk.cn

new Promise((resolve, reject) => {})
来源：http://flr.dianchejie.cn

[U96] JS：async/await 与异常
来源：http://gkb.tanke756.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://rss.ybcxt.top

[U97] JS：并发请求
来源：http://csy.shangyingyoupin.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://ftw.jiagoushi.top

[U98] JS：fetch 带 JSON
来源：http://wbg.fengsongda.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://tgj.redwolf501.top

[U99] JS：事件监听
来源：http://zcj.guowangkeji.top

el.addEventListener("click", e => {})
来源：http://jlm.svipenyu.cn

[U100] JS：DOM 查询
来源：http://dxy.haohaochexian.top

document.querySelector(".item")
来源：http://hdu.yvedp.cn

[U101] JS：classList 操作
来源：http://tmp.jinghuilouyu.cn

el.classList.toggle("active")
来源：http://skt.sysykeji.top

[U102] JS：本地存储
来源：http://qth.birdmap.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://nxx.yuxming.cn

[U103] JS：定时器
来源：http://jsh.wangshuangyany.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://ahh.haohaochexian.top

[U104] JS：防抖
来源：http://ofd.ywan-chungtsiang.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://xtd.chenzaomai.com

[U105] JS：节流
来源：http://hwm.zhixingplan.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://mzn.jinyuanbaomall.cn

[U106] JS：日期格式化
来源：http://qar.zhongyouzk.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://zfr.316326.xyz

[U107] JS：数字千分位
来源：http://ldp.svipenyu.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://wyn.iojbl.cn

[U108] JS：随机整数
来源：http://lul.zhiwuduotai.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://dbg.zhiwuduotai.top

[U109] JS：数组分组
来源：http://sxt.nanxinkj.top

Object.groupBy(arr, x => x.type)
来源：http://mui.jinghuilouyu.cn

[U110] JS：数组分块
来源：http://maw.cashguo.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://wld.yj202588.top

[U111] JS：对象转 Map
来源：http://xmi.havefunace.top

new Map(Object.entries(obj))
来源：http://xfg.zhengqikj.top

[U112] JS：字符串补位
来源：http://exe.yangfankeji.com

"7".padStart(3, "0")
来源：http://bbp.iojbl.cn


<!-- 参考信息 -->