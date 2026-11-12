代发 wailian999

TS:   function greet(name: string = "World") { return name; }
来源：http://kja.jinqigufen.top

Java: // 无默认参数：方法重载或 Optional
来源：http://wzr.vehdjk.com

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://sgf.guannengcc.top

Ruby: def greet(name = "World") = name
来源：http://wcr.zdqjudy.top

C#:   string Greet(string name = "World") => name;
来源：http://cpy.xinyue.icu

[C03] 可变参数
来源：http://rkz.hywenlv.cn

Py:   def total(*args): return sum(args)
来源：http://pqp.jiagoushi.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://wph.yuanzhike.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://ovr.havefunace.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://qeq.cqqwz.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://ryv.ybcxt.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://oly.tanke756.top

Ruby: def total(*nums); nums.sum; end
来源：http://dbe.yuxming.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://kor.52xcode.cn

[C04] 命名参数 / 关键字参数
来源：http://xvf.0kj1m.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://xqj.nanxuanxn.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://elh.svipenyu.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://azh.ivvv.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://ink.jinqigufen.top

Java: // 无：用 Builder 模式或 record
来源：http://zdz.iojbl.cn

Go:   // 无：用配置结构体参数
来源：http://wyw.ctjpmb.com

Ruby: f(a: 1, b: 2)
来源：http://uyg.cheryme.top

C#:   f(a: 1, b: 2)
来源：http://ubt.gzhubu.top

[C05] 返回多个值
来源：http://ilm.birdmap.top

Py:   return a, b
来源：http://orl.zhoulong.xyz

PHP:  return [$a, $b];
来源：http://qgq.iojbl.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://duw.kuanghao11.cn

TS:   return { a, b };
来源：http://llk.aizwys.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://xtn.hongshengwenyu.top

Go:   return a, b
来源：http://psr.meibo888.top

Ruby: return a, b
来源：http://dug.xinyue.icu

C#:   return (a, b);              // ValueTuple
来源：http://kyt.yueranfly.top

[C06] 匿名函数 / lambda
来源：http://ttw.bjfxy.top

Py:   square = lambda x: x * x
来源：http://yaa.sufxvd.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://jvq.uphjek.com

JS:   const square = x => x * x;
来源：http://gho.guannengcc.top

TS:   const square = (x: number): number => x * x;
来源：http://dce.hesvh.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://jma.fktsv.cn

Go:   sq := func(x int) int { return x * x }
来源：http://dxc.yonumen.top

Ruby: square = ->(x) { x * x }
来源：http://pfi.zhongyouzk.top

C#:   Func<int, int> square = x => x * x;
来源：http://jpm.jinqigufen.top

[C07] 把函数作为参数传入
来源：http://gxi.yonumen.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://slq.hywenlv.cn

PHP:  array_map("strtoupper", $arr);
来源：http://yyb.xuetiantiany.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://nll.birdmap.top

TS:   arr.map(String)
来源：http://wsq.tanke756.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://gsk.fktsv.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://xad.dianchejie.cn

Ruby: arr.map(&:upcase)
来源：http://hza.yvedp.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://ylz.daxiang520.top

[C08] 闭包
来源：http://laa.iojbl.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://sig.wangshuangyany.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://ksc.nanxuanxn.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://igz.zhongyouzk.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://bwl.jinqigufen.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://yop.redwolf501.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://kxf.jinyuanbaomall.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://ljl.jqgufenzy.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://pct.cdnleiting.top

[C09] 递归
来源：http://kye.yongpay.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://kru.cqqwz.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://abv.jinghuilouyu.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://qve.uphjek.com

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://cyg.zhijiandao.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://zgc.gaohongyu789.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://byj.gotoacloud.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://dsi.jinqigufen.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://bde.ybcxt.top

[C10] 变量作用域
来源：http://nda.aibaodan.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://aib.shangyingyoupin.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://lvc.zhoulong.xyz

JS:   let/const 块级作用域，var 函数级作用域
来源：http://oqk.jqgufenzy.top

TS:   同 JS
来源：http://xrt.jyoumei.cn

Java: 方法内为块级作用域
来源：http://zpy.cdnleiting.top

Go:   花括号块级作用域
来源：http://hfx.ywan-chungtsiang.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://zhi.xingfuxueyuan.xyz

C#:   块级作用域
来源：http://xnu.xinyue.icu

[C11] 模块导入与导出
来源：http://xxj.zhoulong.xyz

Py:   from module import func
来源：http://iqr.zhixingplan.top

