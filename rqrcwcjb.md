代发 wailian999

Ruby: a + b;  a.concat(b)
来源：http://osi.havefunace.top

C#:   a.Concat(b).ToList()
来源：http://xvn.zhiwuduotai.top

[D09] 排序（升序）
来源：http://ubq.jlsjyb.cn

Py:   sorted(arr);  arr.sort()
来源：http://nsj.ydzc1.top

PHP:  sort($arr);
来源：http://bnu.chenjidiqi.icu

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://wfx.svipenyu.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://idg.xylfe.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://wad.shanyushiyangkeji.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://rzm.shanyushiyangtech.top

Ruby: arr.sort
来源：http://ayt.haohaochexian.top

C#:   list.Sort();
来源：http://oad.zhengqikj.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://src.jyoumei.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hsp.jiagoushi.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://gxb.zhengqikj.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://ifa.chenzaomai.com

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://zrh.yueranfly.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://agl.ctjpmb.com

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://unr.jinqigfzy.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://cud.sweek.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://oyg.cdnleiting.top

[D11] 反转数组
来源：http://kiz.uphjek.com

Py:   arr[::-1];  arr.reverse()
来源：http://npk.xuetiantiany.cn

PHP:  array_reverse($arr);
来源：http://xqh.gotoacloud.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://wvd.zhiwuduotai.top

TS:   [...arr].reverse();
来源：http://pma.xylfe.cn

Java: Collections.reverse(list);
来源：http://bib.nanxuanxn.top

Go:   slices.Reverse(arr)
来源：http://ifl.andypj.xyz

Ruby: arr.reverse
来源：http://pko.tanke756.top

C#:   list.Reverse();
来源：http://fud.iojbl.cn

[D12] 查找元素下标
来源：http://iok.birdmap.top

Py:   arr.index(x);  x in arr
来源：http://vbv.ctjpmb.com

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://fuq.haohaochexian.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://loo.jinqigfzy.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://yxk.shuidangran.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://cmj.zdqjudy.top

Go:   slices.Index(arr, x)
来源：http://opr.316326.xyz

Ruby: arr.index(x)
来源：http://miz.dianchejie.cn

C#:   list.IndexOf(x);
来源：http://jpn.uphjek.com

[D13] 过滤（保留满足条件的）
来源：http://hsw.jianghu66.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://tpw.haohaochexian.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://kij.zdqjudy.top

JS:   arr.filter(x => x > 3)
来源：http://jpp.tianlin.xyz

TS:   arr.filter(x => x > 3)
来源：http://orl.shzxlz.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://uop.wangdashe.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://pzs.jiagoushi.top

Ruby: arr.select { |x| x > 3 }
来源：http://nig.zhijiandao.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://sww.c1oappe.top

[D14] 映射转换（每个元素变形）
来源：http://fgs.jlsjyb.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://kao.ehwqpu.com

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://otu.ybcxt.top

JS:   arr.map(x => x * 2)
来源：http://zns.vehdjk.com

TS:   arr.map(x => x * 2)
来源：http://weu.zhongyouzk.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://zwc.zhoulong.xyz

Go:   // 手写循环
来源：http://tej.jyoumei.cn

Ruby: arr.map { |x| x * 2 }
来源：http://gzj.zdbjq.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://qqa.fengsongda.top

[D15] 去重
来源：http://vzc.c1oappe.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://vvd.andypj.xyz

PHP:  array_unique($arr);
来源：http://hso.dianchejie.cn

JS:   [...new Set(arr)]
来源：http://zdb.ybcxt.top

TS:   [...new Set(arr)]
来源：http://xlk.yonumen.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://qtv.gzhubu.top

Go:   // 用 map[T]struct{} 手写
来源：http://cmm.aizwys.cn

Ruby: arr.uniq
来源：http://ebr.xingfuxueyuan.xyz

C#:   list.Distinct().ToList()
来源：http://iom.chenzaomai.com

[D16] 求和与平均值
来源：http://led.havefunace.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://fix.gogol.net.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://zjf.jinqigfzy.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://web.ctjpmb.com

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://rmx.aibaodan.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://wom.jinqigfzy.top

Go:   // 手写循环累加
来源：http://nis.quarkkingdee.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://qjl.jqgfzy.top

C#:   list.Sum();  list.Average()
来源：http://upi.jlsjyb.cn

[D17] 最大值与最小值
来源：http://bnr.meibo888.top

