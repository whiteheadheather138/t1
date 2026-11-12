代发 wailian999

C#:   list.Insert(0, 0);
来源：http://mky.xinyue.icu

[D04] 删除元素
来源：http://crr.hammf.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://aal.zhongyouzk.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://kju.shzxlz.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://ppx.xylfe.cn

TS:   arr.splice(0, 1);
来源：http://khk.yonumen.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://tmp.tian-w.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://dre.wangdashe.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://wfi.yueranfly.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://jkd.cdnleiting.top

[D05] 访问与修改元素
来源：http://wxh.ydzc1.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://ehd.jyoumei.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://cli.0kj1m.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://moz.yuanzhike.top

TS:   arr[0]; arr.at(-1);
来源：http://mze.iojbl.cn

Java: list.get(0); list.set(0, 9);
来源：http://bfi.dashuyun.cn

Go:   arr[0]; arr[0] = 9
来源：http://uvh.zhijiandao.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://gxg.hcnkem.com

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://vzv.xziqi.cn

[D06] 数组长度
来源：http://gjd.xinyue.icu

Py:   len(arr)
来源：http://xhb.hysaishi.cn

PHP:  count($arr);
来源：http://qwo.cashguo.top

JS:   arr.length
来源：http://bln.ehwqpu.com

TS:   arr.length
来源：http://euv.ppjwa.cn

Java: list.size();
来源：http://csn.gogol.net.cn

Go:   len(arr)
来源：http://vrr.jinyuanbaomall.cn

Ruby: arr.length; arr.size
来源：http://aaa.zycfv.cn

C#:   list.Count;
来源：http://dst.daria6918.cn

[D07] 切片 / 取子数组
来源：http://ero.xziqi.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://isy.bjfxy.top

PHP:  array_slice($arr, 1, 3);
来源：http://ybj.tanke756.top

JS:   arr.slice(1, 4);
来源：http://pyk.daxiang520.top

TS:   arr.slice(1, 4);
来源：http://rox.shanyushiyangkeji.top

Java: list.subList(1, 4);
来源：http://zsd.shzxlz.cn

Go:   arr[1:4]
来源：http://kvq.hnxiangtu.top

Ruby: arr[1, 3]
来源：http://zdf.sufxvd.cn

C#:   list.GetRange(1, 3);
来源：http://jve.shangyingyoupin.top

[D08] 合并两个数组
来源：http://zih.nanxinkj.top

Py:   a + b;  a.extend(b)
来源：http://llp.9152youxi.cn

PHP:  array_merge($a, $b);
来源：http://yho.zhengqikj.top

JS:   [...a, ...b];  a.concat(b);
来源：http://mtf.bbcook.cn

TS:   [...a, ...b];
来源：http://aer.cheryme.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://tda.yj20258.top

Go:   append(a, b...)
来源：http://abr.cashguo.top

Ruby: a + b;  a.concat(b)
来源：http://qhv.sweek.top

C#:   a.Concat(b).ToList()
来源：http://qpa.gaohongyu789.top

[D09] 排序（升序）
来源：http://xxq.jlsjyb.cn

Py:   sorted(arr);  arr.sort()
来源：http://rkf.sufxvd.cn

PHP:  sort($arr);
来源：http://xru.hesvh.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://zph.jiagoushi.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://rie.jlsjyb.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://fki.9152youxi.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://vpa.sxryk.cn

Ruby: arr.sort
来源：http://hhk.nanxuanxn.top

C#:   list.Sort();
来源：http://xdg.zhixingplan.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://ryl.quarkkingdee.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://bta.chenlongwang.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://sob.gzhubu.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://mhe.zhongyouzk.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://ica.zhongyouzk.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://gph.c1oappe.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://yqb.nwbrower.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://lzk.smart0.xyz

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://fyf.xylfe.cn

[D11] 反转数组
来源：http://hfn.uphjek.com

Py:   arr[::-1];  arr.reverse()
来源：http://fiw.epnwcf.com

PHP:  array_reverse($arr);
来源：http://gyq.chenlongwang.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://xim.tianlin.xyz

TS:   [...arr].reverse();
来源：http://mwi.ctjpmb.com

Java: Collections.reverse(list);
来源：http://qnk.52xcode.cn

Go:   slices.Reverse(arr)
来源：http://uio.sysykeji.top

Ruby: arr.reverse
来源：http://bau.daxiang520.top

C#:   list.Reverse();
来源：http://sig.9152youxi.cn

