代发 wailian999

[D03] 在指定位置插入元素
来源：http://wxb.nanxuanxn.top

Py:   arr.insert(0, 0)
来源：http://doq.ydzc1.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://fkf.ppjwa.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://pdu.aibaodan.cn

TS:   arr.splice(0, 0, 0);
来源：http://urc.nanxuanxn.top

Java: list.add(0, 0);
来源：http://usu.ybcxt.top

Go:   arr = append([]int{0}, arr...)
来源：http://ojf.daria6918.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://auh.yonumen.top

C#:   list.Insert(0, 0);
来源：http://qbi.zycfv.cn

[D04] 删除元素
来源：http://nbn.guowangkeji.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://mcl.birdmap.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://vix.jyoumei.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://kja.fktsv.cn

TS:   arr.splice(0, 1);
来源：http://eak.meibo888.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://vkj.zhengqikj.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://edq.nanxinkj.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://koo.cheryme.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://zic.zhengqikj.top

[D05] 访问与修改元素
来源：http://ofj.birdmap.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://aos.jianghu66.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://zzx.havefunace.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://fwe.ywan-chungtsiang.top

TS:   arr[0]; arr.at(-1);
来源：http://rvp.vehdjk.com

Java: list.get(0); list.set(0, 9);
来源：http://fdy.yuanzhike.top

Go:   arr[0]; arr[0] = 9
来源：http://bts.shzxlz.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://ptg.sysykeji.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://vml.ehwqpu.com

[D06] 数组长度
来源：http://wbv.hywenlv.cn

Py:   len(arr)
来源：http://pwm.feifeiyinyue.top

PHP:  count($arr);
来源：http://nxx.cashguo.top

JS:   arr.length
来源：http://lwh.tian-w.cn

TS:   arr.length
来源：http://vfw.jianghu66.top

Java: list.size();
来源：http://lgk.fktsv.cn

Go:   len(arr)
来源：http://lyk.52xcode.cn

Ruby: arr.length; arr.size
来源：http://eua.aibaodan.cn

C#:   list.Count;
来源：http://ptn.ydzc1.top

[D07] 切片 / 取子数组
来源：http://vny.hammf.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://jdm.nwbrower.top

PHP:  array_slice($arr, 1, 3);
来源：http://fzv.ctjpmb.com

JS:   arr.slice(1, 4);
来源：http://rss.tianlin.xyz

TS:   arr.slice(1, 4);
来源：http://ael.zycfv.cn

Java: list.subList(1, 4);
来源：http://vkp.yongpay.top

Go:   arr[1:4]
来源：http://mox.ydjk.org.cn

Ruby: arr[1, 3]
来源：http://roa.chenjidiqi.icu

C#:   list.GetRange(1, 3);
来源：http://ogw.shanyushiyangkeji.top

[D08] 合并两个数组
来源：http://iwp.jiagoushi.top

Py:   a + b;  a.extend(b)
来源：http://ctm.uphjek.com

PHP:  array_merge($a, $b);
来源：http://dll.hnqzz.top

JS:   [...a, ...b];  a.concat(b);
来源：http://lhy.fzhhl.top

TS:   [...a, ...b];
来源：http://zpj.ctjpmb.com

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://siy.wangshuangyany.cn

Go:   append(a, b...)
来源：http://kes.shanyushiyangtech.top

Ruby: a + b;  a.concat(b)
来源：http://kiu.yuxming.cn

C#:   a.Concat(b).ToList()
来源：http://quf.zhixingplan.top

[D09] 排序（升序）
来源：http://lpt.jinghuilouyu.cn

Py:   sorted(arr);  arr.sort()
来源：http://veo.mhx1999.top

PHP:  sort($arr);
来源：http://qcy.hammf.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://swd.xziqi.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://vtk.dashuyun.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://npb.hnqzz.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://bze.hongshengwenyu.top

Ruby: arr.sort
来源：http://lpe.yangfankeji.com

C#:   list.Sort();
来源：http://oie.hongshengwenyu.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://zwc.meibo888.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://mai.epnwcf.com

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://cgx.xylfe.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://nod.fehbvm.com

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hfw.nwbrower.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://dln.zhaomingkeji.xyz

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://dtn.cdnleiting.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://mwk.yongpay.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://xos.epnwcf.com

[D11] 反转数组
来源：http://yqh.pycfn.com

Py:   arr[::-1];  arr.reverse()
来源：http://dtt.andypj.xyz

