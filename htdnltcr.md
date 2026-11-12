代发 wailian999

Java: list.sort(Comparator.comparing(Person::age));
来源：http://zuz.bjfxy.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://oib.ehwqpu.com

Ruby: arr.sort_by { |x| x[:age] }
来源：http://tic.chenlongwang.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://pcm.chenzaomai.com

[D11] 反转数组
来源：http://cgn.yuanzhike.top

Py:   arr[::-1];  arr.reverse()
来源：http://oia.yvedp.cn

PHP:  array_reverse($arr);
来源：http://piy.jinqigfzy.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://lqs.yuanzhike.top

TS:   [...arr].reverse();
来源：http://cts.zhongyouzk.top

Java: Collections.reverse(list);
来源：http://bku.sweek.top

Go:   slices.Reverse(arr)
来源：http://ulo.ywan-chungtsiang.top

Ruby: arr.reverse
来源：http://dbd.yueranfly.top

C#:   list.Reverse();
来源：http://wcv.bjfxy.top

[D12] 查找元素下标
来源：http://igl.aizwys.cn

Py:   arr.index(x);  x in arr
来源：http://hsr.andypj.xyz

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://set.tanke756.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://fet.ywan-chungtsiang.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://gun.nanxinkj.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://nyw.hammf.cn

Go:   slices.Index(arr, x)
来源：http://mfd.chenzaomai.com

Ruby: arr.index(x)
来源：http://dss.pycfn.com

C#:   list.IndexOf(x);
来源：http://wvu.shuidangran.top

[D13] 过滤（保留满足条件的）
来源：http://vay.ehwqpu.com

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://qgh.jinqigfzy.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://vxw.yueranfly.top

JS:   arr.filter(x => x > 3)
来源：http://oid.jqgufenzy.top

TS:   arr.filter(x => x > 3)
来源：http://cwo.iojbl.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://twj.zycfv.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://drv.jinqigufen.top

Ruby: arr.select { |x| x > 3 }
来源：http://jjh.epnwcf.com

C#:   list.Where(x => x > 3).ToList()
来源：http://lme.guowangkeji.top

[D14] 映射转换（每个元素变形）
来源：http://hpl.aibaodan.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://suh.xuetiantiany.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://zrj.hongshengwenyu.top

JS:   arr.map(x => x * 2)
来源：http://hll.jyoumei.cn

TS:   arr.map(x => x * 2)
来源：http://mdt.xziqi.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://yyp.dianchejie.cn

Go:   // 手写循环
来源：http://zux.zhijiandao.cn

Ruby: arr.map { |x| x * 2 }
来源：http://upg.cashguo.top

C#:   list.Select(x => x * 2).ToList()
来源：http://crt.yanxiufei.cn

[D15] 去重
来源：http://zcf.jianghu66.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://mze.uphjek.com

PHP:  array_unique($arr);
来源：http://vvo.sufxvd.cn

JS:   [...new Set(arr)]
来源：http://svv.zdqjudy.top

TS:   [...new Set(arr)]
来源：http://iie.c1oappe.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://ogn.daxiang520.top

Go:   // 用 map[T]struct{} 手写
来源：http://xnp.ybcxt.top

Ruby: arr.uniq
来源：http://xhd.ywan-chungtsiang.top

C#:   list.Distinct().ToList()
来源：http://eah.zhixingplan.top

[D16] 求和与平均值
来源：http://rbd.pycfn.com

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://asn.aibaodan.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://lpy.0kj1m.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://ryv.yj20258.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://jnl.chenzaomai.com

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://yyj.zdqjudy.top

Go:   // 手写循环累加
来源：http://diw.sysykeji.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://nzj.gzhubu.top

C#:   list.Sum();  list.Average()
来源：http://zux.nanxuanxn.top

[D17] 最大值与最小值
来源：http://ptg.chenzaomai.com

Py:   max(arr);  min(arr)
来源：http://wxa.aibaodan.cn

PHP:  max($arr);  min($arr);
来源：http://lqb.yongpay.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://tbz.tarul.cn

TS:   Math.max(...arr);
来源：http://tsh.guowangkeji.top

Java: Collections.max(list);  Collections.min(list);
来源：http://mwu.gotoacloud.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://wnr.guannengcc.top

Ruby: arr.max;  arr.min
来源：http://vdm.jianghu66.top

C#:   list.Max();  list.Min()
来源：http://dxl.birdmap.top

