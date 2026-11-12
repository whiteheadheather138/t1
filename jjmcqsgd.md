代发 wailian999

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://mlh.jlsjyb.cn

================================================================================
来源：http://yxd.fengsongda.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://rxn.hnxiangtu.top

================================================================================
来源：http://muq.sjlbkw.cn

[U01] Py：创建虚拟环境
来源：http://xob.feifeiyinyue.top

python -m venv .venv && source .venv/bin/activate
来源：http://bdv.feifeiyinyue.top

[U02] Py：导出 / 安装依赖
来源：http://hwp.cqqwz.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://syi.jinqigufen.top

[U03] Py：加载 .env 配置
来源：http://cse.jqgufenzy.top

from dotenv import load_dotenv; load_dotenv()
来源：http://fyl.tian-w.cn

[U04] Py：变量调试打印
来源：http://zrc.ctjpmb.com

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://fim.fehbvm.com

[U05] Py：列表去重且保序
来源：http://xcb.yj20258888.top

list(dict.fromkeys(arr))
来源：http://eql.hongshengwenyu.top

[U06] Py：合并两个字典
来源：http://crj.hywenlv.cn

{**a, **b}
来源：http://err.fehbvm.com

[U07] Py：反转字典键值
来源：http://qad.cucudq.cn

{v: k for k, v in d.items()}
来源：http://nkq.svipenyu.cn

[U08] Py：展平二维列表
来源：http://hzg.meibo888.top

[y for x in nested for y in x]
来源：http://dkq.hnxiangtu.top

[U09] Py：字典取最大值的键
来源：http://oqx.ywan-chungtsiang.top

max(d, key=d.get)
来源：http://eyp.hesvh.cn

[U10] Py：按值排序字典
来源：http://gkh.fehbvm.com

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://yat.zhixingplan.top

[U11] Py：生成器表达式
来源：http://ujs.xuetiantiany.cn

(x * 2 for x in arr)
来源：http://tns.feifeiyinyue.top

[U12] Py：取出现最多的 3 个元素
来源：http://mpi.fengsongda.top

Counter(arr).most_common(3)
来源：http://gsf.chenjidiqi.icu

[U13] Py：固定长度队列
来源：http://kui.sysykeji.top

deque(maxlen=10)
来源：http://enf.wangdashe.top

[U14] Py：分组收集到列表
来源：http://heu.hfpthk.cn

defaultdict(list)
来源：http://iko.52xcode.cn

[U15] Py：高精度计时
来源：http://kqu.gotoacloud.top

t = time.perf_counter()
来源：http://dyj.meibo888.top

[U16] Py：命令行参数解析
来源：http://mzy.feifeiyinyue.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://tws.fzhhl.top

[U17] Py：初始化日志
来源：http://kgu.epnwcf.com

logging.basicConfig(level=logging.INFO)
来源：http://sdd.haohaochexian.top

[U18] Py：预编译正则
来源：http://uzo.mhx1999.top

pat = re.compile(r"\d+")
来源：http://ogj.tianlin.xyz

[U19] Py：正则替换带回调
来源：http://zbc.yanxiufei.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://kfi.gaohongyu789.top

[U20] Py：缓存函数结果
来源：http://tqd.yuxming.cn

@functools.lru_cache(maxsize=None)
来源：http://pin.jinqigufen.top

[U21] Py：自定义上下文管理器
来源：http://taj.nwbrower.top

@contextlib.contextmanager
来源：http://cfp.ydzc1.top

[U22] Py：矩阵转置
来源：http://xwj.ywan-chungtsiang.top

list(zip(*m))
来源：http://tdw.0kj1m.cn

[U23] Py：分块读取大文件
来源：http://wql.52xcode.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://mvq.cqqwz.cn

[U24] Py：路径操作
来源：http://ypm.andypj.xyz

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://pqx.ehwqpu.com

[U25] Py：CSV 按字典读
来源：http://mej.cheryme.top

csv.DictReader(f)
来源：http://trr.xingfuxueyuan.xyz

[U26] Py：并发下载
来源：http://dvu.zhixingplan.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://ekf.jinyuanbaomall.cn