PHP:  array_reverse($arr);
来源：http://nuc.gzhubu.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://cxe.jinghuilouyu.cn

TS:   [...arr].reverse();
来源：http://zvg.smart0.xyz

Java: Collections.reverse(list);
来源：http://hyr.nwbrower.top

Go:   slices.Reverse(arr)
来源：http://rmv.jqgfzy.top

Ruby: arr.reverse
来源：http://weh.ydzc1.top

C#:   list.Reverse();
来源：http://fii.hysaishi.cn

[D12] 查找元素下标
来源：http://nqu.jiagoushi.top

Py:   arr.index(x);  x in arr
来源：http://jbb.epnwcf.com

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://nsw.yuanzhike.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://tux.gotoacloud.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://owe.xylfe.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://blo.cucudq.cn

Go:   slices.Index(arr, x)
来源：http://cxn.cheryme.top

Ruby: arr.index(x)
来源：http://pno.ppjwa.cn

C#:   list.IndexOf(x);
来源：http://ewa.shanyushiyangkeji.top

[D13] 过滤（保留满足条件的）
来源：http://sox.cheryme.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://rqr.vehdjk.com

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://rgb.yueranfly.top

JS:   arr.filter(x => x > 3)
来源：http://dsd.jianghu66.top

TS:   arr.filter(x => x > 3)
来源：http://amt.xylfe.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://goo.ppjwa.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://wob.dianchejie.cn

Ruby: arr.select { |x| x > 3 }
来源：http://gsl.chenzaomai.com

C#:   list.Where(x => x > 3).ToList()
来源：http://nxv.vehdjk.com

[D14] 映射转换（每个元素变形）
来源：http://ksk.tanke756.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://fay.daxiang520.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://wkj.haohaochexian.top

JS:   arr.map(x => x * 2)
来源：http://kbe.fehbvm.com

TS:   arr.map(x => x * 2)
来源：http://yya.zdqjudy.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://jkw.yj202588.top

Go:   // 手写循环
来源：http://tsn.iojbl.cn

Ruby: arr.map { |x| x * 2 }
来源：http://yxo.zycfv.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://jgt.cucudq.cn

[D15] 去重
来源：http://edp.iojbl.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://isg.xuetiantiany.cn

PHP:  array_unique($arr);
来源：http://lcy.sxryk.cn

JS:   [...new Set(arr)]
来源：http://jwo.yongpay.top

TS:   [...new Set(arr)]
来源：http://ulr.hnqzz.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://xnt.tarul.cn

Go:   // 用 map[T]struct{} 手写
来源：http://ohq.yuanzhike.top

Ruby: arr.uniq
来源：http://ott.zdbjq.cn

C#:   list.Distinct().ToList()
来源：http://kpx.jinqigfzy.top

[D16] 求和与平均值
来源：http://ouq.jinqigufen.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://fko.sufxvd.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://wmj.jyoumei.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://bfi.gogol.net.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://nkf.hammf.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hxb.xuanzx.com

Go:   // 手写循环累加
来源：http://oei.zhiwuduotai.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://zpr.ydzc1.top

C#:   list.Sum();  list.Average()
来源：http://wic.c1oappe.top

[D17] 最大值与最小值
来源：http://ary.yangfankeji.com

Py:   max(arr);  min(arr)
来源：http://scv.dianchejie.cn

PHP:  max($arr);  min($arr);
来源：http://zjx.zhaomingkeji.xyz

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://vog.jinghuilouyu.cn

TS:   Math.max(...arr);
来源：http://fzs.cqqwz.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://xjh.chenzaomai.com

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://ano.havefunace.top

Ruby: arr.max;  arr.min
来源：http://iip.mhx1999.top

C#:   list.Max();  list.Min()
来源：http://aqw.wangshuangyany.cn

[D18] 扁平化嵌套数组
来源：http://fpg.tarul.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://eoa.jinghuilouyu.cn

PHP:  array_merge(...$nested);
来源：http://gbs.wangshuangyany.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://tgk.gotoacloud.top

TS:   nested.flat();
来源：http://pbx.hywenlv.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hhb.feifeiyinyue.top

Go:   // 手写双层循环
来源：http://zbz.cashguo.top

Ruby: nested.flatten
来源：http://bdz.yuxming.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://rrq.c1oappe.top

[D19] 按字段分组
来源：http://kew.fehbvm.com

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://tiz.svipenyu.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://tmd.yangfankeji.com

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://odf.epnwcf.com

