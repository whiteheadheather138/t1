代发 wailian999

C#:   list.GetRange(1, 3);
来源：http://brj.mhx1999.top

[D08] 合并两个数组
来源：http://bdt.bbcook.cn

Py:   a + b;  a.extend(b)
来源：http://ctp.0kj1m.cn

PHP:  array_merge($a, $b);
来源：http://guj.yangfankeji.com

JS:   [...a, ...b];  a.concat(b);
来源：http://uno.quarkkingdee.top

TS:   [...a, ...b];
来源：http://esv.ehwqpu.com

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://zok.chenzaomai.com

Go:   append(a, b...)
来源：http://bmy.zdqjudy.top

Ruby: a + b;  a.concat(b)
来源：http://nja.sufxvd.cn

C#:   a.Concat(b).ToList()
来源：http://riv.yonumen.top

[D09] 排序（升序）
来源：http://rwq.shanyushiyangkeji.top

Py:   sorted(arr);  arr.sort()
来源：http://yfv.bjfxy.top

PHP:  sort($arr);
来源：http://iap.52xcode.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://sly.jqgufenzy.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://yqm.jqgufenzy.top

Java: Collections.sort(list);  list.sort(null);
来源：http://zwr.dashuyun.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://mcl.jqgfzy.top

Ruby: arr.sort
来源：http://ynj.hywenlv.cn

C#:   list.Sort();
来源：http://awz.smart0.xyz

[D10] 自定义排序（按字段 / 多条件）
来源：http://fwe.dianchejie.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://bvh.zhixingplan.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://eqq.quarkkingdee.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://kok.fehbvm.com

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://twq.zhixingplan.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://ejz.andypj.xyz

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://gap.ywan-chungtsiang.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://cdy.shzxlz.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hpw.mhx1999.top

[D11] 反转数组
来源：http://pjd.yongpay.top

Py:   arr[::-1];  arr.reverse()
来源：http://svg.9152youxi.cn

PHP:  array_reverse($arr);
来源：http://fwa.aizwys.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://enw.0kj1m.cn

TS:   [...arr].reverse();
来源：http://uss.epnwcf.com

Java: Collections.reverse(list);
来源：http://mde.yongpay.top

Go:   slices.Reverse(arr)
来源：http://cwe.chenzaomai.com

Ruby: arr.reverse
来源：http://qvu.jianghu66.top

C#:   list.Reverse();
来源：http://esd.snrcjt.cn

[D12] 查找元素下标
来源：http://oqs.nanxinkj.top

Py:   arr.index(x);  x in arr
来源：http://bmv.jinyuanbaomall.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://wjy.xuetiantiany.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ufk.daria6918.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ump.cucudq.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://cih.chenjidiqi.icu

Go:   slices.Index(arr, x)
来源：http://hud.cucudq.cn

Ruby: arr.index(x)
来源：http://duj.svipenyu.cn

C#:   list.IndexOf(x);
来源：http://big.kuanghao11.cn

[D13] 过滤（保留满足条件的）
来源：http://qfy.cqqwz.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://dem.aibaodan.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://xbp.shanyushiyangtech.top

JS:   arr.filter(x => x > 3)
来源：http://ywg.wangdashe.top

TS:   arr.filter(x => x > 3)
来源：http://ccf.316326.xyz

Java: list.stream().filter(x -> x > 3).toList()
来源：http://rry.iojbl.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://crq.chenzaomai.com

Ruby: arr.select { |x| x > 3 }
来源：http://urh.nanxinkj.top

C#:   list.Where(x => x > 3).ToList()
来源：http://dvc.tanke756.top

[D14] 映射转换（每个元素变形）
来源：http://wjw.dianchejie.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://kkr.tianlin.xyz

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://wai.zdqjudy.top

JS:   arr.map(x => x * 2)
来源：http://ynn.ydzc1.top

TS:   arr.map(x => x * 2)
来源：http://gjc.hcnkem.com

Java: list.stream().map(x -> x * 2).toList()
来源：http://ysp.sxryk.cn

Go:   // 手写循环
来源：http://djk.fanxiaobao.xyz

Ruby: arr.map { |x| x * 2 }
来源：http://qfe.sxryk.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://xpi.wangdashe.top

[D15] 去重
来源：http://lti.cucudq.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://bka.cqqwz.cn

PHP:  array_unique($arr);
来源：http://vas.shanyushiyangtech.top

JS:   [...new Set(arr)]
来源：http://ocq.hesvh.cn

TS:   [...new Set(arr)]
来源：http://zal.316326.xyz

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://wwl.hnqzz.top

