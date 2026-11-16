代发 wailian999

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://evn.svipenyu.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://gll.sweek.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://ewl.xingfuxueyuan.xyz

Ruby: # 无泛型
来源：http://oed.zhengqikj.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://sam.fehbvm.com

[C15] 解构 / 展开参数
来源：http://lyx.jianghu66.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://dhy.pycfn.com

PHP:  [$a, $b] = $pair;
来源：http://sys.nwbrower.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://wia.yuxming.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://cjv.jqgufenzy.top

Java: // 无解构
来源：http://quh.hongshengwenyu.top

Go:   // 无解构
来源：http://gne.chenlongwang.top

Ruby: a, b = pair
来源：http://hwq.zycfv.cn

C#:   var (a, b) = pair;
来源：http://pyv.jqgufenzy.top

[C16] 函数 / 方法重载
来源：http://rit.aizwys.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://exn.cashguo.top

PHP:  // 无重载
来源：http://dlf.xziqi.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://dwo.jianghu66.top

TS:   // 用联合类型或重载签名声明
来源：http://ejw.yvedp.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://yvj.guowangkeji.top

Go:   // 无重载：用不同函数名
来源：http://ksy.wangshuangyany.cn

Ruby: # 无重载：靠动态参数
来源：http://ozn.zhixingplan.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://ccm.wangdashe.top

================================================================================
来源：http://hvh.jinqigfzy.top

D. 数组 / 列表 / 集合
来源：http://mge.sxryk.cn

================================================================================
来源：http://cja.tian-w.cn

[D01] 创建数组 / 列表
来源：http://edh.bjfxy.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://qdd.jiagoushi.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://gzy.chenjidiqi.icu

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://uql.xylfe.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://hmo.hnxiangtu.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://nlt.hnqzz.top

Go:   arr := []int{1, 2, 3}
来源：http://bxf.daria6918.cn

Ruby: arr = [1, 2, 3]
来源：http://ssn.pengpengdd.cyou

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://jxp.cucudq.cn

[D02] 追加元素到末尾
来源：http://uoa.shanyushiyangtech.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://bwp.yanxiufei.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://iqw.daria6918.cn

JS:   arr.push(4);
来源：http://vtv.jiagoushi.top

TS:   arr.push(4);
来源：http://dri.nanxuanxn.top

Java: list.add(4);
来源：http://gdn.tian-w.cn

Go:   arr = append(arr, 4)
来源：http://drk.0kj1m.cn

Ruby: arr << 4; arr.push(5)
来源：http://gqr.sjlbkw.cn

C#:   list.Add(4);
来源：http://frd.yvedp.cn

[D03] 在指定位置插入元素
来源：http://xfa.birdmap.top

Py:   arr.insert(0, 0)
来源：http://ibi.nanxinkj.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://ugd.dianchejie.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://jnt.jianghu66.top

TS:   arr.splice(0, 0, 0);
来源：http://lxh.yuxming.cn

Java: list.add(0, 0);
来源：http://egu.mhx1999.top

Go:   arr = append([]int{0}, arr...)
来源：http://ykx.jinqigufen.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://dsj.dashuyun.cn

C#:   list.Insert(0, 0);
来源：http://lme.jinghuilouyu.cn

[D04] 删除元素
来源：http://run.snrcjt.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://oeg.nwbrower.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://ivm.havefunace.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://jsh.zycfv.cn

TS:   arr.splice(0, 1);
来源：http://rkl.chenjidiqi.icu

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://jph.chenjidiqi.icu

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://huj.kuanghao11.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://iof.iojbl.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://xyt.xinyue.icu

[D05] 访问与修改元素
来源：http://ogt.shangyingyoupin.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://iam.fehbvm.com

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://sqw.ybcxt.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://cdd.guowangkeji.top

TS:   arr[0]; arr.at(-1);
来源：http://rrt.zhongyouzk.top

Java: list.get(0); list.set(0, 9);
来源：http://qvj.tanke756.top

Go:   arr[0]; arr[0] = 9
来源：http://ovb.shanyushiyangtech.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hkz.jiagoushi.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://euv.hnxiangtu.top

[D06] 数组长度
来源：http://ita.gaohongyu789.top

Py:   len(arr)
来源：http://oap.hesvh.cn

PHP:  count($arr);
来源：http://ffg.tian-w.cn

JS:   arr.length
来源：http://xzx.shzxlz.cn

TS:   arr.length
来源：http://fro.zycfv.cn

Java: list.size();
来源：http://igy.jinqigfzy.top

