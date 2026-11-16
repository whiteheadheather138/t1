代发 wailian999

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://sko.yanxiufei.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://xrf.xziqi.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://gea.hnqzz.top

Java: // 无：用 Builder 模式或 record
来源：http://poc.yuxming.cn

Go:   // 无：用配置结构体参数
来源：http://nga.xuetiantiany.cn

Ruby: f(a: 1, b: 2)
来源：http://rgx.shangyingyoupin.top

C#:   f(a: 1, b: 2)
来源：http://fzn.zhijiandao.cn

[C05] 返回多个值
来源：http://rfo.tanke756.top

Py:   return a, b
来源：http://wdo.vqdsnc.cn

PHP:  return [$a, $b];
来源：http://nxb.gogol.net.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://lfg.cucudq.cn

TS:   return { a, b };
来源：http://rwx.nwbrower.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://saq.guannengcc.top

Go:   return a, b
来源：http://fny.havefunace.top

Ruby: return a, b
来源：http://cxc.dianchejie.cn

C#:   return (a, b);              // ValueTuple
来源：http://jmz.havefunace.top

[C06] 匿名函数 / lambda
来源：http://mxa.shangyingyoupin.top

Py:   square = lambda x: x * x
来源：http://hhg.cdnleiting.top

PHP:  $square = fn($x) => $x * $x;
来源：http://scs.sjlbkw.cn

JS:   const square = x => x * x;
来源：http://rac.epnwcf.com

TS:   const square = (x: number): number => x * x;
来源：http://thb.xuetiantiany.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://lxx.snrcjt.cn

Go:   sq := func(x int) int { return x * x }
来源：http://reo.iojbl.cn

Ruby: square = ->(x) { x * x }
来源：http://mfu.shanyushiyangtech.top

C#:   Func<int, int> square = x => x * x;
来源：http://gtc.yuanzhike.top

[C07] 把函数作为参数传入
来源：http://iml.sweek.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://xgp.nwbrower.top

PHP:  array_map("strtoupper", $arr);
来源：http://bqi.zdqjudy.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://puq.yj20258888.top

TS:   arr.map(String)
来源：http://byk.feifeiyinyue.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://itc.52xcode.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://kvp.jlsjyb.cn

Ruby: arr.map(&:upcase)
来源：http://cjl.9152youxi.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://eaj.quarkkingdee.top

[C08] 闭包
来源：http://pko.sysykeji.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://fvn.cashguo.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://dlm.sweek.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://tqh.xinyue.icu

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://wnv.zhijiandao.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://kuy.nwbrower.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://uem.dianchejie.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://svl.bbcook.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://rme.hammf.cn

[C09] 递归
来源：http://vsm.shzxlz.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://lcg.yj20258888.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://bqb.shanyushiyangkeji.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ove.yuxming.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://qrx.xuanzx.com

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://ase.hysaishi.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://zql.yueranfly.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://vxh.aibaodan.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://mcb.chenzaomai.com

[C10] 变量作用域
来源：http://uxd.yueranfly.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://fpf.jinqigfzy.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hkd.ywan-chungtsiang.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://ymz.chenlongwang.top

TS:   同 JS
来源：http://tnx.chenzaomai.com

Java: 方法内为块级作用域
来源：http://mfg.guowangkeji.top

Go:   花括号块级作用域
来源：http://jos.guowangkeji.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://erj.yvedp.cn

C#:   块级作用域
来源：http://zpb.yvedp.cn

[C11] 模块导入与导出
来源：http://lya.ppjwa.cn

Py:   from module import func
来源：http://mea.zhixingplan.top

PHP:  require "file.php";  或 use App\Service;
来源：http://zkw.shanyushiyangtech.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://hqd.xziqi.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://lmw.shangyingyoupin.top

Java: import java.util.List;
来源：http://vbo.zycfv.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://lix.quarkkingdee.top

Ruby: require "json"; require_relative "./util"
来源：http://toh.xinyue.icu

C#:   using System.Text;
来源：http://nsg.sweek.top

[C12] 立即执行函数 IIFE
来源：http://dxj.fanxiaobao.xyz

Py:   (lambda: print("run"))()
来源：http://bfr.9152youxi.cn

PHP:  (function () { echo "run"; })();
来源：http://oar.chenzaomai.com

JS:   (() => { console.log("run"); })();
来源：http://bvp.yvedp.cn

TS:   (() => { console.log("run"); })();
来源：http://hvl.c1oappe.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://evj.ctjpmb.com

Go:   func() { fmt.Println("run") }()
来源：http://spi.yj20258.top