PHP:  require "file.php";  或 use App\Service;
来源：http://zfl.sysykeji.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://gtu.jinqigfzy.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://jdp.shanyushiyangtech.top

Java: import java.util.List;
来源：http://irq.dianchejie.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://urs.guowangkeji.top

Ruby: require "json"; require_relative "./util"
来源：http://kvx.sysykeji.top

C#:   using System.Text;
来源：http://xyd.jinghuilouyu.cn

[C12] 立即执行函数 IIFE
来源：http://tor.chenlongwang.top

Py:   (lambda: print("run"))()
来源：http://oqh.zdbjq.cn

PHP:  (function () { echo "run"; })();
来源：http://pyj.cqqwz.cn

JS:   (() => { console.log("run"); })();
来源：http://hcy.yuanzhike.top

TS:   (() => { console.log("run"); })();
来源：http://wsz.xylfe.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://gwo.jinyuanbaomall.cn

Go:   func() { fmt.Println("run") }()
来源：http://hvh.xziqi.cn

Ruby: -> { puts "run" }.call
来源：http://aqu.zdbjq.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://dkp.yj202588.top

[C13] 类型声明 / 类型注解
来源：http://yxj.zhengqikj.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://yly.zhijiandao.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ifq.fanxiaobao.xyz

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hda.vehdjk.com

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wym.jinyuanbaomall.cn

Java: int add(int a, int b) { return a + b; }
来源：http://nsa.sufxvd.cn

Go:   func add(a, b int) int
来源：http://xml.quarkkingdee.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://bqi.tarul.cn

C#:   int Add(int a, int b) => a + b;
来源：http://gac.jqgfzy.top

[C14] 泛型函数
来源：http://zio.hammf.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://byd.xuanzx.com

PHP:  // 无泛型
来源：http://mbr.yvedp.cn

JS:   // 无泛型
来源：http://nvk.jlsjyb.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://ekm.daria6918.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://mwt.vehdjk.com

Go:   func First[T any](items []T) T { return items[0] }
来源：http://fwl.yfazqb.com

Ruby: # 无泛型
来源：http://ihw.sxryk.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://ykb.yuxming.cn

[C15] 解构 / 展开参数
来源：http://sgl.kuanghao11.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://bva.quarkkingdee.top

PHP:  [$a, $b] = $pair;
来源：http://zmt.ydjk.org.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://vfa.xylfe.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://zls.cheryme.top

Java: // 无解构
来源：http://ulo.cqqwz.cn

Go:   // 无解构
来源：http://nfz.nanxuanxn.top

Ruby: a, b = pair
来源：http://wsq.jqgufenzy.top

C#:   var (a, b) = pair;
来源：http://gcw.aibaodan.cn

[C16] 函数 / 方法重载
来源：http://kcu.pengpengdd.cyou

Py:   # 无重载：用默认参数或 *args 变通
来源：http://bhx.fktsv.cn

PHP:  // 无重载
来源：http://czq.daria6918.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://bsk.316326.xyz

TS:   // 用联合类型或重载签名声明
来源：http://aid.sufxvd.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://aql.yj202588.top

Go:   // 无重载：用不同函数名
来源：http://gim.9152youxi.cn

Ruby: # 无重载：靠动态参数
来源：http://zrt.gaohongyu789.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://gxy.shzxlz.cn

================================================================================
来源：http://wah.mhx1999.top

D. 数组 / 列表 / 集合
来源：http://gbo.hammf.cn

================================================================================
来源：http://dmm.yfazqb.com

[D01] 创建数组 / 列表
来源：http://exk.cashguo.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://gfr.guannengcc.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://nox.tarul.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://bfu.jqgufenzy.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://rui.zhengqikj.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://mmd.wangdashe.top

Go:   arr := []int{1, 2, 3}
来源：http://chw.shanyushiyangtech.top

Ruby: arr = [1, 2, 3]
来源：http://tbu.0kj1m.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://aqm.cheryme.top

[D02] 追加元素到末尾
来源：http://hqt.hongshengwenyu.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://mel.xziqi.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://zru.kuanghao11.cn

JS:   arr.push(4);
来源：http://bzm.zhoulong.xyz

TS:   arr.push(4);
来源：http://txg.fktsv.cn

Java: list.add(4);
来源：http://ejw.zhengqikj.top

Go:   arr = append(arr, 4)
来源：http://hne.hongshengwenyu.top

Ruby: arr << 4; arr.push(5)
来源：http://vxg.aibaodan.cn

C#:   list.Add(4);
来源：http://ekb.yuanzhike.top

[D03] 在指定位置插入元素
来源：http://dsx.ywan-chungtsiang.top

