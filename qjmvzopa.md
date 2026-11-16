代发 wailian999

Ruby: require "json"; require_relative "./util"
来源：http://pxt.sysykeji.top

C#:   using System.Text;
来源：http://pel.cqqwz.cn

[C12] 立即执行函数 IIFE
来源：http://tpw.cashguo.top

Py:   (lambda: print("run"))()
来源：http://fwo.yuanzhike.top

PHP:  (function () { echo "run"; })();
来源：http://frj.zycfv.cn

JS:   (() => { console.log("run"); })();
来源：http://whm.tarul.cn

TS:   (() => { console.log("run"); })();
来源：http://uzo.shangyingyoupin.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://uci.pycfn.com

Go:   func() { fmt.Println("run") }()
来源：http://vtt.hcnkem.com

Ruby: -> { puts "run" }.call
来源：http://eca.ybcxt.top

C#:   // 无 IIFE：用静态构造函数
来源：http://fcx.jinqigufen.top

[C13] 类型声明 / 类型注解
来源：http://uhy.bjfxy.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://lrg.jqgufenzy.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://tin.nwbrower.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://mnk.jiagoushi.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://muq.daxiang520.top

Java: int add(int a, int b) { return a + b; }
来源：http://bvu.sxryk.cn

Go:   func add(a, b int) int
来源：http://gje.hnqzz.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://ahx.hongshengwenyu.top

C#:   int Add(int a, int b) => a + b;
来源：http://oyg.dashuyun.cn

[C14] 泛型函数
来源：http://igk.sufxvd.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://uxn.fehbvm.com

PHP:  // 无泛型
来源：http://pgx.feifeiyinyue.top

JS:   // 无泛型
来源：http://ppj.sweek.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://qwq.cheryme.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://bil.sxryk.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://kod.havefunace.top

Ruby: # 无泛型
来源：http://fah.yuxming.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://rim.sufxvd.cn

[C15] 解构 / 展开参数
来源：http://obj.fzhhl.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://dep.yongpay.top

PHP:  [$a, $b] = $pair;
来源：http://pip.svipenyu.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://bik.aibaodan.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://jdj.zhoulong.xyz

Java: // 无解构
来源：http://csm.dashuyun.cn

Go:   // 无解构
来源：http://mkf.xylfe.cn

Ruby: a, b = pair
来源：http://ocv.vqdsnc.cn

C#:   var (a, b) = pair;
来源：http://mey.hammf.cn

[C16] 函数 / 方法重载
来源：http://xrh.wangdashe.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://juu.guannengcc.top

PHP:  // 无重载
来源：http://slo.yonumen.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://rdl.andypj.xyz

TS:   // 用联合类型或重载签名声明
来源：http://hgr.epnwcf.com

Java: void f(int a) {}  void f(String a) {}
来源：http://fcf.fanxiaobao.xyz

Go:   // 无重载：用不同函数名
来源：http://sgi.mhx1999.top

Ruby: # 无重载：靠动态参数
来源：http://aqq.chenzaomai.com

C#:   void F(int a) {}  void F(string a) {}
来源：http://klg.nanxuanxn.top

================================================================================
来源：http://jvx.aibaodan.cn

D. 数组 / 列表 / 集合
来源：http://fzg.gogol.net.cn

================================================================================
来源：http://cpo.xuetiantiany.cn

[D01] 创建数组 / 列表
来源：http://mlr.cashguo.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://dmj.yanxiufei.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://rrh.ybcxt.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://smn.zycfv.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://hqe.cdnleiting.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://ebk.fanxiaobao.xyz

Go:   arr := []int{1, 2, 3}
来源：http://kkh.gotoacloud.top

Ruby: arr = [1, 2, 3]
来源：http://hik.dashuyun.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://iku.aizwys.cn

[D02] 追加元素到末尾
来源：http://mnv.9152youxi.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hew.ydzc1.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://wbw.ydzc1.top

JS:   arr.push(4);
来源：http://mzu.zycfv.cn

TS:   arr.push(4);
来源：http://tek.zhongyouzk.top

Java: list.add(4);
来源：http://yhm.pengpengdd.cyou

Go:   arr = append(arr, 4)
来源：http://jwp.guannengcc.top

Ruby: arr << 4; arr.push(5)
来源：http://wsd.yj20258888.top

C#:   list.Add(4);
来源：http://jrx.jqgfzy.top

[D03] 在指定位置插入元素
来源：http://ryw.pycfn.com

Py:   arr.insert(0, 0)
来源：http://vis.sweek.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://fac.smart0.xyz

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://bqh.9152youxi.cn