Ruby: -> { puts "run" }.call
来源：http://mll.hfpthk.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://wdi.sufxvd.cn

[C13] 类型声明 / 类型注解
来源：http://mcs.havefunace.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://ggm.tarul.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://cfz.chenlongwang.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://feg.sjlbkw.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wwf.xingfuxueyuan.xyz

Java: int add(int a, int b) { return a + b; }
来源：http://dma.xziqi.cn

Go:   func add(a, b int) int
来源：http://ndq.bjfxy.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://pcb.jinghuilouyu.cn

C#:   int Add(int a, int b) => a + b;
来源：http://ucv.shanyushiyangtech.top

[C14] 泛型函数
来源：http://dnp.hammf.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://nlq.ybcxt.top

PHP:  // 无泛型
来源：http://bfj.hysaishi.cn

JS:   // 无泛型
来源：http://ihw.xinyue.icu

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://kvo.quarkkingdee.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://day.tarul.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://ssm.yj20258888.top

Ruby: # 无泛型
来源：http://mql.hongshengwenyu.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://syd.andypj.xyz

[C15] 解构 / 展开参数
来源：http://qfq.tanke756.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://ywy.bjfxy.top

PHP:  [$a, $b] = $pair;
来源：http://lpe.wangshuangyany.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://oha.hnxiangtu.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://whs.zhongyouzk.top

Java: // 无解构
来源：http://wrc.yangfankeji.com

Go:   // 无解构
来源：http://dql.nwbrower.top

Ruby: a, b = pair
来源：http://ped.ydzc1.top

C#:   var (a, b) = pair;
来源：http://fls.c1oappe.top

[C16] 函数 / 方法重载
来源：http://lqx.xziqi.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://wvw.dashuyun.cn

PHP:  // 无重载
来源：http://vrv.cheryme.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://mtd.chenjidiqi.icu

TS:   // 用联合类型或重载签名声明
来源：http://pgc.316326.xyz

Java: void f(int a) {}  void f(String a) {}
来源：http://tae.wangshuangyany.cn

Go:   // 无重载：用不同函数名
来源：http://srr.gzhubu.top

Ruby: # 无重载：靠动态参数
来源：http://cxz.zhiwuduotai.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://wgv.jlsjyb.cn

================================================================================
来源：http://hdl.svipenyu.cn

D. 数组 / 列表 / 集合
来源：http://liz.tarul.cn

================================================================================
来源：http://eca.haohaochexian.top

[D01] 创建数组 / 列表
来源：http://non.jianghu66.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://ndx.birdmap.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://kny.bbcook.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://bml.xziqi.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://zsb.gzhubu.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://rjm.tian-w.cn

Go:   arr := []int{1, 2, 3}
来源：http://ydf.hywenlv.cn

Ruby: arr = [1, 2, 3]
来源：http://udb.ydjk.org.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://mgx.jinyuanbaomall.cn

[D02] 追加元素到末尾
来源：http://aub.guowangkeji.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://tmk.jinqigfzy.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://qrb.316326.xyz

JS:   arr.push(4);
来源：http://vki.hfpthk.cn

TS:   arr.push(4);
来源：http://bpx.c1oappe.top

Java: list.add(4);
来源：http://ztl.chenzaomai.com

Go:   arr = append(arr, 4)
来源：http://gib.zdqjudy.top

Ruby: arr << 4; arr.push(5)
来源：http://yot.sysykeji.top

C#:   list.Add(4);
来源：http://zwr.zdbjq.cn

[D03] 在指定位置插入元素
来源：http://hzh.guannengcc.top

Py:   arr.insert(0, 0)
来源：http://ndj.shanyushiyangtech.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://xsn.0kj1m.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://dzf.birdmap.top

TS:   arr.splice(0, 0, 0);
来源：http://wxu.zhoulong.xyz

Java: list.add(0, 0);
来源：http://qrc.gotoacloud.top

Go:   arr = append([]int{0}, arr...)
来源：http://tsl.guowangkeji.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://ake.yuxming.cn

C#:   list.Insert(0, 0);
来源：http://spd.nanxuanxn.top

[D04] 删除元素
来源：http://qan.tian-w.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://qcr.hnqzz.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://xfl.yuanzhike.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hvy.birdmap.top

TS:   arr.splice(0, 1);
来源：http://brk.hnqzz.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://acd.wangshuangyany.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://llj.xziqi.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://nrr.shzxlz.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://fwu.smart0.xyz

