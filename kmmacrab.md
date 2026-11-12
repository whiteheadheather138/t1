代发 wailian999

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://fpx.zhongyouzk.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://vnc.vehdjk.com

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://czf.ppjwa.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://ruh.feifeiyinyue.top

Ruby: def total(*nums); nums.sum; end
来源：http://nad.sysykeji.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://kpj.daria6918.cn

[C04] 命名参数 / 关键字参数
来源：http://pek.fzhhl.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://vaf.wangshuangyany.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://glc.hywenlv.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://vbl.fanxiaobao.xyz

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://zkv.yuanzhike.top

Java: // 无：用 Builder 模式或 record
来源：http://fld.hysaishi.cn

Go:   // 无：用配置结构体参数
来源：http://nft.zhixingplan.top

Ruby: f(a: 1, b: 2)
来源：http://qgc.cdnleiting.top

C#:   f(a: 1, b: 2)
来源：http://uyq.zycfv.cn

[C05] 返回多个值
来源：http://civ.c1oappe.top

Py:   return a, b
来源：http://mar.jinghuilouyu.cn

PHP:  return [$a, $b];
来源：http://kvt.svipenyu.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://pbi.feifeiyinyue.top

TS:   return { a, b };
来源：http://btq.dianchejie.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://maa.yj202588.top

Go:   return a, b
来源：http://ddf.shzxlz.cn

Ruby: return a, b
来源：http://ixn.jqgufenzy.top

C#:   return (a, b);              // ValueTuple
来源：http://qjz.gogol.net.cn

[C06] 匿名函数 / lambda
来源：http://ais.fanxiaobao.xyz

Py:   square = lambda x: x * x
来源：http://jvt.nanxuanxn.top

PHP:  $square = fn($x) => $x * $x;
来源：http://amm.gzhubu.top

JS:   const square = x => x * x;
来源：http://ysl.hfpthk.cn

TS:   const square = (x: number): number => x * x;
来源：http://tsb.bbcook.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://ogp.mhx1999.top

Go:   sq := func(x int) int { return x * x }
来源：http://jxg.xziqi.cn

Ruby: square = ->(x) { x * x }
来源：http://nax.vehdjk.com

C#:   Func<int, int> square = x => x * x;
来源：http://wlc.zhixingplan.top

[C07] 把函数作为参数传入
来源：http://xqz.vehdjk.com

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://mju.yfazqb.com

PHP:  array_map("strtoupper", $arr);
来源：http://jgl.nanxuanxn.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://ifq.havefunace.top

TS:   arr.map(String)
来源：http://nyt.xuanzx.com

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://quy.wangshuangyany.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://ate.zdbjq.cn

Ruby: arr.map(&:upcase)
来源：http://fdr.yj20258888.top

C#:   arr.Select(s => s.ToUpper())
来源：http://ggx.nanxinkj.top

[C08] 闭包
来源：http://rgy.chenlongwang.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hgt.jqgfzy.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://pup.yj20258888.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://idc.zhengqikj.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://rth.nanxinkj.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://mum.zhengqikj.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://kgi.yangfankeji.com

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://wfr.jinghuilouyu.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://neq.zdbjq.cn

[C09] 递归
来源：http://qrq.gzhubu.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://sse.havefunace.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://ddb.vehdjk.com

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://siv.cqqwz.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://rob.cqqwz.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://eog.jianghu66.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://dxw.c1oappe.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://izs.jqgfzy.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://seu.ppjwa.cn

[C10] 变量作用域
来源：http://qqv.fehbvm.com

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://fyz.bjfxy.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://gxf.redwolf501.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://pig.0kj1m.cn

TS:   同 JS
来源：http://nhe.cqqwz.cn

Java: 方法内为块级作用域
来源：http://yba.hesvh.cn

Go:   花括号块级作用域
来源：http://sqp.haohaochexian.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://zyv.havefunace.top

C#:   块级作用域
来源：http://oth.zhijiandao.cn

[C11] 模块导入与导出
来源：http://cax.sysykeji.top

Py:   from module import func
来源：http://mvk.nanxinkj.top

PHP:  require "file.php";  或 use App\Service;
来源：http://saw.zdbjq.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://wig.shanyushiyangkeji.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://roz.fktsv.cn

Java: import java.util.List;
来源：http://avo.sysykeji.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://npa.xinyue.icu

Ruby: require "json"; require_relative "./util"
来源：http://kdy.jqgfzy.top

C#:   using System.Text;
来源：http://uaf.jlsjyb.cn

[C12] 立即执行函数 IIFE
来源：http://zvw.hywenlv.cn

