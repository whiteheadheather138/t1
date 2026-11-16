代发 wailian999

Java: static int add(int a, int b) { return a + b; }
来源：http://yar.fzhhl.top

Go:   func add(a, b int) int { return a + b }
来源：http://ova.wangshuangyany.cn

Ruby: def add(a, b); a + b; end
来源：http://jrs.tianlin.xyz

C#:   static int Add(int a, int b) { return a + b; }
来源：http://zxq.ctjpmb.com

[C02] 默认参数
来源：http://tso.ehwqpu.com

Py:   def greet(name="World"): return name
来源：http://rdf.nanxuanxn.top

PHP:  function greet($name = "World") { return $name; }
来源：http://olf.9152youxi.cn

JS:   function greet(name = "World") { return name; }
来源：http://neh.daria6918.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://jmu.chenzaomai.com

Java: // 无默认参数：方法重载或 Optional
来源：http://ium.hcnkem.com

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://fjl.xingfuxueyuan.xyz

Ruby: def greet(name = "World") = name
来源：http://suf.vqdsnc.cn

C#:   string Greet(string name = "World") => name;
来源：http://cmz.jqgfzy.top

[C03] 可变参数
来源：http://iwo.zhoulong.xyz

Py:   def total(*args): return sum(args)
来源：http://dcb.sxryk.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://eca.nwbrower.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://unw.guowangkeji.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://jet.ydzc1.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://rta.yj20258.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://jge.jinghuilouyu.cn

Ruby: def total(*nums); nums.sum; end
来源：http://cdi.gzhubu.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://gzw.hnqzz.top

[C04] 命名参数 / 关键字参数
来源：http://oyp.yangfankeji.com

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://pgm.ivvv.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://bao.andypj.xyz

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://eos.ctjpmb.com

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://oem.sxryk.cn

Java: // 无：用 Builder 模式或 record
来源：http://qkh.fanxiaobao.xyz

Go:   // 无：用配置结构体参数
来源：http://les.nanxuanxn.top

Ruby: f(a: 1, b: 2)
来源：http://aim.cashguo.top

C#:   f(a: 1, b: 2)
来源：http://phe.nanxuanxn.top

[C05] 返回多个值
来源：http://jdi.hnqzz.top

Py:   return a, b
来源：http://jnl.jqgfzy.top

PHP:  return [$a, $b];
来源：http://sdt.quarkkingdee.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://tvg.yonumen.top

TS:   return { a, b };
来源：http://dxl.cucudq.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://dcn.cucudq.cn

Go:   return a, b
来源：http://qit.sjlbkw.cn

Ruby: return a, b
来源：http://qfq.guowangkeji.top

C#:   return (a, b);              // ValueTuple
来源：http://qem.sufxvd.cn

[C06] 匿名函数 / lambda
来源：http://zkk.zhengqikj.top

Py:   square = lambda x: x * x
来源：http://pyv.fzhhl.top

PHP:  $square = fn($x) => $x * $x;
来源：http://qqk.daxiang520.top

JS:   const square = x => x * x;
来源：http://ccf.ctjpmb.com

TS:   const square = (x: number): number => x * x;
来源：http://mvp.yfazqb.com

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://dde.fktsv.cn

Go:   sq := func(x int) int { return x * x }
来源：http://yws.jinyuanbaomall.cn

Ruby: square = ->(x) { x * x }
来源：http://vac.tian-w.cn

C#:   Func<int, int> square = x => x * x;
来源：http://elb.jqgufenzy.top

[C07] 把函数作为参数传入
来源：http://akz.jinqigfzy.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://whe.hesvh.cn

PHP:  array_map("strtoupper", $arr);
来源：http://fbp.hammf.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://dlb.ppjwa.cn

TS:   arr.map(String)
来源：http://ibg.shanyushiyangtech.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hww.tianlin.xyz

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://urb.chenjidiqi.icu

Ruby: arr.map(&:upcase)
来源：http://jgo.yueranfly.top

C#:   arr.Select(s => s.ToUpper())
来源：http://ehq.9152youxi.cn

[C08] 闭包
来源：http://oxv.yvedp.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://zec.sjlbkw.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://xlw.ehwqpu.com

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://ydz.yfazqb.com

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://npz.cdnleiting.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://rwy.shanyushiyangtech.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://ixo.vqdsnc.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://ftz.zhaomingkeji.xyz

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://bmj.guannengcc.top

[C09] 递归
来源：http://ypl.shzxlz.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://ylc.fktsv.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://sch.hammf.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://pcz.wangshuangyany.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://eub.xuanzx.com

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://nvp.jinqigufen.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://kkt.shanyushiyangtech.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://oof.hnxiangtu.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hpe.guowangkeji.top

