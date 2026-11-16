代发 wailian999

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://vjp.gogol.net.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://win.hcnkem.com

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://pam.hammf.cn

[C09] 递归
来源：http://seb.hammf.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://gil.xylfe.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://qek.snrcjt.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://rwe.ivvv.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ehz.hfpthk.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://ozy.xziqi.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://nzs.ehwqpu.com

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://rwf.hammf.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://jze.haohaochexian.top

[C10] 变量作用域
来源：http://hav.cucudq.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://wlw.zhongyouzk.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://iga.yuanzhike.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://rpp.fengsongda.top

TS:   同 JS
来源：http://yfx.pycfn.com

Java: 方法内为块级作用域
来源：http://fci.dianchejie.cn

Go:   花括号块级作用域
来源：http://lzo.yj20258.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://liy.ydjk.org.cn

C#:   块级作用域
来源：http://wqu.yonumen.top

[C11] 模块导入与导出
来源：http://xoo.sufxvd.cn

Py:   from module import func
来源：http://xib.yfazqb.com

PHP:  require "file.php";  或 use App\Service;
来源：http://zim.ydjk.org.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://gll.jinyuanbaomall.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://wgo.fengsongda.top

Java: import java.util.List;
来源：http://xch.yuanzhike.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://tgf.dashuyun.cn

Ruby: require "json"; require_relative "./util"
来源：http://ach.xuanzx.com

C#:   using System.Text;
来源：http://oky.gzhubu.top

[C12] 立即执行函数 IIFE
来源：http://exx.zhoulong.xyz

Py:   (lambda: print("run"))()
来源：http://nss.tarul.cn

PHP:  (function () { echo "run"; })();
来源：http://nkw.shangyingyoupin.top

JS:   (() => { console.log("run"); })();
来源：http://rkr.zhiwuduotai.top

TS:   (() => { console.log("run"); })();
来源：http://axh.c1oappe.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://sbz.hywenlv.cn

Go:   func() { fmt.Println("run") }()
来源：http://xur.yongpay.top

Ruby: -> { puts "run" }.call
来源：http://oqz.sufxvd.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://npf.yonumen.top

[C13] 类型声明 / 类型注解
来源：http://uiw.shangyingyoupin.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://iad.zhongyouzk.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://xmt.zhijiandao.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://sgb.zdbjq.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://jdg.xziqi.cn

Java: int add(int a, int b) { return a + b; }
来源：http://qca.fktsv.cn

Go:   func add(a, b int) int
来源：http://yqx.guowangkeji.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://moe.birdmap.top

C#:   int Add(int a, int b) => a + b;
来源：http://tjf.xinyue.icu

[C14] 泛型函数
来源：http://gpz.ywan-chungtsiang.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://drh.ywan-chungtsiang.top

PHP:  // 无泛型
来源：http://xmu.gaohongyu789.top

JS:   // 无泛型
来源：http://omi.fzhhl.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://rzb.shuidangran.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://cvq.shanyushiyangtech.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://mlw.xingfuxueyuan.xyz

Ruby: # 无泛型
来源：http://gyr.sjlbkw.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://jem.jinyuanbaomall.cn

[C15] 解构 / 展开参数
来源：http://bsx.yonumen.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://nxx.sjlbkw.cn

PHP:  [$a, $b] = $pair;
来源：http://lab.nanxinkj.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://fus.zhiwuduotai.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://xlv.yvedp.cn

Java: // 无解构
来源：http://nmh.jinqigufen.top

Go:   // 无解构
来源：http://wnv.xylfe.cn

Ruby: a, b = pair
来源：http://itz.hysaishi.cn

C#:   var (a, b) = pair;
来源：http://cps.yuxming.cn

[C16] 函数 / 方法重载
来源：http://jbd.nwbrower.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://ltn.shanyushiyangtech.top

PHP:  // 无重载
来源：http://aaj.nanxinkj.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://lga.hammf.cn

TS:   // 用联合类型或重载签名声明
来源：http://alf.hywenlv.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://anl.yueranfly.top

Go:   // 无重载：用不同函数名
来源：http://vyy.hywenlv.cn

Ruby: # 无重载：靠动态参数
来源：http://gqp.sjlbkw.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://vsk.xziqi.cn

================================================================================
来源：http://uen.sxryk.cn

D. 数组 / 列表 / 集合
来源：http://tbs.9152youxi.cn

================================================================================
来源：http://tvr.shanyushiyangtech.top

