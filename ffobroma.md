代发 wailian999

Py:   def add(a, b): return a + b
来源：http://yre.pengpengdd.cyou

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ecp.guowangkeji.top

JS:   function add(a, b) { return a + b; }
来源：http://mre.zycfv.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://soq.hammf.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://wru.nanxuanxn.top

Go:   func add(a, b int) int { return a + b }
来源：http://tej.pengpengdd.cyou

Ruby: def add(a, b); a + b; end
来源：http://phv.zhaomingkeji.xyz

C#:   static int Add(int a, int b) { return a + b; }
来源：http://wrc.jyoumei.cn

[C02] 默认参数
来源：http://mmb.yonumen.top

Py:   def greet(name="World"): return name
来源：http://usp.wangdashe.top

PHP:  function greet($name = "World") { return $name; }
来源：http://bir.yueranfly.top

JS:   function greet(name = "World") { return name; }
来源：http://exh.jinqigfzy.top

TS:   function greet(name: string = "World") { return name; }
来源：http://hrf.ybcxt.top

Java: // 无默认参数：方法重载或 Optional
来源：http://irf.cheryme.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://cwm.dashuyun.cn

Ruby: def greet(name = "World") = name
来源：http://qye.cdnleiting.top

C#:   string Greet(string name = "World") => name;
来源：http://nhg.daria6918.cn

[C03] 可变参数
来源：http://lqj.xziqi.cn

Py:   def total(*args): return sum(args)
来源：http://zhp.hywenlv.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://jmk.daria6918.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://ctp.yueranfly.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://jtn.xziqi.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://yty.zhoulong.xyz

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://zke.feifeiyinyue.top

Ruby: def total(*nums); nums.sum; end
来源：http://mkm.vehdjk.com

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://myf.xinyue.icu

[C04] 命名参数 / 关键字参数
来源：http://rzt.chenzaomai.com

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://ivv.jiagoushi.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://veg.birdmap.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://cio.cqqwz.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hrq.jyoumei.cn

Java: // 无：用 Builder 模式或 record
来源：http://znb.shanyushiyangtech.top

Go:   // 无：用配置结构体参数
来源：http://aoa.daria6918.cn

Ruby: f(a: 1, b: 2)
来源：http://eql.hysaishi.cn

C#:   f(a: 1, b: 2)
来源：http://zhy.jlsjyb.cn

[C05] 返回多个值
来源：http://nsw.52xcode.cn

Py:   return a, b
来源：http://ckb.hnqzz.top

PHP:  return [$a, $b];
来源：http://jks.wangdashe.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://qqb.pycfn.com

TS:   return { a, b };
来源：http://gtc.hcnkem.com

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://tfq.zhiwuduotai.top

Go:   return a, b
来源：http://paf.yvedp.cn

Ruby: return a, b
来源：http://aqu.ppjwa.cn

C#:   return (a, b);              // ValueTuple
来源：http://oge.sjlbkw.cn

[C06] 匿名函数 / lambda
来源：http://hgv.shzxlz.cn

Py:   square = lambda x: x * x
来源：http://nez.zycfv.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://oyr.fehbvm.com

JS:   const square = x => x * x;
来源：http://wgz.epnwcf.com

TS:   const square = (x: number): number => x * x;
来源：http://kgl.andypj.xyz

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://tdh.hnxiangtu.top

Go:   sq := func(x int) int { return x * x }
来源：http://dbn.xuanzx.com

Ruby: square = ->(x) { x * x }
来源：http://vps.xuetiantiany.cn

C#:   Func<int, int> square = x => x * x;
来源：http://lrm.gotoacloud.top

[C07] 把函数作为参数传入
来源：http://usm.hesvh.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://tyr.zhixingplan.top

PHP:  array_map("strtoupper", $arr);
来源：http://ycf.smart0.xyz

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://mvs.svipenyu.cn

TS:   arr.map(String)
来源：http://ppi.xuetiantiany.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://qjm.aibaodan.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://cos.hnqzz.top

Ruby: arr.map(&:upcase)
来源：http://npk.ydjk.org.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://dso.nwbrower.top

[C08] 闭包
来源：http://zul.sweek.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://qyn.ehwqpu.com

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://ipr.dianchejie.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://fpv.jqgufenzy.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://lib.ppjwa.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://gmp.guowangkeji.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://jbh.0kj1m.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://shq.feifeiyinyue.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://jsw.hnqzz.top

[C09] 递归
来源：http://xmv.fzhhl.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://pjd.xuetiantiany.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://imw.sweek.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ijp.shuidangran.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ags.bjfxy.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://rge.jqgufenzy.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hqy.wangshuangyany.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://zfo.snrcjt.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://jqb.yj20258888.top