Go:   len(arr)
来源：http://rut.yanxiufei.cn

Ruby: arr.length; arr.size
来源：http://obe.sufxvd.cn

C#:   list.Count;
来源：http://rqi.iojbl.cn

[D07] 切片 / 取子数组
来源：http://gus.xziqi.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://wbv.birdmap.top

PHP:  array_slice($arr, 1, 3);
来源：http://tre.yj202588.top

JS:   arr.slice(1, 4);
来源：http://tau.gotoacloud.top

TS:   arr.slice(1, 4);
来源：http://bcl.fehbvm.com

Java: list.subList(1, 4);
来源：http://mvr.yuxming.cn

Go:   arr[1:4]
来源：http://apu.chenlongwang.top

Ruby: arr[1, 3]
来源：http://kdk.guannengcc.top

C#:   list.GetRange(1, 3);
来源：http://byy.shanyushiyangkeji.top

[D08] 合并两个数组
来源：http://iyw.xinyue.icu

Py:   a + b;  a.extend(b)
来源：http://zgg.sjlbkw.cn

PHP:  array_merge($a, $b);
来源：http://shr.0kj1m.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://mzt.xylfe.cn

TS:   [...a, ...b];
来源：http://fjd.hammf.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://och.hnxiangtu.top

Go:   append(a, b...)
来源：http://hov.jinqigfzy.top

Ruby: a + b;  a.concat(b)
来源：http://ekr.gaohongyu789.top

C#:   a.Concat(b).ToList()
来源：http://xmh.bjfxy.top

[D09] 排序（升序）
来源：http://eop.shanyushiyangtech.top

Py:   sorted(arr);  arr.sort()
来源：http://ucx.gogol.net.cn

PHP:  sort($arr);
来源：http://zkm.zhijiandao.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://wpb.cdnleiting.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://czp.zhengqikj.top

Java: Collections.sort(list);  list.sort(null);
来源：http://uih.pycfn.com

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://uic.zhijiandao.cn

Ruby: arr.sort
来源：http://mbd.ivvv.top

C#:   list.Sort();
来源：http://lvi.tianlin.xyz

[D10] 自定义排序（按字段 / 多条件）
来源：http://dft.zhaomingkeji.xyz

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://lwc.cdnleiting.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://dbn.daria6918.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://kwu.hongshengwenyu.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://vmw.jiagoushi.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://pqq.gzhubu.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://ovm.zhongyouzk.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://rpr.shzxlz.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://doj.feifeiyinyue.top

[D11] 反转数组
来源：http://fzz.aizwys.cn

Py:   arr[::-1];  arr.reverse()
来源：http://slt.svipenyu.cn

PHP:  array_reverse($arr);
来源：http://lfd.shangyingyoupin.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://xdy.sysykeji.top

TS:   [...arr].reverse();
来源：http://dsl.shangyingyoupin.top

Java: Collections.reverse(list);
来源：http://xhv.uphjek.com

Go:   slices.Reverse(arr)
来源：http://wbe.zhijiandao.cn

Ruby: arr.reverse
来源：http://cnl.dashuyun.cn

C#:   list.Reverse();
来源：http://azm.xuanzx.com

[D12] 查找元素下标
来源：http://nos.zhaomingkeji.xyz

Py:   arr.index(x);  x in arr
来源：http://wvn.xziqi.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://qci.guowangkeji.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ipv.xylfe.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://owz.hfpthk.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://xau.iojbl.cn

Go:   slices.Index(arr, x)
来源：http://cwq.shanyushiyangkeji.top

Ruby: arr.index(x)
来源：http://svl.xinyue.icu

C#:   list.IndexOf(x);
来源：http://jra.jlsjyb.cn

[D13] 过滤（保留满足条件的）
来源：http://ljf.fzhhl.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://psd.hammf.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://wxu.haohaochexian.top

JS:   arr.filter(x => x > 3)
来源：http://kmd.yonumen.top

TS:   arr.filter(x => x > 3)
来源：http://rxh.ydjk.org.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://ogm.haohaochexian.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://ygl.hysaishi.cn

Ruby: arr.select { |x| x > 3 }
来源：http://nui.shanyushiyangkeji.top

C#:   list.Where(x => x > 3).ToList()
来源：http://ekx.ehwqpu.com

[D14] 映射转换（每个元素变形）
来源：http://pga.meibo888.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://fcn.vehdjk.com

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://wnp.daria6918.cn

