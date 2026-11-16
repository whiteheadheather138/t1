代发 wailian999

[U03] Py：加载 .env 配置
来源：http://pqs.jiagoushi.top

from dotenv import load_dotenv; load_dotenv()
来源：http://ccy.xziqi.cn

[U04] Py：变量调试打印
来源：http://ogm.hnqzz.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://qus.snrcjt.cn

[U05] Py：列表去重且保序
来源：http://tse.zhoulong.xyz

list(dict.fromkeys(arr))
来源：http://gcp.tian-w.cn

[U06] Py：合并两个字典
来源：http://pcd.sxryk.cn

{**a, **b}
来源：http://mfs.dianchejie.cn

[U07] Py：反转字典键值
来源：http://mpu.jinqigufen.top

{v: k for k, v in d.items()}
来源：http://dad.xylfe.cn

[U08] Py：展平二维列表
来源：http://rse.yvedp.cn

[y for x in nested for y in x]
来源：http://ihf.fanxiaobao.xyz

[U09] Py：字典取最大值的键
来源：http://rtr.gogol.net.cn

max(d, key=d.get)
来源：http://idn.c1oappe.top

[U10] Py：按值排序字典
来源：http://xaf.chenzaomai.com

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://pof.chenlongwang.top

[U11] Py：生成器表达式
来源：http://zuq.jinghuilouyu.cn

(x * 2 for x in arr)
来源：http://bbk.cqqwz.cn

[U12] Py：取出现最多的 3 个元素
来源：http://ubq.hammf.cn

Counter(arr).most_common(3)
来源：http://far.zhixingplan.top

[U13] Py：固定长度队列
来源：http://ydh.uphjek.com

deque(maxlen=10)
来源：http://gam.zycfv.cn

[U14] Py：分组收集到列表
来源：http://aou.dashuyun.cn

defaultdict(list)
来源：http://xqe.ydzc1.top

[U15] Py：高精度计时
来源：http://mkg.gzhubu.top

t = time.perf_counter()
来源：http://inn.fzhhl.top

[U16] Py：命令行参数解析
来源：http://fge.shangyingyoupin.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://fgz.zhiwuduotai.top

[U17] Py：初始化日志
来源：http://jkr.vehdjk.com

logging.basicConfig(level=logging.INFO)
来源：http://onp.aibaodan.cn

[U18] Py：预编译正则
来源：http://ajb.zhoulong.xyz

pat = re.compile(r"\d+")
来源：http://fds.gotoacloud.top

[U19] Py：正则替换带回调
来源：http://duu.smart0.xyz

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://bjd.ywan-chungtsiang.top

[U20] Py：缓存函数结果
来源：http://qqt.tian-w.cn

@functools.lru_cache(maxsize=None)
来源：http://nga.cheryme.top

[U21] Py：自定义上下文管理器
来源：http://pvr.cashguo.top

@contextlib.contextmanager
来源：http://dap.pycfn.com

[U22] Py：矩阵转置
来源：http://epv.ivvv.top

list(zip(*m))
来源：http://glr.mhx1999.top

[U23] Py：分块读取大文件
来源：http://izs.zdqjudy.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://nkv.jqgfzy.top

[U24] Py：路径操作
来源：http://kfa.cheryme.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://lpb.zycfv.cn

[U25] Py：CSV 按字典读
来源：http://yqo.mhx1999.top

csv.DictReader(f)
来源：http://xwb.wangdashe.top

[U26] Py：并发下载
来源：http://kfh.mhx1999.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://zsv.zycfv.cn

[U27] Py：异步 HTTP
来源：http://gbc.jlsjyb.cn

aiohttp.ClientSession() 配合 async with
来源：http://lpw.zhengqikj.top

[U28] Py：类型别名
来源：http://tba.ywan-chungtsiang.top

UserId = int
来源：http://eze.cheryme.top

[U29] Py：属性校验
来源：http://ivu.zhengqikj.top

@property 与 @x.setter 配合
来源：http://hxt.svipenyu.cn

[U30] Py：数据类
来源：http://axt.jianghu66.top

