代发 wailian999

D. 数组 / 列表 / 集合
来源：http://yfw.yongpay.top

================================================================================
来源：http://cyy.zhongyouzk.top

[D01] 创建数组 / 列表
来源：http://xgb.52xcode.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://twz.jiagoushi.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://lrf.yj20258888.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://kuk.uphjek.com

TS:   const arr: number[] = [1, 2, 3];
来源：http://ycn.yangfankeji.com

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://ejv.cdnleiting.top

Go:   arr := []int{1, 2, 3}
来源：http://osl.yueranfly.top

Ruby: arr = [1, 2, 3]
来源：http://ohj.yuanzhike.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://pjt.ehwqpu.com

[D02] 追加元素到末尾
来源：http://ijs.vqdsnc.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://avl.havefunace.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://yas.nanxuanxn.top

JS:   arr.push(4);
来源：http://bxg.hongshengwenyu.top

TS:   arr.push(4);
来源：http://brl.wangshuangyany.cn

Java: list.add(4);
来源：http://kbi.ppjwa.cn

Go:   arr = append(arr, 4)
来源：http://ggw.shuidangran.top

Ruby: arr << 4; arr.push(5)
来源：http://xqd.tarul.cn

C#:   list.Add(4);
来源：http://cyd.shzxlz.cn

[D03] 在指定位置插入元素
来源：http://efl.birdmap.top

Py:   arr.insert(0, 0)
来源：http://lbf.cheryme.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://fjl.daxiang520.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://lhp.xylfe.cn

TS:   arr.splice(0, 0, 0);
来源：http://ney.0kj1m.cn

Java: list.add(0, 0);
来源：http://wtn.cdnleiting.top

Go:   arr = append([]int{0}, arr...)
来源：http://wbu.feifeiyinyue.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hve.mhx1999.top

C#:   list.Insert(0, 0);
来源：http://vzt.yj20258888.top

[D04] 删除元素
来源：http://win.birdmap.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://rzr.9152youxi.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://uvy.dashuyun.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://laj.smart0.xyz

TS:   arr.splice(0, 1);
来源：http://nxb.hfpthk.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://fmb.52xcode.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://zom.nanxuanxn.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://qpx.zhoulong.xyz

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://jxy.tianlin.xyz

[D05] 访问与修改元素
来源：http://pov.hongshengwenyu.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://ohb.c1oappe.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://abq.tarul.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://ltm.guannengcc.top

TS:   arr[0]; arr.at(-1);
来源：http://rux.nwbrower.top

Java: list.get(0); list.set(0, 9);
来源：http://gtm.cqqwz.cn

Go:   arr[0]; arr[0] = 9
来源：http://zjz.guannengcc.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://ekx.shangyingyoupin.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://ehg.yonumen.top

[D06] 数组长度
来源：http://upw.sufxvd.cn

Py:   len(arr)
来源：http://frh.yangfankeji.com

PHP:  count($arr);
来源：http://lnj.c1oappe.top

JS:   arr.length
来源：http://tkt.zhiwuduotai.top

TS:   arr.length
来源：http://isy.quarkkingdee.top

Java: list.size();
来源：http://xgn.ywan-chungtsiang.top

Go:   len(arr)
来源：http://vop.jinqigfzy.top

Ruby: arr.length; arr.size
来源：http://kjl.jinyuanbaomall.cn

C#:   list.Count;
来源：http://ekv.meibo888.top

[D07] 切片 / 取子数组
来源：http://yqu.redwolf501.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://qii.nanxinkj.top

PHP:  array_slice($arr, 1, 3);
来源：http://ytk.chenzaomai.com

JS:   arr.slice(1, 4);
来源：http://fqp.xinyue.icu

TS:   arr.slice(1, 4);
来源：http://gey.vqdsnc.cn

Java: list.subList(1, 4);
来源：http://qsw.hammf.cn

Go:   arr[1:4]
来源：http://lgx.zhongyouzk.top

Ruby: arr[1, 3]
来源：http://hqk.vqdsnc.cn

C#:   list.GetRange(1, 3);
来源：http://bzh.zdbjq.cn

[D08] 合并两个数组
来源：http://ihi.yonumen.top

Py:   a + b;  a.extend(b)
来源：http://uxg.316326.xyz

PHP:  array_merge($a, $b);
来源：http://php.pengpengdd.cyou

JS:   [...a, ...b];  a.concat(b);
来源：http://cbf.shangyingyoupin.top

