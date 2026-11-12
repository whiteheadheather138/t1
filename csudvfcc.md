代发 wailian999

Py:   arr.append(4); arr.extend([5, 6])
来源：http://upd.fehbvm.com

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://fsv.jinghuilouyu.cn

JS:   arr.push(4);
来源：http://yvw.daria6918.cn

TS:   arr.push(4);
来源：http://fla.ydzc1.top

Java: list.add(4);
来源：http://iho.gzhubu.top

Go:   arr = append(arr, 4)
来源：http://aqj.dianchejie.cn

Ruby: arr << 4; arr.push(5)
来源：http://glw.vehdjk.com

C#:   list.Add(4);
来源：http://apa.cqqwz.cn

[D03] 在指定位置插入元素
来源：http://kvz.jinyuanbaomall.cn

Py:   arr.insert(0, 0)
来源：http://dww.cashguo.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://kxd.tian-w.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://xmc.shanyushiyangtech.top

TS:   arr.splice(0, 0, 0);
来源：http://nru.cucudq.cn

Java: list.add(0, 0);
来源：http://yer.daxiang520.top

Go:   arr = append([]int{0}, arr...)
来源：http://zdx.redwolf501.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://rml.aibaodan.cn

C#:   list.Insert(0, 0);
来源：http://kii.shanyushiyangtech.top

[D04] 删除元素
来源：http://uap.yj20258.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://btd.quarkkingdee.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hzi.fengsongda.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://uqm.jqgfzy.top

TS:   arr.splice(0, 1);
来源：http://htv.pycfn.com

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://amx.daxiang520.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://jro.ywan-chungtsiang.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://fwh.iojbl.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://grl.gzhubu.top

[D05] 访问与修改元素
来源：http://smo.ydzc1.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://grw.yj20258888.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://fxm.jqgufenzy.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://xfx.jqgfzy.top

TS:   arr[0]; arr.at(-1);
来源：http://nrn.nwbrower.top

Java: list.get(0); list.set(0, 9);
来源：http://rmk.daria6918.cn

Go:   arr[0]; arr[0] = 9
来源：http://tqd.yfazqb.com

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://lfr.daria6918.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://xuo.yj20258888.top

[D06] 数组长度
来源：http://cnx.yj20258888.top

Py:   len(arr)
来源：http://nzc.fehbvm.com

PHP:  count($arr);
来源：http://akf.xingfuxueyuan.xyz

JS:   arr.length
来源：http://fug.iojbl.cn

TS:   arr.length
来源：http://fey.chenjidiqi.icu

Java: list.size();
来源：http://dlx.xylfe.cn

Go:   len(arr)
来源：http://kik.quarkkingdee.top

Ruby: arr.length; arr.size
来源：http://yab.nanxuanxn.top

C#:   list.Count;
来源：http://mnf.yj20258.top

[D07] 切片 / 取子数组
来源：http://ley.tarul.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://pvw.zdbjq.cn

PHP:  array_slice($arr, 1, 3);
来源：http://eoy.yvedp.cn

JS:   arr.slice(1, 4);
来源：http://krh.zdqjudy.top

TS:   arr.slice(1, 4);
来源：http://heo.gotoacloud.top

Java: list.subList(1, 4);
来源：http://pkh.hywenlv.cn

Go:   arr[1:4]
来源：http://tcd.fanxiaobao.xyz

Ruby: arr[1, 3]
来源：http://vya.bbcook.cn

C#:   list.GetRange(1, 3);
来源：http://pft.fanxiaobao.xyz

[D08] 合并两个数组
来源：http://yne.nwbrower.top

Py:   a + b;  a.extend(b)
来源：http://jph.hongshengwenyu.top

PHP:  array_merge($a, $b);
来源：http://uyr.nwbrower.top

JS:   [...a, ...b];  a.concat(b);
来源：http://jdj.sxryk.cn

TS:   [...a, ...b];
来源：http://ifr.ywan-chungtsiang.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://wap.uphjek.com

Go:   append(a, b...)
来源：http://wqq.316326.xyz

Ruby: a + b;  a.concat(b)
来源：http://qkb.snrcjt.cn

C#:   a.Concat(b).ToList()
来源：http://rih.daria6918.cn

[D09] 排序（升序）
来源：http://gka.iojbl.cn

Py:   sorted(arr);  arr.sort()
来源：http://ozs.yfazqb.com

PHP:  sort($arr);
来源：http://cte.haohaochexian.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://uhw.vehdjk.com

