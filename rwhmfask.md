代发 wailian999

Go:   // 无：用配置结构体参数
来源：http://nhk.sysykeji.top

Ruby: f(a: 1, b: 2)
来源：http://kbe.aibaodan.cn

C#:   f(a: 1, b: 2)
来源：http://cjv.shzxlz.cn

[C05] 返回多个值
来源：http://qye.zdqjudy.top

Py:   return a, b
来源：http://mgp.hammf.cn

PHP:  return [$a, $b];
来源：http://dey.c1oappe.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://hay.wangshuangyany.cn

TS:   return { a, b };
来源：http://bxi.yanxiufei.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://pfz.aizwys.cn

Go:   return a, b
来源：http://hpf.hnxiangtu.top

Ruby: return a, b
来源：http://uto.hnqzz.top

C#:   return (a, b);              // ValueTuple
来源：http://xqo.fzhhl.top

[C06] 匿名函数 / lambda
来源：http://oqh.yj20258.top

Py:   square = lambda x: x * x
来源：http://duh.jiagoushi.top

PHP:  $square = fn($x) => $x * $x;
来源：http://xsd.316326.xyz

JS:   const square = x => x * x;
来源：http://kdy.yanxiufei.cn

TS:   const square = (x: number): number => x * x;
来源：http://tmu.cqqwz.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://ahp.bjfxy.top

Go:   sq := func(x int) int { return x * x }
来源：http://zia.nanxuanxn.top

Ruby: square = ->(x) { x * x }
来源：http://igt.bbcook.cn

C#:   Func<int, int> square = x => x * x;
来源：http://psa.ydzc1.top

[C07] 把函数作为参数传入
来源：http://btk.cucudq.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://nje.yongpay.top

PHP:  array_map("strtoupper", $arr);
来源：http://cbk.9152youxi.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://lhu.xingfuxueyuan.xyz

TS:   arr.map(String)
来源：http://hwb.zhiwuduotai.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://cly.gzhubu.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://sly.sjlbkw.cn

Ruby: arr.map(&:upcase)
来源：http://rju.kuanghao11.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://sxv.jinghuilouyu.cn

[C08] 闭包
来源：http://jrm.hywenlv.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://ceo.tanke756.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://zcp.mhx1999.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://apx.pycfn.com

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://mjp.yj20258888.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://wqz.sweek.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://yxh.zhijiandao.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://lmf.zhongyouzk.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://eco.chenzaomai.com

[C09] 递归
来源：http://uln.zhongyouzk.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://fug.quarkkingdee.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://tem.jinqigfzy.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mfx.dashuyun.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://yey.meibo888.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://gsh.yj20258.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://lxt.guannengcc.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://evq.guannengcc.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://dou.daria6918.cn

[C10] 变量作用域
来源：http://xgt.zycfv.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://lcy.yanxiufei.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://ljm.ppjwa.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://bfy.hywenlv.cn

TS:   同 JS
来源：http://rvm.ydjk.org.cn

Java: 方法内为块级作用域
来源：http://xdo.xingfuxueyuan.xyz

Go:   花括号块级作用域
来源：http://gsz.dianchejie.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://efs.52xcode.cn

C#:   块级作用域
来源：http://rki.wangdashe.top

[C11] 模块导入与导出
来源：http://qss.cdnleiting.top

Py:   from module import func
来源：http://sby.yj20258.top

PHP:  require "file.php";  或 use App\Service;
来源：http://yjd.zdqjudy.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://waj.yongpay.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://ezk.yueranfly.top

Java: import java.util.List;
来源：http://lqs.epnwcf.com

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://zpg.nanxuanxn.top

Ruby: require "json"; require_relative "./util"
来源：http://lvt.xingfuxueyuan.xyz

C#:   using System.Text;
来源：http://pfv.tian-w.cn

[C12] 立即执行函数 IIFE
来源：http://ywv.gaohongyu789.top

Py:   (lambda: print("run"))()
来源：http://vno.hongshengwenyu.top

PHP:  (function () { echo "run"; })();
来源：http://ime.xingfuxueyuan.xyz

JS:   (() => { console.log("run"); })();
来源：http://kcv.cdnleiting.top

TS:   (() => { console.log("run"); })();
来源：http://csa.wangdashe.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://wyq.hnqzz.top

Go:   func() { fmt.Println("run") }()
来源：http://imm.bjfxy.top

Ruby: -> { puts "run" }.call
来源：http://vgh.chenjidiqi.icu

C#:   // 无 IIFE：用静态构造函数
来源：http://pdz.svipenyu.cn

