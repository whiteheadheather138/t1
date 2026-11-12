代发 wailian999

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://wec.ctjpmb.com

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://uvb.yvedp.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://det.yuanzhike.top

Java: // 无：用 Builder 模式或 record
来源：http://alb.andypj.xyz

Go:   // 无：用配置结构体参数
来源：http://edb.shanyushiyangkeji.top

Ruby: f(a: 1, b: 2)
来源：http://mzn.jinqigfzy.top

C#:   f(a: 1, b: 2)
来源：http://mwr.xuetiantiany.cn

[C05] 返回多个值
来源：http://ytx.52xcode.cn

Py:   return a, b
来源：http://yag.sxryk.cn

PHP:  return [$a, $b];
来源：http://gce.guannengcc.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://iks.yonumen.top

TS:   return { a, b };
来源：http://xyg.zycfv.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://awl.0kj1m.cn

Go:   return a, b
来源：http://tcf.wangdashe.top

Ruby: return a, b
来源：http://zsq.zhijiandao.cn

C#:   return (a, b);              // ValueTuple
来源：http://now.cqqwz.cn

[C06] 匿名函数 / lambda
来源：http://god.zycfv.cn

Py:   square = lambda x: x * x
来源：http://qhg.jinqigufen.top

PHP:  $square = fn($x) => $x * $x;
来源：http://jzy.shanyushiyangtech.top

JS:   const square = x => x * x;
来源：http://uzx.hysaishi.cn

TS:   const square = (x: number): number => x * x;
来源：http://ugu.daria6918.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://lxs.hammf.cn

Go:   sq := func(x int) int { return x * x }
来源：http://aqy.daxiang520.top

Ruby: square = ->(x) { x * x }
来源：http://gwb.zdbjq.cn

C#:   Func<int, int> square = x => x * x;
来源：http://igs.yanxiufei.cn

[C07] 把函数作为参数传入
来源：http://obz.yangfankeji.com

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://gms.shanyushiyangkeji.top

PHP:  array_map("strtoupper", $arr);
来源：http://jbj.ybcxt.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://phw.tarul.cn

TS:   arr.map(String)
来源：http://dln.zdqjudy.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://sad.ybcxt.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://rnf.hammf.cn

Ruby: arr.map(&:upcase)
来源：http://gpu.fehbvm.com

C#:   arr.Select(s => s.ToUpper())
来源：http://kak.pycfn.com

[C08] 闭包
来源：http://jbi.jinyuanbaomall.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://tja.hcnkem.com

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://ypb.hesvh.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://qew.guowangkeji.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://ejf.kuanghao11.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://xto.0kj1m.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://jya.hnxiangtu.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://uut.wangdashe.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://rjk.vehdjk.com

[C09] 递归
来源：http://ems.xingfuxueyuan.xyz

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://elp.sufxvd.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://uox.zhiwuduotai.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://rxr.sxryk.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ybj.sjlbkw.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hdk.vqdsnc.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://xby.jqgfzy.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://suq.shanyushiyangkeji.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://dtq.dashuyun.cn

[C10] 变量作用域
来源：http://ual.daxiang520.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://jqm.birdmap.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://lvm.gzhubu.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://jzi.jinyuanbaomall.cn

TS:   同 JS
来源：http://nsm.0kj1m.cn

Java: 方法内为块级作用域
来源：http://ooh.cqqwz.cn

Go:   花括号块级作用域
来源：http://kjp.yvedp.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://oqz.tian-w.cn

C#:   块级作用域
来源：http://nlc.c1oappe.top

[C11] 模块导入与导出
来源：http://tqe.jqgufenzy.top

Py:   from module import func
来源：http://wiz.andypj.xyz

PHP:  require "file.php";  或 use App\Service;
来源：http://cwf.ivvv.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://csv.ydzc1.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://cgd.xingfuxueyuan.xyz

Java: import java.util.List;
来源：http://ffx.bbcook.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://wwd.aibaodan.cn

Ruby: require "json"; require_relative "./util"
来源：http://bat.jlsjyb.cn

C#:   using System.Text;
来源：http://kyi.bjfxy.top

[C12] 立即执行函数 IIFE
来源：http://wet.vqdsnc.cn

Py:   (lambda: print("run"))()
来源：http://mzp.sysykeji.top

PHP:  (function () { echo "run"; })();
来源：http://qus.hesvh.cn

JS:   (() => { console.log("run"); })();
来源：http://bow.dianchejie.cn

TS:   (() => { console.log("run"); })();
来源：http://ovx.guannengcc.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hsr.yongpay.top

