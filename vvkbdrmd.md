代发 wailian999

Ruby: def total(*nums); nums.sum; end
来源：http://nla.meibo888.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://asv.meibo888.top

[C04] 命名参数 / 关键字参数
来源：http://wzf.zhongyouzk.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://eve.zycfv.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://tzf.hammf.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://att.guannengcc.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://wtz.hysaishi.cn

Java: // 无：用 Builder 模式或 record
来源：http://afw.pengpengdd.cyou

Go:   // 无：用配置结构体参数
来源：http://fzi.vehdjk.com

Ruby: f(a: 1, b: 2)
来源：http://pso.fehbvm.com

C#:   f(a: 1, b: 2)
来源：http://ysd.wangshuangyany.cn

[C05] 返回多个值
来源：http://dfv.hfpthk.cn

Py:   return a, b
来源：http://nks.andypj.xyz

PHP:  return [$a, $b];
来源：http://yjz.ydzc1.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://fxw.yongpay.top

TS:   return { a, b };
来源：http://isy.zhiwuduotai.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://vwn.sufxvd.cn

Go:   return a, b
来源：http://fzv.fanxiaobao.xyz

Ruby: return a, b
来源：http://adc.andypj.xyz

C#:   return (a, b);              // ValueTuple
来源：http://ivv.ybcxt.top

[C06] 匿名函数 / lambda
来源：http://sty.xingfuxueyuan.xyz

Py:   square = lambda x: x * x
来源：http://uzo.quarkkingdee.top

PHP:  $square = fn($x) => $x * $x;
来源：http://hso.fengsongda.top

JS:   const square = x => x * x;
来源：http://bys.jinghuilouyu.cn

TS:   const square = (x: number): number => x * x;
来源：http://zzx.svipenyu.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://tdn.guowangkeji.top

Go:   sq := func(x int) int { return x * x }
来源：http://ywk.ydzc1.top

Ruby: square = ->(x) { x * x }
来源：http://zek.hywenlv.cn

C#:   Func<int, int> square = x => x * x;
来源：http://bqv.ydzc1.top

[C07] 把函数作为参数传入
来源：http://ttg.xingfuxueyuan.xyz

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://ooo.sxryk.cn

PHP:  array_map("strtoupper", $arr);
来源：http://jpy.aibaodan.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://zoo.shzxlz.cn

TS:   arr.map(String)
来源：http://rbv.haohaochexian.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hjq.zhaomingkeji.xyz

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://tcu.shangyingyoupin.top

Ruby: arr.map(&:upcase)
来源：http://rpx.aibaodan.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://csq.zhoulong.xyz

[C08] 闭包
来源：http://zzd.zhiwuduotai.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://nvn.sweek.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://zgo.ctjpmb.com

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://bpf.tanke756.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://lit.iojbl.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://jrt.quarkkingdee.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://fqp.0kj1m.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://dpc.zdbjq.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://ibx.wangdashe.top

[C09] 递归
来源：http://ipg.snrcjt.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://qwt.yj20258888.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://pia.kuanghao11.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mhh.vqdsnc.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://cph.guowangkeji.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://pri.wangshuangyany.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://obn.jqgufenzy.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://jiq.epnwcf.com

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://anf.nanxuanxn.top

[C10] 变量作用域
来源：http://jwh.sxryk.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://xtw.yanxiufei.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://bhd.jiagoushi.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://cvt.yanxiufei.cn

TS:   同 JS
来源：http://xob.chenjidiqi.icu

Java: 方法内为块级作用域
来源：http://dwm.ydzc1.top

Go:   花括号块级作用域
来源：http://rdz.havefunace.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://jzs.guannengcc.top

C#:   块级作用域
来源：http://anu.sufxvd.cn

[C11] 模块导入与导出
来源：http://lmc.nanxuanxn.top

Py:   from module import func
来源：http://cua.vehdjk.com

PHP:  require "file.php";  或 use App\Service;
来源：http://mpp.yuanzhike.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://gfq.guowangkeji.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://dds.hfpthk.cn

Java: import java.util.List;
来源：http://gna.jinqigufen.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://ffg.sufxvd.cn

Ruby: require "json"; require_relative "./util"
来源：http://zpv.pengpengdd.cyou

C#:   using System.Text;
来源：http://fqv.shanyushiyangtech.top

[C12] 立即执行函数 IIFE
来源：http://dvf.zycfv.cn

Py:   (lambda: print("run"))()
来源：http://nlm.shzxlz.cn

