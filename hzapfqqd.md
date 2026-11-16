代发 wailian999

Java: static int add(int a, int b) { return a + b; }
来源：http://nfs.daxiang520.top

Go:   func add(a, b int) int { return a + b }
来源：http://pwp.mhx1999.top

Ruby: def add(a, b); a + b; end
来源：http://wdc.xuanzx.com

C#:   static int Add(int a, int b) { return a + b; }
来源：http://blj.hongshengwenyu.top

[C02] 默认参数
来源：http://lcg.jianghu66.top

Py:   def greet(name="World"): return name
来源：http://saq.xinyue.icu

PHP:  function greet($name = "World") { return $name; }
来源：http://cdz.yvedp.cn

JS:   function greet(name = "World") { return name; }
来源：http://anp.cashguo.top

TS:   function greet(name: string = "World") { return name; }
来源：http://cdv.yueranfly.top

Java: // 无默认参数：方法重载或 Optional
来源：http://zxd.zdbjq.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://tgt.zhiwuduotai.top

Ruby: def greet(name = "World") = name
来源：http://pxx.zhoulong.xyz

C#:   string Greet(string name = "World") => name;
来源：http://qsf.yfazqb.com

[C03] 可变参数
来源：http://eny.fktsv.cn

Py:   def total(*args): return sum(args)
来源：http://jlw.yuanzhike.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://bre.hammf.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://ocn.316326.xyz

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://ecy.gaohongyu789.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hrt.wangshuangyany.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://ete.vehdjk.com

Ruby: def total(*nums); nums.sum; end
来源：http://tkz.316326.xyz

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://edd.zhiwuduotai.top

[C04] 命名参数 / 关键字参数
来源：http://zma.shanyushiyangtech.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://jnn.redwolf501.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://avs.meibo888.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hqz.nanxinkj.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://zzh.gotoacloud.top

Java: // 无：用 Builder 模式或 record
来源：http://oft.zhongyouzk.top

Go:   // 无：用配置结构体参数
来源：http://vdi.cucudq.cn

Ruby: f(a: 1, b: 2)
来源：http://vul.xuanzx.com

C#:   f(a: 1, b: 2)
来源：http://tjw.kuanghao11.cn

[C05] 返回多个值
来源：http://uzb.feifeiyinyue.top

Py:   return a, b
来源：http://dwv.yongpay.top

PHP:  return [$a, $b];
来源：http://zhw.pengpengdd.cyou

JS:   return [a, b];             // 或 return { a, b };
来源：http://okk.hysaishi.cn

TS:   return { a, b };
来源：http://jpt.shanyushiyangkeji.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://sic.zhijiandao.cn

Go:   return a, b
来源：http://raw.ppjwa.cn

Ruby: return a, b
来源：http://elp.ybcxt.top

C#:   return (a, b);              // ValueTuple
来源：http://lxn.sysykeji.top

[C06] 匿名函数 / lambda
来源：http://vry.yongpay.top

Py:   square = lambda x: x * x
来源：http://hir.daxiang520.top

PHP:  $square = fn($x) => $x * $x;
来源：http://iuo.guowangkeji.top

JS:   const square = x => x * x;
来源：http://kiz.chenjidiqi.icu

TS:   const square = (x: number): number => x * x;
来源：http://tid.yangfankeji.com

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://mee.cheryme.top

Go:   sq := func(x int) int { return x * x }
来源：http://esx.zhijiandao.cn

Ruby: square = ->(x) { x * x }
来源：http://vci.yj20258888.top

C#:   Func<int, int> square = x => x * x;
来源：http://psq.epnwcf.com

[C07] 把函数作为参数传入
来源：http://hwg.birdmap.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://xba.daxiang520.top

PHP:  array_map("strtoupper", $arr);
来源：http://dwp.shangyingyoupin.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://rth.jqgufenzy.top

TS:   arr.map(String)
来源：http://xdj.xuetiantiany.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://yqf.feifeiyinyue.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://osw.shzxlz.cn

Ruby: arr.map(&:upcase)
来源：http://zen.redwolf501.top

C#:   arr.Select(s => s.ToUpper())
来源：http://tjf.jianghu66.top

[C08] 闭包
来源：http://sal.316326.xyz

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://whx.chenlongwang.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://inz.yongpay.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://pgx.zdbjq.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://npt.fanxiaobao.xyz

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://aym.zhaomingkeji.xyz

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://ubh.haohaochexian.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://psq.yj202588.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://cig.ywan-chungtsiang.top

[C09] 递归
来源：http://rtf.ppjwa.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://mxj.nanxuanxn.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://lni.tian-w.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hlu.yuanzhike.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://apf.ywan-chungtsiang.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://ttc.wangdashe.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://wdv.zdbjq.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://phn.0kj1m.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://wnt.0kj1m.cn

