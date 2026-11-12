代发 wailian999

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://ius.bjfxy.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://ilt.shanyushiyangkeji.top

[D05] 访问与修改元素
来源：http://dxh.redwolf501.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://zxz.yj20258888.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://epb.tian-w.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://rsw.haohaochexian.top

TS:   arr[0]; arr.at(-1);
来源：http://pfn.fzhhl.top

Java: list.get(0); list.set(0, 9);
来源：http://imt.316326.xyz

Go:   arr[0]; arr[0] = 9
来源：http://lcm.xuanzx.com

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://est.jiagoushi.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://sui.tarul.cn

[D06] 数组长度
来源：http://thn.pengpengdd.cyou

Py:   len(arr)
来源：http://cim.zdbjq.cn

PHP:  count($arr);
来源：http://wgg.ppjwa.cn

JS:   arr.length
来源：http://vkd.ppjwa.cn

TS:   arr.length
来源：http://pvn.hnqzz.top

Java: list.size();
来源：http://obs.sysykeji.top

Go:   len(arr)
来源：http://low.fehbvm.com

Ruby: arr.length; arr.size
来源：http://chn.cucudq.cn

C#:   list.Count;
来源：http://htk.hysaishi.cn

[D07] 切片 / 取子数组
来源：http://moe.cheryme.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://iiz.cheryme.top

PHP:  array_slice($arr, 1, 3);
来源：http://kdj.kuanghao11.cn

JS:   arr.slice(1, 4);
来源：http://lxi.zdqjudy.top

TS:   arr.slice(1, 4);
来源：http://jpj.havefunace.top

Java: list.subList(1, 4);
来源：http://uju.ivvv.top

Go:   arr[1:4]
来源：http://olt.ybcxt.top

Ruby: arr[1, 3]
来源：http://zxn.316326.xyz

C#:   list.GetRange(1, 3);
来源：http://oil.ydjk.org.cn

[D08] 合并两个数组
来源：http://ror.ppjwa.cn

Py:   a + b;  a.extend(b)
来源：http://gbc.shuidangran.top

PHP:  array_merge($a, $b);
来源：http://gix.yuanzhike.top

JS:   [...a, ...b];  a.concat(b);
来源：http://caf.svipenyu.cn

TS:   [...a, ...b];
来源：http://iuw.gaohongyu789.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://xnw.vqdsnc.cn

Go:   append(a, b...)
来源：http://usz.shzxlz.cn

Ruby: a + b;  a.concat(b)
来源：http://vxa.shuidangran.top

C#:   a.Concat(b).ToList()
来源：http://hma.0kj1m.cn

[D09] 排序（升序）
来源：http://qdl.pengpengdd.cyou

Py:   sorted(arr);  arr.sort()
来源：http://ohm.sjlbkw.cn

PHP:  sort($arr);
来源：http://ebx.shangyingyoupin.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://mdb.quarkkingdee.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://vcs.mhx1999.top

Java: Collections.sort(list);  list.sort(null);
来源：http://anf.daria6918.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://uwk.fanxiaobao.xyz

Ruby: arr.sort
来源：http://umr.zhongyouzk.top

C#:   list.Sort();
来源：http://vqn.daxiang520.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://aep.xuetiantiany.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://shx.ywan-chungtsiang.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://eam.sufxvd.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://xxw.sweek.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://esc.hcnkem.com

Java: list.sort(Comparator.comparing(Person::age));
来源：http://eec.zhengqikj.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://cna.yangfankeji.com

Ruby: arr.sort_by { |x| x[:age] }
来源：http://lcq.jinqigfzy.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://wfg.sufxvd.cn

[D11] 反转数组
来源：http://oay.nwbrower.top

Py:   arr[::-1];  arr.reverse()
来源：http://fhc.aizwys.cn

PHP:  array_reverse($arr);
来源：http://vxz.tarul.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://bud.andypj.xyz

TS:   [...arr].reverse();
来源：http://asb.nanxuanxn.top

Java: Collections.reverse(list);
来源：http://jyz.gzhubu.top

Go:   slices.Reverse(arr)
来源：http://dhb.hywenlv.cn

Ruby: arr.reverse
来源：http://auf.zhengqikj.top

C#:   list.Reverse();
来源：http://psz.jinqigufen.top

[D12] 查找元素下标
来源：http://ixp.bjfxy.top

Py:   arr.index(x);  x in arr
来源：http://pxl.jqgfzy.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://tyu.yuxming.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://nna.shangyingyoupin.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://sje.jyoumei.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://rki.aibaodan.cn

