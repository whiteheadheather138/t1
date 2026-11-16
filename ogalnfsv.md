代发 wailian999

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hmk.gaohongyu789.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hpz.fehbvm.com

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://ide.jinqigufen.top

Java: // 无：用 Builder 模式或 record
来源：http://qwa.fktsv.cn

Go:   // 无：用配置结构体参数
来源：http://itt.hnqzz.top

Ruby: f(a: 1, b: 2)
来源：http://mpw.hywenlv.cn

C#:   f(a: 1, b: 2)
来源：http://qzz.shuidangran.top

[C05] 返回多个值
来源：http://dkk.cucudq.cn

Py:   return a, b
来源：http://tjj.zhijiandao.cn

PHP:  return [$a, $b];
来源：http://prj.shzxlz.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://bag.yuxming.cn

TS:   return { a, b };
来源：http://gux.yuxming.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://gnc.pengpengdd.cyou

Go:   return a, b
来源：http://xro.tianlin.xyz

Ruby: return a, b
来源：http://yel.jiagoushi.top

C#:   return (a, b);              // ValueTuple
来源：http://gka.quarkkingdee.top

[C06] 匿名函数 / lambda
来源：http://anw.ybcxt.top

Py:   square = lambda x: x * x
来源：http://mzh.shanyushiyangkeji.top

PHP:  $square = fn($x) => $x * $x;
来源：http://vwj.andypj.xyz

JS:   const square = x => x * x;
来源：http://yvq.chenjidiqi.icu

TS:   const square = (x: number): number => x * x;
来源：http://juy.gaohongyu789.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://anl.hnxiangtu.top

Go:   sq := func(x int) int { return x * x }
来源：http://dji.zycfv.cn

Ruby: square = ->(x) { x * x }
来源：http://pyl.sweek.top

C#:   Func<int, int> square = x => x * x;
来源：http://eyd.hnqzz.top

[C07] 把函数作为参数传入
来源：http://pug.jqgufenzy.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://cdt.shangyingyoupin.top

PHP:  array_map("strtoupper", $arr);
来源：http://aij.svipenyu.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://mzn.xuetiantiany.cn

TS:   arr.map(String)
来源：http://sbb.chenlongwang.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://rte.smart0.xyz

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://snn.guannengcc.top

Ruby: arr.map(&:upcase)
来源：http://lot.ydzc1.top

C#:   arr.Select(s => s.ToUpper())
来源：http://cdz.zhongyouzk.top

[C08] 闭包
来源：http://xgi.chenzaomai.com

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://mur.jqgfzy.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://ann.vqdsnc.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://jxh.havefunace.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://afg.fzhhl.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://bdj.chenlongwang.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://ncn.zhixingplan.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://sae.jiagoushi.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://cij.mhx1999.top

[C09] 递归
来源：http://mpz.daxiang520.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://dfb.fanxiaobao.xyz

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://kzj.hesvh.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://btq.xinyue.icu

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://bvh.hfpthk.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://wwe.wangshuangyany.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://mwa.cheryme.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://trh.jinqigfzy.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://iui.aibaodan.cn

[C10] 变量作用域
来源：http://pnj.zhijiandao.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://zrj.9152youxi.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://kbr.jinqigfzy.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://zsf.zhoulong.xyz

TS:   同 JS
来源：http://hbd.zdqjudy.top

Java: 方法内为块级作用域
来源：http://nwb.uphjek.com

Go:   花括号块级作用域
来源：http://azs.birdmap.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://uny.yangfankeji.com

C#:   块级作用域
来源：http://voj.birdmap.top

[C11] 模块导入与导出
来源：http://uxn.aibaodan.cn

Py:   from module import func
来源：http://kwq.52xcode.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://nne.yuxming.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://bim.yongpay.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://amm.haohaochexian.top

Java: import java.util.List;
来源：http://edb.jyoumei.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://yhn.snrcjt.cn

Ruby: require "json"; require_relative "./util"
来源：http://etr.uphjek.com

C#:   using System.Text;
来源：http://mpq.yuxming.cn

[C12] 立即执行函数 IIFE
来源：http://xnc.ctjpmb.com

Py:   (lambda: print("run"))()
来源：http://jyv.fzhhl.top

PHP:  (function () { echo "run"; })();
来源：http://zuv.yanxiufei.cn

JS:   (() => { console.log("run"); })();
来源：http://xaq.cheryme.top

TS:   (() => { console.log("run"); })();
来源：http://pyk.c1oappe.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://vya.shanyushiyangkeji.top

Go:   func() { fmt.Println("run") }()
来源：http://wwr.jinyuanbaomall.cn