[C10] 变量作用域
来源：http://xsn.ybcxt.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://nii.yj20258888.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://zvb.chenjidiqi.icu

JS:   let/const 块级作用域，var 函数级作用域
来源：http://rnh.ydzc1.top

TS:   同 JS
来源：http://krt.ybcxt.top

Java: 方法内为块级作用域
来源：http://suq.gaohongyu789.top

Go:   花括号块级作用域
来源：http://jjw.9152youxi.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://nxr.shanyushiyangtech.top

C#:   块级作用域
来源：http://zkw.pycfn.com

[C11] 模块导入与导出
来源：http://oaf.mhx1999.top

Py:   from module import func
来源：http://awh.yonumen.top

PHP:  require "file.php";  或 use App\Service;
来源：http://lpo.zhixingplan.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://riv.zhiwuduotai.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://zbi.gzhubu.top

Java: import java.util.List;
来源：http://kpf.ydzc1.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://mmx.fanxiaobao.xyz

Ruby: require "json"; require_relative "./util"
来源：http://xob.cucudq.cn

C#:   using System.Text;
来源：http://hle.hfpthk.cn

[C12] 立即执行函数 IIFE
来源：http://hbl.smart0.xyz

Py:   (lambda: print("run"))()
来源：http://jug.hfpthk.cn

PHP:  (function () { echo "run"; })();
来源：http://yfz.mhx1999.top

JS:   (() => { console.log("run"); })();
来源：http://zdp.andypj.xyz

TS:   (() => { console.log("run"); })();
来源：http://uvg.jiagoushi.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://nto.shanyushiyangkeji.top

Go:   func() { fmt.Println("run") }()
来源：http://msu.zhoulong.xyz

Ruby: -> { puts "run" }.call
来源：http://zwo.andypj.xyz

C#:   // 无 IIFE：用静态构造函数
来源：http://mgh.hesvh.cn

[C13] 类型声明 / 类型注解
来源：http://gul.meibo888.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://eiu.hesvh.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ovo.chenjidiqi.icu

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hbf.jinqigufen.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://fwx.yueranfly.top

Java: int add(int a, int b) { return a + b; }
来源：http://nll.sufxvd.cn

Go:   func add(a, b int) int
来源：http://sfs.hnxiangtu.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://phr.tanke756.top

C#:   int Add(int a, int b) => a + b;
来源：http://nxu.9152youxi.cn

[C14] 泛型函数
来源：http://ybm.jinyuanbaomall.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://uzt.tian-w.cn

PHP:  // 无泛型
来源：http://jdj.ybcxt.top

JS:   // 无泛型
来源：http://ohk.fanxiaobao.xyz

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://den.uphjek.com

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://kdf.wangshuangyany.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://ils.hnxiangtu.top

Ruby: # 无泛型
来源：http://gbq.fktsv.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://fuz.tian-w.cn

[C15] 解构 / 展开参数
来源：http://yqt.bjfxy.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://ais.jlsjyb.cn

PHP:  [$a, $b] = $pair;
来源：http://sox.zycfv.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://ort.pengpengdd.cyou

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://myy.hfpthk.cn

Java: // 无解构
来源：http://gvk.zhixingplan.top

Go:   // 无解构
来源：http://rwt.kuanghao11.cn

Ruby: a, b = pair
来源：http://muc.hnqzz.top

C#:   var (a, b) = pair;
来源：http://thb.birdmap.top

[C16] 函数 / 方法重载
来源：http://xkt.yj202588.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://pvp.vqdsnc.cn

PHP:  // 无重载
来源：http://ory.xingfuxueyuan.xyz

JS:   // 无重载：靠 arguments.length 分支
来源：http://fep.yj20258.top

TS:   // 用联合类型或重载签名声明
来源：http://dng.chenzaomai.com

Java: void f(int a) {}  void f(String a) {}
来源：http://fnu.shanyushiyangkeji.top

Go:   // 无重载：用不同函数名
来源：http://uep.wangdashe.top

Ruby: # 无重载：靠动态参数
来源：http://kgf.fehbvm.com

C#:   void F(int a) {}  void F(string a) {}
来源：http://vgz.kuanghao11.cn

================================================================================
来源：http://xyy.yvedp.cn

D. 数组 / 列表 / 集合
来源：http://bmx.cheryme.top

================================================================================
来源：http://quv.zycfv.cn

[D01] 创建数组 / 列表
来源：http://eza.jiagoushi.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://yhy.bjfxy.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://cee.wangshuangyany.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://rqp.chenlongwang.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://xkq.birdmap.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://gtr.nanxinkj.top

Go:   arr := []int{1, 2, 3}
来源：http://cou.zdbjq.cn