TS:   [...a, ...b];
来源：http://fin.redwolf501.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://vee.zhiwuduotai.top

Go:   append(a, b...)
来源：http://ebe.chenjidiqi.icu

Ruby: a + b;  a.concat(b)
来源：http://kqn.nanxinkj.top

C#:   a.Concat(b).ToList()
来源：http://mtw.jinyuanbaomall.cn

[D09] 排序（升序）
来源：http://aol.vqdsnc.cn

Py:   sorted(arr);  arr.sort()
来源：http://ljy.ppjwa.cn

PHP:  sort($arr);
来源：http://ymw.ivvv.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://uln.shanyushiyangtech.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://mxt.cdnleiting.top

Java: Collections.sort(list);  list.sort(null);
来源：http://htq.tanke756.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://xvg.yj202588.top

Ruby: arr.sort
来源：http://zhf.bbcook.cn

C#:   list.Sort();
来源：http://kap.cheryme.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://wwl.shuidangran.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://xrl.yonumen.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://lzl.fengsongda.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://ute.epnwcf.com

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://qlc.xziqi.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://fks.chenlongwang.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://oqq.yangfankeji.com

Ruby: arr.sort_by { |x| x[:age] }
来源：http://txx.wangdashe.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://oye.zdbjq.cn

[D11] 反转数组
来源：http://bze.ppjwa.cn

Py:   arr[::-1];  arr.reverse()
来源：http://pnb.fengsongda.top

PHP:  array_reverse($arr);
来源：http://afz.meibo888.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://vdq.chenjidiqi.icu

TS:   [...arr].reverse();
来源：http://wob.nanxuanxn.top

Java: Collections.reverse(list);
来源：http://kva.zhongyouzk.top

Go:   slices.Reverse(arr)
来源：http://xkf.bjfxy.top

Ruby: arr.reverse
来源：http://oas.yuanzhike.top

C#:   list.Reverse();
来源：http://mjp.yvedp.cn

[D12] 查找元素下标
来源：http://rbh.jiagoushi.top

Py:   arr.index(x);  x in arr
来源：http://eun.xingfuxueyuan.xyz

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://krj.shzxlz.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://gti.yuanzhike.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://dht.hnqzz.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://cll.316326.xyz

Go:   slices.Index(arr, x)
来源：http://ymh.xylfe.cn

Ruby: arr.index(x)
来源：http://ayu.yanxiufei.cn

C#:   list.IndexOf(x);
来源：http://hsc.shangyingyoupin.top

[D13] 过滤（保留满足条件的）
来源：http://nne.xingfuxueyuan.xyz

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://ohf.uphjek.com

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://oka.ydjk.org.cn

JS:   arr.filter(x => x > 3)
来源：http://scl.jqgufenzy.top

TS:   arr.filter(x => x > 3)
来源：http://koe.cqqwz.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://fxg.sjlbkw.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://pce.aibaodan.cn

Ruby: arr.select { |x| x > 3 }
来源：http://phz.hcnkem.com

C#:   list.Where(x => x > 3).ToList()
来源：http://bcd.nanxuanxn.top

[D14] 映射转换（每个元素变形）
来源：http://cpv.dashuyun.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://pas.fengsongda.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://vjs.feifeiyinyue.top

JS:   arr.map(x => x * 2)
来源：http://djs.haohaochexian.top

TS:   arr.map(x => x * 2)
来源：http://xln.ivvv.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://vfx.gzhubu.top

Go:   // 手写循环
来源：http://qcy.shangyingyoupin.top

Ruby: arr.map { |x| x * 2 }
来源：http://sri.yuanzhike.top

C#:   list.Select(x => x * 2).ToList()
来源：http://xku.ydzc1.top

[D15] 去重
来源：http://lpn.wangdashe.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://brl.vehdjk.com

PHP:  array_unique($arr);
来源：http://qnn.yangfankeji.com

JS:   [...new Set(arr)]
来源：http://gmv.guannengcc.top

TS:   [...new Set(arr)]
来源：http://mch.shangyingyoupin.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hyw.xingfuxueyuan.xyz

Go:   // 用 map[T]struct{} 手写
来源：http://mwi.fzhhl.top

Ruby: arr.uniq
来源：http://mlk.hesvh.cn

C#:   list.Distinct().ToList()
来源：http://jxq.zycfv.cn

[D16] 求和与平均值
来源：http://rgy.hfpthk.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://zdr.jinqigfzy.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://ccs.vehdjk.com

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://ewq.hammf.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://bpt.smart0.xyz

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://oms.0kj1m.cn

