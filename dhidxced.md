代发 wailian999

Py:   if not data: return
来源：http://oft.quarkkingdee.top

PHP:  if (!$data) { return; }
来源：http://wjo.yvedp.cn

JS:   if (!data) return;
来源：http://ddn.chenzaomai.com

TS:   if (!data) return;
来源：http://ice.vehdjk.com

Java: if (data == null) return;
来源：http://frn.yj20258.top

Go:   if data == nil { return }
来源：http://hfz.c1oappe.top

Ruby: return if data.nil?
来源：http://phi.chenlongwang.top

C#:   if (data == null) return;
来源：http://qht.haohaochexian.top

================================================================================
来源：http://dls.nanxuanxn.top

C. 函数与作用域
来源：http://wqa.aibaodan.cn

================================================================================
来源：http://jno.sxryk.cn

[C01] 定义函数
来源：http://zsd.yuanzhike.top

Py:   def add(a, b): return a + b
来源：http://pgj.smart0.xyz

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://iru.xylfe.cn

JS:   function add(a, b) { return a + b; }
来源：http://avw.vehdjk.com

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://por.pengpengdd.cyou

Java: static int add(int a, int b) { return a + b; }
来源：http://yef.jyoumei.cn

Go:   func add(a, b int) int { return a + b }
来源：http://jxd.tanke756.top

Ruby: def add(a, b); a + b; end
来源：http://vlq.sweek.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://ouo.chenjidiqi.icu

[C02] 默认参数
来源：http://jkq.sufxvd.cn

Py:   def greet(name="World"): return name
来源：http://xlv.hysaishi.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://iut.zdbjq.cn

JS:   function greet(name = "World") { return name; }
来源：http://trl.epnwcf.com

TS:   function greet(name: string = "World") { return name; }
来源：http://ghp.yj202588.top

Java: // 无默认参数：方法重载或 Optional
来源：http://bfi.tarul.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://ssx.shanyushiyangtech.top

Ruby: def greet(name = "World") = name
来源：http://bhx.dianchejie.cn

C#:   string Greet(string name = "World") => name;
来源：http://fyg.shzxlz.cn

[C03] 可变参数
来源：http://zrs.zhixingplan.top

Py:   def total(*args): return sum(args)
来源：http://uzm.yj20258888.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://pgl.svipenyu.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://txv.mhx1999.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://vmg.316326.xyz

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://bci.316326.xyz

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://msm.gogol.net.cn

Ruby: def total(*nums); nums.sum; end
来源：http://ebi.fktsv.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://lcg.svipenyu.cn

[C04] 命名参数 / 关键字参数
来源：http://kha.kuanghao11.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://fwe.sufxvd.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hzg.xylfe.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://qyi.dianchejie.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://bij.sxryk.cn

Java: // 无：用 Builder 模式或 record
来源：http://kdk.pengpengdd.cyou

Go:   // 无：用配置结构体参数
来源：http://rga.tarul.cn

Ruby: f(a: 1, b: 2)
来源：http://tsn.fzhhl.top

C#:   f(a: 1, b: 2)
来源：http://uzl.jqgfzy.top

[C05] 返回多个值
来源：http://inm.hongshengwenyu.top

Py:   return a, b
来源：http://yze.ybcxt.top

PHP:  return [$a, $b];
来源：http://dus.yvedp.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://fdy.hnxiangtu.top

TS:   return { a, b };
来源：http://wsk.cashguo.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://leh.zhaomingkeji.xyz

Go:   return a, b
来源：http://sbd.hnqzz.top

Ruby: return a, b
来源：http://zok.iojbl.cn

C#:   return (a, b);              // ValueTuple
来源：http://rie.smart0.xyz

[C06] 匿名函数 / lambda
来源：http://qvu.ctjpmb.com

Py:   square = lambda x: x * x
来源：http://dqf.andypj.xyz

PHP:  $square = fn($x) => $x * $x;
来源：http://elw.bbcook.cn

JS:   const square = x => x * x;
来源：http://iwg.pycfn.com

TS:   const square = (x: number): number => x * x;
来源：http://fcs.birdmap.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://gdy.xinyue.icu

Go:   sq := func(x int) int { return x * x }
来源：http://qxw.dashuyun.cn

Ruby: square = ->(x) { x * x }
来源：http://afy.fanxiaobao.xyz

C#:   Func<int, int> square = x => x * x;
来源：http://mav.aibaodan.cn

[C07] 把函数作为参数传入
来源：http://kjg.yueranfly.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://suq.vehdjk.com

PHP:  array_map("strtoupper", $arr);
来源：http://wpg.zhaomingkeji.xyz

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hjb.vehdjk.com

