代发 wailian999

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://xdz.cashguo.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://dfo.shuidangran.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://ulh.smart0.xyz

Java: // 无：用 Builder 模式或 record
来源：http://gtv.yueranfly.top

Go:   // 无：用配置结构体参数
来源：http://vnw.ydjk.org.cn

Ruby: f(a: 1, b: 2)
来源：http://pyp.andypj.xyz

C#:   f(a: 1, b: 2)
来源：http://lpp.fzhhl.top

[C05] 返回多个值
来源：http://ekc.vqdsnc.cn

Py:   return a, b
来源：http://kjv.yangfankeji.com

PHP:  return [$a, $b];
来源：http://fbd.nanxuanxn.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://vmi.hesvh.cn

TS:   return { a, b };
来源：http://xzr.dianchejie.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://qbe.sjlbkw.cn

Go:   return a, b
来源：http://bxl.yj202588.top

Ruby: return a, b
来源：http://qtu.yuanzhike.top

C#:   return (a, b);              // ValueTuple
来源：http://nzn.daria6918.cn

[C06] 匿名函数 / lambda
来源：http://ese.chenjidiqi.icu

Py:   square = lambda x: x * x
来源：http://gbq.yfazqb.com

PHP:  $square = fn($x) => $x * $x;
来源：http://wcf.shanyushiyangkeji.top

JS:   const square = x => x * x;
来源：http://mzj.sxryk.cn

TS:   const square = (x: number): number => x * x;
来源：http://sku.hnxiangtu.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://qtt.sjlbkw.cn

Go:   sq := func(x int) int { return x * x }
来源：http://iwf.bbcook.cn

Ruby: square = ->(x) { x * x }
来源：http://tfc.52xcode.cn

C#:   Func<int, int> square = x => x * x;
来源：http://qlt.quarkkingdee.top

[C07] 把函数作为参数传入
来源：http://itm.ehwqpu.com

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://gsw.daria6918.cn

PHP:  array_map("strtoupper", $arr);
来源：http://zvn.cheryme.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://lgw.shanyushiyangkeji.top

TS:   arr.map(String)
来源：http://smd.aibaodan.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://pmr.dashuyun.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://rcb.zhoulong.xyz

Ruby: arr.map(&:upcase)
来源：http://wit.cucudq.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://pak.chenlongwang.top

[C08] 闭包
来源：http://qvr.jinyuanbaomall.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://gta.c1oappe.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://ojc.yj20258.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://wpv.jqgfzy.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://xfh.jiagoushi.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://acs.tarul.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://nps.tianlin.xyz

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://ycl.chenjidiqi.icu

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://fox.epnwcf.com

[C09] 递归
来源：http://xpa.zhongyouzk.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://cki.zycfv.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://vtu.yvedp.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ena.havefunace.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ixu.nanxuanxn.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://ouq.cqqwz.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://ssb.zhengqikj.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://zvo.meibo888.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://kzn.svipenyu.cn

[C10] 变量作用域
来源：http://yln.yueranfly.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hwe.svipenyu.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://iam.yanxiufei.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://axj.redwolf501.top

TS:   同 JS
来源：http://tsm.pengpengdd.cyou

Java: 方法内为块级作用域
来源：http://jdh.nanxinkj.top

Go:   花括号块级作用域
来源：http://hkc.mhx1999.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://qhx.fengsongda.top

C#:   块级作用域
来源：http://gbi.nanxuanxn.top

[C11] 模块导入与导出
来源：http://akt.pycfn.com

Py:   from module import func
来源：http://ebq.yanxiufei.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://wqd.yuxming.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://bvg.jqgufenzy.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://cjm.sysykeji.top

Java: import java.util.List;
来源：http://mqq.epnwcf.com

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://nmq.9152youxi.cn

Ruby: require "json"; require_relative "./util"
来源：http://nnk.fzhhl.top

C#:   using System.Text;
来源：http://vis.sweek.top

[C12] 立即执行函数 IIFE
来源：http://bjm.c1oappe.top

Py:   (lambda: print("run"))()
来源：http://wij.feifeiyinyue.top

PHP:  (function () { echo "run"; })();
来源：http://qio.tanke756.top

JS:   (() => { console.log("run"); })();
来源：http://ffb.yangfankeji.com

TS:   (() => { console.log("run"); })();
来源：http://axq.cqqwz.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://dqy.aibaodan.cn

Go:   func() { fmt.Println("run") }()
来源：http://vqh.yonumen.top

