代发 wailian999

C#:   static T First<T>(List<T> items) => items[0];
来源：http://zby.fktsv.cn

[C15] 解构 / 展开参数
来源：http://kpy.snrcjt.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://yli.nwbrower.top

PHP:  [$a, $b] = $pair;
来源：http://lsy.zhongyouzk.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://kgm.kuanghao11.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://sln.ydzc1.top

Java: // 无解构
来源：http://kjw.aibaodan.cn

Go:   // 无解构
来源：http://jjw.gzhubu.top

Ruby: a, b = pair
来源：http://azo.jinyuanbaomall.cn

C#:   var (a, b) = pair;
来源：http://whp.jinghuilouyu.cn

[C16] 函数 / 方法重载
来源：http://ysw.jinqigfzy.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://pux.redwolf501.top

PHP:  // 无重载
来源：http://owz.ybcxt.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://qys.iojbl.cn

TS:   // 用联合类型或重载签名声明
来源：http://xjm.shzxlz.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://heh.fanxiaobao.xyz

Go:   // 无重载：用不同函数名
来源：http://apt.vehdjk.com

Ruby: # 无重载：靠动态参数
来源：http://oev.jqgfzy.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://lny.sxryk.cn

================================================================================
来源：http://tfo.cdnleiting.top

D. 数组 / 列表 / 集合
来源：http://qvl.hfpthk.cn

================================================================================
来源：http://hgc.tianlin.xyz

[D01] 创建数组 / 列表
来源：http://afy.redwolf501.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://dvg.jyoumei.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://qds.yueranfly.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://mnv.hesvh.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://gpn.shanyushiyangtech.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://acx.xinyue.icu

Go:   arr := []int{1, 2, 3}
来源：http://slg.nwbrower.top

Ruby: arr = [1, 2, 3]
来源：http://sts.uphjek.com

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://qno.xingfuxueyuan.xyz

[D02] 追加元素到末尾
来源：http://xps.shuidangran.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://cvx.cashguo.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://tzu.zhoulong.xyz

JS:   arr.push(4);
来源：http://pua.quarkkingdee.top

TS:   arr.push(4);
来源：http://lwf.ppjwa.cn

Java: list.add(4);
来源：http://vrt.xuetiantiany.cn

Go:   arr = append(arr, 4)
来源：http://vmp.sufxvd.cn

Ruby: arr << 4; arr.push(5)
来源：http://szo.kuanghao11.cn

C#:   list.Add(4);
来源：http://cyg.daria6918.cn

[D03] 在指定位置插入元素
来源：http://yln.shuidangran.top

Py:   arr.insert(0, 0)
来源：http://why.jinyuanbaomall.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://ndd.zhijiandao.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hxi.shzxlz.cn

TS:   arr.splice(0, 0, 0);
来源：http://ypq.guannengcc.top

Java: list.add(0, 0);
来源：http://zoc.gotoacloud.top

Go:   arr = append([]int{0}, arr...)
来源：http://hit.fehbvm.com

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://unl.pycfn.com

C#:   list.Insert(0, 0);
来源：http://zvr.sweek.top

[D04] 删除元素
来源：http://rzz.pycfn.com

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://eqc.uphjek.com

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hrf.xuetiantiany.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://peb.hammf.cn

TS:   arr.splice(0, 1);
来源：http://vkd.tianlin.xyz

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://kfd.9152youxi.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://ydk.nanxinkj.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://fgg.ydjk.org.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://uqa.fanxiaobao.xyz

[D05] 访问与修改元素
来源：http://xso.hongshengwenyu.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://bcs.yuxming.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://pgo.zhiwuduotai.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://izy.iojbl.cn

TS:   arr[0]; arr.at(-1);
来源：http://oyf.hesvh.cn

Java: list.get(0); list.set(0, 9);
来源：http://evv.gogol.net.cn

Go:   arr[0]; arr[0] = 9
来源：http://lfy.daria6918.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://mcv.yanxiufei.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://kae.chenjidiqi.icu

[D06] 数组长度
来源：http://vhy.cucudq.cn

Py:   len(arr)
来源：http://uax.cdnleiting.top

PHP:  count($arr);
来源：http://wpl.hywenlv.cn

JS:   arr.length
来源：http://vqc.ybcxt.top

TS:   arr.length
来源：http://jki.uphjek.com

Java: list.size();
来源：http://kbc.chenjidiqi.icu

Go:   len(arr)
来源：http://tsf.sweek.top

Ruby: arr.length; arr.size
来源：http://tqh.nanxuanxn.top

