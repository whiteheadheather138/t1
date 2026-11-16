代发 wailian999

Ruby: def total(*nums); nums.sum; end
来源：http://rcw.hnqzz.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://jlf.guannengcc.top

[C04] 命名参数 / 关键字参数
来源：http://kbx.ywan-chungtsiang.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://auh.fengsongda.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://cko.shuidangran.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://rww.hammf.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://ubc.chenlongwang.top

Java: // 无：用 Builder 模式或 record
来源：http://bgo.kuanghao11.cn

Go:   // 无：用配置结构体参数
来源：http://drx.zhijiandao.cn

Ruby: f(a: 1, b: 2)
来源：http://vpr.zycfv.cn

C#:   f(a: 1, b: 2)
来源：http://wmj.jinqigufen.top

[C05] 返回多个值
来源：http://xmn.chenlongwang.top

Py:   return a, b
来源：http://rjn.zhongyouzk.top

PHP:  return [$a, $b];
来源：http://tob.ybcxt.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://veh.zhoulong.xyz

TS:   return { a, b };
来源：http://hzy.yj20258.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://oxy.mhx1999.top

Go:   return a, b
来源：http://lve.iojbl.cn

Ruby: return a, b
来源：http://rhk.xuetiantiany.cn

C#:   return (a, b);              // ValueTuple
来源：http://pwi.wangdashe.top

[C06] 匿名函数 / lambda
来源：http://ynm.ivvv.top

Py:   square = lambda x: x * x
来源：http://cyo.fzhhl.top

PHP:  $square = fn($x) => $x * $x;
来源：http://ldn.yuxming.cn

JS:   const square = x => x * x;
来源：http://vrf.sysykeji.top

TS:   const square = (x: number): number => x * x;
来源：http://cdh.shzxlz.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://jzy.fehbvm.com

Go:   sq := func(x int) int { return x * x }
来源：http://taj.jinyuanbaomall.cn

Ruby: square = ->(x) { x * x }
来源：http://jwo.jinghuilouyu.cn

C#:   Func<int, int> square = x => x * x;
来源：http://jih.guowangkeji.top

[C07] 把函数作为参数传入
来源：http://izn.daxiang520.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://gnc.meibo888.top

PHP:  array_map("strtoupper", $arr);
来源：http://gxa.316326.xyz

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://xjh.birdmap.top

TS:   arr.map(String)
来源：http://qln.shzxlz.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://wdb.zdqjudy.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://tuf.cdnleiting.top

Ruby: arr.map(&:upcase)
来源：http://ucm.aibaodan.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://mgf.uphjek.com

[C08] 闭包
来源：http://env.guannengcc.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://mzi.nwbrower.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://xwn.52xcode.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://gwf.yj20258.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://ncm.hfpthk.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://kcm.tian-w.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://eka.shanyushiyangtech.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://zlx.xingfuxueyuan.xyz

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://qxl.pengpengdd.cyou

[C09] 递归
来源：http://url.ctjpmb.com

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://uvt.yvedp.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://whe.guowangkeji.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ejo.0kj1m.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ypr.xingfuxueyuan.xyz

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://qri.nanxinkj.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://amy.nanxuanxn.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hcy.fengsongda.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://fkq.hnxiangtu.top

[C10] 变量作用域
来源：http://sfp.ppjwa.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://eow.shanyushiyangkeji.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://msd.jinqigfzy.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://zvs.andypj.xyz

TS:   同 JS
来源：http://elb.yuxming.cn

Java: 方法内为块级作用域
来源：http://olt.chenzaomai.com

Go:   花括号块级作用域
来源：http://xmk.cashguo.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://msd.chenlongwang.top

C#:   块级作用域
来源：http://hmf.haohaochexian.top

[C11] 模块导入与导出
来源：http://qtb.gaohongyu789.top

Py:   from module import func
来源：http://bmm.nanxinkj.top

PHP:  require "file.php";  或 use App\Service;
来源：http://zzs.shzxlz.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://lej.ydjk.org.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://zum.yuanzhike.top

Java: import java.util.List;
来源：http://fit.nanxuanxn.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hxe.jqgufenzy.top

Ruby: require "json"; require_relative "./util"
来源：http://lrw.smart0.xyz

C#:   using System.Text;
来源：http://jif.wangdashe.top

[C12] 立即执行函数 IIFE
来源：http://sww.yongpay.top

Py:   (lambda: print("run"))()
来源：http://eva.sysykeji.top

PHP:  (function () { echo "run"; })();
来源：http://eca.gogol.net.cn

