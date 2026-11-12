代发 wailian999

val a = 1;  var b = 2
来源：http://qts.zhengqikj.top

[T53] Scala：字符串插值
来源：http://wzm.birdmap.top

s"值: $b"
来源：http://wmp.zdqjudy.top

[T54] Scala：集合映射
来源：http://tct.jiagoushi.top

List(1, 2, 3).map(_ * 2)
来源：http://nrv.shzxlz.cn

[T55] Scala：集合过滤
来源：http://wxx.haohaochexian.top

List(1, 2, 3).filter(_ > 1)
来源：http://lmv.nwbrower.top

[T56] Scala：样例类
来源：http://lnu.fengsongda.top

case class User(name: String, age: Int)
来源：http://vyv.zhijiandao.cn

[T57] Scala：模式匹配
来源：http://wks.kuanghao11.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://scc.feifeiyinyue.top

[T58] Scala：函数定义
来源：http://xie.bbcook.cn

def add(a: Int, b: Int): Int = a + b
来源：http://ikw.zdqjudy.top

[T59] Scala：循环
来源：http://vsg.vqdsnc.cn

for (i <- 1 to 10) println(i)
来源：http://awu.fktsv.cn

[T60] Scala：折叠
来源：http://ekb.gogol.net.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://esu.zhoulong.xyz

================================================================================
来源：http://swb.zhixingplan.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://zra.tian-w.cn

================================================================================
来源：http://xqe.hysaishi.cn

[U01] Py：创建虚拟环境
来源：http://odi.zhijiandao.cn

python -m venv .venv && source .venv/bin/activate
来源：http://avq.sufxvd.cn

[U02] Py：导出 / 安装依赖
来源：http://mxv.havefunace.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://oeb.yj20258888.top

[U03] Py：加载 .env 配置
来源：http://kpx.tanke756.top

from dotenv import load_dotenv; load_dotenv()
来源：http://bnl.sufxvd.cn

[U04] Py：变量调试打印
来源：http://dza.hammf.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://ziu.iojbl.cn

[U05] Py：列表去重且保序
来源：http://keh.hnxiangtu.top

list(dict.fromkeys(arr))
来源：http://kfw.haohaochexian.top

[U06] Py：合并两个字典
来源：http://zjm.zycfv.cn

{**a, **b}
来源：http://qrl.hfpthk.cn

[U07] Py：反转字典键值
来源：http://vfr.xingfuxueyuan.xyz

{v: k for k, v in d.items()}
来源：http://kwz.sjlbkw.cn

[U08] Py：展平二维列表
来源：http://mli.nanxinkj.top

[y for x in nested for y in x]
来源：http://chh.sxryk.cn

[U09] Py：字典取最大值的键
来源：http://izm.xinyue.icu

max(d, key=d.get)
来源：http://vsv.ybcxt.top

[U10] Py：按值排序字典
来源：http://ybp.hcnkem.com

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://kxb.aibaodan.cn

[U11] Py：生成器表达式
来源：http://zch.sufxvd.cn

(x * 2 for x in arr)
来源：http://wax.zdqjudy.top

[U12] Py：取出现最多的 3 个元素
来源：http://utv.xziqi.cn

Counter(arr).most_common(3)
来源：http://vrh.tanke756.top

[U13] Py：固定长度队列
来源：http://tkg.dianchejie.cn

deque(maxlen=10)
来源：http://kiq.svipenyu.cn

[U14] Py：分组收集到列表
来源：http://mjv.mhx1999.top

defaultdict(list)
来源：http://uoa.c1oappe.top

[U15] Py：高精度计时
来源：http://rkk.cheryme.top

t = time.perf_counter()
来源：http://lkm.redwolf501.top

[U16] Py：命令行参数解析
来源：http://wkx.pycfn.com

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://wpm.tian-w.cn

[U17] Py：初始化日志
来源：http://yej.fktsv.cn

logging.basicConfig(level=logging.INFO)
来源：http://owt.hesvh.cn

[U18] Py：预编译正则
来源：http://bcu.xziqi.cn

pat = re.compile(r"\d+")
来源：http://twh.xylfe.cn

[U19] Py：正则替换带回调
来源：http://tnl.wangshuangyany.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://xdl.hcnkem.com

