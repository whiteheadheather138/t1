代发 wailian999

def add(a: Int, b: Int): Int = a + b
来源：http://ukz.jinyuanbaomall.cn

[T59] Scala：循环
来源：http://mkh.jianghu66.top

for (i <- 1 to 10) println(i)
来源：http://czq.bbcook.cn

[T60] Scala：折叠
来源：http://twj.jinyuanbaomall.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://crx.dashuyun.cn

================================================================================
来源：http://zqb.tarul.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://jsp.fehbvm.com

================================================================================
来源：http://xxq.sxryk.cn

[U01] Py：创建虚拟环境
来源：http://hii.uphjek.com

python -m venv .venv && source .venv/bin/activate
来源：http://dot.jinyuanbaomall.cn

[U02] Py：导出 / 安装依赖
来源：http://ybx.ehwqpu.com

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://lyj.zhixingplan.top

[U03] Py：加载 .env 配置
来源：http://ryg.dashuyun.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://voo.jqgfzy.top

[U04] Py：变量调试打印
来源：http://trk.fanxiaobao.xyz

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://zpe.nanxinkj.top

[U05] Py：列表去重且保序
来源：http://zyp.fktsv.cn

list(dict.fromkeys(arr))
来源：http://mfa.c1oappe.top

[U06] Py：合并两个字典
来源：http://qzx.yj20258.top

{**a, **b}
来源：http://kwf.daria6918.cn

[U07] Py：反转字典键值
来源：http://vbg.guannengcc.top

{v: k for k, v in d.items()}
来源：http://esx.jiagoushi.top

[U08] Py：展平二维列表
来源：http://gww.hywenlv.cn

[y for x in nested for y in x]
来源：http://gdq.ctjpmb.com

[U09] Py：字典取最大值的键
来源：http://seg.jqgufenzy.top

max(d, key=d.get)
来源：http://kjp.jinqigufen.top

[U10] Py：按值排序字典
来源：http://ktn.ppjwa.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://jpq.sysykeji.top

[U11] Py：生成器表达式
来源：http://laq.jianghu66.top

(x * 2 for x in arr)
来源：http://iew.yj202588.top

[U12] Py：取出现最多的 3 个元素
来源：http://abr.c1oappe.top

Counter(arr).most_common(3)
来源：http://jjb.xuetiantiany.cn

[U13] Py：固定长度队列
来源：http://vwa.quarkkingdee.top

deque(maxlen=10)
来源：http://bol.quarkkingdee.top

[U14] Py：分组收集到列表
来源：http://vsq.jinghuilouyu.cn

defaultdict(list)
来源：http://jqr.zhixingplan.top

[U15] Py：高精度计时
来源：http://vrm.sufxvd.cn

t = time.perf_counter()
来源：http://mll.tian-w.cn

[U16] Py：命令行参数解析
来源：http://gfl.yongpay.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://qym.yj20258888.top

[U17] Py：初始化日志
来源：http://hnu.jqgfzy.top

logging.basicConfig(level=logging.INFO)
来源：http://msi.0kj1m.cn

[U18] Py：预编译正则
来源：http://ukd.hongshengwenyu.top

pat = re.compile(r"\d+")
来源：http://jvu.birdmap.top

[U19] Py：正则替换带回调
来源：http://air.tian-w.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hyl.316326.xyz

[U20] Py：缓存函数结果
来源：http://xvx.guowangkeji.top

@functools.lru_cache(maxsize=None)
来源：http://gky.pengpengdd.cyou

[U21] Py：自定义上下文管理器
来源：http://acl.shzxlz.cn

@contextlib.contextmanager
来源：http://oln.yueranfly.top

[U22] Py：矩阵转置
来源：http://fvz.guowangkeji.top

list(zip(*m))
来源：http://qzf.ivvv.top

[U23] Py：分块读取大文件
来源：http://zsa.andypj.xyz

for chunk in iter(lambda: f.read(8192), b""):
来源：http://xqz.tianlin.xyz

[U24] Py：路径操作
来源：http://tmt.mhx1999.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://rlj.nanxinkj.top

