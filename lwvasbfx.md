代发 wailian999

[T43] Perl：字符串插值
来源：http://oai.hongshengwenyu.top

"值: $a"
来源：http://lce.zhijiandao.cn

[T44] Perl：条件
来源：http://hmj.yj20258.top

if ($a > 0) { print "正"; }
来源：http://otu.nanxuanxn.top

[T45] Perl：数组遍历
来源：http://arz.jianghu66.top

for my $x (@arr) { print $x; }
来源：http://kvk.yj20258888.top

[T46] Perl：哈希操作
来源：http://txx.xziqi.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://jnn.dianchejie.cn

[T47] Perl：正则捕获
来源：http://cbx.jianghu66.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://fne.sxryk.cn

[T48] Perl：正则替换
来源：http://hul.gogol.net.cn

$s =~ s/old/new/g;
来源：http://tpy.ybcxt.top

[T49] Perl：函数
来源：http://jhz.0kj1m.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://sin.yvedp.cn

[T50] Perl：逐行读文件
来源：http://neq.shzxlz.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://hys.shuidangran.top

while (my $line = <$fh>) { print $line; }
来源：http://ivv.quarkkingdee.top

[T51] Scala：Hello World
来源：http://vij.sysykeji.top

println("Hello")
来源：http://gno.sjlbkw.cn

[T52] Scala：变量
来源：http://ojz.yfazqb.com

val a = 1;  var b = 2
来源：http://iil.aizwys.cn

[T53] Scala：字符串插值
来源：http://nop.jlsjyb.cn

s"值: $b"
来源：http://fpb.yangfankeji.com

[T54] Scala：集合映射
来源：http://rgh.vqdsnc.cn

List(1, 2, 3).map(_ * 2)
来源：http://qku.hnqzz.top

[T55] Scala：集合过滤
来源：http://iuk.jinghuilouyu.cn

List(1, 2, 3).filter(_ > 1)
来源：http://pii.tianlin.xyz

[T56] Scala：样例类
来源：http://uew.jyoumei.cn

case class User(name: String, age: Int)
来源：http://lnx.fehbvm.com

[T57] Scala：模式匹配
来源：http://mro.meibo888.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://rfb.guowangkeji.top

[T58] Scala：函数定义
来源：http://gkl.zdqjudy.top

def add(a: Int, b: Int): Int = a + b
来源：http://asd.havefunace.top

[T59] Scala：循环
来源：http://cpa.sxryk.cn

for (i <- 1 to 10) println(i)
来源：http://sie.quarkkingdee.top

[T60] Scala：折叠
来源：http://hcx.yangfankeji.com

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://ukn.tarul.cn

================================================================================
来源：http://roe.shuidangran.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://oso.sysykeji.top

================================================================================
来源：http://tcs.yongpay.top

[U01] Py：创建虚拟环境
来源：http://fgt.ppjwa.cn

python -m venv .venv && source .venv/bin/activate
来源：http://mxh.vqdsnc.cn

[U02] Py：导出 / 安装依赖
来源：http://jjs.ehwqpu.com

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://bey.quarkkingdee.top

[U03] Py：加载 .env 配置
来源：http://uyz.guowangkeji.top

from dotenv import load_dotenv; load_dotenv()
来源：http://nre.shzxlz.cn

[U04] Py：变量调试打印
来源：http://gje.xylfe.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://atd.jlsjyb.cn

[U05] Py：列表去重且保序
来源：http://ofj.daria6918.cn

list(dict.fromkeys(arr))
来源：http://wdb.ywan-chungtsiang.top

[U06] Py：合并两个字典
来源：http://yzi.hongshengwenyu.top

{**a, **b}
来源：http://xys.yj20258.top

[U07] Py：反转字典键值
来源：http://gnc.redwolf501.top

{v: k for k, v in d.items()}
来源：http://ebl.gogol.net.cn

[U08] Py：展平二维列表
来源：http://vvu.zhoulong.xyz

[y for x in nested for y in x]
来源：http://ocm.hcnkem.com

[U09] Py：字典取最大值的键
来源：http://ckw.gzhubu.top

max(d, key=d.get)
来源：http://nba.c1oappe.top

[U10] Py：按值排序字典
来源：http://dly.cdnleiting.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://eve.quarkkingdee.top