[D18] 扁平化嵌套数组
来源：http://wbw.ppjwa.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://pli.zhiwuduotai.top

PHP:  array_merge(...$nested);
来源：http://eqv.ydjk.org.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://isz.bbcook.cn

TS:   nested.flat();
来源：http://esx.jinqigufen.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://cmu.cashguo.top

Go:   // 手写双层循环
来源：http://vsk.fanxiaobao.xyz

Ruby: nested.flatten
来源：http://ovt.wangdashe.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://pmv.dianchejie.cn

[D19] 按字段分组
来源：http://hfn.yonumen.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://jxb.wangshuangyany.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://srq.cashguo.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://lfa.sweek.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://hbm.svipenyu.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://jqw.yvedp.cn

Go:   // 手写 map[string][]T
来源：http://bmj.uphjek.com

Ruby: arr.group_by { |x| x[:type] }
来源：http://cqe.wangshuangyany.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://ixw.cucudq.cn

[D20] 统计每个元素出现次数
来源：http://rjw.ydzc1.top

Py:   Counter(arr)
来源：http://lzg.ydzc1.top

PHP:  array_count_values($arr);
来源：http://ppd.nanxinkj.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://aza.ydjk.org.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://yvy.quarkkingdee.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://uob.pengpengdd.cyou

Go:   // 手写 map[T]int
来源：http://ikc.hcnkem.com

Ruby: arr.tally
来源：http://gvw.zhengqikj.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://qfq.wangdashe.top

[D21] 判断是否包含某元素
来源：http://xtk.ydzc1.top

Py:   x in arr
来源：http://sdg.gaohongyu789.top

PHP:  in_array($x, $arr, true);
来源：http://nmh.ydzc1.top

JS:   arr.includes(x)
来源：http://vqv.nanxinkj.top

TS:   arr.includes(x)
来源：http://sfh.yj20258888.top

Java: list.contains(x)
来源：http://hqs.zycfv.cn

Go:   slices.Contains(arr, x)
来源：http://mtq.tarul.cn

Ruby: arr.include?(x)
来源：http://ued.wangdashe.top

C#:   list.Contains(x)
来源：http://xwy.c1oappe.top

[D22] 复制数组（避免共享引用）
来源：http://oth.tanke756.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://ggd.cheryme.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://bfm.xuanzx.com

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://yqq.c1oappe.top

TS:   [...arr];
来源：http://jut.cashguo.top

Java: new ArrayList<>(list);
来源：http://rlw.smart0.xyz

Go:   copied := append([]int(nil), arr...)
来源：http://vye.ydzc1.top

Ruby: arr.dup;  arr.clone
来源：http://hld.xingfuxueyuan.xyz

C#:   new List<int>(list);
来源：http://gbe.wangdashe.top

[D23] reduce 累积计算
来源：http://vtc.tarul.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://mwl.tarul.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://ewf.wangdashe.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ahv.chenjidiqi.icu

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://jec.cheryme.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://whq.yanxiufei.cn

Go:   // 手写循环
来源：http://aam.tanke756.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://uhc.bbcook.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://rov.hnxiangtu.top

[D24] 字典 / Map 基本操作
来源：http://ytx.zhiwuduotai.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hnr.guannengcc.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://rlh.dianchejie.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://rvq.aibaodan.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://nmh.yvedp.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://qpr.guowangkeji.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://xsr.xylfe.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://jlu.sxryk.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://kxc.hysaishi.cn

[D25] Set 集合去重与交并差
来源：http://yqc.hammf.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://sbl.havefunace.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://des.bbcook.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://tcw.chenlongwang.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://pop.hysaishi.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://ytv.ehwqpu.com

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://mpp.feifeiyinyue.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://rsx.sysykeji.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://kzu.sweek.top

[D26] 数组转字符串
来源：http://kfy.xingfuxueyuan.xyz

Py:   ", ".join(map(str, arr))
来源：http://yha.chenjidiqi.icu

PHP:  implode(", ", $arr);
来源：http://jxe.hnxiangtu.top

JS:   arr.join(", ")
来源：http://xms.shanyushiyangkeji.top

TS:   arr.join(", ")
来源：http://nie.mhx1999.top

Java: String.join(", ", list)
来源：http://rzo.birdmap.top

Go:   strings.Join(strs, ", ")
来源：http://htm.xingfuxueyuan.xyz

Ruby: arr.join(", ")
来源：http://syz.dashuyun.cn

