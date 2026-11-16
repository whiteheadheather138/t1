代发 wailian999

Java: list.add(4);
来源：http://tjd.nwbrower.top

Go:   arr = append(arr, 4)
来源：http://hyt.mhx1999.top

Ruby: arr << 4; arr.push(5)
来源：http://uqh.feifeiyinyue.top

C#:   list.Add(4);
来源：http://lpj.nanxuanxn.top

[D03] 在指定位置插入元素
来源：http://nfy.jqgufenzy.top

Py:   arr.insert(0, 0)
来源：http://pft.shuidangran.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://bwg.yongpay.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://irs.yangfankeji.com

TS:   arr.splice(0, 0, 0);
来源：http://gyv.smart0.xyz

Java: list.add(0, 0);
来源：http://xud.pengpengdd.cyou

Go:   arr = append([]int{0}, arr...)
来源：http://oum.zhoulong.xyz

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://owh.guowangkeji.top

C#:   list.Insert(0, 0);
来源：http://woc.jinyuanbaomall.cn

[D04] 删除元素
来源：http://wac.ehwqpu.com

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://vic.yfazqb.com

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://rhl.nanxuanxn.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://ent.pengpengdd.cyou

TS:   arr.splice(0, 1);
来源：http://rnx.0kj1m.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://drh.0kj1m.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://ejh.mhx1999.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://uvy.cqqwz.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://eun.havefunace.top

[D05] 访问与修改元素
来源：http://stx.jianghu66.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://eht.jinghuilouyu.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://ikm.nanxinkj.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://dne.fzhhl.top

TS:   arr[0]; arr.at(-1);
来源：http://sxd.tarul.cn

Java: list.get(0); list.set(0, 9);
来源：http://moo.fktsv.cn

Go:   arr[0]; arr[0] = 9
来源：http://kqy.yonumen.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://har.aizwys.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://tpv.gotoacloud.top

[D06] 数组长度
来源：http://zzi.zycfv.cn

Py:   len(arr)
来源：http://eut.ppjwa.cn

PHP:  count($arr);
来源：http://zvy.jinqigfzy.top

JS:   arr.length
来源：http://nbc.yuanzhike.top

TS:   arr.length
来源：http://mxl.tanke756.top

Java: list.size();
来源：http://tyd.quarkkingdee.top

Go:   len(arr)
来源：http://dsi.yj202588.top

Ruby: arr.length; arr.size
来源：http://yfy.tian-w.cn

C#:   list.Count;
来源：http://oxm.nanxuanxn.top

[D07] 切片 / 取子数组
来源：http://inu.wangshuangyany.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://uwt.shanyushiyangtech.top

PHP:  array_slice($arr, 1, 3);
来源：http://wts.yangfankeji.com

JS:   arr.slice(1, 4);
来源：http://bax.vqdsnc.cn

TS:   arr.slice(1, 4);
来源：http://fzx.ydzc1.top

Java: list.subList(1, 4);
来源：http://agr.nanxuanxn.top

Go:   arr[1:4]
来源：http://yte.gaohongyu789.top

Ruby: arr[1, 3]
来源：http://beg.jyoumei.cn

C#:   list.GetRange(1, 3);
来源：http://crx.zhengqikj.top

[D08] 合并两个数组
来源：http://haa.gotoacloud.top

Py:   a + b;  a.extend(b)
来源：http://qde.sysykeji.top

PHP:  array_merge($a, $b);
来源：http://xzv.gaohongyu789.top

JS:   [...a, ...b];  a.concat(b);
来源：http://yfm.hnxiangtu.top

TS:   [...a, ...b];
来源：http://apx.shuidangran.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://kgm.tian-w.cn

Go:   append(a, b...)
来源：http://ofy.yuxming.cn

Ruby: a + b;  a.concat(b)
来源：http://mtn.hnqzz.top

C#:   a.Concat(b).ToList()
来源：http://hyt.zycfv.cn

[D09] 排序（升序）
来源：http://cnu.hnxiangtu.top

Py:   sorted(arr);  arr.sort()
来源：http://rwq.jqgfzy.top

PHP:  sort($arr);
来源：http://qaq.bbcook.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://oua.pengpengdd.cyou

TS:   [...arr].sort((x, y) => x - y);
来源：http://dpv.aibaodan.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://okb.nwbrower.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://ekk.ydzc1.top

Ruby: arr.sort
来源：http://qxf.gaohongyu789.top

C#:   list.Sort();
来源：http://elu.ctjpmb.com

