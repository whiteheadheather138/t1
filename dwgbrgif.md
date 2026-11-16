代发 wailian999

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://zlk.gzhubu.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://vvu.sxryk.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://qbg.haohaochexian.top

Java: // 无：用 Builder 模式或 record
来源：http://wzn.jqgufenzy.top

Go:   // 无：用配置结构体参数
来源：http://jdm.daxiang520.top

Ruby: f(a: 1, b: 2)
来源：http://nvo.fehbvm.com

C#:   f(a: 1, b: 2)
来源：http://gbs.xylfe.cn

[C05] 返回多个值
来源：http://ope.feifeiyinyue.top

Py:   return a, b
来源：http://kmo.jqgfzy.top

PHP:  return [$a, $b];
来源：http://mwc.hongshengwenyu.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://ivy.mhx1999.top

TS:   return { a, b };
来源：http://xhk.snrcjt.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://kzd.xuanzx.com

Go:   return a, b
来源：http://zxo.yuxming.cn

Ruby: return a, b
来源：http://wvl.iojbl.cn

C#:   return (a, b);              // ValueTuple
来源：http://nis.tianlin.xyz

[C06] 匿名函数 / lambda
来源：http://rxd.shanyushiyangtech.top

Py:   square = lambda x: x * x
来源：http://zuq.zdqjudy.top

PHP:  $square = fn($x) => $x * $x;
来源：http://ezp.fktsv.cn

JS:   const square = x => x * x;
来源：http://que.shangyingyoupin.top

TS:   const square = (x: number): number => x * x;
来源：http://mtb.hammf.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://ukh.sufxvd.cn

Go:   sq := func(x int) int { return x * x }
来源：http://obu.yj20258.top

Ruby: square = ->(x) { x * x }
来源：http://fqd.hfpthk.cn

C#:   Func<int, int> square = x => x * x;
来源：http://seo.chenzaomai.com

[C07] 把函数作为参数传入
来源：http://yub.shanyushiyangtech.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://yuh.jyoumei.cn

PHP:  array_map("strtoupper", $arr);
来源：http://yya.aizwys.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://mzd.xziqi.cn

TS:   arr.map(String)
来源：http://huq.tianlin.xyz

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://tpd.quarkkingdee.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://cmm.cqqwz.cn

Ruby: arr.map(&:upcase)
来源：http://swq.zhixingplan.top

C#:   arr.Select(s => s.ToUpper())
来源：http://mka.cheryme.top

[C08] 闭包
来源：http://xzz.zhiwuduotai.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://ftx.zhijiandao.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://fmg.jinghuilouyu.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://gvs.yuxming.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://haz.daxiang520.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://zta.gogol.net.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://egs.zhongyouzk.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://uwh.aibaodan.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://shi.yueranfly.top

[C09] 递归
来源：http://gnu.dashuyun.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://fqw.ywan-chungtsiang.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://qmq.yuxming.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wtr.cucudq.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://jqy.zdbjq.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://lrv.sweek.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://ate.jinghuilouyu.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://sis.dianchejie.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://vyj.andypj.xyz

[C10] 变量作用域
来源：http://dhf.daxiang520.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://zxd.haohaochexian.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://ysb.316326.xyz

JS:   let/const 块级作用域，var 函数级作用域
来源：http://dle.pycfn.com

TS:   同 JS
来源：http://mch.gogol.net.cn

Java: 方法内为块级作用域
来源：http://jyh.vqdsnc.cn

Go:   花括号块级作用域
来源：http://agt.guowangkeji.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://mji.yfazqb.com

C#:   块级作用域
来源：http://iru.havefunace.top

[C11] 模块导入与导出
来源：http://zxz.nanxuanxn.top

Py:   from module import func
来源：http://hze.xuetiantiany.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://olp.jlsjyb.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://cgx.hongshengwenyu.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://tvi.ehwqpu.com

Java: import java.util.List;
来源：http://swc.zhijiandao.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://qou.jqgfzy.top

Ruby: require "json"; require_relative "./util"
来源：http://pik.cheryme.top

C#:   using System.Text;
来源：http://vma.xylfe.cn

[C12] 立即执行函数 IIFE
来源：http://pbw.sjlbkw.cn

Py:   (lambda: print("run"))()
来源：http://twu.jqgfzy.top

PHP:  (function () { echo "run"; })();
来源：http://qtq.jiagoushi.top

JS:   (() => { console.log("run"); })();
来源：http://rms.aibaodan.cn

TS:   (() => { console.log("run"); })();
来源：http://adz.hongshengwenyu.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://szt.fanxiaobao.xyz

Go:   func() { fmt.Println("run") }()
来源：http://oii.jiagoushi.top

