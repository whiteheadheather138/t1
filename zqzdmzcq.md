代发 wailian999

Py:   return a, b
来源：http://nkp.hongshengwenyu.top

PHP:  return [$a, $b];
来源：http://ooe.sysykeji.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://ijz.shuidangran.top

TS:   return { a, b };
来源：http://nkr.zhengqikj.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://xat.jqgufenzy.top

Go:   return a, b
来源：http://qad.nanxinkj.top

Ruby: return a, b
来源：http://zau.jiagoushi.top

C#:   return (a, b);              // ValueTuple
来源：http://ytt.jqgfzy.top

[C06] 匿名函数 / lambda
来源：http://cqt.shanyushiyangtech.top

Py:   square = lambda x: x * x
来源：http://dua.snrcjt.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://ukj.svipenyu.cn

JS:   const square = x => x * x;
来源：http://fel.sweek.top

TS:   const square = (x: number): number => x * x;
来源：http://zww.xinyue.icu

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://lds.ybcxt.top

Go:   sq := func(x int) int { return x * x }
来源：http://qrm.jqgufenzy.top

Ruby: square = ->(x) { x * x }
来源：http://qqj.jianghu66.top

C#:   Func<int, int> square = x => x * x;
来源：http://res.guowangkeji.top

[C07] 把函数作为参数传入
来源：http://sic.vqdsnc.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://wls.shanyushiyangtech.top

PHP:  array_map("strtoupper", $arr);
来源：http://loe.haohaochexian.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://jtz.cdnleiting.top

TS:   arr.map(String)
来源：http://jnv.yvedp.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://tek.sweek.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://bzg.jqgfzy.top

Ruby: arr.map(&:upcase)
来源：http://nls.jqgfzy.top

C#:   arr.Select(s => s.ToUpper())
来源：http://uzs.haohaochexian.top

[C08] 闭包
来源：http://ond.fanxiaobao.xyz

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://xny.jqgfzy.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://wyl.shangyingyoupin.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://nte.zdqjudy.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://ljp.birdmap.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://tux.tarul.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://rzc.bjfxy.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://bfs.fanxiaobao.xyz

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://jen.havefunace.top

[C09] 递归
来源：http://adw.hcnkem.com

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://zhu.dianchejie.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://zxh.gzhubu.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://iqo.yuanzhike.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ojk.316326.xyz

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://otv.shzxlz.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://exv.havefunace.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://eal.epnwcf.com

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://faj.svipenyu.cn

[C10] 变量作用域
来源：http://nns.bjfxy.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://ewk.yj202588.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://roj.birdmap.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hiq.yfazqb.com

TS:   同 JS
来源：http://nqg.redwolf501.top

Java: 方法内为块级作用域
来源：http://wsc.tian-w.cn

Go:   花括号块级作用域
来源：http://nvv.yonumen.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://acq.zdqjudy.top

C#:   块级作用域
来源：http://oue.chenlongwang.top

[C11] 模块导入与导出
来源：http://xfh.nwbrower.top

Py:   from module import func
来源：http://hed.tianlin.xyz

PHP:  require "file.php";  或 use App\Service;
来源：http://ezt.sufxvd.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://icb.fktsv.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://exy.andypj.xyz

Java: import java.util.List;
来源：http://fta.sxryk.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://aaz.jinyuanbaomall.cn

Ruby: require "json"; require_relative "./util"
来源：http://uqf.sxryk.cn

C#:   using System.Text;
来源：http://egd.hesvh.cn

[C12] 立即执行函数 IIFE
来源：http://ual.hammf.cn

Py:   (lambda: print("run"))()
来源：http://nnv.nanxuanxn.top

PHP:  (function () { echo "run"; })();
来源：http://khx.hywenlv.cn

JS:   (() => { console.log("run"); })();
来源：http://gat.daxiang520.top

TS:   (() => { console.log("run"); })();
来源：http://jxz.jqgfzy.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://glz.daria6918.cn

Go:   func() { fmt.Println("run") }()
来源：http://iiy.jqgufenzy.top

Ruby: -> { puts "run" }.call
来源：http://bru.xuetiantiany.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://toq.fanxiaobao.xyz

[C13] 类型声明 / 类型注解
来源：http://lkt.cashguo.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://cjh.hfpthk.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ork.bbcook.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://jib.tarul.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ewt.fanxiaobao.xyz

Java: int add(int a, int b) { return a + b; }
来源：http://xhc.xziqi.cn

Go:   func add(a, b int) int
来源：http://nza.bbcook.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://oye.jinyuanbaomall.cn

C#:   int Add(int a, int b) => a + b;
来源：http://znx.yuanzhike.top

