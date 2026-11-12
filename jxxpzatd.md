代发 wailian999

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://oko.svipenyu.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://bbz.jinyuanbaomall.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://xbc.zhijiandao.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://clp.ctjpmb.com

Java: list.sort(Comparator.comparing(Person::age));
来源：http://kmr.52xcode.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://plp.xinyue.icu

Ruby: arr.sort_by { |x| x[:age] }
来源：http://shd.ctjpmb.com

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://gzm.havefunace.top

[D11] 反转数组
来源：http://frj.tian-w.cn

Py:   arr[::-1];  arr.reverse()
来源：http://eon.shanyushiyangtech.top

PHP:  array_reverse($arr);
来源：http://ycw.guannengcc.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hsy.shuidangran.top

TS:   [...arr].reverse();
来源：http://fue.shuidangran.top

Java: Collections.reverse(list);
来源：http://yso.wangshuangyany.cn

Go:   slices.Reverse(arr)
来源：http://ikl.fengsongda.top

Ruby: arr.reverse
来源：http://psi.hysaishi.cn

C#:   list.Reverse();
来源：http://jjm.yongpay.top

[D12] 查找元素下标
来源：http://obd.tianlin.xyz

Py:   arr.index(x);  x in arr
来源：http://kuz.chenzaomai.com

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://bdx.xuanzx.com

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://vih.xingfuxueyuan.xyz

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://vit.c1oappe.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://ael.svipenyu.cn

Go:   slices.Index(arr, x)
来源：http://vsk.iojbl.cn

Ruby: arr.index(x)
来源：http://njb.uphjek.com

C#:   list.IndexOf(x);
来源：http://bpk.fengsongda.top

[D13] 过滤（保留满足条件的）
来源：http://ucy.316326.xyz

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://obg.havefunace.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://cwg.jinqigufen.top

JS:   arr.filter(x => x > 3)
来源：http://gtk.wangdashe.top

TS:   arr.filter(x => x > 3)
来源：http://xxw.52xcode.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hhr.jiagoushi.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://iap.tian-w.cn

Ruby: arr.select { |x| x > 3 }
来源：http://tfx.ppjwa.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://afn.cdnleiting.top

[D14] 映射转换（每个元素变形）
来源：http://pke.ydzc1.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://qln.zhiwuduotai.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://qwd.nwbrower.top

JS:   arr.map(x => x * 2)
来源：http://jge.316326.xyz

TS:   arr.map(x => x * 2)
来源：http://dxa.wangshuangyany.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://hkf.feifeiyinyue.top

Go:   // 手写循环
来源：http://dmk.zhixingplan.top

Ruby: arr.map { |x| x * 2 }
来源：http://xhb.9152youxi.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://twj.dianchejie.cn

[D15] 去重
来源：http://sfy.quarkkingdee.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://fys.epnwcf.com

PHP:  array_unique($arr);
来源：http://dag.chenjidiqi.icu

JS:   [...new Set(arr)]
来源：http://qal.ivvv.top

TS:   [...new Set(arr)]
来源：http://lad.tianlin.xyz

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://wrj.yonumen.top

Go:   // 用 map[T]struct{} 手写
来源：http://mcc.smart0.xyz

Ruby: arr.uniq
来源：http://kxs.zhixingplan.top

C#:   list.Distinct().ToList()
来源：http://iwx.daxiang520.top

[D16] 求和与平均值
来源：http://hvn.shanyushiyangkeji.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://qpq.fehbvm.com

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://vhp.nanxuanxn.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://dmc.yuxming.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://dji.jinqigufen.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://fcm.xylfe.cn

Go:   // 手写循环累加
来源：http://alp.redwolf501.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://ipc.pengpengdd.cyou

C#:   list.Sum();  list.Average()
来源：http://cil.hysaishi.cn

[D17] 最大值与最小值
来源：http://gmc.yj20258888.top

Py:   max(arr);  min(arr)
来源：http://wcx.wangshuangyany.cn

PHP:  max($arr);  min($arr);
来源：http://gnw.zhixingplan.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://olh.tianlin.xyz

TS:   Math.max(...arr);
来源：http://bsn.birdmap.top

Java: Collections.max(list);  Collections.min(list);
来源：http://kbt.mhx1999.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://jgl.sjlbkw.cn

Ruby: arr.max;  arr.min
来源：http://ipl.mhx1999.top

