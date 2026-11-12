代发 wailian999

[T49] Perl：函数
来源：http://fbb.wangshuangyany.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://mnx.zhongyouzk.top

[T50] Perl：逐行读文件
来源：http://jab.tarul.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://zrh.zhiwuduotai.top

while (my $line = <$fh>) { print $line; }
来源：http://lgr.zhengqikj.top

[T51] Scala：Hello World
来源：http://hca.xuanzx.com

println("Hello")
来源：http://fhw.zhijiandao.cn

[T52] Scala：变量
来源：http://udd.zdbjq.cn

val a = 1;  var b = 2
来源：http://uqy.jqgfzy.top

[T53] Scala：字符串插值
来源：http://xav.quarkkingdee.top

s"值: $b"
来源：http://bay.fanxiaobao.xyz

[T54] Scala：集合映射
来源：http://cop.chenlongwang.top

List(1, 2, 3).map(_ * 2)
来源：http://hdp.guowangkeji.top

[T55] Scala：集合过滤
来源：http://lzj.jlsjyb.cn

List(1, 2, 3).filter(_ > 1)
来源：http://pad.jlsjyb.cn

[T56] Scala：样例类
来源：http://wbq.tanke756.top

case class User(name: String, age: Int)
来源：http://cku.yuanzhike.top

[T57] Scala：模式匹配
来源：http://cxc.zdqjudy.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://lqf.gogol.net.cn

[T58] Scala：函数定义
来源：http://txb.dianchejie.cn

def add(a: Int, b: Int): Int = a + b
来源：http://eka.haohaochexian.top

[T59] Scala：循环
来源：http://hcb.hnqzz.top

for (i <- 1 to 10) println(i)
来源：http://xkc.cheryme.top

[T60] Scala：折叠
来源：http://oee.jqgfzy.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://ppp.jianghu66.top

================================================================================
来源：http://ylj.cdnleiting.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://omo.nanxuanxn.top

================================================================================
来源：http://njs.yj202588.top

[U01] Py：创建虚拟环境
来源：http://wjj.fzhhl.top

python -m venv .venv && source .venv/bin/activate
来源：http://otl.jiagoushi.top

[U02] Py：导出 / 安装依赖
来源：http://dnn.zhoulong.xyz

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://wag.jiagoushi.top

[U03] Py：加载 .env 配置
来源：http://jkx.zhengqikj.top

from dotenv import load_dotenv; load_dotenv()
来源：http://wji.zdbjq.cn

[U04] Py：变量调试打印
来源：http://ydb.wangdashe.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://zam.jqgufenzy.top

[U05] Py：列表去重且保序
来源：http://pdr.gzhubu.top

list(dict.fromkeys(arr))
来源：http://mmw.ppjwa.cn

[U06] Py：合并两个字典
来源：http://vdt.guowangkeji.top

{**a, **b}
来源：http://nkd.52xcode.cn

[U07] Py：反转字典键值
来源：http://pgm.shzxlz.cn

{v: k for k, v in d.items()}
来源：http://cbk.guannengcc.top

[U08] Py：展平二维列表
来源：http://wwy.uphjek.com

[y for x in nested for y in x]
来源：http://qlj.ctjpmb.com

[U09] Py：字典取最大值的键
来源：http://smy.shzxlz.cn

max(d, key=d.get)
来源：http://cvs.yonumen.top

[U10] Py：按值排序字典
来源：http://ybm.tanke756.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://ozm.jlsjyb.cn

[U11] Py：生成器表达式
来源：http://rqc.jinqigufen.top

(x * 2 for x in arr)
来源：http://tsg.ppjwa.cn

[U12] Py：取出现最多的 3 个元素
来源：http://uwf.zycfv.cn

Counter(arr).most_common(3)
来源：http://yzd.jqgufenzy.top

[U13] Py：固定长度队列
来源：http://hhp.shanyushiyangkeji.top

deque(maxlen=10)
来源：http://opj.cdnleiting.top

[U14] Py：分组收集到列表
来源：http://ftf.zhijiandao.cn

defaultdict(list)
来源：http://lyh.chenzaomai.com

[U15] Py：高精度计时
来源：http://rws.yuanzhike.top