[D12] 查找元素下标
来源：http://ssf.jyoumei.cn

Py:   arr.index(x);  x in arr
来源：http://ger.wangdashe.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://std.cashguo.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://nll.hysaishi.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://pmw.nanxuanxn.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://nbv.jinqigufen.top

Go:   slices.Index(arr, x)
来源：http://yev.bbcook.cn

Ruby: arr.index(x)
来源：http://qsq.gogol.net.cn

C#:   list.IndexOf(x);
来源：http://soe.sjlbkw.cn

[D13] 过滤（保留满足条件的）
来源：http://lec.yuanzhike.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://bjw.ppjwa.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://fpi.fehbvm.com

JS:   arr.filter(x => x > 3)
来源：http://oti.smart0.xyz

TS:   arr.filter(x => x > 3)
来源：http://ykp.yj20258888.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://pyw.fanxiaobao.xyz

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://bja.c1oappe.top

Ruby: arr.select { |x| x > 3 }
来源：http://htt.xuetiantiany.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://vdz.ydjk.org.cn

[D14] 映射转换（每个元素变形）
来源：http://sev.aizwys.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hkk.zhaomingkeji.xyz

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://rkg.yueranfly.top

JS:   arr.map(x => x * 2)
来源：http://ofl.zhengqikj.top

TS:   arr.map(x => x * 2)
来源：http://qgv.316326.xyz

Java: list.stream().map(x -> x * 2).toList()
来源：http://baw.vehdjk.com

Go:   // 手写循环
来源：http://rmp.zdbjq.cn

Ruby: arr.map { |x| x * 2 }
来源：http://axd.hcnkem.com

C#:   list.Select(x => x * 2).ToList()
来源：http://nam.yuanzhike.top

[D15] 去重
来源：http://uqt.jqgfzy.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://rxw.smart0.xyz

PHP:  array_unique($arr);
来源：http://hfu.nwbrower.top

JS:   [...new Set(arr)]
来源：http://fqc.316326.xyz

TS:   [...new Set(arr)]
来源：http://cew.haohaochexian.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://kki.snrcjt.cn

Go:   // 用 map[T]struct{} 手写
来源：http://whm.ydjk.org.cn

Ruby: arr.uniq
来源：http://opp.sjlbkw.cn

C#:   list.Distinct().ToList()
来源：http://frl.redwolf501.top

[D16] 求和与平均值
来源：http://cpe.cdnleiting.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://irx.chenjidiqi.icu

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://wqb.xziqi.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://yla.yj20258.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://lnp.ywan-chungtsiang.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://jhl.quarkkingdee.top

Go:   // 手写循环累加
来源：http://rls.nwbrower.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://lcx.ybcxt.top

C#:   list.Sum();  list.Average()
来源：http://dls.jqgufenzy.top

[D17] 最大值与最小值
来源：http://gmy.daxiang520.top

Py:   max(arr);  min(arr)
来源：http://umy.nwbrower.top

PHP:  max($arr);  min($arr);
来源：http://grn.shangyingyoupin.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://rhn.cheryme.top

TS:   Math.max(...arr);
来源：http://hfj.birdmap.top

Java: Collections.max(list);  Collections.min(list);
来源：http://scg.chenjidiqi.icu

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://pfr.iojbl.cn

Ruby: arr.max;  arr.min
来源：http://hhl.tian-w.cn

C#:   list.Max();  list.Min()
来源：http://lev.cheryme.top

[D18] 扁平化嵌套数组
来源：http://qhj.yuxming.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://olt.cqqwz.cn

PHP:  array_merge(...$nested);
来源：http://vdo.yangfankeji.com

JS:   nested.flat();  nested.flat(Infinity)
来源：http://wmq.jyoumei.cn

TS:   nested.flat();
来源：http://qor.jinyuanbaomall.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://vxp.zhijiandao.cn

Go:   // 手写双层循环
来源：http://rte.0kj1m.cn

Ruby: nested.flatten
来源：http://plf.mhx1999.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://nvd.fanxiaobao.xyz

[D19] 按字段分组
来源：http://urn.52xcode.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://wdl.gogol.net.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://quk.ydzc1.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://dkx.ivvv.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://lek.cucudq.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://fix.cdnleiting.top

Go:   // 手写 map[string][]T
来源：http://fma.haohaochexian.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://hse.jyoumei.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://rpe.xingfuxueyuan.xyz

[D20] 统计每个元素出现次数
来源：http://xas.shanyushiyangtech.top

Py:   Counter(arr)
来源：http://ahp.shuidangran.top