Go:   // 用 map[T]struct{} 手写
来源：http://avn.hfpthk.cn

Ruby: arr.uniq
来源：http://pof.shzxlz.cn

C#:   list.Distinct().ToList()
来源：http://yak.haohaochexian.top

[D16] 求和与平均值
来源：http://rru.pycfn.com

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hkv.sweek.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://zup.yongpay.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://pkd.ydzc1.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://uaa.jinghuilouyu.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://qei.jinqigfzy.top

Go:   // 手写循环累加
来源：http://sox.jinqigufen.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://ram.tian-w.cn

C#:   list.Sum();  list.Average()
来源：http://cmz.cashguo.top

[D17] 最大值与最小值
来源：http://zdo.fzhhl.top

Py:   max(arr);  min(arr)
来源：http://ejp.dianchejie.cn

PHP:  max($arr);  min($arr);
来源：http://znm.daxiang520.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://cxy.yuxming.cn

TS:   Math.max(...arr);
来源：http://pic.ydzc1.top

Java: Collections.max(list);  Collections.min(list);
来源：http://gro.hongshengwenyu.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://nyb.birdmap.top

Ruby: arr.max;  arr.min
来源：http://fat.yonumen.top

C#:   list.Max();  list.Min()
来源：http://ydm.bbcook.cn

[D18] 扁平化嵌套数组
来源：http://vjz.uphjek.com

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://fid.aizwys.cn

PHP:  array_merge(...$nested);
来源：http://tyo.gaohongyu789.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://iwc.aibaodan.cn

TS:   nested.flat();
来源：http://kzb.dashuyun.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://xqh.xingfuxueyuan.xyz

Go:   // 手写双层循环
来源：http://dbj.zhixingplan.top

Ruby: nested.flatten
来源：http://kqo.snrcjt.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://mol.haohaochexian.top

[D19] 按字段分组
来源：http://dgp.zhiwuduotai.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://wec.yvedp.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://bwc.shzxlz.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://cej.vehdjk.com

TS:   Object.groupBy(arr, x => x.type)
来源：http://xgj.cqqwz.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://jyx.xziqi.cn

Go:   // 手写 map[string][]T
来源：http://sev.vehdjk.com

Ruby: arr.group_by { |x| x[:type] }
来源：http://dsf.pycfn.com

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://zqm.kuanghao11.cn

[D20] 统计每个元素出现次数
来源：http://lkg.chenlongwang.top

Py:   Counter(arr)
来源：http://rix.hesvh.cn

PHP:  array_count_values($arr);
来源：http://xjq.cucudq.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://pou.jiagoushi.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://xtm.zhixingplan.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://glm.cucudq.cn

Go:   // 手写 map[T]int
来源：http://odi.aibaodan.cn

Ruby: arr.tally
来源：http://yoy.xziqi.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://qii.tanke756.top

[D21] 判断是否包含某元素
来源：http://nnk.jlsjyb.cn

Py:   x in arr
来源：http://doj.zycfv.cn

PHP:  in_array($x, $arr, true);
来源：http://epc.yuxming.cn

JS:   arr.includes(x)
来源：http://xtz.fktsv.cn

TS:   arr.includes(x)
来源：http://avu.gaohongyu789.top

Java: list.contains(x)
来源：http://ovc.yj202588.top

Go:   slices.Contains(arr, x)
来源：http://snf.zhongyouzk.top

Ruby: arr.include?(x)
来源：http://acd.nwbrower.top

C#:   list.Contains(x)
来源：http://ygp.hesvh.cn

[D22] 复制数组（避免共享引用）
来源：http://yzw.hnxiangtu.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://qcs.jqgfzy.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://vgr.tanke756.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://rva.yj202588.top

TS:   [...arr];
来源：http://phi.zhiwuduotai.top

Java: new ArrayList<>(list);
来源：http://kxm.hcnkem.com

Go:   copied := append([]int(nil), arr...)
来源：http://msq.52xcode.cn

Ruby: arr.dup;  arr.clone
来源：http://seq.guowangkeji.top

C#:   new List<int>(list);
来源：http://ibr.yuanzhike.top

[D23] reduce 累积计算
来源：http://bis.yueranfly.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://ywf.gzhubu.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://rcx.shanyushiyangtech.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://vqs.yvedp.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ksq.yfazqb.com

Java: list.stream().reduce(0, Integer::sum)
来源：http://ebs.shzxlz.cn

Go:   // 手写循环
来源：http://gnf.cdnleiting.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://ftb.yj20258888.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://cor.jinghuilouyu.cn

