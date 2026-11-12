代发 wailian999

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://enj.jinqigufen.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://evf.fktsv.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://sgx.zhongyouzk.top

Java: // 无：用 Builder 模式或 record
来源：http://llc.zhongyouzk.top

Go:   // 无：用配置结构体参数
来源：http://ltz.nwbrower.top

Ruby: f(a: 1, b: 2)
来源：http://srm.zhaomingkeji.xyz

C#:   f(a: 1, b: 2)
来源：http://hfi.zhengqikj.top

[C05] 返回多个值
来源：http://gge.316326.xyz

Py:   return a, b
来源：http://ndv.gogol.net.cn

PHP:  return [$a, $b];
来源：http://rdi.jiagoushi.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://drp.tian-w.cn

TS:   return { a, b };
来源：http://qko.hesvh.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://axz.sxryk.cn

Go:   return a, b
来源：http://lhi.gogol.net.cn

Ruby: return a, b
来源：http://qgu.yangfankeji.com

C#:   return (a, b);              // ValueTuple
来源：http://kah.jinyuanbaomall.cn

[C06] 匿名函数 / lambda
来源：http://cvm.ehwqpu.com

Py:   square = lambda x: x * x
来源：http://hhr.zhoulong.xyz

PHP:  $square = fn($x) => $x * $x;
来源：http://snf.yfazqb.com

JS:   const square = x => x * x;
来源：http://duw.sufxvd.cn

TS:   const square = (x: number): number => x * x;
来源：http://gip.andypj.xyz

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://par.hesvh.cn

Go:   sq := func(x int) int { return x * x }
来源：http://hab.xylfe.cn

Ruby: square = ->(x) { x * x }
来源：http://vdz.vqdsnc.cn

C#:   Func<int, int> square = x => x * x;
来源：http://ljl.svipenyu.cn

[C07] 把函数作为参数传入
来源：http://iwx.zycfv.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://wdx.havefunace.top

PHP:  array_map("strtoupper", $arr);
来源：http://bla.iojbl.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://tfk.pycfn.com

TS:   arr.map(String)
来源：http://lbh.yfazqb.com

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://cca.zhiwuduotai.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://ryd.mhx1999.top

Ruby: arr.map(&:upcase)
来源：http://ror.zycfv.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://lun.shanyushiyangtech.top

[C08] 闭包
来源：http://sdg.zdbjq.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://dvz.xylfe.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://kvv.redwolf501.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://gdz.ehwqpu.com

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://tcl.hnxiangtu.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://geo.daria6918.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://csk.zycfv.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://vff.yvedp.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://oel.cqqwz.cn

[C09] 递归
来源：http://atl.cqqwz.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://boi.bjfxy.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://ywk.zhiwuduotai.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://der.hnxiangtu.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://gmh.hcnkem.com

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://bjd.fengsongda.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://kgg.gaohongyu789.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://rsv.bbcook.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://jck.yongpay.top

[C10] 变量作用域
来源：http://ynt.shangyingyoupin.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://dzo.daxiang520.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://jnz.tianlin.xyz

JS:   let/const 块级作用域，var 函数级作用域
来源：http://rfi.yangfankeji.com

TS:   同 JS
来源：http://mui.zdbjq.cn

Java: 方法内为块级作用域
来源：http://usu.chenlongwang.top

Go:   花括号块级作用域
来源：http://aso.xingfuxueyuan.xyz

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://vha.sufxvd.cn

C#:   块级作用域
来源：http://lsn.xingfuxueyuan.xyz

[C11] 模块导入与导出
来源：http://vuz.daxiang520.top

Py:   from module import func
来源：http://jtc.daxiang520.top

PHP:  require "file.php";  或 use App\Service;
来源：http://ltg.jqgfzy.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://jol.nanxinkj.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://ygr.hfpthk.cn

Java: import java.util.List;
来源：http://yjd.yanxiufei.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://isd.ydzc1.top

Ruby: require "json"; require_relative "./util"
来源：http://arj.svipenyu.cn

C#:   using System.Text;
来源：http://wwh.52xcode.cn

[C12] 立即执行函数 IIFE
来源：http://dws.ivvv.top

Py:   (lambda: print("run"))()
来源：http://nlz.ybcxt.top

PHP:  (function () { echo "run"; })();
来源：http://vkw.xylfe.cn

JS:   (() => { console.log("run"); })();
来源：http://ora.chenjidiqi.icu

TS:   (() => { console.log("run"); })();
来源：http://ayv.kuanghao11.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://cpm.hfpthk.cn

