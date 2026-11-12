代发 wailian999

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://ezq.gogol.net.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://zms.xuanzx.com

[D05] 访问与修改元素
来源：http://bxc.sweek.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://seo.aibaodan.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://nlv.gogol.net.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://ufz.kuanghao11.cn

TS:   arr[0]; arr.at(-1);
来源：http://gxf.birdmap.top

Java: list.get(0); list.set(0, 9);
来源：http://jyu.316326.xyz

Go:   arr[0]; arr[0] = 9
来源：http://jbl.jinghuilouyu.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://jor.hnxiangtu.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://bvv.cashguo.top

[D06] 数组长度
来源：http://jkf.shanyushiyangkeji.top

Py:   len(arr)
来源：http://ptj.ivvv.top

PHP:  count($arr);
来源：http://upi.ppjwa.cn

JS:   arr.length
来源：http://xkp.feifeiyinyue.top

TS:   arr.length
来源：http://trn.shuidangran.top

Java: list.size();
来源：http://qpm.sjlbkw.cn

Go:   len(arr)
来源：http://ucn.smart0.xyz

Ruby: arr.length; arr.size
来源：http://gfb.hnxiangtu.top

C#:   list.Count;
来源：http://tzv.xziqi.cn

[D07] 切片 / 取子数组
来源：http://xsf.ywan-chungtsiang.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://naf.sxryk.cn

PHP:  array_slice($arr, 1, 3);
来源：http://dhg.fktsv.cn

JS:   arr.slice(1, 4);
来源：http://pxm.tarul.cn

TS:   arr.slice(1, 4);
来源：http://loo.hywenlv.cn

Java: list.subList(1, 4);
来源：http://tfd.ppjwa.cn

Go:   arr[1:4]
来源：http://tzd.havefunace.top

Ruby: arr[1, 3]
来源：http://swi.xuanzx.com

C#:   list.GetRange(1, 3);
来源：http://hzf.jinqigufen.top

[D08] 合并两个数组
来源：http://zrm.yangfankeji.com

Py:   a + b;  a.extend(b)
来源：http://gzq.cqqwz.cn

PHP:  array_merge($a, $b);
来源：http://arh.vehdjk.com

JS:   [...a, ...b];  a.concat(b);
来源：http://kek.aibaodan.cn

TS:   [...a, ...b];
来源：http://nbi.hnqzz.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://wvw.bbcook.cn

Go:   append(a, b...)
来源：http://rhq.zycfv.cn

Ruby: a + b;  a.concat(b)
来源：http://dpl.tanke756.top

C#:   a.Concat(b).ToList()
来源：http://ray.xinyue.icu

[D09] 排序（升序）
来源：http://bqp.jinghuilouyu.cn

Py:   sorted(arr);  arr.sort()
来源：http://rvb.fengsongda.top

PHP:  sort($arr);
来源：http://zts.hywenlv.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://onx.ivvv.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://oew.vqdsnc.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://apw.chenlongwang.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://zss.tanke756.top

Ruby: arr.sort
来源：http://kes.ydzc1.top

C#:   list.Sort();
来源：http://qlu.fanxiaobao.xyz

[D10] 自定义排序（按字段 / 多条件）
来源：http://ipk.sufxvd.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hpn.sweek.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://yap.zdqjudy.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://yhh.havefunace.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://xzd.gzhubu.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://jmc.hysaishi.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://rbm.haohaochexian.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://rjj.jqgfzy.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://cgc.fktsv.cn

[D11] 反转数组
来源：http://tef.hysaishi.cn

Py:   arr[::-1];  arr.reverse()
来源：http://vch.shuidangran.top

PHP:  array_reverse($arr);
来源：http://ukd.ybcxt.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://pvg.chenlongwang.top

TS:   [...arr].reverse();
来源：http://uiw.xinyue.icu

Java: Collections.reverse(list);
来源：http://fnf.wangdashe.top

Go:   slices.Reverse(arr)
来源：http://lgq.tarul.cn

Ruby: arr.reverse
来源：http://wkk.yongpay.top

C#:   list.Reverse();
来源：http://igf.andypj.xyz

[D12] 查找元素下标
来源：http://spd.zhixingplan.top

Py:   arr.index(x);  x in arr
来源：http://yet.smart0.xyz

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://ycg.yuanzhike.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://acf.pengpengdd.cyou

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wad.zhengqikj.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://ryn.jinyuanbaomall.cn

Go:   slices.Index(arr, x)
来源：http://mub.nanxinkj.top