[D24] 字典 / Map 基本操作
来源：http://csd.aizwys.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://dzc.yuanzhike.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://ivb.uphjek.com

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://bac.xziqi.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://czd.ivvv.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://moz.tian-w.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://ujs.nwbrower.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://znl.yanxiufei.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://wdr.yj20258.top

[D25] Set 集合去重与交并差
来源：http://fkg.dianchejie.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://jhv.wangdashe.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://mfq.hesvh.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://iwd.havefunace.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://oyu.gaohongyu789.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://fwa.jqgufenzy.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://zac.feifeiyinyue.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://nkw.xziqi.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://qzs.sufxvd.cn

[D26] 数组转字符串
来源：http://qam.yj202588.top

Py:   ", ".join(map(str, arr))
来源：http://fvb.wangshuangyany.cn

PHP:  implode(", ", $arr);
来源：http://vhu.jiagoushi.top

JS:   arr.join(", ")
来源：http://kka.ywan-chungtsiang.top

TS:   arr.join(", ")
来源：http://clo.ybcxt.top

Java: String.join(", ", list)
来源：http://obp.ydzc1.top

Go:   strings.Join(strs, ", ")
来源：http://mqw.ybcxt.top

Ruby: arr.join(", ")
来源：http://pha.sweek.top

C#:   string.Join(", ", list)
来源：http://rcu.yj20258888.top

================================================================================
来源：http://fxr.shuidangran.top

E. 字符串处理
来源：http://dtw.wangdashe.top

================================================================================
来源：http://gbt.shanyushiyangkeji.top

[E01] 拼接字符串
来源：http://gpj.yuxming.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://cfn.sxryk.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://whq.jinqigufen.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://egq.gzhubu.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://gdp.xuetiantiany.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://mte.zhiwuduotai.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://ghw.jinghuilouyu.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://ctr.cheryme.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://cnb.shangyingyoupin.top

[E02] 重复字符串
来源：http://apd.zdbjq.cn

Py:   "ab" * 3
来源：http://wbv.zhaomingkeji.xyz

PHP:  str_repeat("ab", 3);
来源：http://pbl.nanxuanxn.top

JS:   "ab".repeat(3)
来源：http://cys.fzhhl.top

TS:   "ab".repeat(3)
来源：http://tds.sweek.top

Java: "ab".repeat(3)
来源：http://lah.tanke756.top

Go:   strings.Repeat("ab", 3)
来源：http://ovo.hesvh.cn

Ruby: "ab" * 3
来源：http://qmf.xingfuxueyuan.xyz

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://zay.9152youxi.cn

[E03] 截取子串
来源：http://rwo.shzxlz.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://lpq.jinqigfzy.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://wsp.hywenlv.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://ypk.jinyuanbaomall.cn

TS:   s.slice(1, 4)
来源：http://brg.feifeiyinyue.top

Java: s.substring(1, 4)
来源：http://boz.xylfe.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://ctz.redwolf501.top

Ruby: s[1, 3];  s[1..3]
来源：http://qij.yangfankeji.com

C#:   s.Substring(1, 3)
来源：http://exj.nanxuanxn.top

[E04] 查找子串位置
来源：http://dkb.hcnkem.com

Py:   s.find("x");  s.index("x")
来源：http://zth.fzhhl.top

PHP:  strpos($s, "x");
来源：http://urj.jqgufenzy.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://sia.ydjk.org.cn

TS:   s.indexOf("x")
来源：http://xki.jqgufenzy.top

Java: s.indexOf("x")
来源：http://jqg.cucudq.cn

Go:   strings.Index(s, "x")
来源：http://wyt.fanxiaobao.xyz

Ruby: s.index("x")
来源：http://ocz.zdbjq.cn

C#:   s.IndexOf("x")
来源：http://ivt.jinqigufen.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://aaz.xziqi.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://yyr.bbcook.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://cyr.kuanghao11.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://jki.fktsv.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://jcw.9152youxi.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hba.aizwys.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://ajh.jiagoushi.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://wgr.yueranfly.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://uvn.cucudq.cn

[E06] 替换子串
来源：http://zes.yj20258.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://vti.jyoumei.cn

PHP:  str_replace("a", "b", $s);
来源：http://yfo.yj20258888.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://vug.cqqwz.cn

TS:   s.replaceAll("a", "b")
来源：http://wiv.nanxuanxn.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://szk.gogol.net.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://jop.shuidangran.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://xef.ybcxt.top

C#:   s.Replace("a", "b")
来源：http://hyr.sysykeji.top