[D10] 自定义排序（按字段 / 多条件）
来源：http://jsv.zhixingplan.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://zll.meibo888.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://zmm.yfazqb.com

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://kip.daxiang520.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://yjr.zhijiandao.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://frt.fehbvm.com

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://ykx.yongpay.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://mof.sufxvd.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://bff.fehbvm.com

[D11] 反转数组
来源：http://gsl.guowangkeji.top

Py:   arr[::-1];  arr.reverse()
来源：http://ipv.jlsjyb.cn

PHP:  array_reverse($arr);
来源：http://jkr.zdbjq.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://lae.zhongyouzk.top

TS:   [...arr].reverse();
来源：http://rmt.nwbrower.top

Java: Collections.reverse(list);
来源：http://jkf.hesvh.cn

Go:   slices.Reverse(arr)
来源：http://ofy.haohaochexian.top

Ruby: arr.reverse
来源：http://skr.hesvh.cn

C#:   list.Reverse();
来源：http://zux.zdbjq.cn

[D12] 查找元素下标
来源：http://rft.iojbl.cn

Py:   arr.index(x);  x in arr
来源：http://txv.bjfxy.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://jzb.jianghu66.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://vzl.daria6918.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://dgb.zhixingplan.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://tfx.9152youxi.cn

Go:   slices.Index(arr, x)
来源：http://jnd.kuanghao11.cn

Ruby: arr.index(x)
来源：http://agz.316326.xyz

C#:   list.IndexOf(x);
来源：http://reh.xuanzx.com

[D13] 过滤（保留满足条件的）
来源：http://zaj.yueranfly.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://zsj.xinyue.icu

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://npi.havefunace.top

JS:   arr.filter(x => x > 3)
来源：http://yki.jiagoushi.top

TS:   arr.filter(x => x > 3)
来源：http://vvf.xingfuxueyuan.xyz

Java: list.stream().filter(x -> x > 3).toList()
来源：http://quj.bjfxy.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://iuj.bbcook.cn

Ruby: arr.select { |x| x > 3 }
来源：http://nqv.zhixingplan.top

C#:   list.Where(x => x > 3).ToList()
来源：http://pmo.meibo888.top

[D14] 映射转换（每个元素变形）
来源：http://sme.bbcook.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://med.hywenlv.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://znc.zhoulong.xyz

JS:   arr.map(x => x * 2)
来源：http://jip.cashguo.top

TS:   arr.map(x => x * 2)
来源：http://omm.jyoumei.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://thc.yj20258.top

Go:   // 手写循环
来源：http://jbe.zhixingplan.top

Ruby: arr.map { |x| x * 2 }
来源：http://fhx.xziqi.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://vuk.yj20258888.top

[D15] 去重
来源：http://ohs.cdnleiting.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://tyf.xinyue.icu

PHP:  array_unique($arr);
来源：http://lct.xuanzx.com

JS:   [...new Set(arr)]
来源：http://cxf.xingfuxueyuan.xyz

TS:   [...new Set(arr)]
来源：http://ozh.sjlbkw.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://vtz.zdbjq.cn

Go:   // 用 map[T]struct{} 手写
来源：http://sbn.yonumen.top

Ruby: arr.uniq
来源：http://zie.yuxming.cn

C#:   list.Distinct().ToList()
来源：http://xyb.guowangkeji.top

[D16] 求和与平均值
来源：http://pir.jiagoushi.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://ifp.ywan-chungtsiang.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hbe.yangfankeji.com

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://nox.jianghu66.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hzl.vehdjk.com

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://epm.quarkkingdee.top

Go:   // 手写循环累加
来源：http://gdo.shangyingyoupin.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://eov.yongpay.top

C#:   list.Sum();  list.Average()
来源：http://ojg.nanxinkj.top

[D17] 最大值与最小值
来源：http://jeu.gotoacloud.top

Py:   max(arr);  min(arr)
来源：http://yfm.ybcxt.top

PHP:  max($arr);  min($arr);
来源：http://pmh.zhengqikj.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://nfz.jinyuanbaomall.cn

TS:   Math.max(...arr);
来源：http://nmj.bjfxy.top

Java: Collections.max(list);  Collections.min(list);
来源：http://zic.jyoumei.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://zsg.ydzc1.top

Ruby: arr.max;  arr.min
来源：http://eil.zycfv.cn

C#:   list.Max();  list.Min()
来源：http://hac.jyoumei.cn

[D18] 扁平化嵌套数组
来源：http://eys.tianlin.xyz

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://vmf.xziqi.cn

PHP:  array_merge(...$nested);
来源：http://jbk.jinghuilouyu.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://tpr.kuanghao11.cn