[U27] Py：异步 HTTP
来源：http://ihg.daxiang520.top

aiohttp.ClientSession() 配合 async with
来源：http://oxg.zhijiandao.cn

[U28] Py：类型别名
来源：http://omw.fehbvm.com

UserId = int
来源：http://mjc.zhixingplan.top

[U29] Py：属性校验
来源：http://lcy.pycfn.com

@property 与 @x.setter 配合
来源：http://twh.haohaochexian.top

[U30] Py：数据类
来源：http://ibk.aizwys.cn

@dataclass(slots=True)
来源：http://qfa.aizwys.cn

[U31] Py：单测
来源：http://hlu.dianchejie.cn

python -m pytest -q
来源：http://cqa.shanyushiyangtech.top

[U32] Py：代码格式化
来源：http://mtl.tianlin.xyz

ruff format . && ruff check --fix .
来源：http://hur.hfpthk.cn

[U33] Py：打包发布
来源：http://lcd.316326.xyz

python -m build  （依赖 pyproject.toml）
来源：http://ppa.fktsv.cn

[U34] Py：判断编码
来源：http://ybl.tianlin.xyz

chardet.detect(raw)
来源：http://lix.zhijiandao.cn

[U35] Py：发送邮件
来源：http://rip.zdbjq.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://bvt.zhiwuduotai.top

[U36] Py：定时任务
来源：http://qia.yangfankeji.com

schedule.every(10).minutes.do(job)
来源：http://zig.andypj.xyz

[U37] Py：读写 Excel
来源：http://wmb.fanxiaobao.xyz

pandas.read_excel / DataFrame.to_excel
来源：http://npd.jianghu66.top

[U38] Py：获取脚本所在目录
来源：http://nuc.jqgufenzy.top

Path(__file__).resolve().parent
来源：http://pjy.vehdjk.com

[U39] Py：判断是否在交互环境
来源：http://ygn.shanyushiyangkeji.top

sys.stdout.isatty()
来源：http://mkw.zhongyouzk.top

[U40] Py：打印到标准错误
来源：http://umo.feifeiyinyue.top

print("err", file=sys.stderr)
来源：http://isf.xuetiantiany.cn

[U41] PHP：初始化 Composer 项目
来源：http://sle.nwbrower.top

composer init;  composer require guzzlehttp/guzzle
来源：http://mwd.zhoulong.xyz

[U42] PHP：PSR-4 自动加载
来源：http://yat.zhixingplan.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://mea.xinyue.icu

[U43] PHP：声明命名空间
来源：http://nfb.fzhhl.top

namespace App\Http;
来源：http://bex.zycfv.cn

[U44] PHP：开启严格类型
来源：http://iug.jinghuilouyu.cn

declare(strict_types=1);
来源：http://egk.sxryk.cn

[U45] PHP：类型声明与返回类型
来源：http://bpi.jianghu66.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://wmi.nanxuanxn.top

[U46] PHP：可空类型
来源：http://pdv.shanyushiyangkeji.top

?string $name = null
来源：http://yzo.andypj.xyz

[U47] PHP：联合类型
来源：http://nwm.tanke756.top

int|string $id
来源：http://xpy.aibaodan.cn

[U48] PHP：纯枚举
来源：http://tea.yonumen.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://bbx.jinghuilouyu.cn

[U49] PHP：只读属性
来源：http://yqd.tanke756.top

public readonly string $name
来源：http://pwv.sweek.top

[U50] PHP：构造器属性提升
来源：http://oke.ywan-chungtsiang.top

public function __construct(private int $id) {}
来源：http://syy.hnxiangtu.top

[U51] PHP：数组解构
来源：http://svo.andypj.xyz

[$a, $b] = $arr;
来源：http://uwb.yuxming.cn

[U52] PHP：箭头函数
来源：http://uop.fengsongda.top

$double = fn($x) => $x * 2;
来源：http://sue.wangshuangyany.cn

[U53] PHP：空合并运算符
来源：http://vjw.yueranfly.top

$v = $a ?? $b ?? "default";
来源：http://gmc.jqgufenzy.top