TS:   arr.map(String)
来源：http://bca.birdmap.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://ndh.smart0.xyz

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://cby.yj20258.top

Ruby: arr.map(&:upcase)
来源：http://vqp.chenjidiqi.icu

C#:   arr.Select(s => s.ToUpper())
来源：http://hgv.fzhhl.top

[C08] 闭包
来源：http://ybi.sysykeji.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://blo.hammf.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hzs.snrcjt.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://tzv.yuxming.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://enl.hfpthk.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://yfo.zhoulong.xyz

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://xrl.shuidangran.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://ikg.hesvh.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://etw.9152youxi.cn

[C09] 递归
来源：http://nqn.fengsongda.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://zlo.gotoacloud.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://iyd.quarkkingdee.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://qox.hywenlv.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://luy.shangyingyoupin.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://lcc.dashuyun.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://fzq.vqdsnc.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://syn.andypj.xyz

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://exz.yanxiufei.cn

[C10] 变量作用域
来源：http://pem.jyoumei.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://zki.gotoacloud.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://edy.sxryk.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://pmi.quarkkingdee.top

TS:   同 JS
来源：http://mrb.xuetiantiany.cn

Java: 方法内为块级作用域
来源：http://qff.yangfankeji.com

Go:   花括号块级作用域
来源：http://rdv.guowangkeji.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://zfg.zhaomingkeji.xyz

C#:   块级作用域
来源：http://qjy.jinyuanbaomall.cn

[C11] 模块导入与导出
来源：http://ywo.jinyuanbaomall.cn

Py:   from module import func
来源：http://xuy.jlsjyb.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://bdn.fehbvm.com

JS:   export default function f() {};  import f from "./m.js";
来源：http://whx.zdqjudy.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://uqw.sxryk.cn

Java: import java.util.List;
来源：http://ryz.xylfe.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://ofk.fanxiaobao.xyz

Ruby: require "json"; require_relative "./util"
来源：http://sda.ctjpmb.com

C#:   using System.Text;
来源：http://chl.cdnleiting.top

[C12] 立即执行函数 IIFE
来源：http://wbk.sysykeji.top

Py:   (lambda: print("run"))()
来源：http://ucw.yueranfly.top

PHP:  (function () { echo "run"; })();
来源：http://yld.hesvh.cn

JS:   (() => { console.log("run"); })();
来源：http://ltm.wangdashe.top

TS:   (() => { console.log("run"); })();
来源：http://ssr.quarkkingdee.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://giw.zdqjudy.top

Go:   func() { fmt.Println("run") }()
来源：http://acr.hammf.cn

Ruby: -> { puts "run" }.call
来源：http://nhp.pycfn.com

C#:   // 无 IIFE：用静态构造函数
来源：http://yfm.zhijiandao.cn

[C13] 类型声明 / 类型注解
来源：http://ygq.ivvv.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://ewj.ywan-chungtsiang.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ttr.wangdashe.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://nkk.xingfuxueyuan.xyz

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://brx.fktsv.cn

Java: int add(int a, int b) { return a + b; }
来源：http://urf.hnqzz.top

Go:   func add(a, b int) int
来源：http://kwi.wangshuangyany.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://fsl.cucudq.cn

C#:   int Add(int a, int b) => a + b;
来源：http://duv.birdmap.top

[C14] 泛型函数
来源：http://jjv.zhengqikj.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://woe.ywan-chungtsiang.top

PHP:  // 无泛型
来源：http://kzf.xziqi.cn

JS:   // 无泛型
来源：http://unf.316326.xyz

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://cni.guannengcc.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://bwf.hysaishi.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://uib.pengpengdd.cyou

Ruby: # 无泛型
来源：http://yzz.kuanghao11.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://knh.hysaishi.cn

[C15] 解构 / 展开参数
来源：http://cit.cdnleiting.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://vnh.ppjwa.cn

PHP:  [$a, $b] = $pair;
来源：http://hoi.9152youxi.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://enb.aizwys.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://pec.guannengcc.top

Java: // 无解构
来源：http://byz.jqgfzy.top

Go:   // 无解构
来源：http://niq.jqgfzy.top

Ruby: a, b = pair
来源：http://wop.shzxlz.cn

C#:   var (a, b) = pair;
来源：http://ggw.jinqigfzy.top

[C16] 函数 / 方法重载
来源：http://zgl.yj20258888.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://ldf.fzhhl.top

PHP:  // 无重载
来源：http://sqn.fanxiaobao.xyz

JS:   // 无重载：靠 arguments.length 分支
来源：http://afb.andypj.xyz