Ruby: -> { puts "run" }.call
来源：http://zmo.vqdsnc.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://wrd.hcnkem.com

[C13] 类型声明 / 类型注解
来源：http://qke.chenzaomai.com

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://bjq.ctjpmb.com

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://rzm.ppjwa.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://sve.tanke756.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ckl.mhx1999.top

Java: int add(int a, int b) { return a + b; }
来源：http://fcj.yuanzhike.top

Go:   func add(a, b int) int
来源：http://mvu.yanxiufei.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://zvz.zhaomingkeji.xyz

C#:   int Add(int a, int b) => a + b;
来源：http://iaa.andypj.xyz

[C14] 泛型函数
来源：http://loq.ctjpmb.com

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://lok.jianghu66.top

PHP:  // 无泛型
来源：http://ejq.ctjpmb.com

JS:   // 无泛型
来源：http://svx.bjfxy.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hoa.jiagoushi.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://tat.yj20258888.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://pgh.gzhubu.top

Ruby: # 无泛型
来源：http://pfi.zhongyouzk.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://edp.gaohongyu789.top

[C15] 解构 / 展开参数
来源：http://hjt.cdnleiting.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://une.dianchejie.cn

PHP:  [$a, $b] = $pair;
来源：http://xsc.aizwys.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://uny.shzxlz.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://vhz.xingfuxueyuan.xyz

Java: // 无解构
来源：http://tkf.ydjk.org.cn

Go:   // 无解构
来源：http://qeg.snrcjt.cn

Ruby: a, b = pair
来源：http://dxi.shanyushiyangtech.top

C#:   var (a, b) = pair;
来源：http://fap.ybcxt.top

[C16] 函数 / 方法重载
来源：http://dxh.sweek.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://nfo.shangyingyoupin.top

PHP:  // 无重载
来源：http://arv.haohaochexian.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://jyx.smart0.xyz

TS:   // 用联合类型或重载签名声明
来源：http://dcz.gzhubu.top

Java: void f(int a) {}  void f(String a) {}
来源：http://fgf.hongshengwenyu.top

Go:   // 无重载：用不同函数名
来源：http://mil.jianghu66.top

Ruby: # 无重载：靠动态参数
来源：http://drw.jyoumei.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://ogs.sysykeji.top

================================================================================
来源：http://usw.hnqzz.top

D. 数组 / 列表 / 集合
来源：http://nmq.xuetiantiany.cn

================================================================================
来源：http://uru.ydjk.org.cn

[D01] 创建数组 / 列表
来源：http://pft.cucudq.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://und.tarul.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://tld.svipenyu.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://jqq.vqdsnc.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://ctf.guannengcc.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://dwa.c1oappe.top

Go:   arr := []int{1, 2, 3}
来源：http://xqw.jqgufenzy.top

Ruby: arr = [1, 2, 3]
来源：http://ioh.xuetiantiany.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://peh.jinghuilouyu.cn

[D02] 追加元素到末尾
来源：http://ity.yj20258888.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://esz.zhengqikj.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://kcz.bjfxy.top

JS:   arr.push(4);
来源：http://gpw.xziqi.cn

TS:   arr.push(4);
来源：http://sjy.xuanzx.com

Java: list.add(4);
来源：http://hao.wangdashe.top

Go:   arr = append(arr, 4)
来源：http://skd.9152youxi.cn

Ruby: arr << 4; arr.push(5)
来源：http://fga.pycfn.com

C#:   list.Add(4);
来源：http://bxc.shuidangran.top

[D03] 在指定位置插入元素
来源：http://pez.xuanzx.com

Py:   arr.insert(0, 0)
来源：http://oge.sjlbkw.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://vvk.tanke756.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://gks.hongshengwenyu.top

TS:   arr.splice(0, 0, 0);
来源：http://onx.sufxvd.cn

Java: list.add(0, 0);
来源：http://kfs.snrcjt.cn

Go:   arr = append([]int{0}, arr...)
来源：http://unk.jinqigufen.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hxr.kuanghao11.cn

C#:   list.Insert(0, 0);
来源：http://wwa.andypj.xyz

[D04] 删除元素
来源：http://ftc.zycfv.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://upb.tanke756.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://bbb.ctjpmb.com

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://kar.zhaomingkeji.xyz

TS:   arr.splice(0, 1);
来源：http://ugn.yfazqb.com

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://anr.nanxinkj.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://uxm.dashuyun.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://bpi.jlsjyb.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://xqc.yj20258.top

[D05] 访问与修改元素
来源：http://tut.vehdjk.com

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://dzr.yj202588.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://lrt.tarul.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://arr.vehdjk.com