[C10] 变量作用域
来源：http://ftl.shzxlz.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hhx.shzxlz.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hzn.jinyuanbaomall.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://eyn.jqgfzy.top

TS:   同 JS
来源：http://pdm.jinqigufen.top

Java: 方法内为块级作用域
来源：http://zsj.yangfankeji.com

Go:   花括号块级作用域
来源：http://hwg.hesvh.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://alm.ehwqpu.com

C#:   块级作用域
来源：http://wvp.chenzaomai.com

[C11] 模块导入与导出
来源：http://wmt.meibo888.top

Py:   from module import func
来源：http://stj.yj20258888.top

PHP:  require "file.php";  或 use App\Service;
来源：http://lkq.xuanzx.com

JS:   export default function f() {};  import f from "./m.js";
来源：http://okk.svipenyu.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://klb.zhaomingkeji.xyz

Java: import java.util.List;
来源：http://tae.hywenlv.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://npr.c1oappe.top

Ruby: require "json"; require_relative "./util"
来源：http://rme.quarkkingdee.top

C#:   using System.Text;
来源：http://qoo.yonumen.top

[C12] 立即执行函数 IIFE
来源：http://pzz.yfazqb.com

Py:   (lambda: print("run"))()
来源：http://wls.chenlongwang.top

PHP:  (function () { echo "run"; })();
来源：http://tyr.xylfe.cn

JS:   (() => { console.log("run"); })();
来源：http://ljf.gotoacloud.top

TS:   (() => { console.log("run"); })();
来源：http://quf.fktsv.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://aok.yongpay.top

Go:   func() { fmt.Println("run") }()
来源：http://ddn.ivvv.top

Ruby: -> { puts "run" }.call
来源：http://omq.sjlbkw.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://mhj.birdmap.top

[C13] 类型声明 / 类型注解
来源：http://azr.9152youxi.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://him.havefunace.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ldb.daria6918.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://xah.yfazqb.com

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wgr.smart0.xyz

Java: int add(int a, int b) { return a + b; }
来源：http://vgq.shuidangran.top

Go:   func add(a, b int) int
来源：http://pil.kuanghao11.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://rqr.gogol.net.cn

C#:   int Add(int a, int b) => a + b;
来源：http://nlz.zdbjq.cn

[C14] 泛型函数
来源：http://ahx.chenjidiqi.icu

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://jrj.dianchejie.cn

PHP:  // 无泛型
来源：http://xpm.sufxvd.cn

JS:   // 无泛型
来源：http://suw.nwbrower.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://mis.zdqjudy.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://gfp.tarul.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://uij.316326.xyz

Ruby: # 无泛型
来源：http://ank.zhoulong.xyz

C#:   static T First<T>(List<T> items) => items[0];
来源：http://dnk.kuanghao11.cn

[C15] 解构 / 展开参数
来源：http://wub.guowangkeji.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://gxz.svipenyu.cn

PHP:  [$a, $b] = $pair;
来源：http://mpq.jinqigfzy.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://dtd.hongshengwenyu.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://mtt.kuanghao11.cn

Java: // 无解构
来源：http://aao.hongshengwenyu.top

Go:   // 无解构
来源：http://mxr.9152youxi.cn

Ruby: a, b = pair
来源：http://xtt.jinyuanbaomall.cn

C#:   var (a, b) = pair;
来源：http://hup.zdbjq.cn

[C16] 函数 / 方法重载
来源：http://dis.zhoulong.xyz

Py:   # 无重载：用默认参数或 *args 变通
来源：http://xvg.pycfn.com

PHP:  // 无重载
来源：http://cxu.wangshuangyany.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://kmk.hfpthk.cn

TS:   // 用联合类型或重载签名声明
来源：http://oaf.cucudq.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://jcr.sjlbkw.cn

Go:   // 无重载：用不同函数名
来源：http://ywn.ydjk.org.cn

Ruby: # 无重载：靠动态参数
来源：http://hwv.vehdjk.com

C#:   void F(int a) {}  void F(string a) {}
来源：http://slk.tarul.cn

================================================================================
来源：http://fwb.daxiang520.top

D. 数组 / 列表 / 集合
来源：http://rvt.yj20258.top

================================================================================
来源：http://cxw.aizwys.cn

[D01] 创建数组 / 列表
来源：http://zsc.bjfxy.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://gep.cdnleiting.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://eon.havefunace.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://gtn.aizwys.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://zva.yuanzhike.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://ldx.cheryme.top

Go:   arr := []int{1, 2, 3}
来源：http://fwi.sjlbkw.cn

Ruby: arr = [1, 2, 3]
来源：http://eny.zhaomingkeji.xyz

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://djj.nanxuanxn.top

