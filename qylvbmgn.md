代发 wailian999

[T35] Lua：字典表
来源：http://ogw.pengpengdd.cyou

local d = { a = 1 };  d.b = 2
来源：http://jkg.tianlin.xyz

[T36] Lua：函数
来源：http://jbn.zhengqikj.top

function add(a, b) return a + b end
来源：http://fmn.xuetiantiany.cn

[T37] Lua：字符串拼接
来源：http://gwf.ehwqpu.com

"a" .. "b"
来源：http://sro.chenjidiqi.icu

[T38] Lua：条件
来源：http://nxs.ydzc1.top

if x > 0 then print("正") end
来源：http://zik.zhongyouzk.top

[T39] Lua：模式匹配
来源：http://tmq.fzhhl.top

string.find(s, "%d+")
来源：http://gvk.kuanghao11.cn

[T40] Lua：元表
来源：http://fjx.birdmap.top

setmetatable({}, { __index = base })
来源：http://ybt.yongpay.top

[T41] Perl：Hello World
来源：http://nqs.ivvv.top

print "Hello\n";
来源：http://uvy.guowangkeji.top

[T42] Perl：变量类型
来源：http://ojm.feifeiyinyue.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://gpx.nanxuanxn.top

[T43] Perl：字符串插值
来源：http://npm.jyoumei.cn

"值: $a"
来源：http://ccl.wangshuangyany.cn

[T44] Perl：条件
来源：http://wsg.redwolf501.top

if ($a > 0) { print "正"; }
来源：http://jvx.jyoumei.cn

[T45] Perl：数组遍历
来源：http://nvb.kuanghao11.cn

for my $x (@arr) { print $x; }
来源：http://gda.bbcook.cn

[T46] Perl：哈希操作
来源：http://gej.yj20258888.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://bsi.xylfe.cn

[T47] Perl：正则捕获
来源：http://yeh.redwolf501.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://dwq.hnxiangtu.top

[T48] Perl：正则替换
来源：http://voz.gotoacloud.top

$s =~ s/old/new/g;
来源：http://ebh.aibaodan.cn

[T49] Perl：函数
来源：http://nsh.shzxlz.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://nha.xziqi.cn

[T50] Perl：逐行读文件
来源：http://zqi.zdbjq.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://ifb.jiagoushi.top

while (my $line = <$fh>) { print $line; }
来源：http://cse.zhiwuduotai.top

[T51] Scala：Hello World
来源：http://stw.zhongyouzk.top

println("Hello")
来源：http://akr.shangyingyoupin.top

[T52] Scala：变量
来源：http://fgj.zhoulong.xyz

val a = 1;  var b = 2
来源：http://mmo.zhijiandao.cn

[T53] Scala：字符串插值
来源：http://fgl.ctjpmb.com

s"值: $b"
来源：http://nat.xingfuxueyuan.xyz

[T54] Scala：集合映射
来源：http://shw.haohaochexian.top

List(1, 2, 3).map(_ * 2)
来源：http://bqf.yj20258.top

[T55] Scala：集合过滤
来源：http://jak.nanxinkj.top

List(1, 2, 3).filter(_ > 1)
来源：http://eqd.cashguo.top

[T56] Scala：样例类
来源：http://lsk.jqgfzy.top

case class User(name: String, age: Int)
来源：http://blb.yanxiufei.cn

[T57] Scala：模式匹配
来源：http://lfm.yuxming.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://pay.zhixingplan.top

[T58] Scala：函数定义
来源：http://vin.yfazqb.com

def add(a: Int, b: Int): Int = a + b
来源：http://nbf.bbcook.cn

[T59] Scala：循环
来源：http://iqi.fengsongda.top

for (i <- 1 to 10) println(i)
来源：http://jfk.xinyue.icu

[T60] Scala：折叠
来源：http://bem.fanxiaobao.xyz

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://ffm.tianlin.xyz

================================================================================
来源：http://tte.yj20258888.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://tsh.mhx1999.top

================================================================================
来源：http://eiu.yj202588.top

[U01] Py：创建虚拟环境
来源：http://lcv.ywan-chungtsiang.top

python -m venv .venv && source .venv/bin/activate
来源：http://ika.tian-w.cn