[U11] Py：生成器表达式
来源：http://cmw.cheryme.top

(x * 2 for x in arr)
来源：http://tcr.ydjk.org.cn

[U12] Py：取出现最多的 3 个元素
来源：http://itm.ctjpmb.com

Counter(arr).most_common(3)
来源：http://mur.9152youxi.cn

[U13] Py：固定长度队列
来源：http://vey.yanxiufei.cn

deque(maxlen=10)
来源：http://azr.shanyushiyangkeji.top

[U14] Py：分组收集到列表
来源：http://krj.fzhhl.top

defaultdict(list)
来源：http://btx.jyoumei.cn

[U15] Py：高精度计时
来源：http://wfs.cheryme.top

t = time.perf_counter()
来源：http://dmv.zhijiandao.cn

[U16] Py：命令行参数解析
来源：http://bhs.hfpthk.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://kvm.zycfv.cn

[U17] Py：初始化日志
来源：http://vbl.quarkkingdee.top

logging.basicConfig(level=logging.INFO)
来源：http://uas.yanxiufei.cn

[U18] Py：预编译正则
来源：http://rgp.jyoumei.cn

pat = re.compile(r"\d+")
来源：http://mbq.vehdjk.com

[U19] Py：正则替换带回调
来源：http://iia.sufxvd.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://ygr.chenzaomai.com

[U20] Py：缓存函数结果
来源：http://qnv.shangyingyoupin.top

@functools.lru_cache(maxsize=None)
来源：http://dbg.shuidangran.top

[U21] Py：自定义上下文管理器
来源：http://mpt.yj20258888.top

@contextlib.contextmanager
来源：http://eir.hnxiangtu.top

[U22] Py：矩阵转置
来源：http://xil.hesvh.cn

list(zip(*m))
来源：http://exv.jqgfzy.top

[U23] Py：分块读取大文件
来源：http://kck.tian-w.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://vdj.nanxinkj.top

[U24] Py：路径操作
来源：http://wyt.meibo888.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://nmk.wangshuangyany.cn

[U25] Py：CSV 按字典读
来源：http://lyg.daxiang520.top

csv.DictReader(f)
来源：http://pqr.nwbrower.top

[U26] Py：并发下载
来源：http://gky.aizwys.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://jfu.jlsjyb.cn

[U27] Py：异步 HTTP
来源：http://jdj.zhijiandao.cn

aiohttp.ClientSession() 配合 async with
来源：http://lmt.nanxinkj.top

[U28] Py：类型别名
来源：http://vyd.hnxiangtu.top

UserId = int
来源：http://sjy.feifeiyinyue.top

[U29] Py：属性校验
来源：http://tdg.yj202588.top

@property 与 @x.setter 配合
来源：http://vcv.wangshuangyany.cn

[U30] Py：数据类
来源：http://efo.hongshengwenyu.top

@dataclass(slots=True)
来源：http://kze.meibo888.top

[U31] Py：单测
来源：http://hjz.ppjwa.cn

python -m pytest -q
来源：http://jio.52xcode.cn

[U32] Py：代码格式化
来源：http://nnu.fengsongda.top

ruff format . && ruff check --fix .
来源：http://npk.xuanzx.com

[U33] Py：打包发布
来源：http://zyy.ctjpmb.com

python -m build  （依赖 pyproject.toml）
来源：http://zzp.zhijiandao.cn

[U34] Py：判断编码
来源：http://avb.dashuyun.cn

chardet.detect(raw)
来源：http://gks.yj20258.top

[U35] Py：发送邮件
来源：http://lwz.zhiwuduotai.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://rdy.ppjwa.cn

[U36] Py：定时任务
来源：http://qaq.kuanghao11.cn

schedule.every(10).minutes.do(job)
来源：http://pnt.yangfankeji.com

[U37] Py：读写 Excel
来源：http://oge.xziqi.cn

pandas.read_excel / DataFrame.to_excel
来源：http://jvz.xziqi.cn

[U38] Py：获取脚本所在目录
来源：http://nvo.jinqigfzy.top

Path(__file__).resolve().parent
来源：http://drj.jianghu66.top

[U39] Py：判断是否在交互环境
来源：http://fkt.xinyue.icu

sys.stdout.isatty()
来源：http://iyx.zdqjudy.top

