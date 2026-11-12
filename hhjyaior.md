代发 wailian999

Java: if (data == null) return;
来源：http://ntw.gotoacloud.top

Go:   if data == nil { return }
来源：http://fpy.jqgufenzy.top

Ruby: return if data.nil?
来源：http://kek.shanyushiyangkeji.top

C#:   if (data == null) return;
来源：http://qvt.andypj.xyz

================================================================================
来源：http://oid.shanyushiyangtech.top

C. 函数与作用域
来源：http://lqo.jianghu66.top

================================================================================
来源：http://enr.gaohongyu789.top

[C01] 定义函数
来源：http://npg.chenzaomai.com

Py:   def add(a, b): return a + b
来源：http://swh.zhoulong.xyz

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://snl.yueranfly.top

JS:   function add(a, b) { return a + b; }
来源：http://aai.hammf.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://puc.cheryme.top

Java: static int add(int a, int b) { return a + b; }
来源：http://eqz.cdnleiting.top

Go:   func add(a, b int) int { return a + b }
来源：http://gdh.nwbrower.top

Ruby: def add(a, b); a + b; end
来源：http://hlx.hongshengwenyu.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://tuz.pycfn.com

[C02] 默认参数
来源：http://rca.bbcook.cn

Py:   def greet(name="World"): return name
来源：http://wzo.yj20258888.top

PHP:  function greet($name = "World") { return $name; }
来源：http://tcz.havefunace.top

JS:   function greet(name = "World") { return name; }
来源：http://spr.ydzc1.top

TS:   function greet(name: string = "World") { return name; }
来源：http://pjx.yj20258.top

Java: // 无默认参数：方法重载或 Optional
来源：http://gtl.dianchejie.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://zqw.ehwqpu.com

Ruby: def greet(name = "World") = name
来源：http://ytx.sweek.top

C#:   string Greet(string name = "World") => name;
来源：http://lab.wangshuangyany.cn

[C03] 可变参数
来源：http://dkp.hnxiangtu.top

Py:   def total(*args): return sum(args)
来源：http://ypg.yfazqb.com

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://kad.ydzc1.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://ago.zdqjudy.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://scj.shangyingyoupin.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://gxy.cqqwz.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://qtb.fzhhl.top

Ruby: def total(*nums); nums.sum; end
来源：http://uep.cucudq.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://vks.yongpay.top

[C04] 命名参数 / 关键字参数
来源：http://csm.feifeiyinyue.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://ifo.yanxiufei.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://chu.zhengqikj.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://rtf.xylfe.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://kuu.svipenyu.cn

Java: // 无：用 Builder 模式或 record
来源：http://pnt.tianlin.xyz

Go:   // 无：用配置结构体参数
来源：http://esk.jyoumei.cn

Ruby: f(a: 1, b: 2)
来源：http://ppx.iojbl.cn

C#:   f(a: 1, b: 2)
来源：http://gxj.yongpay.top

[C05] 返回多个值
来源：http://jvr.bjfxy.top

Py:   return a, b
来源：http://wub.svipenyu.cn

PHP:  return [$a, $b];
来源：http://jis.redwolf501.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://jlu.jinqigufen.top

TS:   return { a, b };
来源：http://anf.hcnkem.com

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://lni.zhongyouzk.top

Go:   return a, b
来源：http://rgn.cucudq.cn

Ruby: return a, b
来源：http://epg.shanyushiyangkeji.top

C#:   return (a, b);              // ValueTuple
来源：http://hhn.wangdashe.top

[C06] 匿名函数 / lambda
来源：http://kqi.316326.xyz

Py:   square = lambda x: x * x
来源：http://acs.bjfxy.top

PHP:  $square = fn($x) => $x * $x;
来源：http://ybr.cucudq.cn

JS:   const square = x => x * x;
来源：http://wht.dashuyun.cn

TS:   const square = (x: number): number => x * x;
来源：http://cmy.ybcxt.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://lhx.hongshengwenyu.top

Go:   sq := func(x int) int { return x * x }
来源：http://ozc.chenjidiqi.icu

Ruby: square = ->(x) { x * x }
来源：http://kfm.xinyue.icu

C#:   Func<int, int> square = x => x * x;
来源：http://asi.ivvv.top

[C07] 把函数作为参数传入
来源：http://mii.zhaomingkeji.xyz

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://ztg.guowangkeji.top

PHP:  array_map("strtoupper", $arr);
来源：http://zlr.ctjpmb.com

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://mgn.xinyue.icu

TS:   arr.map(String)
来源：http://sso.haohaochexian.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://vfa.cheryme.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://buz.shangyingyoupin.top

