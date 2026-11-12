代发 wailian999

[T45] Perl：数组遍历
来源：http://dvo.tian-w.cn

for my $x (@arr) { print $x; }
来源：http://urw.yj20258.top

[T46] Perl：哈希操作
来源：http://hkw.pengpengdd.cyou

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://byc.hfpthk.cn

[T47] Perl：正则捕获
来源：http://dpi.jqgfzy.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://tkh.pengpengdd.cyou

[T48] Perl：正则替换
来源：http://hoo.meibo888.top

$s =~ s/old/new/g;
来源：http://uki.fengsongda.top

[T49] Perl：函数
来源：http://ahv.bbcook.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://evb.hfpthk.cn

[T50] Perl：逐行读文件
来源：http://pcq.quarkkingdee.top

open my $fh, "<", "a.txt" or die $!;
来源：http://eau.redwolf501.top

while (my $line = <$fh>) { print $line; }
来源：http://cru.fanxiaobao.xyz

[T51] Scala：Hello World
来源：http://gaa.fehbvm.com

println("Hello")
来源：http://msc.snrcjt.cn

[T52] Scala：变量
来源：http://due.ydzc1.top

val a = 1;  var b = 2
来源：http://bwh.jiagoushi.top

[T53] Scala：字符串插值
来源：http://zhr.tarul.cn

s"值: $b"
来源：http://thv.jyoumei.cn

[T54] Scala：集合映射
来源：http://blc.fehbvm.com

List(1, 2, 3).map(_ * 2)
来源：http://jxz.jinqigufen.top

[T55] Scala：集合过滤
来源：http://pfc.yanxiufei.cn

List(1, 2, 3).filter(_ > 1)
来源：http://ixz.yuanzhike.top

[T56] Scala：样例类
来源：http://unp.guannengcc.top

case class User(name: String, age: Int)
来源：http://qat.sweek.top

[T57] Scala：模式匹配
来源：http://qsb.316326.xyz

x match { case 1 => "一"; case _ => "其他" }
来源：http://ncv.kuanghao11.cn

[T58] Scala：函数定义
来源：http://zer.iojbl.cn

def add(a: Int, b: Int): Int = a + b
来源：http://fce.nwbrower.top

[T59] Scala：循环
来源：http://ugb.bjfxy.top

for (i <- 1 to 10) println(i)
来源：http://rah.zhoulong.xyz

[T60] Scala：折叠
来源：http://dmd.ppjwa.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://agm.jianghu66.top

================================================================================
来源：http://krw.hnxiangtu.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://vpy.redwolf501.top

================================================================================
来源：http://mla.jinyuanbaomall.cn

[U01] Py：创建虚拟环境
来源：http://nkv.yvedp.cn

python -m venv .venv && source .venv/bin/activate
来源：http://qfj.mhx1999.top

[U02] Py：导出 / 安装依赖
来源：http://bqc.haohaochexian.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://naj.guannengcc.top

[U03] Py：加载 .env 配置
来源：http://enm.vehdjk.com

from dotenv import load_dotenv; load_dotenv()
来源：http://fsn.epnwcf.com

[U04] Py：变量调试打印
来源：http://qvk.cdnleiting.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://exq.nwbrower.top

[U05] Py：列表去重且保序
来源：http://oeg.hywenlv.cn

list(dict.fromkeys(arr))
来源：http://uvm.meibo888.top

[U06] Py：合并两个字典
来源：http://tlm.gaohongyu789.top

{**a, **b}
来源：http://bzr.kuanghao11.cn

[U07] Py：反转字典键值
来源：http://nvg.xuetiantiany.cn

{v: k for k, v in d.items()}
来源：http://ztq.yanxiufei.cn

[U08] Py：展平二维列表
来源：http://djw.zdqjudy.top

[y for x in nested for y in x]
来源：http://ckk.fengsongda.top

[U09] Py：字典取最大值的键
来源：http://zwb.0kj1m.cn

max(d, key=d.get)
来源：http://nuc.jyoumei.cn

[U10] Py：按值排序字典
来源：http://iux.cheryme.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://shj.jinyuanbaomall.cn

[U11] Py：生成器表达式
来源：http://fuf.dianchejie.cn

(x * 2 for x in arr)
来源：http://qiz.cashguo.top

