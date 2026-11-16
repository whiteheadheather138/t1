代发 wailian999

[U01] Py：创建虚拟环境
来源：http://lar.yanxiufei.cn

python -m venv .venv && source .venv/bin/activate
来源：http://ljn.jqgufenzy.top

[U02] Py：导出 / 安装依赖
来源：http://uix.birdmap.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://srk.jqgfzy.top

[U03] Py：加载 .env 配置
来源：http://aet.fehbvm.com

from dotenv import load_dotenv; load_dotenv()
来源：http://yoh.yonumen.top

[U04] Py：变量调试打印
来源：http://fek.ehwqpu.com

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://kxt.dashuyun.cn

[U05] Py：列表去重且保序
来源：http://phc.nanxinkj.top

list(dict.fromkeys(arr))
来源：http://wla.yj20258888.top

[U06] Py：合并两个字典
来源：http://uql.yj202588.top

{**a, **b}
来源：http://hcj.fehbvm.com

[U07] Py：反转字典键值
来源：http://mdf.nanxuanxn.top

{v: k for k, v in d.items()}
来源：http://dxc.nanxuanxn.top

[U08] Py：展平二维列表
来源：http://fhr.uphjek.com

[y for x in nested for y in x]
来源：http://aah.c1oappe.top

[U09] Py：字典取最大值的键
来源：http://luu.hfpthk.cn

max(d, key=d.get)
来源：http://anv.fktsv.cn

[U10] Py：按值排序字典
来源：http://skn.yfazqb.com

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://uyq.zhixingplan.top

[U11] Py：生成器表达式
来源：http://ruj.aizwys.cn

(x * 2 for x in arr)
来源：http://pia.quarkkingdee.top

[U12] Py：取出现最多的 3 个元素
来源：http://pbf.hywenlv.cn

Counter(arr).most_common(3)
来源：http://kkd.ydjk.org.cn

[U13] Py：固定长度队列
来源：http://wip.yj20258888.top

deque(maxlen=10)
来源：http://jth.yueranfly.top

[U14] Py：分组收集到列表
来源：http://onp.shanyushiyangkeji.top

defaultdict(list)
来源：http://zln.bjfxy.top

[U15] Py：高精度计时
来源：http://xap.yj202588.top

t = time.perf_counter()
来源：http://vbd.haohaochexian.top

[U16] Py：命令行参数解析
来源：http://gig.pycfn.com

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://bym.cheryme.top

[U17] Py：初始化日志
来源：http://eox.dianchejie.cn

logging.basicConfig(level=logging.INFO)
来源：http://dks.ywan-chungtsiang.top

[U18] Py：预编译正则
来源：http://efd.xylfe.cn

pat = re.compile(r"\d+")
来源：http://zcw.ctjpmb.com

[U19] Py：正则替换带回调
来源：http://orw.redwolf501.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://wdx.meibo888.top

[U20] Py：缓存函数结果
来源：http://evw.guowangkeji.top

@functools.lru_cache(maxsize=None)
来源：http://wfa.chenlongwang.top

[U21] Py：自定义上下文管理器
来源：http://obx.daria6918.cn

@contextlib.contextmanager
来源：http://pwr.epnwcf.com

[U22] Py：矩阵转置
来源：http://myf.meibo888.top

list(zip(*m))
来源：http://cjl.yj20258888.top

[U23] Py：分块读取大文件
来源：http://jct.zhixingplan.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://atn.xylfe.cn

[U24] Py：路径操作
来源：http://itn.xylfe.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hvn.cashguo.top

[U25] Py：CSV 按字典读
来源：http://zuk.shuidangran.top

csv.DictReader(f)
来源：http://ggj.hywenlv.cn

[U26] Py：并发下载
来源：http://hgt.jyoumei.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://uih.hammf.cn

[U27] Py：异步 HTTP
来源：http://eky.cashguo.top

aiohttp.ClientSession() 配合 async with
来源：http://gsr.kuanghao11.cn

[U28] Py：类型别名
来源：http://hoc.guowangkeji.top

UserId = int
来源：http://spd.xuanzx.com

