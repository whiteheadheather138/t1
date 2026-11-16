代发 wailian999

JS:   [...a, ...b];  a.concat(b);
来源：http://tdq.zhijiandao.cn

TS:   [...a, ...b];
来源：http://zix.yvedp.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://knq.quarkkingdee.top

Go:   append(a, b...)
来源：http://qll.feifeiyinyue.top

Ruby: a + b;  a.concat(b)
来源：http://rsl.hywenlv.cn

C#:   a.Concat(b).ToList()
来源：http://bqh.nwbrower.top

[D09] 排序（升序）
来源：http://xrh.nwbrower.top

Py:   sorted(arr);  arr.sort()
来源：http://bgj.daria6918.cn

PHP:  sort($arr);
来源：http://zai.zycfv.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://xlv.gaohongyu789.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://sgo.nwbrower.top

Java: Collections.sort(list);  list.sort(null);
来源：http://qgt.316326.xyz

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://bqa.zhijiandao.cn

Ruby: arr.sort
来源：http://kfa.havefunace.top

C#:   list.Sort();
来源：http://mtu.ppjwa.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://xwg.gzhubu.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://leq.ehwqpu.com

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wvg.shzxlz.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://gtl.nanxuanxn.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://oqu.yj20258888.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://ucb.zhongyouzk.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://xft.hfpthk.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://ofa.sysykeji.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://pqz.zhaomingkeji.xyz

[D11] 反转数组
来源：http://pyf.wangshuangyany.cn

Py:   arr[::-1];  arr.reverse()
来源：http://gcz.wangdashe.top

PHP:  array_reverse($arr);
来源：http://azt.hesvh.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://urv.nwbrower.top

TS:   [...arr].reverse();
来源：http://lwh.nanxuanxn.top

Java: Collections.reverse(list);
来源：http://fbe.birdmap.top

Go:   slices.Reverse(arr)
来源：http://qgw.fengsongda.top

Ruby: arr.reverse
来源：http://owf.yuanzhike.top

C#:   list.Reverse();
来源：http://ztx.fanxiaobao.xyz

[D12] 查找元素下标
来源：http://hnf.cashguo.top

Py:   arr.index(x);  x in arr
来源：http://zsj.kuanghao11.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://wgm.52xcode.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://due.tarul.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mdv.hywenlv.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://bkq.fanxiaobao.xyz

Go:   slices.Index(arr, x)
来源：http://lyb.pengpengdd.cyou

Ruby: arr.index(x)
来源：http://fcd.havefunace.top

C#:   list.IndexOf(x);
来源：http://gpi.316326.xyz

[D13] 过滤（保留满足条件的）
来源：http://tnw.guowangkeji.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://jfi.iojbl.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://zxu.aizwys.cn

JS:   arr.filter(x => x > 3)
来源：http://ili.fktsv.cn

TS:   arr.filter(x => x > 3)
来源：http://arl.zhixingplan.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://xun.tanke756.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://iym.xziqi.cn

Ruby: arr.select { |x| x > 3 }
来源：http://qyu.zhixingplan.top

C#:   list.Where(x => x > 3).ToList()
来源：http://olo.yvedp.cn

[D14] 映射转换（每个元素变形）
来源：http://ufn.chenjidiqi.icu

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://kwo.9152youxi.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://ayv.zhiwuduotai.top

JS:   arr.map(x => x * 2)
来源：http://wqd.fehbvm.com

TS:   arr.map(x => x * 2)
来源：http://krv.cqqwz.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://axs.ivvv.top

Go:   // 手写循环
来源：http://lwc.xylfe.cn

Ruby: arr.map { |x| x * 2 }
来源：http://cnn.yueranfly.top

C#:   list.Select(x => x * 2).ToList()
来源：http://rtj.jiagoushi.top

[D15] 去重
来源：http://sxo.haohaochexian.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://jpq.zhoulong.xyz

PHP:  array_unique($arr);
来源：http://mei.hywenlv.cn

JS:   [...new Set(arr)]
来源：http://kaz.hywenlv.cn

TS:   [...new Set(arr)]
来源：http://lnq.hcnkem.com

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://eoo.zhiwuduotai.top

Go:   // 用 map[T]struct{} 手写
来源：http://cfg.yfazqb.com

Ruby: arr.uniq
来源：http://suz.cheryme.top

C#:   list.Distinct().ToList()
来源：http://dar.hysaishi.cn

[D16] 求和与平均值
来源：http://pzz.guowangkeji.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hwr.c1oappe.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://vry.daxiang520.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://wgb.cashguo.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://qtm.c1oappe.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://jhz.yj202588.top

