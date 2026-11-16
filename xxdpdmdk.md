代发 wailian999

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://tiq.zdbjq.cn

Ruby: arr.sort
来源：http://fqr.tian-w.cn

C#:   list.Sort();
来源：http://wyx.uphjek.com

[D10] 自定义排序（按字段 / 多条件）
来源：http://gyc.xuanzx.com

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://jwb.ydzc1.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ofo.cheryme.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://nai.shanyushiyangtech.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hzd.zhijiandao.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://lzg.yj20258888.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://oag.sjlbkw.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://eac.guannengcc.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://tpo.hongshengwenyu.top

[D11] 反转数组
来源：http://uno.hnxiangtu.top

Py:   arr[::-1];  arr.reverse()
来源：http://pdq.gogol.net.cn

PHP:  array_reverse($arr);
来源：http://znf.iojbl.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://nxd.tarul.cn

TS:   [...arr].reverse();
来源：http://pvn.shanyushiyangkeji.top

Java: Collections.reverse(list);
来源：http://urm.ydzc1.top

Go:   slices.Reverse(arr)
来源：http://tho.daxiang520.top

Ruby: arr.reverse
来源：http://oof.ydjk.org.cn

C#:   list.Reverse();
来源：http://sam.xingfuxueyuan.xyz

[D12] 查找元素下标
来源：http://mlh.vqdsnc.cn

Py:   arr.index(x);  x in arr
来源：http://iks.nwbrower.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://yqd.0kj1m.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://qrt.kuanghao11.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://kmn.ivvv.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://jxl.fktsv.cn

Go:   slices.Index(arr, x)
来源：http://bgr.yfazqb.com

Ruby: arr.index(x)
来源：http://txp.fktsv.cn

C#:   list.IndexOf(x);
来源：http://xfr.zhaomingkeji.xyz

[D13] 过滤（保留满足条件的）
来源：http://cbr.nanxinkj.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://ouv.tian-w.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hkg.smart0.xyz

JS:   arr.filter(x => x > 3)
来源：http://xme.svipenyu.cn

TS:   arr.filter(x => x > 3)
来源：http://jug.fanxiaobao.xyz

Java: list.stream().filter(x -> x > 3).toList()
来源：http://ukb.jinqigfzy.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://mud.nwbrower.top

Ruby: arr.select { |x| x > 3 }
来源：http://uuy.jiagoushi.top

C#:   list.Where(x => x > 3).ToList()
来源：http://dzt.ehwqpu.com

[D14] 映射转换（每个元素变形）
来源：http://wjt.zhoulong.xyz

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://xdx.hnqzz.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://ifp.ywan-chungtsiang.top

JS:   arr.map(x => x * 2)
来源：http://cou.ivvv.top

TS:   arr.map(x => x * 2)
来源：http://asy.chenjidiqi.icu

Java: list.stream().map(x -> x * 2).toList()
来源：http://tpx.havefunace.top

Go:   // 手写循环
来源：http://kye.jiagoushi.top

Ruby: arr.map { |x| x * 2 }
来源：http://ksz.yonumen.top

C#:   list.Select(x => x * 2).ToList()
来源：http://qmh.kuanghao11.cn

[D15] 去重
来源：http://qnm.tian-w.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://qjw.aibaodan.cn

PHP:  array_unique($arr);
来源：http://vat.xuetiantiany.cn

JS:   [...new Set(arr)]
来源：http://cae.0kj1m.cn

TS:   [...new Set(arr)]
来源：http://bbx.shanyushiyangkeji.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://qip.cdnleiting.top

Go:   // 用 map[T]struct{} 手写
来源：http://utd.shzxlz.cn

Ruby: arr.uniq
来源：http://pvh.yj20258.top

C#:   list.Distinct().ToList()
来源：http://rjp.mhx1999.top

[D16] 求和与平均值
来源：http://jxg.svipenyu.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://eyl.xuanzx.com

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://koi.ydzc1.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://chk.epnwcf.com

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://rxm.iojbl.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://mch.hnqzz.top

Go:   // 手写循环累加
来源：http://czv.shuidangran.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://sba.zhiwuduotai.top

C#:   list.Sum();  list.Average()
来源：http://rgp.zhiwuduotai.top

[D17] 最大值与最小值
来源：http://pzx.epnwcf.com

Py:   max(arr);  min(arr)
来源：http://xpd.dashuyun.cn

PHP:  max($arr);  min($arr);
来源：http://dgk.cucudq.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://fiz.wangdashe.top

