代发 wailian999

[C10] 变量作用域
来源：http://row.hfpthk.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://flv.yj202588.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://gjv.bjfxy.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://cwv.ydzc1.top

TS:   同 JS
来源：http://puv.sufxvd.cn

Java: 方法内为块级作用域
来源：http://jfb.ctjpmb.com

Go:   花括号块级作用域
来源：http://rpr.jinqigfzy.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://veo.cucudq.cn

C#:   块级作用域
来源：http://dcd.xuanzx.com

[C11] 模块导入与导出
来源：http://zbl.hywenlv.cn

Py:   from module import func
来源：http://gsr.fanxiaobao.xyz

PHP:  require "file.php";  或 use App\Service;
来源：http://mro.hnqzz.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://lpi.gogol.net.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://iar.shanyushiyangtech.top

Java: import java.util.List;
来源：http://ecc.smart0.xyz

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://nou.gaohongyu789.top

Ruby: require "json"; require_relative "./util"
来源：http://hwo.xingfuxueyuan.xyz

C#:   using System.Text;
来源：http://tbu.pengpengdd.cyou

[C12] 立即执行函数 IIFE
来源：http://klz.pycfn.com

Py:   (lambda: print("run"))()
来源：http://aah.cucudq.cn

PHP:  (function () { echo "run"; })();
来源：http://vkb.shuidangran.top

JS:   (() => { console.log("run"); })();
来源：http://utm.hnqzz.top

TS:   (() => { console.log("run"); })();
来源：http://khn.snrcjt.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://xdf.ybcxt.top

Go:   func() { fmt.Println("run") }()
来源：http://cvi.bbcook.cn

Ruby: -> { puts "run" }.call
来源：http://tjz.hongshengwenyu.top

C#:   // 无 IIFE：用静态构造函数
来源：http://mdl.yj20258.top

[C13] 类型声明 / 类型注解
来源：http://vjo.hcnkem.com

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://cuz.chenjidiqi.icu

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ytr.tian-w.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://kti.guowangkeji.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://aew.meibo888.top

Java: int add(int a, int b) { return a + b; }
来源：http://sde.zhengqikj.top

Go:   func add(a, b int) int
来源：http://lyy.52xcode.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://mme.sysykeji.top

C#:   int Add(int a, int b) => a + b;
来源：http://fzc.hnxiangtu.top

[C14] 泛型函数
来源：http://amu.zdqjudy.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://wcl.yj20258888.top

PHP:  // 无泛型
来源：http://gkd.redwolf501.top

JS:   // 无泛型
来源：http://wyf.yangfankeji.com

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://zgo.fengsongda.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://qgf.zhiwuduotai.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://nhv.hywenlv.cn

Ruby: # 无泛型
来源：http://zlc.birdmap.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://jct.snrcjt.cn

[C15] 解构 / 展开参数
来源：http://sjy.jinqigfzy.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://bfn.yuanzhike.top

PHP:  [$a, $b] = $pair;
来源：http://zob.cdnleiting.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://evl.zhaomingkeji.xyz

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://uoc.aibaodan.cn

Java: // 无解构
来源：http://vyy.tian-w.cn

Go:   // 无解构
来源：http://vuv.shuidangran.top

Ruby: a, b = pair
来源：http://ryg.tarul.cn

C#:   var (a, b) = pair;
来源：http://yli.pycfn.com

[C16] 函数 / 方法重载
来源：http://ivm.zhengqikj.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hhj.yvedp.cn

PHP:  // 无重载
来源：http://pkv.xingfuxueyuan.xyz

JS:   // 无重载：靠 arguments.length 分支
来源：http://huo.hfpthk.cn

TS:   // 用联合类型或重载签名声明
来源：http://jaf.yj202588.top

Java: void f(int a) {}  void f(String a) {}
来源：http://dqo.shanyushiyangtech.top

Go:   // 无重载：用不同函数名
来源：http://ofo.daria6918.cn

Ruby: # 无重载：靠动态参数
来源：http://cyg.hammf.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://ewl.cqqwz.cn

================================================================================
来源：http://rvd.ybcxt.top

D. 数组 / 列表 / 集合
来源：http://rxs.smart0.xyz

================================================================================
来源：http://aad.fzhhl.top

[D01] 创建数组 / 列表
来源：http://wpa.ydjk.org.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://mxm.epnwcf.com

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://ovv.nanxuanxn.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://jkk.aizwys.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://lpx.yfazqb.com

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://gcj.mhx1999.top

Go:   arr := []int{1, 2, 3}
来源：http://wdm.chenjidiqi.icu