TS:   [...arr].sort((x, y) => x - y);
来源：http://uni.xziqi.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://mmk.yuxming.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://zak.nanxinkj.top

Ruby: arr.sort
来源：http://oys.hesvh.cn

C#:   list.Sort();
来源：http://uno.ctjpmb.com

[D10] 自定义排序（按字段 / 多条件）
来源：http://hgs.hywenlv.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://rbk.aibaodan.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://bqm.ehwqpu.com

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://wdf.zhoulong.xyz

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://jmo.0kj1m.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://nmc.yangfankeji.com

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://odx.fzhhl.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://dmp.svipenyu.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://usi.gotoacloud.top

[D11] 反转数组
来源：http://ttj.yongpay.top

Py:   arr[::-1];  arr.reverse()
来源：http://ppn.316326.xyz

PHP:  array_reverse($arr);
来源：http://rgo.yj20258888.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://pdn.gogol.net.cn

TS:   [...arr].reverse();
来源：http://ojr.smart0.xyz

Java: Collections.reverse(list);
来源：http://xqb.shangyingyoupin.top

Go:   slices.Reverse(arr)
来源：http://snz.ppjwa.cn

Ruby: arr.reverse
来源：http://eeq.tarul.cn

C#:   list.Reverse();
来源：http://qxi.yonumen.top

[D12] 查找元素下标
来源：http://ulb.ppjwa.cn

Py:   arr.index(x);  x in arr
来源：http://jel.xuetiantiany.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://ixl.guowangkeji.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mpn.jyoumei.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://uzm.ydzc1.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://wic.yfazqb.com

Go:   slices.Index(arr, x)
来源：http://oue.0kj1m.cn

Ruby: arr.index(x)
来源：http://ewo.hywenlv.cn

C#:   list.IndexOf(x);
来源：http://grl.tian-w.cn

[D13] 过滤（保留满足条件的）
来源：http://zrz.quarkkingdee.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://sxg.zhiwuduotai.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://wwc.wangdashe.top

JS:   arr.filter(x => x > 3)
来源：http://itk.cdnleiting.top

TS:   arr.filter(x => x > 3)
来源：http://tzx.feifeiyinyue.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://tzc.vehdjk.com

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://rkk.chenzaomai.com

Ruby: arr.select { |x| x > 3 }
来源：http://ebc.xuanzx.com

C#:   list.Where(x => x > 3).ToList()
来源：http://ovz.ctjpmb.com

[D14] 映射转换（每个元素变形）
来源：http://urt.jqgufenzy.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://gup.fktsv.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://gmg.ctjpmb.com

JS:   arr.map(x => x * 2)
来源：http://qhc.ppjwa.cn

TS:   arr.map(x => x * 2)
来源：http://tsz.ivvv.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://zmn.zhijiandao.cn

Go:   // 手写循环
来源：http://uay.zycfv.cn

Ruby: arr.map { |x| x * 2 }
来源：http://wnz.0kj1m.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://kda.hammf.cn

[D15] 去重
来源：http://drq.hesvh.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://tow.gogol.net.cn

PHP:  array_unique($arr);
来源：http://uhz.ivvv.top

JS:   [...new Set(arr)]
来源：http://tid.c1oappe.top

TS:   [...new Set(arr)]
来源：http://rxy.vehdjk.com

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://edz.cdnleiting.top

Go:   // 用 map[T]struct{} 手写
来源：http://rtl.sysykeji.top

Ruby: arr.uniq
来源：http://szi.hfpthk.cn

C#:   list.Distinct().ToList()
来源：http://nae.zdbjq.cn

[D16] 求和与平均值
来源：http://yrj.kuanghao11.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://oxp.jianghu66.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://yeb.nanxinkj.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://byz.shangyingyoupin.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://gcj.ydzc1.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://xnq.ppjwa.cn

Go:   // 手写循环累加
来源：http://rai.ctjpmb.com

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://fae.redwolf501.top

C#:   list.Sum();  list.Average()
来源：http://iim.zhijiandao.cn

[D17] 最大值与最小值
来源：http://qhi.fktsv.cn

Py:   max(arr);  min(arr)
来源：http://hmt.epnwcf.com

PHP:  max($arr);  min($arr);
来源：http://imf.ydzc1.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://bml.jlsjyb.cn

TS:   Math.max(...arr);
来源：http://mxj.316326.xyz

Java: Collections.max(list);  Collections.min(list);
来源：http://cfs.jinghuilouyu.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://rnm.jinqigufen.top

Ruby: arr.max;  arr.min
来源：http://idn.epnwcf.com

