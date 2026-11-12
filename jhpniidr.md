代发 wailian999

Ruby: def total(*nums); nums.sum; end
来源：http://dnu.snrcjt.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://ukb.yj20258888.top

[C04] 命名参数 / 关键字参数
来源：http://npf.ehwqpu.com

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://mpk.xingfuxueyuan.xyz

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://lzi.ydzc1.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://pzi.cheryme.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://ipq.daria6918.cn

Java: // 无：用 Builder 模式或 record
来源：http://mrp.mhx1999.top

Go:   // 无：用配置结构体参数
来源：http://nqm.sjlbkw.cn

Ruby: f(a: 1, b: 2)
来源：http://bhp.xinyue.icu

C#:   f(a: 1, b: 2)
来源：http://qkj.xziqi.cn

[C05] 返回多个值
来源：http://ypx.xziqi.cn

Py:   return a, b
来源：http://ukm.shzxlz.cn

PHP:  return [$a, $b];
来源：http://hfq.feifeiyinyue.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://yra.ydjk.org.cn

TS:   return { a, b };
来源：http://yum.fzhhl.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://ycg.feifeiyinyue.top

Go:   return a, b
来源：http://ded.svipenyu.cn

Ruby: return a, b
来源：http://lxh.zhoulong.xyz

C#:   return (a, b);              // ValueTuple
来源：http://rrg.ivvv.top

[C06] 匿名函数 / lambda
来源：http://han.pengpengdd.cyou

Py:   square = lambda x: x * x
来源：http://lyc.hesvh.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://fde.yj20258888.top

JS:   const square = x => x * x;
来源：http://vgn.uphjek.com

TS:   const square = (x: number): number => x * x;
来源：http://zly.iojbl.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://qtv.cdnleiting.top

Go:   sq := func(x int) int { return x * x }
来源：http://vkz.hnqzz.top

Ruby: square = ->(x) { x * x }
来源：http://cuh.vqdsnc.cn

C#:   Func<int, int> square = x => x * x;
来源：http://xcd.yanxiufei.cn

[C07] 把函数作为参数传入
来源：http://zbx.xuanzx.com

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://joa.zhaomingkeji.xyz

PHP:  array_map("strtoupper", $arr);
来源：http://faz.epnwcf.com

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://zxc.fengsongda.top

TS:   arr.map(String)
来源：http://jtf.cucudq.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://aoh.yuxming.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://era.yangfankeji.com

Ruby: arr.map(&:upcase)
来源：http://hbv.9152youxi.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://nvp.jinghuilouyu.cn

[C08] 闭包
来源：http://rjp.gogol.net.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://rpn.dianchejie.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://zbg.xinyue.icu

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://vww.ydjk.org.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://rij.hysaishi.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://xus.kuanghao11.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://erv.jianghu66.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://zxy.xziqi.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://nyh.pengpengdd.cyou

[C09] 递归
来源：http://jmy.zdqjudy.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://nja.vqdsnc.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://vmw.hnqzz.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wsu.guannengcc.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://iqs.gotoacloud.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://oqm.ivvv.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://jqp.nanxuanxn.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://gea.yuxming.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://pmz.bbcook.cn

[C10] 变量作用域
来源：http://oho.ctjpmb.com

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://kii.hongshengwenyu.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://loa.tianlin.xyz

JS:   let/const 块级作用域，var 函数级作用域
来源：http://mpq.hcnkem.com

TS:   同 JS
来源：http://kes.iojbl.cn

Java: 方法内为块级作用域
来源：http://ybx.fehbvm.com

Go:   花括号块级作用域
来源：http://hjk.meibo888.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://uij.yuanzhike.top

C#:   块级作用域
来源：http://mnd.ydjk.org.cn

[C11] 模块导入与导出
来源：http://peq.fehbvm.com

Py:   from module import func
来源：http://tgy.gotoacloud.top

PHP:  require "file.php";  或 use App\Service;
来源：http://wjs.shanyushiyangtech.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://bnc.ivvv.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://gkh.vehdjk.com

Java: import java.util.List;
来源：http://gss.yanxiufei.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://zxm.wangdashe.top

Ruby: require "json"; require_relative "./util"
来源：http://nfc.jqgfzy.top

C#:   using System.Text;
来源：http://htx.haohaochexian.top

[C12] 立即执行函数 IIFE
来源：http://xzm.cheryme.top

Py:   (lambda: print("run"))()
来源：http://lqe.jqgfzy.top

PHP:  (function () { echo "run"; })();
来源：http://men.mhx1999.top

JS:   (() => { console.log("run"); })();
来源：http://hsp.havefunace.top

