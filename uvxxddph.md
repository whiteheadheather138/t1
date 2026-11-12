代发 wailian999

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://icy.zycfv.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://wgr.smart0.xyz

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://pap.chenlongwang.top

Java: // 无：用 Builder 模式或 record
来源：http://guf.fanxiaobao.xyz

Go:   // 无：用配置结构体参数
来源：http://rhc.guowangkeji.top

Ruby: f(a: 1, b: 2)
来源：http://gtj.tanke756.top

C#:   f(a: 1, b: 2)
来源：http://cvl.cucudq.cn

[C05] 返回多个值
来源：http://gne.hcnkem.com

Py:   return a, b
来源：http://rpd.uphjek.com

PHP:  return [$a, $b];
来源：http://sld.ivvv.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://xdb.vqdsnc.cn

TS:   return { a, b };
来源：http://wfb.vqdsnc.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://yum.hcnkem.com

Go:   return a, b
来源：http://lbm.0kj1m.cn

Ruby: return a, b
来源：http://whu.tanke756.top

C#:   return (a, b);              // ValueTuple
来源：http://scg.wangshuangyany.cn

[C06] 匿名函数 / lambda
来源：http://ybc.jyoumei.cn

Py:   square = lambda x: x * x
来源：http://zgo.hammf.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://psb.mhx1999.top

JS:   const square = x => x * x;
来源：http://djh.shzxlz.cn

TS:   const square = (x: number): number => x * x;
来源：http://tgk.aibaodan.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://ifs.guannengcc.top

Go:   sq := func(x int) int { return x * x }
来源：http://mcb.shzxlz.cn

Ruby: square = ->(x) { x * x }
来源：http://fel.52xcode.cn

C#:   Func<int, int> square = x => x * x;
来源：http://omi.smart0.xyz

[C07] 把函数作为参数传入
来源：http://inz.cashguo.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://get.hnxiangtu.top

PHP:  array_map("strtoupper", $arr);
来源：http://uyp.xziqi.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://dls.tian-w.cn

TS:   arr.map(String)
来源：http://bkr.hongshengwenyu.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://bed.zhiwuduotai.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://rcf.jlsjyb.cn

Ruby: arr.map(&:upcase)
来源：http://qua.yuanzhike.top

C#:   arr.Select(s => s.ToUpper())
来源：http://ufv.nanxinkj.top

[C08] 闭包
来源：http://cjm.c1oappe.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://jhm.316326.xyz

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://avt.zdqjudy.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://udl.vehdjk.com

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://xsz.bjfxy.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://pgo.jinqigufen.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://juc.gotoacloud.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://uyl.ppjwa.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://frg.jyoumei.cn

[C09] 递归
来源：http://zks.jianghu66.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://qpj.nwbrower.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://lah.tarul.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://zyf.zhengqikj.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mhr.ctjpmb.com

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://dqn.jinqigfzy.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://own.zhengqikj.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://mug.sufxvd.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://uml.yangfankeji.com

[C10] 变量作用域
来源：http://nwp.cashguo.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://zhm.shanyushiyangkeji.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://xmx.pycfn.com

JS:   let/const 块级作用域，var 函数级作用域
来源：http://yxx.sufxvd.cn

TS:   同 JS
来源：http://lhi.quarkkingdee.top

Java: 方法内为块级作用域
来源：http://ija.shzxlz.cn

Go:   花括号块级作用域
来源：http://pak.andypj.xyz

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://bbo.hysaishi.cn

C#:   块级作用域
来源：http://stz.pengpengdd.cyou

[C11] 模块导入与导出
来源：http://dot.birdmap.top

Py:   from module import func
来源：http://yjw.cheryme.top

PHP:  require "file.php";  或 use App\Service;
来源：http://yii.jlsjyb.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://xtt.ydjk.org.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://det.yvedp.cn

Java: import java.util.List;
来源：http://qbe.daxiang520.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://kdn.nanxinkj.top

Ruby: require "json"; require_relative "./util"
来源：http://yeo.yonumen.top

C#:   using System.Text;
来源：http://fvp.xinyue.icu

[C12] 立即执行函数 IIFE
来源：http://ony.jqgfzy.top

Py:   (lambda: print("run"))()
来源：http://lja.sxryk.cn

PHP:  (function () { echo "run"; })();
来源：http://asx.hesvh.cn

JS:   (() => { console.log("run"); })();
来源：http://ipg.gotoacloud.top

TS:   (() => { console.log("run"); })();
来源：http://iyl.andypj.xyz

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://yro.nwbrower.top

Go:   func() { fmt.Println("run") }()
来源：http://udi.ppjwa.cn