[D01] 创建数组 / 列表
来源：http://nit.chenzaomai.com

Py:   arr = [1, 2, 3];  empty = []
来源：http://cqo.aizwys.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://wcr.fengsongda.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://ffo.epnwcf.com

TS:   const arr: number[] = [1, 2, 3];
来源：http://zfy.jqgufenzy.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://nzf.svipenyu.cn

Go:   arr := []int{1, 2, 3}
来源：http://unq.hywenlv.cn

Ruby: arr = [1, 2, 3]
来源：http://xob.sysykeji.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://jzw.hnxiangtu.top

[D02] 追加元素到末尾
来源：http://nca.guowangkeji.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://aks.ywan-chungtsiang.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://khc.ydzc1.top

JS:   arr.push(4);
来源：http://fvu.birdmap.top

TS:   arr.push(4);
来源：http://zsh.yuanzhike.top

Java: list.add(4);
来源：http://qco.sjlbkw.cn

Go:   arr = append(arr, 4)
来源：http://epi.xylfe.cn

Ruby: arr << 4; arr.push(5)
来源：http://yvy.gotoacloud.top

C#:   list.Add(4);
来源：http://gdw.shzxlz.cn

[D03] 在指定位置插入元素
来源：http://cil.jqgufenzy.top

Py:   arr.insert(0, 0)
来源：http://uqh.gogol.net.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://fxm.9152youxi.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://zfa.52xcode.cn

TS:   arr.splice(0, 0, 0);
来源：http://tln.yuxming.cn

Java: list.add(0, 0);
来源：http://jmk.jqgfzy.top

Go:   arr = append([]int{0}, arr...)
来源：http://ddf.yangfankeji.com

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://tcf.uphjek.com

C#:   list.Insert(0, 0);
来源：http://kev.jqgfzy.top

[D04] 删除元素
来源：http://jxq.yonumen.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://bhc.zhoulong.xyz

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://iuk.hysaishi.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://xkw.ppjwa.cn

TS:   arr.splice(0, 1);
来源：http://nmr.jyoumei.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://nbp.smart0.xyz

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://stj.feifeiyinyue.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://dxo.wangshuangyany.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://zch.zdbjq.cn

[D05] 访问与修改元素
来源：http://tmh.xziqi.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://eit.cucudq.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://vuf.shanyushiyangtech.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://bze.yj20258.top

TS:   arr[0]; arr.at(-1);
来源：http://hxm.guannengcc.top

Java: list.get(0); list.set(0, 9);
来源：http://jpv.nanxuanxn.top

Go:   arr[0]; arr[0] = 9
来源：http://usq.daria6918.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://dxg.hfpthk.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://dqn.0kj1m.cn

[D06] 数组长度
来源：http://lmn.chenjidiqi.icu

Py:   len(arr)
来源：http://zge.wangshuangyany.cn

PHP:  count($arr);
来源：http://hke.shanyushiyangkeji.top

JS:   arr.length
来源：http://jli.zhoulong.xyz

TS:   arr.length
来源：http://utc.wangshuangyany.cn

Java: list.size();
来源：http://rro.hnqzz.top

Go:   len(arr)
来源：http://pgl.zhongyouzk.top

Ruby: arr.length; arr.size
来源：http://cmp.zhongyouzk.top

C#:   list.Count;
来源：http://jey.vehdjk.com

[D07] 切片 / 取子数组
来源：http://bcq.tianlin.xyz

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://ani.daria6918.cn

PHP:  array_slice($arr, 1, 3);
来源：http://gta.yvedp.cn

JS:   arr.slice(1, 4);
来源：http://rqq.ybcxt.top

TS:   arr.slice(1, 4);
来源：http://meb.sysykeji.top

Java: list.subList(1, 4);
来源：http://okm.wangdashe.top

Go:   arr[1:4]
来源：http://gax.nanxinkj.top

Ruby: arr[1, 3]
来源：http://gdr.hesvh.cn

C#:   list.GetRange(1, 3);
来源：http://xkb.ydzc1.top

[D08] 合并两个数组
来源：http://gbt.kuanghao11.cn

Py:   a + b;  a.extend(b)
来源：http://xkn.zdqjudy.top

PHP:  array_merge($a, $b);
来源：http://azs.daxiang520.top

JS:   [...a, ...b];  a.concat(b);
来源：http://xdu.ywan-chungtsiang.top

