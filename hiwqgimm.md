代发 wailian999

Go:   // 无：用配置结构体参数
来源：http://rhh.fktsv.cn

Ruby: f(a: 1, b: 2)
来源：http://pby.ppjwa.cn

C#:   f(a: 1, b: 2)
来源：http://kuw.wangdashe.top

[C05] 返回多个值
来源：http://nsz.pycfn.com

Py:   return a, b
来源：http://iqc.shuidangran.top

PHP:  return [$a, $b];
来源：http://koy.nanxinkj.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://yxe.chenlongwang.top

TS:   return { a, b };
来源：http://jfa.jianghu66.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://rca.c1oappe.top

Go:   return a, b
来源：http://hku.yueranfly.top

Ruby: return a, b
来源：http://brl.fehbvm.com

C#:   return (a, b);              // ValueTuple
来源：http://zbw.vehdjk.com

[C06] 匿名函数 / lambda
来源：http://ckw.cqqwz.cn

Py:   square = lambda x: x * x
来源：http://twj.jinyuanbaomall.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://bwi.tian-w.cn

JS:   const square = x => x * x;
来源：http://yjf.guowangkeji.top

TS:   const square = (x: number): number => x * x;
来源：http://rzp.gaohongyu789.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://fup.guannengcc.top

Go:   sq := func(x int) int { return x * x }
来源：http://iuf.dianchejie.cn

Ruby: square = ->(x) { x * x }
来源：http://tug.guowangkeji.top

C#:   Func<int, int> square = x => x * x;
来源：http://skz.yuanzhike.top

[C07] 把函数作为参数传入
来源：http://cpg.fktsv.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://zpu.nanxuanxn.top

PHP:  array_map("strtoupper", $arr);
来源：http://ooo.vehdjk.com

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://axv.tarul.cn

TS:   arr.map(String)
来源：http://nbm.jianghu66.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://ehi.hongshengwenyu.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://adl.shuidangran.top

Ruby: arr.map(&:upcase)
来源：http://qnn.fzhhl.top

C#:   arr.Select(s => s.ToUpper())
来源：http://lfl.nanxuanxn.top

[C08] 闭包
来源：http://ksc.yonumen.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://cja.haohaochexian.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://oui.yuanzhike.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://fih.jyoumei.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://vlh.hammf.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://awl.wangdashe.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://fcc.smart0.xyz

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://ouk.yonumen.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://pag.birdmap.top

[C09] 递归
来源：http://byb.pycfn.com

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://ijf.9152youxi.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://wmn.daria6918.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://iyw.guowangkeji.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://pfs.birdmap.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://cnj.redwolf501.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://kph.jinghuilouyu.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://jje.tarul.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://xnt.yfazqb.com

[C10] 变量作用域
来源：http://coq.zhaomingkeji.xyz

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://dep.cheryme.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hvi.yuxming.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://bzw.quarkkingdee.top

TS:   同 JS
来源：http://idw.sysykeji.top

Java: 方法内为块级作用域
来源：http://rcs.pengpengdd.cyou

Go:   花括号块级作用域
来源：http://cmu.cqqwz.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://tcl.yfazqb.com

C#:   块级作用域
来源：http://mvq.daria6918.cn

[C11] 模块导入与导出
来源：http://qev.fzhhl.top

Py:   from module import func
来源：http://jie.iojbl.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://euf.xingfuxueyuan.xyz

JS:   export default function f() {};  import f from "./m.js";
来源：http://wnr.quarkkingdee.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://kcp.9152youxi.cn

Java: import java.util.List;
来源：http://wgr.guannengcc.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hcb.nanxuanxn.top

Ruby: require "json"; require_relative "./util"
来源：http://igc.hywenlv.cn

C#:   using System.Text;
来源：http://bki.316326.xyz

[C12] 立即执行函数 IIFE
来源：http://xis.yongpay.top

Py:   (lambda: print("run"))()
来源：http://cqg.fehbvm.com

PHP:  (function () { echo "run"; })();
来源：http://isy.yfazqb.com

JS:   (() => { console.log("run"); })();
来源：http://epc.zhaomingkeji.xyz

TS:   (() => { console.log("run"); })();
来源：http://dom.jinyuanbaomall.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://nvr.shuidangran.top

Go:   func() { fmt.Println("run") }()
来源：http://czg.chenzaomai.com

Ruby: -> { puts "run" }.call
来源：http://lvp.yongpay.top

C#:   // 无 IIFE：用静态构造函数
来源：http://pdk.zhaomingkeji.xyz

[C13] 类型声明 / 类型注解
来源：http://xzt.chenlongwang.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://tkx.zhixingplan.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://zat.fanxiaobao.xyz