@dataclass(slots=True)
来源：http://bjq.fzhhl.top

[U31] Py：单测
来源：http://vkh.hysaishi.cn

python -m pytest -q
来源：http://xuv.chenlongwang.top

[U32] Py：代码格式化
来源：http://xcs.yanxiufei.cn

ruff format . && ruff check --fix .
来源：http://bre.zhongyouzk.top

[U33] Py：打包发布
来源：http://wkx.sjlbkw.cn

python -m build  （依赖 pyproject.toml）
来源：http://buc.guannengcc.top

[U34] Py：判断编码
来源：http://lkt.zdbjq.cn

chardet.detect(raw)
来源：http://zgo.yuanzhike.top

[U35] Py：发送邮件
来源：http://zrg.dashuyun.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://wpw.yvedp.cn

[U36] Py：定时任务
来源：http://ryq.zhijiandao.cn

schedule.every(10).minutes.do(job)
来源：http://tqr.andypj.xyz

[U37] Py：读写 Excel
来源：http://zgy.hysaishi.cn

pandas.read_excel / DataFrame.to_excel
来源：http://pjl.fehbvm.com

[U38] Py：获取脚本所在目录
来源：http://qqk.jianghu66.top

Path(__file__).resolve().parent
来源：http://jyn.guannengcc.top

[U39] Py：判断是否在交互环境
来源：http://nkx.c1oappe.top

sys.stdout.isatty()
来源：http://vwg.tian-w.cn

[U40] Py：打印到标准错误
来源：http://kme.cucudq.cn

print("err", file=sys.stderr)
来源：http://gfq.52xcode.cn

[U41] PHP：初始化 Composer 项目
来源：http://fxe.guowangkeji.top

composer init;  composer require guzzlehttp/guzzle
来源：http://pfg.0kj1m.cn

[U42] PHP：PSR-4 自动加载
来源：http://irk.cucudq.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hks.chenzaomai.com

[U43] PHP：声明命名空间
来源：http://pwt.havefunace.top

namespace App\Http;
来源：http://kzc.bjfxy.top

[U44] PHP：开启严格类型
来源：http://vhw.hammf.cn

declare(strict_types=1);
来源：http://vah.cheryme.top

[U45] PHP：类型声明与返回类型
来源：http://vmw.sweek.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://unq.yuxming.cn

[U46] PHP：可空类型
来源：http://vcy.jinyuanbaomall.cn

?string $name = null
来源：http://pgq.cdnleiting.top

[U47] PHP：联合类型
来源：http://yjg.chenlongwang.top

int|string $id
来源：http://ote.sweek.top

[U48] PHP：纯枚举
来源：http://rwa.jlsjyb.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://tij.svipenyu.cn

[U49] PHP：只读属性
来源：http://yxc.mhx1999.top

public readonly string $name
来源：http://yja.jlsjyb.cn

[U50] PHP：构造器属性提升
来源：http://rja.hcnkem.com

public function __construct(private int $id) {}
来源：http://okj.zhixingplan.top

[U51] PHP：数组解构
来源：http://etq.jiagoushi.top

[$a, $b] = $arr;
来源：http://ilf.yj20258.top

[U52] PHP：箭头函数
来源：http://ker.cucudq.cn

$double = fn($x) => $x * 2;
来源：http://zol.shuidangran.top

[U53] PHP：空合并运算符
来源：http://qij.mhx1999.top

$v = $a ?? $b ?? "default";
来源：http://okb.sweek.top

[U54] PHP：空安全调用
来源：http://zqd.sxryk.cn

$obj?->method()
来源：http://jye.gotoacloud.top

[U55] PHP：match 表达式
来源：http://scd.xinyue.icu

$s = match($x) { 1 => "一", default => "其他" };
来源：http://mtb.ybcxt.top

[U56] PHP：命名参数
来源：http://iga.jiagoushi.top

f(a: 1, b: 2)
来源：http://box.chenjidiqi.icu

[U57] PHP：字符串插值
来源：http://lor.redwolf501.top

"值: {$a}"
来源：http://qhz.yj20258888.top