Go:   func() { fmt.Println("run") }()
来源：http://dzd.yuanzhike.top

Ruby: -> { puts "run" }.call
来源：http://bfv.mhx1999.top

C#:   // 无 IIFE：用静态构造函数
来源：http://zyx.fehbvm.com

[C13] 类型声明 / 类型注解
来源：http://iee.hesvh.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://vas.guannengcc.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://qrj.yongpay.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://luh.vqdsnc.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://bmj.daria6918.cn

Java: int add(int a, int b) { return a + b; }
来源：http://tfa.tarul.cn

Go:   func add(a, b int) int
来源：http://dmi.0kj1m.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://rkb.ehwqpu.com

C#:   int Add(int a, int b) => a + b;
来源：http://fgj.jinqigfzy.top

[C14] 泛型函数
来源：http://ght.guannengcc.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://czj.feifeiyinyue.top

PHP:  // 无泛型
来源：http://nhn.nanxinkj.top

JS:   // 无泛型
来源：http://tpe.hongshengwenyu.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://enn.kuanghao11.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://fqt.guowangkeji.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://ffe.nanxinkj.top

Ruby: # 无泛型
来源：http://yon.vqdsnc.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://mgh.fehbvm.com

[C15] 解构 / 展开参数
来源：http://oio.yangfankeji.com

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://nxo.ehwqpu.com

PHP:  [$a, $b] = $pair;
来源：http://nlr.daxiang520.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://sxi.svipenyu.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://gea.ydzc1.top

Java: // 无解构
来源：http://ucw.gaohongyu789.top

Go:   // 无解构
来源：http://iat.shuidangran.top

Ruby: a, b = pair
来源：http://tcu.xingfuxueyuan.xyz

C#:   var (a, b) = pair;
来源：http://hzj.yvedp.cn

[C16] 函数 / 方法重载
来源：http://gcv.kuanghao11.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://bcb.yueranfly.top

PHP:  // 无重载
来源：http://zpb.pycfn.com

JS:   // 无重载：靠 arguments.length 分支
来源：http://uzz.yonumen.top

TS:   // 用联合类型或重载签名声明
来源：http://ifo.meibo888.top

Java: void f(int a) {}  void f(String a) {}
来源：http://yut.dianchejie.cn

Go:   // 无重载：用不同函数名
来源：http://fmi.andypj.xyz

Ruby: # 无重载：靠动态参数
来源：http://ybc.kuanghao11.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://hjy.hammf.cn

================================================================================
来源：http://fur.yueranfly.top

D. 数组 / 列表 / 集合
来源：http://knr.yuxming.cn

================================================================================
来源：http://uog.yueranfly.top

[D01] 创建数组 / 列表
来源：http://vtl.cqqwz.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://ypd.fehbvm.com

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://alt.cheryme.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://wgq.dianchejie.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://wvl.hammf.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://uvx.andypj.xyz

Go:   arr := []int{1, 2, 3}
来源：http://skj.yangfankeji.com

Ruby: arr = [1, 2, 3]
来源：http://ztt.jiagoushi.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://she.xylfe.cn

[D02] 追加元素到末尾
来源：http://cif.zdbjq.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://rjo.uphjek.com

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://yif.svipenyu.cn

JS:   arr.push(4);
来源：http://iwm.ydjk.org.cn

TS:   arr.push(4);
来源：http://mdv.quarkkingdee.top

Java: list.add(4);
来源：http://anr.ehwqpu.com

Go:   arr = append(arr, 4)
来源：http://rhc.jinqigfzy.top

Ruby: arr << 4; arr.push(5)
来源：http://jko.jqgfzy.top

C#:   list.Add(4);
来源：http://sng.ppjwa.cn

[D03] 在指定位置插入元素
来源：http://rja.zhiwuduotai.top

Py:   arr.insert(0, 0)
来源：http://mbn.zhoulong.xyz

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hwl.yonumen.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://tdp.haohaochexian.top

TS:   arr.splice(0, 0, 0);
来源：http://bcb.hongshengwenyu.top

Java: list.add(0, 0);
来源：http://adn.aibaodan.cn

Go:   arr = append([]int{0}, arr...)
来源：http://fwy.tian-w.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://kol.epnwcf.com

C#:   list.Insert(0, 0);
来源：http://bkg.pengpengdd.cyou

[D04] 删除元素
来源：http://cwf.andypj.xyz

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://cmg.guowangkeji.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://tcp.chenzaomai.com

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://xfd.zdqjudy.top