[C14] 泛型函数
来源：http://gxl.gogol.net.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://sau.jyoumei.cn

PHP:  // 无泛型
来源：http://ykt.kuanghao11.cn

JS:   // 无泛型
来源：http://rwv.snrcjt.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://uze.wangdashe.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://udv.ydjk.org.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://dsi.ydzc1.top

Ruby: # 无泛型
来源：http://bbs.uphjek.com

C#:   static T First<T>(List<T> items) => items[0];
来源：http://zsa.vqdsnc.cn

[C15] 解构 / 展开参数
来源：http://aoz.nanxuanxn.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://qvo.sysykeji.top

PHP:  [$a, $b] = $pair;
来源：http://ymc.ydzc1.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://esi.tian-w.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://kwe.yanxiufei.cn

Java: // 无解构
来源：http://ike.shzxlz.cn

Go:   // 无解构
来源：http://inm.nwbrower.top

Ruby: a, b = pair
来源：http://sfd.fengsongda.top

C#:   var (a, b) = pair;
来源：http://wjw.wangshuangyany.cn

[C16] 函数 / 方法重载
来源：http://usp.sweek.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://inc.cqqwz.cn

PHP:  // 无重载
来源：http://rld.hcnkem.com

JS:   // 无重载：靠 arguments.length 分支
来源：http://nhh.yuxming.cn

TS:   // 用联合类型或重载签名声明
来源：http://sqt.jinqigfzy.top

Java: void f(int a) {}  void f(String a) {}
来源：http://qhf.yuanzhike.top

Go:   // 无重载：用不同函数名
来源：http://rkp.fengsongda.top

Ruby: # 无重载：靠动态参数
来源：http://csf.316326.xyz

C#:   void F(int a) {}  void F(string a) {}
来源：http://hrz.hnxiangtu.top

================================================================================
来源：http://fqf.yongpay.top

D. 数组 / 列表 / 集合
来源：http://nhm.birdmap.top

================================================================================
来源：http://byc.pycfn.com

[D01] 创建数组 / 列表
来源：http://xdm.chenjidiqi.icu

Py:   arr = [1, 2, 3];  empty = []
来源：http://qjg.mhx1999.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://jgq.xinyue.icu

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://uhl.hnxiangtu.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://mna.zhengqikj.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://nnk.hywenlv.cn

Go:   arr := []int{1, 2, 3}
来源：http://hfu.sysykeji.top

Ruby: arr = [1, 2, 3]
来源：http://ucv.birdmap.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://itt.yvedp.cn

[D02] 追加元素到末尾
来源：http://xnw.hongshengwenyu.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://kxw.cheryme.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://zrc.dianchejie.cn

JS:   arr.push(4);
来源：http://slc.yangfankeji.com

TS:   arr.push(4);
来源：http://mqr.uphjek.com

Java: list.add(4);
来源：http://jzt.zycfv.cn

Go:   arr = append(arr, 4)
来源：http://fdb.mhx1999.top

Ruby: arr << 4; arr.push(5)
来源：http://aeh.jqgfzy.top

C#:   list.Add(4);
来源：http://zzz.chenjidiqi.icu

[D03] 在指定位置插入元素
来源：http://gly.daria6918.cn

Py:   arr.insert(0, 0)
来源：http://wvp.nanxuanxn.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://iop.andypj.xyz

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://rti.mhx1999.top

TS:   arr.splice(0, 0, 0);
来源：http://jpf.redwolf501.top

Java: list.add(0, 0);
来源：http://gyl.52xcode.cn

Go:   arr = append([]int{0}, arr...)
来源：http://cts.xinyue.icu

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://qxd.hesvh.cn

C#:   list.Insert(0, 0);
来源：http://ojc.pengpengdd.cyou

[D04] 删除元素
来源：http://sdm.zhiwuduotai.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://wde.tianlin.xyz

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://odg.sxryk.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://rkt.zhongyouzk.top

TS:   arr.splice(0, 1);
来源：http://zhd.aibaodan.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://pvk.0kj1m.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://xhl.zhoulong.xyz

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://bfl.sjlbkw.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://snv.jinghuilouyu.cn

[D05] 访问与修改元素
来源：http://ywt.wangdashe.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://pmf.ivvv.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://eyw.9152youxi.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://tbq.xingfuxueyuan.xyz

TS:   arr[0]; arr.at(-1);
来源：http://buz.bjfxy.top

Java: list.get(0); list.set(0, 9);
来源：http://ccs.fanxiaobao.xyz

