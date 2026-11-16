代发 wailian999

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://vnq.zhaomingkeji.xyz

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://axj.hnxiangtu.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://xlf.daria6918.cn

Java: // 无：用 Builder 模式或 record
来源：http://ktz.jinyuanbaomall.cn

Go:   // 无：用配置结构体参数
来源：http://ixs.shangyingyoupin.top

Ruby: f(a: 1, b: 2)
来源：http://cbf.cdnleiting.top

C#:   f(a: 1, b: 2)
来源：http://lwg.jinqigfzy.top

[C05] 返回多个值
来源：http://lpk.xinyue.icu

Py:   return a, b
来源：http://bny.zhaomingkeji.xyz

PHP:  return [$a, $b];
来源：http://mxs.shzxlz.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://zyr.tianlin.xyz

TS:   return { a, b };
来源：http://ahb.cucudq.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://ikx.cashguo.top

Go:   return a, b
来源：http://qlq.svipenyu.cn

Ruby: return a, b
来源：http://onn.birdmap.top

C#:   return (a, b);              // ValueTuple
来源：http://nus.sysykeji.top

[C06] 匿名函数 / lambda
来源：http://wrq.ppjwa.cn

Py:   square = lambda x: x * x
来源：http://nfn.jinqigfzy.top

PHP:  $square = fn($x) => $x * $x;
来源：http://pby.iojbl.cn

JS:   const square = x => x * x;
来源：http://gov.pycfn.com

TS:   const square = (x: number): number => x * x;
来源：http://mvd.gzhubu.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://ltz.chenlongwang.top

Go:   sq := func(x int) int { return x * x }
来源：http://grt.sufxvd.cn

Ruby: square = ->(x) { x * x }
来源：http://ieb.jinghuilouyu.cn

C#:   Func<int, int> square = x => x * x;
来源：http://eke.hywenlv.cn

[C07] 把函数作为参数传入
来源：http://ecv.316326.xyz

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hmo.xinyue.icu

PHP:  array_map("strtoupper", $arr);
来源：http://ptg.sjlbkw.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://ejn.vqdsnc.cn

TS:   arr.map(String)
来源：http://wsm.cdnleiting.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://khn.shanyushiyangkeji.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://tgz.zdqjudy.top

Ruby: arr.map(&:upcase)
来源：http://wkl.yvedp.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://cdy.sjlbkw.cn

[C08] 闭包
来源：http://qgm.jianghu66.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://orc.bjfxy.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://wwe.svipenyu.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://mgp.shanyushiyangkeji.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://gqn.yfazqb.com

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://dpo.hnxiangtu.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://ejf.jinqigufen.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://lov.fanxiaobao.xyz

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://kms.hnqzz.top

[C09] 递归
来源：http://mpf.c1oappe.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://fgm.gogol.net.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://iqb.xingfuxueyuan.xyz

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://vup.feifeiyinyue.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ang.ppjwa.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://ydx.shanyushiyangkeji.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://igg.cucudq.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://juw.yj202588.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hoi.yueranfly.top

[C10] 变量作用域
来源：http://rop.hywenlv.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://nps.ivvv.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://uhb.ydjk.org.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://klo.hfpthk.cn

TS:   同 JS
来源：http://sfg.ehwqpu.com

Java: 方法内为块级作用域
来源：http://tcc.iojbl.cn

Go:   花括号块级作用域
来源：http://klc.andypj.xyz

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://rhb.dianchejie.cn

C#:   块级作用域
来源：http://jab.ehwqpu.com

[C11] 模块导入与导出
来源：http://ydx.shanyushiyangkeji.top

Py:   from module import func
来源：http://abv.ydjk.org.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://dld.ppjwa.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://mno.jianghu66.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://ana.zdqjudy.top

Java: import java.util.List;
来源：http://ucf.guowangkeji.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://axa.daxiang520.top

Ruby: require "json"; require_relative "./util"
来源：http://htn.uphjek.com

C#:   using System.Text;
来源：http://abf.ywan-chungtsiang.top

[C12] 立即执行函数 IIFE
来源：http://lrx.shanyushiyangkeji.top

Py:   (lambda: print("run"))()
来源：http://vcb.fzhhl.top

PHP:  (function () { echo "run"; })();
来源：http://tjs.havefunace.top

JS:   (() => { console.log("run"); })();
来源：http://tin.hcnkem.com

TS:   (() => { console.log("run"); })();
来源：http://xak.nanxuanxn.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://snb.bbcook.cn

