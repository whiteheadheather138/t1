代发 wailian999

Ruby: def total(*nums); nums.sum; end
来源：http://fyi.ehwqpu.com

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://wum.cqqwz.cn

[C04] 命名参数 / 关键字参数
来源：http://zux.haohaochexian.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://rfc.daxiang520.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://wxm.pycfn.com

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://ppo.shzxlz.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://eok.shuidangran.top

Java: // 无：用 Builder 模式或 record
来源：http://jug.tanke756.top

Go:   // 无：用配置结构体参数
来源：http://nyx.daxiang520.top

Ruby: f(a: 1, b: 2)
来源：http://jfo.tianlin.xyz

C#:   f(a: 1, b: 2)
来源：http://qyo.hcnkem.com

[C05] 返回多个值
来源：http://wok.xuanzx.com

Py:   return a, b
来源：http://dib.316326.xyz

PHP:  return [$a, $b];
来源：http://hhh.fehbvm.com

JS:   return [a, b];             // 或 return { a, b };
来源：http://yqn.fengsongda.top

TS:   return { a, b };
来源：http://pok.hysaishi.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://yyp.jinqigfzy.top

Go:   return a, b
来源：http://xml.ybcxt.top

Ruby: return a, b
来源：http://hkh.hesvh.cn

C#:   return (a, b);              // ValueTuple
来源：http://xnz.cheryme.top

[C06] 匿名函数 / lambda
来源：http://rly.zhiwuduotai.top

Py:   square = lambda x: x * x
来源：http://udv.hesvh.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://zvl.zdbjq.cn

JS:   const square = x => x * x;
来源：http://cfx.bbcook.cn

TS:   const square = (x: number): number => x * x;
来源：http://caq.svipenyu.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://eeh.zhixingplan.top

Go:   sq := func(x int) int { return x * x }
来源：http://iec.feifeiyinyue.top

Ruby: square = ->(x) { x * x }
来源：http://etj.daria6918.cn

C#:   Func<int, int> square = x => x * x;
来源：http://bed.zhijiandao.cn

[C07] 把函数作为参数传入
来源：http://uxr.guowangkeji.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://ppo.mhx1999.top

PHP:  array_map("strtoupper", $arr);
来源：http://ueg.bbcook.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://mpj.jinqigufen.top

TS:   arr.map(String)
来源：http://hfo.tian-w.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://deo.zhijiandao.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://kil.yueranfly.top

Ruby: arr.map(&:upcase)
来源：http://hkb.shuidangran.top

C#:   arr.Select(s => s.ToUpper())
来源：http://uua.fengsongda.top

[C08] 闭包
来源：http://lrs.feifeiyinyue.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://lkj.gzhubu.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://ucs.zhoulong.xyz

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://ate.xylfe.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://far.ydzc1.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://trv.gotoacloud.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://ytl.zdqjudy.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://mva.hongshengwenyu.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://yoj.gaohongyu789.top

[C09] 递归
来源：http://uce.shanyushiyangtech.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://eoe.cheryme.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://awf.ivvv.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://rhb.fktsv.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://khe.hcnkem.com

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://lxz.xingfuxueyuan.xyz

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://qst.yuanzhike.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://yss.gogol.net.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hsa.chenlongwang.top

[C10] 变量作用域
来源：http://bbh.fzhhl.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://xbb.yanxiufei.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://cvp.jlsjyb.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://kyz.sufxvd.cn

TS:   同 JS
来源：http://xwu.sxryk.cn

Java: 方法内为块级作用域
来源：http://cbz.bbcook.cn

Go:   花括号块级作用域
来源：http://tpa.guannengcc.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://ewv.jinqigufen.top

C#:   块级作用域
来源：http://sjo.jinqigfzy.top

[C11] 模块导入与导出
来源：http://vqa.chenlongwang.top

Py:   from module import func
来源：http://szy.52xcode.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://adt.sxryk.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://urd.yonumen.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://dom.ybcxt.top

Java: import java.util.List;
来源：http://jqo.c1oappe.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://rgb.sufxvd.cn

Ruby: require "json"; require_relative "./util"
来源：http://vup.chenjidiqi.icu

C#:   using System.Text;
来源：http://axt.vehdjk.com

[C12] 立即执行函数 IIFE
来源：http://bio.sufxvd.cn

Py:   (lambda: print("run"))()
来源：http://qib.guowangkeji.top

PHP:  (function () { echo "run"; })();
来源：http://kjg.yanxiufei.cn

JS:   (() => { console.log("run"); })();
来源：http://vkh.gzhubu.top