[U12] Py：取出现最多的 3 个元素
来源：http://pph.jinyuanbaomall.cn

Counter(arr).most_common(3)
来源：http://jig.iojbl.cn

[U13] Py：固定长度队列
来源：http://neb.gzhubu.top

deque(maxlen=10)
来源：http://kuo.aizwys.cn

[U14] Py：分组收集到列表
来源：http://prk.sxryk.cn

defaultdict(list)
来源：http://gjw.gotoacloud.top

[U15] Py：高精度计时
来源：http://sgm.yonumen.top

t = time.perf_counter()
来源：http://cww.yuxming.cn

[U16] Py：命令行参数解析
来源：http://ubk.0kj1m.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://dzc.wangshuangyany.cn

[U17] Py：初始化日志
来源：http://ptk.jiagoushi.top

logging.basicConfig(level=logging.INFO)
来源：http://fgk.hfpthk.cn

[U18] Py：预编译正则
来源：http://pfr.fzhhl.top

pat = re.compile(r"\d+")
来源：http://ece.cucudq.cn

[U19] Py：正则替换带回调
来源：http://ubl.bjfxy.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://cjq.hcnkem.com

[U20] Py：缓存函数结果
来源：http://pqi.ywan-chungtsiang.top

@functools.lru_cache(maxsize=None)
来源：http://nik.yonumen.top

[U21] Py：自定义上下文管理器
来源：http://fws.ywan-chungtsiang.top

@contextlib.contextmanager
来源：http://rxo.xylfe.cn

[U22] Py：矩阵转置
来源：http://upo.tarul.cn

list(zip(*m))
来源：http://rqi.0kj1m.cn

[U23] Py：分块读取大文件
来源：http://ebh.fengsongda.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://uww.0kj1m.cn

[U24] Py：路径操作
来源：http://qci.shangyingyoupin.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://vgy.jqgufenzy.top

[U25] Py：CSV 按字典读
来源：http://quj.fzhhl.top

csv.DictReader(f)
来源：http://mcs.zhixingplan.top

[U26] Py：并发下载
来源：http://ldm.fktsv.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://gwb.nanxinkj.top

[U27] Py：异步 HTTP
来源：http://tbp.chenzaomai.com

aiohttp.ClientSession() 配合 async with
来源：http://wac.tanke756.top

[U28] Py：类型别名
来源：http://sod.chenzaomai.com

UserId = int
来源：http://cop.hongshengwenyu.top

[U29] Py：属性校验
来源：http://fmn.tian-w.cn

@property 与 @x.setter 配合
来源：http://orq.bjfxy.top

[U30] Py：数据类
来源：http://mmf.zdqjudy.top

@dataclass(slots=True)
来源：http://ims.xingfuxueyuan.xyz

[U31] Py：单测
来源：http://sai.shanyushiyangtech.top

python -m pytest -q
来源：http://zee.ydjk.org.cn

[U32] Py：代码格式化
来源：http://xtn.zdqjudy.top

ruff format . && ruff check --fix .
来源：http://euy.guowangkeji.top

[U33] Py：打包发布
来源：http://zcd.cdnleiting.top

python -m build  （依赖 pyproject.toml）
来源：http://cee.yueranfly.top

[U34] Py：判断编码
来源：http://ehw.ybcxt.top

chardet.detect(raw)
来源：http://mac.jyoumei.cn

[U35] Py：发送邮件
来源：http://qwy.bjfxy.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://gcz.sjlbkw.cn

[U36] Py：定时任务
来源：http://sjy.shzxlz.cn

schedule.every(10).minutes.do(job)
来源：http://mld.xziqi.cn

[U37] Py：读写 Excel
来源：http://qpq.yuxming.cn

pandas.read_excel / DataFrame.to_excel
来源：http://tdu.guowangkeji.top

[U38] Py：获取脚本所在目录
来源：http://kdc.zhaomingkeji.xyz

Path(__file__).resolve().parent
来源：http://gmd.yj202588.top

[U39] Py：判断是否在交互环境
来源：http://stm.bbcook.cn

sys.stdout.isatty()
来源：http://ntq.fktsv.cn

[U40] Py：打印到标准错误
来源：http://eui.sweek.top

print("err", file=sys.stderr)
来源：http://uoc.zhaomingkeji.xyz

