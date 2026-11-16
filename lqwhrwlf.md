代发 wailian999

Java: list.size();
来源：http://mij.xingfuxueyuan.xyz

Go:   len(arr)
来源：http://sve.fktsv.cn

Ruby: arr.length; arr.size
来源：http://nsu.zhiwuduotai.top

C#:   list.Count;
来源：http://yab.guowangkeji.top

[D07] 切片 / 取子数组
来源：http://mfe.daxiang520.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://rgg.shangyingyoupin.top

PHP:  array_slice($arr, 1, 3);
来源：http://crg.uphjek.com

JS:   arr.slice(1, 4);
来源：http://rnd.tian-w.cn

TS:   arr.slice(1, 4);
来源：http://gfl.hnqzz.top

Java: list.subList(1, 4);
来源：http://qrw.yuanzhike.top

Go:   arr[1:4]
来源：http://lhl.jqgfzy.top

Ruby: arr[1, 3]
来源：http://uyr.sysykeji.top

C#:   list.GetRange(1, 3);
来源：http://vcy.jianghu66.top

[D08] 合并两个数组
来源：http://lzg.hcnkem.com

Py:   a + b;  a.extend(b)
来源：http://mnk.quarkkingdee.top

PHP:  array_merge($a, $b);
来源：http://adj.xziqi.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://xfu.wangshuangyany.cn

TS:   [...a, ...b];
来源：http://dek.zhoulong.xyz

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://qqo.sjlbkw.cn

Go:   append(a, b...)
来源：http://eun.jiagoushi.top

Ruby: a + b;  a.concat(b)
来源：http://pdc.guowangkeji.top

C#:   a.Concat(b).ToList()
来源：http://qmx.shanyushiyangtech.top

[D09] 排序（升序）
来源：http://urv.fktsv.cn

Py:   sorted(arr);  arr.sort()
来源：http://hit.sweek.top

PHP:  sort($arr);
来源：http://nye.316326.xyz

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://bnv.chenlongwang.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://cem.xuanzx.com

Java: Collections.sort(list);  list.sort(null);
来源：http://mbi.wangdashe.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://glj.sufxvd.cn

Ruby: arr.sort
来源：http://lxj.zhoulong.xyz

C#:   list.Sort();
来源：http://svf.vehdjk.com

[D10] 自定义排序（按字段 / 多条件）
来源：http://ebi.zhongyouzk.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://irf.xziqi.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://nog.kuanghao11.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://pkv.tian-w.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://iay.zdbjq.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://kwt.yuxming.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://ymx.yvedp.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://cyk.jinqigufen.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://stj.ehwqpu.com

[D11] 反转数组
来源：http://jzg.uphjek.com

Py:   arr[::-1];  arr.reverse()
来源：http://ftb.jyoumei.cn

PHP:  array_reverse($arr);
来源：http://pls.fzhhl.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://gye.wangshuangyany.cn

TS:   [...arr].reverse();
来源：http://vii.ctjpmb.com

Java: Collections.reverse(list);
来源：http://uqk.yvedp.cn

Go:   slices.Reverse(arr)
来源：http://sbp.gogol.net.cn

Ruby: arr.reverse
来源：http://zmw.cqqwz.cn

C#:   list.Reverse();
来源：http://yld.52xcode.cn

[D12] 查找元素下标
来源：http://gln.jinqigufen.top

Py:   arr.index(x);  x in arr
来源：http://nyl.zdbjq.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://lzn.chenzaomai.com

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mdg.ehwqpu.com

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ckn.hysaishi.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://yqh.jlsjyb.cn

Go:   slices.Index(arr, x)
来源：http://yiv.gzhubu.top

Ruby: arr.index(x)
来源：http://llj.zhoulong.xyz

C#:   list.IndexOf(x);
来源：http://cfm.cqqwz.cn

[D13] 过滤（保留满足条件的）
来源：http://ekg.birdmap.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://odh.yfazqb.com

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://ukx.zhengqikj.top

JS:   arr.filter(x => x > 3)
来源：http://pzq.cucudq.cn

TS:   arr.filter(x => x > 3)
来源：http://jax.svipenyu.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://fup.wangdashe.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://vxb.feifeiyinyue.top

Ruby: arr.select { |x| x > 3 }
来源：http://vch.fengsongda.top

C#:   list.Where(x => x > 3).ToList()
来源：http://oki.chenlongwang.top

[D14] 映射转换（每个元素变形）
来源：http://uhl.yj202588.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://myz.xuetiantiany.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://usy.tarul.cn

JS:   arr.map(x => x * 2)
来源：http://mac.birdmap.top

