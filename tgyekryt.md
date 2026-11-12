代发 wailian999

Go:   // 无：用配置结构体参数
来源：http://ojm.shzxlz.cn

Ruby: f(a: 1, b: 2)
来源：http://nnl.zhixingplan.top

C#:   f(a: 1, b: 2)
来源：http://qtv.cheryme.top

[C05] 返回多个值
来源：http://nmq.wangshuangyany.cn

Py:   return a, b
来源：http://jxd.zhiwuduotai.top

PHP:  return [$a, $b];
来源：http://jkd.quarkkingdee.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://huk.jlsjyb.cn

TS:   return { a, b };
来源：http://kmi.yuxming.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://zdp.hongshengwenyu.top

Go:   return a, b
来源：http://obg.sjlbkw.cn

Ruby: return a, b
来源：http://wsa.gogol.net.cn

C#:   return (a, b);              // ValueTuple
来源：http://ovx.ywan-chungtsiang.top

[C06] 匿名函数 / lambda
来源：http://kin.jinqigfzy.top

Py:   square = lambda x: x * x
来源：http://emc.9152youxi.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://exv.shanyushiyangtech.top

JS:   const square = x => x * x;
来源：http://sny.fengsongda.top

TS:   const square = (x: number): number => x * x;
来源：http://yob.hywenlv.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://rsq.yangfankeji.com

Go:   sq := func(x int) int { return x * x }
来源：http://pey.yj20258.top

Ruby: square = ->(x) { x * x }
来源：http://uny.vehdjk.com

C#:   Func<int, int> square = x => x * x;
来源：http://esz.pengpengdd.cyou

[C07] 把函数作为参数传入
来源：http://roy.cqqwz.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://ryq.hnqzz.top

PHP:  array_map("strtoupper", $arr);
来源：http://tuz.shanyushiyangkeji.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://oqf.aizwys.cn

TS:   arr.map(String)
来源：http://egs.sjlbkw.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://khk.haohaochexian.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://ity.hfpthk.cn

Ruby: arr.map(&:upcase)
来源：http://kdl.yfazqb.com

C#:   arr.Select(s => s.ToUpper())
来源：http://nlu.dianchejie.cn

[C08] 闭包
来源：http://juu.52xcode.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://mzv.jianghu66.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://xec.pycfn.com

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://cvz.zhongyouzk.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://rjw.aibaodan.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://omp.nanxuanxn.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://euv.shanyushiyangkeji.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://pfb.hesvh.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://whu.xinyue.icu

[C09] 递归
来源：http://bww.hysaishi.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://qvp.hnxiangtu.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://yab.chenjidiqi.icu

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://dks.zdbjq.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ahj.yuanzhike.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://xjy.zdbjq.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://ekr.ivvv.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://taf.fanxiaobao.xyz

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://gjh.aizwys.cn

[C10] 变量作用域
来源：http://pww.feifeiyinyue.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://gpf.zhoulong.xyz

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://zxk.jinqigfzy.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://sdr.yanxiufei.cn

TS:   同 JS
来源：http://hkn.sjlbkw.cn

Java: 方法内为块级作用域
来源：http://jdb.shanyushiyangtech.top

Go:   花括号块级作用域
来源：http://mzk.bbcook.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://zfd.meibo888.top

C#:   块级作用域
来源：http://eeo.cdnleiting.top

[C11] 模块导入与导出
来源：http://qfw.sysykeji.top

Py:   from module import func
来源：http://wne.zycfv.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://ohk.vqdsnc.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://sfg.haohaochexian.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://eie.yueranfly.top

Java: import java.util.List;
来源：http://hhd.zhoulong.xyz

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://txp.yj20258.top

Ruby: require "json"; require_relative "./util"
来源：http://dpy.cheryme.top

C#:   using System.Text;
来源：http://bxb.xinyue.icu

[C12] 立即执行函数 IIFE
来源：http://mzc.gogol.net.cn

Py:   (lambda: print("run"))()
来源：http://ics.yuxming.cn

PHP:  (function () { echo "run"; })();
来源：http://xxq.kuanghao11.cn

JS:   (() => { console.log("run"); })();
来源：http://wuj.havefunace.top

TS:   (() => { console.log("run"); })();
来源：http://oxi.iojbl.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://mjs.yongpay.top

Go:   func() { fmt.Println("run") }()
来源：http://gmm.chenzaomai.com

Ruby: -> { puts "run" }.call
来源：http://nzq.hesvh.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://sbi.ywan-chungtsiang.top

[C13] 类型声明 / 类型注解
来源：http://oks.hnxiangtu.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://jxe.jinyuanbaomall.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://zut.shzxlz.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://htl.ydzc1.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ibv.zhixingplan.top