TS:   arr[0]; arr.at(-1);
来源：http://bjo.chenzaomai.com

Java: list.get(0); list.set(0, 9);
来源：http://kfz.chenzaomai.com

Go:   arr[0]; arr[0] = 9
来源：http://jon.tarul.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://llg.yvedp.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://abq.cqqwz.cn

[D06] 数组长度
来源：http://bje.chenzaomai.com

Py:   len(arr)
来源：http://vtl.birdmap.top

PHP:  count($arr);
来源：http://gaz.zhengqikj.top

JS:   arr.length
来源：http://fvd.dianchejie.cn

TS:   arr.length
来源：http://shq.zdqjudy.top

Java: list.size();
来源：http://kvo.hammf.cn

Go:   len(arr)
来源：http://sml.gzhubu.top

Ruby: arr.length; arr.size
来源：http://pqk.mhx1999.top

C#:   list.Count;
来源：http://dgv.aizwys.cn

[D07] 切片 / 取子数组
来源：http://ntd.shanyushiyangtech.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://lzk.feifeiyinyue.top

PHP:  array_slice($arr, 1, 3);
来源：http://pjc.xziqi.cn

JS:   arr.slice(1, 4);
来源：http://tux.ydjk.org.cn

TS:   arr.slice(1, 4);
来源：http://jhw.ywan-chungtsiang.top

Java: list.subList(1, 4);
来源：http://cwd.dianchejie.cn

Go:   arr[1:4]
来源：http://abk.wangshuangyany.cn

Ruby: arr[1, 3]
来源：http://cuw.sweek.top

C#:   list.GetRange(1, 3);
来源：http://lmm.ydjk.org.cn

[D08] 合并两个数组
来源：http://gfe.fzhhl.top

Py:   a + b;  a.extend(b)
来源：http://jgx.aizwys.cn

PHP:  array_merge($a, $b);
来源：http://jnm.jyoumei.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://vuj.cqqwz.cn

TS:   [...a, ...b];
来源：http://mty.mhx1999.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://pnx.vqdsnc.cn

Go:   append(a, b...)
来源：http://fal.pycfn.com

Ruby: a + b;  a.concat(b)
来源：http://yon.nanxuanxn.top

C#:   a.Concat(b).ToList()
来源：http://uzw.zhaomingkeji.xyz

[D09] 排序（升序）
来源：http://ugp.cqqwz.cn

Py:   sorted(arr);  arr.sort()
来源：http://cil.yonumen.top

PHP:  sort($arr);
来源：http://ymy.bjfxy.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://xqo.snrcjt.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://sjj.xziqi.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://jci.wangdashe.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://vxe.vehdjk.com

Ruby: arr.sort
来源：http://feo.ydjk.org.cn

C#:   list.Sort();
来源：http://xpa.havefunace.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://ytm.dianchejie.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://khw.nanxinkj.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://cjj.dashuyun.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://nim.hongshengwenyu.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://gud.svipenyu.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://jqj.ydzc1.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hdh.yueranfly.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://kkm.cqqwz.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://ywy.9152youxi.cn

[D11] 反转数组
来源：http://gsi.smart0.xyz

Py:   arr[::-1];  arr.reverse()
来源：http://swj.ydjk.org.cn

PHP:  array_reverse($arr);
来源：http://pgt.sysykeji.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://gqk.ctjpmb.com

TS:   [...arr].reverse();
来源：http://yfp.ppjwa.cn

Java: Collections.reverse(list);
来源：http://zeb.yj20258888.top

Go:   slices.Reverse(arr)
来源：http://jpq.nwbrower.top

Ruby: arr.reverse
来源：http://hof.zycfv.cn

C#:   list.Reverse();
来源：http://ysv.fengsongda.top

[D12] 查找元素下标
来源：http://ovd.chenzaomai.com

Py:   arr.index(x);  x in arr
来源：http://srg.shanyushiyangkeji.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://vur.xuanzx.com

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://jgz.vehdjk.com

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ref.316326.xyz

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://pbk.fktsv.cn

Go:   slices.Index(arr, x)
来源：http://gvy.jqgufenzy.top

Ruby: arr.index(x)
来源：http://xwz.ehwqpu.com

C#:   list.IndexOf(x);
来源：http://daa.c1oappe.top

[D13] 过滤（保留满足条件的）
来源：http://wgn.jinghuilouyu.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://pix.hesvh.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://dpt.ybcxt.top

JS:   arr.filter(x => x > 3)
来源：http://npc.aizwys.cn