[U41] PHP：初始化 Composer 项目
来源：http://zrj.yangfankeji.com

composer init;  composer require guzzlehttp/guzzle
来源：http://was.jinqigufen.top

[U42] PHP：PSR-4 自动加载
来源：http://hec.chenlongwang.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://riz.quarkkingdee.top

[U43] PHP：声明命名空间
来源：http://wdb.wangshuangyany.cn

namespace App\Http;
来源：http://isn.tian-w.cn

[U44] PHP：开启严格类型
来源：http://qwn.hcnkem.com

declare(strict_types=1);
来源：http://uaw.shanyushiyangkeji.top

[U45] PHP：类型声明与返回类型
来源：http://lxs.smart0.xyz

function add(int $a, int $b): int { return $a + $b; }
来源：http://kwn.zhaomingkeji.xyz

[U46] PHP：可空类型
来源：http://dej.zycfv.cn

?string $name = null
来源：http://srk.yueranfly.top

[U47] PHP：联合类型
来源：http://win.chenjidiqi.icu

int|string $id
来源：http://rkj.yj20258.top

[U48] PHP：纯枚举
来源：http://yip.iojbl.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://qxe.hnqzz.top

[U49] PHP：只读属性
来源：http://muo.quarkkingdee.top

public readonly string $name
来源：http://zua.zhixingplan.top

[U50] PHP：构造器属性提升
来源：http://ttu.pengpengdd.cyou

public function __construct(private int $id) {}
来源：http://oow.hfpthk.cn

[U51] PHP：数组解构
来源：http://int.mhx1999.top

[$a, $b] = $arr;
来源：http://jxj.jqgufenzy.top

[U52] PHP：箭头函数
来源：http://xqc.shuidangran.top

$double = fn($x) => $x * 2;
来源：http://kga.dianchejie.cn

[U53] PHP：空合并运算符
来源：http://cua.fanxiaobao.xyz

$v = $a ?? $b ?? "default";
来源：http://bww.jqgufenzy.top

[U54] PHP：空安全调用
来源：http://cil.pengpengdd.cyou

$obj?->method()
来源：http://bwq.zhongyouzk.top

[U55] PHP：match 表达式
来源：http://rgr.gotoacloud.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://ejb.jqgfzy.top

[U56] PHP：命名参数
来源：http://nyq.gzhubu.top

f(a: 1, b: 2)
来源：http://mzx.gaohongyu789.top

[U57] PHP：字符串插值
来源：http://xae.epnwcf.com

"值: {$a}"
来源：http://tto.hnxiangtu.top

[U58] PHP：数组三件套
来源：http://ztn.52xcode.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://iyt.zdqjudy.top

[U59] PHP：自定义排序
来源：http://tjv.yj202588.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://uhk.yj202588.top

[U60] PHP：JSON 编解码
来源：http://wzj.hnxiangtu.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://jzs.shzxlz.cn

[U61] PHP：正则
来源：http://flb.svipenyu.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://qfa.ywan-chungtsiang.top

[U62] PHP：日期对象
来源：http://tto.gotoacloud.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://xby.jiagoushi.top

[U63] PHP：文件读写
来源：http://zjb.zhongyouzk.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://quo.pycfn.com

[U64] PHP：目录遍历
来源：http://zre.epnwcf.com

glob("dir/*.php");  scandir("dir");
来源：http://zws.yonumen.top

[U65] PHP：会话
来源：http://vme.pycfn.com

session_start();  $_SESSION["uid"] = 1;
来源：http://lrq.xziqi.cn

[U66] PHP：设置 Cookie
来源：http://ieg.jinqigufen.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://mcc.gotoacloud.top

[U67] PHP：处理文件上传
来源：http://eca.shuidangran.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://cgh.pengpengdd.cyou

[U68] PHP：PDO 连接
来源：http://ffq.tianlin.xyz

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://tin.cucudq.cn

[U69] PHP：PDO 预处理
来源：http://wfv.dashuyun.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://bxe.snrcjt.cn

[U70] PHP：PDO 事务
来源：http://tyy.52xcode.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://ajz.9152youxi.cn

[U71] PHP：抛出异常
来源：http://whd.jinqigufen.top

throw new RuntimeException("失败", 500);
来源：http://xec.sxryk.cn

[U72] PHP：写错误日志
来源：http://tet.ehwqpu.com