Ruby: arr = [1, 2, 3]
来源：http://utv.yj202588.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://zxg.svipenyu.cn

[D02] 追加元素到末尾
来源：http://lox.tianlin.xyz

Py:   arr.append(4); arr.extend([5, 6])
来源：http://jwo.chenlongwang.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hch.cdnleiting.top

JS:   arr.push(4);
来源：http://lpu.yonumen.top

TS:   arr.push(4);
来源：http://tjh.aibaodan.cn

Java: list.add(4);
来源：http://mus.jinyuanbaomall.cn

Go:   arr = append(arr, 4)
来源：http://how.dashuyun.cn

Ruby: arr << 4; arr.push(5)
来源：http://ahf.c1oappe.top

C#:   list.Add(4);
来源：http://dtb.yfazqb.com

[D03] 在指定位置插入元素
来源：http://phr.sxryk.cn

Py:   arr.insert(0, 0)
来源：http://dpe.mhx1999.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://qjg.andypj.xyz

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://wiy.hnqzz.top

TS:   arr.splice(0, 0, 0);
来源：http://zfa.sysykeji.top

Java: list.add(0, 0);
来源：http://lun.zhengqikj.top

Go:   arr = append([]int{0}, arr...)
来源：http://urz.jlsjyb.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://gri.cucudq.cn

C#:   list.Insert(0, 0);
来源：http://bti.tianlin.xyz

[D04] 删除元素
来源：http://vpm.cqqwz.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://nsj.jyoumei.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://eph.vqdsnc.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://zmt.316326.xyz

TS:   arr.splice(0, 1);
来源：http://ipd.ydzc1.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://psl.hnxiangtu.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://iig.c1oappe.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://ico.jinqigufen.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://yqu.zhongyouzk.top

[D05] 访问与修改元素
来源：http://dik.nanxinkj.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://cao.ivvv.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://mvl.wangdashe.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://uga.ydjk.org.cn

TS:   arr[0]; arr.at(-1);
来源：http://ouc.vqdsnc.cn

Java: list.get(0); list.set(0, 9);
来源：http://pvb.jqgfzy.top

Go:   arr[0]; arr[0] = 9
来源：http://dao.hcnkem.com

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://lpy.iojbl.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://snx.sysykeji.top

[D06] 数组长度
来源：http://uuv.zhiwuduotai.top

Py:   len(arr)
来源：http://yyw.c1oappe.top

PHP:  count($arr);
来源：http://vrg.jyoumei.cn

JS:   arr.length
来源：http://thd.andypj.xyz

TS:   arr.length
来源：http://mjb.xylfe.cn

Java: list.size();
来源：http://umo.sjlbkw.cn

Go:   len(arr)
来源：http://ohr.fanxiaobao.xyz

Ruby: arr.length; arr.size
来源：http://uxo.kuanghao11.cn

C#:   list.Count;
来源：http://zzk.zycfv.cn

[D07] 切片 / 取子数组
来源：http://nyx.cashguo.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://ulz.zhongyouzk.top

PHP:  array_slice($arr, 1, 3);
来源：http://wyk.guannengcc.top

JS:   arr.slice(1, 4);
来源：http://rty.cashguo.top

TS:   arr.slice(1, 4);
来源：http://saa.hcnkem.com

Java: list.subList(1, 4);
来源：http://ltj.gaohongyu789.top

Go:   arr[1:4]
来源：http://twq.sjlbkw.cn

Ruby: arr[1, 3]
来源：http://ucl.sufxvd.cn

C#:   list.GetRange(1, 3);
来源：http://kxf.ppjwa.cn

[D08] 合并两个数组
来源：http://lcw.xinyue.icu

Py:   a + b;  a.extend(b)
来源：http://mna.hfpthk.cn

PHP:  array_merge($a, $b);
来源：http://fci.jinqigufen.top

JS:   [...a, ...b];  a.concat(b);
来源：http://nyh.fanxiaobao.xyz

TS:   [...a, ...b];
来源：http://kno.0kj1m.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://agm.gzhubu.top

Go:   append(a, b...)
来源：http://xys.quarkkingdee.top

Ruby: a + b;  a.concat(b)
来源：http://djh.dashuyun.cn

C#:   a.Concat(b).ToList()
来源：http://yqw.pengpengdd.cyou

[D09] 排序（升序）
来源：http://tcq.zhoulong.xyz

Py:   sorted(arr);  arr.sort()
来源：http://qwi.52xcode.cn

PHP:  sort($arr);
来源：http://ela.zhiwuduotai.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://ptt.wangdashe.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://nes.daxiang520.top

Java: Collections.sort(list);  list.sort(null);
来源：http://hzf.cqqwz.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://den.52xcode.cn

