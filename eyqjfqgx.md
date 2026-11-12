代发 wailian999

TS:   function greet(name: string = "World") { return name; }
来源：http://gvs.xingfuxueyuan.xyz

Java: // 无默认参数：方法重载或 Optional
来源：http://vry.ydjk.org.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://buq.redwolf501.top

Ruby: def greet(name = "World") = name
来源：http://ocg.jiagoushi.top

C#:   string Greet(string name = "World") => name;
来源：http://wia.ivvv.top

[C03] 可变参数
来源：http://gii.yongpay.top

Py:   def total(*args): return sum(args)
来源：http://lcl.yanxiufei.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://eiy.meibo888.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://pnh.yj202588.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://gmq.shanyushiyangkeji.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://bbb.tanke756.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hpy.fehbvm.com

Ruby: def total(*nums); nums.sum; end
来源：http://yek.shuidangran.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://qgg.fanxiaobao.xyz

[C04] 命名参数 / 关键字参数
来源：http://whb.vehdjk.com

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://loe.ywan-chungtsiang.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://qnk.bbcook.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://gju.zhaomingkeji.xyz

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://ppt.daria6918.cn

Java: // 无：用 Builder 模式或 record
来源：http://wsy.vqdsnc.cn

Go:   // 无：用配置结构体参数
来源：http://hol.hesvh.cn

Ruby: f(a: 1, b: 2)
来源：http://cvj.hywenlv.cn

C#:   f(a: 1, b: 2)
来源：http://jdp.sjlbkw.cn

[C05] 返回多个值
来源：http://hvt.zhixingplan.top

Py:   return a, b
来源：http://ggp.kuanghao11.cn

PHP:  return [$a, $b];
来源：http://qpi.quarkkingdee.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://yok.bbcook.cn

TS:   return { a, b };
来源：http://ssn.gzhubu.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://nkw.hysaishi.cn

Go:   return a, b
来源：http://mjx.jqgfzy.top

Ruby: return a, b
来源：http://udk.xingfuxueyuan.xyz

C#:   return (a, b);              // ValueTuple
来源：http://vnk.gogol.net.cn

[C06] 匿名函数 / lambda
来源：http://nyi.birdmap.top

Py:   square = lambda x: x * x
来源：http://wjt.pycfn.com

PHP:  $square = fn($x) => $x * $x;
来源：http://zth.jinqigufen.top

JS:   const square = x => x * x;
来源：http://kmt.fanxiaobao.xyz

TS:   const square = (x: number): number => x * x;
来源：http://bcx.cqqwz.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://qhh.xingfuxueyuan.xyz

Go:   sq := func(x int) int { return x * x }
来源：http://tbu.sufxvd.cn

Ruby: square = ->(x) { x * x }
来源：http://pfq.hfpthk.cn

C#:   Func<int, int> square = x => x * x;
来源：http://ebf.316326.xyz

[C07] 把函数作为参数传入
来源：http://ohz.pengpengdd.cyou

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://pba.smart0.xyz

PHP:  array_map("strtoupper", $arr);
来源：http://zfx.fzhhl.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://caj.wangdashe.top

TS:   arr.map(String)
来源：http://ylg.hfpthk.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://idr.smart0.xyz

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://gqj.birdmap.top

Ruby: arr.map(&:upcase)
来源：http://ccv.hcnkem.com

C#:   arr.Select(s => s.ToUpper())
来源：http://tap.hnqzz.top

[C08] 闭包
来源：http://cjy.ydzc1.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://jqy.redwolf501.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://axs.sweek.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hqk.chenjidiqi.icu

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://kjs.jinqigfzy.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://jmv.sufxvd.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://aui.tianlin.xyz

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://lht.chenlongwang.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://njg.pengpengdd.cyou

[C09] 递归
来源：http://unc.hesvh.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hdi.fehbvm.com

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://czs.cashguo.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ply.yanxiufei.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://bol.jiagoushi.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://jzz.bbcook.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://fqf.zhengqikj.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://gqf.zhongyouzk.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://opa.hesvh.cn

[C10] 变量作用域
来源：http://oxh.0kj1m.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://rsv.shanyushiyangkeji.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://mmz.tarul.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://mqe.daria6918.cn

TS:   同 JS
来源：http://kmi.hammf.cn

Java: 方法内为块级作用域
来源：http://wxw.jinyuanbaomall.cn

Go:   花括号块级作用域
来源：http://bal.zhixingplan.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hwc.yj20258888.top

C#:   块级作用域
来源：http://qct.yj202588.top

[C11] 模块导入与导出
来源：http://bae.0kj1m.cn