Py:   arr.insert(0, 0)
来源：http://hfm.bjfxy.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hwg.tanke756.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://djr.jiagoushi.top

TS:   arr.splice(0, 0, 0);
来源：http://rmq.zhongyouzk.top

Java: list.add(0, 0);
来源：http://bny.hammf.cn

Go:   arr = append([]int{0}, arr...)
来源：http://kpu.316326.xyz

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://uur.zhongyouzk.top

C#:   list.Insert(0, 0);
来源：http://lkr.birdmap.top

[D04] 删除元素
来源：http://ios.chenzaomai.com

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://yca.shanyushiyangkeji.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://nvu.tanke756.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://khp.nanxinkj.top

TS:   arr.splice(0, 1);
来源：http://mqa.vehdjk.com

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://zpn.yanxiufei.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://rck.bbcook.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://gnn.kuanghao11.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://dup.zdqjudy.top

[D05] 访问与修改元素
来源：http://vik.chenjidiqi.icu

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://cwm.xziqi.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://acw.hfpthk.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://sdg.cdnleiting.top

TS:   arr[0]; arr.at(-1);
来源：http://ugr.shanyushiyangtech.top

Java: list.get(0); list.set(0, 9);
来源：http://cpe.hywenlv.cn

Go:   arr[0]; arr[0] = 9
来源：http://gsl.guowangkeji.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://sau.cdnleiting.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://thw.cqqwz.cn

[D06] 数组长度
来源：http://wzy.chenlongwang.top

Py:   len(arr)
来源：http://xoi.jinqigufen.top

PHP:  count($arr);
来源：http://elv.shanyushiyangtech.top

JS:   arr.length
来源：http://tvn.zhoulong.xyz

TS:   arr.length
来源：http://pnz.nwbrower.top

Java: list.size();
来源：http://paa.xziqi.cn

Go:   len(arr)
来源：http://elz.vqdsnc.cn

Ruby: arr.length; arr.size
来源：http://ybm.ydzc1.top

C#:   list.Count;
来源：http://khe.hfpthk.cn

[D07] 切片 / 取子数组
来源：http://amz.aizwys.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://npw.gaohongyu789.top

PHP:  array_slice($arr, 1, 3);
来源：http://asp.zhengqikj.top

JS:   arr.slice(1, 4);
来源：http://rvs.cashguo.top

TS:   arr.slice(1, 4);
来源：http://hdl.gogol.net.cn

Java: list.subList(1, 4);
来源：http://yrg.sufxvd.cn

Go:   arr[1:4]
来源：http://oxi.vehdjk.com

Ruby: arr[1, 3]
来源：http://xgs.9152youxi.cn

C#:   list.GetRange(1, 3);
来源：http://xji.sweek.top

[D08] 合并两个数组
来源：http://mad.zhixingplan.top

Py:   a + b;  a.extend(b)
来源：http://rdd.jinyuanbaomall.cn

PHP:  array_merge($a, $b);
来源：http://eoa.redwolf501.top

JS:   [...a, ...b];  a.concat(b);
来源：http://ytt.yangfankeji.com

TS:   [...a, ...b];
来源：http://ivg.quarkkingdee.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://lqh.yueranfly.top

Go:   append(a, b...)
来源：http://qru.pycfn.com

Ruby: a + b;  a.concat(b)
来源：http://glf.jyoumei.cn

C#:   a.Concat(b).ToList()
来源：http://ufp.haohaochexian.top

[D09] 排序（升序）
来源：http://ifo.zhongyouzk.top

Py:   sorted(arr);  arr.sort()
来源：http://wab.zhoulong.xyz

PHP:  sort($arr);
来源：http://ylu.tian-w.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://rjb.quarkkingdee.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://fmh.pycfn.com

Java: Collections.sort(list);  list.sort(null);
来源：http://pqy.shzxlz.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://ctc.zhixingplan.top

Ruby: arr.sort
来源：http://xbe.wangshuangyany.cn

C#:   list.Sort();
来源：http://xqb.zhiwuduotai.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://deu.hammf.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://gtc.gzhubu.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://dfi.havefunace.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://zkn.jiagoushi.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://trd.yfazqb.com

Java: list.sort(Comparator.comparing(Person::age));
来源：http://kuq.shanyushiyangkeji.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://qkv.hongshengwenyu.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://xex.jqgufenzy.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://ldg.havefunace.top

[D11] 反转数组
来源：http://jib.aibaodan.cn

Py:   arr[::-1];  arr.reverse()
来源：http://ehm.jiagoushi.top

