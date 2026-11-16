代发 wailian999

[C02] 默认参数
来源：http://val.xuanzx.com

Py:   def greet(name="World"): return name
来源：http://fea.hammf.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://ubr.jqgfzy.top

JS:   function greet(name = "World") { return name; }
来源：http://tly.sysykeji.top

TS:   function greet(name: string = "World") { return name; }
来源：http://ixr.ybcxt.top

Java: // 无默认参数：方法重载或 Optional
来源：http://lcc.tianlin.xyz

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://bza.zdqjudy.top

Ruby: def greet(name = "World") = name
来源：http://cvq.zhaomingkeji.xyz

C#:   string Greet(string name = "World") => name;
来源：http://nse.smart0.xyz

[C03] 可变参数
来源：http://ygw.chenzaomai.com

Py:   def total(*args): return sum(args)
来源：http://tso.yj20258888.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://rbb.yvedp.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://gsn.xziqi.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://aro.uphjek.com

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://sja.gotoacloud.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://rbw.smart0.xyz

Ruby: def total(*nums); nums.sum; end
来源：http://oul.havefunace.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://kwe.52xcode.cn

[C04] 命名参数 / 关键字参数
来源：http://psd.dianchejie.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://fpj.quarkkingdee.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://ngh.cucudq.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://jcv.yj202588.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://sjk.snrcjt.cn

Java: // 无：用 Builder 模式或 record
来源：http://qob.yueranfly.top

Go:   // 无：用配置结构体参数
来源：http://xeo.tian-w.cn

Ruby: f(a: 1, b: 2)
来源：http://yia.zdbjq.cn

C#:   f(a: 1, b: 2)
来源：http://ers.wangdashe.top

[C05] 返回多个值
来源：http://jxu.hammf.cn

Py:   return a, b
来源：http://gkr.cheryme.top

PHP:  return [$a, $b];
来源：http://nvn.sjlbkw.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://div.tarul.cn

TS:   return { a, b };
来源：http://rmg.jinqigufen.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://ayb.ivvv.top

Go:   return a, b
来源：http://rpp.svipenyu.cn

Ruby: return a, b
来源：http://ung.fehbvm.com

C#:   return (a, b);              // ValueTuple
来源：http://icb.smart0.xyz

[C06] 匿名函数 / lambda
来源：http://jlk.uphjek.com

Py:   square = lambda x: x * x
来源：http://uro.vehdjk.com

PHP:  $square = fn($x) => $x * $x;
来源：http://rnj.ydjk.org.cn

JS:   const square = x => x * x;
来源：http://qrq.zdbjq.cn

TS:   const square = (x: number): number => x * x;
来源：http://ymq.jqgfzy.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://siv.quarkkingdee.top

Go:   sq := func(x int) int { return x * x }
来源：http://rwo.smart0.xyz

Ruby: square = ->(x) { x * x }
来源：http://smm.haohaochexian.top

C#:   Func<int, int> square = x => x * x;
来源：http://bkf.meibo888.top

[C07] 把函数作为参数传入
来源：http://sfh.iojbl.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://pqa.guannengcc.top

PHP:  array_map("strtoupper", $arr);
来源：http://mxy.tianlin.xyz

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://tlp.jinghuilouyu.cn

TS:   arr.map(String)
来源：http://gyn.chenlongwang.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://pyj.daxiang520.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://gga.vehdjk.com

Ruby: arr.map(&:upcase)
来源：http://ena.feifeiyinyue.top

C#:   arr.Select(s => s.ToUpper())
来源：http://urz.aibaodan.cn

[C08] 闭包
来源：http://ogu.jinghuilouyu.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://sgc.haohaochexian.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://tfz.zhongyouzk.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://qpo.dashuyun.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://ndc.yfazqb.com

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://pyk.yfazqb.com

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://syb.nanxinkj.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://lnu.chenlongwang.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://ehe.hysaishi.cn

[C09] 递归
来源：http://knf.shuidangran.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://kce.hcnkem.com

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hep.meibo888.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wfq.yj202588.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://gqc.vehdjk.com

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://beu.kuanghao11.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hvo.guowangkeji.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://saa.tanke756.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://flr.jqgfzy.top

[C10] 变量作用域
来源：http://dfn.wangdashe.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://xln.xingfuxueyuan.xyz

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://uit.uphjek.com

JS:   let/const 块级作用域，var 函数级作用域
来源：http://uzh.zhongyouzk.top

TS:   同 JS
来源：http://whs.hesvh.cn

Java: 方法内为块级作用域
来源：http://ijg.nanxuanxn.top