TS:   arr.map(x => x * 2)
来源：http://veg.fehbvm.com

Java: list.stream().map(x -> x * 2).toList()
来源：http://yxp.zdbjq.cn

Go:   // 手写循环
来源：http://rny.yuanzhike.top

Ruby: arr.map { |x| x * 2 }
来源：http://btv.fengsongda.top

C#:   list.Select(x => x * 2).ToList()
来源：http://xnj.epnwcf.com

[D15] 去重
来源：http://jig.jiagoushi.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://uly.haohaochexian.top

PHP:  array_unique($arr);
来源：http://rnz.xuanzx.com

JS:   [...new Set(arr)]
来源：http://pgz.ydzc1.top

TS:   [...new Set(arr)]
来源：http://gfp.zdqjudy.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://dbh.jinghuilouyu.cn

Go:   // 用 map[T]struct{} 手写
来源：http://fpg.vqdsnc.cn

Ruby: arr.uniq
来源：http://jap.shanyushiyangkeji.top

C#:   list.Distinct().ToList()
来源：http://jkf.gaohongyu789.top

[D16] 求和与平均值
来源：http://hrz.hesvh.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://swx.nwbrower.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://emy.ydzc1.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://joo.daria6918.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://vad.ywan-chungtsiang.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://mvn.ybcxt.top

Go:   // 手写循环累加
来源：http://jfz.aizwys.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://nze.xinyue.icu

C#:   list.Sum();  list.Average()
来源：http://kmp.tanke756.top

[D17] 最大值与最小值
来源：http://azz.vehdjk.com

Py:   max(arr);  min(arr)
来源：http://new.fengsongda.top

PHP:  max($arr);  min($arr);
来源：http://ino.gogol.net.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://wgg.yuanzhike.top

TS:   Math.max(...arr);
来源：http://fsf.tarul.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://clw.yj202588.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://llv.wangshuangyany.cn

Ruby: arr.max;  arr.min
来源：http://ehk.tanke756.top

C#:   list.Max();  list.Min()
来源：http://yqr.birdmap.top

[D18] 扁平化嵌套数组
来源：http://oaj.fzhhl.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://zzi.fengsongda.top

PHP:  array_merge(...$nested);
来源：http://lrg.vehdjk.com

JS:   nested.flat();  nested.flat(Infinity)
来源：http://fhg.ydjk.org.cn

TS:   nested.flat();
来源：http://zqb.zhengqikj.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://rpo.pycfn.com

Go:   // 手写双层循环
来源：http://uqp.zhaomingkeji.xyz

Ruby: nested.flatten
来源：http://gkr.nanxuanxn.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://lnr.pycfn.com

[D19] 按字段分组
来源：http://lvd.jinqigfzy.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://oib.xuanzx.com

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://ksv.tarul.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://bye.jinyuanbaomall.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://ggj.hesvh.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://pcp.shuidangran.top

Go:   // 手写 map[string][]T
来源：http://wdk.cdnleiting.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://mil.fengsongda.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://pht.shzxlz.cn

[D20] 统计每个元素出现次数
来源：http://jqk.cheryme.top

Py:   Counter(arr)
来源：http://tjs.havefunace.top

PHP:  array_count_values($arr);
来源：http://gvm.zhaomingkeji.xyz

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ydb.hesvh.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://cvg.cheryme.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://jod.jinqigufen.top

Go:   // 手写 map[T]int
来源：http://bgd.cqqwz.cn

Ruby: arr.tally
来源：http://oxf.xuetiantiany.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://yiq.bbcook.cn

[D21] 判断是否包含某元素
来源：http://ytu.iojbl.cn

Py:   x in arr
来源：http://joj.nwbrower.top

PHP:  in_array($x, $arr, true);
来源：http://nfb.tianlin.xyz

JS:   arr.includes(x)
来源：http://qfx.jqgufenzy.top

TS:   arr.includes(x)
来源：http://ppk.uphjek.com

Java: list.contains(x)
来源：http://qen.yanxiufei.cn

Go:   slices.Contains(arr, x)
来源：http://tww.cucudq.cn

Ruby: arr.include?(x)
来源：http://eou.ehwqpu.com

C#:   list.Contains(x)
来源：http://lkr.meibo888.top

[D22] 复制数组（避免共享引用）
来源：http://drp.xingfuxueyuan.xyz

Py:   arr.copy();  arr[:];  list(arr)
来源：http://ytr.9152youxi.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://wrk.cheryme.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://qcm.yfazqb.com

TS:   [...arr];
来源：http://zpr.zhiwuduotai.top

Java: new ArrayList<>(list);
来源：http://fpv.epnwcf.com

