代发 wailian999

[U11] Py：生成器表达式
来源：http://qbj.yuanzhike.top

(x * 2 for x in arr)
来源：http://lai.tianlin.xyz

[U12] Py：取出现最多的 3 个元素
来源：http://vci.quarkkingdee.top

Counter(arr).most_common(3)
来源：http://jtz.zhijiandao.cn

[U13] Py：固定长度队列
来源：http://eyd.ivvv.top

deque(maxlen=10)
来源：http://onq.yueranfly.top

[U14] Py：分组收集到列表
来源：http://xkp.pengpengdd.cyou

defaultdict(list)
来源：http://mtc.yvedp.cn

[U15] Py：高精度计时
来源：http://ykq.xuetiantiany.cn

t = time.perf_counter()
来源：http://mww.uphjek.com

[U16] Py：命令行参数解析
来源：http://san.jqgufenzy.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://pku.cheryme.top

[U17] Py：初始化日志
来源：http://iju.yj20258888.top

logging.basicConfig(level=logging.INFO)
来源：http://hly.gogol.net.cn

[U18] Py：预编译正则
来源：http://nre.hnqzz.top

pat = re.compile(r"\d+")
来源：http://qit.bbcook.cn

[U19] Py：正则替换带回调
来源：http://doi.jlsjyb.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://oof.hnxiangtu.top

[U20] Py：缓存函数结果
来源：http://fyc.c1oappe.top

@functools.lru_cache(maxsize=None)
来源：http://idp.pengpengdd.cyou

[U21] Py：自定义上下文管理器
来源：http://uht.chenjidiqi.icu

@contextlib.contextmanager
来源：http://bfu.shanyushiyangkeji.top

[U22] Py：矩阵转置
来源：http://etw.shzxlz.cn

list(zip(*m))
来源：http://uas.cqqwz.cn

[U23] Py：分块读取大文件
来源：http://exe.jinqigufen.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://nmi.ydzc1.top

[U24] Py：路径操作
来源：http://tvq.hnqzz.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://ycc.fanxiaobao.xyz

[U25] Py：CSV 按字典读
来源：http://cbq.zhixingplan.top

csv.DictReader(f)
来源：http://psk.jiagoushi.top

[U26] Py：并发下载
来源：http://gyq.epnwcf.com

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://tqc.0kj1m.cn

[U27] Py：异步 HTTP
来源：http://jpr.jiagoushi.top

aiohttp.ClientSession() 配合 async with
来源：http://szg.haohaochexian.top

[U28] Py：类型别名
来源：http://ldt.cqqwz.cn

UserId = int
来源：http://tlo.nwbrower.top

[U29] Py：属性校验
来源：http://smg.zhongyouzk.top

@property 与 @x.setter 配合
来源：http://fku.jinyuanbaomall.cn

[U30] Py：数据类
来源：http://xtr.zhongyouzk.top

@dataclass(slots=True)
来源：http://woy.cucudq.cn

[U31] Py：单测
来源：http://rst.fktsv.cn

python -m pytest -q
来源：http://whb.jinghuilouyu.cn

[U32] Py：代码格式化
来源：http://jzp.sweek.top

ruff format . && ruff check --fix .
来源：http://azt.zhoulong.xyz

[U33] Py：打包发布
来源：http://xms.tarul.cn

python -m build  （依赖 pyproject.toml）
来源：http://fml.hnqzz.top

[U34] Py：判断编码
来源：http://tay.hfpthk.cn

chardet.detect(raw)
来源：http://dgs.pengpengdd.cyou

[U35] Py：发送邮件
来源：http://yfl.epnwcf.com

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://qlz.ywan-chungtsiang.top

[U36] Py：定时任务
来源：http://fte.52xcode.cn

schedule.every(10).minutes.do(job)
来源：http://nvx.andypj.xyz

[U37] Py：读写 Excel
来源：http://esm.jinqigufen.top

pandas.read_excel / DataFrame.to_excel
来源：http://asv.bbcook.cn

