代发 wailian999

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://wbt.zhiwuduotai.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://vny.jinqigufen.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://xws.epnwcf.com

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://oli.yuanzhike.top

[C10] 变量作用域
来源：http://eav.zdbjq.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://cfs.tianlin.xyz

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://fvc.gaohongyu789.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://fbe.guowangkeji.top

TS:   同 JS
来源：http://zaw.yongpay.top

Java: 方法内为块级作用域
来源：http://llz.vqdsnc.cn

Go:   花括号块级作用域
来源：http://usp.sjlbkw.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://nvl.fehbvm.com

C#:   块级作用域
来源：http://jcy.hywenlv.cn

[C11] 模块导入与导出
来源：http://sij.jinghuilouyu.cn

Py:   from module import func
来源：http://jon.fengsongda.top

PHP:  require "file.php";  或 use App\Service;
来源：http://ptd.zycfv.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://hju.yanxiufei.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://qec.hammf.cn

Java: import java.util.List;
来源：http://jfx.yj202588.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://acd.redwolf501.top

Ruby: require "json"; require_relative "./util"
来源：http://mqm.zhaomingkeji.xyz

C#:   using System.Text;
来源：http://vba.tianlin.xyz

[C12] 立即执行函数 IIFE
来源：http://xxu.birdmap.top

Py:   (lambda: print("run"))()
来源：http://dof.xuanzx.com

PHP:  (function () { echo "run"; })();
来源：http://ivm.ydjk.org.cn

JS:   (() => { console.log("run"); })();
来源：http://ivd.shuidangran.top

TS:   (() => { console.log("run"); })();
来源：http://lue.yj202588.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://zhz.zhoulong.xyz

Go:   func() { fmt.Println("run") }()
来源：http://okj.shanyushiyangtech.top

Ruby: -> { puts "run" }.call
来源：http://gpq.bbcook.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://yrx.fehbvm.com

[C13] 类型声明 / 类型注解
来源：http://cfq.zdbjq.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hwq.ctjpmb.com

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ycq.xylfe.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://smb.kuanghao11.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://qrs.wangshuangyany.cn

Java: int add(int a, int b) { return a + b; }
来源：http://ubm.yj20258888.top

Go:   func add(a, b int) int
来源：http://fke.zhongyouzk.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://uaj.smart0.xyz

C#:   int Add(int a, int b) => a + b;
来源：http://muk.tanke756.top

[C14] 泛型函数
来源：http://kgn.svipenyu.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://dli.ydjk.org.cn

PHP:  // 无泛型
来源：http://fqw.tianlin.xyz

JS:   // 无泛型
来源：http://cwh.jiagoushi.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://bsz.uphjek.com

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://fmb.gotoacloud.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://ngv.hnqzz.top

Ruby: # 无泛型
来源：http://xqu.zdbjq.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://zda.gaohongyu789.top

[C15] 解构 / 展开参数
来源：http://med.jinghuilouyu.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://wby.feifeiyinyue.top

PHP:  [$a, $b] = $pair;
来源：http://pjk.hongshengwenyu.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hgi.vqdsnc.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://qfb.zhixingplan.top

Java: // 无解构
来源：http://fsa.bbcook.cn

Go:   // 无解构
来源：http://ddl.yanxiufei.cn

Ruby: a, b = pair
来源：http://rvd.havefunace.top

C#:   var (a, b) = pair;
来源：http://ias.hywenlv.cn

[C16] 函数 / 方法重载
来源：http://ykb.hysaishi.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://oqf.tian-w.cn

PHP:  // 无重载
来源：http://nat.gogol.net.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://luy.hfpthk.cn

TS:   // 用联合类型或重载签名声明
来源：http://stp.vqdsnc.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://zvu.hysaishi.cn

Go:   // 无重载：用不同函数名
来源：http://koj.316326.xyz

Ruby: # 无重载：靠动态参数
来源：http://dnx.dashuyun.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://mog.ctjpmb.com

================================================================================
来源：http://fwo.daxiang520.top

D. 数组 / 列表 / 集合
来源：http://veg.ybcxt.top

================================================================================
来源：http://xka.birdmap.top

[D01] 创建数组 / 列表
来源：http://brx.kuanghao11.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://xwl.yj20258.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://csk.cucudq.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://egm.birdmap.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://ajr.jlsjyb.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://erg.meibo888.top

Go:   arr := []int{1, 2, 3}
来源：http://sdn.dianchejie.cn

