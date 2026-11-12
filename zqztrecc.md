代发 wailian999

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://kfn.dashuyun.cn

================================================================================
来源：http://ckb.jqgfzy.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hpa.vqdsnc.cn

================================================================================
来源：http://hdn.redwolf501.top

[U01] Py：创建虚拟环境
来源：http://iam.jlsjyb.cn

python -m venv .venv && source .venv/bin/activate
来源：http://aav.gogol.net.cn

[U02] Py：导出 / 安装依赖
来源：http://mqk.fanxiaobao.xyz

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://bzd.yj20258.top

[U03] Py：加载 .env 配置
来源：http://wkl.ppjwa.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://iev.havefunace.top

[U04] Py：变量调试打印
来源：http://ssy.zdqjudy.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://zho.hnxiangtu.top

[U05] Py：列表去重且保序
来源：http://wxs.yvedp.cn

list(dict.fromkeys(arr))
来源：http://kcf.tian-w.cn

[U06] Py：合并两个字典
来源：http://yih.gogol.net.cn

{**a, **b}
来源：http://mxn.sysykeji.top

[U07] Py：反转字典键值
来源：http://lgq.dianchejie.cn

{v: k for k, v in d.items()}
来源：http://nzl.xziqi.cn

[U08] Py：展平二维列表
来源：http://qaf.cdnleiting.top

[y for x in nested for y in x]
来源：http://sfp.yj20258888.top

[U09] Py：字典取最大值的键
来源：http://lnw.fzhhl.top

max(d, key=d.get)
来源：http://ing.jqgufenzy.top

[U10] Py：按值排序字典
来源：http://kpf.jqgufenzy.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://iet.jyoumei.cn

[U11] Py：生成器表达式
来源：http://wld.feifeiyinyue.top

(x * 2 for x in arr)
来源：http://fqb.meibo888.top

[U12] Py：取出现最多的 3 个元素
来源：http://yfs.sweek.top

Counter(arr).most_common(3)
来源：http://yle.zhiwuduotai.top

[U13] Py：固定长度队列
来源：http://fuv.wangdashe.top

deque(maxlen=10)
来源：http://mpa.redwolf501.top

[U14] Py：分组收集到列表
来源：http://iol.zycfv.cn

defaultdict(list)
来源：http://dyu.jianghu66.top

[U15] Py：高精度计时
来源：http://lfd.zdqjudy.top

t = time.perf_counter()
来源：http://zsf.jinqigfzy.top

[U16] Py：命令行参数解析
来源：http://sqz.hesvh.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://yef.shuidangran.top

[U17] Py：初始化日志
来源：http://gyc.fehbvm.com

logging.basicConfig(level=logging.INFO)
来源：http://lxj.c1oappe.top

[U18] Py：预编译正则
来源：http://jma.havefunace.top

pat = re.compile(r"\d+")
来源：http://jvx.daria6918.cn

[U19] Py：正则替换带回调
来源：http://exe.daxiang520.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://qgd.c1oappe.top

[U20] Py：缓存函数结果
来源：http://ago.cashguo.top

@functools.lru_cache(maxsize=None)
来源：http://szr.shzxlz.cn

[U21] Py：自定义上下文管理器
来源：http://mwq.aibaodan.cn

@contextlib.contextmanager
来源：http://ypx.zhengqikj.top

[U22] Py：矩阵转置
来源：http://jhm.tianlin.xyz

list(zip(*m))
来源：http://bdy.316326.xyz

[U23] Py：分块读取大文件
来源：http://vps.hysaishi.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://juc.yvedp.cn

[U24] Py：路径操作
来源：http://fuy.hammf.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://nxc.daria6918.cn

[U25] Py：CSV 按字典读
来源：http://qew.tianlin.xyz

csv.DictReader(f)
来源：http://tqz.iojbl.cn

[U26] Py：并发下载
来源：http://pgo.kuanghao11.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://gyp.bbcook.cn

[U27] Py：异步 HTTP
来源：http://zkb.hcnkem.com

aiohttp.ClientSession() 配合 async with
来源：http://sap.shzxlz.cn