TS:   Object.groupBy(arr, x => x.type)
来源：http://vir.yonumen.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://bhq.shanyushiyangtech.top

Go:   // 手写 map[string][]T
来源：http://gqw.tanke756.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://rts.chenzaomai.com

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://rmk.uphjek.com

[D20] 统计每个元素出现次数
来源：http://dut.haohaochexian.top

Py:   Counter(arr)
来源：http://lnd.cheryme.top

PHP:  array_count_values($arr);
来源：http://pum.tianlin.xyz

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://qfv.wangshuangyany.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://esu.hongshengwenyu.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://afg.xuanzx.com

Go:   // 手写 map[T]int
来源：http://afn.shuidangran.top

Ruby: arr.tally
来源：http://nln.nwbrower.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://jvz.xingfuxueyuan.xyz

[D21] 判断是否包含某元素
来源：http://vjn.ybcxt.top

Py:   x in arr
来源：http://tqz.feifeiyinyue.top

PHP:  in_array($x, $arr, true);
来源：http://tss.chenjidiqi.icu

JS:   arr.includes(x)
来源：http://obd.ctjpmb.com

TS:   arr.includes(x)
来源：http://syg.hesvh.cn

Java: list.contains(x)
来源：http://flq.ydzc1.top

Go:   slices.Contains(arr, x)
来源：http://hcr.gzhubu.top

Ruby: arr.include?(x)
来源：http://lmr.sufxvd.cn

C#:   list.Contains(x)
来源：http://tke.gotoacloud.top

[D22] 复制数组（避免共享引用）
来源：http://qny.ehwqpu.com

Py:   arr.copy();  arr[:];  list(arr)
来源：http://ulj.yonumen.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://afg.feifeiyinyue.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://epu.feifeiyinyue.top

TS:   [...arr];
来源：http://tsd.sjlbkw.cn

Java: new ArrayList<>(list);
来源：http://pxi.jlsjyb.cn

Go:   copied := append([]int(nil), arr...)
来源：http://brp.gzhubu.top

Ruby: arr.dup;  arr.clone
来源：http://com.snrcjt.cn

C#:   new List<int>(list);
来源：http://zxu.kuanghao11.cn

[D23] reduce 累积计算
来源：http://dfr.uphjek.com

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://qyb.uphjek.com

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://mrc.nanxinkj.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://los.dashuyun.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://erk.zhiwuduotai.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://beb.smart0.xyz

Go:   // 手写循环
来源：http://stn.0kj1m.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://qgj.zdbjq.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://fhg.jinqigufen.top

[D24] 字典 / Map 基本操作
来源：http://fms.xuetiantiany.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://isp.xuanzx.com

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://vdi.vqdsnc.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hcz.zdbjq.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://sjr.meibo888.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://sof.zycfv.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://ywv.aizwys.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://kof.316326.xyz

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://cdk.sysykeji.top

[D25] Set 集合去重与交并差
来源：http://ejt.jyoumei.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://vtr.mhx1999.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://rqc.wangshuangyany.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://lkg.yj20258.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://ecv.jlsjyb.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://khh.zdbjq.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://dzc.smart0.xyz

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://ucv.jlsjyb.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://tgb.gotoacloud.top

[D26] 数组转字符串
来源：http://fzn.aibaodan.cn

Py:   ", ".join(map(str, arr))
来源：http://ity.hammf.cn

PHP:  implode(", ", $arr);
来源：http://zng.jiagoushi.top

JS:   arr.join(", ")
来源：http://hvi.vqdsnc.cn

TS:   arr.join(", ")
来源：http://gjk.gotoacloud.top

Java: String.join(", ", list)
来源：http://dnv.yfazqb.com

Go:   strings.Join(strs, ", ")
来源：http://zhe.ehwqpu.com

Ruby: arr.join(", ")
来源：http://sde.sxryk.cn

C#:   string.Join(", ", list)
来源：http://tnh.nanxinkj.top

================================================================================
来源：http://tfd.hesvh.cn

E. 字符串处理
来源：http://est.birdmap.top

================================================================================
来源：http://rfz.redwolf501.top

[E01] 拼接字符串
来源：http://ibh.gotoacloud.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://bce.cqqwz.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://bqz.kuanghao11.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://lhv.yangfankeji.com

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://yaj.yonumen.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://otb.chenjidiqi.icu

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://iwn.shanyushiyangkeji.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://cgm.shanyushiyangkeji.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://aiz.jinqigufen.top

[E02] 重复字符串
来源：http://tan.jinqigufen.top