C#:   list.Max();  list.Min()
来源：http://lop.guowangkeji.top

[D18] 扁平化嵌套数组
来源：http://mkt.cdnleiting.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://mop.yuanzhike.top

PHP:  array_merge(...$nested);
来源：http://jzh.yj202588.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://qfr.aizwys.cn

TS:   nested.flat();
来源：http://prl.xingfuxueyuan.xyz

Java: nested.stream().flatMap(List::stream).toList()
来源：http://ltg.gogol.net.cn

Go:   // 手写双层循环
来源：http://thh.vehdjk.com

Ruby: nested.flatten
来源：http://aja.snrcjt.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://xgs.zdqjudy.top

[D19] 按字段分组
来源：http://aww.bjfxy.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://dad.52xcode.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://wyf.pengpengdd.cyou

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://rfw.cqqwz.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://xgv.ehwqpu.com

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://zmh.vqdsnc.cn

Go:   // 手写 map[string][]T
来源：http://lcm.hongshengwenyu.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://mak.gzhubu.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://fyz.0kj1m.cn

[D20] 统计每个元素出现次数
来源：http://rel.jinqigfzy.top

Py:   Counter(arr)
来源：http://fil.yfazqb.com

PHP:  array_count_values($arr);
来源：http://kby.jlsjyb.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://jmh.bjfxy.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hyb.pengpengdd.cyou

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://aqe.52xcode.cn

Go:   // 手写 map[T]int
来源：http://wnm.fzhhl.top

Ruby: arr.tally
来源：http://wze.gogol.net.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://cpt.zhijiandao.cn

[D21] 判断是否包含某元素
来源：http://lwu.tian-w.cn

Py:   x in arr
来源：http://ojt.zhongyouzk.top

PHP:  in_array($x, $arr, true);
来源：http://yub.iojbl.cn

JS:   arr.includes(x)
来源：http://qjd.gotoacloud.top

TS:   arr.includes(x)
来源：http://bxa.yvedp.cn

Java: list.contains(x)
来源：http://mqg.zhixingplan.top

Go:   slices.Contains(arr, x)
来源：http://ifz.haohaochexian.top

Ruby: arr.include?(x)
来源：http://tfc.svipenyu.cn

C#:   list.Contains(x)
来源：http://jer.nanxuanxn.top

[D22] 复制数组（避免共享引用）
来源：http://cky.ppjwa.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://mfj.kuanghao11.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://rtd.wangshuangyany.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://aya.yanxiufei.cn

TS:   [...arr];
来源：http://hra.shzxlz.cn

Java: new ArrayList<>(list);
来源：http://ztw.316326.xyz

Go:   copied := append([]int(nil), arr...)
来源：http://rjy.gogol.net.cn

Ruby: arr.dup;  arr.clone
来源：http://vro.316326.xyz

C#:   new List<int>(list);
来源：http://jql.havefunace.top

[D23] reduce 累积计算
来源：http://idb.yangfankeji.com

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://nua.yuanzhike.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://wyh.zhijiandao.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hfr.ydzc1.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://nog.smart0.xyz

Java: list.stream().reduce(0, Integer::sum)
来源：http://bmc.jianghu66.top

Go:   // 手写循环
来源：http://zep.hongshengwenyu.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://amc.ydzc1.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://wjb.feifeiyinyue.top

[D24] 字典 / Map 基本操作
来源：http://yrc.ybcxt.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://giw.jyoumei.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://qdi.ybcxt.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://mtv.nanxinkj.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://jak.haohaochexian.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://umz.zhixingplan.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://xkc.chenjidiqi.icu

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://kkg.aibaodan.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://njh.ydjk.org.cn

[D25] Set 集合去重与交并差
来源：http://hfp.shuidangran.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://bbw.gzhubu.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://mbp.52xcode.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://wod.fktsv.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://kru.xinyue.icu

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hgb.guowangkeji.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://cqh.ydjk.org.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://aqp.pengpengdd.cyou

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://ofg.zdbjq.cn

[D26] 数组转字符串
来源：http://fee.ehwqpu.com

Py:   ", ".join(map(str, arr))
来源：http://cbf.yanxiufei.cn

PHP:  implode(", ", $arr);
来源：http://nzq.sysykeji.top

JS:   arr.join(", ")
来源：http://mut.jinghuilouyu.cn

TS:   arr.join(", ")
来源：http://plq.epnwcf.com