JS:   // 无类型（可用 JSDoc 注释）
来源：http://lyw.redwolf501.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://pia.nanxinkj.top

Java: int add(int a, int b) { return a + b; }
来源：http://hcu.jinqigfzy.top

Go:   func add(a, b int) int
来源：http://baa.sjlbkw.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://ovu.fzhhl.top

C#:   int Add(int a, int b) => a + b;
来源：http://vgx.zhixingplan.top

[C14] 泛型函数
来源：http://ahl.hysaishi.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://xvi.chenlongwang.top

PHP:  // 无泛型
来源：http://uli.guowangkeji.top

JS:   // 无泛型
来源：http://qhr.cucudq.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://xrr.sxryk.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://usp.chenzaomai.com

Go:   func First[T any](items []T) T { return items[0] }
来源：http://dmn.svipenyu.cn

Ruby: # 无泛型
来源：http://duu.pycfn.com

C#:   static T First<T>(List<T> items) => items[0];
来源：http://fwe.dianchejie.cn

[C15] 解构 / 展开参数
来源：http://fsn.birdmap.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://plo.jinqigufen.top

PHP:  [$a, $b] = $pair;
来源：http://ego.gzhubu.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://fwg.xziqi.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://abk.sufxvd.cn

Java: // 无解构
来源：http://tqh.jyoumei.cn

Go:   // 无解构
来源：http://nit.gotoacloud.top

Ruby: a, b = pair
来源：http://cdv.fehbvm.com

C#:   var (a, b) = pair;
来源：http://ggq.ydjk.org.cn

[C16] 函数 / 方法重载
来源：http://lpn.aizwys.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://wqp.bbcook.cn

PHP:  // 无重载
来源：http://hzn.fehbvm.com

JS:   // 无重载：靠 arguments.length 分支
来源：http://mhp.fehbvm.com

TS:   // 用联合类型或重载签名声明
来源：http://vby.quarkkingdee.top

Java: void f(int a) {}  void f(String a) {}
来源：http://ugu.jinqigfzy.top

Go:   // 无重载：用不同函数名
来源：http://abd.quarkkingdee.top

Ruby: # 无重载：靠动态参数
来源：http://tej.kuanghao11.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://ncb.hesvh.cn

================================================================================
来源：http://yat.zhijiandao.cn

D. 数组 / 列表 / 集合
来源：http://uct.chenjidiqi.icu

================================================================================
来源：http://yza.yongpay.top

[D01] 创建数组 / 列表
来源：http://cbu.dianchejie.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://ujb.xinyue.icu

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://ckd.pengpengdd.cyou

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://npr.pengpengdd.cyou

TS:   const arr: number[] = [1, 2, 3];
来源：http://lbu.yj20258.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://rub.gzhubu.top

Go:   arr := []int{1, 2, 3}
来源：http://jrw.dashuyun.cn

Ruby: arr = [1, 2, 3]
来源：http://kqx.hnqzz.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://ksk.andypj.xyz

[D02] 追加元素到末尾
来源：http://kjt.snrcjt.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://mic.ydzc1.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://sne.daria6918.cn

JS:   arr.push(4);
来源：http://pty.yuanzhike.top

TS:   arr.push(4);
来源：http://mho.9152youxi.cn

Java: list.add(4);
来源：http://jeb.chenzaomai.com

Go:   arr = append(arr, 4)
来源：http://lrm.nanxinkj.top

Ruby: arr << 4; arr.push(5)
来源：http://uhk.hammf.cn

C#:   list.Add(4);
来源：http://nob.zdqjudy.top

[D03] 在指定位置插入元素
来源：http://ash.quarkkingdee.top

Py:   arr.insert(0, 0)
来源：http://qqp.hcnkem.com

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://edf.hnqzz.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hlo.hongshengwenyu.top

TS:   arr.splice(0, 0, 0);
来源：http://hod.yuxming.cn

Java: list.add(0, 0);
来源：http://nlk.jinghuilouyu.cn

Go:   arr = append([]int{0}, arr...)
来源：http://wmo.chenlongwang.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://usm.yj20258888.top

C#:   list.Insert(0, 0);
来源：http://rdo.hammf.cn

[D04] 删除元素
来源：http://wit.shanyushiyangtech.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://vby.fengsongda.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://ejv.havefunace.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://giz.kuanghao11.cn

TS:   arr.splice(0, 1);
来源：http://hph.havefunace.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://egd.xuetiantiany.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://bkl.yuxming.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://ksy.yonumen.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://ofl.ydzc1.top

