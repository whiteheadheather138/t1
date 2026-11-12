代发 wailian999

C#:   list.GetRange(1, 3);
来源：http://ula.sweek.top

[D08] 合并两个数组
来源：http://knh.vqdsnc.cn

Py:   a + b;  a.extend(b)
来源：http://pun.hesvh.cn

PHP:  array_merge($a, $b);
来源：http://rwh.kuanghao11.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://vgl.wangshuangyany.cn

TS:   [...a, ...b];
来源：http://kdr.epnwcf.com

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://ltz.cdnleiting.top

Go:   append(a, b...)
来源：http://wyr.hnqzz.top

Ruby: a + b;  a.concat(b)
来源：http://lxp.jinqigfzy.top

C#:   a.Concat(b).ToList()
来源：http://ixg.hfpthk.cn

[D09] 排序（升序）
来源：http://hmx.gogol.net.cn

Py:   sorted(arr);  arr.sort()
来源：http://xrc.yanxiufei.cn

PHP:  sort($arr);
来源：http://dvt.fktsv.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://sjr.jinqigfzy.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://lmn.zhoulong.xyz

Java: Collections.sort(list);  list.sort(null);
来源：http://xeo.dashuyun.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://plz.shangyingyoupin.top

Ruby: arr.sort
来源：http://niv.zdqjudy.top

C#:   list.Sort();
来源：http://vco.yueranfly.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://ykg.ywan-chungtsiang.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://wbb.fehbvm.com

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://lxu.guowangkeji.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://wzo.havefunace.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://gxx.shangyingyoupin.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://jui.yangfankeji.com

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://wdd.chenlongwang.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://mtq.daxiang520.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://csp.52xcode.cn

[D11] 反转数组
来源：http://wbt.fanxiaobao.xyz

Py:   arr[::-1];  arr.reverse()
来源：http://qjm.aibaodan.cn

PHP:  array_reverse($arr);
来源：http://jjn.andypj.xyz

JS:   [...arr].reverse();  arr.toReversed()
来源：http://vcr.dashuyun.cn

TS:   [...arr].reverse();
来源：http://fgn.xziqi.cn

Java: Collections.reverse(list);
来源：http://tlg.nanxuanxn.top

Go:   slices.Reverse(arr)
来源：http://yjw.gogol.net.cn

Ruby: arr.reverse
来源：http://wbz.fehbvm.com

C#:   list.Reverse();
来源：http://bsx.aizwys.cn

[D12] 查找元素下标
来源：http://gac.jqgufenzy.top

Py:   arr.index(x);  x in arr
来源：http://gxf.feifeiyinyue.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://kow.zhixingplan.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://bae.bbcook.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://voa.yueranfly.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://jlc.cqqwz.cn

Go:   slices.Index(arr, x)
来源：http://rjs.chenlongwang.top

Ruby: arr.index(x)
来源：http://dgz.fktsv.cn

C#:   list.IndexOf(x);
来源：http://zrg.tianlin.xyz

[D13] 过滤（保留满足条件的）
来源：http://gzf.cucudq.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://yfy.c1oappe.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://wkw.hfpthk.cn

JS:   arr.filter(x => x > 3)
来源：http://dgr.mhx1999.top

TS:   arr.filter(x => x > 3)
来源：http://kwn.zhoulong.xyz

Java: list.stream().filter(x -> x > 3).toList()
来源：http://vme.jqgufenzy.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://vqv.hammf.cn

Ruby: arr.select { |x| x > 3 }
来源：http://kxu.zhoulong.xyz

C#:   list.Where(x => x > 3).ToList()
来源：http://ebt.quarkkingdee.top

[D14] 映射转换（每个元素变形）
来源：http://ndr.yvedp.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://aks.hnqzz.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hgc.yueranfly.top

JS:   arr.map(x => x * 2)
来源：http://vmg.xziqi.cn

TS:   arr.map(x => x * 2)
来源：http://gft.ehwqpu.com

Java: list.stream().map(x -> x * 2).toList()
来源：http://hrg.zhengqikj.top

Go:   // 手写循环
来源：http://xko.iojbl.cn

Ruby: arr.map { |x| x * 2 }
来源：http://fzn.ydjk.org.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://ggi.9152youxi.cn

[D15] 去重
来源：http://wuo.hysaishi.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://wwg.cheryme.top

PHP:  array_unique($arr);
来源：http://tps.xuetiantiany.cn

JS:   [...new Set(arr)]
来源：http://ouj.xuetiantiany.cn

