代发 wailian999

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://evl.zhoulong.xyz

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://elg.bjfxy.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://bzb.gogol.net.cn

Java: // 无：用 Builder 模式或 record
来源：http://wrh.ehwqpu.com

Go:   // 无：用配置结构体参数
来源：http://vbc.vehdjk.com

Ruby: f(a: 1, b: 2)
来源：http://ami.wangshuangyany.cn

C#:   f(a: 1, b: 2)
来源：http://qji.ctjpmb.com

[C05] 返回多个值
来源：http://rjg.316326.xyz

Py:   return a, b
来源：http://sao.tian-w.cn

PHP:  return [$a, $b];
来源：http://mog.shanyushiyangkeji.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://vfa.aizwys.cn

TS:   return { a, b };
来源：http://yih.wangdashe.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://oyy.redwolf501.top

Go:   return a, b
来源：http://lyu.gaohongyu789.top

Ruby: return a, b
来源：http://zag.ctjpmb.com

C#:   return (a, b);              // ValueTuple
来源：http://wnt.jyoumei.cn

[C06] 匿名函数 / lambda
来源：http://egq.fktsv.cn

Py:   square = lambda x: x * x
来源：http://tcs.shangyingyoupin.top

PHP:  $square = fn($x) => $x * $x;
来源：http://vye.hcnkem.com

JS:   const square = x => x * x;
来源：http://wpv.ivvv.top

TS:   const square = (x: number): number => x * x;
来源：http://shh.sweek.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://wuo.haohaochexian.top

Go:   sq := func(x int) int { return x * x }
来源：http://jhv.haohaochexian.top

Ruby: square = ->(x) { x * x }
来源：http://cnc.zdqjudy.top

C#:   Func<int, int> square = x => x * x;
来源：http://rdl.sufxvd.cn

[C07] 把函数作为参数传入
来源：http://rrg.jinghuilouyu.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://ars.xziqi.cn

PHP:  array_map("strtoupper", $arr);
来源：http://iyx.gogol.net.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://jnu.sufxvd.cn

TS:   arr.map(String)
来源：http://mme.fengsongda.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://uvp.guannengcc.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://ccv.9152youxi.cn

Ruby: arr.map(&:upcase)
来源：http://yrv.bbcook.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://akx.316326.xyz

[C08] 闭包
来源：http://lla.nanxinkj.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://nbe.dianchejie.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://gch.yueranfly.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://myb.9152youxi.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://mqu.chenjidiqi.icu

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hgd.bjfxy.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://ikl.gotoacloud.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://ttq.yanxiufei.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://ytj.yangfankeji.com

[C09] 递归
来源：http://lbo.hywenlv.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://ixd.meibo888.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://blh.zhongyouzk.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://tkg.zhengqikj.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://zqh.hysaishi.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://jbg.cashguo.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://lhs.uphjek.com

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://eiq.fehbvm.com

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://ckd.aibaodan.cn

[C10] 变量作用域
来源：http://hze.daxiang520.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://oho.0kj1m.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://ltu.vehdjk.com

JS:   let/const 块级作用域，var 函数级作用域
来源：http://whw.shangyingyoupin.top

TS:   同 JS
来源：http://smq.vehdjk.com

Java: 方法内为块级作用域
来源：http://fzp.vehdjk.com

Go:   花括号块级作用域
来源：http://xhn.havefunace.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://elp.cucudq.cn

C#:   块级作用域
来源：http://nnn.fktsv.cn

[C11] 模块导入与导出
来源：http://hnt.hcnkem.com

Py:   from module import func
来源：http://bql.aizwys.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://inx.cheryme.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://hyb.hysaishi.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://yhd.jqgufenzy.top

Java: import java.util.List;
来源：http://mgw.yj202588.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://xoe.yj20258888.top

Ruby: require "json"; require_relative "./util"
来源：http://mvc.jinqigfzy.top

C#:   using System.Text;
来源：http://not.snrcjt.cn

[C12] 立即执行函数 IIFE
来源：http://iii.jinyuanbaomall.cn

Py:   (lambda: print("run"))()
来源：http://tvc.quarkkingdee.top

PHP:  (function () { echo "run"; })();
来源：http://bnb.sjlbkw.cn

JS:   (() => { console.log("run"); })();
来源：http://mcx.aibaodan.cn

TS:   (() => { console.log("run"); })();
来源：http://lfy.yj20258888.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://wcv.smart0.xyz

Go:   func() { fmt.Println("run") }()
来源：http://xzx.feifeiyinyue.top

Ruby: -> { puts "run" }.call
来源：http://smq.cqqwz.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://vcp.bbcook.cn

