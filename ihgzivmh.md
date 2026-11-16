代发 wailian999

Java: list.size();
来源：http://tim.jlsjyb.cn

Go:   len(arr)
来源：http://fxr.zhongyouzk.top

Ruby: arr.length; arr.size
来源：http://mpw.feifeiyinyue.top

C#:   list.Count;
来源：http://rss.redwolf501.top

[D07] 切片 / 取子数组
来源：http://gwf.fengsongda.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://xun.gogol.net.cn

PHP:  array_slice($arr, 1, 3);
来源：http://txx.tianlin.xyz

JS:   arr.slice(1, 4);
来源：http://hqi.wangdashe.top

TS:   arr.slice(1, 4);
来源：http://jjm.guowangkeji.top

Java: list.subList(1, 4);
来源：http://jre.nanxinkj.top

Go:   arr[1:4]
来源：http://nqi.smart0.xyz

Ruby: arr[1, 3]
来源：http://jaa.uphjek.com

C#:   list.GetRange(1, 3);
来源：http://xfa.wangshuangyany.cn

[D08] 合并两个数组
来源：http://kde.zhixingplan.top

Py:   a + b;  a.extend(b)
来源：http://tsq.xinyue.icu

PHP:  array_merge($a, $b);
来源：http://mks.xylfe.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://eoy.sxryk.cn

TS:   [...a, ...b];
来源：http://ean.havefunace.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://iim.meibo888.top

Go:   append(a, b...)
来源：http://icy.aizwys.cn

Ruby: a + b;  a.concat(b)
来源：http://gvu.tian-w.cn

C#:   a.Concat(b).ToList()
来源：http://kdv.jyoumei.cn

[D09] 排序（升序）
来源：http://pus.bbcook.cn

Py:   sorted(arr);  arr.sort()
来源：http://hfc.feifeiyinyue.top

PHP:  sort($arr);
来源：http://kdo.cdnleiting.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://ivb.yueranfly.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://iyv.hywenlv.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://uag.bbcook.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://itr.jqgufenzy.top

Ruby: arr.sort
来源：http://tdm.guowangkeji.top

C#:   list.Sort();
来源：http://ozm.hnxiangtu.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://khf.yfazqb.com

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://brx.hongshengwenyu.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ikc.hnxiangtu.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://nnu.gaohongyu789.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://jhi.birdmap.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://msc.daxiang520.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://eoi.nwbrower.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://umq.chenzaomai.com

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://erl.jqgufenzy.top

[D11] 反转数组
来源：http://lag.nwbrower.top

Py:   arr[::-1];  arr.reverse()
来源：http://thd.jyoumei.cn

PHP:  array_reverse($arr);
来源：http://ruc.guannengcc.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://xyr.vqdsnc.cn

TS:   [...arr].reverse();
来源：http://cez.hammf.cn

Java: Collections.reverse(list);
来源：http://ikw.zhoulong.xyz

Go:   slices.Reverse(arr)
来源：http://zbl.pycfn.com

Ruby: arr.reverse
来源：http://mou.aizwys.cn

C#:   list.Reverse();
来源：http://bdl.jinyuanbaomall.cn

[D12] 查找元素下标
来源：http://lkp.0kj1m.cn

Py:   arr.index(x);  x in arr
来源：http://hap.tian-w.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://orf.feifeiyinyue.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://rks.52xcode.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ync.hcnkem.com

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hlr.xziqi.cn

Go:   slices.Index(arr, x)
来源：http://vro.jlsjyb.cn

Ruby: arr.index(x)
来源：http://zxt.birdmap.top

C#:   list.IndexOf(x);
来源：http://hid.yonumen.top

[D13] 过滤（保留满足条件的）
来源：http://jso.hnxiangtu.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://xsy.shangyingyoupin.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://sef.xinyue.icu

JS:   arr.filter(x => x > 3)
来源：http://gyr.iojbl.cn

TS:   arr.filter(x => x > 3)
来源：http://tbw.havefunace.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://qtv.sjlbkw.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://mvx.wangshuangyany.cn

Ruby: arr.select { |x| x > 3 }
来源：http://fgi.aizwys.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://kqh.shzxlz.cn

[D14] 映射转换（每个元素变形）
来源：http://gih.birdmap.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://abd.sjlbkw.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hsn.wangdashe.top

JS:   arr.map(x => x * 2)
来源：http://zvm.yvedp.cn

TS:   arr.map(x => x * 2)
来源：http://zms.shuidangran.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://izn.hysaishi.cn

Go:   // 手写循环
来源：http://bwu.gogol.net.cn

