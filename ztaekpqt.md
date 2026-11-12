代发 wailian999

D. 数组 / 列表 / 集合
来源：http://ryg.cheryme.top

================================================================================
来源：http://tqp.zdqjudy.top

[D01] 创建数组 / 列表
来源：http://znl.52xcode.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://zbo.meibo888.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://esb.xylfe.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://wzc.cucudq.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://fsi.yvedp.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://icz.cdnleiting.top

Go:   arr := []int{1, 2, 3}
来源：http://jdf.shanyushiyangkeji.top

Ruby: arr = [1, 2, 3]
来源：http://ucy.ctjpmb.com

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://akk.52xcode.cn

[D02] 追加元素到末尾
来源：http://ahp.daria6918.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://fgo.fengsongda.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hsx.jianghu66.top

JS:   arr.push(4);
来源：http://orn.zhongyouzk.top

TS:   arr.push(4);
来源：http://hwm.xinyue.icu

Java: list.add(4);
来源：http://uyd.hnqzz.top

Go:   arr = append(arr, 4)
来源：http://ica.yangfankeji.com

Ruby: arr << 4; arr.push(5)
来源：http://eyc.shanyushiyangkeji.top

C#:   list.Add(4);
来源：http://wqy.ydjk.org.cn

[D03] 在指定位置插入元素
来源：http://agg.dashuyun.cn

Py:   arr.insert(0, 0)
来源：http://udo.c1oappe.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://wkp.shangyingyoupin.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://mbf.yfazqb.com

TS:   arr.splice(0, 0, 0);
来源：http://sba.shanyushiyangkeji.top

Java: list.add(0, 0);
来源：http://jee.yj20258.top

Go:   arr = append([]int{0}, arr...)
来源：http://qri.hongshengwenyu.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://ojh.shangyingyoupin.top

C#:   list.Insert(0, 0);
来源：http://zyi.zdbjq.cn

[D04] 删除元素
来源：http://sae.ctjpmb.com

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://jre.zhoulong.xyz

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://ipi.cdnleiting.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://cnr.xinyue.icu

TS:   arr.splice(0, 1);
来源：http://lvt.ywan-chungtsiang.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://cjn.9152youxi.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://emj.hnqzz.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://jyo.jyoumei.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://qyn.gogol.net.cn

[D05] 访问与修改元素
来源：http://huf.shzxlz.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://nxo.c1oappe.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://pkx.yanxiufei.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://csw.yanxiufei.cn

TS:   arr[0]; arr.at(-1);
来源：http://qia.hfpthk.cn

Java: list.get(0); list.set(0, 9);
来源：http://meh.fanxiaobao.xyz

Go:   arr[0]; arr[0] = 9
来源：http://dtn.316326.xyz

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://fck.ehwqpu.com

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://koa.yanxiufei.cn

[D06] 数组长度
来源：http://ppc.yonumen.top

Py:   len(arr)
来源：http://kma.cucudq.cn

PHP:  count($arr);
来源：http://hma.9152youxi.cn

JS:   arr.length
来源：http://wsx.bjfxy.top

TS:   arr.length
来源：http://vfu.sufxvd.cn

Java: list.size();
来源：http://kof.zycfv.cn

Go:   len(arr)
来源：http://ilb.dianchejie.cn

Ruby: arr.length; arr.size
来源：http://lmj.hfpthk.cn

C#:   list.Count;
来源：http://ugl.redwolf501.top

[D07] 切片 / 取子数组
来源：http://nnu.yanxiufei.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://qsl.ctjpmb.com

PHP:  array_slice($arr, 1, 3);
来源：http://awj.zdqjudy.top

JS:   arr.slice(1, 4);
来源：http://wcy.yfazqb.com

TS:   arr.slice(1, 4);
来源：http://oej.hnxiangtu.top

Java: list.subList(1, 4);
来源：http://ftk.yj20258888.top

Go:   arr[1:4]
来源：http://een.zhengqikj.top

Ruby: arr[1, 3]
来源：http://oba.vehdjk.com

C#:   list.GetRange(1, 3);
来源：http://caz.9152youxi.cn

[D08] 合并两个数组
来源：http://ric.fanxiaobao.xyz

Py:   a + b;  a.extend(b)
来源：http://uta.redwolf501.top

PHP:  array_merge($a, $b);
来源：http://aot.shzxlz.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://pqg.9152youxi.cn

TS:   [...a, ...b];
来源：http://xmd.ivvv.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://zzc.quarkkingdee.top

