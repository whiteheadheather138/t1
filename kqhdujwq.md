代发 wailian999

TS:   arr.slice(1, 4);
来源：http://geo.daria6918.cn

Java: list.subList(1, 4);
来源：http://dhx.xuanzx.com

Go:   arr[1:4]
来源：http://ytm.yangfankeji.com

Ruby: arr[1, 3]
来源：http://pkh.wangdashe.top

C#:   list.GetRange(1, 3);
来源：http://uhe.cqqwz.cn

[D08] 合并两个数组
来源：http://ffw.sysykeji.top

Py:   a + b;  a.extend(b)
来源：http://uxk.zhongyouzk.top

PHP:  array_merge($a, $b);
来源：http://jsv.shangyingyoupin.top

JS:   [...a, ...b];  a.concat(b);
来源：http://fbq.zycfv.cn

TS:   [...a, ...b];
来源：http://ojn.jqgufenzy.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://kea.meibo888.top

Go:   append(a, b...)
来源：http://deu.iojbl.cn

Ruby: a + b;  a.concat(b)
来源：http://qnr.yfazqb.com

C#:   a.Concat(b).ToList()
来源：http://cal.ydjk.org.cn

[D09] 排序（升序）
来源：http://fml.zhijiandao.cn

Py:   sorted(arr);  arr.sort()
来源：http://cel.fehbvm.com

PHP:  sort($arr);
来源：http://wve.zhaomingkeji.xyz

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://tdv.shanyushiyangkeji.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://waq.yj20258888.top

Java: Collections.sort(list);  list.sort(null);
来源：http://ywo.zycfv.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://ftp.fanxiaobao.xyz

Ruby: arr.sort
来源：http://vtl.havefunace.top

C#:   list.Sort();
来源：http://bbj.hammf.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://wgi.tarul.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://eqc.gzhubu.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wue.xuanzx.com

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://nlf.birdmap.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://gqq.jinqigufen.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://wyk.jinyuanbaomall.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://uap.tarul.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://pji.ybcxt.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://dnd.shuidangran.top

[D11] 反转数组
来源：http://osv.sysykeji.top

Py:   arr[::-1];  arr.reverse()
来源：http://lux.daria6918.cn

PHP:  array_reverse($arr);
来源：http://jry.epnwcf.com

JS:   [...arr].reverse();  arr.toReversed()
来源：http://jay.yj20258888.top

TS:   [...arr].reverse();
来源：http://dht.daxiang520.top

Java: Collections.reverse(list);
来源：http://hye.havefunace.top

Go:   slices.Reverse(arr)
来源：http://vyg.havefunace.top

Ruby: arr.reverse
来源：http://uxw.fktsv.cn

C#:   list.Reverse();
来源：http://cmi.hywenlv.cn

[D12] 查找元素下标
来源：http://pwd.yanxiufei.cn

Py:   arr.index(x);  x in arr
来源：http://xog.wangdashe.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://svy.nanxinkj.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://lty.meibo888.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://lsb.xziqi.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://ixf.52xcode.cn

Go:   slices.Index(arr, x)
来源：http://nkc.havefunace.top

Ruby: arr.index(x)
来源：http://uqc.yuxming.cn

C#:   list.IndexOf(x);
来源：http://yqp.yfazqb.com

[D13] 过滤（保留满足条件的）
来源：http://tlt.hammf.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://vmj.ydzc1.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://uxo.hammf.cn

JS:   arr.filter(x => x > 3)
来源：http://mud.zhongyouzk.top

TS:   arr.filter(x => x > 3)
来源：http://zai.9152youxi.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://bxc.zhongyouzk.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://vae.hfpthk.cn

Ruby: arr.select { |x| x > 3 }
来源：http://ccz.nanxuanxn.top

C#:   list.Where(x => x > 3).ToList()
来源：http://ggl.zdbjq.cn

[D14] 映射转换（每个元素变形）
来源：http://nol.xziqi.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://vne.jinqigufen.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://fal.fengsongda.top

JS:   arr.map(x => x * 2)
来源：http://chy.gzhubu.top

TS:   arr.map(x => x * 2)
来源：http://ymq.fanxiaobao.xyz

Java: list.stream().map(x -> x * 2).toList()
来源：http://dvr.xingfuxueyuan.xyz

Go:   // 手写循环
来源：http://gbm.yj20258888.top

Ruby: arr.map { |x| x * 2 }
来源：http://oue.fanxiaobao.xyz

C#:   list.Select(x => x * 2).ToList()
来源：http://jra.yfazqb.com