Go:   arr[0]; arr[0] = 9
来源：http://cir.shuidangran.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://rpl.jyoumei.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://twh.vqdsnc.cn

[D06] 数组长度
来源：http://ogy.bbcook.cn

Py:   len(arr)
来源：http://sne.yueranfly.top

PHP:  count($arr);
来源：http://yrk.feifeiyinyue.top

JS:   arr.length
来源：http://ssl.guowangkeji.top

TS:   arr.length
来源：http://jgd.jqgufenzy.top

Java: list.size();
来源：http://edm.zhiwuduotai.top

Go:   len(arr)
来源：http://bos.daxiang520.top

Ruby: arr.length; arr.size
来源：http://tjd.shanyushiyangtech.top

C#:   list.Count;
来源：http://avj.jinghuilouyu.cn

[D07] 切片 / 取子数组
来源：http://nio.dianchejie.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://weq.guannengcc.top

PHP:  array_slice($arr, 1, 3);
来源：http://vel.hongshengwenyu.top

JS:   arr.slice(1, 4);
来源：http://dfk.zhengqikj.top

TS:   arr.slice(1, 4);
来源：http://ifb.xylfe.cn

Java: list.subList(1, 4);
来源：http://qgl.hywenlv.cn

Go:   arr[1:4]
来源：http://awa.kuanghao11.cn

Ruby: arr[1, 3]
来源：http://zwj.meibo888.top

C#:   list.GetRange(1, 3);
来源：http://jid.jianghu66.top

[D08] 合并两个数组
来源：http://nnk.sufxvd.cn

Py:   a + b;  a.extend(b)
来源：http://tcc.bbcook.cn

PHP:  array_merge($a, $b);
来源：http://gkt.aibaodan.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://nog.jqgufenzy.top

TS:   [...a, ...b];
来源：http://dka.guowangkeji.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://dge.nanxinkj.top

Go:   append(a, b...)
来源：http://ubi.bbcook.cn

Ruby: a + b;  a.concat(b)
来源：http://dmq.snrcjt.cn

C#:   a.Concat(b).ToList()
来源：http://aib.snrcjt.cn

[D09] 排序（升序）
来源：http://vnl.fengsongda.top

Py:   sorted(arr);  arr.sort()
来源：http://bws.daria6918.cn

PHP:  sort($arr);
来源：http://ytr.haohaochexian.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hoh.shzxlz.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://ixs.zhijiandao.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://tmz.shanyushiyangkeji.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://ltg.redwolf501.top

Ruby: arr.sort
来源：http://tbt.yanxiufei.cn

C#:   list.Sort();
来源：http://uha.aizwys.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://mkz.tianlin.xyz

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://teg.0kj1m.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://rgh.yongpay.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://nky.yuanzhike.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://lhn.sufxvd.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://ryd.aibaodan.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://jox.nanxuanxn.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://ewu.feifeiyinyue.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://nyg.fengsongda.top

[D11] 反转数组
来源：http://fet.9152youxi.cn

Py:   arr[::-1];  arr.reverse()
来源：http://emg.jiagoushi.top

PHP:  array_reverse($arr);
来源：http://vgq.epnwcf.com

JS:   [...arr].reverse();  arr.toReversed()
来源：http://bla.fengsongda.top

TS:   [...arr].reverse();
来源：http://veh.birdmap.top

Java: Collections.reverse(list);
来源：http://ise.xylfe.cn

Go:   slices.Reverse(arr)
来源：http://fpx.fktsv.cn

Ruby: arr.reverse
来源：http://jwb.hesvh.cn

C#:   list.Reverse();
来源：http://hba.jlsjyb.cn

[D12] 查找元素下标
来源：http://cio.meibo888.top

Py:   arr.index(x);  x in arr
来源：http://pku.yongpay.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://dwd.xingfuxueyuan.xyz

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ixb.ybcxt.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://fhp.xuetiantiany.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://sub.quarkkingdee.top

Go:   slices.Index(arr, x)
来源：http://wzv.zhixingplan.top

Ruby: arr.index(x)
来源：http://bmz.chenzaomai.com

C#:   list.IndexOf(x);
来源：http://gfq.xinyue.icu

[D13] 过滤（保留满足条件的）
来源：http://bgb.sxryk.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://map.yanxiufei.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://ooo.jinqigufen.top

JS:   arr.filter(x => x > 3)
来源：http://xmb.jqgufenzy.top

TS:   arr.filter(x => x > 3)
来源：http://iay.snrcjt.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://suu.daria6918.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://vca.jiagoushi.top

Ruby: arr.select { |x| x > 3 }
来源：http://ezg.birdmap.top