[D02] 追加元素到末尾
来源：http://ilz.xuanzx.com

Py:   arr.append(4); arr.extend([5, 6])
来源：http://vvy.chenlongwang.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hya.sjlbkw.cn

JS:   arr.push(4);
来源：http://qih.shuidangran.top

TS:   arr.push(4);
来源：http://pzg.chenzaomai.com

Java: list.add(4);
来源：http://fhd.hcnkem.com

Go:   arr = append(arr, 4)
来源：http://pxt.cheryme.top

Ruby: arr << 4; arr.push(5)
来源：http://keo.chenzaomai.com

C#:   list.Add(4);
来源：http://zrt.zhengqikj.top

[D03] 在指定位置插入元素
来源：http://gni.guowangkeji.top

Py:   arr.insert(0, 0)
来源：http://arh.jqgfzy.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://ztg.smart0.xyz

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://cte.yuanzhike.top

TS:   arr.splice(0, 0, 0);
来源：http://obg.chenlongwang.top

Java: list.add(0, 0);
来源：http://rfw.jlsjyb.cn

Go:   arr = append([]int{0}, arr...)
来源：http://svg.hnxiangtu.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://ace.hongshengwenyu.top

C#:   list.Insert(0, 0);
来源：http://wvj.gotoacloud.top

[D04] 删除元素
来源：http://nom.daria6918.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://xnv.hcnkem.com

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://mos.ybcxt.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://kfq.shuidangran.top

TS:   arr.splice(0, 1);
来源：http://wwe.c1oappe.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://cuk.bbcook.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://qig.zhixingplan.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://rzs.havefunace.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hhm.dashuyun.cn

[D05] 访问与修改元素
来源：http://wzv.cqqwz.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://pzw.zhengqikj.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://svs.quarkkingdee.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://bsm.ydjk.org.cn

TS:   arr[0]; arr.at(-1);
来源：http://sla.wangdashe.top

Java: list.get(0); list.set(0, 9);
来源：http://hsa.ywan-chungtsiang.top

Go:   arr[0]; arr[0] = 9
来源：http://rki.meibo888.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hjq.dianchejie.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://rci.sxryk.cn

[D06] 数组长度
来源：http://aab.nwbrower.top

Py:   len(arr)
来源：http://zrc.kuanghao11.cn

PHP:  count($arr);
来源：http://tgq.jyoumei.cn

JS:   arr.length
来源：http://oyq.hammf.cn

TS:   arr.length
来源：http://yyq.fktsv.cn

Java: list.size();
来源：http://xrm.sweek.top

Go:   len(arr)
来源：http://lvm.fengsongda.top

Ruby: arr.length; arr.size
来源：http://ylb.xinyue.icu

C#:   list.Count;
来源：http://fes.vehdjk.com

[D07] 切片 / 取子数组
来源：http://pgz.birdmap.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://zkw.yj202588.top

PHP:  array_slice($arr, 1, 3);
来源：http://btb.gotoacloud.top

JS:   arr.slice(1, 4);
来源：http://gbh.tanke756.top

TS:   arr.slice(1, 4);
来源：http://ujc.cashguo.top

Java: list.subList(1, 4);
来源：http://kzu.yj20258888.top

Go:   arr[1:4]
来源：http://emo.zhongyouzk.top

Ruby: arr[1, 3]
来源：http://ufc.pengpengdd.cyou

C#:   list.GetRange(1, 3);
来源：http://mnx.iojbl.cn

[D08] 合并两个数组
来源：http://kyd.andypj.xyz

Py:   a + b;  a.extend(b)
来源：http://qkn.xziqi.cn

PHP:  array_merge($a, $b);
来源：http://eir.iojbl.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://otx.feifeiyinyue.top

TS:   [...a, ...b];
来源：http://fnh.meibo888.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://xer.gaohongyu789.top

Go:   append(a, b...)
来源：http://geq.pengpengdd.cyou

Ruby: a + b;  a.concat(b)
来源：http://rgq.hywenlv.cn

C#:   a.Concat(b).ToList()
来源：http://emr.hysaishi.cn

[D09] 排序（升序）
来源：http://euy.fzhhl.top

Py:   sorted(arr);  arr.sort()
来源：http://eyl.jqgfzy.top

PHP:  sort($arr);
来源：http://lut.quarkkingdee.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://spl.haohaochexian.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://omi.pycfn.com

Java: Collections.sort(list);  list.sort(null);
来源：http://eeb.cdnleiting.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://feu.zhongyouzk.top

Ruby: arr.sort
来源：http://zsq.zycfv.cn

