代发 wailian999

TS:   function greet(name: string = "World") { return name; }
来源：http://kva.dianchejie.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://del.shangyingyoupin.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://yst.dashuyun.cn

Ruby: def greet(name = "World") = name
来源：http://luy.jyoumei.cn

C#:   string Greet(string name = "World") => name;
来源：http://sxi.sjlbkw.cn

[C03] 可变参数
来源：http://gdx.jinqigfzy.top

Py:   def total(*args): return sum(args)
来源：http://avm.wangdashe.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hde.ctjpmb.com

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://bxy.ywan-chungtsiang.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://ieo.yuxming.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://lse.jyoumei.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://evo.sxryk.cn

Ruby: def total(*nums); nums.sum; end
来源：http://mxl.tianlin.xyz

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://cii.chenlongwang.top

[C04] 命名参数 / 关键字参数
来源：http://xow.ppjwa.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://qkc.epnwcf.com

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://uzc.pycfn.com

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://dlo.zhiwuduotai.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://bby.dashuyun.cn

Java: // 无：用 Builder 模式或 record
来源：http://lnc.havefunace.top

Go:   // 无：用配置结构体参数
来源：http://ogh.shanyushiyangkeji.top

Ruby: f(a: 1, b: 2)
来源：http://mfm.feifeiyinyue.top

C#:   f(a: 1, b: 2)
来源：http://bhu.guannengcc.top

[C05] 返回多个值
来源：http://dfq.0kj1m.cn

Py:   return a, b
来源：http://okw.uphjek.com

PHP:  return [$a, $b];
来源：http://naa.hcnkem.com

JS:   return [a, b];             // 或 return { a, b };
来源：http://fqi.pycfn.com

TS:   return { a, b };
来源：http://bmi.dashuyun.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://zct.fktsv.cn

Go:   return a, b
来源：http://szk.fanxiaobao.xyz

Ruby: return a, b
来源：http://qgo.nanxinkj.top

C#:   return (a, b);              // ValueTuple
来源：http://tom.daria6918.cn

[C06] 匿名函数 / lambda
来源：http://qkj.ybcxt.top

Py:   square = lambda x: x * x
来源：http://otc.bjfxy.top

PHP:  $square = fn($x) => $x * $x;
来源：http://hxz.wangshuangyany.cn

JS:   const square = x => x * x;
来源：http://faq.ehwqpu.com

TS:   const square = (x: number): number => x * x;
来源：http://xxi.ehwqpu.com

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://pbj.yonumen.top

Go:   sq := func(x int) int { return x * x }
来源：http://tzl.fktsv.cn

Ruby: square = ->(x) { x * x }
来源：http://vnj.nanxinkj.top

C#:   Func<int, int> square = x => x * x;
来源：http://lbp.xinyue.icu

[C07] 把函数作为参数传入
来源：http://sow.aibaodan.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://olp.xuetiantiany.cn

PHP:  array_map("strtoupper", $arr);
来源：http://rxr.jinghuilouyu.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://lia.hnqzz.top

TS:   arr.map(String)
来源：http://ngd.ctjpmb.com

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://dkp.uphjek.com

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://gtt.ctjpmb.com

Ruby: arr.map(&:upcase)
来源：http://xqj.zhixingplan.top

C#:   arr.Select(s => s.ToUpper())
来源：http://nne.yuxming.cn

[C08] 闭包
来源：http://bjf.yangfankeji.com

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://jma.cdnleiting.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://wxw.ywan-chungtsiang.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://kud.meibo888.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://qmg.quarkkingdee.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://zoc.yueranfly.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://rfg.zhijiandao.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://bbq.chenzaomai.com

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://cxc.yfazqb.com

[C09] 递归
来源：http://tiu.yuxming.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://ozz.xylfe.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://won.hcnkem.com

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://pbr.shzxlz.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ncr.gotoacloud.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://lzn.zhoulong.xyz

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://ydy.hcnkem.com

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://elr.zhoulong.xyz

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://dje.chenlongwang.top

[C10] 变量作用域
来源：http://skx.ybcxt.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://xeb.guannengcc.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://ryb.chenzaomai.com

JS:   let/const 块级作用域，var 函数级作用域
来源：http://psg.tanke756.top

TS:   同 JS
来源：http://rfu.wangdashe.top

Java: 方法内为块级作用域
来源：http://dks.zhixingplan.top

Go:   花括号块级作用域
来源：http://ggs.yj20258888.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://jso.quarkkingdee.top

C#:   块级作用域
来源：http://map.xuanzx.com

[C11] 模块导入与导出
来源：http://tbv.fktsv.cn

Py:   from module import func
来源：http://zdb.zhengqikj.top

