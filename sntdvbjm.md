代发 wailian999

C#:   list.Insert(0, 0);
来源：http://isr.shanyushiyangtech.top

[D04] 删除元素
来源：http://sft.kuanghao11.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://bbv.cucudq.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://lih.shanyushiyangkeji.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://ktq.jyoumei.cn

TS:   arr.splice(0, 1);
来源：http://qwo.c1oappe.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://tnr.xziqi.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://gwb.bbcook.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://kah.redwolf501.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://dow.sufxvd.cn

[D05] 访问与修改元素
来源：http://tbe.yueranfly.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://qnq.ctjpmb.com

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://nkx.cqqwz.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://ytx.tarul.cn

TS:   arr[0]; arr.at(-1);
来源：http://jcc.uphjek.com

Java: list.get(0); list.set(0, 9);
来源：http://dar.aibaodan.cn

Go:   arr[0]; arr[0] = 9
来源：http://ftq.fzhhl.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hss.daria6918.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://xoz.jinqigfzy.top

[D06] 数组长度
来源：http://ruu.gotoacloud.top

Py:   len(arr)
来源：http://byo.snrcjt.cn

PHP:  count($arr);
来源：http://hfn.sweek.top

JS:   arr.length
来源：http://ykf.sufxvd.cn

TS:   arr.length
来源：http://saj.sufxvd.cn

Java: list.size();
来源：http://ngo.sysykeji.top

Go:   len(arr)
来源：http://ntk.cucudq.cn

Ruby: arr.length; arr.size
来源：http://noi.hongshengwenyu.top

C#:   list.Count;
来源：http://fnn.ybcxt.top

[D07] 切片 / 取子数组
来源：http://yfx.ydzc1.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://tmq.tianlin.xyz

PHP:  array_slice($arr, 1, 3);
来源：http://pom.zhaomingkeji.xyz

JS:   arr.slice(1, 4);
来源：http://cbz.dashuyun.cn

TS:   arr.slice(1, 4);
来源：http://sll.kuanghao11.cn

Java: list.subList(1, 4);
来源：http://ind.kuanghao11.cn

Go:   arr[1:4]
来源：http://pou.jqgfzy.top

Ruby: arr[1, 3]
来源：http://nim.hcnkem.com

C#:   list.GetRange(1, 3);
来源：http://oul.zhaomingkeji.xyz

[D08] 合并两个数组
来源：http://gtl.ydjk.org.cn

Py:   a + b;  a.extend(b)
来源：http://qoy.zycfv.cn

PHP:  array_merge($a, $b);
来源：http://mxh.mhx1999.top

JS:   [...a, ...b];  a.concat(b);
来源：http://mvs.birdmap.top

TS:   [...a, ...b];
来源：http://lvl.sjlbkw.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://mvb.c1oappe.top

Go:   append(a, b...)
来源：http://mcs.xuanzx.com

Ruby: a + b;  a.concat(b)
来源：http://ofs.tian-w.cn

C#:   a.Concat(b).ToList()
来源：http://vny.haohaochexian.top

[D09] 排序（升序）
来源：http://jrm.xingfuxueyuan.xyz

Py:   sorted(arr);  arr.sort()
来源：http://kdk.fengsongda.top

PHP:  sort($arr);
来源：http://ecd.9152youxi.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://bdl.cqqwz.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://krs.c1oappe.top

Java: Collections.sort(list);  list.sort(null);
来源：http://dqc.fanxiaobao.xyz

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://ktq.cashguo.top

Ruby: arr.sort
来源：http://vyn.zhixingplan.top

C#:   list.Sort();
来源：http://dpi.chenlongwang.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://rjk.ehwqpu.com

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://fuc.yfazqb.com

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://rki.aibaodan.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://tuf.zhongyouzk.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://yfe.jlsjyb.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://nmk.xingfuxueyuan.xyz

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://ggx.yueranfly.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://dlh.zhijiandao.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://ohn.ehwqpu.com

[D11] 反转数组
来源：http://uoc.yanxiufei.cn

Py:   arr[::-1];  arr.reverse()
来源：http://mhl.vehdjk.com

PHP:  array_reverse($arr);
来源：http://awn.c1oappe.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://bmi.yuanzhike.top

TS:   [...arr].reverse();
来源：http://bgd.yvedp.cn

Java: Collections.reverse(list);
来源：http://yjh.cucudq.cn

Go:   slices.Reverse(arr)
来源：http://tsp.shzxlz.cn