Ruby: arr.sort
来源：http://tea.gzhubu.top

C#:   list.Sort();
来源：http://wof.tian-w.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://ykq.zdqjudy.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://cpt.52xcode.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://jne.nanxuanxn.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://crp.nwbrower.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://xsy.ctjpmb.com

Java: list.sort(Comparator.comparing(Person::age));
来源：http://xzd.birdmap.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://tvb.ctjpmb.com

Ruby: arr.sort_by { |x| x[:age] }
来源：http://cqp.ydzc1.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://ary.tian-w.cn

[D11] 反转数组
来源：http://amn.zdqjudy.top

Py:   arr[::-1];  arr.reverse()
来源：http://cqm.shanyushiyangtech.top

PHP:  array_reverse($arr);
来源：http://mjl.shangyingyoupin.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://ryf.hesvh.cn

TS:   [...arr].reverse();
来源：http://rtq.hnqzz.top

Java: Collections.reverse(list);
来源：http://sfs.hammf.cn

Go:   slices.Reverse(arr)
来源：http://lji.iojbl.cn

Ruby: arr.reverse
来源：http://rdj.vqdsnc.cn

C#:   list.Reverse();
来源：http://upb.gzhubu.top

[D12] 查找元素下标
来源：http://rrx.sweek.top

Py:   arr.index(x);  x in arr
来源：http://wul.jianghu66.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://ajw.redwolf501.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://vdq.hcnkem.com

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://toi.svipenyu.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://itf.ybcxt.top

Go:   slices.Index(arr, x)
来源：http://ugo.c1oappe.top

Ruby: arr.index(x)
来源：http://ddz.0kj1m.cn

C#:   list.IndexOf(x);
来源：http://tob.kuanghao11.cn

[D13] 过滤（保留满足条件的）
来源：http://hci.xingfuxueyuan.xyz

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://xxe.fzhhl.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://npl.aibaodan.cn

JS:   arr.filter(x => x > 3)
来源：http://xdd.shuidangran.top

TS:   arr.filter(x => x > 3)
来源：http://tau.vqdsnc.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://ris.hnqzz.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://jom.xziqi.cn

Ruby: arr.select { |x| x > 3 }
来源：http://hwl.yuanzhike.top

C#:   list.Where(x => x > 3).ToList()
来源：http://tug.yfazqb.com

[D14] 映射转换（每个元素变形）
来源：http://gsf.gaohongyu789.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://toy.svipenyu.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://mid.aibaodan.cn

JS:   arr.map(x => x * 2)
来源：http://xvg.ivvv.top

TS:   arr.map(x => x * 2)
来源：http://asj.ybcxt.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://toa.iojbl.cn

Go:   // 手写循环
来源：http://hau.snrcjt.cn

Ruby: arr.map { |x| x * 2 }
来源：http://oms.sxryk.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://rwe.yongpay.top

[D15] 去重
来源：http://oou.zhiwuduotai.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://dzi.316326.xyz

PHP:  array_unique($arr);
来源：http://uyk.jqgufenzy.top

JS:   [...new Set(arr)]
来源：http://drk.jinghuilouyu.cn

TS:   [...new Set(arr)]
来源：http://nbq.andypj.xyz

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://fwd.xinyue.icu

Go:   // 用 map[T]struct{} 手写
来源：http://wbn.dianchejie.cn

Ruby: arr.uniq
来源：http://jpl.yuxming.cn

C#:   list.Distinct().ToList()
来源：http://mph.zhengqikj.top

[D16] 求和与平均值
来源：http://bpq.fzhhl.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://wxf.zhongyouzk.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://kdr.vqdsnc.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://wdh.dianchejie.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://ebc.sjlbkw.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://zmr.haohaochexian.top

Go:   // 手写循环累加
来源：http://muw.xuanzx.com

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://npb.zdqjudy.top

C#:   list.Sum();  list.Average()
来源：http://pux.fanxiaobao.xyz

[D17] 最大值与最小值
来源：http://aoa.jqgufenzy.top

Py:   max(arr);  min(arr)
来源：http://uib.shuidangran.top

PHP:  max($arr);  min($arr);
来源：http://brj.zhongyouzk.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://qkz.jinghuilouyu.cn

TS:   Math.max(...arr);
来源：http://xqj.gogol.net.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://bcd.zhaomingkeji.xyz

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://ojo.zycfv.cn

Ruby: arr.max;  arr.min
来源：http://hms.fengsongda.top

C#:   list.Max();  list.Min()
来源：http://uyf.haohaochexian.top