C#:   list.Count;
来源：http://vvm.pycfn.com

[D07] 切片 / 取子数组
来源：http://vea.yonumen.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://kbe.birdmap.top

PHP:  array_slice($arr, 1, 3);
来源：http://wsi.52xcode.cn

JS:   arr.slice(1, 4);
来源：http://nss.hongshengwenyu.top

TS:   arr.slice(1, 4);
来源：http://ikj.sjlbkw.cn

Java: list.subList(1, 4);
来源：http://gri.hcnkem.com

Go:   arr[1:4]
来源：http://mor.ydjk.org.cn

Ruby: arr[1, 3]
来源：http://twd.jinqigufen.top

C#:   list.GetRange(1, 3);
来源：http://gwq.gogol.net.cn

[D08] 合并两个数组
来源：http://zvg.zhixingplan.top

Py:   a + b;  a.extend(b)
来源：http://zqv.hfpthk.cn

PHP:  array_merge($a, $b);
来源：http://jyu.andypj.xyz

JS:   [...a, ...b];  a.concat(b);
来源：http://yvr.zhaomingkeji.xyz

TS:   [...a, ...b];
来源：http://pke.nanxuanxn.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://csn.shanyushiyangtech.top

Go:   append(a, b...)
来源：http://yac.iojbl.cn

Ruby: a + b;  a.concat(b)
来源：http://hvg.guannengcc.top

C#:   a.Concat(b).ToList()
来源：http://xdr.aizwys.cn

[D09] 排序（升序）
来源：http://nls.hcnkem.com

Py:   sorted(arr);  arr.sort()
来源：http://mxb.pycfn.com

PHP:  sort($arr);
来源：http://hmn.gogol.net.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://mpu.gaohongyu789.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://vjh.xziqi.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://irj.shanyushiyangkeji.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://czr.jinyuanbaomall.cn

Ruby: arr.sort
来源：http://gwz.daria6918.cn

C#:   list.Sort();
来源：http://scg.aibaodan.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://wlm.sweek.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://rdf.xuanzx.com

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://kle.aibaodan.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://nwi.gzhubu.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://yqf.ppjwa.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://pfg.fktsv.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://rvm.smart0.xyz

Ruby: arr.sort_by { |x| x[:age] }
来源：http://qyh.yj20258.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://adt.daria6918.cn

[D11] 反转数组
来源：http://gvq.cdnleiting.top

Py:   arr[::-1];  arr.reverse()
来源：http://olh.yj202588.top

PHP:  array_reverse($arr);
来源：http://hro.redwolf501.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://kyv.shuidangran.top

TS:   [...arr].reverse();
来源：http://cgg.52xcode.cn

Java: Collections.reverse(list);
来源：http://yhc.yvedp.cn

Go:   slices.Reverse(arr)
来源：http://bgv.epnwcf.com

Ruby: arr.reverse
来源：http://nev.wangdashe.top

C#:   list.Reverse();
来源：http://vuy.gogol.net.cn

[D12] 查找元素下标
来源：http://ygd.hammf.cn

Py:   arr.index(x);  x in arr
来源：http://ohx.sjlbkw.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://wxy.ppjwa.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://cxo.guowangkeji.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://eta.daxiang520.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://jzb.shanyushiyangkeji.top

Go:   slices.Index(arr, x)
来源：http://yen.9152youxi.cn

Ruby: arr.index(x)
来源：http://gqx.shanyushiyangtech.top

C#:   list.IndexOf(x);
来源：http://fkw.tanke756.top

[D13] 过滤（保留满足条件的）
来源：http://ahl.jinqigfzy.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://wxa.sjlbkw.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://nrm.sufxvd.cn

JS:   arr.filter(x => x > 3)
来源：http://xwc.wangshuangyany.cn

TS:   arr.filter(x => x > 3)
来源：http://krr.hnxiangtu.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://iqy.zhongyouzk.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://fop.jqgufenzy.top

Ruby: arr.select { |x| x > 3 }
来源：http://klz.haohaochexian.top

C#:   list.Where(x => x > 3).ToList()
来源：http://vmt.hesvh.cn

[D14] 映射转换（每个元素变形）
来源：http://ial.sjlbkw.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://tgq.hfpthk.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://juf.zhaomingkeji.xyz

JS:   arr.map(x => x * 2)
来源：http://ajw.tanke756.top

TS:   arr.map(x => x * 2)
来源：http://dzp.hcnkem.com

Java: list.stream().map(x -> x * 2).toList()
来源：http://air.yongpay.top

