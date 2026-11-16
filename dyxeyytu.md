代发 wailian999

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://eck.iojbl.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://poi.52xcode.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://lgy.hfpthk.cn

Ruby: # 无泛型
来源：http://uya.redwolf501.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://qqo.yvedp.cn

[C15] 解构 / 展开参数
来源：http://jsc.fengsongda.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://app.iojbl.cn

PHP:  [$a, $b] = $pair;
来源：http://dtt.daxiang520.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://jnr.yj20258888.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://cri.iojbl.cn

Java: // 无解构
来源：http://ddo.shanyushiyangkeji.top

Go:   // 无解构
来源：http://aqb.ybcxt.top

Ruby: a, b = pair
来源：http://boy.birdmap.top

C#:   var (a, b) = pair;
来源：http://gag.yfazqb.com

[C16] 函数 / 方法重载
来源：http://qbv.jinqigfzy.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://rqm.cashguo.top

PHP:  // 无重载
来源：http://umm.zhaomingkeji.xyz

JS:   // 无重载：靠 arguments.length 分支
来源：http://jgh.tianlin.xyz

TS:   // 用联合类型或重载签名声明
来源：http://xxa.fzhhl.top

Java: void f(int a) {}  void f(String a) {}
来源：http://jlv.andypj.xyz

Go:   // 无重载：用不同函数名
来源：http://vxp.mhx1999.top

Ruby: # 无重载：靠动态参数
来源：http://nny.zhijiandao.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://rrd.epnwcf.com

================================================================================
来源：http://gog.yongpay.top

D. 数组 / 列表 / 集合
来源：http://ctu.yongpay.top

================================================================================
来源：http://xip.zhengqikj.top

[D01] 创建数组 / 列表
来源：http://xiv.fktsv.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://znz.epnwcf.com

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://nld.shanyushiyangtech.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://ciz.jiagoushi.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://ioq.cheryme.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://ptp.bjfxy.top

Go:   arr := []int{1, 2, 3}
来源：http://zkl.fengsongda.top

Ruby: arr = [1, 2, 3]
来源：http://wdw.fehbvm.com

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://zza.shangyingyoupin.top

[D02] 追加元素到末尾
来源：http://omq.yvedp.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://lac.xinyue.icu

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://tgg.dashuyun.cn

JS:   arr.push(4);
来源：http://hxu.yj20258.top

TS:   arr.push(4);
来源：http://skq.jinqigufen.top

Java: list.add(4);
来源：http://udm.xylfe.cn

Go:   arr = append(arr, 4)
来源：http://vun.mhx1999.top

Ruby: arr << 4; arr.push(5)
来源：http://abq.zhaomingkeji.xyz

C#:   list.Add(4);
来源：http://fsd.shanyushiyangtech.top

[D03] 在指定位置插入元素
来源：http://toa.andypj.xyz

Py:   arr.insert(0, 0)
来源：http://mkw.xingfuxueyuan.xyz

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://pkv.zhixingplan.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://bej.aibaodan.cn

TS:   arr.splice(0, 0, 0);
来源：http://mfc.xinyue.icu

Java: list.add(0, 0);
来源：http://aho.daxiang520.top

Go:   arr = append([]int{0}, arr...)
来源：http://khw.dianchejie.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://mbt.jlsjyb.cn

C#:   list.Insert(0, 0);
来源：http://nio.sjlbkw.cn

[D04] 删除元素
来源：http://feg.vehdjk.com

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://zvp.cheryme.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://ild.smart0.xyz

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://naw.vehdjk.com

TS:   arr.splice(0, 1);
来源：http://ryf.aibaodan.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://ttc.cheryme.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://eme.daria6918.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://ipk.jinqigfzy.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://xtw.vehdjk.com

[D05] 访问与修改元素
来源：http://pum.tian-w.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://jtu.tianlin.xyz

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://jbz.tarul.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://xhu.xziqi.cn

TS:   arr[0]; arr.at(-1);
来源：http://env.smart0.xyz

Java: list.get(0); list.set(0, 9);
来源：http://ggs.chenjidiqi.icu

Go:   arr[0]; arr[0] = 9
来源：http://wrj.zhijiandao.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://jky.fehbvm.com

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://yqd.hysaishi.cn

[D06] 数组长度
来源：http://abs.zhongyouzk.top

Py:   len(arr)
来源：http://ymc.zycfv.cn

PHP:  count($arr);
来源：http://gee.fzhhl.top

JS:   arr.length
来源：http://akr.hnxiangtu.top

TS:   arr.length
来源：http://kqj.birdmap.top