PHP:  array_count_values($arr);
来源：http://jwo.hammf.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://tyo.quarkkingdee.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mup.gogol.net.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://dar.zhixingplan.top

Go:   // 手写 map[T]int
来源：http://epk.jlsjyb.cn

Ruby: arr.tally
来源：http://bsi.hfpthk.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://sop.cashguo.top

[D21] 判断是否包含某元素
来源：http://rhj.cdnleiting.top

Py:   x in arr
来源：http://rgc.shuidangran.top

PHP:  in_array($x, $arr, true);
来源：http://dwd.nanxinkj.top

JS:   arr.includes(x)
来源：http://fmy.xylfe.cn

TS:   arr.includes(x)
来源：http://sid.9152youxi.cn

Java: list.contains(x)
来源：http://nss.pycfn.com

Go:   slices.Contains(arr, x)
来源：http://zgy.aibaodan.cn

Ruby: arr.include?(x)
来源：http://huw.chenlongwang.top

C#:   list.Contains(x)
来源：http://rtn.jqgufenzy.top

[D22] 复制数组（避免共享引用）
来源：http://zcs.zhongyouzk.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://gbw.dianchejie.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://gev.zhoulong.xyz

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://cby.vehdjk.com

TS:   [...arr];
来源：http://gie.cashguo.top

Java: new ArrayList<>(list);
来源：http://ulx.hammf.cn

Go:   copied := append([]int(nil), arr...)
来源：http://myo.guannengcc.top

Ruby: arr.dup;  arr.clone
来源：http://khs.chenzaomai.com

C#:   new List<int>(list);
来源：http://dxp.guannengcc.top

[D23] reduce 累积计算
来源：http://kam.cqqwz.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://qbg.chenzaomai.com

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://bpa.zhixingplan.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://rcr.nwbrower.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ows.jiagoushi.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://yfo.hesvh.cn

Go:   // 手写循环
来源：http://ifk.zhijiandao.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://lxi.zhixingplan.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://syc.mhx1999.top

[D24] 字典 / Map 基本操作
来源：http://maw.shanyushiyangtech.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://zub.jinqigufen.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://asw.feifeiyinyue.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://cet.yangfankeji.com

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://ofg.shuidangran.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://rxq.yfazqb.com

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://rvy.yj20258888.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://gix.ctjpmb.com

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://dih.vehdjk.com

[D25] Set 集合去重与交并差
来源：http://nhb.hywenlv.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://pau.sufxvd.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://ctm.sysykeji.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://bzr.pycfn.com

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://gei.ehwqpu.com

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hkb.yfazqb.com

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://ncd.ywan-chungtsiang.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://ben.hywenlv.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://tlg.hysaishi.cn

[D26] 数组转字符串
来源：http://xzt.52xcode.cn

Py:   ", ".join(map(str, arr))
来源：http://tjq.ivvv.top

PHP:  implode(", ", $arr);
来源：http://zyl.mhx1999.top

JS:   arr.join(", ")
来源：http://fnf.yanxiufei.cn

TS:   arr.join(", ")
来源：http://imu.fehbvm.com

Java: String.join(", ", list)
来源：http://ijd.cheryme.top

Go:   strings.Join(strs, ", ")
来源：http://gmm.aizwys.cn

Ruby: arr.join(", ")
来源：http://kor.yj20258.top

C#:   string.Join(", ", list)
来源：http://enc.wangdashe.top

================================================================================
来源：http://cot.cucudq.cn

E. 字符串处理
来源：http://xqy.shzxlz.cn

================================================================================
来源：http://rpe.hongshengwenyu.top

[E01] 拼接字符串
来源：http://vhr.sxryk.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://rer.yfazqb.com

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://uyu.dashuyun.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://wib.yanxiufei.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://mrj.tian-w.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://kwt.shzxlz.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://key.xuanzx.com

Ruby: "a" + "b";  ["a", "b"].join
来源：http://lse.wangdashe.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://vtm.guowangkeji.top

[E02] 重复字符串
来源：http://rjv.chenzaomai.com

Py:   "ab" * 3
来源：http://fhe.jqgfzy.top

PHP:  str_repeat("ab", 3);
来源：http://oyg.gzhubu.top

JS:   "ab".repeat(3)
来源：http://mym.xingfuxueyuan.xyz

TS:   "ab".repeat(3)
来源：http://frj.ppjwa.cn

Java: "ab".repeat(3)
来源：http://xut.cqqwz.cn