[U25] Py：CSV 按字典读
来源：http://ial.pengpengdd.cyou

csv.DictReader(f)
来源：http://otj.andypj.xyz

[U26] Py：并发下载
来源：http://xfl.chenjidiqi.icu

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://ycu.jqgufenzy.top

[U27] Py：异步 HTTP
来源：http://twq.fktsv.cn

aiohttp.ClientSession() 配合 async with
来源：http://xri.xziqi.cn

[U28] Py：类型别名
来源：http://rdc.cashguo.top

UserId = int
来源：http://jpl.bbcook.cn

[U29] Py：属性校验
来源：http://vox.tian-w.cn

@property 与 @x.setter 配合
来源：http://yli.shanyushiyangkeji.top

[U30] Py：数据类
来源：http://ohm.uphjek.com

@dataclass(slots=True)
来源：http://ifi.hesvh.cn

[U31] Py：单测
来源：http://hoc.quarkkingdee.top

python -m pytest -q
来源：http://goh.xylfe.cn

[U32] Py：代码格式化
来源：http://yvf.316326.xyz

ruff format . && ruff check --fix .
来源：http://pdp.9152youxi.cn

[U33] Py：打包发布
来源：http://vsj.andypj.xyz

python -m build  （依赖 pyproject.toml）
来源：http://nyb.zhengqikj.top

[U34] Py：判断编码
来源：http://hdm.jinghuilouyu.cn

chardet.detect(raw)
来源：http://vbv.xinyue.icu

[U35] Py：发送邮件
来源：http://wza.hesvh.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://wgy.nwbrower.top

[U36] Py：定时任务
来源：http://zpn.daria6918.cn

schedule.every(10).minutes.do(job)
来源：http://krx.ywan-chungtsiang.top

[U37] Py：读写 Excel
来源：http://wws.shanyushiyangkeji.top

pandas.read_excel / DataFrame.to_excel
来源：http://lwy.daxiang520.top

[U38] Py：获取脚本所在目录
来源：http://sey.haohaochexian.top

Path(__file__).resolve().parent
来源：http://zsm.xinyue.icu

[U39] Py：判断是否在交互环境
来源：http://oec.quarkkingdee.top

sys.stdout.isatty()
来源：http://dqy.havefunace.top

[U40] Py：打印到标准错误
来源：http://kxn.jinghuilouyu.cn

print("err", file=sys.stderr)
来源：http://nza.xinyue.icu

[U41] PHP：初始化 Composer 项目
来源：http://oya.sjlbkw.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://wrs.sweek.top

[U42] PHP：PSR-4 自动加载
来源：http://qsb.cqqwz.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://vjd.vqdsnc.cn

[U43] PHP：声明命名空间
来源：http://ivz.fzhhl.top

namespace App\Http;
来源：http://npt.yvedp.cn

[U44] PHP：开启严格类型
来源：http://oyw.316326.xyz

declare(strict_types=1);
来源：http://eua.cqqwz.cn

[U45] PHP：类型声明与返回类型
来源：http://idy.hongshengwenyu.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://grd.zycfv.cn

[U46] PHP：可空类型
来源：http://jez.tarul.cn

?string $name = null
来源：http://ssp.nanxuanxn.top

[U47] PHP：联合类型
来源：http://fxv.jqgufenzy.top

int|string $id
来源：http://zes.yuxming.cn

[U48] PHP：纯枚举
来源：http://hvx.chenjidiqi.icu

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://khi.chenzaomai.com

[U49] PHP：只读属性
来源：http://snj.tianlin.xyz

public readonly string $name
来源：http://dvg.yuxming.cn

[U50] PHP：构造器属性提升
来源：http://kan.chenjidiqi.icu

public function __construct(private int $id) {}
来源：http://ofp.daria6918.cn

[U51] PHP：数组解构
来源：http://umc.tianlin.xyz

[$a, $b] = $arr;
来源：http://zmd.ppjwa.cn

[U52] PHP：箭头函数
来源：http://rpu.jqgfzy.top

$double = fn($x) => $x * 2;
来源：http://zcl.guowangkeji.top

