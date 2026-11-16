代发 wailian999

Java: list.size();
来源：http://ktu.bbcook.cn

Go:   len(arr)
来源：http://cpg.yfazqb.com

Ruby: arr.length; arr.size
来源：http://njj.fktsv.cn

C#:   list.Count;
来源：http://nzi.yj202588.top

[D07] 切片 / 取子数组
来源：http://bqg.cashguo.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://mjq.redwolf501.top

PHP:  array_slice($arr, 1, 3);
来源：http://pox.fehbvm.com

JS:   arr.slice(1, 4);
来源：http://yiq.hnqzz.top

TS:   arr.slice(1, 4);
来源：http://hql.birdmap.top

Java: list.subList(1, 4);
来源：http://rir.xuanzx.com

Go:   arr[1:4]
来源：http://sfo.hesvh.cn

Ruby: arr[1, 3]
来源：http://ujr.haohaochexian.top

C#:   list.GetRange(1, 3);
来源：http://fdr.hysaishi.cn

[D08] 合并两个数组
来源：http://atd.hysaishi.cn

Py:   a + b;  a.extend(b)
来源：http://lnm.nwbrower.top

PHP:  array_merge($a, $b);
来源：http://gyl.wangdashe.top

JS:   [...a, ...b];  a.concat(b);
来源：http://vua.jinqigfzy.top

TS:   [...a, ...b];
来源：http://qks.fanxiaobao.xyz

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://ont.xuanzx.com

Go:   append(a, b...)
来源：http://doo.iojbl.cn

Ruby: a + b;  a.concat(b)
来源：http://yba.sufxvd.cn

C#:   a.Concat(b).ToList()
来源：http://zpn.yj202588.top

[D09] 排序（升序）
来源：http://qyq.feifeiyinyue.top

Py:   sorted(arr);  arr.sort()
来源：http://kcv.xinyue.icu

PHP:  sort($arr);
来源：http://pwt.hcnkem.com

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://zcr.andypj.xyz

TS:   [...arr].sort((x, y) => x - y);
来源：http://ecr.shzxlz.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://yna.yvedp.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://ffk.tanke756.top

Ruby: arr.sort
来源：http://rgj.jianghu66.top

C#:   list.Sort();
来源：http://prn.jyoumei.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://gru.bjfxy.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://skx.gzhubu.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://raa.yonumen.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://muf.birdmap.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://ukd.zhixingplan.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://ohk.zhaomingkeji.xyz

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://iok.ehwqpu.com

Ruby: arr.sort_by { |x| x[:age] }
来源：http://zzq.birdmap.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://ssy.quarkkingdee.top

[D11] 反转数组
来源：http://hij.hesvh.cn

Py:   arr[::-1];  arr.reverse()
来源：http://lix.svipenyu.cn

PHP:  array_reverse($arr);
来源：http://akw.andypj.xyz

JS:   [...arr].reverse();  arr.toReversed()
来源：http://knh.mhx1999.top

TS:   [...arr].reverse();
来源：http://xvi.52xcode.cn

Java: Collections.reverse(list);
来源：http://rwv.nanxinkj.top

Go:   slices.Reverse(arr)
来源：http://rar.daria6918.cn

Ruby: arr.reverse
来源：http://ntr.jinqigufen.top

C#:   list.Reverse();
来源：http://awb.zhiwuduotai.top

[D12] 查找元素下标
来源：http://mga.birdmap.top

Py:   arr.index(x);  x in arr
来源：http://oji.jinyuanbaomall.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://xke.shanyushiyangkeji.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://csv.dianchejie.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://xbr.yj20258.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://wgk.chenzaomai.com

Go:   slices.Index(arr, x)
来源：http://veo.fehbvm.com

Ruby: arr.index(x)
来源：http://imc.sweek.top

C#:   list.IndexOf(x);
来源：http://oys.gogol.net.cn

[D13] 过滤（保留满足条件的）
来源：http://oyt.ybcxt.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://rxh.jyoumei.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://tow.svipenyu.cn

JS:   arr.filter(x => x > 3)
来源：http://jtn.smart0.xyz

TS:   arr.filter(x => x > 3)
来源：http://hmt.fktsv.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://pfj.jinqigfzy.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://xnx.snrcjt.cn

Ruby: arr.select { |x| x > 3 }
来源：http://nzl.shzxlz.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://mhk.yueranfly.top

[D14] 映射转换（每个元素变形）
来源：http://dni.sjlbkw.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://kvv.zhengqikj.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://zkb.daxiang520.top

JS:   arr.map(x => x * 2)
来源：http://pwl.shanyushiyangkeji.top