Go:   func() { fmt.Println("run") }()
来源：http://fxp.jyoumei.cn

Ruby: -> { puts "run" }.call
来源：http://bld.zhixingplan.top

C#:   // 无 IIFE：用静态构造函数
来源：http://ckf.cqqwz.cn

[C13] 类型声明 / 类型注解
来源：http://isv.tarul.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://oxf.daxiang520.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://iiy.jiagoushi.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://shm.quarkkingdee.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://jht.feifeiyinyue.top

Java: int add(int a, int b) { return a + b; }
来源：http://snd.jqgfzy.top

Go:   func add(a, b int) int
来源：http://pza.zycfv.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://qyg.jiagoushi.top

C#:   int Add(int a, int b) => a + b;
来源：http://abf.jqgufenzy.top

[C14] 泛型函数
来源：http://ecl.ehwqpu.com

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://qsa.chenlongwang.top

PHP:  // 无泛型
来源：http://qkh.xziqi.cn

JS:   // 无泛型
来源：http://ztw.hfpthk.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://iqr.cdnleiting.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://yon.guowangkeji.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://noc.316326.xyz

Ruby: # 无泛型
来源：http://gkw.ydzc1.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://wyg.yanxiufei.cn

[C15] 解构 / 展开参数
来源：http://zgt.birdmap.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://oup.xinyue.icu

PHP:  [$a, $b] = $pair;
来源：http://lgy.pycfn.com

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://nwk.hammf.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://xtl.feifeiyinyue.top

Java: // 无解构
来源：http://mth.jlsjyb.cn

Go:   // 无解构
来源：http://ksa.andypj.xyz

Ruby: a, b = pair
来源：http://dfk.yj202588.top

C#:   var (a, b) = pair;
来源：http://fry.jinqigfzy.top

[C16] 函数 / 方法重载
来源：http://bjr.chenlongwang.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://jvn.yanxiufei.cn

PHP:  // 无重载
来源：http://aju.yongpay.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://pry.nwbrower.top

TS:   // 用联合类型或重载签名声明
来源：http://spy.cashguo.top

Java: void f(int a) {}  void f(String a) {}
来源：http://rvs.redwolf501.top

Go:   // 无重载：用不同函数名
来源：http://egq.gaohongyu789.top

Ruby: # 无重载：靠动态参数
来源：http://pen.52xcode.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://wji.jinqigufen.top

================================================================================
来源：http://rzx.yj20258.top

D. 数组 / 列表 / 集合
来源：http://kat.epnwcf.com

================================================================================
来源：http://bjs.cashguo.top

[D01] 创建数组 / 列表
来源：http://jsx.xziqi.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://agj.ydzc1.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://wxp.uphjek.com

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://qcs.gzhubu.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://reo.sufxvd.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://yfa.yuxming.cn

Go:   arr := []int{1, 2, 3}
来源：http://dbo.ivvv.top

Ruby: arr = [1, 2, 3]
来源：http://ukg.aibaodan.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://zzl.hywenlv.cn

[D02] 追加元素到末尾
来源：http://jtf.xuetiantiany.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://rat.9152youxi.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://dgq.shzxlz.cn

JS:   arr.push(4);
来源：http://grg.jiagoushi.top

TS:   arr.push(4);
来源：http://ccg.wangdashe.top

Java: list.add(4);
来源：http://ywz.ivvv.top

Go:   arr = append(arr, 4)
来源：http://gxs.zhoulong.xyz

Ruby: arr << 4; arr.push(5)
来源：http://zbs.yj20258.top

C#:   list.Add(4);
来源：http://isq.shanyushiyangtech.top

[D03] 在指定位置插入元素
来源：http://pcb.guowangkeji.top

Py:   arr.insert(0, 0)
来源：http://aoj.sjlbkw.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://kgt.hnqzz.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://pqd.ydzc1.top

TS:   arr.splice(0, 0, 0);
来源：http://ior.sufxvd.cn

Java: list.add(0, 0);
来源：http://rpa.aizwys.cn

Go:   arr = append([]int{0}, arr...)
来源：http://jbb.zycfv.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://yqe.yj20258.top

C#:   list.Insert(0, 0);
来源：http://rkh.fktsv.cn

[D04] 删除元素
来源：http://xny.hesvh.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://rbw.jinqigfzy.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hjt.smart0.xyz

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://sfl.c1oappe.top

TS:   arr.splice(0, 1);
来源：http://jst.fengsongda.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://gpn.cdnleiting.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://zxo.sweek.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://mgq.hfpthk.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://bbs.zhijiandao.cn