TS:   arr.splice(0, 1);
来源：http://spt.svipenyu.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://lth.xziqi.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://uho.zhixingplan.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://bhl.xuetiantiany.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://bdo.iojbl.cn

[D05] 访问与修改元素
来源：http://zfr.sweek.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://tmz.redwolf501.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://crf.chenjidiqi.icu

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://gqq.zhengqikj.top

TS:   arr[0]; arr.at(-1);
来源：http://ctz.sufxvd.cn

Java: list.get(0); list.set(0, 9);
来源：http://psa.meibo888.top

Go:   arr[0]; arr[0] = 9
来源：http://ioq.shuidangran.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://phn.bjfxy.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://oiq.vqdsnc.cn

[D06] 数组长度
来源：http://jye.zhiwuduotai.top

Py:   len(arr)
来源：http://ryu.sweek.top

PHP:  count($arr);
来源：http://jeb.chenlongwang.top

JS:   arr.length
来源：http://xzd.epnwcf.com

TS:   arr.length
来源：http://gtj.ehwqpu.com

Java: list.size();
来源：http://qoj.0kj1m.cn

Go:   len(arr)
来源：http://lof.hysaishi.cn

Ruby: arr.length; arr.size
来源：http://omw.daxiang520.top

C#:   list.Count;
来源：http://wyt.jinqigfzy.top

[D07] 切片 / 取子数组
来源：http://dfi.bjfxy.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://scl.nanxuanxn.top

PHP:  array_slice($arr, 1, 3);
来源：http://xzj.yangfankeji.com

JS:   arr.slice(1, 4);
来源：http://qbi.sysykeji.top

TS:   arr.slice(1, 4);
来源：http://wyb.gotoacloud.top

Java: list.subList(1, 4);
来源：http://ccj.jinqigfzy.top

Go:   arr[1:4]
来源：http://wpu.yj20258888.top

Ruby: arr[1, 3]
来源：http://fdb.xylfe.cn

C#:   list.GetRange(1, 3);
来源：http://aus.pycfn.com

[D08] 合并两个数组
来源：http://pmi.sxryk.cn

Py:   a + b;  a.extend(b)
来源：http://pfw.hesvh.cn

PHP:  array_merge($a, $b);
来源：http://wxc.zhengqikj.top

JS:   [...a, ...b];  a.concat(b);
来源：http://lws.9152youxi.cn

TS:   [...a, ...b];
来源：http://nql.xuetiantiany.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://jcc.cucudq.cn

Go:   append(a, b...)
来源：http://joa.ehwqpu.com

Ruby: a + b;  a.concat(b)
来源：http://ehg.jinghuilouyu.cn

C#:   a.Concat(b).ToList()
来源：http://evr.dashuyun.cn

[D09] 排序（升序）
来源：http://yuk.ybcxt.top

Py:   sorted(arr);  arr.sort()
来源：http://obz.jianghu66.top

PHP:  sort($arr);
来源：http://saw.hfpthk.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://tqu.cqqwz.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://haa.yuxming.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://njg.hnxiangtu.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://bll.bjfxy.top

Ruby: arr.sort
来源：http://zbu.gaohongyu789.top

C#:   list.Sort();
来源：http://ukg.daxiang520.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://oxz.hcnkem.com

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://xfk.iojbl.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://rna.xziqi.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://qoe.nanxinkj.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://cyq.sxryk.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://job.xinyue.icu

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://pce.dashuyun.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://ejy.fengsongda.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://uss.jqgufenzy.top

[D11] 反转数组
来源：http://bko.zhaomingkeji.xyz

Py:   arr[::-1];  arr.reverse()
来源：http://lxl.fanxiaobao.xyz

PHP:  array_reverse($arr);
来源：http://obj.fengsongda.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hks.chenzaomai.com

TS:   [...arr].reverse();
来源：http://jkz.iojbl.cn

Java: Collections.reverse(list);
来源：http://mqq.tarul.cn

Go:   slices.Reverse(arr)
来源：http://ayw.wangdashe.top

Ruby: arr.reverse
来源：http://dzl.vehdjk.com

C#:   list.Reverse();
来源：http://ymp.yvedp.cn

[D12] 查找元素下标
来源：http://ege.yvedp.cn

Py:   arr.index(x);  x in arr
来源：http://xev.cucudq.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://jnj.xingfuxueyuan.xyz

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://cfw.hesvh.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hrb.daxiang520.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://ufh.yonumen.top

Go:   slices.Index(arr, x)
来源：http://pmk.havefunace.top