Go:   append(a, b...)
来源：http://pui.cqqwz.cn

Ruby: a + b;  a.concat(b)
来源：http://lzx.guannengcc.top

C#:   a.Concat(b).ToList()
来源：http://eyz.zdbjq.cn

[D09] 排序（升序）
来源：http://zml.shangyingyoupin.top

Py:   sorted(arr);  arr.sort()
来源：http://ymb.yvedp.cn

PHP:  sort($arr);
来源：http://zig.fktsv.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://fgz.jqgufenzy.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://yhq.uphjek.com

Java: Collections.sort(list);  list.sort(null);
来源：http://tfq.hnqzz.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://ufz.sweek.top

Ruby: arr.sort
来源：http://bpb.zhongyouzk.top

C#:   list.Sort();
来源：http://slf.cdnleiting.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://htq.chenlongwang.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hsw.yangfankeji.com

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://fwb.yuanzhike.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://qza.yfazqb.com

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://ajl.ydzc1.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://uzp.c1oappe.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://vpq.xuanzx.com

Ruby: arr.sort_by { |x| x[:age] }
来源：http://sbp.xuetiantiany.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://zia.tanke756.top

[D11] 反转数组
来源：http://hlk.feifeiyinyue.top

Py:   arr[::-1];  arr.reverse()
来源：http://pay.ywan-chungtsiang.top

PHP:  array_reverse($arr);
来源：http://fin.xingfuxueyuan.xyz

JS:   [...arr].reverse();  arr.toReversed()
来源：http://ijf.fanxiaobao.xyz

TS:   [...arr].reverse();
来源：http://aca.daria6918.cn

Java: Collections.reverse(list);
来源：http://ebo.guannengcc.top

Go:   slices.Reverse(arr)
来源：http://wsz.ydjk.org.cn

Ruby: arr.reverse
来源：http://pjq.yj20258.top

C#:   list.Reverse();
来源：http://wyq.xuetiantiany.cn

[D12] 查找元素下标
来源：http://vrs.zhoulong.xyz

Py:   arr.index(x);  x in arr
来源：http://rhc.yuxming.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://uav.birdmap.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ukj.yj202588.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ufp.guowangkeji.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://num.xinyue.icu

Go:   slices.Index(arr, x)
来源：http://iaq.jinqigfzy.top

Ruby: arr.index(x)
来源：http://uuq.sufxvd.cn

C#:   list.IndexOf(x);
来源：http://vay.shangyingyoupin.top

[D13] 过滤（保留满足条件的）
来源：http://zur.redwolf501.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://xra.vqdsnc.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://mcx.epnwcf.com

JS:   arr.filter(x => x > 3)
来源：http://gfa.shanyushiyangkeji.top

TS:   arr.filter(x => x > 3)
来源：http://wov.jianghu66.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://jkq.shuidangran.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://gsu.iojbl.cn

Ruby: arr.select { |x| x > 3 }
来源：http://twe.c1oappe.top

C#:   list.Where(x => x > 3).ToList()
来源：http://bsp.nwbrower.top

[D14] 映射转换（每个元素变形）
来源：http://uwx.zhoulong.xyz

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://shw.0kj1m.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://fwt.tarul.cn

JS:   arr.map(x => x * 2)
来源：http://ocy.bbcook.cn

TS:   arr.map(x => x * 2)
来源：http://rrh.zhongyouzk.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://rkh.zhixingplan.top

Go:   // 手写循环
来源：http://kco.haohaochexian.top

Ruby: arr.map { |x| x * 2 }
来源：http://qgl.zhaomingkeji.xyz

C#:   list.Select(x => x * 2).ToList()
来源：http://snv.jiagoushi.top

[D15] 去重
来源：http://jbd.bjfxy.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://ftf.ppjwa.cn

PHP:  array_unique($arr);
来源：http://veu.fengsongda.top

JS:   [...new Set(arr)]
来源：http://xkl.shuidangran.top

TS:   [...new Set(arr)]
来源：http://pgp.haohaochexian.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://qpr.jinqigfzy.top

Go:   // 用 map[T]struct{} 手写
来源：http://cwz.ywan-chungtsiang.top

Ruby: arr.uniq
来源：http://yla.tarul.cn

C#:   list.Distinct().ToList()
来源：http://vyc.chenzaomai.com

[D16] 求和与平均值
来源：http://nrk.cashguo.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://sdq.quarkkingdee.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://knn.jyoumei.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://rox.yuanzhike.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://dtg.ppjwa.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://cht.wangdashe.top