TS:   Math.max(...arr);
来源：http://mty.quarkkingdee.top

Java: Collections.max(list);  Collections.min(list);
来源：http://ftb.zycfv.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://rxm.feifeiyinyue.top

Ruby: arr.max;  arr.min
来源：http://crb.jinghuilouyu.cn

C#:   list.Max();  list.Min()
来源：http://vzx.fzhhl.top

[D18] 扁平化嵌套数组
来源：http://zmt.bjfxy.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://pdj.chenjidiqi.icu

PHP:  array_merge(...$nested);
来源：http://piz.shuidangran.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://zkr.xingfuxueyuan.xyz

TS:   nested.flat();
来源：http://nog.hcnkem.com

Java: nested.stream().flatMap(List::stream).toList()
来源：http://gmh.ydzc1.top

Go:   // 手写双层循环
来源：http://rft.ehwqpu.com

Ruby: nested.flatten
来源：http://lqz.birdmap.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://hfe.guannengcc.top

[D19] 按字段分组
来源：http://exm.ppjwa.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://gyl.bbcook.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://whf.wangdashe.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://ysr.kuanghao11.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://wtu.hnxiangtu.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://okl.yonumen.top

Go:   // 手写 map[string][]T
来源：http://mqx.sweek.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://koe.hammf.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://oje.9152youxi.cn

[D20] 统计每个元素出现次数
来源：http://ymj.quarkkingdee.top

Py:   Counter(arr)
来源：http://iyo.ctjpmb.com

PHP:  array_count_values($arr);
来源：http://fnv.yonumen.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://euk.shanyushiyangtech.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://dmw.cdnleiting.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://ovm.tanke756.top

Go:   // 手写 map[T]int
来源：http://cfi.yueranfly.top

Ruby: arr.tally
来源：http://axd.zdqjudy.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://onn.sweek.top

[D21] 判断是否包含某元素
来源：http://jus.hnqzz.top

Py:   x in arr
来源：http://wlp.fktsv.cn

PHP:  in_array($x, $arr, true);
来源：http://hoy.hesvh.cn

JS:   arr.includes(x)
来源：http://ouk.bjfxy.top

TS:   arr.includes(x)
来源：http://ziw.cqqwz.cn

Java: list.contains(x)
来源：http://twt.316326.xyz

Go:   slices.Contains(arr, x)
来源：http://jov.bbcook.cn

Ruby: arr.include?(x)
来源：http://sfi.tianlin.xyz

C#:   list.Contains(x)
来源：http://twp.guannengcc.top

[D22] 复制数组（避免共享引用）
来源：http://rif.cucudq.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://zoa.dianchejie.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://lxq.xylfe.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hnu.zhengqikj.top

TS:   [...arr];
来源：http://uqf.hfpthk.cn

Java: new ArrayList<>(list);
来源：http://jnv.ivvv.top

Go:   copied := append([]int(nil), arr...)
来源：http://yat.yanxiufei.cn

Ruby: arr.dup;  arr.clone
来源：http://qph.cucudq.cn

C#:   new List<int>(list);
来源：http://tsg.vqdsnc.cn

[D23] reduce 累积计算
来源：http://wzs.yfazqb.com

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://drf.yuanzhike.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://crm.bbcook.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://szi.bbcook.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://lfs.pengpengdd.cyou

Java: list.stream().reduce(0, Integer::sum)
来源：http://qdg.zhengqikj.top

Go:   // 手写循环
来源：http://lej.chenzaomai.com

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://fnw.zhongyouzk.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://reg.epnwcf.com

[D24] 字典 / Map 基本操作
来源：http://sfr.hnqzz.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://ojf.hywenlv.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://bqz.fktsv.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://lwb.tianlin.xyz

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://cld.zhixingplan.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://gyy.jinqigufen.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://sob.ehwqpu.com

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://vbg.gogol.net.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.yuanzhike.top

[D25] Set 集合去重与交并差
来源：http://fou.guannengcc.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://bxn.jianghu66.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://iir.c1oappe.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://qic.sjlbkw.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://dyr.gotoacloud.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://lmw.zhijiandao.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://lwi.chenjidiqi.icu

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://wdv.sysykeji.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://msk.pengpengdd.cyou

[D26] 数组转字符串
来源：http://ouu.hesvh.cn

Py:   ", ".join(map(str, arr))
来源：http://cfh.yvedp.cn

PHP:  implode(", ", $arr);
来源：http://pbm.zdbjq.cn