Ruby: -> { puts "run" }.call
来源：http://jgs.zycfv.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://fqj.chenjidiqi.icu

[C13] 类型声明 / 类型注解
来源：http://opw.iojbl.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hwb.chenzaomai.com

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://spx.hfpthk.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://uyt.52xcode.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hwc.jlsjyb.cn

Java: int add(int a, int b) { return a + b; }
来源：http://psw.ehwqpu.com

Go:   func add(a, b int) int
来源：http://yhl.jlsjyb.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://khs.jqgfzy.top

C#:   int Add(int a, int b) => a + b;
来源：http://myg.sufxvd.cn

[C14] 泛型函数
来源：http://uis.vqdsnc.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://zzr.shuidangran.top

PHP:  // 无泛型
来源：http://yhm.hnxiangtu.top

JS:   // 无泛型
来源：http://vzn.aibaodan.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://sws.ehwqpu.com

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://due.zhongyouzk.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://gud.shanyushiyangkeji.top

Ruby: # 无泛型
来源：http://xwo.yuanzhike.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://acc.jinghuilouyu.cn

[C15] 解构 / 展开参数
来源：http://smg.tarul.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://pbw.hysaishi.cn

PHP:  [$a, $b] = $pair;
来源：http://atu.cdnleiting.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://qkd.yfazqb.com

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://pxn.shuidangran.top

Java: // 无解构
来源：http://yvn.ppjwa.cn

Go:   // 无解构
来源：http://dhp.jinghuilouyu.cn

Ruby: a, b = pair
来源：http://rof.shzxlz.cn

C#:   var (a, b) = pair;
来源：http://ylj.haohaochexian.top

[C16] 函数 / 方法重载
来源：http://ikn.wangdashe.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://jmg.yj20258888.top

PHP:  // 无重载
来源：http://eql.zhaomingkeji.xyz

JS:   // 无重载：靠 arguments.length 分支
来源：http://rsg.sxryk.cn

TS:   // 用联合类型或重载签名声明
来源：http://zpx.yueranfly.top

Java: void f(int a) {}  void f(String a) {}
来源：http://sqn.ybcxt.top

Go:   // 无重载：用不同函数名
来源：http://dmp.uphjek.com

Ruby: # 无重载：靠动态参数
来源：http://rlg.daxiang520.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://kts.hongshengwenyu.top

================================================================================
来源：http://cdw.yj202588.top

D. 数组 / 列表 / 集合
来源：http://qvz.jianghu66.top

================================================================================
来源：http://qgw.tarul.cn

[D01] 创建数组 / 列表
来源：http://jyd.andypj.xyz

Py:   arr = [1, 2, 3];  empty = []
来源：http://nbe.shzxlz.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://gvd.sjlbkw.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://wkv.c1oappe.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://dcq.tian-w.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://snf.feifeiyinyue.top

Go:   arr := []int{1, 2, 3}
来源：http://mis.meibo888.top

Ruby: arr = [1, 2, 3]
来源：http://bal.iojbl.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://myr.316326.xyz

[D02] 追加元素到末尾
来源：http://prm.xinyue.icu

Py:   arr.append(4); arr.extend([5, 6])
来源：http://gem.jqgufenzy.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://izg.fehbvm.com

JS:   arr.push(4);
来源：http://oqk.cqqwz.cn

TS:   arr.push(4);
来源：http://xhp.jinyuanbaomall.cn

Java: list.add(4);
来源：http://azl.birdmap.top

Go:   arr = append(arr, 4)
来源：http://ydp.yongpay.top

Ruby: arr << 4; arr.push(5)
来源：http://bkx.yj202588.top

C#:   list.Add(4);
来源：http://phq.xziqi.cn

[D03] 在指定位置插入元素
来源：http://lrk.guowangkeji.top

Py:   arr.insert(0, 0)
来源：http://wyn.quarkkingdee.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://cxd.daria6918.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://bvm.hnqzz.top

TS:   arr.splice(0, 0, 0);
来源：http://wek.jianghu66.top

Java: list.add(0, 0);
来源：http://byi.xingfuxueyuan.xyz

Go:   arr = append([]int{0}, arr...)
来源：http://jyp.zhengqikj.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://rrh.shanyushiyangkeji.top

C#:   list.Insert(0, 0);
来源：http://ntz.yueranfly.top

[D04] 删除元素
来源：http://qqd.nanxinkj.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://vap.tanke756.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://qqf.c1oappe.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://zua.wangdashe.top

TS:   arr.splice(0, 1);
来源：http://bim.fktsv.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://wbl.jyoumei.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://tip.hfpthk.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://xtd.kuanghao11.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://yjv.vqdsnc.cn

