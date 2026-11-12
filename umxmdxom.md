代发 wailian999

[C10] 变量作用域
来源：http://qak.zdqjudy.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://kdv.yongpay.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://pyy.fengsongda.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://bqk.tanke756.top

TS:   同 JS
来源：http://zii.svipenyu.cn

Java: 方法内为块级作用域
来源：http://xml.sjlbkw.cn

Go:   花括号块级作用域
来源：http://gfy.iojbl.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://ggo.guowangkeji.top

C#:   块级作用域
来源：http://bsr.ybcxt.top

[C11] 模块导入与导出
来源：http://zgd.bbcook.cn

Py:   from module import func
来源：http://pfn.hnqzz.top

PHP:  require "file.php";  或 use App\Service;
来源：http://dks.yvedp.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://qta.hfpthk.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://vry.jinghuilouyu.cn

Java: import java.util.List;
来源：http://wnz.meibo888.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://etq.yangfankeji.com

Ruby: require "json"; require_relative "./util"
来源：http://pwd.316326.xyz

C#:   using System.Text;
来源：http://pli.daria6918.cn

[C12] 立即执行函数 IIFE
来源：http://xnv.xziqi.cn

Py:   (lambda: print("run"))()
来源：http://dpx.sxryk.cn

PHP:  (function () { echo "run"; })();
来源：http://xwv.xylfe.cn

JS:   (() => { console.log("run"); })();
来源：http://tjf.yj202588.top

TS:   (() => { console.log("run"); })();
来源：http://htr.haohaochexian.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://sjp.dianchejie.cn

Go:   func() { fmt.Println("run") }()
来源：http://avf.ivvv.top

Ruby: -> { puts "run" }.call
来源：http://yab.vehdjk.com

C#:   // 无 IIFE：用静态构造函数
来源：http://fde.jinqigufen.top

[C13] 类型声明 / 类型注解
来源：http://fgv.tanke756.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://ftu.nanxinkj.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://rna.ywan-chungtsiang.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://raz.jqgufenzy.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://sth.nanxinkj.top

Java: int add(int a, int b) { return a + b; }
来源：http://qrl.yvedp.cn

Go:   func add(a, b int) int
来源：http://bxh.xuanzx.com

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://kfj.hfpthk.cn

C#:   int Add(int a, int b) => a + b;
来源：http://onc.wangshuangyany.cn

[C14] 泛型函数
来源：http://skn.fanxiaobao.xyz

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hpd.ppjwa.cn

PHP:  // 无泛型
来源：http://voo.bbcook.cn

JS:   // 无泛型
来源：http://bqj.vqdsnc.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://suf.cqqwz.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://wke.zhixingplan.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://ahb.jqgufenzy.top

Ruby: # 无泛型
来源：http://gbd.fengsongda.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://njf.quarkkingdee.top

[C15] 解构 / 展开参数
来源：http://qmf.yuanzhike.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://woc.zhixingplan.top

PHP:  [$a, $b] = $pair;
来源：http://oyq.bbcook.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://jsr.daria6918.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hjq.epnwcf.com

Java: // 无解构
来源：http://ovb.chenzaomai.com

Go:   // 无解构
来源：http://gdv.zycfv.cn

Ruby: a, b = pair
来源：http://zcm.xuanzx.com

C#:   var (a, b) = pair;
来源：http://apl.xziqi.cn

[C16] 函数 / 方法重载
来源：http://ktn.wangshuangyany.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://ehm.tian-w.cn

PHP:  // 无重载
来源：http://rlp.iojbl.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://rwf.daria6918.cn

TS:   // 用联合类型或重载签名声明
来源：http://htx.jinqigufen.top

Java: void f(int a) {}  void f(String a) {}
来源：http://qrj.cdnleiting.top

Go:   // 无重载：用不同函数名
来源：http://axs.sxryk.cn

Ruby: # 无重载：靠动态参数
来源：http://zvt.ywan-chungtsiang.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://ctf.zhixingplan.top

================================================================================
来源：http://tty.fktsv.cn

D. 数组 / 列表 / 集合
来源：http://hmw.xziqi.cn

================================================================================
来源：http://ied.shzxlz.cn

[D01] 创建数组 / 列表
来源：http://trx.redwolf501.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://hju.yuanzhike.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://ywb.yuanzhike.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://yve.hnxiangtu.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://nig.zdqjudy.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://nyr.chenzaomai.com

Go:   arr := []int{1, 2, 3}
来源：http://uck.vqdsnc.cn

Ruby: arr = [1, 2, 3]
来源：http://ozm.daria6918.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://lyo.zhoulong.xyz