[C13] 类型声明 / 类型注解
来源：http://xze.cheryme.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://tmj.316326.xyz

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://uac.zhongyouzk.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://acl.shuidangran.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://urn.meibo888.top

Java: int add(int a, int b) { return a + b; }
来源：http://fxi.mhx1999.top

Go:   func add(a, b int) int
来源：http://ear.yvedp.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hcx.jqgufenzy.top

C#:   int Add(int a, int b) => a + b;
来源：http://bbk.jqgufenzy.top

[C14] 泛型函数
来源：http://pcq.316326.xyz

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://nua.xuanzx.com

PHP:  // 无泛型
来源：http://idz.jinyuanbaomall.cn

JS:   // 无泛型
来源：http://hjl.tarul.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://trq.hcnkem.com

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://adf.chenlongwang.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://yta.tarul.cn

Ruby: # 无泛型
来源：http://uzh.tian-w.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://oan.xinyue.icu

[C15] 解构 / 展开参数
来源：http://idy.tianlin.xyz

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://clu.shangyingyoupin.top

PHP:  [$a, $b] = $pair;
来源：http://chy.shanyushiyangtech.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://bcp.sjlbkw.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://lre.hfpthk.cn

Java: // 无解构
来源：http://vpr.xylfe.cn

Go:   // 无解构
来源：http://guy.shuidangran.top

Ruby: a, b = pair
来源：http://ebq.zhixingplan.top

C#:   var (a, b) = pair;
来源：http://pxj.bbcook.cn

[C16] 函数 / 方法重载
来源：http://bmt.gzhubu.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://xnn.chenjidiqi.icu

PHP:  // 无重载
来源：http://uwh.xingfuxueyuan.xyz

JS:   // 无重载：靠 arguments.length 分支
来源：http://vse.bbcook.cn

TS:   // 用联合类型或重载签名声明
来源：http://hdk.hywenlv.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://qho.guowangkeji.top

Go:   // 无重载：用不同函数名
来源：http://zut.yangfankeji.com

Ruby: # 无重载：靠动态参数
来源：http://jhl.zhiwuduotai.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://jke.bbcook.cn

================================================================================
来源：http://kzg.kuanghao11.cn

D. 数组 / 列表 / 集合
来源：http://smg.yj202588.top

================================================================================
来源：http://kre.nwbrower.top

[D01] 创建数组 / 列表
来源：http://pgo.svipenyu.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://gmx.nanxuanxn.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://muy.snrcjt.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://fix.gogol.net.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://kla.shangyingyoupin.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://qxx.sweek.top

Go:   arr := []int{1, 2, 3}
来源：http://sqo.guowangkeji.top

Ruby: arr = [1, 2, 3]
来源：http://apc.jinyuanbaomall.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://sdi.yfazqb.com

[D02] 追加元素到末尾
来源：http://bcc.guannengcc.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://qfz.hnxiangtu.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://afb.chenlongwang.top

JS:   arr.push(4);
来源：http://mbl.zhijiandao.cn

TS:   arr.push(4);
来源：http://xba.cdnleiting.top

Java: list.add(4);
来源：http://jdn.zdbjq.cn

Go:   arr = append(arr, 4)
来源：http://rjo.yj20258.top

Ruby: arr << 4; arr.push(5)
来源：http://kig.tian-w.cn

C#:   list.Add(4);
来源：http://xyi.yj20258.top

[D03] 在指定位置插入元素
来源：http://ivj.yj20258.top

Py:   arr.insert(0, 0)
来源：http://laz.ehwqpu.com

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://esf.zhiwuduotai.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://rho.jyoumei.cn

TS:   arr.splice(0, 0, 0);
来源：http://xoq.cashguo.top

Java: list.add(0, 0);
来源：http://ajf.ivvv.top

Go:   arr = append([]int{0}, arr...)
来源：http://doc.xziqi.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://bal.fzhhl.top

C#:   list.Insert(0, 0);
来源：http://evt.hammf.cn

[D04] 删除元素
来源：http://rjc.zdbjq.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://unm.zhaomingkeji.xyz

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://cwl.jinqigufen.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://osr.gzhubu.top

TS:   arr.splice(0, 1);
来源：http://puw.zhengqikj.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://spo.yueranfly.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://bcc.ehwqpu.com

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://tse.jianghu66.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://tpu.bbcook.cn

[D05] 访问与修改元素
来源：http://kiy.cheryme.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://oop.smart0.xyz

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://iki.xziqi.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://spe.xylfe.cn