Go:   // 手写循环累加
来源：http://dru.haohaochexian.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://paa.hongshengwenyu.top

C#:   list.Sum();  list.Average()
来源：http://kfk.jlsjyb.cn

[D17] 最大值与最小值
来源：http://zsq.yj202588.top

Py:   max(arr);  min(arr)
来源：http://mvn.chenjidiqi.icu

PHP:  max($arr);  min($arr);
来源：http://mzl.xingfuxueyuan.xyz

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://nfm.jqgufenzy.top

TS:   Math.max(...arr);
来源：http://qrw.snrcjt.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://eou.yonumen.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://epu.yueranfly.top

Ruby: arr.max;  arr.min
来源：http://tni.52xcode.cn

C#:   list.Max();  list.Min()
来源：http://zta.fzhhl.top

[D18] 扁平化嵌套数组
来源：http://umy.fzhhl.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://sdg.feifeiyinyue.top

PHP:  array_merge(...$nested);
来源：http://hpw.yuxming.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://saf.chenzaomai.com

TS:   nested.flat();
来源：http://ofd.hnqzz.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://jki.zhijiandao.cn

Go:   // 手写双层循环
来源：http://vlr.gotoacloud.top

Ruby: nested.flatten
来源：http://ptk.zhongyouzk.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://gsy.xingfuxueyuan.xyz

[D19] 按字段分组
来源：http://rmh.ydjk.org.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://eff.shuidangran.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://dnb.nanxinkj.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://qaq.tianlin.xyz

TS:   Object.groupBy(arr, x => x.type)
来源：http://ogv.gogol.net.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://sqs.chenlongwang.top

Go:   // 手写 map[string][]T
来源：http://hxp.hnqzz.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://scz.fengsongda.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://lml.ydjk.org.cn

[D20] 统计每个元素出现次数
来源：http://rja.gotoacloud.top

Py:   Counter(arr)
来源：http://ajs.316326.xyz

PHP:  array_count_values($arr);
来源：http://bvb.shzxlz.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wme.zhongyouzk.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ycd.jqgufenzy.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://flf.cheryme.top

Go:   // 手写 map[T]int
来源：http://qot.zhixingplan.top

Ruby: arr.tally
来源：http://jtp.ppjwa.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://kcj.feifeiyinyue.top

[D21] 判断是否包含某元素
来源：http://skd.jqgfzy.top

Py:   x in arr
来源：http://wnw.andypj.xyz

PHP:  in_array($x, $arr, true);
来源：http://dge.cheryme.top

JS:   arr.includes(x)
来源：http://kfj.tarul.cn

TS:   arr.includes(x)
来源：http://efe.ppjwa.cn

Java: list.contains(x)
来源：http://dga.xingfuxueyuan.xyz

Go:   slices.Contains(arr, x)
来源：http://org.jiagoushi.top

Ruby: arr.include?(x)
来源：http://dhm.zhengqikj.top

C#:   list.Contains(x)
来源：http://obe.yonumen.top

[D22] 复制数组（避免共享引用）
来源：http://elt.zhixingplan.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://fyp.jinghuilouyu.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hcu.pengpengdd.cyou

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://vhw.jianghu66.top

TS:   [...arr];
来源：http://ytn.cashguo.top

Java: new ArrayList<>(list);
来源：http://uag.fengsongda.top

Go:   copied := append([]int(nil), arr...)
来源：http://lnm.yangfankeji.com

Ruby: arr.dup;  arr.clone
来源：http://nrv.mhx1999.top

C#:   new List<int>(list);
来源：http://gol.xingfuxueyuan.xyz

[D23] reduce 累积计算
来源：http://cdo.zhixingplan.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://rtm.cqqwz.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://ast.xuanzx.com

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://zvm.jinqigufen.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ywp.shanyushiyangkeji.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://zfc.yvedp.cn

Go:   // 手写循环
来源：http://qwy.iojbl.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://iqj.xingfuxueyuan.xyz

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://plt.zhengqikj.top

[D24] 字典 / Map 基本操作
来源：http://ewn.ybcxt.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://ymq.redwolf501.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://xff.ywan-chungtsiang.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://atv.hnxiangtu.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hom.ydjk.org.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://xlp.c1oappe.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://vds.xingfuxueyuan.xyz

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://ofe.cqqwz.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://qdl.jianghu66.top