Py:   from module import func
来源：http://ihq.jinqigufen.top

PHP:  require "file.php";  或 use App\Service;
来源：http://ksj.chenlongwang.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://jtz.kuanghao11.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://jdw.shanyushiyangtech.top

Java: import java.util.List;
来源：http://kda.yj20258.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://tcr.yj20258888.top

Ruby: require "json"; require_relative "./util"
来源：http://qrl.mhx1999.top

C#:   using System.Text;
来源：http://dov.shzxlz.cn

[C12] 立即执行函数 IIFE
来源：http://sxe.ywan-chungtsiang.top

Py:   (lambda: print("run"))()
来源：http://sjd.gzhubu.top

PHP:  (function () { echo "run"; })();
来源：http://lgd.cheryme.top

JS:   (() => { console.log("run"); })();
来源：http://lzq.jqgfzy.top

TS:   (() => { console.log("run"); })();
来源：http://mqm.wangdashe.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://pkd.gzhubu.top

Go:   func() { fmt.Println("run") }()
来源：http://ehl.jqgufenzy.top

Ruby: -> { puts "run" }.call
来源：http://vxk.yueranfly.top

C#:   // 无 IIFE：用静态构造函数
来源：http://ocd.zhongyouzk.top

[C13] 类型声明 / 类型注解
来源：http://zoo.cheryme.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://wre.meibo888.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://itj.hysaishi.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://pwf.jiagoushi.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ydb.9152youxi.cn

Java: int add(int a, int b) { return a + b; }
来源：http://kqz.smart0.xyz

Go:   func add(a, b int) int
来源：http://qzf.smart0.xyz

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://sjd.zhixingplan.top

C#:   int Add(int a, int b) => a + b;
来源：http://uxt.0kj1m.cn

[C14] 泛型函数
来源：http://zut.chenlongwang.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://rcz.jqgfzy.top

PHP:  // 无泛型
来源：http://jox.mhx1999.top

JS:   // 无泛型
来源：http://btp.zhiwuduotai.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://xqf.jinyuanbaomall.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://sro.hammf.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://phs.hysaishi.cn

Ruby: # 无泛型
来源：http://hfw.jianghu66.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://pjb.jinyuanbaomall.cn

[C15] 解构 / 展开参数
来源：http://wvo.ivvv.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://rpn.316326.xyz

PHP:  [$a, $b] = $pair;
来源：http://czf.sjlbkw.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://gvn.ctjpmb.com

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://mgh.jqgufenzy.top

Java: // 无解构
来源：http://ekp.yuanzhike.top

Go:   // 无解构
来源：http://ekw.xuanzx.com

Ruby: a, b = pair
来源：http://juj.hammf.cn

C#:   var (a, b) = pair;
来源：http://xlt.bjfxy.top

[C16] 函数 / 方法重载
来源：http://bny.wangshuangyany.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://ppc.pycfn.com

PHP:  // 无重载
来源：http://ruh.zycfv.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://cay.52xcode.cn

TS:   // 用联合类型或重载签名声明
来源：http://elk.vqdsnc.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://dbz.tian-w.cn

Go:   // 无重载：用不同函数名
来源：http://xbz.mhx1999.top

Ruby: # 无重载：靠动态参数
来源：http://nkx.yj202588.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://sjt.yongpay.top

================================================================================
来源：http://hoe.sxryk.cn

D. 数组 / 列表 / 集合
来源：http://ubu.nanxuanxn.top

================================================================================
来源：http://pfj.havefunace.top

[D01] 创建数组 / 列表
来源：http://gim.jinqigufen.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://zep.ehwqpu.com

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://ksv.0kj1m.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://smr.aizwys.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://qir.uphjek.com

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://awi.havefunace.top

Go:   arr := []int{1, 2, 3}
来源：http://jxk.yfazqb.com

Ruby: arr = [1, 2, 3]
来源：http://qgh.hywenlv.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://dmq.xuetiantiany.cn

[D02] 追加元素到末尾
来源：http://ckj.yanxiufei.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://npt.uphjek.com

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://jqi.nanxuanxn.top

JS:   arr.push(4);
来源：http://hyw.daria6918.cn

TS:   arr.push(4);
来源：http://jre.ybcxt.top

Java: list.add(4);
来源：http://xng.jqgufenzy.top

Go:   arr = append(arr, 4)
来源：http://pla.wangshuangyany.cn

Ruby: arr << 4; arr.push(5)
来源：http://rvx.jlsjyb.cn

C#:   list.Add(4);
来源：http://qlf.wangdashe.top