Ruby: arr.reverse
来源：http://smv.ctjpmb.com

C#:   list.Reverse();
来源：http://opb.jinqigfzy.top

[D12] 查找元素下标
来源：http://tcu.andypj.xyz

Py:   arr.index(x);  x in arr
来源：http://rfp.gotoacloud.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://jfi.zhoulong.xyz

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://yey.zhoulong.xyz

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://uno.xylfe.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://ytc.jinqigufen.top

Go:   slices.Index(arr, x)
来源：http://tgz.316326.xyz

Ruby: arr.index(x)
来源：http://ncc.nwbrower.top

C#:   list.IndexOf(x);
来源：http://grv.cqqwz.cn

[D13] 过滤（保留满足条件的）
来源：http://ers.cashguo.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://rur.ppjwa.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://khn.hcnkem.com

JS:   arr.filter(x => x > 3)
来源：http://kbe.aibaodan.cn

TS:   arr.filter(x => x > 3)
来源：http://ege.fktsv.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://znt.nanxinkj.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://wvr.jlsjyb.cn

Ruby: arr.select { |x| x > 3 }
来源：http://uaw.shzxlz.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://pnt.xinyue.icu

[D14] 映射转换（每个元素变形）
来源：http://bim.cucudq.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://sez.hfpthk.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://ryc.nwbrower.top

JS:   arr.map(x => x * 2)
来源：http://upi.cdnleiting.top

TS:   arr.map(x => x * 2)
来源：http://bcb.snrcjt.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://dlp.chenzaomai.com

Go:   // 手写循环
来源：http://dzq.pengpengdd.cyou

Ruby: arr.map { |x| x * 2 }
来源：http://llf.cdnleiting.top

C#:   list.Select(x => x * 2).ToList()
来源：http://ulf.yongpay.top

[D15] 去重
来源：http://oxr.cqqwz.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://ftb.ppjwa.cn

PHP:  array_unique($arr);
来源：http://eof.zhengqikj.top

JS:   [...new Set(arr)]
来源：http://pzf.fehbvm.com

TS:   [...new Set(arr)]
来源：http://dti.gaohongyu789.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://ajv.aibaodan.cn

Go:   // 用 map[T]struct{} 手写
来源：http://xbt.fzhhl.top

Ruby: arr.uniq
来源：http://ylc.smart0.xyz

C#:   list.Distinct().ToList()
来源：http://ayf.xylfe.cn

[D16] 求和与平均值
来源：http://laf.birdmap.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://lrx.yfazqb.com

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://dlz.shanyushiyangkeji.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://wop.yuanzhike.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://tot.jinyuanbaomall.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://bqc.jianghu66.top

Go:   // 手写循环累加
来源：http://dpv.ybcxt.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://djr.daxiang520.top

C#:   list.Sum();  list.Average()
来源：http://lpk.ybcxt.top

[D17] 最大值与最小值
来源：http://gat.jqgufenzy.top

Py:   max(arr);  min(arr)
来源：http://tkz.yangfankeji.com

PHP:  max($arr);  min($arr);
来源：http://cua.tian-w.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://vgs.ydzc1.top

TS:   Math.max(...arr);
来源：http://ohg.wangshuangyany.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://vxb.zycfv.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://pin.nanxinkj.top

Ruby: arr.max;  arr.min
来源：http://pkq.svipenyu.cn

C#:   list.Max();  list.Min()
来源：http://ivn.aizwys.cn

[D18] 扁平化嵌套数组
来源：http://bba.haohaochexian.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://dti.fzhhl.top

PHP:  array_merge(...$nested);
来源：http://ykm.ydzc1.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://frj.sysykeji.top

TS:   nested.flat();
来源：http://xcm.yj20258888.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://jnz.jinyuanbaomall.cn

Go:   // 手写双层循环
来源：http://rmp.nanxuanxn.top

Ruby: nested.flatten
来源：http://wzc.ctjpmb.com

C#:   nested.SelectMany(x => x).ToList()
来源：http://fnt.sxryk.cn

[D19] 按字段分组
来源：http://vtk.shuidangran.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://uaw.hysaishi.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://lfo.shanyushiyangkeji.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://glu.ppjwa.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://hbw.nanxinkj.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://dco.gotoacloud.top

Go:   // 手写 map[string][]T
来源：http://bwy.svipenyu.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://dds.xziqi.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://kej.quarkkingdee.top

[D20] 统计每个元素出现次数
来源：http://jkl.xylfe.cn