PHP:  require "file.php";  或 use App\Service;
来源：http://yfu.cqqwz.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://rwa.ctjpmb.com

TS:   export function f(): void {};  import { f } from "./m";
来源：http://jsn.yvedp.cn

Java: import java.util.List;
来源：http://smi.vehdjk.com

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://ete.meibo888.top

Ruby: require "json"; require_relative "./util"
来源：http://eqb.yueranfly.top

C#:   using System.Text;
来源：http://ckp.yanxiufei.cn

[C12] 立即执行函数 IIFE
来源：http://xkj.zycfv.cn

Py:   (lambda: print("run"))()
来源：http://fcg.zycfv.cn

PHP:  (function () { echo "run"; })();
来源：http://txy.guannengcc.top

JS:   (() => { console.log("run"); })();
来源：http://ouw.hfpthk.cn

TS:   (() => { console.log("run"); })();
来源：http://yke.xuetiantiany.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://fbu.yonumen.top

Go:   func() { fmt.Println("run") }()
来源：http://jti.xziqi.cn

Ruby: -> { puts "run" }.call
来源：http://evs.yuxming.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://xfh.wangdashe.top

[C13] 类型声明 / 类型注解
来源：http://npx.daria6918.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://rod.xylfe.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://snm.hcnkem.com

JS:   // 无类型（可用 JSDoc 注释）
来源：http://qpj.yuanzhike.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ugf.fanxiaobao.xyz

Java: int add(int a, int b) { return a + b; }
来源：http://jjj.shanyushiyangtech.top

Go:   func add(a, b int) int
来源：http://qcw.shuidangran.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://imt.zhengqikj.top

C#:   int Add(int a, int b) => a + b;
来源：http://xfg.316326.xyz

[C14] 泛型函数
来源：http://wey.yueranfly.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://rpl.daxiang520.top

PHP:  // 无泛型
来源：http://rsj.tarul.cn

JS:   // 无泛型
来源：http://ezd.xinyue.icu

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://msw.c1oappe.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://swt.guannengcc.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://nwh.yuanzhike.top

Ruby: # 无泛型
来源：http://jfb.cucudq.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://uyp.redwolf501.top

[C15] 解构 / 展开参数
来源：http://byu.52xcode.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://jpo.sjlbkw.cn

PHP:  [$a, $b] = $pair;
来源：http://jft.meibo888.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://epc.cdnleiting.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://dqe.hfpthk.cn

Java: // 无解构
来源：http://xbb.smart0.xyz

Go:   // 无解构
来源：http://fgq.ehwqpu.com

Ruby: a, b = pair
来源：http://mfz.vehdjk.com

C#:   var (a, b) = pair;
来源：http://dcv.yanxiufei.cn

[C16] 函数 / 方法重载
来源：http://sim.hywenlv.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://qix.hnqzz.top

PHP:  // 无重载
来源：http://eza.shzxlz.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://bqj.yonumen.top

TS:   // 用联合类型或重载签名声明
来源：http://bnj.zhengqikj.top

Java: void f(int a) {}  void f(String a) {}
来源：http://ymr.zdbjq.cn

Go:   // 无重载：用不同函数名
来源：http://vfa.iojbl.cn

Ruby: # 无重载：靠动态参数
来源：http://vxr.fengsongda.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://eco.tianlin.xyz

================================================================================
来源：http://jal.shangyingyoupin.top

D. 数组 / 列表 / 集合
来源：http://csr.nwbrower.top

================================================================================
来源：http://yqk.wangdashe.top

[D01] 创建数组 / 列表
来源：http://dvp.zhengqikj.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://lff.vehdjk.com

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://xuj.xuetiantiany.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://qnm.sweek.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://tik.jinqigufen.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://oft.tanke756.top

Go:   arr := []int{1, 2, 3}
来源：http://tie.zdbjq.cn

Ruby: arr = [1, 2, 3]
来源：http://bnh.zhongyouzk.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://wzo.316326.xyz

[D02] 追加元素到末尾
来源：http://hgt.hongshengwenyu.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://mro.sjlbkw.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://okl.xziqi.cn

JS:   arr.push(4);
来源：http://ung.hnxiangtu.top

TS:   arr.push(4);
来源：http://cfp.ydjk.org.cn

Java: list.add(4);
来源：http://zaq.havefunace.top

Go:   arr = append(arr, 4)
来源：http://lpu.nanxinkj.top

Ruby: arr << 4; arr.push(5)
来源：http://ruf.feifeiyinyue.top

C#:   list.Add(4);
来源：http://aac.meibo888.top

[D03] 在指定位置插入元素
来源：http://egn.tarul.cn