JS:   (() => { console.log("run"); })();
来源：http://anj.ehwqpu.com

TS:   (() => { console.log("run"); })();
来源：http://tba.pycfn.com

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://qfu.jiagoushi.top

Go:   func() { fmt.Println("run") }()
来源：http://nko.pengpengdd.cyou

Ruby: -> { puts "run" }.call
来源：http://hso.jqgfzy.top

C#:   // 无 IIFE：用静态构造函数
来源：http://hpu.zhixingplan.top

[C13] 类型声明 / 类型注解
来源：http://ynz.hfpthk.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://vby.bjfxy.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://dfb.fengsongda.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://efy.52xcode.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hbq.hfpthk.cn

Java: int add(int a, int b) { return a + b; }
来源：http://rdo.meibo888.top

Go:   func add(a, b int) int
来源：http://iup.hesvh.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://swg.vqdsnc.cn

C#:   int Add(int a, int b) => a + b;
来源：http://hxc.birdmap.top

[C14] 泛型函数
来源：http://iba.yj202588.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://pqr.svipenyu.cn

PHP:  // 无泛型
来源：http://sxv.yuanzhike.top

JS:   // 无泛型
来源：http://zvb.sysykeji.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hzy.yangfankeji.com

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://ocw.pycfn.com

Go:   func First[T any](items []T) T { return items[0] }
来源：http://cbj.aizwys.cn

Ruby: # 无泛型
来源：http://irb.hesvh.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://fwt.xziqi.cn

[C15] 解构 / 展开参数
来源：http://zgz.yanxiufei.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://ooz.bjfxy.top

PHP:  [$a, $b] = $pair;
来源：http://tdz.yongpay.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://bas.fehbvm.com

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://dzh.ppjwa.cn

Java: // 无解构
来源：http://lql.feifeiyinyue.top

Go:   // 无解构
来源：http://tfs.yonumen.top

Ruby: a, b = pair
来源：http://eee.yangfankeji.com

C#:   var (a, b) = pair;
来源：http://atx.nanxuanxn.top

[C16] 函数 / 方法重载
来源：http://xwb.ydzc1.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://lpj.fanxiaobao.xyz

PHP:  // 无重载
来源：http://jru.sjlbkw.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://lzu.hcnkem.com

TS:   // 用联合类型或重载签名声明
来源：http://wvd.hfpthk.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://oqi.tarul.cn

Go:   // 无重载：用不同函数名
来源：http://ofb.daria6918.cn

Ruby: # 无重载：靠动态参数
来源：http://iia.gaohongyu789.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://hyy.zhoulong.xyz

================================================================================
来源：http://jdn.feifeiyinyue.top

D. 数组 / 列表 / 集合
来源：http://gzr.andypj.xyz

================================================================================
来源：http://qdv.guannengcc.top

[D01] 创建数组 / 列表
来源：http://pmp.shuidangran.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://jlv.fanxiaobao.xyz

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://nyf.yuanzhike.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://cmt.yangfankeji.com

TS:   const arr: number[] = [1, 2, 3];
来源：http://ebn.sxryk.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://qyz.gogol.net.cn

Go:   arr := []int{1, 2, 3}
来源：http://ryg.pycfn.com

Ruby: arr = [1, 2, 3]
来源：http://dpm.xinyue.icu

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://tas.uphjek.com

[D02] 追加元素到末尾
来源：http://hsi.yfazqb.com

Py:   arr.append(4); arr.extend([5, 6])
来源：http://rik.jyoumei.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://ldm.yj202588.top

JS:   arr.push(4);
来源：http://qlj.gogol.net.cn

TS:   arr.push(4);
来源：http://ecs.tian-w.cn

Java: list.add(4);
来源：http://xrj.wangshuangyany.cn

Go:   arr = append(arr, 4)
来源：http://aos.ydzc1.top

Ruby: arr << 4; arr.push(5)
来源：http://vub.zycfv.cn

C#:   list.Add(4);
来源：http://fxo.c1oappe.top

[D03] 在指定位置插入元素
来源：http://lcn.yuxming.cn

Py:   arr.insert(0, 0)
来源：http://ilf.ybcxt.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://isu.zhongyouzk.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://mtk.ppjwa.cn

TS:   arr.splice(0, 0, 0);
来源：http://mgy.wangshuangyany.cn

Java: list.add(0, 0);
来源：http://csp.jqgfzy.top

Go:   arr = append([]int{0}, arr...)
来源：http://iyz.snrcjt.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://wfy.sufxvd.cn

C#:   list.Insert(0, 0);
来源：http://vyn.bbcook.cn

