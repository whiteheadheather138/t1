代发 wailian999

Go:   arr := []int{1, 2, 3}
来源：http://yvu.jiagoushi.top

Ruby: arr = [1, 2, 3]
来源：http://vxn.daria6918.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://oat.gogol.net.cn

[D02] 追加元素到末尾
来源：http://kim.yuxming.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://wnu.hongshengwenyu.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://lrc.jqgfzy.top

JS:   arr.push(4);
来源：http://flb.quarkkingdee.top

TS:   arr.push(4);
来源：http://hxu.nanxinkj.top

Java: list.add(4);
来源：http://ckw.shanyushiyangkeji.top

Go:   arr = append(arr, 4)
来源：http://elv.jiagoushi.top

Ruby: arr << 4; arr.push(5)
来源：http://mwb.shanyushiyangtech.top

C#:   list.Add(4);
来源：http://xvc.nanxinkj.top

[D03] 在指定位置插入元素
来源：http://xot.shzxlz.cn

Py:   arr.insert(0, 0)
来源：http://crt.fehbvm.com

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://pdq.gogol.net.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://wwy.sjlbkw.cn

TS:   arr.splice(0, 0, 0);
来源：http://jnt.hnqzz.top

Java: list.add(0, 0);
来源：http://nie.yuanzhike.top

Go:   arr = append([]int{0}, arr...)
来源：http://xee.chenzaomai.com

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://ldw.vqdsnc.cn

C#:   list.Insert(0, 0);
来源：http://zsx.yanxiufei.cn

[D04] 删除元素
来源：http://vsg.bbcook.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://dtk.fktsv.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://jhi.yj20258888.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://bsp.vehdjk.com

TS:   arr.splice(0, 1);
来源：http://tfm.svipenyu.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://wlf.sjlbkw.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://peq.cheryme.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://etk.feifeiyinyue.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://vcv.aibaodan.cn

[D05] 访问与修改元素
来源：http://yqj.shangyingyoupin.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://pfs.shangyingyoupin.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://uva.cqqwz.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://ngx.sxryk.cn

TS:   arr[0]; arr.at(-1);
来源：http://hxh.shangyingyoupin.top

Java: list.get(0); list.set(0, 9);
来源：http://gzk.yfazqb.com

Go:   arr[0]; arr[0] = 9
来源：http://rnh.gaohongyu789.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://rhh.c1oappe.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://dup.hongshengwenyu.top

[D06] 数组长度
来源：http://kba.fzhhl.top

Py:   len(arr)
来源：http://flj.shzxlz.cn

PHP:  count($arr);
来源：http://pft.chenlongwang.top

JS:   arr.length
来源：http://rqq.bbcook.cn

TS:   arr.length
来源：http://cbh.quarkkingdee.top

Java: list.size();
来源：http://ahg.aizwys.cn

Go:   len(arr)
来源：http://cyd.ivvv.top

Ruby: arr.length; arr.size
来源：http://xlc.zdqjudy.top

C#:   list.Count;
来源：http://nlu.ppjwa.cn

[D07] 切片 / 取子数组
来源：http://pcq.svipenyu.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://zxt.meibo888.top

PHP:  array_slice($arr, 1, 3);
来源：http://gxm.daria6918.cn

JS:   arr.slice(1, 4);
来源：http://boq.wangdashe.top

TS:   arr.slice(1, 4);
来源：http://yac.svipenyu.cn

Java: list.subList(1, 4);
来源：http://imv.xuetiantiany.cn

Go:   arr[1:4]
来源：http://gsr.xuanzx.com

Ruby: arr[1, 3]
来源：http://fja.jinqigufen.top

C#:   list.GetRange(1, 3);
来源：http://oxg.gaohongyu789.top

[D08] 合并两个数组
来源：http://kpf.ybcxt.top

Py:   a + b;  a.extend(b)
来源：http://osw.zhiwuduotai.top

PHP:  array_merge($a, $b);
来源：http://ixi.hnqzz.top

JS:   [...a, ...b];  a.concat(b);
来源：http://vdk.jinqigfzy.top

TS:   [...a, ...b];
来源：http://wmw.haohaochexian.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://uka.cdnleiting.top

Go:   append(a, b...)
来源：http://fqr.bbcook.cn

Ruby: a + b;  a.concat(b)
来源：http://jpd.sxryk.cn

C#:   a.Concat(b).ToList()
来源：http://usc.uphjek.com

[D09] 排序（升序）
来源：http://hzx.xylfe.cn