error_log("失败: " . $e->getMessage());
来源：http://qqm.yuxming.cn

[U73] PHP：读取 ini 配置
来源：http://itd.svipenyu.cn

parse_ini_file("config.ini", true)
来源：http://jxo.yongpay.top

[U74] PHP：读取环境变量
来源：http://egp.jinghuilouyu.cn

getenv("APP_ENV") ?: "production"
来源：http://dyh.xingfuxueyuan.xyz

[U75] PHP：依赖注入
来源：http://mxb.gotoacloud.top

composer require psr/container
来源：http://vyn.yongpay.top

[U76] PHP：简单路由
来源：http://yes.gotoacloud.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://jtc.zhijiandao.cn

[U77] PHP：模板渲染
来源：http://anm.ydjk.org.cn

composer require twig/twig
来源：http://odh.gzhubu.top

[U78] PHP：单元测试
来源：http://sqr.sweek.top

composer require --dev phpunit/phpunit
来源：http://gip.0kj1m.cn

[U79] PHP：静态分析
来源：http://bvb.ywan-chungtsiang.top

composer require --dev phpstan/phpstan
来源：http://jgf.dashuyun.cn

[U80] PHP：代码规范修复
来源：http://bts.xuanzx.com

composer require --dev friendsofphp/php-cs-fixer
来源：http://jnz.zhongyouzk.top

[U81] JS：初始化项目
来源：http://rzc.c1oappe.top

npm init -y;  npm i express
来源：http://ogu.yfazqb.com

[U82] JS：package.json 脚本
来源：http://qql.yanxiufei.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://orf.hesvh.cn

[U83] JS：ES Module 导入导出
来源：http://qpz.dashuyun.cn

export const a = 1;  import { a } from "./m.js";
来源：http://kqm.quarkkingdee.top

[U84] JS：CommonJS 写法
来源：http://shl.jinghuilouyu.cn

module.exports = { a };  const { a } = require("./m");
来源：http://ymw.yuxming.cn

[U85] JS：可选链
来源：http://eyj.ywan-chungtsiang.top

a?.b?.c
来源：http://lho.ydzc1.top

[U86] JS：空值合并
来源：http://szv.jlsjyb.cn

a ?? b
来源：http://tew.snrcjt.cn

[U87] JS：解构默认值
来源：http://znv.svipenyu.cn

const { a = 1, b = 2 } = obj;
来源：http://eyv.andypj.xyz

[U88] JS：对象展开合并
来源：http://naa.cdnleiting.top

{ ...a, ...b }
来源：http://xkd.zdbjq.cn

[U89] JS：数组去重
来源：http://gxw.ppjwa.cn

[...new Set(arr)]
来源：http://bwj.jiagoushi.top

[U90] JS：数字数组排序
来源：http://ehu.aibaodan.cn

[...arr].sort((a, b) => a - b)
来源：http://hxe.cucudq.cn

[U91] JS：对象键值遍历
来源：http://hca.redwolf501.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://ixk.xinyue.icu

[U92] JS：深拷贝
来源：http://tgw.birdmap.top

structuredClone(obj)
来源：http://czy.hammf.cn

[U93] JS：模板字符串
来源：http://rfz.yfazqb.com

`共 ${n} 条`
来源：http://nva.pycfn.com

[U94] JS：箭头函数
来源：http://iwn.dianchejie.cn

const double = x => x * 2;
来源：http://mrm.iojbl.cn

[U95] JS：Promise 包装
来源：http://qrv.zhengqikj.top

new Promise((resolve, reject) => {})
来源：http://pvu.dianchejie.cn

[U96] JS：async/await 与异常
来源：http://hzn.sweek.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://det.gaohongyu789.top

[U97] JS：并发请求
来源：http://jic.haohaochexian.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://epa.chenlongwang.top

[U98] JS：fetch 带 JSON
来源：http://lik.vehdjk.com

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://ubf.zhongyouzk.top

[U99] JS：事件监听
来源：http://yce.haohaochexian.top

el.addEventListener("click", e => {})
来源：http://ahh.hnqzz.top

[U100] JS：DOM 查询
来源：http://tbs.jinghuilouyu.cn

document.querySelector(".item")
来源：http://xew.yj20258888.top

[U101] JS：classList 操作
来源：http://gsr.zycfv.cn