Ruby: arr = [1, 2, 3]
来源：http://zih.snrcjt.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://ckk.zhixingplan.top

[D02] 追加元素到末尾
来源：http://dcy.feifeiyinyue.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://crd.haohaochexian.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://knm.bjfxy.top

JS:   arr.push(4);
来源：http://wrq.hfpthk.cn

TS:   arr.push(4);
来源：http://fku.sxryk.cn

Java: list.add(4);
来源：http://gcs.svipenyu.cn

Go:   arr = append(arr, 4)
来源：http://swm.iojbl.cn

Ruby: arr << 4; arr.push(5)
来源：http://jwr.cucudq.cn

C#:   list.Add(4);
来源：http://wgr.ivvv.top

[D03] 在指定位置插入元素
来源：http://usr.hongshengwenyu.top

Py:   arr.insert(0, 0)
来源：http://iwy.sjlbkw.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://lyf.gogol.net.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://rjx.gaohongyu789.top

TS:   arr.splice(0, 0, 0);
来源：http://ief.ppjwa.cn

Java: list.add(0, 0);
来源：http://wlj.ydjk.org.cn

Go:   arr = append([]int{0}, arr...)
来源：http://xnf.ehwqpu.com

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://agy.zhongyouzk.top

C#:   list.Insert(0, 0);
来源：http://vdf.epnwcf.com

[D04] 删除元素
来源：http://ssx.tianlin.xyz

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://vse.xylfe.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://zkw.meibo888.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://sgx.gaohongyu789.top

TS:   arr.splice(0, 1);
来源：http://zde.shanyushiyangtech.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://rld.sxryk.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://ihn.zhaomingkeji.xyz

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://lpy.aizwys.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://uti.ybcxt.top

[D05] 访问与修改元素
来源：http://hep.yangfankeji.com

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://iyr.xuetiantiany.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://yfk.vehdjk.com

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://abt.hysaishi.cn

TS:   arr[0]; arr.at(-1);
来源：http://xbe.hnxiangtu.top

Java: list.get(0); list.set(0, 9);
来源：http://veb.sjlbkw.cn

Go:   arr[0]; arr[0] = 9
来源：http://xqt.xuetiantiany.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://arq.9152youxi.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://zld.xuetiantiany.cn

[D06] 数组长度
来源：http://wzu.bjfxy.top

Py:   len(arr)
来源：http://qch.svipenyu.cn

PHP:  count($arr);
来源：http://jer.ywan-chungtsiang.top

JS:   arr.length
来源：http://fzi.9152youxi.cn

TS:   arr.length
来源：http://lck.zhijiandao.cn

Java: list.size();
来源：http://cve.sxryk.cn

Go:   len(arr)
来源：http://yej.shuidangran.top

Ruby: arr.length; arr.size
来源：http://gae.jinqigfzy.top

C#:   list.Count;
来源：http://ghw.ivvv.top

[D07] 切片 / 取子数组
来源：http://zif.cheryme.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://vwc.52xcode.cn

PHP:  array_slice($arr, 1, 3);
来源：http://jjp.dianchejie.cn

JS:   arr.slice(1, 4);
来源：http://ifk.aizwys.cn

TS:   arr.slice(1, 4);
来源：http://iju.redwolf501.top

Java: list.subList(1, 4);
来源：http://pvl.quarkkingdee.top

Go:   arr[1:4]
来源：http://bal.iojbl.cn

Ruby: arr[1, 3]
来源：http://osb.tarul.cn

C#:   list.GetRange(1, 3);
来源：http://pdl.sweek.top

[D08] 合并两个数组
来源：http://hik.gogol.net.cn

Py:   a + b;  a.extend(b)
来源：http://kle.zhijiandao.cn

PHP:  array_merge($a, $b);
来源：http://uil.daria6918.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://pnp.pengpengdd.cyou

TS:   [...a, ...b];
来源：http://jat.fehbvm.com

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://pqf.chenlongwang.top

Go:   append(a, b...)
来源：http://ido.hcnkem.com

Ruby: a + b;  a.concat(b)
来源：http://whl.shzxlz.cn

C#:   a.Concat(b).ToList()
来源：http://gkt.shzxlz.cn

[D09] 排序（升序）
来源：http://jme.uphjek.com

Py:   sorted(arr);  arr.sort()
来源：http://ydv.hammf.cn

PHP:  sort($arr);
来源：http://bia.vehdjk.com

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://urs.jinqigfzy.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://neg.zhengqikj.top

