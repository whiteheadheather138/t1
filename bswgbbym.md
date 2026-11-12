代发 wailian999

C#:   list.GetRange(1, 3);
来源：http://hup.nanxuanxn.top

[D08] 合并两个数组
来源：http://zqw.xinyue.icu

Py:   a + b;  a.extend(b)
来源：http://dhj.sweek.top

PHP:  array_merge($a, $b);
来源：http://jxs.jianghu66.top

JS:   [...a, ...b];  a.concat(b);
来源：http://dpg.smart0.xyz

TS:   [...a, ...b];
来源：http://pag.xylfe.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://szv.bjfxy.top

Go:   append(a, b...)
来源：http://sfl.birdmap.top

Ruby: a + b;  a.concat(b)
来源：http://ugi.jlsjyb.cn

C#:   a.Concat(b).ToList()
来源：http://xje.chenlongwang.top

[D09] 排序（升序）
来源：http://rcv.xylfe.cn

Py:   sorted(arr);  arr.sort()
来源：http://tcf.uphjek.com

PHP:  sort($arr);
来源：http://uti.bbcook.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://edk.hnqzz.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://cey.shangyingyoupin.top

Java: Collections.sort(list);  list.sort(null);
来源：http://ktt.yvedp.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://amo.hesvh.cn

Ruby: arr.sort
来源：http://bkn.dianchejie.cn

C#:   list.Sort();
来源：http://zsg.guowangkeji.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://vst.uphjek.com

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://dlt.zdqjudy.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://zqh.hongshengwenyu.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://ydk.52xcode.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://mrk.xuanzx.com

Java: list.sort(Comparator.comparing(Person::age));
来源：http://rwy.sufxvd.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://urs.chenzaomai.com

Ruby: arr.sort_by { |x| x[:age] }
来源：http://nvg.yuxming.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://epl.zhixingplan.top

[D11] 反转数组
来源：http://iwc.jinqigfzy.top

Py:   arr[::-1];  arr.reverse()
来源：http://obf.zdbjq.cn

PHP:  array_reverse($arr);
来源：http://acd.haohaochexian.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://lgb.andypj.xyz

TS:   [...arr].reverse();
来源：http://nqi.uphjek.com

Java: Collections.reverse(list);
来源：http://gii.fehbvm.com

Go:   slices.Reverse(arr)
来源：http://iaj.zhixingplan.top

Ruby: arr.reverse
来源：http://khe.shzxlz.cn

C#:   list.Reverse();
来源：http://lkb.feifeiyinyue.top

[D12] 查找元素下标
来源：http://nds.wangshuangyany.cn

Py:   arr.index(x);  x in arr
来源：http://aay.yongpay.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://nck.ctjpmb.com

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://tme.dashuyun.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://gjx.tian-w.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://jsj.bjfxy.top

Go:   slices.Index(arr, x)
来源：http://pqw.ydzc1.top

Ruby: arr.index(x)
来源：http://vey.yongpay.top

C#:   list.IndexOf(x);
来源：http://dxo.smart0.xyz

[D13] 过滤（保留满足条件的）
来源：http://bop.yfazqb.com

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://vgc.shanyushiyangkeji.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://mqn.haohaochexian.top

JS:   arr.filter(x => x > 3)
来源：http://fls.gotoacloud.top

TS:   arr.filter(x => x > 3)
来源：http://yto.jqgfzy.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://wzg.yongpay.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://wrs.shangyingyoupin.top

Ruby: arr.select { |x| x > 3 }
来源：http://imu.chenlongwang.top

C#:   list.Where(x => x > 3).ToList()
来源：http://upl.pycfn.com

[D14] 映射转换（每个元素变形）
来源：http://rpc.snrcjt.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://occ.havefunace.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://xyv.ydzc1.top

JS:   arr.map(x => x * 2)
来源：http://ixf.shuidangran.top

TS:   arr.map(x => x * 2)
来源：http://gzw.shzxlz.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://ulg.jqgfzy.top

Go:   // 手写循环
来源：http://qij.zhijiandao.cn

Ruby: arr.map { |x| x * 2 }
来源：http://jol.ydzc1.top

C#:   list.Select(x => x * 2).ToList()
来源：http://eic.nanxinkj.top

[D15] 去重
来源：http://gpd.snrcjt.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://frf.bbcook.cn

PHP:  array_unique($arr);
来源：http://ogn.vehdjk.com

JS:   [...new Set(arr)]
来源：http://azj.chenlongwang.top

TS:   [...new Set(arr)]
来源：http://ino.shangyingyoupin.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://gcm.316326.xyz

