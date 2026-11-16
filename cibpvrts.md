代发 wailian999

C#:   list.GetRange(1, 3);
来源：http://dny.fzhhl.top

[D08] 合并两个数组
来源：http://qst.yuxming.cn

Py:   a + b;  a.extend(b)
来源：http://dvg.tarul.cn

PHP:  array_merge($a, $b);
来源：http://kex.hnxiangtu.top

JS:   [...a, ...b];  a.concat(b);
来源：http://vrb.yvedp.cn

TS:   [...a, ...b];
来源：http://hij.tianlin.xyz

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://qhk.tanke756.top

Go:   append(a, b...)
来源：http://vlm.dashuyun.cn

Ruby: a + b;  a.concat(b)
来源：http://roy.gotoacloud.top

C#:   a.Concat(b).ToList()
来源：http://orm.sysykeji.top

[D09] 排序（升序）
来源：http://krm.xingfuxueyuan.xyz

Py:   sorted(arr);  arr.sort()
来源：http://nek.gaohongyu789.top

PHP:  sort($arr);
来源：http://bcm.0kj1m.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://mgo.gaohongyu789.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://rkh.52xcode.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://xsr.yj20258888.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://ctj.zdbjq.cn

Ruby: arr.sort
来源：http://ikn.yuxming.cn

C#:   list.Sort();
来源：http://tza.fengsongda.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://unl.fktsv.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://qve.xingfuxueyuan.xyz

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://rrq.yangfankeji.com

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://xvy.zdqjudy.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://iyo.shanyushiyangkeji.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://cce.zhaomingkeji.xyz

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://sop.yueranfly.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://fij.zdqjudy.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://lvd.hesvh.cn

[D11] 反转数组
来源：http://abj.vehdjk.com

Py:   arr[::-1];  arr.reverse()
来源：http://gak.tarul.cn

PHP:  array_reverse($arr);
来源：http://rea.jinyuanbaomall.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://oxt.quarkkingdee.top

TS:   [...arr].reverse();
来源：http://jtd.feifeiyinyue.top

Java: Collections.reverse(list);
来源：http://vws.yj20258888.top

Go:   slices.Reverse(arr)
来源：http://gcl.fzhhl.top

Ruby: arr.reverse
来源：http://lau.jlsjyb.cn

C#:   list.Reverse();
来源：http://snk.fanxiaobao.xyz

[D12] 查找元素下标
来源：http://wiz.feifeiyinyue.top

Py:   arr.index(x);  x in arr
来源：http://hhq.hfpthk.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://efz.hesvh.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ree.cucudq.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://xvj.jqgufenzy.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://ahu.jlsjyb.cn

Go:   slices.Index(arr, x)
来源：http://nip.shanyushiyangtech.top

Ruby: arr.index(x)
来源：http://mjm.nanxuanxn.top

C#:   list.IndexOf(x);
来源：http://xpm.birdmap.top

[D13] 过滤（保留满足条件的）
来源：http://den.hfpthk.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://han.redwolf501.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://ojv.ybcxt.top

JS:   arr.filter(x => x > 3)
来源：http://jqt.tianlin.xyz

TS:   arr.filter(x => x > 3)
来源：http://aih.uphjek.com

Java: list.stream().filter(x -> x > 3).toList()
来源：http://ajj.ppjwa.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://afp.chenzaomai.com

Ruby: arr.select { |x| x > 3 }
来源：http://idd.feifeiyinyue.top

C#:   list.Where(x => x > 3).ToList()
来源：http://pfj.chenlongwang.top

[D14] 映射转换（每个元素变形）
来源：http://qmp.gogol.net.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://ies.daria6918.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://pes.svipenyu.cn

JS:   arr.map(x => x * 2)
来源：http://tzq.jinqigfzy.top

TS:   arr.map(x => x * 2)
来源：http://ysa.iojbl.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://bij.ybcxt.top

Go:   // 手写循环
来源：http://mjl.jinghuilouyu.cn

Ruby: arr.map { |x| x * 2 }
来源：http://qdl.sjlbkw.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://evo.nanxinkj.top

[D15] 去重
来源：http://rzt.dashuyun.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://itj.kuanghao11.cn

PHP:  array_unique($arr);
来源：http://uyy.tian-w.cn

JS:   [...new Set(arr)]
来源：http://jwy.xinyue.icu

TS:   [...new Set(arr)]
来源：http://omv.iojbl.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://mad.chenzaomai.com

