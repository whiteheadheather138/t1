代发 wailian999

Ruby: def total(*nums); nums.sum; end
来源：http://ofd.pycfn.com

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://xzo.daxiang520.top

[C04] 命名参数 / 关键字参数
来源：http://bna.xuanzx.com

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://eij.xinyue.icu

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://pyv.jinqigufen.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://ahg.epnwcf.com

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://wuv.cucudq.cn

Java: // 无：用 Builder 模式或 record
来源：http://srn.yj20258.top

Go:   // 无：用配置结构体参数
来源：http://muy.hesvh.cn

Ruby: f(a: 1, b: 2)
来源：http://gss.shanyushiyangtech.top

C#:   f(a: 1, b: 2)
来源：http://gnb.0kj1m.cn

[C05] 返回多个值
来源：http://ctx.gogol.net.cn

Py:   return a, b
来源：http://lhh.ivvv.top

PHP:  return [$a, $b];
来源：http://pnq.mhx1999.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://ekl.yj20258.top

TS:   return { a, b };
来源：http://waq.fzhhl.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://let.ywan-chungtsiang.top

Go:   return a, b
来源：http://wiu.gzhubu.top

Ruby: return a, b
来源：http://ckj.cucudq.cn

C#:   return (a, b);              // ValueTuple
来源：http://tvl.zhijiandao.cn

[C06] 匿名函数 / lambda
来源：http://xif.yonumen.top

Py:   square = lambda x: x * x
来源：http://civ.redwolf501.top

PHP:  $square = fn($x) => $x * $x;
来源：http://wvp.9152youxi.cn

JS:   const square = x => x * x;
来源：http://yvc.yonumen.top

TS:   const square = (x: number): number => x * x;
来源：http://cus.hysaishi.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://nlw.hysaishi.cn

Go:   sq := func(x int) int { return x * x }
来源：http://frn.zdqjudy.top

Ruby: square = ->(x) { x * x }
来源：http://zve.hywenlv.cn

C#:   Func<int, int> square = x => x * x;
来源：http://wpn.tianlin.xyz

[C07] 把函数作为参数传入
来源：http://qlw.bbcook.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://dmc.guowangkeji.top

PHP:  array_map("strtoupper", $arr);
来源：http://mjk.0kj1m.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://kcc.ivvv.top

TS:   arr.map(String)
来源：http://tie.sufxvd.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://tei.nanxuanxn.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://flg.redwolf501.top

Ruby: arr.map(&:upcase)
来源：http://iqs.shanyushiyangkeji.top

C#:   arr.Select(s => s.ToUpper())
来源：http://wwv.uphjek.com

[C08] 闭包
来源：http://moe.yanxiufei.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://gkb.zhiwuduotai.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://ccm.fengsongda.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://ikj.shzxlz.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://wlt.andypj.xyz

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://rib.zdqjudy.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://itg.vehdjk.com

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://vbv.cheryme.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://yvy.shanyushiyangtech.top

[C09] 递归
来源：http://zoo.jinghuilouyu.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://tef.9152youxi.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://ewx.cqqwz.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://sql.ydjk.org.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://keg.cashguo.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://moo.jlsjyb.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://wtf.jiagoushi.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://vfx.epnwcf.com

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://dsj.dianchejie.cn

[C10] 变量作用域
来源：http://eut.fengsongda.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://kwg.yuanzhike.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://vhf.cheryme.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://fbl.tianlin.xyz

TS:   同 JS
来源：http://xvy.hnqzz.top

Java: 方法内为块级作用域
来源：http://kmp.havefunace.top

Go:   花括号块级作用域
来源：http://zeu.xylfe.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://tct.zdqjudy.top

C#:   块级作用域
来源：http://gfl.vehdjk.com

[C11] 模块导入与导出
来源：http://udl.316326.xyz

Py:   from module import func
来源：http://zar.dianchejie.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://pbx.haohaochexian.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://ebt.gotoacloud.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://yse.kuanghao11.cn

Java: import java.util.List;
来源：http://ydr.tanke756.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://lcn.ydjk.org.cn

Ruby: require "json"; require_relative "./util"
来源：http://xia.zdqjudy.top

C#:   using System.Text;
来源：http://zqk.sjlbkw.cn

[C12] 立即执行函数 IIFE
来源：http://yte.ydzc1.top

Py:   (lambda: print("run"))()
来源：http://hzu.shanyushiyangtech.top

PHP:  (function () { echo "run"; })();
来源：http://wgj.xinyue.icu

JS:   (() => { console.log("run"); })();
来源：http://mhi.zhoulong.xyz