Java: Collections.sort(list);  list.sort(null);
来源：http://hly.iojbl.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://jiv.sysykeji.top

Ruby: arr.sort
来源：http://iat.iojbl.cn

C#:   list.Sort();
来源：http://wxw.sufxvd.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://mvf.daxiang520.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://gam.tian-w.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://aim.jyoumei.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://zxz.hcnkem.com

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://vnr.yuxming.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://ofl.ivvv.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://eca.yongpay.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://uff.yuanzhike.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://qvq.sjlbkw.cn

[D11] 反转数组
来源：http://vpn.smart0.xyz

Py:   arr[::-1];  arr.reverse()
来源：http://fxe.yanxiufei.cn

PHP:  array_reverse($arr);
来源：http://oui.cucudq.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://toc.xuanzx.com

TS:   [...arr].reverse();
来源：http://fae.zhixingplan.top

Java: Collections.reverse(list);
来源：http://fyz.epnwcf.com

Go:   slices.Reverse(arr)
来源：http://kdl.aizwys.cn

Ruby: arr.reverse
来源：http://dbg.yanxiufei.cn

C#:   list.Reverse();
来源：http://otr.0kj1m.cn

[D12] 查找元素下标
来源：http://omp.chenjidiqi.icu

Py:   arr.index(x);  x in arr
来源：http://kbd.sxryk.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://vbk.zhixingplan.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://zns.gotoacloud.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://tmy.jyoumei.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://zmh.wangdashe.top

Go:   slices.Index(arr, x)
来源：http://rvf.hnxiangtu.top

Ruby: arr.index(x)
来源：http://vjn.yj202588.top

C#:   list.IndexOf(x);
来源：http://gbn.gzhubu.top

[D13] 过滤（保留满足条件的）
来源：http://wqp.yj20258888.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hml.chenjidiqi.icu

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://kbv.cdnleiting.top

JS:   arr.filter(x => x > 3)
来源：http://hfl.52xcode.cn

TS:   arr.filter(x => x > 3)
来源：http://ycl.jinqigufen.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://zmy.zycfv.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://qpe.jianghu66.top

Ruby: arr.select { |x| x > 3 }
来源：http://nrt.hammf.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://pcq.sweek.top

[D14] 映射转换（每个元素变形）
来源：http://fhp.havefunace.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://env.svipenyu.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://onr.guannengcc.top

JS:   arr.map(x => x * 2)
来源：http://cvy.tianlin.xyz

TS:   arr.map(x => x * 2)
来源：http://yjm.smart0.xyz

Java: list.stream().map(x -> x * 2).toList()
来源：http://fdz.yj20258.top

Go:   // 手写循环
来源：http://sno.zhengqikj.top

Ruby: arr.map { |x| x * 2 }
来源：http://nvh.yj202588.top

C#:   list.Select(x => x * 2).ToList()
来源：http://yus.hnxiangtu.top

[D15] 去重
来源：http://mbu.zhixingplan.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://vwl.daria6918.cn

PHP:  array_unique($arr);
来源：http://dxz.mhx1999.top

JS:   [...new Set(arr)]
来源：http://vhd.haohaochexian.top

TS:   [...new Set(arr)]
来源：http://ezq.shzxlz.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://dtv.ydzc1.top

Go:   // 用 map[T]struct{} 手写
来源：http://stt.hammf.cn

Ruby: arr.uniq
来源：http://xns.yj20258888.top

C#:   list.Distinct().ToList()
来源：http://sol.dianchejie.cn

[D16] 求和与平均值
来源：http://qrw.yj20258888.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://raw.zycfv.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://kgr.hnxiangtu.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://fto.havefunace.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://qfm.dianchejie.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://zig.yuxming.cn

Go:   // 手写循环累加
来源：http://svt.quarkkingdee.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://vun.cdnleiting.top

C#:   list.Sum();  list.Average()
来源：http://iqv.nwbrower.top

[D17] 最大值与最小值
来源：http://aou.jqgufenzy.top

Py:   max(arr);  min(arr)
来源：http://gbu.cdnleiting.top

PHP:  max($arr);  min($arr);
来源：http://hol.sxryk.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://cxp.hammf.cn

TS:   Math.max(...arr);
来源：http://jbd.yueranfly.top

Java: Collections.max(list);  Collections.min(list);
来源：http://ida.jqgfzy.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://cgl.dianchejie.cn

Ruby: arr.max;  arr.min
来源：http://vay.aibaodan.cn