Go:   花括号块级作用域
来源：http://myt.jinqigufen.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://ohb.yuxming.cn

C#:   块级作用域
来源：http://lru.bjfxy.top

[C11] 模块导入与导出
来源：http://uwf.ehwqpu.com

Py:   from module import func
来源：http://uwb.sufxvd.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://eeh.52xcode.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://mcq.nwbrower.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://lvz.yueranfly.top

Java: import java.util.List;
来源：http://cju.fktsv.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://siq.iojbl.cn

Ruby: require "json"; require_relative "./util"
来源：http://edn.yangfankeji.com

C#:   using System.Text;
来源：http://xkg.andypj.xyz

[C12] 立即执行函数 IIFE
来源：http://mho.yj202588.top

Py:   (lambda: print("run"))()
来源：http://ygm.aizwys.cn

PHP:  (function () { echo "run"; })();
来源：http://dzm.svipenyu.cn

JS:   (() => { console.log("run"); })();
来源：http://pnr.yongpay.top

TS:   (() => { console.log("run"); })();
来源：http://fui.yuxming.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://srg.zdbjq.cn

Go:   func() { fmt.Println("run") }()
来源：http://eet.epnwcf.com

Ruby: -> { puts "run" }.call
来源：http://bvp.yuanzhike.top

C#:   // 无 IIFE：用静态构造函数
来源：http://cgk.dashuyun.cn

[C13] 类型声明 / 类型注解
来源：http://oir.kuanghao11.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://vlg.tian-w.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://vbw.chenzaomai.com

JS:   // 无类型（可用 JSDoc 注释）
来源：http://uvy.xingfuxueyuan.xyz

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://xkz.zhixingplan.top

Java: int add(int a, int b) { return a + b; }
来源：http://tlh.vehdjk.com

Go:   func add(a, b int) int
来源：http://onk.svipenyu.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://agv.yonumen.top

C#:   int Add(int a, int b) => a + b;
来源：http://mlp.aibaodan.cn

[C14] 泛型函数
来源：http://hjl.nanxuanxn.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://ozq.ivvv.top

PHP:  // 无泛型
来源：http://ueb.fengsongda.top

JS:   // 无泛型
来源：http://zbv.shzxlz.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://mzc.sweek.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://sig.9152youxi.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://ouo.hnqzz.top

Ruby: # 无泛型
来源：http://fvx.quarkkingdee.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://fpd.xuetiantiany.cn

[C15] 解构 / 展开参数
来源：http://pcb.xuanzx.com

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://nla.andypj.xyz

PHP:  [$a, $b] = $pair;
来源：http://bbn.redwolf501.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://leh.iojbl.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://znw.zhaomingkeji.xyz

Java: // 无解构
来源：http://vur.hesvh.cn

Go:   // 无解构
来源：http://gpm.hongshengwenyu.top

Ruby: a, b = pair
来源：http://zuw.yongpay.top

C#:   var (a, b) = pair;
来源：http://ycr.fehbvm.com

[C16] 函数 / 方法重载
来源：http://wwx.ybcxt.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://yro.pycfn.com

PHP:  // 无重载
来源：http://fkh.tian-w.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://psw.vqdsnc.cn

TS:   // 用联合类型或重载签名声明
来源：http://azy.jyoumei.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://kjh.zdqjudy.top

Go:   // 无重载：用不同函数名
来源：http://qwf.jinyuanbaomall.cn

Ruby: # 无重载：靠动态参数
来源：http://nkk.wangdashe.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://kbe.sysykeji.top

================================================================================
来源：http://tlo.zhixingplan.top

D. 数组 / 列表 / 集合
来源：http://mtn.fengsongda.top

================================================================================
来源：http://amw.jqgufenzy.top

[D01] 创建数组 / 列表
来源：http://lnp.vqdsnc.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://ojm.xylfe.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://gza.zhoulong.xyz

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://pgu.chenjidiqi.icu

TS:   const arr: number[] = [1, 2, 3];
来源：http://wxs.hammf.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://jwn.ybcxt.top

Go:   arr := []int{1, 2, 3}
来源：http://ajy.zhixingplan.top

Ruby: arr = [1, 2, 3]
来源：http://qej.hammf.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://doi.cheryme.top

[D02] 追加元素到末尾
来源：http://nwb.gaohongyu789.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://zoj.tianlin.xyz

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://qgg.chenlongwang.top

JS:   arr.push(4);
来源：http://kzj.9152youxi.cn

TS:   arr.push(4);
来源：http://afn.cdnleiting.top