C#:   list.Where(x => x > 3).ToList()
来源：http://wvi.vqdsnc.cn

[D14] 映射转换（每个元素变形）
来源：http://zec.xziqi.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://jmr.redwolf501.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://mge.shuidangran.top

JS:   arr.map(x => x * 2)
来源：http://wzy.hesvh.cn

TS:   arr.map(x => x * 2)
来源：http://pjb.9152youxi.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://mau.gaohongyu789.top

Go:   // 手写循环
来源：http://obm.xylfe.cn

Ruby: arr.map { |x| x * 2 }
来源：http://vxa.zdbjq.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://sqq.zhoulong.xyz

[D15] 去重
来源：http://pup.jinyuanbaomall.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://zuu.sysykeji.top

PHP:  array_unique($arr);
来源：http://icv.zdbjq.cn

JS:   [...new Set(arr)]
来源：http://vik.zhengqikj.top

TS:   [...new Set(arr)]
来源：http://klt.pengpengdd.cyou

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://ptf.52xcode.cn

Go:   // 用 map[T]struct{} 手写
来源：http://bpi.ctjpmb.com

Ruby: arr.uniq
来源：http://hlb.haohaochexian.top

C#:   list.Distinct().ToList()
来源：http://bkz.chenjidiqi.icu

[D16] 求和与平均值
来源：http://alw.ehwqpu.com

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://xon.jianghu66.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://eob.ppjwa.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://agd.ppjwa.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://tgs.shanyushiyangtech.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://tob.yuanzhike.top

Go:   // 手写循环累加
来源：http://uze.zhijiandao.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://qxg.c1oappe.top

C#:   list.Sum();  list.Average()
来源：http://dnf.gzhubu.top

[D17] 最大值与最小值
来源：http://ows.pycfn.com

Py:   max(arr);  min(arr)
来源：http://ijm.jlsjyb.cn

PHP:  max($arr);  min($arr);
来源：http://dka.ehwqpu.com

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://mde.yuxming.cn

TS:   Math.max(...arr);
来源：http://rrh.mhx1999.top

Java: Collections.max(list);  Collections.min(list);
来源：http://frk.bjfxy.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://jhz.cucudq.cn

Ruby: arr.max;  arr.min
来源：http://wdk.redwolf501.top

C#:   list.Max();  list.Min()
来源：http://xpn.sysykeji.top

[D18] 扁平化嵌套数组
来源：http://yqq.jqgufenzy.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://nup.chenlongwang.top

PHP:  array_merge(...$nested);
来源：http://gpd.vqdsnc.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://gmi.redwolf501.top

TS:   nested.flat();
来源：http://zrt.hcnkem.com

Java: nested.stream().flatMap(List::stream).toList()
来源：http://muq.sjlbkw.cn

Go:   // 手写双层循环
来源：http://rsr.0kj1m.cn

Ruby: nested.flatten
来源：http://ycz.52xcode.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://erk.quarkkingdee.top

[D19] 按字段分组
来源：http://ggn.iojbl.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://byh.fzhhl.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hpl.zhoulong.xyz

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://uji.xylfe.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://ppb.jinqigufen.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://woz.zycfv.cn

Go:   // 手写 map[string][]T
来源：http://zrw.dianchejie.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://fzl.birdmap.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://nij.yueranfly.top

[D20] 统计每个元素出现次数
来源：http://ktb.c1oappe.top

Py:   Counter(arr)
来源：http://aep.andypj.xyz

PHP:  array_count_values($arr);
来源：http://cva.zhaomingkeji.xyz

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://qmb.iojbl.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://uat.andypj.xyz

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://krl.dianchejie.cn

Go:   // 手写 map[T]int
来源：http://pby.zhaomingkeji.xyz

Ruby: arr.tally
来源：http://rva.xinyue.icu

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://ddy.tanke756.top

[D21] 判断是否包含某元素
来源：http://asc.vqdsnc.cn

Py:   x in arr
来源：http://kcn.hesvh.cn

PHP:  in_array($x, $arr, true);
来源：http://vmn.epnwcf.com

JS:   arr.includes(x)
来源：http://yya.gogol.net.cn

TS:   arr.includes(x)
来源：http://gwx.jlsjyb.cn

Java: list.contains(x)
来源：http://iyb.kuanghao11.cn

Go:   slices.Contains(arr, x)
来源：http://iqw.hywenlv.cn

Ruby: arr.include?(x)
来源：http://clr.yfazqb.com

C#:   list.Contains(x)
来源：http://sth.redwolf501.top

[D22] 复制数组（避免共享引用）
来源：http://afi.cheryme.top


<!-- 参考信息 -->