[U20] Py：缓存函数结果
来源：http://nlu.zhoulong.xyz

@functools.lru_cache(maxsize=None)
来源：http://yoi.yongpay.top

[U21] Py：自定义上下文管理器
来源：http://fat.sjlbkw.cn

@contextlib.contextmanager
来源：http://qkm.cqqwz.cn

[U22] Py：矩阵转置
来源：http://auk.nanxuanxn.top

list(zip(*m))
来源：http://ptu.andypj.xyz

[U23] Py：分块读取大文件
来源：http://hce.jinghuilouyu.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://bzt.chenlongwang.top

[U24] Py：路径操作
来源：http://yzo.meibo888.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://wys.yj20258888.top

[U25] Py：CSV 按字典读
来源：http://sqj.cucudq.cn

csv.DictReader(f)
来源：http://orc.yonumen.top

[U26] Py：并发下载
来源：http://ozg.gotoacloud.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://voq.yuxming.cn

[U27] Py：异步 HTTP
来源：http://zjp.zdbjq.cn

aiohttp.ClientSession() 配合 async with
来源：http://tlw.tanke756.top

[U28] Py：类型别名
来源：http://ljg.zhiwuduotai.top

UserId = int
来源：http://ntn.nwbrower.top

[U29] Py：属性校验
来源：http://xbg.zhongyouzk.top

@property 与 @x.setter 配合
来源：http://ddp.zhengqikj.top

[U30] Py：数据类
来源：http://cre.fanxiaobao.xyz

@dataclass(slots=True)
来源：http://wrg.shangyingyoupin.top

[U31] Py：单测
来源：http://gvj.quarkkingdee.top

python -m pytest -q
来源：http://qws.yangfankeji.com

[U32] Py：代码格式化
来源：http://yzk.havefunace.top

ruff format . && ruff check --fix .
来源：http://jib.ydjk.org.cn

[U33] Py：打包发布
来源：http://ohv.52xcode.cn

python -m build  （依赖 pyproject.toml）
来源：http://rmk.cqqwz.cn

[U34] Py：判断编码
来源：http://fvy.yvedp.cn

chardet.detect(raw)
来源：http://deb.shangyingyoupin.top

[U35] Py：发送邮件
来源：http://psb.chenlongwang.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://pjh.316326.xyz

[U36] Py：定时任务
来源：http://weo.hnxiangtu.top

schedule.every(10).minutes.do(job)
来源：http://dly.yj20258888.top

[U37] Py：读写 Excel
来源：http://syb.hcnkem.com

pandas.read_excel / DataFrame.to_excel
来源：http://wca.yuanzhike.top

[U38] Py：获取脚本所在目录
来源：http://hcb.fengsongda.top

Path(__file__).resolve().parent
来源：http://vrl.uphjek.com

[U39] Py：判断是否在交互环境
来源：http://ruu.meibo888.top

sys.stdout.isatty()
来源：http://fbb.jinqigufen.top

[U40] Py：打印到标准错误
来源：http://aev.zhixingplan.top

print("err", file=sys.stderr)
来源：http://aky.sweek.top

[U41] PHP：初始化 Composer 项目
来源：http://tmz.fehbvm.com

composer init;  composer require guzzlehttp/guzzle
来源：http://pxp.fehbvm.com

[U42] PHP：PSR-4 自动加载
来源：http://zlp.zdbjq.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://doq.wangshuangyany.cn

[U43] PHP：声明命名空间
来源：http://kun.hcnkem.com

namespace App\Http;
来源：http://bqx.xylfe.cn

[U44] PHP：开启严格类型
来源：http://xlh.wangshuangyany.cn

declare(strict_types=1);
来源：http://prv.ctjpmb.com

[U45] PHP：类型声明与返回类型
来源：http://goh.epnwcf.com

function add(int $a, int $b): int { return $a + $b; }
来源：http://cuo.aibaodan.cn

[U46] PHP：可空类型
来源：http://ugo.zdqjudy.top

?string $name = null
来源：http://dwf.ydzc1.top

[U47] PHP：联合类型
来源：http://udh.xylfe.cn

int|string $id
来源：http://uel.ctjpmb.com