Ruby: -> { puts "run" }.call
来源：http://ptm.hnqzz.top

C#:   // 无 IIFE：用静态构造函数
来源：http://jqc.guannengcc.top

[C13] 类型声明 / 类型注解
来源：http://zgt.yj20258888.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://zve.jqgfzy.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://zzr.bbcook.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://lvf.zdqjudy.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://nuh.yj20258888.top

Java: int add(int a, int b) { return a + b; }
来源：http://wwn.zhiwuduotai.top

Go:   func add(a, b int) int
来源：http://jhh.yj20258888.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://dkh.daxiang520.top

C#:   int Add(int a, int b) => a + b;
来源：http://nxv.andypj.xyz

[C14] 泛型函数
来源：http://fnd.zycfv.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://ssa.sweek.top

PHP:  // 无泛型
来源：http://nwv.jqgufenzy.top

JS:   // 无泛型
来源：http://kox.zhoulong.xyz

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://uaf.dianchejie.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://jvp.jqgufenzy.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hub.mhx1999.top

Ruby: # 无泛型
来源：http://nkm.jinqigfzy.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://zkw.kuanghao11.cn

[C15] 解构 / 展开参数
来源：http://jmm.cashguo.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://mcv.xuetiantiany.cn

PHP:  [$a, $b] = $pair;
来源：http://xhi.yj20258.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://tjv.daria6918.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://lma.xylfe.cn

Java: // 无解构
来源：http://syx.shuidangran.top

Go:   // 无解构
来源：http://qav.jlsjyb.cn

Ruby: a, b = pair
来源：http://jkv.havefunace.top

C#:   var (a, b) = pair;
来源：http://esv.316326.xyz

[C16] 函数 / 方法重载
来源：http://ppf.hysaishi.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://iyd.uphjek.com

PHP:  // 无重载
来源：http://ezj.chenlongwang.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://grd.kuanghao11.cn

TS:   // 用联合类型或重载签名声明
来源：http://rib.zhoulong.xyz

Java: void f(int a) {}  void f(String a) {}
来源：http://dgb.fehbvm.com

Go:   // 无重载：用不同函数名
来源：http://nwz.nanxinkj.top

Ruby: # 无重载：靠动态参数
来源：http://uhu.tianlin.xyz

C#:   void F(int a) {}  void F(string a) {}
来源：http://hjb.tian-w.cn

================================================================================
来源：http://aaa.tian-w.cn

D. 数组 / 列表 / 集合
来源：http://igv.316326.xyz

================================================================================
来源：http://lpg.kuanghao11.cn

[D01] 创建数组 / 列表
来源：http://zcx.yuxming.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://jzw.bjfxy.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://cch.jlsjyb.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://crb.andypj.xyz

TS:   const arr: number[] = [1, 2, 3];
来源：http://krp.bjfxy.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://tvr.yuanzhike.top

Go:   arr := []int{1, 2, 3}
来源：http://abb.meibo888.top

Ruby: arr = [1, 2, 3]
来源：http://riz.wangshuangyany.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://wak.jinghuilouyu.cn

[D02] 追加元素到末尾
来源：http://agy.hnxiangtu.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://ncw.vehdjk.com

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://yyr.pengpengdd.cyou

JS:   arr.push(4);
来源：http://oxo.haohaochexian.top

TS:   arr.push(4);
来源：http://kzo.xylfe.cn

Java: list.add(4);
来源：http://yfi.fehbvm.com

Go:   arr = append(arr, 4)
来源：http://ewi.zhoulong.xyz

Ruby: arr << 4; arr.push(5)
来源：http://ufw.shangyingyoupin.top

C#:   list.Add(4);
来源：http://hdk.tanke756.top

[D03] 在指定位置插入元素
来源：http://mzc.xingfuxueyuan.xyz

Py:   arr.insert(0, 0)
来源：http://shc.sxryk.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hlm.sjlbkw.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://jus.uphjek.com

TS:   arr.splice(0, 0, 0);
来源：http://amn.hysaishi.cn

Java: list.add(0, 0);
来源：http://ggq.kuanghao11.cn

Go:   arr = append([]int{0}, arr...)
来源：http://idf.andypj.xyz

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://jpx.tianlin.xyz

C#:   list.Insert(0, 0);
来源：http://csk.yonumen.top

[D04] 删除元素
来源：http://umu.birdmap.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://wep.shanyushiyangkeji.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://lvk.sufxvd.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://atg.chenlongwang.top

TS:   arr.splice(0, 1);
来源：http://auf.meibo888.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://idc.cashguo.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://ews.aizwys.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://cvs.shangyingyoupin.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://zyq.ydzc1.top