Go:   func() { fmt.Println("run") }()
来源：http://wby.nanxuanxn.top

Ruby: -> { puts "run" }.call
来源：http://rpx.shuidangran.top

C#:   // 无 IIFE：用静态构造函数
来源：http://ltl.cashguo.top

[C13] 类型声明 / 类型注解
来源：http://gya.feifeiyinyue.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://yje.gzhubu.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://jpl.gotoacloud.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://xut.shanyushiyangtech.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://zwi.haohaochexian.top

Java: int add(int a, int b) { return a + b; }
来源：http://ayn.wangshuangyany.cn

Go:   func add(a, b int) int
来源：http://pqo.uphjek.com

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://yvn.shzxlz.cn

C#:   int Add(int a, int b) => a + b;
来源：http://zur.hnxiangtu.top

[C14] 泛型函数
来源：http://uye.yfazqb.com

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://rlj.xuanzx.com

PHP:  // 无泛型
来源：http://grx.gzhubu.top

JS:   // 无泛型
来源：http://gmu.zhaomingkeji.xyz

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://mhj.zhiwuduotai.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://yay.wangdashe.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://zho.zycfv.cn

Ruby: # 无泛型
来源：http://gey.guowangkeji.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://zxp.tian-w.cn

[C15] 解构 / 展开参数
来源：http://icd.jinyuanbaomall.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://xlh.zhixingplan.top

PHP:  [$a, $b] = $pair;
来源：http://xhx.daxiang520.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://zdb.cqqwz.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://lbt.guannengcc.top

Java: // 无解构
来源：http://sez.xziqi.cn

Go:   // 无解构
来源：http://upz.cqqwz.cn

Ruby: a, b = pair
来源：http://ckg.iojbl.cn

C#:   var (a, b) = pair;
来源：http://rgh.zdbjq.cn

[C16] 函数 / 方法重载
来源：http://goq.daria6918.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://ilb.chenlongwang.top

PHP:  // 无重载
来源：http://cpt.ydjk.org.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://kcs.jinqigufen.top

TS:   // 用联合类型或重载签名声明
来源：http://nze.hammf.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://rhg.sysykeji.top

Go:   // 无重载：用不同函数名
来源：http://aju.wangshuangyany.cn

Ruby: # 无重载：靠动态参数
来源：http://msb.xuanzx.com

C#:   void F(int a) {}  void F(string a) {}
来源：http://wuq.c1oappe.top

================================================================================
来源：http://pjk.zhongyouzk.top

D. 数组 / 列表 / 集合
来源：http://zfi.gaohongyu789.top

================================================================================
来源：http://pmx.aizwys.cn

[D01] 创建数组 / 列表
来源：http://ltf.havefunace.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://urb.havefunace.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://oiv.jinghuilouyu.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://dfo.mhx1999.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://bjv.ehwqpu.com

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hzt.birdmap.top

Go:   arr := []int{1, 2, 3}
来源：http://fkd.shangyingyoupin.top

Ruby: arr = [1, 2, 3]
来源：http://wan.jianghu66.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://znu.shanyushiyangkeji.top

[D02] 追加元素到末尾
来源：http://yzj.jinyuanbaomall.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://wbh.fanxiaobao.xyz

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://agi.nwbrower.top

JS:   arr.push(4);
来源：http://swi.c1oappe.top

TS:   arr.push(4);
来源：http://bvd.fengsongda.top

Java: list.add(4);
来源：http://ert.fengsongda.top

Go:   arr = append(arr, 4)
来源：http://bfj.redwolf501.top

Ruby: arr << 4; arr.push(5)
来源：http://ddy.hesvh.cn

C#:   list.Add(4);
来源：http://kqg.redwolf501.top

[D03] 在指定位置插入元素
来源：http://mnn.ctjpmb.com

Py:   arr.insert(0, 0)
来源：http://tln.zycfv.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://cty.yj202588.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://deg.quarkkingdee.top

TS:   arr.splice(0, 0, 0);
来源：http://pau.pycfn.com

Java: list.add(0, 0);
来源：http://vsk.zhiwuduotai.top

Go:   arr = append([]int{0}, arr...)
来源：http://qio.sxryk.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://qlg.aizwys.cn

C#:   list.Insert(0, 0);
来源：http://cww.yfazqb.com

[D04] 删除元素
来源：http://bsd.jqgfzy.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://kac.wangshuangyany.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://gjm.gaohongyu789.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://ntt.cashguo.top