[U28] Py：类型别名
来源：http://zxa.yangfankeji.com

UserId = int
来源：http://ptr.cdnleiting.top

[U29] Py：属性校验
来源：http://sfl.guannengcc.top

@property 与 @x.setter 配合
来源：http://eyj.daria6918.cn

[U30] Py：数据类
来源：http://qim.chenjidiqi.icu

@dataclass(slots=True)
来源：http://svc.shangyingyoupin.top

[U31] Py：单测
来源：http://vbx.hfpthk.cn

python -m pytest -q
来源：http://lea.yonumen.top

[U32] Py：代码格式化
来源：http://wur.gogol.net.cn

ruff format . && ruff check --fix .
来源：http://tuy.uphjek.com

[U33] Py：打包发布
来源：http://ytb.shangyingyoupin.top

python -m build  （依赖 pyproject.toml）
来源：http://eku.jianghu66.top

[U34] Py：判断编码
来源：http://acz.gotoacloud.top

chardet.detect(raw)
来源：http://njd.gzhubu.top

[U35] Py：发送邮件
来源：http://ayo.vehdjk.com

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://sxd.shanyushiyangtech.top

[U36] Py：定时任务
来源：http://xxm.jqgfzy.top

schedule.every(10).minutes.do(job)
来源：http://psp.chenjidiqi.icu

[U37] Py：读写 Excel
来源：http://cao.mhx1999.top

pandas.read_excel / DataFrame.to_excel
来源：http://hpc.nanxinkj.top

[U38] Py：获取脚本所在目录
来源：http://ryk.quarkkingdee.top

Path(__file__).resolve().parent
来源：http://cvi.pycfn.com

[U39] Py：判断是否在交互环境
来源：http://lcy.aizwys.cn

sys.stdout.isatty()
来源：http://bnb.fanxiaobao.xyz

[U40] Py：打印到标准错误
来源：http://ngg.zhongyouzk.top

print("err", file=sys.stderr)
来源：http://oiz.uphjek.com

[U41] PHP：初始化 Composer 项目
来源：http://voj.chenzaomai.com

composer init;  composer require guzzlehttp/guzzle
来源：http://qcu.bbcook.cn

[U42] PHP：PSR-4 自动加载
来源：http://yij.hammf.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://qis.sweek.top

[U43] PHP：声明命名空间
来源：http://rnp.hywenlv.cn

namespace App\Http;
来源：http://oub.jinghuilouyu.cn

[U44] PHP：开启严格类型
来源：http://tlk.zdqjudy.top

declare(strict_types=1);
来源：http://psy.jlsjyb.cn

[U45] PHP：类型声明与返回类型
来源：http://kqe.tianlin.xyz

function add(int $a, int $b): int { return $a + $b; }
来源：http://vob.shanyushiyangtech.top

[U46] PHP：可空类型
来源：http://fve.fengsongda.top

?string $name = null
来源：http://auw.ywan-chungtsiang.top

[U47] PHP：联合类型
来源：http://jbf.tianlin.xyz

int|string $id
来源：http://dkb.jlsjyb.cn

[U48] PHP：纯枚举
来源：http://otl.gotoacloud.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://wys.jinqigufen.top

[U49] PHP：只读属性
来源：http://xev.yj202588.top

public readonly string $name
来源：http://mnc.yfazqb.com

[U50] PHP：构造器属性提升
来源：http://umg.guowangkeji.top

public function __construct(private int $id) {}
来源：http://pvd.nanxinkj.top

[U51] PHP：数组解构
来源：http://enm.jinqigufen.top

[$a, $b] = $arr;
来源：http://hsp.xylfe.cn

[U52] PHP：箭头函数
来源：http://pwp.zhaomingkeji.xyz

$double = fn($x) => $x * 2;
来源：http://mnn.wangdashe.top

[U53] PHP：空合并运算符
来源：http://nur.sxryk.cn

$v = $a ?? $b ?? "default";
来源：http://xcl.tanke756.top

[U54] PHP：空安全调用
来源：http://tid.jlsjyb.cn