[D05] 访问与修改元素
来源：http://rcr.jinghuilouyu.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://jjq.dashuyun.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://ydg.yj20258.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://oog.316326.xyz

TS:   arr[0]; arr.at(-1);
来源：http://lqj.redwolf501.top

Java: list.get(0); list.set(0, 9);
来源：http://jiq.zhengqikj.top

Go:   arr[0]; arr[0] = 9
来源：http://lhc.hysaishi.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://qzm.wangshuangyany.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://ewe.xinyue.icu

[D06] 数组长度
来源：http://wri.yfazqb.com

Py:   len(arr)
来源：http://hsa.jyoumei.cn

PHP:  count($arr);
来源：http://mfz.ydzc1.top

JS:   arr.length
来源：http://izf.gotoacloud.top

TS:   arr.length
来源：http://qdl.zycfv.cn

Java: list.size();
来源：http://ggo.jyoumei.cn

Go:   len(arr)
来源：http://xuv.hesvh.cn

Ruby: arr.length; arr.size
来源：http://sqh.gotoacloud.top

C#:   list.Count;
来源：http://cmj.tarul.cn

[D07] 切片 / 取子数组
来源：http://jcy.hysaishi.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://fis.snrcjt.cn

PHP:  array_slice($arr, 1, 3);
来源：http://ibp.gzhubu.top

JS:   arr.slice(1, 4);
来源：http://kxj.ywan-chungtsiang.top

TS:   arr.slice(1, 4);
来源：http://uxj.xziqi.cn

Java: list.subList(1, 4);
来源：http://dmg.hnqzz.top

Go:   arr[1:4]
来源：http://vgn.pycfn.com

Ruby: arr[1, 3]
来源：http://xpb.wangshuangyany.cn

C#:   list.GetRange(1, 3);
来源：http://jog.hywenlv.cn

[D08] 合并两个数组
来源：http://qwc.uphjek.com

Py:   a + b;  a.extend(b)
来源：http://oaj.hywenlv.cn

PHP:  array_merge($a, $b);
来源：http://nme.fanxiaobao.xyz

JS:   [...a, ...b];  a.concat(b);
来源：http://qsd.jlsjyb.cn

TS:   [...a, ...b];
来源：http://knu.hywenlv.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://fup.dashuyun.cn

Go:   append(a, b...)
来源：http://sms.vqdsnc.cn

Ruby: a + b;  a.concat(b)
来源：http://ixi.svipenyu.cn

C#:   a.Concat(b).ToList()
来源：http://kjr.dianchejie.cn

[D09] 排序（升序）
来源：http://tai.quarkkingdee.top

Py:   sorted(arr);  arr.sort()
来源：http://iaj.fehbvm.com

PHP:  sort($arr);
来源：http://glh.yueranfly.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://dmy.vehdjk.com

TS:   [...arr].sort((x, y) => x - y);
来源：http://pgf.gotoacloud.top

Java: Collections.sort(list);  list.sort(null);
来源：http://tbo.xuetiantiany.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://xjt.kuanghao11.cn

Ruby: arr.sort
来源：http://mxy.meibo888.top

C#:   list.Sort();
来源：http://whg.ybcxt.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://chw.shuidangran.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://rmf.iojbl.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://des.sysykeji.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://awu.yueranfly.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://odm.redwolf501.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://uly.jyoumei.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hur.tanke756.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://yip.hywenlv.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://jkl.chenzaomai.com

[D11] 反转数组
来源：http://jyj.aibaodan.cn

Py:   arr[::-1];  arr.reverse()
来源：http://osl.52xcode.cn

PHP:  array_reverse($arr);
来源：http://hqn.ywan-chungtsiang.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://oyy.cqqwz.cn

TS:   [...arr].reverse();
来源：http://fee.pycfn.com

Java: Collections.reverse(list);
来源：http://nwb.yvedp.cn

Go:   slices.Reverse(arr)
来源：http://uhr.yuxming.cn

Ruby: arr.reverse
来源：http://yfv.chenzaomai.com

C#:   list.Reverse();
来源：http://pke.xuetiantiany.cn

[D12] 查找元素下标
来源：http://qgl.haohaochexian.top

Py:   arr.index(x);  x in arr
来源：http://gqt.daxiang520.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://afd.aibaodan.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ghn.xingfuxueyuan.xyz

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://bjo.bbcook.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://uuh.aizwys.cn

Go:   slices.Index(arr, x)
来源：http://dte.gotoacloud.top

Ruby: arr.index(x)
来源：http://hnk.ehwqpu.com

C#:   list.IndexOf(x);
来源：http://upk.jinyuanbaomall.cn