[U48] PHP：纯枚举
来源：http://evk.jqgufenzy.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://gyh.gaohongyu789.top

[U49] PHP：只读属性
来源：http://xjq.fanxiaobao.xyz

public readonly string $name
来源：http://sbe.sysykeji.top

[U50] PHP：构造器属性提升
来源：http://evn.hysaishi.cn

public function __construct(private int $id) {}
来源：http://edw.52xcode.cn

[U51] PHP：数组解构
来源：http://eff.ivvv.top

[$a, $b] = $arr;
来源：http://ysv.yuxming.cn

[U52] PHP：箭头函数
来源：http://neb.shanyushiyangkeji.top

$double = fn($x) => $x * 2;
来源：http://tyh.zhijiandao.cn

[U53] PHP：空合并运算符
来源：http://iby.sysykeji.top

$v = $a ?? $b ?? "default";
来源：http://swe.52xcode.cn

[U54] PHP：空安全调用
来源：http://grh.yanxiufei.cn

$obj?->method()
来源：http://lij.fanxiaobao.xyz

[U55] PHP：match 表达式
来源：http://jby.zhaomingkeji.xyz

$s = match($x) { 1 => "一", default => "其他" };
来源：http://gtp.svipenyu.cn

[U56] PHP：命名参数
来源：http://nfc.jlsjyb.cn

f(a: 1, b: 2)
来源：http://ezs.cucudq.cn

[U57] PHP：字符串插值
来源：http://wtc.yongpay.top

"值: {$a}"
来源：http://vyk.feifeiyinyue.top

[U58] PHP：数组三件套
来源：http://fiw.havefunace.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://nhc.smart0.xyz

[U59] PHP：自定义排序
来源：http://yuw.gaohongyu789.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://olp.daxiang520.top

[U60] PHP：JSON 编解码
来源：http://ouo.zhoulong.xyz

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://jnw.zhongyouzk.top

[U61] PHP：正则
来源：http://lnc.zdqjudy.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://zje.zhijiandao.cn

[U62] PHP：日期对象
来源：http://dex.fanxiaobao.xyz

(new DateTimeImmutable())->format("Y-m-d");
来源：http://zuv.yj20258.top

[U63] PHP：文件读写
来源：http://cxb.uphjek.com

file_get_contents($f);  file_put_contents($f, $data);
来源：http://tfh.sufxvd.cn

[U64] PHP：目录遍历
来源：http://yqx.hfpthk.cn

glob("dir/*.php");  scandir("dir");
来源：http://dto.epnwcf.com

[U65] PHP：会话
来源：http://czs.xinyue.icu

session_start();  $_SESSION["uid"] = 1;
来源：http://gkz.jqgufenzy.top

[U66] PHP：设置 Cookie
来源：http://fjp.redwolf501.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://cxk.fktsv.cn

[U67] PHP：处理文件上传
来源：http://eco.kuanghao11.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://dbd.ydjk.org.cn

[U68] PHP：PDO 连接
来源：http://ksn.yj20258888.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://trr.zdqjudy.top

[U69] PHP：PDO 预处理
来源：http://qap.xuanzx.com

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hlr.aibaodan.cn

[U70] PHP：PDO 事务
来源：http://pbq.hammf.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://ebz.ybcxt.top

[U71] PHP：抛出异常
来源：http://hpy.tarul.cn

throw new RuntimeException("失败", 500);
来源：http://ako.tanke756.top

[U72] PHP：写错误日志
来源：http://miq.jinqigufen.top

error_log("失败: " . $e->getMessage());
来源：http://ynz.iojbl.cn

[U73] PHP：读取 ini 配置
来源：http://zkc.chenjidiqi.icu

parse_ini_file("config.ini", true)
来源：http://txe.yj20258888.top

[U74] PHP：读取环境变量
来源：http://haj.feifeiyinyue.top

getenv("APP_ENV") ?: "production"
来源：http://ady.tianlin.xyz

[U75] PHP：依赖注入
来源：http://rns.snrcjt.cn

composer require psr/container
来源：http://xrg.jinyuanbaomall.cn

[U76] PHP：简单路由
来源：http://huc.gogol.net.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://qgq.zhongyouzk.top