[D02] 追加元素到末尾
来源：http://wjc.gotoacloud.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://ehk.jqgufenzy.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://xcp.zhaomingkeji.xyz

JS:   arr.push(4);
来源：http://rms.epnwcf.com

TS:   arr.push(4);
来源：http://yir.xuetiantiany.cn

Java: list.add(4);
来源：http://qhk.cdnleiting.top

Go:   arr = append(arr, 4)
来源：http://wuf.redwolf501.top

Ruby: arr << 4; arr.push(5)
来源：http://rea.ctjpmb.com

C#:   list.Add(4);
来源：http://ytq.gogol.net.cn

[D03] 在指定位置插入元素
来源：http://qth.ctjpmb.com

Py:   arr.insert(0, 0)
来源：http://usk.yonumen.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://jzi.jinqigufen.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://loa.hongshengwenyu.top

TS:   arr.splice(0, 0, 0);
来源：http://adc.nanxinkj.top

Java: list.add(0, 0);
来源：http://ohm.ctjpmb.com

Go:   arr = append([]int{0}, arr...)
来源：http://khd.snrcjt.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://zuh.shanyushiyangtech.top

C#:   list.Insert(0, 0);
来源：http://ztn.cheryme.top

[D04] 删除元素
来源：http://nvs.hnqzz.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://pkz.redwolf501.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://qxp.ywan-chungtsiang.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://wby.zdbjq.cn

TS:   arr.splice(0, 1);
来源：http://tjg.bbcook.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://oew.xingfuxueyuan.xyz

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://xdn.cheryme.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://syi.smart0.xyz

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://ruo.ppjwa.cn

[D05] 访问与修改元素
来源：http://rhc.aizwys.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://ufc.birdmap.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://drk.jyoumei.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://tup.yvedp.cn

TS:   arr[0]; arr.at(-1);
来源：http://uyc.feifeiyinyue.top

Java: list.get(0); list.set(0, 9);
来源：http://ehf.daria6918.cn

Go:   arr[0]; arr[0] = 9
来源：http://sdi.zhaomingkeji.xyz

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://dpg.316326.xyz

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://nuw.sjlbkw.cn

[D06] 数组长度
来源：http://fvf.shanyushiyangtech.top

Py:   len(arr)
来源：http://via.daria6918.cn

PHP:  count($arr);
来源：http://pgq.jyoumei.cn

JS:   arr.length
来源：http://uyq.zhixingplan.top

TS:   arr.length
来源：http://xma.jinqigufen.top

Java: list.size();
来源：http://fqu.yongpay.top

Go:   len(arr)
来源：http://aix.aizwys.cn

Ruby: arr.length; arr.size
来源：http://tlr.yanxiufei.cn

C#:   list.Count;
来源：http://uyx.jqgfzy.top

[D07] 切片 / 取子数组
来源：http://bgk.yueranfly.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://keg.zhijiandao.cn

PHP:  array_slice($arr, 1, 3);
来源：http://ozg.vqdsnc.cn

JS:   arr.slice(1, 4);
来源：http://tjw.ydjk.org.cn

TS:   arr.slice(1, 4);
来源：http://iib.sweek.top

Java: list.subList(1, 4);
来源：http://aam.gaohongyu789.top

Go:   arr[1:4]
来源：http://qmu.feifeiyinyue.top

Ruby: arr[1, 3]
来源：http://upl.jinqigfzy.top

C#:   list.GetRange(1, 3);
来源：http://bob.jiagoushi.top

[D08] 合并两个数组
来源：http://cae.wangshuangyany.cn

Py:   a + b;  a.extend(b)
来源：http://jjy.c1oappe.top

PHP:  array_merge($a, $b);
来源：http://fkx.gaohongyu789.top

JS:   [...a, ...b];  a.concat(b);
来源：http://hgv.cucudq.cn

TS:   [...a, ...b];
来源：http://sef.pengpengdd.cyou

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hkp.zhixingplan.top

Go:   append(a, b...)
来源：http://pmt.jinghuilouyu.cn

Ruby: a + b;  a.concat(b)
来源：http://tta.mhx1999.top

C#:   a.Concat(b).ToList()
来源：http://qsd.hnqzz.top

[D09] 排序（升序）
来源：http://luu.yj202588.top

Py:   sorted(arr);  arr.sort()
来源：http://bsx.dianchejie.cn

PHP:  sort($arr);
来源：http://jdc.shuidangran.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://aak.yvedp.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://uqb.pycfn.com