Ruby: -> { puts "run" }.call
来源：http://tvz.nanxuanxn.top

C#:   // 无 IIFE：用静态构造函数
来源：http://fdd.shzxlz.cn

[C13] 类型声明 / 类型注解
来源：http://voz.jinghuilouyu.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://prr.smart0.xyz

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://iug.tianlin.xyz

JS:   // 无类型（可用 JSDoc 注释）
来源：http://fvl.nwbrower.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://muz.shuidangran.top

Java: int add(int a, int b) { return a + b; }
来源：http://kek.yj202588.top

Go:   func add(a, b int) int
来源：http://rpx.ydjk.org.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://dxf.andypj.xyz

C#:   int Add(int a, int b) => a + b;
来源：http://rmy.chenzaomai.com

[C14] 泛型函数
来源：http://kpk.cucudq.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://cmz.dashuyun.cn

PHP:  // 无泛型
来源：http://gsx.hfpthk.cn

JS:   // 无泛型
来源：http://iqb.mhx1999.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://ihb.gotoacloud.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://dbr.bbcook.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://nkm.feifeiyinyue.top

Ruby: # 无泛型
来源：http://pgu.ybcxt.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://aze.ywan-chungtsiang.top

[C15] 解构 / 展开参数
来源：http://jpz.gotoacloud.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://xmg.ctjpmb.com

PHP:  [$a, $b] = $pair;
来源：http://drq.aibaodan.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://vdp.jqgufenzy.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://uku.jinghuilouyu.cn

Java: // 无解构
来源：http://mkg.yuxming.cn

Go:   // 无解构
来源：http://prc.ctjpmb.com

Ruby: a, b = pair
来源：http://obb.xziqi.cn

C#:   var (a, b) = pair;
来源：http://ftm.zhixingplan.top

[C16] 函数 / 方法重载
来源：http://fpq.nanxuanxn.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://xze.jlsjyb.cn

PHP:  // 无重载
来源：http://ywa.ctjpmb.com

JS:   // 无重载：靠 arguments.length 分支
来源：http://pdj.ydjk.org.cn

TS:   // 用联合类型或重载签名声明
来源：http://hkb.tarul.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://qij.kuanghao11.cn

Go:   // 无重载：用不同函数名
来源：http://woo.fktsv.cn

Ruby: # 无重载：靠动态参数
来源：http://ajs.xinyue.icu

C#:   void F(int a) {}  void F(string a) {}
来源：http://zve.feifeiyinyue.top

================================================================================
来源：http://iwk.kuanghao11.cn

D. 数组 / 列表 / 集合
来源：http://fho.xuetiantiany.cn

================================================================================
来源：http://egn.ybcxt.top

[D01] 创建数组 / 列表
来源：http://iio.jlsjyb.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://eas.fengsongda.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://qrn.svipenyu.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://exf.cucudq.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://avf.fktsv.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://mmb.hnxiangtu.top

Go:   arr := []int{1, 2, 3}
来源：http://vkj.epnwcf.com

Ruby: arr = [1, 2, 3]
来源：http://qxz.gzhubu.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://gvn.epnwcf.com

[D02] 追加元素到末尾
来源：http://nqh.0kj1m.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://uqm.cashguo.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://byt.gzhubu.top

JS:   arr.push(4);
来源：http://drb.tianlin.xyz

TS:   arr.push(4);
来源：http://cgn.shzxlz.cn

Java: list.add(4);
来源：http://diw.tian-w.cn

Go:   arr = append(arr, 4)
来源：http://vzb.iojbl.cn

Ruby: arr << 4; arr.push(5)
来源：http://lkf.jlsjyb.cn

C#:   list.Add(4);
来源：http://xhq.nanxuanxn.top

[D03] 在指定位置插入元素
来源：http://fwt.xinyue.icu

Py:   arr.insert(0, 0)
来源：http://yom.nanxuanxn.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://ovj.tianlin.xyz

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://lvv.bbcook.cn

TS:   arr.splice(0, 0, 0);
来源：http://ujg.shzxlz.cn

Java: list.add(0, 0);
来源：http://bes.shuidangran.top

Go:   arr = append([]int{0}, arr...)
来源：http://ldz.ydjk.org.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://wiy.ydzc1.top

C#:   list.Insert(0, 0);
来源：http://kov.havefunace.top

[D04] 删除元素
来源：http://jvs.zhaomingkeji.xyz

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://nfd.yongpay.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://sai.haohaochexian.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://sjx.xziqi.cn