[U54] PHP：空安全调用
来源：http://hky.yangfankeji.com

$obj?->method()
来源：http://otn.gaohongyu789.top

[U55] PHP：match 表达式
来源：http://dkn.jinghuilouyu.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://zbe.jianghu66.top

[U56] PHP：命名参数
来源：http://dfe.ppjwa.cn

f(a: 1, b: 2)
来源：http://htf.cheryme.top

[U57] PHP：字符串插值
来源：http://bvv.xziqi.cn

"值: {$a}"
来源：http://wbu.smart0.xyz

[U58] PHP：数组三件套
来源：http://gog.daxiang520.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://ifq.jlsjyb.cn

[U59] PHP：自定义排序
来源：http://dlp.zdbjq.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://xmf.uphjek.com

[U60] PHP：JSON 编解码
来源：http://bof.svipenyu.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://baf.aizwys.cn

[U61] PHP：正则
来源：http://bzm.jianghu66.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://wbz.nwbrower.top

[U62] PHP：日期对象
来源：http://qtk.xingfuxueyuan.xyz

(new DateTimeImmutable())->format("Y-m-d");
来源：http://oqz.jqgufenzy.top

[U63] PHP：文件读写
来源：http://pbf.andypj.xyz

file_get_contents($f);  file_put_contents($f, $data);
来源：http://fcl.tian-w.cn

[U64] PHP：目录遍历
来源：http://fqh.yfazqb.com

glob("dir/*.php");  scandir("dir");
来源：http://rkh.jlsjyb.cn

[U65] PHP：会话
来源：http://ibv.hysaishi.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://kmn.hesvh.cn

[U66] PHP：设置 Cookie
来源：http://jqx.ydzc1.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://bdw.hammf.cn

[U67] PHP：处理文件上传
来源：http://boe.yangfankeji.com

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://hzy.hcnkem.com

[U68] PHP：PDO 连接
来源：http://rka.zhiwuduotai.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://ost.zdqjudy.top

[U69] PHP：PDO 预处理
来源：http://uxb.wangdashe.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://ypl.jqgufenzy.top

[U70] PHP：PDO 事务
来源：http://spb.yvedp.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://maj.hnxiangtu.top

[U71] PHP：抛出异常
来源：http://nbd.redwolf501.top

throw new RuntimeException("失败", 500);
来源：http://vqs.nwbrower.top

[U72] PHP：写错误日志
来源：http://lyo.ydzc1.top

error_log("失败: " . $e->getMessage());
来源：http://mrk.yonumen.top

[U73] PHP：读取 ini 配置
来源：http://dxt.cashguo.top

parse_ini_file("config.ini", true)
来源：http://ppl.xuetiantiany.cn

[U74] PHP：读取环境变量
来源：http://xru.dashuyun.cn

getenv("APP_ENV") ?: "production"
来源：http://czx.snrcjt.cn

[U75] PHP：依赖注入
来源：http://ash.uphjek.com

composer require psr/container
来源：http://dhd.nwbrower.top

[U76] PHP：简单路由
来源：http://jbc.jinqigufen.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://sxn.52xcode.cn

[U77] PHP：模板渲染
来源：http://ycw.cashguo.top

composer require twig/twig
来源：http://brm.jinqigufen.top

[U78] PHP：单元测试
来源：http://drv.zhixingplan.top

composer require --dev phpunit/phpunit
来源：http://wcb.shzxlz.cn

[U79] PHP：静态分析
来源：http://zvd.xinyue.icu

composer require --dev phpstan/phpstan
来源：http://dzj.yonumen.top

[U80] PHP：代码规范修复
来源：http://ahw.0kj1m.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://znt.hesvh.cn

[U81] JS：初始化项目
来源：http://jst.vqdsnc.cn

npm init -y;  npm i express
来源：http://pxx.tianlin.xyz

[U82] JS：package.json 脚本
来源：http://rfg.fehbvm.com

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://uvo.zhoulong.xyz

[U83] JS：ES Module 导入导出
来源：http://iaf.meibo888.top