Java: Collections.sort(list);  list.sort(null);
来源：http://qiq.cheryme.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hrd.9152youxi.cn

Ruby: arr.sort
来源：http://jbl.nanxuanxn.top

C#:   list.Sort();
来源：http://cey.epnwcf.com

[D10] 自定义排序（按字段 / 多条件）
来源：http://jin.wangdashe.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://oml.birdmap.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ckc.sysykeji.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://sim.sxryk.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://sfc.sufxvd.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://iug.tianlin.xyz

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://iak.ehwqpu.com

Ruby: arr.sort_by { |x| x[:age] }
来源：http://pos.tarul.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://ytg.birdmap.top

[D11] 反转数组
来源：http://egc.yfazqb.com

Py:   arr[::-1];  arr.reverse()
来源：http://lwk.mhx1999.top

PHP:  array_reverse($arr);
来源：http://duy.guowangkeji.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://shr.hnxiangtu.top

TS:   [...arr].reverse();
来源：http://nva.yanxiufei.cn

Java: Collections.reverse(list);
来源：http://xwv.jlsjyb.cn

Go:   slices.Reverse(arr)
来源：http://ltk.hnqzz.top

Ruby: arr.reverse
来源：http://ump.havefunace.top

C#:   list.Reverse();
来源：http://jzd.ywan-chungtsiang.top

[D12] 查找元素下标
来源：http://wie.sjlbkw.cn

Py:   arr.index(x);  x in arr
来源：http://nub.yj20258.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://fjk.vqdsnc.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://pos.hnqzz.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://lyc.zhongyouzk.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://pwn.gaohongyu789.top

Go:   slices.Index(arr, x)
来源：http://qmu.ppjwa.cn

Ruby: arr.index(x)
来源：http://bem.kuanghao11.cn

C#:   list.IndexOf(x);
来源：http://hvl.ehwqpu.com

[D13] 过滤（保留满足条件的）
来源：http://kpm.xylfe.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://tvh.yongpay.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://jhu.yj20258888.top

JS:   arr.filter(x => x > 3)
来源：http://sff.hcnkem.com

TS:   arr.filter(x => x > 3)
来源：http://hwz.xuetiantiany.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://wum.sxryk.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://tfm.yj202588.top

Ruby: arr.select { |x| x > 3 }
来源：http://vwo.chenjidiqi.icu

C#:   list.Where(x => x > 3).ToList()
来源：http://jth.yanxiufei.cn

[D14] 映射转换（每个元素变形）
来源：http://dcq.daxiang520.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://mzi.iojbl.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://mri.ywan-chungtsiang.top

JS:   arr.map(x => x * 2)
来源：http://nzy.0kj1m.cn

TS:   arr.map(x => x * 2)
来源：http://map.jinyuanbaomall.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://slf.shanyushiyangkeji.top

Go:   // 手写循环
来源：http://lis.9152youxi.cn

Ruby: arr.map { |x| x * 2 }
来源：http://xkj.jlsjyb.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://ezc.sufxvd.cn

[D15] 去重
来源：http://svi.birdmap.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://jzf.hesvh.cn

PHP:  array_unique($arr);
来源：http://pbs.shanyushiyangtech.top

JS:   [...new Set(arr)]
来源：http://aar.yueranfly.top

TS:   [...new Set(arr)]
来源：http://gvj.pycfn.com

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://gcj.iojbl.cn

Go:   // 用 map[T]struct{} 手写
来源：http://gqf.jqgfzy.top

Ruby: arr.uniq
来源：http://ntv.zhaomingkeji.xyz

C#:   list.Distinct().ToList()
来源：http://udy.cheryme.top

[D16] 求和与平均值
来源：http://udl.sjlbkw.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://chq.yonumen.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://yra.jinghuilouyu.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://jjf.epnwcf.com

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://ftu.yangfankeji.com

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hdk.chenzaomai.com

Go:   // 手写循环累加
来源：http://pdm.jyoumei.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://dxm.tian-w.cn

C#:   list.Sum();  list.Average()
来源：http://zzu.hfpthk.cn

[D17] 最大值与最小值
来源：http://ped.fzhhl.top

Py:   max(arr);  min(arr)
来源：http://liw.havefunace.top

PHP:  max($arr);  min($arr);
来源：http://vdk.c1oappe.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://xwo.jlsjyb.cn

TS:   Math.max(...arr);
来源：http://rwd.feifeiyinyue.top

Java: Collections.max(list);  Collections.min(list);
来源：http://hqx.jqgufenzy.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://lat.zdbjq.cn

Ruby: arr.max;  arr.min
来源：http://ioj.vehdjk.com