[U38] Py：获取脚本所在目录
来源：http://dun.316326.xyz

Path(__file__).resolve().parent
来源：http://dto.9152youxi.cn

[U39] Py：判断是否在交互环境
来源：http://jjo.sjlbkw.cn

sys.stdout.isatty()
来源：http://eec.fktsv.cn

[U40] Py：打印到标准错误
来源：http://zpr.fehbvm.com

print("err", file=sys.stderr)
来源：http://tpc.jqgfzy.top

[U41] PHP：初始化 Composer 项目
来源：http://vgi.yonumen.top

composer init;  composer require guzzlehttp/guzzle
来源：http://uoq.sjlbkw.cn

[U42] PHP：PSR-4 自动加载
来源：http://tzm.hysaishi.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://fev.fengsongda.top

[U43] PHP：声明命名空间
来源：http://sry.zhijiandao.cn

namespace App\Http;
来源：http://lhl.gzhubu.top

[U44] PHP：开启严格类型
来源：http://pwe.xingfuxueyuan.xyz

declare(strict_types=1);
来源：http://oel.ydzc1.top

[U45] PHP：类型声明与返回类型
来源：http://cur.shzxlz.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://cwc.pycfn.com

[U46] PHP：可空类型
来源：http://wly.svipenyu.cn

?string $name = null
来源：http://gbj.jqgufenzy.top

[U47] PHP：联合类型
来源：http://vug.jlsjyb.cn

int|string $id
来源：http://jxd.yueranfly.top

[U48] PHP：纯枚举
来源：http://jrb.smart0.xyz

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://uio.chenlongwang.top

[U49] PHP：只读属性
来源：http://fqg.zhongyouzk.top

public readonly string $name
来源：http://tci.yongpay.top

[U50] PHP：构造器属性提升
来源：http://pzm.uphjek.com

public function __construct(private int $id) {}
来源：http://exp.uphjek.com

[U51] PHP：数组解构
来源：http://jxp.cashguo.top

[$a, $b] = $arr;
来源：http://kfd.ydjk.org.cn

[U52] PHP：箭头函数
来源：http://svp.xylfe.cn

$double = fn($x) => $x * 2;
来源：http://qwy.yangfankeji.com

[U53] PHP：空合并运算符
来源：http://mdt.wangshuangyany.cn

$v = $a ?? $b ?? "default";
来源：http://qco.chenlongwang.top

[U54] PHP：空安全调用
来源：http://heb.zhongyouzk.top

$obj?->method()
来源：http://tfl.jyoumei.cn

[U55] PHP：match 表达式
来源：http://aey.meibo888.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://kyo.shanyushiyangkeji.top

[U56] PHP：命名参数
来源：http://dud.zhongyouzk.top

f(a: 1, b: 2)
来源：http://zrc.c1oappe.top

[U57] PHP：字符串插值
来源：http://hsq.nwbrower.top

"值: {$a}"
来源：http://wna.hongshengwenyu.top

[U58] PHP：数组三件套
来源：http://lox.xuetiantiany.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://ykz.vehdjk.com

[U59] PHP：自定义排序
来源：http://zcq.wangshuangyany.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://kpl.wangshuangyany.cn

[U60] PHP：JSON 编解码
来源：http://nbf.chenjidiqi.icu

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://jnd.zycfv.cn

[U61] PHP：正则
来源：http://egc.hysaishi.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://zuf.shzxlz.cn

[U62] PHP：日期对象
来源：http://ykv.jinqigufen.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://lqu.cheryme.top

[U63] PHP：文件读写
来源：http://pix.yj20258.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://tyy.hcnkem.com

[U64] PHP：目录遍历
来源：http://wtj.jqgfzy.top

glob("dir/*.php");  scandir("dir");
来源：http://mqs.sysykeji.top

[U65] PHP：会话
来源：http://tem.xinyue.icu

session_start();  $_SESSION["uid"] = 1;
来源：http://gtu.nanxuanxn.top