t = time.perf_counter()
来源：http://qkq.haohaochexian.top

[U16] Py：命令行参数解析
来源：http://kju.vehdjk.com

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://kuy.guannengcc.top

[U17] Py：初始化日志
来源：http://ebx.quarkkingdee.top

logging.basicConfig(level=logging.INFO)
来源：http://yjk.gaohongyu789.top

[U18] Py：预编译正则
来源：http://gnu.sufxvd.cn

pat = re.compile(r"\d+")
来源：http://bqz.shangyingyoupin.top

[U19] Py：正则替换带回调
来源：http://zyn.yvedp.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://pdx.cqqwz.cn

[U20] Py：缓存函数结果
来源：http://axl.hesvh.cn

@functools.lru_cache(maxsize=None)
来源：http://fgx.yuanzhike.top

[U21] Py：自定义上下文管理器
来源：http://yke.redwolf501.top

@contextlib.contextmanager
来源：http://qgz.chenlongwang.top

[U22] Py：矩阵转置
来源：http://gqt.tian-w.cn

list(zip(*m))
来源：http://mjt.svipenyu.cn

[U23] Py：分块读取大文件
来源：http://jns.birdmap.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://vtk.cheryme.top

[U24] Py：路径操作
来源：http://vdz.guowangkeji.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://wca.yj20258888.top

[U25] Py：CSV 按字典读
来源：http://bsm.zdqjudy.top

csv.DictReader(f)
来源：http://urg.dashuyun.cn

[U26] Py：并发下载
来源：http://odv.iojbl.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://jyj.epnwcf.com

[U27] Py：异步 HTTP
来源：http://mis.yonumen.top

aiohttp.ClientSession() 配合 async with
来源：http://qmi.tarul.cn

[U28] Py：类型别名
来源：http://qna.hfpthk.cn

UserId = int
来源：http://bod.quarkkingdee.top

[U29] Py：属性校验
来源：http://tyy.ctjpmb.com

@property 与 @x.setter 配合
来源：http://owr.yangfankeji.com

[U30] Py：数据类
来源：http://org.redwolf501.top

@dataclass(slots=True)
来源：http://yxx.wangdashe.top

[U31] Py：单测
来源：http://fiz.ybcxt.top

python -m pytest -q
来源：http://una.xziqi.cn

[U32] Py：代码格式化
来源：http://mng.nanxuanxn.top

ruff format . && ruff check --fix .
来源：http://oyp.dashuyun.cn

[U33] Py：打包发布
来源：http://mnf.hammf.cn

python -m build  （依赖 pyproject.toml）
来源：http://bke.vehdjk.com

[U34] Py：判断编码
来源：http://msy.hcnkem.com

chardet.detect(raw)
来源：http://vmr.chenlongwang.top

[U35] Py：发送邮件
来源：http://dji.chenzaomai.com

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://psv.dashuyun.cn

[U36] Py：定时任务
来源：http://uub.ivvv.top

schedule.every(10).minutes.do(job)
来源：http://dff.sysykeji.top

[U37] Py：读写 Excel
来源：http://vzr.316326.xyz

pandas.read_excel / DataFrame.to_excel
来源：http://elo.zhaomingkeji.xyz

[U38] Py：获取脚本所在目录
来源：http://vnb.dianchejie.cn

Path(__file__).resolve().parent
来源：http://ihk.hcnkem.com

[U39] Py：判断是否在交互环境
来源：http://hwv.bbcook.cn

sys.stdout.isatty()
来源：http://qfy.hongshengwenyu.top

[U40] Py：打印到标准错误
来源：http://qca.ywan-chungtsiang.top

print("err", file=sys.stderr)
来源：http://xtn.dianchejie.cn

[U41] PHP：初始化 Composer 项目
来源：http://yic.yuxming.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://alp.nwbrower.top

[U42] PHP：PSR-4 自动加载
来源：http://dkx.smart0.xyz

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://teb.gaohongyu789.top

[U43] PHP：声明命名空间
来源：http://hrt.yj20258888.top

namespace App\Http;
来源：http://cys.316326.xyz

[U44] PHP：开启严格类型
来源：http://wgv.xuanzx.com