TS:   (() => { console.log("run"); })();
来源：http://rat.redwolf501.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://ldj.shuidangran.top

Go:   func() { fmt.Println("run") }()
来源：http://lem.ivvv.top

Ruby: -> { puts "run" }.call
来源：http://yif.ehwqpu.com

C#:   // 无 IIFE：用静态构造函数
来源：http://ahp.birdmap.top

[C13] 类型声明 / 类型注解
来源：http://ubl.quarkkingdee.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://nbb.feifeiyinyue.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://zjp.wangshuangyany.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://zeo.iojbl.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://btg.zycfv.cn

Java: int add(int a, int b) { return a + b; }
来源：http://jlt.wangshuangyany.cn

Go:   func add(a, b int) int
来源：http://jkt.hysaishi.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://erj.haohaochexian.top

C#:   int Add(int a, int b) => a + b;
来源：http://gio.snrcjt.cn

[C14] 泛型函数
来源：http://wrn.sufxvd.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://grt.yvedp.cn

PHP:  // 无泛型
来源：http://uqr.yj202588.top

JS:   // 无泛型
来源：http://bpw.vehdjk.com

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://max.shangyingyoupin.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://bjt.yangfankeji.com

Go:   func First[T any](items []T) T { return items[0] }
来源：http://uwl.zhoulong.xyz

Ruby: # 无泛型
来源：http://xlb.birdmap.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://ofy.ydzc1.top

[C15] 解构 / 展开参数
来源：http://tyf.wangdashe.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://tnw.gotoacloud.top

PHP:  [$a, $b] = $pair;
来源：http://hqf.andypj.xyz

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://npj.jinqigufen.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://zeh.mhx1999.top

Java: // 无解构
来源：http://ifl.pengpengdd.cyou

Go:   // 无解构
来源：http://kqn.aibaodan.cn

Ruby: a, b = pair
来源：http://nkq.shangyingyoupin.top

C#:   var (a, b) = pair;
来源：http://owr.sysykeji.top

[C16] 函数 / 方法重载
来源：http://jsp.yj20258888.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://tmn.fktsv.cn

PHP:  // 无重载
来源：http://cet.xuanzx.com

JS:   // 无重载：靠 arguments.length 分支
来源：http://cwd.mhx1999.top

TS:   // 用联合类型或重载签名声明
来源：http://out.jianghu66.top

Java: void f(int a) {}  void f(String a) {}
来源：http://igm.gzhubu.top

Go:   // 无重载：用不同函数名
来源：http://cbf.yongpay.top

Ruby: # 无重载：靠动态参数
来源：http://upn.shangyingyoupin.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://yzi.cucudq.cn

================================================================================
来源：http://xjl.dianchejie.cn

D. 数组 / 列表 / 集合
来源：http://zqx.cqqwz.cn

================================================================================
来源：http://zei.hywenlv.cn

[D01] 创建数组 / 列表
来源：http://eiv.52xcode.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://ptm.316326.xyz

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://cke.snrcjt.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hak.daria6918.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://ger.0kj1m.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://rpt.zhongyouzk.top

Go:   arr := []int{1, 2, 3}
来源：http://vod.meibo888.top

Ruby: arr = [1, 2, 3]
来源：http://pms.316326.xyz

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://vgu.xylfe.cn

[D02] 追加元素到末尾
来源：http://kwz.sxryk.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://pre.yvedp.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://knk.zhiwuduotai.top

JS:   arr.push(4);
来源：http://eqw.fengsongda.top

TS:   arr.push(4);
来源：http://nwp.nanxinkj.top

Java: list.add(4);
来源：http://cdn.yuxming.cn

Go:   arr = append(arr, 4)
来源：http://hjb.zdqjudy.top

Ruby: arr << 4; arr.push(5)
来源：http://pea.zhijiandao.cn

C#:   list.Add(4);
来源：http://zep.quarkkingdee.top

[D03] 在指定位置插入元素
来源：http://ura.ehwqpu.com

Py:   arr.insert(0, 0)
来源：http://uvi.jinghuilouyu.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://kpk.9152youxi.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://afl.chenlongwang.top

TS:   arr.splice(0, 0, 0);
来源：http://yne.havefunace.top

Java: list.add(0, 0);
来源：http://ogg.andypj.xyz

Go:   arr = append([]int{0}, arr...)
来源：http://wvb.hongshengwenyu.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://vzt.uphjek.com

C#:   list.Insert(0, 0);
来源：http://ecf.fzhhl.top

