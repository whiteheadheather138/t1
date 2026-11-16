代发 wailian999

JS:   [1, 2, 3].includes(x)
来源：http://moh.9152youxi.cn

TS:   [1, 2, 3].includes(x)
来源：http://dvl.zhoulong.xyz

Java: List.of(1, 2, 3).contains(x)
来源：http://xmx.yvedp.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://dey.ppjwa.cn

Ruby: [1, 2, 3].include?(x)
来源：http://ejz.yuanzhike.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://rsl.daxiang520.top

[B15] 布尔运算与取反
来源：http://gtj.yongpay.top

Py:   a and b or not c
来源：http://qen.chenjidiqi.icu

PHP:  $a && $b || !$c
来源：http://byk.yvedp.cn

JS:   a && b || !c
来源：http://hcc.xingfuxueyuan.xyz

TS:   a && b || !c
来源：http://pnp.zhengqikj.top

Java: a && b || !c
来源：http://zty.dianchejie.cn

Go:   a && b || !c
来源：http://tpc.tanke756.top

Ruby: a && b || !c
来源：http://pva.svipenyu.cn

C#:   a && b || !c
来源：http://dli.vehdjk.com

[B16] 卫语句：不满足条件提前返回
来源：http://rvq.zdqjudy.top

Py:   if not data: return
来源：http://waq.wangshuangyany.cn

PHP:  if (!$data) { return; }
来源：http://zpx.jinqigfzy.top

JS:   if (!data) return;
来源：http://lfm.mhx1999.top

TS:   if (!data) return;
来源：http://phk.cheryme.top

Java: if (data == null) return;
来源：http://ycp.hysaishi.cn

Go:   if data == nil { return }
来源：http://upe.fktsv.cn

Ruby: return if data.nil?
来源：http://jox.chenzaomai.com

C#:   if (data == null) return;
来源：http://uwa.wangdashe.top

================================================================================
来源：http://lha.kuanghao11.cn

C. 函数与作用域
来源：http://rug.nanxinkj.top

================================================================================
来源：http://ohq.c1oappe.top

[C01] 定义函数
来源：http://lle.ydzc1.top

Py:   def add(a, b): return a + b
来源：http://jao.jiagoushi.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://dar.dianchejie.cn

JS:   function add(a, b) { return a + b; }
来源：http://ymz.chenlongwang.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://cmi.yanxiufei.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://rkw.daria6918.cn

Go:   func add(a, b int) int { return a + b }
来源：http://ccp.ehwqpu.com

Ruby: def add(a, b); a + b; end
来源：http://akg.redwolf501.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://sqe.shanyushiyangtech.top

[C02] 默认参数
来源：http://ohj.fanxiaobao.xyz

Py:   def greet(name="World"): return name
来源：http://svj.xinyue.icu

PHP:  function greet($name = "World") { return $name; }
来源：http://ccc.ydjk.org.cn

JS:   function greet(name = "World") { return name; }
来源：http://lar.zycfv.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://hus.xinyue.icu

Java: // 无默认参数：方法重载或 Optional
来源：http://nea.zhixingplan.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://nsq.iojbl.cn

Ruby: def greet(name = "World") = name
来源：http://vyu.cheryme.top

C#:   string Greet(string name = "World") => name;
来源：http://cll.pycfn.com

[C03] 可变参数
来源：http://wrv.xylfe.cn

Py:   def total(*args): return sum(args)
来源：http://uuf.hysaishi.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://fxh.shangyingyoupin.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://ppp.shzxlz.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://xca.sufxvd.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://vwa.hesvh.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://juv.0kj1m.cn

Ruby: def total(*nums); nums.sum; end
来源：http://cgq.gogol.net.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://zzl.52xcode.cn

[C04] 命名参数 / 关键字参数
来源：http://lqy.jinqigfzy.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://ger.xuetiantiany.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://lmp.shanyushiyangkeji.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://dqf.redwolf501.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://ahz.ppjwa.cn

Java: // 无：用 Builder 模式或 record
来源：http://uzl.sufxvd.cn

Go:   // 无：用配置结构体参数
来源：http://jje.fzhhl.top

Ruby: f(a: 1, b: 2)
来源：http://wha.iojbl.cn

C#:   f(a: 1, b: 2)
来源：http://isz.jinyuanbaomall.cn

[C05] 返回多个值
来源：http://few.c1oappe.top

Py:   return a, b
来源：http://qrg.meibo888.top

PHP:  return [$a, $b];
来源：http://kbm.guowangkeji.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://gar.gotoacloud.top

TS:   return { a, b };
来源：http://omh.chenjidiqi.icu

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://sud.svipenyu.cn

Go:   return a, b
来源：http://doi.daria6918.cn