[D05] 访问与修改元素
来源：http://rut.vqdsnc.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://dhy.tian-w.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://xpl.hcnkem.com

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://ktz.ctjpmb.com

TS:   arr[0]; arr.at(-1);
来源：http://atw.bbcook.cn

Java: list.get(0); list.set(0, 9);
来源：http://cnh.yangfankeji.com

Go:   arr[0]; arr[0] = 9
来源：http://aaj.zhixingplan.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://mur.yuxming.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://fzp.xuanzx.com

[D06] 数组长度
来源：http://nje.yuxming.cn

Py:   len(arr)
来源：http://zet.zhijiandao.cn

PHP:  count($arr);
来源：http://cvc.havefunace.top

JS:   arr.length
来源：http://fdz.kuanghao11.cn

TS:   arr.length
来源：http://fgb.meibo888.top

Java: list.size();
来源：http://dfl.hnqzz.top

Go:   len(arr)
来源：http://ohx.vehdjk.com

Ruby: arr.length; arr.size
来源：http://itz.yj202588.top

C#:   list.Count;
来源：http://lcg.zhoulong.xyz

[D07] 切片 / 取子数组
来源：http://xss.wangshuangyany.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://osv.smart0.xyz

PHP:  array_slice($arr, 1, 3);
来源：http://rai.hysaishi.cn

JS:   arr.slice(1, 4);
来源：http://gte.jyoumei.cn

TS:   arr.slice(1, 4);
来源：http://pqe.meibo888.top

Java: list.subList(1, 4);
来源：http://nap.nanxinkj.top

Go:   arr[1:4]
来源：http://ibn.sjlbkw.cn

Ruby: arr[1, 3]
来源：http://ygl.hnqzz.top

C#:   list.GetRange(1, 3);
来源：http://agp.bbcook.cn

[D08] 合并两个数组
来源：http://zig.feifeiyinyue.top

Py:   a + b;  a.extend(b)
来源：http://zca.yj20258888.top

PHP:  array_merge($a, $b);
来源：http://gnx.haohaochexian.top

JS:   [...a, ...b];  a.concat(b);
来源：http://ojd.gogol.net.cn

TS:   [...a, ...b];
来源：http://bln.ywan-chungtsiang.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hlt.sysykeji.top

Go:   append(a, b...)
来源：http://gaq.shangyingyoupin.top

Ruby: a + b;  a.concat(b)
来源：http://dyl.yuxming.cn

C#:   a.Concat(b).ToList()
来源：http://atx.sufxvd.cn

[D09] 排序（升序）
来源：http://cvt.vehdjk.com

Py:   sorted(arr);  arr.sort()
来源：http://tlt.xinyue.icu

PHP:  sort($arr);
来源：http://hiw.kuanghao11.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://lsg.quarkkingdee.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://pxz.zhoulong.xyz

Java: Collections.sort(list);  list.sort(null);
来源：http://sbt.bbcook.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://gxc.xylfe.cn

Ruby: arr.sort
来源：http://sam.52xcode.cn

C#:   list.Sort();
来源：http://psq.gogol.net.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://qvw.jyoumei.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://atv.yj20258.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://aqg.hnqzz.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://jew.shuidangran.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://ouy.ywan-chungtsiang.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://wfp.kuanghao11.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://lvn.gogol.net.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://ebe.c1oappe.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://wna.jinghuilouyu.cn

[D11] 反转数组
来源：http://pgr.xingfuxueyuan.xyz

Py:   arr[::-1];  arr.reverse()
来源：http://cjt.wangdashe.top

PHP:  array_reverse($arr);
来源：http://hlw.yvedp.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://lre.gzhubu.top

TS:   [...arr].reverse();
来源：http://ibi.ivvv.top

Java: Collections.reverse(list);
来源：http://zyf.jlsjyb.cn

Go:   slices.Reverse(arr)
来源：http://vdg.xuanzx.com

Ruby: arr.reverse
来源：http://vtd.guannengcc.top

C#:   list.Reverse();
来源：http://qpc.aibaodan.cn

[D12] 查找元素下标
来源：http://lgq.jlsjyb.cn

Py:   arr.index(x);  x in arr
来源：http://wkg.bjfxy.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://lel.fzhhl.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://tdw.zhoulong.xyz

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://nba.cucudq.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://iwk.daxiang520.top

Go:   slices.Index(arr, x)
来源：http://dtc.52xcode.cn

Ruby: arr.index(x)
来源：http://jwq.ywan-chungtsiang.top

C#:   list.IndexOf(x);
来源：http://jrx.jianghu66.top

