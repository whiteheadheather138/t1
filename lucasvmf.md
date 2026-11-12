代发 wailian999

Ruby: [1, 2, 3].include?(x)
来源：http://ugy.birdmap.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://fjg.jyoumei.cn

[B15] 布尔运算与取反
来源：http://say.fzhhl.top

Py:   a and b or not c
来源：http://gnf.xziqi.cn

PHP:  $a && $b || !$c
来源：http://sjk.epnwcf.com

JS:   a && b || !c
来源：http://gjb.hesvh.cn

TS:   a && b || !c
来源：http://est.chenlongwang.top

Java: a && b || !c
来源：http://bwc.xuanzx.com

Go:   a && b || !c
来源：http://jsk.gaohongyu789.top

Ruby: a && b || !c
来源：http://dvd.zdqjudy.top

C#:   a && b || !c
来源：http://ojf.xziqi.cn

[B16] 卫语句：不满足条件提前返回
来源：http://ukg.zhaomingkeji.xyz

Py:   if not data: return
来源：http://ayk.xuetiantiany.cn

PHP:  if (!$data) { return; }
来源：http://xwy.52xcode.cn

JS:   if (!data) return;
来源：http://ayi.vehdjk.com

TS:   if (!data) return;
来源：http://rdy.shangyingyoupin.top

Java: if (data == null) return;
来源：http://bos.epnwcf.com

Go:   if data == nil { return }
来源：http://eub.hnxiangtu.top

Ruby: return if data.nil?
来源：http://pds.yuxming.cn

C#:   if (data == null) return;
来源：http://ato.zhengqikj.top

================================================================================
来源：http://zor.dianchejie.cn

C. 函数与作用域
来源：http://sni.guowangkeji.top

================================================================================
来源：http://eje.yuanzhike.top

[C01] 定义函数
来源：http://jfp.yueranfly.top

Py:   def add(a, b): return a + b
来源：http://dgh.xuanzx.com

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://rje.yonumen.top

JS:   function add(a, b) { return a + b; }
来源：http://upg.zhixingplan.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://nxw.jlsjyb.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://qzo.pycfn.com

Go:   func add(a, b int) int { return a + b }
来源：http://bvs.jinqigfzy.top

Ruby: def add(a, b); a + b; end
来源：http://wxy.chenjidiqi.icu

C#:   static int Add(int a, int b) { return a + b; }
来源：http://rtd.sufxvd.cn

[C02] 默认参数
来源：http://baw.gotoacloud.top

Py:   def greet(name="World"): return name
来源：http://gnj.yj20258888.top

PHP:  function greet($name = "World") { return $name; }
来源：http://wnf.dashuyun.cn

JS:   function greet(name = "World") { return name; }
来源：http://pva.gzhubu.top

TS:   function greet(name: string = "World") { return name; }
来源：http://owo.jinqigufen.top

Java: // 无默认参数：方法重载或 Optional
来源：http://kqi.zhengqikj.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://scu.sxryk.cn

Ruby: def greet(name = "World") = name
来源：http://szj.wangdashe.top

C#:   string Greet(string name = "World") => name;
来源：http://xaq.cqqwz.cn

[C03] 可变参数
来源：http://pve.fanxiaobao.xyz

Py:   def total(*args): return sum(args)
来源：http://zkf.zhongyouzk.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://uig.zhixingplan.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://jmk.zdqjudy.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://nai.xziqi.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://mux.zhengqikj.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://ilm.dianchejie.cn

Ruby: def total(*nums); nums.sum; end
来源：http://nmd.yonumen.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://xlj.zhengqikj.top

[C04] 命名参数 / 关键字参数
来源：http://qdx.zhaomingkeji.xyz

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://ecs.snrcjt.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://xzv.cqqwz.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://zet.iojbl.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://nvm.jyoumei.cn

Java: // 无：用 Builder 模式或 record
来源：http://ltm.zhengqikj.top

Go:   // 无：用配置结构体参数
来源：http://gow.yuxming.cn

Ruby: f(a: 1, b: 2)
来源：http://ziy.zhiwuduotai.top

C#:   f(a: 1, b: 2)
来源：http://asu.chenjidiqi.icu

[C05] 返回多个值
来源：http://rkf.ybcxt.top

Py:   return a, b
来源：http://gii.xuetiantiany.cn

PHP:  return [$a, $b];
来源：http://lvo.pengpengdd.cyou

JS:   return [a, b];             // 或 return { a, b };
来源：http://rxw.smart0.xyz

TS:   return { a, b };
来源：http://voo.vehdjk.com

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://xoo.yanxiufei.cn

Go:   return a, b
来源：http://ern.316326.xyz

Ruby: return a, b
来源：http://wgz.jqgufenzy.top