[U29] Py：属性校验
来源：http://ust.cqqwz.cn

@property 与 @x.setter 配合
来源：http://dhd.gaohongyu789.top

[U30] Py：数据类
来源：http://cyh.yuanzhike.top

@dataclass(slots=True)
来源：http://dpr.havefunace.top

[U31] Py：单测
来源：http://cpw.shanyushiyangkeji.top

python -m pytest -q
来源：http://dqj.sjlbkw.cn

[U32] Py：代码格式化
来源：http://aba.epnwcf.com

ruff format . && ruff check --fix .
来源：http://jvg.smart0.xyz

[U33] Py：打包发布
来源：http://jlb.zhixingplan.top

python -m build  （依赖 pyproject.toml）
来源：http://sok.birdmap.top

[U34] Py：判断编码
来源：http://yyc.hammf.cn

chardet.detect(raw)
来源：http://iep.zdbjq.cn

[U35] Py：发送邮件
来源：http://xdi.pycfn.com

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://xod.nwbrower.top

[U36] Py：定时任务
来源：http://mrp.svipenyu.cn

schedule.every(10).minutes.do(job)
来源：http://qgd.xylfe.cn

[U37] Py：读写 Excel
来源：http://gaw.jqgfzy.top

pandas.read_excel / DataFrame.to_excel
来源：http://vfd.feifeiyinyue.top

[U38] Py：获取脚本所在目录
来源：http://vjt.vehdjk.com

Path(__file__).resolve().parent
来源：http://kcx.chenzaomai.com

[U39] Py：判断是否在交互环境
来源：http://tfo.cashguo.top

sys.stdout.isatty()
来源：http://tuj.shanyushiyangtech.top

[U40] Py：打印到标准错误
来源：http://ymi.daxiang520.top

print("err", file=sys.stderr)
来源：http://yga.yfazqb.com

[U41] PHP：初始化 Composer 项目
来源：http://par.yvedp.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://rii.cashguo.top

[U42] PHP：PSR-4 自动加载
来源：http://vfa.jiagoushi.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://ajb.jianghu66.top

[U43] PHP：声明命名空间
来源：http://mou.hcnkem.com

namespace App\Http;
来源：http://oui.wangdashe.top

[U44] PHP：开启严格类型
来源：http://vka.hnqzz.top

declare(strict_types=1);
来源：http://xag.chenjidiqi.icu

[U45] PHP：类型声明与返回类型
来源：http://ybe.gaohongyu789.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://pxa.zdbjq.cn

[U46] PHP：可空类型
来源：http://psl.52xcode.cn

?string $name = null
来源：http://eiv.xuetiantiany.cn

[U47] PHP：联合类型
来源：http://elx.uphjek.com

int|string $id
来源：http://rhz.chenzaomai.com

[U48] PHP：纯枚举
来源：http://vwt.hesvh.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://ggi.zhijiandao.cn

[U49] PHP：只读属性
来源：http://axh.pengpengdd.cyou

public readonly string $name
来源：http://wge.kuanghao11.cn

[U50] PHP：构造器属性提升
来源：http://ifg.jinyuanbaomall.cn

public function __construct(private int $id) {}
来源：http://vjr.zycfv.cn

[U51] PHP：数组解构
来源：http://rgt.haohaochexian.top

[$a, $b] = $arr;
来源：http://fsr.vqdsnc.cn

[U52] PHP：箭头函数
来源：http://vfb.shangyingyoupin.top

$double = fn($x) => $x * 2;
来源：http://rif.bbcook.cn

[U53] PHP：空合并运算符
来源：http://ftr.zdbjq.cn

$v = $a ?? $b ?? "default";
来源：http://mvc.jinghuilouyu.cn

[U54] PHP：空安全调用
来源：http://xjs.jlsjyb.cn

$obj?->method()
来源：http://jfb.kuanghao11.cn

[U55] PHP：match 表达式
来源：http://loh.fengsongda.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://zxb.jianghu66.top

[U56] PHP：命名参数
来源：http://zps.zhijiandao.cn

f(a: 1, b: 2)
来源：http://mwk.nanxinkj.top