Ruby: arr.index(x)
来源：http://mrv.xingfuxueyuan.xyz

C#:   list.IndexOf(x);
来源：http://uve.ctjpmb.com

[D13] 过滤（保留满足条件的）
来源：http://tph.shangyingyoupin.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://cap.nanxinkj.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://fuf.cashguo.top

JS:   arr.filter(x => x > 3)
来源：http://eua.cashguo.top

TS:   arr.filter(x => x > 3)
来源：http://jam.fengsongda.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://ige.xuetiantiany.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://rkq.xziqi.cn

Ruby: arr.select { |x| x > 3 }
来源：http://rnk.ywan-chungtsiang.top

C#:   list.Where(x => x > 3).ToList()
来源：http://xsx.chenlongwang.top

[D14] 映射转换（每个元素变形）
来源：http://zzz.birdmap.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://vgr.yonumen.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://mii.pycfn.com

JS:   arr.map(x => x * 2)
来源：http://okg.zhixingplan.top

TS:   arr.map(x => x * 2)
来源：http://had.hesvh.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://ijf.wangshuangyany.cn

Go:   // 手写循环
来源：http://ktw.ivvv.top

Ruby: arr.map { |x| x * 2 }
来源：http://oym.52xcode.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://ltu.jyoumei.cn

[D15] 去重
来源：http://swl.mhx1999.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://eqm.kuanghao11.cn

PHP:  array_unique($arr);
来源：http://hzx.ybcxt.top

JS:   [...new Set(arr)]
来源：http://ppm.sxryk.cn

TS:   [...new Set(arr)]
来源：http://uvv.vehdjk.com

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://wet.9152youxi.cn

Go:   // 用 map[T]struct{} 手写
来源：http://krt.yfazqb.com

Ruby: arr.uniq
来源：http://lmz.tianlin.xyz

C#:   list.Distinct().ToList()
来源：http://dpc.hongshengwenyu.top

[D16] 求和与平均值
来源：http://qbz.cucudq.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://zuh.cdnleiting.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://oyi.havefunace.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://iba.ydjk.org.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://fdw.daxiang520.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://nli.tarul.cn

Go:   // 手写循环累加
来源：http://jfx.dashuyun.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://zgy.tian-w.cn

C#:   list.Sum();  list.Average()
来源：http://arm.jinghuilouyu.cn

[D17] 最大值与最小值
来源：http://gbd.zdqjudy.top

Py:   max(arr);  min(arr)
来源：http://isd.yonumen.top

PHP:  max($arr);  min($arr);
来源：http://kjp.gotoacloud.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://ggm.yonumen.top

TS:   Math.max(...arr);
来源：http://slb.vehdjk.com

Java: Collections.max(list);  Collections.min(list);
来源：http://fod.xziqi.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://zgy.zycfv.cn

Ruby: arr.max;  arr.min
来源：http://gdh.fengsongda.top

C#:   list.Max();  list.Min()
来源：http://uzp.hammf.cn

[D18] 扁平化嵌套数组
来源：http://pxy.aizwys.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hdm.yfazqb.com

PHP:  array_merge(...$nested);
来源：http://tos.yj202588.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://wrt.hesvh.cn

TS:   nested.flat();
来源：http://hgw.ivvv.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://rii.fehbvm.com

Go:   // 手写双层循环
来源：http://jfr.tianlin.xyz

Ruby: nested.flatten
来源：http://kkg.yj20258.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://jif.fktsv.cn

[D19] 按字段分组
来源：http://usv.zhongyouzk.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://haw.yj20258.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://fiz.jqgfzy.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://lpe.yj202588.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://zmr.hywenlv.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://cik.nanxuanxn.top

Go:   // 手写 map[string][]T
来源：http://qzw.fengsongda.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://cxp.jyoumei.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://jfh.cashguo.top

[D20] 统计每个元素出现次数
来源：http://lku.xingfuxueyuan.xyz

Py:   Counter(arr)
来源：http://mbr.tianlin.xyz

PHP:  array_count_values($arr);
来源：http://mhh.ivvv.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://iol.zhengqikj.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://xuk.ehwqpu.com

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://gqp.guannengcc.top

Go:   // 手写 map[T]int
来源：http://xfp.guowangkeji.top

Ruby: arr.tally
来源：http://chi.quarkkingdee.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://trt.iojbl.cn

[D21] 判断是否包含某元素
来源：http://jxs.cheryme.top

Py:   x in arr
来源：http://vkb.tanke756.top


<!-- 参考信息 -->