Py:   Counter(arr)
来源：http://vup.cheryme.top

PHP:  array_count_values($arr);
来源：http://yor.quarkkingdee.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mmd.dashuyun.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://whh.yongpay.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://lna.nanxuanxn.top

Go:   // 手写 map[T]int
来源：http://tpv.yfazqb.com

Ruby: arr.tally
来源：http://uie.zhixingplan.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://lmq.xziqi.cn

[D21] 判断是否包含某元素
来源：http://tyx.sxryk.cn

Py:   x in arr
来源：http://fhd.smart0.xyz

PHP:  in_array($x, $arr, true);
来源：http://mgi.jqgfzy.top

JS:   arr.includes(x)
来源：http://emr.yueranfly.top

TS:   arr.includes(x)
来源：http://odp.guannengcc.top

Java: list.contains(x)
来源：http://cee.52xcode.cn

Go:   slices.Contains(arr, x)
来源：http://izo.shzxlz.cn

Ruby: arr.include?(x)
来源：http://vzk.nanxinkj.top

C#:   list.Contains(x)
来源：http://iir.jqgfzy.top

[D22] 复制数组（避免共享引用）
来源：http://yna.nanxinkj.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://xyo.yj20258.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://ngi.yueranfly.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://lnr.zhoulong.xyz

TS:   [...arr];
来源：http://yle.yvedp.cn

Java: new ArrayList<>(list);
来源：http://tyv.uphjek.com

Go:   copied := append([]int(nil), arr...)
来源：http://occ.yvedp.cn

Ruby: arr.dup;  arr.clone
来源：http://axy.yj20258888.top

C#:   new List<int>(list);
来源：http://zgd.yuxming.cn

[D23] reduce 累积计算
来源：http://akn.hfpthk.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://dtc.shangyingyoupin.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hwh.sxryk.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://iic.zhaomingkeji.xyz

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hxv.jinyuanbaomall.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://qes.52xcode.cn

Go:   // 手写循环
来源：http://qgx.zhaomingkeji.xyz

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://vct.snrcjt.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://ycb.kuanghao11.cn

[D24] 字典 / Map 基本操作
来源：http://zif.hnqzz.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://yjv.quarkkingdee.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://xrv.yongpay.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://udz.cashguo.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://fii.hcnkem.com

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://ofz.shanyushiyangtech.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://thx.hfpthk.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://zyx.jyoumei.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://knt.gogol.net.cn

[D25] Set 集合去重与交并差
来源：http://zww.cdnleiting.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://bic.bbcook.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://uci.yonumen.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://utl.gotoacloud.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://mwy.gotoacloud.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://kwt.ywan-chungtsiang.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://nfq.nwbrower.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://ldh.meibo888.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://saw.yanxiufei.cn

[D26] 数组转字符串
来源：http://qez.shanyushiyangtech.top

Py:   ", ".join(map(str, arr))
来源：http://gho.cucudq.cn

PHP:  implode(", ", $arr);
来源：http://sky.yangfankeji.com

JS:   arr.join(", ")
来源：http://utm.jlsjyb.cn

TS:   arr.join(", ")
来源：http://vix.fengsongda.top

Java: String.join(", ", list)
来源：http://ono.chenjidiqi.icu

Go:   strings.Join(strs, ", ")
来源：http://hso.daria6918.cn

Ruby: arr.join(", ")
来源：http://qcr.yonumen.top

C#:   string.Join(", ", list)
来源：http://ryb.jlsjyb.cn

================================================================================
来源：http://thw.tian-w.cn

E. 字符串处理
来源：http://kxk.jyoumei.cn

================================================================================
来源：http://ovk.yuxming.cn

[E01] 拼接字符串
来源：http://wxv.epnwcf.com

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://ehd.sufxvd.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://ehk.bjfxy.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://tyg.tianlin.xyz

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hpy.zdbjq.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://txf.sxryk.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://gjb.hammf.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://kcn.pycfn.com

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://shj.tian-w.cn

[E02] 重复字符串
来源：http://vqb.zdqjudy.top

Py:   "ab" * 3
来源：http://gob.hammf.cn

PHP:  str_repeat("ab", 3);
来源：http://hll.sufxvd.cn

JS:   "ab".repeat(3)
来源：http://vru.hysaishi.cn

TS:   "ab".repeat(3)
来源：http://hsq.zhongyouzk.top

Java: "ab".repeat(3)
来源：http://vne.zhixingplan.top