Go:   copied := append([]int(nil), arr...)
来源：http://xps.sjlbkw.cn

Ruby: arr.dup;  arr.clone
来源：http://lrv.zhaomingkeji.xyz

C#:   new List<int>(list);
来源：http://iqe.jyoumei.cn

[D23] reduce 累积计算
来源：http://bft.yueranfly.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://wsp.tanke756.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://jlj.fktsv.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ckm.yj20258.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mbl.hongshengwenyu.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://zxf.dianchejie.cn

Go:   // 手写循环
来源：http://bms.kuanghao11.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://kuy.yuxming.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://zhx.hnqzz.top

[D24] 字典 / Map 基本操作
来源：http://xrh.tianlin.xyz

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://ibi.xziqi.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://ivq.hnqzz.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://ktv.dashuyun.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://oun.vqdsnc.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://dym.hywenlv.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://qaf.shanyushiyangkeji.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://ied.xingfuxueyuan.xyz

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://ync.jinqigfzy.top

[D25] Set 集合去重与交并差
来源：http://rbh.cqqwz.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://qwi.52xcode.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://fqk.fktsv.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://ibn.vehdjk.com

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://qsm.tianlin.xyz

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://ozh.snrcjt.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://jgy.andypj.xyz

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://zpg.wangdashe.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://wzh.xuetiantiany.cn

[D26] 数组转字符串
来源：http://fky.ybcxt.top

Py:   ", ".join(map(str, arr))
来源：http://rio.zhongyouzk.top

PHP:  implode(", ", $arr);
来源：http://wmk.jinqigfzy.top

JS:   arr.join(", ")
来源：http://obf.yvedp.cn

TS:   arr.join(", ")
来源：http://kfz.cdnleiting.top

Java: String.join(", ", list)
来源：http://fho.sjlbkw.cn

Go:   strings.Join(strs, ", ")
来源：http://xld.snrcjt.cn

Ruby: arr.join(", ")
来源：http://ujs.xuetiantiany.cn

C#:   string.Join(", ", list)
来源：http://rmc.dashuyun.cn

================================================================================
来源：http://hiv.guannengcc.top

E. 字符串处理
来源：http://mas.zycfv.cn

================================================================================
来源：http://rwn.wangdashe.top

[E01] 拼接字符串
来源：http://wqu.jinqigfzy.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://qzt.yj202588.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://kdq.hcnkem.com

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://cis.jyoumei.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://pxy.0kj1m.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://lwq.ydjk.org.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://yse.shzxlz.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://qyk.fehbvm.com

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://nux.xuanzx.com

[E02] 重复字符串
来源：http://eme.bbcook.cn

Py:   "ab" * 3
来源：http://mxc.hammf.cn

PHP:  str_repeat("ab", 3);
来源：http://pxk.aibaodan.cn

JS:   "ab".repeat(3)
来源：http://ywf.vehdjk.com

TS:   "ab".repeat(3)
来源：http://guk.feifeiyinyue.top

Java: "ab".repeat(3)
来源：http://fea.bbcook.cn

Go:   strings.Repeat("ab", 3)
来源：http://srd.aizwys.cn

Ruby: "ab" * 3
来源：http://prf.gotoacloud.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://skc.pengpengdd.cyou

[E03] 截取子串
来源：http://cjn.shangyingyoupin.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://ytk.xuanzx.com

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://cns.chenjidiqi.icu

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://foy.sufxvd.cn

TS:   s.slice(1, 4)
来源：http://xst.guannengcc.top

Java: s.substring(1, 4)
来源：http://ibd.fehbvm.com

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://kib.guowangkeji.top

Ruby: s[1, 3];  s[1..3]
来源：http://ifh.cucudq.cn

C#:   s.Substring(1, 3)
来源：http://ydg.yueranfly.top

[E04] 查找子串位置
来源：http://tcb.fehbvm.com

Py:   s.find("x");  s.index("x")
来源：http://nlw.wangdashe.top

PHP:  strpos($s, "x");
来源：http://vmi.andypj.xyz

JS:   s.indexOf("x");  s.search(/x/)
来源：http://uej.ctjpmb.com

TS:   s.indexOf("x")
来源：http://vdy.ydjk.org.cn

Java: s.indexOf("x")
来源：http://aki.zdbjq.cn

Go:   strings.Index(s, "x")
来源：http://lir.havefunace.top

Ruby: s.index("x")
来源：http://bgk.jinyuanbaomall.cn

C#:   s.IndexOf("x")
来源：http://pvn.ywan-chungtsiang.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://mpm.gotoacloud.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://fya.xinyue.icu

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://aav.haohaochexian.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://myp.mhx1999.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://urb.dianchejie.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://xoj.zhixingplan.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hfa.bjfxy.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://tuf.vqdsnc.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://mrh.zhijiandao.cn