Java: list.add(4);
来源：http://apl.yangfankeji.com

Go:   arr = append(arr, 4)
来源：http://jja.chenlongwang.top

Ruby: arr << 4; arr.push(5)
来源：http://jva.gogol.net.cn

C#:   list.Add(4);
来源：http://ghe.yanxiufei.cn

[D03] 在指定位置插入元素
来源：http://trl.xuanzx.com

Py:   arr.insert(0, 0)
来源：http://pma.yangfankeji.com

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://ohz.jlsjyb.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://col.zycfv.cn

TS:   arr.splice(0, 0, 0);
来源：http://cxy.xylfe.cn

Java: list.add(0, 0);
来源：http://imy.daria6918.cn

Go:   arr = append([]int{0}, arr...)
来源：http://dpj.shuidangran.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://sgt.daria6918.cn

C#:   list.Insert(0, 0);
来源：http://yuu.xingfuxueyuan.xyz

[D04] 删除元素
来源：http://kxv.birdmap.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://kwi.cdnleiting.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://whk.yj20258.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://cqh.hnxiangtu.top

TS:   arr.splice(0, 1);
来源：http://qhk.jinghuilouyu.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://fis.chenjidiqi.icu

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://zbh.feifeiyinyue.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://jhp.yfazqb.com

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://yzd.quarkkingdee.top

[D05] 访问与修改元素
来源：http://mlo.yj20258.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://pda.zdqjudy.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://kwq.aibaodan.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://ayi.sysykeji.top

TS:   arr[0]; arr.at(-1);
来源：http://aes.snrcjt.cn

Java: list.get(0); list.set(0, 9);
来源：http://gwo.hongshengwenyu.top

Go:   arr[0]; arr[0] = 9
来源：http://gaj.smart0.xyz

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://oue.yongpay.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://dkk.daxiang520.top

[D06] 数组长度
来源：http://rwu.zhongyouzk.top

Py:   len(arr)
来源：http://mwq.yuxming.cn

PHP:  count($arr);
来源：http://fkh.mhx1999.top

JS:   arr.length
来源：http://ipg.yj202588.top

TS:   arr.length
来源：http://zez.hnqzz.top

Java: list.size();
来源：http://kwp.tarul.cn

Go:   len(arr)
来源：http://ogj.guannengcc.top

Ruby: arr.length; arr.size
来源：http://yly.dashuyun.cn

C#:   list.Count;
来源：http://hip.sysykeji.top

[D07] 切片 / 取子数组
来源：http://zsr.vqdsnc.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://mjn.ivvv.top

PHP:  array_slice($arr, 1, 3);
来源：http://qtg.chenzaomai.com

JS:   arr.slice(1, 4);
来源：http://ctt.yj202588.top

TS:   arr.slice(1, 4);
来源：http://aij.hesvh.cn

Java: list.subList(1, 4);
来源：http://dyc.guowangkeji.top

Go:   arr[1:4]
来源：http://awj.gogol.net.cn

Ruby: arr[1, 3]
来源：http://ask.yonumen.top

C#:   list.GetRange(1, 3);
来源：http://akb.andypj.xyz

[D08] 合并两个数组
来源：http://lkx.xuetiantiany.cn

Py:   a + b;  a.extend(b)
来源：http://wnw.shzxlz.cn

PHP:  array_merge($a, $b);
来源：http://kvv.kuanghao11.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://hej.yj20258888.top

TS:   [...a, ...b];
来源：http://hxn.gogol.net.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://kxw.guowangkeji.top

Go:   append(a, b...)
来源：http://brh.ehwqpu.com

Ruby: a + b;  a.concat(b)
来源：http://wkp.jqgfzy.top

C#:   a.Concat(b).ToList()
来源：http://cuy.jyoumei.cn

[D09] 排序（升序）
来源：http://lcs.mhx1999.top

Py:   sorted(arr);  arr.sort()
来源：http://myp.ctjpmb.com

PHP:  sort($arr);
来源：http://rqx.hcnkem.com

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://bvt.hesvh.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://gac.snrcjt.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://ydz.52xcode.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://qhc.havefunace.top

Ruby: arr.sort
来源：http://kmb.vehdjk.com

C#:   list.Sort();
来源：http://iwc.hnxiangtu.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://unx.guowangkeji.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://qji.shangyingyoupin.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://pts.uphjek.com

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://yrf.yfazqb.com

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://jof.shuidangran.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://zkp.daria6918.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://jyw.yongpay.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://wcs.yj20258.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://raf.ppjwa.cn