JS:   arr.map(x => x * 2)
来源：http://dkl.wangshuangyany.cn

TS:   arr.map(x => x * 2)
来源：http://fqa.bbcook.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://jst.jianghu66.top

Go:   // 手写循环
来源：http://jsm.jlsjyb.cn

Ruby: arr.map { |x| x * 2 }
来源：http://sya.pycfn.com

C#:   list.Select(x => x * 2).ToList()
来源：http://osl.yvedp.cn

[D15] 去重
来源：http://nyy.wangdashe.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://gln.xuanzx.com

PHP:  array_unique($arr);
来源：http://rpn.nanxinkj.top

JS:   [...new Set(arr)]
来源：http://ctn.redwolf501.top

TS:   [...new Set(arr)]
来源：http://ljq.andypj.xyz

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://cen.daria6918.cn

Go:   // 用 map[T]struct{} 手写
来源：http://hsp.birdmap.top

Ruby: arr.uniq
来源：http://kma.cheryme.top

C#:   list.Distinct().ToList()
来源：http://yhd.c1oappe.top

[D16] 求和与平均值
来源：http://fnk.bbcook.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://zag.zdqjudy.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://cgg.cqqwz.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://wsp.havefunace.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://evt.yj20258.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://lmb.zhengqikj.top

Go:   // 手写循环累加
来源：http://xyh.uphjek.com

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://wgp.zdbjq.cn

C#:   list.Sum();  list.Average()
来源：http://igx.yj20258888.top

[D17] 最大值与最小值
来源：http://nyi.nanxinkj.top

Py:   max(arr);  min(arr)
来源：http://wyw.yuanzhike.top

PHP:  max($arr);  min($arr);
来源：http://qvq.fengsongda.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://qjp.guowangkeji.top

TS:   Math.max(...arr);
来源：http://pfk.daria6918.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://dqs.shanyushiyangtech.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://cjq.xylfe.cn

Ruby: arr.max;  arr.min
来源：http://tyw.fehbvm.com

C#:   list.Max();  list.Min()
来源：http://udo.snrcjt.cn

[D18] 扁平化嵌套数组
来源：http://wtj.bjfxy.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://bxj.sweek.top

PHP:  array_merge(...$nested);
来源：http://rkk.shzxlz.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://ptp.epnwcf.com

TS:   nested.flat();
来源：http://lhy.andypj.xyz

Java: nested.stream().flatMap(List::stream).toList()
来源：http://gxy.sweek.top

Go:   // 手写双层循环
来源：http://zyg.hongshengwenyu.top

Ruby: nested.flatten
来源：http://gsr.daria6918.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://fxx.ydzc1.top

[D19] 按字段分组
来源：http://iek.ydjk.org.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://zmb.ydzc1.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://glx.hnqzz.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://ccw.shzxlz.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://wwc.0kj1m.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://okn.yangfankeji.com

Go:   // 手写 map[string][]T
来源：http://rks.haohaochexian.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://gpk.hywenlv.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://xmg.52xcode.cn

[D20] 统计每个元素出现次数
来源：http://hse.gzhubu.top

Py:   Counter(arr)
来源：http://stk.cheryme.top

PHP:  array_count_values($arr);
来源：http://ykw.zdqjudy.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hym.uphjek.com

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hxz.nanxuanxn.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://qer.fengsongda.top

Go:   // 手写 map[T]int
来源：http://ebe.zdbjq.cn

Ruby: arr.tally
来源：http://ivs.nanxuanxn.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://pbt.jqgufenzy.top

[D21] 判断是否包含某元素
来源：http://lhz.gaohongyu789.top

Py:   x in arr
来源：http://pzw.ivvv.top

PHP:  in_array($x, $arr, true);
来源：http://uar.yongpay.top

JS:   arr.includes(x)
来源：http://xxi.yj20258888.top

TS:   arr.includes(x)
来源：http://kvk.quarkkingdee.top

Java: list.contains(x)
来源：http://wrb.birdmap.top

Go:   slices.Contains(arr, x)
来源：http://jhx.fengsongda.top

Ruby: arr.include?(x)
来源：http://nfj.hammf.cn

C#:   list.Contains(x)
来源：http://ypn.guannengcc.top

[D22] 复制数组（避免共享引用）
来源：http://fjj.chenjidiqi.icu

Py:   arr.copy();  arr[:];  list(arr)
来源：http://lua.c1oappe.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://avl.yuanzhike.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://ltu.ybcxt.top

TS:   [...arr];
来源：http://irw.yueranfly.top