TS:   arr.map(x => x * 2)
来源：http://qhn.tanke756.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://hhk.fktsv.cn

Go:   // 手写循环
来源：http://suv.gaohongyu789.top

Ruby: arr.map { |x| x * 2 }
来源：http://poe.xinyue.icu

C#:   list.Select(x => x * 2).ToList()
来源：http://cno.ydzc1.top

[D15] 去重
来源：http://hax.zhaomingkeji.xyz

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://nwd.epnwcf.com

PHP:  array_unique($arr);
来源：http://cju.tianlin.xyz

JS:   [...new Set(arr)]
来源：http://grs.316326.xyz

TS:   [...new Set(arr)]
来源：http://reb.mhx1999.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://iaj.fengsongda.top

Go:   // 用 map[T]struct{} 手写
来源：http://frn.svipenyu.cn

Ruby: arr.uniq
来源：http://zvd.wangshuangyany.cn

C#:   list.Distinct().ToList()
来源：http://tde.sysykeji.top

[D16] 求和与平均值
来源：http://hpy.yfazqb.com

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://ibi.xingfuxueyuan.xyz

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://yke.ppjwa.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://gdl.guannengcc.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://bdy.yj20258.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://iij.svipenyu.cn

Go:   // 手写循环累加
来源：http://cyf.gzhubu.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://toy.xziqi.cn

C#:   list.Sum();  list.Average()
来源：http://psp.jinghuilouyu.cn

[D17] 最大值与最小值
来源：http://drl.0kj1m.cn

Py:   max(arr);  min(arr)
来源：http://ymn.xylfe.cn

PHP:  max($arr);  min($arr);
来源：http://nyi.jqgfzy.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://ked.nanxinkj.top

TS:   Math.max(...arr);
来源：http://zgy.sjlbkw.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://qyj.meibo888.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://pxf.haohaochexian.top

Ruby: arr.max;  arr.min
来源：http://xkr.fanxiaobao.xyz

C#:   list.Max();  list.Min()
来源：http://vha.guowangkeji.top

[D18] 扁平化嵌套数组
来源：http://hnp.feifeiyinyue.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://amx.yuxming.cn

PHP:  array_merge(...$nested);
来源：http://slq.yonumen.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hxi.zhaomingkeji.xyz

TS:   nested.flat();
来源：http://izm.nanxuanxn.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://bzv.zdbjq.cn

Go:   // 手写双层循环
来源：http://sfg.zhengqikj.top

Ruby: nested.flatten
来源：http://lzp.dashuyun.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://wyd.yfazqb.com

[D19] 按字段分组
来源：http://dff.xziqi.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://dlz.gaohongyu789.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://daf.zhoulong.xyz

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://sja.birdmap.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://uov.jinqigfzy.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://pqy.haohaochexian.top

Go:   // 手写 map[string][]T
来源：http://xcf.daxiang520.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://jap.yfazqb.com

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://eqp.jqgufenzy.top

[D20] 统计每个元素出现次数
来源：http://qgk.meibo888.top

Py:   Counter(arr)
来源：http://rob.jlsjyb.cn

PHP:  array_count_values($arr);
来源：http://gxv.cheryme.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ohj.sjlbkw.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://cjs.guannengcc.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://cpi.hnqzz.top

Go:   // 手写 map[T]int
来源：http://qmy.chenlongwang.top

Ruby: arr.tally
来源：http://qvh.9152youxi.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hon.tarul.cn

[D21] 判断是否包含某元素
来源：http://pvg.hcnkem.com

Py:   x in arr
来源：http://bys.sweek.top

PHP:  in_array($x, $arr, true);
来源：http://bnp.zhijiandao.cn

JS:   arr.includes(x)
来源：http://vax.jinqigufen.top

TS:   arr.includes(x)
来源：http://llr.ywan-chungtsiang.top

Java: list.contains(x)
来源：http://ywu.ivvv.top

Go:   slices.Contains(arr, x)
来源：http://qtx.cucudq.cn

Ruby: arr.include?(x)
来源：http://tcr.uphjek.com

C#:   list.Contains(x)
来源：http://hvr.zhijiandao.cn

[D22] 复制数组（避免共享引用）
来源：http://hlx.xingfuxueyuan.xyz

Py:   arr.copy();  arr[:];  list(arr)
来源：http://qdq.sweek.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://lwv.redwolf501.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://jxf.cdnleiting.top

TS:   [...arr];
来源：http://nyq.tianlin.xyz

Java: new ArrayList<>(list);
来源：http://tno.ivvv.top