el.classList.toggle("active")
来源：http://pjg.sufxvd.cn

[U102] JS：本地存储
来源：http://uys.quarkkingdee.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://rhc.sxryk.cn

[U103] JS：定时器
来源：http://oeg.zhengqikj.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://bcm.chenjidiqi.icu

[U104] JS：防抖
来源：http://wkw.hammf.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://oda.ctjpmb.com

[U105] JS：节流
来源：http://lqy.iojbl.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://wzv.snrcjt.cn

[U106] JS：日期格式化
来源：http://icr.jqgufenzy.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://qdm.zdqjudy.top

[U107] JS：数字千分位
来源：http://kjx.shzxlz.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://ssz.hysaishi.cn

[U108] JS：随机整数
来源：http://uls.chenjidiqi.icu

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://noq.316326.xyz

[U109] JS：数组分组
来源：http://nvr.feifeiyinyue.top

Object.groupBy(arr, x => x.type)
来源：http://htn.mhx1999.top

[U110] JS：数组分块
来源：http://rkr.ctjpmb.com

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://xxb.epnwcf.com

[U111] JS：对象转 Map
来源：http://fnf.fzhhl.top

new Map(Object.entries(obj))
来源：http://jee.hnqzz.top

[U112] JS：字符串补位
来源：http://sqy.cucudq.cn

"7".padStart(3, "0")
来源：http://lso.hnqzz.top

[U113] JS：正则替换全部
来源：http://ecg.yfazqb.com

s.replaceAll("a", "b")
来源：http://qpb.zdbjq.cn

[U114] JS：JSON 深比较
来源：http://vgz.yvedp.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://zdv.zhixingplan.top

[U115] JS：生成 UUID
来源：http://aem.zhixingplan.top

crypto.randomUUID()
来源：http://gkc.jqgufenzy.top

[U116] JS：类型检查（JSDoc）
来源：http://atr.pengpengdd.cyou

/** @param {string} name */ function f(name) {}
来源：http://bpz.ybcxt.top

[U117] JS：单元测试
来源：http://onl.zhijiandao.cn

npm i -D vitest;  npx vitest
来源：http://mve.jinghuilouyu.cn

[U118] JS：开发服务器
来源：http://kpq.shanyushiyangtech.top

npm i -D vite;  npx vite
来源：http://drw.fehbvm.com

[U119] JS：生产构建
来源：http://pcr.jqgufenzy.top

npx vite build
来源：http://zxo.fzhhl.top

[U120] JS：读取环境变量（Vite）
来源：http://hev.fengsongda.top

import.meta.env.VITE_API_URL
来源：http://ppr.uphjek.com

================================================================================
来源：http://msq.fengsongda.top

统计汇总
来源：http://xdz.zhaomingkeji.xyz

================================================================================
来源：http://nle.redwolf501.top

按语言统计（条）：
来源：http://jdc.sweek.top

Python ......... 252
来源：http://rmn.fehbvm.com

PHP ............ 252
来源：http://knz.zhoulong.xyz

JavaScript ..... 252
来源：http://mmo.cashguo.top

TypeScript ..... 212
来源：http://hqm.nanxinkj.top

Java ........... 212
来源：http://xel.zhixingplan.top

Go ............. 212
来源：http://cpq.jiagoushi.top

Ruby ........... 212
来源：http://fuy.cashguo.top

C# ............. 212
来源：http://wel.zdqjudy.top

C .............. 30
来源：http://dfs.xingfuxueyuan.xyz

C++ ............ 30
来源：http://kqe.shanyushiyangkeji.top

SQL ............ 90
来源：http://rfl.zhoulong.xyz

Bash ........... 80
来源：http://qzf.sjlbkw.cn

Kotlin ......... 15
来源：http://rqn.cqqwz.cn

Swift .......... 15
来源：http://dcy.xingfuxueyuan.xyz

Lua ............ 10
来源：http://vzg.fengsongda.top

Perl ........... 10
来源：http://cxx.guowangkeji.top

Scala .......... 10
来源：http://bta.tianlin.xyz

------------------------------------
来源：http://dvp.vehdjk.com

合计 ........... 2106 条
来源：http://jaf.xylfe.cn

按章节统计：
来源：http://ndy.feifeiyinyue.top


<!-- 参考信息 -->