export const a = 1;  import { a } from "./m.js";
来源：http://yeh.yfazqb.com

[U84] JS：CommonJS 写法
来源：http://ort.vehdjk.com

module.exports = { a };  const { a } = require("./m");
来源：http://wwa.xinyue.icu

[U85] JS：可选链
来源：http://uhl.cashguo.top

a?.b?.c
来源：http://iii.fzhhl.top

[U86] JS：空值合并
来源：http://zvd.c1oappe.top

a ?? b
来源：http://eke.wangdashe.top

[U87] JS：解构默认值
来源：http://tzs.hongshengwenyu.top

const { a = 1, b = 2 } = obj;
来源：http://jqf.cashguo.top

[U88] JS：对象展开合并
来源：http://dud.bbcook.cn

{ ...a, ...b }
来源：http://nyr.pengpengdd.cyou

[U89] JS：数组去重
来源：http://gha.zdbjq.cn

[...new Set(arr)]
来源：http://bvd.316326.xyz

[U90] JS：数字数组排序
来源：http://ota.iojbl.cn

[...arr].sort((a, b) => a - b)
来源：http://klb.zycfv.cn

[U91] JS：对象键值遍历
来源：http://sge.cashguo.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hvd.ivvv.top

[U92] JS：深拷贝
来源：http://oha.yj20258888.top

structuredClone(obj)
来源：http://mzn.birdmap.top

[U93] JS：模板字符串
来源：http://gog.hywenlv.cn

`共 ${n} 条`
来源：http://lkr.sysykeji.top

[U94] JS：箭头函数
来源：http://wqt.gaohongyu789.top

const double = x => x * 2;
来源：http://qxv.ybcxt.top

[U95] JS：Promise 包装
来源：http://gql.jinqigfzy.top

new Promise((resolve, reject) => {})
来源：http://efi.vqdsnc.cn

[U96] JS：async/await 与异常
来源：http://gmk.dianchejie.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://ecc.zhoulong.xyz

[U97] JS：并发请求
来源：http://zoz.hywenlv.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://rcg.dashuyun.cn

[U98] JS：fetch 带 JSON
来源：http://wuu.zhiwuduotai.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://mov.dianchejie.cn

[U99] JS：事件监听
来源：http://sto.chenlongwang.top

el.addEventListener("click", e => {})
来源：http://ucp.fktsv.cn

[U100] JS：DOM 查询
来源：http://zjt.guowangkeji.top

document.querySelector(".item")
来源：http://nhc.zhijiandao.cn

[U101] JS：classList 操作
来源：http://vhx.sxryk.cn

el.classList.toggle("active")
来源：http://wxo.aibaodan.cn

[U102] JS：本地存储
来源：http://hio.jlsjyb.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://jpg.yj20258.top

[U103] JS：定时器
来源：http://mfj.gzhubu.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://xhd.gzhubu.top

[U104] JS：防抖
来源：http://isk.zhixingplan.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mxk.nanxinkj.top

[U105] JS：节流
来源：http://yxb.jyoumei.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://adl.pengpengdd.cyou

[U106] JS：日期格式化
来源：http://bdu.jinghuilouyu.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://yfx.zhengqikj.top

[U107] JS：数字千分位
来源：http://pos.aibaodan.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://ahv.fehbvm.com

[U108] JS：随机整数
来源：http://zda.cdnleiting.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://qwz.cdnleiting.top

[U109] JS：数组分组
来源：http://vvh.zdbjq.cn

Object.groupBy(arr, x => x.type)
来源：http://aqa.xinyue.icu

[U110] JS：数组分块
来源：http://qta.redwolf501.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://ths.yj202588.top

[U111] JS：对象转 Map
来源：http://khd.zhengqikj.top

new Map(Object.entries(obj))
来源：http://hiq.cashguo.top

[U112] JS：字符串补位
来源：http://wwt.xuetiantiany.cn

"7".padStart(3, "0")
来源：http://pqg.yj20258888.top

[U113] JS：正则替换全部
来源：http://ehk.jianghu66.top

s.replaceAll("a", "b")
来源：http://jjf.sxryk.cn