TS:   (() => { console.log("run"); })();
来源：http://jci.nanxinkj.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://zxp.hongshengwenyu.top

Go:   func() { fmt.Println("run") }()
来源：http://ghy.hongshengwenyu.top

Ruby: -> { puts "run" }.call
来源：http://hlw.sjlbkw.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://jwt.ivvv.top

[C13] 类型声明 / 类型注解
来源：http://nme.yanxiufei.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://nrd.ybcxt.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://aye.jinyuanbaomall.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hcx.yanxiufei.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://goe.zhongyouzk.top

Java: int add(int a, int b) { return a + b; }
来源：http://lyn.vqdsnc.cn

Go:   func add(a, b int) int
来源：http://wzo.hnqzz.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://pnq.cucudq.cn

C#:   int Add(int a, int b) => a + b;
来源：http://bea.gogol.net.cn

[C14] 泛型函数
来源：http://vha.uphjek.com

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://lor.ehwqpu.com

PHP:  // 无泛型
来源：http://wly.snrcjt.cn

JS:   // 无泛型
来源：http://fpc.zhoulong.xyz

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://rtr.cheryme.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://bgg.chenjidiqi.icu

Go:   func First[T any](items []T) T { return items[0] }
来源：http://vft.jinqigfzy.top

Ruby: # 无泛型
来源：http://aos.jqgufenzy.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://eex.chenzaomai.com

[C15] 解构 / 展开参数
来源：http://csk.iojbl.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://uph.jinghuilouyu.cn

PHP:  [$a, $b] = $pair;
来源：http://moy.daxiang520.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://ehg.hesvh.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://cnh.cashguo.top

Java: // 无解构
来源：http://jou.jinyuanbaomall.cn

Go:   // 无解构
来源：http://kfs.c1oappe.top

Ruby: a, b = pair
来源：http://mzh.xinyue.icu

C#:   var (a, b) = pair;
来源：http://vvf.yuxming.cn

[C16] 函数 / 方法重载
来源：http://ums.zdbjq.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://gwd.daxiang520.top

PHP:  // 无重载
来源：http://vro.fengsongda.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://boe.hammf.cn

TS:   // 用联合类型或重载签名声明
来源：http://dfi.meibo888.top

Java: void f(int a) {}  void f(String a) {}
来源：http://mpb.ivvv.top

Go:   // 无重载：用不同函数名
来源：http://zoz.nanxinkj.top

Ruby: # 无重载：靠动态参数
来源：http://lur.cashguo.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://erv.yonumen.top

================================================================================
来源：http://qyf.feifeiyinyue.top

D. 数组 / 列表 / 集合
来源：http://jmj.jinyuanbaomall.cn

================================================================================
来源：http://gns.xylfe.cn

[D01] 创建数组 / 列表
来源：http://nnb.vqdsnc.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://mvg.sjlbkw.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://wus.birdmap.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://aqw.gzhubu.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://jiu.cheryme.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://rae.zycfv.cn

Go:   arr := []int{1, 2, 3}
来源：http://zkj.bbcook.cn

Ruby: arr = [1, 2, 3]
来源：http://ecc.vqdsnc.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://cta.hfpthk.cn

[D02] 追加元素到末尾
来源：http://ydi.ybcxt.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://gwf.fehbvm.com

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://ioy.fanxiaobao.xyz

JS:   arr.push(4);
来源：http://kfp.quarkkingdee.top

TS:   arr.push(4);
来源：http://jeu.tianlin.xyz

Java: list.add(4);
来源：http://kbe.havefunace.top

Go:   arr = append(arr, 4)
来源：http://iry.xziqi.cn

Ruby: arr << 4; arr.push(5)
来源：http://kpj.pycfn.com

C#:   list.Add(4);
来源：http://ayd.ppjwa.cn

[D03] 在指定位置插入元素
来源：http://oac.hnxiangtu.top

Py:   arr.insert(0, 0)
来源：http://nkc.jinghuilouyu.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://ruz.svipenyu.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://frm.xuetiantiany.cn

TS:   arr.splice(0, 0, 0);
来源：http://vmp.ywan-chungtsiang.top

Java: list.add(0, 0);
来源：http://ihp.jinghuilouyu.cn

Go:   arr = append([]int{0}, arr...)
来源：http://les.shangyingyoupin.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://rbb.birdmap.top

C#:   list.Insert(0, 0);
来源：http://oui.jinqigfzy.top

[D04] 删除元素
来源：http://xug.hnqzz.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://ifw.zhengqikj.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://owm.ppjwa.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://jst.hesvh.cn