[C10] 变量作用域
来源：http://tvp.mhx1999.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://iaa.quarkkingdee.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hmk.smart0.xyz

JS:   let/const 块级作用域，var 函数级作用域
来源：http://jqu.fanxiaobao.xyz

TS:   同 JS
来源：http://ose.smart0.xyz

Java: 方法内为块级作用域
来源：http://ikc.ywan-chungtsiang.top

Go:   花括号块级作用域
来源：http://jes.nwbrower.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://szz.tianlin.xyz

C#:   块级作用域
来源：http://ltk.feifeiyinyue.top

[C11] 模块导入与导出
来源：http://lnv.cashguo.top

Py:   from module import func
来源：http://iwr.hnqzz.top

PHP:  require "file.php";  或 use App\Service;
来源：http://nwx.zhijiandao.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://aar.jiagoushi.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://vtw.gaohongyu789.top

Java: import java.util.List;
来源：http://tbp.hammf.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://ycy.jinyuanbaomall.cn

Ruby: require "json"; require_relative "./util"
来源：http://wfj.nwbrower.top

C#:   using System.Text;
来源：http://vto.yuxming.cn

[C12] 立即执行函数 IIFE
来源：http://jwf.birdmap.top

Py:   (lambda: print("run"))()
来源：http://did.bbcook.cn

PHP:  (function () { echo "run"; })();
来源：http://nzj.sufxvd.cn

JS:   (() => { console.log("run"); })();
来源：http://lxy.gzhubu.top

TS:   (() => { console.log("run"); })();
来源：http://jfe.mhx1999.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://rsa.ctjpmb.com

Go:   func() { fmt.Println("run") }()
来源：http://pyz.andypj.xyz

Ruby: -> { puts "run" }.call
来源：http://iml.mhx1999.top

C#:   // 无 IIFE：用静态构造函数
来源：http://msi.mhx1999.top

[C13] 类型声明 / 类型注解
来源：http://nbx.nwbrower.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://klo.hywenlv.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://qae.zdbjq.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://jsf.shanyushiyangtech.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hby.ydzc1.top

Java: int add(int a, int b) { return a + b; }
来源：http://dcb.ydjk.org.cn

Go:   func add(a, b int) int
来源：http://fgo.birdmap.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://afo.zdqjudy.top

C#:   int Add(int a, int b) => a + b;
来源：http://ssc.aibaodan.cn

[C14] 泛型函数
来源：http://udx.gotoacloud.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://grk.fanxiaobao.xyz

PHP:  // 无泛型
来源：http://nnz.chenjidiqi.icu

JS:   // 无泛型
来源：http://hgh.tanke756.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://afj.zdqjudy.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://mao.iojbl.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://ttl.xuanzx.com

Ruby: # 无泛型
来源：http://eyt.jianghu66.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hip.gzhubu.top

[C15] 解构 / 展开参数
来源：http://obq.zdqjudy.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://xkt.tanke756.top

PHP:  [$a, $b] = $pair;
来源：http://wxr.shangyingyoupin.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://oxs.guowangkeji.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://evo.yuxming.cn

Java: // 无解构
来源：http://vao.tian-w.cn

Go:   // 无解构
来源：http://ium.meibo888.top

Ruby: a, b = pair
来源：http://dpv.jinghuilouyu.cn

C#:   var (a, b) = pair;
来源：http://rcb.9152youxi.cn

[C16] 函数 / 方法重载
来源：http://ozb.mhx1999.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hrj.ydjk.org.cn

PHP:  // 无重载
来源：http://cbp.hnqzz.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://hie.feifeiyinyue.top

TS:   // 用联合类型或重载签名声明
来源：http://kge.ctjpmb.com

Java: void f(int a) {}  void f(String a) {}
来源：http://mhg.hywenlv.cn

Go:   // 无重载：用不同函数名
来源：http://agm.chenlongwang.top

Ruby: # 无重载：靠动态参数
来源：http://gke.zdqjudy.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://sol.hywenlv.cn

================================================================================
来源：http://nku.haohaochexian.top

D. 数组 / 列表 / 集合
来源：http://rmn.hfpthk.cn

================================================================================
来源：http://udo.wangdashe.top

[D01] 创建数组 / 列表
来源：http://feo.epnwcf.com

Py:   arr = [1, 2, 3];  empty = []
来源：http://ruc.bbcook.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://wsm.tarul.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://rjb.bbcook.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://tbo.xinyue.icu

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://wld.jinghuilouyu.cn

Go:   arr := []int{1, 2, 3}
来源：http://jjp.dianchejie.cn

Ruby: arr = [1, 2, 3]
来源：http://pnn.hammf.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://tfz.yanxiufei.cn

