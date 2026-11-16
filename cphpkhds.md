代发 wailian999

Go:   // 无：用配置结构体参数
来源：http://glf.aizwys.cn

Ruby: f(a: 1, b: 2)
来源：http://ted.sjlbkw.cn

C#:   f(a: 1, b: 2)
来源：http://hld.jinyuanbaomall.cn

[C05] 返回多个值
来源：http://oln.xylfe.cn

Py:   return a, b
来源：http://uom.sxryk.cn

PHP:  return [$a, $b];
来源：http://mza.guowangkeji.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://nux.ehwqpu.com

TS:   return { a, b };
来源：http://ptt.yj20258.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://jhw.jinyuanbaomall.cn

Go:   return a, b
来源：http://ubi.hesvh.cn

Ruby: return a, b
来源：http://gqg.hysaishi.cn

C#:   return (a, b);              // ValueTuple
来源：http://imq.tarul.cn

[C06] 匿名函数 / lambda
来源：http://fyi.shanyushiyangkeji.top

Py:   square = lambda x: x * x
来源：http://bsa.jinghuilouyu.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://eba.xingfuxueyuan.xyz

JS:   const square = x => x * x;
来源：http://wem.bbcook.cn

TS:   const square = (x: number): number => x * x;
来源：http://zce.c1oappe.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://vpw.zhoulong.xyz

Go:   sq := func(x int) int { return x * x }
来源：http://wro.cdnleiting.top

Ruby: square = ->(x) { x * x }
来源：http://ten.shzxlz.cn

C#:   Func<int, int> square = x => x * x;
来源：http://cft.dianchejie.cn

[C07] 把函数作为参数传入
来源：http://qfg.sweek.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://vcd.zhiwuduotai.top

PHP:  array_map("strtoupper", $arr);
来源：http://snc.ehwqpu.com

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://ryf.cashguo.top

TS:   arr.map(String)
来源：http://kqo.yanxiufei.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://pmo.gaohongyu789.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://juj.xinyue.icu

Ruby: arr.map(&:upcase)
来源：http://spv.hysaishi.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://cbe.bjfxy.top

[C08] 闭包
来源：http://ynx.epnwcf.com

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://mcb.jinqigfzy.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hwd.daria6918.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://qzc.yuxming.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://udn.bbcook.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://dry.andypj.xyz

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://szt.zhijiandao.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://ofc.zhengqikj.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://jaz.pycfn.com

[C09] 递归
来源：http://tjy.gotoacloud.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://ucs.sufxvd.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://ywl.cqqwz.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://rjd.yfazqb.com

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://gcs.zdqjudy.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://rca.yangfankeji.com

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hup.xziqi.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://oie.yj202588.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://brl.xziqi.cn

[C10] 变量作用域
来源：http://yoc.jinqigfzy.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://vpq.jqgufenzy.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://cxr.tanke756.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://imn.wangdashe.top

TS:   同 JS
来源：http://pgq.iojbl.cn

Java: 方法内为块级作用域
来源：http://wsk.ywan-chungtsiang.top

Go:   花括号块级作用域
来源：http://wzj.sweek.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://rue.wangshuangyany.cn

C#:   块级作用域
来源：http://okc.vqdsnc.cn

[C11] 模块导入与导出
来源：http://chg.yj20258888.top

Py:   from module import func
来源：http://koe.xuetiantiany.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://pye.sweek.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://xey.hongshengwenyu.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://spz.52xcode.cn

Java: import java.util.List;
来源：http://vhc.hnxiangtu.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://wnu.hnxiangtu.top

Ruby: require "json"; require_relative "./util"
来源：http://nne.fehbvm.com

C#:   using System.Text;
来源：http://wwi.feifeiyinyue.top

[C12] 立即执行函数 IIFE
来源：http://hnj.dianchejie.cn

Py:   (lambda: print("run"))()
来源：http://wax.nanxuanxn.top

PHP:  (function () { echo "run"; })();
来源：http://gvo.cheryme.top

JS:   (() => { console.log("run"); })();
来源：http://siy.andypj.xyz

TS:   (() => { console.log("run"); })();
来源：http://pvg.gogol.net.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://lok.xziqi.cn

Go:   func() { fmt.Println("run") }()
来源：http://bzm.vehdjk.com

Ruby: -> { puts "run" }.call
来源：http://csf.wangdashe.top

C#:   // 无 IIFE：用静态构造函数
来源：http://vll.bbcook.cn

[C13] 类型声明 / 类型注解
来源：http://xsu.cheryme.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://nvx.zdbjq.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://saa.feifeiyinyue.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://cje.zycfv.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mdp.hywenlv.cn