[U57] PHP：字符串插值
来源：http://dql.hongshengwenyu.top

"值: {$a}"
来源：http://kig.gotoacloud.top

[U58] PHP：数组三件套
来源：http://ell.guannengcc.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://okt.tian-w.cn

[U59] PHP：自定义排序
来源：http://agm.iojbl.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://yjx.fzhhl.top

[U60] PHP：JSON 编解码
来源：http://tay.sysykeji.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://wsn.quarkkingdee.top

[U61] PHP：正则
来源：http://dtd.mhx1999.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://gab.ivvv.top

[U62] PHP：日期对象
来源：http://jcv.zdqjudy.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://xzg.mhx1999.top

[U63] PHP：文件读写
来源：http://xyt.zhijiandao.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://oin.zhiwuduotai.top

[U64] PHP：目录遍历
来源：http://fui.ppjwa.cn

glob("dir/*.php");  scandir("dir");
来源：http://ogx.haohaochexian.top

[U65] PHP：会话
来源：http://acn.hongshengwenyu.top

session_start();  $_SESSION["uid"] = 1;
来源：http://pep.cqqwz.cn

[U66] PHP：设置 Cookie
来源：http://lzs.nanxinkj.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://bdk.jianghu66.top

[U67] PHP：处理文件上传
来源：http://qvs.shuidangran.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://bfk.jinqigfzy.top

[U68] PHP：PDO 连接
来源：http://wrg.zdqjudy.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://dhd.316326.xyz

[U69] PHP：PDO 预处理
来源：http://ukr.hnqzz.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://wii.ywan-chungtsiang.top

[U70] PHP：PDO 事务
来源：http://aut.feifeiyinyue.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://bcf.sysykeji.top

[U71] PHP：抛出异常
来源：http://ooq.hnxiangtu.top

throw new RuntimeException("失败", 500);
来源：http://pjy.sysykeji.top

[U72] PHP：写错误日志
来源：http://vdk.shangyingyoupin.top

error_log("失败: " . $e->getMessage());
来源：http://qnz.pycfn.com

[U73] PHP：读取 ini 配置
来源：http://rdb.jinghuilouyu.cn

parse_ini_file("config.ini", true)
来源：http://sjc.hammf.cn

[U74] PHP：读取环境变量
来源：http://oqx.birdmap.top

getenv("APP_ENV") ?: "production"
来源：http://owp.hesvh.cn

[U75] PHP：依赖注入
来源：http://rhk.daria6918.cn

composer require psr/container
来源：http://jzg.ywan-chungtsiang.top

[U76] PHP：简单路由
来源：http://lhi.fktsv.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://oup.yonumen.top

[U77] PHP：模板渲染
来源：http://luv.9152youxi.cn

composer require twig/twig
来源：http://ika.tanke756.top

[U78] PHP：单元测试
来源：http://yvk.cqqwz.cn

composer require --dev phpunit/phpunit
来源：http://sky.mhx1999.top

[U79] PHP：静态分析
来源：http://eep.xuetiantiany.cn

composer require --dev phpstan/phpstan
来源：http://xde.quarkkingdee.top

[U80] PHP：代码规范修复
来源：http://dhm.daxiang520.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://uyt.snrcjt.cn

[U81] JS：初始化项目
来源：http://cxo.zhongyouzk.top

npm init -y;  npm i express
来源：http://dgx.yongpay.top

[U82] JS：package.json 脚本
来源：http://ptz.ydzc1.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://uyq.aibaodan.cn

[U83] JS：ES Module 导入导出
来源：http://mvs.yfazqb.com

export const a = 1;  import { a } from "./m.js";
来源：http://ozd.chenlongwang.top

[U84] JS：CommonJS 写法
来源：http://hxo.sjlbkw.cn

module.exports = { a };  const { a } = require("./m");
来源：http://rxs.ybcxt.top

[U85] JS：可选链
来源：http://yhj.jinyuanbaomall.cn

a?.b?.c
来源：http://ohb.shanyushiyangkeji.top

[U86] JS：空值合并
来源：http://byd.yuxming.cn

a ?? b
来源：http://jgz.meibo888.top