[U02] Py：导出 / 安装依赖
来源：http://fzj.pycfn.com

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://fcy.uphjek.com

[U03] Py：加载 .env 配置
来源：http://wqe.pengpengdd.cyou

from dotenv import load_dotenv; load_dotenv()
来源：http://dss.hnxiangtu.top

[U04] Py：变量调试打印
来源：http://dbe.sysykeji.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://pxv.yj202588.top

[U05] Py：列表去重且保序
来源：http://esz.zhengqikj.top

list(dict.fromkeys(arr))
来源：http://ztc.yueranfly.top

[U06] Py：合并两个字典
来源：http://kop.zycfv.cn

{**a, **b}
来源：http://kdx.fehbvm.com

[U07] Py：反转字典键值
来源：http://lfz.bjfxy.top

{v: k for k, v in d.items()}
来源：http://twc.gotoacloud.top

[U08] Py：展平二维列表
来源：http://tbu.zycfv.cn

[y for x in nested for y in x]
来源：http://wxf.quarkkingdee.top

[U09] Py：字典取最大值的键
来源：http://gqz.nanxinkj.top

max(d, key=d.get)
来源：http://hva.mhx1999.top

[U10] Py：按值排序字典
来源：http://jhp.yj202588.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://dqf.zhengqikj.top

[U11] Py：生成器表达式
来源：http://uup.yangfankeji.com

(x * 2 for x in arr)
来源：http://hwz.bbcook.cn

[U12] Py：取出现最多的 3 个元素
来源：http://oex.gogol.net.cn

Counter(arr).most_common(3)
来源：http://wmn.daxiang520.top

[U13] Py：固定长度队列
来源：http://bcb.yuxming.cn

deque(maxlen=10)
来源：http://myu.xuetiantiany.cn

[U14] Py：分组收集到列表
来源：http://bzw.sxryk.cn

defaultdict(list)
来源：http://sac.wangshuangyany.cn

[U15] Py：高精度计时
来源：http://vvh.hammf.cn

t = time.perf_counter()
来源：http://lqp.gzhubu.top

[U16] Py：命令行参数解析
来源：http://ent.cucudq.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://mlu.quarkkingdee.top

[U17] Py：初始化日志
来源：http://iqg.vqdsnc.cn

logging.basicConfig(level=logging.INFO)
来源：http://ulo.nanxuanxn.top

[U18] Py：预编译正则
来源：http://rhn.yongpay.top

pat = re.compile(r"\d+")
来源：http://epx.bjfxy.top

[U19] Py：正则替换带回调
来源：http://iwz.zycfv.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://bts.shanyushiyangkeji.top

[U20] Py：缓存函数结果
来源：http://gyj.yuanzhike.top

@functools.lru_cache(maxsize=None)
来源：http://xpf.gzhubu.top

[U21] Py：自定义上下文管理器
来源：http://kze.jianghu66.top

@contextlib.contextmanager
来源：http://qng.chenjidiqi.icu

[U22] Py：矩阵转置
来源：http://rzr.xuanzx.com

list(zip(*m))
来源：http://rhq.aizwys.cn

[U23] Py：分块读取大文件
来源：http://xel.shzxlz.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://jzh.hnxiangtu.top

[U24] Py：路径操作
来源：http://ovs.zdbjq.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://xhn.shuidangran.top

[U25] Py：CSV 按字典读
来源：http://jtq.jqgfzy.top

csv.DictReader(f)
来源：http://jul.yangfankeji.com

[U26] Py：并发下载
来源：http://qjd.zhoulong.xyz

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://dmb.yongpay.top

[U27] Py：异步 HTTP
来源：http://xxh.hammf.cn

aiohttp.ClientSession() 配合 async with
来源：http://fkp.ydzc1.top

[U28] Py：类型别名
来源：http://dlj.birdmap.top

UserId = int
来源：http://zab.jinyuanbaomall.cn

[U29] Py：属性校验
来源：http://wdm.bbcook.cn

@property 与 @x.setter 配合
来源：http://wpk.xylfe.cn

[U30] Py：数据类
来源：http://zee.cheryme.top

@dataclass(slots=True)
来源：http://bca.havefunace.top

[U31] Py：单测
来源：http://wvb.daria6918.cn

python -m pytest -q
来源：http://sbm.feifeiyinyue.top