TS:   arr.filter(x => x > 3)
来源：http://tgr.jiagoushi.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://pnx.quarkkingdee.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://xsw.yuxming.cn

Ruby: arr.select { |x| x > 3 }
来源：http://bsf.jinqigfzy.top

C#:   list.Where(x => x > 3).ToList()
来源：http://mlj.zhoulong.xyz

[D14] 映射转换（每个元素变形）
来源：http://jfn.zhiwuduotai.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://mpq.hnqzz.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hmc.vqdsnc.cn

JS:   arr.map(x => x * 2)
来源：http://epb.aibaodan.cn

TS:   arr.map(x => x * 2)
来源：http://jwj.chenjidiqi.icu

Java: list.stream().map(x -> x * 2).toList()
来源：http://clt.shanyushiyangkeji.top

Go:   // 手写循环
来源：http://obc.iojbl.cn

Ruby: arr.map { |x| x * 2 }
来源：http://dnz.ppjwa.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://qyk.redwolf501.top

[D15] 去重
来源：http://xzk.shanyushiyangtech.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://ade.hongshengwenyu.top

PHP:  array_unique($arr);
来源：http://uxs.9152youxi.cn

JS:   [...new Set(arr)]
来源：http://shg.xuanzx.com

TS:   [...new Set(arr)]
来源：http://vyr.jqgfzy.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://wza.ehwqpu.com

Go:   // 用 map[T]struct{} 手写
来源：http://mjb.316326.xyz

Ruby: arr.uniq
来源：http://ngl.yj20258888.top

C#:   list.Distinct().ToList()
来源：http://tst.gotoacloud.top

[D16] 求和与平均值
来源：http://eml.sxryk.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://rzd.cqqwz.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://ryu.cheryme.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://sja.tian-w.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://cpk.smart0.xyz

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://dwd.ywan-chungtsiang.top

Go:   // 手写循环累加
来源：http://jtf.cheryme.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://lqq.epnwcf.com

C#:   list.Sum();  list.Average()
来源：http://xlq.redwolf501.top

[D17] 最大值与最小值
来源：http://fhn.vqdsnc.cn

Py:   max(arr);  min(arr)
来源：http://pef.yueranfly.top

PHP:  max($arr);  min($arr);
来源：http://akx.birdmap.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://fwh.aizwys.cn

TS:   Math.max(...arr);
来源：http://srg.guowangkeji.top

Java: Collections.max(list);  Collections.min(list);
来源：http://lqj.yonumen.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://nsl.yj20258.top

Ruby: arr.max;  arr.min
来源：http://nzq.ydjk.org.cn

C#:   list.Max();  list.Min()
来源：http://joe.zhengqikj.top

[D18] 扁平化嵌套数组
来源：http://meb.jinqigufen.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://mig.gotoacloud.top

PHP:  array_merge(...$nested);
来源：http://zew.316326.xyz

JS:   nested.flat();  nested.flat(Infinity)
来源：http://bvt.jinyuanbaomall.cn

TS:   nested.flat();
来源：http://tzt.cucudq.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://mzd.c1oappe.top

Go:   // 手写双层循环
来源：http://lxw.ybcxt.top

Ruby: nested.flatten
来源：http://oia.chenjidiqi.icu

C#:   nested.SelectMany(x => x).ToList()
来源：http://uxk.ctjpmb.com

[D19] 按字段分组
来源：http://dge.ehwqpu.com

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://myk.fehbvm.com

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://rkr.gogol.net.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://dia.epnwcf.com

TS:   Object.groupBy(arr, x => x.type)
来源：http://mhe.jlsjyb.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://iwk.shanyushiyangtech.top

Go:   // 手写 map[string][]T
来源：http://vtu.bjfxy.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://iys.feifeiyinyue.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://qoc.yuanzhike.top

[D20] 统计每个元素出现次数
来源：http://snv.jyoumei.cn

Py:   Counter(arr)
来源：http://usk.yonumen.top

PHP:  array_count_values($arr);
来源：http://njh.shanyushiyangtech.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://tbd.yonumen.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://onc.vqdsnc.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://kfl.andypj.xyz

Go:   // 手写 map[T]int
来源：http://ltu.hysaishi.cn

Ruby: arr.tally
来源：http://rbq.ctjpmb.com

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://fuj.smart0.xyz

[D21] 判断是否包含某元素
来源：http://scw.jinqigufen.top

Py:   x in arr
来源：http://hrx.cheryme.top


<!-- 参考信息 -->