Go:   // 手写循环累加
来源：http://ncc.wangdashe.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://cly.zhongyouzk.top

C#:   list.Sum();  list.Average()
来源：http://zfe.hammf.cn

[D17] 最大值与最小值
来源：http://vst.jqgfzy.top

Py:   max(arr);  min(arr)
来源：http://bke.guannengcc.top

PHP:  max($arr);  min($arr);
来源：http://fqx.pengpengdd.cyou

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://cpg.yuanzhike.top

TS:   Math.max(...arr);
来源：http://ony.andypj.xyz

Java: Collections.max(list);  Collections.min(list);
来源：http://hao.xziqi.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://qmr.dianchejie.cn

Ruby: arr.max;  arr.min
来源：http://fjv.feifeiyinyue.top

C#:   list.Max();  list.Min()
来源：http://cmb.zhaomingkeji.xyz

[D18] 扁平化嵌套数组
来源：http://evl.ydjk.org.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://pkh.mhx1999.top

PHP:  array_merge(...$nested);
来源：http://nzd.sufxvd.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hax.fengsongda.top

TS:   nested.flat();
来源：http://agw.nwbrower.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://bvm.nanxinkj.top

Go:   // 手写双层循环
来源：http://ffn.tarul.cn

Ruby: nested.flatten
来源：http://miv.yanxiufei.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://gmu.fengsongda.top

[D19] 按字段分组
来源：http://vlu.uphjek.com

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://uja.tianlin.xyz

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://kra.vehdjk.com

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://vlr.wangshuangyany.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://kmk.kuanghao11.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://gvr.jianghu66.top

Go:   // 手写 map[string][]T
来源：http://rac.yonumen.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://uej.cheryme.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://sea.yongpay.top

[D20] 统计每个元素出现次数
来源：http://qqo.jyoumei.cn

Py:   Counter(arr)
来源：http://bfu.fktsv.cn

PHP:  array_count_values($arr);
来源：http://apv.ybcxt.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://zwg.yj20258.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://bwv.cqqwz.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://fti.pycfn.com

Go:   // 手写 map[T]int
来源：http://xix.jlsjyb.cn

Ruby: arr.tally
来源：http://eya.zhaomingkeji.xyz

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://uqa.yuanzhike.top

[D21] 判断是否包含某元素
来源：http://jul.ydzc1.top

Py:   x in arr
来源：http://dan.guannengcc.top

PHP:  in_array($x, $arr, true);
来源：http://spy.hysaishi.cn

JS:   arr.includes(x)
来源：http://idl.sxryk.cn

TS:   arr.includes(x)
来源：http://dhs.jlsjyb.cn

Java: list.contains(x)
来源：http://nap.shzxlz.cn

Go:   slices.Contains(arr, x)
来源：http://kxd.cucudq.cn

Ruby: arr.include?(x)
来源：http://mbs.vqdsnc.cn

C#:   list.Contains(x)
来源：http://hfh.hfpthk.cn

[D22] 复制数组（避免共享引用）
来源：http://kjg.shanyushiyangkeji.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://aoc.tianlin.xyz

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://xtg.yanxiufei.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://ndx.nwbrower.top

TS:   [...arr];
来源：http://vwz.hnxiangtu.top

Java: new ArrayList<>(list);
来源：http://tgc.xuetiantiany.cn

Go:   copied := append([]int(nil), arr...)
来源：http://qkb.hfpthk.cn

Ruby: arr.dup;  arr.clone
来源：http://sai.jinyuanbaomall.cn

C#:   new List<int>(list);
来源：http://tml.zhongyouzk.top

[D23] reduce 累积计算
来源：http://hcv.jianghu66.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://stg.pycfn.com

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://qnc.wangshuangyany.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://cqy.snrcjt.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hwm.zdqjudy.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://csm.jinqigfzy.top

Go:   // 手写循环
来源：http://mee.tian-w.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://nwj.vehdjk.com

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://gvh.jianghu66.top

[D24] 字典 / Map 基本操作
来源：http://rvd.hammf.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://wcn.jqgfzy.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://lzb.ctjpmb.com

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://bbl.nanxinkj.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://ujd.yvedp.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://tlw.dianchejie.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://ehn.jyoumei.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://tny.nwbrower.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://zwt.xingfuxueyuan.xyz

[D25] Set 集合去重与交并差
来源：http://etp.yongpay.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://ttp.nwbrower.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://guy.ydjk.org.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hbp.yonumen.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://gxf.havefunace.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://fnw.bbcook.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://vup.hammf.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://pco.ehwqpu.com

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://pgo.gaohongyu789.top

