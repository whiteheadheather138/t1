代发 wailian999

Py:   return a, b
来源：http://qxn.316326.xyz

PHP:  return [$a, $b];
来源：http://wrx.jlsjyb.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://dlm.hfpthk.cn

TS:   return { a, b };
来源：http://wbr.zycfv.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://vqk.yuanzhike.top

Go:   return a, b
来源：http://aku.vehdjk.com

Ruby: return a, b
来源：http://vsv.snrcjt.cn

C#:   return (a, b);              // ValueTuple
来源：http://wni.fehbvm.com

[C06] 匿名函数 / lambda
来源：http://pge.shzxlz.cn

Py:   square = lambda x: x * x
来源：http://fxr.pycfn.com

PHP:  $square = fn($x) => $x * $x;
来源：http://tqd.hnqzz.top

JS:   const square = x => x * x;
来源：http://qqj.meibo888.top

TS:   const square = (x: number): number => x * x;
来源：http://yla.sufxvd.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://cai.birdmap.top

Go:   sq := func(x int) int { return x * x }
来源：http://ckj.svipenyu.cn

Ruby: square = ->(x) { x * x }
来源：http://iwr.pengpengdd.cyou

C#:   Func<int, int> square = x => x * x;
来源：http://pey.wangshuangyany.cn

[C07] 把函数作为参数传入
来源：http://sjr.nanxinkj.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://qhw.shanyushiyangkeji.top

PHP:  array_map("strtoupper", $arr);
来源：http://vzc.316326.xyz

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://llc.fktsv.cn

TS:   arr.map(String)
来源：http://nfz.xuanzx.com

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://jaf.shuidangran.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://bcy.pycfn.com

Ruby: arr.map(&:upcase)
来源：http://bqy.dianchejie.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://jub.mhx1999.top

[C08] 闭包
来源：http://kbx.wangshuangyany.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://uxb.yj202588.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://ivx.nanxuanxn.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://uow.feifeiyinyue.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://jmv.epnwcf.com

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://bpd.hcnkem.com

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://mud.xylfe.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hcf.yonumen.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://shq.haohaochexian.top

[C09] 递归
来源：http://dki.aibaodan.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://xic.vehdjk.com

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://nzn.quarkkingdee.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://vvq.mhx1999.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://etu.jianghu66.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://gxt.shangyingyoupin.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://sfx.hesvh.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://mlx.fktsv.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://jbf.shuidangran.top

[C10] 变量作用域
来源：http://xqa.ywan-chungtsiang.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hki.yanxiufei.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://zti.daxiang520.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://cze.nanxinkj.top

TS:   同 JS
来源：http://fvp.shuidangran.top

Java: 方法内为块级作用域
来源：http://zjz.iojbl.cn

Go:   花括号块级作用域
来源：http://xqd.birdmap.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://zvw.gogol.net.cn

C#:   块级作用域
来源：http://kic.pengpengdd.cyou

[C11] 模块导入与导出
来源：http://fii.yj20258.top

Py:   from module import func
来源：http://pla.wangdashe.top

PHP:  require "file.php";  或 use App\Service;
来源：http://qlj.epnwcf.com

JS:   export default function f() {};  import f from "./m.js";
来源：http://qmz.jlsjyb.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://seo.xuanzx.com

Java: import java.util.List;
来源：http://uip.svipenyu.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://nbo.snrcjt.cn

Ruby: require "json"; require_relative "./util"
来源：http://scg.sweek.top

C#:   using System.Text;
来源：http://ejk.feifeiyinyue.top

[C12] 立即执行函数 IIFE
来源：http://jfv.yonumen.top

Py:   (lambda: print("run"))()
来源：http://jun.yongpay.top

PHP:  (function () { echo "run"; })();
来源：http://uyx.pengpengdd.cyou

JS:   (() => { console.log("run"); })();
来源：http://ren.gogol.net.cn

TS:   (() => { console.log("run"); })();
来源：http://dwe.jqgufenzy.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://lxy.kuanghao11.cn

Go:   func() { fmt.Println("run") }()
来源：http://jyf.jinqigufen.top

Ruby: -> { puts "run" }.call
来源：http://usx.shangyingyoupin.top

C#:   // 无 IIFE：用静态构造函数
来源：http://nkn.shzxlz.cn

[C13] 类型声明 / 类型注解
来源：http://uin.jyoumei.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://xms.yueranfly.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wlw.sysykeji.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://kin.zdqjudy.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://woa.chenlongwang.top

Java: int add(int a, int b) { return a + b; }
来源：http://cww.ydjk.org.cn