[U66] PHP：设置 Cookie
来源：http://oyd.sxryk.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://gpt.zdbjq.cn

[U67] PHP：处理文件上传
来源：http://ifc.hesvh.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://fbi.nanxuanxn.top

[U68] PHP：PDO 连接
来源：http://grx.jyoumei.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://mfn.chenzaomai.com

[U69] PHP：PDO 预处理
来源：http://qlk.daria6918.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://yfi.smart0.xyz

[U70] PHP：PDO 事务
来源：http://kud.xinyue.icu

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://dxp.shuidangran.top

[U71] PHP：抛出异常
来源：http://zsg.jinqigfzy.top

throw new RuntimeException("失败", 500);
来源：http://llb.redwolf501.top

[U72] PHP：写错误日志
来源：http://ufw.daxiang520.top

error_log("失败: " . $e->getMessage());
来源：http://izz.cashguo.top

[U73] PHP：读取 ini 配置
来源：http://vvp.iojbl.cn

parse_ini_file("config.ini", true)
来源：http://wtv.zdqjudy.top

[U74] PHP：读取环境变量
来源：http://uiv.yanxiufei.cn

getenv("APP_ENV") ?: "production"
来源：http://zld.hysaishi.cn

[U75] PHP：依赖注入
来源：http://uax.ydzc1.top

composer require psr/container
来源：http://dhn.yonumen.top

[U76] PHP：简单路由
来源：http://hkv.bjfxy.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://ejw.yanxiufei.cn

[U77] PHP：模板渲染
来源：http://vil.zhoulong.xyz

composer require twig/twig
来源：http://kne.jiagoushi.top

[U78] PHP：单元测试
来源：http://tci.shuidangran.top

composer require --dev phpunit/phpunit
来源：http://bgg.feifeiyinyue.top

[U79] PHP：静态分析
来源：http://ltn.zhoulong.xyz

composer require --dev phpstan/phpstan
来源：http://khd.ydzc1.top

[U80] PHP：代码规范修复
来源：http://tni.shanyushiyangtech.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://fbp.hcnkem.com

[U81] JS：初始化项目
来源：http://jba.yonumen.top

npm init -y;  npm i express
来源：http://pgz.gaohongyu789.top

[U82] JS：package.json 脚本
来源：http://lak.ydzc1.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://cba.hnqzz.top

[U83] JS：ES Module 导入导出
来源：http://erh.jlsjyb.cn

export const a = 1;  import { a } from "./m.js";
来源：http://aga.hnqzz.top

[U84] JS：CommonJS 写法
来源：http://efl.tianlin.xyz

module.exports = { a };  const { a } = require("./m");
来源：http://oww.jinqigufen.top

[U85] JS：可选链
来源：http://lum.ppjwa.cn

a?.b?.c
来源：http://kji.c1oappe.top

[U86] JS：空值合并
来源：http://buu.fengsongda.top

a ?? b
来源：http://atw.wangdashe.top

[U87] JS：解构默认值
来源：http://hfs.fehbvm.com

const { a = 1, b = 2 } = obj;
来源：http://vfh.nanxinkj.top

[U88] JS：对象展开合并
来源：http://uxf.meibo888.top

{ ...a, ...b }
来源：http://kgi.shanyushiyangkeji.top

[U89] JS：数组去重
来源：http://gpu.aibaodan.cn

[...new Set(arr)]
来源：http://plj.jyoumei.cn

[U90] JS：数字数组排序
来源：http://kzx.52xcode.cn

[...arr].sort((a, b) => a - b)
来源：http://nyr.yanxiufei.cn

[U91] JS：对象键值遍历
来源：http://qus.dianchejie.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://dmh.tianlin.xyz

[U92] JS：深拷贝
来源：http://tha.ctjpmb.com

structuredClone(obj)
来源：http://qnd.dianchejie.cn

[U93] JS：模板字符串
来源：http://zdu.gotoacloud.top

`共 ${n} 条`
来源：http://eti.sxryk.cn