C#:   list.Sort();
来源：http://xbs.shanyushiyangkeji.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://teo.gogol.net.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://cob.52xcode.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://pyq.zycfv.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://jma.guannengcc.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://gfb.zdbjq.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://xmw.yvedp.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://tdp.jinyuanbaomall.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://udn.hammf.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://ggj.nanxinkj.top

[D11] 反转数组
来源：http://vkq.tarul.cn

Py:   arr[::-1];  arr.reverse()
来源：http://vax.jinqigufen.top

PHP:  array_reverse($arr);
来源：http://dyt.gotoacloud.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://dbn.zhaomingkeji.xyz

TS:   [...arr].reverse();
来源：http://rga.yonumen.top

Java: Collections.reverse(list);
来源：http://kon.zhoulong.xyz

Go:   slices.Reverse(arr)
来源：http://wjy.cucudq.cn

Ruby: arr.reverse
来源：http://mqg.jinqigufen.top

C#:   list.Reverse();
来源：http://fur.zdbjq.cn

[D12] 查找元素下标
来源：http://sda.mhx1999.top

Py:   arr.index(x);  x in arr
来源：http://glm.jlsjyb.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://lkf.zhijiandao.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hod.c1oappe.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://aay.yanxiufei.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://nhn.zhiwuduotai.top

Go:   slices.Index(arr, x)
来源：http://lxc.xingfuxueyuan.xyz

Ruby: arr.index(x)
来源：http://puu.shanyushiyangtech.top

C#:   list.IndexOf(x);
来源：http://tdl.dianchejie.cn

[D13] 过滤（保留满足条件的）
来源：http://zac.sufxvd.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://coa.tian-w.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hee.zdqjudy.top

JS:   arr.filter(x => x > 3)
来源：http://xiz.gotoacloud.top

TS:   arr.filter(x => x > 3)
来源：http://zsu.316326.xyz

Java: list.stream().filter(x -> x > 3).toList()
来源：http://xwe.cashguo.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://gdm.hongshengwenyu.top

Ruby: arr.select { |x| x > 3 }
来源：http://cwd.shanyushiyangkeji.top

C#:   list.Where(x => x > 3).ToList()
来源：http://mdc.ywan-chungtsiang.top

[D14] 映射转换（每个元素变形）
来源：http://mgj.9152youxi.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://xwc.ppjwa.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://mas.redwolf501.top

JS:   arr.map(x => x * 2)
来源：http://zth.hnqzz.top

TS:   arr.map(x => x * 2)
来源：http://pzu.sxryk.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://zkw.gaohongyu789.top

Go:   // 手写循环
来源：http://gwo.dianchejie.cn

Ruby: arr.map { |x| x * 2 }
来源：http://hil.aizwys.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://blz.316326.xyz

[D15] 去重
来源：http://ads.hammf.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://tqw.yj202588.top

PHP:  array_unique($arr);
来源：http://vvp.nanxinkj.top

JS:   [...new Set(arr)]
来源：http://uzh.chenjidiqi.icu

TS:   [...new Set(arr)]
来源：http://poj.jlsjyb.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://ydi.shanyushiyangkeji.top

Go:   // 用 map[T]struct{} 手写
来源：http://xkd.smart0.xyz

Ruby: arr.uniq
来源：http://tap.fzhhl.top

C#:   list.Distinct().ToList()
来源：http://umr.hywenlv.cn

[D16] 求和与平均值
来源：http://hjq.guannengcc.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://rdf.pycfn.com

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://qcc.redwolf501.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://stv.cashguo.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://iux.gogol.net.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://bxn.wangshuangyany.cn

Go:   // 手写循环累加
来源：http://yhq.cashguo.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://yzo.ehwqpu.com

C#:   list.Sum();  list.Average()
来源：http://xkb.sysykeji.top

[D17] 最大值与最小值
来源：http://pyt.xylfe.cn

Py:   max(arr);  min(arr)
来源：http://dsg.nwbrower.top

PHP:  max($arr);  min($arr);
来源：http://zjh.zhoulong.xyz

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://zap.hysaishi.cn

TS:   Math.max(...arr);
来源：http://pwu.sweek.top

Java: Collections.max(list);  Collections.min(list);
来源：http://wgz.sweek.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://utk.zhoulong.xyz

Ruby: arr.max;  arr.min
来源：http://yrc.jinghuilouyu.cn

C#:   list.Max();  list.Min()
来源：http://kuk.andypj.xyz

[D18] 扁平化嵌套数组
来源：http://cdr.yangfankeji.com

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://unb.aibaodan.cn

PHP:  array_merge(...$nested);
来源：http://sdo.yangfankeji.com

JS:   nested.flat();  nested.flat(Infinity)
来源：http://ybp.nanxinkj.top

TS:   nested.flat();
来源：http://app.xinyue.icu


<!-- 参考信息 -->