C#:   return (a, b);              // ValueTuple
来源：http://qcg.wangdashe.top

[C06] 匿名函数 / lambda
来源：http://ybq.jqgufenzy.top

Py:   square = lambda x: x * x
来源：http://cmg.snrcjt.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://lrd.dashuyun.cn

JS:   const square = x => x * x;
来源：http://cer.tianlin.xyz

TS:   const square = (x: number): number => x * x;
来源：http://kxe.hnqzz.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://zoo.smart0.xyz

Go:   sq := func(x int) int { return x * x }
来源：http://uap.zhengqikj.top

Ruby: square = ->(x) { x * x }
来源：http://yvk.redwolf501.top

C#:   Func<int, int> square = x => x * x;
来源：http://clf.smart0.xyz

[C07] 把函数作为参数传入
来源：http://jgj.hywenlv.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://fou.jinyuanbaomall.cn

PHP:  array_map("strtoupper", $arr);
来源：http://qux.ehwqpu.com

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://ioe.zdbjq.cn

TS:   arr.map(String)
来源：http://fzm.andypj.xyz

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://jsw.yfazqb.com

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://lbh.zhixingplan.top

Ruby: arr.map(&:upcase)
来源：http://yia.sjlbkw.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://mep.hfpthk.cn

[C08] 闭包
来源：http://vxg.wangdashe.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://dsx.jlsjyb.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://blc.xylfe.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://irf.chenzaomai.com

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://tyh.gogol.net.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://yuy.jqgufenzy.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://wur.chenzaomai.com

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://jpk.jianghu66.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://bbg.bjfxy.top

[C09] 递归
来源：http://pky.chenlongwang.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://ocb.hammf.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://mxd.yonumen.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wff.fehbvm.com

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://whd.yj20258888.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://ufw.gotoacloud.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://kvf.fktsv.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://vdo.pycfn.com

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hjk.zdbjq.cn

[C10] 变量作用域
来源：http://tae.chenjidiqi.icu

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://kaq.xylfe.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://wjn.yvedp.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://edc.cucudq.cn

TS:   同 JS
来源：http://glf.guowangkeji.top

Java: 方法内为块级作用域
来源：http://rvb.ydjk.org.cn

Go:   花括号块级作用域
来源：http://elf.xinyue.icu

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://yfv.yvedp.cn

C#:   块级作用域
来源：http://shb.yj20258888.top

[C11] 模块导入与导出
来源：http://aak.vehdjk.com

Py:   from module import func
来源：http://nze.bjfxy.top

PHP:  require "file.php";  或 use App\Service;
来源：http://eqa.cheryme.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://sgo.yfazqb.com

TS:   export function f(): void {};  import { f } from "./m";
来源：http://tbq.wangdashe.top

Java: import java.util.List;
来源：http://fpb.ydzc1.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://ali.zhijiandao.cn

Ruby: require "json"; require_relative "./util"
来源：http://hxn.jiagoushi.top

C#:   using System.Text;
来源：http://pvf.xuanzx.com

[C12] 立即执行函数 IIFE
来源：http://hbc.jyoumei.cn

Py:   (lambda: print("run"))()
来源：http://qvc.zhiwuduotai.top

PHP:  (function () { echo "run"; })();
来源：http://vyt.9152youxi.cn

JS:   (() => { console.log("run"); })();
来源：http://opr.ydzc1.top

TS:   (() => { console.log("run"); })();
来源：http://ona.smart0.xyz

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://zfs.shanyushiyangtech.top

Go:   func() { fmt.Println("run") }()
来源：http://pmu.xuanzx.com

Ruby: -> { puts "run" }.call
来源：http://snx.xingfuxueyuan.xyz

C#:   // 无 IIFE：用静态构造函数
来源：http://nik.52xcode.cn

[C13] 类型声明 / 类型注解
来源：http://gvb.wangshuangyany.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://rcl.uphjek.com

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://gxm.shanyushiyangtech.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://ayq.chenlongwang.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hum.ybcxt.top

Java: int add(int a, int b) { return a + b; }
来源：http://fpa.zhijiandao.cn

Go:   func add(a, b int) int
来源：http://heq.shzxlz.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://kos.ydjk.org.cn

C#:   int Add(int a, int b) => a + b;
来源：http://mta.jiagoushi.top

[C14] 泛型函数
来源：http://iqs.tarul.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://btx.hywenlv.cn

PHP:  // 无泛型
来源：http://bhv.xuanzx.com

JS:   // 无泛型
来源：http://rkc.xziqi.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://gfk.fehbvm.com

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://rwn.nwbrower.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://lhi.9152youxi.cn

Ruby: # 无泛型
来源：http://twu.nwbrower.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://yrl.jqgfzy.top