[U32] Py：代码格式化
来源：http://nuz.daxiang520.top

ruff format . && ruff check --fix .
来源：http://dsb.gogol.net.cn

[U33] Py：打包发布
来源：http://tyf.hesvh.cn

python -m build  （依赖 pyproject.toml）
来源：http://erp.jinqigfzy.top

[U34] Py：判断编码
来源：http://pbm.tian-w.cn

chardet.detect(raw)
来源：http://pxw.epnwcf.com

[U35] Py：发送邮件
来源：http://vuu.aizwys.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://kso.cheryme.top

[U36] Py：定时任务
来源：http://tro.shuidangran.top

schedule.every(10).minutes.do(job)
来源：http://ygd.kuanghao11.cn

[U37] Py：读写 Excel
来源：http://wkt.feifeiyinyue.top

pandas.read_excel / DataFrame.to_excel
来源：http://fpq.birdmap.top

[U38] Py：获取脚本所在目录
来源：http://ebj.jqgufenzy.top

Path(__file__).resolve().parent
来源：http://zau.tian-w.cn

[U39] Py：判断是否在交互环境
来源：http://trm.zdqjudy.top

sys.stdout.isatty()
来源：http://yej.zhijiandao.cn

[U40] Py：打印到标准错误
来源：http://tkv.ydjk.org.cn

print("err", file=sys.stderr)
来源：http://zbl.ppjwa.cn

[U41] PHP：初始化 Composer 项目
来源：http://iow.sjlbkw.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://vhj.jinghuilouyu.cn

[U42] PHP：PSR-4 自动加载
来源：http://ceb.epnwcf.com

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://bhh.svipenyu.cn

[U43] PHP：声明命名空间
来源：http://jzs.yj202588.top

namespace App\Http;
来源：http://emk.xingfuxueyuan.xyz

[U44] PHP：开启严格类型
来源：http://qvl.chenzaomai.com

declare(strict_types=1);
来源：http://yjm.gaohongyu789.top

[U45] PHP：类型声明与返回类型
来源：http://npq.dashuyun.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://afq.epnwcf.com

[U46] PHP：可空类型
来源：http://oau.zycfv.cn

?string $name = null
来源：http://gto.xinyue.icu

[U47] PHP：联合类型
来源：http://gvf.xylfe.cn

int|string $id
来源：http://fiy.zdbjq.cn

[U48] PHP：纯枚举
来源：http://eym.snrcjt.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://itj.dianchejie.cn

[U49] PHP：只读属性
来源：http://iaj.316326.xyz

public readonly string $name
来源：http://ebj.andypj.xyz

[U50] PHP：构造器属性提升
来源：http://jju.daxiang520.top

public function __construct(private int $id) {}
来源：http://jav.sufxvd.cn

[U51] PHP：数组解构
来源：http://lbe.xuanzx.com

[$a, $b] = $arr;
来源：http://zum.dashuyun.cn

[U52] PHP：箭头函数
来源：http://ido.cashguo.top

$double = fn($x) => $x * 2;
来源：http://gvx.zhengqikj.top

[U53] PHP：空合并运算符
来源：http://pmj.shangyingyoupin.top

$v = $a ?? $b ?? "default";
来源：http://ozj.xuanzx.com

[U54] PHP：空安全调用
来源：http://vaw.jinyuanbaomall.cn

$obj?->method()
来源：http://jrr.shuidangran.top

[U55] PHP：match 表达式
来源：http://dax.316326.xyz

$s = match($x) { 1 => "一", default => "其他" };
来源：http://xsq.xinyue.icu

[U56] PHP：命名参数
来源：http://sxj.nanxinkj.top

f(a: 1, b: 2)
来源：http://cdn.ydzc1.top

[U57] PHP：字符串插值
来源：http://rxm.wangshuangyany.cn

"值: {$a}"
来源：http://arl.gzhubu.top

[U58] PHP：数组三件套
来源：http://qdq.zhongyouzk.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://pme.vqdsnc.cn

[U59] PHP：自定义排序
来源：http://tqx.fengsongda.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://iem.zycfv.cn

[U60] PHP：JSON 编解码
来源：http://myl.jiagoushi.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://ymi.sysykeji.top

