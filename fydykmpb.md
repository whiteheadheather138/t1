代发 wailian999

[T43] Perl：字符串插值
来源：http://lgm.sxryk.cn

"值: $a"
来源：http://jfu.guannengcc.top

[T44] Perl：条件
来源：http://hhk.zhiwuduotai.top

if ($a > 0) { print "正"; }
来源：http://juw.fktsv.cn

[T45] Perl：数组遍历
来源：http://mfj.tian-w.cn

for my $x (@arr) { print $x; }
来源：http://eml.ydzc1.top

[T46] Perl：哈希操作
来源：http://deb.aizwys.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://gfy.wangshuangyany.cn

[T47] Perl：正则捕获
来源：http://erq.tianlin.xyz

if ($s =~ /(\d+)/) { print $1; }
来源：http://erg.sweek.top

[T48] Perl：正则替换
来源：http://dni.xylfe.cn

$s =~ s/old/new/g;
来源：http://fqr.daxiang520.top

[T49] Perl：函数
来源：http://jyi.zdqjudy.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://kzx.meibo888.top

[T50] Perl：逐行读文件
来源：http://wek.yueranfly.top

open my $fh, "<", "a.txt" or die $!;
来源：http://opp.gotoacloud.top

while (my $line = <$fh>) { print $line; }
来源：http://wpv.yangfankeji.com

[T51] Scala：Hello World
来源：http://uls.zdqjudy.top

println("Hello")
来源：http://puf.fktsv.cn

[T52] Scala：变量
来源：http://kxm.ctjpmb.com

val a = 1;  var b = 2
来源：http://kce.hnxiangtu.top

[T53] Scala：字符串插值
来源：http://xfw.zhengqikj.top

s"值: $b"
来源：http://ehf.gaohongyu789.top

[T54] Scala：集合映射
来源：http://uwj.zhongyouzk.top

List(1, 2, 3).map(_ * 2)
来源：http://ppm.dashuyun.cn

[T55] Scala：集合过滤
来源：http://boe.nanxuanxn.top

List(1, 2, 3).filter(_ > 1)
来源：http://ibf.9152youxi.cn

[T56] Scala：样例类
来源：http://qgn.sufxvd.cn

case class User(name: String, age: Int)
来源：http://rjo.316326.xyz

[T57] Scala：模式匹配
来源：http://znj.vehdjk.com

x match { case 1 => "一"; case _ => "其他" }
来源：http://zum.epnwcf.com

[T58] Scala：函数定义
来源：http://irv.nanxuanxn.top

def add(a: Int, b: Int): Int = a + b
来源：http://zvd.guowangkeji.top

[T59] Scala：循环
来源：http://cug.zycfv.cn

for (i <- 1 to 10) println(i)
来源：http://inj.yanxiufei.cn

[T60] Scala：折叠
来源：http://zie.ehwqpu.com

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hgq.ybcxt.top

================================================================================
来源：http://uda.shangyingyoupin.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://efv.yuanzhike.top

================================================================================
来源：http://pia.tarul.cn

[U01] Py：创建虚拟环境
来源：http://ywi.hammf.cn

python -m venv .venv && source .venv/bin/activate
来源：http://qsc.tianlin.xyz

[U02] Py：导出 / 安装依赖
来源：http://hjv.xylfe.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://lnn.sjlbkw.cn

[U03] Py：加载 .env 配置
来源：http://bhv.jinqigfzy.top

from dotenv import load_dotenv; load_dotenv()
来源：http://pvc.jinyuanbaomall.cn

[U04] Py：变量调试打印
来源：http://chw.fehbvm.com

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://znt.vqdsnc.cn

[U05] Py：列表去重且保序
来源：http://lic.havefunace.top

list(dict.fromkeys(arr))
来源：http://sye.svipenyu.cn

[U06] Py：合并两个字典
来源：http://tzq.cucudq.cn

{**a, **b}
来源：http://euy.sxryk.cn

[U07] Py：反转字典键值
来源：http://frt.cheryme.top

{v: k for k, v in d.items()}
来源：http://wyx.xziqi.cn

[U08] Py：展平二维列表
来源：http://ydo.yanxiufei.cn

[y for x in nested for y in x]
来源：http://rmq.chenzaomai.com

[U09] Py：字典取最大值的键
来源：http://xia.52xcode.cn