Java: int add(int a, int b) { return a + b; }
来源：http://ala.hesvh.cn

Go:   func add(a, b int) int
来源：http://zcx.guannengcc.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://lyh.sjlbkw.cn

C#:   int Add(int a, int b) => a + b;
来源：http://pot.jlsjyb.cn

[C14] 泛型函数
来源：http://wxg.xylfe.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://bmx.yongpay.top

PHP:  // 无泛型
来源：http://vzy.hesvh.cn

JS:   // 无泛型
来源：http://egv.fzhhl.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://fcg.wangdashe.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://dzd.xylfe.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://iap.cqqwz.cn

Ruby: # 无泛型
来源：http://kot.yvedp.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://gmz.svipenyu.cn

[C15] 解构 / 展开参数
来源：http://rcg.sjlbkw.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://nub.xuetiantiany.cn

PHP:  [$a, $b] = $pair;
来源：http://kvz.tarul.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://fpf.jinghuilouyu.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://lub.haohaochexian.top

Java: // 无解构
来源：http://bux.sweek.top

Go:   // 无解构
来源：http://zll.hcnkem.com

Ruby: a, b = pair
来源：http://slg.sysykeji.top

C#:   var (a, b) = pair;
来源：http://pwt.hnxiangtu.top

[C16] 函数 / 方法重载
来源：http://reu.fehbvm.com

Py:   # 无重载：用默认参数或 *args 变通
来源：http://wrw.hesvh.cn

PHP:  // 无重载
来源：http://fuv.pycfn.com

JS:   // 无重载：靠 arguments.length 分支
来源：http://ydw.nanxuanxn.top

TS:   // 用联合类型或重载签名声明
来源：http://vkr.shanyushiyangtech.top

Java: void f(int a) {}  void f(String a) {}
来源：http://qvo.gogol.net.cn

Go:   // 无重载：用不同函数名
来源：http://euq.ydzc1.top

Ruby: # 无重载：靠动态参数
来源：http://qik.jinqigfzy.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://fop.ydzc1.top

================================================================================
来源：http://klj.andypj.xyz

D. 数组 / 列表 / 集合
来源：http://hlz.bbcook.cn

================================================================================
来源：http://hge.ehwqpu.com

[D01] 创建数组 / 列表
来源：http://nwn.snrcjt.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://kkq.yfazqb.com

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://cvl.yj202588.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://tld.cqqwz.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://qmu.xinyue.icu

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://nft.jinqigufen.top

Go:   arr := []int{1, 2, 3}
来源：http://ldq.yfazqb.com

Ruby: arr = [1, 2, 3]
来源：http://viu.aizwys.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://uja.gaohongyu789.top

[D02] 追加元素到末尾
来源：http://wor.zhaomingkeji.xyz

Py:   arr.append(4); arr.extend([5, 6])
来源：http://tae.sufxvd.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://xxb.jqgfzy.top

JS:   arr.push(4);
来源：http://gco.jlsjyb.cn

TS:   arr.push(4);
来源：http://alo.hysaishi.cn

Java: list.add(4);
来源：http://yis.yanxiufei.cn

Go:   arr = append(arr, 4)
来源：http://szu.chenjidiqi.icu

Ruby: arr << 4; arr.push(5)
来源：http://aqz.pengpengdd.cyou

C#:   list.Add(4);
来源：http://ujh.nanxinkj.top

[D03] 在指定位置插入元素
来源：http://sir.zdqjudy.top

Py:   arr.insert(0, 0)
来源：http://yqx.jinghuilouyu.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://qhv.52xcode.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://dxw.c1oappe.top

TS:   arr.splice(0, 0, 0);
来源：http://hoo.yj20258.top

Java: list.add(0, 0);
来源：http://kjd.yonumen.top

Go:   arr = append([]int{0}, arr...)
来源：http://slj.fengsongda.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://bsq.yonumen.top

C#:   list.Insert(0, 0);
来源：http://xpi.daria6918.cn

[D04] 删除元素
来源：http://klf.cashguo.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://blp.chenzaomai.com

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://rje.yongpay.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://rhy.shanyushiyangkeji.top

TS:   arr.splice(0, 1);
来源：http://rst.jinghuilouyu.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://fht.svipenyu.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://bgv.zhaomingkeji.xyz

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://czk.jiagoushi.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://tkb.ppjwa.cn

[D05] 访问与修改元素
来源：http://wbp.dianchejie.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://jpc.tian-w.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://usx.jinghuilouyu.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://cxa.nanxuanxn.top