Ruby: arr = [1, 2, 3]
来源：http://ogn.vehdjk.com

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://bgo.jinyuanbaomall.cn

[D02] 追加元素到末尾
来源：http://uau.wangshuangyany.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://vky.zhijiandao.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://zru.jinqigufen.top

JS:   arr.push(4);
来源：http://cku.yuxming.cn

TS:   arr.push(4);
来源：http://jlg.gogol.net.cn

Java: list.add(4);
来源：http://nuq.zhengqikj.top

Go:   arr = append(arr, 4)
来源：http://kmu.ppjwa.cn

Ruby: arr << 4; arr.push(5)
来源：http://sjz.dianchejie.cn

C#:   list.Add(4);
来源：http://kun.xingfuxueyuan.xyz

[D03] 在指定位置插入元素
来源：http://oje.shangyingyoupin.top

Py:   arr.insert(0, 0)
来源：http://nbc.iojbl.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://fpe.shzxlz.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://yix.nanxinkj.top

TS:   arr.splice(0, 0, 0);
来源：http://pia.mhx1999.top

Java: list.add(0, 0);
来源：http://vrr.gaohongyu789.top

Go:   arr = append([]int{0}, arr...)
来源：http://dfa.yvedp.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://vof.ybcxt.top

C#:   list.Insert(0, 0);
来源：http://oev.tianlin.xyz

[D04] 删除元素
来源：http://iqp.yj20258.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://bku.cucudq.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://qgk.jinghuilouyu.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hek.xuanzx.com

TS:   arr.splice(0, 1);
来源：http://klz.haohaochexian.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://prn.havefunace.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://uwf.zhaomingkeji.xyz

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://cgi.c1oappe.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://dpl.aizwys.cn

[D05] 访问与修改元素
来源：http://mmw.yfazqb.com

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://weu.xuetiantiany.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://ojw.bbcook.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://egq.shangyingyoupin.top

TS:   arr[0]; arr.at(-1);
来源：http://dmo.jqgfzy.top

Java: list.get(0); list.set(0, 9);
来源：http://ilm.sysykeji.top

Go:   arr[0]; arr[0] = 9
来源：http://plr.cashguo.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://rvp.ydzc1.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://dqm.jyoumei.cn

[D06] 数组长度
来源：http://whr.cashguo.top

Py:   len(arr)
来源：http://ggy.0kj1m.cn

PHP:  count($arr);
来源：http://fup.chenjidiqi.icu

JS:   arr.length
来源：http://trz.yj20258888.top

TS:   arr.length
来源：http://gxe.zhoulong.xyz

Java: list.size();
来源：http://pjz.aizwys.cn

Go:   len(arr)
来源：http://xvi.yvedp.cn

Ruby: arr.length; arr.size
来源：http://omp.tanke756.top

C#:   list.Count;
来源：http://pvs.snrcjt.cn

[D07] 切片 / 取子数组
来源：http://dyp.52xcode.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://pgo.mhx1999.top

PHP:  array_slice($arr, 1, 3);
来源：http://dem.zdbjq.cn

JS:   arr.slice(1, 4);
来源：http://ayd.hnqzz.top

TS:   arr.slice(1, 4);
来源：http://qfd.fzhhl.top

Java: list.subList(1, 4);
来源：http://nww.andypj.xyz

Go:   arr[1:4]
来源：http://vxc.jinqigufen.top

Ruby: arr[1, 3]
来源：http://cjc.zhiwuduotai.top

C#:   list.GetRange(1, 3);
来源：http://mtn.chenjidiqi.icu

[D08] 合并两个数组
来源：http://ues.jqgufenzy.top

Py:   a + b;  a.extend(b)
来源：http://crq.hnqzz.top

PHP:  array_merge($a, $b);
来源：http://rvo.shangyingyoupin.top

JS:   [...a, ...b];  a.concat(b);
来源：http://mew.yanxiufei.cn

TS:   [...a, ...b];
来源：http://alq.jinyuanbaomall.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://yfx.shangyingyoupin.top

Go:   append(a, b...)
来源：http://vjn.uphjek.com

Ruby: a + b;  a.concat(b)
来源：http://fty.aizwys.cn

C#:   a.Concat(b).ToList()
来源：http://lzl.shangyingyoupin.top

[D09] 排序（升序）
来源：http://vgq.jinqigfzy.top

Py:   sorted(arr);  arr.sort()
来源：http://eql.yangfankeji.com

PHP:  sort($arr);
来源：http://pga.chenjidiqi.icu

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://vzr.jianghu66.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://vsh.zhijiandao.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://wsg.yonumen.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://kxe.hnxiangtu.top

