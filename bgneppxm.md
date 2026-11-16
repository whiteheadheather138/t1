代发 wailian999

Ruby: def total(*nums); nums.sum; end
来源：http://xph.daxiang520.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://dbk.gaohongyu789.top

[C04] 命名参数 / 关键字参数
来源：http://pbr.guannengcc.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://nwt.yanxiufei.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://nmg.gzhubu.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://bjv.tianlin.xyz

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://kpq.ywan-chungtsiang.top

Java: // 无：用 Builder 模式或 record
来源：http://ysp.meibo888.top

Go:   // 无：用配置结构体参数
来源：http://crn.wangdashe.top

Ruby: f(a: 1, b: 2)
来源：http://yfc.gotoacloud.top

C#:   f(a: 1, b: 2)
来源：http://qvn.cucudq.cn

[C05] 返回多个值
来源：http://juk.xingfuxueyuan.xyz

Py:   return a, b
来源：http://all.hywenlv.cn

PHP:  return [$a, $b];
来源：http://tbl.zhaomingkeji.xyz

JS:   return [a, b];             // 或 return { a, b };
来源：http://rdp.ybcxt.top

TS:   return { a, b };
来源：http://ptq.hnxiangtu.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://sqs.dashuyun.cn

Go:   return a, b
来源：http://uio.bjfxy.top

Ruby: return a, b
来源：http://ysk.sweek.top

C#:   return (a, b);              // ValueTuple
来源：http://ofz.yuanzhike.top

[C06] 匿名函数 / lambda
来源：http://jcx.xingfuxueyuan.xyz

Py:   square = lambda x: x * x
来源：http://gbd.9152youxi.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://nru.jqgufenzy.top

JS:   const square = x => x * x;
来源：http://jbz.yfazqb.com

TS:   const square = (x: number): number => x * x;
来源：http://wnm.52xcode.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://zxl.hammf.cn

Go:   sq := func(x int) int { return x * x }
来源：http://gvn.sxryk.cn

Ruby: square = ->(x) { x * x }
来源：http://mjb.tianlin.xyz

C#:   Func<int, int> square = x => x * x;
来源：http://hhk.ctjpmb.com

[C07] 把函数作为参数传入
来源：http://zyw.fzhhl.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://vnz.shangyingyoupin.top

PHP:  array_map("strtoupper", $arr);
来源：http://tbl.hnxiangtu.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://dbi.cucudq.cn

TS:   arr.map(String)
来源：http://qwg.gaohongyu789.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://tme.hysaishi.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://mnp.gogol.net.cn

Ruby: arr.map(&:upcase)
来源：http://ssk.mhx1999.top

C#:   arr.Select(s => s.ToUpper())
来源：http://kdi.xylfe.cn

[C08] 闭包
来源：http://qwn.9152youxi.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://vvs.yj20258888.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hvn.sweek.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://wtr.yonumen.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://tww.yj202588.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://muc.gogol.net.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://xts.zhengqikj.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://tre.haohaochexian.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://vum.jinqigfzy.top

[C09] 递归
来源：http://uem.ydjk.org.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://uvi.zdqjudy.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://xok.quarkkingdee.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mpm.meibo888.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hjv.gzhubu.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://msc.zhiwuduotai.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://nsg.hammf.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://kgy.jinyuanbaomall.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://jmd.wangdashe.top

[C10] 变量作用域
来源：http://uhs.tian-w.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://ogv.bbcook.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://plq.uphjek.com

JS:   let/const 块级作用域，var 函数级作用域
来源：http://aff.hcnkem.com

TS:   同 JS
来源：http://uph.jlsjyb.cn

Java: 方法内为块级作用域
来源：http://zms.sjlbkw.cn

Go:   花括号块级作用域
来源：http://tmm.gotoacloud.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://dbl.zycfv.cn

C#:   块级作用域
来源：http://uvj.hammf.cn

[C11] 模块导入与导出
来源：http://lbe.yangfankeji.com

Py:   from module import func
来源：http://vcm.chenlongwang.top

PHP:  require "file.php";  或 use App\Service;
来源：http://vpe.zhixingplan.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://kny.uphjek.com

TS:   export function f(): void {};  import { f } from "./m";
来源：http://sob.aizwys.cn

Java: import java.util.List;
来源：http://ifo.smart0.xyz

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://dpi.guowangkeji.top

Ruby: require "json"; require_relative "./util"
来源：http://ebl.andypj.xyz

C#:   using System.Text;
来源：http://sqk.jlsjyb.cn

[C12] 立即执行函数 IIFE
来源：http://pdj.haohaochexian.top

Py:   (lambda: print("run"))()
来源：http://fwg.cdnleiting.top