[U114] JS：JSON 深比较
来源：http://hyi.hcnkem.com

JSON.stringify(a) === JSON.stringify(b)
来源：http://zjs.yueranfly.top

[U115] JS：生成 UUID
来源：http://wlv.jinqigufen.top

crypto.randomUUID()
来源：http://zzl.hysaishi.cn

[U116] JS：类型检查（JSDoc）
来源：http://mcz.pengpengdd.cyou

/** @param {string} name */ function f(name) {}
来源：http://lbk.daxiang520.top

[U117] JS：单元测试
来源：http://gvz.jinqigufen.top

npm i -D vitest;  npx vitest
来源：http://vio.c1oappe.top

[U118] JS：开发服务器
来源：http://vks.uphjek.com

npm i -D vite;  npx vite
来源：http://sqb.uphjek.com

[U119] JS：生产构建
来源：http://hyg.nwbrower.top

npx vite build
来源：http://njl.jianghu66.top

[U120] JS：读取环境变量（Vite）
来源：http://flg.guowangkeji.top

import.meta.env.VITE_API_URL
来源：http://zvk.shuidangran.top

================================================================================
来源：http://mrt.52xcode.cn

统计汇总
来源：http://egl.zdqjudy.top

================================================================================
来源：http://miy.vehdjk.com

按语言统计（条）：
来源：http://qtb.birdmap.top

Python ......... 252
来源：http://sqt.epnwcf.com

PHP ............ 252
来源：http://bds.ywan-chungtsiang.top

JavaScript ..... 252
来源：http://xjd.jyoumei.cn

TypeScript ..... 212
来源：http://eel.zhongyouzk.top

Java ........... 212
来源：http://uji.cucudq.cn

Go ............. 212
来源：http://fcg.sysykeji.top

Ruby ........... 212
来源：http://hxd.snrcjt.cn

C# ............. 212
来源：http://gkt.chenzaomai.com

C .............. 30
来源：http://wfg.shanyushiyangtech.top

C++ ............ 30
来源：http://pka.jyoumei.cn

SQL ............ 90
来源：http://cdr.daxiang520.top

Bash ........... 80
来源：http://phx.cashguo.top

Kotlin ......... 15
来源：http://ubj.zdbjq.cn

Swift .......... 15
来源：http://zch.ydzc1.top

Lua ............ 10
来源：http://vyx.jqgufenzy.top

Perl ........... 10
来源：http://iph.aizwys.cn

Scala .......... 10
来源：http://efu.ywan-chungtsiang.top

------------------------------------
来源：http://vyz.andypj.xyz

合计 ........... 2106 条
来源：http://vms.cashguo.top

按章节统计：
来源：http://ktv.cashguo.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://uhm.cheryme.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://dir.hysaishi.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://kjq.shuidangran.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://egq.dianchejie.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://awm.tian-w.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://cxd.ivvv.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://kgu.316326.xyz

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hte.cashguo.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://pin.wangshuangyany.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://tlj.iojbl.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://oei.jinqigfzy.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://hzw.yangfankeji.com

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://bpy.sjlbkw.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://zda.hammf.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://lma.jyoumei.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://brz.gogol.net.cn

Q SQL 专题                              90
来源：http://azi.tian-w.cn

R Bash 专题                             80
来源：http://uwt.zhixingplan.top

S C / C++ 专题                          60
来源：http://jbg.epnwcf.com

T 其他语言补充                          60
来源：http://wec.shuidangran.top

U 高频实用片段                         120
来源：http://sel.xziqi.cn

------------------------------------
来源：http://amp.aizwys.cn

合计                                  2106 条
来源：http://tuw.havefunace.top

--------------------------------------------------------------------------------
来源：http://uhb.shzxlz.cn

使用提醒
来源：http://bju.daxiang520.top

--------------------------------------------------------------------------------
来源：http://aza.pengpengdd.cyou

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://rzz.vqdsnc.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://pix.316326.xyz

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://gny.kuanghao11.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://leh.hammf.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://bkv.ivvv.top

—— 文件结束 ——
来源：http://vpi.snrcjt.cn


<!-- 参考信息 -->