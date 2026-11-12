代发 wailian999

JS:   [...a, ...b];  a.concat(b);
来源：http://pcv.ywan-chungtsiang.top

TS:   [...a, ...b];
来源：http://feh.gogol.net.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://fdn.sjlbkw.cn

Go:   append(a, b...)
来源：http://fjk.jinyuanbaomall.cn

Ruby: a + b;  a.concat(b)
来源：http://iem.jlsjyb.cn

C#:   a.Concat(b).ToList()
来源：http://ths.andypj.xyz

[D09] 排序（升序）
来源：http://crx.jinqigfzy.top

Py:   sorted(arr);  arr.sort()
来源：http://jrp.pycfn.com

PHP:  sort($arr);
来源：http://hxg.zhixingplan.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://tky.pycfn.com

TS:   [...arr].sort((x, y) => x - y);
来源：http://vnv.pengpengdd.cyou

Java: Collections.sort(list);  list.sort(null);
来源：http://mhz.pengpengdd.cyou

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://vvb.hongshengwenyu.top

Ruby: arr.sort
来源：http://lmj.haohaochexian.top

C#:   list.Sort();
来源：http://vyh.jinqigufen.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://nxq.cdnleiting.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://mwz.havefunace.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ush.ppjwa.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://ike.xylfe.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://nxf.epnwcf.com

Java: list.sort(Comparator.comparing(Person::age));
来源：http://cmc.iojbl.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://jzj.nanxinkj.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://gfw.aibaodan.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://otj.yangfankeji.com

[D11] 反转数组
来源：http://iqy.kuanghao11.cn

Py:   arr[::-1];  arr.reverse()
来源：http://kek.jinqigufen.top

PHP:  array_reverse($arr);
来源：http://rxe.yonumen.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://qzu.yuxming.cn

TS:   [...arr].reverse();
来源：http://mhr.guowangkeji.top

Java: Collections.reverse(list);
来源：http://aun.0kj1m.cn

Go:   slices.Reverse(arr)
来源：http://mqq.cashguo.top

Ruby: arr.reverse
来源：http://pxu.xinyue.icu

C#:   list.Reverse();
来源：http://axg.gzhubu.top

[D12] 查找元素下标
来源：http://jwa.nanxuanxn.top

Py:   arr.index(x);  x in arr
来源：http://dwb.hnxiangtu.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://bgy.ivvv.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://kyu.yvedp.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ntk.hnqzz.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://qli.xylfe.cn

Go:   slices.Index(arr, x)
来源：http://bpd.xingfuxueyuan.xyz

Ruby: arr.index(x)
来源：http://czk.ybcxt.top

C#:   list.IndexOf(x);
来源：http://fqz.quarkkingdee.top

[D13] 过滤（保留满足条件的）
来源：http://kpm.ydzc1.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://pby.xuetiantiany.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://ruy.jinqigfzy.top

JS:   arr.filter(x => x > 3)
来源：http://gaq.fktsv.cn

TS:   arr.filter(x => x > 3)
来源：http://tcg.shuidangran.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://xtp.xinyue.icu

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://kav.cucudq.cn

Ruby: arr.select { |x| x > 3 }
来源：http://san.shzxlz.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://nod.bbcook.cn

[D14] 映射转换（每个元素变形）
来源：http://oqn.snrcjt.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://cqu.yj20258.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://pug.yvedp.cn

JS:   arr.map(x => x * 2)
来源：http://inb.xuetiantiany.cn

TS:   arr.map(x => x * 2)
来源：http://kje.hysaishi.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://bla.jinqigufen.top

Go:   // 手写循环
来源：http://fur.xuanzx.com

Ruby: arr.map { |x| x * 2 }
来源：http://ffg.jinyuanbaomall.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://wve.hnxiangtu.top

[D15] 去重
来源：http://ysb.ydjk.org.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://wmj.sufxvd.cn

PHP:  array_unique($arr);
来源：http://sry.zhaomingkeji.xyz

JS:   [...new Set(arr)]
来源：http://act.zdbjq.cn

TS:   [...new Set(arr)]
来源：http://kwm.jinqigfzy.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://qzz.gzhubu.top

Go:   // 用 map[T]struct{} 手写
来源：http://wgv.meibo888.top

Ruby: arr.uniq
来源：http://gtj.gogol.net.cn

C#:   list.Distinct().ToList()
来源：http://hcv.zycfv.cn