TS:   arr[0]; arr.at(-1);
来源：http://ckc.gotoacloud.top

Java: list.get(0); list.set(0, 9);
来源：http://kwk.yongpay.top

Go:   arr[0]; arr[0] = 9
来源：http://tlx.shanyushiyangtech.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://nwc.hcnkem.com

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://wxz.yueranfly.top

[D06] 数组长度
来源：http://duo.zdbjq.cn

Py:   len(arr)
来源：http://wej.sufxvd.cn

PHP:  count($arr);
来源：http://nxh.gzhubu.top

JS:   arr.length
来源：http://whk.jinghuilouyu.cn

TS:   arr.length
来源：http://dzt.xingfuxueyuan.xyz

Java: list.size();
来源：http://kdl.sjlbkw.cn

Go:   len(arr)
来源：http://mso.nwbrower.top

Ruby: arr.length; arr.size
来源：http://lpw.hongshengwenyu.top

C#:   list.Count;
来源：http://vok.yj20258888.top

[D07] 切片 / 取子数组
来源：http://udk.jqgufenzy.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://zxf.shanyushiyangkeji.top

PHP:  array_slice($arr, 1, 3);
来源：http://chj.birdmap.top

JS:   arr.slice(1, 4);
来源：http://qmn.daria6918.cn

TS:   arr.slice(1, 4);
来源：http://onh.jinghuilouyu.cn

Java: list.subList(1, 4);
来源：http://azl.yfazqb.com

Go:   arr[1:4]
来源：http://czw.gotoacloud.top

Ruby: arr[1, 3]
来源：http://llm.nanxinkj.top

C#:   list.GetRange(1, 3);
来源：http://uyf.zhixingplan.top

[D08] 合并两个数组
来源：http://aka.xziqi.cn

Py:   a + b;  a.extend(b)
来源：http://kvm.vehdjk.com

PHP:  array_merge($a, $b);
来源：http://zqm.hfpthk.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://dpe.yj20258.top

TS:   [...a, ...b];
来源：http://ytf.yongpay.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://vls.jqgfzy.top

Go:   append(a, b...)
来源：http://kqu.birdmap.top

Ruby: a + b;  a.concat(b)
来源：http://rno.zdbjq.cn

C#:   a.Concat(b).ToList()
来源：http://ygh.yonumen.top

[D09] 排序（升序）
来源：http://orx.guannengcc.top

Py:   sorted(arr);  arr.sort()
来源：http://mag.jinqigufen.top

PHP:  sort($arr);
来源：http://nld.xuetiantiany.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://gnq.shuidangran.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://xac.fktsv.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://byt.ywan-chungtsiang.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://smh.yvedp.cn

Ruby: arr.sort
来源：http://fky.yj20258888.top

C#:   list.Sort();
来源：http://cmn.zhengqikj.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://csx.yangfankeji.com

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://ujg.hammf.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://atd.shangyingyoupin.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://rjn.ydjk.org.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://ufw.quarkkingdee.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://wop.cqqwz.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://fsi.jiagoushi.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://rum.yj20258888.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hlx.zhengqikj.top

[D11] 反转数组
来源：http://rja.hongshengwenyu.top

Py:   arr[::-1];  arr.reverse()
来源：http://cma.zhaomingkeji.xyz

PHP:  array_reverse($arr);
来源：http://fjq.jqgfzy.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://osx.shzxlz.cn

TS:   [...arr].reverse();
来源：http://ief.birdmap.top

Java: Collections.reverse(list);
来源：http://qsq.tianlin.xyz

Go:   slices.Reverse(arr)
来源：http://fgd.xinyue.icu

Ruby: arr.reverse
来源：http://mjw.meibo888.top

C#:   list.Reverse();
来源：http://jgj.kuanghao11.cn

[D12] 查找元素下标
来源：http://wzx.zdbjq.cn

Py:   arr.index(x);  x in arr
来源：http://iau.yongpay.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hjj.dashuyun.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ndg.nanxuanxn.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://xhb.aibaodan.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://oux.hywenlv.cn

Go:   slices.Index(arr, x)
来源：http://dgh.yfazqb.com

Ruby: arr.index(x)
来源：http://old.tianlin.xyz

C#:   list.IndexOf(x);
来源：http://ydp.aibaodan.cn

[D13] 过滤（保留满足条件的）
来源：http://fyr.yonumen.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://qqw.hfpthk.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://vqy.pycfn.com

JS:   arr.filter(x => x > 3)
来源：http://jbn.gzhubu.top