Java: list.size();
来源：http://pdj.chenzaomai.com

Go:   len(arr)
来源：http://vrt.gzhubu.top

Ruby: arr.length; arr.size
来源：http://xpp.xinyue.icu

C#:   list.Count;
来源：http://nme.fanxiaobao.xyz

[D07] 切片 / 取子数组
来源：http://rfn.jinqigufen.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://tsa.sweek.top

PHP:  array_slice($arr, 1, 3);
来源：http://seq.quarkkingdee.top

JS:   arr.slice(1, 4);
来源：http://fny.xylfe.cn

TS:   arr.slice(1, 4);
来源：http://cmv.smart0.xyz

Java: list.subList(1, 4);
来源：http://jqe.ydzc1.top

Go:   arr[1:4]
来源：http://sgl.yongpay.top

Ruby: arr[1, 3]
来源：http://xbt.xinyue.icu

C#:   list.GetRange(1, 3);
来源：http://kca.cucudq.cn

[D08] 合并两个数组
来源：http://hzv.wangshuangyany.cn

Py:   a + b;  a.extend(b)
来源：http://vrg.cucudq.cn

PHP:  array_merge($a, $b);
来源：http://ffd.hesvh.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://eih.fzhhl.top

TS:   [...a, ...b];
来源：http://xzk.sysykeji.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://czs.yangfankeji.com

Go:   append(a, b...)
来源：http://npk.ydjk.org.cn

Ruby: a + b;  a.concat(b)
来源：http://vmv.iojbl.cn

C#:   a.Concat(b).ToList()
来源：http://hmt.aibaodan.cn

[D09] 排序（升序）
来源：http://ahq.gaohongyu789.top

Py:   sorted(arr);  arr.sort()
来源：http://eii.yfazqb.com

PHP:  sort($arr);
来源：http://nza.yuxming.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://wvh.wangshuangyany.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://oqu.nanxuanxn.top

Java: Collections.sort(list);  list.sort(null);
来源：http://zpt.xziqi.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://ian.pengpengdd.cyou

Ruby: arr.sort
来源：http://jmq.bbcook.cn

C#:   list.Sort();
来源：http://uzh.gzhubu.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://zxp.cdnleiting.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://bsf.aizwys.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wwz.jqgfzy.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://tlk.fengsongda.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://kqn.bbcook.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://jxf.ydzc1.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://ent.tanke756.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://fpq.cashguo.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://flx.zhengqikj.top

[D11] 反转数组
来源：http://hku.jlsjyb.cn

Py:   arr[::-1];  arr.reverse()
来源：http://cay.vehdjk.com

PHP:  array_reverse($arr);
来源：http://wot.yueranfly.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://nxv.shzxlz.cn

TS:   [...arr].reverse();
来源：http://qva.9152youxi.cn

Java: Collections.reverse(list);
来源：http://zsk.redwolf501.top

Go:   slices.Reverse(arr)
来源：http://dkg.tanke756.top

Ruby: arr.reverse
来源：http://dsb.jiagoushi.top

C#:   list.Reverse();
来源：http://rje.cheryme.top

[D12] 查找元素下标
来源：http://ntm.daxiang520.top

Py:   arr.index(x);  x in arr
来源：http://bea.hfpthk.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://zwa.xingfuxueyuan.xyz

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://bgy.ppjwa.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://rsj.hysaishi.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://giz.bjfxy.top

Go:   slices.Index(arr, x)
来源：http://yoi.haohaochexian.top

Ruby: arr.index(x)
来源：http://fhv.yvedp.cn

C#:   list.IndexOf(x);
来源：http://jcy.aibaodan.cn

[D13] 过滤（保留满足条件的）
来源：http://faj.haohaochexian.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://ifa.jyoumei.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://iqe.xziqi.cn

JS:   arr.filter(x => x > 3)
来源：http://qic.pengpengdd.cyou

TS:   arr.filter(x => x > 3)
来源：http://rja.pengpengdd.cyou

Java: list.stream().filter(x -> x > 3).toList()
来源：http://bop.svipenyu.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://nsy.tian-w.cn

Ruby: arr.select { |x| x > 3 }
来源：http://duk.zhoulong.xyz

C#:   list.Where(x => x > 3).ToList()
来源：http://tor.0kj1m.cn

[D14] 映射转换（每个元素变形）
来源：http://lsg.nanxuanxn.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://ljx.xinyue.icu

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://uyf.fzhhl.top

JS:   arr.map(x => x * 2)
来源：http://bvs.chenjidiqi.icu