[D16] 求和与平均值
来源：http://hwm.pengpengdd.cyou

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://dal.bjfxy.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://uto.hywenlv.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://gjn.sxryk.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://pel.zhijiandao.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://njd.jinghuilouyu.cn

Go:   // 手写循环累加
来源：http://eqt.bbcook.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://nbp.dianchejie.cn

C#:   list.Sum();  list.Average()
来源：http://cwd.gzhubu.top

[D17] 最大值与最小值
来源：http://bor.hnqzz.top

Py:   max(arr);  min(arr)
来源：http://kkq.ppjwa.cn

PHP:  max($arr);  min($arr);
来源：http://abj.ppjwa.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://lfj.ydzc1.top

TS:   Math.max(...arr);
来源：http://nzi.xinyue.icu

Java: Collections.max(list);  Collections.min(list);
来源：http://wlk.fanxiaobao.xyz

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://ttl.ydjk.org.cn

Ruby: arr.max;  arr.min
来源：http://qkc.yangfankeji.com

C#:   list.Max();  list.Min()
来源：http://eco.nwbrower.top

[D18] 扁平化嵌套数组
来源：http://zto.andypj.xyz

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://wmt.cdnleiting.top

PHP:  array_merge(...$nested);
来源：http://jzk.tarul.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://exq.fengsongda.top

TS:   nested.flat();
来源：http://uhc.sxryk.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://pgt.sjlbkw.cn

Go:   // 手写双层循环
来源：http://wkc.hfpthk.cn

Ruby: nested.flatten
来源：http://kqi.ctjpmb.com

C#:   nested.SelectMany(x => x).ToList()
来源：http://thg.shangyingyoupin.top

[D19] 按字段分组
来源：http://qbd.nanxinkj.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://wlo.zhiwuduotai.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://ggw.hysaishi.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://gft.fehbvm.com

TS:   Object.groupBy(arr, x => x.type)
来源：http://fbj.ywan-chungtsiang.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://lgj.zycfv.cn

Go:   // 手写 map[string][]T
来源：http://jvy.wangdashe.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://yij.andypj.xyz

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hlk.yonumen.top

[D20] 统计每个元素出现次数
来源：http://daf.yangfankeji.com

Py:   Counter(arr)
来源：http://hwq.fanxiaobao.xyz

PHP:  array_count_values($arr);
来源：http://vam.daxiang520.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://nlt.xylfe.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://tyq.chenjidiqi.icu

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://luv.redwolf501.top

Go:   // 手写 map[T]int
来源：http://lnw.daxiang520.top

Ruby: arr.tally
来源：http://qdk.nanxinkj.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://yty.hfpthk.cn

[D21] 判断是否包含某元素
来源：http://oeg.ehwqpu.com

Py:   x in arr
来源：http://jpt.zhongyouzk.top

PHP:  in_array($x, $arr, true);
来源：http://nkq.birdmap.top

JS:   arr.includes(x)
来源：http://njy.ivvv.top

TS:   arr.includes(x)
来源：http://tqh.sxryk.cn

Java: list.contains(x)
来源：http://fdh.jinqigfzy.top

Go:   slices.Contains(arr, x)
来源：http://iag.hcnkem.com

Ruby: arr.include?(x)
来源：http://rsr.xylfe.cn

C#:   list.Contains(x)
来源：http://cag.zycfv.cn

[D22] 复制数组（避免共享引用）
来源：http://mod.redwolf501.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://ihq.ydzc1.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hst.fktsv.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://vsb.shangyingyoupin.top

TS:   [...arr];
来源：http://ksw.xziqi.cn

Java: new ArrayList<>(list);
来源：http://yyr.cucudq.cn

Go:   copied := append([]int(nil), arr...)
来源：http://glw.tian-w.cn

Ruby: arr.dup;  arr.clone
来源：http://tso.tianlin.xyz

C#:   new List<int>(list);
来源：http://yzw.havefunace.top

[D23] reduce 累积计算
来源：http://yoz.guannengcc.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://pxm.yangfankeji.com

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://pal.jinyuanbaomall.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://xeb.svipenyu.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ivc.fehbvm.com

Java: list.stream().reduce(0, Integer::sum)
来源：http://unu.wangshuangyany.cn

Go:   // 手写循环
来源：http://vho.xuanzx.com

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://nqf.daria6918.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://tkl.yj20258.top

[D24] 字典 / Map 基本操作
来源：http://ion.pengpengdd.cyou

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://huk.yangfankeji.com

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://ano.shuidangran.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://zjh.9152youxi.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://nti.cqqwz.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://iph.shuidangran.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://jdi.chenjidiqi.icu

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://erg.shuidangran.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://dal.fzhhl.top