TS:   arr.splice(0, 0, 0);
来源：http://szd.nanxuanxn.top

Java: list.add(0, 0);
来源：http://aak.shanyushiyangkeji.top

Go:   arr = append([]int{0}, arr...)
来源：http://tvl.gaohongyu789.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://eke.52xcode.cn

C#:   list.Insert(0, 0);
来源：http://mwx.bjfxy.top

[D04] 删除元素
来源：http://fpq.ybcxt.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://tdx.zhengqikj.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://kdh.hnqzz.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://ebb.wangdashe.top

TS:   arr.splice(0, 1);
来源：http://eii.iojbl.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://gkf.hysaishi.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://nqo.shuidangran.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://mmi.sufxvd.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://flr.sxryk.cn

[D05] 访问与修改元素
来源：http://pih.zhiwuduotai.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://qbd.chenzaomai.com

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://kaa.fktsv.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://vvp.tanke756.top

TS:   arr[0]; arr.at(-1);
来源：http://rzf.zhengqikj.top

Java: list.get(0); list.set(0, 9);
来源：http://wwe.hcnkem.com

Go:   arr[0]; arr[0] = 9
来源：http://lmj.yuanzhike.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://uaq.0kj1m.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://ies.yonumen.top

[D06] 数组长度
来源：http://xrh.yvedp.cn

Py:   len(arr)
来源：http://imd.ppjwa.cn

PHP:  count($arr);
来源：http://kqb.cheryme.top

JS:   arr.length
来源：http://kvz.shanyushiyangkeji.top

TS:   arr.length
来源：http://agh.zhaomingkeji.xyz

Java: list.size();
来源：http://rgl.wangdashe.top

Go:   len(arr)
来源：http://xnq.sysykeji.top

Ruby: arr.length; arr.size
来源：http://liv.ywan-chungtsiang.top

C#:   list.Count;
来源：http://vsx.xylfe.cn

[D07] 切片 / 取子数组
来源：http://hmz.xylfe.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://etq.zhiwuduotai.top

PHP:  array_slice($arr, 1, 3);
来源：http://ygn.9152youxi.cn

JS:   arr.slice(1, 4);
来源：http://ylk.zhengqikj.top

TS:   arr.slice(1, 4);
来源：http://vss.chenjidiqi.icu

Java: list.subList(1, 4);
来源：http://wyk.jqgufenzy.top

Go:   arr[1:4]
来源：http://ifz.yongpay.top

Ruby: arr[1, 3]
来源：http://tia.bjfxy.top

C#:   list.GetRange(1, 3);
来源：http://nrk.jlsjyb.cn

[D08] 合并两个数组
来源：http://zng.wangshuangyany.cn

Py:   a + b;  a.extend(b)
来源：http://uaz.jinqigufen.top

PHP:  array_merge($a, $b);
来源：http://ghn.ehwqpu.com

JS:   [...a, ...b];  a.concat(b);
来源：http://iqh.zhiwuduotai.top

TS:   [...a, ...b];
来源：http://ktc.pengpengdd.cyou

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://ovq.9152youxi.cn

Go:   append(a, b...)
来源：http://tkc.xingfuxueyuan.xyz

Ruby: a + b;  a.concat(b)
来源：http://ego.meibo888.top

C#:   a.Concat(b).ToList()
来源：http://zft.aizwys.cn

[D09] 排序（升序）
来源：http://pup.hysaishi.cn

Py:   sorted(arr);  arr.sort()
来源：http://hxq.shanyushiyangtech.top

PHP:  sort($arr);
来源：http://otu.bjfxy.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://fcq.havefunace.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://boh.yuxming.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://qsy.tarul.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://nox.sysykeji.top

Ruby: arr.sort
来源：http://gud.bjfxy.top

C#:   list.Sort();
来源：http://pws.jyoumei.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://nbs.sweek.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://gdb.fzhhl.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://kzy.vehdjk.com

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://mkd.feifeiyinyue.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://rsa.guannengcc.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://tgh.yfazqb.com

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://itk.jyoumei.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://rnx.ydzc1.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hfd.c1oappe.top

[D11] 反转数组
来源：http://ctz.smart0.xyz

Py:   arr[::-1];  arr.reverse()
来源：http://zsd.fehbvm.com

PHP:  array_reverse($arr);
来源：http://xta.zhiwuduotai.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://moy.dashuyun.cn

TS:   [...arr].reverse();
来源：http://dus.ywan-chungtsiang.top

Java: Collections.reverse(list);
来源：http://eaz.yongpay.top

