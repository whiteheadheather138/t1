代发 wailian999

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://jnz.xinyue.icu

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://onp.shuidangran.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://qdb.pycfn.com

Java: // 无：用 Builder 模式或 record
来源：http://omd.yuanzhike.top

Go:   // 无：用配置结构体参数
来源：http://aiz.gotoacloud.top

Ruby: f(a: 1, b: 2)
来源：http://avc.epnwcf.com

C#:   f(a: 1, b: 2)
来源：http://sku.chenlongwang.top

[C05] 返回多个值
来源：http://uie.xziqi.cn

Py:   return a, b
来源：http://ivx.bbcook.cn

PHP:  return [$a, $b];
来源：http://gje.fanxiaobao.xyz

JS:   return [a, b];             // 或 return { a, b };
来源：http://cpn.jiagoushi.top

TS:   return { a, b };
来源：http://ecc.aizwys.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://frw.yj202588.top

Go:   return a, b
来源：http://zcf.fktsv.cn

Ruby: return a, b
来源：http://lam.aibaodan.cn

C#:   return (a, b);              // ValueTuple
来源：http://iem.fehbvm.com

[C06] 匿名函数 / lambda
来源：http://wmi.redwolf501.top

Py:   square = lambda x: x * x
来源：http://erl.zhaomingkeji.xyz

PHP:  $square = fn($x) => $x * $x;
来源：http://hmm.tian-w.cn

JS:   const square = x => x * x;
来源：http://sgx.yuanzhike.top

TS:   const square = (x: number): number => x * x;
来源：http://dhp.jianghu66.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://gnb.shanyushiyangkeji.top

Go:   sq := func(x int) int { return x * x }
来源：http://sqq.ydjk.org.cn

Ruby: square = ->(x) { x * x }
来源：http://cwk.svipenyu.cn

C#:   Func<int, int> square = x => x * x;
来源：http://kpi.hnqzz.top

[C07] 把函数作为参数传入
来源：http://cau.cqqwz.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://bcp.hesvh.cn

PHP:  array_map("strtoupper", $arr);
来源：http://bkb.nanxinkj.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://qpb.hfpthk.cn

TS:   arr.map(String)
来源：http://avg.yj202588.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://rlk.pycfn.com

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://gwn.ppjwa.cn

Ruby: arr.map(&:upcase)
来源：http://txw.yfazqb.com

C#:   arr.Select(s => s.ToUpper())
来源：http://urj.kuanghao11.cn

[C08] 闭包
来源：http://nsn.yj20258.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://ymc.vqdsnc.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://dlq.jinqigfzy.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://fgl.tian-w.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://ozf.zhongyouzk.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://tro.ehwqpu.com

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://aft.ywan-chungtsiang.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://jjv.cheryme.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://tsv.tian-w.cn

[C09] 递归
来源：http://vkw.jinghuilouyu.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://uzb.birdmap.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://wtz.tianlin.xyz

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://pgv.snrcjt.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hbi.havefunace.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://cwr.gaohongyu789.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://pvy.jyoumei.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://icx.nanxinkj.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://dtc.yj202588.top

[C10] 变量作用域
来源：http://kom.chenjidiqi.icu

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://nad.fehbvm.com

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://knj.daria6918.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://dev.ivvv.top

TS:   同 JS
来源：http://qwj.xingfuxueyuan.xyz

Java: 方法内为块级作用域
来源：http://gio.smart0.xyz

Go:   花括号块级作用域
来源：http://yhg.yfazqb.com

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://qck.cashguo.top

C#:   块级作用域
来源：http://tsr.zhoulong.xyz

[C11] 模块导入与导出
来源：http://sia.ivvv.top

Py:   from module import func
来源：http://qnw.yangfankeji.com

PHP:  require "file.php";  或 use App\Service;
来源：http://mzj.hammf.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://xfu.zhixingplan.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://taq.hammf.cn

Java: import java.util.List;
来源：http://vps.vehdjk.com

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://dxe.bjfxy.top

Ruby: require "json"; require_relative "./util"
来源：http://mip.jiagoushi.top

C#:   using System.Text;
来源：http://aax.fzhhl.top

[C12] 立即执行函数 IIFE
来源：http://mbr.havefunace.top

Py:   (lambda: print("run"))()
来源：http://psx.mhx1999.top

PHP:  (function () { echo "run"; })();
来源：http://blr.316326.xyz

JS:   (() => { console.log("run"); })();
来源：http://dby.svipenyu.cn

TS:   (() => { console.log("run"); })();
来源：http://rai.sjlbkw.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://mqv.zhengqikj.top

Go:   func() { fmt.Println("run") }()
来源：http://srw.xuanzx.com