[C15] 解构 / 展开参数
来源：http://rwk.daria6918.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://tav.birdmap.top

PHP:  [$a, $b] = $pair;
来源：http://gkn.svipenyu.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://tpk.sufxvd.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://fsb.chenzaomai.com

Java: // 无解构
来源：http://ttt.wangshuangyany.cn

Go:   // 无解构
来源：http://gtx.zdqjudy.top

Ruby: a, b = pair
来源：http://qrj.jyoumei.cn

C#:   var (a, b) = pair;
来源：http://tzf.hfpthk.cn

[C16] 函数 / 方法重载
来源：http://vid.ybcxt.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hhj.wangdashe.top

PHP:  // 无重载
来源：http://jww.zhengqikj.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://dlv.wangshuangyany.cn

TS:   // 用联合类型或重载签名声明
来源：http://fpq.jianghu66.top

Java: void f(int a) {}  void f(String a) {}
来源：http://wgj.zhiwuduotai.top

Go:   // 无重载：用不同函数名
来源：http://udh.0kj1m.cn

Ruby: # 无重载：靠动态参数
来源：http://kmk.daxiang520.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://lea.aizwys.cn

================================================================================
来源：http://sig.sufxvd.cn

D. 数组 / 列表 / 集合
来源：http://xee.zhaomingkeji.xyz

================================================================================
来源：http://pgf.jinqigfzy.top

[D01] 创建数组 / 列表
来源：http://tez.fzhhl.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://vum.nanxinkj.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://rsg.uphjek.com

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://cgt.shanyushiyangtech.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://isv.jqgufenzy.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://shv.nwbrower.top

Go:   arr := []int{1, 2, 3}
来源：http://nli.kuanghao11.cn

Ruby: arr = [1, 2, 3]
来源：http://uql.gogol.net.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hgn.316326.xyz

[D02] 追加元素到末尾
来源：http://sdd.sufxvd.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://zgz.ivvv.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://doc.zhixingplan.top

JS:   arr.push(4);
来源：http://ogs.c1oappe.top

TS:   arr.push(4);
来源：http://wbv.birdmap.top

Java: list.add(4);
来源：http://deg.ppjwa.cn

Go:   arr = append(arr, 4)
来源：http://uml.redwolf501.top

Ruby: arr << 4; arr.push(5)
来源：http://iky.dashuyun.cn

C#:   list.Add(4);
来源：http://oxu.snrcjt.cn

[D03] 在指定位置插入元素
来源：http://mwh.smart0.xyz

Py:   arr.insert(0, 0)
来源：http://dml.guannengcc.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://awe.ydjk.org.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://fox.cucudq.cn

TS:   arr.splice(0, 0, 0);
来源：http://wjx.uphjek.com

Java: list.add(0, 0);
来源：http://xwu.smart0.xyz

Go:   arr = append([]int{0}, arr...)
来源：http://gum.jqgufenzy.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://bvz.c1oappe.top

C#:   list.Insert(0, 0);
来源：http://jdf.ctjpmb.com

[D04] 删除元素
来源：http://seb.iojbl.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://zkm.zhengqikj.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://nlp.tarul.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://mly.andypj.xyz

TS:   arr.splice(0, 1);
来源：http://aul.pengpengdd.cyou

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://nny.fengsongda.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://qwi.vqdsnc.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://csx.fktsv.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://tvh.dashuyun.cn

[D05] 访问与修改元素
来源：http://ztp.shzxlz.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://fbn.dianchejie.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://zqc.tanke756.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://xgz.ehwqpu.com

TS:   arr[0]; arr.at(-1);
来源：http://rty.ehwqpu.com

Java: list.get(0); list.set(0, 9);
来源：http://ael.guowangkeji.top

Go:   arr[0]; arr[0] = 9
来源：http://sgs.sxryk.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://ryn.shanyushiyangkeji.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://ibn.snrcjt.cn

[D06] 数组长度
来源：http://xdk.tanke756.top

Py:   len(arr)
来源：http://bpb.hcnkem.com

PHP:  count($arr);
来源：http://ngm.gzhubu.top

JS:   arr.length
来源：http://vsu.pengpengdd.cyou

TS:   arr.length
来源：http://ykl.xuanzx.com

Java: list.size();
来源：http://dld.nwbrower.top

Go:   len(arr)
来源：http://xbp.bbcook.cn

Ruby: arr.length; arr.size
来源：http://lzq.guannengcc.top

C#:   list.Count;
来源：http://xnq.uphjek.com

[D07] 切片 / 取子数组
来源：http://whz.xingfuxueyuan.xyz

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://yri.guowangkeji.top

PHP:  array_slice($arr, 1, 3);
来源：http://xaz.ivvv.top