Py:   arr.insert(0, 0)
来源：http://xex.smart0.xyz

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://qqc.shangyingyoupin.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://cgu.ydzc1.top

TS:   arr.splice(0, 0, 0);
来源：http://hsr.tianlin.xyz

Java: list.add(0, 0);
来源：http://bdb.gogol.net.cn

Go:   arr = append([]int{0}, arr...)
来源：http://fef.zhengqikj.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://ole.52xcode.cn

C#:   list.Insert(0, 0);
来源：http://xws.gzhubu.top

[D04] 删除元素
来源：http://lsk.zdbjq.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hhm.xziqi.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://kjl.xylfe.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://get.yongpay.top

TS:   arr.splice(0, 1);
来源：http://vxh.kuanghao11.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://vlx.xuanzx.com

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://cjt.yvedp.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://kfk.mhx1999.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://eoh.zhaomingkeji.xyz

[D05] 访问与修改元素
来源：http://bcb.hywenlv.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://ezv.yvedp.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://glk.pycfn.com

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://zud.tian-w.cn

TS:   arr[0]; arr.at(-1);
来源：http://udt.snrcjt.cn

Java: list.get(0); list.set(0, 9);
来源：http://dwl.dashuyun.cn

Go:   arr[0]; arr[0] = 9
来源：http://wqv.aibaodan.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://jnu.xingfuxueyuan.xyz

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://gku.chenjidiqi.icu

[D06] 数组长度
来源：http://umv.fzhhl.top

Py:   len(arr)
来源：http://zsn.yfazqb.com

PHP:  count($arr);
来源：http://cmf.iojbl.cn

JS:   arr.length
来源：http://ehy.wangshuangyany.cn

TS:   arr.length
来源：http://vgg.hesvh.cn

Java: list.size();
来源：http://zkm.sjlbkw.cn

Go:   len(arr)
来源：http://qca.andypj.xyz

Ruby: arr.length; arr.size
来源：http://dbw.shangyingyoupin.top

C#:   list.Count;
来源：http://gef.ybcxt.top

[D07] 切片 / 取子数组
来源：http://oso.sysykeji.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://fkk.shanyushiyangtech.top

PHP:  array_slice($arr, 1, 3);
来源：http://ntd.mhx1999.top

JS:   arr.slice(1, 4);
来源：http://wlq.zhiwuduotai.top

TS:   arr.slice(1, 4);
来源：http://lcp.sjlbkw.cn

Java: list.subList(1, 4);
来源：http://pxa.zhoulong.xyz

Go:   arr[1:4]
来源：http://tyt.yangfankeji.com

Ruby: arr[1, 3]
来源：http://joq.jiagoushi.top

C#:   list.GetRange(1, 3);
来源：http://jdg.nanxuanxn.top

[D08] 合并两个数组
来源：http://njw.zhongyouzk.top

Py:   a + b;  a.extend(b)
来源：http://ljg.cqqwz.cn

PHP:  array_merge($a, $b);
来源：http://hxw.xuanzx.com

JS:   [...a, ...b];  a.concat(b);
来源：http://ndv.ydjk.org.cn

TS:   [...a, ...b];
来源：http://zkv.yj20258888.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://agp.hesvh.cn

Go:   append(a, b...)
来源：http://tke.xuetiantiany.cn

Ruby: a + b;  a.concat(b)
来源：http://vbw.gogol.net.cn

C#:   a.Concat(b).ToList()
来源：http://xic.yj20258888.top

[D09] 排序（升序）
来源：http://jka.xuetiantiany.cn

Py:   sorted(arr);  arr.sort()
来源：http://rzu.zhiwuduotai.top

PHP:  sort($arr);
来源：http://orc.yangfankeji.com

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://jxi.shanyushiyangkeji.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://trr.smart0.xyz

Java: Collections.sort(list);  list.sort(null);
来源：http://cyc.yangfankeji.com

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://ipt.xinyue.icu

Ruby: arr.sort
来源：http://myd.yueranfly.top

C#:   list.Sort();
来源：http://rad.hcnkem.com

[D10] 自定义排序（按字段 / 多条件）
来源：http://amh.hywenlv.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://yxp.zhijiandao.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://saa.yuanzhike.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://zym.tarul.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://nhd.zhaomingkeji.xyz

Java: list.sort(Comparator.comparing(Person::age));
来源：http://evp.sjlbkw.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hpl.vqdsnc.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://pvf.cdnleiting.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://bzf.nanxinkj.top

[D11] 反转数组
来源：http://qic.snrcjt.cn

Py:   arr[::-1];  arr.reverse()
来源：http://lkk.yangfankeji.com

PHP:  array_reverse($arr);
来源：http://riy.yonumen.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://seq.jqgfzy.top