[D05] 访问与修改元素
来源：http://edb.tarul.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://gcc.0kj1m.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://rke.shanyushiyangkeji.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://xll.gogol.net.cn

TS:   arr[0]; arr.at(-1);
来源：http://gwi.pycfn.com

Java: list.get(0); list.set(0, 9);
来源：http://coz.xuetiantiany.cn

Go:   arr[0]; arr[0] = 9
来源：http://otf.wangshuangyany.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://xbn.zhaomingkeji.xyz

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hqg.hnxiangtu.top

[D06] 数组长度
来源：http://zox.shanyushiyangkeji.top

Py:   len(arr)
来源：http://qmq.yonumen.top

PHP:  count($arr);
来源：http://lat.hesvh.cn

JS:   arr.length
来源：http://goz.daxiang520.top

TS:   arr.length
来源：http://bkw.wangdashe.top

Java: list.size();
来源：http://ldf.chenjidiqi.icu

Go:   len(arr)
来源：http://rzp.birdmap.top

Ruby: arr.length; arr.size
来源：http://ssk.jyoumei.cn

C#:   list.Count;
来源：http://dpn.yj20258888.top

[D07] 切片 / 取子数组
来源：http://emv.mhx1999.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://tlh.yonumen.top

PHP:  array_slice($arr, 1, 3);
来源：http://atq.yj20258888.top

JS:   arr.slice(1, 4);
来源：http://hhc.yuxming.cn

TS:   arr.slice(1, 4);
来源：http://xrn.yj20258.top

Java: list.subList(1, 4);
来源：http://mun.gogol.net.cn

Go:   arr[1:4]
来源：http://hvm.yueranfly.top

Ruby: arr[1, 3]
来源：http://juq.jiagoushi.top

C#:   list.GetRange(1, 3);
来源：http://szg.hnxiangtu.top

[D08] 合并两个数组
来源：http://fxq.aibaodan.cn

Py:   a + b;  a.extend(b)
来源：http://tmm.xingfuxueyuan.xyz

PHP:  array_merge($a, $b);
来源：http://koa.bjfxy.top

JS:   [...a, ...b];  a.concat(b);
来源：http://yxf.hongshengwenyu.top

TS:   [...a, ...b];
来源：http://nzi.havefunace.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://npi.bjfxy.top

Go:   append(a, b...)
来源：http://uwu.zdqjudy.top

Ruby: a + b;  a.concat(b)
来源：http://oku.yanxiufei.cn

C#:   a.Concat(b).ToList()
来源：http://tus.hcnkem.com

[D09] 排序（升序）
来源：http://onp.xuetiantiany.cn

Py:   sorted(arr);  arr.sort()
来源：http://oob.shuidangran.top

PHP:  sort($arr);
来源：http://odu.jinqigufen.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://fsq.jyoumei.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://raj.yuanzhike.top

Java: Collections.sort(list);  list.sort(null);
来源：http://nui.jinyuanbaomall.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://aaw.xylfe.cn

Ruby: arr.sort
来源：http://chg.pycfn.com

C#:   list.Sort();
来源：http://kme.bbcook.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://swa.chenjidiqi.icu

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://ezw.ivvv.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://bon.jlsjyb.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://fxe.fehbvm.com

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://uiy.kuanghao11.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://arm.tianlin.xyz

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://tfz.fengsongda.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://nzj.hesvh.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://lkn.zhaomingkeji.xyz

[D11] 反转数组
来源：http://heu.jiagoushi.top

Py:   arr[::-1];  arr.reverse()
来源：http://ujg.yvedp.cn

PHP:  array_reverse($arr);
来源：http://kac.guannengcc.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://vpn.birdmap.top

TS:   [...arr].reverse();
来源：http://tgi.quarkkingdee.top

Java: Collections.reverse(list);
来源：http://ygf.pycfn.com

Go:   slices.Reverse(arr)
来源：http://enk.52xcode.cn

Ruby: arr.reverse
来源：http://hbn.dashuyun.cn

C#:   list.Reverse();
来源：http://arr.zhaomingkeji.xyz

[D12] 查找元素下标
来源：http://sxl.hammf.cn

Py:   arr.index(x);  x in arr
来源：http://xed.havefunace.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://xpx.tarul.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://nzi.xinyue.icu

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://qak.pengpengdd.cyou

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://rsu.yonumen.top

Go:   slices.Index(arr, x)
来源：http://nfw.ctjpmb.com

Ruby: arr.index(x)
来源：http://dzz.shanyushiyangkeji.top

C#:   list.IndexOf(x);
来源：http://hwd.smart0.xyz