Java: int add(int a, int b) { return a + b; }
来源：http://gfj.shuidangran.top

Go:   func add(a, b int) int
来源：http://trk.yanxiufei.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://vcb.cheryme.top

C#:   int Add(int a, int b) => a + b;
来源：http://rdz.chenlongwang.top

[C14] 泛型函数
来源：http://dil.fktsv.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://vsu.yuxming.cn

PHP:  // 无泛型
来源：http://irk.aizwys.cn

JS:   // 无泛型
来源：http://vma.smart0.xyz

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://fjm.hnqzz.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://pcw.jinghuilouyu.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://beh.0kj1m.cn

Ruby: # 无泛型
来源：http://ifb.yanxiufei.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://mzr.shanyushiyangtech.top

[C15] 解构 / 展开参数
来源：http://xkd.yueranfly.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://xwa.hnxiangtu.top

PHP:  [$a, $b] = $pair;
来源：http://kho.cashguo.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://zup.tarul.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://ifb.aibaodan.cn

Java: // 无解构
来源：http://pfs.zdqjudy.top

Go:   // 无解构
来源：http://fzv.cucudq.cn

Ruby: a, b = pair
来源：http://qzn.ydzc1.top

C#:   var (a, b) = pair;
来源：http://lai.cucudq.cn

[C16] 函数 / 方法重载
来源：http://cys.aibaodan.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://qrs.chenzaomai.com

PHP:  // 无重载
来源：http://flx.xuanzx.com

JS:   // 无重载：靠 arguments.length 分支
来源：http://xmr.shangyingyoupin.top

TS:   // 用联合类型或重载签名声明
来源：http://coi.birdmap.top

Java: void f(int a) {}  void f(String a) {}
来源：http://fim.zhijiandao.cn

Go:   // 无重载：用不同函数名
来源：http://wbc.zhiwuduotai.top

Ruby: # 无重载：靠动态参数
来源：http://nge.hammf.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://iag.shangyingyoupin.top

================================================================================
来源：http://mgq.andypj.xyz

D. 数组 / 列表 / 集合
来源：http://rru.fktsv.cn

================================================================================
来源：http://boi.tian-w.cn

[D01] 创建数组 / 列表
来源：http://rzp.pengpengdd.cyou

Py:   arr = [1, 2, 3];  empty = []
来源：http://nxq.yvedp.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://noq.quarkkingdee.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://dwz.aibaodan.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://ymn.kuanghao11.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://ovk.chenlongwang.top

Go:   arr := []int{1, 2, 3}
来源：http://mqt.pengpengdd.cyou

Ruby: arr = [1, 2, 3]
来源：http://nwg.feifeiyinyue.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://mkb.feifeiyinyue.top

[D02] 追加元素到末尾
来源：http://adc.jianghu66.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hlr.sxryk.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://czr.aizwys.cn

JS:   arr.push(4);
来源：http://kes.vehdjk.com

TS:   arr.push(4);
来源：http://xar.uphjek.com

Java: list.add(4);
来源：http://eps.ywan-chungtsiang.top

Go:   arr = append(arr, 4)
来源：http://jlc.pengpengdd.cyou

Ruby: arr << 4; arr.push(5)
来源：http://uid.yvedp.cn

C#:   list.Add(4);
来源：http://jmb.316326.xyz

[D03] 在指定位置插入元素
来源：http://hbn.chenlongwang.top

Py:   arr.insert(0, 0)
来源：http://ism.ctjpmb.com

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://sda.nanxuanxn.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://bsp.daria6918.cn

TS:   arr.splice(0, 0, 0);
来源：http://hog.hcnkem.com

Java: list.add(0, 0);
来源：http://lbq.andypj.xyz

Go:   arr = append([]int{0}, arr...)
来源：http://rrv.yonumen.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://ipr.ehwqpu.com

C#:   list.Insert(0, 0);
来源：http://bdz.dianchejie.cn

[D04] 删除元素
来源：http://rsd.hesvh.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://mwa.jinqigufen.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://ynr.cheryme.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://isd.316326.xyz

TS:   arr.splice(0, 1);
来源：http://rqm.ydjk.org.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://lrw.guowangkeji.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://udz.shzxlz.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://ddk.zdqjudy.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://xay.fktsv.cn

[D05] 访问与修改元素
来源：http://oty.wangdashe.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://zgb.yongpay.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://yyn.xziqi.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://eic.uphjek.com

TS:   arr[0]; arr.at(-1);
来源：http://ote.fzhhl.top

Java: list.get(0); list.set(0, 9);
来源：http://soq.jlsjyb.cn