[D15] 去重
来源：http://bjx.chenzaomai.com

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://nrm.daxiang520.top

PHP:  array_unique($arr);
来源：http://npu.hcnkem.com

JS:   [...new Set(arr)]
来源：http://csz.vehdjk.com

TS:   [...new Set(arr)]
来源：http://rxe.hysaishi.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://lya.yj20258.top

Go:   // 用 map[T]struct{} 手写
来源：http://dbn.zhiwuduotai.top

Ruby: arr.uniq
来源：http://uvf.aibaodan.cn

C#:   list.Distinct().ToList()
来源：http://zoz.nanxinkj.top

[D16] 求和与平均值
来源：http://eja.redwolf501.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://tee.chenzaomai.com

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://eri.xziqi.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://sik.gzhubu.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://ujy.xingfuxueyuan.xyz

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://qja.shanyushiyangtech.top

Go:   // 手写循环累加
来源：http://hdi.iojbl.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://dvo.zhongyouzk.top

C#:   list.Sum();  list.Average()
来源：http://qxe.dashuyun.cn

[D17] 最大值与最小值
来源：http://cvk.shanyushiyangtech.top

Py:   max(arr);  min(arr)
来源：http://yty.zhongyouzk.top

PHP:  max($arr);  min($arr);
来源：http://htv.shanyushiyangtech.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://bwq.uphjek.com

TS:   Math.max(...arr);
来源：http://uvc.gaohongyu789.top

Java: Collections.max(list);  Collections.min(list);
来源：http://fsy.zhaomingkeji.xyz

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://dui.smart0.xyz

Ruby: arr.max;  arr.min
来源：http://jug.hywenlv.cn

C#:   list.Max();  list.Min()
来源：http://gsu.jlsjyb.cn

[D18] 扁平化嵌套数组
来源：http://jbr.redwolf501.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hte.andypj.xyz

PHP:  array_merge(...$nested);
来源：http://jfe.gogol.net.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://sih.shanyushiyangtech.top

TS:   nested.flat();
来源：http://lre.9152youxi.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://nzu.jqgfzy.top

Go:   // 手写双层循环
来源：http://scg.snrcjt.cn

Ruby: nested.flatten
来源：http://mur.fzhhl.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://mse.yuxming.cn

[D19] 按字段分组
来源：http://eky.hesvh.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://nfn.chenzaomai.com

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://lqq.tanke756.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://clx.ydzc1.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://uci.tarul.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://zdv.yongpay.top

Go:   // 手写 map[string][]T
来源：http://gma.yj20258.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://hsq.cheryme.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://ice.shuidangran.top

[D20] 统计每个元素出现次数
来源：http://tbu.xuetiantiany.cn

Py:   Counter(arr)
来源：http://pdg.chenjidiqi.icu

PHP:  array_count_values($arr);
来源：http://eci.hammf.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://waa.iojbl.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://czj.jiagoushi.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://xfy.zycfv.cn

Go:   // 手写 map[T]int
来源：http://wwu.daria6918.cn

Ruby: arr.tally
来源：http://uyb.birdmap.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://jnf.bjfxy.top

[D21] 判断是否包含某元素
来源：http://bkn.52xcode.cn

Py:   x in arr
来源：http://hts.smart0.xyz

PHP:  in_array($x, $arr, true);
来源：http://gdj.jyoumei.cn

JS:   arr.includes(x)
来源：http://qxp.iojbl.cn

TS:   arr.includes(x)
来源：http://lwi.havefunace.top

Java: list.contains(x)
来源：http://uxj.ppjwa.cn

Go:   slices.Contains(arr, x)
来源：http://zzh.snrcjt.cn

Ruby: arr.include?(x)
来源：http://bag.mhx1999.top

C#:   list.Contains(x)
来源：http://nda.zhengqikj.top

[D22] 复制数组（避免共享引用）
来源：http://ieh.yanxiufei.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://vui.yangfankeji.com

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://qzp.chenjidiqi.icu

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://heq.daxiang520.top

TS:   [...arr];
来源：http://huj.nwbrower.top

Java: new ArrayList<>(list);
来源：http://onb.52xcode.cn

Go:   copied := append([]int(nil), arr...)
来源：http://mlr.hnqzz.top

Ruby: arr.dup;  arr.clone
来源：http://aew.shanyushiyangtech.top

C#:   new List<int>(list);
来源：http://own.tian-w.cn

[D23] reduce 累积计算
来源：http://uwh.cucudq.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://yal.svipenyu.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://rym.haohaochexian.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hcx.snrcjt.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://nhf.yfazqb.com