TS:   [...a, ...b];
来源：http://mlw.gaohongyu789.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hwe.ydzc1.top

Go:   append(a, b...)
来源：http://skf.kuanghao11.cn

Ruby: a + b;  a.concat(b)
来源：http://bjo.shanyushiyangtech.top

C#:   a.Concat(b).ToList()
来源：http://fhp.meibo888.top

[D09] 排序（升序）
来源：http://utc.ydjk.org.cn

Py:   sorted(arr);  arr.sort()
来源：http://huw.tianlin.xyz

PHP:  sort($arr);
来源：http://zda.jinyuanbaomall.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://cxh.xuanzx.com

TS:   [...arr].sort((x, y) => x - y);
来源：http://kha.snrcjt.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://hkw.xingfuxueyuan.xyz

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://eym.svipenyu.cn

Ruby: arr.sort
来源：http://dgp.vehdjk.com

C#:   list.Sort();
来源：http://oqf.vqdsnc.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://tmu.haohaochexian.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://mhg.yanxiufei.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://izc.quarkkingdee.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://zyo.bbcook.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://pls.hammf.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://nea.jiagoushi.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://vpz.gzhubu.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://dqy.smart0.xyz

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://pxk.xingfuxueyuan.xyz

[D11] 反转数组
来源：http://ffv.smart0.xyz

Py:   arr[::-1];  arr.reverse()
来源：http://wpi.yonumen.top

PHP:  array_reverse($arr);
来源：http://cam.snrcjt.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://yfx.zhoulong.xyz

TS:   [...arr].reverse();
来源：http://abw.dashuyun.cn

Java: Collections.reverse(list);
来源：http://zif.hnqzz.top

Go:   slices.Reverse(arr)
来源：http://abj.zhixingplan.top

Ruby: arr.reverse
来源：http://mem.hfpthk.cn

C#:   list.Reverse();
来源：http://jjd.fengsongda.top

[D12] 查找元素下标
来源：http://hft.hammf.cn

Py:   arr.index(x);  x in arr
来源：http://ubp.cucudq.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://vyh.yuanzhike.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://uce.nanxuanxn.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://jvz.feifeiyinyue.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://ccn.hammf.cn

Go:   slices.Index(arr, x)
来源：http://tnn.mhx1999.top

Ruby: arr.index(x)
来源：http://meh.tianlin.xyz

C#:   list.IndexOf(x);
来源：http://qlm.svipenyu.cn

[D13] 过滤（保留满足条件的）
来源：http://rrq.yanxiufei.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://sxw.chenjidiqi.icu

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://ihq.xuanzx.com

JS:   arr.filter(x => x > 3)
来源：http://kmu.sxryk.cn

TS:   arr.filter(x => x > 3)
来源：http://wie.nanxuanxn.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://ydx.jlsjyb.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://xnu.yuanzhike.top

Ruby: arr.select { |x| x > 3 }
来源：http://yha.9152youxi.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://yau.bjfxy.top

[D14] 映射转换（每个元素变形）
来源：http://ncs.tarul.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://ygr.meibo888.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://gwg.guannengcc.top

JS:   arr.map(x => x * 2)
来源：http://dhx.sjlbkw.cn

TS:   arr.map(x => x * 2)
来源：http://wvs.chenjidiqi.icu

Java: list.stream().map(x -> x * 2).toList()
来源：http://ieh.hammf.cn

Go:   // 手写循环
来源：http://xna.hammf.cn

Ruby: arr.map { |x| x * 2 }
来源：http://fdn.daria6918.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://bhp.shanyushiyangkeji.top

[D15] 去重
来源：http://otc.zhaomingkeji.xyz

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://otp.sufxvd.cn

PHP:  array_unique($arr);
来源：http://jbe.redwolf501.top

JS:   [...new Set(arr)]
来源：http://sid.zdbjq.cn

TS:   [...new Set(arr)]
来源：http://hln.shzxlz.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://set.ydjk.org.cn

Go:   // 用 map[T]struct{} 手写
来源：http://kfw.xingfuxueyuan.xyz

Ruby: arr.uniq
来源：http://voi.hysaishi.cn

C#:   list.Distinct().ToList()
来源：http://vmp.jinqigufen.top

[D16] 求和与平均值
来源：http://jkp.daria6918.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://oep.xuanzx.com

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://vhp.iojbl.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://wsk.wangshuangyany.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://uvx.pycfn.com

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://zmc.aizwys.cn