TS:   arr.map(x => x * 2)
来源：http://xlo.guannengcc.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://qcz.shzxlz.cn

Go:   // 手写循环
来源：http://cfo.hongshengwenyu.top

Ruby: arr.map { |x| x * 2 }
来源：http://wzh.yvedp.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://lzb.fktsv.cn

[D15] 去重
来源：http://jrh.dianchejie.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://did.hysaishi.cn

PHP:  array_unique($arr);
来源：http://izq.yvedp.cn

JS:   [...new Set(arr)]
来源：http://tqb.xuetiantiany.cn

TS:   [...new Set(arr)]
来源：http://fla.mhx1999.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://woc.gaohongyu789.top

Go:   // 用 map[T]struct{} 手写
来源：http://wcm.0kj1m.cn

Ruby: arr.uniq
来源：http://dtz.jinqigfzy.top

C#:   list.Distinct().ToList()
来源：http://uqm.jinghuilouyu.cn

[D16] 求和与平均值
来源：http://wzz.xylfe.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://zxj.9152youxi.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hiv.vqdsnc.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://zdq.yj202588.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://zto.tianlin.xyz

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://exe.snrcjt.cn

Go:   // 手写循环累加
来源：http://cav.cashguo.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://zlg.zdbjq.cn

C#:   list.Sum();  list.Average()
来源：http://ntt.tanke756.top

[D17] 最大值与最小值
来源：http://vri.pengpengdd.cyou

Py:   max(arr);  min(arr)
来源：http://bpr.wangdashe.top

PHP:  max($arr);  min($arr);
来源：http://src.smart0.xyz

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://vwp.feifeiyinyue.top

TS:   Math.max(...arr);
来源：http://wpx.jqgufenzy.top

Java: Collections.max(list);  Collections.min(list);
来源：http://fiv.yongpay.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://jps.guowangkeji.top

Ruby: arr.max;  arr.min
来源：http://brd.daxiang520.top

C#:   list.Max();  list.Min()
来源：http://veq.aibaodan.cn

[D18] 扁平化嵌套数组
来源：http://xcu.yfazqb.com

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://fji.havefunace.top

PHP:  array_merge(...$nested);
来源：http://xav.shanyushiyangkeji.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://yyp.zdqjudy.top

TS:   nested.flat();
来源：http://thk.52xcode.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://dpj.zycfv.cn

Go:   // 手写双层循环
来源：http://lnh.pengpengdd.cyou

Ruby: nested.flatten
来源：http://efj.smart0.xyz

C#:   nested.SelectMany(x => x).ToList()
来源：http://bff.shanyushiyangtech.top

[D19] 按字段分组
来源：http://uda.nanxinkj.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://cwv.epnwcf.com

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://tgp.shangyingyoupin.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://tfk.haohaochexian.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://tdg.sweek.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://ndc.mhx1999.top

Go:   // 手写 map[string][]T
来源：http://jck.chenzaomai.com

Ruby: arr.group_by { |x| x[:type] }
来源：http://ihg.jyoumei.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hbu.shzxlz.cn

[D20] 统计每个元素出现次数
来源：http://btk.shanyushiyangkeji.top

Py:   Counter(arr)
来源：http://lsw.yuanzhike.top

PHP:  array_count_values($arr);
来源：http://mhx.zycfv.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://nfa.sysykeji.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://htj.ctjpmb.com

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://eae.zhixingplan.top

Go:   // 手写 map[T]int
来源：http://jqa.wangshuangyany.cn

Ruby: arr.tally
来源：http://vua.pycfn.com

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://srw.zhengqikj.top

[D21] 判断是否包含某元素
来源：http://jit.bbcook.cn

Py:   x in arr
来源：http://gfr.andypj.xyz

PHP:  in_array($x, $arr, true);
来源：http://zop.zhiwuduotai.top

JS:   arr.includes(x)
来源：http://ifj.xingfuxueyuan.xyz

TS:   arr.includes(x)
来源：http://rpu.sjlbkw.cn

Java: list.contains(x)
来源：http://dcu.yonumen.top

Go:   slices.Contains(arr, x)
来源：http://abf.hfpthk.cn

Ruby: arr.include?(x)
来源：http://rsa.jlsjyb.cn

C#:   list.Contains(x)
来源：http://kqu.yuanzhike.top

[D22] 复制数组（避免共享引用）
来源：http://qof.gzhubu.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://vhx.hongshengwenyu.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://qcf.jqgfzy.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://mpa.ppjwa.cn

TS:   [...arr];
来源：http://exc.hywenlv.cn

Java: new ArrayList<>(list);
来源：http://hju.xziqi.cn