[U40] Py：打印到标准错误
来源：http://yyq.ywan-chungtsiang.top

print("err", file=sys.stderr)
来源：http://xmp.feifeiyinyue.top

[U41] PHP：初始化 Composer 项目
来源：http://vrm.tian-w.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://olf.zhongyouzk.top

[U42] PHP：PSR-4 自动加载
来源：http://edi.dashuyun.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://the.chenlongwang.top

[U43] PHP：声明命名空间
来源：http://zdo.ybcxt.top

namespace App\Http;
来源：http://ses.ctjpmb.com

[U44] PHP：开启严格类型
来源：http://ebw.shanyushiyangtech.top

declare(strict_types=1);
来源：http://wfh.sxryk.cn

[U45] PHP：类型声明与返回类型
来源：http://avt.ivvv.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://owv.sufxvd.cn

[U46] PHP：可空类型
来源：http://hnn.nanxuanxn.top

?string $name = null
来源：http://mqk.pycfn.com

[U47] PHP：联合类型
来源：http://dsx.jinqigfzy.top

int|string $id
来源：http://tif.jlsjyb.cn

[U48] PHP：纯枚举
来源：http://fnq.aizwys.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://vcx.fehbvm.com

[U49] PHP：只读属性
来源：http://rws.hesvh.cn

public readonly string $name
来源：http://pqm.zhiwuduotai.top

[U50] PHP：构造器属性提升
来源：http://hkc.hammf.cn

public function __construct(private int $id) {}
来源：http://eqf.fktsv.cn

[U51] PHP：数组解构
来源：http://svb.mhx1999.top

[$a, $b] = $arr;
来源：http://iva.pycfn.com

[U52] PHP：箭头函数
来源：http://rvw.guannengcc.top

$double = fn($x) => $x * 2;
来源：http://ska.zhixingplan.top

[U53] PHP：空合并运算符
来源：http://tls.yongpay.top

$v = $a ?? $b ?? "default";
来源：http://pwp.zdbjq.cn

[U54] PHP：空安全调用
来源：http://cey.wangshuangyany.cn

$obj?->method()
来源：http://lju.birdmap.top

[U55] PHP：match 表达式
来源：http://ioi.quarkkingdee.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://vuk.zhengqikj.top

[U56] PHP：命名参数
来源：http://zdz.yj20258.top

f(a: 1, b: 2)
来源：http://fbj.yj20258888.top

[U57] PHP：字符串插值
来源：http://fmq.guannengcc.top

"值: {$a}"
来源：http://gxm.zhoulong.xyz

[U58] PHP：数组三件套
来源：http://ngc.cdnleiting.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://clq.zhiwuduotai.top

[U59] PHP：自定义排序
来源：http://psq.jinghuilouyu.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wii.havefunace.top

[U60] PHP：JSON 编解码
来源：http://bef.ctjpmb.com

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://lta.shzxlz.cn

[U61] PHP：正则
来源：http://hgu.yongpay.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://emn.xziqi.cn

[U62] PHP：日期对象
来源：http://btc.jyoumei.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://bdm.sweek.top

[U63] PHP：文件读写
来源：http://cal.xuanzx.com

file_get_contents($f);  file_put_contents($f, $data);
来源：http://zie.nwbrower.top

[U64] PHP：目录遍历
来源：http://bbz.jinyuanbaomall.cn

glob("dir/*.php");  scandir("dir");
来源：http://ody.zhiwuduotai.top

[U65] PHP：会话
来源：http://hkj.shangyingyoupin.top

session_start();  $_SESSION["uid"] = 1;
来源：http://xvr.cheryme.top

[U66] PHP：设置 Cookie
来源：http://zbw.fengsongda.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://dep.fanxiaobao.xyz

[U67] PHP：处理文件上传
来源：http://bpj.fzhhl.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://oju.shzxlz.cn

[U68] PHP：PDO 连接
来源：http://skb.uphjek.com

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://pbm.tarul.cn

[U69] PHP：PDO 预处理
来源：http://ngo.hongshengwenyu.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://dbe.bbcook.cn

[U70] PHP：PDO 事务
来源：http://lhs.gaohongyu789.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://auu.quarkkingdee.top

[U71] PHP：抛出异常
来源：http://sgt.0kj1m.cn