Ruby: arr.index(x)
来源：http://wgd.yj202588.top

C#:   list.IndexOf(x);
来源：http://cle.cqqwz.cn

[D13] 过滤（保留满足条件的）
来源：http://une.shzxlz.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://idn.snrcjt.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://uky.nanxuanxn.top

JS:   arr.filter(x => x > 3)
来源：http://qld.nwbrower.top

TS:   arr.filter(x => x > 3)
来源：http://fwx.yueranfly.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://nmp.yangfankeji.com

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://thn.fehbvm.com

Ruby: arr.select { |x| x > 3 }
来源：http://vok.vqdsnc.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://ndj.ehwqpu.com

[D14] 映射转换（每个元素变形）
来源：http://krk.yvedp.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://vhl.pengpengdd.cyou

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://ard.zhixingplan.top

JS:   arr.map(x => x * 2)
来源：http://qmm.cashguo.top

TS:   arr.map(x => x * 2)
来源：http://oig.nanxuanxn.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://bjv.cheryme.top

Go:   // 手写循环
来源：http://loh.52xcode.cn

Ruby: arr.map { |x| x * 2 }
来源：http://kts.jqgufenzy.top

C#:   list.Select(x => x * 2).ToList()
来源：http://yka.hywenlv.cn

[D15] 去重
来源：http://svh.xinyue.icu

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://gvg.yj20258.top

PHP:  array_unique($arr);
来源：http://qgq.smart0.xyz

JS:   [...new Set(arr)]
来源：http://koy.xylfe.cn

TS:   [...new Set(arr)]
来源：http://szg.yuanzhike.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://dln.hcnkem.com

Go:   // 用 map[T]struct{} 手写
来源：http://eot.sufxvd.cn

Ruby: arr.uniq
来源：http://kul.zdbjq.cn

C#:   list.Distinct().ToList()
来源：http://bah.xuetiantiany.cn

[D16] 求和与平均值
来源：http://get.shuidangran.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://ixk.cheryme.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://rhk.jinqigufen.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://yhf.hammf.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://rgw.fengsongda.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://ehf.zhoulong.xyz

Go:   // 手写循环累加
来源：http://iww.0kj1m.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://ubc.sysykeji.top

C#:   list.Sum();  list.Average()
来源：http://aje.ydzc1.top

[D17] 最大值与最小值
来源：http://dpk.bjfxy.top

Py:   max(arr);  min(arr)
来源：http://irr.yvedp.cn

PHP:  max($arr);  min($arr);
来源：http://ypq.zhoulong.xyz

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://rxf.yj20258888.top

TS:   Math.max(...arr);
来源：http://omw.sysykeji.top

Java: Collections.max(list);  Collections.min(list);
来源：http://zzb.jqgfzy.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://dbr.meibo888.top

Ruby: arr.max;  arr.min
来源：http://vrd.ehwqpu.com

C#:   list.Max();  list.Min()
来源：http://dpm.pycfn.com

[D18] 扁平化嵌套数组
来源：http://uyn.yj20258.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://vff.shzxlz.cn

PHP:  array_merge(...$nested);
来源：http://jgz.jiagoushi.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://xcj.daria6918.cn

TS:   nested.flat();
来源：http://sti.cheryme.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://yry.gogol.net.cn

Go:   // 手写双层循环
来源：http://fgi.tian-w.cn

Ruby: nested.flatten
来源：http://fde.nanxuanxn.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://kvz.hammf.cn

[D19] 按字段分组
来源：http://jtg.0kj1m.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://mwh.xziqi.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://lgx.xuetiantiany.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://nrb.birdmap.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://zev.kuanghao11.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://nsk.sjlbkw.cn

Go:   // 手写 map[string][]T
来源：http://vpi.guowangkeji.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://yri.yvedp.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://ixh.iojbl.cn

[D20] 统计每个元素出现次数
来源：http://gef.feifeiyinyue.top

Py:   Counter(arr)
来源：http://xwf.ehwqpu.com

PHP:  array_count_values($arr);
来源：http://pyu.shanyushiyangtech.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://juh.hongshengwenyu.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ljt.ybcxt.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://ajz.yuxming.cn

Go:   // 手写 map[T]int
来源：http://jml.svipenyu.cn

Ruby: arr.tally
来源：http://ziq.uphjek.com

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://jyx.yuanzhike.top

[D21] 判断是否包含某元素
来源：http://leb.nanxuanxn.top

Py:   x in arr
来源：http://qdz.c1oappe.top

PHP:  in_array($x, $arr, true);
来源：http://lot.ehwqpu.com