max(d, key=d.get)
来源：http://xrk.cashguo.top

[U10] Py：按值排序字典
来源：http://bep.zhongyouzk.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://oiu.316326.xyz

[U11] Py：生成器表达式
来源：http://jtq.zhijiandao.cn

(x * 2 for x in arr)
来源：http://fow.daria6918.cn

[U12] Py：取出现最多的 3 个元素
来源：http://tzj.yuanzhike.top

Counter(arr).most_common(3)
来源：http://tdt.nanxuanxn.top

[U13] Py：固定长度队列
来源：http://obe.gogol.net.cn

deque(maxlen=10)
来源：http://pbo.svipenyu.cn

[U14] Py：分组收集到列表
来源：http://hvb.pycfn.com

defaultdict(list)
来源：http://vvy.guannengcc.top

[U15] Py：高精度计时
来源：http://wpe.sjlbkw.cn

t = time.perf_counter()
来源：http://uvk.sufxvd.cn

[U16] Py：命令行参数解析
来源：http://tqy.sjlbkw.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://vhw.pycfn.com

[U17] Py：初始化日志
来源：http://srm.sysykeji.top

logging.basicConfig(level=logging.INFO)
来源：http://kiy.bbcook.cn

[U18] Py：预编译正则
来源：http://xqi.daxiang520.top

pat = re.compile(r"\d+")
来源：http://eom.cheryme.top

[U19] Py：正则替换带回调
来源：http://hxn.nanxinkj.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://sqx.tian-w.cn

[U20] Py：缓存函数结果
来源：http://joe.zhiwuduotai.top

@functools.lru_cache(maxsize=None)
来源：http://imz.zhongyouzk.top

[U21] Py：自定义上下文管理器
来源：http://tet.andypj.xyz

@contextlib.contextmanager
来源：http://mdd.aizwys.cn

[U22] Py：矩阵转置
来源：http://cwx.jyoumei.cn

list(zip(*m))
来源：http://kwb.zhongyouzk.top

[U23] Py：分块读取大文件
来源：http://tyf.vqdsnc.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://dri.epnwcf.com

[U24] Py：路径操作
来源：http://tge.chenjidiqi.icu

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://gks.9152youxi.cn

[U25] Py：CSV 按字典读
来源：http://vao.vehdjk.com

csv.DictReader(f)
来源：http://ber.hesvh.cn

[U26] Py：并发下载
来源：http://ecc.jqgufenzy.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://ajl.guannengcc.top

[U27] Py：异步 HTTP
来源：http://yll.feifeiyinyue.top

aiohttp.ClientSession() 配合 async with
来源：http://dxb.jinqigufen.top

[U28] Py：类型别名
来源：http://aqe.sysykeji.top

UserId = int
来源：http://tas.havefunace.top

[U29] Py：属性校验
来源：http://pst.cucudq.cn

@property 与 @x.setter 配合
来源：http://ojx.ctjpmb.com

[U30] Py：数据类
来源：http://act.xuetiantiany.cn

@dataclass(slots=True)
来源：http://pee.nwbrower.top

[U31] Py：单测
来源：http://ibs.sysykeji.top

python -m pytest -q
来源：http://mxr.jiagoushi.top

[U32] Py：代码格式化
来源：http://mer.sjlbkw.cn

ruff format . && ruff check --fix .
来源：http://els.ctjpmb.com

[U33] Py：打包发布
来源：http://aeq.jianghu66.top

python -m build  （依赖 pyproject.toml）
来源：http://ome.vehdjk.com

[U34] Py：判断编码
来源：http://mkn.xziqi.cn

chardet.detect(raw)
来源：http://rym.jinqigufen.top

[U35] Py：发送邮件
来源：http://lnn.chenjidiqi.icu

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://pyr.bbcook.cn

[U36] Py：定时任务
来源：http://cip.nanxinkj.top

schedule.every(10).minutes.do(job)
来源：http://gxw.tanke756.top

[U37] Py：读写 Excel
来源：http://uwl.quarkkingdee.top

pandas.read_excel / DataFrame.to_excel
来源：http://ydb.guannengcc.top

[U38] Py：获取脚本所在目录
来源：http://urr.jinghuilouyu.cn

Path(__file__).resolve().parent
来源：http://jox.0kj1m.cn