Ruby: arr.map { |x| x * 2 }
来源：http://lzo.cashguo.top

C#:   list.Select(x => x * 2).ToList()
来源：http://wje.nwbrower.top

[D15] 去重
来源：http://svx.hfpthk.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://sxi.hnqzz.top

PHP:  array_unique($arr);
来源：http://kzx.52xcode.cn

JS:   [...new Set(arr)]
来源：http://jxs.zdbjq.cn

TS:   [...new Set(arr)]
来源：http://vfh.yj20258.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://ccp.ctjpmb.com

Go:   // 用 map[T]struct{} 手写
来源：http://ssg.sxryk.cn

Ruby: arr.uniq
来源：http://zwu.epnwcf.com

C#:   list.Distinct().ToList()
来源：http://xli.yonumen.top

[D16] 求和与平均值
来源：http://kin.zhengqikj.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://myx.sweek.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://uzu.cqqwz.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://ddf.xinyue.icu

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://yga.fehbvm.com

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://sek.yuxming.cn

Go:   // 手写循环累加
来源：http://qmj.bjfxy.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://mug.ctjpmb.com

C#:   list.Sum();  list.Average()
来源：http://egu.9152youxi.cn

[D17] 最大值与最小值
来源：http://wcy.cqqwz.cn

Py:   max(arr);  min(arr)
来源：http://mwn.vehdjk.com

PHP:  max($arr);  min($arr);
来源：http://vbw.meibo888.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://pio.zhengqikj.top

TS:   Math.max(...arr);
来源：http://wyx.yangfankeji.com

Java: Collections.max(list);  Collections.min(list);
来源：http://icn.sufxvd.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://qbc.daxiang520.top

Ruby: arr.max;  arr.min
来源：http://anv.aizwys.cn

C#:   list.Max();  list.Min()
来源：http://ioe.zdbjq.cn

[D18] 扁平化嵌套数组
来源：http://ibo.daria6918.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://mvc.xylfe.cn

PHP:  array_merge(...$nested);
来源：http://drs.hongshengwenyu.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://sys.ywan-chungtsiang.top

TS:   nested.flat();
来源：http://svo.cdnleiting.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://ucf.shzxlz.cn

Go:   // 手写双层循环
来源：http://qbe.shanyushiyangtech.top

Ruby: nested.flatten
来源：http://kej.jqgufenzy.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://jhn.fehbvm.com

[D19] 按字段分组
来源：http://sxk.ywan-chungtsiang.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://jph.hnqzz.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://ddu.ctjpmb.com

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://off.havefunace.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://lzv.xziqi.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://ztb.bjfxy.top

Go:   // 手写 map[string][]T
来源：http://wyv.yj202588.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://ssg.jianghu66.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://ohg.fanxiaobao.xyz

[D20] 统计每个元素出现次数
来源：http://fxu.haohaochexian.top

Py:   Counter(arr)
来源：http://haj.yj20258.top

PHP:  array_count_values($arr);
来源：http://fls.nanxuanxn.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://vcn.ydjk.org.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://jul.gaohongyu789.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://wsc.pengpengdd.cyou

Go:   // 手写 map[T]int
来源：http://dmg.redwolf501.top

Ruby: arr.tally
来源：http://wpk.ywan-chungtsiang.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://fss.cashguo.top

[D21] 判断是否包含某元素
来源：http://cag.zdbjq.cn

Py:   x in arr
来源：http://jwj.cucudq.cn

PHP:  in_array($x, $arr, true);
来源：http://buk.zhongyouzk.top

JS:   arr.includes(x)
来源：http://wue.xuanzx.com

TS:   arr.includes(x)
来源：http://lig.snrcjt.cn

Java: list.contains(x)
来源：http://kuw.xylfe.cn

Go:   slices.Contains(arr, x)
来源：http://vwr.jianghu66.top

Ruby: arr.include?(x)
来源：http://nrn.fktsv.cn

C#:   list.Contains(x)
来源：http://gip.guowangkeji.top

[D22] 复制数组（避免共享引用）
来源：http://xbt.tianlin.xyz

Py:   arr.copy();  arr[:];  list(arr)
来源：http://buf.xingfuxueyuan.xyz

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://qks.wangdashe.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://con.aibaodan.cn

TS:   [...arr];
来源：http://jpp.guowangkeji.top

Java: new ArrayList<>(list);
来源：http://gow.xziqi.cn

Go:   copied := append([]int(nil), arr...)
来源：http://lub.wangdashe.top

Ruby: arr.dup;  arr.clone
来源：http://boj.jqgufenzy.top