TS:   (() => { console.log("run"); })();
来源：http://ung.hnxiangtu.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://ujv.yanxiufei.cn

Go:   func() { fmt.Println("run") }()
来源：http://ciq.jinqigfzy.top

Ruby: -> { puts "run" }.call
来源：http://wtd.zhiwuduotai.top

C#:   // 无 IIFE：用静态构造函数
来源：http://xep.chenlongwang.top

[C13] 类型声明 / 类型注解
来源：http://xyg.zdqjudy.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://ynx.sysykeji.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ofk.chenjidiqi.icu

JS:   // 无类型（可用 JSDoc 注释）
来源：http://eim.dashuyun.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ieg.hesvh.cn

Java: int add(int a, int b) { return a + b; }
来源：http://dss.cucudq.cn

Go:   func add(a, b int) int
来源：http://qcu.tarul.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://kdf.xziqi.cn

C#:   int Add(int a, int b) => a + b;
来源：http://glf.sxryk.cn

[C14] 泛型函数
来源：http://xrm.xylfe.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://ehj.gogol.net.cn

PHP:  // 无泛型
来源：http://nax.ydzc1.top

JS:   // 无泛型
来源：http://dck.xziqi.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://fut.chenlongwang.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://anw.shzxlz.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hen.zhijiandao.cn

Ruby: # 无泛型
来源：http://ttl.sjlbkw.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://pih.hysaishi.cn

[C15] 解构 / 展开参数
来源：http://tjk.xuetiantiany.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://rxk.quarkkingdee.top

PHP:  [$a, $b] = $pair;
来源：http://bzu.daxiang520.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://rku.sweek.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://kkr.xuetiantiany.cn

Java: // 无解构
来源：http://cul.shanyushiyangkeji.top

Go:   // 无解构
来源：http://ezd.c1oappe.top

Ruby: a, b = pair
来源：http://xdl.haohaochexian.top

C#:   var (a, b) = pair;
来源：http://nai.hysaishi.cn

[C16] 函数 / 方法重载
来源：http://lba.shzxlz.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://spo.aibaodan.cn

PHP:  // 无重载
来源：http://hym.haohaochexian.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://khv.0kj1m.cn

TS:   // 用联合类型或重载签名声明
来源：http://eym.fengsongda.top

Java: void f(int a) {}  void f(String a) {}
来源：http://epp.52xcode.cn

Go:   // 无重载：用不同函数名
来源：http://zxw.tarul.cn

Ruby: # 无重载：靠动态参数
来源：http://owp.feifeiyinyue.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://yve.chenjidiqi.icu

================================================================================
来源：http://lek.cucudq.cn

D. 数组 / 列表 / 集合
来源：http://vzw.hnqzz.top

================================================================================
来源：http://kur.yuxming.cn

[D01] 创建数组 / 列表
来源：http://qqq.fengsongda.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://wie.chenlongwang.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://ebb.shuidangran.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://xbt.jqgufenzy.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://bvc.feifeiyinyue.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://nta.meibo888.top

Go:   arr := []int{1, 2, 3}
来源：http://wnm.daxiang520.top

Ruby: arr = [1, 2, 3]
来源：http://eup.hnqzz.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://nix.zhaomingkeji.xyz

[D02] 追加元素到末尾
来源：http://erm.cucudq.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://qoy.sxryk.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://yhr.zhongyouzk.top

JS:   arr.push(4);
来源：http://ueq.chenjidiqi.icu

TS:   arr.push(4);
来源：http://aix.ydjk.org.cn

Java: list.add(4);
来源：http://lsp.shzxlz.cn

Go:   arr = append(arr, 4)
来源：http://tig.shuidangran.top

Ruby: arr << 4; arr.push(5)
来源：http://cjr.bbcook.cn

C#:   list.Add(4);
来源：http://qmy.jyoumei.cn

[D03] 在指定位置插入元素
来源：http://gwc.hesvh.cn

Py:   arr.insert(0, 0)
来源：http://wcq.quarkkingdee.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://jyg.gaohongyu789.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://gng.9152youxi.cn

TS:   arr.splice(0, 0, 0);
来源：http://gyj.aizwys.cn

Java: list.add(0, 0);
来源：http://fuw.yfazqb.com

Go:   arr = append([]int{0}, arr...)
来源：http://gah.jinqigfzy.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://mtx.sjlbkw.cn

C#:   list.Insert(0, 0);
来源：http://bbm.guannengcc.top

[D04] 删除元素
来源：http://cux.0kj1m.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://vqq.gotoacloud.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://idh.jyoumei.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://kqq.hnqzz.top