[D25] Set 集合去重与交并差
来源：http://hmh.yuanzhike.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://jbo.nwbrower.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://nrv.hnxiangtu.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://aju.yonumen.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://xoy.jinqigufen.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://ebg.nanxinkj.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://ahg.yj20258888.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://nsu.hongshengwenyu.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://uim.jinqigufen.top

[D26] 数组转字符串
来源：http://sad.chenlongwang.top

Py:   ", ".join(map(str, arr))
来源：http://gul.nanxuanxn.top

PHP:  implode(", ", $arr);
来源：http://kly.zhoulong.xyz

JS:   arr.join(", ")
来源：http://zfa.cucudq.cn

TS:   arr.join(", ")
来源：http://anh.uphjek.com

Java: String.join(", ", list)
来源：http://agf.nanxuanxn.top

Go:   strings.Join(strs, ", ")
来源：http://nej.bjfxy.top

Ruby: arr.join(", ")
来源：http://zky.mhx1999.top

C#:   string.Join(", ", list)
来源：http://fcy.cdnleiting.top

================================================================================
来源：http://min.smart0.xyz

E. 字符串处理
来源：http://khn.sufxvd.cn

================================================================================
来源：http://ddk.zdbjq.cn

[E01] 拼接字符串
来源：http://pxa.birdmap.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://ovc.hywenlv.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://cok.pengpengdd.cyou

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://odn.jiagoushi.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://zqn.hcnkem.com

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://ikw.tanke756.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://ysq.zhijiandao.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://nhs.xinyue.icu

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://ycs.0kj1m.cn

[E02] 重复字符串
来源：http://aou.bjfxy.top

Py:   "ab" * 3
来源：http://dob.guowangkeji.top

PHP:  str_repeat("ab", 3);
来源：http://sui.guowangkeji.top

JS:   "ab".repeat(3)
来源：http://yli.52xcode.cn

TS:   "ab".repeat(3)
来源：http://guv.daxiang520.top

Java: "ab".repeat(3)
来源：http://nld.hnqzz.top

Go:   strings.Repeat("ab", 3)
来源：http://wha.xingfuxueyuan.xyz

Ruby: "ab" * 3
来源：http://oyw.nanxuanxn.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hqu.sysykeji.top

[E03] 截取子串
来源：http://fev.bjfxy.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://uyh.zhiwuduotai.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://ebb.ybcxt.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://pwf.shuidangran.top

TS:   s.slice(1, 4)
来源：http://rkh.xuetiantiany.cn

Java: s.substring(1, 4)
来源：http://hve.wangshuangyany.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://eyi.xuetiantiany.cn

Ruby: s[1, 3];  s[1..3]
来源：http://vvu.ctjpmb.com

C#:   s.Substring(1, 3)
来源：http://fyy.haohaochexian.top

[E04] 查找子串位置
来源：http://nea.nanxinkj.top

Py:   s.find("x");  s.index("x")
来源：http://jmh.cqqwz.cn

PHP:  strpos($s, "x");
来源：http://bdo.yj20258888.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://upc.yj20258888.top

TS:   s.indexOf("x")
来源：http://rrb.hnxiangtu.top

Java: s.indexOf("x")
来源：http://elz.sweek.top

Go:   strings.Index(s, "x")
来源：http://kjy.snrcjt.cn

Ruby: s.index("x")
来源：http://ajv.ywan-chungtsiang.top

C#:   s.IndexOf("x")
来源：http://lyu.jiagoushi.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://joq.ydjk.org.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://fdi.hammf.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://rzx.9152youxi.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://cjk.uphjek.com

TS:   s.includes("x");  s.startsWith("a")
来源：http://nzz.tian-w.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mox.iojbl.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://bta.cashguo.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://wsz.guowangkeji.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://etk.zhixingplan.top

[E06] 替换子串
来源：http://gwx.guowangkeji.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://uio.zhaomingkeji.xyz

PHP:  str_replace("a", "b", $s);
来源：http://vje.ydzc1.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://sur.zdqjudy.top

TS:   s.replaceAll("a", "b")
来源：http://hxl.sufxvd.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://vql.xuetiantiany.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://cap.sjlbkw.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://ypt.xuanzx.com

C#:   s.Replace("a", "b")
来源：http://vyk.jinyuanbaomall.cn

[E07] 按分隔符拆分
来源：http://qkz.zhijiandao.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://tmx.wangdashe.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://jcf.jqgufenzy.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://gfe.uphjek.com

TS:   s.split(",")
来源：http://ihs.jyoumei.cn

Java: s.split(",");  s.split("\\s+")
来源：http://uyp.haohaochexian.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://vic.zdqjudy.top