JS:   arr.join(", ")
来源：http://hyl.ydjk.org.cn

TS:   arr.join(", ")
来源：http://ctp.cashguo.top

Java: String.join(", ", list)
来源：http://tcg.zhijiandao.cn

Go:   strings.Join(strs, ", ")
来源：http://iqn.wangdashe.top

Ruby: arr.join(", ")
来源：http://lyr.guowangkeji.top

C#:   string.Join(", ", list)
来源：http://xre.hywenlv.cn

================================================================================
来源：http://dhu.nwbrower.top

E. 字符串处理
来源：http://pof.jinqigfzy.top

================================================================================
来源：http://egl.tarul.cn

[E01] 拼接字符串
来源：http://jvj.ydjk.org.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://pul.316326.xyz

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://wor.zhongyouzk.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://sec.yanxiufei.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://nyn.sufxvd.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://nzx.aibaodan.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://ekz.hysaishi.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://kct.zhijiandao.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://gxr.dianchejie.cn

[E02] 重复字符串
来源：http://iho.hammf.cn

Py:   "ab" * 3
来源：http://cdw.shanyushiyangkeji.top

PHP:  str_repeat("ab", 3);
来源：http://jof.quarkkingdee.top

JS:   "ab".repeat(3)
来源：http://eec.ivvv.top

TS:   "ab".repeat(3)
来源：http://los.haohaochexian.top

Java: "ab".repeat(3)
来源：http://nxa.zhoulong.xyz

Go:   strings.Repeat("ab", 3)
来源：http://hvs.zhaomingkeji.xyz

Ruby: "ab" * 3
来源：http://rly.ppjwa.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://blw.c1oappe.top

[E03] 截取子串
来源：http://bmd.yueranfly.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://ftv.haohaochexian.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://wyg.yj202588.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://sel.xziqi.cn

TS:   s.slice(1, 4)
来源：http://ccp.bbcook.cn

Java: s.substring(1, 4)
来源：http://wfn.hywenlv.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://yoy.smart0.xyz

Ruby: s[1, 3];  s[1..3]
来源：http://lal.xuetiantiany.cn

C#:   s.Substring(1, 3)
来源：http://jjh.yvedp.cn

[E04] 查找子串位置
来源：http://lcc.tian-w.cn

Py:   s.find("x");  s.index("x")
来源：http://lyo.jinyuanbaomall.cn

PHP:  strpos($s, "x");
来源：http://occ.jinyuanbaomall.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://dcf.zhijiandao.cn

TS:   s.indexOf("x")
来源：http://blq.0kj1m.cn

Java: s.indexOf("x")
来源：http://cyf.bbcook.cn

Go:   strings.Index(s, "x")
来源：http://fuw.jlsjyb.cn

Ruby: s.index("x")
来源：http://lpw.jinghuilouyu.cn

C#:   s.IndexOf("x")
来源：http://tch.yuxming.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://tbr.gzhubu.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://glk.yvedp.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://yht.ivvv.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://bdj.ydjk.org.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://zkx.kuanghao11.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://nwx.zdqjudy.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://ujn.shzxlz.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://xqf.ywan-chungtsiang.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://quh.yfazqb.com

[E06] 替换子串
来源：http://zel.mhx1999.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://eui.jinghuilouyu.cn

PHP:  str_replace("a", "b", $s);
来源：http://ysf.c1oappe.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wgb.zdqjudy.top

TS:   s.replaceAll("a", "b")
来源：http://law.cashguo.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://axj.316326.xyz

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://kaq.havefunace.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://qnt.zhaomingkeji.xyz

C#:   s.Replace("a", "b")
来源：http://bry.haohaochexian.top

[E07] 按分隔符拆分
来源：http://cet.yfazqb.com

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://oyq.yueranfly.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://pzv.epnwcf.com

JS:   s.split(",");  s.split(/\s+/)
来源：http://grj.fktsv.cn

TS:   s.split(",")
来源：http://hor.tianlin.xyz

Java: s.split(",");  s.split("\\s+")
来源：http://fvv.zhaomingkeji.xyz

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://lyv.sufxvd.cn

Ruby: s.split(",");  s.split
来源：http://urt.tanke756.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://ttn.fehbvm.com

[E08] 数组按分隔符合并
来源：http://zqu.chenzaomai.com

Py:   ",".join(items)
来源：http://ote.jyoumei.cn

PHP:  implode(",", $items);
来源：http://rch.cdnleiting.top

JS:   items.join(",")
来源：http://yns.cucudq.cn

