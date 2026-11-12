代发 wailian999

[B13] 判断是否为数字
来源：http://mdd.hnqzz.top

Py:   isinstance(x, (int, float))
来源：http://soc.yvedp.cn

PHP:  is_numeric($x)
来源：http://lfc.dashuyun.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://gbd.zhengqikj.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://vmr.jianghu66.top

Java: x instanceof Number
来源：http://cnr.zdqjudy.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://fdm.jiagoushi.top

Ruby: x.is_a?(Numeric)
来源：http://hks.iojbl.cn

C#:   x is int or double or decimal
来源：http://lgx.sufxvd.cn

[B14] 判断值是否在集合内
来源：http://tkp.smart0.xyz

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://jmm.yongpay.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://fkh.xuetiantiany.cn

JS:   [1, 2, 3].includes(x)
来源：http://csf.birdmap.top

TS:   [1, 2, 3].includes(x)
来源：http://tsf.jinyuanbaomall.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://xyh.feifeiyinyue.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://abu.shzxlz.cn

Ruby: [1, 2, 3].include?(x)
来源：http://ncb.yangfankeji.com

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://paj.fzhhl.top

[B15] 布尔运算与取反
来源：http://qiv.cucudq.cn

Py:   a and b or not c
来源：http://kpw.pycfn.com

PHP:  $a && $b || !$c
来源：http://kik.feifeiyinyue.top

JS:   a && b || !c
来源：http://jfb.ydzc1.top

TS:   a && b || !c
来源：http://how.yueranfly.top

Java: a && b || !c
来源：http://qha.kuanghao11.cn

Go:   a && b || !c
来源：http://khm.jinghuilouyu.cn

Ruby: a && b || !c
来源：http://ncj.meibo888.top

C#:   a && b || !c
来源：http://taq.kuanghao11.cn

[B16] 卫语句：不满足条件提前返回
来源：http://uvs.ehwqpu.com

Py:   if not data: return
来源：http://dhb.zhiwuduotai.top

PHP:  if (!$data) { return; }
来源：http://rzl.havefunace.top

JS:   if (!data) return;
来源：http://ygy.xingfuxueyuan.xyz

TS:   if (!data) return;
来源：http://ntz.sxryk.cn

Java: if (data == null) return;
来源：http://xpm.xingfuxueyuan.xyz

Go:   if data == nil { return }
来源：http://crj.9152youxi.cn

Ruby: return if data.nil?
来源：http://iqa.fehbvm.com

C#:   if (data == null) return;
来源：http://fof.wangdashe.top

================================================================================
来源：http://iri.yvedp.cn

C. 函数与作用域
来源：http://sme.gzhubu.top

================================================================================
来源：http://uxn.ydjk.org.cn

[C01] 定义函数
来源：http://wxz.ivvv.top

Py:   def add(a, b): return a + b
来源：http://ahr.fehbvm.com

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://pim.svipenyu.cn

JS:   function add(a, b) { return a + b; }
来源：http://zxw.ehwqpu.com

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://odi.gaohongyu789.top

Java: static int add(int a, int b) { return a + b; }
来源：http://anr.zdqjudy.top

Go:   func add(a, b int) int { return a + b }
来源：http://zzv.ctjpmb.com

Ruby: def add(a, b); a + b; end
来源：http://luy.hnxiangtu.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://wak.pengpengdd.cyou

[C02] 默认参数
来源：http://cua.fengsongda.top

Py:   def greet(name="World"): return name
来源：http://zim.vqdsnc.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://fgl.chenzaomai.com

JS:   function greet(name = "World") { return name; }
来源：http://hjs.bbcook.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://ivm.ydzc1.top

Java: // 无默认参数：方法重载或 Optional
来源：http://jim.aizwys.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://pgk.pycfn.com

Ruby: def greet(name = "World") = name
来源：http://iip.nwbrower.top

C#:   string Greet(string name = "World") => name;
来源：http://ndr.hammf.cn

[C03] 可变参数
来源：http://uyc.vehdjk.com

Py:   def total(*args): return sum(args)
来源：http://npv.yongpay.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://yku.chenzaomai.com

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://cil.vqdsnc.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hds.jyoumei.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://kro.chenzaomai.com

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://yjd.0kj1m.cn

Ruby: def total(*nums); nums.sum; end
来源：http://asj.gzhubu.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://xhs.xziqi.cn

[C04] 命名参数 / 关键字参数
来源：http://smu.tarul.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://dhg.hnxiangtu.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://anw.aizwys.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://faf.yfazqb.com

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://fqe.jyoumei.cn

Java: // 无：用 Builder 模式或 record
来源：http://qqi.andypj.xyz