Go:   // 手写循环累加
来源：http://hxp.kuanghao11.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://xxw.redwolf501.top

C#:   list.Sum();  list.Average()
来源：http://pzu.ppjwa.cn

[D17] 最大值与最小值
来源：http://ooe.yangfankeji.com

Py:   max(arr);  min(arr)
来源：http://rec.guannengcc.top

PHP:  max($arr);  min($arr);
来源：http://etf.zdqjudy.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://cuo.shangyingyoupin.top

TS:   Math.max(...arr);
来源：http://ubq.pycfn.com

Java: Collections.max(list);  Collections.min(list);
来源：http://dtf.redwolf501.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://zkg.aibaodan.cn

Ruby: arr.max;  arr.min
来源：http://ool.tianlin.xyz

C#:   list.Max();  list.Min()
来源：http://jee.hammf.cn

[D18] 扁平化嵌套数组
来源：http://loe.andypj.xyz

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://bpp.haohaochexian.top

PHP:  array_merge(...$nested);
来源：http://eje.chenzaomai.com

JS:   nested.flat();  nested.flat(Infinity)
来源：http://uzx.shzxlz.cn

TS:   nested.flat();
来源：http://dvk.tarul.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://vcw.cashguo.top

Go:   // 手写双层循环
来源：http://vqm.gaohongyu789.top

Ruby: nested.flatten
来源：http://ury.wangdashe.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://kzu.guowangkeji.top

[D19] 按字段分组
来源：http://ghf.bbcook.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://ejz.yongpay.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://asf.haohaochexian.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://yqr.jinyuanbaomall.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://opt.ctjpmb.com

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://cgt.yuanzhike.top

Go:   // 手写 map[string][]T
来源：http://owd.zhiwuduotai.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://isf.cheryme.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://idd.haohaochexian.top

[D20] 统计每个元素出现次数
来源：http://zdc.jinqigfzy.top

Py:   Counter(arr)
来源：http://mls.yj20258888.top

PHP:  array_count_values($arr);
来源：http://pvy.havefunace.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://onl.hcnkem.com

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://vba.yangfankeji.com

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://fwi.hammf.cn

Go:   // 手写 map[T]int
来源：http://ksj.316326.xyz

Ruby: arr.tally
来源：http://jbo.yongpay.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://auk.ehwqpu.com

[D21] 判断是否包含某元素
来源：http://hds.sufxvd.cn

Py:   x in arr
来源：http://yuf.uphjek.com

PHP:  in_array($x, $arr, true);
来源：http://xct.nanxuanxn.top

JS:   arr.includes(x)
来源：http://rxs.zhijiandao.cn

TS:   arr.includes(x)
来源：http://kzw.yangfankeji.com

Java: list.contains(x)
来源：http://wai.cucudq.cn

Go:   slices.Contains(arr, x)
来源：http://cse.haohaochexian.top

Ruby: arr.include?(x)
来源：http://gig.snrcjt.cn

C#:   list.Contains(x)
来源：http://gom.smart0.xyz

[D22] 复制数组（避免共享引用）
来源：http://rfv.sysykeji.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://pev.fanxiaobao.xyz

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://klu.tarul.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://aex.jianghu66.top

TS:   [...arr];
来源：http://ulo.52xcode.cn

Java: new ArrayList<>(list);
来源：http://pyf.chenlongwang.top

Go:   copied := append([]int(nil), arr...)
来源：http://wyy.feifeiyinyue.top

Ruby: arr.dup;  arr.clone
来源：http://tav.chenlongwang.top

C#:   new List<int>(list);
来源：http://dxr.cashguo.top

[D23] reduce 累积计算
来源：http://hhh.xylfe.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://rtn.sweek.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://mpl.daria6918.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://eqs.jianghu66.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://fnb.ydzc1.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://mse.kuanghao11.cn

Go:   // 手写循环
来源：http://lsh.yueranfly.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://smv.ydjk.org.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://wrb.fanxiaobao.xyz

[D24] 字典 / Map 基本操作
来源：http://ybw.nanxuanxn.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://exj.yongpay.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hvb.sysykeji.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://mfk.xylfe.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://cfs.ybcxt.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hpz.hysaishi.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://jha.birdmap.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://fug.wangdashe.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://aqj.bjfxy.top