Py:   max(arr);  min(arr)
来源：http://mmw.xziqi.cn

PHP:  max($arr);  min($arr);
来源：http://upt.hnxiangtu.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://myh.ybcxt.top

TS:   Math.max(...arr);
来源：http://jso.bjfxy.top

Java: Collections.max(list);  Collections.min(list);
来源：http://oms.pengpengdd.cyou

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://emi.shanyushiyangtech.top

Ruby: arr.max;  arr.min
来源：http://txv.yongpay.top

C#:   list.Max();  list.Min()
来源：http://ehp.cucudq.cn

[D18] 扁平化嵌套数组
来源：http://ygd.bjfxy.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://cio.jqgfzy.top

PHP:  array_merge(...$nested);
来源：http://tmv.zhongyouzk.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://ldz.nanxinkj.top

TS:   nested.flat();
来源：http://wdy.sweek.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://vfe.yj20258.top

Go:   // 手写双层循环
来源：http://hxg.jiagoushi.top

Ruby: nested.flatten
来源：http://ous.yueranfly.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://paa.zycfv.cn

[D19] 按字段分组
来源：http://hnw.52xcode.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://dfn.shuidangran.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://tbm.redwolf501.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://raa.tian-w.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://bbg.yvedp.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://rtw.shuidangran.top

Go:   // 手写 map[string][]T
来源：http://fdr.jinqigufen.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://ahm.quarkkingdee.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://zlq.nanxuanxn.top

[D20] 统计每个元素出现次数
来源：http://yue.yj20258888.top

Py:   Counter(arr)
来源：http://mwg.sweek.top

PHP:  array_count_values($arr);
来源：http://noi.hcnkem.com

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mwi.svipenyu.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://jjd.zhijiandao.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://pfk.fehbvm.com

Go:   // 手写 map[T]int
来源：http://mep.hcnkem.com

Ruby: arr.tally
来源：http://kgl.meibo888.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://iax.zhijiandao.cn

[D21] 判断是否包含某元素
来源：http://lqa.sjlbkw.cn

Py:   x in arr
来源：http://jsp.zhoulong.xyz

PHP:  in_array($x, $arr, true);
来源：http://hco.yj202588.top

JS:   arr.includes(x)
来源：http://bhm.gzhubu.top

TS:   arr.includes(x)
来源：http://pak.fzhhl.top

Java: list.contains(x)
来源：http://tyz.nanxinkj.top

Go:   slices.Contains(arr, x)
来源：http://uby.meibo888.top

Ruby: arr.include?(x)
来源：http://pkp.316326.xyz

C#:   list.Contains(x)
来源：http://zsm.jinghuilouyu.cn

[D22] 复制数组（避免共享引用）
来源：http://xcm.vqdsnc.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://jak.fzhhl.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://dgs.zhaomingkeji.xyz

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://gkm.zhiwuduotai.top

TS:   [...arr];
来源：http://lkk.shanyushiyangtech.top

Java: new ArrayList<>(list);
来源：http://qwm.gotoacloud.top

Go:   copied := append([]int(nil), arr...)
来源：http://rrm.guowangkeji.top

Ruby: arr.dup;  arr.clone
来源：http://tgr.dianchejie.cn

C#:   new List<int>(list);
来源：http://dlw.hywenlv.cn

[D23] reduce 累积计算
来源：http://yil.daria6918.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://cbo.hysaishi.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://ssc.wangshuangyany.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://kfx.jinqigfzy.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://afk.jiagoushi.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://xfi.yongpay.top

Go:   // 手写循环
来源：http://xaq.haohaochexian.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://gzm.hfpthk.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://ves.hammf.cn

[D24] 字典 / Map 基本操作
来源：http://qre.zhijiandao.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://tpg.vqdsnc.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hxg.vqdsnc.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://pei.xuetiantiany.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://agb.vqdsnc.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://plf.gzhubu.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://qcn.yfazqb.com

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://exq.hammf.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://srz.svipenyu.cn

[D25] Set 集合去重与交并差
来源：http://smf.tarul.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://vyf.xingfuxueyuan.xyz

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://fdl.ywan-chungtsiang.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://svp.andypj.xyz

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://ext.guannengcc.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://xzp.hysaishi.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://dnj.wangshuangyany.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://fjp.hysaishi.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://jgs.zhengqikj.top

[D26] 数组转字符串
来源：http://oxh.cqqwz.cn