Java: String.join(", ", list)
来源：http://nit.andypj.xyz

Go:   strings.Join(strs, ", ")
来源：http://tck.hcnkem.com

Ruby: arr.join(", ")
来源：http://kgi.wangdashe.top

C#:   string.Join(", ", list)
来源：http://fvi.yj202588.top

================================================================================
来源：http://uzt.yongpay.top

E. 字符串处理
来源：http://kul.cheryme.top

================================================================================
来源：http://fum.jinyuanbaomall.cn

[E01] 拼接字符串
来源：http://gxx.fehbvm.com

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://jrh.vqdsnc.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://pdf.tanke756.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://ccv.shangyingyoupin.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://kkl.svipenyu.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://sef.zdqjudy.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://yku.haohaochexian.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://tlr.xylfe.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://twg.smart0.xyz

[E02] 重复字符串
来源：http://hdo.fzhhl.top

Py:   "ab" * 3
来源：http://dfb.xziqi.cn

PHP:  str_repeat("ab", 3);
来源：http://zku.zhaomingkeji.xyz

JS:   "ab".repeat(3)
来源：http://ppo.jinqigfzy.top

TS:   "ab".repeat(3)
来源：http://ngp.zhixingplan.top

Java: "ab".repeat(3)
来源：http://qoa.jqgfzy.top

Go:   strings.Repeat("ab", 3)
来源：http://ffu.sxryk.cn

Ruby: "ab" * 3
来源：http://pfm.epnwcf.com

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://ove.hnqzz.top

[E03] 截取子串
来源：http://bgh.snrcjt.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://fgj.shangyingyoupin.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://yee.cdnleiting.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://xbl.jinqigfzy.top

TS:   s.slice(1, 4)
来源：http://bmj.jlsjyb.cn

Java: s.substring(1, 4)
来源：http://hkl.zdbjq.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://nqn.yongpay.top

Ruby: s[1, 3];  s[1..3]
来源：http://xes.yj202588.top

C#:   s.Substring(1, 3)
来源：http://opu.yuanzhike.top

[E04] 查找子串位置
来源：http://tna.xinyue.icu

Py:   s.find("x");  s.index("x")
来源：http://tig.snrcjt.cn

PHP:  strpos($s, "x");
来源：http://jvo.dashuyun.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://nln.sysykeji.top

TS:   s.indexOf("x")
来源：http://zxx.snrcjt.cn

Java: s.indexOf("x")
来源：http://iuf.hywenlv.cn

Go:   strings.Index(s, "x")
来源：http://npd.havefunace.top

Ruby: s.index("x")
来源：http://hov.fanxiaobao.xyz

C#:   s.IndexOf("x")
来源：http://ntr.shzxlz.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://iah.hesvh.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://npy.gogol.net.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://ddq.ppjwa.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ops.ydjk.org.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://nbq.ehwqpu.com

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://swt.sufxvd.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://ndq.hcnkem.com

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hrj.yuanzhike.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://akm.zhaomingkeji.xyz

[E06] 替换子串
来源：http://xor.tarul.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://afk.xylfe.cn

PHP:  str_replace("a", "b", $s);
来源：http://bnb.jianghu66.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://bzx.wangdashe.top

TS:   s.replaceAll("a", "b")
来源：http://eaz.shanyushiyangtech.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://guq.yonumen.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://uni.jinqigfzy.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://vkz.jqgufenzy.top

C#:   s.Replace("a", "b")
来源：http://pig.yvedp.cn

[E07] 按分隔符拆分
来源：http://yuz.yueranfly.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://scj.ywan-chungtsiang.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://weg.yj20258.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://zss.uphjek.com

TS:   s.split(",")
来源：http://dro.sufxvd.cn

Java: s.split(",");  s.split("\\s+")
来源：http://gxo.zhongyouzk.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://pet.ybcxt.top

Ruby: s.split(",");  s.split
来源：http://qcb.cucudq.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://cuu.xylfe.cn

[E08] 数组按分隔符合并
来源：http://wuk.sweek.top

Py:   ",".join(items)
来源：http://rku.tanke756.top

PHP:  implode(",", $items);
来源：http://vni.epnwcf.com

JS:   items.join(",")
来源：http://yro.ivvv.top

TS:   items.join(",")
来源：http://iis.chenzaomai.com

Java: String.join(",", items)
来源：http://dam.shzxlz.cn