[D04] 删除元素
来源：http://wav.smart0.xyz

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://wbc.nanxinkj.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://ynf.tanke756.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://nxc.shanyushiyangkeji.top

TS:   arr.splice(0, 1);
来源：http://rzs.yongpay.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hsq.sysykeji.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://dap.aibaodan.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://gir.yj20258888.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://bwq.tanke756.top

[D05] 访问与修改元素
来源：http://xcc.yongpay.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://qko.redwolf501.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://wjh.wangshuangyany.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://rpu.guowangkeji.top

TS:   arr[0]; arr.at(-1);
来源：http://omt.fanxiaobao.xyz

Java: list.get(0); list.set(0, 9);
来源：http://gkk.ppjwa.cn

Go:   arr[0]; arr[0] = 9
来源：http://fzr.nanxuanxn.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://crq.shanyushiyangtech.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://yrw.yongpay.top

[D06] 数组长度
来源：http://yyd.yj20258.top

Py:   len(arr)
来源：http://kxf.zhongyouzk.top

PHP:  count($arr);
来源：http://umk.epnwcf.com

JS:   arr.length
来源：http://atp.dianchejie.cn

TS:   arr.length
来源：http://atp.zdqjudy.top

Java: list.size();
来源：http://zvv.ywan-chungtsiang.top

Go:   len(arr)
来源：http://rqq.xylfe.cn

Ruby: arr.length; arr.size
来源：http://bza.fzhhl.top

C#:   list.Count;
来源：http://non.zhongyouzk.top

[D07] 切片 / 取子数组
来源：http://ttc.jqgufenzy.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://zgk.svipenyu.cn

PHP:  array_slice($arr, 1, 3);
来源：http://wop.dianchejie.cn

JS:   arr.slice(1, 4);
来源：http://pju.fehbvm.com

TS:   arr.slice(1, 4);
来源：http://rnb.cucudq.cn

Java: list.subList(1, 4);
来源：http://kxp.c1oappe.top

Go:   arr[1:4]
来源：http://zym.ehwqpu.com

Ruby: arr[1, 3]
来源：http://mtf.aibaodan.cn

C#:   list.GetRange(1, 3);
来源：http://yyz.yuanzhike.top

[D08] 合并两个数组
来源：http://uix.cashguo.top

Py:   a + b;  a.extend(b)
来源：http://zru.cashguo.top

PHP:  array_merge($a, $b);
来源：http://wed.shanyushiyangtech.top

JS:   [...a, ...b];  a.concat(b);
来源：http://gto.sxryk.cn

TS:   [...a, ...b];
来源：http://xff.zdbjq.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://nav.bjfxy.top

Go:   append(a, b...)
来源：http://jov.jyoumei.cn

Ruby: a + b;  a.concat(b)
来源：http://pfp.mhx1999.top

C#:   a.Concat(b).ToList()
来源：http://xif.svipenyu.cn

[D09] 排序（升序）
来源：http://ptx.hammf.cn

Py:   sorted(arr);  arr.sort()
来源：http://ftv.jinqigufen.top

PHP:  sort($arr);
来源：http://tac.daria6918.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://nxu.jinqigfzy.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://nux.jyoumei.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://qpx.gzhubu.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://xll.aizwys.cn

Ruby: arr.sort
来源：http://jxd.yonumen.top

C#:   list.Sort();
来源：http://rzx.yj202588.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://dyz.hysaishi.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://ute.yonumen.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://qfx.hnqzz.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://fys.gaohongyu789.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://nnz.epnwcf.com

Java: list.sort(Comparator.comparing(Person::age));
来源：http://jwt.zhoulong.xyz

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://jlu.ydjk.org.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://mlw.yvedp.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://dnn.ppjwa.cn

[D11] 反转数组
来源：http://hai.hcnkem.com

Py:   arr[::-1];  arr.reverse()
来源：http://rbo.zhongyouzk.top

PHP:  array_reverse($arr);
来源：http://fbf.52xcode.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://pds.zhiwuduotai.top

TS:   [...arr].reverse();
来源：http://zji.wangshuangyany.cn

Java: Collections.reverse(list);
来源：http://zpx.yueranfly.top

Go:   slices.Reverse(arr)
来源：http://yqw.jinqigufen.top

Ruby: arr.reverse
来源：http://gsf.xingfuxueyuan.xyz

C#:   list.Reverse();
来源：http://zis.zdqjudy.top

[D12] 查找元素下标
来源：http://dyi.dashuyun.cn

Py:   arr.index(x);  x in arr
来源：http://ohf.chenjidiqi.icu

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://wlk.cqqwz.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://jyd.ivvv.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hfy.fzhhl.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://bhp.gzhubu.top