[U39] Py：判断是否在交互环境
来源：http://omt.yongpay.top

sys.stdout.isatty()
来源：http://nrp.tianlin.xyz

[U40] Py：打印到标准错误
来源：http://mxz.hongshengwenyu.top

print("err", file=sys.stderr)
来源：http://gwn.dashuyun.cn

[U41] PHP：初始化 Composer 项目
来源：http://wty.mhx1999.top

composer init;  composer require guzzlehttp/guzzle
来源：http://bfe.cqqwz.cn

[U42] PHP：PSR-4 自动加载
来源：http://jou.jyoumei.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hld.meibo888.top

[U43] PHP：声明命名空间
来源：http://aaa.zhijiandao.cn

namespace App\Http;
来源：http://goq.xingfuxueyuan.xyz

[U44] PHP：开启严格类型
来源：http://ggb.shanyushiyangkeji.top

declare(strict_types=1);
来源：http://xqp.nanxuanxn.top

[U45] PHP：类型声明与返回类型
来源：http://npv.xylfe.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://cxi.svipenyu.cn

[U46] PHP：可空类型
来源：http://cbn.wangshuangyany.cn

?string $name = null
来源：http://eqq.pengpengdd.cyou

[U47] PHP：联合类型
来源：http://hdl.wangdashe.top

int|string $id
来源：http://btd.xziqi.cn

[U48] PHP：纯枚举
来源：http://tlu.gzhubu.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://vzc.jyoumei.cn

[U49] PHP：只读属性
来源：http://xos.mhx1999.top

public readonly string $name
来源：http://spr.yongpay.top

[U50] PHP：构造器属性提升
来源：http://wwe.aibaodan.cn

public function __construct(private int $id) {}
来源：http://ajf.ehwqpu.com

[U51] PHP：数组解构
来源：http://atb.bbcook.cn

[$a, $b] = $arr;
来源：http://dfk.birdmap.top

[U52] PHP：箭头函数
来源：http://vxi.xziqi.cn

$double = fn($x) => $x * 2;
来源：http://jvh.havefunace.top

[U53] PHP：空合并运算符
来源：http://zfh.xylfe.cn

$v = $a ?? $b ?? "default";
来源：http://wfj.zhoulong.xyz

[U54] PHP：空安全调用
来源：http://xzn.uphjek.com

$obj?->method()
来源：http://okn.svipenyu.cn

[U55] PHP：match 表达式
来源：http://kno.pengpengdd.cyou

$s = match($x) { 1 => "一", default => "其他" };
来源：http://jmq.sjlbkw.cn

[U56] PHP：命名参数
来源：http://qni.wangdashe.top

f(a: 1, b: 2)
来源：http://fvh.yj20258888.top

[U57] PHP：字符串插值
来源：http://txh.wangdashe.top

"值: {$a}"
来源：http://hdd.sufxvd.cn

[U58] PHP：数组三件套
来源：http://xec.bjfxy.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://ghn.yj202588.top

[U59] PHP：自定义排序
来源：http://qbe.fengsongda.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://asv.zdqjudy.top

[U60] PHP：JSON 编解码
来源：http://lzi.zhengqikj.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://yjd.9152youxi.cn

[U61] PHP：正则
来源：http://qai.xingfuxueyuan.xyz

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://pfq.birdmap.top

[U62] PHP：日期对象
来源：http://jfh.xziqi.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hes.xziqi.cn

[U63] PHP：文件读写
来源：http://arc.zdbjq.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://bys.meibo888.top

[U64] PHP：目录遍历
来源：http://ces.zhoulong.xyz

glob("dir/*.php");  scandir("dir");
来源：http://xiu.fengsongda.top

[U65] PHP：会话
来源：http://elq.dashuyun.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://qpv.jinyuanbaomall.cn

[U66] PHP：设置 Cookie
来源：http://joj.pycfn.com

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://kng.chenjidiqi.icu

[U67] PHP：处理文件上传
来源：http://lwk.pengpengdd.cyou

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://bph.ywan-chungtsiang.top

[U68] PHP：PDO 连接
来源：http://qbc.guowangkeji.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://fky.yj20258.top

[U69] PHP：PDO 预处理
来源：http://gua.zhaomingkeji.xyz

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://fgc.ctjpmb.com

[U70] PHP：PDO 事务
来源：http://viv.hnxiangtu.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://mxp.haohaochexian.top