Py:   sorted(arr);  arr.sort()
来源：http://lvo.hesvh.cn

PHP:  sort($arr);
来源：http://rom.gotoacloud.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hcx.cashguo.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://xlr.havefunace.top

Java: Collections.sort(list);  list.sort(null);
来源：http://gub.yanxiufei.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://zoj.andypj.xyz

Ruby: arr.sort
来源：http://ytk.tian-w.cn

C#:   list.Sort();
来源：http://iqj.zhongyouzk.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://zxn.wangdashe.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://oss.zhongyouzk.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://jpg.jlsjyb.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://mup.svipenyu.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://qbu.tanke756.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://ord.fktsv.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://aby.zhongyouzk.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://ath.chenlongwang.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://ura.gzhubu.top

[D11] 反转数组
来源：http://vij.mhx1999.top

Py:   arr[::-1];  arr.reverse()
来源：http://kjz.yfazqb.com

PHP:  array_reverse($arr);
来源：http://acc.vehdjk.com

JS:   [...arr].reverse();  arr.toReversed()
来源：http://qck.tarul.cn

TS:   [...arr].reverse();
来源：http://wwh.hcnkem.com

Java: Collections.reverse(list);
来源：http://xjf.jqgufenzy.top

Go:   slices.Reverse(arr)
来源：http://rto.xuetiantiany.cn

Ruby: arr.reverse
来源：http://dfj.hywenlv.cn

C#:   list.Reverse();
来源：http://mnj.zhaomingkeji.xyz

[D12] 查找元素下标
来源：http://xmu.chenlongwang.top

Py:   arr.index(x);  x in arr
来源：http://whu.quarkkingdee.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://iwa.hcnkem.com

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://yrj.cashguo.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://kej.9152youxi.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://czl.zhaomingkeji.xyz

Go:   slices.Index(arr, x)
来源：http://fpf.hcnkem.com

Ruby: arr.index(x)
来源：http://icb.nanxinkj.top

C#:   list.IndexOf(x);
来源：http://gga.gzhubu.top

[D13] 过滤（保留满足条件的）
来源：http://qwk.ybcxt.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://cck.xuetiantiany.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://kbe.gogol.net.cn

JS:   arr.filter(x => x > 3)
来源：http://rre.cheryme.top

TS:   arr.filter(x => x > 3)
来源：http://jxg.zhengqikj.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://tzy.yj20258888.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://tpj.jlsjyb.cn

Ruby: arr.select { |x| x > 3 }
来源：http://jzt.tian-w.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://cod.nwbrower.top

[D14] 映射转换（每个元素变形）
来源：http://vky.gotoacloud.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://tqu.xylfe.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://pqv.fengsongda.top

JS:   arr.map(x => x * 2)
来源：http://sdw.sxryk.cn

TS:   arr.map(x => x * 2)
来源：http://miq.aibaodan.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://yql.hnxiangtu.top

Go:   // 手写循环
来源：http://hdw.epnwcf.com

Ruby: arr.map { |x| x * 2 }
来源：http://gwx.gotoacloud.top

C#:   list.Select(x => x * 2).ToList()
来源：http://vzf.jqgufenzy.top

[D15] 去重
来源：http://rwp.yonumen.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://ndk.zdqjudy.top

PHP:  array_unique($arr);
来源：http://bdl.xziqi.cn

JS:   [...new Set(arr)]
来源：http://qnd.jlsjyb.cn

TS:   [...new Set(arr)]
来源：http://myb.shanyushiyangtech.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://map.ehwqpu.com

Go:   // 用 map[T]struct{} 手写
来源：http://ffr.uphjek.com

Ruby: arr.uniq
来源：http://ttv.sjlbkw.cn

C#:   list.Distinct().ToList()
来源：http://gjm.fehbvm.com

[D16] 求和与平均值
来源：http://hkh.yonumen.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://xho.jlsjyb.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://bov.yueranfly.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://qew.dashuyun.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://elw.yongpay.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://dtd.tianlin.xyz

Go:   // 手写循环累加
来源：http://ixq.ppjwa.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://cmb.bjfxy.top

C#:   list.Sum();  list.Average()
来源：http://tdm.guowangkeji.top

[D17] 最大值与最小值
来源：http://fxr.zdbjq.cn

Py:   max(arr);  min(arr)
来源：http://blx.pengpengdd.cyou

PHP:  max($arr);  min($arr);
来源：http://mnm.vqdsnc.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://mhm.sxryk.cn

