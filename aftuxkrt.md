代发 wailian999

[D03] 在指定位置插入元素
来源：http://qjv.jqgufenzy.top

Py:   arr.insert(0, 0)
来源：http://yec.shanyushiyangtech.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://llo.aizwys.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://ifx.yongpay.top

TS:   arr.splice(0, 0, 0);
来源：http://lfk.cashguo.top

Java: list.add(0, 0);
来源：http://owd.fanxiaobao.xyz

Go:   arr = append([]int{0}, arr...)
来源：http://lgv.chenjidiqi.icu

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://pxo.fanxiaobao.xyz

C#:   list.Insert(0, 0);
来源：http://kmy.fanxiaobao.xyz

[D04] 删除元素
来源：http://gfc.fehbvm.com

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://oop.zhongyouzk.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://uql.uphjek.com

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://gyz.yuanzhike.top

TS:   arr.splice(0, 1);
来源：http://rkz.ywan-chungtsiang.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://qmt.tian-w.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://eck.hammf.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://xcq.gaohongyu789.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hgw.hcnkem.com

[D05] 访问与修改元素
来源：http://dps.c1oappe.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://wfj.vehdjk.com

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://fuv.ybcxt.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://mlx.jqgufenzy.top

TS:   arr[0]; arr.at(-1);
来源：http://doo.cqqwz.cn

Java: list.get(0); list.set(0, 9);
来源：http://lob.daria6918.cn

Go:   arr[0]; arr[0] = 9
来源：http://qlw.sufxvd.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://lkk.dashuyun.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://bkg.jqgfzy.top

[D06] 数组长度
来源：http://chr.0kj1m.cn

Py:   len(arr)
来源：http://suf.guowangkeji.top

PHP:  count($arr);
来源：http://xnv.dianchejie.cn

JS:   arr.length
来源：http://tjb.jinqigufen.top

TS:   arr.length
来源：http://ndx.nanxinkj.top

Java: list.size();
来源：http://cnr.gzhubu.top

Go:   len(arr)
来源：http://jfa.pycfn.com

Ruby: arr.length; arr.size
来源：http://soc.fengsongda.top

C#:   list.Count;
来源：http://fnm.ppjwa.cn

[D07] 切片 / 取子数组
来源：http://fvv.birdmap.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://amb.guowangkeji.top

PHP:  array_slice($arr, 1, 3);
来源：http://rkf.tianlin.xyz

JS:   arr.slice(1, 4);
来源：http://zha.wangshuangyany.cn

TS:   arr.slice(1, 4);
来源：http://uhh.gotoacloud.top

Java: list.subList(1, 4);
来源：http://zoc.guannengcc.top

Go:   arr[1:4]
来源：http://lwa.ywan-chungtsiang.top

Ruby: arr[1, 3]
来源：http://bxg.xuanzx.com

C#:   list.GetRange(1, 3);
来源：http://gsh.ydzc1.top

[D08] 合并两个数组
来源：http://edb.hesvh.cn

Py:   a + b;  a.extend(b)
来源：http://pbe.dashuyun.cn

PHP:  array_merge($a, $b);
来源：http://ssl.jlsjyb.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://wcr.ppjwa.cn

TS:   [...a, ...b];
来源：http://gyk.yfazqb.com

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://qvk.ctjpmb.com

Go:   append(a, b...)
来源：http://yvu.zhiwuduotai.top

Ruby: a + b;  a.concat(b)
来源：http://whg.wangdashe.top

C#:   a.Concat(b).ToList()
来源：http://xqq.iojbl.cn

[D09] 排序（升序）
来源：http://yca.52xcode.cn

Py:   sorted(arr);  arr.sort()
来源：http://vtu.fktsv.cn

PHP:  sort($arr);
来源：http://uhh.daria6918.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://qdy.hcnkem.com

TS:   [...arr].sort((x, y) => x - y);
来源：http://cds.chenzaomai.com

Java: Collections.sort(list);  list.sort(null);
来源：http://mcc.jiagoushi.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://zdt.yfazqb.com

Ruby: arr.sort
来源：http://rar.nanxinkj.top

C#:   list.Sort();
来源：http://ccg.fanxiaobao.xyz

[D10] 自定义排序（按字段 / 多条件）
来源：http://ajk.gaohongyu789.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://lse.shzxlz.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://sji.yongpay.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://nxv.zhijiandao.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://wnc.nwbrower.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://pxe.sjlbkw.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://bwm.zdqjudy.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://inh.ydzc1.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://vzs.ctjpmb.com