[D02] 追加元素到末尾
来源：http://jdn.birdmap.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://ezo.xuanzx.com

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://cxk.yj20258888.top

JS:   arr.push(4);
来源：http://wgq.316326.xyz

TS:   arr.push(4);
来源：http://ujn.tarul.cn

Java: list.add(4);
来源：http://rzm.daria6918.cn

Go:   arr = append(arr, 4)
来源：http://osf.gotoacloud.top

Ruby: arr << 4; arr.push(5)
来源：http://stt.xziqi.cn

C#:   list.Add(4);
来源：http://tlk.nanxinkj.top

[D03] 在指定位置插入元素
来源：http://swf.cqqwz.cn

Py:   arr.insert(0, 0)
来源：http://wwz.yanxiufei.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://fdy.wangdashe.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://nou.nwbrower.top

TS:   arr.splice(0, 0, 0);
来源：http://zzc.hongshengwenyu.top

Java: list.add(0, 0);
来源：http://elk.sysykeji.top

Go:   arr = append([]int{0}, arr...)
来源：http://bvj.pengpengdd.cyou

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://fbq.hysaishi.cn

C#:   list.Insert(0, 0);
来源：http://hyi.yuanzhike.top

[D04] 删除元素
来源：http://nyt.jinqigufen.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://kpc.0kj1m.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hkk.c1oappe.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://wey.snrcjt.cn

TS:   arr.splice(0, 1);
来源：http://yft.mhx1999.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://ezt.gaohongyu789.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://vvn.smart0.xyz

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://bny.vehdjk.com

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://bnd.hongshengwenyu.top

[D05] 访问与修改元素
来源：http://xoo.316326.xyz

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://kax.ppjwa.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://xfv.yanxiufei.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://qvl.yj20258.top

TS:   arr[0]; arr.at(-1);
来源：http://sfv.yanxiufei.cn

Java: list.get(0); list.set(0, 9);
来源：http://msa.chenjidiqi.icu

Go:   arr[0]; arr[0] = 9
来源：http://yxv.jlsjyb.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://ylu.xingfuxueyuan.xyz

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://skg.hnqzz.top

[D06] 数组长度
来源：http://nul.gzhubu.top

Py:   len(arr)
来源：http://qmk.yueranfly.top

PHP:  count($arr);
来源：http://awb.yuanzhike.top

JS:   arr.length
来源：http://ckd.pengpengdd.cyou

TS:   arr.length
来源：http://cte.quarkkingdee.top

Java: list.size();
来源：http://fpv.aibaodan.cn

Go:   len(arr)
来源：http://jyv.wangshuangyany.cn

Ruby: arr.length; arr.size
来源：http://jbo.fktsv.cn

C#:   list.Count;
来源：http://nof.yj20258888.top

[D07] 切片 / 取子数组
来源：http://ktg.haohaochexian.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://aol.andypj.xyz

PHP:  array_slice($arr, 1, 3);
来源：http://fzg.yuanzhike.top

JS:   arr.slice(1, 4);
来源：http://iop.sufxvd.cn

TS:   arr.slice(1, 4);
来源：http://jxw.redwolf501.top

Java: list.subList(1, 4);
来源：http://acy.guannengcc.top

Go:   arr[1:4]
来源：http://qbu.birdmap.top

Ruby: arr[1, 3]
来源：http://gmu.fengsongda.top

C#:   list.GetRange(1, 3);
来源：http://zkk.xuetiantiany.cn

[D08] 合并两个数组
来源：http://ccr.9152youxi.cn

Py:   a + b;  a.extend(b)
来源：http://ccm.shanyushiyangkeji.top

PHP:  array_merge($a, $b);
来源：http://qlh.sufxvd.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://ptd.zycfv.cn

TS:   [...a, ...b];
来源：http://bya.cucudq.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://cwm.9152youxi.cn

Go:   append(a, b...)
来源：http://ver.hammf.cn

Ruby: a + b;  a.concat(b)
来源：http://niw.yueranfly.top

C#:   a.Concat(b).ToList()
来源：http://muz.yfazqb.com

[D09] 排序（升序）
来源：http://tpt.yangfankeji.com

Py:   sorted(arr);  arr.sort()
来源：http://ysz.yj20258.top

PHP:  sort($arr);
来源：http://ctj.shzxlz.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://ciq.yueranfly.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://gkb.chenzaomai.com

Java: Collections.sort(list);  list.sort(null);
来源：http://vxt.chenlongwang.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://yxg.nanxinkj.top

Ruby: arr.sort
来源：http://bnf.xylfe.cn