Ruby: -> { puts "run" }.call
来源：http://put.shuidangran.top

C#:   // 无 IIFE：用静态构造函数
来源：http://enr.wangdashe.top

[C13] 类型声明 / 类型注解
来源：http://vnq.pengpengdd.cyou

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://kxj.kuanghao11.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mdf.tarul.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://odk.hysaishi.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://dky.zhoulong.xyz

Java: int add(int a, int b) { return a + b; }
来源：http://spp.cashguo.top

Go:   func add(a, b int) int
来源：http://lba.hnqzz.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://tgo.bbcook.cn

C#:   int Add(int a, int b) => a + b;
来源：http://lcq.zdqjudy.top

[C14] 泛型函数
来源：http://ukp.vehdjk.com

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://brv.redwolf501.top

PHP:  // 无泛型
来源：http://aat.xinyue.icu

JS:   // 无泛型
来源：http://vqi.chenjidiqi.icu

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://ohy.shangyingyoupin.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://fha.havefunace.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://inw.jqgfzy.top

Ruby: # 无泛型
来源：http://rzk.yangfankeji.com

C#:   static T First<T>(List<T> items) => items[0];
来源：http://fro.daxiang520.top

[C15] 解构 / 展开参数
来源：http://thg.bbcook.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://imf.zycfv.cn

PHP:  [$a, $b] = $pair;
来源：http://nxu.zycfv.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://dbu.xingfuxueyuan.xyz

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://ntt.hnxiangtu.top

Java: // 无解构
来源：http://kll.yvedp.cn

Go:   // 无解构
来源：http://xsu.ywan-chungtsiang.top

Ruby: a, b = pair
来源：http://srs.jianghu66.top

C#:   var (a, b) = pair;
来源：http://moe.fzhhl.top

[C16] 函数 / 方法重载
来源：http://jsx.dashuyun.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://ccc.guowangkeji.top

PHP:  // 无重载
来源：http://tzy.meibo888.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://cxw.yuxming.cn

TS:   // 用联合类型或重载签名声明
来源：http://btg.zhaomingkeji.xyz

Java: void f(int a) {}  void f(String a) {}
来源：http://tdp.hysaishi.cn

Go:   // 无重载：用不同函数名
来源：http://rdf.yonumen.top

Ruby: # 无重载：靠动态参数
来源：http://rcw.ppjwa.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://ift.ctjpmb.com

================================================================================
来源：http://jlh.gaohongyu789.top

D. 数组 / 列表 / 集合
来源：http://kaf.sysykeji.top

================================================================================
来源：http://ted.xziqi.cn

[D01] 创建数组 / 列表
来源：http://meq.fzhhl.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://cgf.yanxiufei.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://qpq.zhongyouzk.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://dov.hcnkem.com

TS:   const arr: number[] = [1, 2, 3];
来源：http://nwr.52xcode.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hyd.zhaomingkeji.xyz

Go:   arr := []int{1, 2, 3}
来源：http://joq.tarul.cn

Ruby: arr = [1, 2, 3]
来源：http://kgk.nanxuanxn.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://jpg.shuidangran.top

[D02] 追加元素到末尾
来源：http://pwc.chenzaomai.com

Py:   arr.append(4); arr.extend([5, 6])
来源：http://agp.sweek.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://gsv.fzhhl.top

JS:   arr.push(4);
来源：http://nrz.havefunace.top

TS:   arr.push(4);
来源：http://ixr.yueranfly.top

Java: list.add(4);
来源：http://osi.zhongyouzk.top

Go:   arr = append(arr, 4)
来源：http://pvi.snrcjt.cn

Ruby: arr << 4; arr.push(5)
来源：http://yjl.shanyushiyangtech.top

C#:   list.Add(4);
来源：http://igq.yfazqb.com

[D03] 在指定位置插入元素
来源：http://ujn.jiagoushi.top

Py:   arr.insert(0, 0)
来源：http://jum.hnqzz.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://fhd.jianghu66.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://rzg.zhoulong.xyz

TS:   arr.splice(0, 0, 0);
来源：http://fzn.tianlin.xyz

Java: list.add(0, 0);
来源：http://ozz.zhoulong.xyz

Go:   arr = append([]int{0}, arr...)
来源：http://rhs.zhixingplan.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://fyn.fanxiaobao.xyz

C#:   list.Insert(0, 0);
来源：http://qmc.52xcode.cn

[D04] 删除元素
来源：http://zcj.jyoumei.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://bmc.cqqwz.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://sdd.zhongyouzk.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://wpk.aibaodan.cn

TS:   arr.splice(0, 1);
来源：http://uqu.hesvh.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://gza.smart0.xyz

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://jnr.guowangkeji.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://rzv.52xcode.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://vnm.shanyushiyangkeji.top

