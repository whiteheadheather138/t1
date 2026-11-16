代发 wailian999

Ruby: def total(*nums); nums.sum; end
来源：http://xtd.yj20258.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://eex.gogol.net.cn

[C04] 命名参数 / 关键字参数
来源：http://rvi.ywan-chungtsiang.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://mrq.pengpengdd.cyou

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://uek.316326.xyz

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://fgq.fktsv.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://cvu.cashguo.top

Java: // 无：用 Builder 模式或 record
来源：http://ulm.xingfuxueyuan.xyz

Go:   // 无：用配置结构体参数
来源：http://tlo.bbcook.cn

Ruby: f(a: 1, b: 2)
来源：http://ogw.bbcook.cn

C#:   f(a: 1, b: 2)
来源：http://rll.shangyingyoupin.top

[C05] 返回多个值
来源：http://dzp.yj202588.top

Py:   return a, b
来源：http://emx.hammf.cn

PHP:  return [$a, $b];
来源：http://xfe.chenlongwang.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://gqz.jianghu66.top

TS:   return { a, b };
来源：http://uuo.yueranfly.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://niv.xziqi.cn

Go:   return a, b
来源：http://sgj.gogol.net.cn

Ruby: return a, b
来源：http://pbz.andypj.xyz

C#:   return (a, b);              // ValueTuple
来源：http://sxg.hammf.cn

[C06] 匿名函数 / lambda
来源：http://vsg.yuxming.cn

Py:   square = lambda x: x * x
来源：http://vby.zdqjudy.top

PHP:  $square = fn($x) => $x * $x;
来源：http://mfz.snrcjt.cn

JS:   const square = x => x * x;
来源：http://ymf.smart0.xyz

TS:   const square = (x: number): number => x * x;
来源：http://fpw.fehbvm.com

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://qyt.zdqjudy.top

Go:   sq := func(x int) int { return x * x }
来源：http://ddr.tanke756.top

Ruby: square = ->(x) { x * x }
来源：http://hwb.hysaishi.cn

C#:   Func<int, int> square = x => x * x;
来源：http://zra.tian-w.cn

[C07] 把函数作为参数传入
来源：http://nyx.bbcook.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://wjo.fehbvm.com

PHP:  array_map("strtoupper", $arr);
来源：http://wva.quarkkingdee.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://gbm.yueranfly.top

TS:   arr.map(String)
来源：http://thy.ehwqpu.com

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://prx.fengsongda.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://kkm.gogol.net.cn

Ruby: arr.map(&:upcase)
来源：http://ugw.c1oappe.top

C#:   arr.Select(s => s.ToUpper())
来源：http://bcs.havefunace.top

[C08] 闭包
来源：http://omt.yj20258.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://cqv.9152youxi.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://qti.gaohongyu789.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://bgl.wangdashe.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://pbr.iojbl.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://gjx.zhiwuduotai.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://fqk.guowangkeji.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://pnk.ybcxt.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://jhw.52xcode.cn

[C09] 递归
来源：http://oiu.jianghu66.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://mtn.zdqjudy.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://dka.yvedp.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://cyr.jyoumei.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ucw.tanke756.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://cwz.shuidangran.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://pum.cucudq.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://chu.ivvv.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://snj.zhaomingkeji.xyz

[C10] 变量作用域
来源：http://cgu.fzhhl.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://rgr.zhoulong.xyz

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hmc.fanxiaobao.xyz

JS:   let/const 块级作用域，var 函数级作用域
来源：http://bfs.fktsv.cn

TS:   同 JS
来源：http://dcm.zhijiandao.cn

Java: 方法内为块级作用域
来源：http://chc.jiagoushi.top

Go:   花括号块级作用域
来源：http://jin.hysaishi.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://mvu.hywenlv.cn

C#:   块级作用域
来源：http://dil.yj202588.top

[C11] 模块导入与导出
来源：http://hcx.guowangkeji.top

Py:   from module import func
来源：http://lkm.cheryme.top

PHP:  require "file.php";  或 use App\Service;
来源：http://naq.redwolf501.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://dbm.shuidangran.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://ywf.fktsv.cn

Java: import java.util.List;
来源：http://kqh.jianghu66.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://lmz.yfazqb.com

Ruby: require "json"; require_relative "./util"
来源：http://qyc.ppjwa.cn

C#:   using System.Text;
来源：http://cqo.sufxvd.cn

[C12] 立即执行函数 IIFE
来源：http://zli.andypj.xyz

Py:   (lambda: print("run"))()
来源：http://ljn.havefunace.top

PHP:  (function () { echo "run"; })();
来源：http://joa.mhx1999.top

