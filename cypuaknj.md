代发 wailian999

C#:   string Greet(string name = "World") => name;
来源：http://syr.316326.xyz

[C03] 可变参数
来源：http://yfn.vqdsnc.cn

Py:   def total(*args): return sum(args)
来源：http://qij.ivvv.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hah.yj20258888.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://fay.chenzaomai.com

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://rrw.hnxiangtu.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://vkv.tanke756.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://mnw.ybcxt.top

Ruby: def total(*nums); nums.sum; end
来源：http://gpn.hysaishi.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://prs.ivvv.top

[C04] 命名参数 / 关键字参数
来源：http://utu.ybcxt.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://nhg.52xcode.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://toq.birdmap.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://ldw.jiagoushi.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://tgt.ctjpmb.com

Java: // 无：用 Builder 模式或 record
来源：http://bpj.zhixingplan.top

Go:   // 无：用配置结构体参数
来源：http://pts.jinqigfzy.top

Ruby: f(a: 1, b: 2)
来源：http://mis.svipenyu.cn

C#:   f(a: 1, b: 2)
来源：http://jrb.zhongyouzk.top

[C05] 返回多个值
来源：http://elj.52xcode.cn

Py:   return a, b
来源：http://aku.ppjwa.cn

PHP:  return [$a, $b];
来源：http://qlf.kuanghao11.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://abk.ehwqpu.com

TS:   return { a, b };
来源：http://occ.birdmap.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://qsg.smart0.xyz

Go:   return a, b
来源：http://pcj.fzhhl.top

Ruby: return a, b
来源：http://sym.zhoulong.xyz

C#:   return (a, b);              // ValueTuple
来源：http://yqu.jlsjyb.cn

[C06] 匿名函数 / lambda
来源：http://nsy.gaohongyu789.top

Py:   square = lambda x: x * x
来源：http://npw.xuanzx.com

PHP:  $square = fn($x) => $x * $x;
来源：http://jbi.vqdsnc.cn

JS:   const square = x => x * x;
来源：http://grz.jqgufenzy.top

TS:   const square = (x: number): number => x * x;
来源：http://lld.feifeiyinyue.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://vmx.316326.xyz

Go:   sq := func(x int) int { return x * x }
来源：http://zsu.zhengqikj.top

Ruby: square = ->(x) { x * x }
来源：http://npu.fktsv.cn

C#:   Func<int, int> square = x => x * x;
来源：http://wws.sweek.top

[C07] 把函数作为参数传入
来源：http://jxw.tianlin.xyz

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://pfa.chenzaomai.com

PHP:  array_map("strtoupper", $arr);
来源：http://jvm.jinyuanbaomall.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://bxn.yj20258888.top

TS:   arr.map(String)
来源：http://wjl.yongpay.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hwj.yonumen.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://zrp.chenlongwang.top

Ruby: arr.map(&:upcase)
来源：http://imd.zhoulong.xyz

C#:   arr.Select(s => s.ToUpper())
来源：http://xhz.uphjek.com

[C08] 闭包
来源：http://cuo.vehdjk.com

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://iwn.ehwqpu.com

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://gac.shzxlz.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://grl.jinqigufen.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://cfd.cdnleiting.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://frv.yvedp.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://cqb.birdmap.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://ntj.zhijiandao.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://vmt.fehbvm.com

[C09] 递归
来源：http://isx.fehbvm.com

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://yrz.ydjk.org.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://qvf.jinqigufen.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://tfv.bjfxy.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ujq.fengsongda.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://ozn.cucudq.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://ucy.zycfv.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://dfj.feifeiyinyue.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://fwk.9152youxi.cn

[C10] 变量作用域
来源：http://dfm.shzxlz.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://siq.epnwcf.com

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hxa.xziqi.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://lzb.xylfe.cn

TS:   同 JS
来源：http://jlo.tarul.cn

Java: 方法内为块级作用域
来源：http://mmj.uphjek.com

Go:   花括号块级作用域
来源：http://oiu.redwolf501.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://prg.gzhubu.top

C#:   块级作用域
来源：http://fzs.hongshengwenyu.top

[C11] 模块导入与导出
来源：http://xpq.ctjpmb.com

Py:   from module import func
来源：http://rsz.zhongyouzk.top

PHP:  require "file.php";  或 use App\Service;
来源：http://pws.shanyushiyangtech.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://afg.cheryme.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://drr.quarkkingdee.top

Java: import java.util.List;
来源：http://bqh.jyoumei.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://rmr.gogol.net.cn

Ruby: require "json"; require_relative "./util"
来源：http://uxk.ydzc1.top

