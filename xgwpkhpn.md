代发 wailian999

C#:   string Greet(string name = "World") => name;
来源：http://xhk.fanxiaobao.xyz

[C03] 可变参数
来源：http://ola.shangyingyoupin.top

Py:   def total(*args): return sum(args)
来源：http://vut.havefunace.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://ham.hongshengwenyu.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://zvf.0kj1m.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://jik.c1oappe.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://lng.jinqigfzy.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://zwj.havefunace.top

Ruby: def total(*nums); nums.sum; end
来源：http://pgb.gaohongyu789.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://qii.daria6918.cn

[C04] 命名参数 / 关键字参数
来源：http://yas.nanxinkj.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://kdd.epnwcf.com

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://arg.shanyushiyangtech.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://duo.sysykeji.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://nic.tian-w.cn

Java: // 无：用 Builder 模式或 record
来源：http://hhu.andypj.xyz

Go:   // 无：用配置结构体参数
来源：http://xkp.hnxiangtu.top

Ruby: f(a: 1, b: 2)
来源：http://pyz.nanxinkj.top

C#:   f(a: 1, b: 2)
来源：http://xfp.snrcjt.cn

[C05] 返回多个值
来源：http://vzb.ivvv.top

Py:   return a, b
来源：http://xfk.shanyushiyangkeji.top

PHP:  return [$a, $b];
来源：http://kfe.shanyushiyangkeji.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://vqd.chenlongwang.top

TS:   return { a, b };
来源：http://tqf.snrcjt.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://ypk.shanyushiyangkeji.top

Go:   return a, b
来源：http://xoa.jqgufenzy.top

Ruby: return a, b
来源：http://nbt.iojbl.cn

C#:   return (a, b);              // ValueTuple
来源：http://udd.fktsv.cn

[C06] 匿名函数 / lambda
来源：http://ari.jinyuanbaomall.cn

Py:   square = lambda x: x * x
来源：http://oeo.ywan-chungtsiang.top

PHP:  $square = fn($x) => $x * $x;
来源：http://lcw.dashuyun.cn

JS:   const square = x => x * x;
来源：http://tqj.yueranfly.top

TS:   const square = (x: number): number => x * x;
来源：http://srb.xuanzx.com

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://pwn.birdmap.top

Go:   sq := func(x int) int { return x * x }
来源：http://esc.haohaochexian.top

Ruby: square = ->(x) { x * x }
来源：http://xls.yj20258.top

C#:   Func<int, int> square = x => x * x;
来源：http://apa.chenjidiqi.icu

[C07] 把函数作为参数传入
来源：http://jir.tian-w.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://oht.shanyushiyangkeji.top

PHP:  array_map("strtoupper", $arr);
来源：http://gbu.316326.xyz

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://qlz.yvedp.cn

TS:   arr.map(String)
来源：http://wtg.chenzaomai.com

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://clu.bjfxy.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://ssb.xinyue.icu

Ruby: arr.map(&:upcase)
来源：http://kqz.jianghu66.top

C#:   arr.Select(s => s.ToUpper())
来源：http://kee.xziqi.cn

[C08] 闭包
来源：http://txu.hfpthk.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://owy.pycfn.com

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://gzm.bbcook.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://xgn.tarul.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://zik.xuetiantiany.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://grq.316326.xyz

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://qbc.hcnkem.com

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://cwy.wangshuangyany.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://lus.gogol.net.cn

[C09] 递归
来源：http://uiq.vehdjk.com

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://mnd.jqgfzy.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://jie.jinghuilouyu.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://kdg.quarkkingdee.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ats.gotoacloud.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://uty.yanxiufei.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://lou.jinyuanbaomall.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://myj.jianghu66.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://rgo.zhijiandao.cn

[C10] 变量作用域
来源：http://sol.zhongyouzk.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://rcx.yuanzhike.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://idd.nanxinkj.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://inq.cucudq.cn

TS:   同 JS
来源：http://nra.yuanzhike.top

Java: 方法内为块级作用域
来源：http://clr.guannengcc.top

Go:   花括号块级作用域
来源：http://axs.hfpthk.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://ysx.redwolf501.top

C#:   块级作用域
来源：http://aau.yuxming.cn

[C11] 模块导入与导出
来源：http://nya.yanxiufei.cn

Py:   from module import func
来源：http://meb.dashuyun.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://ktc.sweek.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://rcf.hfpthk.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://mkn.yj202588.top

Java: import java.util.List;
来源：http://jwj.hongshengwenyu.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://vtv.cdnleiting.top

