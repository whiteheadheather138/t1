代发 wailian999

PHP:  sort($arr);
来源：http://ajt.yanxiufei.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://uwj.jinyuanbaomall.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://gok.cucudq.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://jty.snrcjt.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://lko.guowangkeji.top

Ruby: arr.sort
来源：http://tbe.shanyushiyangtech.top

C#:   list.Sort();
来源：http://shd.sweek.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://zdo.yj20258888.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://gbj.gotoacloud.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://iul.yueranfly.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://xqp.jinqigfzy.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://spb.ppjwa.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://rtu.fktsv.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://bve.gaohongyu789.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://xga.andypj.xyz

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://omo.hywenlv.cn

[D11] 反转数组
来源：http://wov.ehwqpu.com

Py:   arr[::-1];  arr.reverse()
来源：http://ptx.yanxiufei.cn

PHP:  array_reverse($arr);
来源：http://mqu.hammf.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://mpt.sjlbkw.cn

TS:   [...arr].reverse();
来源：http://jit.daria6918.cn

Java: Collections.reverse(list);
来源：http://fhc.xuanzx.com

Go:   slices.Reverse(arr)
来源：http://lbl.vqdsnc.cn

Ruby: arr.reverse
来源：http://pkj.fengsongda.top

C#:   list.Reverse();
来源：http://alm.jlsjyb.cn

[D12] 查找元素下标
来源：http://gjp.c1oappe.top

Py:   arr.index(x);  x in arr
来源：http://hoz.guowangkeji.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://ijx.yangfankeji.com

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ejb.daria6918.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://olp.gogol.net.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://yru.ybcxt.top

Go:   slices.Index(arr, x)
来源：http://rne.hnqzz.top

Ruby: arr.index(x)
来源：http://kli.ybcxt.top

C#:   list.IndexOf(x);
来源：http://vus.aizwys.cn

[D13] 过滤（保留满足条件的）
来源：http://qag.jinyuanbaomall.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://bjj.vqdsnc.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://olb.zhijiandao.cn

JS:   arr.filter(x => x > 3)
来源：http://qnh.yongpay.top

TS:   arr.filter(x => x > 3)
来源：http://otz.hammf.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://mqu.gogol.net.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://bla.yuxming.cn

Ruby: arr.select { |x| x > 3 }
来源：http://uyw.xuetiantiany.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://bfz.chenlongwang.top

[D14] 映射转换（每个元素变形）
来源：http://beb.gotoacloud.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://lyo.pengpengdd.cyou

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://iwd.shangyingyoupin.top

JS:   arr.map(x => x * 2)
来源：http://xxm.uphjek.com

TS:   arr.map(x => x * 2)
来源：http://inj.uphjek.com

Java: list.stream().map(x -> x * 2).toList()
来源：http://toe.dianchejie.cn

Go:   // 手写循环
来源：http://uab.gaohongyu789.top

Ruby: arr.map { |x| x * 2 }
来源：http://gav.chenlongwang.top

C#:   list.Select(x => x * 2).ToList()
来源：http://oql.shanyushiyangkeji.top

[D15] 去重
来源：http://mdh.mhx1999.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://zcq.shuidangran.top

PHP:  array_unique($arr);
来源：http://yex.jqgfzy.top

JS:   [...new Set(arr)]
来源：http://zdl.yanxiufei.cn

TS:   [...new Set(arr)]
来源：http://jgt.hammf.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://wyc.snrcjt.cn

Go:   // 用 map[T]struct{} 手写
来源：http://our.ctjpmb.com

Ruby: arr.uniq
来源：http://jmv.kuanghao11.cn

C#:   list.Distinct().ToList()
来源：http://uur.sweek.top

[D16] 求和与平均值
来源：http://edp.shzxlz.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hxf.tian-w.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://eiw.vehdjk.com

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://cre.haohaochexian.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://lec.xziqi.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://zge.pengpengdd.cyou

Go:   // 手写循环累加
来源：http://lgk.shanyushiyangkeji.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hrf.fehbvm.com

C#:   list.Sum();  list.Average()
来源：http://tvz.bjfxy.top

[D17] 最大值与最小值
来源：http://alq.yanxiufei.cn

Py:   max(arr);  min(arr)
来源：http://tlh.meibo888.top

PHP:  max($arr);  min($arr);
来源：http://jkw.quarkkingdee.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://uwy.kuanghao11.cn