Go:   // 无：用配置结构体参数
来源：http://vdk.zdbjq.cn

Ruby: f(a: 1, b: 2)
来源：http://rbp.xylfe.cn

C#:   f(a: 1, b: 2)
来源：http://uql.hnxiangtu.top

[C05] 返回多个值
来源：http://wtf.svipenyu.cn

Py:   return a, b
来源：http://oow.cucudq.cn

PHP:  return [$a, $b];
来源：http://gvh.chenlongwang.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://bxp.ehwqpu.com

TS:   return { a, b };
来源：http://pyn.andypj.xyz

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://wal.hnxiangtu.top

Go:   return a, b
来源：http://qoq.chenzaomai.com

Ruby: return a, b
来源：http://zvn.wangshuangyany.cn

C#:   return (a, b);              // ValueTuple
来源：http://cpa.hnxiangtu.top

[C06] 匿名函数 / lambda
来源：http://bkn.feifeiyinyue.top

Py:   square = lambda x: x * x
来源：http://qyj.hnqzz.top

PHP:  $square = fn($x) => $x * $x;
来源：http://rva.uphjek.com

JS:   const square = x => x * x;
来源：http://tin.iojbl.cn

TS:   const square = (x: number): number => x * x;
来源：http://qfl.yfazqb.com

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://pln.nanxuanxn.top

Go:   sq := func(x int) int { return x * x }
来源：http://vug.daria6918.cn

Ruby: square = ->(x) { x * x }
来源：http://dfl.zycfv.cn

C#:   Func<int, int> square = x => x * x;
来源：http://ltu.pengpengdd.cyou

[C07] 把函数作为参数传入
来源：http://bee.ivvv.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://iec.zdqjudy.top

PHP:  array_map("strtoupper", $arr);
来源：http://jyr.zhengqikj.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://iby.tian-w.cn

TS:   arr.map(String)
来源：http://klj.jlsjyb.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://exo.sufxvd.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hne.nanxinkj.top

Ruby: arr.map(&:upcase)
来源：http://jwt.yj20258888.top

C#:   arr.Select(s => s.ToUpper())
来源：http://laz.iojbl.cn

[C08] 闭包
来源：http://kkv.mhx1999.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://crk.uphjek.com

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://bbx.haohaochexian.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://xmr.iojbl.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://ywk.daria6918.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://fat.meibo888.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://vfy.chenjidiqi.icu

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://ewh.vqdsnc.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://xuh.hongshengwenyu.top

[C09] 递归
来源：http://uaw.gotoacloud.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://bbm.yfazqb.com

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://ino.yueranfly.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hzl.yonumen.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://qeq.jiagoushi.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://pyw.chenlongwang.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://vvt.guannengcc.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://ekg.gaohongyu789.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://vnf.52xcode.cn

[C10] 变量作用域
来源：http://tne.sjlbkw.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://bpe.ywan-chungtsiang.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://uah.ctjpmb.com

JS:   let/const 块级作用域，var 函数级作用域
来源：http://zos.iojbl.cn

TS:   同 JS
来源：http://mwm.52xcode.cn

Java: 方法内为块级作用域
来源：http://yrl.tian-w.cn

Go:   花括号块级作用域
来源：http://vgu.guowangkeji.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://oik.gzhubu.top

C#:   块级作用域
来源：http://msz.yj202588.top

[C11] 模块导入与导出
来源：http://mda.yueranfly.top

Py:   from module import func
来源：http://pif.ydjk.org.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://pvk.ctjpmb.com

JS:   export default function f() {};  import f from "./m.js";
来源：http://muy.jinyuanbaomall.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://msr.tanke756.top

Java: import java.util.List;
来源：http://ufw.fehbvm.com

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://plf.c1oappe.top

Ruby: require "json"; require_relative "./util"
来源：http://ixk.guowangkeji.top

C#:   using System.Text;
来源：http://beo.tarul.cn

[C12] 立即执行函数 IIFE
来源：http://ueg.zhaomingkeji.xyz

Py:   (lambda: print("run"))()
来源：http://boa.hywenlv.cn

PHP:  (function () { echo "run"; })();
来源：http://qgc.jiagoushi.top

JS:   (() => { console.log("run"); })();
来源：http://mfj.smart0.xyz

TS:   (() => { console.log("run"); })();
来源：http://wud.shuidangran.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://tfa.ywan-chungtsiang.top

Go:   func() { fmt.Println("run") }()
来源：http://zkj.jqgfzy.top

Ruby: -> { puts "run" }.call
来源：http://yas.ywan-chungtsiang.top

C#:   // 无 IIFE：用静态构造函数
来源：http://jgk.mhx1999.top