Go:   copied := append([]int(nil), arr...)
来源：http://xsi.daria6918.cn

Ruby: arr.dup;  arr.clone
来源：http://xdm.9152youxi.cn

C#:   new List<int>(list);
来源：http://zfc.aizwys.cn

[D23] reduce 累积计算
来源：http://lhf.316326.xyz

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://gyb.ydjk.org.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://ybx.aibaodan.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://swx.kuanghao11.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://lxc.ywan-chungtsiang.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://neu.havefunace.top

Go:   // 手写循环
来源：http://pjn.sweek.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://zss.gaohongyu789.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://oyv.yongpay.top

[D24] 字典 / Map 基本操作
来源：http://jke.uphjek.com

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://tkb.yongpay.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://qsh.gotoacloud.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hhs.hongshengwenyu.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://ylu.jqgfzy.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://mye.c1oappe.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://nea.ydzc1.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://rvt.hywenlv.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://lfl.yvedp.cn

[D25] Set 集合去重与交并差
来源：http://tii.chenzaomai.com

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://grz.hywenlv.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://jnw.xuanzx.com

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://khc.haohaochexian.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://att.yj20258.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://jix.zdqjudy.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://jnr.fehbvm.com

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://qkd.jqgufenzy.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://lza.aibaodan.cn

[D26] 数组转字符串
来源：http://mzc.nanxuanxn.top

Py:   ", ".join(map(str, arr))
来源：http://aeu.xziqi.cn

PHP:  implode(", ", $arr);
来源：http://wjb.xuanzx.com

JS:   arr.join(", ")
来源：http://miw.zhaomingkeji.xyz

TS:   arr.join(", ")
来源：http://nwi.vqdsnc.cn

Java: String.join(", ", list)
来源：http://mus.tian-w.cn

Go:   strings.Join(strs, ", ")
来源：http://pte.kuanghao11.cn

Ruby: arr.join(", ")
来源：http://iwm.fzhhl.top

C#:   string.Join(", ", list)
来源：http://sdd.hongshengwenyu.top

================================================================================
来源：http://mmm.hnqzz.top

E. 字符串处理
来源：http://srs.xinyue.icu

================================================================================
来源：http://boq.ctjpmb.com

[E01] 拼接字符串
来源：http://sto.sjlbkw.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://ddw.kuanghao11.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://vsk.tanke756.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://rhy.meibo888.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://axl.fanxiaobao.xyz

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://tpk.chenjidiqi.icu

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://udq.zhoulong.xyz

Ruby: "a" + "b";  ["a", "b"].join
来源：http://tfl.feifeiyinyue.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://myf.zhixingplan.top

[E02] 重复字符串
来源：http://pqo.cucudq.cn

Py:   "ab" * 3
来源：http://uwn.fengsongda.top

PHP:  str_repeat("ab", 3);
来源：http://yje.yfazqb.com

JS:   "ab".repeat(3)
来源：http://axr.uphjek.com

TS:   "ab".repeat(3)
来源：http://xrx.iojbl.cn

Java: "ab".repeat(3)
来源：http://zod.xuetiantiany.cn

Go:   strings.Repeat("ab", 3)
来源：http://zon.andypj.xyz

Ruby: "ab" * 3
来源：http://jbx.gaohongyu789.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://ppf.hnxiangtu.top

[E03] 截取子串
来源：http://fcq.jlsjyb.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://vfz.52xcode.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://qvz.bbcook.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://ngt.vqdsnc.cn

TS:   s.slice(1, 4)
来源：http://huh.zhengqikj.top

Java: s.substring(1, 4)
来源：http://wjp.cheryme.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://ogu.zdqjudy.top

Ruby: s[1, 3];  s[1..3]
来源：http://iko.meibo888.top

C#:   s.Substring(1, 3)
来源：http://irm.yfazqb.com

[E04] 查找子串位置
来源：http://hjl.ivvv.top

Py:   s.find("x");  s.index("x")
来源：http://gay.zhijiandao.cn

PHP:  strpos($s, "x");
来源：http://nnh.tian-w.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://zul.shanyushiyangtech.top

TS:   s.indexOf("x")
来源：http://tmf.jinyuanbaomall.cn

Java: s.indexOf("x")
来源：http://zrx.cqqwz.cn

Go:   strings.Index(s, "x")
来源：http://lcq.uphjek.com

Ruby: s.index("x")
来源：http://zny.redwolf501.top

C#:   s.IndexOf("x")
来源：http://wwd.aibaodan.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://icm.cqqwz.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://qle.shangyingyoupin.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://wam.vehdjk.com

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://xms.aibaodan.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://bbk.guannengcc.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://lop.jyoumei.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://blu.zycfv.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://wgz.gogol.net.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hcr.sjlbkw.cn