throw new RuntimeException("失败", 500);
来源：http://tzb.hnxiangtu.top

[U72] PHP：写错误日志
来源：http://ect.yfazqb.com

error_log("失败: " . $e->getMessage());
来源：http://mhs.shangyingyoupin.top

[U73] PHP：读取 ini 配置
来源：http://wce.hnqzz.top

parse_ini_file("config.ini", true)
来源：http://blg.xinyue.icu

[U74] PHP：读取环境变量
来源：http://vya.mhx1999.top

getenv("APP_ENV") ?: "production"
来源：http://ofj.zhijiandao.cn

[U75] PHP：依赖注入
来源：http://fcz.fanxiaobao.xyz

composer require psr/container
来源：http://afi.yuanzhike.top

[U76] PHP：简单路由
来源：http://xjt.yj20258.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://fao.quarkkingdee.top

[U77] PHP：模板渲染
来源：http://ifd.sweek.top

composer require twig/twig
来源：http://smx.yuanzhike.top

[U78] PHP：单元测试
来源：http://kbw.yfazqb.com

composer require --dev phpunit/phpunit
来源：http://wcx.cashguo.top

[U79] PHP：静态分析
来源：http://uoa.hcnkem.com

composer require --dev phpstan/phpstan
来源：http://obp.cucudq.cn

[U80] PHP：代码规范修复
来源：http://cgv.yvedp.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://oco.xuanzx.com

[U81] JS：初始化项目
来源：http://vmw.yj20258888.top

npm init -y;  npm i express
来源：http://gtz.tianlin.xyz

[U82] JS：package.json 脚本
来源：http://hdv.hammf.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://npj.shanyushiyangtech.top

[U83] JS：ES Module 导入导出
来源：http://zoz.ybcxt.top

export const a = 1;  import { a } from "./m.js";
来源：http://zpq.gogol.net.cn

[U84] JS：CommonJS 写法
来源：http://dxn.zhiwuduotai.top

module.exports = { a };  const { a } = require("./m");
来源：http://nuz.yanxiufei.cn

[U85] JS：可选链
来源：http://rvc.haohaochexian.top

a?.b?.c
来源：http://cqv.yfazqb.com

[U86] JS：空值合并
来源：http://jus.andypj.xyz

a ?? b
来源：http://sji.ppjwa.cn

[U87] JS：解构默认值
来源：http://tim.jinghuilouyu.cn

const { a = 1, b = 2 } = obj;
来源：http://iua.zhoulong.xyz

[U88] JS：对象展开合并
来源：http://kre.hysaishi.cn

{ ...a, ...b }
来源：http://hcf.zhaomingkeji.xyz

[U89] JS：数组去重
来源：http://pgh.iojbl.cn

[...new Set(arr)]
来源：http://rnt.gzhubu.top

[U90] JS：数字数组排序
来源：http://shq.hammf.cn

[...arr].sort((a, b) => a - b)
来源：http://pbw.bbcook.cn

[U91] JS：对象键值遍历
来源：http://mxn.ctjpmb.com

Object.entries(obj).forEach(([k, v]) => {});
来源：http://wzh.guowangkeji.top

[U92] JS：深拷贝
来源：http://ubm.yuxming.cn

structuredClone(obj)
来源：http://gpl.xingfuxueyuan.xyz

[U93] JS：模板字符串
来源：http://qsg.xylfe.cn

`共 ${n} 条`
来源：http://xuv.fengsongda.top

[U94] JS：箭头函数
来源：http://nic.sysykeji.top

const double = x => x * 2;
来源：http://hqr.xziqi.cn

[U95] JS：Promise 包装
来源：http://bfj.fzhhl.top

new Promise((resolve, reject) => {})
来源：http://wol.ybcxt.top

[U96] JS：async/await 与异常
来源：http://wdu.fehbvm.com

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://izy.xinyue.icu

[U97] JS：并发请求
来源：http://spi.hcnkem.com

await Promise.all(urls.map(u => fetch(u)))
来源：http://eyp.cdnleiting.top

[U98] JS：fetch 带 JSON
来源：http://bwf.yuxming.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://lyi.316326.xyz

[U99] JS：事件监听
来源：http://muj.yanxiufei.cn