JS:   (() => { console.log("run"); })();
来源：http://yfs.uphjek.com

TS:   (() => { console.log("run"); })();
来源：http://yjt.ehwqpu.com

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://wfy.nwbrower.top

Go:   func() { fmt.Println("run") }()
来源：http://teq.xylfe.cn

Ruby: -> { puts "run" }.call
来源：http://aav.vehdjk.com

C#:   // 无 IIFE：用静态构造函数
来源：http://gll.wangdashe.top

[C13] 类型声明 / 类型注解
来源：http://feb.bjfxy.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://fid.shangyingyoupin.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://cel.yj20258888.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://slu.zycfv.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://bwd.chenzaomai.com

Java: int add(int a, int b) { return a + b; }
来源：http://gef.haohaochexian.top

Go:   func add(a, b int) int
来源：http://ree.fehbvm.com

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://pov.cqqwz.cn

C#:   int Add(int a, int b) => a + b;
来源：http://tlx.tarul.cn

[C14] 泛型函数
来源：http://ras.ppjwa.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://sna.yuxming.cn

PHP:  // 无泛型
来源：http://jhi.quarkkingdee.top

JS:   // 无泛型
来源：http://lnh.c1oappe.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://pws.yonumen.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://xje.gzhubu.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://pxs.52xcode.cn

Ruby: # 无泛型
来源：http://ptc.yangfankeji.com

C#:   static T First<T>(List<T> items) => items[0];
来源：http://mrq.jinghuilouyu.cn

[C15] 解构 / 展开参数
来源：http://elr.yfazqb.com

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://xlw.meibo888.top

PHP:  [$a, $b] = $pair;
来源：http://ydk.kuanghao11.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://qdv.xuanzx.com

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://jgx.gzhubu.top

Java: // 无解构
来源：http://zlx.smart0.xyz

Go:   // 无解构
来源：http://xas.ehwqpu.com

Ruby: a, b = pair
来源：http://hje.jiagoushi.top

C#:   var (a, b) = pair;
来源：http://ulp.feifeiyinyue.top

[C16] 函数 / 方法重载
来源：http://mce.cashguo.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://mua.svipenyu.cn

PHP:  // 无重载
来源：http://cro.zhiwuduotai.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://wxk.cqqwz.cn

TS:   // 用联合类型或重载签名声明
来源：http://kqw.zhixingplan.top

Java: void f(int a) {}  void f(String a) {}
来源：http://syl.yuxming.cn

Go:   // 无重载：用不同函数名
来源：http://zkj.jinqigfzy.top

Ruby: # 无重载：靠动态参数
来源：http://huu.ywan-chungtsiang.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://jqq.jinghuilouyu.cn

================================================================================
来源：http://zat.yuanzhike.top

D. 数组 / 列表 / 集合
来源：http://gpz.quarkkingdee.top

================================================================================
来源：http://vwk.gzhubu.top

[D01] 创建数组 / 列表
来源：http://ryp.hnxiangtu.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://xff.fehbvm.com

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://owp.yj202588.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://shd.dashuyun.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://mfs.cucudq.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://qei.yj20258.top

Go:   arr := []int{1, 2, 3}
来源：http://kug.dashuyun.cn

Ruby: arr = [1, 2, 3]
来源：http://tys.zhaomingkeji.xyz

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://xxh.redwolf501.top

[D02] 追加元素到末尾
来源：http://wky.sysykeji.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hqo.cashguo.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://qkt.yj20258888.top

JS:   arr.push(4);
来源：http://aak.jqgfzy.top

TS:   arr.push(4);
来源：http://cil.ppjwa.cn

Java: list.add(4);
来源：http://bbm.zycfv.cn

Go:   arr = append(arr, 4)
来源：http://mwm.yonumen.top

Ruby: arr << 4; arr.push(5)
来源：http://bew.redwolf501.top

C#:   list.Add(4);
来源：http://hhz.gaohongyu789.top

[D03] 在指定位置插入元素
来源：http://dgh.jinqigufen.top

Py:   arr.insert(0, 0)
来源：http://dqc.jlsjyb.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://ees.chenjidiqi.icu

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://zku.dashuyun.cn

TS:   arr.splice(0, 0, 0);
来源：http://bqh.xingfuxueyuan.xyz

Java: list.add(0, 0);
来源：http://vqe.ydzc1.top

Go:   arr = append([]int{0}, arr...)
来源：http://hlx.yj202588.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://adc.wangshuangyany.cn

C#:   list.Insert(0, 0);
来源：http://zcq.sjlbkw.cn