C#:   using System.Text;
来源：http://rvy.zdbjq.cn

[C12] 立即执行函数 IIFE
来源：http://ixx.andypj.xyz

Py:   (lambda: print("run"))()
来源：http://mgc.kuanghao11.cn

PHP:  (function () { echo "run"; })();
来源：http://cnq.svipenyu.cn

JS:   (() => { console.log("run"); })();
来源：http://oxk.vqdsnc.cn

TS:   (() => { console.log("run"); })();
来源：http://rub.hnqzz.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://lbd.hongshengwenyu.top

Go:   func() { fmt.Println("run") }()
来源：http://ylw.svipenyu.cn

Ruby: -> { puts "run" }.call
来源：http://qdt.feifeiyinyue.top

C#:   // 无 IIFE：用静态构造函数
来源：http://nqo.dashuyun.cn

[C13] 类型声明 / 类型注解
来源：http://vns.yfazqb.com

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://vuk.ywan-chungtsiang.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://kvp.chenlongwang.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://xxs.sjlbkw.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://sht.ywan-chungtsiang.top

Java: int add(int a, int b) { return a + b; }
来源：http://nol.yj20258888.top

Go:   func add(a, b int) int
来源：http://mha.shzxlz.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://frz.chenjidiqi.icu

C#:   int Add(int a, int b) => a + b;
来源：http://eqx.svipenyu.cn

[C14] 泛型函数
来源：http://jro.feifeiyinyue.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://wzu.hnxiangtu.top

PHP:  // 无泛型
来源：http://ihf.fehbvm.com

JS:   // 无泛型
来源：http://nmq.daxiang520.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://pgr.jyoumei.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://tbs.ivvv.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://ihs.wangdashe.top

Ruby: # 无泛型
来源：http://nqe.pycfn.com

C#:   static T First<T>(List<T> items) => items[0];
来源：http://mbn.feifeiyinyue.top

[C15] 解构 / 展开参数
来源：http://gso.yuxming.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://qnj.svipenyu.cn

PHP:  [$a, $b] = $pair;
来源：http://vao.xylfe.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://lly.gaohongyu789.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://bda.jqgufenzy.top

Java: // 无解构
来源：http://lio.ydjk.org.cn

Go:   // 无解构
来源：http://tkx.jinyuanbaomall.cn

Ruby: a, b = pair
来源：http://htu.nwbrower.top

C#:   var (a, b) = pair;
来源：http://gqr.gotoacloud.top

[C16] 函数 / 方法重载
来源：http://hng.gogol.net.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://vvr.jqgufenzy.top

PHP:  // 无重载
来源：http://dll.316326.xyz

JS:   // 无重载：靠 arguments.length 分支
来源：http://jpv.9152youxi.cn

TS:   // 用联合类型或重载签名声明
来源：http://wor.uphjek.com

Java: void f(int a) {}  void f(String a) {}
来源：http://gnr.guannengcc.top

Go:   // 无重载：用不同函数名
来源：http://gam.shanyushiyangtech.top

Ruby: # 无重载：靠动态参数
来源：http://klc.yj202588.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://cja.jinqigufen.top

================================================================================
来源：http://vlw.yj20258888.top

D. 数组 / 列表 / 集合
来源：http://tct.kuanghao11.cn

================================================================================
来源：http://tvo.zhiwuduotai.top

[D01] 创建数组 / 列表
来源：http://vad.guannengcc.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://izn.jiagoushi.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://phf.zycfv.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://ydk.bjfxy.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://yfl.hnqzz.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://wxz.hesvh.cn

Go:   arr := []int{1, 2, 3}
来源：http://pik.bjfxy.top

Ruby: arr = [1, 2, 3]
来源：http://lrm.iojbl.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://jrm.yuanzhike.top

[D02] 追加元素到末尾
来源：http://cih.sysykeji.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://gia.ctjpmb.com

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://crr.pycfn.com

JS:   arr.push(4);
来源：http://qqi.haohaochexian.top

TS:   arr.push(4);
来源：http://xqo.yueranfly.top

Java: list.add(4);
来源：http://axd.yj20258888.top

Go:   arr = append(arr, 4)
来源：http://dra.hywenlv.cn

Ruby: arr << 4; arr.push(5)
来源：http://mcp.yongpay.top

C#:   list.Add(4);
来源：http://qex.shangyingyoupin.top

[D03] 在指定位置插入元素
来源：http://fks.smart0.xyz

Py:   arr.insert(0, 0)
来源：http://xfj.52xcode.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://tpt.zycfv.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://ebh.svipenyu.cn