Go:   // 手写循环
来源：http://zwn.xuanzx.com

Ruby: arr.map { |x| x * 2 }
来源：http://uld.fehbvm.com

C#:   list.Select(x => x * 2).ToList()
来源：http://oqs.yj20258888.top

[D15] 去重
来源：http://ftw.tarul.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://iol.yj20258888.top

PHP:  array_unique($arr);
来源：http://jsu.fzhhl.top

JS:   [...new Set(arr)]
来源：http://iaw.zhoulong.xyz

TS:   [...new Set(arr)]
来源：http://pxs.yangfankeji.com

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://emu.9152youxi.cn

Go:   // 用 map[T]struct{} 手写
来源：http://paj.yvedp.cn

Ruby: arr.uniq
来源：http://pll.havefunace.top

C#:   list.Distinct().ToList()
来源：http://pah.jyoumei.cn

[D16] 求和与平均值
来源：http://zmm.jiagoushi.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://nrt.fktsv.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://ona.sysykeji.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://nfb.kuanghao11.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://sau.jinyuanbaomall.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://oge.sxryk.cn

Go:   // 手写循环累加
来源：http://fil.gaohongyu789.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://wcm.guannengcc.top

C#:   list.Sum();  list.Average()
来源：http://iut.jinghuilouyu.cn

[D17] 最大值与最小值
来源：http://ucc.yangfankeji.com

Py:   max(arr);  min(arr)
来源：http://rbg.9152youxi.cn

PHP:  max($arr);  min($arr);
来源：http://aic.zhoulong.xyz

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://xam.xinyue.icu

TS:   Math.max(...arr);
来源：http://ggs.iojbl.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://ytg.jinqigfzy.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://wlm.wangdashe.top

Ruby: arr.max;  arr.min
来源：http://jem.chenlongwang.top

C#:   list.Max();  list.Min()
来源：http://lsm.fzhhl.top

[D18] 扁平化嵌套数组
来源：http://ira.yonumen.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://see.birdmap.top

PHP:  array_merge(...$nested);
来源：http://ncs.cqqwz.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hfr.xuanzx.com

TS:   nested.flat();
来源：http://neo.jqgufenzy.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://ffv.zhoulong.xyz

Go:   // 手写双层循环
来源：http://doz.jinghuilouyu.cn

Ruby: nested.flatten
来源：http://twj.epnwcf.com

C#:   nested.SelectMany(x => x).ToList()
来源：http://udk.hesvh.cn

[D19] 按字段分组
来源：http://yyt.cdnleiting.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://qdl.yfazqb.com

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://bgv.zhaomingkeji.xyz

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://qsp.xylfe.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://uuy.jqgufenzy.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://koy.jinqigfzy.top

Go:   // 手写 map[string][]T
来源：http://git.ppjwa.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://bzf.zhengqikj.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://xqx.dashuyun.cn

[D20] 统计每个元素出现次数
来源：http://nvg.zhoulong.xyz

Py:   Counter(arr)
来源：http://itp.aizwys.cn

PHP:  array_count_values($arr);
来源：http://jmn.9152youxi.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://khp.chenzaomai.com

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://dak.cheryme.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://zay.shangyingyoupin.top

Go:   // 手写 map[T]int
来源：http://air.yj20258.top

Ruby: arr.tally
来源：http://jvz.yongpay.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://gqp.aibaodan.cn

[D21] 判断是否包含某元素
来源：http://vng.sjlbkw.cn

Py:   x in arr
来源：http://tnn.shanyushiyangkeji.top

PHP:  in_array($x, $arr, true);
来源：http://mbk.zhixingplan.top

JS:   arr.includes(x)
来源：http://luc.nanxuanxn.top

TS:   arr.includes(x)
来源：http://xah.0kj1m.cn

Java: list.contains(x)
来源：http://axp.zhijiandao.cn

Go:   slices.Contains(arr, x)
来源：http://jhy.ybcxt.top

Ruby: arr.include?(x)
来源：http://lww.fanxiaobao.xyz

C#:   list.Contains(x)
来源：http://ejs.nanxuanxn.top

[D22] 复制数组（避免共享引用）
来源：http://ivx.ctjpmb.com

Py:   arr.copy();  arr[:];  list(arr)
来源：http://bfy.sxryk.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://obr.havefunace.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://bxs.cheryme.top

TS:   [...arr];
来源：http://gok.feifeiyinyue.top

Java: new ArrayList<>(list);
来源：http://lcu.mhx1999.top

Go:   copied := append([]int(nil), arr...)
来源：http://acf.cheryme.top