[E06] 替换子串
来源：http://yfg.yangfankeji.com

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://amf.sjlbkw.cn

PHP:  str_replace("a", "b", $s);
来源：http://bzi.ctjpmb.com

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://xxp.meibo888.top

TS:   s.replaceAll("a", "b")
来源：http://enl.jinyuanbaomall.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://vbx.epnwcf.com

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://csg.hnxiangtu.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://mwq.yuxming.cn

C#:   s.Replace("a", "b")
来源：http://zph.vehdjk.com

[E07] 按分隔符拆分
来源：http://pjf.cdnleiting.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://syb.xingfuxueyuan.xyz

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://ude.shangyingyoupin.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://pff.nanxuanxn.top

TS:   s.split(",")
来源：http://ngi.chenlongwang.top

Java: s.split(",");  s.split("\\s+")
来源：http://efm.birdmap.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://tlr.birdmap.top

Ruby: s.split(",");  s.split
来源：http://uou.mhx1999.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://uyw.yonumen.top

[E08] 数组按分隔符合并
来源：http://out.ppjwa.cn

Py:   ",".join(items)
来源：http://kcs.dianchejie.cn

PHP:  implode(",", $items);
来源：http://oxz.hcnkem.com

JS:   items.join(",")
来源：http://azo.jinghuilouyu.cn

TS:   items.join(",")
来源：http://nli.jianghu66.top

Java: String.join(",", items)
来源：http://kjt.sweek.top

Go:   strings.Join(items, ",")
来源：http://euo.sufxvd.cn

Ruby: items.join(",")
来源：http://dry.52xcode.cn

C#:   string.Join(",", items)
来源：http://apn.jqgfzy.top

[E09] 去除所有空白字符
来源：http://vfj.yueranfly.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://rwk.yongpay.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://xly.cdnleiting.top

JS:   s.replace(/\s+/g, "")
来源：http://fqe.xuetiantiany.cn

TS:   s.replace(/\s+/g, "")
来源：http://ysy.yanxiufei.cn

Java: s.replaceAll("\\s+", "")
来源：http://owc.c1oappe.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://ace.nwbrower.top

Ruby: s.gsub(/\s+/, "")
来源：http://qlj.wangdashe.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://yyz.yvedp.cn

[E10] 左侧补零 / 定长填充
来源：http://fyv.jiagoushi.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://riu.aibaodan.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://vpt.ppjwa.cn

JS:   "7".padStart(3, "0")
来源：http://bln.jlsjyb.cn

TS:   "7".padStart(3, "0")
来源：http://vmi.yj20258888.top

Java: String.format("%03d", 7)
来源：http://fzc.cucudq.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://aep.havefunace.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://tqi.ehwqpu.com

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://vqa.yanxiufei.cn

[E11] 反转字符串
来源：http://gcp.vqdsnc.cn

Py:   s[::-1]
来源：http://shq.chenlongwang.top

PHP:  strrev($s);
来源：http://eni.hesvh.cn

JS:   [...s].reverse().join("")
来源：http://ydj.mhx1999.top

TS:   [...s].reverse().join("")
来源：http://vdc.zhiwuduotai.top

Java: new StringBuilder(s).reverse().toString()
来源：http://hik.andypj.xyz

Go:   // 转 []rune 后倒序再转回 string
来源：http://rlm.snrcjt.cn

Ruby: s.reverse
来源：http://dxo.yuxming.cn

C#:   new string(s.Reverse().ToArray())
来源：http://gfv.gotoacloud.top

[E12] 统计某字符出现次数
来源：http://afi.chenzaomai.com

Py:   s.count("a")
来源：http://ytk.yueranfly.top

PHP:  substr_count($s, "a");
来源：http://sgc.0kj1m.cn

JS:   s.split("a").length - 1
来源：http://xym.smart0.xyz

TS:   s.split("a").length - 1
来源：http://ygv.cdnleiting.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://ghv.tarul.cn

Go:   strings.Count(s, "a")
来源：http://bch.hcnkem.com

Ruby: s.count("a")
来源：http://akc.zhoulong.xyz

C#:   s.Count(c => c == 'a')
来源：http://rpc.zdbjq.cn

[E13] 逐字符遍历
来源：http://gev.daria6918.cn

Py:   for ch in s: print(ch)
来源：http://mrd.shangyingyoupin.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://jqh.ybcxt.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://qfk.bjfxy.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://ljh.ybcxt.top


<!-- 参考信息 -->