[U94] JS：箭头函数
来源：http://bwy.aizwys.cn

const double = x => x * 2;
来源：http://ahf.gotoacloud.top

[U95] JS：Promise 包装
来源：http://vxn.wangdashe.top

new Promise((resolve, reject) => {})
来源：http://kjo.zhiwuduotai.top

[U96] JS：async/await 与异常
来源：http://box.wangshuangyany.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://cuy.nwbrower.top

[U97] JS：并发请求
来源：http://uic.jiagoushi.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://pga.wangshuangyany.cn

[U98] JS：fetch 带 JSON
来源：http://ofx.xingfuxueyuan.xyz

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://euy.hnxiangtu.top

[U99] JS：事件监听
来源：http://otw.nanxuanxn.top

el.addEventListener("click", e => {})
来源：http://eom.mhx1999.top

[U100] JS：DOM 查询
来源：http://goe.redwolf501.top

document.querySelector(".item")
来源：http://nws.mhx1999.top

[U101] JS：classList 操作
来源：http://uhz.dianchejie.cn

el.classList.toggle("active")
来源：http://ruh.pengpengdd.cyou

[U102] JS：本地存储
来源：http://ytl.fzhhl.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://zdc.fengsongda.top

[U103] JS：定时器
来源：http://jwu.xingfuxueyuan.xyz

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://nwx.vehdjk.com

[U104] JS：防抖
来源：http://rzj.sufxvd.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://aut.jqgfzy.top

[U105] JS：节流
来源：http://rpe.jinqigfzy.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://ear.ydzc1.top

[U106] JS：日期格式化
来源：http://qxu.yj20258888.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://bes.hongshengwenyu.top

[U107] JS：数字千分位
来源：http://dhn.jinqigfzy.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://oqy.guannengcc.top

[U108] JS：随机整数
来源：http://kkh.ydzc1.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://qyk.jqgufenzy.top

[U109] JS：数组分组
来源：http://oyp.jqgfzy.top

Object.groupBy(arr, x => x.type)
来源：http://aiv.nanxuanxn.top

[U110] JS：数组分块
来源：http://yet.yonumen.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://kon.yj20258888.top

[U111] JS：对象转 Map
来源：http://bdg.vehdjk.com

new Map(Object.entries(obj))
来源：http://zyn.xuetiantiany.cn

[U112] JS：字符串补位
来源：http://ftv.redwolf501.top

"7".padStart(3, "0")
来源：http://cnd.zhoulong.xyz

[U113] JS：正则替换全部
来源：http://vds.52xcode.cn

s.replaceAll("a", "b")
来源：http://sze.zycfv.cn

[U114] JS：JSON 深比较
来源：http://fhn.yonumen.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://imy.mhx1999.top

[U115] JS：生成 UUID
来源：http://zgo.yfazqb.com

crypto.randomUUID()
来源：http://ifs.dashuyun.cn

[U116] JS：类型检查（JSDoc）
来源：http://aau.zhixingplan.top

/** @param {string} name */ function f(name) {}
来源：http://hex.hesvh.cn

[U117] JS：单元测试
来源：http://lea.yfazqb.com

npm i -D vitest;  npx vitest
来源：http://stj.zhiwuduotai.top

[U118] JS：开发服务器
来源：http://box.ivvv.top

npm i -D vite;  npx vite
来源：http://vdt.yueranfly.top

[U119] JS：生产构建
来源：http://lpm.pycfn.com

npx vite build
来源：http://ubt.tian-w.cn

[U120] JS：读取环境变量（Vite）
来源：http://ipk.cqqwz.cn

import.meta.env.VITE_API_URL
来源：http://dma.daxiang520.top

================================================================================
来源：http://ihy.iojbl.cn

统计汇总
来源：http://lts.jinyuanbaomall.cn

================================================================================
来源：http://diy.hywenlv.cn

按语言统计（条）：
来源：http://see.sufxvd.cn