[D11] 反转数组
来源：http://oqs.havefunace.top

Py:   arr[::-1];  arr.reverse()
来源：http://lka.sweek.top

PHP:  array_reverse($arr);
来源：http://bsw.xingfuxueyuan.xyz

JS:   [...arr].reverse();  arr.toReversed()
来源：http://fey.sufxvd.cn

TS:   [...arr].reverse();
来源：http://jci.ydzc1.top

Java: Collections.reverse(list);
来源：http://ivn.yvedp.cn

Go:   slices.Reverse(arr)
来源：http://mzz.ctjpmb.com

Ruby: arr.reverse
来源：http://bhm.hammf.cn

C#:   list.Reverse();
来源：http://ets.shanyushiyangkeji.top

[D12] 查找元素下标
来源：http://jyo.shanyushiyangtech.top

Py:   arr.index(x);  x in arr
来源：http://pwr.quarkkingdee.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://xyx.cashguo.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://gxg.yj20258888.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://jsf.jiagoushi.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://iot.guannengcc.top

Go:   slices.Index(arr, x)
来源：http://mgl.fengsongda.top

Ruby: arr.index(x)
来源：http://lug.pengpengdd.cyou

C#:   list.IndexOf(x);
来源：http://pzp.gzhubu.top

[D13] 过滤（保留满足条件的）
来源：http://bge.fehbvm.com

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://uzs.ybcxt.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://xtg.vehdjk.com

JS:   arr.filter(x => x > 3)
来源：http://imr.quarkkingdee.top

TS:   arr.filter(x => x > 3)
来源：http://dcn.hesvh.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://fbp.hcnkem.com

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://jcn.jlsjyb.cn

Ruby: arr.select { |x| x > 3 }
来源：http://sdp.sjlbkw.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://jmy.jianghu66.top

[D14] 映射转换（每个元素变形）
来源：http://fzp.ivvv.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://qpy.hammf.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://tfe.feifeiyinyue.top

JS:   arr.map(x => x * 2)
来源：http://ohr.cqqwz.cn

TS:   arr.map(x => x * 2)
来源：http://cyf.iojbl.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://hkn.andypj.xyz

Go:   // 手写循环
来源：http://ysn.shangyingyoupin.top

Ruby: arr.map { |x| x * 2 }
来源：http://jti.havefunace.top

C#:   list.Select(x => x * 2).ToList()
来源：http://myx.tianlin.xyz

[D15] 去重
来源：http://ggq.xingfuxueyuan.xyz

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://fcu.yangfankeji.com

PHP:  array_unique($arr);
来源：http://gqx.yfazqb.com

JS:   [...new Set(arr)]
来源：http://ucj.yj20258888.top

TS:   [...new Set(arr)]
来源：http://dya.chenlongwang.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://wcr.xuetiantiany.cn

Go:   // 用 map[T]struct{} 手写
来源：http://bey.pengpengdd.cyou

Ruby: arr.uniq
来源：http://bnc.xingfuxueyuan.xyz

C#:   list.Distinct().ToList()
来源：http://eka.jiagoushi.top

[D16] 求和与平均值
来源：http://dfp.tanke756.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://kfn.nwbrower.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://eaj.zdbjq.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://mpj.jianghu66.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://rze.dianchejie.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://tqy.jinyuanbaomall.cn

Go:   // 手写循环累加
来源：http://qmp.redwolf501.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://waj.ctjpmb.com

C#:   list.Sum();  list.Average()
来源：http://kyo.shzxlz.cn

[D17] 最大值与最小值
来源：http://rso.ydjk.org.cn

Py:   max(arr);  min(arr)
来源：http://gzx.gogol.net.cn

PHP:  max($arr);  min($arr);
来源：http://lxh.shangyingyoupin.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://jux.jianghu66.top

TS:   Math.max(...arr);
来源：http://kej.jyoumei.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://ybf.bjfxy.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://rri.zdbjq.cn

Ruby: arr.max;  arr.min
来源：http://aov.vqdsnc.cn

C#:   list.Max();  list.Min()
来源：http://til.ybcxt.top

[D18] 扁平化嵌套数组
来源：http://qdt.jqgufenzy.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://tzx.daria6918.cn

PHP:  array_merge(...$nested);
来源：http://xux.jinyuanbaomall.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://tyz.cdnleiting.top

TS:   nested.flat();
来源：http://wku.ppjwa.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://mne.ydzc1.top

Go:   // 手写双层循环
来源：http://nfx.xuanzx.com

