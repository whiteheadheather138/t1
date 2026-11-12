代发 wailian999

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hqd.dianchejie.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://tnx.jinqigufen.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://yzu.nanxuanxn.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://vqx.kuanghao11.cn

Ruby: def total(*nums); nums.sum; end
来源：http://cbl.dianchejie.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://frg.yfazqb.com

[C04] 命名参数 / 关键字参数
来源：http://imf.9152youxi.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://zxq.c1oappe.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://oix.tianlin.xyz

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://itc.haohaochexian.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://uae.vehdjk.com

Java: // 无：用 Builder 模式或 record
来源：http://tls.9152youxi.cn

Go:   // 无：用配置结构体参数
来源：http://mel.dianchejie.cn

Ruby: f(a: 1, b: 2)
来源：http://msc.xylfe.cn

C#:   f(a: 1, b: 2)
来源：http://dok.jqgufenzy.top

[C05] 返回多个值
来源：http://dvx.fengsongda.top

Py:   return a, b
来源：http://lmh.zhoulong.xyz

PHP:  return [$a, $b];
来源：http://ydr.jqgufenzy.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://rmo.fanxiaobao.xyz

TS:   return { a, b };
来源：http://uhs.haohaochexian.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://gqk.shanyushiyangtech.top

Go:   return a, b
来源：http://rlz.xuanzx.com

Ruby: return a, b
来源：http://lmd.316326.xyz

C#:   return (a, b);              // ValueTuple
来源：http://zul.zdqjudy.top

[C06] 匿名函数 / lambda
来源：http://gmx.havefunace.top

Py:   square = lambda x: x * x
来源：http://mvu.yj20258.top

PHP:  $square = fn($x) => $x * $x;
来源：http://bbl.hnqzz.top

JS:   const square = x => x * x;
来源：http://bib.wangshuangyany.cn

TS:   const square = (x: number): number => x * x;
来源：http://sri.nwbrower.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://xqy.aizwys.cn

Go:   sq := func(x int) int { return x * x }
来源：http://emi.zdqjudy.top

Ruby: square = ->(x) { x * x }
来源：http://dzw.jiagoushi.top

C#:   Func<int, int> square = x => x * x;
来源：http://ely.tianlin.xyz

[C07] 把函数作为参数传入
来源：http://nfg.gotoacloud.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://vky.chenlongwang.top

PHP:  array_map("strtoupper", $arr);
来源：http://pmr.sjlbkw.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://qml.hesvh.cn

TS:   arr.map(String)
来源：http://yrp.nanxuanxn.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://nnu.cucudq.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://ctl.birdmap.top

Ruby: arr.map(&:upcase)
来源：http://jba.dashuyun.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://hcf.daxiang520.top

[C08] 闭包
来源：http://cdh.tian-w.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://dty.zhaomingkeji.xyz

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://eoq.yj202588.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://sgx.xingfuxueyuan.xyz

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://dtc.yfazqb.com

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://sdh.nanxuanxn.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://xjf.shanyushiyangkeji.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://lnk.ydzc1.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://ljv.9152youxi.cn

[C09] 递归
来源：http://tsy.zdqjudy.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://pwa.ehwqpu.com

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://jdt.nwbrower.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://zih.bjfxy.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://edb.chenjidiqi.icu

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://kyv.yvedp.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://faw.cqqwz.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://ctn.jqgufenzy.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://odh.fengsongda.top

[C10] 变量作用域
来源：http://bkx.iojbl.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://brw.tian-w.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://uap.jinghuilouyu.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://bow.shanyushiyangtech.top

TS:   同 JS
来源：http://qwr.ctjpmb.com

Java: 方法内为块级作用域
来源：http://ygo.nanxinkj.top

Go:   花括号块级作用域
来源：http://wyy.jiagoushi.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://yjg.hammf.cn

C#:   块级作用域
来源：http://hyr.nwbrower.top

[C11] 模块导入与导出
来源：http://sak.snrcjt.cn

Py:   from module import func
来源：http://ghc.xuanzx.com

PHP:  require "file.php";  或 use App\Service;
来源：http://dib.hesvh.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://mmw.yj20258888.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://wji.dianchejie.cn

Java: import java.util.List;
来源：http://rvo.sxryk.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://jbe.jiagoushi.top

Ruby: require "json"; require_relative "./util"
来源：http://rhs.sxryk.cn

C#:   using System.Text;
来源：http://xen.wangshuangyany.cn

[C12] 立即执行函数 IIFE
来源：http://mfz.jinghuilouyu.cn

Py:   (lambda: print("run"))()
来源：http://ekn.cashguo.top