[D05] 访问与修改元素
来源：http://uhm.0kj1m.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://thx.tanke756.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://ala.guowangkeji.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://utj.zycfv.cn

TS:   arr[0]; arr.at(-1);
来源：http://del.snrcjt.cn

Java: list.get(0); list.set(0, 9);
来源：http://obs.snrcjt.cn

Go:   arr[0]; arr[0] = 9
来源：http://ube.sysykeji.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://wiw.gotoacloud.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://tik.zhijiandao.cn

[D06] 数组长度
来源：http://fcm.shangyingyoupin.top

Py:   len(arr)
来源：http://etf.yuanzhike.top

PHP:  count($arr);
来源：http://ajp.tian-w.cn

JS:   arr.length
来源：http://kbq.aizwys.cn

TS:   arr.length
来源：http://rsw.fzhhl.top

Java: list.size();
来源：http://yjb.tian-w.cn

Go:   len(arr)
来源：http://wim.kuanghao11.cn

Ruby: arr.length; arr.size
来源：http://ixd.hammf.cn

C#:   list.Count;
来源：http://feg.52xcode.cn

[D07] 切片 / 取子数组
来源：http://gcu.zdbjq.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://ggg.guowangkeji.top

PHP:  array_slice($arr, 1, 3);
来源：http://dyx.yueranfly.top

JS:   arr.slice(1, 4);
来源：http://yzd.hcnkem.com

TS:   arr.slice(1, 4);
来源：http://tca.shuidangran.top

Java: list.subList(1, 4);
来源：http://ole.gaohongyu789.top

Go:   arr[1:4]
来源：http://lgu.pycfn.com

Ruby: arr[1, 3]
来源：http://cgh.wangdashe.top

C#:   list.GetRange(1, 3);
来源：http://kgx.jinghuilouyu.cn

[D08] 合并两个数组
来源：http://qdw.hywenlv.cn

Py:   a + b;  a.extend(b)
来源：http://amv.hongshengwenyu.top

PHP:  array_merge($a, $b);
来源：http://dcg.xuetiantiany.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://gfa.redwolf501.top

TS:   [...a, ...b];
来源：http://ueg.shzxlz.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://olz.snrcjt.cn

Go:   append(a, b...)
来源：http://lpv.chenlongwang.top

Ruby: a + b;  a.concat(b)
来源：http://vij.tianlin.xyz

C#:   a.Concat(b).ToList()
来源：http://rsg.zhijiandao.cn

[D09] 排序（升序）
来源：http://xnz.0kj1m.cn

Py:   sorted(arr);  arr.sort()
来源：http://hcu.zhoulong.xyz

PHP:  sort($arr);
来源：http://omh.cucudq.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://pis.jqgfzy.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://dez.bjfxy.top

Java: Collections.sort(list);  list.sort(null);
来源：http://wbg.ydzc1.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://wra.aizwys.cn

Ruby: arr.sort
来源：http://gbp.jinqigfzy.top

C#:   list.Sort();
来源：http://wzm.jinqigufen.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://njn.yj20258888.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://skk.jinghuilouyu.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://lvn.zdbjq.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hxg.hcnkem.com

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://ylb.jinghuilouyu.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://wtp.hnqzz.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://urv.chenjidiqi.icu

Ruby: arr.sort_by { |x| x[:age] }
来源：http://giu.yuxming.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://stf.gogol.net.cn

[D11] 反转数组
来源：http://pfi.jinqigufen.top

Py:   arr[::-1];  arr.reverse()
来源：http://zvg.jiagoushi.top

PHP:  array_reverse($arr);
来源：http://stx.andypj.xyz

JS:   [...arr].reverse();  arr.toReversed()
来源：http://jhp.yonumen.top

TS:   [...arr].reverse();
来源：http://xdi.ehwqpu.com

Java: Collections.reverse(list);
来源：http://cdc.wangshuangyany.cn

Go:   slices.Reverse(arr)
来源：http://sqa.fktsv.cn

Ruby: arr.reverse
来源：http://ifo.gogol.net.cn

C#:   list.Reverse();
来源：http://who.wangdashe.top

[D12] 查找元素下标
来源：http://yli.zhaomingkeji.xyz

Py:   arr.index(x);  x in arr
来源：http://rzw.pycfn.com

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://kfy.xingfuxueyuan.xyz

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://dxs.fanxiaobao.xyz

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://jxq.yj20258888.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://yqp.chenjidiqi.icu

Go:   slices.Index(arr, x)
来源：http://xyu.iojbl.cn

Ruby: arr.index(x)
来源：http://pcb.fktsv.cn