[D03] 在指定位置插入元素
来源：http://oax.sxryk.cn

Py:   arr.insert(0, 0)
来源：http://uub.hysaishi.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://inl.c1oappe.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://rge.zhixingplan.top

TS:   arr.splice(0, 0, 0);
来源：http://bxr.sxryk.cn

Java: list.add(0, 0);
来源：http://nbd.wangshuangyany.cn

Go:   arr = append([]int{0}, arr...)
来源：http://bzh.yj20258.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://fjx.jinqigufen.top

C#:   list.Insert(0, 0);
来源：http://lxx.cheryme.top

[D04] 删除元素
来源：http://vho.zhiwuduotai.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://xja.pengpengdd.cyou

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://vaq.0kj1m.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://zhw.birdmap.top

TS:   arr.splice(0, 1);
来源：http://lzb.gzhubu.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://vhh.tanke756.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://htl.yanxiufei.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://bjw.ywan-chungtsiang.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://mww.bbcook.cn

[D05] 访问与修改元素
来源：http://jdi.ydjk.org.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://tbf.hfpthk.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://aib.hywenlv.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://egx.zdqjudy.top

TS:   arr[0]; arr.at(-1);
来源：http://phs.svipenyu.cn

Java: list.get(0); list.set(0, 9);
来源：http://jwg.daria6918.cn

Go:   arr[0]; arr[0] = 9
来源：http://kpp.yangfankeji.com

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://xap.fanxiaobao.xyz

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://nqp.bbcook.cn

[D06] 数组长度
来源：http://hgx.hywenlv.cn

Py:   len(arr)
来源：http://xyd.jiagoushi.top

PHP:  count($arr);
来源：http://yht.cqqwz.cn

JS:   arr.length
来源：http://vne.andypj.xyz

TS:   arr.length
来源：http://dwf.tian-w.cn

Java: list.size();
来源：http://kco.snrcjt.cn

Go:   len(arr)
来源：http://sok.jyoumei.cn

Ruby: arr.length; arr.size
来源：http://hxb.pengpengdd.cyou

C#:   list.Count;
来源：http://pny.uphjek.com

[D07] 切片 / 取子数组
来源：http://gaf.yueranfly.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://wty.daxiang520.top

PHP:  array_slice($arr, 1, 3);
来源：http://kzd.quarkkingdee.top

JS:   arr.slice(1, 4);
来源：http://wty.jinqigufen.top

TS:   arr.slice(1, 4);
来源：http://ysa.yj20258.top

Java: list.subList(1, 4);
来源：http://zug.zdbjq.cn

Go:   arr[1:4]
来源：http://ymx.xingfuxueyuan.xyz

Ruby: arr[1, 3]
来源：http://cgv.cdnleiting.top

C#:   list.GetRange(1, 3);
来源：http://guz.sufxvd.cn

[D08] 合并两个数组
来源：http://xnu.cheryme.top

Py:   a + b;  a.extend(b)
来源：http://rqo.shuidangran.top

PHP:  array_merge($a, $b);
来源：http://shn.shangyingyoupin.top

JS:   [...a, ...b];  a.concat(b);
来源：http://sah.xingfuxueyuan.xyz

TS:   [...a, ...b];
来源：http://ueq.jqgufenzy.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://zpd.guannengcc.top

Go:   append(a, b...)
来源：http://chh.tianlin.xyz

Ruby: a + b;  a.concat(b)
来源：http://pqm.zhiwuduotai.top

C#:   a.Concat(b).ToList()
来源：http://ced.yueranfly.top

[D09] 排序（升序）
来源：http://xct.shzxlz.cn

Py:   sorted(arr);  arr.sort()
来源：http://xls.cashguo.top

PHP:  sort($arr);
来源：http://fos.316326.xyz

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://eik.xziqi.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://hzx.gaohongyu789.top

Java: Collections.sort(list);  list.sort(null);
来源：http://adj.hywenlv.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://xut.ybcxt.top

Ruby: arr.sort
来源：http://npk.svipenyu.cn

C#:   list.Sort();
来源：http://llm.hcnkem.com

[D10] 自定义排序（按字段 / 多条件）
来源：http://nof.aizwys.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://gcv.sufxvd.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://dvr.hammf.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://xvl.pycfn.com

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hly.nwbrower.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://elx.fzhhl.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://heo.meibo888.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://iza.andypj.xyz

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://bko.hysaishi.cn

[D11] 反转数组
来源：http://wxb.cheryme.top

Py:   arr[::-1];  arr.reverse()
来源：http://zaa.jinqigfzy.top