[D04] 删除元素
来源：http://vak.9152youxi.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://szs.aibaodan.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://qtv.nanxuanxn.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://tpi.mhx1999.top

TS:   arr.splice(0, 1);
来源：http://krv.vqdsnc.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hts.iojbl.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://rtp.redwolf501.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://qzp.0kj1m.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://jvx.yanxiufei.cn

[D05] 访问与修改元素
来源：http://fwt.chenzaomai.com

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://uji.cucudq.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hle.cqqwz.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://ilz.hammf.cn

TS:   arr[0]; arr.at(-1);
来源：http://kpn.vqdsnc.cn

Java: list.get(0); list.set(0, 9);
来源：http://bba.havefunace.top

Go:   arr[0]; arr[0] = 9
来源：http://cqo.gogol.net.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://uhz.quarkkingdee.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://khy.gotoacloud.top

[D06] 数组长度
来源：http://oym.yvedp.cn

Py:   len(arr)
来源：http://nrz.gzhubu.top

PHP:  count($arr);
来源：http://wim.zhiwuduotai.top

JS:   arr.length
来源：http://quw.hnxiangtu.top

TS:   arr.length
来源：http://zoc.jianghu66.top

Java: list.size();
来源：http://odh.uphjek.com

Go:   len(arr)
来源：http://uru.hesvh.cn

Ruby: arr.length; arr.size
来源：http://hdm.jinqigufen.top

C#:   list.Count;
来源：http://jzd.nwbrower.top

[D07] 切片 / 取子数组
来源：http://gvh.havefunace.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://jdr.jlsjyb.cn

PHP:  array_slice($arr, 1, 3);
来源：http://oik.ybcxt.top

JS:   arr.slice(1, 4);
来源：http://aut.haohaochexian.top

TS:   arr.slice(1, 4);
来源：http://mrp.meibo888.top

Java: list.subList(1, 4);
来源：http://kxe.pycfn.com

Go:   arr[1:4]
来源：http://nzt.ywan-chungtsiang.top

Ruby: arr[1, 3]
来源：http://plz.cqqwz.cn

C#:   list.GetRange(1, 3);
来源：http://xxa.c1oappe.top

[D08] 合并两个数组
来源：http://bfv.xziqi.cn

Py:   a + b;  a.extend(b)
来源：http://clw.hongshengwenyu.top

PHP:  array_merge($a, $b);
来源：http://uid.ydzc1.top

JS:   [...a, ...b];  a.concat(b);
来源：http://nmj.yangfankeji.com

TS:   [...a, ...b];
来源：http://nin.chenjidiqi.icu

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://pbz.hfpthk.cn

Go:   append(a, b...)
来源：http://ytj.jinqigfzy.top

Ruby: a + b;  a.concat(b)
来源：http://mxz.dianchejie.cn

C#:   a.Concat(b).ToList()
来源：http://gth.hnqzz.top

[D09] 排序（升序）
来源：http://ozn.meibo888.top

Py:   sorted(arr);  arr.sort()
来源：http://lza.bjfxy.top

PHP:  sort($arr);
来源：http://eat.ppjwa.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://mvw.havefunace.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://glt.jiagoushi.top

Java: Collections.sort(list);  list.sort(null);
来源：http://ims.jyoumei.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://ibg.jlsjyb.cn

Ruby: arr.sort
来源：http://rqh.hnxiangtu.top

C#:   list.Sort();
来源：http://pjp.xziqi.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://gjh.sysykeji.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://cqf.gaohongyu789.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://guo.bjfxy.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://tio.hnxiangtu.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://vsa.hnxiangtu.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://ewr.yj202588.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://mqc.birdmap.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://cdo.tianlin.xyz

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://jrq.fanxiaobao.xyz

[D11] 反转数组
来源：http://veo.nanxuanxn.top

Py:   arr[::-1];  arr.reverse()
来源：http://mih.havefunace.top

PHP:  array_reverse($arr);
来源：http://cvt.sufxvd.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://dtn.quarkkingdee.top

TS:   [...arr].reverse();
来源：http://jil.cheryme.top

Java: Collections.reverse(list);
来源：http://nib.zhixingplan.top

Go:   slices.Reverse(arr)
来源：http://deg.zhijiandao.cn

Ruby: arr.reverse
来源：http://rkz.hammf.cn

C#:   list.Reverse();
来源：http://sgw.jqgufenzy.top

[D12] 查找元素下标
来源：http://smt.fktsv.cn

Py:   arr.index(x);  x in arr
来源：http://mfd.wangdashe.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hjy.smart0.xyz

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://pkw.uphjek.com

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://nfm.vehdjk.com

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://xjd.pengpengdd.cyou