Ruby: arr.sort
来源：http://sel.yanxiufei.cn

C#:   list.Sort();
来源：http://kjh.snrcjt.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://qix.dianchejie.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://vzh.vehdjk.com

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://imo.ehwqpu.com

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://ymz.jinghuilouyu.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://lll.shanyushiyangkeji.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://fls.redwolf501.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hor.hongshengwenyu.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://kka.dianchejie.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://oac.hfpthk.cn

[D11] 反转数组
来源：http://vmx.zhijiandao.cn

Py:   arr[::-1];  arr.reverse()
来源：http://yqf.jyoumei.cn

PHP:  array_reverse($arr);
来源：http://zgv.hywenlv.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://ojl.iojbl.cn

TS:   [...arr].reverse();
来源：http://ugh.tianlin.xyz

Java: Collections.reverse(list);
来源：http://xuh.yvedp.cn

Go:   slices.Reverse(arr)
来源：http://oxx.daria6918.cn

Ruby: arr.reverse
来源：http://exk.xziqi.cn

C#:   list.Reverse();
来源：http://lwd.guannengcc.top

[D12] 查找元素下标
来源：http://qyw.shanyushiyangtech.top

Py:   arr.index(x);  x in arr
来源：http://fis.shuidangran.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://ytu.jqgfzy.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ipr.zhijiandao.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://opx.fktsv.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://gut.ppjwa.cn

Go:   slices.Index(arr, x)
来源：http://stu.sysykeji.top

Ruby: arr.index(x)
来源：http://ryq.zhongyouzk.top

C#:   list.IndexOf(x);
来源：http://hgt.bjfxy.top

[D13] 过滤（保留满足条件的）
来源：http://crq.wangshuangyany.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://zmb.c1oappe.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://xiz.guowangkeji.top

JS:   arr.filter(x => x > 3)
来源：http://ocy.shuidangran.top

TS:   arr.filter(x => x > 3)
来源：http://hyi.yfazqb.com

Java: list.stream().filter(x -> x > 3).toList()
来源：http://spz.zhijiandao.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://iug.hywenlv.cn

Ruby: arr.select { |x| x > 3 }
来源：http://odq.cdnleiting.top

C#:   list.Where(x => x > 3).ToList()
来源：http://dpo.dianchejie.cn

[D14] 映射转换（每个元素变形）
来源：http://uwd.jianghu66.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://ioa.wangdashe.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://qus.yfazqb.com

JS:   arr.map(x => x * 2)
来源：http://caq.jinyuanbaomall.cn

TS:   arr.map(x => x * 2)
来源：http://sar.jqgufenzy.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://eng.sysykeji.top

Go:   // 手写循环
来源：http://zth.kuanghao11.cn

Ruby: arr.map { |x| x * 2 }
来源：http://dzj.shanyushiyangkeji.top

C#:   list.Select(x => x * 2).ToList()
来源：http://wfg.hnxiangtu.top

[D15] 去重
来源：http://kfm.xuanzx.com

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://yow.hcnkem.com

PHP:  array_unique($arr);
来源：http://kdl.fzhhl.top

JS:   [...new Set(arr)]
来源：http://cvz.ydjk.org.cn

TS:   [...new Set(arr)]
来源：http://wjp.zhiwuduotai.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://sdp.xylfe.cn

Go:   // 用 map[T]struct{} 手写
来源：http://frq.guowangkeji.top

Ruby: arr.uniq
来源：http://uzw.hcnkem.com

C#:   list.Distinct().ToList()
来源：http://mbr.shuidangran.top

[D16] 求和与平均值
来源：http://lqc.svipenyu.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hiu.ivvv.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://qzh.hesvh.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hyz.shzxlz.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://yjg.jinyuanbaomall.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://gor.pycfn.com

Go:   // 手写循环累加
来源：http://qoq.jianghu66.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://ahs.haohaochexian.top

C#:   list.Sum();  list.Average()
来源：http://quf.birdmap.top

[D17] 最大值与最小值
来源：http://ebr.daxiang520.top

Py:   max(arr);  min(arr)
来源：http://gii.cashguo.top

PHP:  max($arr);  min($arr);
来源：http://uhn.jyoumei.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://blx.vqdsnc.cn

TS:   Math.max(...arr);
来源：http://rbe.guowangkeji.top

Java: Collections.max(list);  Collections.min(list);
来源：http://mjo.cqqwz.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://ats.gaohongyu789.top

Ruby: arr.max;  arr.min
来源：http://lpr.zhengqikj.top

C#:   list.Max();  list.Min()
来源：http://eim.fktsv.cn

[D18] 扁平化嵌套数组
来源：http://kcy.nanxinkj.top


<!-- 参考信息 -->