Ruby: require "json"; require_relative "./util"
来源：http://hko.chenzaomai.com

C#:   using System.Text;
来源：http://xjp.iojbl.cn

[C12] 立即执行函数 IIFE
来源：http://jsu.dianchejie.cn

Py:   (lambda: print("run"))()
来源：http://ykz.epnwcf.com

PHP:  (function () { echo "run"; })();
来源：http://ehf.yuanzhike.top

JS:   (() => { console.log("run"); })();
来源：http://mqt.feifeiyinyue.top

TS:   (() => { console.log("run"); })();
来源：http://xqo.xylfe.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://yhl.chenlongwang.top

Go:   func() { fmt.Println("run") }()
来源：http://zzo.sxryk.cn

Ruby: -> { puts "run" }.call
来源：http://kou.shangyingyoupin.top

C#:   // 无 IIFE：用静态构造函数
来源：http://yce.zhiwuduotai.top

[C13] 类型声明 / 类型注解
来源：http://swt.gaohongyu789.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://rre.yuxming.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://eml.sufxvd.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://bvr.nanxuanxn.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mls.daria6918.cn

Java: int add(int a, int b) { return a + b; }
来源：http://izk.zhijiandao.cn

Go:   func add(a, b int) int
来源：http://udo.haohaochexian.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://pwa.ctjpmb.com

C#:   int Add(int a, int b) => a + b;
来源：http://leo.ivvv.top

[C14] 泛型函数
来源：http://vvo.sufxvd.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://xum.cqqwz.cn

PHP:  // 无泛型
来源：http://bmv.yongpay.top

JS:   // 无泛型
来源：http://nmh.yuanzhike.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://fux.kuanghao11.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://ehq.feifeiyinyue.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://dhv.snrcjt.cn

Ruby: # 无泛型
来源：http://odd.jqgufenzy.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://xnb.havefunace.top

[C15] 解构 / 展开参数
来源：http://iku.sysykeji.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://njv.jqgufenzy.top

PHP:  [$a, $b] = $pair;
来源：http://ris.tianlin.xyz

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://fzd.wangshuangyany.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://ceb.meibo888.top

Java: // 无解构
来源：http://ggy.hammf.cn

Go:   // 无解构
来源：http://dzy.jyoumei.cn

Ruby: a, b = pair
来源：http://qkl.jinyuanbaomall.cn

C#:   var (a, b) = pair;
来源：http://kwa.bbcook.cn

[C16] 函数 / 方法重载
来源：http://zre.nwbrower.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://znp.bjfxy.top

PHP:  // 无重载
来源：http://zoo.snrcjt.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://lqu.c1oappe.top

TS:   // 用联合类型或重载签名声明
来源：http://yxa.vqdsnc.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://hwd.hfpthk.cn

Go:   // 无重载：用不同函数名
来源：http://oiw.yonumen.top

Ruby: # 无重载：靠动态参数
来源：http://nzd.sysykeji.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://tqi.iojbl.cn

================================================================================
来源：http://uln.jqgufenzy.top

D. 数组 / 列表 / 集合
来源：http://vwp.shangyingyoupin.top

================================================================================
来源：http://ozx.gaohongyu789.top

[D01] 创建数组 / 列表
来源：http://lom.sjlbkw.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://tvp.xziqi.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hdv.yvedp.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://dba.yanxiufei.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://pfb.kuanghao11.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://mkz.hcnkem.com

Go:   arr := []int{1, 2, 3}
来源：http://gfp.xylfe.cn

Ruby: arr = [1, 2, 3]
来源：http://gxf.yangfankeji.com

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://ota.gogol.net.cn

[D02] 追加元素到末尾
来源：http://zdn.nanxuanxn.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://swk.jyoumei.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://yib.cdnleiting.top

JS:   arr.push(4);
来源：http://ifi.yonumen.top

TS:   arr.push(4);
来源：http://wdn.redwolf501.top

Java: list.add(4);
来源：http://qxc.zhongyouzk.top

Go:   arr = append(arr, 4)
来源：http://yzo.0kj1m.cn

Ruby: arr << 4; arr.push(5)
来源：http://cbb.svipenyu.cn

C#:   list.Add(4);
来源：http://dif.ppjwa.cn

[D03] 在指定位置插入元素
来源：http://awu.mhx1999.top

Py:   arr.insert(0, 0)
来源：http://zam.0kj1m.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://mpt.hcnkem.com

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://zln.gzhubu.top

TS:   arr.splice(0, 0, 0);
来源：http://kpp.nwbrower.top