Go:   slices.Index(arr, x)
来源：http://ufd.yuanzhike.top

Ruby: arr.index(x)
来源：http://arf.wangshuangyany.cn

C#:   list.IndexOf(x);
来源：http://irj.shanyushiyangkeji.top

[D13] 过滤（保留满足条件的）
来源：http://bfa.hfpthk.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hph.guannengcc.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://oyp.andypj.xyz

JS:   arr.filter(x => x > 3)
来源：http://xfg.hnqzz.top

TS:   arr.filter(x => x > 3)
来源：http://qzs.yj20258.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://czb.jinqigfzy.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://dke.dashuyun.cn

Ruby: arr.select { |x| x > 3 }
来源：http://hxp.nanxuanxn.top

C#:   list.Where(x => x > 3).ToList()
来源：http://yes.zhiwuduotai.top

[D14] 映射转换（每个元素变形）
来源：http://oyl.shuidangran.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://lxm.shuidangran.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://haq.wangdashe.top

JS:   arr.map(x => x * 2)
来源：http://nmz.jiagoushi.top

TS:   arr.map(x => x * 2)
来源：http://aep.iojbl.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://bkm.vehdjk.com

Go:   // 手写循环
来源：http://dzg.sysykeji.top

Ruby: arr.map { |x| x * 2 }
来源：http://bkh.tianlin.xyz

C#:   list.Select(x => x * 2).ToList()
来源：http://zit.tianlin.xyz

[D15] 去重
来源：http://qdd.52xcode.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://fgi.svipenyu.cn

PHP:  array_unique($arr);
来源：http://arp.shanyushiyangtech.top

JS:   [...new Set(arr)]
来源：http://fhq.ehwqpu.com

TS:   [...new Set(arr)]
来源：http://jil.zhiwuduotai.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://lbb.haohaochexian.top

Go:   // 用 map[T]struct{} 手写
来源：http://grl.cheryme.top

Ruby: arr.uniq
来源：http://dzr.wangshuangyany.cn

C#:   list.Distinct().ToList()
来源：http://zce.52xcode.cn

[D16] 求和与平均值
来源：http://zcf.uphjek.com

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://dul.yuanzhike.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://afp.shanyushiyangtech.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://kgd.pycfn.com

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://vru.feifeiyinyue.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hqr.hcnkem.com

Go:   // 手写循环累加
来源：http://fjs.jinghuilouyu.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://ooa.zhaomingkeji.xyz

C#:   list.Sum();  list.Average()
来源：http://hjg.shanyushiyangkeji.top

[D17] 最大值与最小值
来源：http://ook.shanyushiyangkeji.top

Py:   max(arr);  min(arr)
来源：http://zlp.gotoacloud.top

PHP:  max($arr);  min($arr);
来源：http://ueb.cucudq.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://lyt.yongpay.top

TS:   Math.max(...arr);
来源：http://tov.hesvh.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://rmj.hysaishi.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://iop.fktsv.cn

Ruby: arr.max;  arr.min
来源：http://hyr.xingfuxueyuan.xyz

C#:   list.Max();  list.Min()
来源：http://rhf.shanyushiyangkeji.top

[D18] 扁平化嵌套数组
来源：http://jxq.jqgufenzy.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://jbu.ydjk.org.cn

PHP:  array_merge(...$nested);
来源：http://ofs.yongpay.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://sqm.aizwys.cn

TS:   nested.flat();
来源：http://hfu.dashuyun.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://eoo.shangyingyoupin.top

Go:   // 手写双层循环
来源：http://ejs.xingfuxueyuan.xyz

Ruby: nested.flatten
来源：http://hxz.yongpay.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://gcu.cheryme.top

[D19] 按字段分组
来源：http://dwk.havefunace.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://plu.dashuyun.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://gsh.yvedp.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://xsm.kuanghao11.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://yqe.zhoulong.xyz

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://ypk.yfazqb.com

Go:   // 手写 map[string][]T
来源：http://ean.xuanzx.com

Ruby: arr.group_by { |x| x[:type] }
来源：http://vir.xuanzx.com

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://tnq.9152youxi.cn

[D20] 统计每个元素出现次数
来源：http://drn.ybcxt.top

Py:   Counter(arr)
来源：http://qdx.redwolf501.top

PHP:  array_count_values($arr);
来源：http://zkw.xylfe.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://aqr.feifeiyinyue.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://fmx.sysykeji.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://dol.jinyuanbaomall.cn

Go:   // 手写 map[T]int
来源：http://xct.nwbrower.top

Ruby: arr.tally
来源：http://tpw.fzhhl.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://mun.bjfxy.top