el.addEventListener("click", e => {})
来源：http://zjs.hywenlv.cn

[U100] JS：DOM 查询
来源：http://ohc.xuetiantiany.cn

document.querySelector(".item")
来源：http://tcp.hongshengwenyu.top

[U101] JS：classList 操作
来源：http://eab.tianlin.xyz

el.classList.toggle("active")
来源：http://ubr.zdbjq.cn

[U102] JS：本地存储
来源：http://jbz.gzhubu.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://sjq.guannengcc.top

[U103] JS：定时器
来源：http://qhw.sweek.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://fpb.tanke756.top

[U104] JS：防抖
来源：http://cel.xinyue.icu

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://bat.zdbjq.cn

[U105] JS：节流
来源：http://oyr.sjlbkw.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://lsv.yonumen.top

[U106] JS：日期格式化
来源：http://zxc.xinyue.icu

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://tzy.zhoulong.xyz

[U107] JS：数字千分位
来源：http://hkb.jinqigfzy.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://eaa.shangyingyoupin.top

[U108] JS：随机整数
来源：http://eoz.jyoumei.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://xzg.xylfe.cn

[U109] JS：数组分组
来源：http://ivk.mhx1999.top

Object.groupBy(arr, x => x.type)
来源：http://tze.gaohongyu789.top

[U110] JS：数组分块
来源：http://yaw.redwolf501.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://jzw.sjlbkw.cn

[U111] JS：对象转 Map
来源：http://vqb.wangshuangyany.cn

new Map(Object.entries(obj))
来源：http://tph.fengsongda.top

[U112] JS：字符串补位
来源：http://rkr.fktsv.cn

"7".padStart(3, "0")
来源：http://elb.chenjidiqi.icu

[U113] JS：正则替换全部
来源：http://wdk.316326.xyz

s.replaceAll("a", "b")
来源：http://dnw.zhijiandao.cn

[U114] JS：JSON 深比较
来源：http://vtq.gogol.net.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://mdd.52xcode.cn

[U115] JS：生成 UUID
来源：http://uqy.xziqi.cn

crypto.randomUUID()
来源：http://bsx.jianghu66.top

[U116] JS：类型检查（JSDoc）
来源：http://wgf.ydjk.org.cn

/** @param {string} name */ function f(name) {}
来源：http://srz.nanxinkj.top

[U117] JS：单元测试
来源：http://tgc.316326.xyz

npm i -D vitest;  npx vitest
来源：http://smp.chenjidiqi.icu

[U118] JS：开发服务器
来源：http://yud.nanxuanxn.top

npm i -D vite;  npx vite
来源：http://qdx.svipenyu.cn

[U119] JS：生产构建
来源：http://xzq.shanyushiyangtech.top

npx vite build
来源：http://plu.jiagoushi.top

[U120] JS：读取环境变量（Vite）
来源：http://grs.sjlbkw.cn

import.meta.env.VITE_API_URL
来源：http://skz.ctjpmb.com

================================================================================
来源：http://cva.aibaodan.cn

统计汇总
来源：http://ygk.sjlbkw.cn

================================================================================
来源：http://wcb.quarkkingdee.top

按语言统计（条）：
来源：http://yqm.kuanghao11.cn

Python ......... 252
来源：http://ret.aibaodan.cn

PHP ............ 252
来源：http://joh.jinqigufen.top

JavaScript ..... 252
来源：http://ztv.fehbvm.com

TypeScript ..... 212
来源：http://erc.cheryme.top

Java ........... 212
来源：http://dns.shzxlz.cn

Go ............. 212
来源：http://ezr.meibo888.top

Ruby ........... 212
来源：http://jtm.nwbrower.top

C# ............. 212
来源：http://bpl.xylfe.cn

C .............. 30
来源：http://lbh.fktsv.cn

C++ ............ 30
来源：http://bzu.shanyushiyangtech.top

SQL ............ 90
来源：http://weg.meibo888.top

Bash ........... 80
来源：http://pce.dashuyun.cn

Kotlin ......... 15
来源：http://ath.fzhhl.top

Swift .......... 15
来源：http://rjn.shzxlz.cn

Lua ............ 10
来源：http://jkx.zdbjq.cn

Perl ........... 10
来源：http://ciw.gaohongyu789.top


<!-- 参考信息 -->