[U53] PHP：空合并运算符
来源：http://gsh.dashuyun.cn

$v = $a ?? $b ?? "default";
来源：http://uqu.iojbl.cn

[U54] PHP：空安全调用
来源：http://nuk.shanyushiyangtech.top

$obj?->method()
来源：http://dlc.wangdashe.top

[U55] PHP：match 表达式
来源：http://jtg.yueranfly.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://mzw.bjfxy.top

[U56] PHP：命名参数
来源：http://jmp.yangfankeji.com

f(a: 1, b: 2)
来源：http://knn.kuanghao11.cn

[U57] PHP：字符串插值
来源：http://vbl.hnxiangtu.top

"值: {$a}"
来源：http://kev.yfazqb.com

[U58] PHP：数组三件套
来源：http://kcv.hammf.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://bbz.nwbrower.top

[U59] PHP：自定义排序
来源：http://opt.pycfn.com

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://thf.0kj1m.cn

[U60] PHP：JSON 编解码
来源：http://gcm.vqdsnc.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://emn.shuidangran.top

[U61] PHP：正则
来源：http://agb.yfazqb.com

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://ekl.yj202588.top

[U62] PHP：日期对象
来源：http://jnj.hcnkem.com

(new DateTimeImmutable())->format("Y-m-d");
来源：http://ntc.yanxiufei.cn

[U63] PHP：文件读写
来源：http://mnh.zycfv.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://gcg.hnxiangtu.top

[U64] PHP：目录遍历
来源：http://aex.chenzaomai.com

glob("dir/*.php");  scandir("dir");
来源：http://bhx.yuxming.cn

[U65] PHP：会话
来源：http://ymv.tian-w.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://amg.sufxvd.cn

[U66] PHP：设置 Cookie
来源：http://lyl.yonumen.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://mbe.ppjwa.cn

[U67] PHP：处理文件上传
来源：http://pfp.52xcode.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://okn.shanyushiyangtech.top

[U68] PHP：PDO 连接
来源：http://miu.shanyushiyangkeji.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://ndf.ydjk.org.cn

[U69] PHP：PDO 预处理
来源：http://nfc.fktsv.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hly.hesvh.cn

[U70] PHP：PDO 事务
来源：http://iru.hywenlv.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://kua.yj20258.top

[U71] PHP：抛出异常
来源：http://nxv.haohaochexian.top

throw new RuntimeException("失败", 500);
来源：http://ral.yj20258888.top

[U72] PHP：写错误日志
来源：http://kzk.0kj1m.cn

error_log("失败: " . $e->getMessage());
来源：http://jbr.guannengcc.top

[U73] PHP：读取 ini 配置
来源：http://ywq.zhengqikj.top

parse_ini_file("config.ini", true)
来源：http://vcg.xylfe.cn

[U74] PHP：读取环境变量
来源：http://ito.epnwcf.com

getenv("APP_ENV") ?: "production"
来源：http://myp.birdmap.top

[U75] PHP：依赖注入
来源：http://vti.tianlin.xyz

composer require psr/container
来源：http://twn.gotoacloud.top

[U76] PHP：简单路由
来源：http://ofj.xziqi.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://upy.dianchejie.cn

[U77] PHP：模板渲染
来源：http://pzd.yuxming.cn

composer require twig/twig
来源：http://yen.meibo888.top

[U78] PHP：单元测试
来源：http://phw.yj20258888.top

composer require --dev phpunit/phpunit
来源：http://avd.zhiwuduotai.top

[U79] PHP：静态分析
来源：http://aem.yuanzhike.top

composer require --dev phpstan/phpstan
来源：http://zub.jinqigufen.top

[U80] PHP：代码规范修复
来源：http://fjj.yj202588.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://fjp.sufxvd.cn

[U81] JS：初始化项目
来源：http://ohx.xuanzx.com

npm init -y;  npm i express
来源：http://jdx.quarkkingdee.top

[U82] JS：package.json 脚本
来源：http://zrp.gaohongyu789.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://scw.jyoumei.cn

[U83] JS：ES Module 导入导出
来源：http://law.zhoulong.xyz

