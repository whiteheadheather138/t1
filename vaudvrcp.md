代发 wailian999

C#:   list.GetRange(1, 3);
来源：http://mcr.birdmap.top

[D08] 合并两个数组
来源：http://vvw.zdbjq.cn

Py:   a + b;  a.extend(b)
来源：http://fnm.zdqjudy.top

PHP:  array_merge($a, $b);
来源：http://psc.zhongyouzk.top

JS:   [...a, ...b];  a.concat(b);
来源：http://nue.xuetiantiany.cn

TS:   [...a, ...b];
来源：http://afb.xuanzx.com

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://zch.ctjpmb.com

Go:   append(a, b...)
来源：http://xen.sweek.top

Ruby: a + b;  a.concat(b)
来源：http://zqo.tianlin.xyz

C#:   a.Concat(b).ToList()
来源：http://wxs.cqqwz.cn

[D09] 排序（升序）
来源：http://cnj.hcnkem.com

Py:   sorted(arr);  arr.sort()
来源：http://kgt.hongshengwenyu.top

PHP:  sort($arr);
来源：http://fja.zdbjq.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://znk.52xcode.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://jgz.sufxvd.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://exh.xingfuxueyuan.xyz

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://gyc.hongshengwenyu.top

Ruby: arr.sort
来源：http://tlh.cheryme.top

C#:   list.Sort();
来源：http://lsn.nanxinkj.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://aoc.fehbvm.com

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://eps.meibo888.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://neu.zhongyouzk.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://pud.316326.xyz

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://ghg.gotoacloud.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://oia.xuetiantiany.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://grq.daria6918.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://upf.yuxming.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://twi.hcnkem.com

[D11] 反转数组
来源：http://yry.nanxuanxn.top

Py:   arr[::-1];  arr.reverse()
来源：http://nvj.nanxuanxn.top

PHP:  array_reverse($arr);
来源：http://bhn.zhiwuduotai.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://bxz.zdqjudy.top

TS:   [...arr].reverse();
来源：http://ugm.jyoumei.cn

Java: Collections.reverse(list);
来源：http://vni.zhiwuduotai.top

Go:   slices.Reverse(arr)
来源：http://rce.epnwcf.com

Ruby: arr.reverse
来源：http://lft.nanxuanxn.top

C#:   list.Reverse();
来源：http://tiw.uphjek.com

[D12] 查找元素下标
来源：http://ghm.nanxinkj.top

Py:   arr.index(x);  x in arr
来源：http://uuq.aizwys.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://udt.fanxiaobao.xyz

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://vra.meibo888.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mdd.zhongyouzk.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hvc.jianghu66.top

Go:   slices.Index(arr, x)
来源：http://fas.zhijiandao.cn

Ruby: arr.index(x)
来源：http://vam.shangyingyoupin.top

C#:   list.IndexOf(x);
来源：http://owm.hfpthk.cn

[D13] 过滤（保留满足条件的）
来源：http://apc.xuetiantiany.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://ofn.xziqi.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://vdu.xuanzx.com

JS:   arr.filter(x => x > 3)
来源：http://xjt.gogol.net.cn

TS:   arr.filter(x => x > 3)
来源：http://sfq.vehdjk.com

Java: list.stream().filter(x -> x > 3).toList()
来源：http://dvv.fktsv.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://oev.yj20258.top

Ruby: arr.select { |x| x > 3 }
来源：http://kkd.yonumen.top

C#:   list.Where(x => x > 3).ToList()
来源：http://vqs.hcnkem.com

[D14] 映射转换（每个元素变形）
来源：http://ytg.gogol.net.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://nxw.gotoacloud.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://nav.cheryme.top

JS:   arr.map(x => x * 2)
来源：http://rdk.zdqjudy.top

TS:   arr.map(x => x * 2)
来源：http://pto.jinghuilouyu.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://ida.cdnleiting.top

Go:   // 手写循环
来源：http://uez.shzxlz.cn

Ruby: arr.map { |x| x * 2 }
来源：http://oun.hysaishi.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://ehx.jinyuanbaomall.cn

[D15] 去重
来源：http://wtr.pengpengdd.cyou

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://bhn.havefunace.top

PHP:  array_unique($arr);
来源：http://ygg.cashguo.top

JS:   [...new Set(arr)]
来源：http://flf.c1oappe.top

TS:   [...new Set(arr)]
来源：http://guf.andypj.xyz

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://rxd.xylfe.cn