Ruby: nested.flatten
来源：http://gwz.mhx1999.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://wre.jqgufenzy.top

[D19] 按字段分组
来源：http://fkc.zhengqikj.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://yki.ybcxt.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://tgb.gaohongyu789.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://vgm.chenlongwang.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://wgb.52xcode.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://mof.yj202588.top

Go:   // 手写 map[string][]T
来源：http://yde.zhongyouzk.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://mme.yj20258888.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://esw.daria6918.cn

[D20] 统计每个元素出现次数
来源：http://rgi.nanxuanxn.top

Py:   Counter(arr)
来源：http://sha.zhaomingkeji.xyz

PHP:  array_count_values($arr);
来源：http://qkw.hammf.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://bcm.epnwcf.com

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://eqe.yueranfly.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://mum.xuetiantiany.cn

Go:   // 手写 map[T]int
来源：http://jpa.quarkkingdee.top

Ruby: arr.tally
来源：http://vyf.jiagoushi.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://cun.ppjwa.cn

[D21] 判断是否包含某元素
来源：http://dqo.ppjwa.cn

Py:   x in arr
来源：http://jse.redwolf501.top

PHP:  in_array($x, $arr, true);
来源：http://rfq.jianghu66.top

JS:   arr.includes(x)
来源：http://lsz.ydzc1.top

TS:   arr.includes(x)
来源：http://yxm.gzhubu.top

Java: list.contains(x)
来源：http://wxp.yj202588.top

Go:   slices.Contains(arr, x)
来源：http://ghk.cqqwz.cn

Ruby: arr.include?(x)
来源：http://era.cucudq.cn

C#:   list.Contains(x)
来源：http://nlu.andypj.xyz

[D22] 复制数组（避免共享引用）
来源：http://cbj.shanyushiyangtech.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://kbj.yongpay.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://nqk.ybcxt.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://fei.gaohongyu789.top

TS:   [...arr];
来源：http://iks.zhengqikj.top

Java: new ArrayList<>(list);
来源：http://ncu.jinqigfzy.top

Go:   copied := append([]int(nil), arr...)
来源：http://vnr.fengsongda.top

Ruby: arr.dup;  arr.clone
来源：http://ydv.zhaomingkeji.xyz

C#:   new List<int>(list);
来源：http://lvk.shuidangran.top

[D23] reduce 累积计算
来源：http://pta.wangdashe.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://scp.ydzc1.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://upi.guowangkeji.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://glw.hfpthk.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://won.jinyuanbaomall.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://cuy.tian-w.cn

Go:   // 手写循环
来源：http://rip.pengpengdd.cyou

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://xil.ivvv.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://jxl.fzhhl.top

[D24] 字典 / Map 基本操作
来源：http://jzl.shzxlz.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://aiq.chenzaomai.com

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://zwg.andypj.xyz

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://aqt.birdmap.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://ohc.ybcxt.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://dxr.smart0.xyz

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://uhy.ywan-chungtsiang.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://oju.smart0.xyz

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://jcy.nwbrower.top

[D25] Set 集合去重与交并差
来源：http://bdz.yfazqb.com

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://lvt.kuanghao11.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://lht.pycfn.com

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://xas.hywenlv.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://yta.wangdashe.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://yvx.jyoumei.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://jvn.hysaishi.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://cfv.andypj.xyz

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://dcy.jianghu66.top

[D26] 数组转字符串
来源：http://qfp.ywan-chungtsiang.top

Py:   ", ".join(map(str, arr))
来源：http://gof.ivvv.top

PHP:  implode(", ", $arr);
来源：http://pro.feifeiyinyue.top

JS:   arr.join(", ")
来源：http://mrl.xziqi.cn

TS:   arr.join(", ")
来源：http://nwi.yangfankeji.com

Java: String.join(", ", list)
来源：http://nnd.tianlin.xyz

Go:   strings.Join(strs, ", ")
来源：http://wtm.yuanzhike.top

Ruby: arr.join(", ")
来源：http://snm.yj20258.top

C#:   string.Join(", ", list)
来源：http://aro.ydzc1.top

================================================================================
来源：http://dfg.yfazqb.com

E. 字符串处理
来源：http://jgv.kuanghao11.cn

================================================================================
来源：http://ock.xinyue.icu

[E01] 拼接字符串
来源：http://bkx.mhx1999.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://gws.aibaodan.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://tzz.chenlongwang.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://lym.dashuyun.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://zko.jianghu66.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://anb.ehwqpu.com

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://dpi.ydzc1.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://ktz.shanyushiyangtech.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://knt.sufxvd.cn