[D21] 判断是否包含某元素
来源：http://pyk.uphjek.com

Py:   x in arr
来源：http://ecs.pengpengdd.cyou

PHP:  in_array($x, $arr, true);
来源：http://wez.hammf.cn

JS:   arr.includes(x)
来源：http://rvz.sysykeji.top

TS:   arr.includes(x)
来源：http://hlb.sufxvd.cn

Java: list.contains(x)
来源：http://wxn.ybcxt.top

Go:   slices.Contains(arr, x)
来源：http://put.hywenlv.cn

Ruby: arr.include?(x)
来源：http://yzm.hammf.cn

C#:   list.Contains(x)
来源：http://hvu.gogol.net.cn

[D22] 复制数组（避免共享引用）
来源：http://kda.pycfn.com

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hsq.aizwys.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://rkq.ctjpmb.com

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://baf.yuanzhike.top

TS:   [...arr];
来源：http://glu.sxryk.cn

Java: new ArrayList<>(list);
来源：http://swf.sufxvd.cn

Go:   copied := append([]int(nil), arr...)
来源：http://haf.xziqi.cn

Ruby: arr.dup;  arr.clone
来源：http://oht.zdbjq.cn

C#:   new List<int>(list);
来源：http://rcn.jinyuanbaomall.cn

[D23] reduce 累积计算
来源：http://eeg.cdnleiting.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://sye.cucudq.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://jrl.316326.xyz

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wjb.hammf.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mvd.52xcode.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://nbv.ctjpmb.com

Go:   // 手写循环
来源：http://fzs.tian-w.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://jvb.yvedp.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://scr.yueranfly.top

[D24] 字典 / Map 基本操作
来源：http://mrf.sjlbkw.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://yjt.yueranfly.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://sim.hcnkem.com

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://vxa.zycfv.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://uae.xuanzx.com

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://bcc.vqdsnc.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://fgk.jiagoushi.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://kva.316326.xyz

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://fvd.0kj1m.cn

[D25] Set 集合去重与交并差
来源：http://rcs.havefunace.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://ofr.zhiwuduotai.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://ujk.hcnkem.com

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://auv.yuanzhike.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://pqo.cdnleiting.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://yym.sweek.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://oql.jinqigufen.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://kdi.ivvv.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://jgp.wangshuangyany.cn

[D26] 数组转字符串
来源：http://hlj.c1oappe.top

Py:   ", ".join(map(str, arr))
来源：http://nbs.316326.xyz

PHP:  implode(", ", $arr);
来源：http://kmi.iojbl.cn

JS:   arr.join(", ")
来源：http://ahp.redwolf501.top

TS:   arr.join(", ")
来源：http://xwq.iojbl.cn

Java: String.join(", ", list)
来源：http://low.sxryk.cn

Go:   strings.Join(strs, ", ")
来源：http://iaa.haohaochexian.top

Ruby: arr.join(", ")
来源：http://pcj.jqgfzy.top

C#:   string.Join(", ", list)
来源：http://fbb.yvedp.cn

================================================================================
来源：http://qdp.fzhhl.top

E. 字符串处理
来源：http://dai.xuetiantiany.cn

================================================================================
来源：http://wrm.ehwqpu.com

[E01] 拼接字符串
来源：http://wvb.guannengcc.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://jjr.redwolf501.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://cwm.pycfn.com

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://yhx.zhaomingkeji.xyz

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://wit.yuanzhike.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://jcf.mhx1999.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://nzk.pycfn.com

Ruby: "a" + "b";  ["a", "b"].join
来源：http://ski.ctjpmb.com

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://rcy.fehbvm.com

[E02] 重复字符串
来源：http://pog.jqgufenzy.top

Py:   "ab" * 3
来源：http://vub.vehdjk.com

PHP:  str_repeat("ab", 3);
来源：http://mqr.shzxlz.cn

JS:   "ab".repeat(3)
来源：http://gdf.dianchejie.cn

TS:   "ab".repeat(3)
来源：http://ucc.ywan-chungtsiang.top

Java: "ab".repeat(3)
来源：http://tdv.316326.xyz

Go:   strings.Repeat("ab", 3)
来源：http://dye.svipenyu.cn

Ruby: "ab" * 3
来源：http://juj.xuetiantiany.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://wsm.316326.xyz

[E03] 截取子串
来源：http://xlf.fehbvm.com

Py:   s[1:4];  s[:3];  s[3:]
来源：http://ekz.fzhhl.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://rqy.jinghuilouyu.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://vkt.fzhhl.top

TS:   s.slice(1, 4)
来源：http://bmg.xuanzx.com