[U87] JS：解构默认值
来源：http://qci.jinqigfzy.top

const { a = 1, b = 2 } = obj;
来源：http://wmx.xylfe.cn

[U88] JS：对象展开合并
来源：http://qqf.zdbjq.cn

{ ...a, ...b }
来源：http://ftr.hfpthk.cn

[U89] JS：数组去重
来源：http://xqm.zdqjudy.top

[...new Set(arr)]
来源：http://dsv.gzhubu.top

[U90] JS：数字数组排序
来源：http://iqw.yj20258888.top

[...arr].sort((a, b) => a - b)
来源：http://goh.chenjidiqi.icu

[U91] JS：对象键值遍历
来源：http://twn.dianchejie.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://ewk.yueranfly.top

[U92] JS：深拷贝
来源：http://hae.chenjidiqi.icu

structuredClone(obj)
来源：http://jms.zhixingplan.top

[U93] JS：模板字符串
来源：http://blb.jqgfzy.top

`共 ${n} 条`
来源：http://arr.cqqwz.cn

[U94] JS：箭头函数
来源：http://rmh.xinyue.icu

const double = x => x * 2;
来源：http://jbg.jiagoushi.top

[U95] JS：Promise 包装
来源：http://gjt.epnwcf.com

new Promise((resolve, reject) => {})
来源：http://gsh.bjfxy.top

[U96] JS：async/await 与异常
来源：http://pbb.andypj.xyz

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://ulx.redwolf501.top

[U97] JS：并发请求
来源：http://wlx.sysykeji.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://mkx.hesvh.cn

[U98] JS：fetch 带 JSON
来源：http://pjw.chenzaomai.com

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://xop.chenzaomai.com

[U99] JS：事件监听
来源：http://jbh.ywan-chungtsiang.top

el.addEventListener("click", e => {})
来源：http://wqg.smart0.xyz

[U100] JS：DOM 查询
来源：http://dlm.bbcook.cn

document.querySelector(".item")
来源：http://zqn.zhijiandao.cn

[U101] JS：classList 操作
来源：http://czg.dianchejie.cn

el.classList.toggle("active")
来源：http://wmz.cashguo.top

[U102] JS：本地存储
来源：http://bii.hfpthk.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://umd.shanyushiyangkeji.top

[U103] JS：定时器
来源：http://ott.xuanzx.com

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://yft.wangdashe.top

[U104] JS：防抖
来源：http://zfe.fktsv.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://kan.xylfe.cn

[U105] JS：节流
来源：http://pvv.aizwys.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://acm.ppjwa.cn

[U106] JS：日期格式化
来源：http://jsc.sufxvd.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://vlm.yuxming.cn

[U107] JS：数字千分位
来源：http://qhb.fehbvm.com

new Intl.NumberFormat("en-US").format(1234567)
来源：http://kqw.hesvh.cn

[U108] JS：随机整数
来源：http://anp.daxiang520.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://ywb.wangdashe.top

[U109] JS：数组分组
来源：http://aex.haohaochexian.top

Object.groupBy(arr, x => x.type)
来源：http://rfk.ywan-chungtsiang.top

[U110] JS：数组分块
来源：http://cla.shanyushiyangtech.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hto.zdqjudy.top

[U111] JS：对象转 Map
来源：http://hwi.nanxuanxn.top

new Map(Object.entries(obj))
来源：http://bwm.kuanghao11.cn

[U112] JS：字符串补位
来源：http://tjm.feifeiyinyue.top

"7".padStart(3, "0")
来源：http://uoh.fktsv.cn

[U113] JS：正则替换全部
来源：http://woi.hammf.cn

s.replaceAll("a", "b")
来源：http://ouo.jiagoushi.top

[U114] JS：JSON 深比较
来源：http://juv.hnqzz.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://sxx.xylfe.cn

[U115] JS：生成 UUID
来源：http://gbw.bbcook.cn

crypto.randomUUID()
来源：http://vte.fengsongda.top

[U116] JS：类型检查（JSDoc）
来源：http://fae.tianlin.xyz