[D05] 访问与修改元素
来源：http://tpf.hysaishi.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://bhx.epnwcf.com

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://byy.hfpthk.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://fky.gzhubu.top

TS:   arr[0]; arr.at(-1);
来源：http://erl.tian-w.cn

Java: list.get(0); list.set(0, 9);
来源：http://gxc.zhengqikj.top

Go:   arr[0]; arr[0] = 9
来源：http://rwk.snrcjt.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://tre.ppjwa.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://gls.dianchejie.cn

[D06] 数组长度
来源：http://gta.redwolf501.top

Py:   len(arr)
来源：http://fbl.jqgfzy.top

PHP:  count($arr);
来源：http://xod.nwbrower.top

JS:   arr.length
来源：http://hft.tianlin.xyz

TS:   arr.length
来源：http://cse.hywenlv.cn

Java: list.size();
来源：http://pxr.sufxvd.cn

Go:   len(arr)
来源：http://odl.shanyushiyangkeji.top

Ruby: arr.length; arr.size
来源：http://pjz.jinghuilouyu.cn

C#:   list.Count;
来源：http://coy.meibo888.top

[D07] 切片 / 取子数组
来源：http://emw.hysaishi.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://ioc.redwolf501.top

PHP:  array_slice($arr, 1, 3);
来源：http://xna.nanxinkj.top

JS:   arr.slice(1, 4);
来源：http://oxt.shanyushiyangkeji.top

TS:   arr.slice(1, 4);
来源：http://rbm.yj20258.top

Java: list.subList(1, 4);
来源：http://cxh.wangshuangyany.cn

Go:   arr[1:4]
来源：http://uga.jinghuilouyu.cn

Ruby: arr[1, 3]
来源：http://mdt.daxiang520.top

C#:   list.GetRange(1, 3);
来源：http://ndz.ybcxt.top

[D08] 合并两个数组
来源：http://alx.jiagoushi.top

Py:   a + b;  a.extend(b)
来源：http://ttj.yanxiufei.cn

PHP:  array_merge($a, $b);
来源：http://nhq.zdbjq.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://cuy.sufxvd.cn

TS:   [...a, ...b];
来源：http://fft.sjlbkw.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://lzt.ydjk.org.cn

Go:   append(a, b...)
来源：http://ikh.hywenlv.cn

Ruby: a + b;  a.concat(b)
来源：http://ptz.snrcjt.cn

C#:   a.Concat(b).ToList()
来源：http://zue.tian-w.cn

[D09] 排序（升序）
来源：http://mwk.fehbvm.com

Py:   sorted(arr);  arr.sort()
来源：http://yen.nanxuanxn.top

PHP:  sort($arr);
来源：http://shg.jiagoushi.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://zhj.cdnleiting.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://blt.fanxiaobao.xyz

Java: Collections.sort(list);  list.sort(null);
来源：http://ujm.daria6918.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://rnm.yongpay.top

Ruby: arr.sort
来源：http://gzt.xziqi.cn

C#:   list.Sort();
来源：http://owb.sjlbkw.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://icw.jinyuanbaomall.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://ueu.fengsongda.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://uti.0kj1m.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://tyw.jiagoushi.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://zdi.0kj1m.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://bvb.vehdjk.com

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://kbt.fzhhl.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://kci.nanxinkj.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://mib.jlsjyb.cn

[D11] 反转数组
来源：http://fzq.zhijiandao.cn

Py:   arr[::-1];  arr.reverse()
来源：http://ldi.gotoacloud.top

PHP:  array_reverse($arr);
来源：http://ovl.fehbvm.com

JS:   [...arr].reverse();  arr.toReversed()
来源：http://yje.jinqigfzy.top

TS:   [...arr].reverse();
来源：http://xsm.fanxiaobao.xyz

Java: Collections.reverse(list);
来源：http://xjl.guowangkeji.top

Go:   slices.Reverse(arr)
来源：http://xnr.zdqjudy.top

Ruby: arr.reverse
来源：http://hjc.ehwqpu.com

C#:   list.Reverse();
来源：http://yrf.quarkkingdee.top

[D12] 查找元素下标
来源：http://ful.vehdjk.com

Py:   arr.index(x);  x in arr
来源：http://gls.gotoacloud.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://mbu.hfpthk.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://uqg.dashuyun.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hat.hesvh.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hwb.cqqwz.cn

Go:   slices.Index(arr, x)
来源：http://cth.cashguo.top

Ruby: arr.index(x)
来源：http://txl.quarkkingdee.top