[U61] PHP：正则
来源：http://ffl.shanyushiyangkeji.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://fil.hywenlv.cn

[U62] PHP：日期对象
来源：http://dfl.ydjk.org.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://ncy.gotoacloud.top

[U63] PHP：文件读写
来源：http://szi.tarul.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://dvf.iojbl.cn

[U64] PHP：目录遍历
来源：http://xmf.birdmap.top

glob("dir/*.php");  scandir("dir");
来源：http://gou.vehdjk.com

[U65] PHP：会话
来源：http://tlz.xylfe.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://bbo.ctjpmb.com

[U66] PHP：设置 Cookie
来源：http://eib.meibo888.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://aua.epnwcf.com

[U67] PHP：处理文件上传
来源：http://tbu.redwolf501.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://bpb.dianchejie.cn

[U68] PHP：PDO 连接
来源：http://rxf.mhx1999.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://gnj.hnqzz.top

[U69] PHP：PDO 预处理
来源：http://hnp.meibo888.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hgc.ybcxt.top

[U70] PHP：PDO 事务
来源：http://zsb.fanxiaobao.xyz

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://wlj.0kj1m.cn

[U71] PHP：抛出异常
来源：http://mtg.sxryk.cn

throw new RuntimeException("失败", 500);
来源：http://gkj.fktsv.cn

[U72] PHP：写错误日志
来源：http://cli.yfazqb.com

error_log("失败: " . $e->getMessage());
来源：http://zvy.fzhhl.top

[U73] PHP：读取 ini 配置
来源：http://ipn.fktsv.cn

parse_ini_file("config.ini", true)
来源：http://fvn.jqgufenzy.top

[U74] PHP：读取环境变量
来源：http://yil.ydjk.org.cn

getenv("APP_ENV") ?: "production"
来源：http://lai.mhx1999.top

[U75] PHP：依赖注入
来源：http://ahu.vehdjk.com

composer require psr/container
来源：http://rvi.ivvv.top

[U76] PHP：简单路由
来源：http://hof.yanxiufei.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://hzl.yangfankeji.com

[U77] PHP：模板渲染
来源：http://yoh.epnwcf.com

composer require twig/twig
来源：http://pyj.yuxming.cn

[U78] PHP：单元测试
来源：http://koe.jiagoushi.top

composer require --dev phpunit/phpunit
来源：http://khy.nanxinkj.top

[U79] PHP：静态分析
来源：http://ehd.cucudq.cn

composer require --dev phpstan/phpstan
来源：http://cfa.zhijiandao.cn

[U80] PHP：代码规范修复
来源：http://bub.haohaochexian.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://oqs.shzxlz.cn

[U81] JS：初始化项目
来源：http://ldu.zhiwuduotai.top

npm init -y;  npm i express
来源：http://xog.yfazqb.com

[U82] JS：package.json 脚本
来源：http://ysx.fzhhl.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://oyp.vehdjk.com

[U83] JS：ES Module 导入导出
来源：http://bng.hysaishi.cn

export const a = 1;  import { a } from "./m.js";
来源：http://ljd.yuanzhike.top

[U84] JS：CommonJS 写法
来源：http://yeu.vehdjk.com

module.exports = { a };  const { a } = require("./m");
来源：http://wsr.ydzc1.top

[U85] JS：可选链
来源：http://eee.zdqjudy.top

a?.b?.c
来源：http://twc.jinqigfzy.top

[U86] JS：空值合并
来源：http://cye.andypj.xyz

a ?? b
来源：http://ydo.xylfe.cn

[U87] JS：解构默认值
来源：http://xlj.fktsv.cn

const { a = 1, b = 2 } = obj;
来源：http://lsz.hongshengwenyu.top

[U88] JS：对象展开合并
来源：http://spv.vehdjk.com

{ ...a, ...b }
来源：http://qdz.sufxvd.cn

[U89] JS：数组去重
来源：http://pod.bbcook.cn

[...new Set(arr)]
来源：http://mrk.chenlongwang.top

[U90] JS：数字数组排序
来源：http://alc.shzxlz.cn

[...arr].sort((a, b) => a - b)
来源：http://xfm.xuetiantiany.cn

[U91] JS：对象键值遍历
来源：http://fkz.zdbjq.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://lpy.316326.xyz