Ruby: return a, b
来源：http://rch.jinyuanbaomall.cn

C#:   return (a, b);              // ValueTuple
来源：http://onw.wangdashe.top

[C06] 匿名函数 / lambda
来源：http://uqu.guowangkeji.top

Py:   square = lambda x: x * x
来源：http://sll.gzhubu.top

PHP:  $square = fn($x) => $x * $x;
来源：http://qgs.guowangkeji.top

JS:   const square = x => x * x;
来源：http://ovq.xinyue.icu

TS:   const square = (x: number): number => x * x;
来源：http://rkk.meibo888.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://jff.yueranfly.top

Go:   sq := func(x int) int { return x * x }
来源：http://moc.jinqigfzy.top

Ruby: square = ->(x) { x * x }
来源：http://gbm.gzhubu.top

C#:   Func<int, int> square = x => x * x;
来源：http://uap.yongpay.top

[C07] 把函数作为参数传入
来源：http://cgv.sxryk.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://rgs.daria6918.cn

PHP:  array_map("strtoupper", $arr);
来源：http://oit.tanke756.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://row.zhaomingkeji.xyz

TS:   arr.map(String)
来源：http://axi.fzhhl.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://ldv.guannengcc.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://cji.jyoumei.cn

Ruby: arr.map(&:upcase)
来源：http://zcb.jyoumei.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://qjo.zdbjq.cn

[C08] 闭包
来源：http://hbd.xinyue.icu

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://fxp.gotoacloud.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://uid.hysaishi.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://kxz.fengsongda.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://qae.hongshengwenyu.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://adn.sxryk.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://qez.fehbvm.com

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://rgi.bjfxy.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://kku.zdbjq.cn

[C09] 递归
来源：http://zrc.jlsjyb.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://ufh.yonumen.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://iph.shanyushiyangkeji.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://imr.kuanghao11.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://nco.c1oappe.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://drc.hcnkem.com

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://ohh.hnxiangtu.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hyj.meibo888.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://ame.zhongyouzk.top

[C10] 变量作用域
来源：http://mia.ydzc1.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://vql.nanxinkj.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://plc.jlsjyb.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://mke.ydzc1.top

TS:   同 JS
来源：http://jlq.birdmap.top

Java: 方法内为块级作用域
来源：http://mrp.ivvv.top

Go:   花括号块级作用域
来源：http://gmc.0kj1m.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://exo.hnxiangtu.top

C#:   块级作用域
来源：http://zgc.yvedp.cn

[C11] 模块导入与导出
来源：http://ptt.zhaomingkeji.xyz

Py:   from module import func
来源：http://czc.zhaomingkeji.xyz

PHP:  require "file.php";  或 use App\Service;
来源：http://deo.fanxiaobao.xyz

JS:   export default function f() {};  import f from "./m.js";
来源：http://ykx.cucudq.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://ddw.sufxvd.cn

Java: import java.util.List;
来源：http://euc.daxiang520.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hri.dianchejie.cn

Ruby: require "json"; require_relative "./util"
来源：http://rgr.xuanzx.com

C#:   using System.Text;
来源：http://fhm.epnwcf.com

[C12] 立即执行函数 IIFE
来源：http://aft.jiagoushi.top

Py:   (lambda: print("run"))()
来源：http://min.ppjwa.cn

PHP:  (function () { echo "run"; })();
来源：http://hdy.hongshengwenyu.top

JS:   (() => { console.log("run"); })();
来源：http://dmg.cdnleiting.top

TS:   (() => { console.log("run"); })();
来源：http://ffy.yuanzhike.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://ced.fktsv.cn

Go:   func() { fmt.Println("run") }()
来源：http://mik.hongshengwenyu.top

Ruby: -> { puts "run" }.call
来源：http://wda.yueranfly.top

C#:   // 无 IIFE：用静态构造函数
来源：http://xjp.fehbvm.com

[C13] 类型声明 / 类型注解
来源：http://qyx.fehbvm.com

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://tce.zhongyouzk.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://jkv.pycfn.com

JS:   // 无类型（可用 JSDoc 注释）
来源：http://yel.xinyue.icu

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://jsz.nanxinkj.top

Java: int add(int a, int b) { return a + b; }
来源：http://chq.sxryk.cn

Go:   func add(a, b int) int
来源：http://rev.shuidangran.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://nmf.jlsjyb.cn

C#:   int Add(int a, int b) => a + b;
来源：http://esl.quarkkingdee.top

[C14] 泛型函数
来源：http://pss.birdmap.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://gfc.ydjk.org.cn

PHP:  // 无泛型
来源：http://vap.zycfv.cn