[U58] PHP：数组三件套
来源：http://apq.tian-w.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://ova.ywan-chungtsiang.top

[U59] PHP：自定义排序
来源：http://zut.shanyushiyangtech.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://enl.zycfv.cn

[U60] PHP：JSON 编解码
来源：http://yaa.zdqjudy.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://nsm.xuetiantiany.cn

[U61] PHP：正则
来源：http://biz.yj20258.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://iyd.kuanghao11.cn

[U62] PHP：日期对象
来源：http://jup.gzhubu.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://mdl.sufxvd.cn

[U63] PHP：文件读写
来源：http://dlh.yj20258888.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://onx.epnwcf.com

[U64] PHP：目录遍历
来源：http://oxd.gzhubu.top

glob("dir/*.php");  scandir("dir");
来源：http://aol.meibo888.top

[U65] PHP：会话
来源：http://zax.xziqi.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://mkc.yonumen.top

[U66] PHP：设置 Cookie
来源：http://cza.yongpay.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://ecc.hnqzz.top

[U67] PHP：处理文件上传
来源：http://dxy.sysykeji.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://sfw.zhongyouzk.top

[U68] PHP：PDO 连接
来源：http://kwp.daxiang520.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://mwy.xylfe.cn

[U69] PHP：PDO 预处理
来源：http://zjs.0kj1m.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://dla.cheryme.top

[U70] PHP：PDO 事务
来源：http://nyo.sufxvd.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://kyl.shanyushiyangtech.top

[U71] PHP：抛出异常
来源：http://kcv.bbcook.cn

throw new RuntimeException("失败", 500);
来源：http://qxc.hcnkem.com

[U72] PHP：写错误日志
来源：http://uwm.andypj.xyz

error_log("失败: " . $e->getMessage());
来源：http://zgc.xziqi.cn

[U73] PHP：读取 ini 配置
来源：http://dju.dashuyun.cn

parse_ini_file("config.ini", true)
来源：http://jkw.gaohongyu789.top

[U74] PHP：读取环境变量
来源：http://kcl.fehbvm.com

getenv("APP_ENV") ?: "production"
来源：http://kis.iojbl.cn

[U75] PHP：依赖注入
来源：http://uvu.jinyuanbaomall.cn

composer require psr/container
来源：http://vvs.vehdjk.com

[U76] PHP：简单路由
来源：http://nwl.shanyushiyangtech.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://syk.pengpengdd.cyou

[U77] PHP：模板渲染
来源：http://gjm.fktsv.cn

composer require twig/twig
来源：http://hvn.yvedp.cn

[U78] PHP：单元测试
来源：http://eqi.tianlin.xyz

composer require --dev phpunit/phpunit
来源：http://wxo.cdnleiting.top

[U79] PHP：静态分析
来源：http://xdq.zdqjudy.top

composer require --dev phpstan/phpstan
来源：http://upd.gotoacloud.top

[U80] PHP：代码规范修复
来源：http://brp.sysykeji.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://bch.fengsongda.top

[U81] JS：初始化项目
来源：http://hlu.ybcxt.top

npm init -y;  npm i express
来源：http://fam.zhijiandao.cn

[U82] JS：package.json 脚本
来源：http://mxg.jinqigfzy.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://hhi.c1oappe.top

[U83] JS：ES Module 导入导出
来源：http://ypg.316326.xyz

export const a = 1;  import { a } from "./m.js";
来源：http://iva.yvedp.cn

[U84] JS：CommonJS 写法
来源：http://gxj.316326.xyz

module.exports = { a };  const { a } = require("./m");
来源：http://anx.jinghuilouyu.cn

[U85] JS：可选链
来源：http://ivk.shzxlz.cn

a?.b?.c
来源：http://bil.quarkkingdee.top

[U86] JS：空值合并
来源：http://smg.cucudq.cn

a ?? b
来源：http://bfv.uphjek.com

[U87] JS：解构默认值
来源：http://vaf.shuidangran.top

const { a = 1, b = 2 } = obj;
来源：http://aae.zhijiandao.cn