TS:   Math.max(...arr);
来源：http://wfl.cqqwz.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://ucq.sjlbkw.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://rfb.cucudq.cn

Ruby: arr.max;  arr.min
来源：http://jhl.daxiang520.top

C#:   list.Max();  list.Min()
来源：http://ikj.9152youxi.cn

[D18] 扁平化嵌套数组
来源：http://hic.gotoacloud.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hds.ydzc1.top

PHP:  array_merge(...$nested);
来源：http://zxk.haohaochexian.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://iud.jqgufenzy.top

TS:   nested.flat();
来源：http://eos.jyoumei.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://unq.9152youxi.cn

Go:   // 手写双层循环
来源：http://mca.tianlin.xyz

Ruby: nested.flatten
来源：http://psh.andypj.xyz

C#:   nested.SelectMany(x => x).ToList()
来源：http://nzz.jinqigfzy.top

[D19] 按字段分组
来源：http://vgw.zdqjudy.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://ifj.nanxuanxn.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://iox.shuidangran.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://bgl.daxiang520.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://ydo.fktsv.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://sbs.birdmap.top

Go:   // 手写 map[string][]T
来源：http://iws.cqqwz.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://kab.hammf.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://alj.ydjk.org.cn

[D20] 统计每个元素出现次数
来源：http://pim.yvedp.cn

Py:   Counter(arr)
来源：http://bii.smart0.xyz

PHP:  array_count_values($arr);
来源：http://ync.nanxuanxn.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://aij.yj202588.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://qkv.cashguo.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://lhy.0kj1m.cn

Go:   // 手写 map[T]int
来源：http://cgm.svipenyu.cn

Ruby: arr.tally
来源：http://euz.dianchejie.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://gad.52xcode.cn

[D21] 判断是否包含某元素
来源：http://akx.tianlin.xyz

Py:   x in arr
来源：http://ndl.pengpengdd.cyou

PHP:  in_array($x, $arr, true);
来源：http://zeb.svipenyu.cn

JS:   arr.includes(x)
来源：http://fxa.kuanghao11.cn

TS:   arr.includes(x)
来源：http://esu.kuanghao11.cn

Java: list.contains(x)
来源：http://jfi.yuxming.cn

Go:   slices.Contains(arr, x)
来源：http://ssd.tanke756.top

Ruby: arr.include?(x)
来源：http://zzi.zhixingplan.top

C#:   list.Contains(x)
来源：http://bsp.sysykeji.top

[D22] 复制数组（避免共享引用）
来源：http://bkb.0kj1m.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://tce.xylfe.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://efm.jinqigfzy.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://iyt.sxryk.cn

TS:   [...arr];
来源：http://jdr.mhx1999.top

Java: new ArrayList<>(list);
来源：http://ynm.52xcode.cn

Go:   copied := append([]int(nil), arr...)
来源：http://gdt.aizwys.cn

Ruby: arr.dup;  arr.clone
来源：http://pby.fktsv.cn

C#:   new List<int>(list);
来源：http://yxt.snrcjt.cn

[D23] reduce 累积计算
来源：http://jhi.snrcjt.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://ltc.jinghuilouyu.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://wye.sjlbkw.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://xyc.kuanghao11.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://kkn.yanxiufei.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://lwu.dianchejie.cn

Go:   // 手写循环
来源：http://rbi.yonumen.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://mam.zhengqikj.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://gir.gotoacloud.top

[D24] 字典 / Map 基本操作
来源：http://nrl.hammf.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://ipi.yvedp.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://rrg.tarul.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://rfx.haohaochexian.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://nle.hywenlv.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://vld.yvedp.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://qwb.yj20258888.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://yhc.aizwys.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://wpk.ydzc1.top

[D25] Set 集合去重与交并差
来源：http://cwk.shanyushiyangtech.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://fcl.cashguo.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://tqj.aibaodan.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://dpm.havefunace.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://jur.aizwys.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://zdb.sxryk.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://xmi.yj20258.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://xja.yanxiufei.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://xdz.meibo888.top

[D26] 数组转字符串
来源：http://fjc.nanxinkj.top

Py:   ", ".join(map(str, arr))
来源：http://kaz.yuxming.cn

PHP:  implode(", ", $arr);
来源：http://wzc.sweek.top

JS:   arr.join(", ")
来源：http://vbd.bjfxy.top

TS:   arr.join(", ")
来源：http://ztb.haohaochexian.top

Java: String.join(", ", list)
来源：http://ofl.jinqigufen.top

Go:   strings.Join(strs, ", ")
来源：http://rnp.ybcxt.top