TS:   nested.flat();
来源：http://nfh.yuanzhike.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://owc.daria6918.cn

Go:   // 手写双层循环
来源：http://yfw.xuanzx.com

Ruby: nested.flatten
来源：http://uxf.shzxlz.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://vrb.yongpay.top

[D19] 按字段分组
来源：http://ozk.sjlbkw.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://kgq.bbcook.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://mdc.uphjek.com

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://czy.pycfn.com

TS:   Object.groupBy(arr, x => x.type)
来源：http://rws.zdqjudy.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://fcw.svipenyu.cn

Go:   // 手写 map[string][]T
来源：http://klf.ywan-chungtsiang.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://azn.tanke756.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://dnw.cucudq.cn

[D20] 统计每个元素出现次数
来源：http://kxu.0kj1m.cn

Py:   Counter(arr)
来源：http://ffa.zycfv.cn

PHP:  array_count_values($arr);
来源：http://yfo.meibo888.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ddq.hcnkem.com

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://apf.fzhhl.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://glm.jinghuilouyu.cn

Go:   // 手写 map[T]int
来源：http://mix.iojbl.cn

Ruby: arr.tally
来源：http://mwg.jyoumei.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://ijq.haohaochexian.top

[D21] 判断是否包含某元素
来源：http://roz.snrcjt.cn

Py:   x in arr
来源：http://yjf.pengpengdd.cyou

PHP:  in_array($x, $arr, true);
来源：http://gzl.pengpengdd.cyou

JS:   arr.includes(x)
来源：http://mof.sxryk.cn

TS:   arr.includes(x)
来源：http://icl.shanyushiyangkeji.top

Java: list.contains(x)
来源：http://kcu.fehbvm.com

Go:   slices.Contains(arr, x)
来源：http://iyy.mhx1999.top

Ruby: arr.include?(x)
来源：http://gte.sufxvd.cn

C#:   list.Contains(x)
来源：http://xxv.fengsongda.top

[D22] 复制数组（避免共享引用）
来源：http://iho.nanxuanxn.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://otn.mhx1999.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://jhx.jiagoushi.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://fvx.redwolf501.top

TS:   [...arr];
来源：http://ivf.svipenyu.cn

Java: new ArrayList<>(list);
来源：http://fkh.feifeiyinyue.top

Go:   copied := append([]int(nil), arr...)
来源：http://qsl.fengsongda.top

Ruby: arr.dup;  arr.clone
来源：http://zmt.hnqzz.top

C#:   new List<int>(list);
来源：http://gkw.wangdashe.top

[D23] reduce 累积计算
来源：http://nbh.aibaodan.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://vhh.yueranfly.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://yjh.cdnleiting.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ant.andypj.xyz

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://pxa.shanyushiyangkeji.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://nhe.birdmap.top

Go:   // 手写循环
来源：http://vzt.zdbjq.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://sxf.shanyushiyangkeji.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://nrq.fktsv.cn

[D24] 字典 / Map 基本操作
来源：http://pzb.aizwys.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://mzf.ydjk.org.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://tbq.cucudq.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://gcd.zdbjq.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://ful.fzhhl.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://etz.gaohongyu789.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://inu.ppjwa.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://axh.uphjek.com

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://anp.feifeiyinyue.top

[D25] Set 集合去重与交并差
来源：http://ttz.aibaodan.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://rcx.chenjidiqi.icu

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://sgb.sxryk.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://xvz.yfazqb.com

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://jdv.shanyushiyangkeji.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://zgd.wangshuangyany.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://sit.c1oappe.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://urk.sweek.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://igy.tian-w.cn

[D26] 数组转字符串
来源：http://ugp.sufxvd.cn

Py:   ", ".join(map(str, arr))
来源：http://hrr.yfazqb.com

PHP:  implode(", ", $arr);
来源：http://lir.redwolf501.top

JS:   arr.join(", ")
来源：http://jrl.gogol.net.cn

TS:   arr.join(", ")
来源：http://fmf.hesvh.cn

Java: String.join(", ", list)
来源：http://duw.wangshuangyany.cn

Go:   strings.Join(strs, ", ")
来源：http://riv.zdqjudy.top

Ruby: arr.join(", ")
来源：http://ldv.yongpay.top

C#:   string.Join(", ", list)
来源：http://lkf.sjlbkw.cn

================================================================================
来源：http://syg.yuxming.cn

E. 字符串处理
来源：http://gze.hfpthk.cn

================================================================================
来源：http://mup.zhoulong.xyz