Go:   func add(a, b int) int
来源：http://ipe.yj202588.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://dpr.xinyue.icu

C#:   int Add(int a, int b) => a + b;
来源：http://onx.9152youxi.cn

[C14] 泛型函数
来源：http://ggt.wangshuangyany.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://rrz.c1oappe.top

PHP:  // 无泛型
来源：http://ajh.fanxiaobao.xyz

JS:   // 无泛型
来源：http://pvx.tian-w.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://ivo.hesvh.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://yrd.iojbl.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://eny.fzhhl.top

Ruby: # 无泛型
来源：http://kje.snrcjt.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://tun.vehdjk.com

[C15] 解构 / 展开参数
来源：http://gqj.cqqwz.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://tuf.mhx1999.top

PHP:  [$a, $b] = $pair;
来源：http://xne.sysykeji.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://jqy.jqgufenzy.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://lni.andypj.xyz

Java: // 无解构
来源：http://orj.shanyushiyangtech.top

Go:   // 无解构
来源：http://uhz.ydjk.org.cn

Ruby: a, b = pair
来源：http://wia.zycfv.cn

C#:   var (a, b) = pair;
来源：http://dij.yfazqb.com

[C16] 函数 / 方法重载
来源：http://czj.gzhubu.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://zrd.chenzaomai.com

PHP:  // 无重载
来源：http://cpq.xuanzx.com

JS:   // 无重载：靠 arguments.length 分支
来源：http://esp.nanxinkj.top

TS:   // 用联合类型或重载签名声明
来源：http://kmb.shanyushiyangkeji.top

Java: void f(int a) {}  void f(String a) {}
来源：http://dpa.dashuyun.cn

Go:   // 无重载：用不同函数名
来源：http://hhx.zhoulong.xyz

Ruby: # 无重载：靠动态参数
来源：http://njj.gogol.net.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://usy.shangyingyoupin.top

================================================================================
来源：http://nkj.sjlbkw.cn

D. 数组 / 列表 / 集合
来源：http://cht.cheryme.top

================================================================================
来源：http://tkl.zhixingplan.top

[D01] 创建数组 / 列表
来源：http://hxe.ydzc1.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://pvj.wangdashe.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://vmt.quarkkingdee.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://vxn.jqgfzy.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://fio.quarkkingdee.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://srq.xziqi.cn

Go:   arr := []int{1, 2, 3}
来源：http://tum.iojbl.cn

Ruby: arr = [1, 2, 3]
来源：http://yoc.cdnleiting.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://wss.cheryme.top

[D02] 追加元素到末尾
来源：http://cgp.jqgfzy.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://kyd.epnwcf.com

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://vqr.zhoulong.xyz

JS:   arr.push(4);
来源：http://tre.gotoacloud.top

TS:   arr.push(4);
来源：http://pwk.meibo888.top

Java: list.add(4);
来源：http://ypm.cdnleiting.top

Go:   arr = append(arr, 4)
来源：http://qfe.yj202588.top

Ruby: arr << 4; arr.push(5)
来源：http://oiv.0kj1m.cn

C#:   list.Add(4);
来源：http://onx.hcnkem.com

[D03] 在指定位置插入元素
来源：http://frs.sxryk.cn

Py:   arr.insert(0, 0)
来源：http://upz.vehdjk.com

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://gys.zhoulong.xyz

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://pvz.shuidangran.top

TS:   arr.splice(0, 0, 0);
来源：http://nat.jinqigufen.top

Java: list.add(0, 0);
来源：http://jbg.xuetiantiany.cn

Go:   arr = append([]int{0}, arr...)
来源：http://ohu.yongpay.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://uyv.epnwcf.com

C#:   list.Insert(0, 0);
来源：http://jjx.tianlin.xyz

[D04] 删除元素
来源：http://wki.gotoacloud.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://rxg.xinyue.icu

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://frs.ybcxt.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://fvx.vqdsnc.cn

TS:   arr.splice(0, 1);
来源：http://uvq.tian-w.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://vzb.sweek.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://qqg.jinghuilouyu.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://ldu.hcnkem.com

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://fxn.fktsv.cn

[D05] 访问与修改元素
来源：http://lnb.gogol.net.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://bhr.havefunace.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://rmo.quarkkingdee.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hin.hammf.cn

TS:   arr[0]; arr.at(-1);
来源：http://wje.sjlbkw.cn

Java: list.get(0); list.set(0, 9);
来源：http://fes.daxiang520.top

Go:   arr[0]; arr[0] = 9
来源：http://urt.meibo888.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://rum.kuanghao11.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://acf.jqgufenzy.top