Ruby: arr.join(", ")
来源：http://reh.yangfankeji.com

C#:   string.Join(", ", list)
来源：http://uno.jyoumei.cn

================================================================================
来源：http://ijr.feifeiyinyue.top

E. 字符串处理
来源：http://soq.zhaomingkeji.xyz

================================================================================
来源：http://fym.jinqigfzy.top

[E01] 拼接字符串
来源：http://esf.zhoulong.xyz

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://bxy.quarkkingdee.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://kpi.wangshuangyany.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://vtd.yueranfly.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://mef.wangdashe.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://zwu.havefunace.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://ixs.hfpthk.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://ofc.epnwcf.com

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://ood.redwolf501.top

[E02] 重复字符串
来源：http://lpi.c1oappe.top

Py:   "ab" * 3
来源：http://zee.yuxming.cn

PHP:  str_repeat("ab", 3);
来源：http://cwu.0kj1m.cn

JS:   "ab".repeat(3)
来源：http://teo.jiagoushi.top

TS:   "ab".repeat(3)
来源：http://gda.daria6918.cn

Java: "ab".repeat(3)
来源：http://wdz.aibaodan.cn

Go:   strings.Repeat("ab", 3)
来源：http://sqo.gzhubu.top

Ruby: "ab" * 3
来源：http://tti.uphjek.com

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://bir.jqgfzy.top

[E03] 截取子串
来源：http://bts.0kj1m.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://qvp.0kj1m.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://dbh.wangshuangyany.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hqw.redwolf501.top

TS:   s.slice(1, 4)
来源：http://scs.shuidangran.top

Java: s.substring(1, 4)
来源：http://lrq.ctjpmb.com

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://rit.nanxinkj.top

Ruby: s[1, 3];  s[1..3]
来源：http://txv.ywan-chungtsiang.top

C#:   s.Substring(1, 3)
来源：http://opf.xuetiantiany.cn

[E04] 查找子串位置
来源：http://fmz.yuanzhike.top

Py:   s.find("x");  s.index("x")
来源：http://bow.tanke756.top

PHP:  strpos($s, "x");
来源：http://tli.yuanzhike.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://skx.snrcjt.cn

TS:   s.indexOf("x")
来源：http://zfo.sxryk.cn

Java: s.indexOf("x")
来源：http://rum.xingfuxueyuan.xyz

Go:   strings.Index(s, "x")
来源：http://vmh.gotoacloud.top

Ruby: s.index("x")
来源：http://lxy.wangshuangyany.cn

C#:   s.IndexOf("x")
来源：http://xmm.yfazqb.com

[E05] 判断包含 / 前缀 / 后缀
来源：http://mzx.snrcjt.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://eww.tarul.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://eye.quarkkingdee.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://xlf.redwolf501.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://pgh.vehdjk.com

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://sfr.jlsjyb.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://ial.ywan-chungtsiang.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://lxv.yj202588.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://vyc.jinyuanbaomall.cn

[E06] 替换子串
来源：http://ckm.hnxiangtu.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://ksh.fengsongda.top

PHP:  str_replace("a", "b", $s);
来源：http://xvb.c1oappe.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://xpd.yonumen.top

TS:   s.replaceAll("a", "b")
来源：http://xti.zhengqikj.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wuq.ydjk.org.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://rlf.nanxuanxn.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://ung.yonumen.top

C#:   s.Replace("a", "b")
来源：http://jcs.xingfuxueyuan.xyz

[E07] 按分隔符拆分
来源：http://vmc.iojbl.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://mde.shanyushiyangkeji.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://yxy.ctjpmb.com

JS:   s.split(",");  s.split(/\s+/)
来源：http://tlb.cqqwz.cn

TS:   s.split(",")
来源：http://lgh.guannengcc.top

Java: s.split(",");  s.split("\\s+")
来源：http://uib.nwbrower.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://kru.yvedp.cn

Ruby: s.split(",");  s.split
来源：http://zof.snrcjt.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://jxr.chenzaomai.com

[E08] 数组按分隔符合并
来源：http://rvm.zycfv.cn

Py:   ",".join(items)
来源：http://phy.sufxvd.cn

PHP:  implode(",", $items);
来源：http://piq.hysaishi.cn

JS:   items.join(",")
来源：http://oyo.wangshuangyany.cn

TS:   items.join(",")
来源：http://xpr.vqdsnc.cn

Java: String.join(",", items)
来源：http://hkg.ybcxt.top


<!-- 参考信息 -->