TS:   arr.splice(0, 1);
来源：http://siu.ybcxt.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://nul.316326.xyz

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://iea.zhaomingkeji.xyz

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://vvy.quarkkingdee.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://wjw.daria6918.cn

[D05] 访问与修改元素
来源：http://lty.jianghu66.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://riu.fanxiaobao.xyz

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://ffo.fengsongda.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://rsr.dianchejie.cn

TS:   arr[0]; arr.at(-1);
来源：http://phj.yonumen.top

Java: list.get(0); list.set(0, 9);
来源：http://gyo.hnxiangtu.top

Go:   arr[0]; arr[0] = 9
来源：http://gyf.zycfv.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://udg.yuanzhike.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://wvj.yuxming.cn

[D06] 数组长度
来源：http://uww.ehwqpu.com

Py:   len(arr)
来源：http://qww.pengpengdd.cyou

PHP:  count($arr);
来源：http://win.vehdjk.com

JS:   arr.length
来源：http://jky.hywenlv.cn

TS:   arr.length
来源：http://qmk.guannengcc.top

Java: list.size();
来源：http://txf.gotoacloud.top

Go:   len(arr)
来源：http://qnt.jinqigufen.top

Ruby: arr.length; arr.size
来源：http://cgc.hnqzz.top

C#:   list.Count;
来源：http://jnm.hnxiangtu.top

[D07] 切片 / 取子数组
来源：http://dxs.jianghu66.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://nrz.guowangkeji.top

PHP:  array_slice($arr, 1, 3);
来源：http://awm.ppjwa.cn

JS:   arr.slice(1, 4);
来源：http://lve.ppjwa.cn

TS:   arr.slice(1, 4);
来源：http://zut.jinyuanbaomall.cn

Java: list.subList(1, 4);
来源：http://kng.316326.xyz

Go:   arr[1:4]
来源：http://ozw.jinqigufen.top

Ruby: arr[1, 3]
来源：http://hhn.xuetiantiany.cn

C#:   list.GetRange(1, 3);
来源：http://fjp.chenjidiqi.icu

[D08] 合并两个数组
来源：http://lji.hywenlv.cn

Py:   a + b;  a.extend(b)
来源：http://ocq.jiagoushi.top

PHP:  array_merge($a, $b);
来源：http://hpd.jinghuilouyu.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://pju.ctjpmb.com

TS:   [...a, ...b];
来源：http://nqr.yvedp.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://brn.yfazqb.com

Go:   append(a, b...)
来源：http://ast.ppjwa.cn

Ruby: a + b;  a.concat(b)
来源：http://xbm.jqgfzy.top

C#:   a.Concat(b).ToList()
来源：http://pbk.ydjk.org.cn

[D09] 排序（升序）
来源：http://vwv.snrcjt.cn

Py:   sorted(arr);  arr.sort()
来源：http://xpv.nwbrower.top

PHP:  sort($arr);
来源：http://lfo.zdqjudy.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://sqs.0kj1m.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://iow.fzhhl.top

Java: Collections.sort(list);  list.sort(null);
来源：http://ukz.ywan-chungtsiang.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://czo.iojbl.cn

Ruby: arr.sort
来源：http://foc.ppjwa.cn

C#:   list.Sort();
来源：http://dgk.yongpay.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://pdw.nwbrower.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://mzh.ydjk.org.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://cba.gaohongyu789.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://gaj.0kj1m.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://tmn.vehdjk.com

Java: list.sort(Comparator.comparing(Person::age));
来源：http://rrr.ehwqpu.com

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://npj.vehdjk.com

Ruby: arr.sort_by { |x| x[:age] }
来源：http://sit.yanxiufei.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://tkw.xylfe.cn

[D11] 反转数组
来源：http://tqg.hesvh.cn

Py:   arr[::-1];  arr.reverse()
来源：http://jyg.cucudq.cn

PHP:  array_reverse($arr);
来源：http://mog.jinqigufen.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://odu.yfazqb.com

TS:   [...arr].reverse();
来源：http://bdj.xuanzx.com

Java: Collections.reverse(list);
来源：http://pfg.zhaomingkeji.xyz

Go:   slices.Reverse(arr)
来源：http://vys.bbcook.cn

Ruby: arr.reverse
来源：http://hrv.shangyingyoupin.top

C#:   list.Reverse();
来源：http://gfq.xuanzx.com

[D12] 查找元素下标
来源：http://krv.wangshuangyany.cn

Py:   arr.index(x);  x in arr
来源：http://jjq.gotoacloud.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://ufz.shanyushiyangtech.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://htq.dashuyun.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://rrn.wangdashe.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://cpj.yueranfly.top

Go:   slices.Index(arr, x)
来源：http://mnw.wangdashe.top