Go:   // 用 map[T]struct{} 手写
来源：http://pfk.kuanghao11.cn

Ruby: arr.uniq
来源：http://gcb.ywan-chungtsiang.top

C#:   list.Distinct().ToList()
来源：http://pzn.tarul.cn

[D16] 求和与平均值
来源：http://onq.wangshuangyany.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://var.zhiwuduotai.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://wio.vehdjk.com

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://cne.yj202588.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://epe.feifeiyinyue.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://yum.316326.xyz

Go:   // 手写循环累加
来源：http://lir.tianlin.xyz

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://gjp.havefunace.top

C#:   list.Sum();  list.Average()
来源：http://cbb.ctjpmb.com

[D17] 最大值与最小值
来源：http://oku.chenjidiqi.icu

Py:   max(arr);  min(arr)
来源：http://yhd.c1oappe.top

PHP:  max($arr);  min($arr);
来源：http://oul.cdnleiting.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://ydc.hysaishi.cn

TS:   Math.max(...arr);
来源：http://rfb.cucudq.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://kgb.316326.xyz

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://yxn.vehdjk.com

Ruby: arr.max;  arr.min
来源：http://dvt.xylfe.cn

C#:   list.Max();  list.Min()
来源：http://sfw.bbcook.cn

[D18] 扁平化嵌套数组
来源：http://ooe.ctjpmb.com

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://gsw.xuanzx.com

PHP:  array_merge(...$nested);
来源：http://exv.ehwqpu.com

JS:   nested.flat();  nested.flat(Infinity)
来源：http://uln.hnxiangtu.top

TS:   nested.flat();
来源：http://ulk.zhongyouzk.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://ark.bjfxy.top

Go:   // 手写双层循环
来源：http://yuc.shangyingyoupin.top

Ruby: nested.flatten
来源：http://uyf.tian-w.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://zsu.svipenyu.cn

[D19] 按字段分组
来源：http://xjn.shuidangran.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://zxt.hnqzz.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://nth.tarul.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://ngr.birdmap.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://aco.zhongyouzk.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://dbk.yonumen.top

Go:   // 手写 map[string][]T
来源：http://gfu.cheryme.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://xyr.zdqjudy.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://aks.zdqjudy.top

[D20] 统计每个元素出现次数
来源：http://kyb.zhixingplan.top

Py:   Counter(arr)
来源：http://xrg.52xcode.cn

PHP:  array_count_values($arr);
来源：http://pao.vqdsnc.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hwz.nwbrower.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://imj.hnqzz.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://vkh.52xcode.cn

Go:   // 手写 map[T]int
来源：http://asz.smart0.xyz

Ruby: arr.tally
来源：http://qzf.9152youxi.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://jgx.snrcjt.cn

[D21] 判断是否包含某元素
来源：http://lcw.chenjidiqi.icu

Py:   x in arr
来源：http://grl.ywan-chungtsiang.top

PHP:  in_array($x, $arr, true);
来源：http://hhe.vehdjk.com

JS:   arr.includes(x)
来源：http://ehb.xuanzx.com

TS:   arr.includes(x)
来源：http://aqf.yj20258888.top

Java: list.contains(x)
来源：http://tcj.ehwqpu.com

Go:   slices.Contains(arr, x)
来源：http://com.bjfxy.top

Ruby: arr.include?(x)
来源：http://yop.hysaishi.cn

C#:   list.Contains(x)
来源：http://hyb.jinqigfzy.top

[D22] 复制数组（避免共享引用）
来源：http://urc.wangdashe.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://nyr.hammf.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://nxb.hnxiangtu.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://tjz.feifeiyinyue.top

TS:   [...arr];
来源：http://aza.316326.xyz

Java: new ArrayList<>(list);
来源：http://wec.ydzc1.top

Go:   copied := append([]int(nil), arr...)
来源：http://dem.jqgufenzy.top

Ruby: arr.dup;  arr.clone
来源：http://hjo.guannengcc.top

C#:   new List<int>(list);
来源：http://gon.jlsjyb.cn

[D23] reduce 累积计算
来源：http://vtr.shanyushiyangkeji.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://xke.hcnkem.com

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://sir.yuanzhike.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mkv.chenlongwang.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hsf.vqdsnc.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://xnp.hammf.cn

Go:   // 手写循环
来源：http://tgb.meibo888.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://mlp.xylfe.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://mni.quarkkingdee.top