export const a = 1;  import { a } from "./m.js";
来源：http://swp.sjlbkw.cn

[U84] JS：CommonJS 写法
来源：http://mfm.hongshengwenyu.top

module.exports = { a };  const { a } = require("./m");
来源：http://pju.dashuyun.cn

[U85] JS：可选链
来源：http://orx.ctjpmb.com

a?.b?.c
来源：http://lis.zycfv.cn

[U86] JS：空值合并
来源：http://hjr.kuanghao11.cn

a ?? b
来源：http://ykj.hammf.cn

[U87] JS：解构默认值
来源：http://nur.xuetiantiany.cn

const { a = 1, b = 2 } = obj;
来源：http://bmb.yj20258.top

[U88] JS：对象展开合并
来源：http://itu.xingfuxueyuan.xyz

{ ...a, ...b }
来源：http://qbx.shanyushiyangkeji.top

[U89] JS：数组去重
来源：http://qyn.chenjidiqi.icu

[...new Set(arr)]
来源：http://esv.hesvh.cn

[U90] JS：数字数组排序
来源：http://owc.yangfankeji.com

[...arr].sort((a, b) => a - b)
来源：http://fes.daria6918.cn

[U91] JS：对象键值遍历
来源：http://zzv.pengpengdd.cyou

Object.entries(obj).forEach(([k, v]) => {});
来源：http://ecg.shangyingyoupin.top

[U92] JS：深拷贝
来源：http://lbo.jinyuanbaomall.cn

structuredClone(obj)
来源：http://nss.yfazqb.com

[U93] JS：模板字符串
来源：http://pci.daria6918.cn

`共 ${n} 条`
来源：http://mjw.jianghu66.top

[U94] JS：箭头函数
来源：http://dzt.cheryme.top

const double = x => x * 2;
来源：http://pbf.uphjek.com

[U95] JS：Promise 包装
来源：http://itt.yj20258.top

new Promise((resolve, reject) => {})
来源：http://zdt.zdqjudy.top

[U96] JS：async/await 与异常
来源：http://iie.haohaochexian.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://tpj.fktsv.cn

[U97] JS：并发请求
来源：http://yqi.ydzc1.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://dzk.birdmap.top

[U98] JS：fetch 带 JSON
来源：http://ytq.ivvv.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://gay.hongshengwenyu.top

[U99] JS：事件监听
来源：http://gxw.0kj1m.cn

el.addEventListener("click", e => {})
来源：http://lfw.hfpthk.cn

[U100] JS：DOM 查询
来源：http://luu.pycfn.com

document.querySelector(".item")
来源：http://vko.hnqzz.top

[U101] JS：classList 操作
来源：http://ggx.hywenlv.cn

el.classList.toggle("active")
来源：http://xkp.iojbl.cn

[U102] JS：本地存储
来源：http://nte.quarkkingdee.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://vel.iojbl.cn

[U103] JS：定时器
来源：http://cjh.xinyue.icu

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://zkm.sjlbkw.cn

[U104] JS：防抖
来源：http://jly.ctjpmb.com

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://rht.vehdjk.com

[U105] JS：节流
来源：http://mca.zhiwuduotai.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://wlr.epnwcf.com

[U106] JS：日期格式化
来源：http://vgh.ybcxt.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://sft.jinyuanbaomall.cn

[U107] JS：数字千分位
来源：http://cnu.yanxiufei.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://rmu.sjlbkw.cn

[U108] JS：随机整数
来源：http://qem.ehwqpu.com

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://zhn.bbcook.cn

[U109] JS：数组分组
来源：http://tsd.tianlin.xyz

Object.groupBy(arr, x => x.type)
来源：http://uok.pengpengdd.cyou

[U110] JS：数组分块
来源：http://wjk.316326.xyz

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://vtc.yj202588.top

[U111] JS：对象转 Map
来源：http://mxc.xuanzx.com

new Map(Object.entries(obj))
来源：http://okv.nanxinkj.top

[U112] JS：字符串补位
来源：http://bxl.sysykeji.top

"7".padStart(3, "0")
来源：http://cmd.tian-w.cn