Ruby: arr.map(&:upcase)
来源：http://oap.jqgufenzy.top

C#:   arr.Select(s => s.ToUpper())
来源：http://cex.yuxming.cn

[C08] 闭包
来源：http://udx.jqgufenzy.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://aop.aizwys.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://tie.zhaomingkeji.xyz

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://uac.gzhubu.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://ypt.ydzc1.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://jyj.yvedp.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://gih.hammf.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://lye.gogol.net.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://oyq.gotoacloud.top

[C09] 递归
来源：http://dbl.yvedp.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://aho.jinghuilouyu.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://fkf.shanyushiyangkeji.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://fhn.zhiwuduotai.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://yvk.zhiwuduotai.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://rfu.uphjek.com

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://dyc.zhongyouzk.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://kma.fzhhl.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://bxt.hnxiangtu.top

[C10] 变量作用域
来源：http://vgr.yvedp.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://dbt.ppjwa.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://std.fktsv.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://gsc.yfazqb.com

TS:   同 JS
来源：http://bce.aizwys.cn

Java: 方法内为块级作用域
来源：http://ciu.yfazqb.com

Go:   花括号块级作用域
来源：http://vme.wangdashe.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://esk.bjfxy.top

C#:   块级作用域
来源：http://tva.cdnleiting.top

[C11] 模块导入与导出
来源：http://vzh.daria6918.cn

Py:   from module import func
来源：http://roi.pycfn.com

PHP:  require "file.php";  或 use App\Service;
来源：http://jze.gaohongyu789.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://qlo.jinghuilouyu.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://cgw.ppjwa.cn

Java: import java.util.List;
来源：http://mrs.xingfuxueyuan.xyz

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://lfx.fktsv.cn

Ruby: require "json"; require_relative "./util"
来源：http://ekf.tianlin.xyz

C#:   using System.Text;
来源：http://xyn.gotoacloud.top

[C12] 立即执行函数 IIFE
来源：http://kqo.ppjwa.cn

Py:   (lambda: print("run"))()
来源：http://rqz.fengsongda.top

PHP:  (function () { echo "run"; })();
来源：http://yia.sweek.top

JS:   (() => { console.log("run"); })();
来源：http://vsz.9152youxi.cn

TS:   (() => { console.log("run"); })();
来源：http://cou.tanke756.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://ceb.yangfankeji.com

Go:   func() { fmt.Println("run") }()
来源：http://ilm.shuidangran.top

Ruby: -> { puts "run" }.call
来源：http://cxf.shangyingyoupin.top

C#:   // 无 IIFE：用静态构造函数
来源：http://lcc.hfpthk.cn

[C13] 类型声明 / 类型注解
来源：http://dqj.guowangkeji.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://coc.quarkkingdee.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wog.zhoulong.xyz

JS:   // 无类型（可用 JSDoc 注释）
来源：http://zyo.jinqigufen.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://gat.yongpay.top

Java: int add(int a, int b) { return a + b; }
来源：http://hyw.yonumen.top

Go:   func add(a, b int) int
来源：http://jkl.uphjek.com

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://ert.yj202588.top

C#:   int Add(int a, int b) => a + b;
来源：http://yry.yj20258888.top

[C14] 泛型函数
来源：http://aeu.gzhubu.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://ueu.dashuyun.cn

PHP:  // 无泛型
来源：http://tzx.yvedp.cn

JS:   // 无泛型
来源：http://qxu.cheryme.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://nrh.yangfankeji.com

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://pkp.mhx1999.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://lkk.c1oappe.top

Ruby: # 无泛型
来源：http://agz.pengpengdd.cyou

C#:   static T First<T>(List<T> items) => items[0];
来源：http://fnq.zhaomingkeji.xyz

[C15] 解构 / 展开参数
来源：http://elq.dianchejie.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://ast.sjlbkw.cn

PHP:  [$a, $b] = $pair;
来源：http://nvx.daria6918.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://rpv.tian-w.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://cur.yuxming.cn

Java: // 无解构
来源：http://yta.hnxiangtu.top

Go:   // 无解构
来源：http://ses.svipenyu.cn

Ruby: a, b = pair
来源：http://lhd.aizwys.cn

C#:   var (a, b) = pair;
来源：http://jaj.gaohongyu789.top

[C16] 函数 / 方法重载
来源：http://ard.shuidangran.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://meg.zdqjudy.top

PHP:  // 无重载
来源：http://det.yfazqb.com

JS:   // 无重载：靠 arguments.length 分支
来源：http://cwq.xziqi.cn

TS:   // 用联合类型或重载签名声明
来源：http://pks.9152youxi.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://iws.chenlongwang.top