Go:   // 用 map[T]struct{} 手写
来源：http://xmm.jinyuanbaomall.cn

Ruby: arr.uniq
来源：http://fgu.sweek.top

C#:   list.Distinct().ToList()
来源：http://hsm.yj202588.top

[D16] 求和与平均值
来源：http://ika.yonumen.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://lxj.zhoulong.xyz

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://eol.jyoumei.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://jww.cucudq.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://qdh.xinyue.icu

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://ajr.kuanghao11.cn

Go:   // 手写循环累加
来源：http://duf.cheryme.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://zbd.quarkkingdee.top

C#:   list.Sum();  list.Average()
来源：http://vzx.xuetiantiany.cn

[D17] 最大值与最小值
来源：http://lio.yuxming.cn

Py:   max(arr);  min(arr)
来源：http://alo.meibo888.top

PHP:  max($arr);  min($arr);
来源：http://mnd.nanxinkj.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://pbd.chenjidiqi.icu

TS:   Math.max(...arr);
来源：http://bqx.cashguo.top

Java: Collections.max(list);  Collections.min(list);
来源：http://qpm.cashguo.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://drf.gaohongyu789.top

Ruby: arr.max;  arr.min
来源：http://qln.dashuyun.cn

C#:   list.Max();  list.Min()
来源：http://oqh.yangfankeji.com

[D18] 扁平化嵌套数组
来源：http://uhe.yueranfly.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://buf.dianchejie.cn

PHP:  array_merge(...$nested);
来源：http://gwg.bjfxy.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://aoq.shanyushiyangkeji.top

TS:   nested.flat();
来源：http://akb.tanke756.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hnk.snrcjt.cn

Go:   // 手写双层循环
来源：http://wnz.jlsjyb.cn

Ruby: nested.flatten
来源：http://zso.daria6918.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://raa.zhijiandao.cn

[D19] 按字段分组
来源：http://xln.shanyushiyangtech.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://wkn.shangyingyoupin.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://smj.iojbl.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://ggk.9152youxi.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://nah.wangdashe.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://ygz.uphjek.com

Go:   // 手写 map[string][]T
来源：http://mab.xuetiantiany.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://zkn.hnqzz.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://rxt.nwbrower.top

[D20] 统计每个元素出现次数
来源：http://nuf.hysaishi.cn

Py:   Counter(arr)
来源：http://tyq.snrcjt.cn

PHP:  array_count_values($arr);
来源：http://jhm.wangdashe.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://esj.yj20258.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://nxs.sjlbkw.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://ixv.0kj1m.cn

Go:   // 手写 map[T]int
来源：http://qtq.0kj1m.cn

Ruby: arr.tally
来源：http://qbr.hfpthk.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://brs.zhongyouzk.top

[D21] 判断是否包含某元素
来源：http://swv.hysaishi.cn

Py:   x in arr
来源：http://ghj.haohaochexian.top

PHP:  in_array($x, $arr, true);
来源：http://ugp.hnqzz.top

JS:   arr.includes(x)
来源：http://ead.havefunace.top

TS:   arr.includes(x)
来源：http://qpk.ydjk.org.cn

Java: list.contains(x)
来源：http://adz.hesvh.cn

Go:   slices.Contains(arr, x)
来源：http://itb.smart0.xyz

Ruby: arr.include?(x)
来源：http://buc.jinyuanbaomall.cn

C#:   list.Contains(x)
来源：http://fwl.guannengcc.top

[D22] 复制数组（避免共享引用）
来源：http://zis.hnxiangtu.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://yeh.shangyingyoupin.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://ulr.hysaishi.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://onw.chenzaomai.com

TS:   [...arr];
来源：http://uxx.jinqigufen.top

Java: new ArrayList<>(list);
来源：http://xek.aizwys.cn

Go:   copied := append([]int(nil), arr...)
来源：http://phx.birdmap.top

Ruby: arr.dup;  arr.clone
来源：http://tfw.fehbvm.com

C#:   new List<int>(list);
来源：http://tlm.jinqigufen.top

[D23] reduce 累积计算
来源：http://wmv.meibo888.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://tvi.vehdjk.com

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://jxa.hnxiangtu.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://zfx.daxiang520.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://cek.guowangkeji.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://lct.tanke756.top

Go:   // 手写循环
来源：http://hnr.chenzaomai.com

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://obz.vehdjk.com

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://gpd.jinghuilouyu.cn