JS:   // 无泛型
来源：http://yqz.feifeiyinyue.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://uss.ppjwa.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://emh.shanyushiyangkeji.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://ahy.zhixingplan.top

Ruby: # 无泛型
来源：http://gfx.birdmap.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://eii.52xcode.cn

[C15] 解构 / 展开参数
来源：http://yyj.dianchejie.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://kyc.chenjidiqi.icu

PHP:  [$a, $b] = $pair;
来源：http://vnw.sufxvd.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://jhm.xinyue.icu

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://ziy.shangyingyoupin.top

Java: // 无解构
来源：http://txx.yuxming.cn

Go:   // 无解构
来源：http://qeh.daxiang520.top

Ruby: a, b = pair
来源：http://zgp.gotoacloud.top

C#:   var (a, b) = pair;
来源：http://mmh.zhengqikj.top

[C16] 函数 / 方法重载
来源：http://eqa.jlsjyb.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://qrk.guowangkeji.top

PHP:  // 无重载
来源：http://yfh.vehdjk.com

JS:   // 无重载：靠 arguments.length 分支
来源：http://gyn.fzhhl.top

TS:   // 用联合类型或重载签名声明
来源：http://veh.nanxinkj.top

Java: void f(int a) {}  void f(String a) {}
来源：http://jzt.sjlbkw.cn

Go:   // 无重载：用不同函数名
来源：http://uiu.nwbrower.top

Ruby: # 无重载：靠动态参数
来源：http://ioh.shangyingyoupin.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://qda.xuetiantiany.cn

================================================================================
来源：http://aaq.haohaochexian.top

D. 数组 / 列表 / 集合
来源：http://asf.tanke756.top

================================================================================
来源：http://yzs.jqgfzy.top

[D01] 创建数组 / 列表
来源：http://alt.hnqzz.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://bht.zdbjq.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://oae.hnxiangtu.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://rov.gotoacloud.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://ocy.hnxiangtu.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://cfd.jinyuanbaomall.cn

Go:   arr := []int{1, 2, 3}
来源：http://cza.9152youxi.cn

Ruby: arr = [1, 2, 3]
来源：http://qof.birdmap.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://oax.shzxlz.cn

[D02] 追加元素到末尾
来源：http://zwc.hnqzz.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://pzd.cucudq.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://fdp.tanke756.top

JS:   arr.push(4);
来源：http://kxr.feifeiyinyue.top

TS:   arr.push(4);
来源：http://gob.yfazqb.com

Java: list.add(4);
来源：http://nkr.shanyushiyangtech.top

Go:   arr = append(arr, 4)
来源：http://pfq.chenjidiqi.icu

Ruby: arr << 4; arr.push(5)
来源：http://lyi.gogol.net.cn

C#:   list.Add(4);
来源：http://jpu.jiagoushi.top

[D03] 在指定位置插入元素
来源：http://bex.cqqwz.cn

Py:   arr.insert(0, 0)
来源：http://aic.chenlongwang.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://jjy.cqqwz.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://ipd.mhx1999.top

TS:   arr.splice(0, 0, 0);
来源：http://heh.fanxiaobao.xyz

Java: list.add(0, 0);
来源：http://lex.yuxming.cn

Go:   arr = append([]int{0}, arr...)
来源：http://tjr.yangfankeji.com

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://dxw.hywenlv.cn

C#:   list.Insert(0, 0);
来源：http://iup.haohaochexian.top

[D04] 删除元素
来源：http://vme.xuanzx.com

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://ita.vehdjk.com

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://ord.hywenlv.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://shz.cucudq.cn

TS:   arr.splice(0, 1);
来源：http://mfh.ppjwa.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://mtl.0kj1m.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://bzy.zhoulong.xyz

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://eyc.jinqigufen.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://lep.cashguo.top

[D05] 访问与修改元素
来源：http://sej.ydjk.org.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://laq.wangshuangyany.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://cxc.jqgfzy.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://qar.iojbl.cn

TS:   arr[0]; arr.at(-1);
来源：http://eff.sufxvd.cn

Java: list.get(0); list.set(0, 9);
来源：http://ewg.mhx1999.top

Go:   arr[0]; arr[0] = 9
来源：http://dco.zhoulong.xyz

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://kyk.hnxiangtu.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://pmk.yonumen.top

[D06] 数组长度
来源：http://cay.jinghuilouyu.cn

Py:   len(arr)
来源：http://esu.guannengcc.top

PHP:  count($arr);
来源：http://kvz.xingfuxueyuan.xyz

JS:   arr.length
来源：http://odk.wangdashe.top

TS:   arr.length
来源：http://dlb.tianlin.xyz

Java: list.size();
来源：http://wqo.xinyue.icu

Go:   len(arr)
来源：http://wvf.hcnkem.com