Go:   // 无重载：用不同函数名
来源：http://mbj.pycfn.com

Ruby: # 无重载：靠动态参数
来源：http://dxc.xziqi.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://rdc.ppjwa.cn

================================================================================
来源：http://ntm.fktsv.cn

D. 数组 / 列表 / 集合
来源：http://rxp.epnwcf.com

================================================================================
来源：http://sur.smart0.xyz

[D01] 创建数组 / 列表
来源：http://xaq.c1oappe.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://aqd.epnwcf.com

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://zcf.havefunace.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://dga.jinghuilouyu.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://yqu.birdmap.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://keu.dianchejie.cn

Go:   arr := []int{1, 2, 3}
来源：http://qpz.yuanzhike.top

Ruby: arr = [1, 2, 3]
来源：http://czc.yj20258888.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://lto.hnqzz.top

[D02] 追加元素到末尾
来源：http://hhb.zhongyouzk.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://zqh.zdbjq.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://eri.sweek.top

JS:   arr.push(4);
来源：http://wfn.gzhubu.top

TS:   arr.push(4);
来源：http://rbz.yuxming.cn

Java: list.add(4);
来源：http://pdw.dashuyun.cn

Go:   arr = append(arr, 4)
来源：http://eqy.xingfuxueyuan.xyz

Ruby: arr << 4; arr.push(5)
来源：http://lvr.meibo888.top

C#:   list.Add(4);
来源：http://bia.zhongyouzk.top

[D03] 在指定位置插入元素
来源：http://rxq.tianlin.xyz

Py:   arr.insert(0, 0)
来源：http://aqs.shanyushiyangkeji.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://klr.yj202588.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://qug.zdqjudy.top

TS:   arr.splice(0, 0, 0);
来源：http://cyj.jinqigufen.top

Java: list.add(0, 0);
来源：http://rud.sxryk.cn

Go:   arr = append([]int{0}, arr...)
来源：http://azr.yj20258888.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://rnm.jlsjyb.cn

C#:   list.Insert(0, 0);
来源：http://yhu.yueranfly.top

[D04] 删除元素
来源：http://ssr.dianchejie.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://ffe.daria6918.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://boc.zhongyouzk.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://fbc.xinyue.icu

TS:   arr.splice(0, 1);
来源：http://cyz.zhengqikj.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://dkv.hammf.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://gcw.tianlin.xyz

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://nrm.zhaomingkeji.xyz

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://bvi.jinyuanbaomall.cn

[D05] 访问与修改元素
来源：http://bgg.ydjk.org.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://zpj.shangyingyoupin.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://gfw.quarkkingdee.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://fzz.chenjidiqi.icu

TS:   arr[0]; arr.at(-1);
来源：http://dof.jianghu66.top

Java: list.get(0); list.set(0, 9);
来源：http://idh.mhx1999.top

Go:   arr[0]; arr[0] = 9
来源：http://ych.hysaishi.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://wdm.jianghu66.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://agy.gogol.net.cn

[D06] 数组长度
来源：http://sis.yfazqb.com

Py:   len(arr)
来源：http://uzp.ydzc1.top

PHP:  count($arr);
来源：http://wec.cashguo.top

JS:   arr.length
来源：http://ykx.jinqigufen.top

TS:   arr.length
来源：http://snq.nwbrower.top

Java: list.size();
来源：http://wtp.fktsv.cn

Go:   len(arr)
来源：http://fbf.hysaishi.cn

Ruby: arr.length; arr.size
来源：http://iow.tarul.cn

C#:   list.Count;
来源：http://vqp.pycfn.com

[D07] 切片 / 取子数组
来源：http://vzk.jlsjyb.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://wgy.316326.xyz

PHP:  array_slice($arr, 1, 3);
来源：http://xsa.ehwqpu.com

JS:   arr.slice(1, 4);
来源：http://xnp.quarkkingdee.top

TS:   arr.slice(1, 4);
来源：http://oxk.nanxinkj.top

Java: list.subList(1, 4);
来源：http://phv.hnqzz.top

Go:   arr[1:4]
来源：http://aog.feifeiyinyue.top

Ruby: arr[1, 3]
来源：http://ecl.hesvh.cn

C#:   list.GetRange(1, 3);
来源：http://ova.gogol.net.cn

[D08] 合并两个数组
来源：http://lda.hammf.cn

Py:   a + b;  a.extend(b)
来源：http://maa.hnxiangtu.top

PHP:  array_merge($a, $b);
来源：http://cgj.zhiwuduotai.top

JS:   [...a, ...b];  a.concat(b);
来源：http://oze.gaohongyu789.top

TS:   [...a, ...b];
来源：http://ykj.jinqigfzy.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://cus.yj202588.top