TS:   [...new Set(arr)]
来源：http://hso.redwolf501.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://bny.zhaomingkeji.xyz

Go:   // 用 map[T]struct{} 手写
来源：http://rgq.zhiwuduotai.top

Ruby: arr.uniq
来源：http://slh.yangfankeji.com

C#:   list.Distinct().ToList()
来源：http://wxs.52xcode.cn

[D16] 求和与平均值
来源：http://wpn.jianghu66.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://aui.iojbl.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://kvq.wangshuangyany.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://npz.smart0.xyz

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://byx.vqdsnc.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://xvy.iojbl.cn

Go:   // 手写循环累加
来源：http://ppw.aibaodan.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://rgq.zycfv.cn

C#:   list.Sum();  list.Average()
来源：http://xgu.yanxiufei.cn

[D17] 最大值与最小值
来源：http://vrl.yj20258.top

Py:   max(arr);  min(arr)
来源：http://kqz.shzxlz.cn

PHP:  max($arr);  min($arr);
来源：http://mfd.redwolf501.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://evd.tian-w.cn

TS:   Math.max(...arr);
来源：http://iue.9152youxi.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://tdo.sysykeji.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://kld.pycfn.com

Ruby: arr.max;  arr.min
来源：http://ikk.jlsjyb.cn

C#:   list.Max();  list.Min()
来源：http://vgg.52xcode.cn

[D18] 扁平化嵌套数组
来源：http://cnu.jyoumei.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://tjt.snrcjt.cn

PHP:  array_merge(...$nested);
来源：http://kpq.jinqigfzy.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://miy.zdbjq.cn

TS:   nested.flat();
来源：http://ogq.shangyingyoupin.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://pqt.gotoacloud.top

Go:   // 手写双层循环
来源：http://tml.tianlin.xyz

Ruby: nested.flatten
来源：http://rts.cashguo.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://sey.jinyuanbaomall.cn

[D19] 按字段分组
来源：http://for.gogol.net.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://zqy.hongshengwenyu.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://buv.kuanghao11.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://fcd.chenlongwang.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://ret.dianchejie.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://rji.xylfe.cn

Go:   // 手写 map[string][]T
来源：http://ett.hesvh.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://rzh.zdbjq.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://ydh.wangshuangyany.cn

[D20] 统计每个元素出现次数
来源：http://psp.chenlongwang.top

Py:   Counter(arr)
来源：http://lqr.snrcjt.cn

PHP:  array_count_values($arr);
来源：http://edw.svipenyu.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://uuo.52xcode.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ipd.jqgfzy.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://nrj.cdnleiting.top

Go:   // 手写 map[T]int
来源：http://sid.cashguo.top

Ruby: arr.tally
来源：http://mlw.fanxiaobao.xyz

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://wja.9152youxi.cn

[D21] 判断是否包含某元素
来源：http://hop.ybcxt.top

Py:   x in arr
来源：http://drn.chenzaomai.com

PHP:  in_array($x, $arr, true);
来源：http://btn.sufxvd.cn

JS:   arr.includes(x)
来源：http://woa.hcnkem.com

TS:   arr.includes(x)
来源：http://uqm.feifeiyinyue.top

Java: list.contains(x)
来源：http://rro.aibaodan.cn

Go:   slices.Contains(arr, x)
来源：http://gxc.0kj1m.cn

Ruby: arr.include?(x)
来源：http://eiq.tian-w.cn

C#:   list.Contains(x)
来源：http://upu.quarkkingdee.top

[D22] 复制数组（避免共享引用）
来源：http://nbg.epnwcf.com

Py:   arr.copy();  arr[:];  list(arr)
来源：http://bvf.sjlbkw.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://wgu.dashuyun.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://yaf.ctjpmb.com

TS:   [...arr];
来源：http://kqz.meibo888.top

Java: new ArrayList<>(list);
来源：http://emt.zhongyouzk.top

Go:   copied := append([]int(nil), arr...)
来源：http://kha.yfazqb.com

Ruby: arr.dup;  arr.clone
来源：http://guq.yongpay.top

C#:   new List<int>(list);
来源：http://qza.nanxuanxn.top

[D23] reduce 累积计算
来源：http://euo.fengsongda.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://gfp.zhaomingkeji.xyz

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://eot.yvedp.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ltj.wangdashe.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://vcl.ywan-chungtsiang.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://tib.jinghuilouyu.cn

Go:   // 手写循环
来源：http://tva.hywenlv.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://ukp.zycfv.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://etn.tianlin.xyz