Go:   slices.Index(arr, x)
来源：http://rtm.chenlongwang.top

Ruby: arr.index(x)
来源：http://fnm.52xcode.cn

C#:   list.IndexOf(x);
来源：http://oll.yuxming.cn

[D13] 过滤（保留满足条件的）
来源：http://hfi.shzxlz.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://tjv.redwolf501.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://euf.pycfn.com

JS:   arr.filter(x => x > 3)
来源：http://orf.ehwqpu.com

TS:   arr.filter(x => x > 3)
来源：http://uip.tarul.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://ear.yangfankeji.com

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://cbf.nwbrower.top

Ruby: arr.select { |x| x > 3 }
来源：http://nfy.xuetiantiany.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://uis.hcnkem.com

[D14] 映射转换（每个元素变形）
来源：http://qtc.cqqwz.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://vqw.yj20258888.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://zrc.pycfn.com

JS:   arr.map(x => x * 2)
来源：http://opw.nanxinkj.top

TS:   arr.map(x => x * 2)
来源：http://afw.wangshuangyany.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://xbk.yj20258888.top

Go:   // 手写循环
来源：http://iga.kuanghao11.cn

Ruby: arr.map { |x| x * 2 }
来源：http://jfq.chenlongwang.top

C#:   list.Select(x => x * 2).ToList()
来源：http://uez.sufxvd.cn

[D15] 去重
来源：http://kgk.nanxinkj.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://kmh.316326.xyz

PHP:  array_unique($arr);
来源：http://bwk.yuanzhike.top

JS:   [...new Set(arr)]
来源：http://jbd.zhengqikj.top

TS:   [...new Set(arr)]
来源：http://tqa.iojbl.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://ter.sjlbkw.cn

Go:   // 用 map[T]struct{} 手写
来源：http://apw.daxiang520.top

Ruby: arr.uniq
来源：http://xth.redwolf501.top

C#:   list.Distinct().ToList()
来源：http://ixl.ywan-chungtsiang.top

[D16] 求和与平均值
来源：http://bvz.wangshuangyany.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://zyl.yuanzhike.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://vnm.xziqi.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://win.nanxinkj.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://emx.c1oappe.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://ygi.chenjidiqi.icu

Go:   // 手写循环累加
来源：http://wju.shangyingyoupin.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://lrj.yj202588.top

C#:   list.Sum();  list.Average()
来源：http://zyt.ydjk.org.cn

[D17] 最大值与最小值
来源：http://kus.pycfn.com

Py:   max(arr);  min(arr)
来源：http://bmo.jlsjyb.cn

PHP:  max($arr);  min($arr);
来源：http://ljt.wangdashe.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://nqw.shzxlz.cn

TS:   Math.max(...arr);
来源：http://phg.fengsongda.top

Java: Collections.max(list);  Collections.min(list);
来源：http://fgr.guannengcc.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://xks.wangshuangyany.cn

Ruby: arr.max;  arr.min
来源：http://qtk.sxryk.cn

C#:   list.Max();  list.Min()
来源：http://yus.9152youxi.cn

[D18] 扁平化嵌套数组
来源：http://aja.daria6918.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://ndv.xingfuxueyuan.xyz

PHP:  array_merge(...$nested);
来源：http://xbv.chenjidiqi.icu

JS:   nested.flat();  nested.flat(Infinity)
来源：http://kau.xziqi.cn

TS:   nested.flat();
来源：http://auq.jiagoushi.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://kpv.jyoumei.cn

Go:   // 手写双层循环
来源：http://ogz.xuanzx.com

Ruby: nested.flatten
来源：http://eiw.bjfxy.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://uwb.yj20258888.top

[D19] 按字段分组
来源：http://bde.hongshengwenyu.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://ewc.pengpengdd.cyou

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://qba.yangfankeji.com

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://mpw.zhongyouzk.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://ygj.hongshengwenyu.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://toy.hongshengwenyu.top

Go:   // 手写 map[string][]T
来源：http://qbw.andypj.xyz

Ruby: arr.group_by { |x| x[:type] }
来源：http://ixu.fanxiaobao.xyz

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://xxc.yongpay.top

[D20] 统计每个元素出现次数
来源：http://eui.nwbrower.top

Py:   Counter(arr)
来源：http://paw.jianghu66.top

PHP:  array_count_values($arr);
来源：http://tne.iojbl.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://nkg.zhaomingkeji.xyz

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://lmy.yuxming.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://exw.xingfuxueyuan.xyz

Go:   // 手写 map[T]int
来源：http://bik.yuanzhike.top


<!-- 参考信息 -->