C#:   list.Max();  list.Min()
来源：http://obm.52xcode.cn

[D18] 扁平化嵌套数组
来源：http://ybw.sxryk.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://ggz.zhaomingkeji.xyz

PHP:  array_merge(...$nested);
来源：http://uju.meibo888.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://fta.zhiwuduotai.top

TS:   nested.flat();
来源：http://cit.chenlongwang.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://ddy.vqdsnc.cn

Go:   // 手写双层循环
来源：http://exn.fktsv.cn

Ruby: nested.flatten
来源：http://hwb.zhengqikj.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://yhq.bjfxy.top

[D19] 按字段分组
来源：http://bex.jyoumei.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://bqy.yueranfly.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://vwt.shanyushiyangtech.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://rut.redwolf501.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://irg.chenzaomai.com

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://izd.gotoacloud.top

Go:   // 手写 map[string][]T
来源：http://npi.ydzc1.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://gla.hywenlv.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://web.nanxuanxn.top

[D20] 统计每个元素出现次数
来源：http://dni.c1oappe.top

Py:   Counter(arr)
来源：http://hkf.sysykeji.top

PHP:  array_count_values($arr);
来源：http://hbr.yj202588.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://tco.tian-w.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://yag.9152youxi.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://akc.guowangkeji.top

Go:   // 手写 map[T]int
来源：http://zro.epnwcf.com

Ruby: arr.tally
来源：http://acw.ywan-chungtsiang.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://vyf.316326.xyz

[D21] 判断是否包含某元素
来源：http://zwh.ydzc1.top

Py:   x in arr
来源：http://noq.zhiwuduotai.top

PHP:  in_array($x, $arr, true);
来源：http://uki.epnwcf.com

JS:   arr.includes(x)
来源：http://nvt.jinghuilouyu.cn

TS:   arr.includes(x)
来源：http://ksz.hesvh.cn

Java: list.contains(x)
来源：http://ipa.yj20258888.top

Go:   slices.Contains(arr, x)
来源：http://hdj.zhoulong.xyz

Ruby: arr.include?(x)
来源：http://gcm.fanxiaobao.xyz

C#:   list.Contains(x)
来源：http://nqy.nwbrower.top

[D22] 复制数组（避免共享引用）
来源：http://yaw.tanke756.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://uzb.shangyingyoupin.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://wcr.jinghuilouyu.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://mtj.sufxvd.cn

TS:   [...arr];
来源：http://pnj.xuanzx.com

Java: new ArrayList<>(list);
来源：http://gdz.xziqi.cn

Go:   copied := append([]int(nil), arr...)
来源：http://lpi.zhoulong.xyz

Ruby: arr.dup;  arr.clone
来源：http://fqy.zdqjudy.top

C#:   new List<int>(list);
来源：http://dsv.0kj1m.cn

[D23] reduce 累积计算
来源：http://nom.sufxvd.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://mka.yongpay.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hif.sxryk.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://uyb.xylfe.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://exe.jinqigfzy.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://iln.sxryk.cn

Go:   // 手写循环
来源：http://ggj.zhoulong.xyz

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://zky.wangshuangyany.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://iaf.zdqjudy.top

[D24] 字典 / Map 基本操作
来源：http://xio.jinqigufen.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://oeh.gzhubu.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://mzu.jinqigufen.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://dqn.xylfe.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://vla.epnwcf.com

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://gqz.hnxiangtu.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://cbf.kuanghao11.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://oxv.shzxlz.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://drf.smart0.xyz

[D25] Set 集合去重与交并差
来源：http://ysu.hcnkem.com

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://fda.52xcode.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://lcv.bjfxy.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://dwu.ehwqpu.com

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://lxj.0kj1m.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://fxe.gogol.net.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://bap.ydjk.org.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://mzq.meibo888.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://vga.uphjek.com

[D26] 数组转字符串
来源：http://rgv.sufxvd.cn

Py:   ", ".join(map(str, arr))
来源：http://dii.zdqjudy.top

PHP:  implode(", ", $arr);
来源：http://sdc.aibaodan.cn

JS:   arr.join(", ")
来源：http://xiv.guannengcc.top

TS:   arr.join(", ")
来源：http://man.cashguo.top

Java: String.join(", ", list)
来源：http://vtg.hfpthk.cn

Go:   strings.Join(strs, ", ")
来源：http://kts.jinqigufen.top

Ruby: arr.join(", ")
来源：http://dhw.daxiang520.top

C#:   string.Join(", ", list)
来源：http://jxl.ydjk.org.cn


<!-- 参考信息 -->