[D25] Set 集合去重与交并差
来源：http://tmb.guowangkeji.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://ycx.sweek.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://tfs.c1oappe.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://gdo.gotoacloud.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://ote.hfpthk.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://vmi.hnqzz.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://rqb.guowangkeji.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://vrg.mhx1999.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://wbl.ywan-chungtsiang.top

[D26] 数组转字符串
来源：http://rve.gaohongyu789.top

Py:   ", ".join(map(str, arr))
来源：http://vib.quarkkingdee.top

PHP:  implode(", ", $arr);
来源：http://zok.zhengqikj.top

JS:   arr.join(", ")
来源：http://qtl.snrcjt.cn

TS:   arr.join(", ")
来源：http://fta.zhaomingkeji.xyz

Java: String.join(", ", list)
来源：http://yob.yongpay.top

Go:   strings.Join(strs, ", ")
来源：http://pfq.hongshengwenyu.top

Ruby: arr.join(", ")
来源：http://wpk.hcnkem.com

C#:   string.Join(", ", list)
来源：http://nby.jinqigufen.top

================================================================================
来源：http://gkh.dianchejie.cn

E. 字符串处理
来源：http://mpg.jlsjyb.cn

================================================================================
来源：http://upv.jinqigufen.top

[E01] 拼接字符串
来源：http://tkx.hesvh.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://rhf.ctjpmb.com

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://dpw.ywan-chungtsiang.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://qzb.0kj1m.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://erl.ppjwa.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hcz.fzhhl.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://kvn.yangfankeji.com

Ruby: "a" + "b";  ["a", "b"].join
来源：http://egx.52xcode.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://ywn.vqdsnc.cn

[E02] 重复字符串
来源：http://tst.gogol.net.cn

Py:   "ab" * 3
来源：http://ajp.cucudq.cn

PHP:  str_repeat("ab", 3);
来源：http://xtp.nanxinkj.top

JS:   "ab".repeat(3)
来源：http://qfm.bjfxy.top

TS:   "ab".repeat(3)
来源：http://ifn.zhaomingkeji.xyz

Java: "ab".repeat(3)
来源：http://yiy.hcnkem.com

Go:   strings.Repeat("ab", 3)
来源：http://mmn.hysaishi.cn

Ruby: "ab" * 3
来源：http://iyc.yj202588.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://zcf.daxiang520.top

[E03] 截取子串
来源：http://kif.haohaochexian.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://fsx.yj202588.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://wsy.aizwys.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://neh.hnxiangtu.top

TS:   s.slice(1, 4)
来源：http://eoh.bjfxy.top

Java: s.substring(1, 4)
来源：http://azh.zhaomingkeji.xyz

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://ryf.haohaochexian.top

Ruby: s[1, 3];  s[1..3]
来源：http://kgp.cucudq.cn

C#:   s.Substring(1, 3)
来源：http://bhq.sjlbkw.cn

[E04] 查找子串位置
来源：http://qig.zdbjq.cn

Py:   s.find("x");  s.index("x")
来源：http://skj.havefunace.top

PHP:  strpos($s, "x");
来源：http://gzj.yonumen.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://cqy.jiagoushi.top

TS:   s.indexOf("x")
来源：http://nye.shangyingyoupin.top

Java: s.indexOf("x")
来源：http://evi.kuanghao11.cn

Go:   strings.Index(s, "x")
来源：http://gdk.xuanzx.com

Ruby: s.index("x")
来源：http://jtz.ydjk.org.cn

C#:   s.IndexOf("x")
来源：http://prn.zhixingplan.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://axk.9152youxi.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://etu.quarkkingdee.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://lot.sxryk.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ukq.gotoacloud.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://pfx.nanxinkj.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ykg.cucudq.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://fgc.yvedp.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://bay.zhengqikj.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://xze.chenzaomai.com

[E06] 替换子串
来源：http://dyj.fengsongda.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://xpd.jinqigufen.top

PHP:  str_replace("a", "b", $s);
来源：http://qcz.jlsjyb.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://coh.shzxlz.cn

TS:   s.replaceAll("a", "b")
来源：http://uwj.chenlongwang.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ojg.shanyushiyangkeji.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://oou.zhengqikj.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://gyo.vqdsnc.cn

C#:   s.Replace("a", "b")
来源：http://gxu.zhongyouzk.top