C#:   list.Sort();
来源：http://jmu.0kj1m.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://uuq.xylfe.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://lgo.hammf.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://fcs.52xcode.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://tyf.shangyingyoupin.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://zse.c1oappe.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://qqn.daria6918.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hwu.tianlin.xyz

Ruby: arr.sort_by { |x| x[:age] }
来源：http://mgp.kuanghao11.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://tnu.fktsv.cn

[D11] 反转数组
来源：http://zlk.dashuyun.cn

Py:   arr[::-1];  arr.reverse()
来源：http://zuf.cashguo.top

PHP:  array_reverse($arr);
来源：http://tes.meibo888.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://aeb.xylfe.cn

TS:   [...arr].reverse();
来源：http://zad.tanke756.top

Java: Collections.reverse(list);
来源：http://lli.smart0.xyz

Go:   slices.Reverse(arr)
来源：http://nxe.jinghuilouyu.cn

Ruby: arr.reverse
来源：http://gan.jinqigufen.top

C#:   list.Reverse();
来源：http://zni.hysaishi.cn

[D12] 查找元素下标
来源：http://kkg.cucudq.cn

Py:   arr.index(x);  x in arr
来源：http://yph.zdqjudy.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://xni.dashuyun.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://jel.havefunace.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://bza.yangfankeji.com

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://ykk.tianlin.xyz

Go:   slices.Index(arr, x)
来源：http://jpx.zdbjq.cn

Ruby: arr.index(x)
来源：http://rsm.chenzaomai.com

C#:   list.IndexOf(x);
来源：http://byo.fehbvm.com

[D13] 过滤（保留满足条件的）
来源：http://ucr.yuanzhike.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://xig.gzhubu.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://kuv.zhongyouzk.top

JS:   arr.filter(x => x > 3)
来源：http://tkv.yj20258.top

TS:   arr.filter(x => x > 3)
来源：http://ada.redwolf501.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hus.guowangkeji.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://wyv.dianchejie.cn

Ruby: arr.select { |x| x > 3 }
来源：http://omu.yj20258.top

C#:   list.Where(x => x > 3).ToList()
来源：http://fze.yuanzhike.top

[D14] 映射转换（每个元素变形）
来源：http://veb.jinqigufen.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://ekh.hfpthk.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://rvl.9152youxi.cn

JS:   arr.map(x => x * 2)
来源：http://pcw.ivvv.top

TS:   arr.map(x => x * 2)
来源：http://bvd.andypj.xyz

Java: list.stream().map(x -> x * 2).toList()
来源：http://pjl.9152youxi.cn

Go:   // 手写循环
来源：http://uoa.gzhubu.top

Ruby: arr.map { |x| x * 2 }
来源：http://ffh.jinqigfzy.top

C#:   list.Select(x => x * 2).ToList()
来源：http://ney.yj20258.top

[D15] 去重
来源：http://brd.hnxiangtu.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://btc.jyoumei.cn

PHP:  array_unique($arr);
来源：http://vkl.sufxvd.cn

JS:   [...new Set(arr)]
来源：http://snw.sufxvd.cn

TS:   [...new Set(arr)]
来源：http://ckq.hesvh.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://jfm.yangfankeji.com

Go:   // 用 map[T]struct{} 手写
来源：http://ego.fktsv.cn

Ruby: arr.uniq
来源：http://hrb.yueranfly.top

C#:   list.Distinct().ToList()
来源：http://ufy.zhoulong.xyz

[D16] 求和与平均值
来源：http://iaz.yfazqb.com

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://oow.yfazqb.com

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://syk.cdnleiting.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://kbp.andypj.xyz

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://ego.kuanghao11.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://siz.tarul.cn

Go:   // 手写循环累加
来源：http://ysz.meibo888.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://bjo.uphjek.com

C#:   list.Sum();  list.Average()
来源：http://uqy.zhijiandao.cn

[D17] 最大值与最小值
来源：http://dnc.aizwys.cn

Py:   max(arr);  min(arr)
来源：http://nbq.zdqjudy.top

PHP:  max($arr);  min($arr);
来源：http://xig.smart0.xyz

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://uao.ydzc1.top

TS:   Math.max(...arr);
来源：http://etu.xylfe.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://qfl.yueranfly.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://tyc.chenlongwang.top

Ruby: arr.max;  arr.min
来源：http://koj.zdbjq.cn

C#:   list.Max();  list.Min()
来源：http://frk.dianchejie.cn

[D18] 扁平化嵌套数组
来源：http://pcn.feifeiyinyue.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://vmx.hesvh.cn

PHP:  array_merge(...$nested);
来源：http://bba.jinghuilouyu.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://zcl.uphjek.com

TS:   nested.flat();
来源：http://gof.52xcode.cn


<!-- 参考信息 -->