[D26] 数组转字符串
来源：http://azm.zhaomingkeji.xyz

Py:   ", ".join(map(str, arr))
来源：http://lur.smart0.xyz

PHP:  implode(", ", $arr);
来源：http://mjz.xuanzx.com

JS:   arr.join(", ")
来源：http://fka.jianghu66.top

TS:   arr.join(", ")
来源：http://fxy.yuxming.cn

Java: String.join(", ", list)
来源：http://gfq.yueranfly.top

Go:   strings.Join(strs, ", ")
来源：http://aob.yfazqb.com

Ruby: arr.join(", ")
来源：http://bfb.yj202588.top

C#:   string.Join(", ", list)
来源：http://ixt.gotoacloud.top

================================================================================
来源：http://wem.ctjpmb.com

E. 字符串处理
来源：http://pdh.daria6918.cn

================================================================================
来源：http://szf.bbcook.cn

[E01] 拼接字符串
来源：http://yln.yueranfly.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://bzi.cdnleiting.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://ksb.yueranfly.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://sxo.svipenyu.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://yap.chenlongwang.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://pcy.zdbjq.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://bbv.yongpay.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://yrd.jinqigfzy.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://yvm.sjlbkw.cn

[E02] 重复字符串
来源：http://ykl.jinghuilouyu.cn

Py:   "ab" * 3
来源：http://vpp.zdqjudy.top

PHP:  str_repeat("ab", 3);
来源：http://rlu.vehdjk.com

JS:   "ab".repeat(3)
来源：http://kme.zhijiandao.cn

TS:   "ab".repeat(3)
来源：http://dgq.chenzaomai.com

Java: "ab".repeat(3)
来源：http://pil.tarul.cn

Go:   strings.Repeat("ab", 3)
来源：http://czb.chenjidiqi.icu

Ruby: "ab" * 3
来源：http://dtg.ydjk.org.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://yya.feifeiyinyue.top

[E03] 截取子串
来源：http://mee.hfpthk.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://ixy.guowangkeji.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://mpd.zhoulong.xyz

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://gyc.ctjpmb.com

TS:   s.slice(1, 4)
来源：http://snr.vehdjk.com

Java: s.substring(1, 4)
来源：http://nbr.jiagoushi.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://oln.ywan-chungtsiang.top

Ruby: s[1, 3];  s[1..3]
来源：http://eub.xinyue.icu

C#:   s.Substring(1, 3)
来源：http://rrh.0kj1m.cn

[E04] 查找子串位置
来源：http://apv.cucudq.cn

Py:   s.find("x");  s.index("x")
来源：http://lxk.nanxuanxn.top

PHP:  strpos($s, "x");
来源：http://cqc.gaohongyu789.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://obx.zhijiandao.cn

TS:   s.indexOf("x")
来源：http://hqm.daria6918.cn

Java: s.indexOf("x")
来源：http://ehf.vqdsnc.cn

Go:   strings.Index(s, "x")
来源：http://tpl.jyoumei.cn

Ruby: s.index("x")
来源：http://cwg.xingfuxueyuan.xyz

C#:   s.IndexOf("x")
来源：http://mzf.pengpengdd.cyou

[E05] 判断包含 / 前缀 / 后缀
来源：http://exh.yonumen.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://zme.shzxlz.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://xsb.sysykeji.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://pdx.hesvh.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://zkr.guowangkeji.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://xqp.snrcjt.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://tso.yj20258.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://rig.chenjidiqi.icu

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://ewr.bbcook.cn

[E06] 替换子串
来源：http://viv.yj20258.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://dpf.yj20258.top

PHP:  str_replace("a", "b", $s);
来源：http://xai.andypj.xyz

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://jtj.shanyushiyangkeji.top

TS:   s.replaceAll("a", "b")
来源：http://gyr.bbcook.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ylq.yanxiufei.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://ule.jyoumei.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://vpx.andypj.xyz

C#:   s.Replace("a", "b")
来源：http://bla.aizwys.cn

[E07] 按分隔符拆分
来源：http://ifl.0kj1m.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://msy.xylfe.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://otr.quarkkingdee.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://uoo.zhongyouzk.top

TS:   s.split(",")
来源：http://pnu.yuanzhike.top

Java: s.split(",");  s.split("\\s+")
来源：http://azc.shzxlz.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://wyv.zdqjudy.top


<!-- 参考信息 -->