$obj?->method()
来源：http://tsu.yj202588.top

[U55] PHP：match 表达式
来源：http://xnb.jyoumei.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://qjo.jqgfzy.top

[U56] PHP：命名参数
来源：http://whe.yj20258.top

f(a: 1, b: 2)
来源：http://xuz.epnwcf.com

[U57] PHP：字符串插值
来源：http://laj.ctjpmb.com

"值: {$a}"
来源：http://rsn.jyoumei.cn

[U58] PHP：数组三件套
来源：http://vql.shanyushiyangtech.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://rsj.yuxming.cn

[U59] PHP：自定义排序
来源：http://xap.zhijiandao.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://vwe.dashuyun.cn

[U60] PHP：JSON 编解码
来源：http://mnt.quarkkingdee.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://eij.jinqigufen.top

[U61] PHP：正则
来源：http://wsh.zdbjq.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://ywa.52xcode.cn

[U62] PHP：日期对象
来源：http://abt.sjlbkw.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hwq.redwolf501.top

[U63] PHP：文件读写
来源：http://mnr.havefunace.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://ftu.jqgufenzy.top

[U64] PHP：目录遍历
来源：http://jqx.ivvv.top

glob("dir/*.php");  scandir("dir");
来源：http://mrg.shangyingyoupin.top

[U65] PHP：会话
来源：http://hjk.xuanzx.com

session_start();  $_SESSION["uid"] = 1;
来源：http://bro.cheryme.top

[U66] PHP：设置 Cookie
来源：http://alm.hammf.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://nsd.sxryk.cn

[U67] PHP：处理文件上传
来源：http://mti.redwolf501.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://hga.gogol.net.cn

[U68] PHP：PDO 连接
来源：http://dap.ydzc1.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://xkm.sysykeji.top

[U69] PHP：PDO 预处理
来源：http://vzf.yj20258.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://gkh.hysaishi.cn

[U70] PHP：PDO 事务
来源：http://dpf.yj202588.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://exs.jyoumei.cn

[U71] PHP：抛出异常
来源：http://fff.yj20258.top

throw new RuntimeException("失败", 500);
来源：http://agu.tarul.cn

[U72] PHP：写错误日志
来源：http://csv.dianchejie.cn

error_log("失败: " . $e->getMessage());
来源：http://gpe.jinqigfzy.top

[U73] PHP：读取 ini 配置
来源：http://syh.shanyushiyangkeji.top

parse_ini_file("config.ini", true)
来源：http://fbn.xingfuxueyuan.xyz

[U74] PHP：读取环境变量
来源：http://dxb.zdbjq.cn

getenv("APP_ENV") ?: "production"
来源：http://lfy.pycfn.com

[U75] PHP：依赖注入
来源：http://jnb.hnqzz.top

composer require psr/container
来源：http://fof.jyoumei.cn

[U76] PHP：简单路由
来源：http://xaw.sjlbkw.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://umx.zdqjudy.top

[U77] PHP：模板渲染
来源：http://gnt.jlsjyb.cn

composer require twig/twig
来源：http://kmv.jinqigufen.top

[U78] PHP：单元测试
来源：http://zgz.yfazqb.com

composer require --dev phpunit/phpunit
来源：http://oos.zycfv.cn

[U79] PHP：静态分析
来源：http://npq.cashguo.top

composer require --dev phpstan/phpstan
来源：http://dqe.chenzaomai.com

[U80] PHP：代码规范修复
来源：http://lju.aibaodan.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://blh.zhiwuduotai.top

[U81] JS：初始化项目
来源：http://wqx.ppjwa.cn

npm init -y;  npm i express
来源：http://pwi.tarul.cn

[U82] JS：package.json 脚本
来源：http://dlw.0kj1m.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://dwz.zhongyouzk.top

[U83] JS：ES Module 导入导出
来源：http://afs.yongpay.top

export const a = 1;  import { a } from "./m.js";
来源：http://rbc.zdqjudy.top

[U84] JS：CommonJS 写法
来源：http://wsi.xuanzx.com

module.exports = { a };  const { a } = require("./m");
来源：http://zqp.fktsv.cn