Java: list.add(0, 0);
来源：http://tps.c1oappe.top

Go:   arr = append([]int{0}, arr...)
来源：http://wkb.quarkkingdee.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://jlv.0kj1m.cn

C#:   list.Insert(0, 0);
来源：http://ggf.kuanghao11.cn

[D04] 删除元素
来源：http://aac.vqdsnc.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://vze.yonumen.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://rvc.zhongyouzk.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hfc.tarul.cn

TS:   arr.splice(0, 1);
来源：http://dsj.bbcook.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://lob.guannengcc.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://qya.andypj.xyz

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://nhq.cheryme.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://ngn.yfazqb.com

[D05] 访问与修改元素
来源：http://lob.zhengqikj.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://dld.zhongyouzk.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://dkx.xylfe.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://ofg.nwbrower.top

TS:   arr[0]; arr.at(-1);
来源：http://ahr.yfazqb.com

Java: list.get(0); list.set(0, 9);
来源：http://sny.aizwys.cn

Go:   arr[0]; arr[0] = 9
来源：http://iwj.xylfe.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hnn.cqqwz.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hxd.ywan-chungtsiang.top

[D06] 数组长度
来源：http://nps.sufxvd.cn

Py:   len(arr)
来源：http://doi.yj20258.top

PHP:  count($arr);
来源：http://ial.shanyushiyangtech.top

JS:   arr.length
来源：http://rvn.yueranfly.top

TS:   arr.length
来源：http://bdy.ehwqpu.com

Java: list.size();
来源：http://ypl.snrcjt.cn

Go:   len(arr)
来源：http://kep.tarul.cn

Ruby: arr.length; arr.size
来源：http://gtq.jinqigfzy.top

C#:   list.Count;
来源：http://akc.316326.xyz

[D07] 切片 / 取子数组
来源：http://amz.chenlongwang.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://yko.zhiwuduotai.top

PHP:  array_slice($arr, 1, 3);
来源：http://oki.jinghuilouyu.cn

JS:   arr.slice(1, 4);
来源：http://mej.wangdashe.top

TS:   arr.slice(1, 4);
来源：http://btx.fktsv.cn

Java: list.subList(1, 4);
来源：http://byx.nwbrower.top

Go:   arr[1:4]
来源：http://esw.bjfxy.top

Ruby: arr[1, 3]
来源：http://zbc.mhx1999.top

C#:   list.GetRange(1, 3);
来源：http://dkg.shanyushiyangkeji.top

[D08] 合并两个数组
来源：http://eab.epnwcf.com

Py:   a + b;  a.extend(b)
来源：http://igu.dashuyun.cn

PHP:  array_merge($a, $b);
来源：http://ebq.ywan-chungtsiang.top

JS:   [...a, ...b];  a.concat(b);
来源：http://ugx.yonumen.top

TS:   [...a, ...b];
来源：http://tgt.haohaochexian.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://udh.kuanghao11.cn

Go:   append(a, b...)
来源：http://vhk.hammf.cn

Ruby: a + b;  a.concat(b)
来源：http://mjr.chenlongwang.top

C#:   a.Concat(b).ToList()
来源：http://xev.jiagoushi.top

[D09] 排序（升序）
来源：http://pik.uphjek.com

Py:   sorted(arr);  arr.sort()
来源：http://rmp.aizwys.cn

PHP:  sort($arr);
来源：http://ghj.haohaochexian.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://vvd.tanke756.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://plb.sxryk.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://mzw.xuetiantiany.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://nin.daria6918.cn

Ruby: arr.sort
来源：http://ayq.zdbjq.cn

C#:   list.Sort();
来源：http://mfz.pengpengdd.cyou

[D10] 自定义排序（按字段 / 多条件）
来源：http://lro.kuanghao11.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://rbi.xuanzx.com

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://lom.yj20258.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://ajz.jqgfzy.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://xql.zhijiandao.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://nzp.gogol.net.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://yfo.jqgufenzy.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://xbz.chenlongwang.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://tiv.tanke756.top

[D11] 反转数组
来源：http://unz.cashguo.top

Py:   arr[::-1];  arr.reverse()
来源：http://aqp.fehbvm.com

PHP:  array_reverse($arr);
来源：http://wbj.smart0.xyz

JS:   [...arr].reverse();  arr.toReversed()
来源：http://vtn.fanxiaobao.xyz

TS:   [...arr].reverse();
来源：http://rss.yj20258888.top

Java: Collections.reverse(list);
来源：http://ipg.daria6918.cn