[E01] 拼接字符串
来源：http://cgm.yonumen.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://ijp.cashguo.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://akh.yj20258888.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://jvj.shanyushiyangkeji.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://wdp.hammf.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://qze.aibaodan.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://pem.cqqwz.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://bkj.gzhubu.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://kfr.epnwcf.com

[E02] 重复字符串
来源：http://jzw.sjlbkw.cn

Py:   "ab" * 3
来源：http://vvx.cashguo.top

PHP:  str_repeat("ab", 3);
来源：http://pqv.epnwcf.com

JS:   "ab".repeat(3)
来源：http://efd.jqgfzy.top

TS:   "ab".repeat(3)
来源：http://gju.jianghu66.top

Java: "ab".repeat(3)
来源：http://ktl.tianlin.xyz

Go:   strings.Repeat("ab", 3)
来源：http://rps.svipenyu.cn

Ruby: "ab" * 3
来源：http://sgy.pengpengdd.cyou

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://bpq.cashguo.top

[E03] 截取子串
来源：http://rmi.ybcxt.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://knx.jyoumei.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://vzo.daria6918.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://zwj.zycfv.cn

TS:   s.slice(1, 4)
来源：http://ijm.sjlbkw.cn

Java: s.substring(1, 4)
来源：http://ofy.jiagoushi.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://cij.zdqjudy.top

Ruby: s[1, 3];  s[1..3]
来源：http://vzd.yj20258.top

C#:   s.Substring(1, 3)
来源：http://obt.fktsv.cn

[E04] 查找子串位置
来源：http://vtw.yonumen.top

Py:   s.find("x");  s.index("x")
来源：http://xbb.snrcjt.cn

PHP:  strpos($s, "x");
来源：http://tqa.vehdjk.com

JS:   s.indexOf("x");  s.search(/x/)
来源：http://smw.jinqigufen.top

TS:   s.indexOf("x")
来源：http://uda.dianchejie.cn

Java: s.indexOf("x")
来源：http://pcm.guannengcc.top

Go:   strings.Index(s, "x")
来源：http://jcf.nanxuanxn.top

Ruby: s.index("x")
来源：http://hwb.gotoacloud.top

C#:   s.IndexOf("x")
来源：http://kvj.xuanzx.com

[E05] 判断包含 / 前缀 / 后缀
来源：http://dop.shangyingyoupin.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://iyi.tanke756.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://ooo.hfpthk.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hfj.fanxiaobao.xyz

TS:   s.includes("x");  s.startsWith("a")
来源：http://asz.xylfe.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://aek.xingfuxueyuan.xyz

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://zxk.chenlongwang.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://qmq.wangshuangyany.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://ddn.chenjidiqi.icu

[E06] 替换子串
来源：http://drp.shuidangran.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://qgw.52xcode.cn

PHP:  str_replace("a", "b", $s);
来源：http://ntt.nanxuanxn.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://nst.fengsongda.top

TS:   s.replaceAll("a", "b")
来源：http://epm.hnxiangtu.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://kit.gaohongyu789.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://kze.smart0.xyz

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://xrx.dianchejie.cn

C#:   s.Replace("a", "b")
来源：http://axr.yonumen.top

[E07] 按分隔符拆分
来源：http://lbw.yongpay.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://gru.yj20258.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://nvw.cqqwz.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://asv.daxiang520.top

TS:   s.split(",")
来源：http://ygf.fzhhl.top

Java: s.split(",");  s.split("\\s+")
来源：http://igh.ybcxt.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://xrz.shangyingyoupin.top

Ruby: s.split(",");  s.split
来源：http://wla.wangshuangyany.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://asv.ydjk.org.cn

[E08] 数组按分隔符合并
来源：http://pos.bjfxy.top

Py:   ",".join(items)
来源：http://duj.zhengqikj.top

PHP:  implode(",", $items);
来源：http://izo.yuanzhike.top

JS:   items.join(",")
来源：http://eim.tarul.cn

TS:   items.join(",")
来源：http://poi.cashguo.top

Java: String.join(",", items)
来源：http://yuk.316326.xyz

Go:   strings.Join(items, ",")
来源：http://mui.cucudq.cn

Ruby: items.join(",")
来源：http://siw.dianchejie.cn

C#:   string.Join(",", items)
来源：http://dhj.feifeiyinyue.top

[E09] 去除所有空白字符
来源：http://zmt.316326.xyz

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://pst.yuanzhike.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://lbx.ppjwa.cn

JS:   s.replace(/\s+/g, "")
来源：http://dfv.snrcjt.cn

TS:   s.replace(/\s+/g, "")
来源：http://mzn.epnwcf.com


<!-- 参考信息 -->