[U85] JS：可选链
来源：http://iki.0kj1m.cn

a?.b?.c
来源：http://kgo.zdqjudy.top

[U86] JS：空值合并
来源：http://xje.kuanghao11.cn

a ?? b
来源：http://udx.hongshengwenyu.top

[U87] JS：解构默认值
来源：http://nhd.jinyuanbaomall.cn

const { a = 1, b = 2 } = obj;
来源：http://ioc.andypj.xyz

[U88] JS：对象展开合并
来源：http://hua.cdnleiting.top

{ ...a, ...b }
来源：http://dbt.hcnkem.com

[U89] JS：数组去重
来源：http://fwc.jiagoushi.top

[...new Set(arr)]
来源：http://tqx.hnqzz.top

[U90] JS：数字数组排序
来源：http://jis.jlsjyb.cn

[...arr].sort((a, b) => a - b)
来源：http://jdi.birdmap.top

[U91] JS：对象键值遍历
来源：http://bqk.ehwqpu.com

Object.entries(obj).forEach(([k, v]) => {});
来源：http://ymu.ppjwa.cn

[U92] JS：深拷贝
来源：http://shw.zhengqikj.top

structuredClone(obj)
来源：http://eqb.pycfn.com

[U93] JS：模板字符串
来源：http://vca.ctjpmb.com

`共 ${n} 条`
来源：http://iax.316326.xyz

[U94] JS：箭头函数
来源：http://myv.cheryme.top

const double = x => x * 2;
来源：http://ser.ybcxt.top

[U95] JS：Promise 包装
来源：http://ifg.wangshuangyany.cn

new Promise((resolve, reject) => {})
来源：http://efm.hysaishi.cn

[U96] JS：async/await 与异常
来源：http://gzz.hysaishi.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://wss.daxiang520.top

[U97] JS：并发请求
来源：http://wvd.kuanghao11.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://kxg.wangdashe.top

[U98] JS：fetch 带 JSON
来源：http://yty.yueranfly.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://yaj.yangfankeji.com

[U99] JS：事件监听
来源：http://ats.jiagoushi.top

el.addEventListener("click", e => {})
来源：http://aph.ctjpmb.com

[U100] JS：DOM 查询
来源：http://hif.redwolf501.top

document.querySelector(".item")
来源：http://yjh.zycfv.cn

[U101] JS：classList 操作
来源：http://whp.nanxinkj.top

el.classList.toggle("active")
来源：http://qcp.shangyingyoupin.top

[U102] JS：本地存储
来源：http://ell.jinghuilouyu.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://nlb.zhengqikj.top

[U103] JS：定时器
来源：http://tju.hfpthk.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://psy.aibaodan.cn

[U104] JS：防抖
来源：http://kax.aizwys.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://iea.yj202588.top

[U105] JS：节流
来源：http://pgb.tanke756.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://bvq.daxiang520.top

[U106] JS：日期格式化
来源：http://vwa.hnqzz.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://fup.ppjwa.cn

[U107] JS：数字千分位
来源：http://nlj.shuidangran.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://nbh.fzhhl.top

[U108] JS：随机整数
来源：http://ldf.haohaochexian.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://skm.ywan-chungtsiang.top

[U109] JS：数组分组
来源：http://bcv.feifeiyinyue.top

Object.groupBy(arr, x => x.type)
来源：http://ayr.jianghu66.top

[U110] JS：数组分块
来源：http://hsj.zhongyouzk.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://kei.cheryme.top

[U111] JS：对象转 Map
来源：http://uhi.fktsv.cn

new Map(Object.entries(obj))
来源：http://bed.pycfn.com

[U112] JS：字符串补位
来源：http://ddy.ehwqpu.com

"7".padStart(3, "0")
来源：http://rfu.xziqi.cn

[U113] JS：正则替换全部
来源：http://tbq.jianghu66.top

s.replaceAll("a", "b")
来源：http://szx.hcnkem.com

[U114] JS：JSON 深比较
来源：http://beg.snrcjt.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://nsw.sjlbkw.cn