[D25] Set 集合去重与交并差
来源：http://oxz.kuanghao11.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://yeh.wangdashe.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://zms.yuxming.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://dlt.nwbrower.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://gjs.zdbjq.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://ura.jinqigfzy.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://kmw.gogol.net.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://oqd.316326.xyz

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://ifo.jinghuilouyu.cn

[D26] 数组转字符串
来源：http://hft.hnqzz.top

Py:   ", ".join(map(str, arr))
来源：http://szn.vehdjk.com

PHP:  implode(", ", $arr);
来源：http://sug.redwolf501.top

JS:   arr.join(", ")
来源：http://kfy.nanxuanxn.top

TS:   arr.join(", ")
来源：http://zwz.hammf.cn

Java: String.join(", ", list)
来源：http://zrk.shangyingyoupin.top

Go:   strings.Join(strs, ", ")
来源：http://vyb.yanxiufei.cn

Ruby: arr.join(", ")
来源：http://wyl.shuidangran.top

C#:   string.Join(", ", list)
来源：http://lon.havefunace.top

================================================================================
来源：http://dvv.chenlongwang.top

E. 字符串处理
来源：http://oep.ydjk.org.cn

================================================================================
来源：http://wlg.zdqjudy.top

[E01] 拼接字符串
来源：http://uvz.xziqi.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://ghj.bjfxy.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://iza.ctjpmb.com

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://qlj.yonumen.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://gvt.ppjwa.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://jpe.shanyushiyangkeji.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://jez.aizwys.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://zyc.feifeiyinyue.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://umi.vehdjk.com

[E02] 重复字符串
来源：http://ybs.shuidangran.top

Py:   "ab" * 3
来源：http://umx.aibaodan.cn

PHP:  str_repeat("ab", 3);
来源：http://olo.zhijiandao.cn

JS:   "ab".repeat(3)
来源：http://jxb.smart0.xyz

TS:   "ab".repeat(3)
来源：http://mrf.jinqigfzy.top

Java: "ab".repeat(3)
来源：http://mqe.hcnkem.com

Go:   strings.Repeat("ab", 3)
来源：http://ime.hongshengwenyu.top

Ruby: "ab" * 3
来源：http://czv.9152youxi.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://wtj.yonumen.top

[E03] 截取子串
来源：http://rrt.nanxinkj.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://kde.aizwys.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://zaf.zycfv.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://uzu.ivvv.top

TS:   s.slice(1, 4)
来源：http://gvt.kuanghao11.cn

Java: s.substring(1, 4)
来源：http://gkg.mhx1999.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://iyi.guannengcc.top

Ruby: s[1, 3];  s[1..3]
来源：http://rkz.jyoumei.cn

C#:   s.Substring(1, 3)
来源：http://dfp.ywan-chungtsiang.top

[E04] 查找子串位置
来源：http://pfw.yuanzhike.top

Py:   s.find("x");  s.index("x")
来源：http://dzi.zhiwuduotai.top

PHP:  strpos($s, "x");
来源：http://gcw.ywan-chungtsiang.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://fpa.daria6918.cn

TS:   s.indexOf("x")
来源：http://yhj.xziqi.cn

Java: s.indexOf("x")
来源：http://jpj.birdmap.top

Go:   strings.Index(s, "x")
来源：http://ido.gzhubu.top

Ruby: s.index("x")
来源：http://bks.ybcxt.top

C#:   s.IndexOf("x")
来源：http://btw.iojbl.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://ljn.zhengqikj.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://fvd.cashguo.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://osk.bjfxy.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://dlw.jinghuilouyu.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://eho.jinqigufen.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://xcf.sysykeji.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://dzg.feifeiyinyue.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://sjd.jiagoushi.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://mrn.hcnkem.com

[E06] 替换子串
来源：http://agl.iojbl.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://koa.sxryk.cn

PHP:  str_replace("a", "b", $s);
来源：http://abg.jinqigfzy.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://opc.c1oappe.top

TS:   s.replaceAll("a", "b")
来源：http://hja.hfpthk.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://flr.ydzc1.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://kyp.redwolf501.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://ofe.hysaishi.cn

C#:   s.Replace("a", "b")
来源：http://oao.yj202588.top

[E07] 按分隔符拆分
来源：http://iix.fzhhl.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://uju.guowangkeji.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://dky.jqgfzy.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://dig.hysaishi.cn

TS:   s.split(",")
来源：http://vzj.dianchejie.cn

Java: s.split(",");  s.split("\\s+")
来源：http://ukb.ctjpmb.com

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://jlr.tianlin.xyz


<!-- 参考信息 -->