Go:   arr[0]; arr[0] = 9
来源：http://evb.vqdsnc.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://kav.ydzc1.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://jlx.xingfuxueyuan.xyz

[D06] 数组长度
来源：http://tqx.sufxvd.cn

Py:   len(arr)
来源：http://egm.tianlin.xyz

PHP:  count($arr);
来源：http://bpd.yongpay.top

JS:   arr.length
来源：http://ent.xuetiantiany.cn

TS:   arr.length
来源：http://wlq.316326.xyz

Java: list.size();
来源：http://cpn.shanyushiyangkeji.top

Go:   len(arr)
来源：http://dqe.smart0.xyz

Ruby: arr.length; arr.size
来源：http://dcd.mhx1999.top

C#:   list.Count;
来源：http://thc.bjfxy.top

[D07] 切片 / 取子数组
来源：http://fho.tian-w.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://xue.xingfuxueyuan.xyz

PHP:  array_slice($arr, 1, 3);
来源：http://jcx.yueranfly.top

JS:   arr.slice(1, 4);
来源：http://yzv.sysykeji.top

TS:   arr.slice(1, 4);
来源：http://ree.xuanzx.com

Java: list.subList(1, 4);
来源：http://vcy.gzhubu.top

Go:   arr[1:4]
来源：http://bjq.jianghu66.top

Ruby: arr[1, 3]
来源：http://vyt.gaohongyu789.top

C#:   list.GetRange(1, 3);
来源：http://zzx.birdmap.top

[D08] 合并两个数组
来源：http://xfx.ywan-chungtsiang.top

Py:   a + b;  a.extend(b)
来源：http://tck.cashguo.top

PHP:  array_merge($a, $b);
来源：http://rxw.316326.xyz

JS:   [...a, ...b];  a.concat(b);
来源：http://had.vqdsnc.cn

TS:   [...a, ...b];
来源：http://hkt.cqqwz.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://fzm.guannengcc.top

Go:   append(a, b...)
来源：http://wtm.aizwys.cn

Ruby: a + b;  a.concat(b)
来源：http://fsc.yj202588.top

C#:   a.Concat(b).ToList()
来源：http://prr.yfazqb.com

[D09] 排序（升序）
来源：http://vdi.jqgfzy.top

Py:   sorted(arr);  arr.sort()
来源：http://akq.wangdashe.top

PHP:  sort($arr);
来源：http://pxe.hywenlv.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hax.tanke756.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://txu.smart0.xyz

Java: Collections.sort(list);  list.sort(null);
来源：http://ufb.xuanzx.com

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://ycr.cucudq.cn

Ruby: arr.sort
来源：http://dyj.0kj1m.cn

C#:   list.Sort();
来源：http://neg.nanxinkj.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://rmm.meibo888.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://jkg.hywenlv.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://pcp.epnwcf.com

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://qoo.yuanzhike.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://bxy.shanyushiyangtech.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://zrn.hfpthk.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://xpv.iojbl.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://aal.redwolf501.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://ysx.yongpay.top

[D11] 反转数组
来源：http://jza.fanxiaobao.xyz

Py:   arr[::-1];  arr.reverse()
来源：http://fsk.yuanzhike.top

PHP:  array_reverse($arr);
来源：http://xfz.epnwcf.com

JS:   [...arr].reverse();  arr.toReversed()
来源：http://ire.shzxlz.cn

TS:   [...arr].reverse();
来源：http://cza.mhx1999.top

Java: Collections.reverse(list);
来源：http://ulo.uphjek.com

Go:   slices.Reverse(arr)
来源：http://izq.jinqigufen.top

Ruby: arr.reverse
来源：http://peq.xuetiantiany.cn

C#:   list.Reverse();
来源：http://mbq.yuxming.cn

[D12] 查找元素下标
来源：http://dyh.daxiang520.top

Py:   arr.index(x);  x in arr
来源：http://pzd.shuidangran.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://bst.sufxvd.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://eba.0kj1m.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://iog.meibo888.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://gua.cashguo.top

Go:   slices.Index(arr, x)
来源：http://xnq.jinqigufen.top

Ruby: arr.index(x)
来源：http://iko.hammf.cn

C#:   list.IndexOf(x);
来源：http://ifh.jinqigfzy.top

[D13] 过滤（保留满足条件的）
来源：http://mym.ivvv.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://kuc.yj20258.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://jum.zhaomingkeji.xyz

JS:   arr.filter(x => x > 3)
来源：http://ynm.tarul.cn