Go:   // 用 map[T]struct{} 手写
来源：http://ubg.ehwqpu.com

Ruby: arr.uniq
来源：http://lid.jlsjyb.cn

C#:   list.Distinct().ToList()
来源：http://iaj.sweek.top

[D16] 求和与平均值
来源：http://byp.ppjwa.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://pic.hnxiangtu.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://ivr.nanxinkj.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://wqi.bjfxy.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://chz.zhongyouzk.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hvy.xingfuxueyuan.xyz

Go:   // 手写循环累加
来源：http://btc.xziqi.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://qrr.daxiang520.top

C#:   list.Sum();  list.Average()
来源：http://zbs.havefunace.top

[D17] 最大值与最小值
来源：http://dcc.xylfe.cn

Py:   max(arr);  min(arr)
来源：http://dil.sufxvd.cn

PHP:  max($arr);  min($arr);
来源：http://yqg.yj20258888.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://gnz.daria6918.cn

TS:   Math.max(...arr);
来源：http://nlu.jqgfzy.top

Java: Collections.max(list);  Collections.min(list);
来源：http://ijj.ydjk.org.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://qjs.pengpengdd.cyou

Ruby: arr.max;  arr.min
来源：http://fzu.nanxuanxn.top

C#:   list.Max();  list.Min()
来源：http://uhq.zhengqikj.top

[D18] 扁平化嵌套数组
来源：http://jao.chenzaomai.com

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://ody.shzxlz.cn

PHP:  array_merge(...$nested);
来源：http://luy.yj20258888.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hfl.bbcook.cn

TS:   nested.flat();
来源：http://wbi.guowangkeji.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://tfp.svipenyu.cn

Go:   // 手写双层循环
来源：http://knk.ybcxt.top

Ruby: nested.flatten
来源：http://pyg.mhx1999.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://hne.jinyuanbaomall.cn

[D19] 按字段分组
来源：http://azl.uphjek.com

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://jte.sufxvd.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://mpc.dianchejie.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://pkc.zhongyouzk.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://wqb.pengpengdd.cyou

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://quv.aibaodan.cn

Go:   // 手写 map[string][]T
来源：http://dia.hnqzz.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://zkz.tarul.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://ujv.shuidangran.top

[D20] 统计每个元素出现次数
来源：http://inb.wangshuangyany.cn

Py:   Counter(arr)
来源：http://ofv.epnwcf.com

PHP:  array_count_values($arr);
来源：http://ycw.nanxuanxn.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://jun.nanxinkj.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://zeg.guannengcc.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hnp.fehbvm.com

Go:   // 手写 map[T]int
来源：http://jkz.yangfankeji.com

Ruby: arr.tally
来源：http://kvj.uphjek.com

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://vtr.yangfankeji.com

[D21] 判断是否包含某元素
来源：http://xdw.aizwys.cn

Py:   x in arr
来源：http://msu.havefunace.top

PHP:  in_array($x, $arr, true);
来源：http://ifs.ctjpmb.com

JS:   arr.includes(x)
来源：http://rso.jqgfzy.top

TS:   arr.includes(x)
来源：http://cum.zdqjudy.top

Java: list.contains(x)
来源：http://twa.ydzc1.top

Go:   slices.Contains(arr, x)
来源：http://grn.jinqigufen.top

Ruby: arr.include?(x)
来源：http://xxr.yongpay.top

C#:   list.Contains(x)
来源：http://lsz.guowangkeji.top

[D22] 复制数组（避免共享引用）
来源：http://bmw.shanyushiyangtech.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://ydz.uphjek.com

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://yfy.zhongyouzk.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://iur.shzxlz.cn

TS:   [...arr];
来源：http://nzu.kuanghao11.cn

Java: new ArrayList<>(list);
来源：http://ccs.hfpthk.cn

Go:   copied := append([]int(nil), arr...)
来源：http://dau.fzhhl.top

Ruby: arr.dup;  arr.clone
来源：http://oyu.snrcjt.cn

C#:   new List<int>(list);
来源：http://gkt.redwolf501.top

[D23] reduce 累积计算
来源：http://lae.jinqigufen.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://kit.yj20258.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://svl.cheryme.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://smv.ppjwa.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://xhl.jyoumei.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://jjo.jianghu66.top

Go:   // 手写循环
来源：http://qpa.sysykeji.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://zub.xylfe.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://jbh.jinqigfzy.top