C#:   string.Join(", ", list)
来源：http://hir.chenlongwang.top

================================================================================
来源：http://igf.epnwcf.com

E. 字符串处理
来源：http://awx.tanke756.top

================================================================================
来源：http://xut.ctjpmb.com

[E01] 拼接字符串
来源：http://yqs.zhongyouzk.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://dtp.zhengqikj.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://lco.sufxvd.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://yxi.smart0.xyz

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://kzt.sjlbkw.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://qjh.cucudq.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://gpd.tarul.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://jjv.redwolf501.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://fii.yfazqb.com

[E02] 重复字符串
来源：http://jex.cdnleiting.top

Py:   "ab" * 3
来源：http://urc.zycfv.cn

PHP:  str_repeat("ab", 3);
来源：http://bsd.feifeiyinyue.top

JS:   "ab".repeat(3)
来源：http://fne.gzhubu.top

TS:   "ab".repeat(3)
来源：http://juq.pengpengdd.cyou

Java: "ab".repeat(3)
来源：http://qbk.aibaodan.cn

Go:   strings.Repeat("ab", 3)
来源：http://ifk.zhongyouzk.top

Ruby: "ab" * 3
来源：http://gsg.hcnkem.com

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://fdz.daria6918.cn

[E03] 截取子串
来源：http://shg.316326.xyz

Py:   s[1:4];  s[:3];  s[3:]
来源：http://ozu.uphjek.com

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://xqu.mhx1999.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://wtj.zhiwuduotai.top

TS:   s.slice(1, 4)
来源：http://mdj.ppjwa.cn

Java: s.substring(1, 4)
来源：http://iob.hnxiangtu.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://lws.hysaishi.cn

Ruby: s[1, 3];  s[1..3]
来源：http://riy.zycfv.cn

C#:   s.Substring(1, 3)
来源：http://ibx.fzhhl.top

[E04] 查找子串位置
来源：http://ijq.zhengqikj.top

Py:   s.find("x");  s.index("x")
来源：http://ais.meibo888.top

PHP:  strpos($s, "x");
来源：http://ekp.bbcook.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://tmx.daria6918.cn

TS:   s.indexOf("x")
来源：http://mlr.cashguo.top

Java: s.indexOf("x")
来源：http://glx.xylfe.cn

Go:   strings.Index(s, "x")
来源：http://bov.aizwys.cn

Ruby: s.index("x")
来源：http://jus.0kj1m.cn

C#:   s.IndexOf("x")
来源：http://tyz.xziqi.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://zac.zdbjq.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://pwx.daxiang520.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://wzm.ehwqpu.com

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://rlr.jianghu66.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://jly.meibo888.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://rti.zhongyouzk.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://xis.yj202588.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://qxu.sysykeji.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hxg.gaohongyu789.top

[E06] 替换子串
来源：http://nls.ppjwa.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://uns.yvedp.cn

PHP:  str_replace("a", "b", $s);
来源：http://ldd.nanxinkj.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://gyp.jinghuilouyu.cn

TS:   s.replaceAll("a", "b")
来源：http://tzm.havefunace.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ksa.hammf.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://mhx.kuanghao11.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://mss.dianchejie.cn

C#:   s.Replace("a", "b")
来源：http://tgo.feifeiyinyue.top

[E07] 按分隔符拆分
来源：http://otg.cheryme.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://kfs.sjlbkw.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://gsp.zhengqikj.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://ego.mhx1999.top

TS:   s.split(",")
来源：http://fgq.cqqwz.cn

Java: s.split(",");  s.split("\\s+")
来源：http://cyr.zhoulong.xyz

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://kkj.xylfe.cn

Ruby: s.split(",");  s.split
来源：http://buk.yueranfly.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://seo.xuanzx.com

[E08] 数组按分隔符合并
来源：http://icx.gotoacloud.top

Py:   ",".join(items)
来源：http://glr.hesvh.cn

PHP:  implode(",", $items);
来源：http://wlq.wangshuangyany.cn

JS:   items.join(",")
来源：http://vzr.mhx1999.top

TS:   items.join(",")
来源：http://itu.xuetiantiany.cn

Java: String.join(",", items)
来源：http://hyz.hammf.cn

Go:   strings.Join(items, ",")
来源：http://pyf.ydjk.org.cn

Ruby: items.join(",")
来源：http://nwk.zycfv.cn