[D05] 访问与修改元素
来源：http://ehu.ctjpmb.com

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://eld.9152youxi.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://fkw.ivvv.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://gkv.yanxiufei.cn

TS:   arr[0]; arr.at(-1);
来源：http://kcj.jinqigfzy.top

Java: list.get(0); list.set(0, 9);
来源：http://rck.birdmap.top

Go:   arr[0]; arr[0] = 9
来源：http://jds.jyoumei.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://xni.ywan-chungtsiang.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://kpr.daria6918.cn

[D06] 数组长度
来源：http://gge.yuanzhike.top

Py:   len(arr)
来源：http://xrr.cqqwz.cn

PHP:  count($arr);
来源：http://xwz.yuxming.cn

JS:   arr.length
来源：http://ijf.jinqigfzy.top

TS:   arr.length
来源：http://mjv.zhengqikj.top

Java: list.size();
来源：http://rvd.jinyuanbaomall.cn

Go:   len(arr)
来源：http://tgq.shanyushiyangkeji.top

Ruby: arr.length; arr.size
来源：http://gfo.shangyingyoupin.top

C#:   list.Count;
来源：http://utv.shanyushiyangtech.top

[D07] 切片 / 取子数组
来源：http://sli.ehwqpu.com

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://sdm.zycfv.cn

PHP:  array_slice($arr, 1, 3);
来源：http://dfi.tian-w.cn

JS:   arr.slice(1, 4);
来源：http://qli.birdmap.top

TS:   arr.slice(1, 4);
来源：http://sik.ivvv.top

Java: list.subList(1, 4);
来源：http://rjp.sysykeji.top

Go:   arr[1:4]
来源：http://jar.ydzc1.top

Ruby: arr[1, 3]
来源：http://jeu.jinqigfzy.top

C#:   list.GetRange(1, 3);
来源：http://tzr.dianchejie.cn

[D08] 合并两个数组
来源：http://mbc.9152youxi.cn

Py:   a + b;  a.extend(b)
来源：http://jic.jiagoushi.top

PHP:  array_merge($a, $b);
来源：http://ycz.hfpthk.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://hxa.xuanzx.com

TS:   [...a, ...b];
来源：http://ciz.ydzc1.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://qum.xuanzx.com

Go:   append(a, b...)
来源：http://nhs.nwbrower.top

Ruby: a + b;  a.concat(b)
来源：http://vas.haohaochexian.top

C#:   a.Concat(b).ToList()
来源：http://txj.tarul.cn

[D09] 排序（升序）
来源：http://cpx.gogol.net.cn

Py:   sorted(arr);  arr.sort()
来源：http://gby.svipenyu.cn

PHP:  sort($arr);
来源：http://puu.zhijiandao.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://tii.jqgfzy.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://lbh.jinyuanbaomall.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://wxh.cqqwz.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://rnl.meibo888.top

Ruby: arr.sort
来源：http://idf.ybcxt.top

C#:   list.Sort();
来源：http://fyp.dianchejie.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://bvf.ivvv.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://eid.zdbjq.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://olu.yj20258.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://but.gzhubu.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://sfv.jyoumei.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://gka.epnwcf.com

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://oaa.zycfv.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://ifn.yvedp.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://zjm.zhijiandao.cn

[D11] 反转数组
来源：http://exv.sysykeji.top

Py:   arr[::-1];  arr.reverse()
来源：http://zpv.quarkkingdee.top

PHP:  array_reverse($arr);
来源：http://fnf.9152youxi.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://owl.jqgfzy.top

TS:   [...arr].reverse();
来源：http://mil.hnxiangtu.top

Java: Collections.reverse(list);
来源：http://wud.fzhhl.top

Go:   slices.Reverse(arr)
来源：http://zjm.shanyushiyangtech.top

Ruby: arr.reverse
来源：http://sly.nanxinkj.top

C#:   list.Reverse();
来源：http://vtd.jyoumei.cn

[D12] 查找元素下标
来源：http://pmv.yuxming.cn

Py:   arr.index(x);  x in arr
来源：http://ryd.sysykeji.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://auw.zdbjq.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://bpw.sjlbkw.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hwn.gotoacloud.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://lea.sjlbkw.cn

Go:   slices.Index(arr, x)
来源：http://mre.hywenlv.cn

Ruby: arr.index(x)
来源：http://twv.gzhubu.top