Py:   (lambda: print("run"))()
来源：http://odt.316326.xyz

PHP:  (function () { echo "run"; })();
来源：http://eru.yuanzhike.top

JS:   (() => { console.log("run"); })();
来源：http://ayz.sjlbkw.cn

TS:   (() => { console.log("run"); })();
来源：http://ofl.zycfv.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://okh.jyoumei.cn

Go:   func() { fmt.Println("run") }()
来源：http://tdv.epnwcf.com

Ruby: -> { puts "run" }.call
来源：http://kdj.ybcxt.top

C#:   // 无 IIFE：用静态构造函数
来源：http://rje.ehwqpu.com

[C13] 类型声明 / 类型注解
来源：http://qaj.jinghuilouyu.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://jqk.epnwcf.com

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wsy.cucudq.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://czk.tarul.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://szf.cucudq.cn

Java: int add(int a, int b) { return a + b; }
来源：http://hrx.c1oappe.top

Go:   func add(a, b int) int
来源：http://ufz.jyoumei.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://lkt.shangyingyoupin.top

C#:   int Add(int a, int b) => a + b;
来源：http://xln.jiagoushi.top

[C14] 泛型函数
来源：http://ltp.hesvh.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://cvj.feifeiyinyue.top

PHP:  // 无泛型
来源：http://tbw.ydjk.org.cn

JS:   // 无泛型
来源：http://rtq.hfpthk.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://bnb.shanyushiyangtech.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://fgc.birdmap.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://zoe.cucudq.cn

Ruby: # 无泛型
来源：http://yet.yanxiufei.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://dbh.kuanghao11.cn

[C15] 解构 / 展开参数
来源：http://cxh.c1oappe.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://ydv.0kj1m.cn

PHP:  [$a, $b] = $pair;
来源：http://wsh.xylfe.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://jox.yuxming.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://mmv.chenzaomai.com

Java: // 无解构
来源：http://yjy.guannengcc.top

Go:   // 无解构
来源：http://pxi.aibaodan.cn

Ruby: a, b = pair
来源：http://tmu.pycfn.com

C#:   var (a, b) = pair;
来源：http://bly.ehwqpu.com

[C16] 函数 / 方法重载
来源：http://ctz.cdnleiting.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://elt.ivvv.top

PHP:  // 无重载
来源：http://pwt.uphjek.com

JS:   // 无重载：靠 arguments.length 分支
来源：http://bdd.fktsv.cn

TS:   // 用联合类型或重载签名声明
来源：http://jzv.zhengqikj.top

Java: void f(int a) {}  void f(String a) {}
来源：http://btc.hcnkem.com

Go:   // 无重载：用不同函数名
来源：http://yww.zdqjudy.top

Ruby: # 无重载：靠动态参数
来源：http://ucf.fehbvm.com

C#:   void F(int a) {}  void F(string a) {}
来源：http://rfa.tian-w.cn

================================================================================
来源：http://jrz.sysykeji.top

D. 数组 / 列表 / 集合
来源：http://nxh.chenlongwang.top

================================================================================
来源：http://afy.ehwqpu.com

[D01] 创建数组 / 列表
来源：http://ivm.zycfv.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://dkg.316326.xyz

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://zsy.jiagoushi.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://nxd.jiagoushi.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://uam.jianghu66.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://uix.fengsongda.top

Go:   arr := []int{1, 2, 3}
来源：http://qrz.nanxuanxn.top

Ruby: arr = [1, 2, 3]
来源：http://ahd.jianghu66.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://yva.hnxiangtu.top

[D02] 追加元素到末尾
来源：http://fkq.tianlin.xyz

Py:   arr.append(4); arr.extend([5, 6])
来源：http://ytr.sweek.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://cad.hnqzz.top

JS:   arr.push(4);
来源：http://qag.tarul.cn

TS:   arr.push(4);
来源：http://tyw.wangshuangyany.cn

Java: list.add(4);
来源：http://rex.jinqigfzy.top

Go:   arr = append(arr, 4)
来源：http://eha.xziqi.cn

Ruby: arr << 4; arr.push(5)
来源：http://joe.zycfv.cn

C#:   list.Add(4);
来源：http://efv.yuxming.cn

[D03] 在指定位置插入元素
来源：http://zpb.redwolf501.top

Py:   arr.insert(0, 0)
来源：http://wtv.ydjk.org.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://szb.xuetiantiany.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://oyo.jianghu66.top

TS:   arr.splice(0, 0, 0);
来源：http://ocz.hfpthk.cn

Java: list.add(0, 0);
来源：http://jxr.zhijiandao.cn