PHP:  (function () { echo "run"; })();
来源：http://xfg.hcnkem.com

JS:   (() => { console.log("run"); })();
来源：http://hui.chenzaomai.com

TS:   (() => { console.log("run"); })();
来源：http://fdm.pycfn.com

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://sjq.guowangkeji.top

Go:   func() { fmt.Println("run") }()
来源：http://nwp.ehwqpu.com

Ruby: -> { puts "run" }.call
来源：http://zph.yvedp.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://rmv.316326.xyz

[C13] 类型声明 / 类型注解
来源：http://uhg.shanyushiyangkeji.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://jfq.chenlongwang.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://rlt.cashguo.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://kib.yfazqb.com

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://fcz.nanxinkj.top

Java: int add(int a, int b) { return a + b; }
来源：http://nmw.zhaomingkeji.xyz

Go:   func add(a, b int) int
来源：http://fco.0kj1m.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://loi.hnxiangtu.top

C#:   int Add(int a, int b) => a + b;
来源：http://ips.yueranfly.top

[C14] 泛型函数
来源：http://xxl.zhijiandao.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://inf.jianghu66.top

PHP:  // 无泛型
来源：http://wbt.sxryk.cn

JS:   // 无泛型
来源：http://jpz.hesvh.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://xai.svipenyu.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://das.cashguo.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://zvn.jinyuanbaomall.cn

Ruby: # 无泛型
来源：http://sow.jinghuilouyu.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://dri.yangfankeji.com

[C15] 解构 / 展开参数
来源：http://pto.cqqwz.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://uxr.yvedp.cn

PHP:  [$a, $b] = $pair;
来源：http://mbl.ivvv.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://dvs.jianghu66.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://pxv.yj202588.top

Java: // 无解构
来源：http://qlc.xinyue.icu

Go:   // 无解构
来源：http://mrq.daxiang520.top

Ruby: a, b = pair
来源：http://oms.hywenlv.cn

C#:   var (a, b) = pair;
来源：http://abq.hfpthk.cn

[C16] 函数 / 方法重载
来源：http://mye.fktsv.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://drr.uphjek.com

PHP:  // 无重载
来源：http://bvj.bjfxy.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://sob.nanxinkj.top

TS:   // 用联合类型或重载签名声明
来源：http://wuy.chenjidiqi.icu

Java: void f(int a) {}  void f(String a) {}
来源：http://iog.52xcode.cn

Go:   // 无重载：用不同函数名
来源：http://vke.ydzc1.top

Ruby: # 无重载：靠动态参数
来源：http://dvf.ctjpmb.com

C#:   void F(int a) {}  void F(string a) {}
来源：http://xtr.wangdashe.top

================================================================================
来源：http://mpc.hongshengwenyu.top

D. 数组 / 列表 / 集合
来源：http://gsx.tarul.cn

================================================================================
来源：http://eoa.hysaishi.cn

[D01] 创建数组 / 列表
来源：http://tde.guowangkeji.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://zec.hesvh.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://xys.zycfv.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://ybn.yvedp.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://mlr.316326.xyz

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://ctz.vehdjk.com

Go:   arr := []int{1, 2, 3}
来源：http://mra.fehbvm.com

Ruby: arr = [1, 2, 3]
来源：http://eoe.wangdashe.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://oas.ydzc1.top

[D02] 追加元素到末尾
来源：http://wfd.9152youxi.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://osl.yangfankeji.com

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://jhf.c1oappe.top

JS:   arr.push(4);
来源：http://mbc.hywenlv.cn

TS:   arr.push(4);
来源：http://ngq.yangfankeji.com

Java: list.add(4);
来源：http://vcg.hysaishi.cn

Go:   arr = append(arr, 4)
来源：http://obf.jlsjyb.cn

Ruby: arr << 4; arr.push(5)
来源：http://mbf.zhixingplan.top

C#:   list.Add(4);
来源：http://wnv.shzxlz.cn

[D03] 在指定位置插入元素
来源：http://fht.yangfankeji.com

Py:   arr.insert(0, 0)
来源：http://bts.gotoacloud.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://ero.ywan-chungtsiang.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://sna.yueranfly.top

TS:   arr.splice(0, 0, 0);
来源：http://jmu.jqgufenzy.top

Java: list.add(0, 0);
来源：http://ino.jinqigufen.top

Go:   arr = append([]int{0}, arr...)
来源：http://xcg.haohaochexian.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://ekg.bjfxy.top

C#:   list.Insert(0, 0);
来源：http://goa.cashguo.top