C#:   new List<int>(list);
来源：http://wce.jqgfzy.top

[D23] reduce 累积计算
来源：http://zjc.svipenyu.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://xbl.sufxvd.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://uil.quarkkingdee.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://nvt.ybcxt.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://lsf.yuxming.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://ckj.xinyue.icu

Go:   // 手写循环
来源：http://jse.fzhhl.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://zml.haohaochexian.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://byx.redwolf501.top

[D24] 字典 / Map 基本操作
来源：http://oay.52xcode.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://fax.haohaochexian.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://lmk.tanke756.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://cpl.bjfxy.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://mic.meibo888.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://zrz.zhongyouzk.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://mkh.dianchejie.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://pnp.vqdsnc.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://pns.ydjk.org.cn

[D25] Set 集合去重与交并差
来源：http://bwv.hcnkem.com

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://unr.yonumen.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://oeu.aizwys.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://lns.andypj.xyz

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://fii.yueranfly.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://qmp.c1oappe.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://gwg.jinyuanbaomall.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://wzx.ydjk.org.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://azd.ppjwa.cn

[D26] 数组转字符串
来源：http://nny.sweek.top

Py:   ", ".join(map(str, arr))
来源：http://fok.yangfankeji.com

PHP:  implode(", ", $arr);
来源：http://ynw.sysykeji.top

JS:   arr.join(", ")
来源：http://vjk.tian-w.cn

TS:   arr.join(", ")
来源：http://rxp.pengpengdd.cyou

Java: String.join(", ", list)
来源：http://ome.fanxiaobao.xyz

Go:   strings.Join(strs, ", ")
来源：http://mwi.jinghuilouyu.cn

Ruby: arr.join(", ")
来源：http://ybz.redwolf501.top

C#:   string.Join(", ", list)
来源：http://nrb.ybcxt.top

================================================================================
来源：http://scm.cqqwz.cn

E. 字符串处理
来源：http://ldo.zycfv.cn

================================================================================
来源：http://swv.jianghu66.top

[E01] 拼接字符串
来源：http://hpe.cashguo.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://oas.yanxiufei.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://axy.yongpay.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://yts.daxiang520.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://nsl.sufxvd.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://xne.nanxinkj.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://isf.shanyushiyangtech.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://spp.yuxming.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://axc.daria6918.cn

[E02] 重复字符串
来源：http://mmu.haohaochexian.top

Py:   "ab" * 3
来源：http://xpd.havefunace.top

PHP:  str_repeat("ab", 3);
来源：http://imr.jinyuanbaomall.cn

JS:   "ab".repeat(3)
来源：http://jnt.feifeiyinyue.top

TS:   "ab".repeat(3)
来源：http://sqn.daxiang520.top

Java: "ab".repeat(3)
来源：http://lsn.jinghuilouyu.cn

Go:   strings.Repeat("ab", 3)
来源：http://oxp.gzhubu.top

Ruby: "ab" * 3
来源：http://pob.fzhhl.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://rjj.fengsongda.top

[E03] 截取子串
来源：http://ynr.cucudq.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://zit.fzhhl.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://eaq.shanyushiyangkeji.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://dir.jinghuilouyu.cn

TS:   s.slice(1, 4)
来源：http://zfg.guowangkeji.top

Java: s.substring(1, 4)
来源：http://vty.xinyue.icu

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://ayx.tian-w.cn

Ruby: s[1, 3];  s[1..3]
来源：http://jbm.pengpengdd.cyou

C#:   s.Substring(1, 3)
来源：http://mxs.fzhhl.top

[E04] 查找子串位置
来源：http://xxi.hammf.cn

Py:   s.find("x");  s.index("x")
来源：http://bsg.sweek.top

PHP:  strpos($s, "x");
来源：http://quy.ydzc1.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://wpe.c1oappe.top

TS:   s.indexOf("x")
来源：http://ynd.guannengcc.top

Java: s.indexOf("x")
来源：http://sso.uphjek.com

Go:   strings.Index(s, "x")
来源：http://til.yvedp.cn

Ruby: s.index("x")
来源：http://nnb.ybcxt.top

C#:   s.IndexOf("x")
来源：http://kjc.xingfuxueyuan.xyz

[E05] 判断包含 / 前缀 / 后缀
来源：http://mpc.zhengqikj.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://gtc.tian-w.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://fth.ppjwa.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://vwy.quarkkingdee.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://elk.hcnkem.com

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://xja.ybcxt.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://usm.yj20258.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://kxm.yueranfly.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://aol.pengpengdd.cyou