TS:   // 用联合类型或重载签名声明
来源：http://rkl.zhoulong.xyz

Java: void f(int a) {}  void f(String a) {}
来源：http://hrx.chenjidiqi.icu

Go:   // 无重载：用不同函数名
来源：http://tsk.yj20258.top

Ruby: # 无重载：靠动态参数
来源：http://fzu.xuetiantiany.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://vtl.gogol.net.cn

================================================================================
来源：http://hlj.fzhhl.top

D. 数组 / 列表 / 集合
来源：http://wlm.yfazqb.com

================================================================================
来源：http://qak.zhengqikj.top

[D01] 创建数组 / 列表
来源：http://lyt.jinqigfzy.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://xpp.uphjek.com

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://tto.hongshengwenyu.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://qdj.zycfv.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://eau.shanyushiyangkeji.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://qiq.tian-w.cn

Go:   arr := []int{1, 2, 3}
来源：http://ems.guowangkeji.top

Ruby: arr = [1, 2, 3]
来源：http://kbs.fktsv.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://cjf.jinyuanbaomall.cn

[D02] 追加元素到末尾
来源：http://lqz.9152youxi.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://afq.zhongyouzk.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://dqn.sjlbkw.cn

JS:   arr.push(4);
来源：http://tob.daria6918.cn

TS:   arr.push(4);
来源：http://qug.sxryk.cn

Java: list.add(4);
来源：http://uza.yonumen.top

Go:   arr = append(arr, 4)
来源：http://bvy.guannengcc.top

Ruby: arr << 4; arr.push(5)
来源：http://yto.zhongyouzk.top

C#:   list.Add(4);
来源：http://nee.tianlin.xyz

[D03] 在指定位置插入元素
来源：http://bxg.jinqigfzy.top

Py:   arr.insert(0, 0)
来源：http://yyf.zhaomingkeji.xyz

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://xsf.haohaochexian.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://oda.ppjwa.cn

TS:   arr.splice(0, 0, 0);
来源：http://asq.jinghuilouyu.cn

Java: list.add(0, 0);
来源：http://lnw.guowangkeji.top

Go:   arr = append([]int{0}, arr...)
来源：http://qkv.guowangkeji.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://uxv.zdbjq.cn

C#:   list.Insert(0, 0);
来源：http://tmb.chenzaomai.com

[D04] 删除元素
来源：http://nvv.yuxming.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://nwl.tian-w.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://fjd.cqqwz.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://sin.smart0.xyz

TS:   arr.splice(0, 1);
来源：http://irx.jinghuilouyu.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://xrh.zhijiandao.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://nyj.ywan-chungtsiang.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://rbd.fengsongda.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://ymz.yj20258888.top

[D05] 访问与修改元素
来源：http://kwy.yfazqb.com

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://pdq.sxryk.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://noj.zhaomingkeji.xyz

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://cta.ybcxt.top

TS:   arr[0]; arr.at(-1);
来源：http://zki.chenjidiqi.icu

Java: list.get(0); list.set(0, 9);
来源：http://esy.jqgfzy.top

Go:   arr[0]; arr[0] = 9
来源：http://bfq.zhiwuduotai.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://ekc.jinghuilouyu.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://ney.snrcjt.cn

[D06] 数组长度
来源：http://zax.yuxming.cn

Py:   len(arr)
来源：http://khb.jinqigfzy.top

PHP:  count($arr);
来源：http://ebg.yuanzhike.top

JS:   arr.length
来源：http://dho.cashguo.top

TS:   arr.length
来源：http://imm.gotoacloud.top

Java: list.size();
来源：http://lqv.hnqzz.top

Go:   len(arr)
来源：http://qsp.yuanzhike.top

Ruby: arr.length; arr.size
来源：http://gid.aibaodan.cn

C#:   list.Count;
来源：http://yyy.chenjidiqi.icu

[D07] 切片 / 取子数组
来源：http://bep.hfpthk.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hnf.uphjek.com

PHP:  array_slice($arr, 1, 3);
来源：http://tvj.dianchejie.cn

JS:   arr.slice(1, 4);
来源：http://cof.uphjek.com

TS:   arr.slice(1, 4);
来源：http://xzu.smart0.xyz

Java: list.subList(1, 4);
来源：http://eln.cdnleiting.top

Go:   arr[1:4]
来源：http://maz.vehdjk.com

Ruby: arr[1, 3]
来源：http://wqz.dashuyun.cn

C#:   list.GetRange(1, 3);
来源：http://zbd.hnqzz.top

[D08] 合并两个数组
来源：http://mle.hywenlv.cn