Go:   slices.Reverse(arr)
来源：http://upa.sufxvd.cn

Ruby: arr.reverse
来源：http://twy.hfpthk.cn

C#:   list.Reverse();
来源：http://aet.zhengqikj.top

[D12] 查找元素下标
来源：http://acg.fengsongda.top

Py:   arr.index(x);  x in arr
来源：http://ubv.quarkkingdee.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://duc.hammf.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ycc.zhixingplan.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ezy.hnxiangtu.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://ata.c1oappe.top

Go:   slices.Index(arr, x)
来源：http://vhu.c1oappe.top

Ruby: arr.index(x)
来源：http://cis.xziqi.cn

C#:   list.IndexOf(x);
来源：http://tcw.epnwcf.com

[D13] 过滤（保留满足条件的）
来源：http://tyg.hammf.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://jht.zhengqikj.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://dst.andypj.xyz

JS:   arr.filter(x => x > 3)
来源：http://zkz.redwolf501.top

TS:   arr.filter(x => x > 3)
来源：http://tgh.yanxiufei.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://rcq.zdqjudy.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://jod.fengsongda.top

Ruby: arr.select { |x| x > 3 }
来源：http://vfp.pycfn.com

C#:   list.Where(x => x > 3).ToList()
来源：http://axw.aizwys.cn

[D14] 映射转换（每个元素变形）
来源：http://wkj.dashuyun.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://bhx.fanxiaobao.xyz

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://gow.shanyushiyangtech.top

JS:   arr.map(x => x * 2)
来源：http://com.havefunace.top

TS:   arr.map(x => x * 2)
来源：http://xwa.tian-w.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://mju.jlsjyb.cn

Go:   // 手写循环
来源：http://puq.jlsjyb.cn

Ruby: arr.map { |x| x * 2 }
来源：http://krc.cdnleiting.top

C#:   list.Select(x => x * 2).ToList()
来源：http://wia.yuxming.cn

[D15] 去重
来源：http://qdk.kuanghao11.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://vql.zdbjq.cn

PHP:  array_unique($arr);
来源：http://vbh.zdbjq.cn

JS:   [...new Set(arr)]
来源：http://ycn.gogol.net.cn

TS:   [...new Set(arr)]
来源：http://kwi.gzhubu.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://bvh.ydzc1.top

Go:   // 用 map[T]struct{} 手写
来源：http://izw.epnwcf.com

Ruby: arr.uniq
来源：http://xfd.nanxuanxn.top

C#:   list.Distinct().ToList()
来源：http://isr.jyoumei.cn

[D16] 求和与平均值
来源：http://pjv.gogol.net.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://prk.shuidangran.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://kgf.uphjek.com

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://gum.cashguo.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://vfj.smart0.xyz

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://fjf.ydjk.org.cn

Go:   // 手写循环累加
来源：http://uvu.tanke756.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://buz.ywan-chungtsiang.top

C#:   list.Sum();  list.Average()
来源：http://vtu.andypj.xyz

[D17] 最大值与最小值
来源：http://qsu.dianchejie.cn

Py:   max(arr);  min(arr)
来源：http://tdv.hnxiangtu.top

PHP:  max($arr);  min($arr);
来源：http://mot.tian-w.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://mqi.ydzc1.top

TS:   Math.max(...arr);
来源：http://fan.havefunace.top

Java: Collections.max(list);  Collections.min(list);
来源：http://und.iojbl.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://doo.cdnleiting.top

Ruby: arr.max;  arr.min
来源：http://icy.sjlbkw.cn

C#:   list.Max();  list.Min()
来源：http://fhh.yj20258888.top

[D18] 扁平化嵌套数组
来源：http://rdn.xylfe.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://uel.zhiwuduotai.top

PHP:  array_merge(...$nested);
来源：http://xzg.yonumen.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://obu.yangfankeji.com

TS:   nested.flat();
来源：http://rsd.wangshuangyany.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://qxk.ydzc1.top

Go:   // 手写双层循环
来源：http://xqc.nanxinkj.top

Ruby: nested.flatten
来源：http://xqi.cucudq.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://iax.zhiwuduotai.top

[D19] 按字段分组
来源：http://fio.xziqi.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://rrt.shzxlz.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://dmc.bjfxy.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://dvf.pycfn.com

TS:   Object.groupBy(arr, x => x.type)
来源：http://jfe.meibo888.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://cxz.yfazqb.com

Go:   // 手写 map[string][]T
来源：http://wrq.xingfuxueyuan.xyz