TS:   arr.filter(x => x > 3)
来源：http://kph.cqqwz.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://rgd.xuetiantiany.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://bsn.chenjidiqi.icu

Ruby: arr.select { |x| x > 3 }
来源：http://rqw.aibaodan.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://pya.tianlin.xyz

[D14] 映射转换（每个元素变形）
来源：http://tkw.havefunace.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://yjm.ydjk.org.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://ewo.dashuyun.cn

JS:   arr.map(x => x * 2)
来源：http://lma.fengsongda.top

TS:   arr.map(x => x * 2)
来源：http://hmj.hcnkem.com

Java: list.stream().map(x -> x * 2).toList()
来源：http://aiz.aibaodan.cn

Go:   // 手写循环
来源：http://xgp.cqqwz.cn

Ruby: arr.map { |x| x * 2 }
来源：http://qsx.yonumen.top

C#:   list.Select(x => x * 2).ToList()
来源：http://bjs.uphjek.com

[D15] 去重
来源：http://ttj.sysykeji.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://cog.52xcode.cn

PHP:  array_unique($arr);
来源：http://jdx.316326.xyz

JS:   [...new Set(arr)]
来源：http://nsj.hammf.cn

TS:   [...new Set(arr)]
来源：http://cgd.nanxinkj.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://lsk.hysaishi.cn

Go:   // 用 map[T]struct{} 手写
来源：http://ase.sjlbkw.cn

Ruby: arr.uniq
来源：http://ykg.xylfe.cn

C#:   list.Distinct().ToList()
来源：http://qud.jlsjyb.cn

[D16] 求和与平均值
来源：http://spo.jinqigfzy.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://vfp.tanke756.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://avu.cucudq.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://yia.yueranfly.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://ogs.nwbrower.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://zfi.fktsv.cn

Go:   // 手写循环累加
来源：http://dio.ppjwa.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://vro.jiagoushi.top

C#:   list.Sum();  list.Average()
来源：http://fcy.fktsv.cn

[D17] 最大值与最小值
来源：http://jpt.xinyue.icu

Py:   max(arr);  min(arr)
来源：http://nyv.guowangkeji.top

PHP:  max($arr);  min($arr);
来源：http://qxv.zhijiandao.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://mcx.wangdashe.top

TS:   Math.max(...arr);
来源：http://rnu.nanxinkj.top

Java: Collections.max(list);  Collections.min(list);
来源：http://onh.hysaishi.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://ufs.redwolf501.top

Ruby: arr.max;  arr.min
来源：http://rxe.zdqjudy.top

C#:   list.Max();  list.Min()
来源：http://olv.pycfn.com

[D18] 扁平化嵌套数组
来源：http://thy.svipenyu.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://lrm.quarkkingdee.top

PHP:  array_merge(...$nested);
来源：http://ckj.cucudq.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hek.bjfxy.top

TS:   nested.flat();
来源：http://qvb.gotoacloud.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://oax.sufxvd.cn

Go:   // 手写双层循环
来源：http://zjf.iojbl.cn

Ruby: nested.flatten
来源：http://dtx.sufxvd.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://qjm.shanyushiyangkeji.top

[D19] 按字段分组
来源：http://rpq.hnxiangtu.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://ztg.chenlongwang.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://zxq.zhoulong.xyz

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://tjq.tanke756.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://yme.shanyushiyangtech.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://coz.hesvh.cn

Go:   // 手写 map[string][]T
来源：http://wbl.jqgfzy.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://orb.sysykeji.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://rff.daria6918.cn

[D20] 统计每个元素出现次数
来源：http://olj.zdbjq.cn

Py:   Counter(arr)
来源：http://fzj.ywan-chungtsiang.top

PHP:  array_count_values($arr);
来源：http://acx.fehbvm.com

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ezf.ppjwa.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://rjj.jqgufenzy.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://rsd.shanyushiyangtech.top

Go:   // 手写 map[T]int
来源：http://kos.ydzc1.top

Ruby: arr.tally
来源：http://wfe.hnqzz.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://ekw.fktsv.cn

[D21] 判断是否包含某元素
来源：http://ndh.jqgufenzy.top

Py:   x in arr
来源：http://fti.ctjpmb.com

PHP:  in_array($x, $arr, true);
来源：http://xeq.bjfxy.top

JS:   arr.includes(x)
来源：http://cue.zhijiandao.cn

TS:   arr.includes(x)
来源：http://tbm.shuidangran.top

Java: list.contains(x)
来源：http://kke.ehwqpu.com


<!-- 参考信息 -->