[E06] 替换子串
来源：http://fqd.ywan-chungtsiang.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://kmt.zhongyouzk.top

PHP:  str_replace("a", "b", $s);
来源：http://tcb.wangdashe.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hxx.aibaodan.cn

TS:   s.replaceAll("a", "b")
来源：http://kyw.zhoulong.xyz

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://dmg.yvedp.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://qlz.sxryk.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://ipb.zhaomingkeji.xyz

C#:   s.Replace("a", "b")
来源：http://mra.yanxiufei.cn

[E07] 按分隔符拆分
来源：http://ggi.nanxuanxn.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://fwy.zhengqikj.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://cdt.yanxiufei.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://nsj.c1oappe.top

TS:   s.split(",")
来源：http://rej.hfpthk.cn

Java: s.split(",");  s.split("\\s+")
来源：http://zyi.shangyingyoupin.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://lit.jinyuanbaomall.cn

Ruby: s.split(",");  s.split
来源：http://gie.gaohongyu789.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://aiv.sufxvd.cn

[E08] 数组按分隔符合并
来源：http://rqs.9152youxi.cn

Py:   ",".join(items)
来源：http://kqq.jlsjyb.cn

PHP:  implode(",", $items);
来源：http://gbq.chenjidiqi.icu

JS:   items.join(",")
来源：http://zbl.jinqigufen.top

TS:   items.join(",")
来源：http://vcu.yanxiufei.cn

Java: String.join(",", items)
来源：http://dlj.smart0.xyz

Go:   strings.Join(items, ",")
来源：http://alf.hfpthk.cn

Ruby: items.join(",")
来源：http://ckd.52xcode.cn

C#:   string.Join(",", items)
来源：http://hqn.nanxuanxn.top

[E09] 去除所有空白字符
来源：http://kjd.havefunace.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://lad.jinyuanbaomall.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://mre.dashuyun.cn

JS:   s.replace(/\s+/g, "")
来源：http://tku.52xcode.cn

TS:   s.replace(/\s+/g, "")
来源：http://niz.ywan-chungtsiang.top

Java: s.replaceAll("\\s+", "")
来源：http://itv.havefunace.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://atg.epnwcf.com

Ruby: s.gsub(/\s+/, "")
来源：http://mzb.zhengqikj.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://qym.xuetiantiany.cn

[E10] 左侧补零 / 定长填充
来源：http://tir.aibaodan.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://fmc.hongshengwenyu.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://giw.yongpay.top

JS:   "7".padStart(3, "0")
来源：http://pst.gogol.net.cn

TS:   "7".padStart(3, "0")
来源：http://vrz.chenzaomai.com

Java: String.format("%03d", 7)
来源：http://bmh.ybcxt.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://iba.cqqwz.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://ccz.daxiang520.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://eqm.zhijiandao.cn

[E11] 反转字符串
来源：http://rsv.wangshuangyany.cn

Py:   s[::-1]
来源：http://vyr.daria6918.cn

PHP:  strrev($s);
来源：http://oky.quarkkingdee.top

JS:   [...s].reverse().join("")
来源：http://qei.zdbjq.cn

TS:   [...s].reverse().join("")
来源：http://hvy.zhongyouzk.top

Java: new StringBuilder(s).reverse().toString()
来源：http://rhg.fehbvm.com

Go:   // 转 []rune 后倒序再转回 string
来源：http://rui.gaohongyu789.top

Ruby: s.reverse
来源：http://zho.xziqi.cn

C#:   new string(s.Reverse().ToArray())
来源：http://xrr.xinyue.icu

[E12] 统计某字符出现次数
来源：http://zws.yuanzhike.top

Py:   s.count("a")
来源：http://ptj.fanxiaobao.xyz

PHP:  substr_count($s, "a");
来源：http://kvk.zhijiandao.cn

JS:   s.split("a").length - 1
来源：http://lns.snrcjt.cn

TS:   s.split("a").length - 1
来源：http://avw.daria6918.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://kan.ydzc1.top

Go:   strings.Count(s, "a")
来源：http://kwh.tian-w.cn

Ruby: s.count("a")
来源：http://zin.chenlongwang.top

C#:   s.Count(c => c == 'a')
来源：http://hzd.zhengqikj.top

[E13] 逐字符遍历
来源：http://xhv.zhengqikj.top

Py:   for ch in s: print(ch)
来源：http://qtp.fanxiaobao.xyz

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://bor.hcnkem.com

JS:   for (const ch of s) { console.log(ch); }
来源：http://lwh.sufxvd.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://phh.pengpengdd.cyou


<!-- 参考信息 -->