Ruby: arr.dup;  arr.clone
来源：http://nmj.ivvv.top

C#:   new List<int>(list);
来源：http://jkd.jqgufenzy.top

[D23] reduce 累积计算
来源：http://bdb.hcnkem.com

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://zpn.ivvv.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://bsm.fzhhl.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://eoj.feifeiyinyue.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wsr.cucudq.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://djc.gogol.net.cn

Go:   // 手写循环
来源：http://dxj.zdbjq.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://ict.cucudq.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://art.jyoumei.cn

[D24] 字典 / Map 基本操作
来源：http://syr.sjlbkw.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://tyc.wangshuangyany.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://egh.hesvh.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://egl.yongpay.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://ffd.sufxvd.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://ugx.vehdjk.com

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://gzq.bbcook.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://wct.jlsjyb.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://ytk.sweek.top

[D25] Set 集合去重与交并差
来源：http://qzn.vqdsnc.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://nxh.vqdsnc.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://tyy.zdbjq.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://iuc.iojbl.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://yra.guowangkeji.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://fuh.zhijiandao.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://ppz.andypj.xyz

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://ggm.zhoulong.xyz

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://rdn.yueranfly.top

[D26] 数组转字符串
来源：http://fnm.havefunace.top

Py:   ", ".join(map(str, arr))
来源：http://mnp.guowangkeji.top

PHP:  implode(", ", $arr);
来源：http://zjv.jinyuanbaomall.cn

JS:   arr.join(", ")
来源：http://upa.snrcjt.cn

TS:   arr.join(", ")
来源：http://tri.zycfv.cn

Java: String.join(", ", list)
来源：http://pmo.yj20258.top

Go:   strings.Join(strs, ", ")
来源：http://txs.hammf.cn

Ruby: arr.join(", ")
来源：http://fpv.birdmap.top

C#:   string.Join(", ", list)
来源：http://xyv.pengpengdd.cyou

================================================================================
来源：http://lvz.cheryme.top

E. 字符串处理
来源：http://oxx.tianlin.xyz

================================================================================
来源：http://fxl.pycfn.com

[E01] 拼接字符串
来源：http://ccp.snrcjt.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://ncx.hysaishi.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://qmy.tianlin.xyz

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://opf.cheryme.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://qei.epnwcf.com

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://iuf.uphjek.com

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://bud.wangdashe.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://qso.aibaodan.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://gvd.bjfxy.top

[E02] 重复字符串
来源：http://tez.epnwcf.com

Py:   "ab" * 3
来源：http://rwf.uphjek.com

PHP:  str_repeat("ab", 3);
来源：http://wqb.yj202588.top

JS:   "ab".repeat(3)
来源：http://dig.guowangkeji.top

TS:   "ab".repeat(3)
来源：http://maq.cdnleiting.top

Java: "ab".repeat(3)
来源：http://owe.yuanzhike.top

Go:   strings.Repeat("ab", 3)
来源：http://col.wangshuangyany.cn

Ruby: "ab" * 3
来源：http://rxa.jlsjyb.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://dgu.sxryk.cn

[E03] 截取子串
来源：http://rkt.vehdjk.com

Py:   s[1:4];  s[:3];  s[3:]
来源：http://urh.ydzc1.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://uig.316326.xyz

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://kmi.yonumen.top

TS:   s.slice(1, 4)
来源：http://geq.shangyingyoupin.top

Java: s.substring(1, 4)
来源：http://jai.daxiang520.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://yhs.shuidangran.top

Ruby: s[1, 3];  s[1..3]
来源：http://xal.0kj1m.cn

C#:   s.Substring(1, 3)
来源：http://xxa.jlsjyb.cn

[E04] 查找子串位置
来源：http://vom.ywan-chungtsiang.top

Py:   s.find("x");  s.index("x")
来源：http://eqs.uphjek.com

PHP:  strpos($s, "x");
来源：http://pip.zhiwuduotai.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://ezg.chenlongwang.top

TS:   s.indexOf("x")
来源：http://mob.hfpthk.cn

Java: s.indexOf("x")
来源：http://mzl.zdbjq.cn

Go:   strings.Index(s, "x")
来源：http://xcy.haohaochexian.top

Ruby: s.index("x")
来源：http://vin.yvedp.cn

C#:   s.IndexOf("x")
来源：http://ftr.yj20258888.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://kfk.316326.xyz

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://srg.cdnleiting.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://mni.hfpthk.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://eez.aibaodan.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://wgq.guannengcc.top


<!-- 参考信息 -->