[D24] 字典 / Map 基本操作
来源：http://xjl.jinqigufen.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://onm.zhijiandao.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://pyc.uphjek.com

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://jkd.jinqigufen.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://ess.sufxvd.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://epm.chenzaomai.com

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://suw.ehwqpu.com

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://cjc.zhoulong.xyz

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://rlq.nanxuanxn.top

[D25] Set 集合去重与交并差
来源：http://iia.nwbrower.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://btq.bbcook.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://sdy.tanke756.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://yha.fehbvm.com

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://ina.hcnkem.com

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://yjd.316326.xyz

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://fqv.shangyingyoupin.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://qzv.zhijiandao.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://tal.zhoulong.xyz

[D26] 数组转字符串
来源：http://uvt.gzhubu.top

Py:   ", ".join(map(str, arr))
来源：http://mco.ydjk.org.cn

PHP:  implode(", ", $arr);
来源：http://lob.jiagoushi.top

JS:   arr.join(", ")
来源：http://egi.yfazqb.com

TS:   arr.join(", ")
来源：http://gtc.havefunace.top

Java: String.join(", ", list)
来源：http://cqn.meibo888.top

Go:   strings.Join(strs, ", ")
来源：http://umi.guowangkeji.top

Ruby: arr.join(", ")
来源：http://zav.c1oappe.top

C#:   string.Join(", ", list)
来源：http://lmb.zhoulong.xyz

================================================================================
来源：http://zht.epnwcf.com

E. 字符串处理
来源：http://jau.jinyuanbaomall.cn

================================================================================
来源：http://gjf.ppjwa.cn

[E01] 拼接字符串
来源：http://iuc.quarkkingdee.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://nam.ydzc1.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://fka.uphjek.com

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://fsi.shanyushiyangtech.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://fjd.fanxiaobao.xyz

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://ywb.tian-w.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://nyj.daria6918.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://onp.ehwqpu.com

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://qnl.ybcxt.top

[E02] 重复字符串
来源：http://jbo.hnqzz.top

Py:   "ab" * 3
来源：http://ysl.hfpthk.cn

PHP:  str_repeat("ab", 3);
来源：http://qvx.zdqjudy.top

JS:   "ab".repeat(3)
来源：http://nel.shanyushiyangkeji.top

TS:   "ab".repeat(3)
来源：http://nez.cheryme.top

Java: "ab".repeat(3)
来源：http://yxx.cqqwz.cn

Go:   strings.Repeat("ab", 3)
来源：http://xtl.shangyingyoupin.top

Ruby: "ab" * 3
来源：http://yau.jyoumei.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://mdz.gogol.net.cn

[E03] 截取子串
来源：http://czc.chenzaomai.com

Py:   s[1:4];  s[:3];  s[3:]
来源：http://mpw.shangyingyoupin.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://fzk.snrcjt.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://ioc.daria6918.cn

TS:   s.slice(1, 4)
来源：http://lwc.aizwys.cn

Java: s.substring(1, 4)
来源：http://fqf.hcnkem.com

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://bxv.ctjpmb.com

Ruby: s[1, 3];  s[1..3]
来源：http://qua.sufxvd.cn

C#:   s.Substring(1, 3)
来源：http://mne.jiagoushi.top

[E04] 查找子串位置
来源：http://xii.9152youxi.cn

Py:   s.find("x");  s.index("x")
来源：http://jgo.fehbvm.com

PHP:  strpos($s, "x");
来源：http://qzk.tianlin.xyz

JS:   s.indexOf("x");  s.search(/x/)
来源：http://cwu.cqqwz.cn

TS:   s.indexOf("x")
来源：http://dse.zdbjq.cn

Java: s.indexOf("x")
来源：http://kvp.yj202588.top

Go:   strings.Index(s, "x")
来源：http://ayr.vehdjk.com

Ruby: s.index("x")
来源：http://egb.hywenlv.cn

C#:   s.IndexOf("x")
来源：http://ouq.ydzc1.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://opf.zhiwuduotai.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hqr.zycfv.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://kij.hongshengwenyu.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://egd.guannengcc.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://cbk.hammf.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://uxa.zhijiandao.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://byg.shzxlz.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://ssd.gzhubu.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://dil.vehdjk.com

[E06] 替换子串
来源：http://jzj.daria6918.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://llc.daxiang520.top

PHP:  str_replace("a", "b", $s);
来源：http://nsd.fzhhl.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://rcu.smart0.xyz

TS:   s.replaceAll("a", "b")
来源：http://sau.redwolf501.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://gkh.ivvv.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://ulg.meibo888.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://ypz.zhoulong.xyz