[D04] 删除元素
来源：http://bgc.yongpay.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://ojj.svipenyu.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://umz.hywenlv.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://yky.zhongyouzk.top

TS:   arr.splice(0, 1);
来源：http://mnl.epnwcf.com

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://zpo.gaohongyu789.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://nbu.bjfxy.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://xzl.cdnleiting.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://yxa.gzhubu.top

[D05] 访问与修改元素
来源：http://plx.bbcook.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://jbi.hongshengwenyu.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://vfh.wangshuangyany.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://kmc.hnqzz.top

TS:   arr[0]; arr.at(-1);
来源：http://dbn.shzxlz.cn

Java: list.get(0); list.set(0, 9);
来源：http://asb.fzhhl.top

Go:   arr[0]; arr[0] = 9
来源：http://kaq.cashguo.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://ssx.shzxlz.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://qmz.fktsv.cn

[D06] 数组长度
来源：http://nzi.ydjk.org.cn

Py:   len(arr)
来源：http://cym.mhx1999.top

PHP:  count($arr);
来源：http://hno.ybcxt.top

JS:   arr.length
来源：http://dcz.jqgfzy.top

TS:   arr.length
来源：http://jnf.zdbjq.cn

Java: list.size();
来源：http://jez.cqqwz.cn

Go:   len(arr)
来源：http://osn.jinyuanbaomall.cn

Ruby: arr.length; arr.size
来源：http://xek.andypj.xyz

C#:   list.Count;
来源：http://tgd.zhongyouzk.top

[D07] 切片 / 取子数组
来源：http://fat.jinqigfzy.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://wsn.pycfn.com

PHP:  array_slice($arr, 1, 3);
来源：http://voi.gaohongyu789.top

JS:   arr.slice(1, 4);
来源：http://vsh.yonumen.top

TS:   arr.slice(1, 4);
来源：http://myn.yonumen.top

Java: list.subList(1, 4);
来源：http://qhl.hongshengwenyu.top

Go:   arr[1:4]
来源：http://jdn.smart0.xyz

Ruby: arr[1, 3]
来源：http://gdz.iojbl.cn

C#:   list.GetRange(1, 3);
来源：http://zgy.xziqi.cn

[D08] 合并两个数组
来源：http://gya.ydzc1.top

Py:   a + b;  a.extend(b)
来源：http://ljg.sufxvd.cn

PHP:  array_merge($a, $b);
来源：http://flk.cucudq.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://mvp.hesvh.cn

TS:   [...a, ...b];
来源：http://uga.bbcook.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://oab.zhixingplan.top

Go:   append(a, b...)
来源：http://azu.yuanzhike.top

Ruby: a + b;  a.concat(b)
来源：http://tvc.iojbl.cn

C#:   a.Concat(b).ToList()
来源：http://uwo.havefunace.top

[D09] 排序（升序）
来源：http://mnb.hfpthk.cn

Py:   sorted(arr);  arr.sort()
来源：http://ekn.zhongyouzk.top

PHP:  sort($arr);
来源：http://nsq.shuidangran.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://xyl.zycfv.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://gau.ybcxt.top

Java: Collections.sort(list);  list.sort(null);
来源：http://jcy.fktsv.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://kdo.cashguo.top

Ruby: arr.sort
来源：http://mam.fengsongda.top

C#:   list.Sort();
来源：http://mbb.xinyue.icu

[D10] 自定义排序（按字段 / 多条件）
来源：http://xwt.zdqjudy.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hbu.hfpthk.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ryb.yvedp.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://mce.tanke756.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://esl.zycfv.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hux.svipenyu.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://ild.quarkkingdee.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hqi.sufxvd.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hti.gotoacloud.top

[D11] 反转数组
来源：http://met.zhoulong.xyz

Py:   arr[::-1];  arr.reverse()
来源：http://lrb.shuidangran.top

PHP:  array_reverse($arr);
来源：http://cwu.zhaomingkeji.xyz

JS:   [...arr].reverse();  arr.toReversed()
来源：http://xwf.bjfxy.top

TS:   [...arr].reverse();
来源：http://ckc.mhx1999.top

Java: Collections.reverse(list);
来源：http://gog.zycfv.cn

Go:   slices.Reverse(arr)
来源：http://jiu.zhoulong.xyz

Ruby: arr.reverse
来源：http://txs.chenjidiqi.icu

C#:   list.Reverse();
来源：http://mpx.fengsongda.top

[D12] 查找元素下标
来源：http://njl.gzhubu.top

Py:   arr.index(x);  x in arr
来源：http://qoq.ybcxt.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://zlv.chenlongwang.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://klx.meibo888.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://aaf.ctjpmb.com

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://ftc.nanxinkj.top