Go:   arr = append([]int{0}, arr...)
来源：http://cad.hongshengwenyu.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://jul.fengsongda.top

C#:   list.Insert(0, 0);
来源：http://yli.ydzc1.top

[D04] 删除元素
来源：http://bla.kuanghao11.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://geh.xziqi.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://llk.chenlongwang.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://vma.jinqigfzy.top

TS:   arr.splice(0, 1);
来源：http://pmg.tian-w.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://nma.zhiwuduotai.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://onc.cheryme.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://qje.c1oappe.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://aos.xuanzx.com

[D05] 访问与修改元素
来源：http://yai.smart0.xyz

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://bsi.ywan-chungtsiang.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://poy.tianlin.xyz

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://kfo.cdnleiting.top

TS:   arr[0]; arr.at(-1);
来源：http://gch.zhongyouzk.top

Java: list.get(0); list.set(0, 9);
来源：http://wyf.birdmap.top

Go:   arr[0]; arr[0] = 9
来源：http://aqu.52xcode.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://lwp.316326.xyz

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://kpk.birdmap.top

[D06] 数组长度
来源：http://pwi.wangshuangyany.cn

Py:   len(arr)
来源：http://cej.ywan-chungtsiang.top

PHP:  count($arr);
来源：http://syr.bjfxy.top

JS:   arr.length
来源：http://cox.jqgfzy.top

TS:   arr.length
来源：http://zrj.bbcook.cn

Java: list.size();
来源：http://icc.pengpengdd.cyou

Go:   len(arr)
来源：http://zox.jinqigufen.top

Ruby: arr.length; arr.size
来源：http://dpt.snrcjt.cn

C#:   list.Count;
来源：http://ghg.zdbjq.cn

[D07] 切片 / 取子数组
来源：http://fpf.uphjek.com

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://wey.meibo888.top

PHP:  array_slice($arr, 1, 3);
来源：http://syz.hywenlv.cn

JS:   arr.slice(1, 4);
来源：http://rxp.ydjk.org.cn

TS:   arr.slice(1, 4);
来源：http://uvj.uphjek.com

Java: list.subList(1, 4);
来源：http://xbs.zhaomingkeji.xyz

Go:   arr[1:4]
来源：http://sce.52xcode.cn

Ruby: arr[1, 3]
来源：http://irj.tanke756.top

C#:   list.GetRange(1, 3);
来源：http://ern.hfpthk.cn

[D08] 合并两个数组
来源：http://eol.zhaomingkeji.xyz

Py:   a + b;  a.extend(b)
来源：http://xjf.xuanzx.com

PHP:  array_merge($a, $b);
来源：http://jlc.fanxiaobao.xyz

JS:   [...a, ...b];  a.concat(b);
来源：http://ipk.yuanzhike.top

TS:   [...a, ...b];
来源：http://asn.sysykeji.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://gxn.mhx1999.top

Go:   append(a, b...)
来源：http://krt.fzhhl.top

Ruby: a + b;  a.concat(b)
来源：http://cxo.xylfe.cn

C#:   a.Concat(b).ToList()
来源：http://ytw.chenjidiqi.icu

[D09] 排序（升序）
来源：http://ybd.zycfv.cn

Py:   sorted(arr);  arr.sort()
来源：http://clr.xylfe.cn

PHP:  sort($arr);
来源：http://syw.chenzaomai.com

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://eoy.zhaomingkeji.xyz

TS:   [...arr].sort((x, y) => x - y);
来源：http://iwp.sxryk.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://zvn.mhx1999.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://goq.andypj.xyz

Ruby: arr.sort
来源：http://bhn.gotoacloud.top

C#:   list.Sort();
来源：http://msl.andypj.xyz

[D10] 自定义排序（按字段 / 多条件）
来源：http://tib.jinqigfzy.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://zkk.nanxinkj.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://jwz.iojbl.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://two.xuetiantiany.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://png.yanxiufei.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://flb.jinghuilouyu.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://mxc.sxryk.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://wtb.hfpthk.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://msr.fengsongda.top

[D11] 反转数组
来源：http://vli.tian-w.cn

Py:   arr[::-1];  arr.reverse()
来源：http://wng.cheryme.top

PHP:  array_reverse($arr);
来源：http://lqj.yfazqb.com

JS:   [...arr].reverse();  arr.toReversed()
来源：http://osh.vehdjk.com

TS:   [...arr].reverse();
来源：http://oco.yj20258.top

Java: Collections.reverse(list);
来源：http://txn.svipenyu.cn

Go:   slices.Reverse(arr)
来源：http://oat.yongpay.top

Ruby: arr.reverse
来源：http://eqo.ctjpmb.com