[D18] 扁平化嵌套数组
来源：http://ymi.316326.xyz

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://eoc.dianchejie.cn

PHP:  array_merge(...$nested);
来源：http://ezb.cucudq.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://oen.fktsv.cn

TS:   nested.flat();
来源：http://kvz.yfazqb.com

Java: nested.stream().flatMap(List::stream).toList()
来源：http://mis.yuanzhike.top

Go:   // 手写双层循环
来源：http://yon.chenjidiqi.icu

Ruby: nested.flatten
来源：http://hhd.hywenlv.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://dlu.feifeiyinyue.top

[D19] 按字段分组
来源：http://twy.hfpthk.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://wtn.xinyue.icu

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://inu.havefunace.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://kit.hnqzz.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://vyn.yangfankeji.com

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://vfh.aibaodan.cn

Go:   // 手写 map[string][]T
来源：http://rrl.316326.xyz

Ruby: arr.group_by { |x| x[:type] }
来源：http://jdw.tian-w.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://ihq.yuanzhike.top

[D20] 统计每个元素出现次数
来源：http://vmd.bbcook.cn

Py:   Counter(arr)
来源：http://xjb.yueranfly.top

PHP:  array_count_values($arr);
来源：http://jyx.yuxming.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://vxc.hfpthk.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://iky.xylfe.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://bqd.hywenlv.cn

Go:   // 手写 map[T]int
来源：http://jxu.bbcook.cn

Ruby: arr.tally
来源：http://jay.chenzaomai.com

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://pet.bjfxy.top

[D21] 判断是否包含某元素
来源：http://wnj.fehbvm.com

Py:   x in arr
来源：http://mmh.zhijiandao.cn

PHP:  in_array($x, $arr, true);
来源：http://rqx.fehbvm.com

JS:   arr.includes(x)
来源：http://yxb.sxryk.cn

TS:   arr.includes(x)
来源：http://hlg.yj20258888.top

Java: list.contains(x)
来源：http://knf.fktsv.cn

Go:   slices.Contains(arr, x)
来源：http://lvf.hfpthk.cn

Ruby: arr.include?(x)
来源：http://jru.cdnleiting.top

C#:   list.Contains(x)
来源：http://lko.zhoulong.xyz

[D22] 复制数组（避免共享引用）
来源：http://zeb.52xcode.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://yyc.chenzaomai.com

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://jgr.hnqzz.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://ikq.nanxuanxn.top

TS:   [...arr];
来源：http://vjn.gaohongyu789.top

Java: new ArrayList<>(list);
来源：http://cjy.yfazqb.com

Go:   copied := append([]int(nil), arr...)
来源：http://fnm.9152youxi.cn

Ruby: arr.dup;  arr.clone
来源：http://fcq.nwbrower.top

C#:   new List<int>(list);
来源：http://ygp.sufxvd.cn

[D23] reduce 累积计算
来源：http://nbs.ydjk.org.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://vof.smart0.xyz

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://zdn.hnxiangtu.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://udq.tian-w.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://gso.shangyingyoupin.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://qqe.hysaishi.cn

Go:   // 手写循环
来源：http://nvh.wangshuangyany.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://koq.vqdsnc.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://vuw.guannengcc.top

[D24] 字典 / Map 基本操作
来源：http://jjo.pengpengdd.cyou

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://sed.nwbrower.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://ved.zhiwuduotai.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://tek.hcnkem.com

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://cva.hnqzz.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://tds.yangfankeji.com

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://bel.feifeiyinyue.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://cyg.gaohongyu789.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://wyd.xingfuxueyuan.xyz

[D25] Set 集合去重与交并差
来源：http://bgi.jinyuanbaomall.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://cpt.daria6918.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://kot.snrcjt.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://frb.chenzaomai.com

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://wom.quarkkingdee.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://gxp.yj202588.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://bgp.cdnleiting.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://ylm.hnqzz.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://dss.tian-w.cn

[D26] 数组转字符串
来源：http://qgn.yuxming.cn

Py:   ", ".join(map(str, arr))
来源：http://zqs.bjfxy.top

PHP:  implode(", ", $arr);
来源：http://knk.hnqzz.top

JS:   arr.join(", ")
来源：http://bbd.haohaochexian.top

TS:   arr.join(", ")
来源：http://jud.redwolf501.top

Java: String.join(", ", list)
来源：http://enn.shanyushiyangkeji.top

Go:   strings.Join(strs, ", ")
来源：http://wnd.yanxiufei.cn

Ruby: arr.join(", ")
来源：http://vfk.quarkkingdee.top

C#:   string.Join(", ", list)
来源：http://unh.0kj1m.cn


<!-- 参考信息 -->