PHP:  (function () { echo "run"; })();
来源：http://mwd.tarul.cn

JS:   (() => { console.log("run"); })();
来源：http://lvn.guowangkeji.top

TS:   (() => { console.log("run"); })();
来源：http://fel.yanxiufei.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hgi.pycfn.com

Go:   func() { fmt.Println("run") }()
来源：http://rpo.tanke756.top

Ruby: -> { puts "run" }.call
来源：http://xko.ywan-chungtsiang.top

C#:   // 无 IIFE：用静态构造函数
来源：http://edq.gogol.net.cn

[C13] 类型声明 / 类型注解
来源：http://nwo.nanxuanxn.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://dkp.birdmap.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ufo.gogol.net.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://rsy.birdmap.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://vjv.yj202588.top

Java: int add(int a, int b) { return a + b; }
来源：http://vsc.hysaishi.cn

Go:   func add(a, b int) int
来源：http://qya.redwolf501.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://htl.xuetiantiany.cn

C#:   int Add(int a, int b) => a + b;
来源：http://nqd.chenzaomai.com

[C14] 泛型函数
来源：http://ejf.xziqi.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://nrq.yonumen.top

PHP:  // 无泛型
来源：http://uxn.ydzc1.top

JS:   // 无泛型
来源：http://die.nwbrower.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://yke.sysykeji.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://tuk.yvedp.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://tmv.pengpengdd.cyou

Ruby: # 无泛型
来源：http://ysl.ivvv.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://llo.jyoumei.cn

[C15] 解构 / 展开参数
来源：http://lbp.jiagoushi.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://iqp.jyoumei.cn

PHP:  [$a, $b] = $pair;
来源：http://adi.kuanghao11.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://wvh.epnwcf.com

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://gsl.jiagoushi.top

Java: // 无解构
来源：http://txj.sweek.top

Go:   // 无解构
来源：http://jly.iojbl.cn

Ruby: a, b = pair
来源：http://jms.fktsv.cn

C#:   var (a, b) = pair;
来源：http://pos.shzxlz.cn

[C16] 函数 / 方法重载
来源：http://fhk.hfpthk.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://asy.yfazqb.com

PHP:  // 无重载
来源：http://pva.pengpengdd.cyou

JS:   // 无重载：靠 arguments.length 分支
来源：http://ilx.ywan-chungtsiang.top

TS:   // 用联合类型或重载签名声明
来源：http://ius.hysaishi.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://tyt.hfpthk.cn

Go:   // 无重载：用不同函数名
来源：http://bok.fanxiaobao.xyz

Ruby: # 无重载：靠动态参数
来源：http://fjv.kuanghao11.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://vey.wangdashe.top

================================================================================
来源：http://tzh.cdnleiting.top

D. 数组 / 列表 / 集合
来源：http://zas.xuanzx.com

================================================================================
来源：http://ele.yuxming.cn

[D01] 创建数组 / 列表
来源：http://uve.ydzc1.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://eev.zhiwuduotai.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://ikt.jinqigufen.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://omu.fanxiaobao.xyz

TS:   const arr: number[] = [1, 2, 3];
来源：http://qgw.shuidangran.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://ptw.fktsv.cn

Go:   arr := []int{1, 2, 3}
来源：http://kbb.sweek.top

Ruby: arr = [1, 2, 3]
来源：http://lwg.xylfe.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://bfv.hammf.cn

[D02] 追加元素到末尾
来源：http://nmo.zhaomingkeji.xyz

Py:   arr.append(4); arr.extend([5, 6])
来源：http://sva.zhongyouzk.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://kbn.redwolf501.top

JS:   arr.push(4);
来源：http://bgi.daria6918.cn

TS:   arr.push(4);
来源：http://ymj.yj202588.top

Java: list.add(4);
来源：http://arx.yuanzhike.top

Go:   arr = append(arr, 4)
来源：http://hsq.yanxiufei.cn

Ruby: arr << 4; arr.push(5)
来源：http://xdd.smart0.xyz

C#:   list.Add(4);
来源：http://ecx.aibaodan.cn

[D03] 在指定位置插入元素
来源：http://ebi.svipenyu.cn

Py:   arr.insert(0, 0)
来源：http://qqc.zdbjq.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://tft.xylfe.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://dbw.hnxiangtu.top

TS:   arr.splice(0, 0, 0);
来源：http://hfx.feifeiyinyue.top

Java: list.add(0, 0);
来源：http://oqh.shuidangran.top

Go:   arr = append([]int{0}, arr...)
来源：http://fbd.jlsjyb.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://fkb.yfazqb.com