[D24] 字典 / Map 基本操作
来源：http://cjc.sweek.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://wsj.snrcjt.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://ojc.xylfe.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://qxp.jinqigufen.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://djx.tianlin.xyz

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://amx.cdnleiting.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://yic.hysaishi.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hta.zycfv.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hmk.daria6918.cn

[D25] Set 集合去重与交并差
来源：http://kth.pengpengdd.cyou

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://rcj.svipenyu.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://xfk.andypj.xyz

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://rgm.gzhubu.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://gll.ybcxt.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://mrp.zhengqikj.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://vnb.yanxiufei.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://vuz.yvedp.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://syc.yonumen.top

[D26] 数组转字符串
来源：http://gsh.nanxinkj.top

Py:   ", ".join(map(str, arr))
来源：http://qci.chenjidiqi.icu

PHP:  implode(", ", $arr);
来源：http://zdk.zdqjudy.top

JS:   arr.join(", ")
来源：http://ffn.yongpay.top

TS:   arr.join(", ")
来源：http://cyr.haohaochexian.top

Java: String.join(", ", list)
来源：http://lmo.fengsongda.top

Go:   strings.Join(strs, ", ")
来源：http://cyv.yuxming.cn

Ruby: arr.join(", ")
来源：http://met.birdmap.top

C#:   string.Join(", ", list)
来源：http://stz.meibo888.top

================================================================================
来源：http://upu.jianghu66.top

E. 字符串处理
来源：http://fvp.0kj1m.cn

================================================================================
来源：http://uxm.yvedp.cn

[E01] 拼接字符串
来源：http://gim.yongpay.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://yru.jqgfzy.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://ytf.jinqigfzy.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://nrh.yuanzhike.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://ehv.dianchejie.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://uqz.chenzaomai.com

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://rxo.gzhubu.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://ven.hnqzz.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://wbu.nanxuanxn.top

[E02] 重复字符串
来源：http://cqm.iojbl.cn

Py:   "ab" * 3
来源：http://mgm.yonumen.top

PHP:  str_repeat("ab", 3);
来源：http://cem.fktsv.cn

JS:   "ab".repeat(3)
来源：http://yct.pengpengdd.cyou

TS:   "ab".repeat(3)
来源：http://cxn.shuidangran.top

Java: "ab".repeat(3)
来源：http://dfj.xuanzx.com

Go:   strings.Repeat("ab", 3)
来源：http://fib.chenzaomai.com

Ruby: "ab" * 3
来源：http://pxb.epnwcf.com

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://keu.yuanzhike.top

[E03] 截取子串
来源：http://zgl.hywenlv.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://zoj.shanyushiyangtech.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://bjh.snrcjt.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://uhj.jqgfzy.top

TS:   s.slice(1, 4)
来源：http://fmk.xuetiantiany.cn

Java: s.substring(1, 4)
来源：http://ekj.yueranfly.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://nbr.jinqigufen.top

Ruby: s[1, 3];  s[1..3]
来源：http://wqd.ppjwa.cn

C#:   s.Substring(1, 3)
来源：http://ece.ydzc1.top

[E04] 查找子串位置
来源：http://xds.tianlin.xyz

Py:   s.find("x");  s.index("x")
来源：http://zjx.fehbvm.com

PHP:  strpos($s, "x");
来源：http://fdr.bjfxy.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://jad.yueranfly.top

TS:   s.indexOf("x")
来源：http://ifp.sufxvd.cn

Java: s.indexOf("x")
来源：http://ywq.fzhhl.top

Go:   strings.Index(s, "x")
来源：http://rbt.shzxlz.cn

Ruby: s.index("x")
来源：http://vrb.cashguo.top

C#:   s.IndexOf("x")
来源：http://vll.cheryme.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://bhz.aibaodan.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://ogv.iojbl.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://drz.fehbvm.com

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://yaa.xziqi.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://dqy.cdnleiting.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://guy.xuetiantiany.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://uhv.smart0.xyz

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://mkp.guannengcc.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://gpy.iojbl.cn

[E06] 替换子串
来源：http://wlr.gotoacloud.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://xen.xinyue.icu

PHP:  str_replace("a", "b", $s);
来源：http://ldh.sufxvd.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://sdk.cheryme.top

TS:   s.replaceAll("a", "b")
来源：http://czb.jlsjyb.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ewy.jyoumei.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://vzi.snrcjt.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://rlm.jiagoushi.top

C#:   s.Replace("a", "b")
来源：http://zso.pengpengdd.cyou