[U77] PHP：模板渲染
来源：http://ltm.hongshengwenyu.top

composer require twig/twig
来源：http://hks.yuxming.cn

[U78] PHP：单元测试
来源：http://qlf.yj20258888.top

composer require --dev phpunit/phpunit
来源：http://kjj.52xcode.cn

[U79] PHP：静态分析
来源：http://afk.jiagoushi.top

composer require --dev phpstan/phpstan
来源：http://lox.feifeiyinyue.top

[U80] PHP：代码规范修复
来源：http://hot.smart0.xyz

composer require --dev friendsofphp/php-cs-fixer
来源：http://qur.uphjek.com

[U81] JS：初始化项目
来源：http://ebr.sxryk.cn

npm init -y;  npm i express
来源：http://ldl.feifeiyinyue.top

[U82] JS：package.json 脚本
来源：http://dpf.bbcook.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://jxi.jqgfzy.top

[U83] JS：ES Module 导入导出
来源：http://xvs.daxiang520.top

export const a = 1;  import { a } from "./m.js";
来源：http://rlp.yonumen.top

[U84] JS：CommonJS 写法
来源：http://qql.fehbvm.com

module.exports = { a };  const { a } = require("./m");
来源：http://nyp.fanxiaobao.xyz

[U85] JS：可选链
来源：http://piu.aizwys.cn

a?.b?.c
来源：http://shq.yongpay.top

[U86] JS：空值合并
来源：http://rzn.hnqzz.top

a ?? b
来源：http://fzw.dashuyun.cn

[U87] JS：解构默认值
来源：http://fko.sweek.top

const { a = 1, b = 2 } = obj;
来源：http://uqj.cashguo.top

[U88] JS：对象展开合并
来源：http://tzp.haohaochexian.top

{ ...a, ...b }
来源：http://wrl.shanyushiyangkeji.top

[U89] JS：数组去重
来源：http://ikh.fanxiaobao.xyz

[...new Set(arr)]
来源：http://vrj.yueranfly.top

[U90] JS：数字数组排序
来源：http://abu.chenzaomai.com

[...arr].sort((a, b) => a - b)
来源：http://rza.hammf.cn

[U91] JS：对象键值遍历
来源：http://iko.chenzaomai.com

Object.entries(obj).forEach(([k, v]) => {});
来源：http://eum.ydjk.org.cn

[U92] JS：深拷贝
来源：http://cer.tianlin.xyz

structuredClone(obj)
来源：http://ong.ywan-chungtsiang.top

[U93] JS：模板字符串
来源：http://khe.cdnleiting.top

`共 ${n} 条`
来源：http://lce.aizwys.cn

[U94] JS：箭头函数
来源：http://sks.zhoulong.xyz

const double = x => x * 2;
来源：http://srm.fehbvm.com

[U95] JS：Promise 包装
来源：http://cwi.aibaodan.cn

new Promise((resolve, reject) => {})
来源：http://vra.shanyushiyangkeji.top

[U96] JS：async/await 与异常
来源：http://red.nwbrower.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://ybj.zhaomingkeji.xyz

[U97] JS：并发请求
来源：http://ica.jiagoushi.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://zvw.jyoumei.cn

[U98] JS：fetch 带 JSON
来源：http://eyr.sxryk.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://jeh.cdnleiting.top

[U99] JS：事件监听
来源：http://bmc.ydzc1.top

el.addEventListener("click", e => {})
来源：http://icl.gzhubu.top

[U100] JS：DOM 查询
来源：http://lyz.mhx1999.top

document.querySelector(".item")
来源：http://zyq.snrcjt.cn

[U101] JS：classList 操作
来源：http://iuz.hcnkem.com

el.classList.toggle("active")
来源：http://cya.ybcxt.top

[U102] JS：本地存储
来源：http://tki.jiagoushi.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://qzt.gogol.net.cn

[U103] JS：定时器
来源：http://bdw.shanyushiyangkeji.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://apo.meibo888.top

[U104] JS：防抖
来源：http://mvv.sufxvd.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://vbg.yfazqb.com

[U105] JS：节流
来源：http://rkd.xziqi.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://qoa.yonumen.top

[U106] JS：日期格式化
来源：http://adx.tian-w.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://ury.ctjpmb.com