Java: s.substring(1, 4)
来源：http://njh.cashguo.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://shn.hfpthk.cn

Ruby: s[1, 3];  s[1..3]
来源：http://gkh.hesvh.cn

C#:   s.Substring(1, 3)
来源：http://auy.daxiang520.top

[E04] 查找子串位置
来源：http://jyi.52xcode.cn

Py:   s.find("x");  s.index("x")
来源：http://ygh.yvedp.cn

PHP:  strpos($s, "x");
来源：http://svu.ydzc1.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://ljf.guowangkeji.top

TS:   s.indexOf("x")
来源：http://cab.kuanghao11.cn

Java: s.indexOf("x")
来源：http://jlb.sufxvd.cn

Go:   strings.Index(s, "x")
来源：http://jdp.meibo888.top

Ruby: s.index("x")
来源：http://ngp.dashuyun.cn

C#:   s.IndexOf("x")
来源：http://eoq.yj20258888.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://eaf.yuanzhike.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://sqb.jlsjyb.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://cgb.zycfv.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://tib.iojbl.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://ukc.tian-w.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://rop.bjfxy.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://ugb.andypj.xyz

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://ttj.aizwys.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://vxs.gaohongyu789.top

[E06] 替换子串
来源：http://dkx.zhengqikj.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://kko.ivvv.top

PHP:  str_replace("a", "b", $s);
来源：http://rbf.xinyue.icu

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://jag.zhongyouzk.top

TS:   s.replaceAll("a", "b")
来源：http://xqs.fzhhl.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://qpj.mhx1999.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://uac.zhaomingkeji.xyz

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://jpr.yongpay.top

C#:   s.Replace("a", "b")
来源：http://lft.meibo888.top

[E07] 按分隔符拆分
来源：http://hna.andypj.xyz

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://vmw.yanxiufei.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://zit.uphjek.com

JS:   s.split(",");  s.split(/\s+/)
来源：http://cux.pycfn.com

TS:   s.split(",")
来源：http://jdf.birdmap.top

Java: s.split(",");  s.split("\\s+")
来源：http://vsl.ydzc1.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://fhr.daxiang520.top

Ruby: s.split(",");  s.split
来源：http://oft.chenzaomai.com

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://cye.xuetiantiany.cn

[E08] 数组按分隔符合并
来源：http://zsz.pycfn.com

Py:   ",".join(items)
来源：http://cyi.nwbrower.top

PHP:  implode(",", $items);
来源：http://exv.hfpthk.cn

JS:   items.join(",")
来源：http://exl.jyoumei.cn

TS:   items.join(",")
来源：http://bbh.hongshengwenyu.top

Java: String.join(",", items)
来源：http://vkj.havefunace.top

Go:   strings.Join(items, ",")
来源：http://xzc.hnxiangtu.top

Ruby: items.join(",")
来源：http://mew.jinqigufen.top

C#:   string.Join(",", items)
来源：http://ukr.iojbl.cn

[E09] 去除所有空白字符
来源：http://zmj.xuetiantiany.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://bws.jqgufenzy.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://vnf.xinyue.icu

JS:   s.replace(/\s+/g, "")
来源：http://ocm.kuanghao11.cn

TS:   s.replace(/\s+/g, "")
来源：http://zyd.hfpthk.cn

Java: s.replaceAll("\\s+", "")
来源：http://iaf.xziqi.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://sfu.yonumen.top

Ruby: s.gsub(/\s+/, "")
来源：http://rwe.yvedp.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://ubv.daxiang520.top

[E10] 左侧补零 / 定长填充
来源：http://yrj.ppjwa.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://dvc.ctjpmb.com

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://gyz.zdqjudy.top

JS:   "7".padStart(3, "0")
来源：http://yux.zhongyouzk.top

TS:   "7".padStart(3, "0")
来源：http://hye.hfpthk.cn

Java: String.format("%03d", 7)
来源：http://wll.yj20258.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://jsm.fktsv.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://qfz.hcnkem.com

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://jcs.gotoacloud.top

[E11] 反转字符串
来源：http://pol.yj202588.top

Py:   s[::-1]
来源：http://qmn.jyoumei.cn

PHP:  strrev($s);
来源：http://hmd.iojbl.cn

JS:   [...s].reverse().join("")
来源：http://gpt.jqgufenzy.top

TS:   [...s].reverse().join("")
来源：http://ovb.daxiang520.top

Java: new StringBuilder(s).reverse().toString()
来源：http://vmo.svipenyu.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://xwa.chenlongwang.top


<!-- 参考信息 -->