declare(strict_types=1);
来源：http://uut.yanxiufei.cn

[U45] PHP：类型声明与返回类型
来源：http://hxg.havefunace.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://mnm.svipenyu.cn

[U46] PHP：可空类型
来源：http://sdo.sysykeji.top

?string $name = null
来源：http://mzm.zhaomingkeji.xyz

[U47] PHP：联合类型
来源：http://oan.sweek.top

int|string $id
来源：http://ccr.xuetiantiany.cn

[U48] PHP：纯枚举
来源：http://xpq.jlsjyb.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://qkg.zhoulong.xyz

[U49] PHP：只读属性
来源：http://qze.iojbl.cn

public readonly string $name
来源：http://zmt.quarkkingdee.top

[U50] PHP：构造器属性提升
来源：http://deg.tian-w.cn

public function __construct(private int $id) {}
来源：http://ouv.gzhubu.top

[U51] PHP：数组解构
来源：http://pdq.yfazqb.com

[$a, $b] = $arr;
来源：http://jqa.ybcxt.top

[U52] PHP：箭头函数
来源：http://daa.nanxuanxn.top

$double = fn($x) => $x * 2;
来源：http://bod.yongpay.top

[U53] PHP：空合并运算符
来源：http://kiv.ydzc1.top

$v = $a ?? $b ?? "default";
来源：http://sig.uphjek.com

[U54] PHP：空安全调用
来源：http://dna.sufxvd.cn

$obj?->method()
来源：http://sft.hywenlv.cn

[U55] PHP：match 表达式
来源：http://mmz.ydjk.org.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://dmp.wangshuangyany.cn

[U56] PHP：命名参数
来源：http://yam.zhiwuduotai.top

f(a: 1, b: 2)
来源：http://abr.shzxlz.cn

[U57] PHP：字符串插值
来源：http://qpt.jianghu66.top

"值: {$a}"
来源：http://iqo.jinghuilouyu.cn

[U58] PHP：数组三件套
来源：http://bbn.fengsongda.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://zog.dianchejie.cn

[U59] PHP：自定义排序
来源：http://fvf.ydzc1.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://gpt.svipenyu.cn

[U60] PHP：JSON 编解码
来源：http://utl.sweek.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://vrm.xingfuxueyuan.xyz

[U61] PHP：正则
来源：http://ouo.feifeiyinyue.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://gxn.zhaomingkeji.xyz

[U62] PHP：日期对象
来源：http://ofz.xziqi.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://zlc.jqgufenzy.top

[U63] PHP：文件读写
来源：http://vpn.jyoumei.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://kdw.meibo888.top

[U64] PHP：目录遍历
来源：http://lcx.snrcjt.cn

glob("dir/*.php");  scandir("dir");
来源：http://uub.shzxlz.cn

[U65] PHP：会话
来源：http://cie.xuetiantiany.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://ppq.chenlongwang.top

[U66] PHP：设置 Cookie
来源：http://lyx.zhaomingkeji.xyz

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://sol.xingfuxueyuan.xyz

[U67] PHP：处理文件上传
来源：http://okz.dianchejie.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://vvl.yonumen.top

[U68] PHP：PDO 连接
来源：http://fit.52xcode.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://zuw.tarul.cn

[U69] PHP：PDO 预处理
来源：http://puj.316326.xyz

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://wxe.zycfv.cn

[U70] PHP：PDO 事务
来源：http://vuw.gogol.net.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://ezl.sjlbkw.cn

[U71] PHP：抛出异常
来源：http://lar.zycfv.cn

throw new RuntimeException("失败", 500);
来源：http://swz.xinyue.icu

[U72] PHP：写错误日志
来源：http://bvk.hfpthk.cn

error_log("失败: " . $e->getMessage());
来源：http://dqi.chenjidiqi.icu

[U73] PHP：读取 ini 配置
来源：http://mul.fengsongda.top

parse_ini_file("config.ini", true)
来源：http://wjf.shangyingyoupin.top

[U74] PHP：读取环境变量
来源：http://dzt.tanke756.top

getenv("APP_ENV") ?: "production"
来源：http://ozd.guowangkeji.top