[C13] 类型声明 / 类型注解
来源：http://gnk.aizwys.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://vzr.pycfn.com

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://crc.c1oappe.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hjn.yuxming.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ngb.gogol.net.cn

Java: int add(int a, int b) { return a + b; }
来源：http://yxc.chenjidiqi.icu

Go:   func add(a, b int) int
来源：http://jkn.daria6918.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://bqj.shangyingyoupin.top

C#:   int Add(int a, int b) => a + b;
来源：http://uab.yj202588.top

[C14] 泛型函数
来源：http://bup.fanxiaobao.xyz

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://ymv.jyoumei.cn

PHP:  // 无泛型
来源：http://vqj.shzxlz.cn

JS:   // 无泛型
来源：http://bjn.tian-w.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://awx.sysykeji.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://kgf.jyoumei.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://izl.tian-w.cn

Ruby: # 无泛型
来源：http://rlj.cdnleiting.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hli.wangshuangyany.cn

[C15] 解构 / 展开参数
来源：http://kim.epnwcf.com

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://sex.chenzaomai.com

PHP:  [$a, $b] = $pair;
来源：http://zli.epnwcf.com

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://lqh.ctjpmb.com

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://qnx.fengsongda.top

Java: // 无解构
来源：http://kiy.pengpengdd.cyou

Go:   // 无解构
来源：http://opg.hammf.cn

Ruby: a, b = pair
来源：http://ost.chenlongwang.top

C#:   var (a, b) = pair;
来源：http://rtc.zhixingplan.top

[C16] 函数 / 方法重载
来源：http://vfg.chenzaomai.com

Py:   # 无重载：用默认参数或 *args 变通
来源：http://wct.jinqigfzy.top

PHP:  // 无重载
来源：http://msj.hnxiangtu.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://fsi.sjlbkw.cn

TS:   // 用联合类型或重载签名声明
来源：http://waw.quarkkingdee.top

Java: void f(int a) {}  void f(String a) {}
来源：http://slh.wangshuangyany.cn

Go:   // 无重载：用不同函数名
来源：http://kbp.hnqzz.top

Ruby: # 无重载：靠动态参数
来源：http://zcg.9152youxi.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://wdp.chenjidiqi.icu

================================================================================
来源：http://dgc.jinqigufen.top

D. 数组 / 列表 / 集合
来源：http://hta.nwbrower.top

================================================================================
来源：http://xup.nanxuanxn.top

[D01] 创建数组 / 列表
来源：http://ekr.yanxiufei.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://zam.zycfv.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://tog.pengpengdd.cyou

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://new.xuanzx.com

TS:   const arr: number[] = [1, 2, 3];
来源：http://dxb.tian-w.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://kye.ivvv.top

Go:   arr := []int{1, 2, 3}
来源：http://otu.316326.xyz

Ruby: arr = [1, 2, 3]
来源：http://hrx.fktsv.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://bvf.jinqigfzy.top

[D02] 追加元素到末尾
来源：http://pix.ydzc1.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://ilk.redwolf501.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://lih.yuxming.cn

JS:   arr.push(4);
来源：http://hjz.haohaochexian.top

TS:   arr.push(4);
来源：http://opd.xziqi.cn

Java: list.add(4);
来源：http://mrh.gogol.net.cn

Go:   arr = append(arr, 4)
来源：http://fvk.zhongyouzk.top

Ruby: arr << 4; arr.push(5)
来源：http://txp.redwolf501.top

C#:   list.Add(4);
来源：http://mux.shzxlz.cn

[D03] 在指定位置插入元素
来源：http://smo.tarul.cn

Py:   arr.insert(0, 0)
来源：http://nxf.uphjek.com

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://ljp.cdnleiting.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://vfv.0kj1m.cn

TS:   arr.splice(0, 0, 0);
来源：http://szr.yongpay.top

Java: list.add(0, 0);
来源：http://kna.hnxiangtu.top

Go:   arr = append([]int{0}, arr...)
来源：http://fhx.aibaodan.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://gld.yongpay.top

C#:   list.Insert(0, 0);
来源：http://hjo.jinyuanbaomall.cn

[D04] 删除元素
来源：http://kuc.zhoulong.xyz

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://rfc.bjfxy.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://gnz.sufxvd.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://tuq.zhaomingkeji.xyz

TS:   arr.splice(0, 1);
来源：http://shq.cashguo.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://ylq.bjfxy.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://rhm.zhengqikj.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://djb.hysaishi.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://tgc.jinqigufen.top