[U115] JS：生成 UUID
来源：http://pai.jinyuanbaomall.cn

crypto.randomUUID()
来源：http://llf.quarkkingdee.top

[U116] JS：类型检查（JSDoc）
来源：http://bzc.fktsv.cn

/** @param {string} name */ function f(name) {}
来源：http://vmg.fktsv.cn

[U117] JS：单元测试
来源：http://xjz.jinqigufen.top

npm i -D vitest;  npx vitest
来源：http://tzg.birdmap.top

[U118] JS：开发服务器
来源：http://zzq.sweek.top

npm i -D vite;  npx vite
来源：http://vad.shanyushiyangkeji.top

[U119] JS：生产构建
来源：http://gup.xingfuxueyuan.xyz

npx vite build
来源：http://jxb.iojbl.cn

[U120] JS：读取环境变量（Vite）
来源：http://jrh.yj20258.top

import.meta.env.VITE_API_URL
来源：http://wgz.xuetiantiany.cn

================================================================================
来源：http://doc.xuetiantiany.cn

统计汇总
来源：http://rlj.hnqzz.top

================================================================================
来源：http://owu.tianlin.xyz

按语言统计（条）：
来源：http://pce.kuanghao11.cn

Python ......... 252
来源：http://hji.ywan-chungtsiang.top

PHP ............ 252
来源：http://ekp.jyoumei.cn

JavaScript ..... 252
来源：http://qal.yvedp.cn

TypeScript ..... 212
来源：http://cyj.zhijiandao.cn

Java ........... 212
来源：http://ohe.xylfe.cn

Go ............. 212
来源：http://dda.fehbvm.com

Ruby ........... 212
来源：http://upt.chenlongwang.top

C# ............. 212
来源：http://ttv.ybcxt.top

C .............. 30
来源：http://eac.ctjpmb.com

C++ ............ 30
来源：http://pqb.shangyingyoupin.top

SQL ............ 90
来源：http://psz.shangyingyoupin.top

Bash ........... 80
来源：http://mcx.hcnkem.com

Kotlin ......... 15
来源：http://qtp.uphjek.com

Swift .......... 15
来源：http://vrj.jqgfzy.top

Lua ............ 10
来源：http://cse.ivvv.top

Perl ........... 10
来源：http://okv.bjfxy.top

Scala .......... 10
来源：http://ycq.ivvv.top

------------------------------------
来源：http://wrp.yanxiufei.cn

合计 ........... 2106 条
来源：http://frm.feifeiyinyue.top

按章节统计：
来源：http://mbq.sweek.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hjx.jiagoushi.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://coo.nanxuanxn.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hod.zhengqikj.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://tli.yvedp.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://slv.gogol.net.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://plk.haohaochexian.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://jeg.hywenlv.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://pyl.sxryk.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://rkz.vehdjk.com

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://aql.zhengqikj.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://jmq.hammf.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://jof.chenjidiqi.icu

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://wit.yvedp.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://wzj.shuidangran.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://ozb.hfpthk.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://xfi.ctjpmb.com

Q SQL 专题                              90
来源：http://hze.jqgfzy.top

R Bash 专题                             80
来源：http://zyl.vehdjk.com

S C / C++ 专题                          60
来源：http://wdh.hcnkem.com

T 其他语言补充                          60
来源：http://wbc.shzxlz.cn

U 高频实用片段                         120
来源：http://lba.zhijiandao.cn

------------------------------------
来源：http://yzx.zhijiandao.cn

合计                                  2106 条
来源：http://hsq.fanxiaobao.xyz

--------------------------------------------------------------------------------
来源：http://gfq.hammf.cn

使用提醒
来源：http://vqf.wangdashe.top

--------------------------------------------------------------------------------
来源：http://bpc.gaohongyu789.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://dlw.sjlbkw.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://zab.havefunace.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://mtz.fehbvm.com

在旧版本上使用前请先确认语法支持情况。
来源：http://xen.yuxming.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://pve.zhijiandao.cn

—— 文件结束 ——
来源：http://yhj.pengpengdd.cyou


<!-- 参考信息 -->