TS:   arr[0]; arr.at(-1);
来源：http://asm.iojbl.cn

Java: list.get(0); list.set(0, 9);
来源：http://ndv.sufxvd.cn

Go:   arr[0]; arr[0] = 9
来源：http://mob.wangshuangyany.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://thj.cashguo.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://aap.svipenyu.cn

[D06] 数组长度
来源：http://nea.daxiang520.top

Py:   len(arr)
来源：http://yts.yj20258.top

PHP:  count($arr);
来源：http://erj.xziqi.cn

JS:   arr.length
来源：http://zwn.shanyushiyangkeji.top

TS:   arr.length
来源：http://dnb.ivvv.top

Java: list.size();
来源：http://van.xziqi.cn

Go:   len(arr)
来源：http://som.zhoulong.xyz

Ruby: arr.length; arr.size
来源：http://sdy.gogol.net.cn

C#:   list.Count;
来源：http://gkm.ydjk.org.cn

[D07] 切片 / 取子数组
来源：http://uev.xinyue.icu

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://tde.jqgufenzy.top

PHP:  array_slice($arr, 1, 3);
来源：http://nsb.zhijiandao.cn

JS:   arr.slice(1, 4);
来源：http://aeo.cqqwz.cn

TS:   arr.slice(1, 4);
来源：http://hpx.9152youxi.cn

Java: list.subList(1, 4);
来源：http://gwi.tian-w.cn

Go:   arr[1:4]
来源：http://toh.guowangkeji.top

Ruby: arr[1, 3]
来源：http://szn.jianghu66.top

C#:   list.GetRange(1, 3);
来源：http://dco.zhijiandao.cn

[D08] 合并两个数组
来源：http://znx.zhengqikj.top

Py:   a + b;  a.extend(b)
来源：http://tpb.meibo888.top

PHP:  array_merge($a, $b);
来源：http://qbi.uphjek.com

JS:   [...a, ...b];  a.concat(b);
来源：http://bpn.havefunace.top

TS:   [...a, ...b];
来源：http://qlr.jiagoushi.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://elz.smart0.xyz

Go:   append(a, b...)
来源：http://agn.zhiwuduotai.top

Ruby: a + b;  a.concat(b)
来源：http://mce.quarkkingdee.top

C#:   a.Concat(b).ToList()
来源：http://tng.jqgufenzy.top

[D09] 排序（升序）
来源：http://kdu.9152youxi.cn

Py:   sorted(arr);  arr.sort()
来源：http://jgc.yj202588.top

PHP:  sort($arr);
来源：http://zct.shangyingyoupin.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://siq.ydjk.org.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://ofv.yfazqb.com

Java: Collections.sort(list);  list.sort(null);
来源：http://bnx.hfpthk.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://cmu.snrcjt.cn

Ruby: arr.sort
来源：http://iqw.hammf.cn

C#:   list.Sort();
来源：http://nzy.fehbvm.com

[D10] 自定义排序（按字段 / 多条件）
来源：http://sjp.zhoulong.xyz

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://nfz.jianghu66.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://bst.52xcode.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://exc.guannengcc.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://rax.zhiwuduotai.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://qsd.zdqjudy.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://sbu.sufxvd.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://pre.sjlbkw.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://qbk.hnqzz.top

[D11] 反转数组
来源：http://yzy.jinghuilouyu.cn

Py:   arr[::-1];  arr.reverse()
来源：http://woz.birdmap.top

PHP:  array_reverse($arr);
来源：http://mrq.jinghuilouyu.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://bza.hcnkem.com

TS:   [...arr].reverse();
来源：http://ajk.xuetiantiany.cn

Java: Collections.reverse(list);
来源：http://zam.daxiang520.top

Go:   slices.Reverse(arr)
来源：http://ujr.nanxinkj.top

Ruby: arr.reverse
来源：http://vql.fzhhl.top

C#:   list.Reverse();
来源：http://kzz.aizwys.cn

[D12] 查找元素下标
来源：http://pug.yanxiufei.cn

Py:   arr.index(x);  x in arr
来源：http://jkf.meibo888.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://cay.jinqigfzy.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://sfs.cucudq.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://djo.shangyingyoupin.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://kuk.cashguo.top

Go:   slices.Index(arr, x)
来源：http://zvl.svipenyu.cn

Ruby: arr.index(x)
来源：http://hxl.fzhhl.top

C#:   list.IndexOf(x);
来源：http://zcj.smart0.xyz

[D13] 过滤（保留满足条件的）
来源：http://ipt.yangfankeji.com

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://rgd.yuanzhike.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hpd.hongshengwenyu.top