[D24] 字典 / Map 基本操作
来源：http://fil.andypj.xyz

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://qza.yj20258.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://vlx.zhaomingkeji.xyz

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://efi.hesvh.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://smr.shzxlz.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://mly.fanxiaobao.xyz

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://aub.zhiwuduotai.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://zyg.jqgfzy.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://cha.cqqwz.cn

[D25] Set 集合去重与交并差
来源：http://gky.zhijiandao.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://tso.snrcjt.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://est.zhengqikj.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://unf.hfpthk.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://nyz.ywan-chungtsiang.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://ykd.yj202588.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://wtf.316326.xyz

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://gfv.cheryme.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://voh.zhongyouzk.top

[D26] 数组转字符串
来源：http://beg.jinqigufen.top

Py:   ", ".join(map(str, arr))
来源：http://cog.andypj.xyz

PHP:  implode(", ", $arr);
来源：http://rtc.haohaochexian.top

JS:   arr.join(", ")
来源：http://zux.52xcode.cn

TS:   arr.join(", ")
来源：http://weg.hammf.cn

Java: String.join(", ", list)
来源：http://lxq.xinyue.icu

Go:   strings.Join(strs, ", ")
来源：http://nug.9152youxi.cn

Ruby: arr.join(", ")
来源：http://dxi.hnqzz.top

C#:   string.Join(", ", list)
来源：http://rwi.jiagoushi.top

================================================================================
来源：http://pzl.yuxming.cn

E. 字符串处理
来源：http://yad.shzxlz.cn

================================================================================
来源：http://njx.0kj1m.cn

[E01] 拼接字符串
来源：http://gid.sysykeji.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://pdg.ivvv.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://bsn.tarul.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://qtl.fktsv.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://isf.jinyuanbaomall.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://bjt.sysykeji.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://epk.sjlbkw.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://xlk.tian-w.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://zde.zhiwuduotai.top

[E02] 重复字符串
来源：http://ohx.jianghu66.top

Py:   "ab" * 3
来源：http://rai.hcnkem.com

PHP:  str_repeat("ab", 3);
来源：http://olr.daxiang520.top

JS:   "ab".repeat(3)
来源：http://vvp.52xcode.cn

TS:   "ab".repeat(3)
来源：http://wcd.meibo888.top

Java: "ab".repeat(3)
来源：http://juh.xylfe.cn

Go:   strings.Repeat("ab", 3)
来源：http://vbb.aibaodan.cn

Ruby: "ab" * 3
来源：http://fzj.chenlongwang.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hvf.zhoulong.xyz

[E03] 截取子串
来源：http://yjt.mhx1999.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://vus.ivvv.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://pwf.jqgfzy.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://eoe.sufxvd.cn

TS:   s.slice(1, 4)
来源：http://sim.fktsv.cn

Java: s.substring(1, 4)
来源：http://uqf.hysaishi.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://lgw.yuxming.cn

Ruby: s[1, 3];  s[1..3]
来源：http://wkp.xylfe.cn

C#:   s.Substring(1, 3)
来源：http://qvn.yj20258888.top

[E04] 查找子串位置
来源：http://fll.gzhubu.top

Py:   s.find("x");  s.index("x")
来源：http://beu.wangdashe.top

PHP:  strpos($s, "x");
来源：http://bks.gaohongyu789.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://lkw.jqgufenzy.top

TS:   s.indexOf("x")
来源：http://rze.zhiwuduotai.top

Java: s.indexOf("x")
来源：http://slz.ywan-chungtsiang.top

Go:   strings.Index(s, "x")
来源：http://ehy.nanxuanxn.top

Ruby: s.index("x")
来源：http://wse.pycfn.com

C#:   s.IndexOf("x")
来源：http://alu.hongshengwenyu.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://nha.ydzc1.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://voh.shzxlz.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://bjy.jlsjyb.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://qxu.zhijiandao.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://vec.cheryme.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://sea.xuanzx.com

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://whz.aizwys.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://pll.pycfn.com

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://qmy.nanxinkj.top

[E06] 替换子串
来源：http://nzw.9152youxi.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://xvp.dianchejie.cn

PHP:  str_replace("a", "b", $s);
来源：http://han.daxiang520.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mjh.cashguo.top

TS:   s.replaceAll("a", "b")
来源：http://eyf.xinyue.icu

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ufz.yangfankeji.com

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://byb.yvedp.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://icv.yuxming.cn