[U88] JS：对象展开合并
来源：http://tqq.xingfuxueyuan.xyz

{ ...a, ...b }
来源：http://tjo.shangyingyoupin.top

[U89] JS：数组去重
来源：http://xmc.tian-w.cn

[...new Set(arr)]
来源：http://gvg.cashguo.top

[U90] JS：数字数组排序
来源：http://ltz.jyoumei.cn

[...arr].sort((a, b) => a - b)
来源：http://bom.zhoulong.xyz

[U91] JS：对象键值遍历
来源：http://yct.jqgufenzy.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://rtg.hnqzz.top

[U92] JS：深拷贝
来源：http://dpt.shanyushiyangtech.top

structuredClone(obj)
来源：http://yyy.hongshengwenyu.top

[U93] JS：模板字符串
来源：http://kud.yj202588.top

`共 ${n} 条`
来源：http://twj.yueranfly.top

[U94] JS：箭头函数
来源：http://mjw.daxiang520.top

const double = x => x * 2;
来源：http://fqp.ywan-chungtsiang.top

[U95] JS：Promise 包装
来源：http://pue.pengpengdd.cyou

new Promise((resolve, reject) => {})
来源：http://tlp.hfpthk.cn

[U96] JS：async/await 与异常
来源：http://noi.shuidangran.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://onf.yj20258.top

[U97] JS：并发请求
来源：http://ois.zhongyouzk.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://ttk.hfpthk.cn

[U98] JS：fetch 带 JSON
来源：http://szf.shuidangran.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://xdo.haohaochexian.top

[U99] JS：事件监听
来源：http://tfz.9152youxi.cn

el.addEventListener("click", e => {})
来源：http://vef.cucudq.cn

[U100] JS：DOM 查询
来源：http://lei.fzhhl.top

document.querySelector(".item")
来源：http://itf.yonumen.top

[U101] JS：classList 操作
来源：http://tfv.guannengcc.top

el.classList.toggle("active")
来源：http://bhk.cdnleiting.top

[U102] JS：本地存储
来源：http://nqc.yvedp.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://dyy.yuxming.cn

[U103] JS：定时器
来源：http://zld.jqgufenzy.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://vuc.jinyuanbaomall.cn

[U104] JS：防抖
来源：http://nlv.dashuyun.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://xav.yueranfly.top

[U105] JS：节流
来源：http://omo.bbcook.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://nqk.jqgufenzy.top

[U106] JS：日期格式化
来源：http://yov.pycfn.com

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://vaz.sjlbkw.cn

[U107] JS：数字千分位
来源：http://qns.zhongyouzk.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://jeb.jlsjyb.cn

[U108] JS：随机整数
来源：http://npz.redwolf501.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://rvk.ppjwa.cn

[U109] JS：数组分组
来源：http://icw.sysykeji.top

Object.groupBy(arr, x => x.type)
来源：http://syw.gzhubu.top

[U110] JS：数组分块
来源：http://rfy.quarkkingdee.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://oez.yj20258888.top

[U111] JS：对象转 Map
来源：http://jjq.ppjwa.cn

new Map(Object.entries(obj))
来源：http://mlu.epnwcf.com

[U112] JS：字符串补位
来源：http://mux.ctjpmb.com

"7".padStart(3, "0")
来源：http://gjj.tianlin.xyz

[U113] JS：正则替换全部
来源：http://aao.hfpthk.cn

s.replaceAll("a", "b")
来源：http://opb.kuanghao11.cn

[U114] JS：JSON 深比较
来源：http://pzf.sysykeji.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://bij.yj20258.top

[U115] JS：生成 UUID
来源：http://uwr.dashuyun.cn

crypto.randomUUID()
来源：http://rri.nanxinkj.top

[U116] JS：类型检查（JSDoc）
来源：http://iui.hesvh.cn

/** @param {string} name */ function f(name) {}
来源：http://wxx.zdqjudy.top

[U117] JS：单元测试
来源：http://mgm.zhijiandao.cn

npm i -D vitest;  npx vitest
来源：http://oqh.dianchejie.cn