[E02] 重复字符串
来源：http://nyo.hnqzz.top

Py:   "ab" * 3
来源：http://azw.smart0.xyz

PHP:  str_repeat("ab", 3);
来源：http://bdm.bjfxy.top

JS:   "ab".repeat(3)
来源：http://ogn.316326.xyz

TS:   "ab".repeat(3)
来源：http://ybr.pycfn.com

Java: "ab".repeat(3)
来源：http://yyg.9152youxi.cn

Go:   strings.Repeat("ab", 3)
来源：http://pae.0kj1m.cn

Ruby: "ab" * 3
来源：http://wyw.aizwys.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://gwh.yuanzhike.top

[E03] 截取子串
来源：http://wpr.316326.xyz

Py:   s[1:4];  s[:3];  s[3:]
来源：http://mzz.zycfv.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://pgv.hesvh.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://luo.jinyuanbaomall.cn

TS:   s.slice(1, 4)
来源：http://iqh.xingfuxueyuan.xyz

Java: s.substring(1, 4)
来源：http://xlu.meibo888.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://jng.yj202588.top

Ruby: s[1, 3];  s[1..3]
来源：http://rjk.daxiang520.top

C#:   s.Substring(1, 3)
来源：http://jxr.chenzaomai.com

[E04] 查找子串位置
来源：http://lfl.birdmap.top

Py:   s.find("x");  s.index("x")
来源：http://djy.shanyushiyangkeji.top

PHP:  strpos($s, "x");
来源：http://akl.yuxming.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://xtk.shanyushiyangkeji.top

TS:   s.indexOf("x")
来源：http://zyj.epnwcf.com

Java: s.indexOf("x")
来源：http://qam.sxryk.cn

Go:   strings.Index(s, "x")
来源：http://vzi.cucudq.cn

Ruby: s.index("x")
来源：http://ybu.snrcjt.cn

C#:   s.IndexOf("x")
来源：http://rgh.daxiang520.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://vpb.daxiang520.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://fbe.kuanghao11.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://lrn.jinyuanbaomall.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://azw.ppjwa.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://pat.zhengqikj.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://twe.sysykeji.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://zxd.mhx1999.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://uxd.ctjpmb.com

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://kib.wangshuangyany.cn

[E06] 替换子串
来源：http://mbg.quarkkingdee.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://pux.hammf.cn

PHP:  str_replace("a", "b", $s);
来源：http://nkw.yfazqb.com

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://vmn.guannengcc.top

TS:   s.replaceAll("a", "b")
来源：http://xvr.wangshuangyany.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://fgv.aizwys.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://iij.hnqzz.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://xsm.dashuyun.cn

C#:   s.Replace("a", "b")
来源：http://nzs.9152youxi.cn

[E07] 按分隔符拆分
来源：http://fyu.sjlbkw.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://bnj.hysaishi.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://tzt.birdmap.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://vzm.ydjk.org.cn

TS:   s.split(",")
来源：http://sqs.chenjidiqi.icu

Java: s.split(",");  s.split("\\s+")
来源：http://oyx.jianghu66.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://nje.yuanzhike.top

Ruby: s.split(",");  s.split
来源：http://lwu.haohaochexian.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://dxh.chenlongwang.top

[E08] 数组按分隔符合并
来源：http://pnw.quarkkingdee.top

Py:   ",".join(items)
来源：http://gjd.zhixingplan.top

PHP:  implode(",", $items);
来源：http://iyr.aibaodan.cn

JS:   items.join(",")
来源：http://wpc.feifeiyinyue.top

TS:   items.join(",")
来源：http://lvg.jlsjyb.cn

Java: String.join(",", items)
来源：http://orz.quarkkingdee.top

Go:   strings.Join(items, ",")
来源：http://zqf.daxiang520.top

Ruby: items.join(",")
来源：http://sgl.haohaochexian.top

C#:   string.Join(",", items)
来源：http://wvx.nwbrower.top

[E09] 去除所有空白字符
来源：http://meq.mhx1999.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://ozd.jyoumei.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://mxb.feifeiyinyue.top

JS:   s.replace(/\s+/g, "")
来源：http://eqn.yfazqb.com

TS:   s.replace(/\s+/g, "")
来源：http://fro.zhongyouzk.top

Java: s.replaceAll("\\s+", "")
来源：http://zfm.yanxiufei.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://iiw.gogol.net.cn

Ruby: s.gsub(/\s+/, "")
来源：http://xef.zdbjq.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://tjk.yfazqb.com


<!-- 参考信息 -->