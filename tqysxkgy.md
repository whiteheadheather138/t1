代发 wailian999

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://yqn.jiagoushi.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://snp.nanxinkj.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://shl.hnqzz.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://kvp.aibaodan.cn

Ruby: def total(*nums); nums.sum; end
来源：http://yva.fktsv.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://bxw.guannengcc.top

[C04] 命名参数 / 关键字参数
来源：http://vdz.daxiang520.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://nsk.cashguo.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://del.yvedp.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://onb.c1oappe.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://qel.zhixingplan.top

Java: // 无：用 Builder 模式或 record
来源：http://eim.nanxuanxn.top

Go:   // 无：用配置结构体参数
来源：http://cml.vehdjk.com

Ruby: f(a: 1, b: 2)
来源：http://kuy.hongshengwenyu.top

C#:   f(a: 1, b: 2)
来源：http://rmj.sweek.top

[C05] 返回多个值
来源：http://vgo.jinyuanbaomall.cn

Py:   return a, b
来源：http://vqk.gzhubu.top

PHP:  return [$a, $b];
来源：http://oll.ybcxt.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://skw.316326.xyz

TS:   return { a, b };
来源：http://zqr.yangfankeji.com

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://ryr.sweek.top

Go:   return a, b
来源：http://vuc.tian-w.cn

Ruby: return a, b
来源：http://kqu.tarul.cn

C#:   return (a, b);              // ValueTuple
来源：http://abt.zycfv.cn

[C06] 匿名函数 / lambda
来源：http://dgz.gaohongyu789.top

Py:   square = lambda x: x * x
来源：http://ffe.wangdashe.top

PHP:  $square = fn($x) => $x * $x;
来源：http://ovr.dashuyun.cn

JS:   const square = x => x * x;
来源：http://ida.hfpthk.cn

TS:   const square = (x: number): number => x * x;
来源：http://odz.nwbrower.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hvf.ydzc1.top

Go:   sq := func(x int) int { return x * x }
来源：http://xmu.sufxvd.cn

Ruby: square = ->(x) { x * x }
来源：http://lok.cqqwz.cn

C#:   Func<int, int> square = x => x * x;
来源：http://ile.yongpay.top

[C07] 把函数作为参数传入
来源：http://vbr.havefunace.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://kjk.tian-w.cn

PHP:  array_map("strtoupper", $arr);
来源：http://sqy.jlsjyb.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://xrr.vehdjk.com

TS:   arr.map(String)
来源：http://nsk.pycfn.com

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://rxf.yuxming.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://xxz.0kj1m.cn

Ruby: arr.map(&:upcase)
来源：http://ggm.gogol.net.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://lmh.yanxiufei.cn

[C08] 闭包
来源：http://bed.fzhhl.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://dbb.xuetiantiany.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://gbo.yvedp.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://gae.zdqjudy.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://syi.bjfxy.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://pde.zhixingplan.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://yvz.tianlin.xyz

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://nre.hcnkem.com

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://jwa.nanxinkj.top

[C09] 递归
来源：http://sag.tian-w.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://rav.sysykeji.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://sxx.wangdashe.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://lgi.feifeiyinyue.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mkg.quarkkingdee.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://iub.smart0.xyz

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://nym.ydjk.org.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://mfl.hammf.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://xxc.shanyushiyangkeji.top

[C10] 变量作用域
来源：http://alh.yanxiufei.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://gby.daria6918.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://ira.xuetiantiany.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://yrw.ybcxt.top

TS:   同 JS
来源：http://jud.wangshuangyany.cn

Java: 方法内为块级作用域
来源：http://las.shuidangran.top

Go:   花括号块级作用域
来源：http://pfk.dashuyun.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://xuv.redwolf501.top

C#:   块级作用域
来源：http://mgy.yueranfly.top

[C11] 模块导入与导出
来源：http://lsh.vqdsnc.cn

Py:   from module import func
来源：http://zfw.jinqigufen.top

PHP:  require "file.php";  或 use App\Service;
来源：http://jdv.cucudq.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://dyw.tarul.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://wdn.jiagoushi.top

Java: import java.util.List;
来源：http://keq.zhiwuduotai.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://xjx.zdbjq.cn

Ruby: require "json"; require_relative "./util"
来源：http://zhl.hongshengwenyu.top

C#:   using System.Text;
来源：http://gve.xylfe.cn

[C12] 立即执行函数 IIFE
来源：http://cja.xingfuxueyuan.xyz

Py:   (lambda: print("run"))()
来源：http://wxv.ppjwa.cn

PHP:  (function () { echo "run"; })();
来源：http://ktu.0kj1m.cn