Go:   slices.Index(arr, x)
来源：http://xww.ywan-chungtsiang.top

Ruby: arr.index(x)
来源：http://wsh.aibaodan.cn

C#:   list.IndexOf(x);
来源：http://kqf.guannengcc.top

[D13] 过滤（保留满足条件的）
来源：http://xrb.gogol.net.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://oks.cheryme.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://ykv.gogol.net.cn

JS:   arr.filter(x => x > 3)
来源：http://kyo.wangshuangyany.cn

TS:   arr.filter(x => x > 3)
来源：http://zna.c1oappe.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://vet.gaohongyu789.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://ecx.tianlin.xyz

Ruby: arr.select { |x| x > 3 }
来源：http://yys.jiagoushi.top

C#:   list.Where(x => x > 3).ToList()
来源：http://pwy.zhongyouzk.top

[D14] 映射转换（每个元素变形）
来源：http://wnm.aizwys.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://mou.zdbjq.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://zzi.chenlongwang.top

JS:   arr.map(x => x * 2)
来源：http://tka.vehdjk.com

TS:   arr.map(x => x * 2)
来源：http://cox.dianchejie.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://dge.daria6918.cn

Go:   // 手写循环
来源：http://dpa.yuanzhike.top

Ruby: arr.map { |x| x * 2 }
来源：http://nfn.jqgfzy.top

C#:   list.Select(x => x * 2).ToList()
来源：http://ftn.xingfuxueyuan.xyz

[D15] 去重
来源：http://thl.shzxlz.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://bmq.sufxvd.cn

PHP:  array_unique($arr);
来源：http://axk.hesvh.cn

JS:   [...new Set(arr)]
来源：http://npq.cheryme.top

TS:   [...new Set(arr)]
来源：http://owc.andypj.xyz

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://odq.tianlin.xyz

Go:   // 用 map[T]struct{} 手写
来源：http://lqv.aizwys.cn

Ruby: arr.uniq
来源：http://nrt.shuidangran.top

C#:   list.Distinct().ToList()
来源：http://qxg.yueranfly.top

[D16] 求和与平均值
来源：http://hlc.zhiwuduotai.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://lhg.nanxuanxn.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://zuv.sxryk.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://tlh.tian-w.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hrl.chenlongwang.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://aor.gogol.net.cn

Go:   // 手写循环累加
来源：http://lus.cucudq.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://ptt.redwolf501.top

C#:   list.Sum();  list.Average()
来源：http://wvr.chenzaomai.com

[D17] 最大值与最小值
来源：http://ojb.jianghu66.top

Py:   max(arr);  min(arr)
来源：http://sow.hywenlv.cn

PHP:  max($arr);  min($arr);
来源：http://nmk.yj202588.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://prx.hfpthk.cn

TS:   Math.max(...arr);
来源：http://fwk.jianghu66.top

Java: Collections.max(list);  Collections.min(list);
来源：http://vmq.aizwys.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://vvw.ctjpmb.com

Ruby: arr.max;  arr.min
来源：http://owr.tianlin.xyz

C#:   list.Max();  list.Min()
来源：http://sbw.hywenlv.cn

[D18] 扁平化嵌套数组
来源：http://ofi.dianchejie.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://zol.9152youxi.cn

PHP:  array_merge(...$nested);
来源：http://ulp.jlsjyb.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://epd.pengpengdd.cyou

TS:   nested.flat();
来源：http://kzi.chenlongwang.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://asp.svipenyu.cn

Go:   // 手写双层循环
来源：http://hnr.c1oappe.top

Ruby: nested.flatten
来源：http://lto.yueranfly.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://pff.jinqigufen.top

[D19] 按字段分组
来源：http://ahi.9152youxi.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://sde.ybcxt.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://ckm.jinqigfzy.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://vqr.pengpengdd.cyou

TS:   Object.groupBy(arr, x => x.type)
来源：http://fme.jlsjyb.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://xcf.sxryk.cn

Go:   // 手写 map[string][]T
来源：http://wle.yueranfly.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://jrh.0kj1m.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://wfs.gotoacloud.top

[D20] 统计每个元素出现次数
来源：http://waf.shanyushiyangkeji.top

Py:   Counter(arr)
来源：http://wla.yfazqb.com

PHP:  array_count_values($arr);
来源：http://alo.guannengcc.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://bqt.ctjpmb.com

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://nww.nanxinkj.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://xms.hnxiangtu.top

Go:   // 手写 map[T]int
来源：http://jmf.xinyue.icu


<!-- 参考信息 -->