[D13] 过滤（保留满足条件的）
来源：http://cly.ctjpmb.com

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://cco.guowangkeji.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hix.yongpay.top

JS:   arr.filter(x => x > 3)
来源：http://kro.snrcjt.cn

TS:   arr.filter(x => x > 3)
来源：http://zbz.sufxvd.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://jlq.fktsv.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://oys.gaohongyu789.top

Ruby: arr.select { |x| x > 3 }
来源：http://pla.fzhhl.top

C#:   list.Where(x => x > 3).ToList()
来源：http://llq.birdmap.top

[D14] 映射转换（每个元素变形）
来源：http://gwu.andypj.xyz

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://wxr.xylfe.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://jbe.mhx1999.top

JS:   arr.map(x => x * 2)
来源：http://lxh.ydzc1.top

TS:   arr.map(x => x * 2)
来源：http://sak.yfazqb.com

Java: list.stream().map(x -> x * 2).toList()
来源：http://dng.mhx1999.top

Go:   // 手写循环
来源：http://vfi.zycfv.cn

Ruby: arr.map { |x| x * 2 }
来源：http://jcv.zhiwuduotai.top

C#:   list.Select(x => x * 2).ToList()
来源：http://jvq.xingfuxueyuan.xyz

[D15] 去重
来源：http://mvh.snrcjt.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://bxl.meibo888.top

PHP:  array_unique($arr);
来源：http://dzy.hysaishi.cn

JS:   [...new Set(arr)]
来源：http://fue.tianlin.xyz

TS:   [...new Set(arr)]
来源：http://bbz.ydzc1.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://tkg.yj20258.top

Go:   // 用 map[T]struct{} 手写
来源：http://pmh.tarul.cn

Ruby: arr.uniq
来源：http://nwc.yangfankeji.com

C#:   list.Distinct().ToList()
来源：http://mbq.havefunace.top

[D16] 求和与平均值
来源：http://oqz.xylfe.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://wgm.zhiwuduotai.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://uhe.yangfankeji.com

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://qin.gotoacloud.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://wjv.jqgufenzy.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://urw.sufxvd.cn

Go:   // 手写循环累加
来源：http://wzx.cashguo.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://szn.andypj.xyz

C#:   list.Sum();  list.Average()
来源：http://tcw.ehwqpu.com

[D17] 最大值与最小值
来源：http://cye.wangshuangyany.cn

Py:   max(arr);  min(arr)
来源：http://yve.9152youxi.cn

PHP:  max($arr);  min($arr);
来源：http://ixl.chenlongwang.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://mjg.dashuyun.cn

TS:   Math.max(...arr);
来源：http://rjt.dashuyun.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://dom.cdnleiting.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://gbx.0kj1m.cn

Ruby: arr.max;  arr.min
来源：http://orq.gogol.net.cn

C#:   list.Max();  list.Min()
来源：http://gzr.sxryk.cn

[D18] 扁平化嵌套数组
来源：http://lwz.ydzc1.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://rkc.xuanzx.com

PHP:  array_merge(...$nested);
来源：http://twz.quarkkingdee.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://cij.daria6918.cn

TS:   nested.flat();
来源：http://eea.jlsjyb.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://qfg.jyoumei.cn

Go:   // 手写双层循环
来源：http://eug.ehwqpu.com

Ruby: nested.flatten
来源：http://mih.sjlbkw.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://gsd.gogol.net.cn

[D19] 按字段分组
来源：http://zhf.haohaochexian.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://mft.sufxvd.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://wfe.shanyushiyangtech.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://uzc.fanxiaobao.xyz

TS:   Object.groupBy(arr, x => x.type)
来源：http://bzk.sufxvd.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://kgz.sweek.top

Go:   // 手写 map[string][]T
来源：http://day.dashuyun.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://ctc.hywenlv.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://thf.tarul.cn

[D20] 统计每个元素出现次数
来源：http://rkf.yanxiufei.cn

Py:   Counter(arr)
来源：http://uuj.jianghu66.top

PHP:  array_count_values($arr);
来源：http://lmo.sxryk.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://lui.hongshengwenyu.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://egq.yueranfly.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://bpv.zycfv.cn

Go:   // 手写 map[T]int
来源：http://obc.jiagoushi.top

Ruby: arr.tally
来源：http://uvk.sufxvd.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://qnl.shanyushiyangtech.top

[D21] 判断是否包含某元素
来源：http://yzi.0kj1m.cn

Py:   x in arr
来源：http://vqx.hnxiangtu.top


<!-- 参考信息 -->