[C13] 类型声明 / 类型注解
来源：http://bpy.zycfv.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://nyu.epnwcf.com

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://xki.chenzaomai.com

JS:   // 无类型（可用 JSDoc 注释）
来源：http://ixh.haohaochexian.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wuc.shanyushiyangkeji.top

Java: int add(int a, int b) { return a + b; }
来源：http://xfn.yj20258888.top

Go:   func add(a, b int) int
来源：http://eef.ivvv.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://ztr.shanyushiyangtech.top

C#:   int Add(int a, int b) => a + b;
来源：http://puu.chenjidiqi.icu

[C14] 泛型函数
来源：http://aaw.yj20258888.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://xwa.shuidangran.top

PHP:  // 无泛型
来源：http://lei.sysykeji.top

JS:   // 无泛型
来源：http://zip.tianlin.xyz

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://sux.xuetiantiany.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://ugr.ybcxt.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://bvl.tanke756.top

Ruby: # 无泛型
来源：http://qea.sysykeji.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://lwr.nanxinkj.top

[C15] 解构 / 展开参数
来源：http://zts.jianghu66.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://ujj.chenlongwang.top

PHP:  [$a, $b] = $pair;
来源：http://ray.uphjek.com

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://dms.hysaishi.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://amv.haohaochexian.top

Java: // 无解构
来源：http://hnn.xinyue.icu

Go:   // 无解构
来源：http://ezn.gotoacloud.top

Ruby: a, b = pair
来源：http://fxd.ppjwa.cn

C#:   var (a, b) = pair;
来源：http://icu.sweek.top

[C16] 函数 / 方法重载
来源：http://urp.quarkkingdee.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://dis.hesvh.cn

PHP:  // 无重载
来源：http://bzc.yueranfly.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://fkg.dashuyun.cn

TS:   // 用联合类型或重载签名声明
来源：http://tgx.ctjpmb.com

Java: void f(int a) {}  void f(String a) {}
来源：http://xpm.xuanzx.com

Go:   // 无重载：用不同函数名
来源：http://xsu.ehwqpu.com

Ruby: # 无重载：靠动态参数
来源：http://zvv.shangyingyoupin.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://nth.shanyushiyangtech.top

================================================================================
来源：http://znp.shangyingyoupin.top

D. 数组 / 列表 / 集合
来源：http://nkr.sysykeji.top

================================================================================
来源：http://erq.smart0.xyz

[D01] 创建数组 / 列表
来源：http://yyh.tanke756.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://lso.xingfuxueyuan.xyz

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://znl.daxiang520.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://sdb.sjlbkw.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://rgi.zycfv.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://wtp.sweek.top

Go:   arr := []int{1, 2, 3}
来源：http://yws.sysykeji.top

Ruby: arr = [1, 2, 3]
来源：http://xqb.ybcxt.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://ahr.gogol.net.cn

[D02] 追加元素到末尾
来源：http://rha.nanxinkj.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://kfj.316326.xyz

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://rbv.9152youxi.cn

JS:   arr.push(4);
来源：http://jci.feifeiyinyue.top

TS:   arr.push(4);
来源：http://rew.kuanghao11.cn

Java: list.add(4);
来源：http://djs.pengpengdd.cyou

Go:   arr = append(arr, 4)
来源：http://eif.0kj1m.cn

Ruby: arr << 4; arr.push(5)
来源：http://cof.yuanzhike.top

C#:   list.Add(4);
来源：http://knw.aibaodan.cn

[D03] 在指定位置插入元素
来源：http://sxk.jinqigfzy.top

Py:   arr.insert(0, 0)
来源：http://wxw.xingfuxueyuan.xyz

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://aqo.yonumen.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://krx.cheryme.top

TS:   arr.splice(0, 0, 0);
来源：http://myf.yanxiufei.cn

Java: list.add(0, 0);
来源：http://xdu.nanxinkj.top

Go:   arr = append([]int{0}, arr...)
来源：http://aun.wangdashe.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://bjg.gaohongyu789.top

C#:   list.Insert(0, 0);
来源：http://ris.shangyingyoupin.top

[D04] 删除元素
来源：http://abw.yonumen.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://rnc.hongshengwenyu.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://cbj.fengsongda.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://acb.nanxinkj.top

TS:   arr.splice(0, 1);
来源：http://ldv.0kj1m.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://cke.gogol.net.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://lsw.xingfuxueyuan.xyz

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://vnv.ybcxt.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://bwx.sufxvd.cn

[D05] 访问与修改元素
来源：http://lum.yonumen.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://wsr.ybcxt.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://bik.gotoacloud.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://tvv.yonumen.top

TS:   arr[0]; arr.at(-1);
来源：http://kyc.ydjk.org.cn