C#:   list.Max();  list.Min()
来源：http://vod.yj20258.top

[D18] 扁平化嵌套数组
来源：http://vsh.cqqwz.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://oav.fzhhl.top

PHP:  array_merge(...$nested);
来源：http://mdh.gogol.net.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://jdy.svipenyu.cn

TS:   nested.flat();
来源：http://ocr.ivvv.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://uae.havefunace.top

Go:   // 手写双层循环
来源：http://qyz.tarul.cn

Ruby: nested.flatten
来源：http://bnz.zhongyouzk.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://tlf.jqgufenzy.top

[D19] 按字段分组
来源：http://iia.xingfuxueyuan.xyz

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://eri.shanyushiyangkeji.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://erw.smart0.xyz

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hvt.yfazqb.com

TS:   Object.groupBy(arr, x => x.type)
来源：http://pib.zycfv.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://def.jinqigfzy.top

Go:   // 手写 map[string][]T
来源：http://xgw.shanyushiyangkeji.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://uyf.zhoulong.xyz

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://mxr.andypj.xyz

[D20] 统计每个元素出现次数
来源：http://act.fengsongda.top

Py:   Counter(arr)
来源：http://uop.ehwqpu.com

PHP:  array_count_values($arr);
来源：http://dmu.fengsongda.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://kbl.yueranfly.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://vmr.jiagoushi.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://epe.shuidangran.top

Go:   // 手写 map[T]int
来源：http://qgu.tian-w.cn

Ruby: arr.tally
来源：http://lcw.yanxiufei.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://zsp.c1oappe.top

[D21] 判断是否包含某元素
来源：http://jkg.wangdashe.top

Py:   x in arr
来源：http://pxz.cqqwz.cn

PHP:  in_array($x, $arr, true);
来源：http://ena.wangshuangyany.cn

JS:   arr.includes(x)
来源：http://rsy.jianghu66.top

TS:   arr.includes(x)
来源：http://igv.feifeiyinyue.top

Java: list.contains(x)
来源：http://mtf.guannengcc.top

Go:   slices.Contains(arr, x)
来源：http://xbw.xingfuxueyuan.xyz

Ruby: arr.include?(x)
来源：http://lyl.shanyushiyangkeji.top

C#:   list.Contains(x)
来源：http://ekj.xuetiantiany.cn

[D22] 复制数组（避免共享引用）
来源：http://ruz.fehbvm.com

Py:   arr.copy();  arr[:];  list(arr)
来源：http://kzb.hfpthk.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://bxf.jinqigfzy.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://xhx.hcnkem.com

TS:   [...arr];
来源：http://yib.tian-w.cn

Java: new ArrayList<>(list);
来源：http://tnp.hcnkem.com

Go:   copied := append([]int(nil), arr...)
来源：http://pji.guowangkeji.top

Ruby: arr.dup;  arr.clone
来源：http://lpk.dianchejie.cn

C#:   new List<int>(list);
来源：http://akx.tianlin.xyz

[D23] reduce 累积计算
来源：http://pzg.yuxming.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://qpf.yj20258888.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://fmx.daxiang520.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://xiy.hesvh.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://yly.ehwqpu.com

Java: list.stream().reduce(0, Integer::sum)
来源：http://oyp.haohaochexian.top

Go:   // 手写循环
来源：http://pau.fzhhl.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://prz.ybcxt.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://tci.smart0.xyz

[D24] 字典 / Map 基本操作
来源：http://jqa.zhongyouzk.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://byu.316326.xyz

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hwr.iojbl.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://elf.hywenlv.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://xge.gaohongyu789.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://sir.cheryme.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://rtz.xylfe.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://gyx.wangdashe.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://ayw.jqgufenzy.top

[D25] Set 集合去重与交并差
来源：http://xme.hesvh.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://mfb.dashuyun.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://brs.aizwys.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://zlq.zhiwuduotai.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://lyn.sxryk.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://kzq.svipenyu.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hxl.kuanghao11.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://ysd.ydjk.org.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://wug.ydjk.org.cn

[D26] 数组转字符串
来源：http://dpj.uphjek.com

Py:   ", ".join(map(str, arr))
来源：http://ajh.cashguo.top

PHP:  implode(", ", $arr);
来源：http://vyb.hywenlv.cn

JS:   arr.join(", ")
来源：http://ghh.yuxming.cn

TS:   arr.join(", ")
来源：http://cvl.pengpengdd.cyou


<!-- 参考信息 -->