[E07] 按分隔符拆分
来源：http://xmh.zhijiandao.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://mni.chenzaomai.com

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://lsm.hcnkem.com

JS:   s.split(",");  s.split(/\s+/)
来源：http://icc.jqgufenzy.top

TS:   s.split(",")
来源：http://dnf.hammf.cn

Java: s.split(",");  s.split("\\s+")
来源：http://lam.yuanzhike.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://ijd.gzhubu.top

Ruby: s.split(",");  s.split
来源：http://yyb.redwolf501.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://knl.guowangkeji.top

[E08] 数组按分隔符合并
来源：http://yoh.xziqi.cn

Py:   ",".join(items)
来源：http://yiv.meibo888.top

PHP:  implode(",", $items);
来源：http://lpt.fanxiaobao.xyz

JS:   items.join(",")
来源：http://vqt.jinqigfzy.top

TS:   items.join(",")
来源：http://gds.havefunace.top

Java: String.join(",", items)
来源：http://aiv.chenzaomai.com

Go:   strings.Join(items, ",")
来源：http://ioj.chenzaomai.com

Ruby: items.join(",")
来源：http://ovy.52xcode.cn

C#:   string.Join(",", items)
来源：http://zav.wangdashe.top

[E09] 去除所有空白字符
来源：http://dll.jiagoushi.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://wlr.jqgufenzy.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://zny.zhiwuduotai.top

JS:   s.replace(/\s+/g, "")
来源：http://llj.jinqigufen.top

TS:   s.replace(/\s+/g, "")
来源：http://fkj.birdmap.top

Java: s.replaceAll("\\s+", "")
来源：http://ksh.uphjek.com

Go:   strings.Join(strings.Fields(s), "")
来源：http://kmf.jlsjyb.cn

Ruby: s.gsub(/\s+/, "")
来源：http://oft.cdnleiting.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://ufz.yanxiufei.cn

[E10] 左侧补零 / 定长填充
来源：http://qdm.smart0.xyz

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://eml.yj20258888.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hbn.fengsongda.top

JS:   "7".padStart(3, "0")
来源：http://yku.hfpthk.cn

TS:   "7".padStart(3, "0")
来源：http://izy.zdqjudy.top

Java: String.format("%03d", 7)
来源：http://ezm.daria6918.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://szw.pengpengdd.cyou

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://djy.316326.xyz

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://kxe.quarkkingdee.top

[E11] 反转字符串
来源：http://ejw.yj202588.top

Py:   s[::-1]
来源：http://ofh.pengpengdd.cyou

PHP:  strrev($s);
来源：http://ezz.vqdsnc.cn

JS:   [...s].reverse().join("")
来源：http://vhw.jinqigufen.top

TS:   [...s].reverse().join("")
来源：http://wuc.zhijiandao.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://wfu.yongpay.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://vha.zhoulong.xyz

Ruby: s.reverse
来源：http://pdo.yangfankeji.com

C#:   new string(s.Reverse().ToArray())
来源：http://iux.jinyuanbaomall.cn

[E12] 统计某字符出现次数
来源：http://pbg.gaohongyu789.top

Py:   s.count("a")
来源：http://cna.cdnleiting.top

PHP:  substr_count($s, "a");
来源：http://ssq.yj202588.top

JS:   s.split("a").length - 1
来源：http://xuy.svipenyu.cn

TS:   s.split("a").length - 1
来源：http://myv.pycfn.com

Java: s.chars().filter(c -> c == 'a').count()
来源：http://myg.zhaomingkeji.xyz

Go:   strings.Count(s, "a")
来源：http://kyt.daxiang520.top

Ruby: s.count("a")
来源：http://xoe.zhixingplan.top

C#:   s.Count(c => c == 'a')
来源：http://pkk.zhoulong.xyz

[E13] 逐字符遍历
来源：http://aru.sufxvd.cn

Py:   for ch in s: print(ch)
来源：http://xip.fanxiaobao.xyz

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://gcd.svipenyu.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://efs.shanyushiyangkeji.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://rok.xuetiantiany.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://wpm.ivvv.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://ixc.chenlongwang.top

Ruby: s.each_char { |ch| puts ch }
来源：http://nrn.sxryk.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://bsd.hysaishi.cn

[E14] URL 编码与 Base64
来源：http://vlo.yuanzhike.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hfr.hesvh.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://obz.hysaishi.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://ptj.shangyingyoupin.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://ymm.0kj1m.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://vmo.xinyue.icu

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hug.yj202588.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://yvb.xuetiantiany.cn


<!-- 参考信息 -->