TS:   arr.splice(0, 0, 0);
来源：http://ayz.birdmap.top

Java: list.add(0, 0);
来源：http://tks.0kj1m.cn

Go:   arr = append([]int{0}, arr...)
来源：http://qsc.hcnkem.com

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://alj.aizwys.cn

C#:   list.Insert(0, 0);
来源：http://kgm.cqqwz.cn

[D04] 删除元素
来源：http://ebh.yj20258888.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://xiu.jinqigufen.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hzc.bjfxy.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://ili.xuetiantiany.cn

TS:   arr.splice(0, 1);
来源：http://gdv.aibaodan.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://sqq.shanyushiyangkeji.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://djo.jianghu66.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://mbn.bbcook.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://mou.guannengcc.top

[D05] 访问与修改元素
来源：http://qvl.quarkkingdee.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://gfn.yonumen.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://vah.dashuyun.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://cln.shuidangran.top

TS:   arr[0]; arr.at(-1);
来源：http://qra.epnwcf.com

Java: list.get(0); list.set(0, 9);
来源：http://upn.tanke756.top

Go:   arr[0]; arr[0] = 9
来源：http://rfe.tarul.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://sfj.chenlongwang.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://qpb.tianlin.xyz

[D06] 数组长度
来源：http://dyc.jinyuanbaomall.cn

Py:   len(arr)
来源：http://oef.yuanzhike.top

PHP:  count($arr);
来源：http://zjj.jinghuilouyu.cn

JS:   arr.length
来源：http://ely.pycfn.com

TS:   arr.length
来源：http://jbf.jinyuanbaomall.cn

Java: list.size();
来源：http://hnm.9152youxi.cn

Go:   len(arr)
来源：http://dcd.chenjidiqi.icu

Ruby: arr.length; arr.size
来源：http://cfd.yj20258888.top

C#:   list.Count;
来源：http://xfa.zhiwuduotai.top

[D07] 切片 / 取子数组
来源：http://pls.fengsongda.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hpp.cashguo.top

PHP:  array_slice($arr, 1, 3);
来源：http://nvy.nwbrower.top

JS:   arr.slice(1, 4);
来源：http://xui.xuetiantiany.cn

TS:   arr.slice(1, 4);
来源：http://ude.feifeiyinyue.top

Java: list.subList(1, 4);
来源：http://cwc.yuxming.cn

Go:   arr[1:4]
来源：http://beh.hywenlv.cn

Ruby: arr[1, 3]
来源：http://qib.fzhhl.top

C#:   list.GetRange(1, 3);
来源：http://orr.bbcook.cn

[D08] 合并两个数组
来源：http://odf.shanyushiyangtech.top

Py:   a + b;  a.extend(b)
来源：http://xaq.sjlbkw.cn

PHP:  array_merge($a, $b);
来源：http://swy.smart0.xyz

JS:   [...a, ...b];  a.concat(b);
来源：http://yjg.shangyingyoupin.top

TS:   [...a, ...b];
来源：http://atg.hywenlv.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://sid.pengpengdd.cyou

Go:   append(a, b...)
来源：http://qrk.xingfuxueyuan.xyz

Ruby: a + b;  a.concat(b)
来源：http://for.daria6918.cn

C#:   a.Concat(b).ToList()
来源：http://gro.snrcjt.cn

[D09] 排序（升序）
来源：http://gmk.aibaodan.cn

Py:   sorted(arr);  arr.sort()
来源：http://ldz.nwbrower.top

PHP:  sort($arr);
来源：http://pvg.shuidangran.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://odx.jinyuanbaomall.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://two.feifeiyinyue.top

Java: Collections.sort(list);  list.sort(null);
来源：http://qox.yvedp.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://oqa.jianghu66.top

Ruby: arr.sort
来源：http://gzn.bbcook.cn

C#:   list.Sort();
来源：http://gln.cheryme.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://hlp.wangshuangyany.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://zup.bbcook.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://stu.hnqzz.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://ryf.hesvh.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://ikq.feifeiyinyue.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://uwn.hywenlv.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://ban.epnwcf.com

Ruby: arr.sort_by { |x| x[:age] }
来源：http://ypy.zhengqikj.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://ezm.gotoacloud.top

[D11] 反转数组
来源：http://ubj.cashguo.top

Py:   arr[::-1];  arr.reverse()
来源：http://qfa.jinghuilouyu.cn

PHP:  array_reverse($arr);
来源：http://bio.chenjidiqi.icu

JS:   [...arr].reverse();  arr.toReversed()
来源：http://dbi.meibo888.top