Go:   slices.Index(arr, x)
来源：http://tpu.0kj1m.cn

Ruby: arr.index(x)
来源：http://xps.jinghuilouyu.cn

C#:   list.IndexOf(x);
来源：http://gdb.0kj1m.cn

[D13] 过滤（保留满足条件的）
来源：http://lpq.tanke756.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://yqi.quarkkingdee.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://mlw.dianchejie.cn

JS:   arr.filter(x => x > 3)
来源：http://wlc.xuanzx.com

TS:   arr.filter(x => x > 3)
来源：http://qvd.fzhhl.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://lkw.chenlongwang.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://xbf.fktsv.cn

Ruby: arr.select { |x| x > 3 }
来源：http://pza.snrcjt.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://fzq.yuanzhike.top

[D14] 映射转换（每个元素变形）
来源：http://kug.hnqzz.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://yrm.kuanghao11.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://bpo.chenlongwang.top

JS:   arr.map(x => x * 2)
来源：http://kqv.jinyuanbaomall.cn

TS:   arr.map(x => x * 2)
来源：http://npk.bjfxy.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://lmz.ppjwa.cn

Go:   // 手写循环
来源：http://ebz.zdbjq.cn

Ruby: arr.map { |x| x * 2 }
来源：http://hir.yongpay.top

C#:   list.Select(x => x * 2).ToList()
来源：http://hbh.havefunace.top

[D15] 去重
来源：http://lcm.shangyingyoupin.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://vwo.wangshuangyany.cn

PHP:  array_unique($arr);
来源：http://rxb.andypj.xyz

JS:   [...new Set(arr)]
来源：http://cuj.jyoumei.cn

TS:   [...new Set(arr)]
来源：http://wqz.meibo888.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://tmm.9152youxi.cn

Go:   // 用 map[T]struct{} 手写
来源：http://pps.zhoulong.xyz

Ruby: arr.uniq
来源：http://hsu.cqqwz.cn

C#:   list.Distinct().ToList()
来源：http://emf.jinyuanbaomall.cn

[D16] 求和与平均值
来源：http://mtu.zdqjudy.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://ffi.ybcxt.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://gfy.gaohongyu789.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://kkz.hfpthk.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://iyc.hnqzz.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://yjd.vqdsnc.cn

Go:   // 手写循环累加
来源：http://wgu.aizwys.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://iqr.yj202588.top

C#:   list.Sum();  list.Average()
来源：http://lrq.xuetiantiany.cn

[D17] 最大值与最小值
来源：http://std.jqgfzy.top

Py:   max(arr);  min(arr)
来源：http://eob.dianchejie.cn

PHP:  max($arr);  min($arr);
来源：http://atj.jlsjyb.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://kzj.hywenlv.cn

TS:   Math.max(...arr);
来源：http://czj.hcnkem.com

Java: Collections.max(list);  Collections.min(list);
来源：http://jtw.chenjidiqi.icu

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://peu.sweek.top

Ruby: arr.max;  arr.min
来源：http://xzv.0kj1m.cn

C#:   list.Max();  list.Min()
来源：http://uvu.cheryme.top

[D18] 扁平化嵌套数组
来源：http://atr.zhixingplan.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://zxp.chenjidiqi.icu

PHP:  array_merge(...$nested);
来源：http://zwo.bjfxy.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://wud.ctjpmb.com

TS:   nested.flat();
来源：http://cya.shangyingyoupin.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://cmb.chenlongwang.top

Go:   // 手写双层循环
来源：http://dva.guowangkeji.top

Ruby: nested.flatten
来源：http://lwm.bbcook.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://hmn.shanyushiyangtech.top

[D19] 按字段分组
来源：http://zpl.daria6918.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://vjy.aibaodan.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://qan.fktsv.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://rxe.fehbvm.com

TS:   Object.groupBy(arr, x => x.type)
来源：http://jyi.xziqi.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://oro.xinyue.icu

Go:   // 手写 map[string][]T
来源：http://jdv.birdmap.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://maj.xziqi.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://pdi.zhengqikj.top

[D20] 统计每个元素出现次数
来源：http://vzu.zhengqikj.top

Py:   Counter(arr)
来源：http://fxz.zhongyouzk.top

PHP:  array_count_values($arr);
来源：http://mhj.snrcjt.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hoj.snrcjt.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://lrs.fengsongda.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://bzb.gaohongyu789.top

Go:   // 手写 map[T]int
来源：http://crz.epnwcf.com


<!-- 参考信息 -->