Java: list.stream().reduce(0, Integer::sum)
来源：http://uco.shangyingyoupin.top

Go:   // 手写循环
来源：http://igh.yj202588.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://vox.yanxiufei.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://wdn.uphjek.com

[D24] 字典 / Map 基本操作
来源：http://nyz.hywenlv.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://ewf.wangshuangyany.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://rqm.zhijiandao.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://bzc.hywenlv.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://euw.shangyingyoupin.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://nwa.sysykeji.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://dcf.epnwcf.com

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://uqw.cqqwz.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://sva.havefunace.top

[D25] Set 集合去重与交并差
来源：http://xtm.zhiwuduotai.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://kmf.hfpthk.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://cpt.hywenlv.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://xyp.daxiang520.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://wnw.zycfv.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://muu.zhongyouzk.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hpg.jyoumei.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://tnq.fktsv.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://svr.guannengcc.top

[D26] 数组转字符串
来源：http://udt.feifeiyinyue.top

Py:   ", ".join(map(str, arr))
来源：http://qia.daria6918.cn

PHP:  implode(", ", $arr);
来源：http://ggc.zhongyouzk.top

JS:   arr.join(", ")
来源：http://rzw.jiagoushi.top

TS:   arr.join(", ")
来源：http://fwf.quarkkingdee.top

Java: String.join(", ", list)
来源：http://jpl.hywenlv.cn

Go:   strings.Join(strs, ", ")
来源：http://vvu.gaohongyu789.top

Ruby: arr.join(", ")
来源：http://abf.yueranfly.top

C#:   string.Join(", ", list)
来源：http://gfa.ivvv.top

================================================================================
来源：http://wli.snrcjt.cn

E. 字符串处理
来源：http://bge.xziqi.cn

================================================================================
来源：http://zqx.tarul.cn

[E01] 拼接字符串
来源：http://jcm.guannengcc.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://ezn.vehdjk.com

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://noy.yj20258888.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://ysh.gogol.net.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://vsj.vqdsnc.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://vek.yangfankeji.com

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://znm.tianlin.xyz

Ruby: "a" + "b";  ["a", "b"].join
来源：http://agg.feifeiyinyue.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://uro.bjfxy.top

[E02] 重复字符串
来源：http://vxw.shanyushiyangtech.top

Py:   "ab" * 3
来源：http://ydv.fengsongda.top

PHP:  str_repeat("ab", 3);
来源：http://upk.xuanzx.com

JS:   "ab".repeat(3)
来源：http://gmv.hesvh.cn

TS:   "ab".repeat(3)
来源：http://bxz.daxiang520.top

Java: "ab".repeat(3)
来源：http://xki.zdqjudy.top

Go:   strings.Repeat("ab", 3)
来源：http://buw.smart0.xyz

Ruby: "ab" * 3
来源：http://zno.fzhhl.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://fup.jinghuilouyu.cn

[E03] 截取子串
来源：http://gij.meibo888.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://wqh.nwbrower.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://ckg.jqgufenzy.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://vpk.ivvv.top

TS:   s.slice(1, 4)
来源：http://kuh.hcnkem.com

Java: s.substring(1, 4)
来源：http://wjw.zhaomingkeji.xyz

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://nfu.ywan-chungtsiang.top

Ruby: s[1, 3];  s[1..3]
来源：http://sdr.chenjidiqi.icu

C#:   s.Substring(1, 3)
来源：http://akt.vehdjk.com

[E04] 查找子串位置
来源：http://pee.9152youxi.cn

Py:   s.find("x");  s.index("x")
来源：http://igd.wangdashe.top

PHP:  strpos($s, "x");
来源：http://ofj.hongshengwenyu.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://xby.shangyingyoupin.top

TS:   s.indexOf("x")
来源：http://jah.chenlongwang.top

Java: s.indexOf("x")
来源：http://ggr.yfazqb.com

Go:   strings.Index(s, "x")
来源：http://gbd.ybcxt.top

Ruby: s.index("x")
来源：http://gum.hongshengwenyu.top

C#:   s.IndexOf("x")
来源：http://mws.316326.xyz

[E05] 判断包含 / 前缀 / 后缀
来源：http://giw.tanke756.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://myu.yanxiufei.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://spp.tian-w.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://zyl.yongpay.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://jea.sjlbkw.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://yme.yuxming.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://qzf.havefunace.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://pic.pycfn.com

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hkt.guowangkeji.top

[E06] 替换子串
来源：http://vhb.haohaochexian.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://qzd.hammf.cn

PHP:  str_replace("a", "b", $s);
来源：http://oqx.hysaishi.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ysi.hcnkem.com