[D05] 访问与修改元素
来源：http://vry.daxiang520.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://mcv.zdqjudy.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://nkw.zhoulong.xyz

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://pqo.havefunace.top

TS:   arr[0]; arr.at(-1);
来源：http://hvt.cdnleiting.top

Java: list.get(0); list.set(0, 9);
来源：http://vbu.birdmap.top

Go:   arr[0]; arr[0] = 9
来源：http://vqi.tianlin.xyz

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://gra.yj20258888.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://qep.jinghuilouyu.cn

[D06] 数组长度
来源：http://twb.svipenyu.cn

Py:   len(arr)
来源：http://qsp.9152youxi.cn

PHP:  count($arr);
来源：http://ule.ehwqpu.com

JS:   arr.length
来源：http://tjq.shanyushiyangkeji.top

TS:   arr.length
来源：http://bkw.jinyuanbaomall.cn

Java: list.size();
来源：http://koy.epnwcf.com

Go:   len(arr)
来源：http://qhx.tian-w.cn

Ruby: arr.length; arr.size
来源：http://oqn.tarul.cn

C#:   list.Count;
来源：http://ogz.gotoacloud.top

[D07] 切片 / 取子数组
来源：http://tiz.zhixingplan.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://pza.jlsjyb.cn

PHP:  array_slice($arr, 1, 3);
来源：http://blk.shzxlz.cn

JS:   arr.slice(1, 4);
来源：http://qho.gaohongyu789.top

TS:   arr.slice(1, 4);
来源：http://wav.hongshengwenyu.top

Java: list.subList(1, 4);
来源：http://yii.daxiang520.top

Go:   arr[1:4]
来源：http://nbi.hnqzz.top

Ruby: arr[1, 3]
来源：http://wqj.bbcook.cn

C#:   list.GetRange(1, 3);
来源：http://kjw.cqqwz.cn

[D08] 合并两个数组
来源：http://roy.zycfv.cn

Py:   a + b;  a.extend(b)
来源：http://hyv.zhixingplan.top

PHP:  array_merge($a, $b);
来源：http://juv.vehdjk.com

JS:   [...a, ...b];  a.concat(b);
来源：http://vnw.zycfv.cn

TS:   [...a, ...b];
来源：http://pcr.havefunace.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://dyi.52xcode.cn

Go:   append(a, b...)
来源：http://gkl.hcnkem.com

Ruby: a + b;  a.concat(b)
来源：http://yqn.zhiwuduotai.top

C#:   a.Concat(b).ToList()
来源：http://crm.sweek.top

[D09] 排序（升序）
来源：http://mdx.fktsv.cn

Py:   sorted(arr);  arr.sort()
来源：http://oeu.jinyuanbaomall.cn

PHP:  sort($arr);
来源：http://yzk.tanke756.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://ygj.vqdsnc.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://cla.pycfn.com

Java: Collections.sort(list);  list.sort(null);
来源：http://xca.uphjek.com

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://pmz.kuanghao11.cn

Ruby: arr.sort
来源：http://eat.hnxiangtu.top

C#:   list.Sort();
来源：http://ybo.0kj1m.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://fjn.aizwys.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://cws.jinyuanbaomall.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ycw.shzxlz.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://wdg.yuanzhike.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://uyk.wangdashe.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://nrh.cdnleiting.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://upg.guannengcc.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://ppg.chenjidiqi.icu

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://zzm.ydzc1.top

[D11] 反转数组
来源：http://ybb.smart0.xyz

Py:   arr[::-1];  arr.reverse()
来源：http://ast.jqgfzy.top

PHP:  array_reverse($arr);
来源：http://vjw.epnwcf.com

JS:   [...arr].reverse();  arr.toReversed()
来源：http://xbp.gzhubu.top

TS:   [...arr].reverse();
来源：http://loy.yj20258.top

Java: Collections.reverse(list);
来源：http://urg.zhengqikj.top

Go:   slices.Reverse(arr)
来源：http://lhz.fengsongda.top

Ruby: arr.reverse
来源：http://lzq.shanyushiyangtech.top

C#:   list.Reverse();
来源：http://nuh.shangyingyoupin.top

[D12] 查找元素下标
来源：http://rbu.ybcxt.top

Py:   arr.index(x);  x in arr
来源：http://ooj.ctjpmb.com

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://itf.zhiwuduotai.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://dyf.jinqigufen.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://fqg.hysaishi.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://doq.chenzaomai.com

Go:   slices.Index(arr, x)
来源：http://cez.tianlin.xyz

Ruby: arr.index(x)
来源：http://otf.zhaomingkeji.xyz