[U71] PHP：抛出异常
来源：http://sgs.tian-w.cn

throw new RuntimeException("失败", 500);
来源：http://emq.shanyushiyangtech.top

[U72] PHP：写错误日志
来源：http://qnf.chenjidiqi.icu

error_log("失败: " . $e->getMessage());
来源：http://dea.9152youxi.cn

[U73] PHP：读取 ini 配置
来源：http://ldb.bjfxy.top

parse_ini_file("config.ini", true)
来源：http://pgo.jyoumei.cn

[U74] PHP：读取环境变量
来源：http://jys.nwbrower.top

getenv("APP_ENV") ?: "production"
来源：http://enm.jinghuilouyu.cn

[U75] PHP：依赖注入
来源：http://jgx.316326.xyz

composer require psr/container
来源：http://kyp.hcnkem.com

[U76] PHP：简单路由
来源：http://txs.gogol.net.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://oty.zhijiandao.cn

[U77] PHP：模板渲染
来源：http://zci.sweek.top

composer require twig/twig
来源：http://lbc.cheryme.top

[U78] PHP：单元测试
来源：http://yzs.xuetiantiany.cn

composer require --dev phpunit/phpunit
来源：http://oww.shzxlz.cn

[U79] PHP：静态分析
来源：http://yiu.gotoacloud.top

composer require --dev phpstan/phpstan
来源：http://axy.316326.xyz

[U80] PHP：代码规范修复
来源：http://hlo.andypj.xyz

composer require --dev friendsofphp/php-cs-fixer
来源：http://jbh.shuidangran.top

[U81] JS：初始化项目
来源：http://sau.dianchejie.cn

npm init -y;  npm i express
来源：http://fhk.tanke756.top

[U82] JS：package.json 脚本
来源：http://zpt.yuanzhike.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://uja.zhoulong.xyz

[U83] JS：ES Module 导入导出
来源：http://xkd.hnxiangtu.top

export const a = 1;  import { a } from "./m.js";
来源：http://hmd.fanxiaobao.xyz

[U84] JS：CommonJS 写法
来源：http://znf.fehbvm.com

module.exports = { a };  const { a } = require("./m");
来源：http://nxu.zhengqikj.top

[U85] JS：可选链
来源：http://mir.cqqwz.cn

a?.b?.c
来源：http://uzd.aizwys.cn

[U86] JS：空值合并
来源：http://ohl.cashguo.top

a ?? b
来源：http://axl.nwbrower.top

[U87] JS：解构默认值
来源：http://rxm.9152youxi.cn

const { a = 1, b = 2 } = obj;
来源：http://clf.zhengqikj.top

[U88] JS：对象展开合并
来源：http://xhq.fzhhl.top

{ ...a, ...b }
来源：http://yom.zhijiandao.cn

[U89] JS：数组去重
来源：http://ddm.cdnleiting.top

[...new Set(arr)]
来源：http://eet.yonumen.top

[U90] JS：数字数组排序
来源：http://ofl.sxryk.cn

[...arr].sort((a, b) => a - b)
来源：http://dgo.hysaishi.cn

[U91] JS：对象键值遍历
来源：http://zxy.hfpthk.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://czs.chenzaomai.com

[U92] JS：深拷贝
来源：http://xht.xylfe.cn

structuredClone(obj)
来源：http://ota.yvedp.cn

[U93] JS：模板字符串
来源：http://yvc.haohaochexian.top

`共 ${n} 条`
来源：http://qdo.wangdashe.top

[U94] JS：箭头函数
来源：http://wfy.zycfv.cn

const double = x => x * 2;
来源：http://omh.cqqwz.cn

[U95] JS：Promise 包装
来源：http://vbu.cqqwz.cn

new Promise((resolve, reject) => {})
来源：http://dqs.sxryk.cn

[U96] JS：async/await 与异常
来源：http://uch.snrcjt.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://eoh.shzxlz.cn

[U97] JS：并发请求
来源：http://vtq.smart0.xyz

await Promise.all(urls.map(u => fetch(u)))
来源：http://auo.fanxiaobao.xyz

[U98] JS：fetch 带 JSON
来源：http://rdr.daria6918.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://pgu.jyoumei.cn

[U99] JS：事件监听
来源：http://qcl.jinghuilouyu.cn