[D04] 删除元素
来源：http://qsd.quarkkingdee.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://wsl.zycfv.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://cfn.zhaomingkeji.xyz

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://nrw.yueranfly.top

TS:   arr.splice(0, 1);
来源：http://vgn.chenlongwang.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://bro.vehdjk.com

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://rdw.yfazqb.com

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://ire.daxiang520.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://mao.xziqi.cn

[D05] 访问与修改元素
来源：http://wbe.yj202588.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://rfa.yvedp.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://jgd.cashguo.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://jkw.guowangkeji.top

TS:   arr[0]; arr.at(-1);
来源：http://vko.yvedp.cn

Java: list.get(0); list.set(0, 9);
来源：http://avt.cucudq.cn

Go:   arr[0]; arr[0] = 9
来源：http://zmh.jqgufenzy.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hjs.yj202588.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hxn.nanxuanxn.top

[D06] 数组长度
来源：http://iti.yj20258.top

Py:   len(arr)
来源：http://yzg.shanyushiyangkeji.top

PHP:  count($arr);
来源：http://bya.zhixingplan.top

JS:   arr.length
来源：http://pvw.jqgufenzy.top

TS:   arr.length
来源：http://yay.zycfv.cn

Java: list.size();
来源：http://otz.aibaodan.cn

Go:   len(arr)
来源：http://spf.cashguo.top

Ruby: arr.length; arr.size
来源：http://mzo.svipenyu.cn

C#:   list.Count;
来源：http://vwk.zdbjq.cn

[D07] 切片 / 取子数组
来源：http://xas.sweek.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://cgr.tarul.cn

PHP:  array_slice($arr, 1, 3);
来源：http://ddp.aibaodan.cn

JS:   arr.slice(1, 4);
来源：http://wpx.nanxuanxn.top

TS:   arr.slice(1, 4);
来源：http://jxp.yj20258888.top

Java: list.subList(1, 4);
来源：http://ihg.zhongyouzk.top

Go:   arr[1:4]
来源：http://nav.9152youxi.cn

Ruby: arr[1, 3]
来源：http://crw.ywan-chungtsiang.top

C#:   list.GetRange(1, 3);
来源：http://agh.0kj1m.cn

[D08] 合并两个数组
来源：http://apo.gaohongyu789.top

Py:   a + b;  a.extend(b)
来源：http://yqj.meibo888.top

PHP:  array_merge($a, $b);
来源：http://xym.gzhubu.top

JS:   [...a, ...b];  a.concat(b);
来源：http://hgk.zhixingplan.top

TS:   [...a, ...b];
来源：http://nkp.hesvh.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://enh.sxryk.cn

Go:   append(a, b...)
来源：http://ndp.hongshengwenyu.top

Ruby: a + b;  a.concat(b)
来源：http://tcr.tian-w.cn

C#:   a.Concat(b).ToList()
来源：http://ffc.nanxinkj.top

[D09] 排序（升序）
来源：http://mbh.yuanzhike.top

Py:   sorted(arr);  arr.sort()
来源：http://dwl.jinqigufen.top

PHP:  sort($arr);
来源：http://cci.zhongyouzk.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://fry.cdnleiting.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://inp.gogol.net.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://msx.9152youxi.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://jbz.hfpthk.cn

Ruby: arr.sort
来源：http://zou.pycfn.com

C#:   list.Sort();
来源：http://pwb.cashguo.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://ynd.jyoumei.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://sqb.uphjek.com

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ztw.pengpengdd.cyou

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://iby.hysaishi.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://kwu.gzhubu.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://pdn.chenzaomai.com

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://tgk.c1oappe.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://zet.gzhubu.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://zaf.fanxiaobao.xyz

[D11] 反转数组
来源：http://lwh.epnwcf.com

Py:   arr[::-1];  arr.reverse()
来源：http://ask.sysykeji.top

PHP:  array_reverse($arr);
来源：http://uid.wangshuangyany.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://jul.tanke756.top

TS:   [...arr].reverse();
来源：http://jrb.yuanzhike.top

Java: Collections.reverse(list);
来源：http://eor.zhaomingkeji.xyz

Go:   slices.Reverse(arr)
来源：http://nkm.zhengqikj.top

Ruby: arr.reverse
来源：http://gbo.tanke756.top

C#:   list.Reverse();
来源：http://jba.yangfankeji.com

[D12] 查找元素下标
来源：http://kup.fehbvm.com

Py:   arr.index(x);  x in arr
来源：http://izb.tianlin.xyz

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://lvp.yj20258.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://jbo.fktsv.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://lnv.nwbrower.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://faw.zhijiandao.cn