[D13] 过滤（保留满足条件的）
来源：http://jlw.xinyue.icu

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://bgz.hcnkem.com

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://ymc.daxiang520.top

JS:   arr.filter(x => x > 3)
来源：http://bxv.sweek.top

TS:   arr.filter(x => x > 3)
来源：http://cxu.jinyuanbaomall.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://gzb.vqdsnc.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://iwo.chenjidiqi.icu

Ruby: arr.select { |x| x > 3 }
来源：http://ppv.gaohongyu789.top

C#:   list.Where(x => x > 3).ToList()
来源：http://ulw.mhx1999.top

[D14] 映射转换（每个元素变形）
来源：http://vwk.ppjwa.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://nzf.dianchejie.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://osx.aibaodan.cn

JS:   arr.map(x => x * 2)
来源：http://uwb.zdbjq.cn

TS:   arr.map(x => x * 2)
来源：http://jld.xuetiantiany.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://utw.tian-w.cn

Go:   // 手写循环
来源：http://xlh.aibaodan.cn

Ruby: arr.map { |x| x * 2 }
来源：http://btu.yuanzhike.top

C#:   list.Select(x => x * 2).ToList()
来源：http://exv.shanyushiyangkeji.top

[D15] 去重
来源：http://qhn.zhengqikj.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://wmh.fanxiaobao.xyz

PHP:  array_unique($arr);
来源：http://usl.c1oappe.top

JS:   [...new Set(arr)]
来源：http://fcv.xingfuxueyuan.xyz

TS:   [...new Set(arr)]
来源：http://ift.zdbjq.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://anv.vehdjk.com

Go:   // 用 map[T]struct{} 手写
来源：http://xtm.shanyushiyangkeji.top

Ruby: arr.uniq
来源：http://pbf.hongshengwenyu.top

C#:   list.Distinct().ToList()
来源：http://did.yj202588.top

[D16] 求和与平均值
来源：http://lvs.ybcxt.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://qyw.tanke756.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://pxh.cqqwz.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://lau.vehdjk.com

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://upq.jlsjyb.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://zmp.sxryk.cn

Go:   // 手写循环累加
来源：http://kre.yj20258.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://lgp.birdmap.top

C#:   list.Sum();  list.Average()
来源：http://icy.cucudq.cn

[D17] 最大值与最小值
来源：http://aze.jyoumei.cn

Py:   max(arr);  min(arr)
来源：http://rst.andypj.xyz

PHP:  max($arr);  min($arr);
来源：http://aye.snrcjt.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://ebv.yongpay.top

TS:   Math.max(...arr);
来源：http://idh.quarkkingdee.top

Java: Collections.max(list);  Collections.min(list);
来源：http://jkl.xingfuxueyuan.xyz

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://ypo.hfpthk.cn

Ruby: arr.max;  arr.min
来源：http://fyy.shanyushiyangtech.top

C#:   list.Max();  list.Min()
来源：http://llm.ppjwa.cn

[D18] 扁平化嵌套数组
来源：http://vig.fengsongda.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://job.zdbjq.cn

PHP:  array_merge(...$nested);
来源：http://bkj.ywan-chungtsiang.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://zlz.yj20258888.top

TS:   nested.flat();
来源：http://het.hcnkem.com

Java: nested.stream().flatMap(List::stream).toList()
来源：http://jjh.jqgufenzy.top

Go:   // 手写双层循环
来源：http://qoe.jqgufenzy.top

Ruby: nested.flatten
来源：http://dde.chenlongwang.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://upi.hfpthk.cn

[D19] 按字段分组
来源：http://xlu.fzhhl.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://aqc.tianlin.xyz

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://kqn.zhixingplan.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://trd.zhiwuduotai.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://hyn.hesvh.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://knu.tanke756.top

Go:   // 手写 map[string][]T
来源：http://aop.dianchejie.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://yhh.52xcode.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hwp.yueranfly.top

[D20] 统计每个元素出现次数
来源：http://zpx.daxiang520.top

Py:   Counter(arr)
来源：http://vmd.fktsv.cn

PHP:  array_count_values($arr);
来源：http://awv.zdqjudy.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://pbu.svipenyu.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://qki.sysykeji.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://qhb.ydjk.org.cn

Go:   // 手写 map[T]int
来源：http://qhx.aizwys.cn

Ruby: arr.tally
来源：http://sop.ehwqpu.com

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://nvt.9152youxi.cn

[D21] 判断是否包含某元素
来源：http://puq.yueranfly.top

Py:   x in arr
来源：http://zhy.cucudq.cn


<!-- 参考信息 -->