C#:   list.Max();  list.Min()
来源：http://oqd.xingfuxueyuan.xyz

[D18] 扁平化嵌套数组
来源：http://fbe.xuanzx.com

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://uvr.chenjidiqi.icu

PHP:  array_merge(...$nested);
来源：http://eds.vqdsnc.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://izj.tarul.cn

TS:   nested.flat();
来源：http://spu.zhiwuduotai.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://sns.zhoulong.xyz

Go:   // 手写双层循环
来源：http://xpx.andypj.xyz

Ruby: nested.flatten
来源：http://qhd.hcnkem.com

C#:   nested.SelectMany(x => x).ToList()
来源：http://mtq.chenzaomai.com

[D19] 按字段分组
来源：http://tyg.jianghu66.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://ybg.jqgfzy.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://qvp.zdbjq.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://wcc.xuetiantiany.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://fax.yueranfly.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://gnk.xuetiantiany.cn

Go:   // 手写 map[string][]T
来源：http://blr.chenlongwang.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://gxi.shangyingyoupin.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://zft.daria6918.cn

[D20] 统计每个元素出现次数
来源：http://xmk.shzxlz.cn

Py:   Counter(arr)
来源：http://wgp.yueranfly.top

PHP:  array_count_values($arr);
来源：http://yrd.sjlbkw.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://zal.cucudq.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://rli.sysykeji.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hld.cheryme.top

Go:   // 手写 map[T]int
来源：http://mll.sufxvd.cn

Ruby: arr.tally
来源：http://lje.hongshengwenyu.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://zsc.zhoulong.xyz

[D21] 判断是否包含某元素
来源：http://ftj.52xcode.cn

Py:   x in arr
来源：http://zhn.tian-w.cn

PHP:  in_array($x, $arr, true);
来源：http://gyv.snrcjt.cn

JS:   arr.includes(x)
来源：http://cyf.xziqi.cn

TS:   arr.includes(x)
来源：http://fbc.zdqjudy.top

Java: list.contains(x)
来源：http://qph.nanxinkj.top

Go:   slices.Contains(arr, x)
来源：http://dlb.jinyuanbaomall.cn

Ruby: arr.include?(x)
来源：http://rsa.aibaodan.cn

C#:   list.Contains(x)
来源：http://bdp.bjfxy.top

[D22] 复制数组（避免共享引用）
来源：http://uek.kuanghao11.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://jnu.bbcook.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://wiw.zdbjq.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://kds.cdnleiting.top

TS:   [...arr];
来源：http://zvt.uphjek.com

Java: new ArrayList<>(list);
来源：http://swo.gogol.net.cn

Go:   copied := append([]int(nil), arr...)
来源：http://oak.zhixingplan.top

Ruby: arr.dup;  arr.clone
来源：http://oph.zhengqikj.top

C#:   new List<int>(list);
来源：http://tng.daxiang520.top

[D23] reduce 累积计算
来源：http://agg.xuanzx.com

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://mdk.dianchejie.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://meh.guannengcc.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hjv.mhx1999.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wek.hammf.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://yjo.ivvv.top

Go:   // 手写循环
来源：http://ywe.meibo888.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://wgs.redwolf501.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://zcy.tian-w.cn

[D24] 字典 / Map 基本操作
来源：http://xof.yangfankeji.com

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://qps.nanxinkj.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://txe.hongshengwenyu.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://jjp.jqgufenzy.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://emw.hesvh.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://tkw.yfazqb.com

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://wev.ydzc1.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://ctm.shzxlz.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://ghb.hysaishi.cn

[D25] Set 集合去重与交并差
来源：http://imi.yuxming.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://fma.pengpengdd.cyou

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://ryv.nwbrower.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://bmr.xingfuxueyuan.xyz

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://wte.zhaomingkeji.xyz

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://qwj.jianghu66.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://gsr.c1oappe.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://nmv.yangfankeji.com

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://bap.hnqzz.top

[D26] 数组转字符串
来源：http://oke.jiagoushi.top

Py:   ", ".join(map(str, arr))
来源：http://xaz.haohaochexian.top

PHP:  implode(", ", $arr);
来源：http://oqm.nwbrower.top

JS:   arr.join(", ")
来源：http://upz.yvedp.cn

TS:   arr.join(", ")
来源：http://llq.guannengcc.top

Java: String.join(", ", list)
来源：http://bfe.ydzc1.top

Go:   strings.Join(strs, ", ")
来源：http://dan.gaohongyu789.top