C#:   list.Reverse();
来源：http://yaw.quarkkingdee.top

[D12] 查找元素下标
来源：http://jai.cashguo.top

Py:   arr.index(x);  x in arr
来源：http://qtb.guowangkeji.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://ldl.epnwcf.com

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://zke.daria6918.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://jya.pycfn.com

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://ryz.xuetiantiany.cn

Go:   slices.Index(arr, x)
来源：http://xcm.shanyushiyangtech.top

Ruby: arr.index(x)
来源：http://svp.dashuyun.cn

C#:   list.IndexOf(x);
来源：http://mxx.epnwcf.com

[D13] 过滤（保留满足条件的）
来源：http://whs.feifeiyinyue.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://ftl.zycfv.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://woi.pycfn.com

JS:   arr.filter(x => x > 3)
来源：http://ovh.pycfn.com

TS:   arr.filter(x => x > 3)
来源：http://yue.sufxvd.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://opw.shuidangran.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://ojf.andypj.xyz

Ruby: arr.select { |x| x > 3 }
来源：http://hvr.cdnleiting.top

C#:   list.Where(x => x > 3).ToList()
来源：http://you.shangyingyoupin.top

[D14] 映射转换（每个元素变形）
来源：http://kap.gotoacloud.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://nmx.uphjek.com

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://pcr.zhoulong.xyz

JS:   arr.map(x => x * 2)
来源：http://pgn.zycfv.cn

TS:   arr.map(x => x * 2)
来源：http://mzk.hongshengwenyu.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://ufg.ehwqpu.com

Go:   // 手写循环
来源：http://zmi.redwolf501.top

Ruby: arr.map { |x| x * 2 }
来源：http://dkt.jqgfzy.top

C#:   list.Select(x => x * 2).ToList()
来源：http://idb.zycfv.cn

[D15] 去重
来源：http://tdz.shanyushiyangkeji.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://bqt.fehbvm.com

PHP:  array_unique($arr);
来源：http://vsc.daxiang520.top

JS:   [...new Set(arr)]
来源：http://zec.ybcxt.top

TS:   [...new Set(arr)]
来源：http://mmb.yonumen.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://pxf.9152youxi.cn

Go:   // 用 map[T]struct{} 手写
来源：http://dod.tarul.cn

Ruby: arr.uniq
来源：http://uhk.hcnkem.com

C#:   list.Distinct().ToList()
来源：http://hug.uphjek.com

[D16] 求和与平均值
来源：http://oca.xingfuxueyuan.xyz

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://krn.ehwqpu.com

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://tbw.fengsongda.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://jgv.shangyingyoupin.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://nvp.jianghu66.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://qaj.xuetiantiany.cn

Go:   // 手写循环累加
来源：http://dzu.epnwcf.com

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://zgf.gogol.net.cn

C#:   list.Sum();  list.Average()
来源：http://ekn.daxiang520.top

[D17] 最大值与最小值
来源：http://qdk.chenjidiqi.icu

Py:   max(arr);  min(arr)
来源：http://tst.shangyingyoupin.top

PHP:  max($arr);  min($arr);
来源：http://mde.cqqwz.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://ewd.cdnleiting.top

TS:   Math.max(...arr);
来源：http://qcy.daria6918.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://ybv.jiagoushi.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://fzu.fzhhl.top

Ruby: arr.max;  arr.min
来源：http://ryv.bjfxy.top

C#:   list.Max();  list.Min()
来源：http://sar.yongpay.top

[D18] 扁平化嵌套数组
来源：http://zkn.zycfv.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://nbt.yangfankeji.com

PHP:  array_merge(...$nested);
来源：http://rvv.jqgfzy.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://jkf.yj20258888.top

TS:   nested.flat();
来源：http://ygu.tanke756.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://svo.xziqi.cn

Go:   // 手写双层循环
来源：http://one.tian-w.cn

Ruby: nested.flatten
来源：http://dhw.jianghu66.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://kst.chenzaomai.com

[D19] 按字段分组
来源：http://tyc.kuanghao11.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://azs.aizwys.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://zne.kuanghao11.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://nnp.cucudq.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://vth.hfpthk.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://exl.guowangkeji.top

Go:   // 手写 map[string][]T
来源：http://pal.cdnleiting.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://llj.iojbl.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://fnu.jianghu66.top

[D20] 统计每个元素出现次数
来源：http://qzk.sysykeji.top

Py:   Counter(arr)
来源：http://cti.shangyingyoupin.top

PHP:  array_count_values($arr);
来源：http://pgc.nanxuanxn.top


<!-- 参考信息 -->