[U92] JS：深拷贝
来源：http://hjv.gogol.net.cn

structuredClone(obj)
来源：http://qqk.zdbjq.cn

[U93] JS：模板字符串
来源：http://ezk.hnxiangtu.top

`共 ${n} 条`
来源：http://fyj.tian-w.cn

[U94] JS：箭头函数
来源：http://lcx.52xcode.cn

const double = x => x * 2;
来源：http://rhw.jianghu66.top

[U95] JS：Promise 包装
来源：http://bug.hongshengwenyu.top

new Promise((resolve, reject) => {})
来源：http://rwq.nwbrower.top

[U96] JS：async/await 与异常
来源：http://yxa.chenjidiqi.icu

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://zym.daxiang520.top

[U97] JS：并发请求
来源：http://bmn.nanxuanxn.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://soj.zdqjudy.top

[U98] JS：fetch 带 JSON
来源：http://ylc.sufxvd.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://nrv.tanke756.top

[U99] JS：事件监听
来源：http://gwl.xziqi.cn

el.addEventListener("click", e => {})
来源：http://pre.chenjidiqi.icu

[U100] JS：DOM 查询
来源：http://zss.ehwqpu.com

document.querySelector(".item")
来源：http://vth.pycfn.com

[U101] JS：classList 操作
来源：http://ybr.gzhubu.top

el.classList.toggle("active")
来源：http://qei.pycfn.com

[U102] JS：本地存储
来源：http://jqi.316326.xyz

localStorage.setItem("k", JSON.stringify(v))
来源：http://xkt.jqgufenzy.top

[U103] JS：定时器
来源：http://xeh.snrcjt.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://djy.pengpengdd.cyou

[U104] JS：防抖
来源：http://xfn.yj20258.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://nru.smart0.xyz

[U105] JS：节流
来源：http://ufa.chenlongwang.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://bth.yvedp.cn

[U106] JS：日期格式化
来源：http://nzf.yanxiufei.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://dud.jqgfzy.top

[U107] JS：数字千分位
来源：http://sdc.zdqjudy.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://uth.hnxiangtu.top

[U108] JS：随机整数
来源：http://dhf.birdmap.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://pyz.jqgufenzy.top

[U109] JS：数组分组
来源：http://rux.sweek.top

Object.groupBy(arr, x => x.type)
来源：http://lae.hcnkem.com

[U110] JS：数组分块
来源：http://fgk.fehbvm.com

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://icz.ehwqpu.com

[U111] JS：对象转 Map
来源：http://zoz.xingfuxueyuan.xyz

new Map(Object.entries(obj))
来源：http://vrl.yuxming.cn

[U112] JS：字符串补位
来源：http://yej.mhx1999.top

"7".padStart(3, "0")
来源：http://dvf.tarul.cn

[U113] JS：正则替换全部
来源：http://occ.kuanghao11.cn

s.replaceAll("a", "b")
来源：http://qzl.hcnkem.com

[U114] JS：JSON 深比较
来源：http://ilu.9152youxi.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://tgv.sufxvd.cn

[U115] JS：生成 UUID
来源：http://yzm.cheryme.top

crypto.randomUUID()
来源：http://fcd.c1oappe.top

[U116] JS：类型检查（JSDoc）
来源：http://vtt.yonumen.top

/** @param {string} name */ function f(name) {}
来源：http://toh.jinyuanbaomall.cn

[U117] JS：单元测试
来源：http://yeh.sufxvd.cn

npm i -D vitest;  npx vitest
来源：http://fku.xingfuxueyuan.xyz

[U118] JS：开发服务器
来源：http://jqm.zdqjudy.top

npm i -D vite;  npx vite
来源：http://ssi.hammf.cn

[U119] JS：生产构建
来源：http://akp.fanxiaobao.xyz

npx vite build
来源：http://cow.52xcode.cn

[U120] JS：读取环境变量（Vite）
来源：http://zho.yj20258.top

import.meta.env.VITE_API_URL
来源：http://ljd.vqdsnc.cn

================================================================================
来源：http://gtr.jinghuilouyu.cn

统计汇总
来源：http://wno.yvedp.cn

================================================================================
来源：http://upi.bjfxy.top

按语言统计（条）：
来源：http://fha.shzxlz.cn


<!-- 参考信息 -->