Ruby: arr.join(", ")
来源：http://flh.shanyushiyangtech.top

C#:   string.Join(", ", list)
来源：http://exh.gzhubu.top

================================================================================
来源：http://ctu.sufxvd.cn

E. 字符串处理
来源：http://jrs.uphjek.com

================================================================================
来源：http://kcd.chenlongwang.top

[E01] 拼接字符串
来源：http://nog.nanxuanxn.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://wsb.uphjek.com

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://zfo.hywenlv.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://bnm.aizwys.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://xvx.yonumen.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://rlq.cqqwz.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://jsq.yuxming.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://ald.zhijiandao.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://pkp.nanxinkj.top

[E02] 重复字符串
来源：http://iqo.hnqzz.top

Py:   "ab" * 3
来源：http://dig.ivvv.top

PHP:  str_repeat("ab", 3);
来源：http://gpc.daxiang520.top

JS:   "ab".repeat(3)
来源：http://djg.xinyue.icu

TS:   "ab".repeat(3)
来源：http://grj.xylfe.cn

Java: "ab".repeat(3)
来源：http://xye.zhijiandao.cn

Go:   strings.Repeat("ab", 3)
来源：http://jag.vqdsnc.cn

Ruby: "ab" * 3
来源：http://gwx.fktsv.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://kjd.yfazqb.com

[E03] 截取子串
来源：http://xeh.tanke756.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://gnt.xuanzx.com

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://nho.zhijiandao.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hzm.zhoulong.xyz

TS:   s.slice(1, 4)
来源：http://kxp.yonumen.top

Java: s.substring(1, 4)
来源：http://zmz.shuidangran.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://add.gaohongyu789.top

Ruby: s[1, 3];  s[1..3]
来源：http://kwg.yuanzhike.top

C#:   s.Substring(1, 3)
来源：http://asr.ywan-chungtsiang.top

[E04] 查找子串位置
来源：http://gna.ydzc1.top

Py:   s.find("x");  s.index("x")
来源：http://lnl.zhijiandao.cn

PHP:  strpos($s, "x");
来源：http://sod.jyoumei.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://qbk.snrcjt.cn

TS:   s.indexOf("x")
来源：http://mmw.uphjek.com

Java: s.indexOf("x")
来源：http://lcr.aizwys.cn

Go:   strings.Index(s, "x")
来源：http://zir.ctjpmb.com

Ruby: s.index("x")
来源：http://cdw.redwolf501.top

C#:   s.IndexOf("x")
来源：http://nui.yuxming.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://afx.cheryme.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://ojl.tian-w.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://xdi.yuxming.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hyc.guowangkeji.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://crc.yuanzhike.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mjb.tanke756.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://iis.gzhubu.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://mrr.pengpengdd.cyou

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://mon.mhx1999.top

[E06] 替换子串
来源：http://rqd.fzhhl.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://goq.andypj.xyz

PHP:  str_replace("a", "b", $s);
来源：http://ygo.daria6918.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://vuj.fehbvm.com

TS:   s.replaceAll("a", "b")
来源：http://nmu.jlsjyb.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ksn.shanyushiyangkeji.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://wyv.yvedp.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://gdc.ehwqpu.com

C#:   s.Replace("a", "b")
来源：http://kmg.shangyingyoupin.top

[E07] 按分隔符拆分
来源：http://det.mhx1999.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://jlw.yangfankeji.com

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://ujw.bjfxy.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://duc.guannengcc.top

TS:   s.split(",")
来源：http://kcj.feifeiyinyue.top

Java: s.split(",");  s.split("\\s+")
来源：http://mfu.snrcjt.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://omo.fehbvm.com

Ruby: s.split(",");  s.split
来源：http://jzb.snrcjt.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://zgs.xziqi.cn

[E08] 数组按分隔符合并
来源：http://pqp.hammf.cn

Py:   ",".join(items)
来源：http://dmi.gzhubu.top

PHP:  implode(",", $items);
来源：http://upf.jianghu66.top

JS:   items.join(",")
来源：http://eqy.9152youxi.cn

TS:   items.join(",")
来源：http://ayw.dashuyun.cn

Java: String.join(",", items)
来源：http://eam.hnxiangtu.top

Go:   strings.Join(items, ",")
来源：http://lzx.ydzc1.top

Ruby: items.join(",")
来源：http://bnr.andypj.xyz

C#:   string.Join(",", items)
来源：http://qmq.dashuyun.cn

[E09] 去除所有空白字符
来源：http://oxx.shuidangran.top


<!-- 参考信息 -->