Go:   strings.Repeat("ab", 3)
来源：http://zjw.nwbrower.top

Ruby: "ab" * 3
来源：http://spg.mhx1999.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://xbx.ppjwa.cn

[E03] 截取子串
来源：http://hzx.jinyuanbaomall.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://rms.gaohongyu789.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://ohu.316326.xyz

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://ldi.tarul.cn

TS:   s.slice(1, 4)
来源：http://eto.nanxuanxn.top

Java: s.substring(1, 4)
来源：http://aua.zdqjudy.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://tnt.xuanzx.com

Ruby: s[1, 3];  s[1..3]
来源：http://psw.52xcode.cn

C#:   s.Substring(1, 3)
来源：http://xoz.fengsongda.top

[E04] 查找子串位置
来源：http://pso.ydjk.org.cn

Py:   s.find("x");  s.index("x")
来源：http://vil.yj20258888.top

PHP:  strpos($s, "x");
来源：http://gcf.zhixingplan.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://dba.cqqwz.cn

TS:   s.indexOf("x")
来源：http://nia.yonumen.top

Java: s.indexOf("x")
来源：http://gln.ydjk.org.cn

Go:   strings.Index(s, "x")
来源：http://utu.meibo888.top

Ruby: s.index("x")
来源：http://wjj.guannengcc.top

C#:   s.IndexOf("x")
来源：http://jic.shuidangran.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://mso.guannengcc.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://fqp.yvedp.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://aya.gotoacloud.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://vov.cheryme.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://vir.jinqigufen.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ebw.quarkkingdee.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://enn.vehdjk.com

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://fiu.dashuyun.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://xaj.sjlbkw.cn

[E06] 替换子串
来源：http://bso.ydjk.org.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://vvl.0kj1m.cn

PHP:  str_replace("a", "b", $s);
来源：http://lsp.birdmap.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ovt.yangfankeji.com

TS:   s.replaceAll("a", "b")
来源：http://giw.xuanzx.com

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hyk.jinyuanbaomall.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://wjj.ywan-chungtsiang.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://ska.zhixingplan.top

C#:   s.Replace("a", "b")
来源：http://mok.redwolf501.top

[E07] 按分隔符拆分
来源：http://clm.chenlongwang.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://pzw.daria6918.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://haj.yonumen.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://uzl.ppjwa.cn

TS:   s.split(",")
来源：http://jhx.guowangkeji.top

Java: s.split(",");  s.split("\\s+")
来源：http://ajq.zhengqikj.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://lsb.zhijiandao.cn

Ruby: s.split(",");  s.split
来源：http://eem.ydjk.org.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://jmt.aizwys.cn

[E08] 数组按分隔符合并
来源：http://iua.sysykeji.top

Py:   ",".join(items)
来源：http://buy.wangshuangyany.cn

PHP:  implode(",", $items);
来源：http://egr.dianchejie.cn

JS:   items.join(",")
来源：http://hqi.jlsjyb.cn

TS:   items.join(",")
来源：http://ykd.wangshuangyany.cn

Java: String.join(",", items)
来源：http://uzo.shangyingyoupin.top

Go:   strings.Join(items, ",")
来源：http://wcc.yvedp.cn

Ruby: items.join(",")
来源：http://xla.fzhhl.top

C#:   string.Join(",", items)
来源：http://mer.yvedp.cn

[E09] 去除所有空白字符
来源：http://foj.wangshuangyany.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://vjs.ehwqpu.com

PHP:  preg_replace('/\s+/', '', $s);
来源：http://tui.xuetiantiany.cn

JS:   s.replace(/\s+/g, "")
来源：http://wqn.jyoumei.cn

TS:   s.replace(/\s+/g, "")
来源：http://uvj.zhongyouzk.top

Java: s.replaceAll("\\s+", "")
来源：http://ckt.gaohongyu789.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://mae.zhengqikj.top

Ruby: s.gsub(/\s+/, "")
来源：http://axq.ivvv.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://izl.birdmap.top

[E10] 左侧补零 / 定长填充
来源：http://vza.chenlongwang.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://mtl.jinqigufen.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://ect.chenzaomai.com

JS:   "7".padStart(3, "0")
来源：http://nns.yuanzhike.top

TS:   "7".padStart(3, "0")
来源：http://mee.cheryme.top

Java: String.format("%03d", 7)
来源：http://rjx.feifeiyinyue.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://swl.sxryk.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://sqw.meibo888.top


<!-- 参考信息 -->