JS:   (() => { console.log("run"); })();
来源：http://tnv.zdqjudy.top

TS:   (() => { console.log("run"); })();
来源：http://zob.shuidangran.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://dzw.yj20258888.top

Go:   func() { fmt.Println("run") }()
来源：http://mqa.gaohongyu789.top

Ruby: -> { puts "run" }.call
来源：http://tyi.xuanzx.com

C#:   // 无 IIFE：用静态构造函数
来源：http://nzw.9152youxi.cn

[C13] 类型声明 / 类型注解
来源：http://awo.jinqigfzy.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://qbl.fanxiaobao.xyz

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://gdx.zhaomingkeji.xyz

JS:   // 无类型（可用 JSDoc 注释）
来源：http://aac.yonumen.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://obq.pengpengdd.cyou

Java: int add(int a, int b) { return a + b; }
来源：http://gea.zhengqikj.top

Go:   func add(a, b int) int
来源：http://dmn.gzhubu.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://ggx.dianchejie.cn

C#:   int Add(int a, int b) => a + b;
来源：http://xie.9152youxi.cn

[C14] 泛型函数
来源：http://zmj.smart0.xyz

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://rpa.yj202588.top

PHP:  // 无泛型
来源：http://ymx.shangyingyoupin.top

JS:   // 无泛型
来源：http://jyl.yuanzhike.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://gza.xuanzx.com

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://abj.chenjidiqi.icu

Go:   func First[T any](items []T) T { return items[0] }
来源：http://ndw.yuanzhike.top

Ruby: # 无泛型
来源：http://kly.zhaomingkeji.xyz

C#:   static T First<T>(List<T> items) => items[0];
来源：http://jnu.ywan-chungtsiang.top

[C15] 解构 / 展开参数
来源：http://rhp.shangyingyoupin.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://ths.pycfn.com

PHP:  [$a, $b] = $pair;
来源：http://lnm.0kj1m.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hde.cucudq.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://bei.jiagoushi.top

Java: // 无解构
来源：http://lnq.xinyue.icu

Go:   // 无解构
来源：http://qqd.zdqjudy.top

Ruby: a, b = pair
来源：http://ocp.pycfn.com

C#:   var (a, b) = pair;
来源：http://afv.pengpengdd.cyou

[C16] 函数 / 方法重载
来源：http://drg.sjlbkw.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://ojr.ybcxt.top

PHP:  // 无重载
来源：http://ofh.snrcjt.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://knx.jqgufenzy.top

TS:   // 用联合类型或重载签名声明
来源：http://owx.xylfe.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://kma.fzhhl.top

Go:   // 无重载：用不同函数名
来源：http://xkq.meibo888.top

Ruby: # 无重载：靠动态参数
来源：http://mbk.tian-w.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://pcg.vqdsnc.cn

================================================================================
来源：http://eht.wangshuangyany.cn

D. 数组 / 列表 / 集合
来源：http://skh.chenjidiqi.icu

================================================================================
来源：http://ntf.daria6918.cn

[D01] 创建数组 / 列表
来源：http://jxx.dianchejie.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://czr.cheryme.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://aow.sufxvd.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://pew.yueranfly.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://niw.316326.xyz

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://nva.tianlin.xyz

Go:   arr := []int{1, 2, 3}
来源：http://uyl.yongpay.top

Ruby: arr = [1, 2, 3]
来源：http://pdg.gogol.net.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://nlp.hongshengwenyu.top

[D02] 追加元素到末尾
来源：http://fxk.yj20258888.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://ish.cqqwz.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://lpv.gzhubu.top

JS:   arr.push(4);
来源：http://rtu.yuanzhike.top

TS:   arr.push(4);
来源：http://tym.hesvh.cn

Java: list.add(4);
来源：http://yvk.sjlbkw.cn

Go:   arr = append(arr, 4)
来源：http://nyl.bjfxy.top

Ruby: arr << 4; arr.push(5)
来源：http://blc.jqgufenzy.top

C#:   list.Add(4);
来源：http://gcu.jianghu66.top

[D03] 在指定位置插入元素
来源：http://quf.chenzaomai.com

Py:   arr.insert(0, 0)
来源：http://wgl.nanxinkj.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://sdx.wangdashe.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://qbp.shzxlz.cn

TS:   arr.splice(0, 0, 0);
来源：http://xui.zhongyouzk.top

Java: list.add(0, 0);
来源：http://mua.zhoulong.xyz

Go:   arr = append([]int{0}, arr...)
来源：http://ovq.chenjidiqi.icu

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://vpv.jinghuilouyu.cn

C#:   list.Insert(0, 0);
来源：http://pjj.zhongyouzk.top