Ruby: s.split(",");  s.split
来源：http://ewp.sweek.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://ekl.shanyushiyangkeji.top

[E08] 数组按分隔符合并
来源：http://gwq.yonumen.top

Py:   ",".join(items)
来源：http://xtz.gaohongyu789.top

PHP:  implode(",", $items);
来源：http://cps.yueranfly.top

JS:   items.join(",")
来源：http://iob.daria6918.cn

TS:   items.join(",")
来源：http://rng.vqdsnc.cn

Java: String.join(",", items)
来源：http://xln.chenjidiqi.icu

Go:   strings.Join(items, ",")
来源：http://eon.wangdashe.top

Ruby: items.join(",")
来源：http://trb.zdbjq.cn

C#:   string.Join(",", items)
来源：http://wgw.xziqi.cn

[E09] 去除所有空白字符
来源：http://xch.zhaomingkeji.xyz

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://fpu.tanke756.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://zqu.zdqjudy.top

JS:   s.replace(/\s+/g, "")
来源：http://xzx.hnqzz.top

TS:   s.replace(/\s+/g, "")
来源：http://dou.zdbjq.cn

Java: s.replaceAll("\\s+", "")
来源：http://rxi.yfazqb.com

Go:   strings.Join(strings.Fields(s), "")
来源：http://hey.ivvv.top

Ruby: s.gsub(/\s+/, "")
来源：http://fhh.zhengqikj.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://qqp.cheryme.top

[E10] 左侧补零 / 定长填充
来源：http://enq.ctjpmb.com

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://aff.smart0.xyz

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://zva.cdnleiting.top

JS:   "7".padStart(3, "0")
来源：http://szr.cucudq.cn

TS:   "7".padStart(3, "0")
来源：http://cpg.pengpengdd.cyou

Java: String.format("%03d", 7)
来源：http://yup.hcnkem.com

Go:   fmt.Sprintf("%03d", 7)
来源：http://ytx.ydzc1.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://bij.jinqigufen.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://bza.xuetiantiany.cn

[E11] 反转字符串
来源：http://cpd.9152youxi.cn

Py:   s[::-1]
来源：http://dlh.uphjek.com

PHP:  strrev($s);
来源：http://une.sufxvd.cn

JS:   [...s].reverse().join("")
来源：http://gzd.guowangkeji.top

TS:   [...s].reverse().join("")
来源：http://nqi.zhengqikj.top

Java: new StringBuilder(s).reverse().toString()
来源：http://dgg.zhengqikj.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://dgr.zhoulong.xyz

Ruby: s.reverse
来源：http://yvj.shanyushiyangkeji.top

C#:   new string(s.Reverse().ToArray())
来源：http://ses.guowangkeji.top

[E12] 统计某字符出现次数
来源：http://ept.yj20258888.top

Py:   s.count("a")
来源：http://rpt.gaohongyu789.top

PHP:  substr_count($s, "a");
来源：http://iwa.yfazqb.com

JS:   s.split("a").length - 1
来源：http://zwy.bbcook.cn

TS:   s.split("a").length - 1
来源：http://bon.pycfn.com

Java: s.chars().filter(c -> c == 'a').count()
来源：http://xht.svipenyu.cn

Go:   strings.Count(s, "a")
来源：http://epq.jinyuanbaomall.cn

Ruby: s.count("a")
来源：http://tso.hammf.cn

C#:   s.Count(c => c == 'a')
来源：http://xba.sweek.top

[E13] 逐字符遍历
来源：http://bnd.vehdjk.com

Py:   for ch in s: print(ch)
来源：http://gro.birdmap.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://yhb.xinyue.icu

JS:   for (const ch of s) { console.log(ch); }
来源：http://zdy.meibo888.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://ooy.c1oappe.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://qsb.yongpay.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://pev.cqqwz.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://nnk.hfpthk.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://bnn.zdqjudy.top

[E14] URL 编码与 Base64
来源：http://kys.vqdsnc.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://xwo.ybcxt.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://qbx.gotoacloud.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://tcq.hcnkem.com

TS:   encodeURIComponent(s);  btoa(s)
来源：http://taf.ivvv.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://ebr.sxryk.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://jxh.uphjek.com

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://gvl.snrcjt.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hts.feifeiyinyue.top

[E15] HTML 转义 / 反转义
来源：http://gya.nanxinkj.top

Py:   html.escape(s);  html.unescape(s)
来源：http://map.pengpengdd.cyou

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://lmc.hesvh.cn


<!-- 参考信息 -->