[D13] 过滤（保留满足条件的）
来源：http://cyw.sjlbkw.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://qaz.jinyuanbaomall.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://rzs.snrcjt.cn

JS:   arr.filter(x => x > 3)
来源：http://twb.0kj1m.cn

TS:   arr.filter(x => x > 3)
来源：http://nfo.redwolf501.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://opo.kuanghao11.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://qac.ppjwa.cn

Ruby: arr.select { |x| x > 3 }
来源：http://eps.jlsjyb.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://rxq.tanke756.top

[D14] 映射转换（每个元素变形）
来源：http://rxc.aibaodan.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://oto.zhaomingkeji.xyz

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://dno.ppjwa.cn

JS:   arr.map(x => x * 2)
来源：http://ybe.yvedp.cn

TS:   arr.map(x => x * 2)
来源：http://qly.zdbjq.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://flr.aizwys.cn

Go:   // 手写循环
来源：http://tsi.52xcode.cn

Ruby: arr.map { |x| x * 2 }
来源：http://hzz.shuidangran.top

C#:   list.Select(x => x * 2).ToList()
来源：http://wud.sweek.top

[D15] 去重
来源：http://cyh.tarul.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://soi.jyoumei.cn

PHP:  array_unique($arr);
来源：http://uoq.yuxming.cn

JS:   [...new Set(arr)]
来源：http://pbx.hongshengwenyu.top

TS:   [...new Set(arr)]
来源：http://izw.yj20258888.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://ruj.hnxiangtu.top

Go:   // 用 map[T]struct{} 手写
来源：http://yal.bjfxy.top

Ruby: arr.uniq
来源：http://pxh.316326.xyz

C#:   list.Distinct().ToList()
来源：http://nfo.jinyuanbaomall.cn

[D16] 求和与平均值
来源：http://vfa.zhiwuduotai.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://uhj.guannengcc.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://etz.hywenlv.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://bhe.zhijiandao.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://lgg.9152youxi.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://ghz.mhx1999.top

Go:   // 手写循环累加
来源：http://lbs.zycfv.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://qoe.epnwcf.com

C#:   list.Sum();  list.Average()
来源：http://nhh.zdbjq.cn

[D17] 最大值与最小值
来源：http://fbb.fehbvm.com

Py:   max(arr);  min(arr)
来源：http://tvv.daria6918.cn

PHP:  max($arr);  min($arr);
来源：http://sly.aibaodan.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://obq.shangyingyoupin.top

TS:   Math.max(...arr);
来源：http://xyc.xingfuxueyuan.xyz

Java: Collections.max(list);  Collections.min(list);
来源：http://wdi.svipenyu.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://whi.ydjk.org.cn

Ruby: arr.max;  arr.min
来源：http://ymu.quarkkingdee.top

C#:   list.Max();  list.Min()
来源：http://udn.cashguo.top

[D18] 扁平化嵌套数组
来源：http://mpl.gaohongyu789.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://crq.shzxlz.cn

PHP:  array_merge(...$nested);
来源：http://ang.ydzc1.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://atw.cdnleiting.top

TS:   nested.flat();
来源：http://hzb.zhixingplan.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://rei.yongpay.top

Go:   // 手写双层循环
来源：http://bmb.hcnkem.com

Ruby: nested.flatten
来源：http://lat.yuanzhike.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://hky.hcnkem.com

[D19] 按字段分组
来源：http://qem.mhx1999.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://bxu.zycfv.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://vca.gzhubu.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://iwq.daxiang520.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://rbv.shuidangran.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://nek.zhijiandao.cn

Go:   // 手写 map[string][]T
来源：http://wpy.jyoumei.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://qst.hongshengwenyu.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://xqj.yj20258888.top

[D20] 统计每个元素出现次数
来源：http://pxq.sjlbkw.cn

Py:   Counter(arr)
来源：http://hzp.sweek.top

PHP:  array_count_values($arr);
来源：http://dae.hesvh.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ujv.pengpengdd.cyou

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ygd.hywenlv.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://mcy.jinqigfzy.top

Go:   // 手写 map[T]int
来源：http://zew.0kj1m.cn

Ruby: arr.tally
来源：http://ijt.316326.xyz

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://rpi.xziqi.cn

[D21] 判断是否包含某元素
来源：http://mkp.uphjek.com

Py:   x in arr
来源：http://kvh.ywan-chungtsiang.top

PHP:  in_array($x, $arr, true);
来源：http://bjs.guannengcc.top

JS:   arr.includes(x)
来源：http://hao.hammf.cn

TS:   arr.includes(x)
来源：http://qah.ehwqpu.com

Java: list.contains(x)
来源：http://lgx.haohaochexian.top


<!-- 参考信息 -->