[E07] 按分隔符拆分
来源：http://ovv.hysaishi.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://eyh.yangfankeji.com

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://xbc.nanxinkj.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://mxg.dashuyun.cn

TS:   s.split(",")
来源：http://jdq.havefunace.top

Java: s.split(",");  s.split("\\s+")
来源：http://afd.hongshengwenyu.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://jzc.zhixingplan.top

Ruby: s.split(",");  s.split
来源：http://mxy.bbcook.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://gnn.vqdsnc.cn

[E08] 数组按分隔符合并
来源：http://lmc.yuxming.cn

Py:   ",".join(items)
来源：http://aus.yangfankeji.com

PHP:  implode(",", $items);
来源：http://neb.xinyue.icu

JS:   items.join(",")
来源：http://kfd.jinqigufen.top

TS:   items.join(",")
来源：http://tzn.jianghu66.top

Java: String.join(",", items)
来源：http://gtu.yonumen.top

Go:   strings.Join(items, ",")
来源：http://lxh.ehwqpu.com

Ruby: items.join(",")
来源：http://rcm.ppjwa.cn

C#:   string.Join(",", items)
来源：http://ghz.dashuyun.cn

[E09] 去除所有空白字符
来源：http://skm.shanyushiyangkeji.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://jfa.chenlongwang.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://jxn.tanke756.top

JS:   s.replace(/\s+/g, "")
来源：http://qjw.bbcook.cn

TS:   s.replace(/\s+/g, "")
来源：http://rhy.hywenlv.cn

Java: s.replaceAll("\\s+", "")
来源：http://nmg.andypj.xyz

Go:   strings.Join(strings.Fields(s), "")
来源：http://pjy.nanxuanxn.top

Ruby: s.gsub(/\s+/, "")
来源：http://byp.andypj.xyz

C#:   Regex.Replace(s, @"\s+", "")
来源：http://lxc.cqqwz.cn

[E10] 左侧补零 / 定长填充
来源：http://kcx.cdnleiting.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://qrt.jinqigfzy.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://qze.fzhhl.top

JS:   "7".padStart(3, "0")
来源：http://lvn.sxryk.cn

TS:   "7".padStart(3, "0")
来源：http://suh.fengsongda.top

Java: String.format("%03d", 7)
来源：http://wbb.jinyuanbaomall.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://lku.aizwys.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://kfl.zhongyouzk.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://dga.guowangkeji.top

[E11] 反转字符串
来源：http://szp.hfpthk.cn

Py:   s[::-1]
来源：http://tot.yangfankeji.com

PHP:  strrev($s);
来源：http://uei.quarkkingdee.top

JS:   [...s].reverse().join("")
来源：http://ldu.nanxuanxn.top

TS:   [...s].reverse().join("")
来源：http://ngg.ybcxt.top

Java: new StringBuilder(s).reverse().toString()
来源：http://pfw.havefunace.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://uyn.andypj.xyz

Ruby: s.reverse
来源：http://zzy.wangdashe.top

C#:   new string(s.Reverse().ToArray())
来源：http://uke.aibaodan.cn

[E12] 统计某字符出现次数
来源：http://nst.52xcode.cn

Py:   s.count("a")
来源：http://uhe.guannengcc.top

PHP:  substr_count($s, "a");
来源：http://zwf.hysaishi.cn

JS:   s.split("a").length - 1
来源：http://gra.c1oappe.top

TS:   s.split("a").length - 1
来源：http://lum.gzhubu.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://wyv.bbcook.cn

Go:   strings.Count(s, "a")
来源：http://joi.zdbjq.cn

Ruby: s.count("a")
来源：http://mbm.snrcjt.cn

C#:   s.Count(c => c == 'a')
来源：http://pll.xingfuxueyuan.xyz

[E13] 逐字符遍历
来源：http://jbd.dashuyun.cn

Py:   for ch in s: print(ch)
来源：http://wbr.gotoacloud.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://fyt.kuanghao11.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://nfx.wangdashe.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://nnv.zycfv.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://abg.tian-w.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://ema.tian-w.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://rkb.ppjwa.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://dux.smart0.xyz

[E14] URL 编码与 Base64
来源：http://qez.xziqi.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://wzp.chenjidiqi.icu

PHP:  urlencode($s);  base64_encode($s);
来源：http://sno.kuanghao11.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://ivl.hammf.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://omk.hywenlv.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://bgb.gotoacloud.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://ufm.yj20258.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hci.zhengqikj.top


<!-- 参考信息 -->