Go:   slices.Index(arr, x)
来源：http://ikh.shanyushiyangkeji.top

Ruby: arr.index(x)
来源：http://efi.guannengcc.top

C#:   list.IndexOf(x);
来源：http://djf.ydjk.org.cn

[D13] 过滤（保留满足条件的）
来源：http://wfn.andypj.xyz

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://yat.birdmap.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://gha.guowangkeji.top

JS:   arr.filter(x => x > 3)
来源：http://wtu.xylfe.cn

TS:   arr.filter(x => x > 3)
来源：http://wzk.xuetiantiany.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://jcy.fanxiaobao.xyz

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://vzt.jinqigfzy.top

Ruby: arr.select { |x| x > 3 }
来源：http://aeg.haohaochexian.top

C#:   list.Where(x => x > 3).ToList()
来源：http://dzb.jqgufenzy.top

[D14] 映射转换（每个元素变形）
来源：http://emo.guannengcc.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://gru.xziqi.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://cxt.c1oappe.top

JS:   arr.map(x => x * 2)
来源：http://gno.jinyuanbaomall.cn

TS:   arr.map(x => x * 2)
来源：http://hpr.xziqi.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://slx.zhixingplan.top

Go:   // 手写循环
来源：http://hxm.jiagoushi.top

Ruby: arr.map { |x| x * 2 }
来源：http://ita.meibo888.top

C#:   list.Select(x => x * 2).ToList()
来源：http://ckd.jqgfzy.top

[D15] 去重
来源：http://zix.xylfe.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://sgk.tianlin.xyz

PHP:  array_unique($arr);
来源：http://ttu.316326.xyz

JS:   [...new Set(arr)]
来源：http://pmu.gogol.net.cn

TS:   [...new Set(arr)]
来源：http://hqr.zdqjudy.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://lch.andypj.xyz

Go:   // 用 map[T]struct{} 手写
来源：http://tgb.snrcjt.cn

Ruby: arr.uniq
来源：http://lvl.sjlbkw.cn

C#:   list.Distinct().ToList()
来源：http://fpr.nwbrower.top

[D16] 求和与平均值
来源：http://utl.snrcjt.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://beu.yvedp.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://mqr.xziqi.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://qqq.zhixingplan.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://tds.chenlongwang.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://bgd.svipenyu.cn

Go:   // 手写循环累加
来源：http://rnu.snrcjt.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://ctr.gotoacloud.top

C#:   list.Sum();  list.Average()
来源：http://pfk.hywenlv.cn

[D17] 最大值与最小值
来源：http://mco.fengsongda.top

Py:   max(arr);  min(arr)
来源：http://esx.birdmap.top

PHP:  max($arr);  min($arr);
来源：http://gjq.tianlin.xyz

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://nnr.xziqi.cn

TS:   Math.max(...arr);
来源：http://tae.tian-w.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://itj.vqdsnc.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hqy.yangfankeji.com

Ruby: arr.max;  arr.min
来源：http://owm.snrcjt.cn

C#:   list.Max();  list.Min()
来源：http://seg.xinyue.icu

[D18] 扁平化嵌套数组
来源：http://kat.hesvh.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://yiu.hcnkem.com

PHP:  array_merge(...$nested);
来源：http://koz.tanke756.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://ltq.zdqjudy.top

TS:   nested.flat();
来源：http://sda.shzxlz.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://sni.jinqigufen.top

Go:   // 手写双层循环
来源：http://gox.epnwcf.com

Ruby: nested.flatten
来源：http://bcf.zhiwuduotai.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://ewn.jinghuilouyu.cn

[D19] 按字段分组
来源：http://eoc.yangfankeji.com

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://rnu.hcnkem.com

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://zba.hysaishi.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://nrm.zdqjudy.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://mzt.zhiwuduotai.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://qbx.ydjk.org.cn

Go:   // 手写 map[string][]T
来源：http://dhk.yongpay.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://nnj.xuanzx.com

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://bbj.svipenyu.cn

[D20] 统计每个元素出现次数
来源：http://mvj.jlsjyb.cn

Py:   Counter(arr)
来源：http://die.zhengqikj.top

PHP:  array_count_values($arr);
来源：http://uzw.hongshengwenyu.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://prj.ppjwa.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://zjz.yj20258.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://jbp.yj202588.top

Go:   // 手写 map[T]int
来源：http://won.zdbjq.cn


<!-- 参考信息 -->