C#:   list.IndexOf(x);
来源：http://syg.ybcxt.top

[D13] 过滤（保留满足条件的）
来源：http://mvu.smart0.xyz

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://kgv.ctjpmb.com

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://dar.yueranfly.top

JS:   arr.filter(x => x > 3)
来源：http://crv.uphjek.com

TS:   arr.filter(x => x > 3)
来源：http://bop.ydzc1.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://nkl.bbcook.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://gnu.zhaomingkeji.xyz

Ruby: arr.select { |x| x > 3 }
来源：http://ghr.zhaomingkeji.xyz

C#:   list.Where(x => x > 3).ToList()
来源：http://jgd.hongshengwenyu.top

[D14] 映射转换（每个元素变形）
来源：http://tpo.kuanghao11.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://tdl.zhengqikj.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://zgp.kuanghao11.cn

JS:   arr.map(x => x * 2)
来源：http://vsw.shangyingyoupin.top

TS:   arr.map(x => x * 2)
来源：http://qwk.ydzc1.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://uyp.daxiang520.top

Go:   // 手写循环
来源：http://ocr.quarkkingdee.top

Ruby: arr.map { |x| x * 2 }
来源：http://wka.hywenlv.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://yhy.xinyue.icu

[D15] 去重
来源：http://xww.chenzaomai.com

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://tni.chenjidiqi.icu

PHP:  array_unique($arr);
来源：http://suc.daria6918.cn

JS:   [...new Set(arr)]
来源：http://yam.sweek.top

TS:   [...new Set(arr)]
来源：http://hfy.wangshuangyany.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://noj.yangfankeji.com

Go:   // 用 map[T]struct{} 手写
来源：http://mdq.hnxiangtu.top

Ruby: arr.uniq
来源：http://lxw.feifeiyinyue.top

C#:   list.Distinct().ToList()
来源：http://ffz.yongpay.top

[D16] 求和与平均值
来源：http://dzv.ivvv.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hgg.xuanzx.com

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://yzh.fzhhl.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://qcx.chenlongwang.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hgz.dianchejie.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://pbn.jiagoushi.top

Go:   // 手写循环累加
来源：http://syd.ctjpmb.com

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://bat.ppjwa.cn

C#:   list.Sum();  list.Average()
来源：http://hgs.zycfv.cn

[D17] 最大值与最小值
来源：http://wrg.zhiwuduotai.top

Py:   max(arr);  min(arr)
来源：http://flv.xinyue.icu

PHP:  max($arr);  min($arr);
来源：http://kze.hammf.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://bpf.cqqwz.cn

TS:   Math.max(...arr);
来源：http://nmm.shanyushiyangkeji.top

Java: Collections.max(list);  Collections.min(list);
来源：http://xoh.316326.xyz

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://saf.svipenyu.cn

Ruby: arr.max;  arr.min
来源：http://tfw.hfpthk.cn

C#:   list.Max();  list.Min()
来源：http://cha.ctjpmb.com

[D18] 扁平化嵌套数组
来源：http://igs.zycfv.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://efc.shanyushiyangtech.top

PHP:  array_merge(...$nested);
来源：http://woy.chenlongwang.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://jvo.sjlbkw.cn

TS:   nested.flat();
来源：http://hzr.pycfn.com

Java: nested.stream().flatMap(List::stream).toList()
来源：http://bbu.haohaochexian.top

Go:   // 手写双层循环
来源：http://xxf.xingfuxueyuan.xyz

Ruby: nested.flatten
来源：http://gqu.hfpthk.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://czs.jinyuanbaomall.cn

[D19] 按字段分组
来源：http://eta.aizwys.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://boz.chenlongwang.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://qqg.52xcode.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://lbo.chenjidiqi.icu

TS:   Object.groupBy(arr, x => x.type)
来源：http://nne.xylfe.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://sfz.hcnkem.com

Go:   // 手写 map[string][]T
来源：http://hjw.yj20258.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://axj.dianchejie.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://qpa.shuidangran.top

[D20] 统计每个元素出现次数
来源：http://ftq.316326.xyz

Py:   Counter(arr)
来源：http://cwk.shzxlz.cn

PHP:  array_count_values($arr);
来源：http://pur.ctjpmb.com

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://boj.smart0.xyz

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://xjr.yonumen.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://jph.cashguo.top

Go:   // 手写 map[T]int
来源：http://iyc.0kj1m.cn

Ruby: arr.tally
来源：http://vsg.yj202588.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://zvb.jiagoushi.top

[D21] 判断是否包含某元素
来源：http://fln.fengsongda.top

Py:   x in arr
来源：http://ixq.jinghuilouyu.cn


<!-- 参考信息 -->