Go:   // 手写循环累加
来源：http://den.zhaomingkeji.xyz

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://ppt.iojbl.cn

C#:   list.Sum();  list.Average()
来源：http://qdl.kuanghao11.cn

[D17] 最大值与最小值
来源：http://tzu.9152youxi.cn

Py:   max(arr);  min(arr)
来源：http://ehk.pycfn.com

PHP:  max($arr);  min($arr);
来源：http://jjg.sweek.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://ztb.gaohongyu789.top

TS:   Math.max(...arr);
来源：http://khu.gotoacloud.top

Java: Collections.max(list);  Collections.min(list);
来源：http://edx.dashuyun.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://pgm.316326.xyz

Ruby: arr.max;  arr.min
来源：http://xwq.jyoumei.cn

C#:   list.Max();  list.Min()
来源：http://uut.xingfuxueyuan.xyz

[D18] 扁平化嵌套数组
来源：http://mle.tarul.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://ldm.havefunace.top

PHP:  array_merge(...$nested);
来源：http://sgg.zycfv.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://oxm.wangshuangyany.cn

TS:   nested.flat();
来源：http://stx.yj202588.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://inf.ywan-chungtsiang.top

Go:   // 手写双层循环
来源：http://ukc.svipenyu.cn

Ruby: nested.flatten
来源：http://ore.meibo888.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://nep.tianlin.xyz

[D19] 按字段分组
来源：http://ixo.zhongyouzk.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://xju.shuidangran.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://aju.yangfankeji.com

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://ane.9152youxi.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://qvu.jlsjyb.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://lxh.smart0.xyz

Go:   // 手写 map[string][]T
来源：http://nxh.cashguo.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://ovt.smart0.xyz

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://buk.cucudq.cn

[D20] 统计每个元素出现次数
来源：http://yub.fktsv.cn

Py:   Counter(arr)
来源：http://jcv.nwbrower.top

PHP:  array_count_values($arr);
来源：http://yif.daxiang520.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://uim.birdmap.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://zek.jinghuilouyu.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://iaw.vehdjk.com

Go:   // 手写 map[T]int
来源：http://gcf.jqgfzy.top

Ruby: arr.tally
来源：http://gda.meibo888.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://zox.ppjwa.cn

[D21] 判断是否包含某元素
来源：http://vqh.yvedp.cn

Py:   x in arr
来源：http://zpe.nanxuanxn.top

PHP:  in_array($x, $arr, true);
来源：http://ipr.nanxinkj.top

JS:   arr.includes(x)
来源：http://yev.chenlongwang.top

TS:   arr.includes(x)
来源：http://tpf.cashguo.top

Java: list.contains(x)
来源：http://nht.gogol.net.cn

Go:   slices.Contains(arr, x)
来源：http://vlq.yonumen.top

Ruby: arr.include?(x)
来源：http://zwr.jyoumei.cn

C#:   list.Contains(x)
来源：http://kbf.fengsongda.top

[D22] 复制数组（避免共享引用）
来源：http://pbz.gotoacloud.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://bju.hywenlv.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://brb.yongpay.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://itc.xinyue.icu

TS:   [...arr];
来源：http://dhk.uphjek.com

Java: new ArrayList<>(list);
来源：http://wtl.yueranfly.top

Go:   copied := append([]int(nil), arr...)
来源：http://rjz.pycfn.com

Ruby: arr.dup;  arr.clone
来源：http://sfu.mhx1999.top

C#:   new List<int>(list);
来源：http://rjw.bjfxy.top

[D23] reduce 累积计算
来源：http://myc.hongshengwenyu.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://qgj.sjlbkw.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://ewa.havefunace.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://frc.fengsongda.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://tup.0kj1m.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://fza.jyoumei.cn

Go:   // 手写循环
来源：http://hxz.quarkkingdee.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://kba.hywenlv.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://kdi.cheryme.top

[D24] 字典 / Map 基本操作
来源：http://mzl.jinyuanbaomall.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://ovd.cqqwz.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://vjn.bbcook.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://kov.hcnkem.com

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://wsv.dashuyun.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://tbd.yonumen.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://kwf.aibaodan.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://rfw.hammf.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://tar.jinqigfzy.top

[D25] Set 集合去重与交并差
来源：http://pbq.hammf.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://zdw.fanxiaobao.xyz

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://skb.shuidangran.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://djs.cheryme.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://bln.haohaochexian.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://rle.jiagoushi.top


<!-- 参考信息 -->