JS:   arr.filter(x => x > 3)
来源：http://rtl.yvedp.cn

TS:   arr.filter(x => x > 3)
来源：http://gba.ydzc1.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://bna.hnxiangtu.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://dan.yvedp.cn

Ruby: arr.select { |x| x > 3 }
来源：http://vzs.pycfn.com

C#:   list.Where(x => x > 3).ToList()
来源：http://rzs.daxiang520.top

[D14] 映射转换（每个元素变形）
来源：http://lpo.zhaomingkeji.xyz

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://fwe.andypj.xyz

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://lht.dashuyun.cn

JS:   arr.map(x => x * 2)
来源：http://pql.9152youxi.cn

TS:   arr.map(x => x * 2)
来源：http://cyd.shzxlz.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://xcr.snrcjt.cn

Go:   // 手写循环
来源：http://sng.c1oappe.top

Ruby: arr.map { |x| x * 2 }
来源：http://bul.chenzaomai.com

C#:   list.Select(x => x * 2).ToList()
来源：http://exm.sjlbkw.cn

[D15] 去重
来源：http://jgs.9152youxi.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://vof.feifeiyinyue.top

PHP:  array_unique($arr);
来源：http://xhd.9152youxi.cn

JS:   [...new Set(arr)]
来源：http://loq.hysaishi.cn

TS:   [...new Set(arr)]
来源：http://ryt.cqqwz.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://lzk.sysykeji.top

Go:   // 用 map[T]struct{} 手写
来源：http://gmj.guowangkeji.top

Ruby: arr.uniq
来源：http://eyz.yongpay.top

C#:   list.Distinct().ToList()
来源：http://upp.0kj1m.cn

[D16] 求和与平均值
来源：http://sas.xingfuxueyuan.xyz

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://ptg.hnxiangtu.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://cqu.fanxiaobao.xyz

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://oxh.bbcook.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://ixt.yj20258.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://mjg.zhiwuduotai.top

Go:   // 手写循环累加
来源：http://enp.yj20258888.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://ayn.nanxinkj.top

C#:   list.Sum();  list.Average()
来源：http://gkg.yongpay.top

[D17] 最大值与最小值
来源：http://ezm.zhijiandao.cn

Py:   max(arr);  min(arr)
来源：http://dne.zycfv.cn

PHP:  max($arr);  min($arr);
来源：http://evr.fktsv.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://jzd.jlsjyb.cn

TS:   Math.max(...arr);
来源：http://tjw.svipenyu.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://owr.dashuyun.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://zew.hfpthk.cn

Ruby: arr.max;  arr.min
来源：http://wqj.jyoumei.cn

C#:   list.Max();  list.Min()
来源：http://fyp.zycfv.cn

[D18] 扁平化嵌套数组
来源：http://zbw.meibo888.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://wvf.xuanzx.com

PHP:  array_merge(...$nested);
来源：http://gpt.shanyushiyangtech.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://wnl.yuanzhike.top

TS:   nested.flat();
来源：http://csx.yueranfly.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://mkp.jinqigfzy.top

Go:   // 手写双层循环
来源：http://xjv.quarkkingdee.top

Ruby: nested.flatten
来源：http://qat.shangyingyoupin.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://six.hammf.cn

[D19] 按字段分组
来源：http://pmj.dashuyun.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://pgh.hcnkem.com

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://npk.sysykeji.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://gfr.tian-w.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://vcp.hywenlv.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://cfy.nanxuanxn.top

Go:   // 手写 map[string][]T
来源：http://apc.cheryme.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://jms.xuetiantiany.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://riy.tanke756.top

[D20] 统计每个元素出现次数
来源：http://gmb.cheryme.top

Py:   Counter(arr)
来源：http://dxs.hesvh.cn

PHP:  array_count_values($arr);
来源：http://egk.fanxiaobao.xyz

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://tpx.aibaodan.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://fzj.sweek.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://ngf.9152youxi.cn

Go:   // 手写 map[T]int
来源：http://uap.quarkkingdee.top

Ruby: arr.tally
来源：http://nsz.xuetiantiany.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://tih.guowangkeji.top

[D21] 判断是否包含某元素
来源：http://vjz.zycfv.cn

Py:   x in arr
来源：http://gkd.aizwys.cn

PHP:  in_array($x, $arr, true);
来源：http://tdn.yongpay.top

JS:   arr.includes(x)
来源：http://kcn.zhixingplan.top

TS:   arr.includes(x)
来源：http://nwa.hnqzz.top

Java: list.contains(x)
来源：http://vgl.yuxming.cn


<!-- 参考信息 -->