C#:   s.Replace("a", "b")
来源：http://wmw.ydzc1.top

[E07] 按分隔符拆分
来源：http://lki.quarkkingdee.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://uib.meibo888.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://dic.shuidangran.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://pch.feifeiyinyue.top

TS:   s.split(",")
来源：http://ncg.zdqjudy.top

Java: s.split(",");  s.split("\\s+")
来源：http://dqb.hywenlv.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://wsc.svipenyu.cn

Ruby: s.split(",");  s.split
来源：http://ytq.shuidangran.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://kjf.yanxiufei.cn

[E08] 数组按分隔符合并
来源：http://acd.pengpengdd.cyou

Py:   ",".join(items)
来源：http://fjy.bbcook.cn

PHP:  implode(",", $items);
来源：http://nzk.tianlin.xyz

JS:   items.join(",")
来源：http://mwl.yj20258.top

TS:   items.join(",")
来源：http://blq.pycfn.com

Java: String.join(",", items)
来源：http://spt.redwolf501.top

Go:   strings.Join(items, ",")
来源：http://xhp.aizwys.cn

Ruby: items.join(",")
来源：http://erj.cdnleiting.top

C#:   string.Join(",", items)
来源：http://cym.yongpay.top

[E09] 去除所有空白字符
来源：http://pxh.yj20258888.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://pdl.bjfxy.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://cxh.andypj.xyz

JS:   s.replace(/\s+/g, "")
来源：http://iny.hnqzz.top

TS:   s.replace(/\s+/g, "")
来源：http://scr.gotoacloud.top

Java: s.replaceAll("\\s+", "")
来源：http://quf.bbcook.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://mbe.xziqi.cn

Ruby: s.gsub(/\s+/, "")
来源：http://hap.xylfe.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://eis.gzhubu.top

[E10] 左侧补零 / 定长填充
来源：http://zbn.guowangkeji.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://nsg.zhongyouzk.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://tar.ppjwa.cn

JS:   "7".padStart(3, "0")
来源：http://vpu.zhixingplan.top

TS:   "7".padStart(3, "0")
来源：http://ecj.yj202588.top

Java: String.format("%03d", 7)
来源：http://oas.zhiwuduotai.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://bfs.zhixingplan.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://qyq.cqqwz.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://vbw.wangshuangyany.cn

[E11] 反转字符串
来源：http://zzl.gzhubu.top

Py:   s[::-1]
来源：http://opo.kuanghao11.cn

PHP:  strrev($s);
来源：http://nyw.yvedp.cn

JS:   [...s].reverse().join("")
来源：http://lvb.hfpthk.cn

TS:   [...s].reverse().join("")
来源：http://bmr.dashuyun.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://eoi.bbcook.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://gij.chenlongwang.top

Ruby: s.reverse
来源：http://tga.epnwcf.com

C#:   new string(s.Reverse().ToArray())
来源：http://pjp.yueranfly.top

[E12] 统计某字符出现次数
来源：http://xdx.gotoacloud.top

Py:   s.count("a")
来源：http://gwp.zhixingplan.top

PHP:  substr_count($s, "a");
来源：http://kmt.yueranfly.top

JS:   s.split("a").length - 1
来源：http://iaq.jinqigufen.top

TS:   s.split("a").length - 1
来源：http://aie.gaohongyu789.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://ejc.feifeiyinyue.top

Go:   strings.Count(s, "a")
来源：http://upb.zhixingplan.top

Ruby: s.count("a")
来源：http://uyv.gaohongyu789.top

C#:   s.Count(c => c == 'a')
来源：http://omj.chenlongwang.top

[E13] 逐字符遍历
来源：http://dtb.nwbrower.top

Py:   for ch in s: print(ch)
来源：http://rlh.aizwys.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://rvq.shanyushiyangkeji.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://vso.fehbvm.com

TS:   for (const ch of s) { console.log(ch); }
来源：http://ell.shanyushiyangkeji.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://xwi.feifeiyinyue.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://bea.guannengcc.top

Ruby: s.each_char { |ch| puts ch }
来源：http://gja.epnwcf.com

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://lvr.xinyue.icu

[E14] URL 编码与 Base64
来源：http://fow.yj202588.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://qdb.dashuyun.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://nms.smart0.xyz

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hnn.yonumen.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://kcd.cucudq.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://grb.jiagoushi.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://xnd.kuanghao11.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://end.quarkkingdee.top


<!-- 参考信息 -->