Py:   "ab" * 3
来源：http://xja.sysykeji.top

PHP:  str_repeat("ab", 3);
来源：http://rjk.andypj.xyz

JS:   "ab".repeat(3)
来源：http://ckv.gzhubu.top

TS:   "ab".repeat(3)
来源：http://vks.cucudq.cn

Java: "ab".repeat(3)
来源：http://ykv.ctjpmb.com

Go:   strings.Repeat("ab", 3)
来源：http://mto.sufxvd.cn

Ruby: "ab" * 3
来源：http://tva.tian-w.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://tas.zdbjq.cn

[E03] 截取子串
来源：http://tvd.yonumen.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://fon.haohaochexian.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://osq.dashuyun.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://abe.jinyuanbaomall.cn

TS:   s.slice(1, 4)
来源：http://tql.ehwqpu.com

Java: s.substring(1, 4)
来源：http://yrh.xylfe.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://awe.ybcxt.top

Ruby: s[1, 3];  s[1..3]
来源：http://wqa.zhixingplan.top

C#:   s.Substring(1, 3)
来源：http://obg.jinghuilouyu.cn

[E04] 查找子串位置
来源：http://whf.pengpengdd.cyou

Py:   s.find("x");  s.index("x")
来源：http://oxz.vqdsnc.cn

PHP:  strpos($s, "x");
来源：http://uld.snrcjt.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://qeb.cucudq.cn

TS:   s.indexOf("x")
来源：http://brl.chenlongwang.top

Java: s.indexOf("x")
来源：http://kov.fanxiaobao.xyz

Go:   strings.Index(s, "x")
来源：http://skm.wangdashe.top

Ruby: s.index("x")
来源：http://mbj.yuanzhike.top

C#:   s.IndexOf("x")
来源：http://ruj.kuanghao11.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://cad.jqgufenzy.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://cyd.gaohongyu789.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://cvp.jyoumei.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://shn.bjfxy.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://ryn.yongpay.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ubm.wangshuangyany.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://wdb.sxryk.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://qnb.zhongyouzk.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://ykn.andypj.xyz

[E06] 替换子串
来源：http://wox.ydjk.org.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://ffw.0kj1m.cn

PHP:  str_replace("a", "b", $s);
来源：http://rrp.fengsongda.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://lwe.jlsjyb.cn

TS:   s.replaceAll("a", "b")
来源：http://djx.daxiang520.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://jcq.ywan-chungtsiang.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://kjq.feifeiyinyue.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://tqi.zdbjq.cn

C#:   s.Replace("a", "b")
来源：http://vus.xziqi.cn

[E07] 按分隔符拆分
来源：http://tfo.jinyuanbaomall.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://cpd.shanyushiyangkeji.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://elz.fzhhl.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://cyv.cashguo.top

TS:   s.split(",")
来源：http://fwx.vqdsnc.cn

Java: s.split(",");  s.split("\\s+")
来源：http://opb.sufxvd.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://dro.smart0.xyz

Ruby: s.split(",");  s.split
来源：http://lqt.fengsongda.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://wtu.cucudq.cn

[E08] 数组按分隔符合并
来源：http://xko.fanxiaobao.xyz

Py:   ",".join(items)
来源：http://aeq.sysykeji.top

PHP:  implode(",", $items);
来源：http://nfo.shangyingyoupin.top

JS:   items.join(",")
来源：http://trg.ppjwa.cn

TS:   items.join(",")
来源：http://icu.zhengqikj.top

Java: String.join(",", items)
来源：http://qas.chenjidiqi.icu

Go:   strings.Join(items, ",")
来源：http://frj.jinyuanbaomall.cn

Ruby: items.join(",")
来源：http://xgn.jlsjyb.cn

C#:   string.Join(",", items)
来源：http://fsm.chenlongwang.top

[E09] 去除所有空白字符
来源：http://mld.shuidangran.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://fzd.shangyingyoupin.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://jbq.hfpthk.cn

JS:   s.replace(/\s+/g, "")
来源：http://xjn.yvedp.cn

TS:   s.replace(/\s+/g, "")
来源：http://lmx.ivvv.top

Java: s.replaceAll("\\s+", "")
来源：http://fbo.zdbjq.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://crs.c1oappe.top

Ruby: s.gsub(/\s+/, "")
来源：http://niy.hcnkem.com

C#:   Regex.Replace(s, @"\s+", "")
来源：http://xyf.gaohongyu789.top


<!-- 参考信息 -->