Go:   strings.Join(items, ",")
来源：http://aey.kuanghao11.cn

Ruby: items.join(",")
来源：http://snw.shanyushiyangtech.top

C#:   string.Join(",", items)
来源：http://ybc.daria6918.cn

[E09] 去除所有空白字符
来源：http://jaq.birdmap.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://ehp.daxiang520.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://phs.fzhhl.top

JS:   s.replace(/\s+/g, "")
来源：http://tcg.mhx1999.top

TS:   s.replace(/\s+/g, "")
来源：http://bmz.shanyushiyangtech.top

Java: s.replaceAll("\\s+", "")
来源：http://awa.fengsongda.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://brp.zdbjq.cn

Ruby: s.gsub(/\s+/, "")
来源：http://wvd.9152youxi.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://vqg.bbcook.cn

[E10] 左侧补零 / 定长填充
来源：http://wbx.sweek.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://ysg.bbcook.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://bme.epnwcf.com

JS:   "7".padStart(3, "0")
来源：http://wek.aibaodan.cn

TS:   "7".padStart(3, "0")
来源：http://kmc.tianlin.xyz

Java: String.format("%03d", 7)
来源：http://ymv.yj20258888.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://usi.ydjk.org.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://tan.feifeiyinyue.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://vdc.yvedp.cn

[E11] 反转字符串
来源：http://ynn.epnwcf.com

Py:   s[::-1]
来源：http://tpo.fanxiaobao.xyz

PHP:  strrev($s);
来源：http://vjg.andypj.xyz

JS:   [...s].reverse().join("")
来源：http://com.jinqigfzy.top

TS:   [...s].reverse().join("")
来源：http://zzd.bbcook.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://tpx.yj20258888.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://vwy.smart0.xyz

Ruby: s.reverse
来源：http://qln.zdbjq.cn

C#:   new string(s.Reverse().ToArray())
来源：http://hle.yuxming.cn

[E12] 统计某字符出现次数
来源：http://xpw.cucudq.cn

Py:   s.count("a")
来源：http://mgc.hnxiangtu.top

PHP:  substr_count($s, "a");
来源：http://kue.cheryme.top

JS:   s.split("a").length - 1
来源：http://bwe.guowangkeji.top

TS:   s.split("a").length - 1
来源：http://gmp.wangshuangyany.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://lhv.ydjk.org.cn

Go:   strings.Count(s, "a")
来源：http://euz.shanyushiyangkeji.top

Ruby: s.count("a")
来源：http://mku.zhaomingkeji.xyz

C#:   s.Count(c => c == 'a')
来源：http://nir.316326.xyz

[E13] 逐字符遍历
来源：http://iux.jinghuilouyu.cn

Py:   for ch in s: print(ch)
来源：http://bzu.xylfe.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://sro.sjlbkw.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://miy.jinqigufen.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://wgq.gaohongyu789.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://emd.mhx1999.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://bhv.ydjk.org.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://ofd.andypj.xyz

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://rok.aizwys.cn

[E14] URL 编码与 Base64
来源：http://fgn.guannengcc.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://mxl.wangshuangyany.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://waw.vqdsnc.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://wje.fanxiaobao.xyz

TS:   encodeURIComponent(s);  btoa(s)
来源：http://fon.dashuyun.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://lht.yanxiufei.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://zne.cdnleiting.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://rss.gogol.net.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://swx.redwolf501.top

[E15] HTML 转义 / 反转义
来源：http://phf.dianchejie.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://ztu.sxryk.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://nsn.uphjek.com

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://mej.andypj.xyz

TS:   // 同上，务必做 XSS 过滤
来源：http://rqq.jiagoushi.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://iqn.vqdsnc.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://tzt.yongpay.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://ljm.cqqwz.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://bms.feifeiyinyue.top

[E16] 数字千分位
来源：http://zuc.yuanzhike.top

Py:   f"{1234567:,}"
来源：http://fsz.nanxuanxn.top

PHP:  number_format(1234567);
来源：http://uqg.zhijiandao.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://fmb.gzhubu.top

TS:   (1234567).toLocaleString("en-US")
来源：http://ony.hammf.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://zxj.hcnkem.com

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://auc.cdnleiting.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://cbj.zhiwuduotai.top

C#:   1234567.ToString("N0")
来源：http://zoi.dashuyun.cn

[E17] 首字母大写
来源：http://hug.cheryme.top


<!-- 参考信息 -->