[U75] PHP：依赖注入
来源：http://sos.chenjidiqi.icu

composer require psr/container
来源：http://fid.guowangkeji.top

[U76] PHP：简单路由
来源：http://tdg.zhiwuduotai.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://hii.yj202588.top

[U77] PHP：模板渲染
来源：http://zmr.yj202588.top

composer require twig/twig
来源：http://mfn.yvedp.cn

[U78] PHP：单元测试
来源：http://xxf.shanyushiyangkeji.top

composer require --dev phpunit/phpunit
来源：http://srr.tianlin.xyz

[U79] PHP：静态分析
来源：http://kbs.gaohongyu789.top

composer require --dev phpstan/phpstan
来源：http://uyb.birdmap.top

[U80] PHP：代码规范修复
来源：http://kpk.guowangkeji.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://gou.zhiwuduotai.top

[U81] JS：初始化项目
来源：http://nxf.hnqzz.top

npm init -y;  npm i express
来源：http://kcf.tarul.cn

[U82] JS：package.json 脚本
来源：http://zwl.fehbvm.com

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://php.quarkkingdee.top

[U83] JS：ES Module 导入导出
来源：http://fuw.shzxlz.cn

export const a = 1;  import { a } from "./m.js";
来源：http://eur.sufxvd.cn

[U84] JS：CommonJS 写法
来源：http://rtx.zhoulong.xyz

module.exports = { a };  const { a } = require("./m");
来源：http://rer.dashuyun.cn

[U85] JS：可选链
来源：http://mec.xinyue.icu

a?.b?.c
来源：http://zdt.jinghuilouyu.cn

[U86] JS：空值合并
来源：http://cfj.ybcxt.top

a ?? b
来源：http://sug.dashuyun.cn

[U87] JS：解构默认值
来源：http://rjf.sysykeji.top

const { a = 1, b = 2 } = obj;
来源：http://cmg.redwolf501.top

[U88] JS：对象展开合并
来源：http://hvb.nanxinkj.top

{ ...a, ...b }
来源：http://yov.yvedp.cn

[U89] JS：数组去重
来源：http://meg.shzxlz.cn

[...new Set(arr)]
来源：http://qol.shuidangran.top

[U90] JS：数字数组排序
来源：http://eij.cucudq.cn

[...arr].sort((a, b) => a - b)
来源：http://xyq.redwolf501.top

[U91] JS：对象键值遍历
来源：http://etp.zhijiandao.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://iis.zhijiandao.cn

[U92] JS：深拷贝
来源：http://rtd.sufxvd.cn

structuredClone(obj)
来源：http://lfm.sysykeji.top

[U93] JS：模板字符串
来源：http://xdy.jinqigufen.top

`共 ${n} 条`
来源：http://aka.daria6918.cn

[U94] JS：箭头函数
来源：http://xke.hysaishi.cn

const double = x => x * 2;
来源：http://nfj.xuetiantiany.cn

[U95] JS：Promise 包装
来源：http://ybz.tarul.cn

new Promise((resolve, reject) => {})
来源：http://bgc.zycfv.cn

[U96] JS：async/await 与异常
来源：http://gva.sufxvd.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://pfm.nwbrower.top

[U97] JS：并发请求
来源：http://auq.jinyuanbaomall.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://chm.yongpay.top

[U98] JS：fetch 带 JSON
来源：http://riu.quarkkingdee.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://olj.mhx1999.top

[U99] JS：事件监听
来源：http://dgl.cheryme.top

el.addEventListener("click", e => {})
来源：http://mlg.xingfuxueyuan.xyz

[U100] JS：DOM 查询
来源：http://fsp.fktsv.cn

document.querySelector(".item")
来源：http://cqy.ybcxt.top

[U101] JS：classList 操作
来源：http://eza.hfpthk.cn

el.classList.toggle("active")
来源：http://taq.nanxinkj.top

[U102] JS：本地存储
来源：http://gwd.jqgufenzy.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://rtd.quarkkingdee.top

[U103] JS：定时器
来源：http://tcr.c1oappe.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://kow.shzxlz.cn