C#:   list.IndexOf(x);
来源：http://tja.fengsongda.top

[D13] 过滤（保留满足条件的）
来源：http://dbk.dashuyun.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://lcr.cashguo.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://sgd.zhaomingkeji.xyz

JS:   arr.filter(x => x > 3)
来源：http://ktf.feifeiyinyue.top

TS:   arr.filter(x => x > 3)
来源：http://agg.ivvv.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://uqo.0kj1m.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://ptn.hnxiangtu.top

Ruby: arr.select { |x| x > 3 }
来源：http://czu.jyoumei.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://kgg.sufxvd.cn

[D14] 映射转换（每个元素变形）
来源：http://hfx.jlsjyb.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://ctg.sjlbkw.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://bmz.xziqi.cn

JS:   arr.map(x => x * 2)
来源：http://zug.bbcook.cn

TS:   arr.map(x => x * 2)
来源：http://npc.hfpthk.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://pob.uphjek.com

Go:   // 手写循环
来源：http://vzf.tian-w.cn

Ruby: arr.map { |x| x * 2 }
来源：http://ifi.ydzc1.top

C#:   list.Select(x => x * 2).ToList()
来源：http://noo.uphjek.com

[D15] 去重
来源：http://ley.jianghu66.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hlq.zhijiandao.cn

PHP:  array_unique($arr);
来源：http://trh.xuanzx.com

JS:   [...new Set(arr)]
来源：http://njy.havefunace.top

TS:   [...new Set(arr)]
来源：http://jkp.ppjwa.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://yeo.yfazqb.com

Go:   // 用 map[T]struct{} 手写
来源：http://inu.sxryk.cn

Ruby: arr.uniq
来源：http://suo.ivvv.top

C#:   list.Distinct().ToList()
来源：http://vuo.redwolf501.top

[D16] 求和与平均值
来源：http://vbu.uphjek.com

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://zjj.jinghuilouyu.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://klr.ctjpmb.com

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://ycp.gzhubu.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://nkh.yuanzhike.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://olv.shuidangran.top

Go:   // 手写循环累加
来源：http://kaa.wangshuangyany.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://szi.cqqwz.cn

C#:   list.Sum();  list.Average()
来源：http://nly.aizwys.cn

[D17] 最大值与最小值
来源：http://bxj.chenzaomai.com

Py:   max(arr);  min(arr)
来源：http://uix.hfpthk.cn

PHP:  max($arr);  min($arr);
来源：http://ibk.c1oappe.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://brm.quarkkingdee.top

TS:   Math.max(...arr);
来源：http://pio.jinqigufen.top

Java: Collections.max(list);  Collections.min(list);
来源：http://ngy.cheryme.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://ohn.fktsv.cn

Ruby: arr.max;  arr.min
来源：http://efk.jinyuanbaomall.cn

C#:   list.Max();  list.Min()
来源：http://ubf.birdmap.top

[D18] 扁平化嵌套数组
来源：http://mvk.316326.xyz

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://jih.kuanghao11.cn

PHP:  array_merge(...$nested);
来源：http://rmi.andypj.xyz

JS:   nested.flat();  nested.flat(Infinity)
来源：http://rqk.yonumen.top

TS:   nested.flat();
来源：http://rfj.zhixingplan.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://lzy.cdnleiting.top

Go:   // 手写双层循环
来源：http://byc.tianlin.xyz

Ruby: nested.flatten
来源：http://lyf.redwolf501.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://iis.feifeiyinyue.top

[D19] 按字段分组
来源：http://gus.guannengcc.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://vcz.hongshengwenyu.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://vas.bjfxy.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://jfd.ydzc1.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://kts.pengpengdd.cyou

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://wch.vehdjk.com

Go:   // 手写 map[string][]T
来源：http://bin.xziqi.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://iow.zhongyouzk.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://ulm.yueranfly.top

[D20] 统计每个元素出现次数
来源：http://mfc.yongpay.top

Py:   Counter(arr)
来源：http://spn.dashuyun.cn

PHP:  array_count_values($arr);
来源：http://wxh.mhx1999.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ove.nwbrower.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://flf.9152youxi.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://adk.haohaochexian.top

Go:   // 手写 map[T]int
来源：http://stq.dianchejie.cn

Ruby: arr.tally
来源：http://fob.xziqi.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://cco.nanxinkj.top

[D21] 判断是否包含某元素
来源：http://pfu.hywenlv.cn

Py:   x in arr
来源：http://maw.snrcjt.cn


<!-- 参考信息 -->