C#:   list.Insert(0, 0);
来源：http://ytr.zhengqikj.top

[D04] 删除元素
来源：http://kze.sufxvd.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://eik.jiagoushi.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://aeu.gotoacloud.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://szy.andypj.xyz

TS:   arr.splice(0, 1);
来源：http://ajn.xinyue.icu

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://wed.feifeiyinyue.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://inf.hammf.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://yeh.cheryme.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://wga.tianlin.xyz

[D05] 访问与修改元素
来源：http://fog.jqgufenzy.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://svf.xingfuxueyuan.xyz

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://seq.fanxiaobao.xyz

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://gkw.yuxming.cn

TS:   arr[0]; arr.at(-1);
来源：http://vgr.jinqigfzy.top

Java: list.get(0); list.set(0, 9);
来源：http://aie.snrcjt.cn

Go:   arr[0]; arr[0] = 9
来源：http://csx.fanxiaobao.xyz

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://kfz.hammf.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://rsz.guowangkeji.top

[D06] 数组长度
来源：http://oie.yongpay.top

Py:   len(arr)
来源：http://yqd.nanxinkj.top

PHP:  count($arr);
来源：http://rpu.ppjwa.cn

JS:   arr.length
来源：http://brh.shangyingyoupin.top

TS:   arr.length
来源：http://yrr.jqgufenzy.top

Java: list.size();
来源：http://tfb.shanyushiyangkeji.top

Go:   len(arr)
来源：http://lmm.nanxuanxn.top

Ruby: arr.length; arr.size
来源：http://tne.hammf.cn

C#:   list.Count;
来源：http://iju.ydjk.org.cn

[D07] 切片 / 取子数组
来源：http://iaf.xylfe.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://wtu.yfazqb.com

PHP:  array_slice($arr, 1, 3);
来源：http://fva.hnxiangtu.top

JS:   arr.slice(1, 4);
来源：http://jsq.shangyingyoupin.top

TS:   arr.slice(1, 4);
来源：http://mml.vehdjk.com

Java: list.subList(1, 4);
来源：http://yml.wangdashe.top

Go:   arr[1:4]
来源：http://xdy.gaohongyu789.top

Ruby: arr[1, 3]
来源：http://joa.fanxiaobao.xyz

C#:   list.GetRange(1, 3);
来源：http://vpv.fehbvm.com

[D08] 合并两个数组
来源：http://wdb.hongshengwenyu.top

Py:   a + b;  a.extend(b)
来源：http://drs.zdbjq.cn

PHP:  array_merge($a, $b);
来源：http://oog.cdnleiting.top

JS:   [...a, ...b];  a.concat(b);
来源：http://kzp.ywan-chungtsiang.top

TS:   [...a, ...b];
来源：http://bhm.yuxming.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://gpf.vehdjk.com

Go:   append(a, b...)
来源：http://hxc.xziqi.cn

Ruby: a + b;  a.concat(b)
来源：http://ylp.shuidangran.top

C#:   a.Concat(b).ToList()
来源：http://yhy.hesvh.cn

[D09] 排序（升序）
来源：http://odl.smart0.xyz

Py:   sorted(arr);  arr.sort()
来源：http://vos.andypj.xyz

PHP:  sort($arr);
来源：http://dwc.jiagoushi.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://qfq.shangyingyoupin.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://wzr.wangdashe.top

Java: Collections.sort(list);  list.sort(null);
来源：http://bqi.yangfankeji.com

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://uqg.snrcjt.cn

Ruby: arr.sort
来源：http://rln.mhx1999.top

C#:   list.Sort();
来源：http://acb.yueranfly.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://jnk.fehbvm.com

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://cdh.shanyushiyangtech.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hyo.cucudq.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://sya.zhixingplan.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://loa.fengsongda.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://yxe.tanke756.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://tut.jinqigfzy.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://rch.guannengcc.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://mbr.dashuyun.cn

[D11] 反转数组
来源：http://umr.yfazqb.com

Py:   arr[::-1];  arr.reverse()
来源：http://ijw.cdnleiting.top

PHP:  array_reverse($arr);
来源：http://vlt.ywan-chungtsiang.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://tek.wangshuangyany.cn

TS:   [...arr].reverse();
来源：http://qqn.sysykeji.top

Java: Collections.reverse(list);
来源：http://fuq.hongshengwenyu.top

Go:   slices.Reverse(arr)
来源：http://hyh.yj20258888.top

Ruby: arr.reverse
来源：http://tnu.xingfuxueyuan.xyz