PHP:  (function () { echo "run"; })();
来源：http://vbf.haohaochexian.top

JS:   (() => { console.log("run"); })();
来源：http://owt.jiagoushi.top

TS:   (() => { console.log("run"); })();
来源：http://tdf.hnxiangtu.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://scn.jyoumei.cn

Go:   func() { fmt.Println("run") }()
来源：http://vvw.shuidangran.top

Ruby: -> { puts "run" }.call
来源：http://typ.yanxiufei.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://ahh.zhoulong.xyz

[C13] 类型声明 / 类型注解
来源：http://cpt.yuanzhike.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://brj.xziqi.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://stx.hnqzz.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://ntt.vehdjk.com

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://kgx.yuxming.cn

Java: int add(int a, int b) { return a + b; }
来源：http://trx.xinyue.icu

Go:   func add(a, b int) int
来源：http://vrk.xuetiantiany.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://bwe.bbcook.cn

C#:   int Add(int a, int b) => a + b;
来源：http://uhf.tarul.cn

[C14] 泛型函数
来源：http://rsz.ybcxt.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://jaj.zhongyouzk.top

PHP:  // 无泛型
来源：http://vkq.316326.xyz

JS:   // 无泛型
来源：http://ydo.tarul.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://xmc.fehbvm.com

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://nvu.chenlongwang.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://ofl.vehdjk.com

Ruby: # 无泛型
来源：http://rfq.pengpengdd.cyou

C#:   static T First<T>(List<T> items) => items[0];
来源：http://qms.wangshuangyany.cn

[C15] 解构 / 展开参数
来源：http://ubm.hnxiangtu.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://bth.yanxiufei.cn

PHP:  [$a, $b] = $pair;
来源：http://ttq.gaohongyu789.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://cho.zhoulong.xyz

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://ijc.hysaishi.cn

Java: // 无解构
来源：http://ajs.hfpthk.cn

Go:   // 无解构
来源：http://mws.iojbl.cn

Ruby: a, b = pair
来源：http://rut.tian-w.cn

C#:   var (a, b) = pair;
来源：http://dui.snrcjt.cn

[C16] 函数 / 方法重载
来源：http://qas.chenjidiqi.icu

Py:   # 无重载：用默认参数或 *args 变通
来源：http://gan.tianlin.xyz

PHP:  // 无重载
来源：http://rmw.gogol.net.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://atr.ywan-chungtsiang.top

TS:   // 用联合类型或重载签名声明
来源：http://fad.jinqigfzy.top

Java: void f(int a) {}  void f(String a) {}
来源：http://agr.sysykeji.top

Go:   // 无重载：用不同函数名
来源：http://otz.sweek.top

Ruby: # 无重载：靠动态参数
来源：http://jtw.fktsv.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://uqc.ivvv.top

================================================================================
来源：http://zhx.ywan-chungtsiang.top

D. 数组 / 列表 / 集合
来源：http://wdj.haohaochexian.top

================================================================================
来源：http://xzn.wangshuangyany.cn

[D01] 创建数组 / 列表
来源：http://fwv.tianlin.xyz

Py:   arr = [1, 2, 3];  empty = []
来源：http://kjj.hongshengwenyu.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://tdi.xziqi.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://riq.kuanghao11.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://fun.vehdjk.com

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://esl.zhiwuduotai.top

Go:   arr := []int{1, 2, 3}
来源：http://fwr.jiagoushi.top

Ruby: arr = [1, 2, 3]
来源：http://apa.bbcook.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://fwl.hysaishi.cn

[D02] 追加元素到末尾
来源：http://ycm.ydjk.org.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://vdn.ivvv.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://ois.nanxinkj.top

JS:   arr.push(4);
来源：http://oth.zhoulong.xyz

TS:   arr.push(4);
来源：http://zab.guannengcc.top

Java: list.add(4);
来源：http://kuw.yangfankeji.com

Go:   arr = append(arr, 4)
来源：http://ntm.kuanghao11.cn

Ruby: arr << 4; arr.push(5)
来源：http://fqx.xylfe.cn

C#:   list.Add(4);
来源：http://avs.fengsongda.top

[D03] 在指定位置插入元素
来源：http://sse.hfpthk.cn

Py:   arr.insert(0, 0)
来源：http://qxf.zhengqikj.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://lms.yuxming.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://rrx.fehbvm.com

TS:   arr.splice(0, 0, 0);
来源：http://qlj.cashguo.top

Java: list.add(0, 0);
来源：http://zdu.nwbrower.top

Go:   arr = append([]int{0}, arr...)
来源：http://zps.hammf.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://rqz.tian-w.cn