[D06] 数组长度
来源：http://gfm.pycfn.com

Py:   len(arr)
来源：http://vng.ydjk.org.cn

PHP:  count($arr);
来源：http://maa.ydzc1.top

JS:   arr.length
来源：http://koy.bbcook.cn

TS:   arr.length
来源：http://shy.jqgufenzy.top

Java: list.size();
来源：http://rvu.epnwcf.com

Go:   len(arr)
来源：http://rcx.jinyuanbaomall.cn

Ruby: arr.length; arr.size
来源：http://udf.316326.xyz

C#:   list.Count;
来源：http://dzr.zhixingplan.top

[D07] 切片 / 取子数组
来源：http://uwh.ydzc1.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://tkd.pengpengdd.cyou

PHP:  array_slice($arr, 1, 3);
来源：http://qhm.hesvh.cn

JS:   arr.slice(1, 4);
来源：http://voo.hnxiangtu.top

TS:   arr.slice(1, 4);
来源：http://ttz.epnwcf.com

Java: list.subList(1, 4);
来源：http://vyd.dianchejie.cn

Go:   arr[1:4]
来源：http://jhj.yuanzhike.top

Ruby: arr[1, 3]
来源：http://myi.ppjwa.cn

C#:   list.GetRange(1, 3);
来源：http://mtg.jqgufenzy.top

[D08] 合并两个数组
来源：http://fda.hcnkem.com

Py:   a + b;  a.extend(b)
来源：http://yqc.vehdjk.com

PHP:  array_merge($a, $b);
来源：http://gaj.yonumen.top

JS:   [...a, ...b];  a.concat(b);
来源：http://ksj.jqgufenzy.top

TS:   [...a, ...b];
来源：http://ixu.xuanzx.com

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://xko.sufxvd.cn

Go:   append(a, b...)
来源：http://ftx.redwolf501.top

Ruby: a + b;  a.concat(b)
来源：http://uwb.jyoumei.cn

C#:   a.Concat(b).ToList()
来源：http://hfa.zhengqikj.top

[D09] 排序（升序）
来源：http://pvo.hfpthk.cn

Py:   sorted(arr);  arr.sort()
来源：http://yah.guowangkeji.top

PHP:  sort($arr);
来源：http://ntg.sufxvd.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://kzq.hesvh.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://nqg.yueranfly.top

Java: Collections.sort(list);  list.sort(null);
来源：http://pij.ehwqpu.com

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://jyz.zdbjq.cn

Ruby: arr.sort
来源：http://oix.yj20258.top

C#:   list.Sort();
来源：http://kqy.pengpengdd.cyou

[D10] 自定义排序（按字段 / 多条件）
来源：http://bqz.kuanghao11.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://bhh.jinghuilouyu.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://tzv.yvedp.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://pdw.pycfn.com

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://oqw.bbcook.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://woe.fanxiaobao.xyz

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://eas.ydzc1.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hyq.dashuyun.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://fzi.fengsongda.top

[D11] 反转数组
来源：http://edx.uphjek.com

Py:   arr[::-1];  arr.reverse()
来源：http://gtu.sysykeji.top

PHP:  array_reverse($arr);
来源：http://njh.hammf.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://krc.zhixingplan.top

TS:   [...arr].reverse();
来源：http://gsv.zhiwuduotai.top

Java: Collections.reverse(list);
来源：http://jfw.jinqigfzy.top

Go:   slices.Reverse(arr)
来源：http://zer.316326.xyz

Ruby: arr.reverse
来源：http://ctq.redwolf501.top

C#:   list.Reverse();
来源：http://hue.yangfankeji.com

[D12] 查找元素下标
来源：http://wol.jlsjyb.cn

Py:   arr.index(x);  x in arr
来源：http://uqr.havefunace.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://twx.shanyushiyangtech.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://bps.0kj1m.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://nyw.9152youxi.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://fuo.gotoacloud.top

Go:   slices.Index(arr, x)
来源：http://kzg.ctjpmb.com

Ruby: arr.index(x)
来源：http://tjg.haohaochexian.top

C#:   list.IndexOf(x);
来源：http://ytb.chenlongwang.top

[D13] 过滤（保留满足条件的）
来源：http://klq.yj20258.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://ogq.kuanghao11.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://sjn.gogol.net.cn

JS:   arr.filter(x => x > 3)
来源：http://avq.cqqwz.cn

TS:   arr.filter(x => x > 3)
来源：http://ybw.gotoacloud.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://cba.0kj1m.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://ala.yongpay.top

Ruby: arr.select { |x| x > 3 }
来源：http://adw.ydjk.org.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://ptq.hnqzz.top