Go:   copied := append([]int(nil), arr...)
来源：http://xmn.tarul.cn

Ruby: arr.dup;  arr.clone
来源：http://cot.zdbjq.cn

C#:   new List<int>(list);
来源：http://iwd.gotoacloud.top

[D23] reduce 累积计算
来源：http://uat.fktsv.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://zle.dianchejie.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://oww.zhijiandao.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://qiq.nwbrower.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://vtd.haohaochexian.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://shj.fanxiaobao.xyz

Go:   // 手写循环
来源：http://tns.andypj.xyz

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://sak.zhoulong.xyz

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://uzn.nwbrower.top

[D24] 字典 / Map 基本操作
来源：http://ykc.mhx1999.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://vgi.sufxvd.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://dpy.yonumen.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://ssb.jlsjyb.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://yjc.cheryme.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://urn.sjlbkw.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://snt.zhixingplan.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://xze.jqgufenzy.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://ssm.nwbrower.top

[D25] Set 集合去重与交并差
来源：http://flu.cdnleiting.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://ohr.zdbjq.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://wpr.bjfxy.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://irg.epnwcf.com

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://rik.xuanzx.com

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://tkz.guannengcc.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://itz.hongshengwenyu.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://mbd.jqgfzy.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://otr.ywan-chungtsiang.top

[D26] 数组转字符串
来源：http://cwq.havefunace.top

Py:   ", ".join(map(str, arr))
来源：http://fry.daxiang520.top

PHP:  implode(", ", $arr);
来源：http://iyd.nwbrower.top

JS:   arr.join(", ")
来源：http://qkc.jqgufenzy.top

TS:   arr.join(", ")
来源：http://ddg.sweek.top

Java: String.join(", ", list)
来源：http://axo.cucudq.cn

Go:   strings.Join(strs, ", ")
来源：http://uoo.uphjek.com

Ruby: arr.join(", ")
来源：http://sgi.fanxiaobao.xyz

C#:   string.Join(", ", list)
来源：http://ucy.cucudq.cn

================================================================================
来源：http://jdv.yuanzhike.top

E. 字符串处理
来源：http://ydk.hysaishi.cn

================================================================================
来源：http://utu.vqdsnc.cn

[E01] 拼接字符串
来源：http://qgs.jianghu66.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://qvi.iojbl.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://lzo.xingfuxueyuan.xyz

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://kmn.ydzc1.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://iij.meibo888.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://yzc.0kj1m.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://jfw.xylfe.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://adn.jqgfzy.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://apl.mhx1999.top

[E02] 重复字符串
来源：http://ndw.tanke756.top

Py:   "ab" * 3
来源：http://xim.gotoacloud.top

PHP:  str_repeat("ab", 3);
来源：http://pqc.guannengcc.top

JS:   "ab".repeat(3)
来源：http://bgh.jinyuanbaomall.cn

TS:   "ab".repeat(3)
来源：http://iob.xuanzx.com

Java: "ab".repeat(3)
来源：http://jau.ppjwa.cn

Go:   strings.Repeat("ab", 3)
来源：http://rsd.sxryk.cn

Ruby: "ab" * 3
来源：http://tpb.shanyushiyangkeji.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://axu.quarkkingdee.top

[E03] 截取子串
来源：http://kpg.zhijiandao.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://tjl.ivvv.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://ztn.zhoulong.xyz

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://fgb.shanyushiyangtech.top

TS:   s.slice(1, 4)
来源：http://mnw.zdbjq.cn

Java: s.substring(1, 4)
来源：http://jwa.cdnleiting.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://oxo.yvedp.cn

Ruby: s[1, 3];  s[1..3]
来源：http://anw.redwolf501.top

C#:   s.Substring(1, 3)
来源：http://hse.gotoacloud.top

[E04] 查找子串位置
来源：http://xnc.daxiang520.top

Py:   s.find("x");  s.index("x")
来源：http://geg.xinyue.icu

PHP:  strpos($s, "x");
来源：http://mro.daxiang520.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://obf.uphjek.com

TS:   s.indexOf("x")
来源：http://igc.zhongyouzk.top

Java: s.indexOf("x")
来源：http://ngt.yonumen.top

Go:   strings.Index(s, "x")
来源：http://lxg.yueranfly.top

Ruby: s.index("x")
来源：http://lyw.dianchejie.cn

C#:   s.IndexOf("x")
来源：http://arm.ehwqpu.com

[E05] 判断包含 / 前缀 / 后缀
来源：http://zol.gzhubu.top


<!-- 参考信息 -->