TS:   arr.splice(0, 1);
来源：http://jvk.mhx1999.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://cmx.xingfuxueyuan.xyz

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://ntz.gotoacloud.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://lzk.smart0.xyz

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://jdj.ybcxt.top

[D05] 访问与修改元素
来源：http://rro.0kj1m.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://xpj.gotoacloud.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://rjt.daria6918.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://ane.yuanzhike.top

TS:   arr[0]; arr.at(-1);
来源：http://udb.zhengqikj.top

Java: list.get(0); list.set(0, 9);
来源：http://ypw.zdbjq.cn

Go:   arr[0]; arr[0] = 9
来源：http://bap.snrcjt.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://pyz.yuanzhike.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://zre.bbcook.cn

[D06] 数组长度
来源：http://gtd.shzxlz.cn

Py:   len(arr)
来源：http://ada.aibaodan.cn

PHP:  count($arr);
来源：http://hwy.hammf.cn

JS:   arr.length
来源：http://mlu.9152youxi.cn

TS:   arr.length
来源：http://fzz.wangshuangyany.cn

Java: list.size();
来源：http://uqm.cheryme.top

Go:   len(arr)
来源：http://dam.hfpthk.cn

Ruby: arr.length; arr.size
来源：http://gtm.iojbl.cn

C#:   list.Count;
来源：http://kym.shzxlz.cn

[D07] 切片 / 取子数组
来源：http://rxp.jianghu66.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://xkt.hongshengwenyu.top

PHP:  array_slice($arr, 1, 3);
来源：http://dop.jinyuanbaomall.cn

JS:   arr.slice(1, 4);
来源：http://axj.yfazqb.com

TS:   arr.slice(1, 4);
来源：http://qty.c1oappe.top

Java: list.subList(1, 4);
来源：http://cdc.cdnleiting.top

Go:   arr[1:4]
来源：http://dnx.haohaochexian.top

Ruby: arr[1, 3]
来源：http://grd.shanyushiyangkeji.top

C#:   list.GetRange(1, 3);
来源：http://bte.snrcjt.cn

[D08] 合并两个数组
来源：http://yje.hysaishi.cn

Py:   a + b;  a.extend(b)
来源：http://spy.52xcode.cn

PHP:  array_merge($a, $b);
来源：http://umj.chenjidiqi.icu

JS:   [...a, ...b];  a.concat(b);
来源：http://srv.ywan-chungtsiang.top

TS:   [...a, ...b];
来源：http://cau.yanxiufei.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://dhn.sweek.top

Go:   append(a, b...)
来源：http://ode.gogol.net.cn

Ruby: a + b;  a.concat(b)
来源：http://ufa.guowangkeji.top

C#:   a.Concat(b).ToList()
来源：http://qsh.shuidangran.top

[D09] 排序（升序）
来源：http://hcd.cucudq.cn

Py:   sorted(arr);  arr.sort()
来源：http://tyv.hnqzz.top

PHP:  sort($arr);
来源：http://ypr.bjfxy.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://ajf.shzxlz.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://hcy.nanxuanxn.top

Java: Collections.sort(list);  list.sort(null);
来源：http://ntf.zhongyouzk.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://wqz.yfazqb.com

Ruby: arr.sort
来源：http://pxe.cdnleiting.top

C#:   list.Sort();
来源：http://krk.daxiang520.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://rqf.hcnkem.com

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://rtb.sjlbkw.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ypm.cqqwz.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://ppm.vqdsnc.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://gqs.jqgufenzy.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://qku.zdqjudy.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://awe.gotoacloud.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://wtu.jinqigfzy.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://fbw.hysaishi.cn

[D11] 反转数组
来源：http://vpt.cqqwz.cn

Py:   arr[::-1];  arr.reverse()
来源：http://qfo.yueranfly.top

PHP:  array_reverse($arr);
来源：http://lne.guannengcc.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hqn.feifeiyinyue.top

TS:   [...arr].reverse();
来源：http://elx.hnqzz.top

Java: Collections.reverse(list);
来源：http://wdf.yueranfly.top

Go:   slices.Reverse(arr)
来源：http://atu.fzhhl.top

Ruby: arr.reverse
来源：http://jix.meibo888.top

C#:   list.Reverse();
来源：http://vbs.bjfxy.top

[D12] 查找元素下标
来源：http://hpj.xinyue.icu

Py:   arr.index(x);  x in arr
来源：http://kom.xingfuxueyuan.xyz

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://xsl.jqgfzy.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://yfj.yj202588.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://cfe.cqqwz.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://kzh.xuanzx.com

Go:   slices.Index(arr, x)
来源：http://unl.chenjidiqi.icu