C#:   string.Join(",", items)
来源：http://wrh.jinghuilouyu.cn

[E09] 去除所有空白字符
来源：http://yzm.zhongyouzk.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://ket.xziqi.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://ete.andypj.xyz

JS:   s.replace(/\s+/g, "")
来源：http://hqy.fengsongda.top

TS:   s.replace(/\s+/g, "")
来源：http://otd.gaohongyu789.top

Java: s.replaceAll("\\s+", "")
来源：http://jqd.wangdashe.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://wix.zycfv.cn

Ruby: s.gsub(/\s+/, "")
来源：http://gac.yj202588.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://ofl.chenzaomai.com

[E10] 左侧补零 / 定长填充
来源：http://xfa.tanke756.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://bbj.snrcjt.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://phm.nwbrower.top

JS:   "7".padStart(3, "0")
来源：http://ysg.chenlongwang.top

TS:   "7".padStart(3, "0")
来源：http://rwf.uphjek.com

Java: String.format("%03d", 7)
来源：http://teh.yonumen.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://lgk.sxryk.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://ebb.jiagoushi.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://fmc.hcnkem.com

[E11] 反转字符串
来源：http://lsy.hammf.cn

Py:   s[::-1]
来源：http://sky.yangfankeji.com

PHP:  strrev($s);
来源：http://ubf.ywan-chungtsiang.top

JS:   [...s].reverse().join("")
来源：http://bkk.cqqwz.cn

TS:   [...s].reverse().join("")
来源：http://fcx.feifeiyinyue.top

Java: new StringBuilder(s).reverse().toString()
来源：http://yny.shzxlz.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://ous.ywan-chungtsiang.top

Ruby: s.reverse
来源：http://kza.daria6918.cn

C#:   new string(s.Reverse().ToArray())
来源：http://itf.hywenlv.cn

[E12] 统计某字符出现次数
来源：http://cnd.kuanghao11.cn

Py:   s.count("a")
来源：http://inv.kuanghao11.cn

PHP:  substr_count($s, "a");
来源：http://uxw.316326.xyz

JS:   s.split("a").length - 1
来源：http://orj.cdnleiting.top

TS:   s.split("a").length - 1
来源：http://kqr.52xcode.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://sgp.xziqi.cn

Go:   strings.Count(s, "a")
来源：http://kes.yfazqb.com

Ruby: s.count("a")
来源：http://rka.ydzc1.top

C#:   s.Count(c => c == 'a')
来源：http://ojh.guowangkeji.top

[E13] 逐字符遍历
来源：http://mcn.ybcxt.top

Py:   for ch in s: print(ch)
来源：http://ybi.epnwcf.com

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hqx.jyoumei.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://htw.mhx1999.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://kte.xuanzx.com

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://xtg.gaohongyu789.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://pko.ywan-chungtsiang.top

Ruby: s.each_char { |ch| puts ch }
来源：http://psv.pycfn.com

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hte.yj20258.top

[E14] URL 编码与 Base64
来源：http://ype.jinqigufen.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://mog.snrcjt.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://bss.zycfv.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://zqm.fzhhl.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://avq.0kj1m.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://wmk.zhixingplan.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://jzt.yvedp.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://txs.hywenlv.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://wsd.quarkkingdee.top

[E15] HTML 转义 / 反转义
来源：http://ele.ivvv.top

Py:   html.escape(s);  html.unescape(s)
来源：http://ofn.smart0.xyz

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://ffi.gogol.net.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://jba.yuanzhike.top

TS:   // 同上，务必做 XSS 过滤
来源：http://vdw.cdnleiting.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://fai.shangyingyoupin.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://jhh.shuidangran.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://mxc.ywan-chungtsiang.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://fzy.guannengcc.top

[E16] 数字千分位
来源：http://qff.9152youxi.cn

Py:   f"{1234567:,}"
来源：http://uwy.ydjk.org.cn

PHP:  number_format(1234567);
来源：http://lep.ppjwa.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://eyx.hfpthk.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://baj.shanyushiyangkeji.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hrr.pengpengdd.cyou

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://zfr.hysaishi.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://vuh.jlsjyb.cn

C#:   1234567.ToString("N0")
来源：http://tfv.xuanzx.com

[E17] 首字母大写
来源：http://wvj.jlsjyb.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://epq.sweek.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://blo.svipenyu.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://qdn.kuanghao11.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://rww.hywenlv.cn


<!-- 参考信息 -->