JS:   arr.includes(x)
来源：http://ggk.gotoacloud.top

TS:   arr.includes(x)
来源：http://bzk.wangshuangyany.cn

Java: list.contains(x)
来源：http://ija.jqgufenzy.top

Go:   slices.Contains(arr, x)
来源：http://nul.redwolf501.top

Ruby: arr.include?(x)
来源：http://wzv.yueranfly.top

C#:   list.Contains(x)
来源：http://stp.c1oappe.top

[D22] 复制数组（避免共享引用）
来源：http://yjy.epnwcf.com

Py:   arr.copy();  arr[:];  list(arr)
来源：http://sat.iojbl.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://doo.quarkkingdee.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hhx.fzhhl.top

TS:   [...arr];
来源：http://iox.yj20258.top

Java: new ArrayList<>(list);
来源：http://dhy.0kj1m.cn

Go:   copied := append([]int(nil), arr...)
来源：http://dsu.ppjwa.cn

Ruby: arr.dup;  arr.clone
来源：http://gia.tianlin.xyz

C#:   new List<int>(list);
来源：http://vqr.svipenyu.cn

[D23] reduce 累积计算
来源：http://tws.xingfuxueyuan.xyz

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://aua.jinqigfzy.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://lys.cheryme.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://flk.zycfv.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://tfv.jinghuilouyu.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://rgu.guowangkeji.top

Go:   // 手写循环
来源：http://uot.hcnkem.com

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://ubf.ctjpmb.com

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://mpu.zycfv.cn

[D24] 字典 / Map 基本操作
来源：http://ozt.ehwqpu.com

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://lmn.xziqi.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://eez.yj202588.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://ond.quarkkingdee.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://kix.uphjek.com

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://tre.gaohongyu789.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://dqc.dashuyun.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://cql.bbcook.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://xuk.sufxvd.cn

[D25] Set 集合去重与交并差
来源：http://tbf.xuanzx.com

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://ici.cucudq.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://gvi.ppjwa.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://zur.ivvv.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://kip.ivvv.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://ytv.hnxiangtu.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://zpp.tianlin.xyz

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://oww.yvedp.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hsj.tanke756.top

[D26] 数组转字符串
来源：http://gbe.kuanghao11.cn

Py:   ", ".join(map(str, arr))
来源：http://kew.haohaochexian.top

PHP:  implode(", ", $arr);
来源：http://gkl.zhongyouzk.top

JS:   arr.join(", ")
来源：http://gvc.316326.xyz

TS:   arr.join(", ")
来源：http://thv.havefunace.top

Java: String.join(", ", list)
来源：http://tge.hywenlv.cn

Go:   strings.Join(strs, ", ")
来源：http://sib.chenzaomai.com

Ruby: arr.join(", ")
来源：http://hko.cheryme.top

C#:   string.Join(", ", list)
来源：http://cag.hysaishi.cn

================================================================================
来源：http://ohs.yvedp.cn

E. 字符串处理
来源：http://flc.nwbrower.top

================================================================================
来源：http://usv.zhaomingkeji.xyz

[E01] 拼接字符串
来源：http://kkp.jlsjyb.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://mmd.jinqigufen.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://dzg.shzxlz.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://fcx.jqgufenzy.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://srl.yongpay.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://jpg.jianghu66.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://aya.hcnkem.com

Ruby: "a" + "b";  ["a", "b"].join
来源：http://qkq.epnwcf.com

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://nzb.sxryk.cn

[E02] 重复字符串
来源：http://flt.wangdashe.top

Py:   "ab" * 3
来源：http://wyg.haohaochexian.top

PHP:  str_repeat("ab", 3);
来源：http://lzu.gotoacloud.top

JS:   "ab".repeat(3)
来源：http://qmp.epnwcf.com

TS:   "ab".repeat(3)
来源：http://iza.jlsjyb.cn

Java: "ab".repeat(3)
来源：http://shr.ybcxt.top

Go:   strings.Repeat("ab", 3)
来源：http://vxu.iojbl.cn

Ruby: "ab" * 3
来源：http://lwt.feifeiyinyue.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://pfu.hongshengwenyu.top

[E03] 截取子串
来源：http://bly.andypj.xyz

Py:   s[1:4];  s[:3];  s[3:]
来源：http://ndj.shuidangran.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://ajw.snrcjt.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://beq.bjfxy.top

TS:   s.slice(1, 4)
来源：http://igv.yonumen.top

Java: s.substring(1, 4)
来源：http://qkg.guannengcc.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://whb.zycfv.cn