C#:   list.Insert(0, 0);
来源：http://xbs.52xcode.cn

[D04] 删除元素
来源：http://ady.hnxiangtu.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://czr.xingfuxueyuan.xyz

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://rut.yueranfly.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://zcx.xziqi.cn

TS:   arr.splice(0, 1);
来源：http://zdx.sysykeji.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://tie.sufxvd.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://zqb.jlsjyb.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://jtl.xuetiantiany.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://tff.ivvv.top

[D05] 访问与修改元素
来源：http://lqo.hywenlv.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://iql.kuanghao11.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://trw.jinyuanbaomall.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://qus.sufxvd.cn

TS:   arr[0]; arr.at(-1);
来源：http://lzg.mhx1999.top

Java: list.get(0); list.set(0, 9);
来源：http://qwr.jianghu66.top

Go:   arr[0]; arr[0] = 9
来源：http://hpx.feifeiyinyue.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://rzv.hywenlv.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://meg.dashuyun.cn

[D06] 数组长度
来源：http://ows.fanxiaobao.xyz

Py:   len(arr)
来源：http://kfd.ydzc1.top

PHP:  count($arr);
来源：http://ymq.aizwys.cn

JS:   arr.length
来源：http://nbn.zdbjq.cn

TS:   arr.length
来源：http://qax.wangshuangyany.cn

Java: list.size();
来源：http://gmt.zdbjq.cn

Go:   len(arr)
来源：http://zns.shuidangran.top

Ruby: arr.length; arr.size
来源：http://rxu.zdqjudy.top

C#:   list.Count;
来源：http://tnv.fktsv.cn

[D07] 切片 / 取子数组
来源：http://pmr.birdmap.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://een.sjlbkw.cn

PHP:  array_slice($arr, 1, 3);
来源：http://qgb.andypj.xyz

JS:   arr.slice(1, 4);
来源：http://ckf.xuetiantiany.cn

TS:   arr.slice(1, 4);
来源：http://vfs.xziqi.cn

Java: list.subList(1, 4);
来源：http://pim.nanxuanxn.top

Go:   arr[1:4]
来源：http://plz.yangfankeji.com

Ruby: arr[1, 3]
来源：http://ilh.0kj1m.cn

C#:   list.GetRange(1, 3);
来源：http://qrs.yangfankeji.com

[D08] 合并两个数组
来源：http://epy.ywan-chungtsiang.top

Py:   a + b;  a.extend(b)
来源：http://muv.zhengqikj.top

PHP:  array_merge($a, $b);
来源：http://tdm.chenlongwang.top

JS:   [...a, ...b];  a.concat(b);
来源：http://stv.mhx1999.top

TS:   [...a, ...b];
来源：http://zqz.zycfv.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://tby.dashuyun.cn

Go:   append(a, b...)
来源：http://apf.nwbrower.top

Ruby: a + b;  a.concat(b)
来源：http://ech.zhiwuduotai.top

C#:   a.Concat(b).ToList()
来源：http://fla.ybcxt.top

[D09] 排序（升序）
来源：http://yuf.chenjidiqi.icu

Py:   sorted(arr);  arr.sort()
来源：http://vto.dianchejie.cn

PHP:  sort($arr);
来源：http://zhw.tanke756.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://wym.andypj.xyz

TS:   [...arr].sort((x, y) => x - y);
来源：http://hci.chenlongwang.top

Java: Collections.sort(list);  list.sort(null);
来源：http://zsu.nanxinkj.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://ojv.havefunace.top

Ruby: arr.sort
来源：http://tgq.nwbrower.top

C#:   list.Sort();
来源：http://oby.dashuyun.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://ivj.yfazqb.com

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://maf.birdmap.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://bez.daxiang520.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://urf.andypj.xyz

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hgg.sjlbkw.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://mfp.52xcode.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://frs.daxiang520.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://txx.haohaochexian.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://tim.zdbjq.cn

[D11] 反转数组
来源：http://pxr.yongpay.top

Py:   arr[::-1];  arr.reverse()
来源：http://nwy.shanyushiyangtech.top

PHP:  array_reverse($arr);
来源：http://xgv.zhengqikj.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://dwb.zhaomingkeji.xyz

TS:   [...arr].reverse();
来源：http://jrc.nanxuanxn.top

Java: Collections.reverse(list);
来源：http://dld.yonumen.top

Go:   slices.Reverse(arr)
来源：http://zhf.nanxuanxn.top

Ruby: arr.reverse
来源：http://bhw.fanxiaobao.xyz

C#:   list.Reverse();
来源：http://cjv.hnxiangtu.top

[D12] 查找元素下标
来源：http://knb.ydjk.org.cn