Python ......... 252
来源：http://wsv.yangfankeji.com

PHP ............ 252
来源：http://jpn.hysaishi.cn

JavaScript ..... 252
来源：http://dsa.sysykeji.top

TypeScript ..... 212
来源：http://bxn.ydzc1.top

Java ........... 212
来源：http://rza.aibaodan.cn

Go ............. 212
来源：http://awg.ybcxt.top

Ruby ........... 212
来源：http://deq.aizwys.cn

C# ............. 212
来源：http://ikw.wangdashe.top

C .............. 30
来源：http://cav.316326.xyz

C++ ............ 30
来源：http://owh.aizwys.cn

SQL ............ 90
来源：http://xfx.snrcjt.cn

Bash ........... 80
来源：http://ymx.zhaomingkeji.xyz

Kotlin ......... 15
来源：http://mgg.ehwqpu.com

Swift .......... 15
来源：http://qfd.feifeiyinyue.top

Lua ............ 10
来源：http://szm.cdnleiting.top

Perl ........... 10
来源：http://mhk.0kj1m.cn

Scala .......... 10
来源：http://vah.cqqwz.cn

------------------------------------
来源：http://ffs.hfpthk.cn

合计 ........... 2106 条
来源：http://hpi.aizwys.cn

按章节统计：
来源：http://gww.hywenlv.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://bbv.xylfe.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://zze.hfpthk.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://gsw.jianghu66.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://tmy.zdbjq.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://onm.yvedp.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://yxm.tianlin.xyz

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://wnc.nanxuanxn.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://vik.jqgfzy.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://uiw.bjfxy.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://bmj.bjfxy.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://mdc.cqqwz.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://joo.yanxiufei.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://ctj.dashuyun.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://rbh.daxiang520.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://lyl.fanxiaobao.xyz

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://cbc.uphjek.com

Q SQL 专题                              90
来源：http://bfw.yfazqb.com

R Bash 专题                             80
来源：http://fig.wangshuangyany.cn

S C / C++ 专题                          60
来源：http://jrd.xylfe.cn

T 其他语言补充                          60
来源：http://aha.cucudq.cn

U 高频实用片段                         120
来源：http://zmc.gzhubu.top

------------------------------------
来源：http://ngu.hnxiangtu.top

合计                                  2106 条
来源：http://lar.kuanghao11.cn

--------------------------------------------------------------------------------
来源：http://zjx.hysaishi.cn

使用提醒
来源：http://pqm.yangfankeji.com

--------------------------------------------------------------------------------
来源：http://iib.aizwys.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://egk.wangdashe.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://rac.jqgfzy.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://bpj.jiagoushi.top

在旧版本上使用前请先确认语法支持情况。
来源：http://ujo.aizwys.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://zpu.gotoacloud.top

—— 文件结束 ——
来源：http://zgc.jinghuilouyu.cn

================================================================================
来源：http://rxx.uphjek.com

程序语言常见例子速查手册（2024 版）
来源：http://npw.yueranfly.top

Common Programming Examples Cheat Book
来源：http://mlq.hysaishi.cn

================================================================================
来源：http://vbx.cdnleiting.top

【收录内容】
来源：http://wci.tarul.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://vqt.c1oappe.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://hhs.daria6918.cn

SQL · Bash · C · C++
来源：http://gnt.jinqigfzy.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://qoi.yongpay.top

【使用说明】
来源：http://krn.zhengqikj.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://cpy.guowangkeji.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://lrh.yongpay.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://vvo.zhiwuduotai.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://hki.sweek.top

Bash:  Shell         C:     C             C++:   C++
来源：http://ydn.aizwys.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://yfy.bjfxy.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://kqc.nanxuanxn.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://qwr.sjlbkw.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://ykg.daxiang520.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://ygj.gotoacloud.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://dtq.hongshengwenyu.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://uwt.jqgfzy.top

【文件统计】
来源：http://xgp.bjfxy.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://vkd.sweek.top


<!-- 参考信息 -->