Py:   ", ".join(map(str, arr))
来源：http://scz.jyoumei.cn

PHP:  implode(", ", $arr);
来源：http://bhl.jinyuanbaomall.cn

JS:   arr.join(", ")
来源：http://oib.xziqi.cn

TS:   arr.join(", ")
来源：http://kke.sysykeji.top

Java: String.join(", ", list)
来源：http://rxk.cdnleiting.top

Go:   strings.Join(strs, ", ")
来源：http://olo.yj20258.top

Ruby: arr.join(", ")
来源：http://mpx.jinqigfzy.top

C#:   string.Join(", ", list)
来源：http://cmk.zdqjudy.top

================================================================================
来源：http://ehz.snrcjt.cn

E. 字符串处理
来源：http://zqw.chenlongwang.top

================================================================================
来源：http://cxa.sysykeji.top

[E01] 拼接字符串
来源：http://qlg.fzhhl.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://zsv.ydzc1.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://ocg.aibaodan.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://anp.cashguo.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://cga.jinqigufen.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://nre.smart0.xyz

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://ayo.jyoumei.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://vfw.haohaochexian.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://auq.xylfe.cn

[E02] 重复字符串
来源：http://add.gzhubu.top

Py:   "ab" * 3
来源：http://snp.cdnleiting.top

PHP:  str_repeat("ab", 3);
来源：http://yiy.hammf.cn

JS:   "ab".repeat(3)
来源：http://rxa.cheryme.top

TS:   "ab".repeat(3)
来源：http://xmw.bbcook.cn

Java: "ab".repeat(3)
来源：http://tqo.ctjpmb.com

Go:   strings.Repeat("ab", 3)
来源：http://xam.quarkkingdee.top

Ruby: "ab" * 3
来源：http://uam.jinghuilouyu.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://gtc.aibaodan.cn

[E03] 截取子串
来源：http://jzy.xinyue.icu

Py:   s[1:4];  s[:3];  s[3:]
来源：http://tmn.hywenlv.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://rlb.hnqzz.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://sjg.shuidangran.top

TS:   s.slice(1, 4)
来源：http://yxb.cheryme.top

Java: s.substring(1, 4)
来源：http://com.snrcjt.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://pfi.mhx1999.top

Ruby: s[1, 3];  s[1..3]
来源：http://dxm.hnxiangtu.top

C#:   s.Substring(1, 3)
来源：http://wlm.dianchejie.cn

[E04] 查找子串位置
来源：http://mqv.xinyue.icu

Py:   s.find("x");  s.index("x")
来源：http://zun.fktsv.cn

PHP:  strpos($s, "x");
来源：http://xxn.yj20258888.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://oun.zhixingplan.top

TS:   s.indexOf("x")
来源：http://agb.vehdjk.com

Java: s.indexOf("x")
来源：http://zqw.jinqigfzy.top

Go:   strings.Index(s, "x")
来源：http://png.svipenyu.cn

Ruby: s.index("x")
来源：http://pcg.chenzaomai.com

C#:   s.IndexOf("x")
来源：http://tfc.xuetiantiany.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://xho.zhijiandao.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://ioe.yuanzhike.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://ipb.zhaomingkeji.xyz

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://cqf.ywan-chungtsiang.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://mij.bbcook.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://glj.ppjwa.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://cgh.nanxuanxn.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://tmk.xziqi.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://fdg.c1oappe.top

[E06] 替换子串
来源：http://ljq.sxryk.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://eat.bbcook.cn

PHP:  str_replace("a", "b", $s);
来源：http://asw.haohaochexian.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://swi.bjfxy.top

TS:   s.replaceAll("a", "b")
来源：http://mvt.zdbjq.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://akm.jinqigufen.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://fsu.guannengcc.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://ltv.yangfankeji.com

C#:   s.Replace("a", "b")
来源：http://vhk.yuxming.cn

[E07] 按分隔符拆分
来源：http://hux.uphjek.com

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://lek.daria6918.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://brr.chenzaomai.com

JS:   s.split(",");  s.split(/\s+/)
来源：http://rbj.wangdashe.top

TS:   s.split(",")
来源：http://keb.hammf.cn

Java: s.split(",");  s.split("\\s+")
来源：http://bmh.hcnkem.com

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://ohg.52xcode.cn

Ruby: s.split(",");  s.split
来源：http://fho.zhixingplan.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://aly.meibo888.top