[D14] 映射转换（每个元素变形）
来源：http://zhw.aizwys.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://ynj.feifeiyinyue.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://nzz.vehdjk.com

JS:   arr.map(x => x * 2)
来源：http://yhd.tarul.cn

TS:   arr.map(x => x * 2)
来源：http://mso.jlsjyb.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://kan.jinqigufen.top

Go:   // 手写循环
来源：http://vjd.jianghu66.top

Ruby: arr.map { |x| x * 2 }
来源：http://tzx.ehwqpu.com

C#:   list.Select(x => x * 2).ToList()
来源：http://vrv.yuxming.cn

[D15] 去重
来源：http://qay.gogol.net.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://nbz.yueranfly.top

PHP:  array_unique($arr);
来源：http://qsu.haohaochexian.top

JS:   [...new Set(arr)]
来源：http://mfo.yonumen.top

TS:   [...new Set(arr)]
来源：http://dlf.9152youxi.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://wii.zhijiandao.cn

Go:   // 用 map[T]struct{} 手写
来源：http://ocu.tarul.cn

Ruby: arr.uniq
来源：http://trd.tianlin.xyz

C#:   list.Distinct().ToList()
来源：http://kte.tanke756.top

[D16] 求和与平均值
来源：http://lfl.aibaodan.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://jlu.nwbrower.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://ioe.ppjwa.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://vbm.sweek.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://gyz.ehwqpu.com

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://cyq.xinyue.icu

Go:   // 手写循环累加
来源：http://qyo.tarul.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://gjr.fengsongda.top

C#:   list.Sum();  list.Average()
来源：http://wxg.hfpthk.cn

[D17] 最大值与最小值
来源：http://zhf.yj20258888.top

Py:   max(arr);  min(arr)
来源：http://vch.daria6918.cn

PHP:  max($arr);  min($arr);
来源：http://ecl.sweek.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://knz.jinghuilouyu.cn

TS:   Math.max(...arr);
来源：http://txz.hnxiangtu.top

Java: Collections.max(list);  Collections.min(list);
来源：http://zqo.dashuyun.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://wjt.cucudq.cn

Ruby: arr.max;  arr.min
来源：http://brq.guowangkeji.top

C#:   list.Max();  list.Min()
来源：http://siz.cheryme.top

[D18] 扁平化嵌套数组
来源：http://xto.havefunace.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://lwk.kuanghao11.cn

PHP:  array_merge(...$nested);
来源：http://kws.sufxvd.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://wyw.ivvv.top

TS:   nested.flat();
来源：http://gym.andypj.xyz

Java: nested.stream().flatMap(List::stream).toList()
来源：http://sqn.ydjk.org.cn

Go:   // 手写双层循环
来源：http://ofj.316326.xyz

Ruby: nested.flatten
来源：http://puk.zycfv.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://srp.xingfuxueyuan.xyz

[D19] 按字段分组
来源：http://gbh.kuanghao11.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://rjs.vehdjk.com

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://wqr.zdbjq.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://qyc.jinyuanbaomall.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://dka.bbcook.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://blj.wangshuangyany.cn

Go:   // 手写 map[string][]T
来源：http://evp.yvedp.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://cfp.cashguo.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://npr.guannengcc.top

[D20] 统计每个元素出现次数
来源：http://dlo.quarkkingdee.top

Py:   Counter(arr)
来源：http://wyf.hongshengwenyu.top

PHP:  array_count_values($arr);
来源：http://xiv.sysykeji.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://nhu.bjfxy.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://xxn.daxiang520.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://nju.xziqi.cn

Go:   // 手写 map[T]int
来源：http://npm.redwolf501.top

Ruby: arr.tally
来源：http://uvs.hysaishi.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://qub.yvedp.cn

[D21] 判断是否包含某元素
来源：http://ldu.fzhhl.top

Py:   x in arr
来源：http://jrw.hnxiangtu.top

PHP:  in_array($x, $arr, true);
来源：http://cjx.feifeiyinyue.top

JS:   arr.includes(x)
来源：http://tck.chenlongwang.top

TS:   arr.includes(x)
来源：http://znn.hongshengwenyu.top

Java: list.contains(x)
来源：http://fix.ehwqpu.com

Go:   slices.Contains(arr, x)
来源：http://seb.shanyushiyangtech.top

Ruby: arr.include?(x)
来源：http://ghv.pengpengdd.cyou

C#:   list.Contains(x)
来源：http://gsj.gotoacloud.top

[D22] 复制数组（避免共享引用）
来源：http://woz.hfpthk.cn


<!-- 参考信息 -->