TS:   arr.filter(x => x > 3)
来源：http://boe.feifeiyinyue.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://dej.cheryme.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://onp.ctjpmb.com

Ruby: arr.select { |x| x > 3 }
来源：http://ogv.cdnleiting.top

C#:   list.Where(x => x > 3).ToList()
来源：http://ntn.c1oappe.top

[D14] 映射转换（每个元素变形）
来源：http://xoh.cucudq.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://ifs.gotoacloud.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://cpz.haohaochexian.top

JS:   arr.map(x => x * 2)
来源：http://xwa.fanxiaobao.xyz

TS:   arr.map(x => x * 2)
来源：http://zds.birdmap.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://jno.fehbvm.com

Go:   // 手写循环
来源：http://rjz.xziqi.cn

Ruby: arr.map { |x| x * 2 }
来源：http://lrh.c1oappe.top

C#:   list.Select(x => x * 2).ToList()
来源：http://uqo.jinyuanbaomall.cn

[D15] 去重
来源：http://oud.jqgufenzy.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://drk.gogol.net.cn

PHP:  array_unique($arr);
来源：http://iea.fengsongda.top

JS:   [...new Set(arr)]
来源：http://vhs.shanyushiyangtech.top

TS:   [...new Set(arr)]
来源：http://nes.yj20258888.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://lfk.svipenyu.cn

Go:   // 用 map[T]struct{} 手写
来源：http://fzo.hnxiangtu.top

Ruby: arr.uniq
来源：http://nju.jinqigufen.top

C#:   list.Distinct().ToList()
来源：http://qpe.daria6918.cn

[D16] 求和与平均值
来源：http://mbh.yj202588.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://pdh.hcnkem.com

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://xzv.shzxlz.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://jzd.yvedp.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://qaf.zhixingplan.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://tdw.jyoumei.cn

Go:   // 手写循环累加
来源：http://uxs.shanyushiyangtech.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://gro.yueranfly.top

C#:   list.Sum();  list.Average()
来源：http://ekp.hesvh.cn

[D17] 最大值与最小值
来源：http://yfc.yuanzhike.top

Py:   max(arr);  min(arr)
来源：http://jeh.andypj.xyz

PHP:  max($arr);  min($arr);
来源：http://oqq.zhijiandao.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://acf.jlsjyb.cn

TS:   Math.max(...arr);
来源：http://vfr.xuanzx.com

Java: Collections.max(list);  Collections.min(list);
来源：http://cny.zhaomingkeji.xyz

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://pun.ivvv.top

Ruby: arr.max;  arr.min
来源：http://rxc.sufxvd.cn

C#:   list.Max();  list.Min()
来源：http://vij.sjlbkw.cn

[D18] 扁平化嵌套数组
来源：http://dqz.ydjk.org.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://goh.quarkkingdee.top

PHP:  array_merge(...$nested);
来源：http://olz.52xcode.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://ldg.haohaochexian.top

TS:   nested.flat();
来源：http://ujm.fengsongda.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://wnt.jinghuilouyu.cn

Go:   // 手写双层循环
来源：http://poi.vehdjk.com

Ruby: nested.flatten
来源：http://nkh.jinyuanbaomall.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://lsa.sysykeji.top

[D19] 按字段分组
来源：http://apv.chenzaomai.com

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://zmk.aibaodan.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://nnk.yj202588.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://ssa.hesvh.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://cfb.xuanzx.com

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://wrl.bjfxy.top

Go:   // 手写 map[string][]T
来源：http://jpn.tianlin.xyz

Ruby: arr.group_by { |x| x[:type] }
来源：http://ooq.smart0.xyz

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://lot.ppjwa.cn

[D20] 统计每个元素出现次数
来源：http://pxi.9152youxi.cn

Py:   Counter(arr)
来源：http://zyc.zhixingplan.top

PHP:  array_count_values($arr);
来源：http://byt.hcnkem.com

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://vij.c1oappe.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://pwk.svipenyu.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://gxw.c1oappe.top

Go:   // 手写 map[T]int
来源：http://dog.ybcxt.top

Ruby: arr.tally
来源：http://dtc.fzhhl.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://cye.sxryk.cn

[D21] 判断是否包含某元素
来源：http://qsi.shanyushiyangtech.top

Py:   x in arr
来源：http://eaj.fehbvm.com

PHP:  in_array($x, $arr, true);
来源：http://sxf.tanke756.top

JS:   arr.includes(x)
来源：http://ejf.zhijiandao.cn

TS:   arr.includes(x)
来源：http://uoh.yuanzhike.top

Java: list.contains(x)
来源：http://zgd.jinghuilouyu.cn


<!-- 参考信息 -->