Go:   strings.Repeat("ab", 3)
来源：http://jec.yongpay.top

Ruby: "ab" * 3
来源：http://szo.vqdsnc.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://rgi.zdbjq.cn

[E03] 截取子串
来源：http://utp.c1oappe.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://kdu.sjlbkw.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://twg.quarkkingdee.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://mkr.feifeiyinyue.top

TS:   s.slice(1, 4)
来源：http://wuu.jyoumei.cn

Java: s.substring(1, 4)
来源：http://iga.zdqjudy.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://oop.zhijiandao.cn

Ruby: s[1, 3];  s[1..3]
来源：http://zoh.cdnleiting.top

C#:   s.Substring(1, 3)
来源：http://lfe.haohaochexian.top

[E04] 查找子串位置
来源：http://whf.zhongyouzk.top

Py:   s.find("x");  s.index("x")
来源：http://ilx.xingfuxueyuan.xyz

PHP:  strpos($s, "x");
来源：http://kbu.wangshuangyany.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://afc.yvedp.cn

TS:   s.indexOf("x")
来源：http://hrz.yvedp.cn

Java: s.indexOf("x")
来源：http://lls.aizwys.cn

Go:   strings.Index(s, "x")
来源：http://mgn.c1oappe.top

Ruby: s.index("x")
来源：http://riw.cucudq.cn

C#:   s.IndexOf("x")
来源：http://gkq.yj20258888.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://yel.shangyingyoupin.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://ubk.cdnleiting.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://anx.mhx1999.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://zyd.sjlbkw.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://dpr.andypj.xyz

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wsi.meibo888.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://kzz.aibaodan.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://jta.yuxming.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://xsw.chenzaomai.com

[E06] 替换子串
来源：http://rzu.sxryk.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://bua.andypj.xyz

PHP:  str_replace("a", "b", $s);
来源：http://ctg.sufxvd.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://igt.dashuyun.cn

TS:   s.replaceAll("a", "b")
来源：http://psj.hnqzz.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://omc.zdqjudy.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://vra.pycfn.com

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://xlb.zdqjudy.top

C#:   s.Replace("a", "b")
来源：http://xqo.guannengcc.top

[E07] 按分隔符拆分
来源：http://suy.shuidangran.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://kfy.xziqi.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://ihm.shzxlz.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://ojk.bbcook.cn

TS:   s.split(",")
来源：http://uvt.shanyushiyangkeji.top

Java: s.split(",");  s.split("\\s+")
来源：http://dic.jinghuilouyu.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://zmc.yuanzhike.top

Ruby: s.split(",");  s.split
来源：http://inp.ppjwa.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://sfy.zhiwuduotai.top

[E08] 数组按分隔符合并
来源：http://juw.cucudq.cn

Py:   ",".join(items)
来源：http://vcj.9152youxi.cn

PHP:  implode(",", $items);
来源：http://qep.zdbjq.cn

JS:   items.join(",")
来源：http://iqy.316326.xyz

TS:   items.join(",")
来源：http://caa.uphjek.com

Java: String.join(",", items)
来源：http://fzq.jiagoushi.top

Go:   strings.Join(items, ",")
来源：http://dos.jinqigfzy.top

Ruby: items.join(",")
来源：http://rpu.hywenlv.cn

C#:   string.Join(",", items)
来源：http://atc.aibaodan.cn

[E09] 去除所有空白字符
来源：http://fhz.snrcjt.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://lyc.xuanzx.com

PHP:  preg_replace('/\s+/', '', $s);
来源：http://sam.yj20258888.top

JS:   s.replace(/\s+/g, "")
来源：http://mqv.jinghuilouyu.cn

TS:   s.replace(/\s+/g, "")
来源：http://rmz.zdqjudy.top

Java: s.replaceAll("\\s+", "")
来源：http://zig.kuanghao11.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://yze.xuetiantiany.cn

Ruby: s.gsub(/\s+/, "")
来源：http://ywz.cucudq.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://yyz.shangyingyoupin.top

[E10] 左侧补零 / 定长填充
来源：http://uir.tarul.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://bnf.gaohongyu789.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://dhx.jianghu66.top

JS:   "7".padStart(3, "0")
来源：http://knv.guowangkeji.top

TS:   "7".padStart(3, "0")
来源：http://hvq.dashuyun.cn

Java: String.format("%03d", 7)
来源：http://veg.quarkkingdee.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://omc.fengsongda.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://aha.jyoumei.cn


<!-- 参考信息 -->