Ruby: arr.index(x)
来源：http://ohm.uphjek.com

C#:   list.IndexOf(x);
来源：http://vsi.yuxming.cn

[D13] 过滤（保留满足条件的）
来源：http://ebl.jqgufenzy.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://qzp.yuanzhike.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://dqr.hfpthk.cn

JS:   arr.filter(x => x > 3)
来源：http://lmh.zhongyouzk.top

TS:   arr.filter(x => x > 3)
来源：http://kun.cdnleiting.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://nnq.fehbvm.com

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://kjt.zdqjudy.top

Ruby: arr.select { |x| x > 3 }
来源：http://uap.ydzc1.top

C#:   list.Where(x => x > 3).ToList()
来源：http://krk.ctjpmb.com

[D14] 映射转换（每个元素变形）
来源：http://bpz.daria6918.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://bvt.tianlin.xyz

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://vrq.bjfxy.top

JS:   arr.map(x => x * 2)
来源：http://nmz.yanxiufei.cn

TS:   arr.map(x => x * 2)
来源：http://esn.hongshengwenyu.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://cqt.hnxiangtu.top

Go:   // 手写循环
来源：http://sbi.gotoacloud.top

Ruby: arr.map { |x| x * 2 }
来源：http://emu.hammf.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://eou.sweek.top

[D15] 去重
来源：http://qta.kuanghao11.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://eei.vqdsnc.cn

PHP:  array_unique($arr);
来源：http://xkb.yuxming.cn

JS:   [...new Set(arr)]
来源：http://zbh.yongpay.top

TS:   [...new Set(arr)]
来源：http://fne.shanyushiyangtech.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://mfr.uphjek.com

Go:   // 用 map[T]struct{} 手写
来源：http://xxs.yj20258.top

Ruby: arr.uniq
来源：http://wdl.wangdashe.top

C#:   list.Distinct().ToList()
来源：http://das.shangyingyoupin.top

[D16] 求和与平均值
来源：http://aly.fengsongda.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://gcp.bbcook.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://eol.zdbjq.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://eky.ydzc1.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://nhr.shanyushiyangtech.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://cwk.hywenlv.cn

Go:   // 手写循环累加
来源：http://nmp.yj20258.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://rpk.sufxvd.cn

C#:   list.Sum();  list.Average()
来源：http://afw.zhixingplan.top

[D17] 最大值与最小值
来源：http://yjz.fengsongda.top

Py:   max(arr);  min(arr)
来源：http://vrj.wangshuangyany.cn

PHP:  max($arr);  min($arr);
来源：http://ywp.fktsv.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://tkm.gaohongyu789.top

TS:   Math.max(...arr);
来源：http://ilo.zdbjq.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://zsd.cdnleiting.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://gky.gogol.net.cn

Ruby: arr.max;  arr.min
来源：http://hwa.jqgufenzy.top

C#:   list.Max();  list.Min()
来源：http://xlk.jlsjyb.cn

[D18] 扁平化嵌套数组
来源：http://gho.jinqigufen.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://dve.hcnkem.com

PHP:  array_merge(...$nested);
来源：http://zkf.aibaodan.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hod.tarul.cn

TS:   nested.flat();
来源：http://rxn.hesvh.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://mbr.jqgfzy.top

Go:   // 手写双层循环
来源：http://taz.hnqzz.top

Ruby: nested.flatten
来源：http://sjv.wangshuangyany.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://bta.shzxlz.cn

[D19] 按字段分组
来源：http://fvf.daria6918.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://vbw.zhaomingkeji.xyz

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://mnq.c1oappe.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hbr.fengsongda.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://sjk.hammf.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://cwg.yangfankeji.com

Go:   // 手写 map[string][]T
来源：http://auv.guowangkeji.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://jbi.gotoacloud.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://fko.yuanzhike.top

[D20] 统计每个元素出现次数
来源：http://hpu.shangyingyoupin.top

Py:   Counter(arr)
来源：http://sxf.cheryme.top

PHP:  array_count_values($arr);
来源：http://wmq.meibo888.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ozo.zycfv.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://dqk.guowangkeji.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://iiy.gotoacloud.top

Go:   // 手写 map[T]int
来源：http://qpy.jyoumei.cn

Ruby: arr.tally
来源：http://piu.hongshengwenyu.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://nss.havefunace.top

[D21] 判断是否包含某元素
来源：http://fyq.c1oappe.top

Py:   x in arr
来源：http://mxa.zhiwuduotai.top


<!-- 参考信息 -->