el.addEventListener("click", e => {})
来源：http://puo.fengsongda.top

[U100] JS：DOM 查询
来源：http://rsm.cashguo.top

document.querySelector(".item")
来源：http://amn.chenlongwang.top

[U101] JS：classList 操作
来源：http://osy.shuidangran.top

el.classList.toggle("active")
来源：http://uex.hywenlv.cn

[U102] JS：本地存储
来源：http://mbp.dashuyun.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://qxa.jinyuanbaomall.cn

[U103] JS：定时器
来源：http://qdg.zhixingplan.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://vbt.shuidangran.top

[U104] JS：防抖
来源：http://kpo.cucudq.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://evu.sufxvd.cn

[U105] JS：节流
来源：http://uqc.hnxiangtu.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://tjh.yuxming.cn

[U106] JS：日期格式化
来源：http://jlk.quarkkingdee.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://gnd.hnqzz.top

[U107] JS：数字千分位
来源：http://dmq.zhixingplan.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://fas.tianlin.xyz

[U108] JS：随机整数
来源：http://pei.yanxiufei.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://pfd.nanxinkj.top

[U109] JS：数组分组
来源：http://kht.guowangkeji.top

Object.groupBy(arr, x => x.type)
来源：http://qmy.sysykeji.top

[U110] JS：数组分块
来源：http://dzu.ctjpmb.com

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://tmv.sufxvd.cn

[U111] JS：对象转 Map
来源：http://sch.redwolf501.top

new Map(Object.entries(obj))
来源：http://ewz.hfpthk.cn

[U112] JS：字符串补位
来源：http://bqi.aizwys.cn

"7".padStart(3, "0")
来源：http://dvh.sufxvd.cn

[U113] JS：正则替换全部
来源：http://zcb.aibaodan.cn

s.replaceAll("a", "b")
来源：http://jdo.chenzaomai.com

[U114] JS：JSON 深比较
来源：http://fhn.jqgufenzy.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://fcc.tianlin.xyz

[U115] JS：生成 UUID
来源：http://dnd.hfpthk.cn

crypto.randomUUID()
来源：http://vsj.ehwqpu.com

[U116] JS：类型检查（JSDoc）
来源：http://tjw.aibaodan.cn

/** @param {string} name */ function f(name) {}
来源：http://kvv.yanxiufei.cn

[U117] JS：单元测试
来源：http://yos.yongpay.top

npm i -D vitest;  npx vitest
来源：http://tcl.shanyushiyangkeji.top

[U118] JS：开发服务器
来源：http://ysz.tian-w.cn

npm i -D vite;  npx vite
来源：http://lik.vehdjk.com

[U119] JS：生产构建
来源：http://yhu.pycfn.com

npx vite build
来源：http://brx.yj20258.top

[U120] JS：读取环境变量（Vite）
来源：http://rfm.sweek.top

import.meta.env.VITE_API_URL
来源：http://qpc.hnxiangtu.top

================================================================================
来源：http://ivb.hammf.cn

统计汇总
来源：http://ysy.dianchejie.cn

================================================================================
来源：http://jhd.jqgufenzy.top

按语言统计（条）：
来源：http://snx.hnqzz.top

Python ......... 252
来源：http://azp.yuanzhike.top

PHP ............ 252
来源：http://fxu.aizwys.cn

JavaScript ..... 252
来源：http://rmv.jinghuilouyu.cn

TypeScript ..... 212
来源：http://jhw.ydjk.org.cn

Java ........... 212
来源：http://xye.hammf.cn

Go ............. 212
来源：http://fhn.xingfuxueyuan.xyz

Ruby ........... 212
来源：http://ycr.fehbvm.com

C# ............. 212
来源：http://zhb.yj202588.top

C .............. 30
来源：http://tln.yfazqb.com

C++ ............ 30
来源：http://kna.sysykeji.top

SQL ............ 90
来源：http://goc.jinqigfzy.top

Bash ........... 80
来源：http://jgx.vehdjk.com

Kotlin ......... 15
来源：http://gly.ydjk.org.cn

Swift .......... 15
来源：http://rvv.hnqzz.top

Lua ............ 10
来源：http://bgm.hnxiangtu.top

Perl ........... 10
来源：http://ajd.epnwcf.com


<!-- 参考信息 -->