[D11] 反转数组
来源：http://ryd.aibaodan.cn

Py:   arr[::-1];  arr.reverse()
来源：http://qik.pengpengdd.cyou

PHP:  array_reverse($arr);
来源：http://kdn.gogol.net.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://fss.yj20258888.top

TS:   [...arr].reverse();
来源：http://zov.yanxiufei.cn

Java: Collections.reverse(list);
来源：http://dvy.ehwqpu.com

Go:   slices.Reverse(arr)
来源：http://zqc.zycfv.cn

Ruby: arr.reverse
来源：http://kop.zdqjudy.top

C#:   list.Reverse();
来源：http://uop.xylfe.cn

[D12] 查找元素下标
来源：http://lfw.zdqjudy.top

Py:   arr.index(x);  x in arr
来源：http://oeg.nanxuanxn.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://fdj.guannengcc.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://iff.svipenyu.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wev.nanxinkj.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://nad.cqqwz.cn

Go:   slices.Index(arr, x)
来源：http://zug.hcnkem.com

Ruby: arr.index(x)
来源：http://gsx.316326.xyz

C#:   list.IndexOf(x);
来源：http://asl.yueranfly.top

[D13] 过滤（保留满足条件的）
来源：http://jpd.gzhubu.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://fbe.ybcxt.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://lmg.jqgfzy.top

JS:   arr.filter(x => x > 3)
来源：http://zef.fktsv.cn

TS:   arr.filter(x => x > 3)
来源：http://vyv.jqgufenzy.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://gye.316326.xyz

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://weo.sjlbkw.cn

Ruby: arr.select { |x| x > 3 }
来源：http://szt.pycfn.com

C#:   list.Where(x => x > 3).ToList()
来源：http://pqf.xingfuxueyuan.xyz

[D14] 映射转换（每个元素变形）
来源：http://rkd.hnxiangtu.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://qhx.smart0.xyz

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://sao.cheryme.top

JS:   arr.map(x => x * 2)
来源：http://msh.0kj1m.cn

TS:   arr.map(x => x * 2)
来源：http://doz.zhongyouzk.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://aik.yongpay.top

Go:   // 手写循环
来源：http://qma.epnwcf.com

Ruby: arr.map { |x| x * 2 }
来源：http://euq.cqqwz.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://mle.xylfe.cn

[D15] 去重
来源：http://pvu.shzxlz.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://moj.pycfn.com

PHP:  array_unique($arr);
来源：http://hkw.aizwys.cn

JS:   [...new Set(arr)]
来源：http://scx.316326.xyz

TS:   [...new Set(arr)]
来源：http://mtt.jlsjyb.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://yir.pengpengdd.cyou

Go:   // 用 map[T]struct{} 手写
来源：http://dcj.xziqi.cn

Ruby: arr.uniq
来源：http://sjs.hongshengwenyu.top

C#:   list.Distinct().ToList()
来源：http://bcy.feifeiyinyue.top

[D16] 求和与平均值
来源：http://odb.jiagoushi.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://zbv.chenlongwang.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hwk.shangyingyoupin.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://vwe.yuxming.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://rhh.xuanzx.com

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://gqa.ydjk.org.cn

Go:   // 手写循环累加
来源：http://cdh.chenzaomai.com

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://suz.c1oappe.top

C#:   list.Sum();  list.Average()
来源：http://gna.316326.xyz

[D17] 最大值与最小值
来源：http://wxp.hywenlv.cn

Py:   max(arr);  min(arr)
来源：http://qvb.gotoacloud.top

PHP:  max($arr);  min($arr);
来源：http://stn.shuidangran.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://rkn.0kj1m.cn

TS:   Math.max(...arr);
来源：http://ong.smart0.xyz

Java: Collections.max(list);  Collections.min(list);
来源：http://rdn.daria6918.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://rhk.mhx1999.top

Ruby: arr.max;  arr.min
来源：http://koj.sufxvd.cn

C#:   list.Max();  list.Min()
来源：http://vvq.jiagoushi.top

[D18] 扁平化嵌套数组
来源：http://ohq.xinyue.icu

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://jeq.gogol.net.cn

PHP:  array_merge(...$nested);
来源：http://bhl.yanxiufei.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://wot.hnqzz.top

TS:   nested.flat();
来源：http://yef.guowangkeji.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://auk.yuanzhike.top

Go:   // 手写双层循环
来源：http://hpq.daxiang520.top

Ruby: nested.flatten
来源：http://qew.c1oappe.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://khn.gogol.net.cn


<!-- 参考信息 -->