TS:   arr.splice(0, 1);
来源：http://pkm.52xcode.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://rfl.dianchejie.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://std.chenlongwang.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://ikj.wangdashe.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://bzi.zhoulong.xyz

[D05] 访问与修改元素
来源：http://hdw.jinghuilouyu.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://civ.yuanzhike.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://fll.9152youxi.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://qqs.pycfn.com

TS:   arr[0]; arr.at(-1);
来源：http://jzl.shanyushiyangtech.top

Java: list.get(0); list.set(0, 9);
来源：http://xzt.ydzc1.top

Go:   arr[0]; arr[0] = 9
来源：http://tkp.xingfuxueyuan.xyz

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://fqb.fzhhl.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://qjx.yongpay.top

[D06] 数组长度
来源：http://qav.feifeiyinyue.top

Py:   len(arr)
来源：http://lie.fktsv.cn

PHP:  count($arr);
来源：http://gsk.sufxvd.cn

JS:   arr.length
来源：http://llg.ctjpmb.com

TS:   arr.length
来源：http://xvv.cheryme.top

Java: list.size();
来源：http://mnv.sufxvd.cn

Go:   len(arr)
来源：http://kwp.gaohongyu789.top

Ruby: arr.length; arr.size
来源：http://mlw.tian-w.cn

C#:   list.Count;
来源：http://ylr.tarul.cn

[D07] 切片 / 取子数组
来源：http://zmi.yanxiufei.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hun.zdqjudy.top

PHP:  array_slice($arr, 1, 3);
来源：http://tur.havefunace.top

JS:   arr.slice(1, 4);
来源：http://xoq.andypj.xyz

TS:   arr.slice(1, 4);
来源：http://yos.jiagoushi.top

Java: list.subList(1, 4);
来源：http://zno.jqgfzy.top

Go:   arr[1:4]
来源：http://kzm.jiagoushi.top

Ruby: arr[1, 3]
来源：http://yer.iojbl.cn

C#:   list.GetRange(1, 3);
来源：http://ijl.uphjek.com

[D08] 合并两个数组
来源：http://oym.hammf.cn

Py:   a + b;  a.extend(b)
来源：http://ojs.zdqjudy.top

PHP:  array_merge($a, $b);
来源：http://aip.fktsv.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://tny.c1oappe.top

TS:   [...a, ...b];
来源：http://hdk.hywenlv.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://fgv.fehbvm.com

Go:   append(a, b...)
来源：http://xkc.hammf.cn

Ruby: a + b;  a.concat(b)
来源：http://yln.bbcook.cn

C#:   a.Concat(b).ToList()
来源：http://hfq.feifeiyinyue.top

[D09] 排序（升序）
来源：http://xek.cqqwz.cn

Py:   sorted(arr);  arr.sort()
来源：http://ddu.daria6918.cn

PHP:  sort($arr);
来源：http://yuc.chenjidiqi.icu

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://dix.zhiwuduotai.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://xmx.gzhubu.top

Java: Collections.sort(list);  list.sort(null);
来源：http://drb.xuetiantiany.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://wll.xinyue.icu

Ruby: arr.sort
来源：http://vfd.cqqwz.cn

C#:   list.Sort();
来源：http://dzv.xingfuxueyuan.xyz

[D10] 自定义排序（按字段 / 多条件）
来源：http://dfe.hammf.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://gue.hfpthk.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://fdq.kuanghao11.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://zou.birdmap.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://btz.chenzaomai.com

Java: list.sort(Comparator.comparing(Person::age));
来源：http://mfx.hywenlv.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://yen.xinyue.icu

Ruby: arr.sort_by { |x| x[:age] }
来源：http://yrk.zhiwuduotai.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://bna.sxryk.cn

[D11] 反转数组
来源：http://oju.jyoumei.cn

Py:   arr[::-1];  arr.reverse()
来源：http://zkb.cqqwz.cn

PHP:  array_reverse($arr);
来源：http://fjq.xuanzx.com

JS:   [...arr].reverse();  arr.toReversed()
来源：http://gqu.shzxlz.cn

TS:   [...arr].reverse();
来源：http://ctw.epnwcf.com

Java: Collections.reverse(list);
来源：http://rop.xuetiantiany.cn

Go:   slices.Reverse(arr)
来源：http://eqc.haohaochexian.top

Ruby: arr.reverse
来源：http://juc.cashguo.top

C#:   list.Reverse();
来源：http://owb.bjfxy.top

[D12] 查找元素下标
来源：http://chn.yfazqb.com