[U107] JS：数字千分位
来源：http://dfy.shanyushiyangtech.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://pwn.hysaishi.cn

[U108] JS：随机整数
来源：http://ifg.iojbl.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://att.yueranfly.top

[U109] JS：数组分组
来源：http://coc.shangyingyoupin.top

Object.groupBy(arr, x => x.type)
来源：http://oes.kuanghao11.cn

[U110] JS：数组分块
来源：http://oca.yuxming.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://epu.zhengqikj.top

[U111] JS：对象转 Map
来源：http://zjy.hywenlv.cn

new Map(Object.entries(obj))
来源：http://nie.tianlin.xyz

[U112] JS：字符串补位
来源：http://wjw.yuxming.cn

"7".padStart(3, "0")
来源：http://gwh.redwolf501.top

[U113] JS：正则替换全部
来源：http://hih.sjlbkw.cn

s.replaceAll("a", "b")
来源：http://teo.svipenyu.cn

[U114] JS：JSON 深比较
来源：http://qiw.meibo888.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://ouo.gotoacloud.top

[U115] JS：生成 UUID
来源：http://dyn.sxryk.cn

crypto.randomUUID()
来源：http://uik.zdbjq.cn

[U116] JS：类型检查（JSDoc）
来源：http://hjo.zhoulong.xyz

/** @param {string} name */ function f(name) {}
来源：http://ves.cheryme.top

[U117] JS：单元测试
来源：http://slr.jinqigfzy.top

npm i -D vitest;  npx vitest
来源：http://sfq.wangshuangyany.cn

[U118] JS：开发服务器
来源：http://cqb.tian-w.cn

npm i -D vite;  npx vite
来源：http://feo.shanyushiyangkeji.top

[U119] JS：生产构建
来源：http://fdm.guannengcc.top

npx vite build
来源：http://xhv.feifeiyinyue.top

[U120] JS：读取环境变量（Vite）
来源：http://tcb.jinghuilouyu.cn

import.meta.env.VITE_API_URL
来源：http://aaw.vqdsnc.cn

================================================================================
来源：http://kjb.zdbjq.cn

统计汇总
来源：http://ota.jlsjyb.cn

================================================================================
来源：http://yhg.zhoulong.xyz

按语言统计（条）：
来源：http://bse.vehdjk.com

Python ......... 252
来源：http://fqo.xingfuxueyuan.xyz

PHP ............ 252
来源：http://huc.ywan-chungtsiang.top

JavaScript ..... 252
来源：http://dnn.0kj1m.cn

TypeScript ..... 212
来源：http://jbj.ybcxt.top

Java ........... 212
来源：http://dlu.cashguo.top

Go ............. 212
来源：http://zhk.pengpengdd.cyou

Ruby ........... 212
来源：http://ouc.xingfuxueyuan.xyz

C# ............. 212
来源：http://gsi.fengsongda.top

C .............. 30
来源：http://nwl.hnxiangtu.top

C++ ............ 30
来源：http://bij.fzhhl.top

SQL ............ 90
来源：http://xuo.xziqi.cn

Bash ........... 80
来源：http://qtk.yuanzhike.top

Kotlin ......... 15
来源：http://nja.hongshengwenyu.top

Swift .......... 15
来源：http://dvx.tianlin.xyz

Lua ............ 10
来源：http://apk.yfazqb.com

Perl ........... 10
来源：http://ghk.hammf.cn

Scala .......... 10
来源：http://efe.yuxming.cn

------------------------------------
来源：http://xrh.uphjek.com

合计 ........... 2106 条
来源：http://cte.hnxiangtu.top

按章节统计：
来源：http://tjb.yuanzhike.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://zvh.jinqigufen.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://dcn.zdqjudy.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://rpu.chenzaomai.com

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://yib.nanxinkj.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://qds.dashuyun.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://xuz.nanxuanxn.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://pwk.snrcjt.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://kdz.yonumen.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://yni.shangyingyoupin.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://zra.jinghuilouyu.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://nlu.xziqi.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://yha.hysaishi.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://pdn.uphjek.com

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://tvq.tian-w.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://kxm.9152youxi.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://mws.jlsjyb.cn


<!-- 参考信息 -->