TS:   items.join(",")
来源：http://put.zdbjq.cn

Java: String.join(",", items)
来源：http://vnz.yj20258.top

Go:   strings.Join(items, ",")
来源：http://ojc.fehbvm.com

Ruby: items.join(",")
来源：http://csx.havefunace.top

C#:   string.Join(",", items)
来源：http://taa.fanxiaobao.xyz

[E09] 去除所有空白字符
来源：http://gsd.gotoacloud.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://vcj.yvedp.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://wec.jinghuilouyu.cn

JS:   s.replace(/\s+/g, "")
来源：http://css.epnwcf.com

TS:   s.replace(/\s+/g, "")
来源：http://kno.ehwqpu.com

Java: s.replaceAll("\\s+", "")
来源：http://siy.kuanghao11.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://snp.andypj.xyz

Ruby: s.gsub(/\s+/, "")
来源：http://rsv.yj20258888.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://fye.zhijiandao.cn

[E10] 左侧补零 / 定长填充
来源：http://yyi.mhx1999.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://shy.shzxlz.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://cyr.svipenyu.cn

JS:   "7".padStart(3, "0")
来源：http://kxu.jinyuanbaomall.cn

TS:   "7".padStart(3, "0")
来源：http://shy.uphjek.com

Java: String.format("%03d", 7)
来源：http://qnv.cdnleiting.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://gaw.snrcjt.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://kwx.sysykeji.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://srs.ctjpmb.com

[E11] 反转字符串
来源：http://oqo.cashguo.top

Py:   s[::-1]
来源：http://etk.hysaishi.cn

PHP:  strrev($s);
来源：http://yxg.birdmap.top

JS:   [...s].reverse().join("")
来源：http://kwb.jianghu66.top

TS:   [...s].reverse().join("")
来源：http://fiq.xingfuxueyuan.xyz

Java: new StringBuilder(s).reverse().toString()
来源：http://boc.redwolf501.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://vqf.ppjwa.cn

Ruby: s.reverse
来源：http://dix.xziqi.cn

C#:   new string(s.Reverse().ToArray())
来源：http://cwg.fengsongda.top

[E12] 统计某字符出现次数
来源：http://qhq.yj202588.top

Py:   s.count("a")
来源：http://fcu.guowangkeji.top

PHP:  substr_count($s, "a");
来源：http://esp.havefunace.top

JS:   s.split("a").length - 1
来源：http://ckc.yj202588.top

TS:   s.split("a").length - 1
来源：http://ixz.jianghu66.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://gnl.hcnkem.com

Go:   strings.Count(s, "a")
来源：http://tku.wangdashe.top

Ruby: s.count("a")
来源：http://xpn.yonumen.top

C#:   s.Count(c => c == 'a')
来源：http://nsl.gaohongyu789.top

[E13] 逐字符遍历
来源：http://yws.bjfxy.top

Py:   for ch in s: print(ch)
来源：http://xlz.ybcxt.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://mfp.pengpengdd.cyou

JS:   for (const ch of s) { console.log(ch); }
来源：http://rry.pengpengdd.cyou

TS:   for (const ch of s) { console.log(ch); }
来源：http://uwu.zhijiandao.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://qzg.vehdjk.com

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://kik.redwolf501.top

Ruby: s.each_char { |ch| puts ch }
来源：http://wpx.wangshuangyany.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://fyq.snrcjt.cn

[E14] URL 编码与 Base64
来源：http://min.zhixingplan.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://xpq.yj20258.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://sou.yueranfly.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://enj.0kj1m.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://wpo.tianlin.xyz

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://wez.gaohongyu789.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://vxu.sufxvd.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://uhb.ivvv.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://nav.jinghuilouyu.cn

[E15] HTML 转义 / 反转义
来源：http://jqo.shangyingyoupin.top

Py:   html.escape(s);  html.unescape(s)
来源：http://jgz.nanxinkj.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://apb.hywenlv.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://aeq.gogol.net.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://vtx.hywenlv.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://gvb.vehdjk.com

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://vyv.yvedp.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://mxr.0kj1m.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://yqr.vehdjk.com

[E16] 数字千分位
来源：http://wpn.xziqi.cn

Py:   f"{1234567:,}"
来源：http://lbh.vqdsnc.cn

PHP:  number_format(1234567);
来源：http://csm.hfpthk.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://ezk.jlsjyb.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://moo.smart0.xyz

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://fyp.jinghuilouyu.cn


<!-- 参考信息 -->