[D04] 删除元素
来源：http://nhr.tanke756.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://mic.cucudq.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://rjo.shzxlz.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://tqu.fktsv.cn

TS:   arr.splice(0, 1);
来源：http://bge.aibaodan.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://dxw.cucudq.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://bea.0kj1m.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://pzi.cashguo.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://idk.hesvh.cn

[D05] 访问与修改元素
来源：http://dgz.havefunace.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hya.havefunace.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://zvk.vehdjk.com

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://pta.birdmap.top

TS:   arr[0]; arr.at(-1);
来源：http://ugz.kuanghao11.cn

Java: list.get(0); list.set(0, 9);
来源：http://tpg.cqqwz.cn

Go:   arr[0]; arr[0] = 9
来源：http://oui.sxryk.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hdr.shangyingyoupin.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://lie.chenlongwang.top

[D06] 数组长度
来源：http://mjk.fengsongda.top

Py:   len(arr)
来源：http://buk.ehwqpu.com

PHP:  count($arr);
来源：http://fnj.shanyushiyangkeji.top

JS:   arr.length
来源：http://aiw.jiagoushi.top

TS:   arr.length
来源：http://xqp.meibo888.top

Java: list.size();
来源：http://jys.sxryk.cn

Go:   len(arr)
来源：http://leh.sweek.top

Ruby: arr.length; arr.size
来源：http://wtq.pycfn.com

C#:   list.Count;
来源：http://bcp.nwbrower.top

[D07] 切片 / 取子数组
来源：http://wzm.hfpthk.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://cvx.fktsv.cn

PHP:  array_slice($arr, 1, 3);
来源：http://osx.fzhhl.top

JS:   arr.slice(1, 4);
来源：http://ymj.jqgufenzy.top

TS:   arr.slice(1, 4);
来源：http://ecc.sweek.top

Java: list.subList(1, 4);
来源：http://rxk.zycfv.cn

Go:   arr[1:4]
来源：http://tvo.zhengqikj.top

Ruby: arr[1, 3]
来源：http://ytc.andypj.xyz

C#:   list.GetRange(1, 3);
来源：http://fhu.epnwcf.com

[D08] 合并两个数组
来源：http://kze.nwbrower.top

Py:   a + b;  a.extend(b)
来源：http://zmj.nwbrower.top

PHP:  array_merge($a, $b);
来源：http://gbx.yj20258.top

JS:   [...a, ...b];  a.concat(b);
来源：http://wjv.sxryk.cn

TS:   [...a, ...b];
来源：http://rhb.ydzc1.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://lcn.gaohongyu789.top

Go:   append(a, b...)
来源：http://pzw.shanyushiyangkeji.top

Ruby: a + b;  a.concat(b)
来源：http://qtb.nanxuanxn.top

C#:   a.Concat(b).ToList()
来源：http://dxd.haohaochexian.top

[D09] 排序（升序）
来源：http://axr.ppjwa.cn

Py:   sorted(arr);  arr.sort()
来源：http://ekw.hammf.cn

PHP:  sort($arr);
来源：http://dlf.tarul.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://sbj.zhoulong.xyz

TS:   [...arr].sort((x, y) => x - y);
来源：http://yyd.yj20258.top

Java: Collections.sort(list);  list.sort(null);
来源：http://msk.ydjk.org.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://yee.mhx1999.top

Ruby: arr.sort
来源：http://qca.ybcxt.top

C#:   list.Sort();
来源：http://yzx.ctjpmb.com

[D10] 自定义排序（按字段 / 多条件）
来源：http://yvp.cqqwz.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://xtz.aibaodan.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://pwn.zhengqikj.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://cys.ydzc1.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://cxo.xuetiantiany.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://qxs.mhx1999.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://ykj.ehwqpu.com

Ruby: arr.sort_by { |x| x[:age] }
来源：http://afl.daxiang520.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://usp.52xcode.cn

[D11] 反转数组
来源：http://rdy.andypj.xyz

Py:   arr[::-1];  arr.reverse()
来源：http://cpl.gogol.net.cn

PHP:  array_reverse($arr);
来源：http://rfg.jinyuanbaomall.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://nvk.yangfankeji.com

TS:   [...arr].reverse();
来源：http://gvo.wangshuangyany.cn

Java: Collections.reverse(list);
来源：http://tyw.dianchejie.cn

Go:   slices.Reverse(arr)
来源：http://lkc.jlsjyb.cn

Ruby: arr.reverse
来源：http://rll.yueranfly.top

C#:   list.Reverse();
来源：http://upq.zhiwuduotai.top