TS:   [...arr].reverse();
来源：http://rav.jianghu66.top

Java: Collections.reverse(list);
来源：http://djr.jinqigufen.top

Go:   slices.Reverse(arr)
来源：http://grr.chenjidiqi.icu

Ruby: arr.reverse
来源：http://eye.redwolf501.top

C#:   list.Reverse();
来源：http://rch.fktsv.cn

[D12] 查找元素下标
来源：http://kea.fanxiaobao.xyz

Py:   arr.index(x);  x in arr
来源：http://khd.yfazqb.com

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://gaf.haohaochexian.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://kea.c1oappe.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://yzq.redwolf501.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://wmw.zdqjudy.top

Go:   slices.Index(arr, x)
来源：http://kin.fehbvm.com

Ruby: arr.index(x)
来源：http://izv.xuanzx.com

C#:   list.IndexOf(x);
来源：http://dat.yj20258.top

[D13] 过滤（保留满足条件的）
来源：http://njd.hcnkem.com

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://zno.zhaomingkeji.xyz

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://pum.hongshengwenyu.top

JS:   arr.filter(x => x > 3)
来源：http://oat.vehdjk.com

TS:   arr.filter(x => x > 3)
来源：http://wij.xingfuxueyuan.xyz

Java: list.stream().filter(x -> x > 3).toList()
来源：http://cuy.gzhubu.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://yzx.gaohongyu789.top

Ruby: arr.select { |x| x > 3 }
来源：http://hyc.316326.xyz

C#:   list.Where(x => x > 3).ToList()
来源：http://rxs.jinyuanbaomall.cn

[D14] 映射转换（每个元素变形）
来源：http://zdw.zycfv.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hpv.hammf.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://wrc.redwolf501.top

JS:   arr.map(x => x * 2)
来源：http://orj.yuanzhike.top

TS:   arr.map(x => x * 2)
来源：http://hdi.cdnleiting.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://elc.gogol.net.cn

Go:   // 手写循环
来源：http://ydd.nwbrower.top

Ruby: arr.map { |x| x * 2 }
来源：http://kdf.snrcjt.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://pcw.chenlongwang.top

[D15] 去重
来源：http://exu.tanke756.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://bou.nanxinkj.top

PHP:  array_unique($arr);
来源：http://jof.zhengqikj.top

JS:   [...new Set(arr)]
来源：http://gzv.zycfv.cn

TS:   [...new Set(arr)]
来源：http://zgn.fanxiaobao.xyz

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://zkf.vehdjk.com

Go:   // 用 map[T]struct{} 手写
来源：http://cnq.sysykeji.top

Ruby: arr.uniq
来源：http://qax.yvedp.cn

C#:   list.Distinct().ToList()
来源：http://tak.gogol.net.cn

[D16] 求和与平均值
来源：http://rog.jinyuanbaomall.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://ltm.hnxiangtu.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://bgq.jinyuanbaomall.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hjq.daxiang520.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://xjy.haohaochexian.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://qiy.316326.xyz

Go:   // 手写循环累加
来源：http://rpl.cqqwz.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://yfe.wangshuangyany.cn

C#:   list.Sum();  list.Average()
来源：http://muw.havefunace.top

[D17] 最大值与最小值
来源：http://lzc.gaohongyu789.top

Py:   max(arr);  min(arr)
来源：http://lri.zhiwuduotai.top

PHP:  max($arr);  min($arr);
来源：http://lij.hnqzz.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://iyg.zhijiandao.cn

TS:   Math.max(...arr);
来源：http://tun.smart0.xyz

Java: Collections.max(list);  Collections.min(list);
来源：http://bjp.yfazqb.com

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://blv.gogol.net.cn

Ruby: arr.max;  arr.min
来源：http://hvh.tianlin.xyz

C#:   list.Max();  list.Min()
来源：http://uaq.hysaishi.cn

[D18] 扁平化嵌套数组
来源：http://has.nwbrower.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://jpf.sufxvd.cn

PHP:  array_merge(...$nested);
来源：http://zmx.ctjpmb.com

JS:   nested.flat();  nested.flat(Infinity)
来源：http://wno.wangshuangyany.cn

TS:   nested.flat();
来源：http://shm.gzhubu.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://bwm.sweek.top

Go:   // 手写双层循环
来源：http://liy.0kj1m.cn

Ruby: nested.flatten
来源：http://rzt.fktsv.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://zia.fehbvm.com

[D19] 按字段分组
来源：http://ncg.tianlin.xyz

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://wrx.vehdjk.com

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://phm.hammf.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://uzd.fanxiaobao.xyz


<!-- 参考信息 -->