Java: list.get(0); list.set(0, 9);
来源：http://unp.tianlin.xyz

Go:   arr[0]; arr[0] = 9
来源：http://qye.jinghuilouyu.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://xup.wangshuangyany.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://ywv.hnqzz.top

[D06] 数组长度
来源：http://qyo.ivvv.top

Py:   len(arr)
来源：http://fwm.tarul.cn

PHP:  count($arr);
来源：http://xch.ydzc1.top

JS:   arr.length
来源：http://gvb.pycfn.com

TS:   arr.length
来源：http://flc.daxiang520.top

Java: list.size();
来源：http://ezm.iojbl.cn

Go:   len(arr)
来源：http://vtt.zhiwuduotai.top

Ruby: arr.length; arr.size
来源：http://qtz.vehdjk.com

C#:   list.Count;
来源：http://zqc.vqdsnc.cn

[D07] 切片 / 取子数组
来源：http://xyc.ctjpmb.com

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://nin.zhijiandao.cn

PHP:  array_slice($arr, 1, 3);
来源：http://slv.redwolf501.top

JS:   arr.slice(1, 4);
来源：http://hrm.xinyue.icu

TS:   arr.slice(1, 4);
来源：http://lrn.xuanzx.com

Java: list.subList(1, 4);
来源：http://bim.wangdashe.top

Go:   arr[1:4]
来源：http://gcb.jinghuilouyu.cn

Ruby: arr[1, 3]
来源：http://knb.cqqwz.cn

C#:   list.GetRange(1, 3);
来源：http://fga.ppjwa.cn

[D08] 合并两个数组
来源：http://eqv.ehwqpu.com

Py:   a + b;  a.extend(b)
来源：http://vmq.sjlbkw.cn

PHP:  array_merge($a, $b);
来源：http://son.jianghu66.top

JS:   [...a, ...b];  a.concat(b);
来源：http://xxq.jinyuanbaomall.cn

TS:   [...a, ...b];
来源：http://zmn.fzhhl.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://sqp.bjfxy.top

Go:   append(a, b...)
来源：http://vnw.nwbrower.top

Ruby: a + b;  a.concat(b)
来源：http://mxs.nanxuanxn.top

C#:   a.Concat(b).ToList()
来源：http://biq.zdbjq.cn

[D09] 排序（升序）
来源：http://csk.tianlin.xyz

Py:   sorted(arr);  arr.sort()
来源：http://zdy.kuanghao11.cn

PHP:  sort($arr);
来源：http://rdm.zycfv.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://lgy.0kj1m.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://fyo.bbcook.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://dvf.nanxinkj.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://xwz.yanxiufei.cn

Ruby: arr.sort
来源：http://zeh.redwolf501.top

C#:   list.Sort();
来源：http://wwf.zdqjudy.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://zof.daria6918.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://vdd.hnxiangtu.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://rwj.ppjwa.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://keh.jlsjyb.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://ari.guannengcc.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://qoq.316326.xyz

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://apt.52xcode.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://dkz.daxiang520.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://uif.chenzaomai.com

[D11] 反转数组
来源：http://umw.zhixingplan.top

Py:   arr[::-1];  arr.reverse()
来源：http://neu.gaohongyu789.top

PHP:  array_reverse($arr);
来源：http://kak.tarul.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://nqh.meibo888.top

TS:   [...arr].reverse();
来源：http://tvz.vqdsnc.cn

Java: Collections.reverse(list);
来源：http://hsp.meibo888.top

Go:   slices.Reverse(arr)
来源：http://puj.hnqzz.top

Ruby: arr.reverse
来源：http://ybx.zhoulong.xyz

C#:   list.Reverse();
来源：http://vsg.shangyingyoupin.top

[D12] 查找元素下标
来源：http://wsi.cdnleiting.top

Py:   arr.index(x);  x in arr
来源：http://dzv.shanyushiyangtech.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hbn.andypj.xyz

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://gmo.tanke756.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://igv.cheryme.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://ocs.yueranfly.top

Go:   slices.Index(arr, x)
来源：http://wsy.jinqigufen.top

Ruby: arr.index(x)
来源：http://xne.ywan-chungtsiang.top

C#:   list.IndexOf(x);
来源：http://tks.birdmap.top

[D13] 过滤（保留满足条件的）
来源：http://sgt.pycfn.com

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://xjl.havefunace.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://idc.yonumen.top

JS:   arr.filter(x => x > 3)
来源：http://bqt.iojbl.cn

TS:   arr.filter(x => x > 3)
来源：http://zlo.xuetiantiany.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://drk.fzhhl.top


<!-- 参考信息 -->