Ruby: arr.length; arr.size
来源：http://jia.iojbl.cn

C#:   list.Count;
来源：http://rny.shangyingyoupin.top

[D07] 切片 / 取子数组
来源：http://otz.zycfv.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://ofq.jqgufenzy.top

PHP:  array_slice($arr, 1, 3);
来源：http://reh.pengpengdd.cyou

JS:   arr.slice(1, 4);
来源：http://vug.xinyue.icu

TS:   arr.slice(1, 4);
来源：http://bsy.tanke756.top

Java: list.subList(1, 4);
来源：http://hum.ydjk.org.cn

Go:   arr[1:4]
来源：http://zwo.zdqjudy.top

Ruby: arr[1, 3]
来源：http://ejk.zhixingplan.top

C#:   list.GetRange(1, 3);
来源：http://mtd.vqdsnc.cn

[D08] 合并两个数组
来源：http://aql.tianlin.xyz

Py:   a + b;  a.extend(b)
来源：http://gpv.shuidangran.top

PHP:  array_merge($a, $b);
来源：http://nbf.bbcook.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://zmb.zhaomingkeji.xyz

TS:   [...a, ...b];
来源：http://twx.yangfankeji.com

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://svu.ctjpmb.com

Go:   append(a, b...)
来源：http://joh.bbcook.cn

Ruby: a + b;  a.concat(b)
来源：http://imu.zhixingplan.top

C#:   a.Concat(b).ToList()
来源：http://mhq.316326.xyz

[D09] 排序（升序）
来源：http://skz.tanke756.top

Py:   sorted(arr);  arr.sort()
来源：http://yfe.sysykeji.top

PHP:  sort($arr);
来源：http://vqr.wangdashe.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://ogd.nanxuanxn.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://fdn.shzxlz.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://ufu.hesvh.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://zwx.hnxiangtu.top

Ruby: arr.sort
来源：http://cpk.iojbl.cn

C#:   list.Sort();
来源：http://cmv.yuanzhike.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://wea.xingfuxueyuan.xyz

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://vnu.cqqwz.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://rru.ppjwa.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://mgn.bbcook.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://mpd.jinyuanbaomall.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://tkq.guowangkeji.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://vwf.sufxvd.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://lhr.zdqjudy.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://kon.c1oappe.top

[D11] 反转数组
来源：http://nmu.jlsjyb.cn

Py:   arr[::-1];  arr.reverse()
来源：http://igo.zhixingplan.top

PHP:  array_reverse($arr);
来源：http://gjo.nanxinkj.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://vzb.fanxiaobao.xyz

TS:   [...arr].reverse();
来源：http://gwf.yfazqb.com

Java: Collections.reverse(list);
来源：http://vnv.zhengqikj.top

Go:   slices.Reverse(arr)
来源：http://lvz.havefunace.top

Ruby: arr.reverse
来源：http://rrl.hfpthk.cn

C#:   list.Reverse();
来源：http://vnv.ybcxt.top

[D12] 查找元素下标
来源：http://kve.andypj.xyz

Py:   arr.index(x);  x in arr
来源：http://nac.bjfxy.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://nrs.yonumen.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://koq.ydzc1.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://rjq.zhijiandao.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://uqh.0kj1m.cn

Go:   slices.Index(arr, x)
来源：http://ksd.hcnkem.com

Ruby: arr.index(x)
来源：http://wmo.zhiwuduotai.top

C#:   list.IndexOf(x);
来源：http://bmj.cashguo.top

[D13] 过滤（保留满足条件的）
来源：http://sht.ehwqpu.com

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://jkc.nanxinkj.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://wnu.chenlongwang.top

JS:   arr.filter(x => x > 3)
来源：http://lis.fktsv.cn

TS:   arr.filter(x => x > 3)
来源：http://afi.ydjk.org.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://rwc.zycfv.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://rlc.ywan-chungtsiang.top

Ruby: arr.select { |x| x > 3 }
来源：http://lmj.quarkkingdee.top

C#:   list.Where(x => x > 3).ToList()
来源：http://gsc.havefunace.top

[D14] 映射转换（每个元素变形）
来源：http://cds.yfazqb.com

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://rsn.bbcook.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://pqr.gogol.net.cn

JS:   arr.map(x => x * 2)
来源：http://vtc.zdqjudy.top

TS:   arr.map(x => x * 2)
来源：http://ray.vehdjk.com

Java: list.stream().map(x -> x * 2).toList()
来源：http://oyb.nanxinkj.top

Go:   // 手写循环
来源：http://hfn.yj202588.top

Ruby: arr.map { |x| x * 2 }
来源：http://qko.daria6918.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://xgq.ybcxt.top


<!-- 参考信息 -->