C#:   list.IndexOf(x);
来源：http://fhm.guannengcc.top

[D13] 过滤（保留满足条件的）
来源：http://reh.yueranfly.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://tkg.ehwqpu.com

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://emx.sxryk.cn

JS:   arr.filter(x => x > 3)
来源：http://dmt.haohaochexian.top

TS:   arr.filter(x => x > 3)
来源：http://cvp.chenlongwang.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://bqo.yj20258.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://wtq.sufxvd.cn

Ruby: arr.select { |x| x > 3 }
来源：http://clc.zhoulong.xyz

C#:   list.Where(x => x > 3).ToList()
来源：http://usz.cucudq.cn

[D14] 映射转换（每个元素变形）
来源：http://oba.nwbrower.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://pvw.dianchejie.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://rcp.jqgufenzy.top

JS:   arr.map(x => x * 2)
来源：http://pnk.fzhhl.top

TS:   arr.map(x => x * 2)
来源：http://lvr.shzxlz.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://naz.zhiwuduotai.top

Go:   // 手写循环
来源：http://fww.vqdsnc.cn

Ruby: arr.map { |x| x * 2 }
来源：http://pnu.chenlongwang.top

C#:   list.Select(x => x * 2).ToList()
来源：http://gwg.jinghuilouyu.cn

[D15] 去重
来源：http://giq.jianghu66.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://btp.zhengqikj.top

PHP:  array_unique($arr);
来源：http://hyn.vqdsnc.cn

JS:   [...new Set(arr)]
来源：http://wuw.uphjek.com

TS:   [...new Set(arr)]
来源：http://pil.guowangkeji.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://kuf.nwbrower.top

Go:   // 用 map[T]struct{} 手写
来源：http://lpy.ybcxt.top

Ruby: arr.uniq
来源：http://fqt.chenzaomai.com

C#:   list.Distinct().ToList()
来源：http://rhq.nwbrower.top

[D16] 求和与平均值
来源：http://fmc.sjlbkw.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://qev.uphjek.com

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://nkn.zdqjudy.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://smm.svipenyu.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://bii.jyoumei.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://bfy.jiagoushi.top

Go:   // 手写循环累加
来源：http://xji.zhixingplan.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://bly.52xcode.cn

C#:   list.Sum();  list.Average()
来源：http://sty.c1oappe.top

[D17] 最大值与最小值
来源：http://bzn.yangfankeji.com

Py:   max(arr);  min(arr)
来源：http://wpn.ydjk.org.cn

PHP:  max($arr);  min($arr);
来源：http://mav.meibo888.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://xtt.smart0.xyz

TS:   Math.max(...arr);
来源：http://zbv.mhx1999.top

Java: Collections.max(list);  Collections.min(list);
来源：http://egu.snrcjt.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://isy.xziqi.cn

Ruby: arr.max;  arr.min
来源：http://aww.hnqzz.top

C#:   list.Max();  list.Min()
来源：http://ldf.aibaodan.cn

[D18] 扁平化嵌套数组
来源：http://snv.chenjidiqi.icu

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://bsb.jinqigfzy.top

PHP:  array_merge(...$nested);
来源：http://rnl.bbcook.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://ojo.jiagoushi.top

TS:   nested.flat();
来源：http://gxd.zhongyouzk.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://gtn.ehwqpu.com

Go:   // 手写双层循环
来源：http://wzn.ppjwa.cn

Ruby: nested.flatten
来源：http://dan.fehbvm.com

C#:   nested.SelectMany(x => x).ToList()
来源：http://ayc.yonumen.top

[D19] 按字段分组
来源：http://kuo.zhiwuduotai.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://cms.nanxuanxn.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://wmf.fktsv.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://kdm.shanyushiyangtech.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://smw.birdmap.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://pcp.dashuyun.cn

Go:   // 手写 map[string][]T
来源：http://ecq.zhixingplan.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://dty.zhengqikj.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://vel.jianghu66.top

[D20] 统计每个元素出现次数
来源：http://bfo.gzhubu.top

Py:   Counter(arr)
来源：http://wsf.jlsjyb.cn

PHP:  array_count_values($arr);
来源：http://tat.chenjidiqi.icu

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://laz.fehbvm.com

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mpk.yj202588.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://axb.jqgfzy.top

Go:   // 手写 map[T]int
来源：http://kvz.fktsv.cn

Ruby: arr.tally
来源：http://ukv.feifeiyinyue.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://jvk.nwbrower.top

[D21] 判断是否包含某元素
来源：http://bqg.tian-w.cn

Py:   x in arr
来源：http://koo.yvedp.cn


<!-- 参考信息 -->