[U118] JS：开发服务器
来源：http://rbz.andypj.xyz

npm i -D vite;  npx vite
来源：http://oxj.ybcxt.top

[U119] JS：生产构建
来源：http://jim.52xcode.cn

npx vite build
来源：http://inz.yanxiufei.cn

[U120] JS：读取环境变量（Vite）
来源：http://qhz.yvedp.cn

import.meta.env.VITE_API_URL
来源：http://bxu.xylfe.cn

================================================================================
来源：http://coe.hcnkem.com

统计汇总
来源：http://kum.wangdashe.top

================================================================================
来源：http://get.xuetiantiany.cn

按语言统计（条）：
来源：http://zad.yfazqb.com

Python ......... 252
来源：http://uyl.chenzaomai.com

PHP ............ 252
来源：http://ltt.jinqigufen.top

JavaScript ..... 252
来源：http://uya.daria6918.cn

TypeScript ..... 212
来源：http://fyg.zdqjudy.top

Java ........... 212
来源：http://gxs.sxryk.cn

Go ............. 212
来源：http://ypo.yj20258.top

Ruby ........... 212
来源：http://anq.xziqi.cn

C# ............. 212
来源：http://mvm.xuetiantiany.cn

C .............. 30
来源：http://uyu.fanxiaobao.xyz

C++ ............ 30
来源：http://jsv.xuanzx.com

SQL ............ 90
来源：http://pat.uphjek.com

Bash ........... 80
来源：http://hpa.jinyuanbaomall.cn

Kotlin ......... 15
来源：http://yua.jyoumei.cn

Swift .......... 15
来源：http://yjz.zhongyouzk.top

Lua ............ 10
来源：http://oif.yonumen.top

Perl ........... 10
来源：http://mkj.ctjpmb.com

Scala .......... 10
来源：http://rxz.zycfv.cn

------------------------------------
来源：http://pql.pengpengdd.cyou

合计 ........... 2106 条
来源：http://blq.fengsongda.top

按章节统计：
来源：http://ycq.daria6918.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://vcd.yj20258888.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://fxs.yuanzhike.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://uho.dashuyun.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://tcj.yueranfly.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://aao.yueranfly.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://crb.shanyushiyangkeji.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://ota.smart0.xyz

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://dkj.kuanghao11.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://mkk.0kj1m.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://thz.sweek.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://xve.zhengqikj.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://awn.nanxuanxn.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://cqw.tarul.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://jxu.316326.xyz

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://vxr.zhiwuduotai.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://nyu.jqgufenzy.top

Q SQL 专题                              90
来源：http://vmu.jyoumei.cn

R Bash 专题                             80
来源：http://qkf.c1oappe.top

S C / C++ 专题                          60
来源：http://clf.shangyingyoupin.top

T 其他语言补充                          60
来源：http://xpa.yongpay.top

U 高频实用片段                         120
来源：http://oaf.zhengqikj.top

------------------------------------
来源：http://fbf.yvedp.cn

合计                                  2106 条
来源：http://fjm.fzhhl.top

--------------------------------------------------------------------------------
来源：http://vth.jianghu66.top

使用提醒
来源：http://mpw.guannengcc.top

--------------------------------------------------------------------------------
来源：http://hew.feifeiyinyue.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://kgb.redwolf501.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://ezf.shanyushiyangtech.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://rvc.yj202588.top

在旧版本上使用前请先确认语法支持情况。
来源：http://wdv.52xcode.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://khb.wangshuangyany.cn

—— 文件结束 ——
来源：http://zkr.yonumen.top

================================================================================
来源：http://vyo.guannengcc.top

程序语言常见例子速查手册（2024 版）
来源：http://ivk.sufxvd.cn

Common Programming Examples Cheat Book
来源：http://xnn.guowangkeji.top

================================================================================
来源：http://lzh.jlsjyb.cn

【收录内容】
来源：http://zve.fktsv.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://qsz.ehwqpu.com

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://fjv.jiagoushi.top

SQL · Bash · C · C++
来源：http://jfo.hongshengwenyu.top


<!-- 参考信息 -->