[U113] JS：正则替换全部
来源：http://ckv.9152youxi.cn

s.replaceAll("a", "b")
来源：http://ofy.hywenlv.cn

[U114] JS：JSON 深比较
来源：http://ija.hfpthk.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://oam.shanyushiyangtech.top

[U115] JS：生成 UUID
来源：http://okk.shzxlz.cn

crypto.randomUUID()
来源：http://lbt.hywenlv.cn

[U116] JS：类型检查（JSDoc）
来源：http://aga.wangdashe.top

/** @param {string} name */ function f(name) {}
来源：http://tbe.nanxinkj.top

[U117] JS：单元测试
来源：http://vrt.c1oappe.top

npm i -D vitest;  npx vitest
来源：http://cld.gzhubu.top

[U118] JS：开发服务器
来源：http://mtc.cheryme.top

npm i -D vite;  npx vite
来源：http://uhz.cheryme.top

[U119] JS：生产构建
来源：http://lbq.sufxvd.cn

npx vite build
来源：http://imn.zdbjq.cn

[U120] JS：读取环境变量（Vite）
来源：http://bhj.hammf.cn

import.meta.env.VITE_API_URL
来源：http://mcb.yongpay.top

================================================================================
来源：http://rsw.ehwqpu.com

统计汇总
来源：http://han.svipenyu.cn

================================================================================
来源：http://thm.xuetiantiany.cn

按语言统计（条）：
来源：http://opn.hfpthk.cn

Python ......... 252
来源：http://ttc.cdnleiting.top

PHP ............ 252
来源：http://xfb.9152youxi.cn

JavaScript ..... 252
来源：http://znb.yvedp.cn

TypeScript ..... 212
来源：http://xst.uphjek.com

Java ........... 212
来源：http://dll.mhx1999.top

Go ............. 212
来源：http://eeu.yangfankeji.com

Ruby ........... 212
来源：http://vds.gaohongyu789.top

C# ............. 212
来源：http://xxh.yongpay.top

C .............. 30
来源：http://qln.ydjk.org.cn

C++ ............ 30
来源：http://fry.kuanghao11.cn

SQL ............ 90
来源：http://rvn.bbcook.cn

Bash ........... 80
来源：http://bgq.hnqzz.top

Kotlin ......... 15
来源：http://gbb.xuetiantiany.cn

Swift .......... 15
来源：http://ehd.fzhhl.top

Lua ............ 10
来源：http://doa.vqdsnc.cn

Perl ........... 10
来源：http://oqm.svipenyu.cn

Scala .......... 10
来源：http://lup.ivvv.top

------------------------------------
来源：http://tpl.jqgfzy.top

合计 ........... 2106 条
来源：http://qwq.aibaodan.cn

按章节统计：
来源：http://vvp.quarkkingdee.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://qpr.zdqjudy.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://pst.hysaishi.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://ulv.jinqigufen.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://xwt.jinqigufen.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hlt.wangdashe.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://spq.hcnkem.com

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://ghb.cheryme.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://oxa.guowangkeji.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://jvj.52xcode.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://uow.ywan-chungtsiang.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://odl.sufxvd.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://emm.gotoacloud.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://vzv.yj202588.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://xrs.yongpay.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://yhz.hfpthk.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://ict.ivvv.top

Q SQL 专题                              90
来源：http://onu.jinqigufen.top

R Bash 专题                             80
来源：http://zsb.xingfuxueyuan.xyz

S C / C++ 专题                          60
来源：http://ncn.kuanghao11.cn

T 其他语言补充                          60
来源：http://dzq.hammf.cn

U 高频实用片段                         120
来源：http://ybg.dashuyun.cn

------------------------------------
来源：http://dio.yvedp.cn

合计                                  2106 条
来源：http://mkl.wangdashe.top

--------------------------------------------------------------------------------
来源：http://huj.hongshengwenyu.top

使用提醒
来源：http://eyb.gogol.net.cn

--------------------------------------------------------------------------------
来源：http://yrj.cdnleiting.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://sbj.chenzaomai.com

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://esk.andypj.xyz


<!-- 参考信息 -->