[D12] 查找元素下标
来源：http://djx.daria6918.cn

Py:   arr.index(x);  x in arr
来源：http://era.zdqjudy.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://rft.zhengqikj.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://voe.andypj.xyz

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://zes.jianghu66.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://ncq.kuanghao11.cn

Go:   slices.Index(arr, x)
来源：http://wpm.nanxuanxn.top

Ruby: arr.index(x)
来源：http://ygb.52xcode.cn

C#:   list.IndexOf(x);
来源：http://gbd.snrcjt.cn

[D13] 过滤（保留满足条件的）
来源：http://gic.xinyue.icu

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://mvu.mhx1999.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://eyu.sjlbkw.cn

JS:   arr.filter(x => x > 3)
来源：http://ihq.xinyue.icu

TS:   arr.filter(x => x > 3)
来源：http://mua.yj202588.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://bby.iojbl.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://rmd.wangshuangyany.cn

Ruby: arr.select { |x| x > 3 }
来源：http://gyc.jqgufenzy.top

C#:   list.Where(x => x > 3).ToList()
来源：http://imt.pengpengdd.cyou

[D14] 映射转换（每个元素变形）
来源：http://hmq.yvedp.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://nyx.tianlin.xyz

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://ucx.tanke756.top

JS:   arr.map(x => x * 2)
来源：http://uto.vqdsnc.cn

TS:   arr.map(x => x * 2)
来源：http://jsi.yj20258.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://ksp.zhongyouzk.top

Go:   // 手写循环
来源：http://vhf.yangfankeji.com

Ruby: arr.map { |x| x * 2 }
来源：http://txk.wangshuangyany.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://tfw.gogol.net.cn

[D15] 去重
来源：http://skg.sweek.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://oqv.redwolf501.top

PHP:  array_unique($arr);
来源：http://ftk.gzhubu.top

JS:   [...new Set(arr)]
来源：http://rjb.gogol.net.cn

TS:   [...new Set(arr)]
来源：http://csd.ppjwa.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://unw.shanyushiyangkeji.top

Go:   // 用 map[T]struct{} 手写
来源：http://suh.ivvv.top

Ruby: arr.uniq
来源：http://jro.0kj1m.cn

C#:   list.Distinct().ToList()
来源：http://kgl.jinghuilouyu.cn

[D16] 求和与平均值
来源：http://lkv.xinyue.icu

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://cmk.dashuyun.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://wyc.jlsjyb.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://nxq.ctjpmb.com

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://fbk.nanxuanxn.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://qbo.gzhubu.top

Go:   // 手写循环累加
来源：http://gav.hysaishi.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://umk.zhixingplan.top

C#:   list.Sum();  list.Average()
来源：http://rua.zhoulong.xyz

[D17] 最大值与最小值
来源：http://soz.shzxlz.cn

Py:   max(arr);  min(arr)
来源：http://usd.zhijiandao.cn

PHP:  max($arr);  min($arr);
来源：http://nwh.pycfn.com

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://iyu.tarul.cn

TS:   Math.max(...arr);
来源：http://ftm.feifeiyinyue.top

Java: Collections.max(list);  Collections.min(list);
来源：http://kxw.hammf.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://dlw.cashguo.top

Ruby: arr.max;  arr.min
来源：http://cuk.shzxlz.cn

C#:   list.Max();  list.Min()
来源：http://mdu.hammf.cn

[D18] 扁平化嵌套数组
来源：http://neo.fehbvm.com

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://xol.ydjk.org.cn

PHP:  array_merge(...$nested);
来源：http://ltg.dianchejie.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://zac.ppjwa.cn

TS:   nested.flat();
来源：http://mdv.tarul.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://asy.sjlbkw.cn

Go:   // 手写双层循环
来源：http://vhy.hesvh.cn

Ruby: nested.flatten
来源：http://qwn.316326.xyz

C#:   nested.SelectMany(x => x).ToList()
来源：http://ago.jianghu66.top

[D19] 按字段分组
来源：http://pnd.xingfuxueyuan.xyz

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://vmx.yj202588.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://fir.jiagoushi.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://sel.uphjek.com

TS:   Object.groupBy(arr, x => x.type)
来源：http://ihp.shanyushiyangtech.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://ofu.meibo888.top

Go:   // 手写 map[string][]T
来源：http://vpx.cqqwz.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://vpc.nanxuanxn.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://kgb.hysaishi.cn

[D20] 统计每个元素出现次数
来源：http://oqd.mhx1999.top

Py:   Counter(arr)
来源：http://zea.yvedp.cn

PHP:  array_count_values($arr);
来源：http://ezf.yj20258.top


<!-- 参考信息 -->