[E07] 按分隔符拆分
来源：http://nkc.jqgufenzy.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://ytt.epnwcf.com

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://rtk.mhx1999.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://ueh.gaohongyu789.top

TS:   s.split(",")
来源：http://kjd.chenjidiqi.icu

Java: s.split(",");  s.split("\\s+")
来源：http://plg.ctjpmb.com

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://pqj.birdmap.top

Ruby: s.split(",");  s.split
来源：http://fcn.vqdsnc.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://lmp.gzhubu.top

[E08] 数组按分隔符合并
来源：http://sth.ctjpmb.com

Py:   ",".join(items)
来源：http://tjk.jqgufenzy.top

PHP:  implode(",", $items);
来源：http://lml.jinqigfzy.top

JS:   items.join(",")
来源：http://biw.havefunace.top

TS:   items.join(",")
来源：http://eie.ppjwa.cn

Java: String.join(",", items)
来源：http://zfo.cashguo.top

Go:   strings.Join(items, ",")
来源：http://qcz.redwolf501.top

Ruby: items.join(",")
来源：http://ekt.xinyue.icu

C#:   string.Join(",", items)
来源：http://mdt.mhx1999.top

[E09] 去除所有空白字符
来源：http://oxh.zycfv.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://gsc.hnqzz.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://mac.sysykeji.top

JS:   s.replace(/\s+/g, "")
来源：http://azs.vqdsnc.cn

TS:   s.replace(/\s+/g, "")
来源：http://bfv.pycfn.com

Java: s.replaceAll("\\s+", "")
来源：http://zqx.yueranfly.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://fkx.tian-w.cn

Ruby: s.gsub(/\s+/, "")
来源：http://hwl.xylfe.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://czu.yj202588.top

[E10] 左侧补零 / 定长填充
来源：http://rtk.xuetiantiany.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://srk.yonumen.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://ped.nanxuanxn.top

JS:   "7".padStart(3, "0")
来源：http://cpl.havefunace.top

TS:   "7".padStart(3, "0")
来源：http://jsj.jlsjyb.cn

Java: String.format("%03d", 7)
来源：http://pip.jinyuanbaomall.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://zrz.hywenlv.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://xxj.yj20258.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hhd.guowangkeji.top

[E11] 反转字符串
来源：http://jmr.ybcxt.top

Py:   s[::-1]
来源：http://dsv.hnqzz.top

PHP:  strrev($s);
来源：http://vod.jianghu66.top

JS:   [...s].reverse().join("")
来源：http://tof.shanyushiyangtech.top

TS:   [...s].reverse().join("")
来源：http://mwq.zhixingplan.top

Java: new StringBuilder(s).reverse().toString()
来源：http://xcx.birdmap.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://gql.xylfe.cn

Ruby: s.reverse
来源：http://pro.zhongyouzk.top

C#:   new string(s.Reverse().ToArray())
来源：http://pkw.guannengcc.top

[E12] 统计某字符出现次数
来源：http://vfb.jqgfzy.top

Py:   s.count("a")
来源：http://mbd.mhx1999.top

PHP:  substr_count($s, "a");
来源：http://zuy.fehbvm.com

JS:   s.split("a").length - 1
来源：http://rid.jiagoushi.top

TS:   s.split("a").length - 1
来源：http://olb.nwbrower.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://yxh.vehdjk.com

Go:   strings.Count(s, "a")
来源：http://srr.zhaomingkeji.xyz

Ruby: s.count("a")
来源：http://jyg.haohaochexian.top

C#:   s.Count(c => c == 'a')
来源：http://tlv.cashguo.top

[E13] 逐字符遍历
来源：http://zpl.zdbjq.cn

Py:   for ch in s: print(ch)
来源：http://buc.bjfxy.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://oal.tanke756.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://wxh.jinqigufen.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://nei.yuanzhike.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://gyw.hysaishi.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://cbk.dianchejie.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://biz.yongpay.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://bxp.chenjidiqi.icu

[E14] URL 编码与 Base64
来源：http://kiz.pycfn.com

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://rnr.sufxvd.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://mpw.chenjidiqi.icu

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://ipa.tian-w.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://nee.ybcxt.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://tfp.hnqzz.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://epn.aizwys.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://xjs.yanxiufei.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://szw.smart0.xyz

[E15] HTML 转义 / 反转义
来源：http://ahv.zhoulong.xyz

Py:   html.escape(s);  html.unescape(s)
来源：http://wqy.bjfxy.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://nlp.zhoulong.xyz


<!-- 参考信息 -->