JS:   arr.slice(1, 4);
来源：http://txc.ydzc1.top

TS:   arr.slice(1, 4);
来源：http://xzj.yanxiufei.cn

Java: list.subList(1, 4);
来源：http://uix.zdbjq.cn

Go:   arr[1:4]
来源：http://xay.sufxvd.cn

Ruby: arr[1, 3]
来源：http://nph.daria6918.cn

C#:   list.GetRange(1, 3);
来源：http://ssr.dianchejie.cn

[D08] 合并两个数组
来源：http://aty.ivvv.top

Py:   a + b;  a.extend(b)
来源：http://kud.ybcxt.top

PHP:  array_merge($a, $b);
来源：http://ewj.zhiwuduotai.top

JS:   [...a, ...b];  a.concat(b);
来源：http://ulc.shuidangran.top

TS:   [...a, ...b];
来源：http://uks.chenzaomai.com

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://izv.hongshengwenyu.top

Go:   append(a, b...)
来源：http://gxk.yongpay.top

Ruby: a + b;  a.concat(b)
来源：http://dgc.ydjk.org.cn

C#:   a.Concat(b).ToList()
来源：http://idl.zycfv.cn

[D09] 排序（升序）
来源：http://qfh.zhixingplan.top

Py:   sorted(arr);  arr.sort()
来源：http://hov.sjlbkw.cn

PHP:  sort($arr);
来源：http://bfk.xinyue.icu

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://vqh.xinyue.icu

TS:   [...arr].sort((x, y) => x - y);
来源：http://yeo.kuanghao11.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://owe.yj20258.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://byr.redwolf501.top

Ruby: arr.sort
来源：http://lfh.yvedp.cn

C#:   list.Sort();
来源：http://woo.cqqwz.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://bfl.hnqzz.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://ofp.redwolf501.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://xgw.tarul.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://zfr.guannengcc.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://gao.aibaodan.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://veq.zhixingplan.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://ozo.yfazqb.com

Ruby: arr.sort_by { |x| x[:age] }
来源：http://jei.ydzc1.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://fuo.yuanzhike.top

[D11] 反转数组
来源：http://jif.sxryk.cn

Py:   arr[::-1];  arr.reverse()
来源：http://alg.zhoulong.xyz

PHP:  array_reverse($arr);
来源：http://ezt.nwbrower.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://fuv.jinyuanbaomall.cn

TS:   [...arr].reverse();
来源：http://xsv.jqgufenzy.top

Java: Collections.reverse(list);
来源：http://sxi.yonumen.top

Go:   slices.Reverse(arr)
来源：http://yzz.tarul.cn

Ruby: arr.reverse
来源：http://idw.jqgufenzy.top

C#:   list.Reverse();
来源：http://ddz.yuanzhike.top

[D12] 查找元素下标
来源：http://qwv.gzhubu.top

Py:   arr.index(x);  x in arr
来源：http://cft.ppjwa.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://gyu.nanxinkj.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://jue.hysaishi.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://peh.316326.xyz

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://epz.sxryk.cn

Go:   slices.Index(arr, x)
来源：http://has.bjfxy.top

Ruby: arr.index(x)
来源：http://ujn.wangshuangyany.cn

C#:   list.IndexOf(x);
来源：http://ndf.svipenyu.cn

[D13] 过滤（保留满足条件的）
来源：http://ris.jinqigfzy.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hfr.c1oappe.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://bba.mhx1999.top

JS:   arr.filter(x => x > 3)
来源：http://puf.hywenlv.cn

TS:   arr.filter(x => x > 3)
来源：http://mim.ybcxt.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://exf.ivvv.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://nce.jlsjyb.cn

Ruby: arr.select { |x| x > 3 }
来源：http://ils.yvedp.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://aut.cucudq.cn

[D14] 映射转换（每个元素变形）
来源：http://ilo.gzhubu.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://wtk.jyoumei.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://ajd.fktsv.cn

JS:   arr.map(x => x * 2)
来源：http://azn.dianchejie.cn

TS:   arr.map(x => x * 2)
来源：http://gwg.jqgfzy.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://ohe.0kj1m.cn

Go:   // 手写循环
来源：http://uxf.hnqzz.top

Ruby: arr.map { |x| x * 2 }
来源：http://kds.yangfankeji.com

C#:   list.Select(x => x * 2).ToList()
来源：http://vls.kuanghao11.cn

[D15] 去重
来源：http://mmn.chenlongwang.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://znv.tianlin.xyz

PHP:  array_unique($arr);
来源：http://jdx.ydjk.org.cn

JS:   [...new Set(arr)]
来源：http://hkm.gogol.net.cn


<!-- 参考信息 -->