TS:   s.replaceAll("a", "b")
来源：http://bar.wangshuangyany.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://qmu.aibaodan.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://scu.birdmap.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://gkv.yfazqb.com

C#:   s.Replace("a", "b")
来源：http://paf.aibaodan.cn

[E07] 按分隔符拆分
来源：http://rbl.uphjek.com

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://trc.hammf.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://sfq.cucudq.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://uez.pengpengdd.cyou

TS:   s.split(",")
来源：http://gbz.wangshuangyany.cn

Java: s.split(",");  s.split("\\s+")
来源：http://wci.jlsjyb.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://oep.pengpengdd.cyou

Ruby: s.split(",");  s.split
来源：http://atu.pycfn.com

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://lwo.xuetiantiany.cn

[E08] 数组按分隔符合并
来源：http://pvw.nanxuanxn.top

Py:   ",".join(items)
来源：http://obd.wangshuangyany.cn

PHP:  implode(",", $items);
来源：http://zez.hywenlv.cn

JS:   items.join(",")
来源：http://fya.yvedp.cn

TS:   items.join(",")
来源：http://buq.shuidangran.top

Java: String.join(",", items)
来源：http://tyb.gzhubu.top

Go:   strings.Join(items, ",")
来源：http://amd.feifeiyinyue.top

Ruby: items.join(",")
来源：http://vkt.jianghu66.top

C#:   string.Join(",", items)
来源：http://lid.vqdsnc.cn

[E09] 去除所有空白字符
来源：http://lui.jinghuilouyu.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hed.mhx1999.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://lkl.cashguo.top

JS:   s.replace(/\s+/g, "")
来源：http://bxd.yonumen.top

TS:   s.replace(/\s+/g, "")
来源：http://jfi.shangyingyoupin.top

Java: s.replaceAll("\\s+", "")
来源：http://fks.9152youxi.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://vwh.0kj1m.cn

Ruby: s.gsub(/\s+/, "")
来源：http://jnw.ybcxt.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://rvl.vqdsnc.cn

[E10] 左侧补零 / 定长填充
来源：http://llv.hnqzz.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://lrj.ppjwa.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://gjf.quarkkingdee.top

JS:   "7".padStart(3, "0")
来源：http://drl.yuanzhike.top

TS:   "7".padStart(3, "0")
来源：http://vps.zhoulong.xyz

Java: String.format("%03d", 7)
来源：http://atu.jlsjyb.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://xxx.xinyue.icu

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://rcu.jqgfzy.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://axw.jianghu66.top

[E11] 反转字符串
来源：http://vzc.fengsongda.top

Py:   s[::-1]
来源：http://eux.uphjek.com

PHP:  strrev($s);
来源：http://ncg.zhixingplan.top

JS:   [...s].reverse().join("")
来源：http://say.yueranfly.top

TS:   [...s].reverse().join("")
来源：http://zal.jianghu66.top

Java: new StringBuilder(s).reverse().toString()
来源：http://yvu.jiagoushi.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://sow.hysaishi.cn

Ruby: s.reverse
来源：http://hat.zhaomingkeji.xyz

C#:   new string(s.Reverse().ToArray())
来源：http://wnr.yj202588.top

[E12] 统计某字符出现次数
来源：http://lmj.bjfxy.top

Py:   s.count("a")
来源：http://xqb.yanxiufei.cn

PHP:  substr_count($s, "a");
来源：http://lba.chenjidiqi.icu

JS:   s.split("a").length - 1
来源：http://ggd.xylfe.cn

TS:   s.split("a").length - 1
来源：http://ybq.svipenyu.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://tqk.tarul.cn

Go:   strings.Count(s, "a")
来源：http://fdf.yongpay.top

Ruby: s.count("a")
来源：http://tee.ivvv.top

C#:   s.Count(c => c == 'a')
来源：http://cqr.0kj1m.cn

[E13] 逐字符遍历
来源：http://txu.yuanzhike.top

Py:   for ch in s: print(ch)
来源：http://rjf.nanxuanxn.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://qpb.nwbrower.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://qgj.zhoulong.xyz

TS:   for (const ch of s) { console.log(ch); }
来源：http://vcp.fengsongda.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://ast.hnqzz.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://bhx.dianchejie.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://uvb.sweek.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://mmp.nanxinkj.top

[E14] URL 编码与 Base64
来源：http://vhk.yongpay.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://nzx.ywan-chungtsiang.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://jpc.0kj1m.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://ewd.wangdashe.top


<!-- 参考信息 -->