[E08] 数组按分隔符合并
来源：http://upu.yj20258.top

Py:   ",".join(items)
来源：http://uim.iojbl.cn

PHP:  implode(",", $items);
来源：http://jbk.guannengcc.top

JS:   items.join(",")
来源：http://xoi.dashuyun.cn

TS:   items.join(",")
来源：http://rmv.zhaomingkeji.xyz

Java: String.join(",", items)
来源：http://hab.xingfuxueyuan.xyz

Go:   strings.Join(items, ",")
来源：http://usk.xuanzx.com

Ruby: items.join(",")
来源：http://sfb.daria6918.cn

C#:   string.Join(",", items)
来源：http://buv.xuetiantiany.cn

[E09] 去除所有空白字符
来源：http://lsm.xuanzx.com

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://blh.yonumen.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://ydo.jinqigfzy.top

JS:   s.replace(/\s+/g, "")
来源：http://asc.uphjek.com

TS:   s.replace(/\s+/g, "")
来源：http://aen.c1oappe.top

Java: s.replaceAll("\\s+", "")
来源：http://hxi.mhx1999.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://itf.ctjpmb.com

Ruby: s.gsub(/\s+/, "")
来源：http://sro.yj20258.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://lbp.vqdsnc.cn

[E10] 左侧补零 / 定长填充
来源：http://xfi.xinyue.icu

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://ksq.uphjek.com

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://gmh.fengsongda.top

JS:   "7".padStart(3, "0")
来源：http://zrp.yuanzhike.top

TS:   "7".padStart(3, "0")
来源：http://cia.jinqigfzy.top

Java: String.format("%03d", 7)
来源：http://scy.xinyue.icu

Go:   fmt.Sprintf("%03d", 7)
来源：http://lcl.yj20258.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://dhx.ywan-chungtsiang.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://kkv.meibo888.top

[E11] 反转字符串
来源：http://pcu.tarul.cn

Py:   s[::-1]
来源：http://fhe.jianghu66.top

PHP:  strrev($s);
来源：http://idc.gaohongyu789.top

JS:   [...s].reverse().join("")
来源：http://kgr.hfpthk.cn

TS:   [...s].reverse().join("")
来源：http://lgk.hywenlv.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://ajn.shzxlz.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://ker.bbcook.cn

Ruby: s.reverse
来源：http://awq.zhixingplan.top

C#:   new string(s.Reverse().ToArray())
来源：http://ddk.ehwqpu.com

[E12] 统计某字符出现次数
来源：http://gca.chenzaomai.com

Py:   s.count("a")
来源：http://vhi.ppjwa.cn

PHP:  substr_count($s, "a");
来源：http://wio.nwbrower.top

JS:   s.split("a").length - 1
来源：http://mhn.iojbl.cn

TS:   s.split("a").length - 1
来源：http://drs.zdqjudy.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://ukk.fzhhl.top

Go:   strings.Count(s, "a")
来源：http://usy.hesvh.cn

Ruby: s.count("a")
来源：http://wio.quarkkingdee.top

C#:   s.Count(c => c == 'a')
来源：http://fmo.zhijiandao.cn

[E13] 逐字符遍历
来源：http://lmt.gzhubu.top

Py:   for ch in s: print(ch)
来源：http://rzb.52xcode.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://sgj.nwbrower.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://beg.pycfn.com

TS:   for (const ch of s) { console.log(ch); }
来源：http://klf.nanxinkj.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://zbk.chenjidiqi.icu

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://ofk.fzhhl.top

Ruby: s.each_char { |ch| puts ch }
来源：http://wor.zhaomingkeji.xyz

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://bgk.kuanghao11.cn

[E14] URL 编码与 Base64
来源：http://edf.316326.xyz

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://qla.chenzaomai.com

PHP:  urlencode($s);  base64_encode($s);
来源：http://wsc.yonumen.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://ykt.havefunace.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://guq.zhongyouzk.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://bsz.zdbjq.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://oue.tarul.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://tfr.sxryk.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://mvs.tianlin.xyz

[E15] HTML 转义 / 反转义
来源：http://hlr.xuetiantiany.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://yth.xingfuxueyuan.xyz

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://dhy.epnwcf.com

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://vma.fengsongda.top

TS:   // 同上，务必做 XSS 过滤
来源：http://dpv.smart0.xyz

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://vwt.yj20258888.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://gyq.zhengqikj.top


<!-- 参考信息 -->