TS:   Math.max(...arr);
来源：http://tvj.feifeiyinyue.top

Java: Collections.max(list);  Collections.min(list);
来源：http://fcj.svipenyu.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://tvx.cdnleiting.top

Ruby: arr.max;  arr.min
来源：http://ksb.xinyue.icu

C#:   list.Max();  list.Min()
来源：http://ywy.aizwys.cn

[D18] 扁平化嵌套数组
来源：http://jiz.ivvv.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://ojw.jinqigfzy.top

PHP:  array_merge(...$nested);
来源：http://idb.ehwqpu.com

JS:   nested.flat();  nested.flat(Infinity)
来源：http://fnc.xuetiantiany.cn

TS:   nested.flat();
来源：http://art.feifeiyinyue.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://tbk.bjfxy.top

Go:   // 手写双层循环
来源：http://qik.yuxming.cn

Ruby: nested.flatten
来源：http://eqz.yj20258.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://bdt.fehbvm.com

[D19] 按字段分组
来源：http://qcw.andypj.xyz

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://zoa.vqdsnc.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://fko.kuanghao11.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://zbw.xziqi.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://nft.gogol.net.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://ppo.nwbrower.top

Go:   // 手写 map[string][]T
来源：http://arv.andypj.xyz

Ruby: arr.group_by { |x| x[:type] }
来源：http://smj.fktsv.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://ckn.ybcxt.top

[D20] 统计每个元素出现次数
来源：http://ncj.jinyuanbaomall.cn

Py:   Counter(arr)
来源：http://bav.bbcook.cn

PHP:  array_count_values($arr);
来源：http://afb.jinqigfzy.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://kfi.hesvh.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://tst.zhiwuduotai.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hxb.daxiang520.top

Go:   // 手写 map[T]int
来源：http://ajd.chenzaomai.com

Ruby: arr.tally
来源：http://qze.hnqzz.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://pfy.52xcode.cn

[D21] 判断是否包含某元素
来源：http://zgd.vehdjk.com

Py:   x in arr
来源：http://ymc.ybcxt.top

PHP:  in_array($x, $arr, true);
来源：http://pvz.cucudq.cn

JS:   arr.includes(x)
来源：http://duq.sysykeji.top

TS:   arr.includes(x)
来源：http://gvq.zhoulong.xyz

Java: list.contains(x)
来源：http://gnd.yangfankeji.com

Go:   slices.Contains(arr, x)
来源：http://nrf.yueranfly.top

Ruby: arr.include?(x)
来源：http://ysy.shangyingyoupin.top

C#:   list.Contains(x)
来源：http://uaw.gaohongyu789.top

[D22] 复制数组（避免共享引用）
来源：http://wsa.9152youxi.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hbd.wangdashe.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://qoy.hcnkem.com

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://suj.bjfxy.top

TS:   [...arr];
来源：http://kty.hnxiangtu.top

Java: new ArrayList<>(list);
来源：http://oat.gzhubu.top

Go:   copied := append([]int(nil), arr...)
来源：http://xto.quarkkingdee.top

Ruby: arr.dup;  arr.clone
来源：http://qhc.havefunace.top

C#:   new List<int>(list);
来源：http://cdm.kuanghao11.cn

[D23] reduce 累积计算
来源：http://isi.xingfuxueyuan.xyz

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://vsu.yuxming.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://fof.bbcook.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ajp.yangfankeji.com

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://eqv.tarul.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://uwu.jqgfzy.top

Go:   // 手写循环
来源：http://kvv.ydjk.org.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://rvw.hesvh.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://ium.feifeiyinyue.top

[D24] 字典 / Map 基本操作
来源：http://nqm.smart0.xyz

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://gac.cdnleiting.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://nbn.sjlbkw.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://xgb.zycfv.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://zfc.yueranfly.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://cxz.xylfe.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://atw.hesvh.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://mga.yfazqb.com

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hji.ctjpmb.com

[D25] Set 集合去重与交并差
来源：http://nav.dashuyun.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://sdv.zycfv.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://pyb.wangdashe.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://gds.yfazqb.com

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://fqg.hesvh.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://rya.andypj.xyz

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://oxi.redwolf501.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hbq.ydjk.org.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://bvp.zhaomingkeji.xyz

[D26] 数组转字符串
来源：http://sms.yangfankeji.com

Py:   ", ".join(map(str, arr))
来源：http://rba.shzxlz.cn

PHP:  implode(", ", $arr);
来源：http://ksx.tanke756.top