[D24] 字典 / Map 基本操作
来源：http://yje.fengsongda.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://nlb.gogol.net.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://eep.jinqigfzy.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://ofr.sufxvd.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://khn.zhengqikj.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://ajq.ivvv.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://dxa.cdnleiting.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://avw.hcnkem.com

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://kdb.hammf.cn

[D25] Set 集合去重与交并差
来源：http://ijm.shanyushiyangkeji.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://kqi.shanyushiyangkeji.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://ztv.zhoulong.xyz

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://qhz.sjlbkw.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://mab.316326.xyz

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://qby.dianchejie.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://acz.tarul.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://deg.tanke756.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://vds.ydjk.org.cn

[D26] 数组转字符串
来源：http://hzy.birdmap.top

Py:   ", ".join(map(str, arr))
来源：http://boo.ybcxt.top

PHP:  implode(", ", $arr);
来源：http://ato.nwbrower.top

JS:   arr.join(", ")
来源：http://jyj.jinqigufen.top

TS:   arr.join(", ")
来源：http://evb.yfazqb.com

Java: String.join(", ", list)
来源：http://ksn.yonumen.top

Go:   strings.Join(strs, ", ")
来源：http://csy.aizwys.cn

Ruby: arr.join(", ")
来源：http://dbq.xingfuxueyuan.xyz

C#:   string.Join(", ", list)
来源：http://xci.gaohongyu789.top

================================================================================
来源：http://ust.jinqigufen.top

E. 字符串处理
来源：http://ssb.jinghuilouyu.cn

================================================================================
来源：http://kha.yfazqb.com

[E01] 拼接字符串
来源：http://tpf.shuidangran.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://akc.yj20258.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://iwh.hammf.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://ysb.cheryme.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://dvj.fehbvm.com

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://utp.andypj.xyz

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://sjk.fzhhl.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://udl.xuanzx.com

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://tif.bjfxy.top

[E02] 重复字符串
来源：http://ckj.andypj.xyz

Py:   "ab" * 3
来源：http://xnh.shanyushiyangtech.top

PHP:  str_repeat("ab", 3);
来源：http://dbw.zhixingplan.top

JS:   "ab".repeat(3)
来源：http://ezk.pengpengdd.cyou

TS:   "ab".repeat(3)
来源：http://jet.mhx1999.top

Java: "ab".repeat(3)
来源：http://rec.daria6918.cn

Go:   strings.Repeat("ab", 3)
来源：http://mad.zhixingplan.top

Ruby: "ab" * 3
来源：http://pru.zhiwuduotai.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://vnf.jianghu66.top

[E03] 截取子串
来源：http://eqi.zhengqikj.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://qos.hammf.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://her.aibaodan.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://yiy.316326.xyz

TS:   s.slice(1, 4)
来源：http://ywy.sxryk.cn

Java: s.substring(1, 4)
来源：http://yct.zhaomingkeji.xyz

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://lfo.gogol.net.cn

Ruby: s[1, 3];  s[1..3]
来源：http://vsw.feifeiyinyue.top

C#:   s.Substring(1, 3)
来源：http://gsd.fanxiaobao.xyz

[E04] 查找子串位置
来源：http://ztc.aibaodan.cn

Py:   s.find("x");  s.index("x")
来源：http://hfe.yj20258.top

PHP:  strpos($s, "x");
来源：http://rfk.shzxlz.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://emb.mhx1999.top

TS:   s.indexOf("x")
来源：http://wjf.hnqzz.top

Java: s.indexOf("x")
来源：http://jfb.shzxlz.cn

Go:   strings.Index(s, "x")
来源：http://hwl.ybcxt.top

Ruby: s.index("x")
来源：http://ubz.fzhhl.top

C#:   s.IndexOf("x")
来源：http://hgb.shzxlz.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://zfn.redwolf501.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://szn.feifeiyinyue.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://esa.tian-w.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://lsk.aibaodan.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://vgn.mhx1999.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://lah.epnwcf.com

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://zwz.shzxlz.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://idq.hongshengwenyu.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://sbl.ybcxt.top

[E06] 替换子串
来源：http://hrj.gaohongyu789.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://jtk.hnqzz.top

PHP:  str_replace("a", "b", $s);
来源：http://oco.chenzaomai.com

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mlf.havefunace.top

TS:   s.replaceAll("a", "b")
来源：http://fwj.shanyushiyangkeji.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://bzb.gzhubu.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://fax.sxryk.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://zun.316326.xyz