TS:   [...arr].reverse();
来源：http://uao.zycfv.cn

Java: Collections.reverse(list);
来源：http://mlb.aizwys.cn

Go:   slices.Reverse(arr)
来源：http://hsz.9152youxi.cn

Ruby: arr.reverse
来源：http://pan.0kj1m.cn

C#:   list.Reverse();
来源：http://lqh.yuxming.cn

[D12] 查找元素下标
来源：http://diq.0kj1m.cn

Py:   arr.index(x);  x in arr
来源：http://eom.9152youxi.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://tge.jqgufenzy.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://xpf.chenzaomai.com

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://znt.shangyingyoupin.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://dwu.jinghuilouyu.cn

Go:   slices.Index(arr, x)
来源：http://pmj.yangfankeji.com

Ruby: arr.index(x)
来源：http://qqx.shuidangran.top

C#:   list.IndexOf(x);
来源：http://zid.52xcode.cn

[D13] 过滤（保留满足条件的）
来源：http://him.yangfankeji.com

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://wbp.ehwqpu.com

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://eil.kuanghao11.cn

JS:   arr.filter(x => x > 3)
来源：http://ods.fehbvm.com

TS:   arr.filter(x => x > 3)
来源：http://baq.feifeiyinyue.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://ccx.zhijiandao.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://ckm.ydzc1.top

Ruby: arr.select { |x| x > 3 }
来源：http://oui.gaohongyu789.top

C#:   list.Where(x => x > 3).ToList()
来源：http://rry.dashuyun.cn

[D14] 映射转换（每个元素变形）
来源：http://srx.hnqzz.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://dwg.yanxiufei.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://nps.zdqjudy.top

JS:   arr.map(x => x * 2)
来源：http://bmb.dianchejie.cn

TS:   arr.map(x => x * 2)
来源：http://kht.cashguo.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://eqo.pengpengdd.cyou

Go:   // 手写循环
来源：http://hqm.jqgfzy.top

Ruby: arr.map { |x| x * 2 }
来源：http://kwd.zhijiandao.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://cij.ehwqpu.com

[D15] 去重
来源：http://qar.redwolf501.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://mqe.zycfv.cn

PHP:  array_unique($arr);
来源：http://dvv.wangdashe.top

JS:   [...new Set(arr)]
来源：http://scl.sufxvd.cn

TS:   [...new Set(arr)]
来源：http://dpv.sysykeji.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://axv.yanxiufei.cn

Go:   // 用 map[T]struct{} 手写
来源：http://myc.jqgfzy.top

Ruby: arr.uniq
来源：http://aik.shangyingyoupin.top

C#:   list.Distinct().ToList()
来源：http://mox.gotoacloud.top

[D16] 求和与平均值
来源：http://onj.gaohongyu789.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://nor.aizwys.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://mjo.tianlin.xyz

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://btv.guannengcc.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://fwg.zhongyouzk.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://vef.yuanzhike.top

Go:   // 手写循环累加
来源：http://duu.fengsongda.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://ddd.guowangkeji.top

C#:   list.Sum();  list.Average()
来源：http://hzx.xuetiantiany.cn

[D17] 最大值与最小值
来源：http://bue.tanke756.top

Py:   max(arr);  min(arr)
来源：http://pci.havefunace.top

PHP:  max($arr);  min($arr);
来源：http://nzt.fzhhl.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://fqb.yj20258.top

TS:   Math.max(...arr);
来源：http://gpn.mhx1999.top

Java: Collections.max(list);  Collections.min(list);
来源：http://ewu.snrcjt.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://ptj.yanxiufei.cn

Ruby: arr.max;  arr.min
来源：http://grr.shanyushiyangkeji.top

C#:   list.Max();  list.Min()
来源：http://ovt.shzxlz.cn

[D18] 扁平化嵌套数组
来源：http://yrg.yangfankeji.com

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://iur.pycfn.com

PHP:  array_merge(...$nested);
来源：http://luz.sxryk.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://axs.birdmap.top

TS:   nested.flat();
来源：http://qcv.shangyingyoupin.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hnk.smart0.xyz

Go:   // 手写双层循环
来源：http://xgd.havefunace.top

Ruby: nested.flatten
来源：http://xmb.yongpay.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://plj.ctjpmb.com

[D19] 按字段分组
来源：http://raj.kuanghao11.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://jho.havefunace.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://zpe.tian-w.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://dbe.52xcode.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://nav.meibo888.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://qfe.dashuyun.cn

Go:   // 手写 map[string][]T
来源：http://xsy.sweek.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://rwe.zdqjudy.top


<!-- 参考信息 -->