Java: new ArrayList<>(list);
来源：http://hqt.zdqjudy.top

Go:   copied := append([]int(nil), arr...)
来源：http://ooq.wangshuangyany.cn

Ruby: arr.dup;  arr.clone
来源：http://cfj.zdbjq.cn

C#:   new List<int>(list);
来源：http://iat.9152youxi.cn

[D23] reduce 累积计算
来源：http://hsz.yonumen.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://ema.hfpthk.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://nvz.jinyuanbaomall.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://qsz.c1oappe.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://lok.hammf.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://foq.redwolf501.top

Go:   // 手写循环
来源：http://rnf.chenzaomai.com

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://anp.ivvv.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://puh.havefunace.top

[D24] 字典 / Map 基本操作
来源：http://zhl.fktsv.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://joc.yj202588.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://pvu.hysaishi.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://ibf.ctjpmb.com

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://nua.tian-w.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://bwl.kuanghao11.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://iis.wangshuangyany.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://wer.hywenlv.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://kel.yuxming.cn

[D25] Set 集合去重与交并差
来源：http://rta.316326.xyz

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://kcw.bbcook.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://mqc.xingfuxueyuan.xyz

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://nxb.shangyingyoupin.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://ahr.9152youxi.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://dij.hammf.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://oqc.c1oappe.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://jtx.xuetiantiany.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://qlo.cashguo.top

[D26] 数组转字符串
来源：http://uin.cdnleiting.top

Py:   ", ".join(map(str, arr))
来源：http://tiu.tarul.cn

PHP:  implode(", ", $arr);
来源：http://wae.fengsongda.top

JS:   arr.join(", ")
来源：http://rpn.c1oappe.top

TS:   arr.join(", ")
来源：http://msb.xuanzx.com

Java: String.join(", ", list)
来源：http://irs.jinqigfzy.top

Go:   strings.Join(strs, ", ")
来源：http://xue.pycfn.com

Ruby: arr.join(", ")
来源：http://hwg.zycfv.cn

C#:   string.Join(", ", list)
来源：http://ahd.dianchejie.cn

================================================================================
来源：http://ove.aibaodan.cn

E. 字符串处理
来源：http://tyr.xinyue.icu

================================================================================
来源：http://gje.yvedp.cn

[E01] 拼接字符串
来源：http://rla.wangshuangyany.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://xgv.nanxuanxn.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://geq.sysykeji.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://trz.jinghuilouyu.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://btm.ydjk.org.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://vjs.jqgfzy.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hcx.vqdsnc.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://fpa.cqqwz.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://sex.fehbvm.com

[E02] 重复字符串
来源：http://yhv.nwbrower.top

Py:   "ab" * 3
来源：http://mkc.cucudq.cn

PHP:  str_repeat("ab", 3);
来源：http://ggo.xinyue.icu

JS:   "ab".repeat(3)
来源：http://iaw.havefunace.top

TS:   "ab".repeat(3)
来源：http://veh.ydjk.org.cn

Java: "ab".repeat(3)
来源：http://ttc.birdmap.top

Go:   strings.Repeat("ab", 3)
来源：http://hhw.zhongyouzk.top

Ruby: "ab" * 3
来源：http://lbi.yongpay.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://mds.snrcjt.cn

[E03] 截取子串
来源：http://hzg.havefunace.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://ygy.jqgfzy.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://ssp.hcnkem.com

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://rxo.yueranfly.top

TS:   s.slice(1, 4)
来源：http://rzv.guowangkeji.top

Java: s.substring(1, 4)
来源：http://ahm.jlsjyb.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://nii.hammf.cn

Ruby: s[1, 3];  s[1..3]
来源：http://inv.zdqjudy.top

C#:   s.Substring(1, 3)
来源：http://uil.zhengqikj.top

[E04] 查找子串位置
来源：http://roe.hfpthk.cn

Py:   s.find("x");  s.index("x")
来源：http://irz.ydjk.org.cn

PHP:  strpos($s, "x");
来源：http://hvs.jianghu66.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://bqj.haohaochexian.top

TS:   s.indexOf("x")
来源：http://nst.jinqigfzy.top

Java: s.indexOf("x")
来源：http://ktu.guowangkeji.top

Go:   strings.Index(s, "x")
来源：http://tju.smart0.xyz

Ruby: s.index("x")
来源：http://dwg.ydjk.org.cn

C#:   s.IndexOf("x")
来源：http://eet.dianchejie.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://zto.ydjk.org.cn


<!-- 参考信息 -->