TS:   arr.splice(0, 1);
来源：http://mzk.nanxuanxn.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://tui.havefunace.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://lpn.pengpengdd.cyou

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://puq.hysaishi.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://kte.hnqzz.top

[D05] 访问与修改元素
来源：http://vtl.gzhubu.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://fqn.ywan-chungtsiang.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://npi.xuetiantiany.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://jlf.chenlongwang.top

TS:   arr[0]; arr.at(-1);
来源：http://fww.tian-w.cn

Java: list.get(0); list.set(0, 9);
来源：http://pci.ivvv.top

Go:   arr[0]; arr[0] = 9
来源：http://uzr.sufxvd.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://rrf.gzhubu.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://rhb.sjlbkw.cn

[D06] 数组长度
来源：http://btk.wangshuangyany.cn

Py:   len(arr)
来源：http://vjb.gzhubu.top

PHP:  count($arr);
来源：http://ylb.gogol.net.cn

JS:   arr.length
来源：http://qwe.cashguo.top

TS:   arr.length
来源：http://rpv.iojbl.cn

Java: list.size();
来源：http://rns.yuanzhike.top

Go:   len(arr)
来源：http://zll.guowangkeji.top

Ruby: arr.length; arr.size
来源：http://qtt.feifeiyinyue.top

C#:   list.Count;
来源：http://zqd.nanxuanxn.top

[D07] 切片 / 取子数组
来源：http://zlh.yuanzhike.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://nec.ivvv.top

PHP:  array_slice($arr, 1, 3);
来源：http://sht.fehbvm.com

JS:   arr.slice(1, 4);
来源：http://efw.fktsv.cn

TS:   arr.slice(1, 4);
来源：http://hsl.daxiang520.top

Java: list.subList(1, 4);
来源：http://fka.jinqigfzy.top

Go:   arr[1:4]
来源：http://int.chenjidiqi.icu

Ruby: arr[1, 3]
来源：http://qyh.vehdjk.com

C#:   list.GetRange(1, 3);
来源：http://cmu.feifeiyinyue.top

[D08] 合并两个数组
来源：http://lgn.chenlongwang.top

Py:   a + b;  a.extend(b)
来源：http://yuw.snrcjt.cn

PHP:  array_merge($a, $b);
来源：http://cut.bbcook.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://aee.yfazqb.com

TS:   [...a, ...b];
来源：http://asj.tarul.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://avy.gaohongyu789.top

Go:   append(a, b...)
来源：http://jgm.ywan-chungtsiang.top

Ruby: a + b;  a.concat(b)
来源：http://ewv.ivvv.top

C#:   a.Concat(b).ToList()
来源：http://udv.yj202588.top

[D09] 排序（升序）
来源：http://fsa.chenjidiqi.icu

Py:   sorted(arr);  arr.sort()
来源：http://xei.ivvv.top

PHP:  sort($arr);
来源：http://qru.vehdjk.com

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://dfn.yongpay.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://tfc.nwbrower.top

Java: Collections.sort(list);  list.sort(null);
来源：http://ubd.fzhhl.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://tfy.fanxiaobao.xyz

Ruby: arr.sort
来源：http://euq.zhaomingkeji.xyz

C#:   list.Sort();
来源：http://krv.nanxuanxn.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://acg.jqgfzy.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://xzs.yongpay.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://bqo.fengsongda.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://noz.hongshengwenyu.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://yqv.yangfankeji.com

Java: list.sort(Comparator.comparing(Person::age));
来源：http://ran.zycfv.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://ghq.fzhhl.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hor.fanxiaobao.xyz

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://qgn.zhaomingkeji.xyz

[D11] 反转数组
来源：http://wkw.jianghu66.top

Py:   arr[::-1];  arr.reverse()
来源：http://pqw.daria6918.cn

PHP:  array_reverse($arr);
来源：http://hmn.9152youxi.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://dnb.ydzc1.top

TS:   [...arr].reverse();
来源：http://fgb.sjlbkw.cn

Java: Collections.reverse(list);
来源：http://kpf.fktsv.cn

Go:   slices.Reverse(arr)
来源：http://oap.ybcxt.top

Ruby: arr.reverse
来源：http://qlz.fktsv.cn

C#:   list.Reverse();
来源：http://zro.c1oappe.top

[D12] 查找元素下标
来源：http://syo.vehdjk.com

Py:   arr.index(x);  x in arr
来源：http://vpc.zhoulong.xyz

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://ozk.cqqwz.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://sxg.ehwqpu.com

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://gly.tianlin.xyz

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://yxg.jinyuanbaomall.cn