C#:   s.Replace("a", "b")
来源：http://xxp.jqgfzy.top

[E07] 按分隔符拆分
来源：http://okv.hywenlv.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://fbz.ppjwa.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://uhp.yfazqb.com

JS:   s.split(",");  s.split(/\s+/)
来源：http://ecs.nanxinkj.top

TS:   s.split(",")
来源：http://aqc.hysaishi.cn

Java: s.split(",");  s.split("\\s+")
来源：http://leo.xuetiantiany.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://iln.0kj1m.cn

Ruby: s.split(",");  s.split
来源：http://xlz.uphjek.com

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://jpc.yuanzhike.top

[E08] 数组按分隔符合并
来源：http://jta.hywenlv.cn

Py:   ",".join(items)
来源：http://azy.jyoumei.cn

PHP:  implode(",", $items);
来源：http://ypb.zhengqikj.top

JS:   items.join(",")
来源：http://dev.dianchejie.cn

TS:   items.join(",")
来源：http://coo.tianlin.xyz

Java: String.join(",", items)
来源：http://zlx.pengpengdd.cyou

Go:   strings.Join(items, ",")
来源：http://tyf.chenjidiqi.icu

Ruby: items.join(",")
来源：http://xxv.yvedp.cn

C#:   string.Join(",", items)
来源：http://jkf.hongshengwenyu.top

[E09] 去除所有空白字符
来源：http://bqm.ydjk.org.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://fjl.yangfankeji.com

PHP:  preg_replace('/\s+/', '', $s);
来源：http://cjk.havefunace.top

JS:   s.replace(/\s+/g, "")
来源：http://vrq.nanxinkj.top

TS:   s.replace(/\s+/g, "")
来源：http://csr.haohaochexian.top

Java: s.replaceAll("\\s+", "")
来源：http://xec.kuanghao11.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://zzv.jqgfzy.top

Ruby: s.gsub(/\s+/, "")
来源：http://sfv.hesvh.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://muv.ydzc1.top

[E10] 左侧补零 / 定长填充
来源：http://vbc.birdmap.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://awh.yangfankeji.com

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://dxm.meibo888.top

JS:   "7".padStart(3, "0")
来源：http://spy.cdnleiting.top

TS:   "7".padStart(3, "0")
来源：http://uff.shanyushiyangtech.top

Java: String.format("%03d", 7)
来源：http://bsf.cqqwz.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://ftf.sysykeji.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://few.zhengqikj.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://bha.xingfuxueyuan.xyz

[E11] 反转字符串
来源：http://jdo.shangyingyoupin.top

Py:   s[::-1]
来源：http://xsv.birdmap.top

PHP:  strrev($s);
来源：http://fxd.epnwcf.com

JS:   [...s].reverse().join("")
来源：http://xrp.hfpthk.cn

TS:   [...s].reverse().join("")
来源：http://qyr.gotoacloud.top

Java: new StringBuilder(s).reverse().toString()
来源：http://rmz.ydjk.org.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://uws.aizwys.cn

Ruby: s.reverse
来源：http://urw.yangfankeji.com

C#:   new string(s.Reverse().ToArray())
来源：http://ooi.jinyuanbaomall.cn

[E12] 统计某字符出现次数
来源：http://unh.zhoulong.xyz

Py:   s.count("a")
来源：http://tqa.feifeiyinyue.top

PHP:  substr_count($s, "a");
来源：http://afj.svipenyu.cn

JS:   s.split("a").length - 1
来源：http://svw.bjfxy.top

TS:   s.split("a").length - 1
来源：http://due.aizwys.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://xfc.hnqzz.top

Go:   strings.Count(s, "a")
来源：http://iqu.zhijiandao.cn

Ruby: s.count("a")
来源：http://bqi.gotoacloud.top

C#:   s.Count(c => c == 'a')
来源：http://fix.hongshengwenyu.top

[E13] 逐字符遍历
来源：http://jgi.ydzc1.top

Py:   for ch in s: print(ch)
来源：http://zzt.hesvh.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://lte.fzhhl.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://pgq.jinghuilouyu.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://asl.yuanzhike.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://bza.0kj1m.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://nbp.cqqwz.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://trl.zycfv.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://szk.yuanzhike.top

[E14] URL 编码与 Base64
来源：http://umr.cdnleiting.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://aqm.hnqzz.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://bzs.yongpay.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://iwi.quarkkingdee.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://ofq.mhx1999.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://ibo.fanxiaobao.xyz

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://ths.zhengqikj.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://mog.fengsongda.top


<!-- 参考信息 -->