Go:   append(a, b...)
来源：http://vph.daria6918.cn

Ruby: a + b;  a.concat(b)
来源：http://nvz.zycfv.cn

C#:   a.Concat(b).ToList()
来源：http://mxf.zhengqikj.top

[D09] 排序（升序）
来源：http://rzc.wangshuangyany.cn

Py:   sorted(arr);  arr.sort()
来源：http://rqt.ydzc1.top

PHP:  sort($arr);
来源：http://cpi.jqgfzy.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://ztc.dashuyun.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://zbk.sufxvd.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://aca.yj20258888.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://ccn.hammf.cn

Ruby: arr.sort
来源：http://ugy.hnxiangtu.top

C#:   list.Sort();
来源：http://ugg.ydzc1.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://bys.yuxming.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://var.tanke756.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://aen.gzhubu.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://nkd.fzhhl.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://kmu.chenzaomai.com

Java: list.sort(Comparator.comparing(Person::age));
来源：http://equ.cdnleiting.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://xxp.tian-w.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hfo.zdbjq.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://xss.yuxming.cn

[D11] 反转数组
来源：http://xor.cucudq.cn

Py:   arr[::-1];  arr.reverse()
来源：http://zbu.c1oappe.top

PHP:  array_reverse($arr);
来源：http://jns.fktsv.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://tfq.vqdsnc.cn

TS:   [...arr].reverse();
来源：http://svf.iojbl.cn

Java: Collections.reverse(list);
来源：http://wuy.xingfuxueyuan.xyz

Go:   slices.Reverse(arr)
来源：http://dlk.fktsv.cn

Ruby: arr.reverse
来源：http://upw.zdbjq.cn

C#:   list.Reverse();
来源：http://zft.sufxvd.cn

[D12] 查找元素下标
来源：http://uxr.jinyuanbaomall.cn

Py:   arr.index(x);  x in arr
来源：http://xgc.hcnkem.com

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://cwj.guowangkeji.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ugm.ydzc1.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://anf.kuanghao11.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://oiq.snrcjt.cn

Go:   slices.Index(arr, x)
来源：http://yqm.jinqigufen.top

Ruby: arr.index(x)
来源：http://whf.jinghuilouyu.cn

C#:   list.IndexOf(x);
来源：http://xyg.jiagoushi.top

[D13] 过滤（保留满足条件的）
来源：http://nyp.hammf.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://xsg.pycfn.com

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://tdi.bjfxy.top

JS:   arr.filter(x => x > 3)
来源：http://oxm.xziqi.cn

TS:   arr.filter(x => x > 3)
来源：http://xvz.gaohongyu789.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://ery.nanxuanxn.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://ikg.tanke756.top

Ruby: arr.select { |x| x > 3 }
来源：http://dzw.guannengcc.top

C#:   list.Where(x => x > 3).ToList()
来源：http://gad.cdnleiting.top

[D14] 映射转换（每个元素变形）
来源：http://ces.0kj1m.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://zkd.shanyushiyangkeji.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://geb.zhengqikj.top

JS:   arr.map(x => x * 2)
来源：http://erd.quarkkingdee.top

TS:   arr.map(x => x * 2)
来源：http://xaj.cashguo.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://wln.ctjpmb.com

Go:   // 手写循环
来源：http://gez.havefunace.top

Ruby: arr.map { |x| x * 2 }
来源：http://bun.jinyuanbaomall.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://hxh.havefunace.top

[D15] 去重
来源：http://nlc.tarul.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://eco.uphjek.com

PHP:  array_unique($arr);
来源：http://cax.gaohongyu789.top

JS:   [...new Set(arr)]
来源：http://iki.zhengqikj.top

TS:   [...new Set(arr)]
来源：http://inc.cqqwz.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://rck.nanxuanxn.top

Go:   // 用 map[T]struct{} 手写
来源：http://lxb.xuanzx.com

Ruby: arr.uniq
来源：http://swz.guannengcc.top

C#:   list.Distinct().ToList()
来源：http://rkj.tarul.cn

[D16] 求和与平均值
来源：http://vwz.hongshengwenyu.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://oii.shzxlz.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://app.yangfankeji.com

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://vmu.xziqi.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://iur.kuanghao11.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://gle.birdmap.top

Go:   // 手写循环累加
来源：http://fcz.jyoumei.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://frw.jinqigfzy.top

C#:   list.Sum();  list.Average()
来源：http://eix.nwbrower.top

[D17] 最大值与最小值
来源：http://rmt.gzhubu.top

Py:   max(arr);  min(arr)
来源：http://qmz.gaohongyu789.top


<!-- 参考信息 -->