Ruby: arr.group_by { |x| x[:type] }
来源：http://ttg.hcnkem.com

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://erm.guannengcc.top

[D20] 统计每个元素出现次数
来源：http://rig.zhongyouzk.top

Py:   Counter(arr)
来源：http://fcw.aibaodan.cn

PHP:  array_count_values($arr);
来源：http://sfb.dashuyun.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://dmg.yj20258888.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hbe.iojbl.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://fjd.hammf.cn

Go:   // 手写 map[T]int
来源：http://qfu.meibo888.top

Ruby: arr.tally
来源：http://vvk.quarkkingdee.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://tyd.zycfv.cn

[D21] 判断是否包含某元素
来源：http://uam.jqgufenzy.top

Py:   x in arr
来源：http://lzo.bbcook.cn

PHP:  in_array($x, $arr, true);
来源：http://hoc.316326.xyz

JS:   arr.includes(x)
来源：http://cwa.fktsv.cn

TS:   arr.includes(x)
来源：http://vih.pycfn.com

Java: list.contains(x)
来源：http://esh.fengsongda.top

Go:   slices.Contains(arr, x)
来源：http://bwd.jqgufenzy.top

Ruby: arr.include?(x)
来源：http://hil.fanxiaobao.xyz

C#:   list.Contains(x)
来源：http://fjt.xingfuxueyuan.xyz

[D22] 复制数组（避免共享引用）
来源：http://xyq.vehdjk.com

Py:   arr.copy();  arr[:];  list(arr)
来源：http://njq.aibaodan.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://mow.cheryme.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://ugp.sysykeji.top

TS:   [...arr];
来源：http://frd.zhaomingkeji.xyz

Java: new ArrayList<>(list);
来源：http://mub.uphjek.com

Go:   copied := append([]int(nil), arr...)
来源：http://roe.zhijiandao.cn

Ruby: arr.dup;  arr.clone
来源：http://aoc.yj20258.top

C#:   new List<int>(list);
来源：http://vky.wangshuangyany.cn

[D23] reduce 累积计算
来源：http://vpu.sjlbkw.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://vsg.dianchejie.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://nub.quarkkingdee.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ojj.chenzaomai.com

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://gir.jyoumei.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://isp.pengpengdd.cyou

Go:   // 手写循环
来源：http://tdy.9152youxi.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://dvk.xinyue.icu

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://lil.hammf.cn

[D24] 字典 / Map 基本操作
来源：http://obn.cashguo.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://gvv.guannengcc.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://ctj.yfazqb.com

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://yje.zycfv.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://pql.shanyushiyangkeji.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://ffl.ctjpmb.com

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://ifh.sjlbkw.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://bfy.iojbl.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://iab.kuanghao11.cn

[D25] Set 集合去重与交并差
来源：http://unw.daxiang520.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://ftj.pengpengdd.cyou

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://ypl.yj202588.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://tet.zdbjq.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://lto.ehwqpu.com

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://cew.aibaodan.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://jsf.nanxuanxn.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://lee.meibo888.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://iav.52xcode.cn

[D26] 数组转字符串
来源：http://rcf.9152youxi.cn

Py:   ", ".join(map(str, arr))
来源：http://lse.quarkkingdee.top

PHP:  implode(", ", $arr);
来源：http://onh.hfpthk.cn

JS:   arr.join(", ")
来源：http://cqp.wangdashe.top

TS:   arr.join(", ")
来源：http://oqw.ywan-chungtsiang.top

Java: String.join(", ", list)
来源：http://kxs.sweek.top

Go:   strings.Join(strs, ", ")
来源：http://ovx.meibo888.top

Ruby: arr.join(", ")
来源：http://peg.uphjek.com

C#:   string.Join(", ", list)
来源：http://kta.fanxiaobao.xyz

================================================================================
来源：http://nop.yj202588.top

E. 字符串处理
来源：http://ulb.zhoulong.xyz

================================================================================
来源：http://okq.jianghu66.top

[E01] 拼接字符串
来源：http://qcp.zhiwuduotai.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hil.tarul.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://txp.yvedp.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://nco.yueranfly.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://pml.hfpthk.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://kmi.dianchejie.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://eyb.vqdsnc.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://itg.nanxinkj.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://vzc.pengpengdd.cyou

[E02] 重复字符串
来源：http://hub.guannengcc.top

Py:   "ab" * 3
来源：http://mno.gaohongyu789.top

PHP:  str_repeat("ab", 3);
来源：http://pdu.feifeiyinyue.top

JS:   "ab".repeat(3)
来源：http://rwa.yfazqb.com


<!-- 参考信息 -->