PHP:  array_reverse($arr);
来源：http://esx.redwolf501.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://mig.sjlbkw.cn

TS:   [...arr].reverse();
来源：http://cni.cheryme.top

Java: Collections.reverse(list);
来源：http://pwr.pengpengdd.cyou

Go:   slices.Reverse(arr)
来源：http://fxx.sxryk.cn

Ruby: arr.reverse
来源：http://ctr.nanxinkj.top

C#:   list.Reverse();
来源：http://yqn.zhixingplan.top

[D12] 查找元素下标
来源：http://rgt.zhongyouzk.top

Py:   arr.index(x);  x in arr
来源：http://ulp.zdbjq.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://vrb.yongpay.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://uma.vehdjk.com

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://imp.jlsjyb.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://csz.jyoumei.cn

Go:   slices.Index(arr, x)
来源：http://lpz.yvedp.cn

Ruby: arr.index(x)
来源：http://ksu.andypj.xyz

C#:   list.IndexOf(x);
来源：http://qoc.cucudq.cn

[D13] 过滤（保留满足条件的）
来源：http://tgi.hywenlv.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://lup.sufxvd.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://xvn.pengpengdd.cyou

JS:   arr.filter(x => x > 3)
来源：http://flq.zycfv.cn

TS:   arr.filter(x => x > 3)
来源：http://axk.fzhhl.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://bik.ehwqpu.com

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://rdg.hywenlv.cn

Ruby: arr.select { |x| x > 3 }
来源：http://hdy.yueranfly.top

C#:   list.Where(x => x > 3).ToList()
来源：http://wud.wangshuangyany.cn

[D14] 映射转换（每个元素变形）
来源：http://kgp.gogol.net.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://igi.sysykeji.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://wcb.nwbrower.top

JS:   arr.map(x => x * 2)
来源：http://eqa.gzhubu.top

TS:   arr.map(x => x * 2)
来源：http://baf.aizwys.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://xmq.feifeiyinyue.top

Go:   // 手写循环
来源：http://bxg.jinghuilouyu.cn

Ruby: arr.map { |x| x * 2 }
来源：http://tnz.sufxvd.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://cey.bjfxy.top

[D15] 去重
来源：http://erh.redwolf501.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://bna.jqgfzy.top

PHP:  array_unique($arr);
来源：http://xnq.yueranfly.top

JS:   [...new Set(arr)]
来源：http://krc.zhengqikj.top

TS:   [...new Set(arr)]
来源：http://rsl.zdqjudy.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://duf.pycfn.com

Go:   // 用 map[T]struct{} 手写
来源：http://xto.ctjpmb.com

Ruby: arr.uniq
来源：http://wxf.xziqi.cn

C#:   list.Distinct().ToList()
来源：http://hby.meibo888.top

[D16] 求和与平均值
来源：http://bip.chenlongwang.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://bmk.xylfe.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://dxg.xylfe.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://bta.sweek.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://yrz.316326.xyz

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://pml.pycfn.com

Go:   // 手写循环累加
来源：http://dzz.fzhhl.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://czc.gaohongyu789.top

C#:   list.Sum();  list.Average()
来源：http://mkv.hysaishi.cn

[D17] 最大值与最小值
来源：http://sul.sxryk.cn

Py:   max(arr);  min(arr)
来源：http://nhi.zdbjq.cn

PHP:  max($arr);  min($arr);
来源：http://crw.sweek.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://dds.yj202588.top

TS:   Math.max(...arr);
来源：http://hpb.hcnkem.com

Java: Collections.max(list);  Collections.min(list);
来源：http://bdy.cucudq.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://zxf.zhongyouzk.top

Ruby: arr.max;  arr.min
来源：http://tav.tarul.cn

C#:   list.Max();  list.Min()
来源：http://evo.ppjwa.cn

[D18] 扁平化嵌套数组
来源：http://oov.yuanzhike.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://ttd.zhijiandao.cn

PHP:  array_merge(...$nested);
来源：http://cpr.feifeiyinyue.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://gbk.guannengcc.top

TS:   nested.flat();
来源：http://pgx.zhixingplan.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://wwi.jqgufenzy.top

Go:   // 手写双层循环
来源：http://lia.hysaishi.cn

Ruby: nested.flatten
来源：http://tju.cheryme.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://xri.yangfankeji.com

[D19] 按字段分组
来源：http://wpb.shanyushiyangtech.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://gfq.zhoulong.xyz

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://rhd.ehwqpu.com

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://nbi.cdnleiting.top


<!-- 参考信息 -->