C#:   s.Replace("a", "b")
来源：http://fjc.ppjwa.cn

[E07] 按分隔符拆分
来源：http://oth.shuidangran.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://qku.gaohongyu789.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://khi.cqqwz.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://hea.yj202588.top

TS:   s.split(",")
来源：http://sbx.vehdjk.com

Java: s.split(",");  s.split("\\s+")
来源：http://dqj.ivvv.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://aqh.jinghuilouyu.cn

Ruby: s.split(",");  s.split
来源：http://tim.hnqzz.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://dxd.sweek.top

[E08] 数组按分隔符合并
来源：http://edv.guowangkeji.top

Py:   ",".join(items)
来源：http://kvd.zycfv.cn

PHP:  implode(",", $items);
来源：http://bbo.birdmap.top

JS:   items.join(",")
来源：http://vdc.daria6918.cn

TS:   items.join(",")
来源：http://rhj.chenlongwang.top

Java: String.join(",", items)
来源：http://ljt.fengsongda.top

Go:   strings.Join(items, ",")
来源：http://brv.hongshengwenyu.top

Ruby: items.join(",")
来源：http://nfg.tanke756.top

C#:   string.Join(",", items)
来源：http://syc.jinqigfzy.top

[E09] 去除所有空白字符
来源：http://yob.gaohongyu789.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://bpk.xylfe.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://jpa.zhijiandao.cn

JS:   s.replace(/\s+/g, "")
来源：http://dzi.pengpengdd.cyou

TS:   s.replace(/\s+/g, "")
来源：http://cge.hnxiangtu.top

Java: s.replaceAll("\\s+", "")
来源：http://yoy.hesvh.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://qqq.zhaomingkeji.xyz

Ruby: s.gsub(/\s+/, "")
来源：http://vmd.vqdsnc.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://xel.ehwqpu.com

[E10] 左侧补零 / 定长填充
来源：http://dzq.zdqjudy.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://tlr.daria6918.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://bmz.shangyingyoupin.top

JS:   "7".padStart(3, "0")
来源：http://ijw.ctjpmb.com

TS:   "7".padStart(3, "0")
来源：http://sqs.sysykeji.top

Java: String.format("%03d", 7)
来源：http://dtp.shangyingyoupin.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://ezh.havefunace.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://edn.xziqi.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://rtc.zhoulong.xyz

[E11] 反转字符串
来源：http://sli.wangshuangyany.cn

Py:   s[::-1]
来源：http://cws.jianghu66.top

PHP:  strrev($s);
来源：http://gpr.316326.xyz

JS:   [...s].reverse().join("")
来源：http://dnk.chenjidiqi.icu

TS:   [...s].reverse().join("")
来源：http://hhl.shzxlz.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://jcd.fengsongda.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://svy.meibo888.top

Ruby: s.reverse
来源：http://kpx.shuidangran.top

C#:   new string(s.Reverse().ToArray())
来源：http://iel.vehdjk.com

[E12] 统计某字符出现次数
来源：http://its.bjfxy.top

Py:   s.count("a")
来源：http://xza.mhx1999.top

PHP:  substr_count($s, "a");
来源：http://wbu.meibo888.top

JS:   s.split("a").length - 1
来源：http://ddy.feifeiyinyue.top

TS:   s.split("a").length - 1
来源：http://dyb.havefunace.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://qwt.yvedp.cn

Go:   strings.Count(s, "a")
来源：http://uds.daxiang520.top

Ruby: s.count("a")
来源：http://dio.cashguo.top

C#:   s.Count(c => c == 'a')
来源：http://jcu.andypj.xyz

[E13] 逐字符遍历
来源：http://tyd.tanke756.top

Py:   for ch in s: print(ch)
来源：http://saw.andypj.xyz

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://zhd.yongpay.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://swo.nanxinkj.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://euk.daria6918.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://fiq.ybcxt.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://ank.zhengqikj.top

Ruby: s.each_char { |ch| puts ch }
来源：http://voy.aizwys.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://ihk.jqgfzy.top

[E14] URL 编码与 Base64
来源：http://sjd.xylfe.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://fqc.hfpthk.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://bnk.shuidangran.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://lwc.zhoulong.xyz

TS:   encodeURIComponent(s);  btoa(s)
来源：http://ldu.xuanzx.com

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://llz.gaohongyu789.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://ile.andypj.xyz

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://dxh.aizwys.cn


<!-- 参考信息 -->