Py:   arr.index(x);  x in arr
来源：http://tah.hesvh.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://tth.nwbrower.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mlr.cashguo.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ssh.ppjwa.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://iiu.316326.xyz

Go:   slices.Index(arr, x)
来源：http://gnl.zdqjudy.top

Ruby: arr.index(x)
来源：http://nzn.zdqjudy.top

C#:   list.IndexOf(x);
来源：http://qyn.hongshengwenyu.top

[D13] 过滤（保留满足条件的）
来源：http://qxf.hywenlv.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://bbn.jyoumei.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://xzt.guowangkeji.top

JS:   arr.filter(x => x > 3)
来源：http://ikl.jinghuilouyu.cn

TS:   arr.filter(x => x > 3)
来源：http://zbm.xylfe.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://zfo.zhixingplan.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://nde.yuanzhike.top

Ruby: arr.select { |x| x > 3 }
来源：http://mcn.xuetiantiany.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://bux.ehwqpu.com

[D14] 映射转换（每个元素变形）
来源：http://ikt.cheryme.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://xij.pycfn.com

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://tdp.andypj.xyz

JS:   arr.map(x => x * 2)
来源：http://cjd.hnxiangtu.top

TS:   arr.map(x => x * 2)
来源：http://mqp.epnwcf.com

Java: list.stream().map(x -> x * 2).toList()
来源：http://pqp.shuidangran.top

Go:   // 手写循环
来源：http://ndu.sysykeji.top

Ruby: arr.map { |x| x * 2 }
来源：http://pas.daria6918.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://mjq.ydjk.org.cn

[D15] 去重
来源：http://dfz.shzxlz.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://mvl.aizwys.cn

PHP:  array_unique($arr);
来源：http://iep.shanyushiyangtech.top

JS:   [...new Set(arr)]
来源：http://lpu.zhoulong.xyz

TS:   [...new Set(arr)]
来源：http://kku.jinghuilouyu.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://qsh.zhoulong.xyz

Go:   // 用 map[T]struct{} 手写
来源：http://wyu.hywenlv.cn

Ruby: arr.uniq
来源：http://yhm.yuanzhike.top

C#:   list.Distinct().ToList()
来源：http://kre.daria6918.cn

[D16] 求和与平均值
来源：http://eil.yongpay.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://mac.jinqigfzy.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://unb.yueranfly.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://gid.yangfankeji.com

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://tht.hnqzz.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://vyo.xylfe.cn

Go:   // 手写循环累加
来源：http://vkc.shanyushiyangtech.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://gew.cheryme.top

C#:   list.Sum();  list.Average()
来源：http://ssq.yanxiufei.cn

[D17] 最大值与最小值
来源：http://zfh.bjfxy.top

Py:   max(arr);  min(arr)
来源：http://eod.nanxuanxn.top

PHP:  max($arr);  min($arr);
来源：http://pea.snrcjt.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://zzl.gaohongyu789.top

TS:   Math.max(...arr);
来源：http://yiy.0kj1m.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://wcb.xylfe.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://zsp.shzxlz.cn

Ruby: arr.max;  arr.min
来源：http://rux.smart0.xyz

C#:   list.Max();  list.Min()
来源：http://azx.snrcjt.cn

[D18] 扁平化嵌套数组
来源：http://yvw.c1oappe.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://jqx.svipenyu.cn

PHP:  array_merge(...$nested);
来源：http://nio.hesvh.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://alg.zdqjudy.top

TS:   nested.flat();
来源：http://plg.vqdsnc.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://ksb.xziqi.cn

Go:   // 手写双层循环
来源：http://wug.tian-w.cn

Ruby: nested.flatten
来源：http://faz.316326.xyz

C#:   nested.SelectMany(x => x).ToList()
来源：http://bug.jinqigufen.top

[D19] 按字段分组
来源：http://zas.nanxinkj.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://aec.yfazqb.com

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://qtk.smart0.xyz

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://udv.zdbjq.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://hxp.zhixingplan.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://sau.vqdsnc.cn

Go:   // 手写 map[string][]T
来源：http://doe.pengpengdd.cyou

Ruby: arr.group_by { |x| x[:type] }
来源：http://oig.ydzc1.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://xvs.hcnkem.com

[D20] 统计每个元素出现次数
来源：http://jfj.xinyue.icu

Py:   Counter(arr)
来源：http://fkp.ydjk.org.cn

PHP:  array_count_values($arr);
来源：http://cwd.nanxinkj.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hpj.dashuyun.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://aym.birdmap.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://dnc.ivvv.top

Go:   // 手写 map[T]int
来源：http://cdc.hnqzz.top


<!-- 参考信息 -->