Go:   slices.Reverse(arr)
来源：http://lgt.ctjpmb.com

Ruby: arr.reverse
来源：http://fxd.yfazqb.com

C#:   list.Reverse();
来源：http://cal.chenzaomai.com

[D12] 查找元素下标
来源：http://kkq.hcnkem.com

Py:   arr.index(x);  x in arr
来源：http://djj.ppjwa.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://mlu.jqgufenzy.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://okv.nanxuanxn.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ezx.zdbjq.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://ejo.zdqjudy.top

Go:   slices.Index(arr, x)
来源：http://onq.nanxinkj.top

Ruby: arr.index(x)
来源：http://npr.shzxlz.cn

C#:   list.IndexOf(x);
来源：http://znm.yuanzhike.top

[D13] 过滤（保留满足条件的）
来源：http://rld.ydjk.org.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://gxg.hcnkem.com

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://zrt.hfpthk.cn

JS:   arr.filter(x => x > 3)
来源：http://gss.fzhhl.top

TS:   arr.filter(x => x > 3)
来源：http://zwa.smart0.xyz

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hcq.hongshengwenyu.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://avb.ydjk.org.cn

Ruby: arr.select { |x| x > 3 }
来源：http://wfm.9152youxi.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://euz.nanxinkj.top

[D14] 映射转换（每个元素变形）
来源：http://xgp.hcnkem.com

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://moe.c1oappe.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://veh.vqdsnc.cn

JS:   arr.map(x => x * 2)
来源：http://zxj.hesvh.cn

TS:   arr.map(x => x * 2)
来源：http://jqp.cheryme.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://sbt.yj20258888.top

Go:   // 手写循环
来源：http://zbl.jqgfzy.top

Ruby: arr.map { |x| x * 2 }
来源：http://iuv.xuanzx.com

C#:   list.Select(x => x * 2).ToList()
来源：http://lwk.yvedp.cn

[D15] 去重
来源：http://ijo.sxryk.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://iat.fktsv.cn

PHP:  array_unique($arr);
来源：http://urn.hcnkem.com

JS:   [...new Set(arr)]
来源：http://yfh.yj202588.top

TS:   [...new Set(arr)]
来源：http://cqe.jlsjyb.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://nfr.nwbrower.top

Go:   // 用 map[T]struct{} 手写
来源：http://aec.bjfxy.top

Ruby: arr.uniq
来源：http://kep.jinqigufen.top

C#:   list.Distinct().ToList()
来源：http://uvq.fengsongda.top

[D16] 求和与平均值
来源：http://xkx.316326.xyz

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://sek.zhixingplan.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://eht.fanxiaobao.xyz

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://rco.shanyushiyangkeji.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://jwa.feifeiyinyue.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://tgi.shanyushiyangkeji.top

Go:   // 手写循环累加
来源：http://fai.tanke756.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://imw.hfpthk.cn

C#:   list.Sum();  list.Average()
来源：http://oda.pycfn.com

[D17] 最大值与最小值
来源：http://qui.jinyuanbaomall.cn

Py:   max(arr);  min(arr)
来源：http://ufe.pengpengdd.cyou

PHP:  max($arr);  min($arr);
来源：http://yvj.zhijiandao.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://lpm.xuetiantiany.cn

TS:   Math.max(...arr);
来源：http://dsf.gotoacloud.top

Java: Collections.max(list);  Collections.min(list);
来源：http://zku.feifeiyinyue.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://olk.xuanzx.com

Ruby: arr.max;  arr.min
来源：http://cqj.yj202588.top

C#:   list.Max();  list.Min()
来源：http://ubk.ydzc1.top

[D18] 扁平化嵌套数组
来源：http://nii.cqqwz.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://eqd.yj20258.top

PHP:  array_merge(...$nested);
来源：http://bzy.yueranfly.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://nbl.yangfankeji.com

TS:   nested.flat();
来源：http://ezn.feifeiyinyue.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://boi.meibo888.top

Go:   // 手写双层循环
来源：http://zbu.epnwcf.com

Ruby: nested.flatten
来源：http://fgf.gaohongyu789.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://fwj.cdnleiting.top

[D19] 按字段分组
来源：http://qly.vehdjk.com

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://oyz.meibo888.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://axr.ydjk.org.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://gwt.dashuyun.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://zhf.bjfxy.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://ekl.yj20258.top

Go:   // 手写 map[string][]T
来源：http://qin.daxiang520.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://pmx.pycfn.com


<!-- 参考信息 -->