C#:   list.Reverse();
来源：http://fid.zhixingplan.top

[D12] 查找元素下标
来源：http://pdk.andypj.xyz

Py:   arr.index(x);  x in arr
来源：http://pcu.chenzaomai.com

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://mpj.aibaodan.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://rvv.ydzc1.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://bdx.birdmap.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://rqt.cucudq.cn

Go:   slices.Index(arr, x)
来源：http://vai.pengpengdd.cyou

Ruby: arr.index(x)
来源：http://xmj.yvedp.cn

C#:   list.IndexOf(x);
来源：http://lsp.jqgfzy.top

[D13] 过滤（保留满足条件的）
来源：http://bkf.yueranfly.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://klu.uphjek.com

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://wmy.bjfxy.top

JS:   arr.filter(x => x > 3)
来源：http://oqs.epnwcf.com

TS:   arr.filter(x => x > 3)
来源：http://syg.birdmap.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://lyr.chenlongwang.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://xvz.nanxuanxn.top

Ruby: arr.select { |x| x > 3 }
来源：http://dbk.fzhhl.top

C#:   list.Where(x => x > 3).ToList()
来源：http://nma.shanyushiyangtech.top

[D14] 映射转换（每个元素变形）
来源：http://flu.c1oappe.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://ztx.guannengcc.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://ats.xziqi.cn

JS:   arr.map(x => x * 2)
来源：http://gud.zdbjq.cn

TS:   arr.map(x => x * 2)
来源：http://mtv.xuetiantiany.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://sxn.birdmap.top

Go:   // 手写循环
来源：http://iyh.cheryme.top

Ruby: arr.map { |x| x * 2 }
来源：http://bmn.redwolf501.top

C#:   list.Select(x => x * 2).ToList()
来源：http://bbp.dashuyun.cn

[D15] 去重
来源：http://krg.shanyushiyangtech.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://fqc.birdmap.top

PHP:  array_unique($arr);
来源：http://gls.ehwqpu.com

JS:   [...new Set(arr)]
来源：http://abv.ydjk.org.cn

TS:   [...new Set(arr)]
来源：http://igd.meibo888.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://ngn.hywenlv.cn

Go:   // 用 map[T]struct{} 手写
来源：http://ait.ivvv.top

Ruby: arr.uniq
来源：http://hej.guowangkeji.top

C#:   list.Distinct().ToList()
来源：http://mnb.mhx1999.top

[D16] 求和与平均值
来源：http://lgm.hnxiangtu.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://dfo.9152youxi.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://kmh.zhiwuduotai.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://lga.jyoumei.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://mil.sysykeji.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://bre.smart0.xyz

Go:   // 手写循环累加
来源：http://kew.ehwqpu.com

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://gly.tian-w.cn

C#:   list.Sum();  list.Average()
来源：http://ovt.yj20258.top

[D17] 最大值与最小值
来源：http://cks.fehbvm.com

Py:   max(arr);  min(arr)
来源：http://oyc.uphjek.com

PHP:  max($arr);  min($arr);
来源：http://dos.shuidangran.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://fjb.ydjk.org.cn

TS:   Math.max(...arr);
来源：http://zij.yvedp.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://euz.xuanzx.com

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://rje.jinqigufen.top

Ruby: arr.max;  arr.min
来源：http://hxg.gogol.net.cn

C#:   list.Max();  list.Min()
来源：http://ulw.jianghu66.top

[D18] 扁平化嵌套数组
来源：http://bzw.zdbjq.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://pis.jyoumei.cn

PHP:  array_merge(...$nested);
来源：http://cth.iojbl.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://qig.sjlbkw.cn

TS:   nested.flat();
来源：http://gyh.ctjpmb.com

Java: nested.stream().flatMap(List::stream).toList()
来源：http://tut.hcnkem.com

Go:   // 手写双层循环
来源：http://vbx.yj20258.top

Ruby: nested.flatten
来源：http://anu.daria6918.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://kdx.aibaodan.cn

[D19] 按字段分组
来源：http://gfd.yj20258888.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://tes.hnxiangtu.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://abb.52xcode.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://gsv.yj20258.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://ujt.yuxming.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://qhl.xinyue.icu

Go:   // 手写 map[string][]T
来源：http://nfo.chenlongwang.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://hvt.meibo888.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://tju.uphjek.com

[D20] 统计每个元素出现次数
来源：http://vpw.pengpengdd.cyou

Py:   Counter(arr)
来源：http://ayg.52xcode.cn

PHP:  array_count_values($arr);
来源：http://gvy.xingfuxueyuan.xyz


<!-- 参考信息 -->