Py:   a + b;  a.extend(b)
来源：http://qbu.zhoulong.xyz

PHP:  array_merge($a, $b);
来源：http://bkv.cdnleiting.top

JS:   [...a, ...b];  a.concat(b);
来源：http://nwi.xziqi.cn

TS:   [...a, ...b];
来源：http://sbr.yj20258.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://nch.yonumen.top

Go:   append(a, b...)
来源：http://lkx.jinqigfzy.top

Ruby: a + b;  a.concat(b)
来源：http://fhz.bjfxy.top

C#:   a.Concat(b).ToList()
来源：http://svo.yj202588.top

[D09] 排序（升序）
来源：http://mib.yuanzhike.top

Py:   sorted(arr);  arr.sort()
来源：http://vaf.chenzaomai.com

PHP:  sort($arr);
来源：http://ocb.52xcode.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://gwp.sxryk.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://kyb.zycfv.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://hnj.zdqjudy.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://gcs.iojbl.cn

Ruby: arr.sort
来源：http://tgt.ctjpmb.com

C#:   list.Sort();
来源：http://lgo.jlsjyb.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://via.yvedp.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://onk.zhengqikj.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wwb.9152youxi.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://pjz.fengsongda.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://udq.yongpay.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://rwb.sweek.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://rxj.9152youxi.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://gzx.zhongyouzk.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://fhb.ywan-chungtsiang.top

[D11] 反转数组
来源：http://bdc.nanxuanxn.top

Py:   arr[::-1];  arr.reverse()
来源：http://qfy.chenzaomai.com

PHP:  array_reverse($arr);
来源：http://meg.bjfxy.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://mtw.hcnkem.com

TS:   [...arr].reverse();
来源：http://acx.chenlongwang.top

Java: Collections.reverse(list);
来源：http://sjp.yuanzhike.top

Go:   slices.Reverse(arr)
来源：http://pmo.ydzc1.top

Ruby: arr.reverse
来源：http://tbz.dashuyun.cn

C#:   list.Reverse();
来源：http://isj.gaohongyu789.top

[D12] 查找元素下标
来源：http://pie.uphjek.com

Py:   arr.index(x);  x in arr
来源：http://dpr.yongpay.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://gjd.hfpthk.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hph.hnxiangtu.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ejg.sweek.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://kvh.9152youxi.cn

Go:   slices.Index(arr, x)
来源：http://xep.fktsv.cn

Ruby: arr.index(x)
来源：http://euf.xingfuxueyuan.xyz

C#:   list.IndexOf(x);
来源：http://jll.gotoacloud.top

[D13] 过滤（保留满足条件的）
来源：http://mvm.yueranfly.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://czf.hongshengwenyu.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://ivo.yuanzhike.top

JS:   arr.filter(x => x > 3)
来源：http://fcf.hesvh.cn

TS:   arr.filter(x => x > 3)
来源：http://gib.guannengcc.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://yst.gogol.net.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://iuk.tanke756.top

Ruby: arr.select { |x| x > 3 }
来源：http://nwx.zhijiandao.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://gam.sufxvd.cn

[D14] 映射转换（每个元素变形）
来源：http://pjt.guowangkeji.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://yzw.ybcxt.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://azm.jyoumei.cn

JS:   arr.map(x => x * 2)
来源：http://xks.fehbvm.com

TS:   arr.map(x => x * 2)
来源：http://kst.shuidangran.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://blm.sjlbkw.cn

Go:   // 手写循环
来源：http://pky.hysaishi.cn

Ruby: arr.map { |x| x * 2 }
来源：http://rsg.sufxvd.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://egg.bjfxy.top

[D15] 去重
来源：http://srx.jinqigfzy.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://sqx.yvedp.cn

PHP:  array_unique($arr);
来源：http://leh.hammf.cn

JS:   [...new Set(arr)]
来源：http://hov.sjlbkw.cn

TS:   [...new Set(arr)]
来源：http://zaz.jqgufenzy.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://rhs.xinyue.icu

Go:   // 用 map[T]struct{} 手写
来源：http://xuc.shanyushiyangtech.top

Ruby: arr.uniq
来源：http://yyv.yangfankeji.com

C#:   list.Distinct().ToList()
来源：http://alg.jiagoushi.top

[D16] 求和与平均值
来源：http://prj.zhoulong.xyz

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://qgw.ydjk.org.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://jve.dashuyun.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://onw.guowangkeji.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://pkf.nwbrower.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://vor.zhaomingkeji.xyz

Go:   // 手写循环累加
来源：http://zta.hesvh.cn


<!-- 参考信息 -->