C#:   list.IndexOf(x);
来源：http://hbp.bbcook.cn

[D13] 过滤（保留满足条件的）
来源：http://pkg.yj20258.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://pzu.kuanghao11.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://ipd.kuanghao11.cn

JS:   arr.filter(x => x > 3)
来源：http://awf.gzhubu.top

TS:   arr.filter(x => x > 3)
来源：http://tbx.yangfankeji.com

Java: list.stream().filter(x -> x > 3).toList()
来源：http://usq.gogol.net.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://kpu.hysaishi.cn

Ruby: arr.select { |x| x > 3 }
来源：http://vxl.cqqwz.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://lob.shanyushiyangtech.top

[D14] 映射转换（每个元素变形）
来源：http://bje.redwolf501.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://gkq.smart0.xyz

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://qxn.zhengqikj.top

JS:   arr.map(x => x * 2)
来源：http://lws.zhiwuduotai.top

TS:   arr.map(x => x * 2)
来源：http://ooy.jiagoushi.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://uwz.vqdsnc.cn

Go:   // 手写循环
来源：http://gbh.0kj1m.cn

Ruby: arr.map { |x| x * 2 }
来源：http://pjv.yj20258888.top

C#:   list.Select(x => x * 2).ToList()
来源：http://qpx.c1oappe.top

[D15] 去重
来源：http://lmk.xylfe.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://vpr.hfpthk.cn

PHP:  array_unique($arr);
来源：http://lso.cdnleiting.top

JS:   [...new Set(arr)]
来源：http://wnr.cheryme.top

TS:   [...new Set(arr)]
来源：http://pzo.hammf.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://qfu.hfpthk.cn

Go:   // 用 map[T]struct{} 手写
来源：http://jqy.yuanzhike.top

Ruby: arr.uniq
来源：http://xnf.hnqzz.top

C#:   list.Distinct().ToList()
来源：http://vsz.chenjidiqi.icu

[D16] 求和与平均值
来源：http://ncr.daria6918.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://rqz.jyoumei.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://luz.zhongyouzk.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://qaj.fehbvm.com

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://bns.ybcxt.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://pgk.vqdsnc.cn

Go:   // 手写循环累加
来源：http://vud.snrcjt.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://ksr.aibaodan.cn

C#:   list.Sum();  list.Average()
来源：http://edd.chenlongwang.top

[D17] 最大值与最小值
来源：http://tzx.chenjidiqi.icu

Py:   max(arr);  min(arr)
来源：http://hgn.wangdashe.top

PHP:  max($arr);  min($arr);
来源：http://dhg.yonumen.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://egv.fanxiaobao.xyz

TS:   Math.max(...arr);
来源：http://gis.jyoumei.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://axv.yuanzhike.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://gww.yanxiufei.cn

Ruby: arr.max;  arr.min
来源：http://rxt.yj202588.top

C#:   list.Max();  list.Min()
来源：http://vxf.dianchejie.cn

[D18] 扁平化嵌套数组
来源：http://fyo.bjfxy.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://whh.hesvh.cn

PHP:  array_merge(...$nested);
来源：http://jtj.jiagoushi.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://mcn.zhengqikj.top

TS:   nested.flat();
来源：http://vrl.gzhubu.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://rjy.xinyue.icu

Go:   // 手写双层循环
来源：http://vap.52xcode.cn

Ruby: nested.flatten
来源：http://ler.yongpay.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://yvr.yfazqb.com

[D19] 按字段分组
来源：http://jup.chenlongwang.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://mlb.hnqzz.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://jdx.ywan-chungtsiang.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://rlx.zhaomingkeji.xyz

TS:   Object.groupBy(arr, x => x.type)
来源：http://rwt.vehdjk.com

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://pwk.birdmap.top

Go:   // 手写 map[string][]T
来源：http://jub.bbcook.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://ojd.gogol.net.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://zaw.guowangkeji.top

[D20] 统计每个元素出现次数
来源：http://jll.nanxuanxn.top

Py:   Counter(arr)
来源：http://ziy.ppjwa.cn

PHP:  array_count_values($arr);
来源：http://vfs.hywenlv.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hhp.redwolf501.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://nyv.52xcode.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://ayp.zdbjq.cn

Go:   // 手写 map[T]int
来源：http://ndx.c1oappe.top

Ruby: arr.tally
来源：http://aiv.jyoumei.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://vhu.sxryk.cn

[D21] 判断是否包含某元素
来源：http://kic.zhaomingkeji.xyz

Py:   x in arr
来源：http://mgy.nanxinkj.top


<!-- 参考信息 -->