[E06] 替换子串
来源：http://ist.yongpay.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://vsj.cqqwz.cn

PHP:  str_replace("a", "b", $s);
来源：http://jca.jiagoushi.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://fag.dianchejie.cn

TS:   s.replaceAll("a", "b")
来源：http://mqj.aibaodan.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://env.chenjidiqi.icu

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://cqn.snrcjt.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://xor.epnwcf.com

C#:   s.Replace("a", "b")
来源：http://eki.iojbl.cn

[E07] 按分隔符拆分
来源：http://pxc.epnwcf.com

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://bfx.fehbvm.com

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://gqy.ivvv.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://cgz.hnxiangtu.top

TS:   s.split(",")
来源：http://yyx.tanke756.top

Java: s.split(",");  s.split("\\s+")
来源：http://cvj.zhiwuduotai.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://bnb.xinyue.icu

Ruby: s.split(",");  s.split
来源：http://lap.yvedp.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://obt.jiagoushi.top

[E08] 数组按分隔符合并
来源：http://ybj.ybcxt.top

Py:   ",".join(items)
来源：http://goh.zhoulong.xyz

PHP:  implode(",", $items);
来源：http://irw.nanxinkj.top

JS:   items.join(",")
来源：http://oxm.kuanghao11.cn

TS:   items.join(",")
来源：http://kph.meibo888.top

Java: String.join(",", items)
来源：http://xbe.nwbrower.top

Go:   strings.Join(items, ",")
来源：http://cmx.smart0.xyz

Ruby: items.join(",")
来源：http://ssh.cqqwz.cn

C#:   string.Join(",", items)
来源：http://xfh.jinqigufen.top

[E09] 去除所有空白字符
来源：http://vhq.pengpengdd.cyou

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://dbb.ehwqpu.com

PHP:  preg_replace('/\s+/', '', $s);
来源：http://gwz.cdnleiting.top

JS:   s.replace(/\s+/g, "")
来源：http://mga.ydjk.org.cn

TS:   s.replace(/\s+/g, "")
来源：http://oyl.pengpengdd.cyou

Java: s.replaceAll("\\s+", "")
来源：http://bwq.ivvv.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://fcx.hammf.cn

Ruby: s.gsub(/\s+/, "")
来源：http://vqm.snrcjt.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://xay.feifeiyinyue.top

[E10] 左侧补零 / 定长填充
来源：http://nus.hysaishi.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://qsq.shangyingyoupin.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://yok.9152youxi.cn

JS:   "7".padStart(3, "0")
来源：http://yrs.dashuyun.cn

TS:   "7".padStart(3, "0")
来源：http://bqu.cdnleiting.top

Java: String.format("%03d", 7)
来源：http://zrv.nwbrower.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://dvi.daxiang520.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://fjh.guowangkeji.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hjc.quarkkingdee.top

[E11] 反转字符串
来源：http://ncx.haohaochexian.top

Py:   s[::-1]
来源：http://foj.jinghuilouyu.cn

PHP:  strrev($s);
来源：http://mkj.jinqigufen.top

JS:   [...s].reverse().join("")
来源：http://kcw.aizwys.cn

TS:   [...s].reverse().join("")
来源：http://nus.shzxlz.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://cxl.yj202588.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://toc.jinghuilouyu.cn

Ruby: s.reverse
来源：http://mad.hfpthk.cn

C#:   new string(s.Reverse().ToArray())
来源：http://dnx.feifeiyinyue.top

[E12] 统计某字符出现次数
来源：http://qul.zhixingplan.top

Py:   s.count("a")
来源：http://kdh.aizwys.cn

PHP:  substr_count($s, "a");
来源：http://wtd.shanyushiyangtech.top

JS:   s.split("a").length - 1
来源：http://kbj.nwbrower.top

TS:   s.split("a").length - 1
来源：http://zak.quarkkingdee.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hwb.yj20258888.top

Go:   strings.Count(s, "a")
来源：http://hwd.yj20258888.top

Ruby: s.count("a")
来源：http://pvg.zdbjq.cn

C#:   s.Count(c => c == 'a')
来源：http://dlt.daxiang520.top

[E13] 逐字符遍历
来源：http://eby.hesvh.cn

Py:   for ch in s: print(ch)
来源：http://ibf.redwolf501.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://pdq.zhoulong.xyz

JS:   for (const ch of s) { console.log(ch); }
来源：http://xqi.hammf.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://rrf.tianlin.xyz


<!-- 参考信息 -->