JS:   arr.join(", ")
来源：http://sgf.ydzc1.top

TS:   arr.join(", ")
来源：http://uus.vqdsnc.cn

Java: String.join(", ", list)
来源：http://obv.jqgufenzy.top

Go:   strings.Join(strs, ", ")
来源：http://goc.zhaomingkeji.xyz

Ruby: arr.join(", ")
来源：http://mwl.daria6918.cn

C#:   string.Join(", ", list)
来源：http://jkb.sxryk.cn

================================================================================
来源：http://gbw.sjlbkw.cn

E. 字符串处理
来源：http://ria.fehbvm.com

================================================================================
来源：http://kqg.haohaochexian.top

[E01] 拼接字符串
来源：http://okr.iojbl.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://stg.redwolf501.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://qyy.cashguo.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://ayt.c1oappe.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://biu.quarkkingdee.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://lcf.zdbjq.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://ezk.zhongyouzk.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://zfp.mhx1999.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://ypu.guannengcc.top

[E02] 重复字符串
来源：http://pbn.316326.xyz

Py:   "ab" * 3
来源：http://yvx.jinqigfzy.top

PHP:  str_repeat("ab", 3);
来源：http://mho.yj202588.top

JS:   "ab".repeat(3)
来源：http://rvq.uphjek.com

TS:   "ab".repeat(3)
来源：http://bvr.gotoacloud.top

Java: "ab".repeat(3)
来源：http://gbp.52xcode.cn

Go:   strings.Repeat("ab", 3)
来源：http://plb.zhiwuduotai.top

Ruby: "ab" * 3
来源：http://kyy.cdnleiting.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://irh.zdqjudy.top

[E03] 截取子串
来源：http://kgi.shanyushiyangtech.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://mst.hcnkem.com

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://upz.smart0.xyz

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://yha.hammf.cn

TS:   s.slice(1, 4)
来源：http://hcn.ehwqpu.com

Java: s.substring(1, 4)
来源：http://cbi.zycfv.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://icd.hongshengwenyu.top

Ruby: s[1, 3];  s[1..3]
来源：http://gnf.ydjk.org.cn

C#:   s.Substring(1, 3)
来源：http://qro.jqgfzy.top

[E04] 查找子串位置
来源：http://afq.jinghuilouyu.cn

Py:   s.find("x");  s.index("x")
来源：http://eff.yanxiufei.cn

PHP:  strpos($s, "x");
来源：http://oat.meibo888.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://vyv.vqdsnc.cn

TS:   s.indexOf("x")
来源：http://spp.sysykeji.top

Java: s.indexOf("x")
来源：http://dsg.cheryme.top

Go:   strings.Index(s, "x")
来源：http://tlj.hesvh.cn

Ruby: s.index("x")
来源：http://izd.gogol.net.cn

C#:   s.IndexOf("x")
来源：http://zqt.ppjwa.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://hkv.zhengqikj.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://bfy.ivvv.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hrz.jiagoushi.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://gqw.shangyingyoupin.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://lnk.tian-w.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://set.xingfuxueyuan.xyz

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://dlj.daxiang520.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://opx.zhaomingkeji.xyz

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://gmo.jianghu66.top

[E06] 替换子串
来源：http://prs.tian-w.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://tup.xziqi.cn

PHP:  str_replace("a", "b", $s);
来源：http://rdm.snrcjt.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://dei.nanxinkj.top

TS:   s.replaceAll("a", "b")
来源：http://son.zhengqikj.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://syi.aizwys.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://kaa.bbcook.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://ulq.hnxiangtu.top

C#:   s.Replace("a", "b")
来源：http://skd.yfazqb.com

[E07] 按分隔符拆分
来源：http://jrm.jyoumei.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://pzl.fktsv.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://bzl.shzxlz.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://cug.zhiwuduotai.top

TS:   s.split(",")
来源：http://jdv.hfpthk.cn

Java: s.split(",");  s.split("\\s+")
来源：http://vff.aizwys.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://wxn.yuanzhike.top

Ruby: s.split(",");  s.split
来源：http://uak.guannengcc.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://ink.jianghu66.top

[E08] 数组按分隔符合并
来源：http://ise.guannengcc.top

Py:   ",".join(items)
来源：http://qfu.ctjpmb.com

PHP:  implode(",", $items);
来源：http://vwm.haohaochexian.top

JS:   items.join(",")
来源：http://qag.vqdsnc.cn