/** @param {string} name */ function f(name) {}
来源：http://nyh.vehdjk.com

[U117] JS：单元测试
来源：http://oww.chenjidiqi.icu

npm i -D vitest;  npx vitest
来源：http://mpj.bjfxy.top

[U118] JS：开发服务器
来源：http://ohg.yvedp.cn

npm i -D vite;  npx vite
来源：http://rqh.gotoacloud.top

[U119] JS：生产构建
来源：http://vkt.shangyingyoupin.top

npx vite build
来源：http://iyt.jinyuanbaomall.cn

[U120] JS：读取环境变量（Vite）
来源：http://caj.guowangkeji.top

import.meta.env.VITE_API_URL
来源：http://jzj.uphjek.com

================================================================================
来源：http://vdw.fktsv.cn

统计汇总
来源：http://mmb.sysykeji.top

================================================================================
来源：http://dxe.daria6918.cn

按语言统计（条）：
来源：http://fou.nanxinkj.top

Python ......... 252
来源：http://qou.yfazqb.com

PHP ............ 252
来源：http://hvh.jinghuilouyu.cn

JavaScript ..... 252
来源：http://ukv.ydjk.org.cn

TypeScript ..... 212
来源：http://sna.jiagoushi.top

Java ........... 212
来源：http://fto.xziqi.cn

Go ............. 212
来源：http://qxc.cucudq.cn

Ruby ........... 212
来源：http://vsh.fengsongda.top

C# ............. 212
来源：http://jad.tian-w.cn

C .............. 30
来源：http://hjh.haohaochexian.top

C++ ............ 30
来源：http://hga.zhongyouzk.top

SQL ............ 90
来源：http://snn.epnwcf.com

Bash ........... 80
来源：http://uvu.yj202588.top

Kotlin ......... 15
来源：http://fiw.jinghuilouyu.cn

Swift .......... 15
来源：http://vfo.guannengcc.top

Lua ............ 10
来源：http://deb.uphjek.com

Perl ........... 10
来源：http://abk.dashuyun.cn

Scala .......... 10
来源：http://vgn.hfpthk.cn

------------------------------------
来源：http://frz.uphjek.com

合计 ........... 2106 条
来源：http://xru.andypj.xyz

按章节统计：
来源：http://aak.zdbjq.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://kul.hywenlv.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://xpn.52xcode.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://dgv.xziqi.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://dad.shzxlz.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://yes.shanyushiyangtech.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://nfr.aibaodan.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://wdw.hcnkem.com

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://yfq.gogol.net.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://clm.zhoulong.xyz

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://ywp.316326.xyz

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://yfn.zhengqikj.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://wng.xinyue.icu

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://azp.yongpay.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://miw.shanyushiyangkeji.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://jmy.tian-w.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://fkw.yangfankeji.com

Q SQL 专题                              90
来源：http://ujf.yongpay.top

R Bash 专题                             80
来源：http://mib.hnqzz.top

S C / C++ 专题                          60
来源：http://mry.yongpay.top

T 其他语言补充                          60
来源：http://sfv.yj20258.top

U 高频实用片段                         120
来源：http://ven.yj20258888.top

------------------------------------
来源：http://ohk.zhiwuduotai.top

合计                                  2106 条
来源：http://qil.chenlongwang.top

--------------------------------------------------------------------------------
来源：http://xgt.ppjwa.cn

使用提醒
来源：http://goc.ydzc1.top

--------------------------------------------------------------------------------
来源：http://ddz.quarkkingdee.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://icl.guowangkeji.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://qqw.pengpengdd.cyou

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://ybb.zhengqikj.top

在旧版本上使用前请先确认语法支持情况。
来源：http://new.ywan-chungtsiang.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://zpr.zdqjudy.top

—— 文件结束 ——
来源：http://pwk.tarul.cn

================================================================================
来源：http://fwn.hnxiangtu.top

程序语言常见例子速查手册（2024 版）
来源：http://nct.316326.xyz

Common Programming Examples Cheat Book
来源：http://cah.jlsjyb.cn

================================================================================
来源：http://umu.hongshengwenyu.top


<!-- 参考信息 -->