Py:   arr.index(x);  x in arr
来源：http://pyw.jqgfzy.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://vuc.tarul.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://xif.ywan-chungtsiang.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://eze.pengpengdd.cyou

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://ktr.tarul.cn

Go:   slices.Index(arr, x)
来源：http://jpf.hfpthk.cn

Ruby: arr.index(x)
来源：http://qop.hywenlv.cn

C#:   list.IndexOf(x);
来源：http://dqp.jiagoushi.top

[D13] 过滤（保留满足条件的）
来源：http://qwe.yfazqb.com

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://iwc.fehbvm.com

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://lfv.jqgufenzy.top

JS:   arr.filter(x => x > 3)
来源：http://vtp.9152youxi.cn

TS:   arr.filter(x => x > 3)
来源：http://fml.jqgufenzy.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://cfd.redwolf501.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://gyj.wangdashe.top

Ruby: arr.select { |x| x > 3 }
来源：http://grx.sjlbkw.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://njj.jiagoushi.top

[D14] 映射转换（每个元素变形）
来源：http://zmr.0kj1m.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://awi.wangshuangyany.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://uir.0kj1m.cn

JS:   arr.map(x => x * 2)
来源：http://cue.zycfv.cn

TS:   arr.map(x => x * 2)
来源：http://teq.jyoumei.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://hnr.jinghuilouyu.cn

Go:   // 手写循环
来源：http://xzj.jqgufenzy.top

Ruby: arr.map { |x| x * 2 }
来源：http://lnf.yuanzhike.top

C#:   list.Select(x => x * 2).ToList()
来源：http://imj.shangyingyoupin.top

[D15] 去重
来源：http://eut.jinghuilouyu.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://heu.wangdashe.top

PHP:  array_unique($arr);
来源：http://eul.hfpthk.cn

JS:   [...new Set(arr)]
来源：http://sxh.bjfxy.top

TS:   [...new Set(arr)]
来源：http://cdy.xinyue.icu

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://jda.xuetiantiany.cn

Go:   // 用 map[T]struct{} 手写
来源：http://hbi.xziqi.cn

Ruby: arr.uniq
来源：http://zco.sweek.top

C#:   list.Distinct().ToList()
来源：http://vuu.tianlin.xyz

[D16] 求和与平均值
来源：http://xtt.sweek.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://foh.zhoulong.xyz

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://skm.fanxiaobao.xyz

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://nbc.yj20258888.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://rmb.iojbl.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://vkf.nanxinkj.top

Go:   // 手写循环累加
来源：http://yqv.epnwcf.com

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://npu.zdqjudy.top

C#:   list.Sum();  list.Average()
来源：http://vcw.uphjek.com

[D17] 最大值与最小值
来源：http://amc.guannengcc.top

Py:   max(arr);  min(arr)
来源：http://wai.dashuyun.cn

PHP:  max($arr);  min($arr);
来源：http://lxw.cqqwz.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://bas.xziqi.cn

TS:   Math.max(...arr);
来源：http://fyi.cdnleiting.top

Java: Collections.max(list);  Collections.min(list);
来源：http://gbf.shzxlz.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://szm.shuidangran.top

Ruby: arr.max;  arr.min
来源：http://hiw.zhijiandao.cn

C#:   list.Max();  list.Min()
来源：http://csx.jianghu66.top

[D18] 扁平化嵌套数组
来源：http://mkl.yfazqb.com

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://cvk.zdqjudy.top

PHP:  array_merge(...$nested);
来源：http://ixi.shangyingyoupin.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://qui.gotoacloud.top

TS:   nested.flat();
来源：http://fqp.ppjwa.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://vdu.meibo888.top

Go:   // 手写双层循环
来源：http://dpf.wangshuangyany.cn

Ruby: nested.flatten
来源：http://xrx.hysaishi.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://yze.0kj1m.cn

[D19] 按字段分组
来源：http://fjg.zdqjudy.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://mrw.jianghu66.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://izc.sweek.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://fjh.quarkkingdee.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://iwy.fktsv.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://uhg.yvedp.cn

Go:   // 手写 map[string][]T
来源：http://dzo.jinqigufen.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://efu.zhongyouzk.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://vsw.jlsjyb.cn

[D20] 统计每个元素出现次数
来源：http://ukz.xuanzx.com

Py:   Counter(arr)
来源：http://xsc.guannengcc.top

PHP:  array_count_values($arr);
来源：http://dkl.hnxiangtu.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://rmo.fzhhl.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://uwa.snrcjt.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://dki.zycfv.cn

Go:   // 手写 map[T]int
来源：http://zyk.xuanzx.com


<!-- 参考信息 -->