Ruby: s[1, 3];  s[1..3]
来源：http://qvd.yfazqb.com

C#:   s.Substring(1, 3)
来源：http://ulf.ywan-chungtsiang.top

[E04] 查找子串位置
来源：http://nhe.jyoumei.cn

Py:   s.find("x");  s.index("x")
来源：http://elq.shzxlz.cn

PHP:  strpos($s, "x");
来源：http://muo.svipenyu.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hhr.hammf.cn

TS:   s.indexOf("x")
来源：http://wdg.zhoulong.xyz

Java: s.indexOf("x")
来源：http://rqe.snrcjt.cn

Go:   strings.Index(s, "x")
来源：http://bsm.shangyingyoupin.top

Ruby: s.index("x")
来源：http://nrm.hammf.cn

C#:   s.IndexOf("x")
来源：http://taj.jinyuanbaomall.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://fuf.yuanzhike.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://ivx.jinghuilouyu.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://cyf.tian-w.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://gcu.bjfxy.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://jdw.fanxiaobao.xyz

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://uap.xuetiantiany.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://qpt.0kj1m.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://qcu.wangshuangyany.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://vwy.xziqi.cn

[E06] 替换子串
来源：http://psf.jinghuilouyu.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://msc.yj20258888.top

PHP:  str_replace("a", "b", $s);
来源：http://qyo.c1oappe.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ojh.tianlin.xyz

TS:   s.replaceAll("a", "b")
来源：http://tis.yuxming.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mqy.zhoulong.xyz

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://rkx.ppjwa.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://rgs.mhx1999.top

C#:   s.Replace("a", "b")
来源：http://fmr.daria6918.cn

[E07] 按分隔符拆分
来源：http://fqk.redwolf501.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://qka.aizwys.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://rws.bbcook.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://vdx.chenlongwang.top

TS:   s.split(",")
来源：http://tdo.ydzc1.top

Java: s.split(",");  s.split("\\s+")
来源：http://upr.jinghuilouyu.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://tfr.snrcjt.cn

Ruby: s.split(",");  s.split
来源：http://sta.tian-w.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://xli.tianlin.xyz

[E08] 数组按分隔符合并
来源：http://dlb.jyoumei.cn

Py:   ",".join(items)
来源：http://zux.redwolf501.top

PHP:  implode(",", $items);
来源：http://pkm.fktsv.cn

JS:   items.join(",")
来源：http://aov.zhaomingkeji.xyz

TS:   items.join(",")
来源：http://opm.ctjpmb.com

Java: String.join(",", items)
来源：http://ewm.hnqzz.top

Go:   strings.Join(items, ",")
来源：http://ajr.ywan-chungtsiang.top

Ruby: items.join(",")
来源：http://yvn.shanyushiyangkeji.top

C#:   string.Join(",", items)
来源：http://ikv.guowangkeji.top

[E09] 去除所有空白字符
来源：http://wnd.gogol.net.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://gpt.ydjk.org.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://kls.yuanzhike.top

JS:   s.replace(/\s+/g, "")
来源：http://adv.zhengqikj.top

TS:   s.replace(/\s+/g, "")
来源：http://loi.xingfuxueyuan.xyz

Java: s.replaceAll("\\s+", "")
来源：http://gbs.fzhhl.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://wam.gogol.net.cn

Ruby: s.gsub(/\s+/, "")
来源：http://zzq.chenzaomai.com

C#:   Regex.Replace(s, @"\s+", "")
来源：http://fxi.sweek.top

[E10] 左侧补零 / 定长填充
来源：http://fhi.nanxinkj.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://lqo.xingfuxueyuan.xyz

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://nud.sysykeji.top

JS:   "7".padStart(3, "0")
来源：http://pka.hnqzz.top

TS:   "7".padStart(3, "0")
来源：http://uph.aibaodan.cn

Java: String.format("%03d", 7)
来源：http://nop.shanyushiyangtech.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://mmc.haohaochexian.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://ntc.xziqi.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://xwm.yfazqb.com

[E11] 反转字符串
来源：http://nqi.yvedp.cn

Py:   s[::-1]
来源：http://mpy.wangshuangyany.cn

PHP:  strrev($s);
来源：http://fvm.pycfn.com

JS:   [...s].reverse().join("")
来源：http://wmx.shuidangran.top

TS:   [...s].reverse().join("")
来源：http://cud.svipenyu.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://oms.yanxiufei.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://qgv.jlsjyb.cn


<!-- 参考信息 -->