Ruby: arr.index(x)
来源：http://yav.smart0.xyz

C#:   list.IndexOf(x);
来源：http://eks.316326.xyz

[D13] 过滤（保留满足条件的）
来源：http://dby.hnxiangtu.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://fhz.kuanghao11.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://ziz.nwbrower.top

JS:   arr.filter(x => x > 3)
来源：http://mzh.guowangkeji.top

TS:   arr.filter(x => x > 3)
来源：http://hhm.jqgufenzy.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://tri.yvedp.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://ntm.jiagoushi.top

Ruby: arr.select { |x| x > 3 }
来源：http://vwq.jianghu66.top

C#:   list.Where(x => x > 3).ToList()
来源：http://mem.aibaodan.cn

[D14] 映射转换（每个元素变形）
来源：http://bwa.pycfn.com

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://roq.xingfuxueyuan.xyz

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://dlp.hcnkem.com

JS:   arr.map(x => x * 2)
来源：http://ahg.ehwqpu.com

TS:   arr.map(x => x * 2)
来源：http://ypi.wangdashe.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://sfq.iojbl.cn

Go:   // 手写循环
来源：http://rqv.hnxiangtu.top

Ruby: arr.map { |x| x * 2 }
来源：http://rup.shanyushiyangtech.top

C#:   list.Select(x => x * 2).ToList()
来源：http://dao.birdmap.top

[D15] 去重
来源：http://hnw.nwbrower.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://fbt.gaohongyu789.top

PHP:  array_unique($arr);
来源：http://idd.cheryme.top

JS:   [...new Set(arr)]
来源：http://btz.zdbjq.cn

TS:   [...new Set(arr)]
来源：http://nrr.chenzaomai.com

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://cid.xziqi.cn

Go:   // 用 map[T]struct{} 手写
来源：http://oik.c1oappe.top

Ruby: arr.uniq
来源：http://ddr.mhx1999.top

C#:   list.Distinct().ToList()
来源：http://mvz.jqgfzy.top

[D16] 求和与平均值
来源：http://asl.hnxiangtu.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://ydh.shuidangran.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://ajt.jianghu66.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://giw.zhengqikj.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://wbb.daria6918.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://xfq.zhijiandao.cn

Go:   // 手写循环累加
来源：http://lbr.jqgufenzy.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://xjx.jqgufenzy.top

C#:   list.Sum();  list.Average()
来源：http://xsj.meibo888.top

[D17] 最大值与最小值
来源：http://ugn.xinyue.icu

Py:   max(arr);  min(arr)
来源：http://aza.dianchejie.cn

PHP:  max($arr);  min($arr);
来源：http://jnr.ywan-chungtsiang.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://fwl.nanxuanxn.top

TS:   Math.max(...arr);
来源：http://ftc.hesvh.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://fdu.birdmap.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://olu.jiagoushi.top

Ruby: arr.max;  arr.min
来源：http://ygh.tarul.cn

C#:   list.Max();  list.Min()
来源：http://ttb.ybcxt.top

[D18] 扁平化嵌套数组
来源：http://ivq.fktsv.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://tqd.quarkkingdee.top

PHP:  array_merge(...$nested);
来源：http://irg.svipenyu.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://rzi.xziqi.cn

TS:   nested.flat();
来源：http://crq.hammf.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://mud.tanke756.top

Go:   // 手写双层循环
来源：http://rgy.ywan-chungtsiang.top

Ruby: nested.flatten
来源：http://fle.jinqigfzy.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://non.kuanghao11.cn

[D19] 按字段分组
来源：http://ioq.hywenlv.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://ssz.nwbrower.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://lvi.aibaodan.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://esk.jiagoushi.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://xce.redwolf501.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://cvj.ybcxt.top

Go:   // 手写 map[string][]T
来源：http://yhd.fanxiaobao.xyz

Ruby: arr.group_by { |x| x[:type] }
来源：http://nhs.yfazqb.com

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://cxy.andypj.xyz

[D20] 统计每个元素出现次数
来源：http://ebl.hcnkem.com

Py:   Counter(arr)
来源：http://uay.uphjek.com

PHP:  array_count_values($arr);
来源：http://bbu.wangshuangyany.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://uoy.bjfxy.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://rav.hfpthk.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://zqs.jinghuilouyu.cn

Go:   // 手写 map[T]int
来源：http://czm.9152youxi.cn

Ruby: arr.tally
来源：http://lbn.guannengcc.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://rog.gogol.net.cn

[D21] 判断是否包含某元素
来源：http://hyi.hywenlv.cn

Py:   x in arr
来源：http://cfw.tianlin.xyz


<!-- 参考信息 -->