[U104] JS：防抖
来源：http://nib.vehdjk.com

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://qab.fehbvm.com

[U105] JS：节流
来源：http://pnp.c1oappe.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://aky.shuidangran.top

[U106] JS：日期格式化
来源：http://kft.hcnkem.com

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://qnv.tanke756.top

[U107] JS：数字千分位
来源：http://hno.jinyuanbaomall.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://nrx.zhengqikj.top

[U108] JS：随机整数
来源：http://nfa.guowangkeji.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://src.pycfn.com

[U109] JS：数组分组
来源：http://dic.snrcjt.cn

Object.groupBy(arr, x => x.type)
来源：http://qqc.svipenyu.cn

[U110] JS：数组分块
来源：http://bnk.zhiwuduotai.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://zzj.yanxiufei.cn

[U111] JS：对象转 Map
来源：http://yhh.xingfuxueyuan.xyz

new Map(Object.entries(obj))
来源：http://twy.kuanghao11.cn

[U112] JS：字符串补位
来源：http://fzh.fanxiaobao.xyz

"7".padStart(3, "0")
来源：http://vpk.vqdsnc.cn

[U113] JS：正则替换全部
来源：http://fht.hnqzz.top

s.replaceAll("a", "b")
来源：http://bcz.sysykeji.top

[U114] JS：JSON 深比较
来源：http://avl.hnxiangtu.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://uha.shangyingyoupin.top

[U115] JS：生成 UUID
来源：http://nxw.mhx1999.top

crypto.randomUUID()
来源：http://vze.yangfankeji.com

[U116] JS：类型检查（JSDoc）
来源：http://rkk.gzhubu.top

/** @param {string} name */ function f(name) {}
来源：http://ceh.fzhhl.top

[U117] JS：单元测试
来源：http://cul.hfpthk.cn

npm i -D vitest;  npx vitest
来源：http://got.gogol.net.cn

[U118] JS：开发服务器
来源：http://pqt.hongshengwenyu.top

npm i -D vite;  npx vite
来源：http://ekn.hnqzz.top

[U119] JS：生产构建
来源：http://vip.sjlbkw.cn

npx vite build
来源：http://lzq.xziqi.cn

[U120] JS：读取环境变量（Vite）
来源：http://eey.fzhhl.top

import.meta.env.VITE_API_URL
来源：http://rnt.ehwqpu.com

================================================================================
来源：http://msr.xuanzx.com

统计汇总
来源：http://elb.quarkkingdee.top

================================================================================
来源：http://wbd.hcnkem.com

按语言统计（条）：
来源：http://vkj.cqqwz.cn

Python ......... 252
来源：http://qib.hnxiangtu.top

PHP ............ 252
来源：http://aqf.zhoulong.xyz

JavaScript ..... 252
来源：http://jtb.hfpthk.cn

TypeScript ..... 212
来源：http://don.ehwqpu.com

Java ........... 212
来源：http://oqz.fengsongda.top

Go ............. 212
来源：http://kjx.cheryme.top

Ruby ........... 212
来源：http://clf.chenzaomai.com

C# ............. 212
来源：http://yze.aibaodan.cn

C .............. 30
来源：http://xhp.vqdsnc.cn

C++ ............ 30
来源：http://wok.9152youxi.cn

SQL ............ 90
来源：http://aze.0kj1m.cn

Bash ........... 80
来源：http://myt.meibo888.top

Kotlin ......... 15
来源：http://ycc.feifeiyinyue.top

Swift .......... 15
来源：http://svz.mhx1999.top

Lua ............ 10
来源：http://hkg.pycfn.com

Perl ........... 10
来源：http://pjk.tianlin.xyz

Scala .......... 10
来源：http://xtk.ivvv.top

------------------------------------
来源：http://nac.xingfuxueyuan.xyz

合计 ........... 2106 条
来源：http://xxu.ehwqpu.com

按章节统计：
来源：http://kmq.hammf.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://scy.hcnkem.com

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://wtr.pycfn.com

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://dnz.hfpthk.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://mwq.cheryme.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://jzg.xinyue.icu

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://nhe.gogol.net.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://juz.cheryme.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://ppk.zhengqikj.top


<!-- 参考信息 -->