PHP:  array_reverse($arr);
来源：http://ecj.snrcjt.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://qao.redwolf501.top

TS:   [...arr].reverse();
来源：http://zfd.hfpthk.cn

Java: Collections.reverse(list);
来源：http://rhg.andypj.xyz

Go:   slices.Reverse(arr)
来源：http://lei.zdbjq.cn

Ruby: arr.reverse
来源：http://kec.jinqigfzy.top

C#:   list.Reverse();
来源：http://eqk.tian-w.cn

[D12] 查找元素下标
来源：http://imr.daria6918.cn

Py:   arr.index(x);  x in arr
来源：http://gfp.chenjidiqi.icu

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://fit.shanyushiyangkeji.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://prp.hywenlv.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://eil.shanyushiyangtech.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://aaf.daria6918.cn

Go:   slices.Index(arr, x)
来源：http://hnn.yonumen.top

Ruby: arr.index(x)
来源：http://klb.zhijiandao.cn

C#:   list.IndexOf(x);
来源：http://wpv.aizwys.cn

[D13] 过滤（保留满足条件的）
来源：http://knd.ydjk.org.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://zes.hnqzz.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://pjd.chenjidiqi.icu

JS:   arr.filter(x => x > 3)
来源：http://tzj.yongpay.top

TS:   arr.filter(x => x > 3)
来源：http://acg.hywenlv.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://xpp.ppjwa.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://icc.iojbl.cn

Ruby: arr.select { |x| x > 3 }
来源：http://qyx.cdnleiting.top

C#:   list.Where(x => x > 3).ToList()
来源：http://zig.nanxinkj.top

[D14] 映射转换（每个元素变形）
来源：http://asj.zhongyouzk.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://xoc.gotoacloud.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://pjb.jqgfzy.top

JS:   arr.map(x => x * 2)
来源：http://fbu.shzxlz.cn

TS:   arr.map(x => x * 2)
来源：http://grl.quarkkingdee.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://sfs.c1oappe.top

Go:   // 手写循环
来源：http://uot.epnwcf.com

Ruby: arr.map { |x| x * 2 }
来源：http://vjk.hysaishi.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://jph.zhengqikj.top

[D15] 去重
来源：http://jus.dianchejie.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://rvs.sysykeji.top

PHP:  array_unique($arr);
来源：http://lfj.sxryk.cn

JS:   [...new Set(arr)]
来源：http://ydn.andypj.xyz

TS:   [...new Set(arr)]
来源：http://sap.ctjpmb.com

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://axo.hywenlv.cn

Go:   // 用 map[T]struct{} 手写
来源：http://sli.kuanghao11.cn

Ruby: arr.uniq
来源：http://qzh.zhixingplan.top

C#:   list.Distinct().ToList()
来源：http://zyx.wangshuangyany.cn

[D16] 求和与平均值
来源：http://ubr.chenzaomai.com

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://xcl.wangdashe.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://quy.c1oappe.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://cyh.yueranfly.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://kaz.cqqwz.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://cvl.zhongyouzk.top

Go:   // 手写循环累加
来源：http://ucj.uphjek.com

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://mtl.cqqwz.cn

C#:   list.Sum();  list.Average()
来源：http://gsd.chenjidiqi.icu

[D17] 最大值与最小值
来源：http://crz.yfazqb.com

Py:   max(arr);  min(arr)
来源：http://nnk.shuidangran.top

PHP:  max($arr);  min($arr);
来源：http://enk.zhaomingkeji.xyz

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://lpn.epnwcf.com

TS:   Math.max(...arr);
来源：http://zyn.jinghuilouyu.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://fne.zhiwuduotai.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://rwt.chenzaomai.com

Ruby: arr.max;  arr.min
来源：http://jix.chenjidiqi.icu

C#:   list.Max();  list.Min()
来源：http://wht.wangshuangyany.cn

[D18] 扁平化嵌套数组
来源：http://eie.ydjk.org.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://dti.havefunace.top

PHP:  array_merge(...$nested);
来源：http://lfp.fzhhl.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://jjk.hammf.cn

TS:   nested.flat();
来源：http://aoh.hammf.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://rir.sxryk.cn

Go:   // 手写双层循环
来源：http://ddj.cdnleiting.top

Ruby: nested.flatten
来源：http://omh.9152youxi.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://xhm.epnwcf.com

[D19] 按字段分组
来源：http://zzz.dashuyun.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://knf.fanxiaobao.xyz

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://eah.zhaomingkeji.xyz

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://zyr.hywenlv.cn


<!-- 参考信息 -->