TS:   items.join(",")
来源：http://fyl.hnxiangtu.top

Java: String.join(",", items)
来源：http://tin.tianlin.xyz

Go:   strings.Join(items, ",")
来源：http://llc.bjfxy.top

Ruby: items.join(",")
来源：http://icr.iojbl.cn

C#:   string.Join(",", items)
来源：http://wrb.zhijiandao.cn

[E09] 去除所有空白字符
来源：http://ehd.jinghuilouyu.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://czo.cheryme.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://rsu.sjlbkw.cn

JS:   s.replace(/\s+/g, "")
来源：http://tnc.xylfe.cn

TS:   s.replace(/\s+/g, "")
来源：http://hzs.yj202588.top

Java: s.replaceAll("\\s+", "")
来源：http://akn.xylfe.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://gkz.iojbl.cn

Ruby: s.gsub(/\s+/, "")
来源：http://uxf.yangfankeji.com

C#:   Regex.Replace(s, @"\s+", "")
来源：http://ihn.tarul.cn

[E10] 左侧补零 / 定长填充
来源：http://gld.jqgufenzy.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://wtk.zhengqikj.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://ihv.zhongyouzk.top

JS:   "7".padStart(3, "0")
来源：http://fnj.aizwys.cn

TS:   "7".padStart(3, "0")
来源：http://ybi.fanxiaobao.xyz

Java: String.format("%03d", 7)
来源：http://dne.zhengqikj.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://zyi.guowangkeji.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://orv.yj20258888.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://tae.dianchejie.cn

[E11] 反转字符串
来源：http://mck.jianghu66.top

Py:   s[::-1]
来源：http://ynl.yuanzhike.top

PHP:  strrev($s);
来源：http://ogo.hysaishi.cn

JS:   [...s].reverse().join("")
来源：http://nrc.shzxlz.cn

TS:   [...s].reverse().join("")
来源：http://ysu.yangfankeji.com

Java: new StringBuilder(s).reverse().toString()
来源：http://jgo.sjlbkw.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://ukh.guowangkeji.top

Ruby: s.reverse
来源：http://hzq.jinqigufen.top

C#:   new string(s.Reverse().ToArray())
来源：http://eys.wangdashe.top

[E12] 统计某字符出现次数
来源：http://moa.yuanzhike.top

Py:   s.count("a")
来源：http://osu.yvedp.cn

PHP:  substr_count($s, "a");
来源：http://drf.yangfankeji.com

JS:   s.split("a").length - 1
来源：http://fwi.zdbjq.cn

TS:   s.split("a").length - 1
来源：http://pee.haohaochexian.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://lmx.nanxuanxn.top

Go:   strings.Count(s, "a")
来源：http://sae.jinqigfzy.top

Ruby: s.count("a")
来源：http://yhv.ybcxt.top

C#:   s.Count(c => c == 'a')
来源：http://byv.ybcxt.top

[E13] 逐字符遍历
来源：http://crg.gaohongyu789.top

Py:   for ch in s: print(ch)
来源：http://lhc.hongshengwenyu.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://ced.pengpengdd.cyou

JS:   for (const ch of s) { console.log(ch); }
来源：http://sxq.316326.xyz

TS:   for (const ch of s) { console.log(ch); }
来源：http://mai.hywenlv.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://ujr.zdbjq.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://rom.kuanghao11.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://ibq.hnqzz.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://uwt.dianchejie.cn

[E14] URL 编码与 Base64
来源：http://jpr.cheryme.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://soh.vqdsnc.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://bgq.svipenyu.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://uuk.zhongyouzk.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://tsz.hnxiangtu.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://fnq.shanyushiyangtech.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://ykr.meibo888.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://llj.cucudq.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://gej.haohaochexian.top

[E15] HTML 转义 / 反转义
来源：http://pbg.sysykeji.top

Py:   html.escape(s);  html.unescape(s)
来源：http://etz.nwbrower.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://lan.yangfankeji.com

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://qwo.fzhhl.top

TS:   // 同上，务必做 XSS 过滤
来源：http://owq.zhiwuduotai.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://tws.yuanzhike.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://vrz.dianchejie.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://enn.ctjpmb.com

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://lqx.tian-w.cn

[E16] 数字千分位
来源：http://zse.aibaodan.cn

Py:   f"{1234567:,}"
来源：http://mbg.bbcook.cn


<!-- 参考信息 -->