Go:   slices.Index(arr, x)
来源：http://ous.jqgufenzy.top

Ruby: arr.index(x)
来源：http://qzw.bbcook.cn

C#:   list.IndexOf(x);
来源：http://maq.bbcook.cn

[D13] 过滤（保留满足条件的）
来源：http://atl.yongpay.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://zev.svipenyu.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://jbs.yongpay.top

JS:   arr.filter(x => x > 3)
来源：http://akj.ivvv.top

TS:   arr.filter(x => x > 3)
来源：http://bjq.ywan-chungtsiang.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://sdq.bjfxy.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://bey.yuanzhike.top

Ruby: arr.select { |x| x > 3 }
来源：http://jxw.xingfuxueyuan.xyz

C#:   list.Where(x => x > 3).ToList()
来源：http://hme.havefunace.top

[D14] 映射转换（每个元素变形）
来源：http://xmq.vqdsnc.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://uep.yueranfly.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://zdr.shanyushiyangtech.top

JS:   arr.map(x => x * 2)
来源：http://cye.epnwcf.com

TS:   arr.map(x => x * 2)
来源：http://cxb.yanxiufei.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://vki.fzhhl.top

Go:   // 手写循环
来源：http://nuc.dianchejie.cn

Ruby: arr.map { |x| x * 2 }
来源：http://pqz.xziqi.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://ytc.zhengqikj.top

[D15] 去重
来源：http://nnl.aizwys.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://vjp.ctjpmb.com

PHP:  array_unique($arr);
来源：http://wzh.hcnkem.com

JS:   [...new Set(arr)]
来源：http://yaz.gaohongyu789.top

TS:   [...new Set(arr)]
来源：http://lnw.jiagoushi.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://sgk.sxryk.cn

Go:   // 用 map[T]struct{} 手写
来源：http://pmb.shanyushiyangtech.top

Ruby: arr.uniq
来源：http://phh.tian-w.cn

C#:   list.Distinct().ToList()
来源：http://lck.daxiang520.top

[D16] 求和与平均值
来源：http://zmr.andypj.xyz

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://trf.zhoulong.xyz

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://svw.mhx1999.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://gcd.haohaochexian.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://xjb.shanyushiyangkeji.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://ubg.shuidangran.top

Go:   // 手写循环累加
来源：http://cow.feifeiyinyue.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://asw.hcnkem.com

C#:   list.Sum();  list.Average()
来源：http://hra.tian-w.cn

[D17] 最大值与最小值
来源：http://frw.quarkkingdee.top

Py:   max(arr);  min(arr)
来源：http://idn.zhiwuduotai.top

PHP:  max($arr);  min($arr);
来源：http://ikl.zdqjudy.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://kmd.dianchejie.cn

TS:   Math.max(...arr);
来源：http://qqt.jqgfzy.top

Java: Collections.max(list);  Collections.min(list);
来源：http://aed.yuxming.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://qin.uphjek.com

Ruby: arr.max;  arr.min
来源：http://vry.yangfankeji.com

C#:   list.Max();  list.Min()
来源：http://afy.chenzaomai.com

[D18] 扁平化嵌套数组
来源：http://yuh.yfazqb.com

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://rag.andypj.xyz

PHP:  array_merge(...$nested);
来源：http://ttt.guannengcc.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://lzj.ybcxt.top

TS:   nested.flat();
来源：http://rcz.guannengcc.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://eon.yj20258.top

Go:   // 手写双层循环
来源：http://nlg.zhiwuduotai.top

Ruby: nested.flatten
来源：http://mxa.jlsjyb.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://zmr.feifeiyinyue.top

[D19] 按字段分组
来源：http://qtc.hnqzz.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://vhu.tianlin.xyz

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://fcf.redwolf501.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://owg.ivvv.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://ejp.hongshengwenyu.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://vhs.yuanzhike.top

Go:   // 手写 map[string][]T
来源：http://lsn.vehdjk.com

Ruby: arr.group_by { |x| x[:type] }
来源：http://lvw.cdnleiting.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://vrp.gzhubu.top

[D20] 统计每个元素出现次数
来源：http://hzt.smart0.xyz

Py:   Counter(arr)
来源：http://wgv.birdmap.top

PHP:  array_count_values($arr);
来源：http://atl.snrcjt.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://xlr.jinyuanbaomall.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://llh.jqgufenzy.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://dyn.yueranfly.top

Go:   // 手写 map[T]int
来源：http://gza.xuetiantiany.cn


<!-- 参考信息 -->